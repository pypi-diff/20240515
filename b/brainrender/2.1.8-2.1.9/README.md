# Comparing `tmp/brainrender-2.1.8.tar.gz` & `tmp/brainrender-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainrender-2.1.8.tar", last modified: Thu Apr 25 10:58:19 2024, max compression
+gzip compressed data, was "brainrender-2.1.9.tar", last modified: Wed May 15 16:07:55 2024, max compression
```

## Comparing `brainrender-2.1.8.tar` & `brainrender-2.1.9.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:19.361909 brainrender-2.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:19.341909 brainrender-2.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:19.341909 brainrender-2.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-25 10:58:15.000000 brainrender-2.1.8/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-25 10:58:15.000000 brainrender-2.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-25 10:58:15.000000 brainrender-2.1.8/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-25 10:58:15.000000 brainrender-2.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-25 10:58:15.000000 brainrender-2.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-04-25 10:58:19.361909 brainrender-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-25 10:58:15.000000 brainrender-2.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:19.345908 brainrender-2.1.8/brainrender/
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/_colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/_video.py
--rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/actor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:19.349908 brainrender-2.1.8/brainrender/actors/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/actors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/actors/cylinder.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/actors/line.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/actors/neurons.py
--rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/actors/points.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/actors/ruler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/actors/streamlines.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/actors/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/atlas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:19.349908 brainrender-2.1.8/brainrender/atlas_specific/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/atlas_specific/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:19.349908 brainrender-2.1.8/brainrender/atlas_specific/allen_brain_atlas/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:19.349908 brainrender-2.1.8/brainrender/atlas_specific/allen_brain_atlas/gene_expression/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/atlas_specific/allen_brain_atlas/gene_expression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/atlas_specific/allen_brain_atlas/gene_expression/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/atlas_specific/allen_brain_atlas/gene_expression/ge_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/atlas_specific/allen_brain_atlas/streamlines.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/cameras.py
--rw-r--r--   0 runner    (1001) docker     (127)    12962 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/render.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:19.357909 brainrender-2.1.8/brainrender/resources/
--rw-r--r--   0 runner    (1001) docker     (127)  3474788 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/resources/CC_134_1_ch1inj.obj
--rw-r--r--   0 runner    (1001) docker     (127)  3117970 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/resources/CC_134_2_ch1inj.obj
--rw-r--r--   0 runner    (1001) docker     (127)   126927 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/resources/neuron1.swc
--rw-r--r--   0 runner    (1001) docker     (127)    46208 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/resources/probe_1_striatum.npy
--rw-r--r--   0 runner    (1001) docker     (127)    46208 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/resources/probe_2_RSP.npy
--rw-r--r--   0 runner    (1001) docker     (127)    24128 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/resources/random_cells.h5
--rw-r--r--   0 runner    (1001) docker     (127)    24128 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/resources/random_cells.npy
--rw-r--r--   0 runner    (1001) docker     (127)   637432 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/resources/volume.npy
--rw-r--r--   0 runner    (1001) docker     (127)    14186 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/scene.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    13755 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:19.357909 brainrender-2.1.8/brainrender.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-04-25 10:58:19.000000 brainrender-2.1.8/brainrender.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-25 10:58:19.000000 brainrender-2.1.8/brainrender.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 10:58:19.000000 brainrender-2.1.8/brainrender.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-25 10:58:19.000000 brainrender-2.1.8/brainrender.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 10:58:19.000000 brainrender-2.1.8/brainrender.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-25 10:58:15.000000 brainrender-2.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 10:58:19.361909 brainrender-2.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:07:55.879276 brainrender-2.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:07:55.863276 brainrender-2.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:07:55.863276 brainrender-2.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-15 16:07:50.000000 brainrender-2.1.9/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-15 16:07:50.000000 brainrender-2.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-15 16:07:50.000000 brainrender-2.1.9/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-15 16:07:50.000000 brainrender-2.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-15 16:07:50.000000 brainrender-2.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-05-15 16:07:55.879276 brainrender-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-15 16:07:50.000000 brainrender-2.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:07:55.867276 brainrender-2.1.9/brainrender/
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-15 16:07:50.000000 brainrender-2.1.9/brainrender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-15 16:07:50.000000 brainrender-2.1.9/brainrender/_colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-15 16:07:50.000000 brainrender-2.1.9/brainrender/_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-15 16:07:50.000000 brainrender-2.1.9/brainrender/_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-15 16:07:50.000000 brainrender-2.1.9/brainrender/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-15 16:07:50.000000 brainrender-2.1.9/brainrender/_video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-05-15 16:07:50.000000 brainrender-2.1.9/brainrender/actor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:07:55.867276 brainrender-2.1.9/brainrender/actors/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-15 16:07:50.000000 brainrender-2.1.9/brainrender/actors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-15 16:07:50.000000 brainrender-2.1.9/brainrender/actors/cylinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-15 16:07:50.000000 brainrender-2.1.9/brainrender/actors/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-15 16:07:50.000000 brainrender-2.1.9/brainrender/actors/neurons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-05-15 16:07:50.000000 brainrender-2.1.9/brainrender/actors/points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-15 16:07:50.000000 brainrender-2.1.9/brainrender/actors/ruler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-15 16:07:50.000000 brainrender-2.1.9/brainrender/actors/streamlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-15 16:07:50.000000 brainrender-2.1.9/brainrender/actors/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-05-15 16:07:50.000000 brainrender-2.1.9/brainrender/atlas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:07:55.867276 brainrender-2.1.9/brainrender/atlas_specific/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-15 16:07:50.000000 brainrender-2.1.9/brainrender/atlas_specific/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:07:55.867276 brainrender-2.1.9/brainrender/atlas_specific/allen_brain_atlas/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:07:55.867276 brainrender-2.1.9/brainrender/atlas_specific/allen_brain_atlas/gene_expression/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-15 16:07:50.000000 brainrender-2.1.9/brainrender/atlas_specific/allen_brain_atlas/gene_expression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-05-15 16:07:50.000000 brainrender-2.1.9/brainrender/atlas_specific/allen_brain_atlas/gene_expression/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-15 16:07:50.000000 brainrender-2.1.9/brainrender/atlas_specific/allen_brain_atlas/gene_expression/ge_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-15 16:07:50.000000 brainrender-2.1.9/brainrender/atlas_specific/allen_brain_atlas/streamlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-15 16:07:50.000000 brainrender-2.1.9/brainrender/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-15 16:07:50.000000 brainrender-2.1.9/brainrender/cameras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12793 2024-05-15 16:07:50.000000 brainrender-2.1.9/brainrender/render.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:07:55.879276 brainrender-2.1.9/brainrender/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)  3474788 2024-05-15 16:07:50.000000 brainrender-2.1.9/brainrender/resources/CC_134_1_ch1inj.obj
+-rw-r--r--   0 runner    (1001) docker     (127)  3117970 2024-05-15 16:07:50.000000 brainrender-2.1.9/brainrender/resources/CC_134_2_ch1inj.obj
+-rw-r--r--   0 runner    (1001) docker     (127)   126927 2024-05-15 16:07:50.000000 brainrender-2.1.9/brainrender/resources/neuron1.swc
+-rw-r--r--   0 runner    (1001) docker     (127)    46208 2024-05-15 16:07:50.000000 brainrender-2.1.9/brainrender/resources/probe_1_striatum.npy
+-rw-r--r--   0 runner    (1001) docker     (127)    46208 2024-05-15 16:07:50.000000 brainrender-2.1.9/brainrender/resources/probe_2_RSP.npy
+-rw-r--r--   0 runner    (1001) docker     (127)    24128 2024-05-15 16:07:50.000000 brainrender-2.1.9/brainrender/resources/random_cells.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    24128 2024-05-15 16:07:50.000000 brainrender-2.1.9/brainrender/resources/random_cells.npy
+-rw-r--r--   0 runner    (1001) docker     (127)   637432 2024-05-15 16:07:50.000000 brainrender-2.1.9/brainrender/resources/volume.npy
+-rw-r--r--   0 runner    (1001) docker     (127)    14186 2024-05-15 16:07:50.000000 brainrender-2.1.9/brainrender/scene.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-15 16:07:50.000000 brainrender-2.1.9/brainrender/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13755 2024-05-15 16:07:50.000000 brainrender-2.1.9/brainrender/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:07:55.879276 brainrender-2.1.9/brainrender.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-05-15 16:07:55.000000 brainrender-2.1.9/brainrender.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-15 16:07:55.000000 brainrender-2.1.9/brainrender.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 16:07:55.000000 brainrender-2.1.9/brainrender.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-15 16:07:55.000000 brainrender-2.1.9/brainrender.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 16:07:55.000000 brainrender-2.1.9/brainrender.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-15 16:07:50.000000 brainrender-2.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 16:07:55.879276 brainrender-2.1.9/setup.cfg
```

### Comparing `brainrender-2.1.8/.github/workflows/test_and_deploy.yml` & `brainrender-2.1.9/.github/workflows/test_and_deploy.yml`

 * *Files 7% similar despite different names*

```diff
@@ -34,16 +34,18 @@
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         # Run all supported Python versions on linux
         python-version: ["3.9", "3.10", "3.11"]
         os: [ubuntu-latest]
-        # Include one windows and macos run
+        # Include one windows and macos run each of Intel/ARM
         include:
+        - os: macos-13
+          python-version: "3.11"
         - os: macos-latest
           python-version: "3.11"
         - os: windows-latest
           python-version: "3.11"
 
     steps:
       - name: Install hdf5 libs for Mac
@@ -51,16 +53,21 @@
         run: brew install hdf5
 
       # Helps set up VTK with a headless display
       - uses: pyvista/setup-headless-display-action@v2
 
       # Sets up ffmpeg to we can run video tests on CI
       - uses: FedericoCarboni/setup-ffmpeg@v2
+        if: matrix.os != 'macos-latest'
         id: setup-ffmpeg
 
+      - name: setup ffmpeg on latest Mac with brew
+        if: matrix.os == 'macos-latest'
+        run: brew install ffmpeg
+
       # Run tests
       - uses: neuroinformatics-unit/actions/test@v2
         with:
           python-version: ${{ matrix.python-version }}
           secret-codecov-token: ${{ secrets.CODECOV_TOKEN }}
 
   build_sdist_wheels:
```

### Comparing `brainrender-2.1.8/.gitignore` & `brainrender-2.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.8/CITATION.cff` & `brainrender-2.1.9/CITATION.cff`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.8/LICENSE` & `brainrender-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.8/PKG-INFO` & `brainrender-2.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainrender
-Version: 2.1.8
+Version: 2.1.9
 Summary: Visualisation and exploration of brain atlases and other anatomical data
 Author-email: "Federico Claudi, Adam Tyson, Luigi Petrucco" <hello@brainglobe.info>
 License: BSD-3-Clause
 Project-URL: Homepage, https://brainglobe.info/
 Project-URL: Source Code, https://github.com/brainglobe/brainrender
 Project-URL: Bug Tracker, https://github.com/brainglobe/brainrender/issues
 Project-URL: Documentation, https://brainglobe.info/documentation/brainrender/index.html
@@ -20,14 +20,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: brainglobe-atlasapi>=2.0.1
 Requires-Dist: brainglobe-space>=1.0.0
+Requires-Dist: brainglobe-utils>=0.5.0
 Requires-Dist: h5py
 Requires-Dist: imio
 Requires-Dist: k3d
 Requires-Dist: loguru
 Requires-Dist: morphapi>=0.2.1
 Requires-Dist: msgpack
 Requires-Dist: myterial
@@ -136,15 +137,15 @@
 # Display the figure.
 scene.render()
 
 ```
 
 ## Citing brainrender
 
-If you use BrainRender in your scientific work, please cite:
+If you use brainrender in your scientific work, please cite:
 ```
 Claudi, F., Tyson, A. L., Petrucco, L., Margrie, T.W., Portugues, R.,  Branco, T. (2021) "Visualizing anatomically registered data with Brainrender&quot; <i>eLife</i> 2021;10:e65751 [doi.org/10.7554/eLife.65751](https://doi.org/10.7554/eLife.65751)
 ```
 
 BibTeX:
 
 ``` bibtex
```

### Comparing `brainrender-2.1.8/README.md` & `brainrender-2.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 # Display the figure.
 scene.render()
 
 ```
 
 ## Citing brainrender
 
-If you use BrainRender in your scientific work, please cite:
+If you use brainrender in your scientific work, please cite:
 ```
 Claudi, F., Tyson, A. L., Petrucco, L., Margrie, T.W., Portugues, R.,  Branco, T. (2021) "Visualizing anatomically registered data with Brainrender&quot; <i>eLife</i> 2021;10:e65751 [doi.org/10.7554/eLife.65751](https://doi.org/10.7554/eLife.65751)
 ```
 
 BibTeX:
 
 ``` bibtex
```

### Comparing `brainrender-2.1.8/brainrender/__init__.py` & `brainrender-2.1.9/brainrender/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,27 +20,26 @@
 
 try:
     __version__ = version("brainrender")
 except PackageNotFoundError:
     # package is not installed
     pass
 
-base_dir = Path(os.path.join(os.path.expanduser("~"), ".brainrender"))
-base_dir.mkdir(exist_ok=True)
+base_dir = Path.home() / ".brainglobe" / "brainrender"
+base_dir.mkdir(parents=True, exist_ok=True)
 
 
 # set logger level
 def set_logging(level="INFO", path=None):
     """
     Sets loguru to save all logs to a file i
     brainrender's base directory and to print
     to stdout only logs >= to a given level
     """
     logger.remove()
-    # logger.add(sys.stdout, level=level)
 
     path = path or str(base_dir / "log.log")
     if Path(path).exists():
         Path(path).unlink()
     logger.add(path, level="DEBUG")
 
     if level == "DEBUG":
```

### Comparing `brainrender-2.1.8/brainrender/_colors.py` & `brainrender-2.1.9/brainrender/_colors.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.8/brainrender/_io.py` & `brainrender-2.1.9/brainrender/_io.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.8/brainrender/_jupyter.py` & `brainrender-2.1.9/brainrender/_jupyter.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.8/brainrender/_utils.py` & `brainrender-2.1.9/brainrender/_utils.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.8/brainrender/_video.py` & `brainrender-2.1.9/brainrender/_video.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.8/brainrender/actor.py` & `brainrender-2.1.9/brainrender/actor.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.8/brainrender/actors/cylinder.py` & `brainrender-2.1.9/brainrender/actors/cylinder.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.8/brainrender/actors/line.py` & `brainrender-2.1.9/brainrender/actors/line.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.8/brainrender/actors/neurons.py` & `brainrender-2.1.9/brainrender/actors/neurons.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.8/brainrender/actors/points.py` & `brainrender-2.1.9/brainrender/actors/points.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.8/brainrender/actors/ruler.py` & `brainrender-2.1.9/brainrender/actors/ruler.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.8/brainrender/actors/streamlines.py` & `brainrender-2.1.9/brainrender/actors/streamlines.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.8/brainrender/actors/volume.py` & `brainrender-2.1.9/brainrender/actors/volume.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.8/brainrender/atlas.py` & `brainrender-2.1.9/brainrender/atlas.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.8/brainrender/atlas_specific/allen_brain_atlas/gene_expression/api.py` & `brainrender-2.1.9/brainrender/atlas_specific/allen_brain_atlas/gene_expression/api.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.8/brainrender/atlas_specific/allen_brain_atlas/gene_expression/ge_utils.py` & `brainrender-2.1.9/brainrender/atlas_specific/allen_brain_atlas/gene_expression/ge_utils.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.8/brainrender/atlas_specific/allen_brain_atlas/streamlines.py` & `brainrender-2.1.9/brainrender/atlas_specific/allen_brain_atlas/streamlines.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.8/brainrender/camera.py` & `brainrender-2.1.9/brainrender/camera.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.8/brainrender/cameras.py` & `brainrender-2.1.9/brainrender/cameras.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.8/brainrender/render.py` & `brainrender-2.1.9/brainrender/render.py`

 * *Files 3% similar despite different names*

```diff
@@ -188,28 +188,26 @@
                 pass
 
     def render(
         self,
         interactive=None,
         camera=None,
         zoom=None,
-        update_camera=True,
         **kwargs,
     ):
         """
         Renders the scene.
 
         :param interactive: bool. If note settings.INTERACTIVE is used.
             If true the program's execution is stopped and users
             can interact with scene.
         :param camera: str, dict. If none the default camera is used.
             Pass a valid camera input to specify the camera position when
             the scene is rendered.
         :param zoom: float, if None atlas default is used
-        :param update_camera: bool, if False the camera is not changed
         :param kwargs: additional arguments to pass to self.plotter.show
         """
         logger.debug(
             f"Rendering scene. Interactive: {interactive}, camera: {camera}, zoom: {zoom}"
         )
         # get zoom
         zoom = zoom or self.atlas.zoom
@@ -225,15 +223,15 @@
         else:
             camera = check_camera_param(camera)
 
         if "focal_point" not in camera.keys() or camera["focal_point"] is None:
             camera["focal_point"] = self.root._mesh.center_of_mass()
 
         if not self.backend and camera is not None:
-            camera = set_camera(self, camera)
+            _ = set_camera(self, camera)
 
         # Apply axes correction
         for actor in self.clean_actors:
             if not actor._is_transformed:
                 self._prepare_actor(actor)
                 self.plotter.add(actor.mesh)
 
@@ -262,15 +260,14 @@
             if interactive is None:
                 interactive = settings.INTERACTIVE
 
             self.plotter.show(
                 interactive=interactive,
                 zoom=zoom,
                 bg=settings.BACKGROUND_COLOR,
-                camera=camera.copy() if update_camera else None,
                 rate=40,
                 axes=self.plotter.axes,
             )
         elif self.backend == "k3d":  # pragma: no cover
             # Remove silhouettes
             self.remove(*self.get_actors(br_class="silhouette"))
             print(
```

### Comparing `brainrender-2.1.8/brainrender/resources/CC_134_1_ch1inj.obj` & `brainrender-2.1.9/brainrender/resources/CC_134_1_ch1inj.obj`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.8/brainrender/resources/CC_134_2_ch1inj.obj` & `brainrender-2.1.9/brainrender/resources/CC_134_2_ch1inj.obj`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.8/brainrender/resources/neuron1.swc` & `brainrender-2.1.9/brainrender/resources/neuron1.swc`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.8/brainrender/resources/probe_1_striatum.npy` & `brainrender-2.1.9/brainrender/resources/probe_1_striatum.npy`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.8/brainrender/resources/probe_2_RSP.npy` & `brainrender-2.1.9/brainrender/resources/probe_2_RSP.npy`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.8/brainrender/resources/random_cells.h5` & `brainrender-2.1.9/brainrender/resources/random_cells.h5`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.8/brainrender/resources/random_cells.npy` & `brainrender-2.1.9/brainrender/resources/random_cells.npy`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.8/brainrender/resources/volume.npy` & `brainrender-2.1.9/brainrender/resources/volume.npy`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.8/brainrender/scene.py` & `brainrender-2.1.9/brainrender/scene.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.8/brainrender/settings.py` & `brainrender-2.1.9/brainrender/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,11 +28,11 @@
 DEFAULT_ATLAS = "allen_mouse_25um"  # default atlas
 DEFAULT_CAMERA = "three_quarters"  # Default camera settings (orientation etc. see brainrender.camera.py)
 INTERACTIVE = True  # rendering interactive ?
 LW = 2  # e.g. for silhouettes
 ROOT_COLOR = [0.8, 0.8, 0.8]  # color of the overall brain model's actor
 ROOT_ALPHA = 0.2  # transparency of the overall brain model's actor'
 SCREENSHOT_SCALE = 1
-SHADER_STYLE = "cartoon"  # affects the look of rendered brain regions: [metallic, plastic, shiny, glossy]
+SHADER_STYLE = "cartoon"  # affects the look of rendered brain regions: [metallic, plastic, shiny, glossy, cartoon]
 SHOW_AXES = True
 WHOLE_SCREEN = False  # If true render window is full screen
 OFFSCREEN = False
```

### Comparing `brainrender-2.1.8/brainrender/video.py` & `brainrender-2.1.9/brainrender/video.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.8/brainrender.egg-info/PKG-INFO` & `brainrender-2.1.9/brainrender.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainrender
-Version: 2.1.8
+Version: 2.1.9
 Summary: Visualisation and exploration of brain atlases and other anatomical data
 Author-email: "Federico Claudi, Adam Tyson, Luigi Petrucco" <hello@brainglobe.info>
 License: BSD-3-Clause
 Project-URL: Homepage, https://brainglobe.info/
 Project-URL: Source Code, https://github.com/brainglobe/brainrender
 Project-URL: Bug Tracker, https://github.com/brainglobe/brainrender/issues
 Project-URL: Documentation, https://brainglobe.info/documentation/brainrender/index.html
@@ -20,14 +20,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: brainglobe-atlasapi>=2.0.1
 Requires-Dist: brainglobe-space>=1.0.0
+Requires-Dist: brainglobe-utils>=0.5.0
 Requires-Dist: h5py
 Requires-Dist: imio
 Requires-Dist: k3d
 Requires-Dist: loguru
 Requires-Dist: morphapi>=0.2.1
 Requires-Dist: msgpack
 Requires-Dist: myterial
@@ -136,15 +137,15 @@
 # Display the figure.
 scene.render()
 
 ```
 
 ## Citing brainrender
 
-If you use BrainRender in your scientific work, please cite:
+If you use brainrender in your scientific work, please cite:
 ```
 Claudi, F., Tyson, A. L., Petrucco, L., Margrie, T.W., Portugues, R.,  Branco, T. (2021) "Visualizing anatomically registered data with Brainrender&quot; <i>eLife</i> 2021;10:e65751 [doi.org/10.7554/eLife.65751](https://doi.org/10.7554/eLife.65751)
 ```
 
 BibTeX:
 
 ``` bibtex
```

### Comparing `brainrender-2.1.8/brainrender.egg-info/SOURCES.txt` & `brainrender-2.1.9/brainrender.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.8/pyproject.toml` & `brainrender-2.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 readme = "README.md"
 requires-python = ">=3.9.0"
 dynamic = ["version"]
 
 dependencies = [
     "brainglobe-atlasapi>=2.0.1",
     "brainglobe-space>=1.0.0",
+    "brainglobe-utils>=0.5.0",
     "h5py",
     "imio",
     "k3d",
     "loguru",
     "morphapi>=0.2.1",
     "msgpack",
     "myterial",
```

