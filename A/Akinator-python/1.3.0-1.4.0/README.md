# Comparing `tmp/Akinator-python-1.3.0.tar.gz` & `tmp/Akinator-python-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Akinator-python-1.3.0.tar", last modified: Wed May 15 16:42:15 2024, max compression
+gzip compressed data, was "Akinator-python-1.4.0.tar", last modified: Wed May 15 17:34:27 2024, max compression
```

## Comparing `Akinator-python-1.3.0.tar` & `Akinator-python-1.4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 16:42:15.136895 Akinator-python-1.3.0/
-drwxrwxrwx   0        0        0        0 2024-05-15 16:42:15.122640 Akinator-python-1.3.0/Akinator_python.egg-info/
--rw-rw-rw-   0        0        0     3914 2024-05-15 16:42:15.000000 Akinator-python-1.3.0/Akinator_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2024-05-15 16:42:15.000000 Akinator-python-1.3.0/Akinator_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 16:42:15.000000 Akinator-python-1.3.0/Akinator_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-15 16:42:15.000000 Akinator-python-1.3.0/Akinator_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3914 2024-05-15 16:42:15.135882 Akinator-python-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     3463 2024-05-14 03:02:57.000000 Akinator-python-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 16:42:15.134453 Akinator-python-1.3.0/akinator_python/
--rw-rw-rw-   0        0        0      121 2024-05-15 16:41:10.000000 Akinator-python-1.3.0/akinator_python/__init__.py
--rw-rw-rw-   0        0        0     4566 2024-05-15 16:40:33.000000 Akinator-python-1.3.0/akinator_python/main.py
--rw-rw-rw-   0        0        0       42 2024-05-15 16:42:15.136895 Akinator-python-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0      742 2024-05-15 16:40:58.000000 Akinator-python-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:34:27.107308 Akinator-python-1.4.0/
+drwxrwxrwx   0        0        0        0 2024-05-15 17:34:27.095764 Akinator-python-1.4.0/Akinator_python.egg-info/
+-rw-rw-rw-   0        0        0     3914 2024-05-15 17:34:26.000000 Akinator-python-1.4.0/Akinator_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2024-05-15 17:34:26.000000 Akinator-python-1.4.0/Akinator_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 17:34:26.000000 Akinator-python-1.4.0/Akinator_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-15 17:34:26.000000 Akinator-python-1.4.0/Akinator_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3914 2024-05-15 17:34:27.106310 Akinator-python-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3463 2024-05-14 03:02:57.000000 Akinator-python-1.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 17:34:27.104210 Akinator-python-1.4.0/akinator_python/
+-rw-rw-rw-   0        0        0      121 2024-05-15 17:34:00.000000 Akinator-python-1.4.0/akinator_python/__init__.py
+-rw-rw-rw-   0        0        0     5085 2024-05-15 17:32:30.000000 Akinator-python-1.4.0/akinator_python/main.py
+-rw-rw-rw-   0        0        0       42 2024-05-15 17:34:27.107308 Akinator-python-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      742 2024-05-15 17:33:47.000000 Akinator-python-1.4.0/setup.py
```

### Comparing `Akinator-python-1.3.0/Akinator_python.egg-info/PKG-INFO` & `Akinator-python-1.4.0/Akinator_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akinator-python
-Version: 1.3.0
+Version: 1.4.0
 Summary: A API wrapper for the AkinatorAPI
 Home-page: https://github.com/taka-4602/Akinator-python
 Author: taka4602
 Author-email: shun4602@gmail.com
 Keywords: akinator
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Akinator-python-1.3.0/PKG-INFO` & `Akinator-python-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akinator-python
-Version: 1.3.0
+Version: 1.4.0
 Summary: A API wrapper for the AkinatorAPI
 Home-page: https://github.com/taka-4602/Akinator-python
 Author: taka4602
 Author-email: shun4602@gmail.com
 Keywords: akinator
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Akinator-python-1.3.0/README.md` & `Akinator-python-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `Akinator-python-1.3.0/akinator_python/main.py` & `Akinator-python-1.4.0/akinator_python/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 class Akinator():
     def __init__(self,theme:str="characters",lang:str="jp",child_mode:bool=False) -> None:
         self.ENDPOINT=f"https://{lang}.akinator.com/"
         self.name=None
         self.description=None
         self.photo=None
         self.answer_id=None
+        self.akitude=None
         if theme=="characters":
             sid=1
         elif theme=="objects":
             sid=2
         elif theme=="animals":
             sid=14
         else:
@@ -27,14 +28,15 @@
         }
 
     def start_game(self):
         self.name=None
         self.description=None
         self.photo=None
         self.answer_id=None
+        self.akitude="https://en.akinator.com/assets/img/akitudes_670x1096/defi.png"
         game=requests.post(f"{self.ENDPOINT}game",json={"sid":self.json["sid"],"cm":self.json["cm"]}).text
         soup = BeautifulSoup(game,"html.parser")
         askSoundlike=soup.find(id="askSoundlike")
         question_label=soup.find(id="question-label").get_text()
         session_id=askSoundlike.find(id="session").get("value")
         signature_id=askSoundlike.find(id="signature").get("value")
         self.json["session"]=session_id
@@ -65,21 +67,23 @@
             try:
                 self.json["step"]=int(progression["step"])
                 self.json["progression"]=float(progression["progression"])
                 self.step=int(progression["step"])
                 self.progression=float(progression["progression"])
                 self.question=progression["question"]
                 self.question_id=progression["question_id"]
+                self.akitude=f"https://en.akinator.com/assets/img/akitudes_670x1096/{progression['akitude']}"
             except:
                 self.name=progression["name_proposition"]
                 self.description=progression["description_proposition"]
                 self.photo=progression["photo"]
                 self.answer_id=progression["id_proposition"]
+                self.json["step_last_proposition"]=int(self.json["step"])
             return progression
-        except:
+        except Exception as e:
             raise AkinatorError(progression)
 
     def go_back(self):
         self.name=None
         self.description=None
         self.photo=None
         self.answer_id=None
@@ -92,14 +96,15 @@
             goback=goback.json()
             self.json["step"]=int(goback["step"])
             self.json["progression"]=float(goback["progression"])
             self.step=int(goback["step"])
             self.progression=float(goback["progression"])
             self.question=goback["question"]
             self.question_id=goback["question_id"]
+            self.akitude=f"https://en.akinator.com/assets/img/akitudes_670x1096/{goback['akitude']}"
             return goback
         except:
             raise AkinatorError(goback)
 
     def exclude(self):
         self.name=None
         self.description=None
@@ -112,10 +117,11 @@
             exclude=exclude.json()
             self.json["step"]=int(exclude["step"])
             self.json["progression"]=float(exclude["progression"])
             self.step=int(exclude["step"])
             self.progression=float(exclude["progression"])
             self.question=exclude["question"]
             self.question_id=exclude["question_id"]
+            self.akitude=f"https://en.akinator.com/assets/img/akitudes_670x1096/{exclude['akitude']}"
             return exclude
         except:
             raise AkinatorError(exclude)
```

### Comparing `Akinator-python-1.3.0/setup.py` & `Akinator-python-1.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 def load_readme() -> str:
     with open("README.md",encoding="utf-8_sig") as fin:
         return fin.read()
 setup(
     name='Akinator-python',
-    version='1.3.0',
+    version='1.4.0',
     keywords = "akinator",
     long_description=load_readme(),
     long_description_content_type="text/markdown",
     author='taka4602',
     author_email='shun4602@gmail.com',
     url='https://github.com/taka-4602/Akinator-python',
     description='A API wrapper for the AkinatorAPI',
```

