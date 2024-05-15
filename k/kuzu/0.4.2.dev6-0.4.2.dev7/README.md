# Comparing `tmp/kuzu-0.4.2.dev6.tar.gz` & `tmp/kuzu-0.4.2.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuzu-0.4.2.dev6.tar", last modified: Mon May 13 08:05:04 2024, max compression
+gzip compressed data, was "kuzu-0.4.2.dev7.tar", last modified: Tue May 14 08:04:48 2024, max compression
```

## Comparing `kuzu-0.4.2.dev6.tar` & `kuzu-0.4.2.dev7.tar`

### file list

```diff
@@ -1,2816 +1,2820 @@
-drwx------   0 runner    (1001) docker     (127)        0 2024-05-13 08:05:04.487664 sdist/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-13 08:04:57.031655 sdist/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-13 08:04:58.643657 sdist/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-13 08:04:57.031655 sdist/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-05-13 08:04:58.643657 sdist/README_PYTHON_BUILD.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:05:02.923662 sdist/kuzu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:05:02.923662 sdist/kuzu-source/
--rw-rw-r--   0 runner    (1001) docker     (127)     5560 2024-05-13 08:04:59.000000 sdist/kuzu-source/.clang-format
--rw-rw-r--   0 runner    (1001) docker     (127)      948 2024-05-13 08:04:59.000000 sdist/kuzu-source/.clang-tidy
--rw-rw-r--   0 runner    (1001) docker     (127)      332 2024-05-13 08:04:59.000000 sdist/kuzu-source/.clang-tidy-analyzer
--rw-rw-r--   0 runner    (1001) docker     (127)     1000 2024-05-13 08:04:59.000000 sdist/kuzu-source/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (127)       47 2024-05-13 08:04:59.000000 sdist/kuzu-source/.lcovrc
--rw-rw-r--   0 runner    (1001) docker     (127)     8632 2024-05-13 08:04:59.000000 sdist/kuzu-source/CLA.md
--rw-rw-r--   0 runner    (1001) docker     (127)     9475 2024-05-13 08:04:59.000000 sdist/kuzu-source/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      632 2024-05-13 08:04:59.000000 sdist/kuzu-source/CODE_OF_CONDUCT.md
--rw-rw-r--   0 runner    (1001) docker     (127)     2052 2024-05-13 08:04:59.000000 sdist/kuzu-source/CONTRIBUTING.md
--rw-rw-r--   0 runner    (1001) docker     (127)     1072 2024-05-13 08:04:59.000000 sdist/kuzu-source/LICENSE
--rw-rw-r--   0 runner    (1001) docker     (127)     6896 2024-05-13 08:04:59.000000 sdist/kuzu-source/Makefile
--rw-rw-r--   0 runner    (1001) docker     (127)     3881 2024-05-13 08:04:59.000000 sdist/kuzu-source/README.md
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/scripts/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/scripts/antlr4/
--rw-rw-r--   0 runner    (1001) docker     (127)    26331 2024-05-13 08:04:59.000000 sdist/kuzu-source/scripts/antlr4/Cypher.g4.copy
--rw-rw-r--   0 runner    (1001) docker     (127)     2085 2024-05-13 08:04:59.000000 sdist/kuzu-source/scripts/antlr4/generate_grammar.cmake
--rwxrwxr-x   0 runner    (1001) docker     (127)      299 2024-05-13 08:04:59.000000 sdist/kuzu-source/scripts/check-include-guards.sh
--rwxrwxr-x   0 runner    (1001) docker     (127)       76 2024-05-13 08:04:59.000000 sdist/kuzu-source/scripts/check-no-std-assert.sh
--rwxrwxr-x   0 runner    (1001) docker     (127)     2837 2024-05-13 08:04:59.000000 sdist/kuzu-source/scripts/collect-single-file-header.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/scripts/generate-cpp-docs/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/scripts/generate-cpp-docs/c/
--rw-rw-r--   0 runner    (1001) docker     (127)   126290 2024-05-13 08:04:59.000000 sdist/kuzu-source/scripts/generate-cpp-docs/c/Doxyfile
--rw-rw-r--   0 runner    (1001) docker     (127)     4738 2024-05-13 08:04:59.000000 sdist/kuzu-source/scripts/generate-cpp-docs/collect_files.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/scripts/generate-cpp-docs/cpp/
--rw-rw-r--   0 runner    (1001) docker     (127)   126295 2024-05-13 08:04:59.000000 sdist/kuzu-source/scripts/generate-cpp-docs/cpp/Doxyfile
--rwxrwxr-x   0 runner    (1001) docker     (127)      225 2024-05-13 08:04:59.000000 sdist/kuzu-source/scripts/generate-cpp-docs/doxygen.sh
--rwxrwxr-x   0 runner    (1001) docker     (127)     6998 2024-05-13 08:04:59.000000 sdist/kuzu-source/scripts/get-clangd-diagnostics.py
--rw-rw-r--   0 runner    (1001) docker     (127)      131 2024-05-13 08:04:59.000000 sdist/kuzu-source/scripts/http-server.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/scripts/multiplatform-test-helper/
--rw-rw-r--   0 runner    (1001) docker     (127)     2130 2024-05-13 08:04:59.000000 sdist/kuzu-source/scripts/multiplatform-test-helper/collect-results.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1585 2024-05-13 08:04:59.000000 sdist/kuzu-source/scripts/multiplatform-test-helper/notify-discord.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/scripts/pip-package/
--rw-rw-r--   0 runner    (1001) docker     (127)       37 2024-05-13 08:04:59.000000 sdist/kuzu-source/scripts/pip-package/MANIFEST.in
--rw-rw-r--   0 runner    (1001) docker     (127)     3276 2024-05-13 08:04:59.000000 sdist/kuzu-source/scripts/pip-package/README.md
--rwxrwxr-x   0 runner    (1001) docker     (127)     3277 2024-05-13 08:04:59.000000 sdist/kuzu-source/scripts/pip-package/package_tar.py
--rw-rw-r--   0 runner    (1001) docker     (127)      200 2024-05-13 08:04:59.000000 sdist/kuzu-source/scripts/pip-package/setup.cfg
--rw-rw-r--   0 runner    (1001) docker     (127)     4441 2024-05-13 08:04:59.000000 sdist/kuzu-source/scripts/pip-package/setup.py
--rwxrwxr-x   0 runner    (1001) docker     (127)    12359 2024-05-13 08:04:59.000000 sdist/kuzu-source/scripts/run-clang-format.py
--rw-rw-r--   0 runner    (1001) docker     (127)     3060 2024-05-13 08:04:59.000000 sdist/kuzu-source/scripts/update-nightly-build-version.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/
--rw-rw-r--   0 runner    (1001) docker     (127)     2644 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/antlr4/
--rw-rw-r--   0 runner    (1001) docker     (127)    26331 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/antlr4/Cypher.g4
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/
--rw-rw-r--   0 runner    (1001) docker     (127)      519 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind/
--rw-rw-r--   0 runner    (1001) docker     (127)      766 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      441 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind/bind_attach_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      740 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind/bind_comment_on.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1323 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind/bind_create_macro.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    18633 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind/bind_ddl.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      437 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind/bind_detach_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      518 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind/bind_explain.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6114 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind/bind_export_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2074 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind/bind_extension.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5297 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind/bind_file_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    32965 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind/bind_graph_pattern.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3512 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind/bind_import_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11898 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind/bind_projection_clause.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4787 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind/bind_query.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      702 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind/bind_reading_clause.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1515 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind/bind_standalone_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      566 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind/bind_transaction.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    17249 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind/bind_updating_clause.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      415 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind/bind_use_database.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind/copy/
--rw-rw-r--   0 runner    (1001) docker     (127)      246 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind/copy/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    10625 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind/copy/bind_copy_from.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8100 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind/copy/bind_copy_rdf_graph.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1613 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind/copy/bind_copy_to.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind/ddl/
--rw-rw-r--   0 runner    (1001) docker     (127)      194 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind/ddl/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     3534 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind/ddl/bind_create_rdf_graph.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind/read/
--rw-rw-r--   0 runner    (1001) docker     (127)      267 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind/read/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     3209 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind/read/bind_in_query_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5724 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind/read/bind_load_from.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3009 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind/read/bind_match.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2013 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind/read/bind_unwind.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind_expression/
--rw-rw-r--   0 runner    (1001) docker     (127)      555 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind_expression/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2202 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind_expression/bind_boolean_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3488 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind_expression/bind_case_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3118 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind_expression/bind_comparison_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    14939 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind_expression/bind_function_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1284 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind_expression/bind_literal_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1677 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind_expression/bind_null_operator_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      928 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind_expression/bind_parameter_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5159 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind_expression/bind_property_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3195 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind_expression/bind_subquery_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1531 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bind_expression/bind_variable_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8045 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/binder.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/binder_scope.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      567 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bound_statement_result.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      801 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bound_statement_rewriter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5524 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/bound_statement_visitor.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/expression/
--rw-rw-r--   0 runner    (1001) docker     (127)      380 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/expression/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      498 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/expression/case_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      764 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/expression/expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11104 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/expression/expression_util.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1438 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/expression/function_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      672 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/expression/literal_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      575 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/expression/parameter_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      549 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/expression/variable_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5234 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/expression_binder.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6353 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/expression_visitor.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/query/
--rw-rw-r--   0 runner    (1001) docker     (127)      350 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/query/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      707 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/query/bound_delete_clause.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      707 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/query/bound_insert_clause.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1963 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/query/bound_merge_clause.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      718 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/query/bound_set_clause.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9670 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/query/query_graph.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6621 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/query/query_graph_label_analyzer.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/rewriter/
--rw-rw-r--   0 runner    (1001) docker     (127)      261 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/rewriter/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      742 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/rewriter/match_clause_pattern_label_rewriter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2547 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/rewriter/with_clause_projection_rewriter.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/visitor/
--rw-rw-r--   0 runner    (1001) docker     (127)      230 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/visitor/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      638 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/visitor/default_type_solver.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4801 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/binder/visitor/property_collector.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/c_api/
--rw-rw-r--   0 runner    (1001) docker     (127)      369 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/c_api/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     4034 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/c_api/connection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2653 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/c_api/data_type.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1122 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/c_api/database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1412 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/c_api/flat_tuple.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      286 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/c_api/helpers.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7617 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/c_api/prepared_statement.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4402 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/c_api/query_result.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      745 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/c_api/query_summary.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    19821 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/c_api/value.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      271 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/c_api/version.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/catalog/
--rw-rw-r--   0 runner    (1001) docker     (127)      242 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/catalog/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    19856 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/catalog/catalog.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/catalog/catalog_entry/
--rw-rw-r--   0 runner    (1001) docker     (127)      464 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/catalog/catalog_entry/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1366 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/catalog/catalog_entry/catalog_entry.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/catalog/catalog_entry/catalog_entry_type.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      357 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/catalog/catalog_entry/function_catalog_entry.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2516 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/catalog/catalog_entry/node_table_catalog_entry.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5183 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/catalog/catalog_entry/rdf_graph_catalog_entry.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3770 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/catalog/catalog_entry/rel_group_catalog_entry.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4535 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/catalog/catalog_entry/rel_table_catalog_entry.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1063 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/catalog/catalog_entry/scalar_macro_catalog_entry.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6589 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/catalog/catalog_entry/table_catalog_entry.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8047 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/catalog/catalog_set.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1605 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/catalog/property.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/
--rw-rw-r--   0 runner    (1001) docker     (127)      803 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/arrow/
--rw-rw-r--   0 runner    (1001) docker     (127)      295 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/arrow/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    24685 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/arrow/arrow_array_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    10576 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/arrow/arrow_converter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8673 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/arrow/arrow_null_mask_tree.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    35459 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/arrow/arrow_row_batch.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5340 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/arrow/arrow_type.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      478 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/case_insensitive_map.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      106 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/constants.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/copier_config/
--rw-rw-r--   0 runner    (1001) docker     (127)      256 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/copier_config/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     3078 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/copier_config/csv_reader_config.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/copier_config/rdf_reader_config.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1727 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/copier_config/reader_config.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/data_chunk/
--rw-rw-r--   0 runner    (1001) docker     (127)      250 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/data_chunk/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      470 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/data_chunk/data_chunk.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2669 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/data_chunk/data_chunk_collection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    12601 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/data_chunk/data_chunk_state.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/enums/
--rw-rw-r--   0 runner    (1001) docker     (127)      258 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/enums/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1050 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/enums/path_semantic.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      413 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/enums/rel_direction.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1069 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/enums/rel_multiplicity.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      642 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/enums/table_type.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/exception/
--rw-rw-r--   0 runner    (1001) docker     (127)      316 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/exception/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      377 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/exception/exception.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2665 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/exception/message.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3201 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/expression_type.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/file_system/
--rw-rw-r--   0 runner    (1001) docker     (127)      306 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/file_system/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      999 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/file_system/file_info.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1255 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/file_system/file_system.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    15054 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/file_system/local_file_system.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2708 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/file_system/virtual_file_system.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      977 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/in_mem_overflow_buffer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/keyword_utils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8157 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/md5.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      995 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/metric.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8989 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/null_mask.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1452 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/profiler.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      349 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/random_engine.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/serializer/
--rw-rw-r--   0 runner    (1001) docker     (127)      270 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/serializer/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2842 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/serializer/buffered_file.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      948 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/serializer/buffered_serializer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      347 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/serializer/deserializer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      356 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/serializer/serializer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1355 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/sha256.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/signal/
--rw-rw-r--   0 runner    (1001) docker     (127)      182 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/signal/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1027 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/signal/register.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5079 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/string_utils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      884 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/system_message.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/task_system/
--rw-rw-r--   0 runner    (1001) docker     (127)      236 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/task_system/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2748 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/task_system/progress_bar.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      772 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/task_system/task.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4596 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/task_system/task_scheduler.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9750 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/type_utils.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/types/
--rw-rw-r--   0 runner    (1001) docker     (127)      406 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/types/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     4494 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/types/blob.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    19741 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/types/date_t.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6196 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/types/dtime_t.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    19061 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/types/int128_t.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1174 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/types/internal_id_t.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    17620 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/types/interval_t.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      832 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/types/ku_list.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2364 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/types/ku_string.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11000 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/types/timestamp_t.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    58160 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/types/types.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4363 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/types/uuid.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/types/value/
--rw-rw-r--   0 runner    (1001) docker     (127)      286 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/types/value/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      512 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/types/value/nested.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2379 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/types/value/node.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      354 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/types/value/rdf_variant.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      840 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/types/value/recursive_rel.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2759 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/types/value/rel.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    35482 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/types/value/value.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1298 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/utils.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/vector/
--rw-rw-r--   0 runner    (1001) docker     (127)      210 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/vector/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     3332 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/vector/auxiliary_buffer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    28656 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/vector/value_vector.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1261 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/common/windows_utils.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/expression_evaluator/
--rw-rw-r--   0 runner    (1001) docker     (127)      420 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/expression_evaluator/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     4528 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/expression_evaluator/case_evaluator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      965 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/expression_evaluator/expression_evaluator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      849 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/expression_evaluator/expression_evaluator_utils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3322 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/expression_evaluator/function_evaluator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1063 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/expression_evaluator/literal_evaluator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1545 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/expression_evaluator/node_rel_evaluator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9731 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/expression_evaluator/path_evaluator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1280 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/expression_evaluator/reference_evaluator.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/extension/
--rw-rw-r--   0 runner    (1001) docker     (127)      200 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/extension/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      239 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/extension/catalog_extension.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3182 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/extension/extension.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/
--rw-rw-r--   0 runner    (1001) docker     (127)     1240 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/aggregate/
--rw-rw-r--   0 runner    (1001) docker     (127)      227 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/aggregate/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     3920 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/aggregate/collect.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1835 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/aggregate/count.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1044 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/aggregate/count_star.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    12187 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/aggregate_function.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/arithmetic/
--rw-rw-r--   0 runner    (1001) docker     (127)      299 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/arithmetic/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2611 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/arithmetic/abs.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5505 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/arithmetic/add.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5953 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/arithmetic/divide.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4379 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/arithmetic/modulo.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8121 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/arithmetic/multiply.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2427 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/arithmetic/negate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5848 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/arithmetic/subtract.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/array/
--rw-rw-r--   0 runner    (1001) docker     (127)      210 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/array/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     7204 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/array/array_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1328 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/array/array_value.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2494 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/base_lower_upper_operation.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    20338 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/built_in_function_utils.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/cast/
--rw-rw-r--   0 runner    (1001) docker     (127)      208 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/cast/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     5428 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/cast/cast_array.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11953 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/cast/cast_rdf_variant.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    33750 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/cast_from_string_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2442 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/cast_string_non_nested_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8637 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/comparison_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5169 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/find_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      517 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    12742 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/function_collection.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/list/
--rw-rw-r--   0 runner    (1001) docker     (127)      711 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/list/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2745 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/list/list_agg_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1855 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/list/list_any_value_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2618 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/list/list_append_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2166 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/list/list_concat_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1580 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/list/list_contains_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2146 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/list/list_creation.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1882 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/list/list_distinct_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2189 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/list/list_extract_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1184 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/list/list_position_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2488 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/list/list_prepend_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3640 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/list/list_range_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1561 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/list/list_reverse_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3355 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/list/list_slice_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3684 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/list/list_sort_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1898 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/list/list_to_string_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2240 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/list/list_unique_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1904 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/list/size_function.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/map/
--rw-rw-r--   0 runner    (1001) docker     (127)      283 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/map/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1091 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/map/map_creation_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1670 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/map/map_extract_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      961 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/map/map_keys_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      953 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/map/map_values_function.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/path/
--rw-rw-r--   0 runner    (1001) docker     (127)      299 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/path/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2255 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/path/length_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1144 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/path/nodes_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3841 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/path/properties_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1164 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/path/rels_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1997 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/path/semantic_function.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/pattern/
--rw-rw-r--   0 runner    (1001) docker     (127)      186 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/pattern/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1775 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/pattern/id_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2683 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/scalar_macro_function.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/struct/
--rw-rw-r--   0 runner    (1001) docker     (127)      229 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/struct/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2617 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/struct/struct_extract_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3356 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/struct/struct_pack_function.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/table/
--rw-rw-r--   0 runner    (1001) docker     (127)      218 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/table/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/table/call/
--rw-rw-r--   0 runner    (1001) docker     (127)      360 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/table/call/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1542 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/table/call/checkpoint.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2232 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/table/call/current_setting.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1376 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/table/call/db_version.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2672 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/table/call/show_attached_databases.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5816 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/table/call/show_connection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4202 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/table/call/show_tables.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11070 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/table/call/storage_info.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5471 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/table/call/table_info.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1139 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/table/call_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      364 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/table/scan_functions.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/union/
--rw-rw-r--   0 runner    (1001) docker     (127)      257 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/union/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      628 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/union/union_extract_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      817 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/union/union_tag_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1873 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/union/union_value_function.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/utility/
--rw-rw-r--   0 runner    (1001) docker     (127)      324 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/utility/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     3471 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/utility/coalesce.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3205 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/utility/constant_or_null.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1277 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/utility/count_if.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      870 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/utility/error.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      892 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/utility/md5.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1455 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/utility/nullif.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      950 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/utility/sha256.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1576 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/utility/typeof.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    18396 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/vector_arithmetic_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1389 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/vector_blob_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4267 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/vector_boolean_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    47661 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/vector_cast_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4887 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/vector_date_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9214 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/vector_hash_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      888 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/vector_node_rel_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1516 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/vector_null_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      913 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/vector_rdf_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    14505 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/vector_string_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1205 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/vector_timestamp_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      552 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/function/vector_uuid_functions.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/
--rw-rw-r--   0 runner    (1001) docker     (127)    12753 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/binder.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2756 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/binder_scope.h
--rw-rw-r--   0 runner    (1001) docker     (127)      605 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/bound_attach_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      862 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/bound_comment_on.h
--rw-rw-r--   0 runner    (1001) docker     (127)      842 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/bound_create_macro.h
--rw-rw-r--   0 runner    (1001) docker     (127)      514 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/bound_database_statement.h
--rw-rw-r--   0 runner    (1001) docker     (127)      365 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/bound_detach_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      891 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/bound_explain.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1874 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/bound_export_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      713 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/bound_extension_statement.h
--rw-rw-r--   0 runner    (1001) docker     (127)      877 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/bound_import_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2466 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/bound_scan_source.h
--rw-rw-r--   0 runner    (1001) docker     (127)      790 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/bound_standalone_call.h
--rw-rw-r--   0 runner    (1001) docker     (127)      856 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/bound_statement.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1001 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/bound_statement_result.h
--rw-rw-r--   0 runner    (1001) docker     (127)      348 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/bound_statement_rewriter.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2666 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/bound_statement_visitor.h
--rw-rw-r--   0 runner    (1001) docker     (127)      661 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/bound_transaction_statement.h
--rw-rw-r--   0 runner    (1001) docker     (127)      356 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/bound_use_database.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/copy/
--rw-rw-r--   0 runner    (1001) docker     (127)     3164 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/copy/bound_copy_from.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1071 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/copy/bound_copy_to.h
--rw-rw-r--   0 runner    (1001) docker     (127)      813 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/copy/bound_file_scan_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1014 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/copy/index_look_up_info.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/ddl/
--rw-rw-r--   0 runner    (1001) docker     (127)      530 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/ddl/bound_alter.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3438 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/ddl/bound_alter_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)      574 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/ddl/bound_create_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5837 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/ddl/bound_create_table_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)      664 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/ddl/bound_drop_table.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/expression/
--rw-rw-r--   0 runner    (1001) docker     (127)     1468 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/expression/case_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4768 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/expression/expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2418 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/expression/expression_util.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4539 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/expression/function_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)      832 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/expression/literal_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)      786 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/expression/node_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4286 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/expression/node_rel_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)      918 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/expression/parameter_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1129 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/expression/path_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2561 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/expression/property_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4586 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/expression/rel_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2112 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/expression/subquery_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)      833 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/expression/variable_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5949 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/expression_binder.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2678 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/expression_visitor.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/query/
--rw-rw-r--   0 runner    (1001) docker     (127)     1069 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/query/bound_regular_query.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2487 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/query/normalized_query_part.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1013 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/query/normalized_single_query.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6508 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/query/query_graph.h
--rw-rw-r--   0 runner    (1001) docker     (127)      572 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/query/query_graph_label_analyzer.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/
--rw-rw-r--   0 runner    (1001) docker     (127)     1225 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_in_query_call.h
--rw-rw-r--   0 runner    (1001) docker     (127)      482 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_load_from.h
--rw-rw-r--   0 runner    (1001) docker     (127)      813 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_match_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1010 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_reading_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      869 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_unwind_clause.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/query/return_with_clause/
--rw-rw-r--   0 runner    (1001) docker     (127)     3072 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/query/return_with_clause/bound_projection_body.h
--rw-rw-r--   0 runner    (1001) docker     (127)      923 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/query/return_with_clause/bound_return_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      687 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/query/return_with_clause/bound_with_clause.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/
--rw-rw-r--   0 runner    (1001) docker     (127)     1445 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_delete_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      871 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_delete_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1470 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_insert_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1520 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_insert_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5606 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_merge_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1570 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_set_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      797 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_set_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)      424 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_updating_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      163 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/update_table_type.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/rewriter/
--rw-rw-r--   0 runner    (1001) docker     (127)      515 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/rewriter/match_clause_pattern_label_rewriter.h
--rw-rw-r--   0 runner    (1001) docker     (127)      693 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/rewriter/with_clause_projection_rewriter.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/visitor/
--rw-rw-r--   0 runner    (1001) docker     (127)      781 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/visitor/default_type_solver.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1211 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/binder/visitor/property_collector.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/c_api/
--rw-rw-r--   0 runner    (1001) docker     (127)       86 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/c_api/helpers.h
--rw-rw-r--   0 runner    (1001) docker     (127)    50669 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/c_api/kuzu.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/catalog/
--rw-rw-r--   0 runner    (1001) docker     (127)     6432 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/catalog/catalog.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/
--rw-rw-r--   0 runner    (1001) docker     (127)     3000 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/catalog_entry.h
--rw-rw-r--   0 runner    (1001) docker     (127)      575 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/catalog_entry_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      575 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/dummy_catalog_entry.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1286 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/function_catalog_entry.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2690 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/node_table_catalog_entry.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2482 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/rdf_graph_catalog_entry.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1720 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/rel_group_catalog_entry.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2482 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/rel_table_catalog_entry.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1392 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/scalar_macro_catalog_entry.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3749 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/table_catalog_entry.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2385 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/catalog/catalog_set.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1894 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/catalog/property.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/
--rw-rw-r--   0 runner    (1001) docker     (127)      975 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/api.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/arrow/
--rw-rw-r--   0 runner    (1001) docker     (127)     1542 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/arrow/arrow.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1943 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/arrow/arrow_buffer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1862 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/arrow/arrow_converter.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1449 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/arrow/arrow_nullmask_tree.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2921 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/arrow/arrow_row_batch.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1245 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/assert.h
--rw-rw-r--   0 runner    (1001) docker     (127)      578 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/case_insensitive_map.h
--rw-rw-r--   0 runner    (1001) docker     (127)      559 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/cast.h
--rw-rw-r--   0 runner    (1001) docker     (127)      178 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/column_data_format.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4183 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/concurrent_vector.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9441 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/constants.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/copier_config/
--rw-rw-r--   0 runner    (1001) docker     (127)     1633 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/copier_config/csv_reader_config.h
--rw-rw-r--   0 runner    (1001) docker     (127)      468 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/copier_config/rdf_reader_config.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1302 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/copier_config/reader_config.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3648 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/copy_constructors.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/data_chunk/
--rw-rw-r--   0 runner    (1001) docker     (127)     1576 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/data_chunk/data_chunk.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1261 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/data_chunk/data_chunk_collection.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2116 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/data_chunk/data_chunk_state.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2155 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/data_chunk/sel_vector.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/enums/
--rw-rw-r--   0 runner    (1001) docker     (127)      246 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/enums/alter_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      575 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/enums/clause_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      194 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/enums/conflict_action.h
--rw-rw-r--   0 runner    (1001) docker     (127)      194 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/enums/delete_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      192 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/enums/explain_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1203 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/enums/expression_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      285 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/enums/join_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      364 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/enums/path_semantic.h
--rw-rw-r--   0 runner    (1001) docker     (127)      402 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/enums/query_rel_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      300 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/enums/rel_direction.h
--rw-rw-r--   0 runner    (1001) docker     (127)      359 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/enums/rel_multiplicity.h
--rw-rw-r--   0 runner    (1001) docker     (127)      195 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/enums/scan_source_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      521 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/enums/statement_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      164 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/enums/subquery_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      431 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/enums/table_type.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/exception/
--rw-rw-r--   0 runner    (1001) docker     (127)      302 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/exception/binder.h
--rw-rw-r--   0 runner    (1001) docker     (127)      332 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/exception/buffer_manager.h
--rw-rw-r--   0 runner    (1001) docker     (127)      305 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/exception/catalog.h
--rw-rw-r--   0 runner    (1001) docker     (127)      287 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/exception/connection.h
--rw-rw-r--   0 runner    (1001) docker     (127)      321 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/exception/conversion.h
--rw-rw-r--   0 runner    (1001) docker     (127)      296 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/exception/copy.h
--rw-rw-r--   0 runner    (1001) docker     (127)      403 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/exception/exception.h
--rw-rw-r--   0 runner    (1001) docker     (127)      294 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/exception/extension.h
--rw-rw-r--   0 runner    (1001) docker     (127)      283 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/exception/internal.h
--rw-rw-r--   0 runner    (1001) docker     (127)      274 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/exception/interrupt.h
--rw-rw-r--   0 runner    (1001) docker     (127)      265 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/exception/io.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1260 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/exception/message.h
--rw-rw-r--   0 runner    (1001) docker     (127)      295 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/exception/not_implemented.h
--rw-rw-r--   0 runner    (1001) docker     (127)      307 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/exception/overflow.h
--rw-rw-r--   0 runner    (1001) docker     (127)      365 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/exception/parser.h
--rw-rw-r--   0 runner    (1001) docker     (127)      305 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/exception/runtime.h
--rw-rw-r--   0 runner    (1001) docker     (127)      305 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/exception/storage.h
--rw-rw-r--   0 runner    (1001) docker     (127)      263 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/exception/test.h
--rw-rw-r--   0 runner    (1001) docker     (127)      303 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/exception/transaction_manager.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/file_system/
--rw-rw-r--   0 runner    (1001) docker     (127)     1066 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/file_system/file_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2358 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/file_system/file_system.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2019 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/file_system/local_file_system.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1796 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/file_system/virtual_file_system.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1863 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/in_mem_overflow_buffer.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/keyword/
--rw-rw-r--   0 runner    (1001) docker     (127)     1576 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/keyword/rdf_keyword.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3271 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/md5.h
--rw-rw-r--   0 runner    (1001) docker     (127)      745 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/metric.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3921 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/mpsc_queue.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1346 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/mutex.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1155 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/null_buffer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9142 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/null_mask.h
--rw-rw-r--   0 runner    (1001) docker     (127)      702 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/profiler.h
--rw-rw-r--   0 runner    (1001) docker     (127)      349 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/random_engine.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/serializer/
--rw-rw-r--   0 runner    (1001) docker     (127)     1366 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/serializer/buffered_file.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1716 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/serializer/buffered_serializer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2495 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/serializer/deserializer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      264 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/serializer/reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2467 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/serializer/serializer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      237 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/serializer/writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      557 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/sha256.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2229 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/static_vector.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3858 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/string_format.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4653 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/string_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)      596 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/system_message.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/task_system/
--rw-rw-r--   0 runner    (1001) docker     (127)     1469 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/task_system/progress_bar.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3420 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/task_system/task.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3059 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/task_system/task_scheduler.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1205 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/timer.h
--rw-rw-r--   0 runner    (1001) docker     (127)    11129 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/type_utils.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/types/
--rw-rw-r--   0 runner    (1001) docker     (127)     1666 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/types/blob.h
--rw-rw-r--   0 runner    (1001) docker     (127)    10927 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/types/cast_helpers.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4563 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/types/date_t.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2446 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/types/dtime_t.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6090 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/types/int128_t.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1167 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/types/internal_id_t.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4658 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/types/interval_t.h
--rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/types/ku_list.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2887 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/types/ku_string.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4667 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/types/timestamp_t.h
--rw-rw-r--   0 runner    (1001) docker     (127)    19500 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/types/types.h
--rw-rw-r--   0 runner    (1001) docker     (127)      940 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/types/uuid.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/types/value/
--rw-rw-r--   0 runner    (1001) docker     (127)      319 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/types/value/nested.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1670 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/types/value/node.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1145 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/types/value/rdf_variant.h
--rw-rw-r--   0 runner    (1001) docker     (127)      635 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/types/value/recursive_rel.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1968 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/types/value/rel.h
--rw-rw-r--   0 runner    (1001) docker     (127)    21563 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/types/value/value.h
--rw-rw-r--   0 runner    (1001) docker     (127)      782 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/utils.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/vector/
--rw-rw-r--   0 runner    (1001) docker     (127)     3218 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/vector/auxiliary_buffer.h
--rw-rw-r--   0 runner    (1001) docker     (127)    13651 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/vector/value_vector.h
--rw-rw-r--   0 runner    (1001) docker     (127)      298 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/common/windows_utils.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/expression_evaluator/
--rw-rw-r--   0 runner    (1001) docker     (127)     2419 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/expression_evaluator/case_evaluator.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1382 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/expression_evaluator/expression_evaluator.h
--rw-rw-r--   0 runner    (1001) docker     (127)      433 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/expression_evaluator/expression_evaluator_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1267 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/expression_evaluator/function_evaluator.h
--rw-rw-r--   0 runner    (1001) docker     (127)      871 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/expression_evaluator/literal_evaluator.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1399 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/expression_evaluator/node_rel_evaluator.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2884 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/expression_evaluator/path_evaluator.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1082 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/expression_evaluator/reference_evaluator.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/extension/
--rw-rw-r--   0 runner    (1001) docker     (127)      288 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/extension/catalog_extension.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1491 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/extension/extension.h
--rw-rw-r--   0 runner    (1001) docker     (127)      193 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/extension/extension_action.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/aggregate/
--rw-rw-r--   0 runner    (1001) docker     (127)     3518 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/aggregate/avg.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1139 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/aggregate/base_count.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2409 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/aggregate/collect.h
--rw-rw-r--   0 runner    (1001) docker     (127)      821 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/aggregate/count.h
--rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/aggregate/count_star.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4091 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/aggregate/min_max.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2903 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/aggregate/sum.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6996 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/aggregate_function.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/arithmetic/
--rw-rw-r--   0 runner    (1001) docker     (127)      740 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/arithmetic/abs.h
--rw-rw-r--   0 runner    (1001) docker     (127)      930 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/arithmetic/add.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5133 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/arithmetic/arithmetic_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      957 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/arithmetic/divide.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1109 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/arithmetic/modulo.h
--rw-rw-r--   0 runner    (1001) docker     (127)      975 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/arithmetic/multiply.h
--rw-rw-r--   0 runner    (1001) docker     (127)      520 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/arithmetic/negate.h
--rw-rw-r--   0 runner    (1001) docker     (127)      975 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/arithmetic/subtract.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4696 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/arithmetic/vector_arithmetic_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/array/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/array/functions/
--rw-rw-r--   0 runner    (1001) docker     (127)     1096 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/array/functions/array_cosine_similarity.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1078 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/array/functions/array_cross_product.h
--rw-rw-r--   0 runner    (1001) docker     (127)      824 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/array/functions/array_distance.h
--rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/array/functions/array_inner_product.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2034 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/array/vector_array_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)    24872 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/binary_function_executor.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/blob/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/blob/functions/
--rw-rw-r--   0 runner    (1001) docker     (127)      828 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/blob/functions/decode_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      402 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/blob/functions/encode_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      269 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/blob/functions/octet_length_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      506 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/blob/vector_blob_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/boolean/
--rw-rw-r--   0 runner    (1001) docker     (127)    15040 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/boolean/boolean_function_executor.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4678 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/boolean/boolean_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2493 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/boolean/vector_boolean_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3911 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/built_in_function_utils.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/cast/
--rw-rw-r--   0 runner    (1001) docker     (127)      674 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/cast/cast_function_bind_data.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/cast/functions/
--rw-rw-r--   0 runner    (1001) docker     (127)      539 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_array.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7564 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_from_string_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)    13672 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      993 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_rdf_variant.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7994 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_string_non_nested_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5149 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/cast/functions/numeric_cast.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1795 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/cast/functions/numeric_limits.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3693 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/cast/vector_cast_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/comparison/
--rw-rw-r--   0 runner    (1001) docker     (127)     2928 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/comparison/comparison_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)    10062 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/comparison/vector_comparison_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      509 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/const_function_executor.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/date/
--rw-rw-r--   0 runner    (1001) docker     (127)     4625 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/date/date_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1236 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/date/vector_date_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2897 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      455 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/function_collection.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/hash/
--rw-rw-r--   0 runner    (1001) docker     (127)     6058 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/hash/hash_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      945 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/hash/vector_hash_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/interval/
--rw-rw-r--   0 runner    (1001) docker     (127)     1758 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/interval/interval_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2341 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/interval/vector_interval_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/list/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/list/functions/
--rw-rw-r--   0 runner    (1001) docker     (127)     3521 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/list/functions/base_list_sort_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/list/functions/list_concat_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1987 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/list/functions/list_extract_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1051 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/list/functions/list_len_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1206 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/list/functions/list_position_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1309 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/list/functions/list_reverse_sort_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1312 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/list/functions/list_sort_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      436 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/list/functions/list_to_string_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1231 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/list/functions/list_unique_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3221 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/list/vector_list_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/map/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/map/functions/
--rw-rw-r--   0 runner    (1001) docker     (127)      872 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/map/functions/base_map_extract_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2268 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/map/functions/map_creation_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1515 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/map/functions/map_extract_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      658 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/map/functions/map_keys_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      712 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/map/functions/map_values_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/map/vector_map_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/null/
--rw-rw-r--   0 runner    (1001) docker     (127)     2749 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/null/null_function_executor.h
--rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/null/null_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1154 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/null/vector_null_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/path/
--rw-rw-r--   0 runner    (1001) docker     (127)     6247 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/path/path_function_executor.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1133 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/path/vector_path_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      789 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/pointer_function_executor.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/rdf/
--rw-rw-r--   0 runner    (1001) docker     (127)     1299 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/rdf/rdf_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      393 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/rdf/vector_rdf_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      982 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/rewrite_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)    10274 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/scalar_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1403 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/scalar_macro_function.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/schema/
--rw-rw-r--   0 runner    (1001) docker     (127)      649 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/schema/label_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      258 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/schema/offset_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      642 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/schema/vector_label_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      529 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/schema/vector_node_rel_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/string/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/string/functions/
--rw-rw-r--   0 runner    (1001) docker     (127)     2242 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/string/functions/array_extract_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      669 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/string/functions/base_lower_upper_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2303 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/string/functions/base_pad_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      809 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/string/functions/base_regexp_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      429 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/string/functions/base_str_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/string/functions/contains_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      450 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/string/functions/ends_with_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1459 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/string/functions/find_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      575 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/string/functions/initcap_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      656 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/string/functions/left_operation.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1738 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/string/functions/levenshtein_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      444 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/string/functions/lower_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1035 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/string/functions/lpad_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      765 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/string/functions/ltrim_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      874 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/string/functions/pad_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3067 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_extract_all_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1778 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_extract_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      476 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_full_match_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      477 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_matches_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      710 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_replace_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      640 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/string/functions/repeat_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      570 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/string/functions/reverse_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      673 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/string/functions/right_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1035 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/string/functions/rpad_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      664 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/string/functions/rtrim_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      401 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/string/functions/starts_with_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2808 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/string/functions/substr_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      587 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/string/functions/trim_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      509 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/string/functions/upper_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5537 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/string/vector_string_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/struct/
--rw-rw-r--   0 runner    (1001) docker     (127)     1383 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/struct/vector_struct_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/table/
--rw-rw-r--   0 runner    (1001) docker     (127)     1702 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/table/bind_data.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1905 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/table/bind_input.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3069 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/table/call_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1322 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/table/scan_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      527 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/table/scan_replacement.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4127 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/table_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)    21690 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/ternary_function_executor.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/timestamp/
--rw-rw-r--   0 runner    (1001) docker     (127)     1036 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/timestamp/timestamp_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      508 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/timestamp/vector_timestamp_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)    10907 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/udf_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7851 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/unary_function_executor.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/union/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/union/functions/
--rw-rw-r--   0 runner    (1001) docker     (127)     1234 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/union/functions/union_tag.h
--rw-rw-r--   0 runner    (1001) docker     (127)      519 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/union/vector_union_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/utility/
--rw-rw-r--   0 runner    (1001) docker     (127)      348 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/utility/function_string_bind_data.h
--rw-rw-r--   0 runner    (1001) docker     (127)      999 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/utility/vector_utility_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/uuid/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/uuid/functions/
--rw-rw-r--   0 runner    (1001) docker     (127)      438 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/uuid/functions/gen_random_uuid.h
--rw-rw-r--   0 runner    (1001) docker     (127)      266 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/function/uuid/vector_uuid_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/main/
--rw-rw-r--   0 runner    (1001) docker     (127)     1290 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/main/attached_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1450 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/main/client_config.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6973 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/main/client_context.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7803 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/main/connection.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5111 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/main/database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      812 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/main/database_manager.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1851 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/main/db_config.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1394 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/main/kuzu.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1130 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/main/kuzu_fwd.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3470 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/main/plan_printer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1682 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/main/prepared_statement.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4968 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/main/query_result.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1015 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/main/query_summary.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6918 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/main/settings.h
--rw-rw-r--   0 runner    (1001) docker     (127)      839 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/main/storage_driver.h
--rw-rw-r--   0 runner    (1001) docker     (127)      528 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/main/version.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/optimizer/
--rw-rw-r--   0 runner    (1001) docker     (127)     2295 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/optimizer/acc_hash_join_optimizer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      821 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/optimizer/agg_key_dependency_optimizer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      895 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/optimizer/correlated_subquery_unnest_solver.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2050 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/optimizer/factorization_rewriter.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3621 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/optimizer/filter_push_down_optimizer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1376 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/optimizer/logical_operator_collector.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6889 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/optimizer/logical_operator_visitor.h
--rw-rw-r--   0 runner    (1001) docker     (127)      298 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/optimizer/optimizer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2461 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/optimizer/projection_push_down_optimizer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      572 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/optimizer/remove_factorization_rewriter.h
--rw-rw-r--   0 runner    (1001) docker     (127)      940 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/optimizer/remove_unnecessary_join_optimizer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      556 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/optimizer/top_k_optimizer.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/antlr_parser/
--rw-rw-r--   0 runner    (1001) docker     (127)      895 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/antlr_parser/kuzu_cypher_parser.h
--rw-rw-r--   0 runner    (1001) docker     (127)      620 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/antlr_parser/parser_error_listener.h
--rw-rw-r--   0 runner    (1001) docker     (127)      373 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/antlr_parser/parser_error_strategy.h
--rw-rw-r--   0 runner    (1001) docker     (127)      468 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/attach_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      541 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/comment_on.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1793 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/copy.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1237 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/create_macro.h
--rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/database_statement.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/ddl/
--rw-rw-r--   0 runner    (1001) docker     (127)      397 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/ddl/alter.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1748 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/ddl/alter_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)      447 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/ddl/create_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1782 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/ddl/create_table_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/ddl/drop.h
--rw-rw-r--   0 runner    (1001) docker     (127)      358 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/detach_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      748 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/explain_statement.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/expression/
--rw-rw-r--   0 runner    (1001) docker     (127)     3933 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/expression/parsed_case_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3180 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/expression/parsed_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2663 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/expression/parsed_function_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1495 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/expression/parsed_literal_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)      858 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/expression/parsed_parameter_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1688 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/expression/parsed_property_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/expression/parsed_subquery_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1546 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/expression/parsed_variable_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)      626 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/extension_statement.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/parsed_data/
--rw-rw-r--   0 runner    (1001) docker     (127)      177 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/parsed_data/attach_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1163 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/parsed_expression_visitor.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2613 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/parsed_statement_visitor.h
--rw-rw-r--   0 runner    (1001) docker     (127)      292 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/parser.h
--rw-rw-r--   0 runner    (1001) docker     (127)      975 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/port_db.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/query/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/
--rw-rw-r--   0 runner    (1001) docker     (127)      946 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/node_pattern.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1100 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/pattern_element.h
--rw-rw-r--   0 runner    (1001) docker     (127)      587 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/pattern_element_chain.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1599 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/rel_pattern.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1309 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/query/query_part.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/
--rw-rw-r--   0 runner    (1001) docker     (127)      982 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/in_query_call_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1521 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/load_from.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1212 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/match_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      587 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/reading_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      657 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/unwind_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      928 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/query/regular_query.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/query/return_with_clause/
--rw-rw-r--   0 runner    (1001) docker     (127)     2155 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/query/return_with_clause/projection_body.h
--rw-rw-r--   0 runner    (1001) docker     (127)      485 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/query/return_with_clause/return_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/query/return_with_clause/with_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1798 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/query/single_query.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/
--rw-rw-r--   0 runner    (1001) docker     (127)      898 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/delete_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      601 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/insert_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1341 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/merge_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      538 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/set_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/updating_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1543 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/scan_source.h
--rw-rw-r--   0 runner    (1001) docker     (127)      712 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/standalone_call.h
--rw-rw-r--   0 runner    (1001) docker     (127)      945 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/statement.h
--rw-rw-r--   0 runner    (1001) docker     (127)      568 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/transaction_statement.h
--rw-rw-r--   0 runner    (1001) docker     (127)    12939 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/transformer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      330 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/use_database.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/visitor/
--rw-rw-r--   0 runner    (1001) docker     (127)     1163 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/parser/visitor/statement_read_write_analyzer.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/join_order/
--rw-rw-r--   0 runner    (1001) docker     (127)     2656 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/join_order/cardinality_estimator.h
--rw-rw-r--   0 runner    (1001) docker     (127)      801 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/join_order/cost_model.h
--rw-rw-r--   0 runner    (1001) docker     (127)      469 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/join_order/join_order_util.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2304 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/join_order_enumerator_context.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/ddl/
--rw-rw-r--   0 runner    (1001) docker     (127)      754 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/ddl/logical_alter.h
--rw-rw-r--   0 runner    (1001) docker     (127)      841 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/ddl/logical_create_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)      920 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/ddl/logical_ddl.h
--rw-rw-r--   0 runner    (1001) docker     (127)      795 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/ddl/logical_drop_table.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/extend/
--rw-rw-r--   0 runner    (1001) docker     (127)     1426 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/extend/base_logical_extend.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1107 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/extend/extend_direction.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1278 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/extend/logical_extend.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4582 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/extend/logical_recursive_extend.h
--rw-rw-r--   0 runner    (1001) docker     (127)      200 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/extend/recursive_join_type.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/factorization/
--rw-rw-r--   0 runner    (1001) docker     (127)      442 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/factorization/flatten_resolver.h
--rw-rw-r--   0 runner    (1001) docker     (127)      950 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/factorization/sink_util.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2011 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/logical_accumulate.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2430 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/logical_aggregate.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1376 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/logical_comment_on.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1381 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/logical_create_macro.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1079 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/logical_cross_product.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1632 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/logical_distinct.h
--rw-rw-r--   0 runner    (1001) docker     (127)      784 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/logical_empty_result.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1603 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/logical_explain.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1117 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/logical_filter.h
--rw-rw-r--   0 runner    (1001) docker     (127)      804 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/logical_flatten.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3562 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/logical_hash_join.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/logical_in_query_call.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1843 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/logical_intersect.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1297 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/logical_limit.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1147 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/logical_mark_accmulate.h
--rw-rw-r--   0 runner    (1001) docker     (127)      769 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/logical_multiplcity_reducer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1224 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/logical_node_label_filter.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3462 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/logical_operator.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1616 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/logical_order_by.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2156 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/logical_partitioner.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1176 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/logical_plan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1179 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/logical_plan_util.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1117 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/logical_projection.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1094 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/logical_standalone_call.h
--rw-rw-r--   0 runner    (1001) docker     (127)      969 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/logical_transaction.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1199 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/logical_union.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1413 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/logical_unwind.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/persistent/
--rw-rw-r--   0 runner    (1001) docker     (127)     1473 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_copy_from.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1946 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_copy_to.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2791 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_delete.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2037 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_insert.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3728 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_merge.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2803 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_set.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/scan/
--rw-rw-r--   0 runner    (1001) docker     (127)      643 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_dummy_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1290 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_expressions_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_index_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1217 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_scan_file.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1089 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_scan_internal_id.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1486 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_scan_node_property.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6044 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/schema.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/simple/
--rw-rw-r--   0 runner    (1001) docker     (127)      858 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_attach_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      583 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      578 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_detach_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1383 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_export_db.h
--rw-rw-r--   0 runner    (1001) docker     (127)      915 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_extension.h
--rw-rw-r--   0 runner    (1001) docker     (127)      757 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_import_db.h
--rw-rw-r--   0 runner    (1001) docker     (127)      953 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_simple.h
--rw-rw-r--   0 runner    (1001) docker     (127)      552 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_use_database.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/sip/
--rw-rw-r--   0 runner    (1001) docker     (127)     1588 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/sip/logical_semi_masker.h
--rw-rw-r--   0 runner    (1001) docker     (127)      308 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/operator/sip/side_way_info_passing.h
--rw-rw-r--   0 runner    (1001) docker     (127)    16586 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/planner.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3416 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/planner/subplans_table.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/
--rw-rw-r--   0 runner    (1001) docker     (127)     1252 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/data_pos.h
--rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/execution_context.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2051 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/expression_mapper.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/
--rw-rw-r--   0 runner    (1001) docker     (127)    11146 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/aggregate_hash_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1255 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/aggregate_input.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1824 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/base_aggregate.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1374 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/base_aggregate_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3698 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/hash_aggregate.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1905 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/hash_aggregate_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2811 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/simple_aggregate.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1565 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/simple_aggregate_scan.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/call/
--rw-rw-r--   0 runner    (1001) docker     (127)     2956 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/call/in_query_call.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1361 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/call/standalone_call.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1712 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/comment_on.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2858 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/cross_product.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/ddl/
--rw-rw-r--   0 runner    (1001) docker     (127)     1402 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/ddl/alter.h
--rw-rw-r--   0 runner    (1001) docker     (127)      779 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/ddl/create_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)      945 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/ddl/ddl.h
--rw-rw-r--   0 runner    (1001) docker     (127)      777 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/ddl/drop_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)      583 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/empty_result.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2713 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/filter.h
--rw-rw-r--   0 runner    (1001) docker     (127)      820 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/filtering_operator.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1242 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/flatten.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/hash_join/
--rw-rw-r--   0 runner    (1001) docker     (127)     4460 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/hash_join/hash_join_build.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4687 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/hash_join/hash_join_probe.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3299 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/hash_join/join_hash_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2359 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/index_lookup.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1541 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/index_scan.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/intersect/
--rw-rw-r--   0 runner    (1001) docker     (127)     3204 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/intersect/intersect.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1057 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/intersect/intersect_build.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1208 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/limit.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/macro/
--rw-rw-r--   0 runner    (1001) docker     (127)     1852 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/macro/create_macro.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5181 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/mask.h
--rw-rw-r--   0 runner    (1001) docker     (127)      972 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/multiplicity_reducer.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/order_by/
--rw-rw-r--   0 runner    (1001) docker     (127)     7982 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/order_by/key_block_merger.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1868 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1742 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by_data_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6358 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by_key_encoder.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2060 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by_merge.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2533 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3873 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/order_by/radix_sort.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2942 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/order_by/sort_state.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6218 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/order_by/top_k.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1694 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/order_by/top_k_scanner.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5655 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/partitioner.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/
--rw-rw-r--   0 runner    (1001) docker     (127)     2787 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/batch_insert.h
--rw-rw-r--   0 runner    (1001) docker     (127)      983 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/copy_rdf.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2426 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/copy_to.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3239 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/copy_to_csv.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2885 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/copy_to_parquet.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1604 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/delete.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6124 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/delete_executor.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1005 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/export_db.h
--rw-rw-r--   0 runner    (1001) docker     (127)      840 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/file_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      734 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/import_db.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5440 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/index_builder.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1163 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/insert.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3808 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/insert_executor.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2702 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/merge.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5761 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/node_batch_insert.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/
--rw-rw-r--   0 runner    (1001) docker     (127)     2367 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/base_csv_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1831 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/driver.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1862 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/parallel_csv_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1888 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/serial_csv_reader.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/npy/
--rw-rw-r--   0 runner    (1001) docker     (127)     1754 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/npy/npy_reader.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/
--rw-rw-r--   0 runner    (1001) docker     (127)     1481 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/boolean_column_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1616 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/callback_column_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5214 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/column_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1962 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/decode_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1359 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/interval_column_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1842 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/list_column_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4105 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/parquet_dbp_decoder.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4637 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/parquet_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4238 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/parquet_rle_bp_decoder.h
--rw-rw-r--   0 runner    (1001) docker     (127)      976 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/parquet_timestamp.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1881 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/resizable_buffer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1327 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/string_column_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1262 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/struct_column_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3427 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/templated_column_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6782 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/thrift_tools.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/
--rw-rw-r--   0 runner    (1001) docker     (127)     5911 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/rdf_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7424 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/rdf_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)      380 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/rdf_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2388 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/triple_store.h
--rw-rw-r--   0 runner    (1001) docker     (127)      865 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/reader_bind_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4368 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/rel_batch_insert.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1938 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/set.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6617 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/set_executor.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/
--rw-rw-r--   0 runner    (1001) docker     (127)     3914 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/basic_column_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2248 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/boolean_column_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4081 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/column_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1063 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/interval_column_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1729 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/list_column_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1087 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/parquet_rle_bp_encoder.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3229 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/parquet_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3898 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/standard_column_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5245 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/string_column_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1711 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/struct_column_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4998 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/physical_operator.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1356 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/profile.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1518 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/projection.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/
--rw-rw-r--   0 runner    (1001) docker     (127)     2317 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/all_shortest_path_state.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3932 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/bfs_state.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1693 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/frontier.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6229 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/frontier_scanner.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4590 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/path_property_probe.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5296 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/recursive_join.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1380 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/scan_frontier.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1684 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/shortest_path_state.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1050 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/variable_length_state.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2908 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/result_collector.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/scan/
--rw-rw-r--   0 runner    (1001) docker     (127)     1067 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_multi_node_tables.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1913 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_multi_rel_tables.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2083 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_node_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2179 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_rel_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1085 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3474 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/scan_node_id.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5060 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/semi_masker.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/simple/
--rw-rw-r--   0 runner    (1001) docker     (127)      813 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/simple/attach_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      463 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/simple/database_operator.h
--rw-rw-r--   0 runner    (1001) docker     (127)      696 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/simple/detach_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      966 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/simple/export_db.h
--rw-rw-r--   0 runner    (1001) docker     (127)      690 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/simple/import_db.h
--rw-rw-r--   0 runner    (1001) docker     (127)      941 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/simple/install_extension.h
--rw-rw-r--   0 runner    (1001) docker     (127)      721 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/simple/load_extension.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1297 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/simple/simple.h
--rw-rw-r--   0 runner    (1001) docker     (127)      684 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/simple/use_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1777 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1435 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/skip.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/table_scan/
--rw-rw-r--   0 runner    (1001) docker     (127)     1102 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/table_scan/ftable_scan_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3006 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/table_scan/union_all_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1195 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/transaction.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1499 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/operator/unwind.h
--rw-rw-r--   0 runner    (1001) docker     (127)      388 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/physical_plan.h
--rw-rw-r--   0 runner    (1001) docker     (127)    12402 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/plan_mapper.h
--rw-rw-r--   0 runner    (1001) docker     (127)      638 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/processor.h
--rw-rw-r--   0 runner    (1001) docker     (127)      621 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/processor_task.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/result/
--rw-rw-r--   0 runner    (1001) docker     (127)     1737 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/result/base_hash_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)    16611 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/result/factorized_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1187 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/result/flat_tuple.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1061 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/result/mark_hash_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1519 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/result/result_set.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1063 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/processor/result/result_set_descriptor.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/buffer_manager/
--rw-rw-r--   0 runner    (1001) docker     (127)    10155 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/buffer_manager/bm_file_handle.h
--rw-rw-r--   0 runner    (1001) docker     (127)    13079 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/buffer_manager/buffer_manager.h
--rw-rw-r--   0 runner    (1001) docker     (127)      527 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/buffer_manager/locked_queue.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2759 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/buffer_manager/memory_manager.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1714 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/buffer_manager/vm_region.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/compression/
--rw-rw-r--   0 runner    (1001) docker     (127)    15859 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/compression/compression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1695 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/compression/sign_extend.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3328 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/file_handle.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/index/
--rw-rw-r--   0 runner    (1001) docker     (127)    14400 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/index/hash_index.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1656 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/index/hash_index_header.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2243 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/index/hash_index_slot.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2560 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/index/hash_index_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7162 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/index/in_mem_hash_index.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/local_storage/
--rw-rw-r--   0 runner    (1001) docker     (127)     2514 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/local_storage/local_node_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3159 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/local_storage/local_rel_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1052 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/local_storage/local_storage.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9200 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/local_storage/local_table.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/stats/
--rw-rw-r--   0 runner    (1001) docker     (127)      999 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/stats/metadata_dah_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3254 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/stats/node_table_statistics.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3125 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/stats/nodes_store_statistics.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1594 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/stats/property_statistics.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3873 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/stats/rel_table_statistics.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2721 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/stats/rels_store_statistics.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1947 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/stats/table_statistics.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4449 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/stats/table_statistics_collection.h
--rw-rw-r--   0 runner    (1001) docker     (127)      821 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/storage_extension.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3147 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/storage_manager.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/storage_structure/
--rw-rw-r--   0 runner    (1001) docker     (127)     2297 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/storage_structure/db_file_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)    18677 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/storage_structure/disk_array.h
--rw-rw-r--   0 runner    (1001) docker     (127)      368 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/storage_structure/in_mem_page.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4969 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/storage_structure/overflow_file.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8115 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/storage_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)      804 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/storage_version_info.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/store/
--rw-rw-r--   0 runner    (1001) docker     (127)     4852 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/store/chunked_node_group.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1626 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/store/chunked_node_group_collection.h
--rw-rw-r--   0 runner    (1001) docker     (127)    14266 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/store/column.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9626 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/store/column_chunk.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2508 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/store/dictionary_chunk.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3021 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/store/dictionary_column.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5856 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/store/list_column.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3467 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/store/list_column_chunk.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6212 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/store/node_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3448 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/store/node_table_data.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2528 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/store/null_column.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7138 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/store/rel_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)    12842 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/store/rel_table_data.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3202 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/store/string_column.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2511 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/store/string_column_chunk.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2910 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/store/struct_column.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1968 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/store/struct_column_chunk.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3978 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/store/table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2638 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/store/table_data.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2397 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/undo_buffer.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/wal/
--rw-rw-r--   0 runner    (1001) docker     (127)     2377 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/wal/wal.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5999 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/wal/wal_record.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1888 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/wal_replayer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      725 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/storage/wal_replayer_utils.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/transaction/
--rw-rw-r--   0 runner    (1001) docker     (127)     2666 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/transaction/transaction.h
--rw-rw-r--   0 runner    (1001) docker     (127)      294 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/transaction/transaction_action.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2473 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/transaction/transaction_context.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3396 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/include/transaction/transaction_manager.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/main/
--rw-rw-r--   0 runner    (1001) docker     (127)      444 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/main/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1638 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/main/attached_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    21823 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/main/client_context.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3262 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/main/connection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5810 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/main/database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2483 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/main/database_manager.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1572 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/main/db_config.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    13980 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/main/plan_printer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      810 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/main/prepared_statement.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4054 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/main/query_result.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      578 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/main/query_summary.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4339 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/main/storage_driver.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      317 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/main/version.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/optimizer/
--rw-rw-r--   0 runner    (1001) docker     (127)      602 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/optimizer/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    10541 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/optimizer/acc_hash_join_optimizer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3540 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/optimizer/agg_key_dependency_optimizer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1488 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/optimizer/correlated_subquery_unnest_solver.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    10339 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/optimizer/factorization_rewriter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    12064 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/optimizer/filter_push_down_optimizer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      340 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/optimizer/logical_operator_collector.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5558 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/optimizer/logical_operator_visitor.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2087 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/optimizer/optimizer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    13109 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/optimizer/projection_push_down_optimizer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1201 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/optimizer/remove_factorization_rewriter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1537 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/optimizer/remove_unnecessary_join_optimizer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1902 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/optimizer/top_k_optimizer.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/
--rw-rw-r--   0 runner    (1001) docker     (127)      400 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/antlr_parser/
--rw-rw-r--   0 runner    (1001) docker     (127)      267 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/antlr_parser/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1595 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/antlr_parser/kuzu_cypher_parser.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1391 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/antlr_parser/parser_error_listener.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      827 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/antlr_parser/parser_error_strategy.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      455 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/create_macro.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/expression/
--rw-rw-r--   0 runner    (1001) docker     (127)      346 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/expression/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2127 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/expression/parsed_case_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3281 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/expression/parsed_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      785 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/expression/parsed_function_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      491 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/expression/parsed_property_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      491 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/expression/parsed_variable_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3506 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/parsed_expression_visitor.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4399 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/parsed_statement_visitor.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1641 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/parser.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/transform/
--rw-rw-r--   0 runner    (1001) docker     (127)      726 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/transform/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      646 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/transform/transform_attach_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      450 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/transform/transform_comment_on.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3602 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/transform/transform_copy.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7632 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/transform/transform_ddl.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      392 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/transform/transform_detach_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    27904 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/transform/transform_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      858 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/transform/transform_extension.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7789 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/transform/transform_graph_pattern.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1272 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/transform/transform_macro.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      833 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/transform/transform_port_db.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2587 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/transform/transform_projection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2253 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/transform/transform_query.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2715 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/transform/transform_reading_clause.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      490 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/transform/transform_standalone_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1209 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/transform/transform_transaction.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2681 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/transform/transform_updating_clause.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      380 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/transform/transform_use_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4493 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/transformer.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/visitor/
--rw-rw-r--   0 runner    (1001) docker     (127)      209 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/visitor/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      258 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/parser/visitor/statement_read_write_analyzer.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/
--rw-rw-r--   0 runner    (1001) docker     (127)      339 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/join_order/
--rw-rw-r--   0 runner    (1001) docker     (127)      251 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/join_order/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     5776 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/join_order/cardinality_estimator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1652 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/join_order/cost_model.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      745 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/join_order/join_order_util.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1233 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/join_order_enumerator_context.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/
--rw-rw-r--   0 runner    (1001) docker     (127)     1025 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/ddl/
--rw-rw-r--   0 runner    (1001) docker     (127)      175 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/ddl/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/ddl/logical_ddl.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/extend/
--rw-rw-r--   0 runner    (1001) docker     (127)      253 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/extend/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1348 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/extend/base_logical_extend.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1205 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/extend/logical_extend.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2914 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/extend/logical_recursive_extend.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/factorization/
--rw-rw-r--   0 runner    (1001) docker     (127)      223 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/factorization/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1007 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/factorization/flatten_resolver.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2591 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/factorization/sink_util.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1552 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/logical_accumulate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2870 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/logical_aggregate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      517 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/logical_comment_on.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      523 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/logical_create_macro.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      829 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/logical_cross_product.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1523 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/logical_distinct.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      678 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/logical_dummy_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      800 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/logical_explain.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      822 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/logical_filter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      407 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/logical_flatten.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7224 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/logical_hash_join.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      726 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/logical_in_query_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2606 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/logical_intersect.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1039 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/logical_limit.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1514 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/logical_mark_accumulate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6394 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/logical_operator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2805 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/logical_order_by.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      939 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/logical_partitioner.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1065 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/logical_plan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3973 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/logical_plan_util.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2197 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/logical_projection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1947 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/logical_union.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      980 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/logical_unwind.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/persistent/
--rw-rw-r--   0 runner    (1001) docker     (127)      329 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/persistent/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      853 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_copy_from.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      620 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_copy_to.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1732 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_delete.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2031 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_insert.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1366 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_merge.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2384 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_set.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/scan/
--rw-rw-r--   0 runner    (1001) docker     (127)      328 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/scan/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      347 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/scan/logical_expressions_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      935 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/scan/logical_index_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      643 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/scan/logical_scan_file.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      481 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/scan/logical_scan_internal_id.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      561 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/scan/logical_scan_node_property.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5973 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/schema.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/simple/
--rw-rw-r--   0 runner    (1001) docker     (127)      185 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/simple/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      514 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/operator/simple/logical_simple.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/plan/
--rw-rw-r--   0 runner    (1001) docker     (127)     1042 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/plan/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1329 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/plan/append_accumulate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      814 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/plan/append_aggregate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      816 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/plan/append_cross_product.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1971 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/plan/append_delete.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      553 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/plan/append_distinct.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      399 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/plan/append_dummy_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      473 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/plan/append_expressions_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    13525 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/plan/append_extend.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      913 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/plan/append_filter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      800 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/plan/append_flatten.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      740 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/plan/append_in_query_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2692 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/plan/append_insert.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4805 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/plan/append_join.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      552 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/plan/append_limit.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      658 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/plan/append_mark_accumulate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      439 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/plan/append_multiplicity_reducer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      615 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/plan/append_order_by.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1452 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/plan/append_projection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      684 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/plan/append_scan_file.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1596 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/plan/append_scan_node.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2066 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/plan/append_set.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6469 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/plan/append_simple.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/plan/append_standalone_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      826 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/plan/append_unwind.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8216 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/plan/plan_copy.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    27166 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/plan/plan_join_order.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2684 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/plan/plan_port_db.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3074 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/plan/plan_projection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5987 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/plan/plan_read.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1829 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/plan/plan_single_query.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/plan/plan_standalone_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8673 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/plan/plan_subquery.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6119 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/plan/plan_update.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3507 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/planner.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5305 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/query_planner.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3769 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/planner/subplans_table.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/
--rw-rw-r--   0 runner    (1001) docker     (127)      272 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/
--rw-rw-r--   0 runner    (1001) docker     (127)     1486 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     4798 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/create_factorized_table_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2148 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/create_result_collector.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8210 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/expression_mapper.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      702 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_acc_hash_join.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1102 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_accumulate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9380 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_aggregate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1046 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_comment_on.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    15122 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_copy_from.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4813 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_copy_to.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_create_macro.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1880 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_cross_product.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_ddl.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6207 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_delete.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      750 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_distinct.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1595 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_dummy_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      345 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_empty_result.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1956 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_explain.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1871 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_expressions_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6300 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_extend.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      822 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_filter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      606 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_flatten.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5998 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_hash_join.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1217 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_in_query_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2425 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_index_scan_node.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5186 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_insert.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3182 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_intersect.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      933 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_label_filter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1344 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_limit.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      784 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_mark_accumulate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2627 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_merge.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      533 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_multiplicity_reducer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4327 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_order_by.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6872 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_path_property_probe.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1251 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_projection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3425 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_recursive_extend.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1457 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_scan_file.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      816 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_scan_frontier.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1090 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_scan_node.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3519 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_scan_node_property.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3246 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_semi_masker.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6572 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_set.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4721 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_simple.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      969 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_standalone_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      593 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_transaction.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2083 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_union.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1096 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/map_unwind.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8345 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/map/plan_mapper.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/
--rw-rw-r--   0 runner    (1001) docker     (127)      966 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/aggregate/
--rw-rw-r--   0 runner    (1001) docker     (127)      400 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/aggregate/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    36408 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/aggregate/aggregate_hash_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1691 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/aggregate/base_aggregate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      755 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/aggregate/base_aggregate_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5470 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/aggregate/hash_aggregate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2004 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/aggregate/hash_aggregate_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4824 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/aggregate/simple_aggregate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1388 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/aggregate/simple_aggregate_scan.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/call/
--rw-rw-r--   0 runner    (1001) docker     (127)      230 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/call/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2972 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/call/in_query_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      997 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/call/standalone_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      826 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/comment_on.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1383 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/cross_product.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/ddl/
--rw-rw-r--   0 runner    (1001) docker     (127)      256 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/ddl/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1375 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/ddl/alter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      758 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/ddl/create_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      570 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/ddl/ddl.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      537 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/ddl/drop_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      213 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/empty_result.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2472 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/filter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1148 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/filtering_operator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1237 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/flatten.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/hash_join/
--rw-rw-r--   0 runner    (1001) docker     (127)      270 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/hash_join/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2057 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/hash_join/hash_join_build.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8164 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/hash_join/hash_join_probe.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9263 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/hash_join/join_hash_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4450 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/index_lookup.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1780 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/index_scan.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/intersect/
--rw-rw-r--   0 runner    (1001) docker     (127)      208 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/intersect/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     9643 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/intersect/intersect.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1413 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/limit.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/macro/
--rw-rw-r--   0 runner    (1001) docker     (127)      217 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/macro/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      742 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/macro/create_macro.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      538 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/multiplicity_reducer.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/order_by/
--rw-rw-r--   0 runner    (1001) docker     (127)      410 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/order_by/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    16047 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/order_by/key_block_merger.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1082 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/order_by/order_by.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    14049 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/order_by/order_by_key_encoder.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1554 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/order_by/order_by_merge.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1438 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/order_by/order_by_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    12968 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/order_by/radix_sort.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9040 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/order_by/sort_state.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    12677 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/order_by/top_k.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      834 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/order_by/top_k_scanner.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7757 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/partitioner.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/
--rw-rw-r--   0 runner    (1001) docker     (127)      579 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      473 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/copy_rdf.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      828 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/copy_to.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8358 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/copy_to_csv.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1780 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/copy_to_parquet.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1751 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/delete.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5409 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/delete_executor.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4759 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/index_builder.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      861 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/insert.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7210 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/insert_executor.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3034 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/merge.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11722 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/node_batch_insert.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/
--rw-rw-r--   0 runner    (1001) docker     (127)      325 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/
--rw-rw-r--   0 runner    (1001) docker     (127)      297 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    14378 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/base_csv_reader.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4367 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/driver.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8578 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/parallel_csv_reader.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6554 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/serial_csv_reader.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/npy/
--rw-rw-r--   0 runner    (1001) docker     (127)      211 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/npy/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    13924 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/npy/npy_reader.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/
--rw-rw-r--   0 runner    (1001) docker     (127)      445 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      850 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/boolean_column_reader.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    24123 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/column_reader.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1234 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/interval_column_reader.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5989 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/list_column_reader.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    30053 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/parquet_reader.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1404 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/parquet_timestamp.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3928 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/string_column_reader.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3444 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/struct_column_reader.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/
--rw-rw-r--   0 runner    (1001) docker     (127)      254 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    13995 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/rdf_reader.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    13456 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/rdf_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2966 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/rdf_utils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2052 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/reader_bind_utils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11285 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/rel_batch_insert.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      997 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/set.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6494 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/set_executor.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/
--rw-rw-r--   0 runner    (1001) docker     (127)      564 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    12826 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/basic_column_writer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1538 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/boolean_column_writer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    16444 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/column_writer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1539 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/interval_column_writer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4734 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/list_column_writer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2633 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/parquet_rle_bp_encoder.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11700 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/parquet_writer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8703 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/string_column_writer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4078 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/struct_column_writer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8622 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/physical_operator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1022 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/profile.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1757 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/projection.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/
--rw-rw-r--   0 runner    (1001) docker     (127)      337 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      790 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/frontier.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7361 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/frontier_scanner.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5063 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/path_property_probe.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    12941 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/recursive_join.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      323 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/scan_frontier.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2479 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/result_collector.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/scan/
--rw-rw-r--   0 runner    (1001) docker     (127)      323 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/scan/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1565 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/scan/scan_multi_node_tables.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3737 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/scan/scan_multi_rel_tables.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      792 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/scan/scan_node_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      966 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/scan/scan_rel_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      675 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/scan/scan_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5159 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/scan_node_id.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4537 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/semi_masker.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/simple/
--rw-rw-r--   0 runner    (1001) docker     (127)      381 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/simple/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1975 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/simple/attach_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/simple/detach_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4683 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/simple/export_db.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      527 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/simple/import_db.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2423 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/simple/install_extension.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2205 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/simple/load_extension.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      616 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/simple/simple.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/simple/use_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2443 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/skip.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/table_scan/
--rw-rw-r--   0 runner    (1001) docker     (127)      248 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/table_scan/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2677 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/table_scan/ftable_scan_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1832 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/table_scan/union_all_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2416 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/transaction.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2656 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/operator/unwind.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2709 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/processor.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1788 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/processor_task.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/result/
--rw-rw-r--   0 runner    (1001) docker     (127)      336 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/result/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     7137 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/result/base_hash_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    34389 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/result/factorized_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2119 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/result/flat_tuple.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2304 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/result/mark_hash_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1499 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/result/result_set.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1170 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/processor/result/result_set_descriptor.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/
--rw-rw-r--   0 runner    (1001) docker     (127)      561 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/buffer_manager/
--rw-rw-r--   0 runner    (1001) docker     (127)      277 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/buffer_manager/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     6820 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/buffer_manager/bm_file_handle.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    15736 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/buffer_manager/buffer_manager.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2145 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/buffer_manager/memory_manager.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3721 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/buffer_manager/vm_region.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/compression/
--rw-rw-r--   0 runner    (1001) docker     (127)      258 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/compression/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    35352 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/compression/compression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1880 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/file_handle.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/index/
--rw-rw-r--   0 runner    (1001) docker     (127)      209 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/index/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    33661 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/index/hash_index.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    16151 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/index/in_mem_hash_index.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/local_storage/
--rw-rw-r--   0 runner    (1001) docker     (127)      279 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/local_storage/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     6051 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/local_storage/local_node_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    12337 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/local_storage/local_rel_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1723 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/local_storage/local_storage.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6946 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/local_storage/local_table.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/stats/
--rw-rw-r--   0 runner    (1001) docker     (127)      415 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/stats/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1201 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/stats/metadata_dah_info.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7988 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/stats/node_table_statistics.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5521 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/stats/nodes_store_statistics.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2458 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/stats/property_statistics.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5129 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/stats/rel_table_statistics.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4338 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/stats/rels_store_statistics.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2843 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/stats/table_statistics.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5812 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/stats/table_statistics_collection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11500 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/storage_manager.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/storage_structure/
--rw-rw-r--   0 runner    (1001) docker     (127)      263 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/storage_structure/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     5262 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/storage_structure/db_file_utils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    23949 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/storage_structure/disk_array.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      557 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/storage_structure/in_mem_page.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    10191 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/storage_structure/overflow_file.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4291 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/storage_utils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      737 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/storage_version_info.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/store/
--rw-rw-r--   0 runner    (1001) docker     (127)      649 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/store/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     7050 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/store/chunked_node_group.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2108 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/store/chunked_node_group_collection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    43158 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/store/column.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    27570 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/store/column_chunk.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3687 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/store/dictionary_chunk.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    10644 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/store/dictionary_column.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    22097 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/store/list_column.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    16059 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/store/list_column_chunk.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9833 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/store/node_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    10804 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/store/node_table_data.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8460 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/store/null_column.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9148 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/store/rel_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    51121 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/store/rel_table_data.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11782 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/store/string_column.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7813 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/store/string_column_chunk.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9257 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/store/struct_column.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6184 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/store/struct_column_chunk.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1779 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/store/table_data.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7083 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/undo_buffer.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/wal/
--rw-rw-r--   0 runner    (1001) docker     (127)      191 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/wal/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     3679 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/wal/wal.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5210 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/wal/wal_record.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    13351 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/wal_replayer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1078 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/storage/wal_replayer_utils.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/transaction/
--rw-rw-r--   0 runner    (1001) docker     (127)      240 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/transaction/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      611 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/transaction/transaction.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2976 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/transaction/transaction_context.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6237 2024-05-13 08:04:59.000000 sdist/kuzu-source/src/transaction/transaction_manager.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/
--rw-rw-r--   0 runner    (1001) docker     (127)      489 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_cypher/
--rw-rw-r--   0 runner    (1001) docker     (127)      949 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_cypher/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    56662 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_cypher/cypher_lexer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)   469845 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_cypher/cypher_parser.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_cypher/include/
--rw-rw-r--   0 runner    (1001) docker     (127)     3272 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_cypher/include/cypher_lexer.h
--rw-rw-r--   0 runner    (1001) docker     (127)    88283 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_cypher/include/cypher_parser.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/
--rw-rw-r--   0 runner    (1001) docker     (127)    10564 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     4237 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/LICENSE
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/
--rw-rw-r--   0 runner    (1001) docker     (127)      285 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRErrorListener.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     8375 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRErrorListener.h
--rw-rw-r--   0 runner    (1001) docker     (127)      285 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRErrorStrategy.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     5269 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRErrorStrategy.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      552 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRFileStream.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1018 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRFileStream.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     4326 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRInputStream.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2623 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRInputStream.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1804 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BailErrorStrategy.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2483 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BailErrorStrategy.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1163 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BaseErrorListener.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1377 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BaseErrorListener.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     9946 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BufferedTokenStream.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     8014 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BufferedTokenStream.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      281 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CharStream.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1479 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CharStream.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     4459 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonToken.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     4918 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonToken.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1327 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonTokenFactory.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2564 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonTokenFactory.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1767 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonTokenStream.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2713 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonTokenStream.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      597 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ConsoleErrorListener.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1060 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ConsoleErrorListener.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    11864 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/DefaultErrorStrategy.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)    20289 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/DefaultErrorStrategy.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     3484 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/DiagnosticErrorListener.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3600 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/DiagnosticErrorListener.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2152 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Exceptions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3868 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Exceptions.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1867 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/FailedPredicateException.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1096 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/FailedPredicateException.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2767 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/FlatHashMap.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2676 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/FlatHashSet.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      559 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/InputMismatchException.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      783 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/InputMismatchException.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      350 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/IntStream.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)    10251 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/IntStream.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      615 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/InterpreterRuleContext.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1604 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/InterpreterRuleContext.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     6878 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Lexer.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     7038 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Lexer.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1867 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/LexerInterpreter.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1564 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/LexerInterpreter.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1234 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/LexerNoViableAltException.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      916 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/LexerNoViableAltException.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     2412 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ListTokenSource.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3795 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ListTokenSource.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1585 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/NoViableAltException.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1693 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/NoViableAltException.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    19305 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Parser.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)    19393 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Parser.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    10523 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ParserInterpreter.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     7171 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ParserInterpreter.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     3952 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ParserRuleContext.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     5666 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ParserRuleContext.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1958 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ProxyErrorListener.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1657 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ProxyErrorListener.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1916 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RecognitionException.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3961 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RecognitionException.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     4572 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Recognizer.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     5733 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Recognizer.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     3588 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuleContext.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     5561 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuleContext.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      725 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuleContextWithAltNum.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      985 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuleContextWithAltNum.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     2091 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuntimeMetaData.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     7393 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuntimeMetaData.h
--rw-rw-r--   0 runner    (1001) docker     (127)      246 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Token.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3462 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Token.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1217 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenFactory.h
--rw-rw-r--   0 runner    (1001) docker     (127)      264 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenSource.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3839 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenSource.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      284 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenStream.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     6098 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenStream.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    15023 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenStreamRewriter.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)    12507 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenStreamRewriter.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     5847 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/UnbufferedCharStream.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     4351 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/UnbufferedCharStream.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     7467 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/UnbufferedTokenStream.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     4241 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/UnbufferedTokenStream.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2105 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Version.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1907 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Vocabulary.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     6943 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Vocabulary.h
--rw-rw-r--   0 runner    (1001) docker     (127)      270 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/WritableToken.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      676 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/WritableToken.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2560 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/antlr4-common.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5524 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/antlr4-runtime.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/
--rwxrwxr-x   0 runner    (1001) docker     (127)     4193 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATN.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     4845 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATN.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     4158 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNConfig.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     5513 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNConfig.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     6500 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNConfigSet.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     5185 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNConfigSet.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1252 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNDeserializationOptions.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1302 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNDeserializationOptions.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    21573 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNDeserializer.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      835 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNDeserializer.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1216 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNSimulator.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2761 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNSimulator.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1538 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNState.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     4374 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNState.h
--rw-rw-r--   0 runner    (1001) docker     (127)      990 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNStateType.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      796 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNStateType.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      439 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNType.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1214 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ActionTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1104 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ActionTransition.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      604 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/AmbiguityInfo.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3295 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/AmbiguityInfo.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     4211 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ArrayPredictionContext.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1900 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ArrayPredictionContext.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      840 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/AtomTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1084 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/AtomTransition.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      729 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/BasicBlockStartState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      649 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/BasicState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      762 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/BlockEndState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      853 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/BlockStartState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      520 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ContextSensitivityInfo.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2123 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ContextSensitivityInfo.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      561 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionEventInfo.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2459 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionEventInfo.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      934 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionInfo.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     9762 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionInfo.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      342 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionState.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      960 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      969 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/EpsilonTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1402 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/EpsilonTransition.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      527 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ErrorInfo.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1861 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ErrorInfo.h
--rw-rw-r--   0 runner    (1001) docker     (127)      416 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/HashUtils.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     7271 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LL1Analyzer.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3275 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LL1Analyzer.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     2950 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerATNConfig.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1666 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerATNConfig.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    22025 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerATNSimulator.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     8819 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerATNSimulator.h
--rw-rw-r--   0 runner    (1001) docker     (127)      324 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3494 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     4031 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerActionExecutor.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     6150 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerActionExecutor.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1460 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerActionType.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1306 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerChannelAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1908 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerChannelAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1555 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerCustomAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2772 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerCustomAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1784 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerIndexedCustomAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3046 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerIndexedCustomAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1269 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerModeAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1780 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerModeAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      977 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerMoreAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1701 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerMoreAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1010 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerPopModeAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1735 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerPopModeAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1311 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerPushModeAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1817 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerPushModeAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      977 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerSkipAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1664 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerSkipAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1269 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerTypeAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1717 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerTypeAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      584 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LookaheadEventInfo.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1914 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LookaheadEventInfo.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      736 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LoopEndState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      868 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/NotSetTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      854 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/NotSetTransition.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      484 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/OrderedATNConfigSet.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      631 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/OrderedATNConfigSet.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     2789 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParseInfo.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3665 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParseInfo.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    53167 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParserATNSimulator.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)    45705 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParserATNSimulator.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2278 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParserATNSimulatorOptions.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1052 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PlusBlockStartState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      842 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PlusLoopbackState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      901 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PrecedencePredicateTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1187 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PrecedencePredicateTransition.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      685 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredicateEvalInfo.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2885 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredicateEvalInfo.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1009 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredicateTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1674 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredicateTransition.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    20987 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContext.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     9173 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContext.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2360 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextCache.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2738 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextCache.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5386 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextMergeCache.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4033 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextMergeCache.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2602 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextMergeCacheOptions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextType.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     5939 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionMode.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)    20991 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionMode.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     7943 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ProfilingATNSimulator.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2982 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ProfilingATNSimulator.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      891 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RangeTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      944 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RangeTransition.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      746 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RuleStartState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      911 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RuleStopState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1156 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RuleTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1484 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RuleTransition.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    14979 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SemanticContext.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     9030 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SemanticContext.h
--rw-rw-r--   0 runner    (1001) docker     (127)      451 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SemanticContextType.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3246 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SerializedATNView.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      898 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SetTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1267 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SetTransition.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     2870 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SingletonPredictionContext.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1834 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SingletonPredictionContext.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      754 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/StarBlockStartState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1140 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/StarLoopEntryState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      644 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/StarLoopbackState.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      733 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/StarLoopbackState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      762 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/TokensStartState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      911 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/Transition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2164 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/Transition.h
--rw-rw-r--   0 runner    (1001) docker     (127)      730 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/TransitionType.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      778 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/TransitionType.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      680 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/WildcardTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      839 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/WildcardTransition.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/
--rwxrwxr-x   0 runner    (1001) docker     (127)     2868 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFA.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3045 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFA.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1726 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFASerializer.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      772 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFASerializer.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1490 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFAState.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     6068 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFAState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      509 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/LexerDFASerializer.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      533 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/LexerDFASerializer.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/internal/
--rw-rw-r--   0 runner    (1001) docker     (127)     2694 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/internal/Synchronization.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5499 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/internal/Synchronization.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/
--rwxrwxr-x   0 runner    (1001) docker     (127)     3098 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/InterpreterDataReader.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      989 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/InterpreterDataReader.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1671 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/Interval.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3009 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/Interval.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    13209 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/IntervalSet.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     6478 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/IntervalSet.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     2820 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/MurmurHash.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3595 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/MurmurHash.h
--rw-rw-r--   0 runner    (1001) docker     (127)       71 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/Predicate.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      446 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/Predicate.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/
--rw-rw-r--   0 runner    (1001) docker     (127)      242 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Any.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      370 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Any.h
--rw-rw-r--   0 runner    (1001) docker     (127)      966 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Arrays.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3620 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Arrays.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1828 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/BitSet.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     4837 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/CPPUtils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2582 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/CPPUtils.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1195 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Casts.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4122 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Declarations.h
--rw-rw-r--   0 runner    (1001) docker     (127)      901 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/StringUtils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      425 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/StringUtils.h
--rw-rw-r--   0 runner    (1001) docker     (127)      723 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Unicode.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8728 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Utf8.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2148 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Utf8.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/
--rwxrwxr-x   0 runner    (1001) docker     (127)     5650 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/AbstractParseTreeVisitor.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      677 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ErrorNode.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1255 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ErrorNodeImpl.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1429 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ErrorNodeImpl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1906 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/IterativeParseTreeWalker.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2124 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/IterativeParseTreeWalker.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      349 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTree.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     4216 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTree.h
--rw-rw-r--   0 runner    (1001) docker     (127)      288 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeListener.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1213 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeListener.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1434 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeProperty.h
--rw-rw-r--   0 runner    (1001) docker     (127)      430 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeType.h
--rw-rw-r--   0 runner    (1001) docker     (127)      285 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeVisitor.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2212 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeVisitor.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1381 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeWalker.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2031 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeWalker.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1145 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/TerminalNode.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1281 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/TerminalNodeImpl.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1003 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/TerminalNodeImpl.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     6872 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/Trees.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3060 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/Trees.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/
--rw-rw-r--   0 runner    (1001) docker     (127)      274 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/Chunk.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1460 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/Chunk.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1868 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreeMatch.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     5768 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreeMatch.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1800 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreePattern.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     4384 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreePattern.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    12574 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreePatternMatcher.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     8715 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreePatternMatcher.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1820 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/RuleTagToken.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     4742 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/RuleTagToken.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      811 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TagChunk.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3030 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TagChunk.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      623 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TextChunk.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1464 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TextChunk.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      959 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TokenTagToken.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2786 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TokenTagToken.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/
--rwxrwxr-x   0 runner    (1001) docker     (127)     4960 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPath.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2824 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPath.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      747 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathElement.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1029 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathElement.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6047 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1169 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexer.g4
--rw-rw-r--   0 runner    (1001) docker     (127)     1349 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexer.h
--rw-rw-r--   0 runner    (1001) docker     (127)       98 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexer.tokens
--rwxrwxr-x   0 runner    (1001) docker     (127)      506 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexerErrorListener.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      635 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexerErrorListener.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      647 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathRuleAnywhereElement.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      709 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathRuleAnywhereElement.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      966 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathRuleElement.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      620 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathRuleElement.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      647 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathTokenAnywhereElement.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      631 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathTokenAnywhereElement.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1054 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathTokenElement.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      623 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathTokenElement.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      665 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathWildcardAnywhereElement.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      558 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathWildcardAnywhereElement.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      621 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathWildcardElement.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      542 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathWildcardElement.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/
--rw-rw-r--   0 runner    (1001) docker     (127)     5677 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/CHANGELOG.md
--rw-rw-r--   0 runner    (1001) docker     (127)    12841 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1633 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/CONTRIBUTING.md
--rw-rw-r--   0 runner    (1001) docker     (127)     1084 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/LICENSE
--rw-rw-r--   0 runner    (1001) docker     (127)      652 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/README
--rw-rw-r--   0 runner    (1001) docker     (127)     4099 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/README.md
--rw-rw-r--   0 runner    (1001) docker     (127)      314 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/SECURITY.md
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/common/
--rw-rw-r--   0 runner    (1001) docker     (127)      621 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/common/constants.c
--rw-rw-r--   0 runner    (1001) docker     (127)     8011 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/common/constants.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7965 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/common/context.c
--rw-rw-r--   0 runner    (1001) docker     (127)     4666 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/common/context.h
--rw-rw-r--   0 runner    (1001) docker     (127)   122784 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/common/dictionary.bin
--rw-rw-r--   0 runner    (1001) docker     (127)    51687 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/common/dictionary.bin.br
--rw-rw-r--   0 runner    (1001) docker     (127)   472009 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/common/dictionary.c
--rw-rw-r--   0 runner    (1001) docker     (127)     1951 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/common/dictionary.h
--rw-rw-r--   0 runner    (1001) docker     (127)      513 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/common/platform.c
--rw-rw-r--   0 runner    (1001) docker     (127)    18385 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/common/platform.h
--rw-rw-r--   0 runner    (1001) docker     (127)    17424 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/common/shared_dictionary.c
--rw-rw-r--   0 runner    (1001) docker     (127)     2413 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/common/shared_dictionary_internal.h
--rw-rw-r--   0 runner    (1001) docker     (127)    10677 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/common/transform.c
--rw-rw-r--   0 runner    (1001) docker     (127)     3209 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/common/transform.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1723 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/common/version.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/dec/
--rw-rw-r--   0 runner    (1001) docker     (127)     2285 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/dec/bit_reader.c
--rw-rw-r--   0 runner    (1001) docker     (127)    14854 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/dec/bit_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)   103991 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/dec/decode.c
--rw-rw-r--   0 runner    (1001) docker     (127)    11996 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/dec/huffman.c
--rw-rw-r--   0 runner    (1001) docker     (127)     4107 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/dec/huffman.h
--rw-rw-r--   0 runner    (1001) docker     (127)    31612 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/dec/prefix.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5659 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/dec/state.c
--rw-rw-r--   0 runner    (1001) docker     (127)    12546 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/dec/state.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/
--rw-rw-r--   0 runner    (1001) docker     (127)     5673 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/backward_references.c
--rw-rw-r--   0 runner    (1001) docker     (127)     1301 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/backward_references.h
--rw-rw-r--   0 runner    (1001) docker     (127)    36639 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/backward_references_hq.c
--rw-rw-r--   0 runner    (1001) docker     (127)     3868 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/backward_references_hq.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8181 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/backward_references_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)      813 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/bit_cost.c
--rw-rw-r--   0 runner    (1001) docker     (127)     1685 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/bit_cost.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4109 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/bit_cost_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1137 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/block_encoder_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7395 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/block_splitter.c
--rw-rw-r--   0 runner    (1001) docker     (127)     1674 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/block_splitter.h
--rw-rw-r--   0 runner    (1001) docker     (127)    18673 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/block_splitter_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)    50750 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/brotli_bit_stream.c
--rw-rw-r--   0 runner    (1001) docker     (127)     3477 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/brotli_bit_stream.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1485 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/cluster.c
--rw-rw-r--   0 runner    (1001) docker     (127)     1024 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/cluster.h
--rw-rw-r--   0 runner    (1001) docker     (127)    11826 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/cluster_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1019 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/command.c
--rw-rw-r--   0 runner    (1001) docker     (127)     6892 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/command.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6645 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/compound_dictionary.c
--rw-rw-r--   0 runner    (1001) docker     (127)     2493 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/compound_dictionary.h
--rw-rw-r--   0 runner    (1001) docker     (127)    33255 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/compress_fragment.c
--rw-rw-r--   0 runner    (1001) docker     (127)     3598 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/compress_fragment.h
--rw-rw-r--   0 runner    (1001) docker     (127)    27182 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/compress_fragment_two_pass.c
--rw-rw-r--   0 runner    (1001) docker     (127)     2879 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/compress_fragment_two_pass.h
--rw-rw-r--   0 runner    (1001) docker     (127)   147154 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/dictionary_hash.c
--rw-rw-r--   0 runner    (1001) docker     (127)      646 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/dictionary_hash.h
--rw-rw-r--   0 runner    (1001) docker     (127)    77547 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/encode.c
--rw-rw-r--   0 runner    (1001) docker     (127)    23290 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/encoder_dict.c
--rw-rw-r--   0 runner    (1001) docker     (127)     5046 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/encoder_dict.h
--rw-rw-r--   0 runner    (1001) docker     (127)    14584 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/entropy_encode.c
--rw-rw-r--   0 runner    (1001) docker     (127)     4057 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/entropy_encode.h
--rw-rw-r--   0 runner    (1001) docker     (127)    32951 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/entropy_encode_static.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6024 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/fast_log.c
--rw-rw-r--   0 runner    (1001) docker     (127)     1650 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/fast_log.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2194 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/find_match_length.h
--rw-rw-r--   0 runner    (1001) docker     (127)    24481 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5097 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_composite_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)    11250 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_forgetful_chain_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)    10413 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_longest_match64_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)    10349 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_longest_match_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9414 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_longest_match_quickly_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7226 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_rolling_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)    13081 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_to_binary_tree_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3229 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/histogram.c
--rw-rw-r--   0 runner    (1001) docker     (127)     1875 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/histogram.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1401 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/histogram_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5839 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/literal_cost.c
--rw-rw-r--   0 runner    (1001) docker     (127)      916 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/literal_cost.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5630 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/memory.c
--rw-rw-r--   0 runner    (1001) docker     (127)     4358 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/memory.h
--rw-rw-r--   0 runner    (1001) docker     (127)    26659 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/metablock.c
--rw-rw-r--   0 runner    (1001) docker     (127)     4051 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/metablock.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7642 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/metablock_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1169 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/params.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1969 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/prefix.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7592 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/quality.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6009 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/ringbuffer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3040 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/state.h
--rw-rw-r--   0 runner    (1001) docker     (127)    21117 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/static_dict.c
--rw-rw-r--   0 runner    (1001) docker     (127)     1275 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/static_dict.h
--rw-rw-r--   0 runner    (1001) docker     (127)   469710 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/static_dict_lut.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2269 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/utf8_util.c
--rw-rw-r--   0 runner    (1001) docker     (127)      905 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/utf8_util.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2862 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/enc/write_bits.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/fuzz/
--rw-rw-r--   0 runner    (1001) docker     (127)      338 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/fuzz/BUILD.bazel
--rw-rw-r--   0 runner    (1001) docker     (127)      615 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/fuzz/WORKSPACE.bazel
--rw-rw-r--   0 runner    (1001) docker     (127)     1837 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/fuzz/decode_fuzzer.c
--rw-rw-r--   0 runner    (1001) docker     (127)     1073 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/fuzz/run_decode_fuzzer.c
--rwxrwxr-x   0 runner    (1001) docker     (127)      703 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/fuzz/test_fuzzer.sh
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/include/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/include/brotli/
--rw-rw-r--   0 runner    (1001) docker     (127)    16886 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/include/brotli/decode.h
--rw-rw-r--   0 runner    (1001) docker     (127)    19841 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/include/brotli/encode.h
--rw-rw-r--   0 runner    (1001) docker     (127)    11439 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/include/brotli/port.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3535 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/include/brotli/shared_dictionary.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2615 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/include/brotli/types.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/tools/
--rw-rw-r--   0 runner    (1001) docker     (127)    51996 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/tools/brotli.c
--rw-rw-r--   0 runner    (1001) docker     (127)     4028 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/c/tools/brotli.md
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/docs/
--rw-rw-r--   0 runner    (1001) docker     (127)   215208 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/docs/brotli-comparison-study-2015-09-22.pdf
--rw-rw-r--   0 runner    (1001) docker     (127)     5130 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/docs/brotli.1
--rw-rw-r--   0 runner    (1001) docker     (127)      244 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/docs/brotli.svg
--rw-rw-r--   0 runner    (1001) docker     (127)     1767 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/docs/constants.h.3
--rw-rw-r--   0 runner    (1001) docker     (127)    17452 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/docs/decode.h.3
--rw-rw-r--   0 runner    (1001) docker     (127)    24109 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/docs/encode.h.3
--rw-rw-r--   0 runner    (1001) docker     (127)     3081 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/docs/types.h.3
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/fetch-spec/
--rw-rw-r--   0 runner    (1001) docker     (127)     6077 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/fetch-spec/shared-brotli-fetch-spec.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/scripts/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/scripts/dictionary/
--rw-rw-r--   0 runner    (1001) docker     (127)      176 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/scripts/dictionary/README.md
--rw-rw-r--   0 runner    (1001) docker     (127)      375 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/scripts/dictionary/step-01-download-rfc.py
--rw-rw-r--   0 runner    (1001) docker     (127)      882 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/scripts/dictionary/step-02-rfc-to-bin.py
--rw-rw-r--   0 runner    (1001) docker     (127)      875 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/scripts/dictionary/step-03-validate-bin.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2214 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/scripts/dictionary/step-04-generate-java-literals.py
--rwxrwxr-x   0 runner    (1001) docker     (127)      283 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/scripts/download_testdata.sh
--rw-rw-r--   0 runner    (1001) docker     (127)      273 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/scripts/libbrotlicommon.pc.in
--rw-rw-r--   0 runner    (1001) docker     (127)      300 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/scripts/libbrotlidec.pc.in
--rw-rw-r--   0 runner    (1001) docker     (127)      300 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/brotli/scripts/libbrotlienc.pc.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/fast_float/
--rw-rw-r--   0 runner    (1001) docker     (127)       92 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/fast_float/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/fast_float/include/
--rw-rw-r--   0 runner    (1001) docker     (127)    94376 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/fast_float/include/fast_float.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/fastpfor/
--rw-rw-r--   0 runner    (1001) docker     (127)      150 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/fastpfor/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    10273 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/fastpfor/LICENSE
--rw-rw-r--   0 runner    (1001) docker     (127)     1278 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/fastpfor/README
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/
--rw-rw-r--   0 runner    (1001) docker     (127)    59414 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/bitpacking.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    32124 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/bitpacking.h
--rw-rw-r--   0 runner    (1001) docker     (127)    23572 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/bitpackinghelpers.h
--rw-rw-r--   0 runner    (1001) docker     (127)      273 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/common.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/glob/
--rw-rw-r--   0 runner    (1001) docker     (127)      100 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/glob/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/glob/glob/
--rw-rw-r--   0 runner    (1001) docker     (127)    13001 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/glob/glob/glob.hpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/httplib/
--rw-rw-r--   0 runner    (1001) docker     (127)   311527 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/httplib/httplib.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/
--rw-rw-r--   0 runner    (1001) docker     (127)      918 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    11358 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/LICENSE
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/include/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/
--rw-rw-r--   0 runner    (1001) docker     (127)    26550 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/aes.h
--rw-rw-r--   0 runner    (1001) docker     (127)    15024 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/aria.h
--rw-rw-r--   0 runner    (1001) docker     (127)    25694 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/asn1.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3085 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/base64.h
--rw-rw-r--   0 runner    (1001) docker     (127)    42463 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/bignum.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2394 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/build_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)    13062 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/camellia.h
--rw-rw-r--   0 runner    (1001) docker     (127)    25326 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/ccm.h
--rw-rw-r--   0 runner    (1001) docker     (127)    38245 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/check_config.h
--rw-rw-r--   0 runner    (1001) docker     (127)    51905 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/cipher.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1452 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/constant_time.h
--rw-rw-r--   0 runner    (1001) docker     (127)    11057 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/des.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9867 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/entropy.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7031 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/error.h
--rw-rw-r--   0 runner    (1001) docker     (127)    16632 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/gcm.h
--rw-rw-r--   0 runner    (1001) docker     (127)      531 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/mbedtls_config.h
--rw-rw-r--   0 runner    (1001) docker     (127)    17120 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/md.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4949 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/memory_buffer_alloc.h
--rw-rw-r--   0 runner    (1001) docker     (127)    41167 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/oid.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5270 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/pem.h
--rw-rw-r--   0 runner    (1001) docker     (127)    35543 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/pk.h
--rw-rw-r--   0 runner    (1001) docker     (127)    14433 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/platform.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1973 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/platform_time.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8667 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/platform_util.h
--rw-rw-r--   0 runner    (1001) docker     (127)      978 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/private_access.h
--rw-rw-r--   0 runner    (1001) docker     (127)    51957 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/rsa.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7854 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/sha1.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6640 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/sha256.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7084 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/sha512.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/library/
--rw-rw-r--   0 runner    (1001) docker     (127)    73166 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/library/aes.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    36996 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/library/aria.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11007 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/library/asn1parse.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6762 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/library/base64.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    79733 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/library/bignum.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    56414 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/library/bn_mul.h
--rw-rw-r--   0 runner    (1001) docker     (127)    36100 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/library/camellia.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    47452 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/library/cipher.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    49271 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/library/cipher_wrap.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4532 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/library/cipher_wrap.h
--rw-rw-r--   0 runner    (1001) docker     (127)    17543 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/library/common.h
--rw-rw-r--   0 runner    (1001) docker     (127)    26150 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/library/constant_time.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    12167 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/library/constant_time_internal.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1638 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/library/constant_time_invasive.h
--rw-rw-r--   0 runner    (1001) docker     (127)    18774 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/library/entropy.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6513 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/library/entropy_poll.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2139 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/library/entropy_poll.h
--rw-rw-r--   0 runner    (1001) docker     (127)    34742 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/library/gcm.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    21294 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/library/md.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2086 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/library/md_wrap.h
--rw-rw-r--   0 runner    (1001) docker     (127)    27822 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/library/oid.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    14294 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/library/pem.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    17719 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/library/pk.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    29099 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/library/pk_wrap.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4205 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/library/pk_wrap.h
--rw-rw-r--   0 runner    (1001) docker     (127)    44156 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/library/pkparse.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5125 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/library/platform_util.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    69416 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/library/rsa.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    13253 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/library/rsa_alt_helpers.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8442 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/library/rsa_alt_helpers.h
--rw-rw-r--   0 runner    (1001) docker     (127)    15171 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/library/sha1.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    16212 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/library/sha256.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    18253 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/mbedtls/library/sha512.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/
--rw-rw-r--   0 runner    (1001) docker     (127)     1079 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       46 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/LICENSE
--rw-rw-r--   0 runner    (1001) docker     (127)      976 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/Makefile
--rw-rw-r--   0 runner    (1001) docker     (127)     1879 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/README.md
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/
--rw-rw-r--   0 runner    (1001) docker     (127)      320 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/parquet_constants.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      406 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/parquet_constants.h
--rw-rw-r--   0 runner    (1001) docker     (127)   200148 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/parquet_types.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    72715 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/parquet_types.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1262 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/windows_compatibility.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/
--rwxrwxr-x   0 runner    (1001) docker     (127)     9816 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-internal.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     3296 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-sinksource.cc
--rwxrwxr-x   0 runner    (1001) docker     (127)     7266 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-sinksource.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1837 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-stubs-internal.cc
--rwxrwxr-x   0 runner    (1001) docker     (127)    15040 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-stubs-internal.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     2900 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-stubs-public.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    59102 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy.cc
--rwxrwxr-x   0 runner    (1001) docker     (127)     9748 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/
--rw-rw-r--   0 runner    (1001) docker     (127)     3555 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/TApplicationException.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1208 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/TBase.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     6849 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/TLogging.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     3185 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/TToString.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     3470 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/Thrift.h
--rw-rw-r--   0 runner    (1001) docker     (127)       65 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/config.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/
--rwxrwxr-x   0 runner    (1001) docker     (127)     7931 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TCompactProtocol.h
--rw-rw-r--   0 runner    (1001) docker     (127)    23953 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TCompactProtocol.tcc
--rwxrwxr-x   0 runner    (1001) docker     (127)     1140 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocol.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)    21319 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocol.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     6374 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocolDecorator.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     3216 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocolException.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1151 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocolTypes.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    18266 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TVirtualProtocol.h
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/stdcxx.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      896 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/thrift-config.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      460 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/thrift_export.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/
--rw-rw-r--   0 runner    (1001) docker     (127)     4624 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/PlatformSocket.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     3699 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TBufferTransports.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)    15004 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TBufferTransports.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     9004 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TTransport.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1862 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TTransportException.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3335 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TTransportException.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     5167 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TVirtualTransport.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniz/
--rw-rw-r--   0 runner    (1001) docker     (127)      192 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniz/CMakeLists.txt
--rwxrwxr-x   0 runner    (1001) docker     (127)     1184 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniz/LICENSE
--rwxrwxr-x   0 runner    (1001) docker     (127)   313123 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniz/miniz.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)    66103 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniz/miniz.hpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5058 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/miniz/miniz_wrapper.hpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/nlohmann_json/
--rw-rw-r--   0 runner    (1001) docker     (127)   907860 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/nlohmann_json/json.hpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6268 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/nlohmann_json/json_fwd.hpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pcg/
--rw-rw-r--   0 runner    (1001) docker     (127)     1092 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pcg/LICENSE
--rw-rw-r--   0 runner    (1001) docker     (127)    20241 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pcg/pcg_extras.hpp
--rw-rw-r--   0 runner    (1001) docker     (127)    73551 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pcg/pcg_random.hpp
--rw-rw-r--   0 runner    (1001) docker     (127)    24875 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pcg/pcg_uint128.hpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/
--rw-rw-r--   0 runner    (1001) docker     (127)    11983 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1684 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/LICENSE
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/include/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/
--rw-rw-r--   0 runner    (1001) docker     (127)    23979 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/attr.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7069 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/buffer_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)    65560 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/cast.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8458 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/chrono.h
--rw-rw-r--   0 runner    (1001) docker     (127)      120 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/common.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2096 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/complex.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/
--rw-rw-r--   0 runner    (1001) docker     (127)    28251 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/class.h
--rw-rw-r--   0 runner    (1001) docker     (127)    52330 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/common.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5491 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/descr.h
--rw-rw-r--   0 runner    (1001) docker     (127)    17932 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/init.h
--rw-rw-r--   0 runner    (1001) docker     (127)    26305 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/internals.h
--rw-rw-r--   0 runner    (1001) docker     (127)    42266 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/type_caster_base.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1625 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/typeid.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eigen/
--rw-rw-r--   0 runner    (1001) docker     (127)    31418 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eigen/matrix.h
--rw-rw-r--   0 runner    (1001) docker     (127)    18120 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eigen/tensor.h
--rw-rw-r--   0 runner    (1001) docker     (127)      316 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eigen.h
--rw-rw-r--   0 runner    (1001) docker     (127)    11889 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/embed.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4731 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eval.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5002 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/functional.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8262 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/gil.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8862 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/iostream.h
--rw-rw-r--   0 runner    (1001) docker     (127)    79412 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/numpy.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9103 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/operators.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/options.h
--rw-rw-r--   0 runner    (1001) docker     (127)   126075 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/pybind11.h
--rw-rw-r--   0 runner    (1001) docker     (127)    93433 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/pytypes.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/stl/
--rw-rw-r--   0 runner    (1001) docker     (127)     4185 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/stl/filesystem.h
--rw-rw-r--   0 runner    (1001) docker     (127)    15337 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/stl.h
--rw-rw-r--   0 runner    (1001) docker     (127)    27013 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/stl_bind.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/tools/
--rw-rw-r--   0 runner    (1001) docker     (127)     2350 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/tools/FindCatch.cmake
--rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/tools/FindEigen3.cmake
--rw-rw-r--   0 runner    (1001) docker     (127)    11103 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/tools/FindPythonLibsNew.cmake
--rw-rw-r--   0 runner    (1001) docker     (127)      817 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/tools/JoinPaths.cmake
--rw-rw-r--   0 runner    (1001) docker     (127)     1423 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/tools/check-style.sh
--rw-rw-r--   0 runner    (1001) docker     (127)      952 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/tools/cmake_uninstall.cmake.in
--rw-rw-r--   0 runner    (1001) docker     (127)     1040 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/tools/codespell_ignore_lines_from_errors.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1031 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/tools/libsize.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1282 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/tools/make_changelog.py
--rw-rw-r--   0 runner    (1001) docker     (127)      196 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11.pc.in
--rw-rw-r--   0 runner    (1001) docker     (127)    13487 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11Common.cmake
--rw-rw-r--   0 runner    (1001) docker     (127)     6930 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11Config.cmake.in
--rw-rw-r--   0 runner    (1001) docker     (127)     8957 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11NewTools.cmake
--rw-rw-r--   0 runner    (1001) docker     (127)     8361 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11Tools.cmake
--rw-rw-r--   0 runner    (1001) docker     (127)       94 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/tools/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)     2104 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/tools/setup_global.py.in
--rw-rw-r--   0 runner    (1001) docker     (127)     1234 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pybind11/tools/setup_main.py.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pyparse/
--rw-rw-r--   0 runner    (1001) docker     (127)     4660 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/pyparse/pyparse.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/
--rw-rw-r--   0 runner    (1001) docker     (127)     2716 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1558 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/LICENSE
--rw-rw-r--   0 runner    (1001) docker     (127)    12166 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/bitstate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    40923 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/compile.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    77669 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/dfa.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3379 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/filtered_re2.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/include/
--rw-rw-r--   0 runner    (1001) docker     (127)     2794 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/include/bitmap256.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4074 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/include/filtered_re2.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3685 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/include/logging.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1027 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/include/mix.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4596 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/include/mutex.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1051 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/include/pod_array.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4107 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/include/prefilter.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5397 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/include/prefilter_tree.h
--rw-rw-r--   0 runner    (1001) docker     (127)    20055 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/include/prog.h
--rw-rw-r--   0 runner    (1001) docker     (127)    41735 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/include/re2.h
--rw-rw-r--   0 runner    (1001) docker     (127)    25053 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/include/regexp.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2528 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/include/set.h
--rw-rw-r--   0 runner    (1001) docker     (127)    12285 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/include/sparse_array.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7425 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/include/sparse_set.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6625 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/include/stringpiece.h
--rw-rw-r--   0 runner    (1001) docker     (127)      644 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/include/strutil.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2606 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/include/unicode_casefold.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1595 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/include/unicode_groups.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1575 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/include/utf.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1028 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/include/util.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7825 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/include/walker-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6308 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/mimics_pcre.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    22890 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/nfa.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    22239 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/onepass.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    81544 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/parse.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3448 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/perl_groups.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    18698 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/prefilter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    13255 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/prefilter_tree.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    40537 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/prog.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    42418 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/re2.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    28640 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/regexp.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5872 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/rune.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4636 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/set.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    20853 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/simplify.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2118 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/stringpiece.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5691 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/strutil.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9029 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/tostring.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    13413 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/unicode_casefold.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)   122482 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/re2/unicode_groups.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/serd/
--rw-rw-r--   0 runner    (1001) docker     (127)     1247 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/serd/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/serd/include/
--rw-rw-r--   0 runner    (1001) docker     (127)    33294 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/serd/include/serd.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/serd/src/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/serd/src/LICENSES/
--rw-rw-r--   0 runner    (1001) docker     (127)     1424 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/serd/src/LICENSES/BSD-3-Clause.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      660 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/serd/src/LICENSES/OBSD.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      555 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/serd/src/attributes.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3172 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/serd/src/base64.c
--rw-rw-r--   0 runner    (1001) docker     (127)     1024 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/serd/src/base64.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1966 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/serd/src/byte_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2643 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/serd/src/byte_source.c
--rw-rw-r--   0 runner    (1001) docker     (127)     3444 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/serd/src/byte_source.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6676 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/serd/src/env.c
--rw-rw-r--   0 runner    (1001) docker     (127)    46487 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/serd/src/n3.c
--rw-rw-r--   0 runner    (1001) docker     (127)     9699 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/serd/src/node.c
--rw-rw-r--   0 runner    (1001) docker     (127)      871 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/serd/src/node.h
--rw-rw-r--   0 runner    (1001) docker     (127)    12064 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/serd/src/reader.c
--rw-rw-r--   0 runner    (1001) docker     (127)     4376 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/serd/src/reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3187 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/serd/src/serd_config.h
--rw-rw-r--   0 runner    (1001) docker     (127)      730 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/serd/src/serd_internal.h
--rw-rw-r--   0 runner    (1001) docker     (127)    10745 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/serd/src/serdi.c
--rw-rw-r--   0 runner    (1001) docker     (127)     2552 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/serd/src/stack.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3507 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/serd/src/string.c
--rw-rw-r--   0 runner    (1001) docker     (127)     3394 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/serd/src/string_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1233 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/serd/src/system.c
--rw-rw-r--   0 runner    (1001) docker     (127)      650 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/serd/src/system.h
--rw-rw-r--   0 runner    (1001) docker     (127)      546 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/serd/src/try.h
--rw-rw-r--   0 runner    (1001) docker     (127)    11749 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/serd/src/uri.c
--rw-rw-r--   0 runner    (1001) docker     (127)     2843 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/serd/src/uri_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)    36427 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/serd/src/writer.c
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/
--rw-rw-r--   0 runner    (1001) docker     (127)     1348 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/LICENSE
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/
--rw-rw-r--   0 runner    (1001) docker     (127)     4021 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/async.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2817 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/async_logger-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2560 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/async_logger.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/
--rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/argv.h
--rw-rw-r--   0 runner    (1001) docker     (127)      986 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/env.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3170 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/helpers-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)      718 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/helpers.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2050 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/common-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)    13194 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/common.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/
--rw-rw-r--   0 runner    (1001) docker     (127)     2004 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/backtracer-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1165 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/backtracer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3349 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/circular_q.h
--rw-rw-r--   0 runner    (1001) docker     (127)      603 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/console_globals.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4707 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/file_helper-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1758 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/file_helper.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4471 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/fmt_helper.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1396 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/log_msg-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1204 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/log_msg.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1668 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/log_msg_buffer-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)      935 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/log_msg_buffer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5285 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/mpmc_blocking_q.h
--rw-rw-r--   0 runner    (1001) docker     (127)      930 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/null_mutex.h
--rw-rw-r--   0 runner    (1001) docker     (127)    17897 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/os-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3922 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/os.h
--rw-rw-r--   0 runner    (1001) docker     (127)      620 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/periodic_worker-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1756 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/periodic_worker.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8695 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/registry-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4013 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/registry.h
--rw-rw-r--   0 runner    (1001) docker     (127)      751 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/synchronous_factory.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4252 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/tcp_client-windows.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3885 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/tcp_client.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4275 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/thread_pool-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3519 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/thread_pool.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3134 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/udp_client-windows.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2237 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/udp_client.h
--rw-rw-r--   0 runner    (1001) docker     (127)      188 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/windows_include.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/
--rw-rw-r--   0 runner    (1001) docker     (127)     7380 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bin_to_hex.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/
--rw-rw-r--   0 runner    (1001) docker     (127)     7420 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/args.h
--rw-rw-r--   0 runner    (1001) docker     (127)    68076 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/chrono.h
--rw-rw-r--   0 runner    (1001) docker     (127)    24896 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/color.h
--rw-rw-r--   0 runner    (1001) docker     (127)    21245 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/compile.h
--rw-rw-r--   0 runner    (1001) docker     (127)   111215 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/core.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1408 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/fmt.license.rst
--rw-rw-r--   0 runner    (1001) docker     (127)    74272 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/format-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)   154517 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/format.h
--rw-rw-r--   0 runner    (1001) docker     (127)      100 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/locale.h
--rw-rw-r--   0 runner    (1001) docker     (127)    14123 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/os.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7586 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/ostream.h
--rw-rw-r--   0 runner    (1001) docker     (127)    20023 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/printf.h
--rw-rw-r--   0 runner    (1001) docker     (127)    23218 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/ranges.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4880 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/std.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9001 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/xchar.h
--rw-rw-r--   0 runner    (1001) docker     (127)      551 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/chrono.h
--rw-rw-r--   0 runner    (1001) docker     (127)      559 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/compile.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1042 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/fmt.h
--rw-rw-r--   0 runner    (1001) docker     (127)      554 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/ostr.h
--rw-rw-r--   0 runner    (1001) docker     (127)      551 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/ranges.h
--rw-rw-r--   0 runner    (1001) docker     (127)      641 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/std.h
--rw-rw-r--   0 runner    (1001) docker     (127)      548 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/xchar.h
--rw-rw-r--   0 runner    (1001) docker     (127)      463 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/formatter.h
--rw-rw-r--   0 runner    (1001) docker     (127)      305 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fwd.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6725 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/logger-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)    13412 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/logger.h
--rw-rw-r--   0 runner    (1001) docker     (127)    44468 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/pattern_formatter-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3758 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/pattern_formatter.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/
--rw-rw-r--   0 runner    (1001) docker     (127)     4777 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/android_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4875 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/ansicolor_sink-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3959 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/ansicolor_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1808 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/base_sink-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1568 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/base_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1216 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/basic_file_sink-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2295 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/basic_file_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1705 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/callback_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9452 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/daily_file_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2373 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/dist_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3243 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/dup_filter_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7121 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/hourly_file_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4445 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/kafka_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4003 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/mongo_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2049 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/msvc_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1234 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/null_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1222 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/ostream_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)    12408 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/qt_sinks.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2081 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/ringbuffer_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4917 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/rotating_file_sink-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3229 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/rotating_file_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)      725 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/sink-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)      893 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1435 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/stdout_color_sinks-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1792 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/stdout_color_sinks.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4347 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/stdout_sinks-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2429 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/stdout_sinks.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4239 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/syslog_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4872 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/systemd_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2127 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/tcp_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1858 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/udp_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8888 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/win_eventlog_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6651 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/wincolor_sink-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2716 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/wincolor_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3118 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/spdlog-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)    11771 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/spdlog.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1711 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/stopwatch.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6360 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/tweakme.h
--rw-rw-r--   0 runner    (1001) docker     (127)      417 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/spdlog/spdlog/version.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/taywee_args/
--rw-rw-r--   0 runner    (1001) docker     (127)     1105 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/taywee_args/LICENSE
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/taywee_args/include/
--rw-rw-r--   0 runner    (1001) docker     (127)   152995 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/taywee_args/include/args.hxx
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/utf8proc/
--rw-rw-r--   0 runner    (1001) docker     (127)      142 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/utf8proc/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     5125 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/utf8proc/LICENSE.md
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/utf8proc/include/
--rw-rw-r--   0 runner    (1001) docker     (127)    32757 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/utf8proc/include/utf8proc.h
--rw-rw-r--   0 runner    (1001) docker     (127)  1944550 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/utf8proc/include/utf8proc_data.h
--rw-rw-r--   0 runner    (1001) docker     (127)      888 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/utf8proc/include/utf8proc_wrapper.h
--rw-rw-r--   0 runner    (1001) docker     (127)    37876 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/utf8proc/utf8proc.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4483 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/utf8proc/utf8proc_wrapper.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/
--rw-rw-r--   0 runner    (1001) docker     (127)     1194 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1529 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/LICENSE
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/common/
--rw-rw-r--   0 runner    (1001) docker     (127)     8580 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/common/entropy_common.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2982 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/common/error_private.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    10089 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/common/fse_decompress.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    28008 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/common/xxhash.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2721 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/common/zstd_common.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/compress/
--rw-rw-r--   0 runner    (1001) docker     (127)    26469 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/compress/fse_compress.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7555 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/compress/hist.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    32726 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/compress/huf_compress.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)   183732 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_compress.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6293 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_compress_literals.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    19309 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_compress_sequences.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    43614 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_compress_superblock.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    25428 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_double_fast.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    22459 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_fast.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    52956 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_lazy.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    25024 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_ldm.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    55766 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_opt.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/decompress/
--rw-rw-r--   0 runner    (1001) docker     (127)    51287 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/decompress/huf_decompress.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9136 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/decompress/zstd_ddict.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    83312 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/decompress/zstd_decompress.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    61618 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/decompress/zstd_decompress_block.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/include/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/include/zstd/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/
--rw-rw-r--   0 runner    (1001) docker     (127)    17857 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/bitstream.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5734 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/compiler.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3893 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/debug.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2396 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/error_private.h
--rw-rw-r--   0 runner    (1001) docker     (127)    14574 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/fse.h
--rw-rw-r--   0 runner    (1001) docker     (127)    18012 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/fse_static.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4717 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/huf.h
--rw-rw-r--   0 runner    (1001) docker     (127)    14332 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/huf_static.h
--rw-rw-r--   0 runner    (1001) docker     (127)    12217 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/mem.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9897 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/xxhash.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1779 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/xxhash_static.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3730 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/zstd_errors.h
--rw-rw-r--   0 runner    (1001) docker     (127)    13604 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/zstd_internal.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/
--rw-rw-r--   0 runner    (1001) docker     (127)     3464 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/hist.h
--rw-rw-r--   0 runner    (1001) docker     (127)    46030 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_compress_internal.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1262 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_compress_literals.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2210 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_compress_sequences.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1194 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_compress_superblock.h
--rw-rw-r--   0 runner    (1001) docker     (127)    18777 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_cwksp.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1250 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_double_fast.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1171 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_fast.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2701 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_lazy.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4010 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_ldm.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1972 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_opt.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/include/zstd/decompress/
--rw-rw-r--   0 runner    (1001) docker     (127)     1329 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/include/zstd/decompress/zstd_ddict.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2081 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/include/zstd/decompress/zstd_decompress_block.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6147 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/include/zstd/decompress/zstd_decompress_internal.h
--rw-rw-r--   0 runner    (1001) docker     (127)    61165 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/include/zstd.h
--rw-rw-r--   0 runner    (1001) docker     (127)    60974 2024-05-13 08:04:59.000000 sdist/kuzu-source/third_party/zstd/include/zstd_static.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/
--rw-rw-r--   0 runner    (1001) docker     (127)      297 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/benchmark/
--rw-rw-r--   0 runner    (1001) docker     (127)      251 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/benchmark/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     3132 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/benchmark/benchmark.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3400 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/benchmark/benchmark_runner.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/benchmark/example/
--rw-rw-r--   0 runner    (1001) docker     (127)       73 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/benchmark/example/example.benchmark
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/benchmark/include/
--rw-rw-r--   0 runner    (1001) docker     (127)      994 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/benchmark/include/benchmark.h
--rw-rw-r--   0 runner    (1001) docker     (127)      561 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/benchmark/include/benchmark_config.h
--rw-rw-r--   0 runner    (1001) docker     (127)      836 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/benchmark/include/benchmark_runner.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2195 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/benchmark/main.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/
--rw-rw-r--   0 runner    (1001) docker     (127)     1846 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      332 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/README.md
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/jni/
--rw-rw-r--   0 runner    (1001) docker     (127)    52884 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/jni/kuzu_java.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/main/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/main/java/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/
--rw-rw-r--   0 runner    (1001) docker     (127)     4861 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuConnection.java
--rw-rw-r--   0 runner    (1001) docker     (127)     3587 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuDataType.java
--rw-rw-r--   0 runner    (1001) docker     (127)      716 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuDataTypeID.java
--rw-rw-r--   0 runner    (1001) docker     (127)     2637 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuDatabase.java
--rw-rw-r--   0 runner    (1001) docker     (127)     1734 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuFlatTuple.java
--rw-rw-r--   0 runner    (1001) docker     (127)      495 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuInternalID.java
--rw-rw-r--   0 runner    (1001) docker     (127)     9598 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuNative.java
--rw-rw-r--   0 runner    (1001) docker     (127)      334 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuObjectRefDestroyedException.java
--rw-rw-r--   0 runner    (1001) docker     (127)     2023 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuPreparedStatement.java
--rw-rw-r--   0 runner    (1001) docker     (127)     5236 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuQueryResult.java
--rw-rw-r--   0 runner    (1001) docker     (127)      853 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuQuerySummary.java
--rw-rw-r--   0 runner    (1001) docker     (127)     4622 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValue.java
--rw-rw-r--   0 runner    (1001) docker     (127)     1077 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueListUtil.java
--rw-rw-r--   0 runner    (1001) docker     (127)     2984 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueNodeUtil.java
--rw-rw-r--   0 runner    (1001) docker     (127)     1034 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueRdfVariantUtil.java
--rw-rw-r--   0 runner    (1001) docker     (127)     1024 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueRecursiveRelUtil.java
--rw-rw-r--   0 runner    (1001) docker     (127)     3397 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueRelUtil.java
--rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueStructUtil.java
--rw-rw-r--   0 runner    (1001) docker     (127)      520 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuVersion.java
--rw-rw-r--   0 runner    (1001) docker     (127)      178 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/package-info.java
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/test/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/test/java/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/
--rw-rw-r--   0 runner    (1001) docker     (127)    11911 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/ConnectionTest.java
--rw-rw-r--   0 runner    (1001) docker     (127)     5025 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/DataTypeTest.java
--rw-rw-r--   0 runner    (1001) docker     (127)     1454 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/DatabaseTest.java
--rw-rw-r--   0 runner    (1001) docker     (127)      525 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/ExtensionTest.java
--rw-rw-r--   0 runner    (1001) docker     (127)     1865 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/FlatTupleTest.java
--rw-rw-r--   0 runner    (1001) docker     (127)     1663 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/PreparedStatementTest.java
--rw-rw-r--   0 runner    (1001) docker     (127)     4789 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/QueryResultTest.java
--rw-rw-r--   0 runner    (1001) docker     (127)      940 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/TestBase.java
--rw-rw-r--   0 runner    (1001) docker     (127)     2504 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/TestHelper.java
--rw-rw-r--   0 runner    (1001) docker     (127)    45229 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/ValueTest.java
--rw-rw-r--   0 runner    (1001) docker     (127)      471 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/VersionTest.java
--rw-rw-r--   0 runner    (1001) docker     (127)     2271 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/test.java
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/third_party/
--rw-rw-r--   0 runner    (1001) docker     (127)  2614186 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/java_api/third_party/junit-platform-console-standalone-1.9.3.jar
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/
--rw-rw-r--   0 runner    (1001) docker     (127)     1777 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     3043 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/README.md
--rw-rw-r--   0 runner    (1001) docker     (127)      397 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/build.js
--rw-rw-r--   0 runner    (1001) docker     (127)      615 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/clean.js
--rw-rw-r--   0 runner    (1001) docker     (127)     4452 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/install.js
--rw-rw-r--   0 runner    (1001) docker     (127)     5577 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/package.js
--rw-rw-r--   0 runner    (1001) docker     (127)      672 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/package.json
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/
--rw-rw-r--   0 runner    (1001) docker     (127)     4385 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_connection.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1567 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1635 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_prepared_statement.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5760 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_query_result.h
--rw-rw-r--   0 runner    (1001) docker     (127)      620 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_util.h
--rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/main.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4098 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_connection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2332 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2110 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_prepared_statement.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4835 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_query_result.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    14214 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_util.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/src_js/
--rw-rw-r--   0 runner    (1001) docker     (127)    10896 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/src_js/connection.js
--rw-rw-r--   0 runner    (1001) docker     (127)     4009 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/src_js/database.js
--rw-rw-r--   0 runner    (1001) docker     (127)      499 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/src_js/index.js
--rw-rw-r--   0 runner    (1001) docker     (127)      686 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/src_js/kuzu_native.js
--rw-rw-r--   0 runner    (1001) docker     (127)      238 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/src_js/logging_level.js
--rw-rw-r--   0 runner    (1001) docker     (127)     1210 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/src_js/prepared_statement.js
--rw-rw-r--   0 runner    (1001) docker     (127)     4951 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/src_js/query_result.js
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/test/
--rw-rw-r--   0 runner    (1001) docker     (127)     2212 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/test/common.js
--rw-rw-r--   0 runner    (1001) docker     (127)      629 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/test/test.js
--rw-rw-r--   0 runner    (1001) docker     (127)     3089 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/test/test_concurrency.js
--rw-rw-r--   0 runner    (1001) docker     (127)     9201 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/test/test_connection.js
--rw-rw-r--   0 runner    (1001) docker     (127)    19348 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/test/test_data_type.js
--rw-rw-r--   0 runner    (1001) docker     (127)    10088 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/test/test_database.js
--rw-rw-r--   0 runner    (1001) docker     (127)      266 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/test/test_extension.js
--rw-rw-r--   0 runner    (1001) docker     (127)    10191 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/test/test_parameter.js
--rw-rw-r--   0 runner    (1001) docker     (127)     6242 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/test/test_query_result.js
--rw-rw-r--   0 runner    (1001) docker     (127)      384 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/nodejs_api/test/test_version.js
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/
--rw-rw-r--   0 runner    (1001) docker     (127)     1322 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1136 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/Makefile
--rw-rw-r--   0 runner    (1001) docker     (127)       23 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/README.md
--rw-rw-r--   0 runner    (1001) docker     (127)     2381 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      203 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/requirements_dev.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/cached_import/
--rw-rw-r--   0 runner    (1001) docker     (127)      376 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/cached_import/py_cached_import.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      618 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/cached_import/py_cached_item.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/
--rw-rw-r--   0 runner    (1001) docker     (127)      335 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/arrow_array.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/cached_import/
--rw-rw-r--   0 runner    (1001) docker     (127)      711 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/cached_import/py_cached_import.h
--rw-rw-r--   0 runner    (1001) docker     (127)      521 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/cached_import/py_cached_item.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3938 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/cached_import/py_cached_modules.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/numpy/
--rw-rw-r--   0 runner    (1001) docker     (127)      430 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/numpy/numpy_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1379 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/numpy/numpy_type.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/
--rw-rw-r--   0 runner    (1001) docker     (127)      718 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/pandas_analyzer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1290 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/pandas_bind.h
--rw-rw-r--   0 runner    (1001) docker     (127)      931 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/pandas_column.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1959 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/pandas_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1674 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_connection.h
--rw-rw-r--   0 runner    (1001) docker     (127)      714 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_conversion.h
--rw-rw-r--   0 runner    (1001) docker     (127)      940 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      676 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_object_container.h
--rw-rw-r--   0 runner    (1001) docker     (127)      381 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_prepared_statement.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1470 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_query_result.h
--rw-rw-r--   0 runner    (1001) docker     (127)      709 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_query_result_converter.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1031 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_str_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)      379 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_udf.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pyarrow/
--rw-rw-r--   0 runner    (1001) docker     (127)      383 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pyarrow/pyarrow_bind.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2219 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pyarrow/pyarrow_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)      202 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pybind_include.h
--rw-rw-r--   0 runner    (1001) docker     (127)      549 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/kuzu_binding.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/numpy/
--rw-rw-r--   0 runner    (1001) docker     (127)     9637 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/numpy/numpy_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5514 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/numpy/numpy_type.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/pandas/
--rw-rw-r--   0 runner    (1001) docker     (127)     3945 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/pandas/pandas_analyzer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3943 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/pandas/pandas_bind.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6572 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/pandas/pandas_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    21636 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_connection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4462 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_conversion.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3624 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      564 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_prepared_statement.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    16192 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_query_result.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7703 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_query_result_converter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7733 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_udf.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/pyarrow/
--rw-rw-r--   0 runner    (1001) docker     (127)      866 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/pyarrow/pyarrow_bind.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4410 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_cpp/pyarrow/pyarrow_scan.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_py/
--rw-rw-r--   0 runner    (1001) docker     (127)     2111 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_py/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     8353 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_py/connection.py
--rw-rw-r--   0 runner    (1001) docker     (127)     9620 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_py/database.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1167 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_py/prepared_statement.py
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_py/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)    14470 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_py/query_result.py
--rw-rw-r--   0 runner    (1001) docker     (127)     7586 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_py/torch_geometric_feature_store.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4893 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_py/torch_geometric_graph_store.py
--rw-rw-r--   0 runner    (1001) docker     (127)    13467 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_py/torch_geometric_result_converter.py
--rw-rw-r--   0 runner    (1001) docker     (127)      839 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/src_py/types.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/test/
--rw-rw-r--   0 runner    (1001) docker     (127)     5545 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/test/conftest.py
--rw-rw-r--   0 runner    (1001) docker     (127)    14438 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/test/ground_truth.py
--rw-rw-r--   0 runner    (1001) docker     (127)    24584 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/test/test_arrow.py
--rw-rw-r--   0 runner    (1001) docker     (127)      879 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/test/test_connection.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2687 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/test/test_database.py
--rw-rw-r--   0 runner    (1001) docker     (127)    12786 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/test/test_datatype.py
--rw-rw-r--   0 runner    (1001) docker     (127)    20051 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/test/test_df.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2331 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/test/test_exception.py
--rw-rw-r--   0 runner    (1001) docker     (127)      247 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/test/test_extension.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1947 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/test/test_get_header.py
--rw-rw-r--   0 runner    (1001) docker     (127)      222 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/test/test_helper.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4300 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/test/test_issue.py
--rw-rw-r--   0 runner    (1001) docker     (127)    10889 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/test/test_networkx.py
--rw-rw-r--   0 runner    (1001) docker     (127)     8013 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/test/test_parameter.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4511 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/test/test_prepared_statement.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1780 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/test/test_query_result.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1258 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/test/test_query_result_close.py
--rw-rw-r--   0 runner    (1001) docker     (127)    14156 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/test/test_scan_pandas.py
--rw-rw-r--   0 runner    (1001) docker     (127)    24852 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/test/test_scan_pandas_pyarrow.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1422 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/test/test_scan_polars.py
--rw-rw-r--   0 runner    (1001) docker     (127)      345 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/test/test_timeout.py
--rw-rw-r--   0 runner    (1001) docker     (127)    30361 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/test/test_torch_geometric.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4105 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/test/test_torch_geometric_remote_backend.py
--rw-rw-r--   0 runner    (1001) docker     (127)     5062 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/test/test_udf.py
--rw-rw-r--   0 runner    (1001) docker     (127)      155 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/test/test_version.py
--rw-rw-r--   0 runner    (1001) docker     (127)      215 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/python_api/test/type_aliases.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/rust_api/
--rw-rw-r--   0 runner    (1001) docker     (127)        7 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/rust_api/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (127)    25753 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/rust_api/Cargo.lock
--rw-rw-r--   0 runner    (1001) docker     (127)     1099 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/rust_api/Cargo.toml
--rw-rw-r--   0 runner    (1001) docker     (127)     5702 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/rust_api/build.rs
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/rust_api/include/
--rw-rw-r--   0 runner    (1001) docker     (127)      345 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/rust_api/include/kuzu_arrow.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9653 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/rust_api/include/kuzu_rs.h
-lrwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-05-13 08:05:02.679662 sdist/kuzu-source/tools/rust_api/kuzu-src -> ../..
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/rust_api/src/
--rw-rw-r--   0 runner    (1001) docker     (127)      380 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/rust_api/src/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    13653 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/rust_api/src/connection.rs
--rw-rw-r--   0 runner    (1001) docker     (127)     5847 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/rust_api/src/database.rs
--rw-rw-r--   0 runner    (1001) docker     (127)     1763 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/rust_api/src/error.rs
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/rust_api/src/ffi/
--rw-rw-r--   0 runner    (1001) docker     (127)     1123 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/rust_api/src/ffi/arrow.rs
--rw-rw-r--   0 runner    (1001) docker     (127)    12852 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/rust_api/src/ffi.rs
--rw-rw-r--   0 runner    (1001) docker     (127)      471 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/rust_api/src/kuzu_arrow.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11867 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/rust_api/src/kuzu_rs.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2508 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/rust_api/src/lib.rs
--rw-rw-r--   0 runner    (1001) docker     (127)    12831 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/rust_api/src/logical_type.rs
--rw-rw-r--   0 runner    (1001) docker     (127)     9355 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/rust_api/src/query_result.rs
--rw-rw-r--   0 runner    (1001) docker     (127)     2629 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/rust_api/src/rdf_variant.rs
--rw-rw-r--   0 runner    (1001) docker     (127)    67772 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/rust_api/src/value.rs
--rw-rw-r--   0 runner    (1001) docker     (127)     1730 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/rust_api/update_version.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/shell/
--rw-rw-r--   0 runner    (1001) docker     (127)      428 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/shell/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    27765 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/shell/embedded_shell.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/shell/include/
--rw-rw-r--   0 runner    (1001) docker     (127)      912 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/shell/include/embedded_shell.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3116 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/shell/include/linenoise.h
--rw-rw-r--   0 runner    (1001) docker     (127)    79992 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/shell/linenoise.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3257 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/shell/shell_runner.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/shell/test/
--rw-rw-r--   0 runner    (1001) docker     (127)     5371 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/shell/test/conftest.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/shell/test/files/
--rw-rw-r--   0 runner    (1001) docker     (127)     3075 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/shell/test/files/vPerson.csv
--rw-rw-r--   0 runner    (1001) docker     (127)     1399 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/shell/test/test_helper.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4790 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/shell/test/test_shell_basics.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4804 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/shell/test/test_shell_commands.py
--rw-rw-r--   0 runner    (1001) docker     (127)    11969 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/shell/test/test_shell_control_edit.py
--rw-rw-r--   0 runner    (1001) docker     (127)    12995 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/shell/test/test_shell_control_search.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4297 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/shell/test/test_shell_esc_edit.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4571 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/shell/test/test_shell_esc_search.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4904 2024-05-13 08:04:59.000000 sdist/kuzu-source/tools/shell/test/test_shell_flags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:05:04.487664 sdist/kuzu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-05-13 08:05:04.487664 sdist/kuzu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-13 08:05:04.491664 sdist/kuzu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 08:05:04.487664 sdist/kuzu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-13 08:05:04.487664 sdist/kuzu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 08:05:04.487664 sdist/kuzu.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-13 08:05:02.927662 sdist/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-13 08:04:58.643657 sdist/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-05-13 08:04:58.643657 sdist/setup.py
+drwx------   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:48.755430 sdist/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-14 08:04:42.399441 sdist/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-14 08:04:44.011436 sdist/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-14 08:04:42.399441 sdist/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-05-14 08:04:44.011436 sdist/README_PYTHON_BUILD.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:47.903432 sdist/kuzu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:47.903432 sdist/kuzu-source/
+-rw-rw-r--   0 runner    (1001) docker     (127)     5560 2024-05-14 08:04:44.000000 sdist/kuzu-source/.clang-format
+-rw-rw-r--   0 runner    (1001) docker     (127)      948 2024-05-14 08:04:44.000000 sdist/kuzu-source/.clang-tidy
+-rw-rw-r--   0 runner    (1001) docker     (127)      332 2024-05-14 08:04:44.000000 sdist/kuzu-source/.clang-tidy-analyzer
+-rw-rw-r--   0 runner    (1001) docker     (127)     1000 2024-05-14 08:04:44.000000 sdist/kuzu-source/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (127)       47 2024-05-14 08:04:44.000000 sdist/kuzu-source/.lcovrc
+-rw-rw-r--   0 runner    (1001) docker     (127)     8632 2024-05-14 08:04:44.000000 sdist/kuzu-source/CLA.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     9475 2024-05-14 08:04:44.000000 sdist/kuzu-source/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      632 2024-05-14 08:04:44.000000 sdist/kuzu-source/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     2052 2024-05-14 08:04:44.000000 sdist/kuzu-source/CONTRIBUTING.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     1072 2024-05-14 08:04:44.000000 sdist/kuzu-source/LICENSE
+-rw-rw-r--   0 runner    (1001) docker     (127)     6896 2024-05-14 08:04:44.000000 sdist/kuzu-source/Makefile
+-rw-rw-r--   0 runner    (1001) docker     (127)     3881 2024-05-14 08:04:44.000000 sdist/kuzu-source/README.md
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/scripts/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/scripts/antlr4/
+-rw-rw-r--   0 runner    (1001) docker     (127)    26331 2024-05-14 08:04:44.000000 sdist/kuzu-source/scripts/antlr4/Cypher.g4.copy
+-rw-rw-r--   0 runner    (1001) docker     (127)     2085 2024-05-14 08:04:44.000000 sdist/kuzu-source/scripts/antlr4/generate_grammar.cmake
+-rwxrwxr-x   0 runner    (1001) docker     (127)      299 2024-05-14 08:04:44.000000 sdist/kuzu-source/scripts/check-include-guards.sh
+-rwxrwxr-x   0 runner    (1001) docker     (127)       76 2024-05-14 08:04:44.000000 sdist/kuzu-source/scripts/check-no-std-assert.sh
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2837 2024-05-14 08:04:44.000000 sdist/kuzu-source/scripts/collect-single-file-header.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/scripts/generate-cpp-docs/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/scripts/generate-cpp-docs/c/
+-rw-rw-r--   0 runner    (1001) docker     (127)   126290 2024-05-14 08:04:44.000000 sdist/kuzu-source/scripts/generate-cpp-docs/c/Doxyfile
+-rw-rw-r--   0 runner    (1001) docker     (127)     4738 2024-05-14 08:04:44.000000 sdist/kuzu-source/scripts/generate-cpp-docs/collect_files.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/scripts/generate-cpp-docs/cpp/
+-rw-rw-r--   0 runner    (1001) docker     (127)   126295 2024-05-14 08:04:44.000000 sdist/kuzu-source/scripts/generate-cpp-docs/cpp/Doxyfile
+-rwxrwxr-x   0 runner    (1001) docker     (127)      225 2024-05-14 08:04:44.000000 sdist/kuzu-source/scripts/generate-cpp-docs/doxygen.sh
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6998 2024-05-14 08:04:44.000000 sdist/kuzu-source/scripts/get-clangd-diagnostics.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      131 2024-05-14 08:04:44.000000 sdist/kuzu-source/scripts/http-server.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/scripts/multiplatform-test-helper/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2130 2024-05-14 08:04:44.000000 sdist/kuzu-source/scripts/multiplatform-test-helper/collect-results.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1585 2024-05-14 08:04:44.000000 sdist/kuzu-source/scripts/multiplatform-test-helper/notify-discord.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/scripts/pip-package/
+-rw-rw-r--   0 runner    (1001) docker     (127)       37 2024-05-14 08:04:44.000000 sdist/kuzu-source/scripts/pip-package/MANIFEST.in
+-rw-rw-r--   0 runner    (1001) docker     (127)     3276 2024-05-14 08:04:44.000000 sdist/kuzu-source/scripts/pip-package/README.md
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3277 2024-05-14 08:04:44.000000 sdist/kuzu-source/scripts/pip-package/package_tar.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      200 2024-05-14 08:04:44.000000 sdist/kuzu-source/scripts/pip-package/setup.cfg
+-rw-rw-r--   0 runner    (1001) docker     (127)     4441 2024-05-14 08:04:44.000000 sdist/kuzu-source/scripts/pip-package/setup.py
+-rwxrwxr-x   0 runner    (1001) docker     (127)    12359 2024-05-14 08:04:44.000000 sdist/kuzu-source/scripts/run-clang-format.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     3060 2024-05-14 08:04:44.000000 sdist/kuzu-source/scripts/update-nightly-build-version.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2644 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/antlr4/
+-rw-rw-r--   0 runner    (1001) docker     (127)    26331 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/antlr4/Cypher.g4
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/
+-rw-rw-r--   0 runner    (1001) docker     (127)      519 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind/
+-rw-rw-r--   0 runner    (1001) docker     (127)      766 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      441 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind/bind_attach_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      740 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind/bind_comment_on.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1323 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind/bind_create_macro.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    18633 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind/bind_ddl.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      437 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind/bind_detach_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      518 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind/bind_explain.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6114 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind/bind_export_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2074 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind/bind_extension.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5297 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind/bind_file_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    32965 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind/bind_graph_pattern.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3512 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind/bind_import_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11898 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind/bind_projection_clause.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4787 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind/bind_query.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      702 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind/bind_reading_clause.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1515 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind/bind_standalone_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      566 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind/bind_transaction.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    17249 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind/bind_updating_clause.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      415 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind/bind_use_database.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind/copy/
+-rw-rw-r--   0 runner    (1001) docker     (127)      246 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind/copy/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    10625 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind/copy/bind_copy_from.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8100 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind/copy/bind_copy_rdf_graph.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1613 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind/copy/bind_copy_to.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind/ddl/
+-rw-rw-r--   0 runner    (1001) docker     (127)      194 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind/ddl/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     3534 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind/ddl/bind_create_rdf_graph.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind/read/
+-rw-rw-r--   0 runner    (1001) docker     (127)      267 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind/read/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     3209 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind/read/bind_in_query_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5724 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind/read/bind_load_from.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3009 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind/read/bind_match.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2013 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind/read/bind_unwind.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind_expression/
+-rw-rw-r--   0 runner    (1001) docker     (127)      555 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind_expression/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2202 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind_expression/bind_boolean_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3488 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind_expression/bind_case_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3118 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind_expression/bind_comparison_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    14939 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind_expression/bind_function_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1284 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind_expression/bind_literal_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1677 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind_expression/bind_null_operator_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      928 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind_expression/bind_parameter_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5159 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind_expression/bind_property_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3195 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind_expression/bind_subquery_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1531 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bind_expression/bind_variable_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8045 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/binder.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/binder_scope.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      567 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bound_statement_result.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      801 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bound_statement_rewriter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5524 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/bound_statement_visitor.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/expression/
+-rw-rw-r--   0 runner    (1001) docker     (127)      380 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/expression/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      498 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/expression/case_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      764 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/expression/expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11104 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/expression/expression_util.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1438 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/expression/function_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      672 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/expression/literal_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      575 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/expression/parameter_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      549 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/expression/variable_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5234 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/expression_binder.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6353 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/expression_visitor.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/query/
+-rw-rw-r--   0 runner    (1001) docker     (127)      350 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/query/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      707 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/query/bound_delete_clause.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      707 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/query/bound_insert_clause.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1963 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/query/bound_merge_clause.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      718 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/query/bound_set_clause.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9670 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/query/query_graph.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6621 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/query/query_graph_label_analyzer.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/rewriter/
+-rw-rw-r--   0 runner    (1001) docker     (127)      261 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/rewriter/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      742 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/rewriter/match_clause_pattern_label_rewriter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2547 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/rewriter/with_clause_projection_rewriter.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/visitor/
+-rw-rw-r--   0 runner    (1001) docker     (127)      230 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/visitor/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      638 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/visitor/default_type_solver.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4801 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/binder/visitor/property_collector.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/c_api/
+-rw-rw-r--   0 runner    (1001) docker     (127)      369 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/c_api/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     4034 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/c_api/connection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2653 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/c_api/data_type.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1122 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/c_api/database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1412 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/c_api/flat_tuple.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      286 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/c_api/helpers.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7617 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/c_api/prepared_statement.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4402 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/c_api/query_result.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      745 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/c_api/query_summary.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    19821 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/c_api/value.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      271 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/c_api/version.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/catalog/
+-rw-rw-r--   0 runner    (1001) docker     (127)      242 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/catalog/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    19856 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/catalog/catalog.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/catalog/catalog_entry/
+-rw-rw-r--   0 runner    (1001) docker     (127)      464 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/catalog/catalog_entry/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1366 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/catalog/catalog_entry/catalog_entry.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/catalog/catalog_entry/catalog_entry_type.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      357 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/catalog/catalog_entry/function_catalog_entry.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2516 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/catalog/catalog_entry/node_table_catalog_entry.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5183 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/catalog/catalog_entry/rdf_graph_catalog_entry.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3770 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/catalog/catalog_entry/rel_group_catalog_entry.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4535 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/catalog/catalog_entry/rel_table_catalog_entry.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1063 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/catalog/catalog_entry/scalar_macro_catalog_entry.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6589 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/catalog/catalog_entry/table_catalog_entry.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8047 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/catalog/catalog_set.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1605 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/catalog/property.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/
+-rw-rw-r--   0 runner    (1001) docker     (127)      803 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/arrow/
+-rw-rw-r--   0 runner    (1001) docker     (127)      295 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/arrow/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    24685 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/arrow/arrow_array_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    10576 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/arrow/arrow_converter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8673 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/arrow/arrow_null_mask_tree.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    35459 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/arrow/arrow_row_batch.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5340 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/arrow/arrow_type.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      478 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/case_insensitive_map.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      106 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/constants.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/copier_config/
+-rw-rw-r--   0 runner    (1001) docker     (127)      256 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/copier_config/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     3078 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/copier_config/csv_reader_config.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/copier_config/rdf_reader_config.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1727 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/copier_config/reader_config.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/data_chunk/
+-rw-rw-r--   0 runner    (1001) docker     (127)      250 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/data_chunk/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      470 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/data_chunk/data_chunk.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2669 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/data_chunk/data_chunk_collection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    12601 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/data_chunk/data_chunk_state.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/enums/
+-rw-rw-r--   0 runner    (1001) docker     (127)      258 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/enums/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1050 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/enums/path_semantic.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      413 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/enums/rel_direction.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1069 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/enums/rel_multiplicity.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      642 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/enums/table_type.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/exception/
+-rw-rw-r--   0 runner    (1001) docker     (127)      316 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/exception/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      377 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/exception/exception.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2665 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/exception/message.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3201 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/expression_type.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/file_system/
+-rw-rw-r--   0 runner    (1001) docker     (127)      306 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/file_system/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      999 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/file_system/file_info.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1255 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/file_system/file_system.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    15054 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/file_system/local_file_system.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2708 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/file_system/virtual_file_system.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      977 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/in_mem_overflow_buffer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/keyword_utils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8157 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/md5.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      995 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/metric.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8989 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/null_mask.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1452 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/profiler.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      349 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/random_engine.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/serializer/
+-rw-rw-r--   0 runner    (1001) docker     (127)      270 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/serializer/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2842 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/serializer/buffered_file.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      948 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/serializer/buffered_serializer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      347 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/serializer/deserializer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      356 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/serializer/serializer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1355 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/sha256.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/signal/
+-rw-rw-r--   0 runner    (1001) docker     (127)      182 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/signal/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1027 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/signal/register.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5079 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/string_utils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      884 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/system_message.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/task_system/
+-rw-rw-r--   0 runner    (1001) docker     (127)      236 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/task_system/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2748 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/task_system/progress_bar.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      772 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/task_system/task.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4596 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/task_system/task_scheduler.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9750 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/type_utils.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/types/
+-rw-rw-r--   0 runner    (1001) docker     (127)      406 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/types/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     4494 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/types/blob.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    19741 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/types/date_t.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6196 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/types/dtime_t.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    19061 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/types/int128_t.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1174 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/types/internal_id_t.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    17620 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/types/interval_t.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      832 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/types/ku_list.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2364 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/types/ku_string.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11000 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/types/timestamp_t.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    58160 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/types/types.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4363 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/types/uuid.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/types/value/
+-rw-rw-r--   0 runner    (1001) docker     (127)      286 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/types/value/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      512 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/types/value/nested.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2379 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/types/value/node.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      354 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/types/value/rdf_variant.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      840 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/types/value/recursive_rel.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2759 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/types/value/rel.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    35482 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/types/value/value.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1298 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/utils.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/vector/
+-rw-rw-r--   0 runner    (1001) docker     (127)      210 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/vector/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     3332 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/vector/auxiliary_buffer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    28656 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/vector/value_vector.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1261 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/common/windows_utils.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/expression_evaluator/
+-rw-rw-r--   0 runner    (1001) docker     (127)      420 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/expression_evaluator/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     4528 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/expression_evaluator/case_evaluator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      965 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/expression_evaluator/expression_evaluator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      849 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/expression_evaluator/expression_evaluator_utils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3322 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/expression_evaluator/function_evaluator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1063 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/expression_evaluator/literal_evaluator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1545 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/expression_evaluator/node_rel_evaluator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9731 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/expression_evaluator/path_evaluator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1280 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/expression_evaluator/reference_evaluator.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/extension/
+-rw-rw-r--   0 runner    (1001) docker     (127)      200 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/extension/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      239 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/extension/catalog_extension.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3182 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/extension/extension.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1240 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/aggregate/
+-rw-rw-r--   0 runner    (1001) docker     (127)      227 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/aggregate/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     3878 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/aggregate/collect.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1835 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/aggregate/count.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1044 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/aggregate/count_star.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    12187 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/aggregate_function.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/arithmetic/
+-rw-rw-r--   0 runner    (1001) docker     (127)      299 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/arithmetic/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2611 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/arithmetic/abs.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5505 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/arithmetic/add.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5953 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/arithmetic/divide.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4379 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/arithmetic/modulo.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8121 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/arithmetic/multiply.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2427 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/arithmetic/negate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5848 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/arithmetic/subtract.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/array/
+-rw-rw-r--   0 runner    (1001) docker     (127)      210 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/array/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     7204 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/array/array_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1328 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/array/array_value.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2494 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/base_lower_upper_operation.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    20338 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/built_in_function_utils.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/cast/
+-rw-rw-r--   0 runner    (1001) docker     (127)      208 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/cast/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     5428 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/cast/cast_array.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11953 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/cast/cast_rdf_variant.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    33750 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/cast_from_string_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2442 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/cast_string_non_nested_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8637 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/comparison_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5169 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/find_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      517 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    12742 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/function_collection.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/list/
+-rw-rw-r--   0 runner    (1001) docker     (127)      711 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/list/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2745 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/list/list_agg_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1855 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/list/list_any_value_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2618 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/list/list_append_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2166 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/list/list_concat_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1580 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/list/list_contains_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2146 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/list/list_creation.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1882 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/list/list_distinct_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2189 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/list/list_extract_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1184 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/list/list_position_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2488 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/list/list_prepend_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3640 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/list/list_range_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1561 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/list/list_reverse_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3355 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/list/list_slice_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3684 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/list/list_sort_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1898 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/list/list_to_string_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2240 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/list/list_unique_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1904 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/list/size_function.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/map/
+-rw-rw-r--   0 runner    (1001) docker     (127)      283 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/map/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1091 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/map/map_creation_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1670 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/map/map_extract_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      961 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/map/map_keys_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      953 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/map/map_values_function.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/path/
+-rw-rw-r--   0 runner    (1001) docker     (127)      299 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/path/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2255 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/path/length_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1144 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/path/nodes_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3841 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/path/properties_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1164 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/path/rels_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1997 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/path/semantic_function.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/pattern/
+-rw-rw-r--   0 runner    (1001) docker     (127)      186 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/pattern/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1775 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/pattern/id_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2683 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/scalar_macro_function.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/struct/
+-rw-rw-r--   0 runner    (1001) docker     (127)      229 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/struct/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2617 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/struct/struct_extract_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3356 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/struct/struct_pack_function.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/table/
+-rw-rw-r--   0 runner    (1001) docker     (127)      218 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/table/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/table/call/
+-rw-rw-r--   0 runner    (1001) docker     (127)      360 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/table/call/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1542 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/table/call/checkpoint.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2232 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/table/call/current_setting.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1376 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/table/call/db_version.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2672 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/table/call/show_attached_databases.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5816 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/table/call/show_connection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4202 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/table/call/show_tables.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11070 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/table/call/storage_info.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5471 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/table/call/table_info.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1139 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/table/call_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      364 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/table/scan_functions.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/union/
+-rw-rw-r--   0 runner    (1001) docker     (127)      257 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/union/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      628 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/union/union_extract_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      817 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/union/union_tag_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1873 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/union/union_value_function.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/utility/
+-rw-rw-r--   0 runner    (1001) docker     (127)      324 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/utility/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     3471 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/utility/coalesce.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3205 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/utility/constant_or_null.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1277 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/utility/count_if.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      870 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/utility/error.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      892 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/utility/md5.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1455 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/utility/nullif.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      950 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/utility/sha256.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1576 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/utility/typeof.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    18396 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/vector_arithmetic_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1389 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/vector_blob_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4267 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/vector_boolean_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    47661 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/vector_cast_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4887 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/vector_date_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9214 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/vector_hash_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      888 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/vector_node_rel_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1516 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/vector_null_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      913 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/vector_rdf_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    14505 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/vector_string_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1205 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/vector_timestamp_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      552 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/function/vector_uuid_functions.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/
+-rw-rw-r--   0 runner    (1001) docker     (127)    12753 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/binder.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2756 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/binder_scope.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      605 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/bound_attach_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      862 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/bound_comment_on.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      842 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/bound_create_macro.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      514 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/bound_database_statement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      365 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/bound_detach_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      891 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/bound_explain.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1874 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/bound_export_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      713 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/bound_extension_statement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      877 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/bound_import_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2466 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/bound_scan_source.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      790 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/bound_standalone_call.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      856 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/bound_statement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1001 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/bound_statement_result.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      348 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/bound_statement_rewriter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2666 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/bound_statement_visitor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      661 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/bound_transaction_statement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      356 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/bound_use_database.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/copy/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3164 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/copy/bound_copy_from.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1071 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/copy/bound_copy_to.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      813 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/copy/bound_file_scan_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1014 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/copy/index_look_up_info.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/ddl/
+-rw-rw-r--   0 runner    (1001) docker     (127)      530 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/ddl/bound_alter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3438 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/ddl/bound_alter_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      574 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/ddl/bound_create_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5837 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/ddl/bound_create_table_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      664 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/ddl/bound_drop_table.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/expression/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1468 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/expression/case_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4768 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/expression/expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2418 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/expression/expression_util.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4539 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/expression/function_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      832 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/expression/literal_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      786 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/expression/node_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4286 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/expression/node_rel_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      918 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/expression/parameter_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1129 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/expression/path_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2561 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/expression/property_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4586 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/expression/rel_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2112 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/expression/subquery_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      833 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/expression/variable_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5949 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/expression_binder.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2678 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/expression_visitor.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/query/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1069 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/query/bound_regular_query.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2487 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/query/normalized_query_part.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1013 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/query/normalized_single_query.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6508 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/query/query_graph.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      572 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/query/query_graph_label_analyzer.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1225 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_in_query_call.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      482 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_load_from.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      813 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_match_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1010 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_reading_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      869 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_unwind_clause.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/query/return_with_clause/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3072 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/query/return_with_clause/bound_projection_body.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      923 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/query/return_with_clause/bound_return_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      687 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/query/return_with_clause/bound_with_clause.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1445 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_delete_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      871 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_delete_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1470 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_insert_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1520 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_insert_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5606 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_merge_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1570 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_set_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      797 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_set_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      424 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_updating_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      163 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/update_table_type.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/rewriter/
+-rw-rw-r--   0 runner    (1001) docker     (127)      515 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/rewriter/match_clause_pattern_label_rewriter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      693 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/rewriter/with_clause_projection_rewriter.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/visitor/
+-rw-rw-r--   0 runner    (1001) docker     (127)      781 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/visitor/default_type_solver.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1211 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/binder/visitor/property_collector.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/c_api/
+-rw-rw-r--   0 runner    (1001) docker     (127)       86 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/c_api/helpers.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    50669 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/c_api/kuzu.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/catalog/
+-rw-rw-r--   0 runner    (1001) docker     (127)     6432 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/catalog/catalog.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3000 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/catalog_entry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      575 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/catalog_entry_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      575 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/dummy_catalog_entry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1286 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/function_catalog_entry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2690 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/node_table_catalog_entry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2482 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/rdf_graph_catalog_entry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1720 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/rel_group_catalog_entry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2482 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/rel_table_catalog_entry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1392 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/scalar_macro_catalog_entry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3749 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/table_catalog_entry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2385 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/catalog/catalog_set.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1894 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/catalog/property.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/
+-rw-rw-r--   0 runner    (1001) docker     (127)      975 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/api.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/arrow/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1542 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/arrow/arrow.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1943 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/arrow/arrow_buffer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1862 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/arrow/arrow_converter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1449 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/arrow/arrow_nullmask_tree.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2921 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/arrow/arrow_row_batch.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1245 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/assert.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      578 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/case_insensitive_map.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      559 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/cast.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      178 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/column_data_format.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4183 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/concurrent_vector.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9441 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/constants.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/copier_config/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1633 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/copier_config/csv_reader_config.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      468 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/copier_config/rdf_reader_config.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1302 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/copier_config/reader_config.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3648 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/copy_constructors.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/data_chunk/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1576 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/data_chunk/data_chunk.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1261 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/data_chunk/data_chunk_collection.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2116 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/data_chunk/data_chunk_state.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2155 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/data_chunk/sel_vector.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/enums/
+-rw-rw-r--   0 runner    (1001) docker     (127)      246 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/enums/alter_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      575 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/enums/clause_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      194 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/enums/conflict_action.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      194 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/enums/delete_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      192 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/enums/explain_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1203 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/enums/expression_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      285 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/enums/join_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      364 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/enums/path_semantic.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      402 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/enums/query_rel_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      300 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/enums/rel_direction.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      359 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/enums/rel_multiplicity.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      195 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/enums/scan_source_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      521 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/enums/statement_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      164 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/enums/subquery_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      431 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/enums/table_type.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/exception/
+-rw-rw-r--   0 runner    (1001) docker     (127)      302 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/exception/binder.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      332 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/exception/buffer_manager.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      305 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/exception/catalog.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      287 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/exception/connection.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      321 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/exception/conversion.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      296 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/exception/copy.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      403 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/exception/exception.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      294 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/exception/extension.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      283 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/exception/internal.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      274 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/exception/interrupt.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      265 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/exception/io.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1260 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/exception/message.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      295 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/exception/not_implemented.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      307 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/exception/overflow.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      365 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/exception/parser.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      305 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/exception/runtime.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      305 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/exception/storage.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      263 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/exception/test.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      303 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/exception/transaction_manager.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/file_system/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1066 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/file_system/file_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2358 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/file_system/file_system.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2019 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/file_system/local_file_system.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1796 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/file_system/virtual_file_system.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1863 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/in_mem_overflow_buffer.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/keyword/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1576 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/keyword/rdf_keyword.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3271 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/md5.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      745 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/metric.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3921 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/mpsc_queue.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1346 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/mutex.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1155 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/null_buffer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9142 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/null_mask.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      702 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/profiler.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      349 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/random_engine.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/serializer/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1366 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/serializer/buffered_file.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1716 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/serializer/buffered_serializer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2495 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/serializer/deserializer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      264 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/serializer/reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2467 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/serializer/serializer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      237 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/serializer/writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      557 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/sha256.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2229 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/static_vector.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3858 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/string_format.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4653 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/string_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      596 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/system_message.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/task_system/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1469 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/task_system/progress_bar.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3420 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/task_system/task.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3059 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/task_system/task_scheduler.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1205 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/timer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    11129 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/type_utils.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/types/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1666 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/types/blob.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    10927 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/types/cast_helpers.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4563 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/types/date_t.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2446 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/types/dtime_t.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6090 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/types/int128_t.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1167 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/types/internal_id_t.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4658 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/types/interval_t.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/types/ku_list.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2887 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/types/ku_string.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4667 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/types/timestamp_t.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    19500 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/types/types.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      940 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/types/uuid.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/types/value/
+-rw-rw-r--   0 runner    (1001) docker     (127)      319 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/types/value/nested.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1670 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/types/value/node.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1145 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/types/value/rdf_variant.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      635 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/types/value/recursive_rel.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1968 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/types/value/rel.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    21563 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/types/value/value.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      782 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/utils.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/vector/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3218 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/vector/auxiliary_buffer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    13651 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/vector/value_vector.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      298 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/common/windows_utils.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/expression_evaluator/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2419 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/expression_evaluator/case_evaluator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1382 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/expression_evaluator/expression_evaluator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      433 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/expression_evaluator/expression_evaluator_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1267 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/expression_evaluator/function_evaluator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      871 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/expression_evaluator/literal_evaluator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1399 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/expression_evaluator/node_rel_evaluator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2884 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/expression_evaluator/path_evaluator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1082 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/expression_evaluator/reference_evaluator.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/extension/
+-rw-rw-r--   0 runner    (1001) docker     (127)      288 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/extension/catalog_extension.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1491 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/extension/extension.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      193 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/extension/extension_action.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/aggregate/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3518 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/aggregate/avg.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1139 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/aggregate/base_count.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2409 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/aggregate/collect.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      821 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/aggregate/count.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/aggregate/count_star.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4091 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/aggregate/min_max.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2903 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/aggregate/sum.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6996 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/aggregate_function.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/arithmetic/
+-rw-rw-r--   0 runner    (1001) docker     (127)      740 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/arithmetic/abs.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      930 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/arithmetic/add.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5133 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/arithmetic/arithmetic_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      957 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/arithmetic/divide.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1109 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/arithmetic/modulo.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      975 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/arithmetic/multiply.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      520 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/arithmetic/negate.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      975 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/arithmetic/subtract.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4696 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/arithmetic/vector_arithmetic_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/array/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/array/functions/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1096 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/array/functions/array_cosine_similarity.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1078 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/array/functions/array_cross_product.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      824 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/array/functions/array_distance.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/array/functions/array_inner_product.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2034 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/array/vector_array_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    24872 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/binary_function_executor.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/blob/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/blob/functions/
+-rw-rw-r--   0 runner    (1001) docker     (127)      828 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/blob/functions/decode_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      402 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/blob/functions/encode_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      269 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/blob/functions/octet_length_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      506 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/blob/vector_blob_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/boolean/
+-rw-rw-r--   0 runner    (1001) docker     (127)    15040 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/boolean/boolean_function_executor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4678 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/boolean/boolean_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2493 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/boolean/vector_boolean_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3911 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/built_in_function_utils.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/cast/
+-rw-rw-r--   0 runner    (1001) docker     (127)      674 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/cast/cast_function_bind_data.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/cast/functions/
+-rw-rw-r--   0 runner    (1001) docker     (127)      539 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_array.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7564 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_from_string_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    13672 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      993 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_rdf_variant.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7994 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_string_non_nested_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5149 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/cast/functions/numeric_cast.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1795 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/cast/functions/numeric_limits.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3693 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/cast/vector_cast_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/comparison/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2928 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/comparison/comparison_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    10062 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/comparison/vector_comparison_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      509 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/const_function_executor.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/date/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4625 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/date/date_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1236 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/date/vector_date_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2897 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      455 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/function_collection.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/hash/
+-rw-rw-r--   0 runner    (1001) docker     (127)     6081 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/hash/hash_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      945 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/hash/vector_hash_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/interval/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1758 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/interval/interval_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2341 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/interval/vector_interval_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/list/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/list/functions/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3521 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/list/functions/base_list_sort_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/list/functions/list_concat_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1987 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/list/functions/list_extract_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1051 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/list/functions/list_len_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1206 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/list/functions/list_position_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1309 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/list/functions/list_reverse_sort_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1312 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/list/functions/list_sort_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      436 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/list/functions/list_to_string_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1231 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/list/functions/list_unique_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3221 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/list/vector_list_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/map/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/map/functions/
+-rw-rw-r--   0 runner    (1001) docker     (127)      872 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/map/functions/base_map_extract_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2268 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/map/functions/map_creation_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1515 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/map/functions/map_extract_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      658 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/map/functions/map_keys_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      712 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/map/functions/map_values_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/map/vector_map_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/null/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2749 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/null/null_function_executor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/null/null_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1154 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/null/vector_null_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/path/
+-rw-rw-r--   0 runner    (1001) docker     (127)     6247 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/path/path_function_executor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1133 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/path/vector_path_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      789 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/pointer_function_executor.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/rdf/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1299 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/rdf/rdf_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      393 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/rdf/vector_rdf_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      982 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/rewrite_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    10274 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/scalar_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1403 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/scalar_macro_function.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/schema/
+-rw-rw-r--   0 runner    (1001) docker     (127)      649 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/schema/label_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      258 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/schema/offset_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      642 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/schema/vector_label_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      529 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/schema/vector_node_rel_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/string/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/string/functions/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2242 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/string/functions/array_extract_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      669 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/string/functions/base_lower_upper_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2303 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/string/functions/base_pad_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      809 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/string/functions/base_regexp_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      429 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/string/functions/base_str_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/string/functions/contains_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      450 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/string/functions/ends_with_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1459 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/string/functions/find_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      575 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/string/functions/initcap_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      656 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/string/functions/left_operation.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1738 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/string/functions/levenshtein_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      444 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/string/functions/lower_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1035 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/string/functions/lpad_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      765 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/string/functions/ltrim_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      874 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/string/functions/pad_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3067 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_extract_all_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1778 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_extract_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      476 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_full_match_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      477 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_matches_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      710 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_replace_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      640 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/string/functions/repeat_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      570 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/string/functions/reverse_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      673 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/string/functions/right_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1035 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/string/functions/rpad_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      664 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/string/functions/rtrim_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      401 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/string/functions/starts_with_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2808 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/string/functions/substr_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      587 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/string/functions/trim_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      509 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/string/functions/upper_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5537 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/string/vector_string_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/struct/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1383 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/struct/vector_struct_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/table/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1702 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/table/bind_data.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1905 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/table/bind_input.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3069 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/table/call_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1322 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/table/scan_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      527 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/table/scan_replacement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4127 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/table_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    21690 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/ternary_function_executor.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/timestamp/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1036 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/timestamp/timestamp_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      508 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/timestamp/vector_timestamp_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    10907 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/udf_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7851 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/unary_function_executor.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/union/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/union/functions/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1234 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/union/functions/union_tag.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      519 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/union/vector_union_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/utility/
+-rw-rw-r--   0 runner    (1001) docker     (127)      348 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/utility/function_string_bind_data.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      999 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/utility/vector_utility_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/uuid/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/uuid/functions/
+-rw-rw-r--   0 runner    (1001) docker     (127)      438 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/uuid/functions/gen_random_uuid.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      266 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/function/uuid/vector_uuid_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/main/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1290 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/main/attached_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1450 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/main/client_config.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6973 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/main/client_context.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7803 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/main/connection.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5111 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/main/database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      812 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/main/database_manager.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1851 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/main/db_config.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1394 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/main/kuzu.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1130 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/main/kuzu_fwd.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3470 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/main/plan_printer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1682 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/main/prepared_statement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4968 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/main/query_result.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1015 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/main/query_summary.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6918 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/main/settings.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      839 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/main/storage_driver.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      528 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/main/version.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/optimizer/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2295 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/optimizer/acc_hash_join_optimizer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      821 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/optimizer/agg_key_dependency_optimizer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      895 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/optimizer/correlated_subquery_unnest_solver.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2050 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/optimizer/factorization_rewriter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3621 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/optimizer/filter_push_down_optimizer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1376 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/optimizer/logical_operator_collector.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6889 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/optimizer/logical_operator_visitor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      298 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/optimizer/optimizer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2461 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/optimizer/projection_push_down_optimizer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      572 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/optimizer/remove_factorization_rewriter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      940 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/optimizer/remove_unnecessary_join_optimizer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      556 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/optimizer/top_k_optimizer.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/antlr_parser/
+-rw-rw-r--   0 runner    (1001) docker     (127)      895 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/antlr_parser/kuzu_cypher_parser.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      620 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/antlr_parser/parser_error_listener.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      373 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/antlr_parser/parser_error_strategy.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      468 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/attach_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      541 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/comment_on.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1793 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/copy.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1237 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/create_macro.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/database_statement.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/ddl/
+-rw-rw-r--   0 runner    (1001) docker     (127)      397 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/ddl/alter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1748 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/ddl/alter_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      447 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/ddl/create_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1782 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/ddl/create_table_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/ddl/drop.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      358 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/detach_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      748 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/explain_statement.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/expression/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3933 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/expression/parsed_case_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3180 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/expression/parsed_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2663 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/expression/parsed_function_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1495 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/expression/parsed_literal_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      858 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/expression/parsed_parameter_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1688 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/expression/parsed_property_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/expression/parsed_subquery_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1546 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/expression/parsed_variable_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      626 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/extension_statement.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/parsed_data/
+-rw-rw-r--   0 runner    (1001) docker     (127)      177 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/parsed_data/attach_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1163 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/parsed_expression_visitor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2613 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/parsed_statement_visitor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      292 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/parser.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      975 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/port_db.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/query/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/
+-rw-rw-r--   0 runner    (1001) docker     (127)      946 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/node_pattern.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1100 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/pattern_element.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      587 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/pattern_element_chain.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1599 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/rel_pattern.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1309 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/query/query_part.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/
+-rw-rw-r--   0 runner    (1001) docker     (127)      982 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/in_query_call_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1521 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/load_from.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1212 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/match_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      587 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/reading_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      657 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/unwind_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      928 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/query/regular_query.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/query/return_with_clause/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2155 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/query/return_with_clause/projection_body.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      485 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/query/return_with_clause/return_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/query/return_with_clause/with_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1798 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/query/single_query.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/
+-rw-rw-r--   0 runner    (1001) docker     (127)      898 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/delete_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      601 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/insert_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1341 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/merge_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      538 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/set_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/updating_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1543 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/scan_source.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      712 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/standalone_call.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      945 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/statement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      568 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/transaction_statement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    12939 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/transformer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      330 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/use_database.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/visitor/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1163 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/parser/visitor/statement_read_write_analyzer.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/join_order/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2656 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/join_order/cardinality_estimator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      801 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/join_order/cost_model.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      469 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/join_order/join_order_util.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2304 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/join_order_enumerator_context.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/ddl/
+-rw-rw-r--   0 runner    (1001) docker     (127)      754 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/ddl/logical_alter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      841 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/ddl/logical_create_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      920 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/ddl/logical_ddl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      795 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/ddl/logical_drop_table.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/extend/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1426 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/extend/base_logical_extend.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1107 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/extend/extend_direction.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1278 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/extend/logical_extend.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4582 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/extend/logical_recursive_extend.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      200 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/extend/recursive_join_type.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/factorization/
+-rw-rw-r--   0 runner    (1001) docker     (127)      442 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/factorization/flatten_resolver.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      950 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/factorization/sink_util.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2011 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/logical_accumulate.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2430 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/logical_aggregate.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1376 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/logical_comment_on.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1381 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/logical_create_macro.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1079 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/logical_cross_product.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1632 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/logical_distinct.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      784 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/logical_empty_result.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1603 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/logical_explain.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1117 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/logical_filter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      804 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/logical_flatten.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3562 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/logical_hash_join.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/logical_in_query_call.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1843 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/logical_intersect.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1297 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/logical_limit.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1147 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/logical_mark_accmulate.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      769 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/logical_multiplcity_reducer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1224 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/logical_node_label_filter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3462 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/logical_operator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1616 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/logical_order_by.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2156 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/logical_partitioner.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1176 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/logical_plan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1179 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/logical_plan_util.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1117 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/logical_projection.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1094 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/logical_standalone_call.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      969 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/logical_transaction.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1199 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/logical_union.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1413 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/logical_unwind.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/persistent/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1473 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_copy_from.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1946 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_copy_to.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2791 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_delete.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2037 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_insert.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3728 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_merge.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2803 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_set.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/scan/
+-rw-rw-r--   0 runner    (1001) docker     (127)      643 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_dummy_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1290 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_expressions_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_index_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1217 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_scan_file.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1089 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_scan_internal_id.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1486 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_scan_node_property.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6044 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/schema.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/simple/
+-rw-rw-r--   0 runner    (1001) docker     (127)      858 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_attach_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      583 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      578 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_detach_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1383 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_export_db.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      915 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_extension.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      757 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_import_db.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      953 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_simple.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      552 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_use_database.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/sip/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1588 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/sip/logical_semi_masker.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      308 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/operator/sip/side_way_info_passing.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    16586 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/planner.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3416 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/planner/subplans_table.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1252 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/data_pos.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/execution_context.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2051 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/expression_mapper.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/
+-rw-rw-r--   0 runner    (1001) docker     (127)    11095 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/aggregate_hash_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1255 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/aggregate_input.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1824 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/base_aggregate.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1374 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/base_aggregate_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3664 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/hash_aggregate.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1905 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/hash_aggregate_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2811 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/simple_aggregate.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1565 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/simple_aggregate_scan.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/call/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2956 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/call/in_query_call.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1361 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/call/standalone_call.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1712 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/comment_on.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2858 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/cross_product.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/ddl/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1402 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/ddl/alter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      779 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/ddl/create_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      945 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/ddl/ddl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      777 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/ddl/drop_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      583 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/empty_result.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2713 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/filter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      820 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/filtering_operator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1242 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/flatten.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/hash_join/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4405 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/hash_join/hash_join_build.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4687 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/hash_join/hash_join_probe.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3282 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/hash_join/join_hash_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2359 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/index_lookup.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1541 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/index_scan.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/intersect/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3204 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/intersect/intersect.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1057 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/intersect/intersect_build.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1208 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/limit.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/macro/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1852 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/macro/create_macro.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5181 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/mask.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      972 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/multiplicity_reducer.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/order_by/
+-rw-rw-r--   0 runner    (1001) docker     (127)     7982 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/order_by/key_block_merger.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1868 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1714 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by_data_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6358 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by_key_encoder.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2060 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by_merge.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2533 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3873 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/order_by/radix_sort.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2942 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/order_by/sort_state.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6218 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/order_by/top_k.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1694 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/order_by/top_k_scanner.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5655 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/partitioner.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2787 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/batch_insert.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      983 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/copy_rdf.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2426 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/copy_to.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3239 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/copy_to_csv.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2850 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/copy_to_parquet.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1604 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/delete.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6124 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/delete_executor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1005 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/export_db.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      840 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/file_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      734 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/import_db.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5440 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/index_builder.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1163 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/insert.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3808 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/insert_executor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2702 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/merge.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5761 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/node_batch_insert.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2367 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/base_csv_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1831 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/driver.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1862 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/parallel_csv_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1888 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/serial_csv_reader.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/npy/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1754 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/npy/npy_reader.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1481 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/boolean_column_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1616 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/callback_column_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5214 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/column_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1962 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/decode_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1359 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/interval_column_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1842 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/list_column_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4105 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/parquet_dbp_decoder.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4637 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/parquet_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4238 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/parquet_rle_bp_decoder.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      976 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/parquet_timestamp.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1881 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/resizable_buffer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1327 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/string_column_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1262 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/struct_column_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3427 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/templated_column_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6782 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/thrift_tools.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/
+-rw-rw-r--   0 runner    (1001) docker     (127)     5911 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/rdf_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7424 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/rdf_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      380 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/rdf_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2388 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/triple_store.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      865 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/reader_bind_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4368 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/rel_batch_insert.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1938 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/set.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6617 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/set_executor.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3914 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/basic_column_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2248 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/boolean_column_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4081 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/column_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1063 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/interval_column_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1729 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/list_column_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1087 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/parquet_rle_bp_encoder.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3229 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/parquet_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3898 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/standard_column_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5245 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/string_column_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1711 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/struct_column_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4998 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/physical_operator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1356 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/profile.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1518 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/projection.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2317 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/all_shortest_path_state.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3932 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/bfs_state.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1693 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/frontier.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6229 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/frontier_scanner.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4590 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/path_property_probe.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5296 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/recursive_join.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1380 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/scan_frontier.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1684 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/shortest_path_state.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1050 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/variable_length_state.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2873 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/result_collector.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/scan/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1067 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_multi_node_tables.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1913 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_multi_rel_tables.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2083 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_node_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2179 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_rel_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1085 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3474 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/scan_node_id.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5060 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/semi_masker.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/simple/
+-rw-rw-r--   0 runner    (1001) docker     (127)      813 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/simple/attach_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      463 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/simple/database_operator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      696 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/simple/detach_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      966 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/simple/export_db.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      690 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/simple/import_db.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      941 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/simple/install_extension.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      721 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/simple/load_extension.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1297 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/simple/simple.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      684 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/simple/use_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1777 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1435 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/skip.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/table_scan/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1102 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/table_scan/ftable_scan_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3006 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/table_scan/union_all_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1195 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/transaction.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1499 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/operator/unwind.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      388 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/physical_plan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    12321 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/plan_mapper.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      638 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/processor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      621 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/processor_task.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/result/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1737 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/result/base_hash_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    12804 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/result/factorized_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3030 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/result/factorized_table_schema.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1198 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/result/factorized_table_util.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1187 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/result/flat_tuple.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1044 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/result/mark_hash_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1519 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/result/result_set.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1063 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/processor/result/result_set_descriptor.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/buffer_manager/
+-rw-rw-r--   0 runner    (1001) docker     (127)    10155 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/buffer_manager/bm_file_handle.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    13079 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/buffer_manager/buffer_manager.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      527 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/buffer_manager/locked_queue.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2759 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/buffer_manager/memory_manager.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1714 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/buffer_manager/vm_region.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/compression/
+-rw-rw-r--   0 runner    (1001) docker     (127)    15859 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/compression/compression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1695 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/compression/sign_extend.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3328 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/file_handle.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/index/
+-rw-rw-r--   0 runner    (1001) docker     (127)    14384 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/index/hash_index.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1656 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/index/hash_index_header.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2243 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/index/hash_index_slot.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2560 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/index/hash_index_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7560 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/index/in_mem_hash_index.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/local_storage/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2514 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/local_storage/local_node_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3159 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/local_storage/local_rel_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1052 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/local_storage/local_storage.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9200 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/local_storage/local_table.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/stats/
+-rw-rw-r--   0 runner    (1001) docker     (127)      999 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/stats/metadata_dah_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3254 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/stats/node_table_statistics.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3125 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/stats/nodes_store_statistics.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1594 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/stats/property_statistics.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3873 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/stats/rel_table_statistics.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2721 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/stats/rels_store_statistics.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1947 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/stats/table_statistics.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4449 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/stats/table_statistics_collection.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      821 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/storage_extension.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3147 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/storage_manager.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/storage_structure/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2297 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/storage_structure/db_file_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    18677 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/storage_structure/disk_array.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      368 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/storage_structure/in_mem_page.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4969 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/storage_structure/overflow_file.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8115 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/storage_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      804 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/storage_version_info.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/store/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4852 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/store/chunked_node_group.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1626 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/store/chunked_node_group_collection.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    14266 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/store/column.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9626 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/store/column_chunk.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2508 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/store/dictionary_chunk.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3021 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/store/dictionary_column.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5856 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/store/list_column.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3467 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/store/list_column_chunk.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6212 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/store/node_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3448 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/store/node_table_data.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2528 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/store/null_column.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7138 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/store/rel_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    12842 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/store/rel_table_data.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3202 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/store/string_column.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2511 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/store/string_column_chunk.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2910 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/store/struct_column.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1968 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/store/struct_column_chunk.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3978 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/store/table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2638 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/store/table_data.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2397 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/undo_buffer.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/wal/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2377 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/wal/wal.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5999 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/wal/wal_record.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1888 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/wal_replayer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      725 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/storage/wal_replayer_utils.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/transaction/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2666 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/transaction/transaction.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      294 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/transaction/transaction_action.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2473 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/transaction/transaction_context.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3396 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/include/transaction/transaction_manager.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/main/
+-rw-rw-r--   0 runner    (1001) docker     (127)      444 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/main/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1638 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/main/attached_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    21823 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/main/client_context.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3262 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/main/connection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5810 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/main/database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2483 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/main/database_manager.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1572 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/main/db_config.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    13980 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/main/plan_printer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      810 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/main/prepared_statement.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4054 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/main/query_result.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      578 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/main/query_summary.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4339 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/main/storage_driver.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      317 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/main/version.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/optimizer/
+-rw-rw-r--   0 runner    (1001) docker     (127)      602 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/optimizer/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    10541 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/optimizer/acc_hash_join_optimizer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3540 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/optimizer/agg_key_dependency_optimizer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1488 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/optimizer/correlated_subquery_unnest_solver.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    10339 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/optimizer/factorization_rewriter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    12064 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/optimizer/filter_push_down_optimizer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      340 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/optimizer/logical_operator_collector.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5558 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/optimizer/logical_operator_visitor.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2087 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/optimizer/optimizer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    13109 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/optimizer/projection_push_down_optimizer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1201 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/optimizer/remove_factorization_rewriter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1537 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/optimizer/remove_unnecessary_join_optimizer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1902 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/optimizer/top_k_optimizer.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/
+-rw-rw-r--   0 runner    (1001) docker     (127)      400 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/antlr_parser/
+-rw-rw-r--   0 runner    (1001) docker     (127)      267 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/antlr_parser/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1595 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/antlr_parser/kuzu_cypher_parser.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1391 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/antlr_parser/parser_error_listener.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      827 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/antlr_parser/parser_error_strategy.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      455 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/create_macro.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/expression/
+-rw-rw-r--   0 runner    (1001) docker     (127)      346 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/expression/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2127 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/expression/parsed_case_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3281 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/expression/parsed_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      785 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/expression/parsed_function_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      491 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/expression/parsed_property_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      491 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/expression/parsed_variable_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3506 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/parsed_expression_visitor.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4399 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/parsed_statement_visitor.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1641 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/parser.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/transform/
+-rw-rw-r--   0 runner    (1001) docker     (127)      726 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/transform/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      646 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/transform/transform_attach_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      450 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/transform/transform_comment_on.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3602 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/transform/transform_copy.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7632 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/transform/transform_ddl.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      392 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/transform/transform_detach_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    27904 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/transform/transform_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      858 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/transform/transform_extension.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7789 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/transform/transform_graph_pattern.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1272 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/transform/transform_macro.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      833 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/transform/transform_port_db.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2587 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/transform/transform_projection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2253 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/transform/transform_query.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2715 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/transform/transform_reading_clause.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      490 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/transform/transform_standalone_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1209 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/transform/transform_transaction.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2681 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/transform/transform_updating_clause.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      380 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/transform/transform_use_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4493 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/transformer.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/visitor/
+-rw-rw-r--   0 runner    (1001) docker     (127)      209 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/visitor/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      258 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/parser/visitor/statement_read_write_analyzer.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/
+-rw-rw-r--   0 runner    (1001) docker     (127)      339 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/join_order/
+-rw-rw-r--   0 runner    (1001) docker     (127)      251 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/join_order/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     5776 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/join_order/cardinality_estimator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1652 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/join_order/cost_model.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      745 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/join_order/join_order_util.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1233 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/join_order_enumerator_context.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1025 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/ddl/
+-rw-rw-r--   0 runner    (1001) docker     (127)      175 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/ddl/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/ddl/logical_ddl.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/extend/
+-rw-rw-r--   0 runner    (1001) docker     (127)      253 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/extend/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1348 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/extend/base_logical_extend.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1205 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/extend/logical_extend.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2914 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/extend/logical_recursive_extend.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/factorization/
+-rw-rw-r--   0 runner    (1001) docker     (127)      223 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/factorization/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1007 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/factorization/flatten_resolver.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2591 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/factorization/sink_util.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1552 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/logical_accumulate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2870 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/logical_aggregate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      517 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/logical_comment_on.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      523 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/logical_create_macro.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      829 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/logical_cross_product.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1523 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/logical_distinct.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      678 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/logical_dummy_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      800 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/logical_explain.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      822 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/logical_filter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      407 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/logical_flatten.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7224 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/logical_hash_join.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      726 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/logical_in_query_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2606 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/logical_intersect.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1039 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/logical_limit.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1514 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/logical_mark_accumulate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6394 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/logical_operator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2805 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/logical_order_by.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      939 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/logical_partitioner.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1065 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/logical_plan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3973 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/logical_plan_util.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2197 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/logical_projection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1947 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/logical_union.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      980 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/logical_unwind.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/persistent/
+-rw-rw-r--   0 runner    (1001) docker     (127)      329 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/persistent/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      853 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_copy_from.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      620 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_copy_to.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1732 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_delete.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2031 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_insert.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1366 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_merge.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2384 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_set.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/scan/
+-rw-rw-r--   0 runner    (1001) docker     (127)      328 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/scan/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      347 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/scan/logical_expressions_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      935 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/scan/logical_index_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      643 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/scan/logical_scan_file.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      481 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/scan/logical_scan_internal_id.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      561 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/scan/logical_scan_node_property.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5973 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/schema.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/simple/
+-rw-rw-r--   0 runner    (1001) docker     (127)      185 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/simple/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      514 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/operator/simple/logical_simple.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/plan/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1042 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/plan/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1329 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/plan/append_accumulate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      814 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/plan/append_aggregate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      816 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/plan/append_cross_product.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1971 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/plan/append_delete.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      553 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/plan/append_distinct.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      399 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/plan/append_dummy_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      473 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/plan/append_expressions_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    13525 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/plan/append_extend.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      913 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/plan/append_filter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      800 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/plan/append_flatten.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      740 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/plan/append_in_query_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2692 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/plan/append_insert.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4805 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/plan/append_join.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      552 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/plan/append_limit.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      658 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/plan/append_mark_accumulate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      439 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/plan/append_multiplicity_reducer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      615 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/plan/append_order_by.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1452 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/plan/append_projection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      684 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/plan/append_scan_file.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1596 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/plan/append_scan_node.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2066 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/plan/append_set.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6469 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/plan/append_simple.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/plan/append_standalone_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      826 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/plan/append_unwind.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8216 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/plan/plan_copy.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    27166 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/plan/plan_join_order.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2684 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/plan/plan_port_db.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3074 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/plan/plan_projection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5987 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/plan/plan_read.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1829 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/plan/plan_single_query.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/plan/plan_standalone_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8673 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/plan/plan_subquery.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6119 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/plan/plan_update.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3507 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/planner.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5305 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/query_planner.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3769 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/planner/subplans_table.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/
+-rw-rw-r--   0 runner    (1001) docker     (127)      272 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1486 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     4798 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/create_factorized_table_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1633 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/create_result_collector.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8210 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/expression_mapper.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      702 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_acc_hash_join.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1102 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_accumulate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9149 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_aggregate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1046 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_comment_on.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    15415 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_copy_from.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4131 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_copy_to.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_create_macro.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1880 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_cross_product.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_ddl.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6207 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_delete.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      750 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_distinct.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1560 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_dummy_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      345 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_empty_result.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2008 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_explain.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1871 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_expressions_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6300 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_extend.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      822 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_filter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      606 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_flatten.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5911 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_hash_join.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1217 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_in_query_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2425 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_index_scan_node.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5186 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_insert.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3182 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_intersect.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      933 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_label_filter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1344 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_limit.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      784 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_mark_accumulate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2627 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_merge.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      533 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_multiplicity_reducer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4299 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_order_by.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6872 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_path_property_probe.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1251 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_projection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3425 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_recursive_extend.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1457 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_scan_file.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      816 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_scan_frontier.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1090 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_scan_node.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3519 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_scan_node_property.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3246 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_semi_masker.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6572 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_set.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4721 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_simple.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      969 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_standalone_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      593 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_transaction.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2083 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_union.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1096 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/map_unwind.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7878 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/map/plan_mapper.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/
+-rw-rw-r--   0 runner    (1001) docker     (127)      966 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/aggregate/
+-rw-rw-r--   0 runner    (1001) docker     (127)      400 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/aggregate/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    36261 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/aggregate/aggregate_hash_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1691 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/aggregate/base_aggregate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      755 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/aggregate/base_aggregate_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5452 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/aggregate/hash_aggregate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2004 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/aggregate/hash_aggregate_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4824 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/aggregate/simple_aggregate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1388 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/aggregate/simple_aggregate_scan.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/call/
+-rw-rw-r--   0 runner    (1001) docker     (127)      230 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/call/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2972 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/call/in_query_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      997 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/call/standalone_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      826 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/comment_on.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1383 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/cross_product.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/ddl/
+-rw-rw-r--   0 runner    (1001) docker     (127)      256 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/ddl/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1375 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/ddl/alter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      758 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/ddl/create_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      570 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/ddl/ddl.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      537 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/ddl/drop_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      213 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/empty_result.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2472 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/filter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1148 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/filtering_operator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1237 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/flatten.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/hash_join/
+-rw-rw-r--   0 runner    (1001) docker     (127)      270 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/hash_join/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2056 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/hash_join/hash_join_build.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8164 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/hash_join/hash_join_probe.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9244 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/hash_join/join_hash_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4450 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/index_lookup.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1780 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/index_scan.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/intersect/
+-rw-rw-r--   0 runner    (1001) docker     (127)      208 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/intersect/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     9643 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/intersect/intersect.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1413 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/limit.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/macro/
+-rw-rw-r--   0 runner    (1001) docker     (127)      217 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/macro/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      742 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/macro/create_macro.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      538 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/multiplicity_reducer.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/order_by/
+-rw-rw-r--   0 runner    (1001) docker     (127)      410 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/order_by/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    16047 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/order_by/key_block_merger.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1082 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/order_by/order_by.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    14049 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/order_by/order_by_key_encoder.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1554 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/order_by/order_by_merge.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1438 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/order_by/order_by_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    12968 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/order_by/radix_sort.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9038 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/order_by/sort_state.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    12676 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/order_by/top_k.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      834 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/order_by/top_k_scanner.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7757 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/partitioner.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/
+-rw-rw-r--   0 runner    (1001) docker     (127)      579 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      478 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/copy_rdf.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      828 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/copy_to.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8358 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/copy_to_csv.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1779 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/copy_to_parquet.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1751 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/delete.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5409 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/delete_executor.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4759 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/index_builder.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      861 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/insert.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7210 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/insert_executor.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3034 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/merge.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11774 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/node_batch_insert.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/
+-rw-rw-r--   0 runner    (1001) docker     (127)      325 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/
+-rw-rw-r--   0 runner    (1001) docker     (127)      297 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    14378 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/base_csv_reader.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4367 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/driver.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8578 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/parallel_csv_reader.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6554 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/serial_csv_reader.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/npy/
+-rw-rw-r--   0 runner    (1001) docker     (127)      211 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/npy/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    13924 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/npy/npy_reader.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/
+-rw-rw-r--   0 runner    (1001) docker     (127)      445 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      850 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/boolean_column_reader.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    24123 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/column_reader.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1234 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/interval_column_reader.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5989 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/list_column_reader.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    30053 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/parquet_reader.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1404 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/parquet_timestamp.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3928 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/string_column_reader.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3444 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/struct_column_reader.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/
+-rw-rw-r--   0 runner    (1001) docker     (127)      254 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    13995 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/rdf_reader.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    13456 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/rdf_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2966 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/rdf_utils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2052 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/reader_bind_utils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11290 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/rel_batch_insert.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      997 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/set.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6494 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/set_executor.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/
+-rw-rw-r--   0 runner    (1001) docker     (127)      564 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    12826 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/basic_column_writer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1538 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/boolean_column_writer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    16444 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/column_writer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1539 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/interval_column_writer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4734 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/list_column_writer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2633 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/parquet_rle_bp_encoder.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11700 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/parquet_writer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8703 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/string_column_writer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4078 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/struct_column_writer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8622 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/physical_operator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1022 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/profile.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1757 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/projection.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/
+-rw-rw-r--   0 runner    (1001) docker     (127)      337 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      790 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/frontier.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7361 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/frontier_scanner.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5063 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/path_property_probe.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    12941 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/recursive_join.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      323 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/scan_frontier.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2478 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/result_collector.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/scan/
+-rw-rw-r--   0 runner    (1001) docker     (127)      323 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/scan/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1565 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/scan/scan_multi_node_tables.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3737 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/scan/scan_multi_rel_tables.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      792 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/scan/scan_node_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      966 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/scan/scan_rel_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      675 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/scan/scan_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5159 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/scan_node_id.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4537 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/semi_masker.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/simple/
+-rw-rw-r--   0 runner    (1001) docker     (127)      381 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/simple/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1975 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/simple/attach_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/simple/detach_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4683 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/simple/export_db.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      527 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/simple/import_db.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2423 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/simple/install_extension.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2205 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/simple/load_extension.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      616 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/simple/simple.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/simple/use_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2443 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/skip.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/table_scan/
+-rw-rw-r--   0 runner    (1001) docker     (127)      248 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/table_scan/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2677 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/table_scan/ftable_scan_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1832 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/table_scan/union_all_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2416 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/transaction.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2656 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/operator/unwind.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2709 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/processor.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1788 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/processor_task.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/result/
+-rw-rw-r--   0 runner    (1001) docker     (127)      406 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/result/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     7137 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/result/base_hash_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    30659 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/result/factorized_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1966 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/result/factorized_table_schema.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2744 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/result/factorized_table_util.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2119 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/result/flat_tuple.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2287 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/result/mark_hash_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1499 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/result/result_set.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1170 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/processor/result/result_set_descriptor.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/
+-rw-rw-r--   0 runner    (1001) docker     (127)      561 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/buffer_manager/
+-rw-rw-r--   0 runner    (1001) docker     (127)      277 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/buffer_manager/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     6820 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/buffer_manager/bm_file_handle.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    15736 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/buffer_manager/buffer_manager.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2145 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/buffer_manager/memory_manager.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3721 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/buffer_manager/vm_region.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/compression/
+-rw-rw-r--   0 runner    (1001) docker     (127)      258 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/compression/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    35352 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/compression/compression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1880 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/file_handle.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/index/
+-rw-rw-r--   0 runner    (1001) docker     (127)      209 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/index/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    33507 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/index/hash_index.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    17815 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/index/in_mem_hash_index.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/local_storage/
+-rw-rw-r--   0 runner    (1001) docker     (127)      279 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/local_storage/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     6051 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/local_storage/local_node_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    12337 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/local_storage/local_rel_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1723 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/local_storage/local_storage.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6946 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/local_storage/local_table.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/stats/
+-rw-rw-r--   0 runner    (1001) docker     (127)      415 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/stats/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1201 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/stats/metadata_dah_info.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7988 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/stats/node_table_statistics.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5521 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/stats/nodes_store_statistics.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2458 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/stats/property_statistics.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5129 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/stats/rel_table_statistics.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4338 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/stats/rels_store_statistics.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2843 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/stats/table_statistics.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5812 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/stats/table_statistics_collection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11500 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/storage_manager.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/storage_structure/
+-rw-rw-r--   0 runner    (1001) docker     (127)      263 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/storage_structure/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     5262 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/storage_structure/db_file_utils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    23949 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/storage_structure/disk_array.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      557 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/storage_structure/in_mem_page.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    10191 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/storage_structure/overflow_file.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4291 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/storage_utils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      737 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/storage_version_info.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/store/
+-rw-rw-r--   0 runner    (1001) docker     (127)      649 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/store/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     7050 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/store/chunked_node_group.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2108 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/store/chunked_node_group_collection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    43158 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/store/column.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    27570 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/store/column_chunk.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3687 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/store/dictionary_chunk.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    10644 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/store/dictionary_column.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    22097 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/store/list_column.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    16059 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/store/list_column_chunk.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9833 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/store/node_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    10804 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/store/node_table_data.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8460 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/store/null_column.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9148 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/store/rel_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    51121 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/store/rel_table_data.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11782 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/store/string_column.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7813 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/store/string_column_chunk.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9257 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/store/struct_column.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6184 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/store/struct_column_chunk.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1779 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/store/table_data.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7083 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/undo_buffer.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/wal/
+-rw-rw-r--   0 runner    (1001) docker     (127)      191 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/wal/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     3679 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/wal/wal.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5210 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/wal/wal_record.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    13351 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/wal_replayer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1078 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/storage/wal_replayer_utils.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/transaction/
+-rw-rw-r--   0 runner    (1001) docker     (127)      240 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/transaction/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      611 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/transaction/transaction.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2976 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/transaction/transaction_context.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6237 2024-05-14 08:04:44.000000 sdist/kuzu-source/src/transaction/transaction_manager.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/
+-rw-rw-r--   0 runner    (1001) docker     (127)      489 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_cypher/
+-rw-rw-r--   0 runner    (1001) docker     (127)      949 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_cypher/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    56662 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_cypher/cypher_lexer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)   469845 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_cypher/cypher_parser.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_cypher/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3272 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_cypher/include/cypher_lexer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    88283 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_cypher/include/cypher_parser.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/
+-rw-rw-r--   0 runner    (1001) docker     (127)    10564 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     4237 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/LICENSE
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/
+-rw-rw-r--   0 runner    (1001) docker     (127)      285 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRErrorListener.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     8375 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRErrorListener.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      285 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRErrorStrategy.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5269 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRErrorStrategy.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      552 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRFileStream.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1018 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRFileStream.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4326 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRInputStream.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2623 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRInputStream.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1804 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BailErrorStrategy.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2483 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BailErrorStrategy.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1163 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BaseErrorListener.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1377 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BaseErrorListener.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     9946 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BufferedTokenStream.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     8014 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BufferedTokenStream.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      281 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CharStream.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1479 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CharStream.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4459 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonToken.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4918 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonToken.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1327 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonTokenFactory.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2564 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonTokenFactory.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1767 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonTokenStream.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2713 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonTokenStream.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      597 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ConsoleErrorListener.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1060 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ConsoleErrorListener.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    11864 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/DefaultErrorStrategy.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)    20289 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/DefaultErrorStrategy.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3484 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/DiagnosticErrorListener.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3600 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/DiagnosticErrorListener.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2152 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Exceptions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3868 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Exceptions.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1867 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/FailedPredicateException.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1096 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/FailedPredicateException.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2767 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/FlatHashMap.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2676 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/FlatHashSet.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      559 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/InputMismatchException.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      783 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/InputMismatchException.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      350 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/IntStream.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)    10251 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/IntStream.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      615 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/InterpreterRuleContext.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1604 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/InterpreterRuleContext.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6878 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Lexer.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     7038 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Lexer.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1867 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/LexerInterpreter.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1564 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/LexerInterpreter.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1234 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/LexerNoViableAltException.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      916 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/LexerNoViableAltException.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2412 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ListTokenSource.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3795 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ListTokenSource.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1585 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/NoViableAltException.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1693 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/NoViableAltException.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    19305 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Parser.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)    19393 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Parser.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    10523 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ParserInterpreter.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     7171 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ParserInterpreter.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3952 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ParserRuleContext.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5666 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ParserRuleContext.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1958 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ProxyErrorListener.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1657 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ProxyErrorListener.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1916 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RecognitionException.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3961 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RecognitionException.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4572 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Recognizer.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5733 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Recognizer.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3588 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuleContext.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5561 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuleContext.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      725 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuleContextWithAltNum.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      985 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuleContextWithAltNum.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2091 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuntimeMetaData.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     7393 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuntimeMetaData.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      246 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Token.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3462 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Token.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1217 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenFactory.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      264 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenSource.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3839 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenSource.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      284 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenStream.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6098 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenStream.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    15023 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenStreamRewriter.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)    12507 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenStreamRewriter.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5847 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/UnbufferedCharStream.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4351 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/UnbufferedCharStream.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     7467 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/UnbufferedTokenStream.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4241 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/UnbufferedTokenStream.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2105 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Version.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1907 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Vocabulary.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6943 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Vocabulary.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      270 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/WritableToken.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      676 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/WritableToken.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2560 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/antlr4-common.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5524 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/antlr4-runtime.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4193 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATN.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4845 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATN.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4158 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNConfig.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5513 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNConfig.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6500 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNConfigSet.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5185 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNConfigSet.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1252 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNDeserializationOptions.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1302 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNDeserializationOptions.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    21573 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNDeserializer.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      835 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNDeserializer.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1216 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNSimulator.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2761 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNSimulator.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1538 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNState.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4374 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNState.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      990 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNStateType.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      796 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNStateType.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      439 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNType.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1214 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ActionTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1104 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ActionTransition.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      604 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/AmbiguityInfo.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3295 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/AmbiguityInfo.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4211 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ArrayPredictionContext.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1900 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ArrayPredictionContext.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      840 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/AtomTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1084 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/AtomTransition.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      729 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/BasicBlockStartState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      649 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/BasicState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      762 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/BlockEndState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      853 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/BlockStartState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      520 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ContextSensitivityInfo.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2123 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ContextSensitivityInfo.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      561 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionEventInfo.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2459 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionEventInfo.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      934 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionInfo.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     9762 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionInfo.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      342 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionState.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      960 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      969 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/EpsilonTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1402 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/EpsilonTransition.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      527 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ErrorInfo.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1861 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ErrorInfo.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      416 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/HashUtils.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     7271 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LL1Analyzer.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3275 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LL1Analyzer.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2950 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerATNConfig.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1666 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerATNConfig.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    22025 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerATNSimulator.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     8819 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerATNSimulator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      324 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3494 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4031 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerActionExecutor.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6150 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerActionExecutor.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1460 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerActionType.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1306 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerChannelAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1908 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerChannelAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1555 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerCustomAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2772 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerCustomAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1784 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerIndexedCustomAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3046 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerIndexedCustomAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1269 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerModeAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1780 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerModeAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      977 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerMoreAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1701 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerMoreAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1010 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerPopModeAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1735 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerPopModeAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1311 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerPushModeAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1817 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerPushModeAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      977 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerSkipAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1664 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerSkipAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1269 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerTypeAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1717 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerTypeAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      584 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LookaheadEventInfo.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1914 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LookaheadEventInfo.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      736 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LoopEndState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      868 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/NotSetTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      854 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/NotSetTransition.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      484 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/OrderedATNConfigSet.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      631 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/OrderedATNConfigSet.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2789 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParseInfo.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3665 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParseInfo.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    53167 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParserATNSimulator.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)    45705 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParserATNSimulator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2278 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParserATNSimulatorOptions.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1052 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PlusBlockStartState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      842 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PlusLoopbackState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      901 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PrecedencePredicateTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1187 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PrecedencePredicateTransition.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      685 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredicateEvalInfo.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2885 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredicateEvalInfo.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1009 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredicateTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1674 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredicateTransition.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    20987 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContext.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     9173 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContext.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2360 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextCache.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2738 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextCache.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5386 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextMergeCache.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4033 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextMergeCache.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2602 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextMergeCacheOptions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextType.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5939 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionMode.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)    20991 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionMode.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     7943 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ProfilingATNSimulator.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2982 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ProfilingATNSimulator.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      891 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RangeTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      944 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RangeTransition.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      746 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RuleStartState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      911 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RuleStopState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1156 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RuleTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1484 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RuleTransition.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    14979 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SemanticContext.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     9030 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SemanticContext.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      451 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SemanticContextType.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3246 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SerializedATNView.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      898 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SetTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1267 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SetTransition.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2870 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SingletonPredictionContext.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1834 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SingletonPredictionContext.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      754 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/StarBlockStartState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1140 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/StarLoopEntryState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      644 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/StarLoopbackState.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      733 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/StarLoopbackState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      762 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/TokensStartState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      911 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/Transition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2164 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/Transition.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      730 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/TransitionType.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      778 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/TransitionType.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      680 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/WildcardTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      839 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/WildcardTransition.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2868 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFA.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3045 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFA.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1726 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFASerializer.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      772 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFASerializer.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1490 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFAState.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6068 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFAState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      509 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/LexerDFASerializer.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      533 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/LexerDFASerializer.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/internal/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2694 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/internal/Synchronization.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5499 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/internal/Synchronization.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3098 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/InterpreterDataReader.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      989 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/InterpreterDataReader.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1671 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/Interval.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3009 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/Interval.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    13209 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/IntervalSet.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6478 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/IntervalSet.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2820 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/MurmurHash.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3595 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/MurmurHash.h
+-rw-rw-r--   0 runner    (1001) docker     (127)       71 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/Predicate.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      446 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/Predicate.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/
+-rw-rw-r--   0 runner    (1001) docker     (127)      242 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Any.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      370 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Any.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      966 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Arrays.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3620 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Arrays.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1828 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/BitSet.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4837 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/CPPUtils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2582 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/CPPUtils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1195 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Casts.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4122 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Declarations.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      901 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/StringUtils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      425 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/StringUtils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      723 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Unicode.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8728 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Utf8.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2148 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Utf8.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5650 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/AbstractParseTreeVisitor.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      677 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ErrorNode.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1255 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ErrorNodeImpl.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1429 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ErrorNodeImpl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1906 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/IterativeParseTreeWalker.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2124 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/IterativeParseTreeWalker.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      349 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTree.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4216 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTree.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      288 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeListener.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1213 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeListener.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1434 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeProperty.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      430 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeType.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      285 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeVisitor.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2212 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeVisitor.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1381 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeWalker.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2031 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeWalker.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1145 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/TerminalNode.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1281 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/TerminalNodeImpl.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1003 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/TerminalNodeImpl.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6872 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/Trees.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3060 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/Trees.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/
+-rw-rw-r--   0 runner    (1001) docker     (127)      274 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/Chunk.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1460 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/Chunk.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1868 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreeMatch.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5768 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreeMatch.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1800 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreePattern.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4384 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreePattern.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    12574 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreePatternMatcher.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     8715 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreePatternMatcher.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1820 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/RuleTagToken.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4742 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/RuleTagToken.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      811 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TagChunk.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3030 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TagChunk.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      623 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TextChunk.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1464 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TextChunk.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      959 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TokenTagToken.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2786 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TokenTagToken.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4960 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPath.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2824 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPath.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      747 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathElement.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1029 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathElement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6047 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1169 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexer.g4
+-rw-rw-r--   0 runner    (1001) docker     (127)     1349 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)       98 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexer.tokens
+-rwxrwxr-x   0 runner    (1001) docker     (127)      506 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexerErrorListener.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      635 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexerErrorListener.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      647 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathRuleAnywhereElement.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      709 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathRuleAnywhereElement.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      966 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathRuleElement.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      620 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathRuleElement.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      647 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathTokenAnywhereElement.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      631 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathTokenAnywhereElement.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1054 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathTokenElement.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      623 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathTokenElement.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      665 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathWildcardAnywhereElement.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      558 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathWildcardAnywhereElement.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      621 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathWildcardElement.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      542 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathWildcardElement.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/
+-rw-rw-r--   0 runner    (1001) docker     (127)     5677 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/CHANGELOG.md
+-rw-rw-r--   0 runner    (1001) docker     (127)    12841 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1633 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/CONTRIBUTING.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     1084 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/LICENSE
+-rw-rw-r--   0 runner    (1001) docker     (127)      652 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/README
+-rw-rw-r--   0 runner    (1001) docker     (127)     4099 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/README.md
+-rw-rw-r--   0 runner    (1001) docker     (127)      314 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/SECURITY.md
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/common/
+-rw-rw-r--   0 runner    (1001) docker     (127)      621 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/common/constants.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     8011 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/common/constants.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7965 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/common/context.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     4666 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/common/context.h
+-rw-rw-r--   0 runner    (1001) docker     (127)   122784 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/common/dictionary.bin
+-rw-rw-r--   0 runner    (1001) docker     (127)    51687 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/common/dictionary.bin.br
+-rw-rw-r--   0 runner    (1001) docker     (127)   472009 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/common/dictionary.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     1951 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/common/dictionary.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      513 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/common/platform.c
+-rw-rw-r--   0 runner    (1001) docker     (127)    18385 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/common/platform.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    17424 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/common/shared_dictionary.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     2413 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/common/shared_dictionary_internal.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    10677 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/common/transform.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     3209 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/common/transform.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1723 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/common/version.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/dec/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2285 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/dec/bit_reader.c
+-rw-rw-r--   0 runner    (1001) docker     (127)    14854 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/dec/bit_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)   103991 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/dec/decode.c
+-rw-rw-r--   0 runner    (1001) docker     (127)    11996 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/dec/huffman.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     4107 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/dec/huffman.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    31612 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/dec/prefix.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5659 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/dec/state.c
+-rw-rw-r--   0 runner    (1001) docker     (127)    12546 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/dec/state.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/
+-rw-rw-r--   0 runner    (1001) docker     (127)     5673 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/backward_references.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     1301 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/backward_references.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    36639 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/backward_references_hq.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     3868 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/backward_references_hq.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8181 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/backward_references_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      813 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/bit_cost.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     1685 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/bit_cost.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4109 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/bit_cost_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1137 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/block_encoder_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7395 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/block_splitter.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     1674 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/block_splitter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    18673 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/block_splitter_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    50750 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/brotli_bit_stream.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     3477 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/brotli_bit_stream.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1485 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/cluster.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     1024 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/cluster.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    11826 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/cluster_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1019 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/command.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     6892 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/command.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6645 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/compound_dictionary.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     2493 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/compound_dictionary.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    33255 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/compress_fragment.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     3598 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/compress_fragment.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    27182 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/compress_fragment_two_pass.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     2879 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/compress_fragment_two_pass.h
+-rw-rw-r--   0 runner    (1001) docker     (127)   147154 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/dictionary_hash.c
+-rw-rw-r--   0 runner    (1001) docker     (127)      646 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/dictionary_hash.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    77547 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/encode.c
+-rw-rw-r--   0 runner    (1001) docker     (127)    23290 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/encoder_dict.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     5046 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/encoder_dict.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    14584 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/entropy_encode.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     4057 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/entropy_encode.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    32951 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/entropy_encode_static.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6024 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/fast_log.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     1650 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/fast_log.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2194 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/find_match_length.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    24481 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5097 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_composite_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    11250 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_forgetful_chain_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    10413 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_longest_match64_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    10349 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_longest_match_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9414 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_longest_match_quickly_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7226 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_rolling_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    13081 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_to_binary_tree_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3229 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/histogram.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     1875 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/histogram.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1401 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/histogram_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5839 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/literal_cost.c
+-rw-rw-r--   0 runner    (1001) docker     (127)      916 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/literal_cost.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5630 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/memory.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     4358 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/memory.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    26659 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/metablock.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     4051 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/metablock.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7642 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/metablock_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1169 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/params.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1969 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/prefix.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7592 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/quality.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6009 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/ringbuffer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3040 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/state.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    21117 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/static_dict.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     1275 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/static_dict.h
+-rw-rw-r--   0 runner    (1001) docker     (127)   469710 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/static_dict_lut.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2269 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/utf8_util.c
+-rw-rw-r--   0 runner    (1001) docker     (127)      905 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/utf8_util.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2862 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/enc/write_bits.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/fuzz/
+-rw-rw-r--   0 runner    (1001) docker     (127)      338 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/fuzz/BUILD.bazel
+-rw-rw-r--   0 runner    (1001) docker     (127)      615 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/fuzz/WORKSPACE.bazel
+-rw-rw-r--   0 runner    (1001) docker     (127)     1837 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/fuzz/decode_fuzzer.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     1073 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/fuzz/run_decode_fuzzer.c
+-rwxrwxr-x   0 runner    (1001) docker     (127)      703 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/fuzz/test_fuzzer.sh
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/include/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/include/brotli/
+-rw-rw-r--   0 runner    (1001) docker     (127)    16886 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/include/brotli/decode.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    19841 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/include/brotli/encode.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    11439 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/include/brotli/port.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3535 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/include/brotli/shared_dictionary.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2615 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/include/brotli/types.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/tools/
+-rw-rw-r--   0 runner    (1001) docker     (127)    51996 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/tools/brotli.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     4028 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/c/tools/brotli.md
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/docs/
+-rw-rw-r--   0 runner    (1001) docker     (127)   215208 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/docs/brotli-comparison-study-2015-09-22.pdf
+-rw-rw-r--   0 runner    (1001) docker     (127)     5130 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/docs/brotli.1
+-rw-rw-r--   0 runner    (1001) docker     (127)      244 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/docs/brotli.svg
+-rw-rw-r--   0 runner    (1001) docker     (127)     1767 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/docs/constants.h.3
+-rw-rw-r--   0 runner    (1001) docker     (127)    17452 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/docs/decode.h.3
+-rw-rw-r--   0 runner    (1001) docker     (127)    24109 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/docs/encode.h.3
+-rw-rw-r--   0 runner    (1001) docker     (127)     3081 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/docs/types.h.3
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/fetch-spec/
+-rw-rw-r--   0 runner    (1001) docker     (127)     6077 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/fetch-spec/shared-brotli-fetch-spec.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/scripts/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/scripts/dictionary/
+-rw-rw-r--   0 runner    (1001) docker     (127)      176 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/scripts/dictionary/README.md
+-rw-rw-r--   0 runner    (1001) docker     (127)      375 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/scripts/dictionary/step-01-download-rfc.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      882 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/scripts/dictionary/step-02-rfc-to-bin.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      875 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/scripts/dictionary/step-03-validate-bin.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2214 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/scripts/dictionary/step-04-generate-java-literals.py
+-rwxrwxr-x   0 runner    (1001) docker     (127)      283 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/scripts/download_testdata.sh
+-rw-rw-r--   0 runner    (1001) docker     (127)      273 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/scripts/libbrotlicommon.pc.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      300 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/scripts/libbrotlidec.pc.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      300 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/brotli/scripts/libbrotlienc.pc.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/fast_float/
+-rw-rw-r--   0 runner    (1001) docker     (127)       92 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/fast_float/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/fast_float/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)    94376 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/fast_float/include/fast_float.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/fastpfor/
+-rw-rw-r--   0 runner    (1001) docker     (127)      150 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/fastpfor/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    10273 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/fastpfor/LICENSE
+-rw-rw-r--   0 runner    (1001) docker     (127)     1278 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/fastpfor/README
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/
+-rw-rw-r--   0 runner    (1001) docker     (127)    59414 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/bitpacking.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    32124 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/bitpacking.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    23572 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/bitpackinghelpers.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      273 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/common.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/glob/
+-rw-rw-r--   0 runner    (1001) docker     (127)      100 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/glob/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/glob/glob/
+-rw-rw-r--   0 runner    (1001) docker     (127)    13001 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/glob/glob/glob.hpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/httplib/
+-rw-rw-r--   0 runner    (1001) docker     (127)   311527 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/httplib/httplib.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/
+-rw-rw-r--   0 runner    (1001) docker     (127)      918 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    11358 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/LICENSE
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/include/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/
+-rw-rw-r--   0 runner    (1001) docker     (127)    26550 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/aes.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    15024 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/aria.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    25694 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/asn1.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3085 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/base64.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    42463 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/bignum.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2394 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/build_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    13062 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/camellia.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    25326 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/ccm.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    38245 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/check_config.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    51905 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/cipher.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1452 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/constant_time.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    11057 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/des.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9867 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/entropy.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7031 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/error.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    16632 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/gcm.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      531 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/mbedtls_config.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    17120 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/md.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4949 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/memory_buffer_alloc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    41167 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/oid.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5270 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/pem.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    35543 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/pk.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    14433 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/platform.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1973 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/platform_time.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8667 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/platform_util.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      978 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/private_access.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    51957 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/rsa.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7854 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/sha1.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6640 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/sha256.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7084 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/sha512.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/library/
+-rw-rw-r--   0 runner    (1001) docker     (127)    73166 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/library/aes.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    36996 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/library/aria.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11007 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/library/asn1parse.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6762 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/library/base64.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    79733 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/library/bignum.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    56414 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/library/bn_mul.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    36100 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/library/camellia.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    47452 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/library/cipher.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    49271 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/library/cipher_wrap.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4532 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/library/cipher_wrap.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    17543 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/library/common.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    26150 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/library/constant_time.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    12167 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/library/constant_time_internal.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1638 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/library/constant_time_invasive.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    18774 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/library/entropy.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6513 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/library/entropy_poll.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2139 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/library/entropy_poll.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    34742 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/library/gcm.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    21294 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/library/md.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2086 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/library/md_wrap.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    27822 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/library/oid.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    14294 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/library/pem.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    17719 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/library/pk.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    29099 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/library/pk_wrap.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4205 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/library/pk_wrap.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    44156 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/library/pkparse.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5125 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/library/platform_util.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    69416 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/library/rsa.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    13253 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/library/rsa_alt_helpers.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8442 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/library/rsa_alt_helpers.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    15171 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/library/sha1.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    16212 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/library/sha256.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    18253 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/mbedtls/library/sha512.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1079 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       46 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/LICENSE
+-rw-rw-r--   0 runner    (1001) docker     (127)      976 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/Makefile
+-rw-rw-r--   0 runner    (1001) docker     (127)     1879 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/README.md
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/
+-rw-rw-r--   0 runner    (1001) docker     (127)      320 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/parquet_constants.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      406 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/parquet_constants.h
+-rw-rw-r--   0 runner    (1001) docker     (127)   200148 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/parquet_types.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    72715 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/parquet_types.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1262 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/windows_compatibility.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/
+-rwxrwxr-x   0 runner    (1001) docker     (127)     9816 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-internal.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3296 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-sinksource.cc
+-rwxrwxr-x   0 runner    (1001) docker     (127)     7266 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-sinksource.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1837 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-stubs-internal.cc
+-rwxrwxr-x   0 runner    (1001) docker     (127)    15040 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-stubs-internal.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2900 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-stubs-public.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    59102 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy.cc
+-rwxrwxr-x   0 runner    (1001) docker     (127)     9748 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3555 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/TApplicationException.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1208 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/TBase.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6849 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/TLogging.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3185 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/TToString.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3470 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/Thrift.h
+-rw-rw-r--   0 runner    (1001) docker     (127)       65 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/config.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/
+-rwxrwxr-x   0 runner    (1001) docker     (127)     7931 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TCompactProtocol.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    23953 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TCompactProtocol.tcc
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1140 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocol.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)    21319 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocol.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6374 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocolDecorator.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3216 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocolException.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1151 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocolTypes.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    18266 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TVirtualProtocol.h
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/stdcxx.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      896 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/thrift-config.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      460 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/thrift_export.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4624 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/PlatformSocket.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3699 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TBufferTransports.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)    15004 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TBufferTransports.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     9004 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TTransport.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1862 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TTransportException.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3335 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TTransportException.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5167 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TVirtualTransport.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniz/
+-rw-rw-r--   0 runner    (1001) docker     (127)      192 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniz/CMakeLists.txt
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1184 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniz/LICENSE
+-rwxrwxr-x   0 runner    (1001) docker     (127)   313123 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniz/miniz.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)    66103 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniz/miniz.hpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5058 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/miniz/miniz_wrapper.hpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/nlohmann_json/
+-rw-rw-r--   0 runner    (1001) docker     (127)   907860 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/nlohmann_json/json.hpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6268 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/nlohmann_json/json_fwd.hpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pcg/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1092 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pcg/LICENSE
+-rw-rw-r--   0 runner    (1001) docker     (127)    20241 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pcg/pcg_extras.hpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    73551 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pcg/pcg_random.hpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    24875 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pcg/pcg_uint128.hpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/
+-rw-rw-r--   0 runner    (1001) docker     (127)    11983 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1684 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/LICENSE
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/include/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/
+-rw-rw-r--   0 runner    (1001) docker     (127)    23979 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/attr.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7069 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/buffer_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    65560 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/cast.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8458 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/chrono.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      120 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/common.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2096 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/complex.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/
+-rw-rw-r--   0 runner    (1001) docker     (127)    28251 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/class.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    52330 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/common.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5491 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/descr.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    17932 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/init.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    26305 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/internals.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    42266 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1625 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/typeid.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eigen/
+-rw-rw-r--   0 runner    (1001) docker     (127)    31418 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eigen/matrix.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    18120 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eigen/tensor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      316 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eigen.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    11889 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/embed.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4731 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eval.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5002 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/functional.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8262 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/gil.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8862 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/iostream.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    79412 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/numpy.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9103 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/operators.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/options.h
+-rw-rw-r--   0 runner    (1001) docker     (127)   126075 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/pybind11.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    93433 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/pytypes.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/stl/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4185 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/stl/filesystem.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    15337 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/stl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    27013 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/stl_bind.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/tools/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2350 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/tools/FindCatch.cmake
+-rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/tools/FindEigen3.cmake
+-rw-rw-r--   0 runner    (1001) docker     (127)    11103 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/tools/FindPythonLibsNew.cmake
+-rw-rw-r--   0 runner    (1001) docker     (127)      817 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/tools/JoinPaths.cmake
+-rw-rw-r--   0 runner    (1001) docker     (127)     1423 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/tools/check-style.sh
+-rw-rw-r--   0 runner    (1001) docker     (127)      952 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/tools/cmake_uninstall.cmake.in
+-rw-rw-r--   0 runner    (1001) docker     (127)     1040 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1031 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/tools/libsize.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1282 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/tools/make_changelog.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      196 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11.pc.in
+-rw-rw-r--   0 runner    (1001) docker     (127)    13487 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11Common.cmake
+-rw-rw-r--   0 runner    (1001) docker     (127)     6930 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11Config.cmake.in
+-rw-rw-r--   0 runner    (1001) docker     (127)     8957 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11NewTools.cmake
+-rw-rw-r--   0 runner    (1001) docker     (127)     8361 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11Tools.cmake
+-rw-rw-r--   0 runner    (1001) docker     (127)       94 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/tools/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)     2104 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/tools/setup_global.py.in
+-rw-rw-r--   0 runner    (1001) docker     (127)     1234 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pybind11/tools/setup_main.py.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pyparse/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4660 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/pyparse/pyparse.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2716 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1558 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/LICENSE
+-rw-rw-r--   0 runner    (1001) docker     (127)    12166 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/bitstate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    40923 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/compile.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    77669 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/dfa.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3379 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/filtered_re2.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2794 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/include/bitmap256.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4074 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/include/filtered_re2.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3685 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/include/logging.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1027 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/include/mix.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4596 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/include/mutex.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1051 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/include/pod_array.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4107 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/include/prefilter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5397 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/include/prefilter_tree.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    20055 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/include/prog.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    41735 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/include/re2.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    25053 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/include/regexp.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2528 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/include/set.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    12285 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/include/sparse_array.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7425 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/include/sparse_set.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6625 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/include/stringpiece.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      644 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/include/strutil.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2606 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/include/unicode_casefold.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1595 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/include/unicode_groups.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1575 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/include/utf.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1028 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/include/util.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7825 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/include/walker-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6308 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/mimics_pcre.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    22890 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/nfa.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    22239 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/onepass.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    81544 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/parse.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3448 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/perl_groups.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    18698 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/prefilter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    13255 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/prefilter_tree.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    40537 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/prog.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    42418 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/re2.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    28640 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/regexp.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5872 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/rune.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4636 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/set.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    20853 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/simplify.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2118 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/stringpiece.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5691 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/strutil.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9029 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/tostring.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    13413 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/unicode_casefold.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)   122482 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/re2/unicode_groups.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/serd/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1247 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/serd/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/serd/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)    33294 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/serd/include/serd.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/serd/src/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/serd/src/LICENSES/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1424 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/serd/src/LICENSES/BSD-3-Clause.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      660 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/serd/src/LICENSES/OBSD.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      555 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/serd/src/attributes.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3172 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/serd/src/base64.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     1024 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/serd/src/base64.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1966 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/serd/src/byte_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2643 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/serd/src/byte_source.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     3444 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/serd/src/byte_source.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6676 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/serd/src/env.c
+-rw-rw-r--   0 runner    (1001) docker     (127)    46487 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/serd/src/n3.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     9699 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/serd/src/node.c
+-rw-rw-r--   0 runner    (1001) docker     (127)      871 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/serd/src/node.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    12064 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/serd/src/reader.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     4376 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/serd/src/reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3187 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/serd/src/serd_config.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      730 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/serd/src/serd_internal.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    10745 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/serd/src/serdi.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     2552 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/serd/src/stack.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3507 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/serd/src/string.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     3394 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/serd/src/string_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1233 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/serd/src/system.c
+-rw-rw-r--   0 runner    (1001) docker     (127)      650 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/serd/src/system.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      546 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/serd/src/try.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    11749 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/serd/src/uri.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     2843 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/serd/src/uri_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    36427 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/serd/src/writer.c
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1348 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/LICENSE
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4021 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/async.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2817 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/async_logger-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2560 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/async_logger.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/argv.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      986 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/env.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3170 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/helpers-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      718 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/helpers.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2050 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/common-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    13194 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/common.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2004 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/backtracer-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1165 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/backtracer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3349 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/circular_q.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      603 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/console_globals.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4707 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/file_helper-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1758 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/file_helper.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4471 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/fmt_helper.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1396 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/log_msg-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1204 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/log_msg.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1668 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/log_msg_buffer-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      935 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/log_msg_buffer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5285 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/mpmc_blocking_q.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      930 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/null_mutex.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    17897 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/os-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3922 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/os.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      620 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/periodic_worker-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1756 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/periodic_worker.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8695 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/registry-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4013 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/registry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      751 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/synchronous_factory.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4252 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/tcp_client-windows.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3885 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/tcp_client.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4275 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/thread_pool-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3519 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/thread_pool.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3134 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/udp_client-windows.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2237 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/udp_client.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      188 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/windows_include.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/
+-rw-rw-r--   0 runner    (1001) docker     (127)     7380 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bin_to_hex.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/
+-rw-rw-r--   0 runner    (1001) docker     (127)     7420 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/args.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    68076 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/chrono.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    24896 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/color.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    21245 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/compile.h
+-rw-rw-r--   0 runner    (1001) docker     (127)   111215 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/core.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1408 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/fmt.license.rst
+-rw-rw-r--   0 runner    (1001) docker     (127)    74272 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/format-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)   154517 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/format.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      100 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/locale.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    14123 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/os.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7586 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/ostream.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    20023 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/printf.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    23218 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/ranges.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4880 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/std.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9001 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/xchar.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      551 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/chrono.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      559 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/compile.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1042 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/fmt.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      554 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/ostr.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      551 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/ranges.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      641 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/std.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      548 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/xchar.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      463 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/formatter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      305 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fwd.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6725 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/logger-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    13412 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/logger.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    44468 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/pattern_formatter-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3758 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/pattern_formatter.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4777 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/android_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4875 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/ansicolor_sink-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3959 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/ansicolor_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1808 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/base_sink-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1568 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/base_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1216 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/basic_file_sink-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2295 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/basic_file_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1705 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/callback_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9452 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/daily_file_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2373 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/dist_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3243 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/dup_filter_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7121 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/hourly_file_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4445 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/kafka_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4003 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/mongo_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2049 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/msvc_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1234 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/null_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1222 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/ostream_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    12408 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/qt_sinks.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2081 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/ringbuffer_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4917 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/rotating_file_sink-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3229 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/rotating_file_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      725 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/sink-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      893 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1435 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/stdout_color_sinks-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1792 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/stdout_color_sinks.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4347 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/stdout_sinks-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2429 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/stdout_sinks.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4239 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/syslog_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4872 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/systemd_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2127 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/tcp_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1858 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/udp_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8888 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/win_eventlog_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6651 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/wincolor_sink-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2716 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/wincolor_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3118 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/spdlog-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    11771 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/spdlog.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1711 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/stopwatch.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6360 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/tweakme.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      417 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/spdlog/spdlog/version.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/taywee_args/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1105 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/taywee_args/LICENSE
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/taywee_args/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)   152995 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/taywee_args/include/args.hxx
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/utf8proc/
+-rw-rw-r--   0 runner    (1001) docker     (127)      142 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/utf8proc/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     5125 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/utf8proc/LICENSE.md
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/utf8proc/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)    32757 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/utf8proc/include/utf8proc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)  1944550 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/utf8proc/include/utf8proc_data.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      888 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/utf8proc/include/utf8proc_wrapper.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    37876 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/utf8proc/utf8proc.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4483 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/utf8proc/utf8proc_wrapper.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1194 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1529 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/LICENSE
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/common/
+-rw-rw-r--   0 runner    (1001) docker     (127)     8580 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/common/entropy_common.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2982 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/common/error_private.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    10089 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/common/fse_decompress.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    28008 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/common/xxhash.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2721 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/common/zstd_common.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/compress/
+-rw-rw-r--   0 runner    (1001) docker     (127)    26469 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/compress/fse_compress.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7555 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/compress/hist.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    32726 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/compress/huf_compress.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)   183732 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_compress.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6293 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_compress_literals.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    19309 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_compress_sequences.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    43614 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_compress_superblock.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    25428 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_double_fast.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    22459 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_fast.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    52956 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_lazy.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    25024 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_ldm.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    55766 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_opt.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/decompress/
+-rw-rw-r--   0 runner    (1001) docker     (127)    51287 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/decompress/huf_decompress.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9136 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/decompress/zstd_ddict.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    83312 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/decompress/zstd_decompress.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    61618 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/decompress/zstd_decompress_block.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/include/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/include/zstd/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/
+-rw-rw-r--   0 runner    (1001) docker     (127)    17857 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/bitstream.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5734 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/compiler.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3893 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/debug.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2396 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/error_private.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    14574 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/fse.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    18012 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/fse_static.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4717 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/huf.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    14332 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/huf_static.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    12217 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/mem.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9897 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/xxhash.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1779 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/xxhash_static.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3730 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/zstd_errors.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    13604 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/zstd_internal.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3464 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/hist.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    46030 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_compress_internal.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1262 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_compress_literals.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2210 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_compress_sequences.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1194 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_compress_superblock.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    18777 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_cwksp.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1250 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_double_fast.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1171 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_fast.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2701 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_lazy.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4010 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_ldm.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1972 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_opt.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/include/zstd/decompress/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1329 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/include/zstd/decompress/zstd_ddict.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2081 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/include/zstd/decompress/zstd_decompress_block.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6147 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/include/zstd/decompress/zstd_decompress_internal.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    61165 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/include/zstd.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    60974 2024-05-14 08:04:44.000000 sdist/kuzu-source/third_party/zstd/include/zstd_static.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/
+-rw-rw-r--   0 runner    (1001) docker     (127)      297 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/benchmark/
+-rw-rw-r--   0 runner    (1001) docker     (127)      251 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/benchmark/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     3132 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/benchmark/benchmark.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3400 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/benchmark/benchmark_runner.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/benchmark/example/
+-rw-rw-r--   0 runner    (1001) docker     (127)       73 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/benchmark/example/example.benchmark
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/benchmark/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)      994 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/benchmark/include/benchmark.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      561 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/benchmark/include/benchmark_config.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      836 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/benchmark/include/benchmark_runner.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2195 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/benchmark/main.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1846 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      332 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/README.md
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/jni/
+-rw-rw-r--   0 runner    (1001) docker     (127)    52884 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/jni/kuzu_java.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/main/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/main/java/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4861 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuConnection.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     3587 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuDataType.java
+-rw-rw-r--   0 runner    (1001) docker     (127)      716 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuDataTypeID.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     2637 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuDatabase.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     1734 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuFlatTuple.java
+-rw-rw-r--   0 runner    (1001) docker     (127)      495 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuInternalID.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     9598 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuNative.java
+-rw-rw-r--   0 runner    (1001) docker     (127)      334 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuObjectRefDestroyedException.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     2023 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuPreparedStatement.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     5236 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuQueryResult.java
+-rw-rw-r--   0 runner    (1001) docker     (127)      853 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuQuerySummary.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     4622 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValue.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     1077 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueListUtil.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     2984 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueNodeUtil.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     1034 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueRdfVariantUtil.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     1024 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueRecursiveRelUtil.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     3397 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueRelUtil.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueStructUtil.java
+-rw-rw-r--   0 runner    (1001) docker     (127)      520 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuVersion.java
+-rw-rw-r--   0 runner    (1001) docker     (127)      178 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/package-info.java
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/test/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/test/java/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/
+-rw-rw-r--   0 runner    (1001) docker     (127)    11911 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/ConnectionTest.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     5025 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/DataTypeTest.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     1454 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/DatabaseTest.java
+-rw-rw-r--   0 runner    (1001) docker     (127)      525 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/ExtensionTest.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     1865 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/FlatTupleTest.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     1663 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/PreparedStatementTest.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     4789 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/QueryResultTest.java
+-rw-rw-r--   0 runner    (1001) docker     (127)      940 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/TestBase.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     2504 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/TestHelper.java
+-rw-rw-r--   0 runner    (1001) docker     (127)    45229 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/ValueTest.java
+-rw-rw-r--   0 runner    (1001) docker     (127)      471 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/VersionTest.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     2271 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/test.java
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/third_party/
+-rw-rw-r--   0 runner    (1001) docker     (127)  2614186 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/java_api/third_party/junit-platform-console-standalone-1.9.3.jar
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1777 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     3043 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/README.md
+-rw-rw-r--   0 runner    (1001) docker     (127)      397 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/build.js
+-rw-rw-r--   0 runner    (1001) docker     (127)      615 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/clean.js
+-rw-rw-r--   0 runner    (1001) docker     (127)     4452 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/install.js
+-rw-rw-r--   0 runner    (1001) docker     (127)     5577 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/package.js
+-rw-rw-r--   0 runner    (1001) docker     (127)      672 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/package.json
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4385 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_connection.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1567 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1635 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_prepared_statement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5760 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_query_result.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      620 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_util.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/main.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4098 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_connection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2332 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2110 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_prepared_statement.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4835 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_query_result.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    14214 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_util.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/src_js/
+-rw-rw-r--   0 runner    (1001) docker     (127)    10896 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/src_js/connection.js
+-rw-rw-r--   0 runner    (1001) docker     (127)     4009 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/src_js/database.js
+-rw-rw-r--   0 runner    (1001) docker     (127)      499 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/src_js/index.js
+-rw-rw-r--   0 runner    (1001) docker     (127)      686 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/src_js/kuzu_native.js
+-rw-rw-r--   0 runner    (1001) docker     (127)      238 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/src_js/logging_level.js
+-rw-rw-r--   0 runner    (1001) docker     (127)     1210 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/src_js/prepared_statement.js
+-rw-rw-r--   0 runner    (1001) docker     (127)     4951 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/src_js/query_result.js
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/test/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2212 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/test/common.js
+-rw-rw-r--   0 runner    (1001) docker     (127)      629 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/test/test.js
+-rw-rw-r--   0 runner    (1001) docker     (127)     3089 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/test/test_concurrency.js
+-rw-rw-r--   0 runner    (1001) docker     (127)     9201 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/test/test_connection.js
+-rw-rw-r--   0 runner    (1001) docker     (127)    19348 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/test/test_data_type.js
+-rw-rw-r--   0 runner    (1001) docker     (127)    10088 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/test/test_database.js
+-rw-rw-r--   0 runner    (1001) docker     (127)      266 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/test/test_extension.js
+-rw-rw-r--   0 runner    (1001) docker     (127)    10191 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/test/test_parameter.js
+-rw-rw-r--   0 runner    (1001) docker     (127)     6242 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/test/test_query_result.js
+-rw-rw-r--   0 runner    (1001) docker     (127)      384 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/nodejs_api/test/test_version.js
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1322 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1136 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/Makefile
+-rw-rw-r--   0 runner    (1001) docker     (127)       23 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/README.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     2381 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      203 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/requirements_dev.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/cached_import/
+-rw-rw-r--   0 runner    (1001) docker     (127)      376 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/cached_import/py_cached_import.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      618 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/cached_import/py_cached_item.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)      335 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/arrow_array.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/cached_import/
+-rw-rw-r--   0 runner    (1001) docker     (127)      711 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/cached_import/py_cached_import.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      521 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/cached_import/py_cached_item.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3938 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/cached_import/py_cached_modules.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/numpy/
+-rw-rw-r--   0 runner    (1001) docker     (127)      430 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/numpy/numpy_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1379 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/numpy/numpy_type.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/
+-rw-rw-r--   0 runner    (1001) docker     (127)      718 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/pandas_analyzer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1290 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/pandas_bind.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      931 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/pandas_column.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1959 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/pandas_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1674 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_connection.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      714 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_conversion.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      940 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      676 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_object_container.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      381 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_prepared_statement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1470 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_query_result.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      709 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_query_result_converter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1031 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_str_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      379 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_udf.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pyarrow/
+-rw-rw-r--   0 runner    (1001) docker     (127)      383 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pyarrow/pyarrow_bind.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2219 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pyarrow/pyarrow_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      202 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pybind_include.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      549 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/kuzu_binding.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/numpy/
+-rw-rw-r--   0 runner    (1001) docker     (127)     9637 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/numpy/numpy_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5514 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/numpy/numpy_type.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/pandas/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3945 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/pandas/pandas_analyzer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3943 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/pandas/pandas_bind.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6572 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/pandas/pandas_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    21636 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_connection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4462 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_conversion.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3624 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      564 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_prepared_statement.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    16192 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_query_result.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7703 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_query_result_converter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7733 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_udf.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/pyarrow/
+-rw-rw-r--   0 runner    (1001) docker     (127)      866 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/pyarrow/pyarrow_bind.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4410 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_cpp/pyarrow/pyarrow_scan.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_py/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2111 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_py/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     8353 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_py/connection.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     9620 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_py/database.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1167 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_py/prepared_statement.py
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_py/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)    14470 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_py/query_result.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     7586 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_py/torch_geometric_feature_store.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4893 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_py/torch_geometric_graph_store.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    13467 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_py/torch_geometric_result_converter.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      839 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/src_py/types.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/test/
+-rw-rw-r--   0 runner    (1001) docker     (127)     5545 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/test/conftest.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    14438 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/test/ground_truth.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    24584 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/test/test_arrow.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      879 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/test/test_connection.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2687 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/test/test_database.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    12786 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/test/test_datatype.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    20051 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/test/test_df.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2331 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/test/test_exception.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      247 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/test/test_extension.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1947 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/test/test_get_header.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      222 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/test/test_helper.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4300 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/test/test_issue.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    10889 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/test/test_networkx.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     8013 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/test/test_parameter.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4511 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/test/test_prepared_statement.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1780 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/test/test_query_result.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1258 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/test/test_query_result_close.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    14156 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/test/test_scan_pandas.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    24852 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/test/test_scan_pandas_pyarrow.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1422 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/test/test_scan_polars.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      345 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/test/test_timeout.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    30361 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/test/test_torch_geometric.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4105 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/test/test_torch_geometric_remote_backend.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     5062 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/test/test_udf.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      155 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/test/test_version.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      215 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/python_api/test/type_aliases.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/rust_api/
+-rw-rw-r--   0 runner    (1001) docker     (127)        7 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/rust_api/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (127)    25753 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/rust_api/Cargo.lock
+-rw-rw-r--   0 runner    (1001) docker     (127)     1099 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/rust_api/Cargo.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)     5702 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/rust_api/build.rs
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/rust_api/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)      345 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/rust_api/include/kuzu_arrow.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9653 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/rust_api/include/kuzu_rs.h
+lrwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:47.655433 sdist/kuzu-source/tools/rust_api/kuzu-src -> ../..
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/rust_api/src/
+-rw-rw-r--   0 runner    (1001) docker     (127)      380 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/rust_api/src/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    13653 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/rust_api/src/connection.rs
+-rw-rw-r--   0 runner    (1001) docker     (127)     5847 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/rust_api/src/database.rs
+-rw-rw-r--   0 runner    (1001) docker     (127)     1763 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/rust_api/src/error.rs
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/rust_api/src/ffi/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1123 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/rust_api/src/ffi/arrow.rs
+-rw-rw-r--   0 runner    (1001) docker     (127)    12852 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/rust_api/src/ffi.rs
+-rw-rw-r--   0 runner    (1001) docker     (127)      471 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/rust_api/src/kuzu_arrow.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11867 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/rust_api/src/kuzu_rs.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2508 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/rust_api/src/lib.rs
+-rw-rw-r--   0 runner    (1001) docker     (127)    12831 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/rust_api/src/logical_type.rs
+-rw-rw-r--   0 runner    (1001) docker     (127)     9355 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/rust_api/src/query_result.rs
+-rw-rw-r--   0 runner    (1001) docker     (127)     2629 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/rust_api/src/rdf_variant.rs
+-rw-rw-r--   0 runner    (1001) docker     (127)    67772 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/rust_api/src/value.rs
+-rw-rw-r--   0 runner    (1001) docker     (127)     1730 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/rust_api/update_version.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/shell/
+-rw-rw-r--   0 runner    (1001) docker     (127)      428 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/shell/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    27765 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/shell/embedded_shell.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/shell/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)      912 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/shell/include/embedded_shell.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3116 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/shell/include/linenoise.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    79992 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/shell/linenoise.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3257 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/shell/shell_runner.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/shell/test/
+-rw-rw-r--   0 runner    (1001) docker     (127)     5371 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/shell/test/conftest.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/shell/test/files/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3075 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/shell/test/files/vPerson.csv
+-rw-rw-r--   0 runner    (1001) docker     (127)     1399 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/shell/test/test_helper.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4790 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/shell/test/test_shell_basics.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4804 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/shell/test/test_shell_commands.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    11969 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/shell/test/test_shell_control_edit.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    12995 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/shell/test/test_shell_control_search.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4297 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/shell/test/test_shell_esc_edit.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4571 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/shell/test/test_shell_esc_search.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4904 2024-05-14 08:04:44.000000 sdist/kuzu-source/tools/shell/test/test_shell_flags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:48.755430 sdist/kuzu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-05-14 08:04:48.755430 sdist/kuzu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-14 08:04:48.759430 sdist/kuzu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:04:48.755430 sdist/kuzu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 08:04:48.755430 sdist/kuzu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:04:48.755430 sdist/kuzu.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-14 08:04:47.903432 sdist/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-14 08:04:44.011436 sdist/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-05-14 08:04:44.011436 sdist/setup.py
```

### sdist/kuzu-source/CMakeLists.txt

```diff
@@ -1,10 +1,10 @@
 cmake_minimum_required(VERSION 3.15)
 
-project(Kuzu VERSION 0.4.2.6 LANGUAGES CXX C)
+project(Kuzu VERSION 0.4.2.7 LANGUAGES CXX C)
 
 find_package(Threads REQUIRED)
 
 set(CMAKE_CXX_STANDARD 20)
 set(CMAKE_CXX_STANDARD_REQUIRED TRUE)
 set(CMAKE_CXX_VISIBILITY_PRESET hidden)
 set(CMAKE_C_VISIBILITY_PRESET hidden)
```

### sdist/kuzu-source/src/function/aggregate/collect.cpp

```diff
@@ -39,17 +39,17 @@
     auto state = reinterpret_cast<CollectState*>(state_);
     updateSingleValue(state, input, pos, multiplicity, memoryManager);
 }
 
 void CollectFunction::initCollectStateIfNecessary(CollectState* state, MemoryManager* memoryManager,
     LogicalType& dataType) {
     if (state->factorizedTable == nullptr) {
-        auto tableSchema = std::make_unique<FactorizedTableSchema>();
-        tableSchema->appendColumn(std::make_unique<ColumnSchema>(false /* isUnflat */,
-            0 /* dataChunkPos */, StorageUtils::getDataTypeSize(dataType)));
+        auto tableSchema = FactorizedTableSchema();
+        tableSchema.appendColumn(ColumnSchema(false /* isUnflat */, 0 /* groupID */,
+            StorageUtils::getDataTypeSize(dataType)));
         state->factorizedTable =
             std::make_unique<FactorizedTable>(memoryManager, std::move(tableSchema));
     }
 }
 
 void CollectFunction::updateSingleValue(CollectState* state, ValueVector* input, uint32_t pos,
     uint64_t multiplicity, MemoryManager* memoryManager) {
```

### sdist/kuzu-source/src/include/function/hash/hash_functions.h

```diff
@@ -154,15 +154,15 @@
     auto data64 = reinterpret_cast<const uint64_t*>(key.data());
     for (size_t i = 0u; i < key.size() / 8; i++) {
         auto blockHash = kuzu::function::murmurhash64(*(data64 + i));
         hashValue = kuzu::function::combineHashScalar(hashValue, blockHash);
     }
     uint64_t last = 0;
     for (size_t i = 0u; i < key.size() % 8; i++) {
-        last |= key[key.size() / 8 * 8 + i] << i * 8;
+        last |= static_cast<uint64_t>(key[key.size() / 8 * 8 + i]) << i * 8;
     }
     hashValue = kuzu::function::combineHashScalar(hashValue, kuzu::function::murmurhash64(last));
     result = hashValue;
 }
 
 template<>
 inline void Hash::operation(const std::string& key, common::hash_t& result,
```

### sdist/kuzu-source/src/include/processor/operator/aggregate/aggregate_hash_table.h

```diff
@@ -39,25 +39,25 @@
         common::ValueVector*, uint64_t, uint32_t, uint32_t)>;
 
 class AggregateHashTable : public BaseHashTable {
 public:
     AggregateHashTable(storage::MemoryManager& memoryManager,
         const std::vector<common::LogicalType>& keyTypes,
         const std::vector<common::LogicalType>& payloadTypes, uint64_t numEntriesToAllocate,
-        std::unique_ptr<FactorizedTableSchema> tableSchema)
+        FactorizedTableSchema tableSchema)
         : AggregateHashTable(memoryManager, keyTypes, payloadTypes,
               std::vector<std::unique_ptr<function::AggregateFunction>>{} /* empty aggregates */,
               std::vector<common::LogicalType>{} /* empty distinct agg key*/, numEntriesToAllocate,
               std::move(tableSchema)) {}
 
     AggregateHashTable(storage::MemoryManager& memoryManager,
         std::vector<common::LogicalType> keyTypes, std::vector<common::LogicalType> payloadTypes,
         const std::vector<std::unique_ptr<function::AggregateFunction>>& aggregateFunctions,
         const std::vector<common::LogicalType>& distinctAggKeyTypes, uint64_t numEntriesToAllocate,
-        std::unique_ptr<FactorizedTableSchema> tableSchema);
+        FactorizedTableSchema tableSchema);
 
     uint8_t* getEntry(uint64_t idx) { return factorizedTable->getTuple(idx); }
 
     FactorizedTable* getFactorizedTable() { return factorizedTable.get(); }
 
     uint64_t getNumEntries() const { return factorizedTable->getNumTuples(); }
 
@@ -102,15 +102,15 @@
 
     uint64_t matchFlatVecWithFTColumn(common::ValueVector* vector, uint64_t numMayMatches,
         uint64_t& numNoMatches, uint32_t colIdx);
 
 private:
     void initializeFT(
         const std::vector<std::unique_ptr<function::AggregateFunction>>& aggregateFunctions,
-        std::unique_ptr<FactorizedTableSchema> tableSchema);
+        FactorizedTableSchema tableSchema);
 
     void initializeHashTable(uint64_t numEntriesToAllocate);
 
     void initializeTmpVectors();
 
     // ! This function will only be used by distinct aggregate, which assumes that all groupByKeys
     // are flat.
```

### sdist/kuzu-source/src/include/processor/operator/aggregate/hash_aggregate.h

```diff
@@ -33,19 +33,19 @@
     std::unique_ptr<AggregateHashTable> globalAggregateHashTable;
 };
 
 struct HashAggregateInfo {
     std::vector<DataPos> flatKeysPos;
     std::vector<DataPos> unFlatKeysPos;
     std::vector<DataPos> dependentKeysPos;
-    std::unique_ptr<FactorizedTableSchema> tableSchema;
+    FactorizedTableSchema tableSchema;
     HashTableType hashTableType;
 
     HashAggregateInfo(std::vector<DataPos> flatKeysPos, std::vector<DataPos> unFlatKeysPos,
-        std::vector<DataPos> dependentKeysPos, std::unique_ptr<FactorizedTableSchema> tableSchema,
+        std::vector<DataPos> dependentKeysPos, FactorizedTableSchema tableSchema,
         HashTableType hashTableType);
     HashAggregateInfo(const HashAggregateInfo& other);
 };
 
 struct HashAggregateLocalState {
     std::vector<common::ValueVector*> flatKeyVectors;
     std::vector<common::ValueVector*> unFlatKeyVectors;
```

### sdist/kuzu-source/src/include/processor/operator/hash_join/hash_join_build.h

```diff
@@ -34,34 +34,34 @@
 };
 
 class HashJoinBuildInfo {
     friend class HashJoinBuild;
 
 public:
     HashJoinBuildInfo(std::vector<DataPos> keysPos, std::vector<common::FStateType> fStateTypes,
-        std::vector<DataPos> payloadsPos, std::unique_ptr<FactorizedTableSchema> tableSchema)
+        std::vector<DataPos> payloadsPos, FactorizedTableSchema tableSchema)
         : keysPos{std::move(keysPos)}, fStateTypes{std::move(fStateTypes)},
           payloadsPos{std::move(payloadsPos)}, tableSchema{std::move(tableSchema)} {}
     HashJoinBuildInfo(const HashJoinBuildInfo& other)
         : keysPos{other.keysPos}, fStateTypes{other.fStateTypes}, payloadsPos{other.payloadsPos},
-          tableSchema{other.tableSchema->copy()} {}
+          tableSchema{other.tableSchema.copy()} {}
 
-    inline uint32_t getNumKeys() const { return keysPos.size(); }
+    uint32_t getNumKeys() const { return keysPos.size(); }
 
-    inline FactorizedTableSchema* getTableSchema() const { return tableSchema.get(); }
+    const FactorizedTableSchema* getTableSchema() const { return &tableSchema; }
 
-    inline std::unique_ptr<HashJoinBuildInfo> copy() const {
+    std::unique_ptr<HashJoinBuildInfo> copy() const {
         return std::make_unique<HashJoinBuildInfo>(*this);
     }
 
 private:
     std::vector<DataPos> keysPos;
     std::vector<common::FStateType> fStateTypes;
     std::vector<DataPos> payloadsPos;
-    std::unique_ptr<FactorizedTableSchema> tableSchema;
+    FactorizedTableSchema tableSchema;
 };
 
 class HashJoinBuild : public Sink {
 public:
     HashJoinBuild(std::unique_ptr<ResultSetDescriptor> resultSetDescriptor,
         std::shared_ptr<HashJoinSharedState> sharedState, std::unique_ptr<HashJoinBuildInfo> info,
         std::unique_ptr<PhysicalOperator> child, uint32_t id, const std::string& paramsString)
```

### sdist/kuzu-source/src/include/processor/operator/hash_join/join_hash_table.h

```diff
@@ -5,15 +5,15 @@
 
 namespace kuzu {
 namespace processor {
 
 class JoinHashTable : public BaseHashTable {
 public:
     JoinHashTable(storage::MemoryManager& memoryManager, common::logical_type_vec_t keyTypes,
-        std::unique_ptr<FactorizedTableSchema> tableSchema);
+        FactorizedTableSchema tableSchema);
 
     void appendVectors(const std::vector<common::ValueVector*>& keyVectors,
         const std::vector<common::ValueVector*>& payloadVectors, common::DataChunkState* keyState);
     void appendVector(common::ValueVector* vector,
         const std::vector<BlockAppendingInfo>& appendInfos, ft_col_idx_t colIdx);
 
     // Used in worst-case optimal join
```

### sdist/kuzu-source/src/include/processor/operator/order_by/order_by_data_info.h

```diff
@@ -1,38 +1,38 @@
 #pragma once
 
 #include "processor/data_pos.h"
-#include "processor/result/factorized_table.h"
+#include "processor/result/factorized_table_schema.h"
 
 namespace kuzu {
 namespace processor {
 
 struct OrderByDataInfo {
     std::vector<DataPos> keysPos;
     std::vector<DataPos> payloadsPos;
     std::vector<std::unique_ptr<common::LogicalType>> keyTypes;
     std::vector<std::unique_ptr<common::LogicalType>> payloadTypes;
     std::vector<bool> isAscOrder;
-    std::unique_ptr<FactorizedTableSchema> payloadTableSchema;
+    FactorizedTableSchema payloadTableSchema;
     std::vector<uint32_t> keyInPayloadPos;
 
     OrderByDataInfo(std::vector<DataPos> keysPos, std::vector<DataPos> payloadsPos,
         std::vector<std::unique_ptr<common::LogicalType>> keyTypes,
         std::vector<std::unique_ptr<common::LogicalType>> payloadTypes,
-        std::vector<bool> isAscOrder, std::unique_ptr<FactorizedTableSchema> payloadTableSchema,
+        std::vector<bool> isAscOrder, FactorizedTableSchema payloadTableSchema,
         std::vector<uint32_t> keyInPayloadPos)
         : keysPos{std::move(keysPos)}, payloadsPos{std::move(payloadsPos)},
           keyTypes{std::move(keyTypes)}, payloadTypes{std::move(payloadTypes)},
           isAscOrder{std::move(isAscOrder)}, payloadTableSchema{std::move(payloadTableSchema)},
           keyInPayloadPos{std::move(keyInPayloadPos)} {}
     OrderByDataInfo(const OrderByDataInfo& other)
         : keysPos{other.keysPos}, payloadsPos{other.payloadsPos},
           keyTypes{common::LogicalType::copy(other.keyTypes)},
           payloadTypes{common::LogicalType::copy(other.payloadTypes)}, isAscOrder{other.isAscOrder},
-          payloadTableSchema{other.payloadTableSchema->copy()},
+          payloadTableSchema{other.payloadTableSchema.copy()},
           keyInPayloadPos{other.keyInPayloadPos} {}
 
     std::unique_ptr<OrderByDataInfo> copy() const {
         return std::make_unique<OrderByDataInfo>(*this);
     }
 };
```

### sdist/kuzu-source/src/include/processor/operator/persistent/copy_to_parquet.h

```diff
@@ -7,28 +7,28 @@
 
 namespace kuzu {
 namespace processor {
 
 struct CopyToParquetInfo final : public CopyToInfo {
     kuzu_parquet::format::CompressionCodec::type codec =
         kuzu_parquet::format::CompressionCodec::SNAPPY;
-    std::unique_ptr<FactorizedTableSchema> tableSchema;
+    FactorizedTableSchema tableSchema;
     std::vector<std::unique_ptr<common::LogicalType>> types;
     DataPos countingVecPos;
 
-    CopyToParquetInfo(std::unique_ptr<FactorizedTableSchema> tableSchema,
+    CopyToParquetInfo(FactorizedTableSchema tableSchema,
         std::vector<std::unique_ptr<common::LogicalType>> types, std::vector<std::string> names,
         std::vector<DataPos> dataPoses, std::string fileName, DataPos countingVecPos,
         bool canParallel)
         : CopyToInfo{std::move(names), std::move(dataPoses), std::move(fileName), canParallel},
           tableSchema{std::move(tableSchema)}, types{std::move(types)},
           countingVecPos{std::move(countingVecPos)} {}
 
     std::unique_ptr<CopyToInfo> copy() override {
-        return std::make_unique<CopyToParquetInfo>(tableSchema->copy(),
+        return std::make_unique<CopyToParquetInfo>(tableSchema.copy(),
             common::LogicalType::copy(types), names, dataPoses, fileName, countingVecPos,
             canParallel);
     }
 };
 
 class CopyToParquetLocalState final : public CopyToLocalState {
     void init(CopyToInfo* info, storage::MemoryManager* mm, ResultSet* resultSet) override;
```

### sdist/kuzu-source/src/include/processor/operator/result_collector.h

```diff
@@ -22,23 +22,23 @@
 private:
     std::mutex mtx;
     std::shared_ptr<FactorizedTable> table;
 };
 
 struct ResultCollectorInfo {
     common::AccumulateType accumulateType;
-    std::unique_ptr<FactorizedTableSchema> tableSchema;
+    FactorizedTableSchema tableSchema;
     std::vector<DataPos> payloadPositions;
 
-    ResultCollectorInfo(common::AccumulateType accumulateType,
-        std::unique_ptr<FactorizedTableSchema> tableSchema, std::vector<DataPos> payloadPositions)
+    ResultCollectorInfo(common::AccumulateType accumulateType, FactorizedTableSchema tableSchema,
+        std::vector<DataPos> payloadPositions)
         : accumulateType{accumulateType}, tableSchema{std::move(tableSchema)},
           payloadPositions{std::move(payloadPositions)} {}
     ResultCollectorInfo(const ResultCollectorInfo& other)
-        : accumulateType{other.accumulateType}, tableSchema{other.tableSchema->copy()},
+        : accumulateType{other.accumulateType}, tableSchema{other.tableSchema.copy()},
           payloadPositions{other.payloadPositions} {}
 
     inline std::unique_ptr<ResultCollectorInfo> copy() const {
         return std::make_unique<ResultCollectorInfo>(*this);
     }
 };
```

### sdist/kuzu-source/src/include/processor/plan_mapper.h

```diff
@@ -102,14 +102,15 @@
         std::shared_ptr<PartitionerSharedState> partitionerSharedState,
         std::shared_ptr<BatchInsertSharedState> sharedState, planner::LogicalCopyFrom* copyFrom,
         common::RelDataDirection direction, std::vector<common::LogicalType> columnTypes);
 
     std::unique_ptr<ResultCollector> createResultCollector(common::AccumulateType accumulateType,
         const binder::expression_vector& expressions, planner::Schema* schema,
         std::unique_ptr<PhysicalOperator> prevOperator);
+
     // Scan fTable with row offset.
     std::unique_ptr<PhysicalOperator> createFTableScan(const binder::expression_vector& exprs,
         std::vector<ft_col_idx_t> colIndices, std::shared_ptr<binder::Expression> offset,
         planner::Schema* schema, std::shared_ptr<FactorizedTable> table, uint64_t maxMorselSize,
         std::unique_ptr<PhysicalOperator> child);
     // Scan fTable without row offset.
     std::unique_ptr<PhysicalOperator> createFTableScan(const binder::expression_vector& exprs,
@@ -171,17 +172,15 @@
     std::unique_ptr<RelInsertExecutor> getRelInsertExecutor(const planner::LogicalInsertInfo* info,
         const planner::Schema& inSchema, const planner::Schema& outSchema) const;
     std::unique_ptr<NodeSetExecutor> getNodeSetExecutor(planner::LogicalSetPropertyInfo* info,
         const planner::Schema& inSchema) const;
     std::unique_ptr<RelSetExecutor> getRelSetExecutor(planner::LogicalSetPropertyInfo* info,
         const planner::Schema& inSchema) const;
 
-    std::shared_ptr<FactorizedTable> getSingleStringColumnFTable() const;
-
-    inline uint32_t getOperatorID() { return physicalOperatorID++; }
+    uint32_t getOperatorID() { return physicalOperatorID++; }
 
     static void mapSIPJoin(PhysicalOperator* probe);
 
     static std::vector<DataPos> getDataPos(const binder::expression_vector& expressions,
         const planner::Schema& schema);
 
     static DataPos getDataPos(const binder::Expression& expression, const planner::Schema& schema) {
```

### sdist/kuzu-source/src/include/processor/result/factorized_table.h

```diff
@@ -2,27 +2,20 @@
 
 #include <algorithm>
 #include <numeric>
 
 #include "common/in_mem_overflow_buffer.h"
 #include "common/types/value/value.h"
 #include "common/vector/value_vector.h"
-#include "processor/data_pos.h"
+#include "factorized_table_schema.h"
 #include "storage/buffer_manager/memory_manager.h"
 
 namespace kuzu {
 namespace processor {
 
-// TODO(Guodong/Ziyi): Move these typedef to common and unify them with the ones without `ft_`.
-typedef uint64_t ft_tuple_idx_t;
-typedef uint32_t ft_col_idx_t;
-typedef uint32_t ft_col_offset_t;
-typedef uint32_t ft_block_idx_t;
-typedef uint32_t ft_block_offset_t;
-
 struct BlockAppendingInfo {
     BlockAppendingInfo(uint8_t* data, uint64_t numTuplesToAppend)
         : data{data}, numTuplesToAppend{numTuplesToAppend} {}
 
     uint8_t* data;
     uint64_t numTuplesToAppend;
 };
@@ -81,118 +74,39 @@
 
 private:
     uint32_t numBytesPerTuple;
     uint32_t numTuplesPerBlock;
     std::vector<std::unique_ptr<DataBlock>> blocks;
 };
 
-class ColumnSchema {
-public:
-    ColumnSchema(bool isUnflat, data_chunk_pos_t dataChunksPos, uint32_t numBytes)
-        : isUnflat{isUnflat}, dataChunkPos{dataChunksPos}, numBytes{numBytes},
-          mayContainNulls{false} {}
-
-    ColumnSchema(const ColumnSchema& other);
-
-    inline bool isFlat() const { return !isUnflat; }
-
-    inline data_chunk_pos_t getDataChunkPos() const { return dataChunkPos; }
-
-    inline uint32_t getNumBytes() const { return numBytes; }
-
-    inline bool operator==(const ColumnSchema& other) const {
-        return isUnflat == other.isUnflat && dataChunkPos == other.dataChunkPos &&
-               numBytes == other.numBytes;
-    }
-    inline bool operator!=(const ColumnSchema& other) const { return !(*this == other); }
-
-    inline void setMayContainsNullsToTrue() { mayContainNulls = true; }
-
-    inline bool hasNoNullGuarantee() const { return !mayContainNulls; }
-
-private:
-    // We need isUnflat, dataChunkPos to know the factorization structure in the factorizedTable.
-    bool isUnflat;
-    data_chunk_pos_t dataChunkPos;
-    uint32_t numBytes;
-    bool mayContainNulls;
-};
-
-class FactorizedTableSchema {
-public:
-    FactorizedTableSchema() = default;
-
-    FactorizedTableSchema(const FactorizedTableSchema& other);
-
-    explicit FactorizedTableSchema(std::vector<std::unique_ptr<ColumnSchema>> columns)
-        : columns{std::move(columns)} {}
-
-    void appendColumn(std::unique_ptr<ColumnSchema> column);
-
-    inline ColumnSchema* getColumn(ft_col_idx_t idx) const { return columns[idx].get(); }
-
-    inline uint32_t getNumColumns() const { return columns.size(); }
-
-    inline ft_col_offset_t getNullMapOffset() const { return numBytesForDataPerTuple; }
-
-    inline uint32_t getNumBytesPerTuple() const { return numBytesPerTuple; }
-
-    inline ft_col_offset_t getColOffset(ft_col_idx_t idx) const { return colOffsets[idx]; }
-
-    inline void setMayContainsNullsToTrue(ft_col_idx_t idx) {
-        KU_ASSERT(idx < columns.size());
-        columns[idx]->setMayContainsNullsToTrue();
-    }
-
-    inline bool isEmpty() const { return columns.empty(); }
-
-    bool operator==(const FactorizedTableSchema& other) const;
-    inline bool operator!=(const FactorizedTableSchema& other) const { return !(*this == other); }
-
-    inline std::unique_ptr<FactorizedTableSchema> copy() const {
-        return std::make_unique<FactorizedTableSchema>(*this);
-    }
-
-    uint64_t getNumFlatColumns() const;
-    uint64_t getNumUnflatColumns() const;
-
-private:
-    std::vector<std::unique_ptr<ColumnSchema>> columns;
-    uint32_t numBytesForDataPerTuple = 0;
-    uint32_t numBytesForNullMapPerTuple = 0;
-    uint32_t numBytesPerTuple = 0;
-    std::vector<ft_col_offset_t> colOffsets;
-};
-
 class FlatTupleIterator;
 
 class FactorizedTable {
     friend FlatTupleIterator;
     friend class JoinHashTable;
     friend class PathPropertyProbe;
 
 public:
-    FactorizedTable(storage::MemoryManager* memoryManager,
-        std::unique_ptr<FactorizedTableSchema> tableSchema);
+    FactorizedTable(storage::MemoryManager* memoryManager, FactorizedTableSchema tableSchema);
 
     void append(const std::vector<common::ValueVector*>& vectors);
 
     //! This function appends an empty tuple to the factorizedTable and returns a pointer to that
     //! tuple.
     uint8_t* appendEmptyTuple();
 
     // This function scans numTuplesToScan of rows to vectors starting at tupleIdx. Callers are
     // responsible for making sure all the parameters are valid.
-    inline void scan(std::vector<common::ValueVector*>& vectors, ft_tuple_idx_t tupleIdx,
+    void scan(std::vector<common::ValueVector*>& vectors, ft_tuple_idx_t tupleIdx,
         uint64_t numTuplesToScan) const {
-        std::vector<uint32_t> colIdxes(tableSchema->getNumColumns());
+        std::vector<uint32_t> colIdxes(tableSchema.getNumColumns());
         iota(colIdxes.begin(), colIdxes.end(), 0);
         scan(vectors, tupleIdx, numTuplesToScan, colIdxes);
     }
-    inline bool isEmpty() const { return getNumTuples() == 0; }
+    bool isEmpty() const { return getNumTuples() == 0; }
     void scan(std::vector<common::ValueVector*>& vectors, ft_tuple_idx_t tupleIdx,
         uint64_t numTuplesToScan, std::vector<uint32_t>& colIdxToScan) const;
     // TODO(Guodong): Unify these two interfaces along with `readUnflatCol`.
     void lookup(std::vector<common::ValueVector*>& vectors, std::vector<uint32_t>& colIdxesToScan,
         uint8_t** tuplesToRead, uint64_t startPos, uint64_t numTuplesToRead) const;
     void lookup(std::vector<common::ValueVector*>& vectors,
         const common::SelectionVector* selVector, std::vector<uint32_t>& colIdxesToScan,
@@ -202,83 +116,83 @@
         uint64_t numTuplesToRead) const;
 
     // When we merge two factorizedTables, we need to update the hasNoNullGuarantee based on
     // other factorizedTable.
     void mergeMayContainNulls(FactorizedTable& other);
     void merge(FactorizedTable& other);
 
-    inline common::InMemOverflowBuffer* getInMemOverflowBuffer() const {
+    common::InMemOverflowBuffer* getInMemOverflowBuffer() const {
         return inMemOverflowBuffer.get();
     }
 
     bool hasUnflatCol() const;
-    inline bool hasUnflatCol(std::vector<ft_col_idx_t>& colIdxes) const {
+    bool hasUnflatCol(std::vector<ft_col_idx_t>& colIdxes) const {
         return std::any_of(colIdxes.begin(), colIdxes.end(),
-            [this](ft_col_idx_t colIdx) { return !tableSchema->getColumn(colIdx)->isFlat(); });
+            [this](ft_col_idx_t colIdx) { return !tableSchema.getColumn(colIdx)->isFlat(); });
     }
 
-    inline uint64_t getNumTuples() const { return numTuples; }
+    uint64_t getNumTuples() const { return numTuples; }
     uint64_t getTotalNumFlatTuples() const;
     uint64_t getNumFlatTuples(ft_tuple_idx_t tupleIdx) const;
 
-    inline const std::vector<std::unique_ptr<DataBlock>>& getTupleDataBlocks() {
+    const std::vector<std::unique_ptr<DataBlock>>& getTupleDataBlocks() {
         return flatTupleBlockCollection->getBlocks();
     }
-    inline const FactorizedTableSchema* getTableSchema() const { return tableSchema.get(); }
+    const FactorizedTableSchema* getTableSchema() const { return &tableSchema; }
 
     template<typename TYPE>
-    inline TYPE getData(ft_block_idx_t blockIdx, ft_block_offset_t blockOffset,
+    TYPE getData(ft_block_idx_t blockIdx, ft_block_offset_t blockOffset,
         ft_col_offset_t colOffset) const {
         return *((TYPE*)getCell(blockIdx, blockOffset, colOffset));
     }
 
     uint8_t* getTuple(ft_tuple_idx_t tupleIdx) const;
 
     void updateFlatCell(uint8_t* tuplePtr, ft_col_idx_t colIdx, common::ValueVector* valueVector,
         uint32_t pos);
-    inline void updateFlatCellNoNull(uint8_t* ftTuplePtr, ft_col_idx_t colIdx, void* dataBuf) {
-        memcpy(ftTuplePtr + tableSchema->getColOffset(colIdx), dataBuf,
-            tableSchema->getColumn(colIdx)->getNumBytes());
+    void updateFlatCellNoNull(uint8_t* ftTuplePtr, ft_col_idx_t colIdx, void* dataBuf) {
+        memcpy(ftTuplePtr + tableSchema.getColOffset(colIdx), dataBuf,
+            tableSchema.getColumn(colIdx)->getNumBytes());
     }
 
-    inline uint64_t getNumTuplesPerBlock() const { return numFlatTuplesPerBlock; }
+    uint64_t getNumTuplesPerBlock() const { return numFlatTuplesPerBlock; }
 
-    inline bool hasNoNullGuarantee(ft_col_idx_t colIdx) const {
-        return tableSchema->getColumn(colIdx)->hasNoNullGuarantee();
+    bool hasNoNullGuarantee(ft_col_idx_t colIdx) const {
+        return tableSchema.getColumn(colIdx)->hasNoNullGuarantee();
     }
 
     bool isOverflowColNull(const uint8_t* nullBuffer, ft_tuple_idx_t tupleIdx,
         ft_col_idx_t colIdx) const;
     bool isNonOverflowColNull(const uint8_t* nullBuffer, ft_col_idx_t colIdx) const;
     void setNonOverflowColNull(uint8_t* nullBuffer, ft_col_idx_t colIdx);
     void clear();
 
 private:
     void setOverflowColNull(uint8_t* nullBuffer, ft_col_idx_t colIdx, ft_tuple_idx_t tupleIdx);
 
     uint64_t computeNumTuplesToAppend(
         const std::vector<common::ValueVector*>& vectorsToAppend) const;
 
-    inline uint8_t* getCell(ft_block_idx_t blockIdx, ft_block_offset_t blockOffset,
+    uint8_t* getCell(ft_block_idx_t blockIdx, ft_block_offset_t blockOffset,
         ft_col_offset_t colOffset) const {
         return flatTupleBlockCollection->getBlock(blockIdx)->getData() +
-               blockOffset * tableSchema->getNumBytesPerTuple() + colOffset;
+               blockOffset * tableSchema.getNumBytesPerTuple() + colOffset;
     }
-    inline std::pair<ft_block_idx_t, ft_block_offset_t> getBlockIdxAndTupleIdxInBlock(
+    std::pair<ft_block_idx_t, ft_block_offset_t> getBlockIdxAndTupleIdxInBlock(
         uint64_t tupleIdx) const {
         return std::make_pair(tupleIdx / numFlatTuplesPerBlock, tupleIdx % numFlatTuplesPerBlock);
     }
 
     std::vector<BlockAppendingInfo> allocateFlatTupleBlocks(uint64_t numTuplesToAppend);
     uint8_t* allocateUnflatTupleBlock(uint32_t numBytes);
     void copyFlatVectorToFlatColumn(const common::ValueVector& vector,
         const BlockAppendingInfo& blockAppendInfo, ft_col_idx_t colIdx);
     void copyUnflatVectorToFlatColumn(const common::ValueVector& vector,
         const BlockAppendingInfo& blockAppendInfo, uint64_t numAppendedTuples, ft_col_idx_t colIdx);
-    inline void copyVectorToFlatColumn(const common::ValueVector& vector,
+    void copyVectorToFlatColumn(const common::ValueVector& vector,
         const BlockAppendingInfo& blockAppendInfo, uint64_t numAppendedTuples,
         ft_col_idx_t colIdx) {
         vector.state->isFlat() ?
             copyFlatVectorToFlatColumn(vector, blockAppendInfo, colIdx) :
             copyUnflatVectorToFlatColumn(vector, blockAppendInfo, numAppendedTuples, colIdx);
     }
     void copyVectorToUnflatColumn(const common::ValueVector& vector,
@@ -299,61 +213,49 @@
         common::ValueVector& vector, uint64_t numTuplesToRead) const;
     void readFlatCol(uint8_t** tuplesToRead, ft_col_idx_t colIdx, common::ValueVector& vector,
         uint64_t numTuplesToRead) const;
 
 private:
     storage::MemoryManager* memoryManager;
     // Table Schema. Keeping track of factorization structure.
-    std::unique_ptr<FactorizedTableSchema> tableSchema;
+    FactorizedTableSchema tableSchema;
     // Number of rows in table.
     uint64_t numTuples;
     // Radix sort requires there is a fixed number of tuple in a block.
     uint64_t flatTupleBlockSize;
     uint32_t numFlatTuplesPerBlock;
     // Data blocks for flat tuples.
     std::unique_ptr<DataBlockCollection> flatTupleBlockCollection;
     // Data blocks for unFlat tuples.
     std::unique_ptr<DataBlockCollection> unFlatTupleBlockCollection;
     // Overflow buffer storing variable size part of an entry.
     std::unique_ptr<common::InMemOverflowBuffer> inMemOverflowBuffer;
 };
 
-// TODO(Ziyi): These two functions are used to store the copy message in a factorizedTable because
-// the current QueryProcessor::execute requires the last operator in the physical plan must be
-// ResultCollector. We should remove this class after we remove the assumption that the last
-// operator in the pipeline must be resultCollector.
-class FactorizedTableUtils {
-public:
-    static void appendStringToTable(FactorizedTable* factorizedTable, std::string& outputMsg,
-        storage::MemoryManager* memoryManager);
-    static std::shared_ptr<FactorizedTable> getFactorizedTableForOutputMsg(std::string& outputMsg,
-        storage::MemoryManager* memoryManager);
-};
-
 class FlatTupleIterator {
 public:
     explicit FlatTupleIterator(FactorizedTable& factorizedTable,
         std::vector<common::Value*> values);
 
-    inline bool hasNextFlatTuple() {
+    bool hasNextFlatTuple() {
         return nextTupleIdx < factorizedTable.getNumTuples() || nextFlatTupleIdx < numFlatTuples;
     }
 
     void getNextFlatTuple();
 
     void resetState();
 
 private:
     // The dataChunkPos may be not consecutive, which means some entries in the
     // flatTuplePositionsInDataChunk is invalid. We put pair(UINT64_MAX, UINT64_MAX) in the
     // invalid entries.
-    inline bool isValidDataChunkPos(uint32_t dataChunkPos) const {
+    bool isValidDataChunkPos(uint32_t dataChunkPos) const {
         return flatTuplePositionsInDataChunk[dataChunkPos].first != UINT64_MAX;
     }
-    inline void readValueBufferToValue(uint64_t colIdx, const uint8_t* valueBuffer) {
+    void readValueBufferToValue(uint64_t colIdx, const uint8_t* valueBuffer) {
         values[colIdx]->copyFromRowLayout(valueBuffer);
     }
 
     void readUnflatColToFlatTuple(ft_col_idx_t colIdx, uint8_t* valueBuffer);
 
     void readFlatColToFlatTuple(ft_col_idx_t colIdx, uint8_t* valueBuffer);
 
@@ -363,15 +265,15 @@
 
     // This function is used to update the number of elements in the dataChunk when we want
     // to iterate a new tuple.
     void updateNumElementsInDataChunk();
 
     // This function updates the flatTuplePositionsInDataChunk, so that getNextFlatTuple() can
     // correctly outputs the next flat tuple in the current tuple. For example, we want to read
-    // two unflat columns, which are on different dataChunks A,B and both have 100 columns. The
+    // two unFlat columns, which are on different dataChunks A,B and both have 100 columns. The
     // flatTuplePositionsInDataChunk after the first call to getNextFlatTuple() looks like:
     // {dataChunkA : [0, 100]}, {dataChunkB : [0, 100]} This function updates the
     // flatTuplePositionsInDataChunk to: {dataChunkA: [1, 100]}, {dataChunkB: [0, 100]}. Meaning
     // that the getNextFlatTuple() should read the second element in the first unflat column and
     // the first element in the second unflat column.
     void updateFlatTuplePositionsInDataChunk();
```

### sdist/kuzu-source/src/include/processor/result/mark_hash_table.h

```diff
@@ -5,15 +5,15 @@
 namespace kuzu {
 namespace processor {
 
 class MarkHashTable : public AggregateHashTable {
 public:
     MarkHashTable(storage::MemoryManager& memoryManager, std::vector<common::LogicalType> keyTypes,
         std::vector<common::LogicalType> payloadTypes, uint64_t numEntriesToAllocate,
-        std::unique_ptr<FactorizedTableSchema> tableSchema);
+        FactorizedTableSchema tableSchema);
 
     uint64_t matchFTEntries(const std::vector<common::ValueVector*>& flatKeyVectors,
         const std::vector<common::ValueVector*>& unFlatKeyVectors, uint64_t numMayMatches,
         uint64_t numNoMatches) override;
 
     void initializeFTEntries(const std::vector<common::ValueVector*>& flatKeyVectors,
         const std::vector<common::ValueVector*>& unFlatKeyVectors,
```

### sdist/kuzu-source/src/include/storage/index/hash_index.h

```diff
@@ -103,41 +103,40 @@
         Key key, uint8_t fingerprint) const;
 
     inline void updateSlot(const SlotInfo& slotInfo, const Slot<T>& slot) {
         slotInfo.slotType == SlotType::PRIMARY ? pSlots->update(slotInfo.slotId, slot) :
                                                  oSlots->update(slotInfo.slotId, slot);
     }
 
-    inline Slot<T> getSlot(transaction::TransactionType trxType, const SlotInfo& slotInfo) {
+    inline Slot<T> getSlot(transaction::TransactionType trxType, const SlotInfo& slotInfo) const {
         return slotInfo.slotType == SlotType::PRIMARY ? pSlots->get(slotInfo.slotId, trxType) :
                                                         oSlots->get(slotInfo.slotId, trxType);
     }
 
     inline uint32_t appendPSlot() { return pSlots->pushBack(Slot<T>{}); }
 
     inline uint64_t appendOverflowSlot(Slot<T>&& newSlot) { return oSlots->pushBack(newSlot); }
 
     void splitSlots(HashIndexHeader& header, slot_id_t numSlotsToSplit);
 
     // Resizes the local storage to support the given number of new entries
-    inline void bulkReserve(uint64_t newEntries) override {
-        bulkInsertLocalStorage.reserve(newEntries);
-    }
+    void bulkReserve(uint64_t newEntries) override;
     // Resizes the on-disk index to support the given number of new entries
     void reserve(uint64_t newEntries);
 
     struct HashIndexEntryView {
         slot_id_t diskSlotId;
         uint8_t fingerprint;
         const SlotEntry<T>* entry;
     };
 
-    void sortEntries(typename InMemHashIndex<T>::SlotIterator& slotToMerge,
+    void sortEntries(const InMemHashIndex<T>& insertLocalStorage,
+        typename InMemHashIndex<T>::SlotIterator& slotToMerge,
         std::vector<HashIndexEntryView>& partitions);
-    void mergeBulkInserts();
+    void mergeBulkInserts(const InMemHashIndex<T>& insertLocalStorage);
     // Returns the number of elements merged which matched the given slot id
     size_t mergeSlot(const std::vector<HashIndexEntryView>& slotToMerge,
         typename BaseDiskArray<Slot<T>>::WriteIterator& diskSlotIterator,
         typename BaseDiskArray<Slot<T>>::WriteIterator& diskOverflowSlotIterator, slot_id_t slotId);
 
     inline bool equals(transaction::TransactionType /*trxType*/, Key keyToLookup,
         const T& keyInEntry) const {
@@ -168,15 +167,15 @@
     };
 
     SlotIterator getSlotIterator(slot_id_t slotId, transaction::TransactionType trxType) {
         return SlotIterator{SlotInfo{slotId, SlotType::PRIMARY},
             getSlot(trxType, SlotInfo{slotId, SlotType::PRIMARY})};
     }
 
-    bool nextChainedSlot(transaction::TransactionType trxType, SlotIterator& iter) {
+    bool nextChainedSlot(transaction::TransactionType trxType, SlotIterator& iter) const {
         KU_ASSERT(iter.slotInfo.slotType == SlotType::PRIMARY ||
                   iter.slotInfo.slotId != iter.slot.header.nextOvfSlotId);
         if (iter.slot.header.nextOvfSlotId != 0) {
             iter.slotInfo.slotId = iter.slot.header.nextOvfSlotId;
             iter.slotInfo.slotType = SlotType::OVF;
             iter.slot = getSlot(trxType, iter.slotInfo);
             return true;
@@ -215,16 +214,15 @@
     BufferManager& bm;
     WAL* wal;
     std::shared_ptr<BMFileHandle> fileHandle;
     std::unique_ptr<BaseDiskArray<HashIndexHeader>> headerArray;
     std::unique_ptr<BaseDiskArray<Slot<T>>> pSlots;
     std::unique_ptr<BaseDiskArray<Slot<T>>> oSlots;
     OverflowFileHandle* overflowFileHandle;
-    std::unique_ptr<HashIndexLocalStorage<BufferKeyType>> localStorage;
-    InMemHashIndex<T> bulkInsertLocalStorage;
+    std::unique_ptr<HashIndexLocalStorage<T>> localStorage;
     std::unique_ptr<HashIndexHeader> indexHeaderForReadTrx;
     std::unique_ptr<HashIndexHeader> indexHeaderForWriteTrx;
 };
 
 template<>
 common::hash_t HashIndex<common::ku_string_t>::hashStored(transaction::TransactionType trxType,
     const common::ku_string_t& key) const;
```

### sdist/kuzu-source/src/include/storage/index/in_mem_hash_index.h

```diff
@@ -68,52 +68,61 @@
     // This reserves space for numEntries in total, regardless of existing entries in the builder
     void reserve(uint32_t numEntries);
     // Allocates the given number of new slots, ignoo
     void allocateSlots(uint32_t numSlots);
 
     using BufferKeyType =
         typename std::conditional<std::same_as<T, common::ku_string_t>, std::string, T>::type;
+    using Key =
+        typename std::conditional<std::same_as<T, common::ku_string_t>, std::string_view, T>::type;
     // Appends the buffer to the index. Returns the number of values successfully inserted.
     // I.e. if a key fails to insert, its index will be the return value
     size_t append(const IndexBuffer<BufferKeyType>& buffer);
-    using Key =
-        typename std::conditional<std::same_as<T, common::ku_string_t>, std::string_view, T>::type;
+    inline bool append(Key key, common::offset_t value) {
+        reserve(indexHeader.numEntries + 1);
+        return appendInternal(key, value, HashIndexUtils::hash(key));
+    }
     bool lookup(Key key, common::offset_t& result);
 
-    uint64_t size() { return this->indexHeader.numEntries; }
+    uint64_t size() const { return this->indexHeader.numEntries; }
+    bool empty() const { return size() == 0; }
 
     void clear();
 
     struct SlotIterator {
-        explicit SlotIterator(slot_id_t newSlotId, InMemHashIndex<T>* builder)
+        explicit SlotIterator(slot_id_t newSlotId, const InMemHashIndex<T>* builder)
             : slotInfo{newSlotId, SlotType::PRIMARY}, slot(builder->getSlot(slotInfo)) {}
         SlotInfo slotInfo;
         Slot<T>* slot;
     };
 
     // Leaves the slot pointer pointing at the last slot to make it easier to add a new one
-    inline bool nextChainedSlot(SlotIterator& iter) {
+    inline bool nextChainedSlot(SlotIterator& iter) const {
         iter.slotInfo.slotId = iter.slot->header.nextOvfSlotId;
         iter.slotInfo.slotType = SlotType::OVF;
         if (iter.slot->header.nextOvfSlotId != 0) {
             iter.slot = getSlot(iter.slotInfo);
             return true;
         }
         return false;
     }
 
     inline uint64_t numPrimarySlots() const { return pSlots->size(); }
     inline uint64_t numOverflowSlots() const { return oSlots->size(); }
 
-    inline HashIndexHeader getIndexHeader() { return indexHeader; }
+    inline const HashIndexHeader& getIndexHeader() const { return indexHeader; }
+
+    // Deletes key, maintaining gapless structure by replacing it with the last entry in the
+    // slot
+    bool deleteKey(Key key);
 
 private:
     // Assumes that space has already been allocated for the entry
     bool appendInternal(Key key, common::offset_t value, common::hash_t hash);
-    Slot<T>* getSlot(const SlotInfo& slotInfo);
+    Slot<T>* getSlot(const SlotInfo& slotInfo) const;
 
     uint32_t allocatePSlots(uint32_t numSlotsToAllocate);
     uint32_t allocateAOSlot();
     /*
      * When a slot is split, we add a new slot, which ends up with an
      * id equal to the slot to split's ID + (1 << header.currentLevel).
      * Values are then rehashed using a hash index which is one bit wider than before,
```

### sdist/kuzu-source/src/processor/map/create_result_collector.cpp

```diff
@@ -1,42 +1,34 @@
 #include "binder/expression/expression_util.h"
 #include "processor/operator/result_collector.h"
 #include "processor/plan_mapper.h"
+#include "processor/result/factorized_table_util.h"
 
 using namespace kuzu::common;
 using namespace kuzu::planner;
+using namespace kuzu::binder;
 
 namespace kuzu {
 namespace processor {
 
 std::unique_ptr<ResultCollector> PlanMapper::createResultCollector(AccumulateType accumulateType,
     const binder::expression_vector& expressions, Schema* schema,
     std::unique_ptr<PhysicalOperator> prevOperator) {
     std::vector<DataPos> payloadsPos;
-    auto tableSchema = std::make_unique<FactorizedTableSchema>();
-    for (auto& expression : expressions) {
-        auto dataPos = DataPos(schema->getExpressionPos(*expression));
-        std::unique_ptr<ColumnSchema> columnSchema;
-        if (schema->getGroup(dataPos.dataChunkPos)->isFlat()) {
-            columnSchema = std::make_unique<ColumnSchema>(false /* isUnFlat */,
-                dataPos.dataChunkPos, LogicalTypeUtils::getRowLayoutSize(expression->dataType));
-        } else {
-            columnSchema = std::make_unique<ColumnSchema>(true /* isUnFlat */, dataPos.dataChunkPos,
-                (uint32_t)sizeof(overflow_value_t));
-        }
-        tableSchema->appendColumn(std::move(columnSchema));
-        payloadsPos.push_back(dataPos);
+    for (auto& e : expressions) {
+        payloadsPos.push_back(getDataPos(*e, *schema));
     }
+    auto tableSchema = FactorizedTableUtils::createFTableSchema(expressions, *schema);
     if (accumulateType == AccumulateType::OPTIONAL_) {
-        auto columnSchema = std::make_unique<ColumnSchema>(false /* isUnFlat */,
-            INVALID_DATA_CHUNK_POS, LogicalTypeUtils::getRowLayoutSize(*LogicalType::BOOL()));
-        tableSchema->appendColumn(std::move(columnSchema));
+        auto columnSchema = ColumnSchema(false /* isUnFlat */, INVALID_DATA_CHUNK_POS,
+            LogicalTypeUtils::getRowLayoutSize(*LogicalType::BOOL()));
+        tableSchema.appendColumn(std::move(columnSchema));
     }
     auto table =
-        std::make_shared<FactorizedTable>(clientContext->getMemoryManager(), tableSchema->copy());
+        std::make_shared<FactorizedTable>(clientContext->getMemoryManager(), tableSchema.copy());
     auto sharedState = std::make_shared<ResultCollectorSharedState>(std::move(table));
     auto info =
         std::make_unique<ResultCollectorInfo>(accumulateType, std::move(tableSchema), payloadsPos);
     return make_unique<ResultCollector>(std::make_unique<ResultSetDescriptor>(schema),
         std::move(info), std::move(sharedState), std::move(prevOperator), getOperatorID(),
         binder::ExpressionUtil::toString(expressions));
 }
```

### sdist/kuzu-source/src/processor/map/map_aggregate.cpp

```diff
@@ -93,44 +93,42 @@
     auto aggregate = make_unique<SimpleAggregate>(std::make_unique<ResultSetDescriptor>(inSchema),
         sharedState, std::move(aggFunctions), std::move(aggregateInputInfos),
         std::move(prevOperator), getOperatorID(), paramsString);
     return make_unique<SimpleAggregateScan>(sharedState, aggOutputPos, std::move(aggregate),
         getOperatorID(), paramsString);
 }
 
-static std::unique_ptr<FactorizedTableSchema> getFactorizedTableSchema(
-    const expression_vector& flatKeys, const expression_vector& unFlatKeys,
-    const expression_vector& payloads,
+static FactorizedTableSchema getFactorizedTableSchema(const expression_vector& flatKeys,
+    const expression_vector& unFlatKeys, const expression_vector& payloads,
     std::vector<std::unique_ptr<function::AggregateFunction>>& aggregateFunctions,
     std::shared_ptr<Expression> markExpression) {
     auto isUnFlat = false;
-    auto dataChunkPos = 0u;
-    std::unique_ptr<FactorizedTableSchema> tableSchema = std::make_unique<FactorizedTableSchema>();
+    auto groupID = 0u;
+    auto tableSchema = FactorizedTableSchema();
     for (auto& flatKey : flatKeys) {
         auto size = LogicalTypeUtils::getRowLayoutSize(flatKey->dataType);
-        tableSchema->appendColumn(std::make_unique<ColumnSchema>(isUnFlat, dataChunkPos, size));
+        tableSchema.appendColumn(ColumnSchema(isUnFlat, groupID, size));
     }
     for (auto& unFlatKey : unFlatKeys) {
         auto size = LogicalTypeUtils::getRowLayoutSize(unFlatKey->dataType);
-        tableSchema->appendColumn(std::make_unique<ColumnSchema>(isUnFlat, dataChunkPos, size));
+        tableSchema.appendColumn(ColumnSchema(isUnFlat, groupID, size));
     }
     for (auto& payload : payloads) {
         auto size = LogicalTypeUtils::getRowLayoutSize(payload->dataType);
-        tableSchema->appendColumn(std::make_unique<ColumnSchema>(isUnFlat, dataChunkPos, size));
+        tableSchema.appendColumn(ColumnSchema(isUnFlat, groupID, size));
     }
     for (auto& aggregateFunc : aggregateFunctions) {
-        tableSchema->appendColumn(std::make_unique<ColumnSchema>(isUnFlat, dataChunkPos,
-            aggregateFunc->getAggregateStateSize()));
+        tableSchema.appendColumn(
+            ColumnSchema(isUnFlat, groupID, aggregateFunc->getAggregateStateSize()));
     }
     if (markExpression != nullptr) {
-        tableSchema->appendColumn(std::make_unique<ColumnSchema>(isUnFlat, dataChunkPos,
+        tableSchema.appendColumn(ColumnSchema(isUnFlat, groupID,
             LogicalTypeUtils::getRowLayoutSize(markExpression->dataType)));
     }
-    tableSchema->appendColumn(
-        std::make_unique<ColumnSchema>(isUnFlat, dataChunkPos, sizeof(hash_t)));
+    tableSchema.appendColumn(ColumnSchema(isUnFlat, groupID, sizeof(hash_t)));
     return tableSchema;
 }
 
 std::unique_ptr<PhysicalOperator> PlanMapper::createDistinctHashAggregate(
     const expression_vector& keys, const expression_vector& payloads, Schema* inSchema,
     Schema* outSchema, std::unique_ptr<PhysicalOperator> prevOperator,
     const std::string& paramsString) {
```

### sdist/kuzu-source/src/processor/map/map_copy_from.cpp

```diff
@@ -5,14 +5,15 @@
 #include "processor/operator/call/in_query_call.h"
 #include "processor/operator/index_lookup.h"
 #include "processor/operator/partitioner.h"
 #include "processor/operator/persistent/copy_rdf.h"
 #include "processor/operator/persistent/node_batch_insert.h"
 #include "processor/operator/persistent/rel_batch_insert.h"
 #include "processor/plan_mapper.h"
+#include "processor/result/factorized_table_util.h"
 #include "storage/storage_manager.h"
 
 using namespace kuzu::binder;
 using namespace kuzu::catalog;
 using namespace kuzu::common;
 using namespace kuzu::planner;
 using namespace kuzu::storage;
@@ -101,16 +102,18 @@
     auto copyFromInfo = copyFrom->getInfo();
     auto outFSchema = copyFrom->getSchema();
     auto nodeTableEntry =
         ku_dynamic_cast<TableCatalogEntry*, NodeTableCatalogEntry*>(copyFromInfo->tableEntry);
     // Map reader.
     auto prevOperator = mapOperator(copyFrom->getChild(0).get());
     auto nodeTable = storageManager->getTable(nodeTableEntry->getTableID());
-    auto sharedState = std::make_shared<NodeBatchInsertSharedState>(nodeTable,
-        getSingleStringColumnFTable(), &storageManager->getWAL());
+    auto fTable =
+        FactorizedTableUtils::getSingleStringColumnFTable(clientContext->getMemoryManager());
+    auto sharedState =
+        std::make_shared<NodeBatchInsertSharedState>(nodeTable, fTable, &storageManager->getWAL());
     if (prevOperator->getOperatorType() == PhysicalOperatorType::IN_QUERY_CALL) {
         auto inQueryCall = ku_dynamic_cast<PhysicalOperator*, InQueryCall*>(prevOperator.get());
         sharedState->readerSharedState = inQueryCall->getSharedState();
     } else {
         KU_ASSERT(prevOperator->getOperatorType() == PhysicalOperatorType::AGGREGATE_SCAN);
         auto hashScan = ku_dynamic_cast<PhysicalOperator*, HashAggregateScan*>(prevOperator.get());
         sharedState->distinctSharedState = hashScan->getSharedState().get();
@@ -209,16 +212,18 @@
         relTable->getNumTuples(&transaction::DUMMY_WRITE_TRANSACTION);
     // TODO(Xiyang): Move binding of column types to binder.
     std::vector<LogicalType> columnTypes;
     columnTypes.push_back(*LogicalType::INTERNAL_ID()); // NBR_ID COLUMN.
     for (auto& property : relTableEntry->getPropertiesRef()) {
         columnTypes.push_back(*property.getDataType()->copy());
     }
-    auto batchInsertSharedState = std::make_shared<BatchInsertSharedState>(relTable,
-        getSingleStringColumnFTable(), &storageManager->getWAL());
+    auto fTable =
+        FactorizedTableUtils::getSingleStringColumnFTable(clientContext->getMemoryManager());
+    auto batchInsertSharedState =
+        std::make_shared<BatchInsertSharedState>(relTable, fTable, &storageManager->getWAL());
     auto copyRelFWD = createCopyRel(partitionerSharedState, batchInsertSharedState, copyFrom,
         RelDataDirection::FWD, LogicalType::copy(columnTypes));
     auto copyRelBWD = createCopyRel(partitionerSharedState, batchInsertSharedState, copyFrom,
         RelDataDirection::BWD, std::move(columnTypes));
     physical_op_vector_t result;
     result.push_back(std::move(copyRelBWD));
     result.push_back(std::move(copyRelFWD));
@@ -261,15 +266,16 @@
         rCopy->getSharedState());
     rrLPartitioner->getSharedState()->nodeBatchInsertSharedStates.push_back(
         lCopy->getSharedState());
     KU_ASSERT(rrlChildren[2]->getChild(0)->getOperatorType() == PhysicalOperatorType::INDEX_LOOKUP);
     auto rrlLookup = ku_dynamic_cast<PhysicalOperator*, IndexLookup*>(rrlChildren[2]->getChild(0));
     rrlLookup->setBatchInsertSharedState(rCopy->getSharedState());
     auto sharedState = std::make_shared<CopyRdfSharedState>();
-    auto fTable = getSingleStringColumnFTable();
+    auto fTable =
+        FactorizedTableUtils::getSingleStringColumnFTable(clientContext->getMemoryManager());
     sharedState->fTable = fTable;
     auto copyRdf = std::make_unique<CopyRdf>(std::move(sharedState),
         std::make_unique<ResultSetDescriptor>(copyFrom->getSchema()), getOperatorID(), "");
     for (auto& child : rrlChildren) {
         copyRdf->addChild(std::move(child));
     }
     for (auto& child : rrrChildren) {
```

### sdist/kuzu-source/src/processor/map/map_copy_to.cpp

```diff
@@ -1,43 +1,37 @@
 #include "planner/operator/persistent/logical_copy_to.h"
 #include "processor/operator/persistent/copy_to_csv.h"
 #include "processor/operator/persistent/copy_to_parquet.h"
 #include "processor/plan_mapper.h"
+#include "processor/result/factorized_table_util.h"
 
 using namespace kuzu::common;
 using namespace kuzu::planner;
 using namespace kuzu::storage;
 
 namespace kuzu {
 namespace processor {
 
 std::unique_ptr<CopyToInfo> getCopyToInfo(Schema* childSchema, std::string filePath,
     common::FileType fileType, common::CSVOption copyToOption, std::vector<std::string> columnNames,
     std::vector<std::unique_ptr<LogicalType>> columnsTypes, std::vector<DataPos> vectorsToCopyPos,
     std::vector<bool> isFlat, bool canParallel) {
     switch (fileType) {
     case FileType::PARQUET: {
-        auto copyToSchema = std::make_unique<FactorizedTableSchema>();
-        auto copyToExpressions = childSchema->getExpressionsInScope();
-        auto countingVecPos = DataPos(childSchema->getExpressionPos(*copyToExpressions[0]));
-        for (auto& copyToExpression : copyToExpressions) {
-            auto [dataChunkPos, vectorPos] = childSchema->getExpressionPos(*copyToExpression);
-            std::unique_ptr<ColumnSchema> columnSchema;
-            if (!childSchema->getGroup(dataChunkPos)->isFlat()) {
-                // payload is unFlat and not in the same group as keys
-                columnSchema = std::make_unique<ColumnSchema>(true /* isUnFlat */, dataChunkPos,
-                    sizeof(overflow_value_t));
-                countingVecPos = DataPos(childSchema->getExpressionPos(*copyToExpression));
-            } else {
-                columnSchema = std::make_unique<ColumnSchema>(false /* isUnFlat */, dataChunkPos,
-                    LogicalTypeUtils::getRowLayoutSize(copyToExpression->getDataType()));
+        auto expressions = childSchema->getExpressionsInScope();
+        auto tableSchema = FactorizedTableUtils::createFTableSchema(expressions, *childSchema);
+        auto countingVecPos = DataPos(childSchema->getExpressionPos(*expressions[0]));
+        for (auto& e : expressions) {
+            auto group = childSchema->getGroup(e->getUniqueName());
+            if (!group->isFlat()) {
+                countingVecPos = DataPos(childSchema->getExpressionPos(*e));
             }
-            copyToSchema->appendColumn(std::move(columnSchema));
         }
-        return std::make_unique<CopyToParquetInfo>(std::move(copyToSchema), std::move(columnsTypes),
+
+        return std::make_unique<CopyToParquetInfo>(std::move(tableSchema), std::move(columnsTypes),
             std::move(columnNames), std::move(vectorsToCopyPos), std::move(filePath),
             std::move(countingVecPos), canParallel);
     }
     case FileType::CSV: {
         return std::make_unique<CopyToCSVInfo>(std::move(columnNames), std::move(vectorsToCopyPos),
             std::move(filePath), std::move(isFlat), std::move(copyToOption), canParallel);
     }
@@ -83,16 +77,14 @@
             std::move(copyToInfo), std::move(sharedState), std::move(prevOperator), getOperatorID(),
             copy->getExpressionsForPrinting());
     } else {
         copyTo = std::make_unique<CopyToCSV>(std::make_unique<ResultSetDescriptor>(childSchema),
             std::move(copyToInfo), std::move(sharedState), std::move(prevOperator), getOperatorID(),
             copy->getExpressionsForPrinting());
     }
-    std::shared_ptr<FactorizedTable> fTable;
-    auto ftTableSchema = std::make_unique<FactorizedTableSchema>();
-    fTable = std::make_shared<FactorizedTable>(clientContext->getMemoryManager(),
-        std::move(ftTableSchema));
+    auto fTable = std::make_shared<FactorizedTable>(clientContext->getMemoryManager(),
+        FactorizedTableSchema());
     return createEmptyFTableScan(fTable, 0, std::move(copyTo));
 }
 
 } // namespace processor
 } // namespace kuzu
```

### sdist/kuzu-source/src/processor/map/map_dummy_scan.cpp

```diff
@@ -6,21 +6,21 @@
 
 namespace kuzu {
 namespace processor {
 
 std::unique_ptr<PhysicalOperator> PlanMapper::mapDummyScan(LogicalOperator* /*logicalOperator*/) {
     auto inSchema = std::make_unique<Schema>();
     auto expression = LogicalDummyScan::getDummyExpression();
-    auto tableSchema = std::make_unique<FactorizedTableSchema>();
+    auto tableSchema = FactorizedTableSchema();
     // TODO(Ziyi): remove vectors when we have done the refactor of dataChunk.
     std::vector<std::shared_ptr<ValueVector>> vectors;
     std::vector<ValueVector*> vectorsToAppend;
-    tableSchema->appendColumn(
-        std::make_unique<ColumnSchema>(false, 0 /* all expressions are in the same datachunk */,
-            LogicalTypeUtils::getRowLayoutSize(expression->dataType)));
+    auto columnSchema = ColumnSchema(false, 0 /* groupID */,
+        LogicalTypeUtils::getRowLayoutSize(expression->dataType));
+    tableSchema.appendColumn(std::move(columnSchema));
     auto expressionEvaluator = ExpressionMapper::getEvaluator(expression, inSchema.get());
     auto memoryManager = clientContext->getMemoryManager();
     // expression can be evaluated statically and does not require an actual resultset to init
     expressionEvaluator->init(ResultSet(0) /* dummy resultset */, memoryManager);
     expressionEvaluator->evaluate(clientContext);
     vectors.push_back(expressionEvaluator->resultVector);
     vectorsToAppend.push_back(expressionEvaluator->resultVector.get());
```

### sdist/kuzu-source/src/processor/map/map_explain.cpp

```diff
@@ -1,12 +1,13 @@
 #include "common/profiler.h"
 #include "main/plan_printer.h"
 #include "planner/operator/logical_explain.h"
 #include "processor/operator/profile.h"
 #include "processor/plan_mapper.h"
+#include "processor/result/factorized_table_util.h"
 
 using namespace kuzu::common;
 using namespace kuzu::planner;
 using namespace kuzu::binder;
 
 namespace kuzu {
 namespace processor {
```

### sdist/kuzu-source/src/processor/map/map_hash_join.cpp

```diff
@@ -12,51 +12,51 @@
 
 std::unique_ptr<HashJoinBuildInfo> PlanMapper::createHashBuildInfo(const Schema& buildSchema,
     const expression_vector& keys, const expression_vector& payloads) {
     planner::f_group_pos_set keyGroupPosSet;
     std::vector<DataPos> keysPos;
     std::vector<FStateType> fStateTypes;
     std::vector<DataPos> payloadsPos;
-    auto tableSchema = std::make_unique<FactorizedTableSchema>();
+    auto tableSchema = FactorizedTableSchema();
     for (auto& key : keys) {
         auto pos = DataPos(buildSchema.getExpressionPos(*key));
         keyGroupPosSet.insert(pos.dataChunkPos);
         // Keys are always stored in flat column.
-        auto columnSchema = std::make_unique<ColumnSchema>(false /* isUnFlat */, pos.dataChunkPos,
+        auto columnSchema = ColumnSchema(false /* isUnFlat */, pos.dataChunkPos,
             LogicalTypeUtils::getRowLayoutSize(key->dataType));
-        tableSchema->appendColumn(std::move(columnSchema));
+        tableSchema.appendColumn(std::move(columnSchema));
         keysPos.push_back(pos);
         fStateTypes.push_back(buildSchema.getGroup(pos.dataChunkPos)->isFlat() ?
                                   FStateType::FLAT :
                                   FStateType::UNFLAT);
     }
     for (auto& payload : payloads) {
         auto pos = DataPos(buildSchema.getExpressionPos(*payload));
-        std::unique_ptr<ColumnSchema> columnSchema;
         if (keyGroupPosSet.contains(pos.dataChunkPos) ||
             buildSchema.getGroup(pos.dataChunkPos)->isFlat()) {
             // Payloads need to be stored in flat column in 2 cases
             // 1. payload is in the same chunk as a key. Since keys are always stored as flat,
             // payloads must also be stored as flat.
             // 2. payload is in flat chunk
-            columnSchema = std::make_unique<ColumnSchema>(false /* isUnFlat */, pos.dataChunkPos,
+            auto columnSchema = ColumnSchema(false /* isUnFlat */, pos.dataChunkPos,
                 LogicalTypeUtils::getRowLayoutSize(payload->dataType));
+            tableSchema.appendColumn(std::move(columnSchema));
         } else {
-            columnSchema = std::make_unique<ColumnSchema>(true /* isUnFlat */, pos.dataChunkPos,
+            auto columnSchema = ColumnSchema(true /* isUnFlat */, pos.dataChunkPos,
                 (uint32_t)sizeof(overflow_value_t));
+            tableSchema.appendColumn(std::move(columnSchema));
         }
-        tableSchema->appendColumn(std::move(columnSchema));
         payloadsPos.push_back(pos);
     }
-    auto hashValueColumn = std::make_unique<ColumnSchema>(false /* isUnFlat */,
-        INVALID_DATA_CHUNK_POS, LogicalTypeUtils::getRowLayoutSize(*LogicalType::HASH()));
-    tableSchema->appendColumn(std::move(hashValueColumn));
-    auto pointerColumn = std::make_unique<ColumnSchema>(false /* isUnFlat */,
-        INVALID_DATA_CHUNK_POS, LogicalTypeUtils::getRowLayoutSize(*LogicalType::INT64()));
-    tableSchema->appendColumn(std::move(pointerColumn));
+    auto hashValueColumn = ColumnSchema(false /* isUnFlat */, INVALID_DATA_CHUNK_POS,
+        LogicalTypeUtils::getRowLayoutSize(*LogicalType::HASH()));
+    tableSchema.appendColumn(std::move(hashValueColumn));
+    auto pointerColumn = ColumnSchema(false /* isUnFlat */, INVALID_DATA_CHUNK_POS,
+        LogicalTypeUtils::getRowLayoutSize(*LogicalType::INT64()));
+    tableSchema.appendColumn(std::move(pointerColumn));
     return std::make_unique<HashJoinBuildInfo>(std::move(keysPos), std::move(fStateTypes),
         std::move(payloadsPos), std::move(tableSchema));
 }
 
 std::unique_ptr<PhysicalOperator> PlanMapper::mapHashJoin(LogicalOperator* logicalOperator) {
     auto hashJoin = (LogicalHashJoin*)logicalOperator;
     auto outSchema = hashJoin->getSchema();
```

### sdist/kuzu-source/src/processor/map/map_order_by.cpp

```diff
@@ -19,31 +19,31 @@
     auto prevOperator = mapOperator(logicalOrderBy->getChild(0).get());
     auto paramsString = logicalOrderBy->getExpressionsForPrinting();
     auto keyExpressions = logicalOrderBy->getExpressionsToOrderBy();
     auto payloadExpressions = inSchema->getExpressionsInScope();
     std::vector<DataPos> payloadsPos;
     std::vector<std::unique_ptr<LogicalType>> payloadTypes;
     binder::expression_map<ft_col_idx_t> payloadToColIdx;
-    auto payloadSchema = std::make_unique<FactorizedTableSchema>();
+    auto payloadSchema = FactorizedTableSchema();
     auto mayContainUnFlatKey = inSchema->getNumGroups() == 1;
     for (auto i = 0u; i < payloadExpressions.size(); ++i) {
         auto expression = payloadExpressions[i];
         auto [dataChunkPos, vectorPos] = inSchema->getExpressionPos(*expression);
         payloadsPos.emplace_back(dataChunkPos, vectorPos);
         payloadTypes.push_back(expression->dataType.copy());
-        std::unique_ptr<ColumnSchema> columnSchema;
         if (!inSchema->getGroup(dataChunkPos)->isFlat() && !mayContainUnFlatKey) {
             // payload is unFlat and not in the same group as keys
-            columnSchema = std::make_unique<ColumnSchema>(true /* isUnFlat */, dataChunkPos,
-                sizeof(overflow_value_t));
+            auto columnSchema =
+                ColumnSchema(true /* isUnFlat */, dataChunkPos, sizeof(overflow_value_t));
+            payloadSchema.appendColumn(std::move(columnSchema));
         } else {
-            columnSchema = std::make_unique<ColumnSchema>(false /* isUnFlat */, dataChunkPos,
+            auto columnSchema = ColumnSchema(false /* isUnFlat */, dataChunkPos,
                 LogicalTypeUtils::getRowLayoutSize(expression->getDataType()));
+            payloadSchema.appendColumn(std::move(columnSchema));
         }
-        payloadSchema->appendColumn(std::move(columnSchema));
         payloadToColIdx.insert({expression, i});
     }
     std::vector<DataPos> keysPos;
     std::vector<std::unique_ptr<LogicalType>> keyTypes;
     std::vector<uint32_t> keyInPayloadPos;
     for (auto& expression : keyExpressions) {
         keysPos.emplace_back(inSchema->getExpressionPos(*expression));
```

### sdist/kuzu-source/src/processor/map/plan_mapper.cpp

```diff
@@ -198,18 +198,9 @@
     std::vector<DataPos> result;
     for (auto& expression : expressions) {
         result.emplace_back(getDataPos(*expression, schema));
     }
     return result;
 }
 
-std::shared_ptr<FactorizedTable> PlanMapper::getSingleStringColumnFTable() const {
-    auto ftTableSchema = std::make_unique<FactorizedTableSchema>();
-    ftTableSchema->appendColumn(
-        std::make_unique<ColumnSchema>(false /* flat */, 0 /* dataChunkPos */,
-            LogicalTypeUtils::getRowLayoutSize(LogicalType{LogicalTypeID::STRING})));
-    return std::make_shared<FactorizedTable>(clientContext->getMemoryManager(),
-        std::move(ftTableSchema));
-}
-
 } // namespace processor
 } // namespace kuzu
```

### sdist/kuzu-source/src/processor/operator/aggregate/aggregate_hash_table.cpp

```diff
@@ -9,15 +9,15 @@
 namespace kuzu {
 namespace processor {
 
 AggregateHashTable::AggregateHashTable(MemoryManager& memoryManager,
     std::vector<LogicalType> keyTypes, std::vector<LogicalType> payloadTypes,
     const std::vector<std::unique_ptr<AggregateFunction>>& aggregateFunctions,
     const std::vector<LogicalType>& distinctAggKeyTypes, uint64_t numEntriesToAllocate,
-    std::unique_ptr<FactorizedTableSchema> tableSchema)
+    FactorizedTableSchema tableSchema)
     : BaseHashTable{memoryManager, std::move(keyTypes)}, payloadTypes{std::move(payloadTypes)} {
     initializeFT(aggregateFunctions, std::move(tableSchema));
     initializeHashTable(numEntriesToAllocate);
     KU_ASSERT(aggregateFunctions.size() == distinctAggKeyTypes.size());
     for (auto i = 0u; i < this->aggregateFunctions.size(); ++i) {
         std::unique_ptr<AggregateHashTable> distinctHT;
         if (this->aggregateFunctions[i]->isDistinct) {
@@ -118,15 +118,15 @@
             aggregateStatesOffset += aggregateFunction->getAggregateStateSize();
         }
     }
 }
 
 void AggregateHashTable::initializeFT(
     const std::vector<std::unique_ptr<AggregateFunction>>& aggFuncs,
-    std::unique_ptr<FactorizedTableSchema> tableSchema) {
+    FactorizedTableSchema tableSchema) {
     aggStateColIdxInFT = keyTypes.size() + payloadTypes.size();
     for (auto& dataType : keyTypes) {
         numBytesForKeys += LogicalTypeUtils::getRowLayoutSize(dataType);
     }
     for (auto& dataType : payloadTypes) {
         numBytesForDependentKeys += LogicalTypeUtils::getRowLayoutSize(dataType);
     }
@@ -137,16 +137,16 @@
     for (auto i = 0u; i < aggFuncs.size(); i++) {
         auto& aggFunc = aggFuncs[i];
         aggregateFunctions.push_back(aggFunc->clone());
         updateAggFuncs.push_back(aggFunc->isFunctionDistinct() ?
                                      &AggregateHashTable::updateDistinctAggState :
                                      &AggregateHashTable::updateAggState);
     }
-    hashColIdxInFT = tableSchema->getNumColumns() - 1;
-    hashColOffsetInFT = tableSchema->getColOffset(hashColIdxInFT);
+    hashColIdxInFT = tableSchema.getNumColumns() - 1;
+    hashColOffsetInFT = tableSchema.getColOffset(hashColIdxInFT);
     factorizedTable = std::make_unique<FactorizedTable>(&memoryManager, std::move(tableSchema));
 }
 
 void AggregateHashTable::initializeHashTable(uint64_t numEntriesToAllocate) {
     auto numHashSlotsPerBlock = prevPowerOfTwo(HASH_BLOCK_SIZE / sizeof(HashSlot));
     setMaxNumHashSlots(nextPowerOfTwo(std::max(numHashSlotsPerBlock, numEntriesToAllocate)));
     initSlotConstant(numHashSlotsPerBlock);
@@ -743,32 +743,30 @@
     }
 }
 
 std::unique_ptr<AggregateHashTable> AggregateHashTableUtils::createDistinctHashTable(
     MemoryManager& memoryManager, const std::vector<LogicalType>& groupByKeyTypes,
     const LogicalType& distinctKeyType) {
     std::vector<LogicalType> hashKeyTypes(groupByKeyTypes.size() + 1);
-    auto tableSchema = std::make_unique<FactorizedTableSchema>();
+    auto tableSchema = FactorizedTableSchema();
     auto i = 0u;
     // Group by key columns
     for (; i < groupByKeyTypes.size(); i++) {
         hashKeyTypes[i] = groupByKeyTypes[i];
         auto size = LogicalTypeUtils::getRowLayoutSize(hashKeyTypes[i]);
-        auto columnSchema =
-            std::make_unique<ColumnSchema>(false /* isUnFlat */, 0 /* dataChunkPos */, size);
-        tableSchema->appendColumn(std::move(columnSchema));
+        auto columnSchema = ColumnSchema(false /* isUnFlat */, 0 /* groupID */, size);
+        tableSchema.appendColumn(std::move(columnSchema));
     }
     // Distinct key column
     hashKeyTypes[i] = distinctKeyType;
-    auto columnSchema = std::make_unique<ColumnSchema>(false /* isUnFlat */, 0 /* dataChunkPos */,
+    auto columnSchema = ColumnSchema(false /* isUnFlat */, 0 /* groupID */,
         LogicalTypeUtils::getRowLayoutSize(distinctKeyType));
-    tableSchema->appendColumn(std::move(columnSchema));
+    tableSchema.appendColumn(std::move(columnSchema));
     // Hash column
-    tableSchema->appendColumn(
-        std::make_unique<ColumnSchema>(false /* isUnFlat */, 0 /* dataChunkPos */, sizeof(hash_t)));
+    tableSchema.appendColumn(ColumnSchema(false /* isUnFlat */, 0 /* groupID */, sizeof(hash_t)));
     return std::make_unique<AggregateHashTable>(memoryManager, std::move(hashKeyTypes),
         std::vector<LogicalType>{} /* empty payload types */, 0 /* numEntriesToAllocate */,
         std::move(tableSchema));
 }
 
 } // namespace processor
 } // namespace kuzu
```

### sdist/kuzu-source/src/processor/operator/aggregate/hash_aggregate.cpp

```diff
@@ -48,22 +48,22 @@
         globalAggregateHashTable->getNumEntries() - currentOffset);
     currentOffset += range;
     return std::make_pair(startOffset, startOffset + range);
 }
 
 HashAggregateInfo::HashAggregateInfo(std::vector<DataPos> flatKeysPos,
     std::vector<DataPos> unFlatKeysPos, std::vector<DataPos> dependentKeysPos,
-    std::unique_ptr<FactorizedTableSchema> tableSchema, HashTableType hashTableType)
+    FactorizedTableSchema tableSchema, HashTableType hashTableType)
     : flatKeysPos{std::move(flatKeysPos)}, unFlatKeysPos{std::move(unFlatKeysPos)},
       dependentKeysPos{std::move(dependentKeysPos)}, tableSchema{std::move(tableSchema)},
       hashTableType{hashTableType} {}
 
 HashAggregateInfo::HashAggregateInfo(const HashAggregateInfo& other)
     : flatKeysPos{other.flatKeysPos}, unFlatKeysPos{other.unFlatKeysPos},
-      dependentKeysPos{other.dependentKeysPos}, tableSchema{other.tableSchema->copy()},
+      dependentKeysPos{other.dependentKeysPos}, tableSchema{other.tableSchema.copy()},
       hashTableType{other.hashTableType} {}
 
 void HashAggregateLocalState::init(ResultSet& resultSet, main::ClientContext* context,
     HashAggregateInfo& info,
     std::vector<std::unique_ptr<function::AggregateFunction>>& aggregateFunctions,
     std::vector<common::LogicalType> types) {
     std::vector<LogicalType> keyDataTypes;
```

### sdist/kuzu-source/src/processor/operator/hash_join/hash_join_build.cpp

```diff
@@ -24,15 +24,15 @@
     if (keyState == nullptr) {
         setKeyState(keyVectors[0]->state.get());
     }
     for (auto& pos : info->payloadsPos) {
         payloadVectors.push_back(resultSet->getValueVector(pos).get());
     }
     hashTable = std::make_unique<JoinHashTable>(*context->clientContext->getMemoryManager(),
-        std::move(keyTypes), info->tableSchema->copy());
+        std::move(keyTypes), info->tableSchema.copy());
 }
 
 void HashJoinBuild::setKeyState(common::DataChunkState* state) {
     if (keyState == nullptr) {
         keyState = state;
     } else {
         KU_ASSERT(keyState == state); // two pointers should be pointing to the same state
```

### sdist/kuzu-source/src/processor/operator/hash_join/join_hash_table.cpp

```diff
@@ -7,20 +7,20 @@
 using namespace kuzu::storage;
 using namespace kuzu::function;
 
 namespace kuzu {
 namespace processor {
 
 JoinHashTable::JoinHashTable(MemoryManager& memoryManager, logical_type_vec_t keyTypes,
-    std::unique_ptr<FactorizedTableSchema> tableSchema)
+    FactorizedTableSchema tableSchema)
     : BaseHashTable{memoryManager, std::move(keyTypes)} {
     auto numSlotsPerBlock = HASH_BLOCK_SIZE / sizeof(uint8_t*);
     initSlotConstant(numSlotsPerBlock);
     // Prev pointer is always the last column in the table.
-    prevPtrColOffset = tableSchema->getColOffset(tableSchema->getNumColumns() - PREV_PTR_COL_IDX);
+    prevPtrColOffset = tableSchema.getColOffset(tableSchema.getNumColumns() - PREV_PTR_COL_IDX);
     factorizedTable = std::make_unique<FactorizedTable>(&memoryManager, std::move(tableSchema));
     this->tableSchema = factorizedTable->getTableSchema();
 }
 
 static bool discardNullFromKeys(const std::vector<ValueVector*>& vectors) {
     bool hasNonNullKeys = true;
     for (auto& vector : vectors) {
```

### sdist/kuzu-source/src/processor/operator/order_by/sort_state.cpp

```diff
@@ -9,15 +9,15 @@
     auto encodedKeyBlockColOffset = 0ul;
     for (auto i = 0u; i < orderByDataInfo.keysPos.size(); ++i) {
         auto dataType = orderByDataInfo.keyTypes[i].get();
         if (PhysicalTypeID::STRING == dataType->getPhysicalType()) {
             // If this is a string column, we need to find the factorizedTable offset for this
             // column.
             auto ftColIdx = orderByDataInfo.keyInPayloadPos[i];
-            strKeyColsInfo.emplace_back(orderByDataInfo.payloadTableSchema->getColOffset(ftColIdx),
+            strKeyColsInfo.emplace_back(orderByDataInfo.payloadTableSchema.getColOffset(ftColIdx),
                 encodedKeyBlockColOffset, orderByDataInfo.isAscOrder[i]);
         }
         encodedKeyBlockColOffset += OrderByKeyEncoder::getEncodingSize(*dataType);
     }
     numBytesPerTuple = encodedKeyBlockColOffset + OrderByConstants::NUM_BYTES_FOR_PAYLOAD_IDX;
 }
 
@@ -51,15 +51,15 @@
     }
     return payloadTablesToReturn;
 }
 
 void SortLocalState::init(const OrderByDataInfo& orderByDataInfo, SortSharedState& sharedState,
     storage::MemoryManager* memoryManager) {
     auto [idx, table] =
-        sharedState.getLocalPayloadTable(*memoryManager, *orderByDataInfo.payloadTableSchema);
+        sharedState.getLocalPayloadTable(*memoryManager, orderByDataInfo.payloadTableSchema);
     globalIdx = idx;
     payloadTable = table;
     orderByKeyEncoder = std::make_unique<OrderByKeyEncoder>(orderByDataInfo, memoryManager,
         globalIdx, payloadTable->getNumTuplesPerBlock(), sharedState.getNumBytesPerTuple());
     radixSorter = std::make_unique<RadixSort>(memoryManager, *payloadTable, *orderByKeyEncoder,
         sharedState.getStrKeyColInfo());
 }
```

### sdist/kuzu-source/src/processor/operator/order_by/top_k.cpp

```diff
@@ -103,15 +103,15 @@
     auto payloadFlatState = common::DataChunkState::getSingleValueDataChunkState();
     auto lastPayloadUnflatState = std::make_shared<common::DataChunkState>();
     auto lastPayloadFlatState = common::DataChunkState::getSingleValueDataChunkState();
     for (auto i = 0u; i < orderByDataInfo->payloadTypes.size(); i++) {
         auto type = orderByDataInfo->payloadTypes[i].get();
         auto payloadVec = std::make_unique<common::ValueVector>(*type, memoryManager);
         auto lastPayloadVec = std::make_unique<common::ValueVector>(*type, memoryManager);
-        if (orderByDataInfo->payloadTableSchema->getColumn(i)->isFlat()) {
+        if (orderByDataInfo->payloadTableSchema.getColumn(i)->isFlat()) {
             payloadVec->setState(payloadFlatState);
             lastPayloadVec->setState(lastPayloadFlatState);
         } else {
             payloadVec->setState(payloadUnflatState);
             lastPayloadVec->setState(lastPayloadUnflatState);
         }
         payloadVecsToScan.push_back(payloadVec.get());
```

### sdist/kuzu-source/src/processor/operator/persistent/copy_rdf.cpp

```diff
@@ -1,11 +1,11 @@
 #include "processor/operator/persistent/copy_rdf.h"
 
 #include "common/string_format.h"
-#include "processor/result/factorized_table.h"
+#include "processor/result/factorized_table_util.h"
 
 namespace kuzu {
 namespace processor {
 
 void CopyRdf::finalize(ExecutionContext* context) {
     auto outputMsg = common::stringFormat("Done copy rdf.");
     FactorizedTableUtils::appendStringToTable(sharedState->fTable.get(), outputMsg,
```

### sdist/kuzu-source/src/processor/operator/persistent/copy_to_parquet.cpp

```diff
@@ -5,15 +5,15 @@
 
 using namespace kuzu::common;
 using namespace kuzu::storage;
 
 void CopyToParquetLocalState::init(CopyToInfo* info, storage::MemoryManager* mm,
     ResultSet* resultSet) {
     auto copyToInfo = info->constPtrCast<CopyToParquetInfo>();
-    ft = std::make_unique<FactorizedTable>(mm, copyToInfo->tableSchema->copy());
+    ft = std::make_unique<FactorizedTable>(mm, copyToInfo->tableSchema.copy());
     numTuplesInFT = 0;
     countingVec = nullptr;
     vectorsToAppend.reserve(info->dataPoses.size());
     countingVec = resultSet->getValueVector(copyToInfo->countingVecPos).get();
     for (auto& pos : info->dataPoses) {
         vectorsToAppend.push_back(resultSet->getValueVector(pos).get());
     }
```

### sdist/kuzu-source/src/processor/operator/persistent/node_batch_insert.cpp

```diff
@@ -5,14 +5,15 @@
 #include "common/string_format.h"
 #include "common/types/internal_id_t.h"
 #include "common/types/types.h"
 #include "function/table/scan_functions.h"
 #include "processor/execution_context.h"
 #include "processor/operator/persistent/index_builder.h"
 #include "processor/result/factorized_table.h"
+#include "processor/result/factorized_table_util.h"
 #include "storage/local_storage/local_node_table.h"
 #include "storage/store/chunked_node_group.h"
 #include "storage/store/node_table.h"
 
 using namespace kuzu::catalog;
 using namespace kuzu::common;
 using namespace kuzu::storage;
```

### sdist/kuzu-source/src/processor/operator/persistent/rel_batch_insert.cpp

```diff
@@ -1,13 +1,13 @@
 #include "processor/operator/persistent/rel_batch_insert.h"
 
 #include "common/exception/copy.h"
 #include "common/exception/message.h"
 #include "common/string_format.h"
-#include "processor/result/factorized_table.h"
+#include "processor/result/factorized_table_util.h"
 #include "storage/local_storage/local_rel_table.h"
 #include "storage/store/column_chunk.h"
 #include "storage/store/rel_table.h"
 
 using namespace kuzu::common;
 using namespace kuzu::storage;
```

### sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/parquet_writer.cpp

```diff
@@ -180,15 +180,15 @@
     row_group.__isset.file_offset = true;
 
     auto& states = result.states;
     // iterate over each of the columns of the chunk collection and write them
     KU_ASSERT(ft.getTableSchema()->getNumColumns() == columnWriters.size());
     std::vector<std::unique_ptr<ColumnWriterState>> writerStates;
     std::unique_ptr<DataChunk> unflatDataChunkToRead =
-        std::make_unique<DataChunk>(ft.getTableSchema()->getNumUnflatColumns());
+        std::make_unique<DataChunk>(ft.getTableSchema()->getNumUnFlatColumns());
     std::unique_ptr<DataChunk> flatDataChunkToRead = std::make_unique<DataChunk>(
         ft.getTableSchema()->getNumFlatColumns(), DataChunkState::getSingleValueDataChunkState());
     std::vector<ValueVector*> vectorsToRead;
     vectorsToRead.reserve(columnWriters.size());
     auto numFlatVectors = 0;
     for (auto i = 0u; i < columnWriters.size(); i++) {
         writerStates.emplace_back(columnWriters[i]->initializeWriteState(row_group));
@@ -262,15 +262,15 @@
     fileMetaData.row_groups.push_back(parquetRowGroup);
     fileMetaData.num_rows += parquetRowGroup.num_rows;
 }
 
 void ParquetWriter::readFromFT(FactorizedTable& ft, std::vector<ValueVector*> vectorsToRead,
     uint64_t& numTuplesRead) {
     auto numTuplesToRead =
-        ft.getTableSchema()->getNumUnflatColumns() != 0 ?
+        ft.getTableSchema()->getNumUnFlatColumns() != 0 ?
             1 :
             std::min<uint64_t>(ft.getNumTuples() - numTuplesRead, DEFAULT_VECTOR_CAPACITY);
     ft.scan(vectorsToRead, numTuplesRead, numTuplesToRead);
     numTuplesRead += numTuplesToRead;
 }
 
 void ParquetWriter::finalize() {
```

### sdist/kuzu-source/src/processor/operator/result_collector.cpp

```diff
@@ -17,15 +17,15 @@
         markVector = std::make_unique<ValueVector>(*LogicalType::BOOL(),
             context->clientContext->getMemoryManager());
         markVector->state = DataChunkState::getSingleValueDataChunkState();
         markVector->setValue<bool>(0, true);
         payloadAndMarkVectors.push_back(markVector.get());
     }
     localTable = std::make_unique<FactorizedTable>(context->clientContext->getMemoryManager(),
-        info->tableSchema->copy());
+        info->tableSchema.copy());
 }
 
 void ResultCollector::executeInternal(ExecutionContext* context) {
     while (children[0]->getNextTuple(context)) {
         if (!payloadVectors.empty()) {
             for (auto i = 0u; i < resultSet->multiplicity; i++) {
                 localTable->append(payloadAndMarkVectors);
```

### sdist/kuzu-source/src/processor/result/CMakeLists.txt

```diff
@@ -1,11 +1,13 @@
 add_library(kuzu_processor_result
         OBJECT
         base_hash_table.cpp
         factorized_table.cpp
+        factorized_table_schema.cpp
+        factorized_table_util.cpp
         flat_tuple.cpp
         mark_hash_table.cpp
         result_set.cpp
         result_set_descriptor.cpp
         )
 
 set(ALL_OBJECT_FILES
```

### sdist/kuzu-source/src/processor/result/factorized_table.cpp

```diff
@@ -1,76 +1,20 @@
 #include "processor/result/factorized_table.h"
 
 #include "common/assert.h"
-#include "common/data_chunk/data_chunk_state.h"
 #include "common/exception/runtime.h"
 #include "common/null_buffer.h"
 #include "common/vector/value_vector.h"
 
 using namespace kuzu::common;
 using namespace kuzu::storage;
 
 namespace kuzu {
 namespace processor {
 
-ColumnSchema::ColumnSchema(const ColumnSchema& other) {
-    isUnflat = other.isUnflat;
-    dataChunkPos = other.dataChunkPos;
-    numBytes = other.numBytes;
-    mayContainNulls = other.mayContainNulls;
-}
-
-FactorizedTableSchema::FactorizedTableSchema(const FactorizedTableSchema& other) {
-    for (auto& column : other.columns) {
-        appendColumn(std::make_unique<ColumnSchema>(*column));
-    }
-}
-
-void FactorizedTableSchema::appendColumn(std::unique_ptr<ColumnSchema> column) {
-    numBytesForDataPerTuple += column->getNumBytes();
-    columns.push_back(std::move(column));
-    colOffsets.push_back(
-        colOffsets.empty() ? 0 : colOffsets.back() + getColumn(columns.size() - 2)->getNumBytes());
-    numBytesForNullMapPerTuple = NullBuffer::getNumBytesForNullValues(getNumColumns());
-    numBytesPerTuple = numBytesForDataPerTuple + numBytesForNullMapPerTuple;
-}
-
-bool FactorizedTableSchema::operator==(const FactorizedTableSchema& other) const {
-    if (columns.size() != other.columns.size()) {
-        return false;
-    }
-    for (auto i = 0u; i < columns.size(); i++) {
-        if (*columns[i] != *other.columns[i]) {
-            return false;
-        }
-    }
-    return numBytesForDataPerTuple == other.numBytesForDataPerTuple && numBytesForNullMapPerTuple &&
-           other.numBytesForNullMapPerTuple;
-}
-
-uint64_t FactorizedTableSchema::getNumFlatColumns() const {
-    auto numFlatColumns = 0u;
-    for (auto& column : columns) {
-        if (column->isFlat()) {
-            numFlatColumns++;
-        }
-    }
-    return numFlatColumns;
-}
-
-uint64_t FactorizedTableSchema::getNumUnflatColumns() const {
-    auto numUnflatColumns = 0u;
-    for (auto& column : columns) {
-        if (!column->isFlat()) {
-            numUnflatColumns++;
-        }
-    }
-    return numUnflatColumns;
-}
-
 void DataBlock::copyTuples(DataBlock* blockToCopyFrom, ft_tuple_idx_t tupleIdxToCopyFrom,
     DataBlock* blockToCopyInto, ft_tuple_idx_t tupleIdxToCopyTo, uint32_t numTuplesToCopy,
     uint32_t numBytesPerTuple) {
     for (auto i = 0u; i < numTuplesToCopy; i++) {
         memcpy(blockToCopyInto->getData() + (tupleIdxToCopyTo * numBytesPerTuple),
             blockToCopyFrom->getData() + (tupleIdxToCopyFrom * numBytesPerTuple), numBytesPerTuple);
         tupleIdxToCopyFrom++;
@@ -103,20 +47,19 @@
         oldLastBlock->resetNumTuplesAndFreeSize();
         DataBlock::copyTuples(oldLastBlock.get(), tupleIdxInOldLastBlock, oldLastBlock.get(), 0,
             numTuplesLeftForNewBlock, numBytesPerTuple);
         blocks.push_back(std::move(oldLastBlock));
     }
 }
 
-FactorizedTable::FactorizedTable(MemoryManager* memoryManager,
-    std::unique_ptr<FactorizedTableSchema> tableSchema)
+FactorizedTable::FactorizedTable(MemoryManager* memoryManager, FactorizedTableSchema tableSchema)
     : memoryManager{memoryManager}, tableSchema{std::move(tableSchema)}, numTuples{0} {
-    if (!this->tableSchema->isEmpty()) {
+    if (!this->tableSchema.isEmpty()) {
         inMemOverflowBuffer = std::make_unique<InMemOverflowBuffer>(memoryManager);
-        auto numBytesPerTuple = this->tableSchema->getNumBytesPerTuple();
+        auto numBytesPerTuple = this->tableSchema.getNumBytesPerTuple();
         if (numBytesPerTuple > BufferPoolConstants::PAGE_256KB_SIZE) {
             // I realize it's unlikely to trigger this case because the fixed size part for
             // a column is always small. A quick calculation, assume average column size is 16 bytes
             // then we need more than 16K column to test this. I choose to throw exception until
             // we encounter a use case.
             throw RuntimeException(
                 "Trying to allocate for a large tuple of size greater than 256KB. "
@@ -141,15 +84,15 @@
         }
         KU_ASSERT(numAppendedTuples == numTuplesToAppend);
     }
     numTuples += numTuplesToAppend;
 }
 
 uint8_t* FactorizedTable::appendEmptyTuple() {
-    auto numBytesPerTuple = tableSchema->getNumBytesPerTuple();
+    auto numBytesPerTuple = tableSchema.getNumBytesPerTuple();
     if (flatTupleBlockCollection->needAllocation(numBytesPerTuple)) {
         auto newBlock = std::make_unique<DataBlock>(memoryManager, flatTupleBlockSize);
         flatTupleBlockCollection->append(std::move(newBlock));
     }
     auto block = flatTupleBlockCollection->getLastBlock();
     uint8_t* tuplePtr = block->getWritableData();
     block->freeSize -= numBytesPerTuple;
@@ -174,15 +117,15 @@
     uint64_t numTuplesToRead) const {
     KU_ASSERT(vectors.size() == colIdxesToScan.size());
     for (auto i = 0u; i < colIdxesToScan.size(); i++) {
         auto vector = vectors[i];
         // TODO(Xiyang/Ziyi): we should set up a rule about when to reset. Should it be in operator?
         vector->resetAuxiliaryBuffer();
         ft_col_idx_t colIdx = colIdxesToScan[i];
-        if (tableSchema->getColumn(colIdx)->isFlat()) {
+        if (tableSchema.getColumn(colIdx)->isFlat()) {
             KU_ASSERT(!(vector->state->isFlat() && numTuplesToRead > 1));
             readFlatCol(tuplesToRead + startPos, colIdx, *vector, numTuplesToRead);
         } else {
             // If the caller wants to read an unflat column from factorizedTable, the vector
             // must be unflat and the numTuplesToScan should be 1.
             KU_ASSERT(!vector->state->isFlat() && numTuplesToRead == 1);
             readUnflatCol(tuplesToRead + startPos, colIdx, *vector);
@@ -191,15 +134,15 @@
 }
 
 void FactorizedTable::lookup(std::vector<ValueVector*>& vectors, const SelectionVector* selVector,
     std::vector<ft_col_idx_t>& colIdxesToScan, uint8_t* tupleToRead) const {
     KU_ASSERT(vectors.size() == colIdxesToScan.size());
     for (auto i = 0u; i < colIdxesToScan.size(); i++) {
         ft_col_idx_t colIdx = colIdxesToScan[i];
-        if (tableSchema->getColumn(colIdx)->isFlat()) {
+        if (tableSchema.getColumn(colIdx)->isFlat()) {
             readFlatCol(&tupleToRead, colIdx, *vectors[i], 1);
         } else {
             readUnflatCol(tupleToRead, *selVector, colIdx, *vectors[i]);
         }
     }
 }
 
@@ -212,143 +155,138 @@
     for (auto i = 0u; i < numTuplesToRead; i++) {
         tuplesToRead[i] = getTuple(tupleIdxesToRead[i + startPos]);
     }
     lookup(vectors, colIdxesToScan, tuplesToRead.get(), 0 /* startPos */, numTuplesToRead);
 }
 
 void FactorizedTable::mergeMayContainNulls(FactorizedTable& other) {
-    for (auto i = 0u; i < other.tableSchema->getNumColumns(); i++) {
+    for (auto i = 0u; i < other.tableSchema.getNumColumns(); i++) {
         if (!other.hasNoNullGuarantee(i)) {
-            tableSchema->setMayContainsNullsToTrue(i);
+            tableSchema.setMayContainsNullsToTrue(i);
         }
     }
 }
 
 void FactorizedTable::merge(FactorizedTable& other) {
-    KU_ASSERT(*tableSchema == *other.tableSchema);
+    KU_ASSERT(tableSchema == other.tableSchema);
     if (other.numTuples == 0) {
         return;
     }
     mergeMayContainNulls(other);
     unFlatTupleBlockCollection->append(std::move(other.unFlatTupleBlockCollection));
     flatTupleBlockCollection->merge(*other.flatTupleBlockCollection);
     inMemOverflowBuffer->merge(*other.inMemOverflowBuffer);
     numTuples += other.numTuples;
 }
 
 bool FactorizedTable::hasUnflatCol() const {
-    std::vector<ft_col_idx_t> colIdxes(tableSchema->getNumColumns());
+    std::vector<ft_col_idx_t> colIdxes(tableSchema.getNumColumns());
     iota(colIdxes.begin(), colIdxes.end(), 0);
     return hasUnflatCol(colIdxes);
 }
 
 uint64_t FactorizedTable::getTotalNumFlatTuples() const {
     auto totalNumFlatTuples = 0ul;
     for (auto i = 0u; i < getNumTuples(); i++) {
         totalNumFlatTuples += getNumFlatTuples(i);
     }
     return totalNumFlatTuples;
 }
 
 uint64_t FactorizedTable::getNumFlatTuples(ft_tuple_idx_t tupleIdx) const {
-    std::unordered_map<uint32_t, bool> calculatedDataChunkPoses;
+    std::unordered_map<uint32_t, bool> calculatedGroups;
     uint64_t numFlatTuples = 1;
     auto tupleBuffer = getTuple(tupleIdx);
-    for (auto i = 0u; i < tableSchema->getNumColumns(); i++) {
-        auto column = tableSchema->getColumn(i);
-        if (!calculatedDataChunkPoses.contains(column->getDataChunkPos())) {
-            calculatedDataChunkPoses[column->getDataChunkPos()] = true;
+    for (auto i = 0u; i < tableSchema.getNumColumns(); i++) {
+        auto column = tableSchema.getColumn(i);
+        auto groupID = column->getGroupID();
+        if (!calculatedGroups.contains(groupID)) {
+            calculatedGroups[groupID] = true;
             numFlatTuples *= column->isFlat() ? 1 : ((overflow_value_t*)tupleBuffer)->numElements;
         }
         tupleBuffer += column->getNumBytes();
     }
     return numFlatTuples;
 }
 
 uint8_t* FactorizedTable::getTuple(ft_tuple_idx_t tupleIdx) const {
     KU_ASSERT(tupleIdx < numTuples);
     auto [blockIdx, tupleIdxInBlock] = getBlockIdxAndTupleIdxInBlock(tupleIdx);
     return flatTupleBlockCollection->getBlock(blockIdx)->getData() +
-           tupleIdxInBlock * tableSchema->getNumBytesPerTuple();
+           tupleIdxInBlock * tableSchema.getNumBytesPerTuple();
 }
 
 void FactorizedTable::updateFlatCell(uint8_t* tuplePtr, ft_col_idx_t colIdx,
     ValueVector* valueVector, uint32_t pos) {
-    auto nullBuffer = tuplePtr + tableSchema->getNullMapOffset();
+    auto nullBuffer = tuplePtr + tableSchema.getNullMapOffset();
     if (valueVector->isNull(pos)) {
         setNonOverflowColNull(nullBuffer, colIdx);
     } else {
-        valueVector->copyToRowData(pos, tuplePtr + tableSchema->getColOffset(colIdx),
+        valueVector->copyToRowData(pos, tuplePtr + tableSchema.getColOffset(colIdx),
             inMemOverflowBuffer.get());
         NullBuffer::setNoNull(nullBuffer, colIdx);
     }
 }
 
 bool FactorizedTable::isOverflowColNull(const uint8_t* nullBuffer, ft_tuple_idx_t tupleIdx,
     ft_col_idx_t colIdx) const {
-    KU_ASSERT(colIdx < tableSchema->getNumColumns());
-    if (tableSchema->getColumn(colIdx)->hasNoNullGuarantee()) {
+    KU_ASSERT(colIdx < tableSchema.getNumColumns());
+    if (tableSchema.getColumn(colIdx)->hasNoNullGuarantee()) {
         return false;
     }
     return NullBuffer::isNull(nullBuffer, tupleIdx);
 }
 
 bool FactorizedTable::isNonOverflowColNull(const uint8_t* nullBuffer, ft_col_idx_t colIdx) const {
-    KU_ASSERT(colIdx < tableSchema->getNumColumns());
-    if (tableSchema->getColumn(colIdx)->hasNoNullGuarantee()) {
+    KU_ASSERT(colIdx < tableSchema.getNumColumns());
+    if (tableSchema.getColumn(colIdx)->hasNoNullGuarantee()) {
         return false;
     }
     return NullBuffer::isNull(nullBuffer, colIdx);
 }
 
 void FactorizedTable::setNonOverflowColNull(uint8_t* nullBuffer, ft_col_idx_t colIdx) {
     NullBuffer::setNull(nullBuffer, colIdx);
-    tableSchema->setMayContainsNullsToTrue(colIdx);
+    tableSchema.setMayContainsNullsToTrue(colIdx);
 }
 
 void FactorizedTable::clear() {
     numTuples = 0;
     flatTupleBlockCollection = std::make_unique<DataBlockCollection>(
-        tableSchema->getNumBytesPerTuple(), numFlatTuplesPerBlock);
+        tableSchema.getNumBytesPerTuple(), numFlatTuplesPerBlock);
     unFlatTupleBlockCollection = std::make_unique<DataBlockCollection>();
     inMemOverflowBuffer->resetBuffer();
 }
 
 void FactorizedTable::setOverflowColNull(uint8_t* nullBuffer, ft_col_idx_t colIdx,
     ft_tuple_idx_t tupleIdx) {
     NullBuffer::setNull(nullBuffer, tupleIdx);
-    tableSchema->setMayContainsNullsToTrue(colIdx);
+    tableSchema.setMayContainsNullsToTrue(colIdx);
 }
 
 // TODO(Guodong): change this function to not use dataChunkPos in ColumnSchema.
 uint64_t FactorizedTable::computeNumTuplesToAppend(
     const std::vector<ValueVector*>& vectorsToAppend) const {
     KU_ASSERT(!vectorsToAppend.empty());
-    auto unflatDataChunkPos = -1ul;
     auto numTuplesToAppend = 1ul;
     for (auto i = 0u; i < vectorsToAppend.size(); i++) {
         // If the caller tries to append an unflat vector to a flat column in the
         // factorizedTable, the factorizedTable needs to flatten that vector.
-        if (tableSchema->getColumn(i)->isFlat() && !vectorsToAppend[i]->state->isFlat()) {
-            // The caller is not allowed to append multiple unflat columns from different
+        if (tableSchema.getColumn(i)->isFlat() && !vectorsToAppend[i]->state->isFlat()) {
+            // The caller is not allowed to append multiple unFlat columns from different
             // datachunks to multiple flat columns in the factorizedTable.
-            if (!tableSchema->getColumn(i)->isFlat()) {
-                KU_ASSERT(unflatDataChunkPos == (uint64_t)-1 ||
-                          tableSchema->getColumn(i)->getDataChunkPos() != unflatDataChunkPos);
-                unflatDataChunkPos = tableSchema->getColumn(i)->getDataChunkPos();
-            }
             numTuplesToAppend = vectorsToAppend[i]->state->getSelVector().getSelSize();
         }
     }
     return numTuplesToAppend;
 }
 
 std::vector<BlockAppendingInfo> FactorizedTable::allocateFlatTupleBlocks(
     uint64_t numTuplesToAppend) {
-    auto numBytesPerTuple = tableSchema->getNumBytesPerTuple();
+    auto numBytesPerTuple = tableSchema.getNumBytesPerTuple();
     std::vector<BlockAppendingInfo> appendingInfos;
     while (numTuplesToAppend > 0) {
         if (flatTupleBlockCollection->needAllocation(numBytesPerTuple)) {
             auto newBlock = std::make_unique<DataBlock>(memoryManager, flatTupleBlockSize);
             flatTupleBlockCollection->append(std::move(newBlock));
         }
         auto block = flatTupleBlockCollection->getLastBlock();
@@ -386,88 +324,88 @@
     lastBlock->freeSize -= numBytes;
     return lastBlock->getData();
 }
 
 void FactorizedTable::copyFlatVectorToFlatColumn(const ValueVector& vector,
     const BlockAppendingInfo& blockAppendInfo, ft_col_idx_t colIdx) {
     auto valuePositionInVectorToAppend = vector.state->getSelVector()[0];
-    auto colOffsetInDataBlock = tableSchema->getColOffset(colIdx);
+    auto colOffsetInDataBlock = tableSchema.getColOffset(colIdx);
     auto dstDataPtr = blockAppendInfo.data;
     for (auto i = 0u; i < blockAppendInfo.numTuplesToAppend; i++) {
         if (vector.isNull(valuePositionInVectorToAppend)) {
-            setNonOverflowColNull(dstDataPtr + tableSchema->getNullMapOffset(), colIdx);
+            setNonOverflowColNull(dstDataPtr + tableSchema.getNullMapOffset(), colIdx);
         } else {
             vector.copyToRowData(valuePositionInVectorToAppend, dstDataPtr + colOffsetInDataBlock,
                 inMemOverflowBuffer.get());
         }
-        dstDataPtr += tableSchema->getNumBytesPerTuple();
+        dstDataPtr += tableSchema.getNumBytesPerTuple();
     }
 }
 
 void FactorizedTable::copyUnflatVectorToFlatColumn(const ValueVector& vector,
     const BlockAppendingInfo& blockAppendInfo, uint64_t numAppendedTuples, ft_col_idx_t colIdx) {
-    auto byteOffsetOfColumnInTuple = tableSchema->getColOffset(colIdx);
+    auto byteOffsetOfColumnInTuple = tableSchema.getColOffset(colIdx);
     auto dstTuple = blockAppendInfo.data;
     if (vector.state->getSelVector().isUnfiltered()) {
         if (vector.hasNoNullsGuarantee()) {
             for (auto i = 0u; i < blockAppendInfo.numTuplesToAppend; i++) {
                 vector.copyToRowData(numAppendedTuples + i, dstTuple + byteOffsetOfColumnInTuple,
                     inMemOverflowBuffer.get());
-                dstTuple += tableSchema->getNumBytesPerTuple();
+                dstTuple += tableSchema.getNumBytesPerTuple();
             }
         } else {
             for (auto i = 0u; i < blockAppendInfo.numTuplesToAppend; i++) {
                 if (vector.isNull(numAppendedTuples + i)) {
-                    setNonOverflowColNull(dstTuple + tableSchema->getNullMapOffset(), colIdx);
+                    setNonOverflowColNull(dstTuple + tableSchema.getNullMapOffset(), colIdx);
                 } else {
                     vector.copyToRowData(numAppendedTuples + i,
                         dstTuple + byteOffsetOfColumnInTuple, inMemOverflowBuffer.get());
                 }
-                dstTuple += tableSchema->getNumBytesPerTuple();
+                dstTuple += tableSchema.getNumBytesPerTuple();
             }
         }
     } else {
         if (vector.hasNoNullsGuarantee()) {
             for (auto i = 0u; i < blockAppendInfo.numTuplesToAppend; i++) {
                 vector.copyToRowData(vector.state->getSelVector()[numAppendedTuples + i],
                     dstTuple + byteOffsetOfColumnInTuple, inMemOverflowBuffer.get());
-                dstTuple += tableSchema->getNumBytesPerTuple();
+                dstTuple += tableSchema.getNumBytesPerTuple();
             }
         } else {
             for (auto i = 0u; i < blockAppendInfo.numTuplesToAppend; i++) {
                 auto pos = vector.state->getSelVector()[numAppendedTuples + i];
                 if (vector.isNull(pos)) {
-                    setNonOverflowColNull(dstTuple + tableSchema->getNullMapOffset(), colIdx);
+                    setNonOverflowColNull(dstTuple + tableSchema.getNullMapOffset(), colIdx);
                 } else {
                     vector.copyToRowData(pos, dstTuple + byteOffsetOfColumnInTuple,
                         inMemOverflowBuffer.get());
                 }
-                dstTuple += tableSchema->getNumBytesPerTuple();
+                dstTuple += tableSchema.getNumBytesPerTuple();
             }
         }
     }
 }
 
 // For an unflat column, only an unflat vector is allowed to copy from, for the column, we only
 // store an overflow_value_t, which contains a pointer to the overflow dataBlock in the
 // factorizedTable. NullMasks are stored inside the overflow buffer.
 void FactorizedTable::copyVectorToUnflatColumn(const ValueVector& vector,
     const BlockAppendingInfo& blockAppendInfo, ft_col_idx_t colIdx) {
     KU_ASSERT(!vector.state->isFlat());
     auto unflatTupleValue = appendVectorToUnflatTupleBlocks(vector, colIdx);
-    auto blockPtr = blockAppendInfo.data + tableSchema->getColOffset(colIdx);
+    auto blockPtr = blockAppendInfo.data + tableSchema.getColOffset(colIdx);
     for (auto i = 0u; i < blockAppendInfo.numTuplesToAppend; i++) {
         memcpy(blockPtr, (uint8_t*)&unflatTupleValue, sizeof(overflow_value_t));
-        blockPtr += tableSchema->getNumBytesPerTuple();
+        blockPtr += tableSchema.getNumBytesPerTuple();
     }
 }
 
 void FactorizedTable::copyVectorToColumn(const ValueVector& vector,
     const BlockAppendingInfo& blockAppendInfo, uint64_t numAppendedTuples, ft_col_idx_t colIdx) {
-    if (tableSchema->getColumn(colIdx)->isFlat()) {
+    if (tableSchema.getColumn(colIdx)->isFlat()) {
         copyVectorToFlatColumn(vector, blockAppendInfo, numAppendedTuples, colIdx);
     } else {
         copyVectorToUnflatColumn(vector, blockAppendInfo, colIdx);
     }
 }
 
 overflow_value_t FactorizedTable::appendVectorToUnflatTupleBlocks(const ValueVector& vector,
@@ -519,15 +457,15 @@
     }
     return overflow_value_t{numFlatTuplesInVector, overflowBlockBuffer};
 }
 
 void FactorizedTable::readUnflatCol(uint8_t** tuplesToRead, ft_col_idx_t colIdx,
     ValueVector& vector) const {
     auto overflowColValue =
-        *(overflow_value_t*)(tuplesToRead[0] + tableSchema->getColOffset(colIdx));
+        *(overflow_value_t*)(tuplesToRead[0] + tableSchema.getColOffset(colIdx));
     KU_ASSERT(vector.state->getSelVector().isUnfiltered());
     auto numBytesPerValue = LogicalTypeUtils::getRowLayoutSize(vector.dataType);
     if (hasNoNullGuarantee(colIdx)) {
         vector.setAllNonNull();
         auto val = overflowColValue.value;
         for (auto i = 0u; i < overflowColValue.numElements; i++) {
             vector.copyFromRowData(i, val);
@@ -548,16 +486,15 @@
         }
     }
     vector.state->getSelVectorUnsafe().setSelSize(overflowColValue.numElements);
 }
 
 void FactorizedTable::readUnflatCol(const uint8_t* tupleToRead, const SelectionVector& selVector,
     ft_col_idx_t colIdx, ValueVector& vector) const {
-    auto vectorOverflowValue =
-        *(overflow_value_t*)(tupleToRead + tableSchema->getColOffset(colIdx));
+    auto vectorOverflowValue = *(overflow_value_t*)(tupleToRead + tableSchema.getColOffset(colIdx));
     KU_ASSERT(vector.state->getSelVector().isUnfiltered());
     if (hasNoNullGuarantee(colIdx)) {
         vector.setAllNonNull();
         auto val = vectorOverflowValue.value;
         for (auto i = 0u; i < vectorOverflowValue.numElements; i++) {
             auto pos = selVector[i];
             vector.copyFromRowData(i, val + (pos * vector.getNumBytesPerValue()));
@@ -577,19 +514,19 @@
         }
     }
     vector.state->getSelVectorUnsafe().setSelSize(selVector.getSelSize());
 }
 
 void FactorizedTable::readFlatColToFlatVector(uint8_t* tupleToRead, ft_col_idx_t colIdx,
     ValueVector& vector, sel_t pos) const {
-    if (isNonOverflowColNull(tupleToRead + tableSchema->getNullMapOffset(), colIdx)) {
+    if (isNonOverflowColNull(tupleToRead + tableSchema.getNullMapOffset(), colIdx)) {
         vector.setNull(pos, true);
     } else {
         vector.setNull(pos, false);
-        vector.copyFromRowData(pos, tupleToRead + tableSchema->getColOffset(colIdx));
+        vector.copyFromRowData(pos, tupleToRead + tableSchema.getColOffset(colIdx));
     }
 }
 
 void FactorizedTable::readFlatCol(uint8_t** tuplesToRead, ft_col_idx_t colIdx, ValueVector& vector,
     uint64_t numTuplesToRead) const {
     if (vector.state->isFlat()) {
         auto pos = vector.state->getSelVector()[0];
@@ -602,62 +539,37 @@
 void FactorizedTable::readFlatColToUnflatVector(uint8_t** tuplesToRead, ft_col_idx_t colIdx,
     ValueVector& vector, uint64_t numTuplesToRead) const {
     vector.state->getSelVectorUnsafe().setSelSize(numTuplesToRead);
     if (hasNoNullGuarantee(colIdx)) {
         vector.setAllNonNull();
         for (auto i = 0u; i < numTuplesToRead; i++) {
             auto positionInVectorToWrite = vector.state->getSelVector()[i];
-            auto srcData = tuplesToRead[i] + tableSchema->getColOffset(colIdx);
+            auto srcData = tuplesToRead[i] + tableSchema.getColOffset(colIdx);
             vector.copyFromRowData(positionInVectorToWrite, srcData);
         }
     } else {
         for (auto i = 0u; i < numTuplesToRead; i++) {
             auto positionInVectorToWrite = vector.state->getSelVector()[i];
             auto dataBuffer = tuplesToRead[i];
-            if (isNonOverflowColNull(dataBuffer + tableSchema->getNullMapOffset(), colIdx)) {
+            if (isNonOverflowColNull(dataBuffer + tableSchema.getNullMapOffset(), colIdx)) {
                 vector.setNull(positionInVectorToWrite, true);
             } else {
                 vector.setNull(positionInVectorToWrite, false);
                 vector.copyFromRowData(positionInVectorToWrite,
-                    dataBuffer + tableSchema->getColOffset(colIdx));
+                    dataBuffer + tableSchema.getColOffset(colIdx));
             }
         }
     }
 }
 
-void FactorizedTableUtils::appendStringToTable(FactorizedTable* factorizedTable,
-    std::string& outputMsg, MemoryManager* memoryManager) {
-    auto outputMsgVector = std::make_shared<ValueVector>(LogicalTypeID::STRING, memoryManager);
-    outputMsgVector->state = DataChunkState::getSingleValueDataChunkState();
-    auto outputKUStr = ku_string_t();
-    outputKUStr.overflowPtr =
-        reinterpret_cast<uint64_t>(StringVector::getInMemOverflowBuffer(outputMsgVector.get())
-                                       ->allocateSpace(outputMsg.length()));
-    outputKUStr.set(outputMsg);
-    outputMsgVector->setValue(0, outputKUStr);
-    factorizedTable->append(std::vector<ValueVector*>{outputMsgVector.get()});
-}
-
-std::shared_ptr<FactorizedTable> FactorizedTableUtils::getFactorizedTableForOutputMsg(
-    std::string& outputMsg, storage::MemoryManager* memoryManager) {
-    auto ftTableSchema = std::make_unique<FactorizedTableSchema>();
-    ftTableSchema->appendColumn(
-        std::make_unique<ColumnSchema>(false /* flat */, 0 /* dataChunkPos */,
-            LogicalTypeUtils::getRowLayoutSize(LogicalType{LogicalTypeID::STRING})));
-    auto factorizedTable =
-        std::make_shared<FactorizedTable>(memoryManager, std::move(ftTableSchema));
-    appendStringToTable(factorizedTable.get(), outputMsg, memoryManager);
-    return factorizedTable;
-}
-
 FlatTupleIterator::FlatTupleIterator(FactorizedTable& factorizedTable, std::vector<Value*> values)
     : factorizedTable{factorizedTable}, numFlatTuples{0}, nextFlatTupleIdx{0}, nextTupleIdx{1},
       values{std::move(values)} {
     resetState();
-    KU_ASSERT(this->values.size() == factorizedTable.tableSchema->getNumColumns());
+    KU_ASSERT(this->values.size() == factorizedTable.tableSchema.getNumColumns());
 }
 
 void FlatTupleIterator::getNextFlatTuple() {
     // Go to the next tuple if we have iterated all the flat tuples of the current tuple.
     if (nextFlatTupleIdx >= numFlatTuples) {
         currentTupleBuffer = factorizedTable.getTuple(nextTupleIdx);
         numFlatTuples = factorizedTable.getNumFlatTuples(nextTupleIdx);
@@ -688,24 +600,22 @@
         updateInvalidEntriesInFlatTuplePositionsInDataChunk();
     }
 }
 
 void FlatTupleIterator::readUnflatColToFlatTuple(ft_col_idx_t colIdx, uint8_t* valueBuffer) {
     auto overflowValue =
         (overflow_value_t*)(valueBuffer + factorizedTable.getTableSchema()->getColOffset(colIdx));
-    auto columnInFactorizedTable = factorizedTable.getTableSchema()->getColumn(colIdx);
+    auto groupID = factorizedTable.getTableSchema()->getColumn(colIdx)->getGroupID();
     auto tupleSizeInOverflowBuffer =
         LogicalTypeUtils::getRowLayoutSize(*values[colIdx]->getDataType());
-    valueBuffer =
-        overflowValue->value +
-        tupleSizeInOverflowBuffer *
-            flatTuplePositionsInDataChunk[columnInFactorizedTable->getDataChunkPos()].first;
+    valueBuffer = overflowValue->value +
+                  tupleSizeInOverflowBuffer * flatTuplePositionsInDataChunk[groupID].first;
     auto isNull = factorizedTable.isOverflowColNull(
         overflowValue->value + tupleSizeInOverflowBuffer * overflowValue->numElements,
-        flatTuplePositionsInDataChunk[columnInFactorizedTable->getDataChunkPos()].first, colIdx);
+        flatTuplePositionsInDataChunk[groupID].first, colIdx);
     values[colIdx]->setNull(isNull);
     if (!isNull) {
         readValueBufferToValue(colIdx, valueBuffer);
     }
 }
 
 void FlatTupleIterator::readFlatColToFlatTuple(ft_col_idx_t colIdx, uint8_t* valueBuffer) {
@@ -718,39 +628,40 @@
     }
 }
 
 void FlatTupleIterator::updateInvalidEntriesInFlatTuplePositionsInDataChunk() {
     for (auto i = 0u; i < flatTuplePositionsInDataChunk.size(); i++) {
         bool isValidEntry = false;
         for (auto j = 0u; j < factorizedTable.getTableSchema()->getNumColumns(); j++) {
-            if (factorizedTable.getTableSchema()->getColumn(j)->getDataChunkPos() == i) {
+            if (factorizedTable.getTableSchema()->getColumn(j)->getGroupID() == i) {
                 isValidEntry = true;
                 break;
             }
         }
         if (!isValidEntry) {
             flatTuplePositionsInDataChunk[i] = std::make_pair(UINT64_MAX, UINT64_MAX);
         }
     }
 }
 
 void FlatTupleIterator::updateNumElementsInDataChunk() {
     auto colOffsetInTupleBuffer = 0ul;
     for (auto i = 0u; i < factorizedTable.getTableSchema()->getNumColumns(); i++) {
         auto column = factorizedTable.getTableSchema()->getColumn(i);
+        auto groupID = column->getGroupID();
         // If this is an unflat column, the number of elements is stored in the
         // overflow_value_t struct. Otherwise, the number of elements is 1.
         auto numElementsInDataChunk =
             column->isFlat() ?
                 1 :
                 ((overflow_value_t*)(currentTupleBuffer + colOffsetInTupleBuffer))->numElements;
-        if (column->getDataChunkPos() >= flatTuplePositionsInDataChunk.size()) {
-            flatTuplePositionsInDataChunk.resize(column->getDataChunkPos() + 1);
+        if (groupID >= flatTuplePositionsInDataChunk.size()) {
+            flatTuplePositionsInDataChunk.resize(groupID + 1);
         }
-        flatTuplePositionsInDataChunk[column->getDataChunkPos()] =
+        flatTuplePositionsInDataChunk[groupID] =
             std::make_pair(0 /* nextIdxToReadInDataChunk */, numElementsInDataChunk);
         colOffsetInTupleBuffer += column->getNumBytes();
     }
 }
 
 void FlatTupleIterator::updateFlatTuplePositionsInDataChunk() {
     for (auto i = 0u; i < flatTuplePositionsInDataChunk.size(); i++) {
```

### sdist/kuzu-source/src/processor/result/mark_hash_table.cpp

```diff
@@ -1,15 +1,15 @@
 #include "processor/result/mark_hash_table.h"
 
 namespace kuzu {
 namespace processor {
 
 MarkHashTable::MarkHashTable(storage::MemoryManager& memoryManager,
     std::vector<common::LogicalType> keyTypes, std::vector<common::LogicalType> payloadTypes,
-    uint64_t numEntriesToAllocate, std::unique_ptr<FactorizedTableSchema> tableSchema)
+    uint64_t numEntriesToAllocate, FactorizedTableSchema tableSchema)
     : AggregateHashTable(memoryManager, std::move(keyTypes), std::move(payloadTypes),
           std::vector<std::unique_ptr<function::AggregateFunction>>{} /* empty aggregates */,
           std::vector<common::LogicalType>{} /* empty distinct agg key*/, numEntriesToAllocate,
           std::move(tableSchema)) {
     distinctColIdxInFT = hashColIdxInFT - 1;
 }
```

### sdist/kuzu-source/src/storage/index/hash_index.cpp

```diff
@@ -16,14 +16,15 @@
 #include "storage/buffer_manager/bm_file_handle.h"
 #include "storage/file_handle.h"
 #include "storage/index/hash_index_header.h"
 #include "storage/index/hash_index_slot.h"
 #include "storage/index/hash_index_utils.h"
 #include "storage/index/in_mem_hash_index.h"
 #include "storage/storage_structure/disk_array.h"
+#include "storage/storage_structure/overflow_file.h"
 #include "transaction/transaction.h"
 
 using namespace kuzu::common;
 using namespace kuzu::transaction;
 
 namespace kuzu {
 namespace storage {
@@ -33,85 +34,86 @@
 // Local storage consists of two in memory indexes. One (localInsertionIndex) is to keep track of
 // all newly inserted entries, and the other (localDeletionIndex) is to keep track of newly deleted
 // entries (not available in localInsertionIndex). We assume that in a transaction, the insertions
 // and deletions are very small, thus they can be kept in memory.
 template<typename T>
 class HashIndexLocalStorage {
 public:
-    using Key = typename std::conditional<std::same_as<T, std::string>, std::string_view, T>::type;
+    explicit HashIndexLocalStorage(OverflowFileHandle* handle)
+        : localDeletions{}, localInsertions{handle} {}
+    using OwnedKeyType =
+        typename std::conditional<std::same_as<T, common::ku_string_t>, std::string, T>::type;
+    using Key = typename std::conditional<std::same_as<T, ku_string_t>, std::string_view, T>::type;
     HashIndexLocalLookupState lookup(Key key, common::offset_t& result) {
         if (localDeletions.contains(key)) {
             return HashIndexLocalLookupState::KEY_DELETED;
         }
-        auto elem = localInsertions.find(key);
-        if (elem != localInsertions.end()) {
-            result = elem->second;
+        if (localInsertions.lookup(key, result)) {
             return HashIndexLocalLookupState::KEY_FOUND;
         } else {
             return HashIndexLocalLookupState::KEY_NOT_EXIST;
         }
     }
 
     void deleteKey(Key key) {
-        auto iter = localInsertions.find(key);
-        if (iter != localInsertions.end()) {
-            localInsertions.erase(iter);
-        } else {
-            localDeletions.insert(static_cast<T>(key));
+        if (!localInsertions.deleteKey(key)) {
+            localDeletions.insert(static_cast<OwnedKeyType>(key));
         }
     }
 
     bool insert(Key key, common::offset_t value) {
         auto iter = localDeletions.find(key);
         if (iter != localDeletions.end()) {
             localDeletions.erase(iter);
         }
-        if (localInsertions.contains(key)) {
-            return false;
-        }
-        localInsertions[static_cast<T>(key)] = value;
-        return true;
+        return localInsertions.append(key, value);
+    }
+
+    size_t append(const IndexBuffer<OwnedKeyType>& buffer) {
+        return localInsertions.append(buffer);
     }
 
     inline bool hasUpdates() const { return !(localInsertions.empty() && localDeletions.empty()); }
 
     inline int64_t getNetInserts() const {
         return static_cast<int64_t>(localInsertions.size()) - localDeletions.size();
     }
 
     inline void clear() {
         localInsertions.clear();
         localDeletions.clear();
     }
 
-    void applyLocalChanges(const std::function<void(T)>& deleteOp,
-        const std::function<void(T, common::offset_t)>& insertOp) {
+    void applyLocalChanges(const std::function<void(Key)>& deleteOp,
+        const std::function<void(const InMemHashIndex<T>&)>& insertOp) {
         for (auto& key : localDeletions) {
             deleteOp(key);
         }
-        for (auto& [key, val] : localInsertions) {
-            insertOp(key, val);
-        }
+        insertOp(localInsertions);
     }
 
+    void reserveInserts(uint64_t newEntries) { localInsertions.reserve(newEntries); }
+
+    const InMemHashIndex<T>& getInsertions() { return localInsertions; }
+
 private:
     // When the storage type is string, allow the key type to be string_view with a custom hash
     // function
-    using hash_function = typename std::conditional<std::is_same<T, std::string>::value,
+    using hash_function = typename std::conditional<std::is_same<OwnedKeyType, std::string>::value,
         common::StringUtils::string_hash, std::hash<T>>::type;
-    std::unordered_map<T, common::offset_t, hash_function, std::equal_to<>> localInsertions;
-    std::unordered_set<T, hash_function, std::equal_to<>> localDeletions;
+    std::unordered_set<OwnedKeyType, hash_function, std::equal_to<>> localDeletions;
+    InMemHashIndex<T> localInsertions;
 };
 
 template<typename T>
 HashIndex<T>::HashIndex(const DBFileIDAndName& dbFileIDAndName,
     const std::shared_ptr<BMFileHandle>& fileHandle, OverflowFileHandle* overflowFileHandle,
     uint64_t indexPos, BufferManager& bufferManager, WAL* wal)
     : dbFileIDAndName{dbFileIDAndName}, bm{bufferManager}, wal{wal}, fileHandle(fileHandle),
-      overflowFileHandle(overflowFileHandle), bulkInsertLocalStorage{overflowFileHandle} {
+      overflowFileHandle(overflowFileHandle) {
     // TODO: Handle data not existing
     headerArray = std::make_unique<BaseDiskArray<HashIndexHeader>>(*fileHandle,
         dbFileIDAndName.dbFileID, NUM_HEADER_PAGES * indexPos + INDEX_HEADER_ARRAY_HEADER_PAGE_IDX,
         &bm, wal, Transaction::getDummyReadOnlyTrx().get(), true /*bypassWAL*/);
     // Read indexHeader from the headerArray, which contains only one element.
     this->indexHeaderForReadTrx = std::make_unique<HashIndexHeader>(
         headerArray->get(INDEX_HEADER_IDX_IN_ARRAY, TransactionType::READ_ONLY));
@@ -121,15 +123,15 @@
     pSlots = std::make_unique<BaseDiskArray<Slot<T>>>(*fileHandle, dbFileIDAndName.dbFileID,
         NUM_HEADER_PAGES * indexPos + P_SLOTS_HEADER_PAGE_IDX, &bm, wal,
         Transaction::getDummyReadOnlyTrx().get(), true /*bypassWAL*/);
     oSlots = std::make_unique<BaseDiskArray<Slot<T>>>(*fileHandle, dbFileIDAndName.dbFileID,
         NUM_HEADER_PAGES * indexPos + O_SLOTS_HEADER_PAGE_IDX, &bm, wal,
         Transaction::getDummyReadOnlyTrx().get(), true /*bypassWAL*/);
     // Initialize functions.
-    localStorage = std::make_unique<HashIndexLocalStorage<BufferKeyType>>();
+    localStorage = std::make_unique<HashIndexLocalStorage<T>>(overflowFileHandle);
 }
 
 // For read transactions, local storage is skipped, lookups are performed on the persistent
 // storage. For write transactions, lookups are performed in the local storage first, then in
 // the persistent storage if necessary. In details, there are three cases for the local storage
 // lookup:
 // - the key is found in the local storage, directly return true;
@@ -141,16 +143,15 @@
     if (transaction->isReadOnly()) {
         return lookupInPersistentIndex(transaction->getType(), key, result);
     } else {
         KU_ASSERT(transaction->isWriteTransaction());
         auto localLookupState = localStorage->lookup(key, result);
         if (localLookupState == HashIndexLocalLookupState::KEY_DELETED) {
             return false;
-        } else if (localLookupState == HashIndexLocalLookupState::KEY_FOUND ||
-                   bulkInsertLocalStorage.lookup(key, result)) {
+        } else if (localLookupState == HashIndexLocalLookupState::KEY_FOUND) {
             return true;
         } else {
             KU_ASSERT(localLookupState == HashIndexLocalLookupState::KEY_NOT_EXIST);
             return lookupInPersistentIndex(transaction->getType(), key, result);
         }
     }
 }
@@ -190,15 +191,15 @@
         for (size_t i = 0; i < buffer.size(); i++) {
             const auto& [key, value] = buffer[i];
             if (lookupInPersistentIndex(transaction::TransactionType::WRITE, key, result)) {
                 return i;
             }
         }
     }
-    return bulkInsertLocalStorage.append(buffer);
+    return localStorage->append(buffer);
 }
 
 template<typename T>
 bool HashIndex<T>::lookupInPersistentIndex(TransactionType trxType, Key key, offset_t& result) {
     auto& header = trxType == TransactionType::READ_ONLY ? *this->indexHeaderForReadTrx :
                                                            *this->indexHeaderForWriteTrx;
     // There may not be any primary key slots if we try to lookup on an empty index
@@ -282,24 +283,16 @@
 void HashIndex<T>::prepareCommit() {
     if (localStorage->hasUpdates()) {
         wal->addToUpdatedTables(dbFileIDAndName.dbFileID.nodeIndexID.tableID);
         auto netInserts = localStorage->getNetInserts();
         if (netInserts > 0) {
             reserve(netInserts);
         }
-        localStorage->applyLocalChanges(
-            [this](Key key) -> void { this->deleteFromPersistentIndex(key); },
-            [this](Key key, offset_t value) -> void {
-                this->insertIntoPersistentIndex(key, value);
-            });
-        headerArray->update(INDEX_HEADER_IDX_IN_ARRAY, *indexHeaderForWriteTrx);
-    }
-    if (bulkInsertLocalStorage.size() > 0) {
-        wal->addToUpdatedTables(dbFileIDAndName.dbFileID.nodeIndexID.tableID);
-        mergeBulkInserts();
+        localStorage->applyLocalChanges([&](Key key) { deleteFromPersistentIndex(key); },
+            [&](const auto& insertions) { mergeBulkInserts(insertions); });
         headerArray->update(INDEX_HEADER_IDX_IN_ARRAY, *indexHeaderForWriteTrx);
     }
     headerArray->prepareCommit();
     pSlots->prepareCommit();
     oSlots->prepareCommit();
 }
 
@@ -308,38 +301,36 @@
     if (localStorage->hasUpdates()) {
         wal->addToUpdatedTables(dbFileIDAndName.dbFileID.nodeIndexID.tableID);
     }
 }
 
 template<typename T>
 void HashIndex<T>::checkpointInMemory() {
-    if (!localStorage->hasUpdates() && bulkInsertLocalStorage.size() == 0) {
+    if (!localStorage->hasUpdates()) {
         return;
     }
     *indexHeaderForReadTrx = *indexHeaderForWriteTrx;
     headerArray->checkpointInMemoryIfNecessary();
     pSlots->checkpointInMemoryIfNecessary();
     oSlots->checkpointInMemoryIfNecessary();
     localStorage->clear();
     if constexpr (std::same_as<ku_string_t, T>) {
         overflowFileHandle->checkpointInMemory();
     }
-    bulkInsertLocalStorage.clear();
 }
 
 template<typename T>
 void HashIndex<T>::rollbackInMemory() {
-    if (!localStorage->hasUpdates() && bulkInsertLocalStorage.size() == 0) {
+    if (!localStorage->hasUpdates()) {
         return;
     }
     headerArray->rollbackInMemoryIfNecessary();
     pSlots->rollbackInMemoryIfNecessary();
     oSlots->rollbackInMemoryIfNecessary();
     localStorage->clear();
-    bulkInsertLocalStorage.clear();
     *indexHeaderForWriteTrx = *indexHeaderForReadTrx;
 }
 
 template<>
 inline bool HashIndex<ku_string_t>::equals(transaction::TransactionType trxType,
     std::string_view keyToLookup, const ku_string_t& keyInEntry) const {
     if (HashIndexUtils::areStringPrefixAndLenEqual(keyToLookup, keyInEntry)) {
@@ -457,49 +448,50 @@
     } else {
         splitSlots(*this->indexHeaderForWriteTrx,
             numRequiredSlots - pSlots->getNumElements(TransactionType::WRITE));
     }
 }
 
 template<typename T>
-void HashIndex<T>::sortEntries(typename InMemHashIndex<T>::SlotIterator& slotToMerge,
+void HashIndex<T>::sortEntries(const InMemHashIndex<T>& insertLocalStorage,
+    typename InMemHashIndex<T>::SlotIterator& slotToMerge,
     std::vector<HashIndexEntryView>& entries) {
     do {
         auto numEntries = slotToMerge.slot->header.numEntries();
         for (auto entryPos = 0u; entryPos < numEntries; entryPos++) {
             const auto* entry = &slotToMerge.slot->entries[entryPos];
             const auto hash = hashStored(TransactionType::WRITE, entry->key);
             const auto primarySlot =
                 HashIndexUtils::getPrimarySlotIdForHash(*indexHeaderForWriteTrx, hash);
             entries.push_back(HashIndexEntryView{primarySlot,
                 slotToMerge.slot->header.fingerprints[entryPos], entry});
         }
-    } while (bulkInsertLocalStorage.nextChainedSlot(slotToMerge));
+    } while (insertLocalStorage.nextChainedSlot(slotToMerge));
     std::sort(entries.begin(), entries.end(), [&](auto entry1, auto entry2) -> bool {
         // Sort based on the entry's disk slot ID so that the first slot is at the end
         // Sorting is done reversed so that we can process from the back of the list,
         // using the size to track the remaining entries
         return entry1.diskSlotId > entry2.diskSlotId;
     });
 }
 
 template<typename T>
-void HashIndex<T>::mergeBulkInserts() {
+void HashIndex<T>::mergeBulkInserts(const InMemHashIndex<T>& insertLocalStorage) {
     // TODO: Ideally we can split slots at the same time that we insert new ones
     // Compute the new number of primary slots, and iterate over each slot, determining if it
     // needs to be split (and how many times, which is complicated) and insert/rehash each element
     // one by one. Rehashed entries should be copied into a new slot in-memory, and then that new
     // slot (with the entries from the respective slot in the local storage) should be processed
     // immediately to avoid increasing memory usage (caching one page of slots at a time since split
     // slots usually get rehashed to a new page).
     //
     // On the other hand, two passes may not be significantly slower than one
     // TODO: one pass would also reduce locking when frames are unpinned,
-    // which is useful if this can be paralellized
-    reserve(bulkInsertLocalStorage.size());
+    // which is useful if this can be parallelized
+    reserve(insertLocalStorage.size());
     RUNTIME_CHECK(auto originalNumEntries = this->indexHeaderForWriteTrx->numEntries;);
 
     // Storing as many slots in-memory as on-disk shouldn't be necessary (for one it makes memory
     // usage an issue as we may need significantly more memory to store the slots that we would
     // otherwise) Instead, when merging here we can re-hash and split each in-memory slot (into
     // temporary vector buffers instead of slots for improved performance) and then merge each of
     // those one at a time into the disk slots. That will keep the low memory requirements and still
@@ -518,25 +510,25 @@
     constexpr size_t NUM_SLOTS_PER_PAGE =
         BufferPoolConstants::PAGE_4KB_SIZE / BaseDiskArray<Slot<T>>::getAlignedElementSize();
     std::array<std::vector<HashIndexEntryView>, NUM_SLOTS_PER_PAGE> partitionedEntries;
     // Sort entries for a page of slots at a time, then move vertically and process all entries
     // which map to a given page on disk, then horizontally to the next page in the set. These pages
     // may not be consecutive, but we reduce the memory overhead for storing the information about
     // the sorted data and still just process each page once.
-    for (uint64_t localSlotId = 0; localSlotId < bulkInsertLocalStorage.numPrimarySlots();
+    for (uint64_t localSlotId = 0; localSlotId < insertLocalStorage.numPrimarySlots();
          localSlotId += NUM_SLOTS_PER_PAGE) {
         for (size_t i = 0;
-             i < NUM_SLOTS_PER_PAGE && localSlotId + i < bulkInsertLocalStorage.numPrimarySlots();
+             i < NUM_SLOTS_PER_PAGE && localSlotId + i < insertLocalStorage.numPrimarySlots();
              i++) {
             auto localSlot =
-                typename InMemHashIndex<T>::SlotIterator(localSlotId + i, &bulkInsertLocalStorage);
+                typename InMemHashIndex<T>::SlotIterator(localSlotId + i, &insertLocalStorage);
             partitionedEntries[i].clear();
             // Results are sorted in reverse, so we can process the end first and pop_back to remove
             // them from the vector
-            sortEntries(localSlot, partitionedEntries[i]);
+            sortEntries(insertLocalStorage, localSlot, partitionedEntries[i]);
         }
         // Repeat until there are no un-processed partitions in partitionedEntries
         // This will run at most NUM_SLOTS_PER_PAGE times the number of entries
         std::bitset<NUM_SLOTS_PER_PAGE> done;
         while (!done.all()) {
             std::optional<page_idx_t> diskSlotPage;
             for (size_t i = 0; i < NUM_SLOTS_PER_PAGE; i++) {
@@ -556,15 +548,15 @@
                     }
                 } else {
                     done[i] = true;
                 }
             }
         }
     }
-    KU_ASSERT(originalNumEntries + bulkInsertLocalStorage.getIndexHeader().numEntries ==
+    KU_ASSERT(originalNumEntries + insertLocalStorage.getIndexHeader().numEntries ==
               indexHeaderForWriteTrx->numEntries);
 }
 
 template<typename T>
 size_t HashIndex<T>::mergeSlot(const std::vector<HashIndexEntryView>& slotToMerge,
     typename BaseDiskArray<Slot<T>>::WriteIterator& diskSlotIterator,
     typename BaseDiskArray<Slot<T>>::WriteIterator& diskOverflowSlotIterator,
@@ -614,14 +606,19 @@
         diskEntryPos++;
         merged++;
     }
     return merged;
 }
 
 template<typename T>
+void HashIndex<T>::bulkReserve(uint64_t newEntries) {
+    return localStorage->reserveInserts(newEntries);
+}
+
+template<typename T>
 HashIndex<T>::~HashIndex() = default;
 
 template class HashIndex<int64_t>;
 template class HashIndex<int32_t>;
 template class HashIndex<int16_t>;
 template class HashIndex<int8_t>;
 template class HashIndex<uint64_t>;
```

### sdist/kuzu-source/src/storage/index/in_mem_hash_index.cpp

```diff
@@ -285,15 +285,15 @@
         KU_ASSERT(slot.header.numEntries() == 0);
         slot.header.nextOvfSlotId = SlotHeader::INVALID_OVERFLOW_SLOT_ID;
         return freeOSlotId;
     }
 }
 
 template<typename T>
-Slot<T>* InMemHashIndex<T>::getSlot(const SlotInfo& slotInfo) {
+Slot<T>* InMemHashIndex<T>::getSlot(const SlotInfo& slotInfo) const {
     if (slotInfo.slotType == SlotType::PRIMARY) {
         return &pSlots->operator[](slotInfo.slotId);
     } else {
         return &oSlots->operator[](slotInfo.slotId);
     }
 }
 
@@ -363,14 +363,56 @@
         NUM_HEADER_PAGES * indexPos + O_SLOTS_HEADER_PAGE_IDX, 1 /*numElements */);
 
     headerArray.saveToDisk();
     pSlots.saveToDisk();
     oSlots.saveToDisk();
 }
 
+template<typename T>
+bool InMemHashIndex<T>::deleteKey(Key key) {
+    if (this->indexHeader.numEntries == 0) {
+        return false;
+    }
+    auto hashValue = HashIndexUtils::hash(key);
+    auto fingerprint = HashIndexUtils::getFingerprintForHash(hashValue);
+    auto slotId = HashIndexUtils::getPrimarySlotIdForHash(this->indexHeader, hashValue);
+    SlotIterator iter(slotId, this);
+    std::optional<entry_pos_t> deletedPos = 0;
+    do {
+        for (auto entryPos = 0u; entryPos < getSlotCapacity<T>(); entryPos++) {
+            if (iter.slot->header.isEntryValid(entryPos) &&
+                iter.slot->header.fingerprints[entryPos] == fingerprint &&
+                equals(key, iter.slot->entries[entryPos].key)) {
+                deletedPos = entryPos;
+                iter.slot->header.setEntryInvalid(entryPos);
+                break;
+            }
+        }
+        if (deletedPos.has_value()) {
+            break;
+        }
+    } while (nextChainedSlot(iter));
+
+    if (deletedPos.has_value()) {
+        // Find the last valid entry and move it into the deleted position
+        auto newIter = iter;
+        while (nextChainedSlot(newIter))
+            ;
+        if (newIter.slotInfo != iter.slotInfo ||
+            *deletedPos != newIter.slot->header.numEntries() - 1) {
+            auto lastEntryPos = newIter.slot->header.numEntries();
+            iter.slot->entries[*deletedPos] = newIter.slot->entries[lastEntryPos];
+            iter.slot->header.setEntryValid(*deletedPos,
+                newIter.slot->header.fingerprints[lastEntryPos]);
+            newIter.slot->header.setEntryInvalid(lastEntryPos);
+        }
+    }
+    return false;
+}
+
 template class InMemHashIndex<int64_t>;
 template class InMemHashIndex<int32_t>;
 template class InMemHashIndex<int16_t>;
 template class InMemHashIndex<int8_t>;
 template class InMemHashIndex<uint64_t>;
 template class InMemHashIndex<uint32_t>;
 template class InMemHashIndex<uint16_t>;
```

### sdist/kuzu.egg-info/PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuzu
-Version: 0.4.2.dev6
+Version: 0.4.2.dev7
 Summary: An in-process property graph database management system built for query speed and scalability.
 Home-page: https://github.com/kuzudb/kuzu
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kuzu Version: 0.4.2.dev6 Summary: An in-process
+Metadata-Version: 2.1 Name: kuzu Version: 0.4.2.dev7 Summary: An in-process
 property graph database management system built for query speed and
 scalability. Home-page: https://github.com/kuzudb/kuzu License: MIT Platform:
 UNKNOWN Description-Content-Type: text/markdown License-File: LICENSE
                     [https://kuzudb.com/img/kuzu-logo.png]
 
   _[_G_i_t_h_u_b_ _A_c_t_i_o_n_s_ _B_a_d_g_e_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_i_t_h_u_b_/_k_u_z_u_d_b_/_k_u_z_u_/_b_r_a_n_c_h_/_m_a_s_t_e_r_/
               _g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_N_1_A_T_6_H_7_9_L_M_]_[_d_i_s_c_o_r_d_]_[_t_w_i_t_t_e_r_]
```

### sdist/pyproject.toml

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "kuzu"
 description = "Highly scalable, extremely fast, easy-to-use embeddable graph database"
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = ["graph", "database"]
-version = "0.4.2.dev6"
+version = "0.4.2.dev7"
 
 [project.urls]
 Homepage = "https://kuzudb.com/"
 Documentation = "https://docs.kuzudb.com/"
 Repository = "https://github.com/kuzudb/kuzu"
 Changelog = "https://github.com/kuzudb/kuzu/releases"
```

