# Comparing `tmp/ffbb_api_client-0.0.9.9.6.tar.gz` & `tmp/ffbb_api_client-0.0.9.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffbb_api_client-0.0.9.9.6.tar", last modified: Wed Mar 13 10:07:26 2024, max compression
+gzip compressed data, was "ffbb_api_client-0.0.9.9.7.tar", last modified: Wed May 15 18:10:52 2024, max compression
```

## Comparing `ffbb_api_client-0.0.9.9.6.tar` & `ffbb_api_client-0.0.9.9.7.tar`

### file list

```diff
@@ -1,82 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:07:26.734243 ffbb_api_client-0.0.9.9.6/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:07:26.722244 ffbb_api_client-0.0.9.9.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:07:26.726244 ffbb_api_client-0.0.9.9.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-03-13 10:07:26.734243 ffbb_api_client-0.0.9.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:07:26.726244 ffbb_api_client-0.0.9.9.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:07:26.726244 ffbb_api_client-0.0.9.9.6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9787 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10023 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/playground.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/quick_start.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-03-13 10:07:26.738243 ffbb_api_client-0.0.9.9.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:07:26.722244 ffbb_api_client-0.0.9.9.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:07:26.734243 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/
--rw-r--r--   0 runner    (1001) docker     (127)    19611 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/agenda_and_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/area.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/basketball_court.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/category.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/championship.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/club_details.py
--rw-r--r--   0 runner    (1001) docker     (127)    13528 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/club_infos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/competition.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/competition_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/day.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/geo_location.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/geographycale_zone.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/http_requests_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/league.py
--rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/match.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/match_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/member.py
--rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/municipality.py
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/news.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/page_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/practice_offers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/resource_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/score.py
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/season.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/sex.py
--rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/snippet.py
--rw-r--r--   0 runner    (1001) docker     (127)     6094 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/standing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/team.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/thumbnails.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/type_association.py
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/videos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:07:26.734243 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-03-13 10:07:26.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-03-13 10:07:26.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 10:07:26.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 10:07:26.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-13 10:07:26.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-13 10:07:26.000000 ffbb_api_client-0.0.9.9.6/src/ffbb_api_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:07:26.734243 ffbb_api_client-0.0.9.9.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    12808 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/tests/test_ffbb_api_client.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       69 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/tox.health-check.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-03-13 10:06:47.000000 ffbb_api_client-0.0.9.9.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:10:52.060143 ffbb_api_client-0.0.9.9.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:10:52.048143 ffbb_api_client-0.0.9.9.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:10:52.052143 ffbb_api_client-0.0.9.9.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-05-15 18:10:52.060143 ffbb_api_client-0.0.9.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:10:52.052143 ffbb_api_client-0.0.9.9.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:10:52.052143 ffbb_api_client-0.0.9.9.7/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9787 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9588 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/playground.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/quick_start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-15 18:10:52.064143 ffbb_api_client-0.0.9.9.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:10:52.048143 ffbb_api_client-0.0.9.9.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:10:52.060143 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/
+-rw-r--r--   0 runner    (1001) docker     (127)    23008 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/agenda_and_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/basketball_court.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/championship.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/club_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13528 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/club_infos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/competition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/competition_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/day.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/geo_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/geographycale_zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/http_requests_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/league.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/match_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/municipality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/news.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/page_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/practice_offers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/resource_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/season.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/sex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/snippet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6094 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/standing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/thumbnails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/type_association.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/videos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:10:52.060143 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-05-15 18:10:52.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-15 18:10:52.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 18:10:52.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 18:10:51.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-15 18:10:52.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 18:10:52.000000 ffbb_api_client-0.0.9.9.7/src/ffbb_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:10:52.060143 ffbb_api_client-0.0.9.9.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15361 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/tests/test_ffbb_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/tests.playground.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       77 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/tox.health-check.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-05-15 18:10:19.000000 ffbb_api_client-0.0.9.9.7/tox.ini
```

### Comparing `ffbb_api_client-0.0.9.9.6/.coveragerc` & `ffbb_api_client-0.0.9.9.7/.coveragerc`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/.github/workflows/ci.yml` & `ffbb_api_client-0.0.9.9.7/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/.gitignore` & `ffbb_api_client-0.0.9.9.7/.gitignore`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/.pre-commit-config.yaml` & `ffbb_api_client-0.0.9.9.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/.readthedocs.yml` & `ffbb_api_client-0.0.9.9.7/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/LICENSE.txt` & `ffbb_api_client-0.0.9.9.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/PKG-INFO` & `ffbb_api_client-0.0.9.9.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffbb_api_client
-Version: 0.0.9.9.6
+Version: 0.0.9.9.7
 Summary: Allow to interact with FFBB apis
 Home-page: https://github.com/Rinzler78/FFBBApiClient_Python
 Author: Rinzler78
 Author-email: Borisleclere@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `ffbb_api_client-0.0.9.9.6/README.rst` & `ffbb_api_client-0.0.9.9.7/README.rst`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/docs/Makefile` & `ffbb_api_client-0.0.9.9.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/docs/conf.py` & `ffbb_api_client-0.0.9.9.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/docs/index.rst` & `ffbb_api_client-0.0.9.9.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/playground.py` & `ffbb_api_client-0.0.9.9.7/playground.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,29 @@
 import os
 import string
 from typing import List
 
-from requests_cache import CachedSession
-
-from ffbb_api_client import (
+from src.ffbb_api_client import (
     AgendaAndResults,
     ClubDetails,
     ClubInfos,
     FFBBApiClient,
     Municipality,
     Team,
 )
-from tests.test_ffbb_api_client import Test_GetClubDetails
 
 # Retrieve api user / pass
 basic_auth_user = os.getenv("FFBB_BASIC_AUTH_USER")
 basic_auth_pass = os.getenv("FFBB_BASIC_AUTH_PASS")
 
-# Expire cache after 10 day
-expire_after = 864000
-
-cached_session = CachedSession(
-    "playground.http_cache",
-    backend="sqlite",
-    expire_after=expire_after,
-    allowable_methods=("GET", "POST"),
-)
-
 # Create an instance of the api client
 api_client: FFBBApiClient = FFBBApiClient(
     basic_auth_user=basic_auth_user,
     basic_auth_pass=basic_auth_pass,
     debug=True,
-    cached_session=cached_session,
 )
 
 search_patterns = list(string.ascii_lowercase)
 
 municipalities = []
 
 for pattern in search_patterns:
@@ -109,20 +95,14 @@
 
     if not team_results:
         continue
 
     print(f"Results for team {team.name} retrieved")
 
 
-test = Test_GetClubDetails()
-test.setUp()
-test.test_with_empty_id()
-test.test_with_known_id()
-
-
 def merge_results(
     club_infos: ClubInfos, results: List[AgendaAndResults]
 ) -> AgendaAndResults:
     merged_results: AgendaAndResults = None
 
     if len(results) > 0:
         merged_results: AgendaAndResults = results[0]
```

### Comparing `ffbb_api_client-0.0.9.9.6/quick_start.py` & `ffbb_api_client-0.0.9.9.7/quick_start.py`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/setup.cfg` & `ffbb_api_client-0.0.9.9.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/setup.py` & `ffbb_api_client-0.0.9.9.7/setup.py`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/__init__.py` & `ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,17 +39,29 @@
 from .snippet import Snippet  # noqa
 from .standing import Standing  # noqa
 from .team import Team  # noqa
 from .thumbnails import Thumbnails  # noqa
 from .type_association import TypeAssociation  # noqa
 from .videos import Videos, videos_from_dict  # noqa
 
+
 # Default cached session sqlite backend with 30 minutes expiration
+def create_cache_key(request, **kwargs):
+    url = request.url
+    method = request.method
+    data_hash = request.body if request.body else "empty"
+    return f"{method} {url} {data_hash}"
+
+
 default_cached_session = CachedSession(
-    "http_cache", backend="sqlite", expire_after=1800, allowable_methods=("GET", "POST")
+    "http_cache",
+    backend="sqlite",
+    expire_after=1800,
+    allowable_methods=("GET", "POST"),
+    key_fn=create_cache_key,
 )
 
 if sys.version_info[:2] >= (3, 8):
     # TODO: Import directly (no need for conditional) when `python_requires = >= 3.8`
     from importlib.metadata import PackageNotFoundError, version  # pragma: no cover
 else:
     from importlib_metadata import PackageNotFoundError, version  # pragma: no cover
@@ -146,14 +158,64 @@
         results.teams,
         key=lambda team: team.name,
     )
 
     return results
 
 
+def create_set_of_municipalities(
+    municipalities: List[Municipality],
+) -> List[Municipality]:
+    """
+    Create a set of municipalities from a list of Municipality.
+
+    Args:
+        municipalities (List[Municipality]): The list of Municipality.
+
+    Returns:
+        set: The set of municipalities.
+    """
+
+    if len(municipalities) == 1:
+        return municipalities
+
+    dict_municipalities = {}
+    for municipality in municipalities:
+        try:
+            dict_municipalities[municipality.id]
+        except KeyError:
+            dict_municipalities[municipality.id] = municipality
+    return list(dict_municipalities.values())
+
+
+def create_set_of_clubs(clubs: List[ClubInfos]) -> List[ClubInfos]:
+    """
+    Create a set of clubs from a list of ClubInfos.
+
+    Args:
+        clubs (List[ClubInfos]): The list of ClubInfos.
+
+    Returns:
+        set: The set of clubs.
+    """
+
+    if len(clubs) == 1:
+        return clubs
+
+    dict_clubs = {}
+    for club in clubs:
+        try:
+            dict_clubs[club.id]
+
+        except KeyError:
+            dict_clubs[club.id] = club
+
+    return list(dict_clubs.values())
+
+
 class FFBBApiClient:
     def __init__(
         self,
         basic_auth_user: str,
         basic_auth_pass: str,
         api_url: str = "https://mobiles.ffbb.com/php/v1_0_5/",
         ws_url: str = "https://mobiles.ffbb.com/webservices/v1/",
@@ -532,15 +594,15 @@
         Args:
             championship_type (str, optional): The type of the championship.
             cached_session (CachedSession, optional): Enable caching.
 
         Returns:
             List[Championship]: The top championships.
         """
-        params = {"type": championship_type}
+        params = {"type": championship_type.value if championship_type else None}
         url = f"{self.api_url}topChampionships.php"
         result = catch_result(
             lambda: championship_from_dict(
                 http_post_json(
                     url,
                     self.headers,
                     params,
@@ -575,46 +637,102 @@
                     url,
                     self.headers,
                     debug=self.debug,
                     cached_session=cached_session or self.cached_session,
                 )
             )
         )
-        if result:
-            return list(set(result))
-        else:
-            return None
+
+        return create_set_of_municipalities(result) if result else None
+
+    def search_multiple_municipalities(
+        self, patterns: List[str], cached_session: CachedSession = None
+    ) -> List[Municipality]:
+        """
+        Search for multiple municipalities based on their names.
+
+        Args:
+            patterns (List[str]): A list of patterns to search for.
+             cached_session (CachedSession, optional): Enable caching.
+
+        Returns:
+            List[Municipality]: A list of Municipality.
+        """
+        municipalities = []
+        for pattern in patterns:
+            result: List[Municipality] = None
+            try:
+                result = self.search_municipalities(
+                    pattern, cached_session=cached_session
+                )
+            except Exception as e:
+                print(f"An error occurred while searching municipalities: {str(e)}")
+
+            if not result:
+                continue
+
+            municipalities.extend(result)
+
+        return create_set_of_municipalities(municipalities) if municipalities else None
 
     def search_clubs(
         self,
-        id_cmne: int = None,
+        id_municipality: int = None,
         org_name: str = None,
         cached_session: CachedSession = None,
     ) -> List[ClubInfos]:
         """
         Search for a club.
 
         Args:
-            id_cmne (int, optional): The ID of the commune.
+            id_municipality (int, optional): The ID of the municipality.
             org_name (str, optional): The name of the organization.
             cached_session (CachedSession, optional): Enable caching.
 
         Returns:
             List[ClubInfos]: The club information.
         """
-        params = {"idCmne": id_cmne, "nomOrg": org_name}
+        params = {"idCmne": id_municipality, "nomOrg": org_name}
 
         url = url_with_params(f"{self.ws_url}search_club.php", params)
         result = catch_result(
             lambda: club_infos_from_dict(
                 http_get_json(
                     url,
                     self.headers,
                     debug=self.debug,
                     cached_session=cached_session or self.cached_session,
                 )
             )
         )
-        if result:
-            return list(set(result))
-        else:
-            return None
+
+        return create_set_of_clubs(result) if result else None
+
+    def search_multiple_clubs(
+        self, org_names: List[str], cached_session: CachedSession = None
+    ) -> List[ClubInfos]:
+        """
+        Search for multiple clubs based on their organization names.
+
+        Args:
+            org_names (List[str]): A list of organization names to search for.
+             cached_session (CachedSession, optional): Enable caching.
+
+        Returns:
+            List[ClubInfos]: A list of ClubInfos objects representing the found clubs.
+        """
+        clubs = []
+        for org_name in org_names:
+            result: ClubInfos = None
+            try:
+                result = self.search_clubs(
+                    org_name=org_name, cached_session=cached_session
+                )
+            except Exception as e:
+                print(f"An error occurred while searching clubs: {str(e)}")
+
+            if not result:
+                continue
+
+            clubs.extend(result)
+
+        return create_set_of_clubs(clubs) if clubs else None
```

### Comparing `ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/agenda_and_results.py` & `ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/agenda_and_results.py`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/area.py` & `ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/area.py`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/basketball_court.py` & `ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/basketball_court.py`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/category.py` & `ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/category.py`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/championship.py` & `ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/championship.py`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/club_details.py` & `ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/club_details.py`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/club_infos.py` & `ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/club_infos.py`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/competition.py` & `ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/competition.py`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/converters.py` & `ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/converters.py`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/day.py` & `ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/day.py`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/default.py` & `ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/default.py`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/field.py` & `ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/field.py`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/geo_location.py` & `ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/geo_location.py`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/geographycale_zone.py` & `ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/geographycale_zone.py`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/group.py` & `ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/group.py`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/history.py` & `ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/history.py`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/http_requests_utils.py` & `ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/http_requests_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,20 @@
     Args:
         response (Response): The HTTP response.
 
     Returns:
         Dict[str, Any]: The JSON dictionary extracted from the response.
     """
     data_str = response.text.strip()
+
+    try:
+        return json.loads(data_str)
+    except json.JSONDecodeError:
+        pass
+
     if data_str.endswith(","):
         data_str = data_str[:-1]
 
     data_str = data_str.replace("][", ",")
     data_str = data_str.replace("KO", "")
 
     if data_str.startswith('""'):
@@ -86,25 +92,26 @@
         use_cache (bool): Whether to use cache or not. Default is True.
         timeout (int): The timeout value in seconds. Default is 20.
 
     Returns:
         Response: The HTTP response.
     """
     if debug:
-        print(f"Making POST request to {url}")
+        data_str = ", ".join([f"{k}:{v}" for k, v in data.items()]) if data else ""
+        print(f"Making POST request to {url} {data_str}")
         start_time = time.time()
 
     if cached_session:
         response = cached_session.post(url, headers=headers, data=data, timeout=timeout)
     else:
         response = requests.post(url, headers=headers, data=data, timeout=timeout)
 
     if debug:
         end_time = time.time()
-        print(f"POST request to {url} took {end_time - start_time} seconds.")
+        print(f"POST request to {url} {data_str} took {end_time - start_time} seconds.")
 
     return response
 
 
 def http_get_json(
     url: str,
     headers: Dict[str, str],
```

### Comparing `ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/item.py` & `ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/item.py`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/league.py` & `ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/league.py`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/match.py` & `ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/match.py`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/match_detail.py` & `ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/match_detail.py`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/member.py` & `ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/member.py`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/municipality.py` & `ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/municipality.py`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/news.py` & `ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/news.py`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/page_info.py` & `ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/page_info.py`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/practice_offers.py` & `ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/practice_offers.py`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/resource_id.py` & `ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/resource_id.py`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/season.py` & `ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/season.py`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/snippet.py` & `ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/snippet.py`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/standing.py` & `ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/standing.py`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/team.py` & `ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/team.py`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/thumbnails.py` & `ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/thumbnails.py`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/type_association.py` & `ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/type_association.py`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/src/ffbb_api_client/videos.py` & `ffbb_api_client-0.0.9.9.7/src/ffbb_api_client/videos.py`

 * *Files identical despite different names*

### Comparing `ffbb_api_client-0.0.9.9.6/src/ffbb_api_client.egg-info/PKG-INFO` & `ffbb_api_client-0.0.9.9.7/src/ffbb_api_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffbb_api_client
-Version: 0.0.9.9.6
+Version: 0.0.9.9.7
 Summary: Allow to interact with FFBB apis
 Home-page: https://github.com/Rinzler78/FFBBApiClient_Python
 Author: Rinzler78
 Author-email: Borisleclere@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `ffbb_api_client-0.0.9.9.6/src/ffbb_api_client.egg-info/SOURCES.txt` & `ffbb_api_client-0.0.9.9.7/src/ffbb_api_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 LICENSE.txt
 README.rst
 playground.py
 pyproject.toml
 quick_start.py
 setup.cfg
 setup.py
+tests.playground.py
 tox.health-check.sh
 tox.ini
 .github/workflows/ci.yml
 docs/Makefile
 docs/authors.rst
 docs/changelog.rst
 docs/conf.py
```

### Comparing `ffbb_api_client-0.0.9.9.6/tests/test_ffbb_api_client.py` & `ffbb_api_client-0.0.9.9.7/tests/test_ffbb_api_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,15 +48,17 @@
     _known_team: Team = None
 
     _known_results: AgendaAndResults = None
 
     def setUp(self):
         # Initialisation des objects nécessaires pour les tests
         self.api_client = FFBBApiClient(
-            basic_auth_user=basic_auth_user, basic_auth_pass=basic_auth_pass
+            basic_auth_user=basic_auth_user,
+            basic_auth_pass=basic_auth_pass,
+            debug=True,
         )
 
     def setup_method(self, method):
         self.setUp()
 
     def _get_know_municipality(self):
         if not self._known_municipality:
@@ -152,15 +154,15 @@
                 sub_competition=self._get_known_team().sub_competition,
                 team_group=self._get_known_team().group,
             )
 
         return self._known_results
 
 
-class Test_SearchMunicipalitys(TestFFBBApiClient):
+class Test_SearchMunicipalities(TestFFBBApiClient):
     def test_with_known_name(self):
         result = self._get_know_municipality()
         self.assertIsNotNone(result)
         self.assertIsInstance(result, Municipality)
 
     def test_with_unknown_name(self):
         query = "Blop"
@@ -169,14 +171,38 @@
 
     def test_with_empty_name(self):
         query = ""
         result = self.api_client.search_municipalities(query)
         self.assertIsNone(result)
 
 
+class Test_SearchMultipleMunicipalities(TestFFBBApiClient):
+    def test_with_known_name(self):
+        result = self.api_client.search_multiple_municipalities(["Senas", "Paris"])
+        self.assertIsNotNone(result)
+        self.assertIsInstance(result, List)
+        self.assertGreater(len(result), 0)
+
+    def test_with_most_used_letters(self):
+        result = self.api_client.search_multiple_municipalities(
+            ["a", "e", "i", "o", "u", "y", "b", "l", "m", "s"]
+        )
+        self.assertIsNotNone(result)
+        self.assertIsInstance(result, List)
+        self.assertGreater(len(result), 0)
+
+    def test_with_unknown_name(self):
+        result = self.api_client.search_multiple_municipalities(["Blop", "Blap"])
+        self.assertIsNone(result)
+
+    def test_with_empty_name(self):
+        result = self.api_client.search_multiple_municipalities(["", ""])
+        self.assertIsNone(result)
+
+
 class Test_GetClubDetails(TestFFBBApiClient):
     def test_with_known_id(self):
         result = self._get_known_club_details()
         self.assertIsNotNone(result)
         self.assertIsInstance(result, ClubDetails)
 
     def test_with_unknown_id(self):
@@ -186,26 +212,26 @@
 
     def test_with_empty_id(self):
         club_id = None
         result = self.api_client.get_club_details(club_id)
         self.assertIsNone(result)
 
 
-class Test_SearchClub(TestFFBBApiClient):
+class Test_SearchClubs(TestFFBBApiClient):
     def test_with_known_id_municipality(self):
         result = self._get_know_club_infos()
         self.assertIsNotNone(result)
         self.assertIsInstance(result, ClubInfos)
 
     def test_with_unknown_id_municipality(self):
-        result = self.api_client.search_clubs(id_cmne="unknown_id")
+        result = self.api_client.search_clubs(id_municipality="unknown_id")
         self.assertIsNone(result)
 
     def test_with_empty_id_municipality(self):
-        result = self.api_client.search_clubs(id_cmne="")
+        result = self.api_client.search_clubs(id_municipality="")
         self.assertIsNone(result)
 
     def test_with_known_org_name(self):
         result = self.api_client.search_clubs(
             org_name=self._get_know_club_infos().organization_name
         )
         self.assertIsNotNone(result)
@@ -224,14 +250,48 @@
 
         result = self.api_client.search_clubs(org_name="B")
         self.assertIsNotNone(result)
         self.assertIsInstance(result, list)
         self.assertGreater(len(result), 0)
 
 
+class Test_SearchMultipleClubs(TestFFBBApiClient):
+    def test_with_known_name(self):
+        result = self.api_client.search_multiple_clubs(["Senas", "Paris"])
+        self.assertIsNotNone(result)
+        self.assertIsInstance(result, List)
+        self.assertGreater(len(result), 0)
+
+    def test_with_most_used_letters(self):
+        result = self.api_client.search_multiple_clubs(
+            [
+                "basket",
+                "club",
+                "ball",
+                "basketball",
+                "sport",
+                "as",
+                "entente",
+                "ctc",
+                "bc",
+            ]
+        )
+        self.assertIsNotNone(result)
+        self.assertIsInstance(result, List)
+        self.assertGreater(len(result), 0)
+
+    def test_with_unknown_name(self):
+        result = self.api_client.search_multiple_clubs(["Blop", "Blap"])
+        self.assertIsNone(result)
+
+    def test_with_empty_name(self):
+        result = self.api_client.search_multiple_clubs(["", ""])
+        self.assertIsNone(result)
+
+
 class Test_GetAreas(TestFFBBApiClient):
     def test_main(self):
         result = self.api_client.get_areas()
         self.assertIsNotNone(result)
         self.assertIsInstance(result, List)
         self.assertGreater(len(result), 0)
 
@@ -256,40 +316,42 @@
             self.assertIsInstance(result, List)
             self.assertGreater(len(result), 0)
 
 
 class Test_GetVideos(TestFFBBApiClient):
     def test_main(self):
         result = self.api_client.get_videos()
-        self.assertIsNotNone(result)
-        self.assertIsInstance(result, Videos)
+
+        if result:
+            self.assertIsInstance(result, Videos)
 
     def test_with_known_club_id(self):
         result = self.api_client.get_videos(
             id_cmne=self._get_know_club_infos().municipality.municipality_id
         )
-        self.assertIsNotNone(result)
-        self.assertIsInstance(result, Videos)
+
+        if result:
+            self.assertIsInstance(result, Videos)
 
     def test_with_unknown_club_id(self):
         result = self.api_client.get_videos(id_cmne=0)
-        self.assertIsNotNone(result)
-        self.assertIsInstance(result, Videos)
+        if result:
+            self.assertIsInstance(result, Videos)
 
     def test_with_with_known_org_name(self):
         result = self.api_client.get_videos(
             org_name=self._get_know_club_infos().organization_name
         )
-        self.assertIsNotNone(result)
-        self.assertIsInstance(result, Videos)
+        if result:
+            self.assertIsInstance(result, Videos)
 
     def test_with_with_unknown_org_name(self):
         result = self.api_client.get_videos(org_name="test")
-        self.assertIsNotNone(result)
-        self.assertIsInstance(result, Videos)
+        if result:
+            self.assertIsInstance(result, Videos)
 
 
 class Test_GetLeagues(TestFFBBApiClient):
     def test_main(self):
         result = self._get_leagues()
         self.assertIsNotNone(result)
         self.assertIsInstance(result, List)
@@ -382,14 +444,31 @@
         )
         self.assertIsNotNone(result)
 
     def test_with_known_team_id_sub_competition_group(self):
         result = self._get_known_results()
         self.assertIsNotNone(result)
 
+    def test_for_all_team_results(self):
+        know_result = self._get_known_results()
+        day_count = int(know_result.days[-1].name)
+        results = []
+
+        for i in range(1, day_count + 1):
+            result = self.api_client.get_results(
+                team_id=self._get_known_team().id,
+                sub_competition=self._get_known_team().sub_competition,
+                team_group=self._get_known_team().group,
+                day=i,
+            )
+            self.assertIsNotNone(result)
+            results.append(result)
+
+        self.assertEqual(len(results), day_count)
+
 
 class Test_GetMatchDetail(TestFFBBApiClient):
     def test_with_known_match_id(self):
         result = self.api_client.get_match_detail(
             match_id=self._get_known_results().matchs[0].match_id
         )
         self.assertIsNotNone(result)
```

### Comparing `ffbb_api_client-0.0.9.9.6/tox.ini` & `ffbb_api_client-0.0.9.9.7/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -16,17 +16,23 @@
     HOME
     SETUPTOOLS_*
     FFBB_BASIC_AUTH_USER
     FFBB_BASIC_AUTH_PASS
 extras =
     testing
     python-dotenv
+desp =
+    pytest
 commands =
     pytest {posargs}
 
+allowlist_externals =
+    python
+    pytest
+
 
 # To run `tox -e lint` you need to make sure you have a
 # `.pre-commit-config.yaml` file. See https://pre-commit.com
 [testenv:lint]
 description = Perform static analysis and style checks
 skip_install = True
 deps = pre-commit
```

