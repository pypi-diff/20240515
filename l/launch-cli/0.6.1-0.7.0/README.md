# Comparing `tmp/launch_cli-0.6.1.tar.gz` & `tmp/launch_cli-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "launch_cli-0.6.1.tar", last modified: Fri May  3 18:25:19 2024, max compression
+gzip compressed data, was "launch_cli-0.7.0.tar", last modified: Wed May 15 20:54:36 2024, max compression
```

## Comparing `launch_cli-0.6.1.tar` & `launch_cli-0.7.0.tar`

### file list

```diff
@@ -1,82 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:25:19.304612 launch_cli-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 18:25:07.000000 launch_cli-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19229 2024-05-03 18:25:19.304612 launch_cli-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18217 2024-05-03 18:25:07.000000 launch_cli-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:25:19.300612 launch_cli-0.6.1/launch_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19229 2024-05-03 18:25:19.000000 launch_cli-0.6.1/launch_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-03 18:25:19.000000 launch_cli-0.6.1/launch_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 18:25:19.000000 launch_cli-0.6.1/launch_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-03 18:25:19.000000 launch_cli-0.6.1/launch_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-03 18:25:19.000000 launch_cli-0.6.1/launch_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-03 18:25:19.000000 launch_cli-0.6.1/launch_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-03 18:25:07.000000 launch_cli-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 18:25:19.304612 launch_cli-0.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:25:19.292612 launch_cli-0.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:25:19.296612 launch_cli-0.6.1/src/launch/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:25:19.296612 launch_cli-0.6.1/src/launch/automation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/automation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:25:19.296612 launch_cli-0.6.1/src/launch/automation/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/automation/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13217 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/automation/common/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:25:19.296612 launch_cli-0.6.1/src/launch/automation/helm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/automation/helm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/automation/helm/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:25:19.296612 launch_cli-0.6.1/src/launch/automation/provider/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/automation/provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:25:19.296612 launch_cli-0.6.1/src/launch/automation/provider/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/automation/provider/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/automation/provider/aws/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:25:19.296612 launch_cli-0.6.1/src/launch/automation/provider/az/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/automation/provider/az/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/automation/provider/az/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:25:19.296612 launch_cli-0.6.1/src/launch/automation/terragrunt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/automation/terragrunt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/automation/terragrunt/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:25:19.296612 launch_cli-0.6.1/src/launch/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/cli/entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:25:19.296612 launch_cli-0.6.1/src/launch/cli/github/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/cli/github/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:25:19.296612 launch_cli-0.6.1/src/launch/cli/github/access/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/cli/github/access/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/cli/github/access/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:25:19.296612 launch_cli-0.6.1/src/launch/cli/github/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/cli/github/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/cli/github/hooks/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:25:19.300612 launch_cli-0.6.1/src/launch/cli/github/repo/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/cli/github/repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/cli/github/repo/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:25:19.300612 launch_cli-0.6.1/src/launch/cli/github/version/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/cli/github/version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/cli/github/version/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:25:19.300612 launch_cli-0.6.1/src/launch/cli/helm/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/cli/helm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/cli/helm/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:25:19.300612 launch_cli-0.6.1/src/launch/cli/service/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/cli/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15496 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/cli/service/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:25:19.300612 launch_cli-0.6.1/src/launch/cli/terragrunt/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/cli/terragrunt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14502 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/cli/terragrunt/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:25:19.300612 launch_cli-0.6.1/src/launch/cli/validate/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/cli/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/cli/validate/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:25:19.300612 launch_cli-0.6.1/src/launch/github/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/github/access.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/github/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/github/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/github/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/github/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:25:19.300612 launch_cli-0.6.1/src/launch/local_repo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/local_repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/local_repo/branch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/local_repo/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/local_repo/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/local_repo/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:25:19.300612 launch_cli-0.6.1/src/launch/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/service/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-03 18:25:07.000000 launch_cli-0.6.1/src/launch/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:54:36.791665 launch_cli-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-15 20:54:23.000000 launch_cli-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19229 2024-05-15 20:54:36.791665 launch_cli-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18217 2024-05-15 20:54:23.000000 launch_cli-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:54:36.787665 launch_cli-0.7.0/launch_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19229 2024-05-15 20:54:36.000000 launch_cli-0.7.0/launch_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-15 20:54:36.000000 launch_cli-0.7.0/launch_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 20:54:36.000000 launch_cli-0.7.0/launch_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-15 20:54:36.000000 launch_cli-0.7.0/launch_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-15 20:54:36.000000 launch_cli-0.7.0/launch_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 20:54:36.000000 launch_cli-0.7.0/launch_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-15 20:54:23.000000 launch_cli-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 20:54:36.791665 launch_cli-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:54:36.775665 launch_cli-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:54:36.779665 launch_cli-0.7.0/src/launch/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:54:36.779665 launch_cli-0.7.0/src/launch/automation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/automation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:54:36.783665 launch_cli-0.7.0/src/launch/automation/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/automation/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13217 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/automation/common/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:54:36.783665 launch_cli-0.7.0/src/launch/automation/helm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/automation/helm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/automation/helm/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:54:36.783665 launch_cli-0.7.0/src/launch/automation/provider/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/automation/provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:54:36.783665 launch_cli-0.7.0/src/launch/automation/provider/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/automation/provider/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/automation/provider/aws/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:54:36.783665 launch_cli-0.7.0/src/launch/automation/provider/az/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/automation/provider/az/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/automation/provider/az/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:54:36.783665 launch_cli-0.7.0/src/launch/automation/terragrunt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/automation/terragrunt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/automation/terragrunt/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:54:36.783665 launch_cli-0.7.0/src/launch/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/cli/entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:54:36.783665 launch_cli-0.7.0/src/launch/cli/github/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/cli/github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:54:36.783665 launch_cli-0.7.0/src/launch/cli/github/access/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/cli/github/access/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/cli/github/access/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:54:36.783665 launch_cli-0.7.0/src/launch/cli/github/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/cli/github/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/cli/github/hooks/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:54:36.783665 launch_cli-0.7.0/src/launch/cli/github/repo/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/cli/github/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/cli/github/repo/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:54:36.783665 launch_cli-0.7.0/src/launch/cli/github/version/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/cli/github/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/cli/github/version/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:54:36.783665 launch_cli-0.7.0/src/launch/cli/helm/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/cli/helm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/cli/helm/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:54:36.787665 launch_cli-0.7.0/src/launch/cli/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/cli/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15496 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/cli/service/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:54:36.787665 launch_cli-0.7.0/src/launch/cli/terragrunt/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/cli/terragrunt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14502 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/cli/terragrunt/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:54:36.787665 launch_cli-0.7.0/src/launch/cli/validate/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/cli/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/cli/validate/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:54:36.787665 launch_cli-0.7.0/src/launch/github/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/github/access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/github/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/github/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/github/labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/github/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/github/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:54:36.787665 launch_cli-0.7.0/src/launch/local_repo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/local_repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/local_repo/branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/local_repo/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/local_repo/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/local_repo/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:54:36.787665 launch_cli-0.7.0/src/launch/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/service/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-15 20:54:23.000000 launch_cli-0.7.0/src/launch/update.py
```

### Comparing `launch_cli-0.6.1/LICENSE` & `launch_cli-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `launch_cli-0.6.1/PKG-INFO` & `launch_cli-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: launch-cli
-Version: 0.6.1
+Version: 0.7.0
 Summary: CLI tooling for common Launch functions
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/launchbynttdata/launch-cli
 Project-URL: Issues, https://github.com/launchbynttdata/launch-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `launch_cli-0.6.1/README.md` & `launch_cli-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `launch_cli-0.6.1/launch_cli.egg-info/PKG-INFO` & `launch_cli-0.7.0/launch_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: launch-cli
-Version: 0.6.1
+Version: 0.7.0
 Summary: CLI tooling for common Launch functions
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/launchbynttdata/launch-cli
 Project-URL: Issues, https://github.com/launchbynttdata/launch-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `launch_cli-0.6.1/launch_cli.egg-info/SOURCES.txt` & `launch_cli-0.7.0/launch_cli.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 src/launch/cli/terragrunt/commands.py
 src/launch/cli/validate/__init__.py
 src/launch/cli/validate/commands.py
 src/launch/github/__init__.py
 src/launch/github/access.py
 src/launch/github/auth.py
 src/launch/github/hooks.py
+src/launch/github/labels.py
 src/launch/github/repo.py
 src/launch/github/tags.py
 src/launch/local_repo/__init__.py
 src/launch/local_repo/branch.py
 src/launch/local_repo/predict.py
 src/launch/local_repo/repo.py
 src/launch/local_repo/tags.py
```

### Comparing `launch_cli-0.6.1/pyproject.toml` & `launch_cli-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "launch-cli"
-version = "0.6.1"
+version = "0.7.0"
 description = "CLI tooling for common Launch functions"
 readme = "README.md"
 requires-python = ">=3.11"
 license = {text = "Apache 2.0"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `launch_cli-0.6.1/src/launch/__init__.py` & `launch_cli-0.7.0/src/launch/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from semver import Version
 
-VERSION = "0.6.1"
+VERSION = "0.7.0"
 
 SEMANTIC_VERSION = Version.parse(VERSION)
 GITHUB_ORG_NAME = "launchbynttdata"
 GITHUB_REPO_NAME = "launch-cli"
 SERVICE_SKELETON = "https://github.com/launchbynttdata/lcaf-skeleton-terragrunt.git"
 SKELETON_BRANCH = "main"
 MAIN_BRANCH = "main"
```

### Comparing `launch_cli-0.6.1/src/launch/automation/common/functions.py` & `launch_cli-0.7.0/src/launch/automation/common/functions.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.6.1/src/launch/automation/helm/functions.py` & `launch_cli-0.7.0/src/launch/automation/helm/functions.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.6.1/src/launch/automation/provider/aws/functions.py` & `launch_cli-0.7.0/src/launch/automation/provider/aws/functions.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.6.1/src/launch/automation/provider/az/functions.py` & `launch_cli-0.7.0/src/launch/automation/provider/az/functions.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.6.1/src/launch/automation/terragrunt/functions.py` & `launch_cli-0.7.0/src/launch/automation/terragrunt/functions.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.6.1/src/launch/cli/entrypoint.py` & `launch_cli-0.7.0/src/launch/cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.6.1/src/launch/cli/github/access/commands.py` & `launch_cli-0.7.0/src/launch/cli/github/access/commands.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.6.1/src/launch/cli/github/hooks/commands.py` & `launch_cli-0.7.0/src/launch/cli/github/hooks/commands.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.6.1/src/launch/cli/github/version/commands.py` & `launch_cli-0.7.0/src/launch/cli/github/version/commands.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.6.1/src/launch/cli/helm/commands.py` & `launch_cli-0.7.0/src/launch/cli/helm/commands.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.6.1/src/launch/cli/service/commands.py` & `launch_cli-0.7.0/src/launch/cli/service/commands.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.6.1/src/launch/cli/terragrunt/commands.py` & `launch_cli-0.7.0/src/launch/cli/terragrunt/commands.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.6.1/src/launch/cli/validate/commands.py` & `launch_cli-0.7.0/src/launch/cli/validate/commands.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.6.1/src/launch/env.py` & `launch_cli-0.7.0/src/launch/env.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.6.1/src/launch/github/access.py` & `launch_cli-0.7.0/src/launch/github/access.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.6.1/src/launch/github/auth.py` & `launch_cli-0.7.0/src/launch/github/auth.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.6.1/src/launch/github/hooks.py` & `launch_cli-0.7.0/src/launch/github/hooks.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.6.1/src/launch/github/repo.py` & `launch_cli-0.7.0/src/launch/github/repo.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.6.1/src/launch/github/tags.py` & `launch_cli-0.7.0/src/launch/github/tags.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.6.1/src/launch/local_repo/predict.py` & `launch_cli-0.7.0/src/launch/local_repo/predict.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import itertools
 import logging
+from enum import StrEnum
 
 from semver import Version
 
 logger = logging.getLogger(__name__)
 
 BRANCH_DELIMITER = "/"
 
@@ -13,15 +14,21 @@
 
 ALL_NAME_PARTS = list(
     itertools.chain(MAJOR_NAME_PARTS, MINOR_NAME_PARTS, PATCH_NAME_PARTS)
 )
 
 BREAKING_CHARS = ["!"]
 CAPITALIZE_FIRST_IS_BREAKING = True
-DEFAULT_VERSION = Version(major=0, minor=1, patch=0)
+DEFAULT_VERSION = Version(major=1, minor=0, patch=0)
+
+
+class ChangeType:
+    PATCH = "patch"
+    MINOR = "minor"
+    MAJOR = "major"
 
 
 class InvalidBranchNameException(Exception):
     pass
 
 
 def split_delimiter(branch_name: str, delimiter: str | None = None) -> tuple[str, str]:
@@ -64,23 +71,45 @@
 
 
 def predict_version(
     existing_tags: list[Version],
     branch_name: str,
     breaking_chars: list[str] | None = None,
     capitalize_first_is_breaking: bool | None = None,
-):
-    breaking_change: bool = False
-
+) -> Version:
     if not len(existing_tags):
         logger.warning(f"No tags exist on this repo, defaulting to {DEFAULT_VERSION}")
         return DEFAULT_VERSION
 
     latest_version = latest_tag(tags=existing_tags)
     logger.debug(f"Got {latest_version=} as the latest tag")
+    predicted_change_type = predict_change_type(
+        branch_name=branch_name,
+        breaking_chars=breaking_chars,
+        capitalize_first_is_breaking=capitalize_first_is_breaking,
+    )
+    match predicted_change_type:
+        case ChangeType.MAJOR:
+            return latest_version.bump_major()
+        case ChangeType.MINOR:
+            return latest_version.bump_minor()
+        case ChangeType.PATCH:
+            return latest_version.bump_patch()
+        case _:
+            raise ValueError(
+                f"Unexpected change type predicted: {predicted_change_type=}"
+            )
+
+
+def predict_change_type(
+    branch_name: str,
+    breaking_chars: list[str] | None = None,
+    capitalize_first_is_breaking: bool | None = None,
+) -> ChangeType:
+    breaking_change: bool = False
 
     if not breaking_chars:
         breaking_chars = BREAKING_CHARS
 
     if capitalize_first_is_breaking is None:
         capitalize_first_is_breaking = CAPITALIZE_FIRST_IS_BREAKING
 
@@ -105,15 +134,12 @@
         if revision_type[0] == revision_type[0].upper():
             logger.debug(
                 f"Revision begins with a capital letter, setting {breaking_change=}"
             )
             breaking_change = True
 
     if breaking_change or revision_type.lower().strip() in MAJOR_NAME_PARTS:
-        logger.debug("Bumping major version!")
-        return latest_version.bump_major()
+        return ChangeType.MAJOR
     elif revision_type.lower().strip() in MINOR_NAME_PARTS:
-        logger.debug("Bumping minor version!")
-        return latest_version.bump_minor()
+        return ChangeType.MINOR
     else:
-        logger.debug("Bumping patch version!")
-        return latest_version.bump_patch()
+        return ChangeType.PATCH
```

### Comparing `launch_cli-0.6.1/src/launch/local_repo/repo.py` & `launch_cli-0.7.0/src/launch/local_repo/repo.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.6.1/src/launch/local_repo/tags.py` & `launch_cli-0.7.0/src/launch/local_repo/tags.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.6.1/src/launch/service/common.py` & `launch_cli-0.7.0/src/launch/service/common.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.6.1/src/launch/update.py` & `launch_cli-0.7.0/src/launch/update.py`

 * *Files identical despite different names*

