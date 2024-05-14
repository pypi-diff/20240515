# Comparing `tmp/beaker_bunsen-0.0.1.tar.gz` & `tmp/beaker_bunsen-0.0.2.tar.gz`

## Comparing `beaker_bunsen-0.0.1.tar` & `beaker_bunsen-0.0.2.tar`

### file list

```diff
@@ -1,94 +1,95 @@
--rw-r--r--   0        0        0     6076 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/DEFINITIONS.md
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/.github/workflows/build-publish.yaml
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/.github/workflows/test.yaml
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/src/beaker_bunsen/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/src/beaker_bunsen/__init__.py
--rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/src/beaker_bunsen/bunsen_agent.py
--rw-r--r--   0        0        0     8548 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/src/beaker_bunsen/bunsen_context.py
--rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/src/beaker_bunsen/corpus.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/src/beaker_bunsen/builder/__init__.py
--rw-r--r--   0        0        0     9282 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/src/beaker_bunsen/builder/hooks.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/src/beaker_bunsen/vectordb/__init__.py
--rw-r--r--   0        0        0    14512 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/src/beaker_bunsen/vectordb/chromadb_store.py
--rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/src/beaker_bunsen/vectordb/types.py
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/src/beaker_bunsen/vectordb/vector_store.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/src/beaker_bunsen/vectordb/embedders/__init__.py
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/src/beaker_bunsen/vectordb/embedders/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/src/beaker_bunsen/vectordb/embedders/code.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/src/beaker_bunsen/vectordb/embedders/documentation.py
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/src/beaker_bunsen/vectordb/embedders/examples.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/src/beaker_bunsen/vectordb/loaders/__init__.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/src/beaker_bunsen/vectordb/loaders/base.py
--rw-r--r--   0        0        0     4991 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/src/beaker_bunsen/vectordb/loaders/code_library_loader.py
--rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/src/beaker_bunsen/vectordb/loaders/local_file_loader.py
--rw-r--r--   0        0        0     7215 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/src/beaker_bunsen/vectordb/loaders/schemes.py
--rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/src/beaker_bunsen/vectordb/util/helpers.py
--rw-r--r--   0        0        0    10848 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/src/beaker_bunsen/vectordb/util/splitters.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/test_base_embedder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/test_build.py
--rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/test_chromadb.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/test_code_loaders.py
--rw-r--r--   0        0        0     5306 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/test_corpus.py
--rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/test_documentation_embedder.py
--rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/test_example_embedder.py
--rw-r--r--   0        0        0     4653 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/test_local_file_loader.py
--rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/test_schemes.py
--rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/test_utils.py
--rw-r--r--   0        0        0     9969 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/test_zipped_chromadb.py
--rw-r--r--   0        0        0  1828380 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/store.zip
--rw-r--r--   0        0        0  5947974 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/corpuses/corpus.zip
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/config.yaml
--rw-r--r--   0        0        0  5692346 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/store.zip
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/code/requests
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/code/requests.__version__
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/code/requests._internal_utils
--rw-r--r--   0        0        0    19553 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/code/requests.adapters
--rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/code/requests.api
--rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/code/requests.auth
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/code/requests.certs
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/code/requests.compat
--rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/code/requests.cookies
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/code/requests.exceptions
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/code/requests.help
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/code/requests.hooks
--rw-r--r--   0        0        0    35223 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/code/requests.models
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/code/requests.packages
--rw-r--r--   0        0        0    30373 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/code/requests.sessions
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/code/requests.status_codes
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/code/requests.structures
--rw-r--r--   0        0        0    33448 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/code/requests.utils
--rw-r--r--   0        0        0     9885 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/documentation/mathjax_readme.md
--rw-r--r--   0        0        0    22571 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/documentation/ruff_readme.md
--rw-r--r--   0        0        0     9885 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/documentation/mathjax_readme.md
--rw-r--r--   0        0        0    22571 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/documentation/ruff_readme.md
--rw-r--r--   0        0        0   137697 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/documents/Lunar_Sample_Laboratory_Facility.html
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/documents/yorkshire.txt
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/documents/yorkshire.txt.metadata
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/documents/recipes/.metadata
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/documents/recipes/ham_and_lentil_soup
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/documents/recipes/irish_potato_caserole
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/documents/recipes/tajine_maadnous
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/documents/recipes/winter_risotto
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/documents/recipes/winter_risotto.metadata
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/examples/example_1.md
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/examples/example_2.md
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/examples/example_3.md
--rw-r--r--   0        0        0   307464 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/images/kitten-sad.jpg
--rw-r--r--   0        0        0   417493 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/images/kitten_hacker.jpg
--rw-r--r--   0        0        0    12955 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/images/puppy_hacker.jpg
--rw-r--r--   0        0        0    64027 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/images/puppy_sad.png
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/subproject/pyproject.toml
--rw-r--r--   0        0        0     9885 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/subproject/documentation/mathjax_readme.md
--rw-r--r--   0        0        0    22571 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/subproject/documentation/ruff_readme.md
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/subproject/examples/example_1.md
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/subproject/examples/example_2.md
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/subproject/examples/example_3.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/subproject/src/test_project/__init__.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/subproject/src/test_project/agent.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/tests/data/subproject/src/test_project/context.py
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/README.md
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     6076 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/DEFINITIONS.md
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/.github/workflows/build-publish.yaml
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/__init__.py
+-rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/bunsen_agent.py
+-rw-r--r--   0        0        0     8638 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/bunsen_context.py
+-rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/corpus.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/builder/__init__.py
+-rw-r--r--   0        0        0     9305 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/builder/hooks.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/__init__.py
+-rw-r--r--   0        0        0    14512 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/chromadb_store.py
+-rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/types.py
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/vector_store.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/embedders/__init__.py
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/embedders/base.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/embedders/code.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/embedders/document.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/embedders/documentation.py
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/embedders/examples.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/loaders/__init__.py
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/loaders/base.py
+-rw-r--r--   0        0        0     5352 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/loaders/code_library_loader.py
+-rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/loaders/local_file_loader.py
+-rw-r--r--   0        0        0     7215 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/loaders/schemes.py
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/util/helpers.py
+-rw-r--r--   0        0        0    10848 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/util/splitters.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/test_base_embedder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/test_build.py
+-rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/test_chromadb.py
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/test_code_loaders.py
+-rw-r--r--   0        0        0     5306 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/test_corpus.py
+-rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/test_documentation_embedder.py
+-rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/test_example_embedder.py
+-rw-r--r--   0        0        0     5626 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/test_local_file_loader.py
+-rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/test_schemes.py
+-rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/test_utils.py
+-rw-r--r--   0        0        0     9969 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/test_zipped_chromadb.py
+-rw-r--r--   0        0        0  1828380 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/store.zip
+-rw-r--r--   0        0        0  5947974 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/corpus.zip
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/config.yaml
+-rw-r--r--   0        0        0  5692346 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/store.zip
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.__version__
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests._internal_utils
+-rw-r--r--   0        0        0    19553 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.adapters
+-rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.api
+-rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.auth
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.certs
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.compat
+-rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.cookies
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.exceptions
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.help
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.hooks
+-rw-r--r--   0        0        0    35223 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.models
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.packages
+-rw-r--r--   0        0        0    30373 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.sessions
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.status_codes
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.structures
+-rw-r--r--   0        0        0    33448 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.utils
+-rw-r--r--   0        0        0     9885 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/documentation/mathjax_readme.md
+-rw-r--r--   0        0        0    22571 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/documentation/ruff_readme.md
+-rw-r--r--   0        0        0     9885 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/documentation/mathjax_readme.md
+-rw-r--r--   0        0        0    22571 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/documentation/ruff_readme.md
+-rw-r--r--   0        0        0   137697 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/documents/Lunar_Sample_Laboratory_Facility.html
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/documents/yorkshire.txt
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/documents/yorkshire.txt.metadata
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/documents/recipes/.metadata
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/documents/recipes/ham_and_lentil_soup
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/documents/recipes/irish_potato_caserole
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/documents/recipes/tajine_maadnous
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/documents/recipes/winter_risotto
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/documents/recipes/winter_risotto.metadata
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/examples/example_1.md
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/examples/example_2.md
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/examples/example_3.md
+-rw-r--r--   0        0        0   307464 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/images/kitten-sad.jpg
+-rw-r--r--   0        0        0   417493 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/images/kitten_hacker.jpg
+-rw-r--r--   0        0        0    12955 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/images/puppy_hacker.jpg
+-rw-r--r--   0        0        0    64027 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/images/puppy_sad.png
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/subproject/pyproject.toml
+-rw-r--r--   0        0        0     9885 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/subproject/documentation/mathjax_readme.md
+-rw-r--r--   0        0        0    22571 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/subproject/documentation/ruff_readme.md
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/subproject/examples/example_1.md
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/subproject/examples/example_2.md
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/subproject/examples/example_3.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/subproject/src/test_project/__init__.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/subproject/src/test_project/agent.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/subproject/src/test_project/context.py
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/README.md
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/PKG-INFO
```

### Comparing `beaker_bunsen-0.0.1/DEFINITIONS.md` & `beaker_bunsen-0.0.2/DEFINITIONS.md`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/.github/workflows/test.yaml` & `beaker_bunsen-0.0.2/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/src/beaker_bunsen/bunsen_agent.py` & `beaker_bunsen-0.0.2/src/beaker_bunsen/bunsen_agent.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/src/beaker_bunsen/bunsen_context.py` & `beaker_bunsen-0.0.2/src/beaker_bunsen/bunsen_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,20 +25,25 @@
     from beaker_kernel.kernel import LLMKernel
     from beaker_kernel.lib.subkernels.base import BaseSubkernel
 
 
 logger = logging.getLogger(__name__)
 
 
+class EnvironmentSerializer:
+    pass
+
+
 class BunsenContext(BaseContext):
     agent_cls: BunsenAgent
     corpus: Corpus
 
     enabled_subkernels: list[str]
     bunsen_config: dict[str, Any] | None
+    environment_serializer: EnvironmentSerializer
 
     def __init__(
         self,
         beaker_kernel: "LLMKernel",
         config: Dict[str, Any],
     ) -> None:
         super().__init__(beaker_kernel, self.agent_cls, config)
```

### Comparing `beaker_bunsen-0.0.1/src/beaker_bunsen/corpus.py` & `beaker_bunsen-0.0.2/src/beaker_bunsen/corpus.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/src/beaker_bunsen/builder/hooks.py` & `beaker_bunsen-0.0.2/src/beaker_bunsen/builder/hooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from typing import Any
 
 from hatchling.builders.config import BuilderConfig
 from hatchling.builders.hooks.plugin.interface import BuildHookInterface
 from hatchling.plugin import hookimpl
 
 from beaker_kernel.lib.context import BaseContext
-from ..vectordb.embedders import DocumentationEmbedder, ExampleEmbedder
+from ..vectordb.embedders import DocumentationEmbedder, ExampleEmbedder, CodeEmbedder, PythonEmbedder
 from ..vectordb.loaders import LocalFileLoader, PythonLibraryLoader
 from ..vectordb.chromadb_store import ZippedChromaDBStore
 from ..corpus import Corpus
 
 
 logger = logging.getLogger("bunsen_build")
 
@@ -113,15 +113,15 @@
                 embedder_cls=ExampleEmbedder,
                 loader=LocalFileLoader(locations=[examples_path]),
                 partition="examples",
             )
 
         if python_libraries:
             corpus.ingest(
-                embedder_cls=DocumentationEmbedder,
+                embedder_cls=PythonEmbedder,
                 loader=PythonLibraryLoader(locations=python_libraries),
                 partition="code"
             )
 
         examples = corpus.store.get_all(partition="examples")
         if examples:
             failures = self.test_examples(examples)
```

### Comparing `beaker_bunsen-0.0.1/src/beaker_bunsen/vectordb/chromadb_store.py` & `beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/chromadb_store.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/src/beaker_bunsen/vectordb/types.py` & `beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/types.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/src/beaker_bunsen/vectordb/vector_store.py` & `beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/vector_store.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/src/beaker_bunsen/vectordb/embedders/base.py` & `beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/embedders/base.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/src/beaker_bunsen/vectordb/embedders/examples.py` & `beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/embedders/examples.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/src/beaker_bunsen/vectordb/loaders/code_library_loader.py` & `beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/loaders/code_library_loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     Scheme = PythonModuleScheme
     SLUG = "python"
 
     def discover(
         self,
         locations: list[str] | DefaultType = Default,
         metadata: dict | DefaultType = Default,
+        exclusions: list[str] = Default,
     ):
         """
         The `locations` should be Python packages, modules or submodules that are installed via the pyproject
         requirements.  Each location must be importable using the syntax `import {location}`, so you can include
         either top-level modules such as 'pandas' or submodules such as `pandas.plotting`.  The loader will recurse
         through and to include anything defined "below" the specified location in the import tree. I.e. location
         `pandas` will load all submodules, but `pandas.api.extensions` will not import any other submodules under
@@ -43,34 +44,43 @@
 
         Example: locations=["requests", "os.path", "pandas.core", "pandas.util"]
         """
         if locations is Default:
             locations = self.locations
         if metadata is Default:
             metadata = self.metadata
+        if exclusions is Default:
+            exclusions = self.exclusions
+
+        # Update or define locations and exclusions based on '!' prefix in location.
+        locations, parsed_exclusions = self.parse_locations(locations)
+        exclusions.extend(parsed_exclusions)
 
         modules_to_collect = deque()
         for module_name in locations:
             module_spec = importlib.util.find_spec(module_name)
             if module_spec is None:
                 raise ValueError(f"Module '{module_name}' is not able to be imported. Please ensure that it is listed as a requirement and that 'require-runtime-dependencies' is enabled if error encountered during build.")
             modules_to_collect.append(module_spec)
 
         while modules_to_collect:
             module_spec = modules_to_collect.popleft()
 
-            # TODO: Switch this to type of loader? SourceFileLoader works, ExtensionFileLoader doesn't...
             if not module_spec.origin.endswith('.py'):
                 logger.info(f"Skipping importing non-python file {module_spec.origin}")
                 continue
 
-            # if module_spec.submodule_search_locations:
             if getattr(module_spec, "submodule_search_locations", []):
                 subpkg_info: pkgutil.ModuleInfo = pkgutil.iter_modules(path=module_spec.submodule_search_locations)
                 subpkg_specs = (info.module_finder.find_spec(f"{module_spec.name}.{info.name}") for info in subpkg_info)
+                if self.exclusions:
+                    subpkg_specs = (
+                        spec for spec in subpkg_specs
+                        if not self.should_exclude(spec)
+                    )
                 modules_to_collect.extend(
                     subpkg_specs
                 )
 
             if hasattr(module_spec, "loader"):
                 source = module_spec.loader.get_source(module_spec.name)
             else:
```

### Comparing `beaker_bunsen-0.0.1/src/beaker_bunsen/vectordb/loaders/local_file_loader.py` & `beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/loaders/local_file_loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,19 +13,23 @@
 
     Scheme = LocalFileScheme
     SLUG = "local"
 
     def __init__(
         self,
         locations: list[str] | None = None,
-        metadata: dict | None = None
+        metadata: dict | None = None,
+        exclusions: list[str] | None = None,
     ):
+        exclusions = exclusions or []
         if locations:
+            locations, parsed_exclusions = self.parse_locations(locations)
+            exclusions.extend(parsed_exclusions)
             self._check_locations_exist(locations)
-        super().__init__(locations, metadata)
+        super().__init__(locations, metadata, exclusions)
 
     @staticmethod
     def _check_locations_exist(locations: list[str]):
         missing_locations = []
         for location in locations:
             if isinstance(location, Path):
                 location = str(location.absolute())
@@ -42,17 +46,25 @@
                 collapsed_metadata.update(metadata)
         return collapsed_metadata
 
     def discover(
         self,
         locations: list[str] | DefaultType = Default,
         metadata: dict | DefaultType = Default,
+        exclusions: list[str] = Default,
     ):
+        # Initialize exclusions first so we can extend it if there are any negated locations
+        if exclusions is Default:
+            exclusions = self.exclusions
+
         # Validate locations if they are passed in. If they are not, use location from initialization.
         if locations is not Default:
+            # Update or define locations and exclusions based on '!' prefix in location.
+            locations, parsed_exclusions = self.parse_locations(locations)
+            exclusions.extend(parsed_exclusions)
             self._check_locations_exist(locations)
         else:
             locations = self.locations
 
         if locations is None:
             raise ValueError("No locations specified to discover local files")
 
@@ -61,14 +73,18 @@
             metadata.update(self.metadata)
 
         locations_queue = deque((location, [metadata]) for location in locations)
         while locations_queue:
             location, location_metadata = locations_queue.popleft()
             if isinstance(location, Path):
                 location = str(location.absolute())
+
+            if self.should_exclude(str(location)):
+                continue
+
             if os.path.isdir(location):
                 # Check for directory metadata file
                 dir_metadata_path = os.path.join(location, '.metadata')
                 if os.path.isfile(dir_metadata_path):
                     with open(dir_metadata_path, 'r') as metadata_file:
                         dir_metadata = json.load(metadata_file)
                         location_metadata.append(dir_metadata)
```

### Comparing `beaker_bunsen-0.0.1/src/beaker_bunsen/vectordb/loaders/schemes.py` & `beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/loaders/schemes.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/src/beaker_bunsen/vectordb/util/helpers.py` & `beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/util/helpers.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/src/beaker_bunsen/vectordb/util/splitters.py` & `beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/util/splitters.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/test_base_embedder.py` & `beaker_bunsen-0.0.2/tests/test_base_embedder.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/test_chromadb.py` & `beaker_bunsen-0.0.2/tests/test_chromadb.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/test_code_loaders.py` & `beaker_bunsen-0.0.2/tests/test_code_loaders.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,7 +40,12 @@
     source = python_loader.read(uri)
 
     assert len(source) > 0
     assert isinstance(source, str)
     assert source.startswith('r"""OS')
     assert "\nenviron = " in source
     assert "def makedirs(" in source
+
+
+def test_exclusions_init():
+    # TODO: Fill me in along with other tests
+    pass
```

### Comparing `beaker_bunsen-0.0.1/tests/test_corpus.py` & `beaker_bunsen-0.0.2/tests/test_corpus.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/test_documentation_embedder.py` & `beaker_bunsen-0.0.2/tests/test_documentation_embedder.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/test_example_embedder.py` & `beaker_bunsen-0.0.2/tests/test_example_embedder.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/test_local_file_loader.py` & `beaker_bunsen-0.0.2/tests/test_local_file_loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -94,7 +94,29 @@
     relative_path =  Path("data") / "documents" / "yorkshire.txt"
     data = local_file_loader.read(str(relative_path), base=str(base))
 
     assert len(data) > 0
     assert isinstance(data, str)
     assert data.startswith("Yorkshire")
     assert data.endswith("Yorkshire Rugby Football Union.\n")
+
+def test_exclusions_init():
+    exclusion = "ato"
+    abs_file_path = Path(__file__).parent / "data" / "documents"
+    local_file_loader = LocalFileLoader(
+        locations=[abs_file_path],
+        exclusions=[exclusion],
+    )
+    found_locations = set([record.uri for record in local_file_loader.discover()])
+    # Strip off any `{prefix}:` from the locations
+    found_files = set([location.split(":", maxsplit=1)[1] for location in found_locations])
+
+    files_from_os_walk = set()
+    for path, _, files in os.walk(abs_file_path, ):
+        files_from_os_walk.update([os.path.join(path, f) for f in files if not f.endswith('.metadata')])
+
+    excluded_files = files_from_os_walk - found_files
+
+    assert len(found_files) < len(files_from_os_walk)
+    assert any([exclusion in filename for filename in files_from_os_walk])
+    assert all([exclusion in filename for filename in excluded_files])
+    assert all([exclusion not in filename for filename in found_files])
```

### Comparing `beaker_bunsen-0.0.1/tests/test_schemes.py` & `beaker_bunsen-0.0.2/tests/test_schemes.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/test_utils.py` & `beaker_bunsen-0.0.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/test_zipped_chromadb.py` & `beaker_bunsen-0.0.2/tests/test_zipped_chromadb.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/data/store.zip` & `beaker_bunsen-0.0.2/tests/data/store.zip`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/data/corpuses/corpus.zip` & `beaker_bunsen-0.0.2/tests/data/corpuses/corpus.zip`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/store.zip` & `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/store.zip`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/code/requests` & `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/code/requests._internal_utils` & `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests._internal_utils`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/code/requests.adapters` & `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.adapters`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/code/requests.api` & `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.api`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/code/requests.auth` & `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.auth`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/code/requests.compat` & `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.compat`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/code/requests.cookies` & `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.cookies`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/code/requests.exceptions` & `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.exceptions`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/code/requests.help` & `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.help`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/code/requests.hooks` & `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.hooks`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/code/requests.models` & `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.models`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/code/requests.packages` & `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.packages`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/code/requests.sessions` & `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.sessions`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/code/requests.status_codes` & `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.status_codes`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/code/requests.structures` & `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.structures`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/code/requests.utils` & `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.utils`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/documentation/mathjax_readme.md` & `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/documentation/mathjax_readme.md`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/data/corpuses/test-corpus/resources/documentation/ruff_readme.md` & `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/documentation/ruff_readme.md`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/data/documentation/mathjax_readme.md` & `beaker_bunsen-0.0.2/tests/data/documentation/mathjax_readme.md`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/data/documentation/ruff_readme.md` & `beaker_bunsen-0.0.2/tests/data/documentation/ruff_readme.md`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/data/documents/Lunar_Sample_Laboratory_Facility.html` & `beaker_bunsen-0.0.2/tests/data/documents/Lunar_Sample_Laboratory_Facility.html`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/data/documents/yorkshire.txt` & `beaker_bunsen-0.0.2/tests/data/documents/yorkshire.txt`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/data/documents/recipes/irish_potato_caserole` & `beaker_bunsen-0.0.2/tests/data/documents/recipes/irish_potato_caserole`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/data/documents/recipes/tajine_maadnous` & `beaker_bunsen-0.0.2/tests/data/documents/recipes/tajine_maadnous`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/data/documents/recipes/winter_risotto` & `beaker_bunsen-0.0.2/tests/data/documents/recipes/winter_risotto`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/data/images/kitten-sad.jpg` & `beaker_bunsen-0.0.2/tests/data/images/kitten-sad.jpg`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/data/images/kitten_hacker.jpg` & `beaker_bunsen-0.0.2/tests/data/images/kitten_hacker.jpg`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/data/images/puppy_hacker.jpg` & `beaker_bunsen-0.0.2/tests/data/images/puppy_hacker.jpg`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/data/images/puppy_sad.png` & `beaker_bunsen-0.0.2/tests/data/images/puppy_sad.png`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/data/subproject/pyproject.toml` & `beaker_bunsen-0.0.2/tests/data/subproject/pyproject.toml`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/data/subproject/documentation/mathjax_readme.md` & `beaker_bunsen-0.0.2/tests/data/subproject/documentation/mathjax_readme.md`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/tests/data/subproject/documentation/ruff_readme.md` & `beaker_bunsen-0.0.2/tests/data/subproject/documentation/ruff_readme.md`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/.gitignore` & `beaker_bunsen-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/LICENSE.txt` & `beaker_bunsen-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/README.md` & `beaker_bunsen-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.1/pyproject.toml` & `beaker_bunsen-0.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-  "beaker-kernel~=1.4",
+  "beaker-kernel~=1.5.1",
   "archytas~=1.1.6",
   "chromadb~=0.4.22",
   "tenacity~=8.2.3",
   "tiktoken~=0.5.2",
   "marko~=2.0.3",
   "pysqlite3-binary~=0.5.2",
   "hatchling",
```

### Comparing `beaker_bunsen-0.0.1/PKG-INFO` & `beaker_bunsen-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: beaker-bunsen
-Version: 0.0.1
+Version: 0.0.2
 Summary: Quickly generate new Beaker contexts for new domains and libraries.
 Project-URL: Documentation, https://github.com/unknown/beaker-bunsen#readme
 Project-URL: Issues, https://github.com/unknown/beaker-bunsen/issues
 Project-URL: Source, https://github.com/unknown/beaker-bunsen
 Author-email: Matthew Printz <matt@jataware.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: archytas~=1.1.6
-Requires-Dist: beaker-kernel~=1.4
+Requires-Dist: beaker-kernel~=1.5.1
 Requires-Dist: chromadb~=0.4.22
 Requires-Dist: hatchling
 Requires-Dist: marko~=2.0.3
 Requires-Dist: pysqlite3-binary~=0.5.2
 Requires-Dist: tenacity~=8.2.3
 Requires-Dist: tiktoken~=0.5.2
 Description-Content-Type: text/markdown
```

