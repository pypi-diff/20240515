# Comparing `tmp/beats_swing-0.0.1.tar.gz` & `tmp/beats_swing-0.1.0.tar.gz`

## Comparing `beats_swing-0.0.1.tar` & `beats_swing-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 beats_swing-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 beats_swing-0.0.1/Makefile
--rw-r--r--   0        0        0    13088 2020-02-02 00:00:00.000000 beats_swing-0.0.1/pylintrc
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 beats_swing-0.0.1/test_requirements.txt
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 beats_swing-0.0.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 beats_swing-0.0.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 beats_swing-0.0.1/scripts/explorer.py
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 beats_swing-0.0.1/scripts/first_pass.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 beats_swing-0.0.1/scripts/librosa_explorer.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 beats_swing-0.0.1/scripts/mess_around_w_librosa.py
--rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 beats_swing-0.0.1/scripts/score.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beats_swing-0.0.1/src/beats/__init__.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 beats_swing-0.0.1/src/beats/filtering.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 beats_swing-0.0.1/src/beats/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beats_swing-0.0.1/src/beats/estimators/__init__.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 beats_swing-0.0.1/src/beats/estimators/api.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 beats_swing-0.0.1/src/beats/estimators/librosa.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 beats_swing-0.0.1/src/beats/estimators/trivial.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 beats_swing-0.0.1/src/beats/estimators/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beats_swing-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beats_swing-0.0.1/tests/beats/__init__.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 beats_swing-0.0.1/tests/beats/test_smoke.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 beats_swing-0.0.1/.gitignore
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 beats_swing-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 beats_swing-0.0.1/README.md
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 beats_swing-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 beats_swing-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 beats_swing-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 beats_swing-0.1.0/Makefile
+-rw-r--r--   0        0        0    13088 2020-02-02 00:00:00.000000 beats_swing-0.1.0/pylintrc
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 beats_swing-0.1.0/test_requirements.txt
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 beats_swing-0.1.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 beats_swing-0.1.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 beats_swing-0.1.0/scripts/explorer.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 beats_swing-0.1.0/scripts/first_pass.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 beats_swing-0.1.0/scripts/librosa_explorer.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 beats_swing-0.1.0/scripts/mess_around_w_librosa.py
+-rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 beats_swing-0.1.0/scripts/score.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beats_swing-0.1.0/src/beats/__init__.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 beats_swing-0.1.0/src/beats/cli.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 beats_swing-0.1.0/src/beats/constants.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 beats_swing-0.1.0/src/beats/filtering.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 beats_swing-0.1.0/src/beats/shared_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beats_swing-0.1.0/src/beats/estimators/__init__.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 beats_swing-0.1.0/src/beats/estimators/api.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 beats_swing-0.1.0/src/beats/estimators/librosa.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 beats_swing-0.1.0/src/beats/estimators/trivial.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 beats_swing-0.1.0/src/beats/estimators/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beats_swing-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beats_swing-0.1.0/tests/beats/__init__.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 beats_swing-0.1.0/tests/beats/test_smoke.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 beats_swing-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 beats_swing-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 beats_swing-0.1.0/README.md
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 beats_swing-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 beats_swing-0.1.0/PKG-INFO
```

### Comparing `beats_swing-0.0.1/.pre-commit-config.yaml` & `beats_swing-0.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `beats_swing-0.0.1/Makefile` & `beats_swing-0.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `beats_swing-0.0.1/pylintrc` & `beats_swing-0.1.0/pylintrc`

 * *Files identical despite different names*

### Comparing `beats_swing-0.0.1/test_requirements.txt` & `beats_swing-0.1.0/test_requirements.txt`

 * *Files identical despite different names*

### Comparing `beats_swing-0.0.1/.github/workflows/publish.yml` & `beats_swing-0.1.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `beats_swing-0.0.1/.github/workflows/tests.yml` & `beats_swing-0.1.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `beats_swing-0.0.1/scripts/explorer.py` & `beats_swing-0.1.0/scripts/explorer.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import numpy as np
 import plotly.express as px
 import sounddevice as sd
 import streamlit as st
 from pydub import AudioSegment
 
 from beats.filtering import bass_lowpass
-from beats.types import Vector
+from beats.shared_types import Vector
 
 
 if __name__ == "__main__":
     st.title("mp3 explorer")
 
     mp3_dir = Path(__file__).parent.parent / "data"
     mp3 = st.selectbox(
```

### Comparing `beats_swing-0.0.1/scripts/first_pass.py` & `beats_swing-0.1.0/scripts/first_pass.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 import matplotlib.pyplot as plt
 import numpy as np
 from pydub import AudioSegment
 
 from beats.filtering import bass_band
-from beats.types import Vector
+from beats.shared_types import Vector
 
 
 if __name__ == "__main__":
     mp3_file = (
         Path(__file__).parent.parent
         / "data"
         / "Fats Waller - Ain’t Misbehavin’ (163).mp3"
```

### Comparing `beats_swing-0.0.1/scripts/librosa_explorer.py` & `beats_swing-0.1.0/scripts/librosa_explorer.py`

 * *Files identical despite different names*

### Comparing `beats_swing-0.0.1/scripts/mess_around_w_librosa.py` & `beats_swing-0.1.0/scripts/mess_around_w_librosa.py`

 * *Files identical despite different names*

### Comparing `beats_swing-0.0.1/scripts/score.py` & `beats_swing-0.1.0/scripts/score.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 
 from beats.estimators.api import Estimator
 from beats.estimators.librosa import Librosav1
 from beats.estimators.librosa import Librosav2
 from beats.estimators.trivial import Zero
 from beats.estimators.utils import Metrics
 from beats.estimators.utils import score
-from beats.types import SamplingRate
-from beats.types import Song
-from beats.types import Tempo
-from beats.types import Vector
+from beats.shared_types import SamplingRate
+from beats.shared_types import Song
+from beats.shared_types import Tempo
+from beats.shared_types import Vector
 
 
 def song_from_file(
     audio_file: Path,
 ) -> Tuple[Song, SamplingRate, Tempo]:  # TODO: cache?
     y, fs = librosa.load(str(audio_file), sr=None)
     # tempo should be encoded as the first 3 characters of the file name;
```

### Comparing `beats_swing-0.0.1/src/beats/filtering.py` & `beats_swing-0.1.0/src/beats/filtering.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from typing import Tuple
 
 from scipy.signal import butter
 from scipy.signal import filtfilt
 from scipy.signal import lfilter
 
-from beats.types import Vector
+from beats.shared_types import Vector
 
 
 # Source: https://www.teachmeaudio.com/mixing/techniques/audio-spectrum#bass
 BASS_FREQ: Tuple[float, float] = (40.0, 200.0)
 
 
 def bandpass_filter(
```

### Comparing `beats_swing-0.0.1/src/beats/estimators/api.py` & `beats_swing-0.1.0/src/beats/estimators/api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """This module defines the estimator API."""
 
 import abc
 from typing import Mapping
 
-from beats.types import SamplingRate
-from beats.types import Song
-from beats.types import Tempo
+from beats.shared_types import SamplingRate
+from beats.shared_types import Song
+from beats.shared_types import Tempo
 
 
 class Estimator(abc.ABC):
     """This is the interface for an estimator."""
 
     @abc.abstractmethod
     def tempo(self, song: Song, fs: SamplingRate) -> Tempo:
```

### Comparing `beats_swing-0.0.1/src/beats/estimators/librosa.py` & `beats_swing-0.1.0/src/beats/estimators/librosa.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Librosa-based tempo estimators."""
 
 from typing import Mapping
 
 import librosa
 
 from beats.estimators.api import Estimator
-from beats.types import SamplingRate
-from beats.types import Song
-from beats.types import Tempo
+from beats.shared_types import SamplingRate
+from beats.shared_types import Song
+from beats.shared_types import Tempo
 
 
 class Librosav1(Estimator):
     """Tempo estimator using `librosa.beat.beat_track`."""
 
     def __init__(self, start_bpm: float = 120.0, tightness: float = 100.0):
         self._start_bpm = start_bpm
```

### Comparing `beats_swing-0.0.1/src/beats/estimators/utils.py` & `beats_swing-0.1.0/src/beats/estimators/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import dataclasses
 
 import numpy as np
 import pandas as pd
 from sklearn.metrics import r2_score
 
-from beats.types import Vector
+from beats.shared_types import Vector
 
 
 @dataclasses.dataclass
 class Metrics:
     """A container with various performance metrics."""
 
     mean_squared_error: float
```

### Comparing `beats_swing-0.0.1/.gitignore` & `beats_swing-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `beats_swing-0.0.1/LICENSE.txt` & `beats_swing-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `beats_swing-0.0.1/README.md` & `beats_swing-0.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -2,29 +2,47 @@
 
 ![tests](https://github.com/elvijs/beats/workflows/main/badge.svg)
 ![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)
 ![Black](https://img.shields.io/badge/code%20style-black-000000.svg)
 
 # What is it?
 
-Determine the tempo of a song from its mp3.
+Determine the tempo of a song from its mp3. Designed for swing music. May work in other cases as well.
+
+# Usage
+
+## Non-Python dependencies
+
+```console
+$ sudo apt install ffmpeg
+```
+
+TODO: describe how to use the CLI
 
 # Development
 
-## Prerequisites
+## Algorithm development
+
+### Scoring new estimators
+
+TODO: document how to score their songs.
+
+### Streamlit apps
+
+TODO
 
-`sudo apt install ffmpeg`
+## Package development
 
-## Install (dev mode)
+### Install in dev mode
 
 ```console
 $ make install
 ```
 
-## Usage
+### Common dev tasks
 
 * Auto-format: `make format`
 * Run static checkers: `make statec_checks`
 * Freeze the local env into `test_requirements` (say, after installing new deps):
   `make freeze_requirements`.
 
 ## Issues
```

### Comparing `beats_swing-0.0.1/pyproject.toml` & `beats_swing-0.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "beats_swing"
-version = "0.0.1"
+version = "0.1.0"
 description = "Determine the tempo of an mp3 song. Tweaked for swing music."
 authors = [
     {name = "Elvijs Sarkans", email = "elvijs.sarkans@gmail.com"}
 ]
 readme = "README.md"
 requires-python = ">=3.11"
 
@@ -24,14 +24,17 @@
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
+[project.scripts]
+beats = "beats.cli:main"
+
 [project.urls]
 repository = "https://github.com/elvijs/beats"
 homepage = "https://github.com/elvijs/beats"
 issues = "https://github.com/elvijs/beats/issues"
 
 
 [tool.pytest.ini_options]
```

### Comparing `beats_swing-0.0.1/PKG-INFO` & `beats_swing-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: beats_swing
-Version: 0.0.1
+Version: 0.1.0
 Summary: Determine the tempo of an mp3 song. Tweaked for swing music.
 Project-URL: repository, https://github.com/elvijs/beats
 Project-URL: homepage, https://github.com/elvijs/beats
 Project-URL: issues, https://github.com/elvijs/beats/issues
 Author-email: Elvijs Sarkans <elvijs.sarkans@gmail.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
@@ -24,29 +24,47 @@
 
 ![tests](https://github.com/elvijs/beats/workflows/main/badge.svg)
 ![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)
 ![Black](https://img.shields.io/badge/code%20style-black-000000.svg)
 
 # What is it?
 
-Determine the tempo of a song from its mp3.
+Determine the tempo of a song from its mp3. Designed for swing music. May work in other cases as well.
+
+# Usage
+
+## Non-Python dependencies
+
+```console
+$ sudo apt install ffmpeg
+```
+
+TODO: describe how to use the CLI
 
 # Development
 
-## Prerequisites
+## Algorithm development
+
+### Scoring new estimators
+
+TODO: document how to score their songs.
+
+### Streamlit apps
+
+TODO
 
-`sudo apt install ffmpeg`
+## Package development
 
-## Install (dev mode)
+### Install in dev mode
 
 ```console
 $ make install
 ```
 
-## Usage
+### Common dev tasks
 
 * Auto-format: `make format`
 * Run static checkers: `make statec_checks`
 * Freeze the local env into `test_requirements` (say, after installing new deps):
   `make freeze_requirements`.
 
 ## Issues
```

