# Comparing `tmp/compas_model-0.4.1.tar.gz` & `tmp/compas_model-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compas_model-0.4.1.tar", last modified: Sun May 12 21:26:55 2024, max compression
+gzip compressed data, was "compas_model-0.4.2.tar", last modified: Tue May 14 18:38:58 2024, max compression
```

## Comparing `compas_model-0.4.1.tar` & `compas_model-0.4.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:26:55.469824 compas_model-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-12 21:26:42.000000 compas_model-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-12 21:26:55.469824 compas_model-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-12 21:26:42.000000 compas_model-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-05-12 21:26:42.000000 compas_model-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-12 21:26:42.000000 compas_model-0.4.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-12 21:26:42.000000 compas_model-0.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 21:26:55.473824 compas_model-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:26:55.457824 compas_model-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:26:55.461824 compas_model-0.4.1/src/compas_model/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:26:55.461824 compas_model-0.4.1/src/compas_model/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12192 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/algorithms/collisions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7107 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/algorithms/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/algorithms/nnbrs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:26:55.465824 compas_model-0.4.1/src/compas_model/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/analysis/cra.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:26:55.465824 compas_model-0.4.1/src/compas_model/elements/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7248 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/elements/block.py
--rw-r--r--   0 runner    (1001) docker     (127)    11034 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/elements/element.py
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/elements/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/elements/plate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:26:55.465824 compas_model-0.4.1/src/compas_model/interactions/
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/interactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/interactions/contact.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/interactions/interaction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:26:55.465824 compas_model-0.4.1/src/compas_model/loads/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/loads/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:26:55.465824 compas_model-0.4.1/src/compas_model/materials/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/materials/concrete.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/materials/material.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/materials/reinforcedconcrete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/materials/steel.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/materials/timber.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:26:55.465824 compas_model-0.4.1/src/compas_model/models/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/models/blockmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/models/elementnode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/models/elementtree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/models/groupnode.py
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/models/interactiongraph.py
--rw-r--r--   0 runner    (1001) docker     (127)    20450 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:26:55.465824 compas_model-0.4.1/src/compas_model/notebook/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/notebook/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:26:55.469824 compas_model-0.4.1/src/compas_model/notebook/scene/
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/notebook/scene/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/notebook/scene/blockobject.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/notebook/scene/elementobject.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/notebook/scene/modelobject.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:26:55.469824 compas_model-0.4.1/src/compas_model/rhino/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/rhino/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:26:55.469824 compas_model-0.4.1/src/compas_model/scene/
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/scene/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/scene/blockobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/scene/elementobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/scene/modelobject.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:26:55.469824 compas_model-0.4.1/src/compas_model/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:26:55.469824 compas_model-0.4.1/src/compas_model/viewers/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/viewers/blockmodelviewer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 21:26:42.000000 compas_model-0.4.1/src/compas_model/viewers/modelviewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:26:55.469824 compas_model-0.4.1/src/compas_model.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-12 21:26:55.000000 compas_model-0.4.1/src/compas_model.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-05-12 21:26:55.000000 compas_model-0.4.1/src/compas_model.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 21:26:55.000000 compas_model-0.4.1/src/compas_model.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 21:26:55.000000 compas_model-0.4.1/src/compas_model.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-12 21:26:55.000000 compas_model-0.4.1/src/compas_model.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-12 21:26:55.000000 compas_model-0.4.1/src/compas_model.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:26:55.469824 compas_model-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-12 21:26:42.000000 compas_model-0.4.1/tests/test_algorithms_collider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-12 21:26:42.000000 compas_model-0.4.1/tests/test_interactiongraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-12 21:26:42.000000 compas_model-0.4.1/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-12 21:26:42.000000 compas_model-0.4.1/tests/test_trivial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:38:58.829944 compas_model-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-14 18:38:44.000000 compas_model-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-14 18:38:58.829944 compas_model-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-14 18:38:44.000000 compas_model-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-05-14 18:38:44.000000 compas_model-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-14 18:38:44.000000 compas_model-0.4.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 18:38:44.000000 compas_model-0.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 18:38:58.829944 compas_model-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:38:58.817943 compas_model-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:38:58.817943 compas_model-0.4.2/src/compas_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:38:58.821943 compas_model-0.4.2/src/compas_model/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12192 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/algorithms/collisions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7107 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/algorithms/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/algorithms/nnbrs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:38:58.821943 compas_model-0.4.2/src/compas_model/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/analysis/cra.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:38:58.821943 compas_model-0.4.2/src/compas_model/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7248 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/elements/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11034 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/elements/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/elements/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/elements/plate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:38:58.821943 compas_model-0.4.2/src/compas_model/interactions/
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/interactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/interactions/contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/interactions/interaction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:38:58.821943 compas_model-0.4.2/src/compas_model/loads/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/loads/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:38:58.821943 compas_model-0.4.2/src/compas_model/materials/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/materials/concrete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/materials/material.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/materials/reinforcedconcrete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/materials/steel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/materials/timber.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:38:58.825943 compas_model-0.4.2/src/compas_model/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/models/blockmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/models/elementnode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/models/elementtree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/models/groupnode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/models/interactiongraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20450 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:38:58.825943 compas_model-0.4.2/src/compas_model/notebook/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/notebook/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:38:58.825943 compas_model-0.4.2/src/compas_model/notebook/scene/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/notebook/scene/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/notebook/scene/blockobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/notebook/scene/elementobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/notebook/scene/modelobject.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:38:58.825943 compas_model-0.4.2/src/compas_model/rhino/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/rhino/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:38:58.825943 compas_model-0.4.2/src/compas_model/scene/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/scene/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/scene/blockobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/scene/elementobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/scene/modelobject.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:38:58.825943 compas_model-0.4.2/src/compas_model/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:38:58.825943 compas_model-0.4.2/src/compas_model/viewers/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/viewers/blockmodelviewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:38:44.000000 compas_model-0.4.2/src/compas_model/viewers/modelviewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:38:58.825943 compas_model-0.4.2/src/compas_model.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-14 18:38:58.000000 compas_model-0.4.2/src/compas_model.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-05-14 18:38:58.000000 compas_model-0.4.2/src/compas_model.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 18:38:58.000000 compas_model-0.4.2/src/compas_model.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 18:38:58.000000 compas_model-0.4.2/src/compas_model.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-14 18:38:58.000000 compas_model-0.4.2/src/compas_model.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-14 18:38:58.000000 compas_model-0.4.2/src/compas_model.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:38:58.825943 compas_model-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-14 18:38:44.000000 compas_model-0.4.2/tests/test_algorithms_collider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-14 18:38:44.000000 compas_model-0.4.2/tests/test_interactiongraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-14 18:38:44.000000 compas_model-0.4.2/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-14 18:38:44.000000 compas_model-0.4.2/tests/test_trivial.py
```

### Comparing `compas_model-0.4.1/LICENSE` & `compas_model-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `compas_model-0.4.1/PKG-INFO` & `compas_model-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compas_model
-Version: 0.4.1
+Version: 0.4.2
 Summary: This package provides a universal model datastructure for design, analysis, fabrication, and construction of AEC objects.
 Author-email: tom van mele <tom.v.mele@gmail.com>, petras vestartas <petrasvestartas@gmail.com>
 License: MIT License
         
         ETH Zurich - Block Research Group
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `compas_model-0.4.1/README.md` & `compas_model-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `compas_model-0.4.1/pyproject.toml` & `compas_model-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 ]
 
 # ============================================================================
 # replace bumpversion.cfg
 # ============================================================================
 
 [tool.bumpversion]
-current_version = "0.4.1"
+current_version = "0.4.2"
 message = "Bump version to {new_version}"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "src/compas_model/__init__.py"
 search = "{current_version}"
```

### Comparing `compas_model-0.4.1/src/compas_model/__init__.py` & `compas_model-0.4.2/src/compas_model/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import os
 
 __author__ = ["petras vestartas"]
 __copyright__ = "Block Research Group - ETH Zurich"
 __license__ = "MIT License"
 __email__ = "petrasvestartas@gmail.com"
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 
 HERE = os.path.dirname(__file__)
 
 HOME = os.path.abspath(os.path.join(HERE, "../../"))
 DATA = os.path.abspath(os.path.join(HOME, "data"))
 DOCS = os.path.abspath(os.path.join(HOME, "docs"))
 TEMP = os.path.abspath(os.path.join(HOME, "temp"))
```

### Comparing `compas_model-0.4.1/src/compas_model/algorithms/collisions.py` & `compas_model-0.4.2/src/compas_model/algorithms/collisions.py`

 * *Files identical despite different names*

### Comparing `compas_model-0.4.1/src/compas_model/algorithms/interfaces.py` & `compas_model-0.4.2/src/compas_model/algorithms/interfaces.py`

 * *Files identical despite different names*

### Comparing `compas_model-0.4.1/src/compas_model/analysis/cra.py` & `compas_model-0.4.2/src/compas_model/analysis/cra.py`

 * *Files identical despite different names*

### Comparing `compas_model-0.4.1/src/compas_model/elements/__init__.py` & `compas_model-0.4.2/src/compas_model/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_model-0.4.1/src/compas_model/elements/block.py` & `compas_model-0.4.2/src/compas_model/elements/block.py`

 * *Files identical despite different names*

### Comparing `compas_model-0.4.1/src/compas_model/elements/element.py` & `compas_model-0.4.2/src/compas_model/elements/element.py`

 * *Files identical despite different names*

### Comparing `compas_model-0.4.1/src/compas_model/elements/interface.py` & `compas_model-0.4.2/src/compas_model/elements/interface.py`

 * *Files identical despite different names*

### Comparing `compas_model-0.4.1/src/compas_model/elements/plate.py` & `compas_model-0.4.2/src/compas_model/elements/plate.py`

 * *Files identical despite different names*

### Comparing `compas_model-0.4.1/src/compas_model/interactions/__init__.py` & `compas_model-0.4.2/src/compas_model/interactions/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_model-0.4.1/src/compas_model/interactions/contact.py` & `compas_model-0.4.2/src/compas_model/interactions/contact.py`

 * *Files identical despite different names*

### Comparing `compas_model-0.4.1/src/compas_model/interactions/interaction.py` & `compas_model-0.4.2/src/compas_model/interactions/interaction.py`

 * *Files identical despite different names*

### Comparing `compas_model-0.4.1/src/compas_model/materials/concrete.py` & `compas_model-0.4.2/src/compas_model/materials/concrete.py`

 * *Files identical despite different names*

### Comparing `compas_model-0.4.1/src/compas_model/materials/material.py` & `compas_model-0.4.2/src/compas_model/materials/material.py`

 * *Files identical despite different names*

### Comparing `compas_model-0.4.1/src/compas_model/materials/steel.py` & `compas_model-0.4.2/src/compas_model/materials/steel.py`

 * *Files identical despite different names*

### Comparing `compas_model-0.4.1/src/compas_model/models/elementnode.py` & `compas_model-0.4.2/src/compas_model/models/elementnode.py`

 * *Files identical despite different names*

### Comparing `compas_model-0.4.1/src/compas_model/models/elementtree.py` & `compas_model-0.4.2/src/compas_model/models/elementtree.py`

 * *Files identical despite different names*

### Comparing `compas_model-0.4.1/src/compas_model/models/groupnode.py` & `compas_model-0.4.2/src/compas_model/models/groupnode.py`

 * *Files identical despite different names*

### Comparing `compas_model-0.4.1/src/compas_model/models/interactiongraph.py` & `compas_model-0.4.2/src/compas_model/models/interactiongraph.py`

 * *Files identical despite different names*

### Comparing `compas_model-0.4.1/src/compas_model/models/model.py` & `compas_model-0.4.2/src/compas_model/models/model.py`

 * *Files identical despite different names*

### Comparing `compas_model-0.4.1/src/compas_model/notebook/scene/__init__.py` & `compas_model-0.4.2/src/compas_model/notebook/scene/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_model-0.4.1/src/compas_model/notebook/scene/blockobject.py` & `compas_model-0.4.2/src/compas_model/notebook/scene/blockobject.py`

 * *Files identical despite different names*

### Comparing `compas_model-0.4.1/src/compas_model/notebook/scene/modelobject.py` & `compas_model-0.4.2/src/compas_model/notebook/scene/modelobject.py`

 * *Files identical despite different names*

### Comparing `compas_model-0.4.1/src/compas_model/scene/__init__.py` & `compas_model-0.4.2/src/compas_model/scene/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_model-0.4.1/src/compas_model/scene/elementobject.py` & `compas_model-0.4.2/src/compas_model/scene/elementobject.py`

 * *Files identical despite different names*

### Comparing `compas_model-0.4.1/src/compas_model/scene/modelobject.py` & `compas_model-0.4.2/src/compas_model/scene/modelobject.py`

 * *Files identical despite different names*

### Comparing `compas_model-0.4.1/src/compas_model.egg-info/PKG-INFO` & `compas_model-0.4.2/src/compas_model.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compas_model
-Version: 0.4.1
+Version: 0.4.2
 Summary: This package provides a universal model datastructure for design, analysis, fabrication, and construction of AEC objects.
 Author-email: tom van mele <tom.v.mele@gmail.com>, petras vestartas <petrasvestartas@gmail.com>
 License: MIT License
         
         ETH Zurich - Block Research Group
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `compas_model-0.4.1/src/compas_model.egg-info/SOURCES.txt` & `compas_model-0.4.2/src/compas_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `compas_model-0.4.1/tests/test_algorithms_collider.py` & `compas_model-0.4.2/tests/test_algorithms_collider.py`

 * *Files identical despite different names*

### Comparing `compas_model-0.4.1/tests/test_interactiongraph.py` & `compas_model-0.4.2/tests/test_interactiongraph.py`

 * *Files identical despite different names*

### Comparing `compas_model-0.4.1/tests/test_model.py` & `compas_model-0.4.2/tests/test_model.py`

 * *Files identical despite different names*

