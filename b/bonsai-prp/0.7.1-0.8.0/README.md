# Comparing `tmp/bonsai-prp-0.7.1.tar.gz` & `tmp/bonsai_prp-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bonsai-prp-0.7.1.tar", last modified: Tue Apr  9 11:34:10 2024, max compression
+gzip compressed data, was "bonsai_prp-0.8.0.tar", last modified: Wed May 15 14:08:34 2024, max compression
```

## Comparing `bonsai-prp-0.7.1.tar` & `bonsai_prp-0.8.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:34:10.082589 bonsai-prp-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-09 11:34:10.078589 bonsai-prp-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:34:10.078589 bonsai-prp-0.7.1/bonsai_prp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-09 11:34:10.000000 bonsai-prp-0.7.1/bonsai_prp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-09 11:34:10.000000 bonsai-prp-0.7.1/bonsai_prp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 11:34:10.000000 bonsai-prp-0.7.1/bonsai_prp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 11:34:10.000000 bonsai-prp-0.7.1/bonsai_prp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-09 11:34:10.000000 bonsai-prp-0.7.1/bonsai_prp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-09 11:34:10.000000 bonsai-prp-0.7.1/bonsai_prp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:34:10.074589 bonsai-prp-0.7.1/prp/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16073 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:34:10.078589 bonsai-prp-0.7.1/prp/models/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/models/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     7057 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/models/phenotype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/models/qc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/models/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/models/species.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/models/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/models/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:34:10.078589 bonsai-prp-0.7.1/prp/parse/
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/parse/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/parse/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:34:10.078589 bonsai-prp-0.7.1/prp/parse/phenotype/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/parse/phenotype/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7084 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/parse/phenotype/amrfinder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/parse/phenotype/mykrobe.py
--rw-r--r--   0 runner    (1001) docker     (127)    14502 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/parse/phenotype/resfinder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/parse/phenotype/serotypefinder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/parse/phenotype/tbprofiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/parse/phenotype/virulencefinder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10891 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/parse/qc.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/parse/species.py
--rw-r--r--   0 runner    (1001) docker     (127)     7067 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/parse/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/parse/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/parse/variant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 11:34:10.082589 bonsai-prp-0.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:34:10.078589 bonsai-prp-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:08:34.000383 bonsai_prp-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-15 14:08:34.000383 bonsai_prp-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:08:33.996382 bonsai_prp-0.8.0/bonsai_prp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-15 14:08:33.000000 bonsai_prp-0.8.0/bonsai_prp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-15 14:08:33.000000 bonsai_prp-0.8.0/bonsai_prp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:08:33.000000 bonsai_prp-0.8.0/bonsai_prp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-15 14:08:33.000000 bonsai_prp-0.8.0/bonsai_prp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-15 14:08:33.000000 bonsai_prp-0.8.0/bonsai_prp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 14:08:33.000000 bonsai_prp-0.8.0/bonsai_prp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:08:33.992382 bonsai_prp-0.8.0/prp/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17623 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:08:33.996382 bonsai_prp-0.8.0/prp/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/models/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/models/phenotype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/models/qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/models/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/models/species.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/models/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/models/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:08:33.996382 bonsai_prp-0.8.0/prp/parse/
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/parse/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/parse/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:08:33.996382 bonsai_prp-0.8.0/prp/parse/phenotype/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/parse/phenotype/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7084 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/parse/phenotype/amrfinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/parse/phenotype/mykrobe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14440 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/parse/phenotype/resfinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/parse/phenotype/serotypefinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/parse/phenotype/tbprofiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/parse/phenotype/virulencefinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11232 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/parse/qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/parse/species.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8005 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/parse/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10933 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/parse/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/parse/variant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 14:08:34.000383 bonsai_prp-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:08:33.996382 bonsai_prp-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7892 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/tests/test_cli.py
```

### Comparing `bonsai-prp-0.7.1/LICENSE` & `bonsai_prp-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bonsai-prp-0.7.1/PKG-INFO` & `bonsai_prp-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bonsai-prp
-Version: 0.7.1
+Version: 0.8.0
 Summary: Pipline result processing program for the JASEN pipeline and Bonsai tool.
 Author-email: Markus Johansson <markus.h.johansson@skane.se>, Ryan Kennedy <Ryan.Kennedy@skane.se>
 Project-URL: Repository, https://github.com/Clinical-Genomics-Lund/
 Project-URL: Issues, https://github.com/Clinical-Genomics-Lund/bonsai-prp/issues
 Project-URL: Changelog, https://github.com/Clinical-Genomics-Lund/CHANGELOG.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
@@ -21,14 +21,15 @@
 Requires-Dist: click==8.1.7
 Requires-Dist: pydantic==2.5.2
 Requires-Dist: pandas==2.1.3
 Requires-Dist: Biopython==1.83
 Requires-Dist: cyvcf2
 Requires-Dist: pysam
 Requires-Dist: pyyaml
+Requires-Dist: requests
 Provides-Extra: dev
 Requires-Dist: pylint~=3.0.2; extra == "dev"
 Requires-Dist: black~=23.11.0; extra == "dev"
 Requires-Dist: isort~=5.12.0; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest-cov~=4.1.0; extra == "test"
```

### Comparing `bonsai-prp-0.7.1/README.md` & `bonsai_prp-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `bonsai-prp-0.7.1/bonsai_prp.egg-info/PKG-INFO` & `bonsai_prp-0.8.0/bonsai_prp.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bonsai-prp
-Version: 0.7.1
+Version: 0.8.0
 Summary: Pipline result processing program for the JASEN pipeline and Bonsai tool.
 Author-email: Markus Johansson <markus.h.johansson@skane.se>, Ryan Kennedy <Ryan.Kennedy@skane.se>
 Project-URL: Repository, https://github.com/Clinical-Genomics-Lund/
 Project-URL: Issues, https://github.com/Clinical-Genomics-Lund/bonsai-prp/issues
 Project-URL: Changelog, https://github.com/Clinical-Genomics-Lund/CHANGELOG.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
@@ -21,14 +21,15 @@
 Requires-Dist: click==8.1.7
 Requires-Dist: pydantic==2.5.2
 Requires-Dist: pandas==2.1.3
 Requires-Dist: Biopython==1.83
 Requires-Dist: cyvcf2
 Requires-Dist: pysam
 Requires-Dist: pyyaml
+Requires-Dist: requests
 Provides-Extra: dev
 Requires-Dist: pylint~=3.0.2; extra == "dev"
 Requires-Dist: black~=23.11.0; extra == "dev"
 Requires-Dist: isort~=5.12.0; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest-cov~=4.1.0; extra == "test"
```

### Comparing `bonsai-prp-0.7.1/bonsai_prp.egg-info/SOURCES.txt` & `bonsai_prp-0.8.0/bonsai_prp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bonsai-prp-0.7.1/prp/cli.py` & `bonsai_prp-0.8.0/prp/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """Definition of the PRP command-line interface."""
-from prp import VERSION as __version__
-
 import json
 import logging
 from pathlib import Path
 from typing import List
 
 import click
+import numpy as np
 import pandas as pd
 import pysam
 from cyvcf2 import VCF, Writer
 from pydantic import TypeAdapter, ValidationError
 
+from prp import VERSION as __version__
+
 from .models.metadata import SoupType, SoupVersion
 from .models.phenotype import ElementType
 from .models.qc import QcMethodIndex, QcSoftware
 from .models.sample import MethodIndex, PipelineResult, ReferenceGenome
 from .models.typing import TypingMethod
 from .parse import (
     load_variants,
@@ -32,17 +33,16 @@
     parse_resfinder_amr_pred,
     parse_serotypefinder_oh_typing,
     parse_tbprofiler_amr_pred,
     parse_tbprofiler_lineage_results,
     parse_virulencefinder_stx_typing,
     parse_virulencefinder_vir_pred,
 )
-from .parse.mapping import get_reference_seq_accnr
 from .parse.metadata import get_database_info, get_gb_genome_version, parse_run_info
-from .parse.utils import get_db_version
+from .parse.utils import _get_path, get_db_version, parse_input_dir
 from .parse.variant import annotate_delly_variants
 
 logging.basicConfig(
     level=logging.INFO, format="[%(asctime)s] %(levelname)s in %(module)s: %(message)s"
 )
 LOG = logging.getLogger(__name__)
 
@@ -56,98 +56,100 @@
 
 
 @cli.command()
 @click.option("-i", "--sample-id", required=True, help="Sample identifier")
 @click.option(
     "-u",
     "--run-metadata",
-    type=click.File(),
+    type=click.Path(),
     required=True,
     help="Analysis metadata from the pipeline in json format",
 )
-@click.option("-q", "--quast", type=click.File(), help="Quast quality control metrics")
+@click.option("-q", "--quast", type=click.Path(), help="Quast quality control metrics")
 @click.option(
     "-d",
     "--process-metadata",
-    type=click.File(),
+    type=click.Path(),
     multiple=True,
     help="Nextflow processes metadata from the pipeline in json format",
 )
 @click.option(
-    "-k", "--kraken", type=click.File(), help="Kraken species annotation results"
+    "-k", "--kraken", type=click.Path(), help="Kraken species annotation results"
 )
 @click.option(
     "-a",
     "--amrfinder",
     type=click.Path(),
     help="amrfinderplus anti-microbial resistance results",
 )
-@click.option("-m", "--mlst", type=click.File(), help="MLST prediction results")
-@click.option("-c", "--cgmlst", type=click.File(), help="cgMLST prediction results")
+@click.option("-m", "--mlst", type=click.Path(), help="MLST prediction results")
+@click.option("-c", "--cgmlst", type=click.Path(), help="cgMLST prediction results")
 @click.option(
     "-v",
     "--virulencefinder",
     type=click.Path(),
     help="Virulence factor prediction results",
 )
 @click.option(
     "-r",
     "--resfinder",
-    type=click.File(),
+    type=click.Path(),
     help="Resfinder resistance prediction results",
 )
 @click.option(
     "-s",
     "--serotypefinder",
     type=click.Path(),
     help="Serotypefinder serotype prediction results",
 )
-@click.option("-p", "--quality", type=click.File(), help="postalignqc qc results")
-@click.option("-k", "--mykrobe", type=click.File(), help="mykrobe results")
-@click.option("-t", "--tbprofiler", type=click.File(), help="tbprofiler results")
+@click.option("-p", "--quality", type=click.Path(), help="postalignqc qc results")
+@click.option("-k", "--mykrobe", type=click.Path(), help="mykrobe results")
+@click.option("-t", "--tbprofiler", type=click.Path(), help="tbprofiler results")
+@click.option("--bam", type=click.Path(), help="Read mapping to reference genome")
 @click.option(
     "--reference-genome-fasta", type=click.Path(), help="reference genome fasta file"
 )
 @click.option(
     "--reference-genome-gff", type=click.Path(), help="reference-genome in gff format"
 )
 @click.option(
     "--genome-annotation",
     type=click.Path(),
     multiple=True,
-    help="Genome annotaitons bed format",
+    help="Genome annotations bed format",
 )
-@click.option("--bam", type=click.Path(), help="Read mapping to reference genome")
 @click.option("--snv-vcf", type=click.Path(), help="VCF with SNV variants")
 @click.option("--sv-vcf", type=click.Path(), help="VCF with SV variants")
+@click.option("--symlink_dir", type=click.Path(), help="Dir for symlink")
 @click.option("--correct_alleles", is_flag=True, help="Correct alleles")
 @click.option(
-    "-o", "--output", required=True, type=click.File("w"), help="output filepath"
+    "-o", "--output", required=True, type=click.Path(), help="output filepath"
 )
 def create_bonsai_input(
     sample_id,
     run_metadata,
     quast,
     process_metadata,
     kraken,
+    amrfinder,
     mlst,
     cgmlst,
     virulencefinder,
-    amrfinder,
     resfinder,
     serotypefinder,
     quality,
     mykrobe,
     tbprofiler,
     bam,
     reference_genome_fasta,
     reference_genome_gff,
     genome_annotation,
     snv_vcf,
     sv_vcf,
+    symlink_dir,
     correct_alleles,
     output,
 ):  # pylint: disable=too-many-arguments
     """Combine pipeline results into a standardized json output file."""
     LOG.info("Start generating pipeline result json")
     results = {
         "run_metadata": {
@@ -177,24 +179,25 @@
         LOG.info("Parse cgmlst results")
         res: MethodIndex = parse_cgmlst_results(cgmlst, correct_alleles=correct_alleles)
         results["typing_result"].append(res)
 
     # resfinder of different types
     if resfinder:
         LOG.info("Parse resistance results")
-        pred_res = json.load(resfinder)
-        methods = [
-            ElementType.AMR,
-            ElementType.STRESS,
-        ]
-        for method in methods:
-            res: MethodIndex = parse_resfinder_amr_pred(pred_res, method)
-            # exclude empty results from output
-            if len(res.result.genes) > 0 and len(res.result.variants) > 0:
-                results["element_type_result"].append(res)
+        with open(resfinder, "r", encoding="utf-8") as resfinder_json:
+            pred_res = json.load(resfinder_json)
+            methods = [
+                ElementType.AMR,
+                ElementType.STRESS,
+            ]
+            for method in methods:
+                res: MethodIndex = parse_resfinder_amr_pred(pred_res, method)
+                # exclude empty results from output
+                if len(res.result.genes) > 0 and len(res.result.variants) > 0:
+                    results["element_type_result"].append(res)
 
     # amrfinder
     if amrfinder:
         LOG.info("Parse amr results")
         methods = [
             ElementType.AMR,
             ElementType.STRESS,
@@ -235,14 +238,15 @@
     # mycobacterium tuberculosis
     # mykrobe
     if mykrobe:
         LOG.info("Parse mykrobe results")
         pred_res = pd.read_csv(mykrobe, quotechar='"')
         pred_res.columns.values[3] = "variants"
         pred_res.columns.values[4] = "genes"
+        pred_res.replace(["NA", np.nan], None, inplace=True)
         pred_res = pred_res.to_dict(orient="records")
 
         # verify that sample id is in prediction result
         if not sample_id in pred_res[0]["sample"]:
             LOG.warning(
                 "Sample id %s is not in Mykrobe result, possible sample mixup",
                 sample_id,
@@ -267,84 +271,119 @@
         )
         if lin_res is not None:
             results["typing_result"].append(lin_res)
 
     # tbprofiler
     if tbprofiler:
         LOG.info("Parse tbprofiler results")
-        pred_res = json.load(tbprofiler)
-        db_info: List[SoupVersion] = []
-        db_info = [
-            SoupVersion(
-                name=pred_res["db_version"]["name"],
-                version=get_db_version(pred_res["db_version"]),
-                type=SoupType.DB,
+        with open(tbprofiler, "r", encoding="utf-8") as tbprofiler_json:
+            pred_res = json.load(tbprofiler_json)
+            db_info: List[SoupVersion] = []
+            db_info = [
+                SoupVersion(
+                    name=pred_res["pipeline"]["db_version"]["name"],
+                    version=get_db_version(pred_res["pipeline"]["db_version"]),
+                    type=SoupType.DB,
+                )
+            ]
+            results["run_metadata"]["databases"].extend(db_info)
+            lin_res: MethodIndex = parse_tbprofiler_lineage_results(
+                pred_res, TypingMethod.LINEAGE
             )
-        ]
-        results["run_metadata"]["databases"].extend(db_info)
-        lin_res: MethodIndex = parse_tbprofiler_lineage_results(
-            pred_res, TypingMethod.LINEAGE
-        )
-        results["typing_result"].append(lin_res)
-        amr_res: MethodIndex = parse_tbprofiler_amr_pred(pred_res, ElementType.AMR)
-        results["element_type_result"].append(amr_res)
+            results["typing_result"].append(lin_res)
+            amr_res: MethodIndex = parse_tbprofiler_amr_pred(pred_res, ElementType.AMR)
+            results["element_type_result"].append(amr_res)
 
     # parse SNV and SV variants.
     if snv_vcf:
         results["snv_variants"] = load_variants(snv_vcf)
 
     if sv_vcf:
         results["sv_variants"] = load_variants(sv_vcf)
 
     # entries for reference genome and read mapping
     if all([bam, reference_genome_fasta, reference_genome_gff]):
         # verify that everything pertains to the same reference genome
-        bam_ref_genome = get_reference_seq_accnr(bam)
-        ref_accession, ref_name = get_gb_genome_version(reference_genome_gff)
-        if ref_accession != bam_ref_genome:
-            raise click.UsageError(
-                f"Read mapping used as different reference genome; bam accnr: {bam_ref_genome}; gbff accnr: {ref_accession}"
-            )
-
+        ref_accession, ref_name = get_gb_genome_version(reference_genome_fasta)
         # store file names
-        fasta_idx_path = Path(f"{reference_genome_fasta}.fai")
+        fasta_idx_path = fasta_idx_path = Path(f"{reference_genome_fasta}.fai")
         results["reference_genome"] = ReferenceGenome(
             name=ref_name,
             accession=ref_accession,
             fasta=Path(reference_genome_fasta).name,
             fasta_index=fasta_idx_path.name if fasta_idx_path.is_file() else None,
-            genes=reference_genome_gff,
+            genes=Path(reference_genome_gff).name,
         )
-        results["read_mapping"] = bam
+        results["read_mapping"] = _get_path(symlink_dir, "bam", bam)
         # add annotations
         annotations = [
             {"name": f"annotation_{i}", "file": Path(annot).name}
             for i, annot in enumerate(genome_annotation, start=1)
         ]
         for vcf in [sv_vcf, snv_vcf]:
             if vcf:
+                vcf = _get_path(symlink_dir, "vcf", vcf)
                 name = "SNV" if vcf == sv_vcf else "SV"
-                annotations.append({"name": name, "file": Path(vcf).name})
+                annotations.append({"name": name, "file": vcf})
         # store annotation results
-        results["genome_annotation"] = annotations if len(annotations) > 0 else None
+        results["genome_annotation"] = annotations if annotations else None
 
     try:
         output_data = PipelineResult(
             sample_id=sample_id, schema_version=OUTPUT_SCHEMA_VERSION, **results
         )
     except ValidationError as err:
         click.secho("Input failed Validation", fg="red")
         click.secho(err)
         raise click.Abort
-    LOG.info("Storing results to: %s", output.name)
-    output.write(output_data.model_dump_json(indent=2))
+    LOG.info("Storing results to: %s", output)
+    with open(output, "w", encoding="utf-8") as fout:
+        fout.write(output_data.model_dump_json(indent=2))
     click.secho("Finished generating pipeline output", fg="green")
 
 
 @cli.command()
+@click.option(
+    "-i",
+    "--input-dir",
+    required=True,
+    type=click.Path(exists=True, file_okay=False, dir_okay=True),
+    help="Input directory to JASEN's outdir incl. speciesDir",
+)
+@click.option(
+    "-j",
+    "--jasen-dir",
+    required=True,
+    type=click.Path(exists=True, file_okay=False, dir_okay=True),
+    help="Path to JASEN directory",
+)
+@click.option(
+    "-s",
+    "--symlink_dir",
+    required=False,
+    type=click.Path(exists=True, file_okay=False, dir_okay=True),
+    help="Path to symlink directory",
+)
+@click.option(
+    "-o",
+    "--output-dir",
+    type=click.Path(file_okay=False, dir_okay=True),
+    help="Output directory to incl. speciesDir [default: input_dir]",
+)
+@click.pass_context
+def rerun_bonsai_input(ctx, input_dir, jasen_dir, symlink_dir, output_dir) -> None:
+    """Rerun bonsai input creation for all samples in input directory."""
+    if input_dir:
+        LOG.info("Parse input directory")
+        input_arrays = parse_input_dir(input_dir, jasen_dir, symlink_dir, output_dir)
+        for input_array in input_arrays:
+            ctx.invoke(create_bonsai_input, **input_array)
+
+
+@cli.command()
 def print_schema():
     """Print Pipeline result output format schema."""
     click.secho(PipelineResult.schema_json(indent=2))
 
 
 @cli.command()
 @click.option("-o", "--output", required=True, type=click.File("r"))
@@ -357,17 +396,17 @@
         click.secho("Invalid file format X", fg="red")
         click.secho(err)
     else:
         click.secho(f'The file "{output.name}" is valid', fg="green")
 
 
 @cli.command()
-@click.option("-q", "--quast", type=click.File(), help="Quast quality control metrics")
-@click.option("-p", "--quality", type=click.File(), help="postalignqc qc results")
-@click.option("-c", "--cgmlst", type=click.File(), help="cgMLST prediction results")
+@click.option("-q", "--quast", type=click.Path(), help="Quast quality control metrics")
+@click.option("-p", "--quality", type=click.Path(), help="postalignqc qc results")
+@click.option("-c", "--cgmlst", type=click.Path(), help="cgMLST prediction results")
 @click.option("--correct_alleles", is_flag=True, help="Correct alleles")
 @click.option(
     "-o", "--output", required=True, type=click.File("w"), help="output filepath"
 )
 def create_cdm_input(quast, quality, cgmlst, correct_alleles, output) -> None:
     """Format QC metrics into CDM compatible input file."""
     results = []
@@ -416,15 +455,19 @@
     click.secho("Finished generating QC output", fg="green")
 
 
 @cli.command()
 @click.option("-v", "--vcf", type=click.Path(exists=True), help="VCF file")
 @click.option("-b", "--bed", type=click.Path(exists=True), help="BED file")
 @click.option(
-    "-o", "--output", required=True, type=click.Path(writable=True), help="output filepath"
+    "-o",
+    "--output",
+    required=True,
+    type=click.Path(writable=True),
+    help="output filepath",
 )
 def annotate_delly(vcf, bed, output):
     """Annotate Delly SV varinats with genes in BED file."""
     output = Path(output)
     # load annotation
     if bed is not None:
         annotation = pysam.TabixFile(bed, parser=pysam.asTuple())
@@ -433,15 +476,19 @@
 
     vcf_obj = VCF(vcf)
     variant = next(vcf_obj)
     annot_chrom = False
     if not variant.CHROM in annotation.contigs:
         if len(annotation.contigs) > 1:
             raise click.UsageError(
-                f'"{variant.CHROM}" not in BED file and the file contains {len(annotation.contigs)} chromosomes'
+                (
+                    f'"{variant.CHROM}" not in BED file'
+                    " and the file contains "
+                    f"{len(annotation.contigs)} chromosomes"
+                )
             )
         # if there is only one "chromosome" in the bed file
         annot_chrom = True
         LOG.warning("Annotating variant chromosome to %s", annotation.contigs[0])
     # reset vcf file
     vcf_obj = VCF(vcf)
     vcf_obj.add_info_to_header(
```

### Comparing `bonsai-prp-0.7.1/prp/models/metadata.py` & `bonsai_prp-0.8.0/prp/models/metadata.py`

 * *Files identical despite different names*

### Comparing `bonsai-prp-0.7.1/prp/models/phenotype.py` & `bonsai_prp-0.8.0/prp/models/phenotype.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,15 @@
     resistance_level: str | None = None
     # how was the annotation made
     annotation_type: AnnotationType = Field(..., description="Annotation type")
     annotation_author: str | None = Field(None, description="Annotation author")
     # what information substansiate the annotation
     reference: List[str] = Field([], description="References supporting trait")
     note: str | None = Field(None, description="Note, can be used for confidence score")
+    source: str | None = Field(None, description="Source of variant")
 
 
 class DatabaseReference(RWModel):
     """Refernece to a database."""
 
     ref_database: Optional[str] = None
     ref_id: Optional[str] = None
```

### Comparing `bonsai-prp-0.7.1/prp/models/qc.py` & `bonsai_prp-0.8.0/prp/models/qc.py`

 * *Files identical despite different names*

### Comparing `bonsai-prp-0.7.1/prp/models/sample.py` & `bonsai_prp-0.8.0/prp/models/sample.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 class ReferenceGenome(RWModel):
     """Reference genome."""
 
     name: str
     accession: str
     fasta: str
-    fasta_index: str
+    fasta_index: Optional[str] = None
     genes: str
 
 
 class PipelineResult(SampleBase):
     """Input format of sample object from pipeline."""
 
     schema_version: int = Field(..., alias="schemaVersion", gt=0)
```

### Comparing `bonsai-prp-0.7.1/prp/models/species.py` & `bonsai_prp-0.8.0/prp/models/species.py`

 * *Files identical despite different names*

### Comparing `bonsai-prp-0.7.1/prp/models/tags.py` & `bonsai_prp-0.8.0/prp/models/tags.py`

 * *Files identical despite different names*

### Comparing `bonsai-prp-0.7.1/prp/models/typing.py` & `bonsai_prp-0.8.0/prp/models/typing.py`

 * *Files 14% similar despite different names*

```diff
@@ -88,16 +88,26 @@
     n_novel: int = Field(0, alias="nNovel")
     n_missing: int = Field(0, alias="nNovel")
 
 
 class TypingResultLineage(ResultLineageBase):
     """Lineage results"""
 
+    lineage_depth: float | None = None
     main_lin: str
     sublin: str
 
 
+class TypingResultPhylogenetics(TypingResultLineage):
+    """Phylogenetics results"""
+
+    phylo_group_depth: float | None = None
+    phylo_group: str | None = None
+    species_depth: float | None = None
+    species: str | None = None
+
+
 class TypingResultGeneAllele(VirulenceGene, SerotypeGene):
     """Identification of individual gene alleles."""
 
 
 CgmlstAlleles = Dict[str, int | None | ChewbbacaErrors | MlstErrors | List[int]]
```

### Comparing `bonsai-prp-0.7.1/prp/parse/__init__.py` & `bonsai_prp-0.8.0/prp/parse/__init__.py`

 * *Files identical despite different names*

### Comparing `bonsai-prp-0.7.1/prp/parse/metadata.py` & `bonsai_prp-0.8.0/prp/parse/metadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 """Parse metadata passed to pipeline."""
 import json
 import logging
-from typing import List, TextIO
+from typing import List
 
 from Bio import SeqIO
 
 from ..models.metadata import RunInformation, SoupVersion
 
 LOG = logging.getLogger(__name__)
 
 
-def get_database_info(process_metadata: List[TextIO]) -> List[SoupVersion]:
+def get_database_info(process_metadata: List[str]) -> List[SoupVersion]:
     """Get database or software information.
 
     :param process_metadata: List of file objects for db records.
-    :type process_metadata: List[TextIO]
+    :type process_metadata: List[str]
     :return: Description of software or database version.
     :rtype: List[SoupVersion]
     """
     db_info = []
-    for soup in process_metadata:
-        dbs = json.load(soup)
-        if isinstance(dbs, (list, tuple)):
-            for db in dbs:
-                db_info.append(SoupVersion(**db))
-        else:
-            db_info.append(SoupVersion(**dbs))
+    for soup_filepath in process_metadata:
+        with open(soup_filepath, "r", encoding="utf-8") as soup:
+            dbs = json.load(soup)
+            if isinstance(dbs, (list, tuple)):
+                for db in dbs:
+                    db_info.append(SoupVersion(**db))
+            else:
+                db_info.append(SoupVersion(**dbs))
     return db_info
 
 
-def parse_run_info(run_metadata: TextIO) -> RunInformation:
+def parse_run_info(run_metadata: str) -> RunInformation:
     """Parse nextflow analysis information
 
     :param run_metadata: Nextflow analysis metadata in json format.
-    :type run_metadata: TextIO
+    :type run_metadata: str
     :return: Analysis metadata record.
     :rtype: RunMetadata
     """
     LOG.info("Parse run metadata.")
-    run_info = RunInformation(**json.load(run_metadata))
+    with open(run_metadata, encoding="utf-8") as jsonfile:
+        run_info = RunInformation(**json.load(jsonfile))
     return run_info
 
 
-def get_gb_genome_version(gff_path: str) -> str:
+def get_gb_genome_version(fasta_path: str) -> str:
     """Retrieve genbank genome version"""
-    handler = SeqIO.parse(gff_path, "gb")
-    record = next(handler.records)
-    return record.id, record.description
+    record = next(SeqIO.parse(fasta_path, "fasta"))
+    return record.id, record.description.rstrip(", complete genome")
```

### Comparing `bonsai-prp-0.7.1/prp/parse/phenotype/amrfinder.py` & `bonsai_prp-0.8.0/prp/parse/phenotype/amrfinder.py`

 * *Files identical despite different names*

### Comparing `bonsai-prp-0.7.1/prp/parse/phenotype/mykrobe.py` & `bonsai_prp-0.8.0/prp/parse/phenotype/mykrobe.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
                 annotation_type=AnnotationType.TOOL,
                 annotation_author=Software.MYKROBE.value,
             )
         ]
 
         variants = element_type["variants"].split(";")
         # Mykrobe CSV variant format
-        # <gene>_<amino acid change>-<dna change>:<ref depth>:<alt depth>:<genotype confidence>
+        # <gene>_<aa change>-<nt change>:<ref depth>:<alt depth>:<gt confidence>
         # ref: https://github.com/Mykrobe-tools/mykrobe/wiki/AMR-prediction-output
         pattern = re.compile(r"(.+)_(.+)-(.+):(\d+):(\d+):(\d+)", re.I)
         for var_id, variant in enumerate(variants, start=1):
             # extract variant info using regex
             match = re.search(pattern, variant)
             gene, aa_change, dna_change, ref_depth, alt_depth, conf = match.groups()
```

### Comparing `bonsai-prp-0.7.1/prp/parse/phenotype/resfinder.py` & `bonsai_prp-0.8.0/prp/parse/phenotype/resfinder.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,26 +291,24 @@
         prediction_method = exec_info["parameters"]["method"]
 
     # parse prediction result
     results = []
     for var_id, info in enumerate(resfinder_result["seq_variations"].values(), start=1):
         # Get only variants from desired phenotypes
         if limit_to_phenotypes is not None:
-            intersect = set(info["phenotypes"]) & set(limit_to_phenotypes)
-            if len(intersect) == 0:
+            if len(set(info["phenotypes"]) & set(limit_to_phenotypes)) == 0:
                 continue
         # get gene depth
         if "seq_regions" in resfinder_result:
             info["depth"] = resfinder_result["seq_regions"][info["seq_regions"][0]][
                 "depth"
             ]
         else:
             info["depth"] = 0
         # translate variation type bools into classifier
-        var_type = VariantType.SNV
         if info["substitution"]:
             var_sub_type = VariantSubType.SUBSTITUTION
         elif info["insertion"]:
             var_sub_type = VariantSubType.INSERTION
         elif info["deletion"]:
             var_sub_type = VariantSubType.DELETION
         else:
@@ -327,15 +325,15 @@
                 name=phe,
                 annotation_type=AnnotationType.TOOL,
             )
             for phe in info["phenotypes"]
         ]
         variant = ResfinderVariant(
             id=var_id,
-            variant_type=var_type,
+            variant_type=VariantType.SNV,
             variant_subtype=var_sub_type,
             phenotypes=phenotype,
             # position
             reference_sequence=gene_symbol,
             accession=gene_accnr,
             start=info["ref_start_pos"],
             end=info["ref_end_pos"],
```

### Comparing `bonsai-prp-0.7.1/prp/parse/phenotype/serotypefinder.py` & `bonsai_prp-0.8.0/prp/parse/phenotype/serotypefinder.py`

 * *Files identical despite different names*

### Comparing `bonsai-prp-0.7.1/prp/parse/phenotype/tbprofiler.py` & `bonsai_prp-0.8.0/prp/parse/phenotype/tbprofiler.py`

 * *Files 17% similar despite different names*

```diff
@@ -47,23 +47,23 @@
     susceptible = [drug for drug in drugs if drug not in resistant]
     return {"susceptible": list(susceptible), "resistant": list(resistant)}
 
 
 def _parse_tbprofiler_amr_variants(predictions) -> Tuple[TbProfilerVariant, ...]:
     """Get resistance genes from tbprofiler result."""
     variant_caller = None
-    for prog in predictions["pipeline"]:
-        if prog["Analysis"].lower() == "variant calling":
-            variant_caller = prog["Program"]
+    for prog in predictions["pipeline"]["software"]:
+        if prog["process"].lower() == "variant_calling":
+            variant_caller = prog["software"]
     results = []
 
     # tbprofiler report three categories of variants
     # - dr_variants: known resistance variants
     # - qc_fail_variants: known resistance variants failing qc
-    # - other_variants: variants not in the database but in genes 
+    # - other_variants: variants not in the database but in genes
     #                   associated with resistance
     var_id = 1
     for result_type in ["dr_variants", "other_variants", "qc_fail_variants"]:
         # associated with passed/ failed qc
         if result_type == "qc_fail_variants":
             passed_qc = False
         else:
@@ -77,23 +77,23 @@
             if len(ref_nt) == len(alt_nt):
                 var_sub_type = VariantSubType.SUBSTITUTION
             elif len(ref_nt) > len(alt_nt):
                 var_sub_type = VariantSubType.DELETION
             else:
                 var_sub_type = VariantSubType.INSERTION
 
-            start_pos = int(hit["genome_pos"])
+            start_pos = int(hit["pos"])
             variant = TbProfilerVariant(
                 # classificatoin
                 id=var_id,
                 variant_type=var_type,
                 variant_subtype=var_sub_type,
-                phenotypes=parse_drug_resistance_info(hit.get("drugs", [])),
+                phenotypes=parse_drug_resistance_info(hit.get("annotation", [])),
                 # location
-                reference_sequence=hit["gene"],
+                reference_sequence=hit["gene_name"],
                 accession=hit["feature_id"],
                 start=start_pos,
                 end=start_pos + len(alt_nt),
                 ref_nt=ref_nt,
                 alt_nt=alt_nt,
                 # consequense
                 variant_effect=hit["type"],
@@ -121,33 +121,37 @@
     :type drugs: List[Dict[str, str]]
     :return: Formatted phenotype info
     :rtype: List[PhenotypeInfo]
     """
     phenotypes = []
     for drug in drugs:
         # assign element type
-        if drug["type"] == "drug" and drug["confers"] == "resistance":
+        if drug["type"] == "drug_resistance" or drug["type"] == "who_confidence":
             drug_type = ElementType.AMR
         else:
             drug_type = ElementType.AMR
-            LOG.warning(
-                "Unknown TbProfiler drug; drug: %s, confers: %s; default to %s",
+            LOG.warning((
+                "Unknown TbProfiler drug; drug: %s"
+                ", confers resistance with confidence"
+                ": %s; default to %s"
+            ),
                 drug["type"],
-                drug["confers"],
+                drug["confidence"],
                 drug_type,
             )
-        reference = drug.get("literature")
+        reference = drug.get("comment")
         phenotypes.append(
             PhenotypeInfo(
                 name=drug["drug"],
                 type=drug_type,
                 reference=[] if reference is None else [reference],
                 annotation_type=AnnotationType.TOOL,
                 annotation_author=Software.TBPROFILER.value,
-                note=drug.get("who confidence"),
+                note=drug.get("confidence"),
+                source=drug.get("source"),
             )
         )
     return phenotypes
 
 
 def parse_tbprofiler_amr_pred(
     prediction: Dict[str, Any], resistance_category
```

### Comparing `bonsai-prp-0.7.1/prp/parse/phenotype/virulencefinder.py` & `bonsai_prp-0.8.0/prp/parse/phenotype/virulencefinder.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         if key == "stx":
             continue
         # assign element subtype
         virulence_group = key.split("_")[1] if "_" in key else key
         match virulence_group:
             case "toxin":
                 subtype = ElementVirulenceSubtype.TOXIN
-            case other:
+            case _:
                 subtype = ElementVirulenceSubtype.VIR
         # parse genes
         if not genes == "No hit found":
             for gene in genes.values():
                 vir_genes.append(parse_vir_gene(gene, subtype))
     # sort genes
     genes = sorted(vir_genes, key=lambda entry: (entry.gene_symbol, entry.coverage))
```

### Comparing `bonsai-prp-0.7.1/prp/parse/qc.py` & `bonsai_prp-0.8.0/prp/parse/qc.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,15 +110,17 @@
         """Check if reads are paired"""
         bam_file = pysam.AlignmentFile(self.bam)
         for i, read in enumerate(bam_file):
             if read.is_paired:
                 return True
             if i >= 1000:
                 break
-        # If no paired reads are found in the first 1000 reads or read is None, return False
+        # If no paired reads are found in the
+        # first 1000 reads or read is None
+        # return False
         return False
 
     def system_p(self, cmd: list) -> None:
         """Execute subprocess"""
         LOG.info("RUNNING: %s", " ".join(cmd))
         result = subprocess.run(cmd, check=True, text=True)
         if result.stderr:
@@ -233,64 +235,72 @@
         self.results["n_dup_reads"] = n_dup_reads
         self.results["dup_pct"] = n_dup_reads / n_mapped_reads
         self.results["sample_id"] = self.sample_id
 
         return self.results
 
 
-def parse_quast_results(file: File) -> QcMethodIndex:
+def parse_quast_results(tsv_fpath: str) -> QcMethodIndex:
     """Parse quast file and extract relevant metrics.
 
     Args:
         sep (str): seperator
 
     Returns:
         QuastQcResult: list of key-value pairs
     """
-    LOG.info("Parsing tsv file: %s", file.name)
-    creader = csv.reader(file, delimiter="\t")
-    header = next(creader)
-    raw = [dict(zip(header, row)) for row in creader]
-    qc_res = QuastQcResult(
-        total_length=int(raw[0]["Total length"]),
-        reference_length=raw[0]["Reference length"],
-        largest_contig=raw[0]["Largest contig"],
-        n_contigs=raw[0]["# contigs"],
-        n50=raw[0]["N50"],
-        assembly_gc=raw[0]["GC (%)"],
-        reference_gc=raw[0]["Reference GC (%)"],
-        duplication_ratio=raw[0]["Duplication ratio"],
-    )
+    LOG.info("Parsing tsv file: %s", tsv_fpath)
+    with open(tsv_fpath, "r", encoding="utf-8") as tsvfile:
+        creader = csv.reader(tsvfile, delimiter="\t")
+        header = next(creader)
+        raw = [dict(zip(header, row)) for row in creader]
+        qc_res = QuastQcResult(
+            total_length=int(raw[0]["Total length"]),
+            reference_length=raw[0]["Reference length"],
+            largest_contig=raw[0]["Largest contig"],
+            n_contigs=raw[0]["# contigs"],
+            n50=raw[0]["N50"],
+            assembly_gc=raw[0]["GC (%)"],
+            reference_gc=raw[0]["Reference GC (%)"],
+            duplication_ratio=raw[0]["Duplication ratio"],
+        )
     return QcMethodIndex(software=QcSoftware.QUAST, result=qc_res)
 
 
-def parse_postalignqc_results(input_file: File) -> QcMethodIndex:
+def parse_postalignqc_results(postalignqc_fpath: str) -> QcMethodIndex:
     """Parse postalignqc json file and extract relevant metrics.
 
     Args:
         sep (str): seperator
 
     Returns:
         PostAlignQc: list of key-value pairs
     """
-    LOG.info("Parsing json file: %s", input_file.name)
-    qc_dict = json.load(input_file)
-    qc_res = PostAlignQcResult(
-        ins_size=None if "ins_size" not in qc_dict else int(float(qc_dict["ins_size"])),
-        ins_size_dev=None if "ins_size_dev" not in qc_dict else int(float(qc_dict["ins_size_dev"])),
-        mean_cov=int(qc_dict["mean_cov"]),
-        pct_above_x=qc_dict["pct_above_x"],
-        n_reads=int(qc_dict["n_reads"]),
-        n_mapped_reads=int(qc_dict["n_mapped_reads"]),
-        n_read_pairs=int(qc_dict["n_read_pairs"]),
-        coverage_uniformity=float(qc_dict["coverage_uniformity"]) if qc_dict.get("coverage_uniformity") is not None else None,
-        quartile1=float(qc_dict["quartile1"]),
-        median_cov=float(qc_dict["median_cov"]),
-        quartile3=float(qc_dict["quartile3"]),
-    )
+    LOG.info("Parsing json file: %s", postalignqc_fpath)
+    with open(postalignqc_fpath, "r", encoding="utf-8") as jsonfile:
+        qc_dict = json.load(jsonfile)
+        qc_res = PostAlignQcResult(
+            ins_size=None
+            if "ins_size" not in qc_dict
+            else int(float(qc_dict["ins_size"])),
+            ins_size_dev=None
+            if "ins_size_dev" not in qc_dict
+            else int(float(qc_dict["ins_size_dev"])),
+            mean_cov=int(qc_dict["mean_cov"]),
+            pct_above_x=qc_dict["pct_above_x"],
+            n_reads=int(qc_dict["n_reads"]),
+            n_mapped_reads=int(qc_dict["n_mapped_reads"]),
+            n_read_pairs=int(qc_dict["n_read_pairs"]),
+            coverage_uniformity=float(qc_dict["coverage_uniformity"])
+            if qc_dict.get("coverage_uniformity") is not None
+            else None,
+            quartile1=float(qc_dict["quartile1"]),
+            median_cov=float(qc_dict["median_cov"]),
+            quartile3=float(qc_dict["quartile3"]),
+        )
     return QcMethodIndex(software=QcSoftware.POSTALIGNQC, result=qc_res)
 
 
 def parse_alignment_results(
     sample_id: str,
     bam: File,
     reference: File,
```

### Comparing `bonsai-prp-0.7.1/prp/parse/typing.py` & `bonsai_prp-0.8.0/prp/parse/typing.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 from ..models.sample import MethodIndex
 from ..models.typing import (
     LineageInformation,
     TypingMethod,
     TypingResultCgMlst,
     TypingResultGeneAllele,
-    TypingResultLineage,
     TypingResultMlst,
+    TypingResultPhylogenetics,
 )
 from ..models.typing import TypingSoftware as Software
 from .phenotype.serotypefinder import parse_serotype_gene
 from .phenotype.virulencefinder import parse_vir_gene
 
 LOG = logging.getLogger(__name__)
 
@@ -33,35 +33,36 @@
     elif allele == "-":
         result = None
     else:
         raise ValueError(f"MLST allele {allele} not expected format")
     return result
 
 
-def parse_mlst_results(path: str) -> TypingResultMlst:
+def parse_mlst_results(mlst_fpath: str) -> TypingResultMlst:
     """Parse mlst results from mlst to json object."""
     LOG.info("Parsing mlst results")
-    result = json.load(path)[0]
-    result_obj = TypingResultMlst(
-        scheme=result["scheme"],
-        sequence_type=None
-        if result["sequence_type"] == "-"
-        else result["sequence_type"],
-        alleles={
-            gene: _process_allele_call(allele)
-            for gene, allele in result["alleles"].items()
-        },
-    )
+    with open(mlst_fpath, "r", encoding="utf-8") as jsonfile:
+        result = json.load(jsonfile)[0]
+        result_obj = TypingResultMlst(
+            scheme=result["scheme"],
+            sequence_type=None
+            if result["sequence_type"] == "-"
+            else result["sequence_type"],
+            alleles={
+                gene: _process_allele_call(allele)
+                for gene, allele in result["alleles"].items()
+            },
+        )
     return MethodIndex(
         type=TypingMethod.MLST, software=Software.MLST, result=result_obj
     )
 
 
 def parse_cgmlst_results(
-    file: str, include_novel_alleles: bool = True, correct_alleles: bool = False
+    chewbacca_res_path: str, include_novel_alleles: bool = True, correct_alleles: bool = False
 ) -> TypingResultCgMlst:
     """Parse chewbbaca cgmlst prediction results to json results.
 
     Chewbbaca reports errors in allele profile.
     See: https://github.com/B-UMMI/chewBBACA
     -------------------
     INF-<allele name>, inferred new allele
@@ -99,60 +100,81 @@
         return allele
 
     LOG.info(
         "Parsing cgmslt results, %s including novel alleles",
         "not" if not include_novel_alleles else "",
     )
 
-    creader = csv.reader(file, delimiter="\t")
-    _, *allele_names = (colname.rstrip(".fasta") for colname in next(creader))
-    # parse alleles
-    _, *alleles = next(creader)
+    with open(chewbacca_res_path, encoding='utf-8') as fileh:
+        creader = csv.reader(fileh, delimiter="\t")
+        _, *allele_names = (colname.rstrip(".fasta") for colname in next(creader))
+        # parse alleles
+        _, *alleles = next(creader)
     corrected_alleles = (replace_errors(a) for a in alleles)
     results = TypingResultCgMlst(
         n_novel=sum(1 for a in alleles if a.startswith("INF")),
         n_missing=sum(1 for a in alleles if a in errors),
         alleles=dict(zip(allele_names, corrected_alleles)),
     )
     return MethodIndex(
         type=TypingMethod.CGMLST, software=Software.CHEWBBACA, result=results
     )
 
 
-def parse_tbprofiler_lineage_results(pred_res: dict, method) -> TypingResultLineage:
+def parse_tbprofiler_lineage_results(
+    pred_res: dict, method
+) -> TypingResultPhylogenetics:
     """Parse tbprofiler results for lineage object."""
     LOG.info("Parsing lineage results")
-    result_obj = TypingResultLineage(
-        main_lin=pred_res["main_lin"],
-        sublin=pred_res["sublin"],
+    result_obj = TypingResultPhylogenetics(
+        phylo_group_depth=None,
+        species_depth=None,
+        lineage_depth=None,
+        phylo_group=None,
+        species=None,
+        main_lin=pred_res["main_lineage"],
+        sublin=pred_res["sub_lineage"],
         lineages=pred_res["lineage"],
     )
     return MethodIndex(type=method, software=Software.TBPROFILER, result=result_obj)
 
 
-def parse_mykrobe_lineage_results(pred_res: dict, method) -> TypingResultLineage | None:
+def parse_mykrobe_lineage_results(
+    pred_res: dict, method
+) -> TypingResultPhylogenetics | None:
     """Parse mykrobe results for lineage object."""
     LOG.info("Parsing lineage results")
-    if len(pred_res) > 0:
+    if pred_res:
         lineage = pred_res[0]
+        phylo_group_depth = lineage["phylo_group_depth"]
+        species_depth = lineage["species_depth"]
+        lineage_depth = lineage["lineage_depth"]
         split_lin = lineage["lineage"].split(".")
         main_lin = split_lin[0]
         sublin = lineage["lineage"]
         lin_idxs = lineage["lineage"].lstrip("lineage").split(".")
         lineages = [
             LineageInformation(lineage="lineage" + ".".join(lin_idxs[: idx + 1]))
             for idx in range(len(lin_idxs))
         ]
         # cast to lineage object
-        result_obj = TypingResultLineage(
+        result_obj = TypingResultPhylogenetics(
+            phylo_group_depth=float(phylo_group_depth)
+            if phylo_group_depth
+            else phylo_group_depth,
+            species_depth=float(species_depth) if species_depth else species_depth,
+            lineage_depth=float(lineage_depth) if lineage_depth else lineage_depth,
+            phylo_group=lineage["phylo_group"],
+            species=lineage["species"],
             main_lin=main_lin,
             sublin=sublin,
             lineages=lineages,
         )
         return MethodIndex(type=method, software=Software.MYKROBE, result=result_obj)
+    return None
 
 
 def parse_virulencefinder_stx_typing(path: str) -> MethodIndex | None:
     """Parse virulencefinder's output re stx typing"""
     with open(path, "rb") as inpt:
         pred_obj = json.load(inpt)
         # if has valid results
```

### Comparing `bonsai-prp-0.7.1/prp/parse/variant.py` & `bonsai_prp-0.8.0/prp/parse/variant.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 def _get_variant_type(variant) -> VariantType:
     """Parse variant type."""
     match variant.var_type:
         case "snp":
             var_type = VariantType.SNV
         case "mnp":
             var_type = VariantType.MNV
-        case other:
+        case _:
             var_type = VariantType(variant.var_type.upper())
     return var_type
 
 
 def parse_variant(variant: Variant, var_id: int, caller: str | None = None):
     """Parse variant info from VCF row."""
     # check if variant passed qc filtering
@@ -53,14 +53,15 @@
 
 
 def _get_variant_caller(vcf_obj: VCF) -> str | None:
     """Get source from VCF header to get variant caller sw if possible."""
     match = re.search(SOURCE_PATTERN, vcf_obj.raw_header)
     if match:
         return match.group(1)
+    return None
 
 
 def load_variants(variant_file: str) -> List[VariantBase]:
     """Load variants."""
     vcf_obj = VCF(variant_file)
     try:
         next(vcf_obj)
@@ -77,14 +78,15 @@
     for var_id, variant in enumerate(vcf_obj, start=1):
         variants.append(parse_variant(variant, var_id=var_id, caller=variant_caller))
 
     return variants
 
 
 def annotate_delly_variants(writer, vcf, annotation, annot_chrom=False):
+    """Annotate a variant called by Delly."""
     locus_tag = 3
     gene_symbol = 4
     # annotate variant
     n_annotated = 0
     for variant in vcf:
         # update chromosome
         if annot_chrom:
```

### Comparing `bonsai-prp-0.7.1/pyproject.toml` & `bonsai_prp-0.8.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,16 @@
     "wheel",
     "click==8.1.7",
     "pydantic==2.5.2",
     "pandas==2.1.3",
     "Biopython==1.83",
     "cyvcf2",
     "pysam",
-    "pyyaml"
+    "pyyaml",
+    "requests"
 ]
 
 [project.urls]
 Repository = "https://github.com/Clinical-Genomics-Lund/"
 Issues = "https://github.com/Clinical-Genomics-Lund/bonsai-prp/issues"
 Changelog = "https://github.com/Clinical-Genomics-Lund/CHANGELOG.md"
```

### Comparing `bonsai-prp-0.7.1/tests/test_cli.py` & `bonsai_prp-0.8.0/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,35 +133,33 @@
 def test_cdm_input_cmd(
     ecoli_quast_path, ecoli_bwa_path, ecoli_chewbbaca_path, ecoli_cdm_input
 ):
     """Test command for creating CDM input."""
     runner = CliRunner()
     with runner.isolated_filesystem():
         output_fname = "test_ouptut"
-        result = runner.invoke(
-            create_cdm_input,
-            [
+        args = [
                 "--quast",
                 ecoli_quast_path,
                 "--quality",
                 ecoli_bwa_path,
                 "--cgmlst",
                 ecoli_chewbbaca_path,
                 "--output",
                 output_fname,
-            ],
-        )
+            ]
+        result = runner.invoke(create_cdm_input, args)
 
         # test successful execution of command
         assert result.exit_code == 0
 
         # test correct output format
         with open(output_fname, "rb") as inpt:
-            cmd_output = json.load(inpt)
-            assert cmd_output == ecoli_cdm_input
+            cdm_output = json.load(inpt)
+            assert cdm_output == ecoli_cdm_input
 
 
 def test_annotate_delly(
     mtuberculosis_delly_bcf_path, converged_bed_path, annotated_delly_path
 ):
     """Test command for annotating delly output."""
     runner = CliRunner()
```

