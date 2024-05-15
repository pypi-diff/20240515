# Comparing `tmp/sabctools-8.1.0.tar.gz` & `tmp/sabctools-8.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sabctools-8.1.0.tar", last modified: Wed Dec 20 08:41:47 2023, max compression
+gzip compressed data, was "sabctools-8.2.0.tar", last modified: Wed May 15 11:26:49 2024, max compression
```

## Comparing `sabctools-8.1.0.tar` & `sabctools-8.2.0.tar`

### file list

```diff
@@ -1,113 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 08:41:47.854533 sabctools-8.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    17990 2023-12-20 08:17:02.000000 sabctools-8.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-20 08:17:02.000000 sabctools-8.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2023-12-20 08:41:47.854533 sabctools-8.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2023-12-20 08:17:02.000000 sabctools-8.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-12-20 08:17:02.000000 sabctools-8.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 08:41:47.842533 sabctools-8.1.0/sabctools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2023-12-20 08:41:47.000000 sabctools-8.1.0/sabctools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2023-12-20 08:41:47.000000 sabctools-8.1.0/sabctools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-20 08:41:47.000000 sabctools-8.1.0/sabctools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-12-20 08:41:47.000000 sabctools-8.1.0/sabctools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-20 08:41:47.854533 sabctools-8.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    16301 2023-12-20 08:17:02.000000 sabctools-8.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 08:41:47.842533 sabctools-8.1.0/src/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crc32.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crc32.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 08:41:47.846533 sabctools-8.1.0/src/crcutil-1.0/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/INSTALL
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    50573 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/Makefile.am
--rw-r--r--   0 runner    (1001) docker     (127)    56163 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/Makefile.win
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/NEWS
--rw-r--r--   0 runner    (1001) docker     (127)     6669 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/README
--rw-r--r--   0 runner    (1001) docker     (127)    34611 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/aclocal.m4
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/autogen.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 08:41:47.850533 sabctools-8.1.0/src/crcutil-1.0/code/
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/code/base_types.h
--rw-r--r--   0 runner    (1001) docker     (127)    12545 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/code/crc32c_sse4.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7511 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/code/crc32c_sse4.h
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/code/crc32c_sse4_intrin.h
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/code/crc_casts.h
--rw-r--r--   0 runner    (1001) docker     (127)    21506 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/code/generic_crc.h
--rw-r--r--   0 runner    (1001) docker     (127)     8663 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/code/gf_util.h
--rw-r--r--   0 runner    (1001) docker     (127)     8211 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/code/multiword_128_64_gcc_amd64_sse2.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7459 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/code/multiword_64_64_cl_i386_mmx.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8601 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/code/multiword_64_64_gcc_amd64_asm.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7945 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/code/multiword_64_64_gcc_i386_mmx.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7379 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/code/multiword_64_64_intrinsic_i386_mmx.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7264 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/code/platform.h
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/code/protected_crc.h
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/code/rolling_crc.h
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/code/std_headers.h
--rw-r--r--   0 runner    (1001) docker     (127)     8422 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/code/uint128_sse2.h
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/config.h.in
--rw-r--r--   0 runner    (1001) docker     (127)   212367 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/configure
--rw-r--r--   0 runner    (1001) docker     (127)      744 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/configure.ac
--rw-r--r--   0 runner    (1001) docker     (127)    18615 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/depcomp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 08:41:47.850533 sabctools-8.1.0/src/crcutil-1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    10449 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/examples/interface.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8820 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/examples/interface.h
--rw-r--r--   0 runner    (1001) docker     (127)     6390 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/examples/usage.cc
--rw-r--r--   0 runner    (1001) docker     (127)    13663 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/install-sh
--rw-r--r--   0 runner    (1001) docker     (127)    11419 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/missing
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 08:41:47.850533 sabctools-8.1.0/src/crcutil-1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/tests/aligned_alloc.h
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/tests/bob_jenkins_rng.h
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/tests/rdtsc.h
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/tests/set_hi_pri.c
--rw-r--r--   0 runner    (1001) docker     (127)     7593 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/tests/unittest.cc
--rw-r--r--   0 runner    (1001) docker     (127)    33870 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/tests/unittest.h
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/crcutil-1.0/tests/unittest_helper.h
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/sabctools.cc
--rw-r--r--   0 runner    (1001) docker     (127)      963 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/sabctools.h
--rw-r--r--   0 runner    (1001) docker     (127)      703 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/sabctools.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/sparse.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/sparse.h
--rw-r--r--   0 runner    (1001) docker     (127)     8637 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/unlocked_ssl.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/unlocked_ssl.h
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/utils.cc
--rw-r--r--   0 runner    (1001) docker     (127)      937 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/utils.h
--rw-r--r--   0 runner    (1001) docker     (127)    10297 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/yenc.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/yenc.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 08:41:47.854533 sabctools-8.1.0/src/yencode/
--rw-r--r--   0 runner    (1001) docker     (127)     9182 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/yencode/common.h
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/yencode/crc.cc
--rw-r--r--   0 runner    (1001) docker     (127)      413 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/yencode/crc.h
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/yencode/crc_arm.cc
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/yencode/crc_common.h
--rw-r--r--   0 runner    (1001) docker     (127)    13066 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/yencode/crc_folding.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8230 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/yencode/crc_folding_256.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/yencode/decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/yencode/decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)      754 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/yencode/decoder_avx.cc
--rw-r--r--   0 runner    (1001) docker     (127)      771 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/yencode/decoder_avx2.cc
--rw-r--r--   0 runner    (1001) docker     (127)    31441 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/yencode/decoder_avx2_base.h
--rw-r--r--   0 runner    (1001) docker     (127)    18596 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/yencode/decoder_common.h
--rw-r--r--   0 runner    (1001) docker     (127)    21692 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/yencode/decoder_neon.cc
--rw-r--r--   0 runner    (1001) docker     (127)    22632 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/yencode/decoder_neon64.cc
--rw-r--r--   0 runner    (1001) docker     (127)      644 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/yencode/decoder_sse2.cc
--rw-r--r--   0 runner    (1001) docker     (127)    33901 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/yencode/decoder_sse_base.h
--rw-r--r--   0 runner    (1001) docker     (127)      713 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/yencode/decoder_ssse3.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/yencode/decoder_vbmi2.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5383 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/yencode/encoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)      331 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/yencode/encoder.h
--rw-r--r--   0 runner    (1001) docker     (127)      342 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/yencode/encoder_avx.cc
--rw-r--r--   0 runner    (1001) docker     (127)      339 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/yencode/encoder_avx2.cc
--rw-r--r--   0 runner    (1001) docker     (127)    26195 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/yencode/encoder_avx_base.h
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/yencode/encoder_common.h
--rw-r--r--   0 runner    (1001) docker     (127)    21944 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/yencode/encoder_neon.cc
--rw-r--r--   0 runner    (1001) docker     (127)      247 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/yencode/encoder_sse2.cc
--rw-r--r--   0 runner    (1001) docker     (127)    31590 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/yencode/encoder_sse_base.h
--rw-r--r--   0 runner    (1001) docker     (127)      675 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/yencode/encoder_ssse3.cc
--rw-r--r--   0 runner    (1001) docker     (127)      583 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/yencode/encoder_vbmi2.cc
--rw-r--r--   0 runner    (1001) docker     (127)    72124 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/yencode/hedley.h
--rw-r--r--   0 runner    (1001) docker     (127)     6010 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/yencode/platform.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7722 2023-12-20 08:17:02.000000 sabctools-8.1.0/src/yencode/stdint.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:26:49.766345 sabctools-8.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    17990 2024-05-15 11:22:31.000000 sabctools-8.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-15 11:22:31.000000 sabctools-8.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-15 11:26:49.766345 sabctools-8.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-15 11:22:31.000000 sabctools-8.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-15 11:22:31.000000 sabctools-8.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:26:49.750345 sabctools-8.2.0/sabctools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-15 11:26:49.000000 sabctools-8.2.0/sabctools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-15 11:26:49.000000 sabctools-8.2.0/sabctools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 11:26:49.000000 sabctools-8.2.0/sabctools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 11:26:49.000000 sabctools-8.2.0/sabctools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 11:26:49.766345 sabctools-8.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    17765 2024-05-15 11:22:31.000000 sabctools-8.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:26:49.754345 sabctools-8.2.0/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crc32.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crc32.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:26:49.754345 sabctools-8.2.0/src/crcutil-1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/INSTALL
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    50573 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/Makefile.am
+-rw-r--r--   0 runner    (1001) docker     (127)    56163 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/Makefile.win
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/NEWS
+-rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/README
+-rw-r--r--   0 runner    (1001) docker     (127)    34611 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/aclocal.m4
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/autogen.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:26:49.758345 sabctools-8.2.0/src/crcutil-1.0/code/
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/code/base_types.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12545 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/code/crc32c_sse4.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7511 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/code/crc32c_sse4.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/code/crc32c_sse4_intrin.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/code/crc_casts.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21506 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/code/generic_crc.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8663 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/code/gf_util.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/code/multiword_128_64_gcc_amd64_sse2.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/code/multiword_64_64_cl_i386_mmx.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/code/multiword_64_64_gcc_amd64_asm.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7945 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/code/multiword_64_64_gcc_i386_mmx.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7379 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/code/multiword_64_64_intrinsic_i386_mmx.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7264 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/code/platform.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/code/protected_crc.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/code/rolling_crc.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/code/std_headers.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8422 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/code/uint128_sse2.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/config.h.in
+-rw-r--r--   0 runner    (1001) docker     (127)   212367 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/configure
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/configure.ac
+-rw-r--r--   0 runner    (1001) docker     (127)    18615 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/depcomp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:26:49.758345 sabctools-8.2.0/src/crcutil-1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/examples/interface.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8820 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/examples/interface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/examples/usage.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    13663 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/install-sh
+-rw-r--r--   0 runner    (1001) docker     (127)    11419 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/missing
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:26:49.758345 sabctools-8.2.0/src/crcutil-1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/tests/aligned_alloc.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/tests/bob_jenkins_rng.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/tests/rdtsc.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/tests/set_hi_pri.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7593 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/tests/unittest.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    33870 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/tests/unittest.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/crcutil-1.0/tests/unittest_helper.h
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/sabctools.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/sabctools.h
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/sabctools.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/sparse.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/sparse.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8637 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/unlocked_ssl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/unlocked_ssl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/utils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10285 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yenc.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yenc.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:26:49.766345 sabctools-8.2.0/src/yencode/
+-rw-r--r--   0 runner    (1001) docker     (127)    11026 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yencode/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9326 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yencode/crc.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yencode/crc.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yencode/crc_arm.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6864 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yencode/crc_arm_pmull.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yencode/crc_common.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17801 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yencode/crc_folding.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yencode/crc_folding_256.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yencode/crc_riscv.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10917 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yencode/decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yencode/decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yencode/decoder_avx.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yencode/decoder_avx2.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    23461 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yencode/decoder_avx2_base.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7641 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yencode/decoder_common.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17142 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yencode/decoder_neon.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    17359 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yencode/decoder_neon64.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10838 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yencode/decoder_rvv.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yencode/decoder_sse2.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    25288 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yencode/decoder_sse_base.h
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yencode/decoder_ssse3.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yencode/decoder_vbmi2.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yencode/encoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yencode/encoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yencode/encoder_avx.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yencode/encoder_avx2.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    21399 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yencode/encoder_avx_base.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yencode/encoder_common.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19077 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yencode/encoder_neon.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6214 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yencode/encoder_rvv.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yencode/encoder_sse2.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    24611 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yencode/encoder_sse_base.h
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yencode/encoder_ssse3.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yencode/encoder_vbmi2.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    77413 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yencode/hedley.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yencode/platform.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7722 2024-05-15 11:22:31.000000 sabctools-8.2.0/src/yencode/stdint.h
```

### Comparing `sabctools-8.1.0/LICENSE.md` & `sabctools-8.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/PKG-INFO` & `sabctools-8.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sabctools
-Version: 8.1.0
+Version: 8.2.0
 Summary: C implementations of functions for use within SABnzbd
 Home-page: https://github.com/sabnzbd/sabctools/
 Author: Safihre
 Author-email: safihre@sabnzbd.org
 License: GPLv2+
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `sabctools-8.1.0/README.md` & `sabctools-8.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/sabctools.egg-info/PKG-INFO` & `sabctools-8.2.0/sabctools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sabctools
-Version: 8.1.0
+Version: 8.2.0
 Summary: C implementations of functions for use within SABnzbd
 Home-page: https://github.com/sabnzbd/sabctools/
 Author: Safihre
 Author-email: safihre@sabnzbd.org
 License: GPLv2+
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `sabctools-8.1.0/sabctools.egg-info/SOURCES.txt` & `sabctools-8.2.0/sabctools.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -68,36 +68,40 @@
 src/crcutil-1.0/tests/unittest.cc
 src/crcutil-1.0/tests/unittest.h
 src/crcutil-1.0/tests/unittest_helper.h
 src/yencode/common.h
 src/yencode/crc.cc
 src/yencode/crc.h
 src/yencode/crc_arm.cc
+src/yencode/crc_arm_pmull.cc
 src/yencode/crc_common.h
 src/yencode/crc_folding.cc
 src/yencode/crc_folding_256.cc
+src/yencode/crc_riscv.cc
 src/yencode/decoder.cc
 src/yencode/decoder.h
 src/yencode/decoder_avx.cc
 src/yencode/decoder_avx2.cc
 src/yencode/decoder_avx2_base.h
 src/yencode/decoder_common.h
 src/yencode/decoder_neon.cc
 src/yencode/decoder_neon64.cc
+src/yencode/decoder_rvv.cc
 src/yencode/decoder_sse2.cc
 src/yencode/decoder_sse_base.h
 src/yencode/decoder_ssse3.cc
 src/yencode/decoder_vbmi2.cc
 src/yencode/encoder.cc
 src/yencode/encoder.h
 src/yencode/encoder_avx.cc
 src/yencode/encoder_avx2.cc
 src/yencode/encoder_avx_base.h
 src/yencode/encoder_common.h
 src/yencode/encoder_neon.cc
+src/yencode/encoder_rvv.cc
 src/yencode/encoder_sse2.cc
 src/yencode/encoder_sse_base.h
 src/yencode/encoder_ssse3.cc
 src/yencode/encoder_vbmi2.cc
 src/yencode/hedley.h
 src/yencode/platform.cc
 src/yencode/stdint.h
```

### Comparing `sabctools-8.1.0/setup.py` & `sabctools-8.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,16 +80,20 @@
         IS_AARCH64 = True
 
         log.info("==> Baseline detection: ARM=%s, x86=%s, macOS=%s", IS_ARM, IS_X86, IS_MACOS)
 
         # Determine compiler flags
         gcc_arm_neon_flags = []
         gcc_arm_crc_flags = []
+        gcc_arm_crc_pmull_flags = []
         gcc_vpclmulqdq_flags = []
         gcc_vbmi2_flags = []
+        gcc_avx10_flags = []
+        gcc_rvv_flags = []
+        gcc_rvzbkc_flags = []
         gcc_macros = []
         if self.compiler.compiler_type == "msvc":
             # LTCG not enabled due to issues seen with code generation where
             # different ISA extensions are selected for specific files
             ldflags = ["/OPT:REF", "/OPT:ICF"]
             cflags = ["/O2", "/GS-", "/Gy", "/sdl-", "/Oy", "/Oi"]
         else:
@@ -128,17 +132,19 @@
                         gcc_macros.append(("UNSUPPORTED_PLATFORM_ARM", "1"))
                         IS_ARM = False
                 if not autoconf_check(self.compiler, define_check="__aarch64__"):
                     log.info("==> __aarch64__ not available, disabling 64bit extensions")
                     IS_AARCH64 = False
                 if autoconf_check(self.compiler, flag_check="-march=armv8-a+crc"):
                     gcc_arm_crc_flags.append("-march=armv8-a+crc")
+                    gcc_arm_crc_pmull_flags.append("-march=armv8-a+crc+crypto")
                     # Resolve problems on armv7, see issue #56
                     if not IS_AARCH64:
                         gcc_arm_crc_flags.append("-fno-lto")
+                        gcc_arm_crc_pmull_flags.append("-fno-lto")
                 if not IS_AARCH64 and autoconf_check(self.compiler, flag_check="-mfpu=neon"):
                     gcc_arm_neon_flags.append("-mfpu=neon")
                     # Resolve problems on armv7, see issue #56
                     gcc_arm_neon_flags.append("-fno-lto")
 
             # Check for special x32 case
             if (
@@ -161,14 +167,24 @@
                     "-mavx512bw",
                     "-mpopcnt",
                     "-mbmi",
                     "-mbmi2",
                     "-mlzcnt",
                 ]
 
+            if IS_X86 and autoconf_check(self.compiler, flag_check="-mno-evex512"):
+                gcc_avx10_flags = ["-mno-evex512"]
+
+            if machine.startswith("riscv"):
+                arch_flag = "-march=rv" + ("32" if machine.startswith("riscv32") else "64") + "gc"
+                if autoconf_check(self.compiler, flag_check=arch_flag+"v"):
+                    gcc_rvv_flags = [arch_flag+"v"]
+                if autoconf_check(self.compiler, flag_check=arch_flag+"_zbkc"):
+                    gcc_rvzbkc_flags = [arch_flag+"_zbkc"]
+
         srcdeps_crc_common = ["src/yencode/common.h", "src/yencode/crc_common.h", "src/yencode/crc.h"]
         srcdeps_dec_common = ["src/yencode/common.h", "src/yencode/decoder_common.h", "src/yencode/decoder.h"]
         srcdeps_enc_common = ["src/yencode/common.h", "src/yencode/encoder_common.h", "src/yencode/encoder.h"]
 
         # build yencode/crcutil
         output_dir = os.path.dirname(self.build_lib)
         compiled_objects = []
@@ -236,21 +252,21 @@
                 "depends": srcdeps_dec_common + ["decoder_avx2_base.h"],
                 "gcc_x86_flags": ["-mavx2", "-mpopcnt", "-mbmi", "-mbmi2", "-mlzcnt"],
                 "msvc_x86_flags": ["/arch:AVX2"],
             },
             {
                 "sources": ["src/yencode/encoder_vbmi2.cc"],
                 "depends": srcdeps_enc_common + ["encoder_avx_base.h"],
-                "gcc_x86_flags": gcc_vbmi2_flags,
+                "gcc_x86_flags": gcc_vbmi2_flags + gcc_avx10_flags,
                 "msvc_x86_flags": ["/arch:AVX512"],
             },
             {
                 "sources": ["src/yencode/decoder_vbmi2.cc"],
                 "depends": srcdeps_dec_common + ["decoder_avx2_base.h"],
-                "gcc_x86_flags": gcc_vbmi2_flags,
+                "gcc_x86_flags": gcc_vbmi2_flags + gcc_avx10_flags,
                 "msvc_x86_flags": ["/arch:AVX512"],
             },
             {
                 "sources": ["src/yencode/encoder_neon.cc"],
                 "depends": srcdeps_enc_common,
                 "gcc_arm_flags": gcc_arm_neon_flags,
             },
@@ -261,14 +277,29 @@
             },
             {
                 "sources": ["src/yencode/crc_arm.cc"],
                 "depends": srcdeps_crc_common,
                 "gcc_arm_flags": gcc_arm_crc_flags,
             },
             {
+                "sources": ["src/yencode/crc_arm_pmull.cc"],
+                "depends": srcdeps_crc_common,
+                "gcc_arm_flags": gcc_arm_crc_pmull_flags,
+            },
+            {
+                "sources": ["src/yencode/encoder_rvv.cc", "src/yencode/decoder_rvv.cc"],
+                "depends": srcdeps_enc_common + srcdeps_dec_common,
+                "gcc_rv_flags": gcc_rvv_flags,
+            },
+            {
+                "sources": ["src/yencode/crc_riscv.cc"],
+                "depends": srcdeps_crc_common,
+                "gcc_rv_flags": gcc_rvzbkc_flags,
+            },
+            {
                 "sources": [
                     "src/crcutil-1.0/code/crc32c_sse4.cc",
                     "src/crcutil-1.0/code/multiword_64_64_cl_i386_mmx.cc",
                     "src/crcutil-1.0/code/multiword_64_64_gcc_amd64_asm.cc",
                     "src/crcutil-1.0/code/multiword_64_64_gcc_i386_mmx.cc",
                     "src/crcutil-1.0/code/multiword_64_64_intrinsic_i386_mmx.cc",
                     "src/crcutil-1.0/code/multiword_128_64_gcc_amd64_sse2.cc",
```

### Comparing `sabctools-8.1.0/src/crc32.h` & `sabctools-8.2.0/src/crc32.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/COPYING` & `sabctools-8.2.0/src/crcutil-1.0/COPYING`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/INSTALL` & `sabctools-8.2.0/src/crcutil-1.0/INSTALL`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/LICENSE` & `sabctools-8.2.0/src/crcutil-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/Makefile` & `sabctools-8.2.0/src/crcutil-1.0/Makefile`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/Makefile.am` & `sabctools-8.2.0/src/crcutil-1.0/Makefile.am`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/Makefile.in` & `sabctools-8.2.0/src/crcutil-1.0/Makefile.in`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/Makefile.win` & `sabctools-8.2.0/src/crcutil-1.0/Makefile.win`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/README` & `sabctools-8.2.0/src/crcutil-1.0/README`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/aclocal.m4` & `sabctools-8.2.0/src/crcutil-1.0/aclocal.m4`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/autogen.sh` & `sabctools-8.2.0/src/crcutil-1.0/autogen.sh`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/code/base_types.h` & `sabctools-8.2.0/src/crcutil-1.0/code/base_types.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/code/crc32c_sse4.cc` & `sabctools-8.2.0/src/crcutil-1.0/code/crc32c_sse4.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/code/crc32c_sse4.h` & `sabctools-8.2.0/src/crcutil-1.0/code/crc32c_sse4.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/code/crc32c_sse4_intrin.h` & `sabctools-8.2.0/src/crcutil-1.0/code/crc32c_sse4_intrin.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/code/crc_casts.h` & `sabctools-8.2.0/src/crcutil-1.0/code/crc_casts.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/code/generic_crc.h` & `sabctools-8.2.0/src/crcutil-1.0/code/generic_crc.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/code/gf_util.h` & `sabctools-8.2.0/src/crcutil-1.0/code/gf_util.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/code/multiword_128_64_gcc_amd64_sse2.cc` & `sabctools-8.2.0/src/crcutil-1.0/code/multiword_128_64_gcc_amd64_sse2.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/code/multiword_64_64_cl_i386_mmx.cc` & `sabctools-8.2.0/src/crcutil-1.0/code/multiword_64_64_cl_i386_mmx.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/code/multiword_64_64_gcc_amd64_asm.cc` & `sabctools-8.2.0/src/crcutil-1.0/code/multiword_64_64_gcc_amd64_asm.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/code/multiword_64_64_gcc_i386_mmx.cc` & `sabctools-8.2.0/src/crcutil-1.0/code/multiword_64_64_gcc_i386_mmx.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/code/multiword_64_64_intrinsic_i386_mmx.cc` & `sabctools-8.2.0/src/crcutil-1.0/code/multiword_64_64_intrinsic_i386_mmx.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/code/platform.h` & `sabctools-8.2.0/src/crcutil-1.0/code/platform.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/code/protected_crc.h` & `sabctools-8.2.0/src/crcutil-1.0/code/protected_crc.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/code/rolling_crc.h` & `sabctools-8.2.0/src/crcutil-1.0/code/rolling_crc.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/code/std_headers.h` & `sabctools-8.2.0/src/crcutil-1.0/code/std_headers.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/code/uint128_sse2.h` & `sabctools-8.2.0/src/crcutil-1.0/code/uint128_sse2.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/config.h.in` & `sabctools-8.2.0/src/crcutil-1.0/config.h.in`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/configure` & `sabctools-8.2.0/src/crcutil-1.0/configure`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/configure.ac` & `sabctools-8.2.0/src/crcutil-1.0/configure.ac`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/depcomp` & `sabctools-8.2.0/src/crcutil-1.0/depcomp`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/examples/interface.cc` & `sabctools-8.2.0/src/crcutil-1.0/examples/interface.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/examples/interface.h` & `sabctools-8.2.0/src/crcutil-1.0/examples/interface.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/examples/usage.cc` & `sabctools-8.2.0/src/crcutil-1.0/examples/usage.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/install-sh` & `sabctools-8.2.0/src/crcutil-1.0/install-sh`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/missing` & `sabctools-8.2.0/src/crcutil-1.0/missing`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/tests/aligned_alloc.h` & `sabctools-8.2.0/src/crcutil-1.0/tests/aligned_alloc.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/tests/bob_jenkins_rng.h` & `sabctools-8.2.0/src/crcutil-1.0/tests/bob_jenkins_rng.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/tests/rdtsc.h` & `sabctools-8.2.0/src/crcutil-1.0/tests/rdtsc.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/tests/set_hi_pri.c` & `sabctools-8.2.0/src/crcutil-1.0/tests/set_hi_pri.c`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/tests/unittest.cc` & `sabctools-8.2.0/src/crcutil-1.0/tests/unittest.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/tests/unittest.h` & `sabctools-8.2.0/src/crcutil-1.0/tests/unittest.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/crcutil-1.0/tests/unittest_helper.h` & `sabctools-8.2.0/src/crcutil-1.0/tests/unittest_helper.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/sabctools.h` & `sabctools-8.2.0/src/sabctools.h`

 * *Files 10% similar despite different names*

```diff
@@ -18,10 +18,10 @@
 
 #include <Python.h>
 #include <stdio.h>
 #include <fcntl.h>
 #include <string.h>
 
 /* Version information */
-#define SABCTOOLS_VERSION "8.1.0"
+#define SABCTOOLS_VERSION "8.2.0"
 
 PyMODINIT_FUNC PyInit_sabctools(void);
```

### Comparing `sabctools-8.1.0/src/sabctools.pyi` & `sabctools-8.2.0/src/sabctools.pyi`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/sparse.cc` & `sabctools-8.2.0/src/sparse.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/sparse.h` & `sabctools-8.2.0/src/sparse.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/unlocked_ssl.cc` & `sabctools-8.2.0/src/unlocked_ssl.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/unlocked_ssl.h` & `sabctools-8.2.0/src/unlocked_ssl.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/utils.cc` & `sabctools-8.2.0/src/utils.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/utils.h` & `sabctools-8.2.0/src/utils.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/yenc.cc` & `sabctools-8.2.0/src/yenc.cc`

 * *Files 5% similar despite different names*

```diff
@@ -211,17 +211,17 @@
     }
     dest_loc = PyByteArray_AsString(Py_output_bytearray);
 
     // Lift the GIL
     Py_BEGIN_ALLOW_THREADS;
 
     // send to decoder
-    YencDecoderState state = YDEC_STATE_CRLF;
-    output_len = do_decode(1, (unsigned char*) start_loc, (unsigned char*) dest_loc, yenc_data_length, &state);
-    crc = do_crc32(dest_loc, output_len, crc);
+    RapidYenc::YencDecoderState state = RapidYenc::YDEC_STATE_CRLF;
+    output_len = RapidYenc::decode(1, start_loc, dest_loc, yenc_data_length, &state);
+    crc = RapidYenc::crc32(dest_loc, output_len, crc);
 
     // Return GIL to perform Python modifications
     Py_END_ALLOW_THREADS;
 
     // Is there a valid CRC?
     if (crc != crc_yenc) {
         Py_output_crc = Py_None;
@@ -285,16 +285,16 @@
         return PyErr_NoMemory();
 
     // Free GIL, in case it helps
     Py_BEGIN_ALLOW_THREADS;
 
     // Encode result
     int column = 0;
-    output_len = do_encode(YENC_LINESIZE, &column, (unsigned char*)input_buffer, (unsigned char*)output_buffer, input_len, 1);
-    crc = do_crc32(input_buffer, input_len, 0);
+    output_len = RapidYenc::encode(YENC_LINESIZE, &column, input_buffer, output_buffer, input_len, 1);
+    crc = RapidYenc::crc32(input_buffer, input_len, 0);
 
     // Restore GIL so we can build Python strings
     Py_END_ALLOW_THREADS;
 
     // Build output string
     Py_output_string = PyBytes_FromStringAndSize((char *)output_buffer, output_len);
     if(Py_output_string)
```

### Comparing `sabctools-8.1.0/src/yenc.h` & `sabctools-8.2.0/src/yenc.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.1.0/src/yencode/crc_arm.cc` & `sabctools-8.2.0/src/yencode/crc_arm.cc`

 * *Files 20% similar despite different names*

```diff
@@ -12,14 +12,20 @@
 HEDLEY_WARNING("CRC32 acceleration has been disabled due to broken arm_acle.h shipped in GCC 7.0 - 8.1 [https://gcc.gnu.org/bugzilla/show_bug.cgi?id=81497]. If you need this feature, please use a different compiler or version of GCC");
 # endif
 # if defined(__aarch64__) && HEDLEY_GCC_VERSION_CHECK(9,4,0) && !HEDLEY_GCC_VERSION_CHECK(9,5,0)
 #  undef __ARM_FEATURE_CRC32
 HEDLEY_WARNING("CRC32 acceleration has been disabled due to broken arm_acle.h shipped in GCC 9.4 [https://gcc.gnu.org/bugzilla/show_bug.cgi?id=100985]. If you need this feature, please use a different compiler or version of GCC");
 # endif
 #endif
+#if defined(__ARM_FEATURE_CRC32) && defined(__has_include)
+# if !__has_include(<arm_acle.h>)
+#  undef __ARM_FEATURE_CRC32
+HEDLEY_WARNING("CRC32 acceleration has been disabled due to missing arm_acle.h");
+# endif
+#endif
 
 #if defined(__ARM_FEATURE_CRC32) || (defined(_M_ARM64) && !defined(__clang__)) // MSVC doesn't support CRC for ARM32
 
 /* ARMv8 accelerated CRC */
 #if defined(_MSC_VER) && !defined(__clang__)
 #include <intrin.h>
 #else
@@ -49,157 +55,172 @@
 #else
 # define WORD_T uint32_t
 # define WORDSIZE_LOG 2  // sizeof(WORD_T) == 1<<WORDSIZE_LOG
 # define CRC_WORD(crc, data) __crc32w(crc, _LE32(data))
 #endif
 
 
+
+#ifdef __aarch64__
+static uint32_t crc32_multiply_arm(uint32_t a, uint32_t b) {
+	// perform PMULL
+	uint64_t res = 0;
+	uint64_t a64 = (uint64_t)a << 32;
+	int64_t b64 = (int64_t)b << 32;
+	for(int i=0; i<32; i++) {
+		res ^= a64 & (b64 >> 63);
+		b64 += b64;
+		a64 >>= 1;
+	}
+	// reduction via CRC
+	res = __crc32w(0, res) ^ (res >> 32);
+	return res;
+}
+#endif
+// regular multiply is probably better for AArch32
+
+
 // exploit CPU pipelining during CRC computation; unfortunately I haven't been able to measure any benefit
 // - Neoverse N1: no noticeable difference
 // - Cortex A53: actually runs a bit slower
 //#define ENABLE_PIPELINE_OPT 1
 
 #ifdef ENABLE_PIPELINE_OPT
-// workaround MSVC complaining "unary minus operator applied to unsigned type, result still unsigned"
-#define NEGATE(n) (uint32_t)(-((int32_t)(n)))
-
-static HEDLEY_ALWAYS_INLINE uint32_t crc_multiply(uint32_t a, uint32_t b) {
-    uint32_t res = 0;
-    for(int i=0; i<31; i++) {
-        res ^= NEGATE(b>>31) & a;
-        a = ((a >> 1) ^ (0xEDB88320 & NEGATE(a&1)));
-        b <<= 1;
-    }
-    res ^= NEGATE(b>>31) & a;
-    return res;
-}
-
-static const uint32_t crc_power[] = { // pre-computed 2^n, with first 3 entries removed (saves a shift)
-    0x00800000, 0x00008000, 0xedb88320, 0xb1e6b092, 0xa06a2517, 0xed627dae, 0x88d14467, 0xd7bbfe6a,
-    0xec447f11, 0x8e7ea170, 0x6427800e, 0x4d47bae0, 0x09fe548f, 0x83852d0f, 0x30362f1a, 0x7b5a9cc3,
-    0x31fec169, 0x9fec022a, 0x6c8dedc4, 0x15d6874d, 0x5fde7a4e, 0xbad90e37, 0x2e4e5eef, 0x4eaba214,
-    0xa8a472c0, 0x429a969e, 0x148d302a, 0xc40ba6d0, 0xc4e22c3c, 0x40000000, 0x20000000, 0x08000000
-};
-/* above table can be computed with
-    int main(void) {
-        uint32_t k = 0x80000000 >> 1;
-        for (size_t i = 0; i < 32+3; ++i) {
-            if(i>2) printf("0x%08x, ", k);
-            k = crc_multiply(k, k);
-        }
-        return 0;
-    }
-*/
+#ifndef __aarch64__
+# define crc32_multiply_arm RapidYenc::crc32_multiply_generic
 #endif
+#endif
+
 
 
 // inspired/stolen off https://github.com/jocover/crc32_armv8/blob/master/crc32_armv8.c
 static uint32_t arm_crc_calc(uint32_t crc, const unsigned char *src, long len) {
-
-    // initial alignment
-    if (len >= 16) { // 16 is an arbitrary number; it just needs to be >=8
-        if ((uintptr_t)src & sizeof(uint8_t)) {
-            crc = __crc32b(crc, *src);
-            src++;
-            len--;
-        }
-        if ((uintptr_t)src & sizeof(uint16_t)) {
-            crc = __crc32h(crc, _LE16(*((uint16_t *)src)));
-            src += sizeof(uint16_t);
-            len -= sizeof(uint16_t);
-        }
+	
+	// initial alignment
+	if (len >= 16) { // 16 is an arbitrary number; it just needs to be >=8
+		if ((uintptr_t)src & sizeof(uint8_t)) {
+			crc = __crc32b(crc, *src);
+			src++;
+			len--;
+		}
+		if ((uintptr_t)src & sizeof(uint16_t)) {
+			crc = __crc32h(crc, _LE16(*((uint16_t *)src)));
+			src += sizeof(uint16_t);
+			len -= sizeof(uint16_t);
+		}
 #ifdef __aarch64__
-        if ((uintptr_t)src & sizeof(uint32_t)) {
-            crc = __crc32w(crc, _LE32(*((uint32_t *)src)));
-            src += sizeof(uint32_t);
-            len -= sizeof(uint32_t);
-        }
-#endif
-    }
-
-    const WORD_T* srcW = (const WORD_T*)src;
-
+		if ((uintptr_t)src & sizeof(uint32_t)) {
+			crc = __crc32w(crc, _LE32(*((uint32_t *)src)));
+			src += sizeof(uint32_t);
+			len -= sizeof(uint32_t);
+		}
+#endif
+	}
+	
+	const WORD_T* srcW = (const WORD_T*)src;
+	
 #ifdef ENABLE_PIPELINE_OPT
-    // uses ideas from https://github.com/komrad36/crc#option-13-golden
-    // (this is a slightly less efficient, but much simpler implementation of the idea)
-    const unsigned SPLIT_WORDS_LOG = 10;  // make sure it's at least 2
-    const unsigned SPLIT_WORDS = 1<<SPLIT_WORDS_LOG;
-    while(len >= (long)(sizeof(WORD_T)*SPLIT_WORDS*2)) {
-        // compute 2x CRCs concurrently to leverage piplining
-        uint32_t crc2 = 0;
-        for(unsigned i=0; i<SPLIT_WORDS; i+=4) {
-            crc = CRC_WORD(crc, *srcW);
-            crc2 = CRC_WORD(crc2, *(srcW + SPLIT_WORDS));
-            srcW++;
-            crc = CRC_WORD(crc, *srcW);
-            crc2 = CRC_WORD(crc2, *(srcW + SPLIT_WORDS));
-            srcW++;
-            crc = CRC_WORD(crc, *srcW);
-            crc2 = CRC_WORD(crc2, *(srcW + SPLIT_WORDS));
-            srcW++;
-            crc = CRC_WORD(crc, *srcW);
-            crc2 = CRC_WORD(crc2, *(srcW + SPLIT_WORDS));
-            srcW++;
-        }
-        // merge the CRCs
-        // since we're multiplying by a fixed number, it could be sped up with some lookup tables
-        crc = crc_multiply(crc, crc_power[SPLIT_WORDS_LOG + WORDSIZE_LOG]) ^ crc2;
-        srcW += SPLIT_WORDS;
-        len -= sizeof(WORD_T)*SPLIT_WORDS*2;
-    }
-#endif
-
-    while ((len -= sizeof(WORD_T)*8) >= 0) {
-        crc = CRC_WORD(crc, *(srcW++));
-        crc = CRC_WORD(crc, *(srcW++));
-        crc = CRC_WORD(crc, *(srcW++));
-        crc = CRC_WORD(crc, *(srcW++));
-        crc = CRC_WORD(crc, *(srcW++));
-        crc = CRC_WORD(crc, *(srcW++));
-        crc = CRC_WORD(crc, *(srcW++));
-        crc = CRC_WORD(crc, *(srcW++));
-    }
-    if (len & sizeof(WORD_T)*4) {
-        crc = CRC_WORD(crc, *(srcW++));
-        crc = CRC_WORD(crc, *(srcW++));
-        crc = CRC_WORD(crc, *(srcW++));
-        crc = CRC_WORD(crc, *(srcW++));
-    }
-    if (len & sizeof(WORD_T)*2) {
-        crc = CRC_WORD(crc, *(srcW++));
-        crc = CRC_WORD(crc, *(srcW++));
-    }
-    if (len & sizeof(WORD_T)) {
-        crc = CRC_WORD(crc, *(srcW++));
-    }
-    src = (const unsigned char*)srcW;
-
+	// uses ideas from https://github.com/komrad36/crc#option-13-golden
+	// (this is a slightly less efficient, but much simpler implementation of the idea)
+	const unsigned SPLIT_WORDS_LOG = 10;  // make sure it's at least 2
+	const unsigned SPLIT_WORDS = 1<<SPLIT_WORDS_LOG;
+	const unsigned blockCoeff = RapidYenc::crc_power[SPLIT_WORDS_LOG + WORDSIZE_LOG + 3];
+	while(len >= (long)(sizeof(WORD_T)*SPLIT_WORDS*2)) {
+		// compute 2x CRCs concurrently to leverage piplining
+		uint32_t crc2 = 0;
+		for(unsigned i=0; i<SPLIT_WORDS; i+=4) {
+			crc = CRC_WORD(crc, *srcW);
+			crc2 = CRC_WORD(crc2, *(srcW + SPLIT_WORDS));
+			srcW++;
+			crc = CRC_WORD(crc, *srcW);
+			crc2 = CRC_WORD(crc2, *(srcW + SPLIT_WORDS));
+			srcW++;
+			crc = CRC_WORD(crc, *srcW);
+			crc2 = CRC_WORD(crc2, *(srcW + SPLIT_WORDS));
+			srcW++;
+			crc = CRC_WORD(crc, *srcW);
+			crc2 = CRC_WORD(crc2, *(srcW + SPLIT_WORDS));
+			srcW++;
+		}
+		// merge the CRCs
+		crc = crc32_multiply_arm(crc, blockCoeff) ^ crc2;
+		srcW += SPLIT_WORDS;
+		len -= sizeof(WORD_T)*SPLIT_WORDS*2;
+	}
+#endif
+	
+	while ((len -= sizeof(WORD_T)*8) >= 0) {
+		crc = CRC_WORD(crc, *(srcW++));
+		crc = CRC_WORD(crc, *(srcW++));
+		crc = CRC_WORD(crc, *(srcW++));
+		crc = CRC_WORD(crc, *(srcW++));
+		crc = CRC_WORD(crc, *(srcW++));
+		crc = CRC_WORD(crc, *(srcW++));
+		crc = CRC_WORD(crc, *(srcW++));
+		crc = CRC_WORD(crc, *(srcW++));
+	}
+	if (len & sizeof(WORD_T)*4) {
+		crc = CRC_WORD(crc, *(srcW++));
+		crc = CRC_WORD(crc, *(srcW++));
+		crc = CRC_WORD(crc, *(srcW++));
+		crc = CRC_WORD(crc, *(srcW++));
+	}
+	if (len & sizeof(WORD_T)*2) {
+		crc = CRC_WORD(crc, *(srcW++));
+		crc = CRC_WORD(crc, *(srcW++));
+	}
+	if (len & sizeof(WORD_T)) {
+		crc = CRC_WORD(crc, *(srcW++));
+	}
+	src = (const unsigned char*)srcW;
+	
 #ifdef __aarch64__
-    if (len & sizeof(uint32_t)) {
-        crc = __crc32w(crc, _LE32(*((uint32_t *)src)));
-        src += sizeof(uint32_t);
-    }
-#endif
-    if (len & sizeof(uint16_t)) {
-        crc = __crc32h(crc, _LE16(*((uint16_t *)src)));
-        src += sizeof(uint16_t);
-    }
-    if (len & sizeof(uint8_t))
-        crc = __crc32b(crc, *src);
-
-    return crc;
+	if (len & sizeof(uint32_t)) {
+		crc = __crc32w(crc, _LE32(*((uint32_t *)src)));
+		src += sizeof(uint32_t);
+	}
+#endif
+	if (len & sizeof(uint16_t)) {
+		crc = __crc32h(crc, _LE16(*((uint16_t *)src)));
+		src += sizeof(uint16_t);
+	}
+	if (len & sizeof(uint8_t))
+		crc = __crc32b(crc, *src);
+	
+	return crc;
 }
 
 static uint32_t do_crc32_incremental_arm(const void* data, size_t length, uint32_t init) {
-    return ~arm_crc_calc(~init, (const unsigned char*)data, (long)length);
+	return ~arm_crc_calc(~init, (const unsigned char*)data, (long)length);
 }
 
-void crc_arm_set_funcs(crc_func* _do_crc32_incremental) {
-    *_do_crc32_incremental = &do_crc32_incremental_arm;
-}
-#else
 
-void crc_arm_set_funcs(crc_func *_do_crc32_incremental) {
-    (void) _do_crc32_incremental;
+#if defined(__aarch64__) && (defined(__GNUC__) || defined(_MSC_VER))
+static uint32_t crc32_shift_arm(uint32_t crc1, uint32_t n) {
+	uint32_t result = crc1;
+	uint64_t prod = result;
+	prod <<= 32 - (n&31);
+	result = __crc32w(0, prod) ^ (prod >> 32);
+	n &= ~31;
+	
+	while(n) {
+		result = crc32_multiply_arm(result, RapidYenc::crc_power[ctz32(n)]);
+		n &= n-1;
+	}
+	return result;
 }
+#endif
+
 
+void RapidYenc::crc_arm_set_funcs() {
+	_do_crc32_incremental = &do_crc32_incremental_arm;
+#ifdef __aarch64__
+	_crc32_multiply = &crc32_multiply_arm;
+# if defined(__GNUC__) || defined(_MSC_VER)
+	_crc32_shift = &crc32_shift_arm;
+# endif
+#endif
+	_crc32_isa = ISA_FEATURE_CRC;
+}
+#else
+void RapidYenc::crc_arm_set_funcs() {}
 #endif
```

### Comparing `sabctools-8.1.0/src/yencode/decoder_avx2.cc` & `sabctools-8.2.0/src/yencode/decoder_avx2.cc`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 #include "common.h"
 
-#if defined(__AVX2__) && !defined(YENC_DISABLE_AVX256)
 #include "decoder_common.h"
+#if defined(__AVX2__) && !defined(YENC_DISABLE_AVX256)
 #include "decoder_avx2_base.h"
-void decoder_set_avx2_funcs() {
-    ALIGN_ALLOC(lookups, sizeof(*lookups), 16);
-    decoder_init_lut(lookups->eqFix, lookups->compact);
-    _do_decode = &do_decode_simd<false, false, sizeof(__m256i)*2, do_decode_avx2<false, false, ISA_LEVEL_AVX2> >;
-    _do_decode_raw = &do_decode_simd<true, false, sizeof(__m256i)*2, do_decode_avx2<true, false, ISA_LEVEL_AVX2> >;
-    _do_decode_end_raw = &do_decode_simd<true, true, sizeof(__m256i)*2, do_decode_avx2<true, true, ISA_LEVEL_AVX2> >;
-    _decode_simd_level = ISA_LEVEL_AVX2;
+void RapidYenc::decoder_set_avx2_funcs() {
+	ALIGN_ALLOC(lookups, sizeof(*lookups), 16);
+	decoder_init_lut(lookups->compact);
+	RapidYenc::_do_decode = &do_decode_simd<false, false, sizeof(__m256i)*2, do_decode_avx2<false, false, ISA_LEVEL_AVX2> >;
+	RapidYenc::_do_decode_raw = &do_decode_simd<true, false, sizeof(__m256i)*2, do_decode_avx2<true, false, ISA_LEVEL_AVX2> >;
+	RapidYenc::_do_decode_end_raw = &do_decode_simd<true, true, sizeof(__m256i)*2, do_decode_avx2<true, true, ISA_LEVEL_AVX2> >;
+	RapidYenc::_decode_isa = ISA_LEVEL_AVX2;
 }
 #else
-
-void decoder_set_avx_funcs();
-
-void decoder_set_avx2_funcs() {
-    decoder_set_avx_funcs();
+void RapidYenc::decoder_set_avx2_funcs() {
+	decoder_set_avx_funcs();
 }
-
 #endif
```

### Comparing `sabctools-8.1.0/src/yencode/decoder_avx2_base.h` & `sabctools-8.2.0/src/yencode/decoder_avx2_base.h`

 * *Files 25% similar despite different names*

```diff
@@ -10,617 +10,609 @@
 # define KORTEST32(a, b) ((a) | (b))
 # define KAND32(a, b) ((a) & (b))
 # define KOR32(a, b) ((a) | (b))
 #endif
 
 #pragma pack(16)
 static struct {
-    /*align16*/ struct { char bytes[16]; } compact[32768];
-    uint8_t eqFix[256];
+	/*align16*/ struct { char bytes[16]; } compact[32768];
 } * HEDLEY_RESTRICT lookups;
 #pragma pack()
 
 
 static HEDLEY_ALWAYS_INLINE __m256i force_align_read_256(const void* p) {
 #ifdef _MSC_VER
-    // MSVC complains about casting away volatile
-    return *(__m256i *)(p);
+	// MSVC complains about casting away volatile
+	return *(__m256i *)(p);
 #else
-    return *(volatile __m256i *)(p);
+	return *(volatile __m256i *)(p);
 #endif
 }
 
 // _mm256_castsi128_si256, but upper is defined to be 0
-#if (defined(__clang__) && __clang_major__ >= 5 && (!defined(__APPLE__) || __clang_major__ >= 7)) || (defined(__GNUC__) && __GNUC__ >= 10)
+#if (defined(__clang__) && __clang_major__ >= 5 && (!defined(__APPLE__) || __clang_major__ >= 7)) || (defined(__GNUC__) && __GNUC__ >= 10) || (defined(_MSC_VER) && _MSC_VER >= 1910)
 // intrinsic unsupported in GCC 9 and MSVC < 2017
 # define zext128_256 _mm256_zextsi128_si256
 #else
 // technically a cast is incorrect, due to upper 128 bits being undefined, but should usually work fine
 // alternative may be `_mm256_set_m128i(_mm_setzero_si128(), v)` but unsupported on GCC < 7, and most compilers generate a VINSERTF128 instruction for it
 # ifdef __OPTIMIZE__
 #  define zext128_256 _mm256_castsi128_si256
 # else
 #  define zext128_256(x) _mm256_inserti128_si256(_mm256_setzero_si256(), x, 0)
 # endif
 #endif
 
+#if defined(__tune_icelake_client__) || defined(__tune_icelake_server__) || defined(__tune_tigerlake__) || defined(__tune_rocketlake__) || defined(__tune_alderlake__) || defined(__tune_sapphirerapids__)
+# define COMPRESS_STORE _mm256_mask_compressstoreu_epi8
+#else
+// avoid uCode on Zen4
+# define COMPRESS_STORE(dst, mask, vec) _mm256_storeu_si256((__m256i*)(dst), _mm256_maskz_compress_epi8(mask, vec))
+#endif
 
-template<bool isRaw, bool searchEnd, enum YEncDecIsaLevel use_isa>
-HEDLEY_ALWAYS_INLINE void do_decode_avx2(const uint8_t* HEDLEY_RESTRICT src, long& len, unsigned char* HEDLEY_RESTRICT & p, unsigned char& _escFirst, uint16_t& _nextMask) {
-    HEDLEY_ASSUME(_escFirst == 0 || _escFirst == 1);
-    HEDLEY_ASSUME(_nextMask == 0 || _nextMask == 1 || _nextMask == 2);
-    uintptr_t escFirst = _escFirst;
-    __m256i yencOffset = escFirst ? _mm256_set_epi8(
-        -42,-42,-42,-42,-42,-42,-42,-42,-42,-42,-42,-42,-42,-42,-42,-42,
-        -42,-42,-42,-42,-42,-42,-42,-42,-42,-42,-42,-42,-42,-42,-42,-42-64
-    ) : _mm256_set1_epi8(-42);
-    __m256i minMask = _mm256_set1_epi8('.');
-    if(_nextMask && isRaw) {
-        minMask = _mm256_set_epi8(
-            '.','.','.','.','.','.','.','.','.','.','.','.','.','.','.','.',
-            '.','.','.','.','.','.','.','.','.','.','.','.','.','.',_nextMask==2?0:'.',_nextMask==1?0:'.'
-        );
-    }
+namespace RapidYenc {
 
-    // for some reason, MSVC Win32 seems to crash when trying to compile _mm256_mask_cmpeq_epi8_mask
-    // the crash can be fixed by switching the order of the last two arguments, but it seems to generate wrong code
-    // so just disable the optimisation as it seems to be problematic there
+template<bool isRaw, bool searchEnd, enum YEncDecIsaLevel use_isa>
+HEDLEY_ALWAYS_INLINE void do_decode_avx2(const uint8_t* src, long& len, unsigned char*& p, unsigned char& _escFirst, uint16_t& _nextMask) {
+	HEDLEY_ASSUME(_escFirst == 0 || _escFirst == 1);
+	HEDLEY_ASSUME(_nextMask == 0 || _nextMask == 1 || _nextMask == 2);
+	uintptr_t escFirst = _escFirst;
+	__m256i yencOffset = escFirst ? _mm256_set_epi8(
+		-42,-42,-42,-42,-42,-42,-42,-42,-42,-42,-42,-42,-42,-42,-42,-42,
+		-42,-42,-42,-42,-42,-42,-42,-42,-42,-42,-42,-42,-42,-42,-42,-42-64
+	) : _mm256_set1_epi8(-42);
+	__m256i minMask = _mm256_set1_epi8('.');
+	if(_nextMask && isRaw) {
+		minMask = _mm256_set_epi8(
+			'.','.','.','.','.','.','.','.','.','.','.','.','.','.','.','.',
+			'.','.','.','.','.','.','.','.','.','.','.','.','.','.',_nextMask==2?0:'.',_nextMask==1?0:'.'
+		);
+	}
+	
+	decoder_set_nextMask<isRaw>(src, len, _nextMask); // set this before the loop because we can't check src after it's been overwritten
+	
+	// for some reason, MSVC Win32 seems to crash when trying to compile _mm256_mask_cmpeq_epi8_mask
+	// the crash can be fixed by switching the order of the last two arguments, but it seems to generate wrong code
+	// so just disable the optimisation as it seems to be problematic there
 #if defined(__AVX512VL__) && defined(__AVX512BW__)
 # if defined(_MSC_VER) && !defined(PLATFORM_AMD64) && !defined(__clang__)
-    const bool useAVX3MaskCmp = false;
+	const bool useAVX3MaskCmp = false;
 # else
-    const bool useAVX3MaskCmp = (use_isa >= ISA_LEVEL_AVX3);
+	const bool useAVX3MaskCmp = (use_isa >= ISA_LEVEL_AVX3);
 # endif
 #endif
-    intptr_t i;
-    for(i = -len; i; i += sizeof(__m256i)*2) {
-        __m256i oDataA = _mm256_load_si256((__m256i *)(src+i));
-        __m256i oDataB = _mm256_load_si256((__m256i *)(src+i) + 1);
-
-        // search for special chars
-        __m256i cmpA = _mm256_cmpeq_epi8(oDataA, _mm256_shuffle_epi8(
-            _mm256_set_epi8(
-                -1,'=','\r',-1,-1,'\n',-1,-1,-1,-1,-1,-1,-1,-1,-1,'.',
-                -1,'=','\r',-1,-1,'\n',-1,-1,-1,-1,-1,-1,-1,-1,-1,'.'
-            ),
-            _mm256_min_epu8(oDataA, minMask)
-        ));
-        __m256i cmpB = _mm256_cmpeq_epi8(oDataB, _mm256_shuffle_epi8(
-            _mm256_set_epi8(
-                -1,'=','\r',-1,-1,'\n',-1,-1,-1,-1,-1,-1,-1,-1,-1,'.',
-                -1,'=','\r',-1,-1,'\n',-1,-1,-1,-1,-1,-1,-1,-1,-1,'.'
-            ),
-            _mm256_min_epu8(oDataB, _mm256_set1_epi8('.'))
-        ));
-
-        // TODO: can OR the vectors together to save generating a mask, but may not be worth it
-        uint64_t mask = (uint32_t)_mm256_movemask_epi8(cmpB); // not the most accurate mask if we have invalid sequences; we fix this up later
-        mask = (mask << 32) | (uint32_t)_mm256_movemask_epi8(cmpA);
-        __m256i dataA, dataB;
-        if(use_isa >= ISA_LEVEL_AVX3)
-            dataA = _mm256_add_epi8(oDataA, yencOffset);
-
-        if (mask != 0) {
-            __m256i cmpEqA = _mm256_cmpeq_epi8(oDataA, _mm256_set1_epi8('='));
-            __m256i cmpEqB = _mm256_cmpeq_epi8(oDataB, _mm256_set1_epi8('='));
-            uint64_t maskEq = (uint32_t)_mm256_movemask_epi8(cmpEqB);
-            maskEq = (maskEq << 32) | (uint32_t)_mm256_movemask_epi8(cmpEqA);
-
-            // handle \r\n. sequences
-            // RFC3977 requires the first dot on a line to be stripped, due to dot-stuffing
-            if((isRaw || searchEnd) && LIKELIHOOD(0.45, mask != maskEq)) {
+	intptr_t i;
+	for(i = -len; i; i += sizeof(__m256i)*2) {
+		__m256i oDataA = _mm256_load_si256((__m256i *)(src+i));
+		__m256i oDataB = _mm256_load_si256((__m256i *)(src+i) + 1);
+		
+		// search for special chars
+		__m256i cmpA = _mm256_cmpeq_epi8(oDataA, _mm256_shuffle_epi8(
+			_mm256_set_epi8(
+				-1,'=','\r',-1,-1,'\n',-1,-1,-1,-1,-1,-1,-1,-1,-1,'.',
+				-1,'=','\r',-1,-1,'\n',-1,-1,-1,-1,-1,-1,-1,-1,-1,'.'
+			),
+			_mm256_min_epu8(oDataA, minMask)
+		));
+		__m256i cmpB = _mm256_cmpeq_epi8(oDataB, _mm256_shuffle_epi8(
+			_mm256_set_epi8(
+				-1,'=','\r',-1,-1,'\n',-1,-1,-1,-1,-1,-1,-1,-1,-1,'.',
+				-1,'=','\r',-1,-1,'\n',-1,-1,-1,-1,-1,-1,-1,-1,-1,'.'
+			),
+			_mm256_min_epu8(oDataB, _mm256_set1_epi8('.'))
+		));
+		
+		// TODO: can OR the vectors together to save generating a mask, but may not be worth it
+		uint64_t mask = (uint32_t)_mm256_movemask_epi8(cmpB); // not the most accurate mask if we have invalid sequences; we fix this up later
+		mask = (mask << 32) | (uint32_t)_mm256_movemask_epi8(cmpA);
+		__m256i dataA, dataB;
+		if(use_isa >= ISA_LEVEL_AVX3)
+			dataA = _mm256_add_epi8(oDataA, yencOffset);
+		
+		if (mask != 0) {
+			__m256i cmpEqA = _mm256_cmpeq_epi8(oDataA, _mm256_set1_epi8('='));
+			__m256i cmpEqB = _mm256_cmpeq_epi8(oDataB, _mm256_set1_epi8('='));
+			uint64_t maskEq = (uint32_t)_mm256_movemask_epi8(cmpEqB);
+			maskEq = (maskEq << 32) | (uint32_t)_mm256_movemask_epi8(cmpEqA);
+			
+			// handle \r\n. sequences
+			// RFC3977 requires the first dot on a line to be stripped, due to dot-stuffing
+			if((isRaw || searchEnd) && LIKELIHOOD(0.45, mask != maskEq)) {
 #if 0
-                // prefer shuffling data over unaligned loads on Zen (unknown if worth it on Zen2/Excavator)
-                // unfortunately not beneficial, probably due to available register pressure; this is left here because it could be beneficial if we figure out how to use fewer registers
-                __m256i nextDataA, nextDataB;
-                if(searchEnd) {
-                    nextDataA = _mm256_inserti128_si256(
-                        _mm256_castsi128_si256(_mm256_extracti128_si256(oDataA, 1)),
-                        _mm256_castsi256_si128(oDataB),
-                        1
-                    );
-                    nextDataB = _mm256_inserti128_si256(
-                        _mm256_castsi128_si256(_mm256_extracti128_si256(oDataB, 1)),
-                        _mm_load_si128((__m128i*)(src+i+sizeof(__m256i)*2)),
-                        1
-                    );
-                }
+				// prefer shuffling data over unaligned loads on Zen (unknown if worth it on Zen2/Excavator)
+				// unfortunately not beneficial, probably due to available register pressure; this is left here because it could be beneficial if we figure out how to use fewer registers
+				__m256i nextDataA, nextDataB;
+				if(searchEnd) {
+					nextDataA = _mm256_inserti128_si256(
+						_mm256_castsi128_si256(_mm256_extracti128_si256(oDataA, 1)),
+						_mm256_castsi256_si128(oDataB),
+						1
+					);
+					nextDataB = _mm256_inserti128_si256(
+						_mm256_castsi128_si256(_mm256_extracti128_si256(oDataB, 1)),
+						_mm_load_si128((__m128i*)(src+i+sizeof(__m256i)*2)),
+						1
+					);
+				}
 # define SHIFT_DATA_A(offs) (searchEnd ? _mm256_alignr_epi8(nextDataA, oDataA, offs) : _mm256_loadu_si256((__m256i *)(src+i+offs)))
 # define SHIFT_DATA_B(offs) (searchEnd ? _mm256_alignr_epi8(nextDataB, oDataB, offs) : _mm256_loadu_si256((__m256i *)(src+i+offs) + 1))
 #else
 # define SHIFT_DATA_A(offs) _mm256_loadu_si256((__m256i *)(src+i+offs))
 # define SHIFT_DATA_B(offs) _mm256_loadu_si256((__m256i *)(src+i+offs) + 1)
 #endif
-                __m256i tmpData2A = SHIFT_DATA_A(2);
-                __m256i tmpData2B = SHIFT_DATA_B(2);
-                __m256i match2EqA, match2EqB;
-#if defined(__AVX512VL__) && defined(__AVX512BW__)
-                __mmask32 match2EqMaskA, match2EqMaskB;
-                __mmask32 match0CrMaskA, match0CrMaskB;
-                __mmask32 match2CrXDtMaskA, match2CrXDtMaskB;
-                if(useAVX3MaskCmp && searchEnd) {
-                    match2EqMaskA = _mm256_cmpeq_epi8_mask(_mm256_set1_epi8('='), tmpData2A);
-                    match2EqMaskB = _mm256_cmpeq_epi8_mask(_mm256_set1_epi8('='), tmpData2B);
-                } else
-#endif
-                if(searchEnd) {
-                    match2EqA = _mm256_cmpeq_epi8(_mm256_set1_epi8('='), tmpData2A);
-                    match2EqB = _mm256_cmpeq_epi8(_mm256_set1_epi8('='), tmpData2B);
-                }
-
-                int partialKillDotFound;
-                __m256i match2CrXDtA, match2CrXDtB;
-                if(isRaw) {
-                    // find patterns of \r_.
-
-#if defined(__AVX512VL__) && defined(__AVX512BW__)
-                    if(useAVX3MaskCmp) {
-                        match0CrMaskA = _mm256_cmpeq_epi8_mask(oDataA, _mm256_set1_epi8('\r'));
-                        match0CrMaskB = _mm256_cmpeq_epi8_mask(oDataB, _mm256_set1_epi8('\r'));
-                        match2CrXDtMaskA = _mm256_mask_cmpeq_epi8_mask(match0CrMaskA, tmpData2A, _mm256_set1_epi8('.'));
-                        match2CrXDtMaskB = _mm256_mask_cmpeq_epi8_mask(match0CrMaskB, tmpData2B, _mm256_set1_epi8('.'));
-                        partialKillDotFound = KORTEST32(match2CrXDtMaskA, match2CrXDtMaskB);
-                    } else
-#endif
-                    {
-                        match2CrXDtA = _mm256_and_si256(
-                            _mm256_cmpeq_epi8(oDataA, _mm256_set1_epi8('\r')),
-                            _mm256_cmpeq_epi8(tmpData2A, _mm256_set1_epi8('.'))
-                        );
-                        match2CrXDtB = _mm256_and_si256(
-                            _mm256_cmpeq_epi8(oDataB, _mm256_set1_epi8('\r')),
-                            _mm256_cmpeq_epi8(tmpData2B, _mm256_set1_epi8('.'))
-                        );
-                        partialKillDotFound = _mm256_movemask_epi8(_mm256_or_si256(
-                            match2CrXDtA, match2CrXDtB
-                        ));
-                    }
-                }
-
-                if(isRaw && LIKELIHOOD(0.002, partialKillDotFound)) {
-                    // merge matches for \r\n.
-                    __m256i match2NlDotA, match1NlA;
-                    __m256i match2NlDotB, match1NlB;
-#if defined(__AVX512VL__) && defined(__AVX512BW__)
-                    __mmask32 match1NlMaskA, match1NlMaskB;
-                    __mmask32 match2NlDotMaskA, match2NlDotMaskB;
-                    if(useAVX3MaskCmp) {
-                        match1NlMaskA = _mm256_mask_cmpeq_epi8_mask(
-                            match0CrMaskA,
-                            _mm256_set1_epi8('\n'),
-                            SHIFT_DATA_A(1)
-                        );
-                        match1NlMaskB = _mm256_mask_cmpeq_epi8_mask(
-                            match0CrMaskB,
-                            _mm256_set1_epi8('\n'),
-                            SHIFT_DATA_B(1)
-                        );
-                        match2NlDotMaskA = KAND32(match2CrXDtMaskA, match1NlMaskA);
-                        match2NlDotMaskB = KAND32(match2CrXDtMaskB, match1NlMaskB);
-                    } else
-#endif
-                    {
-                        __m256i match1LfA = _mm256_cmpeq_epi8(
-                            _mm256_set1_epi8('\n'),
-                            SHIFT_DATA_A(1)
-                        );
-                        __m256i match1LfB = _mm256_cmpeq_epi8(
-                            _mm256_set1_epi8('\n'),
-                            SHIFT_DATA_B(1)
-                        );
-                        // force re-computing these to avoid register spills elsewhere
-                        match1NlA = _mm256_and_si256(match1LfA, _mm256_cmpeq_epi8(force_align_read_256(src+i), _mm256_set1_epi8('\r')));
-                        match1NlB = _mm256_and_si256(match1LfB, _mm256_cmpeq_epi8(force_align_read_256(src+i + sizeof(__m256i)), _mm256_set1_epi8('\r')));
-                        match2NlDotA = _mm256_and_si256(match2CrXDtA, match1NlA);
-                        match2NlDotB = _mm256_and_si256(match2CrXDtB, match1NlB);
-                    }
-                    if(searchEnd) {
-                        __m256i tmpData4A;
+				__m256i tmpData2A = SHIFT_DATA_A(2);
+				__m256i tmpData2B = SHIFT_DATA_B(2);
+				__m256i match2EqA, match2EqB;
+#if defined(__AVX512VL__) && defined(__AVX512BW__)
+				__mmask32 match2EqMaskA, match2EqMaskB;
+				__mmask32 match0CrMaskA, match0CrMaskB;
+				__mmask32 match2CrXDtMaskA, match2CrXDtMaskB;
+				if(useAVX3MaskCmp && searchEnd) {
+					match2EqMaskA = _mm256_cmpeq_epi8_mask(_mm256_set1_epi8('='), tmpData2A);
+					match2EqMaskB = _mm256_cmpeq_epi8_mask(_mm256_set1_epi8('='), tmpData2B);
+				} else
+#endif
+				if(searchEnd) {
+					match2EqA = _mm256_cmpeq_epi8(_mm256_set1_epi8('='), tmpData2A);
+					match2EqB = _mm256_cmpeq_epi8(_mm256_set1_epi8('='), tmpData2B);
+				}
+				
+				int partialKillDotFound;
+				__m256i match2CrXDtA, match2CrXDtB;
+				if(isRaw) {
+					// find patterns of \r_.
+					
+#if defined(__AVX512VL__) && defined(__AVX512BW__)
+					if(useAVX3MaskCmp) {
+						match0CrMaskA = _mm256_cmpeq_epi8_mask(oDataA, _mm256_set1_epi8('\r'));
+						match0CrMaskB = _mm256_cmpeq_epi8_mask(oDataB, _mm256_set1_epi8('\r'));
+						match2CrXDtMaskA = _mm256_mask_cmpeq_epi8_mask(match0CrMaskA, tmpData2A, _mm256_set1_epi8('.'));
+						match2CrXDtMaskB = _mm256_mask_cmpeq_epi8_mask(match0CrMaskB, tmpData2B, _mm256_set1_epi8('.'));
+						partialKillDotFound = KORTEST32(match2CrXDtMaskA, match2CrXDtMaskB);
+					} else
+#endif
+					{
+						match2CrXDtA = _mm256_and_si256(
+							_mm256_cmpeq_epi8(oDataA, _mm256_set1_epi8('\r')),
+							_mm256_cmpeq_epi8(tmpData2A, _mm256_set1_epi8('.'))
+						);
+						match2CrXDtB = _mm256_and_si256(
+							_mm256_cmpeq_epi8(oDataB, _mm256_set1_epi8('\r')),
+							_mm256_cmpeq_epi8(tmpData2B, _mm256_set1_epi8('.'))
+						);
+						partialKillDotFound = _mm256_movemask_epi8(_mm256_or_si256(
+							match2CrXDtA, match2CrXDtB
+						));
+					}
+				}
+				
+				if(isRaw && LIKELIHOOD(0.002, partialKillDotFound)) {
+					// merge matches for \r\n.
+					__m256i match2NlDotA, match1NlA;
+					__m256i match2NlDotB, match1NlB;
+#if defined(__AVX512VL__) && defined(__AVX512BW__)
+					__mmask32 match1NlMaskA, match1NlMaskB;
+					__mmask32 match2NlDotMaskA, match2NlDotMaskB;
+					if(useAVX3MaskCmp) {
+						match1NlMaskA = _mm256_mask_cmpeq_epi8_mask(
+							match0CrMaskA,
+							_mm256_set1_epi8('\n'),
+							SHIFT_DATA_A(1)
+						);
+						match1NlMaskB = _mm256_mask_cmpeq_epi8_mask(
+							match0CrMaskB,
+							_mm256_set1_epi8('\n'),
+							SHIFT_DATA_B(1)
+						);
+						match2NlDotMaskA = KAND32(match2CrXDtMaskA, match1NlMaskA);
+						match2NlDotMaskB = KAND32(match2CrXDtMaskB, match1NlMaskB);
+					} else
+#endif
+					{
+						__m256i match1LfA = _mm256_cmpeq_epi8(
+							_mm256_set1_epi8('\n'),
+							SHIFT_DATA_A(1)
+						);
+						__m256i match1LfB = _mm256_cmpeq_epi8(
+							_mm256_set1_epi8('\n'),
+							SHIFT_DATA_B(1)
+						);
+						// force re-computing these to avoid register spills elsewhere
+						match1NlA = _mm256_and_si256(match1LfA, _mm256_cmpeq_epi8(force_align_read_256(src+i), _mm256_set1_epi8('\r')));
+						match1NlB = _mm256_and_si256(match1LfB, _mm256_cmpeq_epi8(force_align_read_256(src+i + sizeof(__m256i)), _mm256_set1_epi8('\r')));
+						match2NlDotA = _mm256_and_si256(match2CrXDtA, match1NlA);
+						match2NlDotB = _mm256_and_si256(match2CrXDtB, match1NlB);
+					}
+					if(searchEnd) {
+						__m256i tmpData4A;
 #if defined(__AVX512VL__) && defined(PLATFORM_AMD64)
-                        if(use_isa >= ISA_LEVEL_AVX3)
-                            // AVX512 with 32 registers shouldn't have any issue with holding onto oData* in registers
-                            tmpData4A = _mm256_alignr_epi32(oDataB, oDataA, 1);
-                        else
-#endif
-                            tmpData4A = SHIFT_DATA_A(4);
-                        __m256i tmpData4B = SHIFT_DATA_B(4);
-                        // match instances of \r\n.\r\n and \r\n.=y
-                        __m256i match3CrA = _mm256_cmpeq_epi8(
-                            _mm256_set1_epi8('\r'),
-                            SHIFT_DATA_A(3)
-                        );
-                        __m256i match3CrB = _mm256_cmpeq_epi8(
-                            _mm256_set1_epi8('\r'),
-                            SHIFT_DATA_B(3)
-                        );
-                        __m256i match4LfA = _mm256_cmpeq_epi8(tmpData4A, _mm256_set1_epi8('\n'));
-                        __m256i match4LfB = _mm256_cmpeq_epi8(tmpData4B, _mm256_set1_epi8('\n'));
-                        __m256i match4EqYA = _mm256_cmpeq_epi16(tmpData4A, _mm256_set1_epi16(0x793d)); // =y
-                        __m256i match4EqYB = _mm256_cmpeq_epi16(tmpData4B, _mm256_set1_epi16(0x793d)); // =y
-
-                        int matchEnd;
-#if defined(__AVX512VL__) && defined(__AVX512BW__)
-                        if(useAVX3MaskCmp) {
-                            __mmask32 match3EqYMaskA = _mm256_mask_cmpeq_epi8_mask(
-                                match2EqMaskA,
-                                _mm256_set1_epi8('y'),
-                                SHIFT_DATA_A(3)
-                            );
-                            __mmask32 match3EqYMaskB = _mm256_mask_cmpeq_epi8_mask(
-                                match2EqMaskB,
-                                _mm256_set1_epi8('y'),
-                                SHIFT_DATA_B(3)
-                            );
-                            __m256i match34EqYA, match34EqYB;
+						if(use_isa >= ISA_LEVEL_AVX3)
+							// AVX512 with 32 registers shouldn't have any issue with holding onto oData* in registers
+							tmpData4A = _mm256_alignr_epi32(oDataB, oDataA, 1);
+						else
+#endif
+							tmpData4A = SHIFT_DATA_A(4);
+						__m256i tmpData4B = SHIFT_DATA_B(4);
+						// match instances of \r\n.\r\n and \r\n.=y
+						__m256i match3CrA = _mm256_cmpeq_epi8(
+							_mm256_set1_epi8('\r'),
+							SHIFT_DATA_A(3)
+						);
+						__m256i match3CrB = _mm256_cmpeq_epi8(
+							_mm256_set1_epi8('\r'),
+							SHIFT_DATA_B(3)
+						);
+						__m256i match4LfA = _mm256_cmpeq_epi8(tmpData4A, _mm256_set1_epi8('\n'));
+						__m256i match4LfB = _mm256_cmpeq_epi8(tmpData4B, _mm256_set1_epi8('\n'));
+						__m256i match4EqYA = _mm256_cmpeq_epi16(tmpData4A, _mm256_set1_epi16(0x793d)); // =y
+						__m256i match4EqYB = _mm256_cmpeq_epi16(tmpData4B, _mm256_set1_epi16(0x793d)); // =y
+						
+						int matchEnd;
+#if defined(__AVX512VL__) && defined(__AVX512BW__)
+						if(useAVX3MaskCmp) {
+							__mmask32 match3EqYMaskA = _mm256_mask_cmpeq_epi8_mask(
+								match2EqMaskA,
+								_mm256_set1_epi8('y'),
+								SHIFT_DATA_A(3)
+							);
+							__mmask32 match3EqYMaskB = _mm256_mask_cmpeq_epi8_mask(
+								match2EqMaskB,
+								_mm256_set1_epi8('y'),
+								SHIFT_DATA_B(3)
+							);
+							__m256i match34EqYA, match34EqYB;
 # ifdef __AVX512VBMI2__
-                            if(use_isa >= ISA_LEVEL_VBMI2) {
-                                match34EqYA = _mm256_shrdi_epi16(_mm256_movm_epi8(match3EqYMaskA), match4EqYA, 8);
-                                match34EqYB = _mm256_shrdi_epi16(_mm256_movm_epi8(match3EqYMaskB), match4EqYB, 8);
-                            } else
+							if(use_isa >= ISA_LEVEL_VBMI2) {
+								match34EqYA = _mm256_shrdi_epi16(_mm256_movm_epi8(match3EqYMaskA), match4EqYA, 8);
+								match34EqYB = _mm256_shrdi_epi16(_mm256_movm_epi8(match3EqYMaskB), match4EqYB, 8);
+							} else
 # endif
-                            {
-                                // (match4EqY & 0xff00) | (match3EqY >> 8)
-                                match34EqYA = _mm256_mask_blend_epi8(match3EqYMaskA>>1, _mm256_and_si256(match4EqYA, _mm256_set1_epi16(-0xff)), _mm256_set1_epi8(-1));
-                                match34EqYB = _mm256_mask_blend_epi8(match3EqYMaskB>>1, _mm256_and_si256(match4EqYB, _mm256_set1_epi16(-0xff)), _mm256_set1_epi8(-1));
-                            }
-                            // merge \r\n and =y matches for tmpData4
-                            __m256i match4EndA = _mm256_ternarylogic_epi32(match34EqYA, match3CrA, match4LfA, 0xF8); // (match3Cr & match4Lf) | match34EqY
-                            __m256i match4EndB = _mm256_ternarylogic_epi32(match34EqYB, match3CrB, match4LfB, 0xF8);
-                            // merge with \r\n. and combine
-                            matchEnd = KORTEST32(
-                                KOR32(
-                                    _mm256_mask_test_epi8_mask(match2NlDotMaskA, match4EndA, match4EndA),
-                                    KAND32(match3EqYMaskA, match1NlMaskA)
-                                ),
-                                KOR32(
-                                    _mm256_mask_test_epi8_mask(match2NlDotMaskB, match4EndB, match4EndB),
-                                    KAND32(match3EqYMaskB, match1NlMaskB)
-                                )
-                            );
-                        } else
-#endif
-                        {
-                            __m256i match3EqYA = _mm256_and_si256(match2EqA, _mm256_cmpeq_epi8(
-                                _mm256_set1_epi8('y'),
-                                SHIFT_DATA_A(3)
-                            ));
-                            __m256i match3EqYB = _mm256_and_si256(match2EqB, _mm256_cmpeq_epi8(
-                                _mm256_set1_epi8('y'),
-                                SHIFT_DATA_B(3)
-                            ));
-                            match4EqYA = _mm256_slli_epi16(match4EqYA, 8); // TODO: also consider using PBLENDVB here with shifted match3EqY instead
-                            match4EqYB = _mm256_slli_epi16(match4EqYB, 8);
-                            // merge \r\n and =y matches for tmpData4
-                            __m256i match4EndA = _mm256_or_si256(
-                                _mm256_and_si256(match3CrA, match4LfA),
-                                _mm256_or_si256(match4EqYA, _mm256_srli_epi16(match3EqYA, 8)) // _mm256_srli_si256 by 1 also works
-                            );
-                            __m256i match4EndB = _mm256_or_si256(
-                                _mm256_and_si256(match3CrB, match4LfB),
-                                _mm256_or_si256(match4EqYB, _mm256_srli_epi16(match3EqYB, 8))
-                            );
-                            // merge with \r\n.
-                            match4EndA = _mm256_and_si256(match4EndA, match2NlDotA);
-                            match4EndB = _mm256_and_si256(match4EndB, match2NlDotB);
-                            // match \r\n=y
-                            __m256i match3EndA = _mm256_and_si256(match3EqYA, match1NlA);
-                            __m256i match3EndB = _mm256_and_si256(match3EqYB, match1NlB);
-                            // combine match sequences
-                            matchEnd = _mm256_movemask_epi8(_mm256_or_si256(
-                                _mm256_or_si256(match4EndA, match3EndA),
-                                _mm256_or_si256(match4EndB, match3EndB)
-                            ));
-                        }
-                        if(LIKELIHOOD(0.002, matchEnd)) {
-                            // terminator found
-                            // there's probably faster ways to do this, but reverting to scalar code should be good enough
-                            len += (long)i;
-                            break;
-                        }
-                    }
-#if defined(__AVX512VL__) && defined(__AVX512BW__)
-                    if(useAVX3MaskCmp) {
-                        mask |= (uint64_t)match2NlDotMaskA << 2;
-                        mask |= (uint64_t)match2NlDotMaskB << 34;
-                        minMask = _mm256_maskz_mov_epi8(~(match2NlDotMaskB>>30), _mm256_set1_epi8('.'));
-                    } else
-#endif
-                    {
-                        mask |= (uint64_t)((uint32_t)_mm256_movemask_epi8(match2NlDotA)) << 2;
-                        mask |= (uint64_t)((uint32_t)_mm256_movemask_epi8(match2NlDotB)) << 34;
-                        match2NlDotB = zext128_256(_mm_srli_si128(_mm256_extracti128_si256(match2NlDotB, 1), 14));
-                        minMask = _mm256_subs_epu8(_mm256_set1_epi8('.'), match2NlDotB);
-                    }
-                }
-                else if(searchEnd) {
-                    bool partialEndFound;
-                    __m256i match3EqYA, match3EqYB;
-#if defined(__AVX512VL__) && defined(__AVX512BW__)
-                    __mmask32 match3EqYMaskA, match3EqYMaskB;
-                    if(useAVX3MaskCmp) {
-                        match3EqYMaskA = _mm256_mask_cmpeq_epi8_mask(
-                            match2EqMaskA,
-                            _mm256_set1_epi8('y'),
-                            SHIFT_DATA_A(3)
-                        );
-                        match3EqYMaskB = _mm256_mask_cmpeq_epi8_mask(
-                            match2EqMaskB,
-                            _mm256_set1_epi8('y'),
-                            SHIFT_DATA_B(3)
-                        );
-                        partialEndFound = KORTEST32(match3EqYMaskA, match3EqYMaskB);
-                    } else
-#endif
-                    {
-                        __m256i match3YA = _mm256_cmpeq_epi8(
-                            _mm256_set1_epi8('y'),
-                            SHIFT_DATA_A(3)
-                        );
-                        __m256i match3YB = _mm256_cmpeq_epi8(
-                            _mm256_set1_epi8('y'),
-                            SHIFT_DATA_B(3)
-                        );
-                        match3EqYA = _mm256_and_si256(match2EqA, match3YA);
-                        match3EqYB = _mm256_and_si256(match2EqB, match3YB);
-                        partialEndFound = _mm256_movemask_epi8(_mm256_or_si256(match3EqYA, match3EqYB));
-                    }
-                    if(LIKELIHOOD(0.002, partialEndFound)) {
-                        bool endFound;
-#if defined(__AVX512VL__) && defined(__AVX512BW__)
-                        if(useAVX3MaskCmp) {
-                            __mmask32 match3LfEqYMaskA = _mm256_mask_cmpeq_epi8_mask(
-                                match3EqYMaskA,
-                                _mm256_set1_epi8('\n'),
-                                SHIFT_DATA_A(1)
-                            );
-                            __mmask32 match3LfEqYMaskB = _mm256_mask_cmpeq_epi8_mask(
-                                match3EqYMaskB,
-                                _mm256_set1_epi8('\n'),
-                                SHIFT_DATA_B(1)
-                            );
-
-                            endFound = KORTEST32(
-                                _mm256_mask_cmpeq_epi8_mask(match3LfEqYMaskA, oDataA, _mm256_set1_epi8('\r')),
-                                _mm256_mask_cmpeq_epi8_mask(match3LfEqYMaskB, oDataB, _mm256_set1_epi8('\r'))
-                            );
-                        } else
-#endif
-                        {
-                            __m256i match1LfA = _mm256_cmpeq_epi8(
-                                _mm256_set1_epi8('\n'),
-                                SHIFT_DATA_A(1)
-                            );
-                            __m256i match1LfB = _mm256_cmpeq_epi8(
-                                _mm256_set1_epi8('\n'),
-                                SHIFT_DATA_B(1)
-                            );
-                            endFound = _mm256_movemask_epi8(_mm256_or_si256(
-                                _mm256_and_si256(
-                                    match3EqYA,
-                                    _mm256_and_si256(match1LfA, _mm256_cmpeq_epi8(force_align_read_256(src+i), _mm256_set1_epi8('\r')))
-                                ),
-                                _mm256_and_si256(
-                                    match3EqYB,
-                                    _mm256_and_si256(match1LfB, _mm256_cmpeq_epi8(force_align_read_256(src+i + sizeof(__m256i)), _mm256_set1_epi8('\r')))
-                                )
-                            ));
-                        }
-                        if(endFound) {
-                            len += (long)i;
-                            break;
-                        }
-                    }
-                    if(isRaw) minMask = _mm256_set1_epi8('.');
-                }
-                else if(isRaw) // no \r_. found
-                    minMask = _mm256_set1_epi8('.');
-            }
+							{
+								// (match4EqY & 0xff00) | (match3EqY >> 8)
+								match34EqYA = _mm256_mask_blend_epi8(match3EqYMaskA>>1, _mm256_and_si256(match4EqYA, _mm256_set1_epi16(-0xff)), _mm256_set1_epi8(-1));
+								match34EqYB = _mm256_mask_blend_epi8(match3EqYMaskB>>1, _mm256_and_si256(match4EqYB, _mm256_set1_epi16(-0xff)), _mm256_set1_epi8(-1));
+							}
+							// merge \r\n and =y matches for tmpData4
+							__m256i match4EndA = _mm256_ternarylogic_epi32(match34EqYA, match3CrA, match4LfA, 0xF8); // (match3Cr & match4Lf) | match34EqY
+							__m256i match4EndB = _mm256_ternarylogic_epi32(match34EqYB, match3CrB, match4LfB, 0xF8);
+							// merge with \r\n. and combine
+							matchEnd = KORTEST32(
+								KOR32(
+									_mm256_mask_test_epi8_mask(match2NlDotMaskA, match4EndA, match4EndA),
+									KAND32(match3EqYMaskA, match1NlMaskA)
+								),
+								KOR32(
+									_mm256_mask_test_epi8_mask(match2NlDotMaskB, match4EndB, match4EndB),
+									KAND32(match3EqYMaskB, match1NlMaskB)
+								)
+							);
+						} else
+#endif
+						{
+							__m256i match3EqYA = _mm256_and_si256(match2EqA, _mm256_cmpeq_epi8(
+								_mm256_set1_epi8('y'),
+								SHIFT_DATA_A(3)
+							));
+							__m256i match3EqYB = _mm256_and_si256(match2EqB, _mm256_cmpeq_epi8(
+								_mm256_set1_epi8('y'),
+								SHIFT_DATA_B(3)
+							));
+							match4EqYA = _mm256_slli_epi16(match4EqYA, 8); // TODO: also consider using PBLENDVB here with shifted match3EqY instead
+							match4EqYB = _mm256_slli_epi16(match4EqYB, 8);
+							// merge \r\n and =y matches for tmpData4
+							__m256i match4EndA = _mm256_or_si256(
+								_mm256_and_si256(match3CrA, match4LfA),
+								_mm256_or_si256(match4EqYA, _mm256_srli_epi16(match3EqYA, 8)) // _mm256_srli_si256 by 1 also works
+							);
+							__m256i match4EndB = _mm256_or_si256(
+								_mm256_and_si256(match3CrB, match4LfB),
+								_mm256_or_si256(match4EqYB, _mm256_srli_epi16(match3EqYB, 8))
+							);
+							// merge with \r\n.
+							match4EndA = _mm256_and_si256(match4EndA, match2NlDotA);
+							match4EndB = _mm256_and_si256(match4EndB, match2NlDotB);
+							// match \r\n=y
+							__m256i match3EndA = _mm256_and_si256(match3EqYA, match1NlA);
+							__m256i match3EndB = _mm256_and_si256(match3EqYB, match1NlB);
+							// combine match sequences
+							matchEnd = _mm256_movemask_epi8(_mm256_or_si256(
+								_mm256_or_si256(match4EndA, match3EndA),
+								_mm256_or_si256(match4EndB, match3EndB)
+							));
+						}
+						if(LIKELIHOOD(0.002, matchEnd)) {
+							// terminator found
+							// there's probably faster ways to do this, but reverting to scalar code should be good enough
+							len += (long)i;
+							_nextMask = decoder_set_nextMask<isRaw>(src+i, mask);
+							break;
+						}
+					}
+#if defined(__AVX512VL__) && defined(__AVX512BW__)
+					if(useAVX3MaskCmp) {
+						mask |= (uint64_t)match2NlDotMaskA << 2;
+						mask |= (uint64_t)match2NlDotMaskB << 34;
+						minMask = _mm256_maskz_mov_epi8(~(match2NlDotMaskB>>30), _mm256_set1_epi8('.'));
+					} else
+#endif
+					{
+						mask |= (uint64_t)((uint32_t)_mm256_movemask_epi8(match2NlDotA)) << 2;
+						mask |= (uint64_t)((uint32_t)_mm256_movemask_epi8(match2NlDotB)) << 34;
+						match2NlDotB = zext128_256(_mm_srli_si128(_mm256_extracti128_si256(match2NlDotB, 1), 14));
+						minMask = _mm256_subs_epu8(_mm256_set1_epi8('.'), match2NlDotB);
+					}
+				}
+				else if(searchEnd) {
+					bool partialEndFound;
+					__m256i match3EqYA, match3EqYB;
+#if defined(__AVX512VL__) && defined(__AVX512BW__)
+					__mmask32 match3EqYMaskA, match3EqYMaskB;
+					if(useAVX3MaskCmp) {
+						match3EqYMaskA = _mm256_mask_cmpeq_epi8_mask(
+							match2EqMaskA,
+							_mm256_set1_epi8('y'),
+							SHIFT_DATA_A(3)
+						);
+						match3EqYMaskB = _mm256_mask_cmpeq_epi8_mask(
+							match2EqMaskB,
+							_mm256_set1_epi8('y'),
+							SHIFT_DATA_B(3)
+						);
+						partialEndFound = KORTEST32(match3EqYMaskA, match3EqYMaskB);
+					} else
+#endif
+					{
+						__m256i match3YA = _mm256_cmpeq_epi8(
+							_mm256_set1_epi8('y'),
+							SHIFT_DATA_A(3)
+						);
+						__m256i match3YB = _mm256_cmpeq_epi8(
+							_mm256_set1_epi8('y'),
+							SHIFT_DATA_B(3)
+						);
+						match3EqYA = _mm256_and_si256(match2EqA, match3YA);
+						match3EqYB = _mm256_and_si256(match2EqB, match3YB);
+						partialEndFound = _mm256_movemask_epi8(_mm256_or_si256(match3EqYA, match3EqYB));
+					}
+					if(LIKELIHOOD(0.002, partialEndFound)) {
+						bool endFound;
+#if defined(__AVX512VL__) && defined(__AVX512BW__)
+						if(useAVX3MaskCmp) {
+							__mmask32 match3LfEqYMaskA = _mm256_mask_cmpeq_epi8_mask(
+								match3EqYMaskA,
+								_mm256_set1_epi8('\n'),
+								SHIFT_DATA_A(1)
+							);
+							__mmask32 match3LfEqYMaskB = _mm256_mask_cmpeq_epi8_mask(
+								match3EqYMaskB,
+								_mm256_set1_epi8('\n'),
+								SHIFT_DATA_B(1)
+							);
+							
+							endFound = KORTEST32(
+								_mm256_mask_cmpeq_epi8_mask(match3LfEqYMaskA, oDataA, _mm256_set1_epi8('\r')),
+								_mm256_mask_cmpeq_epi8_mask(match3LfEqYMaskB, oDataB, _mm256_set1_epi8('\r'))
+							);
+						} else
+#endif
+						{
+							__m256i match1LfA = _mm256_cmpeq_epi8(
+								_mm256_set1_epi8('\n'),
+								SHIFT_DATA_A(1)
+							);
+							__m256i match1LfB = _mm256_cmpeq_epi8(
+								_mm256_set1_epi8('\n'),
+								SHIFT_DATA_B(1)
+							);
+							endFound = _mm256_movemask_epi8(_mm256_or_si256(
+								_mm256_and_si256(
+									match3EqYA,
+									_mm256_and_si256(match1LfA, _mm256_cmpeq_epi8(force_align_read_256(src+i), _mm256_set1_epi8('\r')))
+								),
+								_mm256_and_si256(
+									match3EqYB,
+									_mm256_and_si256(match1LfB, _mm256_cmpeq_epi8(force_align_read_256(src+i + sizeof(__m256i)), _mm256_set1_epi8('\r')))
+								)
+							));
+						}
+						if(endFound) {
+							len += (long)i;
+							_nextMask = decoder_set_nextMask<isRaw>(src+i, mask);
+							break;
+						}
+					}
+					if(isRaw) minMask = _mm256_set1_epi8('.');
+				}
+				else if(isRaw) // no \r_. found
+					minMask = _mm256_set1_epi8('.');
+			}
 #undef SHIFT_DATA_A
 #undef SHIFT_DATA_B
-
-            if(use_isa >= ISA_LEVEL_AVX3)
-                dataB = _mm256_add_epi8(oDataB, _mm256_set1_epi8(-42));
-
-            if(LIKELIHOOD(0.0001, (mask & ((maskEq << 1) + escFirst)) != 0)) {
-                unsigned tmp = lookups->eqFix[(maskEq&0xff) & ~(uint64_t)escFirst];
-                uint64_t maskEq2 = tmp;
-                for(int j=8; j<64; j+=8) {
-                    tmp = lookups->eqFix[(unsigned)((maskEq>>j)&0xff) & ~(tmp>>7)];
-                    maskEq2 |= (uint64_t)tmp<<j;
-                }
-                maskEq = maskEq2;
-
-                mask &= ~(uint64_t)escFirst;
-                escFirst = tmp>>7;
-                // next, eliminate anything following a `=` from the special char mask; this eliminates cases of `=\r` so that they aren't removed
-                maskEq <<= 1;
-                mask &= ~maskEq;
-
-                // unescape chars following `=`
-#if defined(__AVX512VL__) && defined(__AVX512BW__)
-                if(use_isa >= ISA_LEVEL_AVX3) {
-                    // GCC < 7 seems to generate rubbish assembly for this
-                    dataA = _mm256_mask_add_epi8(
-                        dataA,
-                        (__mmask32)maskEq,
-                        dataA,
-                        _mm256_set1_epi8(-64)
-                    );
-                    dataB = _mm256_mask_add_epi8(
-                        dataB,
-                        (__mmask32)(maskEq>>32),
-                        dataB,
-                        _mm256_set1_epi8(-64)
-                    );
-                } else
+			
+			if(use_isa >= ISA_LEVEL_AVX3)
+				dataB = _mm256_add_epi8(oDataB, _mm256_set1_epi8(-42));
+			
+			uint64_t maskEqShift1 = (maskEq << 1) + escFirst;
+			if(LIKELIHOOD(0.0001, (mask & maskEqShift1) != 0)) {
+				maskEq = fix_eqMask<uint64_t>(maskEq, maskEqShift1);
+				mask &= ~(uint64_t)escFirst;
+				escFirst = maskEq>>63;
+				// next, eliminate anything following a `=` from the special char mask; this eliminates cases of `=\r` so that they aren't removed
+				maskEq <<= 1;
+				mask &= ~maskEq;
+				
+				// unescape chars following `=`
+#if defined(__AVX512VL__) && defined(__AVX512BW__)
+				if(use_isa >= ISA_LEVEL_AVX3) {
+					// GCC < 7 seems to generate rubbish assembly for this
+					dataA = _mm256_mask_add_epi8(
+						dataA,
+						(__mmask32)maskEq,
+						dataA,
+						_mm256_set1_epi8(-64)
+					);
+					dataB = _mm256_mask_add_epi8(
+						dataB,
+						(__mmask32)(maskEq>>32),
+						dataB,
+						_mm256_set1_epi8(-64)
+					);
+				} else
 #endif
-                {
-                    // convert maskEq into vector form (i.e. reverse pmovmskb)
+				{
+					// convert maskEq into vector form (i.e. reverse pmovmskb)
 #ifdef PLATFORM_AMD64
-                    __m256i vMaskEq = _mm256_broadcastq_epi64(_mm_cvtsi64_si128(maskEq));
+					__m256i vMaskEq = _mm256_broadcastq_epi64(_mm_cvtsi64_si128(maskEq));
 #else
-                    __m256i vMaskEq = _mm256_permute4x64_epi64(_mm256_insert_epi32(
-                        _mm256_set_epi32(0,0,0,0, 0,0,0, maskEq & 0xffffffff),
-                        maskEq >> 32,
-                        1
-                    ), 0);
-#endif
-                    __m256i vMaskEqA = _mm256_shuffle_epi8(vMaskEq, _mm256_set_epi32(
-                        0x03030303, 0x03030303, 0x02020202, 0x02020202,
-                        0x01010101, 0x01010101, 0x00000000, 0x00000000
-                    ));
-                    __m256i vMaskEqB = _mm256_shuffle_epi8(vMaskEq, _mm256_set_epi32(
-                        0x07070707, 0x07070707, 0x06060606, 0x06060606,
-                        0x05050505, 0x05050505, 0x04040404, 0x04040404
-                    ));
-                    vMaskEqA = _mm256_cmpeq_epi8(
-                        _mm256_and_si256(vMaskEqA, _mm256_set1_epi64x(0x8040201008040201ULL)),
-                        _mm256_set1_epi64x(0x8040201008040201ULL)
-                    );
-                    vMaskEqB = _mm256_cmpeq_epi8(
-                        _mm256_and_si256(vMaskEqB, _mm256_set1_epi64x(0x8040201008040201ULL)),
-                        _mm256_set1_epi64x(0x8040201008040201ULL)
-                    );
-                    dataA = _mm256_add_epi8(oDataA, _mm256_blendv_epi8(yencOffset, _mm256_set1_epi8(-42-64), vMaskEqA));
-                    dataB = _mm256_add_epi8(oDataB, _mm256_blendv_epi8(_mm256_set1_epi8(-42), _mm256_set1_epi8(-42-64), vMaskEqB));
-                }
-            } else {
-                escFirst = (maskEq >> 63);
-
-#if defined(__AVX512VL__) && defined(__AVX512BW__)
-                if(use_isa >= ISA_LEVEL_AVX3) {
-                    dataA = _mm256_mask_add_epi8(
-                        dataA,
-                        (__mmask32)(maskEq << 1),
-                        dataA,
-                        _mm256_set1_epi8(-64)
-                    );
-                    dataB = _mm256_mask_add_epi8(
-                        dataB,
-                        (__mmask32)(maskEq >> 31),
-                        dataB,
-                        _mm256_set1_epi8(-64)
-                    );
-                } else
-#endif
-                {
-                    // << 1 byte
-                    cmpEqA = _mm256_alignr_epi8(cmpEqA, _mm256_inserti128_si256(
-                        _mm256_set1_epi8('='), _mm256_castsi256_si128(cmpEqA), 1
-                    ), 15);
-                    cmpEqB = _mm256_cmpeq_epi8(_mm256_set1_epi8('='), _mm256_loadu_si256((__m256i *)(src+i-1) + 1));
-                    dataA = _mm256_add_epi8(
-                        oDataA,
-                        _mm256_blendv_epi8(
-                            yencOffset,
-                            _mm256_set1_epi8(-42-64),
-                            cmpEqA
-                        )
-                    );
-                    dataB = _mm256_add_epi8(
-                        oDataB,
-                        _mm256_blendv_epi8(
-                            _mm256_set1_epi8(-42),
-                            _mm256_set1_epi8(-42-64),
-                            cmpEqB
-                        )
-                    );
-                }
-            }
-            // subtract 64 from first element if escFirst == 1
-#if defined(__AVX512VL__) && defined(__AVX512BW__)
-            if(use_isa >= ISA_LEVEL_AVX3) {
-                yencOffset = _mm256_mask_add_epi8(_mm256_set1_epi8(-42), (__mmask32)escFirst, _mm256_set1_epi8(-42), _mm256_set1_epi8(-64));
-            } else
-#endif
-            {
-                yencOffset = _mm256_xor_si256(_mm256_set1_epi8(-42), zext128_256(
-                    _mm_slli_epi16(_mm_cvtsi32_si128((int)escFirst), 6)
-                ));
-            }
-
-            // all that's left is to 'compress' the data (skip over masked chars)
+					__m256i vMaskEq = _mm256_permute4x64_epi64(_mm256_insert_epi32(
+						_mm256_set_epi32(0,0,0,0, 0,0,0, maskEq & 0xffffffff),
+						maskEq >> 32,
+						1
+					), 0);
+#endif
+					__m256i vMaskEqA = _mm256_shuffle_epi8(vMaskEq, _mm256_set_epi32(
+						0x03030303, 0x03030303, 0x02020202, 0x02020202,
+						0x01010101, 0x01010101, 0x00000000, 0x00000000
+					));
+					__m256i vMaskEqB = _mm256_shuffle_epi8(vMaskEq, _mm256_set_epi32(
+						0x07070707, 0x07070707, 0x06060606, 0x06060606,
+						0x05050505, 0x05050505, 0x04040404, 0x04040404
+					));
+					vMaskEqA = _mm256_cmpeq_epi8(
+						_mm256_and_si256(vMaskEqA, _mm256_set1_epi64x(0x8040201008040201ULL)),
+						_mm256_set1_epi64x(0x8040201008040201ULL)
+					);
+					vMaskEqB = _mm256_cmpeq_epi8(
+						_mm256_and_si256(vMaskEqB, _mm256_set1_epi64x(0x8040201008040201ULL)),
+						_mm256_set1_epi64x(0x8040201008040201ULL)
+					);
+					dataA = _mm256_add_epi8(oDataA, _mm256_blendv_epi8(yencOffset, _mm256_set1_epi8(-42-64), vMaskEqA));
+					dataB = _mm256_add_epi8(oDataB, _mm256_blendv_epi8(_mm256_set1_epi8(-42), _mm256_set1_epi8(-42-64), vMaskEqB));
+				}
+			} else {
+				escFirst = (maskEq >> 63);
+				
+#if defined(__AVX512VL__) && defined(__AVX512BW__)
+				if(use_isa >= ISA_LEVEL_AVX3) {
+					dataA = _mm256_mask_add_epi8(
+						dataA,
+						(__mmask32)(maskEq << 1),
+						dataA,
+						_mm256_set1_epi8(-64)
+					);
+					dataB = _mm256_mask_add_epi8(
+						dataB,
+						(__mmask32)(maskEq >> 31),
+						dataB,
+						_mm256_set1_epi8(-64)
+					);
+				} else
+#endif
+				{
+					// << 1 byte
+					cmpEqA = _mm256_alignr_epi8(cmpEqA, _mm256_inserti128_si256(
+						_mm256_set1_epi8('='), _mm256_castsi256_si128(cmpEqA), 1
+					), 15);
+					cmpEqB = _mm256_cmpeq_epi8(_mm256_set1_epi8('='), _mm256_loadu_si256((__m256i *)(src+i-1) + 1));
+					dataA = _mm256_add_epi8(
+						oDataA,
+						_mm256_blendv_epi8(
+							yencOffset,
+							_mm256_set1_epi8(-42-64),
+							cmpEqA
+						)
+					);
+					dataB = _mm256_add_epi8(
+						oDataB,
+						_mm256_blendv_epi8(
+							_mm256_set1_epi8(-42),
+							_mm256_set1_epi8(-42-64),
+							cmpEqB
+						)
+					);
+				}
+			}
+			// subtract 64 from first element if escFirst == 1
+#if defined(__AVX512VL__) && defined(__AVX512BW__)
+			if(use_isa >= ISA_LEVEL_AVX3) {
+				yencOffset = _mm256_mask_add_epi8(_mm256_set1_epi8(-42), (__mmask32)escFirst, _mm256_set1_epi8(-42), _mm256_set1_epi8(-64));
+			} else
+#endif
+			{
+				yencOffset = _mm256_xor_si256(_mm256_set1_epi8(-42), zext128_256(
+					_mm_slli_epi16(_mm_cvtsi32_si128((int)escFirst), 6)
+				));
+			}
+			
+			// all that's left is to 'compress' the data (skip over masked chars)
 #if defined(__AVX512VBMI2__) && defined(__AVX512VL__)
-            if(use_isa >= ISA_LEVEL_VBMI2) {
-                _mm256_mask_compressstoreu_epi8(p, KNOT32(mask), dataA);
-                p -= popcnt32(mask & 0xffffffff);
-                _mm256_mask_compressstoreu_epi8((p + XMM_SIZE*2), KNOT32(mask>>32), dataB);
-                p += XMM_SIZE*4 - popcnt32(mask >> 32);
-            } else
-#endif
-            {
-                // lookup compress masks and shuffle
-                __m256i shuf = _mm256_inserti128_si256(
-                    _mm256_castsi128_si256(_mm_load_si128((__m128i*)(lookups->compact + (mask & 0x7fff)))),
-                    *(__m128i*)((char*)lookups->compact + ((mask >> 12) & 0x7fff0)),
-                    1
-                );
-                dataA = _mm256_shuffle_epi8(dataA, shuf);
-
-                _mm_storeu_si128((__m128i*)p, _mm256_castsi256_si128(dataA));
-                // increment output position
-                p -= popcnt32(mask & 0xffff);
-
-                _mm_storeu_si128((__m128i*)(p + XMM_SIZE), _mm256_extracti128_si256(dataA, 1));
-                p -= popcnt32(mask & 0xffff0000);
-
+			if(use_isa >= ISA_LEVEL_VBMI2) {
+				COMPRESS_STORE(p, KNOT32(mask), dataA);
+				p -= popcnt32(mask & 0xffffffff);
+				COMPRESS_STORE((p + XMM_SIZE*2), KNOT32(mask>>32), dataB);
+				p += XMM_SIZE*4 - popcnt32(mask >> 32);
+			} else
+#endif
+			{
+				// lookup compress masks and shuffle
+				__m256i shuf = _mm256_inserti128_si256(
+					_mm256_castsi128_si256(_mm_load_si128((__m128i*)(lookups->compact + (mask & 0x7fff)))),
+					*(__m128i*)((char*)lookups->compact + ((mask >> 12) & 0x7fff0)),
+					1
+				);
+				dataA = _mm256_shuffle_epi8(dataA, shuf);
+				
+				_mm_storeu_si128((__m128i*)p, _mm256_castsi256_si128(dataA));
+				// increment output position
+				p -= popcnt32(mask & 0xffff);
+				
+				_mm_storeu_si128((__m128i*)(p + XMM_SIZE), _mm256_extracti128_si256(dataA, 1));
+				p -= popcnt32(mask & 0xffff0000);
+				
 #ifdef PLATFORM_AMD64
-                mask >>= 28;
-                shuf = _mm256_inserti128_si256(
-                    _mm256_castsi128_si256(_mm_load_si128((__m128i*)((char*)lookups->compact + (mask & 0x7fff0)))),
-                    *(__m128i*)((char*)lookups->compact + ((mask >> 16) & 0x7fff0)),
-                    1
-                );
-                dataB = _mm256_shuffle_epi8(dataB, shuf);
-
-                _mm_storeu_si128((__m128i*)(p + XMM_SIZE*2), _mm256_castsi256_si128(dataB));
-                p -= popcnt32(mask & 0xffff0);
-
-                _mm_storeu_si128((__m128i*)(p + XMM_SIZE*3), _mm256_extracti128_si256(dataB, 1));
-                p -= popcnt32((unsigned int)(mask >> 20));
+				mask >>= 28;
+				shuf = _mm256_inserti128_si256(
+					_mm256_castsi128_si256(_mm_load_si128((__m128i*)((char*)lookups->compact + (mask & 0x7fff0)))),
+					*(__m128i*)((char*)lookups->compact + ((mask >> 16) & 0x7fff0)),
+					1
+				);
+				dataB = _mm256_shuffle_epi8(dataB, shuf);
+				
+				_mm_storeu_si128((__m128i*)(p + XMM_SIZE*2), _mm256_castsi256_si128(dataB));
+				p -= popcnt32(mask & 0xffff0);
+				
+				_mm_storeu_si128((__m128i*)(p + XMM_SIZE*3), _mm256_extracti128_si256(dataB, 1));
+				p -= popcnt32((unsigned int)(mask >> 20));
 #else
-                mask >>= 32;
-                shuf = _mm256_inserti128_si256(
-                    _mm256_castsi128_si256(_mm_load_si128((__m128i*)(lookups->compact + (mask & 0x7fff)))),
-                    *(__m128i*)((char*)lookups->compact + ((mask >> 12) & 0x7fff0)),
-                    1
-                );
-                dataB = _mm256_shuffle_epi8(dataB, shuf);
-
-                _mm_storeu_si128((__m128i*)(p + XMM_SIZE*2), _mm256_castsi256_si128(dataB));
-                p -= popcnt32(mask & 0xffff);
-
-                _mm_storeu_si128((__m128i*)(p + XMM_SIZE*3), _mm256_extracti128_si256(dataB, 1));
-                p -= popcnt32(mask & 0xffff0000);
-#endif
-                p += XMM_SIZE*4;
-            }
-        } else {
-            if(use_isa < ISA_LEVEL_AVX3)
-                dataA = _mm256_add_epi8(oDataA, yencOffset);
-            dataB = _mm256_add_epi8(oDataB, _mm256_set1_epi8(-42));
-
-            _mm256_storeu_si256((__m256i*)p, dataA);
-            _mm256_storeu_si256((__m256i*)p + 1, dataB);
-            p += sizeof(__m256i)*2;
-            escFirst = 0;
-            yencOffset = _mm256_set1_epi8(-42);
-        }
-    }
-    _escFirst = (unsigned char)escFirst;
-    if(isRaw) {
-        // this would be the trivial solution, but requires the compiler holding onto minMask throughout the loop:
-        //_nextMask = ~(uint16_t)_mm256_movemask_epi8(_mm256_cmpeq_epi8(minMask, _mm256_set1_epi8('.')));
-        // instead, just scan the memory to determine what to set nextMask to
-        if(len != 0) { // have to gone through at least one loop cycle
-            if(src[i-2] == '\r' && src[i-1] == '\n' && src[i] == '.')
-                _nextMask = 1;
-            else if(src[i-1] == '\r' && src[i] == '\n' && src[i+1] == '.')
-                _nextMask = 2;
-            else
-                _nextMask = 0;
-        }
-    } else
-        _nextMask = 0;
-    _mm256_zeroupper();
+				mask >>= 32;
+				shuf = _mm256_inserti128_si256(
+					_mm256_castsi128_si256(_mm_load_si128((__m128i*)(lookups->compact + (mask & 0x7fff)))),
+					*(__m128i*)((char*)lookups->compact + ((mask >> 12) & 0x7fff0)),
+					1
+				);
+				dataB = _mm256_shuffle_epi8(dataB, shuf);
+				
+				_mm_storeu_si128((__m128i*)(p + XMM_SIZE*2), _mm256_castsi256_si128(dataB));
+				p -= popcnt32(mask & 0xffff);
+				
+				_mm_storeu_si128((__m128i*)(p + XMM_SIZE*3), _mm256_extracti128_si256(dataB, 1));
+				p -= popcnt32(mask & 0xffff0000);
+#endif
+				p += XMM_SIZE*4;
+			}
+		} else {
+			if(use_isa < ISA_LEVEL_AVX3)
+				dataA = _mm256_add_epi8(oDataA, yencOffset);
+			dataB = _mm256_add_epi8(oDataB, _mm256_set1_epi8(-42));
+			
+			_mm256_storeu_si256((__m256i*)p, dataA);
+			_mm256_storeu_si256((__m256i*)p + 1, dataB);
+			p += sizeof(__m256i)*2;
+			escFirst = 0;
+			yencOffset = _mm256_set1_epi8(-42);
+		}
+	}
+	_escFirst = (unsigned char)escFirst;
+	_mm256_zeroupper();
 }
+} // namespace
 #endif
```

### Comparing `sabctools-8.1.0/src/yencode/decoder_sse2.cc` & `sabctools-8.2.0/src/yencode/decoder_ssse3.cc`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 #include "common.h"
 
-#ifdef __SSE2__
 #include "decoder_common.h"
+#ifdef __SSSE3__
 #include "decoder_sse_base.h"
-
-void decoder_set_sse2_funcs() {
-    decoder_sse_init();
-    decoder_init_lut(lookups->eqFix, lookups->compact);
-    _do_decode = &do_decode_simd<false, false, sizeof(__m128i)*2, do_decode_sse<false, false, ISA_LEVEL_SSE2> >;
-    _do_decode_raw = &do_decode_simd<true, false, sizeof(__m128i)*2, do_decode_sse<true, false, ISA_LEVEL_SSE2> >;
-    _do_decode_end_raw = &do_decode_simd<true, true, sizeof(__m128i)*2, do_decode_sse<true, true, ISA_LEVEL_SSE2> >;
-    _decode_simd_level = ISA_LEVEL_SSE2;
+void RapidYenc::decoder_set_ssse3_funcs() {
+	decoder_sse_init(lookups);
+	decoder_init_lut(lookups->compact);
+	_do_decode = &do_decode_simd<false, false, sizeof(__m128i)*2, do_decode_sse<false, false, ISA_LEVEL_SSSE3> >;
+	_do_decode_raw = &do_decode_simd<true, false, sizeof(__m128i)*2, do_decode_sse<true, false, ISA_LEVEL_SSSE3> >;
+	_do_decode_end_raw = &do_decode_simd<true, true, sizeof(__m128i)*2, do_decode_sse<true, true, ISA_LEVEL_SSSE3> >;
+	_decode_isa = ISA_LEVEL_SSSE3;
 }
 #else
-
-void decoder_set_sse2_funcs() {}
-
+void RapidYenc::decoder_set_ssse3_funcs() {
+	decoder_set_sse2_funcs();
+}
 #endif
```

### Comparing `sabctools-8.1.0/src/yencode/decoder_ssse3.cc` & `sabctools-8.2.0/src/yencode/decoder_avx.cc`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 #include "common.h"
 
-#ifdef __SSSE3__
 #include "decoder_common.h"
+#if defined(__AVX__) && defined(__POPCNT__)
 #include "decoder_sse_base.h"
-void decoder_set_ssse3_funcs() {
-    decoder_sse_init();
-    decoder_init_lut(lookups->eqFix, lookups->compact);
-    _do_decode = &do_decode_simd<false, false, sizeof(__m128i)*2, do_decode_sse<false, false, ISA_LEVEL_SSSE3> >;
-    _do_decode_raw = &do_decode_simd<true, false, sizeof(__m128i)*2, do_decode_sse<true, false, ISA_LEVEL_SSSE3> >;
-    _do_decode_end_raw = &do_decode_simd<true, true, sizeof(__m128i)*2, do_decode_sse<true, true, ISA_LEVEL_SSSE3> >;
-    _decode_simd_level = ISA_LEVEL_SSSE3;
+void RapidYenc::decoder_set_avx_funcs() {
+	decoder_sse_init(lookups);
+	decoder_init_lut(lookups->compact);
+	_do_decode = &do_decode_simd<false, false, sizeof(__m128i)*2, do_decode_sse<false, false, ISA_LEVEL_SSE4_POPCNT> >;
+	_do_decode_raw = &do_decode_simd<true, false, sizeof(__m128i)*2, do_decode_sse<true, false, ISA_LEVEL_SSE4_POPCNT> >;
+	_do_decode_end_raw = &do_decode_simd<true, true, sizeof(__m128i)*2, do_decode_sse<true, true, ISA_LEVEL_SSE4_POPCNT> >;
+	_decode_isa = ISA_LEVEL_AVX;
 }
 #else
-
-void decoder_set_sse2_funcs();
-
-void decoder_set_ssse3_funcs() {
-    decoder_set_sse2_funcs();
+void RapidYenc::decoder_set_avx_funcs() {
+	decoder_set_ssse3_funcs();
 }
-
 #endif
```

### Comparing `sabctools-8.1.0/src/yencode/encoder_ssse3.cc` & `sabctools-8.2.0/src/yencode/encoder_ssse3.cc`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 #include "common.h"
+#include "encoder_common.h"
 
 // slightly faster version which improves the worst case scenario significantly; since worst case doesn't happen often, overall speedup is relatively minor
 // requires PSHUFB (SSSE3) instruction, but will use POPCNT (SSE4.2 (or AMD's ABM, but Phenom doesn't support SSSE3 so doesn't matter)) if available (these only seem to give minor speedups, so considered optional)
 #ifdef __SSSE3__
 #include "encoder_sse_base.h"
 
-void encoder_ssse3_init() {
-    _do_encode = &do_encode_simd< do_encode_sse<ISA_LEVEL_SSSE3> >;
-    encoder_sse_lut<ISA_LEVEL_SSSE3>();
+void RapidYenc::encoder_ssse3_init() {
+	_do_encode = &do_encode_simd< do_encode_sse<ISA_LEVEL_SSSE3> >;
+	encoder_sse_lut<ISA_LEVEL_SSSE3>();
+	_encode_isa = ISA_LEVEL_SSSE3;
 }
 #else
-
-void encoder_sse2_init();
-
-void encoder_ssse3_init() {
-    encoder_sse2_init();
+void RapidYenc::encoder_ssse3_init() {
+	encoder_sse2_init();
 }
-
 #endif
```

### Comparing `sabctools-8.1.0/src/yencode/hedley.h` & `sabctools-8.2.0/src/yencode/hedley.h`

 * *Files 14% similar despite different names*

```diff
@@ -6,44 +6,54 @@
  * the public domain worldwide. This software is distributed without
  * any warranty.
  *
  * For details, see <http://creativecommons.org/publicdomain/zero/1.0/>.
  * SPDX-License-Identifier: CC0-1.0
  */
 
-#if !defined(HEDLEY_VERSION) || (HEDLEY_VERSION < 12)
+#if !defined(HEDLEY_VERSION) || (HEDLEY_VERSION < 15)
 #if defined(HEDLEY_VERSION)
 #  undef HEDLEY_VERSION
 #endif
-#define HEDLEY_VERSION 12
+#define HEDLEY_VERSION 15
 
 #if defined(HEDLEY_STRINGIFY_EX)
 #  undef HEDLEY_STRINGIFY_EX
 #endif
 #define HEDLEY_STRINGIFY_EX(x) #x
 
 #if defined(HEDLEY_STRINGIFY)
 #  undef HEDLEY_STRINGIFY
 #endif
 #define HEDLEY_STRINGIFY(x) HEDLEY_STRINGIFY_EX(x)
 
 #if defined(HEDLEY_CONCAT_EX)
 #  undef HEDLEY_CONCAT_EX
 #endif
-#define HEDLEY_CONCAT_EX(a, b) a##b
+#define HEDLEY_CONCAT_EX(a,b) a##b
 
 #if defined(HEDLEY_CONCAT)
 #  undef HEDLEY_CONCAT
 #endif
-#define HEDLEY_CONCAT(a, b) HEDLEY_CONCAT_EX(a,b)
+#define HEDLEY_CONCAT(a,b) HEDLEY_CONCAT_EX(a,b)
+
+#if defined(HEDLEY_CONCAT3_EX)
+#  undef HEDLEY_CONCAT3_EX
+#endif
+#define HEDLEY_CONCAT3_EX(a,b,c) a##b##c
+
+#if defined(HEDLEY_CONCAT3)
+#  undef HEDLEY_CONCAT3
+#endif
+#define HEDLEY_CONCAT3(a,b,c) HEDLEY_CONCAT3_EX(a,b,c)
 
 #if defined(HEDLEY_VERSION_ENCODE)
 #  undef HEDLEY_VERSION_ENCODE
 #endif
-#define HEDLEY_VERSION_ENCODE(major, minor, revision) (((major) * 1000000) + ((minor) * 1000) + (revision))
+#define HEDLEY_VERSION_ENCODE(major,minor,revision) (((major) * 1000000) + ((minor) * 1000) + (revision))
 
 #if defined(HEDLEY_VERSION_DECODE_MAJOR)
 #  undef HEDLEY_VERSION_DECODE_MAJOR
 #endif
 #define HEDLEY_VERSION_DECODE_MAJOR(version) ((version) / 1000000)
 
 #if defined(HEDLEY_VERSION_DECODE_MINOR)
@@ -67,57 +77,73 @@
 
 #if defined(HEDLEY_GNUC_VERSION_CHECK)
 #  undef HEDLEY_GNUC_VERSION_CHECK
 #endif
 #if defined(HEDLEY_GNUC_VERSION)
 #  define HEDLEY_GNUC_VERSION_CHECK(major,minor,patch) (HEDLEY_GNUC_VERSION >= HEDLEY_VERSION_ENCODE(major, minor, patch))
 #else
-#  define HEDLEY_GNUC_VERSION_CHECK(major, minor, patch) (0)
+#  define HEDLEY_GNUC_VERSION_CHECK(major,minor,patch) (0)
 #endif
 
 #if defined(HEDLEY_MSVC_VERSION)
 #  undef HEDLEY_MSVC_VERSION
 #endif
-#if defined(_MSC_FULL_VER) && (_MSC_FULL_VER >= 140000000)
+#if defined(_MSC_FULL_VER) && (_MSC_FULL_VER >= 140000000) && !defined(__ICL)
 #  define HEDLEY_MSVC_VERSION HEDLEY_VERSION_ENCODE(_MSC_FULL_VER / 10000000, (_MSC_FULL_VER % 10000000) / 100000, (_MSC_FULL_VER % 100000) / 100)
-#elif defined(_MSC_FULL_VER)
+#elif defined(_MSC_FULL_VER) && !defined(__ICL)
 #  define HEDLEY_MSVC_VERSION HEDLEY_VERSION_ENCODE(_MSC_FULL_VER / 1000000, (_MSC_FULL_VER % 1000000) / 10000, (_MSC_FULL_VER % 10000) / 10)
-#elif defined(_MSC_VER)
+#elif defined(_MSC_VER) && !defined(__ICL)
 #  define HEDLEY_MSVC_VERSION HEDLEY_VERSION_ENCODE(_MSC_VER / 100, _MSC_VER % 100, 0)
 #endif
 
 #if defined(HEDLEY_MSVC_VERSION_CHECK)
 #  undef HEDLEY_MSVC_VERSION_CHECK
 #endif
-#if !defined(_MSC_VER)
-#  define HEDLEY_MSVC_VERSION_CHECK(major, minor, patch) (0)
+#if !defined(HEDLEY_MSVC_VERSION)
+#  define HEDLEY_MSVC_VERSION_CHECK(major,minor,patch) (0)
 #elif defined(_MSC_VER) && (_MSC_VER >= 1400)
 #  define HEDLEY_MSVC_VERSION_CHECK(major,minor,patch) (_MSC_FULL_VER >= ((major * 10000000) + (minor * 100000) + (patch)))
 #elif defined(_MSC_VER) && (_MSC_VER >= 1200)
 #  define HEDLEY_MSVC_VERSION_CHECK(major,minor,patch) (_MSC_FULL_VER >= ((major * 1000000) + (minor * 10000) + (patch)))
 #else
 #  define HEDLEY_MSVC_VERSION_CHECK(major,minor,patch) (_MSC_VER >= ((major * 100) + (minor)))
 #endif
 
 #if defined(HEDLEY_INTEL_VERSION)
 #  undef HEDLEY_INTEL_VERSION
 #endif
-#if defined(__INTEL_COMPILER) && defined(__INTEL_COMPILER_UPDATE)
+#if defined(__INTEL_COMPILER) && defined(__INTEL_COMPILER_UPDATE) && !defined(__ICL)
 #  define HEDLEY_INTEL_VERSION HEDLEY_VERSION_ENCODE(__INTEL_COMPILER / 100, __INTEL_COMPILER % 100, __INTEL_COMPILER_UPDATE)
-#elif defined(__INTEL_COMPILER)
+#elif defined(__INTEL_COMPILER) && !defined(__ICL)
 #  define HEDLEY_INTEL_VERSION HEDLEY_VERSION_ENCODE(__INTEL_COMPILER / 100, __INTEL_COMPILER % 100, 0)
 #endif
 
 #if defined(HEDLEY_INTEL_VERSION_CHECK)
 #  undef HEDLEY_INTEL_VERSION_CHECK
 #endif
 #if defined(HEDLEY_INTEL_VERSION)
 #  define HEDLEY_INTEL_VERSION_CHECK(major,minor,patch) (HEDLEY_INTEL_VERSION >= HEDLEY_VERSION_ENCODE(major, minor, patch))
 #else
-#  define HEDLEY_INTEL_VERSION_CHECK(major, minor, patch) (0)
+#  define HEDLEY_INTEL_VERSION_CHECK(major,minor,patch) (0)
+#endif
+
+#if defined(HEDLEY_INTEL_CL_VERSION)
+#  undef HEDLEY_INTEL_CL_VERSION
+#endif
+#if defined(__INTEL_COMPILER) && defined(__INTEL_COMPILER_UPDATE) && defined(__ICL)
+#  define HEDLEY_INTEL_CL_VERSION HEDLEY_VERSION_ENCODE(__INTEL_COMPILER, __INTEL_COMPILER_UPDATE, 0)
+#endif
+
+#if defined(HEDLEY_INTEL_CL_VERSION_CHECK)
+#  undef HEDLEY_INTEL_CL_VERSION_CHECK
+#endif
+#if defined(HEDLEY_INTEL_CL_VERSION)
+#  define HEDLEY_INTEL_CL_VERSION_CHECK(major,minor,patch) (HEDLEY_INTEL_CL_VERSION >= HEDLEY_VERSION_ENCODE(major, minor, patch))
+#else
+#  define HEDLEY_INTEL_CL_VERSION_CHECK(major,minor,patch) (0)
 #endif
 
 #if defined(HEDLEY_PGI_VERSION)
 #  undef HEDLEY_PGI_VERSION
 #endif
 #if defined(__PGI) && defined(__PGIC__) && defined(__PGIC_MINOR__) && defined(__PGIC_PATCHLEVEL__)
 #  define HEDLEY_PGI_VERSION HEDLEY_VERSION_ENCODE(__PGIC__, __PGIC_MINOR__, __PGIC_PATCHLEVEL__)
@@ -125,15 +151,15 @@
 
 #if defined(HEDLEY_PGI_VERSION_CHECK)
 #  undef HEDLEY_PGI_VERSION_CHECK
 #endif
 #if defined(HEDLEY_PGI_VERSION)
 #  define HEDLEY_PGI_VERSION_CHECK(major,minor,patch) (HEDLEY_PGI_VERSION >= HEDLEY_VERSION_ENCODE(major, minor, patch))
 #else
-#  define HEDLEY_PGI_VERSION_CHECK(major, minor, patch) (0)
+#  define HEDLEY_PGI_VERSION_CHECK(major,minor,patch) (0)
 #endif
 
 #if defined(HEDLEY_SUNPRO_VERSION)
 #  undef HEDLEY_SUNPRO_VERSION
 #endif
 #if defined(__SUNPRO_C) && (__SUNPRO_C > 0x1000)
 #  define HEDLEY_SUNPRO_VERSION HEDLEY_VERSION_ENCODE((((__SUNPRO_C >> 16) & 0xf) * 10) + ((__SUNPRO_C >> 12) & 0xf), (((__SUNPRO_C >> 8) & 0xf) * 10) + ((__SUNPRO_C >> 4) & 0xf), (__SUNPRO_C & 0xf) * 10)
@@ -147,15 +173,15 @@
 
 #if defined(HEDLEY_SUNPRO_VERSION_CHECK)
 #  undef HEDLEY_SUNPRO_VERSION_CHECK
 #endif
 #if defined(HEDLEY_SUNPRO_VERSION)
 #  define HEDLEY_SUNPRO_VERSION_CHECK(major,minor,patch) (HEDLEY_SUNPRO_VERSION >= HEDLEY_VERSION_ENCODE(major, minor, patch))
 #else
-#  define HEDLEY_SUNPRO_VERSION_CHECK(major, minor, patch) (0)
+#  define HEDLEY_SUNPRO_VERSION_CHECK(major,minor,patch) (0)
 #endif
 
 #if defined(HEDLEY_EMSCRIPTEN_VERSION)
 #  undef HEDLEY_EMSCRIPTEN_VERSION
 #endif
 #if defined(__EMSCRIPTEN__)
 #  define HEDLEY_EMSCRIPTEN_VERSION HEDLEY_VERSION_ENCODE(__EMSCRIPTEN_major__, __EMSCRIPTEN_minor__, __EMSCRIPTEN_tiny__)
@@ -163,15 +189,15 @@
 
 #if defined(HEDLEY_EMSCRIPTEN_VERSION_CHECK)
 #  undef HEDLEY_EMSCRIPTEN_VERSION_CHECK
 #endif
 #if defined(HEDLEY_EMSCRIPTEN_VERSION)
 #  define HEDLEY_EMSCRIPTEN_VERSION_CHECK(major,minor,patch) (HEDLEY_EMSCRIPTEN_VERSION >= HEDLEY_VERSION_ENCODE(major, minor, patch))
 #else
-#  define HEDLEY_EMSCRIPTEN_VERSION_CHECK(major, minor, patch) (0)
+#  define HEDLEY_EMSCRIPTEN_VERSION_CHECK(major,minor,patch) (0)
 #endif
 
 #if defined(HEDLEY_ARM_VERSION)
 #  undef HEDLEY_ARM_VERSION
 #endif
 #if defined(__CC_ARM) && defined(__ARMCOMPILER_VERSION)
 #  define HEDLEY_ARM_VERSION HEDLEY_VERSION_ENCODE(__ARMCOMPILER_VERSION / 1000000, (__ARMCOMPILER_VERSION % 1000000) / 10000, (__ARMCOMPILER_VERSION % 10000) / 100)
@@ -181,15 +207,15 @@
 
 #if defined(HEDLEY_ARM_VERSION_CHECK)
 #  undef HEDLEY_ARM_VERSION_CHECK
 #endif
 #if defined(HEDLEY_ARM_VERSION)
 #  define HEDLEY_ARM_VERSION_CHECK(major,minor,patch) (HEDLEY_ARM_VERSION >= HEDLEY_VERSION_ENCODE(major, minor, patch))
 #else
-#  define HEDLEY_ARM_VERSION_CHECK(major, minor, patch) (0)
+#  define HEDLEY_ARM_VERSION_CHECK(major,minor,patch) (0)
 #endif
 
 #if defined(HEDLEY_IBM_VERSION)
 #  undef HEDLEY_IBM_VERSION
 #endif
 #if defined(__ibmxl__)
 #  define HEDLEY_IBM_VERSION HEDLEY_VERSION_ENCODE(__ibmxl_version__, __ibmxl_release__, __ibmxl_modification__)
@@ -201,39 +227,39 @@
 
 #if defined(HEDLEY_IBM_VERSION_CHECK)
 #  undef HEDLEY_IBM_VERSION_CHECK
 #endif
 #if defined(HEDLEY_IBM_VERSION)
 #  define HEDLEY_IBM_VERSION_CHECK(major,minor,patch) (HEDLEY_IBM_VERSION >= HEDLEY_VERSION_ENCODE(major, minor, patch))
 #else
-#  define HEDLEY_IBM_VERSION_CHECK(major, minor, patch) (0)
+#  define HEDLEY_IBM_VERSION_CHECK(major,minor,patch) (0)
 #endif
 
 #if defined(HEDLEY_TI_VERSION)
 #  undef HEDLEY_TI_VERSION
 #endif
 #if \
     defined(__TI_COMPILER_VERSION__) && \
-    (\
+    ( \
       defined(__TMS470__) || defined(__TI_ARM__) || \
       defined(__MSP430__) || \
       defined(__TMS320C2000__) \
-)
+    )
 #  if (__TI_COMPILER_VERSION__ >= 16000000)
 #    define HEDLEY_TI_VERSION HEDLEY_VERSION_ENCODE(__TI_COMPILER_VERSION__ / 1000000, (__TI_COMPILER_VERSION__ % 1000000) / 1000, (__TI_COMPILER_VERSION__ % 1000))
 #  endif
 #endif
 
 #if defined(HEDLEY_TI_VERSION_CHECK)
 #  undef HEDLEY_TI_VERSION_CHECK
 #endif
 #if defined(HEDLEY_TI_VERSION)
 #  define HEDLEY_TI_VERSION_CHECK(major,minor,patch) (HEDLEY_TI_VERSION >= HEDLEY_VERSION_ENCODE(major, minor, patch))
 #else
-#  define HEDLEY_TI_VERSION_CHECK(major, minor, patch) (0)
+#  define HEDLEY_TI_VERSION_CHECK(major,minor,patch) (0)
 #endif
 
 #if defined(HEDLEY_TI_CL2000_VERSION)
 #  undef HEDLEY_TI_CL2000_VERSION
 #endif
 #if defined(__TI_COMPILER_VERSION__) && defined(__TMS320C2000__)
 #  define HEDLEY_TI_CL2000_VERSION HEDLEY_VERSION_ENCODE(__TI_COMPILER_VERSION__ / 1000000, (__TI_COMPILER_VERSION__ % 1000000) / 1000, (__TI_COMPILER_VERSION__ % 1000))
@@ -241,15 +267,15 @@
 
 #if defined(HEDLEY_TI_CL2000_VERSION_CHECK)
 #  undef HEDLEY_TI_CL2000_VERSION_CHECK
 #endif
 #if defined(HEDLEY_TI_CL2000_VERSION)
 #  define HEDLEY_TI_CL2000_VERSION_CHECK(major,minor,patch) (HEDLEY_TI_CL2000_VERSION >= HEDLEY_VERSION_ENCODE(major, minor, patch))
 #else
-#  define HEDLEY_TI_CL2000_VERSION_CHECK(major, minor, patch) (0)
+#  define HEDLEY_TI_CL2000_VERSION_CHECK(major,minor,patch) (0)
 #endif
 
 #if defined(HEDLEY_TI_CL430_VERSION)
 #  undef HEDLEY_TI_CL430_VERSION
 #endif
 #if defined(__TI_COMPILER_VERSION__) && defined(__MSP430__)
 #  define HEDLEY_TI_CL430_VERSION HEDLEY_VERSION_ENCODE(__TI_COMPILER_VERSION__ / 1000000, (__TI_COMPILER_VERSION__ % 1000000) / 1000, (__TI_COMPILER_VERSION__ % 1000))
@@ -257,15 +283,15 @@
 
 #if defined(HEDLEY_TI_CL430_VERSION_CHECK)
 #  undef HEDLEY_TI_CL430_VERSION_CHECK
 #endif
 #if defined(HEDLEY_TI_CL430_VERSION)
 #  define HEDLEY_TI_CL430_VERSION_CHECK(major,minor,patch) (HEDLEY_TI_CL430_VERSION >= HEDLEY_VERSION_ENCODE(major, minor, patch))
 #else
-#  define HEDLEY_TI_CL430_VERSION_CHECK(major, minor, patch) (0)
+#  define HEDLEY_TI_CL430_VERSION_CHECK(major,minor,patch) (0)
 #endif
 
 #if defined(HEDLEY_TI_ARMCL_VERSION)
 #  undef HEDLEY_TI_ARMCL_VERSION
 #endif
 #if defined(__TI_COMPILER_VERSION__) && (defined(__TMS470__) || defined(__TI_ARM__))
 #  define HEDLEY_TI_ARMCL_VERSION HEDLEY_VERSION_ENCODE(__TI_COMPILER_VERSION__ / 1000000, (__TI_COMPILER_VERSION__ % 1000000) / 1000, (__TI_COMPILER_VERSION__ % 1000))
@@ -273,15 +299,15 @@
 
 #if defined(HEDLEY_TI_ARMCL_VERSION_CHECK)
 #  undef HEDLEY_TI_ARMCL_VERSION_CHECK
 #endif
 #if defined(HEDLEY_TI_ARMCL_VERSION)
 #  define HEDLEY_TI_ARMCL_VERSION_CHECK(major,minor,patch) (HEDLEY_TI_ARMCL_VERSION >= HEDLEY_VERSION_ENCODE(major, minor, patch))
 #else
-#  define HEDLEY_TI_ARMCL_VERSION_CHECK(major, minor, patch) (0)
+#  define HEDLEY_TI_ARMCL_VERSION_CHECK(major,minor,patch) (0)
 #endif
 
 #if defined(HEDLEY_TI_CL6X_VERSION)
 #  undef HEDLEY_TI_CL6X_VERSION
 #endif
 #if defined(__TI_COMPILER_VERSION__) && defined(__TMS320C6X__)
 #  define HEDLEY_TI_CL6X_VERSION HEDLEY_VERSION_ENCODE(__TI_COMPILER_VERSION__ / 1000000, (__TI_COMPILER_VERSION__ % 1000000) / 1000, (__TI_COMPILER_VERSION__ % 1000))
@@ -289,15 +315,15 @@
 
 #if defined(HEDLEY_TI_CL6X_VERSION_CHECK)
 #  undef HEDLEY_TI_CL6X_VERSION_CHECK
 #endif
 #if defined(HEDLEY_TI_CL6X_VERSION)
 #  define HEDLEY_TI_CL6X_VERSION_CHECK(major,minor,patch) (HEDLEY_TI_CL6X_VERSION >= HEDLEY_VERSION_ENCODE(major, minor, patch))
 #else
-#  define HEDLEY_TI_CL6X_VERSION_CHECK(major, minor, patch) (0)
+#  define HEDLEY_TI_CL6X_VERSION_CHECK(major,minor,patch) (0)
 #endif
 
 #if defined(HEDLEY_TI_CL7X_VERSION)
 #  undef HEDLEY_TI_CL7X_VERSION
 #endif
 #if defined(__TI_COMPILER_VERSION__) && defined(__C7000__)
 #  define HEDLEY_TI_CL7X_VERSION HEDLEY_VERSION_ENCODE(__TI_COMPILER_VERSION__ / 1000000, (__TI_COMPILER_VERSION__ % 1000000) / 1000, (__TI_COMPILER_VERSION__ % 1000))
@@ -305,15 +331,15 @@
 
 #if defined(HEDLEY_TI_CL7X_VERSION_CHECK)
 #  undef HEDLEY_TI_CL7X_VERSION_CHECK
 #endif
 #if defined(HEDLEY_TI_CL7X_VERSION)
 #  define HEDLEY_TI_CL7X_VERSION_CHECK(major,minor,patch) (HEDLEY_TI_CL7X_VERSION >= HEDLEY_VERSION_ENCODE(major, minor, patch))
 #else
-#  define HEDLEY_TI_CL7X_VERSION_CHECK(major, minor, patch) (0)
+#  define HEDLEY_TI_CL7X_VERSION_CHECK(major,minor,patch) (0)
 #endif
 
 #if defined(HEDLEY_TI_CLPRU_VERSION)
 #  undef HEDLEY_TI_CLPRU_VERSION
 #endif
 #if defined(__TI_COMPILER_VERSION__) && defined(__PRU__)
 #  define HEDLEY_TI_CLPRU_VERSION HEDLEY_VERSION_ENCODE(__TI_COMPILER_VERSION__ / 1000000, (__TI_COMPILER_VERSION__ % 1000000) / 1000, (__TI_COMPILER_VERSION__ % 1000))
@@ -321,15 +347,15 @@
 
 #if defined(HEDLEY_TI_CLPRU_VERSION_CHECK)
 #  undef HEDLEY_TI_CLPRU_VERSION_CHECK
 #endif
 #if defined(HEDLEY_TI_CLPRU_VERSION)
 #  define HEDLEY_TI_CLPRU_VERSION_CHECK(major,minor,patch) (HEDLEY_TI_CLPRU_VERSION >= HEDLEY_VERSION_ENCODE(major, minor, patch))
 #else
-#  define HEDLEY_TI_CLPRU_VERSION_CHECK(major, minor, patch) (0)
+#  define HEDLEY_TI_CLPRU_VERSION_CHECK(major,minor,patch) (0)
 #endif
 
 #if defined(HEDLEY_CRAY_VERSION)
 #  undef HEDLEY_CRAY_VERSION
 #endif
 #if defined(_CRAYC)
 #  if defined(_RELEASE_PATCHLEVEL)
@@ -341,35 +367,35 @@
 
 #if defined(HEDLEY_CRAY_VERSION_CHECK)
 #  undef HEDLEY_CRAY_VERSION_CHECK
 #endif
 #if defined(HEDLEY_CRAY_VERSION)
 #  define HEDLEY_CRAY_VERSION_CHECK(major,minor,patch) (HEDLEY_CRAY_VERSION >= HEDLEY_VERSION_ENCODE(major, minor, patch))
 #else
-#  define HEDLEY_CRAY_VERSION_CHECK(major, minor, patch) (0)
+#  define HEDLEY_CRAY_VERSION_CHECK(major,minor,patch) (0)
 #endif
 
 #if defined(HEDLEY_IAR_VERSION)
 #  undef HEDLEY_IAR_VERSION
 #endif
 #if defined(__IAR_SYSTEMS_ICC__)
 #  if __VER__ > 1000
 #    define HEDLEY_IAR_VERSION HEDLEY_VERSION_ENCODE((__VER__ / 1000000), ((__VER__ / 1000) % 1000), (__VER__ % 1000))
 #  else
-#    define HEDLEY_IAR_VERSION HEDLEY_VERSION_ENCODE(VER / 100, __VER__ % 100, 0)
+#    define HEDLEY_IAR_VERSION HEDLEY_VERSION_ENCODE(__VER__ / 100, __VER__ % 100, 0)
 #  endif
 #endif
 
 #if defined(HEDLEY_IAR_VERSION_CHECK)
 #  undef HEDLEY_IAR_VERSION_CHECK
 #endif
 #if defined(HEDLEY_IAR_VERSION)
 #  define HEDLEY_IAR_VERSION_CHECK(major,minor,patch) (HEDLEY_IAR_VERSION >= HEDLEY_VERSION_ENCODE(major, minor, patch))
 #else
-#  define HEDLEY_IAR_VERSION_CHECK(major, minor, patch) (0)
+#  define HEDLEY_IAR_VERSION_CHECK(major,minor,patch) (0)
 #endif
 
 #if defined(HEDLEY_TINYC_VERSION)
 #  undef HEDLEY_TINYC_VERSION
 #endif
 #if defined(__TINYC__)
 #  define HEDLEY_TINYC_VERSION HEDLEY_VERSION_ENCODE(__TINYC__ / 1000, (__TINYC__ / 100) % 10, __TINYC__ % 100)
@@ -377,15 +403,15 @@
 
 #if defined(HEDLEY_TINYC_VERSION_CHECK)
 #  undef HEDLEY_TINYC_VERSION_CHECK
 #endif
 #if defined(HEDLEY_TINYC_VERSION)
 #  define HEDLEY_TINYC_VERSION_CHECK(major,minor,patch) (HEDLEY_TINYC_VERSION >= HEDLEY_VERSION_ENCODE(major, minor, patch))
 #else
-#  define HEDLEY_TINYC_VERSION_CHECK(major, minor, patch) (0)
+#  define HEDLEY_TINYC_VERSION_CHECK(major,minor,patch) (0)
 #endif
 
 #if defined(HEDLEY_DMC_VERSION)
 #  undef HEDLEY_DMC_VERSION
 #endif
 #if defined(__DMC__)
 #  define HEDLEY_DMC_VERSION HEDLEY_VERSION_ENCODE(__DMC__ >> 8, (__DMC__ >> 4) & 0xf, __DMC__ & 0xf)
@@ -393,15 +419,15 @@
 
 #if defined(HEDLEY_DMC_VERSION_CHECK)
 #  undef HEDLEY_DMC_VERSION_CHECK
 #endif
 #if defined(HEDLEY_DMC_VERSION)
 #  define HEDLEY_DMC_VERSION_CHECK(major,minor,patch) (HEDLEY_DMC_VERSION >= HEDLEY_VERSION_ENCODE(major, minor, patch))
 #else
-#  define HEDLEY_DMC_VERSION_CHECK(major, minor, patch) (0)
+#  define HEDLEY_DMC_VERSION_CHECK(major,minor,patch) (0)
 #endif
 
 #if defined(HEDLEY_COMPCERT_VERSION)
 #  undef HEDLEY_COMPCERT_VERSION
 #endif
 #if defined(__COMPCERT_VERSION__)
 #  define HEDLEY_COMPCERT_VERSION HEDLEY_VERSION_ENCODE(__COMPCERT_VERSION__ / 10000, (__COMPCERT_VERSION__ / 100) % 100, __COMPCERT_VERSION__ % 100)
@@ -409,15 +435,15 @@
 
 #if defined(HEDLEY_COMPCERT_VERSION_CHECK)
 #  undef HEDLEY_COMPCERT_VERSION_CHECK
 #endif
 #if defined(HEDLEY_COMPCERT_VERSION)
 #  define HEDLEY_COMPCERT_VERSION_CHECK(major,minor,patch) (HEDLEY_COMPCERT_VERSION >= HEDLEY_VERSION_ENCODE(major, minor, patch))
 #else
-#  define HEDLEY_COMPCERT_VERSION_CHECK(major, minor, patch) (0)
+#  define HEDLEY_COMPCERT_VERSION_CHECK(major,minor,patch) (0)
 #endif
 
 #if defined(HEDLEY_PELLES_VERSION)
 #  undef HEDLEY_PELLES_VERSION
 #endif
 #if defined(__POCC__)
 #  define HEDLEY_PELLES_VERSION HEDLEY_VERSION_ENCODE(__POCC__ / 100, __POCC__ % 100, 0)
@@ -425,116 +451,138 @@
 
 #if defined(HEDLEY_PELLES_VERSION_CHECK)
 #  undef HEDLEY_PELLES_VERSION_CHECK
 #endif
 #if defined(HEDLEY_PELLES_VERSION)
 #  define HEDLEY_PELLES_VERSION_CHECK(major,minor,patch) (HEDLEY_PELLES_VERSION >= HEDLEY_VERSION_ENCODE(major, minor, patch))
 #else
-#  define HEDLEY_PELLES_VERSION_CHECK(major, minor, patch) (0)
+#  define HEDLEY_PELLES_VERSION_CHECK(major,minor,patch) (0)
+#endif
+
+#if defined(HEDLEY_MCST_LCC_VERSION)
+#  undef HEDLEY_MCST_LCC_VERSION
+#endif
+#if defined(__LCC__) && defined(__LCC_MINOR__)
+#  define HEDLEY_MCST_LCC_VERSION HEDLEY_VERSION_ENCODE(__LCC__ / 100, __LCC__ % 100, __LCC_MINOR__)
+#endif
+
+#if defined(HEDLEY_MCST_LCC_VERSION_CHECK)
+#  undef HEDLEY_MCST_LCC_VERSION_CHECK
+#endif
+#if defined(HEDLEY_MCST_LCC_VERSION)
+#  define HEDLEY_MCST_LCC_VERSION_CHECK(major,minor,patch) (HEDLEY_MCST_LCC_VERSION >= HEDLEY_VERSION_ENCODE(major, minor, patch))
+#else
+#  define HEDLEY_MCST_LCC_VERSION_CHECK(major,minor,patch) (0)
 #endif
 
 #if defined(HEDLEY_GCC_VERSION)
 #  undef HEDLEY_GCC_VERSION
 #endif
 #if \
   defined(HEDLEY_GNUC_VERSION) && \
   !defined(__clang__) && \
   !defined(HEDLEY_INTEL_VERSION) && \
   !defined(HEDLEY_PGI_VERSION) && \
   !defined(HEDLEY_ARM_VERSION) && \
+  !defined(HEDLEY_CRAY_VERSION) && \
   !defined(HEDLEY_TI_VERSION) && \
   !defined(HEDLEY_TI_ARMCL_VERSION) && \
   !defined(HEDLEY_TI_CL430_VERSION) && \
   !defined(HEDLEY_TI_CL2000_VERSION) && \
   !defined(HEDLEY_TI_CL6X_VERSION) && \
   !defined(HEDLEY_TI_CL7X_VERSION) && \
   !defined(HEDLEY_TI_CLPRU_VERSION) && \
-  !defined(__COMPCERT__)
+  !defined(__COMPCERT__) && \
+  !defined(HEDLEY_MCST_LCC_VERSION)
 #  define HEDLEY_GCC_VERSION HEDLEY_GNUC_VERSION
 #endif
 
 #if defined(HEDLEY_GCC_VERSION_CHECK)
 #  undef HEDLEY_GCC_VERSION_CHECK
 #endif
 #if defined(HEDLEY_GCC_VERSION)
 #  define HEDLEY_GCC_VERSION_CHECK(major,minor,patch) (HEDLEY_GCC_VERSION >= HEDLEY_VERSION_ENCODE(major, minor, patch))
 #else
-#  define HEDLEY_GCC_VERSION_CHECK(major, minor, patch) (0)
+#  define HEDLEY_GCC_VERSION_CHECK(major,minor,patch) (0)
 #endif
 
 #if defined(HEDLEY_HAS_ATTRIBUTE)
 #  undef HEDLEY_HAS_ATTRIBUTE
 #endif
-#if defined(__has_attribute)
+#if \
+  defined(__has_attribute) && \
+  ( \
+    (!defined(HEDLEY_IAR_VERSION) || HEDLEY_IAR_VERSION_CHECK(8,5,9)) \
+  )
 #  define HEDLEY_HAS_ATTRIBUTE(attribute) __has_attribute(attribute)
 #else
 #  define HEDLEY_HAS_ATTRIBUTE(attribute) (0)
 #endif
 
 #if defined(HEDLEY_GNUC_HAS_ATTRIBUTE)
 #  undef HEDLEY_GNUC_HAS_ATTRIBUTE
 #endif
 #if defined(__has_attribute)
-#  define HEDLEY_GNUC_HAS_ATTRIBUTE(attribute,major,minor,patch) __has_attribute(attribute)
+#  define HEDLEY_GNUC_HAS_ATTRIBUTE(attribute,major,minor,patch) HEDLEY_HAS_ATTRIBUTE(attribute)
 #else
-#  define HEDLEY_GNUC_HAS_ATTRIBUTE(attribute, major, minor, patch) HEDLEY_GNUC_VERSION_CHECK(major,minor,patch)
+#  define HEDLEY_GNUC_HAS_ATTRIBUTE(attribute,major,minor,patch) HEDLEY_GNUC_VERSION_CHECK(major,minor,patch)
 #endif
 
 #if defined(HEDLEY_GCC_HAS_ATTRIBUTE)
 #  undef HEDLEY_GCC_HAS_ATTRIBUTE
 #endif
 #if defined(__has_attribute)
-#  define HEDLEY_GCC_HAS_ATTRIBUTE(attribute,major,minor,patch) __has_attribute(attribute)
+#  define HEDLEY_GCC_HAS_ATTRIBUTE(attribute,major,minor,patch) HEDLEY_HAS_ATTRIBUTE(attribute)
 #else
-#  define HEDLEY_GCC_HAS_ATTRIBUTE(attribute, major, minor, patch) HEDLEY_GCC_VERSION_CHECK(major,minor,patch)
+#  define HEDLEY_GCC_HAS_ATTRIBUTE(attribute,major,minor,patch) HEDLEY_GCC_VERSION_CHECK(major,minor,patch)
 #endif
 
 #if defined(HEDLEY_HAS_CPP_ATTRIBUTE)
 #  undef HEDLEY_HAS_CPP_ATTRIBUTE
 #endif
 #if \
   defined(__has_cpp_attribute) && \
   defined(__cplusplus) && \
-  (!defined(HEDLEY_SUNPRO_VERSION) || HEDLEY_SUNPRO_VERSION_CHECK(5, 15, 0))
+  (!defined(HEDLEY_SUNPRO_VERSION) || HEDLEY_SUNPRO_VERSION_CHECK(5,15,0))
 #  define HEDLEY_HAS_CPP_ATTRIBUTE(attribute) __has_cpp_attribute(attribute)
 #else
 #  define HEDLEY_HAS_CPP_ATTRIBUTE(attribute) (0)
 #endif
 
 #if defined(HEDLEY_HAS_CPP_ATTRIBUTE_NS)
 #  undef HEDLEY_HAS_CPP_ATTRIBUTE_NS
 #endif
 #if !defined(__cplusplus) || !defined(__has_cpp_attribute)
-#  define HEDLEY_HAS_CPP_ATTRIBUTE_NS(ns, attribute) (0)
+#  define HEDLEY_HAS_CPP_ATTRIBUTE_NS(ns,attribute) (0)
 #elif \
   !defined(HEDLEY_PGI_VERSION) && \
   !defined(HEDLEY_IAR_VERSION) && \
-  (!defined(HEDLEY_SUNPRO_VERSION) || HEDLEY_SUNPRO_VERSION_CHECK(5, 15, 0)) && \
-  (!defined(HEDLEY_MSVC_VERSION) || HEDLEY_MSVC_VERSION_CHECK(19, 20, 0))
+  (!defined(HEDLEY_SUNPRO_VERSION) || HEDLEY_SUNPRO_VERSION_CHECK(5,15,0)) && \
+  (!defined(HEDLEY_MSVC_VERSION) || HEDLEY_MSVC_VERSION_CHECK(19,20,0))
 #  define HEDLEY_HAS_CPP_ATTRIBUTE_NS(ns,attribute) HEDLEY_HAS_CPP_ATTRIBUTE(ns::attribute)
 #else
 #  define HEDLEY_HAS_CPP_ATTRIBUTE_NS(ns,attribute) (0)
 #endif
 
 #if defined(HEDLEY_GNUC_HAS_CPP_ATTRIBUTE)
 #  undef HEDLEY_GNUC_HAS_CPP_ATTRIBUTE
 #endif
 #if defined(__has_cpp_attribute) && defined(__cplusplus)
 #  define HEDLEY_GNUC_HAS_CPP_ATTRIBUTE(attribute,major,minor,patch) __has_cpp_attribute(attribute)
 #else
-#  define HEDLEY_GNUC_HAS_CPP_ATTRIBUTE(attribute, major, minor, patch) HEDLEY_GNUC_VERSION_CHECK(major,minor,patch)
+#  define HEDLEY_GNUC_HAS_CPP_ATTRIBUTE(attribute,major,minor,patch) HEDLEY_GNUC_VERSION_CHECK(major,minor,patch)
 #endif
 
 #if defined(HEDLEY_GCC_HAS_CPP_ATTRIBUTE)
 #  undef HEDLEY_GCC_HAS_CPP_ATTRIBUTE
 #endif
 #if defined(__has_cpp_attribute) && defined(__cplusplus)
 #  define HEDLEY_GCC_HAS_CPP_ATTRIBUTE(attribute,major,minor,patch) __has_cpp_attribute(attribute)
 #else
-#  define HEDLEY_GCC_HAS_CPP_ATTRIBUTE(attribute, major, minor, patch) HEDLEY_GCC_VERSION_CHECK(major,minor,patch)
+#  define HEDLEY_GCC_HAS_CPP_ATTRIBUTE(attribute,major,minor,patch) HEDLEY_GCC_VERSION_CHECK(major,minor,patch)
 #endif
 
 #if defined(HEDLEY_HAS_BUILTIN)
 #  undef HEDLEY_HAS_BUILTIN
 #endif
 #if defined(__has_builtin)
 #  define HEDLEY_HAS_BUILTIN(builtin) __has_builtin(builtin)
@@ -544,24 +592,24 @@
 
 #if defined(HEDLEY_GNUC_HAS_BUILTIN)
 #  undef HEDLEY_GNUC_HAS_BUILTIN
 #endif
 #if defined(__has_builtin)
 #  define HEDLEY_GNUC_HAS_BUILTIN(builtin,major,minor,patch) __has_builtin(builtin)
 #else
-#  define HEDLEY_GNUC_HAS_BUILTIN(builtin, major, minor, patch) HEDLEY_GNUC_VERSION_CHECK(major,minor,patch)
+#  define HEDLEY_GNUC_HAS_BUILTIN(builtin,major,minor,patch) HEDLEY_GNUC_VERSION_CHECK(major,minor,patch)
 #endif
 
 #if defined(HEDLEY_GCC_HAS_BUILTIN)
 #  undef HEDLEY_GCC_HAS_BUILTIN
 #endif
 #if defined(__has_builtin)
 #  define HEDLEY_GCC_HAS_BUILTIN(builtin,major,minor,patch) __has_builtin(builtin)
 #else
-#  define HEDLEY_GCC_HAS_BUILTIN(builtin, major, minor, patch) HEDLEY_GCC_VERSION_CHECK(major,minor,patch)
+#  define HEDLEY_GCC_HAS_BUILTIN(builtin,major,minor,patch) HEDLEY_GCC_VERSION_CHECK(major,minor,patch)
 #endif
 
 #if defined(HEDLEY_HAS_FEATURE)
 #  undef HEDLEY_HAS_FEATURE
 #endif
 #if defined(__has_feature)
 #  define HEDLEY_HAS_FEATURE(feature) __has_feature(feature)
@@ -571,24 +619,24 @@
 
 #if defined(HEDLEY_GNUC_HAS_FEATURE)
 #  undef HEDLEY_GNUC_HAS_FEATURE
 #endif
 #if defined(__has_feature)
 #  define HEDLEY_GNUC_HAS_FEATURE(feature,major,minor,patch) __has_feature(feature)
 #else
-#  define HEDLEY_GNUC_HAS_FEATURE(feature, major, minor, patch) HEDLEY_GNUC_VERSION_CHECK(major,minor,patch)
+#  define HEDLEY_GNUC_HAS_FEATURE(feature,major,minor,patch) HEDLEY_GNUC_VERSION_CHECK(major,minor,patch)
 #endif
 
 #if defined(HEDLEY_GCC_HAS_FEATURE)
 #  undef HEDLEY_GCC_HAS_FEATURE
 #endif
 #if defined(__has_feature)
 #  define HEDLEY_GCC_HAS_FEATURE(feature,major,minor,patch) __has_feature(feature)
 #else
-#  define HEDLEY_GCC_HAS_FEATURE(feature, major, minor, patch) HEDLEY_GCC_VERSION_CHECK(major,minor,patch)
+#  define HEDLEY_GCC_HAS_FEATURE(feature,major,minor,patch) HEDLEY_GCC_VERSION_CHECK(major,minor,patch)
 #endif
 
 #if defined(HEDLEY_HAS_EXTENSION)
 #  undef HEDLEY_HAS_EXTENSION
 #endif
 #if defined(__has_extension)
 #  define HEDLEY_HAS_EXTENSION(extension) __has_extension(extension)
@@ -598,24 +646,24 @@
 
 #if defined(HEDLEY_GNUC_HAS_EXTENSION)
 #  undef HEDLEY_GNUC_HAS_EXTENSION
 #endif
 #if defined(__has_extension)
 #  define HEDLEY_GNUC_HAS_EXTENSION(extension,major,minor,patch) __has_extension(extension)
 #else
-#  define HEDLEY_GNUC_HAS_EXTENSION(extension, major, minor, patch) HEDLEY_GNUC_VERSION_CHECK(major,minor,patch)
+#  define HEDLEY_GNUC_HAS_EXTENSION(extension,major,minor,patch) HEDLEY_GNUC_VERSION_CHECK(major,minor,patch)
 #endif
 
 #if defined(HEDLEY_GCC_HAS_EXTENSION)
 #  undef HEDLEY_GCC_HAS_EXTENSION
 #endif
 #if defined(__has_extension)
 #  define HEDLEY_GCC_HAS_EXTENSION(extension,major,minor,patch) __has_extension(extension)
 #else
-#  define HEDLEY_GCC_HAS_EXTENSION(extension, major, minor, patch) HEDLEY_GCC_VERSION_CHECK(major,minor,patch)
+#  define HEDLEY_GCC_HAS_EXTENSION(extension,major,minor,patch) HEDLEY_GCC_VERSION_CHECK(major,minor,patch)
 #endif
 
 #if defined(HEDLEY_HAS_DECLSPEC_ATTRIBUTE)
 #  undef HEDLEY_HAS_DECLSPEC_ATTRIBUTE
 #endif
 #if defined(__has_declspec_attribute)
 #  define HEDLEY_HAS_DECLSPEC_ATTRIBUTE(attribute) __has_declspec_attribute(attribute)
@@ -625,24 +673,24 @@
 
 #if defined(HEDLEY_GNUC_HAS_DECLSPEC_ATTRIBUTE)
 #  undef HEDLEY_GNUC_HAS_DECLSPEC_ATTRIBUTE
 #endif
 #if defined(__has_declspec_attribute)
 #  define HEDLEY_GNUC_HAS_DECLSPEC_ATTRIBUTE(attribute,major,minor,patch) __has_declspec_attribute(attribute)
 #else
-#  define HEDLEY_GNUC_HAS_DECLSPEC_ATTRIBUTE(attribute, major, minor, patch) HEDLEY_GNUC_VERSION_CHECK(major,minor,patch)
+#  define HEDLEY_GNUC_HAS_DECLSPEC_ATTRIBUTE(attribute,major,minor,patch) HEDLEY_GNUC_VERSION_CHECK(major,minor,patch)
 #endif
 
 #if defined(HEDLEY_GCC_HAS_DECLSPEC_ATTRIBUTE)
 #  undef HEDLEY_GCC_HAS_DECLSPEC_ATTRIBUTE
 #endif
 #if defined(__has_declspec_attribute)
 #  define HEDLEY_GCC_HAS_DECLSPEC_ATTRIBUTE(attribute,major,minor,patch) __has_declspec_attribute(attribute)
 #else
-#  define HEDLEY_GCC_HAS_DECLSPEC_ATTRIBUTE(attribute, major, minor, patch) HEDLEY_GCC_VERSION_CHECK(major,minor,patch)
+#  define HEDLEY_GCC_HAS_DECLSPEC_ATTRIBUTE(attribute,major,minor,patch) HEDLEY_GCC_VERSION_CHECK(major,minor,patch)
 #endif
 
 #if defined(HEDLEY_HAS_WARNING)
 #  undef HEDLEY_HAS_WARNING
 #endif
 #if defined(__has_warning)
 #  define HEDLEY_HAS_WARNING(warning) __has_warning(warning)
@@ -652,40 +700,116 @@
 
 #if defined(HEDLEY_GNUC_HAS_WARNING)
 #  undef HEDLEY_GNUC_HAS_WARNING
 #endif
 #if defined(__has_warning)
 #  define HEDLEY_GNUC_HAS_WARNING(warning,major,minor,patch) __has_warning(warning)
 #else
-#  define HEDLEY_GNUC_HAS_WARNING(warning, major, minor, patch) HEDLEY_GNUC_VERSION_CHECK(major,minor,patch)
+#  define HEDLEY_GNUC_HAS_WARNING(warning,major,minor,patch) HEDLEY_GNUC_VERSION_CHECK(major,minor,patch)
 #endif
 
 #if defined(HEDLEY_GCC_HAS_WARNING)
 #  undef HEDLEY_GCC_HAS_WARNING
 #endif
 #if defined(__has_warning)
 #  define HEDLEY_GCC_HAS_WARNING(warning,major,minor,patch) __has_warning(warning)
 #else
-#  define HEDLEY_GCC_HAS_WARNING(warning, major, minor, patch) HEDLEY_GCC_VERSION_CHECK(major,minor,patch)
+#  define HEDLEY_GCC_HAS_WARNING(warning,major,minor,patch) HEDLEY_GCC_VERSION_CHECK(major,minor,patch)
+#endif
+
+#if \
+  (defined(__STDC_VERSION__) && (__STDC_VERSION__ >= 199901L)) || \
+  defined(__clang__) || \
+  HEDLEY_GCC_VERSION_CHECK(3,0,0) || \
+  HEDLEY_INTEL_VERSION_CHECK(13,0,0) || \
+  HEDLEY_IAR_VERSION_CHECK(8,0,0) || \
+  HEDLEY_PGI_VERSION_CHECK(18,4,0) || \
+  HEDLEY_ARM_VERSION_CHECK(4,1,0) || \
+  HEDLEY_TI_VERSION_CHECK(15,12,0) || \
+  HEDLEY_TI_ARMCL_VERSION_CHECK(4,7,0) || \
+  HEDLEY_TI_CL430_VERSION_CHECK(2,0,1) || \
+  HEDLEY_TI_CL2000_VERSION_CHECK(6,1,0) || \
+  HEDLEY_TI_CL6X_VERSION_CHECK(7,0,0) || \
+  HEDLEY_TI_CL7X_VERSION_CHECK(1,2,0) || \
+  HEDLEY_TI_CLPRU_VERSION_CHECK(2,1,0) || \
+  HEDLEY_CRAY_VERSION_CHECK(5,0,0) || \
+  HEDLEY_TINYC_VERSION_CHECK(0,9,17) || \
+  HEDLEY_SUNPRO_VERSION_CHECK(8,0,0) || \
+  (HEDLEY_IBM_VERSION_CHECK(10,1,0) && defined(__C99_PRAGMA_OPERATOR))
+#  define HEDLEY_PRAGMA(value) _Pragma(#value)
+#elif HEDLEY_MSVC_VERSION_CHECK(15,0,0)
+#  define HEDLEY_PRAGMA(value) __pragma(value)
+#else
+#  define HEDLEY_PRAGMA(value)
+#endif
+
+#if defined(HEDLEY_DIAGNOSTIC_PUSH)
+#  undef HEDLEY_DIAGNOSTIC_PUSH
+#endif
+#if defined(HEDLEY_DIAGNOSTIC_POP)
+#  undef HEDLEY_DIAGNOSTIC_POP
+#endif
+#if defined(__clang__)
+#  define HEDLEY_DIAGNOSTIC_PUSH _Pragma("clang diagnostic push")
+#  define HEDLEY_DIAGNOSTIC_POP _Pragma("clang diagnostic pop")
+#elif HEDLEY_INTEL_VERSION_CHECK(13,0,0)
+#  define HEDLEY_DIAGNOSTIC_PUSH _Pragma("warning(push)")
+#  define HEDLEY_DIAGNOSTIC_POP _Pragma("warning(pop)")
+#elif HEDLEY_GCC_VERSION_CHECK(4,6,0)
+#  define HEDLEY_DIAGNOSTIC_PUSH _Pragma("GCC diagnostic push")
+#  define HEDLEY_DIAGNOSTIC_POP _Pragma("GCC diagnostic pop")
+#elif \
+  HEDLEY_MSVC_VERSION_CHECK(15,0,0) || \
+  HEDLEY_INTEL_CL_VERSION_CHECK(2021,1,0)
+#  define HEDLEY_DIAGNOSTIC_PUSH __pragma(warning(push))
+#  define HEDLEY_DIAGNOSTIC_POP __pragma(warning(pop))
+#elif HEDLEY_ARM_VERSION_CHECK(5,6,0)
+#  define HEDLEY_DIAGNOSTIC_PUSH _Pragma("push")
+#  define HEDLEY_DIAGNOSTIC_POP _Pragma("pop")
+#elif \
+    HEDLEY_TI_VERSION_CHECK(15,12,0) || \
+    HEDLEY_TI_ARMCL_VERSION_CHECK(5,2,0) || \
+    HEDLEY_TI_CL430_VERSION_CHECK(4,4,0) || \
+    HEDLEY_TI_CL6X_VERSION_CHECK(8,1,0) || \
+    HEDLEY_TI_CL7X_VERSION_CHECK(1,2,0) || \
+    HEDLEY_TI_CLPRU_VERSION_CHECK(2,1,0)
+#  define HEDLEY_DIAGNOSTIC_PUSH _Pragma("diag_push")
+#  define HEDLEY_DIAGNOSTIC_POP _Pragma("diag_pop")
+#elif HEDLEY_PELLES_VERSION_CHECK(2,90,0)
+#  define HEDLEY_DIAGNOSTIC_PUSH _Pragma("warning(push)")
+#  define HEDLEY_DIAGNOSTIC_POP _Pragma("warning(pop)")
+#else
+#  define HEDLEY_DIAGNOSTIC_PUSH
+#  define HEDLEY_DIAGNOSTIC_POP
 #endif
 
 /* HEDLEY_DIAGNOSTIC_DISABLE_CPP98_COMPAT_WRAP_ is for
    HEDLEY INTERNAL USE ONLY.  API subject to change without notice. */
 #if defined(HEDLEY_DIAGNOSTIC_DISABLE_CPP98_COMPAT_WRAP_)
 #  undef HEDLEY_DIAGNOSTIC_DISABLE_CPP98_COMPAT_WRAP_
 #endif
 #if defined(__cplusplus)
 #  if HEDLEY_HAS_WARNING("-Wc++98-compat")
 #    if HEDLEY_HAS_WARNING("-Wc++17-extensions")
-#      define HEDLEY_DIAGNOSTIC_DISABLE_CPP98_COMPAT_WRAP_(xpr) \
-         HEDLEY_DIAGNOSTIC_PUSH \
-         _Pragma("clang diagnostic ignored \"-Wc++98-compat\"") \
-         _Pragma("clang diagnostic ignored \"-Wc++17-extensions\"") \
-         xpr \
-         HEDLEY_DIAGNOSTIC_POP
+#      if HEDLEY_HAS_WARNING("-Wc++1z-extensions")
+#        define HEDLEY_DIAGNOSTIC_DISABLE_CPP98_COMPAT_WRAP_(xpr) \
+           HEDLEY_DIAGNOSTIC_PUSH \
+           _Pragma("clang diagnostic ignored \"-Wc++98-compat\"") \
+           _Pragma("clang diagnostic ignored \"-Wc++17-extensions\"") \
+           _Pragma("clang diagnostic ignored \"-Wc++1z-extensions\"") \
+           xpr \
+           HEDLEY_DIAGNOSTIC_POP
+#      else
+#        define HEDLEY_DIAGNOSTIC_DISABLE_CPP98_COMPAT_WRAP_(xpr) \
+           HEDLEY_DIAGNOSTIC_PUSH \
+           _Pragma("clang diagnostic ignored \"-Wc++98-compat\"") \
+           _Pragma("clang diagnostic ignored \"-Wc++17-extensions\"") \
+           xpr \
+           HEDLEY_DIAGNOSTIC_POP
+#      endif
 #    else
 #      define HEDLEY_DIAGNOSTIC_DISABLE_CPP98_COMPAT_WRAP_(xpr) \
          HEDLEY_DIAGNOSTIC_PUSH \
          _Pragma("clang diagnostic ignored \"-Wc++98-compat\"") \
          xpr \
          HEDLEY_DIAGNOSTIC_POP
 #    endif
@@ -698,16 +822,16 @@
 #if defined(HEDLEY_CONST_CAST)
 #  undef HEDLEY_CONST_CAST
 #endif
 #if defined(__cplusplus)
 #  define HEDLEY_CONST_CAST(T, expr) (const_cast<T>(expr))
 #elif \
   HEDLEY_HAS_WARNING("-Wcast-qual") || \
-  HEDLEY_GCC_VERSION_CHECK(4, 6, 0) || \
-  HEDLEY_INTEL_VERSION_CHECK(13, 0, 0)
+  HEDLEY_GCC_VERSION_CHECK(4,6,0) || \
+  HEDLEY_INTEL_VERSION_CHECK(13,0,0)
 #  define HEDLEY_CONST_CAST(T, expr) (__extension__ ({ \
       HEDLEY_DIAGNOSTIC_PUSH \
       HEDLEY_DIAGNOSTIC_DISABLE_CAST_QUAL \
       ((T) (expr)); \
       HEDLEY_DIAGNOSTIC_POP \
     }))
 #else
@@ -742,348 +866,329 @@
        _Pragma("clang diagnostic ignored \"-Wold-style-cast\"") \
        ((T) (expr)) \
        HEDLEY_DIAGNOSTIC_POP
 #  elif HEDLEY_IAR_VERSION_CHECK(8,3,0)
 #    define HEDLEY_CPP_CAST(T, expr) \
        HEDLEY_DIAGNOSTIC_PUSH \
        _Pragma("diag_suppress=Pe137") \
-       HEDLEY_DIAGNOSTIC_POP \
+       HEDLEY_DIAGNOSTIC_POP
 #  else
 #    define HEDLEY_CPP_CAST(T, expr) ((T) (expr))
 #  endif
 #else
 #  define HEDLEY_CPP_CAST(T, expr) (expr)
 #endif
 
-#if \
-  (defined(__STDC_VERSION__) && (__STDC_VERSION__ >= 199901L)) || \
-  defined(__clang__) || \
-  HEDLEY_GCC_VERSION_CHECK(3, 0, 0) || \
-  HEDLEY_INTEL_VERSION_CHECK(13, 0, 0) || \
-  HEDLEY_IAR_VERSION_CHECK(8, 0, 0) || \
-  HEDLEY_PGI_VERSION_CHECK(18, 4, 0) || \
-  HEDLEY_ARM_VERSION_CHECK(4, 1, 0) || \
-  HEDLEY_TI_VERSION_CHECK(15, 12, 0) || \
-  HEDLEY_TI_ARMCL_VERSION_CHECK(4, 7, 0) || \
-  HEDLEY_TI_CL430_VERSION_CHECK(2, 0, 1) || \
-  HEDLEY_TI_CL2000_VERSION_CHECK(6, 1, 0) || \
-  HEDLEY_TI_CL6X_VERSION_CHECK(7, 0, 0) || \
-  HEDLEY_TI_CL7X_VERSION_CHECK(1, 2, 0) || \
-  HEDLEY_TI_CLPRU_VERSION_CHECK(2, 1, 0) || \
-  HEDLEY_CRAY_VERSION_CHECK(5, 0, 0) || \
-  HEDLEY_TINYC_VERSION_CHECK(0, 9, 17) || \
-  HEDLEY_SUNPRO_VERSION_CHECK(8, 0, 0) || \
-  (HEDLEY_IBM_VERSION_CHECK(10, 1, 0) && defined(__C99_PRAGMA_OPERATOR))
-#  define HEDLEY_PRAGMA(value) _Pragma(#value)
-#elif HEDLEY_MSVC_VERSION_CHECK(15, 0, 0)
-#  define HEDLEY_PRAGMA(value) __pragma(value)
-#else
-#  define HEDLEY_PRAGMA(value)
-#endif
-
-#if defined(HEDLEY_DIAGNOSTIC_PUSH)
-#  undef HEDLEY_DIAGNOSTIC_PUSH
-#endif
-#if defined(HEDLEY_DIAGNOSTIC_POP)
-#  undef HEDLEY_DIAGNOSTIC_POP
-#endif
-#if defined(__clang__)
-#  define HEDLEY_DIAGNOSTIC_PUSH _Pragma("clang diagnostic push")
-#  define HEDLEY_DIAGNOSTIC_POP _Pragma("clang diagnostic pop")
-#elif HEDLEY_INTEL_VERSION_CHECK(13, 0, 0)
-#  define HEDLEY_DIAGNOSTIC_PUSH _Pragma("warning(push)")
-#  define HEDLEY_DIAGNOSTIC_POP _Pragma("warning(pop)")
-#elif HEDLEY_GCC_VERSION_CHECK(4, 6, 0)
-#  define HEDLEY_DIAGNOSTIC_PUSH _Pragma("GCC diagnostic push")
-#  define HEDLEY_DIAGNOSTIC_POP _Pragma("GCC diagnostic pop")
-#elif HEDLEY_MSVC_VERSION_CHECK(15, 0, 0)
-#  define HEDLEY_DIAGNOSTIC_PUSH __pragma(warning(push))
-#  define HEDLEY_DIAGNOSTIC_POP __pragma(warning(pop))
-#elif HEDLEY_ARM_VERSION_CHECK(5, 6, 0)
-#  define HEDLEY_DIAGNOSTIC_PUSH _Pragma("push")
-#  define HEDLEY_DIAGNOSTIC_POP _Pragma("pop")
-#elif \
-    HEDLEY_TI_VERSION_CHECK(15, 12, 0) || \
-    HEDLEY_TI_ARMCL_VERSION_CHECK(5, 2, 0) || \
-    HEDLEY_TI_CL430_VERSION_CHECK(4, 4, 0) || \
-    HEDLEY_TI_CL6X_VERSION_CHECK(8, 1, 0) || \
-    HEDLEY_TI_CL7X_VERSION_CHECK(1, 2, 0) || \
-    HEDLEY_TI_CLPRU_VERSION_CHECK(2, 1, 0)
-#  define HEDLEY_DIAGNOSTIC_PUSH _Pragma("diag_push")
-#  define HEDLEY_DIAGNOSTIC_POP _Pragma("diag_pop")
-#elif HEDLEY_PELLES_VERSION_CHECK(2, 90, 0)
-#  define HEDLEY_DIAGNOSTIC_PUSH _Pragma("warning(push)")
-#  define HEDLEY_DIAGNOSTIC_POP _Pragma("warning(pop)")
-#else
-#  define HEDLEY_DIAGNOSTIC_PUSH
-#  define HEDLEY_DIAGNOSTIC_POP
-#endif
-
 #if defined(HEDLEY_DIAGNOSTIC_DISABLE_DEPRECATED)
 #  undef HEDLEY_DIAGNOSTIC_DISABLE_DEPRECATED
 #endif
 #if HEDLEY_HAS_WARNING("-Wdeprecated-declarations")
 #  define HEDLEY_DIAGNOSTIC_DISABLE_DEPRECATED _Pragma("clang diagnostic ignored \"-Wdeprecated-declarations\"")
-#elif HEDLEY_INTEL_VERSION_CHECK(13, 0, 0)
+#elif HEDLEY_INTEL_VERSION_CHECK(13,0,0)
 #  define HEDLEY_DIAGNOSTIC_DISABLE_DEPRECATED _Pragma("warning(disable:1478 1786)")
-#elif HEDLEY_PGI_VERSION_CHECK(17, 10, 0)
+#elif HEDLEY_INTEL_CL_VERSION_CHECK(2021,1,0)
+#  define HEDLEY_DIAGNOSTIC_DISABLE_DEPRECATED __pragma(warning(disable:1478 1786))
+#elif HEDLEY_PGI_VERSION_CHECK(20,7,0)
+#  define HEDLEY_DIAGNOSTIC_DISABLE_DEPRECATED _Pragma("diag_suppress 1215,1216,1444,1445")
+#elif HEDLEY_PGI_VERSION_CHECK(17,10,0)
 #  define HEDLEY_DIAGNOSTIC_DISABLE_DEPRECATED _Pragma("diag_suppress 1215,1444")
-#elif HEDLEY_GCC_VERSION_CHECK(4, 3, 0)
+#elif HEDLEY_GCC_VERSION_CHECK(4,3,0)
 #  define HEDLEY_DIAGNOSTIC_DISABLE_DEPRECATED _Pragma("GCC diagnostic ignored \"-Wdeprecated-declarations\"")
-#elif HEDLEY_MSVC_VERSION_CHECK(15, 0, 0)
+#elif HEDLEY_MSVC_VERSION_CHECK(15,0,0)
 #  define HEDLEY_DIAGNOSTIC_DISABLE_DEPRECATED __pragma(warning(disable:4996))
+#elif HEDLEY_MCST_LCC_VERSION_CHECK(1,25,10)
+#  define HEDLEY_DIAGNOSTIC_DISABLE_DEPRECATED _Pragma("diag_suppress 1215,1444")
 #elif \
-    HEDLEY_TI_VERSION_CHECK(15, 12, 0) || \
-    (HEDLEY_TI_ARMCL_VERSION_CHECK(4, 8, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-    HEDLEY_TI_ARMCL_VERSION_CHECK(5, 2, 0) || \
-    (HEDLEY_TI_CL2000_VERSION_CHECK(6, 0, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-    HEDLEY_TI_CL2000_VERSION_CHECK(6, 4, 0) || \
-    (HEDLEY_TI_CL430_VERSION_CHECK(4, 0, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-    HEDLEY_TI_CL430_VERSION_CHECK(4, 3, 0) || \
-    (HEDLEY_TI_CL6X_VERSION_CHECK(7, 2, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-    HEDLEY_TI_CL6X_VERSION_CHECK(7, 5, 0) || \
-    HEDLEY_TI_CL7X_VERSION_CHECK(1, 2, 0) || \
-    HEDLEY_TI_CLPRU_VERSION_CHECK(2, 1, 0)
+    HEDLEY_TI_VERSION_CHECK(15,12,0) || \
+    (HEDLEY_TI_ARMCL_VERSION_CHECK(4,8,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+    HEDLEY_TI_ARMCL_VERSION_CHECK(5,2,0) || \
+    (HEDLEY_TI_CL2000_VERSION_CHECK(6,0,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+    HEDLEY_TI_CL2000_VERSION_CHECK(6,4,0) || \
+    (HEDLEY_TI_CL430_VERSION_CHECK(4,0,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+    HEDLEY_TI_CL430_VERSION_CHECK(4,3,0) || \
+    (HEDLEY_TI_CL6X_VERSION_CHECK(7,2,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+    HEDLEY_TI_CL6X_VERSION_CHECK(7,5,0) || \
+    HEDLEY_TI_CL7X_VERSION_CHECK(1,2,0) || \
+    HEDLEY_TI_CLPRU_VERSION_CHECK(2,1,0)
 #  define HEDLEY_DIAGNOSTIC_DISABLE_DEPRECATED _Pragma("diag_suppress 1291,1718")
-#elif HEDLEY_SUNPRO_VERSION_CHECK(5, 13, 0) && !defined(__cplusplus)
+#elif HEDLEY_SUNPRO_VERSION_CHECK(5,13,0) && !defined(__cplusplus)
 #  define HEDLEY_DIAGNOSTIC_DISABLE_DEPRECATED _Pragma("error_messages(off,E_DEPRECATED_ATT,E_DEPRECATED_ATT_MESS)")
-#elif HEDLEY_SUNPRO_VERSION_CHECK(5, 13, 0) && defined(__cplusplus)
+#elif HEDLEY_SUNPRO_VERSION_CHECK(5,13,0) && defined(__cplusplus)
 #  define HEDLEY_DIAGNOSTIC_DISABLE_DEPRECATED _Pragma("error_messages(off,symdeprecated,symdeprecated2)")
-#elif HEDLEY_IAR_VERSION_CHECK(8, 0, 0)
+#elif HEDLEY_IAR_VERSION_CHECK(8,0,0)
 #  define HEDLEY_DIAGNOSTIC_DISABLE_DEPRECATED _Pragma("diag_suppress=Pe1444,Pe1215")
-#elif HEDLEY_PELLES_VERSION_CHECK(2, 90, 0)
+#elif HEDLEY_PELLES_VERSION_CHECK(2,90,0)
 #  define HEDLEY_DIAGNOSTIC_DISABLE_DEPRECATED _Pragma("warn(disable:2241)")
 #else
 #  define HEDLEY_DIAGNOSTIC_DISABLE_DEPRECATED
 #endif
 
 #if defined(HEDLEY_DIAGNOSTIC_DISABLE_UNKNOWN_PRAGMAS)
 #  undef HEDLEY_DIAGNOSTIC_DISABLE_UNKNOWN_PRAGMAS
 #endif
 #if HEDLEY_HAS_WARNING("-Wunknown-pragmas")
 #  define HEDLEY_DIAGNOSTIC_DISABLE_UNKNOWN_PRAGMAS _Pragma("clang diagnostic ignored \"-Wunknown-pragmas\"")
-#elif HEDLEY_INTEL_VERSION_CHECK(13, 0, 0)
+#elif HEDLEY_INTEL_VERSION_CHECK(13,0,0)
 #  define HEDLEY_DIAGNOSTIC_DISABLE_UNKNOWN_PRAGMAS _Pragma("warning(disable:161)")
-#elif HEDLEY_PGI_VERSION_CHECK(17, 10, 0)
+#elif HEDLEY_INTEL_CL_VERSION_CHECK(2021,1,0)
+#  define HEDLEY_DIAGNOSTIC_DISABLE_UNKNOWN_PRAGMAS __pragma(warning(disable:161))
+#elif HEDLEY_PGI_VERSION_CHECK(17,10,0)
 #  define HEDLEY_DIAGNOSTIC_DISABLE_UNKNOWN_PRAGMAS _Pragma("diag_suppress 1675")
-#elif HEDLEY_GCC_VERSION_CHECK(4, 3, 0)
+#elif HEDLEY_GCC_VERSION_CHECK(4,3,0)
 #  define HEDLEY_DIAGNOSTIC_DISABLE_UNKNOWN_PRAGMAS _Pragma("GCC diagnostic ignored \"-Wunknown-pragmas\"")
-#elif HEDLEY_MSVC_VERSION_CHECK(15, 0, 0)
+#elif HEDLEY_MSVC_VERSION_CHECK(15,0,0)
 #  define HEDLEY_DIAGNOSTIC_DISABLE_UNKNOWN_PRAGMAS __pragma(warning(disable:4068))
 #elif \
-    HEDLEY_TI_VERSION_CHECK(16, 9, 0) || \
-    HEDLEY_TI_CL6X_VERSION_CHECK(8, 0, 0) || \
-    HEDLEY_TI_CL7X_VERSION_CHECK(1, 2, 0) || \
-    HEDLEY_TI_CLPRU_VERSION_CHECK(2, 3, 0)
+    HEDLEY_TI_VERSION_CHECK(16,9,0) || \
+    HEDLEY_TI_CL6X_VERSION_CHECK(8,0,0) || \
+    HEDLEY_TI_CL7X_VERSION_CHECK(1,2,0) || \
+    HEDLEY_TI_CLPRU_VERSION_CHECK(2,3,0)
 #  define HEDLEY_DIAGNOSTIC_DISABLE_UNKNOWN_PRAGMAS _Pragma("diag_suppress 163")
-#elif HEDLEY_TI_CL6X_VERSION_CHECK(8, 0, 0)
+#elif HEDLEY_TI_CL6X_VERSION_CHECK(8,0,0)
 #  define HEDLEY_DIAGNOSTIC_DISABLE_UNKNOWN_PRAGMAS _Pragma("diag_suppress 163")
-#elif HEDLEY_IAR_VERSION_CHECK(8, 0, 0)
+#elif HEDLEY_IAR_VERSION_CHECK(8,0,0)
 #  define HEDLEY_DIAGNOSTIC_DISABLE_UNKNOWN_PRAGMAS _Pragma("diag_suppress=Pe161")
+#elif HEDLEY_MCST_LCC_VERSION_CHECK(1,25,10)
+#  define HEDLEY_DIAGNOSTIC_DISABLE_UNKNOWN_PRAGMAS _Pragma("diag_suppress 161")
 #else
 #  define HEDLEY_DIAGNOSTIC_DISABLE_UNKNOWN_PRAGMAS
 #endif
 
 #if defined(HEDLEY_DIAGNOSTIC_DISABLE_UNKNOWN_CPP_ATTRIBUTES)
 #  undef HEDLEY_DIAGNOSTIC_DISABLE_UNKNOWN_CPP_ATTRIBUTES
 #endif
 #if HEDLEY_HAS_WARNING("-Wunknown-attributes")
 #  define HEDLEY_DIAGNOSTIC_DISABLE_UNKNOWN_CPP_ATTRIBUTES _Pragma("clang diagnostic ignored \"-Wunknown-attributes\"")
-#elif HEDLEY_GCC_VERSION_CHECK(4, 6, 0)
+#elif HEDLEY_GCC_VERSION_CHECK(4,6,0)
 #  define HEDLEY_DIAGNOSTIC_DISABLE_UNKNOWN_CPP_ATTRIBUTES _Pragma("GCC diagnostic ignored \"-Wdeprecated-declarations\"")
-#elif HEDLEY_INTEL_VERSION_CHECK(17, 0, 0)
+#elif HEDLEY_INTEL_VERSION_CHECK(17,0,0)
 #  define HEDLEY_DIAGNOSTIC_DISABLE_UNKNOWN_CPP_ATTRIBUTES _Pragma("warning(disable:1292)")
-#elif HEDLEY_MSVC_VERSION_CHECK(19, 0, 0)
+#elif HEDLEY_INTEL_CL_VERSION_CHECK(2021,1,0)
+#  define HEDLEY_DIAGNOSTIC_DISABLE_UNKNOWN_CPP_ATTRIBUTES __pragma(warning(disable:1292))
+#elif HEDLEY_MSVC_VERSION_CHECK(19,0,0)
 #  define HEDLEY_DIAGNOSTIC_DISABLE_UNKNOWN_CPP_ATTRIBUTES __pragma(warning(disable:5030))
-#elif HEDLEY_PGI_VERSION_CHECK(17, 10, 0)
+#elif HEDLEY_PGI_VERSION_CHECK(20,7,0)
+#  define HEDLEY_DIAGNOSTIC_DISABLE_UNKNOWN_CPP_ATTRIBUTES _Pragma("diag_suppress 1097,1098")
+#elif HEDLEY_PGI_VERSION_CHECK(17,10,0)
 #  define HEDLEY_DIAGNOSTIC_DISABLE_UNKNOWN_CPP_ATTRIBUTES _Pragma("diag_suppress 1097")
-#elif HEDLEY_SUNPRO_VERSION_CHECK(5, 14, 0) && defined(__cplusplus)
+#elif HEDLEY_SUNPRO_VERSION_CHECK(5,14,0) && defined(__cplusplus)
 #  define HEDLEY_DIAGNOSTIC_DISABLE_UNKNOWN_CPP_ATTRIBUTES _Pragma("error_messages(off,attrskipunsup)")
 #elif \
-    HEDLEY_TI_VERSION_CHECK(18, 1, 0) || \
-    HEDLEY_TI_CL6X_VERSION_CHECK(8, 3, 0) || \
-    HEDLEY_TI_CL7X_VERSION_CHECK(1, 2, 0)
+    HEDLEY_TI_VERSION_CHECK(18,1,0) || \
+    HEDLEY_TI_CL6X_VERSION_CHECK(8,3,0) || \
+    HEDLEY_TI_CL7X_VERSION_CHECK(1,2,0)
 #  define HEDLEY_DIAGNOSTIC_DISABLE_UNKNOWN_CPP_ATTRIBUTES _Pragma("diag_suppress 1173")
-#elif HEDLEY_IAR_VERSION_CHECK(8, 0, 0)
+#elif HEDLEY_IAR_VERSION_CHECK(8,0,0)
 #  define HEDLEY_DIAGNOSTIC_DISABLE_UNKNOWN_CPP_ATTRIBUTES _Pragma("diag_suppress=Pe1097")
+#elif HEDLEY_MCST_LCC_VERSION_CHECK(1,25,10)
+#  define HEDLEY_DIAGNOSTIC_DISABLE_UNKNOWN_CPP_ATTRIBUTES _Pragma("diag_suppress 1097")
 #else
 #  define HEDLEY_DIAGNOSTIC_DISABLE_UNKNOWN_CPP_ATTRIBUTES
 #endif
 
 #if defined(HEDLEY_DIAGNOSTIC_DISABLE_CAST_QUAL)
 #  undef HEDLEY_DIAGNOSTIC_DISABLE_CAST_QUAL
 #endif
 #if HEDLEY_HAS_WARNING("-Wcast-qual")
 #  define HEDLEY_DIAGNOSTIC_DISABLE_CAST_QUAL _Pragma("clang diagnostic ignored \"-Wcast-qual\"")
-#elif HEDLEY_INTEL_VERSION_CHECK(13, 0, 0)
+#elif HEDLEY_INTEL_VERSION_CHECK(13,0,0)
 #  define HEDLEY_DIAGNOSTIC_DISABLE_CAST_QUAL _Pragma("warning(disable:2203 2331)")
-#elif HEDLEY_GCC_VERSION_CHECK(3, 0, 0)
+#elif HEDLEY_GCC_VERSION_CHECK(3,0,0)
 #  define HEDLEY_DIAGNOSTIC_DISABLE_CAST_QUAL _Pragma("GCC diagnostic ignored \"-Wcast-qual\"")
 #else
 #  define HEDLEY_DIAGNOSTIC_DISABLE_CAST_QUAL
 #endif
 
+#if defined(HEDLEY_DIAGNOSTIC_DISABLE_UNUSED_FUNCTION)
+#  undef HEDLEY_DIAGNOSTIC_DISABLE_UNUSED_FUNCTION
+#endif
+#if HEDLEY_HAS_WARNING("-Wunused-function")
+#  define HEDLEY_DIAGNOSTIC_DISABLE_UNUSED_FUNCTION _Pragma("clang diagnostic ignored \"-Wunused-function\"")
+#elif HEDLEY_GCC_VERSION_CHECK(3,4,0)
+#  define HEDLEY_DIAGNOSTIC_DISABLE_UNUSED_FUNCTION _Pragma("GCC diagnostic ignored \"-Wunused-function\"")
+#elif HEDLEY_MSVC_VERSION_CHECK(1,0,0)
+#  define HEDLEY_DIAGNOSTIC_DISABLE_UNUSED_FUNCTION __pragma(warning(disable:4505))
+#elif HEDLEY_MCST_LCC_VERSION_CHECK(1,25,10)
+#  define HEDLEY_DIAGNOSTIC_DISABLE_UNUSED_FUNCTION _Pragma("diag_suppress 3142")
+#else
+#  define HEDLEY_DIAGNOSTIC_DISABLE_UNUSED_FUNCTION
+#endif
+
 #if defined(HEDLEY_DEPRECATED)
 #  undef HEDLEY_DEPRECATED
 #endif
 #if defined(HEDLEY_DEPRECATED_FOR)
 #  undef HEDLEY_DEPRECATED_FOR
 #endif
-#if defined(__cplusplus) && (__cplusplus >= 201402L)
-#  define HEDLEY_DEPRECATED(since) HEDLEY_DIAGNOSTIC_DISABLE_CPP98_COMPAT_WRAP_([[deprecated("Since " #since)]])
-#  define HEDLEY_DEPRECATED_FOR(since, replacement) HEDLEY_DIAGNOSTIC_DISABLE_CPP98_COMPAT_WRAP_([[deprecated("Since " #since "; use " #replacement)]])
+#if \
+  HEDLEY_MSVC_VERSION_CHECK(14,0,0) || \
+  HEDLEY_INTEL_CL_VERSION_CHECK(2021,1,0)
+#  define HEDLEY_DEPRECATED(since) __declspec(deprecated("Since " # since))
+#  define HEDLEY_DEPRECATED_FOR(since, replacement) __declspec(deprecated("Since " #since "; use " #replacement))
 #elif \
-  HEDLEY_HAS_EXTENSION(attribute_deprecated_with_message) || \
-  HEDLEY_GCC_VERSION_CHECK(4, 5, 0) || \
-  HEDLEY_INTEL_VERSION_CHECK(13, 0, 0) || \
-  HEDLEY_ARM_VERSION_CHECK(5, 6, 0) || \
-  HEDLEY_SUNPRO_VERSION_CHECK(5, 13, 0) || \
-  HEDLEY_PGI_VERSION_CHECK(17, 10, 0) || \
-  HEDLEY_TI_VERSION_CHECK(18, 1, 0) || \
-  HEDLEY_TI_ARMCL_VERSION_CHECK(18, 1, 0) || \
-  HEDLEY_TI_CL6X_VERSION_CHECK(8, 3, 0) || \
-  HEDLEY_TI_CL7X_VERSION_CHECK(1, 2, 0) || \
-  HEDLEY_TI_CLPRU_VERSION_CHECK(2, 3, 0)
+  (HEDLEY_HAS_EXTENSION(attribute_deprecated_with_message) && !defined(HEDLEY_IAR_VERSION)) || \
+  HEDLEY_GCC_VERSION_CHECK(4,5,0) || \
+  HEDLEY_INTEL_VERSION_CHECK(13,0,0) || \
+  HEDLEY_ARM_VERSION_CHECK(5,6,0) || \
+  HEDLEY_SUNPRO_VERSION_CHECK(5,13,0) || \
+  HEDLEY_PGI_VERSION_CHECK(17,10,0) || \
+  HEDLEY_TI_VERSION_CHECK(18,1,0) || \
+  HEDLEY_TI_ARMCL_VERSION_CHECK(18,1,0) || \
+  HEDLEY_TI_CL6X_VERSION_CHECK(8,3,0) || \
+  HEDLEY_TI_CL7X_VERSION_CHECK(1,2,0) || \
+  HEDLEY_TI_CLPRU_VERSION_CHECK(2,3,0) || \
+  HEDLEY_MCST_LCC_VERSION_CHECK(1,25,10)
 #  define HEDLEY_DEPRECATED(since) __attribute__((__deprecated__("Since " #since)))
 #  define HEDLEY_DEPRECATED_FOR(since, replacement) __attribute__((__deprecated__("Since " #since "; use " #replacement)))
+#elif defined(__cplusplus) && (__cplusplus >= 201402L)
+#  define HEDLEY_DEPRECATED(since) HEDLEY_DIAGNOSTIC_DISABLE_CPP98_COMPAT_WRAP_([[deprecated("Since " #since)]])
+#  define HEDLEY_DEPRECATED_FOR(since, replacement) HEDLEY_DIAGNOSTIC_DISABLE_CPP98_COMPAT_WRAP_([[deprecated("Since " #since "; use " #replacement)]])
 #elif \
   HEDLEY_HAS_ATTRIBUTE(deprecated) || \
-  HEDLEY_GCC_VERSION_CHECK(3, 1, 0) || \
-  HEDLEY_ARM_VERSION_CHECK(4, 1, 0) || \
-  HEDLEY_TI_VERSION_CHECK(15, 12, 0) || \
-  (HEDLEY_TI_ARMCL_VERSION_CHECK(4, 8, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-  HEDLEY_TI_ARMCL_VERSION_CHECK(5, 2, 0) || \
-  (HEDLEY_TI_CL2000_VERSION_CHECK(6, 0, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-  HEDLEY_TI_CL2000_VERSION_CHECK(6, 4, 0) || \
-  (HEDLEY_TI_CL430_VERSION_CHECK(4, 0, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-  HEDLEY_TI_CL430_VERSION_CHECK(4, 3, 0) || \
-  (HEDLEY_TI_CL6X_VERSION_CHECK(7, 2, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-  HEDLEY_TI_CL6X_VERSION_CHECK(7, 5, 0) || \
-  HEDLEY_TI_CL7X_VERSION_CHECK(1, 2, 0) || \
-  HEDLEY_TI_CLPRU_VERSION_CHECK(2, 1, 0)
+  HEDLEY_GCC_VERSION_CHECK(3,1,0) || \
+  HEDLEY_ARM_VERSION_CHECK(4,1,0) || \
+  HEDLEY_TI_VERSION_CHECK(15,12,0) || \
+  (HEDLEY_TI_ARMCL_VERSION_CHECK(4,8,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+  HEDLEY_TI_ARMCL_VERSION_CHECK(5,2,0) || \
+  (HEDLEY_TI_CL2000_VERSION_CHECK(6,0,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+  HEDLEY_TI_CL2000_VERSION_CHECK(6,4,0) || \
+  (HEDLEY_TI_CL430_VERSION_CHECK(4,0,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+  HEDLEY_TI_CL430_VERSION_CHECK(4,3,0) || \
+  (HEDLEY_TI_CL6X_VERSION_CHECK(7,2,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+  HEDLEY_TI_CL6X_VERSION_CHECK(7,5,0) || \
+  HEDLEY_TI_CL7X_VERSION_CHECK(1,2,0) || \
+  HEDLEY_TI_CLPRU_VERSION_CHECK(2,1,0) || \
+  HEDLEY_MCST_LCC_VERSION_CHECK(1,25,10) || \
+  HEDLEY_IAR_VERSION_CHECK(8,10,0)
 #  define HEDLEY_DEPRECATED(since) __attribute__((__deprecated__))
 #  define HEDLEY_DEPRECATED_FOR(since, replacement) __attribute__((__deprecated__))
-#elif HEDLEY_MSVC_VERSION_CHECK(14, 0, 0)
-#  define HEDLEY_DEPRECATED(since) __declspec(deprecated("Since " # since))
-#  define HEDLEY_DEPRECATED_FOR(since, replacement) __declspec(deprecated("Since " #since "; use " #replacement))
 #elif \
-  HEDLEY_MSVC_VERSION_CHECK(13, 10, 0) || \
-  HEDLEY_PELLES_VERSION_CHECK(6, 50, 0)
+  HEDLEY_MSVC_VERSION_CHECK(13,10,0) || \
+  HEDLEY_PELLES_VERSION_CHECK(6,50,0) || \
+  HEDLEY_INTEL_CL_VERSION_CHECK(2021,1,0)
 #  define HEDLEY_DEPRECATED(since) __declspec(deprecated)
 #  define HEDLEY_DEPRECATED_FOR(since, replacement) __declspec(deprecated)
-#elif HEDLEY_IAR_VERSION_CHECK(8, 0, 0)
+#elif HEDLEY_IAR_VERSION_CHECK(8,0,0)
 #  define HEDLEY_DEPRECATED(since) _Pragma("deprecated")
 #  define HEDLEY_DEPRECATED_FOR(since, replacement) _Pragma("deprecated")
 #else
 #  define HEDLEY_DEPRECATED(since)
 #  define HEDLEY_DEPRECATED_FOR(since, replacement)
 #endif
 
 #if defined(HEDLEY_UNAVAILABLE)
 #  undef HEDLEY_UNAVAILABLE
 #endif
 #if \
   HEDLEY_HAS_ATTRIBUTE(warning) || \
-  HEDLEY_GCC_VERSION_CHECK(4, 3, 0) || \
-  HEDLEY_INTEL_VERSION_CHECK(13, 0, 0)
+  HEDLEY_GCC_VERSION_CHECK(4,3,0) || \
+  HEDLEY_INTEL_VERSION_CHECK(13,0,0) || \
+  HEDLEY_MCST_LCC_VERSION_CHECK(1,25,10)
 #  define HEDLEY_UNAVAILABLE(available_since) __attribute__((__warning__("Not available until " #available_since)))
 #else
 #  define HEDLEY_UNAVAILABLE(available_since)
 #endif
 
 #if defined(HEDLEY_WARN_UNUSED_RESULT)
 #  undef HEDLEY_WARN_UNUSED_RESULT
 #endif
 #if defined(HEDLEY_WARN_UNUSED_RESULT_MSG)
 #  undef HEDLEY_WARN_UNUSED_RESULT_MSG
 #endif
-#if (HEDLEY_HAS_CPP_ATTRIBUTE(nodiscard) >= 201907L)
+#if \
+  HEDLEY_HAS_ATTRIBUTE(warn_unused_result) || \
+  HEDLEY_GCC_VERSION_CHECK(3,4,0) || \
+  HEDLEY_INTEL_VERSION_CHECK(13,0,0) || \
+  HEDLEY_TI_VERSION_CHECK(15,12,0) || \
+  (HEDLEY_TI_ARMCL_VERSION_CHECK(4,8,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+  HEDLEY_TI_ARMCL_VERSION_CHECK(5,2,0) || \
+  (HEDLEY_TI_CL2000_VERSION_CHECK(6,0,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+  HEDLEY_TI_CL2000_VERSION_CHECK(6,4,0) || \
+  (HEDLEY_TI_CL430_VERSION_CHECK(4,0,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+  HEDLEY_TI_CL430_VERSION_CHECK(4,3,0) || \
+  (HEDLEY_TI_CL6X_VERSION_CHECK(7,2,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+  HEDLEY_TI_CL6X_VERSION_CHECK(7,5,0) || \
+  HEDLEY_TI_CL7X_VERSION_CHECK(1,2,0) || \
+  HEDLEY_TI_CLPRU_VERSION_CHECK(2,1,0) || \
+  (HEDLEY_SUNPRO_VERSION_CHECK(5,15,0) && defined(__cplusplus)) || \
+  HEDLEY_PGI_VERSION_CHECK(17,10,0) || \
+  HEDLEY_MCST_LCC_VERSION_CHECK(1,25,10)
+#  define HEDLEY_WARN_UNUSED_RESULT __attribute__((__warn_unused_result__))
+#  define HEDLEY_WARN_UNUSED_RESULT_MSG(msg) __attribute__((__warn_unused_result__))
+#elif (HEDLEY_HAS_CPP_ATTRIBUTE(nodiscard) >= 201907L)
 #  define HEDLEY_WARN_UNUSED_RESULT HEDLEY_DIAGNOSTIC_DISABLE_CPP98_COMPAT_WRAP_([[nodiscard]])
 #  define HEDLEY_WARN_UNUSED_RESULT_MSG(msg) HEDLEY_DIAGNOSTIC_DISABLE_CPP98_COMPAT_WRAP_([[nodiscard(msg)]])
 #elif HEDLEY_HAS_CPP_ATTRIBUTE(nodiscard)
 #  define HEDLEY_WARN_UNUSED_RESULT HEDLEY_DIAGNOSTIC_DISABLE_CPP98_COMPAT_WRAP_([[nodiscard]])
 #  define HEDLEY_WARN_UNUSED_RESULT_MSG(msg) HEDLEY_DIAGNOSTIC_DISABLE_CPP98_COMPAT_WRAP_([[nodiscard]])
-#elif \
-  HEDLEY_HAS_ATTRIBUTE(warn_unused_result) || \
-  HEDLEY_GCC_VERSION_CHECK(3, 4, 0) || \
-  HEDLEY_INTEL_VERSION_CHECK(13, 0, 0) || \
-  HEDLEY_TI_VERSION_CHECK(15, 12, 0) || \
-  (HEDLEY_TI_ARMCL_VERSION_CHECK(4, 8, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-  HEDLEY_TI_ARMCL_VERSION_CHECK(5, 2, 0) || \
-  (HEDLEY_TI_CL2000_VERSION_CHECK(6, 0, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-  HEDLEY_TI_CL2000_VERSION_CHECK(6, 4, 0) || \
-  (HEDLEY_TI_CL430_VERSION_CHECK(4, 0, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-  HEDLEY_TI_CL430_VERSION_CHECK(4, 3, 0) || \
-  (HEDLEY_TI_CL6X_VERSION_CHECK(7, 2, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-  HEDLEY_TI_CL6X_VERSION_CHECK(7, 5, 0) || \
-  HEDLEY_TI_CL7X_VERSION_CHECK(1, 2, 0) || \
-  HEDLEY_TI_CLPRU_VERSION_CHECK(2, 1, 0) || \
-  (HEDLEY_SUNPRO_VERSION_CHECK(5, 15, 0) && defined(__cplusplus)) || \
-  HEDLEY_PGI_VERSION_CHECK(17, 10, 0)
-#  define HEDLEY_WARN_UNUSED_RESULT __attribute__((__warn_unused_result__))
-#  define HEDLEY_WARN_UNUSED_RESULT_MSG(msg) __attribute__((__warn_unused_result__))
 #elif defined(_Check_return_) /* SAL */
 #  define HEDLEY_WARN_UNUSED_RESULT _Check_return_
 #  define HEDLEY_WARN_UNUSED_RESULT_MSG(msg) _Check_return_
 #else
 #  define HEDLEY_WARN_UNUSED_RESULT
 #  define HEDLEY_WARN_UNUSED_RESULT_MSG(msg)
 #endif
 
 #if defined(HEDLEY_SENTINEL)
 #  undef HEDLEY_SENTINEL
 #endif
 #if \
   HEDLEY_HAS_ATTRIBUTE(sentinel) || \
-  HEDLEY_GCC_VERSION_CHECK(4, 0, 0) || \
-  HEDLEY_INTEL_VERSION_CHECK(13, 0, 0) || \
-  HEDLEY_ARM_VERSION_CHECK(5, 4, 0)
+  HEDLEY_GCC_VERSION_CHECK(4,0,0) || \
+  HEDLEY_INTEL_VERSION_CHECK(13,0,0) || \
+  HEDLEY_ARM_VERSION_CHECK(5,4,0) || \
+  HEDLEY_MCST_LCC_VERSION_CHECK(1,25,10)
 #  define HEDLEY_SENTINEL(position) __attribute__((__sentinel__(position)))
 #else
 #  define HEDLEY_SENTINEL(position)
 #endif
 
 #if defined(HEDLEY_NO_RETURN)
 #  undef HEDLEY_NO_RETURN
 #endif
-#if HEDLEY_IAR_VERSION_CHECK(8, 0, 0)
+#if HEDLEY_IAR_VERSION_CHECK(8,0,0)
 #  define HEDLEY_NO_RETURN __noreturn
-#elif HEDLEY_INTEL_VERSION_CHECK(13, 0, 0)
+#elif \
+  HEDLEY_INTEL_VERSION_CHECK(13,0,0) || \
+  HEDLEY_MCST_LCC_VERSION_CHECK(1,25,10)
 #  define HEDLEY_NO_RETURN __attribute__((__noreturn__))
 #elif defined(__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #  define HEDLEY_NO_RETURN _Noreturn
 #elif defined(__cplusplus) && (__cplusplus >= 201103L)
 #  define HEDLEY_NO_RETURN HEDLEY_DIAGNOSTIC_DISABLE_CPP98_COMPAT_WRAP_([[noreturn]])
 #elif \
   HEDLEY_HAS_ATTRIBUTE(noreturn) || \
-  HEDLEY_GCC_VERSION_CHECK(3, 2, 0) || \
-  HEDLEY_SUNPRO_VERSION_CHECK(5, 11, 0) || \
-  HEDLEY_ARM_VERSION_CHECK(4, 1, 0) || \
-  HEDLEY_IBM_VERSION_CHECK(10, 1, 0) || \
-  HEDLEY_TI_VERSION_CHECK(15, 12, 0) || \
-  (HEDLEY_TI_ARMCL_VERSION_CHECK(4, 8, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-  HEDLEY_TI_ARMCL_VERSION_CHECK(5, 2, 0) || \
-  (HEDLEY_TI_CL2000_VERSION_CHECK(6, 0, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-  HEDLEY_TI_CL2000_VERSION_CHECK(6, 4, 0) || \
-  (HEDLEY_TI_CL430_VERSION_CHECK(4, 0, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-  HEDLEY_TI_CL430_VERSION_CHECK(4, 3, 0) || \
-  (HEDLEY_TI_CL6X_VERSION_CHECK(7, 2, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-  HEDLEY_TI_CL6X_VERSION_CHECK(7, 5, 0) || \
-  HEDLEY_TI_CL7X_VERSION_CHECK(1, 2, 0) || \
-  HEDLEY_TI_CLPRU_VERSION_CHECK(2, 1, 0)
+  HEDLEY_GCC_VERSION_CHECK(3,2,0) || \
+  HEDLEY_SUNPRO_VERSION_CHECK(5,11,0) || \
+  HEDLEY_ARM_VERSION_CHECK(4,1,0) || \
+  HEDLEY_IBM_VERSION_CHECK(10,1,0) || \
+  HEDLEY_TI_VERSION_CHECK(15,12,0) || \
+  (HEDLEY_TI_ARMCL_VERSION_CHECK(4,8,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+  HEDLEY_TI_ARMCL_VERSION_CHECK(5,2,0) || \
+  (HEDLEY_TI_CL2000_VERSION_CHECK(6,0,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+  HEDLEY_TI_CL2000_VERSION_CHECK(6,4,0) || \
+  (HEDLEY_TI_CL430_VERSION_CHECK(4,0,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+  HEDLEY_TI_CL430_VERSION_CHECK(4,3,0) || \
+  (HEDLEY_TI_CL6X_VERSION_CHECK(7,2,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+  HEDLEY_TI_CL6X_VERSION_CHECK(7,5,0) || \
+  HEDLEY_TI_CL7X_VERSION_CHECK(1,2,0) || \
+  HEDLEY_TI_CLPRU_VERSION_CHECK(2,1,0) || \
+  HEDLEY_IAR_VERSION_CHECK(8,10,0)
 #  define HEDLEY_NO_RETURN __attribute__((__noreturn__))
-#elif HEDLEY_SUNPRO_VERSION_CHECK(5, 10, 0)
+#elif HEDLEY_SUNPRO_VERSION_CHECK(5,10,0)
 #  define HEDLEY_NO_RETURN _Pragma("does_not_return")
-#elif HEDLEY_MSVC_VERSION_CHECK(13, 10, 0)
+#elif \
+  HEDLEY_MSVC_VERSION_CHECK(13,10,0) || \
+  HEDLEY_INTEL_CL_VERSION_CHECK(2021,1,0)
 #  define HEDLEY_NO_RETURN __declspec(noreturn)
-#elif HEDLEY_TI_CL6X_VERSION_CHECK(6, 0, 0) && defined(__cplusplus)
+#elif HEDLEY_TI_CL6X_VERSION_CHECK(6,0,0) && defined(__cplusplus)
 #  define HEDLEY_NO_RETURN _Pragma("FUNC_NEVER_RETURNS;")
-#elif HEDLEY_COMPCERT_VERSION_CHECK(3, 2, 0)
+#elif HEDLEY_COMPCERT_VERSION_CHECK(3,2,0)
 #  define HEDLEY_NO_RETURN __attribute((noreturn))
-#elif HEDLEY_PELLES_VERSION_CHECK(9, 0, 0)
+#elif HEDLEY_PELLES_VERSION_CHECK(9,0,0)
 #  define HEDLEY_NO_RETURN __declspec(noreturn)
 #else
 #  define HEDLEY_NO_RETURN
 #endif
 
 #if defined(HEDLEY_NO_ESCAPE)
 #  undef HEDLEY_NO_ESCAPE
@@ -1100,34 +1205,37 @@
 #if defined(HEDLEY_UNREACHABLE_RETURN)
 #  undef HEDLEY_UNREACHABLE_RETURN
 #endif
 #if defined(HEDLEY_ASSUME)
 #  undef HEDLEY_ASSUME
 #endif
 #if \
-  HEDLEY_MSVC_VERSION_CHECK(13, 10, 0) || \
-  HEDLEY_INTEL_VERSION_CHECK(13, 0, 0)
+  HEDLEY_MSVC_VERSION_CHECK(13,10,0) || \
+  HEDLEY_INTEL_VERSION_CHECK(13,0,0) || \
+  HEDLEY_INTEL_CL_VERSION_CHECK(2021,1,0)
 #  define HEDLEY_ASSUME(expr) __assume(expr)
 #elif HEDLEY_HAS_BUILTIN(__builtin_assume)
 #  define HEDLEY_ASSUME(expr) __builtin_assume(expr)
 #elif \
-    HEDLEY_TI_CL2000_VERSION_CHECK(6, 2, 0) || \
-    HEDLEY_TI_CL6X_VERSION_CHECK(4, 0, 0)
+    HEDLEY_TI_CL2000_VERSION_CHECK(6,2,0) || \
+    HEDLEY_TI_CL6X_VERSION_CHECK(4,0,0)
 #  if defined(__cplusplus)
 #    define HEDLEY_ASSUME(expr) std::_nassert(expr)
 #  else
 #    define HEDLEY_ASSUME(expr) _nassert(expr)
 #  endif
 #endif
 #if \
   (HEDLEY_HAS_BUILTIN(__builtin_unreachable) && (!defined(HEDLEY_ARM_VERSION))) || \
-  HEDLEY_GCC_VERSION_CHECK(4, 5, 0) || \
-  HEDLEY_PGI_VERSION_CHECK(18, 10, 0) || \
-  HEDLEY_INTEL_VERSION_CHECK(13, 0, 0) || \
-  HEDLEY_IBM_VERSION_CHECK(13, 1, 5)
+  HEDLEY_GCC_VERSION_CHECK(4,5,0) || \
+  HEDLEY_PGI_VERSION_CHECK(18,10,0) || \
+  HEDLEY_INTEL_VERSION_CHECK(13,0,0) || \
+  HEDLEY_IBM_VERSION_CHECK(13,1,5) || \
+  HEDLEY_CRAY_VERSION_CHECK(10,0,0) || \
+  HEDLEY_MCST_LCC_VERSION_CHECK(1,25,10)
 #  define HEDLEY_UNREACHABLE() __builtin_unreachable()
 #elif defined(HEDLEY_ASSUME)
 #  define HEDLEY_UNREACHABLE() HEDLEY_ASSUME(0)
 #endif
 #if !defined(HEDLEY_ASSUME)
 #  if defined(HEDLEY_UNREACHABLE)
 #    define HEDLEY_ASSUME(expr) HEDLEY_STATIC_CAST(void, ((expr) ? 1 : (HEDLEY_UNREACHABLE(), 1)))
@@ -1153,64 +1261,65 @@
 HEDLEY_DIAGNOSTIC_PUSH
 #if HEDLEY_HAS_WARNING("-Wpedantic")
 #  pragma clang diagnostic ignored "-Wpedantic"
 #endif
 #if HEDLEY_HAS_WARNING("-Wc++98-compat-pedantic") && defined(__cplusplus)
 #  pragma clang diagnostic ignored "-Wc++98-compat-pedantic"
 #endif
-#if HEDLEY_GCC_HAS_WARNING("-Wvariadic-macros", 4, 0, 0)
+#if HEDLEY_GCC_HAS_WARNING("-Wvariadic-macros",4,0,0)
 #  if defined(__clang__)
 #    pragma clang diagnostic ignored "-Wvariadic-macros"
 #  elif defined(HEDLEY_GCC_VERSION)
 #    pragma GCC diagnostic ignored "-Wvariadic-macros"
 #  endif
 #endif
 #if defined(HEDLEY_NON_NULL)
 #  undef HEDLEY_NON_NULL
 #endif
 #if \
   HEDLEY_HAS_ATTRIBUTE(nonnull) || \
-  HEDLEY_GCC_VERSION_CHECK(3, 3, 0) || \
-  HEDLEY_INTEL_VERSION_CHECK(13, 0, 0) || \
-  HEDLEY_ARM_VERSION_CHECK(4, 1, 0)
+  HEDLEY_GCC_VERSION_CHECK(3,3,0) || \
+  HEDLEY_INTEL_VERSION_CHECK(13,0,0) || \
+  HEDLEY_ARM_VERSION_CHECK(4,1,0)
 #  define HEDLEY_NON_NULL(...) __attribute__((__nonnull__(__VA_ARGS__)))
 #else
 #  define HEDLEY_NON_NULL(...)
 #endif
 HEDLEY_DIAGNOSTIC_POP
 
 #if defined(HEDLEY_PRINTF_FORMAT)
 #  undef HEDLEY_PRINTF_FORMAT
 #endif
-#if defined(__MINGW32__) && HEDLEY_GCC_HAS_ATTRIBUTE(format, 4, 4, 0) && !defined(__USE_MINGW_ANSI_STDIO)
+#if defined(__MINGW32__) && HEDLEY_GCC_HAS_ATTRIBUTE(format,4,4,0) && !defined(__USE_MINGW_ANSI_STDIO)
 #  define HEDLEY_PRINTF_FORMAT(string_idx,first_to_check) __attribute__((__format__(ms_printf, string_idx, first_to_check)))
-#elif defined(__MINGW32__) && HEDLEY_GCC_HAS_ATTRIBUTE(format, 4, 4, 0) && defined(__USE_MINGW_ANSI_STDIO)
+#elif defined(__MINGW32__) && HEDLEY_GCC_HAS_ATTRIBUTE(format,4,4,0) && defined(__USE_MINGW_ANSI_STDIO)
 #  define HEDLEY_PRINTF_FORMAT(string_idx,first_to_check) __attribute__((__format__(gnu_printf, string_idx, first_to_check)))
 #elif \
   HEDLEY_HAS_ATTRIBUTE(format) || \
-  HEDLEY_GCC_VERSION_CHECK(3, 1, 0) || \
-  HEDLEY_INTEL_VERSION_CHECK(13, 0, 0) || \
-  HEDLEY_ARM_VERSION_CHECK(5, 6, 0) || \
-  HEDLEY_IBM_VERSION_CHECK(10, 1, 0) || \
-  HEDLEY_TI_VERSION_CHECK(15, 12, 0) || \
-  (HEDLEY_TI_ARMCL_VERSION_CHECK(4, 8, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-  HEDLEY_TI_ARMCL_VERSION_CHECK(5, 2, 0) || \
-  (HEDLEY_TI_CL2000_VERSION_CHECK(6, 0, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-  HEDLEY_TI_CL2000_VERSION_CHECK(6, 4, 0) || \
-  (HEDLEY_TI_CL430_VERSION_CHECK(4, 0, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-  HEDLEY_TI_CL430_VERSION_CHECK(4, 3, 0) || \
-  (HEDLEY_TI_CL6X_VERSION_CHECK(7, 2, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-  HEDLEY_TI_CL6X_VERSION_CHECK(7, 5, 0) || \
-  HEDLEY_TI_CL7X_VERSION_CHECK(1, 2, 0) || \
-  HEDLEY_TI_CLPRU_VERSION_CHECK(2, 1, 0)
+  HEDLEY_GCC_VERSION_CHECK(3,1,0) || \
+  HEDLEY_INTEL_VERSION_CHECK(13,0,0) || \
+  HEDLEY_ARM_VERSION_CHECK(5,6,0) || \
+  HEDLEY_IBM_VERSION_CHECK(10,1,0) || \
+  HEDLEY_TI_VERSION_CHECK(15,12,0) || \
+  (HEDLEY_TI_ARMCL_VERSION_CHECK(4,8,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+  HEDLEY_TI_ARMCL_VERSION_CHECK(5,2,0) || \
+  (HEDLEY_TI_CL2000_VERSION_CHECK(6,0,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+  HEDLEY_TI_CL2000_VERSION_CHECK(6,4,0) || \
+  (HEDLEY_TI_CL430_VERSION_CHECK(4,0,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+  HEDLEY_TI_CL430_VERSION_CHECK(4,3,0) || \
+  (HEDLEY_TI_CL6X_VERSION_CHECK(7,2,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+  HEDLEY_TI_CL6X_VERSION_CHECK(7,5,0) || \
+  HEDLEY_TI_CL7X_VERSION_CHECK(1,2,0) || \
+  HEDLEY_TI_CLPRU_VERSION_CHECK(2,1,0) || \
+  HEDLEY_MCST_LCC_VERSION_CHECK(1,25,10)
 #  define HEDLEY_PRINTF_FORMAT(string_idx,first_to_check) __attribute__((__format__(__printf__, string_idx, first_to_check)))
-#elif HEDLEY_PELLES_VERSION_CHECK(6, 0, 0)
+#elif HEDLEY_PELLES_VERSION_CHECK(6,0,0)
 #  define HEDLEY_PRINTF_FORMAT(string_idx,first_to_check) __declspec(vaformat(printf,string_idx,first_to_check))
 #else
-#  define HEDLEY_PRINTF_FORMAT(string_idx, first_to_check)
+#  define HEDLEY_PRINTF_FORMAT(string_idx,first_to_check)
 #endif
 
 #if defined(HEDLEY_CONSTEXPR)
 #  undef HEDLEY_CONSTEXPR
 #endif
 #if defined(__cplusplus)
 #  if __cplusplus >= 201103L
@@ -1233,37 +1342,39 @@
 #if defined(HEDLEY_UNPREDICTABLE)
 #  undef HEDLEY_UNPREDICTABLE
 #endif
 #if HEDLEY_HAS_BUILTIN(__builtin_unpredictable)
 #  define HEDLEY_UNPREDICTABLE(expr) __builtin_unpredictable((expr))
 #endif
 #if \
-  (HEDLEY_HAS_BUILTIN(__builtin_expect_with_probability) || \
-  HEDLEY_GCC_VERSION_CHECK(9, 0, 0)) && !defined(HEDLEY_INTEL_VERSION)
+  (HEDLEY_HAS_BUILTIN(__builtin_expect_with_probability) && !defined(HEDLEY_PGI_VERSION)) || \
+  HEDLEY_GCC_VERSION_CHECK(9,0,0) || \
+  HEDLEY_MCST_LCC_VERSION_CHECK(1,25,10)
 #  define HEDLEY_PREDICT(expr, value, probability) __builtin_expect_with_probability(  (expr), (value), (probability))
 #  define HEDLEY_PREDICT_TRUE(expr, probability)   __builtin_expect_with_probability(!!(expr),    1   , (probability))
 #  define HEDLEY_PREDICT_FALSE(expr, probability)  __builtin_expect_with_probability(!!(expr),    0   , (probability))
 #  define HEDLEY_LIKELY(expr)                      __builtin_expect                 (!!(expr),    1                  )
 #  define HEDLEY_UNLIKELY(expr)                    __builtin_expect                 (!!(expr),    0                  )
 #elif \
-  HEDLEY_HAS_BUILTIN(__builtin_expect) || \
-  HEDLEY_GCC_VERSION_CHECK(3, 0, 0) || \
-  HEDLEY_INTEL_VERSION_CHECK(13, 0, 0) || \
-  (HEDLEY_SUNPRO_VERSION_CHECK(5, 15, 0) && defined(__cplusplus)) || \
-  HEDLEY_ARM_VERSION_CHECK(4, 1, 0) || \
-  HEDLEY_IBM_VERSION_CHECK(10, 1, 0) || \
-  HEDLEY_TI_VERSION_CHECK(15, 12, 0) || \
-  HEDLEY_TI_ARMCL_VERSION_CHECK(4, 7, 0) || \
-  HEDLEY_TI_CL430_VERSION_CHECK(3, 1, 0) || \
-  HEDLEY_TI_CL2000_VERSION_CHECK(6, 1, 0) || \
-  HEDLEY_TI_CL6X_VERSION_CHECK(6, 1, 0) || \
-  HEDLEY_TI_CL7X_VERSION_CHECK(1, 2, 0) || \
-  HEDLEY_TI_CLPRU_VERSION_CHECK(2, 1, 0) || \
-  HEDLEY_TINYC_VERSION_CHECK(0, 9, 27) || \
-  HEDLEY_CRAY_VERSION_CHECK(8, 1, 0)
+  (HEDLEY_HAS_BUILTIN(__builtin_expect) && !defined(HEDLEY_INTEL_CL_VERSION)) || \
+  HEDLEY_GCC_VERSION_CHECK(3,0,0) || \
+  HEDLEY_INTEL_VERSION_CHECK(13,0,0) || \
+  (HEDLEY_SUNPRO_VERSION_CHECK(5,15,0) && defined(__cplusplus)) || \
+  HEDLEY_ARM_VERSION_CHECK(4,1,0) || \
+  HEDLEY_IBM_VERSION_CHECK(10,1,0) || \
+  HEDLEY_TI_VERSION_CHECK(15,12,0) || \
+  HEDLEY_TI_ARMCL_VERSION_CHECK(4,7,0) || \
+  HEDLEY_TI_CL430_VERSION_CHECK(3,1,0) || \
+  HEDLEY_TI_CL2000_VERSION_CHECK(6,1,0) || \
+  HEDLEY_TI_CL6X_VERSION_CHECK(6,1,0) || \
+  HEDLEY_TI_CL7X_VERSION_CHECK(1,2,0) || \
+  HEDLEY_TI_CLPRU_VERSION_CHECK(2,1,0) || \
+  HEDLEY_TINYC_VERSION_CHECK(0,9,27) || \
+  HEDLEY_CRAY_VERSION_CHECK(8,1,0) || \
+  HEDLEY_MCST_LCC_VERSION_CHECK(1,25,10)
 #  define HEDLEY_PREDICT(expr, expected, probability) \
      (((probability) >= 0.9) ? __builtin_expect((expr), (expected)) : (HEDLEY_STATIC_CAST(void, expected), (expr)))
 #  define HEDLEY_PREDICT_TRUE(expr, probability) \
      (__extension__ ({ \
        double hedley_probability_ = (probability); \
        ((hedley_probability_ >= 0.9) ? __builtin_expect(!!(expr), 1) : ((hedley_probability_ <= 0.1) ? __builtin_expect(!!(expr), 0) : !!(expr))); \
      }))
@@ -1286,229 +1397,246 @@
 #endif
 
 #if defined(HEDLEY_MALLOC)
 #  undef HEDLEY_MALLOC
 #endif
 #if \
   HEDLEY_HAS_ATTRIBUTE(malloc) || \
-  HEDLEY_GCC_VERSION_CHECK(3, 1, 0) || \
-  HEDLEY_INTEL_VERSION_CHECK(13, 0, 0) || \
-  HEDLEY_SUNPRO_VERSION_CHECK(5, 11, 0) || \
-  HEDLEY_ARM_VERSION_CHECK(4, 1, 0) || \
-  HEDLEY_IBM_VERSION_CHECK(12, 1, 0) || \
-  HEDLEY_TI_VERSION_CHECK(15, 12, 0) || \
-  (HEDLEY_TI_ARMCL_VERSION_CHECK(4, 8, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-  HEDLEY_TI_ARMCL_VERSION_CHECK(5, 2, 0) || \
-  (HEDLEY_TI_CL2000_VERSION_CHECK(6, 0, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-  HEDLEY_TI_CL2000_VERSION_CHECK(6, 4, 0) || \
-  (HEDLEY_TI_CL430_VERSION_CHECK(4, 0, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-  HEDLEY_TI_CL430_VERSION_CHECK(4, 3, 0) || \
-  (HEDLEY_TI_CL6X_VERSION_CHECK(7, 2, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-  HEDLEY_TI_CL6X_VERSION_CHECK(7, 5, 0) || \
-  HEDLEY_TI_CL7X_VERSION_CHECK(1, 2, 0) || \
-  HEDLEY_TI_CLPRU_VERSION_CHECK(2, 1, 0)
+  HEDLEY_GCC_VERSION_CHECK(3,1,0) || \
+  HEDLEY_INTEL_VERSION_CHECK(13,0,0) || \
+  HEDLEY_SUNPRO_VERSION_CHECK(5,11,0) || \
+  HEDLEY_ARM_VERSION_CHECK(4,1,0) || \
+  HEDLEY_IBM_VERSION_CHECK(12,1,0) || \
+  HEDLEY_TI_VERSION_CHECK(15,12,0) || \
+  (HEDLEY_TI_ARMCL_VERSION_CHECK(4,8,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+  HEDLEY_TI_ARMCL_VERSION_CHECK(5,2,0) || \
+  (HEDLEY_TI_CL2000_VERSION_CHECK(6,0,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+  HEDLEY_TI_CL2000_VERSION_CHECK(6,4,0) || \
+  (HEDLEY_TI_CL430_VERSION_CHECK(4,0,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+  HEDLEY_TI_CL430_VERSION_CHECK(4,3,0) || \
+  (HEDLEY_TI_CL6X_VERSION_CHECK(7,2,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+  HEDLEY_TI_CL6X_VERSION_CHECK(7,5,0) || \
+  HEDLEY_TI_CL7X_VERSION_CHECK(1,2,0) || \
+  HEDLEY_TI_CLPRU_VERSION_CHECK(2,1,0) || \
+  HEDLEY_MCST_LCC_VERSION_CHECK(1,25,10)
 #  define HEDLEY_MALLOC __attribute__((__malloc__))
-#elif HEDLEY_SUNPRO_VERSION_CHECK(5, 10, 0)
+#elif HEDLEY_SUNPRO_VERSION_CHECK(5,10,0)
 #  define HEDLEY_MALLOC _Pragma("returns_new_memory")
-#elif HEDLEY_MSVC_VERSION_CHECK(14, 0, 0)
+#elif \
+  HEDLEY_MSVC_VERSION_CHECK(14,0,0) || \
+  HEDLEY_INTEL_CL_VERSION_CHECK(2021,1,0)
 #  define HEDLEY_MALLOC __declspec(restrict)
 #else
 #  define HEDLEY_MALLOC
 #endif
 
 #if defined(HEDLEY_PURE)
 #  undef HEDLEY_PURE
 #endif
 #if \
   HEDLEY_HAS_ATTRIBUTE(pure) || \
-  HEDLEY_GCC_VERSION_CHECK(2, 96, 0) || \
-  HEDLEY_INTEL_VERSION_CHECK(13, 0, 0) || \
-  HEDLEY_SUNPRO_VERSION_CHECK(5, 11, 0) || \
-  HEDLEY_ARM_VERSION_CHECK(4, 1, 0) || \
-  HEDLEY_IBM_VERSION_CHECK(10, 1, 0) || \
-  HEDLEY_TI_VERSION_CHECK(15, 12, 0) || \
-  (HEDLEY_TI_ARMCL_VERSION_CHECK(4, 8, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-  HEDLEY_TI_ARMCL_VERSION_CHECK(5, 2, 0) || \
-  (HEDLEY_TI_CL2000_VERSION_CHECK(6, 0, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-  HEDLEY_TI_CL2000_VERSION_CHECK(6, 4, 0) || \
-  (HEDLEY_TI_CL430_VERSION_CHECK(4, 0, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-  HEDLEY_TI_CL430_VERSION_CHECK(4, 3, 0) || \
-  (HEDLEY_TI_CL6X_VERSION_CHECK(7, 2, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-  HEDLEY_TI_CL6X_VERSION_CHECK(7, 5, 0) || \
-  HEDLEY_TI_CL7X_VERSION_CHECK(1, 2, 0) || \
-  HEDLEY_TI_CLPRU_VERSION_CHECK(2, 1, 0) || \
-  HEDLEY_PGI_VERSION_CHECK(17, 10, 0)
+  HEDLEY_GCC_VERSION_CHECK(2,96,0) || \
+  HEDLEY_INTEL_VERSION_CHECK(13,0,0) || \
+  HEDLEY_SUNPRO_VERSION_CHECK(5,11,0) || \
+  HEDLEY_ARM_VERSION_CHECK(4,1,0) || \
+  HEDLEY_IBM_VERSION_CHECK(10,1,0) || \
+  HEDLEY_TI_VERSION_CHECK(15,12,0) || \
+  (HEDLEY_TI_ARMCL_VERSION_CHECK(4,8,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+  HEDLEY_TI_ARMCL_VERSION_CHECK(5,2,0) || \
+  (HEDLEY_TI_CL2000_VERSION_CHECK(6,0,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+  HEDLEY_TI_CL2000_VERSION_CHECK(6,4,0) || \
+  (HEDLEY_TI_CL430_VERSION_CHECK(4,0,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+  HEDLEY_TI_CL430_VERSION_CHECK(4,3,0) || \
+  (HEDLEY_TI_CL6X_VERSION_CHECK(7,2,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+  HEDLEY_TI_CL6X_VERSION_CHECK(7,5,0) || \
+  HEDLEY_TI_CL7X_VERSION_CHECK(1,2,0) || \
+  HEDLEY_TI_CLPRU_VERSION_CHECK(2,1,0) || \
+  HEDLEY_PGI_VERSION_CHECK(17,10,0) || \
+  HEDLEY_MCST_LCC_VERSION_CHECK(1,25,10)
 #  define HEDLEY_PURE __attribute__((__pure__))
-#elif HEDLEY_SUNPRO_VERSION_CHECK(5, 10, 0)
+#elif HEDLEY_SUNPRO_VERSION_CHECK(5,10,0)
 #  define HEDLEY_PURE _Pragma("does_not_write_global_data")
 #elif defined(__cplusplus) && \
-    (\
-      HEDLEY_TI_CL430_VERSION_CHECK(2, 0, 1) || \
-      HEDLEY_TI_CL6X_VERSION_CHECK(4, 0, 0) || \
-      HEDLEY_TI_CL7X_VERSION_CHECK(1, 2, 0) \
-)
+    ( \
+      HEDLEY_TI_CL430_VERSION_CHECK(2,0,1) || \
+      HEDLEY_TI_CL6X_VERSION_CHECK(4,0,0) || \
+      HEDLEY_TI_CL7X_VERSION_CHECK(1,2,0) \
+    )
 #  define HEDLEY_PURE _Pragma("FUNC_IS_PURE;")
 #else
 #  define HEDLEY_PURE
 #endif
 
 #if defined(HEDLEY_CONST)
 #  undef HEDLEY_CONST
 #endif
 #if \
   HEDLEY_HAS_ATTRIBUTE(const) || \
-  HEDLEY_GCC_VERSION_CHECK(2, 5, 0) || \
-  HEDLEY_INTEL_VERSION_CHECK(13, 0, 0) || \
-  HEDLEY_SUNPRO_VERSION_CHECK(5, 11, 0) || \
-  HEDLEY_ARM_VERSION_CHECK(4, 1, 0) || \
-  HEDLEY_IBM_VERSION_CHECK(10, 1, 0) || \
-  HEDLEY_TI_VERSION_CHECK(15, 12, 0) || \
-  (HEDLEY_TI_ARMCL_VERSION_CHECK(4, 8, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-  HEDLEY_TI_ARMCL_VERSION_CHECK(5, 2, 0) || \
-  (HEDLEY_TI_CL2000_VERSION_CHECK(6, 0, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-  HEDLEY_TI_CL2000_VERSION_CHECK(6, 4, 0) || \
-  (HEDLEY_TI_CL430_VERSION_CHECK(4, 0, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-  HEDLEY_TI_CL430_VERSION_CHECK(4, 3, 0) || \
-  (HEDLEY_TI_CL6X_VERSION_CHECK(7, 2, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-  HEDLEY_TI_CL6X_VERSION_CHECK(7, 5, 0) || \
-  HEDLEY_TI_CL7X_VERSION_CHECK(1, 2, 0) || \
-  HEDLEY_TI_CLPRU_VERSION_CHECK(2, 1, 0) || \
-  HEDLEY_PGI_VERSION_CHECK(17, 10, 0)
+  HEDLEY_GCC_VERSION_CHECK(2,5,0) || \
+  HEDLEY_INTEL_VERSION_CHECK(13,0,0) || \
+  HEDLEY_SUNPRO_VERSION_CHECK(5,11,0) || \
+  HEDLEY_ARM_VERSION_CHECK(4,1,0) || \
+  HEDLEY_IBM_VERSION_CHECK(10,1,0) || \
+  HEDLEY_TI_VERSION_CHECK(15,12,0) || \
+  (HEDLEY_TI_ARMCL_VERSION_CHECK(4,8,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+  HEDLEY_TI_ARMCL_VERSION_CHECK(5,2,0) || \
+  (HEDLEY_TI_CL2000_VERSION_CHECK(6,0,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+  HEDLEY_TI_CL2000_VERSION_CHECK(6,4,0) || \
+  (HEDLEY_TI_CL430_VERSION_CHECK(4,0,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+  HEDLEY_TI_CL430_VERSION_CHECK(4,3,0) || \
+  (HEDLEY_TI_CL6X_VERSION_CHECK(7,2,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+  HEDLEY_TI_CL6X_VERSION_CHECK(7,5,0) || \
+  HEDLEY_TI_CL7X_VERSION_CHECK(1,2,0) || \
+  HEDLEY_TI_CLPRU_VERSION_CHECK(2,1,0) || \
+  HEDLEY_PGI_VERSION_CHECK(17,10,0) || \
+  HEDLEY_MCST_LCC_VERSION_CHECK(1,25,10)
 #  define HEDLEY_CONST __attribute__((__const__))
 #elif \
-  HEDLEY_SUNPRO_VERSION_CHECK(5, 10, 0)
+  HEDLEY_SUNPRO_VERSION_CHECK(5,10,0)
 #  define HEDLEY_CONST _Pragma("no_side_effect")
 #else
 #  define HEDLEY_CONST HEDLEY_PURE
 #endif
 
 #if defined(HEDLEY_RESTRICT)
 #  undef HEDLEY_RESTRICT
 #endif
 #if defined(__STDC_VERSION__) && (__STDC_VERSION__ >= 199901L) && !defined(__cplusplus)
 #  define HEDLEY_RESTRICT restrict
 #elif \
-  HEDLEY_GCC_VERSION_CHECK(3, 1, 0) || \
-  HEDLEY_MSVC_VERSION_CHECK(14, 0, 0) || \
-  HEDLEY_INTEL_VERSION_CHECK(13, 0, 0) || \
-  HEDLEY_ARM_VERSION_CHECK(4, 1, 0) || \
-  HEDLEY_IBM_VERSION_CHECK(10, 1, 0) || \
-  HEDLEY_PGI_VERSION_CHECK(17, 10, 0) || \
-  HEDLEY_TI_CL430_VERSION_CHECK(4, 3, 0) || \
-  HEDLEY_TI_CL2000_VERSION_CHECK(6, 2, 4) || \
-  HEDLEY_TI_CL6X_VERSION_CHECK(8, 1, 0) || \
-  HEDLEY_TI_CL7X_VERSION_CHECK(1, 2, 0) || \
-  (HEDLEY_SUNPRO_VERSION_CHECK(5, 14, 0) && defined(__cplusplus)) || \
-  HEDLEY_IAR_VERSION_CHECK(8, 0, 0) || \
-  defined(__clang__)
+  HEDLEY_GCC_VERSION_CHECK(3,1,0) || \
+  HEDLEY_MSVC_VERSION_CHECK(14,0,0) || \
+  HEDLEY_INTEL_VERSION_CHECK(13,0,0) || \
+  HEDLEY_INTEL_CL_VERSION_CHECK(2021,1,0) || \
+  HEDLEY_ARM_VERSION_CHECK(4,1,0) || \
+  HEDLEY_IBM_VERSION_CHECK(10,1,0) || \
+  HEDLEY_PGI_VERSION_CHECK(17,10,0) || \
+  HEDLEY_TI_CL430_VERSION_CHECK(4,3,0) || \
+  HEDLEY_TI_CL2000_VERSION_CHECK(6,2,4) || \
+  HEDLEY_TI_CL6X_VERSION_CHECK(8,1,0) || \
+  HEDLEY_TI_CL7X_VERSION_CHECK(1,2,0) || \
+  (HEDLEY_SUNPRO_VERSION_CHECK(5,14,0) && defined(__cplusplus)) || \
+  HEDLEY_IAR_VERSION_CHECK(8,0,0) || \
+  defined(__clang__) || \
+  HEDLEY_MCST_LCC_VERSION_CHECK(1,25,10)
 #  define HEDLEY_RESTRICT __restrict
-#elif HEDLEY_SUNPRO_VERSION_CHECK(5, 3, 0) && !defined(__cplusplus)
+#elif HEDLEY_SUNPRO_VERSION_CHECK(5,3,0) && !defined(__cplusplus)
 #  define HEDLEY_RESTRICT _Restrict
 #else
 #  define HEDLEY_RESTRICT
 #endif
 
 #if defined(HEDLEY_INLINE)
 #  undef HEDLEY_INLINE
 #endif
 #if \
   (defined(__STDC_VERSION__) && (__STDC_VERSION__ >= 199901L)) || \
   (defined(__cplusplus) && (__cplusplus >= 199711L))
 #  define HEDLEY_INLINE inline
 #elif \
   defined(HEDLEY_GCC_VERSION) || \
-  HEDLEY_ARM_VERSION_CHECK(6, 2, 0)
+  HEDLEY_ARM_VERSION_CHECK(6,2,0)
 #  define HEDLEY_INLINE __inline__
 #elif \
-  HEDLEY_MSVC_VERSION_CHECK(12, 0, 0) || \
-  HEDLEY_ARM_VERSION_CHECK(4, 1, 0) || \
-  HEDLEY_TI_ARMCL_VERSION_CHECK(5, 1, 0) || \
-  HEDLEY_TI_CL430_VERSION_CHECK(3, 1, 0) || \
-  HEDLEY_TI_CL2000_VERSION_CHECK(6, 2, 0) || \
-  HEDLEY_TI_CL6X_VERSION_CHECK(8, 0, 0) || \
-  HEDLEY_TI_CL7X_VERSION_CHECK(1, 2, 0) || \
-  HEDLEY_TI_CLPRU_VERSION_CHECK(2, 1, 0)
+  HEDLEY_MSVC_VERSION_CHECK(12,0,0) || \
+  HEDLEY_INTEL_CL_VERSION_CHECK(2021,1,0) || \
+  HEDLEY_ARM_VERSION_CHECK(4,1,0) || \
+  HEDLEY_TI_ARMCL_VERSION_CHECK(5,1,0) || \
+  HEDLEY_TI_CL430_VERSION_CHECK(3,1,0) || \
+  HEDLEY_TI_CL2000_VERSION_CHECK(6,2,0) || \
+  HEDLEY_TI_CL6X_VERSION_CHECK(8,0,0) || \
+  HEDLEY_TI_CL7X_VERSION_CHECK(1,2,0) || \
+  HEDLEY_TI_CLPRU_VERSION_CHECK(2,1,0) || \
+  HEDLEY_MCST_LCC_VERSION_CHECK(1,25,10)
 #  define HEDLEY_INLINE __inline
 #else
 #  define HEDLEY_INLINE
 #endif
 
 #if defined(HEDLEY_ALWAYS_INLINE)
 #  undef HEDLEY_ALWAYS_INLINE
 #endif
 #if \
   HEDLEY_HAS_ATTRIBUTE(always_inline) || \
-  HEDLEY_GCC_VERSION_CHECK(4, 0, 0) || \
-  HEDLEY_INTEL_VERSION_CHECK(13, 0, 0) || \
-  HEDLEY_SUNPRO_VERSION_CHECK(5, 11, 0) || \
-  HEDLEY_ARM_VERSION_CHECK(4, 1, 0) || \
-  HEDLEY_IBM_VERSION_CHECK(10, 1, 0) || \
-  HEDLEY_TI_VERSION_CHECK(15, 12, 0) || \
-  (HEDLEY_TI_ARMCL_VERSION_CHECK(4, 8, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-  HEDLEY_TI_ARMCL_VERSION_CHECK(5, 2, 0) || \
-  (HEDLEY_TI_CL2000_VERSION_CHECK(6, 0, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-  HEDLEY_TI_CL2000_VERSION_CHECK(6, 4, 0) || \
-  (HEDLEY_TI_CL430_VERSION_CHECK(4, 0, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-  HEDLEY_TI_CL430_VERSION_CHECK(4, 3, 0) || \
-  (HEDLEY_TI_CL6X_VERSION_CHECK(7, 2, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-  HEDLEY_TI_CL6X_VERSION_CHECK(7, 5, 0) || \
-  HEDLEY_TI_CL7X_VERSION_CHECK(1, 2, 0) || \
-  HEDLEY_TI_CLPRU_VERSION_CHECK(2, 1, 0)
+  HEDLEY_GCC_VERSION_CHECK(4,0,0) || \
+  HEDLEY_INTEL_VERSION_CHECK(13,0,0) || \
+  HEDLEY_SUNPRO_VERSION_CHECK(5,11,0) || \
+  HEDLEY_ARM_VERSION_CHECK(4,1,0) || \
+  HEDLEY_IBM_VERSION_CHECK(10,1,0) || \
+  HEDLEY_TI_VERSION_CHECK(15,12,0) || \
+  (HEDLEY_TI_ARMCL_VERSION_CHECK(4,8,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+  HEDLEY_TI_ARMCL_VERSION_CHECK(5,2,0) || \
+  (HEDLEY_TI_CL2000_VERSION_CHECK(6,0,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+  HEDLEY_TI_CL2000_VERSION_CHECK(6,4,0) || \
+  (HEDLEY_TI_CL430_VERSION_CHECK(4,0,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+  HEDLEY_TI_CL430_VERSION_CHECK(4,3,0) || \
+  (HEDLEY_TI_CL6X_VERSION_CHECK(7,2,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+  HEDLEY_TI_CL6X_VERSION_CHECK(7,5,0) || \
+  HEDLEY_TI_CL7X_VERSION_CHECK(1,2,0) || \
+  HEDLEY_TI_CLPRU_VERSION_CHECK(2,1,0) || \
+  HEDLEY_MCST_LCC_VERSION_CHECK(1,25,10) || \
+  HEDLEY_IAR_VERSION_CHECK(8,10,0)
 #  define HEDLEY_ALWAYS_INLINE __attribute__((__always_inline__)) HEDLEY_INLINE
-#elif HEDLEY_MSVC_VERSION_CHECK(12, 0, 0)
+#elif \
+  HEDLEY_MSVC_VERSION_CHECK(12,0,0) || \
+  HEDLEY_INTEL_CL_VERSION_CHECK(2021,1,0)
 #  define HEDLEY_ALWAYS_INLINE __forceinline
 #elif defined(__cplusplus) && \
-    (\
-      HEDLEY_TI_ARMCL_VERSION_CHECK(5, 2, 0) || \
-      HEDLEY_TI_CL430_VERSION_CHECK(4, 3, 0) || \
-      HEDLEY_TI_CL2000_VERSION_CHECK(6, 4, 0) || \
-      HEDLEY_TI_CL6X_VERSION_CHECK(6, 1, 0) || \
-      HEDLEY_TI_CL7X_VERSION_CHECK(1, 2, 0) || \
-      HEDLEY_TI_CLPRU_VERSION_CHECK(2, 1, 0) \
-)
+    ( \
+      HEDLEY_TI_ARMCL_VERSION_CHECK(5,2,0) || \
+      HEDLEY_TI_CL430_VERSION_CHECK(4,3,0) || \
+      HEDLEY_TI_CL2000_VERSION_CHECK(6,4,0) || \
+      HEDLEY_TI_CL6X_VERSION_CHECK(6,1,0) || \
+      HEDLEY_TI_CL7X_VERSION_CHECK(1,2,0) || \
+      HEDLEY_TI_CLPRU_VERSION_CHECK(2,1,0) \
+    )
 #  define HEDLEY_ALWAYS_INLINE _Pragma("FUNC_ALWAYS_INLINE;")
-#elif HEDLEY_IAR_VERSION_CHECK(8, 0, 0)
+#elif HEDLEY_IAR_VERSION_CHECK(8,0,0)
 #  define HEDLEY_ALWAYS_INLINE _Pragma("inline=forced")
 #else
 #  define HEDLEY_ALWAYS_INLINE HEDLEY_INLINE
 #endif
 
 #if defined(HEDLEY_NEVER_INLINE)
 #  undef HEDLEY_NEVER_INLINE
 #endif
 #if \
   HEDLEY_HAS_ATTRIBUTE(noinline) || \
-  HEDLEY_GCC_VERSION_CHECK(4, 0, 0) || \
-  HEDLEY_INTEL_VERSION_CHECK(13, 0, 0) || \
-  HEDLEY_SUNPRO_VERSION_CHECK(5, 11, 0) || \
-  HEDLEY_ARM_VERSION_CHECK(4, 1, 0) || \
-  HEDLEY_IBM_VERSION_CHECK(10, 1, 0) || \
-  HEDLEY_TI_VERSION_CHECK(15, 12, 0) || \
-  (HEDLEY_TI_ARMCL_VERSION_CHECK(4, 8, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-  HEDLEY_TI_ARMCL_VERSION_CHECK(5, 2, 0) || \
-  (HEDLEY_TI_CL2000_VERSION_CHECK(6, 0, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-  HEDLEY_TI_CL2000_VERSION_CHECK(6, 4, 0) || \
-  (HEDLEY_TI_CL430_VERSION_CHECK(4, 0, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-  HEDLEY_TI_CL430_VERSION_CHECK(4, 3, 0) || \
-  (HEDLEY_TI_CL6X_VERSION_CHECK(7, 2, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-  HEDLEY_TI_CL6X_VERSION_CHECK(7, 5, 0) || \
-  HEDLEY_TI_CL7X_VERSION_CHECK(1, 2, 0) || \
-  HEDLEY_TI_CLPRU_VERSION_CHECK(2, 1, 0)
+  HEDLEY_GCC_VERSION_CHECK(4,0,0) || \
+  HEDLEY_INTEL_VERSION_CHECK(13,0,0) || \
+  HEDLEY_SUNPRO_VERSION_CHECK(5,11,0) || \
+  HEDLEY_ARM_VERSION_CHECK(4,1,0) || \
+  HEDLEY_IBM_VERSION_CHECK(10,1,0) || \
+  HEDLEY_TI_VERSION_CHECK(15,12,0) || \
+  (HEDLEY_TI_ARMCL_VERSION_CHECK(4,8,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+  HEDLEY_TI_ARMCL_VERSION_CHECK(5,2,0) || \
+  (HEDLEY_TI_CL2000_VERSION_CHECK(6,0,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+  HEDLEY_TI_CL2000_VERSION_CHECK(6,4,0) || \
+  (HEDLEY_TI_CL430_VERSION_CHECK(4,0,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+  HEDLEY_TI_CL430_VERSION_CHECK(4,3,0) || \
+  (HEDLEY_TI_CL6X_VERSION_CHECK(7,2,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+  HEDLEY_TI_CL6X_VERSION_CHECK(7,5,0) || \
+  HEDLEY_TI_CL7X_VERSION_CHECK(1,2,0) || \
+  HEDLEY_TI_CLPRU_VERSION_CHECK(2,1,0) || \
+  HEDLEY_MCST_LCC_VERSION_CHECK(1,25,10) || \
+  HEDLEY_IAR_VERSION_CHECK(8,10,0)
 #  define HEDLEY_NEVER_INLINE __attribute__((__noinline__))
-#elif HEDLEY_MSVC_VERSION_CHECK(13, 10, 0)
+#elif \
+  HEDLEY_MSVC_VERSION_CHECK(13,10,0) || \
+  HEDLEY_INTEL_CL_VERSION_CHECK(2021,1,0)
 #  define HEDLEY_NEVER_INLINE __declspec(noinline)
-#elif HEDLEY_PGI_VERSION_CHECK(10, 2, 0)
+#elif HEDLEY_PGI_VERSION_CHECK(10,2,0)
 #  define HEDLEY_NEVER_INLINE _Pragma("noinline")
-#elif HEDLEY_TI_CL6X_VERSION_CHECK(6, 0, 0) && defined(__cplusplus)
+#elif HEDLEY_TI_CL6X_VERSION_CHECK(6,0,0) && defined(__cplusplus)
 #  define HEDLEY_NEVER_INLINE _Pragma("FUNC_CANNOT_INLINE;")
-#elif HEDLEY_IAR_VERSION_CHECK(8, 0, 0)
+#elif HEDLEY_IAR_VERSION_CHECK(8,0,0)
 #  define HEDLEY_NEVER_INLINE _Pragma("inline=never")
-#elif HEDLEY_COMPCERT_VERSION_CHECK(3, 2, 0)
+#elif HEDLEY_COMPCERT_VERSION_CHECK(3,2,0)
 #  define HEDLEY_NEVER_INLINE __attribute((noinline))
-#elif HEDLEY_PELLES_VERSION_CHECK(9, 0, 0)
+#elif HEDLEY_PELLES_VERSION_CHECK(9,0,0)
 #  define HEDLEY_NEVER_INLINE __declspec(noinline)
 #else
 #  define HEDLEY_NEVER_INLINE
 #endif
 
 #if defined(HEDLEY_PRIVATE)
 #  undef HEDLEY_PRIVATE
@@ -1522,72 +1650,79 @@
 #if defined(_WIN32) || defined(__CYGWIN__)
 #  define HEDLEY_PRIVATE
 #  define HEDLEY_PUBLIC   __declspec(dllexport)
 #  define HEDLEY_IMPORT   __declspec(dllimport)
 #else
 #  if \
     HEDLEY_HAS_ATTRIBUTE(visibility) || \
-    HEDLEY_GCC_VERSION_CHECK(3, 3, 0) || \
-    HEDLEY_SUNPRO_VERSION_CHECK(5, 11, 0) || \
-    HEDLEY_INTEL_VERSION_CHECK(13, 0, 0) || \
-    HEDLEY_ARM_VERSION_CHECK(4, 1, 0) || \
-    HEDLEY_IBM_VERSION_CHECK(13, 1, 0) || \
-    (\
+    HEDLEY_GCC_VERSION_CHECK(3,3,0) || \
+    HEDLEY_SUNPRO_VERSION_CHECK(5,11,0) || \
+    HEDLEY_INTEL_VERSION_CHECK(13,0,0) || \
+    HEDLEY_ARM_VERSION_CHECK(4,1,0) || \
+    HEDLEY_IBM_VERSION_CHECK(13,1,0) || \
+    ( \
       defined(__TI_EABI__) && \
-      (\
-        (HEDLEY_TI_CL6X_VERSION_CHECK(7, 2, 0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
-        HEDLEY_TI_CL6X_VERSION_CHECK(7, 5, 0) \
-) \
-)
+      ( \
+        (HEDLEY_TI_CL6X_VERSION_CHECK(7,2,0) && defined(__TI_GNU_ATTRIBUTE_SUPPORT__)) || \
+        HEDLEY_TI_CL6X_VERSION_CHECK(7,5,0) \
+      ) \
+    ) || \
+    HEDLEY_MCST_LCC_VERSION_CHECK(1,25,10)
 #    define HEDLEY_PRIVATE __attribute__((__visibility__("hidden")))
 #    define HEDLEY_PUBLIC  __attribute__((__visibility__("default")))
 #  else
 #    define HEDLEY_PRIVATE
 #    define HEDLEY_PUBLIC
 #  endif
 #  define HEDLEY_IMPORT    extern
 #endif
 
 #if defined(HEDLEY_NO_THROW)
 #  undef HEDLEY_NO_THROW
 #endif
 #if \
   HEDLEY_HAS_ATTRIBUTE(nothrow) || \
-  HEDLEY_GCC_VERSION_CHECK(3, 3, 0) || \
-  HEDLEY_INTEL_VERSION_CHECK(13, 0, 0)
+  HEDLEY_GCC_VERSION_CHECK(3,3,0) || \
+  HEDLEY_INTEL_VERSION_CHECK(13,0,0) || \
+  HEDLEY_MCST_LCC_VERSION_CHECK(1,25,10)
 #  define HEDLEY_NO_THROW __attribute__((__nothrow__))
 #elif \
-  HEDLEY_MSVC_VERSION_CHECK(13, 1, 0) || \
-  HEDLEY_ARM_VERSION_CHECK(4, 1, 0)
+  HEDLEY_MSVC_VERSION_CHECK(13,1,0) || \
+  HEDLEY_INTEL_CL_VERSION_CHECK(2021,1,0) || \
+  HEDLEY_ARM_VERSION_CHECK(4,1,0)
 #  define HEDLEY_NO_THROW __declspec(nothrow)
 #else
 #  define HEDLEY_NO_THROW
 #endif
 
 #if defined(HEDLEY_FALL_THROUGH)
 # undef HEDLEY_FALL_THROUGH
 #endif
-#if HEDLEY_GNUC_HAS_ATTRIBUTE(fallthrough, 7, 0, 0) && !defined(HEDLEY_PGI_VERSION)
+#if \
+  HEDLEY_HAS_ATTRIBUTE(fallthrough) || \
+  HEDLEY_GCC_VERSION_CHECK(7,0,0) || \
+  HEDLEY_MCST_LCC_VERSION_CHECK(1,25,10)
 #  define HEDLEY_FALL_THROUGH __attribute__((__fallthrough__))
-#elif HEDLEY_HAS_CPP_ATTRIBUTE_NS(clang, fallthrough)
+#elif HEDLEY_HAS_CPP_ATTRIBUTE_NS(clang,fallthrough)
 #  define HEDLEY_FALL_THROUGH HEDLEY_DIAGNOSTIC_DISABLE_CPP98_COMPAT_WRAP_([[clang::fallthrough]])
 #elif HEDLEY_HAS_CPP_ATTRIBUTE(fallthrough)
 #  define HEDLEY_FALL_THROUGH HEDLEY_DIAGNOSTIC_DISABLE_CPP98_COMPAT_WRAP_([[fallthrough]])
 #elif defined(__fallthrough) /* SAL */
 #  define HEDLEY_FALL_THROUGH __fallthrough
 #else
 #  define HEDLEY_FALL_THROUGH
 #endif
 
 #if defined(HEDLEY_RETURNS_NON_NULL)
 #  undef HEDLEY_RETURNS_NON_NULL
 #endif
 #if \
   HEDLEY_HAS_ATTRIBUTE(returns_nonnull) || \
-  HEDLEY_GCC_VERSION_CHECK(4, 9, 0)
+  HEDLEY_GCC_VERSION_CHECK(4,9,0) || \
+  HEDLEY_MCST_LCC_VERSION_CHECK(1,25,10)
 #  define HEDLEY_RETURNS_NON_NULL __attribute__((__returns_nonnull__))
 #elif defined(_Ret_notnull_) /* SAL */
 #  define HEDLEY_RETURNS_NON_NULL _Ret_notnull_
 #else
 #  define HEDLEY_RETURNS_NON_NULL
 #endif
 
@@ -1614,62 +1749,63 @@
 /* HEDLEY_IS_CONSTEXPR_ is for
    HEDLEY INTERNAL USE ONLY.  API subject to change without notice. */
 #if defined(HEDLEY_IS_CONSTEXPR_)
 #  undef HEDLEY_IS_CONSTEXPR_
 #endif
 #if \
   HEDLEY_HAS_BUILTIN(__builtin_constant_p) || \
-  HEDLEY_GCC_VERSION_CHECK(3, 4, 0) || \
-  HEDLEY_INTEL_VERSION_CHECK(13, 0, 0) || \
-  HEDLEY_TINYC_VERSION_CHECK(0, 9, 19) || \
-  HEDLEY_ARM_VERSION_CHECK(4, 1, 0) || \
-  HEDLEY_IBM_VERSION_CHECK(13, 1, 0) || \
-  HEDLEY_TI_CL6X_VERSION_CHECK(6, 1, 0) || \
-  (HEDLEY_SUNPRO_VERSION_CHECK(5, 10, 0) && !defined(__cplusplus)) || \
-  HEDLEY_CRAY_VERSION_CHECK(8, 1, 0)
+  HEDLEY_GCC_VERSION_CHECK(3,4,0) || \
+  HEDLEY_INTEL_VERSION_CHECK(13,0,0) || \
+  HEDLEY_TINYC_VERSION_CHECK(0,9,19) || \
+  HEDLEY_ARM_VERSION_CHECK(4,1,0) || \
+  HEDLEY_IBM_VERSION_CHECK(13,1,0) || \
+  HEDLEY_TI_CL6X_VERSION_CHECK(6,1,0) || \
+  (HEDLEY_SUNPRO_VERSION_CHECK(5,10,0) && !defined(__cplusplus)) || \
+  HEDLEY_CRAY_VERSION_CHECK(8,1,0) || \
+  HEDLEY_MCST_LCC_VERSION_CHECK(1,25,10)
 #  define HEDLEY_IS_CONSTANT(expr) __builtin_constant_p(expr)
 #endif
 #if !defined(__cplusplus)
 #  if \
        HEDLEY_HAS_BUILTIN(__builtin_types_compatible_p) || \
-       HEDLEY_GCC_VERSION_CHECK(3, 4, 0) || \
-       HEDLEY_INTEL_VERSION_CHECK(13, 0, 0) || \
-       HEDLEY_IBM_VERSION_CHECK(13, 1, 0) || \
-       HEDLEY_CRAY_VERSION_CHECK(8, 1, 0) || \
-       HEDLEY_ARM_VERSION_CHECK(5, 4, 0) || \
-       HEDLEY_TINYC_VERSION_CHECK(0, 9, 24)
+       HEDLEY_GCC_VERSION_CHECK(3,4,0) || \
+       HEDLEY_INTEL_VERSION_CHECK(13,0,0) || \
+       HEDLEY_IBM_VERSION_CHECK(13,1,0) || \
+       HEDLEY_CRAY_VERSION_CHECK(8,1,0) || \
+       HEDLEY_ARM_VERSION_CHECK(5,4,0) || \
+       HEDLEY_TINYC_VERSION_CHECK(0,9,24)
 #    if defined(__INTPTR_TYPE__)
 #      define HEDLEY_IS_CONSTEXPR_(expr) __builtin_types_compatible_p(__typeof__((1 ? (void*) ((__INTPTR_TYPE__) ((expr) * 0)) : (int*) 0)), int*)
 #    else
 #      include <stdint.h>
 #      define HEDLEY_IS_CONSTEXPR_(expr) __builtin_types_compatible_p(__typeof__((1 ? (void*) ((intptr_t) ((expr) * 0)) : (int*) 0)), int*)
 #    endif
 #  elif \
-       (\
+       ( \
           defined(__STDC_VERSION__) && (__STDC_VERSION__ >= 201112L) && \
           !defined(HEDLEY_SUNPRO_VERSION) && \
           !defined(HEDLEY_PGI_VERSION) && \
           !defined(HEDLEY_IAR_VERSION)) || \
-       HEDLEY_HAS_EXTENSION(c_generic_selections) || \
-       HEDLEY_GCC_VERSION_CHECK(4, 9, 0) || \
-       HEDLEY_INTEL_VERSION_CHECK(17, 0, 0) || \
-       HEDLEY_IBM_VERSION_CHECK(12, 1, 0) || \
-       HEDLEY_ARM_VERSION_CHECK(5, 3, 0)
+       (HEDLEY_HAS_EXTENSION(c_generic_selections) && !defined(HEDLEY_IAR_VERSION)) || \
+       HEDLEY_GCC_VERSION_CHECK(4,9,0) || \
+       HEDLEY_INTEL_VERSION_CHECK(17,0,0) || \
+       HEDLEY_IBM_VERSION_CHECK(12,1,0) || \
+       HEDLEY_ARM_VERSION_CHECK(5,3,0)
 #    if defined(__INTPTR_TYPE__)
 #      define HEDLEY_IS_CONSTEXPR_(expr) _Generic((1 ? (void*) ((__INTPTR_TYPE__) ((expr) * 0)) : (int*) 0), int*: 1, void*: 0)
 #    else
 #      include <stdint.h>
 #      define HEDLEY_IS_CONSTEXPR_(expr) _Generic((1 ? (void*) ((intptr_t) * 0) : (int*) 0), int*: 1, void*: 0)
 #    endif
 #  elif \
        defined(HEDLEY_GCC_VERSION) || \
        defined(HEDLEY_INTEL_VERSION) || \
        defined(HEDLEY_TINYC_VERSION) || \
        defined(HEDLEY_TI_ARMCL_VERSION) || \
-       HEDLEY_TI_CL430_VERSION_CHECK(18, 12, 0) || \
+       HEDLEY_TI_CL430_VERSION_CHECK(18,12,0) || \
        defined(HEDLEY_TI_CL2000_VERSION) || \
        defined(HEDLEY_TI_CL6X_VERSION) || \
        defined(HEDLEY_TI_CL7X_VERSION) || \
        defined(HEDLEY_TI_CLPRU_VERSION) || \
        defined(__clang__)
 #    define HEDLEY_IS_CONSTEXPR_(expr) ( \
          sizeof(void) != \
@@ -1713,25 +1849,26 @@
 #  define HEDLEY_C_DECL
 #endif
 
 #if defined(HEDLEY_STATIC_ASSERT)
 #  undef HEDLEY_STATIC_ASSERT
 #endif
 #if \
-  !defined(__cplusplus) && (\
+  !defined(__cplusplus) && ( \
       (defined(__STDC_VERSION__) && (__STDC_VERSION__ >= 201112L)) || \
-      HEDLEY_HAS_FEATURE(c_static_assert) || \
-      HEDLEY_GCC_VERSION_CHECK(6, 0, 0) || \
-      HEDLEY_INTEL_VERSION_CHECK(13, 0, 0) || \
+      (HEDLEY_HAS_FEATURE(c_static_assert) && !defined(HEDLEY_INTEL_CL_VERSION)) || \
+      HEDLEY_GCC_VERSION_CHECK(6,0,0) || \
+      HEDLEY_INTEL_VERSION_CHECK(13,0,0) || \
       defined(_Static_assert) \
-)
+    )
 #  define HEDLEY_STATIC_ASSERT(expr, message) _Static_assert(expr, message)
 #elif \
   (defined(__cplusplus) && (__cplusplus >= 201103L)) || \
-  HEDLEY_MSVC_VERSION_CHECK(16, 0, 0)
+  HEDLEY_MSVC_VERSION_CHECK(16,0,0) || \
+  HEDLEY_INTEL_CL_VERSION_CHECK(2021,1,0)
 #  define HEDLEY_STATIC_ASSERT(expr, message) HEDLEY_DIAGNOSTIC_DISABLE_CPP98_COMPAT_WRAP_(static_assert(expr, message))
 #else
 #  define HEDLEY_STATIC_ASSERT(expr, message)
 #endif
 
 #if defined(HEDLEY_NULL)
 #  undef HEDLEY_NULL
@@ -1756,22 +1893,22 @@
 #if HEDLEY_HAS_WARNING("-Wunknown-pragmas")
 #  define HEDLEY_MESSAGE(msg) \
   HEDLEY_DIAGNOSTIC_PUSH \
   HEDLEY_DIAGNOSTIC_DISABLE_UNKNOWN_PRAGMAS \
   HEDLEY_PRAGMA(message msg) \
   HEDLEY_DIAGNOSTIC_POP
 #elif \
-  HEDLEY_GCC_VERSION_CHECK(4, 4, 0) || \
-  HEDLEY_INTEL_VERSION_CHECK(13, 0, 0)
+  HEDLEY_GCC_VERSION_CHECK(4,4,0) || \
+  HEDLEY_INTEL_VERSION_CHECK(13,0,0)
 #  define HEDLEY_MESSAGE(msg) HEDLEY_PRAGMA(message msg)
-#elif HEDLEY_CRAY_VERSION_CHECK(5, 0, 0)
+#elif HEDLEY_CRAY_VERSION_CHECK(5,0,0)
 #  define HEDLEY_MESSAGE(msg) HEDLEY_PRAGMA(_CRI message msg)
-#elif HEDLEY_IAR_VERSION_CHECK(8, 0, 0)
+#elif HEDLEY_IAR_VERSION_CHECK(8,0,0)
 #  define HEDLEY_MESSAGE(msg) HEDLEY_PRAGMA(message(msg))
-#elif HEDLEY_PELLES_VERSION_CHECK(2, 0, 0)
+#elif HEDLEY_PELLES_VERSION_CHECK(2,0,0)
 #  define HEDLEY_MESSAGE(msg) HEDLEY_PRAGMA(message(msg))
 #else
 #  define HEDLEY_MESSAGE(msg)
 #endif
 
 #if defined(HEDLEY_WARNING)
 #  undef HEDLEY_WARNING
@@ -1779,19 +1916,21 @@
 #if HEDLEY_HAS_WARNING("-Wunknown-pragmas")
 #  define HEDLEY_WARNING(msg) \
   HEDLEY_DIAGNOSTIC_PUSH \
   HEDLEY_DIAGNOSTIC_DISABLE_UNKNOWN_PRAGMAS \
   HEDLEY_PRAGMA(clang warning msg) \
   HEDLEY_DIAGNOSTIC_POP
 #elif \
-  HEDLEY_GCC_VERSION_CHECK(4, 8, 0) || \
-  HEDLEY_PGI_VERSION_CHECK(18, 4, 0) || \
-  HEDLEY_INTEL_VERSION_CHECK(13, 0, 0)
+  HEDLEY_GCC_VERSION_CHECK(4,8,0) || \
+  HEDLEY_PGI_VERSION_CHECK(18,4,0) || \
+  HEDLEY_INTEL_VERSION_CHECK(13,0,0)
 #  define HEDLEY_WARNING(msg) HEDLEY_PRAGMA(GCC warning msg)
-#elif HEDLEY_MSVC_VERSION_CHECK(15, 0, 0)
+#elif \
+  HEDLEY_MSVC_VERSION_CHECK(15,0,0) || \
+  HEDLEY_INTEL_CL_VERSION_CHECK(2021,1,0)
 #  define HEDLEY_WARNING(msg) HEDLEY_PRAGMA(message(msg))
 #else
 #  define HEDLEY_WARNING(msg) HEDLEY_MESSAGE(msg)
 #endif
 
 #if defined(HEDLEY_REQUIRE)
 #  undef HEDLEY_REQUIRE
@@ -1813,56 +1952,60 @@
        HEDLEY_DIAGNOSTIC_POP
 #  else
 #    define HEDLEY_REQUIRE(expr) __attribute__((diagnose_if(!(expr), #expr, "error")))
 #    define HEDLEY_REQUIRE_MSG(expr,msg) __attribute__((diagnose_if(!(expr), msg, "error")))
 #  endif
 #else
 #  define HEDLEY_REQUIRE(expr)
-#  define HEDLEY_REQUIRE_MSG(expr, msg)
+#  define HEDLEY_REQUIRE_MSG(expr,msg)
 #endif
 
 #if defined(HEDLEY_FLAGS)
 #  undef HEDLEY_FLAGS
 #endif
-#if HEDLEY_HAS_ATTRIBUTE(flag_enum)
+#if HEDLEY_HAS_ATTRIBUTE(flag_enum) && (!defined(__cplusplus) || HEDLEY_HAS_WARNING("-Wbitfield-enum-conversion"))
 #  define HEDLEY_FLAGS __attribute__((__flag_enum__))
+#else
+#  define HEDLEY_FLAGS
 #endif
 
 #if defined(HEDLEY_FLAGS_CAST)
 #  undef HEDLEY_FLAGS_CAST
 #endif
-#if HEDLEY_INTEL_VERSION_CHECK(19, 0, 0)
+#if HEDLEY_INTEL_VERSION_CHECK(19,0,0)
 #  define HEDLEY_FLAGS_CAST(T, expr) (__extension__ ({ \
   HEDLEY_DIAGNOSTIC_PUSH \
       _Pragma("warning(disable:188)") \
       ((T) (expr)); \
       HEDLEY_DIAGNOSTIC_POP \
     }))
 #else
 #  define HEDLEY_FLAGS_CAST(T, expr) HEDLEY_STATIC_CAST(T, expr)
 #endif
 
 #if defined(HEDLEY_EMPTY_BASES)
 #  undef HEDLEY_EMPTY_BASES
 #endif
-#if HEDLEY_MSVC_VERSION_CHECK(19, 0, 23918) && !HEDLEY_MSVC_VERSION_CHECK(20, 0, 0)
+#if \
+  (HEDLEY_MSVC_VERSION_CHECK(19,0,23918) && !HEDLEY_MSVC_VERSION_CHECK(20,0,0)) || \
+  HEDLEY_INTEL_CL_VERSION_CHECK(2021,1,0)
 #  define HEDLEY_EMPTY_BASES __declspec(empty_bases)
 #else
 #  define HEDLEY_EMPTY_BASES
 #endif
 
 /* Remaining macros are deprecated. */
 
 #if defined(HEDLEY_GCC_NOT_CLANG_VERSION_CHECK)
 #  undef HEDLEY_GCC_NOT_CLANG_VERSION_CHECK
 #endif
 #if defined(__clang__)
 #  define HEDLEY_GCC_NOT_CLANG_VERSION_CHECK(major,minor,patch) (0)
 #else
-#  define HEDLEY_GCC_NOT_CLANG_VERSION_CHECK(major, minor, patch) HEDLEY_GCC_VERSION_CHECK(major,minor,patch)
+#  define HEDLEY_GCC_NOT_CLANG_VERSION_CHECK(major,minor,patch) HEDLEY_GCC_VERSION_CHECK(major,minor,patch)
 #endif
 
 #if defined(HEDLEY_CLANG_HAS_ATTRIBUTE)
 #  undef HEDLEY_CLANG_HAS_ATTRIBUTE
 #endif
 #define HEDLEY_CLANG_HAS_ATTRIBUTE(attribute) HEDLEY_HAS_ATTRIBUTE(attribute)
```

### Comparing `sabctools-8.1.0/src/yencode/stdint.h` & `sabctools-8.2.0/src/yencode/stdint.h`

 * *Files identical despite different names*

