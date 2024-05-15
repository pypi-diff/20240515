# Comparing `tmp/WaveFormer-0.1.2.tar.gz` & `tmp/WaveFormer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WaveFormer-0.1.2.tar", last modified: Tue May 14 06:57:02 2024, max compression
+gzip compressed data, was "WaveFormer-0.1.3.tar", last modified: Wed May 15 11:19:10 2024, max compression
```

## Comparing `WaveFormer-0.1.2.tar` & `WaveFormer-0.1.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 06:57:02.252564 WaveFormer-0.1.2/
--rw-rw-rw-   0        0        0    15659 2024-05-14 06:57:02.251535 WaveFormer-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0    13348 2024-05-12 11:33:27.000000 WaveFormer-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 06:57:02.228532 WaveFormer-0.1.2/WaveFormer.egg-info/
--rw-rw-rw-   0        0        0    15659 2024-05-14 06:57:02.000000 WaveFormer-0.1.2/WaveFormer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1151 2024-05-14 06:57:02.000000 WaveFormer-0.1.2/WaveFormer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 06:57:02.000000 WaveFormer-0.1.2/WaveFormer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      362 2024-05-14 06:57:02.000000 WaveFormer-0.1.2/WaveFormer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       43 2024-05-14 06:57:02.000000 WaveFormer-0.1.2/WaveFormer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-14 06:57:02.230037 WaveFormer-0.1.2/audio_modules/
--rw-rw-rw-   0        0        0        0 2023-03-30 08:05:32.000000 WaveFormer-0.1.2/audio_modules/__init__.py
--rw-rw-rw-   0        0        0    33218 2024-05-12 08:58:22.000000 WaveFormer-0.1.2/audio_modules/air.py
-drwxrwxrwx   0        0        0        0 2024-05-14 06:57:02.234548 WaveFormer-0.1.2/audio_modules/core/
--rw-rw-rw-   0        0        0        0 2023-06-07 06:27:05.000000 WaveFormer-0.1.2/audio_modules/core/__init__.py
--rw-rw-rw-   0        0        0     9745 2024-05-12 08:58:45.000000 WaveFormer-0.1.2/audio_modules/core/configs.py
--rw-rw-rw-   0        0        0        0 2023-06-07 06:21:56.000000 WaveFormer-0.1.2/audio_modules/core/forms.py
--rw-rw-rw-   0        0        0    28704 2024-05-05 10:27:34.000000 WaveFormer-0.1.2/audio_modules/core/informers.py
--rw-rw-rw-   0        0        0        0 2023-06-07 06:21:45.000000 WaveFormer-0.1.2/audio_modules/core/reformers.py
-drwxrwxrwx   0        0        0        0 2024-05-14 06:57:02.237550 WaveFormer-0.1.2/audio_modules/extraction/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:17:07.000000 WaveFormer-0.1.2/audio_modules/extraction/__init__.py
--rw-rw-rw-   0        0        0    23908 2024-05-05 11:09:15.000000 WaveFormer-0.1.2/audio_modules/extraction/commands.py
--rw-rw-rw-   0        0        0    15143 2024-05-05 11:09:15.000000 WaveFormer-0.1.2/audio_modules/extraction/core.py
--rw-rw-rw-   0        0        0    28479 2024-05-05 11:09:15.000000 WaveFormer-0.1.2/audio_modules/extraction/extract_configs.py
--rw-rw-rw-   0        0        0     2097 2024-05-05 11:09:15.000000 WaveFormer-0.1.2/audio_modules/extraction/xtgraph.py
-drwxrwxrwx   0        0        0        0 2024-05-14 06:57:02.241484 WaveFormer-0.1.2/audio_modules/nvision/
--rw-rw-rw-   0        0        0        0 2024-05-05 11:53:17.000000 WaveFormer-0.1.2/audio_modules/nvision/__init__.py
--rw-rw-rw-   0        0        0     5696 2024-05-12 08:59:01.000000 WaveFormer-0.1.2/audio_modules/nvision/configs.py
--rw-rw-rw-   0        0        0     6100 2024-05-05 11:09:15.000000 WaveFormer-0.1.2/audio_modules/nvision/core.py
--rw-rw-rw-   0        0        0     3709 2024-05-05 11:09:15.000000 WaveFormer-0.1.2/audio_modules/nvision/ngraph.py
--rw-rw-rw-   0        0        0   110049 2024-05-05 11:09:15.000000 WaveFormer-0.1.2/audio_modules/nvision/plotly_mappings.py
-drwxrwxrwx   0        0        0        0 2024-05-14 06:57:02.247490 WaveFormer-0.1.2/audio_modules/praat/
--rw-rw-rw-   0        0        0        0 2023-06-14 09:13:20.000000 WaveFormer-0.1.2/audio_modules/praat/__init__.py
--rw-rw-rw-   0        0        0     5979 2024-05-12 08:59:21.000000 WaveFormer-0.1.2/audio_modules/praat/configs.py
--rw-rw-rw-   0        0        0     1615 2024-05-12 09:00:03.000000 WaveFormer-0.1.2/audio_modules/praat/core.py
--rw-rw-rw-   0        0        0     1252 2024-05-05 11:09:15.000000 WaveFormer-0.1.2/audio_modules/praat/filters.py
--rw-rw-rw-   0        0        0     9908 2024-05-12 09:00:13.000000 WaveFormer-0.1.2/audio_modules/praat/formant.py
--rw-rw-rw-   0        0        0     1832 2024-05-12 09:00:23.000000 WaveFormer-0.1.2/audio_modules/praat/handlers.py
--rw-rw-rw-   0        0        0     1833 2023-06-14 12:11:37.000000 WaveFormer-0.1.2/audio_modules/praat/processor.py
--rw-rw-rw-   0        0        0     1765 2023-06-14 08:39:57.000000 WaveFormer-0.1.2/audio_modules/praat/spectrogram.py
--rw-rw-rw-   0        0        0     4456 2024-05-05 11:09:15.000000 WaveFormer-0.1.2/audio_modules/types.py
-drwxrwxrwx   0        0        0        0 2024-05-14 06:57:02.250538 WaveFormer-0.1.2/rubberband/
--rw-rw-rw-   0        0        0       64 2023-06-02 09:36:21.000000 WaveFormer-0.1.2/rubberband/__init__.py
--rw-rw-rw-   0        0        0     4910 2024-05-05 12:10:35.000000 WaveFormer-0.1.2/rubberband/options.py
--rw-rw-rw-   0        0        0    12814 2023-06-06 13:00:27.000000 WaveFormer-0.1.2/rubberband/rubberbandstretcher.py
--rw-rw-rw-   0        0        0      272 2024-05-14 06:00:37.000000 WaveFormer-0.1.2/rubberband/wrapper.py
-drwxrwxrwx   0        0        0        0 2024-05-14 06:57:02.250538 WaveFormer-0.1.2/rubberband_builds/
--rw-rw-rw-   0        0        0        0 2023-05-06 11:06:20.000000 WaveFormer-0.1.2/rubberband_builds/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-14 06:57:02.252564 WaveFormer-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      804 2024-05-14 06:53:34.000000 WaveFormer-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 11:19:10.019438 WaveFormer-0.1.3/
+-rw-rw-rw-   0        0        0    16285 2024-05-15 11:19:10.019438 WaveFormer-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0    13348 2024-05-12 11:33:27.000000 WaveFormer-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 11:19:09.981434 WaveFormer-0.1.3/WaveFormer.egg-info/
+-rw-rw-rw-   0        0        0    16285 2024-05-15 11:19:09.000000 WaveFormer-0.1.3/WaveFormer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1151 2024-05-15 11:19:09.000000 WaveFormer-0.1.3/WaveFormer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 11:19:09.000000 WaveFormer-0.1.3/WaveFormer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      362 2024-05-15 11:19:09.000000 WaveFormer-0.1.3/WaveFormer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       43 2024-05-15 11:19:09.000000 WaveFormer-0.1.3/WaveFormer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 11:19:09.983433 WaveFormer-0.1.3/audio_modules/
+-rw-rw-rw-   0        0        0        0 2023-03-30 08:05:32.000000 WaveFormer-0.1.3/audio_modules/__init__.py
+-rw-rw-rw-   0        0        0    33218 2024-05-12 08:58:22.000000 WaveFormer-0.1.3/audio_modules/air.py
+drwxrwxrwx   0        0        0        0 2024-05-15 11:19:09.986432 WaveFormer-0.1.3/audio_modules/core/
+-rw-rw-rw-   0        0        0        0 2023-06-07 06:27:05.000000 WaveFormer-0.1.3/audio_modules/core/__init__.py
+-rw-rw-rw-   0        0        0     9745 2024-05-12 08:58:45.000000 WaveFormer-0.1.3/audio_modules/core/configs.py
+-rw-rw-rw-   0        0        0        0 2023-06-07 06:21:56.000000 WaveFormer-0.1.3/audio_modules/core/forms.py
+-rw-rw-rw-   0        0        0    28704 2024-05-05 10:27:34.000000 WaveFormer-0.1.3/audio_modules/core/informers.py
+-rw-rw-rw-   0        0        0        0 2023-06-07 06:21:45.000000 WaveFormer-0.1.3/audio_modules/core/reformers.py
+drwxrwxrwx   0        0        0        0 2024-05-15 11:19:10.004433 WaveFormer-0.1.3/audio_modules/extraction/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:17:07.000000 WaveFormer-0.1.3/audio_modules/extraction/__init__.py
+-rw-rw-rw-   0        0        0    23908 2024-05-05 11:09:15.000000 WaveFormer-0.1.3/audio_modules/extraction/commands.py
+-rw-rw-rw-   0        0        0    15143 2024-05-05 11:09:15.000000 WaveFormer-0.1.3/audio_modules/extraction/core.py
+-rw-rw-rw-   0        0        0    28479 2024-05-05 11:09:15.000000 WaveFormer-0.1.3/audio_modules/extraction/extract_configs.py
+-rw-rw-rw-   0        0        0     2097 2024-05-05 11:09:15.000000 WaveFormer-0.1.3/audio_modules/extraction/xtgraph.py
+drwxrwxrwx   0        0        0        0 2024-05-15 11:19:10.008433 WaveFormer-0.1.3/audio_modules/nvision/
+-rw-rw-rw-   0        0        0        0 2024-05-05 11:53:17.000000 WaveFormer-0.1.3/audio_modules/nvision/__init__.py
+-rw-rw-rw-   0        0        0     5696 2024-05-12 08:59:01.000000 WaveFormer-0.1.3/audio_modules/nvision/configs.py
+-rw-rw-rw-   0        0        0     6100 2024-05-05 11:09:15.000000 WaveFormer-0.1.3/audio_modules/nvision/core.py
+-rw-rw-rw-   0        0        0     3709 2024-05-05 11:09:15.000000 WaveFormer-0.1.3/audio_modules/nvision/ngraph.py
+-rw-rw-rw-   0        0        0   110049 2024-05-05 11:09:15.000000 WaveFormer-0.1.3/audio_modules/nvision/plotly_mappings.py
+drwxrwxrwx   0        0        0        0 2024-05-15 11:19:10.014438 WaveFormer-0.1.3/audio_modules/praat/
+-rw-rw-rw-   0        0        0        0 2023-06-14 09:13:20.000000 WaveFormer-0.1.3/audio_modules/praat/__init__.py
+-rw-rw-rw-   0        0        0     5979 2024-05-12 08:59:21.000000 WaveFormer-0.1.3/audio_modules/praat/configs.py
+-rw-rw-rw-   0        0        0     1615 2024-05-12 09:00:03.000000 WaveFormer-0.1.3/audio_modules/praat/core.py
+-rw-rw-rw-   0        0        0     1252 2024-05-05 11:09:15.000000 WaveFormer-0.1.3/audio_modules/praat/filters.py
+-rw-rw-rw-   0        0        0     9908 2024-05-12 09:00:13.000000 WaveFormer-0.1.3/audio_modules/praat/formant.py
+-rw-rw-rw-   0        0        0     1832 2024-05-12 09:00:23.000000 WaveFormer-0.1.3/audio_modules/praat/handlers.py
+-rw-rw-rw-   0        0        0     1833 2023-06-14 12:11:37.000000 WaveFormer-0.1.3/audio_modules/praat/processor.py
+-rw-rw-rw-   0        0        0     1765 2023-06-14 08:39:57.000000 WaveFormer-0.1.3/audio_modules/praat/spectrogram.py
+-rw-rw-rw-   0        0        0     4456 2024-05-05 11:09:15.000000 WaveFormer-0.1.3/audio_modules/types.py
+drwxrwxrwx   0        0        0        0 2024-05-15 11:19:10.017439 WaveFormer-0.1.3/rubberband/
+-rw-rw-rw-   0        0        0       64 2023-06-02 09:36:21.000000 WaveFormer-0.1.3/rubberband/__init__.py
+-rw-rw-rw-   0        0        0     4910 2024-05-05 12:10:35.000000 WaveFormer-0.1.3/rubberband/options.py
+-rw-rw-rw-   0        0        0    12814 2023-06-06 13:00:27.000000 WaveFormer-0.1.3/rubberband/rubberbandstretcher.py
+-rw-rw-rw-   0        0        0      272 2024-05-14 06:00:37.000000 WaveFormer-0.1.3/rubberband/wrapper.py
+drwxrwxrwx   0        0        0        0 2024-05-15 11:19:10.018438 WaveFormer-0.1.3/rubberband_builds/
+-rw-rw-rw-   0        0        0        0 2023-05-06 11:06:20.000000 WaveFormer-0.1.3/rubberband_builds/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-15 11:19:10.019438 WaveFormer-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1614 2024-05-15 11:18:30.000000 WaveFormer-0.1.3/setup.py
```

### Comparing `WaveFormer-0.1.2/PKG-INFO` & `WaveFormer-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: WaveFormer
-Version: 0.1.2
+Version: 0.1.3
 Summary: A single unified Advanced Audio Processing toolkit, that provides both High-Level and Low-Level approaches to its extensive collection of tools.
-Home-page: UNKNOWN
+Home-page: https://github.com/heleusbrands/WaveForm/tree/main
 Author: Bloom Research
 Author-email: rosebloomresearch@gmail.com
 License: CC BY 4.0
 Description: ## WaveForm
         
         <span style="color:#E83A6B;"> by Bloom Research </span>
         ____
@@ -216,9 +216,16 @@
         - more...
         
         **WaveGraph**
         
         > WaveGraph is a module that's meant to act as universal automatic plotting utility. It reads the format that the date passed to it is in, and chooses an appropriate graph type automatically. If the data is an Air Array subclass, the format is determined based on which subclass contains the data. If not, it determines it based off the dimensionality of the data, and the content of the data, via the NDtype and subsequently the DimensionalType subclasses that are integrated into the Air module, which are designed for analyzing data to try and automatically determine what type of data it represents (i.e. Full Audio Data, Frequency, Decibel, Pascal, etc.)
         
         
+Keywords: Audio,Audio Processing,Rubberband,Pydub,pytsmod,nwaves,parselmouth,Audio Effects,Rose,Bloom,Audio Research,Formants,pyrubberband,Audio Features,WaveForm,WaveFormer,Sound Design,Audio Visualization,Audio Graph,Audio Array
 Platform: UNKNOWN
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Multimedia :: Sound/Audio
+Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
+Classifier: Topic :: Multimedia :: Sound/Audio :: Conversion
+Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
```

### Comparing `WaveFormer-0.1.2/README.md` & `WaveFormer-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.2/WaveFormer.egg-info/PKG-INFO` & `WaveFormer-0.1.3/WaveFormer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: WaveFormer
-Version: 0.1.2
+Version: 0.1.3
 Summary: A single unified Advanced Audio Processing toolkit, that provides both High-Level and Low-Level approaches to its extensive collection of tools.
-Home-page: UNKNOWN
+Home-page: https://github.com/heleusbrands/WaveForm/tree/main
 Author: Bloom Research
 Author-email: rosebloomresearch@gmail.com
 License: CC BY 4.0
 Description: ## WaveForm
         
         <span style="color:#E83A6B;"> by Bloom Research </span>
         ____
@@ -216,9 +216,16 @@
         - more...
         
         **WaveGraph**
         
         > WaveGraph is a module that's meant to act as universal automatic plotting utility. It reads the format that the date passed to it is in, and chooses an appropriate graph type automatically. If the data is an Air Array subclass, the format is determined based on which subclass contains the data. If not, it determines it based off the dimensionality of the data, and the content of the data, via the NDtype and subsequently the DimensionalType subclasses that are integrated into the Air module, which are designed for analyzing data to try and automatically determine what type of data it represents (i.e. Full Audio Data, Frequency, Decibel, Pascal, etc.)
         
         
+Keywords: Audio,Audio Processing,Rubberband,Pydub,pytsmod,nwaves,parselmouth,Audio Effects,Rose,Bloom,Audio Research,Formants,pyrubberband,Audio Features,WaveForm,WaveFormer,Sound Design,Audio Visualization,Audio Graph,Audio Array
 Platform: UNKNOWN
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Multimedia :: Sound/Audio
+Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
+Classifier: Topic :: Multimedia :: Sound/Audio :: Conversion
+Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
```

### Comparing `WaveFormer-0.1.2/WaveFormer.egg-info/SOURCES.txt` & `WaveFormer-0.1.3/WaveFormer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.2/audio_modules/air.py` & `WaveFormer-0.1.3/audio_modules/air.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.2/audio_modules/core/configs.py` & `WaveFormer-0.1.3/audio_modules/core/configs.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.2/audio_modules/core/informers.py` & `WaveFormer-0.1.3/audio_modules/core/informers.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.2/audio_modules/extraction/commands.py` & `WaveFormer-0.1.3/audio_modules/extraction/commands.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.2/audio_modules/extraction/core.py` & `WaveFormer-0.1.3/audio_modules/extraction/core.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.2/audio_modules/extraction/extract_configs.py` & `WaveFormer-0.1.3/audio_modules/extraction/extract_configs.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.2/audio_modules/extraction/xtgraph.py` & `WaveFormer-0.1.3/audio_modules/extraction/xtgraph.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.2/audio_modules/nvision/configs.py` & `WaveFormer-0.1.3/audio_modules/nvision/configs.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.2/audio_modules/nvision/core.py` & `WaveFormer-0.1.3/audio_modules/nvision/core.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.2/audio_modules/nvision/ngraph.py` & `WaveFormer-0.1.3/audio_modules/nvision/ngraph.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.2/audio_modules/nvision/plotly_mappings.py` & `WaveFormer-0.1.3/audio_modules/nvision/plotly_mappings.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.2/audio_modules/praat/configs.py` & `WaveFormer-0.1.3/audio_modules/praat/configs.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.2/audio_modules/praat/core.py` & `WaveFormer-0.1.3/audio_modules/praat/core.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.2/audio_modules/praat/filters.py` & `WaveFormer-0.1.3/audio_modules/praat/filters.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.2/audio_modules/praat/formant.py` & `WaveFormer-0.1.3/audio_modules/praat/formant.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.2/audio_modules/praat/handlers.py` & `WaveFormer-0.1.3/audio_modules/praat/handlers.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.2/audio_modules/praat/processor.py` & `WaveFormer-0.1.3/audio_modules/praat/processor.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.2/audio_modules/praat/spectrogram.py` & `WaveFormer-0.1.3/audio_modules/praat/spectrogram.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.2/audio_modules/types.py` & `WaveFormer-0.1.3/audio_modules/types.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.2/rubberband/options.py` & `WaveFormer-0.1.3/rubberband/options.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.2/rubberband/rubberbandstretcher.py` & `WaveFormer-0.1.3/rubberband/rubberbandstretcher.py`

 * *Files identical despite different names*

