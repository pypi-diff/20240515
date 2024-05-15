# Comparing `tmp/molpipeline-0.8.0.tar.gz` & `tmp/molpipeline-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molpipeline-0.8.0.tar", last modified: Thu Apr 25 16:14:53 2024, max compression
+gzip compressed data, was "molpipeline-0.8.1.tar", last modified: Wed May 15 12:19:02 2024, max compression
```

## Comparing `molpipeline-0.8.0.tar` & `molpipeline-0.8.1.tar`

### file list

```diff
@@ -1,140 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:14:53.580774 molpipeline-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-25 16:14:44.000000 molpipeline-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-25 16:14:53.580774 molpipeline-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-25 16:14:44.000000 molpipeline-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:14:53.564774 molpipeline-0.8.0/molpipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:14:53.564774 molpipeline-0.8.0/molpipeline/abstract_pipeline_elements/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/abstract_pipeline_elements/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:14:53.564774 molpipeline-0.8.0/molpipeline/abstract_pipeline_elements/any2mol/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/abstract_pipeline_elements/any2mol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/abstract_pipeline_elements/any2mol/string2mol.py
--rw-r--r--   0 runner    (1001) docker     (127)    23644 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/abstract_pipeline_elements/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:14:53.568774 molpipeline-0.8.0/molpipeline/abstract_pipeline_elements/mol2any/
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/abstract_pipeline_elements/mol2any/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12159 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/abstract_pipeline_elements/mol2any/mol2bitvector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6652 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/abstract_pipeline_elements/mol2any/mol2floatvector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/abstract_pipeline_elements/mol2any/mol2string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:14:53.568774 molpipeline-0.8.0/molpipeline/any2mol/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/any2mol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/any2mol/auto2mol.py
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/any2mol/bin2mol.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/any2mol/sdf2mol.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/any2mol/smiles2mol.py
--rw-r--r--   0 runner    (1001) docker     (127)    23790 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/error_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:14:53.568774 molpipeline-0.8.0/molpipeline/estimators/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/estimators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:14:53.568774 molpipeline-0.8.0/molpipeline/estimators/algorithm/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/estimators/algorithm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/estimators/algorithm/connected_component_clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/estimators/algorithm/union_find.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:14:53.568774 molpipeline-0.8.0/molpipeline/estimators/chemprop/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/estimators/chemprop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/estimators/chemprop/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    14929 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/estimators/chemprop/component_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8552 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/estimators/chemprop/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/estimators/chemprop/neural_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/estimators/connected_component_clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/estimators/leader_picker_clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     7775 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/estimators/murcko_scaffold_clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     7178 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/estimators/nearest_neighbor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/estimators/similarity_transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:14:53.568774 molpipeline-0.8.0/molpipeline/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/metrics/ignore_error_scorer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:14:53.572774 molpipeline-0.8.0/molpipeline/mol2any/
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/mol2any/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/mol2any/mol2bin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/mol2any/mol2chemprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     9175 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/mol2any/mol2concatinated_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/mol2any/mol2inchi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/mol2any/mol2morgan_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/mol2any/mol2net_charge.py
--rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/mol2any/mol2rdkit_phys_chem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/mol2any/mol2smiles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:14:53.572774 molpipeline-0.8.0/molpipeline/mol2mol/
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/mol2mol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6792 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/mol2mol/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/mol2mol/reaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/mol2mol/scaffolds.py
--rw-r--r--   0 runner    (1001) docker     (127)    21043 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/mol2mol/standardization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:14:53.572774 molpipeline-0.8.0/molpipeline/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/pipeline/_molpipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    33384 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/pipeline/_skl_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/post_prediction.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:14:53.572774 molpipeline-0.8.0/molpipeline/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/utils/json_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/utils/kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/utils/matrices.py
--rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/utils/molpipeline_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/utils/multi_proc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/utils/substructure_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-25 16:14:44.000000 molpipeline-0.8.0/molpipeline/utils/value_checks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:14:53.580774 molpipeline-0.8.0/molpipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-25 16:14:53.000000 molpipeline-0.8.0/molpipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-25 16:14:53.000000 molpipeline-0.8.0/molpipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:14:53.000000 molpipeline-0.8.0/molpipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-25 16:14:53.000000 molpipeline-0.8.0/molpipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-25 16:14:53.000000 molpipeline-0.8.0/molpipeline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-25 16:14:44.000000 molpipeline-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-25 16:14:44.000000 molpipeline-0.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 16:14:44.000000 molpipeline-0.8.0/requirements_chemprop.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-25 16:14:44.000000 molpipeline-0.8.0/requirements_notebooks.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 16:14:53.580774 molpipeline-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:14:53.572774 molpipeline-0.8.0/test_extras/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-25 16:14:44.000000 molpipeline-0.8.0/test_extras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:14:53.576774 molpipeline-0.8.0/test_extras/test_chemprop/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-25 16:14:44.000000 molpipeline-0.8.0/test_extras/test_chemprop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11001 2024-04-25 16:14:44.000000 molpipeline-0.8.0/test_extras/test_chemprop/test_chemprop_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-04-25 16:14:44.000000 molpipeline-0.8.0/test_extras/test_chemprop/test_component_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8166 2024-04-25 16:14:44.000000 molpipeline-0.8.0/test_extras/test_chemprop/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:14:53.576774 molpipeline-0.8.0/test_extras/test_notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-25 16:14:44.000000 molpipeline-0.8.0/test_extras/test_notebooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-04-25 16:14:44.000000 molpipeline-0.8.0/test_extras/test_notebooks/test_notebooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:14:53.576774 molpipeline-0.8.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:14:53.576774 molpipeline-0.8.0/tests/molpipeline/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-25 16:14:44.000000 molpipeline-0.8.0/tests/molpipeline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:14:53.576774 molpipeline-0.8.0/tests/test_elements/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 16:14:44.000000 molpipeline-0.8.0/tests/test_elements/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:14:53.576774 molpipeline-0.8.0/tests/test_elements/test_any2mol/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 16:14:44.000000 molpipeline-0.8.0/tests/test_elements/test_any2mol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10399 2024-04-25 16:14:44.000000 molpipeline-0.8.0/tests/test_elements/test_any2mol/test_auto2mol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-25 16:14:44.000000 molpipeline-0.8.0/tests/test_elements/test_any2mol/test_bin2mol.py
--rw-r--r--   0 runner    (1001) docker     (127)     9563 2024-04-25 16:14:44.000000 molpipeline-0.8.0/tests/test_elements/test_error_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:14:53.576774 molpipeline-0.8.0/tests/test_elements/test_mol2any/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 16:14:44.000000 molpipeline-0.8.0/tests/test_elements/test_mol2any/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-25 16:14:44.000000 molpipeline-0.8.0/tests/test_elements/test_mol2any/test_mol2bin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-25 16:14:44.000000 molpipeline-0.8.0/tests/test_elements/test_mol2any/test_mol2concatenated.py
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-25 16:14:44.000000 molpipeline-0.8.0/tests/test_elements/test_mol2any/test_mol2inchi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-25 16:14:44.000000 molpipeline-0.8.0/tests/test_elements/test_mol2any/test_mol2morgan_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-04-25 16:14:44.000000 molpipeline-0.8.0/tests/test_elements/test_mol2any/test_mol2net_charge.py
--rw-r--r--   0 runner    (1001) docker     (127)     8665 2024-04-25 16:14:44.000000 molpipeline-0.8.0/tests/test_elements/test_mol2any/test_mol2rdkit_phys_chem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:14:53.576774 molpipeline-0.8.0/tests/test_elements/test_mol2mol/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 16:14:44.000000 molpipeline-0.8.0/tests/test_elements/test_mol2mol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-25 16:14:44.000000 molpipeline-0.8.0/tests/test_elements/test_mol2mol/test_mol2mol_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9768 2024-04-25 16:14:44.000000 molpipeline-0.8.0/tests/test_elements/test_mol2mol/test_mol2mol_standardization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:14:53.580774 molpipeline-0.8.0/tests/test_estimators/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-25 16:14:44.000000 molpipeline-0.8.0/tests/test_estimators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:14:53.580774 molpipeline-0.8.0/tests/test_estimators/test_algorithm/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-25 16:14:44.000000 molpipeline-0.8.0/tests/test_estimators/test_algorithm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8943 2024-04-25 16:14:44.000000 molpipeline-0.8.0/tests/test_estimators/test_algorithm/test_connected_component_clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-25 16:14:44.000000 molpipeline-0.8.0/tests/test_estimators/test_algorithm/test_union_find.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-25 16:14:44.000000 molpipeline-0.8.0/tests/test_estimators/test_connected_component_clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-25 16:14:44.000000 molpipeline-0.8.0/tests/test_estimators/test_leader_picker_clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-04-25 16:14:44.000000 molpipeline-0.8.0/tests/test_estimators/test_murcko_scaffold_clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-04-25 16:14:44.000000 molpipeline-0.8.0/tests/test_estimators/test_nearest_neighbors.py
--rw-r--r--   0 runner    (1001) docker     (127)    10883 2024-04-25 16:14:44.000000 molpipeline-0.8.0/tests/test_estimators/test_similarity_transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:14:53.580774 molpipeline-0.8.0/tests/test_metrics/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-25 16:14:44.000000 molpipeline-0.8.0/tests/test_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-25 16:14:44.000000 molpipeline-0.8.0/tests/test_metrics/test_ignore_error_scorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9421 2024-04-25 16:14:44.000000 molpipeline-0.8.0/tests/test_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:14:53.580774 molpipeline-0.8.0/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 16:14:44.000000 molpipeline-0.8.0/tests/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-25 16:14:44.000000 molpipeline-0.8.0/tests/test_utils/test_json_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:14:53.580774 molpipeline-0.8.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 16:14:44.000000 molpipeline-0.8.0/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-04-25 16:14:44.000000 molpipeline-0.8.0/tests/utils/fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-25 16:14:44.000000 molpipeline-0.8.0/tests/utils/mock_element.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.928191 molpipeline-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-15 12:18:56.000000 molpipeline-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-05-15 12:19:02.928191 molpipeline-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-15 12:18:56.000000 molpipeline-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.908191 molpipeline-0.8.1/molpipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.908191 molpipeline-0.8.1/molpipeline/abstract_pipeline_elements/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/abstract_pipeline_elements/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.912191 molpipeline-0.8.1/molpipeline/abstract_pipeline_elements/any2mol/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/abstract_pipeline_elements/any2mol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/abstract_pipeline_elements/any2mol/string2mol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23644 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/abstract_pipeline_elements/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.912191 molpipeline-0.8.1/molpipeline/abstract_pipeline_elements/mol2any/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/abstract_pipeline_elements/mol2any/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12159 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/abstract_pipeline_elements/mol2any/mol2bitvector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/abstract_pipeline_elements/mol2any/mol2floatvector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/abstract_pipeline_elements/mol2any/mol2string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.912191 molpipeline-0.8.1/molpipeline/any2mol/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/any2mol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/any2mol/auto2mol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/any2mol/bin2mol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/any2mol/sdf2mol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/any2mol/smiles2mol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23790 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/error_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.912191 molpipeline-0.8.1/molpipeline/estimators/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/estimators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.912191 molpipeline-0.8.1/molpipeline/estimators/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/estimators/algorithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/estimators/algorithm/connected_component_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/estimators/algorithm/union_find.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.916191 molpipeline-0.8.1/molpipeline/estimators/chemprop/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/estimators/chemprop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/estimators/chemprop/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14929 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/estimators/chemprop/component_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/estimators/chemprop/lightning_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10841 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/estimators/chemprop/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/estimators/chemprop/neural_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/estimators/connected_component_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/estimators/leader_picker_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7775 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/estimators/murcko_scaffold_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7178 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/estimators/nearest_neighbor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/estimators/similarity_transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.916191 molpipeline-0.8.1/molpipeline/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/metrics/ignore_error_scorer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.916191 molpipeline-0.8.1/molpipeline/mol2any/
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/mol2any/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/mol2any/mol2bin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/mol2any/mol2chemprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9175 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/mol2any/mol2concatinated_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/mol2any/mol2inchi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/mol2any/mol2morgan_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/mol2any/mol2net_charge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/mol2any/mol2rdkit_phys_chem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/mol2any/mol2smiles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.916191 molpipeline-0.8.1/molpipeline/mol2mol/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/mol2mol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8348 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/mol2mol/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/mol2mol/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/mol2mol/scaffolds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21043 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/mol2mol/standardization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.916191 molpipeline-0.8.1/molpipeline/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/pipeline/_molpipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33384 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/pipeline/_skl_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/post_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.920191 molpipeline-0.8.1/molpipeline/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/utils/json_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/utils/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/utils/matrices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/utils/molpipeline_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/utils/multi_proc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/utils/substructure_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/utils/value_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.928191 molpipeline-0.8.1/molpipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-05-15 12:19:02.000000 molpipeline-0.8.1/molpipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-15 12:19:02.000000 molpipeline-0.8.1/molpipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 12:19:02.000000 molpipeline-0.8.1/molpipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-15 12:19:02.000000 molpipeline-0.8.1/molpipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-15 12:19:02.000000 molpipeline-0.8.1/molpipeline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-15 12:18:56.000000 molpipeline-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-15 12:18:56.000000 molpipeline-0.8.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-15 12:18:56.000000 molpipeline-0.8.1/requirements_chemprop.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 12:18:56.000000 molpipeline-0.8.1/requirements_notebooks.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 12:19:02.928191 molpipeline-0.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.920191 molpipeline-0.8.1/test_extras/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-15 12:18:56.000000 molpipeline-0.8.1/test_extras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.920191 molpipeline-0.8.1/test_extras/test_chemprop/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-15 12:18:56.000000 molpipeline-0.8.1/test_extras/test_chemprop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-15 12:18:56.000000 molpipeline-0.8.1/test_extras/test_chemprop/test_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-05-15 12:18:56.000000 molpipeline-0.8.1/test_extras/test_chemprop/test_chemprop_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-05-15 12:18:56.000000 molpipeline-0.8.1/test_extras/test_chemprop/test_component_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-15 12:18:56.000000 molpipeline-0.8.1/test_extras/test_chemprop/test_lightning_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12424 2024-05-15 12:18:56.000000 molpipeline-0.8.1/test_extras/test_chemprop/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.920191 molpipeline-0.8.1/test_extras/test_notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-15 12:18:56.000000 molpipeline-0.8.1/test_extras/test_notebooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-05-15 12:18:56.000000 molpipeline-0.8.1/test_extras/test_notebooks/test_notebooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.920191 molpipeline-0.8.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.920191 molpipeline-0.8.1/tests/test_elements/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_elements/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.924191 molpipeline-0.8.1/tests/test_elements/test_any2mol/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_elements/test_any2mol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10399 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_elements/test_any2mol/test_auto2mol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_elements/test_any2mol/test_bin2mol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9563 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_elements/test_error_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.924191 molpipeline-0.8.1/tests/test_elements/test_mol2any/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_elements/test_mol2any/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_elements/test_mol2any/test_mol2bin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_elements/test_mol2any/test_mol2concatenated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_elements/test_mol2any/test_mol2inchi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_elements/test_mol2any/test_mol2morgan_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_elements/test_mol2any/test_mol2net_charge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8665 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_elements/test_mol2any/test_mol2rdkit_phys_chem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.924191 molpipeline-0.8.1/tests/test_elements/test_mol2mol/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_elements/test_mol2mol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_elements/test_mol2mol/test_mol2mol_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9768 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_elements/test_mol2mol/test_mol2mol_standardization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.924191 molpipeline-0.8.1/tests/test_estimators/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_estimators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.924191 molpipeline-0.8.1/tests/test_estimators/test_algorithm/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_estimators/test_algorithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8943 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_estimators/test_algorithm/test_connected_component_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_estimators/test_algorithm/test_union_find.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_estimators/test_connected_component_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_estimators/test_leader_picker_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_estimators/test_murcko_scaffold_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_estimators/test_nearest_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10883 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_estimators/test_similarity_transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.924191 molpipeline-0.8.1/tests/test_metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_metrics/test_ignore_error_scorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9421 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.928191 molpipeline-0.8.1/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_utils/test_json_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.928191 molpipeline-0.8.1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/utils/fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/utils/mock_element.py
```

### Comparing `molpipeline-0.8.0/LICENSE` & `molpipeline-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/PKG-INFO` & `molpipeline-0.8.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: molpipeline
-Version: 0.8.0
+Version: 0.8.1
 Summary: Integration of rdkit functionality into sklearn pipelines.
 Author: Christian W. Feldmann, Jennifer Hemmerich, Jochen Sieg
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: joblib>=1.3.0
 Requires-Dist: loguru
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: rdkit>=2023.9.1
 Requires-Dist: scipy
 Requires-Dist: setuptools
 Requires-Dist: scikit-learn>=1.4.0
 Requires-Dist: typing_extensions
 Provides-Extra: all
-Requires-Dist: chemprop; extra == "all"
+Requires-Dist: chemprop>=2.0.0; extra == "all"
 Requires-Dist: lightning; extra == "all"
 Requires-Dist: jupyterlab; extra == "all"
 Requires-Dist: seaborn; extra == "all"
 Provides-Extra: chemprop
-Requires-Dist: chemprop; extra == "chemprop"
+Requires-Dist: chemprop>=2.0.0; extra == "chemprop"
 Requires-Dist: lightning; extra == "chemprop"
 Provides-Extra: notebooks
 Requires-Dist: jupyterlab; extra == "notebooks"
 Requires-Dist: seaborn; extra == "notebooks"
 
 # MolPipeline
 MolPipeline is a Python package providing RDKit functionality in a Scikit-learn like fashion.
@@ -45,17 +45,16 @@
 
 
 ## Publications
 
 The publication is freely available [here](https://chemrxiv.org/engage/chemrxiv/article-details/661fec7f418a5379b00ae036).
 
 ## Installation
-Not yet available in pypi. For now, Please download and install via:
 ```commandline
-pip install git+https://github.com/basf/MolPipeline.git
+pip install molpipeline
 ```
 
 ## Usage
 
 See the [notebooks](notebooks) folder for basic and advanced examples of how to use Molpipeline.
 
 A basic example of how to use MolPipeline to create a fingerprint-based model is shown below (see also the [notebook](notebooks/01_getting_started_with_molpipeline.ipynb)):
```

### Comparing `molpipeline-0.8.0/README.md` & `molpipeline-0.8.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -17,17 +17,16 @@
 
 
 ## Publications
 
 The publication is freely available [here](https://chemrxiv.org/engage/chemrxiv/article-details/661fec7f418a5379b00ae036).
 
 ## Installation
-Not yet available in pypi. For now, Please download and install via:
 ```commandline
-pip install git+https://github.com/basf/MolPipeline.git
+pip install molpipeline
 ```
 
 ## Usage
 
 See the [notebooks](notebooks) folder for basic and advanced examples of how to use Molpipeline.
 
 A basic example of how to use MolPipeline to create a fingerprint-based model is shown below (see also the [notebook](notebooks/01_getting_started_with_molpipeline.ipynb)):
```

### Comparing `molpipeline-0.8.0/molpipeline/__init__.py` & `molpipeline-0.8.1/molpipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/abstract_pipeline_elements/any2mol/string2mol.py` & `molpipeline-0.8.1/molpipeline/abstract_pipeline_elements/any2mol/string2mol.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/abstract_pipeline_elements/core.py` & `molpipeline-0.8.1/molpipeline/abstract_pipeline_elements/core.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/abstract_pipeline_elements/mol2any/mol2bitvector.py` & `molpipeline-0.8.1/molpipeline/abstract_pipeline_elements/mol2any/mol2bitvector.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/abstract_pipeline_elements/mol2any/mol2floatvector.py` & `molpipeline-0.8.1/molpipeline/abstract_pipeline_elements/mol2any/mol2floatvector.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         uuid: Optional[str] = None,
     ) -> None:
         """Initialize MolToDescriptorPipelineElement.
 
         Parameters
         ----------
         standardizer: Optional[AnyTransformer], default=StandardScaler()
-           The output is post_processed accoding to the standardizer if not None.
+            The output is post_processed according to the standardizer if not None.
         name: str:
             Name of the PipelineElement.
         n_jobs: int:
             Number of jobs to use for parallelization.
         uuid: Optional[str]
             UUID of the PipelineElement.
```

### Comparing `molpipeline-0.8.0/molpipeline/abstract_pipeline_elements/mol2any/mol2string.py` & `molpipeline-0.8.1/molpipeline/abstract_pipeline_elements/mol2any/mol2string.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/any2mol/auto2mol.py` & `molpipeline-0.8.1/molpipeline/any2mol/auto2mol.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/any2mol/bin2mol.py` & `molpipeline-0.8.1/molpipeline/any2mol/bin2mol.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/any2mol/sdf2mol.py` & `molpipeline-0.8.1/molpipeline/any2mol/sdf2mol.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/any2mol/smiles2mol.py` & `molpipeline-0.8.1/molpipeline/any2mol/smiles2mol.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/error_handling.py` & `molpipeline-0.8.1/molpipeline/error_handling.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/estimators/__init__.py` & `molpipeline-0.8.1/molpipeline/estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/estimators/algorithm/connected_component_clustering.py` & `molpipeline-0.8.1/molpipeline/estimators/algorithm/connected_component_clustering.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/estimators/algorithm/union_find.py` & `molpipeline-0.8.1/molpipeline/estimators/algorithm/union_find.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/estimators/chemprop/abstract.py` & `molpipeline-0.8.1/molpipeline/estimators/chemprop/neural_fingerprint.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,97 +1,111 @@
-"""Parent class of wrapper for Chemprop to make it compatible with scikit-learn."""
+"""Wrap Chemprop in a sklearn like transformer returning the neural fingerprint as a numpy array."""
 
-import abc
-from typing import Any, Iterable
-
-# pylint: disable=duplicate-code
-try:
-    from typing import Self  # type: ignore[attr-defined]
-except ImportError:
-    from typing_extensions import Self
+from typing import Self, Sequence
 
 import numpy as np
 import numpy.typing as npt
+from chemprop.data import BatchMolGraph, MoleculeDataset
+from chemprop.models.model import MPNN
+from lightning import pytorch as pl
 
-try:
-    from chemprop.data import MoleculeDataset, build_dataloader
-    from chemprop.models.model import MPNN
-    from lightning import pytorch as pl
-except ImportError:
-    pass
-from sklearn.base import BaseEstimator
-
-# pylint: enable=duplicate-code
+from molpipeline.estimators.chemprop.abstract import ABCChemprop
 
 
-class ABCChemprop(BaseEstimator, abc.ABC):
-    """Wrap Chemprop in a sklearn like object."""
-
-    model: MPNN
+class ChempropNeuralFP(ABCChemprop):
+    """Wrap Chemprop in a sklearn like transformer returning the neural fingerprint as a numpy array."""
 
     def __init__(
         self,
         model: MPNN,
         lightning_trainer: pl.Trainer | None = None,
         batch_size: int = 64,
         n_jobs: int = 1,
-        **kwargs: Any,
+        disable_fitting: bool = False,
     ) -> None:
-        """Initialize the chemprop abstract model.
+        """Initialize the chemprop neural fingerprint model.
 
         Parameters
         ----------
         model : MPNN
             The chemprop model to wrap.
         lightning_trainer : pl.Trainer, optional
             The lightning trainer to use, by default None
         batch_size : int, optional (default=64)
             The batch size to use.
         n_jobs : int, optional (default=1)
             The number of jobs to use.
-        kwargs : Any
-            Parameters set using `set_params`.
-            Can be used to modify components of the model.
+        disable_fitting : bool, optional (default=False)
+            Whether to allow fitting or set to fixed encoding.
         """
-        self.model = model
-        if lightning_trainer is None:
-            lightning_trainer = pl.Trainer(
-                logger=False,
-                enable_checkpointing=False,
-                max_epochs=500,
-                enable_model_summary=False,
-                callbacks=[],
-            )
-        self.lightning_trainer = lightning_trainer
-        self.batch_size = batch_size
-        self.n_jobs = n_jobs
-        self.set_params(**kwargs)
+        # pylint: disable=duplicate-code
+        super().__init__(
+            model=model,
+            lightning_trainer=lightning_trainer,
+            batch_size=batch_size,
+            n_jobs=n_jobs,
+        )
+        self.disable_fitting = disable_fitting
 
     def fit(
         self,
         X: MoleculeDataset,  # pylint: disable=invalid-name
-        y: Iterable[int | float] | npt.NDArray[np.int_ | np.float_],
+        y: Sequence[int | float] | npt.NDArray[np.int_ | np.float_],
     ) -> Self:
-        """Fit the model to the data.
+        """Fit the model.
 
         Parameters
         ----------
         X : MoleculeDataset
             The input data.
-        y : Iterable[int | float] | npt.NDArray[np.int_ | np.float_]
+        y : Sequence[int | float] | npt.NDArray[np.int_ | np.float_]
             The target data.
 
         Returns
         -------
         Self
             The fitted model.
         """
-        if not isinstance(y, np.ndarray):
-            y = np.array(y)
-        if y.ndim == 1:
-            y = y.reshape(-1, 1)
-        X.Y = y
-        training_data = build_dataloader(
-            X, batch_size=self.batch_size, num_workers=self.n_jobs
-        )
-        self.lightning_trainer.fit(self.model, training_data)
-        return self
+        if self.disable_fitting:
+            return self
+        return super().fit(X, y)
+
+    def transform(
+        self, X: MoleculeDataset  # pylint: disable=invalid-name
+    ) -> npt.NDArray[np.float_]:
+        """Transform the input.
+
+        Parameters
+        ----------
+        X : MoleculeDataset
+            The input data.
+
+        Returns
+        -------
+        npt.NDArray[np.float_]
+            The neural fingerprint of the input data.
+        """
+        self.model.eval()
+        mol_data = [X[i].mg for i in range(len(X))]
+        return self.model.fingerprint(BatchMolGraph(mol_data)).detach().numpy()
+
+    def fit_transform(
+        self,
+        X: MoleculeDataset,  # pylint: disable=invalid-name
+        y: Sequence[int | float] | npt.NDArray[np.int_ | np.float_],
+    ) -> npt.NDArray[np.float_]:
+        """Fit the model and transform the input.
+
+        Parameters
+        ----------
+        X : MoleculeDataset
+            The input data.
+        y : Sequence[int | float] | npt.NDArray[np.int_ | np.float_]
+            The target data.
+
+        Returns
+        -------
+        npt.NDArray[np.float_]
+            The neural fingerprint of the input data.
+        """
+        self.fit(X, y)
+        return self.transform(X)
```

### Comparing `molpipeline-0.8.0/molpipeline/estimators/chemprop/component_wrapper.py` & `molpipeline-0.8.1/molpipeline/estimators/chemprop/component_wrapper.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/estimators/chemprop/models.py` & `molpipeline-0.8.1/molpipeline/estimators/chemprop/models.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Wrapper for Chemprop to make it compatible with scikit-learn."""
 
-from typing import Any
+from typing import Any, Sequence
 
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 import numpy as np
@@ -37,14 +37,77 @@
 )
 from molpipeline.estimators.chemprop.neural_fingerprint import ChempropNeuralFP
 
 
 class ChempropModel(ABCChemprop):
     """Wrap Chemprop in a sklearn like Estimator."""
 
+    _classes_: npt.NDArray[np.int_] | None
+
+    def __init__(
+        self,
+        model: MPNN,
+        lightning_trainer: pl.Trainer | None = None,
+        batch_size: int = 64,
+        n_jobs: int = 1,
+        **kwargs: Any,
+    ) -> None:
+        """Initialize the chemprop abstract model.
+
+        Parameters
+        ----------
+        model : MPNN
+            The chemprop model to wrap.
+        lightning_trainer : pl.Trainer, optional
+            The lightning trainer to use, by default None
+        batch_size : int, optional (default=64)
+            The batch size to use.
+        n_jobs : int, optional (default=1)
+            The number of jobs to use.
+        kwargs : Any
+            Parameters set using `set_params`.
+            Can be used to modify components of the model.
+        """
+        super().__init__(
+            model=model,
+            lightning_trainer=lightning_trainer,
+            batch_size=batch_size,
+            n_jobs=n_jobs,
+            **kwargs,
+        )
+        self._classes_ = None
+
+    @property
+    def classes_(self) -> npt.NDArray[np.int_]:
+        """Return the classes.
+
+        Returns
+        -------
+        npt.NDArray[np.int_]
+            The classes.
+        """
+        if not self._is_classifier():
+            raise ValueError("Model is not a classifier.")
+        if self._classes_ is None:
+            raise ValueError("Classes are not set.")
+        return self._classes_
+
+    @property
+    def _estimator_type(self) -> str:
+        """Return the estimator type.
+
+        Returns
+        -------
+        str
+            The estimator type.
+        """
+        if self._is_classifier():
+            return "classifier"
+        return "regressor"
+
     def _is_binary_classifier(self) -> bool:
         """Check if the model is a binary classifier.
 
         Returns
         -------
         bool
             True if the model is a binary classifier, False otherwise.
@@ -106,14 +169,37 @@
         if self._is_binary_classifier():
             if prediction_array.ndim != 1:
                 raise ValueError(
                     "Binary classification model should output a single probability."
                 )
         return prediction_array
 
+    def fit(
+        self,
+        X: MoleculeDataset,
+        y: Sequence[int | float] | npt.NDArray[np.int_ | np.float_],
+    ) -> Self:
+        """Fit the model to the data.
+
+        Parameters
+        ----------
+        X : MoleculeDataset
+            The input data.
+        y : Sequence[int | float] | npt.NDArray[np.int_ | np.float_]
+            The target data.
+
+        Returns
+        -------
+        Self
+            The fitted model.
+        """
+        if self._is_classifier():
+            self._classes_ = np.unique(y)
+        return super().fit(X, y)
+
     def predict(
         self, X: MoleculeDataset  # pylint: disable=invalid-name
     ) -> npt.NDArray[np.float_]:
         """Predict the output.
 
         Parameters
         ----------
```

### Comparing `molpipeline-0.8.0/molpipeline/estimators/connected_component_clustering.py` & `molpipeline-0.8.1/molpipeline/estimators/connected_component_clustering.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/estimators/leader_picker_clustering.py` & `molpipeline-0.8.1/molpipeline/estimators/leader_picker_clustering.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/estimators/murcko_scaffold_clustering.py` & `molpipeline-0.8.1/molpipeline/estimators/murcko_scaffold_clustering.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/estimators/nearest_neighbor.py` & `molpipeline-0.8.1/molpipeline/estimators/nearest_neighbor.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/estimators/similarity_transformation.py` & `molpipeline-0.8.1/molpipeline/estimators/similarity_transformation.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/metrics/ignore_error_scorer.py` & `molpipeline-0.8.1/molpipeline/metrics/ignore_error_scorer.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/mol2any/__init__.py` & `molpipeline-0.8.1/molpipeline/mol2any/__init__.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/mol2any/mol2bin.py` & `molpipeline-0.8.1/molpipeline/mol2any/mol2bin.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/mol2any/mol2chemprop.py` & `molpipeline-0.8.1/molpipeline/mol2any/mol2chemprop.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/mol2any/mol2concatinated_vector.py` & `molpipeline-0.8.1/molpipeline/mol2any/mol2concatinated_vector.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/mol2any/mol2inchi.py` & `molpipeline-0.8.1/molpipeline/mol2any/mol2inchi.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/mol2any/mol2morgan_fingerprint.py` & `molpipeline-0.8.1/molpipeline/mol2any/mol2morgan_fingerprint.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/mol2any/mol2net_charge.py` & `molpipeline-0.8.1/molpipeline/mol2any/mol2net_charge.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/mol2any/mol2rdkit_phys_chem.py` & `molpipeline-0.8.1/molpipeline/mol2any/mol2rdkit_phys_chem.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/mol2any/mol2smiles.py` & `molpipeline-0.8.1/molpipeline/mol2any/mol2smiles.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/mol2mol/filter.py` & `molpipeline-0.8.1/molpipeline/mol2mol/filter.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,14 +17,30 @@
 )
 from molpipeline.utils.molpipeline_types import OptionalMol, RDKitMol
 
 
 class ElementFilter(_MolToMolPipelineElement):
     """ElementFilter which removes molecules containing chemical elements other than specified."""
 
+    DEFAULT_ALLOWED_ELEMENT_NUMBERS = [
+        1,
+        5,
+        6,
+        7,
+        8,
+        9,
+        14,
+        15,
+        16,
+        17,
+        34,
+        35,
+        53,
+    ]
+
     def __init__(
         self,
         allowed_element_numbers: Optional[list[int]] = None,
         name: str = "ElementFilter",
         n_jobs: int = 1,
         uuid: Optional[str] = None,
     ) -> None:
@@ -40,29 +56,15 @@
         n_jobs: int, optional (default: 1)
             Number of parallel jobs to use.
         uuid: str, optional (default: None)
             Unique identifier of the pipeline element.
         """
         super().__init__(name=name, n_jobs=n_jobs, uuid=uuid)
         if allowed_element_numbers is None:
-            allowed_element_numbers = [
-                1,
-                5,
-                6,
-                7,
-                8,
-                9,
-                14,
-                15,
-                16,
-                17,
-                34,
-                35,
-                53,
-            ]
+            allowed_element_numbers = self.DEFAULT_ALLOWED_ELEMENT_NUMBERS
         if not isinstance(allowed_element_numbers, set):
             self.allowed_element_numbers = set(allowed_element_numbers)
         else:
             self.allowed_element_numbers = allowed_element_numbers
 
     def get_params(self, deep: bool = True) -> dict[str, Any]:
         """Get parameters of ElementFilter.
@@ -145,15 +147,15 @@
         name: str, optional (default: "MixtureFilterPipe")
             Name of the pipeline element.
         n_jobs: int, optional (default: 1)
             Number of parallel jobs to use.
         uuid: str, optional (default: None)
             Unique identifier of the pipeline element.
         """
-        super().__init__(name=name, n_jobs=n_jobs)
+        super().__init__(name=name, n_jobs=n_jobs, uuid=uuid)
 
     def pretransform_single(self, value: RDKitMol) -> OptionalMol:
         """Invalidate molecule containing multiple fragments.
 
         Parameters
         ----------
         value: RDKitMol
@@ -191,15 +193,15 @@
         name: str, optional (default: "EmptyMoleculeFilterPipe")
             Name of the pipeline element.
         n_jobs: int, optional (default: 1)
             Number of parallel jobs to use.
         uuid: str, optional (default: None)
             Unique identifier of the pipeline element.
         """
-        super().__init__(name=name, n_jobs=n_jobs)
+        super().__init__(name=name, n_jobs=n_jobs, uuid=uuid)
 
     def pretransform_single(self, value: RDKitMol) -> OptionalMol:
         """Invalidate empty molecule.
 
         Parameters
         ----------
         value: RDKitMol
@@ -209,7 +211,55 @@
         -------
         OptionalMol
             Molecule if it is not empty, else InvalidInstance.
         """
         if value.GetNumAtoms() == 0:
             return InvalidInstance(self.uuid, "Molecule contains no atoms.", self.name)
         return value
+
+
+class InorganicsFilter(_MolToMolPipelineElement):
+    """Filters Molecules which do not contain any organic (i.e. Carbon) atoms."""
+
+    CARBON_INORGANICS = ["O=C=O", "[C-]#[O+]"]  # CO2 and CO are not organic
+
+    def __init__(
+        self,
+        name: str = "InorganicsFilter",
+        n_jobs: int = 1,
+        uuid: Optional[str] = None,
+    ) -> None:
+        """Initialize InorganicsFilter.
+
+        Parameters
+        ----------
+        name: str, optional (default: "InorganicsFilter")
+            Name of the pipeline element.
+        n_jobs: int, optional (default: 1)
+            Number of parallel jobs to use.
+        uuid: str, optional (default: None)
+            Unique identifier of the pipeline element.
+        """
+        super().__init__(name=name, n_jobs=n_jobs, uuid=uuid)
+
+    def pretransform_single(self, value: RDKitMol) -> OptionalMol:
+        """Invalidate molecules not containing a carbon atom.
+
+        Parameters
+        ----------
+        value: RDKitMol
+            Molecule to check.
+
+        Returns
+        -------
+        OptionalMol
+            Molecule if it contains carbon, else InvalidInstance.
+        """
+        if not any(atom.GetAtomicNum() == 6 for atom in value.GetAtoms()):
+            return InvalidInstance(
+                self.uuid, "Molecule contains no organic atoms.", self.name
+            )
+        smiles = Chem.MolToSmiles(value)
+        print(smiles)
+        if smiles in self.CARBON_INORGANICS:
+            return InvalidInstance(self.uuid, "Molecule is not organic.", self.name)
+        return value
```

### Comparing `molpipeline-0.8.0/molpipeline/mol2mol/reaction.py` & `molpipeline-0.8.1/molpipeline/mol2mol/reaction.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/mol2mol/scaffolds.py` & `molpipeline-0.8.1/molpipeline/mol2mol/scaffolds.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/mol2mol/standardization.py` & `molpipeline-0.8.1/molpipeline/mol2mol/standardization.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/pipeline/_molpipeline.py` & `molpipeline-0.8.1/molpipeline/pipeline/_molpipeline.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/pipeline/_skl_pipeline.py` & `molpipeline-0.8.1/molpipeline/pipeline/_skl_pipeline.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/post_prediction.py` & `molpipeline-0.8.1/molpipeline/post_prediction.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         **params: Any,
     ) -> Self:
         """Fit PostPredictionWrapper.
 
         Parameters
         ----------
         X : npt.NDArray[Any]
-           Input data.
+            Input data.
         y : Optional[npt.NDArray[Any]]
             Target data.
         **params : Any
             Additional parameters for fitting.
 
         Returns
         -------
```

### Comparing `molpipeline-0.8.0/molpipeline/utils/json_operations.py` & `molpipeline-0.8.1/molpipeline/utils/json_operations.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/utils/kernel.py` & `molpipeline-0.8.1/molpipeline/utils/kernel.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/utils/matrices.py` & `molpipeline-0.8.1/molpipeline/utils/matrices.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/utils/molpipeline_types.py` & `molpipeline-0.8.1/molpipeline/utils/molpipeline_types.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/utils/multi_proc.py` & `molpipeline-0.8.1/molpipeline/utils/multi_proc.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/utils/substructure_handling.py` & `molpipeline-0.8.1/molpipeline/utils/substructure_handling.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline/utils/value_checks.py` & `molpipeline-0.8.1/molpipeline/utils/value_checks.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/molpipeline.egg-info/PKG-INFO` & `molpipeline-0.8.1/molpipeline.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: molpipeline
-Version: 0.8.0
+Version: 0.8.1
 Summary: Integration of rdkit functionality into sklearn pipelines.
 Author: Christian W. Feldmann, Jennifer Hemmerich, Jochen Sieg
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: joblib>=1.3.0
 Requires-Dist: loguru
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: rdkit>=2023.9.1
 Requires-Dist: scipy
 Requires-Dist: setuptools
 Requires-Dist: scikit-learn>=1.4.0
 Requires-Dist: typing_extensions
 Provides-Extra: all
-Requires-Dist: chemprop; extra == "all"
+Requires-Dist: chemprop>=2.0.0; extra == "all"
 Requires-Dist: lightning; extra == "all"
 Requires-Dist: jupyterlab; extra == "all"
 Requires-Dist: seaborn; extra == "all"
 Provides-Extra: chemprop
-Requires-Dist: chemprop; extra == "chemprop"
+Requires-Dist: chemprop>=2.0.0; extra == "chemprop"
 Requires-Dist: lightning; extra == "chemprop"
 Provides-Extra: notebooks
 Requires-Dist: jupyterlab; extra == "notebooks"
 Requires-Dist: seaborn; extra == "notebooks"
 
 # MolPipeline
 MolPipeline is a Python package providing RDKit functionality in a Scikit-learn like fashion.
@@ -45,17 +45,16 @@
 
 
 ## Publications
 
 The publication is freely available [here](https://chemrxiv.org/engage/chemrxiv/article-details/661fec7f418a5379b00ae036).
 
 ## Installation
-Not yet available in pypi. For now, Please download and install via:
 ```commandline
-pip install git+https://github.com/basf/MolPipeline.git
+pip install molpipeline
 ```
 
 ## Usage
 
 See the [notebooks](notebooks) folder for basic and advanced examples of how to use Molpipeline.
 
 A basic example of how to use MolPipeline to create a fingerprint-based model is shown below (see also the [notebook](notebooks/01_getting_started_with_molpipeline.ipynb)):
```

### Comparing `molpipeline-0.8.0/molpipeline.egg-info/SOURCES.txt` & `molpipeline-0.8.1/molpipeline.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 molpipeline/estimators/similarity_transformation.py
 molpipeline/estimators/algorithm/__init__.py
 molpipeline/estimators/algorithm/connected_component_clustering.py
 molpipeline/estimators/algorithm/union_find.py
 molpipeline/estimators/chemprop/__init__.py
 molpipeline/estimators/chemprop/abstract.py
 molpipeline/estimators/chemprop/component_wrapper.py
+molpipeline/estimators/chemprop/lightning_wrapper.py
 molpipeline/estimators/chemprop/models.py
 molpipeline/estimators/chemprop/neural_fingerprint.py
 molpipeline/metrics/__init__.py
 molpipeline/metrics/ignore_error_scorer.py
 molpipeline/mol2any/__init__.py
 molpipeline/mol2any/mol2bin.py
 molpipeline/mol2any/mol2chemprop.py
@@ -65,21 +66,22 @@
 molpipeline/utils/matrices.py
 molpipeline/utils/molpipeline_types.py
 molpipeline/utils/multi_proc.py
 molpipeline/utils/substructure_handling.py
 molpipeline/utils/value_checks.py
 test_extras/__init__.py
 test_extras/test_chemprop/__init__.py
+test_extras/test_chemprop/test_abstract.py
 test_extras/test_chemprop/test_chemprop_pipeline.py
 test_extras/test_chemprop/test_component_wrapper.py
+test_extras/test_chemprop/test_lightning_wrapper.py
 test_extras/test_chemprop/test_models.py
 test_extras/test_notebooks/__init__.py
 test_extras/test_notebooks/test_notebooks.py
 tests/test_pipeline.py
-tests/molpipeline/__init__.py
 tests/test_elements/__init__.py
 tests/test_elements/test_error_handling.py
 tests/test_elements/test_any2mol/__init__.py
 tests/test_elements/test_any2mol/test_auto2mol.py
 tests/test_elements/test_any2mol/test_bin2mol.py
 tests/test_elements/test_mol2any/__init__.py
 tests/test_elements/test_mol2any/test_mol2bin.py
```

### Comparing `molpipeline-0.8.0/pyproject.toml` & `molpipeline-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 name = "molpipeline"
 authors = [
     {name = "Christian W. Feldmann"},
     {name = "Jennifer Hemmerich"},
     {name = "Jochen Sieg"}
 ]
 description = "Integration of rdkit functionality into sklearn pipelines."
-version = "0.8.0"
+version = "0.8.1"
 readme = "README.md"
 
 [tool.setuptools.dynamic]
 dependencies = {file = "requirements.txt"}
 
 [tool.setuptools.dynamic.optional-dependencies]
 all = {file = ["requirements_chemprop.txt", "requirements_notebooks.txt"]}
```

### Comparing `molpipeline-0.8.0/test_extras/test_chemprop/test_chemprop_pipeline.py` & `molpipeline-0.8.1/test_extras/test_chemprop/test_chemprop_pipeline.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from typing import TypeVar
 
 import joblib
 import numpy as np
 import pandas as pd
 from chemprop.nn.loss import LossFunction
 from lightning import pytorch as pl
+from lightning.pytorch.accelerators import Accelerator
+from lightning.pytorch.profilers.base import PassThroughProfiler
 from sklearn.base import clone
 from torch import nn
 
 from molpipeline.any2mol import SmilesToMol
 from molpipeline.error_handling import ErrorFilter, FilterReinserter
 from molpipeline.estimators.chemprop.component_wrapper import (
     MPNN,
@@ -213,16 +215,23 @@
                     )
                 elif isinstance(param, LossFunction):
                     self.assertEqual(
                         param.state_dict()["task_weights"],
                         cloned_params[param_name].state_dict()["task_weights"],
                     )
                     self.assertEqual(type(param), type(cloned_params[param_name]))
-                elif isinstance(param, nn.Identity):
+                elif isinstance(param, (nn.Identity, Accelerator, PassThroughProfiler)):
                     self.assertEqual(type(param), type(cloned_params[param_name]))
+                elif param_name == "lightning_trainer__callbacks":
+                    self.assertIsInstance(cloned_params[param_name], list)
+                    self.assertEqual(len(param), len(cloned_params[param_name]))
+                    for callback, cloned_callback in zip(
+                        param, cloned_params[param_name]
+                    ):
+                        self.assertEqual(type(callback), type(cloned_callback))
                 else:
                     self.assertEqual(
                         param, cloned_params[param_name], f"Failed for {param_name}"
                     )
 
     def test_passing_smiles(self) -> None:
         """Test passing SMILES strings to the pipeline.
```

### Comparing `molpipeline-0.8.0/test_extras/test_chemprop/test_component_wrapper.py` & `molpipeline-0.8.1/test_extras/test_chemprop/test_component_wrapper.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/test_extras/test_notebooks/test_notebooks.py` & `molpipeline-0.8.1/test_extras/test_notebooks/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/tests/test_elements/test_any2mol/test_auto2mol.py` & `molpipeline-0.8.1/tests/test_elements/test_any2mol/test_auto2mol.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/tests/test_elements/test_any2mol/test_bin2mol.py` & `molpipeline-0.8.1/tests/test_elements/test_any2mol/test_bin2mol.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/tests/test_elements/test_error_handling.py` & `molpipeline-0.8.1/tests/test_elements/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/tests/test_elements/test_mol2any/test_mol2bin.py` & `molpipeline-0.8.1/tests/test_elements/test_mol2any/test_mol2bin.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/tests/test_elements/test_mol2any/test_mol2concatenated.py` & `molpipeline-0.8.1/tests/test_elements/test_mol2any/test_mol2concatenated.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/tests/test_elements/test_mol2any/test_mol2inchi.py` & `molpipeline-0.8.1/tests/test_elements/test_mol2any/test_mol2inchi.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/tests/test_elements/test_mol2any/test_mol2morgan_fingerprint.py` & `molpipeline-0.8.1/tests/test_elements/test_mol2any/test_mol2morgan_fingerprint.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/tests/test_elements/test_mol2any/test_mol2net_charge.py` & `molpipeline-0.8.1/tests/test_elements/test_mol2any/test_mol2net_charge.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/tests/test_elements/test_mol2any/test_mol2rdkit_phys_chem.py` & `molpipeline-0.8.1/tests/test_elements/test_mol2any/test_mol2rdkit_phys_chem.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/tests/test_elements/test_mol2mol/test_mol2mol_standardization.py` & `molpipeline-0.8.1/tests/test_elements/test_mol2mol/test_mol2mol_standardization.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/tests/test_estimators/test_algorithm/test_connected_component_clustering.py` & `molpipeline-0.8.1/tests/test_estimators/test_algorithm/test_connected_component_clustering.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/tests/test_estimators/test_algorithm/test_union_find.py` & `molpipeline-0.8.1/tests/test_estimators/test_algorithm/test_union_find.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/tests/test_estimators/test_connected_component_clustering.py` & `molpipeline-0.8.1/tests/test_estimators/test_connected_component_clustering.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/tests/test_estimators/test_leader_picker_clustering.py` & `molpipeline-0.8.1/tests/test_estimators/test_leader_picker_clustering.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/tests/test_estimators/test_murcko_scaffold_clustering.py` & `molpipeline-0.8.1/tests/test_estimators/test_murcko_scaffold_clustering.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/tests/test_estimators/test_nearest_neighbors.py` & `molpipeline-0.8.1/tests/test_estimators/test_nearest_neighbors.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/tests/test_estimators/test_similarity_transformation.py` & `molpipeline-0.8.1/tests/test_estimators/test_similarity_transformation.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/tests/test_metrics/test_ignore_error_scorer.py` & `molpipeline-0.8.1/tests/test_metrics/test_ignore_error_scorer.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/tests/test_pipeline.py` & `molpipeline-0.8.1/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/tests/test_utils/test_json_operations.py` & `molpipeline-0.8.1/tests/test_utils/test_json_operations.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/tests/utils/fingerprints.py` & `molpipeline-0.8.1/tests/utils/fingerprints.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.0/tests/utils/mock_element.py` & `molpipeline-0.8.1/tests/utils/mock_element.py`

 * *Files identical despite different names*

