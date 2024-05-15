# Comparing `tmp/mci_dibse_lt2713_matrix_chatbot_generator-1.0.0.tar.gz` & `tmp/mci_dibse_lt2713_matrix_chatbot_generator-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mci_dibse_lt2713_matrix_chatbot_generator-1.0.0.tar", last modified: Wed May 15 16:31:11 2024, max compression
+gzip compressed data, was "mci_dibse_lt2713_matrix_chatbot_generator-1.0.1.tar", last modified: Wed May 15 17:23:05 2024, max compression
```

## Comparing `mci_dibse_lt2713_matrix_chatbot_generator-1.0.0.tar` & `mci_dibse_lt2713_matrix_chatbot_generator-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 16:31:11.987979 mci_dibse_lt2713_matrix_chatbot_generator-1.0.0/
--rw-rw-rw-   0        0        0      407 2024-05-15 16:31:11.987979 mci_dibse_lt2713_matrix_chatbot_generator-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-15 16:31:11.977324 mci_dibse_lt2713_matrix_chatbot_generator-1.0.0/classes/
--rw-rw-rw-   0        0        0      905 2024-05-15 14:58:55.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.0/classes/ChatbotGenerator.py
--rw-rw-rw-   0        0        0     3730 2024-05-15 14:31:43.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.0/classes/QTIParser.py
--rw-rw-rw-   0        0        0     4861 2024-05-15 14:57:01.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.0/classes/UserInterface.py
--rw-rw-rw-   0        0        0       86 2024-05-15 15:56:07.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.0/classes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:31:11.980449 mci_dibse_lt2713_matrix_chatbot_generator-1.0.0/main/
--rw-rw-rw-   0        0        0      105 2024-05-15 16:26:29.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.0/main/__init__.py
--rw-rw-rw-   0        0        0      277 2024-05-15 14:57:53.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.0/main/call_user_interface.py
--rw-rw-rw-   0        0        0        0 2024-05-02 15:14:24.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.0/main/generate_chatbot.py
--rw-rw-rw-   0        0        0       86 2024-05-15 14:48:30.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.0/main/start_user_interface.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:31:11.983845 mci_dibse_lt2713_matrix_chatbot_generator-1.0.0/mci_dibse_lt2713_matrix_chatbot_generator.egg-info/
--rw-rw-rw-   0        0        0      407 2024-05-15 16:31:11.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.0/mci_dibse_lt2713_matrix_chatbot_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      601 2024-05-15 16:31:11.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.0/mci_dibse_lt2713_matrix_chatbot_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 16:31:11.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.0/mci_dibse_lt2713_matrix_chatbot_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-15 16:31:11.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.0/mci_dibse_lt2713_matrix_chatbot_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 16:31:11.988986 mci_dibse_lt2713_matrix_chatbot_generator-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      461 2024-05-15 16:10:14.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:31:11.986858 mci_dibse_lt2713_matrix_chatbot_generator-1.0.0/structures/
--rw-rw-rw-   0        0        0      122 2024-05-15 15:56:07.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.0/structures/__init__.py
--rw-rw-rw-   0        0        0      664 2024-05-15 14:16:21.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.0/structures/answer.py
--rw-rw-rw-   0        0        0      405 2024-05-15 14:16:21.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.0/structures/feedback.py
--rw-rw-rw-   0        0        0     2649 2024-05-15 15:00:07.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.0/structures/question.py
--rw-rw-rw-   0        0        0      666 2024-05-15 15:01:57.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.0/structures/questions.py
--rw-rw-rw-   0        0        0      747 2024-05-15 14:40:04.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.0/structures/transaction.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:23:05.315644 mci_dibse_lt2713_matrix_chatbot_generator-1.0.1/
+-rw-rw-rw-   0        0        0      407 2024-05-15 17:23:05.315644 mci_dibse_lt2713_matrix_chatbot_generator-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-15 17:23:05.303322 mci_dibse_lt2713_matrix_chatbot_generator-1.0.1/main/
+-rw-rw-rw-   0        0        0      105 2024-05-15 16:26:29.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.1/main/__init__.py
+-rw-rw-rw-   0        0        0      277 2024-05-15 14:57:53.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.1/main/call_user_interface.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:23:05.306927 mci_dibse_lt2713_matrix_chatbot_generator-1.0.1/main/classes/
+-rw-rw-rw-   0        0        0      793 2024-05-15 17:21:16.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.1/main/classes/ChatbotGenerator.py
+-rw-rw-rw-   0        0        0     3750 2024-05-15 17:21:16.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.1/main/classes/QTIParser.py
+-rw-rw-rw-   0        0        0     4821 2024-05-15 17:21:16.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.1/main/classes/UserInterface.py
+-rw-rw-rw-   0        0        0       86 2024-05-15 15:56:07.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.1/main/classes/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-02 15:14:24.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.1/main/generate_chatbot.py
+-rw-rw-rw-   0        0        0       86 2024-05-15 14:48:30.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.1/main/start_user_interface.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:23:05.311430 mci_dibse_lt2713_matrix_chatbot_generator-1.0.1/main/structures/
+-rw-rw-rw-   0        0        0      122 2024-05-15 15:56:07.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.1/main/structures/__init__.py
+-rw-rw-rw-   0        0        0      664 2024-05-15 14:16:21.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.1/main/structures/answer.py
+-rw-rw-rw-   0        0        0      405 2024-05-15 14:16:21.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.1/main/structures/feedback.py
+-rw-rw-rw-   0        0        0     2565 2024-05-15 17:21:16.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.1/main/structures/question.py
+-rw-rw-rw-   0        0        0      671 2024-05-15 17:21:16.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.1/main/structures/questions.py
+-rw-rw-rw-   0        0        0      747 2024-05-15 14:40:04.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.1/main/structures/transaction.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:23:05.314646 mci_dibse_lt2713_matrix_chatbot_generator-1.0.1/mci_dibse_lt2713_matrix_chatbot_generator.egg-info/
+-rw-rw-rw-   0        0        0      407 2024-05-15 17:23:05.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.1/mci_dibse_lt2713_matrix_chatbot_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      651 2024-05-15 17:23:05.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.1/mci_dibse_lt2713_matrix_chatbot_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 17:23:05.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.1/mci_dibse_lt2713_matrix_chatbot_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-15 17:23:05.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.1/mci_dibse_lt2713_matrix_chatbot_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 17:23:05.315644 mci_dibse_lt2713_matrix_chatbot_generator-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      461 2024-05-15 17:22:00.000000 mci_dibse_lt2713_matrix_chatbot_generator-1.0.1/setup.py
```

### Comparing `mci_dibse_lt2713_matrix_chatbot_generator-1.0.0/classes/ChatbotGenerator.py` & `mci_dibse_lt2713_matrix_chatbot_generator-1.0.1/main/classes/ChatbotGenerator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-from structures.transaction import Transaction
-from structures.questions import Questions
-from structures.question import Question
-from structures.answer import Answer
-from structures.feedback import Feedback
+from main.structures.transaction import Transaction
+from main.structures.questions import Questions
 
 
 class ChatbotGenerator:
     def __init__(self, transaction, questions):
         if isinstance(transaction, Transaction):
             self.transaction = transaction
         else:
```

### Comparing `mci_dibse_lt2713_matrix_chatbot_generator-1.0.0/classes/QTIParser.py` & `mci_dibse_lt2713_matrix_chatbot_generator-1.0.1/main/classes/QTIParser.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import xml.etree.ElementTree as ET
-from structures.questions import Questions
-from structures.question import Question
-from structures.answer import Answer
-from structures.feedback import Feedback
+from main.structures.questions import Questions
+from main.structures.question import Question
+from main.structures.answer import Answer
+from main.structures.feedback import Feedback
 
 
 class QTIParser:
     def __init__(self, file=None):
         if not file:
             self.file = 'lt_testquiz.xml'
         else:
```

### Comparing `mci_dibse_lt2713_matrix_chatbot_generator-1.0.0/classes/UserInterface.py` & `mci_dibse_lt2713_matrix_chatbot_generator-1.0.1/main/classes/UserInterface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import tkinter as tk
-import uuid
 from tkinter import filedialog
 from tkinter import ttk
 from tkinter import messagebox
 import os
-from structures.transaction import Transaction
-from structures.question import Question
-from classes.QTIParser import QTIParser
-from classes.ChatbotGenerator import ChatbotGenerator
+from main.structures.transaction import Transaction
+from main.classes.QTIParser import QTIParser
+from main.classes.ChatbotGenerator import ChatbotGenerator
 
 
 class UserInterface:
     def __init__(self, questions=None):
         self.fileselection = not questions
         if not self.fileselection:
             self.questions = questions
```

### Comparing `mci_dibse_lt2713_matrix_chatbot_generator-1.0.0/structures/answer.py` & `mci_dibse_lt2713_matrix_chatbot_generator-1.0.1/main/structures/answer.py`

 * *Files identical despite different names*

### Comparing `mci_dibse_lt2713_matrix_chatbot_generator-1.0.0/structures/question.py` & `mci_dibse_lt2713_matrix_chatbot_generator-1.0.1/main/structures/question.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-from structures.answer import Answer
-from structures.feedback import Feedback
-
-
 class Question:
     def __init__(self, identifier, question_type, text=None, answers=None, feedback=None):
         self.id = identifier
         self.type = question_type
         if text is None:
             self.text = ' '
         else:
```

### Comparing `mci_dibse_lt2713_matrix_chatbot_generator-1.0.0/structures/questions.py` & `mci_dibse_lt2713_matrix_chatbot_generator-1.0.1/main/structures/questions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from structures.question import Question
+from main.structures.question import Question
 
 
 class Questions:
     def __init__(self, questions=None):
         if questions:
             self.questions = questions
         else:
```

### Comparing `mci_dibse_lt2713_matrix_chatbot_generator-1.0.0/structures/transaction.py` & `mci_dibse_lt2713_matrix_chatbot_generator-1.0.1/main/structures/transaction.py`

 * *Files identical despite different names*

