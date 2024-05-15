# Comparing `tmp/smartsim-0.6.2.tar.gz` & `tmp/smartsim-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartsim-0.6.2.tar", last modified: Fri Feb 16 07:54:33 2024, max compression
+gzip compressed data, was "smartsim-0.7.0.tar", last modified: Wed May 15 00:41:07 2024, max compression
```

## Comparing `smartsim-0.6.2.tar` & `smartsim-0.7.0.tar`

### file list

```diff
@@ -1,151 +1,199 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:54:33.774295 smartsim-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-02-16 07:54:29.000000 smartsim-0.6.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-16 07:54:29.000000 smartsim-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-02-16 07:54:29.000000 smartsim-0.6.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    33751 2024-02-16 07:54:33.774295 smartsim-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    26787 2024-02-16 07:54:29.000000 smartsim-0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-02-16 07:54:29.000000 smartsim-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-02-16 07:54:33.778296 smartsim-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6794 2024-02-16 07:54:29.000000 smartsim-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:54:33.758295 smartsim-0.6.2/smartsim/
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:54:33.758295 smartsim-0.6.2/smartsim/_core/
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:54:33.762295 smartsim-0.6.2/smartsim/_core/_cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17341 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/_cli/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/_cli/clean.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/_cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/_cli/dbcli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/_cli/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/_cli/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/_cli/site.py
--rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/_cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11018 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/_cli/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:54:33.762295 smartsim-0.6.2/smartsim/_core/_install/
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/_install/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19354 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/_install/buildenv.py
--rw-r--r--   0 runner    (1001) docker     (127)    36217 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/_install/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:54:33.762295 smartsim-0.6.2/smartsim/_core/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8047 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    71337 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/config/keydb.conf
--rw-r--r--   0 runner    (1001) docker     (127)   106517 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/config/redis.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:54:33.762295 smartsim-0.6.2/smartsim/_core/control/
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35755 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/control/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/control/job.py
--rw-r--r--   0 runner    (1001) docker     (127)    14419 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/control/jobmanager.py
--rw-r--r--   0 runner    (1001) docker     (127)    11648 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/control/manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:54:33.766296 smartsim-0.6.2/smartsim/_core/entrypoints/
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/entrypoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12257 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/entrypoints/colocated.py
--rw-r--r--   0 runner    (1001) docker     (127)     7608 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/entrypoints/indirect.py
--rw-r--r--   0 runner    (1001) docker     (127)     6008 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/entrypoints/redis.py
--rw-r--r--   0 runner    (1001) docker     (127)    23617 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/entrypoints/telemetrymonitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:54:33.766296 smartsim-0.6.2/smartsim/_core/generation/
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13771 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/generation/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7130 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/generation/modelwriter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:54:33.766296 smartsim-0.6.2/smartsim/_core/launcher/
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/launcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9318 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/launcher/colocated.py
--rw-r--r--   0 runner    (1001) docker     (127)     6920 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/launcher/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:54:33.766296 smartsim-0.6.2/smartsim/_core/launcher/local/
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/launcher/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/launcher/local/local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:54:33.766296 smartsim-0.6.2/smartsim/_core/launcher/lsf/
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/launcher/lsf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/launcher/lsf/lsfCommands.py
--rw-r--r--   0 runner    (1001) docker     (127)     8280 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/launcher/lsf/lsfLauncher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/launcher/lsf/lsfParser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:54:33.766296 smartsim-0.6.2/smartsim/_core/launcher/pbs/
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/launcher/pbs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/launcher/pbs/pbsCommands.py
--rw-r--r--   0 runner    (1001) docker     (127)     7372 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/launcher/pbs/pbsLauncher.py
--rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/launcher/pbs/pbsParser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:54:33.766296 smartsim-0.6.2/smartsim/_core/launcher/slurm/
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/launcher/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/launcher/slurm/slurmCommands.py
--rw-r--r--   0 runner    (1001) docker     (127)    11580 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/launcher/slurm/slurmLauncher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/launcher/slurm/slurmParser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:54:33.770295 smartsim-0.6.2/smartsim/_core/launcher/step/
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/launcher/step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/launcher/step/alpsStep.py
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/launcher/step/localStep.py
--rw-r--r--   0 runner    (1001) docker     (127)    12348 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/launcher/step/lsfStep.py
--rw-r--r--   0 runner    (1001) docker     (127)     7647 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/launcher/step/mpiStep.py
--rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/launcher/step/pbsStep.py
--rw-r--r--   0 runner    (1001) docker     (127)     8763 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/launcher/step/slurmStep.py
--rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/launcher/step/step.py
--rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/launcher/stepInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/launcher/stepMapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    13720 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/launcher/taskManager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:54:33.770295 smartsim-0.6.2/smartsim/_core/launcher/util/
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/launcher/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/launcher/util/launcherUtil.py
--rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/launcher/util/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:54:33.770295 smartsim-0.6.2/smartsim/_core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9814 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/utils/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     8977 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/utils/redis.py
--rw-r--r--   0 runner    (1001) docker     (127)     8737 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/_core/utils/serialize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:54:33.770295 smartsim-0.6.2/smartsim/database/
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35557 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/database/orchestrator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:54:33.770295 smartsim-0.6.2/smartsim/entity/
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9052 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/entity/dbnode.py
--rw-r--r--   0 runner    (1001) docker     (127)    11607 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/entity/dbobject.py
--rw-r--r--   0 runner    (1001) docker     (127)    24272 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/entity/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/entity/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/entity/entityList.py
--rw-r--r--   0 runner    (1001) docker     (127)    12423 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/entity/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    29345 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/entity/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/entity/strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:54:33.770295 smartsim-0.6.2/smartsim/error/
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/error/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4998 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/error/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    36006 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)    12734 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:54:33.774295 smartsim-0.6.2/smartsim/ml/
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19736 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/ml/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:54:33.774295 smartsim-0.6.2/smartsim/ml/tf/
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/ml/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/ml/tf/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/ml/tf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:54:33.774295 smartsim-0.6.2/smartsim/ml/torch/
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/ml/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/ml/torch/data.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/servertype.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:54:33.774295 smartsim-0.6.2/smartsim/settings/
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8767 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/settings/alpsSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)    23505 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/settings/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/settings/containers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20814 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/settings/lsfSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)    14023 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/settings/mpiSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/settings/mpirunSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     9193 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/settings/palsSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)    10576 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/settings/pbsSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     7564 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    19074 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/settings/slurmSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/slurm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/status.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-16 07:54:33.000000 smartsim-0.6.2/smartsim/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:54:33.774295 smartsim-0.6.2/smartsim/wlm/
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/wlm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/wlm/pbs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12546 2024-02-16 07:54:29.000000 smartsim-0.6.2/smartsim/wlm/slurm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 07:54:33.758295 smartsim-0.6.2/smartsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    33751 2024-02-16 07:54:33.000000 smartsim-0.6.2/smartsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-02-16 07:54:33.000000 smartsim-0.6.2/smartsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 07:54:33.000000 smartsim-0.6.2/smartsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-16 07:54:33.000000 smartsim-0.6.2/smartsim.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 07:54:33.000000 smartsim-0.6.2/smartsim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-02-16 07:54:33.000000 smartsim-0.6.2/smartsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-16 07:54:33.000000 smartsim-0.6.2/smartsim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:41:07.135481 smartsim-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-15 00:41:03.000000 smartsim-0.7.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-15 00:41:03.000000 smartsim-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-05-15 00:41:03.000000 smartsim-0.7.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    27924 2024-05-15 00:41:07.135481 smartsim-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27036 2024-05-15 00:41:03.000000 smartsim-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-05-15 00:41:03.000000 smartsim-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-15 00:41:07.135481 smartsim-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-05-15 00:41:03.000000 smartsim-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:41:07.111482 smartsim-0.7.0/smartsim/
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:41:07.111482 smartsim-0.7.0/smartsim/_core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:41:07.111482 smartsim-0.7.0/smartsim/_core/_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18505 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/_cli/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/_cli/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/_cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/_cli/dbcli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/_cli/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/_cli/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:41:07.115481 smartsim-0.7.0/smartsim/_core/_cli/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     8018 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/_cli/scripts/dragon_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/_cli/site.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/_cli/teardown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/_cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10911 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/_cli/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:41:07.115481 smartsim-0.7.0/smartsim/_core/_install/
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/_install/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19354 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/_install/buildenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36937 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/_install/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:41:07.115481 smartsim-0.7.0/smartsim/_core/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10060 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71337 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/config/keydb.conf
+-rw-r--r--   0 runner    (1001) docker     (127)   106517 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/config/redis.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:41:07.115481 smartsim-0.7.0/smartsim/_core/control/
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37540 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/control/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/control/controller_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/control/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13785 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/control/jobmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11761 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/control/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/control/previewrenderer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:41:07.115481 smartsim-0.7.0/smartsim/_core/entrypoints/
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/entrypoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12384 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/entrypoints/colocated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11979 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/entrypoints/dragon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/entrypoints/dragon_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/entrypoints/indirect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/entrypoints/redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/entrypoints/telemetrymonitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:41:07.119481 smartsim-0.7.0/smartsim/_core/generation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13156 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/generation/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/generation/modelwriter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:41:07.119481 smartsim-0.7.0/smartsim/_core/launcher/
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/launcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9146 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/launcher/colocated.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:41:07.119481 smartsim-0.7.0/smartsim/_core/launcher/dragon/
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/launcher/dragon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28582 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/launcher/dragon/dragonBackend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21188 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/launcher/dragon/dragonConnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12393 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/launcher/dragon/dragonLauncher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/launcher/dragon/dragonSockets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/launcher/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:41:07.119481 smartsim-0.7.0/smartsim/_core/launcher/local/
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/launcher/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/launcher/local/local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:41:07.119481 smartsim-0.7.0/smartsim/_core/launcher/lsf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/launcher/lsf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/launcher/lsf/lsfCommands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8150 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/launcher/lsf/lsfLauncher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/launcher/lsf/lsfParser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:41:07.123481 smartsim-0.7.0/smartsim/_core/launcher/pbs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/launcher/pbs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/launcher/pbs/pbsCommands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7739 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/launcher/pbs/pbsLauncher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/launcher/pbs/pbsParser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:41:07.123481 smartsim-0.7.0/smartsim/_core/launcher/slurm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/launcher/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/launcher/slurm/slurmCommands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11391 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/launcher/slurm/slurmLauncher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/launcher/slurm/slurmParser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:41:07.123481 smartsim-0.7.0/smartsim/_core/launcher/step/
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/launcher/step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/launcher/step/alpsStep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9023 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/launcher/step/dragonStep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/launcher/step/localStep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12043 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/launcher/step/lsfStep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/launcher/step/mpiStep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/launcher/step/pbsStep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/launcher/step/slurmStep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7123 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/launcher/step/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/launcher/stepInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/launcher/stepMapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12837 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/launcher/taskManager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:41:07.123481 smartsim-0.7.0/smartsim/_core/launcher/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/launcher/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/launcher/util/launcherUtil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/launcher/util/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:41:07.123481 smartsim-0.7.0/smartsim/_core/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/schemas/dragonRequests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/schemas/dragonResponses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/schemas/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:41:07.127481 smartsim-0.7.0/smartsim/_core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16083 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/utils/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/utils/redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11945 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/utils/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9074 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/utils/serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:41:07.127481 smartsim-0.7.0/smartsim/_core/utils/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/utils/telemetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18377 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/utils/telemetry/collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9512 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/utils/telemetry/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/utils/telemetry/sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24742 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/utils/telemetry/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/_core/utils/telemetry/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:41:07.127481 smartsim-0.7.0/smartsim/database/
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36594 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/database/orchestrator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:41:07.127481 smartsim-0.7.0/smartsim/entity/
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/entity/dbnode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10584 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/entity/dbobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22331 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/entity/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/entity/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6358 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/entity/entityList.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11887 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/entity/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27360 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/entity/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/entity/strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:41:07.127481 smartsim-0.7.0/smartsim/error/
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/error/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/error/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37226 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12689 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:41:07.127481 smartsim-0.7.0/smartsim/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19147 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/ml/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:41:07.131481 smartsim-0.7.0/smartsim/ml/tf/
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/ml/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/ml/tf/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/ml/tf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:41:07.131481 smartsim-0.7.0/smartsim/ml/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/ml/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/ml/torch/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/servertype.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:41:07.131481 smartsim-0.7.0/smartsim/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/settings/alpsSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22795 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/settings/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/settings/containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/settings/dragonRunSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19578 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/settings/lsfSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12559 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/settings/mpiSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/settings/palsSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9914 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/settings/pbsSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7343 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18146 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/settings/slurmSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:41:07.107482 smartsim-0.7.0/smartsim/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:41:07.107482 smartsim-0.7.0/smartsim/templates/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:41:07.107482 smartsim-0.7.0/smartsim/templates/templates/preview/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:41:07.135481 smartsim-0.7.0/smartsim/templates/templates/preview/plain_text/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/templates/templates/preview/plain_text/activeinfra.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/templates/templates/preview/plain_text/base.template
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/templates/templates/preview/plain_text/clientconfig.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/templates/templates/preview/plain_text/clientconfig_debug.template
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/templates/templates/preview/plain_text/clientconfig_info.template
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/templates/templates/preview/plain_text/clientconfigcolo.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/templates/templates/preview/plain_text/clientconfigcolo_debug.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/templates/templates/preview/plain_text/clientconfigcolo_info.template
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/templates/templates/preview/plain_text/ensemble.template
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/templates/templates/preview/plain_text/ensemble_debug.template
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/templates/templates/preview/plain_text/ensemble_info.template
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/templates/templates/preview/plain_text/experiment.template
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/templates/templates/preview/plain_text/model.template
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/templates/templates/preview/plain_text/model_debug.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/templates/templates/preview/plain_text/model_info.template
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/templates/templates/preview/plain_text/orchestrator.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/templates/templates/preview/plain_text/orchestrator_debug.template
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/templates/templates/preview/plain_text/orchestrator_info.template
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-15 00:41:06.000000 smartsim-0.7.0/smartsim/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:41:07.135481 smartsim-0.7.0/smartsim/wlm/
+-rw-r--r--   0 runner    (1001) docker     (127)     5303 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/wlm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/wlm/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11916 2024-05-15 00:41:03.000000 smartsim-0.7.0/smartsim/wlm/slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:41:07.111482 smartsim-0.7.0/smartsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27924 2024-05-15 00:41:07.000000 smartsim-0.7.0/smartsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-05-15 00:41:07.000000 smartsim-0.7.0/smartsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 00:41:07.000000 smartsim-0.7.0/smartsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-15 00:41:07.000000 smartsim-0.7.0/smartsim.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 00:41:07.000000 smartsim-0.7.0/smartsim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-15 00:41:07.000000 smartsim-0.7.0/smartsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 00:41:07.000000 smartsim-0.7.0/smartsim.egg-info/top_level.txt
```

### Comparing `smartsim-0.6.2/LICENSE.md` & `smartsim-0.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `smartsim-0.6.2/Makefile` & `smartsim-0.7.0/Makefile`

 * *Files 0% similar despite different names*

```diff
@@ -146,19 +146,19 @@
 
 # help: tutorials-dev                  - Build and start a docker container to run the tutorials
 .PHONY: tutorials-dev
 tutorials-dev:
 	@docker compose build tutorials-dev
 	@docker run -p 8888:8888 smartsim-tutorials:dev-latest
 
-# help: tutorials-prod                 - Build and start a docker container to run the tutorials (v0.6.2)
+# help: tutorials-prod                 - Build and start a docker container to run the tutorials (v0.7.0)
 .PHONY: tutorials-prod
 tutorials-prod:
 	@docker compose build tutorials-prod
-	@docker run -p 8888:8888 smartsim-tutorials:v0.6.2
+	@docker run -p 8888:8888 smartsim-tutorials:v0.7.0
 
 
 # help:
 # help: Test
 # help: -------
 
 # help: test                           - Run all tests
```

### Comparing `smartsim-0.6.2/PKG-INFO` & `smartsim-0.7.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,780 +1,759 @@
-Metadata-Version: 2.1
-Name: smartsim
-Version: 0.6.2
-Summary: AI Workflows for Science
-Home-page: https://github.com/CrayLabs/SmartSim
-Author: CrayLabs, a Hewlett Packard Enterprise OSS Organization
-Author-email: craylabs@hpe.com
-License: BSD 2-Clause License
-Project-URL: Source, https://github.com/CrayLabs/SmartSim
-Project-URL: Documentation, https://www.craylabs.org
-Description: 
-        
-        <div align="center">
-            <a href="https://github.com/CrayLabs/SmartSim"><img src="https://raw.githubusercontent.com/CrayLabs/SmartSim/master/doc/images/SmartSim_Large.png" width="90%"><img></a>
-            <br />
-            <br />
-        <div display="inline-block">
-            <a href="https://github.com/CrayLabs/SmartSim"><b>Home</b></a>&nbsp;&nbsp;&nbsp;
-            <a href="https://www.craylabs.org/docs/installation_instructions/basic.html"><b>Install</b></a>&nbsp;&nbsp;&nbsp;
-            <a href="https://www.craylabs.org/docs/overview.html"><b>Documentation</b></a>&nbsp;&nbsp;&nbsp;
-            <a href="https://github.com/CrayLabs"><b>Cray Labs</b></a>&nbsp;&nbsp;&nbsp;
-            <a href="mailto:craylabs@hpe.com"><b>Contact</b></a>&nbsp;&nbsp;&nbsp;
-            <a href="https://join.slack.com/t/craylabs/shared_invite/zt-nw3ag5z5-5PS4tIXBfufu1bIvvr71UA"><b>Join us on Slack!</b></a>&nbsp;&nbsp;&nbsp;
-          </div>
-            <br />
-            <br />
-        </div>
-        
-        
-        <div align="center">
-        
-        [![License](https://img.shields.io/github/license/CrayLabs/SmartSim)](https://github.com/CrayLabs/SmartSim/blob/master/LICENSE.md)
-        ![GitHub last commit](https://img.shields.io/github/last-commit/CrayLabs/SmartSim)
-        ![GitHub deployments](https://img.shields.io/github/deployments/CrayLabs/SmartSim/github-pages?label=doc%20build)
-        ![PyPI - Wheel](https://img.shields.io/pypi/wheel/smartsim)
-        ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/smartsim)
-        ![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/CrayLabs/SmartSim)
-        ![Language](https://img.shields.io/github/languages/top/CrayLabs/SmartSim)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        [![codecov](https://codecov.io/gh/CrayLabs/SmartSim/branch/develop/graph/badge.svg?token=96HFI2F45E)](https://codecov.io/gh/CrayLabs/SmartSim)
-        [![Downloads](https://static.pepy.tech/personalized-badge/smartsim?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/smartsim)
-        
-        </div>
-        
-        ------------
-        
-        # SmartSim
-        
-        SmartSim is made up of two parts
-          1. SmartSim Infrastructure Library (This repository)
-          2. [SmartRedis](https://github.com/CrayLabs/SmartRedis)
-        
-        The two library components are designed to work together, but can also be used
-        independently.
-        
-        *SmartSim* is a workflow library that makes it easier to use common Machine Learning (ML)
-        libraries, like PyTorch and TensorFlow, in High Performance Computing (HPC) simulations
-        and applications. SmartSim launches ML infrastructure on HPC systems alongside user
-        workloads.
-        
-        *SmartRedis* provides an API to connect HPC workloads, particularly (MPI + X) simulations,
-        to the ML infrastructure, namely the The [Orchestrator database](https://www.craylabs.org/docs/orchestrator.html),
-        launched by SmartSim.
-        
-        Applications integrated with the SmartRedis clients, written in Fortran, C, C++ and Python,
-        can send data to and remotely request SmartSim infrastructure to execute ML models and scripts
-        on GPU or CPU. The distributed Client-Server paradigm allows for data to be seamlessly
-        exchanged between applications at runtime without the utilization of MPI.
-        
-        ----------
-        
-        **Table of Contents**
-        - [SmartSim](#smartsim)
-        - [Quick Start](#quick-start)
-        - [SmartSim Infrastructure Library](#smartsim-infrastructure-library)
-          - [Experiments](#experiments)
-            - [Hello World](#hello-world)
-            - [Hello World MPI](#hello-world-mpi)
-          - [Experiments on HPC Systems](#experiments-on-hpc-systems)
-            - [Interactive Launch Example](#interactive-launch-example)
-            - [Batch Launch Examples](#batch-launch-examples)
-        - [Infrastructure Library Applications](#infrastructure-library-applications)
-          - [Redis + RedisAI](#redis--redisai)
-            - [Local Launch](#local-launch)
-            - [Interactive Launch](#interactive-launch)
-            - [Batch Launch](#batch-launch)
-        - [SmartRedis](#smartredis)
-          - [Tensors](#tensors)
-          - [Datasets](#datasets)
-        - [SmartSim + SmartRedis Tutorials](#smartsim--smartredis-tutorials)
-          - [Run the Tutorials](#run-the-tutorials)
-          - [Online Analysis](#online-analysis)
-              - [Lattice Boltzmann Simulation](#lattice-boltzmann-simulation)
-          - [Online Processing](#online-processing)
-            - [Singular Value Decomposition](#singular-value-decomposition)
-          - [Online Inference](#online-inference)
-            - [PyTorch CNN Example](#pytorch-cnn-example)
-        - [Publications](#publications)
-        - [Cite](#cite)
-          - [bibtex](#bibtex)
-        
-        ----
-        
-        # Quick Start
-        
-        
-        The documentation has a number of tutorials that make it easy to get used to SmartSim locally
-        before using it on your system. Each tutorial is a Jupyter notebook that can be run through the
-        [SmartSim Tutorials docker image](https://github.com/orgs/CrayLabs/packages?repo_name=SmartSim)
-        which will run a jupyter lab with the tutorials, SmartSim, and SmartRedis installed.
-        
-        ```bash
-        docker pull ghcr.io/craylabs/smartsim-tutorials:latest
-        docker run -p 8888:8888 ghcr.io/craylabs/smartsim-tutorials:latest
-        # click on link to open jupyter lab
-        ```
-        
-        # SmartSim Infrastructure Library
-        
-        The Infrastructure Library (IL), the ``smartsim`` python package,
-        facilitates the launch of Machine Learning and simulation
-        workflows. The Python interface of the IL creates, configures, launches and monitors
-        applications.
-        
-        ## Experiments
-        
-        The [Experiment](https://www.craylabs.org/docs/api/smartsim_api.html#experiment) object
-        is the main interface of SmartSim. Through the [Experiment](https://www.craylabs.org/docs/api/smartsim_api.html#experiment)
-        users can create references to user applications called ``Models``.
-        ### Hello World
-        
-        Below is a simple example of a workflow that uses the IL to launch hello world
-        program using the local launcher which is designed for laptops and single nodes.
-        
-        ```python
-        from smartsim import Experiment
-        
-        exp = Experiment("simple", launcher="local")
-        
-        settings = exp.create_run_settings("echo", exe_args="Hello World")
-        model = exp.create_model("hello_world", settings)
-        
-        exp.start(model, block=True)
-        print(exp.get_status(model))
-        ```
-        
-        ### Hello World MPI
-        
-        The [Experiment.create_run_settings](https://www.craylabs.org/docs/api/smartsim_api.html#smartsim.experiment.Experiment.create_run_settings) method returns a ``RunSettings`` object which
-        defines how a model is launched. There are many types of ``RunSettings`` [supported by
-        SmartSim](https://www.craylabs.org/docs/api/smartsim_api.html#settings).
-        
-         - ``RunSettings``
-         - ``MpirunSettings``
-         - ``SrunSettings``
-         - ``AprunSettings``
-         - ``JsrunSettings``
-        
-        The following example launches a hello world MPI program using the local launcher
-        for single compute node, workstations and laptops.
-        
-        ```Python
-        from smartsim import Experiment
-        
-        exp = Experiment("hello_world", launcher="local")
-        mpi_settings = exp.create_run_settings(exe="echo",
-                                               exe_args="Hello World!",
-                                               run_command="mpirun")
-        mpi_settings.set_tasks(4)
-        
-        mpi_model = exp.create_model("hello_world", mpi_settings)
-        
-        exp.start(mpi_model, block=True)
-        print(exp.get_status(model))
-        ```
-        
-        If an argument of `run_command="auto"` (the default) is passed to
-        `Experiment.create_run_settings`, SmartSim will attempt to find a run command on the
-        system with which it has a corresponding `RunSettings` class. If one can be found,
-        `Experiment.create_run_settings` will instance and return an object of that type.
-        
-        
-        -----------
-        ## Experiments on HPC Systems
-        
-        SmartSim integrates with common HPC schedulers providing batch and interactive
-        launch capabilities for all applications.
-        
-         - Slurm
-         - LSF
-         - PBSPro
-         - Local (for laptops/single node, no batch)
-        
-        
-        ### Interactive Launch Example
-        
-        The following launches the same ``hello_world`` model in an interactive allocation.
-        
-        ```bash
-        # get interactive allocation (Slurm)
-        salloc -N 3 --ntasks-per-node=20 --ntasks 60 --exclusive -t 00:10:00
-        
-        # get interactive allocation (PBS)
-        qsub -l select=3:ncpus=20 -l walltime=00:10:00 -l place=scatter -I -q <queue>
-        
-        # get interactive allocation (LSF)
-        bsub -Is -W 00:10 -nnodes 3 -P <project> $SHELL
-        ```
-        
-        This same script will run on a SLURM, PBS, or LSF system as the ``launcher``
-        is set to `auto` in the [Experiment](https://www.craylabs.org/docs/api/smartsim_api.html#experiment)
-        initialization. The run command like ``mpirun``,
-        ``aprun`` or ``srun`` will be automatically detected from what is available on the
-        system.
-        
-        ```python
-        # hello_world.py
-        from smartsim import Experiment
-        
-        exp = Experiment("hello_world_exp", launcher="auto")
-        run = exp.create_run_settings(exe="echo", exe_args="Hello World!")
-        run.set_tasks(60)
-        run.set_tasks_per_node(20)
-        
-        model = exp.create_model("hello_world", run)
-        exp.start(model, block=True, summary=True)
-        
-        print(exp.get_status(model))
-        ```
-        ```bash
-        # in interactive terminal
-        python hello_world.py
-        ```
-        
-        
-        This script could also be launched in a batch file instead of an
-        interactive terminal. For example, for Slurm:
-        
-        ```bash
-        #!/bin/bash
-        #SBATCH --exclusive
-        #SBATCH --nodes=3
-        #SBATCH --ntasks-per-node=20
-        #SBATCH --time=00:10:00
-        
-        python /path/to/hello_world.py
-        ```
-        ```bash
-        # on Slurm system
-        sbatch run_hello_world.sh
-        ```
-        
-        
-        ### Batch Launch Examples
-        
-        SmartSim can also launch workloads in a batch directly from Python, without the need
-        for a batch script. Users can launch groups of ``Model`` instances in a ``Ensemble``.
-        
-        The following launches 4 replicas of the the same ``hello_world`` model.
-        
-        ```python
-        # hello_ensemble.py
-        from smartsim import Experiment
-        
-        exp = Experiment("hello_world_batch", launcher="auto")
-        
-        # define resources for all ensemble members
-        batch = exp.create_batch_settings(nodes=4, time="00:10:00", account="12345-Cray")
-        batch.set_queue("premium")
-        
-        # define how each member should run
-        run = exp.create_run_settings(exe="echo", exe_args="Hello World!")
-        run.set_tasks(60)
-        run.set_tasks_per_node(20)
-        
-        ensemble = exp.create_ensemble("hello_world",
-                                       batch_settings=batch,
-                                       run_settings=run,
-                                       replicas=4)
-        exp.start(ensemble, block=True, summary=True)
-        
-        print(exp.get_status(ensemble))
-        ```
-        
-        ```bash
-        python hello_ensemble.py
-        ```
-        
-        Similar to the interactive example, this same script will run on a SLURM, PBS,
-        or LSF system as the ``launcher`` is set to `auto` in the
-        [Experiment](https://www.craylabs.org/docs/api/smartsim_api.html#experiment)
-        initialization. Local launching does not support batch workloads.
-        
-        
-        --------
-        
-        # Infrastructure Library Applications
-         - Orchestrator - In-memory data store and Machine Learning Inference (Redis + RedisAI)
-        
-        ## Redis + RedisAI
-        
-        The ``Orchestrator`` is an in-memory database that utilizes Redis and RedisAI to provide
-        a distributed database and access to ML runtimes from Fortran, C, C++ and Python.
-        
-        SmartSim provides classes that make it simple to launch the database in many
-        configurations and optionally form a distributed database cluster. The examples
-        below will show how to launch the database. Later in this document we will show
-        how to use the database to perform ML inference and processing.
-        
-        
-        ### Local Launch
-        
-        The following script launches a single database using the local launcher.
-        
-        [Experiment.create_database](https://www.craylabs.org/docs/api/smartsim_api.html#smartsim.experiment.Experiment.create_database)
-        will initialize an ``Orchestrator`` instance corresponding to the specified launcher.
-        
-        ```python
-        # run_db_local.py
-        from smartsim import Experiment
-        
-        exp = Experiment("local-db", launcher="local")
-        db = exp.create_database(port=6780,       # database port
-                                 interface="lo")  # network interface to use
-        
-        # by default, SmartSim never blocks execution after the database is launched.
-        exp.start(db)
-        
-        # launch models, analysis, training, inference sessions, etc
-        # that communicate with the database using the SmartRedis clients
-        
-        # stop the database
-        exp.stop(db)
-        ```
-        
-        ### Interactive Launch
-        
-        The ``Orchestrator``, like ``Ensemble`` instances, can be launched locally, in interactive
-        allocations, or in a batch.
-        
-        The following example launches a distributed (3 node) database cluster
-        in an interactive allocation.
-        
-        
-        ```bash
-        # get interactive allocation (Slurm)
-        salloc -N 3 --ntasks-per-node=1 --exclusive -t 00:10:00
-        
-        # get interactive allocation (PBS)
-        qsub -l select=3:ncpus=1 -l walltime=00:10:00 -l place=scatter -I -q queue
-        
-        # get interactive allocation (LSF)
-        bsub -Is -W 00:10 -nnodes 3 -P project $SHELL
-        
-        ```
-        
-        ```python
-        # run_db.py
-        from smartsim import Experiment
-        
-        # auto specified to work across launcher types
-        exp = Experiment("db-on-slurm", launcher="auto")
-        db_cluster = exp.create_database(db_nodes=3,
-                                         db_port=6780,
-                                         batch=False,
-                                         interface="ipogif0")
-        exp.start(db_cluster)
-        
-        print(f"Orchestrator launched on nodes: {db_cluster.hosts}")
-        # launch models, analysis, training, inference sessions, etc
-        # that communicate with the database using the SmartRedis clients
-        
-        exp.stop(db_cluster)
-        ```
-        ```bash
-        # in interactive terminal
-        python run_db.py
-        ```
-        
-        ### Batch Launch
-        
-        The ``Orchestrator`` can also be launched in a batch without the need for an interactive allocation.
-        SmartSim will create the batch file, submit it to the batch system, and then wait for the database
-        to be launched. Users can hit CTRL-C to cancel the launch if needed.
-        
-        ```Python
-        # run_db_batch.py
-        from smartsim import Experiment
-        
-        exp = Experiment("batch-db-on-pbs", launcher="auto")
-        db_cluster = exp.create_database(db_nodes=3,
-                                         db_port=6780,
-                                         batch=True,
-                                         time="00:10:00",
-                                         interface="ib0",
-                                         account="12345-Cray",
-                                         queue="cl40")
-        
-        exp.start(db_cluster)
-        
-        print(f"Orchestrator launched on nodes: {db_cluster.hosts}")
-        # launch models, analysis, training, inference sessions, etc
-        # that communicate with the database using the SmartRedis clients
-        
-        exp.stop(db_cluster)
-        ```
-        
-        ```bash
-        python run_db_batch.py
-        ```
-        
-        ------
-        # SmartRedis
-        
-        The SmartSim IL Clients ([SmartRedis](https://github.com/CrayLabs/SmartRedis))
-        are implementations of Redis clients that implement the RedisAI
-        API with additions specific to scientific workflows.
-        
-        SmartRedis clients are available in Fortran, C, C++, and Python.
-        Users can seamlessly pull and push data from the Orchestrator from different languages.
-        
-        ## Tensors
-        
-        Tensors are the fundamental data structure for the SmartRedis clients. The Clients
-        use the native array format of the language. For example, in Python, a tensor is
-        a NumPy array while the C/C++ clients accept nested and contiguous arrays.
-        
-        When stored in the database, all tensors are stored in the same format. Hence,
-        any language can receive a tensor from the database no matter what supported language
-        the array was sent from. This enables applications in different languages to communicate
-        numerical data with each other at runtime.
-        
-        For more information on the tensor data structure, see
-        [the documentation](https://www.craylabs.org/docs/sr_data_structures.html#tensor)
-        
-        ## Datasets
-        
-        Datasets are collections of Tensors and associated metadata. The ``Dataset`` class
-        is a user space object that can be created, added to, sent to, and retrieved from
-        the Orchestrator.
-        
-        For an example of how to use the ``Dataset`` class, see the [Online Analysis example](#online-analysis)
-        
-        For more information on the API, see the
-        [API documentation](https://www.craylabs.org/docs/sr_data_structures.html#dataset)
-        
-        # SmartSim + SmartRedis Tutorials
-        
-        SmartSim and SmartRedis were designed to work together. When launched through
-        SmartSim, applications using the SmartRedis clients are directly connected to
-        any Orchestrator launched in the same [Experiment](https://www.craylabs.org/docs/api/smartsim_api.html#experiment).
-        
-        In this way, a SmartSim [Experiment](https://www.craylabs.org/docs/api/smartsim_api.html#experiment) becomes a driver for coupled ML and Simulation
-        workflows. The following are simple examples of how to use SmartSim and SmartRedis
-        together.
-        
-        ## Run the Tutorials
-        
-        Each tutorial is a Jupyter notebook that can be run through the
-        [SmartSim Tutorials docker image](https://github.com/orgs/CrayLabs/packages?repo_name=SmartSim)
-        which will run a jupyter lab with the tutorials, SmartSim, and SmartRedis installed.
-        
-        ```bash
-        docker pull ghcr.io/craylabs/smartsim-tutorials:latest
-        docker run -p 8888:8888 ghcr.io/craylabs/smartsim-tutorials:latest
-        ```
-        Each of the following examples can be found in the
-        [SmartSim documentation](https://www.craylabs.org/docs/tutorials/getting_started/getting_started.html).
-        
-        ## Online Analysis
-        
-        Using SmartSim, HPC applications can be monitored in real time by streaming data
-        from the application to the database. SmartRedis clients can retrieve the
-        data, process, analyze it, and finally store any updated data back to the database for
-        use by other clients.
-        
-        The following is an example of how a user could monitor and analyze a simulation.
-        The example here uses the Python client; however, SmartRedis clients are also available
-        for C, C++, and Fortran. All SmartRedis clients implement the same API.
-        
-        The example will produce [this visualization](https://user-images.githubusercontent.com/13009163/127622717-2c9e4cfd-50f4-4d94-88c4-8c05fa2fa616.mp4) while the simulation is running.
-        
-        #### Lattice Boltzmann Simulation
-        
-        Using a [Lattice Boltzmann Simulation](https://en.wikipedia.org/wiki/Lattice_Boltzmann_methods),
-        this example demonstrates how to use the SmartRedis ``Dataset`` API to stream
-        data over the Orchestrator deployed by SmartSim.
-        
-        The simulation will be composed of two parts: `fv_sim.py` which will generate data from
-        the Simulation and store it in the Orchestrator, and `driver.py`
-        which will launch the Orchestrator, start `fv_sim.py` and check for data posted to the
-        Orchestrator to plot updates in real-time.
-        
-        The following code highlights the sections of `fv_sim.py` that are responsible for
-        transmitting the data needed to plot timesteps of the simulation to the Orchestrator.
-        
-        ```Python
-        # fv_sim.py
-        from smartredis import Client
-        import numpy as np
-        
-        # initialization code omitted
-        
-        # save cylinder location to database
-        cylinder = (X - x_res/4)**2 + (Y - y_res/2)**2 < (y_res/4)**2 # bool array
-        client.put_tensor("cylinder", cylinder.astype(np.int8))
-        
-        for time_step in range(steps): # simulation loop
-            for i, cx, cy in zip(idxs, cxs, cys):
-                F[:,:,i] = np.roll(F[:,:,i], cx, axis=1)
-                F[:,:,i] = np.roll(F[:,:,i], cy, axis=0)
-        
-            bndryF = F[cylinder,:]
-            bndryF = bndryF[:,[0,5,6,7,8,1,2,3,4]]
-        
-            rho = np.sum(F, 2)
-            ux  = np.sum(F * cxs, 2) / rho
-            uy  = np.sum(F * cys, 2) / rho
-        
-            Feq = np.zeros(F.shape)
-            for i, cx, cy, w in zip(idxs, cxs, cys, weights):
-                Feq[:,:,i] = rho * w * ( 1 + 3*(cx*ux+cy*uy)  + 9*(cx*ux+cy*uy)**2/2 - 3*(ux**2+uy**2)/2 )
-            F += -(1.0/tau) * (F - Feq)
-            F[cylinder,:] = bndryF
-        
-            # Create a SmartRedis dataset with vorticity data
-            dataset = Dataset(f"data_{str(time_step)}")
-            dataset.add_tensor("ux", ux)
-            dataset.add_tensor("uy", uy)
-        
-            # Put Dataset in db at key "data_{time_step}"
-            client.put_dataset(dataset)
-        ```
-        
-        The driver script, `driver.py`, launches the Orchestrator database and runs
-        the simulation in a non-blocking fashion. The driver script then uses the SmartRedis
-        client to pull the DataSet and plot the vorticity while the simulation is running.
-        
-        ```Python
-        # driver.py
-        time_steps, seed = 3000, 42
-        
-        exp = Experiment("finite_volume_simulation", launcher="local")
-        
-        db = exp.create_database(port=6780,        # database port
-                                 interface="lo")   # network interface db should listen on
-        
-        # create the lb simulation Model reference
-        settings = exp.create_run_settings("python",
-                                           exe_args=["fv_sim.py",
-                                                     f"--seed={seed}",
-                                                     f"--steps={time_steps}"])
-        model = exp.create_model("fv_simulation", settings)
-        model.attach_generator_files(to_copy="fv_sim.py")
-        exp.generate(db, model, overwrite=True)
-        
-        exp.start(db)
-        client = Client(address=db.get_address()[0], cluster=False)
-        
-        # start simulation (non-blocking)
-        exp.start(model, block=False, summary=True)
-        
-        # poll until simulation starts and then retrieve data
-        client.poll_key("cylinder", 200, 100)
-        cylinder = client.get_tensor("cylinder").astype(bool)
-        
-        for i in range(0, time_steps):
-            client.poll_key(f"data_{str(i)}", 10, 1000)
-            dataset = client.get_dataset(f"data_{str(i)}")
-            ux, uy = dataset.get_tensor("ux"), dataset.get_tensor("uy")
-        
-            # analysis/plotting code omitted
-        
-        exp.stop(db)
-        ```
-        
-        For more examples of how to use SmartSim and SmartRedis together to perform
-        online analysis, please see the
-        [online analsysis tutorial section](https://www.craylabs.org/docs/tutorials/online_analysis/lattice/online_analysis.html) of the
-        SmartSim documentation.
-        
-        ## Online Processing
-        
-        Each of the SmartRedis clients can be used to remotely execute
-        [TorchScript](https://pytorch.org/docs/stable/jit.html) code on data
-        stored within the database. The scripts/functions are executed in the Torch
-        runtime linked into the database.
-        
-        Any of the functions available in the
-        [TorchScript builtins](https://pytorch.org/docs/stable/jit_builtin_functions.html#builtin-functions)
-        can be saved as "script" or "functions" in the database and used directly by
-        any of the SmartRedis Clients.
-        
-        ### Singular Value Decomposition
-        
-        For example, the following code sends the built-in
-        [Singular Value Decomposition](https://pytorch.org/docs/stable/generated/torch.svd.html)
-        to the database and execute it on a dummy tensor.
-        
-        ```python
-        import numpy as np
-        from smartredis import Client
-        
-        # don't even need to import torch
-        def calc_svd(input_tensor):
-            return input_tensor.svd()
-        
-        
-        # connect a client to the database
-        client = Client(cluster=False)
-        
-        # get dummy data
-        tensor = np.random.randint(0, 100, size=(5, 3, 2)).astype(np.float32)
-        
-        client.put_tensor("input", tensor)
-        client.set_function("svd", calc_svd)
-        
-        client.run_script("svd", "calc_svd", "input", ["U", "S", "V"])
-        # results are not retrieved immediately in case they need
-        # to be fed to another function/model
-        
-        U = client.get_tensor("U")
-        S = client.get_tensor("S")
-        V = client.get_tensor("V")
-        print(f"U: {U}, S: {S}, V: {V}")
-        ```
-        
-        The processing capabilities make it simple to form computational pipelines of
-        functions, scripts, and models.
-        
-        See the full [TorchScript Language Reference](https://pytorch.org/docs/stable/jit.html#torchscript-language)
-        documentation for more information on available methods, functions, and how
-        to create your own.
-        
-        ## Online Inference
-        
-        SmartSim supports the following frameworks for querying Machine Learning models
-        from C, C++, Fortran and Python with the SmartRedis Clients:
-        
-        <table>
-          <thead>
-            <tr>
-              <th style="text-align:center">RedisAI Version</th>
-              <th style="text-align:center">Libraries</th>
-              <th style="text-align:center">Supported Version</th>
-            </tr>
-          </thead>
-          <tbody style="text-align:center">
-            <tr>
-              <td rowspan="3">1.2.7</td>
-              <td>PyTorch</td>
-              <td>2.0.1</td>
-            </tr>
-            <tr>
-              <td>TensorFlow\Keras</td>
-              <td>2.13.1</td>
-            </tr>
-            <tr>
-              <td>ONNX</td>
-              <td>1.14.1</td>
-            </tr>
-          </tbody>
-        </table>
-        
-        A [number of other libraries](https://github.com/onnx/onnxmltools) are
-        supported through ONNX, like [SciKit-Learn](https://github.com/onnx/sklearn-onnx/)
-        and [XGBoost](https://github.com/onnx/onnxmltools/tree/master/tests/xgboost).
-        
-        **Note:** It's important to remember that SmartSim utilizes a client-server model. To run
-        experiments that utilize the above frameworks, you must first start the Orchestrator
-        database with SmartSim.
-        
-        ### PyTorch CNN Example
-        
-        The example below shows how to spin up a database with SmartSim and
-        invoke a PyTorch CNN model using the SmartRedis clients.
-        
-        ```python
-        # simple_torch_inference.py
-        import io
-        import torch
-        import torch.nn as nn
-        from smartredis import Client
-        from smartsim import Experiment
-        
-        exp = Experiment("simple-online-inference", launcher="local")
-        db = exp.create_database(port=6780, interface="lo")
-        
-        class Net(nn.Module):
-            def __init__(self):
-                super().__init__()
-                self.conv = nn.Conv2d(1, 1, 3)
-        
-            def forward(self, x):
-                return self.conv(x)
-        
-        torch_model = Net()
-        example_forward_input = torch.rand(1, 1, 3, 3)
-        module = torch.jit.trace(torch_model, example_forward_input)
-        model_buffer = io.BytesIO()
-        torch.jit.save(module, model_buffer)
-        
-        exp.start(db, summary=True)
-        
-        address = db.get_address()[0]
-        client = Client(address=address, cluster=False)
-        
-        client.put_tensor("input", example_forward_input.numpy())
-        client.set_model("cnn", model_buffer.getvalue(), "TORCH", device="CPU")
-        client.run_model("cnn", inputs=["input"], outputs=["output"])
-        output = client.get_tensor("output")
-        print(f"Prediction: {output}")
-        
-        exp.stop(db)
-        ```
-        
-        The above python code can be run like any normal python script:
-        ```bash
-        python simple_torch_inference.py
-        ```
-        
-        For more examples of how to use SmartSim and SmartRedis together to perform
-        online inference, please see the
-        [online inference tutorials section](https://www.craylabs.org/docs/tutorials/ml_inference/Inference-in-SmartSim.html) of the
-        SmartSim documentation.
-        
-        --------
-        
-        # Publications
-        
-        The following are public presentations or publications using SmartSim
-        
-         - [Collaboration with NCAR - CGD Seminar](https://www.youtube.com/watch?v=2e-5j427AS0)
-         - [SmartSim: Using Machine Learning in HPC Simulations](https://arxiv.org/abs/2104.09355)
-         - [SmartSim: Online Analytics and Machine Learning for HPC Simulations](https://www.youtube.com/watch?v=JsSgq-fq44w&list=PLuQQBBQFfpgq0OvjKbjcYgTDzDxTqtwua&index=11)
-         - [PyTorch Ecosystem Day Poster](https://assets.pytorch.org/pted2021/posters/J8.png)
-        
-        
-        --------
-        # Cite
-        
-        Please use the following citation when referencing SmartSim, SmartRedis, or any SmartSim related work:
-        
-        Partee et al., “Using Machine Learning at Scale in HPC Simulations with SmartSim:
-        An Application to Ocean Climate Modeling”, Journal of Computational Science, Volume 62, 2022, 101707, ISSN 1877-7503
-        
-        Available: https://doi.org/10.1016/j.jocs.2022.101707.
-        
-        ## bibtex
-        
-        
-        ```latex
-        @article{PARTEE2022101707,
-            title = {Using Machine Learning at scale in numerical simulations with SmartSim: An application to ocean climate modeling},
-            journal = {Journal of Computational Science},
-            volume = {62},
-            pages = {101707},
-            year = {2022},
-            issn = {1877-7503},
-            doi = {https://doi.org/10.1016/j.jocs.2022.101707},
-            url = {https://www.sciencedirect.com/science/article/pii/S1877750322001065},
-            author = {Sam Partee and Matthew Ellis and Alessandro Rigazzi and Andrew E. Shao and Scott Bachman and Gustavo Marques and Benjamin Robbins},
-            keywords = {Deep learning, Numerical simulation, Climate modeling, High performance computing, SmartSim},
-        }
-        ```
-        
-Keywords: scientific,ai,workflow,hpc,analysis
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: <3.12,>=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: mypy
-Provides-Extra: ml
+
+
+<div align="center">
+    <a href="https://github.com/CrayLabs/SmartSim"><img src="https://raw.githubusercontent.com/CrayLabs/SmartSim/master/doc/images/SmartSim_Large.png" width="90%"><img></a>
+    <br />
+    <br />
+<div display="inline-block">
+    <a href="https://github.com/CrayLabs/SmartSim"><b>Home</b></a>&nbsp;&nbsp;&nbsp;
+    <a href="https://www.craylabs.org/docs/installation_instructions/basic.html"><b>Install</b></a>&nbsp;&nbsp;&nbsp;
+    <a href="https://www.craylabs.org/docs/overview.html"><b>Documentation</b></a>&nbsp;&nbsp;&nbsp;
+    <a href="https://github.com/CrayLabs"><b>Cray Labs</b></a>&nbsp;&nbsp;&nbsp;
+    <a href="mailto:craylabs@hpe.com"><b>Contact</b></a>&nbsp;&nbsp;&nbsp;
+    <a href="https://join.slack.com/t/craylabs/shared_invite/zt-nw3ag5z5-5PS4tIXBfufu1bIvvr71UA"><b>Join us on Slack!</b></a>&nbsp;&nbsp;&nbsp;
+  </div>
+    <br />
+    <br />
+</div>
+
+
+<div align="center">
+
+[![License](https://img.shields.io/github/license/CrayLabs/SmartSim)](https://github.com/CrayLabs/SmartSim/blob/master/LICENSE.md)
+![GitHub last commit](https://img.shields.io/github/last-commit/CrayLabs/SmartSim)
+![GitHub deployments](https://img.shields.io/github/deployments/CrayLabs/SmartSim/github-pages?label=doc%20build)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/smartsim)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/smartsim)
+![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/CrayLabs/SmartSim)
+![Language](https://img.shields.io/github/languages/top/CrayLabs/SmartSim)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![codecov](https://codecov.io/gh/CrayLabs/SmartSim/branch/develop/graph/badge.svg?token=96HFI2F45E)](https://codecov.io/gh/CrayLabs/SmartSim)
+[![Downloads](https://static.pepy.tech/personalized-badge/smartsim?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/smartsim)
+
+</div>
+
+------------
+
+# SmartSim
+
+SmartSim is made up of two parts
+  1. SmartSim Infrastructure Library (This repository)
+  2. [SmartRedis](https://github.com/CrayLabs/SmartRedis)
+
+The two library components are designed to work together, but can also be used
+independently.
+
+*SmartSim* is a workflow library that makes it easier to use common Machine Learning (ML)
+libraries, like PyTorch and TensorFlow, in High Performance Computing (HPC) simulations
+and applications. SmartSim launches ML infrastructure on HPC systems alongside user
+workloads.
+
+*SmartRedis* provides an API to connect HPC workloads, particularly (MPI + X) simulations,
+to the ML infrastructure, namely the The [Orchestrator database](https://www.craylabs.org/docs/orchestrator.html),
+launched by SmartSim.
+
+Applications integrated with the SmartRedis clients, written in Fortran, C, C++ and Python,
+can send data to and remotely request SmartSim infrastructure to execute ML models and scripts
+on GPU or CPU. The distributed Client-Server paradigm allows for data to be seamlessly
+exchanged between applications at runtime without the utilization of MPI.
+
+----------
+
+**Table of Contents**
+- [SmartSim](#smartsim)
+- [Quick Start](#quick-start)
+- [SmartSim Infrastructure Library](#smartsim-infrastructure-library)
+  - [Experiments](#experiments)
+    - [Hello World](#hello-world)
+    - [Hello World MPI](#hello-world-mpi)
+  - [Experiments on HPC Systems](#experiments-on-hpc-systems)
+    - [Interactive Launch Example](#interactive-launch-example)
+    - [Batch Launch Examples](#batch-launch-examples)
+- [Infrastructure Library Applications](#infrastructure-library-applications)
+  - [Redis + RedisAI](#redis--redisai)
+    - [Local Launch](#local-launch)
+    - [Interactive Launch](#interactive-launch)
+    - [Batch Launch](#batch-launch)
+- [SmartRedis](#smartredis)
+  - [Tensors](#tensors)
+  - [Datasets](#datasets)
+- [SmartSim + SmartRedis Tutorials](#smartsim--smartredis-tutorials)
+  - [Run the Tutorials](#run-the-tutorials)
+  - [Online Analysis](#online-analysis)
+      - [Lattice Boltzmann Simulation](#lattice-boltzmann-simulation)
+  - [Online Processing](#online-processing)
+    - [Singular Value Decomposition](#singular-value-decomposition)
+  - [Online Inference](#online-inference)
+    - [PyTorch CNN Example](#pytorch-cnn-example)
+- [Publications](#publications)
+- [Cite](#cite)
+  - [bibtex](#bibtex)
+
+----
+
+# Quick Start
+
+
+The documentation has a number of tutorials that make it easy to get used to SmartSim locally
+before using it on your system. Each tutorial is a Jupyter notebook that can be run through the
+[SmartSim Tutorials docker image](https://github.com/orgs/CrayLabs/packages?repo_name=SmartSim)
+which will run a jupyter lab with the tutorials, SmartSim, and SmartRedis installed.
+
+```bash
+docker pull ghcr.io/craylabs/smartsim-tutorials:latest
+docker run -p 8888:8888 ghcr.io/craylabs/smartsim-tutorials:latest
+# click on link to open jupyter lab
+```
+
+# SmartSim Infrastructure Library
+
+The Infrastructure Library (IL), the ``smartsim`` python package,
+facilitates the launch of Machine Learning and simulation
+workflows. The Python interface of the IL creates, configures, launches and monitors
+applications.
+
+## Experiments
+
+The [Experiment](https://www.craylabs.org/docs/api/smartsim_api.html#experiment) object
+is the main interface of SmartSim. Through the [Experiment](https://www.craylabs.org/docs/api/smartsim_api.html#experiment)
+users can create references to user applications called ``Models``.
+### Hello World
+
+Below is a simple example of a workflow that uses the IL to launch hello world
+program using the local launcher which is designed for laptops and single nodes.
+
+```python
+from smartsim import Experiment
+
+exp = Experiment("simple", launcher="local")
+
+settings = exp.create_run_settings("echo", exe_args="Hello World")
+model = exp.create_model("hello_world", settings)
+
+exp.start(model, block=True)
+print(exp.get_status(model))
+```
+
+### Hello World MPI
+
+The [Experiment.create_run_settings](https://www.craylabs.org/docs/api/smartsim_api.html#smartsim.experiment.Experiment.create_run_settings) method returns a ``RunSettings`` object which
+defines how a model is launched. There are many types of ``RunSettings`` [supported by
+SmartSim](https://www.craylabs.org/docs/api/smartsim_api.html#settings).
+
+ - ``RunSettings``
+ - ``MpirunSettings``
+ - ``SrunSettings``
+ - ``AprunSettings``
+ - ``JsrunSettings``
+
+The following example launches a hello world MPI program using the local launcher
+for single compute node, workstations and laptops.
+
+```Python
+from smartsim import Experiment
+
+exp = Experiment("hello_world", launcher="local")
+mpi_settings = exp.create_run_settings(exe="echo",
+                                       exe_args="Hello World!",
+                                       run_command="mpirun")
+mpi_settings.set_tasks(4)
+
+mpi_model = exp.create_model("hello_world", mpi_settings)
+
+exp.start(mpi_model, block=True)
+print(exp.get_status(model))
+```
+
+If an argument of `run_command="auto"` (the default) is passed to
+`Experiment.create_run_settings`, SmartSim will attempt to find a run command on the
+system with which it has a corresponding `RunSettings` class. If one can be found,
+`Experiment.create_run_settings` will instance and return an object of that type.
+
+
+-----------
+## Experiments on HPC Systems
+
+SmartSim integrates with common HPC schedulers providing batch and interactive
+launch capabilities for all applications:
+
+ - Slurm
+ - LSF
+ - PBSPro
+ - Local (for laptops/single node, no batch)
+
+In addition, on Slurm and PBS systems, [Dragon](https://dragonhpc.github.io/dragon/doc/_build/html/index.html)
+can be used as a launcher. Please refer to the documentation for instructions on
+how to insall it on your system and use it in SmartSim.
+
+
+### Interactive Launch Example
+
+The following launches the same ``hello_world`` model in an interactive allocation.
+
+```bash
+# get interactive allocation (Slurm)
+salloc -N 3 --ntasks-per-node=20 --ntasks 60 --exclusive -t 00:10:00
+
+# get interactive allocation (PBS)
+qsub -l select=3:ncpus=20 -l walltime=00:10:00 -l place=scatter -I -q <queue>
+
+# get interactive allocation (LSF)
+bsub -Is -W 00:10 -nnodes 3 -P <project> $SHELL
+```
+
+This same script will run on a SLURM, PBS, or LSF system as the ``launcher``
+is set to `auto` in the [Experiment](https://www.craylabs.org/docs/api/smartsim_api.html#experiment)
+initialization. The run command like ``mpirun``,
+``aprun`` or ``srun`` will be automatically detected from what is available on the
+system.
+
+```python
+# hello_world.py
+from smartsim import Experiment
+
+exp = Experiment("hello_world_exp", launcher="auto")
+run = exp.create_run_settings(exe="echo", exe_args="Hello World!")
+run.set_tasks(60)
+run.set_tasks_per_node(20)
+
+model = exp.create_model("hello_world", run)
+exp.start(model, block=True, summary=True)
+
+print(exp.get_status(model))
+```
+```bash
+# in interactive terminal
+python hello_world.py
+```
+
+
+This script could also be launched in a batch file instead of an
+interactive terminal. For example, for Slurm:
+
+```bash
+#!/bin/bash
+#SBATCH --exclusive
+#SBATCH --nodes=3
+#SBATCH --ntasks-per-node=20
+#SBATCH --time=00:10:00
+
+python /path/to/hello_world.py
+```
+```bash
+# on Slurm system
+sbatch run_hello_world.sh
+```
+
+
+### Batch Launch Examples
+
+SmartSim can also launch workloads in a batch directly from Python, without the need
+for a batch script. Users can launch groups of ``Model`` instances in a ``Ensemble``.
+
+The following launches 4 replicas of the the same ``hello_world`` model.
+
+```python
+# hello_ensemble.py
+from smartsim import Experiment
+
+exp = Experiment("hello_world_batch", launcher="auto")
+
+# define resources for all ensemble members
+batch = exp.create_batch_settings(nodes=4, time="00:10:00", account="12345-Cray")
+batch.set_queue("premium")
+
+# define how each member should run
+run = exp.create_run_settings(exe="echo", exe_args="Hello World!")
+run.set_tasks(60)
+run.set_tasks_per_node(20)
+
+ensemble = exp.create_ensemble("hello_world",
+                               batch_settings=batch,
+                               run_settings=run,
+                               replicas=4)
+exp.start(ensemble, block=True, summary=True)
+
+print(exp.get_status(ensemble))
+```
+
+```bash
+python hello_ensemble.py
+```
+
+Similar to the interactive example, this same script will run on a SLURM, PBS,
+or LSF system as the ``launcher`` is set to `auto` in the
+[Experiment](https://www.craylabs.org/docs/api/smartsim_api.html#experiment)
+initialization. Local launching does not support batch workloads.
+
+
+--------
+
+# Infrastructure Library Applications
+ - Orchestrator - In-memory data store and Machine Learning Inference (Redis + RedisAI)
+
+## Redis + RedisAI
+
+The ``Orchestrator`` is an in-memory database that utilizes Redis and RedisAI to provide
+a distributed database and access to ML runtimes from Fortran, C, C++ and Python.
+
+SmartSim provides classes that make it simple to launch the database in many
+configurations and optionally form a distributed database cluster. The examples
+below will show how to launch the database. Later in this document we will show
+how to use the database to perform ML inference and processing.
+
+
+### Local Launch
+
+The following script launches a single database using the local launcher.
+
+[Experiment.create_database](https://www.craylabs.org/docs/api/smartsim_api.html#smartsim.experiment.Experiment.create_database)
+will initialize an ``Orchestrator`` instance corresponding to the specified launcher.
+
+```python
+# run_db_local.py
+from smartsim import Experiment
+
+exp = Experiment("local-db", launcher="local")
+db = exp.create_database(port=6780,       # database port
+                         interface="lo")  # network interface to use
+
+# by default, SmartSim never blocks execution after the database is launched.
+exp.start(db)
+
+# launch models, analysis, training, inference sessions, etc
+# that communicate with the database using the SmartRedis clients
+
+# stop the database
+exp.stop(db)
+```
+
+### Interactive Launch
+
+The ``Orchestrator``, like ``Ensemble`` instances, can be launched locally, in interactive
+allocations, or in a batch.
+
+The following example launches a distributed (3 node) database cluster
+in an interactive allocation.
+
+
+```bash
+# get interactive allocation (Slurm)
+salloc -N 3 --ntasks-per-node=1 --exclusive -t 00:10:00
+
+# get interactive allocation (PBS)
+qsub -l select=3:ncpus=1 -l walltime=00:10:00 -l place=scatter -I -q queue
+
+# get interactive allocation (LSF)
+bsub -Is -W 00:10 -nnodes 3 -P project $SHELL
+
+```
+
+```python
+# run_db.py
+from smartsim import Experiment
+
+# auto specified to work across launcher types
+exp = Experiment("db-on-slurm", launcher="auto")
+db_cluster = exp.create_database(db_nodes=3,
+                                 db_port=6780,
+                                 batch=False,
+                                 interface="ipogif0")
+exp.start(db_cluster)
+
+print(f"Orchestrator launched on nodes: {db_cluster.hosts}")
+# launch models, analysis, training, inference sessions, etc
+# that communicate with the database using the SmartRedis clients
+
+exp.stop(db_cluster)
+```
+```bash
+# in interactive terminal
+python run_db.py
+```
+
+### Batch Launch
+
+The ``Orchestrator`` can also be launched in a batch without the need for an interactive allocation.
+SmartSim will create the batch file, submit it to the batch system, and then wait for the database
+to be launched. Users can hit CTRL-C to cancel the launch if needed.
+
+```Python
+# run_db_batch.py
+from smartsim import Experiment
+
+exp = Experiment("batch-db-on-pbs", launcher="auto")
+db_cluster = exp.create_database(db_nodes=3,
+                                 db_port=6780,
+                                 batch=True,
+                                 time="00:10:00",
+                                 interface="ib0",
+                                 account="12345-Cray",
+                                 queue="cl40")
+
+exp.start(db_cluster)
+
+print(f"Orchestrator launched on nodes: {db_cluster.hosts}")
+# launch models, analysis, training, inference sessions, etc
+# that communicate with the database using the SmartRedis clients
+
+exp.stop(db_cluster)
+```
+
+```bash
+python run_db_batch.py
+```
+
+------
+# SmartRedis
+
+The SmartSim IL Clients ([SmartRedis](https://github.com/CrayLabs/SmartRedis))
+are implementations of Redis clients that implement the RedisAI
+API with additions specific to scientific workflows.
+
+SmartRedis clients are available in Fortran, C, C++, and Python.
+Users can seamlessly pull and push data from the Orchestrator from different languages.
+
+## Tensors
+
+Tensors are the fundamental data structure for the SmartRedis clients. The Clients
+use the native array format of the language. For example, in Python, a tensor is
+a NumPy array while the C/C++ clients accept nested and contiguous arrays.
+
+When stored in the database, all tensors are stored in the same format. Hence,
+any language can receive a tensor from the database no matter what supported language
+the array was sent from. This enables applications in different languages to communicate
+numerical data with each other at runtime.
+
+For more information on the tensor data structure, see
+[the documentation](https://www.craylabs.org/docs/sr_data_structures.html#tensor)
+
+## Datasets
+
+Datasets are collections of Tensors and associated metadata. The ``Dataset`` class
+is a user space object that can be created, added to, sent to, and retrieved from
+the Orchestrator.
+
+For an example of how to use the ``Dataset`` class, see the [Online Analysis example](#online-analysis)
+
+For more information on the API, see the
+[API documentation](https://www.craylabs.org/docs/sr_data_structures.html#dataset)
+
+# SmartSim + SmartRedis Tutorials
+
+SmartSim and SmartRedis were designed to work together. When launched through
+SmartSim, applications using the SmartRedis clients are directly connected to
+any Orchestrator launched in the same [Experiment](https://www.craylabs.org/docs/api/smartsim_api.html#experiment).
+
+In this way, a SmartSim [Experiment](https://www.craylabs.org/docs/api/smartsim_api.html#experiment) becomes a driver for coupled ML and Simulation
+workflows. The following are simple examples of how to use SmartSim and SmartRedis
+together.
+
+## Run the Tutorials
+
+Each tutorial is a Jupyter notebook that can be run through the
+[SmartSim Tutorials docker image](https://github.com/orgs/CrayLabs/packages?repo_name=SmartSim)
+which will run a jupyter lab with the tutorials, SmartSim, and SmartRedis installed.
+
+```bash
+docker pull ghcr.io/craylabs/smartsim-tutorials:latest
+docker run -p 8888:8888 ghcr.io/craylabs/smartsim-tutorials:latest
+```
+Each of the following examples can be found in the
+[SmartSim documentation](https://www.craylabs.org/docs/tutorials/getting_started/getting_started.html).
+
+## Online Analysis
+
+Using SmartSim, HPC applications can be monitored in real time by streaming data
+from the application to the database. SmartRedis clients can retrieve the
+data, process, analyze it, and finally store any updated data back to the database for
+use by other clients.
+
+The following is an example of how a user could monitor and analyze a simulation.
+The example here uses the Python client; however, SmartRedis clients are also available
+for C, C++, and Fortran. All SmartRedis clients implement the same API.
+
+The example will produce [this visualization](https://user-images.githubusercontent.com/13009163/127622717-2c9e4cfd-50f4-4d94-88c4-8c05fa2fa616.mp4) while the simulation is running.
+
+#### Lattice Boltzmann Simulation
+
+Using a [Lattice Boltzmann Simulation](https://en.wikipedia.org/wiki/Lattice_Boltzmann_methods),
+this example demonstrates how to use the SmartRedis ``Dataset`` API to stream
+data over the Orchestrator deployed by SmartSim.
+
+The simulation will be composed of two parts: `fv_sim.py` which will generate data from
+the Simulation and store it in the Orchestrator, and `driver.py`
+which will launch the Orchestrator, start `fv_sim.py` and check for data posted to the
+Orchestrator to plot updates in real-time.
+
+The following code highlights the sections of `fv_sim.py` that are responsible for
+transmitting the data needed to plot timesteps of the simulation to the Orchestrator.
+
+```Python
+# fv_sim.py
+from smartredis import Client
+import numpy as np
+
+# initialization code omitted
+
+# save cylinder location to database
+cylinder = (X - x_res/4)**2 + (Y - y_res/2)**2 < (y_res/4)**2 # bool array
+client.put_tensor("cylinder", cylinder.astype(np.int8))
+
+for time_step in range(steps): # simulation loop
+    for i, cx, cy in zip(idxs, cxs, cys):
+        F[:,:,i] = np.roll(F[:,:,i], cx, axis=1)
+        F[:,:,i] = np.roll(F[:,:,i], cy, axis=0)
+
+    bndryF = F[cylinder,:]
+    bndryF = bndryF[:,[0,5,6,7,8,1,2,3,4]]
+
+    rho = np.sum(F, 2)
+    ux  = np.sum(F * cxs, 2) / rho
+    uy  = np.sum(F * cys, 2) / rho
+
+    Feq = np.zeros(F.shape)
+    for i, cx, cy, w in zip(idxs, cxs, cys, weights):
+        Feq[:,:,i] = rho * w * ( 1 + 3*(cx*ux+cy*uy)  + 9*(cx*ux+cy*uy)**2/2 - 3*(ux**2+uy**2)/2 )
+    F += -(1.0/tau) * (F - Feq)
+    F[cylinder,:] = bndryF
+
+    # Create a SmartRedis dataset with vorticity data
+    dataset = Dataset(f"data_{str(time_step)}")
+    dataset.add_tensor("ux", ux)
+    dataset.add_tensor("uy", uy)
+
+    # Put Dataset in db at key "data_{time_step}"
+    client.put_dataset(dataset)
+```
+
+The driver script, `driver.py`, launches the Orchestrator database and runs
+the simulation in a non-blocking fashion. The driver script then uses the SmartRedis
+client to pull the DataSet and plot the vorticity while the simulation is running.
+
+```Python
+# driver.py
+time_steps, seed = 3000, 42
+
+exp = Experiment("finite_volume_simulation", launcher="local")
+
+db = exp.create_database(port=6780,        # database port
+                         interface="lo")   # network interface db should listen on
+
+# create the lb simulation Model reference
+settings = exp.create_run_settings("python",
+                                   exe_args=["fv_sim.py",
+                                             f"--seed={seed}",
+                                             f"--steps={time_steps}"])
+model = exp.create_model("fv_simulation", settings)
+model.attach_generator_files(to_copy="fv_sim.py")
+exp.generate(db, model, overwrite=True)
+
+exp.start(db)
+client = Client(address=db.get_address()[0], cluster=False)
+
+# start simulation (non-blocking)
+exp.start(model, block=False, summary=True)
+
+# poll until simulation starts and then retrieve data
+client.poll_key("cylinder", 200, 100)
+cylinder = client.get_tensor("cylinder").astype(bool)
+
+for i in range(0, time_steps):
+    client.poll_key(f"data_{str(i)}", 10, 1000)
+    dataset = client.get_dataset(f"data_{str(i)}")
+    ux, uy = dataset.get_tensor("ux"), dataset.get_tensor("uy")
+
+    # analysis/plotting code omitted
+
+exp.stop(db)
+```
+
+For more examples of how to use SmartSim and SmartRedis together to perform
+online analysis, please see the
+[online analsysis tutorial section](https://www.craylabs.org/docs/tutorials/online_analysis/lattice/online_analysis.html) of the
+SmartSim documentation.
+
+## Online Processing
+
+Each of the SmartRedis clients can be used to remotely execute
+[TorchScript](https://pytorch.org/docs/stable/jit.html) code on data
+stored within the database. The scripts/functions are executed in the Torch
+runtime linked into the database.
+
+Any of the functions available in the
+[TorchScript builtins](https://pytorch.org/docs/stable/jit_builtin_functions.html#builtin-functions)
+can be saved as "script" or "functions" in the database and used directly by
+any of the SmartRedis Clients.
+
+### Singular Value Decomposition
+
+For example, the following code sends the built-in
+[Singular Value Decomposition](https://pytorch.org/docs/stable/generated/torch.svd.html)
+to the database and execute it on a dummy tensor.
+
+```python
+import numpy as np
+from smartredis import Client
+
+# don't even need to import torch
+def calc_svd(input_tensor):
+    return input_tensor.svd()
+
+
+# connect a client to the database
+client = Client(cluster=False)
+
+# get dummy data
+tensor = np.random.randint(0, 100, size=(5, 3, 2)).astype(np.float32)
+
+client.put_tensor("input", tensor)
+client.set_function("svd", calc_svd)
+
+client.run_script("svd", "calc_svd", "input", ["U", "S", "V"])
+# results are not retrieved immediately in case they need
+# to be fed to another function/model
+
+U = client.get_tensor("U")
+S = client.get_tensor("S")
+V = client.get_tensor("V")
+print(f"U: {U}, S: {S}, V: {V}")
+```
+
+The processing capabilities make it simple to form computational pipelines of
+functions, scripts, and models.
+
+See the full [TorchScript Language Reference](https://pytorch.org/docs/stable/jit.html#torchscript-language)
+documentation for more information on available methods, functions, and how
+to create your own.
+
+## Online Inference
+
+SmartSim supports the following frameworks for querying Machine Learning models
+from C, C++, Fortran and Python with the SmartRedis Clients:
+
+<table>
+  <thead>
+    <tr>
+      <th style="text-align:center">RedisAI Version</th>
+      <th style="text-align:center">Libraries</th>
+      <th style="text-align:center">Supported Version</th>
+    </tr>
+  </thead>
+  <tbody style="text-align:center">
+    <tr>
+      <td rowspan="3">1.2.7</td>
+      <td>PyTorch</td>
+      <td>2.0.1</td>
+    </tr>
+    <tr>
+      <td>TensorFlow\Keras</td>
+      <td>2.13.1</td>
+    </tr>
+    <tr>
+      <td>ONNX</td>
+      <td>1.14.1</td>
+    </tr>
+  </tbody>
+</table>
+
+A [number of other libraries](https://github.com/onnx/onnxmltools) are
+supported through ONNX, like [SciKit-Learn](https://github.com/onnx/sklearn-onnx/)
+and [XGBoost](https://github.com/onnx/onnxmltools/tree/master/tests/xgboost).
+
+**Note:** It's important to remember that SmartSim utilizes a client-server model. To run
+experiments that utilize the above frameworks, you must first start the Orchestrator
+database with SmartSim.
+
+### PyTorch CNN Example
+
+The example below shows how to spin up a database with SmartSim and
+invoke a PyTorch CNN model using the SmartRedis clients.
+
+```python
+# simple_torch_inference.py
+import io
+import torch
+import torch.nn as nn
+from smartredis import Client
+from smartsim import Experiment
+
+exp = Experiment("simple-online-inference", launcher="local")
+db = exp.create_database(port=6780, interface="lo")
+
+class Net(nn.Module):
+    def __init__(self):
+        super().__init__()
+        self.conv = nn.Conv2d(1, 1, 3)
+
+    def forward(self, x):
+        return self.conv(x)
+
+torch_model = Net()
+example_forward_input = torch.rand(1, 1, 3, 3)
+module = torch.jit.trace(torch_model, example_forward_input)
+model_buffer = io.BytesIO()
+torch.jit.save(module, model_buffer)
+
+exp.start(db, summary=True)
+
+address = db.get_address()[0]
+client = Client(address=address, cluster=False)
+
+client.put_tensor("input", example_forward_input.numpy())
+client.set_model("cnn", model_buffer.getvalue(), "TORCH", device="CPU")
+client.run_model("cnn", inputs=["input"], outputs=["output"])
+output = client.get_tensor("output")
+print(f"Prediction: {output}")
+
+exp.stop(db)
+```
+
+The above python code can be run like any normal python script:
+```bash
+python simple_torch_inference.py
+```
+
+For more examples of how to use SmartSim and SmartRedis together to perform
+online inference, please see the
+[online inference tutorials section](https://www.craylabs.org/docs/tutorials/ml_inference/Inference-in-SmartSim.html) of the
+SmartSim documentation.
+
+--------
+
+# Publications
+
+The following are public presentations or publications using SmartSim
+
+ - [Collaboration with NCAR - CGD Seminar](https://www.youtube.com/watch?v=2e-5j427AS0)
+ - [SmartSim: Using Machine Learning in HPC Simulations](https://arxiv.org/abs/2104.09355)
+ - [SmartSim: Online Analytics and Machine Learning for HPC Simulations](https://www.youtube.com/watch?v=JsSgq-fq44w&list=PLuQQBBQFfpgq0OvjKbjcYgTDzDxTqtwua&index=11)
+ - [PyTorch Ecosystem Day Poster](https://assets.pytorch.org/pted2021/posters/J8.png)
+
+
+--------
+# Cite
+
+Please use the following citation when referencing SmartSim, SmartRedis, or any SmartSim related work:
+
+Partee et al., “Using Machine Learning at Scale in HPC Simulations with SmartSim:
+An Application to Ocean Climate Modeling”, Journal of Computational Science, Volume 62, 2022, 101707, ISSN 1877-7503
+
+Available: https://doi.org/10.1016/j.jocs.2022.101707.
+
+## bibtex
+
+
+```latex
+@article{PARTEE2022101707,
+    title = {Using Machine Learning at scale in numerical simulations with SmartSim: An application to ocean climate modeling},
+    journal = {Journal of Computational Science},
+    volume = {62},
+    pages = {101707},
+    year = {2022},
+    issn = {1877-7503},
+    doi = {https://doi.org/10.1016/j.jocs.2022.101707},
+    url = {https://www.sciencedirect.com/science/article/pii/S1877750322001065},
+    author = {Sam Partee and Matthew Ellis and Alessandro Rigazzi and Andrew E. Shao and Scott Bachman and Gustavo Marques and Benjamin Robbins},
+    keywords = {Deep learning, Numerical simulation, Climate modeling, High performance computing, SmartSim},
+}
+```
```

#### html2text {}

```diff
@@ -1,12 +1,7 @@
-Metadata-Version: 2.1 Name: smartsim Version: 0.6.2 Summary: AI Workflows for
-Science Home-page: https://github.com/CrayLabs/SmartSim Author: CrayLabs, a
-Hewlett Packard Enterprise OSS Organization Author-email: craylabs@hpe.com
-License: BSD 2-Clause License Project-URL: Source, https://github.com/CrayLabs/
-SmartSim Project-URL: Documentation, https://www.craylabs.org Description:
     _[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_C_r_a_y_L_a_b_s_/_S_m_a_r_t_S_i_m_/_m_a_s_t_e_r_/_d_o_c_/_i_m_a_g_e_s_/
                           _S_m_a_r_t_S_i_m___L_a_r_g_e_._p_n_g_]_[_I_m_a_g_e_]
 
     _HH_oo_mm_ee    _II_nn_ss_tt_aa_ll_ll    _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn    _CC_rr_aa_yy_ _LL_aa_bb_ss    _CC_oo_nn_tt_aa_cc_tt    _JJ_oo_ii_nn_ _uu_ss_ _oo_nn
                                    _SS_ll_aa_cc_kk_!!   
 
 
@@ -91,61 +86,64 @@
 ("hello_world", mpi_settings) exp.start(mpi_model, block=True) print
 (exp.get_status(model)) ``` If an argument of `run_command="auto"` (the
 default) is passed to `Experiment.create_run_settings`, SmartSim will attempt
 to find a run command on the system with which it has a corresponding
 `RunSettings` class. If one can be found, `Experiment.create_run_settings` will
 instance and return an object of that type. ----------- ## Experiments on HPC
 Systems SmartSim integrates with common HPC schedulers providing batch and
-interactive launch capabilities for all applications. - Slurm - LSF - PBSPro -
-Local (for laptops/single node, no batch) ### Interactive Launch Example The
-following launches the same ``hello_world`` model in an interactive allocation.
-```bash # get interactive allocation (Slurm) salloc -N 3 --ntasks-per-node=20 -
--ntasks 60 --exclusive -t 00:10:00 # get interactive allocation (PBS) qsub -
-l select=3:ncpus=20 -l walltime=00:10:00 -l place=scatter -I -q # get
-interactive allocation (LSF) bsub -Is -W 00:10 -nnodes 3 -P $SHELL ``` This
-same script will run on a SLURM, PBS, or LSF system as the ``launcher`` is set
-to `auto` in the [Experiment](https://www.craylabs.org/docs/api/
-smartsim_api.html#experiment) initialization. The run command like ``mpirun``,
-``aprun`` or ``srun`` will be automatically detected from what is available on
-the system. ```python # hello_world.py from smartsim import Experiment exp =
-Experiment("hello_world_exp", launcher="auto") run = exp.create_run_settings
-(exe="echo", exe_args="Hello World!") run.set_tasks(60) run.set_tasks_per_node
-(20) model = exp.create_model("hello_world", run) exp.start(model, block=True,
-summary=True) print(exp.get_status(model)) ``` ```bash # in interactive
-terminal python hello_world.py ``` This script could also be launched in a
-batch file instead of an interactive terminal. For example, for Slurm: ```bash
-#!/bin/bash #SBATCH --exclusive #SBATCH --nodes=3 #SBATCH --ntasks-per-node=20
-#SBATCH --time=00:10:00 python /path/to/hello_world.py ``` ```bash # on Slurm
-system sbatch run_hello_world.sh ``` ### Batch Launch Examples SmartSim can
-also launch workloads in a batch directly from Python, without the need for a
-batch script. Users can launch groups of ``Model`` instances in a ``Ensemble``.
-The following launches 4 replicas of the the same ``hello_world`` model.
-```python # hello_ensemble.py from smartsim import Experiment exp = Experiment
-("hello_world_batch", launcher="auto") # define resources for all ensemble
-members batch = exp.create_batch_settings(nodes=4, time="00:10:00",
-account="12345-Cray") batch.set_queue("premium") # define how each member
-should run run = exp.create_run_settings(exe="echo", exe_args="Hello World!")
-run.set_tasks(60) run.set_tasks_per_node(20) ensemble = exp.create_ensemble
-("hello_world", batch_settings=batch, run_settings=run, replicas=4) exp.start
-(ensemble, block=True, summary=True) print(exp.get_status(ensemble)) ```
-```bash python hello_ensemble.py ``` Similar to the interactive example, this
-same script will run on a SLURM, PBS, or LSF system as the ``launcher`` is set
-to `auto` in the [Experiment](https://www.craylabs.org/docs/api/
-smartsim_api.html#experiment) initialization. Local launching does not support
-batch workloads. -------- # Infrastructure Library Applications - Orchestrator
-- In-memory data store and Machine Learning Inference (Redis + RedisAI) ##
-Redis + RedisAI The ``Orchestrator`` is an in-memory database that utilizes
-Redis and RedisAI to provide a distributed database and access to ML runtimes
-from Fortran, C, C++ and Python. SmartSim provides classes that make it simple
-to launch the database in many configurations and optionally form a distributed
-database cluster. The examples below will show how to launch the database.
-Later in this document we will show how to use the database to perform ML
-inference and processing. ### Local Launch The following script launches a
-single database using the local launcher. [Experiment.create_database](https://
-www.craylabs.org/docs/api/
+interactive launch capabilities for all applications: - Slurm - LSF - PBSPro -
+Local (for laptops/single node, no batch) In addition, on Slurm and PBS
+systems, [Dragon](https://dragonhpc.github.io/dragon/doc/_build/html/
+index.html) can be used as a launcher. Please refer to the documentation for
+instructions on how to insall it on your system and use it in SmartSim. ###
+Interactive Launch Example The following launches the same ``hello_world``
+model in an interactive allocation. ```bash # get interactive allocation
+(Slurm) salloc -N 3 --ntasks-per-node=20 --ntasks 60 --exclusive -t 00:10:00 #
+get interactive allocation (PBS) qsub -l select=3:ncpus=20 -l walltime=00:10:00
+-l place=scatter -I -q # get interactive allocation (LSF) bsub -Is -W 00:10 -
+nnodes 3 -P $SHELL ``` This same script will run on a SLURM, PBS, or LSF system
+as the ``launcher`` is set to `auto` in the [Experiment](https://
+www.craylabs.org/docs/api/smartsim_api.html#experiment) initialization. The run
+command like ``mpirun``, ``aprun`` or ``srun`` will be automatically detected
+from what is available on the system. ```python # hello_world.py from smartsim
+import Experiment exp = Experiment("hello_world_exp", launcher="auto") run =
+exp.create_run_settings(exe="echo", exe_args="Hello World!") run.set_tasks(60)
+run.set_tasks_per_node(20) model = exp.create_model("hello_world", run)
+exp.start(model, block=True, summary=True) print(exp.get_status(model)) ```
+```bash # in interactive terminal python hello_world.py ``` This script could
+also be launched in a batch file instead of an interactive terminal. For
+example, for Slurm: ```bash #!/bin/bash #SBATCH --exclusive #SBATCH --nodes=3
+#SBATCH --ntasks-per-node=20 #SBATCH --time=00:10:00 python /path/to/
+hello_world.py ``` ```bash # on Slurm system sbatch run_hello_world.sh ``` ###
+Batch Launch Examples SmartSim can also launch workloads in a batch directly
+from Python, without the need for a batch script. Users can launch groups of
+``Model`` instances in a ``Ensemble``. The following launches 4 replicas of the
+the same ``hello_world`` model. ```python # hello_ensemble.py from smartsim
+import Experiment exp = Experiment("hello_world_batch", launcher="auto") #
+define resources for all ensemble members batch = exp.create_batch_settings
+(nodes=4, time="00:10:00", account="12345-Cray") batch.set_queue("premium") #
+define how each member should run run = exp.create_run_settings(exe="echo",
+exe_args="Hello World!") run.set_tasks(60) run.set_tasks_per_node(20) ensemble
+= exp.create_ensemble("hello_world", batch_settings=batch, run_settings=run,
+replicas=4) exp.start(ensemble, block=True, summary=True) print(exp.get_status
+(ensemble)) ``` ```bash python hello_ensemble.py ``` Similar to the interactive
+example, this same script will run on a SLURM, PBS, or LSF system as the
+``launcher`` is set to `auto` in the [Experiment](https://www.craylabs.org/
+docs/api/smartsim_api.html#experiment) initialization. Local launching does not
+support batch workloads. -------- # Infrastructure Library Applications -
+Orchestrator - In-memory data store and Machine Learning Inference (Redis +
+RedisAI) ## Redis + RedisAI The ``Orchestrator`` is an in-memory database that
+utilizes Redis and RedisAI to provide a distributed database and access to ML
+runtimes from Fortran, C, C++ and Python. SmartSim provides classes that make
+it simple to launch the database in many configurations and optionally form a
+distributed database cluster. The examples below will show how to launch the
+database. Later in this document we will show how to use the database to
+perform ML inference and processing. ### Local Launch The following script
+launches a single database using the local launcher.
+[Experiment.create_database](https://www.craylabs.org/docs/api/
 smartsim_api.html#smartsim.experiment.Experiment.create_database) will
 initialize an ``Orchestrator`` instance corresponding to the specified
 launcher. ```python # run_db_local.py from smartsim import Experiment exp =
 Experiment("local-db", launcher="local") db = exp.create_database(port=6780, #
 database port interface="lo") # network interface to use # by default, SmartSim
 never blocks execution after the database is launched. exp.start(db) # launch
 models, analysis, training, inference sessions, etc # that communicate with the
@@ -332,15 +330,8 @@
 simulations with SmartSim: An application to ocean climate modeling}, journal =
 {Journal of Computational Science}, volume = {62}, pages = {101707}, year =
 {2022}, issn = {1877-7503}, doi = {https://doi.org/10.1016/j.jocs.2022.101707},
 url = {https://www.sciencedirect.com/science/article/pii/S1877750322001065},
 author = {Sam Partee and Matthew Ellis and Alessandro Rigazzi and Andrew E.
 Shao and Scott Bachman and Gustavo Marques and Benjamin Robbins}, keywords =
 {Deep learning, Numerical simulation, Climate modeling, High performance
-computing, SmartSim}, } ``` Keywords: scientific,ai,workflow,hpc,analysis
-Platform: UNKNOWN Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-License :: OSI Approved :: BSD License Classifier: Intended Audience ::
-Science/Research Classifier: Topic :: Scientific/Engineering Requires-Python:
-<3.12,>=3.8 Description-Content-Type: text/markdown Provides-Extra: dev
-Provides-Extra: mypy Provides-Extra: ml
+computing, SmartSim}, } ```
```

### Comparing `smartsim-0.6.2/README.md` & `smartsim-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: smartsim
+Version: 0.7.0
+Summary: AI Workflows for Science
+Home-page: https://github.com/CrayLabs/SmartSim
+Author: CrayLabs, a Hewlett Packard Enterprise OSS Organization
+Author-email: craylabs@hpe.com
+License: BSD 2-Clause License
+Project-URL: Source, https://github.com/CrayLabs/SmartSim
+Project-URL: Documentation, https://www.craylabs.org
+Keywords: scientific,ai,workflow,hpc,analysis
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: <3.12,>=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: mypy
+Provides-Extra: ml
+License-File: LICENSE.md
+
 
 
 <div align="center">
     <a href="https://github.com/CrayLabs/SmartSim"><img src="https://raw.githubusercontent.com/CrayLabs/SmartSim/master/doc/images/SmartSim_Large.png" width="90%"><img></a>
     <br />
     <br />
 <div display="inline-block">
@@ -170,21 +195,25 @@
 `Experiment.create_run_settings` will instance and return an object of that type.
 
 
 -----------
 ## Experiments on HPC Systems
 
 SmartSim integrates with common HPC schedulers providing batch and interactive
-launch capabilities for all applications.
+launch capabilities for all applications:
 
  - Slurm
  - LSF
  - PBSPro
  - Local (for laptops/single node, no batch)
 
+In addition, on Slurm and PBS systems, [Dragon](https://dragonhpc.github.io/dragon/doc/_build/html/index.html)
+can be used as a launcher. Please refer to the documentation for instructions on
+how to insall it on your system and use it in SmartSim.
+
 
 ### Interactive Launch Example
 
 The following launches the same ``hello_world`` model in an interactive allocation.
 
 ```bash
 # get interactive allocation (Slurm)
@@ -749,7 +778,9 @@
     issn = {1877-7503},
     doi = {https://doi.org/10.1016/j.jocs.2022.101707},
     url = {https://www.sciencedirect.com/science/article/pii/S1877750322001065},
     author = {Sam Partee and Matthew Ellis and Alessandro Rigazzi and Andrew E. Shao and Scott Bachman and Gustavo Marques and Benjamin Robbins},
     keywords = {Deep learning, Numerical simulation, Climate modeling, High performance computing, SmartSim},
 }
 ```
+
+
```

#### html2text {}

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1 Name: smartsim Version: 0.7.0 Summary: AI Workflows for
+Science Home-page: https://github.com/CrayLabs/SmartSim Author: CrayLabs, a
+Hewlett Packard Enterprise OSS Organization Author-email: craylabs@hpe.com
+License: BSD 2-Clause License Project-URL: Source, https://github.com/CrayLabs/
+SmartSim Project-URL: Documentation, https://www.craylabs.org Keywords:
+scientific,ai,workflow,hpc,analysis Platform: UNKNOWN Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
+Approved :: BSD License Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering Requires-Python: <3.12,>=3.9
+Description-Content-Type: text/markdown Provides-Extra: dev Provides-Extra:
+mypy Provides-Extra: ml License-File: LICENSE.md
     _[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_C_r_a_y_L_a_b_s_/_S_m_a_r_t_S_i_m_/_m_a_s_t_e_r_/_d_o_c_/_i_m_a_g_e_s_/
                           _S_m_a_r_t_S_i_m___L_a_r_g_e_._p_n_g_]_[_I_m_a_g_e_]
 
     _HH_oo_mm_ee    _II_nn_ss_tt_aa_ll_ll    _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn    _CC_rr_aa_yy_ _LL_aa_bb_ss    _CC_oo_nn_tt_aa_cc_tt    _JJ_oo_ii_nn_ _uu_ss_ _oo_nn
                                    _SS_ll_aa_cc_kk_!!   
 
 
@@ -86,61 +98,64 @@
 ("hello_world", mpi_settings) exp.start(mpi_model, block=True) print
 (exp.get_status(model)) ``` If an argument of `run_command="auto"` (the
 default) is passed to `Experiment.create_run_settings`, SmartSim will attempt
 to find a run command on the system with which it has a corresponding
 `RunSettings` class. If one can be found, `Experiment.create_run_settings` will
 instance and return an object of that type. ----------- ## Experiments on HPC
 Systems SmartSim integrates with common HPC schedulers providing batch and
-interactive launch capabilities for all applications. - Slurm - LSF - PBSPro -
-Local (for laptops/single node, no batch) ### Interactive Launch Example The
-following launches the same ``hello_world`` model in an interactive allocation.
-```bash # get interactive allocation (Slurm) salloc -N 3 --ntasks-per-node=20 -
--ntasks 60 --exclusive -t 00:10:00 # get interactive allocation (PBS) qsub -
-l select=3:ncpus=20 -l walltime=00:10:00 -l place=scatter -I -q # get
-interactive allocation (LSF) bsub -Is -W 00:10 -nnodes 3 -P $SHELL ``` This
-same script will run on a SLURM, PBS, or LSF system as the ``launcher`` is set
-to `auto` in the [Experiment](https://www.craylabs.org/docs/api/
-smartsim_api.html#experiment) initialization. The run command like ``mpirun``,
-``aprun`` or ``srun`` will be automatically detected from what is available on
-the system. ```python # hello_world.py from smartsim import Experiment exp =
-Experiment("hello_world_exp", launcher="auto") run = exp.create_run_settings
-(exe="echo", exe_args="Hello World!") run.set_tasks(60) run.set_tasks_per_node
-(20) model = exp.create_model("hello_world", run) exp.start(model, block=True,
-summary=True) print(exp.get_status(model)) ``` ```bash # in interactive
-terminal python hello_world.py ``` This script could also be launched in a
-batch file instead of an interactive terminal. For example, for Slurm: ```bash
-#!/bin/bash #SBATCH --exclusive #SBATCH --nodes=3 #SBATCH --ntasks-per-node=20
-#SBATCH --time=00:10:00 python /path/to/hello_world.py ``` ```bash # on Slurm
-system sbatch run_hello_world.sh ``` ### Batch Launch Examples SmartSim can
-also launch workloads in a batch directly from Python, without the need for a
-batch script. Users can launch groups of ``Model`` instances in a ``Ensemble``.
-The following launches 4 replicas of the the same ``hello_world`` model.
-```python # hello_ensemble.py from smartsim import Experiment exp = Experiment
-("hello_world_batch", launcher="auto") # define resources for all ensemble
-members batch = exp.create_batch_settings(nodes=4, time="00:10:00",
-account="12345-Cray") batch.set_queue("premium") # define how each member
-should run run = exp.create_run_settings(exe="echo", exe_args="Hello World!")
-run.set_tasks(60) run.set_tasks_per_node(20) ensemble = exp.create_ensemble
-("hello_world", batch_settings=batch, run_settings=run, replicas=4) exp.start
-(ensemble, block=True, summary=True) print(exp.get_status(ensemble)) ```
-```bash python hello_ensemble.py ``` Similar to the interactive example, this
-same script will run on a SLURM, PBS, or LSF system as the ``launcher`` is set
-to `auto` in the [Experiment](https://www.craylabs.org/docs/api/
-smartsim_api.html#experiment) initialization. Local launching does not support
-batch workloads. -------- # Infrastructure Library Applications - Orchestrator
-- In-memory data store and Machine Learning Inference (Redis + RedisAI) ##
-Redis + RedisAI The ``Orchestrator`` is an in-memory database that utilizes
-Redis and RedisAI to provide a distributed database and access to ML runtimes
-from Fortran, C, C++ and Python. SmartSim provides classes that make it simple
-to launch the database in many configurations and optionally form a distributed
-database cluster. The examples below will show how to launch the database.
-Later in this document we will show how to use the database to perform ML
-inference and processing. ### Local Launch The following script launches a
-single database using the local launcher. [Experiment.create_database](https://
-www.craylabs.org/docs/api/
+interactive launch capabilities for all applications: - Slurm - LSF - PBSPro -
+Local (for laptops/single node, no batch) In addition, on Slurm and PBS
+systems, [Dragon](https://dragonhpc.github.io/dragon/doc/_build/html/
+index.html) can be used as a launcher. Please refer to the documentation for
+instructions on how to insall it on your system and use it in SmartSim. ###
+Interactive Launch Example The following launches the same ``hello_world``
+model in an interactive allocation. ```bash # get interactive allocation
+(Slurm) salloc -N 3 --ntasks-per-node=20 --ntasks 60 --exclusive -t 00:10:00 #
+get interactive allocation (PBS) qsub -l select=3:ncpus=20 -l walltime=00:10:00
+-l place=scatter -I -q # get interactive allocation (LSF) bsub -Is -W 00:10 -
+nnodes 3 -P $SHELL ``` This same script will run on a SLURM, PBS, or LSF system
+as the ``launcher`` is set to `auto` in the [Experiment](https://
+www.craylabs.org/docs/api/smartsim_api.html#experiment) initialization. The run
+command like ``mpirun``, ``aprun`` or ``srun`` will be automatically detected
+from what is available on the system. ```python # hello_world.py from smartsim
+import Experiment exp = Experiment("hello_world_exp", launcher="auto") run =
+exp.create_run_settings(exe="echo", exe_args="Hello World!") run.set_tasks(60)
+run.set_tasks_per_node(20) model = exp.create_model("hello_world", run)
+exp.start(model, block=True, summary=True) print(exp.get_status(model)) ```
+```bash # in interactive terminal python hello_world.py ``` This script could
+also be launched in a batch file instead of an interactive terminal. For
+example, for Slurm: ```bash #!/bin/bash #SBATCH --exclusive #SBATCH --nodes=3
+#SBATCH --ntasks-per-node=20 #SBATCH --time=00:10:00 python /path/to/
+hello_world.py ``` ```bash # on Slurm system sbatch run_hello_world.sh ``` ###
+Batch Launch Examples SmartSim can also launch workloads in a batch directly
+from Python, without the need for a batch script. Users can launch groups of
+``Model`` instances in a ``Ensemble``. The following launches 4 replicas of the
+the same ``hello_world`` model. ```python # hello_ensemble.py from smartsim
+import Experiment exp = Experiment("hello_world_batch", launcher="auto") #
+define resources for all ensemble members batch = exp.create_batch_settings
+(nodes=4, time="00:10:00", account="12345-Cray") batch.set_queue("premium") #
+define how each member should run run = exp.create_run_settings(exe="echo",
+exe_args="Hello World!") run.set_tasks(60) run.set_tasks_per_node(20) ensemble
+= exp.create_ensemble("hello_world", batch_settings=batch, run_settings=run,
+replicas=4) exp.start(ensemble, block=True, summary=True) print(exp.get_status
+(ensemble)) ``` ```bash python hello_ensemble.py ``` Similar to the interactive
+example, this same script will run on a SLURM, PBS, or LSF system as the
+``launcher`` is set to `auto` in the [Experiment](https://www.craylabs.org/
+docs/api/smartsim_api.html#experiment) initialization. Local launching does not
+support batch workloads. -------- # Infrastructure Library Applications -
+Orchestrator - In-memory data store and Machine Learning Inference (Redis +
+RedisAI) ## Redis + RedisAI The ``Orchestrator`` is an in-memory database that
+utilizes Redis and RedisAI to provide a distributed database and access to ML
+runtimes from Fortran, C, C++ and Python. SmartSim provides classes that make
+it simple to launch the database in many configurations and optionally form a
+distributed database cluster. The examples below will show how to launch the
+database. Later in this document we will show how to use the database to
+perform ML inference and processing. ### Local Launch The following script
+launches a single database using the local launcher.
+[Experiment.create_database](https://www.craylabs.org/docs/api/
 smartsim_api.html#smartsim.experiment.Experiment.create_database) will
 initialize an ``Orchestrator`` instance corresponding to the specified
 launcher. ```python # run_db_local.py from smartsim import Experiment exp =
 Experiment("local-db", launcher="local") db = exp.create_database(port=6780, #
 database port interface="lo") # network interface to use # by default, SmartSim
 never blocks execution after the database is launched. exp.start(db) # launch
 models, analysis, training, inference sessions, etc # that communicate with the
```

### Comparing `smartsim-0.6.2/pyproject.toml` & `smartsim-0.7.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -27,44 +27,52 @@
 
 [build-system]
 requires = ["setuptools", "wheel", "cmake>=3.13"]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 88
-target-version = ['py38', 'py39', 'py310']
+target-version = ['py39', 'py310', 'py311']
 exclude = '''
 (
   | \.egg
   | \.git
   | \.hg
   | \.mypy_cache
   | \.nox
   | \.tox
   | \.venv
   | _build
   | build
   | dist
   | setup.py
+  | .*\.py
 )
 '''
+force-exclude = '''
+(
+  .*\.dragon/*
+)
+'''
+
 
 [tool.pytest.ini_options]
 log_cli = true
 log_cli_level = "debug"
 markers = [
   "group_a: fast test subset a",
   "group_b: fast test subset b",
   "slow_tests: tests that take a long duration to complete",
 ]
 
 [tool.isort]
 # supress circular import warning
 profile = "black"
 skip = ["tests/test_configs/circular_config"]
+skip_glob="smartsim/_core/.dragon/*"
 
 [tool.coverage.run]
 source = ["smartsim"]
 # see test_configs/*_cov.cfg for "omit"
 
 [tool.coverage.report]
 ignore_errors = true
@@ -74,15 +82,15 @@
 directory = "htmlcov"
 
 [tool.mypy]
 namespace_packages = true
 files = [
   "smartsim"
 ]
-plugins = []
+plugins = ["pydantic.mypy"]
 ignore_errors = false
 
 # Dynamic typing
 disallow_any_generics = true
 warn_return_any = true
 
 # Strict fn defs
@@ -103,25 +111,28 @@
 # Misc Strictness Settings
 strict_concatenate = false
 strict_equality = true
 
 # Additional Error Codes
 enable_error_code = [
     # "redundant-expr",
-    # "possibly-undefined",
+    "possibly-undefined",
     # "unused-awaitable",
     # "ignore-without-code",
     # "mutable-override",
+    "truthy-bool",
+    "truthy-iterable",
 ]
 
 [[tool.mypy.overrides]]
 # Ignore packages that are not used or not typed
 module = [
   "coloredlogs",
   "redis.cluster",
   "keras",
   "torch",
   "smartsim.ml.torch.*",            # must solve/ignore inheritance issues
   "watchdog",
+  "dragon.*",
 ]
 ignore_missing_imports = true
 ignore_errors = true
```

### Comparing `smartsim-0.6.2/setup.cfg` & `smartsim-0.7.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -10,35 +10,35 @@
 author = CrayLabs, a Hewlett Packard Enterprise OSS Organization
 author_email = craylabs@hpe.com
 contact = CrayLabs, a Hewlett Packard Enterprise OSS Organization
 contact_email = craylabs@hpe.com
 license = BSD 2-Clause License
 keywords = scientific, ai, workflow, hpc, analysis
 classifiers = 
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: BSD License
 	Intended Audience :: Science/Research
 	Topic :: Scientific/Engineering
 
 [options]
 packages = find:
 setup_requires = 
 	setuptools>=39.2
 	cmake>=3.13
 include_package_data = True
-python_requires = >=3.8,<3.12
+python_requires = >=3.9,<3.12
 
 [options.packages.find]
 include = 
 	smartsim*
 exclude = 
 	.third-party
+	.dragon
 	tests
 	doc
 	smartredis
 
 [options.package_data]
 smartsim = 
 	py.typed
```

### Comparing `smartsim-0.6.2/setup.py` & `smartsim-0.7.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,29 +60,30 @@
 #  if set, the version number is set to a developer build
 #  with the current version, git-sha, and suffix. This version
 #  is then written into SmartSim/smartsim/version.py
 #
 #
 # This future is needed to print Python2 EOL message
 from __future__ import print_function
+
 import sys
 
 if sys.version_info < (3,):
     print("Python 2 has reached end-of-life and is not supported by SmartSim")
     sys.exit(-1)
 
 
-import os
 import importlib.util
+import os
 from pathlib import Path
 
 from setuptools import setup
-from setuptools.dist import Distribution
-from setuptools.command.install import install
 from setuptools.command.build_py import build_py
+from setuptools.command.install import install
+from setuptools.dist import Distribution
 
 # Some necessary evils we have to do to be able to use
 # the _install tools in smartsim/smartsim/_core/_install
 # in both the setup.py and in the smart cli
 
 # import the installer classes
 setup_path = Path(os.path.abspath(os.path.dirname(__file__)))
@@ -103,101 +104,111 @@
 # helper classes for building dependencies that are
 # also utilized by the Smart CLI
 build_env = buildenv.BuildEnv(checks=False)
 versions = buildenv.Versioner()
 
 # check for compatible python versions
 if not build_env.is_compatible_python(versions.PYTHON_MIN):
-    print("You are using Python {}. Python >={} is required.".format(build_env.python_version,
-                                                                     ".".join((versions.PYTHON_MIN))))
+    print(
+        "You are using Python {}. Python >={} is required.".format(
+            build_env.python_version, ".".join((versions.PYTHON_MIN))
+        )
+    )
     sys.exit(-1)
 
 if build_env.is_windows():
     print("Windows is not supported by SmartSim")
     sys.exit(-1)
 
 # write the SmartSim version into
 # smartsim/version.py and to be set as
 # __version__ in smartsim/__init__.py
 smartsim_version = versions.write_version(setup_path)
 
+
 class BuildError(Exception):
     pass
 
+
 # Hacky workaround for solving CI build "purelib" issue
 # see https://github.com/google/or-tools/issues/616
 class InstallPlatlib(install):
     def finalize_options(self):
         super().finalize_options()
         if self.distribution.has_ext_modules():
             self.install_lib = self.install_platlib
 
-class SmartSimBuild(build_py):
 
+class SmartSimBuild(build_py):
     def run(self):
-        database_builder = builder.DatabaseBuilder(build_env(),
-                                             build_env.MALLOC,
-                                             build_env.JOBS)
+        database_builder = builder.DatabaseBuilder(
+            build_env(), build_env.MALLOC, build_env.JOBS
+        )
         if not database_builder.is_built:
-            database_builder.build_from_git(versions.REDIS_URL,
-                                         versions.REDIS)
+            database_builder.build_from_git(versions.REDIS_URL, versions.REDIS)
 
             database_builder.cleanup()
 
         # run original build_py command
         super().run()
 
 
 # Tested with wheel v0.29.0
 class BinaryDistribution(Distribution):
     """Distribution which always forces a binary package with platform name
 
-       We use this because we want to pre-package Redis for certain
-       platforms to use.
+    We use this because we want to pre-package Redis for certain
+    platforms to use.
     """
+
     def has_ext_modules(_placeholder):
         return True
 
 
 # Define needed dependencies for the installation
 deps = [
     "psutil>=5.7.2",
     "coloredlogs>=10.0",
     "tabulate>=0.8.9",
     "redis>=4.5",
     "tqdm>=4.50.2",
     "filelock>=3.4.2",
     "protobuf~=3.20",
-    "watchdog>=3.0.0,<4.0.0",
+    "jinja2>=3.1.2",
+    "watchdog>=4.0.0",
+    "pydantic==1.10.14",
+    "pyzmq>=25.1.2",
+    "pygithub>=2.3.0",
 ]
 
 # Add SmartRedis at specific version
 deps.append("smartredis>={}".format(versions.SMARTREDIS))
 
 extras_require = {
     "dev": [
         "black==24.1a1",
         "isort>=5.6.4",
         "pylint>=2.10.0,<3",
         "pytest>=6.0.0",
         "pytest-cov>=2.10.1",
         "click==8.0.2",
+        "pytest-asyncio>=0.23.3",
     ],
     "mypy": [
         "mypy>=1.3.0",
         "types-psutil",
         "types-redis",
         "types-tabulate",
         "types-tqdm",
         "types-tensorflow==2.12.0.9",
         "types-setuptools",
         "typing_extensions>=4.1.0",
     ],
     # see smartsim/_core/_install/buildenv.py for more details
-    **versions.ml_extras_required()
+    **versions.ml_extras_required(),
 }
 
 
 # rest in setup.cfg
 setup(
     version=smartsim_version,
     install_requires=deps,
@@ -208,9 +219,9 @@
     zip_safe=False,
     extras_require=extras_require,
     distclass=BinaryDistribution,
     entry_points={
         "console_scripts": [
             "smart = smartsim._core._cli.__main__:main",
         ]
-    }
+    },
 )
```

### Comparing `smartsim-0.6.2/smartsim/__init__.py` & `smartsim-0.7.0/smartsim/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,13 +26,13 @@
 
 import sys
 
 # -*- coding: utf-8 -*-
 # pylint: disable-next=useless-import-alias
 from .version import __version__ as __version__
 
-if sys.version_info < (3, 8):  # pragma: no cover
-    sys.exit("Python 3.8 or greater must be used with SmartSim.")
+if sys.version_info < (3, 9):  # pragma: no cover
+    sys.exit("Python 3.9 or greater must be used with SmartSim.")
 
 # Main API module
 # pylint: disable=wrong-import-position
 from .experiment import Experiment
```

### Comparing `smartsim-0.6.2/smartsim/_core/__init__.py` & `smartsim-0.7.0/smartsim/_core/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,11 +20,11 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from .control import Controller, Manifest
+from .control import Controller, Manifest, previewrenderer
 from .generation import Generator
 
-__all__ = ["Controller", "Manifest", "Generator"]
+__all__ = ["Controller", "Manifest", "Generator", "previewrenderer"]
```

### Comparing `smartsim-0.6.2/smartsim/_core/_cli/__init__.py` & `smartsim-0.7.0/smartsim/_core/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.6.2/smartsim/_core/_cli/__main__.py` & `smartsim-0.7.0/smartsim/_core/_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.6.2/smartsim/_core/_cli/build.py` & `smartsim-0.7.0/smartsim/_core/_cli/build.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,37 +29,36 @@
 import platform
 import sys
 import typing as t
 from pathlib import Path
 
 from tabulate import tabulate
 
+from smartsim._core._cli.scripts.dragon_install import install_dragon
 from smartsim._core._cli.utils import SMART_LOGGER_FORMAT, color_bool, pip
 from smartsim._core._install import builder
 from smartsim._core._install.buildenv import (
     BuildEnv,
     DbEngine,
     SetupError,
     Version_,
     VersionConflictError,
     Versioner,
 )
-from smartsim._core._install.builder import BuildError
+from smartsim._core._install.builder import BuildError, Device
 from smartsim._core.config import CONFIG
 from smartsim._core.utils.helpers import installed_redisai_backends
 from smartsim.error import SSConfigError
 from smartsim.log import get_logger
 
 logger = get_logger("Smart", fmt=SMART_LOGGER_FORMAT)
 
 # NOTE: all smartsim modules need full paths as the smart cli
 #       may be installed into a different directory.
 
-
-_TDeviceStr = t.Literal["cpu", "gpu"]
 _TPinningStr = t.Literal["==", "!=", ">=", ">", "<=", "<", "~="]
 
 
 def check_py_onnx_version(versions: Versioner) -> None:
     """Check Python environment for ONNX installation"""
     _check_packages_in_python_env(
         {
@@ -130,35 +129,36 @@
         database_builder.cleanup()
     logger.info(f"{database_name} build complete!")
 
 
 def build_redis_ai(
     build_env: BuildEnv,
     versions: Versioner,
-    device: _TDeviceStr,
+    device: Device,
     use_torch: bool = True,
     use_tf: bool = True,
     use_onnx: bool = False,
     torch_dir: t.Union[str, Path, None] = None,
     libtf_dir: t.Union[str, Path, None] = None,
     verbose: bool = False,
+    torch_with_mkl: bool = True,
 ) -> None:
     # make sure user isn't trying to do something silly on MacOS
-    if build_env.PLATFORM == "darwin" and device == "gpu":
+    if build_env.PLATFORM == "darwin" and device == Device.GPU:
         raise BuildError("SmartSim does not support GPU on MacOS")
 
     # decide which runtimes to build
     print("\nML Backends Requested")
     backends_table = [
         ["PyTorch", versions.TORCH, color_bool(use_torch)],
         ["TensorFlow", versions.TENSORFLOW, color_bool(use_tf)],
         ["ONNX", versions.ONNX, color_bool(use_onnx)],
     ]
     print(tabulate(backends_table, tablefmt="fancy_outline"), end="\n\n")
-    print(f"Building for GPU support: {color_bool(device == 'gpu')}\n")
+    print(f"Building for GPU support: {color_bool(device == Device.GPU)}\n")
 
     if not check_backends_install():
         sys.exit(1)
 
     # TORCH
     if use_torch and torch_dir:
         torch_dir = Path(torch_dir).resolve()
@@ -184,22 +184,23 @@
         architecture=builder.Architecture.from_str(platform.machine()),
         torch_dir=str(torch_dir) if torch_dir else "",
         libtf_dir=str(libtf_dir) if libtf_dir else "",
         build_torch=use_torch,
         build_tf=use_tf,
         build_onnx=use_onnx,
         verbose=verbose,
+        torch_with_mkl=torch_with_mkl,
     )
 
     if rai_builder.is_built:
         logger.info("RedisAI installed. Run `smart clean` to remove.")
     else:
         # get the build environment, update with CUDNN env vars
         # if present and building for GPU, otherwise warn the user
-        if device == "gpu":
+        if device == Device.GPU:
             gpu_env = build_env.get_cudnn_env()
             cudnn_env_vars = [
                 "CUDNN_LIBRARY",
                 "CUDNN_INCLUDE_DIR",
                 "CUDNN_INCLUDE_PATH",
                 "CUDNN_LIBRARY_PATH",
             ]
@@ -222,26 +223,24 @@
         # like "from_tarball"
         rai_builder.build_from_git(
             versions.REDISAI_URL, versions.REDISAI_BRANCH, device
         )
         logger.info("ML Backends and RedisAI build complete!")
 
 
-def check_py_torch_version(versions: Versioner, device_in: _TDeviceStr = "cpu") -> None:
+def check_py_torch_version(versions: Versioner, device: Device = Device.CPU) -> None:
     """Check Python environment for TensorFlow installation"""
-
-    device = device_in.lower()
     if BuildEnv.is_macos():
-        if device == "gpu":
+        if device == Device.GPU:
             raise BuildError("SmartSim does not support GPU on MacOS")
         device_suffix = ""
     else:  # linux
-        if device == "cpu":
+        if device == Device.CPU:
             device_suffix = versions.TORCH_CPU_SUFFIX
-        elif device == "gpu":
+        elif device == Device.GPU:
             device_suffix = versions.TORCH_CUDA_SUFFIX
         else:
             raise BuildError("Unrecognized device requested")
 
     torch_deps = {
         "torch": Version_(f"{versions.TORCH}{device_suffix}"),
         "torchvision": Version_(f"{versions.TORCHVISION}{device_suffix}"),
@@ -257,15 +256,17 @@
     if len(missing) == len(torch_deps) and not conflicts:
         # All PyTorch deps are not installed and there are no conflicting
         # python packages. We can try to install torch deps into the current env.
         logger.info(
             "Torch version not found in python environment. "
             "Attempting to install via `pip`"
         )
-        wheel_device = device if device == "cpu" else device_suffix.replace("+", "")
+        wheel_device = (
+            device.value if device == Device.CPU else device_suffix.replace("+", "")
+        )
         pip(
             "install",
             "--extra-index-url",
             f"https://download.pytorch.org/whl/{wheel_device}",
             *(f"{package}=={version}" for package, version in torch_deps.items()),
         )
     elif missing or conflicts:
@@ -335,18 +336,18 @@
             # Incompatible version found
             conflicts.append(spec)
 
     return missing, conflicts
 
 
 def _format_incompatible_python_env_message(
-    missing: t.Iterable[str], conflicting: t.Iterable[str]
+    missing: t.Collection[str], conflicting: t.Collection[str]
 ) -> str:
     indent = "\n\t"
-    fmt_list: t.Callable[[str, t.Iterable[str]], str] = lambda n, l: (
+    fmt_list: t.Callable[[str, t.Collection[str]], str] = lambda n, l: (
         f"{n}:{indent}{indent.join(l)}" if l else ""
     )
     missing_str = fmt_list("Missing", missing)
     conflict_str = fmt_list("Conflicting", conflicting)
     sep = "\n" if missing_str and conflict_str else ""
     return (
         "Python Env Status Warning!\n"
@@ -354,57 +355,75 @@
         f"{missing_str}{sep}{conflict_str}\n\n"
         "Consider installing packages at the requested versions via `pip` or "
         "uninstalling them, installing SmartSim with optional ML dependencies "
         "(`pip install smartsim[ml]`), and running `smart clean && smart build ...`"
     )
 
 
+def _configure_keydb_build(versions: Versioner) -> None:
+    """Configure the redis versions to be used during the build operation"""
+    versions.REDIS = Version_("6.2.0")
+    versions.REDIS_URL = "https://github.com/EQ-Alpha/KeyDB"
+    versions.REDIS_BRANCH = "v6.2.0"
+
+    CONFIG.conf_path = Path(CONFIG.core_path, "config", "keydb.conf")
+    if not CONFIG.conf_path.resolve().is_file():
+        raise SSConfigError(
+            "Database configuration file at REDIS_CONF could not be found"
+        )
+
+
+# pylint: disable-next=too-many-statements
 def execute(
     args: argparse.Namespace, _unparsed_args: t.Optional[t.List[str]] = None, /
 ) -> int:
     verbose = args.v
     keydb = args.keydb
-    device: _TDeviceStr = args.device
-
+    device = Device(args.device.lower())
+    is_dragon_requested = args.dragon
     # torch and tf build by default
     pt = not args.no_pt  # pylint: disable=invalid-name
     tf = not args.no_tf  # pylint: disable=invalid-name
     onnx = args.onnx
 
     build_env = BuildEnv(checks=True)
     logger.info("Running SmartSim build process...")
 
     logger.info("Checking requested versions...")
     versions = Versioner()
 
-    logger.info("Checking for build tools...")
+    logger.debug("Checking for build tools...")
 
     if verbose:
         logger.info("Build Environment:")
         env = build_env.as_dict()
         env_vars = list(env.keys())
         print(tabulate(env, headers=env_vars, tablefmt="github"), "\n")
 
     if keydb:
-        versions.REDIS = Version_("6.2.0")
-        versions.REDIS_URL = "https://github.com/EQ-Alpha/KeyDB"
-        versions.REDIS_BRANCH = "v6.2.0"
-        CONFIG.conf_path = Path(CONFIG.core_path, "config", "keydb.conf")
-        if not CONFIG.conf_path.resolve().is_file():
-            raise SSConfigError(
-                "Database configuration file at REDIS_CONF could not be found"
-            )
+        _configure_keydb_build(versions)
 
     if verbose:
         db_name: DbEngine = "KEYDB" if keydb else "REDIS"
         logger.info("Version Information:")
         vers = versions.as_dict(db_name=db_name)
         version_names = list(vers.keys())
         print(tabulate(vers, headers=version_names, tablefmt="github"), "\n")
 
+    if is_dragon_requested:
+        install_to = CONFIG.core_path / ".dragon"
+        return_code = install_dragon(install_to)
+
+        if return_code == 0:
+            logger.info("Dragon installation complete")
+        elif return_code == 1:
+            logger.info("Dragon installation not supported on platform")
+        else:
+            logger.warning("Dragon installation failed")
+
     try:
         if not args.only_python_packages:
             # REDIS/KeyDB
             build_database(build_env, versions, keydb, verbose)
 
             # REDISAI
             build_redis_ai(
@@ -413,14 +432,15 @@
                 device,
                 pt,
                 tf,
                 onnx,
                 args.torch_dir,
                 args.libtensorflow_dir,
                 verbose=verbose,
+                torch_with_mkl=args.torch_with_mkl,
             )
     except (SetupError, BuildError) as e:
         logger.error(str(e))
         return os.EX_SOFTWARE
 
     backends = installed_redisai_backends()
     backends_str = ", ".join(s.capitalize() for s in backends) if backends else "No"
@@ -449,19 +469,25 @@
         action="store_true",
         default=False,
         help="Enable verbose build process",
     )
     parser.add_argument(
         "--device",
         type=str.lower,
-        default="cpu",
-        choices=["cpu", "gpu"],
+        default=Device.CPU.value,
+        choices=[device.value for device in Device],
         help="Device to build ML runtimes for",
     )
     parser.add_argument(
+        "--dragon",
+        action="store_true",
+        default=False,
+        help="Install the dragon runtime",
+    )
+    parser.add_argument(
         "--only_python_packages",
         action="store_true",
         default=False,
         help="Only evaluate the python packages (i.e. skip building backends)",
     )
     parser.add_argument(
         "--no_pt",
@@ -495,7 +521,13 @@
     )
     parser.add_argument(
         "--keydb",
         action="store_true",
         default=False,
         help="Build KeyDB instead of Redis",
     )
+    parser.add_argument(
+        "--no_torch_with_mkl",
+        dest="torch_with_mkl",
+        action="store_false",
+        help="Do not build Torch with Intel MKL",
+    )
```

### Comparing `smartsim-0.6.2/smartsim/_core/_cli/clean.py` & `smartsim-0.7.0/smartsim/_core/_cli/clean.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.6.2/smartsim/_core/_cli/cli.py` & `smartsim-0.7.0/smartsim/_core/_cli/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 from smartsim._core._cli.clean import configure_parser as clean_parser
 from smartsim._core._cli.clean import execute as clean_execute
 from smartsim._core._cli.clean import execute_all as clobber_execute
 from smartsim._core._cli.dbcli import execute as dbcli_execute
 from smartsim._core._cli.info import execute as info_execute
 from smartsim._core._cli.plugin import plugins
 from smartsim._core._cli.site import execute as site_execute
+from smartsim._core._cli.teardown import configure_parser as teardown_parser
+from smartsim._core._cli.teardown import execute as teardown_execute
 from smartsim._core._cli.utils import MenuItemConfig
 from smartsim._core._cli.validate import configure_parser as validate_parser
 from smartsim._core._cli.validate import execute as validate_execute
 
 
 class SmartCli:
     def __init__(self, menu: t.List[MenuItemConfig]) -> None:
@@ -102,15 +104,15 @@
             self._register_menu_item(item)
 
 
 def default_cli() -> SmartCli:
     menu = [
         MenuItemConfig(
             "build",
-            "Build SmartSim dependencies (Redis, RedisAI, ML runtimes)",
+            "Build SmartSim dependencies (Redis, RedisAI, Dragon, ML runtimes)",
             build_execute,
             build_parser,
         ),
         MenuItemConfig(
             "clean",
             "Remove previous ML runtime installation",
             clean_execute,
@@ -138,10 +140,16 @@
             validate_parser,
         ),
         MenuItemConfig(
             "info",
             "Display information about the current SmartSim installation",
             info_execute,
         ),
+        MenuItemConfig(
+            "teardown",
+            "Clean up allocated resources after an experiment terminates",
+            teardown_execute,
+            teardown_parser,
+        ),
     ]
 
     return SmartCli(menu)
```

### Comparing `smartsim-0.6.2/smartsim/_core/_cli/dbcli.py` & `smartsim-0.7.0/smartsim/_core/_cli/dbcli.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.6.2/smartsim/_core/_cli/info.py` & `smartsim-0.7.0/smartsim/_core/_cli/info.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.6.2/smartsim/_core/_cli/plugin.py` & `smartsim-0.7.0/smartsim/_core/_cli/plugin.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.6.2/smartsim/_core/_cli/site.py` & `smartsim-0.7.0/smartsim/_core/_cli/site.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.6.2/smartsim/_core/_cli/utils.py` & `smartsim-0.7.0/smartsim/_core/_cli/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -74,21 +74,25 @@
             )
 
 
 def clean(core_path: Path, _all: bool = False) -> int:
     """Remove pre existing installations of ML runtimes
 
     :param _all: Remove all non-python dependencies
-    :type _all: bool, optional
     """
 
     build_temp = core_path / ".third-party"
     if build_temp.is_dir():
         shutil.rmtree(build_temp, ignore_errors=True)
 
+    dragon_temp = core_path / ".dragon"
+    if dragon_temp.is_dir():
+        shutil.rmtree(dragon_temp, ignore_errors=True)
+        logger.info("Successfully removed dragon installation")
+
     lib_path = core_path / "lib"
     if lib_path.is_dir():
         # remove RedisAI
         rai_path = lib_path / "redisai.so"
         if rai_path.is_file():
             rai_path.unlink()
             logger.info("Successfully removed existing RedisAI installation")
```

### Comparing `smartsim-0.6.2/smartsim/_core/_cli/validate.py` & `smartsim-0.7.0/smartsim/_core/_cli/validate.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,25 +26,26 @@
 
 import argparse
 import contextlib
 import io
 import multiprocessing as mp
 import os
 import os.path
-import socket
 import tempfile
 import typing as t
 from types import TracebackType
 
 import numpy as np
 from smartredis import Client
 
 from smartsim import Experiment
 from smartsim._core._cli.utils import SMART_LOGGER_FORMAT
+from smartsim._core._install.builder import Device
 from smartsim._core.utils.helpers import installed_redisai_backends
+from smartsim._core.utils.network import find_free_port
 from smartsim.log import get_logger
 
 logger = get_logger("Smart", fmt=SMART_LOGGER_FORMAT)
 
 # Many of the functions in this module will import optional
 # ML python packages only if they are needed to test the build is working
 #
@@ -57,17 +58,14 @@
 
     # pylint: disable-next=unsubscriptable-object
     _TemporaryDirectory = tempfile.TemporaryDirectory[str]
 else:
     _TemporaryDirectory = tempfile.TemporaryDirectory
 
 
-_TCapitalDeviceStr = t.Literal["CPU", "GPU"]
-
-
 class _VerificationTempDir(_TemporaryDirectory):
     """A Temporary directory to be used as a context manager that will only
     clean itself up if no error is raised within its context
     """
 
     def __exit__(
         self,
@@ -84,42 +82,44 @@
 def execute(
     args: argparse.Namespace, _unparsed_args: t.Optional[t.List[str]] = None, /
 ) -> int:
     """Validate the SmartSim installation works as expected given a
     simple experiment
     """
     backends = installed_redisai_backends()
-    device: _TCapitalDeviceStr = args.device.upper()
+    temp_dir = ""
+    device = Device(args.device)
     try:
         with contextlib.ExitStack() as ctx:
             temp_dir = ctx.enter_context(_VerificationTempDir(dir=os.getcwd()))
             validate_env = {
                 "SR_LOG_LEVEL": os.environ.get("SR_LOG_LEVEL", "INFO"),
                 "SR_LOG_FILE": os.environ.get(
                     "SR_LOG_FILE", os.path.join(temp_dir, "smartredis.log")
                 ),
             }
-            if device == "GPU":
+            if device == Device.GPU:
                 validate_env["CUDA_VISIBLE_DEVICES"] = "0"
             ctx.enter_context(_env_vars_set_to(validate_env))
             test_install(
                 location=temp_dir,
                 port=args.port,
                 device=device,
                 with_tf="tensorflow" in backends,
                 with_pt="torch" in backends,
                 with_onnx="onnxruntime" in backends,
             )
     except Exception as e:
         logger.error(
             "SmartSim failed to run a simple experiment!\n"
-            f"Experiment failed due to the following exception:\n{e}\n\n"
-            f"Output files are available at `{temp_dir}`",
+            f"Experiment failed due to the following exception:\n{e}",
             exc_info=True,
         )
+        if temp_dir:
+            logger.info(f"Output files are available at `{temp_dir}`")
         return os.EX_SOFTWARE
     return os.EX_OK
 
 
 def configure_parser(parser: argparse.ArgumentParser) -> None:
     """Build the parser for the command"""
     parser.add_argument(
@@ -132,31 +132,32 @@
             "If not provided, `smart` will attempt to automatically select an "
             "open port"
         ),
     )
     parser.add_argument(
         "--device",
         type=str.lower,
-        default="cpu",
-        choices=["cpu", "gpu"],
+        default=Device.CPU.value,
+        choices=[device.value for device in Device],
         help="Device to test the ML backends against",
     )
 
 
 def test_install(
     location: str,
     port: t.Optional[int],
-    device: _TCapitalDeviceStr,
+    device: Device,
     with_tf: bool,
     with_pt: bool,
     with_onnx: bool,
 ) -> None:
     exp = Experiment("ValidationExperiment", exp_path=location, launcher="local")
-    exp.disable_telemetry()
-    port = _find_free_port() if port is None else port
+    exp.telemetry.disable()
+    port = find_free_port() if port is None else port
+
     with _make_managed_local_orc(exp, port) as client:
         logger.info("Verifying Tensor Transfer")
         client.put_tensor("plain-tensor", np.ones((1, 1, 3, 3)))
         client.get_tensor("plain-tensor")
         if with_pt:
             logger.info("Verifying Torch Backend")
             _test_torch_install(client, device)
@@ -201,23 +202,15 @@
     try:
         (client_addr,) = orc.get_address()
         yield Client(False, address=client_addr)
     finally:
         exp.stop(orc)
 
 
-def _find_free_port() -> int:
-    """A 'good enough' way to find an open port to bind to"""
-    with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as sock:
-        sock.bind(("0.0.0.0", 0))
-        _, port = sock.getsockname()
-        return int(port)
-
-
-def _test_tf_install(client: Client, tmp_dir: str, device: _TCapitalDeviceStr) -> None:
+def _test_tf_install(client: Client, tmp_dir: str, device: Device) -> None:
     recv_conn, send_conn = mp.Pipe(duplex=False)
     # Build the model in a subproc so that keras does not hog the gpu
     proc = mp.Process(target=_build_tf_frozen_model, args=(send_conn, tmp_dir))
     proc.start()
 
     # do not need the sending connection in this proc anymore
     send_conn.close()
@@ -231,15 +224,20 @@
     except EOFError as e:
         raise Exception(
             "Failed to receive serialized model from subprocess. "
             "Is the `tensorflow` python package installed?"
         ) from e
 
     client.set_model_from_file(
-        "keras-fcn", model_path, "TF", device=device, inputs=inputs, outputs=outputs
+        "keras-fcn",
+        model_path,
+        "TF",
+        device=device.value.upper(),
+        inputs=inputs,
+        outputs=outputs,
     )
     client.put_tensor("keras-input", np.random.rand(1, 28, 28).astype(np.float32))
     client.run_model("keras-fcn", inputs=["keras-input"], outputs=["keras-output"])
     client.get_tensor("keras-output")
 
 
 def _build_tf_frozen_model(conn: "Connection", tmp_dir: str) -> None:
@@ -259,27 +257,27 @@
     fcn.compile(
         optimizer="adam", loss="sparse_categorical_crossentropy", metrics=["accuracy"]
     )
     model_path, inputs, outputs = freeze_model(fcn, tmp_dir, "keras_model.pb")
     conn.send((model_path, inputs, outputs))
 
 
-def _test_torch_install(client: Client, device: _TCapitalDeviceStr) -> None:
+def _test_torch_install(client: Client, device: Device) -> None:
     import torch
     from torch import nn
 
     class Net(nn.Module):
         def __init__(self) -> None:
             super().__init__()
             self.conv: t.Callable[..., torch.Tensor] = nn.Conv2d(1, 1, 3)
 
         def forward(self, x: torch.Tensor) -> torch.Tensor:
             return self.conv(x)
 
-    if device == "GPU":
+    if device == Device.GPU:
         device_ = torch.device("cuda")
     else:
         device_ = torch.device("cpu")
 
     net = Net()
     net.to(device_)
     net.eval()
@@ -287,31 +285,31 @@
     forward_input = torch.rand(1, 1, 3, 3).to(device_)
     traced = torch.jit.trace(net, forward_input)  # type: ignore[no-untyped-call]
 
     buffer = io.BytesIO()
     torch.jit.save(traced, buffer)  # type: ignore[no-untyped-call]
     model = buffer.getvalue()
 
-    client.set_model("torch-nn", model, backend="TORCH", device=device)
+    client.set_model("torch-nn", model, backend="TORCH", device=device.value.upper())
     client.put_tensor("torch-in", torch.rand(1, 1, 3, 3).numpy())
     client.run_model("torch-nn", inputs=["torch-in"], outputs=["torch-out"])
     client.get_tensor("torch-out")
 
 
-def _test_onnx_install(client: Client, device: _TCapitalDeviceStr) -> None:
+def _test_onnx_install(client: Client, device: Device) -> None:
     from skl2onnx import to_onnx
     from sklearn.cluster import KMeans
 
     data = np.arange(20, dtype=np.float32).reshape(10, 2)
     model = KMeans(n_clusters=2, n_init=10)
     model.fit(data)
 
     kmeans = to_onnx(model, data, target_opset=11)
     model = kmeans.SerializeToString()
     sample = np.arange(20, dtype=np.float32).reshape(10, 2)
 
     client.put_tensor("onnx-input", sample)
-    client.set_model("onnx-kmeans", model, "ONNX", device=device)
+    client.set_model("onnx-kmeans", model, "ONNX", device=device.value.upper())
     client.run_model(
         "onnx-kmeans", inputs=["onnx-input"], outputs=["onnx-labels", "onnx-transform"]
     )
     client.get_tensor("onnx-labels")
```

### Comparing `smartsim-0.6.2/smartsim/_core/_install/__init__.py` & `smartsim-0.7.0/smartsim/_core/_install/__init__.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.6.2/smartsim/_core/_install/buildenv.py` & `smartsim-0.7.0/smartsim/_core/_install/buildenv.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,23 +263,23 @@
 
     Default versions for SmartSim, SmartRedis, Redis, and RedisAI are
     all set here. Setting a default version for RedisAI also dictates
     default versions of the machine learning libraries.
     """
 
     # compatible Python version
-    PYTHON_MIN = Version_("3.8.0")
+    PYTHON_MIN = Version_("3.9.0")
 
     # Versions
-    SMARTSIM = Version_(get_env("SMARTSIM_VERSION", "0.6.2"))
-    SMARTREDIS = Version_(get_env("SMARTREDIS_VERSION", "0.5.2"))
+    SMARTSIM = Version_(get_env("SMARTSIM_VERSION", "0.7.0"))
+    SMARTREDIS = Version_(get_env("SMARTREDIS_VERSION", "0.5.3"))
     SMARTSIM_SUFFIX = get_env("SMARTSIM_SUFFIX", "")
 
     # Redis
-    REDIS = Version_(get_env("SMARTSIM_REDIS", "7.0.5"))
+    REDIS = Version_(get_env("SMARTSIM_REDIS", "7.2.4"))
     REDIS_URL = get_env("SMARTSIM_REDIS_URL", "https://github.com/redis/redis.git/")
     REDIS_BRANCH = get_env("SMARTSIM_REDIS_BRANCH", REDIS)
 
     # RedisAI
     REDISAI = RedisAIVersion(get_env("SMARTSIM_REDISAI", "1.2.7"))
     REDISAI_URL = get_env(
         "SMARTSIM_REDISAI_URL", "https://github.com/RedisAI/RedisAI.git/"
```

### Comparing `smartsim-0.6.2/smartsim/_core/_install/builder.py` & `smartsim-0.7.0/smartsim/_core/_install/builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 # pylint: disable=too-many-lines
 
 import concurrent.futures
 import enum
+import fileinput
 import itertools
 import os
 import platform
 import re
 import shutil
 import stat
 import subprocess
@@ -49,25 +50,23 @@
 
 # NOTE: This will be imported by setup.py and hence no smartsim related
 # items should be imported into this file.
 
 # TODO: check cmake version and use system if possible to avoid conflicts
 
 TRedisAIBackendStr = t.Literal["tensorflow", "torch", "onnxruntime", "tflite"]
-TDeviceStr = t.Literal["cpu", "gpu"]
-
+_PathLike = t.Union[str, "os.PathLike[str]"]
 _T = t.TypeVar("_T")
 _U = t.TypeVar("_U")
 
 
 def expand_exe_path(exe: str) -> str:
     """Takes an executable and returns the full path to that executable
 
     :param exe: executable or file
-    :type exe: str
     :raises TypeError: if file is not an executable
     :raises FileNotFoundError: if executable cannot be found
     """
 
     # which returns none if not found
     in_path = which(exe)
     if not in_path:
@@ -92,14 +91,19 @@
         string = string.lower()
         for type_ in cls:
             if string in type_.value:
                 return type_
         raise BuildError(f"Unrecognized or unsupported architecture: {string}")
 
 
+class Device(enum.Enum):
+    CPU = "cpu"
+    GPU = "gpu"
+
+
 class OperatingSystem(enum.Enum):
     LINUX = ("linux", "linux2")
     DARWIN = ("darwin",)
 
     @classmethod
     def from_str(cls, string: str, /) -> "OperatingSystem":
         string = string.lower()
@@ -169,15 +173,15 @@
 
     # implemented in base classes
     @property
     def is_built(self) -> bool:
         raise NotImplementedError
 
     def build_from_git(
-        self, git_url: str, branch: str, device: TDeviceStr = "cpu"
+        self, git_url: str, branch: str, device: Device = Device.CPU
     ) -> None:
         raise NotImplementedError
 
     @staticmethod
     def binary_path(binary: str) -> str:
         binary_ = shutil.which(binary)
         if binary_:
@@ -270,21 +274,19 @@
         """Check if Redis or KeyDB is built"""
         bin_files = {file.name for file in self.bin_path.iterdir()}
         redis_files = {"redis-server", "redis-cli"}
         keydb_files = {"keydb-server", "keydb-cli"}
         return redis_files.issubset(bin_files) or keydb_files.issubset(bin_files)
 
     def build_from_git(
-        self, git_url: str, branch: str, device: TDeviceStr = "cpu"
+        self, git_url: str, branch: str, device: Device = Device.CPU
     ) -> None:
         """Build Redis from git
         :param git_url: url from which to retrieve Redis
-        :type git_url: str
         :param branch: branch to checkout
-        :type branch: str
         """
         # pylint: disable=too-many-locals
         database_name = "keydb" if "KeyDB" in git_url else "redis"
         database_build_path = Path(self.build_dir, database_name.lower())
 
         # remove git directory if it exists as it should
         # really never exist as we delete after build
@@ -360,23 +362,23 @@
     """
 
     @property
     @abstractmethod
     def __rai_dependency_name__(self) -> str: ...
 
     @abstractmethod
-    def __place_for_rai__(self, target: t.Union[str, "os.PathLike[str]"]) -> Path: ...
+    def __place_for_rai__(self, target: _PathLike) -> Path: ...
 
     @staticmethod
     @abstractmethod
     def supported_platforms() -> t.Sequence[t.Tuple[OperatingSystem, Architecture]]: ...
 
 
 def _place_rai_dep_at(
-    target: t.Union[str, "os.PathLike[str]"], verbose: bool
+    target: _PathLike, verbose: bool
 ) -> t.Callable[[_RAIBuildDependency], Path]:
     def _place(dep: _RAIBuildDependency) -> Path:
         if verbose:
             print(f"Placing: '{dep.__rai_dependency_name__}'")
         path = dep.__place_for_rai__(target)
         if verbose:
             print(f"Placed: '{dep.__rai_dependency_name__}' at '{path}'")
@@ -401,14 +403,15 @@
         torch_dir: str = "",
         libtf_dir: str = "",
         build_torch: bool = True,
         build_tf: bool = True,
         build_onnx: bool = False,
         jobs: int = 1,
         verbose: bool = False,
+        torch_with_mkl: bool = True,
     ) -> None:
         super().__init__(
             build_env or {},
             jobs=jobs,
             _os=_os,
             architecture=architecture,
             verbose=verbose,
@@ -419,14 +422,17 @@
         # convert to int for RAI build script
         self._torch = build_torch
         self._tf = build_tf
         self._onnx = build_onnx
         self.libtf_dir = libtf_dir
         self.torch_dir = torch_dir
 
+        # extra configuration options
+        self.torch_with_mkl = torch_with_mkl
+
         # Sanity checks
         self._validate_platform()
 
     def _validate_platform(self) -> None:
         unsupported = []
         if self._platform not in _DLPackRepository.supported_platforms():
             unsupported.append("DLPack")
@@ -476,15 +482,15 @@
     def build_onnx(self) -> bool:
         return self._onnx
 
     @property
     def fetch_onnx(self) -> bool:
         return self.build_onnx
 
-    def get_deps_dir_path_for(self, device: TDeviceStr) -> Path:
+    def get_deps_dir_path_for(self, device: Device) -> Path:
         def fail_to_format(reason: str) -> BuildError:  # pragma: no cover
             return BuildError(f"Failed to format RedisAI dependency path: {reason}")
 
         _os, architecture = self._platform
         if _os == OperatingSystem.DARWIN:
             os_ = "macos"
         elif _os == OperatingSystem.LINUX:
@@ -493,46 +499,45 @@
             raise fail_to_format(f"Unknown operating system: {_os}")
         if architecture == Architecture.X64:
             arch = "x64"
         elif architecture == Architecture.ARM64:
             arch = "arm64v8"
         else:  # pragma: no cover
             raise fail_to_format(f"Unknown architecture: {architecture}")
-        return self.rai_build_path / f"deps/{os_}-{arch}-{device}"
+        return self.rai_build_path / f"deps/{os_}-{arch}-{device.value}"
 
     def _get_deps_to_fetch_for(
-        self, device: TDeviceStr
+        self, device: Device
     ) -> t.Tuple[_RAIBuildDependency, ...]:
         os_, arch = self._platform
         # TODO: It would be nice if the backend version numbers were declared
         #       alongside the python package version numbers so that all of the
         #       dependency versions were declared in single location.
         #       Unfortunately importing into this module is non-trivial as it
         #       is used as script in the SmartSim `setup.py`.
 
         # DLPack is always required
         fetchable_deps: t.List[_RAIBuildDependency] = [_DLPackRepository("v0.5_RAI")]
         if self.fetch_torch:
-            pt_dep = _choose_pt_variant(os_)
-            fetchable_deps.append(pt_dep(arch, device, "2.0.1"))
+            pt_dep = _choose_pt_variant(os_)(arch, device, "2.0.1", self.torch_with_mkl)
+            fetchable_deps.append(pt_dep)
         if self.fetch_tf:
             fetchable_deps.append(_TFArchive(os_, arch, device, "2.13.1"))
         if self.fetch_onnx:
             fetchable_deps.append(_ORTArchive(os_, device, "1.16.3"))
 
         return tuple(fetchable_deps)
 
-    def symlink_libtf(self, device: str) -> None:
+    def symlink_libtf(self, device: Device) -> None:
         """Add symbolic link to available libtensorflow in RedisAI deps.
 
         :param device: cpu or gpu
-        :type device: str
         """
         rai_deps_path = sorted(
-            self.rai_build_path.glob(os.path.join("deps", f"*{device}*"))
+            self.rai_build_path.glob(os.path.join("deps", f"*{device.value}*"))
         )
         if not rai_deps_path:
             raise FileNotFoundError("Could not find RedisAI 'deps' directory")
 
         # There should only be one path for a given device,
         # and this should hold even if in the future we use
         # an external build of RedisAI
@@ -573,24 +578,21 @@
 
         for src_file in library_files:
             dst_file = rai_libtf_lib_dir / src_file.name
             if not dst_file.is_file():
                 os.symlink(src_file, dst_file)
 
     def build_from_git(
-        self, git_url: str, branch: str, device: TDeviceStr = "cpu"
+        self, git_url: str, branch: str, device: Device = Device.CPU
     ) -> None:
         """Build RedisAI from git
 
         :param git_url: url from which to retrieve RedisAI
-        :type git_url: str
         :param branch: branch to checkout
-        :type branch: str
         :param device: cpu or gpu
-        :type device: str
         """
         # delete previous build dir (should never be there)
         if self.rai_build_path.is_dir():
             shutil.rmtree(self.rai_build_path)
 
         # Check RedisAI URL
         if not self.is_valid_url(git_url):
@@ -612,22 +614,22 @@
                 os.fspath(self.rai_build_path),
             ],
         )
 
         self.run_command(clone_cmd, out=subprocess.DEVNULL, cwd=self.build_dir)
         self._fetch_deps_for(device)
 
-        if self.libtf_dir and device:
+        if self.libtf_dir and device.value:
             self.symlink_libtf(device)
 
         build_cmd = self._rai_build_env_prefix(
             with_pt=self.build_torch,
             with_tf=self.build_tf,
             with_ort=self.build_onnx,
-            extra_env={"GPU": "1" if device == "gpu" else "0"},
+            extra_env={"GPU": "1" if device == Device.GPU else "0"},
         )
 
         if self.torch_dir:
             self.env["Torch_DIR"] = str(self.torch_dir)
 
         build_cmd.extend(
             [
@@ -670,15 +672,15 @@
             f"WITH_PT={1 if with_pt else 0}",
             f"WITH_TF={1 if with_tf else 0}",
             "WITH_TFLITE=0",  # never use TF Lite (for now)
             f"WITH_ORT={1 if with_ort else 0}",
             *(f"{key}={val}" for key, val in extra_env.items()),
         ]
 
-    def _fetch_deps_for(self, device: TDeviceStr) -> None:
+    def _fetch_deps_for(self, device: Device) -> None:
         if not self.rai_build_path.is_dir():
             raise BuildError("RedisAI build directory not found")
 
         deps_dir = self.get_deps_dir_path_for(device)
         deps_dir.mkdir(parents=True, exist_ok=True)
         if any(deps_dir.iterdir()):
             raise BuildError("RAI build dependency directory is not empty")
@@ -689,21 +691,20 @@
         unique_placed_paths = {os.fspath(path.resolve()) for path in placed_paths}
         if len(unique_placed_paths) != len(to_fetch):
             raise BuildError(
                 f"Expected to place {len(to_fetch)} dependencies, but only "
                 f"found {len(unique_placed_paths)}"
             )
 
-    def _install_backends(self, device: str) -> None:
+    def _install_backends(self, device: Device) -> None:
         """Move backend libraries to smartsim/_core/lib/
         :param device: cpu or cpu
-        :type device: str
         """
         self.rai_install_path = self.rai_build_path.joinpath(
-            f"install-{device}"
+            f"install-{device.value}"
         ).resolve()
         rai_lib = self.rai_install_path / "redisai.so"
         rai_backends = self.rai_install_path / "backends"
 
         if rai_lib.is_file() and rai_backends.is_dir():
             self.copy_dir(rai_backends, self.lib_path / "backends", set_exe=True)
             self.copy_file(rai_lib, self.lib_path / "redisai.so", set_exe=True)
@@ -746,15 +747,15 @@
     @abstractmethod
     def url(self) -> str: ...
 
 
 class _WebGitRepository(_WebLocation):
     def clone(
         self,
-        target: t.Union[str, "os.PathLike[str]"],
+        target: _PathLike,
         depth: t.Optional[int] = None,
         branch: t.Optional[str] = None,
     ) -> None:
         depth_ = ("--depth", str(depth)) if depth is not None else ()
         branch_ = ("--branch", branch) if branch is not None else ()
         _git("clone", "-q", *depth_, *branch_, self.url, os.fspath(target))
 
@@ -776,84 +777,101 @@
     def url(self) -> str:
         return "https://github.com/RedisAI/dlpack.git"
 
     @property
     def __rai_dependency_name__(self) -> str:
         return f"dlpack@{self.url}"
 
-    def __place_for_rai__(self, target: t.Union[str, "os.PathLike[str]"]) -> Path:
+    def __place_for_rai__(self, target: _PathLike) -> Path:
         target = Path(target) / "dlpack"
         self.clone(target, branch=self.version, depth=1)
         if not target.is_dir():
             raise BuildError("Failed to place dlpack")
         return target
 
 
 class _WebArchive(_WebLocation):
     @property
     def name(self) -> str:
         _, name = self.url.rsplit("/", 1)
         return name
 
-    def download(self, target: t.Union[str, "os.PathLike[str]"]) -> Path:
+    def download(self, target: _PathLike) -> Path:
         target = Path(target)
         if target.is_dir():
             target = target / self.name
         file, _ = urllib.request.urlretrieve(self.url, target)
         return Path(file).resolve()
 
 
 class _ExtractableWebArchive(_WebArchive, ABC):
     @abstractmethod
-    def _extract_download(
-        self, download_path: Path, target: t.Union[str, "os.PathLike[str]"]
-    ) -> None: ...
+    def _extract_download(self, download_path: Path, target: _PathLike) -> None: ...
 
-    def extract(self, target: t.Union[str, "os.PathLike[str]"]) -> None:
+    def extract(self, target: _PathLike) -> None:
         with tempfile.TemporaryDirectory() as tmp_dir:
             arch_path = self.download(tmp_dir)
             self._extract_download(arch_path, target)
 
 
 class _WebTGZ(_ExtractableWebArchive):
-    def _extract_download(
-        self, download_path: Path, target: t.Union[str, "os.PathLike[str]"]
-    ) -> None:
+    def _extract_download(self, download_path: Path, target: _PathLike) -> None:
         with tarfile.open(download_path, "r") as tgz_file:
             tgz_file.extractall(target)
 
 
 class _WebZip(_ExtractableWebArchive):
-    def _extract_download(
-        self, download_path: Path, target: t.Union[str, "os.PathLike[str]"]
-    ) -> None:
+    def _extract_download(self, download_path: Path, target: _PathLike) -> None:
         with zipfile.ZipFile(download_path, "r") as zip_file:
             zip_file.extractall(target)
 
 
+class WebTGZ(_WebTGZ):
+    def __init__(self, url: str) -> None:
+        self._url = url
+
+    @property
+    def url(self) -> str:
+        return self._url
+
+
 @dataclass(frozen=True)
 class _PTArchive(_WebZip, _RAIBuildDependency):
     architecture: Architecture
-    device: TDeviceStr
+    device: Device
     version: str
+    with_mkl: bool
 
     @staticmethod
     def supported_platforms() -> t.Sequence[t.Tuple[OperatingSystem, Architecture]]:
         # TODO: This will need to be revisited if the inheritance tree gets deeper
         return tuple(
             itertools.chain.from_iterable(
                 var.supported_platforms() for var in _PTArchive.__subclasses__()
             )
         )
 
     @property
     def __rai_dependency_name__(self) -> str:
         return f"libtorch@{self.url}"
 
-    def __place_for_rai__(self, target: t.Union[str, "os.PathLike[str]"]) -> Path:
+    @staticmethod
+    def _patch_out_mkl(libtorch_root: Path) -> None:
+        _modify_source_files(
+            libtorch_root / "share/cmake/Caffe2/public/mkl.cmake",
+            r"find_package\(MKL QUIET\)",
+            "# find_package(MKL QUIET)",
+        )
+
+    def extract(self, target: _PathLike) -> None:
+        super().extract(target)
+        if not self.with_mkl:
+            self._patch_out_mkl(Path(target))
+
+    def __place_for_rai__(self, target: _PathLike) -> Path:
         self.extract(target)
         target = Path(target) / "libtorch"
         if not target.is_dir():
             raise BuildError("Failed to place RAI dependency: `libtorch`")
         return target
 
 
@@ -861,18 +879,18 @@
 class _PTArchiveLinux(_PTArchive):
     @staticmethod
     def supported_platforms() -> t.Sequence[t.Tuple[OperatingSystem, Architecture]]:
         return ((OperatingSystem.LINUX, Architecture.X64),)
 
     @property
     def url(self) -> str:
-        if self.device == "gpu":
+        if self.device == Device.GPU:
             pt_build = "cu117"
         else:
-            pt_build = "cpu"
+            pt_build = Device.CPU.value
         # pylint: disable-next=line-too-long
         libtorch_archive = (
             f"libtorch-cxx11-abi-shared-without-deps-{self.version}%2B{pt_build}.zip"
         )
         return f"https://download.pytorch.org/libtorch/{pt_build}/{libtorch_archive}"
 
 
@@ -883,30 +901,30 @@
         return (
             (OperatingSystem.DARWIN, Architecture.ARM64),
             (OperatingSystem.DARWIN, Architecture.X64),
         )
 
     @property
     def url(self) -> str:
-        if self.device == "gpu":
+        if self.device == Device.GPU:
             raise BuildError("RedisAI does not currently support GPU on Mac OSX")
         if self.architecture == Architecture.X64:
-            pt_build = "cpu"
+            pt_build = Device.CPU.value
             libtorch_archive = f"libtorch-macos-{self.version}.zip"
             root_url = "https://download.pytorch.org/libtorch"
             return f"{root_url}/{pt_build}/{libtorch_archive}"
         if self.architecture == Architecture.ARM64:
             libtorch_archive = f"libtorch-macos-arm64-{self.version}.zip"
             # pylint: disable-next=line-too-long
             root_url = (
                 "https://github.com/CrayLabs/ml_lib_builder/releases/download/v0.1/"
             )
             return f"{root_url}/{libtorch_archive}"
 
-        raise BuildError("Unsupported architecture for Pytorch: {self.architecture}")
+        raise BuildError(f"Unsupported architecture for Pytorch: {self.architecture}")
 
 
 def _choose_pt_variant(
     os_: OperatingSystem,
 ) -> t.Union[t.Type[_PTArchiveLinux], t.Type[_PTArchiveMacOSX]]:
     if os_ == OperatingSystem.DARWIN:
         return _PTArchiveMacOSX
@@ -917,15 +935,15 @@
 
 
 @t.final
 @dataclass(frozen=True)
 class _TFArchive(_WebTGZ, _RAIBuildDependency):
     os_: OperatingSystem
     architecture: Architecture
-    device: TDeviceStr
+    device: Device
     version: str
 
     @staticmethod
     def supported_platforms() -> t.Sequence[t.Tuple[OperatingSystem, Architecture]]:
         return (
             (OperatingSystem.LINUX, Architecture.X64),
             (OperatingSystem.DARWIN, Architecture.X64),
@@ -933,48 +951,48 @@
 
     @property
     def url(self) -> str:
         if self.architecture == Architecture.X64:
             tf_arch = "x86_64"
         else:
             raise BuildError(
-                "Unexpected Architecture for TF Archive: {self.architecture}"
+                f"Unexpected Architecture for TF Archive: {self.architecture}"
             )
 
         if self.os_ == OperatingSystem.LINUX:
             tf_os = "linux"
             tf_device = self.device
         elif self.os_ == OperatingSystem.DARWIN:
             tf_os = "darwin"
-            if self.device == "gpu":
+            if self.device == Device.GPU:
                 raise BuildError("RedisAI does not currently support GPU on Macos")
-            tf_device = "cpu"
+            tf_device = Device.CPU
         else:
-            raise BuildError("Unexpected OS for TF Archive: {self.os_}")
+            raise BuildError(f"Unexpected OS for TF Archive: {self.os_}")
         return (
             "https://storage.googleapis.com/tensorflow/libtensorflow/"
-            f"libtensorflow-{tf_device}-{tf_os}-{tf_arch}-{self.version}.tar.gz"
+            f"libtensorflow-{tf_device.value}-{tf_os}-{tf_arch}-{self.version}.tar.gz"
         )
 
     @property
     def __rai_dependency_name__(self) -> str:
         return f"libtensorflow@{self.url}"
 
-    def __place_for_rai__(self, target: t.Union[str, "os.PathLike[str]"]) -> Path:
+    def __place_for_rai__(self, target: _PathLike) -> Path:
         target = Path(target) / "libtensorflow"
         target.mkdir()
         self.extract(target)
         return target
 
 
 @t.final
 @dataclass(frozen=True)
 class _ORTArchive(_WebTGZ, _RAIBuildDependency):
     os_: OperatingSystem
-    device: TDeviceStr
+    device: Device
     version: str
 
     @staticmethod
     def supported_platforms() -> t.Sequence[t.Tuple[OperatingSystem, Architecture]]:
         return (
             (OperatingSystem.LINUX, Architecture.X64),
             (OperatingSystem.DARWIN, Architecture.X64),
@@ -985,31 +1003,31 @@
         ort_url_base = (
             "https://github.com/microsoft/onnxruntime/releases/"
             f"download/v{self.version}"
         )
         if self.os_ == OperatingSystem.LINUX:
             ort_os = "linux"
             ort_arch = "x64"
-            ort_build = "-gpu" if self.device == "gpu" else ""
+            ort_build = "-gpu" if self.device == Device.GPU else ""
         elif self.os_ == OperatingSystem.DARWIN:
             ort_os = "osx"
             ort_arch = "x86_64"
             ort_build = ""
-            if self.device == "gpu":
+            if self.device == Device.GPU:
                 raise BuildError("RedisAI does not currently support GPU on Macos")
         else:
-            raise BuildError("Unexpected OS for TF Archive: {self.os_}")
+            raise BuildError(f"Unexpected OS for TF Archive: {self.os_}")
         ort_archive = f"onnxruntime-{ort_os}-{ort_arch}{ort_build}-{self.version}.tgz"
         return f"{ort_url_base}/{ort_archive}"
 
     @property
     def __rai_dependency_name__(self) -> str:
         return f"onnxruntime@{self.url}"
 
-    def __place_for_rai__(self, target: t.Union[str, "os.PathLike[str]"]) -> Path:
+    def __place_for_rai__(self, target: _PathLike) -> Path:
         target = Path(target).resolve() / "onnxruntime"
         self.extract(target)
         try:
             (extracted_dir,) = target.iterdir()
         except ValueError:
             raise BuildError(
                 "Unexpected number of files extracted from ORT archive"
@@ -1042,7 +1060,17 @@
     if plat == Platform(OperatingSystem.DARWIN, Architecture.ARM64):
         cmd = (
             cmd[:where]
             + ["--config", "core.autocrlf=false", "--config", "core.eol=lf"]
             + cmd[where:]
         )
     return cmd
+
+
+def _modify_source_files(
+    files: t.Union[_PathLike, t.Iterable[_PathLike]], regex: str, replacement: str
+) -> None:
+    compiled_regex = re.compile(regex)
+    with fileinput.input(files=files, inplace=True) as handles:
+        for line in handles:
+            line = compiled_regex.sub(replacement, line)
+            print(line, end="")
```

### Comparing `smartsim-0.6.2/smartsim/_core/config/__init__.py` & `smartsim-0.7.0/smartsim/_core/config/__init__.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.6.2/smartsim/_core/config/config.py` & `smartsim-0.7.0/smartsim/_core/config/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -85,24 +85,26 @@
 #  - Defaults: 1
 #
 # SMARTSIM_TEST_ACCOUNT
 #  - Account used to run full launcher test suite on external systems
 #  - Default: None
 
 
+# pylint: disable-next=too-many-public-methods
 class Config:
     def __init__(self) -> None:
         # SmartSim/smartsim/_core
         self.core_path = Path(os.path.abspath(__file__)).parent.parent
 
         dependency_path = os.environ.get("SMARTSIM_DEP_INSTALL_PATH", self.core_path)
 
         self.lib_path = Path(dependency_path, "lib").resolve()
         self.bin_path = Path(dependency_path, "bin").resolve()
         self.conf_path = Path(dependency_path, "config", "redis.conf")
+        self.conf_dir = Path(self.core_path, "config")
 
     @property
     def redisai(self) -> str:
         rai_path = self.lib_path / "redisai.so"
         redisai = Path(os.environ.get("RAI_PATH", rai_path)).resolve()
         if not redisai.is_file():
             raise SSConfigError(
@@ -149,14 +151,38 @@
         return int(os.getenv("SMARTSIM_DB_FILE_PARSE_TRIALS", "10"))
 
     @property
     def database_file_parse_interval(self) -> int:
         return int(os.getenv("SMARTSIM_DB_FILE_PARSE_INTERVAL", "2"))
 
     @property
+    def dragon_dotenv(self) -> Path:
+        """Returns the path to a .env file containing dragon environment variables"""
+        return self.conf_dir / "dragon" / ".env"
+
+    @property
+    def dragon_server_path(self) -> t.Optional[str]:
+        return os.getenv(
+            "SMARTSIM_DRAGON_SERVER_PATH",
+            os.getenv("SMARTSIM_DRAGON_SERVER_PATH_EXP", None),
+        )
+
+    @property
+    def dragon_server_timeout(self) -> int:
+        return int(os.getenv("SMARTSIM_DRAGON_TIMEOUT", "30000"))
+
+    @property
+    def dragon_server_startup_timeout(self) -> int:
+        return int(os.getenv("SMARTSIM_DRAGON_STARTUP_TIMEOUT", "300000"))
+
+    @property
+    def dragon_transport(self) -> str:
+        return os.getenv("SMARTSIM_DRAGON_TRANSPORT", "hsta")
+
+    @property
     def log_level(self) -> str:
         return os.environ.get("SMARTSIM_LOG_LEVEL", "info")
 
     @property
     def jm_interval(self) -> int:
         return int(os.environ.get("SMARTSIM_JM_INTERVAL") or 10)
 
@@ -173,16 +199,22 @@
         return os.environ.get("SMARTSIM_TEST_DEVICE", "CPU")
 
     @property
     def test_num_gpus(self) -> int:  # pragma: no cover
         return int(os.environ.get("SMARTSIM_TEST_NUM_GPUS") or 1)
 
     @property
-    def test_port(self) -> int:  # pragma: no cover
-        return int(os.environ.get("SMARTSIM_TEST_PORT", 6780))
+    def test_ports(self) -> t.Sequence[int]:  # pragma: no cover
+        min_required_ports = 25
+        first_port = int(os.environ.get("SMARTSIM_TEST_PORT", 6780))
+        num_ports = max(
+            int(os.environ.get("SMARTSIM_TEST_NUM_PORTS", min_required_ports)),
+            min_required_ports,
+        )
+        return range(first_port, first_port + num_ports)
 
     @property
     def test_batch_resources(self) -> t.Dict[t.Any, t.Any]:  # pragma: no cover
         resource_str = os.environ.get("SMARTSIM_TEST_BATCH_RESOURCES", "{}")
         resources = json.loads(resource_str)
         if not isinstance(resources, dict):
             raise TypeError(
@@ -216,14 +248,19 @@
 
     @property
     def test_account(self) -> t.Optional[str]:  # pragma: no cover
         # no account by default
         return os.environ.get("SMARTSIM_TEST_ACCOUNT", None)
 
     @property
+    def test_mpi(self) -> bool:  # pragma: no cover
+        # By default, test MPI app if it compiles
+        return int(os.environ.get("SMARTSIM_TEST_MPI", "1")) > 0
+
+    @property
     def telemetry_frequency(self) -> int:
         return int(os.environ.get("SMARTSIM_TELEMETRY_FREQUENCY", 5))
 
     @property
     def telemetry_enabled(self) -> bool:
         return int(os.environ.get("SMARTSIM_FLAG_TELEMETRY", "1")) > 0
 
@@ -231,12 +268,35 @@
     def telemetry_cooldown(self) -> int:
         return int(os.environ.get("SMARTSIM_TELEMETRY_COOLDOWN", 90))
 
     @property
     def telemetry_subdir(self) -> str:
         return ".smartsim/telemetry"
 
+    @property
+    def dragon_default_subdir(self) -> str:
+        return ".smartsim/dragon"
+
+    @property
+    def dragon_log_filename(self) -> str:
+        return "dragon_config.log"
+
+    @property
+    def smartsim_key_path(self) -> str:
+        """Path to a root directory used for persistence of key files. Default
+        value `$HOME/.smartsim/keys`. User-overrideable by setting the environment
+        variable `SMARTSIM_KEY_PATH`.
+
+        :returns: The configured key path.
+        """
+        default_path = Path.home() / ".smartsim" / "keys"
+        return os.environ.get("SMARTSIM_KEY_PATH", str(default_path))
+
+    @property
+    def dragon_pin(self) -> str:
+        return "0.9"
+
 
 @lru_cache(maxsize=128, typed=False)
 def get_config() -> Config:
     # wrap into a function with a cached result
     return Config()
```

### Comparing `smartsim-0.6.2/smartsim/_core/config/keydb.conf` & `smartsim-0.7.0/smartsim/_core/config/keydb.conf`

 * *Files identical despite different names*

### Comparing `smartsim-0.6.2/smartsim/_core/config/redis.conf` & `smartsim-0.7.0/smartsim/_core/config/redis.conf`

 * *Files identical despite different names*

### Comparing `smartsim-0.6.2/smartsim/_core/control/__init__.py` & `smartsim-0.7.0/smartsim/_core/control/__init__.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.6.2/smartsim/_core/control/controller.py` & `smartsim-0.7.0/smartsim/_core/control/controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,58 +23,71 @@
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from __future__ import annotations
 
 import itertools
+import os
 import os.path as osp
 import pathlib
 import pickle
 import signal
 import subprocess
 import sys
 import threading
 import time
 import typing as t
-from os import environ
 
 from smartredis import Client, ConfigOptions
 
 from smartsim._core.utils.network import get_ip_from_host
 
 from ..._core.launcher.step import Step
-from ..._core.utils.helpers import unpack_colo_db_identifier, unpack_db_identifier
+from ..._core.utils.helpers import (
+    SignalInterceptionStack,
+    unpack_colo_db_identifier,
+    unpack_db_identifier,
+)
 from ..._core.utils.redis import (
     db_is_active,
     set_ml_model,
     set_script,
     shutdown_db_node,
 )
 from ...database import Orchestrator
-from ...entity import Ensemble, EntityList, EntitySequence, Model, SmartSimEntity
+from ...entity import Ensemble, EntitySequence, Model, SmartSimEntity
 from ...error import (
     LauncherError,
     SmartSimError,
     SSDBIDConflictError,
     SSInternalError,
     SSUnsupportedError,
 )
 from ...log import get_logger
 from ...servertype import CLUSTERED, STANDALONE
-from ...status import STATUS_CANCELLED, STATUS_RUNNING, TERMINAL_STATUSES
+from ...status import TERMINAL_STATUSES, SmartSimStatus
 from ..config import CONFIG
-from ..launcher import LocalLauncher, LSFLauncher, PBSLauncher, SlurmLauncher
+from ..launcher import (
+    DragonLauncher,
+    LocalLauncher,
+    LSFLauncher,
+    PBSLauncher,
+    SlurmLauncher,
+)
 from ..launcher.launcher import Launcher
 from ..utils import check_cluster_status, create_cluster, serialize
+from .controller_utils import _AnonymousBatchJob, _look_up_launched_data
 from .job import Job
 from .jobmanager import JobManager
 from .manifest import LaunchedManifest, LaunchedManifestBuilder, Manifest
 
 if t.TYPE_CHECKING:
+    from types import FrameType
+
     from ..utils.serialize import TStepLaunchMetaData
 
 
 logger = get_logger(__name__)
 
 # job manager lock
 JM_LOCK = threading.RLock()
@@ -86,15 +99,14 @@
     underlying workload manager or run framework.
     """
 
     def __init__(self, launcher: str = "local") -> None:
         """Initialize a Controller
 
         :param launcher: the type of launcher being used
-        :type launcher: str
         """
         self._jobs = JobManager(JM_LOCK)
         self.init_launcher(launcher)
         self._telemetry_monitor: t.Optional[subprocess.Popen[bytes]] = None
 
     def start(
         self,
@@ -108,55 +120,60 @@
 
         This function should not be called directly, but rather
         through the experiment interface.
 
         The controller will start the job-manager thread upon
         execution of all jobs.
         """
+        # launch a telemetry monitor to track job progress
+        if CONFIG.telemetry_enabled:
+            self._start_telemetry_monitor(exp_path)
+
         self._jobs.kill_on_interrupt = kill_on_interrupt
+
         # register custom signal handler for ^C (SIGINT)
-        signal.signal(signal.SIGINT, self._jobs.signal_interrupt)
+        SignalInterceptionStack.get(signal.SIGINT).push_unique(
+            self._jobs.signal_interrupt
+        )
         launched = self._launch(exp_name, exp_path, manifest)
 
         # start the job manager thread if not already started
         if not self._jobs.actively_monitoring:
             self._jobs.start()
 
         serialize.save_launch_manifest(
             launched.map(_look_up_launched_data(self._launcher))
         )
 
-        # launch a telemetry monitor to track job progress
-        if CONFIG.telemetry_enabled:
-            self._start_telemetry_monitor(exp_path)
-
         # block until all non-database jobs are complete
         if block:
             # poll handles its own keyboard interrupt as
-            # it may be called seperately
+            # it may be called separately
             self.poll(5, True, kill_on_interrupt=kill_on_interrupt)
 
     @property
+    def active_orchestrator_jobs(self) -> t.Dict[str, Job]:
+        """Return active orchestrator jobs."""
+        return {**self._jobs.db_jobs}
+
+    @property
     def orchestrator_active(self) -> bool:
         with JM_LOCK:
             if len(self._jobs.db_jobs) > 0:
                 return True
             return False
 
     def poll(
         self, interval: int, verbose: bool, kill_on_interrupt: bool = True
     ) -> None:
         """Poll running jobs and receive logging output of job status
 
         :param interval: number of seconds to wait before polling again
-        :type interval: int
         :param verbose: set verbosity
-        :type verbose: bool
         :param kill_on_interrupt: flag for killing jobs when SIGINT is received
-        :type kill_on_interrupt: bool, optional
         """
         self._jobs.kill_on_interrupt = kill_on_interrupt
         to_monitor = self._jobs.jobs
         while len(to_monitor) > 0:
             time.sleep(interval)
 
             # acquire lock to avoid "dictionary changed during iteration" error
@@ -168,15 +185,14 @@
 
     def finished(
         self, entity: t.Union[SmartSimEntity, EntitySequence[SmartSimEntity]]
     ) -> bool:
         """Return a boolean indicating wether a job has finished or not
 
         :param entity: object launched by SmartSim.
-        :type entity: Entity | EntitySequence
         :returns: bool
         :raises ValueError: if entity has not been launched yet
         """
         try:
             if isinstance(entity, Orchestrator):
                 raise TypeError("Finished() does not support Orchestrator instances")
             if isinstance(entity, EntitySequence):
@@ -198,15 +214,14 @@
     ) -> None:
         """Stop an instance of an entity
 
         This function will also update the status of the job in
         the jobmanager so that the job appears as "cancelled".
 
         :param entity: entity to be stopped
-        :type entity: Entity | EntitySequence
         """
         with JM_LOCK:
             job = self._jobs[entity.name]
             if job.status not in TERMINAL_STATUSES:
                 logger.info(
                     " ".join(
                         ("Stopping model", entity.name, "with job name", str(job.name))
@@ -221,16 +236,16 @@
                     error=status.error,
                     output=status.output,
                 )
                 self._jobs.move_to_completed(job)
 
     def stop_db(self, db: Orchestrator) -> None:
         """Stop an orchestrator
+
         :param db: orchestrator to be stopped
-        :type db: Orchestrator
         """
         if db.batch:
             self.stop_entity(db)
         else:
             with JM_LOCK:
                 for node in db.entities:
                     for host_ip, port in itertools.product(
@@ -239,24 +254,29 @@
                         retcode, _, _ = shutdown_db_node(host_ip, port)
                         # Sometimes the DB will not shutdown (unless we force NOSAVE)
                         if retcode != 0:
                             self.stop_entity(node)
                             continue
 
                         job = self._jobs[node.name]
-                        job.set_status(STATUS_CANCELLED, "", 0, output=None, error=None)
+                        job.set_status(
+                            SmartSimStatus.STATUS_CANCELLED,
+                            "",
+                            0,
+                            output=None,
+                            error=None,
+                        )
                         self._jobs.move_to_completed(job)
 
         db.reset_hosts()
 
     def stop_entity_list(self, entity_list: EntitySequence[SmartSimEntity]) -> None:
         """Stop an instance of an entity list
 
         :param entity_list: entity list to be stopped
-        :type entity_list: EntitySequence
         """
 
         if entity_list.batch:
             self.stop_entity(entity_list)
         else:
             for entity in entity_list.entities:
                 self.stop_entity(entity)
@@ -267,41 +287,37 @@
         :returns: dict[str, Job]
         """
         with JM_LOCK:
             return self._jobs.completed
 
     def get_entity_status(
         self, entity: t.Union[SmartSimEntity, EntitySequence[SmartSimEntity]]
-    ) -> str:
+    ) -> SmartSimStatus:
         """Get the status of an entity
 
         :param entity: entity to get status of
-        :type entity: SmartSimEntity | EntitySequence
         :raises TypeError: if not SmartSimEntity | EntitySequence
         :return: status of entity
-        :rtype: str
         """
         if not isinstance(entity, (SmartSimEntity, EntitySequence)):
             raise TypeError(
                 "Argument must be of type SmartSimEntity or EntitySequence, "
                 f"not {type(entity)}"
             )
         return self._jobs.get_status(entity)
 
     def get_entity_list_status(
         self, entity_list: EntitySequence[SmartSimEntity]
-    ) -> t.List[str]:
+    ) -> t.List[SmartSimStatus]:
         """Get the statuses of an entity list
 
         :param entity_list: entity list containing entities to
                             get statuses of
-        :type entity_list: EntitySequence
         :raises TypeError: if not EntitySequence
-        :return: list of str statuses
-        :rtype: list
+        :return: list of SmartSimStatus statuses
         """
         if not isinstance(entity_list, EntitySequence):
             raise TypeError(
                 f"Argument was of type {type(entity_list)} not EntitySequence"
             )
         if entity_list.batch:
             return [self.get_entity_status(entity_list)]
@@ -312,56 +328,86 @@
 
     def init_launcher(self, launcher: str) -> None:
         """Initialize the controller with a specific type of launcher.
         SmartSim currently supports slurm, pbs(pro), lsf,
         and local launching
 
         :param launcher: which launcher to initialize
-        :type launcher: str
         :raises SSUnsupportedError: if a string is passed that is not
                                     a supported launcher
         :raises TypeError: if no launcher argument is provided.
         """
         launcher_map: t.Dict[str, t.Type[Launcher]] = {
             "slurm": SlurmLauncher,
             "pbs": PBSLauncher,
             "pals": PBSLauncher,
             "lsf": LSFLauncher,
             "local": LocalLauncher,
+            "dragon": DragonLauncher,
         }
 
         if launcher is not None:
             launcher = launcher.lower()
             if launcher in launcher_map:
                 # create new instance of the launcher
                 self._launcher = launcher_map[launcher]()
                 self._jobs.set_launcher(self._launcher)
             else:
                 raise SSUnsupportedError("Launcher type not supported: " + launcher)
         else:
             raise TypeError("Must provide a 'launcher' argument")
 
+    @staticmethod
+    def symlink_output_files(
+        job_step: Step, entity: t.Union[SmartSimEntity, EntitySequence[SmartSimEntity]]
+    ) -> None:
+        """Create symlinks for entity output files that point to the output files
+        under the .smartsim directory
+
+        :param job_step: Job step instance
+        :param entity: Entity instance
+        """
+        historical_out, historical_err = map(pathlib.Path, job_step.get_output_files())
+        entity_out = pathlib.Path(entity.path) / f"{entity.name}.out"
+        entity_err = pathlib.Path(entity.path) / f"{entity.name}.err"
+
+        # check if there is already a link to a previous run
+        if entity_out.is_symlink() or entity_err.is_symlink():
+            entity_out.unlink()
+            entity_err.unlink()
+
+        historical_err.touch()
+        historical_out.touch()
+
+        if historical_err.exists() and historical_out.exists():
+            entity_out.symlink_to(historical_out)
+            entity_err.symlink_to(historical_err)
+        else:
+            raise FileNotFoundError(
+                f"Output files for {entity.name} could not be found. "
+                "Symlinking files failed."
+            )
+
     def _launch(
         self, exp_name: str, exp_path: str, manifest: Manifest
     ) -> LaunchedManifest[t.Tuple[str, Step]]:
         """Main launching function of the controller
 
         Orchestrators are always launched first so that the
         address of the database can be given to following entities
 
         :param exp_name: The name of the launching experiment
-        :type exp_name: str
         :param exp_path: path to location of ``Experiment`` directory if generated
-        :type exp_path: str
         :param manifest: Manifest of deployables to launch
-        :type manifest: Manifest
         """
 
         manifest_builder = LaunchedManifestBuilder[t.Tuple[str, Step]](
-            exp_name=exp_name, exp_path=exp_path, launcher_name=str(self._launcher)
+            exp_name=exp_name,
+            exp_path=exp_path,
+            launcher_name=str(self._launcher),
         )
         # Loop over deployables to launch and launch multiple orchestrators
         for orchestrator in manifest.dbs:
             for key in self._jobs.get_db_host_addresses():
                 _, db_id = unpack_db_identifier(key, "_")
                 if orchestrator.db_identifier == db_id:
                     raise SSDBIDConflictError(
@@ -381,21 +427,31 @@
         if self.orchestrator_active:
             self._set_dbobjects(manifest)
 
         # create all steps prior to launch
         steps: t.List[
             t.Tuple[Step, t.Union[SmartSimEntity, EntitySequence[SmartSimEntity]]]
         ] = []
+
+        symlink_substeps: t.List[
+            t.Tuple[Step, t.Union[SmartSimEntity, EntitySequence[SmartSimEntity]]]
+        ] = []
+
         for elist in manifest.ensembles:
             ens_telem_dir = manifest_builder.run_telemetry_subdirectory / "ensemble"
             if elist.batch:
                 batch_step, substeps = self._create_batch_job_step(elist, ens_telem_dir)
                 manifest_builder.add_ensemble(
                     elist, [(batch_step.name, step) for step in substeps]
                 )
+
+                # symlink substeps to maintain directory structure
+                for substep, substep_entity in zip(substeps, elist.models):
+                    symlink_substeps.append((substep, substep_entity))
+
                 steps.append((batch_step, elist))
             else:
                 # if ensemble is to be run as separate job steps, aka not in a batch
                 job_steps = [
                     (self._create_job_step(e, ens_telem_dir / elist.name), e)
                     for e in elist.entities
                 ]
@@ -405,27 +461,34 @@
                 steps.extend(job_steps)
         # models themselves cannot be batch steps. If batch settings are
         # attached, wrap them in an anonymous batch job step
         for model in manifest.models:
             model_telem_dir = manifest_builder.run_telemetry_subdirectory / "model"
             if model.batch_settings:
                 anon_entity_list = _AnonymousBatchJob(model)
-                batch_step, _ = self._create_batch_job_step(
+                batch_step, substeps = self._create_batch_job_step(
                     anon_entity_list, model_telem_dir
                 )
                 manifest_builder.add_model(model, (batch_step.name, batch_step))
+
+                symlink_substeps.append((substeps[0], model))
                 steps.append((batch_step, model))
             else:
                 job_step = self._create_job_step(model, model_telem_dir)
                 manifest_builder.add_model(model, (job_step.name, job_step))
                 steps.append((job_step, model))
 
-        # launch steps
+        # launch and symlink steps
         for step, entity in steps:
             self._launch_step(step, entity)
+            self.symlink_output_files(step, entity)
+
+        # symlink substeps to maintain directory structure
+        for substep, entity in symlink_substeps:
+            self.symlink_output_files(substep, entity)
 
         return manifest_builder.finalize()
 
     def _launch_orchestrator(
         self,
         orchestrator: Orchestrator,
         manifest_builder: LaunchedManifestBuilder[t.Tuple[str, Step]],
@@ -433,43 +496,48 @@
         """Launch an Orchestrator instance
 
         This function will launch the Orchestrator instance and
         if on WLM, find the nodes where it was launched and
         set them in the JobManager
 
         :param orchestrator: orchestrator to launch
-        :type orchestrator: Orchestrator
         :param manifest_builder: An `LaunchedManifestBuilder` to record the
                                  names and `Step`s of the launched orchestrator
-        :type manifest_builder: LaunchedManifestBuilder[tuple[str, Step]]
         """
         orchestrator.remove_stale_files()
         orc_telem_dir = manifest_builder.run_telemetry_subdirectory / "database"
 
         # if the orchestrator was launched as a batch workload
         if orchestrator.batch:
             orc_batch_step, substeps = self._create_batch_job_step(
                 orchestrator, orc_telem_dir
             )
             manifest_builder.add_database(
                 orchestrator, [(orc_batch_step.name, step) for step in substeps]
             )
+
             self._launch_step(orc_batch_step, orchestrator)
+            self.symlink_output_files(orc_batch_step, orchestrator)
+
+            # symlink substeps to maintain directory structure
+            for substep, substep_entity in zip(substeps, orchestrator.entities):
+                self.symlink_output_files(substep, substep_entity)
 
         # if orchestrator was run on existing allocation, locally, or in allocation
         else:
             db_steps = [
                 (self._create_job_step(db, orc_telem_dir / orchestrator.name), db)
                 for db in orchestrator.entities
             ]
             manifest_builder.add_database(
                 orchestrator, [(step.name, step) for step, _ in db_steps]
             )
             for db_step in db_steps:
                 self._launch_step(*db_step)
+                self.symlink_output_files(*db_step)
 
         # wait for orchestrator to spin up
         self._orchestrator_launch_wait(orchestrator)
 
         # set the jobs in the job manager to provide SSDB variable to entities
         # if _host isnt set within each
         self._jobs.set_db_hosts(orchestrator)
@@ -502,27 +570,51 @@
         self,
         job_step: Step,
         entity: t.Union[SmartSimEntity, EntitySequence[SmartSimEntity]],
     ) -> None:
         """Use the launcher to launch a job step
 
         :param job_step: a job step instance
-        :type job_step: Step
         :param entity: entity instance
-        :type entity: SmartSimEntity
         :raises SmartSimError: if launch fails
         """
-        try:
-            job_id = self._launcher.run(job_step)
-        except LauncherError as e:
-            msg = f"An error occurred when launching {entity.name} \n"
-            msg += "Check error and output files for details.\n"
-            msg += f"{entity}"
-            logger.error(msg)
-            raise SmartSimError(f"Job step {entity.name} failed to launch") from e
+        # attempt to retrieve entity name in JobManager.completed
+        completed_job = self._jobs.completed.get(entity.name, None)
+
+        # if completed job DNE and is the entity name is not
+        # running in JobManager.jobs or JobManager.db_jobs,
+        # launch the job
+        if completed_job is None and (
+            entity.name not in self._jobs.jobs and entity.name not in self._jobs.db_jobs
+        ):
+            try:
+                job_id = self._launcher.run(job_step)
+            except LauncherError as e:
+                msg = f"An error occurred when launching {entity.name} \n"
+                msg += "Check error and output files for details.\n"
+                msg += f"{entity}"
+                logger.error(msg)
+                raise SmartSimError(f"Job step {entity.name} failed to launch") from e
+
+        # if the completed job does exist and the entity passed in is the same
+        # that has ran and completed, relaunch the entity.
+        elif completed_job is not None and completed_job.entity is entity:
+            try:
+                job_id = self._launcher.run(job_step)
+            except LauncherError as e:
+                msg = f"An error occurred when launching {entity.name} \n"
+                msg += "Check error and output files for details.\n"
+                msg += f"{entity}"
+                logger.error(msg)
+                raise SmartSimError(f"Job step {entity.name} failed to launch") from e
+
+        # the entity is using a duplicate name of an existing entity in
+        # the experiment, throw an error
+        else:
+            raise SSUnsupportedError("SmartSim entities cannot have duplicate names.")
 
         # a job step is a task if it is not managed by a workload manager (i.e. Slurm)
         # but is rather started, monitored, and exited through the Popen interface
         # in the taskmanager
         is_task = not job_step.managed
 
         if self._jobs.query_restart(entity.name):
@@ -536,33 +628,30 @@
         self,
         entity_list: t.Union[Orchestrator, Ensemble, _AnonymousBatchJob],
         telemetry_dir: pathlib.Path,
     ) -> t.Tuple[Step, t.List[Step]]:
         """Use launcher to create batch job step
 
         :param entity_list: EntityList to launch as batch
-        :type entity_list: EntityList
         :param telemetry_dir: Path to a directory in which the batch job step
                               may write telemetry events
-        :type telemetry_dir: pathlib.Path
         :return: batch job step instance and a list of run steps to be
                  executed within the batch job
-        :rtype: tuple[Step, list[Step]]
         """
         if not entity_list.batch_settings:
             raise ValueError(
                 "EntityList must have batch settings to be launched as batch"
             )
 
         telemetry_dir = telemetry_dir / entity_list.name
         batch_step = self._launcher.create_step(
             entity_list.name, entity_list.path, entity_list.batch_settings
         )
         batch_step.meta["entity_type"] = str(type(entity_list).__name__).lower()
-        batch_step.meta["status_dir"] = str(telemetry_dir / entity_list.name)
+        batch_step.meta["status_dir"] = str(telemetry_dir)
 
         substeps = []
         for entity in entity_list.entities:
             # tells step creation not to look for an allocation
             entity.run_settings.in_batch = True
             step = self._create_job_step(entity, telemetry_dir)
             substeps.append(step)
@@ -571,20 +660,17 @@
 
     def _create_job_step(
         self, entity: SmartSimEntity, telemetry_dir: pathlib.Path
     ) -> Step:
         """Create job steps for all entities with the launcher
 
         :param entity: an entity to create a step for
-        :type entity: SmartSimEntity
         :param telemetry_dir: Path to a directory in which the job step
                                may write telemetry events
-        :type telemetry_dir: pathlib.Path
         :return: the job step
-        :rtype: Step
         """
         # get SSDB, SSIN, SSOUT and add to entity run settings
         if isinstance(entity, Model):
             self._prep_entity_client_env(entity)
 
         step = self._launcher.create_step(entity.name, entity.path, entity.run_settings)
 
@@ -593,15 +679,14 @@
 
         return step
 
     def _prep_entity_client_env(self, entity: Model) -> None:
         """Retrieve all connections registered to this entity
 
         :param entity: The entity to retrieve connections from
-        :type entity:  Model
         """
 
         client_env: t.Dict[str, t.Union[str, int, float, bool]] = {}
         address_dict = self._jobs.get_db_host_addresses()
 
         for db_id, addresses in address_dict.items():
             db_name, _ = unpack_db_identifier(db_id, "_")
@@ -658,37 +743,47 @@
         """Save the orchestrator object via pickle
 
         This function saves the orchestrator information to a pickle
         file that can be imported by subsequent experiments to reconnect
         to the orchestrator.
 
         :param orchestrator: Orchestrator configuration to be saved
-        :type orchestrator: Orchestrator
         """
 
-        dat_file = "/".join((orchestrator.path, "smartsim_db.dat"))
-        db_jobs = self._jobs.db_jobs
-        orc_data = {"db": orchestrator, "db_jobs": db_jobs}
-        steps = []
-        for db_job in db_jobs.values():
-            steps.append(self._launcher.step_mapping[db_job.name])
-        orc_data["steps"] = steps
-        with open(dat_file, "wb") as pickle_file:
+        if not orchestrator.is_active():
+            raise Exception("Orchestrator is not running")
+
+        # Extract only the db_jobs associated with this particular orchestrator
+        if orchestrator.batch:
+            job_names = [orchestrator.name]
+        else:
+            job_names = [dbnode.name for dbnode in orchestrator.entities]
+        db_jobs = {
+            name: job for name, job in self._jobs.db_jobs.items() if name in job_names
+        }
+
+        # Extract the associated steps
+        steps = [
+            self._launcher.step_mapping[db_job.name] for db_job in db_jobs.values()
+        ]
+
+        orc_data = {"db": orchestrator, "db_jobs": db_jobs, "steps": steps}
+
+        with open(orchestrator.checkpoint_file, "wb") as pickle_file:
             pickle.dump(orc_data, pickle_file)
 
     def _orchestrator_launch_wait(self, orchestrator: Orchestrator) -> None:
         """Wait for the orchestrator instances to run
 
         In the case where the orchestrator is launched as a batch
         through a WLM, we wait for the orchestrator to exit the
         queue before proceeding so new launched entities can
         be launched with SSDB address
 
         :param orchestrator: orchestrator instance
-        :type orchestrator: Orchestrator
         :raises SmartSimError: if launch fails or manually stopped by user
         """
         if orchestrator.batch:
             logger.info("Orchestrator launched as a batch")
             logger.info("While queued, SmartSim will wait for Orchestrator to run")
             logger.info("CTRL+C interrupt to abort and cancel launch")
 
@@ -698,18 +793,17 @@
                 time.sleep(CONFIG.jm_interval)
                 # manually trigger job update if JM not running
                 if not self._jobs.actively_monitoring:
                     self._jobs.check_jobs()
 
                 # _jobs.get_status acquires JM lock for main thread, no need for locking
                 statuses = self.get_entity_list_status(orchestrator)
-                if all(stat == STATUS_RUNNING for stat in statuses):
+                if all(stat == SmartSimStatus.STATUS_RUNNING for stat in statuses):
                     ready = True
-                    # TODO remove in favor of by node status check
-                    time.sleep(CONFIG.jm_interval)
+                    # TODO: Add a node status check
                 elif any(stat in TERMINAL_STATUSES for stat in statuses):
                     self.stop_db(orchestrator)
                     msg = "Orchestrator failed during startup"
                     msg += f" See {orchestrator.path} for details"
                     raise SmartSimError(msg)
                 else:
                     logger.debug("Waiting for orchestrator instances to spin up...")
@@ -719,22 +813,22 @@
 
                 # re-raise keyboard interrupt so the job manager will display
                 # any running and un-killed jobs as this method is only called
                 # during launch and we handle all keyboard interrupts during
                 # launch explicitly
                 raise
 
-    def reload_saved_db(self, checkpoint_file: str) -> Orchestrator:
+    def reload_saved_db(
+        self, checkpoint_file: t.Union[str, os.PathLike[str]]
+    ) -> Orchestrator:
         with JM_LOCK:
-            if self.orchestrator_active:
-                raise SmartSimError("Orchestrator exists and is active")
 
             if not osp.exists(checkpoint_file):
                 raise FileNotFoundError(
-                    f"The SmartSim database config file {checkpoint_file} "
+                    f"The SmartSim database config file {os.fspath(checkpoint_file)} "
                     "cannot be found."
                 )
 
             try:
                 with open(checkpoint_file, "rb") as pickle_file:
                     db_config = pickle.load(pickle_file)
             except (OSError, IOError) as e:
@@ -762,15 +856,15 @@
 
             # TODO check that each db_object is running
 
             job_steps = zip(db_config["db_jobs"].values(), db_config["steps"])
             try:
                 for db_job, step in job_steps:
                     self._jobs.db_jobs[db_job.ename] = db_job
-                    self._launcher.step_mapping[db_job.name] = step
+                    self._launcher.add_step_to_mapping_table(db_job.name, step)
                     if step.task_id:
                         self._launcher.task_manager.add_existing(int(step.task_id))
             except LauncherError as e:
                 raise SmartSimError("Failed to reconnect orchestrator") from e
 
             # start job manager if not already started
             if not self._jobs.actively_monitoring:
@@ -791,17 +885,17 @@
 
             hosts = list({address.split(":")[0] for address in db_addresses})
             ports = list({int(address.split(":")[-1]) for address in db_addresses})
 
             if not db_is_active(hosts=hosts, ports=ports, num_shards=len(db_addresses)):
                 raise SSInternalError("Cannot set DB Objects, DB is not running")
 
-            environ[f"SSDB{db_name}"] = db_addresses[0]
+            os.environ[f"SSDB{db_name}"] = db_addresses[0]
 
-            environ[f"SR_DB_TYPE{db_name}"] = (
+            os.environ[f"SR_DB_TYPE{db_name}"] = (
                 CLUSTERED if len(db_addresses) > 1 else STANDALONE
             )
 
             options = ConfigOptions.create_from_environment(name)
             client = Client(options, logger_name="SmartSim")
 
             for model in manifest.models:
@@ -829,15 +923,14 @@
                                 set_script(db_script, client)
 
     def _start_telemetry_monitor(self, exp_dir: str) -> None:
         """Spawns a telemetry monitor process to keep track of the life times
         of the processes launched through this controller.
 
         :param exp_dir: An experiment directory
-        :type exp_dir: str
         """
         if (
             self._telemetry_monitor is None
             or self._telemetry_monitor.returncode is not None
         ):
             logger.debug("Starting telemetry monitor process")
             cmd = [
@@ -855,47 +948,7 @@
             self._telemetry_monitor = subprocess.Popen(
                 cmd,
                 stderr=sys.stderr,
                 stdout=sys.stdout,
                 cwd=str(pathlib.Path(__file__).parent.parent.parent),
                 shell=False,
             )
-            logger.debug("Telemetry monitor started")
-
-
-class _AnonymousBatchJob(EntityList[Model]):
-    @staticmethod
-    def _validate(model: Model) -> None:
-        if model.batch_settings is None:
-            msg = "Unable to create _AnonymousBatchJob without batch_settings"
-            raise SmartSimError(msg)
-
-    def __init__(self, model: Model) -> None:
-        self._validate(model)
-        super().__init__(model.name, model.path)
-        self.entities = [model]
-        self.batch_settings = model.batch_settings
-
-    def _initialize_entities(self, **kwargs: t.Any) -> None: ...
-
-
-def _look_up_launched_data(
-    launcher: Launcher,
-) -> t.Callable[[t.Tuple[str, Step]], "TStepLaunchMetaData"]:
-    def _unpack_launched_data(data: t.Tuple[str, Step]) -> "TStepLaunchMetaData":
-        # NOTE: we cannot assume that the name of the launched step
-        # ``launched_step_name`` is equal to the name of the step referring to
-        # the entity ``step.name`` as is the case when an entity list is
-        # launched as a batch job
-        launched_step_name, step = data
-        launched_step_map = launcher.step_mapping[launched_step_name]
-        out_file, err_file = step.get_output_files()
-        return (
-            launched_step_map.step_id,
-            launched_step_map.task_id,
-            launched_step_map.managed,
-            out_file,
-            err_file,
-            pathlib.Path(step.meta.get("status_dir", step.cwd)),
-        )
-
-    return _unpack_launched_data
```

### Comparing `smartsim-0.6.2/smartsim/_core/control/job.py` & `smartsim-0.7.0/smartsim/_core/control/job.py`

 * *Files 26% similar despite different names*

```diff
@@ -20,54 +20,178 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+import pathlib
 import time
 import typing as t
 from dataclasses import dataclass
 
 from ...entity import EntitySequence, SmartSimEntity
-from ...status import STATUS_NEW
+from ...status import SmartSimStatus
 
 
 @dataclass(frozen=True)
 class _JobKey:
+    """A helper class for creating unique lookup keys within the telemetry
+    monitor. These keys are not guaranteed to be unique across experiments,
+    only within an experiment (due to process ID re-use by the OS)"""
+
     step_id: str
+    """The process id of an unmanaged task"""
     task_id: str
+    """The task id of a managed task"""
 
 
 class JobEntity:
-    """API required for a job processed in the JobManager with support for
-    telemetry monitoring
+    """An entity containing run-time SmartSimEntity metadata. The run-time metadata
+    is required to perform telemetry collection. The `JobEntity` satisfies the core
+    API necessary to use a `JobManager` to manage retrieval of managed step updates.
     """
 
     def __init__(self) -> None:
         self.name: str = ""
+        """The entity name"""
         self.path: str = ""
+        """The root path for entity output files"""
         self.step_id: str = ""
+        """The process id of an unmanaged task"""
         self.task_id: str = ""
+        """The task id of a managed task"""
         self.type: str = ""
+        """The type of the associated `SmartSimEntity`"""
         self.timestamp: int = 0
+        """The timestamp when the entity was created"""
         self.status_dir: str = ""
+        """The path configured by the experiment for the entities telemetry output"""
+        self.telemetry_on: bool = False
+        """"Flag indicating if optional telemetry is enabled for the entity"""
+        self.collectors: t.Dict[str, str] = {}
+        """Mapping of collectors enabled for the entity"""
+        self.config: t.Dict[str, str] = {}
+        """Telemetry configuration supplied by the experiment"""
+        self._is_complete: bool = False
+        """Flag indicating if the entity has completed execution"""
 
     @property
     def is_db(self) -> bool:
+        """Returns `True` if the entity represents a database or database shard"""
         return self.type in ["orchestrator", "dbnode"]
 
     @property
     def is_managed(self) -> bool:
+        """Returns `True` if the entity is managed by a workload manager"""
         return bool(self.step_id)
 
     @property
     def key(self) -> _JobKey:
+        """Return a `_JobKey` that identifies an entity.
+        NOTE: not guaranteed to be unique over time due to reused process IDs"""
         return _JobKey(self.step_id, self.task_id)
 
+    @property
+    def is_complete(self) -> bool:
+        """Returns `True` if the entity has completed execution"""
+        return self._is_complete
+
+    def check_completion_status(self) -> None:
+        """Check for telemetry outputs indicating the entity has completed
+        TODO: determine correct location to avoid exposing telemetry
+        implementation details into `JobEntity`
+        """
+        # avoid touching file-system if not necessary
+        if self._is_complete:
+            return
+
+        # status telemetry is tracked in JSON files written to disk. look
+        # for a corresponding `stop` event in the entity status directory
+        state_file = pathlib.Path(self.status_dir) / "stop.json"
+        if state_file.exists():
+            self._is_complete = True
+
+    @staticmethod
+    def _map_db_metadata(entity_dict: t.Dict[str, t.Any], entity: "JobEntity") -> None:
+        """Map DB-specific properties from a runtime manifest onto a `JobEntity`
+
+        :param entity_dict: The raw dictionary deserialized from manifest JSON
+        :param entity: The entity instance to modify
+        """
+        if entity.is_db:
+            # add collectors if they're configured to be enabled in the manifest
+            entity.collectors = {
+                "client": entity_dict.get("client_file", ""),
+                "client_count": entity_dict.get("client_count_file", ""),
+                "memory": entity_dict.get("memory_file", ""),
+            }
+
+            entity.telemetry_on = any(entity.collectors.values())
+            entity.config["host"] = entity_dict.get("hostname", "")
+            entity.config["port"] = entity_dict.get("port", "")
+
+    @staticmethod
+    def _map_standard_metadata(
+        entity_type: str,
+        entity_dict: t.Dict[str, t.Any],
+        entity: "JobEntity",
+        exp_dir: str,
+        raw_experiment: t.Dict[str, t.Any],
+    ) -> None:
+        """Map universal properties from a runtime manifest onto a `JobEntity`
+
+        :param entity_type: The type of the associated `SmartSimEntity`
+        :param entity_dict: The raw dictionary deserialized from manifest JSON
+        :param entity: The entity instance to modify
+        :param exp_dir: The path to the experiment working directory
+        :param raw_experiment: The raw experiment dictionary deserialized from
+        manifest JSON
+        """
+        metadata = entity_dict["telemetry_metadata"]
+        status_dir = pathlib.Path(metadata.get("status_dir"))
+        is_dragon = raw_experiment["launcher"].lower() == "dragon"
+
+        # all entities contain shared properties that identify the task
+        entity.type = entity_type
+        entity.name = (
+            entity_dict["name"]
+            if not is_dragon
+            else entity_dict["telemetry_metadata"]["step_id"]
+        )
+        entity.step_id = str(metadata.get("step_id") or "")
+        entity.task_id = str(metadata.get("task_id") or "")
+        entity.timestamp = int(entity_dict.get("timestamp", "0"))
+        entity.path = str(exp_dir)
+        entity.status_dir = str(status_dir)
+
+    @classmethod
+    def from_manifest(
+        cls,
+        entity_type: str,
+        entity_dict: t.Dict[str, t.Any],
+        exp_dir: str,
+        raw_experiment: t.Dict[str, t.Any],
+    ) -> "JobEntity":
+        """Instantiate a `JobEntity` from the dictionary deserialized from manifest JSON
+
+        :param entity_type: The type of the associated `SmartSimEntity`
+        :param entity_dict: The raw dictionary deserialized from manifest JSON
+        :param exp_dir: The path to the experiment working directory
+        :param raw_experiment: raw experiment deserialized from manifest JSON
+        """
+        entity = JobEntity()
+
+        cls._map_standard_metadata(
+            entity_type, entity_dict, entity, exp_dir, raw_experiment
+        )
+        cls._map_db_metadata(entity_dict, entity)
+
+        return entity
+
 
 class Job:
     """Keep track of various information for the controller.
     In doing so, continuously add various fields of information
     that is queryable by the user through interface methods in
     the controller class.
     """
@@ -79,28 +203,23 @@
         entity: t.Union[SmartSimEntity, EntitySequence[SmartSimEntity], JobEntity],
         launcher: str,
         is_task: bool,
     ) -> None:
         """Initialize a Job.
 
         :param job_name: Name of the job step
-        :type job_name: str
         :param job_id: The id associated with the job
-        :type job_id: str
         :param entity: The SmartSim entity(list) associated with the job
-        :type entity: SmartSimEntity | EntitySequence | JobEntity
         :param launcher: Launcher job was started with
-        :type launcher: str
         :param is_task: process monitored by TaskManager (True) or the WLM (True)
-        :type is_task: bool
         """
         self.name = job_name
         self.jid = job_id
         self.entity = entity
-        self.status = STATUS_NEW
+        self.status = SmartSimStatus.STATUS_NEW
         # status before smartsim status mapping is applied
         self.raw_status: t.Optional[str] = None
         self.returncode: t.Optional[int] = None
         # output is only populated if it's system related (e.g. cmd failed immediately)
         self.output: t.Optional[str] = None
         self.error: t.Optional[str] = None  # same as output
         self.hosts: t.List[str] = []  # currently only used for DB jobs
@@ -112,26 +231,27 @@
     @property
     def ename(self) -> str:
         """Return the name of the entity this job was created from"""
         return self.entity.name
 
     def set_status(
         self,
-        new_status: str,
+        new_status: SmartSimStatus,
         raw_status: str,
         returncode: t.Optional[int],
         error: t.Optional[str] = None,
         output: t.Optional[str] = None,
     ) -> None:
         """Set the status  of a job.
 
         :param new_status: The new status of the job
-        :type new_status: str
+        :param raw_status: The raw status of the launcher
         :param returncode: The return code for the job
-        :type return_code: str
+        :param error: Content produced by stderr
+        :param output: Content produced by stdout
         """
         self.status = new_status
         self.raw_status = raw_status
         self.returncode = returncode
         self.error = error
         self.output = output
 
@@ -145,36 +265,32 @@
 
     def reset(
         self, new_job_name: str, new_job_id: t.Optional[str], is_task: bool
     ) -> None:
         """Reset the job in order to be able to restart it.
 
         :param new_job_name: name of the new job step
-        :type new_job_name: str
         :param new_job_id: new job id to launch under
-        :type new_job_id: int
         :param is_task: process monitored by TaskManager (True) or the WLM (True)
-        :type is_task: bool
         """
         self.name = new_job_name
         self.jid = new_job_id
-        self.status = STATUS_NEW
+        self.status = SmartSimStatus.STATUS_NEW
         self.returncode = None
         self.output = None
         self.error = None
         self.hosts = []
         self.is_task = is_task
         self.start_time = time.time()
         self.history.new_run()
 
     def error_report(self) -> str:
         """A descriptive error report based on job fields
 
         :return: error report for display in terminal
-        :rtype: str
         """
         warning = f"{self.ename} failed. See below for details \n"
         if self.error:
             warning += (
                 f"{self.entity.type} {self.ename} produced the following error \n"
             )
             warning += f"Error: {self.error} \n"
@@ -186,15 +302,14 @@
         warning += f"Error and output file located at: {self.entity.path}"
         return warning
 
     def __str__(self) -> str:
         """Return user-readable string of the Job
 
         :returns: A user-readable string of the Job
-        :rtype: str
         """
         if self.jid:
             job = "{}({}): {}"
             return job.format(self.ename, self.jid, self.status)
 
         job = "{}: {}"
         return job.format(self.ename, self.status)
@@ -204,27 +319,26 @@
     """History of a job instance. Holds various attributes based
     on the previous launches of a job.
     """
 
     def __init__(self, runs: int = 0) -> None:
         """Init a history object for a job
 
-        :param runs: number of runs so far, defaults to 0
-        :type runs: int, optional
+        :param runs: number of runs so far
         """
         self.runs = runs
         self.jids: t.Dict[int, t.Optional[str]] = {}
-        self.statuses: t.Dict[int, str] = {}
+        self.statuses: t.Dict[int, SmartSimStatus] = {}
         self.returns: t.Dict[int, t.Optional[int]] = {}
         self.job_times: t.Dict[int, float] = {}
 
     def record(
         self,
         job_id: t.Optional[str],
-        status: str,
+        status: SmartSimStatus,
         returncode: t.Optional[int],
         job_time: float,
     ) -> None:
         """record the history of a job"""
         self.jids[self.runs] = job_id
         self.statuses[self.runs] = status
         self.returns[self.runs] = returncode
```

### Comparing `smartsim-0.6.2/smartsim/_core/control/jobmanager.py` & `smartsim-0.7.0/smartsim/_core/control/jobmanager.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from collections import ChainMap
 from threading import RLock, Thread
 from types import FrameType
 
 from ...database import Orchestrator
 from ...entity import DBNode, EntitySequence, SmartSimEntity
 from ...log import ContextThread, get_logger
-from ...status import STATUS_NEVER_STARTED, TERMINAL_STATUSES
+from ...status import TERMINAL_STATUSES, SmartSimStatus
 from ..config import CONFIG
 from ..launcher import Launcher, LocalLauncher
 from ..utils.network import get_ip_from_host
 from .job import Job, JobEntity
 
 logger = get_logger(__name__)
 
@@ -57,15 +57,14 @@
     wlm to query information about jobs that the user requests.
     """
 
     def __init__(self, lock: RLock, launcher: t.Optional[Launcher] = None) -> None:
         """Initialize a Jobmanager
 
         :param launcher: a Launcher object to manage jobs
-        :type: SmartSim.Launcher
         """
         self.monitor: t.Optional[Thread] = None
 
         # active jobs
         self.jobs: t.Dict[str, Job] = {}
         self.db_jobs: t.Dict[str, Job] = {}
 
@@ -120,15 +119,14 @@
                 logger.debug("Sleeping, no jobs to monitor")
 
     def move_to_completed(self, job: Job) -> None:
         """Move job to completed queue so that its no longer
            actively monitored by the job manager
 
         :param job: job instance we are transitioning
-        :type job: Job
         """
         with self._lock:
             self.completed[job.ename] = job
             job.record_history()
 
             # remove from actively monitored jobs
             if job.ename in self.db_jobs:
@@ -137,27 +135,24 @@
                 del self.jobs[job.ename]
 
     def __getitem__(self, entity_name: str) -> Job:
         """Return the job associated with the name of the entity
         from which it was created.
 
         :param entity_name: The name of the entity of a job
-        :type entity_name: str
         :returns: the Job associated with the entity_name
-        :rtype: Job
         """
         with self._lock:
             entities = ChainMap(self.db_jobs, self.jobs, self.completed)
             return entities[entity_name]
 
     def __call__(self) -> t.Dict[str, Job]:
         """Returns dictionary all jobs for () operator
 
         :returns: Dictionary of all jobs
-        :rtype: dictionary
         """
         all_jobs = {**self.jobs, **self.db_jobs}
         return all_jobs
 
     def __contains__(self, key: str) -> bool:
         try:
             self[key]  # pylint: disable=pointless-statement
@@ -171,21 +166,17 @@
         job_id: t.Optional[str],
         entity: t.Union[SmartSimEntity, EntitySequence[SmartSimEntity], JobEntity],
         is_task: bool = True,
     ) -> None:
         """Add a job to the job manager which holds specific jobs by type.
 
         :param job_name: name of the job step
-        :type job_name: str
         :param job_id: job step id created by launcher
-        :type job_id: str
         :param entity: entity that was launched on job step
-        :type entity: SmartSimEntity | EntitySequence
         :param is_task: process monitored by TaskManager (True) or the WLM (True)
-        :type is_task: bool
         """
         launcher = str(self._launcher)
         # all operations here should be atomic
         job = Job(job_name, job_id, entity, launcher, is_task)
         if isinstance(entity, (DBNode, Orchestrator)):
             self.db_jobs[entity.name] = job
         elif isinstance(entity, JobEntity) and entity.is_db:
@@ -193,17 +184,15 @@
         else:
             self.jobs[entity.name] = job
 
     def is_finished(self, entity: SmartSimEntity) -> bool:
         """Detect if a job has completed
 
         :param entity: entity to check
-        :type entity: SmartSimEntity
         :return: True if finished
-        :rtype: bool
         """
         with self._lock:
             job = self[entity.name]  # locked operation
             if entity.name in self.completed:
                 if job.status in TERMINAL_STATUSES:
                     return True
             return False
@@ -235,46 +224,42 @@
                             error=status.error,
                             output=status.output,
                         )
 
     def get_status(
         self,
         entity: t.Union[SmartSimEntity, EntitySequence[SmartSimEntity]],
-    ) -> str:
+    ) -> SmartSimStatus:
         """Return the status of a job.
 
         :param entity: SmartSimEntity or EntitySequence instance
-        :type entity: SmartSimEntity | EntitySequence
-        :returns: tuple of status
+        :returns: a SmartSimStatus status
         """
         with self._lock:
             if entity.name in self.completed:
                 return self.completed[entity.name].status
 
             if entity.name in self:
                 job: Job = self[entity.name]  # locked
                 return job.status
 
-            return STATUS_NEVER_STARTED
+            return SmartSimStatus.STATUS_NEVER_STARTED
 
     def set_launcher(self, launcher: Launcher) -> None:
         """Set the launcher of the job manager to a specific launcher instance
 
         :param launcher: child of Launcher
-        :type launcher: Launcher instance
         """
         self._launcher = launcher
 
     def query_restart(self, entity_name: str) -> bool:
         """See if the job just started should be restarted or not.
 
         :param entity_name: name of entity to check for a job for
-        :type entity_name: str
         :return: if job should be restarted instead of started
-        :rtype: bool
         """
         if entity_name in self.completed:
             return True
         return False
 
     def restart_job(
         self,
@@ -283,21 +268,17 @@
         entity_name: str,
         is_task: bool = True,
     ) -> None:
         """Function to reset a job to record history and be
         ready to launch again.
 
         :param job_name: new job step name
-        :type job_name: str
         :param job_id: new job id
-        :type job_id: str
         :param entity_name: name of the entity of the job
-        :type entity_name: str
         :param is_task: process monitored by TaskManager (True) or the WLM (True)
-        :type is_task: bool
 
         """
         with self._lock:
             job = self.completed[entity_name]
             del self.completed[entity_name]
             job.reset(job_name, job_id, is_task)
 
@@ -307,15 +288,14 @@
                 self.jobs[entity_name] = job
 
     def get_db_host_addresses(self) -> t.Dict[str, t.List[str]]:
         """Retrieve the list of hosts for the database
         for corresponding database identifiers
 
         :return: dictionary of host ip addresses
-        :rtype: Dict[str, list]
         """
 
         address_dict: t.Dict[str, t.List[str]] = {}
         for db_job in self.db_jobs.values():
             addresses = []
             if isinstance(db_job.entity, (DBNode, Orchestrator)):
                 db_entity = db_job.entity
@@ -329,15 +309,14 @@
 
         return address_dict
 
     def set_db_hosts(self, orchestrator: Orchestrator) -> None:
         """Set the DB hosts in db_jobs so future entities can query this
 
         :param orchestrator: orchestrator instance
-        :type orchestrator: Orchestrator
         """
         # should only be called during launch in the controller
 
         with self._lock:
             if orchestrator.batch:
                 self.db_jobs[orchestrator.name].hosts = orchestrator.hosts
 
@@ -345,17 +324,17 @@
                 for dbnode in orchestrator.entities:
                     if not dbnode.is_mpmd:
                         self.db_jobs[dbnode.name].hosts = [dbnode.host]
                     else:
                         self.db_jobs[dbnode.name].hosts = dbnode.hosts
 
     def signal_interrupt(self, signo: int, _frame: t.Optional[FrameType]) -> None:
+        """Custom handler for whenever SIGINT is received"""
         if not signo:
             logger.warning("Received SIGINT with no signal number")
-        """Custom handler for whenever SIGINT is received"""
         if self.actively_monitoring and len(self) > 0:
             if self.kill_on_interrupt:
                 for _, job in self().items():
                     if job.status not in TERMINAL_STATUSES and self._launcher:
                         self._launcher.stop(job.name)
             else:
                 logger.warning("SmartSim process interrupted before resource cleanup")
```

### Comparing `smartsim-0.6.2/smartsim/_core/control/manifest.py` & `smartsim-0.7.0/smartsim/_core/control/manifest.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,55 +64,59 @@
 
     @property
     def dbs(self) -> t.List[Orchestrator]:
         """Return a list of Orchestrator instances in Manifest
 
         :raises SmartSimError: if user added to databases to manifest
         :return: List of orchestrator instances
-        :rtype: list[Orchestrator]
         """
         dbs = [item for item in self._deployables if isinstance(item, Orchestrator)]
         return dbs
 
     @property
     def models(self) -> t.List[Model]:
         """Return Model instances in Manifest
 
         :return: model instances
-        :rtype: List[Model]
         """
         _models: t.List[Model] = [
             item for item in self._deployables if isinstance(item, Model)
         ]
         return _models
 
     @property
     def ensembles(self) -> t.List[Ensemble]:
         """Return Ensemble instances in Manifest
 
         :return: list of ensembles
-        :rtype: List[Ensemble]
         """
         return [e for e in self._deployables if isinstance(e, Ensemble)]
 
     @property
     def all_entity_lists(self) -> t.List[EntitySequence[SmartSimEntity]]:
         """All entity lists, including ensembles and
         exceptional ones like Orchestrator
 
         :return: list of entity lists
-        :rtype: List[EntitySequence[SmartSimEntity]]
         """
         _all_entity_lists: t.List[EntitySequence[SmartSimEntity]] = list(self.ensembles)
 
         for db in self.dbs:
             _all_entity_lists.append(db)
 
         return _all_entity_lists
 
+    @property
+    def has_deployable(self) -> bool:
+        """
+        Return True if the manifest contains entities that
+        must be physically deployed
+        """
+        return bool(self._deployables)
+
     @staticmethod
     def _check_names(deployables: t.List[t.Any]) -> None:
         used = []
         for deployable in deployables:
             name = getattr(deployable, "name", None)
             if not name:
                 raise AttributeError("Entity has no name. Please set name attribute.")
@@ -290,15 +294,18 @@
                 f"sequence of length {len(entities)}"
             )
         return tuple(zip(entities, data))
 
     def finalize(self) -> LaunchedManifest[_T]:
         return LaunchedManifest(
             metadata=_LaunchedManifestMetadata(
-                self.run_id, self.exp_name, self.exp_path, self.launcher_name
+                self.run_id,
+                self.exp_name,
+                self.exp_path,
+                self.launcher_name,
             ),
             models=tuple(self._models),
             ensembles=tuple(self._ensembles),
             databases=tuple(self._databases),
         )
```

### Comparing `smartsim-0.6.2/smartsim/_core/entrypoints/__init__.py` & `smartsim-0.7.0/smartsim/_core/entrypoints/__init__.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.6.2/smartsim/_core/entrypoints/colocated.py` & `smartsim-0.7.0/smartsim/_core/entrypoints/colocated.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import os
 import signal
 import socket
 import sys
 import tempfile
 import typing as t
 from pathlib import Path
-from subprocess import PIPE, STDOUT
+from subprocess import STDOUT
 from types import FrameType
 
 import filelock
 import psutil
 from smartredis import Client, ConfigOptions
 from smartredis.error import RedisConnectionError, RedisReplyError
 
@@ -58,19 +58,16 @@
     cleanup()
 
 
 def launch_db_model(client: Client, db_model: t.List[str]) -> str:
     """Parse options to launch model on local cluster
 
     :param client: SmartRedis client connected to local DB
-    :type client: Client
     :param db_model: List of arguments defining the model
-    :type db_model: List[str]
     :return: Name of model
-    :rtype: str
     """
     parser = argparse.ArgumentParser("Set ML model on DB")
     parser.add_argument("--name", type=str)
     parser.add_argument("--file", type=str)
     parser.add_argument("--backend", type=str)
     parser.add_argument("--device", type=str)
     parser.add_argument("--devices_per_node", type=int, default=1)
@@ -125,19 +122,16 @@
     return name
 
 
 def launch_db_script(client: Client, db_script: t.List[str]) -> str:
     """Parse options to launch script on local cluster
 
     :param client: SmartRedis client connected to local DB
-    :type client: Client
     :param db_model: List of arguments defining the script
-    :type db_model: List[str]
     :return: Name of model
-    :rtype: str
     """
     parser = argparse.ArgumentParser("Set script on DB")
     parser.add_argument("--name", type=str)
     parser.add_argument("--func", type=str)
     parser.add_argument("--file", type=str)
     parser.add_argument("--backend", type=str)
     parser.add_argument("--device", type=str)
@@ -173,14 +167,15 @@
     network_interface: str,
     db_cpus: int,
     command: t.List[str],
     db_models: t.List[t.List[str]],
     db_scripts: t.List[t.List[str]],
     db_identifier: str,
 ) -> None:
+    # pylint: disable=too-many-statements
     global DBPID  # pylint: disable=global-statement
 
     lo_address = current_ip("lo")
     ip_addresses = []
     if network_interface:
         try:
             ip_addresses = [
@@ -197,16 +192,25 @@
         cmd = command + [f"--bind {lo_address} {' '.join(ip_addresses)}"]
         # pin source address to avoid random selection by Redis
         cmd += [f"--bind-source-addr {lo_address}"]
 
     # we generally want to catch all exceptions here as
     # if this process dies, the application will most likely fail
     try:
-        process = psutil.Popen(cmd, stdout=PIPE, stderr=STDOUT)
-        DBPID = process.pid
+        hostname = socket.gethostname()
+        filename = (
+            f"colo_orc_{hostname}.log"
+            if os.getenv("SMARTSIM_LOG_LEVEL") == "debug"
+            else os.devnull
+        )
+        with open(filename, "w", encoding="utf-8") as file:
+            process = psutil.Popen(cmd, stdout=file.fileno(), stderr=STDOUT)
+            DBPID = process.pid
+        # printing to stdout shell file for extraction
+        print(f"__PID__{DBPID}__PID__", flush=True)
 
     except Exception as e:
         cleanup()
         logger.error(f"Failed to start database process: {str(e)}")
         raise SSInternalError("Colocated process failed to start") from e
 
     try:
@@ -241,20 +245,16 @@
                 client = Client(options, logger_name="SmartSim")
                 launch_models(client, db_models)
                 launch_db_scripts(client, db_scripts)
             except (RedisConnectionError, RedisReplyError) as ex:
                 raise SSInternalError(
                     "Failed to set model or script, could not connect to database"
                 ) from ex
-            finally:
-                # Make sure we don't keep this around
-                del client
-
-        for line in iter(process.stdout.readline, b""):
-            print(line.decode("utf-8").rstrip(), flush=True)
+            # Make sure we don't keep this around
+            del client
 
     except Exception as e:
         cleanup()
         logger.error(f"Colocated database process failed: {str(e)}")
         raise SSInternalError("Colocated entrypoint raised an error") from e
```

### Comparing `smartsim-0.6.2/smartsim/_core/entrypoints/indirect.py` & `smartsim-0.7.0/smartsim/_core/entrypoints/indirect.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,35 +33,41 @@
 import typing as t
 from types import FrameType
 
 import coloredlogs
 import psutil
 
 import smartsim.log
-from smartsim._core.entrypoints.telemetrymonitor import track_event
-from smartsim._core.utils.helpers import decode_cmd, get_ts
+from smartsim._core.utils.helpers import decode_cmd, get_ts_ms
+from smartsim._core.utils.telemetry.telemetry import write_event
 
 STEP_PID: t.Optional[int] = None
 logger = smartsim.log.get_logger(__name__)
 
 # kill is not catchable
 SIGNALS = [signal.SIGINT, signal.SIGTERM, signal.SIGQUIT, signal.SIGABRT]
 
 
 def main(
     cmd: str,
-    etype: str,
+    entity_type: str,
     cwd: str,
     status_dir: str,
 ) -> int:
-    """The main function of the entrypoint. This function takes an encoded step
-    command and runs it in a subprocess. In the background, this entrypoint
-    will then monitor the subprocess and write out status events such as when
-    the subprocess has started or stopped and write these events to a status
-    directory.
+    """This function receives an encoded step command from a SmartSim Experiment
+    and runs it in a subprocess. The entrypoint integrates with the telemetry
+    monitor by writing status update events. It is useful for wrapping
+    unmanaged tasks - a workload manager can be queried for a managed task
+    to achieve the same result.
+
+    :param cmd: a base64 encoded cmd to execute
+    :param entity_type: `SmartSimEntity` entity class. Valid values
+    include: orchestrator, dbnode, ensemble, model
+    :param cwd: working directory to execute the cmd from
+    :param status_dir: path to the output directory for status updates
     """
     global STEP_PID  # pylint: disable=global-statement
     proxy_pid = os.getpid()
 
     status_path = pathlib.Path(status_dir)
     if not status_path.exists():
         status_path.mkdir(parents=True, exist_ok=True)
@@ -90,57 +96,61 @@
     except Exception as ex:
         start_detail += f" failed to start child process. {ex}"
         start_rc = 1
         logger.error("Failed to create process", exc_info=True)
         cleanup()
         return 1
     finally:
-        track_event(
-            get_ts(),
+        write_event(
+            get_ts_ms(),
             proxy_pid,
             "",  # step_id for unmanaged task is always empty
-            etype,
+            entity_type,
             "start",
             status_path,
-            logger,
             detail=start_detail,
             return_code=start_rc,
         )
 
     logger.info(f"Waiting for child process {STEP_PID} to complete")
-    ret_code = process.wait()
+
+    try:
+        ret_code = process.wait()
+    except Exception:
+        logger.error("Failed to complete process", exc_info=True)
+        ret_code = -1
 
     logger.info(
         f"Indirect proxy {proxy_pid} child process {STEP_PID} complete."
         f" return code: {ret_code}"
     )
     msg = f"Process {STEP_PID} finished with return code: {ret_code}"
-    track_event(
-        get_ts(),
+    write_event(
+        get_ts_ms(),
         proxy_pid,
         "",  # step_id for unmanaged task is always empty
-        etype,
+        entity_type,
         "stop",
         status_path,
-        logger,
         detail=msg,
         return_code=ret_code,
     )
     cleanup()
 
     return ret_code
 
 
 def cleanup() -> None:
     """Perform cleanup required for clean termination"""
-    logger.info("Performing cleanup")
     global STEP_PID  # pylint: disable=global-statement
     if STEP_PID is None:
         return
 
+    logger.info("Performing cleanup")
+
     try:
         # attempt to stop the subprocess performing step-execution
         if psutil.pid_exists(STEP_PID):
             process = psutil.Process(STEP_PID)
             process.terminate()
     except psutil.NoSuchProcess:
         # swallow exception to avoid overwriting outputs from cmd
@@ -224,15 +234,15 @@
 
         # make sure to register the cleanup before the start the process
         # so our signaller will be able to stop the database process.
         register_signal_handlers()
 
         rc = main(
             cmd=parsed_args.command,
-            etype=parsed_args.entity_type,
+            entity_type=parsed_args.entity_type,
             cwd=parsed_args.working_dir,
             status_dir=parsed_args.telemetry_dir,
         )
         sys.exit(rc)
 
     # gracefully exit the processes in the distributed application that
     # we do not want to have start a colocated process. Only one process
```

### Comparing `smartsim-0.6.2/smartsim/_core/entrypoints/redis.py` & `smartsim-0.7.0/smartsim/_core/entrypoints/redis.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 from subprocess import PIPE, STDOUT
 from types import FrameType
 
 import psutil
 
 from smartsim._core.utils.network import current_ip
 from smartsim.entity.dbnode import LaunchedShardData
-from smartsim.error import SSInternalError
 from smartsim.log import get_logger
 
 logger = get_logger(__name__)
 
 """
 Redis/KeyDB entrypoint script
 """
@@ -107,25 +106,27 @@
         args.conf_file,
         *args.rai_module,
         "--port",
         str(args.port),
         *build_cluster_args(shard_data),
         *build_bind_args(src_addr, *bind_addrs),
     ]
+
     print_summary(cmd, args.ifname, shard_data)
 
     try:
         process = psutil.Popen(cmd, stdout=PIPE, stderr=STDOUT)
         DBPID = process.pid
 
         for line in iter(process.stdout.readline, b""):
             print(line.decode("utf-8").rstrip(), flush=True)
-    except Exception as e:
+    except Exception:
         cleanup()
-        raise SSInternalError("Database process starter raised an exception") from e
+        logger.error("Database process starter raised an exception", exc_info=True)
+        return 1
     return 0
 
 
 def cleanup() -> None:
     logger.debug("Cleaning up database instance")
     try:
         # attempt to stop the database process
@@ -175,14 +176,15 @@
         "+ifname", type=str, help="Network Interface name", required=True
     )
     parser.add_argument(
         "+cluster",
         action="store_true",
         help="Specify if this orchestrator shard is part of a cluster",
     )
+
     args_ = parser.parse_args()
 
     # make sure to register the cleanup before the start
     # the process so our signaller will be able to stop
     # the database process.
     for sig in SIGNALS:
         signal.signal(sig, handle_signal)
```

### Comparing `smartsim-0.6.2/smartsim/_core/entrypoints/telemetrymonitor.py` & `smartsim-0.7.0/smartsim/entity/ensemble.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2024 Hewlett Packard Enterprise
+# Copyright (c) 2021-2024, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
@@ -20,671 +20,553 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-import argparse
-import json
-import logging
-import os
-import pathlib
-import signal
-import sys
-import threading
-import time
+import os.path as osp
 import typing as t
-from dataclasses import dataclass, field
-from types import FrameType
+from copy import deepcopy
+from os import getcwd
 
-from watchdog.events import (
-    FileCreatedEvent,
-    FileModifiedEvent,
-    LoggingEventHandler,
-    PatternMatchingEventHandler,
-)
-from watchdog.observers import Observer
-from watchdog.observers.api import BaseObserver
+from tabulate import tabulate
 
-from smartsim._core.config import CONFIG
-from smartsim._core.control.job import JobEntity, _JobKey
-from smartsim._core.control.jobmanager import JobManager
-from smartsim._core.launcher.launcher import Launcher
-from smartsim._core.launcher.local.local import LocalLauncher
-from smartsim._core.launcher.lsf.lsfLauncher import LSFLauncher
-from smartsim._core.launcher.pbs.pbsLauncher import PBSLauncher
-from smartsim._core.launcher.slurm.slurmLauncher import SlurmLauncher
-from smartsim._core.launcher.stepInfo import StepInfo
-from smartsim._core.utils.helpers import get_ts
-from smartsim._core.utils.serialize import MANIFEST_FILENAME
-from smartsim.error.errors import SmartSimError
-from smartsim.status import STATUS_COMPLETED, TERMINAL_STATUSES
-
-"""Telemetry Monitor entrypoint"""
-
-# kill is not catchable
-SIGNALS = [signal.SIGINT, signal.SIGQUIT, signal.SIGTERM, signal.SIGABRT]
-_EventClass = t.Literal["start", "stop", "timestep"]
-_MAX_MANIFEST_LOAD_ATTEMPTS: t.Final[int] = 6
-
-
-@dataclass
-class Run:
-    """Model containing entities of an individual start call for an experiment"""
-
-    timestamp: int
-    models: t.List[JobEntity]
-    orchestrators: t.List[JobEntity]
-    ensembles: t.List[JobEntity]
-
-    def flatten(
-        self, filter_fn: t.Optional[t.Callable[[JobEntity], bool]] = None
-    ) -> t.List[JobEntity]:
-        """Flatten runs into a list of SmartSimEntity run events"""
-        entities = self.models + self.orchestrators + self.ensembles
-        if filter_fn:
-            entities = [entity for entity in entities if filter_fn(entity)]
-        return entities
-
-
-@dataclass
-class RuntimeManifest:
-    """The runtime manifest holds meta information about the experiment entities created
-    at runtime to satisfy the experiment requirements.
+from .._core._install.builder import Device
+from ..error import (
+    EntityExistsError,
+    SmartSimError,
+    SSUnsupportedError,
+    UserStrategyError,
+)
+from ..log import get_logger
+from ..settings.base import BatchSettings, RunSettings
+from .dbobject import DBModel, DBScript
+from .entity import SmartSimEntity
+from .entityList import EntityList
+from .model import Model
+from .strategies import create_all_permutations, random_permutations, step_values
+
+logger = get_logger(__name__)
+
+StrategyFunction = t.Callable[
+    [t.List[str], t.List[t.List[str]], int], t.List[t.Dict[str, str]]
+]
+
+
+class Ensemble(EntityList[Model]):
+    """``Ensemble`` is a group of ``Model`` instances that can
+    be treated as a reference to a single instance.
     """
 
-    name: str
-    path: pathlib.Path
-    launcher: str
-    runs: t.List[Run] = field(default_factory=list)
-
-
-def _hydrate_persistable(
-    persistable_entity: t.Dict[str, t.Any],
-    entity_type: str,
-    exp_dir: str,
-) -> JobEntity:
-    """Populate JobEntity instance with supplied metdata and instance details"""
-    entity = JobEntity()
-
-    metadata = persistable_entity["telemetry_metadata"]
-    status_dir = pathlib.Path(metadata.get("status_dir"))
-
-    entity.type = entity_type
-    entity.name = persistable_entity["name"]
-    entity.step_id = str(metadata.get("step_id") or "")
-    entity.task_id = str(metadata.get("task_id") or "")
-    entity.timestamp = int(persistable_entity.get("timestamp", "0"))
-    entity.path = str(exp_dir)
-    entity.status_dir = str(status_dir)
-
-    return entity
-
-
-def hydrate_persistable(
-    entity_type: str,
-    persistable_entity: t.Dict[str, t.Any],
-    exp_dir: pathlib.Path,
-) -> t.List[JobEntity]:
-    """Map entity data persisted in a manifest file to an object"""
-    entities = []
-
-    # an entity w/parent key creates persistables for entities it contains
-    parent_keys = {"shards", "models"}
-    parent_keys = parent_keys.intersection(persistable_entity.keys())
-    if parent_keys:
-        container = "shards" if "shards" in parent_keys else "models"
-        child_type = "orchestrator" if container == "shards" else "model"
-        for child_entity in persistable_entity[container]:
-            entity = _hydrate_persistable(child_entity, child_type, str(exp_dir))
-            entities.append(entity)
-
-        return entities
-
-    entity = _hydrate_persistable(persistable_entity, entity_type, str(exp_dir))
-    entities.append(entity)
-    return entities
-
-
-def hydrate_persistables(
-    entity_type: str,
-    run: t.Dict[str, t.Any],
-    exp_dir: pathlib.Path,
-) -> t.Dict[str, t.List[JobEntity]]:
-    """Map a collection of entity data persisted in a manifest file to an object"""
-    persisted: t.Dict[str, t.List[JobEntity]] = {
-        "model": [],
-        "orchestrator": [],
-    }
-    for item in run[entity_type]:
-        entities = hydrate_persistable(entity_type, item, exp_dir)
-        for new_entity in entities:
-            persisted[new_entity.type].append(new_entity)
-
-    return persisted
-
-
-def hydrate_runs(
-    persisted_runs: t.List[t.Dict[str, t.Any]], exp_dir: pathlib.Path
-) -> t.List[Run]:
-    """Map run data persisted in a manifest file to an object"""
-    the_runs: t.List[Run] = []
-    for run_instance in persisted_runs:
-        run_entities: t.Dict[str, t.List[JobEntity]] = {
-            "model": [],
-            "orchestrator": [],
-            "ensemble": [],
-        }
-
-        for key in run_entities:
-            _entities = hydrate_persistables(key, run_instance, exp_dir)
-            for entity_type, new_entities in _entities.items():
-                if new_entities:
-                    run_entities[entity_type].extend(new_entities)
-
-        run = Run(
-            run_instance["timestamp"],
-            run_entities["model"],
-            run_entities["orchestrator"],
-            run_entities["ensemble"],
-        )
-        the_runs.append(run)
+    def __init__(
+        self,
+        name: str,
+        params: t.Dict[str, t.Any],
+        path: t.Optional[str] = getcwd(),
+        params_as_args: t.Optional[t.List[str]] = None,
+        batch_settings: t.Optional[BatchSettings] = None,
+        run_settings: t.Optional[RunSettings] = None,
+        perm_strat: str = "all_perm",
+        **kwargs: t.Any,
+    ) -> None:
+        """Initialize an Ensemble of Model instances.
 
-    return the_runs
+        The kwargs argument can be used to pass custom input
+        parameters to the permutation strategy.
 
+        :param name: name of the ensemble
+        :param params: parameters to expand into ``Model`` members
+        :param params_as_args: list of params that should be used as command
+            line arguments to the ``Model`` member executables and not written
+            to generator files
+        :param batch_settings: describes settings for ``Ensemble`` as batch workload
+        :param run_settings: describes how each ``Model`` should be executed
+        :param replicas: number of ``Model`` replicas to create - a keyword
+            argument of kwargs
+        :param perm_strategy: strategy for expanding ``params`` into
+                             ``Model`` instances from params argument
+                             options are "all_perm", "step", "random"
+                             or a callable function.
+        :return: ``Ensemble`` instance
+        """
+        self.params = params or {}
+        self.params_as_args = params_as_args or []
+        self._key_prefixing_enabled = True
+        self.batch_settings = batch_settings
+        self.run_settings = run_settings
+        self.replicas: str
+
+        super().__init__(name, str(path), perm_strat=perm_strat, **kwargs)
+
+    @property
+    def models(self) -> t.Collection[Model]:
+        """An alias for a shallow copy of the ``entities`` attribute"""
+        return list(self.entities)
+
+    def _initialize_entities(self, **kwargs: t.Any) -> None:
+        """Initialize all the models within the ensemble based
+        on the parameters passed to the ensemble and the permutation
+        strategy given at init.
 
-def load_manifest(file_path: str) -> t.Optional[RuntimeManifest]:
-    """Load a persisted manifest and return the content"""
-    manifest_dict: t.Optional[t.Dict[str, t.Any]] = None
-    try_count = 1
-
-    while manifest_dict is None and try_count < _MAX_MANIFEST_LOAD_ATTEMPTS:
-        source = pathlib.Path(file_path)
-        source = source.resolve()
-
-        try:
-            if text := source.read_text(encoding="utf-8").strip():
-                manifest_dict = json.loads(text)
-        except json.JSONDecodeError as ex:
-            print(f"Error loading manifest: {ex}")
-            # hack/fix: handle issues reading file before it is fully written
-            time.sleep(0.5 * try_count)
-        finally:
-            try_count += 1
-
-    if not manifest_dict:
-        return None
-
-    exp = manifest_dict.get("experiment", None)
-    if not exp:
-        raise ValueError("Manifest missing required experiment")
-
-    runs = manifest_dict.get("runs", None)
-    if runs is None:
-        raise ValueError("Manifest missing required runs")
-
-    exp_dir = pathlib.Path(exp["path"])
-    runs = hydrate_runs(runs, exp_dir)
-
-    manifest = RuntimeManifest(
-        name=exp["name"],
-        path=exp_dir,
-        launcher=exp["launcher"],
-        runs=runs,
-    )
-    return manifest
-
-
-def track_event(
-    timestamp: int,
-    task_id: t.Union[int, str],
-    step_id: str,
-    etype: str,
-    action: _EventClass,
-    status_dir: pathlib.Path,
-    logger: logging.Logger,
-    detail: str = "",
-    return_code: t.Optional[int] = None,
-) -> None:
-    """Persist a tracking event for an entity"""
-    tgt_path = status_dir / f"{action}.json"
-    tgt_path.parent.mkdir(parents=True, exist_ok=True)
-
-    try:
-        task_id = int(task_id)
-    except ValueError:
-        pass
-
-    entity_dict = {
-        "timestamp": timestamp,
-        "job_id": task_id,
-        "step_id": step_id,
-        "type": etype,
-        "action": action,
-    }
-
-    if detail is not None:
-        entity_dict["detail"] = detail
-
-    if return_code is not None:
-        entity_dict["return_code"] = return_code
-
-    try:
-        if not tgt_path.exists():
-            # Don't overwrite existing tracking files
-            bytes_written = tgt_path.write_text(json.dumps(entity_dict, indent=2))
-            if bytes_written < 1:
-                logger.warning("event tracking failed to write tracking file.")
-    except Exception:
-        logger.error("Unable to write tracking file.", exc_info=True)
-
-
-def faux_return_code(step_info: StepInfo) -> t.Optional[int]:
-    """Create a faux return code for a task run by the WLM. Must not be
-    called with non-terminal statuses or results may be confusing
-    """
-    if step_info.status not in TERMINAL_STATUSES:
-        return None
+        :raises UserStrategyError: if user generation strategy fails
+        """
+        strategy = self._set_strategy(kwargs.pop("perm_strat"))
+        replicas = kwargs.pop("replicas", None)
+        self.replicas = replicas
+
+        # if a ensemble has parameters and run settings, create
+        # the ensemble and assign run_settings to each member
+        if self.params:
+            if self.run_settings:
+                param_names, params = self._read_model_parameters()
+
+                # Compute all combinations of model parameters and arguments
+                n_models = kwargs.get("n_models", 0)
+                all_model_params = strategy(param_names, params, n_models)
+                if not isinstance(all_model_params, list):
+                    raise UserStrategyError(strategy)
+
+                for i, param_set in enumerate(all_model_params):
+                    if not isinstance(param_set, dict):
+                        raise UserStrategyError(strategy)
+                    run_settings = deepcopy(self.run_settings)
+                    model_name = "_".join((self.name, str(i)))
+                    model = Model(
+                        name=model_name,
+                        params=param_set,
+                        path=osp.join(self.path, model_name),
+                        run_settings=run_settings,
+                        params_as_args=self.params_as_args,
+                    )
+                    model.enable_key_prefixing()
+                    model.params_to_args()
+                    logger.debug(
+                        f"Created ensemble member: {model_name} in {self.name}"
+                    )
+                    self.add_model(model)
+            # cannot generate models without run settings
+            else:
+                raise SmartSimError(
+                    "Ensembles without 'params' or 'replicas' argument to "
+                    "expand into members cannot be given run settings"
+                )
+        else:
+            if self.run_settings:
+                if replicas:
+                    for i in range(replicas):
+                        model_name = "_".join((self.name, str(i)))
+                        model = Model(
+                            name=model_name,
+                            params={},
+                            path=osp.join(self.path, model_name),
+                            run_settings=deepcopy(self.run_settings),
+                        )
+                        model.enable_key_prefixing()
+                        logger.debug(
+                            f"Created ensemble member: {model_name} in {self.name}"
+                        )
+                        self.add_model(model)
+                else:
+                    raise SmartSimError(
+                        "Ensembles without 'params' or 'replicas' argument to "
+                        "expand into members cannot be given run settings"
+                    )
+            # if no params, no run settings and no batch settings, error because we
+            # don't know how to run the ensemble
+            elif not self.batch_settings:
+                raise SmartSimError(
+                    "Ensemble must be provided batch settings or run settings"
+                )
+            else:
+                logger.info("Empty ensemble created for batch launch")
 
-    if step_info.status == STATUS_COMPLETED:
-        return os.EX_OK
+    def add_model(self, model: Model) -> None:
+        """Add a model to this ensemble
 
-    return 1
+        :param model: model instance to be added
+        :raises TypeError: if model is not an instance of ``Model``
+        :raises EntityExistsError: if model already exists in this ensemble
+        """
+        if not isinstance(model, Model):
+            raise TypeError(
+                f"Argument to add_model was of type {type(model)}, not Model"
+            )
+        # "in" operator uses model name for __eq__
+        if model in self.entities:
+            raise EntityExistsError(
+                f"Model {model.name} already exists in ensemble {self.name}"
+            )
+
+        if self._db_models:
+            self._extend_entity_db_models(model, self._db_models)
+        if self._db_scripts:
+            self._extend_entity_db_scripts(model, self._db_scripts)
+
+        self.entities.append(model)
+
+    def register_incoming_entity(self, incoming_entity: SmartSimEntity) -> None:
+        """Register future communication between entities.
+
+        Registers the named data sources that this entity
+        has access to by storing the key_prefix associated
+        with that entity
 
+        Only python clients can have multiple incoming connections
 
-class ManifestEventHandler(PatternMatchingEventHandler):
-    """The ManifestEventHandler monitors an experiment for changes and updates
-    a telemetry datastore as needed.
+        :param incoming_entity: The entity that data will be received from
+        """
+        for model in self.models:
+            model.register_incoming_entity(incoming_entity)
 
-    It contains event handlers that are triggered by changes to a runtime experiment
-    manifest. The runtime manifest differs from a standard manifest. A runtime manifest
-    may contain multiple experiment executions in a `runs` collection.
+    def enable_key_prefixing(self) -> None:
+        """If called, each model within this ensemble will prefix its key with its
+        own model name.
+        """
+        for model in self.models:
+            model.enable_key_prefixing()
 
-    It also contains a long-polling loop that checks experiment entities for updates
-    at each timestep.
-    """
+    def query_key_prefixing(self) -> bool:
+        """Inquire as to whether each model within the ensemble will prefix their keys
 
-    def __init__(
+        :returns: True if all models have key prefixing enabled, False otherwise
+        """
+        return all(model.query_key_prefixing() for model in self.models)
+
+    def attach_generator_files(
         self,
-        pattern: str,
-        logger: logging.Logger,
-        ignore_patterns: t.Any = None,
-        ignore_directories: bool = True,
-        case_sensitive: bool = False,
+        to_copy: t.Optional[t.List[str]] = None,
+        to_symlink: t.Optional[t.List[str]] = None,
+        to_configure: t.Optional[t.List[str]] = None,
     ) -> None:
-        super().__init__(
-            [pattern], ignore_patterns, ignore_directories, case_sensitive
-        )  # type: ignore
-        self._logger = logger
-        self._tracked_runs: t.Dict[int, Run] = {}
-        self._tracked_jobs: t.Dict[_JobKey, JobEntity] = {}
-        self._completed_jobs: t.Dict[_JobKey, JobEntity] = {}
-        self._launcher: t.Optional[Launcher] = None
-        self.job_manager: JobManager = JobManager(threading.RLock())
-        self._launcher_map: t.Dict[str, t.Type[Launcher]] = {
-            "slurm": SlurmLauncher,
-            "pbs": PBSLauncher,
-            "lsf": LSFLauncher,
-            "local": LocalLauncher,
-        }
-
-    def init_launcher(self, launcher: str) -> Launcher:
-        """Initialize the controller with a specific type of launcher.
-        SmartSim currently supports slurm, pbs(pro), lsf,
-        and local launching
-
-        :param launcher: which launcher to initialize
-        :type launcher: str
-        :raises SSUnsupportedError: if a string is passed that is not
-                                    a supported launcher
-        :raises TypeError: if no launcher argument is provided.
-        """
-        if not launcher:
-            raise TypeError("Must provide a 'launcher' argument")
-
-        if launcher_type := self._launcher_map.get(launcher.lower(), None):
-            return launcher_type()
-
-        raise ValueError("Launcher type not supported: " + launcher)
-
-    def set_launcher(self, launcher_type: str) -> None:
-        """Set the launcher for the experiment"""
-        self._launcher = self.init_launcher(launcher_type)
-        self.job_manager.set_launcher(self._launcher)
-        self.job_manager.start()
-
-    def process_manifest(self, manifest_path: str) -> None:
-        """Read the runtime manifest for the experiment and track new entities
-
-        :param manifest_path: The full path to the manifest file
-        :type manifest_path: str
-        """
-        try:
-            manifest = load_manifest(manifest_path)
-            if not manifest:
-                return
-        except json.JSONDecodeError:
-            self._logger.error(f"Malformed manifest encountered: {manifest_path}")
-            return
-        except ValueError:
-            self._logger.error("Manifest content error", exc_info=True)
-            return
-
-        if self._launcher is None:
-            self.set_launcher(manifest.launcher)
-
-        if not self._launcher:
-            raise SmartSimError(f"Unable to set launcher from {manifest_path}")
-
-        runs = [run for run in manifest.runs if run.timestamp not in self._tracked_runs]
-
-        exp_dir = pathlib.Path(manifest_path).parent.parent.parent
-
-        for run in runs:
-            for entity in run.flatten(
-                filter_fn=lambda e: e.key not in self._tracked_jobs and e.is_managed
-            ):
-                entity.path = str(exp_dir)
-
-                self._tracked_jobs[entity.key] = entity
-                track_event(
-                    run.timestamp,
-                    entity.task_id,
-                    entity.step_id,
-                    entity.type,
-                    "start",
-                    pathlib.Path(entity.status_dir),
-                    self._logger,
-                )
+        """Attach files to each model within the ensemble for generation
 
-                if entity.is_managed:
-                    self.job_manager.add_job(
-                        entity.name,
-                        entity.task_id,
-                        entity,
-                        False,
-                    )
-                    self._launcher.step_mapping.add(
-                        entity.name, entity.step_id, entity.task_id, True
-                    )
-            self._tracked_runs[run.timestamp] = run
+        Attach files needed for the entity that, upon generation,
+        will be located in the path of the entity.
 
-    def on_modified(self, event: FileModifiedEvent) -> None:
-        """Event handler for when a file or directory is modified.
+        During generation, files "to_copy" are copied into
+        the path of the entity, and files "to_symlink" are
+        symlinked into the path of the entity.
+
+        Files "to_configure" are text based model input files where
+        parameters for the model are set. Note that only models
+        support the "to_configure" field. These files must have
+        fields tagged that correspond to the values the user
+        would like to change. The tag is settable but defaults
+        to a semicolon e.g. THERMO = ;10;
+
+        :param to_copy: files to copy
+        :param to_symlink: files to symlink
+        :param to_configure: input files with tagged parameters
+        """
+        for model in self.models:
+            model.attach_generator_files(
+                to_copy=to_copy, to_symlink=to_symlink, to_configure=to_configure
+            )
+
+    @property
+    def attached_files_table(self) -> str:
+        """Return a plain-text table with information about files
+        attached to models belonging to this ensemble.
 
-        :param event: Event representing file/directory modification.
-        :type event: FileModifiedEvent
+        :returns: A table of all files attached to all models
         """
-        super().on_modified(event)  # type: ignore
-        self._logger.info(f"processing manifest modified @ {event.src_path}")
-        self.process_manifest(event.src_path)
+        if not self.models:
+            return "The ensemble is empty, no files to show."
 
-    def on_created(self, event: FileCreatedEvent) -> None:
-        """Event handler for when a file or directory is created.
+        table = tabulate(
+            [[model.name, model.attached_files_table] for model in self.models],
+            headers=["Model name", "Files"],
+            tablefmt="grid",
+        )
 
-        :param event: Event representing file/directory creation.
-        :type event: FileCreatedEvent
+        return table
+
+    def print_attached_files(self) -> None:
+        """Print table of attached files to std out"""
+        print(self.attached_files_table)
+
+    @staticmethod
+    def _set_strategy(strategy: str) -> StrategyFunction:
+        """Set the permutation strategy for generating models within
+        the ensemble
+
+        :param strategy: name of the strategy or callable function
+        :raises SSUnsupportedError: if str name is not supported
+        :return: strategy function
         """
-        super().on_created(event)  # type: ignore
-        self._logger.info(f"processing manifest created @ {event.src_path}")
-        self.process_manifest(event.src_path)
+        if strategy == "all_perm":
+            return create_all_permutations
+        if strategy == "step":
+            return step_values
+        if strategy == "random":
+            return random_permutations
+        if callable(strategy):
+            return strategy
+        raise SSUnsupportedError(
+            f"Permutation strategy given is not supported: {strategy}"
+        )
+
+    def _read_model_parameters(self) -> t.Tuple[t.List[str], t.List[t.List[str]]]:
+        """Take in the parameters given to the ensemble and prepare to
+        create models for the ensemble
 
-    def _to_completed(
+        :raises TypeError: if params are of the wrong type
+        :return: param names and values for permutation strategy
+        """
+
+        if not isinstance(self.params, dict):
+            raise TypeError(
+                "Ensemble initialization argument 'params' must be of type dict"
+            )
+
+        param_names: t.List[str] = []
+        parameters: t.List[t.List[str]] = []
+        for name, val in self.params.items():
+            param_names.append(name)
+
+            if isinstance(val, list):
+                val = [str(v) for v in val]
+                parameters.append(val)
+            elif isinstance(val, (int, str)):
+                parameters.append([str(val)])
+            else:
+                raise TypeError(
+                    "Incorrect type for ensemble parameters\n"
+                    + "Must be list, int, or string."
+                )
+        return param_names, parameters
+
+    def add_ml_model(
         self,
-        timestamp: int,
-        entity: JobEntity,
-        step_info: StepInfo,
+        name: str,
+        backend: str,
+        model: t.Optional[bytes] = None,
+        model_path: t.Optional[str] = None,
+        device: str = Device.CPU.value.upper(),
+        devices_per_node: int = 1,
+        first_device: int = 0,
+        batch_size: int = 0,
+        min_batch_size: int = 0,
+        min_batch_timeout: int = 0,
+        tag: str = "",
+        inputs: t.Optional[t.List[str]] = None,
+        outputs: t.Optional[t.List[str]] = None,
     ) -> None:
-        """Move a monitored entity from the active to completed collection to
-        stop monitoring for updates during timesteps.
+        """A TF, TF-lite, PT, or ONNX model to load into the DB at runtime
 
-        :param timestamp: the current timestamp for event logging
-        :type timestamp: int
-        :param entity: the running SmartSim Job
-        :type entity: JobEntity
-        :param experiment_dir: the experiement directory to monitor for changes
-        :type experiment_dir: pathlib.Path
-        :param entity: the StepInfo received when requesting a Job status update
-        :type entity: StepInfo
-        """
-        inactive_entity = self._tracked_jobs.pop(entity.key)
-        if entity.key not in self._completed_jobs:
-            self._completed_jobs[entity.key] = inactive_entity
-
-        job = self.job_manager[entity.name]
-        self.job_manager.move_to_completed(job)
-
-        status_clause = f"status: {step_info.status}"
-        error_clause = f", error: {step_info.error}" if step_info.error else ""
-        detail = f"{status_clause}{error_clause}"
-
-        if hasattr(job.entity, "status_dir"):
-            write_path = pathlib.Path(job.entity.status_dir)
-
-        track_event(
-            timestamp,
-            entity.task_id,
-            entity.step_id,
-            entity.type,
-            "stop",
-            write_path,
-            self._logger,
-            detail=detail,
-            return_code=faux_return_code(step_info),
+        Each ML Model added will be loaded into an
+        orchestrator (converged or not) prior to the execution
+        of every entity belonging to this ensemble
+
+        One of either model (in memory representation) or model_path (file)
+        must be provided
+
+        :param name: key to store model under
+        :param model: model in memory
+        :param model_path: serialized model
+        :param backend: name of the backend (TORCH, TF, TFLITE, ONNX)
+        :param device: name of device for execution
+        :param devices_per_node: number of GPUs per node in multiGPU nodes
+        :param first_device: first device in multi-GPU nodes to use for execution,
+                             defaults to 0; ignored if devices_per_node is 1
+        :param batch_size: batch size for execution
+        :param min_batch_size: minimum batch size for model execution
+        :param min_batch_timeout: time to wait for minimum batch size
+        :param tag: additional tag for model information
+        :param inputs: model inputs (TF only)
+        :param outputs: model outupts (TF only)
+        """
+        db_model = DBModel(
+            name=name,
+            backend=backend,
+            model=model,
+            model_file=model_path,
+            device=device,
+            devices_per_node=devices_per_node,
+            first_device=first_device,
+            batch_size=batch_size,
+            min_batch_size=min_batch_size,
+            min_batch_timeout=min_batch_timeout,
+            tag=tag,
+            inputs=inputs,
+            outputs=outputs,
         )
+        dupe = next(
+            (
+                db_model.name
+                for ensemble_ml_model in self._db_models
+                if ensemble_ml_model.name == db_model.name
+            ),
+            None,
+        )
+        if dupe:
+            raise SSUnsupportedError(
+                f'An ML Model with name "{db_model.name}" already exists'
+            )
+        self._db_models.append(db_model)
+        for entity in self.models:
+            self._extend_entity_db_models(entity, [db_model])
 
-    def on_timestep(self, timestamp: int) -> None:
-        """Called at polling frequency to request status updates on
-        monitored entities
-
-        :param timestamp: the current timestamp for event logging
-        :type timestamp: int
-        :param experiment_dir: the experiement directory to monitor for changes
-        :type experiment_dir: pathlib.Path
-        """
-        entity_map = self._tracked_jobs
-
-        if not self._launcher:
-            return
-
-        # consider not using name to avoid collisions
-        names = {entity.name: entity for entity in entity_map.values()}
-
-        if names:
-            step_updates = self._launcher.get_step_update(list(names.keys()))
-
-            for step_name, step_info in step_updates:
-                if step_info and step_info.status in TERMINAL_STATUSES:
-                    completed_entity = names[step_name]
-                    self._to_completed(timestamp, completed_entity, step_info)
-
-
-def can_shutdown(action_handler: ManifestEventHandler, logger: logging.Logger) -> bool:
-    jobs = action_handler.job_manager.jobs
-    db_jobs = action_handler.job_manager.db_jobs
-
-    has_jobs = bool(jobs)
-    has_dbs = bool(db_jobs)
-    has_running_jobs = has_jobs or has_dbs
-
-    if has_jobs:
-        logger.debug(f"telemetry monitor is monitoring {len(jobs)} jobs")
-    if has_dbs:
-        logger.debug(f"telemetry monitor is monitoring {len(db_jobs)} dbs")
-
-    return not has_running_jobs
-
-
-def event_loop(
-    observer: BaseObserver,
-    action_handler: ManifestEventHandler,
-    frequency: t.Union[int, float],
-    logger: logging.Logger,
-    cooldown_duration: int,
-) -> None:
-    """Executes all attached timestep handlers every <frequency> seconds
-
-    :param observer: (optional) a preconfigured watchdog Observer to inject
-    :type observer: t.Optional[BaseObserver]
-    :param action_handler: The manifest event processor instance
-    :type action_handler: ManifestEventHandler
-    :param frequency: frequency (in seconds) of update loop
-    :type frequency: t.Union[int, float]
-    :param logger: a preconfigured Logger instance
-    :type logger: logging.Logger
-    :param cooldown_duration: number of seconds the telemetry monitor should
-                              poll for new jobs before attempting to shutdown
-    :type cooldown_duration: int
-    """
-    elapsed: int = 0
-    last_ts: int = get_ts()
-
-    while observer.is_alive():
-        timestamp = get_ts()
-        logger.debug(f"Telemetry timestep: {timestamp}")
-        action_handler.on_timestep(timestamp)
-
-        elapsed += timestamp - last_ts
-        last_ts = timestamp
-
-        if can_shutdown(action_handler, logger):
-            if elapsed >= cooldown_duration:
-                logger.info("beginning telemetry manager shutdown")
-                observer.stop()  # type: ignore
-        else:
-            # reset cooldown any time there are still jobs running
-            elapsed = 0
+    def add_script(
+        self,
+        name: str,
+        script: t.Optional[str] = None,
+        script_path: t.Optional[str] = None,
+        device: str = Device.CPU.value.upper(),
+        devices_per_node: int = 1,
+        first_device: int = 0,
+    ) -> None:
+        """TorchScript to launch with every entity belonging to this ensemble
 
-        time.sleep(frequency)
+        Each script added to the model will be loaded into an
+        orchestrator (converged or not) prior to the execution
+        of every entity belonging to this ensemble
+
+        Device selection is either "GPU" or "CPU". If many devices are
+        present, a number can be passed for specification e.g. "GPU:1".
+
+        Setting ``devices_per_node=N``, with N greater than one will result
+        in the model being stored in the first N devices of type ``device``.
+
+        One of either script (in memory string representation) or script_path (file)
+        must be provided
+
+        :param name: key to store script under
+        :param script: TorchScript code
+        :param script_path: path to TorchScript code
+        :param device: device for script execution
+        :param devices_per_node: number of devices on each host
+        :param first_device: first device to use on each host
+        """
+        db_script = DBScript(
+            name=name,
+            script=script,
+            script_path=script_path,
+            device=device,
+            devices_per_node=devices_per_node,
+            first_device=first_device,
+        )
+        dupe = next(
+            (
+                db_script.name
+                for ensemble_script in self._db_scripts
+                if ensemble_script.name == db_script.name
+            ),
+            None,
+        )
+        if dupe:
+            raise SSUnsupportedError(
+                f'A Script with name "{db_script.name}" already exists'
+            )
+        self._db_scripts.append(db_script)
+        for entity in self.models:
+            self._extend_entity_db_scripts(entity, [db_script])
 
+    def add_function(
+        self,
+        name: str,
+        function: t.Optional[str] = None,
+        device: str = Device.CPU.value.upper(),
+        devices_per_node: int = 1,
+        first_device: int = 0,
+    ) -> None:
+        """TorchScript function to launch with every entity belonging to this ensemble
 
-def main(
-    frequency: t.Union[int, float],
-    experiment_dir: pathlib.Path,
-    logger: logging.Logger,
-    observer: t.Optional[BaseObserver] = None,
-    cooldown_duration: t.Optional[int] = 0,
-) -> int:
-    """Setup the monitoring entities and start the timer-based loop that
-    will poll for telemetry data
-
-    :param frequency: frequency (in seconds) of update loop
-    :type frequency: t.Union[int, float]
-    :param experiment_dir: the experiement directory to monitor for changes
-    :type experiment_dir: pathlib.Path
-    :param logger: a preconfigured Logger instance
-    :type logger: logging.Logger
-    :param observer: (optional) a preconfigured Observer to inject
-    :type observer: t.Optional[BaseObserver]
-    :param cooldown_duration: number of seconds the telemetry monitor should
-                              poll for new jobs before attempting to shutdown
-    :type cooldown_duration: int
-    """
-    manifest_relpath = pathlib.Path(CONFIG.telemetry_subdir) / MANIFEST_FILENAME
-    manifest_path = experiment_dir / manifest_relpath
-    monitor_pattern = str(manifest_relpath)
-
-    logger.info(
-        f"Executing telemetry monitor with frequency: {frequency}s"
-        f", on target directory: {experiment_dir}"
-        f" matching pattern: {monitor_pattern}"
-    )
-
-    cooldown_duration = cooldown_duration or CONFIG.telemetry_cooldown
-    log_handler = LoggingEventHandler(logger)  # type: ignore
-    action_handler = ManifestEventHandler(monitor_pattern, logger)
-
-    if observer is None:
-        observer = Observer()
-
-    try:
-        if manifest_path.exists():
-            # a manifest may not exist depending on startup timing
-            action_handler.process_manifest(str(manifest_path))
-
-        observer.schedule(log_handler, experiment_dir, recursive=True)  # type:ignore
-        observer.schedule(action_handler, experiment_dir, recursive=True)  # type:ignore
-        observer.start()  # type: ignore
-
-        event_loop(observer, action_handler, frequency, logger, cooldown_duration)
-        return os.EX_OK
-    except Exception as ex:
-        logger.error(ex)
-    finally:
-        if observer.is_alive():
-            observer.stop()  # type: ignore
-            observer.join()
-
-    return os.EX_SOFTWARE
-
-
-def handle_signal(signo: int, _frame: t.Optional[FrameType]) -> None:
-    """Helper function to ensure clean process termination"""
-    if not signo:
-        logger = logging.getLogger()
-        logger.warning("Received signal with no signo")
-
-
-def register_signal_handlers() -> None:
-    """Register a signal handling function for all termination events"""
-    for sig in SIGNALS:
-        signal.signal(sig, handle_signal)
-
-
-def get_parser() -> argparse.ArgumentParser:
-    """Instantiate a parser to process command line arguments"""
-    arg_parser = argparse.ArgumentParser(description="SmartSim Telemetry Monitor")
-    arg_parser.add_argument(
-        "-frequency",
-        type=int,
-        help="Frequency of telemetry updates (in seconds))",
-        required=True,
-    )
-    arg_parser.add_argument(
-        "-exp_dir",
-        type=str,
-        help="Experiment root directory",
-        required=True,
-    )
-    arg_parser.add_argument(
-        "-cooldown",
-        type=int,
-        help="Default lifetime of telemetry monitor (in seconds) before auto-shutdown",
-        default=CONFIG.telemetry_cooldown,
-    )
-    return arg_parser
-
-
-if __name__ == "__main__":
-    os.environ["PYTHONUNBUFFERED"] = "1"
-
-    parser = get_parser()
-    args = parser.parse_args()
-
-    log = logging.getLogger(f"{__name__}.TelemetryMonitor")
-    log.setLevel(logging.DEBUG)
-    log.propagate = False
-
-    log_path = os.path.join(
-        args.exp_dir, CONFIG.telemetry_subdir, "telemetrymonitor.log"
-    )
-    fh = logging.FileHandler(log_path, "a")
-    log.addHandler(fh)
-
-    # Must register cleanup before the main loop is running
-    register_signal_handlers()
-
-    try:
-        main(
-            int(args.frequency),
-            pathlib.Path(args.exp_dir),
-            log,
-            cooldown_duration=args.cooldown,
+        Each script function to the model will be loaded into a
+        non-converged orchestrator prior to the execution
+        of every entity belonging to this ensemble.
+
+        For converged orchestrators, the :meth:`add_script` method should be used.
+
+        Device selection is either "GPU" or "CPU". If many devices are
+        present, a number can be passed for specification e.g. "GPU:1".
+
+        Setting ``devices_per_node=N``, with N greater than one will result
+        in the script being stored in the first N devices of type ``device``;
+        alternatively, setting ``first_device=M`` will result in the script
+        being stored on nodes M through M + N - 1.
+
+        :param name: key to store function under
+        :param function: TorchScript code
+        :param device: device for script execution
+        :param devices_per_node: number of devices on each host
+        :param first_device: first device to use on each host
+        """
+        db_script = DBScript(
+            name=name,
+            script=function,
+            device=device,
+            devices_per_node=devices_per_node,
+            first_device=first_device,
         )
-        sys.exit(0)
-    except Exception:
-        log.exception(
-            "Shutting down telemetry monitor due to unexpected error", exc_info=True
+        dupe = next(
+            (
+                db_script.name
+                for ensemble_script in self._db_scripts
+                if ensemble_script.name == db_script.name
+            ),
+            None,
         )
+        if dupe:
+            raise SSUnsupportedError(
+                f'A Script with name "{db_script.name}" already exists'
+            )
+        self._db_scripts.append(db_script)
+        for entity in self.models:
+            self._extend_entity_db_scripts(entity, [db_script])
+
+    @staticmethod
+    def _extend_entity_db_models(model: Model, db_models: t.List[DBModel]) -> None:
+        """
+        Ensures that the Machine Learning model names being added to the Ensemble
+        are unique.
+
+        This static method checks if the provided ML model names already exist in
+        the Ensemble. An SSUnsupportedError is raised if any duplicate names are
+        found. Otherwise, it appends the given list of DBModels to the Ensemble.
+
+        :param model: SmartSim Model object.
+        :param db_models: List of DBModels to append to the Ensemble.
+        """
+        for add_ml_model in db_models:
+            dupe = next(
+                (
+                    db_model.name
+                    for db_model in model.db_models
+                    if db_model.name == add_ml_model.name
+                ),
+                None,
+            )
+            if dupe:
+                raise SSUnsupportedError(
+                    f'An ML Model with name "{add_ml_model.name}" already exists'
+                )
+            model.add_ml_model_object(add_ml_model)
+
+    @staticmethod
+    def _extend_entity_db_scripts(model: Model, db_scripts: t.List[DBScript]) -> None:
+        """
+        Ensures that the script/function names being added to the Ensemble are unique.
 
-    sys.exit(1)
+        This static method checks if the provided script/function names already exist
+        in the Ensemble. An SSUnsupportedError is raised if any duplicate names
+        are found. Otherwise, it appends the given list of DBScripts to the
+        Ensemble.
+
+        :param model: SmartSim Model object.
+        :param db_scripts: List of DBScripts to append to the Ensemble.
+        """
+        for add_script in db_scripts:
+            dupe = next(
+                (
+                    add_script.name
+                    for db_script in model.db_scripts
+                    if db_script.name == add_script.name
+                ),
+                None,
+            )
+            if dupe:
+                raise SSUnsupportedError(
+                    f'A Script with name "{add_script.name}" already exists'
+                )
+            model.add_script_object(add_script)
```

### Comparing `smartsim-0.6.2/smartsim/_core/generation/__init__.py` & `smartsim-0.7.0/smartsim/_core/generation/__init__.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.6.2/smartsim/_core/generation/generator.py` & `smartsim-0.7.0/smartsim/_core/generation/generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,33 +60,29 @@
         configured models within an ensemble if there
         is a name collision. Also replace any and all directories
         for the experiment with fresh copies. Otherwise, if overwrite
         is false, raises EntityExistsError when there is a name
         collision between entities.
 
         :param gen_path: Path in which files need to be generated
-        :type gen_path: str
-        :param overwrite: toggle entity replacement, defaults to False
-        :type overwrite: bool, optional
+        :param overwrite: toggle entity replacement
         :param verbose: Whether generation information should be logged to std out
-        :type verbose: bool, optional
         """
         self._writer = ModelWriter()
         self.gen_path = gen_path
         self.overwrite = overwrite
         self.log_level = DEBUG if not verbose else INFO
 
     @property
     def log_file(self) -> str:
         """Returns the location of the file
         summarizing the parameters used for the last generation
         of all generated entities.
 
         :returns: path to file with parameter settings
-        :rtype: str
         """
         return join(self.gen_path, "smartsim_params.txt")
 
     def generate_experiment(self, *args: t.Any) -> None:
         """Run ensemble and experiment file structure generation
 
         Generate the file structure for a SmartSim experiment. This
@@ -125,34 +121,30 @@
 
         A full regular expression might tag specific
         model configurations such that the configuration
         files don't need to be tagged manually.
 
         :param tag: A string of characters that signify
                     the string to be changed. Defaults to ``;``
-        :type tag: str
-
-        :param regex: full regex for the modelwriter to search for,
-                      defaults to None
-        :type regex: str | None
+        :param regex: full regex for the modelwriter to search for
         """
         self._writer.set_tag(tag, regex)
 
     def _gen_exp_dir(self) -> None:
         """Create the directory for an experiment if it does not
         already exist.
         """
 
         if path.isfile(self.gen_path):
             raise FileExistsError(
                 f"Experiment directory could not be created. {self.gen_path} exists"
             )
         if not path.isdir(self.gen_path):
             # keep exists ok for race conditions on NFS
-            pathlib.Path(self.gen_path).mkdir(exist_ok=True)
+            pathlib.Path(self.gen_path).mkdir(exist_ok=True, parents=True)
         else:
             logger.log(
                 level=self.log_level, msg="Working in previously created experiment"
             )
 
         # The log_file only keeps track of the last generation
         # this is to avoid gigantic files in case the user repeats
@@ -163,31 +155,29 @@
             log_file.write(f"Generation start date and time: {dt_string}\n")
 
     def _gen_orc_dir(self, orchestrator_list: t.List[Orchestrator]) -> None:
         """Create the directory that will hold the error, output and
            configuration files for the orchestrator.
 
         :param orchestrator: Orchestrator instance
-        :type orchestrator: Orchestrator | None
         """
         # Loop through orchestrators
         for orchestrator in orchestrator_list:
             orc_path = path.join(self.gen_path, orchestrator.name)
 
             orchestrator.set_path(orc_path)
             # Always remove orchestrator files if present.
             if path.isdir(orc_path):
                 shutil.rmtree(orc_path, ignore_errors=True)
-            pathlib.Path(orc_path).mkdir(exist_ok=self.overwrite)
+            pathlib.Path(orc_path).mkdir(exist_ok=self.overwrite, parents=True)
 
     def _gen_entity_list_dir(self, entity_lists: t.List[Ensemble]) -> None:
         """Generate directories for Ensemble instances
 
         :param entity_lists: list of Ensemble instances
-        :type entity_lists: list
         """
 
         if not entity_lists:
             return
 
         for elist in entity_lists:
             elist_dir = path.join(self.gen_path, elist.name)
@@ -205,17 +195,15 @@
         self,
         entities: t.List[Model],
         entity_list: t.Optional[Ensemble] = None,
     ) -> None:
         """Generate directories for Entity instances
 
         :param entities: list of Model instances
-        :type entities: list[Model]
-        :param entity_list: Ensemble instance, defaults to None
-        :type entity_list: Ensemble | None
+        :param entity_list: Ensemble instance
         :raises EntityExistsError: if a directory already exists for an
                                    entity by that name
         """
         if not entities:
             return
 
         for entity in entities:
@@ -243,26 +231,24 @@
     def _write_tagged_entity_files(self, entity: Model) -> None:
         """Read, configure and write the tagged input files for
            a Model instance within an ensemble. This function
            specifically deals with the tagged files attached to
            an Ensemble.
 
         :param entity: a Model instance
-        :type entity: Model
         """
         if entity.files:
             to_write = []
 
             def _build_tagged_files(tagged: TaggedFilesHierarchy) -> None:
                 """Using a TaggedFileHierarchy, reproduce the tagged file
                 directory structure
 
                 :param tagged: a TaggedFileHierarchy to be built as a
                                directory structure
-                :type tagged: TaggedFilesHierarchy
                 """
                 for file in tagged.files:
                     dst_path = path.join(entity.path, tagged.base, path.basename(file))
                     shutil.copyfile(file, dst_path)
                     to_write.append(dst_path)
 
                 for tagged_dir in tagged.dirs:
@@ -287,17 +273,15 @@
         self, entity: Model, files_to_params: t.Dict[str, t.Dict[str, str]]
     ) -> None:
         """Log which files were modified during generation
 
         and what values were set to the parameters
 
         :param entity: the model being generated
-        :type entity: Model
         :param files_to_params: a dict connecting each file to its parameter settings
-        :type files_to_params: t.Dict[str, t.Dict[str, str]]
         """
         used_params: t.Dict[str, str] = {}
         file_to_tables: t.Dict[str, str] = {}
         for file, params in files_to_params.items():
             used_params.update(params)
             table = tabulate(params.items(), headers=["Name", "Value"])
             file_to_tables[relpath(file, self.gen_path)] = table
@@ -329,28 +313,26 @@
             )
 
     @staticmethod
     def _copy_entity_files(entity: Model) -> None:
         """Copy the entity files and directories attached to this entity.
 
         :param entity: Model
-        :type entity: Model
         """
         if entity.files:
             for to_copy in entity.files.copy:
                 dst_path = path.join(entity.path, path.basename(to_copy))
                 if path.isdir(to_copy):
                     dir_util.copy_tree(to_copy, entity.path)
                 else:
                     shutil.copyfile(to_copy, dst_path)
 
     @staticmethod
     def _link_entity_files(entity: Model) -> None:
         """Symlink the entity files attached to this entity.
 
         :param entity: Model
-        :type entity: Model
         """
         if entity.files:
             for to_link in entity.files.link:
                 dst_path = path.join(entity.path, path.basename(to_link))
                 symlink(to_link, dst_path)
```

### Comparing `smartsim-0.6.2/smartsim/_core/generation/modelwriter.py` & `smartsim-0.7.0/smartsim/_core/generation/modelwriter.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+import collections
 import re
 import typing as t
 
 from smartsim.error.errors import SmartSimError
 
 from ...error import ParameterWriterError
 from ...log import get_logger
@@ -43,18 +44,16 @@
 
     def set_tag(self, tag: str, regex: t.Optional[str] = None) -> None:
         """Set the tag for the modelwriter to search for within
            tagged files attached to an entity.
 
         :param tag: tag for the modelwriter to search for,
                     defaults to semi-colon e.g. ";"
-        :type tag: str
         :param regex: full regex for the modelwriter to search for,
                      defaults to "(;.+;)"
-        :type regex: str, optional
         """
         if regex:
             self.regex = regex
         else:
             self.tag = tag
             self.regex = "".join(("(", tag, ".+", tag, ")"))
 
@@ -64,36 +63,31 @@
         params: t.Dict[str, str],
         make_missing_tags_fatal: bool = False,
     ) -> t.Dict[str, t.Dict[str, str]]:
         """Read, write and configure tagged files attached to a Model
            instance.
 
         :param tagged_files: list of paths to tagged files
-        :type model: list[str]
         :param params: model parameters
-        :type params: dict[str, str]
         :param make_missing_tags_fatal: raise an error if a tag is missing
-        :type make_missing_tags_fatal: bool
         :returns: A dict connecting each file to its parameter settings
-        :rtype: dict[str,dict[str,str]]
         """
         files_to_tags: t.Dict[str, t.Dict[str, str]] = {}
         for tagged_file in tagged_files:
             self._set_lines(tagged_file)
             used_tags = self._replace_tags(params, make_missing_tags_fatal)
             self._write_changes(tagged_file)
             files_to_tags[tagged_file] = used_tags
 
         return files_to_tags
 
     def _set_lines(self, file_path: str) -> None:
         """Set the lines for the modelwrtter to iterate over
 
         :param file_path: path to the newly created and tagged file
-        :type file_path: str
         :raises ParameterWriterError: if the newly created file cannot be read
         """
         try:
             with open(file_path, "r+", encoding="utf-8") as file_stream:
                 self.lines = file_stream.readlines()
         except (IOError, OSError) as e:
             raise ParameterWriterError(file_path) from e
@@ -113,51 +107,39 @@
     def _replace_tags(
         self, params: t.Dict[str, str], make_fatal: bool = False
     ) -> t.Dict[str, str]:
         """Replace the tagged parameters within the file attached to this
            model. The tag defaults to ";"
 
         :param model: The model instance
-        :type model: Model
         :param make_fatal: (Optional) Set to True to force a fatal error
             if a tag is not matched
-        :type make_fatal: bool
         :returns: A dict of parameter names and values set for the file
-        :rtype: dict[str,str]
         """
         edited = []
-        unused_tags: t.Dict[str, t.List[int]] = {}
+        unused_tags: t.DefaultDict[str, t.List[int]] = collections.defaultdict(list)
         used_params: t.Dict[str, str] = {}
-        for i, line in enumerate(self.lines):
-            search = re.search(self.regex, line)
-            if search:
-                while search:
-                    tagged_line = search.group(0)
-                    previous_value = self._get_prev_value(tagged_line)
-                    if self._is_ensemble_spec(tagged_line, params):
-                        new_val = str(params[previous_value])
-                        new_line = re.sub(self.regex, new_val, line, 1)
-                        search = re.search(self.regex, new_line)
-                        used_params[previous_value] = new_val
-                        if not search:
-                            edited.append(new_line)
-                        else:
-                            line = new_line
-
-                    # if a tag is found but is not in this model's configurations
-                    # put in placeholder value
-                    else:
-                        tag = tagged_line.split(self.tag)[1]
-                        if tag not in unused_tags:
-                            unused_tags[tag] = []
-                        unused_tags[tag].append(i + 1)
-                        edited.append(re.sub(self.regex, previous_value, line))
-                        search = None  # Move on to the next tag
-            else:
-                edited.append(line)
+        for i, line in enumerate(self.lines, 1):
+            while search := re.search(self.regex, line):
+                tagged_line = search.group(0)
+                previous_value = self._get_prev_value(tagged_line)
+                if self._is_ensemble_spec(tagged_line, params):
+                    new_val = str(params[previous_value])
+                    line = re.sub(self.regex, new_val, line, 1)
+                    used_params[previous_value] = new_val
+
+                # if a tag is found but is not in this model's configurations
+                # put in placeholder value
+                else:
+                    tag = tagged_line.split(self.tag)[1]
+                    unused_tags[tag].append(i)
+                    line = re.sub(self.regex, previous_value, line)
+                    break
+            edited.append(line)
+
         for tag, value in unused_tags.items():
             missing_tag_message = f"Unused tag {tag} on line(s): {str(value)}"
             if make_fatal:
                 raise SmartSimError(missing_tag_message)
             logger.warning(missing_tag_message)
         self.lines = edited
         return used_params
```

### Comparing `smartsim-0.6.2/smartsim/_core/launcher/__init__.py` & `smartsim-0.7.0/smartsim/_core/launcher/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,20 +20,22 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+from .dragon.dragonLauncher import DragonLauncher
 from .launcher import Launcher
 from .local.local import LocalLauncher
 from .lsf.lsfLauncher import LSFLauncher
 from .pbs.pbsLauncher import PBSLauncher
 from .slurm.slurmLauncher import SlurmLauncher
 
 __all__ = [
     "Launcher",
+    "DragonLauncher",
     "LocalLauncher",
     "LSFLauncher",
     "PBSLauncher",
     "SlurmLauncher",
 ]
```

### Comparing `smartsim-0.6.2/smartsim/_core/launcher/colocated.py` & `smartsim-0.7.0/smartsim/_core/launcher/colocated.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,19 +38,16 @@
 ) -> None:
     """Write the colocated launch script
 
     This file will be written into the cwd of the step that
     is created for this entity.
 
     :param file_name: name of the script to write
-    :type file_name: str
     :param db_log: log file for the db
-    :type db_log: str
     :param colocated_settings: db settings from entity run_settings
-    :type colocated_settings: dict[str, Any]
     """
 
     colocated_cmd = _build_colocated_wrapper_cmd(db_log, **colocated_settings)
 
     with open(file_name, "w", encoding="utf-8") as script_file:
         script_file.write("#!/bin/bash\n")
         script_file.write("set -e\n\n")
@@ -63,17 +60,22 @@
         # run cleanup after all exitcodes
         script_file.write("trap Cleanup exit\n\n")
 
         # force entrypoint to write some debug information to the
         # STDOUT of the job
         if colocated_settings["debug"]:
             script_file.write("export SMARTSIM_LOG_LEVEL=debug\n")
-
-        script_file.write(f"{colocated_cmd}\n")
-        script_file.write("DBPID=$!\n\n")
+        script_file.write(f"db_stdout=$({colocated_cmd})\n")
+        # extract and set DBPID within the shell script that is
+        # enclosed between __PID__ and sent to stdout by the colocated
+        # entrypoints file
+        script_file.write(
+            "DBPID=$(echo $db_stdout | sed -n "
+            "'s/.*__PID__\\([0-9]*\\)__PID__.*/\\1/p')\n"
+        )
 
         # Write the actual launch command for the app
         script_file.write("$@\n\n")
 
 
 def _build_colocated_wrapper_cmd(
     db_log: str,
@@ -84,29 +86,21 @@
     ifname: t.Optional[t.Union[str, t.List[str]]] = None,
     custom_pinning: t.Optional[str] = None,
     **kwargs: t.Any,
 ) -> str:
     """Build the command use to run a colocated DB application
 
     :param db_log: log file for the db
-    :type db_log: str
-    :param cpus: db cpus, defaults to 1
-    :type cpus: int, optional
-    :param rai_args: redisai args, defaults to None
-    :type rai_args: dict[str, str], optional
-    :param extra_db_args: extra redis args, defaults to None
-    :type extra_db_args: dict[str, str], optional
+    :param cpus: db cpus
+    :param rai_args: redisai args
+    :param extra_db_args: extra redis args
     :param port: port to bind DB to
-    :type port: int
     :param ifname: network interface(s) to bind DB to
-    :type ifname: str | list[str], optional
     :param db_cpu_list: The list of CPUs that the database should be limited to
-    :type db_cpu_list: str, optional
     :return: the command to run
-    :rtype: str
     """
     # pylint: disable=too-many-locals
 
     # create unique lockfile name to avoid symlink vulnerability
     # this is the lockfile all the processes in the distributed
     # application will try to acquire. since we use a local tmp
     # directory on the compute node, only one process can acquire
@@ -186,18 +180,16 @@
         db_cmd.extend(db_model_cmd)
 
     db_scripts = kwargs.get("db_scripts", None)
     if db_scripts:
         db_script_cmd = _build_db_script_cmd(db_scripts)
         db_cmd.extend(db_script_cmd)
 
-    # run colocated db in the background
-    db_cmd.append("&")
-
     cmd.extend(db_cmd)
+
     return " ".join(cmd)
 
 
 def _build_db_model_cmd(db_models: t.List[DBModel]) -> t.List[str]:
     cmd = []
     for db_model in db_models:
         cmd.append("+db_model")
@@ -231,15 +223,16 @@
     cmd = []
     for db_script in db_scripts:
         cmd.append("+db_script")
         cmd.append(f"--name={db_script.name}")
         if db_script.func:
             # Notice that here db_script.func is guaranteed to be a str
             # because we don't allow the user to pass a serialized function
-            sanitized_func = db_script.func.replace("\n", "\\n")
+            func = db_script.func
+            sanitized_func = func.replace("\n", "\\n")
             if not (
                 sanitized_func.startswith("'")
                 and sanitized_func.endswith("'")
                 or (sanitized_func.startswith('"') and sanitized_func.endswith('"'))
             ):
                 sanitized_func = '"' + sanitized_func + '"'
             cmd.append(f"--func={sanitized_func}")
```

### Comparing `smartsim-0.6.2/smartsim/_core/launcher/launcher.py` & `smartsim-0.7.0/smartsim/_core/launcher/launcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import abc
 import typing as t
 
+from ..._core.launcher.stepMapping import StepMap
 from ...error import AllocationError, LauncherError, SSUnsupportedError
 from ...settings import SettingsBase
 from .step import Step
 from .stepInfo import StepInfo, UnmanagedStepInfo
 from .stepMapping import StepMapping
 from .taskManager import TaskManager
 
@@ -65,14 +66,23 @@
     def run(self, step: Step) -> t.Optional[str]:
         raise NotImplementedError
 
     @abc.abstractmethod
     def stop(self, step_name: str) -> StepInfo:
         raise NotImplementedError
 
+    def add_step_to_mapping_table(self, name: str, step_map: StepMap) -> None:
+        """Add a StepMap to the Launcher step mapping table
+        making it monitor the step.
+
+        :param name: name of step to be added
+        :param step_map: step map of added step
+        """
+        self.step_mapping[name] = step_map
+
 
 class WLMLauncher(Launcher):  # cov-wlm
     """The base class for any Launcher that utilizes workload
     manager specific commands. This base class is used to provide
     implemented methods that are alike across all WLM launchers.
     """
 
@@ -90,23 +100,19 @@
     # of supported RunSettings types (see slurmLauncher.py for ex)
     def create_step(
         self, name: str, cwd: str, step_settings: SettingsBase
     ) -> Step:  # cov-wlm
         """Create a WLM job step
 
         :param name: name of the entity to be launched
-        :type name: str
         :param cwd: path to launch dir
-        :type cwd: str
         :param step_settings: batch or run settings for entity
-        :type step_settings: BatchSettings | RunSettings
         :raises SSUnsupportedError: if batch or run settings type isnt supported
         :raises LauncherError: if step creation fails
         :return: step instance
-        :rtype: Step
         """
         try:
             step_class = self.supported_rs[type(step_settings)]
         except KeyError:
             raise SSUnsupportedError(
                 f"RunSettings type {type(step_settings)} not supported by this launcher"
             ) from None
@@ -125,17 +131,15 @@
 
     def get_step_update(
         self, step_names: t.List[str]
     ) -> t.List[t.Tuple[str, t.Union[StepInfo, None]]]:  # cov-wlm
         """Get update for a list of job steps
 
         :param step_names: list of job steps to get updates for
-        :type step_names: list[str]
         :return: list of name, job update tuples
-        :rtype: list[(str, StepInfo)]
         """
         updates: t.List[t.Tuple[str, t.Union[StepInfo, None]]] = []
 
         # get updates of jobs managed by workload manager (PBS, Slurm, etc)
         # this is primarily batch jobs.
         s_names, step_ids = self.step_mapping.get_ids(step_names, managed=True)
         if len(step_ids) > 0:
@@ -158,17 +162,15 @@
 
     def _get_unmanaged_step_update(
         self, task_ids: t.List[str]
     ) -> t.List[UnmanagedStepInfo]:  # cov-wlm
         """Get step updates for Popen managed jobs
 
         :param task_ids: task id to check
-        :type task_ids: list[str]
         :return: list of step updates
-        :rtype: list[StepInfo]
         """
         updates = []
         for task_id in task_ids:
             stat, return_code, out, err = self.task_manager.get_task_update(task_id)
             update = UnmanagedStepInfo(stat, return_code, out, err)
             updates.append(update)
         return updates
```

### Comparing `smartsim-0.6.2/smartsim/_core/launcher/local/__init__.py` & `smartsim-0.7.0/smartsim/_core/launcher/dragon/__init__.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.6.2/smartsim/_core/launcher/local/local.py` & `smartsim-0.7.0/smartsim/_core/launcher/local/local.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,17 +55,15 @@
 
     def get_step_update(
         self, step_names: t.List[str]
     ) -> t.List[t.Tuple[str, t.Optional[StepInfo]]]:
         """Get status updates of each job step name provided
 
         :param step_names: list of step_names
-        :type step_names: list[str]
         :return: list of tuples for update
-        :rtype: list[tuple[str, StepInfo | None]]
         """
         # step ids are process ids of the tasks
         # as there is no WLM intermediary
         updates: t.List[t.Tuple[str, t.Optional[StepInfo]]] = []
         s_names, s_ids = self.step_mapping.get_ids(step_names, managed=False)
         for step_name, step_id in zip(s_names, s_ids):
             status, ret_code, out, err = self.task_manager.get_task_update(str(step_id))
@@ -74,31 +72,27 @@
             updates.append(update)
         return updates
 
     def get_step_nodes(self, step_names: t.List[str]) -> t.List[t.List[str]]:
         """Return the address of nodes assigned to the step
 
         :param step_names: list of step_names
-        :type step_names: list[str]
         :return: list of node addresses
-        :rtype: list[list[str]]
 
         TODO: Use socket to find the actual Lo address?
         """
         return [["127.0.0.1"] * len(step_names)]
 
     def run(self, step: Step) -> str:
         """Run a local step created by this launcher. Utilize the shell
            library to execute the command with a Popen. Output and error
            files will be written to the entity path.
 
         :param step: LocalStep instance to run
-        :type step: LocalStep
         :return: task_id of the newly created step
-        :rtype: str
         """
         if not self.task_manager.actively_monitoring:
             self.task_manager.start()
 
         out, err = step.get_output_files()
         cmd = step.get_launch_cmd()
 
@@ -114,17 +108,15 @@
         self.step_mapping.add(step.name, task_id=task_id, managed=False)
         return task_id
 
     def stop(self, step_name: str) -> UnmanagedStepInfo:
         """Stop a job step
 
         :param step_name: name of the step to be stopped
-        :type step_name: str
         :return: a UnmanagedStepInfo instance
-        :rtype: UnmanagedStepInfo
         """
         # step_id is task_id for local. Naming for consistency
         step_id = self.step_mapping[step_name].task_id
 
         self.task_manager.remove_task(str(step_id))
         _, ret_code, out, err = self.task_manager.get_task_update(str(step_id))
         step_info = UnmanagedStepInfo("Cancelled", ret_code, out, err)
```

### Comparing `smartsim-0.6.2/smartsim/_core/launcher/lsf/__init__.py` & `smartsim-0.7.0/smartsim/_core/launcher/local/__init__.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.6.2/smartsim/_core/launcher/lsf/lsfCommands.py` & `smartsim-0.7.0/smartsim/_core/launcher/lsf/lsfCommands.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,57 +29,50 @@
 from ..util.shell import execute_cmd
 
 
 def bjobs(args: t.List[str]) -> t.Tuple[str, str]:
     """Calls LSF bjobs with args
 
     :param args: List of command arguments
-    :type args: List of str
     :returns: Output and error of bjobs
     """
     cmd = ["bjobs"] + args
     _, out, error = execute_cmd(cmd)
     return out, error
 
 
 def bkill(args: t.List[str]) -> t.Tuple[int, str, str]:
     """Calls LSF bkill with args.
 
     returncode is also supplied in this function.
 
     :param args: list of command arguments
-    :type args: list of str
     :return: returncode, output and error
-    :rtype: (int, str, str)
     """
     cmd = ["bkill"] + args
     returncode, out, error = execute_cmd(cmd)
     return returncode, out, error
 
 
 def jskill(args: t.List[str]) -> t.Tuple[int, str, str]:
     """Calls LSF jskill with args.
 
     returncode is also supplied in this function.
 
     :param args: list of command arguments
-    :type args: list of str
     :return: returncode, output and error
-    :rtype: (int, str, str)
     """
 
     cmd = ["jskill"] + args
     returncode, out, error = execute_cmd(cmd)
     return returncode, out, error
 
 
 def jslist(args: t.List[str]) -> t.Tuple[str, str]:
     """Calls LSF jslist with args
 
     :param args: List of command arguments
-    :type args: List of str
     :returns: Output and error of jslist
-    :rtype: (str, str)
     """
     cmd = ["jslist"] + args
     _, out, err = execute_cmd(cmd)
     return out, err
```

### Comparing `smartsim-0.6.2/smartsim/_core/launcher/lsf/lsfLauncher.py` & `smartsim-0.7.0/smartsim/_core/launcher/lsf/lsfLauncher.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     JsrunSettings,
     MpiexecSettings,
     MpirunSettings,
     OrterunSettings,
     RunSettings,
     SettingsBase,
 )
-from ....status import STATUS_CANCELLED, STATUS_COMPLETED
+from ....status import SmartSimStatus
 from ...config import CONFIG
 from ..launcher import WLMLauncher
 from ..step import (
     BsubBatchStep,
     JsrunStep,
     LocalStep,
     MpiexecStep,
@@ -87,18 +87,16 @@
             RunSettings: LocalStep,
         }
 
     def run(self, step: Step) -> t.Optional[str]:
         """Run a job step through LSF
 
         :param step: a job step instance
-        :type step: Step
         :raises LauncherError: if launch fails
         :return: job step id if job is managed
-        :rtype: str
         """
         if not self.task_manager.actively_monitoring:
             self.task_manager.start()
 
         cmd_list = step.get_launch_cmd()
         step_id = None
         task_id = None
@@ -130,17 +128,15 @@
         self.step_mapping.add(step.name, step_id, task_id, step.managed)
         return step_id
 
     def stop(self, step_name: str) -> StepInfo:
         """Stop/cancel a job step
 
         :param step_name: name of the job to stop
-        :type step_name: str
         :return: update for job due to cancel
-        :rtype: StepInfo
         """
         stepmap = self.step_mapping[step_name]
         if stepmap.managed:
             if stepmap.step_id and "." in stepmap.step_id:
                 return_code, _, err = jskill([stepmap.step_id.rpartition(".")[-1]])
             else:
                 return_code, _, err = bkill([str(stepmap.step_id)])
@@ -151,15 +147,17 @@
         else:
             self.task_manager.remove_task(str(stepmap.task_id))
 
         _, step_info = self.get_step_update([step_name])[0]
         if not step_info:
             raise LauncherError(f"Could not get step_info for job step {step_name}")
 
-        step_info.status = STATUS_CANCELLED  # set status to cancelled instead of failed
+        step_info.status = (
+            SmartSimStatus.STATUS_CANCELLED
+        )  # set status to cancelled instead of failed
         return step_info
 
     @staticmethod
     def _get_lsf_step_id(step: Step, interval: int = 2) -> str:
         """Get the step_id of last launched step from jslist"""
         time.sleep(interval)
         step_id: t.Optional[str] = None
@@ -179,17 +177,15 @@
 
         return f"{step.alloc}.{step_id}"
 
     def _get_managed_step_update(self, step_ids: t.List[str]) -> t.List[StepInfo]:
         """Get step updates for WLM managed jobs
 
         :param step_ids: list of job step ids
-        :type step_ids: list[str]
         :return: list of updates for managed jobs
-        :rtype: list[StepInfo]
         """
         updates: t.List[StepInfo] = []
 
         for step_id in step_ids:
             # Batch jobs have integer step id,
             # Jsrun processes have {alloc}.{task_id}
             # Include recently finished jobs
@@ -203,14 +199,14 @@
             else:
                 bjobs_args = ["-a"] + step_ids
                 bjobs_out, _ = bjobs(bjobs_args)
                 stat = parse_bjobs_jobid(bjobs_out, str(step_id))
                 # create LSFBatchStepInfo objects to return
                 batch_info = LSFBatchStepInfo(stat, None)
                 # account for case where job history is not logged by LSF
-                if batch_info.status == STATUS_COMPLETED:
+                if batch_info.status == SmartSimStatus.STATUS_COMPLETED:
                     batch_info.returncode = 0
                 updates.append(batch_info)
         return updates
 
     def __str__(self) -> str:
         return "LSF"
```

### Comparing `smartsim-0.6.2/smartsim/_core/launcher/lsf/lsfParser.py` & `smartsim-0.7.0/smartsim/_core/launcher/lsf/lsfParser.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,31 +27,27 @@
 import typing as t
 
 
 def parse_bsub(output: str) -> str:
     """Parse bsub output and return job id.
 
     :param output: stdout of bsub command
-    :type output: str
     :returns: job id
-    :rtype: str
     """
     for line in output.split("\n"):
         if line.startswith("Job"):
             return line.split()[1][1:-1]
     return ""
 
 
 def parse_bsub_error(output: str) -> str:
     """Parse and return error output of a failed bsub command.
 
     :param output: stderr of qsub command
-    :type output: str
     :returns: error message
-    :rtype: str
     """
     # Search for first non-empty line
     error_lines = []
     copy_lines = False
     for line in output.split("\n"):
         if line.strip().startswith("**"):
             copy_lines = True
@@ -73,19 +69,16 @@
 
 
 def parse_jslist_stepid(output: str, step_id: str) -> t.Tuple[str, t.Optional[str]]:
     """Parse and return output of the jslist command run with
     options to obtain step status
 
     :param output: output of the bjobs command
-    :type output: str
     :param step_id: allocation id or job step id
-    :type step_id: str
     :return: status and return code
-    :rtype: (str, str)
     """
     result: t.Tuple[str, t.Optional[str]] = ("NOTFOUND", None)
 
     for line in output.split("\n"):
         fields = line.split()
         if len(fields) >= 7:
             if fields[0] == step_id:
@@ -97,19 +90,16 @@
 
 
 def parse_bjobs_jobid(output: str, job_id: str) -> str:
     """Parse and return output of the bjobs command run with options
     to obtain job status.
 
     :param output: output of the bjobs command
-    :type output: str
     :param job_id: allocation id or job step id
-    :type job_id: str
     :return: status
-    :rtype: str
     """
     result = "NOTFOUND"
     for line in output.split("\n"):
         fields = line.split()
         if len(fields) >= 3:
             if fields[0] == job_id:
                 stat = fields[2]
@@ -122,17 +112,15 @@
     """Parse and return the bjobs command run with
     options to obtain node list, i.e. with `-w`.
 
     This function parses and returns the nodes of
     a job in a list with the duplicates removed.
 
     :param output: output of the `bjobs -w` command
-    :type output: str
     :return: compute nodes of the allocation or job
-    :rtype: list of str
     """
     nodes = []
 
     lines = output.split("\n")
     nodes_str = lines[1].split()[5]
     nodes = nodes_str.split(":")
 
@@ -142,19 +130,16 @@
 def parse_max_step_id_from_jslist(output: str) -> t.Optional[str]:
     """Parse and return the maximum step id from a jslist command.
     This function must be called immedietaly after a call to jsrun,
     and before the next one, to ensure the id of the last spawned task is
     properly returned
 
     :param output: output bjobs
-    :type output: str
     :param step_name: the name of the step to query
-    :type step_name: str
     :return: the step_id
-    :rtype: str
     """
     max_step_id = None
 
     for line in output.split("\n"):
         if line.startswith("="):
             continue
         fields = line.split()
```

### Comparing `smartsim-0.6.2/smartsim/_core/launcher/pbs/__init__.py` & `smartsim-0.7.0/smartsim/_core/launcher/lsf/__init__.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.6.2/smartsim/_core/launcher/pbs/pbsCommands.py` & `smartsim-0.7.0/smartsim/_core/launcher/pbs/pbsCommands.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,40 +29,36 @@
 from ..util.shell import execute_cmd
 
 
 def qstat(args: t.List[str]) -> t.Tuple[str, str]:
     """Calls PBS qstat with args
 
     :param args: List of command arguments
-    :type args: List of str
     :returns: Output and error of qstat
     """
     cmd = ["qstat"] + args
     _, out, error = execute_cmd(cmd)
     return out, error
 
 
 def qsub(args: t.List[str]) -> t.Tuple[str, str]:
     """Calls PBS qsub with args
 
     :param args: List of command arguments
-    :type args: List of str
     :returns: Output and error of salloc
     """
     cmd = ["qsub"] + args
     _, out, error = execute_cmd(cmd)
     return out, error
 
 
 def qdel(args: t.List[str]) -> t.Tuple[int, str, str]:
     """Calls PBS qdel with args.
 
     returncode is also supplied in this function.
 
     :param args: list of command arguments
-    :type args: list of str
     :return: output and error
-    :rtype: str
     """
     cmd = ["qdel"] + args
     returncode, out, error = execute_cmd(cmd)
     return returncode, out, error
```

### Comparing `smartsim-0.6.2/smartsim/_core/launcher/pbs/pbsLauncher.py` & `smartsim-0.7.0/smartsim/_core/launcher/pbs/pbsLauncher.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,29 +35,33 @@
     MpirunSettings,
     OrterunSettings,
     PalsMpiexecSettings,
     QsubBatchSettings,
     RunSettings,
     SettingsBase,
 )
-from ....status import STATUS_CANCELLED, STATUS_COMPLETED
+from ....status import SmartSimStatus
 from ...config import CONFIG
 from ..launcher import WLMLauncher
 from ..step import (
     AprunStep,
     LocalStep,
     MpiexecStep,
     MpirunStep,
     OrterunStep,
     QsubBatchStep,
     Step,
 )
 from ..stepInfo import PBSStepInfo, StepInfo
 from .pbsCommands import qdel, qstat
-from .pbsParser import parse_qstat_jobid, parse_step_id_from_qstat
+from .pbsParser import (
+    parse_qstat_jobid,
+    parse_qstat_jobid_json,
+    parse_step_id_from_qstat,
+)
 
 logger = get_logger(__name__)
 
 
 class PBSLauncher(WLMLauncher):
     """This class encapsulates the functionality needed
     to launch jobs on systems that use PBS as a workload manager.
@@ -84,18 +88,16 @@
             PalsMpiexecSettings: MpiexecStep,
         }
 
     def run(self, step: Step) -> t.Optional[str]:
         """Run a job step through PBSPro
 
         :param step: a job step instance
-        :type step: Step
         :raises LauncherError: if launch fails
         :return: job step id if job is managed
-        :rtype: str
         """
         if not self.task_manager.actively_monitoring:
             self.task_manager.start()
 
         cmd_list = step.get_launch_cmd()
         step_id: t.Optional[str] = None
         task_id: t.Optional[str] = None
@@ -127,17 +129,15 @@
 
         return step_id
 
     def stop(self, step_name: str) -> StepInfo:
         """Stop/cancel a job step
 
         :param step_name: name of the job to stop
-        :type step_name: str
         :return: update for job due to cancel
-        :rtype: StepInfo
         """
         stepmap = self.step_mapping[step_name]
         if stepmap.managed:
             qdel_rc, _, err = qdel([str(stepmap.step_id)])
             if qdel_rc != 0:
                 logger.warning(f"Unable to cancel job step {step_name}\n {err}")
             if stepmap.task_id:
@@ -145,15 +145,17 @@
         else:
             self.task_manager.remove_task(str(stepmap.task_id))
 
         _, step_info = self.get_step_update([step_name])[0]
         if not step_info:
             raise LauncherError(f"Could not get step_info for job step {step_name}")
 
-        step_info.status = STATUS_CANCELLED  # set status to cancelled instead of failed
+        step_info.status = (
+            SmartSimStatus.STATUS_CANCELLED
+        )  # set status to cancelled instead of failed
         return step_info
 
     @staticmethod
     def _get_pbs_step_id(step: Step, interval: int = 2) -> str:
         """Get the step_id of a step from qstat (rarely used)
 
         Parses qstat JSON output by looking for the step name
@@ -174,28 +176,37 @@
             raise LauncherError("Could not find id of launched job step")
         return step_id
 
     def _get_managed_step_update(self, step_ids: t.List[str]) -> t.List[StepInfo]:
         """Get step updates for WLM managed jobs
 
         :param step_ids: list of job step ids
-        :type step_ids: list[str]
         :return: list of updates for managed jobs
-        :rtype: list[StepInfo]
         """
         updates: t.List[StepInfo] = []
 
         qstat_out, _ = qstat(step_ids)
         stats = [parse_qstat_jobid(qstat_out, str(step_id)) for step_id in step_ids]
+
+        # Fallback: if all jobs result as NOTFOUND, it might be an issue
+        # with truncated names, we resort to json format which does not truncate
+        # information
+        if all(stat is None for stat in stats):
+            qstat_out_json, _ = qstat(["-f", "-F", "json"] + step_ids)
+            stats = [
+                parse_qstat_jobid_json(qstat_out_json, str(step_id))
+                for step_id in step_ids
+            ]
+
         # create PBSStepInfo objects to return
 
         for stat, _ in zip(stats, step_ids):
-            info = PBSStepInfo(stat, None)
+            info = PBSStepInfo(stat or "NOTFOUND", None)
             # account for case where job history is not logged by PBS
-            if info.status == STATUS_COMPLETED:
+            if info.status == SmartSimStatus.STATUS_COMPLETED:
                 info.returncode = 0
 
             updates.append(info)
         return updates
 
     def __str__(self) -> str:
         return "PBS"
```

### Comparing `smartsim-0.6.2/smartsim/_core/launcher/pbs/pbsParser.py` & `smartsim-0.7.0/smartsim/_core/launcher/pbs/pbsParser.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,77 +29,87 @@
 
 
 def parse_qsub(output: str) -> str:
     """Parse qsub output and return job id. For PBS, the
     output is the job id itself.
 
     :param output: stdout of qsub command
-    :type output: str
     :returns: job id
-    :rtype: str
     """
     return output
 
 
 def parse_qsub_error(output: str) -> str:
     """Parse and return error output of a failed qsub command.
 
     :param output: stderr of qsub command
-    :type output: str
     :returns: error message
-    :rtype: str
     """
     # look for error first
     for line in output.split("\n"):
         if line.startswith("qsub:"):
             error = line.split(":")[1]
             return error.strip()
     # if no error line, take first line
     for line in output.split("\n"):
         return line.strip()
     # if neither, present a base error message
     base_err = "PBS run error"
     return base_err
 
 
-def parse_qstat_jobid(output: str, job_id: str) -> str:
+def parse_qstat_jobid(output: str, job_id: str) -> t.Optional[str]:
     """Parse and return output of the qstat command run with options
     to obtain job status.
 
     :param output: output of the qstat command
-    :type output: str
     :param job_id: allocation id or job step id
-    :type job_id: str
     :return: status
-    :rtype: str
     """
-    result = "NOTFOUND"
+    result = None
     for line in output.split("\n"):
         fields = line.split()
         if len(fields) >= 5:
             if fields[0] == job_id:
                 stat = fields[4]
                 result = stat
                 break
     return result
 
 
+def parse_qstat_jobid_json(output: str, job_id: str) -> t.Optional[str]:
+    """Parse and return output of the qstat command run with JSON options
+    to obtain job status.
+
+    :param output: output of the qstat command in JSON format
+    :param job_id: allocation id or job step id
+    :return: status
+    """
+    out_json = load_and_clean_json(output)
+
+    if "Jobs" not in out_json:
+        return None
+    jobs: dict[str, t.Any] = out_json["Jobs"]
+    job: t.Optional[dict[str, t.Any]] = jobs.get(job_id, None)
+    if job is None:
+        return None
+    return str(job.get("job_state", None))
+
+
 def parse_qstat_nodes(output: str) -> t.List[str]:
     """Parse and return the qstat command run with
     options to obtain node list.
 
     This function parses and returns the nodes of
     a job in a list with the duplicates removed.
 
     The `output` parameter must be in JSON format.
 
     :param output: output of the qstat command in JSON format
-    :type output: str
     :return: compute nodes of the allocation or job
-    :rtype: list of str
     """
     nodes: t.List[str] = []
     out_json = load_and_clean_json(output)
     if "Jobs" not in out_json:
         return nodes
     jobs = out_json["Jobs"]
     job = jobs[list(jobs.keys())[0]]
@@ -112,19 +122,16 @@
     return list(sorted(set(nodes)))
 
 
 def parse_step_id_from_qstat(output: str, step_name: str) -> t.Optional[str]:
     """Parse and return the step id from a qstat command
 
     :param output: output qstat
-    :type output: str
     :param step_name: the name of the step to query
-    :type step_name: str
     :return: the step_id
-    :rtype: str
     """
     step_id: t.Optional[str] = None
     out_json = load_and_clean_json(output)
 
     if "Jobs" not in out_json:
         return step_id
     jobs = out_json["Jobs"]
```

### Comparing `smartsim-0.6.2/smartsim/_core/launcher/slurm/__init__.py` & `smartsim-0.7.0/smartsim/_core/launcher/pbs/__init__.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.6.2/smartsim/_core/launcher/slurm/slurmCommands.py` & `smartsim-0.7.0/smartsim/_core/launcher/slurm/slurmCommands.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,74 +34,67 @@
 logger = get_logger(__name__)
 
 
 def sstat(args: t.List[str], *, raise_on_err: bool = False) -> t.Tuple[str, str]:
     """Calls sstat with args
 
     :param args: List of command arguments
-    :type args: List of str
     :returns: Output and error of sstat
     """
     _, out, err = _execute_slurm_cmd("sstat", args, raise_on_err=raise_on_err)
     return out, err
 
 
 def sacct(args: t.List[str], *, raise_on_err: bool = False) -> t.Tuple[str, str]:
     """Calls sacct with args
 
     :param args: List of command arguments
-    :type args: List of str
     :returns: Output and error of sacct
     """
     _, out, err = _execute_slurm_cmd("sacct", args, raise_on_err=raise_on_err)
     return out, err
 
 
 def salloc(args: t.List[str], *, raise_on_err: bool = False) -> t.Tuple[str, str]:
     """Calls slurm salloc with args
 
     :param args: List of command arguments
-    :type args: List of str
     :returns: Output and error of salloc
     """
     _, out, err = _execute_slurm_cmd("salloc", args, raise_on_err=raise_on_err)
     return out, err
 
 
 def sinfo(args: t.List[str], *, raise_on_err: bool = False) -> t.Tuple[str, str]:
     """Calls slurm sinfo with args
 
     :param args: List of command arguments
-    :type args: List of str
     :returns: Output and error of sinfo
     """
     _, out, err = _execute_slurm_cmd("sinfo", args, raise_on_err=raise_on_err)
     return out, err
 
 
 def scontrol(args: t.List[str], *, raise_on_err: bool = False) -> t.Tuple[str, str]:
     """Calls slurm scontrol with args
 
     :param args: List of command arguments
-    :type args: List of str
     :returns: Output and error of sinfo
     """
     _, out, err = _execute_slurm_cmd("scontrol", args, raise_on_err=raise_on_err)
     return out, err
 
 
 def scancel(args: t.List[str], *, raise_on_err: bool = False) -> t.Tuple[int, str, str]:
     """Calls slurm scancel with args.
 
     returncode is also supplied in this function.
 
     :param args: list of command arguments
-    :type args: list of str
     :return: output and error
-    :rtype: str
     """
     return _execute_slurm_cmd("scancel", args, raise_on_err=raise_on_err)
 
 
 def _find_slurm_command(cmd: str) -> str:
     try:
         full_cmd = expand_exe_path(cmd)
```

### Comparing `smartsim-0.6.2/smartsim/_core/launcher/slurm/slurmLauncher.py` & `smartsim-0.7.0/smartsim/_core/launcher/slurm/slurmLauncher.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     MpirunSettings,
     OrterunSettings,
     RunSettings,
     SbatchSettings,
     SettingsBase,
     SrunSettings,
 )
-from ....status import STATUS_CANCELLED
+from ....status import SmartSimStatus
 from ...config import CONFIG
 from ..launcher import WLMLauncher
 from ..step import (
     LocalStep,
     MpiexecStep,
     MpirunStep,
     OrterunStep,
@@ -96,18 +96,16 @@
         29917893.extern|nid00034|44860|
         29917893.0|nid00034|44887,45151,45152,45153,45154,45155|
         29917893.2|nid00034|45174|
 
         would return nid00034
 
         :param step_names: list of job step names
-        :type step_names: list[str]
         :raises LauncherError: if nodelist aquisition fails
         :return: list of hostnames
-        :rtype: list[str]
         """
         _, step_ids = self.step_mapping.get_ids(step_names, managed=True)
         step_str = _create_step_id_str([val for val in step_ids if val is not None])
         output, _ = sstat([step_str, "-i", "-n", "-p", "-a"], raise_on_err=True)
 
         # parse node list for each step
         node_lists = []
@@ -118,18 +116,16 @@
             raise LauncherError("Failed to retrieve nodelist from stat")
         return node_lists
 
     def run(self, step: Step) -> t.Optional[str]:
         """Run a job step through Slurm
 
         :param step: a job step instance
-        :type step: Step
         :raises LauncherError: if launch fails
         :return: job step id if job is managed
-        :rtype: str
         """
         self.check_for_slurm()
         if not self.task_manager.actively_monitoring:
             self.task_manager.start()
 
         cmd_list = step.get_launch_cmd()
         step_id = None
@@ -171,17 +167,15 @@
 
         return step_id
 
     def stop(self, step_name: str) -> StepInfo:
         """Step a job step
 
         :param step_name: name of the job to stop
-        :type step_name: str
         :return: update for job due to cancel
-        :rtype: StepInfo
         """
         stepmap = self.step_mapping[step_name]
         if stepmap.managed:
             step_id = str(stepmap.step_id)
             # Check if step_id is part of colon-separated run,
             # this is reflected in a '+' in the step id,
             # so that the format becomes 12345+1.0.
@@ -214,15 +208,17 @@
         else:
             self.task_manager.remove_task(str(stepmap.task_id))
 
         _, step_info = self.get_step_update([step_name])[0]
         if not step_info:
             raise LauncherError(f"Could not get step_info for job step {step_name}")
 
-        step_info.status = STATUS_CANCELLED  # set status to cancelled instead of failed
+        step_info.status = (
+            SmartSimStatus.STATUS_CANCELLED
+        )  # set status to cancelled instead of failed
         return step_info
 
     @staticmethod
     def _get_slurm_step_id(step: Step, interval: int = 2) -> str:
         """Get the step_id of a step from sacct
 
         Parses sacct output by looking for the step name
@@ -251,17 +247,15 @@
             raise LauncherError("Could not find id of launched job step")
         return step_id
 
     def _get_managed_step_update(self, step_ids: t.List[str]) -> t.List[StepInfo]:
         """Get step updates for WLM managed jobs
 
         :param step_ids: list of job step ids
-        :type step_ids: list[str]
         :return: list of updates for managed jobs
-        :rtype: list[StepInfo]
         """
         step_str = _create_step_id_str(step_ids)
         sacct_out, _ = sacct(
             ["--noheader", "-p", "-b", "--jobs", step_str], raise_on_err=True
         )
 
         # (status, returncode)
```

### Comparing `smartsim-0.6.2/smartsim/_core/launcher/slurm/slurmParser.py` & `smartsim-0.7.0/smartsim/_core/launcher/slurm/slurmParser.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,17 +39,15 @@
     return None
 
 
 def parse_salloc_error(output: str) -> t.Optional[str]:
     """Parse and return error output of a failed salloc command
 
     :param output: stderr output of salloc command
-    :type output: str
     :return: error message
-    :rtype: str
     """
     salloc = which("salloc")
     # look for error first
     for line in output.split("\n"):
         if salloc and line.startswith(salloc + ": error:"):
             error = line.split("error:")[1]
             return error.strip()
@@ -69,34 +67,30 @@
 
 
 def jobid_exact_match(parsed_id: str, job_id: str) -> bool:
     """Check that job_id is an exact match and not
     the prefix of another job_id, like 1 and 11
     or 1.1 and 1.10. Works with job id or step
     id (i.e. with or without a '.' in the id)
+
     :param parsed_id: the id read from the line
-    :type paserd_id: str
     :param job_id: the id to check for equality
-    :type job_id: str
     """
     if "." in job_id:
         return parsed_id == job_id
 
     return parsed_id.split(".")[0] == job_id
 
 
 def parse_sacct(output: str, job_id: str) -> t.Tuple[str, t.Optional[str]]:
     """Parse and return output of the sacct command
 
     :param output: output of the sacct command
-    :type output: str
     :param job_id: allocation id or job step id
-    :type job_id: str
     :return: status and returncode
-    :rtype: tuple
     """
     result: t.Tuple[str, t.Optional[str]] = ("PENDING", None)
     for line in output.split("\n"):
         parts = line.split("|")
         if len(parts) >= 3:
             if jobid_exact_match(parts[0], job_id):
                 stat = parts[1]
@@ -109,17 +103,15 @@
 def parse_sstat_nodes(output: str, job_id: str) -> t.List[str]:
     """Parse and return the sstat command
 
     This function parses and returns the nodes of
     a job in a list with the duplicates removed.
 
     :param output: output of the sstat command
-    :type output: str
     :return: compute nodes of the allocation or job
-    :rtype: list of str
     """
     nodes = []
     for line in output.split("\n"):
         sstat_string = line.split("|")
 
         # sometimes there are \n that we need to ignore
         if len(sstat_string) >= 2:
@@ -130,19 +122,16 @@
 
 
 def parse_step_id_from_sacct(output: str, step_name: str) -> t.Optional[str]:
     """Parse and return the step id from a sacct command
 
     :param output: output of sacct --noheader -p
                    --format=jobname,jobid --job <alloc>
-    :type output: str
     :param step_name: the name of the step to query
-    :type step_name: str
     :return: the step_id
-    :rtype: str
     """
     step_id = None
     for line in output.split("\n"):
         sacct_string = line.split("|")
         if len(sacct_string) >= 2:
             if sacct_string[0] == step_name:
                 step_id = sacct_string[1]
```

### Comparing `smartsim-0.6.2/smartsim/_core/launcher/step/__init__.py` & `smartsim-0.7.0/smartsim/_core/launcher/step/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,13 +21,14 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from .alpsStep import AprunStep
+from .dragonStep import DragonBatchStep, DragonStep
 from .localStep import LocalStep
 from .lsfStep import BsubBatchStep, JsrunStep
 from .mpiStep import MpiexecStep, MpirunStep, OrterunStep
 from .pbsStep import QsubBatchStep
 from .slurmStep import SbatchStep, SrunStep
 from .step import Step
```

### Comparing `smartsim-0.6.2/smartsim/_core/launcher/step/alpsStep.py` & `smartsim-0.7.0/smartsim/_core/launcher/step/alpsStep.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,19 +38,16 @@
 
 
 class AprunStep(Step):
     def __init__(self, name: str, cwd: str, run_settings: AprunSettings) -> None:
         """Initialize a ALPS aprun job step
 
         :param name: name of the entity to be launched
-        :type name: str
         :param cwd: path to launch dir
-        :type cwd: str
         :param run_settings: run settings for entity
-        :type run_settings: AprunSettings
         """
         super().__init__(name, cwd, run_settings)
         self.alloc: t.Optional[str] = None
         if not run_settings.in_batch:
             self._set_alloc()
         self.run_settings = run_settings
 
@@ -61,15 +58,14 @@
         return self.run_settings.mpmd
 
     @proxyable_launch_cmd
     def get_launch_cmd(self) -> t.List[str]:
         """Get the command to launch this step
 
         :return: launch command
-        :rtype: list[str]
         """
         aprun = self.run_settings.run_command
         if not aprun:
             logger.warning("aprun not found in PATH")
             raise RuntimeError("Could not find aprun in PATH")
 
         aprun_cmd = [aprun, "--wdir", self.cwd]
@@ -118,15 +114,14 @@
                 "No allocation specified or found and not running in batch"
             )
 
     def _build_exe(self) -> t.List[str]:
         """Build the executable for this step
 
         :return: executable list
-        :rtype: list[str]
         """
         if self._get_mpmd():
             return self._make_mpmd()
 
         exe = self.run_settings.exe
         args = self.run_settings._exe_args  # pylint: disable=protected-access
         return exe + args
```

### Comparing `smartsim-0.6.2/smartsim/_core/launcher/step/localStep.py` & `smartsim-0.7.0/smartsim/_core/launcher/step/localStep.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.6.2/smartsim/_core/launcher/step/lsfStep.py` & `smartsim-0.7.0/smartsim/_core/launcher/step/lsfStep.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,49 +38,43 @@
 
 
 class BsubBatchStep(Step):
     def __init__(self, name: str, cwd: str, batch_settings: BsubBatchSettings) -> None:
         """Initialize a LSF bsub step
 
         :param name: name of the entity to launch
-        :type name: str
         :param cwd: path to launch dir
-        :type cwd: str
         :param batch_settings: batch settings for entity
-        :type batch_settings: BsubBatchSettings
         """
         super().__init__(name, cwd, batch_settings)
         self.step_cmds: t.List[t.List[str]] = []
         self.managed = True
         self.batch_settings = batch_settings
 
     def get_launch_cmd(self) -> t.List[str]:
         """Get the launch command for the batch
 
         :return: launch command for the batch
-        :rtype: list[str]
         """
         script = self._write_script()
         return [self.batch_settings.batch_cmd, script]
 
     def add_to_batch(self, step: Step) -> None:
         """Add a job step to this batch
 
         :param step: a job step instance e.g. SrunStep
-        :type step: Step
         """
         launch_cmd = step.get_launch_cmd()
         self.step_cmds.append(launch_cmd)
         logger.debug(f"Added step command to batch for {step.name}")
 
     def _write_script(self) -> str:
         """Write the batch script
 
         :return: batch script path after writing
-        :rtype: str
         """
         batch_script = self.get_step_file(ending=".sh")
         output, error = self.get_output_files()
 
         self.batch_settings._format_alloc_flags()  # pylint: disable=protected-access
 
         opts = self.batch_settings.format_batch_args()
@@ -109,19 +103,16 @@
 
 
 class JsrunStep(Step):
     def __init__(self, name: str, cwd: str, run_settings: RunSettings):
         """Initialize a LSF jsrun job step
 
         :param name: name of the entity to be launched
-        :type name: str
         :param cwd: path to launch dir
-        :type cwd: str
         :param run_settings: run settings for entity
-        :type run_settings: RunSettings
         """
         super().__init__(name, cwd, run_settings)
         self.alloc: t.Optional[str] = None
         self.managed = True
         self.run_settings = run_settings
         if not self.run_settings.in_batch:
             self._set_alloc()
@@ -151,15 +142,14 @@
 
         return output, error
 
     def get_launch_cmd(self) -> t.List[str]:
         """Get the command to launch this step
 
         :return: launch command
-        :rtype: list[str]
         """
         jsrun = self.run_settings.run_command
         if not jsrun:
             logger.warning("jsrun not found in PATH")
             raise RuntimeError("Could not find jsrun in PATH")
 
         output, error = self.get_output_files()
@@ -219,15 +209,14 @@
             return self.step_settings.mpmd
         return []
 
     def _build_exe(self) -> t.List[str]:
         """Build the executable for this step
 
         :return: executable list
-        :rtype: list[str]
         """
         exe = self.run_settings.exe
         args = self.run_settings._exe_args  # pylint: disable=protected-access
 
         if self._get_mpmd():
             erf_file = self.get_step_file(ending=".mpmd")
             self._make_mpmd()
```

### Comparing `smartsim-0.6.2/smartsim/_core/launcher/step/mpiStep.py` & `smartsim-0.7.0/smartsim/_core/launcher/step/mpiStep.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,19 +39,16 @@
 
 
 class _BaseMPIStep(Step):
     def __init__(self, name: str, cwd: str, run_settings: RunSettings) -> None:
         """Initialize a job step conforming to the MPI standard
 
         :param name: name of the entity to be launched
-        :type name: str
         :param cwd: path to launch dir
-        :type cwd: str
         :param run_settings: run settings for entity
-        :type run_settings: RunSettings
         """
 
         super().__init__(name, cwd, run_settings)
 
         self.alloc: t.Optional[str] = None
         if not run_settings.in_batch:
             self._set_alloc()
@@ -60,15 +57,14 @@
     _supported_launchers = ["PBS", "SLURM", "LSB"]
 
     @proxyable_launch_cmd
     def get_launch_cmd(self) -> t.List[str]:
         """Get the command to launch this step
 
         :return: launch command
-        :rtype: list[str]
         """
         run_cmd = self.run_settings.run_command
         if not run_cmd:
             raise SmartSimError("No run command specified")
 
         mpi_cmd = [run_cmd, "--wdir", self.cwd]
         # add env vars to mpi command
@@ -126,15 +122,14 @@
             return rs_mpmd
         return []
 
     def _build_exe(self) -> t.List[str]:
         """Build the executable for this step
 
         :return: executable list
-        :rtype: list[str]
         """
         if self._get_mpmd():
             return self._make_mpmd()
 
         exe = self.run_settings.exe
         args = self.run_settings._exe_args  # pylint: disable=protected-access
         return exe + args
@@ -157,54 +152,42 @@
 
 
 class MpiexecStep(_BaseMPIStep):
     def __init__(self, name: str, cwd: str, run_settings: MpiexecSettings) -> None:
         """Initialize an mpiexec job step
 
         :param name: name of the entity to be launched
-        :type name: str
         :param cwd: path to launch dir
-        :type cwd: str
         :param run_settings: run settings for entity
-        :type run_settings: MpiexecSettings
         :param default_run_command: The default command to launch an MPI
                                     application
-        :type default_run_command: str, optional
         """
 
         super().__init__(name, cwd, run_settings)
 
 
 class MpirunStep(_BaseMPIStep):
     def __init__(self, name: str, cwd: str, run_settings: MpirunSettings) -> None:
         """Initialize an mpirun job step
 
         :param name: name of the entity to be launched
-        :type name: str
         :param cwd: path to launch dir
-        :type cwd: str
         :param run_settings: run settings for entity
-        :type run_settings: MpirunSettings
         :param default_run_command: The default command to launch an MPI
                                     application
-        :type default_run_command: str, optional
         """
 
         super().__init__(name, cwd, run_settings)
 
 
 class OrterunStep(_BaseMPIStep):
     def __init__(self, name: str, cwd: str, run_settings: OrterunSettings) -> None:
         """Initialize an orterun job step
 
         :param name: name of the entity to be launched
-        :type name: str
         :param cwd: path to launch dir
-        :type cwd: str
         :param run_settings: run settings for entity
-        :type run_settings: OrterunSettings
         :param default_run_command: The default command to launch an MPI
                                     application
-        :type default_run_command: str, optional
         """
 
         super().__init__(name, cwd, run_settings)
```

### Comparing `smartsim-0.6.2/smartsim/_core/launcher/step/pbsStep.py` & `smartsim-0.7.0/smartsim/_core/launcher/step/pbsStep.py`

 * *Files 15% similar despite different names*

```diff
@@ -34,49 +34,43 @@
 
 
 class QsubBatchStep(Step):
     def __init__(self, name: str, cwd: str, batch_settings: QsubBatchSettings) -> None:
         """Initialize a PBSpro qsub step
 
         :param name: name of the entity to launch
-        :type name: str
         :param cwd: path to launch dir
-        :type cwd: str
         :param batch_settings: batch settings for entity
-        :type batch_settings: QsubBatchSettings
         """
         super().__init__(name, cwd, batch_settings)
         self.step_cmds: t.List[t.List[str]] = []
         self.managed = True
         self.batch_settings = batch_settings
 
     def get_launch_cmd(self) -> t.List[str]:
         """Get the launch command for the batch
 
         :return: launch command for the batch
-        :rtype: list[str]
         """
         script = self._write_script()
         return [self.batch_settings.batch_cmd, script]
 
     def add_to_batch(self, step: Step) -> None:
         """Add a job step to this batch
 
         :param step: a job step instance e.g. SrunStep
-        :type step: Step
         """
         launch_cmd = step.get_launch_cmd()
         self.step_cmds.append(launch_cmd)
         logger.debug(f"Added step command to batch for {step.name}")
 
     def _write_script(self) -> str:
         """Write the batch script
 
         :return: batch script path after writing
-        :rtype: str
         """
         batch_script = self.get_step_file(ending=".sh")
         output, error = self.get_output_files()
         with open(batch_script, "w", encoding="utf-8") as script_file:
             script_file.write("#!/bin/bash\n\n")
             script_file.write(f"#PBS -o {output}\n")
             script_file.write(f"#PBS -e {error}\n")
```

### Comparing `smartsim-0.6.2/smartsim/_core/launcher/step/slurmStep.py` & `smartsim-0.7.0/smartsim/_core/launcher/step/slurmStep.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,50 +38,44 @@
 
 
 class SbatchStep(Step):
     def __init__(self, name: str, cwd: str, batch_settings: SbatchSettings) -> None:
         """Initialize a Slurm Sbatch step
 
         :param name: name of the entity to launch
-        :type name: str
         :param cwd: path to launch dir
-        :type cwd: str
         :param batch_settings: batch settings for entity
-        :type batch_settings: SbatchSettings
         """
         super().__init__(name, cwd, batch_settings)
         self.step_cmds: t.List[t.List[str]] = []
         self.managed = True
         self.batch_settings = batch_settings
 
     def get_launch_cmd(self) -> t.List[str]:
         """Get the launch command for the batch
 
         :return: launch command for the batch
-        :rtype: list[str]
         """
         script = self._write_script()
         return [self.batch_settings.batch_cmd, "--parsable", script]
 
     def add_to_batch(self, step: Step) -> None:
         """Add a job step to this batch
 
         :param step: a job step instance e.g. SrunStep
-        :type step: Step
         """
         launch_cmd = ["cd", step.cwd, ";"]
         launch_cmd += step.get_launch_cmd()
         self.step_cmds.append(launch_cmd)
         logger.debug(f"Added step command to batch for {step.name}")
 
     def _write_script(self) -> str:
         """Write the batch script
 
         :return: batch script path after writing
-        :rtype: str
         """
         batch_script = self.get_step_file(ending=".sh")
         output, error = self.get_output_files()
         with open(batch_script, "w", encoding="utf-8") as script_file:
             script_file.write("#!/bin/bash\n\n")
             script_file.write(f"#SBATCH --output={output}\n")
             script_file.write(f"#SBATCH --error={error}\n")
@@ -104,32 +98,28 @@
 
 
 class SrunStep(Step):
     def __init__(self, name: str, cwd: str, run_settings: SrunSettings) -> None:
         """Initialize a srun job step
 
         :param name: name of the entity to be launched
-        :type name: str
         :param cwd: path to launch dir
-        :type cwd: str
         :param run_settings: run settings for entity
-        :type run_settings: SrunSettings
         """
         super().__init__(name, cwd, run_settings)
         self.alloc: t.Optional[str] = None
         self.managed = True
         self.run_settings = run_settings
         if not self.run_settings.in_batch:
             self._set_alloc()
 
     def get_launch_cmd(self) -> t.List[str]:
         """Get the command to launch this step
 
         :return: launch command
-        :rtype: list[str]
         """
         srun = self.run_settings.run_command
         if not srun:
             raise ValueError("No srun command found in PATH")
 
         output, error = self.get_output_files()
 
@@ -202,15 +192,14 @@
         args: t.List[str] = exe_args if isinstance(exe_args, list) else [exe_args]
         return args
 
     def _build_exe(self) -> t.List[str]:
         """Build the executable for this step
 
         :return: executable list
-        :rtype: list[str]
         """
         if self._get_mpmd():
             return self._make_mpmd()
 
         exe = self.run_settings.exe
         args = self._get_exe_args_list(self.run_settings)
         return exe + args
```

### Comparing `smartsim-0.6.2/smartsim/_core/launcher/step/step.py` & `smartsim-0.7.0/smartsim/_core/launcher/step/step.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from __future__ import annotations
 
 import functools
 import os.path as osp
+import pathlib
 import sys
 import time
 import typing as t
 from os import makedirs
 
 from smartsim._core.config import CONFIG
 from smartsim.error.errors import SmartSimError, UnproxyableStepError
@@ -62,18 +63,29 @@
         raise NotImplementedError
 
     @staticmethod
     def _create_unique_name(entity_name: str) -> str:
         step_name = entity_name + "-" + get_base_36_repr(time.time_ns())
         return step_name
 
+    @staticmethod
+    def _ensure_output_directory_exists(output_dir: str) -> None:
+        """Create the directory for the step output if it doesn't exist already"""
+        if not osp.exists(output_dir):
+            pathlib.Path(output_dir).mkdir(parents=True, exist_ok=True)
+
     def get_output_files(self) -> t.Tuple[str, str]:
-        """Return two paths to error and output files based on cwd"""
-        output = self.get_step_file(ending=".out")
-        error = self.get_step_file(ending=".err")
+        """Return two paths to error and output files based on metadata directory"""
+        try:
+            output_dir = self.meta["status_dir"]
+        except KeyError as exc:
+            raise KeyError("Status directory for this step has not been set.") from exc
+        self._ensure_output_directory_exists(output_dir)
+        output = osp.join(output_dir, f"{self.entity_name}.out")
+        error = osp.join(output_dir, f"{self.entity_name}.err")
         return output, error
 
     def get_step_file(
         self, ending: str = ".sh", script_name: t.Optional[str] = None
     ) -> str:
         """Get the name for a file/script created by the step class
 
@@ -110,56 +122,67 @@
         return script_path
 
     # pylint: disable=no-self-use
     def add_to_batch(self, step: Step) -> None:
         """Add a job step to this batch
 
         :param step: a job step instance e.g. SrunStep
-        :type step: Step
         """
         raise SmartSimError("add_to_batch not implemented for this step type")
 
 
 _StepT = t.TypeVar("_StepT", bound=Step)
 
 
 def proxyable_launch_cmd(
     fn: t.Callable[[_StepT], t.List[str]], /
 ) -> t.Callable[[_StepT], t.List[str]]:
     @functools.wraps(fn)
     def _get_launch_cmd(self: _StepT) -> t.List[str]:
+        """
+        Generate a launch command that executes the `JobStep` with the
+        indirect launching entrypoint instead of directly. The original
+        command is passed to the proxy as a base64 encoded string.
+
+        Steps implementing `get_launch_cmd` and decorated with
+        `proxyable_launch_cmd` will generate status updates that can be consumed
+        by the telemetry monitor and dashboard"""
         original_cmd_list = fn(self)
 
         if not CONFIG.telemetry_enabled:
             return original_cmd_list
 
         if self.managed:
             raise UnproxyableStepError(
-                f"Attempting to proxy managed step of type {type(self)}"
+                f"Attempting to proxy managed step of type {type(self)} "
                 "through the unmanaged step proxy entry point"
             )
 
         proxy_module = "smartsim._core.entrypoints.indirect"
-        etype = self.meta["entity_type"]
+        entity_type = self.meta["entity_type"]
         status_dir = self.meta["status_dir"]
+
+        logger.debug(f"Encoding command{' '.join(original_cmd_list)}")
+
+        # encode the original cmd to avoid potential collisions and escaping
+        # errors when passing it using CLI arguments to the indirect entrypoint
         encoded_cmd = encode_cmd(original_cmd_list)
 
-        # NOTE: this is NOT safe. should either 1) sign cmd and verify OR 2)
-        #       serialize step and let the indirect entrypoint rebuild the
-        #       cmd... for now, test away...
+        # return a new command that executes the proxy and passes
+        # the original command as an argument
         return [
             sys.executable,
             "-m",
             proxy_module,
             "+name",
             self.name,
             "+command",
             encoded_cmd,
             "+entity_type",
-            etype,
+            entity_type,
             "+telemetry_dir",
             status_dir,
             "+working_dir",
             self.cwd,
         ]
 
     return _get_launch_cmd
```

### Comparing `smartsim-0.6.2/smartsim/_core/launcher/stepMapping.py` & `smartsim-0.7.0/smartsim/_core/launcher/stepMapping.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.6.2/smartsim/_core/launcher/taskManager.py` & `smartsim-0.7.0/smartsim/_core/launcher/taskManager.py`

 * *Files 12% similar despite different names*

```diff
@@ -110,25 +110,19 @@
     ) -> str:
         """Start a task managed by the TaskManager
 
         This is an "unmanaged" task, meaning it is NOT managed
         by a workload manager
 
         :param cmd_list: command to run
-        :type cmd_list: list[str]
         :param cwd: current working directory
-        :type cwd: str
         :param env: environment to launch with
-        :type env: dict[str, str], optional. If None, calling environment is inherited
-        :param out: output file, defaults to PIPE
-        :type out: file, optional
-        :param err: error file, defaults to PIPE
-        :type err: file, optional
+        :param out: output file
+        :param err: error file
         :return: task id
-        :rtype: int
         """
         with self._lock:
             proc = execute_async_cmd(cmd_list, cwd, env=env, out=out, err=err)
             task = Task(proc)
             if VERBOSE_TM:
                 logger.debug(f"Starting Task {task.pid}")
             self.tasks.append(task)
@@ -146,34 +140,28 @@
 
         This method is used by launchers to launch managed tasks
         meaning that they ARE managed by a WLM.
 
         This is primarily used for batch job launches
 
         :param cmd_list: command to run
-        :type cmd_list: list[str]
         :param cwd: current working directory
-        :type cwd: str
         :param env: environment to launch with
-        :type env: dict[str, str], optional
-        :param timeout: time to wait, defaults to None
-        :type timeout: int, optional
+        :param timeout: time to wait
         :return: returncode, output, and err
-        :rtype: int, str, str
         """
         returncode, out, err = execute_cmd(cmd_list, cwd=cwd, env=env, timeout=timeout)
         if VERBOSE_TM:
             logger.debug("Ran and waited on task")
         return returncode, out, err
 
     def add_existing(self, task_id: int) -> None:
         """Add existing task to be managed by the TaskManager
 
         :param task_id: task id of existing task
-        :type task_id: str
         :raises LauncherError: If task cannot be found
         """
         with self._lock:
             try:
                 process = psutil.Process(pid=task_id)
                 task = Task(process)
                 self.tasks.append(task)
@@ -182,15 +170,14 @@
                 msg = f"Process provided {task_id} does not exist"
                 raise LauncherError(msg) from None
 
     def remove_task(self, task_id: str) -> None:
         """Remove a task from the TaskManager
 
         :param task_id: id of the task to remove
-        :type task_id: str
         """
         with self._lock:
             if VERBOSE_TM:
                 logger.debug(f"Removing Task {task_id}")
             try:
                 task = self[task_id]
                 if task.is_alive:
@@ -206,17 +193,15 @@
 
     def get_task_update(
         self, task_id: str
     ) -> t.Tuple[str, t.Optional[int], t.Optional[str], t.Optional[str]]:
         """Get the update of a task
 
         :param task_id: task id
-        :type task_id: str
         :return: status, returncode, output, error
-        :rtype: str, int, str, str
         """
         with self._lock:
             try:
                 return_code, out, err = self.task_history[task_id]
                 # has to be == None because rc can be 0
                 if return_code is None:
                     try:
@@ -247,21 +232,17 @@
         err: t.Optional[str] = None,
     ) -> None:
         """Add a task to the task history
 
         Add a task to record its future returncode, output and error
 
         :param task_id: id of the task
-        :type task_id: str
         :param returncode: returncode
-        :type returncode: int, defaults to None
-        :param out: output, defaults to None
-        :type out: str, optional
-        :param err: output, defaults to None
-        :type err: str, optional
+        :param out: output
+        :param err: output
         """
         self.task_history[task_id] = (returncode, out, err)
 
     def __getitem__(self, task_id: str) -> Task:
         with self._lock:
             for task in self.tasks:
                 if task.pid == task_id:
@@ -274,39 +255,36 @@
 
 
 class Task:
     def __init__(self, process: psutil.Process) -> None:
         """Initialize a task
 
         :param process: Popen object
-        :type process: psutil.Process
         """
         self.process = process
         self.pid = str(self.process.pid)
 
     def check_status(self) -> t.Optional[int]:
         """Ping the job and return the returncode if finished
 
         :return: returncode if finished otherwise None
-        :rtype: int
         """
         if self.owned and isinstance(self.process, psutil.Popen):
             poll_result = self.process.poll()
             if poll_result is not None:
                 return int(poll_result)
             return None
         # we can't manage Processed we don't own
         # have to rely on .kill() to stop.
         return self.returncode
 
     def get_io(self) -> t.Tuple[t.Optional[str], t.Optional[str]]:
         """Get the IO from the subprocess
 
         :return: output and error from the Popen
-        :rtype: str, str
         """
         # Process class does not implement communicate
         if not self.owned or not isinstance(self.process, psutil.Popen):
             return None, None
 
         output, error = self.process.communicate()
         if output:
@@ -331,16 +309,15 @@
         if alive:
             for proc in alive:
                 logger.warning(f"Unable to kill emitted process {proc.pid}")
 
     def terminate(self, timeout: int = 10) -> None:
         """Terminate a this process and all children.
 
-        :param timeout: time to wait for task death, defaults to 10
-        :type timeout: int, optional
+        :param timeout: time to wait for task death
         """
 
         def terminate_callback(proc: psutil.Process) -> None:
             logger.debug(f"Cleanly terminated task {proc.pid}")
 
         children = self.process.children(recursive=True)
         children.append(self.process)  # add parent process to be killed
```

### Comparing `smartsim-0.6.2/smartsim/_core/launcher/util/__init__.py` & `smartsim-0.7.0/smartsim/_core/launcher/slurm/__init__.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.6.2/smartsim/_core/launcher/util/launcherUtil.py` & `smartsim-0.7.0/smartsim/_core/launcher/util/launcherUtil.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,29 +34,26 @@
 
     def __init__(
         self, node_name: t.Optional[str] = None, node_ppn: t.Optional[int] = None
     ) -> None:
         """Initialize a ComputeNode
 
         :param node_name: the name of the node
-        :type node_name: str
         :param node_ppn: the number of ppn
-        :type node_ppn: int
         """
         self.name: t.Optional[str] = node_name
         self.ppn: t.Optional[int] = node_ppn
 
     def _is_valid_node(self) -> bool:
         """Check if the node is complete
 
         Currently, validity is judged by name
         and ppn being not None.
 
         :returns: True if valid, false otherwise
-        :rtype: bool
         """
         if self.name is None:
             return False
         if self.ppn is None:
             return False
 
         return True
@@ -76,15 +73,14 @@
     def _is_valid_partition(self) -> bool:
         """Check if the partition is valid
 
         Currently, validity is judged by name
         and each ComputeNode being valid
 
         :returns: True if valid, false otherwise
-        :rtype: bool
         """
         if self.name is None:
             return False
         if len(self.nodes) <= 0:
             return False
         for node in self.nodes:
             if not node._is_valid_node():  # pylint: disable=protected-access
```

### Comparing `smartsim-0.6.2/smartsim/_core/launcher/util/shell.py` & `smartsim-0.7.0/smartsim/_core/launcher/util/shell.py`

 * *Files 11% similar despite different names*

```diff
@@ -45,30 +45,22 @@
     env: t.Optional[t.Dict[str, str]] = None,
     proc_input: str = "",
     timeout: t.Optional[int] = None,
 ) -> t.Tuple[int, str, str]:
     """Execute a command locally
 
     :param cmd_list: list of command with arguments
-    :type cmd_list: list of str
-    :param shell: run in system shell, defaults to False
-    :type shell: bool, optional
-    :param cwd: current working directory, defaults to None
-    :type cwd: str, optional
-    :param env: environment to launcher process with,
-                defaults to None (current env)
-    :type env: dict[str, str], optional
-    :param proc_input: input to the process, defaults to ""
-    :type proc_input: str, optional
-    :param timeout: timeout of the process, defaults to None
-    :type timeout: int, optional
+    :param shell: run in system shell
+    :param cwd: current working directory
+    :param env: environment to launcher process with
+    :param proc_input: input to the process
+    :param timeout: timeout of the process
     :raises ShellError: if timeout of process was exceeded
     :raises ShellError: if child process raises an error
     :return: returncode, output, and error of the process
-    :rtype: tuple of (int, str, str)
     """
     if VERBOSE_SHELL:
         source = "shell" if shell else "Popen"
         logger.debug(f"Executing {source} cmd: {' '.join(cmd_list)}")
 
     # spawning the subprocess and connecting to its output
     proc = psutil.Popen(
@@ -102,21 +94,17 @@
 ) -> psutil.Popen:
     """Execute an asynchronous command
 
     This function executes an asynchronous command and returns a
     popen subprocess object wrapped with psutil.
 
     :param cmd_list: list of command with arguments
-    :type cmd_list: list of str
     :param cwd: current working directory
-    :type cwd: str
     :param env: environment variables to set
-    :type env: dict[str, str]
     :return: the subprocess object
-    :rtype: psutil.Popen
     """
     if VERBOSE_SHELL:
         logger.debug(f"Executing command: {' '.join(cmd_list)}")
 
     try:
         popen_obj = psutil.Popen(
             cmd_list, cwd=cwd, stdout=out, stderr=err, env=env, close_fds=True
```

### Comparing `smartsim-0.6.2/smartsim/_core/utils/__init__.py` & `smartsim-0.7.0/smartsim/ml/torch/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,9 +20,8 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from .helpers import colorize, delete_elements, init_default, installed_redisai_backends
-from .redis import check_cluster_status, create_cluster, db_is_active
+from .data import DataLoader, DynamicDataGenerator, StaticDataGenerator
```

### Comparing `smartsim-0.6.2/smartsim/_core/utils/redis.py` & `smartsim-0.7.0/smartsim/_core/utils/redis.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,31 +49,29 @@
 def create_cluster(hosts: t.List[str], ports: t.List[int]) -> None:  # cov-wlm
     """Connect launched cluster instances.
 
     Should only be used in the case where cluster initialization
     needs to occur manually which is not often.
 
     :param hosts: List of hostnames to connect to
-    :type hosts: List[str]
     :param ports: List of ports for each hostname
-    :type ports: List[int]
     :raises SmartSimError: if cluster creation fails
     """
     ip_list = []
     for host in hosts:
         ip_address = get_ip_from_host(host)
         for port in ports:
             address = ":".join((ip_address, str(port) + " "))
             ip_list.append(address)
 
     # call cluster command
     redis_cli = CONFIG.database_cli
     cmd = [redis_cli, "--cluster", "create"]
     cmd += ip_list
-    cmd += ["--cluster-replicas", "0"]
+    cmd += ["--cluster-replicas", "0", "--cluster-yes"]
     returncode, out, err = execute_cmd(cmd, proc_input="yes", shell=False)
 
     if returncode != 0:
         logger.error(out)
         logger.error(err)
         raise SSInternalError("Database '--cluster create' command failed")
     logger.debug(out)
@@ -81,19 +79,16 @@
 
 def check_cluster_status(
     hosts: t.List[str], ports: t.List[int], trials: int = 10
 ) -> None:  # cov-wlm
     """Check that a Redis/KeyDB cluster is up and running
 
     :param hosts: List of hostnames to connect to
-    :type hosts: List[str]
     :param ports: List of ports for each hostname
-    :type ports: List[int]
     :param trials: number of attempts to verify cluster status
-    :type trials: int, optional
 
     :raises SmartSimError: If cluster status cannot be verified
     """
     cluster_nodes = [
         ClusterNode(get_ip_from_host(host), port)
         for host, port in product(hosts, ports)
     ]
@@ -125,21 +120,17 @@
 def db_is_active(hosts: t.List[str], ports: t.List[int], num_shards: int) -> bool:
     """Check if a DB is running
 
     if the DB is clustered, check cluster status, otherwise
     just ping DB.
 
     :param hosts: list of hosts
-    :type hosts: list[str]
     :param ports: list of ports
-    :type ports: list[int]
     :param num_shards: Number of DB shards
-    :type num_shards: int
     :return: Whether DB is running
-    :rtype: bool
     """
     # if single shard
     if num_shards < 2:
         host = hosts[0]
         port = ports[0]
         try:
             client = redis.Redis(host=host, port=port, db=0)
@@ -206,15 +197,15 @@
                     name=db_script.name, file=str(db_script.file), device=device
                 )
             elif db_script.script:
                 if isinstance(db_script.script, str):
                     client.set_script(
                         name=db_script.name, script=db_script.script, device=device
                     )
-                else:
+                elif callable(db_script.script):
                     client.set_function(
                         name=db_script.name, function=db_script.script, device=device
                     )
             else:
                 raise ValueError(f"No script or file attached to {db_script.name}")
         except RedisReplyError as error:  # pragma: no cover
             logger.error("Error while setting model on orchestrator.")
@@ -225,24 +216,23 @@
     """Send shutdown signal to DB node.
 
     Should only be used in the case where cluster deallocation
     needs to occur manually. Usually, the SmartSim job manager
     will take care of this automatically.
 
     :param host_ip: IP of host to connect to
-    :type hosts: str
     :param ports: Port to which node is listening
-    :type ports: int
     :return: returncode, output, and error of the process
-    :rtype: tuple of (int, str, str)
     """
     redis_cli = CONFIG.database_cli
     cmd = [redis_cli, "-h", host_ip, "-p", str(port), "shutdown"]
     returncode, out, err = execute_cmd(cmd, proc_input="yes", shell=False, timeout=10)
 
     if returncode != 0:
         logger.error(out)
-        logger.error(err)
+        err_msg = "Error while shutting down DB node. "
+        err_msg += f"Return code: {returncode}, err: {err}"
+        logger.error(err_msg)
     elif out:
         logger.debug(out)
 
     return returncode, out, err
```

### Comparing `smartsim-0.6.2/smartsim/_core/utils/serialize.py` & `smartsim-0.7.0/smartsim/_core/utils/serialize.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,18 +29,16 @@
 import json
 import time
 import typing as t
 from pathlib import Path
 
 import smartsim._core._cli.utils as _utils
 import smartsim.log
-from smartsim._core.config import CONFIG
 
 if t.TYPE_CHECKING:
-    from smartsim import Experiment
     from smartsim._core.control.manifest import LaunchedManifest as _Manifest
     from smartsim.database.orchestrator import Orchestrator
     from smartsim.entity import DBNode, Ensemble, Model
     from smartsim.entity.dbobject import DBModel, DBScript
     from smartsim.settings.base import BatchSettings, RunSettings
 
 
@@ -50,17 +48,14 @@
 
 MANIFEST_FILENAME: t.Final[str] = "manifest.json"
 
 _LOGGER = smartsim.log.get_logger(__name__)
 
 
 def save_launch_manifest(manifest: _Manifest[TStepLaunchMetaData]) -> None:
-    if not CONFIG.telemetry_enabled:
-        return
-
     manifest.metadata.run_telemetry_subdirectory.mkdir(parents=True, exist_ok=True)
     exp_out, exp_err = smartsim.log.get_exp_log_paths()
 
     new_run = {
         "run_id": manifest.metadata.run_id,
         "timestamp": int(time.time_ns()),
         "model": [
@@ -78,15 +73,15 @@
     try:
         with open(manifest.metadata.manifest_file_path, "r", encoding="utf-8") as file:
             manifest_dict = json.load(file)
     except (FileNotFoundError, json.JSONDecodeError):
         manifest_dict = {
             "schema info": {
                 "schema_name": "entity manifest",
-                "version": "0.0.3",
+                "version": "0.0.4",
             },
             "experiment": {
                 "name": manifest.metadata.exp_name,
                 "path": manifest.metadata.exp_path,
                 "launcher": manifest.metadata.launcher_name,
                 "out_file": str(exp_out),
                 "err_file": str(exp_err),
@@ -224,24 +219,36 @@
     nodes: t.Sequence[t.Tuple[DBNode, TStepLaunchMetaData]],
 ) -> t.Dict[str, t.Any]:
     db_path = _utils.get_db_path()
     if db_path:
         db_type, _ = db_path.name.split("-", 1)
     else:
         db_type = "Unknown"
+
     return {
         "name": db.name,
         "type": db_type,
         "interface": db._interfaces,  # pylint: disable=protected-access
         "shards": [
             {
                 **shard.to_dict(),
                 "conf_file": shard.cluster_conf_file,
                 "out_file": out_file,
                 "err_file": err_file,
+                "memory_file": (
+                    str(status_dir / "memory.csv") if db.telemetry.is_enabled else ""
+                ),
+                "client_file": (
+                    str(status_dir / "client.csv") if db.telemetry.is_enabled else ""
+                ),
+                "client_count_file": (
+                    str(status_dir / "client_count.csv")
+                    if db.telemetry.is_enabled
+                    else ""
+                ),
                 "telemetry_metadata": {
                     "status_dir": str(status_dir),
                     "step_id": step_id,
                     "task_id": task_id,
                     "managed": managed,
                 },
             }
```

### Comparing `smartsim-0.6.2/smartsim/database/__init__.py` & `smartsim-0.7.0/smartsim/database/__init__.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.6.2/smartsim/database/orchestrator.py` & `smartsim-0.7.0/smartsim/database/orchestrator.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,30 +19,39 @@
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+# pylint: disable=too-many-lines
+
 import itertools
+import os.path as osp
 import sys
 import typing as t
 from os import environ, getcwd, getenv
 from shlex import split as sh_split
 
 import psutil
 from smartredis import Client, ConfigOptions
 from smartredis.error import RedisReplyError
 
 from .._core.config import CONFIG
 from .._core.utils import db_is_active
 from .._core.utils.helpers import is_valid_cmd, unpack_db_identifier
 from .._core.utils.network import get_ip_from_host
-from ..entity import DBNode, EntityList
-from ..error import SmartSimError, SSConfigError, SSUnsupportedError
+from ..entity import DBNode, EntityList, TelemetryConfiguration
+from ..error import (
+    SmartSimError,
+    SSConfigError,
+    SSDBFilesNotParseable,
+    SSUnsupportedError,
+)
 from ..log import get_logger
 from ..servertype import CLUSTERED, STANDALONE
 from ..settings import (
     AprunSettings,
     BsubBatchSettings,
     JsrunSettings,
     MpiexecSettings,
@@ -56,26 +65,27 @@
 from ..settings.base import BatchSettings, RunSettings
 from ..settings.settings import create_batch_settings, create_run_settings
 from ..wlm import detect_launcher
 
 logger = get_logger(__name__)
 
 by_launcher: t.Dict[str, t.List[str]] = {
+    "dragon": [""],
     "slurm": ["srun", "mpirun", "mpiexec"],
     "pbs": ["aprun", "mpirun", "mpiexec"],
     "pals": ["mpiexec"],
     "lsf": ["jsrun"],
     "local": [""],
 }
 
 
 def _detect_command(launcher: str) -> str:
     if launcher in by_launcher:
         for cmd in by_launcher[launcher]:
-            if launcher == "local":
+            if launcher in ["local", "dragon"]:
                 return cmd
             if is_valid_cmd(cmd):
                 return cmd
     msg = (
         "Could not automatically detect a run command to use for launcher "
         f"{launcher}\nSearched for and could not find the following "
         f"commands: {by_launcher[launcher]}"
@@ -101,18 +111,23 @@
             f"Run command {run_command} is not supported on launcher {launcher}\n"
             + "Supported run commands for the given launcher are: "
             + f"{by_launcher[launcher]}"
         )
         raise SmartSimError(msg)
 
 
-def _get_single_command(run_command: str, batch: bool, single_cmd: bool) -> bool:
+def _get_single_command(
+    run_command: str, launcher: str, batch: bool, single_cmd: bool
+) -> bool:
     if not single_cmd:
         return single_cmd
 
+    if launcher == "dragon":
+        return False
+
     if run_command == "srun" and getenv("SLURM_HET_SIZE") is not None:
         msg = (
             "srun can not launch an orchestrator with single_cmd=True in "
             + "a hetereogeneous job. Automatically switching to single_cmd=False."
         )
         logger.info(msg)
         return False
@@ -134,23 +149,25 @@
 def _check_local_constraints(launcher: str, batch: bool) -> None:
     """Check that the local launcher is not launched with invalid batch config"""
     if launcher == "local" and batch:
         msg = "Local orchestrator can not be launched with batch=True"
         raise SmartSimError(msg)
 
 
+# pylint: disable-next=too-many-public-methods
 class Orchestrator(EntityList[DBNode]):
     """The Orchestrator is an in-memory database that can be launched
     alongside entities in SmartSim. Data can be transferred between
     entities by using one of the Python, C, C++ or Fortran clients
     within an entity.
     """
 
     def __init__(
         self,
+        path: t.Optional[str] = getcwd(),
         port: int = 6379,
         interface: t.Union[str, t.List[str]] = "lo",
         launcher: str = "local",
         run_command: str = "auto",
         db_nodes: int = 1,
         batch: bool = False,
         hosts: t.Optional[t.Union[t.List[str], str]] = None,
@@ -161,56 +178,67 @@
         *,
         threads_per_queue: t.Optional[int] = None,
         inter_op_threads: t.Optional[int] = None,
         intra_op_threads: t.Optional[int] = None,
         db_identifier: str = "orchestrator",
         **kwargs: t.Any,
     ) -> None:
-        """Initialize an Orchestrator reference for local launch
-
-        :param port: TCP/IP port, defaults to 6379
-        :type port: int, optional
-        :param interface: network interface(s), defaults to "lo"
-        :type interface: str, list[str], optional
+        """Initialize an ``Orchestrator`` reference for local launch
 
         Extra configurations for RedisAI
 
-        See https://oss.redislabs.com/redisai/configuration/
+        See https://oss.redis.com/redisai/configuration/
 
+        :param path: path to location of ``Orchestrator`` directory
+        :param port: TCP/IP port
+        :param interface: network interface(s)
+        :param launcher: type of launcher being used, options are "slurm", "pbs",
+                         "lsf", or "local". If set to "auto",
+                         an attempt will be made to find an available launcher
+                         on the system.
+        :param run_command: specify launch binary or detect automatically
+        :param db_nodes: number of database shards
+        :param batch: run as a batch workload
+        :param hosts: specify hosts to launch on
+        :param account: account to run batch on
+        :param time: walltime for batch 'HH:MM:SS' format
+        :param alloc: allocation to launch database on
+        :param single_cmd: run all shards with one (MPMD) command
         :param threads_per_queue: threads per GPU device
-        :type threads_per_queue: int, optional
-        :param inter_op_threads: threads accross CPU operations
-        :type inter_op_threads: int, optional
+        :param inter_op_threads: threads across CPU operations
         :param intra_op_threads: threads per CPU operation
-        :type intra_op_threads: int, optional
+        :param db_identifier: an identifier to distinguish this orchestrator in
+            multiple-database experiments
         """
         self.launcher, self.run_command = _autodetect(launcher, run_command)
         _check_run_command(self.launcher, self.run_command)
         _check_local_constraints(self.launcher, batch)
-        single_cmd = _get_single_command(self.run_command, batch, single_cmd)
+        single_cmd = _get_single_command(
+            self.run_command, self.launcher, batch, single_cmd
+        )
         self.ports: t.List[int] = []
         self._hosts: t.List[str] = []
         self._user_hostlist: t.List[str] = []
         if isinstance(interface, str):
             interface = [interface]
         self._interfaces = interface
         self._check_network_interface()
         self.queue_threads = threads_per_queue
         self.inter_threads = inter_op_threads
         self.intra_threads = intra_op_threads
+        self._telemetry_cfg = TelemetryConfiguration()
 
         gpus_per_shard: t.Optional[int] = None
         cpus_per_shard: t.Optional[int] = None
         if self.launcher == "lsf":
             gpus_per_shard = int(kwargs.pop("gpus_per_shard", 0))
             cpus_per_shard = int(kwargs.pop("cpus_per_shard", 4))
-
         super().__init__(
             name=db_identifier,
-            path=getcwd(),
+            path=str(path),
             port=port,
             interface=interface,
             db_nodes=db_nodes,
             batch=batch,
             launcher=self.launcher,
             run_command=self.run_command,
             alloc=alloc,
@@ -261,55 +289,59 @@
             self._fill_reserved()
 
     @property
     def db_identifier(self) -> str:
         """Return the DB identifier, which is common to a DB and all of its nodes
 
         :return: DB identifier
-        :rtype: str
         """
         return self.name
 
     @property
     def num_shards(self) -> int:
-        """Return the number of DB shards contained in the orchestrator.
+        """Return the number of DB shards contained in the Orchestrator.
         This might differ from the number of ``DBNode`` objects, as each
         ``DBNode`` may start more than one shard (e.g. with MPMD).
 
-        :returns: num_shards
-        :rtype: int
+        :returns: the number of DB shards contained in the Orchestrator
         """
         return sum(node.num_shards for node in self.entities)
 
     @property
     def db_nodes(self) -> int:
         """Read only property for the number of nodes an ``Orchestrator`` is
         launched across. Notice that SmartSim currently assumes that each shard
         will be launched on its own node. Therefore this property is currently
         an alias to the ``num_shards`` attribute.
 
         :returns: Number of database nodes
-        :rtype: int
         """
         return self.num_shards
 
     @property
     def hosts(self) -> t.List[str]:
-        """Return the hostnames of orchestrator instance hosts
+        """Return the hostnames of Orchestrator instance hosts
 
         Note that this will only be populated after the orchestrator
         has been launched by SmartSim.
 
-        :return: hostnames
-        :rtype: list[str]
+        :return: the hostnames of Orchestrator instance hosts
         """
         if not self._hosts:
             self._hosts = self._get_db_hosts()
         return self._hosts
 
+    @property
+    def telemetry(self) -> TelemetryConfiguration:
+        """Return the telemetry configuration for this entity.
+
+        :returns: configuration of telemetry for this entity
+        """
+        return self._telemetry_cfg
+
     def reset_hosts(self) -> None:
         """Clear hosts or reset them to last user choice"""
         for node in self.entities:
             node.clear_hosts()
         self._hosts = []
         # This is only needed on LSF
         if self._user_hostlist:
@@ -321,15 +353,14 @@
         for db in self.entities:
             db.remove_stale_dbnode_files()
 
     def get_address(self) -> t.List[str]:
         """Return database addresses
 
         :return: addresses
-        :rtype: list[str]
 
         :raises SmartSimError: If database address cannot be found or is not active
         """
         if not self._hosts:
             raise SmartSimError("Could not find database address")
         if not self.is_active():
             raise SmartSimError("Database is not active")
@@ -341,28 +372,27 @@
             for host, port in itertools.product(self._hosts, self.ports)
         ]
 
     def is_active(self) -> bool:
         """Check if the database is active
 
         :return: True if database is active, False otherwise
-        :rtype: bool
         """
-        if not self._hosts:
+        try:
+            hosts = self.hosts
+        except SSDBFilesNotParseable:
             return False
-
-        return db_is_active(self._hosts, self.ports, self.num_shards)
+        return db_is_active(hosts, self.ports, self.num_shards)
 
     @property
     def _rai_module(self) -> t.Tuple[str, ...]:
         """Get the RedisAI module from third-party installations
 
         :return: Tuple of args to pass to the orchestrator exe
                  to load and configure the RedisAI
-        :rtype: tuple[str]
         """
         module = ["--loadmodule", CONFIG.redisai]
         if self.queue_threads:
             module.extend(("THREADS_PER_QUEUE", str(self.queue_threads)))
         if self.inter_threads:
             module.extend(("INTER_OP_PARALLELISM", str(self.inter_threads)))
         if self.intra_threads:
@@ -373,22 +403,29 @@
     def _redis_exe(self) -> str:
         return CONFIG.database_exe
 
     @property
     def _redis_conf(self) -> str:
         return CONFIG.database_conf
 
+    @property
+    def checkpoint_file(self) -> str:
+        """Get the path to the checkpoint file for this Orchestrator
+
+        :return: Path to the checkpoint file if it exists, otherwise a None
+        """
+        return osp.join(self.path, "smartsim_db.dat")
+
     def set_cpus(self, num_cpus: int) -> None:
         """Set the number of CPUs available to each database shard
 
         This effectively will determine how many cpus can be used for
         compute threads, background threads, and network I/O.
 
         :param num_cpus: number of cpus to set
-        :type num_cpus: int
         """
         if self.batch:
             if self.launcher == "pbs":
                 if hasattr(self, "batch_settings") and self.batch_settings:
                     if hasattr(self.batch_settings, "set_ncpus"):
                         self.batch_settings.set_ncpus(num_cpus)
             if self.launcher == "slurm":
@@ -404,41 +441,38 @@
 
     def set_walltime(self, walltime: str) -> None:
         """Set the batch walltime of the orchestrator
 
         Note: This will only effect orchestrators launched as a batch
 
         :param walltime: amount of time e.g. 10 hours is 10:00:00
-        :type walltime: str
         :raises SmartSimError: if orchestrator isn't launching as batch
         """
         if not self.batch:
             raise SmartSimError("Not running as batch, cannot set walltime")
 
         if hasattr(self, "batch_settings") and self.batch_settings:
             self.batch_settings.set_walltime(walltime)
 
     def set_hosts(self, host_list: t.Union[t.List[str], str]) -> None:
         """Specify the hosts for the ``Orchestrator`` to launch on
 
         :param host_list: list of host (compute node names)
-        :type host_list: str, list[str]
         :raises TypeError: if wrong type
         """
         if isinstance(host_list, str):
             host_list = [host_list.strip()]
         if not isinstance(host_list, list):
             raise TypeError("host_list argument must be a list of strings")
         if not all(isinstance(host, str) for host in host_list):
             raise TypeError("host_list argument must be list of strings")
         self._user_hostlist = host_list.copy()
         # TODO check length
-        if self.batch:
-            if hasattr(self, "batch_settings") and self.batch_settings:
-                self.batch_settings.set_hostlist(host_list)
+        if self.batch and hasattr(self, "batch_settings") and self.batch_settings:
+            self.batch_settings.set_hostlist(host_list)
 
         if self.launcher == "lsf":
             for db in self.entities:
                 db.set_hosts(host_list)
         elif (
             self.launcher == "pals"
             and isinstance(self.entities[0].run_settings, PalsMpiexecSettings)
@@ -461,43 +495,38 @@
     def set_batch_arg(self, arg: str, value: t.Optional[str] = None) -> None:
         """Set a batch argument the orchestrator should launch with
 
         Some commonly used arguments such as --job-name are used
         by SmartSim and will not be allowed to be set.
 
         :param arg: batch argument to set e.g. "exclusive"
-        :type arg: str
         :param value: batch param - set to None if no param value
-        :type value: str | None
         :raises SmartSimError: if orchestrator not launching as batch
         """
         if not hasattr(self, "batch_settings") or not self.batch_settings:
             raise SmartSimError("Not running as batch, cannot set batch_arg")
 
         if arg in self._reserved_batch_args[type(self.batch_settings)]:
             logger.warning(
                 f"Can not set batch argument {arg}: "
                 "it is a reserved keyword in Orchestrator"
             )
         else:
-            if hasattr(self, "batch_settings") and self.batch_settings:
-                self.batch_settings.batch_args[arg] = value
+            self.batch_settings.batch_args[arg] = value
 
     def set_run_arg(self, arg: str, value: t.Optional[str] = None) -> None:
         """Set a run argument the orchestrator should launch
         each node with (it will be passed to `jrun`)
 
         Some commonly used arguments are used
         by SmartSim and will not be allowed to be set.
         For example, "n", "N", etc.
 
         :param arg: run argument to set
-        :type arg: str
         :param value: run parameter - set to None if no parameter value
-        :type value: str | None
         """
         if arg in self._reserved_run_args[type(self.entities[0].run_settings)]:
             logger.warning(
                 f"Can not set batch argument {arg}: "
                 "it is a reserved keyword in Orchestrator"
             )
         else:
@@ -510,83 +539,77 @@
     def enable_checkpoints(self, frequency: int) -> None:
         """Sets the database's save configuration to save the DB every 'frequency'
         seconds given that at least one write operation against the DB occurred in
         that time. E.g., if `frequency` is 900, then the database will save to disk
         after 900 seconds if there is at least 1 change to the dataset.
 
         :param frequency: the given number of seconds before the DB saves
-        :type frequency: int
         """
         self.set_db_conf("save", f"{frequency} 1")
 
     def set_max_memory(self, mem: str) -> None:
         """Sets the max memory configuration. By default there is no memory limit.
         Setting max memory to zero also results in no memory limit. Once a limit is
         surpassed, keys will be removed according to the eviction strategy. The
         specified memory size is case insensitive and supports the typical forms of:
-        1k => 1000 bytes
-        1kb => 1024 bytes
-        1m => 1000000 bytes
-        1mb => 1024*1024 bytes
-        1g => 1000000000 bytes
+
+        1k => 1000 bytes \n
+        1kb => 1024 bytes \n
+        1m => 1000000 bytes \n
+        1mb => 1024*1024 bytes \n
+        1g => 1000000000 bytes \n
         1gb => 1024*1024*1024 bytes
 
         :param mem: the desired max memory size e.g. 3gb
-        :type mem: str
         :raises SmartSimError: If 'mem' is an invalid memory value
         :raises SmartSimError: If database is not active
         """
         self.set_db_conf("maxmemory", mem)
 
     def set_eviction_strategy(self, strategy: str) -> None:
         """Sets how the database will select what to remove when
         'maxmemory' is reached. The default is noeviction.
 
         :param strategy: The max memory policy to use
             e.g. "volatile-lru", "allkeys-lru", etc.
-        :type strategy: str
         :raises SmartSimError: If 'strategy' is an invalid maxmemory policy
         :raises SmartSimError: If database is not active
         """
         self.set_db_conf("maxmemory-policy", strategy)
 
     def set_max_clients(self, clients: int = 50_000) -> None:
         """Sets the max number of connected clients at the same time.
         When the number of DB shards contained in the orchestrator is
         more than two, then every node will use two connections, one
         incoming and another outgoing.
 
         :param clients: the maximum number of connected clients
-        :type clients: int, optional
         """
         self.set_db_conf("maxclients", str(clients))
 
     def set_max_message_size(self, size: int = 1_073_741_824) -> None:
         """Sets the database's memory size limit for bulk requests,
         which are elements representing single strings. The default
         is 1 gigabyte. Message size must be greater than or equal to 1mb.
         The specified memory size should be an integer that represents
         the number of bytes. For example, to set the max message size
         to 1gb, use 1024*1024*1024.
 
         :param size: maximum message size in bytes
-        :type size: int, optional
         """
         self.set_db_conf("proto-max-bulk-len", str(size))
 
     def set_db_conf(self, key: str, value: str) -> None:
         """Set any valid configuration at runtime without the need
         to restart the database. All configuration parameters
         that are set are immediately loaded by the database and
         will take effect starting with the next command executed.
 
         :param key: the configuration parameter
-        :type key: str
         :param value: the database configuration parameter's new value
-        :type value: str
         """
         if self.is_active():
             addresses = []
             for host in self.hosts:
                 for port in self.ports:
                     addresses.append(":".join([get_ip_from_host(host), str(port)]))
 
@@ -843,14 +866,15 @@
             *self._rai_module,
             f"+name={name}",  # name of node
             f"+port={port}",  # redis port
             f"+ifname={','.join(self._interfaces)}",  # pass interface to start script
         ]
         if cluster:
             cmd.append("+cluster")  # is the shard part of a cluster
+
         return cmd
 
     def _get_db_hosts(self) -> t.List[str]:
         hosts = []
         for db in self.entities:
             if not db.is_mpmd:
                 hosts.append(db.host)
```

### Comparing `smartsim-0.6.2/smartsim/entity/__init__.py` & `smartsim-0.7.0/smartsim/entity/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,11 +23,11 @@
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from .dbnode import DBNode
 from .dbobject import *
 from .ensemble import Ensemble
-from .entity import SmartSimEntity
+from .entity import SmartSimEntity, TelemetryConfiguration
 from .entityList import EntityList, EntitySequence
 from .files import TaggedFilesHierarchy
 from .model import Model
```

### Comparing `smartsim-0.6.2/smartsim/entity/dbnode.py` & `smartsim-0.7.0/smartsim/entity/dbnode.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 import os
 import os.path as osp
 import time
 import typing as t
 from dataclasses import dataclass
 
 from .._core.config import CONFIG
-from ..error import SmartSimError
+from ..error import SSDBFilesNotParseable
 from ..log import get_logger
 from ..settings.base import RunSettings
 from .entity import SmartSimEntity
 
 logger = get_logger(__name__)
 
 
@@ -142,17 +142,15 @@
 
     def _get_cluster_conf_filenames(self, port: int) -> t.List[str]:  # cov-lsf
         """Returns the .conf file name for the given port number
 
         This function should bu used if and only if ``_mpmd==True``
 
         :param port: port number
-        :type port: int
         :return: the dbnode configuration file name
-        :rtype: str
         """
         if self.num_shards == 1:
             return [f"nodes-{self.name}-{port}.conf"]
         return [
             f"nodes-{self.name}_{shard_id}-{port}.conf"
             for shard_id in range(self.num_shards)
         ]
@@ -182,17 +180,16 @@
     ) -> "t.List[LaunchedShardData]":
         with fileinput.FileInput(file_paths) as ifstream:
             return cls._parse_launched_shard_info_from_iterable(ifstream, num_shards)
 
     def get_launched_shard_info(self) -> "t.List[LaunchedShardData]":
         """Parse the launched database shard info from the output files
 
-        :raises SmartSimError: if all shard info could not be found
+        :raises SSDBFilesNotParseable: if all shard info could not be found
         :return: The found launched shard info
-        :rtype: list[LaunchedShardData]
         """
         ips: "t.List[LaunchedShardData]" = []
         trials = CONFIG.database_file_parse_trials
         interval = CONFIG.database_file_parse_interval
         output_files = [osp.join(self.path, file) for file in self._output_files]
 
         while len(ips) < self.num_shards and trials > 0:
@@ -210,26 +207,25 @@
         if len(ips) < self.num_shards:
             msg = (
                 f"Failed to parse the launched DB shard information from file(s) "
                 f"{', '.join(output_files)}. Found the information for "
                 f"{len(ips)} out of {self.num_shards} DB shards."
             )
             logger.error(msg)
-            raise SmartSimError(msg)
+            raise SSDBFilesNotParseable(msg)
         return ips
 
     def _parse_db_hosts(self) -> t.List[str]:
         """Parse the database hosts/IPs from the output files
 
         The IP address is preferred, but if hostname is only present
         then a lookup to /etc/hosts is done through the socket library.
 
-        :raises SmartSimError: if host/ip could not be found
+        :raises SSDBFilesNotParseable: if host/ip could not be found
         :return: ip addresses | hostnames
-        :rtype: list[str]
         """
         return list({shard.hostname for shard in self.get_launched_shard_info()})
 
 
 @dataclass(frozen=True)
 class LaunchedShardData:
     """Data class to write and parse data about a launched database shard"""
```

### Comparing `smartsim-0.6.2/smartsim/entity/dbobject.py` & `smartsim-0.7.0/smartsim/entity/dbobject.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import typing as t
 from pathlib import Path
 
-from .._core.utils import init_default
+from .._core._install.builder import Device
 from ..error import SSUnsupportedError
 
 __all__ = ["DBObject", "DBModel", "DBScript"]
 
 
 _DBObjectFuncT = t.TypeVar("_DBObjectFuncT", str, bytes)
 
@@ -42,15 +42,15 @@
     """
 
     def __init__(
         self,
         name: str,
         func: t.Optional[_DBObjectFuncT],
         file_path: t.Optional[str],
-        device: t.Literal["CPU", "GPU"],
+        device: str,
         devices_per_node: int,
         first_device: int,
     ) -> None:
         self.name = name
         self.func: t.Optional[_DBObjectFuncT] = func
         self.file: t.Optional[Path] = (
             None  # Need to have this explicitly to check on it
@@ -71,17 +71,14 @@
         return not self.func
 
     @staticmethod
     def _check_tensor_args(
         inputs: t.Union[str, t.Optional[t.List[str]]],
         outputs: t.Union[str, t.Optional[t.List[str]]],
     ) -> t.Tuple[t.List[str], t.List[str]]:
-        inputs = init_default([], inputs, (list, str))
-        outputs = init_default([], outputs, (list, str))
-
         if isinstance(inputs, str):
             inputs = [inputs]
         if isinstance(outputs, str):
             outputs = [outputs]
         return inputs or [], outputs or []
 
     @staticmethod
@@ -99,51 +96,49 @@
     def _check_filepath(file: str) -> Path:
         file_path = Path(file).resolve()
         if not file_path.is_file():
             raise FileNotFoundError(file_path)
         return file_path
 
     @staticmethod
-    def _check_device(device: t.Literal["CPU", "GPU"]) -> str:
-        device = t.cast(t.Literal["CPU", "GPU"], device.upper())
-        if not device.startswith("CPU") and not device.startswith("GPU"):
+    def _check_device(device: str) -> str:
+        valid_devices = [Device.CPU.value, Device.GPU.value]
+        if not any(device.lower().startswith(dev) for dev in valid_devices):
             raise ValueError("Device argument must start with either CPU or GPU")
         return device
 
     def _enumerate_devices(self) -> t.List[str]:
         """Enumerate devices for a DBObject
 
         :param dbobject: DBObject to enumerate
-        :type dbobject: DBObject
         :return: list of device names
-        :rtype: list[str]
         """
 
         if self.device == "GPU" and self.devices_per_node > 1:
             return [
                 f"{self.device}:{device_num}"
                 for device_num in range(
                     self.first_device, self.first_device + self.devices_per_node
                 )
             ]
 
         return [self.device]
 
     @staticmethod
     def _check_devices(
-        device: t.Literal["CPU", "GPU"],
+        device: str,
         devices_per_node: int,
         first_device: int,
     ) -> None:
-        if device == "CPU" and devices_per_node > 1:
+        if device.lower() == Device.CPU.value and devices_per_node > 1:
             raise SSUnsupportedError(
                 "Cannot set devices_per_node>1 if CPU is specified under devices"
             )
 
-        if device == "CPU" and first_device > 0:
+        if device.lower() == Device.CPU.value and first_device > 0:
             raise SSUnsupportedError(
                 "Cannot set first_device>0 if CPU is specified under devices"
             )
 
         if devices_per_node == 1:
             return
 
@@ -156,15 +151,15 @@
 
 class DBScript(DBObject[str]):
     def __init__(
         self,
         name: str,
         script: t.Optional[str] = None,
         script_path: t.Optional[str] = None,
-        device: t.Literal["CPU", "GPU"] = "CPU",
+        device: str = Device.CPU.value.upper(),
         devices_per_node: int = 1,
         first_device: int = 0,
     ):
         """TorchScript code represenation
 
         Device selection is either "GPU" or "CPU". If many devices are
         present, a number can be passed for specification e.g. "GPU:1".
@@ -174,40 +169,34 @@
         additionally setting ``first_device=M`` will instead result in the
         script being stored on devices M through M + N -1.
 
         One of either script (in memory representation) or script_path (file)
         must be provided
 
         :param name: key to store script under
-        :type name: str
         :param script: TorchScript code
-        :type script: str, optional
-        :param script_path: path to TorchScript code, defaults to None
-        :type script_path: str, optional
-        :param device: device for script execution, defaults to "CPU"
-        :type device: str, optional
+        :param script_path: path to TorchScript code
+        :param device: device for script execution
         :param devices_per_node: number of devices to store the script on
-        :type devices_per_node: int
         :param first_device: first devices to store the script on
-        :type first_device: int
         """
         super().__init__(
             name, script, script_path, device, devices_per_node, first_device
         )
         if not script and not script_path:
             raise ValueError("Either script or script_path must be provided")
 
     @property
-    def script(self) -> t.Optional[str]:
+    def script(self) -> t.Optional[t.Union[bytes, str]]:
         return self.func
 
     def __str__(self) -> str:
         desc_str = "Name: " + self.name + "\n"
         if self.func:
-            desc_str += "Func: " + self.func + "\n"
+            desc_str += "Func: " + str(self.func) + "\n"
         if self.file:
             desc_str += "File path: " + str(self.file) + "\n"
         devices_str = self.device + (
             "s per node\n" if self.devices_per_node > 1 else " per node\n"
         )
         desc_str += "Devices: " + str(self.devices_per_node) + " " + devices_str
         if self.first_device > 0:
@@ -218,15 +207,15 @@
 class DBModel(DBObject[bytes]):
     def __init__(
         self,
         name: str,
         backend: str,
         model: t.Optional[bytes] = None,
         model_file: t.Optional[str] = None,
-        device: t.Literal["CPU", "GPU"] = "CPU",
+        device: str = Device.CPU.value.upper(),
         devices_per_node: int = 1,
         first_device: int = 0,
         batch_size: int = 0,
         min_batch_size: int = 0,
         min_batch_timeout: int = 0,
         tag: str = "",
         inputs: t.Optional[t.List[str]] = None,
@@ -234,39 +223,26 @@
     ) -> None:
         """A TF, TF-lite, PT, or ONNX model to load into the DB at runtime
 
         One of either model (in memory representation) or model_path (file)
         must be provided
 
         :param name: key to store model under
-        :type name: str
         :param model: model in memory
-        :type model: str, optional
         :param model_file: serialized model
-        :type model_file: file path to model, optional
         :param backend: name of the backend (TORCH, TF, TFLITE, ONNX)
-        :type backend: str
-        :param device: name of device for execution, defaults to "CPU"
-        :type device: str, optional
+        :param device: name of device for execution
         :param devices_per_node: number of devices to store the model on
-        :type devices_per_node: int
         :param first_device: The first device to store the model on
-        :type first_device: int
-        :param batch_size: batch size for execution, defaults to 0
-        :type batch_size: int, optional
-        :param min_batch_size: minimum batch size for model execution, defaults to 0
-        :type min_batch_size: int, optional
-        :param min_batch_timeout: time to wait for minimum batch size, defaults to 0
-        :type min_batch_timeout: int, optional
-        :param tag: additional tag for model information, defaults to ""
-        :type tag: str, optional
-        :param inputs: model inputs (TF only), defaults to None
-        :type inputs: list[str], optional
-        :param outputs: model outupts (TF only), defaults to None
-        :type outputs: list[str], optional
+        :param batch_size: batch size for execution
+        :param min_batch_size: minimum batch size for model execution
+        :param min_batch_timeout: time to wait for minimum batch size
+        :param tag: additional tag for model information
+        :param inputs: model inputs (TF only)
+        :param outputs: model outupts (TF only)
         """
         super().__init__(
             name, model, model_file, device, devices_per_node, first_device
         )
         self.backend = self._check_backend(backend)
         if not model and not model_file:
             raise ValueError("Either model or model_file must be provided")
```

### Comparing `smartsim-0.6.2/smartsim/entity/entityList.py` & `smartsim-0.7.0/smartsim/entity/entityList.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,24 +87,22 @@
     @property
     def db_scripts(self) -> t.Iterable["smartsim.entity.DBScript"]:
         """Return an immutable collection of attached scripts"""
         return (script for script in self._db_scripts)
 
     @property
     def batch(self) -> bool:
-        try:
-            if not hasattr(self, "batch_settings"):
-                return False
+        """Property indicating whether or not the entity sequence should be
+        launched as a batch job
 
-            if self.batch_settings:
-                return True
-            return False
-        # local orchestrator cannot launch with batches
-        except AttributeError:
-            return False
+        :return: ``True`` if entity sequence should be launched as a batch job,
+                 ``False`` if the members will be launched individually.
+        """
+        # pylint: disable-next=no-member
+        return hasattr(self, "batch_settings") and self.batch_settings
 
     @property
     def type(self) -> str:
         """Return the name of the class"""
         return type(self).__name__
 
     def set_path(self, new_path: str) -> None:
```

### Comparing `smartsim-0.6.2/smartsim/entity/files.py` & `smartsim-0.7.0/smartsim/entity/files.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,21 +54,18 @@
         tagged: t.Optional[t.List[str]] = None,
         copy: t.Optional[t.List[str]] = None,
         symlink: t.Optional[t.List[str]] = None,
     ) -> None:
         """Initialize an EntityFiles instance
 
         :param tagged: tagged files for model configuration
-        :type tagged: list of str
         :param copy: files or directories to copy into model
                      or node directories
-        :type copy: list of str
         :param symlink: files to symlink into model or node
                         directories
-        :type symlink: list of str
         """
         self.tagged = tagged or []
         self.copy = copy or []
         self.link = symlink or []
         self.tagged_hierarchy = None
         self._check_files()
 
@@ -98,20 +95,17 @@
     @staticmethod
     def _type_check_files(
         file_list: t.Union[t.List[str], None], file_type: str
     ) -> t.List[str]:
         """Check the type of the files provided by the user.
 
         :param file_list: either tagged, copy, or symlink files
-        :type file_list: list of str
         :param file_type: name of the file type e.g. "tagged"
-        :type file_type: str
         :raises TypeError: if incorrect type is provided by user
         :return: file list provided
-        :rtype: list of str
         """
         if file_list:
             if not isinstance(file_list, list):
                 if isinstance(file_list, str):
                     file_list = [file_list]
                 else:
                     raise TypeError(
@@ -124,18 +118,16 @@
 
     @staticmethod
     def _check_path(file_path: str) -> str:
         """Given a user provided path-like str, find the actual path to
            the directory or file and create a full path.
 
         :param file_path: path to a specific file or directory
-        :type file_path: str
         :raises FileNotFoundError: if file or directory does not exist
         :return: full path to file or directory
-        :rtype: str
         """
         full_path = path.abspath(file_path)
         if path.isfile(full_path):
             return full_path
         if path.isdir(full_path):
             return full_path
         raise FileNotFoundError(f"File or Directory {file_path} not found")
@@ -179,20 +171,18 @@
 
     def __init__(self, parent: t.Optional[t.Any] = None, subdir_name: str = "") -> None:
         """Initialize a TaggedFilesHierarchy
 
         :param parent: The parent hierarchy of the new hierarchy,
                        must be None if creating a root hierarchy,
                        must be provided if creating a subhierachy
-        :type parent: TaggedFilesHierarchy | None, optional
         :param subdir_name: Name of subdirectory representd by the new hierarchy,
                             must be "" if creating a root hierarchy,
                             must be any valid dir name if subhierarchy,
                             invalid names are ".", ".." or contain path seperators
-        :type subdir_name: str, optional
         :raises ValueError: if given a subdir_name without a parent,
                             if given a parent without a subdir_name,
                             or if the subdir_name is invalid
         """
         if parent is None and subdir_name:
             raise ValueError(
                 "TaggedFilesHierarchies should not have a subdirectory name without a"
@@ -228,23 +218,20 @@
         """Given a list of absolute paths to files and dirs, create and return
         a TaggedFilesHierarchy instance representing the file hierarchy of
         tagged files. All files in the path list will be placed in the base of
         the file hierarchy.
 
         :param path_list: list of absolute paths to tagged files or dirs
                           containing tagged files
-        :type path_list: list[str]
         :param dir_contents_to_base: When a top level dir is encountered, if
                                      this value is truthy, files in the dir are
                                      put into the base hierarchy level.
                                      Otherwise, a new sub level is created for
                                      the dir
-        :type dir_contents_to_base: bool
         :return: A built tagged file hierarchy for the given files
-        :rtype: TaggedFilesHierarchy
         """
         tagged_file_hierarchy = cls()
         if dir_contents_to_base:
             new_paths = []
             for tagged_path in path_list:
                 if os.path.isdir(tagged_path):
                     new_paths += [
@@ -257,39 +244,36 @@
         tagged_file_hierarchy._add_paths(path_list)
         return tagged_file_hierarchy
 
     def _add_file(self, file: str) -> None:
         """Add a file to the current level in the file hierarchy
 
         :param file: absoute path to a file to add to the hierarchy
-        :type file: str
         """
         self.files.add(file)
 
     def _add_dir(self, dir_path: str) -> None:
         """Add a dir contianing tagged files by creating a new sub level in the
         tagged file hierarchy. All paths within the directroy are added to the
         the new level sub level tagged file hierarchy
 
         :param dir: absoute path to a dir to add to the hierarchy
-        :type dir: str
         """
         tagged_file_hierarchy = TaggedFilesHierarchy(self, path.basename(dir_path))
         # pylint: disable-next=protected-access
         tagged_file_hierarchy._add_paths(
             [path.join(dir_path, file) for file in os.listdir(dir_path)]
         )
 
     def _add_paths(self, paths: t.List[str]) -> None:
         """Takes a list of paths and iterates over it, determining if each
         path is to a file or a dir and then appropriatly adding it to the
         TaggedFilesHierarchy.
 
         :param paths: list of paths to files or dirs to add to the hierarchy
-        :type paths: list[str]
         :raises ValueError: if link to dir is found
         :raises FileNotFoundError: if path does not exist
         """
         for candidate in paths:
             candidate = os.path.abspath(candidate)
             if os.path.isdir(candidate):
                 if os.path.islink(candidate):
```

### Comparing `smartsim-0.6.2/smartsim/entity/model.py` & `smartsim-0.7.0/smartsim/entity/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,22 +22,24 @@
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from __future__ import annotations
 
-import collections.abc
+import itertools
 import re
 import sys
 import typing as t
 import warnings
+from os import getcwd
 from os import path as osp
 
-from .._core.utils.helpers import cat_arg_and_value, init_default
+from .._core._install.builder import Device
+from .._core.utils.helpers import cat_arg_and_value
 from ..error import EntityExistsError, SSUnsupportedError
 from ..log import get_logger
 from ..settings.base import BatchSettings, RunSettings
 from .dbobject import DBModel, DBScript
 from .entity import SmartSimEntity
 from .files import EntityFiles
 
@@ -45,72 +47,74 @@
 
 
 class Model(SmartSimEntity):
     def __init__(
         self,
         name: str,
         params: t.Dict[str, str],
-        path: str,
         run_settings: RunSettings,
+        path: t.Optional[str] = getcwd(),
         params_as_args: t.Optional[t.List[str]] = None,
         batch_settings: t.Optional[BatchSettings] = None,
     ):
         """Initialize a ``Model``
 
         :param name: name of the model
-        :type name: str
         :param params: model parameters for writing into configuration files or
                        to be passed as command line arguments to executable.
-        :type params: dict
         :param path: path to output, error, and configuration files
-        :type path: str
         :param run_settings: launcher settings specified in the experiment
-        :type run_settings: RunSettings
         :param params_as_args: list of parameters which have to be
                                interpreted as command line arguments to
                                be added to run_settings
-        :type params_as_args: list[str]
         :param batch_settings: Launcher settings for running the individual
-                               model as a batch job, defaults to None
-        :type batch_settings: BatchSettings | None
+                               model as a batch job
         """
-        super().__init__(name, path, run_settings)
+        super().__init__(name, str(path), run_settings)
         self.params = params
         self.params_as_args = params_as_args
         self.incoming_entities: t.List[SmartSimEntity] = []
         self._key_prefixing_enabled = False
         self.batch_settings = batch_settings
         self._db_models: t.List[DBModel] = []
         self._db_scripts: t.List[DBScript] = []
         self.files: t.Optional[EntityFiles] = None
 
     @property
     def db_models(self) -> t.Iterable[DBModel]:
-        """Return an immutable collection of attached models"""
+        """Retrieve an immutable collection of attached models
+
+        :return: Return an immutable collection of attached models
+        """
         return (model for model in self._db_models)
 
     @property
     def db_scripts(self) -> t.Iterable[DBScript]:
-        """Return an immutable collection attached of scripts"""
+        """Retrieve an immutable collection attached of scripts
+
+        :return: Return an immutable collection of attached scripts
+        """
         return (script for script in self._db_scripts)
 
     @property
     def colocated(self) -> bool:
-        """Return True if this Model will run with a colocated Orchestrator"""
+        """Return True if this Model will run with a colocated Orchestrator
+
+        :return: Return True of the Model will run with a colocated Orchestrator
+        """
         return bool(self.run_settings.colocated_db_settings)
 
     def register_incoming_entity(self, incoming_entity: SmartSimEntity) -> None:
         """Register future communication between entities.
 
         Registers the named data sources that this entity
         has access to by storing the key_prefix associated
         with that entity
 
         :param incoming_entity: The entity that data will be received from
-        :type incoming_entity: SmartSimEntity
         :raises SmartSimError: if incoming entity has already been registered
         """
         if incoming_entity.name in [
             in_entity.name for in_entity in self.incoming_entities
         ]:
             raise EntityExistsError(
                 f"'{incoming_entity.name}' has already "
@@ -124,15 +128,18 @@
         self._key_prefixing_enabled = True
 
     def disable_key_prefixing(self) -> None:
         """If called, the entity will not prefix its keys with its own model name"""
         self._key_prefixing_enabled = False
 
     def query_key_prefixing(self) -> bool:
-        """Inquire as to whether this entity will prefix its keys with its name"""
+        """Inquire as to whether this entity will prefix its keys with its name
+
+        :return: Return True if entity will prefix its keys with its name
+        """
         return self._key_prefixing_enabled
 
     def attach_generator_files(
         self,
         to_copy: t.Optional[t.List[str]] = None,
         to_symlink: t.Optional[t.List[str]] = None,
         to_configure: t.Optional[t.List[str]] = None,
@@ -151,24 +158,21 @@
         Files "to_configure" are text based model input files where
         parameters for the model are set. Note that only models
         support the "to_configure" field. These files must have
         fields tagged that correspond to the values the user
         would like to change. The tag is settable but defaults
         to a semicolon e.g. THERMO = ;10;
 
-        :param to_copy: files to copy, defaults to []
-        :type to_copy: list, optional
-        :param to_symlink: files to symlink, defaults to []
-        :type to_symlink: list, optional
-        :param to_configure: input files with tagged parameters, defaults to []
-        :type to_configure: list, optional
-        """
-        to_copy = init_default([], to_copy, (list, str))
-        to_symlink = init_default([], to_symlink, (list, str))
-        to_configure = init_default([], to_configure, (list, str))
+        :param to_copy: files to copy
+        :param to_symlink: files to symlink
+        :param to_configure: input files with tagged parameters
+        """
+        to_copy = to_copy or []
+        to_symlink = to_symlink or []
+        to_configure = to_configure or []
 
         # Check that no file collides with the parameter file written
         # by Generator. We check the basename, even though it is more
         # restrictive than what we need (but it avoids relative path issues)
         for strategy in [to_copy, to_symlink, to_configure]:
             if strategy is not None and any(
                 osp.basename(filename) == "smartsim_params.txt" for filename in strategy
@@ -181,15 +185,14 @@
         self.files = EntityFiles(to_configure, to_copy, to_symlink)
 
     @property
     def attached_files_table(self) -> str:
         """Return a list of attached files as a plain text table
 
         :returns: String version of table
-        :rtype: str
         """
         if not self.files:
             return "No file attached to this model."
         return str(self.files)
 
     def print_attached_files(self) -> None:
         """Print a table of the attached files on std out"""
@@ -235,26 +238,20 @@
                 "intra_op_threads": 1,
                 "server_threads": 2 # keydb only
             }
 
         Generally these don't need to be changed.
 
         :param unix_socket: path to where the socket file will be created
-        :type unix_socket: str, optional
         :param socket_permissions: permissions for the socketfile
-        :type socket_permissions: int, optional
-        :param db_cpus: number of cpus to use for orchestrator, defaults to 1
-        :type db_cpus: int, optional
+        :param db_cpus: number of cpus to use for orchestrator
         :param custom_pinning: CPUs to pin the orchestrator to. Passing an empty
                                iterable disables pinning
-        :type custom_pinning: iterable of ints or iterable of ints, optional
         :param debug: launch Model with extra debug information about the colocated db
-        :type debug: bool, optional
         :param kwargs: additional keyword arguments to pass to the orchestrator database
-        :type kwargs: dict, optional
         """
 
         if not re.match(r"^[a-zA-Z0-9.:\,_\-/]*$", unix_socket):
             raise ValueError(
                 f"Invalid name for unix socket: {unix_socket}. Must only "
                 "contain alphanumeric characters or . : _ - /"
             )
@@ -301,28 +298,21 @@
                 inter_op_threads: 1,
                 intra_op_threads: 1,
                 server_threads: 2 # keydb only
             }
 
         Generally these don't need to be changed.
 
-        :param port: port to use for orchestrator database, defaults to 6379
-        :type port: int, optional
-        :param ifname: interface to use for orchestrator, defaults to "lo"
-        :type ifname: str | list[str], optional
-        :param db_cpus: number of cpus to use for orchestrator, defaults to 1
-        :type db_cpus: int, optional
+        :param port: port to use for orchestrator database
+        :param ifname: interface to use for orchestrator
+        :param db_cpus: number of cpus to use for orchestrator
         :param custom_pinning: CPUs to pin the orchestrator to. Passing an empty
                                iterable disables pinning
-        :type custom_pinning: iterable of ints or iterable of ints, optional
         :param debug: launch Model with extra debug information about the colocated db
-        :type debug: bool, optional
         :param kwargs: additional keyword arguments to pass to the orchestrator database
-        :type kwargs: dict, optional
-
         """
 
         tcp_options = {"port": port, "ifname": ifname}
         common_options = {
             "cpus": db_cpus,
             "custom_pinning": custom_pinning,
             "debug": debug,
@@ -410,62 +400,57 @@
 
         self.run_settings.colocated_db_settings = colo_db_config
 
     @staticmethod
     def _create_pinning_string(
         pin_ids: t.Optional[t.Iterable[t.Union[int, t.Iterable[int]]]], cpus: int
     ) -> t.Optional[str]:
-        """Create a comma-separated string CPU ids. By default, None returns
-        0,1,...,cpus-1; an empty iterable will disable pinning altogether,
-        and an iterable constructs a comma separate string (e.g. 0,2,5)
+        """Create a comma-separated string of CPU ids. By default, ``None``
+        returns 0,1,...,cpus-1; an empty iterable will disable pinning
+        altogether, and an iterable constructs a comma separated string of
+        integers (e.g. ``[0, 2, 5]`` -> ``"0,2,5"``)
         """
 
         def _stringify_id(_id: int) -> str:
             """Return the cPU id as a string if an int, otherwise raise a ValueError"""
             if isinstance(_id, int):
                 if _id < 0:
                     raise ValueError("CPU id must be a nonnegative number")
                 return str(_id)
 
             raise TypeError(f"Argument is of type '{type(_id)}' not 'int'")
 
-        _invalid_input_message = (
-            "Expected a cpu pinning specification of type iterable of ints or "
-            f"iterables of ints. Instead got type `{type(pin_ids)}`"
-        )
+        try:
+            pin_ids = tuple(pin_ids) if pin_ids is not None else None
+        except TypeError:
+            raise TypeError(
+                "Expected a cpu pinning specification of type iterable of ints or "
+                f"iterables of ints. Instead got type `{type(pin_ids)}`"
+            ) from None
 
         # Deal with MacOSX limitations first. The "None" (default) disables pinning
-        # and is equivalent to []. The only invalid option is an iterable
+        # and is equivalent to []. The only invalid option is a non-empty pinning
         if sys.platform == "darwin":
-            if pin_ids is None or not pin_ids:
-                return None
-
-            if isinstance(pin_ids, collections.abc.Iterable):
+            if pin_ids:
                 warnings.warn(
                     "CPU pinning is not supported on MacOSX. Ignoring pinning "
                     "specification.",
                     RuntimeWarning,
                 )
-                return None
-            raise TypeError(_invalid_input_message)
+            return None
+
         # Flatten the iterable into a list and check to make sure that the resulting
         # elements are all ints
         if pin_ids is None:
             return ",".join(_stringify_id(i) for i in range(cpus))
         if not pin_ids:
             return None
-        if isinstance(pin_ids, collections.abc.Iterable):
-            pin_list = []
-            for pin_id in pin_ids:
-                if isinstance(pin_id, collections.abc.Iterable):
-                    pin_list.extend([_stringify_id(j) for j in pin_id])
-                else:
-                    pin_list.append(_stringify_id(pin_id))
-            return ",".join(sorted(set(pin_list)))
-        raise TypeError(_invalid_input_message)
+        pin_ids = ((x,) if isinstance(x, int) else x for x in pin_ids)
+        to_fmt = itertools.chain.from_iterable(pin_ids)
+        return ",".join(sorted({_stringify_id(x) for x in to_fmt}))
 
     def params_to_args(self) -> None:
         """Convert parameters to command line arguments and update run settings."""
         if self.params_as_args is not None:
             for param in self.params_as_args:
                 if not param in self.params:
                     raise ValueError(
@@ -483,15 +468,15 @@
 
     def add_ml_model(
         self,
         name: str,
         backend: str,
         model: t.Optional[bytes] = None,
         model_path: t.Optional[str] = None,
-        device: t.Literal["CPU", "GPU"] = "CPU",
+        device: str = Device.CPU.value.upper(),
         devices_per_node: int = 1,
         first_device: int = 0,
         batch_size: int = 0,
         min_batch_size: int = 0,
         min_batch_timeout: int = 0,
         tag: str = "",
         inputs: t.Optional[t.List[str]] = None,
@@ -503,43 +488,30 @@
         orchestrator (converged or not) prior to the execution
         of this Model instance
 
         One of either model (in memory representation) or model_path (file)
         must be provided
 
         :param name: key to store model under
-        :type name: str
         :param backend: name of the backend (TORCH, TF, TFLITE, ONNX)
-        :type backend: str
         :param model: A model in memory (only supported for non-colocated orchestrators)
-        :type model: byte string, optional
         :param model_path: serialized model
-        :type model_path: file path to model
-        :param device: name of device for execution, defaults to "CPU"
-        :type device: str, optional
+        :param device: name of device for execution
         :param devices_per_node: The number of GPU devices available on the host.
                This parameter only applies to GPU devices and will be ignored if device
                is specified as CPU.
-        :type devices_per_node: int
         :param first_device: The first GPU device to use on the host.
                This parameter only applies to GPU devices and will be ignored if device
                is specified as CPU.
-        :type first_device: int
-        :param batch_size: batch size for execution, defaults to 0
-        :type batch_size: int, optional
-        :param min_batch_size: minimum batch size for model execution, defaults to 0
-        :type min_batch_size: int, optional
-        :param min_batch_timeout: time to wait for minimum batch size, defaults to 0
-        :type min_batch_timeout: int, optional
-        :param tag: additional tag for model information, defaults to ""
-        :type tag: str, optional
-        :param inputs: model inputs (TF only), defaults to None
-        :type inputs: list[str], optional
-        :param outputs: model outupts (TF only), defaults to None
-        :type outputs: list[str], optional
+        :param batch_size: batch size for execution
+        :param min_batch_size: minimum batch size for model execution
+        :param min_batch_timeout: time to wait for minimum batch size
+        :param tag: additional tag for model information
+        :param inputs: model inputs (TF only)
+        :param outputs: model outupts (TF only)
         """
         db_model = DBModel(
             name=name,
             backend=backend,
             model=model,
             model_file=model_path,
             device=device,
@@ -555,15 +527,15 @@
         self.add_ml_model_object(db_model)
 
     def add_script(
         self,
         name: str,
         script: t.Optional[str] = None,
         script_path: t.Optional[str] = None,
-        device: t.Literal["CPU", "GPU"] = "CPU",
+        device: str = Device.CPU.value.upper(),
         devices_per_node: int = 1,
         first_device: int = 0,
     ) -> None:
         """TorchScript to launch with this Model instance
 
         Each script added to the model will be loaded into an
         orchestrator (converged or not) prior to the execution
@@ -577,29 +549,23 @@
         alternatively, setting ``first_device=M`` will result in the script
         being stored on nodes M through M + N - 1.
 
         One of either script (in memory string representation) or script_path (file)
         must be provided
 
         :param name: key to store script under
-        :type name: str
         :param script: TorchScript code (only supported for non-colocated orchestrators)
-        :type script: str, optional
         :param script_path: path to TorchScript code
-        :type script_path: str, optional
-        :param device: device for script execution, defaults to "CPU"
-        :type device: str, optional
+        :param device: device for script execution
         :param devices_per_node: The number of GPU devices available on the host.
                This parameter only applies to GPU devices and will be ignored if device
                is specified as CPU.
-        :type devices_per_node: int
         :param first_device: The first GPU device to use on the host.
                This parameter only applies to GPU devices and will be ignored if device
                is specified as CPU.
-        :type first_device: int
         """
         db_script = DBScript(
             name=name,
             script=script,
             script_path=script_path,
             device=device,
             devices_per_node=devices_per_node,
@@ -607,15 +573,15 @@
         )
         self.add_script_object(db_script)
 
     def add_function(
         self,
         name: str,
         function: t.Optional[str] = None,
-        device: t.Literal["CPU", "GPU"] = "CPU",
+        device: str = Device.CPU.value.upper(),
         devices_per_node: int = 1,
         first_device: int = 0,
     ) -> None:
         """TorchScript function to launch with this Model instance
 
         Each script function to the model will be loaded into a
         non-converged orchestrator prior to the execution
@@ -626,27 +592,22 @@
         Device selection is either "GPU" or "CPU". If many devices are
         present, a number can be passed for specification e.g. "GPU:1".
 
         Setting ``devices_per_node=N``, with N greater than one will result
         in the model being stored in the first N devices of type ``device``.
 
         :param name: key to store function under
-        :type name: str
         :param function: TorchScript function code
-        :type function: str, optional
-        :param device: device for script execution, defaults to "CPU"
-        :type device: str, optional
+        :param device: device for script execution
         :param devices_per_node: The number of GPU devices available on the host.
                This parameter only applies to GPU devices and will be ignored if device
                is specified as CPU.
-        :type devices_per_node: int
         :param first_device: The first GPU device to use on the host.
                This parameter only applies to GPU devices and will be ignored if device
                is specified as CPU.
-        :type first_device: int
         """
         db_script = DBScript(
             name=name,
             script=function,
             device=device,
             devices_per_node=devices_per_node,
             first_device=first_device,
```

### Comparing `smartsim-0.6.2/smartsim/entity/strategies.py` & `smartsim-0.7.0/smartsim/entity/strategies.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.6.2/smartsim/error/__init__.py` & `smartsim-0.7.0/smartsim/error/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,13 +28,14 @@
     AllocationError,
     EntityExistsError,
     LauncherError,
     ParameterWriterError,
     ShellError,
     SmartSimError,
     SSConfigError,
+    SSDBFilesNotParseable,
     SSDBIDConflictError,
     SSInternalError,
     SSReservedKeywordError,
     SSUnsupportedError,
     UserStrategyError,
 )
```

### Comparing `smartsim-0.6.2/smartsim/error/errors.py` & `smartsim-0.7.0/smartsim/error/errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,14 +83,20 @@
 
 class SSDBIDConflictError(SmartSimError):
     """Raised in the event that a database identifier
     is not unique when multiple databases are created
     """
 
 
+class SSDBFilesNotParseable(SmartSimError):
+    """Raised when the files related to the database cannot be parsed.
+    Includes the case when the files do not exist.
+    """
+
+
 # Internal Exceptions
 
 
 class SSInternalError(Exception):
     """SSInternalError is raised when an internal error is encountered"""
 
 
@@ -145,7 +151,11 @@
     """Raised when a user attempts to proxy a managed ``Step`` through the
     unmanaged step proxy entry point
     """
 
 
 class SmartSimCLIActionCancelled(SmartSimError):
     """Raised when a `smart` CLI command is terminated"""
+
+
+class PreviewFormatError(SSUnsupportedError):
+    """Raised when the output format of the preview method call is not supported"""
```

### Comparing `smartsim-0.6.2/smartsim/experiment.py` & `smartsim-0.7.0/smartsim/experiment.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,27 +20,36 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+# pylint: disable=too-many-lines
+
 import os
 import os.path as osp
 import typing as t
-from os import getcwd
+from os import environ, getcwd
 
 from tabulate import tabulate
 
+from smartsim._core.config import CONFIG
 from smartsim.error.errors import SSUnsupportedError
+from smartsim.status import SmartSimStatus
 
-from ._core import Controller, Generator, Manifest
-from ._core.utils import init_default
+from ._core import Controller, Generator, Manifest, previewrenderer
 from .database import Orchestrator
-from .entity import Ensemble, Model, SmartSimEntity
+from .entity import (
+    Ensemble,
+    EntitySequence,
+    Model,
+    SmartSimEntity,
+    TelemetryConfiguration,
+)
 from .error import SmartSimError
 from .log import ctx_exp_path, get_logger, method_contextualizer
 from .settings import Container, base, settings
 from .wlm import detect_launcher
 
 logger = get_logger(__name__)
 
@@ -50,19 +59,34 @@
     the currently-executing experiment into context for log enrichment"""
     return exp.exp_path
 
 
 _contextualize = method_contextualizer(ctx_exp_path, _exp_path_map)
 
 
+class ExperimentTelemetryConfiguration(TelemetryConfiguration):
+    """Customized telemetry configuration for an `Experiment`. Ensures
+    backwards compatible behavior with drivers using environment variables
+    to enable experiment telemetry"""
+
+    def __init__(self) -> None:
+        super().__init__(enabled=CONFIG.telemetry_enabled)
+
+    def _on_enable(self) -> None:
+        """Modify the environment variable to enable telemetry."""
+        environ["SMARTSIM_FLAG_TELEMETRY"] = "1"
+
+    def _on_disable(self) -> None:
+        """Modify the environment variable to disable telemetry."""
+        environ["SMARTSIM_FLAG_TELEMETRY"] = "0"
+
+
 # pylint: disable=no-self-use
 class Experiment:
-    """Experiments are the Python user interface for SmartSim.
-
-    Experiment is a factory class that creates stages of a workflow
+    """Experiment is a factory class that creates stages of a workflow
     and manages their execution.
 
     The instances created by an Experiment represent executable code
     that is either user-specified, like the ``Model`` instance created
     by ``Experiment.create_model``, or pre-configured, like the ``Orchestrator``
     instance created by ``Experiment.create_database``.
 
@@ -76,15 +100,15 @@
 
     def __init__(
         self,
         name: str,
         exp_path: t.Optional[str] = None,
         launcher: str = "local",
     ):
-        """Initialize an Experiment instance
+        """Initialize an Experiment instance.
 
         With the default settings, the Experiment will use the
         local launcher, which will start all Experiment created
         instances on the localhost.
 
         Example of initializing an Experiment with the local launcher
 
@@ -97,63 +121,75 @@
         based on the type of system you are running on.
 
         .. highlight:: python
         .. code-block:: python
 
             exp = Experiment(name="my_exp", launcher="slurm")
 
-        If you wish your driver script and Experiment to be run across
+        If you want your Experiment driver script to be run across
         multiple system with different schedulers (workload managers)
-        you can also use the `auto` argument to have the Experiment guess
-        which launcher to use based on system installed binaries and libraries
+        you can also use the `auto` argument to have the Experiment detect
+        which launcher to use based on system installed binaries and libraries.
 
         .. highlight:: python
         .. code-block:: python
 
             exp = Experiment(name="my_exp", launcher="auto")
 
 
         The Experiment path will default to the current working directory
         and if the ``Experiment.generate`` method is called, a directory
         with the Experiment name will be created to house the output
         from the Experiment.
 
         :param name: name for the ``Experiment``
-        :type name: str
-        :param exp_path: path to location of ``Experiment`` directory if generated
-        :type exp_path: str, optional
+        :param exp_path: path to location of ``Experiment`` directory
         :param launcher: type of launcher being used, options are "slurm", "pbs",
                          "lsf", or "local". If set to "auto",
                          an attempt will be made to find an available launcher
                          on the system.
-                         Defaults to "local"
-        :type launcher: str, optional
         """
         self.name = name
         if exp_path:
             if not isinstance(exp_path, str):
                 raise TypeError("exp_path argument was not of type str")
             if not osp.isdir(osp.abspath(exp_path)):
                 raise NotADirectoryError("Experiment path provided does not exist")
             exp_path = osp.abspath(exp_path)
-        self.exp_path: str = init_default(osp.join(getcwd(), name), exp_path, str)
+        else:
+            exp_path = osp.join(getcwd(), name)
 
-        if launcher == "auto":
-            launcher = detect_launcher()
-        if launcher == "cobalt":
-            raise SSUnsupportedError("Cobalt launcher is no longer supported.")
+        self.exp_path = exp_path
 
-        self._control = Controller(launcher=launcher)
         self._launcher = launcher.lower()
+
+        if self._launcher == "auto":
+            self._launcher = detect_launcher()
+        if self._launcher == "cobalt":
+            raise SSUnsupportedError("Cobalt launcher is no longer supported.")
+
+        if launcher == "dragon":
+            self._set_dragon_server_path()
+
+        self._control = Controller(launcher=self._launcher)
+
         self.db_identifiers: t.Set[str] = set()
+        self._telemetry_cfg = ExperimentTelemetryConfiguration()
+
+    def _set_dragon_server_path(self) -> None:
+        """Set path for dragon server through environment varialbes"""
+        if not "SMARTSIM_DRAGON_SERVER_PATH" in environ:
+            environ["SMARTSIM_DRAGON_SERVER_PATH_EXP"] = osp.join(
+                self.exp_path, CONFIG.dragon_default_subdir
+            )
 
     @_contextualize
     def start(
         self,
-        *args: t.Any,
+        *args: t.Union[SmartSimEntity, EntitySequence[SmartSimEntity]],
         block: bool = True,
         summary: bool = False,
         kill_on_interrupt: bool = True,
     ) -> None:
         """Start passed instances using Experiment launcher
 
         Any instance ``Model``, ``Ensemble`` or ``Orchestrator``
@@ -164,15 +200,15 @@
         .. code-block:: python
 
             exp = Experiment(name="my_exp", launcher="slurm")
             settings = exp.create_run_settings(exe="./path/to/binary")
             model = exp.create_model("my_model", settings)
             exp.start(model)
 
-        Multiple instance can also be passed to the start method
+        Multiple entity instances can also be passed to the start method
         at once no matter which type of instance they are. These will
         all be launched together.
 
         .. highlight:: python
         .. code-block:: python
 
             exp.start(model_1, model_2, db, ensemble, block=True)
@@ -190,26 +226,21 @@
         If `kill_on_interrupt=True`, then all jobs launched by this
         experiment are guaranteed to be killed when ^C (SIGINT) signal is
         received. If `kill_on_interrupt=False`, then it is not guaranteed
         that all jobs launched by this experiment will be killed, and the
         zombie processes will need to be manually killed.
 
         :param block: block execution until all non-database
-                      jobs are finished, defaults to True
-        :type block: bool, optional
-        :param summary: print a launch summary prior to launch,
-                        defaults to False
-        :type summary: bool, optional
+                       jobs are finished
+        :param summary: print a launch summary prior to launch
         :param kill_on_interrupt: flag for killing jobs when ^C (SIGINT)
                                   signal is received.
-
-        :type kill_on_interrupt: bool, optional
         """
-
         start_manifest = Manifest(*args)
+        self._create_entity_dir(start_manifest)
         try:
             if summary:
                 self._launch_summary(start_manifest)
             self._control.start(
                 exp_name=self.name,
                 exp_path=self.exp_path,
                 manifest=start_manifest,
@@ -217,15 +248,17 @@
                 kill_on_interrupt=kill_on_interrupt,
             )
         except SmartSimError as e:
             logger.error(e)
             raise
 
     @_contextualize
-    def stop(self, *args: t.Any) -> None:
+    def stop(
+        self, *args: t.Union[SmartSimEntity, EntitySequence[SmartSimEntity]]
+    ) -> None:
         """Stop specific instances launched by this ``Experiment``
 
         Instances of ``Model``, ``Ensemble`` and ``Orchestrator``
         can all be passed as arguments to the stop method.
 
         Whichever launcher was specified at Experiment initialization
         will be used to stop the instance. For example, which using
@@ -237,14 +270,15 @@
         .. highlight:: python
         .. code-block:: python
 
             exp.stop(model)
             # multiple
             exp.stop(model_1, model_2, db, ensemble)
 
+        :param args: One or more SmartSimEntity or EntitySequence objects.
         :raises TypeError: if wrong type
         :raises SmartSimError: if stop request fails
         """
         stop_manifest = Manifest(*args)
         try:
             for entity in stop_manifest.models:
                 self._control.stop_entity(entity)
@@ -256,39 +290,35 @@
         except SmartSimError as e:
             logger.error(e)
             raise
 
     @_contextualize
     def generate(
         self,
-        *args: t.Any,
+        *args: t.Union[SmartSimEntity, EntitySequence[SmartSimEntity]],
         tag: t.Optional[str] = None,
         overwrite: bool = False,
         verbose: bool = False,
     ) -> None:
         """Generate the file structure for an ``Experiment``
 
-        ``Experiment.generate`` creates directories for each instance
-        passed to organize Experiments that launch many instances.
+        ``Experiment.generate`` creates directories for each entity
+        passed to organize Experiments that launch many entities.
 
         If files or directories are attached to ``Model`` objects
         using ``Model.attach_generator_files()``, those files or
         directories will be symlinked, copied, or configured and
         written into the created directory for that instance.
 
         Instances of ``Model``, ``Ensemble`` and ``Orchestrator``
         can all be passed as arguments to the generate method.
 
         :param tag: tag used in `to_configure` generator files
-        :type tag: str, optional
-        :param overwrite: overwrite existing folders and contents,
-               defaults to False
-        :type overwrite: bool, optional
+        :param overwrite: overwrite existing folders and contents
         :param verbose: log parameter settings to std out
-        :type verbose: bool
         """
         try:
             generator = Generator(self.exp_path, overwrite=overwrite, verbose=verbose)
             if tag:
                 generator.set_tag(tag)
             generator.generate_experiment(*args)
         except SmartSimError as e:
@@ -320,22 +350,18 @@
 
         If `kill_on_interrupt=True`, then all jobs launched by this
         experiment are guaranteed to be killed when ^C (SIGINT) signal is
         received. If `kill_on_interrupt=False`, then it is not guaranteed
         that all jobs launched by this experiment will be killed, and the
         zombie processes will need to be manually killed.
 
-        :param interval: frequency (in seconds) of logging to stdout,
-                         defaults to 10 seconds
-        :type interval: int, optional
-        :param verbose: set verbosity, defaults to True
-        :type verbose: bool, optional
+        :param interval: frequency (in seconds) of logging to stdout
+        :param verbose: set verbosity
         :param kill_on_interrupt: flag for killing jobs when SIGINT is received
-        :type kill_on_interrupt: bool, optional
-        :raises SmartSimError:
+        :raises SmartSimError: if poll request fails
         """
         try:
             self._control.poll(interval, verbose, kill_on_interrupt=kill_on_interrupt)
         except SmartSimError as e:
             logger.error(e)
             raise
 
@@ -347,29 +373,29 @@
         as an argument.
 
         Passing ``Orchestrator`` will return an error as a
         database deployment is never finished until stopped
         by the user.
 
         :param entity: object launched by this ``Experiment``
-        :type entity: Model | Ensemble
-        :returns: True if job has completed, False otherwise
-        :rtype: bool
+        :returns: True if the job has finished, False otherwise
         :raises SmartSimError: if entity has not been launched
                                by this ``Experiment``
         """
         try:
             return self._control.finished(entity)
         except SmartSimError as e:
             logger.error(e)
             raise
 
     @_contextualize
-    def get_status(self, *args: t.Any) -> t.List[str]:
-        """Query the status of launched instances
+    def get_status(
+        self, *args: t.Union[SmartSimEntity, EntitySequence[SmartSimEntity]]
+    ) -> t.List[SmartSimStatus]:
+        """Query the status of launched entity instances
 
         Return a smartsim.status string representing
         the status of the launched instance.
 
         .. highlight:: python
         .. code-block:: python
 
@@ -383,20 +409,19 @@
         .. code-block:: python
 
             statuses = exp.get_status(model, ensemble, orchestrator)
             complete = [s == smartsim.status.STATUS_COMPLETED for s in statuses]
             assert all(complete)
 
         :returns: status of the instances passed as arguments
-        :rtype: list[str]
         :raises SmartSimError: if status retrieval fails
         """
         try:
             manifest = Manifest(*args)
-            statuses: t.List[str] = []
+            statuses: t.List[SmartSimStatus] = []
             for entity in manifest.models:
                 statuses.append(self._control.get_entity_status(entity))
             for entity_list in manifest.all_entity_lists:
                 statuses.extend(self._control.get_entity_list_status(entity_list))
             return statuses
         except SmartSimError as e:
             logger.error(e)
@@ -407,69 +432,69 @@
         self,
         name: str,
         params: t.Optional[t.Dict[str, t.Any]] = None,
         batch_settings: t.Optional[base.BatchSettings] = None,
         run_settings: t.Optional[base.RunSettings] = None,
         replicas: t.Optional[int] = None,
         perm_strategy: str = "all_perm",
+        path: t.Optional[str] = None,
         **kwargs: t.Any,
     ) -> Ensemble:
         """Create an ``Ensemble`` of ``Model`` instances
 
         Ensembles can be launched sequentially or as a batch
         if using a non-local launcher. e.g. slurm
 
         Ensembles require one of the following combinations
-        of arguments
+        of arguments:
 
             - ``run_settings`` and ``params``
             - ``run_settings`` and ``replicas``
             - ``batch_settings``
             - ``batch_settings``, ``run_settings``, and ``params``
             - ``batch_settings``, ``run_settings``, and ``replicas``
 
         If given solely batch settings, an empty ensemble
-        will be created that models can be added to manually
+        will be created that Models can be added to manually
         through ``Ensemble.add_model()``.
-        The entire ensemble will launch as one batch.
+        The entire Ensemble will launch as one batch.
 
         Provided batch and run settings, either ``params``
         or ``replicas`` must be passed and the entire ensemble
         will launch as a single batch.
 
         Provided solely run settings, either ``params``
-        or ``replicas`` must be passed and the ensemble members
+        or ``replicas`` must be passed and the Ensemble members
         will each launch sequentially.
 
         The kwargs argument can be used to pass custom input
         parameters to the permutation strategy.
 
-        :param name: name of the ensemble
-        :type name: str
+        :param name: name of the ``Ensemble``
         :param params: parameters to expand into ``Model`` members
-        :type params: dict[str, Any]
         :param batch_settings: describes settings for ``Ensemble`` as batch workload
-        :type batch_settings: BatchSettings
         :param run_settings: describes how each ``Model`` should be executed
-        :type run_settings: RunSettings
         :param replicas: number of replicas to create
-        :type replicas: int
         :param perm_strategy: strategy for expanding ``params`` into
                               ``Model`` instances from params argument
                               options are "all_perm", "step", "random"
-                              or a callable function. Default is "all_perm".
-        :type perm_strategy: str, optional
+                              or a callable function.
         :raises SmartSimError: if initialization fails
         :return: ``Ensemble`` instance
-        :rtype: Ensemble
         """
+        if name is None:
+            raise AttributeError("Entity has no name. Please set name attribute.")
+        check_path = path or osp.join(self.exp_path, name)
+        entity_path: str = osp.abspath(check_path)
+
         try:
             new_ensemble = Ensemble(
-                name,
-                params or {},
+                name=name,
+                params=params or {},
+                path=entity_path,
                 batch_settings=batch_settings,
                 run_settings=run_settings,
                 perm_strat=perm_strategy,
                 replicas=replicas,
                 **kwargs,
             )
             return new_ensemble
@@ -493,35 +518,35 @@
         executable code in SmartSim. ``Model`` instances are named
         references to pieces of a workflow that can be parameterized,
         and executed.
 
         ``Model`` instances can be launched sequentially, as a batch job,
         or as a group by adding them into an ``Ensemble``.
 
-        All models require a reference to run settings to specify which
+        All ``Models`` require a reference to run settings to specify which
         executable to launch as well provide options for how to launch
         the executable with the underlying WLM. Furthermore, batch a
-        reference to a batch settings can be added to launch the model
-        as a batch job through ``Experiment.start``. If a model with
+        reference to a batch settings can be added to launch the ``Model``
+        as a batch job through ``Experiment.start``. If a ``Model`` with
         a reference to a set of batch settings is added to a larger
         entity with its own set of batch settings (for e.g. an
         ``Ensemble``) the batch settings of the larger entity will take
-        precedence and the batch setting of the model will be
+        precedence and the batch setting of the ``Model`` will be
         strategically ignored.
 
         Parameters supplied in the `params` argument can be written into
-        configuration files supplied at runtime to the model through
+        configuration files supplied at runtime to the ``Model`` through
         ``Model.attach_generator_files``. `params` can also be turned
         into executable arguments by calling ``Model.params_to_args``
 
         By default, ``Model`` instances will be executed in the
-        current working directory if no `path` argument is supplied.
+        exp_path/model_name directory if no `path` argument is supplied.
         If a ``Model`` instance is passed to ``Experiment.generate``,
         a directory within the ``Experiment`` directory will be created
-        to house the input and output files from the model.
+        to house the input and output files from the ``Model``.
 
         Example initialization of a ``Model`` instance
 
         .. highlight:: python
         .. code-block:: python
 
             from smartsim import Experiment
@@ -549,44 +574,39 @@
         New in 0.4.2, ``Model`` instances can now be colocated with
         an Orchestrator database over either TCP or UDS using the
         ``Model.colocate_db_tcp`` or ``Model.colocate_db_uds`` method
         respectively. The original ``Model.colocate_db`` method is now
         deprecated, but remains as an alias for ``Model.colocate_db_tcp``
         for backward compatibility.
 
-        :param name: name of the model
-        :type name: str
+        :param name: name of the ``Model``
         :param run_settings: defines how ``Model`` should be run
-        :type run_settings: RunSettings
-        :param params: model parameters for writing into configuration files
-        :type params: dict, optional
-        :param path: path to where the model should be executed at runtime
-        :type path: str, optional
-        :param enable_key_prefixing: If True, data sent to the Orchestrator
+        :param params: ``Model`` parameters for writing into configuration files
+        :param path: path to where the ``Model`` should be executed at runtime
+        :param enable_key_prefixing: If True, data sent to the ``Orchestrator``
                                      using SmartRedis from this ``Model`` will
                                      be prefixed with the ``Model`` name.
-                                     Default is True.
-        :type enable_key_prefixing: bool, optional
-        :param batch_settings: Settings to run model individually as a batch job,
-                               defaults to None
-        :type batch_settings: BatchSettings | None
+        :param batch_settings: Settings to run ``Model`` individually as a batch job.
         :raises SmartSimError: if initialization fails
         :return: the created ``Model``
-        :rtype: Model
         """
-        path = init_default(getcwd(), path, str)
-
-        if path is None:
-            path = getcwd()
+        if name is None:
+            raise AttributeError("Entity has no name. Please set name attribute.")
+        check_path = path or osp.join(self.exp_path, name)
+        entity_path: str = osp.abspath(check_path)
         if params is None:
             params = {}
 
         try:
             new_model = Model(
-                name, params, path, run_settings, batch_settings=batch_settings
+                name=name,
+                params=params,
+                path=entity_path,
+                run_settings=run_settings,
+                batch_settings=batch_settings,
             )
             if enable_key_prefixing:
                 new_model.enable_key_prefixing()
             return new_model
         except SmartSimError as e:
             logger.error(e)
             raise
@@ -601,15 +621,15 @@
         env_vars: t.Optional[t.Dict[str, t.Optional[str]]] = None,
         container: t.Optional[Container] = None,
         **kwargs: t.Any,
     ) -> settings.RunSettings:
         """Create a ``RunSettings`` instance.
 
         run_command="auto" will attempt to automatically
-        match a run command on the system with a RunSettings
+        match a run command on the system with a ``RunSettings``
         class in SmartSim. If found, the class corresponding
         to that run_command will be created and returned.
 
         If the local launcher is being used, auto detection will
         be turned off.
 
         If a recognized run command is passed, the ``RunSettings``
@@ -622,27 +642,20 @@
         Run Commands with implemented helper classes:
          - aprun (ALPS)
          - srun (SLURM)
          - mpirun (OpenMPI)
          - jsrun (LSF)
 
         :param run_command: command to run the executable
-        :type run_command: str
         :param exe: executable to run
-        :type exe: str
         :param exe_args: arguments to pass to the executable
-        :type exe_args: list[str], optional
         :param run_args: arguments to pass to the ``run_command``
-        :type run_args: dict[str, t.Union[int, str, float, None]], optional
         :param env_vars: environment variables to pass to the executable
-        :type env_vars: dict[str, str], optional
         :param container: if execution environment is containerized
-        :type container: Container, optional
         :return: the created ``RunSettings``
-        :rtype: RunSettings
         """
 
         try:
             return settings.create_run_settings(
                 self._launcher,
                 exe,
                 exe_args=exe_args,
@@ -685,26 +698,20 @@
                 "exclusive": None
             }
             bs = exp.create_batch_settings(nodes=3,
                                            time="10:00:00",
                                            batch_args=batch_args)
             bs.set_account("default")
 
-        :param nodes: number of nodes for batch job, defaults to 1
-        :type nodes: int, optional
-        :param time: length of batch job, defaults to ""
-        :type time: str, optional
-        :param queue: queue or partition (if slurm), defaults to ""
-        :type queue: str, optional
-        :param account: user account name for batch system, defaults to ""
-        :type account: str, optional
-        :param batch_args: additional batch arguments, defaults to None
-        :type batch_args: dict[str, str], optional
+        :param nodes: number of nodes for batch job
+        :param time: length of batch job
+        :param queue: queue or partition (if slurm)
+        :param account: user account name for batch system
+        :param batch_args: additional batch arguments
         :return: a newly created BatchSettings instance
-        :rtype: BatchSettings
         :raises SmartSimError: if batch creation fails
         """
         try:
             return settings.create_batch_settings(
                 self._launcher,
                 nodes=nodes,
                 time=time,
@@ -717,80 +724,70 @@
             logger.error(e)
             raise
 
     @_contextualize
     def create_database(
         self,
         port: int = 6379,
+        path: t.Optional[str] = None,
         db_nodes: int = 1,
         batch: bool = False,
         hosts: t.Optional[t.Union[t.List[str], str]] = None,
         run_command: str = "auto",
-        interface: str = "ipogif0",
+        interface: t.Union[str, t.List[str]] = "ipogif0",
         account: t.Optional[str] = None,
         time: t.Optional[str] = None,
         queue: t.Optional[str] = None,
         single_cmd: bool = True,
         db_identifier: str = "orchestrator",
         **kwargs: t.Any,
     ) -> Orchestrator:
-        """Initialize an Orchestrator database
+        """Initialize an ``Orchestrator`` database
 
         The ``Orchestrator`` database is a key-value store based
-        on Redis that can be launched together with other Experiment
+        on Redis that can be launched together with other ``Experiment``
         created instances for online data storage.
 
         When launched, ``Orchestrator`` can be used to communicate
         data between Fortran, Python, C, and C++ applications.
 
         Machine Learning models in Pytorch, Tensorflow, and ONNX (i.e. scikit-learn)
-        can also be stored within the Orchestrator database where they
+        can also be stored within the ``Orchestrator`` database where they
         can be called remotely and executed on CPU or GPU where
         the database is hosted.
 
         To enable a SmartSim ``Model`` to communicate with the database
         the workload must utilize the SmartRedis clients. For more
         information on the database, and SmartRedis clients see the
-        documentation at www.craylabs.org
+        documentation at https://www.craylabs.org/docs/smartredis.html
 
-        :param port: TCP/IP port, defaults to 6379
-        :type port: int, optional
-        :param db_nodes: number of database shards, defaults to 1
-        :type db_nodes: int, optional
-        :param batch: run as a batch workload, defaults to False
-        :type batch: bool, optional
-        :param hosts: specify hosts to launch on, defaults to None
-        :type hosts: list[str], optional
-        :param run_command: specify launch binary or detect automatically,
-            defaults to "auto"
-        :type run_command: str, optional
-        :param interface: Network interface, defaults to "ipogif0"
-        :type interface: str, optional
-        :param account: account to run batch on, defaults to None
-        :type account: str, optional
-        :param time: walltime for batch 'HH:MM:SS' format, defaults to None
-        :type time: str, optional
-        :param queue: queue to run the batch on, defaults to None
-        :type queue: str, optional
-        :param single_cmd: run all shards with one (MPMD) command, defaults to True
-        :type single_cmd: bool, optional
+        :param port: TCP/IP port
+        :param db_nodes: number of database shards
+        :param batch: run as a batch workload
+        :param hosts: specify hosts to launch on
+        :param run_command: specify launch binary or detect automatically
+        :param interface: Network interface
+        :param account: account to run batch on
+        :param time: walltime for batch 'HH:MM:SS' format
+        :param queue: queue to run the batch on
+        :param single_cmd: run all shards with one (MPMD) command
         :param db_identifier: an identifier to distinguish this orchestrator in
-            multiple-database experiments, defaults to "orchestrator"
-        :type db_identifier: str, optional
+            multiple-database experiments
         :raises SmartSimError: if detection of launcher or of run command fails
         :raises SmartSimError: if user indicated an incompatible run command
             for the launcher
-        :return: Orchestrator
-        :rtype: Orchestrator or derived class
+        :return: Orchestrator or derived class
         """
 
-        self.append_to_db_identifier_list(db_identifier)
-
+        self._append_to_db_identifier_list(db_identifier)
+        check_path = path or osp.join(self.exp_path, db_identifier)
+        entity_path: str = osp.abspath(check_path)
         return Orchestrator(
             port=port,
+            path=entity_path,
             db_nodes=db_nodes,
             batch=batch,
             hosts=hosts,
             run_command=run_command,
             interface=interface,
             account=account,
             time=time,
@@ -809,37 +806,80 @@
         that was launched by a previous ``Experiment``. This can be
         helpful in the case where separate runs of an ``Experiment``
         wish to use the same ``Orchestrator`` instance currently
         running on a system.
 
         :param checkpoint: the `smartsim_db.dat` file created
                            when an ``Orchestrator`` is launched
-        :type checkpoint: str
         """
         try:
             orc = self._control.reload_saved_db(checkpoint)
             return orc
         except SmartSimError as e:
             logger.error(e)
             raise
 
+    def preview(
+        self,
+        *args: t.Any,
+        verbosity_level: previewrenderer.Verbosity = previewrenderer.Verbosity.INFO,
+        output_format: previewrenderer.Format = previewrenderer.Format.PLAINTEXT,
+        output_filename: t.Optional[str] = None,
+    ) -> None:
+        """Preview entity information prior to launch. This method
+        aggregates multiple pieces of information to give users insight
+        into what and how entities will be launched.  Any instance of
+        ``Model``, ``Ensemble``, or ``Orchestrator`` created by the
+        Experiment can be passed as an argument to the preview method.
+
+        Verbosity levels:
+         - info: Display user-defined fields and entities.
+         - debug: Display user-defined field and entities and auto-generated
+            fields.
+         - developer: Display user-defined field and entities, auto-generated
+            fields, and run commands.
+
+        :param verbosity_level: verbosity level specified by user, defaults to info.
+        :param output_format: Set output format. The possible accepted
+            output formats are ``plain_text``.
+            Defaults to ``plain_text``.
+        :param output_filename: Specify name of file and extension to write
+            preview data to. If no output filename is set, the preview will be
+            output to stdout. Defaults to None.
+        """
+
+        # Retrieve any active orchestrator jobs
+        active_dbjobs = self._control.active_orchestrator_jobs
+
+        preview_manifest = Manifest(*args)
+
+        previewrenderer.render(
+            self,
+            preview_manifest,
+            verbosity_level,
+            output_format,
+            output_filename,
+            active_dbjobs,
+        )
+
+    @property
+    def launcher(self) -> str:
+        return self._launcher
+
     @_contextualize
     def summary(self, style: str = "github") -> str:
         """Return a summary of the ``Experiment``
 
         The summary will show each instance that has been
         launched and completed in this ``Experiment``
 
         :param style: the style in which the summary table is formatted,
-                       for a full list of styles see:
-                       https://github.com/astanin/python-tabulate#table-format,
-                       defaults to "github"
-        :type style: str, optional
+                       for a full list of styles see the table-format section of:
+                       https://github.com/astanin/python-tabulate
         :return: tabulate string of ``Experiment`` history
-        :rtype: str
         """
         values = []
         headers = [
             "Name",
             "Entity-Type",
             "JobID",
             "RunID",
@@ -865,19 +905,26 @@
             headers,
             showindex=True,
             tablefmt=style,
             missingval="None",
             disable_numparse=True,
         )
 
+    @property
+    def telemetry(self) -> TelemetryConfiguration:
+        """Return the telemetry configuration for this entity.
+
+        :returns: configuration of telemetry for this entity
+        """
+        return self._telemetry_cfg
+
     def _launch_summary(self, manifest: Manifest) -> None:
         """Experiment pre-launch summary of entities that will be launched
 
         :param manifest: Manifest of deployables.
-        :type manifest: Manifest
         """
 
         summary = "\n\n=== Launch Summary ===\n"
         summary += f"Experiment: {self.name}\n"
         summary += f"Experiment Path: {self.exp_path}\n"
         summary += f"Launcher: {self._launcher}\n"
         if manifest.models:
@@ -890,52 +937,37 @@
         else:
             summary += "Database Status: inactive\n"
 
         summary += f"\n{str(manifest)}"
 
         logger.info(summary)
 
+    def _create_entity_dir(self, start_manifest: Manifest) -> None:
+        def create_entity_dir(entity: t.Union[Orchestrator, Model, Ensemble]) -> None:
+            if not os.path.isdir(entity.path):
+                os.makedirs(entity.path)
+
+        for model in start_manifest.models:
+            create_entity_dir(model)
+
+        for orch in start_manifest.dbs:
+            create_entity_dir(orch)
+
+        for ensemble in start_manifest.ensembles:
+            create_entity_dir(ensemble)
+
+            for member in ensemble.models:
+                create_entity_dir(member)
+
     def __str__(self) -> str:
         return self.name
 
-    def append_to_db_identifier_list(self, db_identifier: str) -> None:
+    def _append_to_db_identifier_list(self, db_identifier: str) -> None:
         """Check if db_identifier already exists when calling create_database"""
         if db_identifier in self.db_identifiers:
             logger.warning(
                 f"A database with the identifier {db_identifier} has already been made "
                 "An error will be raised if multiple databases are started "
                 "with the same identifier"
             )
         # Otherwise, add
         self.db_identifiers.add(db_identifier)
-
-    def enable_telemetry(self) -> None:
-        """Experiments will start producing telemetry for all entities run
-        through ``Experiment.start``
-
-        .. warning::
-
-            This method is currently implemented so that ALL ``Experiment``
-            instances will begin producing telemetry data. In the future it
-            is planned to have this method work on a "per instance" basis!
-        """
-        self._set_telemetry(True)
-
-    def disable_telemetry(self) -> None:
-        """Experiments will stop producing telemetry for all entities run
-        through ``Experiment.start``
-
-        .. warning::
-
-            This method is currently implemented so that ALL ``Experiment``
-            instances will stop producing telemetry data. In the future it
-            is planned to have this method work on a "per instance" basis!
-        """
-        self._set_telemetry(False)
-
-    @staticmethod
-    def _set_telemetry(switch: bool, /) -> None:
-        tm_key = "SMARTSIM_FLAG_TELEMETRY"
-        if switch:
-            os.environ[tm_key] = "1"
-        else:
-            os.environ[tm_key] = "0"
```

### Comparing `smartsim-0.6.2/smartsim/log.py` & `smartsim-0.7.0/smartsim/log.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,27 +23,29 @@
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import functools
 import logging
 import pathlib
+import socket
 import sys
 import threading
 import typing as t
 from contextvars import ContextVar, copy_context
 
 import coloredlogs
 
 from smartsim._core.config import CONFIG
 
 # constants
 DEFAULT_DATE_FORMAT: t.Final[str] = "%H:%M:%S"
 DEFAULT_LOG_FORMAT: t.Final[str] = (
-    "%(asctime)s %(hostname)s %(name)s[%(process)d] %(levelname)s %(message)s"
+    "%(asctime)s %(hostname)s %(name)s[%(process)d:%(threadName)s] "
+    "%(levelname)s %(message)s"
 )
 EXPERIMENT_LOG_FORMAT = DEFAULT_LOG_FORMAT.replace("s[%", "s {%(exp_path)s} [%")
 
 # configure colored loggs
 coloredlogs.DEFAULT_DATE_FORMAT = DEFAULT_DATE_FORMAT
 coloredlogs.DEFAULT_LOG_FORMAT = DEFAULT_LOG_FORMAT
 
@@ -70,17 +72,15 @@
          - quiet: Just shows errors and warnings
          - info: Show basic information and errors (default)
          - debug: Shows info, errors and user debug information
          - developer: Shows everything happening during execution
                       extremely verbose logging.
 
     :param user_log_level: log level specified by user, defaults to info
-    :type user_log_level: str
     :returns: Log level for coloredlogs
-    :rtype: str
     """
     user_log_level = user_log_level.lower()
     if user_log_level in ["info", "debug", "warning"]:
         return user_log_level
     if user_log_level == "quiet":
         return "warning"
     # extremely verbose logging used internally
@@ -90,25 +90,20 @@
 
 
 def get_exp_log_paths() -> t.Tuple[t.Optional[pathlib.Path], t.Optional[pathlib.Path]]:
     """Returns the output and error file paths to experiment logs.
     Returns None for both paths if experiment context is unavailable.
 
     :returns: 2-tuple of paths to experiment logs in form (output_path, error_path)
-    if telemetry is enabled, a 2-tuple of None otherwise
-    :rtype: Tuple[pathlib.Path | None, pathlib.Path | None]
     """
     default_paths = None, None
 
-    if not CONFIG.telemetry_enabled:
-        return default_paths
-
-    if _exp_path := ctx_exp_path.get():
-        file_out = pathlib.Path(_exp_path) / CONFIG.telemetry_subdir / "smartsim.out"
-        file_err = pathlib.Path(_exp_path) / CONFIG.telemetry_subdir / "smartsim.err"
+    if _path := ctx_exp_path.get():
+        file_out = pathlib.Path(_path) / CONFIG.telemetry_subdir / "logs/smartsim.out"
+        file_err = pathlib.Path(_path) / CONFIG.telemetry_subdir / "logs/smartsim.err"
         return file_out, file_err
 
     return default_paths
 
 
 class ContextThread(threading.Thread):
     """Thread that ensures the context vars of the caller are available"""
@@ -123,22 +118,42 @@
     """Filter that performs enrichment of a log record by adding context
     information about the experiment being executed"""
 
     def filter(self, record: logging.LogRecord) -> bool:
         """Enrich log records with active experiment context
 
         :param record: the record to evaluate for filtering
-        :type record: logging.LogRecord
         :returns: always True
-        :rtype: bool
         """
         record.exp_path = ctx_exp_path.get()
         return True
 
 
+class HostnameFilter(logging.Filter):
+    """Filter that performs enrichment of a log record by adding
+    the hostname of the machine executing the code"""
+
+    def __init__(self, name: str = "") -> None:
+        super().__init__(name)
+        self._hostname = ""
+
+    @property
+    @functools.lru_cache
+    def hostname(self) -> str:
+        """Returns the hostname of the machine executing the code"""
+        self._hostname = socket.gethostname()
+        return self._hostname
+
+    def filter(self, record: logging.LogRecord) -> bool:
+        # the hostname may already added if using the `ColoredLogs` plugin
+        if not hasattr(record, "hostname"):
+            record.hostname = self.hostname
+        return True
+
+
 class ContextAwareLogger(logging.Logger):
     """A logger customized to automatically write experiment logs to a
     dynamic target directory by inspecting the value of a context var"""
 
     def __init__(self, name: str, level: t.Union[int, str] = 0) -> None:
         super().__init__(name, level)
         self.addFilter(ContextInjectingLogFilter(name="exp-ctx-log-filter"))
@@ -190,21 +205,17 @@
 
         logger.info("This is a message")
         logger.debug("This is a debug message")
         logger.error("This is an error message")
         logger.warning("This is a warning message")
 
     :param name: the name of the desired logger
-    :type name: str
     :param log_level: what level to set the logger to
-    :type log_level: str
     :param fmt: the format of the log messages
-    :type fmt: str
     :returns: logger instance
-    :rtype: logging.Logger
     """
     # if name is None, then logger is the root logger
     # if not root logger, get the name of file without prefix.
     user_log_level = CONFIG.log_level
     if user_log_level != "developer":
         name = "SmartSim"
 
@@ -221,44 +232,38 @@
 class LowPassFilter(logging.Filter):
     """A filter that passes all records below a specified level"""
 
     def __init__(self, maximum_level: str = "INFO"):
         """Create a low-pass log filter allowing messages below a specific log level
 
         :param maximum_level: The maximum log level to be passed by the filter
-        :type maximum_level: str
         """
         super().__init__()
         self.max = maximum_level
 
     def filter(self, record: logging.LogRecord) -> bool:
         """Filter log records; pass those less than or equal to the maximum level
 
         :param record: the record to evaluate for filtering
-        :type record: logging.LogRecord
         :returns: True if record level passes filter, False otherwise
-        :rtype: bool
         """
         # If a string representation of the level is passed in,
         # the corresponding numeric value is returned.
         level_no: int = logging.getLevelName(self.max)
         return record.levelno <= level_no
 
 
 def log_to_file(filename: str, log_level: str = "debug") -> None:
     """Installs a second filestream handler to the root logger,
     allowing subsequent logging calls to be sent to filename.
 
     :param filename: the name of the desired log file.
-    :type filename: str
-
     :param log_level: as defined in get_logger.  Can be specified
                       to allow the file to store more or less verbose
                       logging information.
-    :type log_level: str
     """
     logger = logging.getLogger("SmartSim")
     stream = open(  # pylint: disable=consider-using-with
         filename, "w+", encoding="utf-8"
     )
     coloredlogs.install(stream=stream, logger=logger, level=log_level)
 
@@ -270,27 +275,21 @@
     fmt: t.Optional[str] = EXPERIMENT_LOG_FORMAT,
     log_filter: t.Optional[logging.Filter] = None,
 ) -> logging.Handler:
     """Installs a second filestream handler to the root logger,
     allowing subsequent logging calls to be sent to filename.
 
     :param filename: the name of the desired log file.
-    :type filename: str
     :param log_level: as defined in get_logger.  Can be specified
                       to allow the file to store more or less verbose
                       logging information.
-    :type log_level: int | str
     :param logger: an existing logger to add the handler to
-    :type logger: (optional) logging.Logger
     :param fmt: a log format for the handler (otherwise, EXPERIMENT_LOG_FORMAT)
-    :type fmt: (optional) str
     :param log_filter: log filter to attach to handler
-    :type log_filter: (optional) logging.Filter
     :return: logging.Handler
-    :rtype: logging.Handler
     """
     # ensure logs are written even if specified dir doesn't exist
     log_path = pathlib.Path(filename)
     if not log_path.parent.exists():
         log_path.parent.mkdir(parents=True, exist_ok=True)
 
     handler = logging.FileHandler(filename, mode="a+", encoding="utf-8")
@@ -318,17 +317,16 @@
     to be placed into global context prior to execution of the
     decorated method.
     Usage Note: the use of `self` below requires that the decorated function is passed
     the object containing a value that will be modified in the context. `ctx_map`
     must accept an instance of matching type.
 
     :param ctx_var: The ContextVar that will be modified
-    :type ctx_var: ContextVar
     :param ctx_map: A function that returns the value to be set to ctx_var
-    :type ctx_map: t.Callable[[_T], _ContextT]"""
+    """
 
     def _contextualize(
         fn: "t.Callable[Concatenate[_T, _PR], _RT]", /
     ) -> "t.Callable[Concatenate[_T, _PR], _RT]":
         """Executes the decorated method in a cloned context and ensures
         `ctx_var` is updated to the value returned by `ctx_map` prior to
         calling the decorated method"""
```

### Comparing `smartsim-0.6.2/smartsim/ml/__init__.py` & `smartsim-0.7.0/smartsim/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.6.2/smartsim/ml/data.py` & `smartsim-0.7.0/smartsim/ml/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,21 +53,17 @@
     information about the aggregation list holding the training datasets.
 
     Each training dataset will store batches of samples and (optionally) labels or
     targets in the form of tensors. The tensors must always have the same names, which
     can be accessed in ``DataInfo.sample_name`` and ``DataInfo.target_name``.
 
     :param list_name: Name of the aggregation list used for sample datasets
-    :type list_name: str
     :param sample_name: Name of tensor holding training samples in stored datasets.
-    :type sample_name: str
     :param target_name: Name of tensor holding targets or labels in stored datasets.
-    :type target_name: str
     :num_classes: Number of classes (for categorical data).
-    :type num_classes: int | None
     """
 
     def __init__(
         self,
         list_name: str,
         sample_name: str = "samples",
         target_name: str = "targets",
@@ -82,15 +78,14 @@
     def publish(self, client: Client) -> None:
         """Upload DataInfo information to Orchestrator
 
         The information is put on the DB as a DataSet, with strings
         stored as metastrings and integers stored as metascalars.
 
         :param client: Client to connect to Database
-        :type client: SmartRedis.Client
         """
         info_ds = Dataset(self._ds_name)
         info_ds.add_meta_string("sample_name", self.sample_name)
         if self.target_name:
             info_ds.add_meta_string("target_name", self.target_name)
         if self.num_classes:
             info_ds.add_meta_scalar("num_classes", self.num_classes)
@@ -100,24 +95,24 @@
         """Download DataInfo information from Orchestrator
 
         The information retrieved from the DB is used to populate
         this object's members. If the information is not available
         on the DB, the object members are not modified.
 
         :param client: Client to connect to Database
-        :type client: SmartRedis.Client
         """
         try:
             info_ds = client.get_dataset(self._ds_name)
-        except RedisReplyError:
+        except RedisReplyError as e:
             # If the info was not published, proceed with default parameters
             logger.warning(
                 "Could not retrieve data for DataInfo object, the following "
                 "values will be kept."
             )
+            logger.error(f"Original error from Redis was {e}")
             logger.warning(str(self))
             return
         self.sample_name = info_ds.get_meta_strings("sample_name")[0]
         field_names = info_ds.get_metadata_field_names()
         if "target_name" in field_names:
             self.target_name = info_ds.get_meta_strings("target_name")[0]
         if "num_classes" in field_names:
@@ -144,29 +139,21 @@
     the batches which are uploaded.
 
     Each time a new batch is available, it is sufficient to call `put_batch`,
     and the data will be stored following the naming convention specified
     by the attributes of this class.
 
     :param list_name: Name of the dataset as stored on the Orchestrator
-    :type list_name: str
     :param sample_name: Name of samples tensor in uploaded Datasets
-    :type sample_name: str
     :param target_name: Name of targets tensor (if needed) in uploaded Datasets
-    :type target_name: str
     :param num_classes: Number of classes of targets, if categorical
-    :type num_classes: int
     :param cluster: Whether the SmartSim Orchestrator is being run as a cluster
-    :type cluster: bool
     :param address: Address of Redis DB as <ip_address>:<port>
-    :type address: str
     :param rank: Rank of DataUploader in multi-process application (e.g. MPI rank).
-    :type rank: int
     :param verbose: If output should be logged to screen.
-    :type verbose: bool
 
     """
 
     def __init__(
         self,
         list_name: str = "training_data",
         sample_name: str = "samples",
@@ -262,43 +249,31 @@
 
     Calling `update_data()`
      - check if new batches are available and download them,
        if `dynamic` is set to `True`
      - shuffle the dataset if `shuffle` is set to ``True``.
 
     :param batch_size: Size of batches obtained with __iter__
-    :type batch_size: int
     :param dynamic: Whether new batches should be donwnloaded when ``update_data``
         is called.
-    :type dtnamic: bool
     :param shuffle: whether order of samples has to be shuffled when
         calling `update_data`
-    :type shuffle: bool
     :param data_info_or_list_name: DataInfo object with details about dataset to
         download, if a string is passed, it is used to download DataInfo data
         from DB, assuming it was stored with ``list_name=data_info_or_list_name``
-    :type data_info_or_list_name: DataInfo | str
     :param list_name: Name of aggregation list used to upload data
-    :type list_name: str
     :param cluster: Whether the Orchestrator will be run as a cluster
-    :type cluster: bool
     :param address: Address of Redis client as <ip_address>:<port>
-    :type address: str
     :param replica_rank: When StaticDataDownloader is used distributedly,
         indicates the rank of this object
-    :type replica_rank: int
     :param num_replicas: When BatchDownlaoder is used distributedly, indicates
                          the total number of ranks
-    :type num_replicas: int
     :param verbose: Whether log messages should be printed
-    :type verbose: bool
     :param init_samples: whether samples should be initialized in the constructor
-    :type init_samples: bool
     :param max_fetch_trials: maximum number of attempts to initialize data
-    :type max_fetch_trials: int
     """
 
     def __init__(
         self,
         data_info_or_list_name: t.Union[str, DataInfo],
         batch_size: int = 32,
         dynamic: bool = True,
@@ -306,14 +281,15 @@
         cluster: bool = True,
         address: t.Optional[str] = None,
         replica_rank: int = 0,
         num_replicas: int = 1,
         verbose: bool = False,
         init_samples: bool = True,
         max_fetch_trials: int = -1,
+        wait_interval: float = 10.0,
     ) -> None:
         self.address = address
         self.cluster = cluster
         self.verbose = verbose
         self.samples: t.Optional["npt.NDArray[t.Any]"] = None
         self.targets: t.Optional["npt.NDArray[t.Any]"] = None
         self.num_samples = 0
@@ -332,15 +308,15 @@
         self._client: t.Optional[Client] = None
         sskeyin = environ.get("SSKEYIN", "")
         self.uploader_keys = sskeyin.split(",")
 
         self.set_replica_parameters(replica_rank, num_replicas)
 
         if init_samples:
-            self.init_samples(max_fetch_trials)
+            self.init_samples(max_fetch_trials, wait_interval)
 
     @property
     def client(self) -> Client:
         if self._client is None:
             raise ValueError("Client not initialized")
         return self._client
 
@@ -374,15 +350,14 @@
         return self._info.num_classes
 
     @property
     def need_targets(self) -> bool:
         """Compute if targets have to be downloaded.
 
         :return: Whether targets (or labels) should be downloaded
-        :rtype: bool
         """
         return bool(self.target_name) and not self.autoencoding
 
     def __len__(self) -> int:
         length = int(np.floor(self.num_samples / self.batch_size))
         return length
 
@@ -400,32 +375,32 @@
                 "init_samples() or initialize generator with init_samples=True"
             )
 
         yield from (
             self._data_generation(self._calc_indices(idx)) for idx in range(len(self))
         )
 
-    def init_samples(self, init_trials: int = -1) -> None:
+    def init_samples(self, init_trials: int = -1, wait_interval: float = 10.0) -> None:
         """Initialize samples (and targets, if needed).
 
         A new attempt to download samples will be made every ten seconds,
         for ``init_trials`` times.
+
         :param init_trials: maximum number of attempts to fetch data
-        :type init_trials: int
         """
         self._client = Client(self.cluster, self.address)
 
         num_trials = 0
         max_trials = init_trials or -1
         while not self and num_trials != max_trials:
             self._update_samples_and_targets()
-            self.log(
-                "DataLoader could not download samples, will try again in 10 seconds"
-            )
-            time.sleep(10)
+            msg = "DataLoader could not download samples, will try again in "
+            msg += f"{wait_interval} seconds"
+            self.log(msg)
+            time.sleep(wait_interval)
             num_trials += 1
 
         if not self:
             raise SSInternalError(
                 "Could not download samples in given number of trials"
             )
         if self.shuffle:
```

### Comparing `smartsim-0.6.2/smartsim/ml/tf/__init__.py` & `smartsim-0.7.0/smartsim/ml/tf/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,27 +31,26 @@
 logger = get_logger(__name__)
 
 vers = Versioner()
 TF_VERSION = vers.TENSORFLOW
 
 try:
     import tensorflow as tf
-
-    installed_tf = Version_(tf.__version__)
-    assert installed_tf >= "2.4.0"
-
 except ImportError:  # pragma: no cover
     raise ModuleNotFoundError(
         f"TensorFlow {TF_VERSION} is not installed. "
-        "Please install it to use smartsim.tf"
+        "Please install it to use smartsim.ml.tf"
     ) from None
+
+try:
+    installed_tf = Version_(tf.__version__)
+    assert installed_tf >= TF_VERSION
 except AssertionError:  # pragma: no cover
-    msg = (
+    raise SmartSimError(
         f"TensorFlow >= {TF_VERSION} is required for smartsim. "
         f"tf, you have {tf.__version__}"
-    )
-    raise SmartSimError() from None
+    ) from None
 
 
 # pylint: disable=wrong-import-position
 from .data import DynamicDataGenerator, StaticDataGenerator
 from .utils import freeze_model, serialize_model
```

### Comparing `smartsim-0.6.2/smartsim/ml/tf/data.py` & `smartsim-0.7.0/smartsim/ml/tf/data.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.6.2/smartsim/ml/tf/utils.py` & `smartsim-0.7.0/smartsim/ml/tf/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,21 +43,17 @@
     must be frozen and the inputs and outputs provided to the
     smartredis.client.set_model_from_file() method.
 
     This utiliy function provides everything users need to take
     a trained model and put it inside an ``orchestrator`` instance
 
     :param model: TensorFlow or Keras model
-    :type model: tf.Module
     :param output_dir: output dir to save model file to
-    :type output_dir: str
     :param file_name: name of model file to create
-    :type file_name: str
     :return: path to model file, model input layer names, model output layer names
-    :rtype: str, list[str], list[str]
     """
     # TODO figure out why layer names don't match up to
     # specified name in Model init.
 
     if not file_name.endswith(".pb"):
         file_name = file_name + ".pb"
 
@@ -89,17 +85,15 @@
     must be frozen and the inputs and outputs provided to the
     smartredis.client.set_model() method.
 
     This utiliy function provides everything users need to take
     a trained model and put it inside an ``orchestrator`` instance.
 
     :param model: TensorFlow or Keras model
-    :type model: tf.Module
     :return: serialized model, model input layer names, model output layer names
-    :rtype: str, list[str], list[str]
     """
 
     full_model = tf.function(model)
     full_model = full_model.get_concrete_function(
         tf.TensorSpec(model.inputs[0].shape, model.inputs[0].dtype)
     )
```

### Comparing `smartsim-0.6.2/smartsim/ml/torch/__init__.py` & `smartsim-0.7.0/smartsim/_core/utils/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,8 +20,16 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from .data import DataLoader, DynamicDataGenerator, StaticDataGenerator
+from .helpers import (
+    check_for_utility,
+    colorize,
+    delete_elements,
+    execute_platform_cmd,
+    installed_redisai_backends,
+    is_crayex_platform,
+)
+from .redis import check_cluster_status, create_cluster, db_is_active
```

### Comparing `smartsim-0.6.2/smartsim/ml/torch/data.py` & `smartsim-0.7.0/smartsim/ml/torch/data.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.6.2/smartsim/servertype.py` & `smartsim-0.7.0/smartsim/servertype.py`

 * *Files identical despite different names*

### Comparing `smartsim-0.6.2/smartsim/settings/__init__.py` & `smartsim-0.7.0/smartsim/settings/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from .alpsSettings import AprunSettings
 from .base import RunSettings, SettingsBase
 from .containers import Container, Singularity
+from .dragonRunSettings import DragonRunSettings
 from .lsfSettings import BsubBatchSettings, JsrunSettings
 from .mpiSettings import MpiexecSettings, MpirunSettings, OrterunSettings
 from .palsSettings import PalsMpiexecSettings
 from .pbsSettings import QsubBatchSettings
 from .slurmSettings import SbatchSettings, SrunSettings
 
 __all__ = [
@@ -42,10 +43,11 @@
     "OrterunSettings",
     "QsubBatchSettings",
     "RunSettings",
     "SettingsBase",
     "SbatchSettings",
     "SrunSettings",
     "PalsMpiexecSettings",
+    "DragonRunSettings",
     "Container",
     "Singularity",
 ]
```

### Comparing `smartsim-0.6.2/smartsim/settings/alpsSettings.py` & `smartsim-0.7.0/smartsim/settings/alpsSettings.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,21 +42,17 @@
         **kwargs: t.Any,
     ):
         """Settings to run job with ``aprun`` command
 
         ``AprunSettings`` can be used for the `pbs` launcher.
 
         :param exe: executable
-        :type exe: str
-        :param exe_args: executable arguments, defaults to None
-        :type exe_args: str | list[str], optional
-        :param run_args: arguments for run command, defaults to None
-        :type run_args: dict[str, t.Union[int, str, float, None]], optional
-        :param env_vars: environment vars to launch job with, defaults to None
-        :type env_vars: dict[str, str], optional
+        :param exe_args: executable arguments
+        :param run_args: arguments for run command
+        :param env_vars: environment vars to launch job with
         """
         super().__init__(
             exe,
             exe_args,
             run_command="aprun",
             run_args=run_args,
             env_vars=env_vars,
@@ -67,15 +63,14 @@
     def make_mpmd(self, settings: RunSettings) -> None:
         """Make job an MPMD job
 
         This method combines two ``AprunSettings``
         into a single MPMD command joined with ':'
 
         :param settings: ``AprunSettings`` instance
-        :type settings: AprunSettings
         """
         if self.colocated_db_settings:
             raise SSUnsupportedError(
                 "Colocated models cannot be run as a mpmd workload"
             )
         if self.container:
             raise SSUnsupportedError(
@@ -85,43 +80,39 @@
 
     def set_cpus_per_task(self, cpus_per_task: int) -> None:
         """Set the number of cpus to use per task
 
         This sets ``--cpus-per-pe``
 
         :param cpus_per_task: number of cpus to use per task
-        :type cpus_per_task: int
         """
         self.run_args["cpus-per-pe"] = int(cpus_per_task)
 
     def set_tasks(self, tasks: int) -> None:
         """Set the number of tasks for this job
 
         This sets ``--pes``
 
         :param tasks: number of tasks
-        :type tasks: int
         """
         self.run_args["pes"] = int(tasks)
 
     def set_tasks_per_node(self, tasks_per_node: int) -> None:
         """Set the number of tasks for this job
 
         This sets ``--pes-per-node``
 
         :param tasks_per_node: number of tasks per node
-        :type tasks_per_node: int
         """
         self.run_args["pes-per-node"] = int(tasks_per_node)
 
     def set_hostlist(self, host_list: t.Union[str, t.List[str]]) -> None:
         """Specify the hostlist for this job
 
         :param host_list: hosts to launch on
-        :type host_list: str | list[str]
         :raises TypeError: if not str or list of str
         """
         if isinstance(host_list, str):
             host_list = [host_list.strip()]
         if not isinstance(host_list, list):
             raise TypeError("host_list argument must be a list of strings")
         if not all(isinstance(host, str) for host in host_list):
@@ -130,23 +121,21 @@
 
     def set_hostlist_from_file(self, file_path: str) -> None:
         """Use the contents of a file to set the node list
 
         This sets ``--node-list-file``
 
         :param file_path: Path to the hostlist file
-        :type file_path: str
         """
         self.run_args["node-list-file"] = file_path
 
     def set_excluded_hosts(self, host_list: t.Union[str, t.List[str]]) -> None:
         """Specify a list of hosts to exclude for launching this job
 
         :param host_list: hosts to exclude
-        :type host_list: str | list[str]
         :raises TypeError: if not str or list of str
         """
         if isinstance(host_list, str):
             host_list = [host_list.strip()]
         if not isinstance(host_list, list):
             raise TypeError("host_list argument must be a list of strings")
         if not all(isinstance(host, str) for host in host_list):
@@ -155,61 +144,56 @@
 
     def set_cpu_bindings(self, bindings: t.Union[int, t.List[int]]) -> None:
         """Specifies the cores to which MPI processes are bound
 
         This sets ``--cpu-binding``
 
         :param bindings: List of cpu numbers
-        :type bindings: list[int] | int
         """
         if isinstance(bindings, int):
             bindings = [bindings]
         self.run_args["cpu-binding"] = ",".join(str(int(num)) for num in bindings)
 
     def set_memory_per_node(self, memory_per_node: int) -> None:
         """Specify the real memory required per node
 
         This sets ``--memory-per-pe`` in megabytes
 
         :param memory_per_node: Per PE memory limit in megabytes
-        :type memory_per_node: int
         """
         self.run_args["memory-per-pe"] = int(memory_per_node)
 
     def set_verbose_launch(self, verbose: bool) -> None:
         """Set the job to run in verbose mode
 
         This sets ``--debug`` arg to the highest level
 
         :param verbose: Whether the job should be run verbosely
-        :type verbose: bool
         """
         if verbose:
             self.run_args["debug"] = 7
         else:
             self.run_args.pop("debug", None)
 
     def set_quiet_launch(self, quiet: bool) -> None:
         """Set the job to run in quiet mode
 
         This sets ``--quiet``
 
         :param quiet: Whether the job should be run quietly
-        :type quiet: bool
         """
         if quiet:
             self.run_args["quiet"] = None
         else:
             self.run_args.pop("quiet", None)
 
     def format_run_args(self) -> t.List[str]:
         """Return a list of ALPS formatted run arguments
 
         :return: list of ALPS arguments for these settings
-        :rtype: list[str]
         """
         # args launcher uses
         args = []
         restricted = ["wdir"]
 
         for opt, value in self.run_args.items():
             if opt not in restricted:
@@ -224,24 +208,22 @@
                         args += ["=".join((prefix + opt, str(value)))]
         return args
 
     def format_env_vars(self) -> t.List[str]:
         """Format the environment variables for aprun
 
         :return: list of env vars
-        :rtype: list[str]
         """
         formatted = []
         if self.env_vars:
             for name, value in self.env_vars.items():
                 formatted += ["-e", name + "=" + str(value)]
         return formatted
 
     def set_walltime(self, walltime: str) -> None:
         """Set the walltime of the job
 
         Walltime is given in total number of seconds
 
         :param walltime: wall time
-        :type walltime: str
         """
         self.run_args["cpu-time-limit"] = str(walltime)
```

### Comparing `smartsim-0.6.2/smartsim/settings/base.py` & `smartsim-0.7.0/smartsim/settings/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -71,27 +71,19 @@
 
         .. highlight:: python
         .. code-block:: python
 
             rs = RunSettings("echo", "hello", "mpirun", run_args={"-np": "2"})
 
         :param exe: executable to run
-        :type exe: str
-        :param exe_args: executable arguments, defaults to None
-        :type exe_args: str | list[str], optional
-        :param run_command: launch binary (e.g. "srun"), defaults to empty str
-        :type run_command: str, optional
-        :param run_args: arguments for run command (e.g. `-np` for `mpiexec`),
-            defaults to None
-        :type run_args: dict[str, str], optional
-        :param env_vars: environment vars to launch job with, defaults to None
-        :type env_vars: dict[str, str], optional
-        :param container: container type for workload (e.g. "singularity"),
-            defaults to None
-        :type container: Container, optional
+        :param exe_args: executable arguments
+        :param run_command: launch binary (e.g. "srun")
+        :param run_args: arguments for run command (e.g. `-np` for `mpiexec`)
+        :param env_vars: environment vars to launch job with
+        :param container: container type for workload (e.g. "singularity")
         """
         # Do not expand executable if running within a container
         self.exe = [exe] if container else [expand_exe_path(exe)]
         self.exe_args = exe_args or []
         self.run_args = run_args or {}
         self.env_vars = env_vars or {}
         self.container = container
@@ -113,286 +105,298 @@
                     t.Dict[str, str],
                 ],
             ]
         ] = None
 
     @property
     def exe_args(self) -> t.Union[str, t.List[str]]:
+        """Return an immutable list of attached executable arguments.
+
+        :returns: attached executable arguments
+        """
         return self._exe_args
 
     @exe_args.setter
     def exe_args(self, value: t.Union[str, t.List[str], None]) -> None:
+        """Set the executable arguments.
+
+        :param value: executable arguments
+        """
         self._exe_args = self._build_exe_args(value)
 
     @property
     def run_args(self) -> t.Dict[str, t.Union[int, str, float, None]]:
+        """Return an immutable list of attached run arguments.
+
+        :returns: attached run arguments
+        """
         return self._run_args
 
     @run_args.setter
     def run_args(self, value: t.Dict[str, t.Union[int, str, float, None]]) -> None:
+        """Set the run arguments.
+
+        :param value: run arguments
+        """
         self._run_args = copy.deepcopy(value)
 
     @property
     def env_vars(self) -> t.Dict[str, t.Optional[str]]:
+        """Return an immutable list of attached environment variables.
+
+        :returns: attached environment variables
+        """
         return self._env_vars
 
     @env_vars.setter
     def env_vars(self, value: t.Dict[str, t.Optional[str]]) -> None:
+        """Set the environment variables.
+
+        :param value: environment variables
+        """
         self._env_vars = copy.deepcopy(value)
 
     # To be overwritten by subclasses. Set of reserved args a user cannot change
     reserved_run_args = set()  # type: set[str]
 
     def set_nodes(self, nodes: int) -> None:
         """Set the number of nodes
 
         :param nodes: number of nodes to run with
-        :type nodes: int
         """
         logger.warning(
             (
                 "Node specification not implemented for this "
                 f"RunSettings type: {type(self)}"
             )
         )
 
     def set_tasks(self, tasks: int) -> None:
         """Set the number of tasks to launch
 
         :param tasks: number of tasks to launch
-        :type tasks: int
         """
         logger.warning(
             (
                 "Task specification not implemented for this "
                 f"RunSettings type: {type(self)}"
             )
         )
 
     def set_tasks_per_node(self, tasks_per_node: int) -> None:
         """Set the number of tasks per node
 
         :param tasks_per_node: number of tasks to launch per node
-        :type tasks_per_node: int
         """
         logger.warning(
             (
                 "Task per node specification not implemented for this "
                 f"RunSettings type: {type(self)}"
             )
         )
 
     def set_task_map(self, task_mapping: str) -> None:
         """Set a task mapping
 
         :param task_mapping: task mapping
-        :type task_mapping: str
         """
         logger.warning(
             (
                 "Task mapping specification not implemented for this "
                 f"RunSettings type: {type(self)}"
             )
         )
 
     def set_cpus_per_task(self, cpus_per_task: int) -> None:
         """Set the number of cpus per task
 
         :param cpus_per_task: number of cpus per task
-        :type cpus_per_task: int
         """
         logger.warning(
             (
                 "CPU per node specification not implemented for this "
                 f"RunSettings type: {type(self)}"
             )
         )
 
     def set_hostlist(self, host_list: t.Union[str, t.List[str]]) -> None:
         """Specify the hostlist for this job
 
         :param host_list: hosts to launch on
-        :type host_list: str | list[str]
         """
         logger.warning(
             (
                 "Hostlist specification not implemented for this "
                 f"RunSettings type: {type(self)}"
             )
         )
 
     def set_hostlist_from_file(self, file_path: str) -> None:
         """Use the contents of a file to specify the hostlist for this job
 
         :param file_path: Path to the hostlist file
-        :type file_path: str
         """
         logger.warning(
             (
                 "Hostlist from file specification not implemented for this "
                 f"RunSettings type: {type(self)}"
             )
         )
 
     def set_excluded_hosts(self, host_list: t.Union[str, t.List[str]]) -> None:
         """Specify a list of hosts to exclude for launching this job
 
         :param host_list: hosts to exclude
-        :type host_list: str | list[str]
         """
         logger.warning(
             (
                 "Excluded host list specification not implemented for this "
                 f"RunSettings type: {type(self)}"
             )
         )
 
     def set_cpu_bindings(self, bindings: t.Union[int, t.List[int]]) -> None:
         """Set the cores to which MPI processes are bound
 
         :param bindings: List specifing the cores to which MPI processes are bound
-        :type bindings: list[int] | int
         """
         logger.warning(
             (
                 "CPU binding specification not implemented for this "
                 f"RunSettings type: {type(self)}"
             )
         )
 
     def set_memory_per_node(self, memory_per_node: int) -> None:
         """Set the amount of memory required per node in megabytes
 
         :param memory_per_node: Number of megabytes per node
-        :type memory_per_node: int
         """
         logger.warning(
             (
                 "Memory per node specification not implemented for this "
                 f"RunSettings type: {type(self)}"
             )
         )
 
     def set_verbose_launch(self, verbose: bool) -> None:
         """Set the job to run in verbose mode
 
         :param verbose: Whether the job should be run verbosely
-        :type verbose: bool
         """
         logger.warning(
             (
                 "Verbose specification not implemented for this "
                 f"RunSettings type: {type(self)}"
             )
         )
 
     def set_quiet_launch(self, quiet: bool) -> None:
         """Set the job to run in quiet mode
 
         :param quiet: Whether the job should be run quietly
-        :type quiet: bool
         """
         logger.warning(
             (
                 "Quiet specification not implemented for this "
                 f"RunSettings type: {type(self)}"
             )
         )
 
     def set_broadcast(self, dest_path: t.Optional[str] = None) -> None:
         """Copy executable file to allocated compute nodes
 
         :param dest_path: Path to copy an executable file
-        :type dest_path: str | None
         """
         logger.warning(
             (
                 "Broadcast specification not implemented for this "
                 f"RunSettings type: {type(self)}"
             )
         )
 
     def set_time(self, hours: int = 0, minutes: int = 0, seconds: int = 0) -> None:
         """Automatically format and set wall time
 
         :param hours: number of hours to run job
-        :type hours: int
         :param minutes: number of minutes to run job
-        :type minutes: int
         :param seconds: number of seconds to run job
-        :type seconds: int
         """
         return self.set_walltime(
             self._fmt_walltime(int(hours), int(minutes), int(seconds))
         )
 
+    def set_node_feature(self, feature_list: t.Union[str, t.List[str]]) -> None:
+        """Specify the node feature for this job
+
+        :param feature_list: node feature to launch on
+        """
+        logger.warning(
+            (
+                "Feature specification not implemented for this "
+                f"RunSettings type: {type(self)}"
+            )
+        )
+
     @staticmethod
     def _fmt_walltime(hours: int, minutes: int, seconds: int) -> str:
         """Convert hours, minutes, and seconds into valid walltime format
 
         By defualt the formatted wall time is the total number of seconds.
 
         :param hours: number of hours to run job
-        :type hours: int
         :param minutes: number of minutes to run job
-        :type minutes: int
         :param seconds: number of seconds to run job
-        :type seconds: int
         :returns: Formatted walltime
-        :rtype: str
         """
         time_ = hours * 3600
         time_ += minutes * 60
         time_ += seconds
         return str(time_)
 
     def set_walltime(self, walltime: str) -> None:
         """Set the formatted walltime
 
         :param walltime: Time in format required by launcher``
-        :type walltime: str
         """
         logger.warning(
             (
                 "Walltime specification not implemented for this "
                 f"RunSettings type: {type(self)}"
             )
         )
 
     def set_binding(self, binding: str) -> None:
         """Set binding
 
         :param binding: Binding
-        :type binding: str
         """
         logger.warning(
             (
                 "binding specification not implemented for this "
                 f"RunSettings type: {type(self)}"
             )
         )
 
     def set_mpmd_preamble(self, preamble_lines: t.List[str]) -> None:
         """Set preamble to a file to make a job MPMD
 
         :param preamble_lines: lines to put at the beginning of a file.
-        :type preamble_lines: list[str]
         """
         logger.warning(
             (
                 "MPMD preamble specification not implemented for this "
                 f"RunSettings type: {type(self)}"
             )
         )
 
     def make_mpmd(self, settings: RunSettings) -> None:
         """Make job an MPMD job
 
         :param settings: ``RunSettings`` instance
-        :type settings: RunSettings
         """
         logger.warning(
             (
                 "Make MPMD specification not implemented for this "
                 f"RunSettings type: {type(self)}"
             )
         )
@@ -400,15 +404,14 @@
     @property
     def run_command(self) -> t.Optional[str]:
         """Return the launch binary used to launch the executable
 
         Attempt to expand the path to the executable if possible
 
         :returns: launch binary e.g. mpiexec
-        :type: str | None
         """
         cmd = self._run_command
 
         if cmd:
             if is_valid_cmd(cmd):
                 # command is valid and will be expanded
                 return expand_exe_path(cmd)
@@ -424,15 +427,14 @@
         To fully inherit the current user environment, add the
         workload-manager-specific flag to the launch command through the
         :meth:`add_exe_args` method. For example, ``--export=ALL`` for
         slurm, or ``-V`` for PBS/aprun.
 
 
         :param env_vars: environment variables to update or add
-        :type env_vars: dict[str, Union[str, int, float, bool]]
         :raises TypeError: if env_vars values cannot be coerced to strings
         """
         val_types = (str, int, float, bool)
         # Coerce env_vars values to str as a convenience to user
         for env, val in env_vars.items():
             if not isinstance(val, val_types):
                 raise TypeError(
@@ -441,24 +443,16 @@
 
             self.env_vars[env] = str(val)
 
     def add_exe_args(self, args: t.Union[str, t.List[str]]) -> None:
         """Add executable arguments to executable
 
         :param args: executable arguments
-        :type args: str | list[str]
-        :raises TypeError: if exe args are not strings
         """
-        if isinstance(args, str):
-            args = args.split()
-
-        for arg in args:
-            if not isinstance(arg, str):
-                raise TypeError("Executable arguments should be a list of str")
-
+        args = self._build_exe_args(args)
         self._exe_args.extend(args)
 
     def set(
         self, arg: str, value: t.Optional[str] = None, condition: bool = True
     ) -> None:
         """Allows users to set individual run arguments.
 
@@ -499,19 +493,16 @@
 
             rs.format_run_args()
             # returns ["exclusive", "None", "partition", "debug"] iff
               socket.gethostname()=="testing-system"
             # otherwise returns ["exclusive", "None"]
 
         :param arg: name of the argument
-        :type arg: str
         :param value: value of the argument
-        :type value: str | None
         :param conditon: set the argument if condition evaluates to True
-        :type condition: bool
         """
         if not isinstance(arg, str):
             raise TypeError("Argument name should be of type str")
         if value is not None and not isinstance(value, str):
             raise TypeError("Argument value should be of type str or None")
         arg = arg.strip().lstrip("-")
 
@@ -529,55 +520,53 @@
 
         if arg in self.run_args and value != self.run_args[arg]:
             logger.warning(f"Overwritting argument '{arg}' with value '{value}'")
         self.run_args[arg] = value
 
     @staticmethod
     def _build_exe_args(exe_args: t.Optional[t.Union[str, t.List[str]]]) -> t.List[str]:
-        """Convert exe_args input to a desired collection format"""
-        if exe_args:
-            if isinstance(exe_args, str):
-                return exe_args.split()
-            if isinstance(exe_args, list):
-                exe_args = copy.deepcopy(exe_args)
-                plain_type = all(isinstance(arg, (str)) for arg in exe_args)
-                if not plain_type:
-                    nested_type = all(
-                        all(isinstance(arg, (str)) for arg in exe_args_list)
-                        for exe_args_list in exe_args
-                    )
-                    if not nested_type:
-                        raise TypeError(
-                            "Executable arguments were not list of str or str"
-                        )
-                    return exe_args
-                return exe_args
-            raise TypeError("Executable arguments were not list of str or str")
-        return []
+        """Check and convert exe_args input to a desired collection format"""
+        if not exe_args:
+            return []
+
+        if isinstance(exe_args, list):
+            exe_args = copy.deepcopy(exe_args)
+
+        if not (
+            isinstance(exe_args, str)
+            or (
+                isinstance(exe_args, list)
+                and all(isinstance(arg, str) for arg in exe_args)
+            )
+        ):
+            raise TypeError("Executable arguments were not a list of str or a str.")
+
+        if isinstance(exe_args, str):
+            return exe_args.split()
+
+        return exe_args
 
     def format_run_args(self) -> t.List[str]:
         """Return formatted run arguments
 
         For ``RunSettings``, the run arguments are passed
         literally with no formatting.
 
         :return: list run arguments for these settings
-        :rtype: list[str]
         """
         formatted = []
         for arg, value in self.run_args.items():
             formatted.append(arg)
             formatted.append(str(value))
         return formatted
 
     def format_env_vars(self) -> t.List[str]:
         """Build environment variable string
 
         :returns: formatted list of strings to export variables
-        :rtype: list[str]
         """
         formatted = []
         for key, val in self.env_vars.items():
             if val is None:
                 formatted.append(f"{key}=")
             else:
                 formatted.append(f"{key}={val}")
@@ -615,27 +604,34 @@
         """Return the batch command
 
         Tests to see if we can expand the batch command
         path. If we can, then returns the expanded batch
         command. If we cannot, returns the batch command as is.
 
         :returns: batch command
-        :type: str
         """
         if is_valid_cmd(self._batch_cmd):
             return expand_exe_path(self._batch_cmd)
 
         return self._batch_cmd
 
     @property
     def batch_args(self) -> t.Dict[str, t.Optional[str]]:
+        """Retrieve attached batch arguments
+
+        :returns: attached batch arguments
+        """
         return self._batch_args
 
     @batch_args.setter
     def batch_args(self, value: t.Dict[str, t.Optional[str]]) -> None:
+        """Attach batch arguments
+
+        :param value: dictionary of batch arguments
+        """
         self._batch_args = copy.deepcopy(value) if value else {}
 
     def set_nodes(self, num_nodes: int) -> None:
         raise NotImplementedError
 
     def set_hostlist(self, host_list: t.Union[str, t.List[str]]) -> None:
         raise NotImplementedError
@@ -652,37 +648,38 @@
     def format_batch_args(self) -> t.List[str]:
         raise NotImplementedError
 
     def set_batch_command(self, command: str) -> None:
         """Set the command used to launch the batch e.g. ``sbatch``
 
         :param command: batch command
-        :type command: str
         """
         self._batch_cmd = command
 
     def add_preamble(self, lines: t.List[str]) -> None:
         """Add lines to the batch file preamble. The lines are just
         written (unmodified) at the beginning of the batch file
         (after the WLM directives) and can be used to e.g.
         start virtual environments before running the executables.
 
         :param line: lines to add to preamble.
-        :type line: str or list[str]
         """
         if isinstance(lines, str):
             self._preamble += [lines]
         elif isinstance(lines, list):
             self._preamble += lines
         else:
             raise TypeError("Expected str or List[str] for lines argument")
 
     @property
     def preamble(self) -> t.Iterable[str]:
-        """Return an iterable of preamble clauses to be prepended to the batch file"""
+        """Return an iterable of preamble clauses to be prepended to the batch file
+
+        :return: attached preamble clauses
+        """
         return (clause for clause in self._preamble)
 
     def __str__(self) -> str:  # pragma: no-cover
         string = f"Batch Command: {self._batch_cmd}"
         if self.batch_args:
             string += f"\nBatch arguments:\n{fmt_dict(self.batch_args)}"
         return string
```

### Comparing `smartsim-0.6.2/smartsim/settings/containers.py` & `smartsim-0.7.0/smartsim/settings/containers.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,21 +35,17 @@
 class Container:
     """Base class for container types in SmartSim.
 
     Container types are used to embed all the information needed to
     launch a workload within a container into a single object.
 
     :param image: local or remote path to container image
-    :type image: str
     :param args: arguments to container command
-    :type args: str | list[str], optional
     :param mount: paths to mount (bind) from host machine into image.
-    :type mount: str | list[str] | dict[str, str], optional
     :param working_directory: path of the working directory within the container
-    :type working_directory: str
     """
 
     def __init__(
         self, image: str, args: str = "", mount: str = "", working_directory: str = ""
     ) -> None:
         # Validate types
         if not isinstance(image, str):
@@ -66,15 +62,14 @@
         self.mount = mount
         self.working_directory = working_directory
 
     def _containerized_run_command(self, run_command: str) -> str:
         """Return modified run_command with container commands prepended.
 
         :param run_command: run command from a RunSettings class
-        :type run_command: str
         """
         raise NotImplementedError(
             "Containerized run command specification not implemented for this "
             f"Container type: {type(self)}"
         )
 
 
@@ -95,19 +90,16 @@
         disabled by a
         `system administrator
         <https://apptainer.org/docs/admin/1.0/configfiles.html#bind-mount-management>`_
 
 
     :param image: local or remote path to container image,
         e.g. ``docker://sylabsio/lolcow``
-    :type image: str
     :param args: arguments to 'singularity exec' command
-    :type args: str | list[str], optional
     :param mount: paths to mount (bind) from host machine into image.
-    :type mount: str | list[str] | dict[str, str], optional
     """
 
     def __init__(self, *args: t.Any, **kwargs: t.Any) -> None:
         super().__init__(*args, **kwargs)
 
     def _container_cmds(self, default_working_directory: str = "") -> t.List[str]:
         """Return list of container commands to be inserted before exe.
```

### Comparing `smartsim-0.6.2/smartsim/settings/lsfSettings.py` & `smartsim-0.7.0/smartsim/settings/lsfSettings.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,21 +47,17 @@
         **_kwargs: t.Any,
     ) -> None:
         """Settings to run job with ``jsrun`` command
 
         ``JsrunSettings`` should only be used on LSF-based systems.
 
         :param exe: executable
-        :type exe: str
-        :param exe_args: executable arguments, defaults to None
-        :type exe_args: str | list[str], optional
-        :param run_args: arguments for run command, defaults to None
-        :type run_args: dict[str, t.Union[int, str, float, None]], optional
-        :param env_vars: environment vars to launch job with, defaults to None
-        :type env_vars: dict[str, str], optional
+        :param exe_args: executable arguments
+        :param run_args: arguments for run command
+        :param env_vars: environment vars to launch job with
         """
         super().__init__(
             exe,
             exe_args,
             run_command="jsrun",
             run_args=run_args,
             env_vars=env_vars,
@@ -77,28 +73,26 @@
 
     def set_num_rs(self, num_rs: t.Union[str, int]) -> None:
         """Set the number of resource sets to use
 
         This sets ``--nrs``.
 
         :param num_rs: Number of resource sets or `ALL_HOSTS`
-        :type num_rs: int or str
         """
         if isinstance(num_rs, str):
             self.run_args["nrs"] = num_rs
         else:
             self.run_args["nrs"] = int(num_rs)
 
     def set_cpus_per_rs(self, cpus_per_rs: int) -> None:
         """Set the number of cpus to use per resource set
 
         This sets ``--cpu_per_rs``
 
         :param cpus_per_rs: number of cpus to use per resource set or ALL_CPUS
-        :type cpus_per_rs: int or str
         """
         if self.colocated_db_settings:
             db_cpus = int(t.cast(int, self.colocated_db_settings.get("db_cpus", 0)))
             if not db_cpus:
                 raise ValueError("db_cpus must be configured on colocated_db_settings")
 
             if cpus_per_rs < db_cpus:
@@ -113,111 +107,101 @@
 
     def set_gpus_per_rs(self, gpus_per_rs: int) -> None:
         """Set the number of gpus to use per resource set
 
         This sets ``--gpu_per_rs``
 
         :param gpus_per_rs: number of gpus to use per resource set or ALL_GPUS
-        :type gpus_per_rs: int or str
         """
         if isinstance(gpus_per_rs, str):
             self.run_args["gpu_per_rs"] = gpus_per_rs
         else:
             self.run_args["gpu_per_rs"] = int(gpus_per_rs)
 
     def set_rs_per_host(self, rs_per_host: int) -> None:
         """Set the number of resource sets to use per host
 
         This sets ``--rs_per_host``
 
         :param rs_per_host: number of resource sets to use per host
-        :type rs_per_host: int
         """
         self.run_args["rs_per_host"] = int(rs_per_host)
 
     def set_tasks(self, tasks: int) -> None:
         """Set the number of tasks for this job
 
         This sets ``--np``
 
         :param tasks: number of tasks
-        :type tasks: int
         """
         self.run_args["np"] = int(tasks)
 
     def set_tasks_per_rs(self, tasks_per_rs: int) -> None:
         """Set the number of tasks per resource set
 
         This sets ``--tasks_per_rs``
 
         :param tasks_per_rs: number of tasks per resource set
-        :type tasks_per_rs: int
         """
         self.run_args["tasks_per_rs"] = int(tasks_per_rs)
 
     def set_tasks_per_node(self, tasks_per_node: int) -> None:
         """Set the number of tasks per resource set.
 
         This function is an alias for `set_tasks_per_rs`.
 
         :param tasks_per_node: number of tasks per resource set
-        :type tasks_per_node: int
         """
         self.set_tasks_per_rs(int(tasks_per_node))
 
     def set_cpus_per_task(self, cpus_per_task: int) -> None:
         """Set the number of cpus per tasks.
 
         This function is an alias for `set_cpus_per_rs`.
 
         :param cpus_per_task: number of cpus per resource set
-        :type cpus_per_task: int
         """
         self.set_cpus_per_rs(int(cpus_per_task))
 
     def set_memory_per_rs(self, memory_per_rs: int) -> None:
         """Specify the number of megabytes of memory to assign to a resource set
 
         This sets ``--memory_per_rs``
 
         :param memory_per_rs: Number of megabytes per rs
-        :type memory_per_rs: int
         """
         self.run_args["memory_per_rs"] = int(memory_per_rs)
 
     def set_memory_per_node(self, memory_per_node: int) -> None:
         """Specify the number of megabytes of memory to assign to a resource set
 
         Alias for `set_memory_per_rs`.
 
         :param memory_per_node: Number of megabytes per rs
-        :type memory_per_node: int
         """
         self.set_memory_per_rs(int(memory_per_node))
 
     def set_binding(self, binding: str) -> None:
         """Set binding
 
         This sets ``--bind``
 
         :param binding: Binding, e.g. `packed:21`
-        :type binding: str
         """
         self.run_args["bind"] = binding
 
     def make_mpmd(self, settings: RunSettings) -> None:
         """Make step an MPMD (or SPMD) job.
 
         This method will activate job execution through an ERF file.
 
         Optionally, this method adds an instance of ``JsrunSettings`` to
         the list of settings to be launched in the same ERF file.
 
         :param settings: ``JsrunSettings`` instance
-        :type settings: JsrunSettings, optional
         """
         if self.colocated_db_settings:
             raise SSUnsupportedError(
                 "Colocated models cannot be run as a mpmd workload"
             )
 
         self.mpmd.append(settings)
@@ -227,15 +211,14 @@
         `oversubscribe-cpu : allow` or `overlapping-rs : allow`.
         Can be used to set `launch_distribution`. If it is not present,
         it will be inferred from the settings, or set to `packed` by
         default.
 
         :param preamble_lines: lines to put at the beginning of the ERF
                                file.
-        :type preamble_lines: list[str]
         """
         self.mpmd_preamble_lines = preamble_lines
 
     def set_erf_sets(self, erf_sets: t.Dict[str, str]) -> None:
         """Set resource sets used for ERF (SPMD or MPMD) steps.
 
         ``erf_sets`` is a dictionary used to fill the ERF
@@ -245,25 +228,23 @@
         and memory.
         The key `rank` is used to give specific ranks, as in
         `{"rank": "1, 2, 5"}`, while the key `rank_count` is used to specify
         the count only, as in `{"rank_count": "3"}`. If both are specified,
         only `rank` is used.
 
         :param hosts: dictionary of resources
-        :type hosts: dict[str,str]
         """
         self.erf_sets = copy.deepcopy(erf_sets)
 
     def format_env_vars(self) -> t.List[str]:
         """Format environment variables. Each variable needs
         to be passed with ``--env``. If a variable is set to ``None``,
         its value is propagated from the current environment.
 
         :returns: formatted list of strings to export variables
-        :rtype: list[str]
         """
         format_str = []
         for k, v in self.env_vars.items():
             if v:
                 format_str += ["-E", f"{k}={v}"]
             else:
                 format_str += ["-E", f"{k}"]
@@ -275,26 +256,23 @@
         This sets ``--stdio_mode individual``
         and inserts the suffix into the output name. The resulting
         output name will be ``self.name + suffix + .out``.
 
         :param suffix: Optional suffix to add to output file names,
                        it can contain `%j`, `%h`, `%p`, or `%t`,
                        as specified by `jsrun` options.
-        :type suffix: str, optional
-
         """
         self.run_args["stdio_mode"] = "individual"
         if suffix:
             self.individual_suffix = suffix
 
     def format_run_args(self) -> t.List[str]:
         """Return a list of LSF formatted run arguments
 
         :return: list of LSF arguments for these settings
-        :rtype: list[str]
         """
         # args launcher uses
         args = []
         restricted = ["chdir", "h", "stdio_stdout", "o", "stdio_stderr", "k"]
         if self.mpmd or "erf_input" in self.run_args.keys():
             restricted.extend(
                 [
@@ -399,24 +377,19 @@
         project: t.Optional[str] = None,
         batch_args: t.Optional[t.Dict[str, t.Optional[str]]] = None,
         smts: int = 0,
         **kwargs: t.Any,
     ) -> None:
         """Specify ``bsub`` batch parameters for a job
 
-        :param nodes: number of nodes for batch, defaults to None
-        :type nodes: int, optional
-        :param time: walltime for batch job in format hh:mm, defaults to None
-        :type time: str, optional
-        :param project: project for batch launch, defaults to None
-        :type project: str, optional
-        :param batch_args: overrides for LSF batch arguments, defaults to None
-        :type batch_args: dict[str, str], optional
-        :param smts: SMTs, defaults to 0
-        :type smts: int, optional
+        :param nodes: number of nodes for batch
+        :param time: walltime for batch job in format hh:mm
+        :param project: project for batch launch
+        :param batch_args: overrides for LSF batch arguments
+        :param smts: SMTs
         """
         self.project: t.Optional[str] = None
 
         if project:
             kwargs.pop("account", None)
         else:
             project = kwargs.pop("account", None)
@@ -441,15 +414,14 @@
         """Set the walltime
 
         This sets ``-W``.
 
         :param walltime: Time in hh:mm format, e.g. "10:00" for 10 hours,
                          if time is supplied in hh:mm:ss format, seconds
                          will be ignored and walltime will be set as ``hh:mm``
-        :type walltime: str
         """
         # For compatibility with other launchers, as explained in docstring
         if walltime:
             if len(walltime.split(":")) > 2:
                 walltime = ":".join(walltime.split(":")[:2])
         self.walltime = walltime
 
@@ -457,67 +429,65 @@
         """Set SMTs
 
         This sets ``-alloc_flags``. If the user sets
         SMT explicitly through ``-alloc_flags``, then that
         takes precedence.
 
         :param smts: SMT (e.g on Summit: 1, 2, or 4)
-        :type smts: int
         """
         self.smts = smts
 
     def set_project(self, project: str) -> None:
         """Set the project
 
         This sets ``-P``.
 
         :param time: project name
-        :type time: str
         """
         if project:
             self.project = project
 
     def set_account(self, account: str) -> None:
         """Set the project
 
         this function is an alias for `set_project`.
 
         :param account: project name
-        :type account: str
         """
         self.set_project(account)
 
     def set_nodes(self, num_nodes: int) -> None:
         """Set the number of nodes for this batch job
 
         This sets ``-nnodes``.
 
         :param nodes: number of nodes
-        :type nodes: int
         """
         if num_nodes:
             self.batch_args["nnodes"] = str(int(num_nodes))
 
     def set_expert_mode_req(self, res_req: str, slots: int) -> None:
         """Set allocation for expert mode. This
         will activate expert mode (``-csm``) and
         disregard all other allocation options.
 
         This sets ``-csm -n slots -R res_req``
+
+        :param res_req: specific resource requirements
+        :param slots: number of resources to allocate
         """
         self.expert_mode = True
         self.batch_args["csm"] = "y"
         self.batch_args["R"] = res_req
         self.batch_args["n"] = str(slots)
 
     def set_hostlist(self, host_list: t.Union[str, t.List[str]]) -> None:
         """Specify the hostlist for this job
 
         :param host_list: hosts to launch on
-        :type host_list: str | list[str]
         :raises TypeError: if not str or list of str
         """
         if isinstance(host_list, str):
             host_list = [host_list.strip()]
         if not isinstance(host_list, list):
             raise TypeError("host_list argument must be a list of strings")
         if not all(isinstance(host, str) for host in host_list):
@@ -526,23 +496,21 @@
 
     def set_tasks(self, tasks: int) -> None:
         """Set the number of tasks for this job
 
         This sets ``-n``
 
         :param tasks: number of tasks
-        :type tasks: int
         """
         self.batch_args["n"] = str(int(tasks))
 
     def set_queue(self, queue: str) -> None:
         """Set the queue for this job
 
         :param queue: The queue to submit the job on
-        :type queue: str
         """
         if queue:
             self.batch_args["q"] = queue
 
     def _format_alloc_flags(self) -> None:
         """Format ``alloc_flags`` checking if user already
         set it. Currently only adds SMT flag if missing
@@ -569,15 +537,14 @@
             if len(flags) > 1:
                 self.batch_args["alloc_flags"] = '"' + " ".join(flags) + '"'
 
     def format_batch_args(self) -> t.List[str]:
         """Get the formatted batch arguments for a preview
 
         :return: list of batch arguments for Qsub
-        :rtype: list[str]
         """
         opts = []
 
         self._format_alloc_flags()
 
         for opt, value in self.batch_args.items():
             if self.expert_mode and opt in self.easy_settings:
```

### Comparing `smartsim-0.6.2/smartsim/settings/mpiSettings.py` & `smartsim-0.7.0/smartsim/settings/mpiSettings.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,24 +57,19 @@
         environment
 
         Any arguments passed in the ``run_args`` dict will be converted
         command line arguments and prefixed with ``--``. Values of
         None can be provided for arguments that do not have values.
 
         :param exe: executable
-        :type exe: str
-        :param exe_args: executable arguments, defaults to None
-        :type exe_args: str | list[str], optional
-        :param run_args: arguments for run command, defaults to None
-        :type run_args: dict[str, str], optional
-        :param env_vars: environment vars to launch job with, defaults to None
-        :type env_vars: dict[str, str], optional
+        :param exe_args: executable arguments
+        :param run_args: arguments for run command
+        :param env_vars: environment vars to launch job with
         :param fail_if_missing_exec: Throw an exception of the MPI command
                                      is missing. Otherwise, throw a warning
-        :type fail_if_missing_exec: bool, optional
         """
         super().__init__(
             exe,
             exe_args,
             run_command=run_command,
             run_args=run_args,
             env_vars=env_vars,
@@ -97,15 +92,14 @@
     def make_mpmd(self, settings: RunSettings) -> None:
         """Make a mpmd workload by combining two ``mpirun`` commands
 
         This connects the two settings to be executed with a single
         Model instance
 
         :param settings: MpirunSettings instance
-        :type settings: MpirunSettings
         """
         if self.colocated_db_settings:
             raise SSUnsupportedError(
                 "Colocated models cannot be run as a mpmd workload"
             )
         self.mpmd.append(settings)
 
@@ -113,66 +107,60 @@
         """Set ``mpirun`` task mapping
 
         this sets ``--map-by <mapping>``
 
         For examples, see the man page for ``mpirun``
 
         :param task_mapping: task mapping
-        :type task_mapping: str
         """
         self.run_args["map-by"] = task_mapping
 
     def set_cpus_per_task(self, cpus_per_task: int) -> None:
         """Set the number of tasks for this job
 
         This sets ``--cpus-per-proc`` for MPI compliant implementations
 
         note: this option has been deprecated in openMPI 4.0+
         and will soon be replaced.
 
         :param cpus_per_task: number of tasks
-        :type cpus_per_task: int
         """
         self.run_args["cpus-per-proc"] = int(cpus_per_task)
 
     def set_cpu_binding_type(self, bind_type: str) -> None:
         """Specifies the cores to which MPI processes are bound
 
         This sets ``--bind-to`` for MPI compliant implementations
 
         :param bind_type: binding type
-        :type bind_type: str
         """
         self.run_args["bind-to"] = bind_type
 
     def set_tasks_per_node(self, tasks_per_node: int) -> None:
         """Set the number of tasks per node
 
         :param tasks_per_node: number of tasks to launch per node
-        :type tasks_per_node: int
         """
         self.run_args["npernode"] = int(tasks_per_node)
 
     def set_tasks(self, tasks: int) -> None:
         """Set the number of tasks for this job
 
         This sets ``-n`` for MPI compliant implementations
 
         :param tasks: number of tasks
-        :type tasks: int
         """
         self.run_args["n"] = int(tasks)
 
     def set_hostlist(self, host_list: t.Union[str, t.List[str]]) -> None:
         """Set the hostlist for the ``mpirun`` command
 
         This sets ``--host``
 
         :param host_list: list of host names
-        :type host_list: str | list[str]
         :raises TypeError: if not str or list of str
         """
         if isinstance(host_list, str):
             host_list = [host_list.strip()]
         if not isinstance(host_list, list):
             raise TypeError("host_list argument must be a list of strings")
         if not all(isinstance(host, str) for host in host_list):
@@ -181,51 +169,47 @@
 
     def set_hostlist_from_file(self, file_path: str) -> None:
         """Use the contents of a file to set the hostlist
 
         This sets ``--hostfile``
 
         :param file_path: Path to the hostlist file
-        :type file_path: str
         """
         self.run_args["hostfile"] = file_path
 
     def set_verbose_launch(self, verbose: bool) -> None:
         """Set the job to run in verbose mode
 
         This sets ``--verbose``
 
         :param verbose: Whether the job should be run verbosely
-        :type verbose: bool
         """
         if verbose:
             self.run_args["verbose"] = None
         else:
             self.run_args.pop("verbose", None)
 
     def set_quiet_launch(self, quiet: bool) -> None:
         """Set the job to run in quiet mode
 
         This sets ``--quiet``
 
         :param quiet: Whether the job should be run quietly
-        :type quiet: bool
         """
         if quiet:
             self.run_args["quiet"] = None
         else:
             self.run_args.pop("quiet", None)
 
     def set_broadcast(self, dest_path: t.Optional[str] = None) -> None:
         """Copy the specified executable(s) to remote machines
 
         This sets ``--preload-binary``
 
         :param dest_path: Destination path (Ignored)
-        :type dest_path: str | None
         """
         if dest_path is not None and isinstance(dest_path, str):
             logger.warning(
                 (
                     f"{type(self)} cannot set a destination path during broadcast. "
                     "Using session directory instead"
                 )
@@ -234,23 +218,21 @@
 
     def set_walltime(self, walltime: str) -> None:
         """Set the maximum number of seconds that a job will run
 
         This sets ``--timeout``
 
         :param walltime: number like string of seconds that a job will run in secs
-        :type walltime: str
         """
         self.run_args["timeout"] = walltime
 
     def format_run_args(self) -> t.List[str]:
         """Return a list of MPI-standard formatted run arguments
 
         :return: list of MPI-standard arguments for these settings
-        :rtype: list[str]
         """
         # args launcher uses
         args = []
         restricted = ["wdir", "wd"]
 
         for opt, value in self.run_args.items():
             if opt not in restricted:
@@ -261,15 +243,14 @@
                     args += [prefix + opt, str(value)]
         return args
 
     def format_env_vars(self) -> t.List[str]:
         """Format the environment variables for mpirun
 
         :return: list of env vars
-        :rtype: list[str]
         """
         formatted = []
         env_string = "-x"
 
         if self.env_vars:
             for name, value in self.env_vars.items():
                 if value:
@@ -295,21 +276,17 @@
         environment
 
         Any arguments passed in the ``run_args`` dict will be converted
         into ``mpirun`` arguments and prefixed with ``--``. Values of
         None can be provided for arguments that do not have values.
 
         :param exe: executable
-        :type exe: str
-        :param exe_args: executable arguments, defaults to None
-        :type exe_args: str | list[str], optional
-        :param run_args: arguments for run command, defaults to None
-        :type run_args: dict[str, t.Union[int, str, float, None]], optional
-        :param env_vars: environment vars to launch job with, defaults to None
-        :type env_vars: dict[str, str], optional
+        :param exe_args: executable arguments
+        :param run_args: arguments for run command
+        :param env_vars: environment vars to launch job with
         """
         super().__init__(exe, exe_args, "mpirun", run_args, env_vars, **kwargs)
 
 
 class MpiexecSettings(_BaseMPISettings):
     def __init__(
         self,
@@ -326,21 +303,17 @@
         environment
 
         Any arguments passed in the ``run_args`` dict will be converted
         into ``mpiexec`` arguments and prefixed with ``--``. Values of
         None can be provided for arguments that do not have values.
 
         :param exe: executable
-        :type exe: str
-        :param exe_args: executable arguments, defaults to None
-        :type exe_args: str | list[str], optional
-        :param run_args: arguments for run command, defaults to None
-        :type run_args: dict[str, t.Union[int, str, float, None]], optional
-        :param env_vars: environment vars to launch job with, defaults to None
-        :type env_vars: dict[str, str], optional
+        :param exe_args: executable arguments
+        :param run_args: arguments for run command
+        :param env_vars: environment vars to launch job with
         """
         super().__init__(exe, exe_args, "mpiexec", run_args, env_vars, **kwargs)
 
         completed_process = subprocess.run(
             [self._run_command, "--help"], capture_output=True, check=False
         )
         help_statement = completed_process.stdout.decode()
@@ -366,16 +339,12 @@
         environment
 
         Any arguments passed in the ``run_args`` dict will be converted
         into ``orterun`` arguments and prefixed with ``--``. Values of
         None can be provided for arguments that do not have values.
 
         :param exe: executable
-        :type exe: str
-        :param exe_args: executable arguments, defaults to None
-        :type exe_args: str | list[str], optional
-        :param run_args: arguments for run command, defaults to None
-        :type run_args: dict[str, t.Union[int, str, float, None]], optional
-        :param env_vars: environment vars to launch job with, defaults to None
-        :type env_vars: dict[str, str], optional
+        :param exe_args: executable arguments
+        :param run_args: arguments for run command
+        :param env_vars: environment vars to launch job with
         """
         super().__init__(exe, exe_args, "orterun", run_args, env_vars, **kwargs)
```

### Comparing `smartsim-0.6.2/smartsim/settings/mpirunSettings.py` & `smartsim-0.7.0/smartsim/_core/launcher/util/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,23 +19,7 @@
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
-from warnings import simplefilter, warn
-
-from ..log import get_logger
-
-# pylint: disable-next=unused-import
-from .mpiSettings import MpiexecSettings, MpirunSettings, OrterunSettings
-
-logger = get_logger(__name__)
-
-simplefilter("once", DeprecationWarning)
-warn(
-    "mpirunSettings will be deprecated; use mpiSettings instead.",
-    DeprecationWarning,
-    stacklevel=2,
-)
```

### Comparing `smartsim-0.6.2/smartsim/settings/palsSettings.py` & `smartsim-0.7.0/smartsim/settings/palsSettings.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,21 +41,17 @@
     environment
 
     Any arguments passed in the ``run_args`` dict will be converted
     into ``mpiexec`` arguments and prefixed with ``--``. Values of
     None can be provided for arguments that do not have values.
 
     :param exe: executable
-    :type exe: str
-    :param exe_args: executable arguments, defaults to None
-    :type exe_args: str | list[str], optional
-    :param run_args: arguments for run command, defaults to None
-    :type run_args: dict[str, str], optional
-    :param env_vars: environment vars to launch job with, defaults to None
-    :type env_vars: dict[str, str], optional
+    :param exe_args: executable arguments
+    :param run_args: arguments for run command
+    :param env_vars: environment vars to launch job with
     """
 
     def __init__(
         self,
         exe: str,
         exe_args: t.Optional[t.Union[str, t.List[str]]] = None,
         run_args: t.Optional[t.Dict[str, t.Union[int, str, float, None]]] = None,
@@ -70,24 +66,19 @@
         environment
 
         Any arguments passed in the ``run_args`` dict will be converted
         command line arguments and prefixed with ``--``. Values of
         None can be provided for arguments that do not have values.
 
         :param exe: executable
-        :type exe: str
-        :param exe_args: executable arguments, defaults to None
-        :type exe_args: str | list[str], optional
-        :param run_args: arguments for run command, defaults to None
-        :type run_args: dict[str, t.Union[int, str, float, None]], optional
-        :param env_vars: environment vars to launch job with, defaults to None
-        :type env_vars: dict[str, str], optional
+        :param exe_args: executable arguments
+        :param run_args: arguments for run command
+        :param env_vars: environment vars to launch job with
         :param fail_if_missing_exec: Throw an exception of the MPI command
                                      is missing. Otherwise, throw a warning
-        :type fail_if_missing_exec: bool, optional
         """
         super().__init__(
             exe,
             exe_args,
             run_command="mpiexec",
             run_args=run_args,
             env_vars=env_vars,
@@ -99,108 +90,98 @@
         """Set ``mpirun`` task mapping
 
         this sets ``--map-by <mapping>``
 
         For examples, see the man page for ``mpirun``
 
         :param task_mapping: task mapping
-        :type task_mapping: str
         """
         logger.warning("set_task_map not supported under PALS")
 
     def set_cpus_per_task(self, cpus_per_task: int) -> None:
         """Set the number of tasks for this job
 
         This sets ``--cpus-per-proc`` for MPI compliant implementations
 
         note: this option has been deprecated in openMPI 4.0+
         and will soon be replaced.
 
         :param cpus_per_task: number of tasks
-        :type cpus_per_task: int
         """
         logger.warning("set_cpus_per_task not supported under PALS")
 
     def set_cpu_binding_type(self, bind_type: str) -> None:
         """Specifies the cores to which MPI processes are bound
 
         This sets ``--bind-to`` for MPI compliant implementations
 
         :param bind_type: binding type
-        :type bind_type: str
         """
         self.run_args["cpu-bind"] = bind_type
 
     def set_tasks(self, tasks: int) -> None:
         """Set the number of tasks
 
         :param tasks: number of total tasks to launch
-        :type tasks: int
         """
         self.run_args["np"] = int(tasks)
 
     def set_tasks_per_node(self, tasks_per_node: int) -> None:
         """Set the number of tasks per node
 
         :param tasks_per_node: number of tasks to launch per node
-        :type tasks_per_node: int
         """
         self.run_args["ppn"] = int(tasks_per_node)
 
     def set_quiet_launch(self, quiet: bool) -> None:
         """Set the job to run in quiet mode
 
         This sets ``--quiet``
 
         :param quiet: Whether the job should be run quietly
-        :type quiet: bool
         """
 
         logger.warning("set_quiet_launch not supported under PALS")
 
     def set_broadcast(self, dest_path: t.Optional[str] = None) -> None:
         """Copy the specified executable(s) to remote machines
 
         This sets ``--preload-binary``
 
         :param dest_path: Destination path (Ignored)
-        :type dest_path: str | None
         """
         if dest_path is not None and isinstance(dest_path, str):
             logger.warning(
                 (
                     f"{type(self)} cannot set a destination path during broadcast. "
                     "Using session directory instead"
                 )
             )
         self.run_args["transfer"] = None
 
     def set_walltime(self, walltime: str) -> None:
         """Set the maximum number of seconds that a job will run
 
         :param walltime: number like string of seconds that a job will run in secs
-        :type walltime: str
         """
         logger.warning("set_walltime not supported under PALS")
 
     def set_gpu_affinity_script(self, affinity: str, *args: t.Any) -> None:
         """Set the GPU affinity through a bash script
 
         :param affinity: path to the affinity script
-        :type affinity: str
         """
         self.affinity_script.append(str(affinity))
         for arg in args:
             self.affinity_script.append(str(arg))
 
     def format_run_args(self) -> t.List[str]:
         """Return a list of MPI-standard formatted run arguments
 
         :return: list of MPI-standard arguments for these settings
-        :rtype: list[str]
         """
         # args launcher uses
         args = []
         restricted = ["wdir", "wd"]
 
         for opt, value in self.run_args.items():
             if opt not in restricted:
@@ -215,15 +196,14 @@
 
         return args
 
     def format_env_vars(self) -> t.List[str]:
         """Format the environment variables for mpirun
 
         :return: list of env vars
-        :rtype: list[str]
         """
         formatted = []
 
         export_vars = []
         if self.env_vars:
             for name, value in self.env_vars.items():
                 if value:
@@ -238,15 +218,14 @@
 
     def set_hostlist(self, host_list: t.Union[str, t.List[str]]) -> None:
         """Set the hostlist for the PALS ``mpiexec`` command
 
         This sets ``--hosts``
 
         :param host_list: list of host names
-        :type host_list: str | list[str]
         :raises TypeError: if not str or list of str
         """
         if isinstance(host_list, str):
             host_list = [host_list.strip()]
         if not isinstance(host_list, list):
             raise TypeError("host_list argument must be a list of strings")
         if not all(isinstance(host, str) for host in host_list):
```

### Comparing `smartsim-0.6.2/smartsim/settings/pbsSettings.py` & `smartsim-0.7.0/smartsim/settings/pbsSettings.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,28 +49,21 @@
 
         ``nodes``, and ``ncpus`` are used to create the
         select statement for PBS if a select statement is not
         included in the ``resources``. If both are supplied
         the value for select statement supplied in ``resources``
         will override.
 
-        :param nodes: number of nodes for batch, defaults to None
-        :type nodes: int, optional
-        :param ncpus: number of cpus per node, defaults to None
-        :type ncpus: int, optional
-        :param time: walltime for batch job, defaults to None
-        :type time: str, optional
-        :param queue: queue to run batch in, defaults to None
-        :type queue: str, optional
-        :param account: account for batch launch, defaults to None
-        :type account: str, optional
-        :param resources: overrides for resource arguments, defaults to None
-        :type resources: dict[str, str], optional
-        :param batch_args: overrides for PBS batch arguments, defaults to None
-        :type batch_args: dict[str, str], optional
+        :param nodes: number of nodes for batch
+        :param ncpus: number of cpus per node
+        :param time: walltime for batch job
+        :param queue: queue to run batch in
+        :param account: account for batch launch
+        :param resources: overrides for resource arguments
+        :param batch_args: overrides for PBS batch arguments
         """
 
         self._ncpus = ncpus
 
         self.resources = resources or {}
         resource_nodes = self.resources.get("nodes", None)
 
@@ -108,25 +101,23 @@
         In PBS, 'select' is the more primitive way of describing how
         many nodes to allocate for the job. 'nodes' is equivalent to
         'select' with a 'place' statement. Assuming that only advanced
         users would use 'set_resource' instead, defining the number of
         nodes here is sets the 'nodes' resource.
 
         :param num_nodes: number of nodes
-        :type num_nodes: int
         """
 
         if num_nodes:
             self.set_resource("nodes", num_nodes)
 
     def set_hostlist(self, host_list: t.Union[str, t.List[str]]) -> None:
         """Specify the hostlist for this job
 
         :param host_list: hosts to launch on
-        :type host_list: str | list[str]
         :raises TypeError: if not str or list of str
         """
         if isinstance(host_list, str):
             host_list = [host_list.strip()]
         if not isinstance(host_list, list):
             raise TypeError("host_list argument must be a list of strings")
         if not all(isinstance(host, str) for host in host_list):
@@ -139,72 +130,65 @@
         format = "HH:MM:SS"
 
         If a walltime argument is provided in
         ``QsubBatchSettings.resources``, then
         this value will be overridden
 
         :param walltime: wall time
-        :type walltime: str
         """
         if walltime:
             self.set_resource("walltime", walltime)
 
     def set_queue(self, queue: str) -> None:
         """Set the queue for the batch job
 
         :param queue: queue name
-        :type queue: str
         """
         if queue:
             self.batch_args["q"] = str(queue)
 
     def set_ncpus(self, num_cpus: t.Union[int, str]) -> None:
         """Set the number of cpus obtained in each node.
 
         If a select argument is provided in
         ``QsubBatchSettings.resources``, then
         this value will be overridden
 
         :param num_cpus: number of cpus per node in select
-        :type num_cpus: int
         """
         self._ncpus = int(num_cpus)
 
     def set_account(self, account: str) -> None:
         """Set the account for this batch job
 
         :param acct: account id
-        :type acct: str
         """
         if account:
             self.batch_args["A"] = str(account)
 
     def set_resource(self, resource_name: str, value: t.Union[str, int]) -> None:
         """Set a resource value for the Qsub batch
 
         If a select statement is provided, the nodes and ncpus
         arguments will be overridden. Likewise for Walltime
 
         :param resource_name: name of resource, e.g. walltime
-        :type resource_name: str
         :param value: value
-        :type value: str
         """
         # TODO add error checking here
         # TODO include option to overwrite place (warning for orchestrator?)
         updated_dict = self.resources
         updated_dict.update({resource_name: value})
         self._sanity_check_resources(updated_dict)
         self.resources = updated_dict
 
     def format_batch_args(self) -> t.List[str]:
         """Get the formatted batch arguments for a preview
 
         :return: batch arguments for Qsub
-        :rtype: list[str]
         :raises ValueError: if options are supplied without values
         """
         opts = self._create_resource_list()
         for opt, value in self.batch_args.items():
             prefix = "-"
             if not value:
                 raise ValueError("PBS options without values are not allowed")
```

### Comparing `smartsim-0.6.2/smartsim/settings/settings.py` & `smartsim-0.7.0/smartsim/settings/settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 from .._core.utils.helpers import is_valid_cmd
 from ..error import SmartSimError
 from ..settings import (
     AprunSettings,
     BsubBatchSettings,
     Container,
+    DragonRunSettings,
     JsrunSettings,
     MpiexecSettings,
     MpirunSettings,
     OrterunSettings,
     PalsMpiexecSettings,
     QsubBatchSettings,
     RunSettings,
@@ -59,38 +60,34 @@
 ) -> base.BatchSettings:
     """Create a ``BatchSettings`` instance
 
     See Experiment.create_batch_settings for details
 
     :param launcher: launcher for this experiment, if set to 'auto',
                      an attempt will be made to find an available launcher on the system
-    :type launcher: str
-    :param nodes: number of nodes for batch job, defaults to 1
-    :type nodes: int, optional
-    :param time: length of batch job, defaults to ""
-    :type time: str, optional
-    :param queue: queue or partition (if slurm), defaults to ""
-    :type queue: str, optional
-    :param account: user account name for batch system, defaults to ""
-    :type account: str, optional
-    :param batch_args: additional batch arguments, defaults to None
-    :type batch_args: dict[str, str], optional
+    :param nodes: number of nodes for batch job
+    :param time: length of batch job
+    :param queue: queue or partition (if slurm)
+    :param account: user account name for batch system
+    :param batch_args: additional batch arguments
     :return: a newly created BatchSettings instance
-    :rtype: BatchSettings
     :raises SmartSimError: if batch creation fails
     """
     # all supported batch class implementations
     by_launcher: t.Dict[str, t.Callable[..., base.BatchSettings]] = {
         "pbs": QsubBatchSettings,
         "slurm": SbatchSettings,
         "lsf": BsubBatchSettings,
+        "pals": QsubBatchSettings,
     }
 
-    if launcher == "auto":
+    if launcher in ["auto", "dragon"]:
         launcher = detect_launcher()
+        if launcher == "dragon":
+            by_launcher["dragon"] = by_launcher[launcher]
 
     if launcher == "local":
         raise SmartSimError("Local launcher does not support batch workloads")
 
     # detect the batch class to use based on the launcher provided by
     # the user
     try:
@@ -123,29 +120,21 @@
 ) -> RunSettings:
     """Create a ``RunSettings`` instance.
 
     See Experiment.create_run_settings docstring for more details
 
     :param launcher: launcher to create settings for, if set to 'auto',
                      an attempt will be made to find an available launcher on the system
-    :type launcher: str
     :param run_command: command to run the executable
-    :type run_command: str
     :param exe: executable to run
-    :type exe: str
     :param exe_args: arguments to pass to the executable
-    :type exe_args: list[str], optional
     :param run_args: arguments to pass to the ``run_command``
-    :type run_args: list[str], optional
     :param env_vars: environment variables to pass to the executable
-    :type env_vars: dict[str, str], optional
-    :param container: container type for workload (e.g. "singularity"), defaults to None
-    :type container: Container, optional
+    :param container: container type for workload (e.g. "singularity")
     :return: the created ``RunSettings``
-    :rtype: RunSettings
     :raises SmartSimError: if run_command=="auto" and detection fails
     """
     # all supported RunSettings child classes
     supported: t.Dict[str, _TRunSettingsSelector] = {
         "aprun": lambda launcher: AprunSettings,
         "srun": lambda launcher: SrunSettings,
         "mpirun": lambda launcher: MpirunSettings,
@@ -155,27 +144,28 @@
         "orterun": lambda launcher: OrterunSettings,
         "jsrun": lambda launcher: JsrunSettings,
     }
 
     # run commands supported by each launcher
     # in order of suspected user preference
     by_launcher = {
+        "dragon": [""],
         "slurm": ["srun", "mpirun", "mpiexec"],
         "pbs": ["aprun", "mpirun", "mpiexec"],
         "pals": ["mpiexec"],
         "lsf": ["jsrun", "mpirun", "mpiexec"],
         "local": [""],
     }
 
     if launcher == "auto":
         launcher = detect_launcher()
 
     def _detect_command(launcher: str) -> str:
         if launcher in by_launcher:
-            if launcher == "local":
+            if launcher in ["local", "dragon"]:
                 return ""
 
             for cmd in by_launcher[launcher]:
                 if is_valid_cmd(cmd):
                     return cmd
         msg = (
             "Could not automatically detect a run command to use for launcher "
@@ -189,14 +179,19 @@
     launcher = launcher.lower()
 
     # detect run_command automatically for all but local launcher
     if run_command == "auto":
         # no auto detection for local, revert to false
         run_command = _detect_command(launcher)
 
+    if launcher == "dragon":
+        return DragonRunSettings(
+            exe=exe, exe_args=exe_args, env_vars=env_vars, container=container, **kwargs
+        )
+
     # if user specified and supported or auto detection worked
     if run_command and run_command in supported:
         return supported[run_command](launcher)(
             exe, exe_args, run_args, env_vars, container=container, **kwargs
         )
 
     # 1) user specified and not implementation in SmartSim
```

### Comparing `smartsim-0.6.2/smartsim/settings/slurmSettings.py` & `smartsim-0.7.0/smartsim/settings/slurmSettings.py`

 * *Files 17% similar despite different names*

```diff
@@ -51,23 +51,18 @@
 
         ``SrunSettings`` should only be used on Slurm based systems.
 
         If an allocation is specified, the instance receiving these run
         parameters will launch on that allocation.
 
         :param exe: executable to run
-        :type exe: str
-        :param exe_args: executable arguments, defaults to None
-        :type exe_args: list[str] | str, optional
-        :param run_args: srun arguments without dashes, defaults to None
-        :type run_args: dict[str, t.Union[int, str, float, None]], optional
-        :param env_vars: environment variables for job, defaults to None
-        :type env_vars: dict[str, str], optional
-        :param alloc: allocation ID if running on existing alloc, defaults to None
-        :type alloc: str, optional
+        :param exe_args: executable arguments
+        :param run_args: srun arguments without dashes
+        :param env_vars: environment variables for job
+        :param alloc: allocation ID if running on existing alloc
         """
         super().__init__(
             exe,
             exe_args,
             run_command="srun",
             run_args=run_args,
             env_vars=env_vars,
@@ -80,26 +75,24 @@
 
     def set_nodes(self, nodes: int) -> None:
         """Set the number of nodes
 
         Effectively this is setting: ``srun --nodes <num_nodes>``
 
         :param nodes: number of nodes to run with
-        :type nodes: int
         """
         self.run_args["nodes"] = int(nodes)
 
     def make_mpmd(self, settings: RunSettings) -> None:
         """Make a mpmd workload by combining two ``srun`` commands
 
         This connects the two settings to be executed with a single
         Model instance
 
         :param settings: SrunSettings instance
-        :type settings: SrunSettings
         """
         if self.colocated_db_settings:
             raise SSUnsupportedError(
                 "Colocated models cannot be run as a mpmd workload"
             )
         if self.container:
             raise SSUnsupportedError(
@@ -113,15 +106,14 @@
 
     def set_hostlist(self, host_list: t.Union[str, t.List[str]]) -> None:
         """Specify the hostlist for this job
 
         This sets ``--nodelist``
 
         :param host_list: hosts to launch on
-        :type host_list: str | list[str]
         :raises TypeError: if not str or list of str
         """
         if isinstance(host_list, str):
             host_list = [host_list.strip()]
         if not isinstance(host_list, list):
             raise TypeError("host_list argument must be a list of strings")
         if not all(isinstance(host, str) for host in host_list):
@@ -130,23 +122,21 @@
 
     def set_hostlist_from_file(self, file_path: str) -> None:
         """Use the contents of a file to set the node list
 
         This sets ``--nodefile``
 
         :param file_path: Path to the hostlist file
-        :type file_path: str
         """
         self.run_args["nodefile"] = file_path
 
     def set_excluded_hosts(self, host_list: t.Union[str, t.List[str]]) -> None:
         """Specify a list of hosts to exclude for launching this job
 
         :param host_list: hosts to exclude
-        :type host_list: list[str]
         :raises TypeError:
         """
         if isinstance(host_list, str):
             host_list = [host_list.strip()]
         if not isinstance(host_list, list):
             raise TypeError("host_list argument must be a list of strings")
         if not all(isinstance(host, str) for host in host_list):
@@ -155,132 +145,132 @@
 
     def set_cpus_per_task(self, cpus_per_task: int) -> None:
         """Set the number of cpus to use per task
 
         This sets ``--cpus-per-task``
 
         :param num_cpus: number of cpus to use per task
-        :type num_cpus: int
         """
         self.run_args["cpus-per-task"] = int(cpus_per_task)
 
     def set_tasks(self, tasks: int) -> None:
         """Set the number of tasks for this job
 
         This sets ``--ntasks``
 
         :param tasks: number of tasks
-        :type tasks: int
         """
         self.run_args["ntasks"] = int(tasks)
 
     def set_tasks_per_node(self, tasks_per_node: int) -> None:
         """Set the number of tasks for this job
 
         This sets ``--ntasks-per-node``
 
         :param tasks_per_node: number of tasks per node
-        :type tasks_per_node: int
         """
         self.run_args["ntasks-per-node"] = int(tasks_per_node)
 
     def set_cpu_bindings(self, bindings: t.Union[int, t.List[int]]) -> None:
         """Bind by setting CPU masks on tasks
 
         This sets ``--cpu-bind`` using the ``map_cpu:<list>`` option
 
         :param bindings: List specifing the cores to which MPI processes are bound
-        :type bindings: list[int] | int
         """
         if isinstance(bindings, int):
             bindings = [bindings]
         self.run_args["cpu_bind"] = "map_cpu:" + ",".join(
             str(int(num)) for num in bindings
         )
 
     def set_memory_per_node(self, memory_per_node: int) -> None:
         """Specify the real memory required per node
 
         This sets ``--mem`` in megabytes
 
         :param memory_per_node: Amount of memory per node in megabytes
-        :type memory_per_node: int
         """
         self.run_args["mem"] = f"{int(memory_per_node)}M"
 
     def set_verbose_launch(self, verbose: bool) -> None:
         """Set the job to run in verbose mode
 
         This sets ``--verbose``
 
         :param verbose: Whether the job should be run verbosely
-        :type verbose: bool
         """
         if verbose:
             self.run_args["verbose"] = None
         else:
             self.run_args.pop("verbose", None)
 
     def set_quiet_launch(self, quiet: bool) -> None:
         """Set the job to run in quiet mode
 
         This sets ``--quiet``
 
         :param quiet: Whether the job should be run quietly
-        :type quiet: bool
         """
         if quiet:
             self.run_args["quiet"] = None
         else:
             self.run_args.pop("quiet", None)
 
     def set_broadcast(self, dest_path: t.Optional[str] = None) -> None:
         """Copy executable file to allocated compute nodes
 
         This sets ``--bcast``
 
         :param dest_path: Path to copy an executable file
-        :type dest_path: str | None
         """
         self.run_args["bcast"] = dest_path
 
+    def set_node_feature(self, feature_list: t.Union[str, t.List[str]]) -> None:
+        """Specify the node feature for this job
+
+        This sets ``-C``
+
+        :param feature_list: node feature to launch on
+        :raises TypeError: if not str or list of str
+        """
+        if isinstance(feature_list, str):
+            feature_list = [feature_list.strip()]
+        elif not all(isinstance(feature, str) for feature in feature_list):
+            raise TypeError("node_feature argument must be string or list of strings")
+        self.run_args["C"] = ",".join(feature_list)
+
     @staticmethod
     def _fmt_walltime(hours: int, minutes: int, seconds: int) -> str:
         """Convert hours, minutes, and seconds into valid walltime format
 
         Converts time to format HH:MM:SS
 
         :param hours: number of hours to run job
-        :type hours: int
         :param minutes: number of minutes to run job
-        :type minutes: int
         :param seconds: number of seconds to run job
-        :type seconds: int
         :returns: Formatted walltime
-        :rtype: str
         """
         return fmt_walltime(hours, minutes, seconds)
 
     def set_walltime(self, walltime: str) -> None:
         """Set the walltime of the job
 
         format = "HH:MM:SS"
 
         :param walltime: wall time
-        :type walltime: str
         """
         self.run_args["time"] = str(walltime)
 
     def set_het_group(self, het_group: t.Iterable[int]) -> None:
         """Set the heterogeneous group for this job
 
         this sets `--het-group`
 
         :param het_group: list of heterogeneous groups
-        :type het_group: int or iterable of ints
         """
         het_size_env = os.getenv("SLURM_HET_SIZE")
         if het_size_env is None:
             msg = "Requested to set het group, but the allocation is not a het job"
             raise ValueError(msg)
 
         het_size = int(het_size_env)
@@ -301,15 +291,14 @@
         logger.warning(msg)
         self.run_args["het-group"] = ",".join(str(group) for group in het_group)
 
     def format_run_args(self) -> t.List[str]:
         """Return a list of slurm formatted run arguments
 
         :return: list of slurm arguments for these settings
-        :rtype: list[str]
         """
         # add additional slurm arguments based on key length
         opts = []
         for opt, value in self.run_args.items():
             short_arg = bool(len(str(opt)) == 1)
             prefix = "-" if short_arg else "--"
             if not value:
@@ -334,36 +323,34 @@
                 preexisting_var = os.environ.get(k, None)
                 if preexisting_var is not None and preexisting_var != v:
                     msg = (
                         f"Variable {k} is set to {preexisting_var} in current "
                         "environment. If the job is running in an interactive "
                         f"allocation, the value {v} will not be set. Please "
                         "consider removing the variable from the environment "
-                        "and re-run the experiment."
+                        "and re-running the experiment."
                     )
                     logger.warning(msg)
 
     def format_env_vars(self) -> t.List[str]:
         """Build bash compatible environment variable string for Slurm
 
         :returns: the formatted string of environment variables
-        :rtype: list[str]
         """
         self.check_env_vars()
         return [f"{k}={v}" for k, v in self.env_vars.items() if "," not in str(v)]
 
     def format_comma_sep_env_vars(self) -> t.Tuple[str, t.List[str]]:
         """Build environment variable string for Slurm
 
         Slurm takes exports in comma separated lists
         the list starts with all as to not disturb the rest of the environment
         for more information on this, see the slurm documentation for srun
 
         :returns: the formatted string of environment variables
-        :rtype: tuple[str, list[str]]
         """
         self.check_env_vars()
         exportable_env, compound_env, key_only = [], [], []
 
         for k, v in self.env_vars.items():
             kvp = f"{k}={v}"
 
@@ -388,21 +375,17 @@
 
 def fmt_walltime(hours: int, minutes: int, seconds: int) -> str:
     """Helper function walltime format conversion
 
     Converts time to format HH:MM:SS
 
     :param hours: number of hours to run job
-    :type hours: int
     :param minutes: number of minutes to run job
-    :type minutes: int
     :param seconds: number of seconds to run job
-    :type seconds: int
     :returns: Formatted walltime
-    :rtype: str
     """
     delta = datetime.timedelta(hours=hours, minutes=minutes, seconds=seconds)
     fmt_str = str(delta)
     if delta.seconds // 3600 < 10:
         fmt_str = "0" + fmt_str
     return fmt_str
 
@@ -423,22 +406,18 @@
 
         If the argument doesn't have a parameter, put `None`
         as the value. e.g. {'exclusive': None}
 
         Initialization values provided (nodes, time, account)
         will overwrite the same arguments in ``batch_args`` if present
 
-        :param nodes: number of nodes, defaults to None
-        :type nodes: int, optional
+        :param nodes: number of nodes
         :param time: walltime for job, e.g. "10:00:00" for 10 hours
-        :type time: str, optional
-        :param account: account for job, defaults to None
-        :type account: str, optional
-        :param batch_args: extra batch arguments, defaults to None
-        :type batch_args: dict[str, str], optional
+        :param account: account for job
+        :param batch_args: extra batch arguments
         """
         super().__init__(
             "sbatch",
             batch_args=batch_args,
             nodes=nodes,
             account=account,
             time=time,
@@ -447,87 +426,79 @@
 
     def set_walltime(self, walltime: str) -> None:
         """Set the walltime of the job
 
         format = "HH:MM:SS"
 
         :param walltime: wall time
-        :type walltime: str
         """
         # TODO check for formatting here
         if walltime:
             self.batch_args["time"] = walltime
 
     def set_nodes(self, num_nodes: int) -> None:
         """Set the number of nodes for this batch job
 
         :param num_nodes: number of nodes
-        :type num_nodes: int
         """
         if num_nodes:
             self.batch_args["nodes"] = str(int(num_nodes))
 
     def set_account(self, account: str) -> None:
         """Set the account for this batch job
 
         :param account: account id
-        :type account: str
         """
         if account:
             self.batch_args["account"] = account
 
     def set_partition(self, partition: str) -> None:
         """Set the partition for the batch job
 
         :param partition: partition name
-        :type partition: str
         """
         self.batch_args["partition"] = str(partition)
 
     def set_queue(self, queue: str) -> None:
         """alias for set_partition
 
         Sets the partition for the slurm batch job
 
         :param queue: the partition to run the batch job on
-        :type queue: str
         """
         if queue:
             self.set_partition(queue)
 
     def set_cpus_per_task(self, cpus_per_task: int) -> None:
         """Set the number of cpus to use per task
 
         This sets ``--cpus-per-task``
 
         :param num_cpus: number of cpus to use per task
-        :type num_cpus: int
         """
         self.batch_args["cpus-per-task"] = str(int(cpus_per_task))
 
     def set_hostlist(self, host_list: t.Union[str, t.List[str]]) -> None:
         """Specify the hostlist for this job
 
         :param host_list: hosts to launch on
-        :type host_list: str | list[str]
         :raises TypeError: if not str or list of str
         """
         if isinstance(host_list, str):
             host_list = [host_list.strip()]
         if not isinstance(host_list, list):
             raise TypeError("host_list argument must be a list of strings")
         if not all(isinstance(host, str) for host in host_list):
             raise TypeError("host_list argument must be list of strings")
         self.batch_args["nodelist"] = ",".join(host_list)
 
     def format_batch_args(self) -> t.List[str]:
         """Get the formatted batch arguments for a preview
 
         :return: batch arguments for Sbatch
-        :rtype: list[str]
         """
         opts = []
         # TODO add restricted here
         for opt, value in self.batch_args.items():
             # attach "-" prefix if argument is 1 character otherwise "--"
             short_arg = bool(len(str(opt)) == 1)
             prefix = "-" if short_arg else "--"
```

### Comparing `smartsim-0.6.2/smartsim/slurm.py` & `smartsim-0.7.0/smartsim/_core/utils/telemetry/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,27 +19,7 @@
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
-
-from warnings import simplefilter, warn
-
-# pylint: disable-next=unused-import
-from .wlm.slurm import (
-    _get_alloc_cmd,
-    _get_system_partition_info,
-    get_allocation,
-    get_default_partition,
-    release_allocation,
-    validate,
-)
-
-simplefilter("once", category=DeprecationWarning)
-DEPRECATION_MSG = (
-    "`smartsim.slurm` has been deprecated and will be removed in a future release.\n"
-    "Please update your code to use `smartsim.wlm.slurm`"
-)
-warn(DEPRECATION_MSG, category=DeprecationWarning, stacklevel=2)
```

### Comparing `smartsim-0.6.2/smartsim/status.py` & `smartsim-0.7.0/smartsim/status.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,31 +20,25 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+from enum import Enum
 
-# Statuses that are applied to jobs
-STATUS_RUNNING = "Running"
-STATUS_COMPLETED = "Completed"
-STATUS_CANCELLED = "Cancelled"
-STATUS_FAILED = "Failed"
-STATUS_NEW = "New"
-STATUS_PAUSED = "Paused"
-STATUS_NEVER_STARTED = "NeverStarted"
 
-# SmartSim status mapping
-SMARTSIM_STATUS = {
-    "Running": STATUS_RUNNING,
-    "Paused": STATUS_PAUSED,
-    "Completed": STATUS_COMPLETED,
-    "Cancelled": STATUS_CANCELLED,
-    "Failed": STATUS_FAILED,
-    "New": STATUS_NEW,
-    "NeverStarted": STATUS_NEVER_STARTED,
-}
+class SmartSimStatus(Enum):
+    STATUS_RUNNING = "Running"
+    STATUS_COMPLETED = "Completed"
+    STATUS_CANCELLED = "Cancelled"
+    STATUS_FAILED = "Failed"
+    STATUS_NEW = "New"
+    STATUS_PAUSED = "Paused"
+    STATUS_NEVER_STARTED = "NeverStarted"
+
 
-# Status groupings
-TERMINAL_STATUSES = {STATUS_CANCELLED, STATUS_COMPLETED, STATUS_FAILED}
-LIVE_STATUSES = {STATUS_RUNNING, STATUS_PAUSED, STATUS_NEW}
+TERMINAL_STATUSES = {
+    SmartSimStatus.STATUS_CANCELLED,
+    SmartSimStatus.STATUS_COMPLETED,
+    SmartSimStatus.STATUS_FAILED,
+}
```

### Comparing `smartsim-0.6.2/smartsim/wlm/__init__.py` & `smartsim-0.7.0/smartsim/wlm/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,17 +71,15 @@
 
 
 def get_hosts(launcher: t.Optional[str] = None) -> t.List[str]:
     """Get the name of the hosts used in an allocation.
 
     :param launcher: Name of the WLM to use to collect allocation info. If no launcher
                      is provided ``detect_launcher`` is used to select a launcher.
-    :type launcher: str | None
     :returns: Names of the hosts
-    :rtype: list[str]
     :raises SSUnsupportedError: User attempted to use an unsupported WLM
     """
     if launcher is None:
         launcher = detect_launcher()
     if launcher == "pbs":
         return _pbs.get_hosts()
     if launcher == "slurm":
@@ -90,17 +88,15 @@
 
 
 def get_queue(launcher: t.Optional[str] = None) -> str:
     """Get the name of the queue used in an allocation.
 
     :param launcher: Name of the WLM to use to collect allocation info. If no launcher
                      is provided ``detect_launcher`` is used to select a launcher.
-    :type launcher: str | None
     :returns: Name of the queue
-    :rtype: str
     :raises SSUnsupportedError: User attempted to use an unsupported WLM
     """
     if launcher is None:
         launcher = detect_launcher()
     if launcher == "pbs":
         return _pbs.get_queue()
     if launcher == "slurm":
@@ -109,17 +105,15 @@
 
 
 def get_tasks(launcher: t.Optional[str] = None) -> int:
     """Get the number of tasks in an allocation.
 
     :param launcher: Name of the WLM to use to collect allocation info. If no launcher
                      is provided ``detect_launcher`` is used to select a launcher.
-    :type launcher: str | None
     :returns: Number of tasks
-    :rtype: int
     :raises SSUnsupportedError: User attempted to use an unsupported WLM
     """
     if launcher is None:
         launcher = detect_launcher()
     if launcher == "pbs":
         return _pbs.get_tasks()
     if launcher == "slurm":
@@ -128,17 +122,15 @@
 
 
 def get_tasks_per_node(launcher: t.Optional[str] = None) -> t.Dict[str, int]:
     """Get a map of nodes in an allocation to the number of tasks on each node.
 
     :param launcher: Name of the WLM to use to collect allocation info. If no launcher
                      is provided ``detect_launcher`` is used to select a launcher.
-    :type launcher: str | None
     :returns: Map of nodes to number of processes on that node
-    :rtype: dict[str, int]
     :raises SSUnsupportedError: User attempted to use an unsupported WLM
     """
     if launcher is None:
         launcher = detect_launcher()
     if launcher == "pbs":
         return _pbs.get_tasks_per_node()
     if launcher == "slurm":
```

### Comparing `smartsim-0.6.2/smartsim/wlm/pbs.py` & `smartsim-0.7.0/smartsim/wlm/pbs.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 from .._core.launcher.pbs.pbsCommands import qstat
 
 
 def get_hosts() -> t.List[str]:
     """Get the name of the hosts used in a PBS allocation.
 
     :returns: Names of the host nodes
-    :rtype: list[str]
     :raises SmartSimError: ``PBS_NODEFILE`` is not set
     """
     hosts = []
     if "PBS_NODEFILE" in os.environ:
         node_file_path = os.environ["PBS_NODEFILE"]
         with open(node_file_path, "r", encoding="utf-8") as node_file:
             for line in node_file.readlines():
@@ -55,15 +54,14 @@
     )
 
 
 def get_queue() -> str:
     """Get the name of queue in a PBS allocation.
 
     :returns: The name of the queue
-    :rtype: str
     :raises SmartSimError: ``PBS_QUEUE`` is not set
     """
     if "PBS_QUEUE" in os.environ:
         return os.environ["PBS_QUEUE"]
     raise SmartSimError("Could not parse queue from PBS_QUEUE")
 
 
@@ -72,15 +70,14 @@
 
     .. note::
 
         This method requires ``qstat`` be installed on the
         node from which it is run.
 
     :returns: Then number of tasks in the allocation
-    :rtype: int
     :raises LauncherError: Could not access ``qstat``
     :raises SmartSimError: ``PBS_JOBID`` is not set
     """
     if "PBS_JOBID" in os.environ:
         if not which("qstat"):
             raise LauncherError(
                 "Attempted PBS function without access to PBS(qstat) at the call site"
@@ -99,16 +96,15 @@
     """Get the number of processes on each chunk in a PBS allocation.
 
     .. note::
 
         This method requires ``qstat`` be installed on the
         node from which it is run.
 
-    :returns: Map of chunks to number of processes on that chunck
-    :rtype: dict[str, int]
+    :returns: Map of chunks to number of processes on that chunk
     :raises LauncherError: Could not access ``qstat``
     :raises SmartSimError: ``PBS_JOBID`` is not set
     """
     if "PBS_JOBID" in os.environ:
         if not which("qstat"):
             raise LauncherError(
                 (
```

### Comparing `smartsim-0.6.2/smartsim/wlm/slurm.py` & `smartsim-0.7.0/smartsim/wlm/slurm.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 import os
 import typing as t
 from shutil import which
 
 from .._core.launcher.slurm.slurmCommands import salloc, scancel, scontrol, sinfo
 from .._core.launcher.slurm.slurmParser import parse_salloc, parse_salloc_error
 from .._core.launcher.util.launcherUtil import ComputeNode, Partition
-from .._core.utils.helpers import init_default
 from ..error import (
     AllocationError,
     LauncherError,
     SmartSimError,
     SSReservedKeywordError,
 )
 from ..log import get_logger
@@ -56,39 +55,34 @@
     Anything passed to the options will be processed as a Slurm
     argument and appended to the salloc command with the appropriate
     prefix (e.g. "-" or "--").
 
     The options can be used to pass extra settings to the
     workload manager such as the following for Slurm:
 
-        - nodelist="nid00004"
+    - nodelist="nid00004"
 
     For arguments without a value, pass None or and empty
     string as the value. For Slurm:
 
-        - exclusive=None
+    - exclusive=None
 
-    :param nodes: number of nodes for the allocation, defaults to 1
-    :type nodes: int, optional
-    :param time: wall time of the allocation, HH:MM:SS format, defaults to None
-    :type time: str, optional
-    :param account: account id for allocation, defaults to None
-    :type account: str, optional
-    :param options: additional options for the slurm wlm, defaults to None
-    :type options: dict[str, str], optional
+    :param nodes: number of nodes for the allocation
+    :param time: wall time of the allocation, HH:MM:SS format
+    :param account: account id for allocation
+    :param options: additional options for the slurm wlm
     :raises LauncherError: if the allocation is not successful
     :return: the id of the allocation
-    :rtype: str
     """
     if not which("salloc"):
         raise LauncherError(
             "Attempted slurm function without access to slurm(salloc) at the call site"
         )
 
-    options = init_default({}, options, dict)
+    options = options or {}
 
     salloc_args = _get_alloc_cmd(nodes, time, account, options=options)
     debug_msg = " ".join(salloc_args[1:])
     logger.debug(f"Allocation settings: {debug_msg}")
 
     _, err = salloc(salloc_args)
     alloc_id = parse_salloc(err)
@@ -104,15 +98,14 @@
     return str(alloc_id)
 
 
 def release_allocation(alloc_id: str) -> None:
     """Free an allocation's resources
 
     :param alloc_id: allocation id
-    :type alloc_id: str
     :raises LauncherError: if allocation could not be freed
     """
     if not which("scancel"):
         raise LauncherError(
             "Attempted slurm function without access to slurm(salloc) at the call site"
         )
 
@@ -133,23 +126,19 @@
 
 
 def validate(nodes: int = 1, ppn: int = 1, partition: t.Optional[str] = None) -> bool:
     """Check that there are sufficient resources in the provided Slurm partitions.
 
     if no partition is provided, the default partition is found and used.
 
-    :param nodes: Override the default node count to validate, defaults to 1
-    :type nodes: int, optional
-    :param ppn: Override the default processes per node to validate, defaults to 1
-    :type ppn: int, optional
-    :param partition: partition to validate, defaults to None
-    :type partition: str, optional
+    :param nodes: Override the default node count to validate
+    :param ppn: Override the default processes per node to validate
+    :param partition: partition to validate
     :raises: LauncherError
     :returns: True if resources are available, False otherwise
-    :rtype: bool
     """
     sys_partitions = _get_system_partition_info()
 
     n_avail_nodes = 0
     avail_nodes = set()
 
     p_name = partition
@@ -185,15 +174,14 @@
 def get_default_partition() -> str:
     """Returns the default partition from Slurm
 
     This default partition is assumed to be the partition with
     a star following its partition name in sinfo output
 
     :returns: the name of the default partition
-    :rtype: str
     """
     sinfo_output, _ = sinfo(["--noheader", "--format", "%P"])
 
     default = None
     for line in sinfo_output.split("\n"):
         if line.endswith("*"):
             default = line.strip("*")
@@ -202,15 +190,14 @@
         raise LauncherError("Could not find default partition!")
     return default
 
 
 def _get_system_partition_info() -> t.Dict[str, Partition]:
     """Build a dictionary of slurm partitions
     :returns: dict of Partition objects
-    :rtype: dict
     """
 
     sinfo_output, _ = sinfo(["--noheader", "--format", "%R %n %c"])
 
     partitions: t.Dict[str, Partition] = {}
     for line in sinfo_output.split("\n"):
         line = line.strip()
@@ -276,17 +263,15 @@
 
 def _validate_time_format(time: str) -> str:
     """Convert time into valid walltime format
 
     By defualt the formatted wall time is the total number of seconds.
 
     :param time: number of hours to run job
-    :type time: str
     :returns: Formatted walltime
-    :rtype: str
     """
     try:
         hours, minutes, seconds = map(int, time.split(":"))
     except ValueError as e:
         raise ValueError(
             "Input time must be formatted as `HH:MM:SS` with valid Integers."
         ) from e
@@ -298,15 +283,14 @@
 
     .. note::
 
         This method requires access to ``scontrol`` from the node
         on which it is run
 
     :returns: Names of the host nodes
-    :rtype: list[str]
     :raises LauncherError: Could not access ``scontrol``
     :raises SmartSimError: ``SLURM_JOB_NODELIST`` is not set
     """
     if "SLURM_JOB_NODELIST" in os.environ:
         if not which("scontrol"):
             raise LauncherError(
                 (
@@ -321,27 +305,25 @@
     raise SmartSimError("Could not parse allocation nodes from SLURM_JOB_NODELIST")
 
 
 def get_queue() -> str:
     """Get the name of queue in a slurm allocation.
 
     :returns: The name of the queue
-    :rtype: str
     :raises SmartSimError: ``SLURM_JOB_PARTITION`` is not set
     """
     if job_partition := os.environ.get("SLURM_JOB_PARTITION", None):
         return job_partition
     raise SmartSimError("Could not parse queue from SLURM_JOB_PARTITION")
 
 
 def get_tasks() -> int:
     """Get the number of tasks in a slurm allocation.
 
     :returns: Then number of tasks in the allocation
-    :rtype: int
     :raises SmartSimError: ``SLURM_NTASKS`` is not set
     """
     if ntasks_str := os.environ.get("SLURM_NTASKS", 0):
         return int(ntasks_str)
     raise SmartSimError("Could not parse number of requested tasks from SLURM_NTASKS")
 
 
@@ -350,15 +332,14 @@
 
     .. note::
 
         This method requires access to ``scontrol`` from the node
         on which it is run
 
     :returns: Map of nodes to number of tasks on that node
-    :rtype: dict[str, int]
     :raises SmartSimError: ``SLURM_TASKS_PER_NODE`` is not set
     """
     if "SLURM_TASKS_PER_NODE" in os.environ:
         tasks_per_node_strs = os.environ.get("SLURM_TASKS_PER_NODE", "").split(",")
         tasks_per_node_list = []
         for tasks_per_node_str in tasks_per_node_strs:
             if "(" in tasks_per_node_str:
```

### Comparing `smartsim-0.6.2/smartsim.egg-info/PKG-INFO` & `smartsim-0.7.0/smartsim.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,780 +1,786 @@
 Metadata-Version: 2.1
 Name: smartsim
-Version: 0.6.2
+Version: 0.7.0
 Summary: AI Workflows for Science
 Home-page: https://github.com/CrayLabs/SmartSim
 Author: CrayLabs, a Hewlett Packard Enterprise OSS Organization
 Author-email: craylabs@hpe.com
 License: BSD 2-Clause License
 Project-URL: Source, https://github.com/CrayLabs/SmartSim
 Project-URL: Documentation, https://www.craylabs.org
-Description: 
-        
-        <div align="center">
-            <a href="https://github.com/CrayLabs/SmartSim"><img src="https://raw.githubusercontent.com/CrayLabs/SmartSim/master/doc/images/SmartSim_Large.png" width="90%"><img></a>
-            <br />
-            <br />
-        <div display="inline-block">
-            <a href="https://github.com/CrayLabs/SmartSim"><b>Home</b></a>&nbsp;&nbsp;&nbsp;
-            <a href="https://www.craylabs.org/docs/installation_instructions/basic.html"><b>Install</b></a>&nbsp;&nbsp;&nbsp;
-            <a href="https://www.craylabs.org/docs/overview.html"><b>Documentation</b></a>&nbsp;&nbsp;&nbsp;
-            <a href="https://github.com/CrayLabs"><b>Cray Labs</b></a>&nbsp;&nbsp;&nbsp;
-            <a href="mailto:craylabs@hpe.com"><b>Contact</b></a>&nbsp;&nbsp;&nbsp;
-            <a href="https://join.slack.com/t/craylabs/shared_invite/zt-nw3ag5z5-5PS4tIXBfufu1bIvvr71UA"><b>Join us on Slack!</b></a>&nbsp;&nbsp;&nbsp;
-          </div>
-            <br />
-            <br />
-        </div>
-        
-        
-        <div align="center">
-        
-        [![License](https://img.shields.io/github/license/CrayLabs/SmartSim)](https://github.com/CrayLabs/SmartSim/blob/master/LICENSE.md)
-        ![GitHub last commit](https://img.shields.io/github/last-commit/CrayLabs/SmartSim)
-        ![GitHub deployments](https://img.shields.io/github/deployments/CrayLabs/SmartSim/github-pages?label=doc%20build)
-        ![PyPI - Wheel](https://img.shields.io/pypi/wheel/smartsim)
-        ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/smartsim)
-        ![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/CrayLabs/SmartSim)
-        ![Language](https://img.shields.io/github/languages/top/CrayLabs/SmartSim)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        [![codecov](https://codecov.io/gh/CrayLabs/SmartSim/branch/develop/graph/badge.svg?token=96HFI2F45E)](https://codecov.io/gh/CrayLabs/SmartSim)
-        [![Downloads](https://static.pepy.tech/personalized-badge/smartsim?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/smartsim)
-        
-        </div>
-        
-        ------------
-        
-        # SmartSim
-        
-        SmartSim is made up of two parts
-          1. SmartSim Infrastructure Library (This repository)
-          2. [SmartRedis](https://github.com/CrayLabs/SmartRedis)
-        
-        The two library components are designed to work together, but can also be used
-        independently.
-        
-        *SmartSim* is a workflow library that makes it easier to use common Machine Learning (ML)
-        libraries, like PyTorch and TensorFlow, in High Performance Computing (HPC) simulations
-        and applications. SmartSim launches ML infrastructure on HPC systems alongside user
-        workloads.
-        
-        *SmartRedis* provides an API to connect HPC workloads, particularly (MPI + X) simulations,
-        to the ML infrastructure, namely the The [Orchestrator database](https://www.craylabs.org/docs/orchestrator.html),
-        launched by SmartSim.
-        
-        Applications integrated with the SmartRedis clients, written in Fortran, C, C++ and Python,
-        can send data to and remotely request SmartSim infrastructure to execute ML models and scripts
-        on GPU or CPU. The distributed Client-Server paradigm allows for data to be seamlessly
-        exchanged between applications at runtime without the utilization of MPI.
-        
-        ----------
-        
-        **Table of Contents**
-        - [SmartSim](#smartsim)
-        - [Quick Start](#quick-start)
-        - [SmartSim Infrastructure Library](#smartsim-infrastructure-library)
-          - [Experiments](#experiments)
-            - [Hello World](#hello-world)
-            - [Hello World MPI](#hello-world-mpi)
-          - [Experiments on HPC Systems](#experiments-on-hpc-systems)
-            - [Interactive Launch Example](#interactive-launch-example)
-            - [Batch Launch Examples](#batch-launch-examples)
-        - [Infrastructure Library Applications](#infrastructure-library-applications)
-          - [Redis + RedisAI](#redis--redisai)
-            - [Local Launch](#local-launch)
-            - [Interactive Launch](#interactive-launch)
-            - [Batch Launch](#batch-launch)
-        - [SmartRedis](#smartredis)
-          - [Tensors](#tensors)
-          - [Datasets](#datasets)
-        - [SmartSim + SmartRedis Tutorials](#smartsim--smartredis-tutorials)
-          - [Run the Tutorials](#run-the-tutorials)
-          - [Online Analysis](#online-analysis)
-              - [Lattice Boltzmann Simulation](#lattice-boltzmann-simulation)
-          - [Online Processing](#online-processing)
-            - [Singular Value Decomposition](#singular-value-decomposition)
-          - [Online Inference](#online-inference)
-            - [PyTorch CNN Example](#pytorch-cnn-example)
-        - [Publications](#publications)
-        - [Cite](#cite)
-          - [bibtex](#bibtex)
-        
-        ----
-        
-        # Quick Start
-        
-        
-        The documentation has a number of tutorials that make it easy to get used to SmartSim locally
-        before using it on your system. Each tutorial is a Jupyter notebook that can be run through the
-        [SmartSim Tutorials docker image](https://github.com/orgs/CrayLabs/packages?repo_name=SmartSim)
-        which will run a jupyter lab with the tutorials, SmartSim, and SmartRedis installed.
-        
-        ```bash
-        docker pull ghcr.io/craylabs/smartsim-tutorials:latest
-        docker run -p 8888:8888 ghcr.io/craylabs/smartsim-tutorials:latest
-        # click on link to open jupyter lab
-        ```
-        
-        # SmartSim Infrastructure Library
-        
-        The Infrastructure Library (IL), the ``smartsim`` python package,
-        facilitates the launch of Machine Learning and simulation
-        workflows. The Python interface of the IL creates, configures, launches and monitors
-        applications.
-        
-        ## Experiments
-        
-        The [Experiment](https://www.craylabs.org/docs/api/smartsim_api.html#experiment) object
-        is the main interface of SmartSim. Through the [Experiment](https://www.craylabs.org/docs/api/smartsim_api.html#experiment)
-        users can create references to user applications called ``Models``.
-        ### Hello World
-        
-        Below is a simple example of a workflow that uses the IL to launch hello world
-        program using the local launcher which is designed for laptops and single nodes.
-        
-        ```python
-        from smartsim import Experiment
-        
-        exp = Experiment("simple", launcher="local")
-        
-        settings = exp.create_run_settings("echo", exe_args="Hello World")
-        model = exp.create_model("hello_world", settings)
-        
-        exp.start(model, block=True)
-        print(exp.get_status(model))
-        ```
-        
-        ### Hello World MPI
-        
-        The [Experiment.create_run_settings](https://www.craylabs.org/docs/api/smartsim_api.html#smartsim.experiment.Experiment.create_run_settings) method returns a ``RunSettings`` object which
-        defines how a model is launched. There are many types of ``RunSettings`` [supported by
-        SmartSim](https://www.craylabs.org/docs/api/smartsim_api.html#settings).
-        
-         - ``RunSettings``
-         - ``MpirunSettings``
-         - ``SrunSettings``
-         - ``AprunSettings``
-         - ``JsrunSettings``
-        
-        The following example launches a hello world MPI program using the local launcher
-        for single compute node, workstations and laptops.
-        
-        ```Python
-        from smartsim import Experiment
-        
-        exp = Experiment("hello_world", launcher="local")
-        mpi_settings = exp.create_run_settings(exe="echo",
-                                               exe_args="Hello World!",
-                                               run_command="mpirun")
-        mpi_settings.set_tasks(4)
-        
-        mpi_model = exp.create_model("hello_world", mpi_settings)
-        
-        exp.start(mpi_model, block=True)
-        print(exp.get_status(model))
-        ```
-        
-        If an argument of `run_command="auto"` (the default) is passed to
-        `Experiment.create_run_settings`, SmartSim will attempt to find a run command on the
-        system with which it has a corresponding `RunSettings` class. If one can be found,
-        `Experiment.create_run_settings` will instance and return an object of that type.
-        
-        
-        -----------
-        ## Experiments on HPC Systems
-        
-        SmartSim integrates with common HPC schedulers providing batch and interactive
-        launch capabilities for all applications.
-        
-         - Slurm
-         - LSF
-         - PBSPro
-         - Local (for laptops/single node, no batch)
-        
-        
-        ### Interactive Launch Example
-        
-        The following launches the same ``hello_world`` model in an interactive allocation.
-        
-        ```bash
-        # get interactive allocation (Slurm)
-        salloc -N 3 --ntasks-per-node=20 --ntasks 60 --exclusive -t 00:10:00
-        
-        # get interactive allocation (PBS)
-        qsub -l select=3:ncpus=20 -l walltime=00:10:00 -l place=scatter -I -q <queue>
-        
-        # get interactive allocation (LSF)
-        bsub -Is -W 00:10 -nnodes 3 -P <project> $SHELL
-        ```
-        
-        This same script will run on a SLURM, PBS, or LSF system as the ``launcher``
-        is set to `auto` in the [Experiment](https://www.craylabs.org/docs/api/smartsim_api.html#experiment)
-        initialization. The run command like ``mpirun``,
-        ``aprun`` or ``srun`` will be automatically detected from what is available on the
-        system.
-        
-        ```python
-        # hello_world.py
-        from smartsim import Experiment
-        
-        exp = Experiment("hello_world_exp", launcher="auto")
-        run = exp.create_run_settings(exe="echo", exe_args="Hello World!")
-        run.set_tasks(60)
-        run.set_tasks_per_node(20)
-        
-        model = exp.create_model("hello_world", run)
-        exp.start(model, block=True, summary=True)
-        
-        print(exp.get_status(model))
-        ```
-        ```bash
-        # in interactive terminal
-        python hello_world.py
-        ```
-        
-        
-        This script could also be launched in a batch file instead of an
-        interactive terminal. For example, for Slurm:
-        
-        ```bash
-        #!/bin/bash
-        #SBATCH --exclusive
-        #SBATCH --nodes=3
-        #SBATCH --ntasks-per-node=20
-        #SBATCH --time=00:10:00
-        
-        python /path/to/hello_world.py
-        ```
-        ```bash
-        # on Slurm system
-        sbatch run_hello_world.sh
-        ```
-        
-        
-        ### Batch Launch Examples
-        
-        SmartSim can also launch workloads in a batch directly from Python, without the need
-        for a batch script. Users can launch groups of ``Model`` instances in a ``Ensemble``.
-        
-        The following launches 4 replicas of the the same ``hello_world`` model.
-        
-        ```python
-        # hello_ensemble.py
-        from smartsim import Experiment
-        
-        exp = Experiment("hello_world_batch", launcher="auto")
-        
-        # define resources for all ensemble members
-        batch = exp.create_batch_settings(nodes=4, time="00:10:00", account="12345-Cray")
-        batch.set_queue("premium")
-        
-        # define how each member should run
-        run = exp.create_run_settings(exe="echo", exe_args="Hello World!")
-        run.set_tasks(60)
-        run.set_tasks_per_node(20)
-        
-        ensemble = exp.create_ensemble("hello_world",
-                                       batch_settings=batch,
-                                       run_settings=run,
-                                       replicas=4)
-        exp.start(ensemble, block=True, summary=True)
-        
-        print(exp.get_status(ensemble))
-        ```
-        
-        ```bash
-        python hello_ensemble.py
-        ```
-        
-        Similar to the interactive example, this same script will run on a SLURM, PBS,
-        or LSF system as the ``launcher`` is set to `auto` in the
-        [Experiment](https://www.craylabs.org/docs/api/smartsim_api.html#experiment)
-        initialization. Local launching does not support batch workloads.
-        
-        
-        --------
-        
-        # Infrastructure Library Applications
-         - Orchestrator - In-memory data store and Machine Learning Inference (Redis + RedisAI)
-        
-        ## Redis + RedisAI
-        
-        The ``Orchestrator`` is an in-memory database that utilizes Redis and RedisAI to provide
-        a distributed database and access to ML runtimes from Fortran, C, C++ and Python.
-        
-        SmartSim provides classes that make it simple to launch the database in many
-        configurations and optionally form a distributed database cluster. The examples
-        below will show how to launch the database. Later in this document we will show
-        how to use the database to perform ML inference and processing.
-        
-        
-        ### Local Launch
-        
-        The following script launches a single database using the local launcher.
-        
-        [Experiment.create_database](https://www.craylabs.org/docs/api/smartsim_api.html#smartsim.experiment.Experiment.create_database)
-        will initialize an ``Orchestrator`` instance corresponding to the specified launcher.
-        
-        ```python
-        # run_db_local.py
-        from smartsim import Experiment
-        
-        exp = Experiment("local-db", launcher="local")
-        db = exp.create_database(port=6780,       # database port
-                                 interface="lo")  # network interface to use
-        
-        # by default, SmartSim never blocks execution after the database is launched.
-        exp.start(db)
-        
-        # launch models, analysis, training, inference sessions, etc
-        # that communicate with the database using the SmartRedis clients
-        
-        # stop the database
-        exp.stop(db)
-        ```
-        
-        ### Interactive Launch
-        
-        The ``Orchestrator``, like ``Ensemble`` instances, can be launched locally, in interactive
-        allocations, or in a batch.
-        
-        The following example launches a distributed (3 node) database cluster
-        in an interactive allocation.
-        
-        
-        ```bash
-        # get interactive allocation (Slurm)
-        salloc -N 3 --ntasks-per-node=1 --exclusive -t 00:10:00
-        
-        # get interactive allocation (PBS)
-        qsub -l select=3:ncpus=1 -l walltime=00:10:00 -l place=scatter -I -q queue
-        
-        # get interactive allocation (LSF)
-        bsub -Is -W 00:10 -nnodes 3 -P project $SHELL
-        
-        ```
-        
-        ```python
-        # run_db.py
-        from smartsim import Experiment
-        
-        # auto specified to work across launcher types
-        exp = Experiment("db-on-slurm", launcher="auto")
-        db_cluster = exp.create_database(db_nodes=3,
-                                         db_port=6780,
-                                         batch=False,
-                                         interface="ipogif0")
-        exp.start(db_cluster)
-        
-        print(f"Orchestrator launched on nodes: {db_cluster.hosts}")
-        # launch models, analysis, training, inference sessions, etc
-        # that communicate with the database using the SmartRedis clients
-        
-        exp.stop(db_cluster)
-        ```
-        ```bash
-        # in interactive terminal
-        python run_db.py
-        ```
-        
-        ### Batch Launch
-        
-        The ``Orchestrator`` can also be launched in a batch without the need for an interactive allocation.
-        SmartSim will create the batch file, submit it to the batch system, and then wait for the database
-        to be launched. Users can hit CTRL-C to cancel the launch if needed.
-        
-        ```Python
-        # run_db_batch.py
-        from smartsim import Experiment
-        
-        exp = Experiment("batch-db-on-pbs", launcher="auto")
-        db_cluster = exp.create_database(db_nodes=3,
-                                         db_port=6780,
-                                         batch=True,
-                                         time="00:10:00",
-                                         interface="ib0",
-                                         account="12345-Cray",
-                                         queue="cl40")
-        
-        exp.start(db_cluster)
-        
-        print(f"Orchestrator launched on nodes: {db_cluster.hosts}")
-        # launch models, analysis, training, inference sessions, etc
-        # that communicate with the database using the SmartRedis clients
-        
-        exp.stop(db_cluster)
-        ```
-        
-        ```bash
-        python run_db_batch.py
-        ```
-        
-        ------
-        # SmartRedis
-        
-        The SmartSim IL Clients ([SmartRedis](https://github.com/CrayLabs/SmartRedis))
-        are implementations of Redis clients that implement the RedisAI
-        API with additions specific to scientific workflows.
-        
-        SmartRedis clients are available in Fortran, C, C++, and Python.
-        Users can seamlessly pull and push data from the Orchestrator from different languages.
-        
-        ## Tensors
-        
-        Tensors are the fundamental data structure for the SmartRedis clients. The Clients
-        use the native array format of the language. For example, in Python, a tensor is
-        a NumPy array while the C/C++ clients accept nested and contiguous arrays.
-        
-        When stored in the database, all tensors are stored in the same format. Hence,
-        any language can receive a tensor from the database no matter what supported language
-        the array was sent from. This enables applications in different languages to communicate
-        numerical data with each other at runtime.
-        
-        For more information on the tensor data structure, see
-        [the documentation](https://www.craylabs.org/docs/sr_data_structures.html#tensor)
-        
-        ## Datasets
-        
-        Datasets are collections of Tensors and associated metadata. The ``Dataset`` class
-        is a user space object that can be created, added to, sent to, and retrieved from
-        the Orchestrator.
-        
-        For an example of how to use the ``Dataset`` class, see the [Online Analysis example](#online-analysis)
-        
-        For more information on the API, see the
-        [API documentation](https://www.craylabs.org/docs/sr_data_structures.html#dataset)
-        
-        # SmartSim + SmartRedis Tutorials
-        
-        SmartSim and SmartRedis were designed to work together. When launched through
-        SmartSim, applications using the SmartRedis clients are directly connected to
-        any Orchestrator launched in the same [Experiment](https://www.craylabs.org/docs/api/smartsim_api.html#experiment).
-        
-        In this way, a SmartSim [Experiment](https://www.craylabs.org/docs/api/smartsim_api.html#experiment) becomes a driver for coupled ML and Simulation
-        workflows. The following are simple examples of how to use SmartSim and SmartRedis
-        together.
-        
-        ## Run the Tutorials
-        
-        Each tutorial is a Jupyter notebook that can be run through the
-        [SmartSim Tutorials docker image](https://github.com/orgs/CrayLabs/packages?repo_name=SmartSim)
-        which will run a jupyter lab with the tutorials, SmartSim, and SmartRedis installed.
-        
-        ```bash
-        docker pull ghcr.io/craylabs/smartsim-tutorials:latest
-        docker run -p 8888:8888 ghcr.io/craylabs/smartsim-tutorials:latest
-        ```
-        Each of the following examples can be found in the
-        [SmartSim documentation](https://www.craylabs.org/docs/tutorials/getting_started/getting_started.html).
-        
-        ## Online Analysis
-        
-        Using SmartSim, HPC applications can be monitored in real time by streaming data
-        from the application to the database. SmartRedis clients can retrieve the
-        data, process, analyze it, and finally store any updated data back to the database for
-        use by other clients.
-        
-        The following is an example of how a user could monitor and analyze a simulation.
-        The example here uses the Python client; however, SmartRedis clients are also available
-        for C, C++, and Fortran. All SmartRedis clients implement the same API.
-        
-        The example will produce [this visualization](https://user-images.githubusercontent.com/13009163/127622717-2c9e4cfd-50f4-4d94-88c4-8c05fa2fa616.mp4) while the simulation is running.
-        
-        #### Lattice Boltzmann Simulation
-        
-        Using a [Lattice Boltzmann Simulation](https://en.wikipedia.org/wiki/Lattice_Boltzmann_methods),
-        this example demonstrates how to use the SmartRedis ``Dataset`` API to stream
-        data over the Orchestrator deployed by SmartSim.
-        
-        The simulation will be composed of two parts: `fv_sim.py` which will generate data from
-        the Simulation and store it in the Orchestrator, and `driver.py`
-        which will launch the Orchestrator, start `fv_sim.py` and check for data posted to the
-        Orchestrator to plot updates in real-time.
-        
-        The following code highlights the sections of `fv_sim.py` that are responsible for
-        transmitting the data needed to plot timesteps of the simulation to the Orchestrator.
-        
-        ```Python
-        # fv_sim.py
-        from smartredis import Client
-        import numpy as np
-        
-        # initialization code omitted
-        
-        # save cylinder location to database
-        cylinder = (X - x_res/4)**2 + (Y - y_res/2)**2 < (y_res/4)**2 # bool array
-        client.put_tensor("cylinder", cylinder.astype(np.int8))
-        
-        for time_step in range(steps): # simulation loop
-            for i, cx, cy in zip(idxs, cxs, cys):
-                F[:,:,i] = np.roll(F[:,:,i], cx, axis=1)
-                F[:,:,i] = np.roll(F[:,:,i], cy, axis=0)
-        
-            bndryF = F[cylinder,:]
-            bndryF = bndryF[:,[0,5,6,7,8,1,2,3,4]]
-        
-            rho = np.sum(F, 2)
-            ux  = np.sum(F * cxs, 2) / rho
-            uy  = np.sum(F * cys, 2) / rho
-        
-            Feq = np.zeros(F.shape)
-            for i, cx, cy, w in zip(idxs, cxs, cys, weights):
-                Feq[:,:,i] = rho * w * ( 1 + 3*(cx*ux+cy*uy)  + 9*(cx*ux+cy*uy)**2/2 - 3*(ux**2+uy**2)/2 )
-            F += -(1.0/tau) * (F - Feq)
-            F[cylinder,:] = bndryF
-        
-            # Create a SmartRedis dataset with vorticity data
-            dataset = Dataset(f"data_{str(time_step)}")
-            dataset.add_tensor("ux", ux)
-            dataset.add_tensor("uy", uy)
-        
-            # Put Dataset in db at key "data_{time_step}"
-            client.put_dataset(dataset)
-        ```
-        
-        The driver script, `driver.py`, launches the Orchestrator database and runs
-        the simulation in a non-blocking fashion. The driver script then uses the SmartRedis
-        client to pull the DataSet and plot the vorticity while the simulation is running.
-        
-        ```Python
-        # driver.py
-        time_steps, seed = 3000, 42
-        
-        exp = Experiment("finite_volume_simulation", launcher="local")
-        
-        db = exp.create_database(port=6780,        # database port
-                                 interface="lo")   # network interface db should listen on
-        
-        # create the lb simulation Model reference
-        settings = exp.create_run_settings("python",
-                                           exe_args=["fv_sim.py",
-                                                     f"--seed={seed}",
-                                                     f"--steps={time_steps}"])
-        model = exp.create_model("fv_simulation", settings)
-        model.attach_generator_files(to_copy="fv_sim.py")
-        exp.generate(db, model, overwrite=True)
-        
-        exp.start(db)
-        client = Client(address=db.get_address()[0], cluster=False)
-        
-        # start simulation (non-blocking)
-        exp.start(model, block=False, summary=True)
-        
-        # poll until simulation starts and then retrieve data
-        client.poll_key("cylinder", 200, 100)
-        cylinder = client.get_tensor("cylinder").astype(bool)
-        
-        for i in range(0, time_steps):
-            client.poll_key(f"data_{str(i)}", 10, 1000)
-            dataset = client.get_dataset(f"data_{str(i)}")
-            ux, uy = dataset.get_tensor("ux"), dataset.get_tensor("uy")
-        
-            # analysis/plotting code omitted
-        
-        exp.stop(db)
-        ```
-        
-        For more examples of how to use SmartSim and SmartRedis together to perform
-        online analysis, please see the
-        [online analsysis tutorial section](https://www.craylabs.org/docs/tutorials/online_analysis/lattice/online_analysis.html) of the
-        SmartSim documentation.
-        
-        ## Online Processing
-        
-        Each of the SmartRedis clients can be used to remotely execute
-        [TorchScript](https://pytorch.org/docs/stable/jit.html) code on data
-        stored within the database. The scripts/functions are executed in the Torch
-        runtime linked into the database.
-        
-        Any of the functions available in the
-        [TorchScript builtins](https://pytorch.org/docs/stable/jit_builtin_functions.html#builtin-functions)
-        can be saved as "script" or "functions" in the database and used directly by
-        any of the SmartRedis Clients.
-        
-        ### Singular Value Decomposition
-        
-        For example, the following code sends the built-in
-        [Singular Value Decomposition](https://pytorch.org/docs/stable/generated/torch.svd.html)
-        to the database and execute it on a dummy tensor.
-        
-        ```python
-        import numpy as np
-        from smartredis import Client
-        
-        # don't even need to import torch
-        def calc_svd(input_tensor):
-            return input_tensor.svd()
-        
-        
-        # connect a client to the database
-        client = Client(cluster=False)
-        
-        # get dummy data
-        tensor = np.random.randint(0, 100, size=(5, 3, 2)).astype(np.float32)
-        
-        client.put_tensor("input", tensor)
-        client.set_function("svd", calc_svd)
-        
-        client.run_script("svd", "calc_svd", "input", ["U", "S", "V"])
-        # results are not retrieved immediately in case they need
-        # to be fed to another function/model
-        
-        U = client.get_tensor("U")
-        S = client.get_tensor("S")
-        V = client.get_tensor("V")
-        print(f"U: {U}, S: {S}, V: {V}")
-        ```
-        
-        The processing capabilities make it simple to form computational pipelines of
-        functions, scripts, and models.
-        
-        See the full [TorchScript Language Reference](https://pytorch.org/docs/stable/jit.html#torchscript-language)
-        documentation for more information on available methods, functions, and how
-        to create your own.
-        
-        ## Online Inference
-        
-        SmartSim supports the following frameworks for querying Machine Learning models
-        from C, C++, Fortran and Python with the SmartRedis Clients:
-        
-        <table>
-          <thead>
-            <tr>
-              <th style="text-align:center">RedisAI Version</th>
-              <th style="text-align:center">Libraries</th>
-              <th style="text-align:center">Supported Version</th>
-            </tr>
-          </thead>
-          <tbody style="text-align:center">
-            <tr>
-              <td rowspan="3">1.2.7</td>
-              <td>PyTorch</td>
-              <td>2.0.1</td>
-            </tr>
-            <tr>
-              <td>TensorFlow\Keras</td>
-              <td>2.13.1</td>
-            </tr>
-            <tr>
-              <td>ONNX</td>
-              <td>1.14.1</td>
-            </tr>
-          </tbody>
-        </table>
-        
-        A [number of other libraries](https://github.com/onnx/onnxmltools) are
-        supported through ONNX, like [SciKit-Learn](https://github.com/onnx/sklearn-onnx/)
-        and [XGBoost](https://github.com/onnx/onnxmltools/tree/master/tests/xgboost).
-        
-        **Note:** It's important to remember that SmartSim utilizes a client-server model. To run
-        experiments that utilize the above frameworks, you must first start the Orchestrator
-        database with SmartSim.
-        
-        ### PyTorch CNN Example
-        
-        The example below shows how to spin up a database with SmartSim and
-        invoke a PyTorch CNN model using the SmartRedis clients.
-        
-        ```python
-        # simple_torch_inference.py
-        import io
-        import torch
-        import torch.nn as nn
-        from smartredis import Client
-        from smartsim import Experiment
-        
-        exp = Experiment("simple-online-inference", launcher="local")
-        db = exp.create_database(port=6780, interface="lo")
-        
-        class Net(nn.Module):
-            def __init__(self):
-                super().__init__()
-                self.conv = nn.Conv2d(1, 1, 3)
-        
-            def forward(self, x):
-                return self.conv(x)
-        
-        torch_model = Net()
-        example_forward_input = torch.rand(1, 1, 3, 3)
-        module = torch.jit.trace(torch_model, example_forward_input)
-        model_buffer = io.BytesIO()
-        torch.jit.save(module, model_buffer)
-        
-        exp.start(db, summary=True)
-        
-        address = db.get_address()[0]
-        client = Client(address=address, cluster=False)
-        
-        client.put_tensor("input", example_forward_input.numpy())
-        client.set_model("cnn", model_buffer.getvalue(), "TORCH", device="CPU")
-        client.run_model("cnn", inputs=["input"], outputs=["output"])
-        output = client.get_tensor("output")
-        print(f"Prediction: {output}")
-        
-        exp.stop(db)
-        ```
-        
-        The above python code can be run like any normal python script:
-        ```bash
-        python simple_torch_inference.py
-        ```
-        
-        For more examples of how to use SmartSim and SmartRedis together to perform
-        online inference, please see the
-        [online inference tutorials section](https://www.craylabs.org/docs/tutorials/ml_inference/Inference-in-SmartSim.html) of the
-        SmartSim documentation.
-        
-        --------
-        
-        # Publications
-        
-        The following are public presentations or publications using SmartSim
-        
-         - [Collaboration with NCAR - CGD Seminar](https://www.youtube.com/watch?v=2e-5j427AS0)
-         - [SmartSim: Using Machine Learning in HPC Simulations](https://arxiv.org/abs/2104.09355)
-         - [SmartSim: Online Analytics and Machine Learning for HPC Simulations](https://www.youtube.com/watch?v=JsSgq-fq44w&list=PLuQQBBQFfpgq0OvjKbjcYgTDzDxTqtwua&index=11)
-         - [PyTorch Ecosystem Day Poster](https://assets.pytorch.org/pted2021/posters/J8.png)
-        
-        
-        --------
-        # Cite
-        
-        Please use the following citation when referencing SmartSim, SmartRedis, or any SmartSim related work:
-        
-        Partee et al., “Using Machine Learning at Scale in HPC Simulations with SmartSim:
-        An Application to Ocean Climate Modeling”, Journal of Computational Science, Volume 62, 2022, 101707, ISSN 1877-7503
-        
-        Available: https://doi.org/10.1016/j.jocs.2022.101707.
-        
-        ## bibtex
-        
-        
-        ```latex
-        @article{PARTEE2022101707,
-            title = {Using Machine Learning at scale in numerical simulations with SmartSim: An application to ocean climate modeling},
-            journal = {Journal of Computational Science},
-            volume = {62},
-            pages = {101707},
-            year = {2022},
-            issn = {1877-7503},
-            doi = {https://doi.org/10.1016/j.jocs.2022.101707},
-            url = {https://www.sciencedirect.com/science/article/pii/S1877750322001065},
-            author = {Sam Partee and Matthew Ellis and Alessandro Rigazzi and Andrew E. Shao and Scott Bachman and Gustavo Marques and Benjamin Robbins},
-            keywords = {Deep learning, Numerical simulation, Climate modeling, High performance computing, SmartSim},
-        }
-        ```
-        
 Keywords: scientific,ai,workflow,hpc,analysis
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: <3.12,>=3.8
+Requires-Python: <3.12,>=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: mypy
 Provides-Extra: ml
+License-File: LICENSE.md
+
+
+
+<div align="center">
+    <a href="https://github.com/CrayLabs/SmartSim"><img src="https://raw.githubusercontent.com/CrayLabs/SmartSim/master/doc/images/SmartSim_Large.png" width="90%"><img></a>
+    <br />
+    <br />
+<div display="inline-block">
+    <a href="https://github.com/CrayLabs/SmartSim"><b>Home</b></a>&nbsp;&nbsp;&nbsp;
+    <a href="https://www.craylabs.org/docs/installation_instructions/basic.html"><b>Install</b></a>&nbsp;&nbsp;&nbsp;
+    <a href="https://www.craylabs.org/docs/overview.html"><b>Documentation</b></a>&nbsp;&nbsp;&nbsp;
+    <a href="https://github.com/CrayLabs"><b>Cray Labs</b></a>&nbsp;&nbsp;&nbsp;
+    <a href="mailto:craylabs@hpe.com"><b>Contact</b></a>&nbsp;&nbsp;&nbsp;
+    <a href="https://join.slack.com/t/craylabs/shared_invite/zt-nw3ag5z5-5PS4tIXBfufu1bIvvr71UA"><b>Join us on Slack!</b></a>&nbsp;&nbsp;&nbsp;
+  </div>
+    <br />
+    <br />
+</div>
+
+
+<div align="center">
+
+[![License](https://img.shields.io/github/license/CrayLabs/SmartSim)](https://github.com/CrayLabs/SmartSim/blob/master/LICENSE.md)
+![GitHub last commit](https://img.shields.io/github/last-commit/CrayLabs/SmartSim)
+![GitHub deployments](https://img.shields.io/github/deployments/CrayLabs/SmartSim/github-pages?label=doc%20build)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/smartsim)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/smartsim)
+![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/CrayLabs/SmartSim)
+![Language](https://img.shields.io/github/languages/top/CrayLabs/SmartSim)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![codecov](https://codecov.io/gh/CrayLabs/SmartSim/branch/develop/graph/badge.svg?token=96HFI2F45E)](https://codecov.io/gh/CrayLabs/SmartSim)
+[![Downloads](https://static.pepy.tech/personalized-badge/smartsim?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/smartsim)
+
+</div>
+
+------------
+
+# SmartSim
+
+SmartSim is made up of two parts
+  1. SmartSim Infrastructure Library (This repository)
+  2. [SmartRedis](https://github.com/CrayLabs/SmartRedis)
+
+The two library components are designed to work together, but can also be used
+independently.
+
+*SmartSim* is a workflow library that makes it easier to use common Machine Learning (ML)
+libraries, like PyTorch and TensorFlow, in High Performance Computing (HPC) simulations
+and applications. SmartSim launches ML infrastructure on HPC systems alongside user
+workloads.
+
+*SmartRedis* provides an API to connect HPC workloads, particularly (MPI + X) simulations,
+to the ML infrastructure, namely the The [Orchestrator database](https://www.craylabs.org/docs/orchestrator.html),
+launched by SmartSim.
+
+Applications integrated with the SmartRedis clients, written in Fortran, C, C++ and Python,
+can send data to and remotely request SmartSim infrastructure to execute ML models and scripts
+on GPU or CPU. The distributed Client-Server paradigm allows for data to be seamlessly
+exchanged between applications at runtime without the utilization of MPI.
+
+----------
+
+**Table of Contents**
+- [SmartSim](#smartsim)
+- [Quick Start](#quick-start)
+- [SmartSim Infrastructure Library](#smartsim-infrastructure-library)
+  - [Experiments](#experiments)
+    - [Hello World](#hello-world)
+    - [Hello World MPI](#hello-world-mpi)
+  - [Experiments on HPC Systems](#experiments-on-hpc-systems)
+    - [Interactive Launch Example](#interactive-launch-example)
+    - [Batch Launch Examples](#batch-launch-examples)
+- [Infrastructure Library Applications](#infrastructure-library-applications)
+  - [Redis + RedisAI](#redis--redisai)
+    - [Local Launch](#local-launch)
+    - [Interactive Launch](#interactive-launch)
+    - [Batch Launch](#batch-launch)
+- [SmartRedis](#smartredis)
+  - [Tensors](#tensors)
+  - [Datasets](#datasets)
+- [SmartSim + SmartRedis Tutorials](#smartsim--smartredis-tutorials)
+  - [Run the Tutorials](#run-the-tutorials)
+  - [Online Analysis](#online-analysis)
+      - [Lattice Boltzmann Simulation](#lattice-boltzmann-simulation)
+  - [Online Processing](#online-processing)
+    - [Singular Value Decomposition](#singular-value-decomposition)
+  - [Online Inference](#online-inference)
+    - [PyTorch CNN Example](#pytorch-cnn-example)
+- [Publications](#publications)
+- [Cite](#cite)
+  - [bibtex](#bibtex)
+
+----
+
+# Quick Start
+
+
+The documentation has a number of tutorials that make it easy to get used to SmartSim locally
+before using it on your system. Each tutorial is a Jupyter notebook that can be run through the
+[SmartSim Tutorials docker image](https://github.com/orgs/CrayLabs/packages?repo_name=SmartSim)
+which will run a jupyter lab with the tutorials, SmartSim, and SmartRedis installed.
+
+```bash
+docker pull ghcr.io/craylabs/smartsim-tutorials:latest
+docker run -p 8888:8888 ghcr.io/craylabs/smartsim-tutorials:latest
+# click on link to open jupyter lab
+```
+
+# SmartSim Infrastructure Library
+
+The Infrastructure Library (IL), the ``smartsim`` python package,
+facilitates the launch of Machine Learning and simulation
+workflows. The Python interface of the IL creates, configures, launches and monitors
+applications.
+
+## Experiments
+
+The [Experiment](https://www.craylabs.org/docs/api/smartsim_api.html#experiment) object
+is the main interface of SmartSim. Through the [Experiment](https://www.craylabs.org/docs/api/smartsim_api.html#experiment)
+users can create references to user applications called ``Models``.
+### Hello World
+
+Below is a simple example of a workflow that uses the IL to launch hello world
+program using the local launcher which is designed for laptops and single nodes.
+
+```python
+from smartsim import Experiment
+
+exp = Experiment("simple", launcher="local")
+
+settings = exp.create_run_settings("echo", exe_args="Hello World")
+model = exp.create_model("hello_world", settings)
+
+exp.start(model, block=True)
+print(exp.get_status(model))
+```
+
+### Hello World MPI
+
+The [Experiment.create_run_settings](https://www.craylabs.org/docs/api/smartsim_api.html#smartsim.experiment.Experiment.create_run_settings) method returns a ``RunSettings`` object which
+defines how a model is launched. There are many types of ``RunSettings`` [supported by
+SmartSim](https://www.craylabs.org/docs/api/smartsim_api.html#settings).
+
+ - ``RunSettings``
+ - ``MpirunSettings``
+ - ``SrunSettings``
+ - ``AprunSettings``
+ - ``JsrunSettings``
+
+The following example launches a hello world MPI program using the local launcher
+for single compute node, workstations and laptops.
+
+```Python
+from smartsim import Experiment
+
+exp = Experiment("hello_world", launcher="local")
+mpi_settings = exp.create_run_settings(exe="echo",
+                                       exe_args="Hello World!",
+                                       run_command="mpirun")
+mpi_settings.set_tasks(4)
+
+mpi_model = exp.create_model("hello_world", mpi_settings)
+
+exp.start(mpi_model, block=True)
+print(exp.get_status(model))
+```
+
+If an argument of `run_command="auto"` (the default) is passed to
+`Experiment.create_run_settings`, SmartSim will attempt to find a run command on the
+system with which it has a corresponding `RunSettings` class. If one can be found,
+`Experiment.create_run_settings` will instance and return an object of that type.
+
+
+-----------
+## Experiments on HPC Systems
+
+SmartSim integrates with common HPC schedulers providing batch and interactive
+launch capabilities for all applications:
+
+ - Slurm
+ - LSF
+ - PBSPro
+ - Local (for laptops/single node, no batch)
+
+In addition, on Slurm and PBS systems, [Dragon](https://dragonhpc.github.io/dragon/doc/_build/html/index.html)
+can be used as a launcher. Please refer to the documentation for instructions on
+how to insall it on your system and use it in SmartSim.
+
+
+### Interactive Launch Example
+
+The following launches the same ``hello_world`` model in an interactive allocation.
+
+```bash
+# get interactive allocation (Slurm)
+salloc -N 3 --ntasks-per-node=20 --ntasks 60 --exclusive -t 00:10:00
+
+# get interactive allocation (PBS)
+qsub -l select=3:ncpus=20 -l walltime=00:10:00 -l place=scatter -I -q <queue>
+
+# get interactive allocation (LSF)
+bsub -Is -W 00:10 -nnodes 3 -P <project> $SHELL
+```
+
+This same script will run on a SLURM, PBS, or LSF system as the ``launcher``
+is set to `auto` in the [Experiment](https://www.craylabs.org/docs/api/smartsim_api.html#experiment)
+initialization. The run command like ``mpirun``,
+``aprun`` or ``srun`` will be automatically detected from what is available on the
+system.
+
+```python
+# hello_world.py
+from smartsim import Experiment
+
+exp = Experiment("hello_world_exp", launcher="auto")
+run = exp.create_run_settings(exe="echo", exe_args="Hello World!")
+run.set_tasks(60)
+run.set_tasks_per_node(20)
+
+model = exp.create_model("hello_world", run)
+exp.start(model, block=True, summary=True)
+
+print(exp.get_status(model))
+```
+```bash
+# in interactive terminal
+python hello_world.py
+```
+
+
+This script could also be launched in a batch file instead of an
+interactive terminal. For example, for Slurm:
+
+```bash
+#!/bin/bash
+#SBATCH --exclusive
+#SBATCH --nodes=3
+#SBATCH --ntasks-per-node=20
+#SBATCH --time=00:10:00
+
+python /path/to/hello_world.py
+```
+```bash
+# on Slurm system
+sbatch run_hello_world.sh
+```
+
+
+### Batch Launch Examples
+
+SmartSim can also launch workloads in a batch directly from Python, without the need
+for a batch script. Users can launch groups of ``Model`` instances in a ``Ensemble``.
+
+The following launches 4 replicas of the the same ``hello_world`` model.
+
+```python
+# hello_ensemble.py
+from smartsim import Experiment
+
+exp = Experiment("hello_world_batch", launcher="auto")
+
+# define resources for all ensemble members
+batch = exp.create_batch_settings(nodes=4, time="00:10:00", account="12345-Cray")
+batch.set_queue("premium")
+
+# define how each member should run
+run = exp.create_run_settings(exe="echo", exe_args="Hello World!")
+run.set_tasks(60)
+run.set_tasks_per_node(20)
+
+ensemble = exp.create_ensemble("hello_world",
+                               batch_settings=batch,
+                               run_settings=run,
+                               replicas=4)
+exp.start(ensemble, block=True, summary=True)
+
+print(exp.get_status(ensemble))
+```
+
+```bash
+python hello_ensemble.py
+```
+
+Similar to the interactive example, this same script will run on a SLURM, PBS,
+or LSF system as the ``launcher`` is set to `auto` in the
+[Experiment](https://www.craylabs.org/docs/api/smartsim_api.html#experiment)
+initialization. Local launching does not support batch workloads.
+
+
+--------
+
+# Infrastructure Library Applications
+ - Orchestrator - In-memory data store and Machine Learning Inference (Redis + RedisAI)
+
+## Redis + RedisAI
+
+The ``Orchestrator`` is an in-memory database that utilizes Redis and RedisAI to provide
+a distributed database and access to ML runtimes from Fortran, C, C++ and Python.
+
+SmartSim provides classes that make it simple to launch the database in many
+configurations and optionally form a distributed database cluster. The examples
+below will show how to launch the database. Later in this document we will show
+how to use the database to perform ML inference and processing.
+
+
+### Local Launch
+
+The following script launches a single database using the local launcher.
+
+[Experiment.create_database](https://www.craylabs.org/docs/api/smartsim_api.html#smartsim.experiment.Experiment.create_database)
+will initialize an ``Orchestrator`` instance corresponding to the specified launcher.
+
+```python
+# run_db_local.py
+from smartsim import Experiment
+
+exp = Experiment("local-db", launcher="local")
+db = exp.create_database(port=6780,       # database port
+                         interface="lo")  # network interface to use
+
+# by default, SmartSim never blocks execution after the database is launched.
+exp.start(db)
+
+# launch models, analysis, training, inference sessions, etc
+# that communicate with the database using the SmartRedis clients
+
+# stop the database
+exp.stop(db)
+```
+
+### Interactive Launch
+
+The ``Orchestrator``, like ``Ensemble`` instances, can be launched locally, in interactive
+allocations, or in a batch.
+
+The following example launches a distributed (3 node) database cluster
+in an interactive allocation.
+
+
+```bash
+# get interactive allocation (Slurm)
+salloc -N 3 --ntasks-per-node=1 --exclusive -t 00:10:00
+
+# get interactive allocation (PBS)
+qsub -l select=3:ncpus=1 -l walltime=00:10:00 -l place=scatter -I -q queue
+
+# get interactive allocation (LSF)
+bsub -Is -W 00:10 -nnodes 3 -P project $SHELL
+
+```
+
+```python
+# run_db.py
+from smartsim import Experiment
+
+# auto specified to work across launcher types
+exp = Experiment("db-on-slurm", launcher="auto")
+db_cluster = exp.create_database(db_nodes=3,
+                                 db_port=6780,
+                                 batch=False,
+                                 interface="ipogif0")
+exp.start(db_cluster)
+
+print(f"Orchestrator launched on nodes: {db_cluster.hosts}")
+# launch models, analysis, training, inference sessions, etc
+# that communicate with the database using the SmartRedis clients
+
+exp.stop(db_cluster)
+```
+```bash
+# in interactive terminal
+python run_db.py
+```
+
+### Batch Launch
+
+The ``Orchestrator`` can also be launched in a batch without the need for an interactive allocation.
+SmartSim will create the batch file, submit it to the batch system, and then wait for the database
+to be launched. Users can hit CTRL-C to cancel the launch if needed.
+
+```Python
+# run_db_batch.py
+from smartsim import Experiment
+
+exp = Experiment("batch-db-on-pbs", launcher="auto")
+db_cluster = exp.create_database(db_nodes=3,
+                                 db_port=6780,
+                                 batch=True,
+                                 time="00:10:00",
+                                 interface="ib0",
+                                 account="12345-Cray",
+                                 queue="cl40")
+
+exp.start(db_cluster)
+
+print(f"Orchestrator launched on nodes: {db_cluster.hosts}")
+# launch models, analysis, training, inference sessions, etc
+# that communicate with the database using the SmartRedis clients
+
+exp.stop(db_cluster)
+```
+
+```bash
+python run_db_batch.py
+```
+
+------
+# SmartRedis
+
+The SmartSim IL Clients ([SmartRedis](https://github.com/CrayLabs/SmartRedis))
+are implementations of Redis clients that implement the RedisAI
+API with additions specific to scientific workflows.
+
+SmartRedis clients are available in Fortran, C, C++, and Python.
+Users can seamlessly pull and push data from the Orchestrator from different languages.
+
+## Tensors
+
+Tensors are the fundamental data structure for the SmartRedis clients. The Clients
+use the native array format of the language. For example, in Python, a tensor is
+a NumPy array while the C/C++ clients accept nested and contiguous arrays.
+
+When stored in the database, all tensors are stored in the same format. Hence,
+any language can receive a tensor from the database no matter what supported language
+the array was sent from. This enables applications in different languages to communicate
+numerical data with each other at runtime.
+
+For more information on the tensor data structure, see
+[the documentation](https://www.craylabs.org/docs/sr_data_structures.html#tensor)
+
+## Datasets
+
+Datasets are collections of Tensors and associated metadata. The ``Dataset`` class
+is a user space object that can be created, added to, sent to, and retrieved from
+the Orchestrator.
+
+For an example of how to use the ``Dataset`` class, see the [Online Analysis example](#online-analysis)
+
+For more information on the API, see the
+[API documentation](https://www.craylabs.org/docs/sr_data_structures.html#dataset)
+
+# SmartSim + SmartRedis Tutorials
+
+SmartSim and SmartRedis were designed to work together. When launched through
+SmartSim, applications using the SmartRedis clients are directly connected to
+any Orchestrator launched in the same [Experiment](https://www.craylabs.org/docs/api/smartsim_api.html#experiment).
+
+In this way, a SmartSim [Experiment](https://www.craylabs.org/docs/api/smartsim_api.html#experiment) becomes a driver for coupled ML and Simulation
+workflows. The following are simple examples of how to use SmartSim and SmartRedis
+together.
+
+## Run the Tutorials
+
+Each tutorial is a Jupyter notebook that can be run through the
+[SmartSim Tutorials docker image](https://github.com/orgs/CrayLabs/packages?repo_name=SmartSim)
+which will run a jupyter lab with the tutorials, SmartSim, and SmartRedis installed.
+
+```bash
+docker pull ghcr.io/craylabs/smartsim-tutorials:latest
+docker run -p 8888:8888 ghcr.io/craylabs/smartsim-tutorials:latest
+```
+Each of the following examples can be found in the
+[SmartSim documentation](https://www.craylabs.org/docs/tutorials/getting_started/getting_started.html).
+
+## Online Analysis
+
+Using SmartSim, HPC applications can be monitored in real time by streaming data
+from the application to the database. SmartRedis clients can retrieve the
+data, process, analyze it, and finally store any updated data back to the database for
+use by other clients.
+
+The following is an example of how a user could monitor and analyze a simulation.
+The example here uses the Python client; however, SmartRedis clients are also available
+for C, C++, and Fortran. All SmartRedis clients implement the same API.
+
+The example will produce [this visualization](https://user-images.githubusercontent.com/13009163/127622717-2c9e4cfd-50f4-4d94-88c4-8c05fa2fa616.mp4) while the simulation is running.
+
+#### Lattice Boltzmann Simulation
+
+Using a [Lattice Boltzmann Simulation](https://en.wikipedia.org/wiki/Lattice_Boltzmann_methods),
+this example demonstrates how to use the SmartRedis ``Dataset`` API to stream
+data over the Orchestrator deployed by SmartSim.
+
+The simulation will be composed of two parts: `fv_sim.py` which will generate data from
+the Simulation and store it in the Orchestrator, and `driver.py`
+which will launch the Orchestrator, start `fv_sim.py` and check for data posted to the
+Orchestrator to plot updates in real-time.
+
+The following code highlights the sections of `fv_sim.py` that are responsible for
+transmitting the data needed to plot timesteps of the simulation to the Orchestrator.
+
+```Python
+# fv_sim.py
+from smartredis import Client
+import numpy as np
+
+# initialization code omitted
+
+# save cylinder location to database
+cylinder = (X - x_res/4)**2 + (Y - y_res/2)**2 < (y_res/4)**2 # bool array
+client.put_tensor("cylinder", cylinder.astype(np.int8))
+
+for time_step in range(steps): # simulation loop
+    for i, cx, cy in zip(idxs, cxs, cys):
+        F[:,:,i] = np.roll(F[:,:,i], cx, axis=1)
+        F[:,:,i] = np.roll(F[:,:,i], cy, axis=0)
+
+    bndryF = F[cylinder,:]
+    bndryF = bndryF[:,[0,5,6,7,8,1,2,3,4]]
+
+    rho = np.sum(F, 2)
+    ux  = np.sum(F * cxs, 2) / rho
+    uy  = np.sum(F * cys, 2) / rho
+
+    Feq = np.zeros(F.shape)
+    for i, cx, cy, w in zip(idxs, cxs, cys, weights):
+        Feq[:,:,i] = rho * w * ( 1 + 3*(cx*ux+cy*uy)  + 9*(cx*ux+cy*uy)**2/2 - 3*(ux**2+uy**2)/2 )
+    F += -(1.0/tau) * (F - Feq)
+    F[cylinder,:] = bndryF
+
+    # Create a SmartRedis dataset with vorticity data
+    dataset = Dataset(f"data_{str(time_step)}")
+    dataset.add_tensor("ux", ux)
+    dataset.add_tensor("uy", uy)
+
+    # Put Dataset in db at key "data_{time_step}"
+    client.put_dataset(dataset)
+```
+
+The driver script, `driver.py`, launches the Orchestrator database and runs
+the simulation in a non-blocking fashion. The driver script then uses the SmartRedis
+client to pull the DataSet and plot the vorticity while the simulation is running.
+
+```Python
+# driver.py
+time_steps, seed = 3000, 42
+
+exp = Experiment("finite_volume_simulation", launcher="local")
+
+db = exp.create_database(port=6780,        # database port
+                         interface="lo")   # network interface db should listen on
+
+# create the lb simulation Model reference
+settings = exp.create_run_settings("python",
+                                   exe_args=["fv_sim.py",
+                                             f"--seed={seed}",
+                                             f"--steps={time_steps}"])
+model = exp.create_model("fv_simulation", settings)
+model.attach_generator_files(to_copy="fv_sim.py")
+exp.generate(db, model, overwrite=True)
+
+exp.start(db)
+client = Client(address=db.get_address()[0], cluster=False)
+
+# start simulation (non-blocking)
+exp.start(model, block=False, summary=True)
+
+# poll until simulation starts and then retrieve data
+client.poll_key("cylinder", 200, 100)
+cylinder = client.get_tensor("cylinder").astype(bool)
+
+for i in range(0, time_steps):
+    client.poll_key(f"data_{str(i)}", 10, 1000)
+    dataset = client.get_dataset(f"data_{str(i)}")
+    ux, uy = dataset.get_tensor("ux"), dataset.get_tensor("uy")
+
+    # analysis/plotting code omitted
+
+exp.stop(db)
+```
+
+For more examples of how to use SmartSim and SmartRedis together to perform
+online analysis, please see the
+[online analsysis tutorial section](https://www.craylabs.org/docs/tutorials/online_analysis/lattice/online_analysis.html) of the
+SmartSim documentation.
+
+## Online Processing
+
+Each of the SmartRedis clients can be used to remotely execute
+[TorchScript](https://pytorch.org/docs/stable/jit.html) code on data
+stored within the database. The scripts/functions are executed in the Torch
+runtime linked into the database.
+
+Any of the functions available in the
+[TorchScript builtins](https://pytorch.org/docs/stable/jit_builtin_functions.html#builtin-functions)
+can be saved as "script" or "functions" in the database and used directly by
+any of the SmartRedis Clients.
+
+### Singular Value Decomposition
+
+For example, the following code sends the built-in
+[Singular Value Decomposition](https://pytorch.org/docs/stable/generated/torch.svd.html)
+to the database and execute it on a dummy tensor.
+
+```python
+import numpy as np
+from smartredis import Client
+
+# don't even need to import torch
+def calc_svd(input_tensor):
+    return input_tensor.svd()
+
+
+# connect a client to the database
+client = Client(cluster=False)
+
+# get dummy data
+tensor = np.random.randint(0, 100, size=(5, 3, 2)).astype(np.float32)
+
+client.put_tensor("input", tensor)
+client.set_function("svd", calc_svd)
+
+client.run_script("svd", "calc_svd", "input", ["U", "S", "V"])
+# results are not retrieved immediately in case they need
+# to be fed to another function/model
+
+U = client.get_tensor("U")
+S = client.get_tensor("S")
+V = client.get_tensor("V")
+print(f"U: {U}, S: {S}, V: {V}")
+```
+
+The processing capabilities make it simple to form computational pipelines of
+functions, scripts, and models.
+
+See the full [TorchScript Language Reference](https://pytorch.org/docs/stable/jit.html#torchscript-language)
+documentation for more information on available methods, functions, and how
+to create your own.
+
+## Online Inference
+
+SmartSim supports the following frameworks for querying Machine Learning models
+from C, C++, Fortran and Python with the SmartRedis Clients:
+
+<table>
+  <thead>
+    <tr>
+      <th style="text-align:center">RedisAI Version</th>
+      <th style="text-align:center">Libraries</th>
+      <th style="text-align:center">Supported Version</th>
+    </tr>
+  </thead>
+  <tbody style="text-align:center">
+    <tr>
+      <td rowspan="3">1.2.7</td>
+      <td>PyTorch</td>
+      <td>2.0.1</td>
+    </tr>
+    <tr>
+      <td>TensorFlow\Keras</td>
+      <td>2.13.1</td>
+    </tr>
+    <tr>
+      <td>ONNX</td>
+      <td>1.14.1</td>
+    </tr>
+  </tbody>
+</table>
+
+A [number of other libraries](https://github.com/onnx/onnxmltools) are
+supported through ONNX, like [SciKit-Learn](https://github.com/onnx/sklearn-onnx/)
+and [XGBoost](https://github.com/onnx/onnxmltools/tree/master/tests/xgboost).
+
+**Note:** It's important to remember that SmartSim utilizes a client-server model. To run
+experiments that utilize the above frameworks, you must first start the Orchestrator
+database with SmartSim.
+
+### PyTorch CNN Example
+
+The example below shows how to spin up a database with SmartSim and
+invoke a PyTorch CNN model using the SmartRedis clients.
+
+```python
+# simple_torch_inference.py
+import io
+import torch
+import torch.nn as nn
+from smartredis import Client
+from smartsim import Experiment
+
+exp = Experiment("simple-online-inference", launcher="local")
+db = exp.create_database(port=6780, interface="lo")
+
+class Net(nn.Module):
+    def __init__(self):
+        super().__init__()
+        self.conv = nn.Conv2d(1, 1, 3)
+
+    def forward(self, x):
+        return self.conv(x)
+
+torch_model = Net()
+example_forward_input = torch.rand(1, 1, 3, 3)
+module = torch.jit.trace(torch_model, example_forward_input)
+model_buffer = io.BytesIO()
+torch.jit.save(module, model_buffer)
+
+exp.start(db, summary=True)
+
+address = db.get_address()[0]
+client = Client(address=address, cluster=False)
+
+client.put_tensor("input", example_forward_input.numpy())
+client.set_model("cnn", model_buffer.getvalue(), "TORCH", device="CPU")
+client.run_model("cnn", inputs=["input"], outputs=["output"])
+output = client.get_tensor("output")
+print(f"Prediction: {output}")
+
+exp.stop(db)
+```
+
+The above python code can be run like any normal python script:
+```bash
+python simple_torch_inference.py
+```
+
+For more examples of how to use SmartSim and SmartRedis together to perform
+online inference, please see the
+[online inference tutorials section](https://www.craylabs.org/docs/tutorials/ml_inference/Inference-in-SmartSim.html) of the
+SmartSim documentation.
+
+--------
+
+# Publications
+
+The following are public presentations or publications using SmartSim
+
+ - [Collaboration with NCAR - CGD Seminar](https://www.youtube.com/watch?v=2e-5j427AS0)
+ - [SmartSim: Using Machine Learning in HPC Simulations](https://arxiv.org/abs/2104.09355)
+ - [SmartSim: Online Analytics and Machine Learning for HPC Simulations](https://www.youtube.com/watch?v=JsSgq-fq44w&list=PLuQQBBQFfpgq0OvjKbjcYgTDzDxTqtwua&index=11)
+ - [PyTorch Ecosystem Day Poster](https://assets.pytorch.org/pted2021/posters/J8.png)
+
+
+--------
+# Cite
+
+Please use the following citation when referencing SmartSim, SmartRedis, or any SmartSim related work:
+
+Partee et al., “Using Machine Learning at Scale in HPC Simulations with SmartSim:
+An Application to Ocean Climate Modeling”, Journal of Computational Science, Volume 62, 2022, 101707, ISSN 1877-7503
+
+Available: https://doi.org/10.1016/j.jocs.2022.101707.
+
+## bibtex
+
+
+```latex
+@article{PARTEE2022101707,
+    title = {Using Machine Learning at scale in numerical simulations with SmartSim: An application to ocean climate modeling},
+    journal = {Journal of Computational Science},
+    volume = {62},
+    pages = {101707},
+    year = {2022},
+    issn = {1877-7503},
+    doi = {https://doi.org/10.1016/j.jocs.2022.101707},
+    url = {https://www.sciencedirect.com/science/article/pii/S1877750322001065},
+    author = {Sam Partee and Matthew Ellis and Alessandro Rigazzi and Andrew E. Shao and Scott Bachman and Gustavo Marques and Benjamin Robbins},
+    keywords = {Deep learning, Numerical simulation, Climate modeling, High performance computing, SmartSim},
+}
+```
+
+
```

#### html2text {}

```diff
@@ -1,12 +1,19 @@
-Metadata-Version: 2.1 Name: smartsim Version: 0.6.2 Summary: AI Workflows for
+Metadata-Version: 2.1 Name: smartsim Version: 0.7.0 Summary: AI Workflows for
 Science Home-page: https://github.com/CrayLabs/SmartSim Author: CrayLabs, a
 Hewlett Packard Enterprise OSS Organization Author-email: craylabs@hpe.com
 License: BSD 2-Clause License Project-URL: Source, https://github.com/CrayLabs/
-SmartSim Project-URL: Documentation, https://www.craylabs.org Description:
+SmartSim Project-URL: Documentation, https://www.craylabs.org Keywords:
+scientific,ai,workflow,hpc,analysis Platform: UNKNOWN Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
+Approved :: BSD License Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering Requires-Python: <3.12,>=3.9
+Description-Content-Type: text/markdown Provides-Extra: dev Provides-Extra:
+mypy Provides-Extra: ml License-File: LICENSE.md
     _[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_C_r_a_y_L_a_b_s_/_S_m_a_r_t_S_i_m_/_m_a_s_t_e_r_/_d_o_c_/_i_m_a_g_e_s_/
                           _S_m_a_r_t_S_i_m___L_a_r_g_e_._p_n_g_]_[_I_m_a_g_e_]
 
     _HH_oo_mm_ee    _II_nn_ss_tt_aa_ll_ll    _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn    _CC_rr_aa_yy_ _LL_aa_bb_ss    _CC_oo_nn_tt_aa_cc_tt    _JJ_oo_ii_nn_ _uu_ss_ _oo_nn
                                    _SS_ll_aa_cc_kk_!!   
 
 
@@ -91,61 +98,64 @@
 ("hello_world", mpi_settings) exp.start(mpi_model, block=True) print
 (exp.get_status(model)) ``` If an argument of `run_command="auto"` (the
 default) is passed to `Experiment.create_run_settings`, SmartSim will attempt
 to find a run command on the system with which it has a corresponding
 `RunSettings` class. If one can be found, `Experiment.create_run_settings` will
 instance and return an object of that type. ----------- ## Experiments on HPC
 Systems SmartSim integrates with common HPC schedulers providing batch and
-interactive launch capabilities for all applications. - Slurm - LSF - PBSPro -
-Local (for laptops/single node, no batch) ### Interactive Launch Example The
-following launches the same ``hello_world`` model in an interactive allocation.
-```bash # get interactive allocation (Slurm) salloc -N 3 --ntasks-per-node=20 -
--ntasks 60 --exclusive -t 00:10:00 # get interactive allocation (PBS) qsub -
-l select=3:ncpus=20 -l walltime=00:10:00 -l place=scatter -I -q # get
-interactive allocation (LSF) bsub -Is -W 00:10 -nnodes 3 -P $SHELL ``` This
-same script will run on a SLURM, PBS, or LSF system as the ``launcher`` is set
-to `auto` in the [Experiment](https://www.craylabs.org/docs/api/
-smartsim_api.html#experiment) initialization. The run command like ``mpirun``,
-``aprun`` or ``srun`` will be automatically detected from what is available on
-the system. ```python # hello_world.py from smartsim import Experiment exp =
-Experiment("hello_world_exp", launcher="auto") run = exp.create_run_settings
-(exe="echo", exe_args="Hello World!") run.set_tasks(60) run.set_tasks_per_node
-(20) model = exp.create_model("hello_world", run) exp.start(model, block=True,
-summary=True) print(exp.get_status(model)) ``` ```bash # in interactive
-terminal python hello_world.py ``` This script could also be launched in a
-batch file instead of an interactive terminal. For example, for Slurm: ```bash
-#!/bin/bash #SBATCH --exclusive #SBATCH --nodes=3 #SBATCH --ntasks-per-node=20
-#SBATCH --time=00:10:00 python /path/to/hello_world.py ``` ```bash # on Slurm
-system sbatch run_hello_world.sh ``` ### Batch Launch Examples SmartSim can
-also launch workloads in a batch directly from Python, without the need for a
-batch script. Users can launch groups of ``Model`` instances in a ``Ensemble``.
-The following launches 4 replicas of the the same ``hello_world`` model.
-```python # hello_ensemble.py from smartsim import Experiment exp = Experiment
-("hello_world_batch", launcher="auto") # define resources for all ensemble
-members batch = exp.create_batch_settings(nodes=4, time="00:10:00",
-account="12345-Cray") batch.set_queue("premium") # define how each member
-should run run = exp.create_run_settings(exe="echo", exe_args="Hello World!")
-run.set_tasks(60) run.set_tasks_per_node(20) ensemble = exp.create_ensemble
-("hello_world", batch_settings=batch, run_settings=run, replicas=4) exp.start
-(ensemble, block=True, summary=True) print(exp.get_status(ensemble)) ```
-```bash python hello_ensemble.py ``` Similar to the interactive example, this
-same script will run on a SLURM, PBS, or LSF system as the ``launcher`` is set
-to `auto` in the [Experiment](https://www.craylabs.org/docs/api/
-smartsim_api.html#experiment) initialization. Local launching does not support
-batch workloads. -------- # Infrastructure Library Applications - Orchestrator
-- In-memory data store and Machine Learning Inference (Redis + RedisAI) ##
-Redis + RedisAI The ``Orchestrator`` is an in-memory database that utilizes
-Redis and RedisAI to provide a distributed database and access to ML runtimes
-from Fortran, C, C++ and Python. SmartSim provides classes that make it simple
-to launch the database in many configurations and optionally form a distributed
-database cluster. The examples below will show how to launch the database.
-Later in this document we will show how to use the database to perform ML
-inference and processing. ### Local Launch The following script launches a
-single database using the local launcher. [Experiment.create_database](https://
-www.craylabs.org/docs/api/
+interactive launch capabilities for all applications: - Slurm - LSF - PBSPro -
+Local (for laptops/single node, no batch) In addition, on Slurm and PBS
+systems, [Dragon](https://dragonhpc.github.io/dragon/doc/_build/html/
+index.html) can be used as a launcher. Please refer to the documentation for
+instructions on how to insall it on your system and use it in SmartSim. ###
+Interactive Launch Example The following launches the same ``hello_world``
+model in an interactive allocation. ```bash # get interactive allocation
+(Slurm) salloc -N 3 --ntasks-per-node=20 --ntasks 60 --exclusive -t 00:10:00 #
+get interactive allocation (PBS) qsub -l select=3:ncpus=20 -l walltime=00:10:00
+-l place=scatter -I -q # get interactive allocation (LSF) bsub -Is -W 00:10 -
+nnodes 3 -P $SHELL ``` This same script will run on a SLURM, PBS, or LSF system
+as the ``launcher`` is set to `auto` in the [Experiment](https://
+www.craylabs.org/docs/api/smartsim_api.html#experiment) initialization. The run
+command like ``mpirun``, ``aprun`` or ``srun`` will be automatically detected
+from what is available on the system. ```python # hello_world.py from smartsim
+import Experiment exp = Experiment("hello_world_exp", launcher="auto") run =
+exp.create_run_settings(exe="echo", exe_args="Hello World!") run.set_tasks(60)
+run.set_tasks_per_node(20) model = exp.create_model("hello_world", run)
+exp.start(model, block=True, summary=True) print(exp.get_status(model)) ```
+```bash # in interactive terminal python hello_world.py ``` This script could
+also be launched in a batch file instead of an interactive terminal. For
+example, for Slurm: ```bash #!/bin/bash #SBATCH --exclusive #SBATCH --nodes=3
+#SBATCH --ntasks-per-node=20 #SBATCH --time=00:10:00 python /path/to/
+hello_world.py ``` ```bash # on Slurm system sbatch run_hello_world.sh ``` ###
+Batch Launch Examples SmartSim can also launch workloads in a batch directly
+from Python, without the need for a batch script. Users can launch groups of
+``Model`` instances in a ``Ensemble``. The following launches 4 replicas of the
+the same ``hello_world`` model. ```python # hello_ensemble.py from smartsim
+import Experiment exp = Experiment("hello_world_batch", launcher="auto") #
+define resources for all ensemble members batch = exp.create_batch_settings
+(nodes=4, time="00:10:00", account="12345-Cray") batch.set_queue("premium") #
+define how each member should run run = exp.create_run_settings(exe="echo",
+exe_args="Hello World!") run.set_tasks(60) run.set_tasks_per_node(20) ensemble
+= exp.create_ensemble("hello_world", batch_settings=batch, run_settings=run,
+replicas=4) exp.start(ensemble, block=True, summary=True) print(exp.get_status
+(ensemble)) ``` ```bash python hello_ensemble.py ``` Similar to the interactive
+example, this same script will run on a SLURM, PBS, or LSF system as the
+``launcher`` is set to `auto` in the [Experiment](https://www.craylabs.org/
+docs/api/smartsim_api.html#experiment) initialization. Local launching does not
+support batch workloads. -------- # Infrastructure Library Applications -
+Orchestrator - In-memory data store and Machine Learning Inference (Redis +
+RedisAI) ## Redis + RedisAI The ``Orchestrator`` is an in-memory database that
+utilizes Redis and RedisAI to provide a distributed database and access to ML
+runtimes from Fortran, C, C++ and Python. SmartSim provides classes that make
+it simple to launch the database in many configurations and optionally form a
+distributed database cluster. The examples below will show how to launch the
+database. Later in this document we will show how to use the database to
+perform ML inference and processing. ### Local Launch The following script
+launches a single database using the local launcher.
+[Experiment.create_database](https://www.craylabs.org/docs/api/
 smartsim_api.html#smartsim.experiment.Experiment.create_database) will
 initialize an ``Orchestrator`` instance corresponding to the specified
 launcher. ```python # run_db_local.py from smartsim import Experiment exp =
 Experiment("local-db", launcher="local") db = exp.create_database(port=6780, #
 database port interface="lo") # network interface to use # by default, SmartSim
 never blocks execution after the database is launched. exp.start(db) # launch
 models, analysis, training, inference sessions, etc # that communicate with the
@@ -332,15 +342,8 @@
 simulations with SmartSim: An application to ocean climate modeling}, journal =
 {Journal of Computational Science}, volume = {62}, pages = {101707}, year =
 {2022}, issn = {1877-7503}, doi = {https://doi.org/10.1016/j.jocs.2022.101707},
 url = {https://www.sciencedirect.com/science/article/pii/S1877750322001065},
 author = {Sam Partee and Matthew Ellis and Alessandro Rigazzi and Andrew E.
 Shao and Scott Bachman and Gustavo Marques and Benjamin Robbins}, keywords =
 {Deep learning, Numerical simulation, Climate modeling, High performance
-computing, SmartSim}, } ``` Keywords: scientific,ai,workflow,hpc,analysis
-Platform: UNKNOWN Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-License :: OSI Approved :: BSD License Classifier: Intended Audience ::
-Science/Research Classifier: Topic :: Scientific/Engineering Requires-Python:
-<3.12,>=3.8 Description-Content-Type: text/markdown Provides-Extra: dev
-Provides-Extra: mypy Provides-Extra: ml
+computing, SmartSim}, } ```
```

