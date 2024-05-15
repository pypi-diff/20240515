# Comparing `tmp/juntagrico-pg-1.5.0.tar.gz` & `tmp/juntagrico_pg-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\juntagrico-pg-1.5.0.tar", last modified: Tue Feb  8 09:32:23 2022, max compression
+gzip compressed data, was "juntagrico_pg-1.6.0.tar", last modified: Wed May 15 19:41:10 2024, max compression
```

## Comparing `juntagrico-pg-1.5.0.tar` & `juntagrico_pg-1.6.0.tar`

### file list

```diff
@@ -1,36 +1,33 @@
-drwxrwxrwx   0        0        0        0 2022-02-08 09:32:23.479748 juntagrico-pg-1.5.0/
--rw-rw-rw-   0        0        0     7816 2019-10-06 17:57:05.000000 juntagrico-pg-1.5.0/LICENSE
--rw-rw-rw-   0        0        0      212 2021-05-02 19:34:14.000000 juntagrico-pg-1.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2895 2022-02-08 09:32:23.479748 juntagrico-pg-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     1820 2021-05-02 19:34:14.000000 juntagrico-pg-1.5.0/README.md
-drwxrwxrwx   0        0        0        0 2022-02-08 09:32:23.322748 juntagrico-pg-1.5.0/juntagrico_pg/
--rw-rw-rw-   0        0        0       43 2022-02-08 09:32:03.000000 juntagrico-pg-1.5.0/juntagrico_pg/__init__.py
--rw-rw-rw-   0        0        0        0 2021-03-23 19:14:44.000000 juntagrico-pg-1.5.0/juntagrico_pg/admin.py
-drwxrwxrwx   0        0        0        0 2022-02-08 09:32:23.379757 juntagrico-pg-1.5.0/juntagrico_pg/dao/
--rw-rw-rw-   0        0        0        0 2019-10-06 17:57:05.000000 juntagrico-pg-1.5.0/juntagrico_pg/dao/__init__.py
-drwxrwxrwx   0        0        0        0 2022-02-08 09:32:23.381761 juntagrico-pg-1.5.0/juntagrico_pg/entity/
--rw-rw-rw-   0        0        0        0 2019-10-06 17:57:05.000000 juntagrico-pg-1.5.0/juntagrico_pg/entity/__init__.py
--rw-rw-rw-   0        0        0      326 2021-05-02 19:38:52.000000 juntagrico-pg-1.5.0/juntagrico_pg/juntagricoapp.py
-drwxrwxrwx   0        0        0        0 2022-02-08 09:32:23.413766 juntagrico-pg-1.5.0/juntagrico_pg/migrations/
--rw-rw-rw-   0        0        0      561 2019-10-07 07:41:45.000000 juntagrico-pg-1.5.0/juntagrico_pg/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      394 2019-10-07 08:31:43.000000 juntagrico-pg-1.5.0/juntagrico_pg/migrations/0002_auto_20191007_1031.py
--rw-rw-rw-   0        0        0        0 2019-10-06 17:57:05.000000 juntagrico-pg-1.5.0/juntagrico_pg/migrations/__init__.py
--rw-rw-rw-   0        0        0      259 2019-10-07 08:31:34.000000 juntagrico-pg-1.5.0/juntagrico_pg/models.py
-drwxrwxrwx   0        0        0        0 2022-02-08 09:32:23.271747 juntagrico-pg-1.5.0/juntagrico_pg/templates/
-drwxrwxrwx   0        0        0        0 2022-02-08 09:32:23.449747 juntagrico-pg-1.5.0/juntagrico_pg/templates/jpg/
--rw-rw-rw-   0        0        0     1473 2021-05-02 19:34:14.000000 juntagrico-pg-1.5.0/juntagrico_pg/templates/jpg/home.html
--rw-rw-rw-   0        0        0      136 2021-05-02 19:38:52.000000 juntagrico-pg-1.5.0/juntagrico_pg/templates/jpg/menu.html
--rw-rw-rw-   0        0        0      162 2019-10-07 07:51:27.000000 juntagrico-pg-1.5.0/juntagrico_pg/urls.py
-drwxrwxrwx   0        0        0        0 2022-02-08 09:32:23.477747 juntagrico-pg-1.5.0/juntagrico_pg/util/
--rw-rw-rw-   0        0        0        0 2019-10-06 17:57:05.000000 juntagrico-pg-1.5.0/juntagrico_pg/util/__init__.py
--rw-rw-rw-   0        0        0      554 2020-01-02 22:20:08.000000 juntagrico-pg-1.5.0/juntagrico_pg/util/output.py
--rw-rw-rw-   0        0        0      969 2021-05-02 19:38:52.000000 juntagrico-pg-1.5.0/juntagrico_pg/views.py
-drwxrwxrwx   0        0        0        0 2022-02-08 09:32:23.372752 juntagrico-pg-1.5.0/juntagrico_pg.egg-info/
--rw-rw-rw-   0        0        0     2895 2022-02-08 09:32:23.000000 juntagrico-pg-1.5.0/juntagrico_pg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      727 2022-02-08 09:32:23.000000 juntagrico-pg-1.5.0/juntagrico_pg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-02-08 09:32:23.000000 juntagrico-pg-1.5.0/juntagrico_pg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2022-02-08 09:32:23.000000 juntagrico-pg-1.5.0/juntagrico_pg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2022-02-08 09:32:23.000000 juntagrico-pg-1.5.0/juntagrico_pg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       56 2022-02-08 09:30:59.000000 juntagrico-pg-1.5.0/requirements.txt
--rw-rw-rw-   0        0        0       75 2022-02-08 09:32:23.482747 juntagrico-pg-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1629 2021-05-02 19:34:14.000000 juntagrico-pg-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:41:10.526907 juntagrico_pg-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-15 19:41:04.000000 juntagrico_pg-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-15 19:41:04.000000 juntagrico_pg-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12093 2024-05-15 19:41:10.522907 juntagrico_pg-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-15 19:41:04.000000 juntagrico_pg-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:41:10.522907 juntagrico_pg-1.6.0/juntagrico_pg/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 19:41:04.000000 juntagrico_pg-1.6.0/juntagrico_pg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-15 19:41:04.000000 juntagrico_pg-1.6.0/juntagrico_pg/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:41:10.522907 juntagrico_pg-1.6.0/juntagrico_pg/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-15 19:41:04.000000 juntagrico_pg-1.6.0/juntagrico_pg/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-15 19:41:04.000000 juntagrico_pg-1.6.0/juntagrico_pg/migrations/0002_auto_20191007_1031.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:41:04.000000 juntagrico_pg-1.6.0/juntagrico_pg/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-15 19:41:04.000000 juntagrico_pg-1.6.0/juntagrico_pg/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:41:10.518907 juntagrico_pg-1.6.0/juntagrico_pg/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:41:10.522907 juntagrico_pg-1.6.0/juntagrico_pg/templates/jpg/
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-15 19:41:04.000000 juntagrico_pg-1.6.0/juntagrico_pg/templates/jpg/home.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:41:10.518907 juntagrico_pg-1.6.0/juntagrico_pg/templates/juntagrico/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:41:10.522907 juntagrico_pg-1.6.0/juntagrico_pg/templates/juntagrico/menu/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-15 19:41:04.000000 juntagrico_pg-1.6.0/juntagrico_pg/templates/juntagrico/menu/admin.html
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-15 19:41:04.000000 juntagrico_pg-1.6.0/juntagrico_pg/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:41:10.522907 juntagrico_pg-1.6.0/juntagrico_pg/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:41:04.000000 juntagrico_pg-1.6.0/juntagrico_pg/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-15 19:41:04.000000 juntagrico_pg-1.6.0/juntagrico_pg/util/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-15 19:41:04.000000 juntagrico_pg-1.6.0/juntagrico_pg/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:41:10.522907 juntagrico_pg-1.6.0/juntagrico_pg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12093 2024-05-15 19:41:10.000000 juntagrico_pg-1.6.0/juntagrico_pg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-15 19:41:10.000000 juntagrico_pg-1.6.0/juntagrico_pg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 19:41:10.000000 juntagrico_pg-1.6.0/juntagrico_pg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-15 19:41:10.000000 juntagrico_pg-1.6.0/juntagrico_pg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 19:41:10.000000 juntagrico_pg-1.6.0/juntagrico_pg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-15 19:41:04.000000 juntagrico_pg-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 19:41:04.000000 juntagrico_pg-1.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 19:41:10.526907 juntagrico_pg-1.6.0/setup.cfg
```

### Comparing `juntagrico-pg-1.5.0/LICENSE` & `juntagrico_pg-1.6.0/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,165 +1,165 @@
-                   GNU LESSER GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-
-  This version of the GNU Lesser General Public License incorporates
-the terms and conditions of version 3 of the GNU General Public
-License, supplemented by the additional permissions listed below.
-
-  0. Additional Definitions.
-
-  As used herein, "this License" refers to version 3 of the GNU Lesser
-General Public License, and the "GNU GPL" refers to version 3 of the GNU
-General Public License.
-
-  "The Library" refers to a covered work governed by this License,
-other than an Application or a Combined Work as defined below.
-
-  An "Application" is any work that makes use of an interface provided
-by the Library, but which is not otherwise based on the Library.
-Defining a subclass of a class defined by the Library is deemed a mode
-of using an interface provided by the Library.
-
-  A "Combined Work" is a work produced by combining or linking an
-Application with the Library.  The particular version of the Library
-with which the Combined Work was made is also called the "Linked
-Version".
-
-  The "Minimal Corresponding Source" for a Combined Work means the
-Corresponding Source for the Combined Work, excluding any source code
-for portions of the Combined Work that, considered in isolation, are
-based on the Application, and not on the Linked Version.
-
-  The "Corresponding Application Code" for a Combined Work means the
-object code and/or source code for the Application, including any data
-and utility programs needed for reproducing the Combined Work from the
-Application, but excluding the System Libraries of the Combined Work.
-
-  1. Exception to Section 3 of the GNU GPL.
-
-  You may convey a covered work under sections 3 and 4 of this License
-without being bound by section 3 of the GNU GPL.
-
-  2. Conveying Modified Versions.
-
-  If you modify a copy of the Library, and, in your modifications, a
-facility refers to a function or data to be supplied by an Application
-that uses the facility (other than as an argument passed when the
-facility is invoked), then you may convey a copy of the modified
-version:
-
-   a) under this License, provided that you make a good faith effort to
-   ensure that, in the event an Application does not supply the
-   function or data, the facility still operates, and performs
-   whatever part of its purpose remains meaningful, or
-
-   b) under the GNU GPL, with none of the additional permissions of
-   this License applicable to that copy.
-
-  3. Object Code Incorporating Material from Library Header Files.
-
-  The object code form of an Application may incorporate material from
-a header file that is part of the Library.  You may convey such object
-code under terms of your choice, provided that, if the incorporated
-material is not limited to numerical parameters, data structure
-layouts and accessors, or small macros, inline functions and templates
-(ten or fewer lines in length), you do both of the following:
-
-   a) Give prominent notice with each copy of the object code that the
-   Library is used in it and that the Library and its use are
-   covered by this License.
-
-   b) Accompany the object code with a copy of the GNU GPL and this license
-   document.
-
-  4. Combined Works.
-
-  You may convey a Combined Work under terms of your choice that,
-taken together, effectively do not restrict modification of the
-portions of the Library contained in the Combined Work and reverse
-engineering for debugging such modifications, if you also do each of
-the following:
-
-   a) Give prominent notice with each copy of the Combined Work that
-   the Library is used in it and that the Library and its use are
-   covered by this License.
-
-   b) Accompany the Combined Work with a copy of the GNU GPL and this license
-   document.
-
-   c) For a Combined Work that displays copyright notices during
-   execution, include the copyright notice for the Library among
-   these notices, as well as a reference directing the user to the
-   copies of the GNU GPL and this license document.
-
-   d) Do one of the following:
-
-       0) Convey the Minimal Corresponding Source under the terms of this
-       License, and the Corresponding Application Code in a form
-       suitable for, and under terms that permit, the user to
-       recombine or relink the Application with a modified version of
-       the Linked Version to produce a modified Combined Work, in the
-       manner specified by section 6 of the GNU GPL for conveying
-       Corresponding Source.
-
-       1) Use a suitable shared library mechanism for linking with the
-       Library.  A suitable mechanism is one that (a) uses at run time
-       a copy of the Library already present on the user's computer
-       system, and (b) will operate properly with a modified version
-       of the Library that is interface-compatible with the Linked
-       Version.
-
-   e) Provide Installation Information, but only if you would otherwise
-   be required to provide such information under section 6 of the
-   GNU GPL, and only to the extent that such information is
-   necessary to install and execute a modified version of the
-   Combined Work produced by recombining or relinking the
-   Application with a modified version of the Linked Version. (If
-   you use option 4d0, the Installation Information must accompany
-   the Minimal Corresponding Source and Corresponding Application
-   Code. If you use option 4d1, you must provide the Installation
-   Information in the manner specified by section 6 of the GNU GPL
-   for conveying Corresponding Source.)
-
-  5. Combined Libraries.
-
-  You may place library facilities that are a work based on the
-Library side by side in a single library together with other library
-facilities that are not Applications and are not covered by this
-License, and convey such a combined library under terms of your
-choice, if you do both of the following:
-
-   a) Accompany the combined library with a copy of the same work based
-   on the Library, uncombined with any other library facilities,
-   conveyed under the terms of this License.
-
-   b) Give prominent notice with the combined library that part of it
-   is a work based on the Library, and explaining where to find the
-   accompanying uncombined form of the same work.
-
-  6. Revised Versions of the GNU Lesser General Public License.
-
-  The Free Software Foundation may publish revised and/or new versions
-of the GNU Lesser General Public License from time to time. Such new
-versions will be similar in spirit to the present version, but may
-differ in detail to address new problems or concerns.
-
-  Each version is given a distinguishing version number. If the
-Library as you received it specifies that a certain numbered version
-of the GNU Lesser General Public License "or any later version"
-applies to it, you have the option of following the terms and
-conditions either of that published version or of any later version
-published by the Free Software Foundation. If the Library as you
-received it does not specify a version number of the GNU Lesser
-General Public License, you may choose any version of the GNU Lesser
-General Public License ever published by the Free Software Foundation.
-
-  If the Library as you received it specifies that a proxy can decide
-whether future versions of the GNU Lesser General Public License shall
-apply, that proxy's public statement of acceptance of any version is
-permanent authorization for you to choose that version for the
-Library.
+                   GNU LESSER GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+
+  This version of the GNU Lesser General Public License incorporates
+the terms and conditions of version 3 of the GNU General Public
+License, supplemented by the additional permissions listed below.
+
+  0. Additional Definitions.
+
+  As used herein, "this License" refers to version 3 of the GNU Lesser
+General Public License, and the "GNU GPL" refers to version 3 of the GNU
+General Public License.
+
+  "The Library" refers to a covered work governed by this License,
+other than an Application or a Combined Work as defined below.
+
+  An "Application" is any work that makes use of an interface provided
+by the Library, but which is not otherwise based on the Library.
+Defining a subclass of a class defined by the Library is deemed a mode
+of using an interface provided by the Library.
+
+  A "Combined Work" is a work produced by combining or linking an
+Application with the Library.  The particular version of the Library
+with which the Combined Work was made is also called the "Linked
+Version".
+
+  The "Minimal Corresponding Source" for a Combined Work means the
+Corresponding Source for the Combined Work, excluding any source code
+for portions of the Combined Work that, considered in isolation, are
+based on the Application, and not on the Linked Version.
+
+  The "Corresponding Application Code" for a Combined Work means the
+object code and/or source code for the Application, including any data
+and utility programs needed for reproducing the Combined Work from the
+Application, but excluding the System Libraries of the Combined Work.
+
+  1. Exception to Section 3 of the GNU GPL.
+
+  You may convey a covered work under sections 3 and 4 of this License
+without being bound by section 3 of the GNU GPL.
+
+  2. Conveying Modified Versions.
+
+  If you modify a copy of the Library, and, in your modifications, a
+facility refers to a function or data to be supplied by an Application
+that uses the facility (other than as an argument passed when the
+facility is invoked), then you may convey a copy of the modified
+version:
+
+   a) under this License, provided that you make a good faith effort to
+   ensure that, in the event an Application does not supply the
+   function or data, the facility still operates, and performs
+   whatever part of its purpose remains meaningful, or
+
+   b) under the GNU GPL, with none of the additional permissions of
+   this License applicable to that copy.
+
+  3. Object Code Incorporating Material from Library Header Files.
+
+  The object code form of an Application may incorporate material from
+a header file that is part of the Library.  You may convey such object
+code under terms of your choice, provided that, if the incorporated
+material is not limited to numerical parameters, data structure
+layouts and accessors, or small macros, inline functions and templates
+(ten or fewer lines in length), you do both of the following:
+
+   a) Give prominent notice with each copy of the object code that the
+   Library is used in it and that the Library and its use are
+   covered by this License.
+
+   b) Accompany the object code with a copy of the GNU GPL and this license
+   document.
+
+  4. Combined Works.
+
+  You may convey a Combined Work under terms of your choice that,
+taken together, effectively do not restrict modification of the
+portions of the Library contained in the Combined Work and reverse
+engineering for debugging such modifications, if you also do each of
+the following:
+
+   a) Give prominent notice with each copy of the Combined Work that
+   the Library is used in it and that the Library and its use are
+   covered by this License.
+
+   b) Accompany the Combined Work with a copy of the GNU GPL and this license
+   document.
+
+   c) For a Combined Work that displays copyright notices during
+   execution, include the copyright notice for the Library among
+   these notices, as well as a reference directing the user to the
+   copies of the GNU GPL and this license document.
+
+   d) Do one of the following:
+
+       0) Convey the Minimal Corresponding Source under the terms of this
+       License, and the Corresponding Application Code in a form
+       suitable for, and under terms that permit, the user to
+       recombine or relink the Application with a modified version of
+       the Linked Version to produce a modified Combined Work, in the
+       manner specified by section 6 of the GNU GPL for conveying
+       Corresponding Source.
+
+       1) Use a suitable shared library mechanism for linking with the
+       Library.  A suitable mechanism is one that (a) uses at run time
+       a copy of the Library already present on the user's computer
+       system, and (b) will operate properly with a modified version
+       of the Library that is interface-compatible with the Linked
+       Version.
+
+   e) Provide Installation Information, but only if you would otherwise
+   be required to provide such information under section 6 of the
+   GNU GPL, and only to the extent that such information is
+   necessary to install and execute a modified version of the
+   Combined Work produced by recombining or relinking the
+   Application with a modified version of the Linked Version. (If
+   you use option 4d0, the Installation Information must accompany
+   the Minimal Corresponding Source and Corresponding Application
+   Code. If you use option 4d1, you must provide the Installation
+   Information in the manner specified by section 6 of the GNU GPL
+   for conveying Corresponding Source.)
+
+  5. Combined Libraries.
+
+  You may place library facilities that are a work based on the
+Library side by side in a single library together with other library
+facilities that are not Applications and are not covered by this
+License, and convey such a combined library under terms of your
+choice, if you do both of the following:
+
+   a) Accompany the combined library with a copy of the same work based
+   on the Library, uncombined with any other library facilities,
+   conveyed under the terms of this License.
+
+   b) Give prominent notice with the combined library that part of it
+   is a work based on the Library, and explaining where to find the
+   accompanying uncombined form of the same work.
+
+  6. Revised Versions of the GNU Lesser General Public License.
+
+  The Free Software Foundation may publish revised and/or new versions
+of the GNU Lesser General Public License from time to time. Such new
+versions will be similar in spirit to the present version, but may
+differ in detail to address new problems or concerns.
+
+  Each version is given a distinguishing version number. If the
+Library as you received it specifies that a certain numbered version
+of the GNU Lesser General Public License "or any later version"
+applies to it, you have the option of following the terms and
+conditions either of that published version or of any later version
+published by the Free Software Foundation. If the Library as you
+received it does not specify a version number of the GNU Lesser
+General Public License, you may choose any version of the GNU Lesser
+General Public License ever published by the Free Software Foundation.
+
+  If the Library as you received it specifies that a proxy can decide
+whether future versions of the GNU Lesser General Public License shall
+apply, that proxy's public statement of acceptance of any version is
+permanent authorization for you to choose that version for the
+Library.
```

### Comparing `juntagrico-pg-1.5.0/PKG-INFO` & `juntagrico_pg-1.6.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,45 @@
-Metadata-Version: 1.1
-Name: juntagrico-pg
-Version: 1.5.0
-Summary: juntagrico-pg
-Home-page: http://juntagrico.org
-Author: juntagrico
-Author-email: info@juntagrico.org
-License: LPGLv3
-Description: # juntagrico-pg
-        
-        
-        [![juntagrico-ci](https://github.com/juntagrico/juntagrico-pg/actions/workflows/juntagrico-ci.yml/badge.svg?branch=main&event=push)](https://github.com/juntagrico/juntagrico-pg/actions/workflows/juntagrico-ci.yml)
-        [![Maintainability](https://api.codeclimate.com/v1/badges/02bb5f131cc157fcc4b9/maintainability)](https://codeclimate.com/github/juntagrico/juntagrico-pg/maintainability)
-        [![Test Coverage](https://api.codeclimate.com/v1/badges/02bb5f131cc157fcc4b9/test_coverage)](https://codeclimate.com/github/juntagrico/juntagrico-pg/test_coverage)
-        [![image](https://img.shields.io/pypi/v/juntagrico-pg.svg)](https://pypi.python.org/pypi/juntagrico-pg)
-        [![image](https://img.shields.io/pypi/l/juntagrico-pg.svg)](https://pypi.python.org/pypi/juntagrico-pg)
-        [![image](https://img.shields.io/pypi/pyversions/juntagrico-pg.svg)](https://pypi.python.org/pypi/juntagrico-pg)
-        [![image](https://img.shields.io/pypi/status/juntagrico-pg.svg)](https://pypi.python.org/pypi/juntagrico-pg)
-        [![image](https://img.shields.io/pypi/dm/juntagrico-pg.svg)](https://pypi.python.org/pypi/juntagrico-pg/)
-        [![image](https://img.shields.io/github/last-commit/juntagrico/juntagrico-pg.svg)](https://github.com/juntagrico/juntagrico-pg)
-        [![image](https://img.shields.io/github/commit-activity/y/juntagrico/juntagrico-pg)](https://github.com/juntagrico/juntagrico-pg)
-        [![Requirements Status](https://requires.io/github/juntagrico/juntagrico-pg/requirements.svg?branch=main)](https://requires.io/github/juntagrico/juntagrico-pg/requirements/?branch=main)
-        
-        postgres db editor for juntagrico.
-        
-        This is an extension for juntagrico. You can find more information about juntagrico here
-        (https://github.com/juntagrico/juntagrico)
-        
-        For more information information about how to install this app hop over to the doc section of the repo.
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.1
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Other Audience
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 
-Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
+# juntagrico-pg
+
+
+[![juntagrico-ci](https://github.com/juntagrico/juntagrico-pg/actions/workflows/juntagrico-ci.yml/badge.svg?branch=main&event=push)](https://github.com/juntagrico/juntagrico-pg/actions/workflows/juntagrico-ci.yml)
+[![Maintainability](https://api.codeclimate.com/v1/badges/02bb5f131cc157fcc4b9/maintainability)](https://codeclimate.com/github/juntagrico/juntagrico-pg/maintainability)
+[![Test Coverage](https://api.codeclimate.com/v1/badges/02bb5f131cc157fcc4b9/test_coverage)](https://codeclimate.com/github/juntagrico/juntagrico-pg/test_coverage)
+[![image](https://img.shields.io/pypi/v/juntagrico-pg.svg)](https://pypi.python.org/pypi/juntagrico-pg)
+[![image](https://img.shields.io/pypi/l/juntagrico-pg.svg)](https://pypi.python.org/pypi/juntagrico-pg)
+[![image](https://img.shields.io/pypi/pyversions/juntagrico-pg.svg)](https://pypi.python.org/pypi/juntagrico-pg)
+[![image](https://img.shields.io/pypi/status/juntagrico-pg.svg)](https://pypi.python.org/pypi/juntagrico-pg)
+[![image](https://img.shields.io/pypi/dm/juntagrico-pg.svg)](https://pypi.python.org/pypi/juntagrico-pg/)
+[![image](https://img.shields.io/github/last-commit/juntagrico/juntagrico-pg.svg)](https://github.com/juntagrico/juntagrico-pg)
+[![image](https://img.shields.io/github/commit-activity/y/juntagrico/juntagrico-pg)](https://github.com/juntagrico/juntagrico-pg)
+
+postgres db editor for juntagrico.
+
+This is an extension for juntagrico. You can find more information about juntagrico here
+(https://github.com/juntagrico/juntagrico)
+
+# Installation
+
+Install juntagrico-pg via `pip`
+
+    $ pip install juntagrico-pg
+
+or add it in your projects `requirements.txt`
+
+In `settings.py` add `'juntagrico_pg',` **before** juntagrico.
+
+```python
+INSTALLED_APPS = [
+    ...
+    'juntagrico_pg',
+    'juntagrico',
+]
+```
+
+In your `urls.py` you also need to extend the pattern:
+
+```python
+urlpatterns = [
+    ...
+    path('', include('juntagrico_pg.urls')),
+]
+```
```

### Comparing `juntagrico-pg-1.5.0/juntagrico_pg/templates/jpg/home.html` & `juntagrico_pg-1.6.0/juntagrico_pg/templates/jpg/home.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 {% extends "base.html" %}
+{% load i18n %}
 {% load juntagrico.config %}
 {% block page_title %}
     <h3>juntagrico-pg</h3>
 {% endblock %}
 
 {% block content %}
     <div class="row">
         <div class="col-md-12">
             <textarea id="textarea_id" wrap="off" rows="25" style="overflow-y: scroll; overflow-x: scroll; width: 100%; font-family: monospace; font-size: 0.75em; height: 100%">
             </textarea>
         </div>
     </div>
-    <div class="row mt-3">
-        <div class="col-md-9">
-            <form id="sql-form">
-                {% csrf_token %}
+    <form id="sql-form">
+        <div class="row mt-3">
+            {% csrf_token %}
+            <div class="col-md-9">
                 <input class="form-control" id="sql" name="sql">
-             </form>
+            </div>
+            <div class="col-md-3">
+                <input type="submit" class="btn btn-success" id="execute" value="{% trans "Ausführen" %}">
+            </div>
         </div>
-        <div class="col-md-3">
-            <button type="button" class="btn btn-success" id="execute">Execute</button>
-        </div>
-    </div>
+    </form>
 {% endblock %}
 {% block scripts %}
     <script>
         $(document).ready(function(){
-            $('.btn').on('click', function() {
+            $('#sql-form').on('submit', function() {
                 var textarea = $('#textarea_id');
                 textarea.val(textarea.val() + '\n\n' + $("#sql").val());
-                $.post( "/jpg/sql",
+                $.post( "{% url "jpg:sql" %}",
                     $("#sql-form").serialize(),
                     function( data ) {
                     var textarea = $('#textarea_id');
                     textarea.val(textarea.val() + '\n\n' + data);
                     textarea.scrollTop(textarea[0].scrollHeight);
                     $("#sql").val("")
                 });
+                return false
             });
         });
     </script>
 {% endblock %}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `juntagrico-pg-1.5.0/juntagrico_pg/views.py` & `juntagrico_pg-1.6.0/juntagrico_pg/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pgspecial.main import PGSpecial
 
 from juntagrico_pg.util.output import pretty_print
 
 
 @permission_required('juntagrico_pg.can_sql')
 def home(request):
-    return render(request, "jpg/home.html", {})
+    return render(request, "jpg/home.html")
 
 
 @permission_required('juntagrico_pg.can_sql')
 def execute_sql(request):
     if request.method != 'POST':
         raise Http404
     sql = request.POST.get('sql')
```

### Comparing `juntagrico-pg-1.5.0/juntagrico_pg.egg-info/SOURCES.txt` & `juntagrico_pg-1.6.0/juntagrico_pg.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 requirements.txt
-setup.cfg
-setup.py
 juntagrico_pg/__init__.py
-juntagrico_pg/admin.py
-juntagrico_pg/juntagricoapp.py
+juntagrico_pg/apps.py
 juntagrico_pg/models.py
 juntagrico_pg/urls.py
 juntagrico_pg/views.py
 juntagrico_pg.egg-info/PKG-INFO
 juntagrico_pg.egg-info/SOURCES.txt
 juntagrico_pg.egg-info/dependency_links.txt
 juntagrico_pg.egg-info/requires.txt
 juntagrico_pg.egg-info/top_level.txt
-juntagrico_pg/dao/__init__.py
-juntagrico_pg/entity/__init__.py
 juntagrico_pg/migrations/0001_initial.py
 juntagrico_pg/migrations/0002_auto_20191007_1031.py
 juntagrico_pg/migrations/__init__.py
 juntagrico_pg/templates/jpg/home.html
-juntagrico_pg/templates/jpg/menu.html
+juntagrico_pg/templates/juntagrico/menu/admin.html
 juntagrico_pg/util/__init__.py
 juntagrico_pg/util/output.py
```

