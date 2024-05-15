# Comparing `tmp/compas_ifc-0.4.0.tar.gz` & `tmp/compas_ifc-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compas_ifc-0.4.0.tar", last modified: Tue May 14 10:30:56 2024, max compression
+gzip compressed data, was "compas_ifc-0.4.1.tar", last modified: Wed May 15 10:36:13 2024, max compression
```

## Comparing `compas_ifc-0.4.0.tar` & `compas_ifc-0.4.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 10:30:56.775451 compas_ifc-0.4.0/
--rw-rw-rw-   0        0        0      167 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/AUTHORS.md
--rw-rw-rw-   0        0        0     1265 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/CHANGELOG.md
--rw-rw-rw-   0        0        0     1069 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/LICENSE
--rw-rw-rw-   0        0        0      442 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5418 2024-05-14 10:30:56.775451 compas_ifc-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     2457 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/README.md
--rw-rw-rw-   0        0        0     3919 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0      126 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       18 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 10:30:56.775451 compas_ifc-0.4.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-14 10:30:56.744194 compas_ifc-0.4.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-14 10:30:56.759827 compas_ifc-0.4.0/src/compas_ifc/
--rw-rw-rw-   0        0        0      993 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/__init__.py
--rw-rw-rw-   0        0        0       38 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/__main__.py
--rw-rw-rw-   0        0        0     3096 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/attributes.py
-drwxrwxrwx   0        0        0        0 2024-05-14 10:30:56.759827 compas_ifc-0.4.0/src/compas_ifc/brep/
--rw-rw-rw-   0        0        0      445 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/brep/__init__.py
--rw-rw-rw-   0        0        0      787 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/brep/tessellatedbrep.py
--rw-rw-rw-   0        0        0     1789 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/brep/tessellatedbrepobject.py
-drwxrwxrwx   0        0        0        0 2024-05-14 10:30:56.759827 compas_ifc-0.4.0/src/compas_ifc/entities/
--rw-rw-rw-   0        0        0     6698 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/entities/__init__.py
--rw-rw-rw-   0        0        0     2997 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/entities/building.py
--rw-rw-rw-   0        0        0     3341 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/entities/buildingelements.py
--rw-rw-rw-   0        0        0     3152 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/entities/buildingstorey.py
--rw-rw-rw-   0        0        0     1109 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/entities/element.py
--rw-rw-rw-   0        0        0     7962 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/entities/entity.py
--rw-rw-rw-   0        0        0      169 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/entities/geographicelement.py
--rw-rw-rw-   0        0        0     3943 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/entities/objectdefinition.py
--rw-rw-rw-   0        0        0     6956 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/entities/product.py
--rw-rw-rw-   0        0        0     5607 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/entities/project.py
--rw-rw-rw-   0        0        0      791 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/entities/root.py
--rw-rw-rw-   0        0        0     1764 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/entities/site.py
--rw-rw-rw-   0        0        0      789 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/entities/space.py
--rw-rw-rw-   0        0        0      748 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/entities/spatialelement.py
--rw-rw-rw-   0        0        0     1799 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/helpers.py
--rw-rw-rw-   0        0        0     9510 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/model.py
--rw-rw-rw-   0        0        0     8305 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/reader.py
--rw-rw-rw-   0        0        0     9693 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/representation.py
-drwxrwxrwx   0        0        0        0 2024-05-14 10:30:56.775451 compas_ifc-0.4.0/src/compas_ifc/resources/
--rw-rw-rw-   0        0        0     4270 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/resources/__init__.py
--rw-rw-rw-   0        0        0    10041 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/resources/brep.py
--rw-rw-rw-   0        0        0     2099 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/resources/geometricconstraint.py
--rw-rw-rw-   0        0        0     7697 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/resources/geometricmodel.py
--rw-rw-rw-   0        0        0     5366 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/resources/geometry.py
--rw-rw-rw-   0        0        0     1729 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/resources/mesh.py
--rw-rw-rw-   0        0        0     1049 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/resources/primities.py
--rw-rw-rw-   0        0        0     2401 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/resources/representation.py
--rw-rw-rw-   0        0        0     3342 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/resources/shapes.py
-drwxrwxrwx   0        0        0        0 2024-05-14 10:30:56.775451 compas_ifc-0.4.0/src/compas_ifc/viewer/
--rw-rw-rw-   0        0        0      387 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/viewer/__init__.py
--rw-rw-rw-   0        0        0     9349 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/viewer/app.py
--rw-rw-rw-   0        0        0     4177 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/viewer/config.json
-drwxrwxrwx   0        0        0        0 2024-05-14 10:30:56.775451 compas_ifc-0.4.0/src/compas_ifc/viewer/objects/
--rw-rw-rw-   0        0        0      305 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/viewer/objects/__init__.py
--rw-rw-rw-   0        0        0      624 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/viewer/objects/entityobject.py
--rw-rw-rw-   0        0        0      240 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/viewer/objects/projectobject.py
--rw-rw-rw-   0        0        0    13747 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/writer.py
-drwxrwxrwx   0        0        0        0 2024-05-14 10:30:56.775451 compas_ifc-0.4.0/src/compas_ifc.egg-info/
--rw-rw-rw-   0        0        0     5418 2024-05-14 10:30:56.000000 compas_ifc-0.4.0/src/compas_ifc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1768 2024-05-14 10:30:56.000000 compas_ifc-0.4.0/src/compas_ifc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 10:30:56.000000 compas_ifc-0.4.0/src/compas_ifc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-14 10:30:56.000000 compas_ifc-0.4.0/src/compas_ifc.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      139 2024-05-14 10:30:56.000000 compas_ifc-0.4.0/src/compas_ifc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-14 10:30:56.000000 compas_ifc-0.4.0/src/compas_ifc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 10:36:13.851902 compas_ifc-0.4.1/
+-rw-rw-rw-   0        0        0      167 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/AUTHORS.md
+-rw-rw-rw-   0        0        0     1335 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1069 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0      442 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5418 2024-05-15 10:36:13.851902 compas_ifc-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2457 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/README.md
+-rw-rw-rw-   0        0        0     3919 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0      126 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/requirements-dev.txt
+-rw-rw-rw-   0        0        0       18 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 10:36:13.851902 compas_ifc-0.4.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-15 10:36:13.820650 compas_ifc-0.4.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-15 10:36:13.836275 compas_ifc-0.4.1/src/compas_ifc/
+-rw-rw-rw-   0        0        0      993 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/__init__.py
+-rw-rw-rw-   0        0        0       38 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/__main__.py
+-rw-rw-rw-   0        0        0     3096 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/attributes.py
+drwxrwxrwx   0        0        0        0 2024-05-15 10:36:13.836275 compas_ifc-0.4.1/src/compas_ifc/brep/
+-rw-rw-rw-   0        0        0      445 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/brep/__init__.py
+-rw-rw-rw-   0        0        0      787 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/brep/tessellatedbrep.py
+-rw-rw-rw-   0        0        0     1789 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/brep/tessellatedbrepobject.py
+drwxrwxrwx   0        0        0        0 2024-05-15 10:36:13.851902 compas_ifc-0.4.1/src/compas_ifc/entities/
+-rw-rw-rw-   0        0        0     6698 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/entities/__init__.py
+-rw-rw-rw-   0        0        0     2997 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/entities/building.py
+-rw-rw-rw-   0        0        0     3341 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/entities/buildingelements.py
+-rw-rw-rw-   0        0        0     3152 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/entities/buildingstorey.py
+-rw-rw-rw-   0        0        0     1109 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/entities/element.py
+-rw-rw-rw-   0        0        0     7962 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/entities/entity.py
+-rw-rw-rw-   0        0        0      169 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/entities/geographicelement.py
+-rw-rw-rw-   0        0        0     3943 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/entities/objectdefinition.py
+-rw-rw-rw-   0        0        0     6956 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/entities/product.py
+-rw-rw-rw-   0        0        0     5607 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/entities/project.py
+-rw-rw-rw-   0        0        0      791 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/entities/root.py
+-rw-rw-rw-   0        0        0     1764 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/entities/site.py
+-rw-rw-rw-   0        0        0      789 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/entities/space.py
+-rw-rw-rw-   0        0        0      748 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/entities/spatialelement.py
+-rw-rw-rw-   0        0        0     1799 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/helpers.py
+-rw-rw-rw-   0        0        0     9510 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/model.py
+-rw-rw-rw-   0        0        0     8305 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/reader.py
+-rw-rw-rw-   0        0        0     9693 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/representation.py
+drwxrwxrwx   0        0        0        0 2024-05-15 10:36:13.851902 compas_ifc-0.4.1/src/compas_ifc/resources/
+-rw-rw-rw-   0        0        0     4270 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/resources/__init__.py
+-rw-rw-rw-   0        0        0    10041 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/resources/brep.py
+-rw-rw-rw-   0        0        0     2099 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/resources/geometricconstraint.py
+-rw-rw-rw-   0        0        0     7697 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/resources/geometricmodel.py
+-rw-rw-rw-   0        0        0     5366 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/resources/geometry.py
+-rw-rw-rw-   0        0        0     1729 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/resources/mesh.py
+-rw-rw-rw-   0        0        0     1049 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/resources/primities.py
+-rw-rw-rw-   0        0        0     2401 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/resources/representation.py
+-rw-rw-rw-   0        0        0     3342 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/resources/shapes.py
+drwxrwxrwx   0        0        0        0 2024-05-15 10:36:13.851902 compas_ifc-0.4.1/src/compas_ifc/viewer/
+-rw-rw-rw-   0        0        0      387 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/viewer/__init__.py
+-rw-rw-rw-   0        0        0     9349 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/viewer/app.py
+-rw-rw-rw-   0        0        0     4177 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/viewer/config.json
+drwxrwxrwx   0        0        0        0 2024-05-15 10:36:13.851902 compas_ifc-0.4.1/src/compas_ifc/viewer/objects/
+-rw-rw-rw-   0        0        0      305 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/viewer/objects/__init__.py
+-rw-rw-rw-   0        0        0      624 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/viewer/objects/entityobject.py
+-rw-rw-rw-   0        0        0      240 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/viewer/objects/projectobject.py
+-rw-rw-rw-   0        0        0    13747 2024-05-15 10:35:51.000000 compas_ifc-0.4.1/src/compas_ifc/writer.py
+drwxrwxrwx   0        0        0        0 2024-05-15 10:36:13.851902 compas_ifc-0.4.1/src/compas_ifc.egg-info/
+-rw-rw-rw-   0        0        0     5418 2024-05-15 10:36:13.000000 compas_ifc-0.4.1/src/compas_ifc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1768 2024-05-15 10:36:13.000000 compas_ifc-0.4.1/src/compas_ifc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 10:36:13.000000 compas_ifc-0.4.1/src/compas_ifc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-15 10:36:13.000000 compas_ifc-0.4.1/src/compas_ifc.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      139 2024-05-15 10:36:13.000000 compas_ifc-0.4.1/src/compas_ifc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-15 10:36:13.000000 compas_ifc-0.4.1/src/compas_ifc.egg-info/top_level.txt
```

### Comparing `compas_ifc-0.4.0/CHANGELOG.md` & `compas_ifc-0.4.1/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.4.1] 2024-05-15
+
+### Added
+
+### Changed
+
+### Removed
+
+
 ## [0.4.0] 2024-05-14
 
 ### Added
 
 * Added support to export to `IFC2x3`.
 * Added support pre-load geometries using `multi-processing`.
```

### Comparing `compas_ifc-0.4.0/LICENSE` & `compas_ifc-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.4.0/PKG-INFO` & `compas_ifc-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compas_ifc
-Version: 0.4.0
+Version: 0.4.1
 Summary: High-level IFC interface for COMPAS.
 Author-email: Tom Van Mele <van.mele@arch.ethz.ch>, Li Chen <li.chen@arch.ethz.ch>
 License: MIT License
         
         ETH Zurich
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `compas_ifc-0.4.0/README.md` & `compas_ifc-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.4.0/pyproject.toml` & `compas_ifc-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 ]
 
 # ============================================================================
 # replace bumpversion.cfg
 # ============================================================================
 
 [tool.bumpversion]
-current_version = "0.4.0"
+current_version = "0.4.1"
 message = "Bump version to {new_version}"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "src/compas_ifc/__init__.py"
 search = "{current_version}"
```

### Comparing `compas_ifc-0.4.0/src/compas_ifc/__init__.py` & `compas_ifc-0.4.1/src/compas_ifc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import os
 
 
 __author__ = ["tom van mele"]
 __copyright__ = "ETH Zurich"
 __license__ = "MIT License"
 __email__ = "van.mele@arch.ethz.ch"
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 
 
 HERE = os.path.dirname(__file__)
 
 HOME = os.path.abspath(os.path.join(HERE, "../../"))
 DATA = os.path.abspath(os.path.join(HOME, "data"))
 DOCS = os.path.abspath(os.path.join(HOME, "docs"))
```

### Comparing `compas_ifc-0.4.0/src/compas_ifc/attributes.py` & `compas_ifc-0.4.1/src/compas_ifc/attributes.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.4.0/src/compas_ifc/brep/tessellatedbrep.py` & `compas_ifc-0.4.1/src/compas_ifc/brep/tessellatedbrep.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.4.0/src/compas_ifc/brep/tessellatedbrepobject.py` & `compas_ifc-0.4.1/src/compas_ifc/brep/tessellatedbrepobject.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,23 +10,23 @@
     def __init__(self, tessellatedbrep: TessellatedBrep, facecolors=None, **kwargs):
         super().__init__(item=tessellatedbrep, **kwargs)
         self.tessellatedbrep = tessellatedbrep
         self.facecolors = facecolors
 
         # TODO: it is not facecolors, it is verexcolor
         if not self.facecolors:
-            self.facecolors = [Color(0.5, 0.5, 0.5) for _ in range(len(self.tessellatedbrep.faces) * 3)]
+            self.facecolors = [Color(0.9, 0.9, 0.9) for _ in range(len(self.tessellatedbrep.faces) * 3)]
 
     def _read_points_data(self):
         pass
 
     def _read_lines_data(self):
         positions = self.tessellatedbrep.vertices.tolist()
         elements = self.tessellatedbrep.edges.tolist()
-        colors = [Color(0.5, 0.5, 0.5)] * len(elements)
+        colors = [Color(0.1, 0.1, 0.1)] * len(elements)
         return positions, colors, elements
 
     def _read_frontfaces_data(self):
         positions = self.tessellatedbrep.vertices[self.tessellatedbrep.faces].reshape(-1, 3).tolist()
         elements = np.arange(len(positions) * 3).reshape(-1, 3).tolist()
         colors = [Color(*color) for color in self.facecolors]
         return positions, colors, elements
```

### Comparing `compas_ifc-0.4.0/src/compas_ifc/entities/__init__.py` & `compas_ifc-0.4.1/src/compas_ifc/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.4.0/src/compas_ifc/entities/building.py` & `compas_ifc-0.4.1/src/compas_ifc/entities/building.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.4.0/src/compas_ifc/entities/buildingelements.py` & `compas_ifc-0.4.1/src/compas_ifc/entities/buildingelements.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.4.0/src/compas_ifc/entities/buildingstorey.py` & `compas_ifc-0.4.1/src/compas_ifc/entities/buildingstorey.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.4.0/src/compas_ifc/entities/element.py` & `compas_ifc-0.4.1/src/compas_ifc/entities/element.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.4.0/src/compas_ifc/entities/entity.py` & `compas_ifc-0.4.1/src/compas_ifc/entities/entity.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.4.0/src/compas_ifc/entities/objectdefinition.py` & `compas_ifc-0.4.1/src/compas_ifc/entities/objectdefinition.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.4.0/src/compas_ifc/entities/product.py` & `compas_ifc-0.4.1/src/compas_ifc/entities/product.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.4.0/src/compas_ifc/entities/project.py` & `compas_ifc-0.4.1/src/compas_ifc/entities/project.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.4.0/src/compas_ifc/entities/root.py` & `compas_ifc-0.4.1/src/compas_ifc/entities/root.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.4.0/src/compas_ifc/entities/site.py` & `compas_ifc-0.4.1/src/compas_ifc/entities/site.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.4.0/src/compas_ifc/entities/space.py` & `compas_ifc-0.4.1/src/compas_ifc/entities/space.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.4.0/src/compas_ifc/entities/spatialelement.py` & `compas_ifc-0.4.1/src/compas_ifc/entities/spatialelement.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.4.0/src/compas_ifc/helpers.py` & `compas_ifc-0.4.1/src/compas_ifc/helpers.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.4.0/src/compas_ifc/model.py` & `compas_ifc-0.4.1/src/compas_ifc/model.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.4.0/src/compas_ifc/reader.py` & `compas_ifc-0.4.1/src/compas_ifc/reader.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.4.0/src/compas_ifc/representation.py` & `compas_ifc-0.4.1/src/compas_ifc/representation.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.4.0/src/compas_ifc/resources/__init__.py` & `compas_ifc-0.4.1/src/compas_ifc/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.4.0/src/compas_ifc/resources/brep.py` & `compas_ifc-0.4.1/src/compas_ifc/resources/brep.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.4.0/src/compas_ifc/resources/geometricconstraint.py` & `compas_ifc-0.4.1/src/compas_ifc/resources/geometricconstraint.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.4.0/src/compas_ifc/resources/geometricmodel.py` & `compas_ifc-0.4.1/src/compas_ifc/resources/geometricmodel.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.4.0/src/compas_ifc/resources/geometry.py` & `compas_ifc-0.4.1/src/compas_ifc/resources/geometry.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.4.0/src/compas_ifc/resources/mesh.py` & `compas_ifc-0.4.1/src/compas_ifc/resources/mesh.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.4.0/src/compas_ifc/resources/primities.py` & `compas_ifc-0.4.1/src/compas_ifc/resources/primities.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.4.0/src/compas_ifc/resources/representation.py` & `compas_ifc-0.4.1/src/compas_ifc/resources/representation.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.4.0/src/compas_ifc/resources/shapes.py` & `compas_ifc-0.4.1/src/compas_ifc/resources/shapes.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.4.0/src/compas_ifc/viewer/app.py` & `compas_ifc-0.4.1/src/compas_ifc/viewer/app.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.4.0/src/compas_ifc/viewer/config.json` & `compas_ifc-0.4.1/src/compas_ifc/viewer/config.json`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.4.0/src/compas_ifc/viewer/objects/entityobject.py` & `compas_ifc-0.4.1/src/compas_ifc/viewer/objects/entityobject.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.4.0/src/compas_ifc/writer.py` & `compas_ifc-0.4.1/src/compas_ifc/writer.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.4.0/src/compas_ifc.egg-info/PKG-INFO` & `compas_ifc-0.4.1/src/compas_ifc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compas_ifc
-Version: 0.4.0
+Version: 0.4.1
 Summary: High-level IFC interface for COMPAS.
 Author-email: Tom Van Mele <van.mele@arch.ethz.ch>, Li Chen <li.chen@arch.ethz.ch>
 License: MIT License
         
         ETH Zurich
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `compas_ifc-0.4.0/src/compas_ifc.egg-info/SOURCES.txt` & `compas_ifc-0.4.1/src/compas_ifc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

