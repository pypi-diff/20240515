# Comparing `tmp/kaxe-0.1.1.tar.gz` & `tmp/kaxe-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaxe-0.1.1.tar", last modified: Thu Feb 22 12:01:38 2024, max compression
+gzip compressed data, was "kaxe-0.1.2.tar", last modified: Tue May 14 21:04:39 2024, max compression
```

## Comparing `kaxe-0.1.1.tar` & `kaxe-0.1.2.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:01:38.202245 kaxe-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-22 12:01:29.000000 kaxe-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-22 12:01:29.000000 kaxe-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-02-22 12:01:38.202245 kaxe-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-02-22 12:01:29.000000 kaxe-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-02-22 12:01:29.000000 kaxe-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 12:01:38.202245 kaxe-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:01:38.178244 kaxe-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:01:38.182244 kaxe-0.1.1/src/kaxe/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:01:38.182244 kaxe-0.1.1/src/kaxe/chart/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/chart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9806 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/chart/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/chart/pie.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:01:38.182244 kaxe-0.1.1/src/kaxe/core/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9410 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/core/axis.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/core/fileloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/core/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/core/legend.py
--rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/core/marker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/core/round.py
--rw-r--r--   0 runner    (1001) docker     (127)    12389 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/core/shapes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/core/styles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/core/symbol.py
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/core/text.py
--rw-r--r--   0 runner    (1001) docker     (127)    10392 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/core/window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:01:38.186245 kaxe-0.1.1/src/kaxe/data/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/data/excel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:01:38.186245 kaxe-0.1.1/src/kaxe/objects/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/objects/equation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/objects/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/objects/map.py
--rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/objects/mapdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/objects/pillar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/objects/point.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:01:38.186245 kaxe-0.1.1/src/kaxe/plot/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/plot/box.py
--rw-r--r--   0 runner    (1001) docker     (127)    20972 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/plot/diagonal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/plot/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     8882 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/plot/polar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/plot/standard.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/plot/themes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:01:38.186245 kaxe-0.1.1/src/kaxe/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:01:38.202245 kaxe-0.1.1/src/kaxe/resources/computer-modern-family/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/resources/computer-modern-family/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   185780 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.bright-oblique.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   145840 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.bright-roman.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   146988 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.bright-semibold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   183844 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.bright-semiboldoblique.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   291936 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.classical-serif-italic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   205612 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.concrete-bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   276804 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.concrete-bolditalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   275808 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.concrete-italic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   210868 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.concrete-roman.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   200524 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.sans-serif-bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   234180 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.sans-serif-boldoblique.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   199792 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.sans-serif-demi-condensed-demicondensed.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   149416 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.sans-serif-medium.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   185920 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.sans-serif-oblique.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   221904 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.serif-bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   285096 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.serif-bolditalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   253980 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.serif-extra-boldslanted.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   267732 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.serif-extra-romanslanted.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   289276 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.serif-italic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   235656 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.serif-roman.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   240848 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.serif-upright-italic-uprightitalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   227272 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.typewriter-text-bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   256112 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.typewriter-text-bolditalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   249680 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.typewriter-text-italic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   213632 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.typewriter-text-light.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   247768 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.typewriter-text-lightoblique.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   214528 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.typewriter-text-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   232632 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.typewriter-text-variable-width-italic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   193880 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.typewriter-text-variable-width-medium.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/resources/computer-modern-family/readme.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-02-22 12:01:29.000000 kaxe-0.1.1/src/kaxe/resources/symboltriangle.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:01:38.202245 kaxe-0.1.1/src/kaxe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-02-22 12:01:38.000000 kaxe-0.1.1/src/kaxe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-02-22 12:01:38.000000 kaxe-0.1.1/src/kaxe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 12:01:38.000000 kaxe-0.1.1/src/kaxe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-22 12:01:38.000000 kaxe-0.1.1/src/kaxe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-22 12:01:38.000000 kaxe-0.1.1/src/kaxe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:01:38.202245 kaxe-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    18489 2024-02-22 12:01:30.000000 kaxe-0.1.1/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:04:39.940588 kaxe-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-14 21:04:35.000000 kaxe-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 21:04:35.000000 kaxe-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-05-14 21:04:39.940588 kaxe-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-14 21:04:35.000000 kaxe-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-14 21:04:35.000000 kaxe-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 21:04:39.940588 kaxe-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:04:39.916588 kaxe-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:04:39.916588 kaxe-0.1.2/src/kaxe/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:04:39.920588 kaxe-0.1.2/src/kaxe/chart/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/chart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9806 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/chart/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/chart/pie.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:04:39.920588 kaxe-0.1.2/src/kaxe/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9410 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/core/axis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/core/fileloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/core/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/core/legend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/core/marker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/core/round.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12389 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/core/shapes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/core/styles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/core/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/core/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10652 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/core/window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:04:39.920588 kaxe-0.1.2/src/kaxe/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/data/excel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:04:39.924588 kaxe-0.1.2/src/kaxe/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/objects/equation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/objects/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/objects/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/objects/mapdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/objects/pillar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/objects/point.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:04:39.924588 kaxe-0.1.2/src/kaxe/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/plot/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20972 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/plot/diagonal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/plot/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8882 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/plot/polar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/plot/standard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/plot/themes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:04:39.924588 kaxe-0.1.2/src/kaxe/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:04:39.936588 kaxe-0.1.2/src/kaxe/resources/computer-modern-family/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/resources/computer-modern-family/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   185780 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.bright-oblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   145840 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.bright-roman.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   146988 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.bright-semibold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   183844 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.bright-semiboldoblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   291936 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.classical-serif-italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   205612 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.concrete-bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   276804 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.concrete-bolditalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   275808 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.concrete-italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   210868 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.concrete-roman.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   200524 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.sans-serif-bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   234180 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.sans-serif-boldoblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   199792 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.sans-serif-demi-condensed-demicondensed.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   149416 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.sans-serif-medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   185920 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.sans-serif-oblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   221904 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.serif-bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   285096 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.serif-bolditalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   253980 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.serif-extra-boldslanted.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   267732 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.serif-extra-romanslanted.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   289276 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.serif-italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   235656 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.serif-roman.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   240848 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.serif-upright-italic-uprightitalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   227272 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.typewriter-text-bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   256112 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.typewriter-text-bolditalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   249680 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.typewriter-text-italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   213632 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.typewriter-text-light.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   247768 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.typewriter-text-lightoblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   214528 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.typewriter-text-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   232632 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.typewriter-text-variable-width-italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   193880 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.typewriter-text-variable-width-medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/resources/computer-modern-family/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-14 21:04:35.000000 kaxe-0.1.2/src/kaxe/resources/symboltriangle.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:04:39.936588 kaxe-0.1.2/src/kaxe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-05-14 21:04:39.000000 kaxe-0.1.2/src/kaxe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-14 21:04:39.000000 kaxe-0.1.2/src/kaxe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 21:04:39.000000 kaxe-0.1.2/src/kaxe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-14 21:04:39.000000 kaxe-0.1.2/src/kaxe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 21:04:39.000000 kaxe-0.1.2/src/kaxe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:04:39.936588 kaxe-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    18489 2024-05-14 21:04:35.000000 kaxe-0.1.2/tests/test.py
```

### Comparing `kaxe-0.1.1/LICENSE` & `kaxe-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/PKG-INFO` & `kaxe-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaxe
-Version: 0.1.1
+Version: 0.1.2
 Summary: A small graphing tool for functions, points, equations and more
 Author-email: Valter Yde Daugberg <valter@hotmail.com>
 Project-URL: Homepage, https://github.com/valteryde/kaxe
 Project-URL: Issues, https://github.com/valteryde/kaxe/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `kaxe-0.1.1/README.md` & `kaxe-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/pyproject.toml` & `kaxe-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "kaxe"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Valter Yde Daugberg", email="valter@hotmail.com" },
 ]
 description = "A small graphing tool for functions, points, equations and more"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `kaxe-0.1.1/src/kaxe/chart/bar.py` & `kaxe-0.1.2/src/kaxe/chart/bar.py`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/chart/pie.py` & `kaxe-0.1.2/src/kaxe/chart/pie.py`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/core/axis.py` & `kaxe-0.1.2/src/kaxe/core/axis.py`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/core/helper.py` & `kaxe-0.1.2/src/kaxe/core/helper.py`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/core/legend.py` & `kaxe-0.1.2/src/kaxe/core/legend.py`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/core/marker.py` & `kaxe-0.1.2/src/kaxe/core/marker.py`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/core/round.py` & `kaxe-0.1.2/src/kaxe/core/round.py`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/core/shapes.py` & `kaxe-0.1.2/src/kaxe/core/shapes.py`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/core/styles.py` & `kaxe-0.1.2/src/kaxe/core/styles.py`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/core/symbol.py` & `kaxe-0.1.2/src/kaxe/core/symbol.py`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/core/text.py` & `kaxe-0.1.2/src/kaxe/core/text.py`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/core/window.py` & `kaxe-0.1.2/src/kaxe/core/window.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,20 +162,31 @@
                     vertical.append(i.farTop)
                     vertical.append(i.farBottom)
                 except AttributeError:
                     continue
             
             try:
                 if not self.windowAxis[0]: self.windowAxis[0] = min(horizontal)
+            except Exception as e:
+                self.windowAxis[2] = -10
+            
+            try:
                 if not self.windowAxis[1]: self.windowAxis[1] = max(horizontal)
+            except Exception as e:
+                self.windowAxis[1] = 10
+            
+            try:
                 if not self.windowAxis[2]: self.windowAxis[2] = min(vertical)
+            except Exception as e:
+                self.windowAxis[2] = -5
+            
+            try:
                 if not self.windowAxis[3]: self.windowAxis[3] = max(vertical)
             except Exception as e:
-                logging.warn(e) # not tested
-                self.windowAxis = [-10, 10, -5, 5]
+                self.windowAxis[3] = 5
 
 
     # baking
     def __bake__(self):
         # finish making plot
         # fit "plot" into window 
         startTime = time.time()        
@@ -348,8 +359,8 @@
         return: x,y position according to basis (1,0), (0,1) in abstract space
         """
 
         p = [None, None]
         if not x is None: p[0] = (x+self.offset[0]-self.padding[0])/self.scale[0]
         if not y is None: p[1] = (y+self.offset[1]-self.padding[1])/self.scale[1]
 
-        return p
+        return p
```

### Comparing `kaxe-0.1.1/src/kaxe/data/excel.py` & `kaxe-0.1.2/src/kaxe/data/excel.py`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/objects/equation.py` & `kaxe-0.1.2/src/kaxe/objects/equation.py`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/objects/function.py` & `kaxe-0.1.2/src/kaxe/objects/function.py`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/objects/map.py` & `kaxe-0.1.2/src/kaxe/objects/map.py`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/objects/mapdata.py` & `kaxe-0.1.2/src/kaxe/objects/mapdata.py`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/objects/pillar.py` & `kaxe-0.1.2/src/kaxe/objects/pillar.py`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/objects/point.py` & `kaxe-0.1.2/src/kaxe/objects/point.py`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/plot/box.py` & `kaxe-0.1.2/src/kaxe/plot/box.py`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/plot/diagonal.py` & `kaxe-0.1.2/src/kaxe/plot/diagonal.py`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/plot/log.py` & `kaxe-0.1.2/src/kaxe/plot/log.py`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/plot/polar.py` & `kaxe-0.1.2/src/kaxe/plot/polar.py`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/plot/standard.py` & `kaxe-0.1.2/src/kaxe/plot/standard.py`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.bright-oblique.ttf` & `kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.bright-oblique.ttf`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.bright-roman.ttf` & `kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.bright-roman.ttf`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.bright-semibold.ttf` & `kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.bright-semibold.ttf`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.bright-semiboldoblique.ttf` & `kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.bright-semiboldoblique.ttf`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.classical-serif-italic.ttf` & `kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.classical-serif-italic.ttf`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.concrete-bold.ttf` & `kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.concrete-bold.ttf`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.concrete-bolditalic.ttf` & `kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.concrete-bolditalic.ttf`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.concrete-italic.ttf` & `kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.concrete-italic.ttf`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.concrete-roman.ttf` & `kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.concrete-roman.ttf`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.sans-serif-bold.ttf` & `kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.sans-serif-bold.ttf`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.sans-serif-boldoblique.ttf` & `kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.sans-serif-boldoblique.ttf`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.sans-serif-demi-condensed-demicondensed.ttf` & `kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.sans-serif-demi-condensed-demicondensed.ttf`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.sans-serif-medium.ttf` & `kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.sans-serif-medium.ttf`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.sans-serif-oblique.ttf` & `kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.sans-serif-oblique.ttf`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.serif-bold.ttf` & `kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.serif-bold.ttf`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.serif-bolditalic.ttf` & `kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.serif-bolditalic.ttf`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.serif-extra-boldslanted.ttf` & `kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.serif-extra-boldslanted.ttf`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.serif-extra-romanslanted.ttf` & `kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.serif-extra-romanslanted.ttf`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.serif-italic.ttf` & `kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.serif-italic.ttf`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.serif-roman.ttf` & `kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.serif-roman.ttf`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.serif-upright-italic-uprightitalic.ttf` & `kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.serif-upright-italic-uprightitalic.ttf`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.typewriter-text-bold.ttf` & `kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.typewriter-text-bold.ttf`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.typewriter-text-bolditalic.ttf` & `kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.typewriter-text-bolditalic.ttf`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.typewriter-text-italic.ttf` & `kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.typewriter-text-italic.ttf`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.typewriter-text-light.ttf` & `kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.typewriter-text-light.ttf`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.typewriter-text-lightoblique.ttf` & `kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.typewriter-text-lightoblique.ttf`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.typewriter-text-regular.ttf` & `kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.typewriter-text-regular.ttf`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.typewriter-text-variable-width-italic.ttf` & `kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.typewriter-text-variable-width-italic.ttf`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/resources/computer-modern-family/cmu.typewriter-text-variable-width-medium.ttf` & `kaxe-0.1.2/src/kaxe/resources/computer-modern-family/cmu.typewriter-text-variable-width-medium.ttf`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe/resources/symboltriangle.png` & `kaxe-0.1.2/src/kaxe/resources/symboltriangle.png`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/src/kaxe.egg-info/PKG-INFO` & `kaxe-0.1.2/src/kaxe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaxe
-Version: 0.1.1
+Version: 0.1.2
 Summary: A small graphing tool for functions, points, equations and more
 Author-email: Valter Yde Daugberg <valter@hotmail.com>
 Project-URL: Homepage, https://github.com/valteryde/kaxe
 Project-URL: Issues, https://github.com/valteryde/kaxe/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `kaxe-0.1.1/src/kaxe.egg-info/SOURCES.txt` & `kaxe-0.1.2/src/kaxe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kaxe-0.1.1/tests/test.py` & `kaxe-0.1.2/tests/test.py`

 * *Files identical despite different names*

