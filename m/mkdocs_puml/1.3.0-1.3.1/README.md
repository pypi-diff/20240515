# Comparing `tmp/mkdocs_puml-1.3.0.tar.gz` & `tmp/mkdocs_puml-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_puml-1.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mkdocs_puml-1.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mkdocs_puml-1.3.0.tar` & `mkdocs_puml-1.3.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      237 2022-09-15 12:01:38.953711 mkdocs_puml-1.3.0/.coveragerc
--rw-r--r--   0        0        0    31089 2023-01-25 09:20:39.582596 mkdocs_puml-1.3.0/.docs/logo.png
--rw-r--r--   0        0        0       43 2022-09-15 12:01:38.953802 mkdocs_puml-1.3.0/.flake8
--rw-r--r--   0        0        0      655 2023-01-25 09:42:12.642417 mkdocs_puml-1.3.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2022-11-13 12:18:46.573988 mkdocs_puml-1.3.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1284 2024-01-02 10:06:29.414708 mkdocs_puml-1.3.0/.github/workflows/checks.yml
--rw-r--r--   0        0        0     5494 2023-07-30 09:50:18.334236 mkdocs_puml-1.3.0/.gitignore
--rw-r--r--   0        0        0      404 2024-01-02 10:06:29.415474 mkdocs_puml-1.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      220 2023-07-30 09:50:18.334890 mkdocs_puml-1.3.0/.vscode/settings.json
--rw-r--r--   0        0        0     1082 2022-09-15 12:01:38.954367 mkdocs_puml-1.3.0/LICENSE
--rw-r--r--   0        0        0      581 2024-01-02 10:06:29.415940 mkdocs_puml-1.3.0/Pipfile
--rw-r--r--   0        0        0    79073 2024-04-05 14:23:42.978809 mkdocs_puml-1.3.0/Pipfile.lock
--rw-r--r--   0        0        0     4005 2024-04-05 14:07:33.659657 mkdocs_puml-1.3.0/README.md
--rw-r--r--   0        0        0       68 2024-04-05 14:06:58.394749 mkdocs_puml-1.3.0/mkdocs_puml/__init__.py
--rw-r--r--   0        0        0      948 2023-02-18 11:50:55.936744 mkdocs_puml-1.3.0/mkdocs_puml/encoder.py
--rw-r--r--   0        0        0     5370 2024-04-05 14:15:19.574845 mkdocs_puml-1.3.0/mkdocs_puml/plugin.py
--rw-r--r--   0        0        0     4054 2024-04-05 14:05:29.674877 mkdocs_puml-1.3.0/mkdocs_puml/puml.py
--rw-r--r--   0        0        0      628 2024-01-02 09:06:43.936369 mkdocs_puml-1.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-09-15 12:01:38.956165 mkdocs_puml-1.3.0/tests/__init__.py
--rw-r--r--   0        0        0      866 2023-03-22 10:02:51.667442 mkdocs_puml-1.3.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2022-09-20 17:56:58.447859 mkdocs_puml-1.3.0/tests/plugins/__init__.py
--rw-r--r--   0        0        0     2374 2023-06-28 09:10:05.717513 mkdocs_puml-1.3.0/tests/plugins/conftest.py
--rw-r--r--   0        0        0     2247 2023-06-28 09:10:05.717746 mkdocs_puml-1.3.0/tests/plugins/test_plugin.py
--rw-r--r--   0        0        0      197 2022-09-15 12:01:38.956431 mkdocs_puml-1.3.0/tests/test_encoder.py
--rw-r--r--   0        0        0      876 2023-01-25 09:21:05.750584 mkdocs_puml-1.3.0/tests/test_puml.py
--rw-r--r--   0        0        0     1074 2023-03-22 10:02:51.667954 mkdocs_puml-1.3.0/tests/testdata/markdown.md
--rw-r--r--   0        0        0      375 2022-09-20 17:56:58.448279 mkdocs_puml-1.3.0/tests/testdata/output.html
--rw-r--r--   0        0        0     2255 2022-09-15 12:01:38.956767 mkdocs_puml-1.3.0/tests/testdata/plantuml.svg
--rw-r--r--   0        0        0     4458 1970-01-01 00:00:00.000000 mkdocs_puml-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      237 2022-09-15 12:01:38.953711 mkdocs_puml-1.3.1/.coveragerc
+-rw-r--r--   0        0        0    31089 2023-01-25 09:20:39.582596 mkdocs_puml-1.3.1/.docs/logo.png
+-rw-r--r--   0        0        0       43 2022-09-15 12:01:38.953802 mkdocs_puml-1.3.1/.flake8
+-rw-r--r--   0        0        0      655 2023-01-25 09:42:12.642417 mkdocs_puml-1.3.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2022-11-13 12:18:46.573988 mkdocs_puml-1.3.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1284 2024-01-02 10:06:29.414708 mkdocs_puml-1.3.1/.github/workflows/checks.yml
+-rw-r--r--   0        0        0     5494 2023-07-30 09:50:18.334236 mkdocs_puml-1.3.1/.gitignore
+-rw-r--r--   0        0        0      404 2024-01-02 10:06:29.415474 mkdocs_puml-1.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      220 2023-07-30 09:50:18.334890 mkdocs_puml-1.3.1/.vscode/settings.json
+-rw-r--r--   0        0        0     1082 2022-09-15 12:01:38.954367 mkdocs_puml-1.3.1/LICENSE
+-rw-r--r--   0        0        0      581 2024-01-02 10:06:29.415940 mkdocs_puml-1.3.1/Pipfile
+-rw-r--r--   0        0        0    78484 2024-05-15 13:12:52.453333 mkdocs_puml-1.3.1/Pipfile.lock
+-rw-r--r--   0        0        0     4005 2024-05-15 13:12:52.454281 mkdocs_puml-1.3.1/README.md
+-rw-r--r--   0        0        0       68 2024-05-15 13:12:52.454641 mkdocs_puml-1.3.1/mkdocs_puml/__init__.py
+-rw-r--r--   0        0        0      948 2023-02-18 11:50:55.936744 mkdocs_puml-1.3.1/mkdocs_puml/encoder.py
+-rw-r--r--   0        0        0     5396 2024-05-15 13:12:52.455371 mkdocs_puml-1.3.1/mkdocs_puml/plugin.py
+-rw-r--r--   0        0        0     4054 2024-05-15 13:12:52.455860 mkdocs_puml-1.3.1/mkdocs_puml/puml.py
+-rw-r--r--   0        0        0      628 2024-01-02 09:06:43.936369 mkdocs_puml-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-09-15 12:01:38.956165 mkdocs_puml-1.3.1/tests/__init__.py
+-rw-r--r--   0        0        0      866 2023-03-22 10:02:51.667442 mkdocs_puml-1.3.1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2022-09-20 17:56:58.447859 mkdocs_puml-1.3.1/tests/plugins/__init__.py
+-rw-r--r--   0        0        0     2374 2023-06-28 09:10:05.717513 mkdocs_puml-1.3.1/tests/plugins/conftest.py
+-rw-r--r--   0        0        0     2247 2023-06-28 09:10:05.717746 mkdocs_puml-1.3.1/tests/plugins/test_plugin.py
+-rw-r--r--   0        0        0      197 2022-09-15 12:01:38.956431 mkdocs_puml-1.3.1/tests/test_encoder.py
+-rw-r--r--   0        0        0      876 2023-01-25 09:21:05.750584 mkdocs_puml-1.3.1/tests/test_puml.py
+-rw-r--r--   0        0        0     1074 2023-03-22 10:02:51.667954 mkdocs_puml-1.3.1/tests/testdata/markdown.md
+-rw-r--r--   0        0        0      375 2022-09-20 17:56:58.448279 mkdocs_puml-1.3.1/tests/testdata/output.html
+-rw-r--r--   0        0        0     2255 2022-09-15 12:01:38.956767 mkdocs_puml-1.3.1/tests/testdata/plantuml.svg
+-rw-r--r--   0        0        0     4458 1970-01-01 00:00:00.000000 mkdocs_puml-1.3.1/PKG-INFO
```

### Comparing `mkdocs_puml-1.3.0/.docs/logo.png` & `mkdocs_puml-1.3.1/.docs/logo.png`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.3.0/.github/ISSUE_TEMPLATE/bug_report.md` & `mkdocs_puml-1.3.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.3.0/.github/ISSUE_TEMPLATE/feature_request.md` & `mkdocs_puml-1.3.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.3.0/.github/workflows/checks.yml` & `mkdocs_puml-1.3.1/.github/workflows/checks.yml`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.3.0/.gitignore` & `mkdocs_puml-1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.3.0/LICENSE` & `mkdocs_puml-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.3.0/Pipfile` & `mkdocs_puml-1.3.1/Pipfile`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.3.0/Pipfile.lock` & `mkdocs_puml-1.3.1/Pipfile.lock`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9744161522633745%*

 * *Differences: {"'default'": "{'docutils': {'hashes': "*

 * *              "['sha256:3a6b18732edf182daa3cd12775bbb338cf5691468f91eeeb109deff6ebfa986f', "*

 * *              "'sha256:dafca5b9e384f0e419294eb4d2ff9fa826435bf15f15b7bd45723e8ad76811b2'], "*

 * *              '\'markers\': "python_version >= \'3.9\'", \'version\': \'==0.21.2\'}, \'idna\': '*

 * *              "{'hashes': "*

 * *              "['sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc', "*

 * *              "'sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427 […]*

```diff
@@ -126,19 +126,19 @@
                 "sha256:ca9853ad459e787e2192211578cc907e7594e294c7ccc834310722b41b9ca6de"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==8.1.7"
         },
         "docutils": {
             "hashes": [
-                "sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6",
-                "sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b"
+                "sha256:3a6b18732edf182daa3cd12775bbb338cf5691468f91eeeb109deff6ebfa986f",
+                "sha256:dafca5b9e384f0e419294eb4d2ff9fa826435bf15f15b7bd45723e8ad76811b2"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==0.20.1"
+            "markers": "python_version >= '3.9'",
+            "version": "==0.21.2"
         },
         "flit": {
             "hashes": [
                 "sha256:076c3aaba5ac24cf0ad3251f910900d95a08218e6bcb26f21fef1036cc4679ca",
                 "sha256:d75edf5eb324da20d53570a6a6f87f51e606eee8384925cd66a90611140844c7"
             ],
             "index": "pypi",
@@ -158,27 +158,27 @@
                 "sha256:8337dd7b50877f163d4c0289bc1f1c7f127550241988d568c1db512c4324a619",
                 "sha256:9c535c4c61193c2df8871222567d7fd7e5014d835f97dc7b7439069e2413d343"
             ],
             "version": "==2.1.0"
         },
         "idna": {
             "hashes": [
-                "sha256:9ecdbbd083b06798ae1e86adcbfe8ab1479cf864e4ee30fe4e46a003d12491ca",
-                "sha256:c05567e9c24a6b9faaa835c4821bad0590fbb9d5779e7caa6e1cc4978e7eb24f"
+                "sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc",
+                "sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0"
             ],
             "markers": "python_version >= '3.5'",
-            "version": "==3.6"
+            "version": "==3.7"
         },
         "jinja2": {
             "hashes": [
-                "sha256:7d6d50dd97d52cbc355597bd845fabfbac3f551e1f99619e39a35ce8c370b5fa",
-                "sha256:ac8bd6544d4bb2c9792bf3a159e80bba8fda7f07e81bc3aed565432d5925ba90"
+                "sha256:4a3aee7acbbe7303aede8e9648d13b8bf88a429282aa6122a993f0ac800cb369",
+                "sha256:bc5dd2abb727a5319567b7a813e6a2e7318c39f4f487cfe6c89c6f9c7d25197d"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.1.3"
+            "version": "==3.1.4"
         },
         "markdown": {
             "hashes": [
                 "sha256:48f276f4d8cfb8ce6527c8f79e2ee29708508bf4d40aa410fbc3b4ee832c850f",
                 "sha256:ed4f41f6daecbeeb96e576ce414c41d2d876daa9a16cb35fa8ed8c2ddfad0224"
             ],
             "markers": "python_version >= '3.8'",
@@ -256,20 +256,28 @@
                 "sha256:70775750742b25c0d8f36c55aed03d24c3384d17c951b3175d898bd778ef0307"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.3.4"
         },
         "mkdocs": {
             "hashes": [
-                "sha256:3b3a78e736b31158d64dbb2f8ba29bd46a379d0c6e324c2246c3bc3d2189cfc1",
-                "sha256:eb7c99214dcb945313ba30426c2451b735992c73c2e10838f76d09e39ff4d0e2"
+                "sha256:1eb5cb7676b7d89323e62b56235010216319217d4af5ddc543a91beb8d125ea7",
+                "sha256:a73f735824ef83a4f3bcb7a231dcab23f5a838f88b7efc54a0eef5fbdbc3c512"
             ],
             "index": "pypi",
-            "markers": "python_version >= '3.7'",
-            "version": "==1.5.3"
+            "markers": "python_version >= '3.8'",
+            "version": "==1.6.0"
+        },
+        "mkdocs-get-deps": {
+            "hashes": [
+                "sha256:162b3d129c7fad9b19abfdcb9c1458a651628e4b1dea628ac68790fb3061c60c",
+                "sha256:2bf11d0b133e77a0dd036abeeb06dec8775e46efa526dc70667d8863eefc6134"
+            ],
+            "markers": "python_version >= '3.8'",
+            "version": "==0.2.0"
         },
         "packaging": {
             "hashes": [
                 "sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5",
                 "sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9"
             ],
             "markers": "python_version >= '3.7'",
@@ -281,19 +289,19 @@
                 "sha256:a482d51503a1ab33b1c67a6c3813a26953dbdc71c31dacaef9a838c4e29f5712"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==0.12.1"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:0614df2a2f37e1a662acbd8e2b25b92ccf8632929bc6d43467e17fe89c75e068",
-                "sha256:ef0cc731df711022c174543cb70a9b5bd22e5a9337c8624ef2c2ceb8ddad8768"
+                "sha256:2d7a1657e36a80ea911db832a8a6ece5ee53d8de21edd5cc5879af6530b1bfee",
+                "sha256:38b7b51f512eed9e84a22788b4bce1de17c0adb134d6becb09836e37d8654cd3"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==4.2.0"
+            "version": "==4.2.2"
         },
         "python-dateutil": {
             "hashes": [
                 "sha256:37dd54208da7e1cd875388217d5e00ebd4179249f90fb72437e91a35459a0ad3",
                 "sha256:a8b2bc7bffae282281c8140a97d3aa9c14da0b136dfe83f850eea9a5f7470427"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
@@ -432,19 +440,19 @@
             "markers": "python_version >= '3.8'",
             "version": "==4.0.0"
         }
     },
     "develop": {
         "babel": {
             "hashes": [
-                "sha256:6919867db036398ba21eb5c7a0f6b28ab8cbc3ae7a73a44ebe34ae74a4e7d363",
-                "sha256:efb1a25b7118e67ce3a259bed20545c29cb68be8ad2c784c83689981b7a57287"
+                "sha256:08706bdad8d0a3413266ab61bd6c34d0c28d6e1e7badf40a2cebe67644e2e1fb",
+                "sha256:8daf0e265d05768bc6c7a314cf1321e9a123afc328cc635c18622a2f30a04413"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==2.14.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==2.15.0"
         },
         "bracex": {
             "hashes": [
                 "sha256:a27eaf1df42cf561fed58b7a8f3fdf129d1ea16a81e1fadd1d17989bc6384beb",
                 "sha256:efdc71eff95eaff5e0f8cfebe7d01adf2c8637c8c92edaf63ef348c241a82418"
             ],
             "markers": "python_version >= '3.8'",
@@ -579,87 +587,87 @@
             "version": "==0.4.6"
         },
         "coverage": {
             "extras": [
                 "toml"
             ],
             "hashes": [
-                "sha256:00838a35b882694afda09f85e469c96367daa3f3f2b097d846a7216993d37f4c",
-                "sha256:0513b9508b93da4e1716744ef6ebc507aff016ba115ffe8ecff744d1322a7b63",
-                "sha256:09c3255458533cb76ef55da8cc49ffab9e33f083739c8bd4f58e79fecfe288f7",
-                "sha256:09ef9199ed6653989ebbcaacc9b62b514bb63ea2f90256e71fea3ed74bd8ff6f",
-                "sha256:09fa497a8ab37784fbb20ab699c246053ac294d13fc7eb40ec007a5043ec91f8",
-                "sha256:0f9f50e7ef2a71e2fae92774c99170eb8304e3fdf9c8c3c7ae9bab3e7229c5cf",
-                "sha256:137eb07173141545e07403cca94ab625cc1cc6bc4c1e97b6e3846270e7e1fea0",
-                "sha256:1f384c3cc76aeedce208643697fb3e8437604b512255de6d18dae3f27655a384",
-                "sha256:201bef2eea65e0e9c56343115ba3814e896afe6d36ffd37bab783261db430f76",
-                "sha256:38dd60d7bf242c4ed5b38e094baf6401faa114fc09e9e6632374388a404f98e7",
-                "sha256:3b799445b9f7ee8bf299cfaed6f5b226c0037b74886a4e11515e569b36fe310d",
-                "sha256:3ea79bb50e805cd6ac058dfa3b5c8f6c040cb87fe83de10845857f5535d1db70",
-                "sha256:40209e141059b9370a2657c9b15607815359ab3ef9918f0196b6fccce8d3230f",
-                "sha256:41c9c5f3de16b903b610d09650e5e27adbfa7f500302718c9ffd1c12cf9d6818",
-                "sha256:54eb8d1bf7cacfbf2a3186019bcf01d11c666bd495ed18717162f7eb1e9dd00b",
-                "sha256:598825b51b81c808cb6f078dcb972f96af96b078faa47af7dfcdf282835baa8d",
-                "sha256:5fc1de20b2d4a061b3df27ab9b7c7111e9a710f10dc2b84d33a4ab25065994ec",
-                "sha256:623512f8ba53c422fcfb2ce68362c97945095b864cda94a92edbaf5994201083",
-                "sha256:690db6517f09336559dc0b5f55342df62370a48f5469fabf502db2c6d1cffcd2",
-                "sha256:69eb372f7e2ece89f14751fbcbe470295d73ed41ecd37ca36ed2eb47512a6ab9",
-                "sha256:73bfb9c09951125d06ee473bed216e2c3742f530fc5acc1383883125de76d9cd",
-                "sha256:742a76a12aa45b44d236815d282b03cfb1de3b4323f3e4ec933acfae08e54ade",
-                "sha256:7c95949560050d04d46b919301826525597f07b33beba6187d04fa64d47ac82e",
-                "sha256:8130a2aa2acb8788e0b56938786c33c7c98562697bf9f4c7d6e8e5e3a0501e4a",
-                "sha256:8a2b2b78c78293782fd3767d53e6474582f62443d0504b1554370bde86cc8227",
-                "sha256:8ce1415194b4a6bd0cdcc3a1dfbf58b63f910dcb7330fe15bdff542c56949f87",
-                "sha256:9ca28a302acb19b6af89e90f33ee3e1906961f94b54ea37de6737b7ca9d8827c",
-                "sha256:a4cdc86d54b5da0df6d3d3a2f0b710949286094c3a6700c21e9015932b81447e",
-                "sha256:aa5b1c1bfc28384f1f53b69a023d789f72b2e0ab1b3787aae16992a7ca21056c",
-                "sha256:aadacf9a2f407a4688d700e4ebab33a7e2e408f2ca04dbf4aef17585389eff3e",
-                "sha256:ae71e7ddb7a413dd60052e90528f2f65270aad4b509563af6d03d53e979feafd",
-                "sha256:b14706df8b2de49869ae03a5ccbc211f4041750cd4a66f698df89d44f4bd30ec",
-                "sha256:b1a93009cb80730c9bca5d6d4665494b725b6e8e157c1cb7f2db5b4b122ea562",
-                "sha256:b2991665420a803495e0b90a79233c1433d6ed77ef282e8e152a324bbbc5e0c8",
-                "sha256:b2c5edc4ac10a7ef6605a966c58929ec6c1bd0917fb8c15cb3363f65aa40e677",
-                "sha256:b4d33f418f46362995f1e9d4f3a35a1b6322cb959c31d88ae56b0298e1c22357",
-                "sha256:b91cbc4b195444e7e258ba27ac33769c41b94967919f10037e6355e998af255c",
-                "sha256:c74880fc64d4958159fbd537a091d2a585448a8f8508bf248d72112723974cbd",
-                "sha256:c901df83d097649e257e803be22592aedfd5182f07b3cc87d640bbb9afd50f49",
-                "sha256:cac99918c7bba15302a2d81f0312c08054a3359eaa1929c7e4b26ebe41e9b286",
-                "sha256:cc4f1358cb0c78edef3ed237ef2c86056206bb8d9140e73b6b89fbcfcbdd40e1",
-                "sha256:ccd341521be3d1b3daeb41960ae94a5e87abe2f46f17224ba5d6f2b8398016cf",
-                "sha256:ce4b94265ca988c3f8e479e741693d143026632672e3ff924f25fab50518dd51",
-                "sha256:cf271892d13e43bc2b51e6908ec9a6a5094a4df1d8af0bfc360088ee6c684409",
-                "sha256:d5ae728ff3b5401cc320d792866987e7e7e880e6ebd24433b70a33b643bb0384",
-                "sha256:d71eec7d83298f1af3326ce0ff1d0ea83c7cb98f72b577097f9083b20bdaf05e",
-                "sha256:d898fe162d26929b5960e4e138651f7427048e72c853607f2b200909794ed978",
-                "sha256:d89d7b2974cae412400e88f35d86af72208e1ede1a541954af5d944a8ba46c57",
-                "sha256:dfa8fe35a0bb90382837b238fff375de15f0dcdb9ae68ff85f7a63649c98527e",
-                "sha256:e0be5efd5127542ef31f165de269f77560d6cdef525fffa446de6f7e9186cfb2",
-                "sha256:fdfafb32984684eb03c2d83e1e51f64f0906b11e64482df3c5db936ce3839d48",
-                "sha256:ff7687ca3d7028d8a5f0ebae95a6e4827c5616b31a4ee1192bdfde697db110d4"
+                "sha256:0646599e9b139988b63704d704af8e8df7fa4cbc4a1f33df69d97f36cb0a38de",
+                "sha256:0cdcbc320b14c3e5877ee79e649677cb7d89ef588852e9583e6b24c2e5072661",
+                "sha256:0d0a0f5e06881ecedfe6f3dd2f56dcb057b6dbeb3327fd32d4b12854df36bf26",
+                "sha256:1434e088b41594baa71188a17533083eabf5609e8e72f16ce8c186001e6b8c41",
+                "sha256:16db7f26000a07efcf6aea00316f6ac57e7d9a96501e990a36f40c965ec7a95d",
+                "sha256:1cc0fe9b0b3a8364093c53b0b4c0c2dd4bb23acbec4c9240b5f284095ccf7981",
+                "sha256:1fc81d5878cd6274ce971e0a3a18a8803c3fe25457165314271cf78e3aae3aa2",
+                "sha256:2ec92012fefebee89a6b9c79bc39051a6cb3891d562b9270ab10ecfdadbc0c34",
+                "sha256:39afcd3d4339329c5f58de48a52f6e4e50f6578dd6099961cf22228feb25f38f",
+                "sha256:4a7b0ceee8147444347da6a66be737c9d78f3353b0681715b668b72e79203e4a",
+                "sha256:4a9ca3f2fae0088c3c71d743d85404cec8df9be818a005ea065495bedc33da35",
+                "sha256:4bf0655ab60d754491004a5efd7f9cccefcc1081a74c9ef2da4735d6ee4a6223",
+                "sha256:4cc37def103a2725bc672f84bd939a6fe4522310503207aae4d56351644682f1",
+                "sha256:4fc84a37bfd98db31beae3c2748811a3fa72bf2007ff7902f68746d9757f3746",
+                "sha256:5037f8fcc2a95b1f0e80585bd9d1ec31068a9bcb157d9750a172836e98bc7a90",
+                "sha256:54de9ef3a9da981f7af93eafde4ede199e0846cd819eb27c88e2b712aae9708c",
+                "sha256:556cf1a7cbc8028cb60e1ff0be806be2eded2daf8129b8811c63e2b9a6c43bca",
+                "sha256:57e0204b5b745594e5bc14b9b50006da722827f0b8c776949f1135677e88d0b8",
+                "sha256:5a5740d1fb60ddf268a3811bcd353de34eb56dc24e8f52a7f05ee513b2d4f596",
+                "sha256:5c3721c2c9e4c4953a41a26c14f4cef64330392a6d2d675c8b1db3b645e31f0e",
+                "sha256:5fa567e99765fe98f4e7d7394ce623e794d7cabb170f2ca2ac5a4174437e90dd",
+                "sha256:5fd215c0c7d7aab005221608a3c2b46f58c0285a819565887ee0b718c052aa4e",
+                "sha256:6175d1a0559986c6ee3f7fccfc4a90ecd12ba0a383dcc2da30c2b9918d67d8a3",
+                "sha256:61c4bf1ba021817de12b813338c9be9f0ad5b1e781b9b340a6d29fc13e7c1b5e",
+                "sha256:6537e7c10cc47c595828b8a8be04c72144725c383c4702703ff4e42e44577312",
+                "sha256:68f962d9b72ce69ea8621f57551b2fa9c70509af757ee3b8105d4f51b92b41a7",
+                "sha256:7352b9161b33fd0b643ccd1f21f3a3908daaddf414f1c6cb9d3a2fd618bf2572",
+                "sha256:796a79f63eca8814ca3317a1ea443645c9ff0d18b188de470ed7ccd45ae79428",
+                "sha256:79afb6197e2f7f60c4824dd4b2d4c2ec5801ceb6ba9ce5d2c3080e5660d51a4f",
+                "sha256:7a588d39e0925f6a2bff87154752481273cdb1736270642aeb3635cb9b4cad07",
+                "sha256:8748731ad392d736cc9ccac03c9845b13bb07d020a33423fa5b3a36521ac6e4e",
+                "sha256:8fe7502616b67b234482c3ce276ff26f39ffe88adca2acf0261df4b8454668b4",
+                "sha256:9314d5678dcc665330df5b69c1e726a0e49b27df0461c08ca12674bcc19ef136",
+                "sha256:9735317685ba6ec7e3754798c8871c2f49aa5e687cc794a0b1d284b2389d1bd5",
+                "sha256:9981706d300c18d8b220995ad22627647be11a4276721c10911e0e9fa44c83e8",
+                "sha256:9e78295f4144f9dacfed4f92935fbe1780021247c2fabf73a819b17f0ccfff8d",
+                "sha256:b016ea6b959d3b9556cb401c55a37547135a587db0115635a443b2ce8f1c7228",
+                "sha256:b6cf3764c030e5338e7f61f95bd21147963cf6aa16e09d2f74f1fa52013c1206",
+                "sha256:beccf7b8a10b09c4ae543582c1319c6df47d78fd732f854ac68d518ee1fb97fa",
+                "sha256:c0884920835a033b78d1c73b6d3bbcda8161a900f38a488829a83982925f6c2e",
+                "sha256:c3e757949f268364b96ca894b4c342b41dc6f8f8b66c37878aacef5930db61be",
+                "sha256:ca498687ca46a62ae590253fba634a1fe9836bc56f626852fb2720f334c9e4e5",
+                "sha256:d1d0d98d95dd18fe29dc66808e1accf59f037d5716f86a501fc0256455219668",
+                "sha256:d21918e9ef11edf36764b93101e2ae8cc82aa5efdc7c5a4e9c6c35a48496d601",
+                "sha256:d7fed867ee50edf1a0b4a11e8e5d0895150e572af1cd6d315d557758bfa9c057",
+                "sha256:db66fc317a046556a96b453a58eced5024af4582a8dbdc0c23ca4dbc0d5b3146",
+                "sha256:dde0070c40ea8bb3641e811c1cfbf18e265d024deff6de52c5950677a8fb1e0f",
+                "sha256:df4e745a81c110e7446b1cc8131bf986157770fa405fe90e15e850aaf7619bc8",
+                "sha256:e2213def81a50519d7cc56ed643c9e93e0247f5bbe0d1247d15fa520814a7cd7",
+                "sha256:ef48e2707fb320c8f139424a596f5b69955a85b178f15af261bab871873bb987",
+                "sha256:f152cbf5b88aaeb836127d920dd0f5e7edff5a66f10c079157306c4343d86c19",
+                "sha256:fc0b4d8bfeabd25ea75e94632f5b6e047eef8adaed0c2161ada1e922e7f7cece"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==7.4.4"
+            "version": "==7.5.1"
         },
         "distlib": {
             "hashes": [
                 "sha256:034db59a0b96f8ca18035f36290806a9a6e6bd9d1ff91e45a7f172eb17e51784",
                 "sha256:1530ea13e350031b6312d8580ddb6b27a104275a31106523b8f123787f494f64"
             ],
             "version": "==0.3.8"
         },
         "exceptiongroup": {
             "markers": "python_version < '3.11'"
         },
         "filelock": {
             "hashes": [
-                "sha256:5ffa845303983e7a0b7ae17636509bc97997d58afeafa72fb141a17b152284cb",
-                "sha256:a79895a25bbefdf55d1a2a0a80968f7dbb28edcd6d4234a0afb3f37ecde4b546"
+                "sha256:43339835842f110ca7ae60f1e1c160714c5a6afd15a2873419ab185334975c0f",
+                "sha256:6ea72da3be9b8c82afd3edcf99f2fffbb5076335a5ae4d03248bb5b6c3eae78a"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==3.13.3"
+            "version": "==3.14.0"
         },
         "flake8": {
             "hashes": [
                 "sha256:33f96621059e65eec474169085dc92bf26e7b2d47366b70be2f67ab80dc25132",
                 "sha256:a6dfbb75e03252917f2473ea9653f7cd799c3064e54d4c8140044c5c065f53c3"
             ],
             "index": "pypi",
@@ -671,46 +679,46 @@
                 "sha256:8337dd7b50877f163d4c0289bc1f1c7f127550241988d568c1db512c4324a619",
                 "sha256:9c535c4c61193c2df8871222567d7fd7e5014d835f97dc7b7439069e2413d343"
             ],
             "version": "==2.1.0"
         },
         "identify": {
             "hashes": [
-                "sha256:10a7ca245cfcd756a554a7288159f72ff105ad233c7c4b9c6f0f4d108f5f6791",
-                "sha256:c4de0081837b211594f8e877a6b4fad7ca32bbfc1a9307fdd61c28bfe923f13e"
+                "sha256:37d93f380f4de590500d9dba7db359d0d3da95ffe7f9de1753faa159e71e7dfa",
+                "sha256:e5e00f54165f9047fbebeb4a560f9acfb8af4c88232be60a488e9b68d122745d"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==2.5.35"
+            "version": "==2.5.36"
         },
         "idna": {
             "hashes": [
-                "sha256:9ecdbbd083b06798ae1e86adcbfe8ab1479cf864e4ee30fe4e46a003d12491ca",
-                "sha256:c05567e9c24a6b9faaa835c4821bad0590fbb9d5779e7caa6e1cc4978e7eb24f"
+                "sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc",
+                "sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0"
             ],
             "markers": "python_version >= '3.5'",
-            "version": "==3.6"
+            "version": "==3.7"
         },
         "importlib-metadata": {
             "markers": "python_version < '3.10'"
         },
         "iniconfig": {
             "hashes": [
                 "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3",
                 "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
         "jinja2": {
             "hashes": [
-                "sha256:7d6d50dd97d52cbc355597bd845fabfbac3f551e1f99619e39a35ce8c370b5fa",
-                "sha256:ac8bd6544d4bb2c9792bf3a159e80bba8fda7f07e81bc3aed565432d5925ba90"
+                "sha256:4a3aee7acbbe7303aede8e9648d13b8bf88a429282aa6122a993f0ac800cb369",
+                "sha256:bc5dd2abb727a5319567b7a813e6a2e7318c39f4f487cfe6c89c6f9c7d25197d"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.1.3"
+            "version": "==3.1.4"
         },
         "markdown": {
             "hashes": [
                 "sha256:48f276f4d8cfb8ce6527c8f79e2ee29708508bf4d40aa410fbc3b4ee832c850f",
                 "sha256:ed4f41f6daecbeeb96e576ce414c41d2d876daa9a16cb35fa8ed8c2ddfad0224"
             ],
             "markers": "python_version >= '3.8'",
@@ -796,38 +804,46 @@
                 "sha256:70775750742b25c0d8f36c55aed03d24c3384d17c951b3175d898bd778ef0307"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.3.4"
         },
         "mkdocs": {
             "hashes": [
-                "sha256:3b3a78e736b31158d64dbb2f8ba29bd46a379d0c6e324c2246c3bc3d2189cfc1",
-                "sha256:eb7c99214dcb945313ba30426c2451b735992c73c2e10838f76d09e39ff4d0e2"
+                "sha256:1eb5cb7676b7d89323e62b56235010216319217d4af5ddc543a91beb8d125ea7",
+                "sha256:a73f735824ef83a4f3bcb7a231dcab23f5a838f88b7efc54a0eef5fbdbc3c512"
             ],
             "index": "pypi",
-            "markers": "python_version >= '3.7'",
-            "version": "==1.5.3"
+            "markers": "python_version >= '3.8'",
+            "version": "==1.6.0"
         },
         "mkdocs-awesome-pages-plugin": {
             "hashes": [
                 "sha256:9c795587695bd1ee85a8b7e43293005418df5a8b9ef296a3e628be427b693b4d",
                 "sha256:c3f7d366ecfe99b64524c49a84d8e13c576c19a918ea2e6f59bb486a259313af"
             ],
             "index": "pypi",
             "markers": "python_version >= '3.7'",
             "version": "==2.9.2"
         },
+        "mkdocs-get-deps": {
+            "hashes": [
+                "sha256:162b3d129c7fad9b19abfdcb9c1458a651628e4b1dea628ac68790fb3061c60c",
+                "sha256:2bf11d0b133e77a0dd036abeeb06dec8775e46efa526dc70667d8863eefc6134"
+            ],
+            "markers": "python_version >= '3.8'",
+            "version": "==0.2.0"
+        },
         "mkdocs-material": {
             "hashes": [
-                "sha256:06ae1275a72db1989cf6209de9e9ecdfbcfdbc24c58353877b2bb927dbe413e4",
-                "sha256:14a2a60119a785e70e765dd033e6211367aca9fc70230e577c1cf6a326949571"
+                "sha256:22a853a456ae8c581c4628159574d6fc7c71b2c7569dc9c3a82cc70432219599",
+                "sha256:8c7a377d323567934e6cd46915e64dc209efceaec0dec1cf2202184f5649862c"
             ],
             "index": "pypi",
             "markers": "python_version >= '3.8'",
-            "version": "==9.5.17"
+            "version": "==9.5.22"
         },
         "mkdocs-material-extensions": {
             "hashes": [
                 "sha256:10c9511cea88f568257f960358a467d12b970e1f7b2c0e5fb2bb48cab1928443",
                 "sha256:adff8b62700b25cb77b53358dad940f3ef973dd6db797907c49e3c2ef3ab4e31"
             ],
             "markers": "python_version >= '3.8'",
@@ -869,36 +885,36 @@
                 "sha256:a482d51503a1ab33b1c67a6c3813a26953dbdc71c31dacaef9a838c4e29f5712"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==0.12.1"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:0614df2a2f37e1a662acbd8e2b25b92ccf8632929bc6d43467e17fe89c75e068",
-                "sha256:ef0cc731df711022c174543cb70a9b5bd22e5a9337c8624ef2c2ceb8ddad8768"
+                "sha256:2d7a1657e36a80ea911db832a8a6ece5ee53d8de21edd5cc5879af6530b1bfee",
+                "sha256:38b7b51f512eed9e84a22788b4bce1de17c0adb134d6becb09836e37d8654cd3"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==4.2.0"
+            "version": "==4.2.2"
         },
         "pluggy": {
             "hashes": [
-                "sha256:7db9f7b503d67d1c5b95f59773ebb58a8c1c288129a88665838012cfb07b8981",
-                "sha256:8c85c2876142a764e5b7548e7d9a0e0ddb46f5185161049a79b7e974454223be"
+                "sha256:2cffa88e94fdc978c4c574f15f9e59b7f4201d439195c3715ca9e2486f1d0cf1",
+                "sha256:44e1ad92c8ca002de6377e165f3e0f1be63266ab4d554740532335b9d75ea669"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==1.4.0"
+            "version": "==1.5.0"
         },
         "pre-commit": {
             "hashes": [
-                "sha256:5eae9e10c2b5ac51577c3452ec0a490455c45a0533f7960f993a0d01e59decab",
-                "sha256:e209d61b8acdcf742404408531f0c37d49d2c734fd7cff2d6076083d191cb060"
+                "sha256:8ca3ad567bc78a4972a3f1a477e94a79d4597e8140a6e0b651c5e33899c3654a",
+                "sha256:fae36fd1d7ad7d6a5a1c0b0d5adb2ed1a3bda5a21bf6c3e5372073d7a11cd4c5"
             ],
             "index": "pypi",
             "markers": "python_version >= '3.9'",
-            "version": "==3.7.0"
+            "version": "==3.7.1"
         },
         "pycodestyle": {
             "hashes": [
                 "sha256:41ba0e7afc9752dfb53ced5489e89f8186be00e599e712660695b7a75ff2663f",
                 "sha256:44fe31000b2d866f2e41841b18528a505fbd7fef9017b04eff4e2648a0fadc67"
             ],
             "markers": "python_version >= '3.8'",
@@ -910,36 +926,36 @@
                 "sha256:84b5be138a2dfbb40689ca07e2152deb896a65c3a3e24c251c5c62489568074a"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==3.2.0"
         },
         "pygments": {
             "hashes": [
-                "sha256:b27c2826c47d0f3219f29554824c30c5e8945175d888647acd804ddd04af846c",
-                "sha256:da46cec9fd2de5be3a8a784f434e4c4ab670b4ff54d605c4c2717e9d49c4c367"
+                "sha256:786ff802f32e91311bff3889f6e9a86e81505fe99f2735bb6d60ae0c5004f199",
+                "sha256:b8e6aca0523f3ab76fee51799c488e38782ac06eafcf95e7ba832985c8e7b13a"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==2.17.2"
+            "markers": "python_version >= '3.8'",
+            "version": "==2.18.0"
         },
         "pymdown-extensions": {
             "hashes": [
-                "sha256:c70e146bdd83c744ffc766b4671999796aba18842b268510a329f7f64700d584",
-                "sha256:f5cc7000d7ff0d1ce9395d216017fa4df3dde800afb1fb72d1c7d3fd35e710f4"
+                "sha256:3ab1db5c9e21728dabf75192d71471f8e50f216627e9a1fa9535ecb0231b9940",
+                "sha256:f938326115884f48c6059c67377c46cf631c733ef3629b6eed1349989d1b30cb"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==10.7.1"
+            "version": "==10.8.1"
         },
         "pytest": {
             "hashes": [
-                "sha256:2a8386cfc11fa9d2c50ee7b2a57e7d898ef90470a7a34c4b949ff59662bb78b7",
-                "sha256:ac978141a75948948817d360297b7aae0fcb9d6ff6bc9ec6d514b85d5a65c044"
+                "sha256:1733f0620f6cda4095bbf0d9ff8022486e91892245bb9e7d5542c018f612f233",
+                "sha256:d507d4482197eac0ba2bae2e9babf0672eb333017bcedaa5fb1a3d42c1174b3f"
             ],
             "index": "pypi",
             "markers": "python_version >= '3.8'",
-            "version": "==8.1.1"
+            "version": "==8.2.0"
         },
         "pytest-cov": {
             "hashes": [
                 "sha256:4f0764a1219df53214206bf1feea4633c3b558a2925c8b59f144f682861ce652",
                 "sha256:5837b58e9f6ebd335b0f8060eecce69b662415b16dc503883a02f45dfeb14857"
             ],
             "index": "pypi",
@@ -1017,127 +1033,113 @@
                 "sha256:af31106dec8a4d68c60207c1886031cbf839b68aa7abccdb19868200532c2069"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.1"
         },
         "regex": {
             "hashes": [
-                "sha256:0694219a1d54336fd0445ea382d49d36882415c0134ee1e8332afd1529f0baa5",
-                "sha256:086dd15e9435b393ae06f96ab69ab2d333f5d65cbe65ca5a3ef0ec9564dfe770",
-                "sha256:094ba386bb5c01e54e14434d4caabf6583334090865b23ef58e0424a6286d3dc",
-                "sha256:09da66917262d9481c719599116c7dc0c321ffcec4b1f510c4f8a066f8768105",
-                "sha256:0ecf44ddf9171cd7566ef1768047f6e66975788258b1c6c6ca78098b95cf9a3d",
-                "sha256:0fda75704357805eb953a3ee15a2b240694a9a514548cd49b3c5124b4e2ad01b",
-                "sha256:11a963f8e25ab5c61348d090bf1b07f1953929c13bd2309a0662e9ff680763c9",
-                "sha256:150c39f5b964e4d7dba46a7962a088fbc91f06e606f023ce57bb347a3b2d4630",
-                "sha256:1b9d811f72210fa9306aeb88385b8f8bcef0dfbf3873410413c00aa94c56c2b6",
-                "sha256:1e0eabac536b4cc7f57a5f3d095bfa557860ab912f25965e08fe1545e2ed8b4c",
-                "sha256:22a86d9fff2009302c440b9d799ef2fe322416d2d58fc124b926aa89365ec482",
-                "sha256:22f3470f7524b6da61e2020672df2f3063676aff444db1daa283c2ea4ed259d6",
-                "sha256:263ef5cc10979837f243950637fffb06e8daed7f1ac1e39d5910fd29929e489a",
-                "sha256:283fc8eed679758de38fe493b7d7d84a198b558942b03f017b1f94dda8efae80",
-                "sha256:29171aa128da69afdf4bde412d5bedc335f2ca8fcfe4489038577d05f16181e5",
-                "sha256:298dc6354d414bc921581be85695d18912bea163a8b23cac9a2562bbcd5088b1",
-                "sha256:2aae8101919e8aa05ecfe6322b278f41ce2994c4a430303c4cd163fef746e04f",
-                "sha256:2f4e475a80ecbd15896a976aa0b386c5525d0ed34d5c600b6d3ebac0a67c7ddf",
-                "sha256:34e4af5b27232f68042aa40a91c3b9bb4da0eeb31b7632e0091afc4310afe6cb",
-                "sha256:37f8e93a81fc5e5bd8db7e10e62dc64261bcd88f8d7e6640aaebe9bc180d9ce2",
-                "sha256:3a17d3ede18f9cedcbe23d2daa8a2cd6f59fe2bf082c567e43083bba3fb00347",
-                "sha256:3b1de218d5375cd6ac4b5493e0b9f3df2be331e86520f23382f216c137913d20",
-                "sha256:43f7cd5754d02a56ae4ebb91b33461dc67be8e3e0153f593c509e21d219c5060",
-                "sha256:4558410b7a5607a645e9804a3e9dd509af12fb72b9825b13791a37cd417d73a5",
-                "sha256:4719bb05094d7d8563a450cf8738d2e1061420f79cfcc1fa7f0a44744c4d8f73",
-                "sha256:4bfc2b16e3ba8850e0e262467275dd4d62f0d045e0e9eda2bc65078c0110a11f",
-                "sha256:518440c991f514331f4850a63560321f833979d145d7d81186dbe2f19e27ae3d",
-                "sha256:51f4b32f793812714fd5307222a7f77e739b9bc566dc94a18126aba3b92b98a3",
-                "sha256:531ac6cf22b53e0696f8e1d56ce2396311254eb806111ddd3922c9d937151dae",
-                "sha256:5cd05d0f57846d8ba4b71d9c00f6f37d6b97d5e5ef8b3c3840426a475c8f70f4",
-                "sha256:5dd58946bce44b53b06d94aa95560d0b243eb2fe64227cba50017a8d8b3cd3e2",
-                "sha256:60080bb3d8617d96f0fb7e19796384cc2467447ef1c491694850ebd3670bc457",
-                "sha256:636ba0a77de609d6510235b7f0e77ec494d2657108f777e8765efc060094c98c",
-                "sha256:67d3ccfc590e5e7197750fcb3a2915b416a53e2de847a728cfa60141054123d4",
-                "sha256:68191f80a9bad283432385961d9efe09d783bcd36ed35a60fb1ff3f1ec2efe87",
-                "sha256:7502534e55c7c36c0978c91ba6f61703faf7ce733715ca48f499d3dbbd7657e0",
-                "sha256:7aa47c2e9ea33a4a2a05f40fcd3ea36d73853a2aae7b4feab6fc85f8bf2c9704",
-                "sha256:7d2af3f6b8419661a0c421584cfe8aaec1c0e435ce7e47ee2a97e344b98f794f",
-                "sha256:7e316026cc1095f2a3e8cc012822c99f413b702eaa2ca5408a513609488cb62f",
-                "sha256:88ad44e220e22b63b0f8f81f007e8abbb92874d8ced66f32571ef8beb0643b2b",
-                "sha256:88d1f7bef20c721359d8675f7d9f8e414ec5003d8f642fdfd8087777ff7f94b5",
-                "sha256:89723d2112697feaa320c9d351e5f5e7b841e83f8b143dba8e2d2b5f04e10923",
-                "sha256:8a0ccf52bb37d1a700375a6b395bff5dd15c50acb745f7db30415bae3c2b0715",
-                "sha256:8c2c19dae8a3eb0ea45a8448356ed561be843b13cbc34b840922ddf565498c1c",
-                "sha256:905466ad1702ed4acfd67a902af50b8db1feeb9781436372261808df7a2a7bca",
-                "sha256:9852b76ab558e45b20bf1893b59af64a28bd3820b0c2efc80e0a70a4a3ea51c1",
-                "sha256:98a2636994f943b871786c9e82bfe7883ecdaba2ef5df54e1450fa9869d1f756",
-                "sha256:9aa1a67bbf0f957bbe096375887b2505f5d8ae16bf04488e8b0f334c36e31360",
-                "sha256:9eda5f7a50141291beda3edd00abc2d4a5b16c29c92daf8d5bd76934150f3edc",
-                "sha256:a6d1047952c0b8104a1d371f88f4ab62e6275567d4458c1e26e9627ad489b445",
-                "sha256:a9b6d73353f777630626f403b0652055ebfe8ff142a44ec2cf18ae470395766e",
-                "sha256:a9cc99d6946d750eb75827cb53c4371b8b0fe89c733a94b1573c9dd16ea6c9e4",
-                "sha256:ad83e7545b4ab69216cef4cc47e344d19622e28aabec61574b20257c65466d6a",
-                "sha256:b014333bd0217ad3d54c143de9d4b9a3ca1c5a29a6d0d554952ea071cff0f1f8",
-                "sha256:b43523d7bc2abd757119dbfb38af91b5735eea45537ec6ec3a5ec3f9562a1c53",
-                "sha256:b521dcecebc5b978b447f0f69b5b7f3840eac454862270406a39837ffae4e697",
-                "sha256:b77e27b79448e34c2c51c09836033056a0547aa360c45eeeb67803da7b0eedaf",
-                "sha256:b7a635871143661feccce3979e1727c4e094f2bdfd3ec4b90dfd4f16f571a87a",
-                "sha256:b7fca9205b59c1a3d5031f7e64ed627a1074730a51c2a80e97653e3e9fa0d415",
-                "sha256:ba1b30765a55acf15dce3f364e4928b80858fa8f979ad41f862358939bdd1f2f",
-                "sha256:ba99d8077424501b9616b43a2d208095746fb1284fc5ba490139651f971d39d9",
-                "sha256:c25a8ad70e716f96e13a637802813f65d8a6760ef48672aa3502f4c24ea8b400",
-                "sha256:c3c4a78615b7762740531c27cf46e2f388d8d727d0c0c739e72048beb26c8a9d",
-                "sha256:c40281f7d70baf6e0db0c2f7472b31609f5bc2748fe7275ea65a0b4601d9b392",
-                "sha256:c7ad32824b7f02bb3c9f80306d405a1d9b7bb89362d68b3c5a9be53836caebdb",
-                "sha256:cb3fe77aec8f1995611f966d0c656fdce398317f850d0e6e7aebdfe61f40e1cd",
-                "sha256:cc038b2d8b1470364b1888a98fd22d616fba2b6309c5b5f181ad4483e0017861",
-                "sha256:cc37b9aeebab425f11f27e5e9e6cf580be7206c6582a64467a14dda211abc232",
-                "sha256:cc6bb9aa69aacf0f6032c307da718f61a40cf970849e471254e0e91c56ffca95",
-                "sha256:d126361607b33c4eb7b36debc173bf25d7805847346dd4d99b5499e1fef52bc7",
-                "sha256:d15b274f9e15b1a0b7a45d2ac86d1f634d983ca40d6b886721626c47a400bf39",
-                "sha256:d166eafc19f4718df38887b2bbe1467a4f74a9830e8605089ea7a30dd4da8887",
-                "sha256:d498eea3f581fbe1b34b59c697512a8baef88212f92e4c7830fcc1499f5b45a5",
-                "sha256:d6f7e255e5fa94642a0724e35406e6cb7001c09d476ab5fce002f652b36d0c39",
-                "sha256:d78bd484930c1da2b9679290a41cdb25cc127d783768a0369d6b449e72f88beb",
-                "sha256:d865984b3f71f6d0af64d0d88f5733521698f6c16f445bb09ce746c92c97c586",
-                "sha256:d902a43085a308cef32c0d3aea962524b725403fd9373dea18110904003bac97",
-                "sha256:d94a1db462d5690ebf6ae86d11c5e420042b9898af5dcf278bd97d6bda065423",
-                "sha256:da695d75ac97cb1cd725adac136d25ca687da4536154cdc2815f576e4da11c69",
-                "sha256:db2a0b1857f18b11e3b0e54ddfefc96af46b0896fb678c85f63fb8c37518b3e7",
-                "sha256:df26481f0c7a3f8739fecb3e81bc9da3fcfae34d6c094563b9d4670b047312e1",
-                "sha256:e14b73607d6231f3cc4622809c196b540a6a44e903bcfad940779c80dffa7be7",
-                "sha256:e2610e9406d3b0073636a3a2e80db05a02f0c3169b5632022b4e81c0364bcda5",
-                "sha256:e692296c4cc2873967771345a876bcfc1c547e8dd695c6b89342488b0ea55cd8",
-                "sha256:e693e233ac92ba83a87024e1d32b5f9ab15ca55ddd916d878146f4e3406b5c91",
-                "sha256:e81469f7d01efed9b53740aedd26085f20d49da65f9c1f41e822a33992cb1590",
-                "sha256:e8c7e08bb566de4faaf11984af13f6bcf6a08f327b13631d41d62592681d24fe",
-                "sha256:ed19b3a05ae0c97dd8f75a5d8f21f7723a8c33bbc555da6bbe1f96c470139d3c",
-                "sha256:efb2d82f33b2212898f1659fb1c2e9ac30493ac41e4d53123da374c3b5541e64",
-                "sha256:f44dd4d68697559d007462b0a3a1d9acd61d97072b71f6d1968daef26bc744bd",
-                "sha256:f72cbae7f6b01591f90814250e636065850c5926751af02bb48da94dfced7baa",
-                "sha256:f7bc09bc9c29ebead055bcba136a67378f03d66bf359e87d0f7c759d6d4ffa31",
-                "sha256:ff100b203092af77d1a5a7abe085b3506b7eaaf9abf65b73b7d6905b6cb76988"
+                "sha256:031219782d97550c2098d9a68ce9e9eaefe67d2d81d8ff84c8354f9c009e720c",
+                "sha256:0709ba544cf50bd5cb843df4b8bb6701bae2b70a8e88da9add8386cbca5c1385",
+                "sha256:0a9f89d7db5ef6bdf53e5cc8e6199a493d0f1374b3171796b464a74ebe8e508a",
+                "sha256:0bc94873ba11e34837bffd7e5006703abeffc4514e2f482022f46ce05bd25e67",
+                "sha256:0ce56a923f4c01d7568811bfdffe156268c0a7aae8a94c902b92fe34c4bde785",
+                "sha256:0faecb6d5779753a6066a3c7a0471a8d29fe25d9981ca9e552d6d1b8f8b6a594",
+                "sha256:1118ba9def608250250f4b3e3f48c62f4562ba16ca58ede491b6e7554bfa09ff",
+                "sha256:12446827f43c7881decf2c126762e11425de5eb93b3b0d8b581344c16db7047a",
+                "sha256:14905ed75c7a6edf423eb46c213ed3f4507c38115f1ed3c00f4ec9eafba50e58",
+                "sha256:15e593386ec6331e0ab4ac0795b7593f02ab2f4b30a698beb89fbdc34f92386a",
+                "sha256:160ba087232c5c6e2a1e7ad08bd3a3f49b58c815be0504d8c8aacfb064491cd8",
+                "sha256:161a206c8f3511e2f5fafc9142a2cc25d7fe9a1ec5ad9b4ad2496a7c33e1c5d2",
+                "sha256:169fd0acd7a259f58f417e492e93d0e15fc87592cd1e971c8c533ad5703b5830",
+                "sha256:193b7c6834a06f722f0ce1ba685efe80881de7c3de31415513862f601097648c",
+                "sha256:1a3903128f9e17a500618e80c68165c78c741ebb17dd1a0b44575f92c3c68b02",
+                "sha256:1d5bd666466c8f00a06886ce1397ba8b12371c1f1c6d1bef11013e9e0a1464a8",
+                "sha256:224a9269f133564109ce668213ef3cb32bc72ccf040b0b51c72a50e569e9dc9e",
+                "sha256:236cace6c1903effd647ed46ce6dd5d76d54985fc36dafc5256032886736c85d",
+                "sha256:249fbcee0a277c32a3ce36d8e36d50c27c968fdf969e0fbe342658d4e010fbc8",
+                "sha256:29d839829209f3c53f004e1de8c3113efce6d98029f044fa5cfee666253ee7e6",
+                "sha256:2c8982ee19ccecabbaeac1ba687bfef085a6352a8c64f821ce2f43e6d76a9298",
+                "sha256:2f30a5ab8902f93930dc6f627c4dd5da2703333287081c85cace0fc6e21c25af",
+                "sha256:304e7e2418146ae4d0ef0e9ffa28f881f7874b45b4994cc2279b21b6e7ae50c8",
+                "sha256:32e5f3b8e32918bfbdd12eca62e49ab3031125c454b507127ad6ecbd86e62fca",
+                "sha256:334b79ce9c08f26b4659a53f42892793948a613c46f1b583e985fd5a6bf1c149",
+                "sha256:33d19f0cde6838c81acffff25c7708e4adc7dd02896c9ec25c3939b1500a1778",
+                "sha256:3799e36d60a35162bb35b2246d8bb012192b7437dff807ef79c14e7352706306",
+                "sha256:42be5de7cc8c1edac55db92d82b68dc8e683b204d6f5414c5a51997a323d7081",
+                "sha256:44b3267cea873684af022822195298501568ed44d542f9a2d9bebc0212e99069",
+                "sha256:458d68d34fb74b906709735c927c029e62f7d06437a98af1b5b6258025223210",
+                "sha256:45cc13d398b6359a7708986386f72bd156ae781c3e83a68a6d4cee5af04b1ce9",
+                "sha256:4e7eaf9df15423d07b6050fb91f86c66307171b95ea53e2d87a7993b6d02c7f7",
+                "sha256:4fad420b14ae1970a1f322e8ae84a1d9d89375eb71e1b504060ab2d1bfe68f3c",
+                "sha256:504b5116e2bd1821efd815941edff7535e93372a098e156bb9dffde30264e798",
+                "sha256:50e7e96a527488334379e05755b210b7da4a60fc5d6481938c1fa053e0c92184",
+                "sha256:51d27844763c273a122e08a3e86e7aefa54ee09fb672d96a645ece0454d8425e",
+                "sha256:5253dcb0bfda7214523de58b002eb0090cb530d7c55993ce5f6d17faf953ece7",
+                "sha256:534efd2653ebc4f26fc0e47234e53bf0cb4715bb61f98c64d2774a278b58c846",
+                "sha256:560278c9975694e1f0bc50da187abf2cdc1e4890739ea33df2bc4a85eeef143e",
+                "sha256:571452362d552de508c37191b6abbbb660028b8b418e2d68c20779e0bc8eaaa8",
+                "sha256:62b5f7910b639f3c1d122d408421317c351e213ca39c964ad4121f27916631c6",
+                "sha256:696639a73ca78a380acfaa0a1f6dd8220616a99074c05bba9ba8bb916914b224",
+                "sha256:6ccdeef4584450b6f0bddd5135354908dacad95425fcb629fe36d13e48b60f32",
+                "sha256:70364a097437dd0a90b31cd77f09f7387ad9ac60ef57590971f43b7fca3082a5",
+                "sha256:7117cb7d6ac7f2e985f3d18aa8a1728864097da1a677ffa69e970ca215baebf1",
+                "sha256:7467ad8b0eac0b28e52679e972b9b234b3de0ea5cee12eb50091d2b68145fe36",
+                "sha256:7d35d4cc9270944e95f9c88af757b0c9fc43f396917e143a5756608462c5223b",
+                "sha256:7dda3091838206969c2b286f9832dff41e2da545b99d1cfaea9ebd8584d02708",
+                "sha256:853cc36e756ff673bf984e9044ccc8fad60b95a748915dddeab9488aea974c73",
+                "sha256:8722f72068b3e1156a4b2e1afde6810f1fc67155a9fa30a4b9d5b4bc46f18fb0",
+                "sha256:8c6c71cf92b09e5faa72ea2c68aa1f61c9ce11cb66fdc5069d712f4392ddfd00",
+                "sha256:903350bf44d7e4116b4d5898b30b15755d61dcd3161e3413a49c7db76f0bee5a",
+                "sha256:91b53dea84415e8115506cc62e441a2b54537359c63d856d73cb1abe05af4c9a",
+                "sha256:951be1eae7b47660412dc4938777a975ebc41936d64e28081bf2e584b47ec246",
+                "sha256:972b49f2fe1047b9249c958ec4fa1bdd2cf8ce305dc19d27546d5a38e57732d8",
+                "sha256:9a8625849387b9d558d528e263ecc9c0fbde86cfa5c2f0eef43fff480ae24d71",
+                "sha256:9cdbb1998da94607d5eec02566b9586f0e70d6438abf1b690261aac0edda7ab6",
+                "sha256:9e6d4d6ae1827b2f8c7200aaf7501c37cf3f3896c86a6aaf2566448397c823dd",
+                "sha256:aab65121229c2ecdf4a31b793d99a6a0501225bd39b616e653c87b219ed34a49",
+                "sha256:ab98016541543692a37905871a5ffca59b16e08aacc3d7d10a27297b443f572d",
+                "sha256:ad45f3bccfcb00868f2871dce02a755529838d2b86163ab8a246115e80cfb7d6",
+                "sha256:b43b78f9386d3d932a6ce5af4b45f393d2e93693ee18dc4800d30a8909df700e",
+                "sha256:b66421f8878a0c82fc0c272a43e2121c8d4c67cb37429b764f0d5ad70b82993b",
+                "sha256:ba034c8db4b264ef1601eb33cd23d87c5013b8fb48b8161debe2e5d3bd9156b0",
+                "sha256:bbdc5db2c98ac2bf1971ffa1410c87ca7a15800415f788971e8ba8520fc0fda9",
+                "sha256:bc0db93ad039fc2fe32ccd3dd0e0e70c4f3d6e37ae83f0a487e1aba939bd2fbd",
+                "sha256:bf7c8ee4861d9ef5b1120abb75846828c811f932d63311596ad25fa168053e00",
+                "sha256:bf9596cba92ce7b1fd32c7b07c6e3212c7eed0edc271757e48bfcd2b54646452",
+                "sha256:c43395a3b7cc9862801a65c6994678484f186ce13c929abab44fb8a9e473a55a",
+                "sha256:c46a76a599fcbf95f98755275c5527304cc4f1bb69919434c1e15544d7052910",
+                "sha256:ca23b41355ba95929e9505ee04e55495726aa2282003ed9b012d86f857d3e49b",
+                "sha256:cd832bd9b6120d6074f39bdfbb3c80e416848b07ac72910f1c7f03131a6debc3",
+                "sha256:cfa6d61a76c77610ba9274c1a90a453062bdf6887858afbe214d18ad41cf6bde",
+                "sha256:d8a0f0ab5453e409586b11ebe91c672040bc804ca98d03a656825f7890cbdf88",
+                "sha256:e91b1976358e17197157b405cab408a5f4e33310cda211c49fc6da7cffd0b2f0",
+                "sha256:ea057306ab469130167014b662643cfaed84651c792948891d003cf0039223a5",
+                "sha256:eda3dd46df535da787ffb9036b5140f941ecb91701717df91c9daf64cabef953",
+                "sha256:f03b1dbd4d9596dd84955bb40f7d885204d6aac0d56a919bb1e0ff2fb7e1735a",
+                "sha256:fa9335674d7c819674467c7b46154196c51efbaf5f5715187fd366814ba3fa39"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==2023.12.25"
+            "markers": "python_version >= '3.8'",
+            "version": "==2024.5.10"
         },
         "requests": {
             "hashes": [
                 "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f",
                 "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
             "index": "pypi",
             "markers": "python_version >= '3.7'",
             "version": "==2.31.0"
         },
         "setuptools": {
             "hashes": [
-                "sha256:0ff4183f8f42cd8fa3acea16c45205521a4ef28f73c6391d8a25e92893134f2e",
-                "sha256:c21c49fb1042386df081cb5d86759792ab89efca84cf114889191cd09aacc80c"
+                "sha256:6c1fccdac05a97e598fb0ae3bbed5904ccb317337a51139dcd51453611bbb987",
+                "sha256:c636ac361bc47580504644275c9ad802c50415c7522212252c033bd15f301f32"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==69.2.0"
+            "version": "==69.5.1"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
@@ -1152,19 +1154,19 @@
                 "sha256:d0570876c61ab9e520d776c38acbbb5b05a776d3f9ff98a5c8fd5162a444cf19"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==2.2.1"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:961c026ac520bac5f69acb8ea063e8a4f071bcc9457b9c1f28f6b085c511583a",
-                "sha256:e08e13ecdca7a0bd53798f356d5831434afa5b07b93f0abdf0797b7a06ffe197"
+                "sha256:82bf0f4eebbb78d36ddaee0283d43fe5736b53880b8a8cdcd37390a07ac3741c",
+                "sha256:a624db5e94f01ad993d476b9ee5346fdf7b9de43ccaee0e0197012dc838a0e9b"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==20.25.1"
+            "version": "==20.26.2"
         },
         "watchdog": {
             "hashes": [
                 "sha256:11e12fafb13372e18ca1bbf12d50f593e7280646687463dd47730fd4f4d5d257",
                 "sha256:2895bf0518361a9728773083908801a376743bcc37dfa252b801af8fd281b1ca",
                 "sha256:39cb34b1f1afbf23e9562501673e7146777efe95da24fab5707b88f7fb11649b",
                 "sha256:45cc09cc4c3b43fb10b59ef4d07318d9a3ecdbff03abd2e36e77b6dd9f9a5c85",
@@ -1195,18 +1197,18 @@
                 "sha256:f9b2fdca47dc855516b2d66eef3c39f2672cbf7e7a42e7e67ad2cbfcd6ba107d"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==4.0.0"
         },
         "wcmatch": {
             "hashes": [
-                "sha256:24c19cedc92bc9c9e27f39db4e1824d72f95bd2cea32b254a47a45b1a1b227ed",
-                "sha256:c0088c7f6426cf6bf27e530e2b7b734031905f7e490475fd83c7c5008ab581b3"
+                "sha256:17d3ad3758f9d0b5b4dedc770b65420d4dac62e680229c287bf24c9db856a478",
+                "sha256:a70222b86dea82fb382dd87b73278c10756c138bd6f8f714e2183128887b9eb2"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==8.5.1"
+            "version": "==8.5.2"
         },
         "zipp": {
             "markers": "python_version < '3.10'"
         }
     }
 }
```

### Comparing `mkdocs_puml-1.3.0/README.md` & `mkdocs_puml-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.3.0/mkdocs_puml/encoder.py` & `mkdocs_puml-1.3.1/mkdocs_puml/encoder.py`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.3.0/mkdocs_puml/plugin.py` & `mkdocs_puml-1.3.1/mkdocs_puml/plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         for v in schemes:
             output = self._replace(v, output)
             page.content = self._replace(v, page.content)
 
             # MkDocs >=1.4 doesn't have html attribute.
             # This is required for integration with mkdocs-print-page plugin.
             # TODO: Remove the support of older versions in future releases
-            if hasattr(page, 'html'):
+            if hasattr(page, 'html') and page.html is not None:
                 page.html = self._replace(v, page.html)
 
         return output
 
     def _replace(self, key: str, content: str) -> str:
         """Replace a UUID key with a real diagram in a
         content
```

### Comparing `mkdocs_puml-1.3.0/mkdocs_puml/puml.py` & `mkdocs_puml-1.3.1/mkdocs_puml/puml.py`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.3.0/pyproject.toml` & `mkdocs_puml-1.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.3.0/tests/conftest.py` & `mkdocs_puml-1.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.3.0/tests/plugins/conftest.py` & `mkdocs_puml-1.3.1/tests/plugins/conftest.py`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.3.0/tests/plugins/test_plugin.py` & `mkdocs_puml-1.3.1/tests/plugins/test_plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.3.0/tests/test_puml.py` & `mkdocs_puml-1.3.1/tests/test_puml.py`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.3.0/tests/testdata/markdown.md` & `mkdocs_puml-1.3.1/tests/testdata/markdown.md`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.3.0/tests/testdata/plantuml.svg` & `mkdocs_puml-1.3.1/tests/testdata/plantuml.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.3.0/PKG-INFO` & `mkdocs_puml-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs_puml
-Version: 1.3.0
+Version: 1.3.1
 Summary: Package that brings PlantUML to MkDocs
 Author-email: Mikhail Kravets <michkravets@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: requests >= 2.27, < 3.0
 Requires-Dist: markdown >= 3.2.1, < 4.0
```

