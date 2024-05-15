# Comparing `tmp/cvprocessor-0.5.9.tar.gz` & `tmp/cvprocessor-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvprocessor-0.5.9.tar", last modified: Tue May 14 08:11:25 2024, max compression
+gzip compressed data, was "cvprocessor-0.6.0.tar", last modified: Wed May 15 04:49:41 2024, max compression
```

## Comparing `cvprocessor-0.5.9.tar` & `cvprocessor-0.6.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 08:11:25.218123 cvprocessor-0.5.9/
--rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.5.9/LICENSE
--rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-14 08:11:25.217465 cvprocessor-0.5.9/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)     1053 2024-05-08 07:27:08.000000 cvprocessor-0.5.9/README.md
--rw-r--r--   0 fernando   (501) staff       (20)      769 2024-05-14 08:10:44.000000 cvprocessor-0.5.9/pyproject.toml
--rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-14 08:11:25.218239 cvprocessor-0.5.9/setup.cfg
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 08:11:25.200479 cvprocessor-0.5.9/src/
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 08:11:25.213076 cvprocessor-0.5.9/src/cvprocessor/
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.5.9/src/cvprocessor/__init__.py
--rw-r--r--   0 fernando   (501) staff       (20)    10569 2024-05-14 06:57:49.000000 cvprocessor-0.5.9/src/cvprocessor/authors.py
--rw-r--r--   0 fernando   (501) staff       (20)      363 2024-05-13 06:25:00.000000 cvprocessor-0.5.9/src/cvprocessor/common.py
--rw-r--r--   0 fernando   (501) staff       (20)     9312 2024-05-14 08:06:44.000000 cvprocessor-0.5.9/src/cvprocessor/cv.py
--rw-r--r--   0 fernando   (501) staff       (20)     5199 2024-05-14 06:09:41.000000 cvprocessor-0.5.9/src/cvprocessor/education.py
--rw-r--r--   0 fernando   (501) staff       (20)     5577 2024-05-14 06:10:28.000000 cvprocessor-0.5.9/src/cvprocessor/experience.py
--rw-r--r--   0 fernando   (501) staff       (20)     3317 2024-05-14 06:24:49.000000 cvprocessor-0.5.9/src/cvprocessor/grants_awards.py
--rw-r--r--   0 fernando   (501) staff       (20)     6731 2024-05-14 06:59:18.000000 cvprocessor-0.5.9/src/cvprocessor/institutes.py
--rw-r--r--   0 fernando   (501) staff       (20)     1547 2024-05-14 04:41:36.000000 cvprocessor-0.5.9/src/cvprocessor/intro.py
--rw-r--r--   0 fernando   (501) staff       (20)     1630 2024-05-14 06:28:31.000000 cvprocessor-0.5.9/src/cvprocessor/memberships.py
--rw-r--r--   0 fernando   (501) staff       (20)     3458 2024-05-14 06:21:07.000000 cvprocessor-0.5.9/src/cvprocessor/news.py
--rw-r--r--   0 fernando   (501) staff       (20)    18348 2024-05-14 08:03:10.000000 cvprocessor-0.5.9/src/cvprocessor/publications.py
--rw-r--r--   0 fernando   (501) staff       (20)     2147 2024-05-14 06:29:12.000000 cvprocessor-0.5.9/src/cvprocessor/references.py
--rw-r--r--   0 fernando   (501) staff       (20)     1656 2024-05-14 08:06:36.000000 cvprocessor-0.5.9/src/cvprocessor/research_interests.py
--rw-r--r--   0 fernando   (501) staff       (20)     2123 2024-05-14 06:27:58.000000 cvprocessor-0.5.9/src/cvprocessor/service.py
--rw-r--r--   0 fernando   (501) staff       (20)     2938 2024-05-14 06:27:29.000000 cvprocessor-0.5.9/src/cvprocessor/skills.py
--rw-r--r--   0 fernando   (501) staff       (20)     6111 2024-05-14 08:10:16.000000 cvprocessor-0.5.9/src/cvprocessor/software.py
--rw-r--r--   0 fernando   (501) staff       (20)     4702 2024-05-14 06:26:31.000000 cvprocessor-0.5.9/src/cvprocessor/supervision.py
--rw-r--r--   0 fernando   (501) staff       (20)     7223 2024-05-14 06:25:31.000000 cvprocessor-0.5.9/src/cvprocessor/teaching.py
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 08:11:25.216785 cvprocessor-0.5.9/src/cvprocessor.egg-info/
--rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-14 08:11:25.000000 cvprocessor-0.5.9/src/cvprocessor.egg-info/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)      771 2024-05-14 08:11:25.000000 cvprocessor-0.5.9/src/cvprocessor.egg-info/SOURCES.txt
--rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-14 08:11:25.000000 cvprocessor-0.5.9/src/cvprocessor.egg-info/dependency_links.txt
--rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-14 08:11:25.000000 cvprocessor-0.5.9/src/cvprocessor.egg-info/requires.txt
--rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-14 08:11:25.000000 cvprocessor-0.5.9/src/cvprocessor.egg-info/top_level.txt
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-15 04:49:41.189552 cvprocessor-0.6.0/
+-rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.6.0/LICENSE
+-rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-15 04:49:41.188759 cvprocessor-0.6.0/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)     1053 2024-05-08 07:27:08.000000 cvprocessor-0.6.0/README.md
+-rw-r--r--   0 fernando   (501) staff       (20)      769 2024-05-15 04:48:58.000000 cvprocessor-0.6.0/pyproject.toml
+-rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-15 04:49:41.189710 cvprocessor-0.6.0/setup.cfg
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-15 04:49:41.163948 cvprocessor-0.6.0/src/
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-15 04:49:41.183695 cvprocessor-0.6.0/src/cvprocessor/
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.6.0/src/cvprocessor/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)    10464 2024-05-15 03:47:26.000000 cvprocessor-0.6.0/src/cvprocessor/authors.py
+-rw-r--r--   0 fernando   (501) staff       (20)      363 2024-05-15 02:16:23.000000 cvprocessor-0.6.0/src/cvprocessor/common.py
+-rw-r--r--   0 fernando   (501) staff       (20)     7888 2024-05-15 04:48:38.000000 cvprocessor-0.6.0/src/cvprocessor/cv.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4882 2024-05-15 03:56:47.000000 cvprocessor-0.6.0/src/cvprocessor/education.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3758 2024-05-15 04:08:11.000000 cvprocessor-0.6.0/src/cvprocessor/experience.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4051 2024-05-15 03:58:18.000000 cvprocessor-0.6.0/src/cvprocessor/grants_awards.py
+-rw-r--r--   0 fernando   (501) staff       (20)     7113 2024-05-15 04:39:45.000000 cvprocessor-0.6.0/src/cvprocessor/institutes.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1943 2024-05-15 04:09:24.000000 cvprocessor-0.6.0/src/cvprocessor/intro.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1921 2024-05-15 04:10:03.000000 cvprocessor-0.6.0/src/cvprocessor/memberships.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4435 2024-05-15 04:11:19.000000 cvprocessor-0.6.0/src/cvprocessor/news.py
+-rw-r--r--   0 fernando   (501) staff       (20)    16102 2024-05-15 04:47:01.000000 cvprocessor-0.6.0/src/cvprocessor/publications.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2697 2024-05-15 04:26:24.000000 cvprocessor-0.6.0/src/cvprocessor/references.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1656 2024-05-15 04:26:39.000000 cvprocessor-0.6.0/src/cvprocessor/research_interests.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2540 2024-05-15 04:27:18.000000 cvprocessor-0.6.0/src/cvprocessor/service.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3316 2024-05-15 04:27:50.000000 cvprocessor-0.6.0/src/cvprocessor/skills.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4916 2024-05-15 04:39:59.000000 cvprocessor-0.6.0/src/cvprocessor/software.py
+-rw-r--r--   0 fernando   (501) staff       (20)     5247 2024-05-15 04:39:23.000000 cvprocessor-0.6.0/src/cvprocessor/supervision.py
+-rw-r--r--   0 fernando   (501) staff       (20)     5270 2024-05-15 02:19:52.000000 cvprocessor-0.6.0/src/cvprocessor/teaching.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3482 2024-05-15 02:26:14.000000 cvprocessor-0.6.0/src/cvprocessor/year_data.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-15 04:49:41.187940 cvprocessor-0.6.0/src/cvprocessor.egg-info/
+-rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-15 04:49:41.000000 cvprocessor-0.6.0/src/cvprocessor.egg-info/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)      800 2024-05-15 04:49:41.000000 cvprocessor-0.6.0/src/cvprocessor.egg-info/SOURCES.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-15 04:49:41.000000 cvprocessor-0.6.0/src/cvprocessor.egg-info/dependency_links.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-15 04:49:41.000000 cvprocessor-0.6.0/src/cvprocessor.egg-info/requires.txt
+-rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-15 04:49:41.000000 cvprocessor-0.6.0/src/cvprocessor.egg-info/top_level.txt
```

### Comparing `cvprocessor-0.5.9/LICENSE` & `cvprocessor-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.9/PKG-INFO` & `cvprocessor-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.5.9
+Version: 0.6.0
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.5.9/README.md` & `cvprocessor-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.9/pyproject.toml` & `cvprocessor-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cvprocessor"
-version = "0.5.9"
+version = "0.6.0"
 authors = [
     { name = "F. Fernando Jurado-Lasso", email = "fdo.jurado@gmail.com" },
 ]
 description = "CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cvprocessor-0.5.9/src/cvprocessor/authors.py` & `cvprocessor-0.6.0/src/cvprocessor/authors.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,39 +6,69 @@
     Classes:
     AuthorsData: A class to represent an author.
     Authors: A class to represent a list of authors.
 """
 import pandas as pd
 
 
-class ContactInfo:
+class Contact:
     """
     A class to represent the contact information of an author.
     """
 
     def __init__(self):
         self.email = str()
         self.telephone = str()
         self.website = str()
         self.address = str()
         self.location = str()
 
+    def get_email(self):
+        """
+        Returns the email of the author.
+        """
+        return self.email
+
+    def get_telephone(self):
+        """
+        Returns the telephone of the author.
+        """
+        return self.telephone
+
+    def get_website(self):
+        """
+        Returns the website of the author.
+        """
+        return self.website
+
+    def get_address(self):
+        """
+        Returns the address of the author.
+        """
+        return self.address
+
+    def get_location(self):
+        """
+        Returns the location of the author.
+        """
+        return self.location
+
     def load(self, filename):
         """
         Loads the contact information of the author.
         """
         self.email = filename["Email"]
         self.telephone = filename["Telephone"]
         self.website = filename["Website"]
         self.address = filename["Address"]
         self.location = filename["Location"]
 
     def __repr__(self):
         string = (
-            f"ContactInfo("
+            f"Contact("
             f"email={self.email}, "
             f"telephone={self.telephone}, "
             f"website={self.website}, "
             f"address={self.address}, "
             f"location={self.location})"
         )
         return string
@@ -48,39 +78,69 @@
         string += f"Telephone: {self.telephone}\n"
         string += f"Website: {self.website}\n"
         string += f"Address: {self.address}\n"
         string += f"Location: {self.location}\n"
         return string
 
 
-class ResearchInfo:
+class Social:
     """
-    A class to represent the research information of an author.
+    A class to represent the social profiles of an author.
     """
 
     def __init__(self):
         self.linkedin = str()
         self.github = str()
         self.google_scholar = str()
         self.orcid = str()
         self.researchgate = str()
 
+    def get_linkedin(self):
+        """
+        Returns the LinkedIn of the author.
+        """
+        return self.linkedin
+
+    def get_github(self):
+        """
+        Returns the GitHub of the author.
+        """
+        return self.github
+
+    def get_google_scholar(self):
+        """
+        Returns the Google Scholar of the author.
+        """
+        return self.google_scholar
+
+    def get_orcid(self):
+        """
+        Returns the ORCID of the author.
+        """
+        return self.orcid
+
+    def get_researchgate(self):
+        """
+        Returns the ResearchGate of the author.
+        """
+        return self.researchgate
+
     def load(self, filename):
         """
         Loads the research information of the author.
         """
         self.linkedin = filename["LinkedIn"]
         self.github = filename["GitHub"]
         self.google_scholar = filename["Google Scholar"]
         self.orcid = filename["ORCID"]
         self.researchgate = filename["ResearchGate"]
 
     def __repr__(self):
         string = (
-            f"ResearchInfo("
+            f"Social("
             f"linkedin={self.linkedin}, "
             f"github={self.github}, "
             f"google_scholar={self.google_scholar}, "
             f"orcid={self.orcid}, "
             f"researchgate={self.researchgate})"
         )
         return string
@@ -90,234 +150,189 @@
         string += f"GitHub: {self.github}\n"
         string += f"Google Scholar: {self.google_scholar}\n"
         string += f"ORCID: {self.orcid}\n"
         string += f"ResearchGate: {self.researchgate}\n"
         return string
 
 
-class PersonalInfo:
+class Personal:
     """
     A class to represent the personal information of an author.
+
+    Attributes:
+    name (str): The name of the author.
+    lastname (str): The lastname of the author.
+    alias_long (str): The long alias of the author.
+    alias_short (str): The short alias of the author.
+    job_title (str): The job title of the author.
     """
 
     def __init__(self):
         self.name = str()
         self.lastname = str()
         self.alias_long = str()
         self.alias_short = str()
         self.job_title = str()
-        self.fingerprint = str()
-        self.public_key = str()
+
+    def get_name(self):
+        """
+        Returns the name of the author.
+        """
+        return self.name
+
+    def get_lastname(self):
+        """
+        Returns the lastname of the author.
+        """
+        return self.lastname
+
+    def get_alias_long(self):
+        """
+        Returns the long alias of the author.
+        """
+        return self.alias_long
+
+    def get_alias_short(self):
+        """
+        Returns the short alias of the author.
+        """
+        return self.alias_short
+
+    def get_job_title(self):
+        """
+        Returns the job title of the author.
+        """
+        return self.job_title
 
     def load(self, filename):
         """
         Loads the personal information of the author.
         """
         self.name = filename["Name"]
         self.lastname = filename["Lastname"]
         self.alias_long = filename["Alias Long"]
         self.alias_short = filename["Alias Short"]
         self.job_title = filename["Job Title"]
-        self.fingerprint = filename["Fingerprint"]
-        self.public_key = filename["Public Key"]
 
     def __repr__(self):
         string = (
-            f"AuthorPersonalInfo("
+            f"Personal("
             f"name={self.name}, "
             f"lastname={self.lastname}, "
             f"alias_long={self.alias_long}, "
             f"alias_short={self.alias_short}, "
-            f"job_title={self.job_title}, "
-            f"fingerprint={self.fingerprint}, "
-            f"public_key={self.public_key})"
+            f"job_title={self.job_title})"
         )
         return string
 
-    def __str__(self):
-        string = f"Name: {self.name}\n"
-        string += f"Lastname: {self.lastname}\n"
-        string += f"Alias Long: {self.alias_long}\n"
-        string += f"Alias Short: {self.alias_short}\n"
-        string += f"Job Title: {self.job_title}\n"
-        string += f"Fingerprint: {self.fingerprint}\n"
-        string += f"Public Key: {self.public_key}\n"
-        return string
-
 
-class AuthorsData:
+class Security:
     """
-    A class to represent an author.
+    A class to represent the security details of an author.
 
     Attributes:
-    id (int): The ID of the author.
-    affiliations (list): The affiliations of the author.
-    personal_info (PersonalInfo): The personal information of the author.
-    contact_info (ContactInfo): The contact information of the author.
-    research_info (ResearchInfo): The research information of the author.
-
-    Methods:
-    load(filename): Loads the author data from the file.
-    __str__(): Returns a string representation of the author.
-    __repr__(): Returns a string representation of the author.
+    fingerprint (str): The fingerprint of the author.
+    public_key (str): The public key of the author.
     """
 
     def __init__(self):
-        self.id = int()
-        self.affiliations = []
-        self.personal_info = PersonalInfo()
-        self.contact_info = ContactInfo()
-        self.research_info = ResearchInfo()
-
-    def get_id(self):
-        """
-        Returns the ID of the author.
-        """
-        return self.id
-
-    def get_affiliations(self):
-        """
-        Returns the affiliations of the author.
-        """
-        return self.affiliations
-
-    def get_name(self):
-        """
-        Returns the name of the author.
-        """
-        return self.personal_info.name
-
-    def get_lastname(self):
-        """
-        Returns the lastname of the author.
-        """
-        return self.personal_info.lastname
-
-    def get_alias_long(self):
-        """
-        Returns the long alias of the author.
-        """
-        return self.personal_info.alias_long
-
-    def get_alias_short(self):
-        """
-        Returns the short alias of the author.
-        """
-        return self.personal_info.alias_short
-
-    def get_job_title(self):
-        """
-        Returns the job title of the author.
-        """
-        return self.personal_info.job_title
+        self.fingerprint = str()
+        self.public_key = str()
 
     def get_fingerprint(self):
         """
         Returns the fingerprint of the author.
         """
-        return self.personal_info.fingerprint
+        return self.fingerprint
 
     def get_public_key(self):
         """
         Returns the public key of the author.
         """
-        return self.personal_info.public_key
+        return self.public_key
 
-    def get_email(self):
-        """
-        Returns the email of the author.
-        """
-        return self.contact_info.email
-
-    def get_telephone(self):
+    def load(self, filename):
         """
-        Returns the telephone of the author.
+        Loads the security details of the author.
         """
-        return self.contact_info.telephone
+        self.fingerprint = filename["Fingerprint"]
+        self.public_key = filename["Public Key"]
 
-    def get_website(self):
-        """
-        Returns the website of the author.
-        """
-        return self.contact_info.website
+    def __repr__(self):
+        string = (
+            f"Security("
+            f"fingerprint={self.fingerprint}, "
+            f"public_key={self.public_key})"
+        )
+        return string
 
-    def get_address(self):
-        """
-        Returns the address of the author.
-        """
-        return self.contact_info.address
 
-    def get_location(self):
-        """
-        Returns the location of the author.
-        """
-        return self.contact_info.location
+class AuthorsData:
+    """
+    A class to represent an author.
 
-    def get_linkedin(self):
-        """
-        Returns the LinkedIn of the author.
-        """
-        return self.research_info.linkedin
+    Attributes:
+    id (int): The ID of the author.
+    affiliations (list): The affiliations of the author.
+    personal_info (Personal): The personal information of the author.
+    contact_info (Contact): The contact information of the author.
+    research_info (Social): The research information of the author.
 
-    def get_github(self):
-        """
-        Returns the GitHub of the author.
-        """
-        return self.research_info.github
+    Methods:
+    load(filename): Loads the author data from the file.
+    __str__(): Returns a string representation of the author.
+    __repr__(): Returns a string representation of the author.
+    """
 
-    def get_google_scholar(self):
-        """
-        Returns the Google Scholar of the author.
-        """
-        return self.research_info.google_scholar
+    def __init__(self):
+        self.id = int()
+        self.affiliation_ids = []
+        self.personal = Personal()
+        self.contact = Contact()
+        self.social = Social()
+        self.security = Security()
 
-    def get_orcid(self):
+    def get_id(self):
         """
-        Returns the ORCID of the author.
+        Returns the ID of the author.
         """
-        return self.research_info.orcid
+        return self.id
 
-    def get_researchgate(self):
+    def get_affiliation_ids(self):
         """
-        Returns the ResearchGate of the author.
+        Returns the affiliations of the author.
         """
-        return self.research_info.researchgate
+        return self.affiliation_ids
 
     def load(self, filename):
         """
         Loads the author data from the file.
         """
         self.id = filename["id"]
         if isinstance(filename["Affiliations"], str) and\
                 ("," in filename["Affiliations"] or ";" in filename["Affiliations"]):
             affiliations = filename["Affiliations"].split(",")
             for affiliation in affiliations:
-                self.affiliations.append(int(affiliation))
+                self.affiliation_ids.append(int(affiliation))
         else:
-            self.affiliations.append(int(filename["Affiliations"]))
-        self.personal_info.load(filename)
-        self.contact_info.load(filename)
-        self.research_info.load(filename)
-
-    def __str__(self):
-        string = f"id: {self.id}\n"
-        string += f"Affiliation: {self.affiliations}\n"
-        string += str(self.personal_info)
-        string += str(self.contact_info)
-        string += str(self.research_info)
-        return string
+            self.affiliation_ids.append(int(filename["Affiliations"]))
+        self.personal.load(filename)
+        self.contact.load(filename)
+        self.social.load(filename)
+        self.security.load(filename)
 
     def __repr__(self):
         string = (
             f"Author("
             f"id={self.id}, "
-            f"affiliation={repr(self.affiliations)}, "
-            f"personal_info={repr(self.personal_info)}, "
-            f"contact_info={repr(self.contact_info)}, "
-            f"research_info={repr(self.research_info)})"
+            f"affiliation={repr(self.affiliation_ids)}, "
+            f"personal={repr(self.personal)}, "
+            f"contact={repr(self.contact)}, "
+            f"social={repr(self.social)}, "
+            f"security={repr(self.security)})"
         )
         return string
 
 
 class Authors:
     """
     A class to represent a list of authors.
@@ -343,16 +358,17 @@
             author_id = int(author_id)
         if affiliation_id is None:
             for author in self.authors:
                 if author.get_id() == author_id:
                     return author
             return None
         for author in self.authors:
-            if author.get_id() == author_id and affiliation_id in author.get_affiliations():
+            if author.get_id() == author_id and affiliation_id in author.get_affiliation_ids():
                 return author
+        return None
 
     def load(self, filename):
         """
         Loads the authors from the file.
         """
         authors_df = pd.read_excel(filename, sheet_name="Authors")
         for _, row in authors_df.iterrows():
@@ -367,7 +383,10 @@
 
     def __repr__(self):
         string = (
             f"Authors("
             f"authors={repr(self.authors)})"
         )
         return string
+
+    def __iter__(self):
+        return iter(self.authors)
```

### Comparing `cvprocessor-0.5.9/src/cvprocessor/cv.py` & `cvprocessor-0.6.0/src/cvprocessor/cv.py`

 * *Files 16% similar despite different names*

```diff
@@ -135,136 +135,100 @@
     The CV class is used to create a CV object that stores all the information from the CV file.
 
     :param filename: The filename of the CV file.
     :type filename: str
     """
 
     def __init__(self, filename):
-        self.professional_info = ProfessionalInfo()
-        self.personal_info = PersonalInfo()
-        self.academic_info = AcademicInfo()
+        self.professional = ProfessionalInfo()
+        self.personal = PersonalInfo()
+        self.academic = AcademicInfo()
         self.software = Software()
         self.news = News()
         self._load_cv(filename)
 
-    def get_author(self, author_id):
+    def get_publications_apa_citation(self, publication_title):
         """
-        The get_author method is used to get the author by the given author ID.
+        The get_publications_apa_citation method is used to get the APA citation of the publication.
 
-        :param author_id: The author ID.
-        :type author_id: int
+        :param publication_title: The title of the publication.
+        :type publication_title: str
         """
-        return self.personal_info.authors.get_author(author_id)
-
-    def get_institute(self, institute_id):
-        """
-        The get_institute method is used to get the institute by the given institute ID.
-
-        :param institute_id: The institute ID.
-        :type institute_id: int
-        """
-        return self.academic_info.institutes.get_institute(institute_id)
-
-    def get_software(self, software_id):
-        """
-        The get_software method is used to get the software by the given software ID.
-
-        :param software_id: The software ID.
-        :type software_id: int
-        """
-        return self.software.get_software(software_id)
-
-    def get_publications_count(self):
-        """
-        The get_publications_count method is used to get the number of publications.
-        """
-        return self.academic_info.publications.get_publications_count()
-
-    def get_publications_unique_sources(self):
-        """
-        The get_publications_unique_sources method is used to get the unique sources of the publications.
-        """
-        return self.academic_info.publications.get_unique_sources()
-
-    def get_publications_document_types_ordered(self):
-        """
-        The get_publications_document_types_ordered method is used to get the document types of the publications in order.
-        """
-        return self.academic_info.publications.get_document_types_ordered()
-
-    def get_publications_num_publications_by_document_type(self, document_type):
-        """
-        The get_publications_num_publications_by_document_type method is used to get the number of publications by the given document type.
-
-        :param document_type: The document type.
-        :type document_type: str
-        """
-        return self.academic_info.publications.get_num_publications_by_document_type(document_type)
-
-    def get_publications_num_publications_by_author(self, author_id):
-        """
-        The get_publications_num_publications_by_author method is used to get the number of publications by the given author.
-
-        :param author_id: The author ID.
-        :type author_id: int
-        """
-        return self.academic_info.publications.get_num_publications_by_author(author_id)
+        pub = self.academic.publications.get_publication_by_title(
+            publication_title)
+        if pub is None:
+            return None
+        apa = pub.get_apa_citation()
+        authors_ids_affiliations_ids = pub.get_auth_id_aff_id()
+        authors_ids = []
+        for author_id in authors_ids_affiliations_ids:
+            authors_ids.append(author_id.get_author_id())
+        authors_alias_short = []
+        for author_id in authors_ids:
+            author = self.personal.authors.get_author(author_id)
+            if author is not None:
+                authors_alias_short.append(author.get_alias_short())
+        if len(authors_alias_short) > 1:
+            authors_alias_short[-1] = "& " + authors_alias_short[-1]
+        authors_alias_short = ", ".join(authors_alias_short)
+        apa = authors_alias_short + apa
+        return apa
 
     def get_research_interests(self):
         """
-        The get_reserach_interests method is used to get the research interests.
+        The get_research_interests method is used to get the research interests.
         """
-        return self.academic_info.research_interests.get_interests()
+        return self.academic.research_interests.get_interests()
 
     def get_research_keywords(self):
         """
         The get_research_keywords method is used to get the research keywords.
         """
-        return self.academic_info.research_interests.get_keywords()
+        return self.academic.research_interests.get_keywords()
 
     def _load_cv(self, filename):
         """
         The _load_cv method is used to load the CV file.
 
         :param filename: The filename of the CV file.
         :type filename: str
         """
-        self.academic_info.education.load(filename)
-        self.academic_info.institutes.load(filename)
+        self.academic.education.load(filename)
+        self.academic.institutes.load(filename)
         self.software.load(filename)
-        self.personal_info.intro.load(filename)
-        self.personal_info.authors.load(filename)
+        self.personal.intro.load(filename)
+        self.personal.authors.load(filename)
         self.news.load(filename)
-        self.academic_info.publications.load(filename)
-        self.academic_info.research_interests.load(filename)
-        self.academic_info.grants_awards.load(filename)
-        self.academic_info.teaching.load(filename)
-        self.academic_info.supervision.load(filename)
-        self.professional_info.experience.load(filename)
-        self.professional_info.skills.load(filename)
-        self.professional_info.service.load(filename)
-        self.professional_info.memberships.load(filename)
-        self.personal_info.references.load(filename)
+        self.academic.publications.load(filename)
+        self.academic.research_interests.load(filename)
+        self.academic.grants_awards.load(filename)
+        self.academic.teaching.load(filename)
+        self.academic.supervision.load(filename)
+        self.professional.experience.load(filename)
+        self.professional.skills.load(filename)
+        self.professional.service.load(filename)
+        self.professional.memberships.load(filename)
+        self.personal.references.load(filename)
 
     def __str__(self):
-        string = f"Academic Info: {self.academic_info}\n"
-        string += f"Personal Info: {self.personal_info}\n"
-        string += f"Professional Info: {self.professional_info}\n"
+        string = f"Academic Info: {self.academic}\n"
+        string += f"Personal Info: {self.personal}\n"
+        string += f"Professional Info: {self.professional}\n"
         string += f"Software: {self.software}\n"
         string += f"News: {self.news}\n"
         return string
 
     def __repr__(self):
         string = (
             f"CV("
-            f"academic_info={repr(self.academic_info)}, "
-            f"personal_info={repr(self.personal_info)}, "
-            f"professional_info={repr(self.professional_info)}, "
+            f"academic={repr(self.academic)}, "
+            f"personal={repr(self.personal)}, "
+            f"professional={repr(self.professional)}, "
             f"software={repr(self.software)}, "
             f"news={repr(self.news)})\n")
         return string
 
 
 if __name__ == "__main__":
     cv = CV("cv.xlsx")
-    print(str(cv.personal_info.references))
+    print(str(cv.personal.references))
     sys.exit(0)
```

### Comparing `cvprocessor-0.5.9/src/cvprocessor/education.py` & `cvprocessor-0.6.0/src/cvprocessor/education.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 This module contains the classes to represent the education data of an author.
 """
 import pandas as pd
+from cvprocessor import year_data as yd
 
 
 class ThesisInfo:
     """
     A class to represent the thesis information of an author.
 
     Attributes:
@@ -19,14 +20,32 @@
     """
 
     def __init__(self):
         self.thesis = None
         self.thesis_link = None
         self.advisor = None
 
+    def get_thesis(self):
+        """
+        Get the thesis.
+        """
+        return self.thesis
+
+    def get_thesis_link(self):
+        """
+        Get the thesis link.
+        """
+        return self.thesis_link
+
+    def get_advisor(self):
+        """
+        Get the advisor.
+        """
+        return self.advisor
+
     def load(self, filename):
         """
         Load the thesis information.
         """
         self.thesis = filename["Thesis"]
         self.thesis_link = filename["Thesis link"]
         self.advisor = filename["Advisor"]
@@ -43,88 +62,71 @@
             f"thesis={self.thesis}, "
             f"thesis_link={self.thesis_link}, "
             f"advisor={self.advisor})"
         )
         return string
 
 
-class EducationPeriod:
+class EducationData:
     """
-    A class to represent the education period of an author.
-
-    Attributes:
-    year: The year.
-    start_year: The start year.
-    end_year: The end year.
-
-    Methods:
-    __str__: Returns the string representation of the education period.
-    __repr__: Returns the string representation of the education period.
+    A class to represent the education data of an author.
     """
 
     def __init__(self):
-        self.start_year = None
-        self.end_year = None
-        self.year = None
+        self.degree = str()
+        self.award = str()
+        self.institution = str()
+        self.education_period = []
+        self.thesis_info = ThesisInfo()
 
-    def load(self, filename):
+    def get_degree(self):
         """
-        Load the education period.
+        Get the degree.
         """
-        years = filename["Year"]
-        years = years.split(";")
-        years = list(filter(None, years))
-        self.year = years[0]
-        start_year = years[0].split("-")[0].strip()
-        end_year = years[-1].split("-")[-1].strip()
-        if len(start_year.split()) == 2:
-            start_year = '1 '+start_year
-        if len(end_year.split()) == 2:
-            end_year = "1 "+end_year
-        self.start_year = pd.to_datetime(
-            start_year, format="%d %b %Y")
-        self.end_year = pd.to_datetime(
-            end_year, format="%d %b %Y")
+        return self.degree
 
-    def __str__(self):
-        string = f"Year: {self.year}\n"
-        string += f"Start year: {self.start_year}\n"
-        string += f"End year: {self.end_year}\n"
-        return string
+    def get_institution(self):
+        """
+        Get the institution.
+        """
+        return self.institution
 
-    def __repr__(self):
-        string = (
-            f"EducationPeriod("
-            f"year={self.year}, "
-            f"start_year={self.start_year}, "
-            f"end_year={self.end_year})"
-        )
-        return string
+    def get_award(self):
+        """
+        Get the award.
+        """
+        return self.award
 
+    def get_start_year(self):
+        """
+        Get the start year of this experience.
+        """
+        return yd.get_start_year(self.education_period)
 
-class EducationData:
-    """
-    A class to represent the education data of an author.
-    """
+    def get_end_year(self):
+        """
+        Get the end year of this experience.
+        """
+        return yd.get_end_year(self.education_period)
 
-    def __init__(self):
-        self.degree = str()
-        self.award = str()
-        self.institution = str()
-        self.education_period = EducationPeriod()
-        self.thesis_info = ThesisInfo()
+    def process_year_data(self, filename):
+        """
+        Process the year data.
+        """
+        self.education_period = yd.process_year_data(
+            filename, self.education_period)
 
     def load(self, filename):
         """
         Load the education data from the filename.
         """
         self.degree = filename["Degree"]
         self.award = filename["Award"]
         self.institution = filename["Institution"]
-        self.education_period.load(filename)
+        self.process_year_data(filename)
         self.thesis_info.load(filename)
 
     def __str__(self):
         string = f"Degree: {self.degree}\n"
         string += f"Award: {self.award}\n"
         string += f"Institution: {self.institution}\n"
         string += str(self.education_period)
@@ -167,18 +169,21 @@
         """
         education_df = pd.read_excel(filename, sheet_name="Education")
         for _, row in education_df.iterrows():
             self.educations.append(EducationData())
             self.educations[-1].load(row)
         # sort the education data by end year
         self.educations = sorted(
-            self.educations, key=lambda x: x.education_period.end_year, reverse=True)
+            self.educations, key=lambda x: x.get_end_year(), reverse=True)
 
     def __str__(self) -> str:
         string = ""
         for education in self.educations:
             string += str(education) + "\n"
         return string
 
     def __repr__(self) -> str:
         string = f"Education(educations={repr(self.educations)})"
         return string
+
+    def __iter__(self):
+        return iter(self.educations)
```

### Comparing `cvprocessor-0.5.9/src/cvprocessor/grants_awards.py` & `cvprocessor-0.6.0/src/cvprocessor/grants_awards.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,14 +23,44 @@
     def __init__(self):
         self.year: pd.Timestamp = pd.Timestamp("NaT")
         self.description = str()
         self.institution = str()
         self.country = str()
         self.value = str()
 
+    def get_year(self):
+        """
+        Get the year of the grant or award.
+        """
+        return self.year
+
+    def get_description(self):
+        """
+        Get the description of the grant or award.
+        """
+        return self.description
+
+    def get_institution(self):
+        """
+        Get the institution that awarded the grant or award.
+        """
+        return self.institution
+
+    def get_country(self):
+        """
+        Get the country where the grant or award was awarded.
+        """
+        return self.country
+
+    def get_value(self):
+        """
+        Get the value of the grant or award.
+        """
+        return self.value
+
     def load(self, filename):
         """
         Load the grants and awards data from the given file.
         """
         year = filename["Year"]
         self.year = pd.to_datetime(year, format="%Y").year
         self.description = filename["Description"]
@@ -98,7 +128,10 @@
         for grants_award in self.grants_awards:
             string += str(grants_award) + "\n"
         return string
 
     def __repr__(self) -> str:
         string = f"GrantsAwards(grants_awards={repr(list(self.grants_awards))})"
         return string
+
+    def __iter__(self):
+        return iter(self.grants_awards)
```

### Comparing `cvprocessor-0.5.9/src/cvprocessor/institutes.py` & `cvprocessor-0.6.0/src/cvprocessor/institutes.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,66 +1,140 @@
 """
 This module contains the classes to handle the data of the institutes.
 """
 import pandas as pd
 
 
-class InstituteInfo:
+class Personal:
     """
-    A class to represent the information of an institute.
+    A class to represent the personal information of an institute.
+
+    Attributes:
+    name (str): The name of the institute.
+    name_abbr (str): The abbreviation of the institute.
     """
 
     def __init__(self):
-        self.id = None
         self.name = None
-        self.name_abbr = None
-        self.department = None
-        self.department_abbr = None
+        self.abbrv = None
+
+    def get_name(self):
+        """
+        Get the name of the institute.
+        """
+        return self.name
+
+    def get_abbrv(self):
+        """
+        Get the abbreviation of the institute.
+        """
+        return self.abbrv
 
     def load(self, filename):
         """
         Load the institute information.
         """
-        self.id = filename["id"]
         self.name = filename["Name"]
-        self.name_abbr = filename["Name Abbreviation"]
-        self.department = filename["Department"]
-        self.department_abbr = filename["Department Abbreviation"]
+        self.abbrv = filename["Name Abbreviation"]
 
     def __str__(self):
-        string = f"Institute ID: {self.id}\n"
-        string += f"Institute Name: {self.name}\n"
-        string += f"Institute Name Abbreviation: {self.name_abbr}\n"
-        string += f"Institute Department: {self.department}\n"
-        string += f"Institute Department Abbreviation: {self.department_abbr}\n"
+        string = f"Institute Name: {self.name}\n"
+        string += f"Institute Abbreviation: {self.abbrv}\n"
         return string
 
     def __repr__(self):
         string = (
-            f"InstituteInfo("
-            f"id={self.id}, "
+            f"Personal("
             f"name={self.name}, "
-            f"name_abbr={self.name_abbr}, "
-            f"department={self.department}, "
-            f"department_abbr={self.department_abbr})"
+            f"name_abbr={self.abbrv})"
+        )
+        return string
+
+
+class Department:
+    """
+    A class to represent the department of an institute.
+
+    Attributes:
+    department (str): The name of the department.
+    department_abbr (str): The abbreviation of the department.
+    """
+
+    def __init__(self):
+        self.name = None
+        self.abbrv = None
+
+    def get_name(self):
+        """
+        Get the name of the department.
+        """
+        return self.name
+
+    def get_abbrv(self):
+        """
+        Get the abbreviation of the department.
+        """
+        return self.abbrv
+
+    def load(self, filename):
+        """
+        Load the institute information.
+        """
+        self.name = filename["Department"]
+        self.abbrv = filename["Department Abbreviation"]
+
+    def __str__(self):
+        string = f"Institute Department: {self.name}\n"
+        string += f"Institute Department Abbreviation: {self.abbrv}\n"
+        return string
+
+    def __repr__(self):
+        string = (
+            f"Department("
+            f"department={self.name}, "
+            f"department_abbr={self.abbrv})"
         )
         return string
 
 
-class InstituteLocation:
+class Location:
     """
     A class to represent the location of an institute.
     """
 
     def __init__(self):
         self.address = str()
         self.city = str()
         self.country = str()
         self.coordinates = tuple()
 
+    def get_address(self):
+        """
+        Get the address of the institute.
+        """
+        return self.address
+
+    def get_city(self):
+        """
+        Get the city of the institute.
+        """
+        return self.city
+
+    def get_country(self):
+        """
+        Get the country of the institute.
+        """
+        return self.country
+
+    def get_coordinates(self):
+        """
+        Get the coordinates of the institute.
+        """
+        return self.coordinates
+
     def convert_coordinates(self, lalng):
         """
         Convert the latitude and longitude coordinates to a float value.
         """
         lalng = lalng.replace("°", "").strip()
         if "S" in lalng or "W" in lalng:
             lalng = lalng.replace("S", "").replace("W", "")
@@ -95,111 +169,63 @@
         string += f"Institute City: {self.city}\n"
         string += f"Institute Country: {self.country}\n"
         string += f"Institute Coordinates: {self.coordinates}\n"
         return string
 
     def __repr__(self):
         string = (
-            f"InstituteLocation("
+            f"Location("
             f"address={self.address}, "
             f"city={self.city}, "
             f"country={self.country}, "
             f"coordinates={self.coordinates})"
         )
         return string
 
 
 class InstituteData:
     """
     A class to represent the data of an institute.
     """
 
     def __init__(self):
-        self.info = InstituteInfo()
-        self.location = InstituteLocation()
-        self.url = None
+        self.id = str()
+        self.personal = Personal()
+        self.department = Department()
+        self.location = Location()
+        self.url = str()
 
     def get_id(self):
         """
         Get the ID of the institute.
         """
-        return self.info.id
-
-    def get_name(self):
-        """
-        Get the name of the institute.
-        """
-        return self.info.name
-
-    def get_name_abbr(self):
-        """
-        Get the name abbreviation of the institute.
-        """
-        return self.info.name_abbr
-
-    def get_department(self):
-        """
-        Get the department of the institute.
-        """
-        return self.info.department
-
-    def get_department_abbr(self):
-        """
-        Get the department abbreviation of the institute.
-        """
-        return self.info.department_abbr
-
-    def get_address(self):
-        """
-        Get the address of the institute.
-        """
-        return self.location.address
-
-    def get_city(self):
-        """
-        Get the city of the institute.
-        """
-        return self.location.city
-
-    def get_country(self):
-        """
-        Get the country of the institute.
-        """
-        return self.location.country
-
-    def get_coordinates(self):
-        """
-        Get the coordinates of the institute.
-        """
-        return self.location.coordinates
+        return self.id
 
     def get_url(self):
         """
         Get the URL of the institute.
         """
         return self.url
 
     def load(self, pd_dataframe):
         """
         Load the data from a pandas dataframe.
         """
-        self.info.load(pd_dataframe)
+        self.id = pd_dataframe["id"]
+        self.personal.load(pd_dataframe)
+        self.department.load(pd_dataframe)
         self.location.load(pd_dataframe)
         self.url = pd_dataframe["URL"]
 
-    def __str__(self):
-        string = str(self.info)
-        string += str(self.location)
-        string += f"url: \n{self.url}\n"
-        return string
-
     def __repr__(self):
         string = (
             f"InstituteData("
-            f"info={repr(self.info)}, "
+            f"id={self.id}, "
+            f"personal={repr(self.personal)}, "
+            f"department={repr(self.department)}, "
             f"location={repr(self.location)}, "
             f"url={self.url})"
         )
         return string
 
 
 class Institutes:
@@ -243,7 +269,10 @@
         for institute in self.institutes:
             string += str(institute) + "\n"
         return string
 
     def __repr__(self):
         string = f"Institutes(Institute={repr(self.institutes)})"
         return string
+
+    def __iter__(self):
+        return iter(self.institutes)
```

### Comparing `cvprocessor-0.5.9/src/cvprocessor/intro.py` & `cvprocessor-0.6.0/src/cvprocessor/intro.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,17 +16,35 @@
     Methods:
     __init__(filename): Initializes the Intro class by loading the introduction from the given file.
     __str__(): Returns a string representation of the Intro class.
     __repr__(): Returns a string representation of the Intro class.
     """
 
     def __init__(self):
-        self.short_summary = None
-        self.long_summary = None
-        self.tagline = None
+        self.short_summary = str()
+        self.long_summary = str()
+        self.tagline = str()
+
+    def get_short_summary(self):
+        """
+        Get the short summary of the CV file.
+        """
+        return self.short_summary
+
+    def get_long_summary(self):
+        """
+        Get the long summary of the CV file.
+        """
+        return self.long_summary
+
+    def get_tagline(self):
+        """
+        Get the tagline of the CV file.
+        """
+        return self.tagline
 
     def load(self, filename):
         """
         Load the introduction from the given file.
         """
         intro = pd.read_excel(filename, sheet_name="Intro")
         self.short_summary = intro["Short summary"].values[0]
```

### Comparing `cvprocessor-0.5.9/src/cvprocessor/memberships.py` & `cvprocessor-0.6.0/src/cvprocessor/memberships.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,26 @@
     membership (str): The membership.
     """
 
     def __init__(self):
         self.year: pd.Timestamp = pd.Timestamp("NaT")
         self.membership = str()
 
+    def get_year(self):
+        """
+        Get the year of the membership.
+        """
+        return self.year
+
+    def get_membership(self):
+        """
+        Get the membership.
+        """
+        return self.membership
+
     def load(self, filename):
         """
         Load the membership data.
         """
         self.year = filename["Year"]
         self.membership = filename["Membership"]
 
@@ -56,7 +68,10 @@
         string = ""
         for membership in self.memberships:
             string += str(membership) + "\n"
         return string
 
     def __repr__(self):
         return f"Memberships(memberships={repr(list(map(repr, self.memberships)))})\n"
+
+    def __iter__(self):
+        return iter(self.memberships)
```

### Comparing `cvprocessor-0.5.9/src/cvprocessor/publications.py` & `cvprocessor-0.6.0/src/cvprocessor/publications.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,260 +3,306 @@
 """
 import pandas as pd
 
 
 from cvprocessor import common
 
 
-class PublicationBasicInfo:
+class Source:
     """
-    A class to represent the basic information of a publication.
+    A class to represent the source of a publication.
+
+    Attributes:
+    volume (str): The volume of the publication.
+    issue (str): The issue of the publication.
+    artno (str): The article number of the publication.
     """
 
     def __init__(self):
-        self.title = str()
-        self.year: pd.Timestamp = pd.Timestamp("NaT")
+        self.volume = str()
+        self.issue = str()
+        self.artno = str()
         self.source = str()
 
-    def process_year_data(self, year):
+    def get_volume(self):
         """
-        Process the year data.
+        Get the volume of the publication.
         """
-        if len(year.split()) == 1:
-            year = 'Jan ' + year
-        self.year = pd.to_datetime(year, format="%b %Y")
+        return self.volume
 
-    def load(self, filename):
+    def get_issue(self):
         """
-        Load the publication basic information from the file.
+        Get the issue of the publication.
         """
-        self.title = filename["Title"]
-        self.process_year_data(filename["Year"])
-        self.source = filename["Source"]
-
-    def __repr__(self):
-        string = (
-            f"PublicationBasicInfo("
-            f"title={self.title}, "
-            f"year={self.year}, "
-            f"source={self.source})"
-        )
-        return string
+        return self.issue
 
-    def __str__(self):
-        string = f"Title: {self.title}\n"
-        string += f"Year: {self.year}\n"
-        string += f"Source: {self.source}\n"
-        return string
-
-
-class PublicationJournalInfo:
-    """
-    A class to represent the journal information of a publication.
-
-    Attributes:
-    volume (str): The volume of the publication.
-    issue (str): The issue of the publication.
-    artno (str): The article number of the publication.
-    """
+    def get_artno(self):
+        """
+        Get the article number of the publication.
+        """
+        return self.artno
 
-    def __init__(self):
-        self.volume = str()
-        self.issue = str()
-        self.artno = str()
+    def get_source(self):
+        """
+        Get the source of the publication.
+        """
+        return self.source
 
     def load(self, filename):
         """
         Load the publication journal information from the file.
         """
         self.volume = filename["Volume"]
         self.issue = filename["Issue"]
         self.artno = filename["Art. No."]
+        self.source = filename["Source"]
 
     def __repr__(self):
         string = (
-            f"PublicationJournalInfo("
+            f"Source("
             f"volume={self.volume}, "
             f"issue={self.issue}, "
-            f"artno={self.artno})"
+            f"artno={self.artno}, "
+            f"source={self.source})"
         )
         return string
 
-    def __str__(self):
-        string = f"Volume: {self.volume}\n"
-        string += f"Issue: {self.issue}\n"
-        string += f"Art. No.: {self.artno}\n"
-        return string
-
 
-class PublicationPageInfo:
+class Pages:
     """
     A class to represent the page information of a publication.
 
     Attributes:
     page_start (str): The starting page of the publication.
     page_end (str): The ending page of the publication.
     """
 
     def __init__(self):
         self.page_start = str()
         self.page_end = str()
 
+    def get_page_start(self):
+        """
+        Get the starting page of the publication.
+        """
+        return self.page_start
+
+    def get_page_end(self):
+        """
+        Get the ending page of the publication.
+        """
+        return self.page_end
+
     def load(self, filename):
         """
         Load the publication page information from the file.
         """
         self.page_start = filename["Page start"]
         self.page_end = filename["Page end"]
 
     def __repr__(self):
         string = (
-            f"PublicationPageInfo("
+            f"Pages("
             f"page_start={self.page_start}, "
             f"page_end={self.page_end})"
         )
         return string
 
     def __str__(self):
         string = f"Page start: {self.page_start}\n"
         string += f"Page end: {self.page_end}\n"
         return string
 
 
-class PublicationDetails:
+class Details:
     """
     A class to represent the details of a publication.
 
     Attributes:
     basic_info (PublicationBasicInfo): The basic information of the publication.
-    journal_info (PublicationJournalInfo): The journal information of the publication.
-    page_info (PublicationPageInfo): The page information of the publication.
+    journal_info (Source): The journal information of the publication.
+    page_info (Pages): The page information of the publication.
     document_type (str): The document type of the publication.
     """
 
     def __init__(self):
-        self.basic_info = PublicationBasicInfo()
-        self.journal_info = PublicationJournalInfo()
-        self.page_info = PublicationPageInfo()
+        self.title = str()
+        self.year = pd.Timestamp("NaT")
+        self.source = Source()
+        self.pages = Pages()
         self.document_type = str()
+        self.abstract = str()
+        self.keywords = str()
+
+    def get_title(self):
+        """
+        Get the title of the publication.
+        """
+        return self.title
+
+    def get_year(self):
+        """
+        Get the year of the publication.
+        """
+        return self.year
+
+    def get_document_type(self):
+        """
+        Get the document type of the publication.
+        """
+        return self.document_type
+
+    def get_abstract(self):
+        """
+        Get the abstract of the publication.
+        """
+        return self.abstract
+
+    def get_keywords(self):
+        """
+        Get the keywords of the publication.
+        """
+        return self.keywords
 
     def load(self, filename):
         """
         Load the publication details from the file.
         """
-        self.basic_info.load(filename)
-        self.journal_info.load(filename)
-        self.page_info.load(filename)
+        self.title = filename["Title"]
+        self.year = filename["Year"]
+        self.source.load(filename)
+        self.pages.load(filename)
         self.document_type = filename["Document Type"]
+        self.abstract = filename["Abstract"]
+        self.keywords = filename["Keywords"]
 
     def __repr__(self):
         string = (
-            f"PublicationDetails("
-            f"basic_info={self.basic_info}, "
-            f"journal_info={self.journal_info}, "
-            f"page_info={self.page_info})"
+            f"Details("
+            f"title={self.title}, "
+            f"year={self.year}, "
+            f"source={repr(self.source)}, "
+            f"pages={repr(self.pages)}, "
+            f"document_type={self.document_type}, "
+            f"abstract={self.abstract}, "
+            f"keywords={self.keywords})"
         )
         return string
 
-    def __str__(self):
-        string = str(self.basic_info)
-        string += str(self.journal_info)
-        string += str(self.page_info)
-        return string
-
 
-class PublicationResources:
+class Social:
     """
     A class to represent the resources of a publication.
 
     Attributes:
     code (str): The code of the publication.
     slides (str): The slides of the publication.
-    abstract (str): The abstract of the publication.
-    keywords (str): The keywords of the publication.
     doi (str): The DOI of the publication.
     preprint_doi (str): The preprint DOI of the publication.
     """
 
     def __init__(self):
         self.code = str()
         self.slides = str()
-        self.abstract = str()
-        self.keywords = str()
         self.doi = str()
         self.preprint_doi = str()
 
+    def get_code(self):
+        """
+        Get the code of the publication.
+        """
+        return self.code
+
+    def get_slides(self):
+        """
+        Get the slides of the publication.
+        """
+        return self.slides
+
+    def get_doi(self):
+        """
+        Get the DOI of the publication.
+        """
+        return self.doi
+
+    def get_preprint_doi(self):
+        """
+        Get the preprint DOI of the publication.
+        """
+        return self.preprint_doi
+
     def load(self, filename):
         """
         Load the publication resources from the file.
         """
         self.code = filename["Code"]
         self.slides = filename["Slides"]
-        self.abstract = filename["Abstract"]
-        self.keywords = filename["Keywords"]
         self.doi = filename["DOI"]
         self.preprint_doi = filename["Preprint DOI"]
 
     def __repr__(self):
         string = (
-            f"PublicationResources("
+            f"Social("
             f"code={self.code}, "
             f"slides={self.slides}, "
-            f"abstract={self.abstract}, "
-            f"keywords={self.keywords}, "
             f"doi={self.doi}, "
             f"preprint_doi={self.preprint_doi})"
         )
         return string
 
     def __str__(self):
         string = f"Code: {self.code}\n"
         string += f"Slides: {self.slides}\n"
-        string += f"Abstract: {self.abstract}\n"
-        string += f"Keywords: {self.keywords}\n"
         string += f"DOI: {self.doi}\n"
         string += f"Preprint DOI: {self.preprint_doi}\n"
         return string
 
 
-class PublicationRights:
+class Rights:
     """
     A class to represent the rights of a publication.
 
     Attributes:
-    jcr (str): The JCR of the publication.
     license (str): The license of the publication.
     copyright (str): The copyright of the publication.
     """
 
     def __init__(self):
-        self.jcr = str()
         self.license = str()
         self.copyright = str()
 
+    def get_license(self):
+        """
+        Get the license of the publication.
+        """
+        return self.license
+
+    def get_copyright(self):
+        """
+        Get the copyright of the publication.
+        """
+        return self.copyright
+
     def load(self, filename):
         """
         Load the publication rights from the file.
         """
-        self.jcr = filename["JCR"]
         self.license = filename["License"]
         self.copyright = filename["Copyright"]
 
     def __repr__(self):
         string = (
-            f"PublicationRights("
-            f"jcr={self.jcr}, "
+            f"Rights("
             f"license={self.license}, "
             f"copyright={self.copyright})"
         )
         return string
 
     def __str__(self):
-        string = f"JCR: {self.jcr}\n"
-        string += f"License: {self.license}\n"
+        string = f"License: {self.license}\n"
         string += f"Copyright: {self.copyright}"
         return string
 
 
 class AuthorIDAffiliationIDs:
     """
     A class to represent the author ID and affiliation IDs.
@@ -304,142 +350,34 @@
 
 class PublicationsData:
     """
     A class to represent the data of a publication.
 
     Attributes:
     authors_ids (list): The list of author IDs and affiliation IDs.
-    details (PublicationDetails): The details of the publication.
-    resources (PublicationResources): The resources of the publication.
-    rights (PublicationRights): The rights of the publication.
+    details (Details): The details of the publication.
+    resources (Social): The resources of the publication.
+    rights (Rights): The rights of the publication.
 
     Methods:
     load: Load the publication data from the file.
     build_apa_citation: Build the APA citation.
     """
 
     def __init__(self):
-        self.authors_ids = []
-        self.details = PublicationDetails()
-        self.resources = PublicationResources()
-        self.rights = PublicationRights()
-
-    def get_title(self):
-        """
-        Get the title of the publication.
-        """
-        return self.details.basic_info.title
-
-    def get_year(self):
-        """
-        Get the year of the publication.
-        """
-        return self.details.basic_info.year
-
-    def get_source(self):
-        """
-        Get the source of the publication.
-        """
-        return self.details.basic_info.source
-
-    def get_volume(self):
-        """
-        Get the volume of the publication.
-        """
-        return self.details.journal_info.volume
-
-    def get_issue(self):
-        """
-        Get the issue of the publication.
-        """
-        return self.details.journal_info.issue
-
-    def get_artno(self):
-        """
-        Get the article number of the publication.
-        """
-        return self.details.journal_info.artno
-
-    def get_page_start(self):
-        """
-        Get the starting page of the publication.
-        """
-        return self.details.page_info.page_start
-
-    def get_page_end(self):
-        """
-        Get the ending page of the publication.
-        """
-        return self.details.page_info.page_end
+        self.auth_id_aff_id = []
+        self.details = Details()
+        self.social = Social()
+        self.rights = Rights()
 
-    def get_document_type(self):
+    def get_auth_id_aff_id(self):
         """
-        Get the document type of the publication.
-        """
-        return self.details.document_type
-
-    def get_code(self):
-        """
-        Get the code of the publication.
-        """
-        return self.resources.code
-
-    def get_slides(self):
-        """
-        Get the slides of the publication.
+        Get the author IDs and affiliation IDs.
         """
-        return self.resources.slides
-
-    def get_abstract(self):
-        """
-        Get the abstract of the publication.
-        """
-        return self.resources.abstract
-
-    def get_keywords(self):
-        """
-        Get the keywords of the publication.
-        """
-        return self.resources.keywords
-
-    def get_doi(self):
-        """
-        Get the DOI of the publication.
-        """
-        return self.resources.doi
-
-    def get_preprint_doi(self):
-        """
-        Get the preprint DOI of the publication.
-        """
-        return self.resources.preprint_doi
-
-    def get_jcr(self):
-        """
-        Get the JCR of the publication.
-        """
-        return self.rights.jcr
-
-    def get_license(self):
-        """
-        Get the license of the publication.
-        """
-        return self.rights.license
-
-    def get_copyright(self):
-        """
-        Get the copyright of the publication.
-        """
-        return self.rights.copyright
-
-    def get_authors_ids(self):
-        """
-        Get the authors' IDs and affiliation IDs.
-        """
-        return self.authors_ids
+        return self.auth_id_aff_id
 
     def load(self, filename):
         """
         Load the publication data from the file.
         """
         authors_list = filename["Authors"].split(",")
         authors = []
@@ -453,62 +391,58 @@
                 author_id = author
                 author_affiliation = None
             authors.append(AuthorIDAffiliationIDs())
             authors[-1].author_id = int(author_id)
             if author_affiliation is not None:
                 for affiliation in author_affiliation:
                     authors[-1].add_affiliation_id(int(affiliation))
-        self.authors_ids = authors
+        self.auth_id_aff_id = authors
         self.details.load(filename)
-        self.resources.load(filename)
+        self.social.load(filename)
         self.rights.load(filename)
 
-    def build_apa_citation(self):
+    def get_apa_citation(self) -> str:
         """
         Build the APA citation.
         """
         citation = ""
-        authors = [f"{author.author_id}" for author in self.authors_ids]
-        unique_authors = [authors[i] for i in range(
-            len(authors)) if authors[i] not in authors[:i]]
-        citation += ', '.join(unique_authors)
-        if not common.check_nan(self.details.basic_info.year):
-            citation += f" ({self.details.basic_info.year.year}). "
-        if not common.check_nan(self.details.basic_info.title):
-            citation += f"{self.details.basic_info.title}. "
-        if not common.check_nan(self.details.basic_info.source):
-            citation += f"{self.details.basic_info.source}, "
-        if not common.check_nan(self.details.journal_info.volume):
-            citation += f", {int(self.details.journal_info.volume)}"
-        if not common.check_nan(self.details.journal_info.issue):
-            citation += f"({int(self.details.journal_info.issue)})"
-        if not common.check_nan(self.details.journal_info.artno):
-            citation += f"{self.details.journal_info.artno}"
-        if not common.check_nan(self.details.page_info.page_start):
-            citation += f", pp. {int(self.details.page_info.page_start)}"
-        if not common.check_nan(self.details.page_info.page_end):
-            citation += f"-{int(self.details.page_info.page_end)}"
-        if not common.check_nan(self.resources.doi):
-            citation += f", doi: {self.resources.doi}"
+        if not common.check_nan(self.details.get_year()):
+            citation += f"({self.details.get_year().year}). "
+        if not common.check_nan(self.details.get_title()):
+            citation += f"{self.details.get_title()}. "
+        if not common.check_nan(self.details.source.get_source()):
+            citation += f"{self.details.source.get_source()}"
+        if not common.check_nan(self.details.source.get_volume()):
+            citation += f", {int(self.details.source.get_volume())}"
+        if not common.check_nan(self.details.source.get_issue()):
+            citation += f"({int(self.details.source.get_issue())})"
+        if not common.check_nan(self.details.source.get_artno()):
+            citation += f"{self.details.source.get_artno()}"
+        if not common.check_nan(self.details.pages.get_page_start()):
+            citation += f", pp. {int(self.details.pages.get_page_start())}"
+        if not common.check_nan(self.details.pages.get_page_end()):
+            citation += f"-{int(self.details.pages.get_page_end())}"
+        if not common.check_nan(self.social.get_doi()):
+            citation += f", doi: {self.social.get_doi()}"
         citation += "."
         return citation
 
     def __str__(self) -> str:
-        string = f"Authors' IDs and Affiliation IDs: {list(map(str, self.authors_ids))}\n"
+        string = f"Authors' IDs and Affiliation IDs: {list(map(str, self.auth_id_aff_id))}\n"
         string += str(self.details)
-        string += str(self.resources)
+        string += str(self.social)
         string += str(self.rights)
         return string
 
     def __repr__(self) -> str:
         string = (
             f"PublicationsData("
-            f"authors={repr(self.authors_ids)}, "
+            f"authors={repr(self.auth_id_aff_id)}, "
             f"details={repr(self.details)}, "
-            f"resources={repr(self.resources)}, "
+            f"social={repr(self.social)}, "
             f"rights={repr(self.rights)})"
         )
         return string
 
 
 class Publications():
     """
@@ -538,26 +472,35 @@
 
     def get_unique_sources(self):
         """
         Gets the number of unique sources.
         """
         sources = set()
         for publication in self.publications:
-            sources.add(publication.details.basic_info.source)
+            sources.add(publication.details.source.get_source())
         return len(sources)
 
     def get_document_types(self):
         """
         Gets the document types.
         """
         document_types = set()
-        for publication in self.publications:
+        for publication in self:
             document_types.add(publication.details.document_type)
         return document_types
 
+    def get_publication_by_title(self, title):
+        """
+        Get the publication by the title.
+        """
+        for publication in self:
+            if publication.details.get_title() == title:
+                return publication
+        return None
+
     def get_document_types_ordered(self):
         """
         Gets the document types ordered.
         """
         document_types = []
         for publication in self.publications:
             if publication.details.document_type not in document_types:
@@ -576,41 +519,40 @@
 
     def get_num_publications_by_author(self, author_id):
         """
         Gets the number of publications by author.
         """
         count = 0
         for publication in self:
-            for author in publication.get_authors_ids():
-                if author.get_author_id() == author_id:
+            for auth_id_aff_id in publication.get_auth_id_aff_id():
+                if auth_id_aff_id.get_author_id() == author_id:
                     count += 1
-                    break
         return count
 
     def get_publications_year_range(self):
         """
         Gets the year range of the publications.
         """
         years = []
         for publication in self.publications:
-            years.append(publication.details.basic_info.year)
+            years.append(publication.details.get_year().year)
         return min(years), max(years)
 
     def load(self, filename):
         """
         Load the publications data from the file.
         """
         publications_df = pd.read_excel(
             filename, sheet_name="Publications")
         for _, row in publications_df.iterrows():
             self.publications.append(PublicationsData())
             self.publications[-1].load(row)
         self.publications = sorted(
             self.publications, key=lambda x: (
-                x.details.document_type, x.details.basic_info.year), reverse=True
+                x.details.get_year(), x.details.get_title()), reverse=True
         )
 
     def __str__(self):
         string = ""
         for publication in self.publications:
             string += str(publication) + "\n\n"
         return string
```

### Comparing `cvprocessor-0.5.9/src/cvprocessor/references.py` & `cvprocessor-0.6.0/src/cvprocessor/references.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,38 @@
 
     def __init__(self):
         self.name = str()
         self.email = str()
         self.position = str()
         self.institution = str()
 
+    def get_name(self):
+        """
+        Get the name of the reference.
+        """
+        return self.name
+
+    def get_email(self):
+        """
+        Get the email of the reference.
+        """
+        return self.email
+
+    def get_position(self):
+        """
+        Get the position of the reference.
+        """
+        return self.position
+
+    def get_institution(self):
+        """
+        Get the institution of the reference.
+        """
+        return self.institution
+
     def load(self, filename):
         """
         Load the reference data.
         """
         self.name = filename["Name"]
         self.email = filename["Email"]
         self.position = filename["Position"]
@@ -76,7 +100,10 @@
         string = ""
         for reference in self.references:
             string += str(reference) + "\n"
         return string
 
     def __repr__(self):
         return f"References({repr(self.references)})"
+
+    def __iter__(self):
+        return iter(self.references)
```

### Comparing `cvprocessor-0.5.9/src/cvprocessor/research_interests.py` & `cvprocessor-0.6.0/src/cvprocessor/research_interests.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.9/src/cvprocessor/service.py` & `cvprocessor-0.6.0/src/cvprocessor/service.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,14 +15,32 @@
     """
 
     def __init__(self):
         self.type = str()
         self.venue = str()
         self.link = str()
 
+    def get_type(self) -> str:
+        """
+        Get the type of the service.
+        """
+        return self.type
+
+    def get_venue(self) -> str:
+        """
+        Get the venue of the service.
+        """
+        return self.venue
+
+    def get_link(self) -> str:
+        """
+        Get the link to the service.
+        """
+        return self.link
+
     def load(self, filename) -> None:
         """
         Load the service data.
         """
         self.type = filename["Type"]
         self.venue = filename["Venue"]
         self.link = filename["Link"]
@@ -80,7 +98,10 @@
         for service in self.services:
             string += str(service) + "\n"
         return string
 
     def __repr__(self):
         string = f"Services(services={repr(list(self.services))})"
         return string
+
+    def __iter__(self):
+        return iter(self.services)
```

### Comparing `cvprocessor-0.5.9/src/cvprocessor/skills.py` & `cvprocessor-0.6.0/src/cvprocessor/skills.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,32 @@
     """
 
     def __init__(self):
         self.type = None
         self.skill = None
         self.level = None
 
+    def get_type(self):
+        """
+        Get the type of the skill.
+        """
+        return self.type
+
+    def get_skill(self):
+        """
+        Get the skill.
+        """
+        return self.skill
+
+    def get_level(self):
+        """
+        Get the level of the skill.
+        """
+        return self.level
+
     def load(self, filename):
         """
         Load the skill data.
         """
         self.type = filename["Type"]
         self.skill = filename["Skill"]
         self.level = filename["Level"]
@@ -104,7 +122,10 @@
         for skill in self.skills:
             string += str(skill) + "\n"
         return string
 
     def __repr__(self):
         string = f"Skills(skills={repr(list(self.skills))})"
         return string
+
+    def __iter__(self):
+        return iter(self.skills)
```

### Comparing `cvprocessor-0.5.9/src/cvprocessor/software.py` & `cvprocessor-0.6.0/src/cvprocessor/software.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,72 +1,46 @@
 """
 This module contains the Software class and SofwareData class.
 """
 import pandas as pd
 
 
-class SoftwareInfo:
-    """
-    A class to represent the information of a software.
-
-    Attributes:
-    id (int): The ID of the software.
-    name (str): The name of the software.
-    version (str): The version of the software.
-    description (str): The description of the software.
-    """
-
-    def __init__(self):
-        self.id = str()
-        self.name = str()
-        self.version = str()
-        self.description = str()
-
-    def load(self, filename):
-        """
-        Load the software information.
-        """
-        self.id = filename["id"]
-        self.name = filename["Name"]
-        self.version = filename["Version"]
-        self.description = filename["Description"]
-
-    def __str__(self) -> str:
-        string = f"ID: {self.id}\n"
-        string += f"Name: {self.name}\n"
-        string += f"Version: {self.version}\n"
-        string += f"Description: {self.description}\n"
-        return string
-
-    def __repr__(self) -> str:
-        string = (
-            f"SoftwareInfo("
-            f"id={self.id}, "
-            f"name={self.name}, "
-            f"version={self.version}, "
-            f"description={self.description})"
-        )
-        return string
-
-
-class SoftwareResources:
+class Social:
     """
     A class to represent the resources of a software.
 
     Attributes:
     repository (str): The repository link of the software.
     demo (str): The demo link of the software.
     website (str): The website link of the software.
     """
 
     def __init__(self):
         self.repository = str()
         self.demo = str()
         self.website = str()
 
+    def get_repository(self):
+        """
+        Get the repository link of the software.
+        """
+        return self.repository
+
+    def get_demo(self):
+        """
+        Get the demo link of the software.
+        """
+        return self.demo
+
+    def get_website(self):
+        """
+        Get the website link of the software.
+        """
+        return self.website
+
     def load(self, filename):
         """
         Load the software resources.
         """
         self.repository = filename["Repository"]
         self.demo = filename["Demo"]
         self.website = filename["Website"]
@@ -75,80 +49,65 @@
         string = f"Repository: {self.repository}\n"
         string += f"Demo: {self.demo}\n"
         string += f"Website: {self.website}\n"
         return string
 
     def __repr__(self) -> str:
         string = (
-            f"SoftwareResources("
+            f"Social("
             f"repository={self.repository}, "
             f"demo={self.demo}, "
             f"website={self.website})"
         )
         return string
 
 
 class SoftwareData:
     """
     The SoftwareData class is used to store the software data.
 
     Attributes:
-    info (SoftwareInfo): The information of the software.
-    resources (SoftwareResources): The resources of the software.
+    info (Details): The information of the software.
+    resources (Social): The resources of the software.
     summary (str): The summary of the software.
     license (str): The license of the software.
     """
 
     def __init__(self):
-        self.info = SoftwareInfo()
-        self.resources = SoftwareResources()
+        self.id = str()
+        self.name = str()
+        self.version = str()
+        self.description = str()
+        self.social = Social()
         self.summary = str()
         self.license = str()
 
     def get_id(self):
         """
         Get the ID of the software.
         """
-        return self.info.id
+        return self.id
 
     def get_name(self):
         """
         Get the name of the software.
         """
-        return self.info.name
+        return self.name
 
     def get_version(self):
         """
         Get the version of the software.
         """
-        return self.info.version
+        return self.version
 
     def get_description(self):
         """
         Get the description of the software.
         """
-        return self.info.description
-
-    def get_repository(self):
-        """
-        Get the repository link of the software.
-        """
-        return self.resources.repository
-
-    def get_demo(self):
-        """
-        Get the demo link of the software.
-        """
-        return self.resources.demo
-
-    def get_website(self):
-        """
-        Get the website link of the software.
-        """
-        return self.resources.website
+        return self.description
 
     def get_summary(self):
         """
         Get the summary of the software.
         """
         return self.summary
 
@@ -158,31 +117,30 @@
         """
         return self.license
 
     def load(self, filename) -> None:
         """
         Load the software data from a file.
         """
-        self.info.load(filename)
-        self.resources.load(filename)
+        self.id = filename["id"]
+        self.name = filename["Name"]
+        self.version = filename["Version"]
+        self.description = filename["Description"]
+        self.social.load(filename)
         self.summary = filename["Summary"]
         self.license = filename["License"]
 
-    def __str__(self) -> str:
-        string = str(self.info)
-        string += str(self.resources)
-        string += f"Summary: {self.summary}\n"
-        string += f"License: {self.license}\n\n"
-        return string
-
     def __repr__(self) -> str:
         string = (
             f"SoftwareData("
-            f"info={repr(self.info)}, "
-            f"resources={repr(self.resources)}, "
+            f"id={self.id}, "
+            f"name={self.name}, "
+            f"version={self.version}, "
+            f"description={self.description}, "
+            f"social={repr(self.social)}, "
             f"summary={self.summary}, "
             f"license={self.license})"
         )
         return string
 
 
 class Software:
```

### Comparing `cvprocessor-0.5.9/src/cvprocessor/supervision.py` & `cvprocessor-0.6.0/src/cvprocessor/supervision.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,103 +1,149 @@
 """
 This module contains the classes and methods to process the supervision data from the CV.
 """
 import pandas as pd
 
 
-class SupervisionInfo:
+class AcademicDetails:
     """
-    A class to represent the information of a supervision.
+    The AcademicDetails class is used to store the academic details.
 
     Attributes:
-    students (list): The students of the supervision.
-    year (int): The year of the supervision.
-    title (str): The title of the supervision.
-    program (str): The program of the supervision.
-    type (str): The type of the supervision.
+    year (str): The year.
+    title (str): The title.
+    program (str): The program.
+    type (str): The type.
     """
 
     def __init__(self):
-        self.students = str()
         self.year = str()
         self.title = str()
         self.program = str()
         self.type = str()
 
+    def get_year(self):
+        """
+        Get the year.
+        """
+        return self.year
+
+    def get_title(self):
+        """
+        Get the title.
+        """
+        return self.title
+
+    def get_program(self):
+        """
+        Get the program.
+        """
+        return self.program
+
+    def get_type(self):
+        """
+        Get the type.
+        """
+        return self.type
+
     def load(self, filename):
         """
-        Load the supervision information.
+        Load the academic details.
         """
-        self.students = filename["Students"]
         self.year = filename["Year"]
         self.title = filename["Title"]
         self.program = filename["Program"]
         self.type = filename["Type"]
 
-    def __str__(self) -> str:
-        string = f"Students: {self.students}\n"
-        string += f"Year: {self.year}\n"
-        string += f"Title: {self.title}\n"
-        string += f"Program: {self.program}\n"
-        string += f"Type: {self.type}\n"
-        return string
-
     def __repr__(self) -> str:
-        string = (
-            f"SupervisionInfo("
-            f"students={self.students}, "
+        return (
+            f"AcademicDetails("
             f"year={self.year}, "
             f"title={self.title}, "
             f"program={self.program}, "
             f"type={self.type})"
         )
-        return string
 
 
-class SupervisionData:
+class SupervisionDetails:
     """
-    A class to represent the data of a supervision.
+    The SupervisionDetails class is used to store the supervision details.
 
     Attributes:
-    info (SupervisionInfo): The information of the supervision.
-    institution (str): The institution of the supervision.
-    supervisors (list): The supervisors of the supervision.
-    students (list): The students of the supervision.
+    institution (str): The institution.
+    supervisors (str): The supervisors.
+    students (str): The students.
     """
 
     def __init__(self):
-        self.info = SupervisionInfo()
         self.institution = str()
         self.supervisors = str()
         self.students = str()
 
+    def get_institution(self):
+        """
+        Get the institution.
+        """
+        return self.institution
+
+    def get_supervisors(self):
+        """
+        Get the supervisors.
+        """
+        return self.supervisors
+
+    def get_students(self):
+        """
+        Get the students.
+        """
+        return self.students
+
     def load(self, filename):
         """
-        Load the supervision data.
+        Load the supervision details.
         """
-        self.info.load(filename)
         self.institution = filename["Institution"]
         self.supervisors = filename["Supervisors"]
-
-    def __str__(self) -> str:
-        string = str(self.info)
-        string += f"Institution: {self.institution}\n"
-        string += f"Supervisors: {self.supervisors}\n"
-        string += f"Students: {self.students}\n"
-        return string
+        self.students = filename["Students"]
 
     def __repr__(self) -> str:
-        string = (
-            f"SupervisionData("
-            f"info={repr(self.info)}, "
+        return (
+            f"SupervisionDetails("
             f"institution={self.institution}, "
             f"supervisors={self.supervisors}, "
             f"students={self.students})"
         )
-        return string
+
+
+class SupervisionData:
+    """
+    The Supervision class is used to store the supervision data.
+
+    Attributes:
+    info (AcademicDetails): The academic details.
+    institution (str): The institution.
+    """
+
+    def __init__(self):
+        self.academic = AcademicDetails()
+        self.supervision = SupervisionDetails()
+
+    def load(self, filename):
+        """
+        Load the supervision data.
+        """
+        self.academic.load(filename)
+        self.supervision.load(filename)
+
+    def __repr__(self) -> str:
+        return (
+            f"SupervisionData("
+            f"info={repr(self.academic)}, "
+            f"institution={self.supervision.institution})"
+        )
 
 
 class Supervision:
     """
     A class to represent the supervision data.
 
     Attributes:
@@ -114,43 +160,46 @@
 
     def get_supervision_types_ordered(self):
         """
         Get the supervision types in order.
         """
         supervision_types = []
         for supervision in self.supervisions:
-            if supervision.info.type not in supervision_types:
-                supervision_types.append(supervision.info.type)
+            if supervision.academic.type not in supervision_types:
+                supervision_types.append(supervision.academic.type)
         return supervision_types
 
     def get_num_supervision_by_document_type(self, supervision_type):
         """
         Get the number of supervision by document type.
         """
         count = 0
         for supervision in self.supervisions:
-            if supervision.info.type == supervision_type:
+            if supervision.academic.type == supervision_type:
                 count += 1
         return count
 
     def load(self, filename):
         """
         Load the supervision data.
         """
         supervision_df = pd.read_excel(filename, sheet_name="Supervision")
         for _, row in supervision_df.iterrows():
             supervision_data = SupervisionData()
             supervision_data.load(row)
             self.supervisions.append(supervision_data)
         # sort the supervision data by type and year
         self.supervisions = sorted(
-            self.supervisions, key=lambda x: (x.info.type, x.info.year), reverse=True)
+            self.supervisions, key=lambda x: (x.academic.type, x.academic.year), reverse=True)
 
     def __str__(self) -> str:
         string = ""
         for supervision in self.supervisions:
             string += str(supervision) + "\n"
         return string
 
     def __repr__(self) -> str:
         string = f"Supervision(supervision={repr(list(self.supervisions))})"
         return string
+
+    def __iter__(self):
+        return iter(self.supervisions)
```

### Comparing `cvprocessor-0.5.9/src/cvprocessor/teaching.py` & `cvprocessor-0.6.0/src/cvprocessor/teaching.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,63 +1,12 @@
 """
 This module contains the classes to process the teaching data from the CV.
 """
 import pandas as pd
-
-
-class YearData:
-    """
-    A class to represent the year data.
-
-    Attributes:
-    year_range (str): The year range.
-    start_year (datetime): The start year.
-    end_year (datetime): The end year.
-    """
-
-    def __init__(self):
-        self.year_range = None
-        self.start_year = None
-        self.end_year = None
-
-    def format_year(self, year):
-        """
-        Format the year to a datetime object.
-        """
-        year = year.strip()
-        year = pd.to_datetime(year, format="%b %Y")
-        return year
-
-    def process_year_range(self, year_range):
-        """
-        Process the year range.
-        """
-        year_range = year_range.split("-")
-        self.start_year = self.format_year(year_range[0])
-        self.start_year = pd.to_datetime(self.start_year, format="%b %Y")
-        if len(year_range) > 1:
-            self.end_year = self.format_year(year_range[1])
-            self.end_year = pd.to_datetime(self.end_year, format="%b %Y")
-        else:
-            self.end_year = None
-
-    def __str__(self):
-        string = f"Year range: {self.year_range}\n"
-        string += f"Start year: {self.start_year}\n"
-        string += f"End year: {self.end_year}\n"
-        return string
-
-    def __repr__(self):
-        string = (
-            f"YearData("
-            f"year_range={self.year_range}, "
-            f"start_year={self.start_year}, "
-            f"end_year={self.end_year})"
-        )
-        return string
+from cvprocessor import year_data as yd
 
 
 class TeachingInfo:
     """
     A class to represent the teaching information.
 
     Attributes:
@@ -73,50 +22,47 @@
         self.position = str()
         self.course = str()
         self.link = str()
         self.type = str()
 
     def get_start_year(self):
         """
-        Get the start year of this teaching activity.
+        Get the start year of the teaching.
         """
-        min_year = 1e6
-        date = None
-        for year in self.years:
-            if int(year.start_year.year) < min_year:
-                min_year = int(year.start_year.year)
-                date = year.start_year
-        return date
+        return yd.get_start_year(self.years)
 
     def get_end_year(self):
         """
-        Get the end year of this teaching activity.
+        Get the end year of the teaching.
+        """
+        return yd.get_end_year(self.years)
+
+    def get_position(self):
+        """
+        Get the position of the teaching.
+        """
+        return self.position
+
+    def get_course(self):
+        """
+        Get the course of the teaching.
         """
-        max_year = -1
-        date = None
-        for year in self.years:
-            if year.end_year is not None:
-                if int(year.end_year.year) > max_year:
-                    max_year = int(year.end_year.year)
-                    date = year.end_year
-        return date
+        return self.course
 
-    def add_year(self, year):
+    def get_link(self):
         """
-        Add a year to the year list.
+        Get the link of the teaching.
         """
-        assert isinstance(year, YearData)
-        self.years.append(year)
+        return self.link
 
-    def sort_years(self):
+    def get_type(self):
         """
-        Sort the years by start year.
+        Get the type of the teaching.
         """
-        self.years = sorted(
-            self.years, key=lambda x: x.start_year, reverse=True)
+        return self.type
 
     def __str__(self):
         string = f"Year: {list(map(str, self.years))}\n"
         string += f"Position: {self.position}\n"
         string += f"Course: {self.course}\n"
         string += f"Link: {self.link}\n"
         string += f"Type: {self.type}\n"
@@ -163,22 +109,15 @@
         """
         return self.info.get_end_year()
 
     def process_year_data(self, filename):
         """
         Process the year data.
         """
-        year_range = filename["Year"].split(";")
-        year_range = list(filter(None, year_range))
-        for year in year_range:
-            year_data = YearData()
-            year_data.year_range = year
-            year_data.process_year_range(year)
-            self.info.add_year(year_data)
-        self.info.sort_years()
+        self.info.years = yd.process_year_data(filename, self.info.years)
 
     def load(self, filename):
         """
         Load the teaching data.
         """
         self.process_year_data(filename)
         self.info.position = filename["Position"]
@@ -252,7 +191,10 @@
         for teaching in self.teaching:
             string += str(teaching) + "\n"
         return string
 
     def __repr__(self):
         string = f"Teaching(teaching={repr(self.teaching)})"
         return string
+
+    def __iter__(self):
+        return iter(self.teaching)
```

### Comparing `cvprocessor-0.5.9/src/cvprocessor.egg-info/PKG-INFO` & `cvprocessor-0.6.0/src/cvprocessor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.5.9
+Version: 0.6.0
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.5.9/src/cvprocessor.egg-info/SOURCES.txt` & `cvprocessor-0.6.0/src/cvprocessor.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -16,12 +16,13 @@
 src/cvprocessor/references.py
 src/cvprocessor/research_interests.py
 src/cvprocessor/service.py
 src/cvprocessor/skills.py
 src/cvprocessor/software.py
 src/cvprocessor/supervision.py
 src/cvprocessor/teaching.py
+src/cvprocessor/year_data.py
 src/cvprocessor.egg-info/PKG-INFO
 src/cvprocessor.egg-info/SOURCES.txt
 src/cvprocessor.egg-info/dependency_links.txt
 src/cvprocessor.egg-info/requires.txt
 src/cvprocessor.egg-info/top_level.txt
```

