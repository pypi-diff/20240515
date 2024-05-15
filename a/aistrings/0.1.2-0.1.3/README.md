# Comparing `tmp/aistrings-0.1.2.tar.gz` & `tmp/aistrings-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aistrings-0.1.2.tar", max compression
+gzip compressed data, was "aistrings-0.1.3.tar", max compression
```

## Comparing `aistrings-0.1.2.tar` & `aistrings-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1075 2024-05-14 12:02:20.808856 aistrings-0.1.2/LICENSE
--rw-r--r--   0        0        0     4122 2024-05-14 16:46:08.409320 aistrings-0.1.2/README.md
--rw-r--r--   0        0        0       28 2024-05-14 20:02:17.831668 aistrings-0.1.2/aistrings/__init__.py
--rw-r--r--   0        0        0     4100 2024-05-14 20:03:31.003148 aistrings-0.1.2/aistrings/astr.py
--rw-r--r--   0        0        0        0 2024-05-14 08:32:15.520265 aistrings-0.1.2/aistrings/models/__init__.py
--rw-r--r--   0        0        0      249 2024-05-14 16:46:08.412076 aistrings-0.1.2/aistrings/models/base.py
--rw-r--r--   0        0        0     1557 2024-05-14 19:51:46.243536 aistrings-0.1.2/aistrings/models/openai.py
--rw-r--r--   0        0        0      450 2024-05-14 20:04:35.524374 aistrings-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4903 1970-01-01 00:00:00.000000 aistrings-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-05-14 12:02:20.808856 aistrings-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4260 2024-05-15 11:40:19.387161 aistrings-0.1.3/README.md
+-rw-r--r--   0        0        0       28 2024-05-14 20:11:45.402871 aistrings-0.1.3/aistrings/__init__.py
+-rw-r--r--   0        0        0     7124 2024-05-15 11:42:59.404349 aistrings-0.1.3/aistrings/astr.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:32:15.520265 aistrings-0.1.3/aistrings/models/__init__.py
+-rw-r--r--   0        0        0      249 2024-05-14 20:11:45.404115 aistrings-0.1.3/aistrings/models/base.py
+-rw-r--r--   0        0        0     1557 2024-05-14 20:11:45.404859 aistrings-0.1.3/aistrings/models/openai.py
+-rw-r--r--   0        0        0      450 2024-05-15 11:45:17.708943 aistrings-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5041 1970-01-01 00:00:00.000000 aistrings-0.1.3/PKG-INFO
```

### Comparing `aistrings-0.1.2/LICENSE` & `aistrings-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aistrings-0.1.2/README.md` & `aistrings-0.1.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 AiStrings uses language models to build a string API that is aware of semantics.
 The built in string APIs operate on syntax or morphology.
 For example matching two strings with a regex or a fuzzy string matching algorithm will never match
 2 strings that essentially mean the same but look completely different.
 
 AiStrings provides semantics aware string APIs with a familiar interface.
 
+```bash
+pip install aistrings
+```
+
+Make sure to set `OPENAI_API_KEY` in your `.env` file or directly in your environment.
+
 ```python
 from dotenv import load_dotenv
 from aistrings import AiStrings
 
 load_dotenv()
 
 astr = AiStrings(provider_name="openai", model_name="gpt-3.5-turbo-0125")
@@ -19,122 +25,121 @@
     "The cat sleeps too much",
     "The dog jumps over the fence",
     "The cat jumps over the fence",
     "I am so happy"
 ]
 query = "The cat is very agile!"
 
-response, index = astr.match(query, targets)
-print(f"Option at index {index} is the best: \"{response}\"")
+response, index = astr.find(query, targets)
+print(f"Index: {index}, Target: \"{response}\"")
 ```
 
 ```
-Option at index 2 is the best: "The cat jumps over the fence"
+Index: 2, Target: "The cat jumps over the fence"
 ```
 
 Keep track of the costs with:
 
 ```python
 astr.log_history()
 # or
 print("Total Cost: ", astr.cumulative_cost)
 ```
 
 ```
 History
 ----------------------
-  Action: match
+  Action: find
   Input: The cat is very agile!
   Output: The cat jumps over the fence
   Cost: 4.35e-05
   Time: 2024-05-14 14:50:25.698692
 
 Total Cost: 4.35e-05
 ----------------------
 # or
 Total Cost: 4.35e-05
 ```
 
 Currently available operations:
 
-- astr.summarize
-- astr.match
+- astr.find
 - astr.split
-
-coming soon:
 - astr.replace
 - astr.substr
+- astr.match
+- astr.summarize
+
+coming soon:
+
 - astr.translate
 - astr.answer
 - astr.is_factual
 - astr.make_verbose
 - astr.elaborate
 - astr.correct_grammar
 - astr.detect_lang
 - astr.detect_sentiment
 
 ## More Examples
 
-### Split
+For all examples first run
 
-```python
+```
 from dotenv import load_dotenv
-
 from aistrings import AiStrings
-
 load_dotenv()
+astr = AiStrings(provider_name="openai", model_name="gpt-4-0125-preview")
+```
 
-astr = AiStrings(provider_name="openai", model_name="gpt-4-0125-preview", temperature=1)
+### Replace
 
+```python
+text = "I have never seen Saturn through a telescope, but I would really love to see it once."
+criterion = "Replace every single verb in the text with the word cat."
+response = astr.replace(text, criterion)
+print(response)
+```
+
+```
+I cat never cat Saturn through a telescope, but I cat really cat to cat it once.
+```
+
+### Split
+
+```python
 text = "I have never seen Saturn through a telescope, but I would really love to see it once."
 criterion = "Split the text using names of planets of the solar system as separators."
 response = astr.split(text, criterion)
-astr.log_history()
 print(response)
 ```
 
 ```
 ['I have never seen ', ' through a telescope, but I would really love to see it once.']
 ```
 
 ### Join
 
 ```python
-from dotenv import load_dotenv
-
-from aistrings import AiStrings
-
-load_dotenv()
-
-astr = AiStrings(provider_name="openai", model_name="gpt-4-0125-preview")
-
 text_list = [
     "The cat sleeps too much during the day, so it wakes up in the night and wants to play.",
     "When the cat wakes up in the night and wants to play it usually starts walking across my pillow.",
 ]
 criterion = "Join the texts and remove duplicate information and use as few words as possible."
-
 response = astr.join(text_list, criterion)
 print(response)
 ```
 
 ```
 The cat sleeps too much during the day, so it wakes up in the night and wants to play, usually starting by walking across my pillow.
 ```
 
 ### Summarize
 
 ```python
-from dotenv import load_dotenv
-
-from aistrings import AiStrings
-
-load_dotenv()
-
-astr = AiStrings(provider_name="openai", model_name="gpt-3.5-turbo-0125")
 response = astr.summarize(
     "Mars is the fourth planet from the Sun. The surface of Mars is orange-red because it is covered in iron(III) oxide dust, giving it the nickname 'the Red Planet'.[21][22]"
     " Mars is among the brightest objects in Earth's sky, and its high-contrast albedo features have made it a common subject for telescope viewing. "
     "It is classified as a terrestrial planet and is the second smallest of the Solar System's planets with a diameter of 6,779 km (4,212 mi). "
     "In terms of orbital motion, a Martian solar day (sol) is equal to 24.5 hours, and a Martian solar year is equal to 1.88 Earth years (687 Earth days). "
     "Mars has two natural satellites that are small and irregular in shape: Phobos and Deimos. "
 )
```

### Comparing `aistrings-0.1.2/aistrings/models/openai.py` & `aistrings-0.1.3/aistrings/models/openai.py`

 * *Files identical despite different names*

### Comparing `aistrings-0.1.2/PKG-INFO` & `aistrings-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aistrings
-Version: 0.1.2
+Version: 0.1.3
 Summary: An API to manipulate strings semantically.
 Home-page: https://github.com/daniele-roncaglioni/aistrings
 License: MIT
 Author: roncaglionidaniele
 Author-email: roncaglionidaniele@icloud.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -23,14 +23,20 @@
 AiStrings uses language models to build a string API that is aware of semantics.
 The built in string APIs operate on syntax or morphology.
 For example matching two strings with a regex or a fuzzy string matching algorithm will never match
 2 strings that essentially mean the same but look completely different.
 
 AiStrings provides semantics aware string APIs with a familiar interface.
 
+```bash
+pip install aistrings
+```
+
+Make sure to set `OPENAI_API_KEY` in your `.env` file or directly in your environment.
+
 ```python
 from dotenv import load_dotenv
 from aistrings import AiStrings
 
 load_dotenv()
 
 astr = AiStrings(provider_name="openai", model_name="gpt-3.5-turbo-0125")
@@ -39,122 +45,121 @@
     "The cat sleeps too much",
     "The dog jumps over the fence",
     "The cat jumps over the fence",
     "I am so happy"
 ]
 query = "The cat is very agile!"
 
-response, index = astr.match(query, targets)
-print(f"Option at index {index} is the best: \"{response}\"")
+response, index = astr.find(query, targets)
+print(f"Index: {index}, Target: \"{response}\"")
 ```
 
 ```
-Option at index 2 is the best: "The cat jumps over the fence"
+Index: 2, Target: "The cat jumps over the fence"
 ```
 
 Keep track of the costs with:
 
 ```python
 astr.log_history()
 # or
 print("Total Cost: ", astr.cumulative_cost)
 ```
 
 ```
 History
 ----------------------
-  Action: match
+  Action: find
   Input: The cat is very agile!
   Output: The cat jumps over the fence
   Cost: 4.35e-05
   Time: 2024-05-14 14:50:25.698692
 
 Total Cost: 4.35e-05
 ----------------------
 # or
 Total Cost: 4.35e-05
 ```
 
 Currently available operations:
 
-- astr.summarize
-- astr.match
+- astr.find
 - astr.split
-
-coming soon:
 - astr.replace
 - astr.substr
+- astr.match
+- astr.summarize
+
+coming soon:
+
 - astr.translate
 - astr.answer
 - astr.is_factual
 - astr.make_verbose
 - astr.elaborate
 - astr.correct_grammar
 - astr.detect_lang
 - astr.detect_sentiment
 
 ## More Examples
 
-### Split
+For all examples first run
 
-```python
+```
 from dotenv import load_dotenv
-
 from aistrings import AiStrings
-
 load_dotenv()
+astr = AiStrings(provider_name="openai", model_name="gpt-4-0125-preview")
+```
 
-astr = AiStrings(provider_name="openai", model_name="gpt-4-0125-preview", temperature=1)
+### Replace
 
+```python
+text = "I have never seen Saturn through a telescope, but I would really love to see it once."
+criterion = "Replace every single verb in the text with the word cat."
+response = astr.replace(text, criterion)
+print(response)
+```
+
+```
+I cat never cat Saturn through a telescope, but I cat really cat to cat it once.
+```
+
+### Split
+
+```python
 text = "I have never seen Saturn through a telescope, but I would really love to see it once."
 criterion = "Split the text using names of planets of the solar system as separators."
 response = astr.split(text, criterion)
-astr.log_history()
 print(response)
 ```
 
 ```
 ['I have never seen ', ' through a telescope, but I would really love to see it once.']
 ```
 
 ### Join
 
 ```python
-from dotenv import load_dotenv
-
-from aistrings import AiStrings
-
-load_dotenv()
-
-astr = AiStrings(provider_name="openai", model_name="gpt-4-0125-preview")
-
 text_list = [
     "The cat sleeps too much during the day, so it wakes up in the night and wants to play.",
     "When the cat wakes up in the night and wants to play it usually starts walking across my pillow.",
 ]
 criterion = "Join the texts and remove duplicate information and use as few words as possible."
-
 response = astr.join(text_list, criterion)
 print(response)
 ```
 
 ```
 The cat sleeps too much during the day, so it wakes up in the night and wants to play, usually starting by walking across my pillow.
 ```
 
 ### Summarize
 
 ```python
-from dotenv import load_dotenv
-
-from aistrings import AiStrings
-
-load_dotenv()
-
-astr = AiStrings(provider_name="openai", model_name="gpt-3.5-turbo-0125")
 response = astr.summarize(
     "Mars is the fourth planet from the Sun. The surface of Mars is orange-red because it is covered in iron(III) oxide dust, giving it the nickname 'the Red Planet'.[21][22]"
     " Mars is among the brightest objects in Earth's sky, and its high-contrast albedo features have made it a common subject for telescope viewing. "
     "It is classified as a terrestrial planet and is the second smallest of the Solar System's planets with a diameter of 6,779 km (4,212 mi). "
     "In terms of orbital motion, a Martian solar day (sol) is equal to 24.5 hours, and a Martian solar year is equal to 1.88 Earth years (687 Earth days). "
     "Mars has two natural satellites that are small and irregular in shape: Phobos and Deimos. "
 )
```

