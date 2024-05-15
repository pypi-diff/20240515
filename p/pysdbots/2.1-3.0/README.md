# Comparing `tmp/pysdbots-2.1.tar.gz` & `tmp/pysdbots-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysdbots-2.1.tar", last modified: Sat Jul 15 12:30:06 2023, max compression
+gzip compressed data, was "pysdbots-3.0.tar", last modified: Wed May 15 12:22:13 2024, max compression
```

## Comparing `pysdbots-2.1.tar` & `pysdbots-3.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 12:30:06.096149 pysdbots-2.1/
--rw-rw-rw-   0        0        0     1093 2022-08-26 22:30:10.000000 pysdbots-2.1/LICENSE
--rw-rw-rw-   0        0        0     2682 2023-07-15 12:30:06.093149 pysdbots-2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1494 2023-07-15 12:18:50.000000 pysdbots-2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-15 12:30:06.048946 pysdbots-2.1/pysdbots/
--rw-rw-rw-   0        0        0      261 2023-07-15 11:27:56.000000 pysdbots-2.1/pysdbots/__init__.py
--rw-rw-rw-   0        0        0     1587 2023-07-14 21:27:21.000000 pysdbots-2.1/pysdbots/pysdbots.py
-drwxrwxrwx   0        0        0        0 2023-07-15 12:30:06.090121 pysdbots-2.1/pysdbots.egg-info/
--rw-rw-rw-   0        0        0     2682 2023-07-15 12:30:05.000000 pysdbots-2.1/pysdbots.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-07-15 12:30:05.000000 pysdbots-2.1/pysdbots.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 12:30:05.000000 pysdbots-2.1/pysdbots.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-15 12:30:05.000000 pysdbots-2.1/pysdbots.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-15 12:30:05.000000 pysdbots-2.1/pysdbots.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 12:30:06.097155 pysdbots-2.1/setup.cfg
--rw-rw-rw-   0        0        0     1528 2023-07-15 12:19:19.000000 pysdbots-2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 12:22:13.296184 pysdbots-3.0/
+-rw-rw-rw-   0        0        0     1093 2024-05-10 17:21:31.000000 pysdbots-3.0/LICENSE
+-rw-rw-rw-   0        0        0     2767 2024-05-15 12:22:13.293185 pysdbots-3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1494 2024-05-10 17:21:31.000000 pysdbots-3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 12:22:13.190047 pysdbots-3.0/pysdbots/
+-rw-rw-rw-   0        0        0      260 2024-05-11 17:35:47.000000 pysdbots-3.0/pysdbots/__init__.py
+-rw-rw-rw-   0        0        0       19 2024-05-11 17:34:40.000000 pysdbots-3.0/pysdbots/__version__.py
+-rw-rw-rw-   0        0        0     9022 2024-05-11 18:17:29.000000 pysdbots-3.0/pysdbots/pysdbots.py
+drwxrwxrwx   0        0        0        0 2024-05-15 12:22:13.291353 pysdbots-3.0/pysdbots.egg-info/
+-rw-rw-rw-   0        0        0     2767 2024-05-15 12:22:12.000000 pysdbots-3.0/pysdbots.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2024-05-15 12:22:13.000000 pysdbots-3.0/pysdbots.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 12:22:12.000000 pysdbots-3.0/pysdbots.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-15 12:22:12.000000 pysdbots-3.0/pysdbots.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-15 12:22:12.000000 pysdbots-3.0/pysdbots.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 12:22:13.296184 pysdbots-3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1882 2024-05-15 12:14:20.000000 pysdbots-3.0/setup.py
```

### Comparing `pysdbots-2.1/LICENSE` & `pysdbots-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysdbots-2.1/PKG-INFO` & `pysdbots-3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysdbots
-Version: 2.1
+Version: 3.0
 Summary: A Project Made To Centralize Various APIs 📖 No Authorization Needed :)
 Home-page: https://github.com/Damantha126/pysdbots
 Author: DamanthaJasinghe
 Author-email: damanthaja@gmail.com
 License: MIT
 Project-URL: Tracker, https://github.com/Damantha126/pysdbots/issues
 Project-URL: Community, https://t.me/SDBOTs_inifinity
@@ -17,16 +17,18 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests>=2.28.1
 
 # 📕 [Documentation](https://docs.sdbots.tech)
 <p align="center">
     <a href="https://t.me/SDBOTs_inifinity">
         <img src="https://telegra.ph/file/a040faed9f94a9a7cb289.jpg" alt="sdbots" width="640">
     </a>
     <br>
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: pysdbots Version: 2.1 Summary: A Project Made To
+Metadata-Version: 2.1 Name: pysdbots Version: 3.0 Summary: A Project Made To
 Centralize Various APIs ð No Authorization Needed :) Home-page: https://
 github.com/Damantha126/pysdbots Author: DamanthaJasinghe Author-email:
 damanthaja@gmail.com License: MIT Project-URL: Tracker, https://github.com/
 Damantha126/pysdbots/issues Project-URL: Community, https://t.me/
 SDBOTs_inifinity Project-URL: Source, https://github.com/Damantha126/pysdbots
 Project-URL: Documentation, https://docs.sdbots.tech Keywords: sdbots,python-
 pakage,sd-api,api,damanthaja,mritzme,damantha126,pysdbots,jasinghe,damantha-
 jasinghe Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Description-Content-Type:
-text/markdown License-File: LICENSE # ð [Documentation](https://
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Description-Content-Type: text/markdown License-
+File: LICENSE Requires-Dist: requests>=2.28.1 # ð [Documentation](https://
 docs.sdbots.tech)
                                    _[_s_d_b_o_t_s_]
   AA PPrroojjeecctt MMaaddee TToo CCeennttrraalliizzee VVaarriioouuss AAPPIIss ?ð??? NNoo AAuutthhoorriizzaattiioonn NNeeeeddeedd ::))
                     _HH_oo_mm_ee_pp_aa_gg_ee_ ?â??¢ _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn_ ?â??¢ _CC_hh_aa_nn_nn_ee_ll
 # â¢ Features FFeeaattuurreess ooff tthhee ssddbboottss AAPPII
 ?â??¤ TTeelleeggrraapphh LLiinnkk
 ?â??¤ FFaasstt RReessppoonnssee
```

### Comparing `pysdbots-2.1/README.md` & `pysdbots-3.0/README.md`

 * *Files identical despite different names*

### Comparing `pysdbots-2.1/pysdbots.egg-info/PKG-INFO` & `pysdbots-3.0/pysdbots.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysdbots
-Version: 2.1
+Version: 3.0
 Summary: A Project Made To Centralize Various APIs 📖 No Authorization Needed :)
 Home-page: https://github.com/Damantha126/pysdbots
 Author: DamanthaJasinghe
 Author-email: damanthaja@gmail.com
 License: MIT
 Project-URL: Tracker, https://github.com/Damantha126/pysdbots/issues
 Project-URL: Community, https://t.me/SDBOTs_inifinity
@@ -17,16 +17,18 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests>=2.28.1
 
 # 📕 [Documentation](https://docs.sdbots.tech)
 <p align="center">
     <a href="https://t.me/SDBOTs_inifinity">
         <img src="https://telegra.ph/file/a040faed9f94a9a7cb289.jpg" alt="sdbots" width="640">
     </a>
     <br>
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: pysdbots Version: 2.1 Summary: A Project Made To
+Metadata-Version: 2.1 Name: pysdbots Version: 3.0 Summary: A Project Made To
 Centralize Various APIs ð No Authorization Needed :) Home-page: https://
 github.com/Damantha126/pysdbots Author: DamanthaJasinghe Author-email:
 damanthaja@gmail.com License: MIT Project-URL: Tracker, https://github.com/
 Damantha126/pysdbots/issues Project-URL: Community, https://t.me/
 SDBOTs_inifinity Project-URL: Source, https://github.com/Damantha126/pysdbots
 Project-URL: Documentation, https://docs.sdbots.tech Keywords: sdbots,python-
 pakage,sd-api,api,damanthaja,mritzme,damantha126,pysdbots,jasinghe,damantha-
 jasinghe Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Description-Content-Type:
-text/markdown License-File: LICENSE # ð [Documentation](https://
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Description-Content-Type: text/markdown License-
+File: LICENSE Requires-Dist: requests>=2.28.1 # ð [Documentation](https://
 docs.sdbots.tech)
                                    _[_s_d_b_o_t_s_]
   AA PPrroojjeecctt MMaaddee TToo CCeennttrraalliizzee VVaarriioouuss AAPPIIss ?ð??? NNoo AAuutthhoorriizzaattiioonn NNeeeeddeedd ::))
                     _HH_oo_mm_ee_pp_aa_gg_ee_ ?â??¢ _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn_ ?â??¢ _CC_hh_aa_nn_nn_ee_ll
 # â¢ Features FFeeaattuurreess ooff tthhee ssddbboottss AAPPII
 ?â??¤ TTeelleeggrraapphh LLiinnkk
 ?â??¤ FFaasstt RReessppoonnssee
```

### Comparing `pysdbots-2.1/setup.py` & `pysdbots-3.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,53 @@
+import os
+from typing import Dict
 import setuptools
+from pysdbots import __docs__
+
+base_path = os.path.abspath(os.path.dirname(__file__))
 
 with open("README.md", encoding="utf8") as readme:
     long_description = readme.read()
 
+about: Dict = {}
+with open(
+    os.path.join(
+        base_path,
+        'pysdbots',
+        '__version__.py',
+    ), encoding='utf-8',
+) as f:
+    exec(f.read(), about)
+
 setuptools.setup(
     name="pysdbots",
     packages=setuptools.find_packages(),
-    version="2.1",
+    version=about['__version__'],
     license="MIT",
     description="A Project Made To Centralize Various APIs 📖 No Authorization Needed :)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="DamanthaJasinghe",
     author_email="damanthaja@gmail.com",
     url="https://github.com/Damantha126/pysdbots",
     keywords=["sdbots", "python-pakage", "sd-api", "api", "damanthaja", "mritzme", "damantha126", "pysdbots", "jasinghe", "damantha-jasinghe"],
     install_requires=["requests>=2.28.1"],
     project_urls={
         "Tracker": "https://github.com/Damantha126/pysdbots/issues",
         "Community": "https://t.me/SDBOTs_inifinity",
         "Source": "https://github.com/Damantha126/pysdbots",
-        "Documentation": "https://docs.sdbots.tech",
+        "Documentation": __docs__,
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
 )
```

