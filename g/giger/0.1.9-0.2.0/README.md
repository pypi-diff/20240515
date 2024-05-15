# Comparing `tmp/giger-0.1.9.tar.gz` & `tmp/giger-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giger-0.1.9.tar", last modified: Sat Aug 19 16:08:33 2023, max compression
+gzip compressed data, was "giger-0.2.0.tar", last modified: Wed May 15 11:28:51 2024, max compression
```

## Comparing `giger-0.1.9.tar` & `giger-0.2.0.tar`

### file list

```diff
@@ -1,165 +1,147 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.127545 giger-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-19 16:02:08.000000 giger-0.1.9/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)     9504 2023-08-19 16:02:08.000000 giger-0.1.9/.gitchangelog.rc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.071545 giger-0.1.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.095545 giger-0.1.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-08-19 16:02:08.000000 giger-0.1.9/.github/workflows/documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-08-19 16:02:08.000000 giger-0.1.9/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-08-19 16:02:08.000000 giger-0.1.9/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-19 16:02:08.000000 giger-0.1.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-08-19 16:02:08.000000 giger-0.1.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-19 16:02:08.000000 giger-0.1.9/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-19 16:02:08.000000 giger-0.1.9/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-08-19 16:02:08.000000 giger-0.1.9/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11630 2023-08-19 16:02:08.000000 giger-0.1.9/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-19 16:02:08.000000 giger-0.1.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-19 16:02:08.000000 giger-0.1.9/Manifest.in
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-08-19 16:08:33.127545 giger-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-08-19 16:02:08.000000 giger-0.1.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.099545 giger-0.1.9/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-19 16:02:08.000000 giger-0.1.9/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.099545 giger-0.1.9/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-19 16:02:08.000000 giger-0.1.9/docs/_static/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.099545 giger-0.1.9/docs/_static/styles/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-08-19 16:02:08.000000 giger-0.1.9/docs/_static/styles/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.099545 giger-0.1.9/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-08-19 16:02:08.000000 giger-0.1.9/docs/_templates/page.html
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-19 16:02:08.000000 giger-0.1.9/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-19 16:02:08.000000 giger-0.1.9/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-08-19 16:02:08.000000 giger-0.1.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-19 16:02:08.000000 giger-0.1.9/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-08-19 16:02:08.000000 giger-0.1.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-19 16:02:08.000000 giger-0.1.9/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-19 16:02:08.000000 giger-0.1.9/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-19 16:02:08.000000 giger-0.1.9/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.075544 giger-0.1.9/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.075544 giger-0.1.9/examples/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.103545 giger-0.1.9/examples/assets/fonts/
--rwxr-xr-x   0 runner    (1001) docker     (123)    24224 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/fonts/AnotherTag.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    38692 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/fonts/Marsneveneksk.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)    45888 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/fonts/MostWasted.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.075544 giger-0.1.9/examples/assets/img/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.107545 giger-0.1.9/examples/assets/img/faces/
--rw-r--r--   0 runner    (1001) docker     (123)   436995 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/img/faces/johann.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    89758 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/img/faces/kevin.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    41504 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/img/faces/leif.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    34171 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/img/faces/palina.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   119989 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/img/faces/peter.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   151489 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/img/faces/zakk.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.111545 giger-0.1.9/examples/assets/img/sketches/
--rw-r--r--   0 runner    (1001) docker     (123)    64768 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/img/sketches/honeymachine.png
--rw-r--r--   0 runner    (1001) docker     (123)    20067 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/img/sketches/zonk.png
--rw-r--r--   0 runner    (1001) docker     (123)    27881 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/img/sketches/zuri.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.075544 giger-0.1.9/examples/assets/txt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.115545 giger-0.1.9/examples/assets/txt/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/txt/prompts/_negative.txt
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/txt/prompts/graffiti.txt
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/txt/prompts/gravedigger.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/txt/prompts/spawn.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.115545 giger-0.1.9/examples/assets/txt/prompts/vampire/
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/txt/prompts/vampire/ancient.txt
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/txt/prompts/vampire/modern.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-19 16:02:08.000000 giger-0.1.9/examples/assets/txt/prompts/viking.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.115545 giger-0.1.9/examples/batch/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-08-19 16:02:08.000000 giger-0.1.9/examples/batch/README.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     5660 2023-08-19 16:02:08.000000 giger-0.1.9/examples/batch/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-19 16:02:08.000000 giger-0.1.9/examples/batch/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.115545 giger-0.1.9/examples/graffiti/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-08-19 16:02:08.000000 giger-0.1.9/examples/graffiti/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-08-19 16:02:08.000000 giger-0.1.9/examples/graffiti/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-19 16:02:08.000000 giger-0.1.9/examples/graffiti/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-08-19 16:02:08.000000 giger-0.1.9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.115545 giger-0.1.9/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-19 16:02:08.000000 giger-0.1.9/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-08-19 16:08:33.127545 giger-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-08-19 16:02:08.000000 giger-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.079544 giger-0.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.115545 giger-0.1.9/src/giger/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-08-19 16:02:08.000000 giger-0.1.9/src/giger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-08-19 16:02:08.000000 giger-0.1.9/src/giger/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.119545 giger-0.1.9/src/giger/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-08-19 16:02:08.000000 giger-0.1.9/src/giger/commands/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-08-19 16:02:08.000000 giger-0.1.9/src/giger/commands/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-08-19 16:02:08.000000 giger-0.1.9/src/giger/commands/roop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-08-19 16:02:08.000000 giger-0.1.9/src/giger/commands/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.119545 giger-0.1.9/src/giger/services/
--rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-08-19 16:02:08.000000 giger-0.1.9/src/giger/services/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    13400 2023-08-19 16:02:08.000000 giger-0.1.9/src/giger/services/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-08-19 16:02:08.000000 giger-0.1.9/src/giger/services/roop.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-08-19 16:02:08.000000 giger-0.1.9/src/giger/services/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.119545 giger-0.1.9/src/giger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-08-19 16:08:33.000000 giger-0.1.9/src/giger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-08-19 16:08:33.000000 giger-0.1.9/src/giger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-19 16:08:33.000000 giger-0.1.9/src/giger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-19 16:08:33.000000 giger-0.1.9/src/giger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-19 16:02:18.000000 giger-0.1.9/src/giger.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-19 16:08:33.000000 giger-0.1.9/src/giger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-19 16:08:33.000000 giger-0.1.9/src/giger.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.119545 giger-0.1.9/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.119545 giger-0.1.9/tests/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-08-19 16:02:08.000000 giger-0.1.9/tests/commands/test_image_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-08-19 16:02:08.000000 giger-0.1.9/tests/commands/test_prompt_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-08-19 16:02:08.000000 giger-0.1.9/tests/commands/test_roop_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-08-19 16:02:08.000000 giger-0.1.9/tests/commands/test_template_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-19 16:02:08.000000 giger-0.1.9/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.119545 giger-0.1.9/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)    11793 2023-08-19 16:02:08.000000 giger-0.1.9/tests/fixtures/face.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    30558 2023-08-19 16:02:08.000000 giger-0.1.9/tests/fixtures/fail.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-19 16:02:08.000000 giger-0.1.9/tests/fixtures/hero.yml
--rw-r--r--   0 runner    (1001) docker     (123)    42528 2023-08-19 16:02:08.000000 giger-0.1.9/tests/fixtures/input.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.119545 giger-0.1.9/tests/services/
--rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-08-19 16:02:08.000000 giger-0.1.9/tests/services/test_image_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-08-19 16:02:08.000000 giger-0.1.9/tests/services/test_prompt_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-08-19 16:02:08.000000 giger-0.1.9/tests/services/test_roop_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-08-19 16:02:08.000000 giger-0.1.9/tests/services/test_template_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.083545 giger-0.1.9/tests/snapshots/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.083545 giger-0.1.9/tests/snapshots/cli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.123545 giger-0.1.9/tests/snapshots/cli/image/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/cli/image/basic.yml.snapshot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.123545 giger-0.1.9/tests/snapshots/cli/prompt/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/cli/prompt/basic.yml.snapshot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.123545 giger-0.1.9/tests/snapshots/cli/roop/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/cli/roop/basic.yml.snapshot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.123545 giger-0.1.9/tests/snapshots/cli/template/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/cli/template/basic.yml.snapshot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.083545 giger-0.1.9/tests/snapshots/commands/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.083545 giger-0.1.9/tests/snapshots/commands/image/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.123545 giger-0.1.9/tests/snapshots/commands/image/controlnet/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/commands/image/controlnet/basic.yml.snapshot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.123545 giger-0.1.9/tests/snapshots/commands/image/img2img/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/commands/image/img2img/basic.yml.snapshot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.123545 giger-0.1.9/tests/snapshots/commands/image/txt2img/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/commands/image/txt2img/basic.yml.snapshot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.123545 giger-0.1.9/tests/snapshots/commands/prompt/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/commands/prompt/basic.yml.snapshot
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/commands/prompt/output.yml.snapshot
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/commands/prompt/stdin.yml.snapshot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.123545 giger-0.1.9/tests/snapshots/commands/roop/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/commands/roop/basic.yml.snapshot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.123545 giger-0.1.9/tests/snapshots/commands/template/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/commands/template/basic.yml.snapshot
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/commands/template/data.yml.snapshot
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/commands/template/output.yml.snapshot
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/commands/template/stdin.yml.snapshot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.087545 giger-0.1.9/tests/snapshots/services/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.087545 giger-0.1.9/tests/snapshots/services/image/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.123545 giger-0.1.9/tests/snapshots/services/image/controlnet/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/services/image/controlnet/basic.from_pretrained.yml.snapshot
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/services/image/controlnet/basic.pipeline.yml.snapshot
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/services/image/controlnet/cuda.from_pretrained.yml.snapshot
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/services/image/controlnet/cuda.pipeline.yml.snapshot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.123545 giger-0.1.9/tests/snapshots/services/image/img2img/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/services/image/img2img/basic.from_pretrained.yml.snapshot
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/services/image/img2img/basic.pipeline.yml.snapshot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.123545 giger-0.1.9/tests/snapshots/services/image/txt2img/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/services/image/txt2img/basic.from_pretrained.yml.snapshot
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/services/image/txt2img/basic.pipeline.yml.snapshot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 16:08:33.127545 giger-0.1.9/tests/snapshots/services/prompt/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/services/prompt/advanced.txt.snapshot
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/services/prompt/basic.txt.snapshot
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/services/prompt/compel_full.txt.snapshot
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/services/prompt/compel_full_full.txt.snapshot
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/services/prompt/compel_subtle.txt.snapshot
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-19 16:02:08.000000 giger-0.1.9/tests/snapshots/services/prompt/compel_subtle_empty.txt.snapshot
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-08-19 16:02:08.000000 giger-0.1.9/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-08-19 16:02:08.000000 giger-0.1.9/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.532621 giger-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-15 11:28:43.000000 giger-0.2.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-05-15 11:28:43.000000 giger-0.2.0/.gitchangelog.rc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.508620 giger-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.516620 giger-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-15 11:28:43.000000 giger-0.2.0/.github/workflows/documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-15 11:28:43.000000 giger-0.2.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-15 11:28:43.000000 giger-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-15 11:28:43.000000 giger-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-15 11:28:43.000000 giger-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-15 11:28:43.000000 giger-0.2.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-15 11:28:43.000000 giger-0.2.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-05-15 11:28:43.000000 giger-0.2.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11630 2024-05-15 11:28:43.000000 giger-0.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-15 11:28:43.000000 giger-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-15 11:28:43.000000 giger-0.2.0/Manifest.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-05-15 11:28:51.532621 giger-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-15 11:28:43.000000 giger-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.516620 giger-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-15 11:28:43.000000 giger-0.2.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.516620 giger-0.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 11:28:43.000000 giger-0.2.0/docs/_static/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.516620 giger-0.2.0/docs/_static/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-15 11:28:43.000000 giger-0.2.0/docs/_static/styles/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.520620 giger-0.2.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-05-15 11:28:43.000000 giger-0.2.0/docs/_templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-15 11:28:43.000000 giger-0.2.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-15 11:28:43.000000 giger-0.2.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11722 2024-05-15 11:28:43.000000 giger-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-15 11:28:43.000000 giger-0.2.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-15 11:28:43.000000 giger-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-15 11:28:43.000000 giger-0.2.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-15 11:28:43.000000 giger-0.2.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-15 11:28:43.000000 giger-0.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.508620 giger-0.2.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.520620 giger-0.2.0/examples/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-15 11:28:43.000000 giger-0.2.0/examples/batch/README.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6010 2024-05-15 11:28:43.000000 giger-0.2.0/examples/batch/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 11:28:43.000000 giger-0.2.0/examples/batch/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.520620 giger-0.2.0/examples/graffiti/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-15 11:28:43.000000 giger-0.2.0/examples/graffiti/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-05-15 11:28:43.000000 giger-0.2.0/examples/graffiti/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.520620 giger-0.2.0/examples/graffiti/fonts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24224 2024-05-15 11:28:43.000000 giger-0.2.0/examples/graffiti/fonts/AnotherTag.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    38692 2024-05-15 11:28:43.000000 giger-0.2.0/examples/graffiti/fonts/Marsneveneksk.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (127)    45888 2024-05-15 11:28:43.000000 giger-0.2.0/examples/graffiti/fonts/MostWasted.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-15 11:28:43.000000 giger-0.2.0/examples/graffiti/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.520620 giger-0.2.0/examples/styled/
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 11:28:43.000000 giger-0.2.0/examples/styled/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10149 2024-05-15 11:28:43.000000 giger-0.2.0/examples/styled/styled.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-15 11:28:43.000000 giger-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.520620 giger-0.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-15 11:28:43.000000 giger-0.2.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-15 11:28:51.532621 giger-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-15 11:28:43.000000 giger-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.508620 giger-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.520620 giger-0.2.0/src/giger/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-15 11:28:43.000000 giger-0.2.0/src/giger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-15 11:28:43.000000 giger-0.2.0/src/giger/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.524621 giger-0.2.0/src/giger/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-05-15 11:28:43.000000 giger-0.2.0/src/giger/commands/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-15 11:28:43.000000 giger-0.2.0/src/giger/commands/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-15 11:28:43.000000 giger-0.2.0/src/giger/commands/roop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-15 11:28:43.000000 giger-0.2.0/src/giger/commands/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-15 11:28:43.000000 giger-0.2.0/src/giger/commands/upscale.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.524621 giger-0.2.0/src/giger/services/
+-rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-05-15 11:28:43.000000 giger-0.2.0/src/giger/services/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14480 2024-05-15 11:28:43.000000 giger-0.2.0/src/giger/services/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-15 11:28:43.000000 giger-0.2.0/src/giger/services/roop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-15 11:28:43.000000 giger-0.2.0/src/giger/services/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-15 11:28:43.000000 giger-0.2.0/src/giger/services/upscale.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.532621 giger-0.2.0/src/giger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-05-15 11:28:51.000000 giger-0.2.0/src/giger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-15 11:28:51.000000 giger-0.2.0/src/giger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 11:28:51.000000 giger-0.2.0/src/giger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-15 11:28:51.000000 giger-0.2.0/src/giger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 11:28:51.000000 giger-0.2.0/src/giger.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-15 11:28:51.000000 giger-0.2.0/src/giger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 11:28:51.000000 giger-0.2.0/src/giger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.524621 giger-0.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.524621 giger-0.2.0/tests/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-05-15 11:28:43.000000 giger-0.2.0/tests/commands/test_image_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-15 11:28:43.000000 giger-0.2.0/tests/commands/test_prompt_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-15 11:28:43.000000 giger-0.2.0/tests/commands/test_roop_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-15 11:28:43.000000 giger-0.2.0/tests/commands/test_template_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-15 11:28:43.000000 giger-0.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.524621 giger-0.2.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)    11793 2024-05-15 11:28:43.000000 giger-0.2.0/tests/fixtures/face.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    30558 2024-05-15 11:28:43.000000 giger-0.2.0/tests/fixtures/fail.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-15 11:28:43.000000 giger-0.2.0/tests/fixtures/hero.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    42528 2024-05-15 11:28:43.000000 giger-0.2.0/tests/fixtures/input.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.524621 giger-0.2.0/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-05-15 11:28:43.000000 giger-0.2.0/tests/services/test_image_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-15 11:28:43.000000 giger-0.2.0/tests/services/test_prompt_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-15 11:28:43.000000 giger-0.2.0/tests/services/test_roop_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-15 11:28:43.000000 giger-0.2.0/tests/services/test_template_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.512620 giger-0.2.0/tests/snapshots/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.512620 giger-0.2.0/tests/snapshots/cli/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.524621 giger-0.2.0/tests/snapshots/cli/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-15 11:28:43.000000 giger-0.2.0/tests/snapshots/cli/image/basic.yml.snapshot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.524621 giger-0.2.0/tests/snapshots/cli/prompt/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-15 11:28:43.000000 giger-0.2.0/tests/snapshots/cli/prompt/basic.yml.snapshot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.524621 giger-0.2.0/tests/snapshots/cli/roop/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-15 11:28:43.000000 giger-0.2.0/tests/snapshots/cli/roop/basic.yml.snapshot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.528621 giger-0.2.0/tests/snapshots/cli/template/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-15 11:28:43.000000 giger-0.2.0/tests/snapshots/cli/template/basic.yml.snapshot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.512620 giger-0.2.0/tests/snapshots/commands/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.512620 giger-0.2.0/tests/snapshots/commands/image/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.528621 giger-0.2.0/tests/snapshots/commands/image/controlnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-15 11:28:43.000000 giger-0.2.0/tests/snapshots/commands/image/controlnet/basic.yml.snapshot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.528621 giger-0.2.0/tests/snapshots/commands/image/img2img/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-15 11:28:43.000000 giger-0.2.0/tests/snapshots/commands/image/img2img/basic.yml.snapshot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.528621 giger-0.2.0/tests/snapshots/commands/image/txt2img/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-15 11:28:43.000000 giger-0.2.0/tests/snapshots/commands/image/txt2img/basic.yml.snapshot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.528621 giger-0.2.0/tests/snapshots/commands/prompt/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 11:28:43.000000 giger-0.2.0/tests/snapshots/commands/prompt/basic.yml.snapshot
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 11:28:43.000000 giger-0.2.0/tests/snapshots/commands/prompt/output.yml.snapshot
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 11:28:43.000000 giger-0.2.0/tests/snapshots/commands/prompt/stdin.yml.snapshot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.528621 giger-0.2.0/tests/snapshots/commands/roop/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-15 11:28:43.000000 giger-0.2.0/tests/snapshots/commands/roop/basic.yml.snapshot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.528621 giger-0.2.0/tests/snapshots/commands/template/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-15 11:28:43.000000 giger-0.2.0/tests/snapshots/commands/template/basic.yml.snapshot
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-15 11:28:43.000000 giger-0.2.0/tests/snapshots/commands/template/data.yml.snapshot
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-15 11:28:43.000000 giger-0.2.0/tests/snapshots/commands/template/output.yml.snapshot
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-15 11:28:43.000000 giger-0.2.0/tests/snapshots/commands/template/stdin.yml.snapshot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.512620 giger-0.2.0/tests/snapshots/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.512620 giger-0.2.0/tests/snapshots/services/image/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.528621 giger-0.2.0/tests/snapshots/services/image/controlnet/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 11:28:43.000000 giger-0.2.0/tests/snapshots/services/image/controlnet/basic.from_pretrained.yml.snapshot
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 11:28:43.000000 giger-0.2.0/tests/snapshots/services/image/controlnet/basic.pipeline.yml.snapshot
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 11:28:43.000000 giger-0.2.0/tests/snapshots/services/image/controlnet/cuda.from_pretrained.yml.snapshot
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 11:28:43.000000 giger-0.2.0/tests/snapshots/services/image/controlnet/cuda.pipeline.yml.snapshot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.528621 giger-0.2.0/tests/snapshots/services/image/img2img/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 11:28:43.000000 giger-0.2.0/tests/snapshots/services/image/img2img/basic.from_pretrained.yml.snapshot
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 11:28:43.000000 giger-0.2.0/tests/snapshots/services/image/img2img/basic.pipeline.yml.snapshot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.528621 giger-0.2.0/tests/snapshots/services/image/txt2img/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 11:28:43.000000 giger-0.2.0/tests/snapshots/services/image/txt2img/basic.from_pretrained.yml.snapshot
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 11:28:43.000000 giger-0.2.0/tests/snapshots/services/image/txt2img/basic.pipeline.yml.snapshot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:28:51.532621 giger-0.2.0/tests/snapshots/services/prompt/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-15 11:28:43.000000 giger-0.2.0/tests/snapshots/services/prompt/advanced.txt.snapshot
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-15 11:28:43.000000 giger-0.2.0/tests/snapshots/services/prompt/basic.txt.snapshot
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-15 11:28:43.000000 giger-0.2.0/tests/snapshots/services/prompt/compel_full.txt.snapshot
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 11:28:43.000000 giger-0.2.0/tests/snapshots/services/prompt/compel_full_full.txt.snapshot
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-15 11:28:43.000000 giger-0.2.0/tests/snapshots/services/prompt/compel_subtle.txt.snapshot
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 11:28:43.000000 giger-0.2.0/tests/snapshots/services/prompt/compel_subtle_empty.txt.snapshot
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-05-15 11:28:43.000000 giger-0.2.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-15 11:28:43.000000 giger-0.2.0/tox.ini
```

### Comparing `giger-0.1.9/.coveragerc` & `giger-0.2.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `giger-0.1.9/.gitchangelog.rc` & `giger-0.2.0/.gitchangelog.rc`

 * *Files identical despite different names*

### Comparing `giger-0.1.9/.github/workflows/documentation.yml` & `giger-0.2.0/.github/workflows/documentation.yml`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
           fetch-depth: 0
       - name: Setup Pages
         uses: actions/configure-pages@v3
       - name: Setup Python
         uses: actions/setup-python@v3
       - name: Install dependencies
         run: |
-          pip install -r docs/requirements.txt && pip install -e .
+          pip install -r docs/requirements.txt
       - name: Sphinx build
         run: |
           make -C docs html
       - name: Upload artifact
         uses: actions/upload-pages-artifact@v2
         with:
           # Upload entire repository
```

### Comparing `giger-0.1.9/.github/workflows/test.yml` & `giger-0.2.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `giger-0.1.9/.gitignore` & `giger-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `giger-0.1.9/.pre-commit-config.yaml` & `giger-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `giger-0.1.9/.readthedocs.yml` & `giger-0.2.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `giger-0.1.9/CHANGELOG.rst` & `giger-0.2.0/CHANGELOG.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,37 @@
 Changelog
 =========
 
 
+0.1.10 (2023-08-21)
+-------------------
+
+Fix
+~~~
+- Inswapper repo. [Sebastian Krüger]
+- Prompt command and service args passing. [Sebastian Krüger]
+
+Changes
+~~~~~~~
+- Remove stable diffusion link. [Sebastian Krüger]
+- Batch tuple dimension fix. [Sebastian Krüger]
+
+
 0.1.9 (2023-08-19)
 ------------------
 
 Fix
 ~~~
 - Image seed generator cuda switch. [Sebastian Krüger]
 - Prompt camera style, improve startup time. [Sebastian Krüger]
 
 Changes
 ~~~~~~~
+- Publish workflow manual dispatch. [Sebastian Krüger]
+- CHANGELOG. [Sebastian Krüger]
 - Remove cuda from tests. [Sebastian Krüger]
 - Fix batch seed. [Sebastian Krüger]
 - Fix batch. [Sebastian Krüger]
 - Bash batch scripts to python. [Sebastian Krüger]
 - Remove docs hint. [Sebastian Krüger]
 - Pre-commit conventional-commit. [Sebastian Krüger]
 - Graffiti example with streamlit. [Sebastian Krüger]
```

### Comparing `giger-0.1.9/CONTRIBUTING.rst` & `giger-0.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `giger-0.1.9/LICENSE.txt` & `giger-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `giger-0.1.9/PKG-INFO` & `giger-0.2.0/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: giger
-Version: 0.1.9
-Summary: CLI for Stable Diffusion tasks.
-Home-page: https://github.com/artificialhoney/giger/
-Author: Sebastian Krüger
-Author-email: sk@honeymachine.io
-License: MIT
-Project-URL: Documentation, https://artificialhoney.github.io/giger/
-Project-URL: Source, https://github.com/artificialhoney/giger/
-Project-URL: Tracker, https://github.com/artificialhoney/giger/issues
-Project-URL: Download, https://pypi.org/project/giger/#files
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Description-Content-Type: text/x-rst; charset=UTF-8
-Provides-Extra: testing
-License-File: LICENSE.txt
-
 =====
 giger
 =====
 
 .. image:: https://img.shields.io/pypi/v/giger.svg
     :alt: PyPI-Server
     :target: https://pypi.org/project/giger/
@@ -38,14 +19,16 @@
     :target: https://opensource.org/licenses/MIT
 .. image:: https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold
     :alt: Project generated with PyScaffold
     :target: https://pyscaffold.org/
 
 CLI for Stable Diffusion tasks.
 
+Read more: `https://artificialhoney.github.io/giger <https://artificialhoney.github.io/giger>`_
+
 ------------
 Installation
 ------------
 
 .. code:: bash
 
    pip install giger
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `giger-0.1.9/docs/Makefile` & `giger-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `giger-0.1.9/docs/_templates/page.html` & `giger-0.2.0/docs/_templates/page.html`

 * *Files 16% similar despite different names*

```diff
@@ -54,292 +54,268 @@
 00000350: 7b25 2d20 656e 6469 6620 257d 0a3c 2f64  {%- endif %}.</d
 00000360: 6976 3e0a 3c64 6976 2063 6c61 7373 3d22  iv>.<div class="
 00000370: 626f 7474 6f6d 2d6f 662d 7061 6765 223e  bottom-of-page">
 00000380: 0a20 203c 6469 7620 636c 6173 733d 226c  .  <div class="l
 00000390: 6566 742d 6465 7461 696c 7322 3e0a 2020  eft-details">.  
 000003a0: 2020 7b25 2d20 6966 2073 686f 775f 636f    {%- if show_co
 000003b0: 7079 7269 6768 7420 257d 0a20 2020 203c  pyright %}.    <
-000003c0: 6469 7620 636c 6173 733d 2263 6f70 7972  div class="copyr
-000003d0: 6967 6874 223e 0a20 2020 2020 207b 2520  ight">.      {% 
-000003e0: 7472 616e 7320 6c61 7374 5f75 7064 6174  trans last_updat
-000003f0: 6564 3d6c 6173 745f 7570 6461 7465 647c  ed=last_updated|
-00000400: 6520 2d25 7d20 7b7b 206c 6173 745f 7570  e -%} {{ last_up
-00000410: 6461 7465 6420 7d7d 266e 6273 703b 207b  dated }}&nbsp; {
-00000420: 252d 0a20 2020 2020 2065 6e64 7472 616e  %-.      endtran
-00000430: 7320 2d25 7dc2 a90a 2020 2020 2020 3c61  s -%}...      <a
-00000440: 2068 7265 663d 222f 223e 2048 6f6e 6579   href="/"> Honey
-00000450: 6d61 6368 696e 6520 3c2f 613e 2e20 4372  machine </a>. Cr
-00000460: 6561 7465 6420 7769 7468 20f0 9f8c b8ef  eated with .....
-00000470: b88f 2062 7920 5365 6261 7374 6961 6e2e  .. by Sebastian.
-00000480: 0a20 2020 2020 203c 6120 6872 6566 3d22  .      <a href="
-00000490: 6874 7470 733a 2f2f 7878 2e68 6f6e 6579  https://xx.honey
-000004a0: 6d61 6368 696e 652e 696f 223e 5858 3c2f  machine.io">XX</
-000004b0: 613e 0a20 2020 2020 207c 0a20 2020 2020  a>.      |.     
-000004c0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-000004d0: 2f2f 6172 7469 6669 6369 616c 686f 6e65  //artificialhone
-000004e0: 792e 6769 7468 7562 2e69 6f2f 7374 6162  y.github.io/stab
-000004f0: 6c65 2d64 6966 6675 7369 6f6e 220a 2020  le-diffusion".  
-00000500: 2020 2020 2020 3e53 7461 626c 6520 4469        >Stable Di
-00000510: 6666 7573 696f 6e3c 2f61 0a20 2020 2020  ffusion</a.     
-00000520: 203e 0a20 2020 2020 207c 0a20 2020 2020   >.      |.     
-00000530: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-00000540: 2f2f 6172 7469 6669 6369 616c 686f 6e65  //artificialhone
-00000550: 792e 6769 7468 7562 2e69 6f2f 6769 6765  y.github.io/gige
-00000560: 7222 3e47 6967 6572 3c2f 613e 0a20 2020  r">Giger</a>.   
-00000570: 2020 207c 0a20 2020 2020 203c 6120 6872     |.      <a hr
-00000580: 6566 3d22 6874 7470 733a 2f2f 6172 7469  ef="https://arti
-00000590: 6669 6369 616c 686f 6e65 792e 6769 7468  ficialhoney.gith
-000005a0: 7562 2e69 6f2f 616d 6978 223e 416d 6978  ub.io/amix">Amix
-000005b0: 3c2f 613e 0a20 2020 203c 2f64 6976 3e0a  </a>.    </div>.
-000005c0: 2020 2020 7b25 2d20 656e 6469 6620 257d      {%- endif %}
-000005d0: 0a20 203c 2f64 6976 3e0a 2020 3c64 6976  .  </div>.  <div
-000005e0: 2063 6c61 7373 3d22 7269 6768 742d 6465   class="right-de
-000005f0: 7461 696c 7322 3e0a 2020 2020 7b25 2069  tails">.    {% i
-00000600: 6620 7468 656d 655f 666f 6f74 6572 5f69  f theme_footer_i
-00000610: 636f 6e73 206f 7220 5245 4144 5448 4544  cons or READTHED
-00000620: 4f43 5320 2d25 7d0a 2020 2020 3c64 6976  OCS -%}.    <div
-00000630: 2063 6c61 7373 3d22 6963 6f6e 7322 3e0a   class="icons">.
-00000640: 2020 2020 2020 7b25 2069 6620 7468 656d        {% if them
-00000650: 655f 666f 6f74 6572 5f69 636f 6e73 202d  e_footer_icons -
-00000660: 257d 207b 2520 666f 7220 6963 6f6e 5f64  %} {% for icon_d
-00000670: 6963 7420 696e 2074 6865 6d65 5f66 6f6f  ict in theme_foo
-00000680: 7465 725f 6963 6f6e 7320 2d25 7d0a 2020  ter_icons -%}.  
-00000690: 2020 2020 3c61 0a20 2020 2020 2020 2063      <a.        c
-000006a0: 6c61 7373 3d22 6d75 7465 642d 6c69 6e6b  lass="muted-link
-000006b0: 207b 7b20 6963 6f6e 5f64 6963 742e 636c   {{ icon_dict.cl
-000006c0: 6173 7320 7d7d 220a 2020 2020 2020 2020  ass }}".        
-000006d0: 6872 6566 3d22 7b7b 2069 636f 6e5f 6469  href="{{ icon_di
-000006e0: 6374 2e75 726c 207d 7d22 0a20 2020 2020  ct.url }}".     
-000006f0: 2020 2061 7269 612d 6c61 6265 6c3d 227b     aria-label="{
-00000700: 7b20 6963 6f6e 5f64 6963 742e 6e61 6d65  { icon_dict.name
-00000710: 207d 7d22 0a20 2020 2020 203e 0a20 2020   }}".      >.   
-00000720: 2020 2020 207b 7b2d 2069 636f 6e5f 6469       {{- icon_di
-00000730: 6374 2e68 746d 6c20 2d7d 7d0a 2020 2020  ct.html -}}.    
-00000740: 2020 3c2f 613e 0a20 2020 2020 207b 2520    </a>.      {% 
-00000750: 656e 6466 6f72 2025 7d20 7b25 2d20 656c  endfor %} {%- el
-00000760: 7365 202d 257d 207b 232d 2053 686f 7720  se -%} {#- Show 
-00000770: 5265 6164 2074 6865 2044 6f63 7320 7072  Read the Docs pr
-00000780: 6f6a 6563 7420 2d23 7d20 7b25 2d20 6966  oject -#} {%- if
-00000790: 0a20 2020 2020 2052 4541 4454 4845 444f  .      READTHEDO
-000007a0: 4353 2061 6e64 2073 6c75 6720 2d25 7d0a  CS and slug -%}.
-000007b0: 2020 2020 2020 3c61 0a20 2020 2020 2020        <a.       
-000007c0: 2063 6c61 7373 3d22 6d75 7465 642d 6c69   class="muted-li
-000007d0: 6e6b 220a 2020 2020 2020 2020 6872 6566  nk".        href
-000007e0: 3d22 6874 7470 733a 2f2f 7265 6164 7468  ="https://readth
-000007f0: 6564 6f63 732e 6f72 672f 7072 6f6a 6563  edocs.org/projec
-00000800: 7473 2f7b 7b20 736c 7567 207d 7d22 0a20  ts/{{ slug }}". 
-00000810: 2020 2020 2020 2061 7269 612d 6c61 6265         aria-labe
-00000820: 6c3d 224f 6e20 5265 6164 2074 6865 2044  l="On Read the D
-00000830: 6f63 7322 0a20 2020 2020 203e 0a20 2020  ocs".      >.   
-00000840: 2020 2020 203c 7376 6720 783d 2230 7078       <svg x="0px
-00000850: 2220 793d 2230 7078 2220 7669 6577 426f  " y="0px" viewBo
-00000860: 783d 222d 3132 3520 3231 3720 3336 3020  x="-125 217 360 
-00000870: 3336 3022 2078 6d6c 3a73 7061 6365 3d22  360" xml:space="
-00000880: 7072 6573 6572 7665 223e 0a20 2020 2020  preserve">.     
-00000890: 2020 2020 203c 7061 7468 0a20 2020 2020       <path.     
-000008a0: 2020 2020 2020 2066 696c 6c3d 2263 7572         fill="cur
-000008b0: 7265 6e74 436f 6c6f 7222 0a20 2020 2020  rentColor".     
-000008c0: 2020 2020 2020 2064 3d22 4d33 392e 322c         d="M39.2,
-000008d0: 3339 312e 3363 2d34 2e32 2c30 2e36 2d37  391.3c-4.2,0.6-7
-000008e0: 2e31 2c34 2e34 2d36 2e35 2c38 2e35 6330  .1,4.4-6.5,8.5c0
-000008f0: 2e34 2c33 2c32 2e36 2c35 2e35 2c35 2e35  .4,3,2.6,5.5,5.5
-00000900: 2c36 2e33 2063 302c 302c 3138 2e35 2c36  ,6.3 c0,0,18.5,6
-00000910: 2e31 2c35 302c 382e 3763 3235 2e33 2c32  .1,50,8.7c25.3,2
-00000920: 2e31 2c35 342d 312e 382c 3534 2d31 2e38  .1,54-1.8,54-1.8
-00000930: 6334 2e32 2d30 2e31 2c37 2e35 2d33 2e36  c4.2-0.1,7.5-3.6
-00000940: 2c37 2e34 2d37 2e38 632d 302e 312d 342e  ,7.4-7.8c-0.1-4.
-00000950: 322d 332e 362d 372e 352d 372e 382d 372e  2-3.6-7.5-7.8-7.
-00000960: 3463 2d30 2e35 2c30 2d31 2c30 2e31 2d31  4c-0.5,0-1,0.1-1
-00000970: 2e35 2c30 2e32 2063 302c 302d 3238 2e31  .5,0.2 c0,0-28.1
-00000980: 2c33 2e35 2d35 302e 392c 312e 3663 2d33  ,3.5-50.9,1.6c-3
-00000990: 302e 312d 322e 342d 3436 2e35 2d37 2e39  0.1-2.4-46.5-7.9
-000009a0: 2d34 362e 352d 372e 3943 3431 2e37 2c33  -46.5-7.9C41.7,3
-000009b0: 3931 2e33 2c34 302e 342c 3339 312e 312c  91.3,40.4,391.1,
-000009c0: 3339 2e32 2c33 3931 2e33 7a20 4d33 392e  39.2,391.3z M39.
-000009d0: 322c 3335 332e 3663 2d34 2e32 2c30 2e36  2,353.6c-4.2,0.6
-000009e0: 2d37 2e31 2c34 2e34 2d36 2e35 2c38 2e35  -7.1,4.4-6.5,8.5
-000009f0: 2063 302e 342c 332c 322e 362c 352e 352c   c0.4,3,2.6,5.5,
-00000a00: 352e 352c 362e 3363 302c 302c 3138 2e35  5.5,6.3c0,0,18.5
-00000a10: 2c36 2e31 2c35 302c 382e 3763 3235 2e33  ,6.1,50,8.7c25.3
-00000a20: 2c32 2e31 2c35 342d 312e 382c 3534 2d31  ,2.1,54-1.8,54-1
-00000a30: 2e38 6334 2e32 2d30 2e31 2c37 2e35 2d33  .8c4.2-0.1,7.5-3
-00000a40: 2e36 2c37 2e34 2d37 2e38 632d 302e 312d  .6,7.4-7.8c-0.1-
-00000a50: 342e 322d 332e 362d 372e 352d 372e 382d  4.2-3.6-7.5-7.8-
-00000a60: 372e 3420 632d 302e 352c 302d 312c 302e  7.4 c-0.5,0-1,0.
-00000a70: 312d 312e 352c 302e 3263 302c 302d 3238  1-1.5,0.2c0,0-28
-00000a80: 2e31 2c33 2e35 2d35 302e 392c 312e 3663  .1,3.5-50.9,1.6c
-00000a90: 2d33 302e 312d 322e 342d 3436 2e35 2d37  -30.1-2.4-46.5-7
-00000aa0: 2e39 2d34 362e 352d 372e 3943 3431 2e37  .9-46.5-7.9C41.7
-00000ab0: 2c33 3533 2e36 2c34 302e 342c 3335 332e  ,353.6,40.4,353.
-00000ac0: 342c 3339 2e32 2c33 3533 2e36 7a20 4d33  4,39.2,353.6z M3
-00000ad0: 392e 322c 3331 352e 3920 632d 342e 322c  9.2,315.9 c-4.2,
-00000ae0: 302e 362d 372e 312c 342e 342d 362e 352c  0.6-7.1,4.4-6.5,
-00000af0: 382e 3563 302e 342c 332c 322e 362c 352e  8.5c0.4,3,2.6,5.
-00000b00: 352c 352e 352c 362e 3363 302c 302c 3138  5,5.5,6.3c0,0,18
-00000b10: 2e35 2c36 2e31 2c35 302c 382e 3763 3235  .5,6.1,50,8.7c25
-00000b20: 2e33 2c32 2e31 2c35 342d 312e 382c 3534  .3,2.1,54-1.8,54
-00000b30: 2d31 2e38 6334 2e32 2d30 2e31 2c37 2e35  -1.8c4.2-0.1,7.5
-00000b40: 2d33 2e36 2c37 2e34 2d37 2e38 2063 2d30  -3.6,7.4-7.8 c-0
-00000b50: 2e31 2d34 2e32 2d33 2e36 2d37 2e35 2d37  .1-4.2-3.6-7.5-7
-00000b60: 2e38 2d37 2e34 632d 302e 352c 302d 312c  .8-7.4c-0.5,0-1,
-00000b70: 302e 312d 312e 352c 302e 3263 302c 302d  0.1-1.5,0.2c0,0-
-00000b80: 3238 2e31 2c33 2e35 2d35 302e 392c 312e  28.1,3.5-50.9,1.
-00000b90: 3663 2d33 302e 312d 322e 342d 3436 2e35  6c-30.1-2.4-46.5
-00000ba0: 2d37 2e39 2d34 362e 352d 372e 3920 4334  -7.9-46.5-7.9 C4
-00000bb0: 312e 372c 3331 352e 392c 3430 2e34 2c33  1.7,315.9,40.4,3
-00000bc0: 3135 2e38 2c33 392e 322c 3331 352e 397a  15.8,39.2,315.9z
-00000bd0: 204d 3339 2e32 2c32 3738 2e33 632d 342e   M39.2,278.3c-4.
-00000be0: 322c 302e 362d 372e 312c 342e 342d 362e  2,0.6-7.1,4.4-6.
-00000bf0: 352c 382e 3563 302e 342c 332c 322e 362c  5,8.5c0.4,3,2.6,
-00000c00: 352e 352c 352e 352c 362e 3363 302c 302c  5.5,5.5,6.3c0,0,
-00000c10: 3138 2e35 2c36 2e31 2c35 302c 382e 3720  18.5,6.1,50,8.7 
-00000c20: 6332 352e 332c 322e 312c 3534 2d31 2e38  c25.3,2.1,54-1.8
-00000c30: 2c35 342d 312e 3863 342e 322d 302e 312c  ,54-1.8c4.2-0.1,
-00000c40: 372e 352d 332e 362c 372e 342d 372e 3863  7.5-3.6,7.4-7.8c
-00000c50: 2d30 2e31 2d34 2e32 2d33 2e36 2d37 2e35  -0.1-4.2-3.6-7.5
-00000c60: 2d37 2e38 2d37 2e34 632d 302e 352c 302d  -7.8-7.4c-0.5,0-
-00000c70: 312c 302e 312d 312e 352c 302e 3263 302c  1,0.1-1.5,0.2c0,
-00000c80: 302d 3238 2e31 2c33 2e35 2d35 302e 392c  0-28.1,3.5-50.9,
-00000c90: 312e 3620 632d 3330 2e31 2d32 2e34 2d34  1.6 c-30.1-2.4-4
-00000ca0: 362e 352d 372e 392d 3436 2e35 2d37 2e39  6.5-7.9-46.5-7.9
-00000cb0: 4334 312e 372c 3237 382e 322c 3430 2e34  C41.7,278.2,40.4
-00000cc0: 2c32 3738 2e31 2c33 392e 322c 3237 382e  ,278.1,39.2,278.
-00000cd0: 337a 204d 2d31 332e 362c 3233 382e 3563  3z M-13.6,238.5c
-00000ce0: 2d33 392e 362c 302e 332d 3534 2e33 2c31  -39.6,0.3-54.3,1
-00000cf0: 322e 352d 3534 2e33 2c31 322e 3576 3239  2.5-54.3,12.5v29
-00000d00: 352e 3720 6330 2c30 2c31 342e 342d 3132  5.7 c0,0,14.4-12
-00000d10: 2e34 2c36 302e 382d 3130 2e35 7335 352e  .4,60.8-10.5s55.
-00000d20: 392c 3138 2e32 2c31 3132 2e39 2c31 392e  9,18.2,112.9,19.
-00000d30: 3373 3731 2e33 2d38 2e38 2c37 312e 332d  3s71.3-8.8,71.3-
-00000d40: 382e 386c 302e 382d 3330 312e 3463 302c  8.8l0.8-301.4c0,
-00000d50: 302d 3235 2e36 2c37 2e33 2d37 352e 362c  0-25.6,7.3-75.6,
-00000d60: 372e 3763 2d34 392e 392c 302e 342d 3631  7.7c-49.9,0.4-61
-00000d70: 2e39 2d31 322e 372d 3130 372e 372d 3134  .9-12.7-107.7-14
-00000d80: 2e32 2043 2d38 2e32 2c32 3338 2e36 2d31  .2 C-8.2,238.6-1
-00000d90: 302e 392c 3233 382e 352d 3133 2e36 2c32  0.9,238.5-13.6,2
-00000da0: 3338 2e35 7a20 4d31 392e 352c 3235 372e  38.5z M19.5,257.
-00000db0: 3863 302c 302c 3234 2c37 2e39 2c36 382e  8c0,0,24,7.9,68.
-00000dc0: 332c 3130 2e31 6333 372e 352c 312e 392c  3,10.1c37.5,1.9,
-00000dd0: 3735 2d33 2e37 2c37 352d 332e 3776 3236  75-3.7,75-3.7v26
-00000de0: 372e 3963 302c 302d 3139 2c31 302d 3636  7.9c0,0-19,10-66
-00000df0: 2e35 2c36 2e36 2043 3539 2e35 2c35 3336  .5,6.6 C59.5,536
-00000e00: 2e31 2c31 392c 3532 322e 312c 3139 2c35  .1,19,522.1,19,5
-00000e10: 3232 2e31 4c31 392e 352c 3235 372e 387a  22.1L19.5,257.8z
-00000e20: 204d 2d33 2e36 2c32 3634 2e38 6334 2e32   M-3.6,264.8c4.2
-00000e30: 2c30 2c37 2e37 2c33 2e34 2c37 2e37 2c37  ,0,7.7,3.4,7.7,7
-00000e40: 2e37 6330 2c34 2e32 2d33 2e34 2c37 2e37  .7c0,4.2-3.4,7.7
-00000e50: 2d37 2e37 2c37 2e37 6330 2c30 2d31 322e  -7.7,7.7c0,0-12.
-00000e60: 342c 302e 312d 3230 2c30 2e38 2063 2d31  4,0.1-20,0.8 c-1
-00000e70: 322e 372c 312e 332d 3231 2e34 2c35 2e39  2.7,1.3-21.4,5.9
-00000e80: 2d32 312e 342c 352e 3963 2d33 2e37 2c32  -21.4,5.9c-3.7,2
-00000e90: 2d38 2e34 2c30 2e35 2d31 302e 332d 332e  -8.4,0.5-10.3-3.
-00000ea0: 3263 2d32 2d33 2e37 2d30 2e35 2d38 2e34  2c-2-3.7-0.5-8.4
-00000eb0: 2c33 2e32 2d31 302e 3363 302c 302c 302c  ,3.2-10.3c0,0,0,
-00000ec0: 302c 302c 3063 302c 302c 3131 2e33 2d36  0,0,0c0,0,11.3-6
-00000ed0: 2c32 372d 372e 3520 432d 3136 2c32 3634  ,27-7.5 C-16,264
-00000ee0: 2e39 2d33 2e36 2c32 3634 2e38 2d33 2e36  .9-3.6,264.8-3.6
-00000ef0: 2c32 3634 2e38 7a20 4d2d 3131 2c33 3032  ,264.8z M-11,302
-00000f00: 2e36 6334 2e32 2d30 2e31 2c37 2e34 2c30  .6c4.2-0.1,7.4,0
-00000f10: 2c37 2e34 2c30 6334 2e32 2c30 2e35 2c37  ,7.4,0c4.2,0.5,7
-00000f20: 2e32 2c34 2e33 2c36 2e37 2c38 2e35 632d  .2,4.3,6.7,8.5c-
-00000f30: 302e 342c 332e 352d 332e 322c 362e 332d  0.4,3.5-3.2,6.3-
-00000f40: 362e 372c 362e 3720 6330 2c30 2d31 322e  6.7,6.7 c0,0-12.
-00000f50: 342c 302e 312d 3230 2c30 2e38 632d 3132  4,0.1-20,0.8c-12
-00000f60: 2e37 2c31 2e33 2d32 312e 342c 352e 392d  .7,1.3-21.4,5.9-
-00000f70: 3231 2e34 2c35 2e39 632d 332e 372c 322d  21.4,5.9c-3.7,2-
-00000f80: 382e 342c 302e 352d 3130 2e33 2d33 2e32  8.4,0.5-10.3-3.2
-00000f90: 632d 322d 332e 372d 302e 352d 382e 342c  c-2-3.7-0.5-8.4,
-00000fa0: 332e 322d 3130 2e33 6330 2c30 2c31 312e  3.2-10.3c0,0,11.
-00000fb0: 332d 362c 3237 2d37 2e35 2043 2d32 302e  3-6,27-7.5 C-20.
-00000fc0: 352c 3330 322e 392d 3135 2e32 2c33 3032  5,302.9-15.2,302
-00000fd0: 2e37 2d31 312c 3330 322e 367a 204d 2d33  .7-11,302.6z M-3
-00000fe0: 2e36 2c33 3430 2e32 6334 2e32 2c30 2c37  .6,340.2c4.2,0,7
-00000ff0: 2e37 2c33 2e34 2c37 2e37 2c37 2e37 732d  .7,3.4,7.7,7.7s-
-00001000: 332e 342c 372e 372d 372e 372c 372e 3763  3.4,7.7-7.7,7.7c
-00001010: 302c 302d 3132 2e34 2d30 2e31 2d32 302c  0,0-12.4-0.1-20,
-00001020: 302e 3720 632d 3132 2e37 2c31 2e33 2d32  0.7 c-12.7,1.3-2
-00001030: 312e 342c 352e 392d 3231 2e34 2c35 2e39  1.4,5.9-21.4,5.9
-00001040: 632d 332e 372c 322d 382e 342c 302e 352d  c-3.7,2-8.4,0.5-
-00001050: 3130 2e33 2d33 2e32 632d 322d 332e 372d  10.3-3.2c-2-3.7-
-00001060: 302e 352d 382e 342c 332e 322d 3130 2e33  0.5-8.4,3.2-10.3
-00001070: 6330 2c30 2c31 312e 332d 362c 3237 2d37  c0,0,11.3-6,27-7
-00001080: 2e35 432d 3136 2c33 3430 2e31 2d33 2e36  .5C-16,340.1-3.6
-00001090: 2c33 3430 2e32 2d33 2e36 2c33 3430 2e32  ,340.2-3.6,340.2
-000010a0: 7a22 0a20 2020 2020 2020 2020 202f 3e0a  z".          />.
-000010b0: 2020 2020 2020 2020 3c2f 7376 673e 0a20          </svg>. 
-000010c0: 2020 2020 203c 2f61 3e0a 2020 2020 2020       </a>.      
-000010d0: 7b25 2d20 656e 6469 6620 2d25 7d20 7b23  {%- endif -%} {#
-000010e0: 2d20 5368 6f77 2047 6974 4875 6220 7265  - Show GitHub re
-000010f0: 706f 7369 746f 7279 2068 6f6d 6520 2d23  pository home -#
-00001100: 7d20 7b25 2d20 6966 2052 4541 4454 4845  } {%- if READTHE
-00001110: 444f 4353 2061 6e64 0a20 2020 2020 2064  DOCS and.      d
-00001120: 6973 706c 6179 5f67 6974 6875 6220 616e  isplay_github an
-00001130: 6420 6769 7468 7562 5f75 7365 7220 213d  d github_user !=
-00001140: 2022 4e6f 6e65 2220 616e 6420 6769 7468   "None" and gith
-00001150: 7562 5f72 6570 6f20 213d 2022 4e6f 6e65  ub_repo != "None
-00001160: 2220 2d25 7d0a 2020 2020 2020 3c61 0a20  " -%}.      <a. 
-00001170: 2020 2020 2020 2063 6c61 7373 3d22 6d75         class="mu
-00001180: 7465 642d 6c69 6e6b 220a 2020 2020 2020  ted-link".      
-00001190: 2020 6872 6566 3d22 6874 7470 733a 2f2f    href="https://
-000011a0: 6769 7468 7562 2e63 6f6d 2f7b 7b20 6769  github.com/{{ gi
-000011b0: 7468 7562 5f75 7365 7220 7d7d 2f7b 7b20  thub_user }}/{{ 
-000011c0: 6769 7468 7562 5f72 6570 6f20 7d7d 220a  github_repo }}".
-000011d0: 2020 2020 2020 2020 6172 6961 2d6c 6162          aria-lab
-000011e0: 656c 3d22 4f6e 2047 6974 4875 6222 0a20  el="On GitHub". 
-000011f0: 2020 2020 203e 0a20 2020 2020 2020 203c       >.        <
-00001200: 7376 670a 2020 2020 2020 2020 2020 7374  svg.          st
-00001210: 726f 6b65 3d22 6375 7272 656e 7443 6f6c  roke="currentCol
-00001220: 6f72 220a 2020 2020 2020 2020 2020 6669  or".          fi
-00001230: 6c6c 3d22 6375 7272 656e 7443 6f6c 6f72  ll="currentColor
-00001240: 220a 2020 2020 2020 2020 2020 7374 726f  ".          stro
-00001250: 6b65 2d77 6964 7468 3d22 3022 0a20 2020  ke-width="0".   
-00001260: 2020 2020 2020 2076 6965 7742 6f78 3d22         viewBox="
-00001270: 3020 3020 3136 2031 3622 0a20 2020 2020  0 0 16 16".     
-00001280: 2020 203e 0a20 2020 2020 2020 2020 203c     >.          <
-00001290: 7061 7468 0a20 2020 2020 2020 2020 2020  path.           
-000012a0: 2066 696c 6c2d 7275 6c65 3d22 6576 656e   fill-rule="even
-000012b0: 6f64 6422 0a20 2020 2020 2020 2020 2020  odd".           
-000012c0: 2064 3d22 4d38 2030 4333 2e35 3820 3020   d="M8 0C3.58 0 
-000012d0: 3020 332e 3538 2030 2038 6330 2033 2e35  0 3.58 0 8c0 3.5
-000012e0: 3420 322e 3239 2036 2e35 3320 352e 3437  4 2.29 6.53 5.47
-000012f0: 2037 2e35 392e 342e 3037 2e35 352d 2e31   7.59.4.07.55-.1
-00001300: 372e 3535 2d2e 3338 2030 2d2e 3139 2d2e  7.55-.38 0-.19-.
-00001310: 3031 2d2e 3832 2d2e 3031 2d31 2e34 392d  01-.82-.01-1.49-
-00001320: 322e 3031 2e33 372d 322e 3533 2d2e 3439  2.01.37-2.53-.49
-00001330: 2d32 2e36 392d 2e39 342d 2e30 392d 2e32  -2.69-.94-.09-.2
-00001340: 332d 2e34 382d 2e39 342d 2e38 322d 312e  3-.48-.94-.82-1.
-00001350: 3133 2d2e 3238 2d2e 3135 2d2e 3638 2d2e  13-.28-.15-.68-.
-00001360: 3532 2d2e 3031 2d2e 3533 2e36 332d 2e30  52-.01-.53.63-.0
-00001370: 3120 312e 3038 2e35 3820 312e 3233 2e38  1 1.08.58 1.23.8
-00001380: 322e 3732 2031 2e32 3120 312e 3837 2e38  2.72 1.21 1.87.8
-00001390: 3720 322e 3333 2e36 362e 3037 2d2e 3532  7 2.33.66.07-.52
-000013a0: 2e32 382d 2e38 372e 3531 2d31 2e30 372d  .28-.87.51-1.07-
-000013b0: 312e 3738 2d2e 322d 332e 3634 2d2e 3839  1.78-.2-3.64-.89
-000013c0: 2d33 2e36 342d 332e 3935 2030 2d2e 3837  -3.64-3.95 0-.87
-000013d0: 2e33 312d 312e 3539 2e38 322d 322e 3135  .31-1.59.82-2.15
-000013e0: 2d2e 3038 2d2e 322d 2e33 362d 312e 3032  -.08-.2-.36-1.02
-000013f0: 2e30 382d 322e 3132 2030 2030 202e 3637  .08-2.12 0 0 .67
-00001400: 2d2e 3231 2032 2e32 2e38 322e 3634 2d2e  -.21 2.2.82.64-.
-00001410: 3138 2031 2e33 322d 2e32 3720 322d 2e32  18 1.32-.27 2-.2
-00001420: 372e 3638 2030 2031 2e33 362e 3039 2032  7.68 0 1.36.09 2
-00001430: 202e 3237 2031 2e35 332d 312e 3034 2032   .27 1.53-1.04 2
-00001440: 2e32 2d2e 3832 2032 2e32 2d2e 3832 2e34  .2-.82 2.2-.82.4
-00001450: 3420 312e 312e 3136 2031 2e39 322e 3038  4 1.1.16 1.92.08
-00001460: 2032 2e31 322e 3531 2e35 362e 3832 2031   2.12.51.56.82 1
-00001470: 2e32 372e 3832 2032 2e31 3520 3020 332e  .27.82 2.15 0 3.
-00001480: 3037 2d31 2e38 3720 332e 3735 2d33 2e36  07-1.87 3.75-3.6
-00001490: 3520 332e 3935 2e32 392e 3235 2e35 342e  5 3.95.29.25.54.
-000014a0: 3733 2e35 3420 312e 3438 2030 2031 2e30  73.54 1.48 0 1.0
-000014b0: 372d 2e30 3120 312e 3933 2d2e 3031 2032  7-.01 1.93-.01 2
-000014c0: 2e32 2030 202e 3231 2e31 352e 3436 2e35  .2 0 .21.15.46.5
-000014d0: 352e 3338 4138 2e30 3133 2038 2e30 3133  5.38A8.013 8.013
-000014e0: 2030 2030 2030 2031 3620 3863 302d 342e   0 0 0 16 8c0-4.
-000014f0: 3432 2d33 2e35 382d 382d 382d 387a 220a  42-3.58-8-8-8z".
-00001500: 2020 2020 2020 2020 2020 3e3c 2f70 6174            ></pat
-00001510: 683e 0a20 2020 2020 2020 203c 2f73 7667  h>.        </svg
-00001520: 3e0a 2020 2020 2020 3c2f 613e 0a20 2020  >.      </a>.   
-00001530: 2020 207b 252d 2065 6e64 6966 202d 257d     {%- endif -%}
-00001540: 207b 252d 2065 6e64 6966 2025 7d0a 2020   {%- endif %}.  
-00001550: 2020 3c2f 6469 763e 0a20 2020 207b 252d    </div>.    {%-
-00001560: 2065 6e64 6966 2025 7d0a 2020 3c2f 6469   endif %}.  </di
-00001570: 763e 0a3c 2f64 6976 3e0a 7b25 2065 6e64  v>.</div>.{% end
-00001580: 626c 6f63 6b20 257d 0a                   block %}.
+000003c0: 6469 7620 636c 6173 733d 2268 6d2d 636f  div class="hm-co
+000003d0: 7079 7269 6768 7420 636f 7079 7269 6768  pyright copyrigh
+000003e0: 7422 3e0a 2020 2020 3c2f 6469 763e 0a20  t">.    </div>. 
+000003f0: 2020 207b 252d 2065 6e64 6966 2025 7d0a     {%- endif %}.
+00000400: 2020 3c2f 6469 763e 0a20 203c 6469 7620    </div>.  <div 
+00000410: 636c 6173 733d 2272 6967 6874 2d64 6574  class="right-det
+00000420: 6169 6c73 223e 0a20 2020 207b 2520 6966  ails">.    {% if
+00000430: 2074 6865 6d65 5f66 6f6f 7465 725f 6963   theme_footer_ic
+00000440: 6f6e 7320 6f72 2052 4541 4454 4845 444f  ons or READTHEDO
+00000450: 4353 202d 257d 0a20 2020 203c 6469 7620  CS -%}.    <div 
+00000460: 636c 6173 733d 2269 636f 6e73 223e 0a20  class="icons">. 
+00000470: 2020 2020 207b 2520 6966 2074 6865 6d65       {% if theme
+00000480: 5f66 6f6f 7465 725f 6963 6f6e 7320 2d25  _footer_icons -%
+00000490: 7d20 7b25 2066 6f72 2069 636f 6e5f 6469  } {% for icon_di
+000004a0: 6374 2069 6e20 7468 656d 655f 666f 6f74  ct in theme_foot
+000004b0: 6572 5f69 636f 6e73 202d 257d 0a20 2020  er_icons -%}.   
+000004c0: 2020 203c 610a 2020 2020 2020 2020 636c     <a.        cl
+000004d0: 6173 733d 226d 7574 6564 2d6c 696e 6b20  ass="muted-link 
+000004e0: 7b7b 2069 636f 6e5f 6469 6374 2e63 6c61  {{ icon_dict.cla
+000004f0: 7373 207d 7d22 0a20 2020 2020 2020 2068  ss }}".        h
+00000500: 7265 663d 227b 7b20 6963 6f6e 5f64 6963  ref="{{ icon_dic
+00000510: 742e 7572 6c20 7d7d 220a 2020 2020 2020  t.url }}".      
+00000520: 2020 6172 6961 2d6c 6162 656c 3d22 7b7b    aria-label="{{
+00000530: 2069 636f 6e5f 6469 6374 2e6e 616d 6520   icon_dict.name 
+00000540: 7d7d 220a 2020 2020 2020 3e0a 2020 2020  }}".      >.    
+00000550: 2020 2020 7b7b 2d20 6963 6f6e 5f64 6963      {{- icon_dic
+00000560: 742e 6874 6d6c 202d 7d7d 0a20 2020 2020  t.html -}}.     
+00000570: 203c 2f61 3e0a 2020 2020 2020 7b25 2065   </a>.      {% e
+00000580: 6e64 666f 7220 257d 207b 252d 2065 6c73  ndfor %} {%- els
+00000590: 6520 2d25 7d20 7b23 2d20 5368 6f77 2052  e -%} {#- Show R
+000005a0: 6561 6420 7468 6520 446f 6373 2070 726f  ead the Docs pro
+000005b0: 6a65 6374 202d 237d 207b 252d 2069 660a  ject -#} {%- if.
+000005c0: 2020 2020 2020 5245 4144 5448 4544 4f43        READTHEDOC
+000005d0: 5320 616e 6420 736c 7567 202d 257d 0a20  S and slug -%}. 
+000005e0: 2020 2020 203c 610a 2020 2020 2020 2020       <a.        
+000005f0: 636c 6173 733d 226d 7574 6564 2d6c 696e  class="muted-lin
+00000600: 6b22 0a20 2020 2020 2020 2068 7265 663d  k".        href=
+00000610: 2268 7474 7073 3a2f 2f72 6561 6474 6865  "https://readthe
+00000620: 646f 6373 2e6f 7267 2f70 726f 6a65 6374  docs.org/project
+00000630: 732f 7b7b 2073 6c75 6720 7d7d 220a 2020  s/{{ slug }}".  
+00000640: 2020 2020 2020 6172 6961 2d6c 6162 656c        aria-label
+00000650: 3d22 4f6e 2052 6561 6420 7468 6520 446f  ="On Read the Do
+00000660: 6373 220a 2020 2020 2020 3e0a 2020 2020  cs".      >.    
+00000670: 2020 2020 3c73 7667 2078 3d22 3070 7822      <svg x="0px"
+00000680: 2079 3d22 3070 7822 2076 6965 7742 6f78   y="0px" viewBox
+00000690: 3d22 2d31 3235 2032 3137 2033 3630 2033  ="-125 217 360 3
+000006a0: 3630 2220 786d 6c3a 7370 6163 653d 2270  60" xml:space="p
+000006b0: 7265 7365 7276 6522 3e0a 2020 2020 2020  reserve">.      
+000006c0: 2020 2020 3c70 6174 680a 2020 2020 2020      <path.      
+000006d0: 2020 2020 2020 6669 6c6c 3d22 6375 7272        fill="curr
+000006e0: 656e 7443 6f6c 6f72 220a 2020 2020 2020  entColor".      
+000006f0: 2020 2020 2020 643d 224d 3339 2e32 2c33        d="M39.2,3
+00000700: 3931 2e33 632d 342e 322c 302e 362d 372e  91.3c-4.2,0.6-7.
+00000710: 312c 342e 342d 362e 352c 382e 3563 302e  1,4.4-6.5,8.5c0.
+00000720: 342c 332c 322e 362c 352e 352c 352e 352c  4,3,2.6,5.5,5.5,
+00000730: 362e 3320 6330 2c30 2c31 382e 352c 362e  6.3 c0,0,18.5,6.
+00000740: 312c 3530 2c38 2e37 6332 352e 332c 322e  1,50,8.7c25.3,2.
+00000750: 312c 3534 2d31 2e38 2c35 342d 312e 3863  1,54-1.8,54-1.8c
+00000760: 342e 322d 302e 312c 372e 352d 332e 362c  4.2-0.1,7.5-3.6,
+00000770: 372e 342d 372e 3863 2d30 2e31 2d34 2e32  7.4-7.8c-0.1-4.2
+00000780: 2d33 2e36 2d37 2e35 2d37 2e38 2d37 2e34  -3.6-7.5-7.8-7.4
+00000790: 632d 302e 352c 302d 312c 302e 312d 312e  c-0.5,0-1,0.1-1.
+000007a0: 352c 302e 3220 6330 2c30 2d32 382e 312c  5,0.2 c0,0-28.1,
+000007b0: 332e 352d 3530 2e39 2c31 2e36 632d 3330  3.5-50.9,1.6c-30
+000007c0: 2e31 2d32 2e34 2d34 362e 352d 372e 392d  .1-2.4-46.5-7.9-
+000007d0: 3436 2e35 2d37 2e39 4334 312e 372c 3339  46.5-7.9C41.7,39
+000007e0: 312e 332c 3430 2e34 2c33 3931 2e31 2c33  1.3,40.4,391.1,3
+000007f0: 392e 322c 3339 312e 337a 204d 3339 2e32  9.2,391.3z M39.2
+00000800: 2c33 3533 2e36 632d 342e 322c 302e 362d  ,353.6c-4.2,0.6-
+00000810: 372e 312c 342e 342d 362e 352c 382e 3520  7.1,4.4-6.5,8.5 
+00000820: 6330 2e34 2c33 2c32 2e36 2c35 2e35 2c35  c0.4,3,2.6,5.5,5
+00000830: 2e35 2c36 2e33 6330 2c30 2c31 382e 352c  .5,6.3c0,0,18.5,
+00000840: 362e 312c 3530 2c38 2e37 6332 352e 332c  6.1,50,8.7c25.3,
+00000850: 322e 312c 3534 2d31 2e38 2c35 342d 312e  2.1,54-1.8,54-1.
+00000860: 3863 342e 322d 302e 312c 372e 352d 332e  8c4.2-0.1,7.5-3.
+00000870: 362c 372e 342d 372e 3863 2d30 2e31 2d34  6,7.4-7.8c-0.1-4
+00000880: 2e32 2d33 2e36 2d37 2e35 2d37 2e38 2d37  .2-3.6-7.5-7.8-7
+00000890: 2e34 2063 2d30 2e35 2c30 2d31 2c30 2e31  .4 c-0.5,0-1,0.1
+000008a0: 2d31 2e35 2c30 2e32 6330 2c30 2d32 382e  -1.5,0.2c0,0-28.
+000008b0: 312c 332e 352d 3530 2e39 2c31 2e36 632d  1,3.5-50.9,1.6c-
+000008c0: 3330 2e31 2d32 2e34 2d34 362e 352d 372e  30.1-2.4-46.5-7.
+000008d0: 392d 3436 2e35 2d37 2e39 4334 312e 372c  9-46.5-7.9C41.7,
+000008e0: 3335 332e 362c 3430 2e34 2c33 3533 2e34  353.6,40.4,353.4
+000008f0: 2c33 392e 322c 3335 332e 367a 204d 3339  ,39.2,353.6z M39
+00000900: 2e32 2c33 3135 2e39 2063 2d34 2e32 2c30  .2,315.9 c-4.2,0
+00000910: 2e36 2d37 2e31 2c34 2e34 2d36 2e35 2c38  .6-7.1,4.4-6.5,8
+00000920: 2e35 6330 2e34 2c33 2c32 2e36 2c35 2e35  .5c0.4,3,2.6,5.5
+00000930: 2c35 2e35 2c36 2e33 6330 2c30 2c31 382e  ,5.5,6.3c0,0,18.
+00000940: 352c 362e 312c 3530 2c38 2e37 6332 352e  5,6.1,50,8.7c25.
+00000950: 332c 322e 312c 3534 2d31 2e38 2c35 342d  3,2.1,54-1.8,54-
+00000960: 312e 3863 342e 322d 302e 312c 372e 352d  1.8c4.2-0.1,7.5-
+00000970: 332e 362c 372e 342d 372e 3820 632d 302e  3.6,7.4-7.8 c-0.
+00000980: 312d 342e 322d 332e 362d 372e 352d 372e  1-4.2-3.6-7.5-7.
+00000990: 382d 372e 3463 2d30 2e35 2c30 2d31 2c30  8-7.4c-0.5,0-1,0
+000009a0: 2e31 2d31 2e35 2c30 2e32 6330 2c30 2d32  .1-1.5,0.2c0,0-2
+000009b0: 382e 312c 332e 352d 3530 2e39 2c31 2e36  8.1,3.5-50.9,1.6
+000009c0: 632d 3330 2e31 2d32 2e34 2d34 362e 352d  c-30.1-2.4-46.5-
+000009d0: 372e 392d 3436 2e35 2d37 2e39 2043 3431  7.9-46.5-7.9 C41
+000009e0: 2e37 2c33 3135 2e39 2c34 302e 342c 3331  .7,315.9,40.4,31
+000009f0: 352e 382c 3339 2e32 2c33 3135 2e39 7a20  5.8,39.2,315.9z 
+00000a00: 4d33 392e 322c 3237 382e 3363 2d34 2e32  M39.2,278.3c-4.2
+00000a10: 2c30 2e36 2d37 2e31 2c34 2e34 2d36 2e35  ,0.6-7.1,4.4-6.5
+00000a20: 2c38 2e35 6330 2e34 2c33 2c32 2e36 2c35  ,8.5c0.4,3,2.6,5
+00000a30: 2e35 2c35 2e35 2c36 2e33 6330 2c30 2c31  .5,5.5,6.3c0,0,1
+00000a40: 382e 352c 362e 312c 3530 2c38 2e37 2063  8.5,6.1,50,8.7 c
+00000a50: 3235 2e33 2c32 2e31 2c35 342d 312e 382c  25.3,2.1,54-1.8,
+00000a60: 3534 2d31 2e38 6334 2e32 2d30 2e31 2c37  54-1.8c4.2-0.1,7
+00000a70: 2e35 2d33 2e36 2c37 2e34 2d37 2e38 632d  .5-3.6,7.4-7.8c-
+00000a80: 302e 312d 342e 322d 332e 362d 372e 352d  0.1-4.2-3.6-7.5-
+00000a90: 372e 382d 372e 3463 2d30 2e35 2c30 2d31  7.8-7.4c-0.5,0-1
+00000aa0: 2c30 2e31 2d31 2e35 2c30 2e32 6330 2c30  ,0.1-1.5,0.2c0,0
+00000ab0: 2d32 382e 312c 332e 352d 3530 2e39 2c31  -28.1,3.5-50.9,1
+00000ac0: 2e36 2063 2d33 302e 312d 322e 342d 3436  .6 c-30.1-2.4-46
+00000ad0: 2e35 2d37 2e39 2d34 362e 352d 372e 3943  .5-7.9-46.5-7.9C
+00000ae0: 3431 2e37 2c32 3738 2e32 2c34 302e 342c  41.7,278.2,40.4,
+00000af0: 3237 382e 312c 3339 2e32 2c32 3738 2e33  278.1,39.2,278.3
+00000b00: 7a20 4d2d 3133 2e36 2c32 3338 2e35 632d  z M-13.6,238.5c-
+00000b10: 3339 2e36 2c30 2e33 2d35 342e 332c 3132  39.6,0.3-54.3,12
+00000b20: 2e35 2d35 342e 332c 3132 2e35 7632 3935  .5-54.3,12.5v295
+00000b30: 2e37 2063 302c 302c 3134 2e34 2d31 322e  .7 c0,0,14.4-12.
+00000b40: 342c 3630 2e38 2d31 302e 3573 3535 2e39  4,60.8-10.5s55.9
+00000b50: 2c31 382e 322c 3131 322e 392c 3139 2e33  ,18.2,112.9,19.3
+00000b60: 7337 312e 332d 382e 382c 3731 2e33 2d38  s71.3-8.8,71.3-8
+00000b70: 2e38 6c30 2e38 2d33 3031 2e34 6330 2c30  .8l0.8-301.4c0,0
+00000b80: 2d32 352e 362c 372e 332d 3735 2e36 2c37  -25.6,7.3-75.6,7
+00000b90: 2e37 632d 3439 2e39 2c30 2e34 2d36 312e  .7c-49.9,0.4-61.
+00000ba0: 392d 3132 2e37 2d31 3037 2e37 2d31 342e  9-12.7-107.7-14.
+00000bb0: 3220 432d 382e 322c 3233 382e 362d 3130  2 C-8.2,238.6-10
+00000bc0: 2e39 2c32 3338 2e35 2d31 332e 362c 3233  .9,238.5-13.6,23
+00000bd0: 382e 357a 204d 3139 2e35 2c32 3537 2e38  8.5z M19.5,257.8
+00000be0: 6330 2c30 2c32 342c 372e 392c 3638 2e33  c0,0,24,7.9,68.3
+00000bf0: 2c31 302e 3163 3337 2e35 2c31 2e39 2c37  ,10.1c37.5,1.9,7
+00000c00: 352d 332e 372c 3735 2d33 2e37 7632 3637  5-3.7,75-3.7v267
+00000c10: 2e39 6330 2c30 2d31 392c 3130 2d36 362e  .9c0,0-19,10-66.
+00000c20: 352c 362e 3620 4335 392e 352c 3533 362e  5,6.6 C59.5,536.
+00000c30: 312c 3139 2c35 3232 2e31 2c31 392c 3532  1,19,522.1,19,52
+00000c40: 322e 314c 3139 2e35 2c32 3537 2e38 7a20  2.1L19.5,257.8z 
+00000c50: 4d2d 332e 362c 3236 342e 3863 342e 322c  M-3.6,264.8c4.2,
+00000c60: 302c 372e 372c 332e 342c 372e 372c 372e  0,7.7,3.4,7.7,7.
+00000c70: 3763 302c 342e 322d 332e 342c 372e 372d  7c0,4.2-3.4,7.7-
+00000c80: 372e 372c 372e 3763 302c 302d 3132 2e34  7.7,7.7c0,0-12.4
+00000c90: 2c30 2e31 2d32 302c 302e 3820 632d 3132  ,0.1-20,0.8 c-12
+00000ca0: 2e37 2c31 2e33 2d32 312e 342c 352e 392d  .7,1.3-21.4,5.9-
+00000cb0: 3231 2e34 2c35 2e39 632d 332e 372c 322d  21.4,5.9c-3.7,2-
+00000cc0: 382e 342c 302e 352d 3130 2e33 2d33 2e32  8.4,0.5-10.3-3.2
+00000cd0: 632d 322d 332e 372d 302e 352d 382e 342c  c-2-3.7-0.5-8.4,
+00000ce0: 332e 322d 3130 2e33 6330 2c30 2c30 2c30  3.2-10.3c0,0,0,0
+00000cf0: 2c30 2c30 6330 2c30 2c31 312e 332d 362c  ,0,0c0,0,11.3-6,
+00000d00: 3237 2d37 2e35 2043 2d31 362c 3236 342e  27-7.5 C-16,264.
+00000d10: 392d 332e 362c 3236 342e 382d 332e 362c  9-3.6,264.8-3.6,
+00000d20: 3236 342e 387a 204d 2d31 312c 3330 322e  264.8z M-11,302.
+00000d30: 3663 342e 322d 302e 312c 372e 342c 302c  6c4.2-0.1,7.4,0,
+00000d40: 372e 342c 3063 342e 322c 302e 352c 372e  7.4,0c4.2,0.5,7.
+00000d50: 322c 342e 332c 362e 372c 382e 3563 2d30  2,4.3,6.7,8.5c-0
+00000d60: 2e34 2c33 2e35 2d33 2e32 2c36 2e33 2d36  .4,3.5-3.2,6.3-6
+00000d70: 2e37 2c36 2e37 2063 302c 302d 3132 2e34  .7,6.7 c0,0-12.4
+00000d80: 2c30 2e31 2d32 302c 302e 3863 2d31 322e  ,0.1-20,0.8c-12.
+00000d90: 372c 312e 332d 3231 2e34 2c35 2e39 2d32  7,1.3-21.4,5.9-2
+00000da0: 312e 342c 352e 3963 2d33 2e37 2c32 2d38  1.4,5.9c-3.7,2-8
+00000db0: 2e34 2c30 2e35 2d31 302e 332d 332e 3263  .4,0.5-10.3-3.2c
+00000dc0: 2d32 2d33 2e37 2d30 2e35 2d38 2e34 2c33  -2-3.7-0.5-8.4,3
+00000dd0: 2e32 2d31 302e 3363 302c 302c 3131 2e33  .2-10.3c0,0,11.3
+00000de0: 2d36 2c32 372d 372e 3520 432d 3230 2e35  -6,27-7.5 C-20.5
+00000df0: 2c33 3032 2e39 2d31 352e 322c 3330 322e  ,302.9-15.2,302.
+00000e00: 372d 3131 2c33 3032 2e36 7a20 4d2d 332e  7-11,302.6z M-3.
+00000e10: 362c 3334 302e 3263 342e 322c 302c 372e  6,340.2c4.2,0,7.
+00000e20: 372c 332e 342c 372e 372c 372e 3773 2d33  7,3.4,7.7,7.7s-3
+00000e30: 2e34 2c37 2e37 2d37 2e37 2c37 2e37 6330  .4,7.7-7.7,7.7c0
+00000e40: 2c30 2d31 322e 342d 302e 312d 3230 2c30  ,0-12.4-0.1-20,0
+00000e50: 2e37 2063 2d31 322e 372c 312e 332d 3231  .7 c-12.7,1.3-21
+00000e60: 2e34 2c35 2e39 2d32 312e 342c 352e 3963  .4,5.9-21.4,5.9c
+00000e70: 2d33 2e37 2c32 2d38 2e34 2c30 2e35 2d31  -3.7,2-8.4,0.5-1
+00000e80: 302e 332d 332e 3263 2d32 2d33 2e37 2d30  0.3-3.2c-2-3.7-0
+00000e90: 2e35 2d38 2e34 2c33 2e32 2d31 302e 3363  .5-8.4,3.2-10.3c
+00000ea0: 302c 302c 3131 2e33 2d36 2c32 372d 372e  0,0,11.3-6,27-7.
+00000eb0: 3543 2d31 362c 3334 302e 312d 332e 362c  5C-16,340.1-3.6,
+00000ec0: 3334 302e 322d 332e 362c 3334 302e 327a  340.2-3.6,340.2z
+00000ed0: 220a 2020 2020 2020 2020 2020 2f3e 0a20  ".          />. 
+00000ee0: 2020 2020 2020 203c 2f73 7667 3e0a 2020         </svg>.  
+00000ef0: 2020 2020 3c2f 613e 0a20 2020 2020 207b      </a>.      {
+00000f00: 252d 2065 6e64 6966 202d 257d 207b 232d  %- endif -%} {#-
+00000f10: 2053 686f 7720 4769 7448 7562 2072 6570   Show GitHub rep
+00000f20: 6f73 6974 6f72 7920 686f 6d65 202d 237d  ository home -#}
+00000f30: 207b 252d 2069 6620 5245 4144 5448 4544   {%- if READTHED
+00000f40: 4f43 5320 616e 640a 2020 2020 2020 6469  OCS and.      di
+00000f50: 7370 6c61 795f 6769 7468 7562 2061 6e64  splay_github and
+00000f60: 2067 6974 6875 625f 7573 6572 2021 3d20   github_user != 
+00000f70: 224e 6f6e 6522 2061 6e64 2067 6974 6875  "None" and githu
+00000f80: 625f 7265 706f 2021 3d20 224e 6f6e 6522  b_repo != "None"
+00000f90: 202d 257d 0a20 2020 2020 203c 610a 2020   -%}.      <a.  
+00000fa0: 2020 2020 2020 636c 6173 733d 226d 7574        class="mut
+00000fb0: 6564 2d6c 696e 6b22 0a20 2020 2020 2020  ed-link".       
+00000fc0: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+00000fd0: 6974 6875 622e 636f 6d2f 7b7b 2067 6974  ithub.com/{{ git
+00000fe0: 6875 625f 7573 6572 207d 7d2f 7b7b 2067  hub_user }}/{{ g
+00000ff0: 6974 6875 625f 7265 706f 207d 7d22 0a20  ithub_repo }}". 
+00001000: 2020 2020 2020 2061 7269 612d 6c61 6265         aria-labe
+00001010: 6c3d 224f 6e20 4769 7448 7562 220a 2020  l="On GitHub".  
+00001020: 2020 2020 3e0a 2020 2020 2020 2020 3c73      >.        <s
+00001030: 7667 0a20 2020 2020 2020 2020 2073 7472  vg.          str
+00001040: 6f6b 653d 2263 7572 7265 6e74 436f 6c6f  oke="currentColo
+00001050: 7222 0a20 2020 2020 2020 2020 2066 696c  r".          fil
+00001060: 6c3d 2263 7572 7265 6e74 436f 6c6f 7222  l="currentColor"
+00001070: 0a20 2020 2020 2020 2020 2073 7472 6f6b  .          strok
+00001080: 652d 7769 6474 683d 2230 220a 2020 2020  e-width="0".    
+00001090: 2020 2020 2020 7669 6577 426f 783d 2230        viewBox="0
+000010a0: 2030 2031 3620 3136 220a 2020 2020 2020   0 16 16".      
+000010b0: 2020 3e0a 2020 2020 2020 2020 2020 3c70    >.          <p
+000010c0: 6174 680a 2020 2020 2020 2020 2020 2020  ath.            
+000010d0: 6669 6c6c 2d72 756c 653d 2265 7665 6e6f  fill-rule="eveno
+000010e0: 6464 220a 2020 2020 2020 2020 2020 2020  dd".            
+000010f0: 643d 224d 3820 3043 332e 3538 2030 2030  d="M8 0C3.58 0 0
+00001100: 2033 2e35 3820 3020 3863 3020 332e 3534   3.58 0 8c0 3.54
+00001110: 2032 2e32 3920 362e 3533 2035 2e34 3720   2.29 6.53 5.47 
+00001120: 372e 3539 2e34 2e30 372e 3535 2d2e 3137  7.59.4.07.55-.17
+00001130: 2e35 352d 2e33 3820 302d 2e31 392d 2e30  .55-.38 0-.19-.0
+00001140: 312d 2e38 322d 2e30 312d 312e 3439 2d32  1-.82-.01-1.49-2
+00001150: 2e30 312e 3337 2d32 2e35 332d 2e34 392d  .01.37-2.53-.49-
+00001160: 322e 3639 2d2e 3934 2d2e 3039 2d2e 3233  2.69-.94-.09-.23
+00001170: 2d2e 3438 2d2e 3934 2d2e 3832 2d31 2e31  -.48-.94-.82-1.1
+00001180: 332d 2e32 382d 2e31 352d 2e36 382d 2e35  3-.28-.15-.68-.5
+00001190: 322d 2e30 312d 2e35 332e 3633 2d2e 3031  2-.01-.53.63-.01
+000011a0: 2031 2e30 382e 3538 2031 2e32 332e 3832   1.08.58 1.23.82
+000011b0: 2e37 3220 312e 3231 2031 2e38 372e 3837  .72 1.21 1.87.87
+000011c0: 2032 2e33 332e 3636 2e30 372d 2e35 322e   2.33.66.07-.52.
+000011d0: 3238 2d2e 3837 2e35 312d 312e 3037 2d31  28-.87.51-1.07-1
+000011e0: 2e37 382d 2e32 2d33 2e36 342d 2e38 392d  .78-.2-3.64-.89-
+000011f0: 332e 3634 2d33 2e39 3520 302d 2e38 372e  3.64-3.95 0-.87.
+00001200: 3331 2d31 2e35 392e 3832 2d32 2e31 352d  31-1.59.82-2.15-
+00001210: 2e30 382d 2e32 2d2e 3336 2d31 2e30 322e  .08-.2-.36-1.02.
+00001220: 3038 2d32 2e31 3220 3020 3020 2e36 372d  08-2.12 0 0 .67-
+00001230: 2e32 3120 322e 322e 3832 2e36 342d 2e31  .21 2.2.82.64-.1
+00001240: 3820 312e 3332 2d2e 3237 2032 2d2e 3237  8 1.32-.27 2-.27
+00001250: 2e36 3820 3020 312e 3336 2e30 3920 3220  .68 0 1.36.09 2 
+00001260: 2e32 3720 312e 3533 2d31 2e30 3420 322e  .27 1.53-1.04 2.
+00001270: 322d 2e38 3220 322e 322d 2e38 322e 3434  2-.82 2.2-.82.44
+00001280: 2031 2e31 2e31 3620 312e 3932 2e30 3820   1.1.16 1.92.08 
+00001290: 322e 3132 2e35 312e 3536 2e38 3220 312e  2.12.51.56.82 1.
+000012a0: 3237 2e38 3220 322e 3135 2030 2033 2e30  27.82 2.15 0 3.0
+000012b0: 372d 312e 3837 2033 2e37 352d 332e 3635  7-1.87 3.75-3.65
+000012c0: 2033 2e39 352e 3239 2e32 352e 3534 2e37   3.95.29.25.54.7
+000012d0: 332e 3534 2031 2e34 3820 3020 312e 3037  3.54 1.48 0 1.07
+000012e0: 2d2e 3031 2031 2e39 332d 2e30 3120 322e  -.01 1.93-.01 2.
+000012f0: 3220 3020 2e32 312e 3135 2e34 362e 3535  2 0 .21.15.46.55
+00001300: 2e33 3841 382e 3031 3320 382e 3031 3320  .38A8.013 8.013 
+00001310: 3020 3020 3020 3136 2038 6330 2d34 2e34  0 0 0 16 8c0-4.4
+00001320: 322d 332e 3538 2d38 2d38 2d38 7a22 0a20  2-3.58-8-8-8z". 
+00001330: 2020 2020 2020 2020 203e 3c2f 7061 7468           ></path
+00001340: 3e0a 2020 2020 2020 2020 3c2f 7376 673e  >.        </svg>
+00001350: 0a20 2020 2020 203c 2f61 3e0a 2020 2020  .      </a>.    
+00001360: 2020 7b25 2d20 656e 6469 6620 2d25 7d20    {%- endif -%} 
+00001370: 7b25 2d20 656e 6469 6620 257d 0a20 2020  {%- endif %}.   
+00001380: 203c 2f64 6976 3e0a 2020 2020 7b25 2d20   </div>.    {%- 
+00001390: 656e 6469 6620 257d 0a20 203c 2f64 6976  endif %}.  </div
+000013a0: 3e0a 3c2f 6469 763e 0a3c 7363 7269 7074  >.</div>.<script
+000013b0: 2073 7263 3d22 2f2f 6172 7469 6669 6369   src="//artifici
+000013c0: 616c 686f 6e65 792e 6769 7468 7562 2e69  alhoney.github.i
+000013d0: 6f2f 686f 6e65 796d 6163 6869 6e65 2e6a  o/honeymachine.j
+000013e0: 7322 2064 6566 6572 3e3c 2f73 6372 6970  s" defer></scrip
+000013f0: 743e 0a7b 2520 656e 6462 6c6f 636b 2025  t>.{% endblock %
+00001400: 7d0a                                     }.
```

### Comparing `giger-0.1.9/docs/conf.py` & `giger-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `giger-0.1.9/docs/index.rst` & `giger-0.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `giger-0.1.9/examples/assets/fonts/AnotherTag.ttf` & `giger-0.2.0/examples/graffiti/fonts/AnotherTag.ttf`

 * *Files identical despite different names*

### Comparing `giger-0.1.9/examples/assets/fonts/Marsneveneksk.ttf` & `giger-0.2.0/examples/graffiti/fonts/Marsneveneksk.ttf`

 * *Files identical despite different names*

### Comparing `giger-0.1.9/examples/assets/fonts/MostWasted.ttf` & `giger-0.2.0/examples/graffiti/fonts/MostWasted.ttf`

 * *Files identical despite different names*

### Comparing `giger-0.1.9/examples/batch/batch.py` & `giger-0.2.0/examples/batch/batch.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,22 +8,30 @@
 
 from giger.services.image import ImageService
 from giger.services.prompt import PromptService
 from giger.services.roop import RoopService
 
 _logger = logging.getLogger(__name__)
 
+_negative_prompt = "deformed, missing limbs, amputated, pants, shorts, cat ears, bad anatomy, naked, no clothes, disfigured, poorly drawn face, mutation, mutated, ugly, disgusting, blurry, watermark, watermarked, oversaturated, obese, doubled face, b&w, black and white, sepia, nude, frekles, no masks, duplicate image, blur, paintings, sketches, lowres, monochrome, grayscale, bad anatomy, fat, facing away, looking away, tilted head, lowres, bad anatomy, bad hands, text, error, missing fingers, extra digit, fewer digits, cropped, username, blurry, bad feet, cropped, worst quality, low quality, normal quality, jpeg artifacts, signature, watermark, easy negative, glasses"
+
 
 def is_valid_file(parser, arg):
     if not os.path.exists(arg):
         parser.error("The file %s does not exist!" % arg)
     else:
         return open(arg, "r")  # return an open file handle
 
 
+def tuple_type(strings):
+    strings = strings.replace("(", "").replace(")", "")
+    mapped_int = map(int, strings.split(","))
+    return tuple(mapped_int)
+
+
 class CharacterCLI:
     def parse_args(self, args):
         """
         Parse command line parameters
         """
 
         parser = argparse.ArgumentParser(prog="batch", description="Simple batch tool")
@@ -41,28 +49,14 @@
             "--very-verbose",
             dest="loglevel",
             help="set loglevel to DEBUG",
             action="store_const",
             const=logging.DEBUG,
         )
         parser.add_argument(
-            "-a",
-            "--artist",
-            help="Artist name",
-            type=str,
-            default="H.R. Giger",
-        )
-        parser.add_argument(
-            "-t",
-            "--time",
-            help="Time description",
-            type=str,
-            default="Ancient",
-        )
-        parser.add_argument(
             "-m",
             "--model",
             help="The Stable Diffusion model to use",
             default="Lykon/DreamShaper",
         )
         parser.add_argument(
             "-o", "--output", help="Batch output", type=str, required=True
@@ -74,27 +68,37 @@
             type=str,
             default="batch",
         )
         parser.add_argument("-c", "--count", help="Batch count", default=10, type=int)
         parser.add_argument("-s", "--seed", help="Batch seed", type=int, default=0)
 
         parser.add_argument(
-            "-d", "--dimension", help="Image dimension", type=tuple, default=(768, 432)
+            "-d",
+            "--dimension",
+            help="Image dimension",
+            type=tuple_type,
+            default=(768, 432),
         )
-        parser.add_argument("-l", "--lora", help="LoRa scale", type=float, default=0.75)
+        parser.add_argument("-l", "--lora", help="LoRa scale", type=float, default=1.0)
         parser.add_argument(
             "-p",
             "--prompts",
             help="Prompts txt file",
             required=True,
             metavar="FILE",
             type=lambda x: is_valid_file(parser, x),
         )
 
-        parser.add_argument("-n", "--negative_prompt", help="Negative prompt", type=str)
+        parser.add_argument(
+            "-n",
+            "--negative_prompt",
+            help="Negative prompt",
+            type=str,
+            default=_negative_prompt,
+        )
         parser.add_argument("-f", "--face", help="Face input image", required=False)
 
         return parser.parse_args(args)
 
     def setup_logging(self, loglevel):
         """
         Setup basic logging
@@ -129,26 +133,19 @@
         path = os.path.join(args.output, args.batch_name)
         Path(path).mkdir(parents=True, exist_ok=True)
         seed = args.seed
         for description in args.prompts:
             _logger.info(f'Generating prompt for "{description}"')
             prompt = prompt_service.generate(
                 description=[description],
-                time=args.time,
-                type="Comic Book",
-                art_style=["Concept Art"],
-                artist=[args.artist],
                 realism=["Photorealistic"],
                 rendering_engine=["Octane Render"],
-                lightning_angle=["Back Light"],
                 lightning_style=["Cinematic"],
-                camera_position=["Full-Body Shot"],
-                camera_style=["Long Exposure"],
                 resolution=["8k"],
-                compel_style="subtle",
+                compel_style="full",
             )
             _logger.info(f'Running batch for "{prompt}"')
             image_service.txt2img(
                 args.model,
                 prompt,
                 args.negative_prompt,
                 path,
```

### Comparing `giger-0.1.9/examples/graffiti/app.py` & `giger-0.2.0/examples/graffiti/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,14 @@
 
 def controlnet_image():
     img = Image.new("RGB", (WIDTH, HEIGHT), "white")
     draw = ImageDraw.Draw(img)
     ttf = ImageFont.truetype(
         os.path.join(
             os.path.dirname(__file__),
-            "..",
-            "assets",
             "fonts",
             "{0}.ttf".format(font.replace(" ", "")),
         ),
         300,
     )
     draw.text((WIDTH / 2, HEIGHT / 2), tag, font=ttf, fill="black", anchor="mm")
     return img
```

### Comparing `giger-0.1.9/setup.cfg` & `giger-0.2.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,18 @@
 	=src
 install_requires = 
 	importlib-metadata; python_version<"3.8"
 	transformers
 	jinja2
 	pyyaml
 	diffusers
+	peft
+	absl-py
+	astunparse
+	array-record
 	torch
 	torchvision
 	piexif
 	accelerate
 	xformers
 	compel
 	safetensors
```

### Comparing `giger-0.1.9/setup.py` & `giger-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `giger-0.1.9/src/giger/__init__.py` & `giger-0.2.0/src/giger/__init__.py`

 * *Files identical despite different names*

### Comparing `giger-0.1.9/src/giger/cli.py` & `giger-0.2.0/src/giger/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from giger import __version__
 
 from .commands.image import ImageCommand
 from .commands.prompt import PromptCommand
 from .commands.roop import RoopCommand
 from .commands.template import TemplateCommand
+from .commands.upscale import UpscaleCommand
 
 warnings.filterwarnings("ignore", category=FutureWarning)
 
 
 __author__ = "Sebastian Krüger"
 __copyright__ = "Sebastian Krüger"
 __license__ = "MIT"
@@ -60,14 +61,15 @@
 
         subparsers = parser.add_subparsers(dest="command", required=True)
 
         self.template = TemplateCommand(subparsers)
         self.prompt = PromptCommand(subparsers)
         self.image = ImageCommand(subparsers)
         self.roop = RoopCommand(subparsers)
+        self.upscale = UpscaleCommand(subparsers)
 
         return parser.parse_args(args)
 
     def setup_logging(self, loglevel):
         """
         Setup basic logging
 
@@ -95,14 +97,16 @@
             if args.loglevel == logging.DEBUG:
                 utils.logging.set_verbosity_debug()
             elif args.loglevel == logging.INFO:
                 utils.logging.set_verbosity_info()
             else:
                 utils.logging.set_verbosity_error()
             self.image.execute(args)
+        elif args.command == "upscale":
+            self.upscale.execute(args)
         else:
             self.roop.execute(args)
 
 
 def run():
     CLI().run(sys.argv[1:])
```

### Comparing `giger-0.1.9/src/giger/commands/image.py` & `giger-0.2.0/src/giger/commands/image.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,14 +59,17 @@
         )
         self.parser.add_argument(
             "--lora_filename", help="The LoRA file name", nargs="*", default=[]
         )
         self.parser.add_argument(
             "--lora_scale", help="The LoRA scale", nargs="*", default=[], type=float
         )
+        self.parser.add_argument(
+            "--bypass_safety", help="Bypass Safety (NSFW)", action="store_true"
+        )
 
     def execute(self, args):
         if args.seed == None:
             seed = random.randint(0, 1000000)
         else:
             seed = args.seed
 
@@ -114,14 +117,15 @@
                         args.control_guidance_end,
                         args.input,
                         loras,
                         s,
                         args.batch_size,
                         args.inference_steps,
                         args.name + "-" + str(x).rjust(3, "0"),
+                        args.bypass_safety,
                     )
                 else:
                     self.service.img2img(
                         args.model,
                         prompt,
                         args.negative_prompt,
                         path,
@@ -129,22 +133,24 @@
                         args.height,
                         args.input,
                         loras,
                         s,
                         args.batch_size,
                         args.inference_steps,
                         args.name + "-" + str(x).rjust(3, "0"),
+                        args.bypass_safety,
                     )
             else:
                 self.service.txt2img(
                     args.model,
                     prompt,
                     args.negative_prompt,
                     path,
                     args.width,
                     args.height,
                     loras,
                     s,
                     args.batch_size,
                     args.inference_steps,
                     args.name + "-" + str(x).rjust(3, "0"),
+                    args.bypass_safety,
                 )
```

### Comparing `giger-0.1.9/src/giger/commands/prompt.py` & `giger-0.2.0/src/giger/commands/prompt.py`

 * *Files identical despite different names*

### Comparing `giger-0.1.9/src/giger/commands/roop.py` & `giger-0.2.0/src/giger/commands/roop.py`

 * *Files identical despite different names*

### Comparing `giger-0.1.9/src/giger/commands/template.py` & `giger-0.2.0/src/giger/commands/template.py`

 * *Files identical despite different names*

### Comparing `giger-0.1.9/src/giger/services/image.py` & `giger-0.2.0/src/giger/services/image.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,17 +8,26 @@
 from diffusers import (
     ControlNetModel,
     StableDiffusionControlNetPipeline,
     StableDiffusionImg2ImgPipeline,
     StableDiffusionPipeline,
     UniPCMultistepScheduler,
 )
+from huggingface_hub import Repository
 from PIL import Image
 
 
+def _bypass_safety(images, clip_input):
+    if len(images.shape) == 4:
+        num_images = images.shape[0]
+        return images, [False] * num_images
+    else:
+        return images, False
+
+
 class ImageService:
     def __init__(self):
         if torch.cuda.is_available():
             self.cuda = True
         else:
             self.cuda = False
 
@@ -31,16 +40,21 @@
         width,
         height,
         loras=[],
         seed=0,
         count=1,
         steps=50,
         name="txt2img",
+        bypass_safety=False,
     ):
         pipeline = self._setup_pipeline(model, StableDiffusionPipeline, loras)
+
+        if bypass_safety:
+            pipeline.safety_checker = _bypass_safety
+
         exif_bytes = self._get_exif_bytes(prompt)
         generator = self._create_generator(seed, count)
         conditioning = self._add_compel(pipeline, prompt)
         images = pipeline(
             prompt_embeds=conditioning,
             generator=generator,
             width=width,
@@ -61,16 +75,21 @@
         height,
         image,
         loras=[],
         seed=0,
         count=1,
         steps=50,
         name="img2img",
+        bypass_safety=False,
     ):
         pipeline = self._setup_pipeline(model, StableDiffusionImg2ImgPipeline, loras)
+
+        if bypass_safety:
+            pipeline.safety_checker = _bypass_safety
+
         exif_bytes = self._get_exif_bytes(prompt)
         generator = self._create_generator(seed, count)
         conditioning = self._add_compel(pipeline, prompt)
         images = pipeline(
             prompt_embeds=conditioning,
             generator=generator,
             num_images_per_prompt=count,
@@ -94,18 +113,23 @@
         control_guidance_end,
         image,
         loras=[],
         seed=0,
         count=1,
         steps=50,
         name="controlnet",
+        bypass_safety=False,
     ):
         pipeline = self._setup_pipeline(
             model, StableDiffusionControlNetPipeline, loras, controlnet_model
         )
+
+        if bypass_safety:
+            pipeline.safety_checker = _bypass_safety
+
         exif_bytes = self._get_exif_bytes(prompt)
         generator = self._create_generator(seed, count)
         # speed up diffusion process with faster scheduler and memory optimization
         pipeline.scheduler = UniPCMultistepScheduler.from_config(
             pipeline.scheduler.config
         )
         conditioning = self._add_compel(pipeline, prompt)
@@ -123,24 +147,26 @@
             control_guidance_start=control_guidance_start,
             control_guidance_end=control_guidance_end,
         )
         self._save_images(images, output, name, seed, exif_bytes)
 
     def _save_images(self, images, output, name, seed, exif_bytes=None):
         for x in range(len(list(images[0]))):
+            p = os.path.join(
+                Path(output).resolve(),
+                name
+                + "-"
+                + str(seed + x).rjust(6, "0")
+                + "-"
+                + str(x).rjust(3, "0")
+                + ".png",
+            )
+
             images[0][x].save(
-                os.path.join(
-                    Path(output).resolve(),
-                    name
-                    + "-"
-                    + str(x).rjust(3, "0")
-                    + "-"
-                    + str(seed + x).rjust(6, "0")
-                    + ".png",
-                ),
+                p,
                 exif=exif_bytes,
             )
 
     def _create_generator(self, seed, count):
         if self.cuda:
             return [
                 torch.Generator(device="cuda").manual_seed(i + seed)
@@ -181,20 +207,25 @@
         else:
             if controlnet:
                 pipeline = type.from_pretrained(
                     model, torch_dtype=torch.float32, controlnet=controlnet
                 )
             else:
                 pipeline = type.from_pretrained(model, torch_dtype=torch.float32)
+        adapters = []
         for lora_index in range(len(loras)):
-            pipeline._lora_scale = loras[lora_index]["scale"]
+            adapter = "lora" + str(lora_index)
+            adapters += [adapter]
             pipeline.load_lora_weights(
-                loras[lora_index]["model"], weight_name=loras[lora_index]["filename"]
+                loras[lora_index]["model"],
+                weight_name=loras[lora_index]["filename"],
+                adapter_name=adapter,
             )
-            pipeline._lora_scale = 1.0
+
+        pipeline.set_adapters(adapters, adapter_weights=[x["scale"] for x in loras])
 
         return pipeline
 
     def _add_compel(self, pipeline, prompt):
         compel = Compel(
             tokenizer=pipeline.tokenizer, text_encoder=pipeline.text_encoder
         )
```

### Comparing `giger-0.1.9/src/giger/services/prompt.py` & `giger-0.2.0/src/giger/services/prompt.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,15 +9,16 @@
         return [
             "Ancient",
             "Antique",
             "Futuristic",
             "Modern",
             "Old-fashioned",
             "Retro",
-            "Youthful" "{{time}}",
+            "Youthful",
+            "{{time}}",
         ]
 
     def types():
         return [
             "3D Render",
             "Abstract Painting",
             "Acrylic Painting",
@@ -125,15 +126,16 @@
             "Sand Painting",
             "Speed Painting",
             "Spray Paint",
             "Spray Painting",
             "Stained Glass",
             "Sticker",
             "Still Life Painting",
-            "Stone Cut" "Street Art",
+            "Stone Cut",
+            "Street Art",
             "Studio Ghibli Style",
             "Surrealism Painting",
             "Tanjore Painting",
             "Tempera Painting",
             "Velvet Painting",
             "Watercolor Painting",
             "Woodburning Style",
@@ -240,15 +242,16 @@
             "Thomas Kinkade",
             "Tivadar Csontváry Kosztka",
             "Victo Ngai",
             "Vincent Di Fate",
             "Vincent van Gogh",
             "Wes Anderson",
             "William Blake",
-            "Yoshitaka Amano" "Édouard Manet",
+            "Yoshitaka Amano",
+            "Édouard Manet",
             "{{artist}}",
         ]
 
     def realisms():
         return [
             "Ambient Occlusion",
             "Atmospheric",
@@ -264,15 +267,16 @@
         ]
 
     def rendering_engines():
         return [
             "Octane Render",
             "Ray Tracing",
             "Unreal Engine",
-            "V-Ray" "{{rendering_engine}}",
+            "V-Ray",
+            "{{rendering_engine}}",
         ]
 
     def lightning_angles():
         return [
             "Back Light",
             "Front Light",
             "Light From Left",
@@ -336,15 +340,15 @@
             "Fisheye",
             "Golden hour",
             "Infrared",
             "Kodachrome",
             "Long Exposure",
             "Macro",
             "Polaroid",
-            "{{style}}",
+            "{{camera_style}}",
         ]
 
     def compositions():
         return [
             "Asymetric",
             "Centered",
             "Golden Ratio",
@@ -370,34 +374,43 @@
         return [
             "{{resolution}}",
             "8k",
             "HD",
             "Full HD",
         ]
 
-    def generate(
-        self,
-        time=None,
-        type=None,
-        description=None,
-        background_color=None,
-        art_style=None,
-        artist=None,
-        realism=None,
-        rendering_engine=None,
-        lightning_angle=None,
-        lightning_style=None,
-        camera_position=None,
-        camera=None,
-        camera_style=None,
-        composition=None,
-        iso=None,
-        resolution=None,
-        compel_style=None,
-    ):
+    def generate(self, **kwargs):
+        description = kwargs["description"] if "description" in kwargs else None
+        time = kwargs["time"] if "time" in kwargs else None
+        type = kwargs["type"] if "type" in kwargs else None
+        background_color = (
+            kwargs["background_color"] if "background_color" in kwargs else None
+        )
+        art_style = kwargs["art_style"] if "art_style" in kwargs else None
+        artist = kwargs["artist"] if "artist" in kwargs else None
+        realism = kwargs["realism"] if "realism" in kwargs else None
+        rendering_engine = (
+            kwargs["rendering_engine"] if "rendering_engine" in kwargs else None
+        )
+        lightning_angle = (
+            kwargs["lightning_angle"] if "lightning_angle" in kwargs else None
+        )
+        lightning_style = (
+            kwargs["lightning_style"] if "lightning_style" in kwargs else None
+        )
+        camera_position = (
+            kwargs["camera_position"] if "camera_position" in kwargs else None
+        )
+        camera = kwargs["camera"] if "camera" in kwargs else None
+        camera_style = kwargs["camera_style"] if "camera_style" in kwargs else None
+        composition = kwargs["composition"] if "composition" in kwargs else None
+        iso = kwargs["iso"] if "iso" in kwargs else None
+        resolution = kwargs["resolution"] if "resolution" in kwargs else None
+        compel_style = kwargs["compel_style"] if "compel_style" in kwargs else None
+
         separator = ", "
 
         context = []
         prompt = []
         style = []
         image = []
```

### Comparing `giger-0.1.9/src/giger/services/roop.py` & `giger-0.2.0/src/giger/services/roop.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,23 +18,25 @@
         face_analyser.prepare(ctx_id=0, det_size=det_size)
 
         face = face_analyser.get(source)
         if len(face) == 0 and det_size[0] > 320 and det_size[1] > 320:
             det_size_half = (det_size[0] // 2, det_size[1] // 2)
             return self._get_face(source, det_size=det_size_half)
         try:
-            return sorted(face, key=lambda x: x.bbox[0])[0]
+            return sorted(face, key=lambda x: x.bbox[0])
         except:
             return None
 
     def swap(self, source, input, output, model_name=None):
         if not model_name:
             roop_dir = os.path.join(str(Path.home()), "roop")
             if not os.path.exists(roop_dir):
-                Repository(roop_dir, clone_from="henryruhs/roop", revision="main")
+                Repository(
+                    roop_dir, clone_from="ezioruan/inswapper_128.onnx", revision="main"
+                )
             model_name = os.path.join(roop_dir, "inswapper_128.onnx")
         source_image = Image.open(source).convert("RGB")
         input_image = Image.open(input).convert("RGB")
         if "exif" in input_image.info:
             exif = input_image.info["exif"]
         else:
             exif = None
@@ -48,12 +50,14 @@
             return
         model = insightface.model_zoo.get_model(
             model_name, providers=["CPUExecutionProvider"]
         )
         if model == None:
             _logger.warn('Cannot load model "{0}". Exiting.'.format(model_name))
             return
-        result = model.get(numpy.array(input_image), input_face, source_face)
+        result = numpy.array(input_image)
+        for f in list(input_face):
+            result = model.get(result, f, source_face[0])
         result_image = Image.fromarray(result)
         result_image.save(output, exif=exif) if exif != None else result_image.save(
             output
         )
```

### Comparing `giger-0.1.9/src/giger.egg-info/SOURCES.txt` & `giger-0.2.0/src/giger.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -24,57 +24,45 @@
 docs/index.rst
 docs/license.rst
 docs/readme.rst
 docs/requirements.txt
 docs/_static/.gitignore
 docs/_static/styles/custom.css
 docs/_templates/page.html
-examples/assets/fonts/AnotherTag.ttf
-examples/assets/fonts/Marsneveneksk.ttf
-examples/assets/fonts/MostWasted.ttf
-examples/assets/img/faces/johann.jpg
-examples/assets/img/faces/kevin.jpg
-examples/assets/img/faces/leif.jpg
-examples/assets/img/faces/palina.jpg
-examples/assets/img/faces/peter.jpg
-examples/assets/img/faces/zakk.jpg
-examples/assets/img/sketches/honeymachine.png
-examples/assets/img/sketches/zonk.png
-examples/assets/img/sketches/zuri.png
-examples/assets/txt/prompts/_negative.txt
-examples/assets/txt/prompts/graffiti.txt
-examples/assets/txt/prompts/gravedigger.txt
-examples/assets/txt/prompts/spawn.txt
-examples/assets/txt/prompts/viking.txt
-examples/assets/txt/prompts/vampire/ancient.txt
-examples/assets/txt/prompts/vampire/modern.txt
 examples/batch/README.rst
 examples/batch/batch.py
 examples/batch/requirements.txt
 examples/graffiti/README.rst
 examples/graffiti/app.py
 examples/graffiti/requirements.txt
+examples/graffiti/fonts/AnotherTag.ttf
+examples/graffiti/fonts/Marsneveneksk.ttf
+examples/graffiti/fonts/MostWasted.ttf
+examples/styled/requirements.txt
+examples/styled/styled.py
 requirements/test.txt
 src/giger/__init__.py
 src/giger/cli.py
 src/giger.egg-info/PKG-INFO
 src/giger.egg-info/SOURCES.txt
 src/giger.egg-info/dependency_links.txt
 src/giger.egg-info/entry_points.txt
 src/giger.egg-info/not-zip-safe
 src/giger.egg-info/requires.txt
 src/giger.egg-info/top_level.txt
 src/giger/commands/image.py
 src/giger/commands/prompt.py
 src/giger/commands/roop.py
 src/giger/commands/template.py
+src/giger/commands/upscale.py
 src/giger/services/image.py
 src/giger/services/prompt.py
 src/giger/services/roop.py
 src/giger/services/template.py
+src/giger/services/upscale.py
 tests/conftest.py
 tests/test_cli.py
 tests/commands/test_image_command.py
 tests/commands/test_prompt_command.py
 tests/commands/test_roop_command.py
 tests/commands/test_template_command.py
 tests/fixtures/face.jpg
```

### Comparing `giger-0.1.9/tests/commands/test_image_command.py` & `giger-0.2.0/tests/commands/test_image_command.py`

 * *Files identical despite different names*

### Comparing `giger-0.1.9/tests/commands/test_prompt_command.py` & `giger-0.2.0/tests/commands/test_prompt_command.py`

 * *Files identical despite different names*

### Comparing `giger-0.1.9/tests/commands/test_roop_command.py` & `giger-0.2.0/tests/commands/test_roop_command.py`

 * *Files identical despite different names*

### Comparing `giger-0.1.9/tests/commands/test_template_command.py` & `giger-0.2.0/tests/commands/test_template_command.py`

 * *Files identical despite different names*

### Comparing `giger-0.1.9/tests/fixtures/face.jpg` & `giger-0.2.0/tests/fixtures/face.jpg`

 * *Files identical despite different names*

### Comparing `giger-0.1.9/tests/fixtures/fail.jpg` & `giger-0.2.0/tests/fixtures/fail.jpg`

 * *Files identical despite different names*

### Comparing `giger-0.1.9/tests/fixtures/input.jpg` & `giger-0.2.0/tests/fixtures/input.jpg`

 * *Files identical despite different names*

### Comparing `giger-0.1.9/tests/services/test_image_service.py` & `giger-0.2.0/tests/services/test_image_service.py`

 * *Files identical despite different names*

### Comparing `giger-0.1.9/tests/services/test_prompt_service.py` & `giger-0.2.0/tests/services/test_prompt_service.py`

 * *Files identical despite different names*

### Comparing `giger-0.1.9/tests/services/test_roop_service.py` & `giger-0.2.0/tests/services/test_roop_service.py`

 * *Files identical despite different names*

### Comparing `giger-0.1.9/tests/test_cli.py` & `giger-0.2.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `giger-0.1.9/tox.ini` & `giger-0.2.0/tox.ini`

 * *Files identical despite different names*

