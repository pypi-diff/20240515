# Comparing `tmp/fontprimer-0.2.0.tar.gz` & `tmp/fontprimer-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fontprimer-0.2.0.tar", last modified: Wed May  8 09:32:36 2024, max compression
+gzip compressed data, was "fontprimer-0.2.1.tar", last modified: Wed May 15 13:50:14 2024, max compression
```

## Comparing `fontprimer-0.2.0.tar` & `fontprimer-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 09:32:36.176988 fontprimer-0.2.0/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 09:32:36.174671 fontprimer-0.2.0/Lib/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 09:32:36.175687 fontprimer-0.2.0/Lib/fontprimer/
--rw-r--r--   0 simon      (501) staff       (20)    12583 2024-05-08 09:08:56.000000 fontprimer-0.2.0/Lib/fontprimer/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2337 2023-10-27 13:45:30.000000 fontprimer-0.2.0/Lib/fontprimer/colrguidelines.py
--rw-r--r--   0 simon      (501) staff       (20)     3946 2023-10-27 12:18:02.000000 fontprimer-0.2.0/Lib/fontprimer/guidelines.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 09:32:36.176519 fontprimer-0.2.0/Lib/fontprimer.egg-info/
--rw-r--r--   0 simon      (501) staff       (20)      279 2024-05-08 09:32:36.000000 fontprimer-0.2.0/Lib/fontprimer.egg-info/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)      292 2024-05-08 09:32:36.000000 fontprimer-0.2.0/Lib/fontprimer.egg-info/SOURCES.txt
--rw-r--r--   0 simon      (501) staff       (20)        1 2024-05-08 09:32:36.000000 fontprimer-0.2.0/Lib/fontprimer.egg-info/dependency_links.txt
--rw-r--r--   0 simon      (501) staff       (20)       38 2024-05-08 09:32:36.000000 fontprimer-0.2.0/Lib/fontprimer.egg-info/requires.txt
--rw-r--r--   0 simon      (501) staff       (20)       11 2024-05-08 09:32:36.000000 fontprimer-0.2.0/Lib/fontprimer.egg-info/top_level.txt
--rw-r--r--   0 simon      (501) staff       (20)      279 2024-05-08 09:32:36.176769 fontprimer-0.2.0/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)      525 2024-05-08 09:26:49.000000 fontprimer-0.2.0/pyproject.toml
--rw-r--r--   0 simon      (501) staff       (20)       38 2024-05-08 09:32:36.177035 fontprimer-0.2.0/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-15 13:50:14.439834 fontprimer-0.2.1/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-15 13:50:14.436380 fontprimer-0.2.1/Lib/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-15 13:50:14.437726 fontprimer-0.2.1/Lib/fontprimer/
+-rw-r--r--   0 simon      (501) staff       (20)    12583 2024-05-08 09:08:56.000000 fontprimer-0.2.1/Lib/fontprimer/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2337 2023-10-27 13:45:30.000000 fontprimer-0.2.1/Lib/fontprimer/colrguidelines.py
+-rw-r--r--   0 simon      (501) staff       (20)     4121 2024-05-15 13:37:36.000000 fontprimer-0.2.1/Lib/fontprimer/guidelines.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-15 13:50:14.439069 fontprimer-0.2.1/Lib/fontprimer.egg-info/
+-rw-r--r--   0 simon      (501) staff       (20)      279 2024-05-15 13:50:14.000000 fontprimer-0.2.1/Lib/fontprimer.egg-info/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)      292 2024-05-15 13:50:14.000000 fontprimer-0.2.1/Lib/fontprimer.egg-info/SOURCES.txt
+-rw-r--r--   0 simon      (501) staff       (20)        1 2024-05-15 13:50:14.000000 fontprimer-0.2.1/Lib/fontprimer.egg-info/dependency_links.txt
+-rw-r--r--   0 simon      (501) staff       (20)       38 2024-05-15 13:50:14.000000 fontprimer-0.2.1/Lib/fontprimer.egg-info/requires.txt
+-rw-r--r--   0 simon      (501) staff       (20)       11 2024-05-15 13:50:14.000000 fontprimer-0.2.1/Lib/fontprimer.egg-info/top_level.txt
+-rw-r--r--   0 simon      (501) staff       (20)      279 2024-05-15 13:50:14.439489 fontprimer-0.2.1/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)      525 2024-05-08 09:26:49.000000 fontprimer-0.2.1/pyproject.toml
+-rw-r--r--   0 simon      (501) staff       (20)       38 2024-05-15 13:50:14.439913 fontprimer-0.2.1/setup.cfg
```

### Comparing `fontprimer-0.2.0/Lib/fontprimer/__init__.py` & `fontprimer-0.2.1/Lib/fontprimer/__init__.py`

 * *Files identical despite different names*

### Comparing `fontprimer-0.2.0/Lib/fontprimer/colrguidelines.py` & `fontprimer-0.2.1/Lib/fontprimer/colrguidelines.py`

 * *Files identical despite different names*

### Comparing `fontprimer-0.2.0/Lib/fontprimer/guidelines.py` & `fontprimer-0.2.1/Lib/fontprimer/guidelines.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,98 +1,121 @@
 from glyphsLib.classes import GSLINE, GSFont, GSNode, GSPath, GSGlyph, GSLayer
 
 
 # from https://github.com/mekkablue/Glyphs-Scripts/blob/a4421210dd17305e3205b7ca998cab579b778bf6/Paths/Fill%20Up%20with%20Rectangles.py
 def drawRect(myBottomLeft, myTopRight):
     myRect = GSPath()
-    myCoordinates = [[myBottomLeft[0], myBottomLeft[1]], [myTopRight[0], myBottomLeft[1]], [myTopRight[0], myTopRight[1]], [myBottomLeft[0], myTopRight[1]]]
+    myCoordinates = [
+        [myBottomLeft[0], myBottomLeft[1]],
+        [myTopRight[0], myBottomLeft[1]],
+        [myTopRight[0], myTopRight[1]],
+        [myBottomLeft[0], myTopRight[1]],
+    ]
 
     for thisPoint in myCoordinates:
-      newNode = GSNode((thisPoint[0], thisPoint[1]), GSLINE)
-      myRect.nodes.append(newNode)
+        newNode = GSNode((thisPoint[0], thisPoint[1]), GSLINE)
+        myRect.nodes.append(newNode)
 
     myRect.closed = True
     return myRect
 
+
 def decomposed_paths(layer):
     newpaths = [l.clone() for l in layer.paths]
     for component in layer.components:
         transform = component.transform
         to_append = decomposed_paths(component.layer)
         for path in to_append:
             path.applyTransform(transform)
         newpaths += to_append
     return newpaths
 
+
 def decompose_all_layers(font):
     for glyph in font.glyphs:
         for layer in glyph.layers:
             layer.shapes = list(layer.paths) + decomposed_paths(layer)
 
+
 def add_guidelines(font, args):
     for glyph in font.glyphs:
         if glyph.name.startswith("_"):
             continue
         if not glyph.export:
             continue
         # Skip combining marks
         for layer in glyph.layers:
             # If this has any components which don't start in "_part", skip it
-            if layer.components and not all(component.name.startswith("_part") for component in layer.components):
+            if layer.components and not all(
+                component.name.startswith("_part") for component in layer.components
+            ):
                 continue
             # Skip anything with underscore anchors
             if any(anchor.name.startswith("_") for anchor in layer.anchors):
                 continue
             master = layer.master
             heightsAndThicknesses = [
                 (master.descender, args.default_thickness),
-                (0, args.thicker_thickness),
+                (0 + args.thicker_thickness / 2, args.thicker_thickness),
                 (master.xHeight, args.default_thickness),
-                (master.ascender, args.default_thickness)
+                (master.ascender, args.default_thickness),
             ]
-            
+
             for height, thickness in heightsAndThicknesses:
-                bottomLeft = (-args.overlap, height)
-                topRight = (layer.width+args.overlap, height+thickness)
+                bottomLeft = (-args.overlap, height - thickness / 2)
+                topRight = (layer.width + args.overlap, height + thickness / 2)
                 layerRect = drawRect(bottomLeft, topRight)
                 layer.shapes.append(layerRect)
 
+
 def add_guideline_glyph(font, thickness):
     if "_guide" in font.glyphs:
         return
     font.glyphs.append(GSGlyph("_guide"))
     for master in font.masters:
         layer = GSLayer()
         layer.associatedMasterId = master.id
         layer.layerId = master.id
         layer.width = 1000
-        layer.shapes = [ GSPath() ]
+        layer.shapes = [GSPath()]
         layer.shapes[0].nodes = [
-                GSNode((0, 0), GSLINE),
-                GSNode((1000, 0), GSLINE),
-                GSNode((1000, thickness), GSLINE),
-                GSNode((0, thickness), GSLINE)
-            ]
+            GSNode((0, 0), GSLINE),
+            GSNode((1000, 0), GSLINE),
+            GSNode((1000, thickness), GSLINE),
+            GSNode((0, thickness), GSLINE),
+        ]
         font.glyphs["_guide"].layers.append(layer)
     pass
 
+
 if __name__ == "__main__":
     import argparse
+
     parser = argparse.ArgumentParser()
     parser.add_argument("font", help="Glyphs file", metavar="GLYPHS")
-    parser.add_argument("--color", action="store_true", help="Output a single stroke for color processing")
+    parser.add_argument(
+        "--color",
+        action="store_true",
+        help="Output a single stroke for color processing",
+    )
     parser.add_argument("--output", "-o", help="Output file", metavar="GLYPHS")
-    parser.add_argument("--overlap", help="Overlap of the guidelines", type=int, default=10)
-    parser.add_argument("--default-thickness", help="Default guideline thickness", type=int, default=16)
-    parser.add_argument("--thicker-thickness", help="Thicker guideline thickness", type=int, default=32)
+    parser.add_argument(
+        "--overlap", help="Overlap of the guidelines", type=int, default=10
+    )
+    parser.add_argument(
+        "--default-thickness", help="Default guideline thickness", type=int, default=16
+    )
+    parser.add_argument(
+        "--thicker-thickness", help="Thicker guideline thickness", type=int, default=32
+    )
     args = parser.parse_args()
 
     if not args.output:
         args.output = args.font
     font = GSFont(args.font)
     if args.color:
         add_guideline_glyph(font, args.default_thickness)
     else:
         decompose_all_layers(font)
         add_guidelines(font, args)
-    print("Saving on "+args.output)
+    print("Saving on " + args.output)
     font.save(args.output)
```

### Comparing `fontprimer-0.2.0/pyproject.toml` & `fontprimer-0.2.1/pyproject.toml`

 * *Files identical despite different names*

