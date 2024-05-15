# Comparing `tmp/giger-0.1.8.tar.gz` & `tmp/giger-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giger-0.1.8.tar", last modified: Thu Aug 17 22:58:52 2023, max compression
+gzip compressed data, was "giger-0.1.9.tar", last modified: Sat Aug 19 16:08:33 2023, max compression
```

## Comparing `giger-0.1.8.tar` & `giger-0.1.9.tar`

### file list

```diff
@@ -1,155 +1,165 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.316604 giger-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-17 22:51:19.000000 giger-0.1.8/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)     9504 2023-08-17 22:51:19.000000 giger-0.1.8/.gitchangelog.rc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.236603 giger-0.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.264603 giger-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-08-17 22:51:19.000000 giger-0.1.8/.github/workflows/documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-08-17 22:51:19.000000 giger-0.1.8/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-08-17 22:51:19.000000 giger-0.1.8/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-17 22:51:19.000000 giger-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-17 22:51:19.000000 giger-0.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-17 22:51:19.000000 giger-0.1.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-17 22:51:19.000000 giger-0.1.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-08-17 22:51:19.000000 giger-0.1.8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11630 2023-08-17 22:51:19.000000 giger-0.1.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-17 22:51:19.000000 giger-0.1.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-17 22:51:19.000000 giger-0.1.8/Manifest.in
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-08-17 22:58:52.316604 giger-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-08-17 22:51:19.000000 giger-0.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.272604 giger-0.1.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-17 22:51:19.000000 giger-0.1.8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.272604 giger-0.1.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-17 22:51:19.000000 giger-0.1.8/docs/_static/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.272604 giger-0.1.8/docs/_static/styles/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-08-17 22:51:19.000000 giger-0.1.8/docs/_static/styles/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.272604 giger-0.1.8/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-08-17 22:51:19.000000 giger-0.1.8/docs/_templates/page.html
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-17 22:51:19.000000 giger-0.1.8/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-17 22:51:19.000000 giger-0.1.8/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-08-17 22:51:19.000000 giger-0.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-17 22:51:19.000000 giger-0.1.8/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-08-17 22:51:19.000000 giger-0.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-17 22:51:19.000000 giger-0.1.8/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-17 22:51:19.000000 giger-0.1.8/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-17 22:51:19.000000 giger-0.1.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.240603 giger-0.1.8/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.240603 giger-0.1.8/examples/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.236603 giger-0.1.8/examples/assets/img/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.284604 giger-0.1.8/examples/assets/img/faces/
--rw-r--r--   0 runner    (1001) docker     (123)   436995 2023-08-17 22:51:19.000000 giger-0.1.8/examples/assets/img/faces/johann.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    89758 2023-08-17 22:51:19.000000 giger-0.1.8/examples/assets/img/faces/kevin.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    41504 2023-08-17 22:51:19.000000 giger-0.1.8/examples/assets/img/faces/leif.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    34171 2023-08-17 22:51:19.000000 giger-0.1.8/examples/assets/img/faces/palina.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   119989 2023-08-17 22:51:19.000000 giger-0.1.8/examples/assets/img/faces/peter.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   151489 2023-08-17 22:51:19.000000 giger-0.1.8/examples/assets/img/faces/zakk.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.292604 giger-0.1.8/examples/assets/img/sketches/
--rw-r--r--   0 runner    (1001) docker     (123)    64768 2023-08-17 22:51:19.000000 giger-0.1.8/examples/assets/img/sketches/honeymachine.png
--rw-r--r--   0 runner    (1001) docker     (123)    20067 2023-08-17 22:51:19.000000 giger-0.1.8/examples/assets/img/sketches/zonk.png
--rw-r--r--   0 runner    (1001) docker     (123)    27881 2023-08-17 22:51:19.000000 giger-0.1.8/examples/assets/img/sketches/zuri.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.240603 giger-0.1.8/examples/assets/txt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.296604 giger-0.1.8/examples/assets/txt/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-17 22:51:19.000000 giger-0.1.8/examples/assets/txt/prompts/_negative.txt
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-17 22:51:19.000000 giger-0.1.8/examples/assets/txt/prompts/graffiti.txt
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-08-17 22:51:19.000000 giger-0.1.8/examples/assets/txt/prompts/gravedigger.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-17 22:51:19.000000 giger-0.1.8/examples/assets/txt/prompts/spawn.txt
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-17 22:51:19.000000 giger-0.1.8/examples/assets/txt/prompts/vampire.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-17 22:51:19.000000 giger-0.1.8/examples/assets/txt/prompts/viking.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.240603 giger-0.1.8/examples/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.296604 giger-0.1.8/examples/scripts/batch/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3395 2023-08-17 22:51:19.000000 giger-0.1.8/examples/scripts/batch/images.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      344 2023-08-17 22:51:19.000000 giger-0.1.8/examples/scripts/batch/roop.sh
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-08-17 22:51:19.000000 giger-0.1.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.296604 giger-0.1.8/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-17 22:51:19.000000 giger-0.1.8/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-08-17 22:58:52.316604 giger-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-08-17 22:51:19.000000 giger-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.240603 giger-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.296604 giger-0.1.8/src/giger/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-08-17 22:51:19.000000 giger-0.1.8/src/giger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-08-17 22:51:19.000000 giger-0.1.8/src/giger/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.300604 giger-0.1.8/src/giger/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-08-17 22:51:19.000000 giger-0.1.8/src/giger/commands/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-08-17 22:51:19.000000 giger-0.1.8/src/giger/commands/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-08-17 22:51:19.000000 giger-0.1.8/src/giger/commands/roop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-08-17 22:51:19.000000 giger-0.1.8/src/giger/commands/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.300604 giger-0.1.8/src/giger/services/
--rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-08-17 22:51:19.000000 giger-0.1.8/src/giger/services/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    13345 2023-08-17 22:51:19.000000 giger-0.1.8/src/giger/services/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-08-17 22:51:19.000000 giger-0.1.8/src/giger/services/roop.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-08-17 22:51:19.000000 giger-0.1.8/src/giger/services/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.300604 giger-0.1.8/src/giger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-08-17 22:58:52.000000 giger-0.1.8/src/giger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-08-17 22:58:52.000000 giger-0.1.8/src/giger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-17 22:58:52.000000 giger-0.1.8/src/giger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-17 22:58:52.000000 giger-0.1.8/src/giger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-17 22:51:31.000000 giger-0.1.8/src/giger.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-17 22:58:52.000000 giger-0.1.8/src/giger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-17 22:58:52.000000 giger-0.1.8/src/giger.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.300604 giger-0.1.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.300604 giger-0.1.8/tests/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-08-17 22:51:19.000000 giger-0.1.8/tests/commands/test_image_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-08-17 22:51:19.000000 giger-0.1.8/tests/commands/test_prompt_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-08-17 22:51:19.000000 giger-0.1.8/tests/commands/test_roop_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-08-17 22:51:19.000000 giger-0.1.8/tests/commands/test_template_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-17 22:51:19.000000 giger-0.1.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.304604 giger-0.1.8/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)    11793 2023-08-17 22:51:19.000000 giger-0.1.8/tests/fixtures/face.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    30558 2023-08-17 22:51:19.000000 giger-0.1.8/tests/fixtures/fail.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-17 22:51:19.000000 giger-0.1.8/tests/fixtures/hero.yml
--rw-r--r--   0 runner    (1001) docker     (123)    42528 2023-08-17 22:51:19.000000 giger-0.1.8/tests/fixtures/input.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.304604 giger-0.1.8/tests/services/
--rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-08-17 22:51:19.000000 giger-0.1.8/tests/services/test_image_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-08-17 22:51:19.000000 giger-0.1.8/tests/services/test_prompt_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-08-17 22:51:19.000000 giger-0.1.8/tests/services/test_roop_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-08-17 22:51:19.000000 giger-0.1.8/tests/services/test_template_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.252603 giger-0.1.8/tests/snapshots/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.248603 giger-0.1.8/tests/snapshots/cli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.304604 giger-0.1.8/tests/snapshots/cli/image/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-17 22:51:19.000000 giger-0.1.8/tests/snapshots/cli/image/basic.yml.snapshot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.304604 giger-0.1.8/tests/snapshots/cli/prompt/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-08-17 22:51:19.000000 giger-0.1.8/tests/snapshots/cli/prompt/basic.yml.snapshot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.304604 giger-0.1.8/tests/snapshots/cli/roop/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-17 22:51:19.000000 giger-0.1.8/tests/snapshots/cli/roop/basic.yml.snapshot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.304604 giger-0.1.8/tests/snapshots/cli/template/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-08-17 22:51:19.000000 giger-0.1.8/tests/snapshots/cli/template/basic.yml.snapshot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.252603 giger-0.1.8/tests/snapshots/commands/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.252603 giger-0.1.8/tests/snapshots/commands/image/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.304604 giger-0.1.8/tests/snapshots/commands/image/controlnet/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-17 22:51:19.000000 giger-0.1.8/tests/snapshots/commands/image/controlnet/basic.yml.snapshot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.304604 giger-0.1.8/tests/snapshots/commands/image/img2img/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-17 22:51:19.000000 giger-0.1.8/tests/snapshots/commands/image/img2img/basic.yml.snapshot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.304604 giger-0.1.8/tests/snapshots/commands/image/txt2img/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-08-17 22:51:19.000000 giger-0.1.8/tests/snapshots/commands/image/txt2img/basic.yml.snapshot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.304604 giger-0.1.8/tests/snapshots/commands/prompt/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-17 22:51:19.000000 giger-0.1.8/tests/snapshots/commands/prompt/basic.yml.snapshot
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-17 22:51:19.000000 giger-0.1.8/tests/snapshots/commands/prompt/output.yml.snapshot
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-17 22:51:19.000000 giger-0.1.8/tests/snapshots/commands/prompt/stdin.yml.snapshot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.304604 giger-0.1.8/tests/snapshots/commands/roop/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-17 22:51:19.000000 giger-0.1.8/tests/snapshots/commands/roop/basic.yml.snapshot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.308604 giger-0.1.8/tests/snapshots/commands/template/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-17 22:51:19.000000 giger-0.1.8/tests/snapshots/commands/template/basic.yml.snapshot
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-17 22:51:19.000000 giger-0.1.8/tests/snapshots/commands/template/data.yml.snapshot
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-17 22:51:19.000000 giger-0.1.8/tests/snapshots/commands/template/output.yml.snapshot
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-17 22:51:19.000000 giger-0.1.8/tests/snapshots/commands/template/stdin.yml.snapshot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.256603 giger-0.1.8/tests/snapshots/services/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.256603 giger-0.1.8/tests/snapshots/services/image/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.312604 giger-0.1.8/tests/snapshots/services/image/controlnet/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-17 22:51:19.000000 giger-0.1.8/tests/snapshots/services/image/controlnet/basic.from_pretrained.yml.snapshot
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-17 22:51:19.000000 giger-0.1.8/tests/snapshots/services/image/controlnet/basic.pipeline.yml.snapshot
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-17 22:51:19.000000 giger-0.1.8/tests/snapshots/services/image/controlnet/cuda.from_pretrained.yml.snapshot
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-17 22:51:19.000000 giger-0.1.8/tests/snapshots/services/image/controlnet/cuda.pipeline.yml.snapshot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.312604 giger-0.1.8/tests/snapshots/services/image/img2img/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-17 22:51:19.000000 giger-0.1.8/tests/snapshots/services/image/img2img/basic.from_pretrained.yml.snapshot
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-17 22:51:19.000000 giger-0.1.8/tests/snapshots/services/image/img2img/basic.pipeline.yml.snapshot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.312604 giger-0.1.8/tests/snapshots/services/image/txt2img/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-17 22:51:19.000000 giger-0.1.8/tests/snapshots/services/image/txt2img/basic.from_pretrained.yml.snapshot
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-17 22:51:19.000000 giger-0.1.8/tests/snapshots/services/image/txt2img/basic.pipeline.yml.snapshot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 22:58:52.316604 giger-0.1.8/tests/snapshots/services/prompt/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-08-17 22:51:19.000000 giger-0.1.8/tests/snapshots/services/prompt/advanced.txt.snapshot
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-17 22:51:19.000000 giger-0.1.8/tests/snapshots/services/prompt/basic.txt.snapshot
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-08-17 22:51:19.000000 giger-0.1.8/tests/snapshots/services/prompt/compel_full.txt.snapshot
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-17 22:51:19.000000 giger-0.1.8/tests/snapshots/services/prompt/compel_full_full.txt.snapshot
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-08-17 22:51:19.000000 giger-0.1.8/tests/snapshots/services/prompt/compel_subtle.txt.snapshot
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-17 22:51:19.000000 giger-0.1.8/tests/snapshots/services/prompt/compel_subtle_empty.txt.snapshot
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-08-17 22:51:19.000000 giger-0.1.8/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-08-17 22:51:19.000000 giger-0.1.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.127545 giger-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-19 16:02:08.000000 giger-0.1.9/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)     9504 2023-08-19 16:02:08.000000 giger-0.1.9/.gitchangelog.rc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.071545 giger-0.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.095545 giger-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-08-19 16:02:08.000000 giger-0.1.9/.github/workflows/documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-08-19 16:02:08.000000 giger-0.1.9/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-08-19 16:02:08.000000 giger-0.1.9/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-19 16:02:08.000000 giger-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-08-19 16:02:08.000000 giger-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-19 16:02:08.000000 giger-0.1.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-19 16:02:08.000000 giger-0.1.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-08-19 16:02:08.000000 giger-0.1.9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11630 2023-08-19 16:02:08.000000 giger-0.1.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-19 16:02:08.000000 giger-0.1.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-19 16:02:08.000000 giger-0.1.9/Manifest.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-08-19 16:08:33.127545 giger-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-08-19 16:02:08.000000 giger-0.1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.099545 giger-0.1.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-19 16:02:08.000000 giger-0.1.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.099545 giger-0.1.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-19 16:02:08.000000 giger-0.1.9/docs/_static/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.099545 giger-0.1.9/docs/_static/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-08-19 16:02:08.000000 giger-0.1.9/docs/_static/styles/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.099545 giger-0.1.9/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-08-19 16:02:08.000000 giger-0.1.9/docs/_templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-19 16:02:08.000000 giger-0.1.9/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-19 16:02:08.000000 giger-0.1.9/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-08-19 16:02:08.000000 giger-0.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-19 16:02:08.000000 giger-0.1.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-08-19 16:02:08.000000 giger-0.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-19 16:02:08.000000 giger-0.1.9/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-19 16:02:08.000000 giger-0.1.9/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-19 16:02:08.000000 giger-0.1.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.075544 giger-0.1.9/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.075544 giger-0.1.9/examples/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.103545 giger-0.1.9/examples/assets/fonts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24224 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/fonts/AnotherTag.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    38692 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/fonts/Marsneveneksk.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45888 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/fonts/MostWasted.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.075544 giger-0.1.9/examples/assets/img/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.107545 giger-0.1.9/examples/assets/img/faces/
+-rw-r--r--   0 runner    (1001) docker     (123)   436995 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/img/faces/johann.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    89758 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/img/faces/kevin.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    41504 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/img/faces/leif.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    34171 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/img/faces/palina.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   119989 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/img/faces/peter.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   151489 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/img/faces/zakk.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.111545 giger-0.1.9/examples/assets/img/sketches/
+-rw-r--r--   0 runner    (1001) docker     (123)    64768 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/img/sketches/honeymachine.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20067 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/img/sketches/zonk.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27881 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/img/sketches/zuri.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.075544 giger-0.1.9/examples/assets/txt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.115545 giger-0.1.9/examples/assets/txt/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/txt/prompts/_negative.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/txt/prompts/graffiti.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/txt/prompts/gravedigger.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/txt/prompts/spawn.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.115545 giger-0.1.9/examples/assets/txt/prompts/vampire/
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/txt/prompts/vampire/ancient.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/txt/prompts/vampire/modern.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/txt/prompts/viking.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.115545 giger-0.1.9/examples/batch/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-08-19 16:02:08.000000 giger-0.1.9/examples/batch/README.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5660 2023-08-19 16:02:08.000000 giger-0.1.9/examples/batch/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-19 16:02:08.000000 giger-0.1.9/examples/batch/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.115545 giger-0.1.9/examples/graffiti/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-08-19 16:02:08.000000 giger-0.1.9/examples/graffiti/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-08-19 16:02:08.000000 giger-0.1.9/examples/graffiti/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-19 16:02:08.000000 giger-0.1.9/examples/graffiti/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-08-19 16:02:08.000000 giger-0.1.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.115545 giger-0.1.9/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-19 16:02:08.000000 giger-0.1.9/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-08-19 16:08:33.127545 giger-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-08-19 16:02:08.000000 giger-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.079544 giger-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.115545 giger-0.1.9/src/giger/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-08-19 16:02:08.000000 giger-0.1.9/src/giger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-08-19 16:02:08.000000 giger-0.1.9/src/giger/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.119545 giger-0.1.9/src/giger/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-08-19 16:02:08.000000 giger-0.1.9/src/giger/commands/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-08-19 16:02:08.000000 giger-0.1.9/src/giger/commands/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-08-19 16:02:08.000000 giger-0.1.9/src/giger/commands/roop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-08-19 16:02:08.000000 giger-0.1.9/src/giger/commands/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.119545 giger-0.1.9/src/giger/services/
+-rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-08-19 16:02:08.000000 giger-0.1.9/src/giger/services/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13400 2023-08-19 16:02:08.000000 giger-0.1.9/src/giger/services/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-08-19 16:02:08.000000 giger-0.1.9/src/giger/services/roop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-08-19 16:02:08.000000 giger-0.1.9/src/giger/services/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.119545 giger-0.1.9/src/giger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-08-19 16:08:33.000000 giger-0.1.9/src/giger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-08-19 16:08:33.000000 giger-0.1.9/src/giger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-19 16:08:33.000000 giger-0.1.9/src/giger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-19 16:08:33.000000 giger-0.1.9/src/giger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-19 16:02:18.000000 giger-0.1.9/src/giger.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-19 16:08:33.000000 giger-0.1.9/src/giger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-19 16:08:33.000000 giger-0.1.9/src/giger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.119545 giger-0.1.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.119545 giger-0.1.9/tests/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-08-19 16:02:08.000000 giger-0.1.9/tests/commands/test_image_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-08-19 16:02:08.000000 giger-0.1.9/tests/commands/test_prompt_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-08-19 16:02:08.000000 giger-0.1.9/tests/commands/test_roop_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-08-19 16:02:08.000000 giger-0.1.9/tests/commands/test_template_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-19 16:02:08.000000 giger-0.1.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.119545 giger-0.1.9/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)    11793 2023-08-19 16:02:08.000000 giger-0.1.9/tests/fixtures/face.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    30558 2023-08-19 16:02:08.000000 giger-0.1.9/tests/fixtures/fail.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-19 16:02:08.000000 giger-0.1.9/tests/fixtures/hero.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    42528 2023-08-19 16:02:08.000000 giger-0.1.9/tests/fixtures/input.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.119545 giger-0.1.9/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-08-19 16:02:08.000000 giger-0.1.9/tests/services/test_image_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-08-19 16:02:08.000000 giger-0.1.9/tests/services/test_prompt_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-08-19 16:02:08.000000 giger-0.1.9/tests/services/test_roop_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-08-19 16:02:08.000000 giger-0.1.9/tests/services/test_template_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.083545 giger-0.1.9/tests/snapshots/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.083545 giger-0.1.9/tests/snapshots/cli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.123545 giger-0.1.9/tests/snapshots/cli/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/cli/image/basic.yml.snapshot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.123545 giger-0.1.9/tests/snapshots/cli/prompt/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/cli/prompt/basic.yml.snapshot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.123545 giger-0.1.9/tests/snapshots/cli/roop/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/cli/roop/basic.yml.snapshot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.123545 giger-0.1.9/tests/snapshots/cli/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/cli/template/basic.yml.snapshot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.083545 giger-0.1.9/tests/snapshots/commands/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.083545 giger-0.1.9/tests/snapshots/commands/image/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.123545 giger-0.1.9/tests/snapshots/commands/image/controlnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/commands/image/controlnet/basic.yml.snapshot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.123545 giger-0.1.9/tests/snapshots/commands/image/img2img/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/commands/image/img2img/basic.yml.snapshot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.123545 giger-0.1.9/tests/snapshots/commands/image/txt2img/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/commands/image/txt2img/basic.yml.snapshot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.123545 giger-0.1.9/tests/snapshots/commands/prompt/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/commands/prompt/basic.yml.snapshot
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/commands/prompt/output.yml.snapshot
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/commands/prompt/stdin.yml.snapshot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.123545 giger-0.1.9/tests/snapshots/commands/roop/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/commands/roop/basic.yml.snapshot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.123545 giger-0.1.9/tests/snapshots/commands/template/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/commands/template/basic.yml.snapshot
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/commands/template/data.yml.snapshot
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/commands/template/output.yml.snapshot
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/commands/template/stdin.yml.snapshot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.087545 giger-0.1.9/tests/snapshots/services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.087545 giger-0.1.9/tests/snapshots/services/image/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.123545 giger-0.1.9/tests/snapshots/services/image/controlnet/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/services/image/controlnet/basic.from_pretrained.yml.snapshot
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/services/image/controlnet/basic.pipeline.yml.snapshot
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/services/image/controlnet/cuda.from_pretrained.yml.snapshot
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/services/image/controlnet/cuda.pipeline.yml.snapshot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.123545 giger-0.1.9/tests/snapshots/services/image/img2img/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/services/image/img2img/basic.from_pretrained.yml.snapshot
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/services/image/img2img/basic.pipeline.yml.snapshot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.123545 giger-0.1.9/tests/snapshots/services/image/txt2img/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/services/image/txt2img/basic.from_pretrained.yml.snapshot
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/services/image/txt2img/basic.pipeline.yml.snapshot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.127545 giger-0.1.9/tests/snapshots/services/prompt/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/services/prompt/advanced.txt.snapshot
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/services/prompt/basic.txt.snapshot
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/services/prompt/compel_full.txt.snapshot
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/services/prompt/compel_full_full.txt.snapshot
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/services/prompt/compel_subtle.txt.snapshot
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/services/prompt/compel_subtle_empty.txt.snapshot
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-08-19 16:02:08.000000 giger-0.1.9/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-08-19 16:02:08.000000 giger-0.1.9/tox.ini
```

### Comparing `giger-0.1.8/.coveragerc` & `giger-0.1.9/.coveragerc`

 * *Files identical despite different names*

### Comparing `giger-0.1.8/.gitchangelog.rc` & `giger-0.1.9/.gitchangelog.rc`

 * *Files identical despite different names*

### Comparing `giger-0.1.8/.github/workflows/documentation.yml` & `giger-0.1.9/.github/workflows/documentation.yml`

 * *Files 7% similar despite different names*

```diff
@@ -35,15 +35,15 @@
           fetch-depth: 0
       - name: Setup Pages
         uses: actions/configure-pages@v3
       - name: Setup Python
         uses: actions/setup-python@v3
       - name: Install dependencies
         run: |
-          pip install -r docs/requirements.txt && pip install -r requirements.txt
+          pip install -r docs/requirements.txt && pip install -e .
       - name: Sphinx build
         run: |
           make -C docs html
       - name: Upload artifact
         uses: actions/upload-pages-artifact@v2
         with:
           # Upload entire repository
```

### Comparing `giger-0.1.8/.github/workflows/publish.yml` & `giger-0.1.9/.github/workflows/publish.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 name: Publish
 
 on:
   push:
     tags:
       - "[0-9]+.[0-9]+.[0-9]+"
+  # Allows you to run this workflow manually from the Actions tab
+  workflow_dispatch:
 
 jobs:
   publish:
     environment:
       name: publish
     runs-on: ubuntu-latest
     steps:
```

### Comparing `giger-0.1.8/.github/workflows/test.yml` & `giger-0.1.9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `giger-0.1.8/.gitignore` & `giger-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `giger-0.1.8/.pre-commit-config.yaml` & `giger-0.1.9/.pre-commit-config.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -15,7 +15,12 @@
       - id: isort
         name: isort (python)
         args: ["--profile", "black"]
   - repo: https://github.com/psf/black
     rev: 23.7.0
     hooks:
       - id: black
+  - repo: https://github.com/compilerla/conventional-pre-commit
+    rev: v2.3.0
+    hooks:
+      - id: conventional-pre-commit
+        stages: [commit-msg]
```

### Comparing `giger-0.1.8/.readthedocs.yml` & `giger-0.1.9/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `giger-0.1.8/CHANGELOG.rst` & `giger-0.1.9/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,42 @@
 Changelog
 =========
 
 
+0.1.9 (2023-08-19)
+------------------
+
+Fix
+~~~
+- Image seed generator cuda switch. [Sebastian Krüger]
+- Prompt camera style, improve startup time. [Sebastian Krüger]
+
+Changes
+~~~~~~~
+- Remove cuda from tests. [Sebastian Krüger]
+- Fix batch seed. [Sebastian Krüger]
+- Fix batch. [Sebastian Krüger]
+- Bash batch scripts to python. [Sebastian Krüger]
+- Remove docs hint. [Sebastian Krüger]
+- Pre-commit conventional-commit. [Sebastian Krüger]
+- Graffiti example with streamlit. [Sebastian Krüger]
+- Docs workflow. [Sebastian Krüger]
+
+
 0.1.8 (2023-08-17)
 ------------------
 
 Fix
 ~~~
 - Runtime dependencies. [Sebastian Krüger]
 
+Other
+~~~~~
+- CHANGELOG. [Sebastian Krüger]
+
 
 0.1.7 (2023-08-17)
 ------------------
 
 Fix
 ~~~
 - Dtype for non cuda devices. [Sebastian Krüger]
```

### Comparing `giger-0.1.8/CONTRIBUTING.rst` & `giger-0.1.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `giger-0.1.8/LICENSE.txt` & `giger-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `giger-0.1.8/PKG-INFO` & `giger-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giger
-Version: 0.1.8
+Version: 0.1.9
 Summary: CLI for Stable Diffusion tasks.
 Home-page: https://github.com/artificialhoney/giger/
 Author: Sebastian Krüger
 Author-email: sk@honeymachine.io
 License: MIT
 Project-URL: Documentation, https://artificialhoney.github.io/giger/
 Project-URL: Source, https://github.com/artificialhoney/giger/
@@ -50,15 +50,15 @@
 
    pip install giger
 
 -----
 Usage
 -----
 
-Please check first of all the help function and the `examples <https://github.com/artificialhoney/giger/tree/main/examples/scripts/>`_.
+Please check first of all the help function and the `examples <https://github.com/artificialhoney/giger/tree/main/examples/>`_.
 
 .. code-block:: bash
 
     giger --help
 
 Also make sure to always obtain the latest version.
```

### Comparing `giger-0.1.8/README.rst` & `giger-0.1.9/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
    pip install giger
 
 -----
 Usage
 -----
 
-Please check first of all the help function and the `examples <https://github.com/artificialhoney/giger/tree/main/examples/scripts/>`_.
+Please check first of all the help function and the `examples <https://github.com/artificialhoney/giger/tree/main/examples/>`_.
 
 .. code-block:: bash
 
     giger --help
 
 Also make sure to always obtain the latest version.
```

### Comparing `giger-0.1.8/docs/Makefile` & `giger-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `giger-0.1.8/docs/_templates/page.html` & `giger-0.1.9/docs/_templates/page.html`

 * *Files identical despite different names*

### Comparing `giger-0.1.8/docs/conf.py` & `giger-0.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `giger-0.1.8/examples/assets/img/faces/johann.jpg` & `giger-0.1.9/examples/assets/img/faces/johann.jpg`

 * *Files identical despite different names*

### Comparing `giger-0.1.8/examples/assets/img/faces/kevin.jpg` & `giger-0.1.9/examples/assets/img/faces/kevin.jpg`

 * *Files identical despite different names*

### Comparing `giger-0.1.8/examples/assets/img/faces/leif.jpg` & `giger-0.1.9/examples/assets/img/faces/leif.jpg`

 * *Files identical despite different names*

### Comparing `giger-0.1.8/examples/assets/img/faces/palina.jpg` & `giger-0.1.9/examples/assets/img/faces/palina.jpg`

 * *Files identical despite different names*

### Comparing `giger-0.1.8/examples/assets/img/faces/peter.jpg` & `giger-0.1.9/examples/assets/img/faces/peter.jpg`

 * *Files identical despite different names*

### Comparing `giger-0.1.8/examples/assets/img/faces/zakk.jpg` & `giger-0.1.9/examples/assets/img/faces/zakk.jpg`

 * *Files identical despite different names*

### Comparing `giger-0.1.8/examples/assets/img/sketches/honeymachine.png` & `giger-0.1.9/examples/assets/img/sketches/honeymachine.png`

 * *Files identical despite different names*

### Comparing `giger-0.1.8/examples/assets/img/sketches/zonk.png` & `giger-0.1.9/examples/assets/img/sketches/zonk.png`

 * *Files identical despite different names*

### Comparing `giger-0.1.8/examples/assets/img/sketches/zuri.png` & `giger-0.1.9/examples/assets/img/sketches/zuri.png`

 * *Files identical despite different names*

### Comparing `giger-0.1.8/examples/assets/txt/prompts/_negative.txt` & `giger-0.1.9/examples/assets/txt/prompts/_negative.txt`

 * *Files identical despite different names*

### Comparing `giger-0.1.8/examples/assets/txt/prompts/vampire.txt` & `giger-0.1.9/examples/assets/txt/prompts/vampire/ancient.txt`

 * *Files identical despite different names*

### Comparing `giger-0.1.8/setup.cfg` & `giger-0.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `giger-0.1.8/setup.py` & `giger-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `giger-0.1.8/src/giger/__init__.py` & `giger-0.1.9/src/giger/__init__.py`

 * *Files identical despite different names*

### Comparing `giger-0.1.8/src/giger/cli.py` & `giger-0.1.9/src/giger/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 #!/usr/bin/env python
 
 import argparse
 import logging
 import sys
 import warnings
 
-from diffusers import utils
-
 from giger import __version__
 
 from .commands.image import ImageCommand
 from .commands.prompt import PromptCommand
 from .commands.roop import RoopCommand
 from .commands.template import TemplateCommand
 
@@ -80,29 +78,30 @@
         logging.basicConfig(
             level=loglevel,
             stream=sys.stdout,
             format=logformat,
             datefmt="%Y-%m-%d %H:%M:%S",
         )
 
-        if loglevel == logging.DEBUG:
-            utils.logging.set_verbosity_debug()
-        elif loglevel == logging.INFO:
-            utils.logging.set_verbosity_info()
-        else:
-            utils.logging.set_verbosity_error()
-
     def run(self, args):
         args = self.parse_args(args)
         self.setup_logging(args.loglevel)
         if args.command == "template":
             self.template.execute(args)
         elif args.command == "prompt":
             self.prompt.execute(args)
         elif args.command == "image":
+            from diffusers import utils
+
+            if args.loglevel == logging.DEBUG:
+                utils.logging.set_verbosity_debug()
+            elif args.loglevel == logging.INFO:
+                utils.logging.set_verbosity_info()
+            else:
+                utils.logging.set_verbosity_error()
             self.image.execute(args)
         else:
             self.roop.execute(args)
 
 
 def run():
     CLI().run(sys.argv[1:])
```

### Comparing `giger-0.1.8/src/giger/commands/image.py` & `giger-0.1.9/src/giger/commands/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,17 +90,18 @@
 
         _logger.info('Creating image for "{0}"'.format(prompt))
 
         from ..services.image import ImageService
 
         self.service = ImageService()
 
+        path = os.path.join(args.output, args.name)
+        pathlib.Path(path).mkdir(parents=True, exist_ok=True)
+
         for x in range(args.batch_count):
-            path = os.path.join(args.output, args.name)
-            pathlib.Path(path).mkdir(parents=True, exist_ok=True)
             s = seed + x * args.batch_size
             if args.input != None:
                 if args.controlnet_model != None:
                     self.service.controlnet(
                         args.model,
                         prompt,
                         args.negative_prompt,
```

### Comparing `giger-0.1.8/src/giger/commands/prompt.py` & `giger-0.1.9/src/giger/commands/prompt.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,17 @@
         self.parser.add_argument(
             "--lightning_style", choices=PromptService.lightning_styles(), nargs="*"
         )
         self.parser.add_argument(
             "--camera_position", choices=PromptService.camera_positions(), nargs="*"
         )
         self.parser.add_argument("--camera", choices=PromptService.cameras(), nargs="*")
-        self.parser.add_argument("--style", choices=PromptService.styles(), nargs="*")
+        self.parser.add_argument(
+            "--camera_style", choices=PromptService.camera_styles(), nargs="*"
+        )
         self.parser.add_argument(
             "--composition", choices=PromptService.compositions(), nargs="*"
         )
         self.parser.add_argument("--iso", choices=PromptService.isos())
         self.parser.add_argument(
             "--resolution", choices=PromptService.resolutions(), nargs="*"
         )
```

### Comparing `giger-0.1.8/src/giger/commands/roop.py` & `giger-0.1.9/src/giger/commands/roop.py`

 * *Files identical despite different names*

### Comparing `giger-0.1.8/src/giger/commands/template.py` & `giger-0.1.9/src/giger/commands/template.py`

 * *Files identical despite different names*

### Comparing `giger-0.1.8/src/giger/services/image.py` & `giger-0.1.9/src/giger/services/image.py`

 * *Files 4% similar despite different names*

```diff
@@ -137,15 +137,21 @@
                     + str(seed + x).rjust(6, "0")
                     + ".png",
                 ),
                 exif=exif_bytes,
             )
 
     def _create_generator(self, seed, count):
-        return [torch.Generator().manual_seed(i + seed) for i in range(count)]
+        if self.cuda:
+            return [
+                torch.Generator(device="cuda").manual_seed(i + seed)
+                for i in range(count)
+            ]
+        else:
+            return [torch.Generator().manual_seed(i + seed) for i in range(count)]
 
     def _get_exif_bytes(self, prompt):
         exif_ifd = {piexif.ImageIFD.ImageDescription: prompt.encode()}
         exif_dict = {
             "0th": exif_ifd,
             "Exif": {},
             "1st": {},
```

### Comparing `giger-0.1.8/src/giger/services/prompt.py` & `giger-0.1.9/src/giger/services/prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -326,15 +326,15 @@
             "Canon",
             "Leica M",
             "Leica" "Nikon",
             "Sony alpha",
             "{{camera}}",
         ]
 
-    def styles():
+    def camera_styles():
         return [
             "Early Wet Plate",
             "Fisheye",
             "Golden hour",
             "Infrared",
             "Kodachrome",
             "Long Exposure",
@@ -384,14 +384,15 @@
         artist=None,
         realism=None,
         rendering_engine=None,
         lightning_angle=None,
         lightning_style=None,
         camera_position=None,
         camera=None,
+        camera_style=None,
         composition=None,
         iso=None,
         resolution=None,
         compel_style=None,
     ):
         separator = ", "
 
@@ -422,16 +423,16 @@
             image.append(separator.join(lightning_angle))
         if lightning_style != None and len(lightning_style) > 0:
             image.append(separator.join(lightning_style))
         if camera_position != None and len(camera_position) > 0:
             image.append(separator.join(camera_position))
         if camera != None and len(camera) > 0:
             image.append(separator.join(camera))
-        if style != None and len(style) > 0:
-            image.append(separator.join(style))
+        if camera_style != None and len(camera_style) > 0:
+            image.append(separator.join(camera_style))
         if composition != None and len(composition) > 0:
             image.append(separator.join(composition))
         if iso != None:
             image.append(iso)
         if resolution != None and len(resolution) > 0:
             image.append(separator.join(resolution))
```

### Comparing `giger-0.1.8/src/giger/services/roop.py` & `giger-0.1.9/src/giger/services/roop.py`

 * *Files identical despite different names*

### Comparing `giger-0.1.8/src/giger.egg-info/PKG-INFO` & `giger-0.1.9/src/giger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giger
-Version: 0.1.8
+Version: 0.1.9
 Summary: CLI for Stable Diffusion tasks.
 Home-page: https://github.com/artificialhoney/giger/
 Author: Sebastian Krüger
 Author-email: sk@honeymachine.io
 License: MIT
 Project-URL: Documentation, https://artificialhoney.github.io/giger/
 Project-URL: Source, https://github.com/artificialhoney/giger/
@@ -50,15 +50,15 @@
 
    pip install giger
 
 -----
 Usage
 -----
 
-Please check first of all the help function and the `examples <https://github.com/artificialhoney/giger/tree/main/examples/scripts/>`_.
+Please check first of all the help function and the `examples <https://github.com/artificialhoney/giger/tree/main/examples/>`_.
 
 .. code-block:: bash
 
     giger --help
 
 Also make sure to always obtain the latest version.
```

### Comparing `giger-0.1.8/src/giger.egg-info/SOURCES.txt` & `giger-0.1.9/src/giger.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -24,31 +24,39 @@
 docs/index.rst
 docs/license.rst
 docs/readme.rst
 docs/requirements.txt
 docs/_static/.gitignore
 docs/_static/styles/custom.css
 docs/_templates/page.html
+examples/assets/fonts/AnotherTag.ttf
+examples/assets/fonts/Marsneveneksk.ttf
+examples/assets/fonts/MostWasted.ttf
 examples/assets/img/faces/johann.jpg
 examples/assets/img/faces/kevin.jpg
 examples/assets/img/faces/leif.jpg
 examples/assets/img/faces/palina.jpg
 examples/assets/img/faces/peter.jpg
 examples/assets/img/faces/zakk.jpg
 examples/assets/img/sketches/honeymachine.png
 examples/assets/img/sketches/zonk.png
 examples/assets/img/sketches/zuri.png
 examples/assets/txt/prompts/_negative.txt
 examples/assets/txt/prompts/graffiti.txt
 examples/assets/txt/prompts/gravedigger.txt
 examples/assets/txt/prompts/spawn.txt
-examples/assets/txt/prompts/vampire.txt
 examples/assets/txt/prompts/viking.txt
-examples/scripts/batch/images.sh
-examples/scripts/batch/roop.sh
+examples/assets/txt/prompts/vampire/ancient.txt
+examples/assets/txt/prompts/vampire/modern.txt
+examples/batch/README.rst
+examples/batch/batch.py
+examples/batch/requirements.txt
+examples/graffiti/README.rst
+examples/graffiti/app.py
+examples/graffiti/requirements.txt
 requirements/test.txt
 src/giger/__init__.py
 src/giger/cli.py
 src/giger.egg-info/PKG-INFO
 src/giger.egg-info/SOURCES.txt
 src/giger.egg-info/dependency_links.txt
 src/giger.egg-info/entry_points.txt
```

### Comparing `giger-0.1.8/tests/commands/test_image_command.py` & `giger-0.1.9/tests/commands/test_image_command.py`

 * *Files identical despite different names*

### Comparing `giger-0.1.8/tests/commands/test_prompt_command.py` & `giger-0.1.9/tests/commands/test_prompt_command.py`

 * *Files identical despite different names*

### Comparing `giger-0.1.8/tests/commands/test_roop_command.py` & `giger-0.1.9/tests/commands/test_roop_command.py`

 * *Files identical despite different names*

### Comparing `giger-0.1.8/tests/commands/test_template_command.py` & `giger-0.1.9/tests/commands/test_template_command.py`

 * *Files identical despite different names*

### Comparing `giger-0.1.8/tests/fixtures/face.jpg` & `giger-0.1.9/tests/fixtures/face.jpg`

 * *Files identical despite different names*

### Comparing `giger-0.1.8/tests/fixtures/fail.jpg` & `giger-0.1.9/tests/fixtures/fail.jpg`

 * *Files identical despite different names*

### Comparing `giger-0.1.8/tests/fixtures/input.jpg` & `giger-0.1.9/tests/fixtures/input.jpg`

 * *Files identical despite different names*

### Comparing `giger-0.1.8/tests/services/test_image_service.py` & `giger-0.1.9/tests/services/test_image_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                 "prompt": "A viking with long hair and sword",
                 "negative_prompt": None,
                 "output": tmp_dir,
                 "width": 512,
                 "height": 512,
                 "loras": [{"model": "model", "filename": "filename", "scale": 1.0}],
             },
-            True,
+            False,
         )
     ]
 
     from_pretrained = StableDiffusionPipeline.from_pretrained
     StableDiffusionPipeline.from_pretrained = MagicMock()
     pipeline_mock = MagicMock()
     pipeline_mock.to = MagicMock()
@@ -152,15 +152,15 @@
         "controlnet_model": "test",
         "controlnet_conditioning_scale": 1,
         "control_guidance_start": 1,
         "control_guidance_end": 1,
         "input": input,
     }
 
-    fixtures = [("basic", data, False), ("cuda", data, True)]
+    fixtures = [("basic", data, False)]
 
     from_pretrained = StableDiffusionControlNetPipeline.from_pretrained
     StableDiffusionControlNetPipeline.from_pretrained = MagicMock()
     pipeline_mock = MagicMock()
     pipeline_mock.to = MagicMock()
     pipeline_mock.enable_model_cpu_offload = MagicMock()
     pipeline_mock.enable_xformers_memory_efficient_attention = MagicMock()
```

### Comparing `giger-0.1.8/tests/services/test_prompt_service.py` & `giger-0.1.9/tests/services/test_prompt_service.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         "artist": ["Artist"],
         "realism": ["Realism"],
         "rendering_engine": ["RenderingEngine"],
         "lightning_angle": ["LightningAngle"],
         "lightning_style": ["LightningStyle"],
         "camera_position": ["CameraPosition"],
         "camera": ["Camera"],
+        "camera_style": ["Infrared"],
         "composition": ["Composition"],
         "iso": "Iso",
         "resolution": ["Resolution"],
     }
     fixtures = [
         (
             "basic",
```

### Comparing `giger-0.1.8/tests/services/test_roop_service.py` & `giger-0.1.9/tests/services/test_roop_service.py`

 * *Files identical despite different names*

### Comparing `giger-0.1.8/tests/test_cli.py` & `giger-0.1.9/tests/test_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,22 +16,29 @@
 __copyright__ = "Sebastian Krüger"
 __license__ = "MIT"
 
 
 def test_loglevel():
     """CLI Loglevel Tests"""
     fixtures = [(logging.INFO, "-v"), (logging.DEBUG, "-vv")]
-    execute = TemplateCommand.execute
-    TemplateCommand.execute = MagicMock()
+    execute = ImageCommand.execute
+    ImageCommand.execute = MagicMock()
 
     for loglevel, fixture in fixtures:
-        sys.argv = ["giger", fixture, "template"]
+        sys.argv = [
+            "giger",
+            fixture,
+            "image",
+            "A viking with long hair and sword",
+            "--output",
+            "viking",
+        ]
         run()
         assert logging.get_verbosity() == loglevel
-    TemplateCommand.execute = execute
+    ImageCommand.execute = execute
 
 
 def test_template(snapshot):
     """CLI Template Tests"""
     snapshots_dir = os.path.join(
         os.path.dirname(__file__), "snapshots", "cli", "template"
     )
```

### Comparing `giger-0.1.8/tox.ini` & `giger-0.1.9/tox.ini`

 * *Files identical despite different names*

