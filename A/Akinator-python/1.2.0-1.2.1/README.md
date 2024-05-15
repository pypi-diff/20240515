# Comparing `tmp/Akinator-python-1.2.0.tar.gz` & `tmp/Akinator-python-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Akinator-python-1.2.0.tar", last modified: Tue May 14 03:17:54 2024, max compression
+gzip compressed data, was "Akinator-python-1.2.1.tar", last modified: Wed May 15 09:44:19 2024, max compression
```

## Comparing `Akinator-python-1.2.0.tar` & `Akinator-python-1.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 03:17:54.016808 Akinator-python-1.2.0/
-drwxrwxrwx   0        0        0        0 2024-05-14 03:17:54.008349 Akinator-python-1.2.0/Akinator_python.egg-info/
--rw-rw-rw-   0        0        0     3914 2024-05-14 03:17:53.000000 Akinator-python-1.2.0/Akinator_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2024-05-14 03:17:53.000000 Akinator-python-1.2.0/Akinator_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 03:17:53.000000 Akinator-python-1.2.0/Akinator_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-14 03:17:53.000000 Akinator-python-1.2.0/Akinator_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3914 2024-05-14 03:17:54.016808 Akinator-python-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3463 2024-05-14 03:02:57.000000 Akinator-python-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 03:17:54.013327 Akinator-python-1.2.0/akinator_python/
--rw-rw-rw-   0        0        0      121 2024-05-14 03:17:21.000000 Akinator-python-1.2.0/akinator_python/__init__.py
--rw-rw-rw-   0        0        0     4522 2024-05-14 03:16:39.000000 Akinator-python-1.2.0/akinator_python/main.py
--rw-rw-rw-   0        0        0       42 2024-05-14 03:17:54.016808 Akinator-python-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      742 2024-05-14 03:17:39.000000 Akinator-python-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 09:44:19.594107 Akinator-python-1.2.1/
+drwxrwxrwx   0        0        0        0 2024-05-15 09:44:19.579880 Akinator-python-1.2.1/Akinator_python.egg-info/
+-rw-rw-rw-   0        0        0     3914 2024-05-15 09:44:18.000000 Akinator-python-1.2.1/Akinator_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2024-05-15 09:44:19.000000 Akinator-python-1.2.1/Akinator_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 09:44:18.000000 Akinator-python-1.2.1/Akinator_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-15 09:44:18.000000 Akinator-python-1.2.1/Akinator_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3914 2024-05-15 09:44:19.594107 Akinator-python-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3463 2024-05-14 03:02:57.000000 Akinator-python-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 09:44:19.594107 Akinator-python-1.2.1/akinator_python/
+-rw-rw-rw-   0        0        0      121 2024-05-15 09:38:40.000000 Akinator-python-1.2.1/akinator_python/__init__.py
+-rw-rw-rw-   0        0        0     4574 2024-05-15 09:42:55.000000 Akinator-python-1.2.1/akinator_python/main.py
+-rw-rw-rw-   0        0        0       42 2024-05-15 09:44:19.594107 Akinator-python-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      742 2024-05-15 09:43:54.000000 Akinator-python-1.2.1/setup.py
```

### Comparing `Akinator-python-1.2.0/Akinator_python.egg-info/PKG-INFO` & `Akinator-python-1.2.1/Akinator_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akinator-python
-Version: 1.2.0
+Version: 1.2.1
 Summary: A API wrapper for the AkinatorAPI
 Home-page: https://github.com/taka-4602/Akinator-python
 Author: taka4602
 Author-email: shun4602@gmail.com
 Keywords: akinator
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Akinator-python-1.2.0/PKG-INFO` & `Akinator-python-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akinator-python
-Version: 1.2.0
+Version: 1.2.1
 Summary: A API wrapper for the AkinatorAPI
 Home-page: https://github.com/taka-4602/Akinator-python
 Author: taka4602
 Author-email: shun4602@gmail.com
 Keywords: akinator
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Akinator-python-1.2.0/README.md` & `Akinator-python-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `Akinator-python-1.2.0/akinator_python/main.py` & `Akinator-python-1.2.1/akinator_python/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,25 +14,28 @@
             sid=1
         elif theme=="objects":
             sid=2
         elif theme=="animals":
             sid=14
         else:
             raise AkinatorError("the theme must be 'characters' / 'objects' / 'animals'")
-        self.session=requests.session()
         self.json={
             "step":0,
             "progression":0.0,
             "sid":sid,
             "cm":child_mode,
             "answer":0,
         }
 
     def start_game(self):
-        game=self.session.post(f"{self.ENDPOINT}game",json={"sid":self.json["sid"],"cm":self.json["cm"]}).text
+        self.name=None
+        self.description=None
+        self.photo=None
+        self.answer_id=None
+        game=requests.post(f"{self.ENDPOINT}game",json={"sid":self.json["sid"],"cm":self.json["cm"]}).text
         soup = BeautifulSoup(game,"html.parser")
         askSoundlike=soup.find(id="askSoundlike")
         question_label=soup.find(id="question-label").get_text()
         session_id=askSoundlike.find(id="session").get("value")
         signature_id=askSoundlike.find(id="signature").get("value")
         self.json["session"]=session_id
         self.json["signature"]=signature_id
@@ -51,15 +54,15 @@
         elif answer=="p":
             self.json["answer"]=3
         elif answer=="pn":
             self.json["answer"]=4
         else:
             raise AkinatorError("the answer must be 'y' / 'n' / 'idk' / 'p' / 'pn'")
         try:
-            progression=self.session.post(f"{self.ENDPOINT}answer",json=self.json)
+            progression=requests.post(f"{self.ENDPOINT}answer",json=self.json)
             progression=progression.json()
             if progression["completion"]=="KO":
                 raise AkinatorError("completion : KO")
             try:
                 self.json["step"]=int(progression["step"])
                 self.json["progression"]=float(progression["progression"])
                 self.step=int(progression["step"])
@@ -81,15 +84,15 @@
         self.photo=None
         self.answer_id=None
         if self.json["step"]==0:
             raise AkinatorError("it's first question")
         if "answer" in self.json:
             del self.json["answer"]
         try:
-            goback=self.session.post(f"{self.ENDPOINT}cancel_answer",json=self.json)
+            goback=requests.post(f"{self.ENDPOINT}cancel_answer",json=self.json)
             goback=goback.json()
             self.json["step"]=int(goback["step"])
             self.json["progression"]=float(goback["progression"])
             self.step=int(goback["step"])
             self.progression=float(goback["progression"])
             self.question=goback["question"]
             self.question_id=goback["question_id"]
@@ -101,15 +104,15 @@
         self.name=None
         self.description=None
         self.photo=None
         self.answer_id=None
         if "answer" in self.json:
             del self.json["answer"]
         try:
-            exclude=self.session.post(f"{self.ENDPOINT}exclude",json=self.json)
+            exclude=requests.post(f"{self.ENDPOINT}exclude",json=self.json)
             exclude=exclude.json()
             self.json["step"]=int(self.json["step"])
             self.json["progression"]=float(self.json["progression"])
             self.step=int(exclude["step"])
             self.progression=float(exclude["progression"])
             self.question=exclude["question"]
             self.question_id=exclude["question_id"]
```

### Comparing `Akinator-python-1.2.0/setup.py` & `Akinator-python-1.2.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 def load_readme() -> str:
     with open("README.md",encoding="utf-8_sig") as fin:
         return fin.read()
 setup(
     name='Akinator-python',
-    version='1.2.0',
+    version='1.2.1',
     keywords = "akinator",
     long_description=load_readme(),
     long_description_content_type="text/markdown",
     author='taka4602',
     author_email='shun4602@gmail.com',
     url='https://github.com/taka-4602/Akinator-python',
     description='A API wrapper for the AkinatorAPI',
```

