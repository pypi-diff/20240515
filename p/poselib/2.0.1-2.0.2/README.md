# Comparing `tmp/poselib-2.0.1-pp39-pypy39_pp73-win_amd64.whl.zip` & `tmp/poselib-2.0.2-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,10 @@
-Zip file size: 679108 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat  2292736 b- defN 24-Mar-09 12:59 poselib.pypy39-pp73-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1551 b- defN 24-Mar-09 12:59 poselib-2.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      162 b- defN 24-Mar-09 12:59 poselib-2.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      107 b- defN 24-Mar-09 12:59 poselib-2.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 24-Mar-09 12:59 poselib-2.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      479 b- defN 24-Mar-09 12:59 poselib-2.0.1.dist-info/RECORD
-6 files, 2295045 bytes uncompressed, 678246 bytes compressed:  70.4%
+Zip file size: 1078153 bytes, number of entries: 8
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-15 07:22 poselib-2.0.2.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-15 07:22 poselib.libs/
+-rwxr-xr-x  2.0 unx  3513736 b- defN 24-May-15 07:22 poselib.cpython-311-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx     1522 b- defN 24-May-15 07:22 poselib-2.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      176 b- defN 24-May-15 07:22 poselib-2.0.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx      491 b- defN 24-May-15 07:22 poselib-2.0.2.dist-info/RECORD
+-rw-r--r--  2.0 unx       10 b- defN 24-May-15 07:22 poselib-2.0.2.dist-info/top_level.txt
+-rw-r--r--  2.0 unx      152 b- defN 24-May-15 07:22 poselib-2.0.2.dist-info/WHEEL
+8 files, 3516087 bytes uncompressed, 1077053 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -1,19 +1,25 @@
-Filename: poselib.pypy39-pp73-win_amd64.pyd
+Filename: poselib-2.0.2.dist-info/
 Comment: 
 
-Filename: poselib-2.0.1.dist-info/LICENSE
+Filename: poselib.libs/
 Comment: 
 
-Filename: poselib-2.0.1.dist-info/METADATA
+Filename: poselib.cpython-311-x86_64-linux-gnu.so
 Comment: 
 
-Filename: poselib-2.0.1.dist-info/WHEEL
+Filename: poselib-2.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: poselib-2.0.1.dist-info/top_level.txt
+Filename: poselib-2.0.2.dist-info/METADATA
 Comment: 
 
-Filename: poselib-2.0.1.dist-info/RECORD
+Filename: poselib-2.0.2.dist-info/RECORD
+Comment: 
+
+Filename: poselib-2.0.2.dist-info/top_level.txt
+Comment: 
+
+Filename: poselib-2.0.2.dist-info/WHEEL
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## Comparing `poselib-2.0.1.dist-info/LICENSE` & `poselib-2.0.2.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-BSD 3-Clause License
-
-Copyright (c) 2020, Viktor Larsson
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 3-Clause License
+
+Copyright (c) 2020, Viktor Larsson
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

