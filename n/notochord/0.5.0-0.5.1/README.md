# Comparing `tmp/notochord-0.5.0.tar.gz` & `tmp/notochord-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notochord-0.5.0.tar", max compression
+gzip compressed data, was "notochord-0.5.1.tar", max compression
```

## Comparing `notochord-0.5.0.tar` & `notochord-0.5.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1084 2023-11-28 17:22:02.563723 notochord-0.5.0/LICENSE
--rw-r--r--   0        0        0     5191 2024-03-16 00:07:55.452937 notochord-0.5.0/README.md
--rw-r--r--   0        0        0      764 2024-03-15 23:49:34.317574 notochord-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       87 2023-11-28 17:22:02.566423 notochord-0.5.0/src/notochord/__init__.py
--rw-r--r--   0        0        0      867 2023-11-28 17:22:02.566475 notochord-0.5.0/src/notochord/__main__.py
--rw-r--r--   0        0        0      163 2023-11-28 17:22:02.566552 notochord-0.5.0/src/notochord/app/__init__.py
--rw-r--r--   0        0        0      316 2023-11-28 17:22:02.566610 notochord-0.5.0/src/notochord/app/harmonizer.css
--rw-r--r--   0        0        0    10522 2023-11-28 17:22:02.566797 notochord-0.5.0/src/notochord/app/harmonizer.py
--rw-r--r--   0        0        0     1558 2024-03-15 23:37:21.311846 notochord-0.5.0/src/notochord/app/homunculus.css
--rw-r--r--   0        0        0    40348 2024-03-15 23:37:21.312518 notochord-0.5.0/src/notochord/app/homunculus.py
--rw-r--r--   0        0        0    18983 2023-11-28 17:22:02.567055 notochord-0.5.0/src/notochord/app/improviser-txala.py
--rw-r--r--   0        0        0      385 2023-11-28 17:22:02.567122 notochord-0.5.0/src/notochord/app/improviser.css
--rw-r--r--   0        0        0    19710 2024-03-15 23:37:21.312878 notochord-0.5.0/src/notochord/app/improviser.py
--rw-r--r--   0        0        0     4752 2023-11-28 17:22:02.567254 notochord-0.5.0/src/notochord/app/preset.json
--rw-r--r--   0        0        0     2091 2023-12-16 16:51:15.812048 notochord-0.5.0/src/notochord/app/server.py
--rw-r--r--   0        0        0     3073 2023-11-28 17:22:02.567375 notochord-0.5.0/src/notochord/app/simple_harmonizer.py
--rw-r--r--   0        0        0    10631 2024-03-15 23:37:21.313178 notochord-0.5.0/src/notochord/data.py
--rw-r--r--   0        0        0    12790 2023-11-28 17:22:02.567536 notochord-0.5.0/src/notochord/distributions.py
--rw-r--r--   0        0        0    46919 2024-03-15 23:37:21.313772 notochord-0.5.0/src/notochord/model.py
--rw-r--r--   0        0        0    12706 2024-03-15 23:37:21.314168 notochord-0.5.0/src/notochord/perform.py
--rw-r--r--   0        0        0     2528 2023-11-28 17:22:02.567874 notochord-0.5.0/src/notochord/rnn.py
--rw-r--r--   0        0        0    13940 2024-03-15 23:37:21.314427 notochord-0.5.0/src/notochord/train.py
--rw-r--r--   0        0        0     2488 2023-11-28 17:22:02.568040 notochord-0.5.0/src/notochord/util.py
--rw-r--r--   0        0        0     5983 1970-01-01 00:00:00.000000 notochord-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-11-28 17:22:02.563723 notochord-0.5.1/LICENSE
+-rw-r--r--   0        0        0     4650 2024-05-15 20:23:17.997516 notochord-0.5.1/README.md
+-rw-r--r--   0        0        0      833 2024-05-15 20:38:01.811173 notochord-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0       87 2023-11-28 17:22:02.566423 notochord-0.5.1/src/notochord/__init__.py
+-rw-r--r--   0        0        0      898 2024-05-15 20:23:17.997905 notochord-0.5.1/src/notochord/__main__.py
+-rw-r--r--   0        0        0      163 2023-11-28 17:22:02.566552 notochord-0.5.1/src/notochord/app/__init__.py
+-rw-r--r--   0        0        0      316 2023-11-28 17:22:02.566610 notochord-0.5.1/src/notochord/app/harmonizer.css
+-rw-r--r--   0        0        0    10522 2023-11-28 17:22:02.566797 notochord-0.5.1/src/notochord/app/harmonizer.py
+-rw-r--r--   0        0        0     1479 2024-05-15 20:23:17.998076 notochord-0.5.1/src/notochord/app/homunculus.css
+-rw-r--r--   0        0        0    44887 2024-05-15 20:23:17.998440 notochord-0.5.1/src/notochord/app/homunculus.py
+-rw-r--r--   0        0        0    18983 2023-11-28 17:22:02.567055 notochord-0.5.1/src/notochord/app/improviser-txala.py
+-rw-r--r--   0        0        0      385 2023-11-28 17:22:02.567122 notochord-0.5.1/src/notochord/app/improviser.css
+-rw-r--r--   0        0        0    19710 2024-04-24 13:59:31.571434 notochord-0.5.1/src/notochord/app/improviser.py
+-rw-r--r--   0        0        0     4842 2024-05-15 20:23:17.998613 notochord-0.5.1/src/notochord/app/preset.json
+-rw-r--r--   0        0        0     4413 2024-05-15 20:23:17.998802 notochord-0.5.1/src/notochord/app/server.py
+-rw-r--r--   0        0        0     3073 2023-11-28 17:22:02.567375 notochord-0.5.1/src/notochord/app/simple_harmonizer.py
+-rw-r--r--   0        0        0    10631 2024-04-24 13:59:31.572536 notochord-0.5.1/src/notochord/data.py
+-rw-r--r--   0        0        0    12790 2023-11-28 17:22:02.567536 notochord-0.5.1/src/notochord/distributions.py
+-rw-r--r--   0        0        0    47353 2024-05-15 20:23:17.999241 notochord-0.5.1/src/notochord/model.py
+-rw-r--r--   0        0        0    12706 2024-04-24 13:59:31.573908 notochord-0.5.1/src/notochord/perform.py
+-rw-r--r--   0        0        0     2528 2023-11-28 17:22:02.567874 notochord-0.5.1/src/notochord/rnn.py
+-rw-r--r--   0        0        0    13940 2024-04-24 13:59:31.574327 notochord-0.5.1/src/notochord/train.py
+-rw-r--r--   0        0        0     2488 2023-11-28 17:22:02.568040 notochord-0.5.1/src/notochord/util.py
+-rw-r--r--   0        0        0     5443 1970-01-01 00:00:00.000000 notochord-0.5.1/PKG-INFO
```

### Comparing `notochord-0.5.0/LICENSE` & `notochord-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `notochord-0.5.0/README.md` & `notochord-0.5.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -5,72 +5,70 @@
 </div>
 
 Notochord is a neural network model for MIDI performances. This package contains the training and inference model implemented in pytorch, as well as interactive MIDI processing apps using iipyper. 
 <!-- Some further examples involving SuperCollider and TidalCycles can be found in the parent repo under `examples`. -->
 
 ## Getting Started
 
-Using your python environment manager of choice (i.e. virtualenv, [conda](https://github.com/conda-forge/miniforge)), make a new environment with a Python version at least 3.10. Then `pip install notochord`.
+Using your python environment manager of choice (e.g. virtualenv, [conda](https://github.com/conda-forge/miniforge)), make a new environment with a Python version at least 3.10. Then `pip install notochord`.
 
 For developing `notochord`, see our [dev repo](https://github.com/Intelligent-Instruments-Lab/iil-dev.git)
 
-<!-- Follow the instructions in the root repo to set up an `iil-python-tools` environment. Then download a model checkpoint (e.g. `notochord_lakh_50G_deep.pt`) from the releases page: https://github.com/Intelligent-Instruments-Lab/iil-python-tools/releases . From here, I'll assume the model file is saved at `~/Downloads/notochord_lakh_50G_deep.pt`. -->
-
 ### Install fluidsynth (optional)
 [fluidsynth](https://github.com/FluidSynth/fluidsynth) is a General MIDI synthesizer which you can install from the package manager. On macOS:
 ```
 brew install fluidsynth
 ```
 fluidsynth needs a soundfont to run, like this one: https://drive.google.com/file/d/1-cwBWZIYYTxFwzcWFaoGA7Kjx5SEjVAa/view
 
 run fluidsynth in a terminal. For example, `fluidsynth -v -o midi.portname="fluidsynth" -o synth.midi-bank-select=mma ~/'Downloads/soundfonts/Timbres of Heaven (XGM) 4.00(G).sf2'`
 
 ## Notochord MIDI Apps
 
 Notochord includes several [iipyper](https://github.com/Intelligent-Instruments-Lab/iipyper.git) apps which can be run in a terminal. They have a clickable text-mode user interface and connect directly to MIDI ports, so you can wire them up to your controllers, DAW, etc.
 
-The Notochord harmonizer adds extra concurrent notes for each MIDI note you play in. In a terminal, make sure the `iil-python-tools` conda environment is active (`conda activate iil-python-tools`) and run:
+The Notochord harmonizer adds extra concurrent notes for each MIDI note you play in. In a terminal, make sure your notochord Python environment is active and run:
 ```
-python -m notochord harmonizer
+notochord harmonizer
 ```
-try `python -m notochord harmonizer --help`
+try `notochord harmonizer --help`
 to see more options.
 
-the ``homunculus'' gives you a UI to manage multiple input, harmonizing or autonomous notochord channels:
+the "homunculus" gives you a UI to manage multiple input, harmonizing or autonomous notochord channels:
 ```
-python -m notochord homunculus
+notochord homunculus
 ```
 You can set the MIDI in and out ports with `--midi-in` and `--midi-out`. If you use a General MIDI synthesizer like fluidsynth, you can add `--send-pc` to also send program change messages.
 
 If you are using fluidsynth, try:
 ```
-python -m notochord homunculus --send-pc --midi-out fluidsynth --thru
+notochord homunculus --send-pc --midi-out fluidsynth --thru
 ```
 
 ## Python API
 
-See the docstrings for `Notochord.feed` and `Notochord.query` in `notochord/model.py` for the low-level Notochord inference API which can be used from Python code. `notochord/app/simple_harmonizer.py` provides a minimal example of how to build an interactive app.
+See the docs for `Notochord.feed` and `Notochord.query` for the low-level Notochord inference API which can be used from Python code. `notochord/app/simple_harmonizer.py` provides a minimal example of how to build an interactive app.
 
 ## OSC server
 
 You can also expose the inference API over Open Sound Control:
 ```
-python -m notochord server
+notochord server
 ```
 this will run notochord and listen continously for OSC messages.
 
 <!-- `examples/notochord/generate-demo.scd` and `examples/notochord/harmonize-demo.scd` are example scripts for interacting with the notochord server from SuperCollider. -->
 
 ## Tidal interface
 
-see `examples/notochord/tidalcycles` in the archived [iil-python-tools](https://github.com/Intelligent-Instruments-Lab/iil-python-tools/tree/master/examples) repo (updated examples coming soon):
+see `notochord/tidalcycles` in [iil-examples](https://github.com/Intelligent-Instruments-Lab/iil-examples.git) repo (updated examples coming soon):
 
 add `Notochord.hs` to your tidal boot file. Probably replace the `tidal <- startTidal` line with something like:
 ```haskell
-:script ~/iil-python-tools/examples/notochord/tidalcycles/Notochord.hs
+:script ~/iil-examples/notochord/tidalcycles/Notochord.hs
 
 let sdOscMap = (superdirtTarget, [superdirtShape])
 let oscMap = [sdOscMap,ncOscMap]
 
 tidal <- startStream defaultConfig {cFrameTimespan = 1/240} oscMap
 ```
```

### Comparing `notochord-0.5.0/pyproject.toml` & `notochord-0.5.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 [tool.poetry]
 name = "notochord"
-version = "0.5.0"
-description = " Notochord is a real-time neural network model for MIDI performances. "
+version = "0.5.1"
+description = "Notochord is a real-time neural network model for MIDI performances."
 authors = ["Victor Shepardson <victor.shepardson@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.10"
-torch = ">=1.13,<3"
+python = ">=3.10,<3.13"
+torch = ">=1.13,<2.3"
 numpy = "^1.23"
-pandas = "^1.5"
+pandas = "^2.0"
 tqdm = "^4.64"
 sf2utils = "^0.9"
 appdirs = "^1.4.4"
-iipyper = "~0.1.0"
+iipyper = "~0.1.2"
 
 [tool.poetry.group.dev.dependencies]
 mkdocs = "^1.5.3"
 mkdocstrings = {extras = ["python"], version = "^0.23.0"}
 mkdocs-gen-files = "^0.5.0"
 mkdocs-include-markdown-plugin = "^6.0.4"
 mkdocs-material = "^9.4.8"
 mkdocs-material-extensions = "^1.3"
 mkdocs-autorefs = "^0.5.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.poetry.scripts]
+notochord = 'notochord.__main__:_main'
```

### Comparing `notochord-0.5.0/src/notochord/app/harmonizer.py` & `notochord-0.5.1/src/notochord/app/harmonizer.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.0/src/notochord/app/homunculus.css` & `notochord-0.5.1/src/notochord/app/homunculus.css`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 TUI {
     layout: vertical;
 }
 
 NotoControl {
     layout: horizontal;
     background: $boost;
-    height: 5;
-    margin: 1;
+    height: 4;
+    # margin: 1;
     min-width: 50;
-    padding: 1;
+    # padding: 1;
     dock: bottom;
 }
 
 NotoPresets {
     /* layout: horizontal; */
     /* width: 1fr; */
     layout: grid;
@@ -67,34 +67,31 @@
 InstrumentSelect Grid {
     grid-size: 8 16;
 }
 InstrumentSelect Button {
     border: none;
     min-width: 5;
     height: 2;
-    /* border-top: none; */
-    /* border-bottom: none; */
-    /* border-left: none; */
-    /* border-right: none; */
 
 }
 
 /* MixerButtons Button {
     height: 5;
     border: solid purple;
 } */
 
 NotoPrediction {
     content-align: center middle;
     height: 3;
 }
 
-TextLog {
-    height: 1fr;
-    border: solid purple;
+NotoLog {
+    height: 0.5fr;
+    # border: tall purple;
+    outline-top: double purple;
 }
 
 Button {
     /* outline: solid red; */
     width: 16;
 }
```

### Comparing `notochord-0.5.0/src/notochord/app/homunculus.py` & `notochord-0.5.1/src/notochord/app/homunculus.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,32 +20,38 @@
 # TODO: grey out predictions when player or muted notochord
 
 # TODO: controls display panel
 # TODO: held notes display panel
 # TODO: counts / weights display panel
 # TODO: MIDI learn
 
+import time
+
 from typing import Optional, Dict, Any
 from numbers import Number
 import math
 import functools as ft
 import json
 from pathlib import Path
 from collections import defaultdict
+from datetime import datetime
 
 import numpy as np
 
+import torch
+torch.set_num_threads(1)
+
 import iipyper, notochord
 from notochord import Notochord, NotoPerformance
 from iipyper import OSC, MIDI, run, Stopwatch, repeat, cleanup, TUI, profile, lock
 
 from rich.panel import Panel
 from rich.pretty import Pretty
 from textual.reactive import reactive
-from textual.widgets import Header, Footer, Static, Button, RichLog, Label
+from textual.widgets import Header, Footer, Static, Button, Log, RichLog, Label
 from textual.screen import Screen
 from textual.containers import Grid
 
 def main(
     checkpoint="notochord-latest.ckpt", # Notochord checkpoint
     config:Dict[int,Dict[str,Any]]=None, # map MIDI channel : GM instrument
 
@@ -73,17 +79,38 @@
     predict_input=True, # forecasted next events can be for input (preserves model distribution, but can lead to Notochord deciding not to play)
     predict_follow=False,
     debug_query=False, # don't query notochord when there is no pending event.
     testing=False,
     estimated_latency=1e-2,
     soundfont=None,
     limit_input=None,
-    thru_vel_offset=None
+    thru_vel_offset=None,
+    profiler=0,
     ):
     """
+    This a terminal app for using Notochord interactively with MIDI controllers and synthesizers. Arguments to main can be given on the command line as flags, for example:
+
+    `python -m notochord homunculus --initial-query --config '{1:{mode:auto, inst:1}}'`
+    
+    16 voices correspond to the 16 MIDI channels. Each voice can be in one of three modes:
+
+        * input (appearing like "-->01"), voice 1 comes from MIDI input channel 1.
+        * follow (appearing like "01->02"), voice 2 plays whenever voice 1 plays.
+        * auto (appearing like just "03"), voice 3 plays autonomously.
+
+    Click the top section of each voice to cycle the mode.
+
+    Each voice is also assigned a [General MIDI instrument](https://en.wikipedia.org/wiki/General_MIDI#Program_change_events). Each 'input' and 'auto' voice should have a unique General MIDI instrument, but 'follow' voices can be duplicates of other voices. 
+
+    Click the middle section of each voice to choose a new instrument.
+
+    The bottom section of each voice allows muting individual voices.
+
+    Along the bottom, there are global query, sustain, mute and reset buttons. Query manually replaces the next pending note. Sustain stops all auto voices from playing without ending any open notes. Mute ends all open notes and stops auto voices. Reset ends all open notes, forgets all context and sets the Notochord model to its initial state.
+
     Args:
         checkpoint: path to notochord model checkpoint.
 
         config: mapping from MIDI channels to voice specs.
             MIDI channels and General MIDI instruments are indexed from 1.
             see https://en.wikipedia.org/wiki/General_MIDI for instrument numbers.
             There are 3 modes of voice: 'auto', 'follow' and 'input'.
@@ -290,14 +317,16 @@
         for c,i in channel_insts():
             do_send_pc(c, i)
     
     # load notochord model
     try:
         noto = Notochord.from_checkpoint(checkpoint)
         noto.eval()
+        noto.feed(0,0,0,0)
+        noto.query()
         noto.reset()
     except Exception:
         print("""error loading notochord model""")
         raise
 
     # main stopwatch to track time difference between MIDI events
     stopwatch = Stopwatch()
@@ -317,18 +346,20 @@
 
     follow_status = {'depth':0}
 
     def display_event(tag, memo, inst, pitch, vel, channel, **kw):
         """print an event to the terminal"""
         if tag is None:
             return
-        s = f'{tag}:\t {inst=:4d}    {pitch=:4d}    {vel=:4d}    {channel=:3d}'
+        now = str(datetime.now())[:-2]
+        s = f'{now}   inst {inst:3d}   pitch {pitch:3d}   vel {vel:3d}   ch {channel:2d} {tag}'
+        # s = f'{tag}:\t{inst=:4d}   {pitch=:4d}   {vel=:4d}   {channel=:3d}'
         if memo is not None:
-            s += f'    ({memo})'
-        tui(note=s)
+            s += f' ({memo})'
+        tui.defer(note=s)
 
     def play_event(
             event, channel, 
             parent=None, # parent note as (channel, inst, pitch)
             feed=True, 
             send=True, 
             tag=None, memo=None):
@@ -337,36 +368,42 @@
         vel = event['vel'] = math.ceil(event['vel'])
         dt = stopwatch.punch()
         if 'time' not in event or not nominal_time:
             event['time'] = dt
 
         # send out as MIDI
         if send:
-            midi.send(
-                'note_on' if vel > 0 else 'note_off', 
-                note=event['pitch'], velocity=vel, channel=channel-1)
+            with profile('\tmidi.send', print=print, enable=profiler>1):
+                midi.send(
+                    'note_on' if vel > 0 else 'note_off', 
+                    note=event['pitch'], velocity=vel, channel=channel-1)
 
         # print
-        display_event(tag, memo=memo, channel=channel, **event)
+        with profile('\tdisplay_event', print=print, enable=profiler>1):
+            display_event(
+                tag, memo=memo, channel=channel, **event)
 
         if feed:
             # feed to NotoPerformance
             # put a stopwatch in the held_note_data field for tracking note length
-            history.feed(held_note_data={
-                'duration':Stopwatch(),
-                'parent':parent
-                }, channel=channel, **event)
+            with profile('\thistory.feed', print=print, enable=profiler>1):
+                history.feed(held_note_data={
+                    'duration':Stopwatch(),
+                    'parent':parent
+                    }, channel=channel, **event)
             # feed to model
-            noto.feed(**event)
+            with profile('\tnoto.feed', print=print, enable=profiler>1):
+                noto.feed(**event)
 
         follow_status['depth'] += 1
-        # print(f'{follow_status=}')
-        follow_event(event, channel)
-        follow_status['depth'] -= 1
-        # print(f'{follow_status=}')
+        with profile('\t'*follow_status['depth']+'follow.event', print=print, enable=profiler>1):
+            # print(f'{follow_status=}')
+            follow_event(event, channel)
+            follow_status['depth'] -= 1
+            # print(f'{follow_status=}')
 
     def follow_event(source_event, source_channel):
         source_vel = source_event['vel']
         source_pitch = source_event['pitch']
         source_inst = source_event['inst']
         source_k = (source_channel, source_inst, source_pitch)
 
@@ -430,31 +467,32 @@
     # @lock
     def noto_reset():
         """reset Notochord and end all of its held notes"""
         print('RESET')
 
         # cancel pending predictions
         pending.event = None
-        tui(prediction=pending.event)
+        tui.defer(prediction=pending.event)
         
         # end Notochord held notes
         # for (chan,inst,pitch) in history.note_triples:
         for note in history.notes:
             if note.inst in mode_insts('auto'):
                 play_event(
                     dict(inst=note.inst, pitch=note.pitch, vel=0),
                     channel=note.chan, 
                     feed=False, # skip feeding Notochord since we are resetting it
                     tag='NOTO', memo='reset')
-        # reset stopwatch
-        stopwatch.punch()
+                
         # reset notochord state
         noto.reset()
         # reset history
         history.push()
+        # reset stopwatch
+        stopwatch.punch()
 
         # TODO: feed note-ons from any held input/follower notes?
 
         # query the fresh notochord for a new prediction
         if pending.gate:
             auto_query()
 
@@ -473,15 +511,15 @@
         # if unmuting, we're done
         if pending.gate:
             if sustain:
                 auto_query()
             return
         # cancel pending predictions
         pending.event = None
-        tui(prediction=pending.event)
+        tui.defer(prediction=pending.event)
 
         if sustain:
             return
         
         # end+feed all held notes
         # for (chan,inst,pitch) in history.note_triples:
         for note in history.notes:
@@ -498,42 +536,42 @@
         for (_, inst, pitch), note_data in history.note_data.items():
             dur = note_data['duration'].read()
             if (
                 inst in mode_insts('auto') 
                 and dur > max_note_len*(.1+controls.get('steer_duration', 1))
                 ):
                 # query for the end of a note with flexible timing
-                # with profile('query', print=print):
+                # with profile('query', print=print, enable=profiler):
                 t = stopwatch.read()
                 pending.event = noto.query(
                     next_inst=inst, next_pitch=pitch,
                     next_vel=0, min_time=t, max_time=t+0.5)
                 print(f'END STUCK NOTE {inst=},{pitch=}')
-                tui(prediction=pending.event)
+                tui.defer(prediction=pending.event)
                 return
 
         # all_insts = mode_insts(('auto', 'input', 'follow'), allow_muted=True)
         # counts = history.inst_counts(n=n_recent, insts=all_insts)
         counts = defaultdict(int)
         for i,c in history.inst_counts(n=n_recent).items():
             counts[i] = c
-        print(f'{counts=}')
+        # print(f'{counts=}')
 
         inst_modes = ['auto']
         if predict_follow:
             inst_modes.append('follow')
         if predict_input:
             inst_modes.append('input')
         allowed_insts = mode_insts(inst_modes, allow_muted=False)
 
         # assert len(allowed_insts - all_insts)==0, (allowed_insts, all_insts)
 
         # held_notes = history.held_inst_pitch_map(all_insts)
         held_notes = history.held_inst_pitch_map()
-        print(f'{held_notes=}')
+        # print(f'{held_notes=}')
 
         steer_time = 1-controls.get('steer_rate', 0.5)
         steer_pitch = controls.get('steer_pitch', 0.5)
         steer_density = controls.get('steer_density', 0.5)
         
         tqt = (max(0,steer_time-0.5), min(1, steer_time+0.5))
         tqp = (max(0,steer_pitch-0.5), min(1, steer_pitch+0.5))
@@ -541,26 +579,30 @@
         # if using nominal time,
         # *subtract* estimated feed latency to min_time; (TODO: really should
         #   set no min time when querying, use stopwatch when re-querying...)
         # if using actual time, *add* estimated query latency
         time_offset = -5e-3 if nominal_time else 10e-3
         min_time = stopwatch.read()+time_offset
 
+        # idea: maintain an 'instrument presence' quantity
+        # incorporating time since / number of notes was playing
+        # ideally this would distinguish sustained from percussive instruments too
+        
         # balance_sample: note-ons only from instruments which have played less
         inst_weights = None
         if balance_sample:
             inst_weights = {}
             mc = max(counts.values()) if len(counts) else 0
             for i in allowed_insts:
                 # if i in counts:
                 inst_weights[i] = np.exp(max(0, mc - counts[i] - n_margin))
                 # else:
                     # inst_weights[i] = 1.
 
-        print(f'{inst_weights=}')
+        # print(f'{inst_weights=}')
 
         # VTIP is better for time interventions,
         # VIPT is better for instrument interventions
         if min_time > estimated_latency or abs(tqt) > abs(tqp):
             query_method = noto.query_vtip
         else:
             query_method = noto.query_vipt
@@ -579,52 +621,63 @@
             for i in allowed_insts
             if i in held_notes
         }
 
         max_t = None if max_time is None else max(max_time, min_time+0.2)
 
         try:
-            pending.event = query_method(
-                note_on_map, note_off_map,
-                min_time=min_time, max_time=max_t,
-                truncate_quantile_time=tqt,
-                truncate_quantile_pitch=tqp,
-                steer_density=steer_density,
-                inst_weights=inst_weights,
-                no_steer=mode_insts(('input','follow'), allow_muted=False),
-            )
+            with profile('\tquery_method', print=print, enable=profiler>1):
+                pending.event = query_method(
+                    note_on_map, note_off_map,
+                    min_time=min_time, max_time=max_t,
+                    truncate_quantile_time=tqt,
+                    truncate_quantile_pitch=tqp,
+                    steer_density=steer_density,
+                    inst_weights=inst_weights,
+                    no_steer=mode_insts(('input','follow'), allow_muted=False),
+                )
         except Exception:
             # print(f'WARNING: query failed. {allowed_insts=} {note_on_map=} {note_off_map=}')
             pending.event = None
 
         # display the predicted event
-        tui(prediction=pending.event)
+        tui.defer(prediction=pending.event)
 
     #### MIDI handling
 
     # print all incoming MIDI for debugging
     if dump_midi:
         @midi.handle
         def _(msg):
             print(msg)
 
-    @midi.handle(type='program_change')
-    def _(msg):
-        """Program change events set instruments"""
-        raise NotImplementedError
+    # @midi.handle(type='program_change')
+    # def _(msg):
+        # """
+        # Program change events set GM instruments on the corresponding channel
+        # """
+        # raise NotImplementedError
 
     @midi.handle(type='pitchwheel')
     def _(msg):
+        """
+        pitchwheel affects steer_pitch
+        """
         controls['steer_pitch'] = (msg.pitch+8192)/16384
         # print(controls)
 
     # very basic CC handling for controls
     @midi.handle(type='control_change')
     def _(msg):
-        """CC messages on any channel"""
+        """
+        these are global controls listening on all channels: 
+        CC 01: steer pitch (>64 higher pitches, <64 lower)
+        CC 02: steer density (>64 more simultaneous notes, <64 fewer)
+        CC 03: steer rate (>64 more events, <64 fewer)
+        """
 
         if msg.control==1:
             controls['steer_pitch'] = msg.value/127
             print(f"{controls['steer_pitch']=}")
         if msg.control==2:
             controls['steer_density'] = msg.value/127
             print(f"{controls['steer_density']=}")
@@ -637,15 +690,15 @@
         if msg.control==5:
             auto_query()
         if msg.control==6:
             noto_mute()
 
     # very basic OSC handling for controls
     if osc_port is not None:
-        @osc.args('/notochord/improviser/*')
+        @osc.args('/notochord/homunculus/*')
         def _(route, *a):
             print('OSC:', route, *a)
             ctrl = route.split['/'][3]
             if ctrl=='reset':
                 noto_reset()
             elif ctrl=='query':
                 auto_query()
@@ -659,15 +712,19 @@
                 print(controls)
 
     input_sw = Stopwatch()
     dropped = set()# (channel, pitch)
     input_dts = []
     @midi.handle(type=('note_on', 'note_off'))
     def _(msg):
-        """MIDI NoteOn events from the player"""
+        """
+        MIDI NoteOn and NoteOff events affect input channels
+        e.g. a channel displaying -->01 will listen to note events on channel 1
+        a channel displaying 02->03 will follow note events on channel 2
+        """
         # convert from 0-index
         channel = msg.channel+1
 
         if channel not in mode_chans('input'):
             print(f'WARNING: ignoring MIDI {msg} on non-input channel')
             return
         
@@ -702,15 +759,15 @@
             return
         if vel>0 and limit_input and input_dens>limit_input:
             print(f'WARNING: ignoring rate-limited input {input_dens=}')
             dropped.add(k)
             return 
 
         # feed event to Notochord
-        # with profile('feed', print=print):
+        # with profile('feed', print=print, enable=profiler):
         play_event(
             {'inst':inst, 'pitch':pitch, 'vel':vel}, 
             channel=channel, send=thru, tag='PLAYER')
 
         # query for new prediction
         auto_query()
 
@@ -720,14 +777,15 @@
     def auto_event():
         # 'auto' event happens:
         event = pending.event
         inst, pitch, vel = event['inst'], event['pitch'], math.ceil(event['vel'])
         chan = auto_inst_channel(inst)
 
         # note on which is already playing or note off which is not
+
         if (vel>0) == ((inst, pitch) in history.note_pairs): 
             print(f're-query for invalid {vel=}, {inst=}, {pitch=}')
             auto_query()
             return
         
         play_event(event, channel=chan, tag='NOTO')
 
@@ -741,19 +799,21 @@
             not testing and
             pending.gate and
             stopwatch.read() > dt
             ):
             # if so, check if it is a notochord-controlled instrument
             if pending.event['inst'] in mode_insts('auto'):
                 # prediction happens
-                auto_event()
+                with profile('auto_event', print=print, enable=profiler):
+                    auto_event()
             # query for new prediction
             if dt < noto.max_dt and not debug_query:
             # if not debug_query:
-                auto_query()
+                with profile('auto_query', print=print, enable=profiler):
+                    auto_query()
 
     @cleanup
     def _():
         """end any remaining notes"""
         # print(f'cleanup: {notes=}')
         # for (chan,inst,pitch) in history.note_triples:
         for note in history.notes:
@@ -772,15 +832,20 @@
         for p,k in enumerate(presets):
             tui.set_preset(p, k)
 
     @tui.on
     def mount():
         update_config()
         update_presets()
-
+        print('welcome to notochord homunculus')
+        print('MIDI handling:')
+        print(midi.get_docs())
+        if osc_port is not None:
+            print('OSC handling:')
+            print(osc.get_docs())
 
     ### set_* does whatever necessary to change channel properties
     ### calls update_config() to keep the UI in sync
 
     def set_mode(c, m, update=True):
         if c in config:
             prev_m = config[c]['mode']
@@ -832,15 +897,14 @@
             )
         def on_button_pressed(self, event: Button.Pressed) -> None:
             # print(event.button.id)
             # i = 1
             i = int(event.button.id.split('_')[-1])
             self.app.pop_screen()
             set_inst(self.channel, i)
-    # inst_select = InstrumentSelect(None)
 
     def set_inst(c, i, update=True):
         print(f'SET INSTRUMENT {i}')
         if c in config:
             prev_i = config[c]['inst']
         else:
             prev_i = None
@@ -965,18 +1029,18 @@
     if initial_query:
         auto_query(predict_input=False, predict_follow=False)
 
     if use_tui:
         tui.run()
 
 ### def TUI components ###
-class NotoLog(RichLog):
+class NotoLog(Log):
     value = reactive('')
     def watch_value(self, time: float) -> None:
-        self.write(self.value)
+        self.write_line(self.value)
 
 class NotoPrediction(Static):
     value = reactive(None)
     def watch_value(self, time: float) -> None:
         evt = self.value
         if evt is None:
             s = ''
@@ -1009,44 +1073,64 @@
 
     def compose(self):
         yield Button(
             f"{self.idx:02d}", 
             id=mode_id(self.idx),
             classes="cmode"
             )
-        # yield Select(
-        #     [(s,i+1) for i,s in enumerate(gm_names)], 
-        #     id=inst_id(self.idx),
-        #     classes="cinst"
-        #     )
         yield Button(
             f"--- \n-----\n-----", 
             id=inst_id(self.idx),
             classes="cinst"
             )
         yield Button(
             f"MUTE", 
             id=mute_id(self.idx),
             classes="cmute"
             )
         
+    def on_mount(self) -> None:
+        lines = [
+            "cycle channel mode:",
+            f"-->{self.idx:02d}   input from MIDI channel {self.idx}"
+        ]
+        if self.idx > 0: lines.append(
+            f"{self.idx-1:02d}->{self.idx:02d}  follow channel {self.idx-1}")
+        lines.append(
+            f"{self.idx:02d}      notochord plays autonomously"
+        )
+        self.query_one("#"+mode_id(self.idx)).tooltip = '\n'.join(lines)
+        self.query_one("#"+inst_id(self.idx)).tooltip = "open instrument picker"
+        self.query_one("#"+mute_id(self.idx)).tooltip = f"mute channel {self.idx}"
+        
 class NotoPresets(Static):
+    n_presets = 10
     def compose(self):
-        for i in range(10):
+        for i in range(NotoPresets.n_presets):
             yield Button('---', id=preset_id(i))
 
+    def on_mount(self) -> None:
+        for i in range(NotoPresets.n_presets):
+            self.query_one("#"+preset_id(i)).tooltip = f"load preset {i}"
+
 class NotoControl(Static):
     def compose(self):
         # yield NotoToggle()
         # yield Checkbox("Mute", id="mute")
         yield Button("Mute", id="mute", variant="error")
         yield Button("Sustain", id="sustain", variant="primary")
         yield Button("Query", id="query")
         yield Button("Reset", id="reset", variant='warning')
 
+    def on_mount(self) -> None:
+        self.query_one("#mute").tooltip = "master mute notochord"
+        self.query_one("#sustain").tooltip = "master sustain -- prevent any NoteOffs from notochord"
+        self.query_one("#query").tooltip = "manually query a new event"
+        self.query_one("#reset").tooltip = "reset notochord"
+
 class NotoTUI(TUI):
     CSS_PATH = 'homunculus.css'
 
     BINDINGS = [
         ("m", "mute", "Mute Notochord"),
         ("s", "sustain", "Sustain"),
         ("q", "query", "Re-query Notochord"),
@@ -1059,14 +1143,17 @@
         yield NotoLog(id='note')
         yield NotoPrediction(id='prediction')
         yield Mixer()
         yield NotoPresets()
         yield NotoControl()
         yield Footer()
 
+    def on_mount(self) -> None:
+        self.query_one(NotoPrediction).tooltip = "displays the next predicted event"
+
     def set_preset(self, idx, name):
         node = self.query_one('#'+preset_id(idx))
         node.label = name
 
     def set_channel(self, chan, cfg):
         # print(f'set_channel {cfg}')
         inst_node = self.query_one('#'+inst_id(chan))
```

### Comparing `notochord-0.5.0/src/notochord/app/improviser-txala.py` & `notochord-0.5.1/src/notochord/app/improviser-txala.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.0/src/notochord/app/improviser.py` & `notochord-0.5.1/src/notochord/app/improviser.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.0/src/notochord/app/preset.json` & `notochord-0.5.1/src/notochord/app/preset.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9925223214285713%*

 * *Differences: {"'ens1'": "{'1': {'mode': 'auto'}, '3': {'source': 2}, '4': {'source': 3}, '5': {'source': 4}, "*

 * *           "'6': {'source': 5}, '7': {'source': 6}, '11': {'source': 10}, '12': {'source': 11}, "*

 * *           "'13': {'source': 12}, '14': {'source': 13}, '15': {'source': 14}, '16': {'source': "*

 * *           "15}, '10': OrderedDict([('mode', 'follow'), ('inst', 129), ('source', 9), ('mute', "*

 * *           'True)])}'}*

```diff
@@ -36,75 +36,81 @@
                 77
             ]
         }
     },
     "ens1": {
         "1": {
             "inst": 29,
-            "mode": "input"
+            "mode": "auto"
+        },
+        "10": {
+            "inst": 129,
+            "mode": "follow",
+            "mute": true,
+            "source": 9
         },
         "11": {
             "inst": 122,
             "mode": "follow",
             "mute": true,
             "range": [
                 60,
                 72
             ],
-            "source": 1
+            "source": 10
         },
         "12": {
             "inst": 48,
             "mode": "follow",
             "mute": true,
             "range": [
                 0,
                 81
             ],
-            "source": 1
+            "source": 11
         },
         "13": {
             "inst": 78,
             "mode": "follow",
             "mute": true,
-            "source": 8,
+            "source": 12,
             "transpose": [
                 7,
                 12
             ]
         },
         "14": {
             "inst": 93,
             "mode": "follow",
             "mute": true,
-            "source": 7,
+            "source": 13,
             "transpose": [
                 12,
                 24
             ]
         },
         "15": {
             "inst": 21,
             "mode": "follow",
             "mute": true,
-            "source": 7,
+            "source": 14,
             "transpose": [
                 0,
                 4
             ]
         },
         "16": {
             "inst": 16,
             "mode": "follow",
             "mute": true,
             "range": [
                 84,
                 108
             ],
-            "source": 1
+            "source": 15
         },
         "2": {
             "inst": 7,
             "mode": "follow",
             "mute": true,
             "source": 1,
             "transpose": [
@@ -112,59 +118,59 @@
                 15
             ]
         },
         "3": {
             "inst": 12,
             "mode": "follow",
             "mute": true,
-            "source": 1,
+            "source": 2,
             "transpose": [
                 12,
                 24
             ]
         },
         "4": {
             "inst": 13,
             "mode": "follow",
             "mute": true,
-            "source": 1,
+            "source": 3,
             "transpose": [
                 -15,
                 -3
             ]
         },
         "5": {
             "inst": 33,
             "mode": "follow",
             "mute": true,
-            "source": 1,
+            "source": 4,
             "transpose": [
                 -36,
                 -12
             ]
         },
         "6": {
             "inst": 10,
             "mode": "follow",
             "mute": true,
             "range": [
                 72,
                 96
             ],
-            "source": 1
+            "source": 5
         },
         "7": {
             "inst": 60,
             "mode": "follow",
             "mute": true,
             "range": [
                 12,
                 36
             ],
-            "source": 1
+            "source": 6
         },
         "8": {
             "inst": 74,
             "mode": "follow",
             "mute": true,
             "source": 7,
             "transpose": [
```

### Comparing `notochord-0.5.0/src/notochord/app/simple_harmonizer.py` & `notochord-0.5.1/src/notochord/app/simple_harmonizer.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.0/src/notochord/data.py` & `notochord-0.5.1/src/notochord/data.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.0/src/notochord/distributions.py` & `notochord-0.5.1/src/notochord/distributions.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.0/src/notochord/model.py` & `notochord-0.5.1/src/notochord/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1125,63 +1125,73 @@
                     'pitch_params': params[iperm[1]],
                     'time_params': params[iperm[2]],
                     'vel_params': params[iperm[3]]
                 }
 
             return r
 
-
     def predict(self, inst, pitch, time, vel, **kw):
         """
         DEPRECATED: alias for feed_query
         """
         self.feed(inst, pitch, time, vel)
         return self.query(**kw)
 
     def feed_query(self, inst, pitch, time, vel, **kw):
         """
-        call self.feed with *args, then self.query with **kwargs.
+        feed an event to the model, 
+        then query for the next predicted event and return it.
         """
         self.feed(inst, pitch, time, vel)
         return self.query(**kw)
 
     def query_feed(self, *a, **kw):
         """
-        call self.query with *args **kwargs, then self.feed with result,
-            and return result
+        query for the next predicted event and immediately feed it to the model,
+        also returning the predicted event.
         """
         r = self.query(*a, **kw)
         self.feed(r['inst'], r['pitch'], r['time'], r['vel'])
         return r
 
     def feed_query_feed(self, inst, pitch, time, vel, **kw):
         """
-        call self.feed with *args, then self.query with **kwargs.
+        given an event, return the next predicted event, 
+        feeding both to the model.
         """
         self.feed(inst, pitch, time, vel)
         return self.query_feed(**kw)
     
     def reset(self, start=True):
         """
         resets internal model state.
         Args:
             start: if True, send start tokens through the model
         """
         self.step = 0
-        for n,t in zip(self.cell_state_names(), self.initial_state):
-            getattr(self, n)[:] = t.detach()
-        if start:
-            self.feed(
-                self.instrument_start_token, self.pitch_start_token, 0., 0.)
+        with torch.inference_mode():
+            for n,t in zip(self.cell_state_names(), self.initial_state):
+                getattr(self, n)[:] = t
+            if start:
+                self.feed(
+                    self.instrument_start_token, self.pitch_start_token, 0., 0.)
+        # for n,t in zip(self.cell_state_names(), self.initial_state):
+        #     getattr(self, n)[:] = t.detach()
+        # if start:
+        #     self.feed(
+        #         self.instrument_start_token, self.pitch_start_token, 0., 0.)
 
     @classmethod
     def from_checkpoint(cls, path):
         """
         create a Notochord from a checkpoint file containing 
         hyperparameters and model weights.
+
+        Args:
+            path: file path to Notochord model
         """
         if path=="notochord-latest.ckpt":
             import appdirs
             d = Path(appdirs.user_data_dir('Notochord', 'IIL'))
             d.mkdir(exist_ok=True)
             path = d / path
             # maybe download
```

### Comparing `notochord-0.5.0/src/notochord/perform.py` & `notochord-0.5.1/src/notochord/perform.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.0/src/notochord/rnn.py` & `notochord-0.5.1/src/notochord/rnn.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.0/src/notochord/train.py` & `notochord-0.5.1/src/notochord/train.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.0/src/notochord/util.py` & `notochord-0.5.1/src/notochord/util.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.0/PKG-INFO` & `notochord-0.5.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,98 +1,96 @@
 Metadata-Version: 2.1
 Name: notochord
-Version: 0.5.0
-Summary:  Notochord is a real-time neural network model for MIDI performances. 
+Version: 0.5.1
+Summary: Notochord is a real-time neural network model for MIDI performances.
 License: MIT
 Author: Victor Shepardson
 Author-email: victor.shepardson@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
-Requires-Dist: iipyper (>=0.1.0,<0.2.0)
+Requires-Dist: iipyper (>=0.1.2,<0.2.0)
 Requires-Dist: numpy (>=1.23,<2.0)
-Requires-Dist: pandas (>=1.5,<2.0)
+Requires-Dist: pandas (>=2.0,<3.0)
 Requires-Dist: sf2utils (>=0.9,<0.10)
-Requires-Dist: torch (>=1.13,<3)
+Requires-Dist: torch (>=1.13,<2.3)
 Requires-Dist: tqdm (>=4.64,<5.0)
 Description-Content-Type: text/markdown
 
 # Notochord ([Paper](https://zenodo.org/record/7088404 "Notochord AIMC 2022 paper") | [Video](https://www.youtube.com/watch?v=mkBKAyudL0A "Notochord AIMC 2022 video"))
  
 <div align="middle">
 <img alt="Max Ernst, Stratified Rocks, Nature's Gift of Gneiss Lava Iceland Moss 2 kinds of lungwort 2 kinds of ruptures of the perinaeum growths of the heart b) the same thing in a well-polished little box somewhat more expensive, 1920" src="https://user-images.githubusercontent.com/4522484/223191876-251d461a-5bfc-439a-8df0-3841e7c76c4a.jpeg" width="60%" />
 </div>
 
 Notochord is a neural network model for MIDI performances. This package contains the training and inference model implemented in pytorch, as well as interactive MIDI processing apps using iipyper. 
 <!-- Some further examples involving SuperCollider and TidalCycles can be found in the parent repo under `examples`. -->
 
 ## Getting Started
 
-Using your python environment manager of choice (i.e. virtualenv, [conda](https://github.com/conda-forge/miniforge)), make a new environment with a Python version at least 3.10. Then `pip install notochord`.
+Using your python environment manager of choice (e.g. virtualenv, [conda](https://github.com/conda-forge/miniforge)), make a new environment with a Python version at least 3.10. Then `pip install notochord`.
 
 For developing `notochord`, see our [dev repo](https://github.com/Intelligent-Instruments-Lab/iil-dev.git)
 
-<!-- Follow the instructions in the root repo to set up an `iil-python-tools` environment. Then download a model checkpoint (e.g. `notochord_lakh_50G_deep.pt`) from the releases page: https://github.com/Intelligent-Instruments-Lab/iil-python-tools/releases . From here, I'll assume the model file is saved at `~/Downloads/notochord_lakh_50G_deep.pt`. -->
-
 ### Install fluidsynth (optional)
 [fluidsynth](https://github.com/FluidSynth/fluidsynth) is a General MIDI synthesizer which you can install from the package manager. On macOS:
 ```
 brew install fluidsynth
 ```
 fluidsynth needs a soundfont to run, like this one: https://drive.google.com/file/d/1-cwBWZIYYTxFwzcWFaoGA7Kjx5SEjVAa/view
 
 run fluidsynth in a terminal. For example, `fluidsynth -v -o midi.portname="fluidsynth" -o synth.midi-bank-select=mma ~/'Downloads/soundfonts/Timbres of Heaven (XGM) 4.00(G).sf2'`
 
 ## Notochord MIDI Apps
 
 Notochord includes several [iipyper](https://github.com/Intelligent-Instruments-Lab/iipyper.git) apps which can be run in a terminal. They have a clickable text-mode user interface and connect directly to MIDI ports, so you can wire them up to your controllers, DAW, etc.
 
-The Notochord harmonizer adds extra concurrent notes for each MIDI note you play in. In a terminal, make sure the `iil-python-tools` conda environment is active (`conda activate iil-python-tools`) and run:
+The Notochord harmonizer adds extra concurrent notes for each MIDI note you play in. In a terminal, make sure your notochord Python environment is active and run:
 ```
-python -m notochord harmonizer
+notochord harmonizer
 ```
-try `python -m notochord harmonizer --help`
+try `notochord harmonizer --help`
 to see more options.
 
-the ``homunculus'' gives you a UI to manage multiple input, harmonizing or autonomous notochord channels:
+the "homunculus" gives you a UI to manage multiple input, harmonizing or autonomous notochord channels:
 ```
-python -m notochord homunculus
+notochord homunculus
 ```
 You can set the MIDI in and out ports with `--midi-in` and `--midi-out`. If you use a General MIDI synthesizer like fluidsynth, you can add `--send-pc` to also send program change messages.
 
 If you are using fluidsynth, try:
 ```
-python -m notochord homunculus --send-pc --midi-out fluidsynth --thru
+notochord homunculus --send-pc --midi-out fluidsynth --thru
 ```
 
 ## Python API
 
-See the docstrings for `Notochord.feed` and `Notochord.query` in `notochord/model.py` for the low-level Notochord inference API which can be used from Python code. `notochord/app/simple_harmonizer.py` provides a minimal example of how to build an interactive app.
+See the docs for `Notochord.feed` and `Notochord.query` for the low-level Notochord inference API which can be used from Python code. `notochord/app/simple_harmonizer.py` provides a minimal example of how to build an interactive app.
 
 ## OSC server
 
 You can also expose the inference API over Open Sound Control:
 ```
-python -m notochord server
+notochord server
 ```
 this will run notochord and listen continously for OSC messages.
 
 <!-- `examples/notochord/generate-demo.scd` and `examples/notochord/harmonize-demo.scd` are example scripts for interacting with the notochord server from SuperCollider. -->
 
 ## Tidal interface
 
-see `examples/notochord/tidalcycles` in the archived [iil-python-tools](https://github.com/Intelligent-Instruments-Lab/iil-python-tools/tree/master/examples) repo (updated examples coming soon):
+see `notochord/tidalcycles` in [iil-examples](https://github.com/Intelligent-Instruments-Lab/iil-examples.git) repo (updated examples coming soon):
 
 add `Notochord.hs` to your tidal boot file. Probably replace the `tidal <- startTidal` line with something like:
 ```haskell
-:script ~/iil-python-tools/examples/notochord/tidalcycles/Notochord.hs
+:script ~/iil-examples/notochord/tidalcycles/Notochord.hs
 
 let sdOscMap = (superdirtTarget, [superdirtShape])
 let oscMap = [sdOscMap,ncOscMap]
 
 tidal <- startStream defaultConfig {cFrameTimespan = 1/240} oscMap
 ```
```

