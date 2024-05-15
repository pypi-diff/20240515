# Comparing `tmp/boax-0.1.1.tar.gz` & `tmp/boax-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boax-0.1.1.tar", last modified: Thu Apr  4 20:46:33 2024, max compression
+gzip compressed data, was "boax-0.1.2.tar", last modified: Wed May 15 05:56:23 2024, max compression
```

## Comparing `boax-0.1.1.tar` & `boax-0.1.2.tar`

### file list

```diff
@@ -1,101 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.501217 boax-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-04 20:46:22.000000 boax-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-04 20:46:33.501217 boax-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-04-04 20:46:22.000000 boax-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.489217 boax-0.1.1/boax/
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-04 20:46:22.000000 boax-0.1.1/boax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.489217 boax-0.1.1/boax/core/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-04 20:46:22.000000 boax-0.1.1/boax/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.489217 boax-0.1.1/boax/core/distributions/
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-04 20:46:22.000000 boax-0.1.1/boax/core/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-04 20:46:22.000000 boax-0.1.1/boax/core/distributions/beta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-04 20:46:22.000000 boax-0.1.1/boax/core/distributions/gamma.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-04 20:46:22.000000 boax-0.1.1/boax/core/distributions/multivariate_normal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-04 20:46:22.000000 boax-0.1.1/boax/core/distributions/normal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-04 20:46:22.000000 boax-0.1.1/boax/core/distributions/poisson.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-04 20:46:22.000000 boax-0.1.1/boax/core/distributions/transformed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-04 20:46:22.000000 boax-0.1.1/boax/core/distributions/uniform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.489217 boax-0.1.1/boax/core/samplers/
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-04 20:46:22.000000 boax-0.1.1/boax/core/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-04 20:46:22.000000 boax-0.1.1/boax/core/samplers/alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-04 20:46:22.000000 boax-0.1.1/boax/core/samplers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.489217 boax-0.1.1/boax/core/samplers/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-04 20:46:22.000000 boax-0.1.1/boax/core/samplers/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-04 20:46:22.000000 boax-0.1.1/boax/core/samplers/functions/quasi_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-04 20:46:22.000000 boax-0.1.1/boax/core/samplers/functions/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.489217 boax-0.1.1/boax/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-04 20:46:22.000000 boax-0.1.1/boax/optimization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.493217 boax-0.1.1/boax/optimization/acquisitions/
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-04 20:46:22.000000 boax-0.1.1/boax/optimization/acquisitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-04-04 20:46:22.000000 boax-0.1.1/boax/optimization/acquisitions/alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-04 20:46:22.000000 boax-0.1.1/boax/optimization/acquisitions/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.493217 boax-0.1.1/boax/optimization/acquisitions/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-04 20:46:22.000000 boax-0.1.1/boax/optimization/acquisitions/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-04 20:46:22.000000 boax-0.1.1/boax/optimization/acquisitions/constraints/alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-04 20:46:22.000000 boax-0.1.1/boax/optimization/acquisitions/constraints/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.493217 boax-0.1.1/boax/optimization/acquisitions/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-04 20:46:22.000000 boax-0.1.1/boax/optimization/acquisitions/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-04 20:46:22.000000 boax-0.1.1/boax/optimization/acquisitions/functions/analytic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-04 20:46:22.000000 boax-0.1.1/boax/optimization/acquisitions/functions/monte_carlo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-04 20:46:22.000000 boax-0.1.1/boax/optimization/acquisitions/transformed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.493217 boax-0.1.1/boax/optimization/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-04 20:46:22.000000 boax-0.1.1/boax/optimization/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-04 20:46:22.000000 boax-0.1.1/boax/optimization/optimizers/alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-04 20:46:22.000000 boax-0.1.1/boax/optimization/optimizers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.493217 boax-0.1.1/boax/optimization/optimizers/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-04 20:46:22.000000 boax-0.1.1/boax/optimization/optimizers/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-04 20:46:22.000000 boax-0.1.1/boax/optimization/optimizers/functions/initialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-04 20:46:22.000000 boax-0.1.1/boax/optimization/optimizers/functions/scipy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.493217 boax-0.1.1/boax/prediction/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.493217 boax-0.1.1/boax/prediction/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.493217 boax-0.1.1/boax/prediction/models/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/functions/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/functions/multi_fidelity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.497217 boax-0.1.1/boax/prediction/models/kernels/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/kernels/alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/kernels/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.497217 boax-0.1.1/boax/prediction/models/kernels/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/kernels/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/kernels/functions/distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/kernels/functions/matern.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/kernels/functions/periodic.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/kernels/functions/rbf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/kernels/functions/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/kernels/transformed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.497217 boax-0.1.1/boax/prediction/models/likelihoods/
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/likelihoods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/likelihoods/alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/likelihoods/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.497217 boax-0.1.1/boax/prediction/models/likelihoods/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/likelihoods/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/likelihoods/functions/conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/likelihoods/functions/marginal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.497217 boax-0.1.1/boax/prediction/models/means/
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/means/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/means/alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/means/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/transformed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.497217 boax-0.1.1/boax/prediction/objectives/
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/objectives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/objectives/alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/objectives/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/objectives/transformed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.497217 boax-0.1.1/boax/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-04 20:46:22.000000 boax-0.1.1/boax/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-04-04 20:46:22.000000 boax-0.1.1/boax/utils/functools.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-04 20:46:22.000000 boax-0.1.1/boax/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-04 20:46:22.000000 boax-0.1.1/boax/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.497217 boax-0.1.1/boax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-04 20:46:33.000000 boax-0.1.1/boax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-04-04 20:46:33.000000 boax-0.1.1/boax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 20:46:33.000000 boax-0.1.1/boax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-04 20:46:33.000000 boax-0.1.1/boax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-04 20:46:33.000000 boax-0.1.1/boax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-04 20:46:22.000000 boax-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 20:46:33.501217 boax-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:56:23.207525 boax-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-15 05:56:12.000000 boax-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-05-15 05:56:23.207525 boax-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-05-15 05:56:12.000000 boax-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:56:23.191525 boax-0.1.2/boax/
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-15 05:56:12.000000 boax-0.1.2/boax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:56:23.195525 boax-0.1.2/boax/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-15 05:56:12.000000 boax-0.1.2/boax/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:56:23.195525 boax-0.1.2/boax/core/distributions/
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-15 05:56:12.000000 boax-0.1.2/boax/core/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-05-15 05:56:12.000000 boax-0.1.2/boax/core/distributions/beta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-15 05:56:12.000000 boax-0.1.2/boax/core/distributions/gamma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-15 05:56:12.000000 boax-0.1.2/boax/core/distributions/multivariate_normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-15 05:56:12.000000 boax-0.1.2/boax/core/distributions/normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-15 05:56:12.000000 boax-0.1.2/boax/core/distributions/poisson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-15 05:56:12.000000 boax-0.1.2/boax/core/distributions/transformed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-15 05:56:12.000000 boax-0.1.2/boax/core/distributions/uniform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:56:23.195525 boax-0.1.2/boax/core/samplers/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-15 05:56:12.000000 boax-0.1.2/boax/core/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-05-15 05:56:12.000000 boax-0.1.2/boax/core/samplers/alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-15 05:56:12.000000 boax-0.1.2/boax/core/samplers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:56:23.195525 boax-0.1.2/boax/core/samplers/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-15 05:56:12.000000 boax-0.1.2/boax/core/samplers/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-15 05:56:12.000000 boax-0.1.2/boax/core/samplers/functions/iid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-15 05:56:12.000000 boax-0.1.2/boax/core/samplers/functions/quasi_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-15 05:56:12.000000 boax-0.1.2/boax/core/samplers/functions/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:56:23.195525 boax-0.1.2/boax/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-15 05:56:12.000000 boax-0.1.2/boax/optimization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:56:23.195525 boax-0.1.2/boax/optimization/acquisitions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-15 05:56:12.000000 boax-0.1.2/boax/optimization/acquisitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9086 2024-05-15 05:56:12.000000 boax-0.1.2/boax/optimization/acquisitions/alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-15 05:56:12.000000 boax-0.1.2/boax/optimization/acquisitions/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:56:23.199525 boax-0.1.2/boax/optimization/acquisitions/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-15 05:56:12.000000 boax-0.1.2/boax/optimization/acquisitions/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-15 05:56:12.000000 boax-0.1.2/boax/optimization/acquisitions/constraints/alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-15 05:56:12.000000 boax-0.1.2/boax/optimization/acquisitions/constraints/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:56:23.199525 boax-0.1.2/boax/optimization/acquisitions/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-15 05:56:12.000000 boax-0.1.2/boax/optimization/acquisitions/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-15 05:56:12.000000 boax-0.1.2/boax/optimization/acquisitions/functions/analytic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-15 05:56:12.000000 boax-0.1.2/boax/optimization/acquisitions/functions/monte_carlo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-15 05:56:12.000000 boax-0.1.2/boax/optimization/acquisitions/transformed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:56:23.199525 boax-0.1.2/boax/optimization/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-15 05:56:12.000000 boax-0.1.2/boax/optimization/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-15 05:56:12.000000 boax-0.1.2/boax/optimization/optimizers/alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-15 05:56:12.000000 boax-0.1.2/boax/optimization/optimizers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:56:23.199525 boax-0.1.2/boax/optimization/optimizers/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-15 05:56:12.000000 boax-0.1.2/boax/optimization/optimizers/initializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-15 05:56:12.000000 boax-0.1.2/boax/optimization/optimizers/initializers/alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-15 05:56:12.000000 boax-0.1.2/boax/optimization/optimizers/initializers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:56:23.199525 boax-0.1.2/boax/optimization/optimizers/solvers/
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-15 05:56:12.000000 boax-0.1.2/boax/optimization/optimizers/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-15 05:56:12.000000 boax-0.1.2/boax/optimization/optimizers/solvers/alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-15 05:56:12.000000 boax-0.1.2/boax/optimization/optimizers/solvers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:56:23.199525 boax-0.1.2/boax/prediction/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-15 05:56:12.000000 boax-0.1.2/boax/prediction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:56:23.199525 boax-0.1.2/boax/prediction/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-15 05:56:12.000000 boax-0.1.2/boax/prediction/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-15 05:56:12.000000 boax-0.1.2/boax/prediction/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:56:23.199525 boax-0.1.2/boax/prediction/models/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-15 05:56:12.000000 boax-0.1.2/boax/prediction/models/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-15 05:56:12.000000 boax-0.1.2/boax/prediction/models/functions/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-15 05:56:12.000000 boax-0.1.2/boax/prediction/models/functions/multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-05-15 05:56:12.000000 boax-0.1.2/boax/prediction/models/gaussian_process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:56:23.203525 boax-0.1.2/boax/prediction/models/kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-15 05:56:12.000000 boax-0.1.2/boax/prediction/models/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-15 05:56:12.000000 boax-0.1.2/boax/prediction/models/kernels/alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-15 05:56:12.000000 boax-0.1.2/boax/prediction/models/kernels/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:56:23.203525 boax-0.1.2/boax/prediction/models/kernels/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-15 05:56:12.000000 boax-0.1.2/boax/prediction/models/kernels/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-15 05:56:12.000000 boax-0.1.2/boax/prediction/models/kernels/functions/distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-15 05:56:12.000000 boax-0.1.2/boax/prediction/models/kernels/functions/matern.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-15 05:56:12.000000 boax-0.1.2/boax/prediction/models/kernels/functions/periodic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-15 05:56:12.000000 boax-0.1.2/boax/prediction/models/kernels/functions/rbf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-15 05:56:12.000000 boax-0.1.2/boax/prediction/models/kernels/functions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-05-15 05:56:12.000000 boax-0.1.2/boax/prediction/models/kernels/transformed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:56:23.203525 boax-0.1.2/boax/prediction/models/likelihoods/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-15 05:56:12.000000 boax-0.1.2/boax/prediction/models/likelihoods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-15 05:56:12.000000 boax-0.1.2/boax/prediction/models/likelihoods/alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-15 05:56:12.000000 boax-0.1.2/boax/prediction/models/likelihoods/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:56:23.203525 boax-0.1.2/boax/prediction/models/likelihoods/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-15 05:56:12.000000 boax-0.1.2/boax/prediction/models/likelihoods/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-15 05:56:12.000000 boax-0.1.2/boax/prediction/models/likelihoods/functions/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-15 05:56:12.000000 boax-0.1.2/boax/prediction/models/likelihoods/functions/marginal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:56:23.203525 boax-0.1.2/boax/prediction/models/means/
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-15 05:56:12.000000 boax-0.1.2/boax/prediction/models/means/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-15 05:56:12.000000 boax-0.1.2/boax/prediction/models/means/alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-15 05:56:12.000000 boax-0.1.2/boax/prediction/models/means/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-05-15 05:56:12.000000 boax-0.1.2/boax/prediction/models/transformed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:56:23.203525 boax-0.1.2/boax/prediction/objectives/
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-15 05:56:12.000000 boax-0.1.2/boax/prediction/objectives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-15 05:56:12.000000 boax-0.1.2/boax/prediction/objectives/alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-15 05:56:12.000000 boax-0.1.2/boax/prediction/objectives/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-15 05:56:12.000000 boax-0.1.2/boax/prediction/objectives/transformed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:56:23.207525 boax-0.1.2/boax/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-15 05:56:12.000000 boax-0.1.2/boax/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-15 05:56:12.000000 boax-0.1.2/boax/utils/functools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-15 05:56:12.000000 boax-0.1.2/boax/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-15 05:56:12.000000 boax-0.1.2/boax/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:56:23.207525 boax-0.1.2/boax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-05-15 05:56:23.000000 boax-0.1.2/boax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-15 05:56:23.000000 boax-0.1.2/boax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 05:56:23.000000 boax-0.1.2/boax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-15 05:56:23.000000 boax-0.1.2/boax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 05:56:23.000000 boax-0.1.2/boax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-15 05:56:12.000000 boax-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 05:56:23.207525 boax-0.1.2/setup.cfg
```

### Comparing `boax-0.1.1/LICENSE` & `boax-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/PKG-INFO` & `boax-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boax
-Version: 0.1.1
+Version: 0.1.2
 Summary: Boax is a Bayesian Optimization library for JAX.
 Project-URL: homepage, https://github.com/Lando-L/boax
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.11
@@ -46,22 +46,18 @@
 
 Boax is a composable library of core components for Bayesian Optimization that is **designed for flexibility**. It comes with low-level interfaces for:
 
 * **Core capabilities** (`boax.core`):
   * Common Distributions
   * Monte-Carlo Samplers
 * **Fitting a surrogate model to data** (`boax.prediction`):
-  * Kernels Functions
-  * Likelihood Functions
-  * Mean Functions
   * Model Functions
   * Objective Functions
 * **Constructing and optimizing acquisition functions** (`boax.optimization`):
   * Acquisition Functions
-  * Constraint Functions
   * Optimizer Functions
 
 ## Installation
 
 You can install the latest released version of Boax from PyPI via:
 
 ```sh
@@ -72,70 +68,82 @@
 
 ```sh
 pip install git+https://github.com/Lando-L/boax.git
 ```
 
 ## Basic Usage
 
-Here is a basic example of using the Boax API for defining a Gaussian Process model, constructing an Acquisition function, and combining the two for optimzation. For more details check out the [docs](https://boax.readthedocs.io/en/latest/).
+Here is a basic example of using the Boax API for defining a Gaussian Process model, constructing an Acquisition function, and generating the next batch of data points to query. For more details check out the [docs](https://boax.readthedocs.io/en/latest/).
 
 1. Defining a Gaussian Process model:
 
 ```python
 from boax.prediction import models
 
-model = models.gaussian_process(
+model = models.gaussian_process.exact(
   models.means.zero(),
   models.kernels.scaled(
-    models.kernels.rbf(1.0),
-    0.5
+    models.kernels.rbf(1.0), 0.5
   ),
   models.likelihoods.gaussian(1e-4),
   x_train,
   y_train,
 )
 ```
 
 2. Constructing an Acquisition function.
 
 ```python
+from jax import vmap
 from boax.optimization import acquisitions
 
-acquisition = acquisitions.upper_confidence_bound(
-  beta=2.0
+acqf = models.outcome_transformed(
+  vmap(model),
+  acquisitions.upper_confidence_bound(2.0)
 )
 ```
 
-3. Combining the two for optimization
+3. Generating the next batch of data points to query.
 
 ```python
-from jax import jit, random, vmap
 from jax import numpy as jnp
+from jax import random
+from boax.core import distributions, samplers
 from boax.optimization import optimizers
 
-def acqf(x):
-  return acquisition(vmap(model)(x))
+key = random.key(0)
 
-key1, key2 = random.split(random.key(0))
+batch_size, num_results, num_restarts = 1, 100, 10
 bounds = jnp.array([[-1.0, 1.0]])
-x0 = random.uniform(key1, shape=(100, 1, 1))
-bfgs = optimizers.bfgs(jit(acqf), bounds, x0, 10)
-candidates = bfgs.init(key2)
-next_candidates, values = bfgs.update(candidates)
+
+sampler = samplers.halton_uniform(
+  distributions.uniform.uniform(bounds[:, 0], bounds[:, 1])
+)
+
+optimizer = optimizers.batch(
+  optimizers.initializers.q_batch(
+    acqf, sampler, batch_size, num_results, num_restarts,
+  ),
+  optimizers.solvers.scipy(
+    acqf, bounds,  
+  ),
+)
+
+next_x, value = optimizer(key)
 ```
 
 ## Citing Boax
 
 To cite Boax please use the citation:
 
 ```bibtex
 @software{boax2023github,
   author = {Lando L{\"o}per},
   title = {{B}oax: A Bayesian Optimization library for {JAX}},
   url = {https://github.com/Lando-L/boax},
-  version = {0.1.1},
+  version = {0.1.2},
   year = {2023},
 }
 ```
 
 In the above bibtex entry, the version number
 is intended to be that from [boax/version.py](https://github.com/Lando-L/boax/blob/main/boax/version.py), and the year corresponds to the project's open-source release.
```

### Comparing `boax-0.1.1/README.md` & `boax-0.1.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -14,22 +14,18 @@
 
 Boax is a composable library of core components for Bayesian Optimization that is **designed for flexibility**. It comes with low-level interfaces for:
 
 * **Core capabilities** (`boax.core`):
   * Common Distributions
   * Monte-Carlo Samplers
 * **Fitting a surrogate model to data** (`boax.prediction`):
-  * Kernels Functions
-  * Likelihood Functions
-  * Mean Functions
   * Model Functions
   * Objective Functions
 * **Constructing and optimizing acquisition functions** (`boax.optimization`):
   * Acquisition Functions
-  * Constraint Functions
   * Optimizer Functions
 
 ## Installation
 
 You can install the latest released version of Boax from PyPI via:
 
 ```sh
@@ -40,70 +36,82 @@
 
 ```sh
 pip install git+https://github.com/Lando-L/boax.git
 ```
 
 ## Basic Usage
 
-Here is a basic example of using the Boax API for defining a Gaussian Process model, constructing an Acquisition function, and combining the two for optimzation. For more details check out the [docs](https://boax.readthedocs.io/en/latest/).
+Here is a basic example of using the Boax API for defining a Gaussian Process model, constructing an Acquisition function, and generating the next batch of data points to query. For more details check out the [docs](https://boax.readthedocs.io/en/latest/).
 
 1. Defining a Gaussian Process model:
 
 ```python
 from boax.prediction import models
 
-model = models.gaussian_process(
+model = models.gaussian_process.exact(
   models.means.zero(),
   models.kernels.scaled(
-    models.kernels.rbf(1.0),
-    0.5
+    models.kernels.rbf(1.0), 0.5
   ),
   models.likelihoods.gaussian(1e-4),
   x_train,
   y_train,
 )
 ```
 
 2. Constructing an Acquisition function.
 
 ```python
+from jax import vmap
 from boax.optimization import acquisitions
 
-acquisition = acquisitions.upper_confidence_bound(
-  beta=2.0
+acqf = models.outcome_transformed(
+  vmap(model),
+  acquisitions.upper_confidence_bound(2.0)
 )
 ```
 
-3. Combining the two for optimization
+3. Generating the next batch of data points to query.
 
 ```python
-from jax import jit, random, vmap
 from jax import numpy as jnp
+from jax import random
+from boax.core import distributions, samplers
 from boax.optimization import optimizers
 
-def acqf(x):
-  return acquisition(vmap(model)(x))
+key = random.key(0)
 
-key1, key2 = random.split(random.key(0))
+batch_size, num_results, num_restarts = 1, 100, 10
 bounds = jnp.array([[-1.0, 1.0]])
-x0 = random.uniform(key1, shape=(100, 1, 1))
-bfgs = optimizers.bfgs(jit(acqf), bounds, x0, 10)
-candidates = bfgs.init(key2)
-next_candidates, values = bfgs.update(candidates)
+
+sampler = samplers.halton_uniform(
+  distributions.uniform.uniform(bounds[:, 0], bounds[:, 1])
+)
+
+optimizer = optimizers.batch(
+  optimizers.initializers.q_batch(
+    acqf, sampler, batch_size, num_results, num_restarts,
+  ),
+  optimizers.solvers.scipy(
+    acqf, bounds,  
+  ),
+)
+
+next_x, value = optimizer(key)
 ```
 
 ## Citing Boax
 
 To cite Boax please use the citation:
 
 ```bibtex
 @software{boax2023github,
   author = {Lando L{\"o}per},
   title = {{B}oax: A Bayesian Optimization library for {JAX}},
   url = {https://github.com/Lando-L/boax},
-  version = {0.1.1},
+  version = {0.1.2},
   year = {2023},
 }
 ```
 
 In the above bibtex entry, the version number
 is intended to be that from [boax/version.py](https://github.com/Lando-L/boax/blob/main/boax/version.py), and the year corresponds to the project's open-source release.
```

### Comparing `boax-0.1.1/boax/__init__.py` & `boax-0.1.2/boax/__init__.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/core/__init__.py` & `boax-0.1.2/boax/core/__init__.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/core/distributions/__init__.py` & `boax-0.1.2/boax/core/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/core/distributions/beta.py` & `boax-0.1.2/boax/core/distributions/beta.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/core/distributions/gamma.py` & `boax-0.1.2/boax/core/distributions/gamma.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
   a: Array
   b: Array
 
 
 def gamma(a: Array, b: Array = jnp.ones(())) -> Gamma:
   """
-  Smart constructor for the beta distribution.
+  Smart constructor for the gamma distribution.
 
   Args:
     a: The shape parameter.
     b: The rate parameter.
 
   Returns:
     The `Gamma` distribution object.
```

### Comparing `boax-0.1.1/boax/core/distributions/multivariate_normal.py` & `boax-0.1.2/boax/core/distributions/multivariate_normal.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/core/distributions/normal.py` & `boax-0.1.2/boax/core/distributions/normal.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/core/distributions/poisson.py` & `boax-0.1.2/boax/core/distributions/poisson.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
   """
 
   mu: Array
 
 
 def poisson(mu: Array) -> Poisson:
   """
-  Smart constructor for the beta distribution.
+  Smart constructor for the poisson distribution.
 
   Args:
     mu: The rate parameter.
 
   Returns:
     The `Poisson` distribution object.
   """
```

### Comparing `boax-0.1.1/boax/core/distributions/transformed.py` & `boax-0.1.2/boax/core/distributions/transformed.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/core/distributions/uniform.py` & `boax-0.1.2/boax/core/distributions/uniform.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/core/samplers/__init__.py` & `boax-0.1.2/boax/prediction/models/likelihoods/functions/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,12 +8,11 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""The samplers sub-package."""
+"""The likelihood functions sub-package."""
 
-from .alias import halton_normal as halton_normal
-from .alias import halton_uniform as halton_uniform
-from .base import Sampler as Sampler
+from . import conditional as conditional
+from . import marginal as marginal
```

### Comparing `boax-0.1.1/boax/core/samplers/alias.py` & `boax-0.1.2/boax/core/samplers/alias.py`

 * *Files 26% similar despite different names*

```diff
@@ -23,23 +23,73 @@
 from boax.core.distributions.normal import Normal
 from boax.core.distributions.uniform import Uniform
 from boax.core.samplers import functions
 from boax.core.samplers.base import Sampler
 from boax.utils.functools import compose
 
 
+def uniform(
+  uniform: Uniform = Uniform(jnp.zeros((1,)), jnp.ones((1,))),
+) -> Sampler:
+  """
+  The i.i.d. uniform sampler.
+
+  Example:
+    >>> sampler = uniform()
+    >>> base_samples =  sampler(key, (128,))
+
+  Args:
+    uniform: The base uniform distribution.
+
+  Returns:
+    The corresponding `Sampler`.
+  """
+
+  out_shape = lax.broadcast_shapes(uniform.a.shape, uniform.b.shape)
+
+  return compose(
+    partial(partial, distributions.uniform.sample)(uniform),
+    partial(functions.iid.uniform, ndims=out_shape[0]),
+  )
+
+
+def normal(
+  normal: Normal = Normal(jnp.zeros((1,)), jnp.ones((1,))),
+) -> Sampler:
+  """
+  The i.i.d. normal sampler.
+
+  Example:
+    >>> sampler = normal()
+    >>> base_samples = sampler(key, (128,))
+
+  Args:
+    normal: The base normal distribution.
+
+  Returns:
+    The corresponding `Sampler`.
+  """
+
+  out_shape = lax.broadcast_shapes(normal.loc.shape, normal.scale.shape)
+
+  return compose(
+    partial(partial, distributions.normal.sample)(normal),
+    partial(functions.iid.normal, ndims=out_shape[0]),
+  )
+
+
 def halton_uniform(
   uniform: Uniform = Uniform(jnp.zeros((1,)), jnp.ones((1,))),
 ) -> Sampler:
   """
   The quasi-MC uniform sampler based on halton sequences.
 
   Example:
-    >>> sampler = halton_uniform(uniform)
-    >>> base_samples = sampler(key, 128)
+    >>> sampler = halton_uniform()
+    >>> base_samples = sampler(key, (128,))
 
   Args:
     uniform: The base uniform distribution.
 
   Returns:
     The corresponding `Sampler`.
   """
@@ -62,15 +112,15 @@
 def halton_normal(
   normal: Normal = Normal(jnp.zeros((1,)), jnp.ones((1,))),
 ) -> Sampler:
   """
   The quasi-MC normal sampler based on halton sequences.
 
   Example:
-    >>> sampler = halton_normal(normal)
+    >>> sampler = halton_normal()
     >>> base_samples = sampler(key, 128)
 
   Args:
     normal: The base normal distribution.
 
   Returns:
     The corresponding `Sampler`.
```

### Comparing `boax-0.1.1/boax/core/samplers/base.py` & `boax-0.1.2/boax/optimization/optimizers/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,33 +8,29 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Base interface for samplers."""
+"""Base interface for optimizers."""
 
-from typing import Protocol
+from typing import Protocol, Tuple
 
 from boax.utils.typing import Array, PRNGKey
 
 
-class Sampler(Protocol):
+class Optimizer(Protocol):
   """
-  A callable type for sampling functions.
-
-  A sampler takes a PRNG key and a number of results as input
-  and returns `num_results` samples.
+  A callable type for the optimization functions.
   """
 
-  def __call__(self, key: PRNGKey, num_results: int) -> Array:
+  def __call__(self, key: PRNGKey) -> Tuple[Array, Array]:
     """
-    Draws `num_results` of samples.
+    The optimization function.
 
     Args:
-      key: The pseudo-random number generator key.
-      candidates: The number of results to return.
+      key: A PRNG key.
 
     Returns:
-      A set of `num_results` samples.
+      A tuple of the maxima and their acquisition values.
     """
```

### Comparing `boax-0.1.1/boax/core/samplers/functions/__init__.py` & `boax-0.1.2/boax/optimization/acquisitions/functions/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""The sampler functions sub-package."""
+"""The acquisition functions sub-package."""
 
-from . import quasi_random as quasi_random
-from . import utils as utils
+from . import analytic as analytic
+from . import monte_carlo as monte_carlo
```

### Comparing `boax-0.1.1/boax/core/samplers/functions/quasi_random.py` & `boax-0.1.2/boax/core/samplers/functions/quasi_random.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,28 +10,33 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Quasi Random sampling functions."""
 
+from typing import Sequence
+
 from jax import numpy as jnp
 from jax import random
 
 from boax.core.samplers.functions.utils import primes_less_than
 from boax.utils.typing import Array, PRNGKey
 
 # The maximum dimension we support. This is limited by the number of primes in the PRIMES array.
 MAX_DIMENSION = 10000
 PRIMES = primes_less_than(104729 + 1)
 assert len(PRIMES) == MAX_DIMENSION
 
 
-def halton_sequence(key: PRNGKey, num_samples: int, ndims: int) -> Array:
+def halton_sequence(
+  key: PRNGKey, sample_shape: Sequence[int], ndims: int
+) -> Array:
   shuffle_key, correction_key = random.split(key)
+  num_samples = jnp.prod(jnp.asarray(sample_shape))
 
   radixes = PRIMES[0:ndims][..., jnp.newaxis]
   indices = jnp.reshape(jnp.arange(num_samples) + 1, (-1, 1, 1))
 
   max_sizes_by_axes = jnp.floor(jnp.log(num_samples) / jnp.log(radixes) + 1)
   max_size = jnp.max(max_sizes_by_axes)
 
@@ -44,16 +49,17 @@
 
   coeffs = jnp.floor_divide(indices, weights) * weight_mask % radixes
   shuffled = halton_shuffle(shuffle_key, coeffs, radixes) * weight_mask
 
   base_values = jnp.sum(shuffled / (radixes * weights), axis=-1)
   zero_correction = random.uniform(correction_key, (ndims, 1))
 
-  return (
-    base_values + (zero_correction / (radixes**max_sizes_by_axes)).flatten()
+  return jnp.reshape(
+    base_values + (zero_correction / (radixes**max_sizes_by_axes)).flatten(),
+    sample_shape + (ndims,),
   )
 
 
 def halton_shuffle(key: PRNGKey, coeffs: Array, radixes: Array) -> Array:
   icoeffs = jnp.astype(coeffs, jnp.int32)
   iradixes = jnp.astype(radixes, jnp.int32)
   num_coeffs = coeffs.shape[-1]
```

### Comparing `boax-0.1.1/boax/core/samplers/functions/utils.py` & `boax-0.1.2/boax/core/samplers/functions/utils.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/optimization/__init__.py` & `boax-0.1.2/boax/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/optimization/acquisitions/__init__.py` & `boax-0.1.2/boax/optimization/acquisitions/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,13 +21,16 @@
   log_probability_of_improvement as log_probability_of_improvement,
 )
 from .alias import posterior_mean as posterior_mean
 from .alias import posterior_scale as posterior_scale
 from .alias import probability_of_improvement as probability_of_improvement
 from .alias import q_expected_improvement as q_expected_improvement
 from .alias import q_knowledge_gradient as q_knowledge_gradient
+from .alias import (
+  q_multi_fidelity_knowledge_gradient as q_multi_fidelity_knowledge_gradient,
+)
 from .alias import q_probability_of_improvement as q_probability_of_improvement
 from .alias import q_upper_confidence_bound as q_upper_confidence_bound
 from .alias import upper_confidence_bound as upper_confidence_bound
 from .base import Acquisition as Acquisition
 from .transformed import constrained as constrained
 from .transformed import log_constrained as log_constrained
```

### Comparing `boax-0.1.1/boax/optimization/acquisitions/alias.py` & `boax-0.1.2/boax/optimization/acquisitions/alias.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,24 +12,25 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Alias for acquisition functions."""
 
 import math
 from functools import partial
-from operator import attrgetter
+from operator import attrgetter, itemgetter
+from typing import Callable, Tuple
 
 from jax import jit, lax, scipy
 from jax import numpy as jnp
 
 from boax.core import distributions
 from boax.core.distributions.normal import Normal
 from boax.optimization.acquisitions import functions
 from boax.optimization.acquisitions.base import Acquisition
-from boax.utils.functools import compose
+from boax.utils.functools import apply, compose, unwrap
 from boax.utils.typing import Array, Numeric
 
 
 def probability_of_improvement(
   best: Numeric,
 ) -> Acquisition[Normal]:
   """
@@ -37,15 +38,15 @@
 
   Probability of improvement over the best function value observed so far.
 
   `PI(x) = P(y >= best), y ~ f(x)`
 
   Example:
     >>> acqf = probability_of_improvement(0.2)
-    >>> poi = acqf(model(xs))
+    >>> poi = acqf(vmap(model)(xs))
 
   Args:
     best: The best function value observed so far.
 
   Returns:
     The corresponding `Acquisition`.
   """
@@ -67,15 +68,15 @@
 
   Logarithm of the probability of improvement over the best function value observed so far.
 
   `logPI(x) = log(P(y >= best)), y ~ f(x)`
 
   Example:
     >>> acqf = log_probability_of_improvement(0.2)
-    >>> log_poi = acqf(model(xs))
+    >>> log_poi = acqf(vmap(model)(xs))
 
   Args:
     best: The best function value observed so far.
 
   Returns:
     The corresponding `Acquisition`.
   """
@@ -99,15 +100,15 @@
 
   `EI(x) = E(max(f(x) - best, 0))`,
 
   where the expectation is taken over the value of stochastic function `f` at `x`.
 
   Example:
     >>> acqf = expected_improvement(0.2)
-    >>> ei = acqf(model(xs))
+    >>> ei = acqf(vmap(model)(xs))
 
   Args:
     best: The best function value observed so far.
 
   Returns:
     The corresponding `Acquisition`.
   """
@@ -134,15 +135,15 @@
 
   References:
     Ament, Sebastian, et al. "Unexpected improvements to expected improvement for bayesian optimization."
     arXiv preprint arXiv:2310.20708 (2023).
 
   Example:
     >>> acqf = log_expected_improvement(0.2)
-    >>> log_ei = acqf(model(xs))
+    >>> log_ei = acqf(vmap(model)(xs))
 
   Args:
     best: The best function value observed so far.
 
   Returns:
     The corresponding `Acquisition`.
   """
@@ -164,15 +165,15 @@
   Upper confidence bound comprises of the posterior mean plus an additional term:
   the posterior standard deviation weighted by a trade-off parameter, `beta`.
 
   `UCB(x) = loc(x) + sqrt(beta) * scale(x)`
 
   Example:
     >>> acqf = upper_confidence_bound(2.0)
-    >>> ucb = acqf(model(xs))
+    >>> ucb = acqf(vmap(model)(xs))
 
   Args:
     beta: The mean and covariance trade-off parameter.
 
   Returns:
     The corresponding `Acquisition`.
   """
@@ -187,15 +188,15 @@
 
 def posterior_mean() -> Acquisition:
   """
   The Posterior mean acquisition function.
 
   Example:
     >>> acqf = posterior_mean()
-    >>> mean = acqf(model(xs))
+    >>> mean = acqf(vmap(model)(xs))
 
   Args:
     model: A gaussian process regression surrogate model.
 
   Returns:
     The corresponding `Acquisition`.
   """
@@ -210,15 +211,15 @@
 
 def posterior_scale() -> Acquisition:
   """
   The Posterior scale acquisition function.
 
   Example:
     >>> acqf = posterior_scale()
-    >>> scale = acqf(model(xs))
+    >>> scale = acqf(vmap(model)(xs))
 
   Args:
     model: A gaussian process regression surrogate model.
 
   Returns:
     The corresponding `Acquisition`.
   """
@@ -244,27 +245,27 @@
   to support auto-differentiation, the indicator is replaced with a sigmoid
   function with temperature parameter tau.
 
   `qPI(x) = P(max y >= best), y ~ f(x), x = (x_1,...,x_q)`
 
   Example:
     >>> acqf = q_probability_of_improvement(1.0, 0.2)
-    >>> qpoi = acqf(model(xs))
+    >>> qpoi = acqf(vmap(model)(xs))
 
   Args:
     tau: The temperature parameter.
     best: The best function value observed so far.
 
   Returns:
     The corresponding `Acquisition`.
   """
 
   return jit(
     compose(
-      partial(jnp.mean, axis=-1),
+      partial(jnp.mean, axis=0),
       partial(jnp.amax, axis=-1),
       partial(functions.monte_carlo.qpoi, best=best, tau=tau),
     )
   )
 
 
 def q_expected_improvement(
@@ -277,26 +278,26 @@
   (2) evaluating the improvement over the current best for each sample
   (3) maximizing over q (4) averaging over the samples.
 
   `qEI(x) = E(max(max y - best, 0)), y ~ f(x), x = (x_1,...,x_q)`
 
   Example:
     >>> acqf = q_expected_improvement(0.2)
-    >>> qei = acqf(model(xs))
+    >>> qei = acqf(vmap(model)(xs))
 
   Args:
     best: The best function value observed so far.
 
   Returns:
     The corresponding `Acquisition`.
   """
 
   return jit(
     compose(
-      partial(jnp.mean, axis=-1),
+      partial(jnp.mean, axis=0),
       partial(jnp.amax, axis=-1),
       partial(functions.monte_carlo.qei, best=best),
     )
   )
 
 
 def q_upper_confidence_bound(
@@ -307,52 +308,87 @@
 
   `qUCB = E(max(mean + |y_tilde - mean|))`,
 
   where `y_tilde ~ N(mean(x), beta * pi/2 * cov(x))` and `f(x) ~ N(mean(x), cov(x)).`
 
   Example:
     >>> acqf = q_upper_confidence_bound(2.0)
-    >>> qucb = acqf(model(xs))
+    >>> qucb = acqf(vmap(model)(xs))
 
   Args:
     beta: The mean and covariance trade-off parameter.
 
   Returns:
     The corresponding `Acquisition`.
   """
 
   beta_prime = lax.sqrt(beta * math.pi / 2)
 
   return jit(
     compose(
-      partial(jnp.mean, axis=-1),
+      partial(jnp.mean, axis=0),
       partial(jnp.amax, axis=-1),
       partial(functions.monte_carlo.qucb, beta=beta_prime),
     )
   )
 
 
 def q_knowledge_gradient(
   best: Numeric,
 ) -> Acquisition[Normal]:
   """
   MC-based batch Knowledge Gradient acquisition function.
 
   Example:
     >>> acqf = q_knowledge_gradient(0.2)
-    >>> qucb = acqf(model(xs))
+    >>> qkg = acqf(vmap(model)(xs))
 
   Args:
     best: The best function value observed so far.
 
   Returns:
     The corresponding `Acquisition`.
   """
 
   return jit(
     compose(
-      partial(jnp.mean, axis=-1),
+      partial(jnp.mean, axis=0),
       partial(jnp.squeeze, axis=-1),
       partial(lax.sub, y=best),
       attrgetter('loc'),
     )
   )
+
+
+def q_multi_fidelity_knowledge_gradient(
+  best: Numeric,
+  cost_fn: Callable,
+) -> Acquisition[Tuple[Normal, Array]]:
+  """
+  MC-based batch multi-fidelity Knowledge Gradient acquisition function.
+
+  Example:
+    >>> acqf = q_knowledge_gradient(0.2, cost_fn)
+    >>> qmfkg = acqf(vmap(model)(xs))
+
+  Args:
+    best: The best function value observed so far.
+
+  Returns:
+    The corresponding `Acquisition`.
+  """
+
+  return jit(
+    compose(
+      partial(jnp.mean, axis=0),
+      apply(
+        unwrap(cost_fn),
+        compose(
+          partial(jnp.squeeze, axis=-1),
+          partial(lax.sub, y=best),
+          attrgetter('loc'),
+          itemgetter(0),
+        ),
+        itemgetter(1),
+      ),
+    )
+  )
```

### Comparing `boax-0.1.1/boax/optimization/acquisitions/base.py` & `boax-0.1.2/boax/optimization/acquisitions/base.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/optimization/acquisitions/constraints/__init__.py` & `boax-0.1.2/boax/optimization/acquisitions/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/optimization/acquisitions/constraints/alias.py` & `boax-0.1.2/boax/optimization/acquisitions/constraints/alias.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/optimization/acquisitions/constraints/base.py` & `boax-0.1.2/boax/optimization/acquisitions/constraints/base.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/optimization/acquisitions/functions/__init__.py` & `boax-0.1.2/boax/prediction/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""The acquisition functions sub-package."""
+"""The prediction module."""
 
-from . import analytic as analytic
-from . import monte_carlo as monte_carlo
+from . import models as models
+from . import objectives as objectives
```

### Comparing `boax-0.1.1/boax/optimization/acquisitions/functions/analytic.py` & `boax-0.1.2/boax/optimization/acquisitions/functions/analytic.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/optimization/acquisitions/functions/monte_carlo.py` & `boax-0.1.2/boax/optimization/acquisitions/functions/monte_carlo.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/optimization/acquisitions/transformed.py` & `boax-0.1.2/boax/optimization/acquisitions/transformed.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/optimization/optimizers/__init__.py` & `boax-0.1.2/boax/utils/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""The optimizers sub-package."""
+"""The optimization module."""
 
-from .alias import bfgs as bfgs
-from .base import Optimizer as Optimizer
+from . import functools as functools
+from . import typing as typing
```

### Comparing `boax-0.1.1/boax/optimization/optimizers/alias.py` & `boax-0.1.2/boax/optimization/optimizers/alias.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,55 +8,69 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Alias for acquisition function maximizers."""
+"""Alias for optimizers."""
 
-from functools import partial
-from typing import Callable
+from jax import numpy as jnp
+from jax import random
 
-from boax.optimization.optimizers import functions
 from boax.optimization.optimizers.base import Optimizer
-from boax.utils.typing import Array
+from boax.optimization.optimizers.initializers.base import Initializer
+from boax.optimization.optimizers.solvers.base import Solver
 
 
-def bfgs(
-  fn: Callable[[Array], Array],
-  bounds: Array,
-  x0: Array,
-  num_samples: int,
-) -> Optimizer:
+def batch(initializer: Initializer, solver: Solver) -> Optimizer:
   """
-  The BFGS acquisition function optimizer.
+  Batch optimizer.
 
   Example:
-    >>> optimizer = bfgs(fn, bounds, x0, num_samples)
-    >>> candidates = optimizer.init(key)
-    >>> next_candidates, values = optimizer(candidates)
+    >>> optimizer = batch(initializer, solver)
+    >>> next_candidates = optimizer(key)
 
   Args:
-    fn: The function to be optimized.
-    bounds: The bounds of the search space.
-    x0: The index points to consider.
-    num_samples: The number of sampled candidates.
+    initializer: The initializer function.
+    solver: The solver function.
 
   Returns:
-    The corresponding `Optimizer`.
+    The batch `Optimizer`.
   """
 
-  return Optimizer(
-    partial(
-      functions.initialization.q_batch,
-      fn=fn,
-      x0=x0,
-      num_samples=num_samples,
-    ),
-    partial(
-      functions.scipy.maximize,
-      fn=fn,
-      bounds=bounds,
-      method='bfgs',
-    ),
-  )
+  def optimizer(key):
+    candidates = initializer(key)
+    next_candidates, values = solver(candidates)
+    idx = jnp.argmax(values)
+
+    return next_candidates[idx], values[idx]
+
+  return optimizer
+
+
+def sequential(initializer: Initializer, solver: Solver, q: int) -> Optimizer:
+  """
+  Sequential optimizer.
+
+  Example:
+    >>> optimizer = sequential(initializer, solver)
+    >>> next_candidates = optimizer(key, fun, bounds, q, num_samples, num_restarts)
+
+  Args:
+    initializer: The initializer function.
+    solver: The solver function.
+
+  Returns:
+    The sequential `Optimizer`.
+  """
+
+  inner = batch(initializer, solver)
+
+  def optimizer(key):
+    next_candidates, values = zip(
+      *(inner(random.fold_in(key, i)) for i in range(q))
+    )
+
+    return (jnp.concatenate(list(next_candidates)), jnp.array(list(values)))
+
+  return optimizer
```

### Comparing `boax-0.1.1/boax/optimization/optimizers/functions/__init__.py` & `boax-0.1.2/boax/core/samplers/functions/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,11 +8,12 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""The maximizer functions sub-package."""
+"""The sampler functions sub-package."""
 
-from . import initialization as initialization
-from . import scipy as scipy
+from . import iid as iid
+from . import quasi_random as quasi_random
+from . import utils as utils
```

### Comparing `boax-0.1.1/boax/optimization/optimizers/functions/initialization.py` & `boax-0.1.2/boax/prediction/models/kernels/functions/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,30 +8,13 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Initializes candidates."""
+"""The kernel functions sub-package."""
 
-from typing import Callable
-
-from jax import nn, random
-from jax import numpy as jnp
-
-from boax.utils.typing import Array, Numeric, PRNGKey
-
-
-def q_batch(
-  key: PRNGKey,
-  fn: Callable[[Array], Array],
-  x0: Array,
-  num_samples: int,
-  eta: Numeric = 1.0,
-) -> Array:
-  return random.choice(
-    key,
-    x0,
-    (num_samples,),
-    p=jnp.exp(eta * nn.standardize(fn(x0), axis=0)),
-  )
+from . import matern as matern
+from . import periodic as periodic
+from . import rbf as rbf
+from . import utils as utils
```

### Comparing `boax-0.1.1/boax/optimization/optimizers/functions/scipy.py` & `boax-0.1.2/boax/optimization/optimizers/solvers/alias.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,43 +8,61 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""The scipy maximization functions."""
+"""Alias for solver functions."""
 
 from functools import partial
-from typing import Callable, Tuple
+from typing import Callable
 
 from jax import numpy as jnp
 from jax.scipy import optimize
 
+from boax.optimization.optimizers.solvers.base import Solver
 from boax.utils.functools import compose
 from boax.utils.typing import Array
 
 
-def maximize(
-  candidates: Array,
-  fn: Callable[[Array], Array],
+def scipy(
+  fun: Callable[[Array], Array],
   bounds: Array,
-  method: str,
-) -> Tuple[Array, Array]:
-  results = optimize.minimize(
-    fun=compose(
-      jnp.negative,
-      jnp.sum,
-      fn,
-      partial(jnp.reshape, newshape=candidates.shape),
-    ),
-    x0=candidates.flatten(),
-    method=method,
-  )
-
-  clipped = jnp.clip(
-    jnp.reshape(results.x, candidates.shape),
-    a_min=bounds[:, 0],
-    a_max=bounds[:, 1],
-  )
+  method: str = 'bfgs',
+) -> Solver:
+  """
+  Scipy solver.
+
+  Example:
+    >>> solver = scipy(fun, bounds)
+    >>> next_candidates, values = solver(candidates)
+
+  Args:
+    bounds: The bounds of the search space.
+    method: The solver method.
+
+  Returns:
+    The scipy `Solver`.
+  """
+
+  def solver(candidates):
+    results = optimize.minimize(
+      fun=compose(
+        jnp.negative,
+        jnp.sum,
+        fun,
+        partial(jnp.reshape, newshape=candidates.shape),
+      ),
+      x0=candidates.flatten(),
+      method=method,
+    )
+
+    clipped = jnp.clip(
+      jnp.reshape(results.x, candidates.shape),
+      a_min=bounds[:, 0],
+      a_max=bounds[:, 1],
+    )
 
-  return clipped, fn(clipped)
+    return clipped, fun(clipped)
+
+  return solver
```

### Comparing `boax-0.1.1/boax/prediction/__init__.py` & `boax-0.1.2/boax/prediction/objectives/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,11 +8,12 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""The prediction module."""
+"""The objectives sub-package."""
 
-from . import models as models
-from . import objectives as objectives
+from .alias import negative_log_likelihood as negative_log_likelihood
+from .base import Objective as Objective
+from .transformed import penalized as penalized
```

### Comparing `boax-0.1.1/boax/prediction/models/__init__.py` & `boax-0.1.2/boax/prediction/models/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,18 +10,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """The models sub-package."""
 
+from . import gaussian_process as gaussian_process
 from . import kernels as kernels
 from . import likelihoods as likelihoods
 from . import means as means
-from .alias import gaussian_process as gaussian_process
-from .alias import multi_fidelity as multi_fidelity
 from .base import Model as Model
 from .transformed import input_transformed as input_transformed
 from .transformed import joined as joined
 from .transformed import outcome_transformed as outcome_transformed
 from .transformed import sampled as sampled
 from .transformed import scaled as scaled
```

### Comparing `boax-0.1.1/boax/prediction/models/alias.py` & `boax-0.1.2/boax/prediction/models/gaussian_process.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,43 +8,44 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Alias for surrogate models."""
+"""Gaussian for surrogate models."""
 
 from functools import partial
 from typing import Callable, TypeVar
 
-from jax import jit
+from jax import jit, vmap
+from jax import numpy as jnp
 
 from boax.core.distributions.multivariate_normal import MultivariateNormal
 from boax.prediction.models import functions
 from boax.prediction.models.base import Model
 from boax.prediction.models.kernels.base import Kernel
 from boax.prediction.models.likelihoods.base import Likelihood
 from boax.prediction.models.means.base import Mean
 from boax.utils.functools import compose
 from boax.utils.typing import Array, Numeric
 
 T = TypeVar('T')
 
 
-def gaussian_process(
+def exact(
   mean_fn: Mean,
   kernel_fn: Kernel,
   likelihood_fn: Likelihood[MultivariateNormal, T],
   observation_index_points: Array | None = None,
   observations: Array | None = None,
   jitter: Numeric = 1e-6,
 ) -> Model[T]:
   """
-  The gaussian process model.
+  The exact gaussian process model.
 
   Example:
     >>> model = gaussian_process(mean_fn, kernel_fn)
     >>> mean, cov = model(xs)
 
   Args:
     mean_fn: The process' mean function.
@@ -82,41 +83,67 @@
           kernel_fn=kernel_fn,
           jitter=jitter,
         ),
       )
     )
 
 
+def fantasy(
+  mean_fn: Mean,
+  kernel_fn: Kernel,
+  jitter: Numeric = 1e-6,
+) -> Callable[[Array, Array, Array], MultivariateNormal]:
+  return vmap(
+    vmap(
+      jit(
+        partial(
+          functions.gaussian.posterior,
+          mean_fn=mean_fn,
+          kernel_fn=kernel_fn,
+          jitter=jitter,
+        )
+      ),
+      in_axes=(0, None, 0),
+    )
+  )
+
+
 def multi_fidelity(
   mean_fn: Mean,
   kernel_fn: Callable[[Array, Array], Kernel],
   likelihood_fn: Likelihood[MultivariateNormal, T],
   observation_index_points: Array | None = None,
+  observation_fidelities: Array | None = None,
   observations: Array | None = None,
   jitter: Numeric = 1e-6,
 ) -> Model[T]:
   """
   The multi fidelity gaussian process model.
 
   Example:
     >>> model = multi_fidelity(mean_fn, kernel_fn, 1e-4)
     >>> mean, cov = model(x_train, y_train)(xs)
 
   Args:
     mean_fn: The process' mean function.
     kernel_fn: The process' covariance function.
     observation_index_points: The index points of the given observations.
+    observation_fidelities: The fidelities of the given observatons.
     observations: The observed values.
     jitter: The scalar added to the diagonal of the covariance matrix to ensure positive definiteness.
 
   Returns:
     The multi fidelity gaussian process `Model`.
   """
 
-  if observation_index_points is None or observations is None:
+  if (
+    observation_index_points is None
+    or observation_fidelities is None
+    or observations is None
+  ):
     return jit(
       compose(
         likelihood_fn,
         partial(
           functions.multi_fidelity.prior,
           mean_fn=mean_fn,
           kernel_fn=kernel_fn,
@@ -128,14 +155,51 @@
   else:
     return jit(
       compose(
         likelihood_fn,
         partial(
           functions.multi_fidelity.posterior,
           observation_index_points=observation_index_points,
+          observation_fidelities=observation_fidelities,
           observations=observations,
           mean_fn=mean_fn,
           kernel_fn=kernel_fn,
           jitter=jitter,
         ),
       )
     )
+
+
+def multi_fidelity_fantasy(
+  mean_fn: Mean,
+  kernel_fn: Callable[[Array, Array], Kernel],
+  jitter: Numeric = 1e-6,
+) -> Callable[[Array, Array, Array], MultivariateNormal]:
+  fantasy_fn = vmap(
+    vmap(
+      jit(
+        partial(
+          functions.multi_fidelity.posterior,
+          mean_fn=mean_fn,
+          kernel_fn=kernel_fn,
+          jitter=jitter,
+        )
+      ),
+      in_axes=(0, 0, None, None, 0),
+    )
+  )
+
+  def fn(
+    fantasy_points,
+    observation_index_points,
+    observation_fidelities,
+    observations,
+  ):
+    return fantasy_fn(
+      fantasy_points,
+      jnp.ones_like(fantasy_points),
+      observation_index_points,
+      observation_fidelities,
+      observations,
+    )
+
+  return fn
```

### Comparing `boax-0.1.1/boax/prediction/models/base.py` & `boax-0.1.2/boax/prediction/models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
   """
   A callable type for surrogate models.
 
   A model takes a set of `n x d`-dim index points as input
   and returns a posterior prediction of type `T`.
   """
 
-  def __call__(self, index_points: Array) -> T:
+  def __call__(self, index_points: Array, **kwargs) -> T:
     """
     Computes the posterior prediction at the index points.
 
     Args:
       index_points: The `n x d` index points.
 
     Returns:
```

### Comparing `boax-0.1.1/boax/prediction/models/functions/__init__.py` & `boax-0.1.2/boax/prediction/models/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/prediction/models/functions/gaussian.py` & `boax-0.1.2/boax/prediction/models/functions/gaussian.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/prediction/models/functions/multi_fidelity.py` & `boax-0.1.2/boax/prediction/models/functions/multi_fidelity.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,62 +10,62 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Multi fidelity functions."""
 
-from typing import Callable, Tuple
+from typing import Callable
 
 from jax import numpy as jnp
 from jax import scipy
 
 from boax.core import distributions
 from boax.core.distributions.multivariate_normal import MultivariateNormal
 from boax.prediction.models.kernels.base import Kernel
 from boax.prediction.models.means.base import Mean
 from boax.utils.typing import Array, Numeric
 
 
-def split(values: Array) -> Tuple[Array, Array]:
-  return jnp.split(values, [values.shape[-1] - 1], axis=-1)
-
-
 def prior(
   index_points: Array,
+  fidelities: Array,
   mean_fn: Mean,
   kernel_fn: Callable[[Array, Array], Kernel],
   jitter: Numeric,
 ) -> MultivariateNormal:
-  values, fidelities = split(index_points)
-
-  Kxx = kernel_fn(fidelities, fidelities)(values, values)
-  mean = mean_fn(values)
+  Kxx = kernel_fn(fidelities, fidelities)(index_points, index_points)
+  mean = mean_fn(index_points)
   cov = Kxx + jitter * jnp.identity(Kxx.shape[-1])
 
   return distributions.multivariate_normal.multivariate_normal(mean, cov)
 
 
 def posterior(
   index_points: Array,
+  fidelities: Array,
   observation_index_points: Array,
+  observation_fidelities: Array,
   observations: Array,
   mean_fn: Mean,
   kernel_fn: Callable[[Array, Array], Kernel],
   jitter: Numeric,
 ) -> MultivariateNormal:
-  ivalues, ifidelities = split(index_points)
-  ovalues, ofidelities = split(observation_index_points)
+  mz = mean_fn(index_points)
+  mx = mean_fn(observation_index_points)
 
-  mz = mean_fn(ivalues)
-  mx = mean_fn(ovalues)
+  Kxx = kernel_fn(observation_fidelities, observation_fidelities)(
+    observation_index_points, observation_index_points
+  )
+
+  Kxz = kernel_fn(observation_fidelities, fidelities)(
+    observation_index_points, index_points
+  )
 
-  Kxx = kernel_fn(ofidelities, ofidelities)(ovalues, ovalues)
-  Kxz = kernel_fn(ofidelities, ifidelities)(ovalues, ivalues)
-  Kzz = kernel_fn(ifidelities, ifidelities)(ivalues, ivalues)
+  Kzz = kernel_fn(fidelities, fidelities)(index_points, index_points)
 
   K = Kxx + jitter * jnp.identity(Kxx.shape[-1])
   chol = scipy.linalg.cholesky(K, lower=True)
   kinvy = scipy.linalg.solve_triangular(
     chol.T, scipy.linalg.solve_triangular(chol, observations - mx, lower=True)
   )
   v = scipy.linalg.solve_triangular(chol, Kxz, lower=True)
```

### Comparing `boax-0.1.1/boax/prediction/models/kernels/__init__.py` & `boax-0.1.2/boax/prediction/models/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/prediction/models/kernels/alias.py` & `boax-0.1.2/boax/prediction/models/kernels/alias.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/prediction/models/kernels/base.py` & `boax-0.1.2/boax/prediction/models/kernels/base.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/prediction/models/kernels/functions/distance.py` & `boax-0.1.2/boax/prediction/models/kernels/functions/distance.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/prediction/models/kernels/functions/matern.py` & `boax-0.1.2/boax/prediction/models/kernels/functions/matern.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/prediction/models/kernels/functions/periodic.py` & `boax-0.1.2/boax/prediction/models/kernels/functions/periodic.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/prediction/models/kernels/functions/rbf.py` & `boax-0.1.2/boax/prediction/models/kernels/functions/rbf.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/prediction/models/kernels/functions/utils.py` & `boax-0.1.2/boax/prediction/models/kernels/functions/utils.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/prediction/models/kernels/transformed.py` & `boax-0.1.2/boax/prediction/models/kernels/transformed.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/prediction/models/likelihoods/__init__.py` & `boax-0.1.2/boax/prediction/models/likelihoods/__init__.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/prediction/models/likelihoods/alias.py` & `boax-0.1.2/boax/prediction/models/likelihoods/alias.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/prediction/models/likelihoods/base.py` & `boax-0.1.2/boax/prediction/models/likelihoods/base.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/prediction/models/likelihoods/functions/__init__.py` & `boax-0.1.2/boax/optimization/optimizers/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,11 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""The likelihood functions sub-package."""
+"""The optimizers sub-package."""
 
-from . import conditional as conditional
-from . import marginal as marginal
+from . import initializers as initializers
+from . import solvers as solvers
+from .alias import batch as batch
+from .alias import sequential as sequential
+from .base import Optimizer as Optimizer
```

### Comparing `boax-0.1.1/boax/prediction/models/likelihoods/functions/conditional.py` & `boax-0.1.2/boax/prediction/models/likelihoods/functions/conditional.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/prediction/models/likelihoods/functions/marginal.py` & `boax-0.1.2/boax/prediction/models/likelihoods/functions/marginal.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/prediction/models/means/__init__.py` & `boax-0.1.2/boax/prediction/models/means/__init__.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/prediction/models/means/alias.py` & `boax-0.1.2/boax/prediction/models/means/alias.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/prediction/models/means/base.py` & `boax-0.1.2/boax/prediction/models/means/base.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/prediction/models/transformed.py` & `boax-0.1.2/boax/prediction/models/transformed.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,45 +11,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Transformation functions for models."""
 
 from functools import partial
-from typing import Callable, Sequence, TypeVar
+from typing import Any, Callable, Sequence, TypeVar
 
 from jax import vmap
 
 from boax.prediction.models.base import Model
 from boax.utils.functools import apply, call, compose
 from boax.utils.typing import Array
 
 A = TypeVar('A')
 B = TypeVar('B')
 T = TypeVar('T')
 
 
-def joined(*models: Model[T]) -> Model[Sequence[T]]:
-  """
-  Constructs a joined model.
-
-  Example:
-    >>> transformed = joined(objective_model, cost_model)
-    >>> objective_result, cost_result = transformed(xs)
-
-  Args:
-    models: The models to be joined.
-
-  Returns:
-    The transformed `Model` function.
-  """
-
-  return apply(tuple, *models)
-
-
 def outcome_transformed(
   model: Model[A],
   *transformation_fns: Callable[[A], B],
 ) -> Model[B]:
   """
   Constructs an outcome transformed model.
 
@@ -92,14 +74,32 @@
 
   return compose(
     model,
     *reversed(transformation_fns),
   )
 
 
+def joined(*models: Model[Any]) -> Model[Sequence[Any]]:
+  """
+  Constructs a joined model.
+
+  Example:
+    >>> transformed = joined(objective_model, cost_model)
+    >>> objective_result, cost_result = transformed(xs)
+
+  Args:
+    models: The models to be joined.
+
+  Returns:
+    The transformed `Model` function.
+  """
+
+  return apply(tuple, *models)
+
+
 def scaled(
   model: Model[T],
   scale_fn: Callable[[T, Array, Array], T],
   loc: Array,
   scale: Array,
 ) -> Model[T]:
   """
```

### Comparing `boax-0.1.1/boax/prediction/objectives/__init__.py` & `boax-0.1.2/boax/optimization/optimizers/solvers/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,12 +8,11 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""The objectives sub-package."""
+"""The initializers sub-package."""
 
-from .alias import negative_log_likelihood as negative_log_likelihood
-from .base import Objective as Objective
-from .transformed import penalized as penalized
+from .alias import scipy as scipy
+from .base import Solver as Solver
```

### Comparing `boax-0.1.1/boax/prediction/objectives/alias.py` & `boax-0.1.2/boax/prediction/objectives/alias.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/prediction/objectives/base.py` & `boax-0.1.2/boax/prediction/objectives/base.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/prediction/objectives/transformed.py` & `boax-0.1.2/boax/prediction/objectives/transformed.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/utils/__init__.py` & `boax-0.1.2/boax/optimization/optimizers/initializers/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,11 +8,12 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""The optimization module."""
+"""The initializers sub-package."""
 
-from . import functools as functools
-from . import typing as typing
+from .alias import q_batch as q_batch
+from .alias import q_batch_nonnegative as q_batch_nonnegative
+from .base import Initializer as Initializer
```

### Comparing `boax-0.1.1/boax/utils/functools.py` & `boax-0.1.2/boax/utils/functools.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/utils/typing.py` & `boax-0.1.2/boax/utils/typing.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.1/boax/version.py` & `boax-0.1.2/boax/version.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 """Current boax version at head on GitHub"""
 
-__version__ = '0.1.1'
+__version__ = '0.1.2'
```

### Comparing `boax-0.1.1/boax.egg-info/PKG-INFO` & `boax-0.1.2/boax.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boax
-Version: 0.1.1
+Version: 0.1.2
 Summary: Boax is a Bayesian Optimization library for JAX.
 Project-URL: homepage, https://github.com/Lando-L/boax
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.11
@@ -46,22 +46,18 @@
 
 Boax is a composable library of core components for Bayesian Optimization that is **designed for flexibility**. It comes with low-level interfaces for:
 
 * **Core capabilities** (`boax.core`):
   * Common Distributions
   * Monte-Carlo Samplers
 * **Fitting a surrogate model to data** (`boax.prediction`):
-  * Kernels Functions
-  * Likelihood Functions
-  * Mean Functions
   * Model Functions
   * Objective Functions
 * **Constructing and optimizing acquisition functions** (`boax.optimization`):
   * Acquisition Functions
-  * Constraint Functions
   * Optimizer Functions
 
 ## Installation
 
 You can install the latest released version of Boax from PyPI via:
 
 ```sh
@@ -72,70 +68,82 @@
 
 ```sh
 pip install git+https://github.com/Lando-L/boax.git
 ```
 
 ## Basic Usage
 
-Here is a basic example of using the Boax API for defining a Gaussian Process model, constructing an Acquisition function, and combining the two for optimzation. For more details check out the [docs](https://boax.readthedocs.io/en/latest/).
+Here is a basic example of using the Boax API for defining a Gaussian Process model, constructing an Acquisition function, and generating the next batch of data points to query. For more details check out the [docs](https://boax.readthedocs.io/en/latest/).
 
 1. Defining a Gaussian Process model:
 
 ```python
 from boax.prediction import models
 
-model = models.gaussian_process(
+model = models.gaussian_process.exact(
   models.means.zero(),
   models.kernels.scaled(
-    models.kernels.rbf(1.0),
-    0.5
+    models.kernels.rbf(1.0), 0.5
   ),
   models.likelihoods.gaussian(1e-4),
   x_train,
   y_train,
 )
 ```
 
 2. Constructing an Acquisition function.
 
 ```python
+from jax import vmap
 from boax.optimization import acquisitions
 
-acquisition = acquisitions.upper_confidence_bound(
-  beta=2.0
+acqf = models.outcome_transformed(
+  vmap(model),
+  acquisitions.upper_confidence_bound(2.0)
 )
 ```
 
-3. Combining the two for optimization
+3. Generating the next batch of data points to query.
 
 ```python
-from jax import jit, random, vmap
 from jax import numpy as jnp
+from jax import random
+from boax.core import distributions, samplers
 from boax.optimization import optimizers
 
-def acqf(x):
-  return acquisition(vmap(model)(x))
+key = random.key(0)
 
-key1, key2 = random.split(random.key(0))
+batch_size, num_results, num_restarts = 1, 100, 10
 bounds = jnp.array([[-1.0, 1.0]])
-x0 = random.uniform(key1, shape=(100, 1, 1))
-bfgs = optimizers.bfgs(jit(acqf), bounds, x0, 10)
-candidates = bfgs.init(key2)
-next_candidates, values = bfgs.update(candidates)
+
+sampler = samplers.halton_uniform(
+  distributions.uniform.uniform(bounds[:, 0], bounds[:, 1])
+)
+
+optimizer = optimizers.batch(
+  optimizers.initializers.q_batch(
+    acqf, sampler, batch_size, num_results, num_restarts,
+  ),
+  optimizers.solvers.scipy(
+    acqf, bounds,  
+  ),
+)
+
+next_x, value = optimizer(key)
 ```
 
 ## Citing Boax
 
 To cite Boax please use the citation:
 
 ```bibtex
 @software{boax2023github,
   author = {Lando L{\"o}per},
   title = {{B}oax: A Bayesian Optimization library for {JAX}},
   url = {https://github.com/Lando-L/boax},
-  version = {0.1.1},
+  version = {0.1.2},
   year = {2023},
 }
 ```
 
 In the above bibtex entry, the version number
 is intended to be that from [boax/version.py](https://github.com/Lando-L/boax/blob/main/boax/version.py), and the year corresponds to the project's open-source release.
```

### Comparing `boax-0.1.1/boax.egg-info/SOURCES.txt` & `boax-0.1.2/boax.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 boax/core/distributions/poisson.py
 boax/core/distributions/transformed.py
 boax/core/distributions/uniform.py
 boax/core/samplers/__init__.py
 boax/core/samplers/alias.py
 boax/core/samplers/base.py
 boax/core/samplers/functions/__init__.py
+boax/core/samplers/functions/iid.py
 boax/core/samplers/functions/quasi_random.py
 boax/core/samplers/functions/utils.py
 boax/optimization/__init__.py
 boax/optimization/acquisitions/__init__.py
 boax/optimization/acquisitions/alias.py
 boax/optimization/acquisitions/base.py
 boax/optimization/acquisitions/transformed.py
@@ -33,21 +34,24 @@
 boax/optimization/acquisitions/constraints/base.py
 boax/optimization/acquisitions/functions/__init__.py
 boax/optimization/acquisitions/functions/analytic.py
 boax/optimization/acquisitions/functions/monte_carlo.py
 boax/optimization/optimizers/__init__.py
 boax/optimization/optimizers/alias.py
 boax/optimization/optimizers/base.py
-boax/optimization/optimizers/functions/__init__.py
-boax/optimization/optimizers/functions/initialization.py
-boax/optimization/optimizers/functions/scipy.py
+boax/optimization/optimizers/initializers/__init__.py
+boax/optimization/optimizers/initializers/alias.py
+boax/optimization/optimizers/initializers/base.py
+boax/optimization/optimizers/solvers/__init__.py
+boax/optimization/optimizers/solvers/alias.py
+boax/optimization/optimizers/solvers/base.py
 boax/prediction/__init__.py
 boax/prediction/models/__init__.py
-boax/prediction/models/alias.py
 boax/prediction/models/base.py
+boax/prediction/models/gaussian_process.py
 boax/prediction/models/transformed.py
 boax/prediction/models/functions/__init__.py
 boax/prediction/models/functions/gaussian.py
 boax/prediction/models/functions/multi_fidelity.py
 boax/prediction/models/kernels/__init__.py
 boax/prediction/models/kernels/alias.py
 boax/prediction/models/kernels/base.py
```

### Comparing `boax-0.1.1/pyproject.toml` & `boax-0.1.2/pyproject.toml`

 * *Files identical despite different names*

