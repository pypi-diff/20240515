# Comparing `tmp/jaxns-2.4.9.tar.gz` & `tmp/jaxns-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxns-2.4.9.tar", last modified: Thu Feb 22 03:47:21 2024, max compression
+gzip compressed data, was "jaxns-2.5.0.tar", last modified: Wed May 15 10:21:59 2024, max compression
```

## Comparing `jaxns-2.4.9.tar` & `jaxns-2.5.0.tar`

### file list

```diff
@@ -1,91 +1,96 @@
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-02-22 03:47:21.637219 jaxns-2.4.9/
--rw-rw-r--   0 albert    (1000) albert    (1000)     2553 2023-07-28 03:56:53.000000 jaxns-2.4.9/LICENSE
--rw-r--r--   0 albert    (1000) albert    (1000)    15421 2024-02-22 03:47:21.637219 jaxns-2.4.9/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)    14695 2024-02-22 03:29:52.000000 jaxns-2.4.9/README.md
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-02-22 03:47:21.625219 jaxns-2.4.9/jaxns/
--rw-rw-r--   0 albert    (1000) albert    (1000)      288 2023-12-11 00:50:30.000000 jaxns-2.4.9/jaxns/__init__.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-02-22 03:47:21.625219 jaxns-2.4.9/jaxns/experimental/
--rw-rw-r--   0 albert    (1000) albert    (1000)      147 2024-01-10 09:23:52.000000 jaxns-2.4.9/jaxns/experimental/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    12992 2024-01-31 16:18:52.000000 jaxns-2.4.9/jaxns/experimental/evidence_maximisation.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    21128 2024-01-29 17:05:52.000000 jaxns-2.4.9/jaxns/experimental/global_optimisation.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3280 2024-01-29 16:58:54.000000 jaxns-2.4.9/jaxns/experimental/public.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-02-22 03:47:21.625219 jaxns-2.4.9/jaxns/experimental/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2024-01-10 01:28:49.000000 jaxns-2.4.9/jaxns/experimental/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      679 2024-01-31 17:17:38.000000 jaxns-2.4.9/jaxns/experimental/tests/test_evidence_maximisation.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3961 2024-01-29 17:06:40.000000 jaxns-2.4.9/jaxns/experimental/tests/test_global_optimisation.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-02-22 03:47:21.629219 jaxns-2.4.9/jaxns/framework/
--rw-rw-r--   0 albert    (1000) albert    (1000)      180 2023-12-11 01:06:46.000000 jaxns-2.4.9/jaxns/framework/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5885 2024-01-31 12:49:58.000000 jaxns-2.4.9/jaxns/framework/abc.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5656 2024-01-08 14:18:38.000000 jaxns-2.4.9/jaxns/framework/bases.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3349 2024-01-08 12:42:05.000000 jaxns-2.4.9/jaxns/framework/distribution.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     6525 2024-01-31 12:49:58.000000 jaxns-2.4.9/jaxns/framework/model.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     9229 2024-02-22 03:14:36.000000 jaxns-2.4.9/jaxns/framework/ops.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     6228 2024-01-31 12:49:58.000000 jaxns-2.4.9/jaxns/framework/prior.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    12894 2024-02-22 03:19:29.000000 jaxns-2.4.9/jaxns/framework/special_priors.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-02-22 03:47:21.629219 jaxns-2.4.9/jaxns/framework/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)      144 2023-12-10 01:41:41.000000 jaxns-2.4.9/jaxns/framework/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1894 2024-02-22 03:13:31.000000 jaxns-2.4.9/jaxns/framework/tests/test_model.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    10272 2024-02-21 03:32:49.000000 jaxns-2.4.9/jaxns/framework/tests/test_prior.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-02-22 03:47:21.629219 jaxns-2.4.9/jaxns/internals/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-07-28 03:56:05.000000 jaxns-2.4.9/jaxns/internals/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3003 2024-01-09 16:10:02.000000 jaxns-2.4.9/jaxns/internals/cumulative_ops.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      853 2023-12-11 11:21:48.000000 jaxns-2.4.9/jaxns/internals/linalg.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    12950 2023-12-20 00:59:59.000000 jaxns-2.4.9/jaxns/internals/log_semiring.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     8962 2024-01-31 03:49:25.000000 jaxns-2.4.9/jaxns/internals/maps.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2792 2023-12-10 16:34:33.000000 jaxns-2.4.9/jaxns/internals/random.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1899 2023-07-28 03:56:05.000000 jaxns-2.4.9/jaxns/internals/shapes.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     6415 2024-01-15 16:09:59.000000 jaxns-2.4.9/jaxns/internals/shrinkage_statistics.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2248 2023-12-10 16:34:32.000000 jaxns-2.4.9/jaxns/internals/stats.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-02-22 03:47:21.633219 jaxns-2.4.9/jaxns/internals/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-07-28 03:56:05.000000 jaxns-2.4.9/jaxns/internals/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1752 2024-01-31 11:46:29.000000 jaxns-2.4.9/jaxns/internals/tests/test_cumulative_ops.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      304 2023-12-11 11:21:48.000000 jaxns-2.4.9/jaxns/internals/tests/test_linalg.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5500 2023-12-10 16:34:33.000000 jaxns-2.4.9/jaxns/internals/tests/test_log_semiring.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3629 2024-01-31 03:39:54.000000 jaxns-2.4.9/jaxns/internals/tests/test_maps.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1337 2023-12-11 11:21:48.000000 jaxns-2.4.9/jaxns/internals/tests/test_random.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1110 2023-07-28 03:56:05.000000 jaxns-2.4.9/jaxns/internals/tests/test_shapes.py
--rw-rw-r--   0 albert    (1000) albert    (1000)        3 2024-01-09 16:10:02.000000 jaxns-2.4.9/jaxns/internals/tests/test_shrink_statistics.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1186 2023-07-28 03:56:05.000000 jaxns-2.4.9/jaxns/internals/tests/test_stats.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     8107 2024-01-31 11:49:01.000000 jaxns-2.4.9/jaxns/internals/tests/test_tree_structure.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      792 2024-02-20 02:02:51.000000 jaxns-2.4.9/jaxns/internals/tests/test_types.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    15740 2024-01-10 02:40:26.000000 jaxns-2.4.9/jaxns/internals/tree_structure.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     7012 2024-02-20 02:01:35.000000 jaxns-2.4.9/jaxns/internals/types.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-02-22 03:47:21.633219 jaxns-2.4.9/jaxns/nested_sampler/
--rw-rw-r--   0 albert    (1000) albert    (1000)       50 2023-12-10 16:33:43.000000 jaxns-2.4.9/jaxns/nested_sampler/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1132 2023-12-10 16:34:32.000000 jaxns-2.4.9/jaxns/nested_sampler/abc.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      303 2023-12-10 16:33:43.000000 jaxns-2.4.9/jaxns/nested_sampler/bases.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    35927 2024-01-31 12:49:58.000000 jaxns-2.4.9/jaxns/nested_sampler/standard_static.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    18751 2024-01-31 12:49:58.000000 jaxns-2.4.9/jaxns/plotting.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     7642 2024-01-31 12:49:58.000000 jaxns-2.4.9/jaxns/public.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-02-22 03:47:21.633219 jaxns-2.4.9/jaxns/samplers/
--rw-rw-r--   0 albert    (1000) albert    (1000)      198 2023-12-10 16:33:43.000000 jaxns-2.4.9/jaxns/samplers/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1892 2024-01-08 18:14:31.000000 jaxns-2.4.9/jaxns/samplers/abc.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2695 2024-01-28 16:29:45.000000 jaxns-2.4.9/jaxns/samplers/bases.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-02-22 03:47:21.633219 jaxns-2.4.9/jaxns/samplers/multi_ellipsoid/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-12-10 01:41:41.000000 jaxns-2.4.9/jaxns/samplers/multi_ellipsoid/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3152 2023-12-10 01:41:41.000000 jaxns-2.4.9/jaxns/samplers/multi_ellipsoid/em_gmm.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    29796 2023-12-10 16:34:32.000000 jaxns-2.4.9/jaxns/samplers/multi_ellipsoid/multi_ellipsoid_utils.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-02-22 03:47:21.637219 jaxns-2.4.9/jaxns/samplers/multi_ellipsoid/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-12-10 01:41:41.000000 jaxns-2.4.9/jaxns/samplers/multi_ellipsoid/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1309 2023-12-10 01:41:41.000000 jaxns-2.4.9/jaxns/samplers/multi_ellipsoid/tests/test_em_gmm.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5364 2023-12-11 11:21:48.000000 jaxns-2.4.9/jaxns/samplers/multi_ellipsoid/tests/test_multi_ellipsoid.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     4787 2024-01-08 18:04:15.000000 jaxns-2.4.9/jaxns/samplers/multi_ellipsoidal_samplers.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    10355 2024-01-09 16:10:02.000000 jaxns-2.4.9/jaxns/samplers/multi_slice_sampler.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    15922 2024-01-29 17:05:52.000000 jaxns-2.4.9/jaxns/samplers/uni_slice_sampler.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3497 2024-01-09 14:57:10.000000 jaxns-2.4.9/jaxns/samplers/uniform_samplers.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-02-22 03:47:21.637219 jaxns-2.4.9/jaxns/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-07-28 03:56:05.000000 jaxns-2.4.9/jaxns/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     9716 2024-01-24 18:26:27.000000 jaxns-2.4.9/jaxns/tests/conftest.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3245 2024-01-15 16:09:59.000000 jaxns-2.4.9/jaxns/tests/test_nested_sampler.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      816 2023-12-20 00:59:59.000000 jaxns-2.4.9/jaxns/tests/test_utils.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    20463 2024-02-20 02:01:35.000000 jaxns-2.4.9/jaxns/utils.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      716 2023-07-28 03:56:05.000000 jaxns-2.4.9/jaxns/warnings.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-02-22 03:47:21.637219 jaxns-2.4.9/jaxns.egg-info/
--rw-r--r--   0 albert    (1000) albert    (1000)    15421 2024-02-22 03:47:21.000000 jaxns-2.4.9/jaxns.egg-info/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)     2546 2024-02-22 03:47:21.000000 jaxns-2.4.9/jaxns.egg-info/SOURCES.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        1 2024-02-22 03:47:21.000000 jaxns-2.4.9/jaxns.egg-info/dependency_links.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)      107 2024-02-22 03:47:21.000000 jaxns-2.4.9/jaxns.egg-info/requires.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        6 2024-02-22 03:47:21.000000 jaxns-2.4.9/jaxns.egg-info/top_level.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)      103 2023-07-28 03:56:05.000000 jaxns-2.4.9/pyproject.toml
--rw-rw-r--   0 albert    (1000) albert    (1000)       38 2024-02-22 03:47:21.637219 jaxns-2.4.9/setup.cfg
--rwxrwxr-x   0 albert    (1000) albert    (1000)     1078 2024-02-22 03:25:26.000000 jaxns-2.4.9/setup.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-15 10:21:59.363427 jaxns-2.5.0/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2518 2024-03-20 16:58:01.000000 jaxns-2.5.0/LICENSE
+-rw-r--r--   0 albert    (1000) albert    (1000)    17828 2024-05-15 10:21:59.363427 jaxns-2.5.0/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)    17147 2024-05-15 09:59:15.000000 jaxns-2.5.0/README.md
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-15 10:21:59.351427 jaxns-2.5.0/jaxns/
+-rw-rw-r--   0 albert    (1000) albert    (1000)      145 2024-03-12 14:37:32.000000 jaxns-2.5.0/jaxns/__init__.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-15 10:21:59.355427 jaxns-2.5.0/jaxns/experimental/
+-rw-rw-r--   0 albert    (1000) albert    (1000)      147 2024-01-10 09:23:52.000000 jaxns-2.5.0/jaxns/experimental/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    13924 2024-05-08 19:44:48.000000 jaxns-2.5.0/jaxns/experimental/evidence_maximisation.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    21782 2024-04-26 13:09:03.000000 jaxns-2.5.0/jaxns/experimental/global_optimisation.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3280 2024-01-29 16:58:54.000000 jaxns-2.5.0/jaxns/experimental/public.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-15 10:21:59.355427 jaxns-2.5.0/jaxns/experimental/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2024-01-10 01:28:49.000000 jaxns-2.5.0/jaxns/experimental/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2065 2024-04-26 13:09:03.000000 jaxns-2.5.0/jaxns/experimental/tests/test_evidence_maximisation.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3961 2024-01-29 17:06:40.000000 jaxns-2.5.0/jaxns/experimental/tests/test_global_optimisation.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-15 10:21:59.355427 jaxns-2.5.0/jaxns/framework/
+-rw-rw-r--   0 albert    (1000) albert    (1000)      217 2024-05-15 09:45:25.000000 jaxns-2.5.0/jaxns/framework/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5885 2024-01-31 12:49:58.000000 jaxns-2.5.0/jaxns/framework/abc.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5707 2024-03-14 00:16:44.000000 jaxns-2.5.0/jaxns/framework/bases.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1629 2024-05-15 09:45:25.000000 jaxns-2.5.0/jaxns/framework/jaxify.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     6725 2024-03-12 14:42:15.000000 jaxns-2.5.0/jaxns/framework/model.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    11345 2024-03-14 00:16:44.000000 jaxns-2.5.0/jaxns/framework/ops.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     6738 2024-03-12 14:33:47.000000 jaxns-2.5.0/jaxns/framework/prior.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    18691 2024-04-26 13:09:03.000000 jaxns-2.5.0/jaxns/framework/special_priors.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-15 10:21:59.355427 jaxns-2.5.0/jaxns/framework/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2024-03-11 13:51:33.000000 jaxns-2.5.0/jaxns/framework/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1067 2024-05-15 09:45:25.000000 jaxns-2.5.0/jaxns/framework/tests/test_jaxify.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4432 2024-05-15 09:45:25.000000 jaxns-2.5.0/jaxns/framework/tests/test_model.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    15702 2024-04-26 13:09:03.000000 jaxns-2.5.0/jaxns/framework/tests/test_prior.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3304 2024-03-06 13:22:27.000000 jaxns-2.5.0/jaxns/framework/wrapped_tfp_distribution.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-15 10:21:59.359428 jaxns-2.5.0/jaxns/internals/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-07-28 03:56:05.000000 jaxns-2.5.0/jaxns/internals/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4281 2024-05-15 09:16:27.000000 jaxns-2.5.0/jaxns/internals/cumulative_ops.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      853 2023-12-11 11:21:48.000000 jaxns-2.5.0/jaxns/internals/linalg.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    12950 2023-12-20 00:59:59.000000 jaxns-2.5.0/jaxns/internals/log_semiring.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)       92 2024-03-12 14:42:15.000000 jaxns-2.5.0/jaxns/internals/logging.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     8916 2024-04-26 13:09:03.000000 jaxns-2.5.0/jaxns/internals/maps.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2306 2024-04-26 13:09:03.000000 jaxns-2.5.0/jaxns/internals/namedtuple_utils.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2791 2024-03-20 16:51:32.000000 jaxns-2.5.0/jaxns/internals/random.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1899 2023-07-28 03:56:05.000000 jaxns-2.5.0/jaxns/internals/shapes.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     6524 2024-05-15 09:16:27.000000 jaxns-2.5.0/jaxns/internals/shrinkage_statistics.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2248 2023-12-10 16:34:32.000000 jaxns-2.5.0/jaxns/internals/stats.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-15 10:21:59.359428 jaxns-2.5.0/jaxns/internals/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-07-28 03:56:05.000000 jaxns-2.5.0/jaxns/internals/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4738 2024-05-15 09:16:27.000000 jaxns-2.5.0/jaxns/internals/tests/test_cumulative_ops.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      304 2023-12-11 11:21:48.000000 jaxns-2.5.0/jaxns/internals/tests/test_linalg.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5500 2023-12-10 16:34:33.000000 jaxns-2.5.0/jaxns/internals/tests/test_log_semiring.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3629 2024-01-31 03:39:54.000000 jaxns-2.5.0/jaxns/internals/tests/test_maps.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1760 2024-04-26 13:09:03.000000 jaxns-2.5.0/jaxns/internals/tests/test_namedtuple_utils.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1337 2023-12-11 11:21:48.000000 jaxns-2.5.0/jaxns/internals/tests/test_random.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1110 2023-07-28 03:56:05.000000 jaxns-2.5.0/jaxns/internals/tests/test_shapes.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)        3 2024-01-09 16:10:02.000000 jaxns-2.5.0/jaxns/internals/tests/test_shrink_statistics.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1186 2023-07-28 03:56:05.000000 jaxns-2.5.0/jaxns/internals/tests/test_stats.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     7880 2024-05-15 09:16:27.000000 jaxns-2.5.0/jaxns/internals/tests/test_tree_structure.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      792 2024-02-20 02:02:51.000000 jaxns-2.5.0/jaxns/internals/tests/test_types.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    15775 2024-05-15 09:16:27.000000 jaxns-2.5.0/jaxns/internals/tree_structure.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     7075 2024-03-11 23:55:22.000000 jaxns-2.5.0/jaxns/internals/types.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-15 10:21:59.359428 jaxns-2.5.0/jaxns/nested_sampler/
+-rw-rw-r--   0 albert    (1000) albert    (1000)       50 2023-12-10 16:33:43.000000 jaxns-2.5.0/jaxns/nested_sampler/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1132 2023-12-10 16:34:32.000000 jaxns-2.5.0/jaxns/nested_sampler/abc.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      303 2023-12-10 16:33:43.000000 jaxns-2.5.0/jaxns/nested_sampler/bases.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    36092 2024-05-08 19:44:48.000000 jaxns-2.5.0/jaxns/nested_sampler/standard_static.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    19018 2024-04-26 13:09:03.000000 jaxns-2.5.0/jaxns/plotting.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     7651 2024-04-26 13:09:03.000000 jaxns-2.5.0/jaxns/public.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-15 10:21:59.363427 jaxns-2.5.0/jaxns/samplers/
+-rw-rw-r--   0 albert    (1000) albert    (1000)      198 2023-12-10 16:33:43.000000 jaxns-2.5.0/jaxns/samplers/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1892 2024-01-08 18:14:31.000000 jaxns-2.5.0/jaxns/samplers/abc.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2695 2024-01-28 16:29:45.000000 jaxns-2.5.0/jaxns/samplers/bases.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-15 10:21:59.363427 jaxns-2.5.0/jaxns/samplers/multi_ellipsoid/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-12-10 01:41:41.000000 jaxns-2.5.0/jaxns/samplers/multi_ellipsoid/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4677 2024-02-22 03:55:35.000000 jaxns-2.5.0/jaxns/samplers/multi_ellipsoid/em_gmm.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    29798 2024-04-26 13:09:03.000000 jaxns-2.5.0/jaxns/samplers/multi_ellipsoid/multi_ellipsoid_utils.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-15 10:21:59.363427 jaxns-2.5.0/jaxns/samplers/multi_ellipsoid/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-12-10 01:41:41.000000 jaxns-2.5.0/jaxns/samplers/multi_ellipsoid/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1309 2024-02-22 03:58:12.000000 jaxns-2.5.0/jaxns/samplers/multi_ellipsoid/tests/test_em_gmm.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5345 2024-04-26 13:09:03.000000 jaxns-2.5.0/jaxns/samplers/multi_ellipsoid/tests/test_multi_ellipsoid.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4813 2024-04-26 13:09:03.000000 jaxns-2.5.0/jaxns/samplers/multi_ellipsoidal_samplers.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    10290 2024-05-15 09:16:27.000000 jaxns-2.5.0/jaxns/samplers/multi_slice_sampler.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    15063 2024-05-15 09:16:27.000000 jaxns-2.5.0/jaxns/samplers/uni_slice_sampler.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3502 2024-04-26 13:09:03.000000 jaxns-2.5.0/jaxns/samplers/uniform_samplers.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-15 10:21:59.363427 jaxns-2.5.0/jaxns/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-07-28 03:56:05.000000 jaxns-2.5.0/jaxns/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    11000 2024-03-05 23:02:32.000000 jaxns-2.5.0/jaxns/tests/conftest.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3245 2024-04-26 13:09:53.000000 jaxns-2.5.0/jaxns/tests/test_nested_sampler.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      816 2023-12-20 00:59:59.000000 jaxns-2.5.0/jaxns/tests/test_utils.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    20138 2024-05-08 19:44:48.000000 jaxns-2.5.0/jaxns/utils.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      678 2024-03-12 14:33:47.000000 jaxns-2.5.0/jaxns/warnings.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-05-15 10:21:59.363427 jaxns-2.5.0/jaxns.egg-info/
+-rw-r--r--   0 albert    (1000) albert    (1000)    17828 2024-05-15 10:21:59.000000 jaxns-2.5.0/jaxns.egg-info/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2741 2024-05-15 10:21:59.000000 jaxns-2.5.0/jaxns.egg-info/SOURCES.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        1 2024-05-15 10:21:59.000000 jaxns-2.5.0/jaxns.egg-info/dependency_links.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)       92 2024-05-15 10:21:59.000000 jaxns-2.5.0/jaxns.egg-info/requires.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        6 2024-05-15 10:21:59.000000 jaxns-2.5.0/jaxns.egg-info/top_level.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)      103 2023-07-28 03:56:05.000000 jaxns-2.5.0/pyproject.toml
+-rw-rw-r--   0 albert    (1000) albert    (1000)       38 2024-05-15 10:21:59.363427 jaxns-2.5.0/setup.cfg
+-rwxrwxr-x   0 albert    (1000) albert    (1000)     1049 2024-05-15 09:56:23.000000 jaxns-2.5.0/setup.py
```

### Comparing `jaxns-2.4.9/PKG-INFO` & `jaxns-2.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: jaxns
-Version: 2.4.9
-Summary: Nested Sampling in JAX
-Home-page: https://github.com/joshuaalbert/jaxns
-Author: Joshua G. Albert
-Author-email: albert@strw.leidenuniv.nl
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: jax
-Requires-Dist: jaxlib
-Requires-Dist: chex
-Requires-Dist: typing_extensions
-Requires-Dist: matplotlib
-Requires-Dist: numpy
-Requires-Dist: scipy
-Requires-Dist: tensorflow_probability
-Requires-Dist: tqdm
-Requires-Dist: dm-haiku
-Requires-Dist: optax
-Requires-Dist: jaxopt
-
 [![Python](https://img.shields.io/pypi/pyversions/jaxns.svg)](https://badge.fury.io/py/jaxns)
 [![PyPI](https://badge.fury.io/py/jaxns.svg)](https://badge.fury.io/py/jaxns)
 [![Documentation Status](https://readthedocs.org/projects/jaxns/badge/?version=latest)](https://jaxns.readthedocs.io/en/latest/?badge=latest)
 
 Main
 Status: ![Workflow name](https://github.com/JoshuaAlbert/jaxns/actions/workflows/unittests.yml/badge.svg?branch=main)
 
@@ -189,15 +163,20 @@
 # Just-in-time compilation (usually useful)
 ns_jit = jax.jit(ns)
 ```
 
 You can inspect the results, and plot them.
 
 ```python
-from jaxns import summary, plot_diagnostics, plot_cornerplot
+from jaxns import summary, plot_diagnostics, plot_cornerplot, save_results, load_results
+
+# Optionally save the results to file
+save_results(results, 'results.json')
+# To load the results back use this
+results = load_results('results.json')
 
 summary(results)
 plot_diagnostics(results)
 plot_cornerplot(results)
 ```
 
 Output:
@@ -241,14 +220,63 @@
     samples=results.samples,
     log_weights=results.log_dp_mean,
     S=1000,
     replace=True
 )
 ```
 
+### Maximising the evidence
+
+The Bayesian evidence is the ultimate model selection density, and choosing a model that maximises the evidence is
+the best way to select a model. We can use the evidence maximisation algorithm to optimise the parametrised variables
+of the model, in the manner that maximises the evidence. Below `EvidenceMaximisation` does this for the model we defined
+above, where the parametrised variables are
+automatically constrained to be in the right range, and numerical stability is ensured with proper scaling.
+
+We see that the evidence maximisation chooses a `sigma` the is very small.
+
+```python
+from jaxns.experimental import EvidenceMaximisation
+
+# Let's train the sigma parameter to maximise the evidence
+
+em = EvidenceMaximisation(model, ns_kwargs=dict(max_samples=1e4))
+results, params = em.train(num_steps=5)
+
+summary(results, with_parametrised=True)
+```
+
+Output:
+
+```
+--------
+Termination Conditions:
+Small remaining evidence
+--------
+likelihood evals: 72466
+samples: 1440
+phantom samples: 0
+likelihood evals / sample: 50.3
+phantom fraction (%): 0.0%
+--------
+logZ=-1.119 +- 0.098
+H=-0.93
+ESS=241
+--------
+sigma: mean +- std.dev. | 10%ile / 50%ile / 90%ile | MAP est. | max(L) est.
+sigma: 5.40077599e-05 +- 3.6e-12 | 5.40077563e-05 / 5.40077563e-05 / 5.40077563e-05 | 5.40077563e-05 | 5.40077563e-05
+--------
+uncert: mean +- std.dev. | 10%ile / 50%ile / 90%ile | MAP est. | max(L) est.
+uncert: 0.6 +- 0.54 | 0.05 / 0.45 / 1.37 | 0.0 | 0.0
+--------
+x: mean +- std.dev. | 10%ile / 50%ile / 90%ile | MAP est. | max(L) est.
+x: 0.01 +- 0.56 | -0.6 / -0.0 / 0.69 | 0.0 | -0.0
+--------
+```
+
 # Documentation
 
 You can read the documentation [here](https://jaxns.readthedocs.io/en/latest/#). In addition, JAXNS is partially
 described in the
 [original paper](https://arxiv.org/abs/2012.15286), as well as the paper on [Phantom-Powered Nested
 Sampling paper](https://arxiv.org/abs/2312.11330).
 
@@ -331,17 +359,30 @@
 The algorithm is fairly memory bound, so running parallelisation over multiple CPUs on the same machine may not yield
 the expected speed up, and depends on how expensive the likelihood evaluations are. Running over separate physical
 devices
 is the best way to achieve speed up.
 
 # Change Log
 
+15 May, 2024 -- JAXNS 2.5.0 released. Added ability to handle non-JAX likelihoods, e.g. if you have a simulation
+framework with python bindings you can now use it for likelihoods in JAXNS. Small performance improvements.
+
+22 Apr, 2024 -- JAXNS 2.4.13 released. Fixes bug where slice sampling not invariant to monotonic transforms of
+likelihod.
+
+20 Mar, 2024 -- JAXNS 2.4.12 released. Minor bug fixes, and readability improvements. Added Empirical special prior.
+
+5 Mar, 2024 -- JAXNS 2.4.11/b released. Add `random_init` to parametrised variables. Enable special priors to be
+parametrised.
+
+23 Feb, 2024 -- JAXNS 2.4.10 released. Hotfix for import error.
+
 21 Feb, 2024 -- JAXNS 2.4.9 released. Minor improvements to some priors, and bug fixes.
 
-31 Jan, 2024 -- JAXNS 2.4.8 released. Improved global optimisation performance using gradient slicing. 
+31 Jan, 2024 -- JAXNS 2.4.8 released. Improved global optimisation performance using gradient slicing.
 Improved evidence maximisation.
 
 25 Jan, 2024 -- JAXNS 2.4.6/7 released. Added logging. Use L-BFGS for Evidence Maximisation M-step. Fix bug in finetune.
 
 24 Jan, 2024 -- JAXNS 2.4.5 released. Gradient based finetuning global optimisation using L-BFGS. Added ability to
 simulate prior models without bulding model (for data generation.)
```

### Comparing `jaxns-2.4.9/README.md` & `jaxns-2.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: jaxns
+Version: 2.5.0
+Summary: Nested Sampling in JAX
+Home-page: https://github.com/joshuaalbert/jaxns
+Author: Joshua G. Albert
+Author-email: albert@strw.leidenuniv.nl
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: jax>=0.4.25
+Requires-Dist: jaxlib
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: tensorflow_probability
+Requires-Dist: tqdm
+Requires-Dist: dm-haiku
+Requires-Dist: optax
+Requires-Dist: jaxopt
+
 [![Python](https://img.shields.io/pypi/pyversions/jaxns.svg)](https://badge.fury.io/py/jaxns)
 [![PyPI](https://badge.fury.io/py/jaxns.svg)](https://badge.fury.io/py/jaxns)
 [![Documentation Status](https://readthedocs.org/projects/jaxns/badge/?version=latest)](https://jaxns.readthedocs.io/en/latest/?badge=latest)
 
 Main
 Status: ![Workflow name](https://github.com/JoshuaAlbert/jaxns/actions/workflows/unittests.yml/badge.svg?branch=main)
 
@@ -163,15 +187,20 @@
 # Just-in-time compilation (usually useful)
 ns_jit = jax.jit(ns)
 ```
 
 You can inspect the results, and plot them.
 
 ```python
-from jaxns import summary, plot_diagnostics, plot_cornerplot
+from jaxns import summary, plot_diagnostics, plot_cornerplot, save_results, load_results
+
+# Optionally save the results to file
+save_results(results, 'results.json')
+# To load the results back use this
+results = load_results('results.json')
 
 summary(results)
 plot_diagnostics(results)
 plot_cornerplot(results)
 ```
 
 Output:
@@ -215,14 +244,63 @@
     samples=results.samples,
     log_weights=results.log_dp_mean,
     S=1000,
     replace=True
 )
 ```
 
+### Maximising the evidence
+
+The Bayesian evidence is the ultimate model selection density, and choosing a model that maximises the evidence is
+the best way to select a model. We can use the evidence maximisation algorithm to optimise the parametrised variables
+of the model, in the manner that maximises the evidence. Below `EvidenceMaximisation` does this for the model we defined
+above, where the parametrised variables are
+automatically constrained to be in the right range, and numerical stability is ensured with proper scaling.
+
+We see that the evidence maximisation chooses a `sigma` the is very small.
+
+```python
+from jaxns.experimental import EvidenceMaximisation
+
+# Let's train the sigma parameter to maximise the evidence
+
+em = EvidenceMaximisation(model, ns_kwargs=dict(max_samples=1e4))
+results, params = em.train(num_steps=5)
+
+summary(results, with_parametrised=True)
+```
+
+Output:
+
+```
+--------
+Termination Conditions:
+Small remaining evidence
+--------
+likelihood evals: 72466
+samples: 1440
+phantom samples: 0
+likelihood evals / sample: 50.3
+phantom fraction (%): 0.0%
+--------
+logZ=-1.119 +- 0.098
+H=-0.93
+ESS=241
+--------
+sigma: mean +- std.dev. | 10%ile / 50%ile / 90%ile | MAP est. | max(L) est.
+sigma: 5.40077599e-05 +- 3.6e-12 | 5.40077563e-05 / 5.40077563e-05 / 5.40077563e-05 | 5.40077563e-05 | 5.40077563e-05
+--------
+uncert: mean +- std.dev. | 10%ile / 50%ile / 90%ile | MAP est. | max(L) est.
+uncert: 0.6 +- 0.54 | 0.05 / 0.45 / 1.37 | 0.0 | 0.0
+--------
+x: mean +- std.dev. | 10%ile / 50%ile / 90%ile | MAP est. | max(L) est.
+x: 0.01 +- 0.56 | -0.6 / -0.0 / 0.69 | 0.0 | -0.0
+--------
+```
+
 # Documentation
 
 You can read the documentation [here](https://jaxns.readthedocs.io/en/latest/#). In addition, JAXNS is partially
 described in the
 [original paper](https://arxiv.org/abs/2012.15286), as well as the paper on [Phantom-Powered Nested
 Sampling paper](https://arxiv.org/abs/2312.11330).
 
@@ -305,17 +383,30 @@
 The algorithm is fairly memory bound, so running parallelisation over multiple CPUs on the same machine may not yield
 the expected speed up, and depends on how expensive the likelihood evaluations are. Running over separate physical
 devices
 is the best way to achieve speed up.
 
 # Change Log
 
+15 May, 2024 -- JAXNS 2.5.0 released. Added ability to handle non-JAX likelihoods, e.g. if you have a simulation
+framework with python bindings you can now use it for likelihoods in JAXNS. Small performance improvements.
+
+22 Apr, 2024 -- JAXNS 2.4.13 released. Fixes bug where slice sampling not invariant to monotonic transforms of
+likelihod.
+
+20 Mar, 2024 -- JAXNS 2.4.12 released. Minor bug fixes, and readability improvements. Added Empirical special prior.
+
+5 Mar, 2024 -- JAXNS 2.4.11/b released. Add `random_init` to parametrised variables. Enable special priors to be
+parametrised.
+
+23 Feb, 2024 -- JAXNS 2.4.10 released. Hotfix for import error.
+
 21 Feb, 2024 -- JAXNS 2.4.9 released. Minor improvements to some priors, and bug fixes.
 
-31 Jan, 2024 -- JAXNS 2.4.8 released. Improved global optimisation performance using gradient slicing. 
+31 Jan, 2024 -- JAXNS 2.4.8 released. Improved global optimisation performance using gradient slicing.
 Improved evidence maximisation.
 
 25 Jan, 2024 -- JAXNS 2.4.6/7 released. Added logging. Use L-BFGS for Evidence Maximisation M-step. Fix bug in finetune.
 
 24 Jan, 2024 -- JAXNS 2.4.5 released. Gradient based finetuning global optimisation using L-BFGS. Added ability to
 simulate prior models without bulding model (for data generation.)
```

### Comparing `jaxns-2.4.9/jaxns/experimental/evidence_maximisation.py` & `jaxns-2.5.0/jaxns/experimental/evidence_maximisation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-import logging
+import dataclasses
+import time
 from functools import partial
 from typing import Tuple, Dict, Any, Optional, NamedTuple
 
 import jax
+import jaxopt
 import numpy as np
 import tensorflow_probability.substrates.jax as tfp
 from jax import numpy as jnp, random
 from jax._src.scipy.special import logsumexp
 from jaxopt import NonlinearCG, ArmijoSGD
 from tqdm import tqdm
 
 from jaxns.internals.cumulative_ops import cumulative_op_static
 from jaxns.internals.log_semiring import LogSpace
+from jaxns.internals.logging import logger
 
 try:
     import haiku as hk
 except ImportError:
     print("You must `pip install dm-haiku` first.")
     raise
 
@@ -32,16 +35,14 @@
 __all__ = [
     'EvidenceMaximisation'
 ]
 
 tfpd = tfp.distributions
 tfpk = tfp.math.psd_kernels
 
-logger = logging.getLogger('jaxns')
-
 
 class MStepData(NamedTuple):
     U_samples: jnp.ndarray
     log_weights: jnp.ndarray
     # log_dp_mean: jnp.ndarray
     # log_L_samples: jnp.ndarray
     # log_Z_mean: jnp.ndarray
@@ -56,76 +57,76 @@
 
     Returns:
         next largest n**2
     """
     return int(2 ** np.ceil(np.log2(x)))
 
 
+@dataclasses.dataclass(eq=False)
 class EvidenceMaximisation:
     """
-    Evidence Maximisation class, that implements the E and M steps. Iteratively computes the evidence and maximises it.
-    """
-
-    def __init__(self, model: Model, ns_kwargs: Dict[str, Any],
-                 max_num_epochs: int = 50, gtol=1e-2, momentum=0.9,
-                 log_Z_ftol=1., log_Z_atol=1e-4,
-                 batch_size: int = 128,
-                 termination_cond: Optional[TerminationCondition] = None,
-                 verbose: bool = False):
+    Evidence Maximisation class, that implements the E and M steps. Iteratively computes the evidence and maximises it
+    using stochastic minibatching over samples from E-step.
 
-        """
-        Initialise the EM class.
-
-        Args:
-            model: The model to train.
-            max_num_epochs: The maximum number of epochs to run M-step for.
-            gtol: The parameter tolerance for the M-step. End when all parameters change by less than gtol.
-            log_Z_ftol, log_Z_atol: The tolerances for the change in the evidence as function of log_Z_uncert.
-                Terminate if the change in log_Z is less than max(log_Z_ftol * log_Z_uncert, log_Z_atol).
-            ns_kwargs: The keyword arguments to pass to the nested sampler. Needs at least `max_samples`.
-            verbose: Whether to print progress verbosely.
-        """
-        if not isinstance(model, Model):
-            raise ValueError("model must be an instance of ParametrisedModel")
-        self.model = model
-        self.max_num_epochs = max_num_epochs
-        self.gtol = gtol
-        self.momentum = momentum
-        self.log_Z_ftol = log_Z_ftol
-        self.log_Z_atol = log_Z_atol
-        self._verbose = bool(verbose)
-        self._ns_kwargs = ns_kwargs
-        self._batch_size = batch_size
-        self._termination_cond = termination_cond or TerminationCondition()
+    Args:
+        model: The model to train.
+        ns_kwargs: The keyword arguments to pass to the nested sampler. Needs at least `max_samples`.
+        max_num_epochs: The maximum number of epochs to run M-step for.
+        gtol: The parameter tolerance for the M-step. End when all parameters change by less than gtol.
+        log_Z_ftol, log_Z_atol: The tolerances for the change in the evidence as function of log_Z_uncert.
+            Terminate if the change in log_Z is less than max(log_Z_ftol * log_Z_uncert, log_Z_atol).
+        batch_size: The batch size to use for the M-step.
+        momentum: The momentum to use for the M-step.
+        termination_cond: The termination condition to use for the nested sampler.
+        solver: The solver to use for the M-step. Either 'adam' or 'armijo'.
+        verbose: Whether to print progress verbosely.
+    """
+    model: Model
+    ns_kwargs: Dict[str, Any]
+    max_num_epochs: int = 50
+    gtol: float = 1e-2
+    log_Z_ftol: float = 1.
+    log_Z_atol: float = 1e-4
+    batch_size: int = 128
+    termination_cond: Optional[TerminationCondition] = None
+    solver: str = 'armijo'
+    verbose: bool = False
+
+    def __post_init__(self):
+        if 'max_samples' not in self.ns_kwargs:
+            raise ValueError("ns_kwargs must contain 'max_samples'.")
         self._e_step = self._create_e_step()
         self._m_step = self._create_m_step_stochastic()
 
     def _create_e_step(self):
         """
         Create a compiled function that runs nested sampling and returns trimmed results.
 
         Returns:
             A compiled function that runs nested sampling and returns trimmed results.
         """
 
         def _ns_solve(params: hk.MutableParams, key: random.PRNGKey) -> Tuple[
             IntArray, StaticStandardNestedSamplerState]:
             model = self.model(params=params)
-            ns = DefaultNestedSampler(model=model, **self._ns_kwargs)
-            termination_reason, state = ns(key)
+            ns = DefaultNestedSampler(model=model, **self.ns_kwargs)
+            termination_reason, state = ns(key, self.termination_cond)
             return termination_reason, state
 
         # Ahead of time compile the function
-        ns_compiled = jax.jit(_ns_solve).lower(self.model.params, random.PRNGKey(42)).compile()
+        t0 = time.time()
+        ns_solve_compiled = jax.jit(_ns_solve).lower(self.model.params, random.PRNGKey(42)).compile()
+        if self.verbose:
+            logger.info(f"E-step compilation time: {time.time() - t0:.2f}s")
+        ns = DefaultNestedSampler(model=self.model(params=self.model.params), **self.ns_kwargs)
 
         def _e_step(key: PRNGKey, params: hk.MutableParams, p_bar: tqdm) -> NestedSamplerResults:
             p_bar.set_description(f"Running E-step... {p_bar.desc}")
-            termination_reason, state = ns_compiled(params, key)
-            ns = DefaultNestedSampler(model=self.model(params=params), **self._ns_kwargs)
-            # Trim now
+            termination_reason, state = ns_solve_compiled(params, key)
+            # Trim results
             return ns.to_results(termination_reason=termination_reason, state=state, trim=True)
 
         return _e_step
 
     def e_step(self, key: PRNGKey, params: hk.MutableParams, p_bar: tqdm) -> NestedSamplerResults:
         """
         The E-step is just nested sampling.
@@ -141,19 +142,19 @@
 
         # The E-step is just nested sampling
         return self._e_step(key, params, p_bar)
 
     def _m_step_iterator(self, key: PRNGKey, data: MStepData):
         num_samples = int(data.U_samples.shape[0])
         permutation = jax.random.permutation(key, num_samples)
-        num_batches = num_samples // self._batch_size
+        num_batches = num_samples // self.batch_size
         if num_batches == 0:
             raise RuntimeError("Batch size is too large for number of samples.")
         for i in range(num_batches):
-            perm = permutation[i * self._batch_size:(i + 1) * self._batch_size]
+            perm = permutation[i * self.batch_size:(i + 1) * self.batch_size]
             batch = MStepData(
                 U_samples=data.U_samples[perm],
                 log_weights=data.log_weights[perm]
             )
             yield batch
 
     def _create_m_step_stochastic(self):
@@ -167,29 +168,51 @@
             # We add the log_Z_mean because log_dp_mean is normalised
             log_Z = logsumexp(log_dZ)
             return log_Z
 
         def loss(params: hk.MutableParams, data: MStepData):
             log_Z, grad = jax.value_and_grad(log_evidence, argnums=0)(params, data)
             obj = -log_Z
-            grad = jax.tree_map(jnp.negative, grad)
+            grad = jax.tree.map(jnp.negative, grad)
+
+            # If objective is -+inf, or nan, then the gradient is nan
+            grad = jax.tree.map(lambda x: jnp.where(jnp.isfinite(obj), x, jnp.zeros_like(x)), grad)
+
+            # Clip the gradient
+            grad = jax.tree.map(lambda x: jnp.clip(x, -10, 10), grad)
+
             aux = (log_Z,)
-            if self._verbose:
-                jax.debug.print("log_Z={log_Z}", log_Z=log_Z)
+            if self.verbose:
+                jax.debug.print("(minibatch) log_Z={log_Z}", log_Z=log_Z)
             return (obj, aux), grad
 
-        solver = ArmijoSGD(
-            fun=loss,
-            has_aux=True,
-            value_and_grad=True,
-            jit=True,
-            unroll=False,
-            verbose=self._verbose,
-            momentum=self.momentum
-        )
+        if self.solver == 'adam':
+            solver = jaxopt.OptaxSolver(
+                fun=loss,
+                opt=optax.adam(learning_rate=1e-2),
+                has_aux=True,
+                value_and_grad=True,
+                jit=True,
+                unroll=False,
+                verbose=self.verbose,
+                maxiter=1000
+            )
+        elif self.solver == 'armijo':
+            solver = ArmijoSGD(
+                fun=loss,
+                has_aux=True,
+                value_and_grad=True,
+                jit=True,
+                unroll=False,
+                verbose=self.verbose,
+                momentum=0.,  # momentum does not help
+                maxiter=1000
+            )
+        else:
+            raise ValueError(f"Unknown solver {self.solver}")
 
         def _m_step_stochastic(key: PRNGKey, params: hk.MutableParams, data: MStepData) -> Tuple[hk.MutableParams, Any]:
             """
             The M-step is just evidence maximisation.
 
             Args:
                 key: The random number generator key.
@@ -220,27 +243,27 @@
 
             log_Z, _ = cumulative_op_static(op=op, init=jnp.asarray(-jnp.inf, float_type), xs=data)
             return log_Z
 
         def loss(params: hk.MutableParams, data: MStepData):
             log_Z, grad = jax.value_and_grad(log_evidence, argnums=0)(params, data)
             obj = -log_Z
-            grad = jax.tree_map(jnp.negative, grad)
+            grad = jax.tree.map(jnp.negative, grad)
             aux = (log_Z,)
-            if self._verbose:
+            if self.verbose:
                 jax.debug.print("log_Z={log_Z}", log_Z=log_Z)
             return (obj, aux), grad
 
         solver = NonlinearCG(
             fun=loss,
             has_aux=True,
             value_and_grad=True,
             jit=True,
             unroll=False,
-            verbose=self._verbose
+            verbose=self.verbose
         )
 
         @partial(jax.jit, static_argnums=(0,))
         def _m_step(key: PRNGKey, params: hk.MutableParams, data: MStepData) -> Tuple[hk.MutableParams, Any]:
             """
             The M-step is just evidence maximisation.
 
@@ -274,46 +297,48 @@
         # next_power_2 pad
         num_samples = int(ns_results.total_num_samples)
         n = next_power_2(num_samples)
 
         p_bar.set_description(f"Running M-step ({num_samples} samples padded to {n})... {p_bar.desc}")
 
         def _pad_to_n(x, fill_value, dtype):
+            if x.shape[0] == n:
+                return x
             return jnp.concatenate([x, jnp.full((n - x.shape[0],) + x.shape[1:], fill_value, dtype)], axis=0)
 
         log_weights = ns_results.log_dp_mean - ns_results.log_L_samples + ns_results.log_Z_mean
         data = MStepData(
             U_samples=_pad_to_n(ns_results.U_samples, 0.5, float_type),
             log_weights=_pad_to_n(log_weights, -jnp.inf, float_type)
         )
         desc = p_bar.desc
         last_params = params
         epoch = 0
         log_Z = None
         while epoch < self.max_num_epochs:
             params, (log_Z,) = self._m_step(key=key, params=params, data=data)
-            l_oo = jax.tree_map(lambda x, y: jnp.max(jnp.abs(x - y)), last_params, params)
+            l_oo = jax.tree.map(lambda x, y: jnp.max(jnp.abs(x - y)) if np.size(x) > 0 else 0.,
+                                last_params, params)
             last_params = params
             p_bar.set_description(f"{desc}: Epoch {epoch}: log_Z={log_Z}, l_oo={l_oo}")
-            if all(_l_oo < self.gtol for _l_oo in jax.tree_leaves(l_oo)):
+            if all(_l_oo < self.gtol for _l_oo in jax.tree.leaves(l_oo)):
                 break
             epoch += 1
 
         return params, log_Z
 
     def train(self, num_steps: int = 10, params: Optional[hk.MutableParams] = None) -> \
             Tuple[
                 NestedSamplerResults, hk.MutableParams]:
         """
         Train the model using EM for num_steps.
 
         Args:
             num_steps: The number of steps to train for, or until convergence.
             params: The initial parameters to use. If None, then the model's params are used.
-            do_final_e_step: Whether to do a final E-step after training, for updated evidence.
 
         Returns:
             The trained parameters.
         """
         if params is None:
             params = self.model.params
 
@@ -334,15 +359,15 @@
                     f"Step {step}: log Z = {ns_results.log_Z_mean:.4f} +- {ns_results.log_Z_uncert:.4f}"
                 )
             ns_results = self.e_step(key=key_e_stek, params=params, p_bar=p_bar)
             # Update progress bar description
 
             # Check termination condition
             log_Z_change = jnp.abs(ns_results.log_Z_mean - log_Z)
-            if log_Z_change < max(self.log_Z_ftol * ns_results.log_Z_uncert, self.log_Z_atol):
+            if log_Z_change < max(float(self.log_Z_ftol * ns_results.log_Z_uncert), self.log_Z_atol):
                 p_bar.set_description(f"Convergence achieved at step {step}.")
                 break
 
             # Update log_Z and log_Z_uncert values
             log_Z = ns_results.log_Z_mean
 
             # Execute the m_step
```

### Comparing `jaxns-2.4.9/jaxns/experimental/global_optimisation.py` & `jaxns-2.5.0/jaxns/experimental/global_optimisation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import io
-import logging
 from typing import NamedTuple, Optional, Union, TextIO, Tuple, List
 
+import jax
 import jax.nn
 import jax.numpy as jnp
 import numpy as np
-from jax import lax, random, pmap, tree_map
+from jax import lax, random, pmap
 from jax._src.lax import parallel
 from jax._src.scipy.special import logit
 from jaxopt import NonlinearCG
 
 from jaxns.framework.bases import BaseAbstractModel
+from jaxns.internals.logging import logger
 from jaxns.internals.maps import remove_chunk_dim
 from jaxns.internals.types import PRNGKey, StaticStandardNestedSamplerState, BoolArray, StaticStandardSampleCollection, \
     int_type, Sample, IntArray, UType, FloatArray, LikelihoodInputType, XType
 from jaxns.nested_sampler.standard_static import draw_uniform_samples, _inter_sync_shrinkage_process, \
     create_init_termination_register
 from jaxns.samplers.bases import BaseAbstractSampler
 from jaxns.utils import _bit_mask
 
-logger = logging.getLogger('jaxns')
-
 __all__ = [
     'GlobalOptimisationResults',
     'GlobalOptimisationTerminationCondition',
     'GlobalOptimisationState',
     'SimpleGlobalOptimisation'
 ]
 
@@ -132,24 +131,28 @@
         done, termination_reason = _set_done_bit(reached_log_L_contour, 1,
                                                  done=done, termination_reason=termination_reason)
 
     if term_cond.rtol is not None:
         # relative spread of log-likelihood values below threshold
         max_log_L = jnp.max(state.samples.log_L)
         min_log_L = jnp.min(state.samples.log_L)
-        diff_log_L = jnp.abs(max_log_L - min_log_L)
-        reached_rtol = diff_log_L <= 0.5 * term_cond.rtol * jnp.abs(max_log_L + min_log_L)
+        diff_log_L = jnp.abs(max_log_L - min_log_L)  # NaN = inf - inf
+        diff_log_L = jnp.where(jnp.isnan(diff_log_L), jnp.inf, diff_log_L)
+        mean_log_L = 0.5 * jnp.abs(max_log_L + min_log_L)  # = inf - inf
+        mean_log_L = jnp.where(jnp.isnan(mean_log_L), jnp.inf, mean_log_L)
+        reached_rtol = diff_log_L <= term_cond.rtol * mean_log_L
         done, termination_reason = _set_done_bit(reached_rtol, 2,
                                                  done=done, termination_reason=termination_reason)
 
     if term_cond.atol is not None:
         # absolute spread of log-likelihood values below threshold
         max_log_L = jnp.max(state.samples.log_L)
         min_log_L = jnp.min(state.samples.log_L)
-        diff_log_L = jnp.abs(max_log_L - min_log_L)
+        diff_log_L = jnp.abs(max_log_L - min_log_L)  # NaN = inf - inf
+        diff_log_L = jnp.where(jnp.isnan(diff_log_L), jnp.inf, diff_log_L)
         reached_atol = diff_log_L <= term_cond.atol
         done, termination_reason = _set_done_bit(reached_atol, 3,
                                                  done=done, termination_reason=termination_reason)
 
     if term_cond.min_efficiency is not None:
         # efficiency below threshold
         efficiency = state.samples.log_L.shape[0] / jnp.sum(state.samples.num_likelihood_evaluations)
@@ -225,15 +228,15 @@
 
         k = sampler.num_phantom()
         if k > 0:
             def _repeat(x):
                 return jnp.repeat(x, (k + 1), axis=0)
 
             fake_state = fake_state._replace(
-                sample_collection=tree_map(_repeat, fake_state.sample_collection)
+                sample_collection=jax.tree.map(_repeat, fake_state.sample_collection)
             )
 
         fake_state, fake_termination_register = _inter_sync_shrinkage_process(
             init_state=fake_state,
             sampler=sampler,
             num_samples=num_samples * (1 + k),
             init_termination_register=create_init_termination_register()
@@ -251,15 +254,15 @@
             )
 
             def _select(x):
                 x = jnp.reshape(x, ((k + 1), num_samples) + x.shape[1:])  # [k+1, N, ...]
                 return x[choose_idx, jnp.arange(num_samples)]  # [N, ...]
 
             fake_state = fake_state._replace(
-                sample_collection=tree_map(
+                sample_collection=jax.tree.map(
                     _select,
                     fake_state.sample_collection
                 )
             )
 
         samples = Sample(
             U_sample=fake_state.sample_collection.U_samples,
@@ -361,15 +364,25 @@
         best_idx = jnp.argmax(state.samples.log_L)
         U_solution = state.samples.U_sample[best_idx]
         X_solution = self.model.transform(U_solution)
         solution = self.model.prepare_input(U_solution)
         max_log_L = state.samples.log_L[best_idx]
         min_log_L = jnp.min(state.samples.log_L)
         relative_spread = 2. * jnp.abs(max_log_L - min_log_L) / jnp.abs(max_log_L + min_log_L)
+        relative_spread = jnp.where(
+            jnp.isnan(relative_spread),
+            jnp.asarray(jnp.inf, relative_spread.dtype),
+            relative_spread
+        )
         absolute_spread = jnp.abs(max_log_L - min_log_L)
+        absolute_spread = jnp.where(
+            jnp.isnan(absolute_spread),
+            jnp.asarray(jnp.inf, absolute_spread.dtype),
+            absolute_spread
+        )
         return GlobalOptimisationResults(
             U_solution=state.samples.U_sample[best_idx],
             X_solution=X_solution,
             solution=solution,
             log_L_solution=state.samples.log_L[best_idx],
             num_likelihood_evaluations=state.num_likelihood_evaluations,
             num_samples=state.num_samples,
```

### Comparing `jaxns-2.4.9/jaxns/experimental/public.py` & `jaxns-2.5.0/jaxns/experimental/public.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.4.9/jaxns/experimental/tests/test_global_optimisation.py` & `jaxns-2.5.0/jaxns/experimental/tests/test_global_optimisation.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.4.9/jaxns/framework/abc.py` & `jaxns-2.5.0/jaxns/framework/abc.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.4.9/jaxns/framework/bases.py` & `jaxns-2.5.0/jaxns/framework/bases.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from abc import abstractmethod
 from typing import Tuple, Optional, Generator, Callable
 
 import jax.numpy as jnp
+import numpy as np
+from jax import lax
 
 from jaxns.framework.abc import AbstractModel, AbstractPrior, AbstractDistribution
 from jaxns.internals.shapes import tuple_prod
 from jaxns.internals.types import LikelihoodInputType
 from jaxns.internals.types import LikelihoodType, UType, XType, RandomVariableType, MeasureType
 
 __all__ = [
@@ -87,23 +89,23 @@
         Args:
             X: X-space representation
 
         Returns:
             log probability of the prior
         """
         log_prob = self._log_prob(X)
-        if log_prob.size > 1:
+        if np.size(log_prob) > 1:
             log_prob = jnp.sum(log_prob)
         if log_prob.shape != ():
-            log_prob = log_prob.reshape(())
+            log_prob = lax.reshape(log_prob, ())
         return log_prob
 
 
 PriorModelGen = Generator[BaseAbstractPrior, RandomVariableType, LikelihoodInputType]
-PriorModelType = Callable[[], PriorModelGen]
+PriorModelType = Callable[[...], PriorModelGen]
 
 
 class BaseAbstractModel(AbstractModel):
     """
     The base model class with public methods.
     """
```

### Comparing `jaxns-2.4.9/jaxns/framework/distribution.py` & `jaxns-2.5.0/jaxns/framework/wrapped_tfp_distribution.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import tensorflow_probability.substrates.jax as tfp
 
 from jaxns.framework.bases import BaseAbstractDistribution
 from jaxns.internals.types import FloatArray, IntArray, BoolArray
 
 __all__ = [
-    "Distribution",
+    "WrappedTFPDistribution",
     "InvalidDistribution"
 ]
 
 tfpd = tfp.distributions
 
 
 class InvalidDistribution(Exception):
@@ -42,17 +42,17 @@
             dist = dist.distribution
             continue
         break
     # Must reverse the chain because the first distribution is the last in the chain.
     return chain[::-1]
 
 
-class Distribution(BaseAbstractDistribution):
+class WrappedTFPDistribution(BaseAbstractDistribution):
     """
-    Represents a distribution, which must have defined forward and inverse transformations, and a log_prob.
+    Represents a wrapped TFP distribution.
     """
 
     def __init__(self, dist: tfpd.Distribution):
         self.dist_chain = distribution_chain(dist)
         check_dist = self.dist_chain[0]
         if isinstance(self.dist_chain[0], tfpd.Sample):
             check_dist = self.dist_chain[0].distribution
```

### Comparing `jaxns-2.4.9/jaxns/framework/model.py` & `jaxns-2.5.0/jaxns/framework/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-import logging
+import warnings
 from typing import Optional
 from uuid import uuid4
 
 import numpy as np
 from jax import random, vmap, jit, numpy as jnp
 
+from jaxns.internals.logging import logger
+
 try:
     import haiku as hk
 except ImportError:
-    print("You must `pip install dm-haiku` first.")
+    warnings.warn("You must `pip install dm-haiku` first.")
     raise
 
 from jaxns.framework.bases import BaseAbstractModel, PriorModelType
 from jaxns.framework.ops import transform, prepare_input, compute_log_prob_prior, compute_log_likelihood, parse_prior, \
     parse_joint, transform_parametrised
 from jaxns.internals.types import PRNGKey, FloatArray, float_type, LikelihoodType, UType, XType, LikelihoodInputType
 
 __all__ = [
     'Model'
 ]
 
-logger = logging.getLogger('jaxns')
-
 
 class Model(BaseAbstractModel):
     """
     Represents a Bayesian model in terms of a generative prior, and likelihood function.
     """
 
     def __init__(self, prior_model: PriorModelType, log_likelihood: LikelihoodType,
@@ -36,15 +36,15 @@
         # ).apply(params=self._params, rng=None)
         if params is None:
             params = self.init_params(rng=random.PRNGKey(0))
         self._params = params
         # Parse the prior model to get place holders
         self.__U_placeholder, self.__X_placeholder = hk.transform(
             lambda: parse_prior(prior_model=self.prior_model)
-        ).apply(params=self._params, rng=None)
+        ).apply(params=self._params, rng=random.PRNGKey(0))
         self._id = str(uuid4())  # Used for making sure it's hashable, so it can be used as a key in a dict.
 
     @property
     def num_params(self) -> int:
         if self._params is None:
             raise RuntimeError("Model has not been initialised")
         return hk.data_structures.tree_size(self._params)
@@ -133,54 +133,56 @@
 
         return hk.transform(_sample_U).apply(params=self._params, rng=key)
 
     def transform(self, U: UType) -> XType:
         def _transform():
             return transform(U=U, prior_model=self.prior_model)
 
-        return hk.transform(_transform).apply(params=self._params, rng=None)
+        return hk.transform(_transform).apply(params=self._params, rng=random.PRNGKey(0))
 
     def transform_parametrised(self, U: UType) -> XType:
         def _transform():
             return transform_parametrised(U=U, prior_model=self.prior_model)
 
-        return hk.transform(_transform).apply(params=self._params, rng=None)
+        return hk.transform(_transform).apply(params=self._params, rng=random.PRNGKey(0))
 
     def forward(self, U: UType, allow_nan: bool = False) -> FloatArray:
         if self._params is None:
             raise RuntimeError("Model has not been initialised")
 
         def _forward():
             return compute_log_likelihood(U=U, prior_model=self.prior_model, log_likelihood=self.log_likelihood,
                                           allow_nan=allow_nan)
 
-        return hk.transform(_forward).apply(params=self._params, rng=None)
+        return hk.transform(_forward).apply(params=self._params, rng=random.PRNGKey(0))
 
     def log_prob_prior(self, U: UType) -> FloatArray:
         if self._params is None:
             raise RuntimeError("Model has not been initialised")
 
         def _log_prob_prior():
             return compute_log_prob_prior(U=U, prior_model=self.prior_model)
 
-        return hk.transform(_log_prob_prior).apply(params=self._params, rng=None)
+        return hk.transform(_log_prob_prior).apply(params=self._params, rng=random.PRNGKey(0))
 
     def prepare_input(self, U: UType) -> LikelihoodInputType:
         if self._params is None:
             raise RuntimeError("Model has not been initialised")
 
         def _prepare_input():
             return prepare_input(U=U, prior_model=self.prior_model)
 
-        return hk.transform(_prepare_input).apply(params=self._params, rng=None)
+        return hk.transform(_prepare_input).apply(params=self._params, rng=random.PRNGKey(0))
 
     def sanity_check(self, key: PRNGKey, S: int):
         U = jit(vmap(self.sample_U))(random.split(key, S))
         log_L = jit(vmap(lambda u: self.forward(u, allow_nan=True)))(U)
         logger.info("Sanity check...")
         for _U, _log_L in zip(U, log_L):
             if jnp.isnan(_log_L):
-                logger.info(f"Found bad point: {_U} -> {self.transform(_U)}")
+                logger.info(f"Found bad point:"
+                             f"\n{_U} -> {self.transform(_U)}"
+                             f"\n -> {self.transform_parametrised(_U)}")
         assert not any(np.isnan(log_L))
         logger.info("Sanity check passed")
         if 'parsed_prior' in self.__dict__:
             del self.__dict__['parsed_prior']
```

### Comparing `jaxns-2.4.9/jaxns/framework/ops.py` & `jaxns-2.5.0/jaxns/framework/ops.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,53 @@
-from typing import Tuple
+import inspect
+import warnings
+from typing import Tuple, Callable
 
 import jax
-from jax import numpy as jnp
+from jax import numpy as jnp, lax
 
-from jaxns.framework.bases import PriorModelType, BaseAbstractPrior
-from jaxns.framework.prior import InvalidPriorName, SingularPrior
+from jaxns.framework.bases import PriorModelType, BaseAbstractPrior, PriorModelGen
+from jaxns.framework.prior import InvalidPriorName, SingularPrior, Prior
 from jaxns.internals.types import UType, XType, float_type, LikelihoodInputType, FloatArray, LikelihoodType, PRNGKey, \
     isinstance_namedtuple
 
 __all__ = [
     'simulate_prior_model'
 ]
 
 
+def _get_prior_model_gen(prior_model: PriorModelType) -> PriorModelGen:
+    gen = prior_model()
+    # Check if gen is a generator
+    if not inspect.isgenerator(gen):
+        warnings.warn("The provided prior_model is not a generator, this may mean you forget `yield` statements. "
+                      "This means there are no Bayesian variables.")
+
+        def dummy_prior_model(output):
+            _ = yield Prior(0.)
+            return output
+
+        # Make an empty generator that returns the output.
+        gen = dummy_prior_model(gen)
+    return gen
+
+
 def compute_U_ndims(prior_model: PriorModelType) -> int:
     """
     Computes placeholders of model.
 
     Args:
         prior_model: a callable that produces a prior model generator
 
     Returns:
         number of U dims
     """
     U_ndims = 0
-    gen = prior_model()
+    gen = _get_prior_model_gen(prior_model=prior_model)
+
     prior_response = None
     names = set()
     while True:
         try:
             prior: BaseAbstractPrior = gen.send(prior_response)
             d = prior.base_ndims
             U_ndims += d
@@ -66,15 +85,16 @@
     Args:
         prior_model: a callable that produces a prior model generator
 
     Returns:
         U placeholder, X placeholder
     """
     U_ndims = 0
-    gen = prior_model()
+    gen = _get_prior_model_gen(prior_model=prior_model)
+
     prior_response = None
     names = set()
     X_placeholder: XType = dict()
     while True:
         try:
             prior: BaseAbstractPrior = gen.send(prior_response)
             d = prior.base_ndims
@@ -101,15 +121,16 @@
     Args:
         prior_model: a callable that produces a prior model generator
 
     Returns:
         U placeholder, X placeholder
     """
     U_ndims = 0
-    gen = prior_model()
+    gen = _get_prior_model_gen(prior_model=prior_model)
+
     prior_response = None
     names = set()
     X_placeholder: XType = dict()
     while True:
         try:
             prior: BaseAbstractPrior = gen.send(prior_response)
             d = prior.base_ndims
@@ -141,15 +162,16 @@
         U: [U_ndims] a flat array of i.i.d. samples of U[0,1]
         prior_model: a callable that produces a prior model generator
 
     Returns:
         the prior variables
     """
 
-    gen = prior_model()
+    gen = _get_prior_model_gen(prior_model=prior_model)
+
     prior_response = None
     names = set()
     X_collection = dict()
     idx = 0
     while True:
         try:
             prior: BaseAbstractPrior = gen.send(prior_response)
@@ -176,15 +198,16 @@
         U: [U_ndims] a flat array of i.i.d. samples of U[0,1]
         prior_model: a callable that produces a prior model generator
 
     Returns:
         the parametrised prior variables
     """
 
-    gen = prior_model()
+    gen = _get_prior_model_gen(prior_model=prior_model)
+
     prior_response = None
     names = set()
     Y_collection = dict()
     idx = 0
     while True:
         try:
             prior: BaseAbstractPrior = gen.send(prior_response)
@@ -211,15 +234,16 @@
         U: [U_ndims] a flat array of i.i.d. samples of U[0,1]
         prior_model: a callable that produces a prior model generator
 
     Returns:
         the conditional variables of likelihood model
     """
 
-    gen = prior_model()
+    gen = _get_prior_model_gen(prior_model=prior_model)
+
     prior_response = None
     idx = 0
     while True:
         try:
             prior: BaseAbstractPrior = gen.send(prior_response)
             d = prior.base_ndims
             u = jnp.reshape(U[idx:idx + d], prior.base_shape)
@@ -241,15 +265,16 @@
         U: [U_ndims] a flat array of i.i.d. samples of U[0,1]
         prior_model: a callable that produces a prior model generator
 
     Returns:
         prior log-density
     """
 
-    gen = prior_model()
+    gen = _get_prior_model_gen(prior_model=prior_model)
+
     prior_response = None
     log_prob = []
     idx = 0
     while True:
         try:
             prior: BaseAbstractPrior = gen.send(prior_response)
             d = prior.base_ndims
@@ -275,14 +300,56 @@
 
     Returns:
         log-likelihood
     """
 
     V = prepare_input(U=U, prior_model=prior_model)
     log_L = jnp.asarray(log_likelihood(*V), float_type)
-    if not allow_nan:
-        log_L = jnp.where(jnp.isnan(log_L), -jnp.inf, log_L)
     if log_L.size != 1:
         raise ValueError(f"Log likelihood should be scalar, but got {log_L.shape}.")
     if log_L.shape != ():
-        log_L = jnp.reshape(log_L, ())
+        log_L = lax.reshape(log_L, ())
+    if not allow_nan:
+        is_nan = lax.ne(log_L, log_L)
+        log_L = lax.select(is_nan, jnp.asarray(-jnp.inf, log_L.dtype), log_L)
     return log_L
+
+
+def memoize_prior_model(prior_model: PriorModelType, *args, **kwargs) -> Callable:
+    """
+    Memoize the prior model into a pure function. This can be used, e.g. to compute jacobians, or gradients inside a
+    prior model.
+
+    Args:
+        prior_model: a prior model
+        *args: inputs
+        **kwargs: inputs
+
+    Returns:
+        a pure function that takes the inputs and passes the prior values appropriately at execution time.
+    """
+    gen = prior_model(*args, **kwargs)
+    prior_response = None
+    stack = []
+    while True:
+        try:
+            prior: BaseAbstractPrior = gen.send(prior_response)
+            prior_response = yield prior
+            stack.append(prior_response)
+        except StopIteration as e:
+            # output = e.value
+            break
+
+    def _pure_fn(*args, **kwargs):
+        gen = prior_model(*args, **kwargs)
+        stack_iter = iter(stack)
+        prior_response = None
+        while True:
+            try:
+                _ = gen.send(prior_response)
+                prior_response = next(stack_iter)
+            except StopIteration as e:
+                output = e.value
+                break
+        return output
+
+    return _pure_fn
```

### Comparing `jaxns-2.4.9/jaxns/framework/prior.py` & `jaxns-2.5.0/jaxns/framework/prior.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-import logging
+import warnings
 from typing import Tuple, Optional, Union
 
 import haiku as hk
 import jax.nn
 import tensorflow_probability.substrates.jax as tfp
 from jax import numpy as jnp
 
 from jaxns.framework.bases import BaseAbstractPrior, BaseAbstractDistribution
-from jaxns.framework.distribution import Distribution
+from jaxns.framework.wrapped_tfp_distribution import WrappedTFPDistribution
 from jaxns.internals.types import FloatArray, IntArray, BoolArray, XType, UType, float_type
 
 tfpd = tfp.distributions
 
 __all__ = [
     "Prior",
     "InvalidPriorName"
 ]
 
-logger = logging.getLogger('jaxns')
-
 
 class InvalidPriorName(Exception):
     """
     Raised when a prior name is already taken.
     """
 
     def __init__(self, name: Optional[str] = None):
@@ -31,58 +29,60 @@
 
 class SingularPrior(BaseAbstractPrior):
     """
     Represents a singular prior, which has no inverse transformation, but does have a log_prob
         (at the singular value).
     """
 
-    def __init__(self, value: jnp.ndarray, dist: BaseAbstractDistribution, name: Optional[str] = None):
+    def __init__(self, value: jnp.ndarray, base_prior: BaseAbstractPrior, name: Optional[str] = None):
         super().__init__(name=name)
         self.value = value
-        self.dist = dist
+        self.base_prior = base_prior
 
     def __repr__(self):
-        return f"{self.value} -> {self.dist}"
+        return f"{self.value} -> {self.base_prior}"
 
     def _dtype(self):
-        return self.dist.dtype
+        return self.base_prior.dtype
 
     def _base_shape(self) -> Tuple[int, ...]:
         return (0,)  # Singular prior has no base shape
 
     def _shape(self) -> Tuple[int, ...]:
-        return self.dist.shape
+        return self.base_prior.shape
 
     def _forward(self, U: UType) -> Union[FloatArray, IntArray, BoolArray]:
         return self.value
 
-    def _inverse(self, X: XType) -> FloatArray:
+    def _inverse(self, X: XType) -> UType:
         return jnp.asarray([], float_type)
 
     def _log_prob(self, X: XType) -> FloatArray:
-        return self.dist.log_prob(X)
+        return self.base_prior.log_prob(X)
 
 
 class Prior(BaseAbstractPrior):
     """
     Represents a generative prior.
     """
 
-    def __init__(self, dist_or_value: Union[tfpd.Distribution, BaseAbstractDistribution, jnp.ndarray],
+    def __init__(self, dist_or_value: Union[tfpd.Distribution, FloatArray, IntArray, BoolArray],
                  name: Optional[str] = None):
         super(Prior, self).__init__(name=name)
         if isinstance(dist_or_value, tfpd.Distribution):
+            self._dist = WrappedTFPDistribution(dist_or_value)
             self._type = 'dist'
-            self._dist = Distribution(dist_or_value)
-        elif isinstance(dist_or_value, BaseAbstractDistribution):
-            self._type = 'dist'
-            self._dist = dist_or_value
         else:
+            try:
+                self._value = jnp.asarray(dist_or_value)
+            except TypeError:
+                raise ValueError(f"Could not convert {dist_or_value} to array.")
+            except Exception as e:
+                raise e
             self._type = 'value'
-            self._value = jnp.asarray(dist_or_value)
         self.name = name
 
     @property
     def dist(self) -> BaseAbstractDistribution:
         if self._type != 'dist':
             raise ValueError(f"Wrong type, got {self._type}")
         return self._dist
@@ -137,53 +137,62 @@
         if self._type == 'value':
             return jnp.asarray(0., float_type)
         elif self._type == 'dist':
             return self.dist.log_prob(X=X)
         else:
             raise NotImplementedError()
 
-    def parametrised(self) -> SingularPrior:
+    def parametrised(self, random_init: bool = False) -> SingularPrior:
         """
-        Convert this prior into a non-Bayesian parameter, that takes a single value in the model, but still has an associated
-        log_prob. The parameter is registered as a `hk.Parameter` with added `_param` name suffix.
+        Convert this prior into a non-Bayesian parameter, that takes a single value in the model, but still has an
+        associated log_prob. The parameter is registered as a `hk.Parameter` with added `_param` name suffix. Prior
+        must have a name.
+
+        Args:
+            random_init: whether to initialise the parameter randomly or at the median of the distribution.
 
         Returns:
             A singular prior.
+
+        Raises:
+            ValueError: if the prior has no name.
         """
-        if self._type == 'value':
-            raise ValueError("Cannot parametrise a prior without distribution.")
-        return prior_to_parametrised_singular(self)
+        return prior_to_parametrised_singular(self, random_init=random_init)
 
 
-def prior_to_parametrised_singular(prior: Prior) -> SingularPrior:
+def prior_to_parametrised_singular(prior: BaseAbstractPrior, random_init: bool = False) -> SingularPrior:
     """
     Convert a prior into a non-Bayesian parameter, that takes a single value in the model, but still has an associated
     log_prob. The parameter is registered as a `hk.Parameter` with added `_param` name suffix.
 
     To constrain the parameter we use a Normal parameter with centre on unit cube, and scale covering the whole cube,
     as the base representation. This base representation covers the whole real line and be reliably used with SGD, etc.
 
     Args:
         prior: any prior
+        random_init: whether to initialise the parameter randomly or at the median of the distribution.
 
     Returns:
         A parameter representing the prior.
     """
     if prior.name is None:
         raise ValueError("Prior must have a name to be parametrised.")
     name = f"{prior.name}_param"
     # Initialises at median of distribution.
-    init_value = jnp.zeros(prior.base_shape, dtype=float_type)
+    if random_init:
+        init_value = jax.random.normal(hk.next_rng_key(), shape=prior.base_shape, dtype=float_type)
+    else:
+        init_value = jnp.zeros(prior.base_shape, dtype=float_type)
     if init_value.size == 0:
-        logger.warning(f"Creating a zero-sized parameter for {prior.name}. Probably unintended.")
+        warnings.warn(f"Creating a zero-sized parameter for {prior.name}. Probably unintended.")
     norm_U_base_param = hk.get_parameter(
         name=name,
         shape=prior.base_shape,
         dtype=float_type,
         init=hk.initializers.Constant(init_value)
     )
     # transform [-inf, inf] -> [0,1]
     # Sigmoid is faster than ndtr to save FLOPs
     # U_base_param = ndtr(norm_U_base_param)
     U_base_param = jax.nn.sigmoid(norm_U_base_param)
     param = prior.forward(U_base_param)
-    return SingularPrior(value=param, dist=prior.dist, name=prior.name)
+    return SingularPrior(value=param, base_prior=prior, name=prior.name)
```

### Comparing `jaxns-2.4.9/jaxns/framework/tests/test_model.py` & `jaxns-2.5.0/jaxns/experimental/tests/test_evidence_maximisation.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,70 +1,65 @@
-from typing import NamedTuple
+import time
 
-import jax.random
+import jax
+import numpy as np
 import pytest
 import tensorflow_probability.substrates.jax as tfp
-from jax import numpy as jnp
 
-from jaxns.framework.model import Model
-from jaxns.framework.prior import Prior
+from jaxns import Prior, Model
+from jaxns.experimental import EvidenceMaximisation
 
 tfpd = tfp.distributions
 
 
-def test_gh144():
-    class Output(NamedTuple):
-        x: jnp.ndarray
-        y: jnp.ndarray
-
+@pytest.mark.parametrize("solver", ['adam', 'armijo'])
+def test_basic(solver):
     def prior_model():
-        x = yield Prior(dist_or_value=jnp.asarray(0.))
-        y = yield Prior(dist_or_value=jnp.asarray(0.))
-        return Output(x, y)
+        x = yield Prior(tfpd.Uniform(0., 1.))
+        y = yield Prior(tfpd.Normal(x, 1.), name='y').parametrised()
+        sigma = yield Prior(tfpd.Exponential(1.))
+        return y, sigma
 
-    def log_likelihood(z: Output):
-        return z.x + z.y
+    def log_likelihood(y, sigma):
+        return tfpd.Normal(y, sigma).log_prob(0.)
 
     model = Model(prior_model=prior_model, log_likelihood=log_likelihood)
-    assert model.U_ndims == 0
-    model.sanity_check(key=jax.random.PRNGKey(0), S=10)
-
 
-def test_gh95():
-    def prior_model():
-        x = yield Prior(dist_or_value=jnp.asarray(0.))
-        return x
+    em = EvidenceMaximisation(model=model, ns_kwargs=dict(max_samples=1e5), verbose=False, solver=solver)
+    t0 = time.time()
+    ns_results, params = em.train(num_steps=3)
+    print(f"Time taken ({solver}): {time.time() - t0}")
 
-    def log_likelihood(x):
-        return jnp.sum(x)
+    def change(x, y):
+        if np.size(x) > 0:
+            return np.any(np.abs(x - y) > 1e-2)
+        return True
 
-    model = Model(prior_model=prior_model, log_likelihood=log_likelihood)
-    assert model.U_ndims == 0
+    assert all(
+        change(p, p_) for p, p_ in zip(jax.tree.leaves(model.params), jax.tree.leaves(params)))
 
 
-def test_parametrised_singular():
+def test_basic_zero_size_param():
     def prior_model():
-        x = yield Prior(dist_or_value=jnp.asarray(0.), name='x').parametrised()
-        return x
+        x = yield Prior(tfpd.Uniform(0., 1.))
+        y = yield Prior(tfpd.Normal(x, 1.), name='y').parametrised()
+        z = yield Prior(0., name='z').parametrised()  # This is a zero size parameter
+        sigma = yield Prior(tfpd.Exponential(1.))
+        return y, z, sigma
 
-    def log_likelihood(x):
-        return jnp.sum(x)
-
-    with pytest.raises(ValueError, match="Cannot parametrise a prior without distribution."):
-        _ = Model(prior_model=prior_model, log_likelihood=log_likelihood)
+    def log_likelihood(y, z, sigma):
+        return tfpd.Normal(y, sigma).log_prob(0.) + z
 
+    model = Model(prior_model=prior_model, log_likelihood=log_likelihood)
 
-def test_parametrised():
-    def prior_model():
-        x = yield Prior(tfpd.Uniform(), name='x').parametrised()
-        return x
+    em = EvidenceMaximisation(model=model, ns_kwargs=dict(max_samples=1e5))
+    assert any(np.size(p) == 0 for p in jax.tree.leaves(model.params))
 
-    def log_likelihood(x):
-        return jnp.sum(x)
+    ns_results, params = em.train(num_steps=1)
 
-    model = Model(prior_model=prior_model, log_likelihood=log_likelihood)
-    assert model.num_params == 1
-    assert model.U_ndims == 0
+    def change(x, y):
+        if np.size(x) > 0:
+            return np.any(np.abs(x - y) > 1e-2)
+        return True
 
-    log_prob_joint = model.log_prob_joint(model.U_placeholder, allow_nan=True)
-    assert log_prob_joint.shape == ()
-    assert log_prob_joint == 0.5, "Didn't init at median of uniform"
+    assert all(
+        change(p, p_) for p, p_ in zip(jax.tree.leaves(model.params), jax.tree.leaves(params)))
```

### Comparing `jaxns-2.4.9/jaxns/internals/linalg.py` & `jaxns-2.5.0/jaxns/internals/linalg.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.4.9/jaxns/internals/log_semiring.py` & `jaxns-2.5.0/jaxns/internals/log_semiring.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.4.9/jaxns/internals/maps.py` & `jaxns-2.5.0/jaxns/internals/maps.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import inspect
-import logging
+import warnings
 from typing import TypeVar, Callable, Optional
 
 import jax
-from jax import tree_map, pmap, numpy as jnp, lax, tree_util
+from jax import pmap, numpy as jnp, lax
 
 from jaxns.internals.types import int_type
 
-logger = logging.getLogger(__name__)
-
 
 def replace_index(operand, update, start_index):
     """
     Replaces an index or slice with an update.
     If update is too big to respect start_index then start_index is shifted, which will give non-intuitive results.
     """
     if len(operand.shape) != len(update.shape):
@@ -45,17 +43,17 @@
         raise ValueError(f"function {f.__old_name__} has already done prepare_func_args.")
 
     (args, varargs, varkw, defaults, kwonlyargs, kwonlydefaults, annotations) = \
         inspect.getfullargspec(f)
 
     # TODO: this gets displayed each time we prepare a function. Using a cache would be cleaner for user.
     if varargs is not None:
-        logger.warning(f"Function {f.__name__} has *varargs parameter ({varargs}), and is being dropped.")
+        warnings.warn(f"Function {f.__name__} has *varargs parameter ({varargs}), and is being dropped.")
     if varkw is not None:
-        logger.warning(f"Function {f.__name__} has **varkw parameter ({varkw}), and is being dropped.")
+        warnings.warn(f"Function {f.__name__} has **varkw parameter ({varkw}), and is being dropped.")
 
     expected_keys = set(args + kwonlyargs)
 
     if defaults is None:  # no defaults
         num_defaults = 0
         defaults = ()
     else:
@@ -114,29 +112,29 @@
 
             _, result = lax.scan(body, (), (args, kwargs), unroll=unroll)
             return result
 
         if chunk_size > 1:
             # Get from first leaf
             if len(args) > 0:
-                batch_size = tree_util.tree_leaves(args)[0].shape[0]
+                batch_size = jax.tree.leaves(args)[0].shape[0]
             else:
-                batch_size = tree_util.tree_leaves(kwargs)[0].shape[0]
+                batch_size = jax.tree.leaves(kwargs)[0].shape[0]
             remainder = batch_size % chunk_size
             extra = (chunk_size - remainder) % chunk_size
             if extra > 0:
-                (args, kwargs) = tree_map(lambda x: _pad_extra(x, chunk_size), (args, kwargs))
-            (args, kwargs) = tree_map(
+                (args, kwargs) = jax.tree.map(lambda x: _pad_extra(x, chunk_size), (args, kwargs))
+            (args, kwargs) = jax.tree.map(
                 lambda x: jnp.reshape(x, (chunk_size, x.shape[0] // chunk_size) + x.shape[1:]),
                 (args, kwargs)
             )
             result = pmap(queue)(*args, **kwargs)  # [chunksize, batch_size // chunksize, ...]
-            result = tree_map(lambda x: jnp.reshape(x, (-1,) + x.shape[2:]), result)
+            result = jax.tree.map(lambda x: jnp.reshape(x, (-1,) + x.shape[2:]), result)
             if extra > 0:
-                result = tree_map(lambda x: x[:-extra], result)
+                result = jax.tree.map(lambda x: x[:-extra], result)
         else:
             result = queue(*args, **kwargs)
         return result
 
     _f.__doc__ = f.__doc__
     _f.__annotations__ = f.__annotations__
     return _f
@@ -154,15 +152,15 @@
         extra = 0
     T = N // chunksize
     # arg = jnp.reshape(arg, (chunksize, N // chunksize) + arg.shape[1:])
     return arg
 
 
 def prepad(a, chunksize: int):
-    return tree_map(lambda arg: _pad_extra(arg, chunksize), a)
+    return jax.tree.map(lambda arg: _pad_extra(arg, chunksize), a)
 
 
 T = TypeVar('T')
 
 
 def remove_chunk_dim(py_tree: T) -> T:
     """
@@ -170,15 +168,15 @@
 
     Args:
         py_tree: pytree to remove chunk dimension from
 
     Returns:
         pytree with chunk dimension removed
     """
-    leaves = tree_util.tree_leaves(py_tree)
+    leaves = jax.tree.leaves(py_tree)
 
     # Check consistency
     for leaf in leaves:
         if len(leaf.shape) < 1:
             raise ValueError(f"Expected all leaves to have at least one dimension, got {leaf.shape}")
         if leaf.shape[0] != leaves[0].shape[0]:
             raise ValueError(
@@ -188,15 +186,15 @@
     def _remove_chunk_dim(a):
         shape = list(a.shape)
         if len(shape) == 1:
             return a[0]
         shape = [shape[0] * shape[1]] + shape[2:]
         return jnp.reshape(a, shape)
 
-    return tree_map(_remove_chunk_dim, py_tree)
+    return jax.tree.map(_remove_chunk_dim, py_tree)
 
 
 def add_chunk_dim(py_tree: T, chunk_size: int) -> T:
     """
     Add a chunk dimension to a pytree
 
     Args:
@@ -208,15 +206,15 @@
     """
 
     def _add_chunk_dim(a):
         shape = list(a.shape)
         shape = [chunk_size, shape[0] // chunk_size] + shape[1:]
         return jnp.reshape(a, shape)
 
-    return tree_map(_add_chunk_dim, py_tree)
+    return jax.tree.map(_add_chunk_dim, py_tree)
 
 
 def chunked_vmap(f, chunk_size: Optional[int] = None, unroll: int = 1):
     """
     A version of vmap which chunks the input into smaller pieces to avoid memory issues.
 
     Args:
@@ -244,29 +242,29 @@
 
             _, result = lax.scan(f=body, init=(), xs=(args, kwargs), unroll=unroll)
             return result
 
         if chunk_size > 1:
             # Get from first leaf
             if len(args) > 0:
-                batch_size = tree_util.tree_leaves(args)[0].shape[0]
+                batch_size = jax.tree.leaves(args)[0].shape[0]
             else:
-                batch_size = tree_util.tree_leaves(kwargs)[0].shape[0]
+                batch_size = jax.tree.leaves(kwargs)[0].shape[0]
             remainder = batch_size % chunk_size
             extra = (chunk_size - remainder) % chunk_size
             if extra > 0:
-                (args, kwargs) = tree_map(lambda x: _pad_extra(x, chunk_size), (args, kwargs))
-            (args, kwargs) = tree_map(
+                (args, kwargs) = jax.tree.map(lambda x: _pad_extra(x, chunk_size), (args, kwargs))
+            (args, kwargs) = jax.tree.map(
                 lambda x: jnp.reshape(x, (chunk_size, x.shape[0] // chunk_size) + x.shape[1:]),
                 (args, kwargs)
             )
             result = jax.vmap(queue)(*args, **kwargs)  # [chunksize, batch_size // chunksize, ...]
-            result = tree_map(lambda x: jnp.reshape(x, (-1,) + x.shape[2:]), result)
+            result = jax.tree.map(lambda x: jnp.reshape(x, (-1,) + x.shape[2:]), result)
             if extra > 0:
-                result = tree_map(lambda x: x[:-extra], result)
+                result = jax.tree.map(lambda x: x[:-extra], result)
         else:
             result = queue(*args, **kwargs)
         return result
 
     _f.__doc__ = f.__doc__
     _f.__annotations__ = f.__annotations__
     return _f
```

### Comparing `jaxns-2.4.9/jaxns/internals/random.py` & `jaxns-2.5.0/jaxns/internals/random.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     if special_orthogonal:
         R *= jnp.sign(R)
     Q = Q @ jnp.diag(jnp.sign(jnp.diag(R)))
     return Q
 
 
 def resample_indicies(key: PRNGKey, log_weights: Optional[FloatArray] = None, S: Optional[int] = None,
-                      replace: bool = False, num_total: Optional[int] = None) -> IntArray:
+                      replace: bool = True, num_total: Optional[int] = None) -> IntArray:
     """
     Get resample indicies according to a given weighting, with or without replacement.
 
     Args:
         key: PRNGKey
         log_weights: Optional log weights
         S: Optional number of samples. Computes effective sample size from log weights if not given.
```

### Comparing `jaxns-2.4.9/jaxns/internals/shapes.py` & `jaxns-2.5.0/jaxns/internals/shapes.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.4.9/jaxns/internals/shrinkage_statistics.py` & `jaxns-2.5.0/jaxns/internals/shrinkage_statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Tuple, Optional, NamedTuple
 
 import jax.numpy as jnp
 
-from jaxns.internals.cumulative_ops import cumulative_op_static, cumulative_op_dynamic
+from jaxns.internals.cumulative_ops import cumulative_op_dynamic, scan_associative_cumulative_op, cumulative_op_static
 from jaxns.internals.log_semiring import LogSpace
 from jaxns.internals.tree_structure import SampleTreeGraph, count_crossed_edges
 from jaxns.internals.types import MeasureType, EvidenceCalculation, float_type, IntArray, FloatArray
 
 
 def compute_enclosed_prior_volume(sample_tree: SampleTreeGraph) -> MeasureType:
     """
@@ -24,16 +24,16 @@
         X_mean = LogSpace(log_X)
         # T_mean = LogSpace(jnp.log(num_live_points) - jnp.log(num_live_points + 1.))
         # T_mean = LogSpace(jnp.log(1.) - jnp.log(1. + 1./num_live_points))
         T_mean = LogSpace(- jnp.logaddexp(0., -jnp.log(num_live_points)))
         next_X_mean = X_mean * T_mean
         return next_X_mean.log_abs_val
 
-    _, log_X = cumulative_op_static(op=op, init=jnp.asarray(-jnp.inf, float_type),
-                                    xs=live_point_counts.num_live_points)
+    _, log_X = scan_associative_cumulative_op(op=op, init=jnp.asarray(-jnp.inf, float_type),
+                                              xs=live_point_counts.num_live_points)
     return log_X
 
 
 class EvidenceUpdateVariables(NamedTuple):
     num_live_points: FloatArray
     log_L_next: FloatArray
 
@@ -137,13 +137,14 @@
     init = init_evidence_calc()
     xs = EvidenceUpdateVariables(
         num_live_points=num_live_points.astype(float_type),
         log_L_next=log_L
     )
     if num_samples is not None:
         stop_idx = num_samples
-        final_accumulate, result = cumulative_op_dynamic(op=_update_evidence_calc_op, init=init, xs=xs, stop_idx=stop_idx)
+        final_accumulate, result = cumulative_op_dynamic(op=_update_evidence_calc_op, init=init, xs=xs,
+                                                         stop_idx=stop_idx)
     else:
         final_accumulate, result = cumulative_op_static(op=_update_evidence_calc_op, init=init, xs=xs)
     final_evidence_calculation = final_accumulate
     per_sample_evidence_calculation = result
     return final_evidence_calculation, per_sample_evidence_calculation
```

### Comparing `jaxns-2.4.9/jaxns/internals/stats.py` & `jaxns-2.5.0/jaxns/internals/stats.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.4.9/jaxns/internals/tests/test_log_semiring.py` & `jaxns-2.5.0/jaxns/internals/tests/test_log_semiring.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.4.9/jaxns/internals/tests/test_maps.py` & `jaxns-2.5.0/jaxns/internals/tests/test_maps.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.4.9/jaxns/internals/tests/test_random.py` & `jaxns-2.5.0/jaxns/internals/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.4.9/jaxns/internals/tests/test_shapes.py` & `jaxns-2.5.0/jaxns/internals/tests/test_shapes.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.4.9/jaxns/internals/tests/test_stats.py` & `jaxns-2.5.0/jaxns/internals/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.4.9/jaxns/internals/tests/test_tree_structure.py` & `jaxns-2.5.0/jaxns/internals/tests/test_tree_structure.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,67 +1,74 @@
 from timeit import default_timer
 
 import jax
 import numpy as np
-from jax import tree_map, numpy as jnp, random
+from jax import numpy as jnp, random
 
 from jaxns.internals.tree_structure import SampleTreeGraph, SampleLivePointCounts, count_crossed_edges, \
     count_intervals_naive, \
     plot_tree, count_old, count_crossed_edges_less_fast, concatenate_sample_trees, unbatch_state
 from jaxns.internals.types import StaticStandardNestedSamplerState, StaticStandardSampleCollection
 
 
+def pytree_assert_equal(a, b):
+    print(a)
+    print(b)
+    for x, y in zip(jax.tree.leaves(a), jax.tree.leaves(b)):
+        np.testing.assert_allclose(x, y)
+
+
 def test_naive():
     S = SampleTreeGraph(
         sender_node_idx=jnp.asarray([0, 0, 0, 1, 2, 3]),
         log_L=jnp.asarray([1, 2, 3, 4, 5, 6])
     )
     plot_tree(S)
     expected = SampleLivePointCounts(
         samples_indices=jnp.asarray([0, 1, 2, 3, 4, 5]),
         num_live_points=jnp.asarray([3, 3, 3, 3, 2, 1])
     )
-    assert all(tree_map(lambda x, y: np.array_equal(x, y), count_intervals_naive(S), expected))
-    assert all(tree_map(lambda x, y: np.array_equal(x, y), count_intervals_naive(S), count_old(S)))
+    assert all(jax.tree.map(lambda x, y: np.array_equal(x, y), count_intervals_naive(S), expected))
+    assert all(jax.tree.map(lambda x, y: np.array_equal(x, y), count_intervals_naive(S), count_old(S)))
 
 
 def test_basic():
     S = SampleTreeGraph(
         sender_node_idx=jnp.asarray([0, 0, 0, 1, 2, 3]),
         log_L=jnp.asarray([1, 2, 3, 4, 5, 6])
     )
-    assert all(tree_map(lambda x, y: np.array_equal(x, y), count_crossed_edges(S), count_intervals_naive(S)))
-    assert all(tree_map(lambda x, y: np.array_equal(x, y), count_crossed_edges(S), count_old(S)))
-    assert all(tree_map(lambda x, y: np.array_equal(x, y), count_crossed_edges(S), count_crossed_edges_less_fast(S)))
+    pytree_assert_equal(count_crossed_edges(S), count_intervals_naive(S))
+    pytree_assert_equal(count_crossed_edges(S), count_old(S))
+    pytree_assert_equal(count_crossed_edges(S), count_crossed_edges_less_fast(S))
 
     S = SampleTreeGraph(
         sender_node_idx=jnp.asarray([0, 0, 0, 1, 3, 2]),
         log_L=jnp.asarray([1, 2, 3, 4, 6, 5])
     )
 
-    assert all(tree_map(lambda x, y: np.array_equal(x, y), count_crossed_edges(S), count_intervals_naive(S)))
-    assert all(tree_map(lambda x, y: np.array_equal(x, y), count_crossed_edges(S), count_old(S)))
-    assert all(tree_map(lambda x, y: np.array_equal(x, y), count_crossed_edges(S), count_crossed_edges_less_fast(S)))
+    pytree_assert_equal(count_crossed_edges(S), count_intervals_naive(S))
+    pytree_assert_equal(count_crossed_edges(S), count_old(S))
+    pytree_assert_equal(count_crossed_edges(S), count_crossed_edges_less_fast(S))
 
 
 def test_with_num_samples():
     S1 = SampleTreeGraph(
         sender_node_idx=jnp.asarray([0, 0, 0, 1, 2, 3, 4, 5, 0, 0]),
         log_L=jnp.asarray([1, 2, 3, 4, 5, 6, 7, 8, jnp.inf, jnp.inf])
     )
     num_samples = 8
 
     S2 = SampleTreeGraph(
         sender_node_idx=jnp.asarray([0, 0, 0, 1, 2, 3, 4, 5]),
         log_L=jnp.asarray([1, 2, 3, 4, 5, 6, 7, 8])
     )
 
-    assert all(tree_map(lambda x, y: np.array_equal(x[:num_samples], y),
-                        count_crossed_edges(S1, num_samples),
-                        count_crossed_edges(S2)))
+    x = jax.tree.map(lambda x: x[:num_samples], count_crossed_edges(S1, num_samples))
+
+    pytree_assert_equal(x, count_crossed_edges(S2))
 
     output = count_crossed_edges(S1, num_samples)
     print(output)
     np.testing.assert_array_equal(output.num_live_points[num_samples:], 0)
 
 
 def test_random_tree():
@@ -83,17 +90,17 @@
     S = SampleTreeGraph(
         sender_node_idx=jnp.asarray(parent_idx),
         log_L=jnp.asarray(log_L)[1:]
     )
 
     plot_tree(S)
 
-    assert all(tree_map(lambda x, y: np.array_equal(x, y), count_crossed_edges(S), count_intervals_naive(S)))
-    assert all(tree_map(lambda x, y: np.array_equal(x, y), count_crossed_edges(S), count_old(S)))
-    assert all(tree_map(lambda x, y: np.array_equal(x, y), count_crossed_edges(S), count_crossed_edges_less_fast(S)))
+    pytree_assert_equal(count_crossed_edges(S), count_intervals_naive(S))
+    pytree_assert_equal(count_crossed_edges(S), count_old(S))
+    pytree_assert_equal(count_crossed_edges(S), count_crossed_edges_less_fast(S))
 
     T = count_crossed_edges_less_fast(S)
     import pylab as plt
     plt.plot(S.log_L[T.samples_indices], T.num_live_points)
     plt.show()
 
 
@@ -179,15 +186,15 @@
             U_samples=jnp.asarray([1., 1., 0.])[:, None],
             num_likelihood_evaluations=jnp.asarray([1, 2, 0]),
             phantom=jnp.asarray([True, False, False])
         ),
         front_idx=jnp.asarray([1])
     )
 
-    batched_state = tree_map(lambda x, y: jnp.stack([x, y], axis=0), single_state_1, single_state_2)
+    batched_state = jax.tree.map(lambda x, y: jnp.stack([x, y], axis=0), single_state_1, single_state_2)
 
     unbatched_state = unbatch_state(batched_state)
 
     print(unbatched_state)
 
     # The second element of first batch is not measure so it should be at end of unbatched
     expected_state = StaticStandardNestedSamplerState(
@@ -213,9 +220,9 @@
             num_likelihood_evaluations=jnp.asarray([1, 1, 2, 2, 0, 0]),
             phantom=jnp.asarray([True, True, False, False, False, False])
         ),
         front_idx=jnp.asarray([2, 3])
     )
 
     # compare pytrees
-    for a, b in zip(jax.tree_util.tree_leaves(unbatched_state), jax.tree_util.tree_leaves(expected_state)):
+    for a, b in zip(jax.tree.leaves(unbatched_state), jax.tree.leaves(expected_state)):
         assert jnp.all(a == b)
```

### Comparing `jaxns-2.4.9/jaxns/internals/tests/test_types.py` & `jaxns-2.5.0/jaxns/internals/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.4.9/jaxns/internals/tree_structure.py` & `jaxns-2.5.0/jaxns/internals/tree_structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import NamedTuple, List, Tuple, Union, Optional
 
-from jax import numpy as jnp, lax, tree_map, core
+import jax
+from jax import numpy as jnp, lax, core
 from jax._src.numpy import lax_numpy
 
+from jaxns.internals.cumulative_ops import cumulative_op_dynamic, scan_associative_cumulative_op, cumulative_op_static
 from jaxns.internals.maps import remove_chunk_dim
-from jaxns.internals.cumulative_ops import cumulative_op_static, cumulative_op_dynamic
 from jaxns.internals.types import MeasureType, IntArray, float_type, FloatArray, StaticStandardNestedSamplerState, \
     int_type
 
 
 class SampleTreeGraph(NamedTuple):
     """
     Represents tree structure of samples.
@@ -67,16 +68,14 @@
 
     def op(crossed_edges, last_node):
         # init = 1
         # delta = degree(nodes[last_node]) - 1
         crossed_edges += out_degree[last_node] - 1
         return crossed_edges
 
-
-
     if num_samples is not None:
         _, crossed_edges_sorted = cumulative_op_dynamic(
             op=op,
             init=jnp.asarray(1, out_degree.dtype),
             xs=sort_idx,
             stop_idx=num_samples,
             pre_op=False,
@@ -410,11 +409,11 @@
     )
     unbatched_state = unbatched_state._replace(
         sample_collection=unbatched_state.sample_collection._replace(sender_node_idx=sender_node_idx)
     )
 
     # Rearrange the samples
     unbatched_state = unbatched_state._replace(
-        sample_collection=tree_map(lambda x: x[sort_idx], unbatched_state.sample_collection),
+        sample_collection=jax.tree.map(lambda x: x[sort_idx], unbatched_state.sample_collection),
         front_idx=front_idx
     )
     return unbatched_state
```

### Comparing `jaxns-2.4.9/jaxns/internals/types.py` & `jaxns-2.5.0/jaxns/internals/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import NamedTuple, Optional, Union, Any, Callable, Tuple, Dict, List, TypeVar
 
-import chex
+import jax
 import numpy as np
 from jax import numpy as jnp
 
 __all__ = [
     'EvidenceCalculation',
     'TerminationCondition',
     'StaticStandardNestedSamplerState',
@@ -24,23 +24,23 @@
     'MeasureType'
 ]
 
 float_type = jnp.result_type(float)
 int_type = jnp.result_type(int)
 complex_type = jnp.result_type(complex)
 
-PRNGKey = chex.PRNGKey
-FloatArray = chex.Array
-IntArray = chex.Array
-BoolArray = chex.Array
+PRNGKey = jax.Array
+FloatArray = Union[jax.Array, float]
+IntArray = Union[jax.Array, int]
+BoolArray = Union[jax.Array, bool]
 
 LikelihoodType = Callable[..., FloatArray]
 RandomVariableType = TypeVar('RandomVariableType')
 MeasureType = TypeVar('MeasureType')
-LikelihoodInputType = Tuple[RandomVariableType, ...]  # Likelihood conditional variables
+LikelihoodInputType = Union[Tuple[RandomVariableType, ...], RandomVariableType]  # Likelihood conditional variables
 UType = FloatArray  # Sample space type
 XType = Dict[str, RandomVariableType]  # Prior variable type
 
 
 class EvidenceCalculation(NamedTuple):
     """
     Contains a running estimate of evidence and related quantities.
@@ -69,16 +69,16 @@
         log_L_contour: Terminate if this log(L) contour is reached. A contour is reached if any dead point
             has log(L) > log_L_contour. Uncollected live points are not considered.
         efficiency_threshold: Terminate if the efficiency (num_samples / num_likelihood_evaluations) is less than this,
             for the last shrinkage iteration.
     """
     ess: Optional[FloatArray] = jnp.asarray(jnp.inf, float_type)
     evidence_uncert: Optional[FloatArray] = jnp.asarray(0., float_type)
-    live_evidence_frac: Optional[FloatArray] = None # Depreceated use dlogZ
-    dlogZ: Optional[FloatArray] = jnp.asarray(np.log(1. + 1e-3), float_type) #
+    live_evidence_frac: Optional[FloatArray] = None  # Depreceated use dlogZ
+    dlogZ: Optional[FloatArray] = jnp.asarray(np.log(1. + 1e-3), float_type)  #
     max_samples: Optional[IntArray] = jnp.asarray(jnp.iinfo(int_type).max, int_type)
     max_num_likelihood_evaluations: Optional[IntArray] = jnp.asarray(jnp.iinfo(int_type).max, int_type)
     log_L_contour: Optional[FloatArray] = jnp.asarray(jnp.inf, float_type)
     efficiency_threshold: Optional[FloatArray] = jnp.asarray(0., float_type)
 
     def __and__(self, other):
         return TerminationConditionConjunction(conds=[self, other])
@@ -143,23 +143,25 @@
 class StaticStandardSampleCollection(NamedTuple):
     sender_node_idx: IntArray  # [N] with values in [0, N]
     log_L: MeasureType  # [N] log(L) of each sample
     U_samples: UType  # [N, D] samples in U-space
     num_likelihood_evaluations: IntArray  # [N] number of likelihood evaluations for each sample
     phantom: BoolArray  # [N] whether the sample is a phantom sample
 
+
 class TerminationRegister(NamedTuple):
     num_samples_used: IntArray
     evidence_calc: EvidenceCalculation
     evidence_calc_with_remaining: EvidenceCalculation
     num_likelihood_evaluations: IntArray
     log_L_contour: FloatArray
     efficiency: FloatArray
     plateau: BoolArray
 
+
 class StaticStandardNestedSamplerState(NamedTuple):
     key: PRNGKey
     next_sample_idx: IntArray  # the next sample insert index <==> the number of samples
     sample_collection: StaticStandardSampleCollection
     front_idx: IntArray  # the index of the front of the live points within sample collection
```

### Comparing `jaxns-2.4.9/jaxns/nested_sampler/abc.py` & `jaxns-2.5.0/jaxns/nested_sampler/abc.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.4.9/jaxns/nested_sampler/standard_static.py` & `jaxns-2.5.0/jaxns/nested_sampler/standard_static.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-import logging
+import warnings
 from typing import Tuple, NamedTuple, Any, Union
 
 import jax
-from jax import random, pmap, tree_map, numpy as jnp, lax, core, vmap
+from jax import random, pmap, numpy as jnp, lax, core, vmap
 from jax._src.lax import parallel
 
 from jaxns.framework.bases import BaseAbstractModel
 from jaxns.internals.cumulative_ops import cumulative_op_static
 from jaxns.internals.log_semiring import LogSpace, normalise_log_space
+from jaxns.internals.logging import logger
 from jaxns.internals.shrinkage_statistics import compute_evidence_stats, init_evidence_calc, \
     update_evicence_calculation, EvidenceUpdateVariables, _update_evidence_calc_op
 from jaxns.internals.stats import linear_to_log_stats, effective_sample_size
 from jaxns.internals.tree_structure import SampleTreeGraph, count_crossed_edges, unbatch_state
+from jaxns.internals.types import TerminationCondition
+from jaxns.internals.types import TerminationCondition
 from jaxns.internals.types import TerminationCondition, IntArray, PRNGKey, BoolArray, int_type, UType, MeasureType, \
     float_type, \
     TerminationConditionDisjunction, \
     TerminationConditionConjunction, Sample, StaticStandardSampleCollection, \
     StaticStandardNestedSamplerState, NestedSamplerResults, EvidenceCalculation, TerminationRegister
 from jaxns.nested_sampler.bases import BaseAbstractNestedSampler
 from jaxns.samplers.abc import SamplerState
@@ -23,16 +26,14 @@
 from jaxns.samplers.uniform_samplers import UniformSampler
 
 __all__ = [
     'TerminationCondition',
     'StandardStaticNestedSampler'
 ]
 
-logger = logging.getLogger('jaxns')
-
 
 def _inter_sync_shrinkage_process(
         init_state: StaticStandardNestedSamplerState,
         init_termination_register: TerminationRegister,
         sampler: BaseAbstractSampler,
         num_samples: int) -> Tuple[StaticStandardNestedSamplerState, TerminationRegister]:
     """
@@ -176,28 +177,28 @@
             sample_collection=new_sample_collection
         )
 
         return new_carry, new_return
 
     # Sampler state is created before all this work. Quickly updated during shrinkage.
     init_sampler_state = sampler.pre_process(state=init_state)
-    init_front_sample_collection = tree_map(lambda x: x[init_state.front_idx], init_state.sample_collection)
+    init_front_sample_collection = jax.tree.map(lambda x: x[init_state.front_idx], init_state.sample_collection)
     key, carry_key = random.split(init_state.key)
     init_carry = CarryType(
         sampler_state=init_sampler_state,
         key=carry_key,
         front_idx=init_state.front_idx,
         front_sample_collection=init_front_sample_collection,
         next_sample_idx=init_state.next_sample_idx,
         evidence_calc=init_termination_register.evidence_calc
     )
     out_carry, out_return = lax.scan(body, init_carry, jnp.arange(num_samples), unroll=1)
 
     # Replace the samples in the sample collection with out_return counterparts.
-    sample_collection = tree_map(
+    sample_collection = jax.tree.map(
         lambda x, y: x.at[out_return.replace_idx].set(y),
         init_state.sample_collection,
         out_return.sample_collection
     )
     # Note, discard front_sample_collection since it's already in out_return, and we've replaced the whole front.
 
     # Take front_idx and next_sample_idx from carry, which have been kept up-to-date at every iteration.
@@ -214,17 +215,17 @@
         op=_update_evidence_calc_op,
         init=out_carry.evidence_calc,
         xs=EvidenceUpdateVariables(
             num_live_points=jnp.arange(_n, 0., -1., float_type),
             log_L_next=jnp.sort(out_carry.front_sample_collection.log_L)
         ),
     )
-    num_likelihood_evaluations = init_termination_register.num_likelihood_evaluations + jnp.sum(
-        out_return.sample_collection.num_likelihood_evaluations)
-    efficiency = out_return.sample_collection.log_L.size / num_likelihood_evaluations
+    num_likelihood_evaluations = jnp.asarray(init_termination_register.num_likelihood_evaluations + jnp.sum(
+        out_return.sample_collection.num_likelihood_evaluations), int_type)
+    efficiency = jnp.asarray(out_return.sample_collection.log_L.size / num_likelihood_evaluations, float_type)
     plateau = jnp.all(jnp.equal(out_carry.front_sample_collection.log_L, out_carry.front_sample_collection.log_L[0]))
     termination_register = TerminationRegister(
         num_samples_used=out_carry.next_sample_idx,
         evidence_calc=out_carry.evidence_calc,
         evidence_calc_with_remaining=evidence_calc_with_remaining,
         num_likelihood_evaluations=num_likelihood_evaluations,
         log_L_contour=out_carry.evidence_calc.log_L,
@@ -390,15 +391,15 @@
         for c in term_cond.conds:
             _done, _reason = determine_termination(term_cond=c, termination_register=termination_register)
             done = jnp.bitwise_or(_done, done)
             termination_reason = jnp.bitwise_or(_reason, termination_reason)
         return done, termination_reason
 
     if term_cond.live_evidence_frac is not None:
-        logger.warning("live_evidence_frac is deprecated, use dlogZ instead.")
+        warnings.warn("live_evidence_frac is deprecated, use dlogZ instead.")
 
     if term_cond.max_samples is not None:
         # used all points
         reached_max_samples = termination_register.num_samples_used >= term_cond.max_samples
         done, termination_reason = _set_done_bit(reached_max_samples, 0,
                                                  done=done, termination_reason=termination_reason)
 
@@ -606,15 +607,15 @@
         self.sampler = sampler
         self.num_live_points = int(num_live_points)
         self.num_parallel_workers = int(num_parallel_workers)
         self.verbose = bool(verbose)
         remainder = max_samples % self.num_live_points
         extra = (max_samples - remainder) % self.num_live_points
         if extra > 0:
-            logger.warning(
+            warnings.warn(
                 f"Increasing max_samples ({max_samples}) by {extra} to closest multiple of "
                 f"num_live_points {self.num_live_points}."
             )
         max_samples = int(max_samples + extra)
         if self.num_parallel_workers > 1:
             logger.info(f"Using {self.num_parallel_workers} parallel workers, each running identical samplers.")
         super().__init__(model=model, max_samples=max_samples)
@@ -630,15 +631,15 @@
         num_samples = jnp.minimum(state.next_sample_idx, state.sample_collection.log_L.size)
 
         sample_collection = state.sample_collection
 
         if trim:
             if isinstance(num_samples, core.Tracer):
                 raise RuntimeError("Tracer detected, but expected imperative context.")
-            sample_collection = tree_map(lambda x: x[:num_samples], sample_collection)
+            sample_collection = jax.tree.map(lambda x: x[:num_samples], sample_collection)
 
             sample_tree = SampleTreeGraph(
                 sender_node_idx=sample_collection.sender_node_idx,
                 log_L=sample_collection.log_L
             )
 
             live_point_counts = count_crossed_edges(sample_tree=sample_tree)
```

### Comparing `jaxns-2.4.9/jaxns/plotting.py` & `jaxns-2.5.0/jaxns/plotting.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-import logging
+import warnings
 from typing import Optional, List, Union
 
+import jax
 import jax.numpy as jnp
 import numpy as np
 import pylab as plt
 from jax import random
 from matplotlib.animation import FuncAnimation
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 from scipy.stats import gaussian_kde
 
 from jaxns.internals.log_semiring import cumulative_logsumexp, LogSpace, normalise_log_space
 from jaxns.internals.shapes import tuple_prod
 from jaxns.internals.types import NestedSamplerResults, int_type
 from jaxns.utils import resample
 
-logger = logging.getLogger('jaxns')
-
 __all__ = ['plot_diagnostics',
            'plot_cornerplot']
 
 
 def plot_diagnostics(results: NestedSamplerResults, save_name=None):
     """
     Plot diagnostics of the nested sampling run.
@@ -40,15 +39,23 @@
     log_L = np.asarray(results.log_L_samples)
     max_log_likelihood = np.max(log_L)
     log_dp_mean = np.asarray(results.log_dp_mean)
     log_cum_evidence = cumulative_logsumexp(log_dp_mean)
     cum_evidence = np.exp(log_cum_evidence)
     log_Z_mean = np.asarray(results.log_Z_mean)
     num_likelihood_evaluations_per_sample = np.asarray(results.num_likelihood_evaluations_per_sample)
-    efficiency = 1. / num_likelihood_evaluations_per_sample
+    if np.any(num_likelihood_evaluations_per_sample == 0):
+        warnings.warn("Found samples with zero likelihood evaluations.")
+        efficiency = np.where(
+            num_likelihood_evaluations_per_sample == 0,
+            np.nan,
+            1. / num_likelihood_evaluations_per_sample
+        )
+    else:
+        efficiency = 1. / num_likelihood_evaluations_per_sample
     mean_efficiency = np.exp(results.log_efficiency)
     # Plot the number of live points
     axs[0].plot(-log_X, num_live_points_per_sample, c='black')
     axs[0].set_ylabel(r'$n_{\rm live}$')
     # detect if too small log likelihood
     rel_log_L = log_L - max_log_likelihood
     axs[1].plot(-log_X, np.exp(rel_log_L), c='black')
@@ -76,15 +83,15 @@
     axs[4].set_xlabel(r'$- \log X$')
     if save_name is not None:
         fig.savefig(save_name, bbox_inches='tight', dpi=300, pad_inches=0.0)
     plt.show()
 
 
 def plot_cornerplot(results: NestedSamplerResults, variables: Optional[List[str]] = None,
-                    with_parametrised:bool=False,
+                    with_parametrised: bool = False,
                     save_name: Optional[str] = None, kde_overlay: bool = False):
     """
     Plots a cornerplot of the posterior samples.
 
     Args:
         results: NestedSamplerResult
         variables: list of variable names to plot. Plots all collected samples by default.
@@ -153,15 +160,15 @@
                 continue
             # Plot the marginal distribution
             _samples = leaves[:, row]  # [num_samples]
             _parameter = parameters[row]
             _log_weights = log_weights
             is_finite = np.isfinite(_samples)
             if np.bitwise_not(np.all(is_finite)):
-                logger.warning(f"Found {np.sum(np.bitwise_not(is_finite))} non-finite samples for {_parameter}")
+                warnings.warn(f"Found {np.sum(np.bitwise_not(is_finite))} non-finite samples for {_parameter}")
                 _samples = _samples[is_finite]
                 _log_weights = _log_weights[is_finite]
             _weights = np.exp(_log_weights)
             # Percentiles
             per_1, per_5, per_50, per_95, per_99 = weighted_percentile(_samples, _log_weights,
                                                                        [1, 5, 50, 95, 99])
             # Plot the histogram, from 1_per to 99_per
@@ -196,15 +203,15 @@
                 continue
 
             # Get the samples for the 2D histogram
             _samples = leaves[:, [row, col]]  # [num_samples, 2]
             _log_weights = log_weights
             is_finite = np.all(np.isfinite(_samples), axis=-1)  # [num_samples]
             if np.bitwise_not(np.all(is_finite)):
-                logger.warning(
+                warnings.warn(
                     f"Found {np.sum(np.bitwise_not(is_finite))} non-finite samples for {parameters[row]} and {parameters[col]}")
                 _samples = _samples[is_finite]
                 _log_weights = _log_weights[is_finite]
             _weights = np.exp(_log_weights)
 
             # Plot the 2D histogram, over ranges set by the 1_per and 99_per of each parameter
             ranges = [param_limits[parameters[col]], param_limits[parameters[row]]]
@@ -432,18 +439,17 @@
         ax.figure.colorbar(sm, cax=cax, orientation='vertical', label=label)
 
 
 def corner_cornerplot(results: NestedSamplerResults):
     try:
         import corner
     except ImportError:
-        logger.warning("You must run `pip install corner`")
+        warnings.warn("You must run `pip install corner`")
         exit(0)
     try:
         import arviz as az
     except ImportError:
-        logger.warning("You must run `pip install arviz`")
+        warnings.warn("You must run `pip install arviz`")
         exit(0)
-    from jax import tree_map
     samples = resample(random.PRNGKey(42), results.samples, results.log_dp_mean, S=int(results.ESS))
-    corner.corner(az.from_dict(posterior=tree_map(lambda x: x[None], samples)), )
+    corner.corner(az.from_dict(posterior=jax.tree.map(lambda x: x[None], samples)), )
     plt.show()
```

### Comparing `jaxns-2.4.9/jaxns/public.py` & `jaxns-2.5.0/jaxns/public.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import logging
+import warnings
 from typing import Optional, Tuple, Union
 
+import jax
 import jax.numpy as jnp
 import tensorflow_probability.substrates.jax as tfp
-from jax import tree_map, core
+from jax import core
 
 from jaxns.framework.bases import BaseAbstractModel
+from jaxns.internals.logging import logger
 from jaxns.internals.types import PRNGKey, IntArray, StaticStandardNestedSamplerState, TerminationCondition, \
     NestedSamplerResults
 from jaxns.nested_sampler.bases import BaseAbstractNestedSampler
 from jaxns.nested_sampler.standard_static import StandardStaticNestedSampler
 from jaxns.plotting import plot_cornerplot, plot_diagnostics
 from jaxns.samplers.uni_slice_sampler import UniDimSliceSampler
 from jaxns.utils import summary, save_results, load_results
 
 tfpd = tfp.distributions
 
-logger = logging.getLogger('jaxns')
-
 __all__ = [
     'DefaultNestedSampler',
     'ApproximateNestedSampler',
     'ExactNestedSampler',
     'TerminationCondition'
 ]
 
@@ -82,15 +82,15 @@
                 self._c = 50 * model.U_ndims if c is None else int(c)
             else:
                 self._c = 30 * model.U_ndims if c is None else int(c)
         if self._c <= 0:
             raise ValueError(f"Expected c > 0, got c={self._c}")
         # Sanity check for max_samples (should be able to at least do one shrinkage)
         if max_samples < self._c * (self._k + 1):
-            logger.warning(f"max_samples={max_samples} is likely too small!")
+            warnings.warn(f"max_samples={max_samples} is likely too small!")
         self._nested_sampler = StandardStaticNestedSampler(
             model=model,
             num_live_points=self._c,
             max_samples=max_samples,
             sampler=UniDimSliceSampler(
                 model=model,
                 num_slices=model.U_ndims * self._s,
@@ -180,21 +180,21 @@
             raise RuntimeError("Tracer detected, but expected imperative context.")
 
         def trim(x):
             if x.size > 1:
                 return x[:results.total_num_samples]
             return x
 
-        results = tree_map(trim, results)
+        results = jax.tree.map(trim, results)
         return results
 
 
 class ApproximateNestedSampler(DefaultNestedSampler):
     def __init__(self, *args, **kwargs):
-        logger.warning(f"ApproximateNestedSampler is deprecated. Use DefaultNestedSampler instead.")
+        warnings.warn(f"ApproximateNestedSampler is deprecated. Use DefaultNestedSampler instead.")
         super().__init__(*args, **kwargs)
 
 
 class ExactNestedSampler(ApproximateNestedSampler):
     def __init__(self, *args, **kwargs):
-        logger.warning(f"ExactNestedSampler is deprecated. Use DefaultNestedSampler instead.")
+        warnings.warn(f"ExactNestedSampler is deprecated. Use DefaultNestedSampler instead.")
         super().__init__(*args, **kwargs)
```

### Comparing `jaxns-2.4.9/jaxns/samplers/abc.py` & `jaxns-2.5.0/jaxns/samplers/abc.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.4.9/jaxns/samplers/bases.py` & `jaxns-2.5.0/jaxns/samplers/bases.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.4.9/jaxns/samplers/multi_ellipsoid/multi_ellipsoid_utils.py` & `jaxns-2.5.0/jaxns/samplers/multi_ellipsoid/multi_ellipsoid_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from typing import NamedTuple, Tuple, Literal
 
+import jax
 import numpy as np
 import pylab as plt
-from jax import numpy as jnp, vmap, random, tree_map, lax
+from jax import numpy as jnp, vmap, random, lax
 from jax._src.scipy.special import gammaln
 
 from jaxns.internals.log_semiring import LogSpace
-from jaxns.samplers.multi_ellipsoid.em_gmm import em_gmm
 from jaxns.internals.types import IntArray, FloatArray, PRNGKey, BoolArray
 from jaxns.internals.types import UType, int_type, float_type
+from jaxns.samplers.multi_ellipsoid.em_gmm import em_gmm
 
 __all__ = [
     'ellipsoid_clustering',
     'sample_multi_ellipsoid',
     'MultEllipsoidState',
 ]
 
@@ -660,15 +661,15 @@
     # state is zeros except first ellipsoid
     cluster_id = jnp.zeros(N, dtype=int_type)
     params = EllipsoidParams(
         mu=jnp.zeros((K, D), float_type),
         radii=jnp.zeros((K, D), float_type),
         rotation=jnp.zeros((K, D, D), float_type)
     )
-    params: EllipsoidParams = tree_map(lambda x, y: x.at[0].set(y), params, init_ellipsoid)
+    params: EllipsoidParams = jax.tree.map(lambda x, y: x.at[0].set(y), params, init_ellipsoid)
     state = MultEllipsoidState(
         cluster_id=cluster_id,
         params=params
     )
 
     # Initial tracking parameters
     log_VS_subclusters = jnp.asarray([log_VS] + [-jnp.inf] * (K - 1))
@@ -692,33 +693,34 @@
             jnp.where(body_state.done_splitting, jnp.iinfo(body_state.split_depth.dtype).max, body_state.split_depth)
         )
         mask = body_state.state.cluster_id == select_split
         # estimated volume in sub-cluster
         log_VS = body_state.log_VS_subclusters[select_split]
 
         # params of ellipsoid
-        params = tree_map(lambda x: x[select_split], body_state.state.params)
+        params = jax.tree.map(lambda x: x[select_split], body_state.state.params)
 
         # Perform a split on points in the given mask
         # Strategy: if no split we replace child0 with parent and child1 gets zero-size ellipsoid that has no members.
         cluster_split_result: ClusterSplitResult = cluster_split(
             key=split_key,
             params=params,
             points=points,
             mask=mask,
             log_VS=log_VS,
             method=method
         )
 
         # Update the parameters in given component that is being split with child 0
-        params = tree_map(lambda x, y: jnp.where(cluster_split_result.successful_split, x.at[select_split].set(y), x),
-                          body_state.state.params,
-                          cluster_split_result.params0)
+        params = jax.tree.map(
+            lambda x, y: jnp.where(cluster_split_result.successful_split, x.at[select_split].set(y), x),
+            body_state.state.params,
+            cluster_split_result.params0)
         # Update the parameters in `next_k` with child 1
-        params = tree_map(
+        params = jax.tree.map(
             lambda x, y: jnp.where(cluster_split_result.successful_split, x.at[body_state.next_k].set(y), x),
             params,
             cluster_split_result.params1)
         # select_split stays the same cluster_id taking on child 0, but next_k gets child 1
         cluster_id = jnp.where(
             cluster_split_result.successful_split & (cluster_split_result.unsorted_cluster_id == 1) & mask,
             body_state.next_k,
```

### Comparing `jaxns-2.4.9/jaxns/samplers/multi_ellipsoid/tests/test_em_gmm.py` & `jaxns-2.5.0/jaxns/samplers/multi_ellipsoid/tests/test_em_gmm.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.4.9/jaxns/samplers/multi_ellipsoid/tests/test_multi_ellipsoid.py` & `jaxns-2.5.0/jaxns/samplers/multi_ellipsoid/tests/test_multi_ellipsoid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
+import jax
 import numpy as np
 import pylab as plt
 import tensorflow_probability.substrates.jax as tfp
-from jax import numpy as jnp, random, tree_map, disable_jit, vmap
+from jax import numpy as jnp, random, disable_jit, vmap
 
-import jaxns.internals.maps
 from jaxns.framework.bases import PriorModelGen
 from jaxns.framework.model import Model
 from jaxns.framework.prior import Prior
-from jaxns.nested_sampler.standard_static import draw_uniform_samples
 from jaxns.internals.random import random_ortho_matrix
+from jaxns.internals.types import float_type, Sample
+from jaxns.nested_sampler.standard_static import draw_uniform_samples
 from jaxns.samplers.multi_ellipsoid.multi_ellipsoid_utils import log_ellipsoid_volume, ellipsoid_clustering, \
     bounding_ellipsoid, covariance_to_rotational, ellipsoid_params, point_in_ellipsoid, plot_ellipses, \
     EllipsoidParams, maha_ellipsoid, circle_to_ellipsoid, ellipsoid_to_circle
-from jaxns.internals.types import float_type, Sample
 
 tfpd = tfp.distributions
 
 
 def test_ellipsoid_clustering():
     def prior_model() -> PriorModelGen:
         x = yield Prior(tfpd.Uniform(low=0, high=2))
@@ -32,15 +32,15 @@
                   log_likelihood=log_likelihood)
 
     n = 1000
     live_points = draw_uniform_samples(random.PRNGKey(43),
                                        num_live_points=n,
                                        model=model)
     keep = live_points.log_L > log_likelihood(1.1, 1.1)
-    reservoir: Sample = tree_map(lambda x: x[keep], live_points)
+    reservoir: Sample = jax.tree.map(lambda x: x[keep], live_points)
     plt.scatter(reservoir.U_sample[:, 0], reservoir.U_sample[:, 1])
     with disable_jit():
         state = ellipsoid_clustering(random.PRNGKey(42), points=reservoir.U_sample,
                                      log_VS=jnp.asarray(0., float_type),
                                      max_num_ellipsoids=10)
         plot_ellipses(params=state.params)
     # plt.show()
@@ -96,15 +96,15 @@
                                    mean=jnp.zeros(N),
                                    cov=cov,
                                    shape=(n,))
 
     mu, radii, rotation = ellipsoid_params(points=X, mask=jnp.ones(n, jnp.bool_))
     inside = vmap(lambda x: point_in_ellipsoid(x, mu, radii, rotation))(X)
     plt.scatter(X[:, 0], X[:, 1], c=inside)
-    plot_ellipses(tree_map(lambda x: x[None], EllipsoidParams(mu, radii, rotation)))
+    plot_ellipses(jax.tree.map(lambda x: x[None], EllipsoidParams(mu, radii, rotation)))
 
     assert np.all(inside)
 
     rho_max = jnp.max(vmap(lambda x: maha_ellipsoid(x, mu, radii, rotation))(X))
     assert jnp.isclose(rho_max, 1.)
 
     points = jnp.asarray([[0., 1.], [0., -1.], [1.5, 0.], [-1.5, 0.]])
```

### Comparing `jaxns-2.4.9/jaxns/samplers/multi_ellipsoidal_samplers.py` & `jaxns-2.5.0/jaxns/samplers/multi_ellipsoidal_samplers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import NamedTuple, Tuple
 
-from jax import random, numpy as jnp, lax, tree_map
+import jax
+from jax import random, numpy as jnp, lax
 
 from jaxns.internals.shrinkage_statistics import compute_evidence_stats
 from jaxns.internals.tree_structure import SampleTreeGraph, count_crossed_edges
 from jaxns.internals.types import IntArray, StaticStandardNestedSamplerState, UType, StaticStandardSampleCollection
 from jaxns.internals.types import PRNGKey, FloatArray
 from jaxns.internals.types import Sample, int_type
 from jaxns.samplers.abc import SamplerState
@@ -55,15 +56,16 @@
             key=sampler_key,
             points=points,
             log_VS=final_evidence_stats.log_X_mean,
             max_num_ellipsoids=self.max_num_ellipsoids,
             method='em_gmm'
         )
 
-    def post_process(self, sample_collection: StaticStandardSampleCollection, sampler_state: SamplerState) -> SamplerState:
+    def post_process(self, sample_collection: StaticStandardSampleCollection,
+                     sampler_state: SamplerState) -> SamplerState:
         return sampler_state
 
     @property
     def max_num_ellipsoids(self):
         return 2 ** self._depth
 
     def get_sample(self, key: PRNGKey, log_L_constraint: FloatArray,
@@ -118,9 +120,9 @@
         sample = Sample(
             U_sample=final_carry.U,
             log_L_constraint=log_L_constraint,
             log_L=final_carry.log_L,
             num_likelihood_evaluations=final_carry.num_likelihood_evals
         )
 
-        phantom_samples = tree_map(lambda x: jnp.zeros((0,) + x.shape, x.dtype), sample)
+        phantom_samples = jax.tree.map(lambda x: jnp.zeros((0,) + x.shape, x.dtype), sample)
         return sample, phantom_samples
```

### Comparing `jaxns-2.4.9/jaxns/samplers/multi_slice_sampler.py` & `jaxns-2.5.0/jaxns/samplers/multi_slice_sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-import logging
 from typing import TypeVar, NamedTuple, Tuple, Optional
 
-from jax import numpy as jnp, random, tree_map, lax
+import jax
+from jax import numpy as jnp, random, lax
 
 from jaxns.framework.bases import BaseAbstractModel
 from jaxns.internals.cumulative_ops import cumulative_op_static
 from jaxns.internals.types import PRNGKey, FloatArray, BoolArray, Sample, int_type, StaticStandardNestedSamplerState, \
     UType, \
     IntArray, float_type, StaticStandardSampleCollection
 from jaxns.samplers.abc import SamplerState
 from jaxns.samplers.bases import SeedPoint, BaseAbstractMarkovSampler
 
 __all__ = [
     'MultiDimSliceSampler'
 ]
 
-logger = logging.getLogger('jaxns')
-
 T = TypeVar('T')
 
 
 def _slice_bounds(key: PRNGKey, point_U0: FloatArray, num_restrict_dims: int) -> Tuple[FloatArray, FloatArray]:
     """
     Get the slice bounds, randomly selecting which dimensions to slice in.
 
@@ -194,15 +192,15 @@
                 raise ValueError(f"Expected num_restriction dim in (1, {model.U_ndims}], got {num_restrict_dims}.")
         self.num_restrict_dims = int(num_restrict_dims)
 
     def num_phantom(self) -> int:
         return self.num_phantom_save
 
     def pre_process(self, state: StaticStandardNestedSamplerState) -> SamplerState:
-        sample_collection = tree_map(lambda x: x[state.front_idx], state.sample_collection)
+        sample_collection = jax.tree.map(lambda x: x[state.front_idx], state.sample_collection)
         return (sample_collection,)
 
     def post_process(self, sample_collection: StaticStandardSampleCollection,
                      sampler_state: SamplerState) -> SamplerState:
         return (sample_collection,)
 
     def get_seed_point(self, key: PRNGKey, sampler_state: SamplerState,
@@ -256,16 +254,15 @@
             log_L_constraint=log_L_constraint,
             log_L=seed_point.log_L0,
             num_likelihood_evaluations=jnp.asarray(0, int_type)
         )
         final_sample, cumulative_samples = cumulative_op_static(
             op=propose_op,
             init=init_sample,
-            xs=random.split(key, self.num_slices),
-            unroll=2
+            xs=random.split(key, self.num_slices)
         )
 
         # Last sample is the final sample, the rest are potential phantom samples
         # Take only the last num_phantom_save phantom samples
-        phantom_samples: Sample = tree_map(lambda x: x[-(self.num_phantom_save + 1):-1], cumulative_samples)
+        phantom_samples: Sample = jax.tree.map(lambda x: x[-(self.num_phantom_save + 1):-1], cumulative_samples)
 
         return final_sample, phantom_samples
```

### Comparing `jaxns-2.4.9/jaxns/samplers/uni_slice_sampler.py` & `jaxns-2.5.0/jaxns/samplers/uni_slice_sampler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,24 @@
-import logging
 from typing import TypeVar, NamedTuple, Tuple
 
 import jax
-from jax import numpy as jnp, random, lax, tree_map
+from jax import numpy as jnp, random, lax
 
 from jaxns.framework.bases import BaseAbstractModel
 from jaxns.internals.cumulative_ops import cumulative_op_static
 from jaxns.internals.types import PRNGKey, FloatArray, BoolArray, Sample, float_type, int_type, \
     StaticStandardNestedSamplerState, \
     IntArray, UType, StaticStandardSampleCollection
 from jaxns.samplers.abc import SamplerState
 from jaxns.samplers.bases import SeedPoint, BaseAbstractMarkovSampler
 
 __all__ = [
     'UniDimSliceSampler'
 ]
 
-logger = logging.getLogger('jaxns')
-
 T = TypeVar('T')
 
 
 def _sample_direction(n_key: PRNGKey, ndim: int) -> FloatArray:
     """
     Choose a direction randomly from S^(D-1).
 
@@ -82,47 +79,31 @@
     point_U = point_U0 + t * direction
     # close_to_zero = (left >= -10*jnp.finfo(left.dtype).eps) & (right <= 10*jnp.finfo(right.dtype).eps)
     # point_U = jnp.where(close_to_zero, point_U0, point_U)
     # t = jnp.where(close_to_zero, jnp.zeros_like(t), t)
     return point_U, t
 
 
-def _shrink_interval(key: PRNGKey, t: FloatArray, left: FloatArray, right: FloatArray, log_L_proposal: FloatArray,
-                     log_L_constraint: FloatArray, log_L0: FloatArray,
+def _shrink_interval(key: PRNGKey, t: FloatArray, left: FloatArray, right: FloatArray,
                      midpoint_shrink: bool) -> Tuple[FloatArray, FloatArray]:
     """
     Not successful proposal, so shrink, optionally apply exponential shrinkage.
     """
     # witout exponential shrinkage, we shrink to failed proposal point, which is 100% correct.
     left = jnp.where(t < 0., t, left)
     right = jnp.where(t > 0., t, right)
-    key, t_key, midpoint_key = random.split(key, 3)
 
     if midpoint_shrink:
-        # we take two points along lines from origin:
-        #  - alpha: one from a satisfying point (t=0) to non-satisfying proposal,
-        #  - beta: and, one from non-satisfying proposal to the constraint.
-        # We shrink to alpha point if beta point is above alpha point.
-        # Intuitively, the tangent from constraint is more accurate than proposal and should be a supremum of heights
-        # in reasonable cases.
-        # An extension is to make alpha shrink to constraint line, which would shrink very fast, but introduce
-        # auto-correlation which must be later refined away.
-        # Line logic:
-        # logL(t) = m * t + b
-        # logL(0) = b
-        # (logL(t_R) - logL(0))/t_R
-        # logL(t_R*alpha) = (logL(t_R) - logL(0))*alpha + logL(0)
-        alpha_key, beta_key = random.split(midpoint_key, 2)
-        alpha = random.uniform(alpha_key)
-        beta = random.uniform(beta_key)
-        logL_alpha = log_L0 + alpha * (log_L_proposal - log_L0)
-        logL_beta = log_L_proposal + beta * (log_L_constraint - log_L_proposal)
-        do_mid_point_shrink = logL_alpha < logL_beta
-        left = jnp.where((t < 0.) & do_mid_point_shrink, alpha * left, left)
-        right = jnp.where((t > 0.) & do_mid_point_shrink, alpha * right, right)
+        # For this to be correct it must be invariant to monotonic rescaling of the likelihood.
+        # Therefore, it must only use the knowledge of ordering of the likelihoods.
+        # Basic version: shrink to midpoint of interval, i.e. alpha = 0.5.
+        # Extended version: shrink to random point in interval.
+        alpha = random.uniform(key)
+        left = jnp.where((t < 0.), alpha * left, left)
+        right = jnp.where((t > 0.), alpha * right, right)
     return left, right
 
 
 def _new_proposal(key: PRNGKey, seed_point: SeedPoint, midpoint_shrink: bool, perfect: bool,
                   gradient_slice: bool,
                   log_L_constraint: FloatArray,
                   model: BaseAbstractModel) -> Tuple[FloatArray, FloatArray, IntArray]:
@@ -165,17 +146,14 @@
     def body(carry: Carry) -> Carry:
         key, t_key, shrink_key = random.split(carry.key, 3)
         left, right = _shrink_interval(
             key=shrink_key,
             t=carry.t,
             left=carry.left,
             right=carry.right,
-            log_L_proposal=carry.log_L,
-            log_L_constraint=log_L_constraint,
-            log_L0=seed_point.log_L0,
             midpoint_shrink=midpoint_shrink
         )
         point_U, t = _pick_point_in_interval(
             key=t_key,
             point_U0=seed_point.U0,
             direction=carry.direction,
             left=left,
@@ -246,54 +224,58 @@
         init_val=init_carry
     )
     return carry.point_U, carry.log_L, carry.num_likelihood_evaluations
 
 
 class UniDimSliceSampler(BaseAbstractMarkovSampler):
     """
-    Slice sampler for a single dimension. Produces correlated (non-i.i.d.) samples.
+    Slice sampler for a single dimension. Produces correlated samples.
     """
 
     def __init__(self, model: BaseAbstractModel, num_slices: int, num_phantom_save: int, midpoint_shrink: bool,
-                 perfect: bool, gradient_slice: bool = False):
+                 perfect: bool, gradient_slice: bool = False, adaptive_shrink: bool = False):
         """
         Unidimensional slice sampler.
 
         Args:
             model: AbstractModel
             num_slices: number of slices between acceptance. Note: some other software use units of prior dimension.
             midpoint_shrink: if true then contract to the midpoint of interval on rejection. Otherwise, contract to
                 rejection point. Speeds up convergence, but introduces minor auto-correlation.
             num_phantom_save: number of phantom samples to save. Phantom samples are samples that meeting the constraint
                 but are not accepted. They can be used for numerous things, e.g. to estimate the evidence uncertainty.
             perfect: if true then perform exponential shrinkage from maximal bounds, requiring no step-out procedure.
                 Otherwise, uses a doubling procedure (exponentially finding bracket).
                 Note: Perfect is a misnomer, as perfection also depends on the number of slices between acceptance.
-            gradient_slice: if true then always slice along gradient direction.
+            gradient_slice: if true then always slice along increasing gradient direction.
+            adaptive_shrink: if true then shrink interval to random point in interval, rather than midpoint.
         """
         super().__init__(model=model)
         if num_slices < 1:
             raise ValueError(f"num_slices should be >= 1, got {num_slices}.")
         if num_phantom_save < 0:
             raise ValueError(f"num_phantom_save should be >= 0, got {num_phantom_save}.")
         if num_phantom_save >= num_slices:
             raise ValueError(f"num_phantom_save should be < num_slices, got {num_phantom_save} >= {num_slices}.")
         self.num_slices = int(num_slices)
         self.num_phantom_save = int(num_phantom_save)
         self.midpoint_shrink = bool(midpoint_shrink)
         self.perfect = bool(perfect)
         self.gradient_slice = bool(gradient_slice)
+        self.adaptive_shrink = bool(adaptive_shrink)
+        if self.adaptive_shrink:
+            raise NotImplementedError("Adaptive shrinkage not implemented.")
         if not self.perfect:
             raise ValueError("Only perfect slice sampler is implemented.")
 
     def num_phantom(self) -> int:
         return self.num_phantom_save
 
     def pre_process(self, state: StaticStandardNestedSamplerState) -> SamplerState:
-        sample_collection = tree_map(lambda x: x[state.front_idx], state.sample_collection)
+        sample_collection = jax.tree.map(lambda x: x[state.front_idx], state.sample_collection)
         if self.perfect:  # nothing needed
             return (sample_collection,)
         else:  # TODO: step out with doubling, using ellipsoidal clustering
             return (sample_collection,)  # multi_ellipsoidal_params()
 
     def post_process(self, sample_collection: StaticStandardSampleCollection,
                      sampler_state: SamplerState) -> SamplerState:
@@ -355,21 +337,20 @@
             log_L_constraint=log_L_constraint,
             log_L=seed_point.log_L0,
             num_likelihood_evaluations=jnp.asarray(0, int_type)
         )
         final_sample, cumulative_samples = cumulative_op_static(
             op=propose_op,
             init=init_sample,
-            xs=random.split(key, self.num_slices),
-            unroll=2
+            xs=random.split(key, self.num_slices)
         )
 
         # Last sample is the final sample, the rest are potential phantom samples
         # Take only the last num_phantom_save phantom samples
-        phantom_samples: Sample = tree_map(lambda x: x[-(self.num_phantom_save + 1):-1], cumulative_samples)
+        phantom_samples: Sample = jax.tree.map(lambda x: x[-(self.num_phantom_save + 1):-1], cumulative_samples)
 
         # Due to the cumulative nature of the sampler, the final number of likelihood evaluations should be divided
         # equally among the accepted sample and retained phantom samples.
         num_likelihood_evaluations_per_phantom_sample = (
                 final_sample.num_likelihood_evaluations / (self.num_phantom_save + 1)
         ).astype(int_type)
         num_likelihood_evaluations_per_accepted_sample = (
```

### Comparing `jaxns-2.4.9/jaxns/samplers/uniform_samplers.py` & `jaxns-2.5.0/jaxns/samplers/uniform_samplers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import NamedTuple, Tuple
 
-from jax import random, numpy as jnp, lax, tree_map
+import jax
+from jax import random, numpy as jnp, lax
 
 from jaxns.framework.bases import BaseAbstractModel
 from jaxns.internals.types import IntArray, StaticStandardNestedSamplerState, UType, MeasureType, \
     StaticStandardSampleCollection
 from jaxns.internals.types import PRNGKey, FloatArray
 from jaxns.internals.types import Sample, int_type
 from jaxns.samplers.abc import SamplerState
@@ -82,9 +83,9 @@
 
         sample = Sample(
             U_sample=carry_state.U,
             log_L_constraint=log_L_constraint,
             log_L=carry_state.log_L,
             num_likelihood_evaluations=carry_state.num_likelihood_evals
         )
-        phantom_samples = tree_map(lambda x: jnp.zeros((0,) + x.shape, x.dtype), sample)
+        phantom_samples = jax.tree.map(lambda x: jnp.zeros((0,) + x.shape, x.dtype), sample)
         return sample, phantom_samples
```

### Comparing `jaxns-2.4.9/jaxns/tests/conftest.py` & `jaxns-2.5.0/jaxns/tests/conftest.py`

 * *Files 9% similar despite different names*

```diff
@@ -63,14 +63,51 @@
     ns.plot_diagnostics(results)
     ns.summary(results)
     # exact_ns.plot_cornerplot(results)
     return log_Z_true, results
 
 
 @pytest.fixture(scope='package')
+def basic_model_with_obj():
+    class Obj:
+        def __init__(self, x):
+            self.x = x
+
+    def prior_model() -> PriorModelGen:
+        x = yield Prior(tfpd.Uniform(low=0, high=1), name='x')
+        return Obj(x)
+
+    def log_likelihood(obj: Obj):
+        return - jnp.sum(obj.x ** 2)
+
+    model = Model(prior_model=prior_model,
+                  log_likelihood=log_likelihood)
+
+    log_Z_true = bruteforce_evidence(model=model, S=200)
+    return model, log_Z_true
+
+
+@pytest.fixture(scope='package')
+def basic_with_obj_run_results(basic_model_with_obj):
+    model, log_Z_true = basic_model_with_obj
+
+    ns = DefaultNestedSampler(model=model, max_samples=1000, verbose=True)
+    ns_jit = jax.jit(lambda key: ns(key))
+    ns_compiled = ns_jit.lower(random.PRNGKey(42)).compile()
+    with Timer():
+        termination_reason, state = ns_compiled(random.PRNGKey(42))
+        termination_reason.block_until_ready()
+    results = ns.to_results(termination_reason=termination_reason, state=state)
+    ns.plot_diagnostics(results)
+    ns.summary(results)
+    # exact_ns.plot_cornerplot(results)
+    return log_Z_true, results
+
+
+@pytest.fixture(scope='package')
 def basic2_model():
     n = 2
 
     # Prior is uniform in U[0,1]
     # Likelihood is 1 - x**n
     # Z = 1 - 1/n+1
 
@@ -280,25 +317,27 @@
     # plot_cornerplot(results)
 
     return log_Z_true, results
 
 
 @pytest.fixture(scope='package')
 def all_run_results(
-        basic_run_results,
-        basic2_run_results,
-        basic3_run_results,
-        plateau_run_results,
-        basic_mvn_run_results,
-        basic_mvn_run_results_parallel,
-        multiellipsoidal_mvn_run_results
+        # basic_run_results,
+        basic_with_obj_run_results,
+        # basic2_run_results,
+        # basic3_run_results,
+        # plateau_run_results,
+        # basic_mvn_run_results,
+        # basic_mvn_run_results_parallel,
+        # multiellipsoidal_mvn_run_results
 ):
     # Return tuples with names
     return [
-        ('basic', basic_run_results),
-        ('basic2', basic2_run_results),
-        ('basic3', basic3_run_results),
-        ('plateau', plateau_run_results),
-        ('basic_mvn', basic_mvn_run_results),
-        ('basic_mvn_parallel', basic_mvn_run_results_parallel),
-        ('multiellipsoidal_mvn', multiellipsoidal_mvn_run_results)
+        # ('basic', basic_run_results),
+        ('basic_with_obj', basic_with_obj_run_results),
+        # ('basic2', basic2_run_results),
+        # ('basic3', basic3_run_results),
+        # ('plateau', plateau_run_results),
+        # ('basic_mvn', basic_mvn_run_results),
+        # ('basic_mvn_parallel', basic_mvn_run_results_parallel),
+        # ('multiellipsoidal_mvn', multiellipsoidal_mvn_run_results)
     ]
```

### Comparing `jaxns-2.4.9/jaxns/tests/test_nested_sampler.py` & `jaxns-2.5.0/jaxns/tests/test_nested_sampler.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.4.9/jaxns/tests/test_utils.py` & `jaxns-2.5.0/jaxns/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.4.9/jaxns/utils.py` & `jaxns-2.5.0/jaxns/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import io
-import logging
+import json
+import warnings
 from typing import NamedTuple, TextIO, Union, Optional, Tuple, TypeVar, Callable
 
+import jax
 import numpy as np
-from jax import numpy as jnp, tree_map, vmap, random, jit, lax
+from jax import numpy as jnp, vmap, random, jit, lax
 
 from jaxns.framework.bases import BaseAbstractModel
 from jaxns.internals.cumulative_ops import cumulative_op_static
 from jaxns.internals.log_semiring import LogSpace
 from jaxns.internals.maps import prepare_func_args
+from jaxns.internals.namedtuple_utils import serialise_namedtuple, deserialise_namedtuple
 from jaxns.internals.random import resample_indicies
 from jaxns.internals.types import NestedSamplerResults, float_type, XType, UType, FloatArray, IntArray, \
     isinstance_namedtuple
 from jaxns.internals.types import PRNGKey
 from jaxns.warnings import deprecated
 
-logger = logging.getLogger('jaxns')
-
 __all__ = [
     'resample',
     'marginalise_static_from_U',
     'marginalise_dynamic_from_U',
     'marginalise_static',
     'marginalise_dynamic',
     'maximum_a_posteriori_point',
@@ -34,30 +35,30 @@
     'save_results',
     'load_pytree',
     'load_results'
 ]
 
 
 def resample(key: PRNGKey, samples: Union[XType, UType], log_weights: jnp.ndarray, S: int = None,
-             replace: bool = False) -> XType:
+             replace: bool = True) -> XType:
     """
     Resample the weighted samples into uniformly weighted samples.
 
     Args:
         key: PRNGKey
         samples: samples from nested sampled results
         log_weights: log-posterior weight
         S: number of samples to generate. Will use Kish's estimate of ESS if None.
         replace: whether to sample with replacement
 
     Returns:
         equally weighted samples
     """
     idx = resample_indicies(key, log_weights, S=S, replace=replace)
-    return tree_map(lambda s: s[idx, ...], samples)
+    return jax.tree.map(lambda s: s[idx, ...], samples)
 
 
 _V = TypeVar('_V')
 
 
 def evaluate_map_estimate_from_U(results: NestedSamplerResults, model: BaseAbstractModel, fun: Callable[..., _V]) -> _V:
     """
@@ -94,15 +95,15 @@
     """
     U_samples = resample(key, U_samples, log_weights, S=ESS, replace=True)
 
     def _eval(U):
         V = model.prepare_input(U=U)
         return fun(*V)
 
-    marginalised = tree_map(lambda marg: jnp.nanmean(marg, axis=0), vmap(_eval)(U_samples))
+    marginalised = jax.tree.map(lambda marg: jnp.nanmean(marg, axis=0), vmap(_eval)(U_samples))
     return marginalised
 
 
 def marginalise_dynamic_from_U(key: PRNGKey, U_samples: UType, model: BaseAbstractModel, log_weights: jnp.ndarray,
                                ESS: jnp.ndarray,
                                fun: Callable[..., _V]) -> _V:
     """
@@ -125,29 +126,29 @@
         V = model.prepare_input(U=U)
         return fun(*V)
 
     def body(state):
         (key, i, count, marginalised) = state
         key, resample_key = random.split(key, 2)
         _samples = resample(resample_key, U_samples, log_weights, S=1)
-        _sample = tree_map(lambda v: v[0], _samples)
+        _sample = jax.tree.map(lambda v: v[0], _samples)
         update = _eval(_sample)
-        count = tree_map(lambda y, c: jnp.where(jnp.any(jnp.isnan(y)), c, c + jnp.asarray(1, c.dtype)),
-                         update, count)
-        marginalised = tree_map(lambda x, y: jnp.where(jnp.isnan(y), x, x + y.astype(x.dtype)),
-                                marginalised, update)
+        count = jax.tree.map(lambda y, c: jnp.where(jnp.any(jnp.isnan(y)), c, c + jnp.asarray(1, c.dtype)),
+                             update, count)
+        marginalised = jax.tree.map(lambda x, y: jnp.where(jnp.isnan(y), x, x + y.astype(x.dtype)),
+                                    marginalised, update)
         return (key, i + jnp.ones_like(i), count, marginalised)
 
-    test_output = fun(**tree_map(lambda v: v[0], U_samples))
-    count = tree_map(lambda x: jnp.asarray(0, x.dtype), test_output)
-    init_marginalised = tree_map(lambda x: jnp.zeros_like(x), test_output)
+    test_output = fun(**jax.tree.map(lambda v: v[0], U_samples))
+    count = jax.tree.map(lambda x: jnp.asarray(0, x.dtype), test_output)
+    init_marginalised = jax.tree.map(lambda x: jnp.zeros_like(x), test_output)
     (_, _, count, marginalised) = lax.while_loop(lambda state: state[1] < ESS,
                                                  body,
                                                  (key, jnp.array(0, ESS.dtype), count, init_marginalised))
-    marginalised = tree_map(lambda x, c: x / c, marginalised, count)
+    marginalised = jax.tree.map(lambda x, c: x / c, marginalised, count)
     return marginalised
 
 
 def marginalise_static(key: PRNGKey, samples: XType, log_weights: jnp.ndarray, ESS: int, fun: Callable[..., _V]) -> _V:
     """
     Marginalises function over posterior samples, where ESS is static.
 
@@ -159,15 +160,15 @@
         fun (:code:`callable(**kwargs)`): function to marginalise
 
     Returns:
         expectation over resampled samples
     """
     fun = prepare_func_args(fun)
     samples = resample(key, samples, log_weights, S=ESS, replace=True)
-    marginalised = tree_map(lambda marg: jnp.nanmean(marg, axis=0), vmap(fun)(**samples))
+    marginalised = jax.tree.map(lambda marg: jnp.nanmean(marg, axis=0), vmap(fun)(**samples))
     return marginalised
 
 
 def marginalise_dynamic(key: PRNGKey, samples: XType, log_weights: jnp.ndarray, ESS: jnp.ndarray,
                         fun: Callable[..., _V]) -> _V:
     """
     Marginalises function over posterior samples, where ESS can be dynamic.
@@ -185,29 +186,29 @@
     fun = prepare_func_args(fun)
     ESS = jnp.asarray(ESS)
 
     def body(state):
         (key, i, count, marginalised) = state
         key, resample_key = random.split(key, 2)
         _samples = resample(resample_key, samples, log_weights, S=1)
-        _sample = tree_map(lambda v: v[0], _samples)
+        _sample = jax.tree.map(lambda v: v[0], _samples)
         update = fun(**_sample)
-        count = tree_map(lambda y, c: jnp.where(jnp.any(jnp.isnan(y)), c, c + jnp.asarray(1, c.dtype)),
-                         update, count)
-        marginalised = tree_map(lambda x, y: jnp.where(jnp.isnan(y), x, x + y.astype(x.dtype)),
-                                marginalised, update)
+        count = jax.tree.map(lambda y, c: jnp.where(jnp.any(jnp.isnan(y)), c, c + jnp.asarray(1, c.dtype)),
+                             update, count)
+        marginalised = jax.tree.map(lambda x, y: jnp.where(jnp.isnan(y), x, x + y.astype(x.dtype)),
+                                    marginalised, update)
         return (key, i + jnp.ones_like(i), count, marginalised)
 
-    test_output = fun(**tree_map(lambda v: v[0], samples))
-    count = tree_map(lambda x: jnp.asarray(0, x.dtype), test_output)
-    init_marginalised = tree_map(lambda x: jnp.zeros_like(x), test_output)
+    test_output = fun(**jax.tree.map(lambda v: v[0], samples))
+    count = jax.tree.map(lambda x: jnp.asarray(0, x.dtype), test_output)
+    init_marginalised = jax.tree.map(lambda x: jnp.zeros_like(x), test_output)
     (_, _, count, marginalised) = lax.while_loop(lambda state: state[1] < ESS,
                                                  body,
                                                  (key, jnp.array(0, ESS.dtype), count, init_marginalised))
-    marginalised = tree_map(lambda x, c: x / c, marginalised, count)
+    marginalised = jax.tree.map(lambda x, c: x / c, marginalised, count)
     return marginalised
 
 
 def maximum_a_posteriori_point(results: NestedSamplerResults) -> XType:
     """
     Get the MAP point of a nested sampling result.
     Does this by choosing the point with largest L(x) p(x).
@@ -216,15 +217,15 @@
         results (NestedSamplerResult): Nested sampler result
 
     Returns:
         dict of samples at MAP-point.
     """
 
     map_idx = jnp.argmax(results.log_posterior_density)
-    map_points = tree_map(lambda x: x[map_idx], results.samples)
+    map_points = jax.tree.map(lambda x: x[map_idx], results.samples)
     return map_points
 
 
 def maximum_a_posteriori_point_U(results: NestedSamplerResults) -> UType:
     """
     Get the MAP point of a nested sampling result.
     Does this by choosing the point with largest L(x) p(x).
@@ -233,15 +234,15 @@
         results (NestedSamplerResult): Nested sampler result
 
     Returns:
         dict of samples at MAP-point.
     """
 
     map_idx = jnp.argmax(results.log_posterior_density)
-    map_points = tree_map(lambda x: x[map_idx], results.U_samples)
+    map_points = jax.tree.map(lambda x: x[map_idx], results.U_samples)
     return map_points
 
 
 def evaluate_map_estimate(results: NestedSamplerResults, fun: Callable[..., _V]) -> _V:
     """
     Marginalises function over posterior samples, where ESS is static.
 
@@ -350,24 +351,24 @@
     )
 
     samples = results.samples
     if with_parametrised:
         samples.update(results.parametrised_samples)
 
     max_like_idx = np.argmax(results.log_L_samples)
-    max_like_points = tree_map(lambda x: x[max_like_idx], samples)
+    max_like_points = jax.tree.map(lambda x: x[max_like_idx], samples)
 
     uniform_samples = resample(random.PRNGKey(23426),
                                samples,
                                results.log_dp_mean,
                                S=max(100, int(results.ESS)),
                                replace=True)
 
     max_map_idx = np.argmax(results.log_posterior_density)
-    map_points = tree_map(lambda x: x[max_map_idx], results.samples)
+    map_points = jax.tree.map(lambda x: x[max_map_idx], results.samples)
 
     for name in uniform_samples.keys():
         _samples = uniform_samples[name].reshape((uniform_samples[name].shape[0], -1))
         _max_like_points = max_like_points[name].reshape((-1,))
         _map_points = map_points[name].reshape((-1,))
         ndims = _samples.shape[1]
         _print("--------")
@@ -499,91 +500,72 @@
     Args:
         model: model
         S: resolution of grid
 
     Returns:
         log(Z)
     """
-    logger.warning(f"")
+    warnings.warn(f"")
 
     u_vec = jnp.linspace(jnp.finfo(float_type).eps, 1. - jnp.finfo(float_type).eps, S)
     du = u_vec[1] - u_vec[0]
     args = jnp.stack([x.flatten() for x in jnp.meshgrid(*[u_vec] * model.U_ndims, indexing='ij')], axis=-1)
     samples = jit(vmap(model.transform))(args)
     log_L = jit(vmap(model.forward))(args)
     dZ = LogSpace(log_L) * LogSpace(jnp.log(du)) ** model.U_ndims
     return samples, dZ.log_abs_val
 
 
 def save_pytree(pytree: NamedTuple, save_file: str):
     """
-    Saves results of nested sampler in a npz file.
+    Saves results of nested sampler in a json file.
 
     Args:
         pytree: Nested sampler result
         save_file: filename
     """
-    pytree_np = tree_map(lambda v: np.asarray(v) if v is not None else None, pytree)
-
-    def _pytree_asdict(pytree):
-        _data_dict = pytree._asdict()
-        data_dict = {}
-        for k, v in _data_dict.items():
-            if isinstance_namedtuple(v):
-                data_dict[k] = _pytree_asdict(v)
-            elif isinstance(v, (dict, np.ndarray, None.__class__)):
-                data_dict[k] = v
-            else:
-                raise ValueError("key, value pair {}, {} unknown".format(k, v))
-        return data_dict
-
-    data_dict = _pytree_asdict(pytree_np)
-    np.savez(save_file, **data_dict)
+    if not isinstance_namedtuple(pytree):
+        raise ValueError(f"Expected NamedTuple, got {type(pytree)}")
+    with open(save_file, 'w') as fp:
+        json.dump(serialise_namedtuple(pytree), fp, indent=2)
 
 
 def save_results(results: NestedSamplerResults, save_file: str):
     """
-    Saves results of nested sampler in a npz file.
+    Saves results of nested sampler in a json file.
 
     Args:
         results (NestedSamplerResults): Nested sampler result
         save_file (str): filename
     """
+    if not save_file.lower().endswith('.json'):
+        warnings.warn(f"Filename {save_file} does not end with .json. "
+                      f"We let this pass, but you should consider using a .json file extension.")
     save_pytree(results, save_file)
 
 
 def load_pytree(save_file: str):
     """
-    Loads saved nested sampler results from a npz file.
+    Loads saved nested sampler results from a json file.
 
     Args:
         save_file (str): filename
 
     Returns:
         NestedSamplerResults
     """
-    _data_dict = np.load(save_file, allow_pickle=True)
-    data_dict = {}
-    for k, v in _data_dict.items():
-        if v.size == 1:
-            if v.item() is None:
-                data_dict[k] = None
-            else:
-                data_dict[k] = tree_map(lambda v: jnp.asarray(v), v.item())
-        else:
-            data_dict[k] = jnp.asarray(v)
-
-    return data_dict
+    with open(save_file, 'r') as fp:
+        data_dict = json.load(fp)
+    return deserialise_namedtuple(data_dict)
 
 
 def load_results(save_file: str) -> NestedSamplerResults:
     """
-    Loads saved nested sampler results from a npz file.
+    Loads saved nested sampler results from a json file.
 
     Args:
         save_file (str): filename
 
     Returns:
         NestedSamplerResults
     """
-    data_dict = load_pytree(save_file)
-    return NestedSamplerResults(**data_dict)
+    return load_pytree(save_file)
```

### Comparing `jaxns-2.4.9/jaxns.egg-info/PKG-INFO` & `jaxns-2.5.0/jaxns.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: jaxns
-Version: 2.4.9
+Version: 2.5.0
 Summary: Nested Sampling in JAX
 Home-page: https://github.com/joshuaalbert/jaxns
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: jax
+Requires-Dist: jax>=0.4.25
 Requires-Dist: jaxlib
-Requires-Dist: chex
-Requires-Dist: typing_extensions
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: tensorflow_probability
 Requires-Dist: tqdm
 Requires-Dist: dm-haiku
 Requires-Dist: optax
@@ -189,15 +187,20 @@
 # Just-in-time compilation (usually useful)
 ns_jit = jax.jit(ns)
 ```
 
 You can inspect the results, and plot them.
 
 ```python
-from jaxns import summary, plot_diagnostics, plot_cornerplot
+from jaxns import summary, plot_diagnostics, plot_cornerplot, save_results, load_results
+
+# Optionally save the results to file
+save_results(results, 'results.json')
+# To load the results back use this
+results = load_results('results.json')
 
 summary(results)
 plot_diagnostics(results)
 plot_cornerplot(results)
 ```
 
 Output:
@@ -241,14 +244,63 @@
     samples=results.samples,
     log_weights=results.log_dp_mean,
     S=1000,
     replace=True
 )
 ```
 
+### Maximising the evidence
+
+The Bayesian evidence is the ultimate model selection density, and choosing a model that maximises the evidence is
+the best way to select a model. We can use the evidence maximisation algorithm to optimise the parametrised variables
+of the model, in the manner that maximises the evidence. Below `EvidenceMaximisation` does this for the model we defined
+above, where the parametrised variables are
+automatically constrained to be in the right range, and numerical stability is ensured with proper scaling.
+
+We see that the evidence maximisation chooses a `sigma` the is very small.
+
+```python
+from jaxns.experimental import EvidenceMaximisation
+
+# Let's train the sigma parameter to maximise the evidence
+
+em = EvidenceMaximisation(model, ns_kwargs=dict(max_samples=1e4))
+results, params = em.train(num_steps=5)
+
+summary(results, with_parametrised=True)
+```
+
+Output:
+
+```
+--------
+Termination Conditions:
+Small remaining evidence
+--------
+likelihood evals: 72466
+samples: 1440
+phantom samples: 0
+likelihood evals / sample: 50.3
+phantom fraction (%): 0.0%
+--------
+logZ=-1.119 +- 0.098
+H=-0.93
+ESS=241
+--------
+sigma: mean +- std.dev. | 10%ile / 50%ile / 90%ile | MAP est. | max(L) est.
+sigma: 5.40077599e-05 +- 3.6e-12 | 5.40077563e-05 / 5.40077563e-05 / 5.40077563e-05 | 5.40077563e-05 | 5.40077563e-05
+--------
+uncert: mean +- std.dev. | 10%ile / 50%ile / 90%ile | MAP est. | max(L) est.
+uncert: 0.6 +- 0.54 | 0.05 / 0.45 / 1.37 | 0.0 | 0.0
+--------
+x: mean +- std.dev. | 10%ile / 50%ile / 90%ile | MAP est. | max(L) est.
+x: 0.01 +- 0.56 | -0.6 / -0.0 / 0.69 | 0.0 | -0.0
+--------
+```
+
 # Documentation
 
 You can read the documentation [here](https://jaxns.readthedocs.io/en/latest/#). In addition, JAXNS is partially
 described in the
 [original paper](https://arxiv.org/abs/2012.15286), as well as the paper on [Phantom-Powered Nested
 Sampling paper](https://arxiv.org/abs/2312.11330).
 
@@ -331,17 +383,30 @@
 The algorithm is fairly memory bound, so running parallelisation over multiple CPUs on the same machine may not yield
 the expected speed up, and depends on how expensive the likelihood evaluations are. Running over separate physical
 devices
 is the best way to achieve speed up.
 
 # Change Log
 
+15 May, 2024 -- JAXNS 2.5.0 released. Added ability to handle non-JAX likelihoods, e.g. if you have a simulation
+framework with python bindings you can now use it for likelihoods in JAXNS. Small performance improvements.
+
+22 Apr, 2024 -- JAXNS 2.4.13 released. Fixes bug where slice sampling not invariant to monotonic transforms of
+likelihod.
+
+20 Mar, 2024 -- JAXNS 2.4.12 released. Minor bug fixes, and readability improvements. Added Empirical special prior.
+
+5 Mar, 2024 -- JAXNS 2.4.11/b released. Add `random_init` to parametrised variables. Enable special priors to be
+parametrised.
+
+23 Feb, 2024 -- JAXNS 2.4.10 released. Hotfix for import error.
+
 21 Feb, 2024 -- JAXNS 2.4.9 released. Minor improvements to some priors, and bug fixes.
 
-31 Jan, 2024 -- JAXNS 2.4.8 released. Improved global optimisation performance using gradient slicing. 
+31 Jan, 2024 -- JAXNS 2.4.8 released. Improved global optimisation performance using gradient slicing.
 Improved evidence maximisation.
 
 25 Jan, 2024 -- JAXNS 2.4.6/7 released. Added logging. Use L-BFGS for Evidence Maximisation M-step. Fix bug in finetune.
 
 24 Jan, 2024 -- JAXNS 2.4.5 released. Gradient based finetuning global optimisation using L-BFGS. Added ability to
 simulate prior models without bulding model (for data generation.)
```

### Comparing `jaxns-2.4.9/jaxns.egg-info/SOURCES.txt` & `jaxns-2.5.0/jaxns.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,38 +18,43 @@
 ./jaxns/experimental/public.py
 ./jaxns/experimental/tests/__init__.py
 ./jaxns/experimental/tests/test_evidence_maximisation.py
 ./jaxns/experimental/tests/test_global_optimisation.py
 ./jaxns/framework/__init__.py
 ./jaxns/framework/abc.py
 ./jaxns/framework/bases.py
-./jaxns/framework/distribution.py
+./jaxns/framework/jaxify.py
 ./jaxns/framework/model.py
 ./jaxns/framework/ops.py
 ./jaxns/framework/prior.py
 ./jaxns/framework/special_priors.py
+./jaxns/framework/wrapped_tfp_distribution.py
 ./jaxns/framework/tests/__init__.py
+./jaxns/framework/tests/test_jaxify.py
 ./jaxns/framework/tests/test_model.py
 ./jaxns/framework/tests/test_prior.py
 ./jaxns/internals/__init__.py
 ./jaxns/internals/cumulative_ops.py
 ./jaxns/internals/linalg.py
 ./jaxns/internals/log_semiring.py
+./jaxns/internals/logging.py
 ./jaxns/internals/maps.py
+./jaxns/internals/namedtuple_utils.py
 ./jaxns/internals/random.py
 ./jaxns/internals/shapes.py
 ./jaxns/internals/shrinkage_statistics.py
 ./jaxns/internals/stats.py
 ./jaxns/internals/tree_structure.py
 ./jaxns/internals/types.py
 ./jaxns/internals/tests/__init__.py
 ./jaxns/internals/tests/test_cumulative_ops.py
 ./jaxns/internals/tests/test_linalg.py
 ./jaxns/internals/tests/test_log_semiring.py
 ./jaxns/internals/tests/test_maps.py
+./jaxns/internals/tests/test_namedtuple_utils.py
 ./jaxns/internals/tests/test_random.py
 ./jaxns/internals/tests/test_shapes.py
 ./jaxns/internals/tests/test_shrink_statistics.py
 ./jaxns/internals/tests/test_stats.py
 ./jaxns/internals/tests/test_tree_structure.py
 ./jaxns/internals/tests/test_types.py
 ./jaxns/nested_sampler/__init__.py
```

### Comparing `jaxns-2.4.9/setup.py` & `jaxns-2.5.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages
 from setuptools import setup
 
 install_requires = [
-    'jax',
+    'jax>=0.4.25',
     'jaxlib',
-    'chex',
-    'typing_extensions',
     'matplotlib',
     'numpy',
     'scipy',
     'tensorflow_probability',
     'tqdm',
     'dm-haiku',
     'optax',
     'jaxopt'
 ]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='jaxns',
-      version='2.4.9',
+      version='2.5.0',
       description='Nested Sampling in JAX',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/joshuaalbert/jaxns",
       author='Joshua G. Albert',
       author_email='albert@strw.leidenuniv.nl',
       install_requires=install_requires,
```

