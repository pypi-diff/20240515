# Comparing `tmp/bisos.b-0.4.tar.gz` & `tmp/bisos.b-0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bisos.b-0.4.tar", last modified: Sat May 11 20:37:10 2024, max compression
+gzip compressed data, was "bisos.b-0.41.tar", last modified: Wed May 15 00:39:37 2024, max compression
```

## Comparing `bisos.b-0.4.tar` & `bisos.b-0.41.tar`

### file list

```diff
@@ -1,64 +1,149 @@
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 20:37:10.747785 bisos.b-0.4/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       71 2022-06-29 18:37:11.000000 bisos.b-0.4/MANIFEST.in
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     1451 2024-05-11 20:37:10.747785 bisos.b-0.4/PKG-INFO
--rw-rw-r--   0 bystar    (2001) bisos     (2222)      588 2024-05-11 20:37:10.000000 bisos.b-0.4/README.rst
--rw-rw-r--   0 bystar    (2001) bisos     (2222)      149 2022-06-29 18:37:11.000000 bisos.b-0.4/TITLE.txt
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 20:37:10.743785 bisos.b-0.4/bin/
--rwxrwxr-x   0 bystar    (2001) bisos     (2222)    19819 2022-09-05 19:26:17.000000 bisos.b-0.4/bin/csExamples.cs
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 20:37:10.743785 bisos.b-0.4/bisos/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       56 2022-06-29 18:37:11.000000 bisos.b-0.4/bisos/__init__.py
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 20:37:10.747785 bisos.b-0.4/bisos/b/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     1737 2024-01-31 20:57:45.000000 bisos.b-0.4/bisos/b/__init__.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    21226 2022-09-25 07:34:23.000000 bisos.b-0.4/bisos/b/ast.py
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 20:37:10.747785 bisos.b-0.4/bisos/b/b_io/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)      937 2022-09-24 22:01:52.000000 bisos.b-0.4/bisos/b/b_io/__init__.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     6660 2024-02-10 04:42:43.000000 bisos.b-0.4/bisos/b/b_io/ann.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    20187 2024-05-11 04:58:53.000000 bisos.b-0.4/bisos/b/b_io/eh.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     5690 2022-09-24 22:01:52.000000 bisos.b-0.4/bisos/b/b_io/io.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    19072 2022-09-25 22:24:52.000000 bisos.b-0.4/bisos/b/b_io/k1-eh.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    18680 2022-09-29 22:51:34.000000 bisos.b-0.4/bisos/b/b_io/log.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     6469 2022-09-24 22:01:52.000000 bisos.b-0.4/bisos/b/b_io/out.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     5458 2022-09-24 22:01:52.000000 bisos.b-0.4/bisos/b/b_io/stderr.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     5484 2022-09-24 22:01:52.000000 bisos.b-0.4/bisos/b/b_io/stdin.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     5164 2024-02-10 04:42:43.000000 bisos.b-0.4/bisos/b/b_io/stdout.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     7392 2022-09-25 22:17:29.000000 bisos.b-0.4/bisos/b/b_io/tm.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    14148 2022-09-24 22:27:10.000000 bisos.b-0.4/bisos/b/clsMethod_csu.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     4866 2022-09-27 05:11:31.000000 bisos.b-0.4/bisos/b/comment.py
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 20:37:10.747785 bisos.b-0.4/bisos/b/cs/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)      810 2022-09-24 22:06:28.000000 bisos.b-0.4/bisos/b/cs/__init__.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    15312 2022-09-24 22:06:28.000000 bisos.b-0.4/bisos/b/cs/arg.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    81313 2024-05-11 04:58:53.000000 bisos.b-0.4/bisos/b/cs/cs.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    29593 2024-05-11 04:58:53.000000 bisos.b-0.4/bisos/b/cs/examples.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    12803 2024-01-22 02:29:29.000000 bisos.b-0.4/bisos/b/cs/globalContext.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    41249 2022-09-24 22:06:28.000000 bisos.b-0.4/bisos/b/cs/inCmnd.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    73247 2024-02-09 01:54:18.000000 bisos.b-0.4/bisos/b/cs/k1-ro.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    11210 2022-11-26 05:16:19.000000 bisos.b-0.4/bisos/b/cs/main.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    21929 2024-05-11 04:58:53.000000 bisos.b-0.4/bisos/b/cs/param.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    97134 2024-05-11 20:35:17.000000 bisos.b-0.4/bisos/b/cs/ro.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     9270 2024-01-22 22:24:25.000000 bisos.b-0.4/bisos/b/cs/rpyc.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    12903 2022-09-24 22:06:28.000000 bisos.b-0.4/bisos/b/cs/rtInvoker.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    12636 2022-09-24 22:06:28.000000 bisos.b-0.4/bisos/b/cs/runArgs.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    17615 2022-09-25 17:31:18.000000 bisos.b-0.4/bisos/b/cs/track.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    11057 2022-09-24 22:27:10.000000 bisos.b-0.4/bisos/b/dir.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     7470 2022-09-24 22:27:10.000000 bisos.b-0.4/bisos/b/exception.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    42680 2024-02-01 19:53:47.000000 bisos.b-0.4/bisos/b/fp.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    54004 2024-05-11 04:58:53.000000 bisos.b-0.4/bisos/b/fpCls.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     8338 2022-10-04 19:54:17.000000 bisos.b-0.4/bisos/b/fpath.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    10387 2024-02-04 06:51:44.000000 bisos.b-0.4/bisos/b/fto.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     8464 2022-09-24 22:27:10.000000 bisos.b-0.4/bisos/b/fv.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     6672 2022-10-02 20:47:08.000000 bisos.b-0.4/bisos/b/importFile.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     9887 2022-09-29 19:54:59.000000 bisos.b-0.4/bisos/b/niche.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    15955 2024-05-11 04:58:53.000000 bisos.b-0.4/bisos/b/op.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    15728 2022-12-07 20:03:07.000000 bisos.b-0.4/bisos/b/pyRunAs.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    22794 2024-01-19 18:26:36.000000 bisos.b-0.4/bisos/b/subProc.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     7242 2022-09-24 22:27:10.000000 bisos.b-0.4/bisos/b/types.py
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 20:37:10.743785 bisos.b-0.4/bisos.b.egg-info/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     1451 2024-05-11 20:37:10.000000 bisos.b-0.4/bisos.b.egg-info/PKG-INFO
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     1107 2024-05-11 20:37:10.000000 bisos.b-0.4/bisos.b.egg-info/SOURCES.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        1 2024-05-11 20:37:10.000000 bisos.b-0.4/bisos.b.egg-info/dependency_links.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        1 2024-05-11 20:37:10.000000 bisos.b-0.4/bisos.b.egg-info/not-zip-safe
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       25 2024-05-11 20:37:10.000000 bisos.b-0.4/bisos.b.egg-info/requires.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        6 2024-05-11 20:37:10.000000 bisos.b-0.4/bisos.b.egg-info/top_level.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    35067 2024-05-11 20:37:10.000000 bisos.b-0.4/lh-agpl3-LICENSE.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       38 2024-05-11 20:37:10.747785 bisos.b-0.4/setup.cfg
--rwxrwxr-x   0 bystar    (2001) bisos     (2222)     1616 2024-05-11 20:35:17.000000 bisos.b-0.4/setup.py
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-15 00:39:37.673351 bisos.b-0.41/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       66 2024-05-15 00:38:43.000000 bisos.b-0.41/MANIFEST.in
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     7219 2024-05-15 00:39:37.673351 bisos.b-0.41/PKG-INFO
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     5840 2024-05-14 22:44:32.000000 bisos.b-0.41/README.org
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     5840 2024-05-14 22:44:32.000000 bisos.b-0.41/README.txt
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-15 00:39:37.657351 bisos.b-0.41/bisos/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       56 2022-06-29 18:37:11.000000 bisos.b-0.41/bisos/__init__.py
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-15 00:39:37.657351 bisos.b-0.41/bisos/b/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     1737 2024-01-31 20:57:45.000000 bisos.b-0.41/bisos/b/__init__.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    21226 2022-09-25 07:34:23.000000 bisos.b-0.41/bisos/b/ast.py
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-15 00:39:37.657351 bisos.b-0.41/bisos/b/b_io/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)      937 2022-09-24 22:01:52.000000 bisos.b-0.41/bisos/b/b_io/__init__.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     6660 2024-02-10 04:42:43.000000 bisos.b-0.41/bisos/b/b_io/ann.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    20187 2024-05-11 04:58:53.000000 bisos.b-0.41/bisos/b/b_io/eh.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     5690 2022-09-24 22:01:52.000000 bisos.b-0.41/bisos/b/b_io/io.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    19072 2022-09-25 22:24:52.000000 bisos.b-0.41/bisos/b/b_io/k1-eh.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    18680 2022-09-29 22:51:34.000000 bisos.b-0.41/bisos/b/b_io/log.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     6469 2022-09-24 22:01:52.000000 bisos.b-0.41/bisos/b/b_io/out.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     5458 2022-09-24 22:01:52.000000 bisos.b-0.41/bisos/b/b_io/stderr.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     5484 2022-09-24 22:01:52.000000 bisos.b-0.41/bisos/b/b_io/stdin.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     5164 2024-02-10 04:42:43.000000 bisos.b-0.41/bisos/b/b_io/stdout.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     7392 2022-09-25 22:17:29.000000 bisos.b-0.41/bisos/b/b_io/tm.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    14148 2022-09-24 22:27:10.000000 bisos.b-0.41/bisos/b/clsMethod_csu.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     4866 2022-09-27 05:11:31.000000 bisos.b-0.41/bisos/b/comment.py
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-15 00:39:37.661351 bisos.b-0.41/bisos/b/cs/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)      810 2022-09-24 22:06:28.000000 bisos.b-0.41/bisos/b/cs/__init__.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    15312 2022-09-24 22:06:28.000000 bisos.b-0.41/bisos/b/cs/arg.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    81313 2024-05-11 04:58:53.000000 bisos.b-0.41/bisos/b/cs/cs.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    29593 2024-05-11 04:58:53.000000 bisos.b-0.41/bisos/b/cs/examples.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    12803 2024-01-22 02:29:29.000000 bisos.b-0.41/bisos/b/cs/globalContext.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    41249 2022-09-24 22:06:28.000000 bisos.b-0.41/bisos/b/cs/inCmnd.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    73247 2024-02-09 01:54:18.000000 bisos.b-0.41/bisos/b/cs/k1-ro.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    11210 2022-11-26 05:16:19.000000 bisos.b-0.41/bisos/b/cs/main.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    21929 2024-05-11 04:58:53.000000 bisos.b-0.41/bisos/b/cs/param.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    97134 2024-05-11 20:35:17.000000 bisos.b-0.41/bisos/b/cs/ro.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     9270 2024-01-22 22:24:25.000000 bisos.b-0.41/bisos/b/cs/rpyc.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    12903 2022-09-24 22:06:28.000000 bisos.b-0.41/bisos/b/cs/rtInvoker.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    12636 2022-09-24 22:06:28.000000 bisos.b-0.41/bisos/b/cs/runArgs.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    17615 2022-09-25 17:31:18.000000 bisos.b-0.41/bisos/b/cs/track.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    11057 2022-09-24 22:27:10.000000 bisos.b-0.41/bisos/b/dir.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     7470 2022-09-24 22:27:10.000000 bisos.b-0.41/bisos/b/exception.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    42680 2024-02-01 19:53:47.000000 bisos.b-0.41/bisos/b/fp.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    54004 2024-05-11 04:58:53.000000 bisos.b-0.41/bisos/b/fpCls.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     8338 2022-10-04 19:54:17.000000 bisos.b-0.41/bisos/b/fpath.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    10387 2024-02-04 06:51:44.000000 bisos.b-0.41/bisos/b/fto.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     8464 2022-09-24 22:27:10.000000 bisos.b-0.41/bisos/b/fv.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     6672 2022-10-02 20:47:08.000000 bisos.b-0.41/bisos/b/importFile.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     9887 2022-09-29 19:54:59.000000 bisos.b-0.41/bisos/b/niche.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    15955 2024-05-11 04:58:53.000000 bisos.b-0.41/bisos/b/op.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    15728 2022-12-07 20:03:07.000000 bisos.b-0.41/bisos/b/pyRunAs.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    22794 2024-01-19 18:26:36.000000 bisos.b-0.41/bisos/b/subProc.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     7242 2022-09-24 22:27:10.000000 bisos.b-0.41/bisos/b/types.py
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-15 00:39:37.657351 bisos.b-0.41/bisos.b.egg-info/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     7219 2024-05-15 00:39:37.000000 bisos.b-0.41/bisos.b.egg-info/PKG-INFO
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     3727 2024-05-15 00:39:37.000000 bisos.b-0.41/bisos.b.egg-info/SOURCES.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        1 2024-05-15 00:39:37.000000 bisos.b-0.41/bisos.b.egg-info/dependency_links.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        1 2024-05-15 00:39:37.000000 bisos.b-0.41/bisos.b.egg-info/not-zip-safe
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       72 2024-05-15 00:39:37.000000 bisos.b-0.41/bisos.b.egg-info/requires.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        6 2024-05-15 00:39:37.000000 bisos.b-0.41/bisos.b.egg-info/top_level.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    35067 2024-05-15 00:39:36.000000 bisos.b-0.41/lh-agpl3-LICENSE.txt
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-15 00:39:37.661351 bisos.b-0.41/panels/
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-15 00:39:37.661351 bisos.b-0.41/panels/_nodeBase_/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       18 2024-01-10 00:22:33.000000 bisos.b-0.41/panels/_nodeBase_/_objectType_
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       11 2024-01-10 00:22:33.000000 bisos.b-0.41/panels/_nodeBase_/_treeProc_
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        5 2024-01-10 00:22:33.000000 bisos.b-0.41/panels/_nodeBase_/_tree_
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)     2296 2024-01-17 19:54:14.000000 bisos.b-0.41/panels/_nodeBase_/bleePanelProc.sh
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        0 2024-01-10 00:22:33.000000 bisos.b-0.41/panels/_nodeBase_/destDesc
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        0 2024-01-10 00:22:33.000000 bisos.b-0.41/panels/_nodeBase_/foldDesc
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)     5575 2024-01-17 19:54:12.000000 bisos.b-0.41/panels/_nodeBase_/ftoProc.sh
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    16677 2024-05-08 21:53:42.000000 bisos.b-0.41/panels/_nodeBase_/fullUsagePanel-en.org
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       18 2024-01-10 00:22:33.000000 bisos.b-0.41/panels/_objectType_
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       17 2024-01-10 00:22:33.000000 bisos.b-0.41/panels/_treeProc_
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        5 2024-01-10 00:22:33.000000 bisos.b-0.41/panels/_tree_
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-15 00:39:37.665351 bisos.b-0.41/panels/bisos.b.b_io/
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-15 00:39:37.665351 bisos.b-0.41/panels/bisos.b.b_io/_nodeBase_/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       18 2024-01-10 00:22:33.000000 bisos.b-0.41/panels/bisos.b.b_io/_nodeBase_/_objectType_
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       11 2024-01-10 00:22:33.000000 bisos.b-0.41/panels/bisos.b.b_io/_nodeBase_/_treeProc_
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        5 2024-01-10 00:22:33.000000 bisos.b-0.41/panels/bisos.b.b_io/_nodeBase_/_tree_
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)     2309 2024-01-17 19:53:53.000000 bisos.b-0.41/panels/bisos.b.b_io/_nodeBase_/bleePanelProc.sh
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        0 2024-01-10 00:22:33.000000 bisos.b-0.41/panels/bisos.b.b_io/_nodeBase_/destDesc
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        0 2024-01-10 00:22:33.000000 bisos.b-0.41/panels/bisos.b.b_io/_nodeBase_/foldDesc
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)     5588 2024-01-17 19:53:51.000000 bisos.b-0.41/panels/bisos.b.b_io/_nodeBase_/ftoProc.sh
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    12365 2024-02-10 05:38:34.000000 bisos.b-0.41/panels/bisos.b.b_io/_nodeBase_/fullUsagePanel-en.org
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       18 2024-01-10 00:22:33.000000 bisos.b-0.41/panels/bisos.b.b_io/_objectType_
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       17 2024-01-10 00:22:33.000000 bisos.b-0.41/panels/bisos.b.b_io/_treeProc_
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        5 2024-01-10 00:22:33.000000 bisos.b-0.41/panels/bisos.b.b_io/_tree_
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)     2298 2024-01-17 19:53:46.000000 bisos.b-0.41/panels/bisos.b.b_io/bleePanelProc.sh
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)     5588 2024-01-17 19:53:43.000000 bisos.b-0.41/panels/bisos.b.b_io/ftoProc.sh
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-15 00:39:37.665351 bisos.b-0.41/panels/bisos.b.cs/
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-15 00:39:37.665351 bisos.b-0.41/panels/bisos.b.cs/_nodeBase_/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       18 2024-01-10 00:22:33.000000 bisos.b-0.41/panels/bisos.b.cs/_nodeBase_/_objectType_
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       11 2024-01-10 00:22:33.000000 bisos.b-0.41/panels/bisos.b.cs/_nodeBase_/_treeProc_
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        5 2024-01-10 00:22:33.000000 bisos.b-0.41/panels/bisos.b.cs/_nodeBase_/_tree_
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)     2307 2024-01-17 19:54:06.000000 bisos.b-0.41/panels/bisos.b.cs/_nodeBase_/bleePanelProc.sh
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        0 2024-01-10 00:22:33.000000 bisos.b-0.41/panels/bisos.b.cs/_nodeBase_/destDesc
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        0 2024-01-10 00:22:33.000000 bisos.b-0.41/panels/bisos.b.cs/_nodeBase_/foldDesc
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)     5586 2024-01-17 19:54:03.000000 bisos.b-0.41/panels/bisos.b.cs/_nodeBase_/ftoProc.sh
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    22182 2024-02-10 05:43:04.000000 bisos.b-0.41/panels/bisos.b.cs/_nodeBase_/fullUsagePanel-en.org
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       18 2024-01-10 00:22:33.000000 bisos.b-0.41/panels/bisos.b.cs/_objectType_
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       17 2024-01-10 00:22:33.000000 bisos.b-0.41/panels/bisos.b.cs/_treeProc_
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        5 2024-01-10 00:22:33.000000 bisos.b-0.41/panels/bisos.b.cs/_tree_
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)     2296 2024-01-17 19:53:59.000000 bisos.b-0.41/panels/bisos.b.cs/bleePanelProc.sh
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)     5586 2024-01-17 19:53:56.000000 bisos.b-0.41/panels/bisos.b.cs/ftoProc.sh
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)     2285 2024-01-17 19:53:41.000000 bisos.b-0.41/panels/bleePanelProc.sh
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-15 00:39:37.669351 bisos.b-0.41/panels/evolution/
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-15 00:39:37.669351 bisos.b-0.41/panels/evolution/_nodeBase_/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       18 2024-01-21 05:01:19.000000 bisos.b-0.41/panels/evolution/_nodeBase_/_objectType_
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       11 2024-01-21 05:01:14.000000 bisos.b-0.41/panels/evolution/_nodeBase_/_treeProc_
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        5 2024-01-21 05:01:14.000000 bisos.b-0.41/panels/evolution/_nodeBase_/_tree_
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)     2317 2024-01-21 20:05:57.000000 bisos.b-0.41/panels/evolution/_nodeBase_/bleePanelProc.sh
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        0 2024-01-21 05:01:25.000000 bisos.b-0.41/panels/evolution/_nodeBase_/destDesc
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        0 2024-01-21 05:01:25.000000 bisos.b-0.41/panels/evolution/_nodeBase_/foldDesc
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)     5596 2024-01-21 20:05:55.000000 bisos.b-0.41/panels/evolution/_nodeBase_/ftoProc.sh
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    10839 2024-01-21 20:05:55.000000 bisos.b-0.41/panels/evolution/_nodeBase_/fullUsagePanel-en.org
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       18 2024-01-21 05:01:14.000000 bisos.b-0.41/panels/evolution/_objectType_
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       17 2024-01-21 05:01:19.000000 bisos.b-0.41/panels/evolution/_treeProc_
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        5 2024-01-21 05:01:10.000000 bisos.b-0.41/panels/evolution/_tree_
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)     2306 2024-01-21 20:05:53.000000 bisos.b-0.41/panels/evolution/bleePanelProc.sh
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)     5596 2024-01-21 20:05:51.000000 bisos.b-0.41/panels/evolution/ftoProc.sh
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-15 00:39:37.669351 bisos.b-0.41/panels/fileParameters/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       18 2024-01-10 00:22:55.000000 bisos.b-0.41/panels/fileParameters/_objectType_
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       17 2024-01-10 00:22:55.000000 bisos.b-0.41/panels/fileParameters/_treeProc_
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        5 2024-01-10 00:22:55.000000 bisos.b-0.41/panels/fileParameters/_tree_
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)     1953 2024-01-10 00:22:55.000000 bisos.b-0.41/panels/fileParameters/bleePanelProc.sh
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        0 2024-01-10 00:22:55.000000 bisos.b-0.41/panels/fileParameters/destDesc
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        0 2024-01-10 00:22:55.000000 bisos.b-0.41/panels/fileParameters/foldDesc
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)     4972 2024-01-10 00:22:55.000000 bisos.b-0.41/panels/fileParameters/ftoProc.sh
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     9984 2024-01-27 05:14:25.000000 bisos.b-0.41/panels/fileParameters/fullUsagePanel-en.org
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-15 00:39:37.673351 bisos.b-0.41/panels/fileTreeObject-FTO/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       18 2024-01-10 00:22:55.000000 bisos.b-0.41/panels/fileTreeObject-FTO/_objectType_
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       17 2024-01-10 00:22:55.000000 bisos.b-0.41/panels/fileTreeObject-FTO/_treeProc_
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        5 2024-01-10 00:22:55.000000 bisos.b-0.41/panels/fileTreeObject-FTO/_tree_
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)     1957 2024-01-10 00:22:55.000000 bisos.b-0.41/panels/fileTreeObject-FTO/bleePanelProc.sh
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        0 2024-01-10 00:22:55.000000 bisos.b-0.41/panels/fileTreeObject-FTO/destDesc
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        0 2024-01-10 00:22:55.000000 bisos.b-0.41/panels/fileTreeObject-FTO/foldDesc
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)     4976 2024-01-10 00:22:55.000000 bisos.b-0.41/panels/fileTreeObject-FTO/ftoProc.sh
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    10584 2024-01-10 00:22:55.000000 bisos.b-0.41/panels/fileTreeObject-FTO/fullUsagePanel-en.org
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-15 00:39:37.673351 bisos.b-0.41/panels/fileVariables/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       18 2024-01-10 00:22:55.000000 bisos.b-0.41/panels/fileVariables/_objectType_
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       17 2024-01-10 00:22:55.000000 bisos.b-0.41/panels/fileVariables/_treeProc_
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        5 2024-01-10 00:22:55.000000 bisos.b-0.41/panels/fileVariables/_tree_
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)     1952 2024-01-10 00:22:55.000000 bisos.b-0.41/panels/fileVariables/bleePanelProc.sh
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        0 2024-01-10 00:22:55.000000 bisos.b-0.41/panels/fileVariables/destDesc
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        0 2024-01-10 00:22:55.000000 bisos.b-0.41/panels/fileVariables/foldDesc
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)     4971 2024-01-10 00:22:55.000000 bisos.b-0.41/panels/fileVariables/ftoProc.sh
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    10524 2024-01-10 00:22:55.000000 bisos.b-0.41/panels/fileVariables/fullUsagePanel-en.org
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)     5647 2024-01-17 19:53:38.000000 bisos.b-0.41/panels/ftoProc.sh
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       38 2024-05-15 00:39:37.673351 bisos.b-0.41/setup.cfg
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)     2029 2024-05-14 23:30:20.000000 bisos.b-0.41/setup.py
```

### Comparing `bisos.b-0.4/bisos/b/__init__.py` & `bisos.b-0.41/bisos/b/__init__.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/ast.py` & `bisos.b-0.41/bisos/b/ast.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/b_io/__init__.py` & `bisos.b-0.41/bisos/b/b_io/__init__.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/b_io/ann.py` & `bisos.b-0.41/bisos/b/b_io/ann.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/b_io/eh.py` & `bisos.b-0.41/bisos/b/b_io/eh.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/b_io/io.py` & `bisos.b-0.41/bisos/b/b_io/io.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/b_io/k1-eh.py` & `bisos.b-0.41/bisos/b/b_io/k1-eh.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/b_io/log.py` & `bisos.b-0.41/bisos/b/b_io/log.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/b_io/out.py` & `bisos.b-0.41/bisos/b/b_io/out.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/b_io/stderr.py` & `bisos.b-0.41/bisos/b/b_io/stderr.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/b_io/stdin.py` & `bisos.b-0.41/bisos/b/b_io/stdin.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/b_io/stdout.py` & `bisos.b-0.41/bisos/b/b_io/stdout.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/b_io/tm.py` & `bisos.b-0.41/bisos/b/b_io/tm.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/clsMethod_csu.py` & `bisos.b-0.41/bisos/b/clsMethod_csu.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/comment.py` & `bisos.b-0.41/bisos/b/comment.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/cs/__init__.py` & `bisos.b-0.41/bisos/b/cs/__init__.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/cs/arg.py` & `bisos.b-0.41/bisos/b/cs/arg.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/cs/cs.py` & `bisos.b-0.41/bisos/b/cs/cs.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/cs/examples.py` & `bisos.b-0.41/bisos/b/cs/examples.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/cs/globalContext.py` & `bisos.b-0.41/bisos/b/cs/globalContext.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/cs/inCmnd.py` & `bisos.b-0.41/bisos/b/cs/inCmnd.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/cs/k1-ro.py` & `bisos.b-0.41/bisos/b/cs/k1-ro.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/cs/main.py` & `bisos.b-0.41/bisos/b/cs/main.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/cs/param.py` & `bisos.b-0.41/bisos/b/cs/param.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/cs/ro.py` & `bisos.b-0.41/bisos/b/cs/ro.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/cs/rpyc.py` & `bisos.b-0.41/bisos/b/cs/rpyc.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/cs/rtInvoker.py` & `bisos.b-0.41/bisos/b/cs/rtInvoker.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/cs/runArgs.py` & `bisos.b-0.41/bisos/b/cs/runArgs.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/cs/track.py` & `bisos.b-0.41/bisos/b/cs/track.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/dir.py` & `bisos.b-0.41/bisos/b/dir.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/exception.py` & `bisos.b-0.41/bisos/b/exception.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/fp.py` & `bisos.b-0.41/bisos/b/fp.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/fpCls.py` & `bisos.b-0.41/bisos/b/fpCls.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/fpath.py` & `bisos.b-0.41/bisos/b/fpath.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/fto.py` & `bisos.b-0.41/bisos/b/fto.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/fv.py` & `bisos.b-0.41/bisos/b/fv.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/importFile.py` & `bisos.b-0.41/bisos/b/importFile.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/niche.py` & `bisos.b-0.41/bisos/b/niche.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/op.py` & `bisos.b-0.41/bisos/b/op.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/pyRunAs.py` & `bisos.b-0.41/bisos/b/pyRunAs.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/subProc.py` & `bisos.b-0.41/bisos/b/subProc.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/bisos/b/types.py` & `bisos.b-0.41/bisos/b/types.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.4/lh-agpl3-LICENSE.txt` & `bisos.b-0.41/lh-agpl3-LICENSE.txt`

 * *Files identical despite different names*

