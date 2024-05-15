# Comparing `tmp/erpbrasil.edoc-2.8.0.tar.gz` & `tmp/erpbrasil.edoc-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erpbrasil.edoc-2.8.0.tar", last modified: Fri May 10 02:59:02 2024, max compression
+gzip compressed data, was "erpbrasil.edoc-2.9.0.tar", last modified: Wed May 15 19:14:32 2024, max compression
```

## Comparing `erpbrasil.edoc-2.8.0.tar` & `erpbrasil.edoc-2.9.0.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-05-10 02:59:02.132316 erpbrasil.edoc-2.8.0/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      511 2024-05-10 02:52:49.000000 erpbrasil.edoc-2.8.0/.bumpversion.cfg
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     2893 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/.cookiecutterrc
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      182 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/.coveragerc
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      215 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/.editorconfig
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-05-10 02:59:02.124317 erpbrasil.edoc-2.8.0/.github/
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-05-10 02:59:02.128316 erpbrasil.edoc-2.8.0/.github/workflows/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     2568 2024-05-10 00:18:43.000000 erpbrasil.edoc-2.8.0/.github/workflows/github-actions.yml
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      207 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/.github/workflows/pre-commit.yml
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      509 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/.pre-commit-config.yaml
--rw-rw-r--   0 antonio   (1000) antonio   (1000)       64 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/AUTHORS.rst
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     1180 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/CHANGELOG.rst
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     2756 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/CONTRIBUTING.rst
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     1106 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/LICENSE
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      450 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/MANIFEST.in
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     4553 2024-05-10 02:59:02.132316 erpbrasil.edoc-2.8.0/PKG-INFO
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     3137 2024-05-10 02:44:10.000000 erpbrasil.edoc-2.8.0/README.rst
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-05-10 02:59:02.128316 erpbrasil.edoc-2.8.0/ci/
--rwxrwxr-x   0 antonio   (1000) antonio   (1000)     2952 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/ci/bootstrap.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)       54 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/ci/requirements.txt
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-05-10 02:59:02.124317 erpbrasil.edoc-2.8.0/ci/templates/
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-05-10 02:59:02.124317 erpbrasil.edoc-2.8.0/ci/templates/.github/
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-05-10 02:59:02.128316 erpbrasil.edoc-2.8.0/ci/templates/.github/workflows/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     1979 2024-05-10 00:18:43.000000 erpbrasil.edoc-2.8.0/ci/templates/.github/workflows/github-actions.yml
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-05-10 02:59:02.128316 erpbrasil.edoc-2.8.0/docs/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)       28 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/docs/authors.rst
--rw-rw-r--   0 antonio   (1000) antonio   (1000)       30 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/docs/changelog.rst
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     1302 2024-05-10 02:44:18.000000 erpbrasil.edoc-2.8.0/docs/conf.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)       33 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/docs/contributing.rst
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      244 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/docs/index.rst
--rw-rw-r--   0 antonio   (1000) antonio   (1000)       94 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/docs/installation.rst
--rw-rw-r--   0 antonio   (1000) antonio   (1000)       27 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/docs/readme.rst
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-05-10 02:59:02.128316 erpbrasil.edoc-2.8.0/docs/reference/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      126 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/docs/reference/erpbrasil.edoc.rst
--rw-rw-r--   0 antonio   (1000) antonio   (1000)       66 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/docs/reference/index.rst
--rw-rw-r--   0 antonio   (1000) antonio   (1000)       29 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/docs/requirements.txt
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      109 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/docs/spelling_wordlist.txt
--rw-rw-r--   0 antonio   (1000) antonio   (1000)       83 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/docs/usage.rst
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      360 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/pyproject.toml
--rw-rw-r--   0 antonio   (1000) antonio   (1000)       99 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/requirements.txt
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      508 2024-05-10 02:59:02.132316 erpbrasil.edoc-2.8.0/setup.cfg
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     3595 2024-05-10 02:44:13.000000 erpbrasil.edoc-2.8.0/setup.py
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-05-10 02:59:02.128316 erpbrasil.edoc-2.8.0/src/
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-05-10 02:59:02.128316 erpbrasil.edoc-2.8.0/src/erpbrasil/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      245 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/__init__.py
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-05-10 02:59:02.128316 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      455 2024-05-10 02:44:20.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/__init__.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      398 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/__main__.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     6611 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/chave.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      832 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/cli.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     7386 2024-05-10 00:18:43.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/edoc.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    11114 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/mde.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     9884 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/mdfe.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    14711 2024-05-10 00:18:43.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/nfce.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    46177 2024-05-10 02:01:41.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/nfe.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     3543 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/nfse.py
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-05-10 02:59:02.132316 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/provedores/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)        0 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/provedores/__init__.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     7047 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/provedores/barueri.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     1007 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/provedores/cidades.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     2239 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/provedores/dsf.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     9943 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/provedores/ginfes.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    12459 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/provedores/issnet.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     6563 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/provedores/paulistana.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     1545 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/resposta.py
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-05-10 02:59:02.128316 erpbrasil.edoc-2.8.0/src/erpbrasil.edoc.egg-info/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     4553 2024-05-10 02:59:02.000000 erpbrasil.edoc-2.8.0/src/erpbrasil.edoc.egg-info/PKG-INFO
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     2677 2024-05-10 02:59:02.000000 erpbrasil.edoc-2.8.0/src/erpbrasil.edoc.egg-info/SOURCES.txt
--rw-rw-r--   0 antonio   (1000) antonio   (1000)        1 2024-05-10 02:59:02.000000 erpbrasil.edoc-2.8.0/src/erpbrasil.edoc.egg-info/dependency_links.txt
--rw-rw-r--   0 antonio   (1000) antonio   (1000)       60 2024-05-10 02:59:02.000000 erpbrasil.edoc-2.8.0/src/erpbrasil.edoc.egg-info/entry_points.txt
--rw-rw-r--   0 antonio   (1000) antonio   (1000)       25 2024-05-10 02:59:02.000000 erpbrasil.edoc-2.8.0/src/erpbrasil.edoc.egg-info/namespace_packages.txt
--rw-rw-r--   0 antonio   (1000) antonio   (1000)        1 2024-05-10 02:44:32.000000 erpbrasil.edoc-2.8.0/src/erpbrasil.edoc.egg-info/not-zip-safe
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      281 2024-05-10 02:59:02.000000 erpbrasil.edoc-2.8.0/src/erpbrasil.edoc.egg-info/requires.txt
--rw-rw-r--   0 antonio   (1000) antonio   (1000)       10 2024-05-10 02:59:02.000000 erpbrasil.edoc-2.8.0/src/erpbrasil.edoc.egg-info/top_level.txt
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-05-10 02:59:02.132316 erpbrasil.edoc-2.8.0/tests/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)        0 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/tests/__init__.py
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-05-10 02:59:02.128316 erpbrasil.edoc-2.8.0/tests/fixtures/
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-05-10 02:59:02.132316 erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    11491 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_cancelar_documento.yaml
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     9234 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_cancelar_documento_ginfes.yaml
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     8187 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_chave.yaml
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    11291 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_ciencia_da_operacao.yaml
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    11477 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_confirmacao_da_operacao.yaml
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     6969 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_consulta_documento.yaml
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    10324 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_consulta_documento_ginfes.yaml
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     6744 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_desconhecimento_da_operacao.yaml
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    16217 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_envia_documento.yaml
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    17539 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_envia_documento_ginfes.yaml
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     2497 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_nsu_especifico.yaml
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     6764 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_operacao_nao_realizada.yaml
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     6533 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_status_servico.yaml
--rw-rw-r--   0 antonio   (1000) antonio   (1000)   139572 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_ultimo_nsu.yaml
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     1632 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/tests/test_certificate_mixin.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     2188 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/tests/test_erpbrasil_edoc.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     2513 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/tests/test_erpbrasil_edoc_manifestacao.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     2282 2024-05-10 00:18:43.000000 erpbrasil.edoc-2.8.0/tests/test_erpbrasil_edoc_nfe.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     5936 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/tests/test_erpbrasil_edoc_nfse_ginfes.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     5431 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/tests/test_erpbrasil_edoc_nfse_paulistana.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      823 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/tests/test_erpbrasil_edoc_situacao.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     1803 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/tox.ini
+drwxr-xr-x   0 neto      (1000) neto      (1000)        0 2024-05-15 19:14:32.240163 erpbrasil.edoc-2.9.0/
+-rw-r--r--   0 neto      (1000) neto      (1000)      511 2024-05-15 18:52:11.000000 erpbrasil.edoc-2.9.0/.bumpversion.cfg
+-rw-r--r--   0 neto      (1000) neto      (1000)     2893 2024-01-23 13:14:48.000000 erpbrasil.edoc-2.9.0/.cookiecutterrc
+-rw-r--r--   0 neto      (1000) neto      (1000)      182 2024-01-23 13:14:48.000000 erpbrasil.edoc-2.9.0/.coveragerc
+-rw-r--r--   0 neto      (1000) neto      (1000)      215 2024-01-23 13:14:48.000000 erpbrasil.edoc-2.9.0/.editorconfig
+drwxr-xr-x   0 neto      (1000) neto      (1000)        0 2024-05-15 19:14:32.230163 erpbrasil.edoc-2.9.0/.github/
+drwxr-xr-x   0 neto      (1000) neto      (1000)        0 2024-05-15 19:14:32.230163 erpbrasil.edoc-2.9.0/.github/workflows/
+-rw-r--r--   0 neto      (1000) neto      (1000)     2568 2024-05-15 18:51:54.000000 erpbrasil.edoc-2.9.0/.github/workflows/github-actions.yml
+-rw-r--r--   0 neto      (1000) neto      (1000)      207 2024-01-23 13:17:03.000000 erpbrasil.edoc-2.9.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 neto      (1000) neto      (1000)      509 2024-05-15 18:51:54.000000 erpbrasil.edoc-2.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 neto      (1000) neto      (1000)       64 2024-01-23 13:14:48.000000 erpbrasil.edoc-2.9.0/AUTHORS.rst
+-rw-r--r--   0 neto      (1000) neto      (1000)     1304 2024-05-15 19:05:43.000000 erpbrasil.edoc-2.9.0/CHANGELOG.rst
+-rw-r--r--   0 neto      (1000) neto      (1000)     2756 2024-05-15 18:51:54.000000 erpbrasil.edoc-2.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 neto      (1000) neto      (1000)     1106 2024-01-23 13:17:03.000000 erpbrasil.edoc-2.9.0/LICENSE
+-rw-r--r--   0 neto      (1000) neto      (1000)      450 2024-01-23 13:17:03.000000 erpbrasil.edoc-2.9.0/MANIFEST.in
+-rw-r--r--   0 neto      (1000) neto      (1000)     4677 2024-05-15 19:14:32.240163 erpbrasil.edoc-2.9.0/PKG-INFO
+-rw-r--r--   0 neto      (1000) neto      (1000)     3137 2024-05-15 18:52:14.000000 erpbrasil.edoc-2.9.0/README.rst
+drwxr-xr-x   0 neto      (1000) neto      (1000)        0 2024-05-15 19:14:32.230163 erpbrasil.edoc-2.9.0/ci/
+-rwxr-xr-x   0 neto      (1000) neto      (1000)     2952 2024-01-23 13:17:03.000000 erpbrasil.edoc-2.9.0/ci/bootstrap.py
+-rw-r--r--   0 neto      (1000) neto      (1000)       54 2024-01-23 13:17:03.000000 erpbrasil.edoc-2.9.0/ci/requirements.txt
+drwxr-xr-x   0 neto      (1000) neto      (1000)        0 2024-05-15 19:14:32.230163 erpbrasil.edoc-2.9.0/ci/templates/
+drwxr-xr-x   0 neto      (1000) neto      (1000)        0 2024-05-15 19:14:32.230163 erpbrasil.edoc-2.9.0/ci/templates/.github/
+drwxr-xr-x   0 neto      (1000) neto      (1000)        0 2024-05-15 19:14:32.230163 erpbrasil.edoc-2.9.0/ci/templates/.github/workflows/
+-rw-r--r--   0 neto      (1000) neto      (1000)     1979 2024-05-15 18:51:54.000000 erpbrasil.edoc-2.9.0/ci/templates/.github/workflows/github-actions.yml
+drwxr-xr-x   0 neto      (1000) neto      (1000)        0 2024-05-15 19:14:32.230163 erpbrasil.edoc-2.9.0/docs/
+-rw-r--r--   0 neto      (1000) neto      (1000)       28 2024-01-23 13:14:48.000000 erpbrasil.edoc-2.9.0/docs/authors.rst
+-rw-r--r--   0 neto      (1000) neto      (1000)       30 2024-01-23 13:14:48.000000 erpbrasil.edoc-2.9.0/docs/changelog.rst
+-rw-r--r--   0 neto      (1000) neto      (1000)     1302 2024-05-15 18:52:17.000000 erpbrasil.edoc-2.9.0/docs/conf.py
+-rw-r--r--   0 neto      (1000) neto      (1000)       33 2024-01-23 13:14:48.000000 erpbrasil.edoc-2.9.0/docs/contributing.rst
+-rw-r--r--   0 neto      (1000) neto      (1000)      244 2024-01-23 13:17:03.000000 erpbrasil.edoc-2.9.0/docs/index.rst
+-rw-r--r--   0 neto      (1000) neto      (1000)       94 2024-01-23 13:14:48.000000 erpbrasil.edoc-2.9.0/docs/installation.rst
+-rw-r--r--   0 neto      (1000) neto      (1000)       27 2024-01-23 13:14:48.000000 erpbrasil.edoc-2.9.0/docs/readme.rst
+drwxr-xr-x   0 neto      (1000) neto      (1000)        0 2024-05-15 19:14:32.230163 erpbrasil.edoc-2.9.0/docs/reference/
+-rw-r--r--   0 neto      (1000) neto      (1000)      126 2024-01-23 13:14:48.000000 erpbrasil.edoc-2.9.0/docs/reference/erpbrasil.edoc.rst
+-rw-r--r--   0 neto      (1000) neto      (1000)       66 2024-01-23 13:14:48.000000 erpbrasil.edoc-2.9.0/docs/reference/index.rst
+-rw-r--r--   0 neto      (1000) neto      (1000)       29 2024-01-23 13:14:48.000000 erpbrasil.edoc-2.9.0/docs/requirements.txt
+-rw-r--r--   0 neto      (1000) neto      (1000)      109 2024-01-23 13:14:48.000000 erpbrasil.edoc-2.9.0/docs/spelling_wordlist.txt
+-rw-r--r--   0 neto      (1000) neto      (1000)       83 2024-05-15 18:51:54.000000 erpbrasil.edoc-2.9.0/docs/usage.rst
+-rw-r--r--   0 neto      (1000) neto      (1000)      360 2024-05-15 18:51:54.000000 erpbrasil.edoc-2.9.0/pyproject.toml
+-rw-r--r--   0 neto      (1000) neto      (1000)       99 2024-01-23 13:17:03.000000 erpbrasil.edoc-2.9.0/requirements.txt
+-rw-r--r--   0 neto      (1000) neto      (1000)      508 2024-05-15 19:14:32.240163 erpbrasil.edoc-2.9.0/setup.cfg
+-rw-r--r--   0 neto      (1000) neto      (1000)     3595 2024-05-15 18:52:15.000000 erpbrasil.edoc-2.9.0/setup.py
+drwxr-xr-x   0 neto      (1000) neto      (1000)        0 2024-05-15 19:14:32.230163 erpbrasil.edoc-2.9.0/src/
+drwxr-xr-x   0 neto      (1000) neto      (1000)        0 2024-05-15 19:14:32.230163 erpbrasil.edoc-2.9.0/src/erpbrasil/
+-rw-r--r--   0 neto      (1000) neto      (1000)      245 2024-01-23 13:17:03.000000 erpbrasil.edoc-2.9.0/src/erpbrasil/__init__.py
+drwxr-xr-x   0 neto      (1000) neto      (1000)        0 2024-05-15 19:14:32.230163 erpbrasil.edoc-2.9.0/src/erpbrasil/edoc/
+-rw-r--r--   0 neto      (1000) neto      (1000)      455 2024-05-15 18:52:18.000000 erpbrasil.edoc-2.9.0/src/erpbrasil/edoc/__init__.py
+-rw-r--r--   0 neto      (1000) neto      (1000)      398 2024-05-15 18:51:54.000000 erpbrasil.edoc-2.9.0/src/erpbrasil/edoc/__main__.py
+-rw-r--r--   0 neto      (1000) neto      (1000)     6611 2024-05-15 18:51:54.000000 erpbrasil.edoc-2.9.0/src/erpbrasil/edoc/chave.py
+-rw-r--r--   0 neto      (1000) neto      (1000)      832 2024-05-15 18:51:54.000000 erpbrasil.edoc-2.9.0/src/erpbrasil/edoc/cli.py
+-rw-r--r--   0 neto      (1000) neto      (1000)     7386 2024-05-15 18:51:54.000000 erpbrasil.edoc-2.9.0/src/erpbrasil/edoc/edoc.py
+-rw-r--r--   0 neto      (1000) neto      (1000)    11114 2024-05-15 18:51:54.000000 erpbrasil.edoc-2.9.0/src/erpbrasil/edoc/mde.py
+-rw-r--r--   0 neto      (1000) neto      (1000)     9884 2024-01-23 13:17:03.000000 erpbrasil.edoc-2.9.0/src/erpbrasil/edoc/mdfe.py
+-rw-r--r--   0 neto      (1000) neto      (1000)    14711 2024-05-15 18:51:54.000000 erpbrasil.edoc-2.9.0/src/erpbrasil/edoc/nfce.py
+-rw-r--r--   0 neto      (1000) neto      (1000)    47214 2024-05-15 18:51:54.000000 erpbrasil.edoc-2.9.0/src/erpbrasil/edoc/nfe.py
+-rw-r--r--   0 neto      (1000) neto      (1000)     3543 2024-01-23 13:17:03.000000 erpbrasil.edoc-2.9.0/src/erpbrasil/edoc/nfse.py
+drwxr-xr-x   0 neto      (1000) neto      (1000)        0 2024-05-15 19:14:32.230163 erpbrasil.edoc-2.9.0/src/erpbrasil/edoc/provedores/
+-rw-r--r--   0 neto      (1000) neto      (1000)        0 2024-01-23 13:14:48.000000 erpbrasil.edoc-2.9.0/src/erpbrasil/edoc/provedores/__init__.py
+-rw-r--r--   0 neto      (1000) neto      (1000)     7047 2024-05-15 18:51:54.000000 erpbrasil.edoc-2.9.0/src/erpbrasil/edoc/provedores/barueri.py
+-rw-r--r--   0 neto      (1000) neto      (1000)     1007 2024-01-23 13:17:03.000000 erpbrasil.edoc-2.9.0/src/erpbrasil/edoc/provedores/cidades.py
+-rw-r--r--   0 neto      (1000) neto      (1000)     2239 2024-01-23 13:17:03.000000 erpbrasil.edoc-2.9.0/src/erpbrasil/edoc/provedores/dsf.py
+-rw-r--r--   0 neto      (1000) neto      (1000)     9943 2024-05-15 18:51:54.000000 erpbrasil.edoc-2.9.0/src/erpbrasil/edoc/provedores/ginfes.py
+-rw-r--r--   0 neto      (1000) neto      (1000)    12459 2024-05-15 18:51:54.000000 erpbrasil.edoc-2.9.0/src/erpbrasil/edoc/provedores/issnet.py
+-rw-r--r--   0 neto      (1000) neto      (1000)     6563 2024-01-23 13:17:03.000000 erpbrasil.edoc-2.9.0/src/erpbrasil/edoc/provedores/paulistana.py
+-rw-r--r--   0 neto      (1000) neto      (1000)     1545 2024-01-23 13:17:03.000000 erpbrasil.edoc-2.9.0/src/erpbrasil/edoc/resposta.py
+drwxr-xr-x   0 neto      (1000) neto      (1000)        0 2024-05-15 19:14:32.230163 erpbrasil.edoc-2.9.0/src/erpbrasil.edoc.egg-info/
+-rw-r--r--   0 neto      (1000) neto      (1000)     4677 2024-05-15 19:14:32.000000 erpbrasil.edoc-2.9.0/src/erpbrasil.edoc.egg-info/PKG-INFO
+-rw-r--r--   0 neto      (1000) neto      (1000)     2677 2024-05-15 19:14:32.000000 erpbrasil.edoc-2.9.0/src/erpbrasil.edoc.egg-info/SOURCES.txt
+-rw-r--r--   0 neto      (1000) neto      (1000)        1 2024-05-15 19:14:32.000000 erpbrasil.edoc-2.9.0/src/erpbrasil.edoc.egg-info/dependency_links.txt
+-rw-r--r--   0 neto      (1000) neto      (1000)       60 2024-05-15 19:14:32.000000 erpbrasil.edoc-2.9.0/src/erpbrasil.edoc.egg-info/entry_points.txt
+-rw-r--r--   0 neto      (1000) neto      (1000)       25 2024-05-15 19:14:32.000000 erpbrasil.edoc-2.9.0/src/erpbrasil.edoc.egg-info/namespace_packages.txt
+-rw-r--r--   0 neto      (1000) neto      (1000)        1 2024-05-15 19:14:32.000000 erpbrasil.edoc-2.9.0/src/erpbrasil.edoc.egg-info/not-zip-safe
+-rw-r--r--   0 neto      (1000) neto      (1000)      281 2024-05-15 19:14:32.000000 erpbrasil.edoc-2.9.0/src/erpbrasil.edoc.egg-info/requires.txt
+-rw-r--r--   0 neto      (1000) neto      (1000)       10 2024-05-15 19:14:32.000000 erpbrasil.edoc-2.9.0/src/erpbrasil.edoc.egg-info/top_level.txt
+drwxr-xr-x   0 neto      (1000) neto      (1000)        0 2024-05-15 19:14:32.230163 erpbrasil.edoc-2.9.0/tests/
+-rw-r--r--   0 neto      (1000) neto      (1000)        0 2024-01-23 13:17:03.000000 erpbrasil.edoc-2.9.0/tests/__init__.py
+drwxr-xr-x   0 neto      (1000) neto      (1000)        0 2024-05-15 19:14:32.230163 erpbrasil.edoc-2.9.0/tests/fixtures/
+drwxr-xr-x   0 neto      (1000) neto      (1000)        0 2024-05-15 19:14:32.240163 erpbrasil.edoc-2.9.0/tests/fixtures/vcr_cassettes/
+-rw-r--r--   0 neto      (1000) neto      (1000)    11491 2024-01-23 13:14:48.000000 erpbrasil.edoc-2.9.0/tests/fixtures/vcr_cassettes/test_cancelar_documento.yaml
+-rw-r--r--   0 neto      (1000) neto      (1000)     9234 2024-01-23 13:14:48.000000 erpbrasil.edoc-2.9.0/tests/fixtures/vcr_cassettes/test_cancelar_documento_ginfes.yaml
+-rw-r--r--   0 neto      (1000) neto      (1000)     8187 2024-01-23 13:17:03.000000 erpbrasil.edoc-2.9.0/tests/fixtures/vcr_cassettes/test_chave.yaml
+-rw-r--r--   0 neto      (1000) neto      (1000)    11291 2024-01-23 13:17:03.000000 erpbrasil.edoc-2.9.0/tests/fixtures/vcr_cassettes/test_ciencia_da_operacao.yaml
+-rw-r--r--   0 neto      (1000) neto      (1000)    11477 2024-01-23 13:14:48.000000 erpbrasil.edoc-2.9.0/tests/fixtures/vcr_cassettes/test_confirmacao_da_operacao.yaml
+-rw-r--r--   0 neto      (1000) neto      (1000)     6969 2024-01-23 13:14:48.000000 erpbrasil.edoc-2.9.0/tests/fixtures/vcr_cassettes/test_consulta_documento.yaml
+-rw-r--r--   0 neto      (1000) neto      (1000)    10324 2024-01-23 13:14:48.000000 erpbrasil.edoc-2.9.0/tests/fixtures/vcr_cassettes/test_consulta_documento_ginfes.yaml
+-rw-r--r--   0 neto      (1000) neto      (1000)     6744 2024-01-23 13:14:48.000000 erpbrasil.edoc-2.9.0/tests/fixtures/vcr_cassettes/test_desconhecimento_da_operacao.yaml
+-rw-r--r--   0 neto      (1000) neto      (1000)    16217 2024-01-23 13:14:48.000000 erpbrasil.edoc-2.9.0/tests/fixtures/vcr_cassettes/test_envia_documento.yaml
+-rw-r--r--   0 neto      (1000) neto      (1000)    17539 2024-01-23 13:14:48.000000 erpbrasil.edoc-2.9.0/tests/fixtures/vcr_cassettes/test_envia_documento_ginfes.yaml
+-rw-r--r--   0 neto      (1000) neto      (1000)     2497 2024-01-23 13:14:48.000000 erpbrasil.edoc-2.9.0/tests/fixtures/vcr_cassettes/test_nsu_especifico.yaml
+-rw-r--r--   0 neto      (1000) neto      (1000)     6764 2024-01-23 13:14:48.000000 erpbrasil.edoc-2.9.0/tests/fixtures/vcr_cassettes/test_operacao_nao_realizada.yaml
+-rw-r--r--   0 neto      (1000) neto      (1000)     6533 2024-01-23 13:14:48.000000 erpbrasil.edoc-2.9.0/tests/fixtures/vcr_cassettes/test_status_servico.yaml
+-rw-r--r--   0 neto      (1000) neto      (1000)   139572 2024-01-23 13:17:03.000000 erpbrasil.edoc-2.9.0/tests/fixtures/vcr_cassettes/test_ultimo_nsu.yaml
+-rw-r--r--   0 neto      (1000) neto      (1000)     1632 2024-01-23 13:17:03.000000 erpbrasil.edoc-2.9.0/tests/test_certificate_mixin.py
+-rw-r--r--   0 neto      (1000) neto      (1000)     2188 2024-05-15 18:51:54.000000 erpbrasil.edoc-2.9.0/tests/test_erpbrasil_edoc.py
+-rw-r--r--   0 neto      (1000) neto      (1000)     2513 2024-05-15 18:51:54.000000 erpbrasil.edoc-2.9.0/tests/test_erpbrasil_edoc_manifestacao.py
+-rw-r--r--   0 neto      (1000) neto      (1000)     2282 2024-05-15 18:51:54.000000 erpbrasil.edoc-2.9.0/tests/test_erpbrasil_edoc_nfe.py
+-rw-r--r--   0 neto      (1000) neto      (1000)     5936 2024-05-15 18:51:54.000000 erpbrasil.edoc-2.9.0/tests/test_erpbrasil_edoc_nfse_ginfes.py
+-rw-r--r--   0 neto      (1000) neto      (1000)     5431 2024-01-23 13:14:48.000000 erpbrasil.edoc-2.9.0/tests/test_erpbrasil_edoc_nfse_paulistana.py
+-rw-r--r--   0 neto      (1000) neto      (1000)      823 2024-01-23 13:17:03.000000 erpbrasil.edoc-2.9.0/tests/test_erpbrasil_edoc_situacao.py
+-rw-r--r--   0 neto      (1000) neto      (1000)     1803 2024-05-15 18:51:54.000000 erpbrasil.edoc-2.9.0/tox.ini
```

### Comparing `erpbrasil.edoc-2.8.0/.cookiecutterrc` & `erpbrasil.edoc-2.9.0/.cookiecutterrc`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/.github/workflows/github-actions.yml` & `erpbrasil.edoc-2.9.0/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/CHANGELOG.rst` & `erpbrasil.edoc-2.9.0/CHANGELOG.rst`

 * *Files 18% similar despite different names*

```diff
@@ -50,7 +50,12 @@
 - Manifestação do Destinatário
 - Consulta Cadastro
 
 2.2.0 (2021-05-26)
 ~~~~~~~~~~~~~~~~~~
 
 - Nota Paulistana
+
+2.9.0 (2024-05-15)
+~~~~~~~~~~~~~~~~~~
+
+- Suporte para emissão de NF-e utilizando as Sefaz autorizadoras de contingência.
```

### Comparing `erpbrasil.edoc-2.8.0/CONTRIBUTING.rst` & `erpbrasil.edoc-2.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/LICENSE` & `erpbrasil.edoc-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/PKG-INFO` & `erpbrasil.edoc-2.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erpbrasil.edoc
-Version: 2.8.0
+Version: 2.9.0
 Summary: Emissão de documentos fiscais e outras obrigações (NF-E, NFS-E, MDF-E, CT-E, REINF, E-SOCIAL)
 Home-page: https://github.com/erpbrasil/erpbrasil.edoc
 Author: Luis Felipe Mileo
 Author-email: mileo@kmee.com.br
 License: MIT
 Project-URL: Documentation, https://erpbrasiledoc.readthedocs.io/
 Project-URL: Changelog, https://erpbrasiledoc.readthedocs.io/en/latest/changelog.html
@@ -174,8 +174,13 @@
 - Consulta Cadastro
 
 2.2.0 (2021-05-26)
 ~~~~~~~~~~~~~~~~~~
 
 - Nota Paulistana
 
+2.9.0 (2024-05-15)
+~~~~~~~~~~~~~~~~~~
+
+- Suporte para emissão de NF-e utilizando as Sefaz autorizadoras de contingência.
+
```

### Comparing `erpbrasil.edoc-2.8.0/README.rst` & `erpbrasil.edoc-2.9.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -17,17 +17,17 @@
     :alt: Coverage Status
     :target: https://codecov.io/github/erpbrasil/erpbrasil.edoc
 
 .. |version| image:: https://img.shields.io/pypi/v/erpbrasil.edoc.svg
     :alt: PyPI Package latest release
     :target: https://pypi.org/project/erpbrasil.edoc
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/erpbrasil/erpbrasil.edoc/v2.8.0.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/erpbrasil/erpbrasil.edoc/v2.9.0.svg
     :alt: Commits since latest release
-    :target: https://github.com/erpbrasil/erpbrasil.edoc/compare/v2.8.0...master
+    :target: https://github.com/erpbrasil/erpbrasil.edoc/compare/v2.9.0...master
 
 .. |wheel| image:: https://img.shields.io/pypi/wheel/erpbrasil.edoc.svg
     :alt: PyPI Wheel
     :target: https://pypi.org/project/erpbrasil.edoc
 
 .. |supported-versions| image:: https://img.shields.io/pypi/pyversions/erpbrasil.edoc.svg
     :alt: Supported versions
```

### Comparing `erpbrasil.edoc-2.8.0/ci/bootstrap.py` & `erpbrasil.edoc-2.9.0/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/ci/templates/.github/workflows/github-actions.yml` & `erpbrasil.edoc-2.9.0/ci/templates/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/docs/conf.py` & `erpbrasil.edoc-2.9.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 source_suffix = ".rst"
 master_doc = "index"
 project = "erpbrasil.edoc"
 year = "2019"
 author = "Luis Felipe Mileo"
 copyright = f"{year}, {author}"
-version = release = "2.8.0"
+version = release = "2.9.0"
 
 pygments_style = "trac"
 templates_path = ["."]
 extlinks = {
     "issue": ("https://github.com/erpbrasil/erpbrasil.edoc/issues/%s", "#"),
     "pr": ("https://github.com/erpbrasil/erpbrasil.edoc/pull/%s", "PR #"),
 }
```

### Comparing `erpbrasil.edoc-2.8.0/setup.py` & `erpbrasil.edoc-2.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         join(dirname(__file__), *names), encoding=kwargs.get("encoding", "utf8")
     ) as fh:
         return fh.read()
 
 
 setup(
     name="erpbrasil.edoc",
-    version="2.8.0",
+    version="2.9.0",
     license="MIT",
     description=(
         "Emissão de documentos fiscais e outras obrigações"
         " (NF-E, NFS-E, MDF-E, CT-E, REINF, E-SOCIAL)"
     ),
     long_description="{}\n{}".format(
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub(
```

### Comparing `erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/chave.py` & `erpbrasil.edoc-2.9.0/src/erpbrasil/edoc/chave.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/cli.py` & `erpbrasil.edoc-2.9.0/src/erpbrasil/edoc/cli.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/edoc.py` & `erpbrasil.edoc-2.9.0/src/erpbrasil/edoc/edoc.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/mde.py` & `erpbrasil.edoc-2.9.0/src/erpbrasil/edoc/mde.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/mdfe.py` & `erpbrasil.edoc-2.9.0/src/erpbrasil/edoc/mdfe.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/nfce.py` & `erpbrasil.edoc-2.9.0/src/erpbrasil/edoc/nfce.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/nfe.py` & `erpbrasil.edoc-2.9.0/src/erpbrasil/edoc/nfe.py`

 * *Files 5% similar despite different names*

```diff
@@ -162,22 +162,24 @@
         WS_NFE_RET_AUTORIZACAO: "NFeRetAutorizacao4/NFeRetAutorizacao4.asmx?wsdl",  # noqa
     },
 }
 
 SVC_AN = {
     AMBIENTE_PRODUCAO: {
         "servidor": "www.svc.fazenda.gov.br",
+        WS_NFE_INUTILIZACAO: "NFeInutilizacao4/NFeInutilizacao4.asmx?wsdl",
         WS_NFE_CONSULTA: "NFeConsultaProtocolo4/NFeConsultaProtocolo4.asmx?wsdl",  # noqa
         WS_NFE_SITUACAO: "NFeStatusServico4/NFeStatusServico4.asmx?wsdl",
         WS_NFE_RECEPCAO_EVENTO: "NFeRecepcaoEvento4/NFeRecepcaoEvento4.asmx?wsdl",  # noqa
         WS_NFE_AUTORIZACAO: "NFeAutorizacao4/NFeAutorizacao4.asmx?wsdl",
         WS_NFE_RET_AUTORIZACAO: "NFeRetAutorizacao4/NFeRetAutorizacao4.asmx?wsdl",  # noqa
     },
     AMBIENTE_HOMOLOGACAO: {
-        "servidor": "hom.svc.fazenda.gov.br",
+        "servidor": "hom.sefazvirtual.fazenda.gov.br",
+        WS_NFE_INUTILIZACAO: "NFeInutilizacao4/NFeInutilizacao4.asmx?wsdl",
         WS_NFE_CONSULTA: "NFeConsultaProtocolo4/NFeConsultaProtocolo4.asmx?wsdl",  # noqa
         WS_NFE_SITUACAO: "NFeStatusServico4/NFeStatusServico4.asmx?wsdl",
         WS_NFE_RECEPCAO_EVENTO: "NFeRecepcaoEvento4/NFeRecepcaoEvento4.asmx?wsdl",  # noqa
         WS_NFE_AUTORIZACAO: "NFeAutorizacao4/NFeAutorizacao4.asmx?wsdl",
         WS_NFE_RET_AUTORIZACAO: "NFeRetAutorizacao4/NFeRetAutorizacao4.asmx?wsdl",  # noqa
     },
 }
@@ -640,49 +642,57 @@
             WS_NFE_CADASTRO: "ws/cadconsultacadastro2.asmx",
             WS_NFE_RECEPCAO_EVENTO: "ws/NFeRecepcaoEvento4.asmx?wsdl",
             WS_NFCE_QR_CODE: "https://homologacao.nfce.fazenda.sp.gov.br/NFCEConsultaPublica/Paginas/ConstultaQRCode.aspx",
         },
     },
 }
 
+
+# Dicionário `ESTADO_WS` mapeia unidade federativa (UF) para uma tupla contendo
+# o serviço de webservices (WS) normal e o serviço de contingência.
+# Cada chave é uma sigla de UF e cada valor é uma tupla (servico_normal,
+# servico_contingencia). Exceção para a chave `AN` que representa o órgão de
+# Ambiente Nacional e não uma UF.
 ESTADO_WS = {
-    "AC": SVRS,
-    "AL": SVRS,
-    "AM": UFAM,
-    "AP": SVRS,
-    "BA": UFBA,
-    "CE": UFCE,
-    "DF": SVRS,
-    "ES": SVRS,
-    "GO": UFGO,
-    "MA": SVAN,
-    "MG": UFMG,
-    "MS": UFMS,
-    "MT": UFMT,
-    "PA": SVRS,
-    "PB": SVRS,
-    "PE": UFPE,
-    "PI": SVRS,
-    "PR": UFPR,
-    "RJ": SVRS,
-    "RN": SVRS,
-    "RO": SVRS,
-    "RR": SVRS,
-    "RS": UFRS,
-    "SC": SVRS,
-    "SE": SVRS,
-    "SP": UFSP,
-    "TO": SVRS,
-    "AN": AN,
+    "AC": (SVRS, SVC_AN),
+    "AL": (SVRS, SVC_AN),
+    "AM": (UFAM, SVC_RS),
+    "AP": (SVRS, SVC_AN),
+    "BA": (UFBA, SVC_RS),
+    "CE": (UFCE, SVC_AN),
+    "DF": (SVRS, SVC_AN),
+    "ES": (SVRS, SVC_AN),
+    "GO": (UFGO, SVC_RS),
+    "MA": (SVAN, SVC_RS),
+    "MG": (UFMG, SVC_AN),
+    "MS": (UFMS, SVC_RS),
+    "MT": (UFMT, SVC_RS),
+    "PA": (SVRS, SVC_AN),
+    "PB": (SVRS, SVC_AN),
+    "PE": (UFPE, SVC_RS),
+    "PI": (SVRS, SVC_RS),
+    "PR": (UFPR, SVC_RS),
+    "RJ": (SVRS, SVC_AN),
+    "RN": (SVRS, SVC_AN),
+    "RO": (SVRS, SVC_AN),
+    "RR": (SVRS, SVC_AN),
+    "RS": (UFRS, SVC_AN),
+    "SC": (SVRS, SVC_AN),
+    "SE": (SVRS, SVC_AN),
+    "SP": (UFSP, SVC_AN),
+    "TO": (SVRS, SVC_AN),
+    "AN": (AN, AN),
 }
 
 
-def localizar_url(servico, estado, mod="55", ambiente=2):
+def localizar_url(servico, estado, mod="55", ambiente=2, contingencia=False):
     sigla = SIGLA_ESTADO[estado]
-    ws = ESTADO_WS[sigla]
+
+    ws_normal, ws_contingencia = ESTADO_WS[sigla]
+    ws = ws_contingencia if contingencia else ws_normal
 
     if servico in (WS_DFE_DISTRIBUICAO, WS_DOWNLOAD_NFE):
         ws = AN
 
     if mod in ws:
         dominio = ws[mod][ambiente]["servidor"]
         complemento = ws[mod][ambiente][servico]
@@ -730,41 +740,60 @@
         self,
         transmissao,
         uf,
         versao="4.00",
         ambiente="2",
         mod="55",
         envio_sincrono=False,
+        contingencia=False,
     ):
         super().__init__(transmissao, envio_sincrono)
         self.versao = str(versao)
         self.ambiente = str(ambiente)
         self.uf = int(uf)
         self.mod = str(mod)
+        self.contingencia = contingencia
 
     def _edoc_situacao_ja_enviado(self, proc_consulta):
         if proc_consulta.resposta.cStat in ("100", "110", "150", "301", "302"):
             return True
         return False
 
+    def _get_ws_endpoint(self, service):
+        """
+        Obtém o endpoint de um webservice específico.
+
+        Esta função localiza a URL do endpoint para um dado serviço,
+        utilizando atributos da instância como a unidade federativa (UF),
+        o modelo (mod), o ambiente e a contingência.
+        """
+        endpoint = localizar_url(
+            service,
+            str(self.uf),
+            self.mod,
+            int(self.ambiente),
+            self.contingencia,
+        )
+        return endpoint
+
     def get_documento_id(self, edoc):
         return edoc.infNFe.Id[:3], edoc.infNFe.Id[3:]
 
     def status_servico(self):
         raiz = retConsStatServ.TConsStatServ(
             versao=self.versao,
             tpAmb=self.ambiente,
             cUF=self.uf,
             xServ="STATUS",
         )
         raiz.original_tagname_ = "consStatServ"
         return self._post(
             raiz,
             # 'https://hom.sefazvirtual.fazenda.gov.br/NFeStatusServico4/NFeStatusServico4.asmx?wsdl',
-            localizar_url(WS_NFE_SITUACAO, str(self.uf), self.mod, int(self.ambiente)),
+            self._get_ws_endpoint(WS_NFE_SITUACAO),
             "nfeStatusServicoNF",
             retConsStatServ,
         )
 
     def consulta_documento(self, chave):
         # NfeConsultaProtocolo
         raiz = retConsSitNFe.TConsSitNFe(
@@ -773,15 +802,15 @@
             xServ="CONSULTAR",
             chNFe=chave,
         )
         raiz.original_tagname_ = "consSitNFe"
         return self._post(
             raiz,
             # 'https://hom.sefazvirtual.fazenda.gov.br/NFeConsultaProtocolo4/NFeConsultaProtocolo4.asmx?wsdl',
-            localizar_url(WS_NFE_CONSULTA, str(self.uf), self.mod, int(self.ambiente)),
+            self._get_ws_endpoint(WS_NFE_CONSULTA),
             "nfeConsultaNF",
             retConsSitNFe,
         )
 
     def envia_documento(self, edoc):
         """
 
@@ -801,34 +830,30 @@
         )
         raiz.original_tagname_ = "enviNFe"
         xml_envio_string, xml_envio_etree = self._generateds_to_string_etree(raiz)
         xml_envio_etree.append(etree.fromstring(xml_assinado))
         return self._post(
             xml_envio_etree,
             # 'https://hom.sefazvirtual.fazenda.gov.br/NFeAutorizacao4/NFeAutorizacao4.asmx?wsdl',
-            localizar_url(
-                WS_NFE_AUTORIZACAO, str(self.uf), self.mod, int(self.ambiente)
-            ),
+            self._get_ws_endpoint(WS_NFE_AUTORIZACAO),
             "nfeAutorizacaoLote",
             retEnviNFe,
         )
 
     def envia_inutilizacao(self, evento):
         tinut = retInutNFe.TInutNFe(versao=self.versao, infInut=evento, Signature=None)
         tinut.original_tagname_ = "inutNFe"
 
         xml_assinado = self.assina_raiz(tinut, tinut.infInut.Id)
 
         xml_envio_etree = etree.fromstring(xml_assinado)
 
         return self._post(
             xml_envio_etree,
-            localizar_url(
-                WS_NFE_INUTILIZACAO, str(self.uf), self.mod, int(self.ambiente)
-            ),
+            self._get_ws_endpoint(WS_NFE_INUTILIZACAO),
             "nfeInutilizacaoNF",
             retInutNFe,
         )
 
     def consulta_recibo(self, numero=False, proc_envio=False):
         if proc_envio:
             numero = proc_envio.resposta.infRec.nRec
@@ -840,17 +865,15 @@
             versao=self.versao,
             tpAmb=self.ambiente,
             nRec=numero,
         )
         raiz.original_tagname_ = "consReciNFe"
         return self._post(
             raiz,
-            localizar_url(
-                WS_NFE_RET_AUTORIZACAO, str(self.uf), self.mod, int(self.ambiente)
-            ),
+            self._get_ws_endpoint(WS_NFE_RET_AUTORIZACAO),
             # 'ws/nferetautorizacao4.asmx'
             "nfeRetAutorizacaoLote",
             retConsReciNFe,
         )
 
     def enviar_lote_evento(self, lista_eventos, numero_lote=False):
         if not numero_lote:
@@ -867,17 +890,15 @@
             )
             evento.original_tagname_ = "evento"
             xml_assinado = self.assina_raiz(evento, evento.infEvento.Id)
             xml_envio_etree.append(etree.fromstring(xml_assinado))
 
         return self._post(
             xml_envio_etree,
-            localizar_url(
-                WS_NFE_RECEPCAO_EVENTO, str(self.uf), self.mod, int(self.ambiente)
-            ),
+            self._get_ws_endpoint(WS_NFE_RECEPCAO_EVENTO),
             "nfeRecepcaoEvento",
             retEnvEvento,
         )
 
     def cancela_documento(
         self, chave, protocolo_autorizacao, justificativa, data_hora_evento=False
     ):
@@ -1019,17 +1040,15 @@
             distNSU=distNSU,
             consNSU=consNSU,
             consChNFe=consChNFe,
         )
 
         return self._post(
             raiz,
-            localizar_url(
-                WS_DFE_DISTRIBUICAO, str(self.uf), self.mod, int(self.ambiente)
-            ),
+            self._get_ws_endpoint(WS_DFE_DISTRIBUICAO),
             "nfeDistDFeInteresse",
             retDistDFeInt,
         )
 
     def monta_processo(self, edoc, proc_envio, proc_recibo=None):
         nfe = proc_envio.envio_raiz.find("{" + self._namespace + "}NFe")
         if proc_recibo:
@@ -1087,11 +1106,11 @@
             versao="2.00",
             infCons=infCons,
         )
         raiz.original_tagname_ = "ConsCad"
 
         return self._post(
             raiz,
-            localizar_url(WS_NFE_CADASTRO, str(self.uf), self.mod, int(self.ambiente)),
+            self._get_ws_endpoint(WS_NFE_CADASTRO),
             "consultaCadastro",
             retConsCad,
         )
```

### Comparing `erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/nfse.py` & `erpbrasil.edoc-2.9.0/src/erpbrasil/edoc/nfse.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/provedores/barueri.py` & `erpbrasil.edoc-2.9.0/src/erpbrasil/edoc/provedores/barueri.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/provedores/cidades.py` & `erpbrasil.edoc-2.9.0/src/erpbrasil/edoc/provedores/cidades.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/provedores/dsf.py` & `erpbrasil.edoc-2.9.0/src/erpbrasil/edoc/provedores/dsf.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/provedores/ginfes.py` & `erpbrasil.edoc-2.9.0/src/erpbrasil/edoc/provedores/ginfes.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/provedores/issnet.py` & `erpbrasil.edoc-2.9.0/src/erpbrasil/edoc/provedores/issnet.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/provedores/paulistana.py` & `erpbrasil.edoc-2.9.0/src/erpbrasil/edoc/provedores/paulistana.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/resposta.py` & `erpbrasil.edoc-2.9.0/src/erpbrasil/edoc/resposta.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/src/erpbrasil.edoc.egg-info/PKG-INFO` & `erpbrasil.edoc-2.9.0/src/erpbrasil.edoc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erpbrasil.edoc
-Version: 2.8.0
+Version: 2.9.0
 Summary: Emissão de documentos fiscais e outras obrigações (NF-E, NFS-E, MDF-E, CT-E, REINF, E-SOCIAL)
 Home-page: https://github.com/erpbrasil/erpbrasil.edoc
 Author: Luis Felipe Mileo
 Author-email: mileo@kmee.com.br
 License: MIT
 Project-URL: Documentation, https://erpbrasiledoc.readthedocs.io/
 Project-URL: Changelog, https://erpbrasiledoc.readthedocs.io/en/latest/changelog.html
@@ -174,8 +174,13 @@
 - Consulta Cadastro
 
 2.2.0 (2021-05-26)
 ~~~~~~~~~~~~~~~~~~
 
 - Nota Paulistana
 
+2.9.0 (2024-05-15)
+~~~~~~~~~~~~~~~~~~
+
+- Suporte para emissão de NF-e utilizando as Sefaz autorizadoras de contingência.
+
```

### Comparing `erpbrasil.edoc-2.8.0/src/erpbrasil.edoc.egg-info/SOURCES.txt` & `erpbrasil.edoc-2.9.0/src/erpbrasil.edoc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_cancelar_documento.yaml` & `erpbrasil.edoc-2.9.0/tests/fixtures/vcr_cassettes/test_cancelar_documento.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_cancelar_documento_ginfes.yaml` & `erpbrasil.edoc-2.9.0/tests/fixtures/vcr_cassettes/test_cancelar_documento_ginfes.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_chave.yaml` & `erpbrasil.edoc-2.9.0/tests/fixtures/vcr_cassettes/test_chave.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_ciencia_da_operacao.yaml` & `erpbrasil.edoc-2.9.0/tests/fixtures/vcr_cassettes/test_ciencia_da_operacao.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_confirmacao_da_operacao.yaml` & `erpbrasil.edoc-2.9.0/tests/fixtures/vcr_cassettes/test_confirmacao_da_operacao.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_consulta_documento.yaml` & `erpbrasil.edoc-2.9.0/tests/fixtures/vcr_cassettes/test_consulta_documento.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_consulta_documento_ginfes.yaml` & `erpbrasil.edoc-2.9.0/tests/fixtures/vcr_cassettes/test_consulta_documento_ginfes.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_desconhecimento_da_operacao.yaml` & `erpbrasil.edoc-2.9.0/tests/fixtures/vcr_cassettes/test_desconhecimento_da_operacao.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_envia_documento.yaml` & `erpbrasil.edoc-2.9.0/tests/fixtures/vcr_cassettes/test_envia_documento.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_envia_documento_ginfes.yaml` & `erpbrasil.edoc-2.9.0/tests/fixtures/vcr_cassettes/test_envia_documento_ginfes.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_nsu_especifico.yaml` & `erpbrasil.edoc-2.9.0/tests/fixtures/vcr_cassettes/test_nsu_especifico.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_operacao_nao_realizada.yaml` & `erpbrasil.edoc-2.9.0/tests/fixtures/vcr_cassettes/test_operacao_nao_realizada.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_status_servico.yaml` & `erpbrasil.edoc-2.9.0/tests/fixtures/vcr_cassettes/test_status_servico.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_ultimo_nsu.yaml` & `erpbrasil.edoc-2.9.0/tests/fixtures/vcr_cassettes/test_ultimo_nsu.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/tests/test_certificate_mixin.py` & `erpbrasil.edoc-2.9.0/tests/test_certificate_mixin.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/tests/test_erpbrasil_edoc.py` & `erpbrasil.edoc-2.9.0/tests/test_erpbrasil_edoc.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/tests/test_erpbrasil_edoc_manifestacao.py` & `erpbrasil.edoc-2.9.0/tests/test_erpbrasil_edoc_manifestacao.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/tests/test_erpbrasil_edoc_nfe.py` & `erpbrasil.edoc-2.9.0/tests/test_erpbrasil_edoc_nfe.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/tests/test_erpbrasil_edoc_nfse_ginfes.py` & `erpbrasil.edoc-2.9.0/tests/test_erpbrasil_edoc_nfse_ginfes.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/tests/test_erpbrasil_edoc_nfse_paulistana.py` & `erpbrasil.edoc-2.9.0/tests/test_erpbrasil_edoc_nfse_paulistana.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/tests/test_erpbrasil_edoc_situacao.py` & `erpbrasil.edoc-2.9.0/tests/test_erpbrasil_edoc_situacao.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.8.0/tox.ini` & `erpbrasil.edoc-2.9.0/tox.ini`

 * *Files identical despite different names*

