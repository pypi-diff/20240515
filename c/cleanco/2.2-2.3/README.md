# Comparing `tmp/cleanco-2.2.tar.gz` & `tmp/cleanco-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/petri/Code/koodaamo/cleanco/dist/tmppo3wpftu/cleanco-2.2.tar", last modified: Tue Nov 16 19:42:49 2021, max compression
+gzip compressed data, was "cleanco-2.3.tar", last modified: Wed May 15 16:18:03 2024, max compression
```

## Comparing `cleanco-2.2.tar` & `cleanco-2.3.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 petri      (501) staff       (20)        0 2021-11-16 19:42:49.586188 cleanco-2.2/
--rw-r--r--   0 petri      (501) staff       (20)     1098 2020-04-18 07:51:53.000000 cleanco-2.2/LICENSE.txt
--rw-r--r--   0 petri      (501) staff       (20)     3447 2021-11-16 19:42:49.586381 cleanco-2.2/PKG-INFO
--rw-r--r--   0 petri      (501) staff       (20)     2929 2021-11-16 19:27:50.000000 cleanco-2.2/README.md
-drwxr-xr-x   0 petri      (501) staff       (20)        0 2021-11-16 19:42:49.584701 cleanco-2.2/cleanco/
--rw-r--r--   0 petri      (501) staff       (20)      110 2021-11-16 19:28:23.000000 cleanco-2.2/cleanco/__init__.py
--rw-r--r--   0 petri      (501) staff       (20)     1685 2020-05-04 19:42:38.000000 cleanco-2.2/cleanco/classify.py
--rw-r--r--   0 petri      (501) staff       (20)     3617 2021-11-16 19:16:43.000000 cleanco-2.2/cleanco/clean.py
--rw-r--r--   0 petri      (501) staff       (20)     4975 2020-04-25 16:46:38.000000 cleanco-2.2/cleanco/clean_old.py
--rw-r--r--   0 petri      (501) staff       (20)     3671 2020-06-21 19:58:47.000000 cleanco-2.2/cleanco/non_nfkd_map.py
--rw-r--r--   0 petri      (501) staff       (20)     7106 2021-11-15 19:47:28.000000 cleanco-2.2/cleanco/termdata.py
-drwxr-xr-x   0 petri      (501) staff       (20)        0 2021-11-16 19:42:49.585856 cleanco-2.2/cleanco.egg-info/
--rw-r--r--   0 petri      (501) staff       (20)     3447 2021-11-16 19:42:49.000000 cleanco-2.2/cleanco.egg-info/PKG-INFO
--rw-r--r--   0 petri      (501) staff       (20)      286 2021-11-16 19:42:49.000000 cleanco-2.2/cleanco.egg-info/SOURCES.txt
--rw-r--r--   0 petri      (501) staff       (20)        1 2021-11-16 19:42:49.000000 cleanco-2.2/cleanco.egg-info/dependency_links.txt
--rw-r--r--   0 petri      (501) staff       (20)        8 2021-11-16 19:42:49.000000 cleanco-2.2/cleanco.egg-info/top_level.txt
--rw-r--r--   0 petri      (501) staff       (20)       63 2021-11-16 19:42:49.587099 cleanco-2.2/setup.cfg
--rwxr-xr-x   0 petri      (501) staff       (20)      886 2021-11-16 19:30:24.000000 cleanco-2.2/setup.py
+drwxr-xr-x   0 petri      (501) staff       (20)        0 2024-05-15 16:18:03.087478 cleanco-2.3/
+-rw-r--r--   0 petri      (501) staff       (20)     1098 2020-04-18 07:51:53.000000 cleanco-2.3/LICENSE.txt
+-rw-r--r--   0 petri      (501) staff       (20)     3427 2024-05-15 16:18:03.087116 cleanco-2.3/PKG-INFO
+-rw-r--r--   0 petri      (501) staff       (20)     2929 2021-11-16 19:27:50.000000 cleanco-2.3/README.md
+drwxr-xr-x   0 petri      (501) staff       (20)        0 2024-05-15 16:18:03.069706 cleanco-2.3/cleanco/
+-rw-r--r--   0 petri      (501) staff       (20)      110 2021-11-16 19:28:23.000000 cleanco-2.3/cleanco/__init__.py
+-rw-r--r--   0 petri      (501) staff       (20)     1685 2020-05-04 19:42:38.000000 cleanco-2.3/cleanco/classify.py
+-rw-r--r--   0 petri      (501) staff       (20)     3617 2021-11-16 19:16:43.000000 cleanco-2.3/cleanco/clean.py
+-rw-r--r--   0 petri      (501) staff       (20)     4975 2020-04-25 16:46:38.000000 cleanco-2.3/cleanco/clean_old.py
+-rw-r--r--   0 petri      (501) staff       (20)     3671 2020-06-21 19:58:47.000000 cleanco-2.3/cleanco/non_nfkd_map.py
+-rw-r--r--   0 petri      (501) staff       (20)     7176 2024-05-15 16:08:52.000000 cleanco-2.3/cleanco/termdata.py
+drwxr-xr-x   0 petri      (501) staff       (20)        0 2024-05-15 16:18:03.085719 cleanco-2.3/cleanco.egg-info/
+-rw-r--r--   0 petri      (501) staff       (20)     3427 2024-05-15 16:18:03.000000 cleanco-2.3/cleanco.egg-info/PKG-INFO
+-rw-r--r--   0 petri      (501) staff       (20)      310 2024-05-15 16:18:03.000000 cleanco-2.3/cleanco.egg-info/SOURCES.txt
+-rw-r--r--   0 petri      (501) staff       (20)        1 2024-05-15 16:18:03.000000 cleanco-2.3/cleanco.egg-info/dependency_links.txt
+-rw-r--r--   0 petri      (501) staff       (20)        8 2024-05-15 16:18:03.000000 cleanco-2.3/cleanco.egg-info/top_level.txt
+-rw-r--r--   0 petri      (501) staff       (20)       63 2024-05-15 16:18:03.088603 cleanco-2.3/setup.cfg
+-rwxr-xr-x   0 petri      (501) staff       (20)      886 2024-05-15 16:09:58.000000 cleanco-2.3/setup.py
+drwxr-xr-x   0 petri      (501) staff       (20)        0 2024-05-15 16:18:03.083787 cleanco-2.3/tests/
+-rw-r--r--   0 petri      (501) staff       (20)     4048 2021-11-16 19:16:43.000000 cleanco-2.3/tests/test_cleanname.py
```

### Comparing `cleanco-2.2/LICENSE.txt` & `cleanco-2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cleanco-2.2/PKG-INFO` & `cleanco-2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cleanco
-Version: 2.2
+Version: 2.3
 Summary: Python library to process company names
 Home-page: https://github.com/psolin/cleanco
 Author: Paul Solin
 Author-email: paul@paulsolin.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Topic :: Office/Business
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -73,9 +72,7 @@
 
 To run tests, simply install the package and run `python setup.py test`. To run tests on multiple Python versions, install `tox` and run it (see the provided tox.ini).
 
 ## Special thanks to:
 
 - Wikipedia's [Types of Business Entity article](http://en.wikipedia.org/wiki/Types_of_business_entity), where I spent hours of research.
 - Contributors: [Petri Savolainen](https://github.com/petri)
-
-
```

### Comparing `cleanco-2.2/README.md` & `cleanco-2.3/README.md`

 * *Files identical despite different names*

### Comparing `cleanco-2.2/cleanco/classify.py` & `cleanco-2.3/cleanco/classify.py`

 * *Files identical despite different names*

### Comparing `cleanco-2.2/cleanco/clean.py` & `cleanco-2.3/cleanco/clean.py`

 * *Files identical despite different names*

### Comparing `cleanco-2.2/cleanco/clean_old.py` & `cleanco-2.3/cleanco/clean_old.py`

 * *Files identical despite different names*

### Comparing `cleanco-2.2/cleanco/non_nfkd_map.py` & `cleanco-2.3/cleanco/non_nfkd_map.py`

 * *Files identical despite different names*

### Comparing `cleanco-2.2/cleanco/termdata.py` & `cleanco-2.3/cleanco/termdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
       's.m.b.a.', 'g/s'
    ],
    'Dominican Republic': ['c. por a.', 'cxa', 's.a.', 's.a.s.', 'srl.', 'srl', 'eirl.', 'sa',
       'sas'
    ],
    'Ecuador': ['s.a.', 'c.a.', 'sa', 'ep'],
    'Egypt': ['sae'],
-   'Estonia': ['fie'],
+   'Estonia': ['fie', 'oü', 'as'],
    'Finland': ['t:mi', 'tmi', 'as oy', 'as.oy', 'ay', 'ky', 'oy', 'oyj', 'ok'],
    'France': ['sicav', 'sarl', 'sogepa', 'ei', 'eurl', 'sasu', 'fcp', 'gie', 'sep', 'snc',
       'scs', 'sca', 'scop', 'sem', 'sas'
    ],
    'Germany': ['gmbh & co. kg', 'e.g.', 'e.v.', 'gbr', 'ohg', 'partg',
       'kgaa', 'gmbh', 'g.m.b.h.', 'ag', 'mbh & co. kg'
    ],
@@ -93,21 +93,22 @@
    ],
    'Iceland': ['ehf.', 'hf.', 'ohf.', 's.f.', 'ses.'],
    'India': ['pvt. ltd.', 'ltd.', 'psu', 'pse'],
    'Indonesia': ['ud', 'fa', 'pt'],
    'Ireland': ['cpt', 'teo'],
    'Israel': ['b.m.', 'bm', 'ltd', 'limited'],
    'Italy': ['s.n.c.', 's.a.s.', 's.p.a.', 's.a.p.a.', 's.r.l.', 's.c.r.l.', 's.s.'],
+   'Japan': ['k.k.','g.k.','gk','y.k.'],
    'Latvia': ['as', 'sia', 'ik', 'ps', 'ks'],
    'Lebanon': ['sal'],
    'Lithuania': ['uab', 'ab', 'ij', 'mb'],
    'Luxemborg': ['s.a.', 's.a.r.l.', 'secs'],
    'Macedonia': ['d.o.o.', 'd.o.o.e.l', 'k.d.a.', 'j.t.d.', 'a.d.', 'k.d.'],
    'Malaysia': ['bhd.', 'sdn. bhd.'],
-   'Mexico': ['s.a.', 's. de. r.l.', 's. en c.', 's.a.b.', 's.a.p.i.'],
+   'Mexico': ['s.a.', 's. de. r.l.', 's. en c.', 's.a.b.', 's.a.p.i.', 's.a. de c.v.'],
    'Mongolia': ['xk', 'xxk'],
    'Netherlands': ['v.o.f.', 'c.v.', 'b.v.', 'n.v.'],
    'New Zealand': ['tapui', 'ltd', 'limited'],
    'Nigeria': ['gte.', 'plc', 'ltd.', 'ultd.'],
    'Norway': ['asa', 'as', 'ans', 'ba', 'bl', 'da', 'etat', 'fkf', 'hf', 'iks', 'kf',
       'ks', 'nuf', 'rhf', 'sf'
    ],
```

### Comparing `cleanco-2.2/cleanco.egg-info/PKG-INFO` & `cleanco-2.3/cleanco.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cleanco
-Version: 2.2
+Version: 2.3
 Summary: Python library to process company names
 Home-page: https://github.com/psolin/cleanco
 Author: Paul Solin
 Author-email: paul@paulsolin.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Topic :: Office/Business
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -73,9 +72,7 @@
 
 To run tests, simply install the package and run `python setup.py test`. To run tests on multiple Python versions, install `tox` and run it (see the provided tox.ini).
 
 ## Special thanks to:
 
 - Wikipedia's [Types of Business Entity article](http://en.wikipedia.org/wiki/Types_of_business_entity), where I spent hours of research.
 - Contributors: [Petri Savolainen](https://github.com/petri)
-
-
```

### Comparing `cleanco-2.2/setup.py` & `cleanco-2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='cleanco',
       description='Python library to process company names',
       long_description=long_description,
       long_description_content_type='text/markdown',
-      version='2.2',
+      version='2.3',
       license="MIT",
       license_files=('LICENSE.txt',),
       classifiers = [
          "Topic :: Office/Business",
          "Development Status :: 4 - Beta",
          "Intended Audience :: Developers",
          "License :: OSI Approved :: MIT License",
```

