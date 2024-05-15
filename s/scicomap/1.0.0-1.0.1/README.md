# Comparing `tmp/scicomap-1.0.0.tar.gz` & `tmp/scicomap-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scicomap-1.0.0.tar", last modified: Sat Sep 30 22:20:33 2023, max compression
+gzip compressed data, was "scicomap-1.0.1.tar", last modified: Wed May 15 20:44:26 2024, max compression
```

## Comparing `scicomap-1.0.0.tar` & `scicomap-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 bsatom    (1000) bsatom    (1000)        0 2023-09-30 22:20:33.657031 scicomap-1.0.0/
--rw-rw-r--   0 bsatom    (1000) bsatom    (1000)     1071 2023-09-24 13:37:49.000000 scicomap-1.0.0/LICENSE.md
--rw-r--r--   0 bsatom    (1000) bsatom    (1000)    12652 2023-09-30 22:20:33.657031 scicomap-1.0.0/PKG-INFO
--rw-rw-r--   0 bsatom    (1000) bsatom    (1000)     9829 2023-09-29 14:41:40.000000 scicomap-1.0.0/README.md
--rw-rw-r--   0 bsatom    (1000) bsatom    (1000)     1501 2023-09-29 16:52:00.000000 scicomap-1.0.0/pyproject.toml
--rw-rw-r--   0 bsatom    (1000) bsatom    (1000)       38 2023-09-30 22:20:33.657031 scicomap-1.0.0/setup.cfg
-drwxrwxr-x   0 bsatom    (1000) bsatom    (1000)        0 2023-09-30 22:20:33.629030 scicomap-1.0.0/src/
-drwxrwxr-x   0 bsatom    (1000) bsatom    (1000)        0 2023-09-30 22:20:33.637030 scicomap-1.0.0/src/scicomap/
--rw-rw-r--   0 bsatom    (1000) bsatom    (1000)      338 2023-09-29 16:51:57.000000 scicomap-1.0.0/src/scicomap/__init__.py
--rw-rw-r--   0 bsatom    (1000) bsatom    (1000)    12622 2023-09-29 14:41:41.000000 scicomap-1.0.0/src/scicomap/cblind.py
--rw-rw-r--   0 bsatom    (1000) bsatom    (1000)    33833 2023-09-29 14:41:41.000000 scicomap-1.0.0/src/scicomap/cmath.py
-drwxrwxr-x   0 bsatom    (1000) bsatom    (1000)        0 2023-09-30 22:20:33.645031 scicomap-1.0.0/src/scicomap/data/
--rw-rw-r--   0 bsatom    (1000) bsatom    (1000)    83066 2023-09-29 14:41:41.000000 scicomap-1.0.0/src/scicomap/data/grmhd.png
--rw-rw-r--   0 bsatom    (1000) bsatom    (1000)   174061 2023-09-29 14:41:41.000000 scicomap-1.0.0/src/scicomap/data/jacksboro_fault_dem.npz
--rw-rw-r--   0 bsatom    (1000) bsatom    (1000)    33229 2023-09-29 14:41:41.000000 scicomap-1.0.0/src/scicomap/data/s1045.ima.gz
--rw-rw-r--   0 bsatom    (1000) bsatom    (1000)   803731 2023-09-29 14:41:41.000000 scicomap-1.0.0/src/scicomap/data/tng.jpg
--rw-rw-r--   0 bsatom    (1000) bsatom    (1000)  1019152 2023-09-29 14:41:41.000000 scicomap-1.0.0/src/scicomap/data/vortex.jpg
--rw-rw-r--   0 bsatom    (1000) bsatom    (1000)     3969 2023-09-29 14:41:41.000000 scicomap-1.0.0/src/scicomap/datasets.py
--rw-rw-r--   0 bsatom    (1000) bsatom    (1000)    51818 2023-09-29 14:41:41.000000 scicomap-1.0.0/src/scicomap/scicomap.py
--rw-rw-r--   0 bsatom    (1000) bsatom    (1000)    10054 2023-09-29 14:41:41.000000 scicomap-1.0.0/src/scicomap/utils.py
-drwxrwxr-x   0 bsatom    (1000) bsatom    (1000)        0 2023-09-30 22:20:33.637030 scicomap-1.0.0/src/scicomap.egg-info/
--rw-r--r--   0 bsatom    (1000) bsatom    (1000)    12652 2023-09-30 22:20:33.000000 scicomap-1.0.0/src/scicomap.egg-info/PKG-INFO
--rw-rw-r--   0 bsatom    (1000) bsatom    (1000)      512 2023-09-30 22:20:33.000000 scicomap-1.0.0/src/scicomap.egg-info/SOURCES.txt
--rw-rw-r--   0 bsatom    (1000) bsatom    (1000)        1 2023-09-30 22:20:33.000000 scicomap-1.0.0/src/scicomap.egg-info/dependency_links.txt
--rw-rw-r--   0 bsatom    (1000) bsatom    (1000)      299 2023-09-30 22:20:33.000000 scicomap-1.0.0/src/scicomap.egg-info/requires.txt
--rw-rw-r--   0 bsatom    (1000) bsatom    (1000)        9 2023-09-30 22:20:33.000000 scicomap-1.0.0/src/scicomap.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 20:44:26.567395 scicomap-1.0.1/
+-rw-rw-rw-   0        0        0     1091 2024-05-15 20:33:41.000000 scicomap-1.0.1/LICENSE.md
+-rw-rw-rw-   0        0        0    13019 2024-05-15 20:44:26.554393 scicomap-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10132 2024-05-15 20:33:41.000000 scicomap-1.0.1/README.md
+-rw-rw-rw-   0        0        0     1565 2024-05-15 20:40:33.000000 scicomap-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-15 20:44:26.567395 scicomap-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-15 20:44:26.217103 scicomap-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-15 20:44:26.360382 scicomap-1.0.1/src/scicomap/
+-rw-rw-rw-   0        0        0      355 2024-05-15 20:39:25.000000 scicomap-1.0.1/src/scicomap/__init__.py
+-rw-rw-rw-   0        0        0    12959 2024-05-15 20:33:42.000000 scicomap-1.0.1/src/scicomap/cblind.py
+-rw-rw-rw-   0        0        0    34907 2024-05-15 20:33:42.000000 scicomap-1.0.1/src/scicomap/cmath.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:44:26.524397 scicomap-1.0.1/src/scicomap/data/
+-rw-rw-rw-   0        0        0    83066 2024-05-15 20:33:42.000000 scicomap-1.0.1/src/scicomap/data/grmhd.png
+-rw-rw-rw-   0        0        0   174061 2024-05-15 20:33:42.000000 scicomap-1.0.1/src/scicomap/data/jacksboro_fault_dem.npz
+-rw-rw-rw-   0        0        0    33229 2024-05-15 20:33:42.000000 scicomap-1.0.1/src/scicomap/data/s1045.ima.gz
+-rw-rw-rw-   0        0        0   803731 2024-05-15 20:33:42.000000 scicomap-1.0.1/src/scicomap/data/tng.jpg
+-rw-rw-rw-   0        0        0  1019152 2024-05-15 20:33:42.000000 scicomap-1.0.1/src/scicomap/data/vortex.jpg
+-rw-rw-rw-   0        0        0     4098 2024-05-15 20:33:42.000000 scicomap-1.0.1/src/scicomap/datasets.py
+-rw-rw-rw-   0        0        0    53316 2024-05-15 20:33:42.000000 scicomap-1.0.1/src/scicomap/scicomap.py
+-rw-rw-rw-   0        0        0    10346 2024-05-15 20:33:42.000000 scicomap-1.0.1/src/scicomap/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:44:26.539394 scicomap-1.0.1/src/scicomap.egg-info/
+-rw-rw-rw-   0        0        0    13019 2024-05-15 20:44:26.000000 scicomap-1.0.1/src/scicomap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2024-05-15 20:44:26.000000 scicomap-1.0.1/src/scicomap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 20:44:26.000000 scicomap-1.0.1/src/scicomap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      299 2024-05-15 20:44:26.000000 scicomap-1.0.1/src/scicomap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-15 20:44:26.000000 scicomap-1.0.1/src/scicomap.egg-info/top_level.txt
```

### Comparing `scicomap-1.0.0/LICENSE.md` & `scicomap-1.0.1/LICENSE.md`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) [2021] [Thomas Bury]
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) [2021] [Thomas Bury]
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `scicomap-1.0.0/PKG-INFO` & `scicomap-1.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,294 +1,296 @@
-Metadata-Version: 2.1
-Name: scicomap
-Version: 1.0.0
-Summary: data visualization on maps with varying levels of granularity
-Author-email: Thomas Bury <bury.thomas@gmail.com>
-License: MIT License
-        
-        Copyright (c) [2021] [Thomas Bury]
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-Project-URL: homepage, https://github.com/ThomasBury/scicomap
-Project-URL: documentation, https://github.com/ThomasBury/scicomap
-Project-URL: repository, https://github.com/ThomasBury/scicomap.git
-Project-URL: changelog, https://github.com/ThomasBury/scicomap
-Project-URL: Tracker, https://github.com/ThomasBury/scicomap/issues
-Keywords: visualization,color,uniform,scientific
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: scipy
-Requires-Dist: colorspacious
-Requires-Dist: colorcet
-Requires-Dist: cmcrameri
-Requires-Dist: cmocean
-Requires-Dist: cmasher>=1.5.8
-Requires-Dist: palettable>=3.3.0
-Requires-Dist: matplotlib>=3.3.0
-Provides-Extra: doc
-Requires-Dist: ipykernel; extra == "doc"
-Requires-Dist: ipython_genutils; extra == "doc"
-Requires-Dist: pandoc; extra == "doc"
-Requires-Dist: sphinx; extra == "doc"
-Requires-Dist: sphinxawesome-theme==5.0.0b5; extra == "doc"
-Requires-Dist: nbsphinx; extra == "doc"
-Requires-Dist: sphinx-autodoc-typehints; extra == "doc"
-Requires-Dist: sphinx-copybutton; extra == "doc"
-Requires-Dist: sphinx-tabs; extra == "doc"
-Provides-Extra: lint
-Requires-Dist: black; extra == "lint"
-Requires-Dist: flake8; extra == "lint"
-Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: pytest-cov; extra == "test"
-
-<img src="pics/logo.png" alt="drawing" width="200"/>
-
-[buy me caffeine](https://ko-fi.com/V7V72SOHX)
-
-
-
-# Scientific color maps 
-
-## Blog post
-
-[Scicomap Medium blog post (free)](https://towardsdatascience.com/your-colour-map-is-bad-heres-how-to-fix-it-lessons-learnt-from-the-event-horizon-telescope-b82523f09469)
-
-[Tutorial notebook](./docs/notebooks/tutorial.ipynb)
-
-## Installation
-
-```shell
-pip install scicomap
-```
-
-## Introduction 
-
-Scicomap is a package that provides scientific color maps and tools to standardize your favourite color maps if you don't like the built-in ones.
-Scicomap currently provides sequential, bi-sequential, diverging, circular, qualitative and miscellaneous color maps. You can easily draw examples, compare the rendering, see how colorblind people will perceive the color maps. I will illustrate the scicomap capabilities below.
-
-This package is heavily based on the [Event Horyzon Plot package](https://github.com/liamedeiros/ehtplot/tree/docs) and uses good color maps found in the [the python portage of the Fabio Crameri](https://github.com/callumrollo/cmcrameri), [cmasher](https://cmasher.readthedocs.io/), [palettable](https://jiffyclub.github.io/palettable/), [colorcet](https://colorcet.holoviz.org/) and [cmocean](https://matplotlib.org/cmocean/)
-
-## Motivation
-
-The accurate representation of data is essential. Many common color maps distort data through uneven colour gradients and are often unreadable to those with color-vision deficiency. An infamous example is the jet color map. These color maps do not render all the information you want to illustrate or even worse render false information through artefacts. Scientist or not, your goal is to communicate visual information in the most accurate and appealing fashion. Moreover, do not overlook colour-vision deficiency, which represents 8% of the (Caucasian) male population.
-
-## Color spaces
-
-Perceptual uniformity is the idea that Euclidean distance between colors in color space should match human color perception distance judgements. For example, a blue and red that are at a distance d apart should look as discriminable as green and purple that are at a distance d apart.
-Scicomap uses the CAM02-UCS color space (Uniform Colour Space). Its three coordinates are usually denoted by J', a', and b'. And its cylindrical coordinates are J', C', and h'. The perceptual color space Jab is similar to Lab. However, Jab uses an updated color appearance model that in theory provides greater precision for discriminability measurements.
-
- * Lightness: also known as value or tone, is a representation of a color's brightness
- * Chroma: the intrinsic difference between a color and gray of an object
- * Hue: the degree to which a stimulus can be described as similar to or different from stimuli that are described as red, green, blue, and yellow
-
-## Encoding information
-
- * Lightness J': for a scalar value, intensity. It must vary linearly with the physical quantity
- * hue h' can encode an additional physical quantity, the change of hue should be linearly proportional to the quantity. The hue h' is also ideal in making an image more attractive without interfering with the representation of pixel values.
- * chroma is less recognizable and should not be used to encode physical information
-  
-## Color map uniformization
-
-Following the references and the theories, the uniformization is performed by
-
- * Making the color map linear in J'
- * Lifting the color map (making it lighter, i.e. increasing the minimal value of J')
- * Symmetrizing the chroma to avoid further artefacts
- * Avoid kinks and edges in the chroma curve
- * Bitonic symmetrization or not
-
-
-# Scicomap
-
-## Choosing the right type of color maps
-Scicomap provides a bunch of color maps for different applications. The different types of color map are 
-
-```python
-import scicomap as sc
-sc_map = sc.SciCoMap()
-sc_map.get_ctype()
-```
-
-```
-dict_keys(['diverging', 'sequential', 'multi-sequential', 'circular', 'miscellaneous', 'qualitative'])
-```
-
-I'll refer to the [The misuse of colour in science communication](https://www.nature.com/articles/s41467-020-19160-7.pdf) for choosing the right scientific color map
-
-<td align="left"><img src="pics/choosing-cmap.png" width="500"/></td>
-
-## Get the matplotlib cmap
-
-
-```python
-plt_cmap_obj = sc_map.get_mpl_color_map()
-```
-
-## Choosing the color map for a given type
-
-Get the color maps for a given type
-
-```python
-sc_map = sc.ScicoSequential()
-sc_map.get_color_map_names()
-```
-
-```
-dict_keys(['afmhot', 'amber', 'amber_r', 'amp', 'apple', 'apple_r', 'autumn', 'batlow', 'bilbao', 'bilbao_r', 'binary', 'Blues', 'bone', 'BuGn', 'BuPu', 'chroma', 'chroma_r', 'cividis', 'cool', 'copper', 'cosmic', 'cosmic_r', 'deep', 'dense', 'dusk', 'dusk_r', 'eclipse', 'eclipse_r', 'ember', 'ember_r', 'fall', 'fall_r', 'gem', 'gem_r', 'gist_gray', 'gist_heat', 'gist_yarg', 'GnBu', 'Greens', 'gray', 'Greys', 'haline', 'hawaii', 'hawaii_r', 'heat', 'heat_r', 'hot', 'ice', 'inferno', 'imola', 'imola_r', 'lapaz', 'lapaz_r', 'magma', 'matter', 'neon', 'neon_r', 'neutral', 'neutral_r', 'nuuk', 'nuuk_r', 'ocean', 'ocean_r', 'OrRd', 'Oranges', 'pink', 'plasma', 'PuBu', 'PuBuGn', 'PuRd', 'Purples', 'rain', 'rainbow', 'rainbow-sc', 'rainbow-sc_r', 'rainforest', 'rainforest_r', 'RdPu', 'Reds', 'savanna', 'savanna_r', 'sepia', 'sepia_r', 'speed', 'solar', 'spring', 'summer', 'tempo', 'thermal', 'thermal_r', 'thermal-2', 'tokyo', 'tokyo_r', 'tropical', 'tropical_r', 'turbid', 'turku', 'turku_r', 'viridis', 'winter', 'Wistia', 'YlGn', 'YlGnBu', 'YlOrBr', 'YlOrRd'])
-```
-
-## Assessing a color map
-
-In order to assess if a color map should be corrected or not, `scicomap` provides a way to quickly check if the lightness is linear, how asymmetric and smooth is the chroma and how the color map renders for color-deficient users. I will illustrate some of the artefacts using classical images, as the pyramid and specific functions for each kind of color map.
-
-
-### An infamous example
-
-```python
-import scicomap as sc
-import matplotlib.pyplot as plt
-
-# the thing that should not be
-ugly_jet = plt.get_cmap("jet")
-sc_map =  sc.ScicoMiscellaneous(cmap=ugly_jet)
-f=sc_map.assess_cmap(figsize=(22,10))
-```
-
-
-<td align="left"><img src="pics/jet.png" width="1000"/></td>
- 
-
-Clearly, the lightness is not linear, has edges and kinks. The chroma is not smooth and asymmetrical. See the below illustration to see how bad and how many artefacts the jet color map introduces
-
-
-<td align="left"><img src="pics/jet2.png" width="1000"/></td>
-
-
-## Correcting a color map - Example
-
-### Sequential color map
-
-Let's assess the built-in color map `hawaii` without correction:
-
-```python
-sc_map = sc.ScicoSequential(cmap='hawaii')
-f=sc_map.assess_cmap(figsize=(22,10))
-```
-
-<td align="left"><img src="pics/hawaii.png" width="1000"/></td>
-
-
-The color map seems ok, however, the lightness is not linear and the chroma is asymmetrical even if smooth. Those small defects introduce artefact in the information rendering, as we can visualize using the following example
-
-
-```python
-f=sc_map.draw_example()
-```
-
-<td align="left"><img src="pics/hawaii-examples.png" width="1000"/></td>
-
-
-We can clearly see the artefacts, especially for the pyramid for which our eyes should only pick out the corners in the pyramid (ideal situation). Those artefacts are even more striking for color-deficient users (this might not always be the case). Hopefully, `scicomap` provides an easy way to correct those defects:
-
-```python
-# fixing the color map, using the same minimal lightness (lift=None), 
-# not normalizing to bitone and 
-# smoothing the chroma
-sc_map.unif_sym_cmap(lift=None, 
-                     bitonic=False, 
-                     diffuse=True)
-
-# re-assess the color map after fixing it                     
-f=sc_map.assess_cmap(figsize=(22,10))
-```
-
-<td align="left"><img src="pics/hawaii-fixed.png" width="1000"/></td>
-
-
-After fixing the color map, the artefacts are less present
-
-<td align="left"><img src="pics/hawaii-fixed-examples.png" width="1000"/></td>
-
-# All the built-in color maps
-
-## Sequential
-
-<td align="left"><img src="pics/seq-cmaps-all.png" width="500"/></td>
-
-## Diverging
-
-
-<td align="left"><img src="pics/div-cmaps-all.png" width="500"/></td>
-
-## Mutli-sequential
-
-<td align="left"><img src="pics/multi-cmaps-all.png" width="500"/></td>
-
-## Miscellaneous
-
-<td align="left"><img src="pics/misc-cmaps-all.png" width="500"/></td>
-
-## Circular
-
-<td align="left"><img src="pics/circular-cmaps-all.png" width="500"/></td>
-
-## Qualitative
-
-<td align="left"><img src="pics/qual-cmaps-all.png" width="500"/></td>
-
-# References
-
- * [The misuse of colour in science communication](https://www.nature.com/articles/s41467-020-19160-7.pdf)
- * [Why We Use Bad Color Maps and What You Can Do About It](https://www.kennethmoreland.com/color-advice/BadColorMaps.pdf)
- * [THE RAINBOW IS DEAD…LONG LIVE THE RAINBOW! – SERIES OUTLINE](https://mycarta.wordpress.com/2012/05/29/the-rainbow-is-dead-long-live-the-rainbow-series-outline/)
- * [Scientific colour maps](https://www.fabiocrameri.ch/colourmaps/)
- * [Picking a colour scale for scientific graphics](https://betterfigures.org/2015/06/23/picking-a-colour-scale-for-scientific-graphics/)
- * [ColorCET](https://colorcet.com/)
- * [Good Colour Maps: How to Design Them](https://arxiv.org/abs/1509.03700)
- * [Perceptually uniform color space for image signals including high dynamic range and wide gamut](https://www.osapublishing.org/oe/fulltext.cfm?uri=oe-25-13-15131&id=368272)
-
-
-# Changes log
-
-### 1.0.0
-
- - Docstring
- - Tutorial notebook
- - Web documentation
-
-### 0.4
-
- - Including files in source distributions
-
-### 0.3
-
- - Add a section "how to use with matplotlib"
- - [Bug] Center diverging color map in examples
-
-### 0.2
-
- - [Bug] Fix typo in chart titles
-
-### 0.1
-
- - First version
+Metadata-Version: 2.1
+Name: scicomap
+Version: 1.0.1
+Summary: data visualization on maps with varying levels of granularity
+Author-email: Thomas Bury <bury.thomas@gmail.com>
+License: MIT License
+        
+        Copyright (c) [2021] [Thomas Bury]
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+Project-URL: homepage, https://github.com/ThomasBury/scicomap
+Project-URL: documentation, https://github.com/ThomasBury/scicomap
+Project-URL: repository, https://github.com/ThomasBury/scicomap.git
+Project-URL: changelog, https://github.com/ThomasBury/scicomap
+Project-URL: Tracker, https://github.com/ThomasBury/scicomap/issues
+Keywords: visualization,color,uniform,scientific
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: scipy
+Requires-Dist: colorspacious
+Requires-Dist: colorcet
+Requires-Dist: cmcrameri
+Requires-Dist: cmocean
+Requires-Dist: cmasher>=1.5.8
+Requires-Dist: palettable>=3.3.0
+Requires-Dist: matplotlib>=3.3.0
+Provides-Extra: doc
+Requires-Dist: ipykernel; extra == "doc"
+Requires-Dist: ipython_genutils; extra == "doc"
+Requires-Dist: pandoc; extra == "doc"
+Requires-Dist: sphinx; extra == "doc"
+Requires-Dist: sphinxawesome-theme==5.0.0b5; extra == "doc"
+Requires-Dist: nbsphinx; extra == "doc"
+Requires-Dist: sphinx-autodoc-typehints; extra == "doc"
+Requires-Dist: sphinx-copybutton; extra == "doc"
+Requires-Dist: sphinx-tabs; extra == "doc"
+Provides-Extra: lint
+Requires-Dist: black; extra == "lint"
+Requires-Dist: flake8; extra == "lint"
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+
+<img src="pics/logo.png" alt="drawing" width="200"/>
+
+[buy me caffeine](https://ko-fi.com/V7V72SOHX)
+
+
+
+# Scientific color maps 
+
+## Blog post
+
+[Scicomap Medium blog post (free)](https://towardsdatascience.com/your-colour-map-is-bad-heres-how-to-fix-it-lessons-learnt-from-the-event-horizon-telescope-b82523f09469)
+
+[Official Documentation](https://scicomap.readthedocs.io/en/latest/)
+
+[Tutorial notebook](./docs/notebooks/tutorial.ipynb)
+
+## Installation
+
+```shell
+pip install scicomap
+```
+
+## Introduction 
+
+Scicomap is a package that provides scientific color maps and tools to standardize your favourite color maps if you don't like the built-in ones.
+Scicomap currently provides sequential, bi-sequential, diverging, circular, qualitative and miscellaneous color maps. You can easily draw examples, compare the rendering, see how colorblind people will perceive the color maps. I will illustrate the scicomap capabilities below.
+
+This package is heavily based on the [Event Horyzon Plot package](https://github.com/liamedeiros/ehtplot/tree/docs) and uses good color maps found in the [the python portage of the Fabio Crameri](https://github.com/callumrollo/cmcrameri), [cmasher](https://cmasher.readthedocs.io/), [palettable](https://jiffyclub.github.io/palettable/), [colorcet](https://colorcet.holoviz.org/) and [cmocean](https://matplotlib.org/cmocean/)
+
+## Motivation
+
+The accurate representation of data is essential. Many common color maps distort data through uneven colour gradients and are often unreadable to those with color-vision deficiency. An infamous example is the jet color map. These color maps do not render all the information you want to illustrate or even worse render false information through artefacts. Scientist or not, your goal is to communicate visual information in the most accurate and appealing fashion. Moreover, do not overlook colour-vision deficiency, which represents 8% of the (Caucasian) male population.
+
+## Color spaces
+
+Perceptual uniformity is the idea that Euclidean distance between colors in color space should match human color perception distance judgements. For example, a blue and red that are at a distance d apart should look as discriminable as green and purple that are at a distance d apart.
+Scicomap uses the CAM02-UCS color space (Uniform Colour Space). Its three coordinates are usually denoted by J', a', and b'. And its cylindrical coordinates are J', C', and h'. The perceptual color space Jab is similar to Lab. However, Jab uses an updated color appearance model that in theory provides greater precision for discriminability measurements.
+
+ * Lightness: also known as value or tone, is a representation of a color's brightness
+ * Chroma: the intrinsic difference between a color and gray of an object
+ * Hue: the degree to which a stimulus can be described as similar to or different from stimuli that are described as red, green, blue, and yellow
+
+## Encoding information
+
+ * Lightness J': for a scalar value, intensity. It must vary linearly with the physical quantity
+ * hue h' can encode an additional physical quantity, the change of hue should be linearly proportional to the quantity. The hue h' is also ideal in making an image more attractive without interfering with the representation of pixel values.
+ * chroma is less recognizable and should not be used to encode physical information
+  
+## Color map uniformization
+
+Following the references and the theories, the uniformization is performed by
+
+ * Making the color map linear in J'
+ * Lifting the color map (making it lighter, i.e. increasing the minimal value of J')
+ * Symmetrizing the chroma to avoid further artefacts
+ * Avoid kinks and edges in the chroma curve
+ * Bitonic symmetrization or not
+
+
+# Scicomap
+
+## Choosing the right type of color maps
+Scicomap provides a bunch of color maps for different applications. The different types of color map are 
+
+```python
+import scicomap as sc
+sc_map = sc.SciCoMap()
+sc_map.get_ctype()
+```
+
+```
+dict_keys(['diverging', 'sequential', 'multi-sequential', 'circular', 'miscellaneous', 'qualitative'])
+```
+
+I'll refer to the [The misuse of colour in science communication](https://www.nature.com/articles/s41467-020-19160-7.pdf) for choosing the right scientific color map
+
+<td align="left"><img src="pics/choosing-cmap.png" width="500"/></td>
+
+## Get the matplotlib cmap
+
+
+```python
+plt_cmap_obj = sc_map.get_mpl_color_map()
+```
+
+## Choosing the color map for a given type
+
+Get the color maps for a given type
+
+```python
+sc_map = sc.ScicoSequential()
+sc_map.get_color_map_names()
+```
+
+```
+dict_keys(['afmhot', 'amber', 'amber_r', 'amp', 'apple', 'apple_r', 'autumn', 'batlow', 'bilbao', 'bilbao_r', 'binary', 'Blues', 'bone', 'BuGn', 'BuPu', 'chroma', 'chroma_r', 'cividis', 'cool', 'copper', 'cosmic', 'cosmic_r', 'deep', 'dense', 'dusk', 'dusk_r', 'eclipse', 'eclipse_r', 'ember', 'ember_r', 'fall', 'fall_r', 'gem', 'gem_r', 'gist_gray', 'gist_heat', 'gist_yarg', 'GnBu', 'Greens', 'gray', 'Greys', 'haline', 'hawaii', 'hawaii_r', 'heat', 'heat_r', 'hot', 'ice', 'inferno', 'imola', 'imola_r', 'lapaz', 'lapaz_r', 'magma', 'matter', 'neon', 'neon_r', 'neutral', 'neutral_r', 'nuuk', 'nuuk_r', 'ocean', 'ocean_r', 'OrRd', 'Oranges', 'pink', 'plasma', 'PuBu', 'PuBuGn', 'PuRd', 'Purples', 'rain', 'rainbow', 'rainbow-sc', 'rainbow-sc_r', 'rainforest', 'rainforest_r', 'RdPu', 'Reds', 'savanna', 'savanna_r', 'sepia', 'sepia_r', 'speed', 'solar', 'spring', 'summer', 'tempo', 'thermal', 'thermal_r', 'thermal-2', 'tokyo', 'tokyo_r', 'tropical', 'tropical_r', 'turbid', 'turku', 'turku_r', 'viridis', 'winter', 'Wistia', 'YlGn', 'YlGnBu', 'YlOrBr', 'YlOrRd'])
+```
+
+## Assessing a color map
+
+In order to assess if a color map should be corrected or not, `scicomap` provides a way to quickly check if the lightness is linear, how asymmetric and smooth is the chroma and how the color map renders for color-deficient users. I will illustrate some of the artefacts using classical images, as the pyramid and specific functions for each kind of color map.
+
+
+### An infamous example
+
+```python
+import scicomap as sc
+import matplotlib.pyplot as plt
+
+# the thing that should not be
+ugly_jet = plt.get_cmap("jet")
+sc_map =  sc.ScicoMiscellaneous(cmap=ugly_jet)
+f=sc_map.assess_cmap(figsize=(22,10))
+```
+
+
+<td align="left"><img src="pics/jet.png" width="1000"/></td>
+ 
+
+Clearly, the lightness is not linear, has edges and kinks. The chroma is not smooth and asymmetrical. See the below illustration to see how bad and how many artefacts the jet color map introduces
+
+
+<td align="left"><img src="pics/jet2.png" width="1000"/></td>
+
+
+## Correcting a color map - Example
+
+### Sequential color map
+
+Let's assess the built-in color map `hawaii` without correction:
+
+```python
+sc_map = sc.ScicoSequential(cmap='hawaii')
+f=sc_map.assess_cmap(figsize=(22,10))
+```
+
+<td align="left"><img src="pics/hawaii.png" width="1000"/></td>
+
+
+The color map seems ok, however, the lightness is not linear and the chroma is asymmetrical even if smooth. Those small defects introduce artefact in the information rendering, as we can visualize using the following example
+
+
+```python
+f=sc_map.draw_example()
+```
+
+<td align="left"><img src="pics/hawaii-examples.png" width="1000"/></td>
+
+
+We can clearly see the artefacts, especially for the pyramid for which our eyes should only pick out the corners in the pyramid (ideal situation). Those artefacts are even more striking for color-deficient users (this might not always be the case). Hopefully, `scicomap` provides an easy way to correct those defects:
+
+```python
+# fixing the color map, using the same minimal lightness (lift=None), 
+# not normalizing to bitone and 
+# smoothing the chroma
+sc_map.unif_sym_cmap(lift=None, 
+                     bitonic=False, 
+                     diffuse=True)
+
+# re-assess the color map after fixing it                     
+f=sc_map.assess_cmap(figsize=(22,10))
+```
+
+<td align="left"><img src="pics/hawaii-fixed.png" width="1000"/></td>
+
+
+After fixing the color map, the artefacts are less present
+
+<td align="left"><img src="pics/hawaii-fixed-examples.png" width="1000"/></td>
+
+# All the built-in color maps
+
+## Sequential
+
+<td align="left"><img src="pics/seq-cmaps-all.png" width="500"/></td>
+
+## Diverging
+
+
+<td align="left"><img src="pics/div-cmaps-all.png" width="500"/></td>
+
+## Mutli-sequential
+
+<td align="left"><img src="pics/multi-cmaps-all.png" width="500"/></td>
+
+## Miscellaneous
+
+<td align="left"><img src="pics/misc-cmaps-all.png" width="500"/></td>
+
+## Circular
+
+<td align="left"><img src="pics/circular-cmaps-all.png" width="500"/></td>
+
+## Qualitative
+
+<td align="left"><img src="pics/qual-cmaps-all.png" width="500"/></td>
+
+# References
+
+ * [The misuse of colour in science communication](https://www.nature.com/articles/s41467-020-19160-7.pdf)
+ * [Why We Use Bad Color Maps and What You Can Do About It](https://www.kennethmoreland.com/color-advice/BadColorMaps.pdf)
+ * [THE RAINBOW IS DEAD…LONG LIVE THE RAINBOW! – SERIES OUTLINE](https://mycarta.wordpress.com/2012/05/29/the-rainbow-is-dead-long-live-the-rainbow-series-outline/)
+ * [Scientific colour maps](https://www.fabiocrameri.ch/colourmaps/)
+ * [Picking a colour scale for scientific graphics](https://betterfigures.org/2015/06/23/picking-a-colour-scale-for-scientific-graphics/)
+ * [ColorCET](https://colorcet.com/)
+ * [Good Colour Maps: How to Design Them](https://arxiv.org/abs/1509.03700)
+ * [Perceptually uniform color space for image signals including high dynamic range and wide gamut](https://www.osapublishing.org/oe/fulltext.cfm?uri=oe-25-13-15131&id=368272)
+
+
+# Changes log
+
+### 1.0.0
+
+ - Docstring
+ - Tutorial notebook
+ - Web documentation
+
+### 0.4
+
+ - Including files in source distributions
+
+### 0.3
+
+ - Add a section "how to use with matplotlib"
+ - [Bug] Center diverging color map in examples
+
+### 0.2
+
+ - [Bug] Fix typo in chart titles
+
+### 0.1
+
+ - First version
```

### Comparing `scicomap-1.0.0/README.md` & `scicomap-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,231 +1,233 @@
-<img src="pics/logo.png" alt="drawing" width="200"/>
-
-[buy me caffeine](https://ko-fi.com/V7V72SOHX)
-
-
-
-# Scientific color maps 
-
-## Blog post
-
-[Scicomap Medium blog post (free)](https://towardsdatascience.com/your-colour-map-is-bad-heres-how-to-fix-it-lessons-learnt-from-the-event-horizon-telescope-b82523f09469)
-
-[Tutorial notebook](./docs/notebooks/tutorial.ipynb)
-
-## Installation
-
-```shell
-pip install scicomap
-```
-
-## Introduction 
-
-Scicomap is a package that provides scientific color maps and tools to standardize your favourite color maps if you don't like the built-in ones.
-Scicomap currently provides sequential, bi-sequential, diverging, circular, qualitative and miscellaneous color maps. You can easily draw examples, compare the rendering, see how colorblind people will perceive the color maps. I will illustrate the scicomap capabilities below.
-
-This package is heavily based on the [Event Horyzon Plot package](https://github.com/liamedeiros/ehtplot/tree/docs) and uses good color maps found in the [the python portage of the Fabio Crameri](https://github.com/callumrollo/cmcrameri), [cmasher](https://cmasher.readthedocs.io/), [palettable](https://jiffyclub.github.io/palettable/), [colorcet](https://colorcet.holoviz.org/) and [cmocean](https://matplotlib.org/cmocean/)
-
-## Motivation
-
-The accurate representation of data is essential. Many common color maps distort data through uneven colour gradients and are often unreadable to those with color-vision deficiency. An infamous example is the jet color map. These color maps do not render all the information you want to illustrate or even worse render false information through artefacts. Scientist or not, your goal is to communicate visual information in the most accurate and appealing fashion. Moreover, do not overlook colour-vision deficiency, which represents 8% of the (Caucasian) male population.
-
-## Color spaces
-
-Perceptual uniformity is the idea that Euclidean distance between colors in color space should match human color perception distance judgements. For example, a blue and red that are at a distance d apart should look as discriminable as green and purple that are at a distance d apart.
-Scicomap uses the CAM02-UCS color space (Uniform Colour Space). Its three coordinates are usually denoted by J', a', and b'. And its cylindrical coordinates are J', C', and h'. The perceptual color space Jab is similar to Lab. However, Jab uses an updated color appearance model that in theory provides greater precision for discriminability measurements.
-
- * Lightness: also known as value or tone, is a representation of a color's brightness
- * Chroma: the intrinsic difference between a color and gray of an object
- * Hue: the degree to which a stimulus can be described as similar to or different from stimuli that are described as red, green, blue, and yellow
-
-## Encoding information
-
- * Lightness J': for a scalar value, intensity. It must vary linearly with the physical quantity
- * hue h' can encode an additional physical quantity, the change of hue should be linearly proportional to the quantity. The hue h' is also ideal in making an image more attractive without interfering with the representation of pixel values.
- * chroma is less recognizable and should not be used to encode physical information
-  
-## Color map uniformization
-
-Following the references and the theories, the uniformization is performed by
-
- * Making the color map linear in J'
- * Lifting the color map (making it lighter, i.e. increasing the minimal value of J')
- * Symmetrizing the chroma to avoid further artefacts
- * Avoid kinks and edges in the chroma curve
- * Bitonic symmetrization or not
-
-
-# Scicomap
-
-## Choosing the right type of color maps
-Scicomap provides a bunch of color maps for different applications. The different types of color map are 
-
-```python
-import scicomap as sc
-sc_map = sc.SciCoMap()
-sc_map.get_ctype()
-```
-
-```
-dict_keys(['diverging', 'sequential', 'multi-sequential', 'circular', 'miscellaneous', 'qualitative'])
-```
-
-I'll refer to the [The misuse of colour in science communication](https://www.nature.com/articles/s41467-020-19160-7.pdf) for choosing the right scientific color map
-
-<td align="left"><img src="pics/choosing-cmap.png" width="500"/></td>
-
-## Get the matplotlib cmap
-
-
-```python
-plt_cmap_obj = sc_map.get_mpl_color_map()
-```
-
-## Choosing the color map for a given type
-
-Get the color maps for a given type
-
-```python
-sc_map = sc.ScicoSequential()
-sc_map.get_color_map_names()
-```
-
-```
-dict_keys(['afmhot', 'amber', 'amber_r', 'amp', 'apple', 'apple_r', 'autumn', 'batlow', 'bilbao', 'bilbao_r', 'binary', 'Blues', 'bone', 'BuGn', 'BuPu', 'chroma', 'chroma_r', 'cividis', 'cool', 'copper', 'cosmic', 'cosmic_r', 'deep', 'dense', 'dusk', 'dusk_r', 'eclipse', 'eclipse_r', 'ember', 'ember_r', 'fall', 'fall_r', 'gem', 'gem_r', 'gist_gray', 'gist_heat', 'gist_yarg', 'GnBu', 'Greens', 'gray', 'Greys', 'haline', 'hawaii', 'hawaii_r', 'heat', 'heat_r', 'hot', 'ice', 'inferno', 'imola', 'imola_r', 'lapaz', 'lapaz_r', 'magma', 'matter', 'neon', 'neon_r', 'neutral', 'neutral_r', 'nuuk', 'nuuk_r', 'ocean', 'ocean_r', 'OrRd', 'Oranges', 'pink', 'plasma', 'PuBu', 'PuBuGn', 'PuRd', 'Purples', 'rain', 'rainbow', 'rainbow-sc', 'rainbow-sc_r', 'rainforest', 'rainforest_r', 'RdPu', 'Reds', 'savanna', 'savanna_r', 'sepia', 'sepia_r', 'speed', 'solar', 'spring', 'summer', 'tempo', 'thermal', 'thermal_r', 'thermal-2', 'tokyo', 'tokyo_r', 'tropical', 'tropical_r', 'turbid', 'turku', 'turku_r', 'viridis', 'winter', 'Wistia', 'YlGn', 'YlGnBu', 'YlOrBr', 'YlOrRd'])
-```
-
-## Assessing a color map
-
-In order to assess if a color map should be corrected or not, `scicomap` provides a way to quickly check if the lightness is linear, how asymmetric and smooth is the chroma and how the color map renders for color-deficient users. I will illustrate some of the artefacts using classical images, as the pyramid and specific functions for each kind of color map.
-
-
-### An infamous example
-
-```python
-import scicomap as sc
-import matplotlib.pyplot as plt
-
-# the thing that should not be
-ugly_jet = plt.get_cmap("jet")
-sc_map =  sc.ScicoMiscellaneous(cmap=ugly_jet)
-f=sc_map.assess_cmap(figsize=(22,10))
-```
-
-
-<td align="left"><img src="pics/jet.png" width="1000"/></td>
- 
-
-Clearly, the lightness is not linear, has edges and kinks. The chroma is not smooth and asymmetrical. See the below illustration to see how bad and how many artefacts the jet color map introduces
-
-
-<td align="left"><img src="pics/jet2.png" width="1000"/></td>
-
-
-## Correcting a color map - Example
-
-### Sequential color map
-
-Let's assess the built-in color map `hawaii` without correction:
-
-```python
-sc_map = sc.ScicoSequential(cmap='hawaii')
-f=sc_map.assess_cmap(figsize=(22,10))
-```
-
-<td align="left"><img src="pics/hawaii.png" width="1000"/></td>
-
-
-The color map seems ok, however, the lightness is not linear and the chroma is asymmetrical even if smooth. Those small defects introduce artefact in the information rendering, as we can visualize using the following example
-
-
-```python
-f=sc_map.draw_example()
-```
-
-<td align="left"><img src="pics/hawaii-examples.png" width="1000"/></td>
-
-
-We can clearly see the artefacts, especially for the pyramid for which our eyes should only pick out the corners in the pyramid (ideal situation). Those artefacts are even more striking for color-deficient users (this might not always be the case). Hopefully, `scicomap` provides an easy way to correct those defects:
-
-```python
-# fixing the color map, using the same minimal lightness (lift=None), 
-# not normalizing to bitone and 
-# smoothing the chroma
-sc_map.unif_sym_cmap(lift=None, 
-                     bitonic=False, 
-                     diffuse=True)
-
-# re-assess the color map after fixing it                     
-f=sc_map.assess_cmap(figsize=(22,10))
-```
-
-<td align="left"><img src="pics/hawaii-fixed.png" width="1000"/></td>
-
-
-After fixing the color map, the artefacts are less present
-
-<td align="left"><img src="pics/hawaii-fixed-examples.png" width="1000"/></td>
-
-# All the built-in color maps
-
-## Sequential
-
-<td align="left"><img src="pics/seq-cmaps-all.png" width="500"/></td>
-
-## Diverging
-
-
-<td align="left"><img src="pics/div-cmaps-all.png" width="500"/></td>
-
-## Mutli-sequential
-
-<td align="left"><img src="pics/multi-cmaps-all.png" width="500"/></td>
-
-## Miscellaneous
-
-<td align="left"><img src="pics/misc-cmaps-all.png" width="500"/></td>
-
-## Circular
-
-<td align="left"><img src="pics/circular-cmaps-all.png" width="500"/></td>
-
-## Qualitative
-
-<td align="left"><img src="pics/qual-cmaps-all.png" width="500"/></td>
-
-# References
-
- * [The misuse of colour in science communication](https://www.nature.com/articles/s41467-020-19160-7.pdf)
- * [Why We Use Bad Color Maps and What You Can Do About It](https://www.kennethmoreland.com/color-advice/BadColorMaps.pdf)
- * [THE RAINBOW IS DEAD…LONG LIVE THE RAINBOW! – SERIES OUTLINE](https://mycarta.wordpress.com/2012/05/29/the-rainbow-is-dead-long-live-the-rainbow-series-outline/)
- * [Scientific colour maps](https://www.fabiocrameri.ch/colourmaps/)
- * [Picking a colour scale for scientific graphics](https://betterfigures.org/2015/06/23/picking-a-colour-scale-for-scientific-graphics/)
- * [ColorCET](https://colorcet.com/)
- * [Good Colour Maps: How to Design Them](https://arxiv.org/abs/1509.03700)
- * [Perceptually uniform color space for image signals including high dynamic range and wide gamut](https://www.osapublishing.org/oe/fulltext.cfm?uri=oe-25-13-15131&id=368272)
-
-
-# Changes log
-
-### 1.0.0
-
- - Docstring
- - Tutorial notebook
- - Web documentation
-
-### 0.4
-
- - Including files in source distributions
-
-### 0.3
-
- - Add a section "how to use with matplotlib"
- - [Bug] Center diverging color map in examples
-
-### 0.2
-
- - [Bug] Fix typo in chart titles
-
-### 0.1
-
- - First version
+<img src="pics/logo.png" alt="drawing" width="200"/>
+
+[buy me caffeine](https://ko-fi.com/V7V72SOHX)
+
+
+
+# Scientific color maps 
+
+## Blog post
+
+[Scicomap Medium blog post (free)](https://towardsdatascience.com/your-colour-map-is-bad-heres-how-to-fix-it-lessons-learnt-from-the-event-horizon-telescope-b82523f09469)
+
+[Official Documentation](https://scicomap.readthedocs.io/en/latest/)
+
+[Tutorial notebook](./docs/notebooks/tutorial.ipynb)
+
+## Installation
+
+```shell
+pip install scicomap
+```
+
+## Introduction 
+
+Scicomap is a package that provides scientific color maps and tools to standardize your favourite color maps if you don't like the built-in ones.
+Scicomap currently provides sequential, bi-sequential, diverging, circular, qualitative and miscellaneous color maps. You can easily draw examples, compare the rendering, see how colorblind people will perceive the color maps. I will illustrate the scicomap capabilities below.
+
+This package is heavily based on the [Event Horyzon Plot package](https://github.com/liamedeiros/ehtplot/tree/docs) and uses good color maps found in the [the python portage of the Fabio Crameri](https://github.com/callumrollo/cmcrameri), [cmasher](https://cmasher.readthedocs.io/), [palettable](https://jiffyclub.github.io/palettable/), [colorcet](https://colorcet.holoviz.org/) and [cmocean](https://matplotlib.org/cmocean/)
+
+## Motivation
+
+The accurate representation of data is essential. Many common color maps distort data through uneven colour gradients and are often unreadable to those with color-vision deficiency. An infamous example is the jet color map. These color maps do not render all the information you want to illustrate or even worse render false information through artefacts. Scientist or not, your goal is to communicate visual information in the most accurate and appealing fashion. Moreover, do not overlook colour-vision deficiency, which represents 8% of the (Caucasian) male population.
+
+## Color spaces
+
+Perceptual uniformity is the idea that Euclidean distance between colors in color space should match human color perception distance judgements. For example, a blue and red that are at a distance d apart should look as discriminable as green and purple that are at a distance d apart.
+Scicomap uses the CAM02-UCS color space (Uniform Colour Space). Its three coordinates are usually denoted by J', a', and b'. And its cylindrical coordinates are J', C', and h'. The perceptual color space Jab is similar to Lab. However, Jab uses an updated color appearance model that in theory provides greater precision for discriminability measurements.
+
+ * Lightness: also known as value or tone, is a representation of a color's brightness
+ * Chroma: the intrinsic difference between a color and gray of an object
+ * Hue: the degree to which a stimulus can be described as similar to or different from stimuli that are described as red, green, blue, and yellow
+
+## Encoding information
+
+ * Lightness J': for a scalar value, intensity. It must vary linearly with the physical quantity
+ * hue h' can encode an additional physical quantity, the change of hue should be linearly proportional to the quantity. The hue h' is also ideal in making an image more attractive without interfering with the representation of pixel values.
+ * chroma is less recognizable and should not be used to encode physical information
+  
+## Color map uniformization
+
+Following the references and the theories, the uniformization is performed by
+
+ * Making the color map linear in J'
+ * Lifting the color map (making it lighter, i.e. increasing the minimal value of J')
+ * Symmetrizing the chroma to avoid further artefacts
+ * Avoid kinks and edges in the chroma curve
+ * Bitonic symmetrization or not
+
+
+# Scicomap
+
+## Choosing the right type of color maps
+Scicomap provides a bunch of color maps for different applications. The different types of color map are 
+
+```python
+import scicomap as sc
+sc_map = sc.SciCoMap()
+sc_map.get_ctype()
+```
+
+```
+dict_keys(['diverging', 'sequential', 'multi-sequential', 'circular', 'miscellaneous', 'qualitative'])
+```
+
+I'll refer to the [The misuse of colour in science communication](https://www.nature.com/articles/s41467-020-19160-7.pdf) for choosing the right scientific color map
+
+<td align="left"><img src="pics/choosing-cmap.png" width="500"/></td>
+
+## Get the matplotlib cmap
+
+
+```python
+plt_cmap_obj = sc_map.get_mpl_color_map()
+```
+
+## Choosing the color map for a given type
+
+Get the color maps for a given type
+
+```python
+sc_map = sc.ScicoSequential()
+sc_map.get_color_map_names()
+```
+
+```
+dict_keys(['afmhot', 'amber', 'amber_r', 'amp', 'apple', 'apple_r', 'autumn', 'batlow', 'bilbao', 'bilbao_r', 'binary', 'Blues', 'bone', 'BuGn', 'BuPu', 'chroma', 'chroma_r', 'cividis', 'cool', 'copper', 'cosmic', 'cosmic_r', 'deep', 'dense', 'dusk', 'dusk_r', 'eclipse', 'eclipse_r', 'ember', 'ember_r', 'fall', 'fall_r', 'gem', 'gem_r', 'gist_gray', 'gist_heat', 'gist_yarg', 'GnBu', 'Greens', 'gray', 'Greys', 'haline', 'hawaii', 'hawaii_r', 'heat', 'heat_r', 'hot', 'ice', 'inferno', 'imola', 'imola_r', 'lapaz', 'lapaz_r', 'magma', 'matter', 'neon', 'neon_r', 'neutral', 'neutral_r', 'nuuk', 'nuuk_r', 'ocean', 'ocean_r', 'OrRd', 'Oranges', 'pink', 'plasma', 'PuBu', 'PuBuGn', 'PuRd', 'Purples', 'rain', 'rainbow', 'rainbow-sc', 'rainbow-sc_r', 'rainforest', 'rainforest_r', 'RdPu', 'Reds', 'savanna', 'savanna_r', 'sepia', 'sepia_r', 'speed', 'solar', 'spring', 'summer', 'tempo', 'thermal', 'thermal_r', 'thermal-2', 'tokyo', 'tokyo_r', 'tropical', 'tropical_r', 'turbid', 'turku', 'turku_r', 'viridis', 'winter', 'Wistia', 'YlGn', 'YlGnBu', 'YlOrBr', 'YlOrRd'])
+```
+
+## Assessing a color map
+
+In order to assess if a color map should be corrected or not, `scicomap` provides a way to quickly check if the lightness is linear, how asymmetric and smooth is the chroma and how the color map renders for color-deficient users. I will illustrate some of the artefacts using classical images, as the pyramid and specific functions for each kind of color map.
+
+
+### An infamous example
+
+```python
+import scicomap as sc
+import matplotlib.pyplot as plt
+
+# the thing that should not be
+ugly_jet = plt.get_cmap("jet")
+sc_map =  sc.ScicoMiscellaneous(cmap=ugly_jet)
+f=sc_map.assess_cmap(figsize=(22,10))
+```
+
+
+<td align="left"><img src="pics/jet.png" width="1000"/></td>
+ 
+
+Clearly, the lightness is not linear, has edges and kinks. The chroma is not smooth and asymmetrical. See the below illustration to see how bad and how many artefacts the jet color map introduces
+
+
+<td align="left"><img src="pics/jet2.png" width="1000"/></td>
+
+
+## Correcting a color map - Example
+
+### Sequential color map
+
+Let's assess the built-in color map `hawaii` without correction:
+
+```python
+sc_map = sc.ScicoSequential(cmap='hawaii')
+f=sc_map.assess_cmap(figsize=(22,10))
+```
+
+<td align="left"><img src="pics/hawaii.png" width="1000"/></td>
+
+
+The color map seems ok, however, the lightness is not linear and the chroma is asymmetrical even if smooth. Those small defects introduce artefact in the information rendering, as we can visualize using the following example
+
+
+```python
+f=sc_map.draw_example()
+```
+
+<td align="left"><img src="pics/hawaii-examples.png" width="1000"/></td>
+
+
+We can clearly see the artefacts, especially for the pyramid for which our eyes should only pick out the corners in the pyramid (ideal situation). Those artefacts are even more striking for color-deficient users (this might not always be the case). Hopefully, `scicomap` provides an easy way to correct those defects:
+
+```python
+# fixing the color map, using the same minimal lightness (lift=None), 
+# not normalizing to bitone and 
+# smoothing the chroma
+sc_map.unif_sym_cmap(lift=None, 
+                     bitonic=False, 
+                     diffuse=True)
+
+# re-assess the color map after fixing it                     
+f=sc_map.assess_cmap(figsize=(22,10))
+```
+
+<td align="left"><img src="pics/hawaii-fixed.png" width="1000"/></td>
+
+
+After fixing the color map, the artefacts are less present
+
+<td align="left"><img src="pics/hawaii-fixed-examples.png" width="1000"/></td>
+
+# All the built-in color maps
+
+## Sequential
+
+<td align="left"><img src="pics/seq-cmaps-all.png" width="500"/></td>
+
+## Diverging
+
+
+<td align="left"><img src="pics/div-cmaps-all.png" width="500"/></td>
+
+## Mutli-sequential
+
+<td align="left"><img src="pics/multi-cmaps-all.png" width="500"/></td>
+
+## Miscellaneous
+
+<td align="left"><img src="pics/misc-cmaps-all.png" width="500"/></td>
+
+## Circular
+
+<td align="left"><img src="pics/circular-cmaps-all.png" width="500"/></td>
+
+## Qualitative
+
+<td align="left"><img src="pics/qual-cmaps-all.png" width="500"/></td>
+
+# References
+
+ * [The misuse of colour in science communication](https://www.nature.com/articles/s41467-020-19160-7.pdf)
+ * [Why We Use Bad Color Maps and What You Can Do About It](https://www.kennethmoreland.com/color-advice/BadColorMaps.pdf)
+ * [THE RAINBOW IS DEAD…LONG LIVE THE RAINBOW! – SERIES OUTLINE](https://mycarta.wordpress.com/2012/05/29/the-rainbow-is-dead-long-live-the-rainbow-series-outline/)
+ * [Scientific colour maps](https://www.fabiocrameri.ch/colourmaps/)
+ * [Picking a colour scale for scientific graphics](https://betterfigures.org/2015/06/23/picking-a-colour-scale-for-scientific-graphics/)
+ * [ColorCET](https://colorcet.com/)
+ * [Good Colour Maps: How to Design Them](https://arxiv.org/abs/1509.03700)
+ * [Perceptually uniform color space for image signals including high dynamic range and wide gamut](https://www.osapublishing.org/oe/fulltext.cfm?uri=oe-25-13-15131&id=368272)
+
+
+# Changes log
+
+### 1.0.0
+
+ - Docstring
+ - Tutorial notebook
+ - Web documentation
+
+### 0.4
+
+ - Including files in source distributions
+
+### 0.3
+
+ - Add a section "how to use with matplotlib"
+ - [Bug] Center diverging color map in examples
+
+### 0.2
+
+ - [Bug] Fix typo in chart titles
+
+### 0.1
+
+ - First version
```

### Comparing `scicomap-1.0.0/pyproject.toml` & `scicomap-1.0.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-[build-system]
-requires = ["setuptools"]
-build-backend = "setuptools.build_meta"
-
-[tool.setuptools.dynamic]
-version = {attr = "scicomap.__version__"}
-
-[tool.setuptools]
-package-data = {"scicomap.data" = ["*.png", "*.npz", "*.gz", "*.jpg"]}
-
-[project]
-name = "scicomap"
-dynamic = ["version"]
-requires-python = ">=3.8"
-description = "data visualization on maps with varying levels of granularity"
-authors = [{name = "Thomas Bury", email = "bury.thomas@gmail.com"}]
-readme = {file = "README.md", content-type = "text/markdown"}
-keywords = ["visualization", "color", "uniform", "scientific"]
-license = {file = "LICENSE.md"}
-classifiers = [
-    "Programming Language :: Python :: 3"
-]
-
-dependencies = [
-    "numpy",
-    "pandas",
-    "scipy",
-    "colorspacious",
-    "colorcet",
-    "cmcrameri",
-    "cmocean",
-    "cmasher >= 1.5.8",
-    "palettable >= 3.3.0",
-    "matplotlib >= 3.3.0",
-]
-
-[project.urls]
-homepage = "https://github.com/ThomasBury/scicomap"
-documentation = "https://github.com/ThomasBury/scicomap"
-repository = "https://github.com/ThomasBury/scicomap.git"
-changelog = "https://github.com/ThomasBury/scicomap"
-Tracker = "https://github.com/ThomasBury/scicomap/issues"
-
-[project.optional-dependencies]
-doc = [
-    "ipykernel",
-    "ipython_genutils",
-    "pandoc",
-    "sphinx",
-    "sphinxawesome-theme==5.0.0b5",
-    "nbsphinx",
-    "sphinx-autodoc-typehints",
-    "sphinx-copybutton",
-    "sphinx-tabs",
-]
-lint = [
-    "black",
-    "flake8"
-]
-test = [
-    "pytest",
-    "pytest-cov",
-]
+[build-system]
+requires = ["setuptools"]
+build-backend = "setuptools.build_meta"
+
+[tool.setuptools.dynamic]
+version = {attr = "scicomap.__version__"}
+
+[tool.setuptools]
+package-data = {"scicomap.data" = ["*.png", "*.npz", "*.gz", "*.jpg"]}
+
+[project]
+name = "scicomap"
+dynamic = ["version"]
+requires-python = ">=3.10"
+description = "data visualization on maps with varying levels of granularity"
+authors = [{name = "Thomas Bury", email = "bury.thomas@gmail.com"}]
+readme = {file = "README.md", content-type = "text/markdown"}
+keywords = ["visualization", "color", "uniform", "scientific"]
+license = {file = "LICENSE.md"}
+classifiers = [
+    "Programming Language :: Python :: 3"
+]
+
+dependencies = [
+    "numpy",
+    "pandas",
+    "scipy",
+    "colorspacious",
+    "colorcet",
+    "cmcrameri",
+    "cmocean",
+    "cmasher >= 1.5.8",
+    "palettable >= 3.3.0",
+    "matplotlib >= 3.3.0",
+]
+
+[project.urls]
+homepage = "https://github.com/ThomasBury/scicomap"
+documentation = "https://github.com/ThomasBury/scicomap"
+repository = "https://github.com/ThomasBury/scicomap.git"
+changelog = "https://github.com/ThomasBury/scicomap"
+Tracker = "https://github.com/ThomasBury/scicomap/issues"
+
+[project.optional-dependencies]
+doc = [
+    "ipykernel",
+    "ipython_genutils",
+    "pandoc",
+    "sphinx",
+    "sphinxawesome-theme==5.0.0b5",
+    "nbsphinx",
+    "sphinx-autodoc-typehints",
+    "sphinx-copybutton",
+    "sphinx-tabs",
+]
+lint = [
+    "black",
+    "flake8"
+]
+test = [
+    "pytest",
+    "pytest-cov",
+]
```

### Comparing `scicomap-1.0.0/src/scicomap/cblind.py` & `scicomap-1.0.1/src/scicomap/cblind.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,337 +1,337 @@
-"""
-Module collecting function for evaluating and transforming cmap to render
-color weak or blind vision
-"""
-
-import itertools
-import numpy as np
-import matplotlib.pyplot as plt
-from typing import List, Tuple, Union, Callable, Optional
-from colorspacious import cspace_converter
-from matplotlib.colors import Colormap, ListedColormap
-from scicomap.cmath import get_ctab
-
-_deuter50_space = {"name": "sRGB1+CVD", "cvd_type": "deuteranomaly", "severity": 50}
-_deuter50_to_sRGB1 = cspace_converter(_deuter50_space, "sRGB1")
-
-_deuter100_space = {"name": "sRGB1+CVD", "cvd_type": "deuteranomaly", "severity": 100}
-_deuter100_to_sRGB1 = cspace_converter(_deuter100_space, "sRGB1")
-
-_prot50_space = {"name": "sRGB1+CVD", "cvd_type": "protanomaly", "severity": 50}
-_prot50_to_sRGB1 = cspace_converter(_prot50_space, "sRGB1")
-
-_prot100_space = {"name": "sRGB1+CVD", "cvd_type": "protanomaly", "severity": 100}
-_prot100_to_sRGB1 = cspace_converter(_prot100_space, "sRGB1")
-
-_trit50_space = {"name": "sRGB1+CVD", "cvd_type": "tritanomaly", "severity": 50}
-_trit50_to_sRGB1 = cspace_converter(_trit50_space, "sRGB1")
-
-_trit100_space = {"name": "sRGB1+CVD", "cvd_type": "tritanomaly", "severity": 100}
-_trit100_to_sRGB1 = cspace_converter(_trit100_space, "sRGB1")
-
-
-def colorblind_transform(RGBA: np.ndarray, colorblind_space: callable) -> np.ndarray:
-    """
-    Apply a colorblind transformation to an RGBA image.
-
-    Parameters
-    ----------
-    RGBA : np.ndarray
-        An input RGBA image represented as a NumPy array with shape (..., 4).
-    colorblind_space : callable
-        A callable representing the colorblind transformation function.
-        This function should take an RGB color (as a NumPy array with shape (..., 3))
-        as input and return the transformed RGB color as output.
-
-    Returns
-    -------
-    np.ndarray
-        The colorblind-transformed RGBA image, represented as a NumPy array with the same shape
-        as the input RGBA, where the RGB channels are transformed and the alpha channel is preserved.
-
-    Notes
-    -----
-    This function applies a colorblind transformation to an RGBA image by first clipping the input
-    colors, applying the colorblind transformation using the provided `colorblind_space` function,
-    and then concatenating the transformed RGB channels with the original alpha channel.
-
-    The `colorblind_space` function should accept an RGB color (as a NumPy array with shape (..., 3))
-    and return the transformed RGB color.
-
-    Example
-    -------
-    >>> import numpy as np
-    >>> def simulate_colorblindness(rgb):
-    ...     # Simulate colorblindness by desaturating the colors
-    ...     return np.mean(rgb, axis=-1, keepdims=True)
-    >>> rgba_image = np.random.rand(10, 10, 4)  # Example RGBA image
-    >>> transformed_image = colorblind_transform(rgba_image, simulate_colorblindness)
-    """
-    # clipping, alpha handling
-    RGB = RGBA[..., :3]
-    RGB = np.clip(colorblind_space(RGB), 0, 1)
-    return np.concatenate((RGB, RGBA[..., 3:]), axis=-1)
-
-
-def _get_color_weak_cmap(
-    color_map: Union[str, Colormap],
-    n_images: int
-) -> Tuple[List[Union[str, Colormap]], List[str]]:
-    """
-    Generate color maps for different color vision deficiencies.
-
-    Parameters
-    ----------
-    color_map : str or mcolors.Colormap
-        The base color map to be used.
-    n_images : int
-        The number of color maps to generate, including the base color map.
-
-    Returns
-    -------
-    Tuple[List[Union[str, mcolors.Colormap]], List[str]]
-        A tuple containing two lists:
-        1. List of color maps, including the base color map and color maps transformed for color vision deficiencies.
-        2. List of subtitles describing each color map in the order they appear in the color maps list.
-
-    Notes
-    -----
-    This function generates color maps for different color vision deficiencies, including deuteranopia and protanopia,
-    by transforming the base color map using colorblind transformations. It also generates color maps for tritanopia
-    and a normal color vision map. The `n_images` parameter specifies the total number of color maps to generate.
-
-    Example
-    -------
-    >>> base_cmap = 'viridis'
-    >>> n_color_maps = 5
-    >>> c_maps, sub_title = _get_color_weak_cmap(base_cmap, n_color_maps)
-    >>> print(c_maps)
-    >>> print(sub_title)
-    """
-    _deuter50_transform = lambda x: colorblind_transform(x, _deuter50_to_sRGB1)
-    _deuter100_transform = lambda x: colorblind_transform(x, _deuter100_to_sRGB1)
-    _prot50_transform = lambda x: colorblind_transform(x, _prot50_to_sRGB1)
-    _trit100_transform = lambda x: colorblind_transform(x, _trit100_to_sRGB1)
-
-    deuter50_cm = _colorblind_cmap(color_map, _deuter50_transform)
-    deuter100_cm = _colorblind_cmap(color_map, _deuter100_transform)
-    prot50_cm = _colorblind_cmap(color_map, _prot50_transform)
-    trit100_cm = _colorblind_cmap(color_map, _trit100_transform)
-    c_maps = [color_map, deuter50_cm, prot50_cm, deuter100_cm, trit100_cm]
-    n_blank = n_images - 1
-    sub_title = (
-        ["Normal\n(~95%% of pop)"]
-        + n_blank * [""]
-        + ["Deuter-50%\n(RG-weak, D/P: 5%% of male)"]
-        + n_blank * [""]
-        + ["Prot-50%\n(RG-weak, D/P: 5%% of male)"]
-        + n_blank * [""]
-        + ["Deuter-100%\n(RG-blind, D/P: 5%% of male)"]
-        + n_blank * [""]
-        + ["Trit-100%%\n(BY deficient, very rare)"]
-        + n_blank * [""]
-    )
-
-    return c_maps, sub_title
-
-
-def _get_color_weak_ctab(
-    color_map: Union[str, Callable],
-    n_blank: int
-) -> Tuple[List[np.ndarray], List[str]]:
-    """
-    Generate color tables (ctabs) for different color vision deficiencies.
-
-    Parameters
-    ----------
-    color_map : str or Callable
-        The base color map or a callable function to generate it.
-    n_blank : int
-        The number of blank entries to insert between each pair of generated color tables.
-
-    Returns
-    -------
-    Tuple[List[np.ndarray], List[str]]
-        A tuple containing two lists:
-        1. List of color tables, including the base color table and tables transformed for color vision deficiencies.
-        2. List of subtitles describing each color table in the order they appear in the color tables list.
-
-    Notes
-    -----
-    This function generates color tables (ctabs) for different color vision deficiencies, including deuteranopia and protanopia,
-    by transforming the base color table using colorblind transformations. It also generates color tables for tritanopia
-    and a normal color vision table. The `n_blank` parameter specifies the number of blank entries between each pair
-    of generated color tables.
-
-    Example
-    -------
-    >>> base_color_map = 'viridis'
-    >>> n_blank_entries = 3
-    >>> c_tabs, sub_title = _get_color_weak_ctab(base_color_map, n_blank_entries)
-    >>> print(c_tabs)
-    >>> print(sub_title)
-    """
-    _deuter100_transform = lambda x: colorblind_transform(x, _deuter100_to_sRGB1)
-    ctab = get_ctab(color_map)  # get the colormap as a color table in sRGB
-    ctab_deuter100 = _deuter100_transform(ctab)
-
-    _deuter50_transform = lambda x: colorblind_transform(x, _deuter50_to_sRGB1)
-    ctab_deuter50 = _deuter50_transform(ctab)
-
-    _prot50_transform = lambda x: colorblind_transform(x, _prot50_to_sRGB1)
-    ctab_prot50 = _prot50_transform(ctab)
-
-    _trit100_transform = lambda x: colorblind_transform(x, _trit100_to_sRGB1)
-    # _trit100_transform = lambda x: colorblind_transform(x, _trit100_to_sRGB1)
-    ctab_trit100 = _trit100_transform(ctab)
-
-    c_tabs = [ctab, ctab_deuter50, ctab_prot50, ctab_deuter100, ctab_trit100]
-    sub_title = (
-        ["Normal\n(~95%% of pop)"]
-        + n_blank * [""]
-        + ["Deuter-50%\n(RG-weak, D/P: 5%% of male)"]
-        + n_blank * [""]
-        + ["Prot-50%\n(RG-weak, D/P: 5%% of male)"]
-        + n_blank * [""]
-        + ["Deuter-100%\n(RG-blind, D/P: 5%% of male)"]
-        + n_blank * [""]
-        + ["Trit-100%\n(BY deficient, very rare)"]
-        + n_blank * [""]
-    )
-
-    return c_tabs, sub_title
-
-
-def _colorblind_cmap(
-    cmap: Union[str, Callable],
-    c_space_transf: Callable
-) -> ListedColormap:
-    """
-    Create a colorblind-friendly colormap by applying a color space transformation to a base colormap.
-
-    Parameters
-    ----------
-    cmap : str or Callable
-        The base colormap or a callable function to generate it.
-    c_space_transf : Callable
-        A function for transforming the color space to create a colorblind-friendly colormap.
-
-    Returns
-    -------
-    ListedColormap
-        A colorblind-friendly colormap created by applying the specified color space transformation.
-
-    Notes
-    -----
-    This function takes a base colormap and applies a color space transformation using the provided `c_space_transf`
-    function to create a colorblind-friendly colormap. It returns the resulting colormap as a `ListedColormap` object.
-
-    Example
-    -------
-    >>> base_colormap = 'viridis'
-    >>> def deuteranopia_transform(x):
-    ...     # Your color space transformation function for deuteranopia
-    ...     pass
-    >>> colorblind_cm = _colorblind_cmap(base_colormap, deuteranopia_transform)
-    >>> print(colorblind_cm)
-    """
-    ctab = get_ctab(cmap)  # get the colormap as a color table in sRGB
-    ctab_cb = c_space_transf(ctab)
-    return ListedColormap(np.clip(ctab_cb, 0, 1))
-
-def colorblind_vision(
-    cmap: Union[str, List[str], List[Colormap]],
-    figsize: Optional[Tuple[int, int]] = None,
-    n_colors: int = 10,
-    facecolor: str = "black"
-) -> plt.Figure:
-    """
-    Generate a visualization of colorblind-friendly colormaps.
-
-    Parameters
-    ----------
-    cmap : str, list of str, or list of plt.Colormap
-        The base colormap(s) or list of colormaps to visualize.
-    figsize : tuple of int, optional
-        The size of the generated figure (width, height).
-    n_colors : int, optional (default=10)
-        The number of colors to include in the colorblind visualization.
-    facecolor : {'black', 'white'}, optional (default='black')
-        The facecolor for the generated figure.
-
-    Returns
-    -------
-    plt.Figure
-        A Matplotlib figure showing colorblind-friendly versions of the specified colormap(s).
-
-    Notes
-    -----
-    This function generates a figure displaying colorblind-friendly versions of the input colormap(s).
-    It creates subplots for each colormap and visualizes the colormap with a gradient of colors.
-
-    Example
-    -------
-    >>> base_colormap = 'viridis'
-    >>> colorblind_fig = colorblind_vision(base_colormap, figsize=(8, 6))
-    >>> plt.show()
-    """
-
-    gradient = np.linspace(0, 1, n_colors)
-    gradient = np.vstack((gradient, gradient))
-
-    cmap_dic = {}
-    visible_spectrum_cmap = plt.get_cmap("gist_rainbow")
-    spectral_list, _ = _get_color_weak_cmap(color_map=visible_spectrum_cmap, n_images=0)
-    cmap_dic["visible spectrum"] = spectral_list
-
-    if isinstance(cmap, list):
-        for cm in cmap:
-            cmap_list, _ = _get_color_weak_cmap(color_map=cm, n_images=0)
-            cmap_dic[cm.name] = cmap_list
-    else:
-        cmap_list, _ = _get_color_weak_cmap(color_map=cmap, n_images=0)
-        cmap_dic[cmap.name] = cmap_list
-
-    sub_titles = (
-        ["Normal\n~95%% of pop"]
-        + ["Deuter-50%\nRG-weak, D/P: 5%% of male"]
-        + ["Prot-50%\nRG-weak, D/P: 5%% of male"]
-        + ["Deuter-100%\nRG-blind, D/P: 5%% of male"]
-        + ["Trit-100%\nBY deficient, very rare"]
-    )
-
-    nrows = len(spectral_list)
-    ncols = len(cmap_dic)
-
-    if figsize is None:
-        figsize = (10, 0.25 * nrows)
-
-    fontcolor = "white" if facecolor == "black" else "black"
-    fig, axes = plt.subplots(
-        nrows=nrows, ncols=ncols, figsize=figsize, facecolor=facecolor
-    )
-    fig.subplots_adjust(top=0.95, bottom=0.01, left=0.2, right=0.99)
-
-    cmap_list = list(cmap_dic.values())
-    cmap_name = list(cmap_dic.keys())
-
-    for i, j in itertools.product(range(nrows), range(ncols)):
-        ax = axes[i, j]
-        cmap = cmap_list[j][i]
-        ax.imshow(gradient, aspect="auto", cmap=cmap)
-        if i == 0:
-            font = {"color": fontcolor, "size": 24}
-            ax.set_title(cmap_name[j], fontdict=font)
-        if j == 0:
-            font = {"color": fontcolor, "size": 14}
-            pos = list(ax.get_position().bounds)
-            x_text = pos[0] - 0.01
-            y_text = pos[1] + pos[3] / 2.0
-            fig.text(
-                x_text, y_text, sub_titles[i], va="center", ha="right", fontdict=font
-            )
-
-    for ax in axes:
-        ax[0].set_axis_off()
-        ax[1].set_axis_off()
-    return fig
+"""
+Module collecting function for evaluating and transforming cmap to render
+color weak or blind vision
+"""
+
+import itertools
+import numpy as np
+import matplotlib.pyplot as plt
+from typing import List, Tuple, Union, Callable, Optional
+from colorspacious import cspace_converter
+from matplotlib.colors import Colormap, ListedColormap
+from scicomap.cmath import get_ctab
+
+_deuter50_space = {"name": "sRGB1+CVD", "cvd_type": "deuteranomaly", "severity": 50}
+_deuter50_to_sRGB1 = cspace_converter(_deuter50_space, "sRGB1")
+
+_deuter100_space = {"name": "sRGB1+CVD", "cvd_type": "deuteranomaly", "severity": 100}
+_deuter100_to_sRGB1 = cspace_converter(_deuter100_space, "sRGB1")
+
+_prot50_space = {"name": "sRGB1+CVD", "cvd_type": "protanomaly", "severity": 50}
+_prot50_to_sRGB1 = cspace_converter(_prot50_space, "sRGB1")
+
+_prot100_space = {"name": "sRGB1+CVD", "cvd_type": "protanomaly", "severity": 100}
+_prot100_to_sRGB1 = cspace_converter(_prot100_space, "sRGB1")
+
+_trit50_space = {"name": "sRGB1+CVD", "cvd_type": "tritanomaly", "severity": 50}
+_trit50_to_sRGB1 = cspace_converter(_trit50_space, "sRGB1")
+
+_trit100_space = {"name": "sRGB1+CVD", "cvd_type": "tritanomaly", "severity": 100}
+_trit100_to_sRGB1 = cspace_converter(_trit100_space, "sRGB1")
+
+
+def colorblind_transform(RGBA: np.ndarray, colorblind_space: callable) -> np.ndarray:
+    """
+    Apply a colorblind transformation to an RGBA image.
+
+    Parameters
+    ----------
+    RGBA : np.ndarray
+        An input RGBA image represented as a NumPy array with shape (..., 4).
+    colorblind_space : callable
+        A callable representing the colorblind transformation function.
+        This function should take an RGB color (as a NumPy array with shape (..., 3))
+        as input and return the transformed RGB color as output.
+
+    Returns
+    -------
+    np.ndarray
+        The colorblind-transformed RGBA image, represented as a NumPy array with the same shape
+        as the input RGBA, where the RGB channels are transformed and the alpha channel is preserved.
+
+    Notes
+    -----
+    This function applies a colorblind transformation to an RGBA image by first clipping the input
+    colors, applying the colorblind transformation using the provided `colorblind_space` function,
+    and then concatenating the transformed RGB channels with the original alpha channel.
+
+    The `colorblind_space` function should accept an RGB color (as a NumPy array with shape (..., 3))
+    and return the transformed RGB color.
+
+    Example
+    -------
+    >>> import numpy as np
+    >>> def simulate_colorblindness(rgb):
+    ...     # Simulate colorblindness by desaturating the colors
+    ...     return np.mean(rgb, axis=-1, keepdims=True)
+    >>> rgba_image = np.random.rand(10, 10, 4)  # Example RGBA image
+    >>> transformed_image = colorblind_transform(rgba_image, simulate_colorblindness)
+    """
+    # clipping, alpha handling
+    RGB = RGBA[..., :3]
+    RGB = np.clip(colorblind_space(RGB), 0, 1)
+    return np.concatenate((RGB, RGBA[..., 3:]), axis=-1)
+
+
+def _get_color_weak_cmap(
+    color_map: Union[str, Colormap],
+    n_images: int
+) -> Tuple[List[Union[str, Colormap]], List[str]]:
+    """
+    Generate color maps for different color vision deficiencies.
+
+    Parameters
+    ----------
+    color_map : str or mcolors.Colormap
+        The base color map to be used.
+    n_images : int
+        The number of color maps to generate, including the base color map.
+
+    Returns
+    -------
+    Tuple[List[Union[str, mcolors.Colormap]], List[str]]
+        A tuple containing two lists:
+        1. List of color maps, including the base color map and color maps transformed for color vision deficiencies.
+        2. List of subtitles describing each color map in the order they appear in the color maps list.
+
+    Notes
+    -----
+    This function generates color maps for different color vision deficiencies, including deuteranopia and protanopia,
+    by transforming the base color map using colorblind transformations. It also generates color maps for tritanopia
+    and a normal color vision map. The `n_images` parameter specifies the total number of color maps to generate.
+
+    Example
+    -------
+    >>> base_cmap = 'viridis'
+    >>> n_color_maps = 5
+    >>> c_maps, sub_title = _get_color_weak_cmap(base_cmap, n_color_maps)
+    >>> print(c_maps)
+    >>> print(sub_title)
+    """
+    _deuter50_transform = lambda x: colorblind_transform(x, _deuter50_to_sRGB1)
+    _deuter100_transform = lambda x: colorblind_transform(x, _deuter100_to_sRGB1)
+    _prot50_transform = lambda x: colorblind_transform(x, _prot50_to_sRGB1)
+    _trit100_transform = lambda x: colorblind_transform(x, _trit100_to_sRGB1)
+
+    deuter50_cm = _colorblind_cmap(color_map, _deuter50_transform)
+    deuter100_cm = _colorblind_cmap(color_map, _deuter100_transform)
+    prot50_cm = _colorblind_cmap(color_map, _prot50_transform)
+    trit100_cm = _colorblind_cmap(color_map, _trit100_transform)
+    c_maps = [color_map, deuter50_cm, prot50_cm, deuter100_cm, trit100_cm]
+    n_blank = n_images - 1
+    sub_title = (
+        ["Normal\n(~95%% of pop)"]
+        + n_blank * [""]
+        + ["Deuter-50%\n(RG-weak, D/P: 5%% of male)"]
+        + n_blank * [""]
+        + ["Prot-50%\n(RG-weak, D/P: 5%% of male)"]
+        + n_blank * [""]
+        + ["Deuter-100%\n(RG-blind, D/P: 5%% of male)"]
+        + n_blank * [""]
+        + ["Trit-100%%\n(BY deficient, very rare)"]
+        + n_blank * [""]
+    )
+
+    return c_maps, sub_title
+
+
+def _get_color_weak_ctab(
+    color_map: Union[str, Callable],
+    n_blank: int
+) -> Tuple[List[np.ndarray], List[str]]:
+    """
+    Generate color tables (ctabs) for different color vision deficiencies.
+
+    Parameters
+    ----------
+    color_map : str or Callable
+        The base color map or a callable function to generate it.
+    n_blank : int
+        The number of blank entries to insert between each pair of generated color tables.
+
+    Returns
+    -------
+    Tuple[List[np.ndarray], List[str]]
+        A tuple containing two lists:
+        1. List of color tables, including the base color table and tables transformed for color vision deficiencies.
+        2. List of subtitles describing each color table in the order they appear in the color tables list.
+
+    Notes
+    -----
+    This function generates color tables (ctabs) for different color vision deficiencies, including deuteranopia and protanopia,
+    by transforming the base color table using colorblind transformations. It also generates color tables for tritanopia
+    and a normal color vision table. The `n_blank` parameter specifies the number of blank entries between each pair
+    of generated color tables.
+
+    Example
+    -------
+    >>> base_color_map = 'viridis'
+    >>> n_blank_entries = 3
+    >>> c_tabs, sub_title = _get_color_weak_ctab(base_color_map, n_blank_entries)
+    >>> print(c_tabs)
+    >>> print(sub_title)
+    """
+    _deuter100_transform = lambda x: colorblind_transform(x, _deuter100_to_sRGB1)
+    ctab = get_ctab(color_map)  # get the colormap as a color table in sRGB
+    ctab_deuter100 = _deuter100_transform(ctab)
+
+    _deuter50_transform = lambda x: colorblind_transform(x, _deuter50_to_sRGB1)
+    ctab_deuter50 = _deuter50_transform(ctab)
+
+    _prot50_transform = lambda x: colorblind_transform(x, _prot50_to_sRGB1)
+    ctab_prot50 = _prot50_transform(ctab)
+
+    _trit100_transform = lambda x: colorblind_transform(x, _trit100_to_sRGB1)
+    # _trit100_transform = lambda x: colorblind_transform(x, _trit100_to_sRGB1)
+    ctab_trit100 = _trit100_transform(ctab)
+
+    c_tabs = [ctab, ctab_deuter50, ctab_prot50, ctab_deuter100, ctab_trit100]
+    sub_title = (
+        ["Normal\n(~95%% of pop)"]
+        + n_blank * [""]
+        + ["Deuter-50%\n(RG-weak, D/P: 5%% of male)"]
+        + n_blank * [""]
+        + ["Prot-50%\n(RG-weak, D/P: 5%% of male)"]
+        + n_blank * [""]
+        + ["Deuter-100%\n(RG-blind, D/P: 5%% of male)"]
+        + n_blank * [""]
+        + ["Trit-100%\n(BY deficient, very rare)"]
+        + n_blank * [""]
+    )
+
+    return c_tabs, sub_title
+
+
+def _colorblind_cmap(
+    cmap: Union[str, Callable],
+    c_space_transf: Callable
+) -> ListedColormap:
+    """
+    Create a colorblind-friendly colormap by applying a color space transformation to a base colormap.
+
+    Parameters
+    ----------
+    cmap : str or Callable
+        The base colormap or a callable function to generate it.
+    c_space_transf : Callable
+        A function for transforming the color space to create a colorblind-friendly colormap.
+
+    Returns
+    -------
+    ListedColormap
+        A colorblind-friendly colormap created by applying the specified color space transformation.
+
+    Notes
+    -----
+    This function takes a base colormap and applies a color space transformation using the provided `c_space_transf`
+    function to create a colorblind-friendly colormap. It returns the resulting colormap as a `ListedColormap` object.
+
+    Example
+    -------
+    >>> base_colormap = 'viridis'
+    >>> def deuteranopia_transform(x):
+    ...     # Your color space transformation function for deuteranopia
+    ...     pass
+    >>> colorblind_cm = _colorblind_cmap(base_colormap, deuteranopia_transform)
+    >>> print(colorblind_cm)
+    """
+    ctab = get_ctab(cmap)  # get the colormap as a color table in sRGB
+    ctab_cb = c_space_transf(ctab)
+    return ListedColormap(np.clip(ctab_cb, 0, 1))
+
+def colorblind_vision(
+    cmap: Union[str, List[str], List[Colormap]],
+    figsize: Optional[Tuple[int, int]] = None,
+    n_colors: int = 10,
+    facecolor: str = "black"
+) -> plt.Figure:
+    """
+    Generate a visualization of colorblind-friendly colormaps.
+
+    Parameters
+    ----------
+    cmap : str, list of str, or list of plt.Colormap
+        The base colormap(s) or list of colormaps to visualize.
+    figsize : tuple of int, optional
+        The size of the generated figure (width, height).
+    n_colors : int, optional (default=10)
+        The number of colors to include in the colorblind visualization.
+    facecolor : {'black', 'white'}, optional (default='black')
+        The facecolor for the generated figure.
+
+    Returns
+    -------
+    plt.Figure
+        A Matplotlib figure showing colorblind-friendly versions of the specified colormap(s).
+
+    Notes
+    -----
+    This function generates a figure displaying colorblind-friendly versions of the input colormap(s).
+    It creates subplots for each colormap and visualizes the colormap with a gradient of colors.
+
+    Example
+    -------
+    >>> base_colormap = 'viridis'
+    >>> colorblind_fig = colorblind_vision(base_colormap, figsize=(8, 6))
+    >>> plt.show()
+    """
+
+    gradient = np.linspace(0, 1, n_colors)
+    gradient = np.vstack((gradient, gradient))
+
+    cmap_dic = {}
+    visible_spectrum_cmap = plt.get_cmap("gist_rainbow")
+    spectral_list, _ = _get_color_weak_cmap(color_map=visible_spectrum_cmap, n_images=0)
+    cmap_dic["visible spectrum"] = spectral_list
+
+    if isinstance(cmap, list):
+        for cm in cmap:
+            cmap_list, _ = _get_color_weak_cmap(color_map=cm, n_images=0)
+            cmap_dic[cm.name] = cmap_list
+    else:
+        cmap_list, _ = _get_color_weak_cmap(color_map=cmap, n_images=0)
+        cmap_dic[cmap.name] = cmap_list
+
+    sub_titles = (
+        ["Normal\n~95%% of pop"]
+        + ["Deuter-50%\nRG-weak, D/P: 5%% of male"]
+        + ["Prot-50%\nRG-weak, D/P: 5%% of male"]
+        + ["Deuter-100%\nRG-blind, D/P: 5%% of male"]
+        + ["Trit-100%\nBY deficient, very rare"]
+    )
+
+    nrows = len(spectral_list)
+    ncols = len(cmap_dic)
+
+    if figsize is None:
+        figsize = (10, 0.25 * nrows)
+
+    fontcolor = "white" if facecolor == "black" else "black"
+    fig, axes = plt.subplots(
+        nrows=nrows, ncols=ncols, figsize=figsize, facecolor=facecolor
+    )
+    fig.subplots_adjust(top=0.95, bottom=0.01, left=0.2, right=0.99)
+
+    cmap_list = list(cmap_dic.values())
+    cmap_name = list(cmap_dic.keys())
+
+    for i, j in itertools.product(range(nrows), range(ncols)):
+        ax = axes[i, j]
+        cmap = cmap_list[j][i]
+        ax.imshow(gradient, aspect="auto", cmap=cmap)
+        if i == 0:
+            font = {"color": fontcolor, "size": 24}
+            ax.set_title(cmap_name[j], fontdict=font)
+        if j == 0:
+            font = {"color": fontcolor, "size": 14}
+            pos = list(ax.get_position().bounds)
+            x_text = pos[0] - 0.01
+            y_text = pos[1] + pos[3] / 2.0
+            fig.text(
+                x_text, y_text, sub_titles[i], va="center", ha="right", fontdict=font
+            )
+
+    for ax in axes:
+        ax[0].set_axis_off()
+        ax[1].set_axis_off()
+    return fig
```

### Comparing `scicomap-1.0.0/src/scicomap/cmath.py` & `scicomap-1.0.1/src/scicomap/cmath.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,1080 +1,1080 @@
-"""
-Module for performing color math. Heavily based on colorspacious, viscm and ethplot.
-The main model of perceptual distance is the "CAM02-UCS" color-space
-(Uniform Colour Space version of the CIECAM02).
-
-This module uses Cartesian Lab and CIECAM02 color spaces and cylindrical
-CIELCh (hereafter LCh) and CIEJCh (hereafter JCh) color spaces which have coordinates L*, J*, C*, and h.
-The lightness coordinates L* and J* are identical to Lab and Jab. The chroma (relative saturation)
-C* and hue h (in degree h°) are simply C* = sqrt(a*^2 + b*^2) and h = atan2(b*, a*) according
-to Redness-Greenness a and Yellowness-Blueness b in their own coordinates.
-
-https://github.com/liamedeiros/ehtplot/blob/7a0567496ba9ab72f4a541d5994352bbe4eac764/ehtplot/color/cmath.py
-"""
-
-import numpy as np
-import warnings
-import matplotlib
-from colorspacious import cspace_convert
-from matplotlib.colors import Colormap, ListedColormap
-from scipy.interpolate import CubicSpline
-from typing import List, Tuple, Union, Callable, Optional
-
-
-def get_ctab(cmap: Union[Colormap, list]) -> np.ndarray:
-    """
-    Get the color table (ctab) of a matplotlib colormap.
-
-    Parameters
-    ----------
-    cmap : matplotlib.colors.Colormap or list
-        The colormap for which to retrieve the color table (ctab).
-        This can be a matplotlib Colormap or a list of color values.
-
-    Returns
-    -------
-    np.ndarray
-        An array representing the color table (ctab) as a sequence of color values.
-
-    Raises
-    ------
-    TypeError
-        If `cmap` is neither a matplotlib Colormap nor a list of color values.
-
-    Example
-    -------
-    >>> import matplotlib.pyplot as plt
-    >>> cmap = plt.get_cmap("viridis")
-    >>> ctab = get_ctab(cmap)
-    >>> print(ctab)
-    """
-    if isinstance(cmap, Colormap):
-        return np.array([cmap(v) for v in np.linspace(0, 1, cmap.N)])
-    elif isinstance(cmap, list):
-        return np.array(cmap)
-    else:
-        TypeError("`cmap` is neither a matplotlib Colormap nor a list of str/uples")
-
-
-
-def max_chroma(
-    Jp: Union[float, np.ndarray], 
-    hp: Union[float, np.ndarray], 
-    Cpmin: float = 0.0, 
-    Cpmax: Union[float, str] = "auto", 
-    eps: float = 1024 * np.finfo(np.float).eps, 
-    clip: bool = True
-) -> Union[float, np.ndarray]:
-    """
-    Calculate the maximum chroma (Cp) for a given lightness (Jp) and hue (hp) in the CAM02-UCS color space.
-
-    Parameters
-    ----------
-    Jp : float or np.ndarray
-        Lightness parameter (range: [0, 100]).
-    hp : float or np.ndarray
-        Hue angle in degrees (range: [0, 360]).
-    Cpmin : float, optional (default=0.0)
-        Minimum allowable chroma value (range: [0, Cpmax]).
-    Cpmax : float or str, optional (default="auto")
-        Maximum allowable chroma value (range: [Cpmin, sqrt(100*Jp)]).
-        If set to "auto", it will be calculated based on Jp.
-    eps : float, optional (default=1024 * np.finfo(np.float).eps)
-        A small value used to handle numerical precision issues.
-    clip : bool, optional (default=True)
-        If True, clip Jp values to the valid range before calculation.
-
-    Returns
-    -------
-    float or np.ndarray
-        Maximum chroma (Cp) value(s) corresponding to the input Jp and hp.
-
-    Raises
-    ------
-    ValueError
-        If Jp is out of range.
-    ArithmeticError
-        If the function does not fully converge.
-
-    Example
-    -------
-    >>> Jp = 70
-    >>> hp = 30
-    >>> Cp = max_chroma(Jp, hp)
-    >>> print(Cp)
-    """
-    Jpmin = 5.54015251457561e-22
-    Jpmaxv = 98.98016
-    Jpmax = 99.99871678107648
-
-    if clip:
-        Jp = np.clip(Jp, Jpmin, min(Jpmaxv, Jpmax))
-
-    if np.any(Jp < Jpmin) or np.any(Jp > Jpmax):
-        raise ValueError("J' out of range.")
-
-    if np.any(Jp > Jpmaxv):
-        raise ValueError(
-            "J' is out of range such that the corresponding sRGB colorspace "
-            + "is offset and C' == 0 is no longer a valid assumption."
-        )
-
-    if Cpmax == "auto":
-        Cpmax = np.clip(np.sqrt(100 * Jp), 0, 64)
-
-    CpU = np.full(len(Jp), Cpmax)  # np.full() works for both scalar and array
-    CpL = np.full(len(Jp), Cpmin)  # np.full() works for both scalar and array
-
-    for i in range(64):
-        Cp = 0.5 * (CpU + CpL)
-
-        # Fix when we hit machine precision
-        need_fix = Cp == CpU
-        Cp[need_fix] = CpL[need_fix]
-
-        Jpapbp = np.stack([Jp, Cp * np.cos(hp), Cp * np.sin(hp)], axis=-1)
-        sRGB = transform(Jpapbp, inverse=True)
-        edge = 2.0 * np.amax(abs(sRGB - 0.5), -1)
-
-        if 1.0 - eps <= np.min(edge) and np.max(edge) <= 1.0:
-            break
-
-        I = edge >= 1.0
-        CpU[I] = Cp[I]
-        CpL[~I] = Cp[~I]
-    else:
-        raise ArithmeticError("WARNING: max_chroma() has not fully converged")
-
-    return Cp
-
-
-def transform(
-    ctab: np.ndarray,
-    src: str = "sRGB1",
-    dst: str = "CAM02-UCS",
-    inverse: bool = False
-) -> np.ndarray:
-    """
-    Transform a color table from one color space to another.
-
-    Parameters
-    ----------
-    ctab : np.ndarray
-        A color table in the source color space.
-    src : str, optional (default="sRGB1")
-        The source color space (e.g., "sRGB1", "CAM02-UCS").
-    dst : str, optional (default="CAM02-UCS")
-        The destination color space (e.g., "sRGB1", "CAM02-UCS").
-    inverse : bool, optional (default=False)
-        If True, perform an inverse color space transformation.
-
-    Returns
-    -------
-    np.ndarray
-        A color table in the destination color space.
-
-    Example
-    -------
-    >>> import numpy as np
-    >>> ctab = np.array([[0.5, 0.2, 0.1], [0.3, 0.6, 0.9]])
-    >>> transformed_ctab = transform(ctab, src="sRGB1", dst="CAM02-UCS")
-    >>> print(transformed_ctab)
-    """
-    out = ctab.copy()
-    if not inverse:
-        out[:, :3] = cspace_convert(out[:, :3], src, dst)
-    else:
-        out[:, :3] = cspace_convert(out[:, :3], dst, src)
-    return out
-
-
-def interp(
-    x: float,
-    xp: np.ndarray,
-    yp: np.ndarray
-) -> float:
-    """
-    One-dimensional linear interpolation.
-
-    Parameters
-    ----------
-    x : float
-        The x-coordinate at which to interpolate.
-    xp : np.ndarray
-        1-D array of x-coordinates of data points.
-    yp : np.ndarray
-        1-D array of y-coordinates of data points.
-
-    Returns
-    -------
-    float
-        The interpolated value at x.
-
-    Notes
-    -----
-    This function performs linear interpolation between data points defined by
-    (xp, yp). It supports both increasing and decreasing xp arrays.
-
-    Example
-    -------
-    >>> import numpy as np
-    >>> x = 3.5
-    >>> xp = np.array([1.0, 2.0, 4.0, 5.0])
-    >>> yp = np.array([0.0, 1.0, 2.0, 3.0])
-    >>> interpolated_value = interp(x, xp, yp)
-    >>> print(interpolated_value)
-    1.5
-    """
-    if xp[0] < xp[-1]:
-        return np.interp(x, xp, yp)
-    else:
-        return np.interp(x, np.flip(xp, 0), np.flip(yp, 0))
-
-
-def extrema(a: np.ndarray) -> np.ndarray:
-    """
-    Find the indices of local extrema in a 1-D array.
-
-    Parameters
-    ----------
-    a : np.ndarray
-        1-D array in which to find local extrema.
-
-    Returns
-    -------
-    np.ndarray
-        Indices of local extrema.
-
-    Notes
-    -----
-    This function finds the indices of local extrema (maxima or minima) in the
-    input array `a`. It returns an array of indices corresponding to the local
-    extrema points.
-
-    An extremum point is detected if the product of the differences between
-    the point, the previous point, and the next point in `a` is less than or
-    equal to zero.
-
-    Example
-    -------
-    >>> import numpy as np
-    >>> a = np.array([1, 3, 7, 1, 2, 6, 2, 9])
-    >>> extrema_indices = extrema(a)
-    >>> print(extrema_indices)
-    [2 3 5 6 7]
-    """
-    da = a[1:] - a[:-1]
-    xa = da[1:] * da[:-1]
-    return np.argwhere(xa <= 0.0)[:, 0] + 1
-
-
-def classify(Jpapbp: np.ndarray) -> str:
-    """
-    Classify a colormap based on its appearance in the Jpapbp color space.
-
-    Parameters
-    ----------
-    Jpapbp : np.ndarray
-        Array of colors in the Jpapbp color space.
-
-    Returns
-    -------
-    str
-        A string representing the colormap classification:
-        - 'circular-div' for circular and diverging colormaps.
-        - 'circular-flat' for circular and flat colormaps.
-        - 'sequential' for sequential colormaps.
-        - 'divergent' for diverging colormaps.
-        - 'asym_div' for asymmetric diverging colormaps.
-        - 'multiseq' for multi-sequential colormaps.
-        - 'unknown' for unknown or unclassified colormaps.
-
-    Notes
-    -----
-    This function classifies a colormap based on its appearance in the Jpapbp
-    color space. The classification is determined by the number and positions
-    of extrema in the luminance channel (J) of the colormap.
-
-    Example
-    -------
-    >>> import numpy as np
-    >>> Jpapbp = np.array([[50, 10, 20], [40, 15, 25], [60, 5, 10]])
-    >>> colormap_class = classify(Jpapbp)
-    >>> print(colormap_class)
-    'sequential'
-    """
-
-    N = Jpapbp.shape[0]
-    large_diff_lum = Jpapbp[:, 0].max() - Jpapbp[:, 0].min() > 0.5
-    first_and_last_simeq = (
-        sum(abs(np.floor(Jpapbp[0, ...]) - np.floor(Jpapbp[-1, ...]))) < 4
-    )
-
-    # some of the cmcrameri colormaps have kind of a small hook at the end of the array
-    # artifact increasing the number of extrema by +1. A rough fix is not considering the
-    # beginning  and the end of the cmap
-    x = extrema(Jpapbp[10:-10, 0])
-    x += 10
-
-    if (len(x) == 1 or large_diff_lum) and first_and_last_simeq:
-        return "circular-div"
-    elif len(x) != 1 and first_and_last_simeq:
-        return "circular-flat"
-    elif len(x) == 0:
-        return "sequential"
-    # strictly, the extremum should be at the middle element set([(N + 1) // 2 - 1, N // 2]):
-    # cmcrameri uses another parametrization and is not perfectly symmetric
-    # in the Jc'h space
-    elif len(x) == 1 and x[0] in np.arange((N + 1) // 2 - 5, N // 2 + 5, 1):
-        return "divergent"
-    elif len(x) == 1 and x[0] not in np.arange((N + 1) // 2 - 5, N // 2 + 5, 1):
-        return "asym_div"
-    elif len(x) == 2 and (x[1] == x[0] + 1):
-        return "multiseq"
-    else:
-        return "unknown"
-
-
-def uniformize(Jpapbp: np.ndarray, JpL: float = None, JpR: float = None,
-               Jplower: float = None, Jpupper: float = None) -> np.ndarray:
-    """
-    Uniformize a colormap in the Jpapbp color space, linear in lightness J'
-
-    Parameters
-    ----------
-    Jpapbp : np.ndarray
-        Array of colors in the Jpapbp color space.
-    JpL : float, optional
-        Left luminance boundary for uniformization.
-    JpR : float, optional
-        Right luminance boundary for uniformization.
-    Jplower : float, optional
-        Lower luminance limit for uniformization.
-    Jpupper : float, optional
-        Upper luminance limit for uniformization.
-
-    Returns
-    -------
-    np.ndarray
-        The uniformized colormap in the Jpapbp color space.
-
-    Notes
-    -----
-    This function uniformizes a colormap by linearly interpolating between
-    specified luminance values (JpL and JpR) in the Jpapbp color space. You
-    can optionally provide lower (Jplower) and upper (Jpupper) luminance
-    limits to restrict the uniformization range.
-
-    Example
-    -------
-    >>> import numpy as np
-    >>> Jpapbp = np.array([[50, 10, 20], [40, 15, 25], [60, 5, 10]])
-    >>> JpL = 40
-    >>> JpR = 60
-    >>> uniformized_cmap = uniformize(Jpapbp, JpL, JpR)
-    >>> print(uniformized_cmap)
-    array([[40. , 10. , 20. ],
-           [50. , 12.5, 22.5],
-           [60. , 15. , 25. ]])
-    """
-    if JpL is None:
-        JpL = Jpapbp[0, 0]
-    if JpR is None:
-        JpR = Jpapbp[-1, 0]
-
-    if Jplower is not None:
-        JpL, JpR = max(JpL, Jplower), max(JpR, Jplower)
-    if Jpupper is not None:
-        JpL, JpR = min(JpL, Jpupper), min(JpR, Jpupper)
-
-    out = Jpapbp.copy()
-    out[:, 0] = np.linspace(JpL, JpR, out.shape[0])
-    out[:, 1] = interp(out[:, 0], Jpapbp[:, 0], Jpapbp[:, 1])
-    out[:, 2] = interp(out[:, 0], Jpapbp[:, 0], Jpapbp[:, 2])
-    return out
-
-
-def factor(
-    Cp: np.ndarray,
-    softening: float = 1.0,
-    bitonic: bool = True,
-    diffuse: bool = True,
-    CpL: float = None,
-    CpR: float = None,
-    verbose: bool = False,
-    diverging: bool = False,
-) -> np.ndarray:
-    """
-    Compute the factor required to perform several chroma operations.
-
-    Parameters
-    ----------
-    Cp : np.ndarray
-        Array of chroma values.
-    softening : float, optional
-        Softening factor applied to the chroma values.
-    bitonic : bool, optional
-        If True, enforce bitonicity for non-diverging chroma values.
-    diffuse : bool, optional
-        If True, apply diffusion to the chroma values.
-    CpL : float, optional
-        Left chroma boundary.
-    CpR : float, optional
-        Right chroma boundary.
-    verbose : bool, optional
-        If True, print verbose messages during computation.
-    diverging : bool, optional
-        If True, consider the chroma values as diverging.
-
-    Returns
-    -------
-    np.ndarray
-        The computed factor for chroma operations.
-
-    Notes
-    -----
-    This function computes a factor required for performing various chroma
-    operations. It can enforce bitonicity for non-diverging chroma values and
-    apply diffusion. You can specify left (CpL) and right (CpR) chroma
-    boundaries. The softening factor (softening) smoothens the chroma values.
-
-    Example
-    -------
-    >>> import numpy as np
-    >>> Cp = np.array([2.0, 5.0, 8.0, 5.0, 2.0])
-    >>> factor_values = factor(Cp, softening=0.5, bitonic=True, diffuse=False)
-    >>> print(factor_values)
-    array([0.72727273, 0.5       , 0.27272727, 0.5       , 0.72727273])
-    """
-    S = Cp + softening
-    s = S.copy()
-
-    N = len(Cp)
-    H = N // 2
-    m = np.minimum(s[:H], np.flip(s[-H:]))
-
-    # Bitonic only for non diverging
-    if bitonic and (not diverging):  # force half of Cp increase monotonically
-        if m[H - 1] > s[H]:
-            m[H - 1] = s[H]
-            if verbose:
-                print("Enforce bitonic at {}".format(s[H]))
-        for i in range(H - 1, 0, -1):
-            if m[i - 1] > m[i]:
-                m[i - 1] = m[i]
-                if verbose:
-                    print("Enforce bitonic at {}".format(m[i]))
-
-    s[:+H] = m
-    s[-H:] = np.flip(m)
-
-    if CpL is not None:
-        s[0] = CpL + softening
-    if CpR is not None:
-        s[-1] = CpR + softening
-
-    if diffuse:  # diffuse s using forward Euler
-        for i in range(N):
-            s[1:-1] += 0.5 * (s[2:] + s[:-2] - 2.0 * s[1:-1])
-
-    return s / S
-
-
-def symmetrize(Jpapbp: np.ndarray, **kwargs) -> np.ndarray:
-    """
-    Make a sequential colormap symmetric in chroma C'.
-
-    Parameters
-    ----------
-    Jpapbp : np.ndarray
-        Array of Jpapbp values.
-
-    Returns
-    -------
-    np.ndarray
-        The symmetric colormap in chroma C'.
-
-    Other Parameters
-    ----------------
-    **kwargs
-        Additional keyword arguments to pass to the `factor` function.
-
-    Notes
-    -----
-    This function makes a sequential colormap symmetric in chroma C'.
-    It uses the `factor` function to adjust the chroma values.
-
-    Example
-    -------
-    >>> import numpy as np
-    >>> Jpapbp = np.array([[40.0, 20.0, 10.0], [60.0, 30.0, 15.0]])
-    >>> symmetric_colormap = symmetrize(Jpapbp, softening=0.2, bitonic=True, diffuse=True)
-    >>> print(symmetric_colormap)
-    array([[40.        , 20.        , 10.        ],
-           [60.        , 30.        , 15.        ]])
-    """
-    out = Jpapbp.copy()
-    Jp = out[:, 0]
-    Cp = np.sqrt(out[:, 1] * out[:, 1] + out[:, 2] * out[:, 2])
-
-    f = factor(Cp, **kwargs)
-    out[:, 1] *= f
-    out[:, 2] *= f
-    return out
-
-
-def adjust_sequential(
-    Jpapbp: np.ndarray, roundup: float = None, bi_seq: bool = False
-) -> np.ndarray:
-    """
-    Adjust a sequential colormap in chroma C' and optionally create a bidirectional sequential colormap.
-
-    Parameters
-    ----------
-    Jpapbp : np.ndarray
-        Array of Jpapbp values.
-
-    roundup : float, optional
-        Value to round down the lower chroma bound to. If provided, the lower chroma bound will be rounded up to the nearest multiple of `roundup`. Default is None.
-
-    bi_seq : bool, optional
-        If True, create a bidirectional sequential colormap by adjusting two segments of the input colormap. Default is False.
-
-    Returns
-    -------
-    np.ndarray
-        The adjusted sequential colormap in chroma C'.
-
-    Notes
-    -----
-    This function adjusts a sequential colormap in chroma C' by optionally rounding down the lower chroma bound and creating a bidirectional sequential colormap.
-
-    Example
-    -------
-    >>> import numpy as np
-    >>> Jpapbp = np.array([[40.0, 20.0, 10.0], [60.0, 30.0, 15.0]])
-    >>> adjusted_colormap = adjust_sequential(Jpapbp, roundup=0.1, bi_seq=True)
-    >>> print(adjusted_colormap)
-    array([[40. , 20. , 10. ],
-           [60. , 30. , 15. ],
-           [40.1, 20. , 10. ],
-           [59.9, 30. , 15. ]])
-    """
-
-    if bi_seq:
-        x_boundary = extrema(Jpapbp[:, 0])[0]
-        Jpapbp1 = Jpapbp[: x_boundary + 1, ...].copy()
-        Jpapbp2 = Jpapbp[x_boundary + 1 :, ...].copy()
-        Jp = Jpapbp1[:, 0]
-        Jplower = min(Jp[0], Jp[-1])
-        if roundup is not None:
-            Jplower = np.ceil(Jplower / roundup) * roundup
-        Jpapbp1 = uniformize(Jpapbp1, Jplower=Jplower)
-        Jp = Jpapbp2[:, 0]
-        Jplower = min(Jp[0], Jp[-1])
-        if roundup is not None:
-            Jplower = np.ceil(Jplower / roundup) * roundup
-        Jpapbp2 = uniformize(Jpapbp2, Jplower=Jplower)
-        return np.append(Jpapbp1, Jpapbp2, axis=0)
-    else:
-        Jp = Jpapbp[:, 0]
-        Jplower = min(Jp[0], Jp[-1])
-        if roundup is not None:
-            Jplower = np.ceil(Jplower / roundup) * roundup
-
-        return uniformize(Jpapbp, Jplower=Jplower)
-
-
-def adjust_circular_flat(Jpapbp: np.ndarray) -> np.ndarray:
-    """
-    Adjust a flat circular colormap, making the lightness constant.
-
-    Parameters
-    ----------
-    Jpapbp : np.ndarray
-        Array of Jpapbp values.
-
-    Returns
-    -------
-    np.ndarray
-        The adjusted colormap with constant lightness.
-
-    Notes
-    -----
-    This function adjusts a flat circular colormap by making the lightness constant.
-
-    Example
-    -------
-    >>> import numpy as np
-    >>> Jpapbp = np.array([[50.0, 20.0, 10.0], [60.0, 30.0, 15.0]])
-    >>> adjusted_colormap = adjust_circular_flat(Jpapbp)
-    >>> print(adjusted_colormap)
-    array([[55., 20., 10.],
-           [55., 30., 15.]])
-    """
-    out = Jpapbp.copy()
-    Jp = out[:, 0].ravel()
-    out[:, 0] = np.ones_like(Jp) * np.nanmean(Jp)
-    return out
-
-
-def adjust_circular(Jpapbp: np.ndarray, roundup: float = None) -> np.ndarray:
-    """
-    Adjust a circular colormap.
-
-    This function adjusts a circular colormap by making modifications based on the given parameters.
-
-    Parameters
-    ----------
-    Jpapbp : np.ndarray
-        Array of Jpapbp values.
-    roundup : float, optional
-        Value to round Jplower, by default None.
-
-    Returns
-    -------
-    np.ndarray
-        The adjusted colormap.
-
-    Notes
-    -----
-    This function adjusts a circular colormap based on the parameters provided.
-
-    Example
-    -------
-    >>> import numpy as np
-    >>> Jpapbp = np.array([[50.0, 20.0, 10.0], [60.0, 30.0, 15.0]])
-    >>> adjusted_colormap = adjust_circular(Jpapbp, roundup=5.0)
-    >>> print(adjusted_colormap)
-    array([[55., 20., 10.],
-           [60., 30., 15.]])
-    """
-    Jp = Jpapbp[:, 0]
-    x_extr = extrema(Jp)
-    h = x_extr[0]
-    H = h + 1
-    N = Jpapbp.shape[0]
-    # h = (N + 1) // 2 - 1  # == H-1 if even; == H if odd
-    # H = N // 2
-
-    if Jp[1] > Jp[0]:  # hill
-        Jplower = max(Jp[0], Jp[-1])
-        Jpupper = min(Jp[h], Jp[H])
-    else:  # valley
-        Jplower = max(Jp[h], Jp[H])
-        Jpupper = min(Jp[0], Jp[-1])
-    if roundup is not None:
-        Jplower = np.ceil(Jplower / roundup) * roundup
-
-    L = uniformize(Jpapbp[: h + 1, :], Jplower=Jplower, Jpupper=Jpupper)
-    R = uniformize(Jpapbp[H:, :], Jplower=Jplower, Jpupper=Jpupper)
-    return np.append(L, R[N % 2 :, :], axis=0)
-
-
-def adjust_divergent(
-    Jpapbp: np.ndarray,
-    roundup: float = None,
-    circular: bool = False,
-    symmetric: bool = True
-) -> np.ndarray:
-    """
-    Adjust a divergent colormap.
-
-    This function adjusts a divergent colormap by making modifications based on the given parameters.
-
-    Parameters
-    ----------
-    Jpapbp : np.ndarray
-        Array of Jpapbp values.
-    roundup : float, optional
-        Value to round Jplower, by default None.
-    circular : bool, optional
-        Whether to make the colormap circular, by default False.
-    symmetric : bool, optional
-        Whether to make the colormap symmetric, by default True.
-
-    Returns
-    -------
-    np.ndarray
-        The adjusted colormap.
-
-    Notes
-    -----
-    This function adjusts a divergent colormap based on the parameters provided.
-
-    Example
-    -------
-    >>> import numpy as np
-    >>> Jpapbp = np.array([[50.0, 20.0, 10.0], [60.0, 30.0, 15.0]])
-    >>> adjusted_colormap = adjust_divergent(Jpapbp, roundup=5.0, circular=True, symmetric=True)
-    >>> print(adjusted_colormap)
-    array([[55., 20., 10.],
-           [60., 30., 15.]])
-    """
-    Jp = Jpapbp[:, 0]
-    out = Jpapbp.copy()
-    x_extr = extrema(Jp)
-    h = x_extr[0]
-    H = h + 1
-    N = Jpapbp.shape[0]
-    # h = (N + 1) // 2 - 1  # == H-1 if even; == H if odd
-    # H = N // 2
-
-    if Jp[1] > Jp[0] and symmetric:  # hill
-        Jplower = max(Jp[0], Jp[-1])
-        Jpupper = min(Jp[h], Jp[H])
-    elif Jp[1] > Jp[0] and not symmetric:  # hill
-        Jplower = Jp[0]
-        Jpupper = Jp[h]
-    elif Jp[1] < Jp[0] and symmetric:  # valley
-        Jplower = max(Jp[h], Jp[H])
-        Jpupper = min(Jp[0], Jp[-1])
-    else:
-        Jplower = Jp[h]
-        Jpupper = Jp[-1]
-    if roundup is not None:
-        Jplower = np.ceil(Jplower / roundup) * roundup
-
-    L = uniformize(Jpapbp[: h + 1, :], Jplower=Jplower, Jpupper=Jpupper)
-    R = uniformize(Jpapbp[H:, :], Jplower=Jplower, Jpupper=Jpupper)
-    Jpapbp_unif = np.append(L, R[N % 2 :, :], axis=0)
-
-    if circular:
-        theta = 2 * np.pi * np.linspace(0, 1, out.shape[0])
-        out[0, 1:3] = out[-1, 1:3]
-        cs = CubicSpline(theta, out[:, 1:3], bc_type="periodic")
-        Jpapbp_unif[:, 1:3] = cs(theta)
-    return Jpapbp_unif
-
-
-def uniformize_cmap(
-    cmap: ListedColormap,
-    name: str = "new_cmap",
-    lift: float = None,
-    uniformized: bool = False
-) -> Tuple[ListedColormap, bool]:
-    """
-    Uniformize a colormap.
-
-    This function uniformizes a given colormap if it's not already uniformized.
-
-    Parameters
-    ----------
-    cmap : ListedColormap
-        The input colormap to be uniformized.
-    name : str, optional
-        The name of the new colormap, by default "new_cmap".
-    lift : float, optional
-        Value to round Jplower, by default None.
-    uniformized : bool, optional
-        Indicates whether the colormap is already uniformized, by default False.
-
-    Returns
-    -------
-    Tuple[ListedColormap, bool]
-        A tuple containing the uniformized colormap and a boolean indicating if
-        the colormap was uniformized.
-
-    Notes
-    -----
-    This function uniformizes a colormap by analyzing its color table and transforming
-    it into a uniformized version based on its color characteristics.
-
-    Example
-    -------
-    >>> import matplotlib.pyplot as plt
-    >>> from matplotlib.colors import ListedColormap
-    >>> from my_module import uniformize_cmap
-    >>> # Create a sample colormap
-    >>> original_cmap = plt.get_cmap("viridis")
-    >>> uniformized_cmap, was_uniformized = uniformize_cmap(original_cmap, name="uniform_viridis", lift=5.0)
-    >>> if was_uniformized:
-    ...     print("Colormap was uniformized.")
-    ... else:
-    ...     print("Colormap was already uniformized.")
-    >>> # Now you can use the uniformized_cmap for plotting.
-
-    """
-    # if not uniformized yet, uniformize the cmap
-    # else do nothing
-    if not uniformized:
-        # get the color table
-        ctab = get_ctab(cmap)
-        # transform to Jpapbp
-        t_ctab = transform(ctab)
-        # find if sequential or divergent or unknown
-        cmap_type = classify(t_ctab)
-        if cmap_type == "divergent":
-            lin_ctab = adjust_divergent(t_ctab, roundup=lift)
-        elif cmap_type == "asym_div":
-            lin_ctab = adjust_divergent(t_ctab, roundup=lift, symmetric=False)
-        elif cmap_type == "sequential":
-            lin_ctab = adjust_sequential(t_ctab, roundup=lift)
-        elif cmap_type == "multiseq":
-            lin_ctab = adjust_sequential(t_ctab, roundup=lift, bi_seq=True)
-        elif cmap_type == "circular-flat":
-            lin_ctab = adjust_circular_flat(t_ctab)
-        elif cmap_type == "circular-div":
-            lin_ctab = adjust_divergent(t_ctab, roundup=lift, circular=True)
-        else:
-            warnings.warn(
-                "The colormap {} type is unknown (not recognized as sequential or divergent)\n"
-                "Not uniformized".format(name)
-            )
-            lin_ctab = t_ctab
-
-        lin_cmap = transform(ctab=lin_ctab, inverse=True)
-
-        return ListedColormap(np.clip(lin_cmap, 0, 1), name=name), True
-    else:
-        return cmap, True
-
-
-def symmetrize_cmap(
-    cmap: ListedColormap,
-    name: str = "new_cmap",
-    bitonic: bool = True,
-    diffuse: bool = True
-) -> ListedColormap:
-    """
-    Symmetrize a colormap.
-
-    This function symmetrizes a given colormap based on its color characteristics.
-
-    Parameters
-    ----------
-    cmap : ListedColormap
-        The input colormap to be symmetrized.
-    name : str, optional
-        The name of the new colormap, by default "new_cmap".
-    bitonic : bool, optional
-        If True, ensures that half of Cp increases monotonically, by default True.
-    diffuse : bool, optional
-        If True, diffuses the colormap, by default True.
-
-    Returns
-    -------
-    ListedColormap
-        The symmetrized colormap.
-
-    Notes
-    -----
-    This function symmetrizes a colormap by analyzing its color table, transforming
-    it into a symmetrical version based on its color characteristics, and returning
-    it as a matplotlib ListedColormap.
-
-    Example
-    -------
-    >>> import matplotlib.pyplot as plt
-    >>> from matplotlib.colors import ListedColormap
-    >>> from my_module import symmetrize_cmap
-    >>> # Create a sample colormap
-    >>> original_cmap = plt.get_cmap("coolwarm")
-    >>> symmetrized_cmap = symmetrize_cmap(original_cmap, name="symmetric_coolwarm", bitonic=True, diffuse=True)
-    >>> # Now you can use the symmetrized_cmap for plotting.
-
-    """
-    # get the color table
-    ctab = get_ctab(cmap)
-    # transform to Jpapbp
-    t_ctab = transform(ctab)
-    # find if sequential or divergent or unknown
-    cmap_type = classify(t_ctab)
-    diverging = True if cmap_type == "divergent" else False
-    lin_ctab = symmetrize(t_ctab, bitonic=bitonic, diffuse=diffuse, diverging=diverging)
-    # get back a matplotlib cmap object
-    s_cmap = transform(ctab=lin_ctab, inverse=True)
-    return ListedColormap(np.clip(s_cmap, 0, 1), name=name)
-
-
-def unif_sym_cmap(
-    cmap: ListedColormap,
-    name: str = "new_cmap",
-    lift: float = None,
-    uniformized: bool = False,
-    bitonic: bool = True,
-    diffuse: bool = True
-) -> tuple[ListedColormap, bool]:
-    """
-    Uniformize and symmetrize a colormap (perceptually homogeneous).
-
-    This function performs both uniformization and symmetrization of a given colormap
-    based on its color characteristics (symmetric saturation for even perception of both sides of the cmap).
-
-    Parameters
-    ----------
-    cmap : ListedColormap
-        The input colormap to be uniformized and symmetrized.
-    name : str, optional
-        The name of the new colormap, by default "new_cmap".
-    lift : float, optional
-        A parameter controlling the degree of uniformization, by default None.
-    uniformized : bool, optional
-        If True, skip uniformization step if the colormap is already uniformized,
-        by default False.
-    bitonic : bool, optional
-        If True, ensures that half of Cp increases monotonically, by default True.
-    diffuse : bool, optional
-        If True, diffuses the colormap, by default True.
-
-    Returns
-    -------
-    tuple[ListedColormap, bool]
-        A tuple containing the uniformized and symmetrized colormap, and a boolean
-        indicating whether uniformization was performed.
-
-    Notes
-    -----
-    This function first checks if uniformization is needed based on the `uniformized`
-    parameter. If uniformization is performed, the colormap is transformed into a
-    uniformized version based on its color characteristics. Then, symmetrization is
-    applied to the uniformized colormap. The final colormap is returned along with
-    a boolean indicating whether uniformization was performed.
-
-    Example
-    -------
-    >>> import matplotlib.pyplot as plt
-    >>> from matplotlib.colors import ListedColormap
-    >>> from my_module import unif_sym_cmap
-    >>> # Create a sample colormap
-    >>> original_cmap = plt.get_cmap("coolwarm")
-    >>> uniformized_symmetric_cmap, uniformized = unif_sym_cmap(original_cmap, name="uni_sym_coolwarm", lift=0.1)
-    >>> # Now you can use the uniformized_symmetric_cmap for plotting.
-
-    """
-    uni_cmap, uniformized = uniformize_cmap(
-        cmap, name=name, lift=lift, uniformized=uniformized
-    )
-    return (
-        symmetrize_cmap(uni_cmap, name=name, bitonic=bitonic, diffuse=diffuse),
-        uniformized,
-    )
-
-
-def _ax_cylinder_JCh(
-    ax: matplotlib.axes.Axes,
-    cmap: Colormap,
-    title: str
-) -> matplotlib.axes.Axes:
-    """
-    Plot Jp, Cp, and hp coordinates in a cylindrical representation for a colormap.
-
-    This function visualizes the J' (lightness), C' (chroma), and h' (hue) coordinates
-    of a colormap in a cylindrical representation.
-
-    Parameters
-    ----------
-    ax : matplotlib.axes._axes.Axes
-        The matplotlib axes object to plot on.
-    cmap : matplotlib.colors.Colormap
-        The input colormap to visualize.
-    title : str
-        The title of the plot.
-
-    Returns
-    -------
-    matplotlib.axes._axes.Axes
-        The matplotlib axes object containing the plotted data.
-
-    Notes
-    -----
-    This function takes a colormap and extracts its J', C', and h' coordinates in
-    the CAM02-UCS color space. It then plots these coordinates in a cylindrical
-    representation, where J' and C' are shown on one axis, and h' on another axis.
-
-    Example
-    -------
-    >>> import matplotlib.pyplot as plt
-    >>> from matplotlib.colors import ListedColormap
-    >>> from my_module import _ax_cylinder_JCh
-    >>> # Create a sample colormap
-    >>> cmap = plt.get_cmap("coolwarm")
-    >>> fig, ax = plt.subplots()
-    >>> _ax_cylinder_JCh(ax, cmap, title="Cylindrical JCh Coordinates")
-
-    """
-    ctab = get_ctab(cmap)  # get the colormap as a color table in sRGB
-    Jpapbp = transform(ctab)  # transform color table into CAM02-UCS colorspace
-
-    Jp = Jpapbp[:, 0]
-    ap = Jpapbp[:, 1]
-    bp = Jpapbp[:, 2]
-
-    Cp = np.sqrt(ap * ap + bp * bp)
-    hp = np.arctan2(bp, ap) * 180 / np.pi
-    v = np.linspace(0.0, 1.0, len(Jp))
-
-    ax.set_title(title + "\nJpCphp coord. (cyl)", fontsize=14)
-    ax.set_xlabel("Value", fontsize=14)
-
-    axtx = ax.twinx()
-    ax.set_ylim(0, 100)
-    ax.set_ylabel("J' & C' (0-100)", fontsize=14)
-    axtx.set_ylim(-180, 180)
-    axtx.set_ylabel("h' (degrees)", fontsize=14)
-
-    ax.scatter(v, Jp, color=ctab, label="J' (lightness)")
-    ax.plot(v, Cp, c="k", linestyle="--", label="C' (chroma)")
-    axtx.scatter(v[::15], hp[::15], s=10, c="k")
-    ax.scatter([], [], s=10, c="k", label="h' (hue)")
-    ax.legend(loc="best")
-    return ax
-
-
-def _ax_scatter_Jpapbp(
-    ax: matplotlib.axes.Axes,
-    cmap: Colormap,
-    title: str
-) -> matplotlib.axes.Axes:
-    """
-    Create a scatter plot in 3D to visualize Jpapbp coordinates of a colormap.
-
-    This function creates a 3D scatter plot to visualize the J', a', and b' coordinates
-    of a colormap in the CAM02-UCS color space.
-
-    Parameters
-    ----------
-    ax : matplotlib.axes._axes.Axes
-        The matplotlib axes object to plot on.
-    cmap : matplotlib.colors.Colormap
-        The input colormap to visualize.
-    title : str
-        The title of the plot.
-
-    Returns
-    -------
-    matplotlib.axes._axes.Axes
-        The matplotlib axes object containing the plotted data.
-
-    Notes
-    -----
-    This function takes a colormap, extracts its J', a', and b' coordinates in the
-    CAM02-UCS color space, and creates a 3D scatter plot to visualize these coordinates.
-
-    Example
-    -------
-    >>> import matplotlib.pyplot as plt
-    >>> from matplotlib.colors import ListedColormap
-    >>> from my_module import _ax_scatter_Jpapbp
-    >>> # Create a sample colormap
-    >>> cmap = plt.get_cmap("coolwarm")
-    >>> fig = plt.figure()
-    >>> ax = fig.add_subplot(111, projection='3d')
-    >>> _ax_scatter_Jpapbp(ax, cmap, title="Jpapbp Scatter Plot")
-
-    """
-    ctab = get_ctab(cmap)  # get the colormap as a color table in sRGB
-    Jpapbp = transform(ctab)  # transform color table into CAM02-UCS colorspace
-
-    # ax.plot(Jpapbp[:, 1], Jpapbp[:, 2], Jpapbp[:, 0])
-    x_dots = np.linspace(0, 1, Jpapbp.shape[0])
-    RGB_dots = cmap(x_dots)[:, :3]
-    Jpapbp_dots = transform(RGB_dots)
-    ax.scatter(
-        Jpapbp_dots[:, 1], Jpapbp_dots[:, 2], Jpapbp_dots[:, 0], c=RGB_dots[:, :], s=80
-    )
-    ax.set_xlabel("a' (green -> red)")
-    ax.set_ylabel("b' (blue -> yellow)")
-    ax.set_zlabel("J'/K (black -> white)")
-    ax.set_title(title + "\nJpapbp coord.", fontsize=14)
-    return ax
+"""
+Module for performing color math. Heavily based on colorspacious, viscm and ethplot.
+The main model of perceptual distance is the "CAM02-UCS" color-space
+(Uniform Colour Space version of the CIECAM02).
+
+This module uses Cartesian Lab and CIECAM02 color spaces and cylindrical
+CIELCh (hereafter LCh) and CIEJCh (hereafter JCh) color spaces which have coordinates L*, J*, C*, and h.
+The lightness coordinates L* and J* are identical to Lab and Jab. The chroma (relative saturation)
+C* and hue h (in degree h°) are simply C* = sqrt(a*^2 + b*^2) and h = atan2(b*, a*) according
+to Redness-Greenness a and Yellowness-Blueness b in their own coordinates.
+
+https://github.com/liamedeiros/ehtplot/blob/7a0567496ba9ab72f4a541d5994352bbe4eac764/ehtplot/color/cmath.py
+"""
+
+import numpy as np
+import warnings
+import matplotlib
+from colorspacious import cspace_convert
+from matplotlib.colors import Colormap, ListedColormap
+from scipy.interpolate import CubicSpline
+from typing import List, Tuple, Union, Callable, Optional
+
+
+def get_ctab(cmap: Union[Colormap, list]) -> np.ndarray:
+    """
+    Get the color table (ctab) of a matplotlib colormap.
+
+    Parameters
+    ----------
+    cmap : matplotlib.colors.Colormap or list
+        The colormap for which to retrieve the color table (ctab).
+        This can be a matplotlib Colormap or a list of color values.
+
+    Returns
+    -------
+    np.ndarray
+        An array representing the color table (ctab) as a sequence of color values.
+
+    Raises
+    ------
+    TypeError
+        If `cmap` is neither a matplotlib Colormap nor a list of color values.
+
+    Example
+    -------
+    >>> import matplotlib.pyplot as plt
+    >>> cmap = plt.get_cmap("viridis")
+    >>> ctab = get_ctab(cmap)
+    >>> print(ctab)
+    """
+    if isinstance(cmap, Colormap):
+        return np.array([cmap(v) for v in np.linspace(0, 1, cmap.N)])
+    elif isinstance(cmap, list):
+        return np.array(cmap)
+    else:
+        TypeError("`cmap` is neither a matplotlib Colormap nor a list of str/uples")
+
+
+
+def max_chroma(
+    Jp: Union[float, np.ndarray], 
+    hp: Union[float, np.ndarray], 
+    Cpmin: float = 0.0, 
+    Cpmax: Union[float, str] = "auto", 
+    eps: float = 1024 * np.finfo(float).eps, 
+    clip: bool = True
+) -> Union[float, np.ndarray]:
+    """
+    Calculate the maximum chroma (Cp) for a given lightness (Jp) and hue (hp) in the CAM02-UCS color space.
+
+    Parameters
+    ----------
+    Jp : float or np.ndarray
+        Lightness parameter (range: [0, 100]).
+    hp : float or np.ndarray
+        Hue angle in degrees (range: [0, 360]).
+    Cpmin : float, optional (default=0.0)
+        Minimum allowable chroma value (range: [0, Cpmax]).
+    Cpmax : float or str, optional (default="auto")
+        Maximum allowable chroma value (range: [Cpmin, sqrt(100*Jp)]).
+        If set to "auto", it will be calculated based on Jp.
+    eps : float, optional (default=1024 * np.finfo(float).eps)
+        A small value used to handle numerical precision issues.
+    clip : bool, optional (default=True)
+        If True, clip Jp values to the valid range before calculation.
+
+    Returns
+    -------
+    float or np.ndarray
+        Maximum chroma (Cp) value(s) corresponding to the input Jp and hp.
+
+    Raises
+    ------
+    ValueError
+        If Jp is out of range.
+    ArithmeticError
+        If the function does not fully converge.
+
+    Example
+    -------
+    >>> Jp = 70
+    >>> hp = 30
+    >>> Cp = max_chroma(Jp, hp)
+    >>> print(Cp)
+    """
+    Jpmin = 5.54015251457561e-22
+    Jpmaxv = 98.98016
+    Jpmax = 99.99871678107648
+
+    if clip:
+        Jp = np.clip(Jp, Jpmin, min(Jpmaxv, Jpmax))
+
+    if np.any(Jp < Jpmin) or np.any(Jp > Jpmax):
+        raise ValueError("J' out of range.")
+
+    if np.any(Jp > Jpmaxv):
+        raise ValueError(
+            "J' is out of range such that the corresponding sRGB colorspace "
+            + "is offset and C' == 0 is no longer a valid assumption."
+        )
+
+    if Cpmax == "auto":
+        Cpmax = np.clip(np.sqrt(100 * Jp), 0, 64)
+
+    CpU = np.full(len(Jp), Cpmax)  # np.full() works for both scalar and array
+    CpL = np.full(len(Jp), Cpmin)  # np.full() works for both scalar and array
+
+    for i in range(64):
+        Cp = 0.5 * (CpU + CpL)
+
+        # Fix when we hit machine precision
+        need_fix = Cp == CpU
+        Cp[need_fix] = CpL[need_fix]
+
+        Jpapbp = np.stack([Jp, Cp * np.cos(hp), Cp * np.sin(hp)], axis=-1)
+        sRGB = transform(Jpapbp, inverse=True)
+        edge = 2.0 * np.amax(abs(sRGB - 0.5), -1)
+
+        if 1.0 - eps <= np.min(edge) and np.max(edge) <= 1.0:
+            break
+
+        I = edge >= 1.0
+        CpU[I] = Cp[I]
+        CpL[~I] = Cp[~I]
+    else:
+        raise ArithmeticError("WARNING: max_chroma() has not fully converged")
+
+    return Cp
+
+
+def transform(
+    ctab: np.ndarray,
+    src: str = "sRGB1",
+    dst: str = "CAM02-UCS",
+    inverse: bool = False
+) -> np.ndarray:
+    """
+    Transform a color table from one color space to another.
+
+    Parameters
+    ----------
+    ctab : np.ndarray
+        A color table in the source color space.
+    src : str, optional (default="sRGB1")
+        The source color space (e.g., "sRGB1", "CAM02-UCS").
+    dst : str, optional (default="CAM02-UCS")
+        The destination color space (e.g., "sRGB1", "CAM02-UCS").
+    inverse : bool, optional (default=False)
+        If True, perform an inverse color space transformation.
+
+    Returns
+    -------
+    np.ndarray
+        A color table in the destination color space.
+
+    Example
+    -------
+    >>> import numpy as np
+    >>> ctab = np.array([[0.5, 0.2, 0.1], [0.3, 0.6, 0.9]])
+    >>> transformed_ctab = transform(ctab, src="sRGB1", dst="CAM02-UCS")
+    >>> print(transformed_ctab)
+    """
+    out = ctab.copy()
+    if not inverse:
+        out[:, :3] = cspace_convert(out[:, :3], src, dst)
+    else:
+        out[:, :3] = cspace_convert(out[:, :3], dst, src)
+    return out
+
+
+def interp(
+    x: float,
+    xp: np.ndarray,
+    yp: np.ndarray
+) -> float:
+    """
+    One-dimensional linear interpolation.
+
+    Parameters
+    ----------
+    x : float
+        The x-coordinate at which to interpolate.
+    xp : np.ndarray
+        1-D array of x-coordinates of data points.
+    yp : np.ndarray
+        1-D array of y-coordinates of data points.
+
+    Returns
+    -------
+    float
+        The interpolated value at x.
+
+    Notes
+    -----
+    This function performs linear interpolation between data points defined by
+    (xp, yp). It supports both increasing and decreasing xp arrays.
+
+    Example
+    -------
+    >>> import numpy as np
+    >>> x = 3.5
+    >>> xp = np.array([1.0, 2.0, 4.0, 5.0])
+    >>> yp = np.array([0.0, 1.0, 2.0, 3.0])
+    >>> interpolated_value = interp(x, xp, yp)
+    >>> print(interpolated_value)
+    1.5
+    """
+    if xp[0] < xp[-1]:
+        return np.interp(x, xp, yp)
+    else:
+        return np.interp(x, np.flip(xp, 0), np.flip(yp, 0))
+
+
+def extrema(a: np.ndarray) -> np.ndarray:
+    """
+    Find the indices of local extrema in a 1-D array.
+
+    Parameters
+    ----------
+    a : np.ndarray
+        1-D array in which to find local extrema.
+
+    Returns
+    -------
+    np.ndarray
+        Indices of local extrema.
+
+    Notes
+    -----
+    This function finds the indices of local extrema (maxima or minima) in the
+    input array `a`. It returns an array of indices corresponding to the local
+    extrema points.
+
+    An extremum point is detected if the product of the differences between
+    the point, the previous point, and the next point in `a` is less than or
+    equal to zero.
+
+    Example
+    -------
+    >>> import numpy as np
+    >>> a = np.array([1, 3, 7, 1, 2, 6, 2, 9])
+    >>> extrema_indices = extrema(a)
+    >>> print(extrema_indices)
+    [2 3 5 6 7]
+    """
+    da = a[1:] - a[:-1]
+    xa = da[1:] * da[:-1]
+    return np.argwhere(xa <= 0.0)[:, 0] + 1
+
+
+def classify(Jpapbp: np.ndarray) -> str:
+    """
+    Classify a colormap based on its appearance in the Jpapbp color space.
+
+    Parameters
+    ----------
+    Jpapbp : np.ndarray
+        Array of colors in the Jpapbp color space.
+
+    Returns
+    -------
+    str
+        A string representing the colormap classification:
+        - 'circular-div' for circular and diverging colormaps.
+        - 'circular-flat' for circular and flat colormaps.
+        - 'sequential' for sequential colormaps.
+        - 'divergent' for diverging colormaps.
+        - 'asym_div' for asymmetric diverging colormaps.
+        - 'multiseq' for multi-sequential colormaps.
+        - 'unknown' for unknown or unclassified colormaps.
+
+    Notes
+    -----
+    This function classifies a colormap based on its appearance in the Jpapbp
+    color space. The classification is determined by the number and positions
+    of extrema in the luminance channel (J) of the colormap.
+
+    Example
+    -------
+    >>> import numpy as np
+    >>> Jpapbp = np.array([[50, 10, 20], [40, 15, 25], [60, 5, 10]])
+    >>> colormap_class = classify(Jpapbp)
+    >>> print(colormap_class)
+    'sequential'
+    """
+
+    N = Jpapbp.shape[0]
+    large_diff_lum = Jpapbp[:, 0].max() - Jpapbp[:, 0].min() > 0.5
+    first_and_last_simeq = (
+        sum(abs(np.floor(Jpapbp[0, ...]) - np.floor(Jpapbp[-1, ...]))) < 4
+    )
+
+    # some of the cmcrameri colormaps have kind of a small hook at the end of the array
+    # artifact increasing the number of extrema by +1. A rough fix is not considering the
+    # beginning  and the end of the cmap
+    x = extrema(Jpapbp[10:-10, 0])
+    x += 10
+
+    if (len(x) == 1 or large_diff_lum) and first_and_last_simeq:
+        return "circular-div"
+    elif len(x) != 1 and first_and_last_simeq:
+        return "circular-flat"
+    elif len(x) == 0:
+        return "sequential"
+    # strictly, the extremum should be at the middle element set([(N + 1) // 2 - 1, N // 2]):
+    # cmcrameri uses another parametrization and is not perfectly symmetric
+    # in the Jc'h space
+    elif len(x) == 1 and x[0] in np.arange((N + 1) // 2 - 5, N // 2 + 5, 1):
+        return "divergent"
+    elif len(x) == 1 and x[0] not in np.arange((N + 1) // 2 - 5, N // 2 + 5, 1):
+        return "asym_div"
+    elif len(x) == 2 and (x[1] == x[0] + 1):
+        return "multiseq"
+    else:
+        return "unknown"
+
+
+def uniformize(Jpapbp: np.ndarray, JpL: float = None, JpR: float = None,
+               Jplower: float = None, Jpupper: float = None) -> np.ndarray:
+    """
+    Uniformize a colormap in the Jpapbp color space, linear in lightness J'
+
+    Parameters
+    ----------
+    Jpapbp : np.ndarray
+        Array of colors in the Jpapbp color space.
+    JpL : float, optional
+        Left luminance boundary for uniformization.
+    JpR : float, optional
+        Right luminance boundary for uniformization.
+    Jplower : float, optional
+        Lower luminance limit for uniformization.
+    Jpupper : float, optional
+        Upper luminance limit for uniformization.
+
+    Returns
+    -------
+    np.ndarray
+        The uniformized colormap in the Jpapbp color space.
+
+    Notes
+    -----
+    This function uniformizes a colormap by linearly interpolating between
+    specified luminance values (JpL and JpR) in the Jpapbp color space. You
+    can optionally provide lower (Jplower) and upper (Jpupper) luminance
+    limits to restrict the uniformization range.
+
+    Example
+    -------
+    >>> import numpy as np
+    >>> Jpapbp = np.array([[50, 10, 20], [40, 15, 25], [60, 5, 10]])
+    >>> JpL = 40
+    >>> JpR = 60
+    >>> uniformized_cmap = uniformize(Jpapbp, JpL, JpR)
+    >>> print(uniformized_cmap)
+    array([[40. , 10. , 20. ],
+           [50. , 12.5, 22.5],
+           [60. , 15. , 25. ]])
+    """
+    if JpL is None:
+        JpL = Jpapbp[0, 0]
+    if JpR is None:
+        JpR = Jpapbp[-1, 0]
+
+    if Jplower is not None:
+        JpL, JpR = max(JpL, Jplower), max(JpR, Jplower)
+    if Jpupper is not None:
+        JpL, JpR = min(JpL, Jpupper), min(JpR, Jpupper)
+
+    out = Jpapbp.copy()
+    out[:, 0] = np.linspace(JpL, JpR, out.shape[0])
+    out[:, 1] = interp(out[:, 0], Jpapbp[:, 0], Jpapbp[:, 1])
+    out[:, 2] = interp(out[:, 0], Jpapbp[:, 0], Jpapbp[:, 2])
+    return out
+
+
+def factor(
+    Cp: np.ndarray,
+    softening: float = 1.0,
+    bitonic: bool = True,
+    diffuse: bool = True,
+    CpL: float = None,
+    CpR: float = None,
+    verbose: bool = False,
+    diverging: bool = False,
+) -> np.ndarray:
+    """
+    Compute the factor required to perform several chroma operations.
+
+    Parameters
+    ----------
+    Cp : np.ndarray
+        Array of chroma values.
+    softening : float, optional
+        Softening factor applied to the chroma values.
+    bitonic : bool, optional
+        If True, enforce bitonicity for non-diverging chroma values.
+    diffuse : bool, optional
+        If True, apply diffusion to the chroma values.
+    CpL : float, optional
+        Left chroma boundary.
+    CpR : float, optional
+        Right chroma boundary.
+    verbose : bool, optional
+        If True, print verbose messages during computation.
+    diverging : bool, optional
+        If True, consider the chroma values as diverging.
+
+    Returns
+    -------
+    np.ndarray
+        The computed factor for chroma operations.
+
+    Notes
+    -----
+    This function computes a factor required for performing various chroma
+    operations. It can enforce bitonicity for non-diverging chroma values and
+    apply diffusion. You can specify left (CpL) and right (CpR) chroma
+    boundaries. The softening factor (softening) smoothens the chroma values.
+
+    Example
+    -------
+    >>> import numpy as np
+    >>> Cp = np.array([2.0, 5.0, 8.0, 5.0, 2.0])
+    >>> factor_values = factor(Cp, softening=0.5, bitonic=True, diffuse=False)
+    >>> print(factor_values)
+    array([0.72727273, 0.5       , 0.27272727, 0.5       , 0.72727273])
+    """
+    S = Cp + softening
+    s = S.copy()
+
+    N = len(Cp)
+    H = N // 2
+    m = np.minimum(s[:H], np.flip(s[-H:]))
+
+    # Bitonic only for non diverging
+    if bitonic and (not diverging):  # force half of Cp increase monotonically
+        if m[H - 1] > s[H]:
+            m[H - 1] = s[H]
+            if verbose:
+                print("Enforce bitonic at {}".format(s[H]))
+        for i in range(H - 1, 0, -1):
+            if m[i - 1] > m[i]:
+                m[i - 1] = m[i]
+                if verbose:
+                    print("Enforce bitonic at {}".format(m[i]))
+
+    s[:+H] = m
+    s[-H:] = np.flip(m)
+
+    if CpL is not None:
+        s[0] = CpL + softening
+    if CpR is not None:
+        s[-1] = CpR + softening
+
+    if diffuse:  # diffuse s using forward Euler
+        for i in range(N):
+            s[1:-1] += 0.5 * (s[2:] + s[:-2] - 2.0 * s[1:-1])
+
+    return s / S
+
+
+def symmetrize(Jpapbp: np.ndarray, **kwargs) -> np.ndarray:
+    """
+    Make a sequential colormap symmetric in chroma C'.
+
+    Parameters
+    ----------
+    Jpapbp : np.ndarray
+        Array of Jpapbp values.
+
+    Returns
+    -------
+    np.ndarray
+        The symmetric colormap in chroma C'.
+
+    Other Parameters
+    ----------------
+    **kwargs
+        Additional keyword arguments to pass to the `factor` function.
+
+    Notes
+    -----
+    This function makes a sequential colormap symmetric in chroma C'.
+    It uses the `factor` function to adjust the chroma values.
+
+    Example
+    -------
+    >>> import numpy as np
+    >>> Jpapbp = np.array([[40.0, 20.0, 10.0], [60.0, 30.0, 15.0]])
+    >>> symmetric_colormap = symmetrize(Jpapbp, softening=0.2, bitonic=True, diffuse=True)
+    >>> print(symmetric_colormap)
+    array([[40.        , 20.        , 10.        ],
+           [60.        , 30.        , 15.        ]])
+    """
+    out = Jpapbp.copy()
+    Jp = out[:, 0]
+    Cp = np.sqrt(out[:, 1] * out[:, 1] + out[:, 2] * out[:, 2])
+
+    f = factor(Cp, **kwargs)
+    out[:, 1] *= f
+    out[:, 2] *= f
+    return out
+
+
+def adjust_sequential(
+    Jpapbp: np.ndarray, roundup: float = None, bi_seq: bool = False
+) -> np.ndarray:
+    """
+    Adjust a sequential colormap in chroma C' and optionally create a bidirectional sequential colormap.
+
+    Parameters
+    ----------
+    Jpapbp : np.ndarray
+        Array of Jpapbp values.
+
+    roundup : float, optional
+        Value to round down the lower chroma bound to. If provided, the lower chroma bound will be rounded up to the nearest multiple of `roundup`. Default is None.
+
+    bi_seq : bool, optional
+        If True, create a bidirectional sequential colormap by adjusting two segments of the input colormap. Default is False.
+
+    Returns
+    -------
+    np.ndarray
+        The adjusted sequential colormap in chroma C'.
+
+    Notes
+    -----
+    This function adjusts a sequential colormap in chroma C' by optionally rounding down the lower chroma bound and creating a bidirectional sequential colormap.
+
+    Example
+    -------
+    >>> import numpy as np
+    >>> Jpapbp = np.array([[40.0, 20.0, 10.0], [60.0, 30.0, 15.0]])
+    >>> adjusted_colormap = adjust_sequential(Jpapbp, roundup=0.1, bi_seq=True)
+    >>> print(adjusted_colormap)
+    array([[40. , 20. , 10. ],
+           [60. , 30. , 15. ],
+           [40.1, 20. , 10. ],
+           [59.9, 30. , 15. ]])
+    """
+
+    if bi_seq:
+        x_boundary = extrema(Jpapbp[:, 0])[0]
+        Jpapbp1 = Jpapbp[: x_boundary + 1, ...].copy()
+        Jpapbp2 = Jpapbp[x_boundary + 1 :, ...].copy()
+        Jp = Jpapbp1[:, 0]
+        Jplower = min(Jp[0], Jp[-1])
+        if roundup is not None:
+            Jplower = np.ceil(Jplower / roundup) * roundup
+        Jpapbp1 = uniformize(Jpapbp1, Jplower=Jplower)
+        Jp = Jpapbp2[:, 0]
+        Jplower = min(Jp[0], Jp[-1])
+        if roundup is not None:
+            Jplower = np.ceil(Jplower / roundup) * roundup
+        Jpapbp2 = uniformize(Jpapbp2, Jplower=Jplower)
+        return np.append(Jpapbp1, Jpapbp2, axis=0)
+    else:
+        Jp = Jpapbp[:, 0]
+        Jplower = min(Jp[0], Jp[-1])
+        if roundup is not None:
+            Jplower = np.ceil(Jplower / roundup) * roundup
+
+        return uniformize(Jpapbp, Jplower=Jplower)
+
+
+def adjust_circular_flat(Jpapbp: np.ndarray) -> np.ndarray:
+    """
+    Adjust a flat circular colormap, making the lightness constant.
+
+    Parameters
+    ----------
+    Jpapbp : np.ndarray
+        Array of Jpapbp values.
+
+    Returns
+    -------
+    np.ndarray
+        The adjusted colormap with constant lightness.
+
+    Notes
+    -----
+    This function adjusts a flat circular colormap by making the lightness constant.
+
+    Example
+    -------
+    >>> import numpy as np
+    >>> Jpapbp = np.array([[50.0, 20.0, 10.0], [60.0, 30.0, 15.0]])
+    >>> adjusted_colormap = adjust_circular_flat(Jpapbp)
+    >>> print(adjusted_colormap)
+    array([[55., 20., 10.],
+           [55., 30., 15.]])
+    """
+    out = Jpapbp.copy()
+    Jp = out[:, 0].ravel()
+    out[:, 0] = np.ones_like(Jp) * np.nanmean(Jp)
+    return out
+
+
+def adjust_circular(Jpapbp: np.ndarray, roundup: float = None) -> np.ndarray:
+    """
+    Adjust a circular colormap.
+
+    This function adjusts a circular colormap by making modifications based on the given parameters.
+
+    Parameters
+    ----------
+    Jpapbp : np.ndarray
+        Array of Jpapbp values.
+    roundup : float, optional
+        Value to round Jplower, by default None.
+
+    Returns
+    -------
+    np.ndarray
+        The adjusted colormap.
+
+    Notes
+    -----
+    This function adjusts a circular colormap based on the parameters provided.
+
+    Example
+    -------
+    >>> import numpy as np
+    >>> Jpapbp = np.array([[50.0, 20.0, 10.0], [60.0, 30.0, 15.0]])
+    >>> adjusted_colormap = adjust_circular(Jpapbp, roundup=5.0)
+    >>> print(adjusted_colormap)
+    array([[55., 20., 10.],
+           [60., 30., 15.]])
+    """
+    Jp = Jpapbp[:, 0]
+    x_extr = extrema(Jp)
+    h = x_extr[0]
+    H = h + 1
+    N = Jpapbp.shape[0]
+    # h = (N + 1) // 2 - 1  # == H-1 if even; == H if odd
+    # H = N // 2
+
+    if Jp[1] > Jp[0]:  # hill
+        Jplower = max(Jp[0], Jp[-1])
+        Jpupper = min(Jp[h], Jp[H])
+    else:  # valley
+        Jplower = max(Jp[h], Jp[H])
+        Jpupper = min(Jp[0], Jp[-1])
+    if roundup is not None:
+        Jplower = np.ceil(Jplower / roundup) * roundup
+
+    L = uniformize(Jpapbp[: h + 1, :], Jplower=Jplower, Jpupper=Jpupper)
+    R = uniformize(Jpapbp[H:, :], Jplower=Jplower, Jpupper=Jpupper)
+    return np.append(L, R[N % 2 :, :], axis=0)
+
+
+def adjust_divergent(
+    Jpapbp: np.ndarray,
+    roundup: float = None,
+    circular: bool = False,
+    symmetric: bool = True
+) -> np.ndarray:
+    """
+    Adjust a divergent colormap.
+
+    This function adjusts a divergent colormap by making modifications based on the given parameters.
+
+    Parameters
+    ----------
+    Jpapbp : np.ndarray
+        Array of Jpapbp values.
+    roundup : float, optional
+        Value to round Jplower, by default None.
+    circular : bool, optional
+        Whether to make the colormap circular, by default False.
+    symmetric : bool, optional
+        Whether to make the colormap symmetric, by default True.
+
+    Returns
+    -------
+    np.ndarray
+        The adjusted colormap.
+
+    Notes
+    -----
+    This function adjusts a divergent colormap based on the parameters provided.
+
+    Example
+    -------
+    >>> import numpy as np
+    >>> Jpapbp = np.array([[50.0, 20.0, 10.0], [60.0, 30.0, 15.0]])
+    >>> adjusted_colormap = adjust_divergent(Jpapbp, roundup=5.0, circular=True, symmetric=True)
+    >>> print(adjusted_colormap)
+    array([[55., 20., 10.],
+           [60., 30., 15.]])
+    """
+    Jp = Jpapbp[:, 0]
+    out = Jpapbp.copy()
+    x_extr = extrema(Jp)
+    h = x_extr[0]
+    H = h + 1
+    N = Jpapbp.shape[0]
+    # h = (N + 1) // 2 - 1  # == H-1 if even; == H if odd
+    # H = N // 2
+
+    if Jp[1] > Jp[0] and symmetric:  # hill
+        Jplower = max(Jp[0], Jp[-1])
+        Jpupper = min(Jp[h], Jp[H])
+    elif Jp[1] > Jp[0] and not symmetric:  # hill
+        Jplower = Jp[0]
+        Jpupper = Jp[h]
+    elif Jp[1] < Jp[0] and symmetric:  # valley
+        Jplower = max(Jp[h], Jp[H])
+        Jpupper = min(Jp[0], Jp[-1])
+    else:
+        Jplower = Jp[h]
+        Jpupper = Jp[-1]
+    if roundup is not None:
+        Jplower = np.ceil(Jplower / roundup) * roundup
+
+    L = uniformize(Jpapbp[: h + 1, :], Jplower=Jplower, Jpupper=Jpupper)
+    R = uniformize(Jpapbp[H:, :], Jplower=Jplower, Jpupper=Jpupper)
+    Jpapbp_unif = np.append(L, R[N % 2 :, :], axis=0)
+
+    if circular:
+        theta = 2 * np.pi * np.linspace(0, 1, out.shape[0])
+        out[0, 1:3] = out[-1, 1:3]
+        cs = CubicSpline(theta, out[:, 1:3], bc_type="periodic")
+        Jpapbp_unif[:, 1:3] = cs(theta)
+    return Jpapbp_unif
+
+
+def uniformize_cmap(
+    cmap: ListedColormap,
+    name: str = "new_cmap",
+    lift: float = None,
+    uniformized: bool = False
+) -> Tuple[ListedColormap, bool]:
+    """
+    Uniformize a colormap.
+
+    This function uniformizes a given colormap if it's not already uniformized.
+
+    Parameters
+    ----------
+    cmap : ListedColormap
+        The input colormap to be uniformized.
+    name : str, optional
+        The name of the new colormap, by default "new_cmap".
+    lift : float, optional
+        Value to round Jplower, by default None.
+    uniformized : bool, optional
+        Indicates whether the colormap is already uniformized, by default False.
+
+    Returns
+    -------
+    Tuple[ListedColormap, bool]
+        A tuple containing the uniformized colormap and a boolean indicating if
+        the colormap was uniformized.
+
+    Notes
+    -----
+    This function uniformizes a colormap by analyzing its color table and transforming
+    it into a uniformized version based on its color characteristics.
+
+    Example
+    -------
+    >>> import matplotlib.pyplot as plt
+    >>> from matplotlib.colors import ListedColormap
+    >>> from my_module import uniformize_cmap
+    >>> # Create a sample colormap
+    >>> original_cmap = plt.get_cmap("viridis")
+    >>> uniformized_cmap, was_uniformized = uniformize_cmap(original_cmap, name="uniform_viridis", lift=5.0)
+    >>> if was_uniformized:
+    ...     print("Colormap was uniformized.")
+    ... else:
+    ...     print("Colormap was already uniformized.")
+    >>> # Now you can use the uniformized_cmap for plotting.
+
+    """
+    # if not uniformized yet, uniformize the cmap
+    # else do nothing
+    if not uniformized:
+        # get the color table
+        ctab = get_ctab(cmap)
+        # transform to Jpapbp
+        t_ctab = transform(ctab)
+        # find if sequential or divergent or unknown
+        cmap_type = classify(t_ctab)
+        if cmap_type == "divergent":
+            lin_ctab = adjust_divergent(t_ctab, roundup=lift)
+        elif cmap_type == "asym_div":
+            lin_ctab = adjust_divergent(t_ctab, roundup=lift, symmetric=False)
+        elif cmap_type == "sequential":
+            lin_ctab = adjust_sequential(t_ctab, roundup=lift)
+        elif cmap_type == "multiseq":
+            lin_ctab = adjust_sequential(t_ctab, roundup=lift, bi_seq=True)
+        elif cmap_type == "circular-flat":
+            lin_ctab = adjust_circular_flat(t_ctab)
+        elif cmap_type == "circular-div":
+            lin_ctab = adjust_divergent(t_ctab, roundup=lift, circular=True)
+        else:
+            warnings.warn(
+                "The colormap {} type is unknown (not recognized as sequential or divergent)\n"
+                "Not uniformized".format(name)
+            )
+            lin_ctab = t_ctab
+
+        lin_cmap = transform(ctab=lin_ctab, inverse=True)
+
+        return ListedColormap(np.clip(lin_cmap, 0, 1), name=name), True
+    else:
+        return cmap, True
+
+
+def symmetrize_cmap(
+    cmap: ListedColormap,
+    name: str = "new_cmap",
+    bitonic: bool = True,
+    diffuse: bool = True
+) -> ListedColormap:
+    """
+    Symmetrize a colormap.
+
+    This function symmetrizes a given colormap based on its color characteristics.
+
+    Parameters
+    ----------
+    cmap : ListedColormap
+        The input colormap to be symmetrized.
+    name : str, optional
+        The name of the new colormap, by default "new_cmap".
+    bitonic : bool, optional
+        If True, ensures that half of Cp increases monotonically, by default True.
+    diffuse : bool, optional
+        If True, diffuses the colormap, by default True.
+
+    Returns
+    -------
+    ListedColormap
+        The symmetrized colormap.
+
+    Notes
+    -----
+    This function symmetrizes a colormap by analyzing its color table, transforming
+    it into a symmetrical version based on its color characteristics, and returning
+    it as a matplotlib ListedColormap.
+
+    Example
+    -------
+    >>> import matplotlib.pyplot as plt
+    >>> from matplotlib.colors import ListedColormap
+    >>> from my_module import symmetrize_cmap
+    >>> # Create a sample colormap
+    >>> original_cmap = plt.get_cmap("coolwarm")
+    >>> symmetrized_cmap = symmetrize_cmap(original_cmap, name="symmetric_coolwarm", bitonic=True, diffuse=True)
+    >>> # Now you can use the symmetrized_cmap for plotting.
+
+    """
+    # get the color table
+    ctab = get_ctab(cmap)
+    # transform to Jpapbp
+    t_ctab = transform(ctab)
+    # find if sequential or divergent or unknown
+    cmap_type = classify(t_ctab)
+    diverging = True if cmap_type == "divergent" else False
+    lin_ctab = symmetrize(t_ctab, bitonic=bitonic, diffuse=diffuse, diverging=diverging)
+    # get back a matplotlib cmap object
+    s_cmap = transform(ctab=lin_ctab, inverse=True)
+    return ListedColormap(np.clip(s_cmap, 0, 1), name=name)
+
+
+def unif_sym_cmap(
+    cmap: ListedColormap,
+    name: str = "new_cmap",
+    lift: float = None,
+    uniformized: bool = False,
+    bitonic: bool = True,
+    diffuse: bool = True
+) -> tuple[ListedColormap, bool]:
+    """
+    Uniformize and symmetrize a colormap (perceptually homogeneous).
+
+    This function performs both uniformization and symmetrization of a given colormap
+    based on its color characteristics (symmetric saturation for even perception of both sides of the cmap).
+
+    Parameters
+    ----------
+    cmap : ListedColormap
+        The input colormap to be uniformized and symmetrized.
+    name : str, optional
+        The name of the new colormap, by default "new_cmap".
+    lift : float, optional
+        A parameter controlling the degree of uniformization, by default None.
+    uniformized : bool, optional
+        If True, skip uniformization step if the colormap is already uniformized,
+        by default False.
+    bitonic : bool, optional
+        If True, ensures that half of Cp increases monotonically, by default True.
+    diffuse : bool, optional
+        If True, diffuses the colormap, by default True.
+
+    Returns
+    -------
+    tuple[ListedColormap, bool]
+        A tuple containing the uniformized and symmetrized colormap, and a boolean
+        indicating whether uniformization was performed.
+
+    Notes
+    -----
+    This function first checks if uniformization is needed based on the `uniformized`
+    parameter. If uniformization is performed, the colormap is transformed into a
+    uniformized version based on its color characteristics. Then, symmetrization is
+    applied to the uniformized colormap. The final colormap is returned along with
+    a boolean indicating whether uniformization was performed.
+
+    Example
+    -------
+    >>> import matplotlib.pyplot as plt
+    >>> from matplotlib.colors import ListedColormap
+    >>> from my_module import unif_sym_cmap
+    >>> # Create a sample colormap
+    >>> original_cmap = plt.get_cmap("coolwarm")
+    >>> uniformized_symmetric_cmap, uniformized = unif_sym_cmap(original_cmap, name="uni_sym_coolwarm", lift=0.1)
+    >>> # Now you can use the uniformized_symmetric_cmap for plotting.
+
+    """
+    uni_cmap, uniformized = uniformize_cmap(
+        cmap, name=name, lift=lift, uniformized=uniformized
+    )
+    return (
+        symmetrize_cmap(uni_cmap, name=name, bitonic=bitonic, diffuse=diffuse),
+        uniformized,
+    )
+
+
+def _ax_cylinder_JCh(
+    ax: matplotlib.axes.Axes,
+    cmap: Colormap,
+    title: str
+) -> matplotlib.axes.Axes:
+    """
+    Plot Jp, Cp, and hp coordinates in a cylindrical representation for a colormap.
+
+    This function visualizes the J' (lightness), C' (chroma), and h' (hue) coordinates
+    of a colormap in a cylindrical representation.
+
+    Parameters
+    ----------
+    ax : matplotlib.axes._axes.Axes
+        The matplotlib axes object to plot on.
+    cmap : matplotlib.colors.Colormap
+        The input colormap to visualize.
+    title : str
+        The title of the plot.
+
+    Returns
+    -------
+    matplotlib.axes._axes.Axes
+        The matplotlib axes object containing the plotted data.
+
+    Notes
+    -----
+    This function takes a colormap and extracts its J', C', and h' coordinates in
+    the CAM02-UCS color space. It then plots these coordinates in a cylindrical
+    representation, where J' and C' are shown on one axis, and h' on another axis.
+
+    Example
+    -------
+    >>> import matplotlib.pyplot as plt
+    >>> from matplotlib.colors import ListedColormap
+    >>> from my_module import _ax_cylinder_JCh
+    >>> # Create a sample colormap
+    >>> cmap = plt.get_cmap("coolwarm")
+    >>> fig, ax = plt.subplots()
+    >>> _ax_cylinder_JCh(ax, cmap, title="Cylindrical JCh Coordinates")
+
+    """
+    ctab = get_ctab(cmap)  # get the colormap as a color table in sRGB
+    Jpapbp = transform(ctab)  # transform color table into CAM02-UCS colorspace
+
+    Jp = Jpapbp[:, 0]
+    ap = Jpapbp[:, 1]
+    bp = Jpapbp[:, 2]
+
+    Cp = np.sqrt(ap * ap + bp * bp)
+    hp = np.arctan2(bp, ap) * 180 / np.pi
+    v = np.linspace(0.0, 1.0, len(Jp))
+
+    ax.set_title(title + "\nJpCphp coord. (cyl)", fontsize=14)
+    ax.set_xlabel("Value", fontsize=14)
+
+    axtx = ax.twinx()
+    ax.set_ylim(0, 100)
+    ax.set_ylabel("J' & C' (0-100)", fontsize=14)
+    axtx.set_ylim(-180, 180)
+    axtx.set_ylabel("h' (degrees)", fontsize=14)
+
+    ax.scatter(v, Jp, color=ctab, label="J' (lightness)")
+    ax.plot(v, Cp, c="k", linestyle="--", label="C' (chroma)")
+    axtx.scatter(v[::15], hp[::15], s=10, c="k")
+    ax.scatter([], [], s=10, c="k", label="h' (hue)")
+    ax.legend(loc="best")
+    return ax
+
+
+def _ax_scatter_Jpapbp(
+    ax: matplotlib.axes.Axes,
+    cmap: Colormap,
+    title: str
+) -> matplotlib.axes.Axes:
+    """
+    Create a scatter plot in 3D to visualize Jpapbp coordinates of a colormap.
+
+    This function creates a 3D scatter plot to visualize the J', a', and b' coordinates
+    of a colormap in the CAM02-UCS color space.
+
+    Parameters
+    ----------
+    ax : matplotlib.axes._axes.Axes
+        The matplotlib axes object to plot on.
+    cmap : matplotlib.colors.Colormap
+        The input colormap to visualize.
+    title : str
+        The title of the plot.
+
+    Returns
+    -------
+    matplotlib.axes._axes.Axes
+        The matplotlib axes object containing the plotted data.
+
+    Notes
+    -----
+    This function takes a colormap, extracts its J', a', and b' coordinates in the
+    CAM02-UCS color space, and creates a 3D scatter plot to visualize these coordinates.
+
+    Example
+    -------
+    >>> import matplotlib.pyplot as plt
+    >>> from matplotlib.colors import ListedColormap
+    >>> from my_module import _ax_scatter_Jpapbp
+    >>> # Create a sample colormap
+    >>> cmap = plt.get_cmap("coolwarm")
+    >>> fig = plt.figure()
+    >>> ax = fig.add_subplot(111, projection='3d')
+    >>> _ax_scatter_Jpapbp(ax, cmap, title="Jpapbp Scatter Plot")
+
+    """
+    ctab = get_ctab(cmap)  # get the colormap as a color table in sRGB
+    Jpapbp = transform(ctab)  # transform color table into CAM02-UCS colorspace
+
+    # ax.plot(Jpapbp[:, 1], Jpapbp[:, 2], Jpapbp[:, 0])
+    x_dots = np.linspace(0, 1, Jpapbp.shape[0])
+    RGB_dots = cmap(x_dots)[:, :3]
+    Jpapbp_dots = transform(RGB_dots)
+    ax.scatter(
+        Jpapbp_dots[:, 1], Jpapbp_dots[:, 2], Jpapbp_dots[:, 0], c=RGB_dots[:, :], s=80
+    )
+    ax.set_xlabel("a' (green -> red)")
+    ax.set_ylabel("b' (blue -> yellow)")
+    ax.set_zlabel("J'/K (black -> white)")
+    ax.set_title(title + "\nJpapbp coord.", fontsize=14)
+    return ax
```

### Comparing `scicomap-1.0.0/src/scicomap/data/grmhd.png` & `scicomap-1.0.1/src/scicomap/data/grmhd.png`

 * *Files identical despite different names*

### Comparing `scicomap-1.0.0/src/scicomap/data/jacksboro_fault_dem.npz` & `scicomap-1.0.1/src/scicomap/data/jacksboro_fault_dem.npz`

 * *Files identical despite different names*

### Comparing `scicomap-1.0.0/src/scicomap/data/s1045.ima.gz` & `scicomap-1.0.1/src/scicomap/data/s1045.ima.gz`

 * *Files identical despite different names*

### Comparing `scicomap-1.0.0/src/scicomap/data/tng.jpg` & `scicomap-1.0.1/src/scicomap/data/tng.jpg`

 * *Files identical despite different names*

### Comparing `scicomap-1.0.0/src/scicomap/data/vortex.jpg` & `scicomap-1.0.1/src/scicomap/data/vortex.jpg`

 * *Files identical despite different names*

### Comparing `scicomap-1.0.0/src/scicomap/datasets.py` & `scicomap-1.0.1/src/scicomap/datasets.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-import gzip
-import warnings
-from pkg_resources import resource_stream, resource_filename
-import numpy as np
-import matplotlib.image as mpimg
-from os.path import dirname, join
-
-
-def load_hill_topography() -> np.ndarray:
-    """
-    Load hill topography elevation data.
-
-    This function loads hill topography elevation data from a pre-stored NumPy .npz file.
-    The elevation data represents the topography of a geographical region.
-
-    Returns
-    -------
-    numpy.ndarray
-        A NumPy array containing elevation data, representing the topography.
-
-    Notes
-    -----
-    The elevation data is typically a 2D array representing the elevation (height) of
-    different points in the geographical region. It can be used for various geographic
-    and geological analyses.
-
-    Example
-    -------
-    >>> from my_module import load_hill_topography
-    >>> elevation_data = load_hill_topography()
-    >>> print(elevation_data.shape)  # Print the shape of the loaded elevation data.
-
-    """
-    stream = resource_stream(__name__, "data/jacksboro_fault_dem.npz")
-    # module_path = dirname(__file__)
-    # data_file_name = join(module_path, 'data', 'jacksboro_fault_dem.npz')
-    with np.load(stream) as dem:
-        elevation = dem["elevation"]
-    return elevation
-
-
-def load_scan_image() -> np.ndarray:
-    """
-    Load a scanned image.
-
-    This function loads a scanned image from a pre-stored gzip-compressed binary file.
-    The image data is assumed to be in a specific format and is returned as a NumPy array.
-
-    Returns
-    -------
-    numpy.ndarray
-        A NumPy array containing the scanned image data.
-
-    Notes
-    -----
-    The scanned image data is expected to be a grayscale image, and the function assumes
-    that it's stored in a specific binary format. The image is typically a 2D array
-    of pixel values representing the scanned content.
-
-    Example
-    -------
-    >>> from my_module import load_scan_image
-    >>> scan_image = load_scan_image()
-    >>> print(scan_image.shape)  # Print the shape of the loaded scanned image.
-
-    """
-    # module_path = dirname(__file__)
-    # data_file_name = join(module_path, 'data', 's1045.ima.gz')
-    stream = resource_stream(__name__, "data/s1045.ima.gz")
-    with gzip.open(stream) as dfile:
-        scan_im = np.frombuffer(dfile.read(), np.uint16).reshape((256, 256))
-    return scan_im
-
-
-def load_pic(name: str = "grmhd") -> np.ndarray:
-    """
-    Load an image.
-
-    This function loads an image from a pre-stored image file based on the provided `name`.
-    The image data is returned as a NumPy array.
-
-    Parameters
-    ----------
-    name : str, optional
-        The name of the image to load. Default is "grmhd".
-        Supported names: "grmhd", "vortex", "tng".
-
-    Returns
-    -------
-    numpy.ndarray
-        A NumPy array containing the image data.
-
-    Raises
-    ------
-    TypeError
-        If the `name` parameter is not a string.
-
-    Notes
-    -----
-    This function loads an image file based on the provided `name`. It assumes
-    that the image files are stored in a specific directory structure.
-
-    Example
-    -------
-    >>> from my_module import load_pic
-    >>> grmhd_image = load_pic("grmhd")
-    >>> print(grmhd_image.shape)  # Print the shape of the loaded image.
-
-    """
-
-    if not isinstance(name, str):
-        TypeError("name should be a string")
-
-    module_path = dirname(__file__)
-    im_path = resource_filename(__name__, "data/grmhd.png")
-    # pic_path = join(module_path, 'data', 'grmhd.png')
-    if name == "grmhd":
-        im_path = resource_filename(__name__, "data/grmhd.png")
-    elif name == "vortex":
-        im_path = resource_filename(__name__, "data/vortex.jpg")
-    elif name == "tng":
-        im_path = resource_filename(__name__, "data/tng.jpg")
-    else:
-        warnings.warn(
-            "Using a default image, name should be in ['grmhd', 'vortex', 'tng']"
-        )
-
-    img = mpimg.imread(im_path)
-    return img[:, :, 0]
+import gzip
+import warnings
+from pkg_resources import resource_stream, resource_filename
+import numpy as np
+import matplotlib.image as mpimg
+from os.path import dirname, join
+
+
+def load_hill_topography() -> np.ndarray:
+    """
+    Load hill topography elevation data.
+
+    This function loads hill topography elevation data from a pre-stored NumPy .npz file.
+    The elevation data represents the topography of a geographical region.
+
+    Returns
+    -------
+    numpy.ndarray
+        A NumPy array containing elevation data, representing the topography.
+
+    Notes
+    -----
+    The elevation data is typically a 2D array representing the elevation (height) of
+    different points in the geographical region. It can be used for various geographic
+    and geological analyses.
+
+    Example
+    -------
+    >>> from my_module import load_hill_topography
+    >>> elevation_data = load_hill_topography()
+    >>> print(elevation_data.shape)  # Print the shape of the loaded elevation data.
+
+    """
+    stream = resource_stream(__name__, "data/jacksboro_fault_dem.npz")
+    # module_path = dirname(__file__)
+    # data_file_name = join(module_path, 'data', 'jacksboro_fault_dem.npz')
+    with np.load(stream) as dem:
+        elevation = dem["elevation"]
+    return elevation
+
+
+def load_scan_image() -> np.ndarray:
+    """
+    Load a scanned image.
+
+    This function loads a scanned image from a pre-stored gzip-compressed binary file.
+    The image data is assumed to be in a specific format and is returned as a NumPy array.
+
+    Returns
+    -------
+    numpy.ndarray
+        A NumPy array containing the scanned image data.
+
+    Notes
+    -----
+    The scanned image data is expected to be a grayscale image, and the function assumes
+    that it's stored in a specific binary format. The image is typically a 2D array
+    of pixel values representing the scanned content.
+
+    Example
+    -------
+    >>> from my_module import load_scan_image
+    >>> scan_image = load_scan_image()
+    >>> print(scan_image.shape)  # Print the shape of the loaded scanned image.
+
+    """
+    # module_path = dirname(__file__)
+    # data_file_name = join(module_path, 'data', 's1045.ima.gz')
+    stream = resource_stream(__name__, "data/s1045.ima.gz")
+    with gzip.open(stream) as dfile:
+        scan_im = np.frombuffer(dfile.read(), np.uint16).reshape((256, 256))
+    return scan_im
+
+
+def load_pic(name: str = "grmhd") -> np.ndarray:
+    """
+    Load an image.
+
+    This function loads an image from a pre-stored image file based on the provided `name`.
+    The image data is returned as a NumPy array.
+
+    Parameters
+    ----------
+    name : str, optional
+        The name of the image to load. Default is "grmhd".
+        Supported names: "grmhd", "vortex", "tng".
+
+    Returns
+    -------
+    numpy.ndarray
+        A NumPy array containing the image data.
+
+    Raises
+    ------
+    TypeError
+        If the `name` parameter is not a string.
+
+    Notes
+    -----
+    This function loads an image file based on the provided `name`. It assumes
+    that the image files are stored in a specific directory structure.
+
+    Example
+    -------
+    >>> from my_module import load_pic
+    >>> grmhd_image = load_pic("grmhd")
+    >>> print(grmhd_image.shape)  # Print the shape of the loaded image.
+
+    """
+
+    if not isinstance(name, str):
+        TypeError("name should be a string")
+
+    module_path = dirname(__file__)
+    im_path = resource_filename(__name__, "data/grmhd.png")
+    # pic_path = join(module_path, 'data', 'grmhd.png')
+    if name == "grmhd":
+        im_path = resource_filename(__name__, "data/grmhd.png")
+    elif name == "vortex":
+        im_path = resource_filename(__name__, "data/vortex.jpg")
+    elif name == "tng":
+        im_path = resource_filename(__name__, "data/tng.jpg")
+    else:
+        warnings.warn(
+            "Using a default image, name should be in ['grmhd', 'vortex', 'tng']"
+        )
+
+    img = mpimg.imread(im_path)
+    return img[:, :, 0]
```

### Comparing `scicomap-1.0.0/src/scicomap/scicomap.py` & `scicomap-1.0.1/src/scicomap/scicomap.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,1498 +1,1498 @@
-"""
-Main module for scientific colormaps. It uses the CAM02-UCS color space
-Its three coordinates are usually denoted by J', a', and b' and its cylindrical coordinates are J', C', and h'.
-This package is built on matplotlib, colorspacious, viscm and EHTplot packages for
-the color mathematics and transformations and uses colormaps coming from different packages aiming
-to provide scientific colormaps but requiring some adjustments.
-
-- Provide sequential, multi-sequential, diverging, circular and qualitative (discrete) cmaps
-- Uniformize: linearize the CAM02-UCS lightness J'
-- Symmetrize: make the CAM02-UCS chroma C' symmetrical, bitonic or not, smooth or not
-- Get the matplotlib cmap object, before and after the adjustments
-- Charts to assess the quality of the colormaps (JCh plot)
-- Charts to assess the readability by colour weak/deficient/blind people
-- Charts for illustrating all the available colormaps
-
-The module structure is the following:
----------------------------------------
-- ``SciCoMap`` Parent class for all the colormap types
-- ``ScicoSequential`` Child class for sequential colormaps
-- ``ScicoMultiSequential`` Child class for multi-sequential colormaps
-- ``ScicoDiverging`` Child class for diverging colormaps
-- ``ScicoCircular`` Child class for circular colormaps (circular diverging and circular flat aka phase)
-- ``ScicoMiscellaneous`` Child class for continuous colormaps which are none of the above
-- ``ScicoQualitative`` Child class for discrete colormaps
-- ``plot_colormap`` function for illustrating all the color maps of a given type
-- ``plot_colorblind_vision`` function for comparing the rendering with different color deficiencies
-- ``compare_cmap`` function for comparing the rendering when using an image.
-
-"""
-
-import matplotlib.pyplot as plt
-import matplotlib.image as mpimg
-from matplotlib.colors import Colormap, ListedColormap
-import numpy as np
-from scicomap.datasets import load_hill_topography, load_scan_image, load_pic
-from typing import List, Tuple, Union, Callable, Optional, Dict, Any
-
-# Scientific Colours
-import colorcet as cc
-import cmasher as cmr
-from cmcrameri import cm as scico
-import cmocean
-from palettable.cubehelix import perceptual_rainbow_16, classic_16
-from palettable.cartocolors.qualitative import Bold_10, Pastel_10, Prism_10, Vivid_10
-from palettable.colorbrewer.qualitative import Set1_9
-
-# internal import
-from scicomap.cmath import (
-    uniformize_cmap,
-    symmetrize_cmap,
-    unif_sym_cmap,
-    _ax_cylinder_JCh,
-    _ax_scatter_Jpapbp,
-)
-from scicomap.cblind import _get_color_weak_cmap, colorblind_vision
-from scicomap.utils import (
-    _pyramid,
-    _pyramid_zombie,
-    _fn_with_roots,
-    _periodic_fn,
-    _plot_examples,
-    _plot_examples_qual,
-    _complex_phase,
-)
-
-
-class SciCoMap:
-    """
-    Get a matplotlib-compatible colormap from different packages, mainly scientific color maps [1]_ [2]_ [3]_ [4]_
-
-    Parameters
-    ----------
-    ctype : str, optional
-        Color map type, one of {'sequential', 'multi-sequential', 'diverging',
-        'circular', 'miscellaneous', 'qualitative'}. Default is 'sequential'.
-    cmap : str or cmap object, optional
-        The name of the color map you want to use or the matplotlib cmap object.
-        Default is 'thermal'.
-
-    Attributes
-    ----------
-    color_map_dic : dict
-        The mapping dictionary for some colormaps.
-    ctype : str
-        Color map type, one of {'sequential', 'diverging', 'qualitative'}.
-    cname : str
-        The name of the color map.
-    cmap : matplotlib cmap or list of hex/rgb
-        The color map.
-    uniformized : bool
-        If the cmap has been uniformized or not.
-
-    Methods
-    -------
-    get_ctype()
-        Get the colormap type.
-    get_mpl_color_map()
-        Get the matplotlib colormap (cmap object).
-    uniformize_cmap(lift=None)
-        Uniformize the colormap (linearize the brightness J').
-    symmetrize_cmap(bitonic=True, diffuse=True)
-        Symmetrize the hue (h').
-    unif_sym_cmap(lift=None, bitonic=True, diffuse=True)
-        Uniformize and symmetrize at once.
-    get_color_map_names()
-        Get the name of all the available color maps.
-    get_color_map_dic()
-        Get the color maps dictionary.
-    assess_cmap(figsize=(18, 8))
-        Plot the Jch tensor to visualize the brightness (J'), the hue (h'), and the chroma (c').
-    illustrate_palettes(figsize=(12, 10), n_colors=256)
-        Plot the gradient or discrete palettes of all the colormaps of the given type.
-    colorblind(figsize=(12, 5), n_colors=256, facecolor="black")
-        Plot the gradient or barchart of the colormap for different kinds of color deficiencies.
-
-    Examples
-    --------
-    ccmap = SciCoMap(ctype='sequential', cmap='thermal')
-    mpl_map = ccmap.get_mpl_color_map()
-
-    References
-    ----------
-    [1] https://www.kennethmoreland.com/color-advice/
-    [2] https://mycarta.wordpress.com/2012/05/29/the-rainbow-is-dead-long-live-the-rainbow-series-outline/
-    [3] http://www.fabiocrameri.ch/colourmaps.php
-    [4] https://betterfigures.org/2015/06/23/picking-a-colour-scale-for-scientific-graphics/
-    """
-
-    def __init__(self, ctype: str = "sequential", cmap: Union[str, Colormap] = "thermal"):
-        self.ctype = ctype
-        self.color_map_dic = get_cmap_dict()
-        self.cmap = cmap
-        self.cname = "cmap"
-        self.uniformized = False
-
-    def __repr__(self):
-        s = f"SciCoMap(ctype={self.ctype}, cmap={self.cname})"
-        return s
-
-    @classmethod
-    def get_ctype(cls) -> List[str]:
-        """Return the colormap type."""
-        return list(get_cmap_dict().keys())
-
-    def get_mpl_color_map(self) -> Colormap:
-        """
-        Get the matplotlib colormap object.
-
-        Returns
-        -------
-        color_map : mpl colormap
-            The colormap object.
-        """
-        if isinstance(self.cmap, str):
-            if self.cmap not in self.color_map_dic[self.ctype].keys():
-                raise ValueError(
-                    f"Current built-in cmaps are: {self.color_map_dic[self.ctype].keys()}"
-                )
-            self.cname = self.cmap
-            self.cmap = self.color_map_dic[self.ctype][self.cmap]
-        else:
-            self.cname = self.cmap.name
-
-        return self.cmap
-
-    def uniformize_cmap(self, lift: Optional[int] = None):
-        """
-        Uniformize the colormap, meaning linearizing the brightness (J')
-        in the CAM02-UCS color space.
-
-        Parameters
-        ----------
-        lift : None or int in [0, 100], optional
-            Lift or not the darkest part of the colormap.
-
-        Returns
-        -------
-        None
-        """
-        self.get_mpl_color_map()
-        self.cmap, self.uniformized = uniformize_cmap(
-            cmap=self.cmap, name=self.cname, lift=lift, uniformized=self.uniformized
-        )
-
-    def symmetrize_cmap(self, bitonic: bool = True, diffuse: bool = True):
-        """
-        Symmetrize the colormap (the hue) in the CAM02-UCS color space.
-        It can be symmetrized in a bitonic way or not (if bitonic, the hue
-        curve will be symmetric with an extremum at its center).
-
-        The hue curve can be smoothed (diffuse) or not (edges might occur).
-
-        Parameters
-        ----------
-        bitonic : bool, optional (default=True)
-            Bitonic symmetrization or not (extremum located at the center of the hue curve).
-        diffuse : bool, optional (default=True)
-            Smooth hue curve or not (if not, edges might occur).
-
-        Returns
-        -------
-        None
-        """
-        self.get_mpl_color_map()
-        self.cmap = symmetrize_cmap(
-            cmap=self.cmap, name=self.cname, bitonic=bitonic, diffuse=diffuse
-        )
-
-    def unif_sym_cmap(
-        self, lift: Optional[int] = None, bitonic: bool = True, diffuse: bool = True
-    ):
-        """
-        First, uniformize the colormap, meaning linearizing the brightness (J')
-        in the CAM02-UCS color space.
-
-        Second, symmetrize the colormap (the hue) in the CAM02-UCS color space.
-        It can be symmetrized in a bitonic way or not (if bitonic, the hue
-        curve will be symmetric with an extremum at its center).
-
-        The hue curve can be smoothed (diffuse) or not (edges might occur).
-
-        Parameters
-        ----------
-        lift : None or int in [0, 100], optional
-            Lift or not the darkest part of the colormap.
-        bitonic : bool, optional (default=True)
-            Bitonic symmetrization or not (extremum located at the center of the hue curve).
-        diffuse : bool, optional (default=True)
-            Smooth hue curve or not (if not, edges might occur).
-
-        Returns
-        -------
-        None
-        """
-        self.get_mpl_color_map()
-        self.cmap, self.uniformized = unif_sym_cmap(
-            cmap=self.cmap,
-            name=self.cname,
-            lift=lift,
-            uniformized=self.uniformized,
-            bitonic=bitonic,
-            diffuse=diffuse,
-        )
-
-    def get_color_map_names(self) -> List[str]:
-        """
-        Get the names of the implemented colormaps for the chosen ctype.
-
-        Returns
-        -------
-        List of str
-            List of colormap names.
-        """
-        return list(self.color_map_dic[self.ctype].keys())
-
-    @classmethod
-    def get_color_map_dic(cls) -> dict:
-        """
-        Get the mapping dict of all the available color maps.
-
-        Returns
-        -------
-        dict
-            The dictionary of all the color maps for all ctypes.
-        """
-        return get_cmap_dict()
-
-    def assess_cmap(self, figsize: Tuple[int, int] = (18, 8)) -> plt.figure:
-        """
-        Plot J', C', and h' of a colormap as a function of the mapped value.
-
-        The CAM02-UCS lightness J' is linearized for generating perceptually uniform colormaps
-        (working definition of Perceptually Uniform Sequential colormaps by matplotlib).
-
-        Hue h' can encode an additional physical quantity in an image
-        (when used in this way, the change of hue should be linearly
-        proportional to the quantity).
-
-        The other dimension chroma is less recognizable and should not be
-        used to encode physical information. Since sRGB is only a subset
-        of the Lab color space, there are human recognizable colors that
-        are not displayable. In order to accurately represent the physical
-        quantities.
-
-        Parameters
-        ----------
-        figsize : 2-tuple of int, optional
-            The figure size.
-
-        Returns
-        -------
-        matplotlib.figure.Figure
-            The matplotlib figure object.
-        """
-        color_map = self.get_mpl_color_map()
-        return jch_plot(cmap=color_map, figsize=figsize)
-
-    def illustrate_palettes(
-        self, figsize: Tuple[int, int] = (12, 10), n_colors: int = 256, facecolor: str = "black"
-    ):
-        """
-        Draw the gradient or discrete color palettes for each colormap of the chosen ctype.
-
-        Parameters
-        ----------
-        figsize : 2-tuple of int, optional
-            The figure size.
-        n_colors : int, optional
-            The number of colors to plot (e.g., 10 for qualitative and 256 for continuous).
-        facecolor : str, optional
-            The chart face color. It should be a string of built-in matplotlib colors or a hex color.
-
-        Returns
-        -------
-        None
-        """
-        cmap_list = self.get_color_map_names()
-        ctype = self.ctype
-        plot_colormap(ctype, cmap_list, figsize, n_colors, facecolor)
-        plt.show()
-
-    def colorblind(
-        self, figsize: Tuple[int, int] = (12, 5), n_colors: int = 256, facecolor: str = "black"
-    ):
-        """
-        Draw the gradient or discrete color palettes for different kinds of color vision deficiencies.
-
-        Parameters
-        ----------
-        figsize : 2-tuple of int, optional
-            The figure size.
-        n_colors : int, optional
-            The number of colors to plot (e.g., 10 for qualitative and 256 for continuous).
-        facecolor : str, optional
-            The chart face color. It should be a string of built-in matplotlib colors or a hex color.
-
-        Returns
-        -------
-        None
-        """
-        plot_colorblind_vision(
-            ctype=self.ctype,
-            cmap_list=[self.get_mpl_color_map()],
-            figsize=figsize,
-            n_colors=n_colors,
-            facecolor=facecolor,
-        )
-
-class ScicoSequential(SciCoMap):
-    """
-    Get a matplotlib-compatible sequential color map from different packages providing scientific color maps [1]_ [2]_ [3]_ [4]_
-
-    Parameters
-    ----------
-    cmap : str or matplotlib colormap, optional
-        The name of the color map you want to use. Default is 'thermal'.
-
-    Attributes
-    ----------
-    color_map_dic : dict
-        The mapping dictionary for some colormaps.
-    ctype : str
-        Color map type, one of {'sequential', 'diverging', 'qualitative'}.
-    cname : str
-        The name of the color map.
-    cmap : matplotlib colormap or list of hex/rgb
-        The color map.
-
-    Methods
-    -------
-    get_mpl_color_map()
-        Get the matplotlib color map (or list of hex/rgb colors for qualitative).
-    get_color_map_names()
-        Get the name of all the available color maps.
-    get_color_map_dic()
-        Get the color maps dictionary.
-    illustrate_palettes()
-        Plot the gradient or the discrete palettes (all of them).
-    draw_example(facecolor="black")
-        Draw two charts for illustrative purposes.
-
-    Examples
-    --------
-    sc_map = ScicoSequential(cname='chroma')
-    mpl_map = sc_map.get_mpl_color_map()
-    sc_map.draw_example()
-
-    References
-    ----------
-    [1] https://www.kennethmoreland.com/color-advice/
-    [2] https://mycarta.wordpress.com/2012/05/29/the-rainbow-is-dead-long-live-the-rainbow-series-outline/
-    [3] http://www.fabiocrameri.ch/colourmaps.php
-    [4] https://betterfigures.org/2015/06/23/picking-a-colour-scale-for-scientific-graphics/
-    """
-
-    def __init__(self, cmap: Union[str, Colormap] = "thermal"):
-        super().__init__(cmap=cmap, ctype="sequential")
-
-    def __repr__(self):
-        s = f"ScicoSequential(cmap={self.cname})"
-        return s
-
-    def draw_example(self, facecolor: str = "black", figsize: tuple = (20, 20), cblind: bool = True):
-        """
-        Draw two charts for illustrative purposes.
-
-        Parameters
-        ----------
-        facecolor : str, optional
-            The chart face color. It should be a string of built-in matplotlib colors or a hex color.
-        figsize : tuple, optional
-            The figure size.
-        cblind : bool, optional
-            Whether to simulate color vision deficiencies.
-
-        Returns
-        -------
-        matplotlib.figure.Figure
-            The matplotlib figure object.
-        """
-        color_map = self.get_mpl_color_map()
-        elevation = load_hill_topography()
-        scan_im = load_scan_image()
-        xpyr, ypyr, zpyr = _pyramid()
-        per_x, per_z, per_z = _periodic_fn()
-        images = [elevation, scan_im, zpyr, "3D", per_z, "3D"]
-
-        fig = _plot_examples(
-            color_map=color_map,
-            images=images,
-            arr_3d=[(xpyr, ypyr, zpyr), (per_x, per_z, per_z)],
-            figsize=figsize,
-            facecolor=facecolor,
-            cname=self.cname,
-            cblind=cblind,
-        )
-
-        return fig
-
-class ScicoMultiSequential(SciCoMap):
-    """
-    Get a matplotlib-compatible sequential color map from different packages.
-    Useful for continuous values, for which there is no "centre" or mid-value.
-    Some are suited to a dark background, and others for light backgrounds.
-
-    Parameters
-    ----------
-    cmap : str or matplotlib colormap, optional
-        The name of the color map you want to use. Default is 'chroma'.
-
-    Attributes
-    ----------
-    color_map_dic : dict
-        The mapping dictionary for some colormaps.
-    ctype : str
-        Color map type, one of {'sequential', 'diverging', 'qualitative'}.
-    cname : str
-        The name of the color map.
-    cmap : matplotlib colormap or list of hex/rgb
-        The color map.
-
-    Methods
-    -------
-    get_mpl_color_map()
-        Get the matplotlib color map (or list of hex/rgb colors for qualitative).
-    get_color_map_names()
-        Get the name of all the available color maps.
-    get_color_map_dic()
-        Get the color maps dictionary.
-    illustrate_palettes()
-        Plot the gradient or the discrete palettes (all of them).
-    draw_example(facecolor="black")
-        Draw two charts for illustrative purposes.
-
-    Examples
-    --------
-    sc_map = ScicoMultiSequential(cname='chroma')
-    mpl_map = sc_map.get_mpl_color_map()
-    sc_map.draw_example()
-
-    References
-    ----------
-    [1] https://www.kennethmoreland.com/color-advice/
-    [2] https://mycarta.wordpress.com/2012/05/29/the-rainbow-is-dead-long-live-the-rainbow-series-outline/
-    [3] http://www.fabiocrameri.ch/colourmaps.php
-    [4] https://betterfigures.org/2015/06/23/picking-a-colour-scale-for-scientific-graphics/
-    """
-
-    def __init__(self, cmap: Union[str, Colormap] = "chroma"):
-        super().__init__(cmap=cmap, ctype="multi-sequential")
-
-    def __repr__(self):
-        s = f"ScicoMultiSequential(cmap={self.cname})"
-        return s
-
-    def draw_example(self, facecolor: str = "black", figsize: tuple = (20, 20), cblind: bool = True):
-        """
-        Draw two charts for illustrative purposes.
-
-        Parameters
-        ----------
-        facecolor : str, optional
-            The chart face color. It should be a string of built-in matplotlib colors or a hex color.
-        figsize : tuple, optional
-            The figure size.
-        cblind : bool, optional
-            Whether to simulate color vision deficiencies.
-
-        Returns
-        -------
-        matplotlib.figure.Figure
-            The matplotlib figure object.
-        """
-        color_map = self.get_mpl_color_map()
-        elevation = load_hill_topography()
-        scan_im = load_scan_image()
-        xpyr, ypyr, zpyr = _pyramid_zombie(stacked=True)
-        per_x, per_z, per_z = _periodic_fn()
-        images = [elevation, scan_im, zpyr, "3D", per_z, "3D"]
-
-        fig = _plot_examples(
-            color_map=color_map,
-            images=images,
-            arr_3d=[(xpyr, ypyr, zpyr), (per_x, per_z, per_z)],
-            figsize=figsize,
-            facecolor=facecolor,
-            cname=self.cname,
-            cblind=cblind,
-        )
-
-        return fig
-
-
-class ScicoDiverging(SciCoMap):
-    """
-    Get a matplotlib-compatible diverging color map from different packages.
-    Useful for continuous values with a "center" or mid-value.
-    Some are suited to dark backgrounds, and others for light backgrounds [1]_ [2]_ [3]_ [4]_
-
-    Parameters
-    ----------
-    cmap : str or matplotlib colormap, optional
-        The name of the color map you want to use. Default is 'wildfire'.
-
-    Attributes
-    ----------
-    color_map_dic : dict
-        The mapping dictionary for some colormaps.
-    ctype : str
-        Color map type, one of {'sequential', 'diverging', 'qualitative'}.
-    cname : str
-        The name of the color map.
-    cmap : matplotlib colormap or list of hex/rgb
-        The color map.
-
-    Methods
-    -------
-    get_mpl_color_map()
-        Get the matplotlib color map (or list of hex/rgb colors for qualitative).
-    get_color_map_names()
-        Get the name of all the available color maps.
-    get_color_map_dic()
-        Get the color maps dictionary.
-    illustrate_palettes()
-        Plot the gradient or the discrete palettes (all of them).
-    draw_example(facecolor="black")
-        Draw two charts for illustrative purposes.
-
-    Examples
-    --------
-    sc_map = ScicoDiverging(cname='redshift')
-    mpl_map = sc_map.get_mpl_color_map()
-    sc_map.draw_example()
-
-    References
-    ----------
-    [1] https://www.kennethmoreland.com/color-advice/
-    [2] https://mycarta.wordpress.com/2012/05/29/the-rainbow-is-dead-long-live-the-rainbow-series-outline/
-    [3] http://www.fabiocrameri.ch/colourmaps.php
-    [4] https://betterfigures.org/2015/06/23/picking-a-colour-scale-for-scientific-graphics/
-    """
-
-    def __init__(self, cmap: Union[str, Colormap] = "wildfire"):
-        super().__init__(cmap=cmap, ctype="diverging")
-
-    def __repr__(self):
-        s = f"ScicoDiverging(cmap={self.cname})"
-        return s
-
-    def draw_example(self, facecolor: str = "black", figsize: tuple = (20, 20)):
-        """
-        Draw two charts for illustrative purposes.
-
-        Parameters
-        ----------
-        facecolor : str, optional
-            The chart face color. It should be a string of built-in matplotlib colors or a hex color.
-        figsize : tuple, optional
-            The figure size.
-
-        Returns
-        -------
-        matplotlib.figure.Figure
-            The matplotlib figure object.
-        """
-        color_map = self.get_mpl_color_map()
-        # Create diverging image data
-        image_div = _fn_with_roots()
-        xpyr, ypyr, zpyr = _pyramid_zombie(stacked=False)
-        per_x, per_z, per_z = _periodic_fn()
-
-        images = [image_div, zpyr, "3D", per_z, "3D"]
-
-        fig = _plot_examples(
-            color_map=color_map,
-            images=images,
-            arr_3d=[(xpyr, ypyr, zpyr), (per_x, per_z, per_z)],
-            figsize=figsize,
-            facecolor=facecolor,
-            cname=self.cname,
-            norm=True,
-        )
-
-        return fig
-
-
-class ScicoCircular(SciCoMap):
-    """
-    Get a matplotlib-compatible circular color map from different packages.
-    Useful for angular values (circular "flat" as the phase cmap).
-    There is no "center" or mid-value for circular color maps.
-    Some are suited for dark backgrounds, and others for light backgrounds [1]_ [2]_ [3]_ [4]_
-
-    Parameters
-    ----------
-    cmap : str or matplotlib colormap, optional
-        The name of the color map you want to use. Default is 'colorwheel'.
-
-    Attributes
-    ----------
-    color_map_dic : dict
-        The mapping dictionary for some colormaps.
-    ctype : str
-        Color map type, one of {'sequential', 'diverging', 'qualitative'}.
-    cname : str
-        The name of the color map.
-    cmap : matplotlib colormap or list of hex/rgb
-        The color map.
-
-    Methods
-    -------
-    get_mpl_color_map()
-        Get the matplotlib color map (or list of hex/rgb colors for qualitative).
-    get_color_map_names()
-        Get the name of all the available color maps.
-    get_color_map_dic()
-        Get the color maps dictionary.
-    illustrate_palettes()
-        Plot the gradient or the discrete palettes (all of them).
-    draw_example(facecolor="black")
-        Draw two charts for illustrative purposes.
-
-    Examples
-    --------
-    sc_map = ScicoCircular(cname='colorwheel')
-    mpl_map = sc_map.get_mpl_color_map()
-    sc_map.draw_example()
-
-    References
-    ----------
-    [1] https://www.kennethmoreland.com/color-advice/
-    [2] https://mycarta.wordpress.com/2012/05/29/the-rainbow-is-dead-long-live-the-rainbow-series-outline/
-    [3] http://www.fabiocrameri.ch/colourmaps.php
-    [4] https://betterfigures.org/2015/06/23/picking-a-colour-scale-for-scientific-graphics/
-    """
-
-    def __init__(self, cmap: Union[str, Colormap] = "colorwheel"):
-        super().__init__(cmap=cmap, ctype="circular")
-
-    def __repr__(self):
-        s = f"ScicoCircular(cmap={self.cname})"
-        return s
-
-    def draw_example(self, facecolor: str = "black", figsize: tuple = (20, 20), cblind: bool = True):
-        """
-        Draw two charts for illustrative purposes.
-
-        Parameters
-        ----------
-        facecolor : str, optional
-            The chart face color. It should be a string of built-in matplotlib colors or a hex color.
-        figsize : tuple, optional
-            The figure size.
-        cblind : bool, optional
-            Plot the colorblind version. Default is True.
-
-        Returns
-        -------
-        matplotlib.figure.Figure
-            The matplotlib figure object.
-        """
-        color_map = self.get_mpl_color_map()
-        elevation = load_hill_topography()
-        scan_im = load_scan_image()
-        per_x, per_z, per_z = _periodic_fn()
-        images = [elevation, scan_im, "electric", "complex"]
-
-        fig = _plot_examples(
-            color_map=color_map,
-            images=images,
-            arr_3d=None,
-            figsize=figsize,
-            facecolor=facecolor,
-            cname=self.cname,
-            cblind=cblind,
-        )
-
-        return fig
-
-
-class ScicoMiscellaneous(SciCoMap):
-    """
-    Get a matplotlib-compatible sequential color map from different packages.
-    Useful for continuous values, for which there is no "center" or mid-value.
-    Some are suited for dark backgrounds, and others for light backgrounds [1]_ [2]_ [3]_ [4]_
-
-    Parameters
-    ----------
-    cmap : str or matplotlib colormap, optional
-        The name of the color map you want to use. Default is 'turbo'.
-
-    Attributes
-    ----------
-    color_map_dic : dict
-        The mapping dictionary for some colormaps.
-    ctype : str
-        Color map type, one of {'sequential', 'diverging', 'qualitative'}.
-    cname : str
-        The name of the color map.
-    cmap : matplotlib colormap or list of hex/rgb
-        The color map.
-
-    Methods
-    -------
-    get_mpl_color_map()
-        Get the matplotlib color map (or list of hex/rgb colors for qualitative).
-    get_color_map_names()
-        Get the name of all the available color maps.
-    get_color_map_dic()
-        Get the color maps dictionary.
-    illustrate_palettes()
-        Plot the gradient or the discrete palettes (all of them).
-    draw_example(facecolor="black")
-        Draw two charts for illustrative purposes.
-
-    Examples
-    --------
-    sc_map = ScicoSequential(cname='chroma')
-    mpl_map = sc_map.get_mpl_color_map()
-    sc_map.draw_example()
-
-    References
-    ----------
-    [1] https://www.kennethmoreland.com/color-advice/
-    [2] https://mycarta.wordpress.com/2012/05/29/the-rainbow-is-dead-long-live-the-rainbow-series-outline/
-    [3] http://www.fabiocrameri.ch/colourmaps.php
-    [4] https://betterfigures.org/2015/06/23/picking-a-colour-scale-for-scientific-graphics/
-    """
-
-    def __init__(self, cmap: Union[str, Colormap] = "turbo"):
-        super().__init__(cmap=cmap, ctype="miscellaneous")
-
-    def __repr__(self):
-        s = f"ScicoMiscellaneous(cmap={self.cname})"
-        return s
-
-    def draw_example(self, facecolor: str = "black", figsize: tuple = (20, 20)):
-        """
-        Draw two charts for illustrative purposes.
-
-        Parameters
-        ----------
-        facecolor : str, optional
-            The chart face color. It should be a string of built-in matplotlib colors or a hex color.
-        figsize : tuple, optional
-            The figure size.
-
-        Returns
-        -------
-        matplotlib.figure.Figure
-            The matplotlib figure object.
-        """
-        color_map = self.get_mpl_color_map()
-        image_div = _fn_with_roots()
-        xpyr, ypyr, zpyr = _pyramid_zombie(stacked=False)
-        per_x, per_z, per_z = _periodic_fn()
-
-        images = [image_div, zpyr, "3D", per_z, "3D"]
-
-        fig = _plot_examples(
-            color_map=color_map,
-            images=images,
-            arr_3d=[(xpyr, ypyr, zpyr), (per_x, per_z, per_z)],
-            figsize=figsize,
-            facecolor=facecolor,
-            cname=self.cname,
-            norm=True,
-        )
-
-        return fig
-
-
-class ScicoQualitative(SciCoMap):
-    """
-    Get a matplotlib-compatible qualitative list of colors from different packages.
-    Useful for discrete values or categorical variables.
-    Some are suited for dark backgrounds, and others for light backgrounds [1]_ [2]_ [3]_ [4]_
-
-    Parameters
-    ----------
-    cmap : str or matplotlib colormap, optional
-        The name of the color map you want to use. Default is 'glasbey_dark'.
-
-    Attributes
-    ----------
-    color_map_dic : dict
-        The mapping dictionary for some colormaps.
-    ctype : str
-        Color map type, one of {'sequential', 'diverging', 'qualitative'}.
-    cname : str
-        The name of the color map.
-    cmap : matplotlib colormap or list of hex/rgb
-        The color map.
-
-    Methods
-    -------
-    get_mpl_color_map()
-        Get the matplotlib color map (or list of hex/rgb colors for qualitative).
-    get_color_map_names()
-        Get the name of all the available color maps.
-    get_color_map_dic()
-        Get the color maps dictionary.
-    illustrate_palettes()
-        Plot the gradient or the discrete palettes (all of them).
-    draw_example(facecolor="black")
-        Draw two charts for illustrative purposes.
-
-    Examples
-    --------
-    sc_map = ScicoQualitative(cname='glasbey_dark')
-    mpl_map = sc_map.get_mpl_color_map()
-    sc_map.draw_example()
-
-    References
-    ----------
-    [1] https://www.kennethmoreland.com/color-advice/
-    [2] https://mycarta.wordpress.com/2012/05/29/the-rainbow-is-dead-long-live-the-rainbow-series-outline/
-    [3] http://www.fabiocrameri.ch/colourmaps.php
-    [4] https://betterfigures.org/2015/06/23/picking-a-colour-scale-for-scientific-graphics/
-    """
-
-    def __init__(self, cmap: Union[str, Colormap] = "glasbey_dark"):
-        super().__init__(cmap=cmap, ctype="qualitative")
-
-    def __repr__(self):
-        s = f"ScicoQualitative(cmap={self.cname})"
-        return s
-
-    def draw_example(self, facecolor: str = "black", figsize: tuple = (20, 20)):
-        """
-        Draw two charts for illustrative purposes.
-
-        Parameters
-        ----------
-        facecolor : str, optional
-            The chart face color. It should be a string of built-in matplotlib colors or a hex color.
-        figsize : tuple, optional
-            The figure size.
-
-        Returns
-        -------
-        matplotlib.figure.Figure
-            The matplotlib figure object.
-        """
-        color_map = self.get_mpl_color_map()
-
-        # data from United Nations World Population Prospects (Revision 2019)
-        # https://population.un.org/wpp/, license: CC BY 3.0 IGO
-        year = [1950, 1960, 1970, 1980, 1990, 2000, 2010, 2018]
-        population_by_continent = {
-            "africa": [228, 284, 365, 477, 631, 814, 1044, 1275],
-            "americas": [340, 425, 519, 619, 727, 840, 943, 1006],
-            "asia": [1394, 1686, 2120, 2625, 3202, 3714, 4169, 4560],
-            "europe": [220, 253, 276, 295, 310, 303, 294, 293],
-            "oceania": [12, 15, 19, 22, 26, 31, 36, 39],
-        }
-        x = np.linspace(0, 10)
-        # Fixing random state for reproducibility
-        np.random.seed(19680801)
-        noisy_trends = np.array(
-            [
-                np.sin(x) + x + np.random.randn(50),
-                np.sin(x) + 0.5 * x + np.random.randn(50),
-                np.sin(x) + 2 * x + np.random.randn(50),
-                np.sin(x) - 0.5 * x + np.random.randn(50),
-                np.sin(x) - 2 * x + np.random.randn(50),
-                np.sin(x) + np.random.randn(50),
-            ]
-        )
-        noisy_trends = noisy_trends.T
-
-        dict_arr = [population_by_continent, "scatter", noisy_trends]
-
-        return _plot_examples_qual(
-            color_map=color_map,
-            dict_arr=dict_arr,
-            figsize=figsize,
-            facecolor=facecolor,
-            cname=self.cname,
-            year=year,
-        )
-
-
-def get_cmap_dict() -> Dict[str, Dict[str, Any]]:
-    """
-    Get a dictionary of color maps organized by categories.
-
-    Returns
-    -------
-    dict
-        A nested dictionary containing various color maps categorized as 'diverging', 'sequential',
-        'multi-sequential', 'circular', 'miscellaneous', and 'qualitative'. Each category
-        contains a dictionary of color maps with their associated names.
-    """
-    cmap_dict = {
-        "diverging": {
-            "berlin": scico.berlin,
-            "bjy": cc.cm.bjy,
-            "bky": cc.cm.bky,
-            "BrBG": plt.get_cmap("BrBG"),
-            "broc": scico.broc,
-            "bwr": plt.get_cmap("bwr"),
-            "coolwarm": plt.get_cmap("coolwarm"),
-            "curl": cmocean.cm.curl,
-            "delta": cmocean.cm.delta,
-            "fusion": cmr.fusion,
-            "fusion_r": cmr.fusion_r,
-            "guppy": cmr.guppy,
-            "guppy_r": cmr.guppy_r,
-            "iceburn": cmr.iceburn,
-            "iceburn_r": cmr.iceburn_r,
-            "lisbon": scico.lisbon,
-            "PRGn": plt.get_cmap("PRGn"),
-            "PiYG": plt.get_cmap("PiYG"),
-            "pride": cmr.pride,
-            "pride_r": cmr.pride_r,
-            "PuOr": plt.get_cmap("PuOr"),
-            "RdBu": plt.get_cmap("RdBu"),
-            "RdGy": plt.get_cmap("RdGy"),
-            "RdYlBu": plt.get_cmap("RdYlBu"),
-            "RdYlGn": plt.get_cmap("RdYlGn"),
-            "redshift": cmr.redshift,
-            "redshift_r": cmr.redshift_r,
-            "roma": scico.roma,
-            "seasons_r": cmr.seasons_r,
-            "seismic": plt.get_cmap("seismic"),
-            "spectral": plt.get_cmap("Spectral"),
-            "turbo": plt.get_cmap("turbo"),
-            "vanimo": scico.vanimo,
-            "vik": scico.vik,
-            "viola": cmr.viola,
-            "viola_r": cmr.viola_r,
-            "waterlily": cmr.waterlily,
-            "waterlily_r": cmr.waterlily_r,
-            "watermelon": cmr.watermelon,
-            "watermelon_r": cmr.watermelon_r,
-            "wildfire": cmr.wildfire,
-            "wildfire_r": cmr.wildfire_r,
-        },
-        "sequential": {
-            "afmhot": plt.get_cmap("afmhot"),
-            "amber": cmr.amber,
-            "amber_r": cmr.amber_r,
-            "amp": cmocean.cm.amp,
-            "apple": cmr.apple,
-            "apple_r": cmr.apple_r,
-            "autumn": plt.get_cmap("autumn"),
-            "batlow": scico.batlow,
-            "bilbao": scico.bilbao,
-            "bilbao_r": scico.bilbao_r,
-            "binary": plt.get_cmap("binary"),
-            "Blues": plt.get_cmap("Blues"),
-            "bone": plt.get_cmap("bone"),
-            "BuGn": plt.get_cmap("BuGn"),
-            "BuPu": plt.get_cmap("BuPu"),
-            "chroma": cmr.chroma,
-            "chroma_r": cmr.chroma_r,
-            "cividis": plt.get_cmap("cividis"),
-            "cool": plt.get_cmap("cool"),
-            "copper": plt.get_cmap("copper"),
-            "cosmic": cmr.cosmic,
-            "cosmic_r": cmr.cosmic_r,
-            "deep": cmocean.cm.deep,
-            "dense": cmocean.cm.dense,
-            "dusk": cmr.dusk,
-            "dusk_r": cmr.dusk_r,
-            "eclipse": cmr.eclipse,
-            "eclipse_r": cmr.eclipse_r,
-            "ember": cmr.ember,
-            "ember_r": cmr.ember_r,
-            "fall": cmr.fall,
-            "fall_r": cmr.fall_r,
-            "gem": cmr.gem,
-            "gem_r": cmr.gem_r,
-            "gist_gray": plt.get_cmap("gist_gray"),
-            "gist_heat": plt.get_cmap("gist_heat"),
-            "gist_yarg": plt.get_cmap("gist_yarg"),
-            "GnBu": plt.get_cmap("GnBu"),
-            "Greens": plt.get_cmap("Greens"),
-            "gray": plt.get_cmap("gray"),
-            "Greys": plt.get_cmap("Greys"),
-            "haline": cmocean.cm.haline,
-            "hawaii": scico.hawaii,
-            "hawaii_r": scico.hawaii,
-            "heat": cmr.torch,
-            "heat_r": cmr.torch_r,
-            "hot": plt.get_cmap("hot"),
-            "ice": cmocean.cm.ice,
-            "inferno": plt.get_cmap("inferno"),
-            "imola": scico.imola,
-            "imola_r": scico.imola_r,
-            "lapaz": scico.lapaz,
-            "lapaz_r": scico.lapaz_r,
-            "magma": plt.get_cmap("magma"),
-            "matter": cmocean.cm.matter,
-            "neon": cmr.neon,
-            "neon_r": cmr.neon_r,
-            "neutral": cmr.neutral,
-            "neutral_r": cmr.neutral_r,
-            "nuuk": scico.nuuk,
-            "nuuk_r": scico.nuuk,
-            "ocean": cmr.ocean,
-            "ocean_r": cmr.ocean_r,
-            "OrRd": plt.get_cmap("OrRd"),
-            "Oranges": plt.get_cmap("Oranges"),
-            "pink": plt.get_cmap("pink"),
-            "plasma": plt.get_cmap("plasma"),
-            "PuBu": plt.get_cmap("PuBu"),
-            "PuBuGn": plt.get_cmap("PuBuGn"),
-            "PuRd": plt.get_cmap("PuRd"),
-            "Purples": plt.get_cmap("Purples"),
-            "rain": cmocean.cm.rain,
-            "rainbow": perceptual_rainbow_16.mpl_colormap,
-            "rainbow-sc": scico.batlow,
-            "rainbow-sc_r": scico.batlow_r,
-            "rainforest": cmr.rainforest,
-            "rainforest_r": cmr.rainforest_r,
-            "RdPu": plt.get_cmap("RdPu"),
-            "Reds": plt.get_cmap("Reds"),
-            "savanna": cmr.savanna,
-            "savanna_r": cmr.savanna_r,
-            "sepia": cmr.sepia,
-            "sepia_r": cmr.sepia_r,
-            "speed": cmocean.cm.speed,
-            "solar": cmocean.cm.solar,
-            "spring": plt.get_cmap("spring"),
-            "summer": plt.get_cmap("summer"),
-            "tempo": cmocean.cm.tempo,
-            "thermal": cmocean.cm.thermal,
-            "thermal_r": cmocean.cm.thermal_r,
-            "thermal-2": cc.cm.bmy,
-            "tokyo": scico.tokyo,
-            "tokyo_r": scico.tokyo_r,
-            "tropical": cmr.tropical,
-            "tropical_r": cmr.tropical_r,
-            "turbid": cmocean.cm.turbid,
-            "turku": scico.turku,
-            "turku_r": scico.turku_r,
-            "viridis": plt.get_cmap("viridis"),
-            "winter": plt.get_cmap("winter"),
-            "Wistia": plt.get_cmap("Wistia"),
-            "YlGn": plt.get_cmap("YlGn"),
-            "YlGnBu": plt.get_cmap("YlGnBu"),
-            "YlOrBr": plt.get_cmap("YlOrBr"),
-            "YlOrRd": plt.get_cmap("YlOrRd"),
-        },
-        "multi-sequential": {
-            "bukavu": scico.bukavu,
-            "fes": scico.fes,
-            "infinity": cmr.infinity,
-            "infinity_s": cmr.infinity_s,
-            "oleron": scico.oleron,
-            "topo": cmocean.cm.topo,
-        },
-        "circular": {
-            "bamo": scico.bamO,
-            "broco": scico.brocO,
-            "cet_c1": cc.cm.CET_C1,
-            "colorwheel": cc.cm.colorwheel,
-            "corko": scico.corkO,
-            "phase": cmocean.cm.phase,
-            "rainbow-iso": cc.cm.CET_I1,
-            "romao": scico.romaO,
-            "seasons": cmr.seasons,
-            "seasons_s": cmr.seasons_s,
-            "twilight": plt.get_cmap("twilight"),
-            "twilight_s": plt.get_cmap("twilight_shifted"),
-        },
-        "miscellaneous": {
-            "oxy": cmocean.cm.oxy,
-            "rainbow-kov": cc.cm.rainbow,
-            "turbo": plt.get_cmap("turbo"),
-        },
-        "qualitative": {
-            "538": ListedColormap(
-                [
-                    [0, 143 / 255, 213 / 255],
-                    [252 / 255, 79 / 255, 48 / 255],
-                    [229 / 255, 174 / 255, 56 / 255],
-                    [109 / 255, 144 / 255, 79 / 255],
-                    [139 / 255, 139 / 255, 139 / 255],
-                    [129 / 255, 15 / 255, 124 / 255],
-                ],
-                name="538",
-            ),
-            "bold": ListedColormap(Bold_10.mpl_colors, name="bold"),
-            "brewer": ListedColormap(Set1_9.mpl_colors, name="brewer"),
-            "colorblind": ListedColormap(
-                [
-                    [0.1, 0.1, 0.1],
-                    [230 / 255, 159 / 255, 0],
-                    [86 / 255, 180 / 255, 233 / 255],
-                    [0, 158 / 255, 115 / 255],
-                    [213 / 255, 94 / 255, 0],
-                    [0, 114 / 255, 178 / 255],
-                ],
-                name="colorblind",
-            ),
-            "glasbey": cc.cm.glasbey,
-            "glasbey_bw": cc.cm.glasbey_bw,
-            "glasbey_category10": cc.cm.glasbey_category10,
-            "glasbey_dark": cc.cm.glasbey_dark,
-            "glasbey_hv": cc.cm.glasbey_hv,
-            "glasbey_light": cc.cm.glasbey_light,
-            "pastel": ListedColormap(Pastel_10.mpl_colors, name="pastel"),
-            "prism": ListedColormap(Prism_10.mpl_colors, name="prism"),
-            "vivid": ListedColormap(Vivid_10.mpl_colors, name="vivid"),
-        },
-    }
-    return cmap_dict
-
-
-def get_available_ctype():
-    """return available the colormap type"""
-    return get_cmap_dict.keys()
-
-
-def plot_colormap(
-    ctype,
-    cmap_list="all",
-    figsize=None,
-    n_colors=10,
-    facecolor="black",
-    uniformize=True,
-    symmetrize=False,
-    unif_kwargs=None,
-    sym_kwargs=None,
-):
-    """
-    Plot the gradient of the corresponding color palette (or bar plot if qualitative)
-
-    :param ctype: str, default="sequential"
-        the color map type
-    :param cmap_list: list of string or 'all', default='all
-        list of color map names to draw
-    :param figsize: 2-uple of int
-        the figure size
-    :param n_colors: int, default=10
-        the number of colors to plot (e.g. 10 for qualitative and 256 for continuous)
-    :param facecolor: str
-        the chart face color. It should be a string of builtin matplotlib colors or a string
-        corresponding to a hex color.
-    :param uniformize: Boolean, default=True
-        uniformize or not the cmap before plotting
-    :param symmetrize: Boolean, default=False
-        symmetrize or not the cmap before plotting
-    :param unif_kwargs: dict or None
-        the kwargs for the uniformize_cmap method
-    :param sym_kwargs: dict or None
-        the kwargs for the symmetrize_cmap method
-    :return:
-    """
-    if sym_kwargs is None:
-        sym_kwargs = {}
-    if unif_kwargs is None:
-        unif_kwargs = {}
-
-    gradient = np.linspace(0, 1, n_colors)
-    gradient = np.vstack((gradient, gradient))
-
-    if cmap_list == "all":
-        cmap_list = list(SciCoMap(ctype=ctype).get_color_map_names())
-
-    nrows = len(cmap_list)
-
-    if figsize is None:
-        figsize = (10, 0.25 * nrows)
-
-    fontcolor = "white" if facecolor == "black" else "black"
-    font = {"color": fontcolor, "size": 16}
-    fig, axes = plt.subplots(nrows=nrows, figsize=figsize, facecolor=facecolor)
-    fig.subplots_adjust(top=0.95, bottom=0.01, left=0.2, right=0.99)
-    axes[0].set_title("Colormaps", fontdict=font)
-
-    for ax, name in zip(axes, cmap_list):
-
-        cmap = SciCoMap(ctype=ctype, cmap=name)
-
-        if uniformize:
-            cmap.uniformize_cmap(**unif_kwargs)
-        if symmetrize:
-            cmap.symmetrize_cmap(**sym_kwargs)
-
-        cmap = cmap.get_mpl_color_map()
-
-        if ctype == "qualitative":
-            col_map = cmap(range(10)) if cmap.N > 10 else cmap(range(cmap.N))
-            x = np.linspace(0, 1, len(col_map))
-            ax.bar(x, np.ones_like(x), color=col_map, width=1 / (len(col_map) - 1))
-        else:
-            ax.imshow(gradient, aspect="auto", cmap=cmap)
-
-        pos = list(ax.get_position().bounds)
-        x_text = pos[0] - 0.01
-        y_text = pos[1] + pos[3] / 2.0
-
-        font = {"color": fontcolor, "size": 12}
-        fig.text(x_text, y_text, name, va="center", ha="right", fontdict=font)
-
-    # Turn off *all* ticks & spines, not just the ones with colormaps.
-    for ax in axes:
-        ax.set_axis_off()
-    return fig
-
-
-def plot_colorblind_vision(
-    ctype="sequential",
-    cmap_list="all",
-    figsize=None,
-    n_colors=10,
-    facecolor="black",
-    uniformize=True,
-    symmetrize=False,
-    unif_kwargs=None,
-    sym_kwargs=None,
-):
-    """
-
-    Render the color map (adjusted or not) in different color deficiencies vision
-
-
-    :param ctype: str, default="sequential"
-        the color map type
-    :param cmap_list: list of string or 'all', default='all
-        list of color map names to draw
-    :param figsize: 2-uple of int
-        the figure size
-    :param n_colors: int, default=10
-        the number of colors to plot (e.g. 10 for qualitative and 256 for continuous)
-    :param facecolor: str
-        the chart face color. It should be a string of builtin matplotlib colors or a string
-        corresponding to a hex color.
-    :param uniformize: Boolean, default=True
-        uniformize or not the cmap before plotting
-    :param symmetrize: Boolean, default=False
-        symmetrize or not the cmap before plotting
-    :param unif_kwargs: dict or None
-        the kwargs for the uniformize_cmap method
-    :param sym_kwargs: dict or None
-        the kwargs for the symmetrize_cmap method
-    :return:
-    """
-    if sym_kwargs is None:
-        sym_kwargs = {}
-    if unif_kwargs is None:
-        unif_kwargs = {}
-    cm_list = []
-
-    if cmap_list == "all":
-        cmap_list = list(SciCoMap(ctype=ctype).get_color_map_names())
-
-    for name in cmap_list:
-        cmap = SciCoMap(ctype=ctype, cmap=name)
-        if uniformize:
-            cmap.uniformize_cmap(**unif_kwargs)
-        if symmetrize:
-            cmap.symmetrize_cmap(**sym_kwargs)
-        cmap = cmap.get_mpl_color_map()
-        cm_list.append(cmap)
-
-    return colorblind_vision(
-        cmap=cm_list, figsize=figsize, n_colors=n_colors, facecolor=facecolor
-    )
-
-
-def compare_cmap(
-    image="scan",
-    ctype="sequential",
-    cm_list=None,
-    ncols=3,
-    uniformize=True,
-    title=True,
-    symmetrize=False,
-    unif_kwargs=None,
-    sym_kwargs=None,
-    facecolor="black",
-    figsize=None,
-):
-    """
-    Utility function to visualize how the different color maps render the details and the information.
-    You can pass the image of your choice, like a topographic profile for sequential and sea-earth level for
-    diverging (negative and positive values) for instance.
-    Some are suited to a dark background and others for light backgrounds.
-
-    :param image: str or None
-        the path to the jpg or png picture you want to use for the comparison or one
-        of the builtin images as a pyramid image to visualize if there is any artifact
-    :param ctype: str,
-        either "sequential", "diverging", "qualitative"
-    :param cm_list: list of str or None
-        the list of cmaps you want to compare, if None all of them (for the chosen ctype) will be compared
-    :param ncols: int
-        the number of columns in the matplotlib subplot figure
-    :param uniformize: Boolean, default=True
-        uniformize or not the cmap before plotting
-    :param title: Boolean, default=True
-        display the cmap name as a title
-    :param symmetrize: Boolean, default=False
-        symmetrize or not the cmap before plotting
-    :param unif_kwargs: dict or None
-        the kwargs for the uniformize_cmap method
-    :param sym_kwargs: dict or None
-        the kwargs for the symmetrize_cmap method
-    :param facecolor: str
-        the chart face color. It should be a string of builtin matplotlib colors or a string
-        corresponding to a hex color.
-    :param figsize: tuple or None
-        the figure size
-
-    :return: f, matplotlib figure
-    """
-
-    if unif_kwargs is None:
-        unif_kwargs = {}
-    if sym_kwargs is None:
-        sym_kwargs = {}
-
-    if image is not None and not isinstance(image, str):
-        raise TypeError("image should be a string or a path to an existing file")
-
-    if (image is not None) and (image.endswith(("jpg", "jpeg", "png"))):
-        img = mpimg.imread(image)
-        lum_img = img[:, :, 0]
-    elif image == "pyramid":
-        lum_img = _pyramid()
-    elif image == "topography":
-        lum_img = load_hill_topography()
-    elif image == "fn_roots":
-        lum_img = _fn_with_roots()
-    elif image == "scan":
-        lum_img = load_scan_image()
-    elif image == "phase":
-        lum_img = _complex_phase()
-    elif image == "grmhd":
-        lum_img = load_pic(name=image)
-    elif image == "vortex":
-        lum_img = load_pic(name=image)
-    elif image == "tng":
-        lum_img = load_pic(name=image)
-    else:
-        lum_img = _pyramid()
-
-    if cm_list is None:
-        cm_list = list(SciCoMap(ctype=ctype).get_color_map_names())
-
-    nrows = int(np.ceil(len(cm_list) / ncols))
-    # delete non-used axes
-    n_charts = len(cm_list)
-    n_subplots = nrows * ncols
-
-    if figsize is None:
-        figsize = (2 * ncols, 2.5 * nrows)
-    f, axs = plt.subplots(
-        nrows=nrows,
-        ncols=ncols,
-        figsize=figsize,
-        # subplot_kw={"aspect": 1},
-        facecolor=facecolor,
-        # gridspec_kw={"hspace": 0.0, "wspace": 0.5},
-    )
-    # Make the axes accessible with single indexing
-    axs = axs.flatten()
-    fontcolor = "white" if facecolor == "black" else "black"
-
-    # loop over the columns to illustrate
-    for i, color_map in enumerate(cm_list):
-        # select the axis where the map will go
-        if n_charts > 1:
-            ax = axs[i]
-        else:
-            ax = axs
-
-        chartcm = SciCoMap(ctype=ctype, cmap=color_map)
-
-        if uniformize:
-            chartcm.uniformize_cmap(**unif_kwargs)
-        if symmetrize:
-            chartcm.symmetrize_cmap(**sym_kwargs)
-
-        ax.imshow(lum_img, cmap=chartcm.get_mpl_color_map())
-        if title:
-            ax.set_title(color_map, fontsize=16, color=fontcolor)
-        # Remove axis clutter
-        ax.set_axis_off()
-
-    if n_subplots > n_charts > 1:
-        for i in range(n_charts, n_subplots):
-            ax = axs[i]
-            ax.set_axis_off()
-
-    # Display the figure
-    # plt.tight_layout(pad=0, w_pad=0.5, h_pad=0)
-    h_space = 0.25 if title else 0.0
-    f.subplots_adjust(wspace=0.0, hspace=h_space)
-
-    return f
-
-
-def jch_plot(cmap, figsize=(12, 10)):
-    """
-    Stolen from the ehtplot package
-
-    Plot J', C', and h' of a colormap as function of the mapped value
-
-    The CAM02-UCS lightness J' should serve us as a good approximation for
-    generating perceptually uniform colormaps. In fact, linearity in J'
-    is used as the working definition of Perceptually Uniform Sequential
-    colormaps by matplotlib.
-
-    Hue h' can encode an additional physical quantity in an image
-    (when used in this way, the change of hue should be linearly
-    proportional to the quantity)
-
-    The other dimension chroma is less recognizable and should not be
-    used to encode physical information. Since sRGB is only a subset
-    of the Lab color space, there are human recognizable colors that
-    are not displayable. In order to accurately represent the physical
-    quantities.
-
-    :param cmap: string or matplotlib.colors.Colormap): The colormap to
-            be plotted.
-    :param figsize: 2-uple of int
-        the figure size
-    """
-    f = plt.figure(figsize=figsize)
-    c_maps, _ = _get_color_weak_cmap(cmap, n_images=2)
-    color_map, deuter50_cm, prot50_cm, deuter100_cm, trit100_cm = c_maps
-
-    title_str = cmap if isinstance(cmap, str) else cmap.name
-    f.suptitle(title_str, fontsize=24)
-
-    ax0 = f.add_subplot(2, 4, 1)
-    ax0 = _ax_cylinder_JCh(ax0, cmap, title="Normal (90-95%% of pop)")
-
-    ax2 = f.add_subplot(2, 4, 3)
-    ax2 = _ax_cylinder_JCh(ax2, deuter50_cm, title="Deuter-50%, RG-weak")
-
-    ax4 = f.add_subplot(2, 4, 7)
-    ax4 = _ax_cylinder_JCh(ax4, deuter100_cm, title="Deuter-100%, RG-blind")
-
-    ax6 = f.add_subplot(2, 4, 5)
-    ax6 = _ax_cylinder_JCh(ax6, trit100_cm, title="Trit-100%, BY deficient")
-
-    ax3d = f.add_subplot(2, 4, 2, projection="3d", elev=25, azim=-75)
-    ax3d = _ax_scatter_Jpapbp(ax3d, cmap, title="Normal (90-95%% of pop)")
-
-    ax3d2 = f.add_subplot(2, 4, 4, projection="3d", elev=25, azim=-75)
-    ax3d2 = _ax_scatter_Jpapbp(ax3d2, deuter50_cm, title="Deuter-50%, RG-weak")
-
-    ax3d3 = f.add_subplot(2, 4, 8, projection="3d", elev=25, azim=-75)
-    ax3d3 = _ax_scatter_Jpapbp(ax3d3, deuter100_cm, title="Deuter-100%, RG-blind")
-
-    ax3d4 = f.add_subplot(2, 4, 6, projection="3d", elev=25, azim=-75)
-    ax3d4 = _ax_scatter_Jpapbp(ax3d4, trit100_cm, title="Trit-100%, BY deficient")
-
-    plt.tight_layout()
-
-    return f
+"""
+Main module for scientific colormaps. It uses the CAM02-UCS color space
+Its three coordinates are usually denoted by J', a', and b' and its cylindrical coordinates are J', C', and h'.
+This package is built on matplotlib, colorspacious, viscm and EHTplot packages for
+the color mathematics and transformations and uses colormaps coming from different packages aiming
+to provide scientific colormaps but requiring some adjustments.
+
+- Provide sequential, multi-sequential, diverging, circular and qualitative (discrete) cmaps
+- Uniformize: linearize the CAM02-UCS lightness J'
+- Symmetrize: make the CAM02-UCS chroma C' symmetrical, bitonic or not, smooth or not
+- Get the matplotlib cmap object, before and after the adjustments
+- Charts to assess the quality of the colormaps (JCh plot)
+- Charts to assess the readability by colour weak/deficient/blind people
+- Charts for illustrating all the available colormaps
+
+The module structure is the following:
+---------------------------------------
+- ``SciCoMap`` Parent class for all the colormap types
+- ``ScicoSequential`` Child class for sequential colormaps
+- ``ScicoMultiSequential`` Child class for multi-sequential colormaps
+- ``ScicoDiverging`` Child class for diverging colormaps
+- ``ScicoCircular`` Child class for circular colormaps (circular diverging and circular flat aka phase)
+- ``ScicoMiscellaneous`` Child class for continuous colormaps which are none of the above
+- ``ScicoQualitative`` Child class for discrete colormaps
+- ``plot_colormap`` function for illustrating all the color maps of a given type
+- ``plot_colorblind_vision`` function for comparing the rendering with different color deficiencies
+- ``compare_cmap`` function for comparing the rendering when using an image.
+
+"""
+
+import matplotlib.pyplot as plt
+import matplotlib.image as mpimg
+from matplotlib.colors import Colormap, ListedColormap
+import numpy as np
+from scicomap.datasets import load_hill_topography, load_scan_image, load_pic
+from typing import List, Tuple, Union, Callable, Optional, Dict, Any
+
+# Scientific Colours
+import colorcet as cc
+import cmasher as cmr
+from cmcrameri import cm as scico
+import cmocean
+from palettable.cubehelix import perceptual_rainbow_16, classic_16
+from palettable.cartocolors.qualitative import Bold_10, Pastel_10, Prism_10, Vivid_10
+from palettable.colorbrewer.qualitative import Set1_9
+
+# internal import
+from scicomap.cmath import (
+    uniformize_cmap,
+    symmetrize_cmap,
+    unif_sym_cmap,
+    _ax_cylinder_JCh,
+    _ax_scatter_Jpapbp,
+)
+from scicomap.cblind import _get_color_weak_cmap, colorblind_vision
+from scicomap.utils import (
+    _pyramid,
+    _pyramid_zombie,
+    _fn_with_roots,
+    _periodic_fn,
+    _plot_examples,
+    _plot_examples_qual,
+    _complex_phase,
+)
+
+
+class SciCoMap:
+    """
+    Get a matplotlib-compatible colormap from different packages, mainly scientific color maps [1]_ [2]_ [3]_ [4]_
+
+    Parameters
+    ----------
+    ctype : str, optional
+        Color map type, one of {'sequential', 'multi-sequential', 'diverging',
+        'circular', 'miscellaneous', 'qualitative'}. Default is 'sequential'.
+    cmap : str or cmap object, optional
+        The name of the color map you want to use or the matplotlib cmap object.
+        Default is 'thermal'.
+
+    Attributes
+    ----------
+    color_map_dic : dict
+        The mapping dictionary for some colormaps.
+    ctype : str
+        Color map type, one of {'sequential', 'diverging', 'qualitative'}.
+    cname : str
+        The name of the color map.
+    cmap : matplotlib cmap or list of hex/rgb
+        The color map.
+    uniformized : bool
+        If the cmap has been uniformized or not.
+
+    Methods
+    -------
+    get_ctype()
+        Get the colormap type.
+    get_mpl_color_map()
+        Get the matplotlib colormap (cmap object).
+    uniformize_cmap(lift=None)
+        Uniformize the colormap (linearize the brightness J').
+    symmetrize_cmap(bitonic=True, diffuse=True)
+        Symmetrize the hue (h').
+    unif_sym_cmap(lift=None, bitonic=True, diffuse=True)
+        Uniformize and symmetrize at once.
+    get_color_map_names()
+        Get the name of all the available color maps.
+    get_color_map_dic()
+        Get the color maps dictionary.
+    assess_cmap(figsize=(18, 8))
+        Plot the Jch tensor to visualize the brightness (J'), the hue (h'), and the chroma (c').
+    illustrate_palettes(figsize=(12, 10), n_colors=256)
+        Plot the gradient or discrete palettes of all the colormaps of the given type.
+    colorblind(figsize=(12, 5), n_colors=256, facecolor="black")
+        Plot the gradient or barchart of the colormap for different kinds of color deficiencies.
+
+    Examples
+    --------
+    ccmap = SciCoMap(ctype='sequential', cmap='thermal')
+    mpl_map = ccmap.get_mpl_color_map()
+
+    References
+    ----------
+    [1] https://www.kennethmoreland.com/color-advice/
+    [2] https://mycarta.wordpress.com/2012/05/29/the-rainbow-is-dead-long-live-the-rainbow-series-outline/
+    [3] http://www.fabiocrameri.ch/colourmaps.php
+    [4] https://betterfigures.org/2015/06/23/picking-a-colour-scale-for-scientific-graphics/
+    """
+
+    def __init__(self, ctype: str = "sequential", cmap: Union[str, Colormap] = "thermal"):
+        self.ctype = ctype
+        self.color_map_dic = get_cmap_dict()
+        self.cmap = cmap
+        self.cname = "cmap"
+        self.uniformized = False
+
+    def __repr__(self):
+        s = f"SciCoMap(ctype={self.ctype}, cmap={self.cname})"
+        return s
+
+    @classmethod
+    def get_ctype(cls) -> List[str]:
+        """Return the colormap type."""
+        return list(get_cmap_dict().keys())
+
+    def get_mpl_color_map(self) -> Colormap:
+        """
+        Get the matplotlib colormap object.
+
+        Returns
+        -------
+        color_map : mpl colormap
+            The colormap object.
+        """
+        if isinstance(self.cmap, str):
+            if self.cmap not in self.color_map_dic[self.ctype].keys():
+                raise ValueError(
+                    f"Current built-in cmaps are: {self.color_map_dic[self.ctype].keys()}"
+                )
+            self.cname = self.cmap
+            self.cmap = self.color_map_dic[self.ctype][self.cmap]
+        else:
+            self.cname = self.cmap.name
+
+        return self.cmap
+
+    def uniformize_cmap(self, lift: Optional[int] = None):
+        """
+        Uniformize the colormap, meaning linearizing the brightness (J')
+        in the CAM02-UCS color space.
+
+        Parameters
+        ----------
+        lift : None or int in [0, 100], optional
+            Lift or not the darkest part of the colormap.
+
+        Returns
+        -------
+        None
+        """
+        self.get_mpl_color_map()
+        self.cmap, self.uniformized = uniformize_cmap(
+            cmap=self.cmap, name=self.cname, lift=lift, uniformized=self.uniformized
+        )
+
+    def symmetrize_cmap(self, bitonic: bool = True, diffuse: bool = True):
+        """
+        Symmetrize the colormap (the hue) in the CAM02-UCS color space.
+        It can be symmetrized in a bitonic way or not (if bitonic, the hue
+        curve will be symmetric with an extremum at its center).
+
+        The hue curve can be smoothed (diffuse) or not (edges might occur).
+
+        Parameters
+        ----------
+        bitonic : bool, optional (default=True)
+            Bitonic symmetrization or not (extremum located at the center of the hue curve).
+        diffuse : bool, optional (default=True)
+            Smooth hue curve or not (if not, edges might occur).
+
+        Returns
+        -------
+        None
+        """
+        self.get_mpl_color_map()
+        self.cmap = symmetrize_cmap(
+            cmap=self.cmap, name=self.cname, bitonic=bitonic, diffuse=diffuse
+        )
+
+    def unif_sym_cmap(
+        self, lift: Optional[int] = None, bitonic: bool = True, diffuse: bool = True
+    ):
+        """
+        First, uniformize the colormap, meaning linearizing the brightness (J')
+        in the CAM02-UCS color space.
+
+        Second, symmetrize the colormap (the hue) in the CAM02-UCS color space.
+        It can be symmetrized in a bitonic way or not (if bitonic, the hue
+        curve will be symmetric with an extremum at its center).
+
+        The hue curve can be smoothed (diffuse) or not (edges might occur).
+
+        Parameters
+        ----------
+        lift : None or int in [0, 100], optional
+            Lift or not the darkest part of the colormap.
+        bitonic : bool, optional (default=True)
+            Bitonic symmetrization or not (extremum located at the center of the hue curve).
+        diffuse : bool, optional (default=True)
+            Smooth hue curve or not (if not, edges might occur).
+
+        Returns
+        -------
+        None
+        """
+        self.get_mpl_color_map()
+        self.cmap, self.uniformized = unif_sym_cmap(
+            cmap=self.cmap,
+            name=self.cname,
+            lift=lift,
+            uniformized=self.uniformized,
+            bitonic=bitonic,
+            diffuse=diffuse,
+        )
+
+    def get_color_map_names(self) -> List[str]:
+        """
+        Get the names of the implemented colormaps for the chosen ctype.
+
+        Returns
+        -------
+        List of str
+            List of colormap names.
+        """
+        return list(self.color_map_dic[self.ctype].keys())
+
+    @classmethod
+    def get_color_map_dic(cls) -> dict:
+        """
+        Get the mapping dict of all the available color maps.
+
+        Returns
+        -------
+        dict
+            The dictionary of all the color maps for all ctypes.
+        """
+        return get_cmap_dict()
+
+    def assess_cmap(self, figsize: Tuple[int, int] = (18, 8)) -> plt.figure:
+        """
+        Plot J', C', and h' of a colormap as a function of the mapped value.
+
+        The CAM02-UCS lightness J' is linearized for generating perceptually uniform colormaps
+        (working definition of Perceptually Uniform Sequential colormaps by matplotlib).
+
+        Hue h' can encode an additional physical quantity in an image
+        (when used in this way, the change of hue should be linearly
+        proportional to the quantity).
+
+        The other dimension chroma is less recognizable and should not be
+        used to encode physical information. Since sRGB is only a subset
+        of the Lab color space, there are human recognizable colors that
+        are not displayable. In order to accurately represent the physical
+        quantities.
+
+        Parameters
+        ----------
+        figsize : 2-tuple of int, optional
+            The figure size.
+
+        Returns
+        -------
+        matplotlib.figure.Figure
+            The matplotlib figure object.
+        """
+        color_map = self.get_mpl_color_map()
+        return jch_plot(cmap=color_map, figsize=figsize)
+
+    def illustrate_palettes(
+        self, figsize: Tuple[int, int] = (12, 10), n_colors: int = 256, facecolor: str = "black"
+    ):
+        """
+        Draw the gradient or discrete color palettes for each colormap of the chosen ctype.
+
+        Parameters
+        ----------
+        figsize : 2-tuple of int, optional
+            The figure size.
+        n_colors : int, optional
+            The number of colors to plot (e.g., 10 for qualitative and 256 for continuous).
+        facecolor : str, optional
+            The chart face color. It should be a string of built-in matplotlib colors or a hex color.
+
+        Returns
+        -------
+        None
+        """
+        cmap_list = self.get_color_map_names()
+        ctype = self.ctype
+        plot_colormap(ctype, cmap_list, figsize, n_colors, facecolor)
+        plt.show()
+
+    def colorblind(
+        self, figsize: Tuple[int, int] = (12, 5), n_colors: int = 256, facecolor: str = "black"
+    ):
+        """
+        Draw the gradient or discrete color palettes for different kinds of color vision deficiencies.
+
+        Parameters
+        ----------
+        figsize : 2-tuple of int, optional
+            The figure size.
+        n_colors : int, optional
+            The number of colors to plot (e.g., 10 for qualitative and 256 for continuous).
+        facecolor : str, optional
+            The chart face color. It should be a string of built-in matplotlib colors or a hex color.
+
+        Returns
+        -------
+        None
+        """
+        plot_colorblind_vision(
+            ctype=self.ctype,
+            cmap_list=[self.get_mpl_color_map()],
+            figsize=figsize,
+            n_colors=n_colors,
+            facecolor=facecolor,
+        )
+
+class ScicoSequential(SciCoMap):
+    """
+    Get a matplotlib-compatible sequential color map from different packages providing scientific color maps [1]_ [2]_ [3]_ [4]_
+
+    Parameters
+    ----------
+    cmap : str or matplotlib colormap, optional
+        The name of the color map you want to use. Default is 'thermal'.
+
+    Attributes
+    ----------
+    color_map_dic : dict
+        The mapping dictionary for some colormaps.
+    ctype : str
+        Color map type, one of {'sequential', 'diverging', 'qualitative'}.
+    cname : str
+        The name of the color map.
+    cmap : matplotlib colormap or list of hex/rgb
+        The color map.
+
+    Methods
+    -------
+    get_mpl_color_map()
+        Get the matplotlib color map (or list of hex/rgb colors for qualitative).
+    get_color_map_names()
+        Get the name of all the available color maps.
+    get_color_map_dic()
+        Get the color maps dictionary.
+    illustrate_palettes()
+        Plot the gradient or the discrete palettes (all of them).
+    draw_example(facecolor="black")
+        Draw two charts for illustrative purposes.
+
+    Examples
+    --------
+    sc_map = ScicoSequential(cname='chroma')
+    mpl_map = sc_map.get_mpl_color_map()
+    sc_map.draw_example()
+
+    References
+    ----------
+    [1] https://www.kennethmoreland.com/color-advice/
+    [2] https://mycarta.wordpress.com/2012/05/29/the-rainbow-is-dead-long-live-the-rainbow-series-outline/
+    [3] http://www.fabiocrameri.ch/colourmaps.php
+    [4] https://betterfigures.org/2015/06/23/picking-a-colour-scale-for-scientific-graphics/
+    """
+
+    def __init__(self, cmap: Union[str, Colormap] = "thermal"):
+        super().__init__(cmap=cmap, ctype="sequential")
+
+    def __repr__(self):
+        s = f"ScicoSequential(cmap={self.cname})"
+        return s
+
+    def draw_example(self, facecolor: str = "black", figsize: tuple = (20, 20), cblind: bool = True):
+        """
+        Draw two charts for illustrative purposes.
+
+        Parameters
+        ----------
+        facecolor : str, optional
+            The chart face color. It should be a string of built-in matplotlib colors or a hex color.
+        figsize : tuple, optional
+            The figure size.
+        cblind : bool, optional
+            Whether to simulate color vision deficiencies.
+
+        Returns
+        -------
+        matplotlib.figure.Figure
+            The matplotlib figure object.
+        """
+        color_map = self.get_mpl_color_map()
+        elevation = load_hill_topography()
+        scan_im = load_scan_image()
+        xpyr, ypyr, zpyr = _pyramid()
+        per_x, per_z, per_z = _periodic_fn()
+        images = [elevation, scan_im, zpyr, "3D", per_z, "3D"]
+
+        fig = _plot_examples(
+            color_map=color_map,
+            images=images,
+            arr_3d=[(xpyr, ypyr, zpyr), (per_x, per_z, per_z)],
+            figsize=figsize,
+            facecolor=facecolor,
+            cname=self.cname,
+            cblind=cblind,
+        )
+
+        return fig
+
+class ScicoMultiSequential(SciCoMap):
+    """
+    Get a matplotlib-compatible sequential color map from different packages.
+    Useful for continuous values, for which there is no "centre" or mid-value.
+    Some are suited to a dark background, and others for light backgrounds.
+
+    Parameters
+    ----------
+    cmap : str or matplotlib colormap, optional
+        The name of the color map you want to use. Default is 'chroma'.
+
+    Attributes
+    ----------
+    color_map_dic : dict
+        The mapping dictionary for some colormaps.
+    ctype : str
+        Color map type, one of {'sequential', 'diverging', 'qualitative'}.
+    cname : str
+        The name of the color map.
+    cmap : matplotlib colormap or list of hex/rgb
+        The color map.
+
+    Methods
+    -------
+    get_mpl_color_map()
+        Get the matplotlib color map (or list of hex/rgb colors for qualitative).
+    get_color_map_names()
+        Get the name of all the available color maps.
+    get_color_map_dic()
+        Get the color maps dictionary.
+    illustrate_palettes()
+        Plot the gradient or the discrete palettes (all of them).
+    draw_example(facecolor="black")
+        Draw two charts for illustrative purposes.
+
+    Examples
+    --------
+    sc_map = ScicoMultiSequential(cname='chroma')
+    mpl_map = sc_map.get_mpl_color_map()
+    sc_map.draw_example()
+
+    References
+    ----------
+    [1] https://www.kennethmoreland.com/color-advice/
+    [2] https://mycarta.wordpress.com/2012/05/29/the-rainbow-is-dead-long-live-the-rainbow-series-outline/
+    [3] http://www.fabiocrameri.ch/colourmaps.php
+    [4] https://betterfigures.org/2015/06/23/picking-a-colour-scale-for-scientific-graphics/
+    """
+
+    def __init__(self, cmap: Union[str, Colormap] = "chroma"):
+        super().__init__(cmap=cmap, ctype="multi-sequential")
+
+    def __repr__(self):
+        s = f"ScicoMultiSequential(cmap={self.cname})"
+        return s
+
+    def draw_example(self, facecolor: str = "black", figsize: tuple = (20, 20), cblind: bool = True):
+        """
+        Draw two charts for illustrative purposes.
+
+        Parameters
+        ----------
+        facecolor : str, optional
+            The chart face color. It should be a string of built-in matplotlib colors or a hex color.
+        figsize : tuple, optional
+            The figure size.
+        cblind : bool, optional
+            Whether to simulate color vision deficiencies.
+
+        Returns
+        -------
+        matplotlib.figure.Figure
+            The matplotlib figure object.
+        """
+        color_map = self.get_mpl_color_map()
+        elevation = load_hill_topography()
+        scan_im = load_scan_image()
+        xpyr, ypyr, zpyr = _pyramid_zombie(stacked=True)
+        per_x, per_z, per_z = _periodic_fn()
+        images = [elevation, scan_im, zpyr, "3D", per_z, "3D"]
+
+        fig = _plot_examples(
+            color_map=color_map,
+            images=images,
+            arr_3d=[(xpyr, ypyr, zpyr), (per_x, per_z, per_z)],
+            figsize=figsize,
+            facecolor=facecolor,
+            cname=self.cname,
+            cblind=cblind,
+        )
+
+        return fig
+
+
+class ScicoDiverging(SciCoMap):
+    """
+    Get a matplotlib-compatible diverging color map from different packages.
+    Useful for continuous values with a "center" or mid-value.
+    Some are suited to dark backgrounds, and others for light backgrounds [1]_ [2]_ [3]_ [4]_
+
+    Parameters
+    ----------
+    cmap : str or matplotlib colormap, optional
+        The name of the color map you want to use. Default is 'wildfire'.
+
+    Attributes
+    ----------
+    color_map_dic : dict
+        The mapping dictionary for some colormaps.
+    ctype : str
+        Color map type, one of {'sequential', 'diverging', 'qualitative'}.
+    cname : str
+        The name of the color map.
+    cmap : matplotlib colormap or list of hex/rgb
+        The color map.
+
+    Methods
+    -------
+    get_mpl_color_map()
+        Get the matplotlib color map (or list of hex/rgb colors for qualitative).
+    get_color_map_names()
+        Get the name of all the available color maps.
+    get_color_map_dic()
+        Get the color maps dictionary.
+    illustrate_palettes()
+        Plot the gradient or the discrete palettes (all of them).
+    draw_example(facecolor="black")
+        Draw two charts for illustrative purposes.
+
+    Examples
+    --------
+    sc_map = ScicoDiverging(cname='redshift')
+    mpl_map = sc_map.get_mpl_color_map()
+    sc_map.draw_example()
+
+    References
+    ----------
+    [1] https://www.kennethmoreland.com/color-advice/
+    [2] https://mycarta.wordpress.com/2012/05/29/the-rainbow-is-dead-long-live-the-rainbow-series-outline/
+    [3] http://www.fabiocrameri.ch/colourmaps.php
+    [4] https://betterfigures.org/2015/06/23/picking-a-colour-scale-for-scientific-graphics/
+    """
+
+    def __init__(self, cmap: Union[str, Colormap] = "wildfire"):
+        super().__init__(cmap=cmap, ctype="diverging")
+
+    def __repr__(self):
+        s = f"ScicoDiverging(cmap={self.cname})"
+        return s
+
+    def draw_example(self, facecolor: str = "black", figsize: tuple = (20, 20)):
+        """
+        Draw two charts for illustrative purposes.
+
+        Parameters
+        ----------
+        facecolor : str, optional
+            The chart face color. It should be a string of built-in matplotlib colors or a hex color.
+        figsize : tuple, optional
+            The figure size.
+
+        Returns
+        -------
+        matplotlib.figure.Figure
+            The matplotlib figure object.
+        """
+        color_map = self.get_mpl_color_map()
+        # Create diverging image data
+        image_div = _fn_with_roots()
+        xpyr, ypyr, zpyr = _pyramid_zombie(stacked=False)
+        per_x, per_z, per_z = _periodic_fn()
+
+        images = [image_div, zpyr, "3D", per_z, "3D"]
+
+        fig = _plot_examples(
+            color_map=color_map,
+            images=images,
+            arr_3d=[(xpyr, ypyr, zpyr), (per_x, per_z, per_z)],
+            figsize=figsize,
+            facecolor=facecolor,
+            cname=self.cname,
+            norm=True,
+        )
+
+        return fig
+
+
+class ScicoCircular(SciCoMap):
+    """
+    Get a matplotlib-compatible circular color map from different packages.
+    Useful for angular values (circular "flat" as the phase cmap).
+    There is no "center" or mid-value for circular color maps.
+    Some are suited for dark backgrounds, and others for light backgrounds [1]_ [2]_ [3]_ [4]_
+
+    Parameters
+    ----------
+    cmap : str or matplotlib colormap, optional
+        The name of the color map you want to use. Default is 'colorwheel'.
+
+    Attributes
+    ----------
+    color_map_dic : dict
+        The mapping dictionary for some colormaps.
+    ctype : str
+        Color map type, one of {'sequential', 'diverging', 'qualitative'}.
+    cname : str
+        The name of the color map.
+    cmap : matplotlib colormap or list of hex/rgb
+        The color map.
+
+    Methods
+    -------
+    get_mpl_color_map()
+        Get the matplotlib color map (or list of hex/rgb colors for qualitative).
+    get_color_map_names()
+        Get the name of all the available color maps.
+    get_color_map_dic()
+        Get the color maps dictionary.
+    illustrate_palettes()
+        Plot the gradient or the discrete palettes (all of them).
+    draw_example(facecolor="black")
+        Draw two charts for illustrative purposes.
+
+    Examples
+    --------
+    sc_map = ScicoCircular(cname='colorwheel')
+    mpl_map = sc_map.get_mpl_color_map()
+    sc_map.draw_example()
+
+    References
+    ----------
+    [1] https://www.kennethmoreland.com/color-advice/
+    [2] https://mycarta.wordpress.com/2012/05/29/the-rainbow-is-dead-long-live-the-rainbow-series-outline/
+    [3] http://www.fabiocrameri.ch/colourmaps.php
+    [4] https://betterfigures.org/2015/06/23/picking-a-colour-scale-for-scientific-graphics/
+    """
+
+    def __init__(self, cmap: Union[str, Colormap] = "colorwheel"):
+        super().__init__(cmap=cmap, ctype="circular")
+
+    def __repr__(self):
+        s = f"ScicoCircular(cmap={self.cname})"
+        return s
+
+    def draw_example(self, facecolor: str = "black", figsize: tuple = (20, 20), cblind: bool = True):
+        """
+        Draw two charts for illustrative purposes.
+
+        Parameters
+        ----------
+        facecolor : str, optional
+            The chart face color. It should be a string of built-in matplotlib colors or a hex color.
+        figsize : tuple, optional
+            The figure size.
+        cblind : bool, optional
+            Plot the colorblind version. Default is True.
+
+        Returns
+        -------
+        matplotlib.figure.Figure
+            The matplotlib figure object.
+        """
+        color_map = self.get_mpl_color_map()
+        elevation = load_hill_topography()
+        scan_im = load_scan_image()
+        per_x, per_z, per_z = _periodic_fn()
+        images = [elevation, scan_im, "electric", "complex"]
+
+        fig = _plot_examples(
+            color_map=color_map,
+            images=images,
+            arr_3d=None,
+            figsize=figsize,
+            facecolor=facecolor,
+            cname=self.cname,
+            cblind=cblind,
+        )
+
+        return fig
+
+
+class ScicoMiscellaneous(SciCoMap):
+    """
+    Get a matplotlib-compatible sequential color map from different packages.
+    Useful for continuous values, for which there is no "center" or mid-value.
+    Some are suited for dark backgrounds, and others for light backgrounds [1]_ [2]_ [3]_ [4]_
+
+    Parameters
+    ----------
+    cmap : str or matplotlib colormap, optional
+        The name of the color map you want to use. Default is 'turbo'.
+
+    Attributes
+    ----------
+    color_map_dic : dict
+        The mapping dictionary for some colormaps.
+    ctype : str
+        Color map type, one of {'sequential', 'diverging', 'qualitative'}.
+    cname : str
+        The name of the color map.
+    cmap : matplotlib colormap or list of hex/rgb
+        The color map.
+
+    Methods
+    -------
+    get_mpl_color_map()
+        Get the matplotlib color map (or list of hex/rgb colors for qualitative).
+    get_color_map_names()
+        Get the name of all the available color maps.
+    get_color_map_dic()
+        Get the color maps dictionary.
+    illustrate_palettes()
+        Plot the gradient or the discrete palettes (all of them).
+    draw_example(facecolor="black")
+        Draw two charts for illustrative purposes.
+
+    Examples
+    --------
+    sc_map = ScicoSequential(cname='chroma')
+    mpl_map = sc_map.get_mpl_color_map()
+    sc_map.draw_example()
+
+    References
+    ----------
+    [1] https://www.kennethmoreland.com/color-advice/
+    [2] https://mycarta.wordpress.com/2012/05/29/the-rainbow-is-dead-long-live-the-rainbow-series-outline/
+    [3] http://www.fabiocrameri.ch/colourmaps.php
+    [4] https://betterfigures.org/2015/06/23/picking-a-colour-scale-for-scientific-graphics/
+    """
+
+    def __init__(self, cmap: Union[str, Colormap] = "turbo"):
+        super().__init__(cmap=cmap, ctype="miscellaneous")
+
+    def __repr__(self):
+        s = f"ScicoMiscellaneous(cmap={self.cname})"
+        return s
+
+    def draw_example(self, facecolor: str = "black", figsize: tuple = (20, 20)):
+        """
+        Draw two charts for illustrative purposes.
+
+        Parameters
+        ----------
+        facecolor : str, optional
+            The chart face color. It should be a string of built-in matplotlib colors or a hex color.
+        figsize : tuple, optional
+            The figure size.
+
+        Returns
+        -------
+        matplotlib.figure.Figure
+            The matplotlib figure object.
+        """
+        color_map = self.get_mpl_color_map()
+        image_div = _fn_with_roots()
+        xpyr, ypyr, zpyr = _pyramid_zombie(stacked=False)
+        per_x, per_z, per_z = _periodic_fn()
+
+        images = [image_div, zpyr, "3D", per_z, "3D"]
+
+        fig = _plot_examples(
+            color_map=color_map,
+            images=images,
+            arr_3d=[(xpyr, ypyr, zpyr), (per_x, per_z, per_z)],
+            figsize=figsize,
+            facecolor=facecolor,
+            cname=self.cname,
+            norm=True,
+        )
+
+        return fig
+
+
+class ScicoQualitative(SciCoMap):
+    """
+    Get a matplotlib-compatible qualitative list of colors from different packages.
+    Useful for discrete values or categorical variables.
+    Some are suited for dark backgrounds, and others for light backgrounds [1]_ [2]_ [3]_ [4]_
+
+    Parameters
+    ----------
+    cmap : str or matplotlib colormap, optional
+        The name of the color map you want to use. Default is 'glasbey_dark'.
+
+    Attributes
+    ----------
+    color_map_dic : dict
+        The mapping dictionary for some colormaps.
+    ctype : str
+        Color map type, one of {'sequential', 'diverging', 'qualitative'}.
+    cname : str
+        The name of the color map.
+    cmap : matplotlib colormap or list of hex/rgb
+        The color map.
+
+    Methods
+    -------
+    get_mpl_color_map()
+        Get the matplotlib color map (or list of hex/rgb colors for qualitative).
+    get_color_map_names()
+        Get the name of all the available color maps.
+    get_color_map_dic()
+        Get the color maps dictionary.
+    illustrate_palettes()
+        Plot the gradient or the discrete palettes (all of them).
+    draw_example(facecolor="black")
+        Draw two charts for illustrative purposes.
+
+    Examples
+    --------
+    sc_map = ScicoQualitative(cname='glasbey_dark')
+    mpl_map = sc_map.get_mpl_color_map()
+    sc_map.draw_example()
+
+    References
+    ----------
+    [1] https://www.kennethmoreland.com/color-advice/
+    [2] https://mycarta.wordpress.com/2012/05/29/the-rainbow-is-dead-long-live-the-rainbow-series-outline/
+    [3] http://www.fabiocrameri.ch/colourmaps.php
+    [4] https://betterfigures.org/2015/06/23/picking-a-colour-scale-for-scientific-graphics/
+    """
+
+    def __init__(self, cmap: Union[str, Colormap] = "glasbey_dark"):
+        super().__init__(cmap=cmap, ctype="qualitative")
+
+    def __repr__(self):
+        s = f"ScicoQualitative(cmap={self.cname})"
+        return s
+
+    def draw_example(self, facecolor: str = "black", figsize: tuple = (20, 20)):
+        """
+        Draw two charts for illustrative purposes.
+
+        Parameters
+        ----------
+        facecolor : str, optional
+            The chart face color. It should be a string of built-in matplotlib colors or a hex color.
+        figsize : tuple, optional
+            The figure size.
+
+        Returns
+        -------
+        matplotlib.figure.Figure
+            The matplotlib figure object.
+        """
+        color_map = self.get_mpl_color_map()
+
+        # data from United Nations World Population Prospects (Revision 2019)
+        # https://population.un.org/wpp/, license: CC BY 3.0 IGO
+        year = [1950, 1960, 1970, 1980, 1990, 2000, 2010, 2018]
+        population_by_continent = {
+            "africa": [228, 284, 365, 477, 631, 814, 1044, 1275],
+            "americas": [340, 425, 519, 619, 727, 840, 943, 1006],
+            "asia": [1394, 1686, 2120, 2625, 3202, 3714, 4169, 4560],
+            "europe": [220, 253, 276, 295, 310, 303, 294, 293],
+            "oceania": [12, 15, 19, 22, 26, 31, 36, 39],
+        }
+        x = np.linspace(0, 10)
+        # Fixing random state for reproducibility
+        np.random.seed(19680801)
+        noisy_trends = np.array(
+            [
+                np.sin(x) + x + np.random.randn(50),
+                np.sin(x) + 0.5 * x + np.random.randn(50),
+                np.sin(x) + 2 * x + np.random.randn(50),
+                np.sin(x) - 0.5 * x + np.random.randn(50),
+                np.sin(x) - 2 * x + np.random.randn(50),
+                np.sin(x) + np.random.randn(50),
+            ]
+        )
+        noisy_trends = noisy_trends.T
+
+        dict_arr = [population_by_continent, "scatter", noisy_trends]
+
+        return _plot_examples_qual(
+            color_map=color_map,
+            dict_arr=dict_arr,
+            figsize=figsize,
+            facecolor=facecolor,
+            cname=self.cname,
+            year=year,
+        )
+
+
+def get_cmap_dict() -> Dict[str, Dict[str, Any]]:
+    """
+    Get a dictionary of color maps organized by categories.
+
+    Returns
+    -------
+    dict
+        A nested dictionary containing various color maps categorized as 'diverging', 'sequential',
+        'multi-sequential', 'circular', 'miscellaneous', and 'qualitative'. Each category
+        contains a dictionary of color maps with their associated names.
+    """
+    cmap_dict = {
+        "diverging": {
+            "berlin": scico.berlin,
+            "bjy": cc.cm.bjy,
+            "bky": cc.cm.bky,
+            "BrBG": plt.get_cmap("BrBG"),
+            "broc": scico.broc,
+            "bwr": plt.get_cmap("bwr"),
+            "coolwarm": plt.get_cmap("coolwarm"),
+            "curl": cmocean.cm.curl,
+            "delta": cmocean.cm.delta,
+            "fusion": cmr.fusion,
+            "fusion_r": cmr.fusion_r,
+            "guppy": cmr.guppy,
+            "guppy_r": cmr.guppy_r,
+            "iceburn": cmr.iceburn,
+            "iceburn_r": cmr.iceburn_r,
+            "lisbon": scico.lisbon,
+            "PRGn": plt.get_cmap("PRGn"),
+            "PiYG": plt.get_cmap("PiYG"),
+            "pride": cmr.pride,
+            "pride_r": cmr.pride_r,
+            "PuOr": plt.get_cmap("PuOr"),
+            "RdBu": plt.get_cmap("RdBu"),
+            "RdGy": plt.get_cmap("RdGy"),
+            "RdYlBu": plt.get_cmap("RdYlBu"),
+            "RdYlGn": plt.get_cmap("RdYlGn"),
+            "redshift": cmr.redshift,
+            "redshift_r": cmr.redshift_r,
+            "roma": scico.roma,
+            "seasons_r": cmr.seasons_r,
+            "seismic": plt.get_cmap("seismic"),
+            "spectral": plt.get_cmap("Spectral"),
+            "turbo": plt.get_cmap("turbo"),
+            "vanimo": scico.vanimo,
+            "vik": scico.vik,
+            "viola": cmr.viola,
+            "viola_r": cmr.viola_r,
+            "waterlily": cmr.waterlily,
+            "waterlily_r": cmr.waterlily_r,
+            "watermelon": cmr.watermelon,
+            "watermelon_r": cmr.watermelon_r,
+            "wildfire": cmr.wildfire,
+            "wildfire_r": cmr.wildfire_r,
+        },
+        "sequential": {
+            "afmhot": plt.get_cmap("afmhot"),
+            "amber": cmr.amber,
+            "amber_r": cmr.amber_r,
+            "amp": cmocean.cm.amp,
+            "apple": cmr.apple,
+            "apple_r": cmr.apple_r,
+            "autumn": plt.get_cmap("autumn"),
+            "batlow": scico.batlow,
+            "bilbao": scico.bilbao,
+            "bilbao_r": scico.bilbao_r,
+            "binary": plt.get_cmap("binary"),
+            "Blues": plt.get_cmap("Blues"),
+            "bone": plt.get_cmap("bone"),
+            "BuGn": plt.get_cmap("BuGn"),
+            "BuPu": plt.get_cmap("BuPu"),
+            "chroma": cmr.chroma,
+            "chroma_r": cmr.chroma_r,
+            "cividis": plt.get_cmap("cividis"),
+            "cool": plt.get_cmap("cool"),
+            "copper": plt.get_cmap("copper"),
+            "cosmic": cmr.cosmic,
+            "cosmic_r": cmr.cosmic_r,
+            "deep": cmocean.cm.deep,
+            "dense": cmocean.cm.dense,
+            "dusk": cmr.dusk,
+            "dusk_r": cmr.dusk_r,
+            "eclipse": cmr.eclipse,
+            "eclipse_r": cmr.eclipse_r,
+            "ember": cmr.ember,
+            "ember_r": cmr.ember_r,
+            "fall": cmr.fall,
+            "fall_r": cmr.fall_r,
+            "gem": cmr.gem,
+            "gem_r": cmr.gem_r,
+            "gist_gray": plt.get_cmap("gist_gray"),
+            "gist_heat": plt.get_cmap("gist_heat"),
+            "gist_yarg": plt.get_cmap("gist_yarg"),
+            "GnBu": plt.get_cmap("GnBu"),
+            "Greens": plt.get_cmap("Greens"),
+            "gray": plt.get_cmap("gray"),
+            "Greys": plt.get_cmap("Greys"),
+            "haline": cmocean.cm.haline,
+            "hawaii": scico.hawaii,
+            "hawaii_r": scico.hawaii,
+            "heat": cmr.torch,
+            "heat_r": cmr.torch_r,
+            "hot": plt.get_cmap("hot"),
+            "ice": cmocean.cm.ice,
+            "inferno": plt.get_cmap("inferno"),
+            "imola": scico.imola,
+            "imola_r": scico.imola_r,
+            "lapaz": scico.lapaz,
+            "lapaz_r": scico.lapaz_r,
+            "magma": plt.get_cmap("magma"),
+            "matter": cmocean.cm.matter,
+            "neon": cmr.neon,
+            "neon_r": cmr.neon_r,
+            "neutral": cmr.neutral,
+            "neutral_r": cmr.neutral_r,
+            "nuuk": scico.nuuk,
+            "nuuk_r": scico.nuuk,
+            "ocean": cmr.ocean,
+            "ocean_r": cmr.ocean_r,
+            "OrRd": plt.get_cmap("OrRd"),
+            "Oranges": plt.get_cmap("Oranges"),
+            "pink": plt.get_cmap("pink"),
+            "plasma": plt.get_cmap("plasma"),
+            "PuBu": plt.get_cmap("PuBu"),
+            "PuBuGn": plt.get_cmap("PuBuGn"),
+            "PuRd": plt.get_cmap("PuRd"),
+            "Purples": plt.get_cmap("Purples"),
+            "rain": cmocean.cm.rain,
+            "rainbow": perceptual_rainbow_16.mpl_colormap,
+            "rainbow-sc": scico.batlow,
+            "rainbow-sc_r": scico.batlow_r,
+            "rainforest": cmr.rainforest,
+            "rainforest_r": cmr.rainforest_r,
+            "RdPu": plt.get_cmap("RdPu"),
+            "Reds": plt.get_cmap("Reds"),
+            "savanna": cmr.savanna,
+            "savanna_r": cmr.savanna_r,
+            "sepia": cmr.sepia,
+            "sepia_r": cmr.sepia_r,
+            "speed": cmocean.cm.speed,
+            "solar": cmocean.cm.solar,
+            "spring": plt.get_cmap("spring"),
+            "summer": plt.get_cmap("summer"),
+            "tempo": cmocean.cm.tempo,
+            "thermal": cmocean.cm.thermal,
+            "thermal_r": cmocean.cm.thermal_r,
+            "thermal-2": cc.cm.bmy,
+            "tokyo": scico.tokyo,
+            "tokyo_r": scico.tokyo_r,
+            "tropical": cmr.tropical,
+            "tropical_r": cmr.tropical_r,
+            "turbid": cmocean.cm.turbid,
+            "turku": scico.turku,
+            "turku_r": scico.turku_r,
+            "viridis": plt.get_cmap("viridis"),
+            "winter": plt.get_cmap("winter"),
+            "Wistia": plt.get_cmap("Wistia"),
+            "YlGn": plt.get_cmap("YlGn"),
+            "YlGnBu": plt.get_cmap("YlGnBu"),
+            "YlOrBr": plt.get_cmap("YlOrBr"),
+            "YlOrRd": plt.get_cmap("YlOrRd"),
+        },
+        "multi-sequential": {
+            "bukavu": scico.bukavu,
+            "fes": scico.fes,
+            "infinity": cmr.infinity,
+            "infinity_s": cmr.infinity_s,
+            "oleron": scico.oleron,
+            "topo": cmocean.cm.topo,
+        },
+        "circular": {
+            "bamo": scico.bamO,
+            "broco": scico.brocO,
+            "cet_c1": cc.cm.CET_C1,
+            "colorwheel": cc.cm.colorwheel,
+            "corko": scico.corkO,
+            "phase": cmocean.cm.phase,
+            "rainbow-iso": cc.cm.CET_I1,
+            "romao": scico.romaO,
+            "seasons": cmr.seasons,
+            "seasons_s": cmr.seasons_s,
+            "twilight": plt.get_cmap("twilight"),
+            "twilight_s": plt.get_cmap("twilight_shifted"),
+        },
+        "miscellaneous": {
+            "oxy": cmocean.cm.oxy,
+            "rainbow-kov": cc.cm.rainbow,
+            "turbo": plt.get_cmap("turbo"),
+        },
+        "qualitative": {
+            "538": ListedColormap(
+                [
+                    [0, 143 / 255, 213 / 255],
+                    [252 / 255, 79 / 255, 48 / 255],
+                    [229 / 255, 174 / 255, 56 / 255],
+                    [109 / 255, 144 / 255, 79 / 255],
+                    [139 / 255, 139 / 255, 139 / 255],
+                    [129 / 255, 15 / 255, 124 / 255],
+                ],
+                name="538",
+            ),
+            "bold": ListedColormap(Bold_10.mpl_colors, name="bold"),
+            "brewer": ListedColormap(Set1_9.mpl_colors, name="brewer"),
+            "colorblind": ListedColormap(
+                [
+                    [0.1, 0.1, 0.1],
+                    [230 / 255, 159 / 255, 0],
+                    [86 / 255, 180 / 255, 233 / 255],
+                    [0, 158 / 255, 115 / 255],
+                    [213 / 255, 94 / 255, 0],
+                    [0, 114 / 255, 178 / 255],
+                ],
+                name="colorblind",
+            ),
+            "glasbey": cc.cm.glasbey,
+            "glasbey_bw": cc.cm.glasbey_bw,
+            "glasbey_category10": cc.cm.glasbey_category10,
+            "glasbey_dark": cc.cm.glasbey_dark,
+            "glasbey_hv": cc.cm.glasbey_hv,
+            "glasbey_light": cc.cm.glasbey_light,
+            "pastel": ListedColormap(Pastel_10.mpl_colors, name="pastel"),
+            "prism": ListedColormap(Prism_10.mpl_colors, name="prism"),
+            "vivid": ListedColormap(Vivid_10.mpl_colors, name="vivid"),
+        },
+    }
+    return cmap_dict
+
+
+def get_available_ctype():
+    """return available the colormap type"""
+    return get_cmap_dict.keys()
+
+
+def plot_colormap(
+    ctype,
+    cmap_list="all",
+    figsize=None,
+    n_colors=10,
+    facecolor="black",
+    uniformize=True,
+    symmetrize=False,
+    unif_kwargs=None,
+    sym_kwargs=None,
+):
+    """
+    Plot the gradient of the corresponding color palette (or bar plot if qualitative)
+
+    :param ctype: str, default="sequential"
+        the color map type
+    :param cmap_list: list of string or 'all', default='all
+        list of color map names to draw
+    :param figsize: 2-uple of int
+        the figure size
+    :param n_colors: int, default=10
+        the number of colors to plot (e.g. 10 for qualitative and 256 for continuous)
+    :param facecolor: str
+        the chart face color. It should be a string of builtin matplotlib colors or a string
+        corresponding to a hex color.
+    :param uniformize: Boolean, default=True
+        uniformize or not the cmap before plotting
+    :param symmetrize: Boolean, default=False
+        symmetrize or not the cmap before plotting
+    :param unif_kwargs: dict or None
+        the kwargs for the uniformize_cmap method
+    :param sym_kwargs: dict or None
+        the kwargs for the symmetrize_cmap method
+    :return:
+    """
+    if sym_kwargs is None:
+        sym_kwargs = {}
+    if unif_kwargs is None:
+        unif_kwargs = {}
+
+    gradient = np.linspace(0, 1, n_colors)
+    gradient = np.vstack((gradient, gradient))
+
+    if cmap_list == "all":
+        cmap_list = list(SciCoMap(ctype=ctype).get_color_map_names())
+
+    nrows = len(cmap_list)
+
+    if figsize is None:
+        figsize = (10, 0.25 * nrows)
+
+    fontcolor = "white" if facecolor == "black" else "black"
+    font = {"color": fontcolor, "size": 16}
+    fig, axes = plt.subplots(nrows=nrows, figsize=figsize, facecolor=facecolor)
+    fig.subplots_adjust(top=0.95, bottom=0.01, left=0.2, right=0.99)
+    axes[0].set_title("Colormaps", fontdict=font)
+
+    for ax, name in zip(axes, cmap_list):
+
+        cmap = SciCoMap(ctype=ctype, cmap=name)
+
+        if uniformize:
+            cmap.uniformize_cmap(**unif_kwargs)
+        if symmetrize:
+            cmap.symmetrize_cmap(**sym_kwargs)
+
+        cmap = cmap.get_mpl_color_map()
+
+        if ctype == "qualitative":
+            col_map = cmap(range(10)) if cmap.N > 10 else cmap(range(cmap.N))
+            x = np.linspace(0, 1, len(col_map))
+            ax.bar(x, np.ones_like(x), color=col_map, width=1 / (len(col_map) - 1))
+        else:
+            ax.imshow(gradient, aspect="auto", cmap=cmap)
+
+        pos = list(ax.get_position().bounds)
+        x_text = pos[0] - 0.01
+        y_text = pos[1] + pos[3] / 2.0
+
+        font = {"color": fontcolor, "size": 12}
+        fig.text(x_text, y_text, name, va="center", ha="right", fontdict=font)
+
+    # Turn off *all* ticks & spines, not just the ones with colormaps.
+    for ax in axes:
+        ax.set_axis_off()
+    return fig
+
+
+def plot_colorblind_vision(
+    ctype="sequential",
+    cmap_list="all",
+    figsize=None,
+    n_colors=10,
+    facecolor="black",
+    uniformize=True,
+    symmetrize=False,
+    unif_kwargs=None,
+    sym_kwargs=None,
+):
+    """
+
+    Render the color map (adjusted or not) in different color deficiencies vision
+
+
+    :param ctype: str, default="sequential"
+        the color map type
+    :param cmap_list: list of string or 'all', default='all
+        list of color map names to draw
+    :param figsize: 2-uple of int
+        the figure size
+    :param n_colors: int, default=10
+        the number of colors to plot (e.g. 10 for qualitative and 256 for continuous)
+    :param facecolor: str
+        the chart face color. It should be a string of builtin matplotlib colors or a string
+        corresponding to a hex color.
+    :param uniformize: Boolean, default=True
+        uniformize or not the cmap before plotting
+    :param symmetrize: Boolean, default=False
+        symmetrize or not the cmap before plotting
+    :param unif_kwargs: dict or None
+        the kwargs for the uniformize_cmap method
+    :param sym_kwargs: dict or None
+        the kwargs for the symmetrize_cmap method
+    :return:
+    """
+    if sym_kwargs is None:
+        sym_kwargs = {}
+    if unif_kwargs is None:
+        unif_kwargs = {}
+    cm_list = []
+
+    if cmap_list == "all":
+        cmap_list = list(SciCoMap(ctype=ctype).get_color_map_names())
+
+    for name in cmap_list:
+        cmap = SciCoMap(ctype=ctype, cmap=name)
+        if uniformize:
+            cmap.uniformize_cmap(**unif_kwargs)
+        if symmetrize:
+            cmap.symmetrize_cmap(**sym_kwargs)
+        cmap = cmap.get_mpl_color_map()
+        cm_list.append(cmap)
+
+    return colorblind_vision(
+        cmap=cm_list, figsize=figsize, n_colors=n_colors, facecolor=facecolor
+    )
+
+
+def compare_cmap(
+    image="scan",
+    ctype="sequential",
+    cm_list=None,
+    ncols=3,
+    uniformize=True,
+    title=True,
+    symmetrize=False,
+    unif_kwargs=None,
+    sym_kwargs=None,
+    facecolor="black",
+    figsize=None,
+):
+    """
+    Utility function to visualize how the different color maps render the details and the information.
+    You can pass the image of your choice, like a topographic profile for sequential and sea-earth level for
+    diverging (negative and positive values) for instance.
+    Some are suited to a dark background and others for light backgrounds.
+
+    :param image: str or None
+        the path to the jpg or png picture you want to use for the comparison or one
+        of the builtin images as a pyramid image to visualize if there is any artifact
+    :param ctype: str,
+        either "sequential", "diverging", "qualitative"
+    :param cm_list: list of str or None
+        the list of cmaps you want to compare, if None all of them (for the chosen ctype) will be compared
+    :param ncols: int
+        the number of columns in the matplotlib subplot figure
+    :param uniformize: Boolean, default=True
+        uniformize or not the cmap before plotting
+    :param title: Boolean, default=True
+        display the cmap name as a title
+    :param symmetrize: Boolean, default=False
+        symmetrize or not the cmap before plotting
+    :param unif_kwargs: dict or None
+        the kwargs for the uniformize_cmap method
+    :param sym_kwargs: dict or None
+        the kwargs for the symmetrize_cmap method
+    :param facecolor: str
+        the chart face color. It should be a string of builtin matplotlib colors or a string
+        corresponding to a hex color.
+    :param figsize: tuple or None
+        the figure size
+
+    :return: f, matplotlib figure
+    """
+
+    if unif_kwargs is None:
+        unif_kwargs = {}
+    if sym_kwargs is None:
+        sym_kwargs = {}
+
+    if image is not None and not isinstance(image, str):
+        raise TypeError("image should be a string or a path to an existing file")
+
+    if (image is not None) and (image.endswith(("jpg", "jpeg", "png"))):
+        img = mpimg.imread(image)
+        lum_img = img[:, :, 0]
+    elif image == "pyramid":
+        lum_img = _pyramid()
+    elif image == "topography":
+        lum_img = load_hill_topography()
+    elif image == "fn_roots":
+        lum_img = _fn_with_roots()
+    elif image == "scan":
+        lum_img = load_scan_image()
+    elif image == "phase":
+        lum_img = _complex_phase()
+    elif image == "grmhd":
+        lum_img = load_pic(name=image)
+    elif image == "vortex":
+        lum_img = load_pic(name=image)
+    elif image == "tng":
+        lum_img = load_pic(name=image)
+    else:
+        lum_img = _pyramid()
+
+    if cm_list is None:
+        cm_list = list(SciCoMap(ctype=ctype).get_color_map_names())
+
+    nrows = int(np.ceil(len(cm_list) / ncols))
+    # delete non-used axes
+    n_charts = len(cm_list)
+    n_subplots = nrows * ncols
+
+    if figsize is None:
+        figsize = (2 * ncols, 2.5 * nrows)
+    f, axs = plt.subplots(
+        nrows=nrows,
+        ncols=ncols,
+        figsize=figsize,
+        # subplot_kw={"aspect": 1},
+        facecolor=facecolor,
+        # gridspec_kw={"hspace": 0.0, "wspace": 0.5},
+    )
+    # Make the axes accessible with single indexing
+    axs = axs.flatten()
+    fontcolor = "white" if facecolor == "black" else "black"
+
+    # loop over the columns to illustrate
+    for i, color_map in enumerate(cm_list):
+        # select the axis where the map will go
+        if n_charts > 1:
+            ax = axs[i]
+        else:
+            ax = axs
+
+        chartcm = SciCoMap(ctype=ctype, cmap=color_map)
+
+        if uniformize:
+            chartcm.uniformize_cmap(**unif_kwargs)
+        if symmetrize:
+            chartcm.symmetrize_cmap(**sym_kwargs)
+
+        ax.imshow(lum_img, cmap=chartcm.get_mpl_color_map())
+        if title:
+            ax.set_title(color_map, fontsize=16, color=fontcolor)
+        # Remove axis clutter
+        ax.set_axis_off()
+
+    if n_subplots > n_charts > 1:
+        for i in range(n_charts, n_subplots):
+            ax = axs[i]
+            ax.set_axis_off()
+
+    # Display the figure
+    # plt.tight_layout(pad=0, w_pad=0.5, h_pad=0)
+    h_space = 0.25 if title else 0.0
+    f.subplots_adjust(wspace=0.0, hspace=h_space)
+
+    return f
+
+
+def jch_plot(cmap, figsize=(12, 10)):
+    """
+    Stolen from the ehtplot package
+
+    Plot J', C', and h' of a colormap as function of the mapped value
+
+    The CAM02-UCS lightness J' should serve us as a good approximation for
+    generating perceptually uniform colormaps. In fact, linearity in J'
+    is used as the working definition of Perceptually Uniform Sequential
+    colormaps by matplotlib.
+
+    Hue h' can encode an additional physical quantity in an image
+    (when used in this way, the change of hue should be linearly
+    proportional to the quantity)
+
+    The other dimension chroma is less recognizable and should not be
+    used to encode physical information. Since sRGB is only a subset
+    of the Lab color space, there are human recognizable colors that
+    are not displayable. In order to accurately represent the physical
+    quantities.
+
+    :param cmap: string or matplotlib.colors.Colormap): The colormap to
+            be plotted.
+    :param figsize: 2-uple of int
+        the figure size
+    """
+    f = plt.figure(figsize=figsize)
+    c_maps, _ = _get_color_weak_cmap(cmap, n_images=2)
+    color_map, deuter50_cm, prot50_cm, deuter100_cm, trit100_cm = c_maps
+
+    title_str = cmap if isinstance(cmap, str) else cmap.name
+    f.suptitle(title_str, fontsize=24)
+
+    ax0 = f.add_subplot(2, 4, 1)
+    ax0 = _ax_cylinder_JCh(ax0, cmap, title="Normal (90-95%% of pop)")
+
+    ax2 = f.add_subplot(2, 4, 3)
+    ax2 = _ax_cylinder_JCh(ax2, deuter50_cm, title="Deuter-50%, RG-weak")
+
+    ax4 = f.add_subplot(2, 4, 7)
+    ax4 = _ax_cylinder_JCh(ax4, deuter100_cm, title="Deuter-100%, RG-blind")
+
+    ax6 = f.add_subplot(2, 4, 5)
+    ax6 = _ax_cylinder_JCh(ax6, trit100_cm, title="Trit-100%, BY deficient")
+
+    ax3d = f.add_subplot(2, 4, 2, projection="3d", elev=25, azim=-75)
+    ax3d = _ax_scatter_Jpapbp(ax3d, cmap, title="Normal (90-95%% of pop)")
+
+    ax3d2 = f.add_subplot(2, 4, 4, projection="3d", elev=25, azim=-75)
+    ax3d2 = _ax_scatter_Jpapbp(ax3d2, deuter50_cm, title="Deuter-50%, RG-weak")
+
+    ax3d3 = f.add_subplot(2, 4, 8, projection="3d", elev=25, azim=-75)
+    ax3d3 = _ax_scatter_Jpapbp(ax3d3, deuter100_cm, title="Deuter-100%, RG-blind")
+
+    ax3d4 = f.add_subplot(2, 4, 6, projection="3d", elev=25, azim=-75)
+    ax3d4 = _ax_scatter_Jpapbp(ax3d4, trit100_cm, title="Trit-100%, BY deficient")
+
+    plt.tight_layout()
+
+    return f
```

### Comparing `scicomap-1.0.0/src/scicomap/utils.py` & `scicomap-1.0.1/src/scicomap/utils.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,292 +1,292 @@
-import itertools
-import numpy as np
-import matplotlib as mpl
-import matplotlib.pyplot as plt
-import matplotlib.image as mpimg
-from matplotlib.colors import ListedColormap
-from matplotlib.patches import Circle
-from mpl_toolkits.axes_grid1 import make_axes_locatable
-from os.path import dirname, join
-
-# internal import
-from scicomap.cblind import _get_color_weak_ctab, _get_color_weak_cmap
-
-
-
-def _pyramid(n=513):
-    """Create a pyramid function"""
-    s = np.linspace(-1.0, 1.0, n)
-    x, y = np.meshgrid(s, s)
-    z = 1.0 - np.maximum(abs(x), abs(y))
-    return x, y, z
-
-
-def _pyramid_zombie(n=513, stacked=False):
-    """Create a pyramid and its zombie copy (buried pyramid)"""
-    # image plot
-    s_y = np.linspace(-1.0, 1.0, n)
-    x, y = np.meshgrid(s_y, s_y)
-    z = 1.0 - np.maximum(abs(x), abs(y))
-    z = np.hstack((z, z - 1)) if stacked else np.hstack((z, -z))
-    # 3d plot
-    s_x = np.linspace(-1.0, 3.0, 2 * n)
-    s_y = np.linspace(-1.0, 1.0, n)
-    x, y = np.meshgrid(s_x, s_y)
-    return x, y, z
-
-
-def _periodic_fn():
-    """Create a periodic function with a step function"""
-    dx = dy = 0.05
-    y, x = np.mgrid[-5 : 5 + dy : dy, -5 : 10 + dx : dx]
-    z = (
-        np.sin(x) ** 10
-        + np.cos(10 + y * x)
-        + np.cos(x)
-        + 0.2 * y
-        + 0.1 * x
-        + np.heaviside(x, 1) * np.heaviside(y, 1)
-    )
-    z = z - np.mean(z)
-    return x, y, z
-
-
-def _fn_with_roots(n=250):
-    """Create a function with roots, for diverging colormaps"""
-    x, y = np.meshgrid(np.linspace(-3, 3, n), np.linspace(-2, 2, n))
-    return (1 - x / 2 + x**5 + y**3) * np.exp(-(x**2) - y**2)
-
-
-def _complex_phase(n=100):
-    """argument of a function in the complex plane, cyclic colormaps"""
-    x, y = np.ogrid[-3 : 3 : n * 1j, -3 : 3 : n * 1j]
-    z = x + 1j * y
-    # w = (z ** 2 - 1) * (z - 2 - 1j) ** 2 / (z ** 2 + 2 + 2j)
-    w = (z**2 - 1) * (z - 2 - 1j) ** 2
-    return np.angle(w)
-
-
-def _plot_complex_arg(ax, cmap, facecolor="black", title=False):
-    """Create mlp ax of the complex argument"""
-    arg_z = _complex_phase(n=100)
-    title_color = "white" if facecolor == "black" else "black"
-    ang = ax.imshow(np.degrees(arg_z), extent=[-2, 2, -2, 2], cmap=cmap)
-
-    ax.set_xlim(-2, 2)
-    ax.set_ylim(-2, 2)
-    ax.set_aspect("equal")
-    if title:
-        ax.set_xlabel("Re", color=title_color, fontsize=12)
-        ax.set_ylabel("Im", color=title_color, fontsize=12)
-        ax.set_title(
-            r"Argument of $(z^2 - 1)(z - 2 - j)^2$", color=title_color, fontsize=14
-        )
-
-    divider = make_axes_locatable(ax)
-    cax = divider.append_axes("right", size="5%", pad=0.05)
-    cax.yaxis.label.set_color(title_color)
-    cax.tick_params(axis="y", colors=title_color)
-    plt.colorbar(ang, cax=cax)
-    return ax
-
-
-def _E(q, r0, x, y):
-    """Return the electric field vector E=(Ex,Ey) due to charge q at r0."""
-    den = np.hypot(x - r0[0], y - r0[1]) ** 3
-    return q * (x - r0[0]) / den, q * (y - r0[1]) / den
-
-
-def _angle_E(n_neg_charges):
-    """Create the angle of the electric field with the x-axis"""
-    # Grid of x, y points
-    nx, ny = 64, 64
-    x = np.linspace(-2, 2, nx)
-    y = np.linspace(-2, 2, ny)
-    X, Y = np.meshgrid(x, y)
-
-    # Create a multipole with nq charges of alternating sign, equally spaced
-    # on the unit circle.
-    nq = 2 ** int(n_neg_charges)
-    charges = []
-    for i in range(nq):
-        q = i % 2 * 2 - 1
-        charges.append((q, (np.cos(2 * np.pi * i / nq), np.sin(2 * np.pi * i / nq))))
-
-    # Electric field vector, E=(Ex, Ey), as separate components
-    Ex, Ey = np.zeros((ny, nx)), np.zeros((ny, nx))
-    for charge in charges:
-        ex, ey = _E(*charge, x=X, y=Y)
-        Ex += ex
-        Ey += ey
-
-    # angle wrt to 1_x
-    cos_th = Ex / np.hypot(Ex, Ey)
-    return np.degrees(np.arccos(cos_th)), charges, x, y, Ex, Ey
-
-
-def _plot_e_field(ax, cmap, n_neg_charges=2, facecolor="black", title=False):
-    """Create the mpl ax of the electric field"""
-    title_color = "white" if facecolor == "black" else "black"
-
-    th_deg, charges, x, y, Ex, Ey = _angle_E(n_neg_charges)
-
-    # Plot the streamlines with an appropriate colormap and arrow style
-    ax.streamplot(
-        x,
-        y,
-        Ex,
-        Ey,
-        color="black",
-        linewidth=0.5,
-        density=0.5,
-        arrowstyle="fancy",
-        arrowsize=1,
-    )
-
-    ang = ax.imshow(th_deg, extent=[-2, 2, -2, 2], cmap=cmap)
-
-    # Add filled circles for the charges themselves
-    charge_colors = {True: "#f50000", False: "#0091ff"}
-    charge_label = {True: "+", False: "-"}
-    label_align = {True: "center", False: "center"}
-    for q, pos in charges:
-        ax.add_patch(Circle(pos, 0.175, color=charge_colors[q > 0]))
-        ax.annotate(
-            charge_label[q > 0], xy=pos, fontsize=30, ha="center", va=label_align[q > 0]
-        )
-
-    ax.set_xlabel("")
-    ax.set_ylabel("")
-    ax.set_xlim(-2, 2)
-    ax.set_ylim(-2, 2)
-    ax.set_aspect("equal")
-    if title:
-        ax.set_title(
-            r"Angle of $\vec{E}$ with the x-axis", color=title_color, fontsize=14
-        )
-
-    divider = make_axes_locatable(ax)
-    cax = divider.append_axes("right", size="5%", pad=0.05)
-    cax.yaxis.label.set_color(title_color)
-    cax.tick_params(axis="y", colors=title_color)
-    plt.colorbar(ang, cax=cax)
-
-    return ax
-
-
-def _plot_examples(
-    color_map, images, arr_3d, figsize, facecolor, cname, cblind=True, norm=False
-):
-    """Create the figure based on the provided images, continuous colormaps"""
-    fig = plt.figure(figsize=figsize, facecolor=facecolor)
-    n_images = len(images)
-    if cblind:
-        c_maps, sub_title = _get_color_weak_cmap(color_map, n_images)
-    else:
-        c_maps = [color_map]
-        sub_title = [""] * n_images
-
-    title_color = "white" if facecolor == "black" else "black"
-
-    axi = 1
-    idx_3d = 0
-    n_rows = len(c_maps)
-    n_cols = len(images)
-
-    for c_map, im in itertools.product(c_maps, images):
-
-        if isinstance(im, str) and ("3D" in im):
-            px, py, pz = arr_3d[idx_3d]
-            ax3d = fig.add_subplot(
-                n_rows,
-                n_cols,
-                axi,
-                projection="3d",
-                facecolor=facecolor,
-                elev=10,
-                azim=-45,
-            )
-            ax3d.plot_surface(px, py, pz, cmap=c_map, linewidth=0, antialiased=False)
-            ax3d = plt.gca()
-            ax3d.xaxis.set_ticklabels([])
-            ax3d.yaxis.set_ticklabels([])
-            ax3d.zaxis.set_ticklabels([])
-            idx_3d = 0 if idx_3d == 1 else 1
-        elif isinstance(im, str) and ("electric" in im):
-            ax = fig.add_subplot(n_rows, n_cols, axi, facecolor=facecolor)
-            ax = _plot_e_field(
-                ax, c_map, n_neg_charges=2, facecolor=facecolor, title=axi <= n_cols
-            )
-        elif isinstance(im, str) and ("complex" in im):
-            ax = fig.add_subplot(n_rows, n_cols, axi, facecolor=facecolor)
-            ax = _plot_complex_arg(ax, c_map, facecolor, title=axi <= n_cols)
-        else:
-            cmap_norm = mpl.colors.CenteredNorm() if norm else None
-            ax = fig.add_subplot(n_rows, n_cols, axi, facecolor=facecolor)
-            ax.imshow(im, cmap=c_map, aspect="auto", norm=cmap_norm)
-            ax.get_xaxis().set_visible(False)
-            ax.get_yaxis().set_visible(False)
-            ax.set_title(sub_title[axi - 1], color=title_color, fontsize=16, loc="left")
-
-        axi += 1
-    fig.suptitle(cname, color=title_color, fontsize=24, y=0.95)
-    return fig
-
-
-def _plot_examples_qual(color_map, dict_arr, figsize, facecolor, cname, year):
-    """Create the figure with examples for discrete colormaps"""
-    fig = plt.figure(figsize=figsize, facecolor=facecolor)
-
-    c_tabs, sub_title = _get_color_weak_ctab(color_map, len(dict_arr) - 1)
-
-    title_color = "white" if facecolor == "black" else "black"
-
-    axi = 1
-    n_rows = len(c_tabs)
-    n_cols = len(dict_arr)
-
-    for c_map, d in itertools.product(c_tabs, dict_arr):
-
-        if axi in range(1, n_rows * n_cols, len(dict_arr)):
-            ax = fig.add_subplot(n_rows, n_cols, axi, facecolor=facecolor)
-            n_colors = len(d.keys())
-            ax.stackplot(
-                year, d.values(), labels=d.keys(), colors=c_map[range(n_colors), ...]
-            )
-            ax.legend(loc="upper left")
-            ax.set_facecolor(facecolor)
-            ax.set_title(sub_title[axi - 1], color=title_color, fontsize=16, loc="left")
-            ax.get_xaxis().set_visible(False)
-            ax.get_yaxis().set_visible(False)
-        elif axi in range(2, n_rows * n_cols, n_cols):
-            ax = fig.add_subplot(n_rows, n_cols, axi, facecolor=facecolor)
-            N = 45
-            x, y = np.random.rand(2, N)
-            np.random.seed(19680801)
-            s = np.random.randint(10, 220, size=N)
-            c = np.random.randint(0, 5, size=N)
-            scatter = ax.scatter(
-                x, y, cmap=ListedColormap(np.clip(c_map, 0, 1)), s=s, c=c
-            )
-            # produce a legend with the unique colors from the scatter
-            legend1 = ax.legend(
-                *scatter.legend_elements(), loc="lower left", title="Classes"
-            )
-            ax.add_artist(legend1)
-            ax.set_facecolor(facecolor)
-            # produce a legend with a cross section of sizes from the scatter
-            handles, labels = scatter.legend_elements(prop="sizes", alpha=0.6)
-            legend2 = ax.legend(handles, labels, loc="upper right", title="Sizes")
-            ax.get_xaxis().set_visible(False)
-            ax.get_yaxis().set_visible(False)
-        else:
-            ax = fig.add_subplot(n_rows, n_cols, axi, facecolor=facecolor)
-            n_colors = d.shape[1]
-            for col in range(n_colors):
-                ax.plot(d[..., col], color=c_map[col, ...])
-            ax.set_facecolor(facecolor)
-            ax.get_xaxis().set_visible(False)
-            ax.get_yaxis().set_visible(False)
-        axi += 1
-    fig.suptitle(cname, color=title_color, fontsize=24, y=0.95)
-    return fig
+import itertools
+import numpy as np
+import matplotlib as mpl
+import matplotlib.pyplot as plt
+import matplotlib.image as mpimg
+from matplotlib.colors import ListedColormap
+from matplotlib.patches import Circle
+from mpl_toolkits.axes_grid1 import make_axes_locatable
+from os.path import dirname, join
+
+# internal import
+from scicomap.cblind import _get_color_weak_ctab, _get_color_weak_cmap
+
+
+
+def _pyramid(n=513):
+    """Create a pyramid function"""
+    s = np.linspace(-1.0, 1.0, n)
+    x, y = np.meshgrid(s, s)
+    z = 1.0 - np.maximum(abs(x), abs(y))
+    return x, y, z
+
+
+def _pyramid_zombie(n=513, stacked=False):
+    """Create a pyramid and its zombie copy (buried pyramid)"""
+    # image plot
+    s_y = np.linspace(-1.0, 1.0, n)
+    x, y = np.meshgrid(s_y, s_y)
+    z = 1.0 - np.maximum(abs(x), abs(y))
+    z = np.hstack((z, z - 1)) if stacked else np.hstack((z, -z))
+    # 3d plot
+    s_x = np.linspace(-1.0, 3.0, 2 * n)
+    s_y = np.linspace(-1.0, 1.0, n)
+    x, y = np.meshgrid(s_x, s_y)
+    return x, y, z
+
+
+def _periodic_fn():
+    """Create a periodic function with a step function"""
+    dx = dy = 0.05
+    y, x = np.mgrid[-5 : 5 + dy : dy, -5 : 10 + dx : dx]
+    z = (
+        np.sin(x) ** 10
+        + np.cos(10 + y * x)
+        + np.cos(x)
+        + 0.2 * y
+        + 0.1 * x
+        + np.heaviside(x, 1) * np.heaviside(y, 1)
+    )
+    z = z - np.mean(z)
+    return x, y, z
+
+
+def _fn_with_roots(n=250):
+    """Create a function with roots, for diverging colormaps"""
+    x, y = np.meshgrid(np.linspace(-3, 3, n), np.linspace(-2, 2, n))
+    return (1 - x / 2 + x**5 + y**3) * np.exp(-(x**2) - y**2)
+
+
+def _complex_phase(n=100):
+    """argument of a function in the complex plane, cyclic colormaps"""
+    x, y = np.ogrid[-3 : 3 : n * 1j, -3 : 3 : n * 1j]
+    z = x + 1j * y
+    # w = (z ** 2 - 1) * (z - 2 - 1j) ** 2 / (z ** 2 + 2 + 2j)
+    w = (z**2 - 1) * (z - 2 - 1j) ** 2
+    return np.angle(w)
+
+
+def _plot_complex_arg(ax, cmap, facecolor="black", title=False):
+    """Create mlp ax of the complex argument"""
+    arg_z = _complex_phase(n=100)
+    title_color = "white" if facecolor == "black" else "black"
+    ang = ax.imshow(np.degrees(arg_z), extent=[-2, 2, -2, 2], cmap=cmap)
+
+    ax.set_xlim(-2, 2)
+    ax.set_ylim(-2, 2)
+    ax.set_aspect("equal")
+    if title:
+        ax.set_xlabel("Re", color=title_color, fontsize=12)
+        ax.set_ylabel("Im", color=title_color, fontsize=12)
+        ax.set_title(
+            r"Argument of $(z^2 - 1)(z - 2 - j)^2$", color=title_color, fontsize=14
+        )
+
+    divider = make_axes_locatable(ax)
+    cax = divider.append_axes("right", size="5%", pad=0.05)
+    cax.yaxis.label.set_color(title_color)
+    cax.tick_params(axis="y", colors=title_color)
+    plt.colorbar(ang, cax=cax)
+    return ax
+
+
+def _E(q, r0, x, y):
+    """Return the electric field vector E=(Ex,Ey) due to charge q at r0."""
+    den = np.hypot(x - r0[0], y - r0[1]) ** 3
+    return q * (x - r0[0]) / den, q * (y - r0[1]) / den
+
+
+def _angle_E(n_neg_charges):
+    """Create the angle of the electric field with the x-axis"""
+    # Grid of x, y points
+    nx, ny = 64, 64
+    x = np.linspace(-2, 2, nx)
+    y = np.linspace(-2, 2, ny)
+    X, Y = np.meshgrid(x, y)
+
+    # Create a multipole with nq charges of alternating sign, equally spaced
+    # on the unit circle.
+    nq = 2 ** int(n_neg_charges)
+    charges = []
+    for i in range(nq):
+        q = i % 2 * 2 - 1
+        charges.append((q, (np.cos(2 * np.pi * i / nq), np.sin(2 * np.pi * i / nq))))
+
+    # Electric field vector, E=(Ex, Ey), as separate components
+    Ex, Ey = np.zeros((ny, nx)), np.zeros((ny, nx))
+    for charge in charges:
+        ex, ey = _E(*charge, x=X, y=Y)
+        Ex += ex
+        Ey += ey
+
+    # angle wrt to 1_x
+    cos_th = Ex / np.hypot(Ex, Ey)
+    return np.degrees(np.arccos(cos_th)), charges, x, y, Ex, Ey
+
+
+def _plot_e_field(ax, cmap, n_neg_charges=2, facecolor="black", title=False):
+    """Create the mpl ax of the electric field"""
+    title_color = "white" if facecolor == "black" else "black"
+
+    th_deg, charges, x, y, Ex, Ey = _angle_E(n_neg_charges)
+
+    # Plot the streamlines with an appropriate colormap and arrow style
+    ax.streamplot(
+        x,
+        y,
+        Ex,
+        Ey,
+        color="black",
+        linewidth=0.5,
+        density=0.5,
+        arrowstyle="fancy",
+        arrowsize=1,
+    )
+
+    ang = ax.imshow(th_deg, extent=[-2, 2, -2, 2], cmap=cmap)
+
+    # Add filled circles for the charges themselves
+    charge_colors = {True: "#f50000", False: "#0091ff"}
+    charge_label = {True: "+", False: "-"}
+    label_align = {True: "center", False: "center"}
+    for q, pos in charges:
+        ax.add_patch(Circle(pos, 0.175, color=charge_colors[q > 0]))
+        ax.annotate(
+            charge_label[q > 0], xy=pos, fontsize=30, ha="center", va=label_align[q > 0]
+        )
+
+    ax.set_xlabel("")
+    ax.set_ylabel("")
+    ax.set_xlim(-2, 2)
+    ax.set_ylim(-2, 2)
+    ax.set_aspect("equal")
+    if title:
+        ax.set_title(
+            r"Angle of $\vec{E}$ with the x-axis", color=title_color, fontsize=14
+        )
+
+    divider = make_axes_locatable(ax)
+    cax = divider.append_axes("right", size="5%", pad=0.05)
+    cax.yaxis.label.set_color(title_color)
+    cax.tick_params(axis="y", colors=title_color)
+    plt.colorbar(ang, cax=cax)
+
+    return ax
+
+
+def _plot_examples(
+    color_map, images, arr_3d, figsize, facecolor, cname, cblind=True, norm=False
+):
+    """Create the figure based on the provided images, continuous colormaps"""
+    fig = plt.figure(figsize=figsize, facecolor=facecolor)
+    n_images = len(images)
+    if cblind:
+        c_maps, sub_title = _get_color_weak_cmap(color_map, n_images)
+    else:
+        c_maps = [color_map]
+        sub_title = [""] * n_images
+
+    title_color = "white" if facecolor == "black" else "black"
+
+    axi = 1
+    idx_3d = 0
+    n_rows = len(c_maps)
+    n_cols = len(images)
+
+    for c_map, im in itertools.product(c_maps, images):
+
+        if isinstance(im, str) and ("3D" in im):
+            px, py, pz = arr_3d[idx_3d]
+            ax3d = fig.add_subplot(
+                n_rows,
+                n_cols,
+                axi,
+                projection="3d",
+                facecolor=facecolor,
+                elev=10,
+                azim=-45,
+            )
+            ax3d.plot_surface(px, py, pz, cmap=c_map, linewidth=0, antialiased=False)
+            ax3d = plt.gca()
+            ax3d.xaxis.set_ticklabels([])
+            ax3d.yaxis.set_ticklabels([])
+            ax3d.zaxis.set_ticklabels([])
+            idx_3d = 0 if idx_3d == 1 else 1
+        elif isinstance(im, str) and ("electric" in im):
+            ax = fig.add_subplot(n_rows, n_cols, axi, facecolor=facecolor)
+            ax = _plot_e_field(
+                ax, c_map, n_neg_charges=2, facecolor=facecolor, title=axi <= n_cols
+            )
+        elif isinstance(im, str) and ("complex" in im):
+            ax = fig.add_subplot(n_rows, n_cols, axi, facecolor=facecolor)
+            ax = _plot_complex_arg(ax, c_map, facecolor, title=axi <= n_cols)
+        else:
+            cmap_norm = mpl.colors.CenteredNorm() if norm else None
+            ax = fig.add_subplot(n_rows, n_cols, axi, facecolor=facecolor)
+            ax.imshow(im, cmap=c_map, aspect="auto", norm=cmap_norm)
+            ax.get_xaxis().set_visible(False)
+            ax.get_yaxis().set_visible(False)
+            ax.set_title(sub_title[axi - 1], color=title_color, fontsize=16, loc="left")
+
+        axi += 1
+    fig.suptitle(cname, color=title_color, fontsize=24, y=0.95)
+    return fig
+
+
+def _plot_examples_qual(color_map, dict_arr, figsize, facecolor, cname, year):
+    """Create the figure with examples for discrete colormaps"""
+    fig = plt.figure(figsize=figsize, facecolor=facecolor)
+
+    c_tabs, sub_title = _get_color_weak_ctab(color_map, len(dict_arr) - 1)
+
+    title_color = "white" if facecolor == "black" else "black"
+
+    axi = 1
+    n_rows = len(c_tabs)
+    n_cols = len(dict_arr)
+
+    for c_map, d in itertools.product(c_tabs, dict_arr):
+
+        if axi in range(1, n_rows * n_cols, len(dict_arr)):
+            ax = fig.add_subplot(n_rows, n_cols, axi, facecolor=facecolor)
+            n_colors = len(d.keys())
+            ax.stackplot(
+                year, d.values(), labels=d.keys(), colors=c_map[range(n_colors), ...]
+            )
+            ax.legend(loc="upper left")
+            ax.set_facecolor(facecolor)
+            ax.set_title(sub_title[axi - 1], color=title_color, fontsize=16, loc="left")
+            ax.get_xaxis().set_visible(False)
+            ax.get_yaxis().set_visible(False)
+        elif axi in range(2, n_rows * n_cols, n_cols):
+            ax = fig.add_subplot(n_rows, n_cols, axi, facecolor=facecolor)
+            N = 45
+            x, y = np.random.rand(2, N)
+            np.random.seed(19680801)
+            s = np.random.randint(10, 220, size=N)
+            c = np.random.randint(0, 5, size=N)
+            scatter = ax.scatter(
+                x, y, cmap=ListedColormap(np.clip(c_map, 0, 1)), s=s, c=c
+            )
+            # produce a legend with the unique colors from the scatter
+            legend1 = ax.legend(
+                *scatter.legend_elements(), loc="lower left", title="Classes"
+            )
+            ax.add_artist(legend1)
+            ax.set_facecolor(facecolor)
+            # produce a legend with a cross section of sizes from the scatter
+            handles, labels = scatter.legend_elements(prop="sizes", alpha=0.6)
+            legend2 = ax.legend(handles, labels, loc="upper right", title="Sizes")
+            ax.get_xaxis().set_visible(False)
+            ax.get_yaxis().set_visible(False)
+        else:
+            ax = fig.add_subplot(n_rows, n_cols, axi, facecolor=facecolor)
+            n_colors = d.shape[1]
+            for col in range(n_colors):
+                ax.plot(d[..., col], color=c_map[col, ...])
+            ax.set_facecolor(facecolor)
+            ax.get_xaxis().set_visible(False)
+            ax.get_yaxis().set_visible(False)
+        axi += 1
+    fig.suptitle(cname, color=title_color, fontsize=24, y=0.95)
+    return fig
```

### Comparing `scicomap-1.0.0/src/scicomap.egg-info/PKG-INFO` & `scicomap-1.0.1/src/scicomap.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,294 +1,296 @@
-Metadata-Version: 2.1
-Name: scicomap
-Version: 1.0.0
-Summary: data visualization on maps with varying levels of granularity
-Author-email: Thomas Bury <bury.thomas@gmail.com>
-License: MIT License
-        
-        Copyright (c) [2021] [Thomas Bury]
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-Project-URL: homepage, https://github.com/ThomasBury/scicomap
-Project-URL: documentation, https://github.com/ThomasBury/scicomap
-Project-URL: repository, https://github.com/ThomasBury/scicomap.git
-Project-URL: changelog, https://github.com/ThomasBury/scicomap
-Project-URL: Tracker, https://github.com/ThomasBury/scicomap/issues
-Keywords: visualization,color,uniform,scientific
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: scipy
-Requires-Dist: colorspacious
-Requires-Dist: colorcet
-Requires-Dist: cmcrameri
-Requires-Dist: cmocean
-Requires-Dist: cmasher>=1.5.8
-Requires-Dist: palettable>=3.3.0
-Requires-Dist: matplotlib>=3.3.0
-Provides-Extra: doc
-Requires-Dist: ipykernel; extra == "doc"
-Requires-Dist: ipython_genutils; extra == "doc"
-Requires-Dist: pandoc; extra == "doc"
-Requires-Dist: sphinx; extra == "doc"
-Requires-Dist: sphinxawesome-theme==5.0.0b5; extra == "doc"
-Requires-Dist: nbsphinx; extra == "doc"
-Requires-Dist: sphinx-autodoc-typehints; extra == "doc"
-Requires-Dist: sphinx-copybutton; extra == "doc"
-Requires-Dist: sphinx-tabs; extra == "doc"
-Provides-Extra: lint
-Requires-Dist: black; extra == "lint"
-Requires-Dist: flake8; extra == "lint"
-Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: pytest-cov; extra == "test"
-
-<img src="pics/logo.png" alt="drawing" width="200"/>
-
-[buy me caffeine](https://ko-fi.com/V7V72SOHX)
-
-
-
-# Scientific color maps 
-
-## Blog post
-
-[Scicomap Medium blog post (free)](https://towardsdatascience.com/your-colour-map-is-bad-heres-how-to-fix-it-lessons-learnt-from-the-event-horizon-telescope-b82523f09469)
-
-[Tutorial notebook](./docs/notebooks/tutorial.ipynb)
-
-## Installation
-
-```shell
-pip install scicomap
-```
-
-## Introduction 
-
-Scicomap is a package that provides scientific color maps and tools to standardize your favourite color maps if you don't like the built-in ones.
-Scicomap currently provides sequential, bi-sequential, diverging, circular, qualitative and miscellaneous color maps. You can easily draw examples, compare the rendering, see how colorblind people will perceive the color maps. I will illustrate the scicomap capabilities below.
-
-This package is heavily based on the [Event Horyzon Plot package](https://github.com/liamedeiros/ehtplot/tree/docs) and uses good color maps found in the [the python portage of the Fabio Crameri](https://github.com/callumrollo/cmcrameri), [cmasher](https://cmasher.readthedocs.io/), [palettable](https://jiffyclub.github.io/palettable/), [colorcet](https://colorcet.holoviz.org/) and [cmocean](https://matplotlib.org/cmocean/)
-
-## Motivation
-
-The accurate representation of data is essential. Many common color maps distort data through uneven colour gradients and are often unreadable to those with color-vision deficiency. An infamous example is the jet color map. These color maps do not render all the information you want to illustrate or even worse render false information through artefacts. Scientist or not, your goal is to communicate visual information in the most accurate and appealing fashion. Moreover, do not overlook colour-vision deficiency, which represents 8% of the (Caucasian) male population.
-
-## Color spaces
-
-Perceptual uniformity is the idea that Euclidean distance between colors in color space should match human color perception distance judgements. For example, a blue and red that are at a distance d apart should look as discriminable as green and purple that are at a distance d apart.
-Scicomap uses the CAM02-UCS color space (Uniform Colour Space). Its three coordinates are usually denoted by J', a', and b'. And its cylindrical coordinates are J', C', and h'. The perceptual color space Jab is similar to Lab. However, Jab uses an updated color appearance model that in theory provides greater precision for discriminability measurements.
-
- * Lightness: also known as value or tone, is a representation of a color's brightness
- * Chroma: the intrinsic difference between a color and gray of an object
- * Hue: the degree to which a stimulus can be described as similar to or different from stimuli that are described as red, green, blue, and yellow
-
-## Encoding information
-
- * Lightness J': for a scalar value, intensity. It must vary linearly with the physical quantity
- * hue h' can encode an additional physical quantity, the change of hue should be linearly proportional to the quantity. The hue h' is also ideal in making an image more attractive without interfering with the representation of pixel values.
- * chroma is less recognizable and should not be used to encode physical information
-  
-## Color map uniformization
-
-Following the references and the theories, the uniformization is performed by
-
- * Making the color map linear in J'
- * Lifting the color map (making it lighter, i.e. increasing the minimal value of J')
- * Symmetrizing the chroma to avoid further artefacts
- * Avoid kinks and edges in the chroma curve
- * Bitonic symmetrization or not
-
-
-# Scicomap
-
-## Choosing the right type of color maps
-Scicomap provides a bunch of color maps for different applications. The different types of color map are 
-
-```python
-import scicomap as sc
-sc_map = sc.SciCoMap()
-sc_map.get_ctype()
-```
-
-```
-dict_keys(['diverging', 'sequential', 'multi-sequential', 'circular', 'miscellaneous', 'qualitative'])
-```
-
-I'll refer to the [The misuse of colour in science communication](https://www.nature.com/articles/s41467-020-19160-7.pdf) for choosing the right scientific color map
-
-<td align="left"><img src="pics/choosing-cmap.png" width="500"/></td>
-
-## Get the matplotlib cmap
-
-
-```python
-plt_cmap_obj = sc_map.get_mpl_color_map()
-```
-
-## Choosing the color map for a given type
-
-Get the color maps for a given type
-
-```python
-sc_map = sc.ScicoSequential()
-sc_map.get_color_map_names()
-```
-
-```
-dict_keys(['afmhot', 'amber', 'amber_r', 'amp', 'apple', 'apple_r', 'autumn', 'batlow', 'bilbao', 'bilbao_r', 'binary', 'Blues', 'bone', 'BuGn', 'BuPu', 'chroma', 'chroma_r', 'cividis', 'cool', 'copper', 'cosmic', 'cosmic_r', 'deep', 'dense', 'dusk', 'dusk_r', 'eclipse', 'eclipse_r', 'ember', 'ember_r', 'fall', 'fall_r', 'gem', 'gem_r', 'gist_gray', 'gist_heat', 'gist_yarg', 'GnBu', 'Greens', 'gray', 'Greys', 'haline', 'hawaii', 'hawaii_r', 'heat', 'heat_r', 'hot', 'ice', 'inferno', 'imola', 'imola_r', 'lapaz', 'lapaz_r', 'magma', 'matter', 'neon', 'neon_r', 'neutral', 'neutral_r', 'nuuk', 'nuuk_r', 'ocean', 'ocean_r', 'OrRd', 'Oranges', 'pink', 'plasma', 'PuBu', 'PuBuGn', 'PuRd', 'Purples', 'rain', 'rainbow', 'rainbow-sc', 'rainbow-sc_r', 'rainforest', 'rainforest_r', 'RdPu', 'Reds', 'savanna', 'savanna_r', 'sepia', 'sepia_r', 'speed', 'solar', 'spring', 'summer', 'tempo', 'thermal', 'thermal_r', 'thermal-2', 'tokyo', 'tokyo_r', 'tropical', 'tropical_r', 'turbid', 'turku', 'turku_r', 'viridis', 'winter', 'Wistia', 'YlGn', 'YlGnBu', 'YlOrBr', 'YlOrRd'])
-```
-
-## Assessing a color map
-
-In order to assess if a color map should be corrected or not, `scicomap` provides a way to quickly check if the lightness is linear, how asymmetric and smooth is the chroma and how the color map renders for color-deficient users. I will illustrate some of the artefacts using classical images, as the pyramid and specific functions for each kind of color map.
-
-
-### An infamous example
-
-```python
-import scicomap as sc
-import matplotlib.pyplot as plt
-
-# the thing that should not be
-ugly_jet = plt.get_cmap("jet")
-sc_map =  sc.ScicoMiscellaneous(cmap=ugly_jet)
-f=sc_map.assess_cmap(figsize=(22,10))
-```
-
-
-<td align="left"><img src="pics/jet.png" width="1000"/></td>
- 
-
-Clearly, the lightness is not linear, has edges and kinks. The chroma is not smooth and asymmetrical. See the below illustration to see how bad and how many artefacts the jet color map introduces
-
-
-<td align="left"><img src="pics/jet2.png" width="1000"/></td>
-
-
-## Correcting a color map - Example
-
-### Sequential color map
-
-Let's assess the built-in color map `hawaii` without correction:
-
-```python
-sc_map = sc.ScicoSequential(cmap='hawaii')
-f=sc_map.assess_cmap(figsize=(22,10))
-```
-
-<td align="left"><img src="pics/hawaii.png" width="1000"/></td>
-
-
-The color map seems ok, however, the lightness is not linear and the chroma is asymmetrical even if smooth. Those small defects introduce artefact in the information rendering, as we can visualize using the following example
-
-
-```python
-f=sc_map.draw_example()
-```
-
-<td align="left"><img src="pics/hawaii-examples.png" width="1000"/></td>
-
-
-We can clearly see the artefacts, especially for the pyramid for which our eyes should only pick out the corners in the pyramid (ideal situation). Those artefacts are even more striking for color-deficient users (this might not always be the case). Hopefully, `scicomap` provides an easy way to correct those defects:
-
-```python
-# fixing the color map, using the same minimal lightness (lift=None), 
-# not normalizing to bitone and 
-# smoothing the chroma
-sc_map.unif_sym_cmap(lift=None, 
-                     bitonic=False, 
-                     diffuse=True)
-
-# re-assess the color map after fixing it                     
-f=sc_map.assess_cmap(figsize=(22,10))
-```
-
-<td align="left"><img src="pics/hawaii-fixed.png" width="1000"/></td>
-
-
-After fixing the color map, the artefacts are less present
-
-<td align="left"><img src="pics/hawaii-fixed-examples.png" width="1000"/></td>
-
-# All the built-in color maps
-
-## Sequential
-
-<td align="left"><img src="pics/seq-cmaps-all.png" width="500"/></td>
-
-## Diverging
-
-
-<td align="left"><img src="pics/div-cmaps-all.png" width="500"/></td>
-
-## Mutli-sequential
-
-<td align="left"><img src="pics/multi-cmaps-all.png" width="500"/></td>
-
-## Miscellaneous
-
-<td align="left"><img src="pics/misc-cmaps-all.png" width="500"/></td>
-
-## Circular
-
-<td align="left"><img src="pics/circular-cmaps-all.png" width="500"/></td>
-
-## Qualitative
-
-<td align="left"><img src="pics/qual-cmaps-all.png" width="500"/></td>
-
-# References
-
- * [The misuse of colour in science communication](https://www.nature.com/articles/s41467-020-19160-7.pdf)
- * [Why We Use Bad Color Maps and What You Can Do About It](https://www.kennethmoreland.com/color-advice/BadColorMaps.pdf)
- * [THE RAINBOW IS DEAD…LONG LIVE THE RAINBOW! – SERIES OUTLINE](https://mycarta.wordpress.com/2012/05/29/the-rainbow-is-dead-long-live-the-rainbow-series-outline/)
- * [Scientific colour maps](https://www.fabiocrameri.ch/colourmaps/)
- * [Picking a colour scale for scientific graphics](https://betterfigures.org/2015/06/23/picking-a-colour-scale-for-scientific-graphics/)
- * [ColorCET](https://colorcet.com/)
- * [Good Colour Maps: How to Design Them](https://arxiv.org/abs/1509.03700)
- * [Perceptually uniform color space for image signals including high dynamic range and wide gamut](https://www.osapublishing.org/oe/fulltext.cfm?uri=oe-25-13-15131&id=368272)
-
-
-# Changes log
-
-### 1.0.0
-
- - Docstring
- - Tutorial notebook
- - Web documentation
-
-### 0.4
-
- - Including files in source distributions
-
-### 0.3
-
- - Add a section "how to use with matplotlib"
- - [Bug] Center diverging color map in examples
-
-### 0.2
-
- - [Bug] Fix typo in chart titles
-
-### 0.1
-
- - First version
+Metadata-Version: 2.1
+Name: scicomap
+Version: 1.0.1
+Summary: data visualization on maps with varying levels of granularity
+Author-email: Thomas Bury <bury.thomas@gmail.com>
+License: MIT License
+        
+        Copyright (c) [2021] [Thomas Bury]
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+Project-URL: homepage, https://github.com/ThomasBury/scicomap
+Project-URL: documentation, https://github.com/ThomasBury/scicomap
+Project-URL: repository, https://github.com/ThomasBury/scicomap.git
+Project-URL: changelog, https://github.com/ThomasBury/scicomap
+Project-URL: Tracker, https://github.com/ThomasBury/scicomap/issues
+Keywords: visualization,color,uniform,scientific
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: scipy
+Requires-Dist: colorspacious
+Requires-Dist: colorcet
+Requires-Dist: cmcrameri
+Requires-Dist: cmocean
+Requires-Dist: cmasher>=1.5.8
+Requires-Dist: palettable>=3.3.0
+Requires-Dist: matplotlib>=3.3.0
+Provides-Extra: doc
+Requires-Dist: ipykernel; extra == "doc"
+Requires-Dist: ipython_genutils; extra == "doc"
+Requires-Dist: pandoc; extra == "doc"
+Requires-Dist: sphinx; extra == "doc"
+Requires-Dist: sphinxawesome-theme==5.0.0b5; extra == "doc"
+Requires-Dist: nbsphinx; extra == "doc"
+Requires-Dist: sphinx-autodoc-typehints; extra == "doc"
+Requires-Dist: sphinx-copybutton; extra == "doc"
+Requires-Dist: sphinx-tabs; extra == "doc"
+Provides-Extra: lint
+Requires-Dist: black; extra == "lint"
+Requires-Dist: flake8; extra == "lint"
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+
+<img src="pics/logo.png" alt="drawing" width="200"/>
+
+[buy me caffeine](https://ko-fi.com/V7V72SOHX)
+
+
+
+# Scientific color maps 
+
+## Blog post
+
+[Scicomap Medium blog post (free)](https://towardsdatascience.com/your-colour-map-is-bad-heres-how-to-fix-it-lessons-learnt-from-the-event-horizon-telescope-b82523f09469)
+
+[Official Documentation](https://scicomap.readthedocs.io/en/latest/)
+
+[Tutorial notebook](./docs/notebooks/tutorial.ipynb)
+
+## Installation
+
+```shell
+pip install scicomap
+```
+
+## Introduction 
+
+Scicomap is a package that provides scientific color maps and tools to standardize your favourite color maps if you don't like the built-in ones.
+Scicomap currently provides sequential, bi-sequential, diverging, circular, qualitative and miscellaneous color maps. You can easily draw examples, compare the rendering, see how colorblind people will perceive the color maps. I will illustrate the scicomap capabilities below.
+
+This package is heavily based on the [Event Horyzon Plot package](https://github.com/liamedeiros/ehtplot/tree/docs) and uses good color maps found in the [the python portage of the Fabio Crameri](https://github.com/callumrollo/cmcrameri), [cmasher](https://cmasher.readthedocs.io/), [palettable](https://jiffyclub.github.io/palettable/), [colorcet](https://colorcet.holoviz.org/) and [cmocean](https://matplotlib.org/cmocean/)
+
+## Motivation
+
+The accurate representation of data is essential. Many common color maps distort data through uneven colour gradients and are often unreadable to those with color-vision deficiency. An infamous example is the jet color map. These color maps do not render all the information you want to illustrate or even worse render false information through artefacts. Scientist or not, your goal is to communicate visual information in the most accurate and appealing fashion. Moreover, do not overlook colour-vision deficiency, which represents 8% of the (Caucasian) male population.
+
+## Color spaces
+
+Perceptual uniformity is the idea that Euclidean distance between colors in color space should match human color perception distance judgements. For example, a blue and red that are at a distance d apart should look as discriminable as green and purple that are at a distance d apart.
+Scicomap uses the CAM02-UCS color space (Uniform Colour Space). Its three coordinates are usually denoted by J', a', and b'. And its cylindrical coordinates are J', C', and h'. The perceptual color space Jab is similar to Lab. However, Jab uses an updated color appearance model that in theory provides greater precision for discriminability measurements.
+
+ * Lightness: also known as value or tone, is a representation of a color's brightness
+ * Chroma: the intrinsic difference between a color and gray of an object
+ * Hue: the degree to which a stimulus can be described as similar to or different from stimuli that are described as red, green, blue, and yellow
+
+## Encoding information
+
+ * Lightness J': for a scalar value, intensity. It must vary linearly with the physical quantity
+ * hue h' can encode an additional physical quantity, the change of hue should be linearly proportional to the quantity. The hue h' is also ideal in making an image more attractive without interfering with the representation of pixel values.
+ * chroma is less recognizable and should not be used to encode physical information
+  
+## Color map uniformization
+
+Following the references and the theories, the uniformization is performed by
+
+ * Making the color map linear in J'
+ * Lifting the color map (making it lighter, i.e. increasing the minimal value of J')
+ * Symmetrizing the chroma to avoid further artefacts
+ * Avoid kinks and edges in the chroma curve
+ * Bitonic symmetrization or not
+
+
+# Scicomap
+
+## Choosing the right type of color maps
+Scicomap provides a bunch of color maps for different applications. The different types of color map are 
+
+```python
+import scicomap as sc
+sc_map = sc.SciCoMap()
+sc_map.get_ctype()
+```
+
+```
+dict_keys(['diverging', 'sequential', 'multi-sequential', 'circular', 'miscellaneous', 'qualitative'])
+```
+
+I'll refer to the [The misuse of colour in science communication](https://www.nature.com/articles/s41467-020-19160-7.pdf) for choosing the right scientific color map
+
+<td align="left"><img src="pics/choosing-cmap.png" width="500"/></td>
+
+## Get the matplotlib cmap
+
+
+```python
+plt_cmap_obj = sc_map.get_mpl_color_map()
+```
+
+## Choosing the color map for a given type
+
+Get the color maps for a given type
+
+```python
+sc_map = sc.ScicoSequential()
+sc_map.get_color_map_names()
+```
+
+```
+dict_keys(['afmhot', 'amber', 'amber_r', 'amp', 'apple', 'apple_r', 'autumn', 'batlow', 'bilbao', 'bilbao_r', 'binary', 'Blues', 'bone', 'BuGn', 'BuPu', 'chroma', 'chroma_r', 'cividis', 'cool', 'copper', 'cosmic', 'cosmic_r', 'deep', 'dense', 'dusk', 'dusk_r', 'eclipse', 'eclipse_r', 'ember', 'ember_r', 'fall', 'fall_r', 'gem', 'gem_r', 'gist_gray', 'gist_heat', 'gist_yarg', 'GnBu', 'Greens', 'gray', 'Greys', 'haline', 'hawaii', 'hawaii_r', 'heat', 'heat_r', 'hot', 'ice', 'inferno', 'imola', 'imola_r', 'lapaz', 'lapaz_r', 'magma', 'matter', 'neon', 'neon_r', 'neutral', 'neutral_r', 'nuuk', 'nuuk_r', 'ocean', 'ocean_r', 'OrRd', 'Oranges', 'pink', 'plasma', 'PuBu', 'PuBuGn', 'PuRd', 'Purples', 'rain', 'rainbow', 'rainbow-sc', 'rainbow-sc_r', 'rainforest', 'rainforest_r', 'RdPu', 'Reds', 'savanna', 'savanna_r', 'sepia', 'sepia_r', 'speed', 'solar', 'spring', 'summer', 'tempo', 'thermal', 'thermal_r', 'thermal-2', 'tokyo', 'tokyo_r', 'tropical', 'tropical_r', 'turbid', 'turku', 'turku_r', 'viridis', 'winter', 'Wistia', 'YlGn', 'YlGnBu', 'YlOrBr', 'YlOrRd'])
+```
+
+## Assessing a color map
+
+In order to assess if a color map should be corrected or not, `scicomap` provides a way to quickly check if the lightness is linear, how asymmetric and smooth is the chroma and how the color map renders for color-deficient users. I will illustrate some of the artefacts using classical images, as the pyramid and specific functions for each kind of color map.
+
+
+### An infamous example
+
+```python
+import scicomap as sc
+import matplotlib.pyplot as plt
+
+# the thing that should not be
+ugly_jet = plt.get_cmap("jet")
+sc_map =  sc.ScicoMiscellaneous(cmap=ugly_jet)
+f=sc_map.assess_cmap(figsize=(22,10))
+```
+
+
+<td align="left"><img src="pics/jet.png" width="1000"/></td>
+ 
+
+Clearly, the lightness is not linear, has edges and kinks. The chroma is not smooth and asymmetrical. See the below illustration to see how bad and how many artefacts the jet color map introduces
+
+
+<td align="left"><img src="pics/jet2.png" width="1000"/></td>
+
+
+## Correcting a color map - Example
+
+### Sequential color map
+
+Let's assess the built-in color map `hawaii` without correction:
+
+```python
+sc_map = sc.ScicoSequential(cmap='hawaii')
+f=sc_map.assess_cmap(figsize=(22,10))
+```
+
+<td align="left"><img src="pics/hawaii.png" width="1000"/></td>
+
+
+The color map seems ok, however, the lightness is not linear and the chroma is asymmetrical even if smooth. Those small defects introduce artefact in the information rendering, as we can visualize using the following example
+
+
+```python
+f=sc_map.draw_example()
+```
+
+<td align="left"><img src="pics/hawaii-examples.png" width="1000"/></td>
+
+
+We can clearly see the artefacts, especially for the pyramid for which our eyes should only pick out the corners in the pyramid (ideal situation). Those artefacts are even more striking for color-deficient users (this might not always be the case). Hopefully, `scicomap` provides an easy way to correct those defects:
+
+```python
+# fixing the color map, using the same minimal lightness (lift=None), 
+# not normalizing to bitone and 
+# smoothing the chroma
+sc_map.unif_sym_cmap(lift=None, 
+                     bitonic=False, 
+                     diffuse=True)
+
+# re-assess the color map after fixing it                     
+f=sc_map.assess_cmap(figsize=(22,10))
+```
+
+<td align="left"><img src="pics/hawaii-fixed.png" width="1000"/></td>
+
+
+After fixing the color map, the artefacts are less present
+
+<td align="left"><img src="pics/hawaii-fixed-examples.png" width="1000"/></td>
+
+# All the built-in color maps
+
+## Sequential
+
+<td align="left"><img src="pics/seq-cmaps-all.png" width="500"/></td>
+
+## Diverging
+
+
+<td align="left"><img src="pics/div-cmaps-all.png" width="500"/></td>
+
+## Mutli-sequential
+
+<td align="left"><img src="pics/multi-cmaps-all.png" width="500"/></td>
+
+## Miscellaneous
+
+<td align="left"><img src="pics/misc-cmaps-all.png" width="500"/></td>
+
+## Circular
+
+<td align="left"><img src="pics/circular-cmaps-all.png" width="500"/></td>
+
+## Qualitative
+
+<td align="left"><img src="pics/qual-cmaps-all.png" width="500"/></td>
+
+# References
+
+ * [The misuse of colour in science communication](https://www.nature.com/articles/s41467-020-19160-7.pdf)
+ * [Why We Use Bad Color Maps and What You Can Do About It](https://www.kennethmoreland.com/color-advice/BadColorMaps.pdf)
+ * [THE RAINBOW IS DEAD…LONG LIVE THE RAINBOW! – SERIES OUTLINE](https://mycarta.wordpress.com/2012/05/29/the-rainbow-is-dead-long-live-the-rainbow-series-outline/)
+ * [Scientific colour maps](https://www.fabiocrameri.ch/colourmaps/)
+ * [Picking a colour scale for scientific graphics](https://betterfigures.org/2015/06/23/picking-a-colour-scale-for-scientific-graphics/)
+ * [ColorCET](https://colorcet.com/)
+ * [Good Colour Maps: How to Design Them](https://arxiv.org/abs/1509.03700)
+ * [Perceptually uniform color space for image signals including high dynamic range and wide gamut](https://www.osapublishing.org/oe/fulltext.cfm?uri=oe-25-13-15131&id=368272)
+
+
+# Changes log
+
+### 1.0.0
+
+ - Docstring
+ - Tutorial notebook
+ - Web documentation
+
+### 0.4
+
+ - Including files in source distributions
+
+### 0.3
+
+ - Add a section "how to use with matplotlib"
+ - [Bug] Center diverging color map in examples
+
+### 0.2
+
+ - [Bug] Fix typo in chart titles
+
+### 0.1
+
+ - First version
```

### Comparing `scicomap-1.0.0/src/scicomap.egg-info/SOURCES.txt` & `scicomap-1.0.1/src/scicomap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

