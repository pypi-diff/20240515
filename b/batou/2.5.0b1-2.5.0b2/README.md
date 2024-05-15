# Comparing `tmp/batou-2.5.0b1.tar.gz` & `tmp/batou-2.5.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batou-2.5.0b1.tar", last modified: Fri Apr 19 05:17:23 2024, max compression
+gzip compressed data, was "batou-2.5.0b2.tar", last modified: Wed May 15 10:56:26 2024, max compression
```

## Comparing `batou-2.5.0b1.tar` & `batou-2.5.0b2.tar`

### file list

```diff
@@ -1,268 +1,268 @@
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.102186 batou-2.5.0b1/
--rw-r--r--   0 zagy       (501) staff       (20)    31241 2024-04-19 05:17:22.000000 batou-2.5.0b1/CHANGES.history.txt
--rw-r--r--   0 zagy       (501) staff       (20)     1608 2024-04-19 05:17:22.000000 batou-2.5.0b1/LICENSE.txt
--rw-r--r--   0 zagy       (501) staff       (20)      212 2024-04-19 05:17:22.000000 batou-2.5.0b1/MANIFEST.in
--rw-r--r--   0 zagy       (501) staff       (20)     3973 2024-04-19 05:17:23.102099 batou-2.5.0b1/PKG-INFO
--rw-r--r--   0 zagy       (501) staff       (20)     2691 2024-04-19 05:17:22.000000 batou-2.5.0b1/README.md
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.073315 batou-2.5.0b1/doc/
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.080193 batou-2.5.0b1/doc/source/
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.080741 batou-2.5.0b1/doc/source/api/
--rw-r--r--   0 zagy       (501) staff       (20)      886 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/api/component.txt
--rw-r--r--   0 zagy       (501) staff       (20)     2299 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/api/environment.txt
--rw-r--r--   0 zagy       (501) staff       (20)       48 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/api/templates.txt
--rw-r--r--   0 zagy       (501) staff       (20)       63 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/api/utilities.txt
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.080861 batou-2.5.0b1/doc/source/cli/
--rw-r--r--   0 zagy       (501) staff       (20)     4731 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/cli/index.txt
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.081564 batou-2.5.0b1/doc/source/components/
--rw-r--r--   0 zagy       (501) staff       (20)     1025 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/components/cmmi.txt
--rw-r--r--   0 zagy       (501) staff       (20)     2941 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/components/downloads-vcs.txt
--rw-r--r--   0 zagy       (501) staff       (20)     5657 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/components/files.txt
--rw-r--r--   0 zagy       (501) staff       (20)     4820 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/components/python.txt
--rw-r--r--   0 zagy       (501) staff       (20)     3050 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/components/services.txt
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.082032 batou-2.5.0b1/doc/source/dev/
--rw-r--r--   0 zagy       (501) staff       (20)      718 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/dev/authors.txt
--rw-r--r--   0 zagy       (501) staff       (20)     8555 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/dev/contributing.txt
--rw-r--r--   0 zagy       (501) staff       (20)     1711 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/dev/testing.txt
--rw-r--r--   0 zagy       (501) staff       (20)     2809 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/dev/todo.txt
--rw-r--r--   0 zagy       (501) staff       (20)     8498 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/index.txt
--rw-r--r--   0 zagy       (501) staff       (20)     4799 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/upgrading.txt
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.082699 batou-2.5.0b1/doc/source/user/
--rw-r--r--   0 zagy       (501) staff       (20)    10870 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/user/advanced.txt
--rw-r--r--   0 zagy       (501) staff       (20)     2565 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/user/install.txt
--rw-r--r--   0 zagy       (501) staff       (20)     3848 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/user/installation-deb.txt
--rw-r--r--   0 zagy       (501) staff       (20)     3798 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/user/installation-rpm.txt
--rw-r--r--   0 zagy       (501) staff       (20)     2907 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/user/intro.txt
--rw-r--r--   0 zagy       (501) staff       (20)    47505 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/user/quickstart.txt
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.075183 batou-2.5.0b1/examples/
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.082957 batou-2.5.0b1/examples/api/
--rw-r--r--   0 zagy       (501) staff       (20)      349 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/api/index.txt
--rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/api/requirements.txt
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.083060 batou-2.5.0b1/examples/django/
--rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/django/requirements.txt
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.083169 batou-2.5.0b1/examples/durations/
--rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/durations/requirements.txt
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.083272 batou-2.5.0b1/examples/errors/
--rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/errors/requirements.txt
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.083378 batou-2.5.0b1/examples/errors2/
--rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/errors2/requirements.txt
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.083486 batou-2.5.0b1/examples/errorsnohost/
--rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/errorsnohost/requirements.txt
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.083593 batou-2.5.0b1/examples/ignores/
--rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/ignores/requirements.txt
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.083704 batou-2.5.0b1/examples/largetempl/
--rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/largetempl/requirements.txt
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.083811 batou-2.5.0b1/examples/package/
--rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/package/requirements.txt
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.083913 batou-2.5.0b1/examples/sync_async/
--rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/sync_async/requirements.txt
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.084018 batou-2.5.0b1/examples/tutorial-buildout/
--rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/tutorial-buildout/requirements.txt
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.084123 batou-2.5.0b1/examples/tutorial-component/
--rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/tutorial-component/requirements.txt
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.084237 batou-2.5.0b1/examples/tutorial-helloworld/
--rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/tutorial-helloworld/requirements.txt
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.084345 batou-2.5.0b1/examples/tutorial-parallelize/
--rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/tutorial-parallelize/requirements.txt
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.084454 batou-2.5.0b1/examples/tutorial-provision-container/
--rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/tutorial-provision-container/requirements.txt
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.084561 batou-2.5.0b1/examples/tutorial-secrets/
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.074943 batou-2.5.0b1/examples/tutorial-secrets/environments/
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.084670 batou-2.5.0b1/examples/tutorial-secrets/environments/age/
--rw-r--r--   0 zagy       (501) staff       (20)     2269 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/tutorial-secrets/environments/age/age_keys.txt
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.084787 batou-2.5.0b1/examples/tutorial-secrets/environments/age-diffable/
--rw-r--r--   0 zagy       (501) staff       (20)     2269 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/tutorial-secrets/environments/age-diffable/age_keys.txt
--rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/tutorial-secrets/requirements.txt
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.084897 batou-2.5.0b1/examples/vagrant/
--rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/vagrant/requirements.txt
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.085005 batou-2.5.0b1/examples/vagrant-multi/
--rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/vagrant-multi/requirements.txt
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.085111 batou-2.5.0b1/examples/venvs/
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.085217 batou-2.5.0b1/examples/venvs/environments/
--rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/venvs/environments/requirements.txt
--rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/venvs/requirements.txt
--rw-r--r--   0 zagy       (501) staff       (20)      129 2024-04-19 05:17:22.000000 batou-2.5.0b1/pyproject.toml
--rw-r--r--   0 zagy       (501) staff       (20)      277 2024-04-19 05:17:22.000000 batou-2.5.0b1/requirements-dev.txt
--rw-r--r--   0 zagy       (501) staff       (20)      139 2024-04-19 05:17:23.102414 batou-2.5.0b1/setup.cfg
--rw-r--r--   0 zagy       (501) staff       (20)     2248 2024-04-19 05:17:22.000000 batou-2.5.0b1/setup.py
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.075484 batou-2.5.0b1/src/
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.087773 batou-2.5.0b1/src/batou/
--rw-r--r--   0 zagy       (501) staff       (20)    25625 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/__init__.py
--rw-r--r--   0 zagy       (501) staff       (20)      997 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/_output.py
--rw-r--r--   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/agent.py
--rw-r--r--   0 zagy       (501) staff       (20)      163 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/c.py
--rw-r--r--   0 zagy       (501) staff       (20)    41055 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/component.py
--rw-r--r--   0 zagy       (501) staff       (20)      795 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/conftest.py
--rw-r--r--   0 zagy       (501) staff       (20)    14886 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/deploy.py
--rw-r--r--   0 zagy       (501) staff       (20)    21045 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/environment.py
--rw-r--r--   0 zagy       (501) staff       (20)     1507 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/fixtures.py
--rw-r--r--   0 zagy       (501) staff       (20)    12064 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/host.py
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.088633 batou-2.5.0b1/src/batou/init-template/
--rw-r--r--   0 zagy       (501) staff       (20)       44 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/init-template/.hgignore
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.075706 batou-2.5.0b1/src/batou/init-template/components/
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.088746 batou-2.5.0b1/src/batou/init-template/components/example/
--rw-r--r--   0 zagy       (501) staff       (20)      177 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/init-template/components/example/component.py
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.088853 batou-2.5.0b1/src/batou/init-template/environments/
--rw-r--r--   0 zagy       (501) staff       (20)       66 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/init-template/environments/dev.cfg
--rw-r--r--   0 zagy       (501) staff       (20)      411 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/insecure-private.key
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.091106 batou-2.5.0b1/src/batou/lib/
--rw-r--r--   0 zagy       (501) staff       (20)       29 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/__init__.py
--rw-r--r--   0 zagy       (501) staff       (20)     3983 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/appenv.py
--rw-r--r--   0 zagy       (501) staff       (20)     6457 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/archive.py
--rw-r--r--   0 zagy       (501) staff       (20)     3297 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/buildout.py
--rw-r--r--   0 zagy       (501) staff       (20)     2211 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/cmmi.py
--rw-r--r--   0 zagy       (501) staff       (20)     2524 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/cron.py
--rw-r--r--   0 zagy       (501) staff       (20)     1224 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/debian.py
--rw-r--r--   0 zagy       (501) staff       (20)     2286 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/download.py
--rw-r--r--   0 zagy       (501) staff       (20)    23943 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/file.py
--rw-r--r--   0 zagy       (501) staff       (20)     6872 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/git.py
--rw-r--r--   0 zagy       (501) staff       (20)      854 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/goceptnet.py
--rw-r--r--   0 zagy       (501) staff       (20)     1388 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/logrotate.py
--rw-r--r--   0 zagy       (501) staff       (20)     4541 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/mercurial.py
--rw-r--r--   0 zagy       (501) staff       (20)     3647 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/mysql.py
--rw-r--r--   0 zagy       (501) staff       (20)     2814 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/nagios.py
--rw-r--r--   0 zagy       (501) staff       (20)      707 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/package.py
--rw-r--r--   0 zagy       (501) staff       (20)     8150 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/python.py
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.092117 batou-2.5.0b1/src/batou/lib/resources/
--rw-r--r--   0 zagy       (501) staff       (20)     2120 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/resources/check_supervisor.py.in
--rw-r--r--   0 zagy       (501) staff       (20)      244 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/resources/crontab
--rw-r--r--   0 zagy       (501) staff       (20)      548 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/resources/init.sh
--rw-r--r--   0 zagy       (501) staff       (20)      299 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/resources/logrotate.in
--rw-r--r--   0 zagy       (501) staff       (20)      840 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/resources/nagios.cfg
--rw-r--r--   0 zagy       (501) staff       (20)      153 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/resources/nrpe.cfg
--rw-r--r--   0 zagy       (501) staff       (20)      380 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/resources/supervisor.buildout.cfg
--rw-r--r--   0 zagy       (501) staff       (20)      609 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/resources/supervisor.conf
--rw-r--r--   0 zagy       (501) staff       (20)      932 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/service.py
--rw-r--r--   0 zagy       (501) staff       (20)    10273 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/supervisor.py
--rw-r--r--   0 zagy       (501) staff       (20)     1172 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/svn.py
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.094264 batou-2.5.0b1/src/batou/lib/tests/
--rw-r--r--   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/tests/__init__.py
--rw-r--r--   0 zagy       (501) staff       (20)     3083 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/tests/test_appenv.py
--rw-r--r--   0 zagy       (501) staff       (20)     3858 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/tests/test_archive.py
--rw-r--r--   0 zagy       (501) staff       (20)     2449 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/tests/test_buildout.py
--rw-r--r--   0 zagy       (501) staff       (20)     3261 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/tests/test_cmmi.py
--rw-r--r--   0 zagy       (501) staff       (20)     2110 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/tests/test_cron.py
--rw-r--r--   0 zagy       (501) staff       (20)      639 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/tests/test_debian.py
--rw-r--r--   0 zagy       (501) staff       (20)     2158 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/tests/test_download.py
--rw-r--r--   0 zagy       (501) staff       (20)    32144 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/tests/test_file.py
--rw-r--r--   0 zagy       (501) staff       (20)    11092 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/tests/test_git.py
--rw-r--r--   0 zagy       (501) staff       (20)     6165 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/tests/test_mercurial.py
--rw-r--r--   0 zagy       (501) staff       (20)      121 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/tests/test_mysql.py
--rw-r--r--   0 zagy       (501) staff       (20)      847 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/tests/test_nagios.py
--rw-r--r--   0 zagy       (501) staff       (20)     1430 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/tests/test_python.py
--rw-r--r--   0 zagy       (501) staff       (20)     1693 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/tests/test_service.py
--rw-r--r--   0 zagy       (501) staff       (20)     3106 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/tests/test_supervisor.py
--rw-r--r--   0 zagy       (501) staff       (20)      707 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/tests/test_svn.py
--rw-r--r--   0 zagy       (501) staff       (20)     6608 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/main.py
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.094388 batou-2.5.0b1/src/batou/migrate/
--rw-r--r--   0 zagy       (501) staff       (20)     3377 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/migrate/__init__.py
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.095044 batou-2.5.0b1/src/batou/migrate/migrations/
--rw-r--r--   0 zagy       (501) staff       (20)      389 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/migrate/migrations/2300.py
--rw-r--r--   0 zagy       (501) staff       (20)     1775 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/migrate/migrations/2301.py
--rw-r--r--   0 zagy       (501) staff       (20)      874 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/migrate/migrations/2302.py
--rw-r--r--   0 zagy       (501) staff       (20)      790 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/migrate/migrations/2303.py
--rw-r--r--   0 zagy       (501) staff       (20)     1282 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/migrate/migrations/2400.py
--rw-r--r--   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/migrate/migrations/__init__.py
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.095221 batou-2.5.0b1/src/batou/migrate/tests/
--rw-r--r--   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/migrate/tests/__init__.py
--rw-r--r--   0 zagy       (501) staff       (20)     4532 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/migrate/tests/test_migrate.py
--rw-r--r--   0 zagy       (501) staff       (20)    15653 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/provision.py
--rw-r--r--   0 zagy       (501) staff       (20)    11728 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/remote_core.py
--rw-r--r--   0 zagy       (501) staff       (20)    13588 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/repository.py
--rw-r--r--   0 zagy       (501) staff       (20)     6424 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/resources.py
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.095709 batou-2.5.0b1/src/batou/secrets/
--rw-r--r--   0 zagy       (501) staff       (20)    24397 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/secrets/__init__.py
--rw-r--r--   0 zagy       (501) staff       (20)     4372 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/secrets/edit.py
--rw-r--r--   0 zagy       (501) staff       (20)    17282 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/secrets/encryption.py
--rw-r--r--   0 zagy       (501) staff       (20)     2800 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/secrets/manage.py
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.096147 batou-2.5.0b1/src/batou/secrets/tests/
--rw-r--r--   0 zagy       (501) staff       (20)       23 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/secrets/tests/__init__.py
--rw-r--r--   0 zagy       (501) staff       (20)     5126 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/secrets/tests/test_editor.py
--rw-r--r--   0 zagy       (501) staff       (20)     3994 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/secrets/tests/test_manage.py
--rw-r--r--   0 zagy       (501) staff       (20)     4379 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/secrets/tests/test_secrets.py
--rw-r--r--   0 zagy       (501) staff       (20)     2696 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/template.py
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.098355 batou-2.5.0b1/src/batou/tests/
--rw-r--r--   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/__init__.py
--rw-r--r--   0 zagy       (501) staff       (20)      666 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/conftest.py
--rw-r--r--   0 zagy       (501) staff       (20)     3012 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/ellipsis.py
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.078747 batou-2.5.0b1/src/batou/tests/fixture/
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.098462 batou-2.5.0b1/src/batou/tests/fixture/basic_service/
--rw-r--r--   0 zagy       (501) staff       (20)       33 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/basic_service/.batou.json
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.076847 batou-2.5.0b1/src/batou/tests/fixture/basic_service/components/
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.098577 batou-2.5.0b1/src/batou/tests/fixture/basic_service/components/zeo/
--rw-r--r--   0 zagy       (501) staff       (20)      178 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/basic_service/components/zeo/component.py
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.098684 batou-2.5.0b1/src/batou/tests/fixture/basic_service/components/zope/
--rw-r--r--   0 zagy       (501) staff       (20)       72 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/basic_service/components/zope/component.py
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.077065 batou-2.5.0b1/src/batou/tests/fixture/basic_service/environments/
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.098796 batou-2.5.0b1/src/batou/tests/fixture/basic_service/environments/dev/
--rw-r--r--   0 zagy       (501) staff       (20)       79 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/basic_service/environments/dev/environment.cfg
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.098907 batou-2.5.0b1/src/batou/tests/fixture/basic_service/environments/production/
--rw-r--r--   0 zagy       (501) staff       (20)      128 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/basic_service/environments/production/environment.cfg
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.099014 batou-2.5.0b1/src/batou/tests/fixture/component/
--rw-r--r--   0 zagy       (501) staff       (20)       40 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/component/haproxy.cfg
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.099126 batou-2.5.0b1/src/batou/tests/fixture/sample_service/
--rw-r--r--   0 zagy       (501) staff       (20)       33 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/sample_service/.batou.json
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.077357 batou-2.5.0b1/src/batou/tests/fixture/sample_service/components/
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.099233 batou-2.5.0b1/src/batou/tests/fixture/sample_service/components/hello/
--rw-r--r--   0 zagy       (501) staff       (20)      973 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/sample_service/components/hello/component.py
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.078227 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.099349 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-multiple-components/
--rw-r--r--   0 zagy       (501) staff       (20)      144 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-multiple-components/environment.cfg
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.099462 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-multiple-hosts/
--rw-r--r--   0 zagy       (501) staff       (20)       88 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-multiple-hosts/environment.cfg
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.099573 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-overlapping-components/
--rw-r--r--   0 zagy       (501) staff       (20)      110 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-overlapping-components/environment.cfg
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.099681 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-resolver/
--rw-r--r--   0 zagy       (501) staff       (20)       72 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-resolver/environment.cfg
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.099801 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-resolver-invalid/
--rw-r--r--   0 zagy       (501) staff       (20)       90 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-resolver-invalid/environment.cfg
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.099932 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-with-env-config/
--rw-r--r--   0 zagy       (501) staff       (20)      191 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-with-env-config/environment.cfg
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.100053 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-with-overrides/
--rw-r--r--   0 zagy       (501) staff       (20)       94 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-with-overrides/environment.cfg
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.100178 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-with-provide-require/
--rw-r--r--   0 zagy       (501) staff       (20)       85 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-with-provide-require/environment.cfg
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.100309 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-with-vfs-sandbox/
--rw-r--r--   0 zagy       (501) staff       (20)       64 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-with-vfs-sandbox/environment.cfg
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.100437 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-without-env-config/
--rw-r--r--   0 zagy       (501) staff       (20)       26 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-without-env-config/environment.cfg
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.100563 batou-2.5.0b1/src/batou/tests/fixture/service_early_resource/
--rw-r--r--   0 zagy       (501) staff       (20)       33 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/service_early_resource/.batou.json
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.078523 batou-2.5.0b1/src/batou/tests/fixture/service_early_resource/components/
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.100697 batou-2.5.0b1/src/batou/tests/fixture/service_early_resource/components/zeo/
--rw-r--r--   0 zagy       (501) staff       (20)      346 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/service_early_resource/components/zeo/component.py
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.100825 batou-2.5.0b1/src/batou/tests/fixture/service_early_resource/components/zope/
--rw-r--r--   0 zagy       (501) staff       (20)      116 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/service_early_resource/components/zope/component.py
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.078667 batou-2.5.0b1/src/batou/tests/fixture/service_early_resource/environments/
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.100952 batou-2.5.0b1/src/batou/tests/fixture/service_early_resource/environments/dev/
--rw-r--r--   0 zagy       (501) staff       (20)       62 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/service_early_resource/environments/dev/environment.cfg
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.101196 batou-2.5.0b1/src/batou/tests/fixture/template/
--rw-r--r--   0 zagy       (501) staff       (20)       84 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/template/haproxy.cfg
--rw-r--r--   0 zagy       (501) staff       (20)      119 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/template/haproxy.cfg.jinja2
--rw-r--r--   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/test_bootstrap.py
--rw-r--r--   0 zagy       (501) staff       (20)    18565 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/test_component.py
--rw-r--r--   0 zagy       (501) staff       (20)     4776 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/test_config.py
--rw-r--r--   0 zagy       (501) staff       (20)     5707 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/test_dependencies.py
--rw-r--r--   0 zagy       (501) staff       (20)     3012 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/test_deploy.py
--rw-r--r--   0 zagy       (501) staff       (20)    11409 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/test_endtoend.py
--rw-r--r--   0 zagy       (501) staff       (20)     8674 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/test_environment.py
--rw-r--r--   0 zagy       (501) staff       (20)     2311 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/test_exceptions.py
--rw-r--r--   0 zagy       (501) staff       (20)      606 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/test_host.py
--rw-r--r--   0 zagy       (501) staff       (20)     1488 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/test_main.py
--rw-r--r--   0 zagy       (501) staff       (20)     2144 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/test_remote.py
--rw-r--r--   0 zagy       (501) staff       (20)     9398 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/test_remote_core.py
--rw-r--r--   0 zagy       (501) staff       (20)     3648 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/test_repository.py
--rw-r--r--   0 zagy       (501) staff       (20)      743 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/test_resources.py
--rw-r--r--   0 zagy       (501) staff       (20)     2630 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/test_template.py
--rw-r--r--   0 zagy       (501) staff       (20)    16458 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/test_utils.py
--rw-r--r--   0 zagy       (501) staff       (20)     1169 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/test_vfs.py
--rw-r--r--   0 zagy       (501) staff       (20)    19590 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/utils.py
--rw-r--r--   0 zagy       (501) staff       (20)        8 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/version.txt
--rw-r--r--   0 zagy       (501) staff       (20)     1009 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/vfs.py
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.101489 batou-2.5.0b1/src/batou.egg-info/
--rw-r--r--   0 zagy       (501) staff       (20)     3973 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou.egg-info/PKG-INFO
--rw-r--r--   0 zagy       (501) staff       (20)     6900 2024-04-19 05:17:23.000000 batou-2.5.0b1/src/batou.egg-info/SOURCES.txt
--rw-r--r--   0 zagy       (501) staff       (20)        1 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou.egg-info/dependency_links.txt
--rw-r--r--   0 zagy       (501) staff       (20)      220 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou.egg-info/entry_points.txt
--rw-r--r--   0 zagy       (501) staff       (20)        1 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou.egg-info/not-zip-safe
--rw-r--r--   0 zagy       (501) staff       (20)      184 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou.egg-info/requires.txt
--rw-r--r--   0 zagy       (501) staff       (20)        6 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou.egg-info/top_level.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.039900 batou-2.5.0b2/
+-rw-r--r--   0 zagy       (501) staff       (20)    31241 2024-05-15 10:56:25.000000 batou-2.5.0b2/CHANGES.history.txt
+-rw-r--r--   0 zagy       (501) staff       (20)     1608 2024-05-15 10:56:25.000000 batou-2.5.0b2/LICENSE.txt
+-rw-r--r--   0 zagy       (501) staff       (20)      212 2024-05-15 10:56:25.000000 batou-2.5.0b2/MANIFEST.in
+-rw-r--r--   0 zagy       (501) staff       (20)     4016 2024-05-15 10:56:26.039822 batou-2.5.0b2/PKG-INFO
+-rw-r--r--   0 zagy       (501) staff       (20)     2691 2024-05-15 10:56:25.000000 batou-2.5.0b2/README.md
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.009139 batou-2.5.0b2/doc/
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.015678 batou-2.5.0b2/doc/source/
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.016252 batou-2.5.0b2/doc/source/api/
+-rw-r--r--   0 zagy       (501) staff       (20)      886 2024-05-15 10:56:25.000000 batou-2.5.0b2/doc/source/api/component.txt
+-rw-r--r--   0 zagy       (501) staff       (20)     2299 2024-05-15 10:56:25.000000 batou-2.5.0b2/doc/source/api/environment.txt
+-rw-r--r--   0 zagy       (501) staff       (20)       48 2024-05-15 10:56:25.000000 batou-2.5.0b2/doc/source/api/templates.txt
+-rw-r--r--   0 zagy       (501) staff       (20)       63 2024-05-15 10:56:25.000000 batou-2.5.0b2/doc/source/api/utilities.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.016391 batou-2.5.0b2/doc/source/cli/
+-rw-r--r--   0 zagy       (501) staff       (20)     4731 2024-05-15 10:56:25.000000 batou-2.5.0b2/doc/source/cli/index.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.017070 batou-2.5.0b2/doc/source/components/
+-rw-r--r--   0 zagy       (501) staff       (20)     1025 2024-05-15 10:56:25.000000 batou-2.5.0b2/doc/source/components/cmmi.txt
+-rw-r--r--   0 zagy       (501) staff       (20)     2941 2024-05-15 10:56:25.000000 batou-2.5.0b2/doc/source/components/downloads-vcs.txt
+-rw-r--r--   0 zagy       (501) staff       (20)     5657 2024-05-15 10:56:25.000000 batou-2.5.0b2/doc/source/components/files.txt
+-rw-r--r--   0 zagy       (501) staff       (20)     4820 2024-05-15 10:56:25.000000 batou-2.5.0b2/doc/source/components/python.txt
+-rw-r--r--   0 zagy       (501) staff       (20)     3050 2024-05-15 10:56:25.000000 batou-2.5.0b2/doc/source/components/services.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.017650 batou-2.5.0b2/doc/source/dev/
+-rw-r--r--   0 zagy       (501) staff       (20)      718 2024-05-15 10:56:25.000000 batou-2.5.0b2/doc/source/dev/authors.txt
+-rw-r--r--   0 zagy       (501) staff       (20)     8555 2024-05-15 10:56:25.000000 batou-2.5.0b2/doc/source/dev/contributing.txt
+-rw-r--r--   0 zagy       (501) staff       (20)     1711 2024-05-15 10:56:25.000000 batou-2.5.0b2/doc/source/dev/testing.txt
+-rw-r--r--   0 zagy       (501) staff       (20)     2809 2024-05-15 10:56:25.000000 batou-2.5.0b2/doc/source/dev/todo.txt
+-rw-r--r--   0 zagy       (501) staff       (20)     8498 2024-05-15 10:56:25.000000 batou-2.5.0b2/doc/source/index.txt
+-rw-r--r--   0 zagy       (501) staff       (20)     4799 2024-05-15 10:56:25.000000 batou-2.5.0b2/doc/source/upgrading.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.018529 batou-2.5.0b2/doc/source/user/
+-rw-r--r--   0 zagy       (501) staff       (20)    10870 2024-05-15 10:56:25.000000 batou-2.5.0b2/doc/source/user/advanced.txt
+-rw-r--r--   0 zagy       (501) staff       (20)     2565 2024-05-15 10:56:25.000000 batou-2.5.0b2/doc/source/user/install.txt
+-rw-r--r--   0 zagy       (501) staff       (20)     3848 2024-05-15 10:56:25.000000 batou-2.5.0b2/doc/source/user/installation-deb.txt
+-rw-r--r--   0 zagy       (501) staff       (20)     3798 2024-05-15 10:56:25.000000 batou-2.5.0b2/doc/source/user/installation-rpm.txt
+-rw-r--r--   0 zagy       (501) staff       (20)     2907 2024-05-15 10:56:25.000000 batou-2.5.0b2/doc/source/user/intro.txt
+-rw-r--r--   0 zagy       (501) staff       (20)    47505 2024-05-15 10:56:25.000000 batou-2.5.0b2/doc/source/user/quickstart.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.011083 batou-2.5.0b2/examples/
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.018856 batou-2.5.0b2/examples/api/
+-rw-r--r--   0 zagy       (501) staff       (20)      349 2024-05-15 10:56:25.000000 batou-2.5.0b2/examples/api/index.txt
+-rw-r--r--   0 zagy       (501) staff       (20)       60 2024-05-15 10:56:25.000000 batou-2.5.0b2/examples/api/requirements.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.018999 batou-2.5.0b2/examples/django/
+-rw-r--r--   0 zagy       (501) staff       (20)       60 2024-05-15 10:56:25.000000 batou-2.5.0b2/examples/django/requirements.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.019139 batou-2.5.0b2/examples/durations/
+-rw-r--r--   0 zagy       (501) staff       (20)       60 2024-05-15 10:56:25.000000 batou-2.5.0b2/examples/durations/requirements.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.019279 batou-2.5.0b2/examples/errors/
+-rw-r--r--   0 zagy       (501) staff       (20)       60 2024-05-15 10:56:25.000000 batou-2.5.0b2/examples/errors/requirements.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.019414 batou-2.5.0b2/examples/errors2/
+-rw-r--r--   0 zagy       (501) staff       (20)       60 2024-05-15 10:56:25.000000 batou-2.5.0b2/examples/errors2/requirements.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.019554 batou-2.5.0b2/examples/errorsnohost/
+-rw-r--r--   0 zagy       (501) staff       (20)       60 2024-05-15 10:56:25.000000 batou-2.5.0b2/examples/errorsnohost/requirements.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.019684 batou-2.5.0b2/examples/ignores/
+-rw-r--r--   0 zagy       (501) staff       (20)       60 2024-05-15 10:56:25.000000 batou-2.5.0b2/examples/ignores/requirements.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.019822 batou-2.5.0b2/examples/largetempl/
+-rw-r--r--   0 zagy       (501) staff       (20)       60 2024-05-15 10:56:25.000000 batou-2.5.0b2/examples/largetempl/requirements.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.019954 batou-2.5.0b2/examples/package/
+-rw-r--r--   0 zagy       (501) staff       (20)       60 2024-05-15 10:56:25.000000 batou-2.5.0b2/examples/package/requirements.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.020072 batou-2.5.0b2/examples/sync_async/
+-rw-r--r--   0 zagy       (501) staff       (20)       60 2024-05-15 10:56:25.000000 batou-2.5.0b2/examples/sync_async/requirements.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.020186 batou-2.5.0b2/examples/tutorial-buildout/
+-rw-r--r--   0 zagy       (501) staff       (20)       60 2024-05-15 10:56:25.000000 batou-2.5.0b2/examples/tutorial-buildout/requirements.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.020301 batou-2.5.0b2/examples/tutorial-component/
+-rw-r--r--   0 zagy       (501) staff       (20)       60 2024-05-15 10:56:25.000000 batou-2.5.0b2/examples/tutorial-component/requirements.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.020429 batou-2.5.0b2/examples/tutorial-helloworld/
+-rw-r--r--   0 zagy       (501) staff       (20)       60 2024-05-15 10:56:25.000000 batou-2.5.0b2/examples/tutorial-helloworld/requirements.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.020542 batou-2.5.0b2/examples/tutorial-parallelize/
+-rw-r--r--   0 zagy       (501) staff       (20)       60 2024-05-15 10:56:25.000000 batou-2.5.0b2/examples/tutorial-parallelize/requirements.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.020656 batou-2.5.0b2/examples/tutorial-provision-container/
+-rw-r--r--   0 zagy       (501) staff       (20)       60 2024-05-15 10:56:25.000000 batou-2.5.0b2/examples/tutorial-provision-container/requirements.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.020780 batou-2.5.0b2/examples/tutorial-secrets/
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.010870 batou-2.5.0b2/examples/tutorial-secrets/environments/
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.020924 batou-2.5.0b2/examples/tutorial-secrets/environments/age/
+-rw-r--r--   0 zagy       (501) staff       (20)     2269 2024-05-15 10:56:25.000000 batou-2.5.0b2/examples/tutorial-secrets/environments/age/age_keys.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.021103 batou-2.5.0b2/examples/tutorial-secrets/environments/age-diffable/
+-rw-r--r--   0 zagy       (501) staff       (20)     2269 2024-05-15 10:56:25.000000 batou-2.5.0b2/examples/tutorial-secrets/environments/age-diffable/age_keys.txt
+-rw-r--r--   0 zagy       (501) staff       (20)       60 2024-05-15 10:56:25.000000 batou-2.5.0b2/examples/tutorial-secrets/requirements.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.021250 batou-2.5.0b2/examples/vagrant/
+-rw-r--r--   0 zagy       (501) staff       (20)       60 2024-05-15 10:56:25.000000 batou-2.5.0b2/examples/vagrant/requirements.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.021388 batou-2.5.0b2/examples/vagrant-multi/
+-rw-r--r--   0 zagy       (501) staff       (20)       60 2024-05-15 10:56:25.000000 batou-2.5.0b2/examples/vagrant-multi/requirements.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.021522 batou-2.5.0b2/examples/venvs/
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.021651 batou-2.5.0b2/examples/venvs/environments/
+-rw-r--r--   0 zagy       (501) staff       (20)       60 2024-05-15 10:56:25.000000 batou-2.5.0b2/examples/venvs/environments/requirements.txt
+-rw-r--r--   0 zagy       (501) staff       (20)       60 2024-05-15 10:56:25.000000 batou-2.5.0b2/examples/venvs/requirements.txt
+-rw-r--r--   0 zagy       (501) staff       (20)      139 2024-05-15 10:56:25.000000 batou-2.5.0b2/pyproject.toml
+-rw-r--r--   0 zagy       (501) staff       (20)      277 2024-05-15 10:56:25.000000 batou-2.5.0b2/requirements-dev.txt
+-rw-r--r--   0 zagy       (501) staff       (20)      139 2024-05-15 10:56:26.040154 batou-2.5.0b2/setup.cfg
+-rw-r--r--   0 zagy       (501) staff       (20)     2106 2024-05-15 10:56:25.000000 batou-2.5.0b2/setup.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.011336 batou-2.5.0b2/src/
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.024425 batou-2.5.0b2/src/batou/
+-rw-r--r--   0 zagy       (501) staff       (20)    25625 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/__init__.py
+-rw-r--r--   0 zagy       (501) staff       (20)      997 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/_output.py
+-rw-r--r--   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/agent.py
+-rw-r--r--   0 zagy       (501) staff       (20)      163 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/c.py
+-rw-r--r--   0 zagy       (501) staff       (20)    41055 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/component.py
+-rw-r--r--   0 zagy       (501) staff       (20)      795 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/conftest.py
+-rw-r--r--   0 zagy       (501) staff       (20)    14886 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/deploy.py
+-rw-r--r--   0 zagy       (501) staff       (20)    21045 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/environment.py
+-rw-r--r--   0 zagy       (501) staff       (20)     1507 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/fixtures.py
+-rw-r--r--   0 zagy       (501) staff       (20)    12064 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/host.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.025484 batou-2.5.0b2/src/batou/init-template/
+-rw-r--r--   0 zagy       (501) staff       (20)       44 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/init-template/.hgignore
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.011531 batou-2.5.0b2/src/batou/init-template/components/
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.025613 batou-2.5.0b2/src/batou/init-template/components/example/
+-rw-r--r--   0 zagy       (501) staff       (20)      177 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/init-template/components/example/component.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.025736 batou-2.5.0b2/src/batou/init-template/environments/
+-rw-r--r--   0 zagy       (501) staff       (20)       66 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/init-template/environments/dev.cfg
+-rw-r--r--   0 zagy       (501) staff       (20)      411 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/insecure-private.key
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.028111 batou-2.5.0b2/src/batou/lib/
+-rw-r--r--   0 zagy       (501) staff       (20)       29 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/__init__.py
+-rw-r--r--   0 zagy       (501) staff       (20)     3983 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/appenv.py
+-rw-r--r--   0 zagy       (501) staff       (20)     6457 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/archive.py
+-rw-r--r--   0 zagy       (501) staff       (20)     3297 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/buildout.py
+-rw-r--r--   0 zagy       (501) staff       (20)     2211 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/cmmi.py
+-rw-r--r--   0 zagy       (501) staff       (20)     2524 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/cron.py
+-rw-r--r--   0 zagy       (501) staff       (20)     1224 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/debian.py
+-rw-r--r--   0 zagy       (501) staff       (20)     2286 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/download.py
+-rw-r--r--   0 zagy       (501) staff       (20)    23943 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/file.py
+-rw-r--r--   0 zagy       (501) staff       (20)     6872 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/git.py
+-rw-r--r--   0 zagy       (501) staff       (20)      854 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/goceptnet.py
+-rw-r--r--   0 zagy       (501) staff       (20)     1432 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/logrotate.py
+-rw-r--r--   0 zagy       (501) staff       (20)     4541 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/mercurial.py
+-rw-r--r--   0 zagy       (501) staff       (20)     3647 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/mysql.py
+-rw-r--r--   0 zagy       (501) staff       (20)     2814 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/nagios.py
+-rw-r--r--   0 zagy       (501) staff       (20)      707 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/package.py
+-rw-r--r--   0 zagy       (501) staff       (20)     8150 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/python.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.029018 batou-2.5.0b2/src/batou/lib/resources/
+-rw-r--r--   0 zagy       (501) staff       (20)     2120 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/resources/check_supervisor.py.in
+-rw-r--r--   0 zagy       (501) staff       (20)      244 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/resources/crontab
+-rw-r--r--   0 zagy       (501) staff       (20)      548 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/resources/init.sh
+-rw-r--r--   0 zagy       (501) staff       (20)      299 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/resources/logrotate.in
+-rw-r--r--   0 zagy       (501) staff       (20)      840 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/resources/nagios.cfg
+-rw-r--r--   0 zagy       (501) staff       (20)      153 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/resources/nrpe.cfg
+-rw-r--r--   0 zagy       (501) staff       (20)      380 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/resources/supervisor.buildout.cfg
+-rw-r--r--   0 zagy       (501) staff       (20)      609 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/resources/supervisor.conf
+-rw-r--r--   0 zagy       (501) staff       (20)      932 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/service.py
+-rw-r--r--   0 zagy       (501) staff       (20)    10273 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/supervisor.py
+-rw-r--r--   0 zagy       (501) staff       (20)     1172 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/svn.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.031333 batou-2.5.0b2/src/batou/lib/tests/
+-rw-r--r--   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/tests/__init__.py
+-rw-r--r--   0 zagy       (501) staff       (20)     3083 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/tests/test_appenv.py
+-rw-r--r--   0 zagy       (501) staff       (20)     4432 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/tests/test_archive.py
+-rw-r--r--   0 zagy       (501) staff       (20)     2366 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/tests/test_buildout.py
+-rw-r--r--   0 zagy       (501) staff       (20)     3261 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/tests/test_cmmi.py
+-rw-r--r--   0 zagy       (501) staff       (20)     2110 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/tests/test_cron.py
+-rw-r--r--   0 zagy       (501) staff       (20)      639 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/tests/test_debian.py
+-rw-r--r--   0 zagy       (501) staff       (20)     2158 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/tests/test_download.py
+-rw-r--r--   0 zagy       (501) staff       (20)    32144 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/tests/test_file.py
+-rw-r--r--   0 zagy       (501) staff       (20)    11092 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/tests/test_git.py
+-rw-r--r--   0 zagy       (501) staff       (20)     6165 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/tests/test_mercurial.py
+-rw-r--r--   0 zagy       (501) staff       (20)      121 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/tests/test_mysql.py
+-rw-r--r--   0 zagy       (501) staff       (20)      847 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/tests/test_nagios.py
+-rw-r--r--   0 zagy       (501) staff       (20)     1430 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/tests/test_python.py
+-rw-r--r--   0 zagy       (501) staff       (20)     1693 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/tests/test_service.py
+-rw-r--r--   0 zagy       (501) staff       (20)     3106 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/tests/test_supervisor.py
+-rw-r--r--   0 zagy       (501) staff       (20)      707 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/lib/tests/test_svn.py
+-rw-r--r--   0 zagy       (501) staff       (20)     6635 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/main.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.031493 batou-2.5.0b2/src/batou/migrate/
+-rw-r--r--   0 zagy       (501) staff       (20)     3473 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/migrate/__init__.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.032420 batou-2.5.0b2/src/batou/migrate/migrations/
+-rw-r--r--   0 zagy       (501) staff       (20)      389 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/migrate/migrations/2300.py
+-rw-r--r--   0 zagy       (501) staff       (20)     1775 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/migrate/migrations/2301.py
+-rw-r--r--   0 zagy       (501) staff       (20)      874 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/migrate/migrations/2302.py
+-rw-r--r--   0 zagy       (501) staff       (20)      790 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/migrate/migrations/2303.py
+-rw-r--r--   0 zagy       (501) staff       (20)     1282 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/migrate/migrations/2400.py
+-rw-r--r--   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/migrate/migrations/__init__.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.032609 batou-2.5.0b2/src/batou/migrate/tests/
+-rw-r--r--   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/migrate/tests/__init__.py
+-rw-r--r--   0 zagy       (501) staff       (20)     4532 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/migrate/tests/test_migrate.py
+-rw-r--r--   0 zagy       (501) staff       (20)    15653 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/provision.py
+-rw-r--r--   0 zagy       (501) staff       (20)    11728 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/remote_core.py
+-rw-r--r--   0 zagy       (501) staff       (20)    13588 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/repository.py
+-rw-r--r--   0 zagy       (501) staff       (20)     6424 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/resources.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.033129 batou-2.5.0b2/src/batou/secrets/
+-rw-r--r--   0 zagy       (501) staff       (20)    24397 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/secrets/__init__.py
+-rw-r--r--   0 zagy       (501) staff       (20)     4372 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/secrets/edit.py
+-rw-r--r--   0 zagy       (501) staff       (20)    17610 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/secrets/encryption.py
+-rw-r--r--   0 zagy       (501) staff       (20)     2800 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/secrets/manage.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.033595 batou-2.5.0b2/src/batou/secrets/tests/
+-rw-r--r--   0 zagy       (501) staff       (20)       23 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/secrets/tests/__init__.py
+-rw-r--r--   0 zagy       (501) staff       (20)     5126 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/secrets/tests/test_editor.py
+-rw-r--r--   0 zagy       (501) staff       (20)     3994 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/secrets/tests/test_manage.py
+-rw-r--r--   0 zagy       (501) staff       (20)     5606 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/secrets/tests/test_secrets.py
+-rw-r--r--   0 zagy       (501) staff       (20)     2696 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/template.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.036042 batou-2.5.0b2/src/batou/tests/
+-rw-r--r--   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/__init__.py
+-rw-r--r--   0 zagy       (501) staff       (20)      666 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/conftest.py
+-rw-r--r--   0 zagy       (501) staff       (20)     3012 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/ellipsis.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.014230 batou-2.5.0b2/src/batou/tests/fixture/
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.036152 batou-2.5.0b2/src/batou/tests/fixture/basic_service/
+-rw-r--r--   0 zagy       (501) staff       (20)       33 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/fixture/basic_service/.batou.json
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.012540 batou-2.5.0b2/src/batou/tests/fixture/basic_service/components/
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.036269 batou-2.5.0b2/src/batou/tests/fixture/basic_service/components/zeo/
+-rw-r--r--   0 zagy       (501) staff       (20)      178 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/fixture/basic_service/components/zeo/component.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.036386 batou-2.5.0b2/src/batou/tests/fixture/basic_service/components/zope/
+-rw-r--r--   0 zagy       (501) staff       (20)       72 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/fixture/basic_service/components/zope/component.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.012734 batou-2.5.0b2/src/batou/tests/fixture/basic_service/environments/
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.036498 batou-2.5.0b2/src/batou/tests/fixture/basic_service/environments/dev/
+-rw-r--r--   0 zagy       (501) staff       (20)       79 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/fixture/basic_service/environments/dev/environment.cfg
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.036613 batou-2.5.0b2/src/batou/tests/fixture/basic_service/environments/production/
+-rw-r--r--   0 zagy       (501) staff       (20)      128 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/fixture/basic_service/environments/production/environment.cfg
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.036729 batou-2.5.0b2/src/batou/tests/fixture/component/
+-rw-r--r--   0 zagy       (501) staff       (20)       40 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/fixture/component/haproxy.cfg
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.036846 batou-2.5.0b2/src/batou/tests/fixture/sample_service/
+-rw-r--r--   0 zagy       (501) staff       (20)       33 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/fixture/sample_service/.batou.json
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.012997 batou-2.5.0b2/src/batou/tests/fixture/sample_service/components/
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.036957 batou-2.5.0b2/src/batou/tests/fixture/sample_service/components/hello/
+-rw-r--r--   0 zagy       (501) staff       (20)      973 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/fixture/sample_service/components/hello/component.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.013761 batou-2.5.0b2/src/batou/tests/fixture/sample_service/environments/
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.037084 batou-2.5.0b2/src/batou/tests/fixture/sample_service/environments/test-multiple-components/
+-rw-r--r--   0 zagy       (501) staff       (20)      144 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/fixture/sample_service/environments/test-multiple-components/environment.cfg
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.037200 batou-2.5.0b2/src/batou/tests/fixture/sample_service/environments/test-multiple-hosts/
+-rw-r--r--   0 zagy       (501) staff       (20)       88 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/fixture/sample_service/environments/test-multiple-hosts/environment.cfg
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.037316 batou-2.5.0b2/src/batou/tests/fixture/sample_service/environments/test-overlapping-components/
+-rw-r--r--   0 zagy       (501) staff       (20)      110 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/fixture/sample_service/environments/test-overlapping-components/environment.cfg
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.037433 batou-2.5.0b2/src/batou/tests/fixture/sample_service/environments/test-resolver/
+-rw-r--r--   0 zagy       (501) staff       (20)       72 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/fixture/sample_service/environments/test-resolver/environment.cfg
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.037552 batou-2.5.0b2/src/batou/tests/fixture/sample_service/environments/test-resolver-invalid/
+-rw-r--r--   0 zagy       (501) staff       (20)       90 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/fixture/sample_service/environments/test-resolver-invalid/environment.cfg
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.037674 batou-2.5.0b2/src/batou/tests/fixture/sample_service/environments/test-with-env-config/
+-rw-r--r--   0 zagy       (501) staff       (20)      191 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/fixture/sample_service/environments/test-with-env-config/environment.cfg
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.037796 batou-2.5.0b2/src/batou/tests/fixture/sample_service/environments/test-with-overrides/
+-rw-r--r--   0 zagy       (501) staff       (20)       94 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/fixture/sample_service/environments/test-with-overrides/environment.cfg
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.037912 batou-2.5.0b2/src/batou/tests/fixture/sample_service/environments/test-with-provide-require/
+-rw-r--r--   0 zagy       (501) staff       (20)       85 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/fixture/sample_service/environments/test-with-provide-require/environment.cfg
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.038028 batou-2.5.0b2/src/batou/tests/fixture/sample_service/environments/test-with-vfs-sandbox/
+-rw-r--r--   0 zagy       (501) staff       (20)       64 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/fixture/sample_service/environments/test-with-vfs-sandbox/environment.cfg
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.038142 batou-2.5.0b2/src/batou/tests/fixture/sample_service/environments/test-without-env-config/
+-rw-r--r--   0 zagy       (501) staff       (20)       26 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/fixture/sample_service/environments/test-without-env-config/environment.cfg
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.038261 batou-2.5.0b2/src/batou/tests/fixture/service_early_resource/
+-rw-r--r--   0 zagy       (501) staff       (20)       33 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/fixture/service_early_resource/.batou.json
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.014035 batou-2.5.0b2/src/batou/tests/fixture/service_early_resource/components/
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.038376 batou-2.5.0b2/src/batou/tests/fixture/service_early_resource/components/zeo/
+-rw-r--r--   0 zagy       (501) staff       (20)      346 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/fixture/service_early_resource/components/zeo/component.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.038488 batou-2.5.0b2/src/batou/tests/fixture/service_early_resource/components/zope/
+-rw-r--r--   0 zagy       (501) staff       (20)      116 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/fixture/service_early_resource/components/zope/component.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.014158 batou-2.5.0b2/src/batou/tests/fixture/service_early_resource/environments/
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.038623 batou-2.5.0b2/src/batou/tests/fixture/service_early_resource/environments/dev/
+-rw-r--r--   0 zagy       (501) staff       (20)       62 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/fixture/service_early_resource/environments/dev/environment.cfg
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.038852 batou-2.5.0b2/src/batou/tests/fixture/template/
+-rw-r--r--   0 zagy       (501) staff       (20)       84 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/fixture/template/haproxy.cfg
+-rw-r--r--   0 zagy       (501) staff       (20)      119 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/fixture/template/haproxy.cfg.jinja2
+-rw-r--r--   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/test_bootstrap.py
+-rw-r--r--   0 zagy       (501) staff       (20)    18565 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/test_component.py
+-rw-r--r--   0 zagy       (501) staff       (20)     4776 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/test_config.py
+-rw-r--r--   0 zagy       (501) staff       (20)     5707 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/test_dependencies.py
+-rw-r--r--   0 zagy       (501) staff       (20)     3085 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/test_deploy.py
+-rw-r--r--   0 zagy       (501) staff       (20)    11415 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/test_endtoend.py
+-rw-r--r--   0 zagy       (501) staff       (20)     8674 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/test_environment.py
+-rw-r--r--   0 zagy       (501) staff       (20)     2311 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/test_exceptions.py
+-rw-r--r--   0 zagy       (501) staff       (20)      606 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/test_host.py
+-rw-r--r--   0 zagy       (501) staff       (20)     1488 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/test_main.py
+-rw-r--r--   0 zagy       (501) staff       (20)     2144 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/test_remote.py
+-rw-r--r--   0 zagy       (501) staff       (20)     9398 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/test_remote_core.py
+-rw-r--r--   0 zagy       (501) staff       (20)     3648 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/test_repository.py
+-rw-r--r--   0 zagy       (501) staff       (20)      743 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/test_resources.py
+-rw-r--r--   0 zagy       (501) staff       (20)     2630 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/test_template.py
+-rw-r--r--   0 zagy       (501) staff       (20)    16458 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/test_utils.py
+-rw-r--r--   0 zagy       (501) staff       (20)     1169 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/tests/test_vfs.py
+-rw-r--r--   0 zagy       (501) staff       (20)    19589 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/utils.py
+-rw-r--r--   0 zagy       (501) staff       (20)        8 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/version.txt
+-rw-r--r--   0 zagy       (501) staff       (20)     1009 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou/vfs.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-15 10:56:26.039019 batou-2.5.0b2/src/batou.egg-info/
+-rw-r--r--   0 zagy       (501) staff       (20)     4016 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou.egg-info/PKG-INFO
+-rw-r--r--   0 zagy       (501) staff       (20)     6900 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou.egg-info/SOURCES.txt
+-rw-r--r--   0 zagy       (501) staff       (20)        1 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou.egg-info/dependency_links.txt
+-rw-r--r--   0 zagy       (501) staff       (20)      220 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou.egg-info/entry_points.txt
+-rw-r--r--   0 zagy       (501) staff       (20)        1 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou.egg-info/not-zip-safe
+-rw-r--r--   0 zagy       (501) staff       (20)      212 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou.egg-info/requires.txt
+-rw-r--r--   0 zagy       (501) staff       (20)        6 2024-05-15 10:56:25.000000 batou-2.5.0b2/src/batou.egg-info/top_level.txt
```

### Comparing `batou-2.5.0b1/CHANGES.history.txt` & `batou-2.5.0b2/CHANGES.history.txt`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/LICENSE.txt` & `batou-2.5.0b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/PKG-INFO` & `batou-2.5.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batou
-Version: 2.5.0b1
+Version: 2.5.0b2
 Summary: A utility for automating multi-host, multi-environment software builds and deployments.
 Home-page: https://batou.readthedocs.io/en/latest/
 Author: Christian Theune
 Author-email: ct@flyingcircus.io
 License: BSD (2-clause)
 Keywords: deployment
 Classifier: License :: OSI Approved :: BSD License
@@ -15,20 +15,21 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: ConfigUpdater>=3.0.1
-Requires-Dist: Jinja2==3.0.1
+Requires-Dist: Jinja2>=3.1.4
 Requires-Dist: requests
 Requires-Dist: setuptools>=38.3
 Requires-Dist: execnet>=1.8.1
 Requires-Dist: importlib_metadata
-Requires-Dist: py
+Requires-Dist: importlib_resources
+Requires-Dist: py>=1.11.0
 Requires-Dist: pyyaml
 Requires-Dist: remote-pdb
 Provides-Extra: test
 Requires-Dist: mock; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-coverage; extra == "test"
 Requires-Dist: pytest-instafail; extra == "test"
```

### Comparing `batou-2.5.0b1/README.md` & `batou-2.5.0b2/README.md`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/doc/source/api/component.txt` & `batou-2.5.0b2/doc/source/api/component.txt`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/doc/source/api/environment.txt` & `batou-2.5.0b2/doc/source/api/environment.txt`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/doc/source/cli/index.txt` & `batou-2.5.0b2/doc/source/cli/index.txt`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/doc/source/components/cmmi.txt` & `batou-2.5.0b2/doc/source/components/cmmi.txt`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/doc/source/components/downloads-vcs.txt` & `batou-2.5.0b2/doc/source/components/downloads-vcs.txt`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/doc/source/components/files.txt` & `batou-2.5.0b2/doc/source/components/files.txt`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/doc/source/components/python.txt` & `batou-2.5.0b2/doc/source/components/python.txt`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/doc/source/components/services.txt` & `batou-2.5.0b2/doc/source/components/services.txt`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/doc/source/dev/authors.txt` & `batou-2.5.0b2/doc/source/dev/authors.txt`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/doc/source/dev/contributing.txt` & `batou-2.5.0b2/doc/source/dev/contributing.txt`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/doc/source/dev/testing.txt` & `batou-2.5.0b2/doc/source/dev/testing.txt`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/doc/source/dev/todo.txt` & `batou-2.5.0b2/doc/source/dev/todo.txt`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/doc/source/index.txt` & `batou-2.5.0b2/doc/source/index.txt`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/doc/source/upgrading.txt` & `batou-2.5.0b2/doc/source/upgrading.txt`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/doc/source/user/advanced.txt` & `batou-2.5.0b2/doc/source/user/advanced.txt`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/doc/source/user/install.txt` & `batou-2.5.0b2/doc/source/user/install.txt`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/doc/source/user/installation-deb.txt` & `batou-2.5.0b2/doc/source/user/installation-deb.txt`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/doc/source/user/installation-rpm.txt` & `batou-2.5.0b2/doc/source/user/installation-rpm.txt`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/doc/source/user/intro.txt` & `batou-2.5.0b2/doc/source/user/intro.txt`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/doc/source/user/quickstart.txt` & `batou-2.5.0b2/doc/source/user/quickstart.txt`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/examples/tutorial-secrets/environments/age/age_keys.txt` & `batou-2.5.0b2/examples/tutorial-secrets/environments/age/age_keys.txt`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/examples/tutorial-secrets/environments/age-diffable/age_keys.txt` & `batou-2.5.0b2/examples/tutorial-secrets/environments/age-diffable/age_keys.txt`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/setup.py` & `batou-2.5.0b2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,23 +9,22 @@
 version = open("src/batou/version.txt").read().strip()
 
 setup(
     name="batou",
     version=version,
     install_requires=[
         "ConfigUpdater>=3.0.1",
-        # As long as we support 3.6 we're stuck here, to avoid
-        # https://stackoverflow.com/questions/67659135/flask-token-object-has-no-attribute-test-render-template-error
-        "Jinja2==3.0.1",
+        "Jinja2>=3.1.4",
         "requests",
         # ConfigUpdater does not manage its minimum requirements correctly.
         "setuptools>=38.3",
         "execnet>=1.8.1",
         "importlib_metadata",
-        "py",
+        "importlib_resources",
+        "py>=1.11.0",
         "pyyaml",
         "remote-pdb",
     ],
     extras_require={
         "test": [
             "mock",
             "pytest",
```

### Comparing `batou-2.5.0b1/src/batou/__init__.py` & `batou-2.5.0b2/src/batou/__init__.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/_output.py` & `batou-2.5.0b2/src/batou/_output.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/component.py` & `batou-2.5.0b2/src/batou/component.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/conftest.py` & `batou-2.5.0b2/src/batou/conftest.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/deploy.py` & `batou-2.5.0b2/src/batou/deploy.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/environment.py` & `batou-2.5.0b2/src/batou/environment.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/fixtures.py` & `batou-2.5.0b2/src/batou/fixtures.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/host.py` & `batou-2.5.0b2/src/batou/host.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/lib/appenv.py` & `batou-2.5.0b2/src/batou/lib/appenv.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/lib/archive.py` & `batou-2.5.0b2/src/batou/lib/archive.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/lib/buildout.py` & `batou-2.5.0b2/src/batou/lib/buildout.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/lib/cmmi.py` & `batou-2.5.0b2/src/batou/lib/cmmi.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/lib/cron.py` & `batou-2.5.0b2/src/batou/lib/cron.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/lib/debian.py` & `batou-2.5.0b2/src/batou/lib/debian.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/lib/download.py` & `batou-2.5.0b2/src/batou/lib/download.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/lib/file.py` & `batou-2.5.0b2/src/batou/lib/file.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/lib/git.py` & `batou-2.5.0b2/src/batou/lib/git.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/lib/goceptnet.py` & `batou-2.5.0b2/src/batou/lib/goceptnet.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/lib/logrotate.py` & `batou-2.5.0b2/src/batou/lib/logrotate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os.path
 
-import pkg_resources
+import importlib_resources
 
 from batou.component import Component, HookComponent, platform
 from batou.lib.file import File
 
 
 class RotatedLogfile(HookComponent):
 
@@ -21,16 +21,18 @@
         self.path = self.map(self.path)
         self.args = list(map(str.strip, self.args.split(",")))
 
 
 class Logrotate(Component):
 
     common_config = b""
-    logrotate_template = pkg_resources.resource_string(
-        __name__, "resources/logrotate.in"
+    logrotate_template = (
+        importlib_resources.files(__name__)
+        .joinpath("resources/logrotate.in")
+        .read_bytes()
     )
 
     def configure(self):
         self.logfiles = self.require(RotatedLogfile.key, host=self.host)
         self.logfiles.sort(key=lambda logfile: logfile.path)
 
         config = self.common_config + self.logrotate_template
```

### Comparing `batou-2.5.0b1/src/batou/lib/mercurial.py` & `batou-2.5.0b2/src/batou/lib/mercurial.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/lib/mysql.py` & `batou-2.5.0b2/src/batou/lib/mysql.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/lib/nagios.py` & `batou-2.5.0b2/src/batou/lib/nagios.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/lib/package.py` & `batou-2.5.0b2/src/batou/lib/package.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/lib/python.py` & `batou-2.5.0b2/src/batou/lib/python.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/lib/resources/check_supervisor.py.in` & `batou-2.5.0b2/src/batou/lib/resources/check_supervisor.py.in`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/lib/resources/init.sh` & `batou-2.5.0b2/src/batou/lib/resources/init.sh`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/lib/resources/nagios.cfg` & `batou-2.5.0b2/src/batou/lib/resources/nagios.cfg`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/lib/resources/supervisor.conf` & `batou-2.5.0b2/src/batou/lib/resources/supervisor.conf`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/lib/service.py` & `batou-2.5.0b2/src/batou/lib/service.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/lib/supervisor.py` & `batou-2.5.0b2/src/batou/lib/supervisor.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/lib/svn.py` & `batou-2.5.0b2/src/batou/lib/svn.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/lib/tests/test_appenv.py` & `batou-2.5.0b2/src/batou/lib/tests/test_appenv.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/lib/tests/test_archive.py` & `batou-2.5.0b2/src/batou/lib/tests/test_archive.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 import os
+import pathlib
 import sys
 import time
 
 import pytest
-from pkg_resources import resource_filename
 
 from batou.lib.archive import Extract
 
 
 def test_unknown_extension_raises():
     extract = Extract("example.unknown")
     extract.workdir = ""
@@ -23,26 +23,29 @@
     extractor = extract.sub_components[0]
     with pytest.raises(AssertionError):
         extractor.verify()
 
 
 def test_untar_extracts_archive_to_target_directory(root):
     extract = Extract(
-        resource_filename(__name__, "example.tar.gz"), target="example"
+        # resource_filename(__name__, "example.tar.gz"), target="example"
+        pathlib.Path(__file__).parent / "example.tar.gz",
+        target="example",
     )
     root.component += extract
     root.component.deploy()
     assert os.listdir(str(extract.target)) == ["foo"]
 
 
 def test_ignores_ctime_for_directories(root):
     # This is hard to test: ctime can not be changed directly,
     # we thus have to perform a somewhat elaborate dance to align
     # the starts as we wish.
-    archive = resource_filename(__name__, "example.tar.gz")
+    # archive = resource_filename(__name__, "example.tar.gz")
+    archive = pathlib.Path(__file__).parent / "example.tar.gz"
     extract = Extract(archive, target="example")
 
     root.component += extract
     root.component.deploy()
     # No assertion raised, nothing to extract
     extract.extractor.verify()
 
@@ -56,33 +59,40 @@
 
     # No assertion raised, still nothing to extract
     extract.extractor.verify()
 
 
 def test_untar_can_strip_paths_off_archived_files(root):
     extract = Extract(
-        resource_filename(__name__, "example.tar.gz"), target="example", strip=1
+        # resource_filename(__name__, "example.tar.gz"), target="example", strip=1
+        pathlib.Path(__file__).parent / "example.tar.gz",
+        target="example",
+        strip=1,
     )
     root.component += extract
     root.component.deploy()
     assert os.listdir(str(extract.target)) == ["bar"]
 
 
 def test_zip_extracts_archive_to_target_directory(root):
     extract = Extract(
-        resource_filename(__name__, "example.zip"), target="example"
+        # resource_filename(__name__, "example.zip"), target="example"
+        pathlib.Path(__file__).parent / "example.zip",
+        target="example",
     )
     root.component += extract
     root.component.deploy()
     assert os.listdir(str(extract.target)) == ["foo"]
 
 
 def test_zip_overwrites_existing_files(root):
     extract = Extract(
-        resource_filename(__name__, "example.zip"), target="example"
+        # resource_filename(__name__, "example.zip"), target="example"
+        pathlib.Path(__file__).parent / "example.zip",
+        target="example",
     )
     root.component += extract
 
     target = "%s/mycomponent/example/foo/bar" % root.environment.workdir_base
     os.makedirs(target)
     filename = target + "/qux"
     with open(filename, "w") as f:
@@ -94,15 +104,17 @@
         assert "" == f.read()
 
 
 @pytest.mark.slow
 @pytest.mark.skipif(sys.platform != "darwin", reason="only runs on OS X")
 def test_dmg_extracts_archive_to_target_directory(root):
     extract = Extract(
-        resource_filename(__name__, "example.dmg"), target="example"
+        # resource_filename(__name__, "example.dmg"), target="example"
+        pathlib.Path(__file__).parent / "example.dmg",
+        target="example",
     )
     root.component += extract
     root.component.deploy()
 
     assert sorted(os.listdir(str(extract.target))) == [
         " ",
         "a\u0308sdf.txt",
@@ -114,12 +126,15 @@
     start_bin = extract.target + "/example.app/MacOS/start.bin"
     with open(start_bin) as start_bin:
         assert start_bin.read() == "I start the example app! ;)"
 
 
 def test_dmg_does_not_support_strip(root):
     extract = Extract(
-        resource_filename(__name__, "example.dmg"), strip=1, target="example"
+        # resource_filename(__name__, "example.dmg"), strip=1, target="example"
+        pathlib.Path(__file__).parent / "example.dmg",
+        strip=1,
+        target="example",
     )
     with pytest.raises(ValueError) as e:
         root.component += extract
         assert e.value.args[0] == "Strip is not supported by DMGExtractor"
```

### Comparing `batou-2.5.0b1/src/batou/lib/tests/test_buildout.py` & `batou-2.5.0b2/src/batou/lib/tests/test_buildout.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os.path
+import pathlib
 import sys
 
 import mock
-import pkg_resources
 import pytest
 
 from batou.utils import CmdExecutionError
 
 from ..buildout import Buildout
 from ..file import File
 
@@ -47,17 +47,15 @@
 def test_runs_buildout_successfully(root):
     b = Buildout(
         python="2.7",
         version="2.13.4",
         setuptools="44.1.1",
         config=File(
             "buildout.cfg",
-            source=pkg_resources.resource_filename(
-                __name__, "buildout-example.cfg"
-            ),
+            source=pathlib.Path(__file__).parent / "buildout-example.cfg",
         ),
     )
     root.component += b
     root.component.deploy()
     assert os.path.isdir(
         os.path.join(root.environment.workdir_base, "mycomponent/parts")
     )
@@ -73,17 +71,15 @@
         python="3",
         version="3.0.0b1",
         setuptools="54.1.1",
         wheel="0.36.2",
         pip="21.0.1",
         config=File(
             "buildout3.cfg",
-            source=pkg_resources.resource_filename(
-                __name__, "buildout3-example.cfg"
-            ),
+            source=str(pathlib.Path(__file__).parent / "buildout3-example.cfg"),
         ),
     )
     root.component += b
     try:
         root.component.deploy()
     except CmdExecutionError as e:
         e.report()
```

### Comparing `batou-2.5.0b1/src/batou/lib/tests/test_cmmi.py` & `batou-2.5.0b2/src/batou/lib/tests/test_cmmi.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/lib/tests/test_cron.py` & `batou-2.5.0b2/src/batou/lib/tests/test_cron.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/lib/tests/test_debian.py` & `batou-2.5.0b2/src/batou/lib/tests/test_debian.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/lib/tests/test_download.py` & `batou-2.5.0b2/src/batou/lib/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/lib/tests/test_file.py` & `batou-2.5.0b2/src/batou/lib/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/lib/tests/test_git.py` & `batou-2.5.0b2/src/batou/lib/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/lib/tests/test_mercurial.py` & `batou-2.5.0b2/src/batou/lib/tests/test_mercurial.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/lib/tests/test_nagios.py` & `batou-2.5.0b2/src/batou/lib/tests/test_nagios.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/lib/tests/test_python.py` & `batou-2.5.0b2/src/batou/lib/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/lib/tests/test_service.py` & `batou-2.5.0b2/src/batou/lib/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/lib/tests/test_supervisor.py` & `batou-2.5.0b2/src/batou/lib/tests/test_supervisor.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/lib/tests/test_svn.py` & `batou-2.5.0b2/src/batou/lib/tests/test_svn.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/main.py` & `batou-2.5.0b2/src/batou/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 import argparse
 import os
 import os.path
 import sys
 import textwrap
 from typing import Optional
 
-import pkg_resources
+import importlib_resources
 
 import batou
 import batou.deploy
 import batou.migrate
 import batou.secrets.edit
 import batou.secrets.encryption
 import batou.secrets.manage
 from batou._output import TerminalBackend, output
 
 
 def main(args: Optional[list] = None) -> None:
     os.chdir(os.environ["APPENV_BASEDIR"])
-    version = pkg_resources.resource_string(__name__, "version.txt")
-    version = version.decode("ascii").strip()
+    version = (
+        importlib_resources.files("batou")
+        .joinpath("version.txt")
+        .read_text()
+        .strip()
+    )
     parser = argparse.ArgumentParser(
         description=(
             "batou v{}: multi-(host|component|environment|version|platform)"
             " deployment"
         ).format(version),
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
```

### Comparing `batou-2.5.0b1/src/batou/migrate/__init__.py` & `batou-2.5.0b2/src/batou/migrate/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import importlib
 import json
 import textwrap
 from typing import List
 
-import pkg_resources
+import importlib_resources
 
 from batou._output import TerminalBackend, output
 
 CONFIG_FILE_NAME = ".batou.json"
 MIGRATION_MODULE = "batou.migrate"
 
 
@@ -37,17 +37,20 @@
     """
     with open(CONFIG_FILE_NAME) as f:
         return int(json.load(f)["migration"]["version"])
 
 
 def get_migration_steps() -> List[int]:
     """Return the sorted list of all known migration steps."""
-    migration_files = pkg_resources.resource_listdir(
-        MIGRATION_MODULE, "migrations"
+    migration_files = (
+        importlib_resources.files(MIGRATION_MODULE)
+        .joinpath("migrations")
+        .iterdir()
     )
+    migration_files = [x.name for x in migration_files]
     return sorted(
         int(x.partition(".")[0])
         for x in migration_files
         if not x.startswith(("_", "tests"))
     )
```

### Comparing `batou-2.5.0b1/src/batou/migrate/migrations/2301.py` & `batou-2.5.0b2/src/batou/migrate/migrations/2301.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/migrate/migrations/2302.py` & `batou-2.5.0b2/src/batou/migrate/migrations/2302.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/migrate/migrations/2303.py` & `batou-2.5.0b2/src/batou/migrate/migrations/2303.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/migrate/migrations/2400.py` & `batou-2.5.0b2/src/batou/migrate/migrations/2400.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/migrate/tests/test_migrate.py` & `batou-2.5.0b2/src/batou/migrate/tests/test_migrate.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/provision.py` & `batou-2.5.0b2/src/batou/provision.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/remote_core.py` & `batou-2.5.0b2/src/batou/remote_core.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/repository.py` & `batou-2.5.0b2/src/batou/repository.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/resources.py` & `batou-2.5.0b2/src/batou/resources.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/secrets/__init__.py` & `batou-2.5.0b2/src/batou/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/secrets/edit.py` & `batou-2.5.0b2/src/batou/secrets/edit.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/secrets/encryption.py` & `batou-2.5.0b2/src/batou/secrets/encryption.py`

 * *Files 1% similar despite different names*

```diff
@@ -486,17 +486,25 @@
         for section in config.sections():
             # if section is called batou, skip
             if section == "batou":
                 continue
             # for each option
             for option in config[section]:
                 # decrypt the value
-                config[section][option].value = self.decrypt_age_string(
+                decrypted = self.decrypt_age_string(
                     config[section][option].value
                 )
+                if "\n" in decrypted:
+                    # multiline: accounts for indents
+                    config[section][option].set_values(
+                        decrypted.split("\n"),
+                        prepend_newline=False,
+                    )
+                else:
+                    config[section][option].value = decrypted
 
         # cache the decrypted content
         self._decrypted_content = config
         self._encrypted_content = config_encrypted
 
         # return the decrypted content as bytes
         return str(config).encode("utf-8")
```

### Comparing `batou-2.5.0b1/src/batou/secrets/manage.py` & `batou-2.5.0b2/src/batou/secrets/manage.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/secrets/tests/test_editor.py` & `batou-2.5.0b2/src/batou/secrets/tests/test_editor.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/secrets/tests/test_manage.py` & `batou-2.5.0b2/src/batou/secrets/tests/test_manage.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/secrets/tests/test_secrets.py` & `batou-2.5.0b2/src/batou/secrets/tests/test_secrets.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import mock
 import pytest
 
 import batou
 from batou.secrets import GPGSecretProvider
 from batou.secrets.encryption import (
     AGEEncryptedFile,
+    DiffableAGEEncryptedFile,
     EncryptedFile,
     GPGEncryptedFile,
 )
 
 FIXTURE = pathlib.Path(__file__).parent / "fixture"
 cleartext_file = FIXTURE / "cleartext.cfg"
 FIXTURE_ENCRYPTED_CONFIG = FIXTURE / "encrypted.cfg"
@@ -139,7 +140,43 @@
 [asdf]
 x = 1
 """,
                 ["foobar@example.com"],
             )
 
     assert encrypted_file.read_bytes() == FIXTURE_ENCRYPTED_CONFIG.read_bytes()
+
+
+def test_write_and_read_age_diffable(encrypted_file):
+    encrypted = DiffableAGEEncryptedFile(
+        pathlib.Path(encrypted_file), writeable=True
+    )
+    content = b"""\
+[batou]
+members = ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIACZ8++sQADp8fztgumfw2i+WSgzMHB7MgSpkM2y5pHi batou-ci-test-key
+
+[asdf]
+value = This is a very long
+    multiline string
+    that should be encrypted
+    and decrypted correctly
+"""
+    # parse content as config to ensure that the content is valid
+    config = configparser.ConfigParser()
+    config.read_string(content.decode("utf-8"))
+
+    with encrypted as secrets:
+        secrets.write(
+            content,
+            [
+                "ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIACZ8++sQADp8fztgumfw2i+WSgzMHB7MgSpkM2y5pHi batou-ci-test-key"
+            ],
+        )
+
+    assert content != encrypted_file.read_bytes()
+    assert 0 != encrypted_file.stat().st_size
+
+    with DiffableAGEEncryptedFile(encrypted_file) as secrets:
+        # we want the multiline string to be read correctly
+        secret_config = configparser.ConfigParser()
+        secret_config.read_string(secrets.cleartext)
+        assert config["asdf"]["value"] == secret_config["asdf"]["value"]
```

### Comparing `batou-2.5.0b1/src/batou/template.py` & `batou-2.5.0b2/src/batou/template.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/tests/conftest.py` & `batou-2.5.0b2/src/batou/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/tests/ellipsis.py` & `batou-2.5.0b2/src/batou/tests/ellipsis.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/tests/fixture/sample_service/components/hello/component.py` & `batou-2.5.0b2/src/batou/tests/fixture/sample_service/components/hello/component.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/tests/test_component.py` & `batou-2.5.0b2/src/batou/tests/test_component.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/tests/test_config.py` & `batou-2.5.0b2/src/batou/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/tests/test_dependencies.py` & `batou-2.5.0b2/src/batou/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/tests/test_deploy.py` & `batou-2.5.0b2/src/batou/tests/test_deploy.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
             provision_rebuild=False,
         )
 
     assert r.value.code == 1
 
     out, err = capsys.readouterr()
     assert err == ""
+    # save the output to a file to compare it with the expected output
     assert out == Ellipsis(
         """\
 batou/2... (cpython 3...)
 ================================== Preparing ===================================
 main: Loading environment `errors`...
 main: Verifying repository ...
 main: Loading secrets ...
@@ -42,16 +43,15 @@
 
 ERROR: Failed loading component file
            File: .../examples/errors/components/component6/component.py
       Exception: No module named 'asdf'
 Traceback (simplified, most recent call last):
   File ".../examples/errors/components/component6/component.py", line 1, in <module>
     import asdf  # noqa: F401 import unused
-
-
+...
 ERROR: Missing component
       Component: missingcomponent
 
 ERROR: Superfluous section in environment configuration
         Section: superfluoussection
 
 ERROR: Override section for unknown component found
```

### Comparing `batou-2.5.0b1/src/batou/tests/test_endtoend.py` & `batou-2.5.0b2/src/batou/tests/test_endtoend.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,15 @@
 
 ERROR: Failed loading component file
            File: .../examples/errors/components/component6/component.py
       Exception: No module named 'asdf'
 Traceback (simplified, most recent call last):
   File ".../errors/components/component6/component.py", line 1, in <module>
     import asdf  # noqa: F401 import unused
-
-
+...
 ERROR: Missing component
       Component: missingcomponent
 
 ERROR: Superfluous section in environment configuration
         Section: superfluoussection
 
 ERROR: Override section for unknown component found
@@ -88,16 +87,15 @@
 
 ERROR: Failed loading component file
            File: .../examples/errors/components/component6/component.py
       Exception: No module named 'asdf'
 Traceback (simplified, most recent call last):
   File ".../examples/errors/components/component6/component.py", line 1, in <module>
     import asdf  # noqa: F401 import unused
-
-
+...
 ERROR: Missing component
       Component: missingcomponent
 
 ERROR: Superfluous section in environment configuration
         Section: superfluoussection
 
 ERROR: Override section for unknown component found
@@ -123,15 +121,15 @@
 
 ERROR: Trying to access address family IPv6 which is not configured for localhost:22.
            Hint: Use `require_v6=True` when instantiating the Address object.
 
 ERROR: crontab: No cron jobs found.
  Affected hosts: localhost
 
-ERROR: malformed node or string: <...Name object at 0x...>
+ERROR: malformed node or strin...: <...Name object at 0x...>
       Attribute: Component1.do_what_is_needed
      Conversion: convert_literal('false')
  Affected hosts: localhost
 
 ERROR: Error while expanding attribute:
         Message: TemplatingError: An error occured while rendering a template (Component5): KeyError: 'doesnotexist'
       Attribute: Component5.attribute_cannot_be_expanded
```

### Comparing `batou-2.5.0b1/src/batou/tests/test_environment.py` & `batou-2.5.0b2/src/batou/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/tests/test_exceptions.py` & `batou-2.5.0b2/src/batou/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/tests/test_host.py` & `batou-2.5.0b2/src/batou/tests/test_host.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/tests/test_main.py` & `batou-2.5.0b2/src/batou/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/tests/test_remote.py` & `batou-2.5.0b2/src/batou/tests/test_remote.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/tests/test_remote_core.py` & `batou-2.5.0b2/src/batou/tests/test_remote_core.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/tests/test_repository.py` & `batou-2.5.0b2/src/batou/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/tests/test_resources.py` & `batou-2.5.0b2/src/batou/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/tests/test_template.py` & `batou-2.5.0b2/src/batou/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/tests/test_utils.py` & `batou-2.5.0b2/src/batou/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/tests/test_vfs.py` & `batou-2.5.0b2/src/batou/tests/test_vfs.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou/utils.py` & `batou-2.5.0b2/src/batou/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import socket
 import subprocess
 import sys
 import time
 from collections import defaultdict
 from typing import Optional
 
-import pkg_resources
+import importlib_metadata
 
 from batou import (
     DeploymentError,
     GetAddressInfoError,
     IPAddressConfigurationError,
     output,
 )
@@ -40,15 +40,15 @@
         return self[key]
 
 
 def self_id():
     template = "batou/{version} ({python}, {system})"
     system = os.uname()
     system = " ".join([system[0], system[2], system[4]])
-    version = pkg_resources.require("batou")[0].version
+    version = importlib_metadata.version("batou")
     python = sys.implementation.name
     python += " {0}.{1}.{2}-{3}{4}".format(*sys.version_info)
     return template.format(**locals())
 
 
 class MultiFile(object):
     def __init__(self, files):
```

### Comparing `batou-2.5.0b1/src/batou/vfs.py` & `batou-2.5.0b2/src/batou/vfs.py`

 * *Files identical despite different names*

### Comparing `batou-2.5.0b1/src/batou.egg-info/PKG-INFO` & `batou-2.5.0b2/src/batou.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batou
-Version: 2.5.0b1
+Version: 2.5.0b2
 Summary: A utility for automating multi-host, multi-environment software builds and deployments.
 Home-page: https://batou.readthedocs.io/en/latest/
 Author: Christian Theune
 Author-email: ct@flyingcircus.io
 License: BSD (2-clause)
 Keywords: deployment
 Classifier: License :: OSI Approved :: BSD License
@@ -15,20 +15,21 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: ConfigUpdater>=3.0.1
-Requires-Dist: Jinja2==3.0.1
+Requires-Dist: Jinja2>=3.1.4
 Requires-Dist: requests
 Requires-Dist: setuptools>=38.3
 Requires-Dist: execnet>=1.8.1
 Requires-Dist: importlib_metadata
-Requires-Dist: py
+Requires-Dist: importlib_resources
+Requires-Dist: py>=1.11.0
 Requires-Dist: pyyaml
 Requires-Dist: remote-pdb
 Provides-Extra: test
 Requires-Dist: mock; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-coverage; extra == "test"
 Requires-Dist: pytest-instafail; extra == "test"
```

### Comparing `batou-2.5.0b1/src/batou.egg-info/SOURCES.txt` & `batou-2.5.0b2/src/batou.egg-info/SOURCES.txt`

 * *Files identical despite different names*

