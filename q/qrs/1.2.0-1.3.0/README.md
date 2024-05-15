# Comparing `tmp/qrs-1.2.0.tar.gz` & `tmp/qrs-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qrs-1.2.0.tar", last modified: Thu Jan 25 00:11:24 2024, max compression
+gzip compressed data, was "qrs-1.3.0.tar", last modified: Wed May 15 00:04:03 2024, max compression
```

## Comparing `qrs-1.2.0.tar` & `qrs-1.3.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 00:11:24.619618 qrs-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-01-25 00:11:15.000000 qrs-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-01-25 00:11:24.619618 qrs-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-01-25 00:11:15.000000 qrs-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 00:11:24.611618 qrs-1.2.0/qrs/
--rw-r--r--   0 runner    (1001) docker     (127)    13181 2024-01-25 00:11:15.000000 qrs-1.2.0/qrs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  2905592 2024-01-25 00:11:15.000000 qrs-1.2.0/qrs/wordlist.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 00:11:24.619618 qrs-1.2.0/qrs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-01-25 00:11:24.000000 qrs-1.2.0/qrs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-01-25 00:11:24.000000 qrs-1.2.0/qrs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 00:11:24.000000 qrs-1.2.0/qrs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-25 00:11:24.000000 qrs-1.2.0/qrs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-25 00:11:24.000000 qrs-1.2.0/qrs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-01-25 00:11:24.000000 qrs-1.2.0/qrs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 00:11:24.000000 qrs-1.2.0/qrs.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-25 00:11:24.619618 qrs-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-01-25 00:11:15.000000 qrs-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:04:03.216973 qrs-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-15 00:03:57.000000 qrs-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7245 2024-05-15 00:04:03.216973 qrs-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-05-15 00:03:57.000000 qrs-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:04:03.208973 qrs-1.3.0/qrs/
+-rw-r--r--   0 runner    (1001) docker     (127)    15389 2024-05-15 00:03:57.000000 qrs-1.3.0/qrs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-15 00:03:57.000000 qrs-1.3.0/qrs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2905592 2024-05-15 00:03:57.000000 qrs-1.3.0/qrs/wordlist.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:04:03.216973 qrs-1.3.0/qrs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7245 2024-05-15 00:04:03.000000 qrs-1.3.0/qrs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-15 00:04:03.000000 qrs-1.3.0/qrs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 00:04:03.000000 qrs-1.3.0/qrs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-15 00:04:03.000000 qrs-1.3.0/qrs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 00:04:03.000000 qrs-1.3.0/qrs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 00:04:03.000000 qrs-1.3.0/qrs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 00:04:03.000000 qrs-1.3.0/qrs.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 00:04:03.216973 qrs-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-15 00:03:57.000000 qrs-1.3.0/setup.py
```

### Comparing `qrs-1.2.0/LICENSE` & `qrs-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qrs-1.2.0/PKG-INFO` & `qrs-1.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 Metadata-Version: 2.1
 Name: qrs
-Version: 1.2.0
-Summary: Provides word game-related tools that can be configured with custom settings, letter scores, and wordlists.
+Version: 1.3.0
+Summary: Provides word game-related tools that can be configured with custom settings,
 Home-page: https://github.com/silvncr/qrs
 Author: silvncr
 License: MIT
-Classifier: Programming Language :: Python
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python
 Classifier: Topic :: Games/Entertainment :: Board Games
 Classifier: Topic :: Games/Entertainment :: Puzzle Games
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Classifier: Typing :: Typed
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: jarguments==0.0.1
+Requires-Dist: jarguments==0.1.0
 
 <!-- omit from toc -->
 # qrs
 
 tool for *Quarrel* (and other word games)
 
-![[publish status](https://github.com/silvncr/qrs/actions/workflows/python-publish.yml)](https://img.shields.io/github/actions/workflow/status/silvncr/qrs/python-publish.yml)
-![[latest release](https://github.com/silvncr/qrs/releases/latest)](https://img.shields.io/github/v/release/silvncr/qrs)
+![downloads](https://img.shields.io/pypi/dm/qrs)
+![status](https://img.shields.io/github/actions/workflow/status/silvncr/qrs/python-publish.yml)
+![version](https://img.shields.io/pypi/v/qrs)
 
 ## Summary
 
 Provides word game-related tools that can be configured with custom settings, letter scores, and wordlists.
 
-> Works on Python 3.6 and above. Tested on Windows 10.
+> Supports Python 3.8 and above. Tested on Windows 10.
 
 ## Contents
 
 - [Summary](#summary)
 - [Contents](#contents)
 - [The qrs library](#the-qrs-library)
 - [Direct execution](#direct-execution)
@@ -44,23 +52,17 @@
 Install the qrs library to use its functionality in your projects.
 
 ```sh
 python -m pip install --upgrade qrs
 ```
 
 ```py
->>> from qrs import build_settings, Ruleset
->>> q = Ruleset(
-...     build_settings(
-...         {'max': 8}
-...     )
-... )
->>> print(
-...     q.solve_str('wetodlnm')
-... )
+>>> from qrs import Ruleset
+>>> q = Ruleset({'max': 8})
+>>> print(q.solve_str('wetodlnm'))
 
         --- query: delmnotw (8 letters) ---
 
         8 letters - 18 points
          MELTDOWN
 
         5 letters - 14 points
@@ -84,27 +86,27 @@
 $ qrs
 
 qrs: _
 ```
 
 Upon being called from the command line, it will display an input screen.
 
-Type your letters into the field, press Enter, and wait for the program to calculate the best words. Once done, choose one from the list that corresponds with the number of letters you have available or the next lowest. See the example below to find out why you might not need to use all of your spaces.
+Enter your letters and wait for the program to calculate the best words. Choose one from the list that corresponds with the number of letters you have available, or the next longest. See the example below to find out why you might not need to use all of your spaces.
 
 ## Example case
 
 Here's an example using the default program settings. Our situation is the following:
 
 - We're playing *Quarrel*, and thus, we get eight letters.
 - Our letters are `wetodlnm`.
 - We have seven spaces to use.
 
 After installing the library, we'll open a command line and run the program.
 
-Since we know we don't need words longer than eight letters, we can minimise loading time by configuring the program to only calculate for words of that length. We can do this by passing our desired settings as command arguments:
+The program will have to load a wordlist, which takes longer as the range of word lengths increases. Since we know we don't need words longer than eight letters, we can minimise loading time by configuring the program to only calculate for words of that length. We can do this by passing our desired settings as command arguments:
 
 ```sh
 $ qrs --max 8
 
 qrs: _
 ```
 
@@ -116,15 +118,15 @@
 > ```
 >
 > ```sh
 > ## from folder with qrs.json
 > $ qrs
 > ```
 
-The program will have to load a wordlist whichever way it is run. Once it finishes loading, we can input our letters and press Enter.
+Once it finishes loading, we can enter our letters.
 
 ```py
 qrs: wetodlnm
 
         --- query: delmnotw (8 letters) ---
 
         8 letters - 18 points
@@ -133,45 +135,48 @@
         5 letters - 14 points
          MOWED
 
         4 letters - 12 points
          MEWL
 
         3 letters - 10 points
-         MEW, MOW
+         MEW, MOW, WEM
 
         2 letters - 6 points
-         OW, WE, WO
+         EW, OW, WE, WO
 
 qrs: _
 ```
 
 This output tells us that the anagram is `MELTDOWN`, but we can't make that word because we can only use seven letters. In this case, our best word is `MOWED` (14 points). Based on this output, we also know that our opponent cannot score higher than us without all eight spaces.
 
 > Note: a word like `LETDOWN` scores the same number of points as `MOWED`, but isn't recognised as a "best word" in this case. This is because when words are tied for points, the program will choose the word/s with the fewest letters.
 >
 > The fewer letters your word has, the faster you can write it into your game. This is especially important in *Quarrel*, as the tiebreaker for equal points is input speed.
+>
+> You can choose to display longer, tied words by enabling the `--doubles` setting.
 
 ## Settings
 
 Upon being run from the command line, the program will automatically generate (or look for) a `qrs.json` file in the directory from which the command is run. This file contains the program's settings, which can be changed to suit your needs.
 
-When using qrs as a library, you should pass a `dict` with any of the following keys into `build_settings` to generate a full settings object, then pass the output to a `Ruleset` to create a new instance. Here are all the currently supported settings:
+When using qrs as a library, pass a `dict` with any of the following keys to a `Ruleset` to create a new instance. Here are all the currently supported settings:
 
 | Setting | Default | Description |
-|:-:|:-:|:--|
-| `debug` | `false` | Shows the program's inner workings whilst calculating. Note that this may negatively affect performance on certain devices or IDEs. |
-| `exclude` | `[]` | List of words that the program will never output. |
-| `game` | `"quarrel"` | Determines the letter scoring system used for calculating points. The value here is passed into `build_letter_scores()`, and defaults back if invalid. |
-| `include` | `[]` | List of additional words for the wordlist. |
-| `lower` | `false`| Displays output in lowercase letters. The default setting displays capital letters to mimic the style of word games like *Scrabble* and *Quarrel*, however some people may find lowercase output more readable. |
-| `max` | longest length in wordlist | Determines the maximum word length the program will calculate for. |
-| `min` | `2` | Determines the minimum word length the program will calculate for. |
-| `noscores` | `false` | Determines whether point values for words are considered, in which case only the highest-scoring words are displayed. If you don't care about scoring, turn this on to see all words. |
-| `repeats` | `false` | Determines whether letters can be used more than once. Change this according to your word game's rules; for example, *Scrabble* tiles can only be used once in a single word, whereas *New York Times*'s *Spelling Bee* allows the reuse of letters. |
+| :-: | :-: | :-- |
+| `debug` 🐛 | `false` | Prints the program's inner workings whilst calculating. Note that many consecutive print statements may negatively affect performance on certain devices or IDEs. |
+| `doubles` 🔀 | `false` | Shows longer words that tie for score (like the `MOWED` / `LETDOWN` example above). |
+| `exclude` ⛔ | `[]` | List of words that the program will never output. |
+| `game` 🎮 | `"quarrel"` | Determines the letter scoring system used for calculating points. The value here is passed into `build_letter_scores()`, and defaults back if invalid. |
+| `include` ✔️ | `[]` | List of additional words for the wordlist. |
+| `lower` 💻 | `false` | Displays output in lowercase letters. The default setting displays capital letters to mimic the style of word games like *Scrabble* and *Quarrel*, however some people may find lowercase output more readable. |
+| `max` 🔼 | longest length in wordlist | Determines the maximum word length the program will calculate for. |
+| `min` 🔽 | `2` | Determines the minimum word length the program will calculate for. |
+| `noscores` 💯 | `false` | Determines whether point values for words are considered, in which case only the highest-scoring words are displayed. If you don't care about scoring, turn this on to see all words. |
+| `repeats` 🔁 | `false` | Determines whether letters can be used more than once. Change this according to your word game's rules; for example, *Scrabble* tiles can only be used once in a word, whereas *New York Times*'s *Spelling Bee* allows the reuse of letters. |
 
 When running directly:
 
 - To change your settings, do one of the following:
   - Open `qrs.json` in a text editor and change any values. Make sure to save the file once you're done.
   - Pass the setting as a command argument like this: `--setting value`
     - If applicable, this will automatically update the settings file.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `qrs-1.2.0/README.md` & `qrs-1.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 <!-- omit from toc -->
 # qrs
 
 tool for *Quarrel* (and other word games)
 
-![[publish status](https://github.com/silvncr/qrs/actions/workflows/python-publish.yml)](https://img.shields.io/github/actions/workflow/status/silvncr/qrs/python-publish.yml)
-![[latest release](https://github.com/silvncr/qrs/releases/latest)](https://img.shields.io/github/v/release/silvncr/qrs)
+![downloads](https://img.shields.io/pypi/dm/qrs)
+![status](https://img.shields.io/github/actions/workflow/status/silvncr/qrs/python-publish.yml)
+![version](https://img.shields.io/pypi/v/qrs)
 
 ## Summary
 
 Provides word game-related tools that can be configured with custom settings, letter scores, and wordlists.
 
-> Works on Python 3.6 and above. Tested on Windows 10.
+> Supports Python 3.8 and above. Tested on Windows 10.
 
 ## Contents
 
 - [Summary](#summary)
 - [Contents](#contents)
 - [The qrs library](#the-qrs-library)
 - [Direct execution](#direct-execution)
@@ -26,23 +27,17 @@
 Install the qrs library to use its functionality in your projects.
 
 ```sh
 python -m pip install --upgrade qrs
 ```
 
 ```py
->>> from qrs import build_settings, Ruleset
->>> q = Ruleset(
-...     build_settings(
-...         {'max': 8}
-...     )
-... )
->>> print(
-...     q.solve_str('wetodlnm')
-... )
+>>> from qrs import Ruleset
+>>> q = Ruleset({'max': 8})
+>>> print(q.solve_str('wetodlnm'))
 
         --- query: delmnotw (8 letters) ---
 
         8 letters - 18 points
          MELTDOWN
 
         5 letters - 14 points
@@ -66,27 +61,27 @@
 $ qrs
 
 qrs: _
 ```
 
 Upon being called from the command line, it will display an input screen.
 
-Type your letters into the field, press Enter, and wait for the program to calculate the best words. Once done, choose one from the list that corresponds with the number of letters you have available or the next lowest. See the example below to find out why you might not need to use all of your spaces.
+Enter your letters and wait for the program to calculate the best words. Choose one from the list that corresponds with the number of letters you have available, or the next longest. See the example below to find out why you might not need to use all of your spaces.
 
 ## Example case
 
 Here's an example using the default program settings. Our situation is the following:
 
 - We're playing *Quarrel*, and thus, we get eight letters.
 - Our letters are `wetodlnm`.
 - We have seven spaces to use.
 
 After installing the library, we'll open a command line and run the program.
 
-Since we know we don't need words longer than eight letters, we can minimise loading time by configuring the program to only calculate for words of that length. We can do this by passing our desired settings as command arguments:
+The program will have to load a wordlist, which takes longer as the range of word lengths increases. Since we know we don't need words longer than eight letters, we can minimise loading time by configuring the program to only calculate for words of that length. We can do this by passing our desired settings as command arguments:
 
 ```sh
 $ qrs --max 8
 
 qrs: _
 ```
 
@@ -98,15 +93,15 @@
 > ```
 >
 > ```sh
 > ## from folder with qrs.json
 > $ qrs
 > ```
 
-The program will have to load a wordlist whichever way it is run. Once it finishes loading, we can input our letters and press Enter.
+Once it finishes loading, we can enter our letters.
 
 ```py
 qrs: wetodlnm
 
         --- query: delmnotw (8 letters) ---
 
         8 letters - 18 points
@@ -115,45 +110,48 @@
         5 letters - 14 points
          MOWED
 
         4 letters - 12 points
          MEWL
 
         3 letters - 10 points
-         MEW, MOW
+         MEW, MOW, WEM
 
         2 letters - 6 points
-         OW, WE, WO
+         EW, OW, WE, WO
 
 qrs: _
 ```
 
 This output tells us that the anagram is `MELTDOWN`, but we can't make that word because we can only use seven letters. In this case, our best word is `MOWED` (14 points). Based on this output, we also know that our opponent cannot score higher than us without all eight spaces.
 
 > Note: a word like `LETDOWN` scores the same number of points as `MOWED`, but isn't recognised as a "best word" in this case. This is because when words are tied for points, the program will choose the word/s with the fewest letters.
 >
 > The fewer letters your word has, the faster you can write it into your game. This is especially important in *Quarrel*, as the tiebreaker for equal points is input speed.
+>
+> You can choose to display longer, tied words by enabling the `--doubles` setting.
 
 ## Settings
 
 Upon being run from the command line, the program will automatically generate (or look for) a `qrs.json` file in the directory from which the command is run. This file contains the program's settings, which can be changed to suit your needs.
 
-When using qrs as a library, you should pass a `dict` with any of the following keys into `build_settings` to generate a full settings object, then pass the output to a `Ruleset` to create a new instance. Here are all the currently supported settings:
+When using qrs as a library, pass a `dict` with any of the following keys to a `Ruleset` to create a new instance. Here are all the currently supported settings:
 
 | Setting | Default | Description |
-|:-:|:-:|:--|
-| `debug` | `false` | Shows the program's inner workings whilst calculating. Note that this may negatively affect performance on certain devices or IDEs. |
-| `exclude` | `[]` | List of words that the program will never output. |
-| `game` | `"quarrel"` | Determines the letter scoring system used for calculating points. The value here is passed into `build_letter_scores()`, and defaults back if invalid. |
-| `include` | `[]` | List of additional words for the wordlist. |
-| `lower` | `false`| Displays output in lowercase letters. The default setting displays capital letters to mimic the style of word games like *Scrabble* and *Quarrel*, however some people may find lowercase output more readable. |
-| `max` | longest length in wordlist | Determines the maximum word length the program will calculate for. |
-| `min` | `2` | Determines the minimum word length the program will calculate for. |
-| `noscores` | `false` | Determines whether point values for words are considered, in which case only the highest-scoring words are displayed. If you don't care about scoring, turn this on to see all words. |
-| `repeats` | `false` | Determines whether letters can be used more than once. Change this according to your word game's rules; for example, *Scrabble* tiles can only be used once in a single word, whereas *New York Times*'s *Spelling Bee* allows the reuse of letters. |
+| :-: | :-: | :-- |
+| `debug` 🐛 | `false` | Prints the program's inner workings whilst calculating. Note that many consecutive print statements may negatively affect performance on certain devices or IDEs. |
+| `doubles` 🔀 | `false` | Shows longer words that tie for score (like the `MOWED` / `LETDOWN` example above). |
+| `exclude` ⛔ | `[]` | List of words that the program will never output. |
+| `game` 🎮 | `"quarrel"` | Determines the letter scoring system used for calculating points. The value here is passed into `build_letter_scores()`, and defaults back if invalid. |
+| `include` ✔️ | `[]` | List of additional words for the wordlist. |
+| `lower` 💻 | `false` | Displays output in lowercase letters. The default setting displays capital letters to mimic the style of word games like *Scrabble* and *Quarrel*, however some people may find lowercase output more readable. |
+| `max` 🔼 | longest length in wordlist | Determines the maximum word length the program will calculate for. |
+| `min` 🔽 | `2` | Determines the minimum word length the program will calculate for. |
+| `noscores` 💯 | `false` | Determines whether point values for words are considered, in which case only the highest-scoring words are displayed. If you don't care about scoring, turn this on to see all words. |
+| `repeats` 🔁 | `false` | Determines whether letters can be used more than once. Change this according to your word game's rules; for example, *Scrabble* tiles can only be used once in a word, whereas *New York Times*'s *Spelling Bee* allows the reuse of letters. |
 
 When running directly:
 
 - To change your settings, do one of the following:
   - Open `qrs.json` in a text editor and change any values. Make sure to save the file once you're done.
   - Pass the setting as a command argument like this: `--setting value`
     - If applicable, this will automatically update the settings file.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `qrs-1.2.0/qrs/__init__.py` & `qrs-1.3.0/qrs/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,523 +1,684 @@
 '''
-Provides word game-related tools that can be configured with custom settings, letter scores, and wordlists.
+Provides word game-related tools that can be configured with custom settings,
+letter scores, and wordlists.
 '''
 
-# imports
+from __future__ import annotations
+
 from contextlib import suppress
 from copy import deepcopy
 from json import decoder, dumps, load
-from os import path
+from os import path as os_path
 from string import ascii_lowercase
-from sys import path as syspath
-from typing import Any, Dict, List, Optional, Tuple, Union
+from sys import path as sys_path
+from typing import Any, Self
 
 # metadata
 __author__ = 'silvncr'
 __license__ = 'MIT'
 __module_name__ = 'qrs'
-__python_version__ = '3.6'
-__version__ = '1.2.0'
+__python_version__ = '3.8'
+__version__ = '1.3.0'
 
 
 # get full wordlist from file
-wordlist_full = sorted(
-	open(
-		path.join(
-			path.dirname(__file__), 'wordlist.txt'
-		)
-	).read().strip().split('\n')
-)
+with open(
+	os_path.join(
+		os_path.dirname(__file__),
+		'wordlist.txt',
+	),
+) as f:
+	wordlist_full = sorted(
+		f.read().splitlines(),
+	)
+max_length_full = max(len(word) for word in wordlist_full)
 
-# command-line arguments; formatted as (arg, sarg, type, default, multiple, help)
-kwargs = [
+
+# command line arguments; (arg, sarg, type, default, multiple, help)
+qrs_kwargs = [
 	('debug', 'd', bool, False, ..., 'Whether to display debug information'),
-	('exclude', 'e', str, [], True, 'Words to exclude'),
+	('doubles', 'b', bool, False, ..., 'Whether to show longer, tied words'),
+	('exclude', 'e', str, [], True, 'List of words to exclude'),
 	('game', 'g', str, 'quarrel', None, 'Scoring system to use'),
-	('include', 'i', str, [], True, 'Words to include'),
+	('include', 'i', str, [], True, 'List of words to include'),
 	('lower', 'l', bool, False, ..., 'Whether output should be lowercase'),
-	('max', 'm', int, max(len(word) for word in wordlist_full), None, 'Maximum length of words'),
+	('max', 'm', int, max_length_full, None, 'Maximum length of words'),
 	('min', 'n', int, 2, None, 'Minimum length of words'),
 	('noscores', 's', bool, False, ..., 'Whether to ignore scores'),
-	('repeats', 'r', bool, False, ..., 'Whether letters are allowed to repeat'),
+	('repeats', 'r', bool, False, ..., 'Whether letters can repeat'),
 ]
 
+
 # get letter scores for name
 def build_letter_scores(
-	name: Optional[str] = None,
-) -> Dict[str, int]:
+	name: str | None = None,
+	/,
+) -> dict[str, int]:
 	'''
-	Returns the letter scores for the given name. To be passed into the `Ruleset` class.
+	Returns the letter scores for the given name. To be passed into the
+	`Ruleset` class.
 
 	Args:
-		`name: str` (optional): The name of the letter scoring system. Defaults to *Quarrel*.
+	----
+		name: `str` (optional)
+			The name of the letter scoring system.
+			Defaults to *Quarrel*.
 
 	Returns:
-		`dict[str, int]`: A dictionary of letter scores, with letters as keys and scores as values, or an empty dictionary if `name` is invalid.
+	-------
+		`dict[str, int]`
+			A dictionary of letter scores, with letters as keys and scores
+			as values, or an empty dictionary if `name` is invalid.
 	'''
 
 	# name default
 	if not name:
 		name = 'quarrel'
 
 	# return letter scores
 	return next(
 		(
 			val for key, val in {
 				'quarrel': {
 					'a': 1, 'b': 5, 'c': 2, 'd': 3, 'e': 1, 'f': 5, 'g': 4,
 					'h': 4, 'i': 1, 'j': 15, 'k': 6, 'l': 2, 'm': 4, 'n': 1,
 					'o': 1, 'p': 3, 'q': 15, 'r': 2, 's': 1, 't': 1, 'u': 3,
-					'v': 6, 'w': 5, 'x': 10, 'y': 5, 'z': 12
+					'v': 6, 'w': 5, 'x': 10, 'y': 5, 'z': 12,
 				},
 				'scrabble': {
 					'a': 1, 'b': 3, 'c': 3, 'd': 2, 'e': 1, 'f': 4, 'g': 2,
 					'h': 4, 'i': 1, 'j': 8, 'k': 5, 'l': 1, 'm': 3, 'n': 1,
 					'o': 1, 'p': 3, 'q': 10, 'r': 1, 's': 1, 't': 1, 'u': 1,
-					'v': 4, 'w': 4, 'x': 8, 'y': 4, 'z': 10
+					'v': 4, 'w': 4, 'x': 8, 'y': 4, 'z': 10,
 				},
 			}.items() if name == key
-		), {}
+		), {},
 	)
 
+
 # get query string
 def build_query(
 	query: str,
+	/,
+	*,
 	repeat_letters: bool = True,
 ) -> str:
 	'''
 	Returns a sorted query string, with optional repeats.
 
 	Args:
-		`query: str`: Query string to sort.
-		`repeat_letters: bool` (optional): Whether to allow repeating letters in the query string. Usually the *opposite* of `Ruleset()['repeats']`. Defaults to True.
+	----
+		query: `str`
+			Query string to sort.
+		repeat_letters: `bool` (optional)
+			Whether to allow repeating letters in the query string.
+			Usually the *opposite* of `Ruleset()['repeats']`.
+			Defaults to True.
 
 	Returns:
+	-------
 		`str`: The inputted query string, but sorted.
 	'''
-
-	# return query string
 	return ''.join(
 		sorted(query)
 		if repeat_letters
-		else sorted(list(set(dict.fromkeys(query))))
+		else sorted(set(dict.fromkeys(query))),
 	).lower()
 
+
 # get settings object from settings
 def build_settings(
-	user_settings: 'Optional[dict[str, Any]]' = None,
-	wordlist: 'Optional[list[str]]' = None,
-) -> Dict[str, Any]:
+	user_settings: dict[str, Any] | None = None,
+	wordlist: list[str] | None = None,
+	/,
+) -> dict[str, Any]:
 	'''
-	Returns the settings for the given user settings. To be passsed into the `Ruleset` class.
+	Returns the settings for the given user settings.
 
 	Args:
-		`user_settings: dict[str, Any]` (optional): Custom settings to override the default settings. Defaults to an empty dictionary.
-		`wordlist: list[str]` (optional): Wordlist used to determine defaults for word-related settings.
+	----
+		user_settings: `dict[str, Any]` (optional)
+			Custom settings to override the default settings.
+			Defaults to an empty dictionary.
+		wordlist: `list[str]` (optional)
+			Wordlist used to determine defaults for word-related settings.
 
 	Returns:
+	-------
 		`dict[str, Any]`: A dictionary of settings.
 	'''
 
 	# user_settings default
 	if not user_settings:
 		user_settings = {}
 
 	# wordlist default
-	if not wordlist:
-		wordlist = wordlist_full
+	_wordlist = wordlist or wordlist_full
 
 	# remove excluded words
 	if 'exclude' in user_settings:
 		for word in user_settings['exclude']:
-			if (word) and (word in wordlist):
-				wordlist.remove(word)
+			if (word) and (word in _wordlist):
+				_wordlist.remove(word)
 
 	# add included words
 	if 'include' in user_settings:
 		for word in user_settings['include']:
-			if (word) and (word not in wordlist):
-				wordlist.append(word)
+			if (word) and (word not in _wordlist):
+				_wordlist.append(word)
 
-	# build defaults
+	# build defaults and determine min-max
 	settings = {
-		**{str(arg): default for arg, _, _, default, _, _ in kwargs},
+		**{
+			str(arg): default
+			for arg, _, _, default, _, _ in qrs_kwargs
+		},
 		**user_settings,
 		'min': max(user_settings['min'], 2) if 'min' in user_settings else 2,
-		'max': min(user_settings['max'], max(len(word) for word in wordlist))
-		if 'max' in user_settings
-		else max(len(word) for word in wordlist),
+		'max': min(user_settings['max'], max(len(word) for word in _wordlist))
+			if 'max' in user_settings
+			else max(len(word) for word in _wordlist),
 	}
 
-	# set min-max
+	# set game
 	return {
-		**settings, **{
-			'game': str(
-				settings['game']
-				if build_letter_scores(settings['game'])
-				else 'quarrel'
-			)
-		}
+		**settings,
+		'game': str(
+			settings['game']
+			if build_letter_scores(settings['game'])
+			else 'quarrel',
+		),
 	}
 
+
 # word game ruleset class
 class Ruleset:
+	'''Defines a word game ruleset with custom settings and wordlist.'''
+
 	def __init__(
-		self,
-		settings: 'Optional[dict[str, Any]]' = None,
-		wordlist: 'Optional[list[str]]' = None,
+		self: Ruleset,
+		/,
+		settings: dict[str, Any] | None = None,
+		wordlist: list[str] | None = None,
 	) -> None:
 		'''
 		Defines a word game ruleset with the given settings and wordlist.
 
 		Args:
-			`settings: dict[str, Any]` (optional): Custom settings to override the default settings. Should be an output from `build_settings()`. Defaults to an empty dictionary.
-			`wordlist: list[str]` (optional): A list of words to be used in the ruleset. Defaults to the full Scrabble wordlist.
+		----
+			settings: `dict[str, Any]` (optional)
+				Custom settings to override the default settings.
+			wordlist: `list[str]` (optional)
+				A list of words to be used in the ruleset.
+				Defaults to the *Collins Scrabble Dictionary (2019)*,
+				which is the only built-in wordlist.
 
 		Returns:
+		-------
 			A `Ruleset` with the specified settings and wordlist.
 		'''
 
 		# settings default
 		settings = settings or {}
 
 		# wordlist default
-		wordlist = wordlist or wordlist_full
+		_wordlist = wordlist or wordlist_full
 
 		# remove excluded words
 		if 'exclude' in settings:
 			for word in settings['exclude']:
-				if (word) and (word in wordlist):
-					wordlist.remove(word)
+				if (word) and (word in _wordlist):
+					_wordlist.remove(word)
 
 		# add included words
 		if 'include' in settings:
 			for word in settings['include']:
-				if (word) and (word not in wordlist):
-					wordlist.append(word)
+				if (word) and (word not in _wordlist):
+					_wordlist.append(word)
 
 		# get settings
-		settings = build_settings(settings, wordlist)
+		settings = build_settings(settings, _wordlist)
 
 		# adjust wordlist to settings
-		wordlist = [
-			word for word in wordlist
+		_wordlist = [
+			word for word in _wordlist
 			if settings['min'] <= len(word) <= settings['max']
 		]
 
 		# set attributes
 		self.settings = settings
 		self.scores = {
-			word: sum(build_letter_scores(self['game'])[char] for char in word)
+			word: sum(
+				build_letter_scores(self['game'])[char] for char in word
+			)
 			for word in sorted(
-				sorted(wordlist),
+				sorted(_wordlist),
 				key=lambda word: (
 					len(word), sum(
 						build_letter_scores(self['game'])[char]
 						for char in word
-					)
-				), reverse=True
+					),
+				), reverse=True,
 			)
 		}
-		self.wordlist = wordlist
+		self.wordlist = _wordlist
 
 	# getitem method
-	def __getitem__(self, key: str) -> Any:
+	def __getitem__(
+			self: Self,
+			key: str,
+			/,
+		) -> ...:
 		'''
-		Returns the value of the given setting, as defined in the ruleset's settings.
+		Returns the value of the given setting, as defined in the ruleset's
+		settings.
 
 		Args:
-			`key: str`: The setting to get the value of.
+		----
+			key: `str`
+				The setting to get the value of.
 
 		Returns:
-			`Any`: The value of the given setting.
+		-------
+			The value of the given setting.
 		'''
 
 		# return setting, or raise error
-		if key in self.settings.keys():
+		if key in self.settings:
 			return self.settings[key]
-		else:
-			raise KeyError(f'{key} not found in settings')
+		msg = f'{key} not found in settings'
+		raise KeyError(msg)
 
 	# get settings
 	def get_settings(
-		self,
-	) -> Dict[str, Any]:
-		'''
-		Returns the current settings.
-		'''
+		self: Self,
+		/,
+	) -> dict[str, Any]:
+		'Returns the current settings as a dictionary.'
 
 		# return settings object
 		return self.settings
 
 	# get settings as string
 	def get_settings_str(
-		self,
+		self: Self,
+		/,
 	) -> str:
-		'''
-		Returns the current settings as a JSON string, formatted with tabs.
-		'''
+		'Returns the current settings as a JSON string, formatted with tabs.'
 
 		# return settings string
-		return dumps(self.settings, indent=2, sort_keys=True).replace('  ', '\t')
+		return dumps(self.settings, indent=2, sort_keys=True) \
+			.replace('  ', '\t')
 
 	# solve function
 	def solve(
-		self,
+		self: Self,
 		query: str,
-	) -> Tuple[Dict[int, List[Union[List[str], str]]], bool]:
+		/,
+	) -> tuple[dict[int, list[str]], bool]:
 		'''
-		Finds all possible words that can be formed from the given query string using the set wordlist.
+		Finds all possible words that can be formed from the given query
+		string using the set wordlist.
 
 		Args:
-			`query: str`: A string representing the query to be solved.
+		----
+			query: `str`
+				A string representing the query to be solved.
 
 		Returns:
-			`tuple`: A tuple containing a dictionary of best words by length, and a boolean indicating whether an anagram was found.
+		-------
+			`tuple[dict, bool]`: A tuple containing a dictionary of best words
+			by length, and a boolean indicating whether an anagram was found.
 		'''
 
 		# build query
-		query = build_query(query, not self['repeats'])
+		query = build_query(query, repeat_letters=not self['repeats'])
 
 		# initialise output object
 		scores = {}
 
 		# prepare debug output
 		if self['debug']:
 			print('')
 
 		# iterate through possible word lengths
 		for len_iter in range(
-			2, (self['max'] if self['repeats'] else len(query)) + 1
+			max(2, min([2, self['min']])),
+			(self['max'] if self['repeats'] else len(query)) + 1,
 		)[::-1]:
 			scores = {
-				**scores, **{
-					len_iter: [[], 0]
-				}
+				**scores,
+				len_iter: [[], 0],
 			}
 
 			# iterate through wordlist
 			for word in self.scores:
 				query_iter, word_iter = deepcopy(query), deepcopy(word)
 				word_fits = False
 
-				# handle ignore_scores
+				# handle noscores
 				if (
-					len(word) == len_iter if self['noscores'] else len(word) <= len_iter
+					len(word) == len_iter
+					if self['noscores']
+					else len(word) <= len_iter
 				) and set(word) <= set(query):
-					if not self['noscores'] and self.scores[word] < scores[len_iter][1]:
+					if (
+						not self['noscores']
+						and self.scores[word] < scores[len_iter][1]
+					):
 						continue
 
-					# handle allow_repeats
+					# handle repeats
 					if self['repeats']:
 						word_fits = all(char in query for char in word)
 
-					# iterate through letters
+					# handle no repeats
 					else:
+						if self['debug']:
+							print(f' - checking [{word}]')
+
+						# iterate through word characters
 						for char in word:
 							query_iter = query_iter.replace(char, ' ', 1)
 							word_iter = word_iter.replace(char, ' ', 1)
 
-							# debug info
-							if self['debug']:
-								print(f'input: {[query_iter]} | {[word]}: {[word_iter]}')
+						# check if word length is correct
+						_length_fits = len(word) == len_iter
+
+						# check if word fits query
+						_spaces_fit = query_iter.count(' ') != 0 \
+							and query_iter.count(' ') == word_iter.count(' ')
+
+						# check if word fits doubles criteria
+						if self['doubles']:
+							_doubles_fits = True
+						else:
+							_doubles_fits = query_iter.count(' ') == \
+								word_iter.count(' ') != 0
+
+						# debug info
+						if self['debug']:
+							print(f'\t{[
+								_length_fits,
+								_spaces_fit,
+								_doubles_fits,
+							]}')
 
 						# check if word fits
-						if query_iter.count(' ') == word_iter.count(' ') != 0:
+						if all([
+							_length_fits,
+							_spaces_fit,
+							_doubles_fits,
+						]):
 							word_fits = True
 
-							# debug info
-							if self['debug']:
-								print(f'{[word]} fits for {[len_iter]}')
 
 				# add word to output
 				if word_fits:
 					scores[len_iter][0].append(word)
 
+					# debug info
+					if self['debug']:
+						print(
+							f'\tinput: [{query_iter}] |',
+							f'[{word}]: [{word_iter}]',
+						)
+						print(f'\t[{word}] fits for [{len_iter}]')
+						if not word_iter.strip() and not query_iter.strip() \
+							and len(word) == len(query):
+							print(f'\tanagram found: [{word}]')
+
 					# update score
 					if not self['noscores']:
-						scores[len_iter][1] = self.scores[scores[len_iter][0][0]]
+						scores[len_iter][1] = self.scores[
+							scores[len_iter][0][0]
+						]
 
 			# debug info
 			if self['debug']:
-				print(f' - output for {[len_iter]}: {scores[len_iter][0]}')
+				print(f'output for [{len_iter}]: {scores[len_iter][0]}')
 
 		# determine whether an anagram was found
 		try:
 			anagram_found = len(scores[len(query)][0][0]) == len(query)
 		except (IndexError, KeyError):
 			anagram_found = False
 
-		# remove empty lists
+		# remove empty or non-compliant lists
 		for key, val in deepcopy(scores).items():
 			with suppress(IndexError, KeyError):
 				if not val:
 					del scores[key]
 					if self['debug']:
-						print(f' - removed {[key]} for empty list')
-				elif not self['noscores'] and any(
-					word in scores[key][0] for word in scores[key-1][0]
+						print(f' - removed [{key}] for empty list')
+					continue
+				if not self['noscores'] and any(
+					word in scores[key][0] for word in scores[key - 1][0]
 				):
 					del scores[key]
 					if self['debug']:
-						print(f' - removed {[key]} for duplicate/s')
+						print(f' - removed [{key}] for duplicate/s')
+					continue
+				if not self['doubles']:
+					for _key in scores:
+						if _key < key and any(
+							self.scores[word] <= self.scores[_word]
+							for word in scores[key][0]
+							for _word in scores[_key][0]
+						):
+							del scores[key]
+							if self['debug']:
+								print(f' - removed [{key}] for doubles')
+							break
+					continue
+				if self['debug']:
+					print(f' - kept [{key}]')
 
 		# return solved object and anagram status
 		return scores, anagram_found
 
 	# solve to string function
 	def solve_str(
-		self,
-		query: str
-	):
+		self: Self,
+		query: str,
+		/,
+	) -> str:
 		'''
-		Finds all possible words that can be formed from the given query string, using the set wordlist.
+		Finds all possible words that can be formed from the given query
+		string, using the set wordlist.
 
 		Args:
-			query (`str`): A string representing the query to be solved.
+		----
+			query: `str`
+				A string representing the query to be solved.
 
 		Returns:
-			`str`: A string representing the output of the solver, formatted with headers and indentation.
+		-------
+			`str`: A string representing the output of the solver, formatted
+			with headers and indentation.
 		'''
 
 		# build query
-		query = build_query(query, not self['repeats'])
+		query = build_query(query, repeat_letters=not self['repeats'])
 
 		# get solved object and anagram status
 		scores, anagram_found = self.solve(query)
 
 		# prepare anagram message
-		anagram_found = '' if anagram_found else '  \t warning: anagram not found\n\n'
+		anagram_found = '' \
+			if anagram_found \
+			else '  \t warning: anagram not found\n\n'
 
 		# return output string
 		return str(
 			f'\n  \t--- query: {query} ({len(query)} letters'
 			+ (' + repeats' if self['repeats'] else '') + ') ---\n\n' + (
 				(
 					anagram_found + '\n\n'.join(
 						f'\t{key} letters'
 						+ (
 							''
 							if self['noscores']
 							else f' - {scores[key][1]} points'
 						) + '\n\t ' + ', '.join(
 							sorted(
-								word.lower() if self['lower'] else word.upper()
+								word.lower()
+								if self['lower']
+								else word.upper()
 								for word in scores[key][0]
-							)
+							),
 						)
-						for key in scores.keys()
+						for key in scores
 						if scores[key][0]
 					)
 				)
-				if any(scores[key][0] for key in scores.keys())
+				if any(scores[key][0] for key in scores)
 				else '\t no words found'
-			) + '\n'
+			) + '\n',
 		)
 
 	# get wordlist
 	def get_wordlist(
-		self,
-		output_type: type = List[str],
-	) -> Any:
+		self: Self,
+		output_type: type = list[str],
+		/,
+	) -> ...:
 		'''
 		Returns the current wordlist, as defined in the ruleset settings.
 
 		Args:
-			`output_type: type`: Type for output to be converted to. Defaults to `list[str]`.
+		----
+			output_type: `type`
+				Type for output to be converted to.
+				Defaults to `list[str]`.
 
 		Returns:
+		-------
 			`Any`: The wordlist, converted to `output_type`.
 		'''
 
 		# return wordlist as specified type
 		return output_type(self.wordlist)
 
+
 # entry point
-def main():
+def main() -> None:
+	'''
+	Provides the functionality for the entrypoint function.
+
+	```sh
+	$ qrs
+	```
+
+	Not intended to be used within scripts,
+	except in this library's `__main__.py`.
+	'''
+
+	# load status
+	ready_for_input = False
 
 	# imports
 	from jarguments import JArgument, JParser
 
 	# get arguments
-	args = JParser(
+	jargs = JParser(
 		*{
-			JArgument(arg, type, default, sarg, nargs, help)
-			for arg, sarg, type, default, nargs, help in kwargs
-		}
+			JArgument(
+				name=arg,
+				type=arg_type,
+				default=None,
+				short_name=sarg,
+				multiple=nargs,
+				help=arg_help,
+			) for arg, sarg, arg_type, _, nargs, arg_help in qrs_kwargs
+		},
 	)
 
 	# show message
 	with suppress(KeyboardInterrupt):
 		print('\n\tloading settings and wordlist..')
 
 		# load settings
 		try:
 			with open(
-				path.join(
-					syspath[0], 'qrs.json'
-				), 'tr'
+				os_path.join(
+					sys_path[0], 'qrs.json',
+				), 'tr',
 			) as settings_file:
 				settings_import = load(settings_file)
 
 		# file is empty
 		except decoder.JSONDecodeError:
 			settings_import = {}
 
 			# display message
-			print('\t\'qrs.json\' is empty or invalid; continuing with default/given settings..')
+			print(
+				'\t\'qrs.json\' is empty or invalid;',
+				'continuing with default/given settings..',
+			)
 
 		# file cannot be loaded
 		except FileNotFoundError:
 			settings_import = {}
 
 			# display message
-			print('\tfailed to load \'qrs.json\'; continuing with default/given settings..')
+			print(
+				'\tcould not find \'qrs.json\';',
+				'continuing with default/given settings..',
+			)
 
 		# load ruleset
 		q = Ruleset(
-			settings=build_settings(
-				{
-					**settings_import, **{
-						arg: getattr(args, arg)
-						for arg, _, _, _, _, _ in kwargs
-						if getattr(args, arg, None) is not None
-					}
-				}
-			)
+			{
+				**settings_import, **{
+					arg: getattr(jargs, arg)
+					for arg, _, _, _, _, _ in qrs_kwargs
+					if getattr(jargs, arg, None) is not None
+				},
+			},
 		)
 
 		# save settings
 		try:
 			with open(
-				path.join(
-					syspath[0], 'qrs.json'
-				), 'tw'
+				os_path.join(
+					sys_path[0], 'qrs.json',
+				), 'tw',
 			) as settings_file:
 				settings_file.write(
-					q.get_settings_str()
+					q.get_settings_str() + '\n',
 				)
 
 		# if settings file cannot be saved
-		except Exception:
-			print('\tfailed to save \'qrs.json\'; continuing without saving..')
+		except OSError:
+			print('\tfailed to save \'qrs.json\';',
+				'continuing without saving..')
 
 		# debug info
-		if (args.debug or q['debug']):
+		if (jargs.debug or q['debug']):
 			print(f'\n{q.get_settings_str()}')
 
-		# show message
+		# prepare for input
+		ready_for_input = True
 		print('\n\t\tdone!\n')
 
 		# input loop
 		while True:
 			query = ''
 			while not all([
 				q['min'] <= len(query) <= q['max'],
-				all(char in ascii_lowercase for char in query)
+				all(char in ascii_lowercase for char in query),
 			]):
 				query = input('qrs: ')
 			print(q.solve_str(query))
 
+	# pretty exit
+	print(
+		'\n' if ready_for_input else '',
+		'\n\texiting..',
+	)
+
+
 # main function
 if __name__ == '__main__':
 	main()
```

### Comparing `qrs-1.2.0/qrs/wordlist.txt` & `qrs-1.3.0/qrs/wordlist.txt`

 * *Files identical despite different names*

### Comparing `qrs-1.2.0/qrs.egg-info/PKG-INFO` & `qrs-1.3.0/qrs.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 Metadata-Version: 2.1
 Name: qrs
-Version: 1.2.0
-Summary: Provides word game-related tools that can be configured with custom settings, letter scores, and wordlists.
+Version: 1.3.0
+Summary: Provides word game-related tools that can be configured with custom settings,
 Home-page: https://github.com/silvncr/qrs
 Author: silvncr
 License: MIT
-Classifier: Programming Language :: Python
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python
 Classifier: Topic :: Games/Entertainment :: Board Games
 Classifier: Topic :: Games/Entertainment :: Puzzle Games
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Classifier: Typing :: Typed
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: jarguments==0.0.1
+Requires-Dist: jarguments==0.1.0
 
 <!-- omit from toc -->
 # qrs
 
 tool for *Quarrel* (and other word games)
 
-![[publish status](https://github.com/silvncr/qrs/actions/workflows/python-publish.yml)](https://img.shields.io/github/actions/workflow/status/silvncr/qrs/python-publish.yml)
-![[latest release](https://github.com/silvncr/qrs/releases/latest)](https://img.shields.io/github/v/release/silvncr/qrs)
+![downloads](https://img.shields.io/pypi/dm/qrs)
+![status](https://img.shields.io/github/actions/workflow/status/silvncr/qrs/python-publish.yml)
+![version](https://img.shields.io/pypi/v/qrs)
 
 ## Summary
 
 Provides word game-related tools that can be configured with custom settings, letter scores, and wordlists.
 
-> Works on Python 3.6 and above. Tested on Windows 10.
+> Supports Python 3.8 and above. Tested on Windows 10.
 
 ## Contents
 
 - [Summary](#summary)
 - [Contents](#contents)
 - [The qrs library](#the-qrs-library)
 - [Direct execution](#direct-execution)
@@ -44,23 +52,17 @@
 Install the qrs library to use its functionality in your projects.
 
 ```sh
 python -m pip install --upgrade qrs
 ```
 
 ```py
->>> from qrs import build_settings, Ruleset
->>> q = Ruleset(
-...     build_settings(
-...         {'max': 8}
-...     )
-... )
->>> print(
-...     q.solve_str('wetodlnm')
-... )
+>>> from qrs import Ruleset
+>>> q = Ruleset({'max': 8})
+>>> print(q.solve_str('wetodlnm'))
 
         --- query: delmnotw (8 letters) ---
 
         8 letters - 18 points
          MELTDOWN
 
         5 letters - 14 points
@@ -84,27 +86,27 @@
 $ qrs
 
 qrs: _
 ```
 
 Upon being called from the command line, it will display an input screen.
 
-Type your letters into the field, press Enter, and wait for the program to calculate the best words. Once done, choose one from the list that corresponds with the number of letters you have available or the next lowest. See the example below to find out why you might not need to use all of your spaces.
+Enter your letters and wait for the program to calculate the best words. Choose one from the list that corresponds with the number of letters you have available, or the next longest. See the example below to find out why you might not need to use all of your spaces.
 
 ## Example case
 
 Here's an example using the default program settings. Our situation is the following:
 
 - We're playing *Quarrel*, and thus, we get eight letters.
 - Our letters are `wetodlnm`.
 - We have seven spaces to use.
 
 After installing the library, we'll open a command line and run the program.
 
-Since we know we don't need words longer than eight letters, we can minimise loading time by configuring the program to only calculate for words of that length. We can do this by passing our desired settings as command arguments:
+The program will have to load a wordlist, which takes longer as the range of word lengths increases. Since we know we don't need words longer than eight letters, we can minimise loading time by configuring the program to only calculate for words of that length. We can do this by passing our desired settings as command arguments:
 
 ```sh
 $ qrs --max 8
 
 qrs: _
 ```
 
@@ -116,15 +118,15 @@
 > ```
 >
 > ```sh
 > ## from folder with qrs.json
 > $ qrs
 > ```
 
-The program will have to load a wordlist whichever way it is run. Once it finishes loading, we can input our letters and press Enter.
+Once it finishes loading, we can enter our letters.
 
 ```py
 qrs: wetodlnm
 
         --- query: delmnotw (8 letters) ---
 
         8 letters - 18 points
@@ -133,45 +135,48 @@
         5 letters - 14 points
          MOWED
 
         4 letters - 12 points
          MEWL
 
         3 letters - 10 points
-         MEW, MOW
+         MEW, MOW, WEM
 
         2 letters - 6 points
-         OW, WE, WO
+         EW, OW, WE, WO
 
 qrs: _
 ```
 
 This output tells us that the anagram is `MELTDOWN`, but we can't make that word because we can only use seven letters. In this case, our best word is `MOWED` (14 points). Based on this output, we also know that our opponent cannot score higher than us without all eight spaces.
 
 > Note: a word like `LETDOWN` scores the same number of points as `MOWED`, but isn't recognised as a "best word" in this case. This is because when words are tied for points, the program will choose the word/s with the fewest letters.
 >
 > The fewer letters your word has, the faster you can write it into your game. This is especially important in *Quarrel*, as the tiebreaker for equal points is input speed.
+>
+> You can choose to display longer, tied words by enabling the `--doubles` setting.
 
 ## Settings
 
 Upon being run from the command line, the program will automatically generate (or look for) a `qrs.json` file in the directory from which the command is run. This file contains the program's settings, which can be changed to suit your needs.
 
-When using qrs as a library, you should pass a `dict` with any of the following keys into `build_settings` to generate a full settings object, then pass the output to a `Ruleset` to create a new instance. Here are all the currently supported settings:
+When using qrs as a library, pass a `dict` with any of the following keys to a `Ruleset` to create a new instance. Here are all the currently supported settings:
 
 | Setting | Default | Description |
-|:-:|:-:|:--|
-| `debug` | `false` | Shows the program's inner workings whilst calculating. Note that this may negatively affect performance on certain devices or IDEs. |
-| `exclude` | `[]` | List of words that the program will never output. |
-| `game` | `"quarrel"` | Determines the letter scoring system used for calculating points. The value here is passed into `build_letter_scores()`, and defaults back if invalid. |
-| `include` | `[]` | List of additional words for the wordlist. |
-| `lower` | `false`| Displays output in lowercase letters. The default setting displays capital letters to mimic the style of word games like *Scrabble* and *Quarrel*, however some people may find lowercase output more readable. |
-| `max` | longest length in wordlist | Determines the maximum word length the program will calculate for. |
-| `min` | `2` | Determines the minimum word length the program will calculate for. |
-| `noscores` | `false` | Determines whether point values for words are considered, in which case only the highest-scoring words are displayed. If you don't care about scoring, turn this on to see all words. |
-| `repeats` | `false` | Determines whether letters can be used more than once. Change this according to your word game's rules; for example, *Scrabble* tiles can only be used once in a single word, whereas *New York Times*'s *Spelling Bee* allows the reuse of letters. |
+| :-: | :-: | :-- |
+| `debug` 🐛 | `false` | Prints the program's inner workings whilst calculating. Note that many consecutive print statements may negatively affect performance on certain devices or IDEs. |
+| `doubles` 🔀 | `false` | Shows longer words that tie for score (like the `MOWED` / `LETDOWN` example above). |
+| `exclude` ⛔ | `[]` | List of words that the program will never output. |
+| `game` 🎮 | `"quarrel"` | Determines the letter scoring system used for calculating points. The value here is passed into `build_letter_scores()`, and defaults back if invalid. |
+| `include` ✔️ | `[]` | List of additional words for the wordlist. |
+| `lower` 💻 | `false` | Displays output in lowercase letters. The default setting displays capital letters to mimic the style of word games like *Scrabble* and *Quarrel*, however some people may find lowercase output more readable. |
+| `max` 🔼 | longest length in wordlist | Determines the maximum word length the program will calculate for. |
+| `min` 🔽 | `2` | Determines the minimum word length the program will calculate for. |
+| `noscores` 💯 | `false` | Determines whether point values for words are considered, in which case only the highest-scoring words are displayed. If you don't care about scoring, turn this on to see all words. |
+| `repeats` 🔁 | `false` | Determines whether letters can be used more than once. Change this according to your word game's rules; for example, *Scrabble* tiles can only be used once in a word, whereas *New York Times*'s *Spelling Bee* allows the reuse of letters. |
 
 When running directly:
 
 - To change your settings, do one of the following:
   - Open `qrs.json` in a text editor and change any values. Make sure to save the file once you're done.
   - Pass the setting as a command argument like this: `--setting value`
     - If applicable, this will automatically update the settings file.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

