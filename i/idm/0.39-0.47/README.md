# Comparing `tmp/idm-0.39.tar.gz` & `tmp/idm-0.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\idm-0.39.tar", last modified: Sun Aug  9 06:36:14 2020, max compression
+gzip compressed data, was "idm-0.47.tar", last modified: Wed May 15 07:14:39 2024, max compression
```

## Comparing `idm-0.39.tar` & `idm-0.47.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2020-08-09 06:36:14.000000 idm-0.39/
--rw-rw-rw-   0        0        0     1885 2020-02-12 11:19:05.000000 idm-0.39/LICENSE.rst
--rw-rw-rw-   0        0        0     2810 2020-08-09 06:36:14.000000 idm-0.39/PKG-INFO
--rw-rw-rw-   0        0        0     1229 2020-08-09 06:34:46.000000 idm-0.39/README.rst
--rw-rw-rw-   0        0        0       14 2020-08-09 06:02:15.000000 idm-0.39/__version__.py
-drwxrwxrwx   0        0        0        0 2020-08-09 06:36:14.000000 idm-0.39/idm/
--rw-rw-rw-   0        0        0      185 2020-02-12 11:19:24.000000 idm-0.39/idm/__init__.py
--rw-rw-rw-   0        0        0       58 2020-02-12 11:19:05.000000 idm-0.39/idm/__main__.py
--rw-rw-rw-   0        0        0       14 2020-08-09 06:02:15.000000 idm-0.39/idm/__version__.py
--rw-rw-rw-   0        0        0     3015 2020-08-09 06:01:57.000000 idm-0.39/idm/idm.py
-drwxrwxrwx   0        0        0        0 2020-08-09 06:36:14.000000 idm-0.39/idm.egg-info/
--rw-rw-rw-   0        0        0     2810 2020-08-09 06:36:13.000000 idm-0.39/idm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2020-08-09 06:36:13.000000 idm-0.39/idm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-08-09 06:36:13.000000 idm-0.39/idm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2020-08-09 06:36:13.000000 idm-0.39/idm.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2020-08-09 06:36:13.000000 idm-0.39/idm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2020-08-09 06:36:13.000000 idm-0.39/idm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      163 2020-08-09 06:36:14.000000 idm-0.39/setup.cfg
--rw-rw-rw-   0        0        0     2048 2020-02-12 11:19:05.000000 idm-0.39/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:14:39.852871 idm-0.47/
+-rw-rw-rw-   0        0        0     1626 2024-05-15 05:51:48.000000 idm-0.47/LICENSE.rst
+-rw-rw-rw-   0        0        0     2791 2024-05-15 07:14:39.853875 idm-0.47/PKG-INFO
+-rw-rw-rw-   0        0        0     1840 2024-05-15 06:02:22.000000 idm-0.47/README.md
+-rw-rw-rw-   0        0        0       16 2024-05-15 07:13:53.000000 idm-0.47/__version__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:14:39.824032 idm-0.47/idm/
+-rw-rw-rw-   0        0        0      185 2024-05-15 04:50:30.000000 idm-0.47/idm/__init__.py
+-rw-rw-rw-   0        0        0       58 2024-05-15 04:50:30.000000 idm-0.47/idm/__main__.py
+-rw-rw-rw-   0        0        0       16 2024-05-15 07:13:53.000000 idm-0.47/idm/__version__.py
+-rw-rw-rw-   0        0        0     5195 2024-05-15 05:38:44.000000 idm-0.47/idm/idm.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:14:39.851872 idm-0.47/idm.egg-info/
+-rw-rw-rw-   0        0        0     2791 2024-05-15 07:14:39.000000 idm-0.47/idm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2024-05-15 07:14:39.000000 idm-0.47/idm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 07:14:39.000000 idm-0.47/idm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-05-15 07:14:39.000000 idm-0.47/idm.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      103 2024-05-15 07:14:39.000000 idm-0.47/idm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-15 07:14:39.000000 idm-0.47/idm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      164 2024-05-15 07:14:39.855413 idm-0.47/setup.cfg
+-rw-rw-rw-   0        0        0     2321 2024-05-15 07:13:41.000000 idm-0.47/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `idm-0.39/LICENSE.rst` & `idm-0.47/LICENSE.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright © 2019 by the cumulus13 team.
+Copyright © 2019-2024 by the cumulus13 team.
 
 Some rights reserved.
 
 Redistribution and use in source and binary forms of the software as
 well as documentation, with or without modification, are permitted
 provided that the following conditions are met:
 
@@ -24,16 +24,8 @@
 COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT,
 INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT
 NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF
 USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF
 THIS SOFTWARE AND DOCUMENTATION, EVEN IF ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGE.
-
-----
-
-idm uses parts of optparse written by Hadi Cahyadi, LD. Ward and maintained
-by the Python Software Foundation.
-
-Copyright © 2017-2019 Hadi Cahyadi, LD. All rights reserved.
-Copyright © 2002-2006 Python Software Foundation. All rights reserved.
+SUCH DAMAGE.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+iso-8859-1
```

