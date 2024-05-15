# Comparing `tmp/pyprocessors_segment_renseignor-0.5.4.tar.gz` & `tmp/pyprocessors_segment_renseignor-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprocessors_segment_renseignor-0.5.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyprocessors_segment_renseignor-0.5.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyprocessors_segment_renseignor-0.5.4.tar` & `pyprocessors_segment_renseignor-0.5.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rwxr-xr-x   0        0        0      507 2024-05-07 08:59:54.596728 pyprocessors_segment_renseignor-0.5.4/.bumpversion.cfg
--rwxr-xr-x   0        0        0     1760 2024-05-07 08:59:54.596728 pyprocessors_segment_renseignor-0.5.4/.gitignore
--rwxr-xr-x   0        0        0      419 2024-05-07 08:59:54.596728 pyprocessors_segment_renseignor-0.5.4/.pre-commit-config.yaml
--rwxr-xr-x   0        0        0      202 2024-05-07 08:59:54.596728 pyprocessors_segment_renseignor-0.5.4/.readthedocs.yml
--rwxr-xr-x   0        0        0      127 2024-05-07 08:59:54.596728 pyprocessors_segment_renseignor-0.5.4/AUTHORS.md
--rwxr-xr-x   0        0        0      268 2024-05-07 08:59:54.596728 pyprocessors_segment_renseignor-0.5.4/CHANGELOG.md
--rwxr-xr-x   0        0        0      476 2024-05-07 08:59:54.596728 pyprocessors_segment_renseignor-0.5.4/Dockerfile
--rwxr-xr-x   0        0        0    10251 2024-05-07 08:59:54.596728 pyprocessors_segment_renseignor-0.5.4/Jenkinsfile
--rwxr-xr-x   0        0        0     1082 2024-05-07 08:59:54.596728 pyprocessors_segment_renseignor-0.5.4/LICENSE
--rwxr-xr-x   0        0        0     1693 2024-05-07 08:59:54.596728 pyprocessors_segment_renseignor-0.5.4/README.md
--rwxr-xr-x   0        0        0      961 2024-05-07 08:59:54.596728 pyprocessors_segment_renseignor-0.5.4/RELEASE.md
--rwxr-xr-x   0        0        0     1559 2024-05-07 08:59:54.596728 pyprocessors_segment_renseignor-0.5.4/bumpversion.py
--rwxr-xr-x   0        0        0       62 2024-05-07 08:59:54.596728 pyprocessors_segment_renseignor-0.5.4/docs/.gitignore
--rwxr-xr-x   0        0        0      268 2024-05-07 08:59:54.596728 pyprocessors_segment_renseignor-0.5.4/docs/CHANGELOG.md
--rwxr-xr-x   0        0        0     1082 2024-05-07 08:59:54.596728 pyprocessors_segment_renseignor-0.5.4/docs/LICENSE
--rwxr-xr-x   0        0        0        0 2024-05-07 08:59:54.596728 pyprocessors_segment_renseignor-0.5.4/docs/_static/.gitkeep
--rwxr-xr-x   0        0        0        0 2024-05-07 08:59:54.596728 pyprocessors_segment_renseignor-0.5.4/docs/_templates/.gitkeep
--rwxr-xr-x   0        0        0     2929 2024-05-07 08:59:54.596728 pyprocessors_segment_renseignor-0.5.4/docs/conf.py
--rwxr-xr-x   0        0        0      152 2024-05-07 08:59:54.596728 pyprocessors_segment_renseignor-0.5.4/docs/index.rst
--rwxr-xr-x   0        0        0       98 2024-05-07 08:59:54.596728 pyprocessors_segment_renseignor-0.5.4/mypy.ini
--rwxr-xr-x   0        0        0     2279 2024-05-07 08:59:54.596728 pyprocessors_segment_renseignor-0.5.4/pyproject.toml
--rwxr-xr-x   0        0        0       59 2024-05-07 09:48:49.887102 pyprocessors_segment_renseignor-0.5.4/src/pyprocessors_segment_renseignor/__init__.py
--rwxr-xr-x   0        0        0     6546 2024-05-07 08:59:54.596728 pyprocessors_segment_renseignor-0.5.4/src/pyprocessors_segment_renseignor/segment_renseignor.py
--rwxr-xr-x   0        0        0        0 2024-05-07 08:59:54.596728 pyprocessors_segment_renseignor-0.5.4/tests/__init__.py
--rw-r--r--   0        0        0    48908 2024-05-07 09:48:47.123012 pyprocessors_segment_renseignor-0.5.4/tests/data/renseignor-document-segmented.json
--rw-r--r--   0        0        0    82169 2024-05-07 08:59:54.600728 pyprocessors_segment_renseignor-0.5.4/tests/data/renseignor-document-test.json
--rwxr-xr-x   0        0        0     1047 2024-05-07 08:59:54.600728 pyprocessors_segment_renseignor-0.5.4/tests/test_segment_renseignor.py
--rwxr-xr-x   0        0        0      927 2024-05-07 09:47:19.192165 pyprocessors_segment_renseignor-0.5.4/tox.ini
--rw-r--r--   0        0        0     1376 1970-01-01 00:00:00.000000 pyprocessors_segment_renseignor-0.5.4/setup.py
--rw-r--r--   0        0        0     3430 1970-01-01 00:00:00.000000 pyprocessors_segment_renseignor-0.5.4/PKG-INFO
+-rwxr-xr-x   0        0        0      507 2024-05-07 11:02:48.904337 pyprocessors_segment_renseignor-0.5.8/.bumpversion.cfg
+-rwxr-xr-x   0        0        0     1803 2024-05-07 11:02:48.908336 pyprocessors_segment_renseignor-0.5.8/.gitignore
+-rwxr-xr-x   0        0        0      419 2024-05-07 11:02:48.908336 pyprocessors_segment_renseignor-0.5.8/.pre-commit-config.yaml
+-rwxr-xr-x   0        0        0      202 2024-05-07 11:02:48.908336 pyprocessors_segment_renseignor-0.5.8/.readthedocs.yml
+-rwxr-xr-x   0        0        0      127 2024-05-07 11:02:48.908336 pyprocessors_segment_renseignor-0.5.8/AUTHORS.md
+-rwxr-xr-x   0        0        0      268 2024-05-07 11:02:48.908336 pyprocessors_segment_renseignor-0.5.8/CHANGELOG.md
+-rwxr-xr-x   0        0        0      476 2024-05-07 11:02:48.908336 pyprocessors_segment_renseignor-0.5.8/Dockerfile
+-rw-r--r--   0        0        0    14014 2024-05-07 11:02:48.908336 pyprocessors_segment_renseignor-0.5.8/Jenkinsfile
+-rwxr-xr-x   0        0        0     1082 2024-05-07 11:02:48.908336 pyprocessors_segment_renseignor-0.5.8/LICENSE
+-rwxr-xr-x   0        0        0     1693 2024-05-07 11:02:48.908336 pyprocessors_segment_renseignor-0.5.8/README.md
+-rwxr-xr-x   0        0        0      961 2024-05-07 11:02:48.908336 pyprocessors_segment_renseignor-0.5.8/RELEASE.md
+-rwxr-xr-x   0        0        0     1559 2024-05-07 11:02:48.908336 pyprocessors_segment_renseignor-0.5.8/bumpversion.py
+-rwxr-xr-x   0        0        0       62 2024-05-07 11:02:48.908336 pyprocessors_segment_renseignor-0.5.8/docs/.gitignore
+-rwxr-xr-x   0        0        0      268 2024-05-07 11:02:48.908336 pyprocessors_segment_renseignor-0.5.8/docs/CHANGELOG.md
+-rwxr-xr-x   0        0        0     1082 2024-05-07 11:02:48.908336 pyprocessors_segment_renseignor-0.5.8/docs/LICENSE
+-rwxr-xr-x   0        0        0        0 2024-05-07 11:02:48.908336 pyprocessors_segment_renseignor-0.5.8/docs/_static/.gitkeep
+-rwxr-xr-x   0        0        0        0 2024-05-07 11:02:48.908336 pyprocessors_segment_renseignor-0.5.8/docs/_templates/.gitkeep
+-rwxr-xr-x   0        0        0     2929 2024-05-07 11:02:48.908336 pyprocessors_segment_renseignor-0.5.8/docs/conf.py
+-rwxr-xr-x   0        0        0      152 2024-05-07 11:02:48.908336 pyprocessors_segment_renseignor-0.5.8/docs/index.rst
+-rwxr-xr-x   0        0        0       98 2024-05-07 11:02:48.908336 pyprocessors_segment_renseignor-0.5.8/mypy.ini
+-rwxr-xr-x   0        0        0     2279 2024-05-07 11:02:48.908336 pyprocessors_segment_renseignor-0.5.8/pyproject.toml
+-rwxr-xr-x   0        0        0       59 2024-05-07 11:04:17.623032 pyprocessors_segment_renseignor-0.5.8/src/pyprocessors_segment_renseignor/__init__.py
+-rwxr-xr-x   0        0        0     6560 2024-05-07 11:02:48.908336 pyprocessors_segment_renseignor-0.5.8/src/pyprocessors_segment_renseignor/segment_renseignor.py
+-rwxr-xr-x   0        0        0        0 2024-05-07 11:02:48.908336 pyprocessors_segment_renseignor-0.5.8/tests/__init__.py
+-rw-r--r--   0        0        0    49921 2024-05-07 11:04:14.986952 pyprocessors_segment_renseignor-0.5.8/tests/data/renseignor-document-segmented.json
+-rw-r--r--   0        0        0    82169 2024-05-07 11:02:48.912337 pyprocessors_segment_renseignor-0.5.8/tests/data/renseignor-document-test.json
+-rwxr-xr-x   0        0        0     1047 2024-05-07 11:02:48.912337 pyprocessors_segment_renseignor-0.5.8/tests/test_segment_renseignor.py
+-rwxr-xr-x   0        0        0      927 2024-05-07 11:02:48.912337 pyprocessors_segment_renseignor-0.5.8/tox.ini
+-rw-r--r--   0        0        0     1376 1970-01-01 00:00:00.000000 pyprocessors_segment_renseignor-0.5.8/setup.py
+-rw-r--r--   0        0        0     3430 1970-01-01 00:00:00.000000 pyprocessors_segment_renseignor-0.5.8/PKG-INFO
```

### Comparing `pyprocessors_segment_renseignor-0.5.4/.gitignore` & `pyprocessors_segment_renseignor-0.5.8/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -123,7 +123,11 @@
 dmypy.json
 
 # Pyre type checker
 .pyre/
 
 # PyCharm stuff:
 .idea
+
+# Specific
+.groovylintrc.json
+.emailNotif
```

### Comparing `pyprocessors_segment_renseignor-0.5.4/LICENSE` & `pyprocessors_segment_renseignor-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprocessors_segment_renseignor-0.5.4/README.md` & `pyprocessors_segment_renseignor-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `pyprocessors_segment_renseignor-0.5.4/RELEASE.md` & `pyprocessors_segment_renseignor-0.5.8/RELEASE.md`

 * *Files identical despite different names*

### Comparing `pyprocessors_segment_renseignor-0.5.4/bumpversion.py` & `pyprocessors_segment_renseignor-0.5.8/bumpversion.py`

 * *Files identical despite different names*

### Comparing `pyprocessors_segment_renseignor-0.5.4/docs/LICENSE` & `pyprocessors_segment_renseignor-0.5.8/docs/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprocessors_segment_renseignor-0.5.4/docs/conf.py` & `pyprocessors_segment_renseignor-0.5.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyprocessors_segment_renseignor-0.5.4/pyproject.toml` & `pyprocessors_segment_renseignor-0.5.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyprocessors_segment_renseignor-0.5.4/src/pyprocessors_segment_renseignor/segment_renseignor.py` & `pyprocessors_segment_renseignor-0.5.8/src/pyprocessors_segment_renseignor/segment_renseignor.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
                         tanns = list(g)
                         atext = ""
                         for a in tanns:
                             if a.labelName == "footer":
                                 atext += useful_text[previous:a.start].strip()
                                 previous = a.end
                             elif a.labelName == "source":
-                                ametadata = {}
+                                ametadata = {"TOPIC": topic}
                                 if a.properties is not None:
                                     for k, v in a.properties.items():
                                         if k == "DATE":
                                             ametadata["ARTICLE DATE"] = v
                                         elif k == "SOURCE/Name":
                                             ametadata["SOURCE NAME"] = v
                                 ametadata.update(metadata)
```

### Comparing `pyprocessors_segment_renseignor-0.5.4/tests/data/renseignor-document-segmented.json` & `pyprocessors_segment_renseignor-0.5.8/tests/data/renseignor-document-segmented.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9744047619047623%*

 * *Differences: {'0': "{'metadata': {'TOPIC': None}}",*

 * * '1': "{'metadata': {'TOPIC': None}}",*

 * * '10': "{'metadata': {'TOPIC': 'MILITAIRE'}}",*

 * * '11': "{'metadata': {'TOPIC': 'MILITAIRE'}}",*

 * * '12': "{'metadata': {'TOPIC': 'MILITAIRE'}}",*

 * * '13': "{'metadata': {'TOPIC': 'MILITAIRE'}}",*

 * * '14': "{'metadata': {'TOPIC': 'MILITAIRE'}}",*

 * * '15': "{'metadata': {'TOPIC': 'MILITAIRE'}}",*

 * * '16': "{'metadata': {'TOPIC': 'MILITAIRE'}}",*

 * * '17': "{'metadata': {'TOPIC': 'MILITAIRE'}}",*

 * * '18': "{'metadata': {'TOPIC': 'MILITAIRE'}}",*

 * * '19': "{'m […]*

```diff
@@ -1,308 +1,336 @@
 [
     {
         "identifier": "1312-0",
         "metadata": {
             "ARTICLE DATE": "03-01-2024",
             "PUBLICATION DATE": "7 janvier 2024",
             "PUBLICATION NUMBER": "1312",
-            "SOURCE NAME": "Radio Prague international"
+            "SOURCE NAME": "Radio Prague international",
+            "TOPIC": null
         },
         "text": "Une ancienne r\u00e9dactrice en chef de la BBC aurait travaill\u00e9 pour les\nservices de renseignement tch\u00e9coslovaques...\nSelon des documents d'archives, Ter\u00e9zia Javorska, ancienne r\u00e9dactrice\nen  chef  de  la  section  tch\u00e9coslovaque  de  la  BBC et,  jusqu'en  2005,\nresponsable  des  \u00e9missions  en  slovaque  de  BBC  World  Service,  a\ntravaill\u00e9 en tant que collaboratrice puis agent du Service de s\u00e9curit\u00e9 de\nl'\u00c9tat  (StB)  de  la  Tch\u00e9coslovaquie  communiste.  Le  site  HlidaciPes a\nsoulign\u00e9 ce mercredi que des informations provenant des archives de la\nStB  ont  \u00e9t\u00e9  retrouv\u00e9es  \u00e0  Prague  par  un  journaliste  du  Daily  Mail\nbritannique.  Un officier  de la StB,  qui  travaillait  alors sous couverture\ndiplomatique  \u00e0  l'ambassade  tch\u00e9coslovaque  de  Londres,  a  recrut\u00e9\nT. Javorska  au  milieu  des  ann\u00e9es  1980.  \u00ab Les  experts  en  s\u00e9curit\u00e9\nestiment  qu'il  s'agit  du  premier  cas  connu d'agent  de  renseignement\n\u00e9tranger infiltr\u00e9 \u00e0 la  BBC depuis le d\u00e9but de la Guerre froide \u00bb \u00e9crit le\nDaily Mail.",
         "title": "Une ancienne r\u00e9dactrice en chef de la BBC aurait travaill\u00e9 pour les\nservices de renseignement tch\u00e9coslovaques"
     },
     {
         "identifier": "1312-1",
         "metadata": {
             "ARTICLE DATE": "01-01-2024",
             "PUBLICATION DATE": "7 janvier 2024",
             "PUBLICATION NUMBER": "1312",
-            "SOURCE NAME": "La voix de la Turquie"
+            "SOURCE NAME": "La voix de la Turquie",
+            "TOPIC": null
         },
         "text": "En Syrie, un cadre pr\u00e9sum\u00e9 du groupe \u00c9tat islamique captur\u00e9 par\nles services de renseignement turcs...\nL'Agence turque du renseignement (MIT) a captur\u00e9 lundi le chef de file\nde Daesh dans la ville d'Alep, en Syrie, Abdullah al-Jundi, qui planifiait\ndes attaques contre les forces turques dans les zones des op\u00e9rations\nBouclier de l'Euphrate  et Branche d'Olivier. Al-Jundi, surnomm\u00e9 Hattab\nEl-Muhacir,  \u00e9tait  responsable  de  la  planification  d'actions  contre  les\nv\u00e9hicules appartenant aux forces de s\u00e9curit\u00e9 turques en Syrie selon les\nforces de s\u00e9curit\u00e9. Le terroriste a \u00e9t\u00e9 captur\u00e9 lors d'une op\u00e9ration men\u00e9e\npar le MIT et les forces de s\u00e9curit\u00e9 locales affili\u00e9es \u00e0 l'arm\u00e9e nationale\nsyrienne dans la zone de l'op\u00e9ration Bouclier de l'Euphrate. Le terroriste\na \u00e9galement fourni des informations sur les membres de l'organisation\nimpliqu\u00e9s  dans  des  activit\u00e9s  terroristes.  Du  mat\u00e9riel  num\u00e9rique\ncontenant des donn\u00e9es sur les plans d\u2019action de Daesh a \u00e9galement \u00e9t\u00e9\nsaisi au cours de l'op\u00e9ration, ce qui est de nature \u00e0 perturber les activit\u00e9s\nde l'organisation.  En 2013,  la  Turquie  est  devenue l'un  des premiers\npays  \u00e0  d\u00e9clarer  Daesh  organisation  terroriste.  Depuis,  le  pays  a  \u00e9t\u00e9\nattaqu\u00e9  \u00e0  plusieurs  reprises  par  le  groupe  terroriste,  avec  plus  de\n300 personnes tu\u00e9es et des centaines d'autres bless\u00e9es dans au moins\ndix  attentats  suicide,  sept  attentats  \u00e0  la  bombe  et  quatre  attaques\narm\u00e9es. En r\u00e9ponse, la Turquie a lanc\u00e9 des op\u00e9rations antiterroristes \u00e0\nl'int\u00e9rieur et \u00e0 l'ext\u00e9rieur du pays pour pr\u00e9venir de nouvelles attaques.",
         "title": "En Syrie, un cadre pr\u00e9sum\u00e9 du groupe \u00c9tat islamique captur\u00e9 par\nles services de renseignement turcs"
     },
     {
         "identifier": "1312-2",
         "metadata": {
             "ARTICLE DATE": "02-01-2024",
             "PUBLICATION DATE": "7 janvier 2024",
             "PUBLICATION NUMBER": "1312",
-            "SOURCE NAME": "Deutsche Welle"
+            "SOURCE NAME": "Deutsche Welle",
+            "TOPIC": null
         },
         "text": "En  Allemagne,  garde  \u00e0  vue  prolong\u00e9e  pour  deux  islamistes\npr\u00e9sum\u00e9s...\nLa  justice  allemande  a  prolong\u00e9  hier  lundi  la  garde-\u00e0-vue  de  deux\nislamistes pr\u00e9sum\u00e9s arr\u00eat\u00e9s ces derniers jours en raison de soup\u00e7ons de\npr\u00e9paration d\u2019un attentat le soir  du nouvel An contre la cath\u00e9drale de\nCologne, dans l\u2019ouest du pays.",
         "title": "En  Allemagne,  garde  \u00e0  vue  prolong\u00e9e  pour  deux  islamistes\npr\u00e9sum\u00e9s"
     },
     {
         "identifier": "1312-3",
         "metadata": {
             "ARTICLE DATE": "03-01-2024",
             "PUBLICATION DATE": "7 janvier 2024",
             "PUBLICATION NUMBER": "1312",
-            "SOURCE NAME": "Press TV"
+            "SOURCE NAME": "Press TV",
+            "TOPIC": "TERRORISME"
         },
         "text": "\u2026\n\nPlusieurs dizaines de morts lors d\u2019un double attentat terroriste dans le sud-est de l\u2019Iran...\nDeux attentats terroristes \u00e0 Kerman, dans le sud-est du pays, ont fait mercredi 3 janvier 73 morts et\n170 bless\u00e9s, selon l\u2019Organisation des urgences iranienne. Les explosions se sont produites pr\u00e8s de la\ns\u00e9pulture  du  g\u00e9n\u00e9ral  martyr  iranien,  Qassem  Soleimani,  o\u00f9  les  gens  s\u2019\u00e9taient  rassembl\u00e9s  pour\nparticiper \u00e0 la c\u00e9r\u00e9monie du quatri\u00e8me anniversaire de sa mort en martyr. Des ambulances se sont\npr\u00e9cipit\u00e9es sur place. Selon  IRNA,  la premi\u00e8re explosion s\u2019est produite \u00e0 environ 700 m\u00e8tres de la\ntombe du g\u00e9n\u00e9ral Soleimani et la seconde, \u00e0 environ un kilom\u00e8tre plus loin. L\u2019agence de presse Tasnim\na cit\u00e9 des sources anonymes affirmant que deux valises charg\u00e9es d\u2019explosifs d\u00e9clench\u00e9es \u00e0 distance\n\u00e9taient \u00e0 l\u2019origine des explosions. La premi\u00e8re explosion s\u2019est produite \u00e0 14h50, heure locale, et la\nseconde 15 minutes plus tard. Certaines personnes ont \u00e9t\u00e9 bless\u00e9es lors du mouvement de foule o\u00f9\ns\u2019\u00e9tait produite la premi\u00e8re explosion. Les autorit\u00e9s affirment que tous les bless\u00e9s ont \u00e9t\u00e9 transf\u00e9r\u00e9s\nvers des h\u00f4pitaux et que la situation est sous contr\u00f4le.",
         "title": "\u2026\n\nPlusieurs dizaines de morts lors d\u2019un double attentat terroriste dans le sud-est de l\u2019Iran"
     },
     {
         "identifier": "1312-4",
         "metadata": {
             "ARTICLE DATE": "04-01-2023",
             "PUBLICATION DATE": "7 janvier 2024",
             "PUBLICATION NUMBER": "1312",
-            "SOURCE NAME": "La voix de l\u2019Am\u00e9rique"
+            "SOURCE NAME": "La voix de l\u2019Am\u00e9rique",
+            "TOPIC": "TERRORISME"
         },
         "text": "Washington rejette les accusations iraniennes accusant les \u00c9tats-Unis et Isra\u00ebl d\u2019\u00eatre impliqu\u00e9s\ndans l\u2019attentat de Kerman...\nLes \u00c9tats-Unis ont jug\u00e9 absurde toute suggestion que les \u00c9tats-Unis ou Isra\u00ebl seraient impliqu\u00e9s dans\nl\u2019attentat  perp\u00e9tr\u00e9  mercredi  en  Iran  pr\u00e8s  de  la  tombe  de  Qassem  Soleimani,  l\u2019ex-architecte  des\nop\u00e9rations militaires iraniennes au Moyen-Orient, dont l\u2019Iran comm\u00e9more le quatri\u00e8me anniversaire de\nla mort selon des m\u00e9dias d\u2019\u00c9tat. Au moins 103 personnes ont \u00e9t\u00e9 tu\u00e9es et plus de 211 bless\u00e9es dans\ncet attentat. Le porte-parole du d\u00e9partement d\u2019\u00c9tat, Matthew Miller, a assur\u00e9 qu\u2019aucun pays n\u2019avait\nint\u00e9r\u00eat \u00e0 une escalade dans la r\u00e9gion. \u00ab Les \u00c9tats-Unis n\u2019ont \u00e9t\u00e9 impliqu\u00e9s en aucune fa\u00e7on. Toute\naffirmation contraire est absurde \u00bb a-t-il soulign\u00e9 \u00e0 la presse. L\u2019Iran a accus\u00e9 Isra\u00ebl et les \u00c9tats-Unis\nd\u2019\u00eatre derri\u00e8re l\u2019attentat.",
         "title": "Washington rejette les accusations iraniennes accusant les \u00c9tats-Unis et Isra\u00ebl d\u2019\u00eatre impliqu\u00e9s\ndans l\u2019attentat de Kerman"
     },
     {
         "identifier": "1312-5",
         "metadata": {
             "ARTICLE DATE": "05-01-2024",
             "PUBLICATION DATE": "7 janvier 2024",
             "PUBLICATION NUMBER": "1312",
-            "SOURCE NAME": "Press TV"
+            "SOURCE NAME": "Press TV",
+            "TOPIC": "TERRORISME"
         },
         "text": "Le double attentat de Kerman revendiqu\u00e9 par le groupe \u00c9tat islamique...\nLe groupe terroriste Daesh a revendiqu\u00e9 dans un communiqu\u00e9 l\u2019attentat terroriste qui a co\u00fbt\u00e9 la vie \u00e0\n84 personnes qui allaient se recueillir sur la tombe du martyr Qassem Soleimani \u00e0 Kerman. Daesh a\n\u00e9galement affirm\u00e9 qu\u2019Omar al-Movhed et Seif-o-Allah, deux de ses membres, \u00e9taient les deux auteurs\nde cet attentat qui ont activ\u00e9 leur ceinture explosive. Les deux explosions sont survenues mercredi\napr\u00e8s-midi 3 janvier sur la route menant au cimeti\u00e8re des martyrs \u00e0 Kerman. Elles ont fait 84 martyrs et\n284 bless\u00e9s, ce qui a suscit\u00e9 la condamnation de divers pays et groupes.",
         "title": "Le double attentat de Kerman revendiqu\u00e9 par le groupe \u00c9tat islamique"
     },
     {
         "identifier": "1312-6",
         "metadata": {
             "ARTICLE DATE": "04-01-2024",
             "PUBLICATION DATE": "7 janvier 2024",
             "PUBLICATION NUMBER": "1312",
-            "SOURCE NAME": "La voix de la Turquie"
+            "SOURCE NAME": "La voix de la Turquie",
+            "TOPIC": "TERRORISME"
         },
         "text": "Un membre pr\u00e9sum\u00e9 du PKK neutralis\u00e9 par les forces turques dans le nord de l\u2019Irak...\nLes services de renseignement turcs ont neutralis\u00e9 un terroriste du PKK qui pr\u00e9parait  une attaque\ncontre la Turquie lors d'une op\u00e9ration transfrontali\u00e8re dans le nord de l'Irak, ont indiqu\u00e9 des sources\ns\u00e9curitaires ce jeudi. L'Organisation nationale du renseignement (MIT) avait d\u00e9couvert que Sadik Seyh\nAhmet,  un terroriste du PKK/KCK, op\u00e9rait  dans les zones rurales des r\u00e9gions de Souleimaniye et\nPenjwin en Irak, ont d\u00e9clar\u00e9 les sources sous couvert d'anonymat. Sadik Seyh Ahmet, qui pr\u00e9parait des\nattaques  terroristes  contre  la  Turquie,  a  \u00e9t\u00e9  localis\u00e9  par  les  services  de  renseignement  turcs  et\nneutralis\u00e9 lors de l'op\u00e9ration. Le terroriste, qui \u00e9tait venu en Turquie au d\u00e9but des mouvements anti-\nr\u00e9gime en Syrie, est retourn\u00e9 en Syrie en 2015 et a men\u00e9 des activit\u00e9s arm\u00e9es au sein du PKK/YPG. Il\na \u00e9galement \u00e9t\u00e9 d\u00e9couvert qu'Ahmet, qui avait op\u00e9r\u00e9 dans diff\u00e9rentes positions au nom du groupe\nterroriste en Syrie pendant longtemps, avait ensuite d\u00e9m\u00e9nag\u00e9 en Irak et avait finalement agi avec les\npr\u00e9tendus membres de haut niveau du groupe terroriste situ\u00e9s \u00e0 la fronti\u00e8re irako-iranienne. L'op\u00e9ration\nantiterroriste a eu lieu apr\u00e8s l'attaque terroriste du PKK du 29 d\u00e9cembre qui a tu\u00e9 douze soldats turcs\ndans le nord de l'Irak. Depuis lors, les frappes a\u00e9riennes turques ont d\u00e9truit des dizaines de cibles\nterroristes dans le nord de l'Irak et en Syrie, neutralisant des terroristes de haut niveau. Les terroristes\ndu PKK se cachent  souvent  dans le nord de l'Irak pour planifier  des attaques transfrontali\u00e8res en\nTurquie. Le groupe a \u00e9galement une branche syrienne, connue sous le nom de YPG.",
         "title": "Un membre pr\u00e9sum\u00e9 du PKK neutralis\u00e9 par les forces turques dans le nord de l\u2019Irak"
     },
     {
         "identifier": "1312-7",
         "metadata": {
             "ARTICLE DATE": "02-01-2024",
             "PUBLICATION DATE": "7 janvier 2024",
             "PUBLICATION NUMBER": "1312",
-            "SOURCE NAME": "La voix de la Turquie"
+            "SOURCE NAME": "La voix de la Turquie",
+            "TOPIC": "ACTIVIT\u00c9S DES SERVICES DE RENSEIGNEMENT"
         },
         "text": "\u2026\n\nEn  Turquie,  arrestation  d\u2019une  trentaine  de  personnes  accus\u00e9es  d\u2019espionnage  au  profit  du\nMossad...\nLes  autorit\u00e9s  turques  ont  arr\u00eat\u00e9  33 personnes  soup\u00e7onn\u00e9es  de  s'\u00eatre  livr\u00e9es  \u00e0  des  activit\u00e9s\nd'espionnage pour le compte du Mossad, le service de renseignement ext\u00e9rieur isra\u00e9lien, selon des\nsources s\u00e9curitaires. Ces arrestations font suite \u00e0 une enqu\u00eate men\u00e9e par le Bureau d'enqu\u00eate sur le\nterrorisme  et  les  crimes  organis\u00e9s  du  Bureau  du  procureur  d'Istanbul,  ax\u00e9e  sur  l'espionnage\ninternational. Les suspects auraient \u00e9t\u00e9 impliqu\u00e9s dans des activit\u00e9s telles que le renseignement, la\nsurveillance,  l'agression  et  l'enl\u00e8vement  pour  le  compte  du  Mossad.  Une  op\u00e9ration  antiterroriste,\norganis\u00e9e conjointement par l'Organisation nationale du renseignement (MIT) et la police d'Istanbul, a\npermis d\u2019appr\u00e9hender les suspects. Des \u00ab descentes \u00bb simultan\u00e9es \u00e0 57 adresses dans huit provinces\nont permis de capturer les suspects, tandis que des op\u00e9rations de recherche de 13 autres suspects\nsont en cours. Se faisant passer pour des employ\u00e9s d'une soci\u00e9t\u00e9 de conseil bas\u00e9e \u00e0 Istanbul, les\nsuspects ont fourni au Mossad des informations sur les Palestiniens en Turquie en \u00e9change d'argent.\nIsra\u00ebl n'a pas r\u00e9agi \u00e0 ces all\u00e9gations.",
         "title": "\u2026\n\nEn  Turquie,  arrestation  d\u2019une  trentaine  de  personnes  accus\u00e9es  d\u2019espionnage  au  profit  du\nMossad"
     },
     {
         "identifier": "1312-8",
         "metadata": {
             "ARTICLE DATE": "03-01-2024",
             "PUBLICATION DATE": "7 janvier 2024",
             "PUBLICATION NUMBER": "1312",
-            "SOURCE NAME": "Radio Ta\u00efwan international"
+            "SOURCE NAME": "Radio Ta\u00efwan international",
+            "TOPIC": "ACTIVIT\u00c9S DES SERVICES DE RENSEIGNEMENT"
         },
         "text": "Trois militaires ta\u00efwanais soup\u00e7onn\u00e9s d\u2019espionnage au profit de la Chine...\nLe minist\u00e8re de la D\u00e9fense a confirm\u00e9 hier un dossier d\u2019espionnage impliquant au moins trois militaires\net un membre d\u2019une maison de pr\u00eat clandestine. Plusieurs m\u00e9dias ta\u00efwanais ont r\u00e9v\u00e9l\u00e9 que les trois\nmilitaires impliqu\u00e9s dans l\u2019affaire seraient en poste dans une station radar de l\u2019arm\u00e9e de l\u2019air dans le\nsud  du  pays.  Selon  les  m\u00e9dias,  n\u2019\u00e9tant  plus  en  mesure  de  rembourser  leurs  pr\u00eats,  les  militaires\nauraient fourni des informations  classiffi\u00e9es de leur unit\u00e9 \u00e0 la Chine communiste. Plusieurs suspects\nont \u00e9t\u00e9 entendus par les procureurs de Chiaotou, de la ville de Kaohisung, dont trois ont \u00e9t\u00e9 remis en\nlibert\u00e9 sous caution. Selon le minist\u00e8re de la D\u00e9fense, la Chine populaire se serait servi de maisons de\npr\u00eat clandestines pour d\u00e9velopper \u00e0 Ta\u00efwan de nouveaux r\u00e9seaux d\u2019espionnage.",
         "title": "Trois militaires ta\u00efwanais soup\u00e7onn\u00e9s d\u2019espionnage au profit de la Chine"
     },
     {
         "identifier": "1312-9",
         "metadata": {
             "ARTICLE DATE": "02-01-2024",
             "PUBLICATION DATE": "7 janvier 2024",
             "PUBLICATION NUMBER": "1312",
-            "SOURCE NAME": "La voix de la Turquie"
+            "SOURCE NAME": "La voix de la Turquie",
+            "TOPIC": "MILITAIRE"
         },
         "text": "\u2026\n\nUn b\u00e2timent de guerre iranien d\u00e9ploy\u00e9 en mer Rouge...\nL\u2019Iran a d\u00e9ploy\u00e9 un de ses navires de guerre en mer Rouge dans un contexte de tensions, les rebelles\nHouthis  du Y\u00e9men ciblant  les  navires  marchands venant  ou \u00e0  destination d\u2019Isra\u00ebl.  Les \u00c9tats-Unis\ns'opposent \u00e0 l'action des Houthis en mer Rouge. Le navire de guerre iranien Alborz est entr\u00e9 en mer\nRouge par le d\u00e9troit de Bab el-Mandeb rapporte l\u2019agence de presse iranienne Tasnim, alors que les\ntensions sont vives sur cette voie strat\u00e9gique pour le commerce mondial, th\u00e9\u00e2tre d'attaques r\u00e9p\u00e9t\u00e9es\ndes Houthis du Y\u00e9men contre des navires marchands li\u00e9s \u00e0 Isra\u00ebl. N\u00e9anmoins, l'agence de presse\nTasnim n'a pas pr\u00e9cis\u00e9 les raisons de ce d\u00e9ploiement. La flotte iranienne op\u00e8re dans la zone depuis\n2009, pour s\u00e9curiser les voies de navigation et repousser les pirates, entre autres, a-t-elle, par ailleurs\npr\u00e9cis\u00e9.",
         "title": "\u2026\n\nUn b\u00e2timent de guerre iranien d\u00e9ploy\u00e9 en mer Rouge"
     },
     {
         "identifier": "1312-10",
         "metadata": {
             "ARTICLE DATE": "03-01-2024",
             "PUBLICATION DATE": "7 janvier 2024",
             "PUBLICATION NUMBER": "1312",
-            "SOURCE NAME": "Deutsche Welle"
+            "SOURCE NAME": "Deutsche Welle",
+            "TOPIC": "MILITAIRE"
         },
         "text": "Multiplication des vols de ballons chinois \u00e0 proximit\u00e9 de Ta\u00efwan \u00e0 l\u2019approche des \u00e9lections\npr\u00e9sidentielles...\nTa\u00efwan a d\u00e9tect\u00e9  quatre  ballons chinois  avant  la  pr\u00e9sidentielle.  C\u2019est  ce qu\u2019a  indiqu\u00e9 le  minist\u00e8re\nta\u00efwanais de la D\u00e9fense. Les ballons chinois ont \u00e9t\u00e9 rep\u00e9r\u00e9s au-dessus de la ligne m\u00e9diane du d\u00e9troit\nde Ta\u00efwan qui s\u00e9pare l\u2019\u00eele de la Chine continentale. Les observations de ballons chinois \u00e0 Ta\u00efwan ont\nd\u00e9but\u00e9 le mois dernier et interviennent \u00e0 moins de deux semaines de la pr\u00e9sidentielle tr\u00e8s cruciale\ndans l\u2019\u00eele, le 13 janvier. Le minist\u00e8re ta\u00efwanais de la D\u00e9fense a signal\u00e9 avoir observ\u00e9 des ballons \u00e0 six\nreprises en d\u00e9cembre.",
         "title": "Multiplication des vols de ballons chinois \u00e0 proximit\u00e9 de Ta\u00efwan \u00e0 l\u2019approche des \u00e9lections\npr\u00e9sidentielles"
     },
     {
         "identifier": "1312-11",
         "metadata": {
             "ARTICLE DATE": "05-01-2024",
             "PUBLICATION DATE": "7 janvier 2024",
             "PUBLICATION NUMBER": "1312",
-            "SOURCE NAME": "Radio Ta\u00efwan international"
+            "SOURCE NAME": "Radio Ta\u00efwan international",
+            "TOPIC": "MILITAIRE"
         },
         "text": "Dans  une  semaine,  les  Ta\u00efwanais  vont  \u00e9lire  leur  nouveau  pr\u00e9sident  et  leurs  repr\u00e9sentants  au\nParlement.  Or,  depuis  le  1er janvier  jusqu\u2019\u00e0  ce  vendredi  5 janvier  \u00e0  6 heures  du  matin,  Ta\u00efwan  a\nobserv\u00e9 le passage de dix ballons chinois dont cinq ont travers\u00e9 le ciel de Ta\u00efwan. Sans commenter\nl\u2019arriv\u00e9e massive de ces ballons, John Kirby, coordinateur des communications strat\u00e9giques au Conseilde  s\u00e9curit\u00e9  nationale  de  la  Maison-Blanche,  a  appel\u00e9  la  communaut\u00e9  internationale  \u00e0  ne  jamais\ninterf\u00e9rer dans les \u00e9lections d\u00e9mocratiques libres et \u00e9quitables \u00e0 Ta\u00efwan. Du c\u00f4t\u00e9 de Ta\u00efwan, plusieurs\nchercheurs ont comment\u00e9 aujourd\u2019hui l\u2019envoi de ces ballons et demandent au gouvernement d\u2019adopter\ndes mesures plus actives pour \u00e9viter la guerre cognitive, comme l\u2019indique le professeur Lin Ying-yu,\nchercheur  \u00e0  l\u2019Institut  de  recherche  sur  les  affaires  et  les  strat\u00e9gies  internationales  de  l\u2019universit\u00e9\nTamkang : \u00ab La Chine souhaite \u00e9galement, \u00e0 travers ce genre de mouvement, d\u00e9montrer l\u2019incapacit\u00e9\ndu  minist\u00e8re  ta\u00efwanais  de  la  D\u00e9fense,  ce  qui  engendrera  la  m\u00e9fiance  du  public  \u00e0  l\u2019\u00e9gard  du\ngouvernement. Cela rel\u00e8ve des techniques souvent utilis\u00e9es dans la guerre cognitive \u00bb.",
         "title": "(Radio Ta\u00efwan international, le 05-01-2024)"
     },
     {
         "identifier": "1312-12",
         "metadata": {
             "ARTICLE DATE": "02-01-2024",
             "PUBLICATION DATE": "7 janvier 2024",
             "PUBLICATION NUMBER": "1312",
-            "SOURCE NAME": "La voix de la Turquie"
+            "SOURCE NAME": "La voix de la Turquie",
+            "TOPIC": "MILITAIRE"
         },
         "text": "Le porte-avions am\u00e9ricain USS Gerald Ford en passe de quitter la M\u00e9diterran\u00e9e...\nLa marine am\u00e9ricaine a annonc\u00e9 ce mardi que le porte-avions USS Gerald R. Ford allait regagner sa\nbase aux \u00c9tats-Unis, apr\u00e8s des mois pass\u00e9s en M\u00e9diterran\u00e9e pour dissuader toute menace contre\nIsra\u00ebl \u00e0 la suite de l\u2019attaque men\u00e9e par le Hamas. La VIe Flotte am\u00e9ricaine (commandement naval\nbas\u00e9  en  Europe  et  responsable  des  navires  naviguant  en  M\u00e9diterran\u00e9e),  a  d\u00e9clar\u00e9  dans  un\ncommuniqu\u00e9 publi\u00e9 sur son site internet que le porte-avions quittera la r\u00e9gion dans les prochains jours.\nLe communiqu\u00e9 a expliqu\u00e9 que des ordres avaient \u00e9t\u00e9 donn\u00e9s au porte-avions pour se diriger vers la\nM\u00e9diterran\u00e9e orientale afin de contribuer \u00e0 la dissuasion r\u00e9gionale et \u00e0 la pr\u00e9servation de la posture\nd\u00e9fensive.  \u00ab Le porte-avions retournera \u00e0 son port  principal  comme pr\u00e9vu pour pr\u00e9parer les futurs\nd\u00e9ploiements.  Le minist\u00e8re de la D\u00e9fense \u00e9value constamment la situation \u00e0 l\u2019\u00e9chelle mondiale et\nmaintiendra de larges capacit\u00e9s \u00e0 la fois en M\u00e9diterran\u00e9e et au Moyen-Orient. Nous coop\u00e9rons avec\nnos alli\u00e9s  et  partenaires  pour  renforcer  la  s\u00e9curit\u00e9  maritime dans la  r\u00e9gion,  et  le  minist\u00e8re  de la\nD\u00e9fense continuera \u00e0 \u0153uvrer pour dissuader tout \u00c9tat ou entit\u00e9 non gouvernementale d\u2019intensifier cette\ncrise  en  dehors  de  Gaza \u00bb lit-on  de  m\u00eame  source.  L\u2019USS Ford et  les  navires  de  guerre  qui\nl'accompagnent seront remplac\u00e9s par les navires qui se trouvaient en mer Rouge et qui ont travers\u00e9 la\nM\u00e9diterran\u00e9e  orientale  au  cours  des  derniers  jours.  Les  \u00c9tats-Unis  ont  envoy\u00e9  l\u2019USS Ford en\nM\u00e9diterran\u00e9e orientale pour qu\u2019il se trouve \u00e0 courte distance d\u2019Isra\u00ebl, au lendemain des \u00e9v\u00e9nements du\n7 octobre. L\u2019USS Ford est rest\u00e9 dans la r\u00e9gion pendant trois mois, tandis que les navires de guerre qui\nl'accompagnaient ont navigu\u00e9 vers la mer Rouge, o\u00f9 ils ont intercept\u00e9 \u00e0 plusieurs reprises des missiles\nbalistiques et  des attaques de drones lanc\u00e9es par le groupe y\u00e9m\u00e9nite Houthis contre des navires\nassoci\u00e9s \u00e0 Isra\u00ebl, en solidarit\u00e9 avec la bande de Gaza, en proie \u00e0 une guerre isra\u00e9lienne d\u00e9vastatrice\ndepuis le 7 octobre dernier.",
         "title": "Le porte-avions am\u00e9ricain USS Gerald Ford en passe de quitter la M\u00e9diterran\u00e9e"
     },
     {
         "identifier": "1312-13",
         "metadata": {
             "ARTICLE DATE": "03-01-2024",
             "PUBLICATION DATE": "7 janvier 2024",
             "PUBLICATION NUMBER": "1312",
-            "SOURCE NAME": "Radio Roumanie international"
+            "SOURCE NAME": "Radio Roumanie international",
+            "TOPIC": "MILITAIRE"
         },
         "text": "La Roumanie envisage l\u2019am\u00e9nagement d\u2019abris pr\u00e8s de sa fronti\u00e8re avec l\u2019Ukraine...\nLes autorit\u00e9s roumaines ont adopt\u00e9 des mesures pour pr\u00e9venir les incidents tels ceux signal\u00e9s l'ann\u00e9e\nderni\u00e8re  lorsque des drones utilis\u00e9s par  la  Russie  dans la  guerre  en Ukraine sont  tomb\u00e9s sur  le\nterritoire de la Roumanie ou ont p\u00e9n\u00e9tr\u00e9 l'espace a\u00e9rien de la Roumanie, a affirm\u00e9 mardi soir, dans une\ninterview t\u00e9l\u00e9vis\u00e9e, le ministre roumain de la D\u00e9fense, Angen T\u00eelvar. Il a \u00e9voqu\u00e9 l'am\u00e9nagement d'abris,\nla mise en place d'alarmes et l'instruction des repr\u00e9sentants des autorit\u00e9s locales. Le ministre roumain\nde la D\u00e9fense a ajout\u00e9 que si la Roumanie d\u00e9tenait des \u00e9quipements performants pour d\u00e9pister de tels\nappareils, la distance r\u00e9duite entre les localit\u00e9s roumaines o\u00f9 de tels incidents ont eu lieu et le port\nukrainien le plus proche compliquent consid\u00e9rablement leur action.",
         "title": "La Roumanie envisage l\u2019am\u00e9nagement d\u2019abris pr\u00e8s de sa fronti\u00e8re avec l\u2019Ukraine"
     },
     {
         "identifier": "1312-14",
         "metadata": {
             "ARTICLE DATE": "04-01-2024",
             "PUBLICATION DATE": "7 janvier 2024",
             "PUBLICATION NUMBER": "1312",
-            "SOURCE NAME": "Radio Vatican"
+            "SOURCE NAME": "Radio Vatican",
+            "TOPIC": "MILITAIRE"
         },
         "text": "La  d\u00e9fense  antia\u00e9rienne  de  Kiev  en  passe  de  manquer  de  munitions  selon  un  g\u00e9n\u00e9ral\nukrainien...\nL\u2019Ukraine n\u2019aura, \u00e0 moyen terme, plus assez de munitions pour parer les attaques a\u00e9riennes russes.\nC\u2019est la mise en garde d\u2019un g\u00e9n\u00e9ral ukrainien qui appelle les Occidentaux \u00e0 reconstituer les stocks\nukrainiens. Les syst\u00e8mes mobiles de d\u00e9fense antia\u00e9rienne interceptent encore la majeure partie des\ndrones et des missiles russes, mais certains passent entre les mailles du filet.",
         "title": "La  d\u00e9fense  antia\u00e9rienne  de  Kiev  en  passe  de  manquer  de  munitions  selon  un  g\u00e9n\u00e9ral\nukrainien"
     },
     {
         "identifier": "1312-15",
         "metadata": {
             "PUBLICATION DATE": "7 janvier 2024",
-            "PUBLICATION NUMBER": "1312"
+            "PUBLICATION NUMBER": "1312",
+            "TOPIC": "MILITAIRE"
         },
         "text": "Patrouilles maritimes conjointes am\u00e9ricano-philippines en mer de Chine m\u00e9ridionale...\nLes Philippines et les \u00c9tats-Unis ont entam\u00e9 des patrouilles conjointes en mer de Chine m\u00e9ridionale,\nzone  contest\u00e9e.  Mercredi,  l'arm\u00e9e  philippine  a  annonc\u00e9  le  d\u00e9but  de  ces  patrouilles  maritimes  et\na\u00e9riennes conjointes de deux jours avec l'arm\u00e9e am\u00e9ricaine.  C'est  la  deuxi\u00e8me fois  que les deuxparties participent ensemble \u00e0 des exercices en mer de Chine m\u00e9ridionale \u00e0 l\u2019initiative du pr\u00e9sident\nphilippin Ferdinand Marcos Jr. Les Philippines ont d\u00e9ploy\u00e9 quatre navires de combat tandis que les\n\u00c9tats-Unis ont  d\u00e9ploy\u00e9 le porte-avions  USS Carl  Vinson,  deux destroyers,  un croiseur et  plusieurs\navions de combat, ce qui d\u00e9montre un exercice \u00e0 plus grande \u00e9chelle. Le chef d'\u00e9tat-major des forces\narm\u00e9es philippines, le g\u00e9n\u00e9ral Romeo Brawner, a d\u00e9clar\u00e9 que cette activit\u00e9 militaire conjointe marquait\nune avanc\u00e9e significative dans l'alliance bilat\u00e9rale. Il a not\u00e9 que la coalition est plus forte que jamais et\nqu\u2019elle fait progresser un ordre international fond\u00e9 sur des r\u00e8gles, et une r\u00e9gion indopacifique libre et\nouverte face aux d\u00e9fis r\u00e9gionaux. Ces remarques visent apparemment \u00e0 contrer la pr\u00e9sence croissante\nde P\u00e9kin en mer de Chine m\u00e9ridionale. La Chine a ripost\u00e9. Le Commandement du th\u00e9\u00e2tre sud de\nl'arm\u00e9e chinoise a annonc\u00e9 mercredi soir qu'il m\u00e8nerait des patrouilles de routine en mer de Chine\nm\u00e9ridionale de mercredi \u00e0 jeudi. Il a indiqu\u00e9 que les troupes pr\u00e9sentes dans la r\u00e9gion resteraient en\n\u00e9tat d'alerte constant et d\u00e9fendraient la souverainet\u00e9 nationale, la s\u00e9curit\u00e9 et les droits maritimes de la\nChine.",
         "title": "Patrouilles maritimes conjointes am\u00e9ricano-philippines en mer de Chine m\u00e9ridionale"
     },
     {
         "identifier": "1312-16",
         "metadata": {
             "ARTICLE DATE": "03-01-2024",
             "PUBLICATION DATE": "7 janvier 2024",
             "PUBLICATION NUMBER": "1312",
-            "SOURCE NAME": "KBS World Radio"
+            "SOURCE NAME": "KBS World Radio",
+            "TOPIC": "MILITAIRE"
         },
         "text": "Radio Japon international, le 04-01-2024)\n\nPremi\u00e8res man\u0153uvres de l\u2019ann\u00e9e pour la marine sud-cor\u00e9enne...\nLa marine sud-cor\u00e9enne a men\u00e9, aujourd\u2019hui, ses premi\u00e8res man\u0153uvres de l\u2019ann\u00e9e. L\u2019objectif : afficher\nsa  volont\u00e9  de  riposte  ferme aux  \u00e9ventuelles  attaques  du  Nord,  sur  fond  d\u2019escalade  des  tensions\nmilitaires dans la p\u00e9ninsule. Un total de treize navires, dont un d\u2019escorte, le nouveau  Cheonan, ont\nparticip\u00e9 \u00e0 ces exercices. C\u2019\u00e9tait son premier d\u00e9ploiement pour un entra\u00eenement de tir en mer Jaune.\nPour information, le premier  Cheonan avait coul\u00e9, le 26 mars 2010, apr\u00e8s avoir \u00e9t\u00e9 touch\u00e9 par une\ntorpille nord-cor\u00e9enne, pr\u00e8s de l\u2019\u00eele de Baengnyeong. Le mois dernier, le nouveau navire \u00e9ponyme a\nentam\u00e9 sa mission. La marine a d\u00e9clar\u00e9 que, gr\u00e2ce \u00e0 ces entra\u00eenements de combat r\u00e9el, elle pourra\nrenforcer ses capacit\u00e9s de r\u00e9action en cas d\u2019attaque du Nord. Rappelons que le dirigeant nord-cor\u00e9en\nKim Jong-un a indiqu\u00e9, lors de l\u2019assembl\u00e9e pl\u00e9ni\u00e8re du Parti des travailleurs, tenue fin d\u00e9cembre, qu\u2019il\ncontinuerait d\u2019acc\u00e9l\u00e9rer les pr\u00e9parations \u00e0 la guerre afin de dominer la totalit\u00e9 de la p\u00e9ninsule.",
         "title": "Radio Japon international, le 04-01-2024)\n\nPremi\u00e8res man\u0153uvres de l\u2019ann\u00e9e pour la marine sud-cor\u00e9enne"
     },
     {
         "identifier": "1312-17",
         "metadata": {
             "ARTICLE DATE": "04-01-2024",
             "PUBLICATION DATE": "7 janvier 2024",
             "PUBLICATION NUMBER": "1312",
-            "SOURCE NAME": "KBS World Radio"
+            "SOURCE NAME": "KBS World Radio",
+            "TOPIC": "MILITAIRE"
         },
         "text": "Les exercices militaires sud-cor\u00e9ens vivement critiqu\u00e9s par Pyongyang...\nLa Cor\u00e9e du Nord a ouvertement critiqu\u00e9 les r\u00e9cents exercices militaires de l\u2019arm\u00e9e sud-cor\u00e9enne et\naverti que 2024 serait une ann\u00e9e avec des risques d\u2019affrontements violents plus \u00e9lev\u00e9s. Dans un texte\npubli\u00e9 aujourd\u2019hui par son agence de presse officielle, la  KCNA, le r\u00e9gime communiste a notamment\nmis en avant que les forces sp\u00e9ciales sud-cor\u00e9ennes avaient r\u00e9cemment effectu\u00e9 un entra\u00eenement\nhivernal  et  a  reproch\u00e9  au  Sud  de  commencer  cette  nouvelle  ann\u00e9e  avec  un  comportement\nautodestructeur.  Les Nord-Cor\u00e9ens ont pu lire ce m\u00eame commentaire dans le  Rodong Sinmun.  Le\njournal officiel du Parti des travailleurs y a pr\u00e9tendu que les plus hauts grad\u00e9s de l\u2019arm\u00e9e fantoche sud-\ncor\u00e9enne d\u00e9versaient un flot de paroles agressives et insufflaient un climat belliqueux. Et d\u2019ajouter que\nles forces d\u2019invasion avec, \u00e0 leur t\u00eate, les \u00c9tats-Unis et le Japon, sont de plus en plus pr\u00e9sentes dans\nla p\u00e9ninsule, et incitent diff\u00e9rentes provocations telles que les frappes nucl\u00e9aires. Dans cet article, plus\nde pr\u00e9cisions sont \u00e9galement donn\u00e9es sur l\u2019\u00e9tat d\u2019esprit actuel qui r\u00e8gne \u00e0 Pyongyang : en parlant de\nS\u00e9oul  et  Washington,  il  a  annonc\u00e9  que  \u00ab les  fanatiques  d\u2019affrontements  n\u2019\u00e9prouveront  que  des\nmoments  douloureux  inimaginables \u00bb.  De  l\u2019avis  des  experts  sud-cor\u00e9ens  sur  la  question  nord-\ncor\u00e9enne,  le  r\u00e9gime  de  Kim  Jong-un  aurait  fustig\u00e9  les  man\u0153uvres  que  l\u2019arm\u00e9e  du  Sud  m\u00e8ne\nhabituellement en d\u00e9but d\u2019ann\u00e9e pour justifier ses futures provocations. Ces derniers jours en effet,\nKim Jong-un intensifie ses critiques \u00e0 l\u2019\u00e9gard du Sud. Il  a par exemple d\u00e9clar\u00e9, lors de la r\u00e9cente\nassembl\u00e9e  pl\u00e9ni\u00e8re  du  Parti  des  travailleurs,  que  les  deux  Cor\u00e9es  \u00e9taient  des  pays  hostiles  et\nbellig\u00e9rants. Par ailleurs, l\u2019arm\u00e9e de terre sud-cor\u00e9enne a annonc\u00e9 avoir  lanc\u00e9 le 29 d\u00e9cembre les\npremiers exercices militaires de l\u2019ann\u00e9e avec les \u00c9tats-Unis. Les man\u0153uvres ont dur\u00e9 une semaine. Il\ns\u2019agissait pour essentiel de s\u2019entra\u00eener aux tirs r\u00e9els au combat. L\u2019objectif : renforcer les capacit\u00e9s \u00e0\nmener les op\u00e9rations des forces combin\u00e9es.",
         "title": "Les exercices militaires sud-cor\u00e9ens vivement critiqu\u00e9s par Pyongyang"
     },
     {
         "identifier": "1312-18",
         "metadata": {
             "ARTICLE DATE": "05-01-2024",
             "PUBLICATION DATE": "7 janvier 2024",
             "PUBLICATION NUMBER": "1312",
-            "SOURCE NAME": "KBS World Radio"
+            "SOURCE NAME": "KBS World Radio",
+            "TOPIC": "MILITAIRE"
         },
         "text": "La Cor\u00e9e du Nord aurait proc\u00e9d\u00e9 au d\u00e9ploiement d\u2019un grand nombre de mines terrestres le long\nde la zone d\u00e9militaris\u00e9e...\nLe dirigeant nord-cor\u00e9en, Kim Jong-un, a inspect\u00e9 une usine de tracteurs-\u00e9recteurs-lanceurs. C\u2019est ce\nqu\u2019a rapport\u00e9 aujourd\u2019hui le Rodong Sinmun. Il \u00e9tait accompagn\u00e9 de sa fille Ju-ae, consid\u00e9r\u00e9e comme\n\u00ab sa successeure \u00bb.  \u00c9tait  \u00e9galement pr\u00e9sente Kim Yo-jong, sa puissante petite s\u0153ur,  ainsi  que JoYong-won,  le secr\u00e9taire du comit\u00e9 central  du Parti  des travailleurs.  Le journal  officiel  du Parti  des\ntravailleurs  a  publi\u00e9  une  photo  montrant  plusieurs  v\u00e9hicules  de  lancement  de  missiles  balistiques\nintercontinentaux (ICBM) Hwasong-18, affirmant que la Cor\u00e9e du Nord traversait une p\u00e9riode critique\ndurant laquelle il fallait qu\u2019elle se pr\u00e9pare plus rigoureusement \u00e0 une confrontation militaire avec ses\nadversaires.  Le  leader  supr\u00eame  a  f\u00e9licit\u00e9  cette  augmentation  de  la  production  des  rampes  de\nlancement,  avant  d\u2019ordonner  de  prendre  des  mesures  de  modernisation  des  capacit\u00e9s  de  l\u2019usine.\nParall\u00e8lement,  Pyongyang  a  enterr\u00e9  un  grand  nombre  de  mines  sur  la  route  le  long  de  la  ligne\nferroviaire  de Gyeongui,  dans la  zone d\u00e9militaris\u00e9e (DMZ).  Cela a lieu peu de temps apr\u00e8s avoir\nd\u00e9clar\u00e9 la rupture de l'accord militaire intercor\u00e9en du 19 septembre 2018. Un responsable de l\u2019arm\u00e9e\nsud-cor\u00e9enne a d\u00e9clar\u00e9 que leur installation avait \u00e9t\u00e9 observ\u00e9e depuis d\u00e9but d\u00e9cembre. Cette route\nreliant les deux Cor\u00e9es a \u00e9t\u00e9 construite en 2004 et a \u00e9t\u00e9 largement emprunt\u00e9e par les entreprises\nimplant\u00e9es  dans  le  complexe  industriel  de  Gaeseong.  Le  royaume  ermite  a  \u00e9galement  restaur\u00e9\nplusieurs postes de garde au sein de la DMZ. Pour rappel, conform\u00e9ment \u00e0 l\u2019accord militaire bilat\u00e9ral\nde 2018, il les avait d\u00e9truits et \u00e9vacu\u00e9s. Cependant, apr\u00e8s avoir d\u00e9clar\u00e9 son annulation en novembre,\nle Nord a commenc\u00e9 \u00e0 red\u00e9ployer des troupes dans la zone et \u00e0 \u00e9riger des constructions en bois.",
         "title": "La Cor\u00e9e du Nord aurait proc\u00e9d\u00e9 au d\u00e9ploiement d\u2019un grand nombre de mines terrestres le long\nde la zone d\u00e9militaris\u00e9e"
     },
     {
         "identifier": "1312-19",
         "metadata": {
             "ARTICLE DATE": "05-01-2024",
             "PUBLICATION DATE": "7 janvier 2024",
             "PUBLICATION NUMBER": "1312",
-            "SOURCE NAME": "KBS World Radio"
+            "SOURCE NAME": "KBS World Radio",
+            "TOPIC": "MILITAIRE"
         },
         "text": "Plusieurs centaines d\u2019obus tir\u00e9s en mer Jaune par l\u2019artillerie nord-cor\u00e9enne...\nLa Cor\u00e9e du Nord a lanc\u00e9 ce matin pr\u00e8s de 200 obus d'artillerie en mer Jaune qui s\u00e9pare la p\u00e9ninsule\ncor\u00e9enne et  le  continent  chinois.  Selon l\u2019\u00e9tat-major  interarm\u00e9es sud-cor\u00e9en (JCS),  ces tirs  ont  \u00e9t\u00e9\neffectu\u00e9s entre 9 heures et 11 heures pr\u00e8s des caps de Jangsan et Dungsan. Ces deux derniers sont\nrespectivement au nord des \u00eeles sud-cor\u00e9ennes de Baengnyeong et de Yeonpyeong. La plupart des\nobus a \u00e9t\u00e9 tir\u00e9e par de l'artillerie c\u00f4ti\u00e8re et les projectiles sont tomb\u00e9s au nord de la NLL, la fronti\u00e8re\nmaritime inter-cor\u00e9enne. Au Sud, aucun d\u00e9g\u00e2t n\u2019a \u00e9t\u00e9 signal\u00e9, que ce soit du c\u00f4t\u00e9 des habitants comme\ndu c\u00f4t\u00e9 de l\u2019arm\u00e9e. Le JCS a expliqu\u00e9 que le royaume ermite a repris ses provocations dans la zone\ntampon  de  la  mer  \u00e0  l\u2019ouest  apr\u00e8s  avoir  rompu  unilat\u00e9ralement,  en  novembre,  l\u2019accord  militaire\nintercor\u00e9en du 19 septembre. S\u00e9oul surveille chaque mouvement au nord du 38e parall\u00e8le et ce, en\ncoop\u00e9ration \u00e9troite avec Washington. Il a d'ores et d\u00e9j\u00e0 pr\u00e9vu de mettre en \u0153uvre des mesures en\nr\u00e9ponse \u00e0 cette nouvelle provocation de Pyongyang. Les autorit\u00e9s militaires, notamment, envisagent\nd\u2019effectuer  un  tir  de  riposte.  Dans  l\u2019\u00eele  de  Yeonpyeong,  les  autorit\u00e9s  locales  ont  \u00e9mis  un  ordre\nd\u2019\u00e9vacuation aux riverains d\u00e8s le d\u00e9but de ces tirs.",
         "title": "Plusieurs centaines d\u2019obus tir\u00e9s en mer Jaune par l\u2019artillerie nord-cor\u00e9enne"
     },
     {
         "identifier": "1312-20",
         "metadata": {
             "ARTICLE DATE": "05-01-2024",
             "PUBLICATION DATE": "7 janvier 2024",
             "PUBLICATION NUMBER": "1312",
-            "SOURCE NAME": "KBS World Radio"
+            "SOURCE NAME": "KBS World Radio",
+            "TOPIC": "MILITAIRE"
         },
         "text": "Tirs maritimes sud-cor\u00e9ens en r\u00e9ponse aux tirs de sa voisine du nord...\nLa tension est mont\u00e9e d\u2019un cran entre les deux Cor\u00e9es. L\u2019arm\u00e9e sud-cor\u00e9enne a effectu\u00e9 cet apr\u00e8s-\nmidi des tirs maritimes en r\u00e9ponse aux provocations de Pyongyang qui ont eu lieu plus t\u00f4t dans la\njourn\u00e9e. Selon l\u2019\u00e9tat-major interarm\u00e9es sud-cor\u00e9en (JCS), la 6e brigade et l\u2019unit\u00e9 de  Yeonpyeong de\nl\u2019infanterie  de  la  marine  ont  proc\u00e9d\u00e9,  vers  15 heures,  \u00e0  un  exercice  de  tirs.  Ils  ont  mobilis\u00e9  le\nK9 Thunder,  le  canon  d'artillerie  automoteur, ainsi  que  des  canons  de  chars.  Ils  sont  d\u00e9ploy\u00e9s\nrespectivement sur l\u2019\u00eele de Baengnyeong et de Yeonpyeong en mer Jaune, qui s\u00e9pare la p\u00e9ninsule\ncor\u00e9enne et le continent chinois. Notons que c\u2019est la premi\u00e8re fois que les troupes d\u00e9ploy\u00e9es sur les\n\u00eeles dans le nord-ouest du pays m\u00e8nent un tel entra\u00eenement depuis la conclusion de l\u2019accord militaire\nintercor\u00e9en du 19 septembre 2018. C\u2019est au nord de ces derni\u00e8res que la Cor\u00e9e du Nord a lanc\u00e9, ce\nmatin, plus de 200 obus d'artillerie.",
         "title": "Tirs maritimes sud-cor\u00e9ens en r\u00e9ponse aux tirs de sa voisine du nord"
     },
     {
         "identifier": "1312-21",
         "metadata": {
             "ARTICLE DATE": "01-01-2024",
             "PUBLICATION DATE": "7 janvier 2024",
             "PUBLICATION NUMBER": "1312",
-            "SOURCE NAME": "Radio Ta\u00efwan international"
+            "SOURCE NAME": "Radio Ta\u00efwan international",
+            "TOPIC": "L'ACTUALIT\u00c9 DES MARCHANDS D'ARMES"
         },
         "text": "\u2026\n\nLes avions de combat F-16V command\u00e9s par Ta\u00efwan devraient \u00eatre livr\u00e9s avant la fin 2024...\nLes 66 appareils F-16V que Ta\u00efwan avait achet\u00e9s aupr\u00e8s des \u00c9tats-Unis en 2019 et dont la livraison\ndevait d\u00e9buter en 2023 devraient \u00eatre livr\u00e9s \u00e0 partir du troisi\u00e8me trimestre 2024. Le minist\u00e8re ta\u00efwanais\nde la D\u00e9fense a pr\u00e9cis\u00e9 que conform\u00e9ment au projet initial, l\u2019ensemble de ces 66 appareils devrait \u00eatre\nlivr\u00e9 avant la fin 2024. Selon le projet du minist\u00e8re, les chasseurs F-16V nouvellement achet\u00e9s seront\nstationn\u00e9s sur la base de l\u2019arm\u00e9e de l\u2019air de Taitung, dans le sud-est de Ta\u00efwan. L'arm\u00e9e d\u00e9clare avoir\nachev\u00e9 la construction des infrastructures et les ajustements organisationnels. La mission d\u2019origine\nd\u2019entra\u00eenement au vol a \u00e9t\u00e9 transf\u00e9r\u00e9e \u00e0 Gangshan, Kaohsiung. Selon le budget de 2024, l\u2019arm\u00e9e de\nl\u2019air pr\u00e9voit d'envoyer 65 officiers et soldats aux \u00c9tats-Unis pour une formation tactique entre janvier etd\u00e9cembre, avec un budget de 39,59 millions de dollars ta\u00efwanais (soit plus de 1,1 million d\u2019euros). Ce\nnombre d\u00e9passe les 50 militaires envoy\u00e9s au total durant les trois ann\u00e9es pr\u00e9c\u00e9dentes.",
         "title": "\u2026\n\nLes avions de combat F-16V command\u00e9s par Ta\u00efwan devraient \u00eatre livr\u00e9s avant la fin 2024"
     },
     {
         "identifier": "1312-22",
         "metadata": {
             "ARTICLE DATE": "04-01-2024",
             "PUBLICATION DATE": "7 janvier 2024",
             "PUBLICATION NUMBER": "1312",
-            "SOURCE NAME": "Radio Ta\u00efwan international"
+            "SOURCE NAME": "Radio Ta\u00efwan international",
+            "TOPIC": "L'ACTUALIT\u00c9 DES MARCHANDS D'ARMES"
         },
         "text": "Ta\u00efwan  en  passe  d\u2019acheter  \u00e0  la  France  des  composants  de  missiles  air-air  destin\u00e9s  \u00e0  ses\nMirage 2000...\nLe gouvernement ta\u00efwanais s'est engag\u00e9 \u00e0 acheter des parties et des composants de missiles air-air \u00e0\nla France pour \u00e9quiper la flotte ta\u00efwanaise de Mirage 2000, un contrat d'un montant de 396,8 millions\nde dollars ta\u00efwanais, soit environ 11,7 millions d'euros. Le minist\u00e8re de la D\u00e9fense ta\u00efwanais a post\u00e9\nhier une note sur le syst\u00e8me d'approvisionnement en ligne du gouvernement qui indique le r\u00e9sultat d'un\nprocessus d'offre limit\u00e9 pour des parties et des composants de missiles. Le document officiel d\u2019appel\nd\u2019offres indique que la soci\u00e9t\u00e9 MBDA a remport\u00e9 l'offre. MBDA Missile Systems est une filiale d'Airbus\net  un  leader  europ\u00e9en dans la  conception  de missiles  et  de  syst\u00e8mes de missiles.  Il  est  indiqu\u00e9\nqu'agence comp\u00e9tente, l'arm\u00e9e de l'air de la R\u00e9publique de Chine, sera livr\u00e9e entre janvier 2024 et\nd\u00e9cembre 2028 \u00e0 Hsinchu.",
         "title": "Ta\u00efwan  en  passe  d\u2019acheter  \u00e0  la  France  des  composants  de  missiles  air-air  destin\u00e9s  \u00e0  ses\nMirage 2000"
     },
     {
         "identifier": "1312-23",
         "metadata": {
             "ARTICLE DATE": "02-01-2024",
             "PUBLICATION DATE": "7 janvier 2024",
             "PUBLICATION NUMBER": "1312",
-            "SOURCE NAME": "Radio Prague international"
+            "SOURCE NAME": "Radio Prague international",
+            "TOPIC": "L'ACTUALIT\u00c9 DES MARCHANDS D'ARMES"
         },
         "text": "Plus d\u2019un millier de pistolets-mitrailleurs tch\u00e8ques command\u00e9s par la police espagnole...\n\u00c0 la fin de l\u2019ann\u00e9e 2023, la police espagnole a conclu un troisi\u00e8me contrat en deux ans pour l\u2019achat de\npistolets-mitrailleurs Scorpion fabriqu\u00e9s par le fabricant d\u2019armes tch\u00e8que Ceska zbrojovka. Selon le site\nweb  espagnol  Infodefensa,  la  police  fait  l\u2019acquisition  d\u2019au  moins  1 250 pistolets-mitrailleurs  CZ\nScorpion EVO3 A1 pour un montant de 2,141 millions d\u2019euros. La police espagnole a ainsi d\u00e9j\u00e0 achet\u00e9\nenviron 2 000 pistolets-mitrailleurs depuis la fin 2021. Le fabricant d\u2019armes tch\u00e8que Ceska zbrojovka\nfait partie du holding Colt CZ, l\u2019un des principaux fabricants mondiaux d'armes l\u00e9g\u00e8res destin\u00e9es aux\nforces arm\u00e9es, \u00e0 la d\u00e9fense personnelle, \u00e0 la chasse, au tir sportif et \u00e0 d\u2019autres usages commerciaux.\nLe groupe a son si\u00e8ge en Tch\u00e9quie et poss\u00e8de des sites de production en R\u00e9publique tch\u00e8que, aux\n\u00c9tats-Unis, au Canada et en Su\u00e8de. Il emploie plus de 2 000 personnes.",
         "title": "Plus d\u2019un millier de pistolets-mitrailleurs tch\u00e8ques command\u00e9s par la police espagnole"
     },
     {
         "identifier": "1312-24",
         "metadata": {
             "ARTICLE DATE": "04-01-2024",
             "PUBLICATION DATE": "7 janvier 2024",
             "PUBLICATION NUMBER": "1312",
-            "SOURCE NAME": "Radio Roumanie international"
+            "SOURCE NAME": "Radio Roumanie international",
+            "TOPIC": "L'ACTUALIT\u00c9 DES MARCHANDS D'ARMES"
         },
         "text": "L\u2019OTAN va soutenir l\u2019achat d\u2019un millier de missiles Patriot destin\u00e9s \u00e0 ses membres...\nL'OTAN a annonc\u00e9 que son Agence de soutien et d'acquisitions offrirait son soutien \u00e0 un groupe d\u2019\u00c9tats\nmembres, y compris l'Allemagne, les Pays-Bas, la Roumanie et l'Espagne, pour l'achat d'un millier de\nmissiles de d\u00e9fense antia\u00e9rienne  Patriot. Selon un communiqu\u00e9 de l'alliance militaire. \u00ab L'acquisition\nmultinationale consolid\u00e9e, dans l'esprit de l'Initiative bouclier du ciel europ\u00e9en (European Sky Shield\nInitiative) permet de r\u00e9aliser des \u00e9conomies et de soutenir l'expansion de la capacit\u00e9 de production des\nnouveaux missiles GEM-T afin de r\u00e9pondre \u00e0 la demande croissante \u00bb. L'agence a attribu\u00e9 le contrat,\nd'une valeur de 5,5 milliards de dollars, \u00e0 COMLOG, une joint-venture entre une entreprise am\u00e9ricaine\net une autre allemande. Les missiles Patriot co\u00fbtent presque 4 millions de dollars chacun et le contrat\ncouvre aussi la fourniture de pi\u00e8ces d'\u00e9change et l'entretien. Le secr\u00e9taire g\u00e9n\u00e9ral de l'OTAN, Jens\nStoltenberg, a soulign\u00e9 qu'il \u00e9tait essentiel d'intensifier la production de munitions pour la s\u00e9curit\u00e9 des\n\u00c9tats alli\u00e9s et de l'Ukraine.",
         "title": "L\u2019OTAN va soutenir l\u2019achat d\u2019un millier de missiles Patriot destin\u00e9s \u00e0 ses membres"
     },
     {
         "identifier": "1312-25",
         "metadata": {
             "ARTICLE DATE": "05-01-2024",
             "PUBLICATION DATE": "7 janvier 2024",
             "PUBLICATION NUMBER": "1312",
-            "SOURCE NAME": "Radio Vatican"
+            "SOURCE NAME": "Radio Vatican",
+            "TOPIC": "L'ACTUALIT\u00c9 DES MARCHANDS D'ARMES"
         },
         "text": "Des missiles balistiques nord-cor\u00e9ens auraient \u00e9t\u00e9 utilis\u00e9s par la Russie contre l\u2019Ukraine selon\nla Maison-Blanche...\nLa Maison-Blanche affirme que des missiles fournis par Pyongyang \u00e0 Moscou ont \u00e9t\u00e9 utilis\u00e9s lors des\nattaques  d\u2019envergure  ces  derniers  jours  en  Ukraine,  pr\u00e9cis\u00e9ment  des  syst\u00e8mes  de  lancement  de\nmissiles  balistiques  et  plusieurs  missiles  balistiques.  Selon  le  porte-parole  du  Conseil  de  s\u00e9curit\u00e9\nnationale am\u00e9ricain, ce transfert d\u2019armement souligne le besoin pour le Congr\u00e8s am\u00e9ricain d\u2019approuver\nun nouveau paquet d\u2019aide militaire \u00e0 l\u2019Ukraine.",
         "title": "Des missiles balistiques nord-cor\u00e9ens auraient \u00e9t\u00e9 utilis\u00e9s par la Russie contre l\u2019Ukraine selon\nla Maison-Blanche"
     },
     {
         "identifier": "1312-26",
         "metadata": {
             "ARTICLE DATE": "05-01-2024",
             "PUBLICATION DATE": "7 janvier 2024",
             "PUBLICATION NUMBER": "1312",
-            "SOURCE NAME": "La voix de l\u2019Am\u00e9rique"
+            "SOURCE NAME": "La voix de l\u2019Am\u00e9rique",
+            "TOPIC": "L'ACTUALIT\u00c9 DES MARCHANDS D'ARMES"
         },
         "text": "Livraison de drones turcs \u00e0 la junte au pouvoir au Mali...\nAu Mali, les militaires au pouvoir ont r\u00e9ceptionn\u00e9 jeudi une livraison de drones de Turquie lors d\u2019une\nc\u00e9r\u00e9monie en pr\u00e9sence du chef de la junte, le colonel Assimi Go\u00efta. De fabrication turque, ces drones\npermettent de surveiller le territoire national, de d\u00e9tecter des cibles suspectes, de les traquer et de les\nfrapper  au besoin avec une pr\u00e9cision chirurgicale,  a  dit  dans un discours le  ma\u00eetre  de c\u00e9r\u00e9monies\u2019exprimant au nom de l\u2019\u00e9tat-major de l\u2019arm\u00e9e de l\u2019air.",
         "title": "Livraison de drones turcs \u00e0 la junte au pouvoir au Mali"
     },
     {
         "identifier": "1312-27",
         "metadata": {
             "ARTICLE DATE": "02-01-2024",
             "PUBLICATION DATE": "7 janvier 2024",
             "PUBLICATION NUMBER": "1312",
-            "SOURCE NAME": "Radio Japon international"
+            "SOURCE NAME": "Radio Japon international",
+            "TOPIC": "CYBERESPACE"
         },
         "text": "\u2026\n\nLe Japon met en garde contre les Fake News diffus\u00e9es apr\u00e8s le s\u00e9isme ayant frapp\u00e9 le centre du\npays...\nDes informations trompeuses ou fausses ont \u00e9t\u00e9 diffus\u00e9es sur internet concernant le tremblement de\nterre et le tsunami qui ont frapp\u00e9 le centre du Japon lundi. Juste apr\u00e8s le s\u00e9isme, des vid\u00e9os semblant\nmontrer les d\u00e9g\u00e2ts, ainsi que des demandes de secours de personnes affirmant \u00eatre coinc\u00e9es sous des\nb\u00e2timents  effondr\u00e9s,  ont  \u00e9t\u00e9  publi\u00e9es  sur  X,  la  plateforme anciennement  connue sous le  nom de\nTwitter.  La  NHK a  confirm\u00e9  que  certains  messages  contenaient  de  fausses  informations.  Des\nmessages appelant \u00e0 l\u2019aide mentionnaient des adresses inexistantes ou incluaient des vid\u00e9os sans\nrapport  avec les \u00e9v\u00e8nements de lundi.  Certaines images \u00e9taient celles du tsunami de 2011, qui  a\nfrapp\u00e9 l'est du Japon apr\u00e8s un puissant s\u00e9isme. L\u2019une de ces publications a \u00e9t\u00e9 consult\u00e9e plus d\u2019un\nmillion de fois. D'autres messages contiennent des informations infond\u00e9es sur les causes du s\u00e9isme et\nde l'incendie dans la ville de Wajima, ainsi que sur la centrale nucl\u00e9aire de Shika, toutes deux situ\u00e9es\ndans le d\u00e9partement d'Ishikawa. Un compte a lanc\u00e9 un appel aux dons en monnaie num\u00e9rique, l'auteur\naffirmant  avoir  \u00e9t\u00e9  touch\u00e9 par  la  catastrophe.  Les  fausses nouvelles  ont  tendance \u00e0  se  propager\nfacilement  au  moment  d\u2019une  catastrophe,  alors  que  de  nombreuses  personnes  recherchent  des\ninformations.  Elles peuvent semer la confusion dans les zones touch\u00e9es et  entraver les efforts de\nsecours. Les internautes sont exhort\u00e9s \u00e0 v\u00e9rifier l\u2019authenticit\u00e9 des informations ou des m\u00e9dias avant de\nles republier.",
         "title": "\u2026\n\nLe Japon met en garde contre les Fake News diffus\u00e9es apr\u00e8s le s\u00e9isme ayant frapp\u00e9 le centre du\npays"
     }
 ]
```

### Comparing `pyprocessors_segment_renseignor-0.5.4/tests/data/renseignor-document-test.json` & `pyprocessors_segment_renseignor-0.5.8/tests/data/renseignor-document-test.json`

 * *Files identical despite different names*

### Comparing `pyprocessors_segment_renseignor-0.5.4/tests/test_segment_renseignor.py` & `pyprocessors_segment_renseignor-0.5.8/tests/test_segment_renseignor.py`

 * *Files identical despite different names*

### Comparing `pyprocessors_segment_renseignor-0.5.4/tox.ini` & `pyprocessors_segment_renseignor-0.5.8/tox.ini`

 * *Files identical despite different names*

### Comparing `pyprocessors_segment_renseignor-0.5.4/setup.py` & `pyprocessors_segment_renseignor-0.5.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
           'dirty-equals']}
 
 entry_points = \
 {'pyprocessors.plugins': ['segment_renseignor = '
                           'pyprocessors_segment_renseignor.segment_renseignor:SegmentRenseignorProcessor']}
 
 setup(name='pyprocessors-segment_renseignor',
-      version='0.5.4',
+      version='0.5.8',
       description='Sherpa Consolidation processor',
       author='Olivier Terrier',
       author_email='olivier.terrier@kairntech.com',
       url='https://github.com/oterrier/pyprocessors_segment_renseignor/',
       packages=packages,
       package_data=package_data,
       package_dir=package_dir,
```

### Comparing `pyprocessors_segment_renseignor-0.5.4/PKG-INFO` & `pyprocessors_segment_renseignor-0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprocessors-segment_renseignor
-Version: 0.5.4
+Version: 0.5.8
 Summary: Sherpa Consolidation processor
 Home-page: https://github.com/oterrier/pyprocessors_segment_renseignor/
 Keywords: 
 Author: Olivier Terrier
 Author-email: olivier.terrier@kairntech.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

