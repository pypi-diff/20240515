# Comparing `tmp/zope.interface-6.2.tar.gz` & `tmp/zope.interface-6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zope.interface-6.2.tar", last modified: Fri Feb 16 07:42:53 2024, max compression
+gzip compressed data, was "zope.interface-6.3.tar", last modified: Fri Apr 12 15:13:37 2024, max compression
```

## Comparing `zope.interface-6.2.tar` & `zope.interface-6.3.tar`

### file list

```diff
@@ -1,110 +1,134 @@
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-16 07:42:53.332718 zope.interface-6.2/
--rw-r--r--   0 m.howitz   (502) staff       (20)      588 2024-02-16 07:42:52.000000 zope.interface-6.2/.coveragerc
--rwxr-xr-x   0 m.howitz   (502) staff       (20)     2259 2024-02-16 07:42:52.000000 zope.interface-6.2/.manylinux-install.sh
--rwxr-xr-x   0 m.howitz   (502) staff       (20)      509 2024-02-16 07:42:52.000000 zope.interface-6.2/.manylinux.sh
--rw-r--r--   0 m.howitz   (502) staff       (20)      664 2024-02-16 07:42:52.000000 zope.interface-6.2/.readthedocs.yaml
--rw-r--r--   0 m.howitz   (502) staff       (20)    38873 2024-02-16 07:42:52.000000 zope.interface-6.2/CHANGES.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      799 2024-02-16 07:42:52.000000 zope.interface-6.2/CONTRIBUTING.md
--rw-r--r--   0 m.howitz   (502) staff       (20)       32 2024-02-16 07:42:52.000000 zope.interface-6.2/COPYRIGHT.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2024-02-16 07:42:52.000000 zope.interface-6.2/LICENSE.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)      579 2024-02-16 07:42:52.000000 zope.interface-6.2/MANIFEST.in
--rw-r--r--   0 m.howitz   (502) staff       (20)    41923 2024-02-16 07:42:53.332606 zope.interface-6.2/PKG-INFO
--rw-r--r--   0 m.howitz   (502) staff       (20)     1353 2024-02-16 07:42:52.000000 zope.interface-6.2/README.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     1971 2024-02-16 07:42:52.000000 zope.interface-6.2/appveyor.yml
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-16 07:42:53.317380 zope.interface-6.2/benchmarks/
--rw-r--r--   0 m.howitz   (502) staff       (20)     8497 2024-02-16 07:42:52.000000 zope.interface-6.2/benchmarks/micro.py
--rw-r--r--   0 m.howitz   (502) staff       (20)      838 2024-02-16 07:42:52.000000 zope.interface-6.2/build.cmd
--rw-r--r--   0 m.howitz   (502) staff       (20)      215 2024-02-16 07:42:52.000000 zope.interface-6.2/buildout.cfg
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-16 07:42:53.320127 zope.interface-6.2/docs/
--rw-r--r--   0 m.howitz   (502) staff       (20)     5592 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/Makefile
--rw-r--r--   0 m.howitz   (502) staff       (20)    41051 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/README.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)    33998 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/README.ru.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)    18817 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/adapter.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)    21169 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/adapter.ru.rst
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-16 07:42:53.321381 zope.interface-6.2/docs/api/
--rw-r--r--   0 m.howitz   (502) staff       (20)      691 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/api/adapters.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     1283 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/api/common.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     2465 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/api/components.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)    21746 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/api/declarations.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      165 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/api/index.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      687 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/api/ro.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     9948 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/api/specifications.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       28 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/changes.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     9130 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/conf.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1742 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/foodforthought.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     9509 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/hacking.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     6537 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/human.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)    10681 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/human.ru.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      639 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/index.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     5110 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/make.bat
--rw-r--r--   0 m.howitz   (502) staff       (20)       68 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/requirements.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)    10222 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/verify.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      599 2024-02-16 07:42:53.332985 zope.interface-6.2/setup.cfg
--rw-r--r--   0 m.howitz   (502) staff       (20)     5014 2024-02-16 07:42:52.000000 zope.interface-6.2/setup.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-16 07:42:53.314466 zope.interface-6.2/src/
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-16 07:42:53.321572 zope.interface-6.2/src/zope/
--rw-r--r--   0 m.howitz   (502) staff       (20)       56 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/__init__.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-16 07:42:53.325064 zope.interface-6.2/src/zope/interface/
--rw-r--r--   0 m.howitz   (502) staff       (20)     3460 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/__init__.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     4369 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/_compat.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1057 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/_flatten.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    57205 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/_zope_interface_coptimizations.c
--rw-r--r--   0 m.howitz   (502) staff       (20)    36218 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/adapter.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     3892 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/advice.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-16 07:42:53.326789 zope.interface-6.2/src/zope/interface/common/
--rw-r--r--   0 m.howitz   (502) staff       (20)    10462 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/common/__init__.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     3027 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/common/builtins.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     6792 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/common/collections.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    20964 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/common/idatetime.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     5368 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/common/interfaces.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1242 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/common/io.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     4678 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/common/mapping.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1682 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/common/numbers.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     5526 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/common/sequence.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-16 07:42:53.328035 zope.interface-6.2/src/zope/interface/common/tests/
--rw-r--r--   0 m.howitz   (502) staff       (20)     5309 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/common/tests/__init__.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     3907 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/common/tests/basemapping.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1345 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/common/tests/test_builtins.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     5718 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/common/tests/test_collections.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1923 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/common/tests/test_idatetime.py
--rw-r--r--   0 m.howitz   (502) staff       (20)      813 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/common/tests/test_import_interfaces.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1597 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/common/tests/test_io.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1394 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/common/tests/test_numbers.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    43007 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/declarations.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     4068 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/document.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     8636 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/exceptions.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    39099 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/interface.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    50126 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/interfaces.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    25829 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/registry.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    24157 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/ro.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-16 07:42:53.331680 zope.interface-6.2/src/zope/interface/tests/
--rw-r--r--   0 m.howitz   (502) staff       (20)     3961 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/__init__.py
--rw-r--r--   0 m.howitz   (502) staff       (20)      898 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/advisory_testing.py
--rw-r--r--   0 m.howitz   (502) staff       (20)      912 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/dummy.py
--rw-r--r--   0 m.howitz   (502) staff       (20)      890 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/idummy.py
--rw-r--r--   0 m.howitz   (502) staff       (20)      839 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/m1.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     3015 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/odd.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    79479 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/test_adapter.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     5962 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/test_advice.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1290 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/test_compile_flags.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    82140 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/test_declarations.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    17164 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/test_document.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1120 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/test_element.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     6412 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/test_exceptions.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    92312 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/test_interface.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     4377 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/test_interfaces.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     7566 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/test_odd_declarations.py
--rw-r--r--   0 m.howitz   (502) staff       (20)   112910 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/test_registry.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    14124 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/test_ro.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1934 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/test_sorting.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    19191 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/test_verify.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     7226 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/verify.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-16 07:42:53.331923 zope.interface-6.2/src/zope.interface.egg-info/
--rw-r--r--   0 m.howitz   (502) staff       (20)    41923 2024-02-16 07:42:53.000000 zope.interface-6.2/src/zope.interface.egg-info/PKG-INFO
--rw-r--r--   0 m.howitz   (502) staff       (20)     2953 2024-02-16 07:42:53.000000 zope.interface-6.2/src/zope.interface.egg-info/SOURCES.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        1 2024-02-16 07:42:53.000000 zope.interface-6.2/src/zope.interface.egg-info/dependency_links.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        5 2024-02-16 07:42:53.000000 zope.interface-6.2/src/zope.interface.egg-info/namespace_packages.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        1 2024-02-16 07:42:53.000000 zope.interface-6.2/src/zope.interface.egg-info/not-zip-safe
--rw-r--r--   0 m.howitz   (502) staff       (20)      170 2024-02-16 07:42:53.000000 zope.interface-6.2/src/zope.interface.egg-info/requires.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        5 2024-02-16 07:42:53.000000 zope.interface-6.2/src/zope.interface.egg-info/top_level.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)     2045 2024-02-16 07:42:52.000000 zope.interface-6.2/tox.ini
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:13:37.232517 zope.interface-6.3/
+-rw-r--r--   0 jens       (501) staff       (20)      588 2024-04-12 14:44:49.000000 zope.interface-6.3/.coveragerc
+-rwxr-xr-x   0 jens       (501) staff       (20)     2259 2024-04-12 14:44:49.000000 zope.interface-6.3/.manylinux-install.sh
+-rwxr-xr-x   0 jens       (501) staff       (20)      509 2024-04-12 14:44:49.000000 zope.interface-6.3/.manylinux.sh
+-rw-r--r--   0 jens       (501) staff       (20)      664 2024-04-12 14:44:49.000000 zope.interface-6.3/.readthedocs.yaml
+-rw-r--r--   0 jens       (501) staff       (20)    38966 2024-04-12 14:52:40.000000 zope.interface-6.3/CHANGES.rst
+-rw-r--r--   0 jens       (501) staff       (20)      799 2024-04-12 14:44:49.000000 zope.interface-6.3/CONTRIBUTING.md
+-rw-r--r--   0 jens       (501) staff       (20)       32 2023-01-03 12:44:50.000000 zope.interface-6.3/COPYRIGHT.txt
+-rw-r--r--   0 jens       (501) staff       (20)     2070 2023-01-03 12:44:50.000000 zope.interface-6.3/LICENSE.txt
+-rw-r--r--   0 jens       (501) staff       (20)      579 2024-04-12 14:51:36.000000 zope.interface-6.3/MANIFEST.in
+-rw-r--r--   0 jens       (501) staff       (20)    42016 2024-04-12 15:13:37.232439 zope.interface-6.3/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)     1353 2023-01-03 12:44:50.000000 zope.interface-6.3/README.rst
+-rw-r--r--   0 jens       (501) staff       (20)     1971 2024-04-12 14:51:59.000000 zope.interface-6.3/appveyor.yml
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:13:37.220392 zope.interface-6.3/benchmarks/
+-rw-r--r--   0 jens       (501) staff       (20)     8497 2023-01-03 12:44:50.000000 zope.interface-6.3/benchmarks/micro.py
+-rw-r--r--   0 jens       (501) staff       (20)      838 2023-01-03 12:44:50.000000 zope.interface-6.3/build.cmd
+-rw-r--r--   0 jens       (501) staff       (20)      215 2023-01-03 12:44:50.000000 zope.interface-6.3/buildout.cfg
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:13:37.222163 zope.interface-6.3/docs/
+-rw-r--r--   0 jens       (501) staff       (20)     5592 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/Makefile
+-rw-r--r--   0 jens       (501) staff       (20)    41051 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/README.rst
+-rw-r--r--   0 jens       (501) staff       (20)    33998 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/README.ru.rst
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:13:37.218221 zope.interface-6.3/docs/_build/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:13:37.222253 zope.interface-6.3/docs/_build/doctest/
+-rw-r--r--   0 jens       (501) staff       (20)     1292 2024-04-12 14:47:42.000000 zope.interface-6.3/docs/_build/doctest/output.txt
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:13:37.218262 zope.interface-6.3/docs/_build/html/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:13:37.223447 zope.interface-6.3/docs/_build/html/_sources/
+-rw-r--r--   0 jens       (501) staff       (20)    41051 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/_build/html/_sources/README.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)    33998 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/_build/html/_sources/README.ru.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)    18817 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/_build/html/_sources/adapter.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)    21169 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/_build/html/_sources/adapter.ru.rst.txt
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:13:37.224182 zope.interface-6.3/docs/_build/html/_sources/api/
+-rw-r--r--   0 jens       (501) staff       (20)      691 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/_build/html/_sources/api/adapters.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     1283 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/_build/html/_sources/api/common.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     2465 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/_build/html/_sources/api/components.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)    21746 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/_build/html/_sources/api/declarations.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)      165 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/_build/html/_sources/api/index.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)      687 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/_build/html/_sources/api/ro.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     9948 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/_build/html/_sources/api/specifications.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)       28 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/_build/html/_sources/changes.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     1742 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/_build/html/_sources/foodforthought.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     9509 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/_build/html/_sources/hacking.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     6537 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/_build/html/_sources/human.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)    10681 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/_build/html/_sources/human.ru.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)      639 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)    10222 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/_build/html/_sources/verify.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)    18817 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/adapter.rst
+-rw-r--r--   0 jens       (501) staff       (20)    21169 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/adapter.ru.rst
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:13:37.224931 zope.interface-6.3/docs/api/
+-rw-r--r--   0 jens       (501) staff       (20)      691 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/api/adapters.rst
+-rw-r--r--   0 jens       (501) staff       (20)     1283 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/api/common.rst
+-rw-r--r--   0 jens       (501) staff       (20)     2465 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/api/components.rst
+-rw-r--r--   0 jens       (501) staff       (20)    21746 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/api/declarations.rst
+-rw-r--r--   0 jens       (501) staff       (20)      165 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/api/index.rst
+-rw-r--r--   0 jens       (501) staff       (20)      687 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/api/ro.rst
+-rw-r--r--   0 jens       (501) staff       (20)     9948 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/api/specifications.rst
+-rw-r--r--   0 jens       (501) staff       (20)       28 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/changes.rst
+-rw-r--r--   0 jens       (501) staff       (20)     9130 2024-04-12 14:41:20.000000 zope.interface-6.3/docs/conf.py
+-rw-r--r--   0 jens       (501) staff       (20)     1742 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/foodforthought.rst
+-rw-r--r--   0 jens       (501) staff       (20)     9509 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/hacking.rst
+-rw-r--r--   0 jens       (501) staff       (20)     6537 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/human.rst
+-rw-r--r--   0 jens       (501) staff       (20)    10681 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/human.ru.rst
+-rw-r--r--   0 jens       (501) staff       (20)      639 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/index.rst
+-rw-r--r--   0 jens       (501) staff       (20)     5110 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/make.bat
+-rw-r--r--   0 jens       (501) staff       (20)       68 2023-10-05 10:12:16.000000 zope.interface-6.3/docs/requirements.txt
+-rw-r--r--   0 jens       (501) staff       (20)    10222 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/verify.rst
+-rw-r--r--   0 jens       (501) staff       (20)      599 2024-04-12 15:13:37.233159 zope.interface-6.3/setup.cfg
+-rw-r--r--   0 jens       (501) staff       (20)     5014 2024-04-12 14:52:58.000000 zope.interface-6.3/setup.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:13:37.218506 zope.interface-6.3/src/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:13:37.225032 zope.interface-6.3/src/zope/
+-rw-r--r--   0 jens       (501) staff       (20)       56 2023-01-03 12:44:50.000000 zope.interface-6.3/src/zope/__init__.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:13:37.227583 zope.interface-6.3/src/zope/interface/
+-rw-r--r--   0 jens       (501) staff       (20)     3460 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)     4369 2023-01-03 12:44:50.000000 zope.interface-6.3/src/zope/interface/_compat.py
+-rw-r--r--   0 jens       (501) staff       (20)     1057 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/_flatten.py
+-rw-r--r--   0 jens       (501) staff       (20)    57205 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/_zope_interface_coptimizations.c
+-rw-r--r--   0 jens       (501) staff       (20)    36218 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/adapter.py
+-rw-r--r--   0 jens       (501) staff       (20)     3892 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/advice.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:13:37.228631 zope.interface-6.3/src/zope/interface/common/
+-rw-r--r--   0 jens       (501) staff       (20)    10462 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/common/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)     3027 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/common/builtins.py
+-rw-r--r--   0 jens       (501) staff       (20)     6792 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/common/collections.py
+-rw-r--r--   0 jens       (501) staff       (20)    20964 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/common/idatetime.py
+-rw-r--r--   0 jens       (501) staff       (20)     5368 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/common/interfaces.py
+-rw-r--r--   0 jens       (501) staff       (20)     1242 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/common/io.py
+-rw-r--r--   0 jens       (501) staff       (20)     4678 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/common/mapping.py
+-rw-r--r--   0 jens       (501) staff       (20)     1682 2023-01-03 12:44:50.000000 zope.interface-6.3/src/zope/interface/common/numbers.py
+-rw-r--r--   0 jens       (501) staff       (20)     5526 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/common/sequence.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:13:37.229436 zope.interface-6.3/src/zope/interface/common/tests/
+-rw-r--r--   0 jens       (501) staff       (20)     5309 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/common/tests/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)     3907 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/common/tests/basemapping.py
+-rw-r--r--   0 jens       (501) staff       (20)     1345 2023-01-03 12:44:50.000000 zope.interface-6.3/src/zope/interface/common/tests/test_builtins.py
+-rw-r--r--   0 jens       (501) staff       (20)     5718 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/common/tests/test_collections.py
+-rw-r--r--   0 jens       (501) staff       (20)     1923 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/common/tests/test_idatetime.py
+-rw-r--r--   0 jens       (501) staff       (20)      813 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/common/tests/test_import_interfaces.py
+-rw-r--r--   0 jens       (501) staff       (20)     1597 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/common/tests/test_io.py
+-rw-r--r--   0 jens       (501) staff       (20)     1394 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/common/tests/test_numbers.py
+-rw-r--r--   0 jens       (501) staff       (20)    43007 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/declarations.py
+-rw-r--r--   0 jens       (501) staff       (20)     4068 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/document.py
+-rw-r--r--   0 jens       (501) staff       (20)     8636 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/exceptions.py
+-rw-r--r--   0 jens       (501) staff       (20)    39260 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/interface.py
+-rw-r--r--   0 jens       (501) staff       (20)    50126 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/interfaces.py
+-rw-r--r--   0 jens       (501) staff       (20)    25829 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/registry.py
+-rw-r--r--   0 jens       (501) staff       (20)    24157 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/ro.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:13:37.231755 zope.interface-6.3/src/zope/interface/tests/
+-rw-r--r--   0 jens       (501) staff       (20)     3961 2023-01-03 12:44:50.000000 zope.interface-6.3/src/zope/interface/tests/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)      898 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/tests/advisory_testing.py
+-rw-r--r--   0 jens       (501) staff       (20)      912 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/tests/dummy.py
+-rw-r--r--   0 jens       (501) staff       (20)      890 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/tests/idummy.py
+-rw-r--r--   0 jens       (501) staff       (20)      839 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/tests/m1.py
+-rw-r--r--   0 jens       (501) staff       (20)     3015 2023-01-03 12:44:50.000000 zope.interface-6.3/src/zope/interface/tests/odd.py
+-rw-r--r--   0 jens       (501) staff       (20)    79479 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/tests/test_adapter.py
+-rw-r--r--   0 jens       (501) staff       (20)     5962 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/tests/test_advice.py
+-rw-r--r--   0 jens       (501) staff       (20)     1290 2023-01-03 12:44:50.000000 zope.interface-6.3/src/zope/interface/tests/test_compile_flags.py
+-rw-r--r--   0 jens       (501) staff       (20)    82140 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/tests/test_declarations.py
+-rw-r--r--   0 jens       (501) staff       (20)    17164 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/tests/test_document.py
+-rw-r--r--   0 jens       (501) staff       (20)     1120 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/tests/test_element.py
+-rw-r--r--   0 jens       (501) staff       (20)     6412 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/tests/test_exceptions.py
+-rw-r--r--   0 jens       (501) staff       (20)    92312 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/tests/test_interface.py
+-rw-r--r--   0 jens       (501) staff       (20)     4377 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/tests/test_interfaces.py
+-rw-r--r--   0 jens       (501) staff       (20)     7566 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/tests/test_odd_declarations.py
+-rw-r--r--   0 jens       (501) staff       (20)   112910 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/tests/test_registry.py
+-rw-r--r--   0 jens       (501) staff       (20)    14124 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/tests/test_ro.py
+-rw-r--r--   0 jens       (501) staff       (20)     1934 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/tests/test_sorting.py
+-rw-r--r--   0 jens       (501) staff       (20)    19191 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/tests/test_verify.py
+-rw-r--r--   0 jens       (501) staff       (20)     7226 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/verify.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:13:37.231920 zope.interface-6.3/src/zope.interface.egg-info/
+-rw-r--r--   0 jens       (501) staff       (20)    42016 2024-04-12 15:13:37.000000 zope.interface-6.3/src/zope.interface.egg-info/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)     3783 2024-04-12 15:13:37.000000 zope.interface-6.3/src/zope.interface.egg-info/SOURCES.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2024-04-12 15:13:37.000000 zope.interface-6.3/src/zope.interface.egg-info/dependency_links.txt
+-rw-r--r--   0 jens       (501) staff       (20)        5 2024-04-12 15:13:37.000000 zope.interface-6.3/src/zope.interface.egg-info/namespace_packages.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2023-01-03 13:57:16.000000 zope.interface-6.3/src/zope.interface.egg-info/not-zip-safe
+-rw-r--r--   0 jens       (501) staff       (20)      170 2024-04-12 15:13:37.000000 zope.interface-6.3/src/zope.interface.egg-info/requires.txt
+-rw-r--r--   0 jens       (501) staff       (20)        5 2024-04-12 15:13:37.000000 zope.interface-6.3/src/zope.interface.egg-info/top_level.txt
+-rw-r--r--   0 jens       (501) staff       (20)     2045 2024-04-12 14:51:36.000000 zope.interface-6.3/tox.ini
```

### Comparing `zope.interface-6.2/.coveragerc` & `zope.interface-6.3/.coveragerc`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/.manylinux-install.sh` & `zope.interface-6.3/.manylinux-install.sh`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/.readthedocs.yaml` & `zope.interface-6.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/CHANGES.rst` & `zope.interface-6.3/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 =========
  Changes
 =========
 
+6.3 (2024-04-12)
+================
+
+- Add preliminary support for Python 3.13 as of 3.13a6.
+
+
 6.2 (2024-02-16)
 ================
 
 - Add preliminary support for Python 3.13 as of 3.13a3.
 
 - Add support to use the pipe (``|``) syntax for ``typing.Union``.
   (`#280 <https://github.com/zopefoundation/zope.interface/issues/280>`_)
```

### Comparing `zope.interface-6.2/CONTRIBUTING.md` & `zope.interface-6.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/LICENSE.txt` & `zope.interface-6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/MANIFEST.in` & `zope.interface-6.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/PKG-INFO` & `zope.interface-6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zope.interface
-Version: 6.2
+Version: 6.3
 Summary: Interfaces for Python
 Home-page: https://github.com/zopefoundation/zope.interface
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Keywords: interface,components,plugins
 Classifier: Development Status :: 5 - Production/Stable
@@ -71,14 +71,20 @@
 
 For detailed documentation, please see https://zopeinterface.readthedocs.io/en/latest/
 
 =========
  Changes
 =========
 
+6.3 (2024-04-12)
+================
+
+- Add preliminary support for Python 3.13 as of 3.13a6.
+
+
 6.2 (2024-02-16)
 ================
 
 - Add preliminary support for Python 3.13 as of 3.13a3.
 
 - Add support to use the pipe (``|``) syntax for ``typing.Union``.
   (`#280 <https://github.com/zopefoundation/zope.interface/issues/280>`_)
```

### Comparing `zope.interface-6.2/README.rst` & `zope.interface-6.3/README.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/appveyor.yml` & `zope.interface-6.3/appveyor.yml`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/benchmarks/micro.py` & `zope.interface-6.3/benchmarks/micro.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/build.cmd` & `zope.interface-6.3/build.cmd`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/docs/Makefile` & `zope.interface-6.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/docs/README.rst` & `zope.interface-6.3/docs/README.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/docs/README.ru.rst` & `zope.interface-6.3/docs/README.ru.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/docs/adapter.rst` & `zope.interface-6.3/docs/_build/html/_sources/adapter.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/docs/adapter.ru.rst` & `zope.interface-6.3/docs/_build/html/_sources/adapter.ru.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/docs/api/adapters.rst` & `zope.interface-6.3/docs/_build/html/_sources/api/adapters.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/docs/api/common.rst` & `zope.interface-6.3/docs/_build/html/_sources/api/common.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/docs/api/components.rst` & `zope.interface-6.3/docs/_build/html/_sources/api/components.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/docs/api/declarations.rst` & `zope.interface-6.3/docs/_build/html/_sources/api/declarations.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/docs/api/ro.rst` & `zope.interface-6.3/docs/_build/html/_sources/api/ro.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/docs/api/specifications.rst` & `zope.interface-6.3/docs/_build/html/_sources/api/specifications.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/docs/conf.py` & `zope.interface-6.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/docs/foodforthought.rst` & `zope.interface-6.3/docs/_build/html/_sources/foodforthought.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/docs/hacking.rst` & `zope.interface-6.3/docs/_build/html/_sources/hacking.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/docs/human.rst` & `zope.interface-6.3/docs/_build/html/_sources/human.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/docs/human.ru.rst` & `zope.interface-6.3/docs/_build/html/_sources/human.ru.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/docs/index.rst` & `zope.interface-6.3/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/docs/make.bat` & `zope.interface-6.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/docs/verify.rst` & `zope.interface-6.3/docs/_build/html/_sources/verify.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/setup.cfg` & `zope.interface-6.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/setup.py` & `zope.interface-6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 long_description = (
         read('README.rst')
         + '\n' +
         read('CHANGES.rst')
         )
 
 setup(name='zope.interface',
-      version='6.2',
+      version='6.3',
       url='https://github.com/zopefoundation/zope.interface',
       license='ZPL 2.1',
       description='Interfaces for Python',
       author='Zope Foundation and Contributors',
       author_email='zope-dev@zope.org',
       long_description=long_description,
       classifiers=[
```

### Comparing `zope.interface-6.2/src/zope/interface/__init__.py` & `zope.interface-6.3/src/zope/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/_compat.py` & `zope.interface-6.3/src/zope/interface/_compat.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/_flatten.py` & `zope.interface-6.3/src/zope/interface/_flatten.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/_zope_interface_coptimizations.c` & `zope.interface-6.3/src/zope/interface/_zope_interface_coptimizations.c`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/adapter.py` & `zope.interface-6.3/src/zope/interface/adapter.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/advice.py` & `zope.interface-6.3/src/zope/interface/advice.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/common/__init__.py` & `zope.interface-6.3/src/zope/interface/common/__init__.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/common/builtins.py` & `zope.interface-6.3/src/zope/interface/common/builtins.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/common/collections.py` & `zope.interface-6.3/src/zope/interface/common/collections.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/common/idatetime.py` & `zope.interface-6.3/src/zope/interface/common/idatetime.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/common/interfaces.py` & `zope.interface-6.3/src/zope/interface/common/interfaces.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/common/io.py` & `zope.interface-6.3/src/zope/interface/common/io.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/common/mapping.py` & `zope.interface-6.3/src/zope/interface/common/mapping.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/common/numbers.py` & `zope.interface-6.3/src/zope/interface/common/numbers.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/common/sequence.py` & `zope.interface-6.3/src/zope/interface/common/sequence.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/common/tests/__init__.py` & `zope.interface-6.3/src/zope/interface/common/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/common/tests/basemapping.py` & `zope.interface-6.3/src/zope/interface/common/tests/basemapping.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/common/tests/test_builtins.py` & `zope.interface-6.3/src/zope/interface/common/tests/test_builtins.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/common/tests/test_collections.py` & `zope.interface-6.3/src/zope/interface/common/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/common/tests/test_idatetime.py` & `zope.interface-6.3/src/zope/interface/common/tests/test_idatetime.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/common/tests/test_import_interfaces.py` & `zope.interface-6.3/src/zope/interface/common/tests/test_import_interfaces.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/common/tests/test_io.py` & `zope.interface-6.3/src/zope/interface/common/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/common/tests/test_numbers.py` & `zope.interface-6.3/src/zope/interface/common/tests/test_numbers.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/declarations.py` & `zope.interface-6.3/src/zope/interface/declarations.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/document.py` & `zope.interface-6.3/src/zope/interface/document.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/exceptions.py` & `zope.interface-6.3/src/zope/interface/exceptions.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/interface.py` & `zope.interface-6.3/src/zope/interface/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -795,14 +795,17 @@
             if aname not in (
                 # __locals__: Python 3 sometimes adds this.
                 '__locals__',
                 # __qualname__: PEP 3155 (Python 3.3+)
                 '__qualname__',
                 # __annotations__: PEP 3107 (Python 3.0+)
                 '__annotations__',
+                # __static_attributes__: Python 3.13a6+
+                # https://github.com/python/cpython/pull/115913
+                '__static_attributes__',
             )
             and aval is not _decorator_non_return
         }
 
     def interfaces(self):
         """Return an iterator for the interfaces in the specification.
         """
```

### Comparing `zope.interface-6.2/src/zope/interface/interfaces.py` & `zope.interface-6.3/src/zope/interface/interfaces.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/registry.py` & `zope.interface-6.3/src/zope/interface/registry.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/ro.py` & `zope.interface-6.3/src/zope/interface/ro.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/tests/__init__.py` & `zope.interface-6.3/src/zope/interface/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/tests/advisory_testing.py` & `zope.interface-6.3/src/zope/interface/tests/advisory_testing.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/tests/dummy.py` & `zope.interface-6.3/src/zope/interface/tests/dummy.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/tests/idummy.py` & `zope.interface-6.3/src/zope/interface/tests/idummy.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/tests/m1.py` & `zope.interface-6.3/src/zope/interface/tests/m1.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/tests/odd.py` & `zope.interface-6.3/src/zope/interface/tests/odd.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/tests/test_adapter.py` & `zope.interface-6.3/src/zope/interface/tests/test_adapter.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/tests/test_advice.py` & `zope.interface-6.3/src/zope/interface/tests/test_advice.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/tests/test_compile_flags.py` & `zope.interface-6.3/src/zope/interface/tests/test_compile_flags.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/tests/test_declarations.py` & `zope.interface-6.3/src/zope/interface/tests/test_declarations.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/tests/test_document.py` & `zope.interface-6.3/src/zope/interface/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/tests/test_element.py` & `zope.interface-6.3/src/zope/interface/tests/test_element.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/tests/test_exceptions.py` & `zope.interface-6.3/src/zope/interface/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/tests/test_interface.py` & `zope.interface-6.3/src/zope/interface/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/tests/test_interfaces.py` & `zope.interface-6.3/src/zope/interface/tests/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/tests/test_odd_declarations.py` & `zope.interface-6.3/src/zope/interface/tests/test_odd_declarations.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/tests/test_registry.py` & `zope.interface-6.3/src/zope/interface/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/tests/test_ro.py` & `zope.interface-6.3/src/zope/interface/tests/test_ro.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/tests/test_sorting.py` & `zope.interface-6.3/src/zope/interface/tests/test_sorting.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/tests/test_verify.py` & `zope.interface-6.3/src/zope/interface/tests/test_verify.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope/interface/verify.py` & `zope.interface-6.3/src/zope/interface/verify.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.2/src/zope.interface.egg-info/PKG-INFO` & `zope.interface-6.3/src/zope.interface.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zope.interface
-Version: 6.2
+Version: 6.3
 Summary: Interfaces for Python
 Home-page: https://github.com/zopefoundation/zope.interface
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Keywords: interface,components,plugins
 Classifier: Development Status :: 5 - Production/Stable
@@ -71,14 +71,20 @@
 
 For detailed documentation, please see https://zopeinterface.readthedocs.io/en/latest/
 
 =========
  Changes
 =========
 
+6.3 (2024-04-12)
+================
+
+- Add preliminary support for Python 3.13 as of 3.13a6.
+
+
 6.2 (2024-02-16)
 ================
 
 - Add preliminary support for Python 3.13 as of 3.13a3.
 
 - Add support to use the pipe (``|``) syntax for ``typing.Union``.
   (`#280 <https://github.com/zopefoundation/zope.interface/issues/280>`_)
```

### Comparing `zope.interface-6.2/tox.ini` & `zope.interface-6.3/tox.ini`

 * *Files identical despite different names*

