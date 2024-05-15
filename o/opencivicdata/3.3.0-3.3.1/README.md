# Comparing `tmp/opencivicdata-3.3.0.tar.gz` & `tmp/opencivicdata-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencivicdata-3.3.0.tar", last modified: Tue May 16 15:59:36 2023, max compression
+gzip compressed data, was "opencivicdata-3.3.1.tar", last modified: Wed May 15 18:54:41 2024, max compression
```

## Comparing `opencivicdata-3.3.0.tar` & `opencivicdata-3.3.1.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:36.010058 opencivicdata-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      624 2023-05-16 15:59:36.010058 opencivicdata-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      851 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:35.994058 opencivicdata-3.3.0/opencivicdata/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6495 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/common.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:35.998058 opencivicdata-3.3.0/opencivicdata/core/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:35.998058 opencivicdata-3.3.0/opencivicdata/core/admin/
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1599 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/admin/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2888 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/admin/organization.py
--rw-r--r--   0 runner    (1001) docker     (122)     1918 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/admin/other.py
--rw-r--r--   0 runner    (1001) docker     (122)     2689 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/admin/person.py
--rw-r--r--   0 runner    (1001) docker     (122)      188 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:35.998058 opencivicdata-3.3.0/opencivicdata/core/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:35.998058 opencivicdata-3.3.0/opencivicdata/core/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2623 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/management/commands/loaddivisions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:35.998058 opencivicdata-3.3.0/opencivicdata/core/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)    33372 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)      437 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/migrations/0002_post_maximum_memberships.py
--rw-r--r--   0 runner    (1001) docker     (122)    41542 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/migrations/0003_field_docs.py
--rw-r--r--   0 runner    (1001) docker     (122)     3559 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/migrations/0004_auto_20171005_2028.py
--rw-r--r--   0 runner    (1001) docker     (122)     1097 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/migrations/0005_auto_20191031_1507.py
--rw-r--r--   0 runner    (1001) docker     (122)     1081 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/migrations/0005_auto_20191124_1658.py
--rw-r--r--   0 runner    (1001) docker     (122)      267 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/migrations/0006_merge_20200103_1432.py
--rw-r--r--   0 runner    (1001) docker     (122)     1575 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/migrations/0007_jurisdiction_last_seen_membership_last_seen_and_more.py
--rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/migrations/0008_auto_20221215_1132.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:36.002058 opencivicdata-3.3.0/opencivicdata/core/models/
--rw-r--r--   0 runner    (1001) docker     (122)      480 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4661 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/models/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     4901 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/models/division.py
--rw-r--r--   0 runner    (1001) docker     (122)     1677 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/models/jurisdiction.py
--rw-r--r--   0 runner    (1001) docker     (122)    16752 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/core/models/people_orgs.py
--rw-r--r--   0 runner    (1001) docker     (122)     3023 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/divisions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:36.002058 opencivicdata-3.3.0/opencivicdata/elections/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:36.002058 opencivicdata-3.3.0/opencivicdata/elections/admin/
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/admin/candidacy.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:36.002058 opencivicdata-3.3.0/opencivicdata/elections/admin/contests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/admin/contests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3250 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/admin/contests/ballot_measure.py
--rw-r--r--   0 runner    (1001) docker     (122)     1733 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/admin/contests/candidate.py
--rw-r--r--   0 runner    (1001) docker     (122)     1428 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/admin/contests/party.py
--rw-r--r--   0 runner    (1001) docker     (122)     1171 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/admin/election.py
--rw-r--r--   0 runner    (1001) docker     (122)      198 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:36.002058 opencivicdata-3.3.0/opencivicdata/elections/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)    42827 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)      657 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/migrations/0002_auto_20170731_2047.py
--rw-r--r--   0 runner    (1001) docker     (122)      398 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/migrations/0003_election_fk.py
--rw-r--r--   0 runner    (1001) docker     (122)    12472 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/migrations/0004_field_docs.py
--rw-r--r--   0 runner    (1001) docker     (122)     3059 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/migrations/0005_auto_20170823_1648.py
--rw-r--r--   0 runner    (1001) docker     (122)     2269 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/migrations/0006_auto_20171005_2029.py
--rw-r--r--   0 runner    (1001) docker     (122)     6210 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/migrations/0007_auto_20171022_0234.py
--rw-r--r--   0 runner    (1001) docker     (122)     1944 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/migrations/0008_auto_20181029_1527.py
--rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/migrations/0009_auto_20221208_1041.py
--rw-r--r--   0 runner    (1001) docker     (122)     1756 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/migrations/0010_auto_20221215_1132.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:36.002058 opencivicdata-3.3.0/opencivicdata/elections/models/
--rw-r--r--   0 runner    (1001) docker     (122)      718 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3645 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/models/candidacy.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:36.006058 opencivicdata-3.3.0/opencivicdata/elections/models/contests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/models/contests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6084 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/models/contests/ballot_measure.py
--rw-r--r--   0 runner    (1001) docker     (122)     1726 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/models/contests/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3970 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/models/contests/candidate.py
--rw-r--r--   0 runner    (1001) docker     (122)     2929 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/models/contests/party.py
--rw-r--r--   0 runner    (1001) docker     (122)     2705 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/elections/models/election.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:36.006058 opencivicdata-3.3.0/opencivicdata/legislative/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:36.006058 opencivicdata-3.3.0/opencivicdata/legislative/admin/
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3877 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/admin/bill.py
--rw-r--r--   0 runner    (1001) docker     (122)     2879 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/admin/event.py
--rw-r--r--   0 runner    (1001) docker     (122)     1827 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/admin/vote.py
--rw-r--r--   0 runner    (1001) docker     (122)      202 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:36.006058 opencivicdata-3.3.0/opencivicdata/legislative/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)    44134 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)      769 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/migrations/0002_more_extras.py
--rw-r--r--   0 runner    (1001) docker     (122)     1714 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/migrations/0003_time_changes.py
--rw-r--r--   0 runner    (1001) docker     (122)     5477 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/migrations/0004_auto_20171005_2027.py
--rw-r--r--   0 runner    (1001) docker     (122)     6798 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/migrations/0005_auto_20171005_2028.py
--rw-r--r--   0 runner    (1001) docker     (122)      484 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/migrations/0006_billversion_extras.py
--rw-r--r--   0 runner    (1001) docker     (122)      484 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/migrations/0007_auto_20181029_1527.py
--rw-r--r--   0 runner    (1001) docker     (122)      299 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/migrations/0008_longer_event_name.py
--rw-r--r--   0 runner    (1001) docker     (122)     1832 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/migrations/0009_searchablebill.py
--rw-r--r--   0 runner    (1001) docker     (122)     1793 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/migrations/0010_auto_20191031_1507.py
--rw-r--r--   0 runner    (1001) docker     (122)      606 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/migrations/0011_auto_20191124_1658.py
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/migrations/0012_billdocument_extras.py
--rw-r--r--   0 runner    (1001) docker     (122)      472 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/migrations/0013_auto_20200326_0458.py
--rw-r--r--   0 runner    (1001) docker     (122)     1035 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/migrations/0014_bill_last_seen_event_last_seen_voteevent_last_seen.py
--rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/migrations/0015_auto_20221215_1132.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:36.010058 opencivicdata-3.3.0/opencivicdata/legislative/models/
--rw-r--r--   0 runner    (1001) docker     (122)      678 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7735 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/models/bill.py
--rw-r--r--   0 runner    (1001) docker     (122)     6998 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/models/event.py
--rw-r--r--   0 runner    (1001) docker     (122)      923 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/models/session.py
--rw-r--r--   0 runner    (1001) docker     (122)     3396 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/legislative/models/vote.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:36.010058 opencivicdata-3.3.0/opencivicdata/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6647 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)      384 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/tests/test_division.py
--rw-r--r--   0 runner    (1001) docker     (122)     2630 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/tests/test_elections.py
--rw-r--r--   0 runner    (1001) docker     (122)     1552 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/tests/test_loaddivisions.py
--rw-r--r--   0 runner    (1001) docker     (122)    14560 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)      441 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/opencivicdata/tests/test_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:59:35.998058 opencivicdata-3.3.0/opencivicdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      624 2023-05-16 15:59:35.000000 opencivicdata-3.3.0/opencivicdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4608 2023-05-16 15:59:35.000000 opencivicdata-3.3.0/opencivicdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-16 15:59:35.000000 opencivicdata-3.3.0/opencivicdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       96 2023-05-16 15:59:35.000000 opencivicdata-3.3.0/opencivicdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-05-16 15:59:35.000000 opencivicdata-3.3.0/opencivicdata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-05-16 15:59:36.010058 opencivicdata-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1021 2023-05-16 15:59:26.000000 opencivicdata-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:41.430410 opencivicdata-3.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-15 18:54:41.430410 opencivicdata-3.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:41.418411 opencivicdata-3.3.1/opencivicdata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6495 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:41.422411 opencivicdata-3.3.1/opencivicdata/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:41.422411 opencivicdata-3.3.1/opencivicdata/core/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/core/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/core/admin/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/core/admin/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/core/admin/other.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/core/admin/person.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/core/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:41.422411 opencivicdata-3.3.1/opencivicdata/core/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/core/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:41.422411 opencivicdata-3.3.1/opencivicdata/core/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/core/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/core/management/commands/loaddivisions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:41.422411 opencivicdata-3.3.1/opencivicdata/core/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    33372 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/core/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/core/migrations/0002_post_maximum_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41542 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/core/migrations/0003_field_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/core/migrations/0004_auto_20171005_2028.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/core/migrations/0005_auto_20191031_1507.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/core/migrations/0005_auto_20191124_1658.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/core/migrations/0006_merge_20200103_1432.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/core/migrations/0007_jurisdiction_last_seen_membership_last_seen_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/core/migrations/0008_auto_20221215_1132.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/core/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:41.422411 opencivicdata-3.3.1/opencivicdata/core/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/core/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/core/models/division.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/core/models/jurisdiction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16752 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/core/models/people_orgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/divisions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:41.422411 opencivicdata-3.3.1/opencivicdata/elections/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/elections/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:41.422411 opencivicdata-3.3.1/opencivicdata/elections/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/elections/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/elections/admin/candidacy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:41.422411 opencivicdata-3.3.1/opencivicdata/elections/admin/contests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/elections/admin/contests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/elections/admin/contests/ballot_measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/elections/admin/contests/candidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/elections/admin/contests/party.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/elections/admin/election.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/elections/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:41.426411 opencivicdata-3.3.1/opencivicdata/elections/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    42827 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/elections/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/elections/migrations/0002_auto_20170731_2047.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/elections/migrations/0003_election_fk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12472 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/elections/migrations/0004_field_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/elections/migrations/0005_auto_20170823_1648.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/elections/migrations/0006_auto_20171005_2029.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/elections/migrations/0007_auto_20171022_0234.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/elections/migrations/0008_auto_20181029_1527.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/elections/migrations/0009_auto_20221208_1041.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/elections/migrations/0010_auto_20221215_1132.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/elections/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:41.426411 opencivicdata-3.3.1/opencivicdata/elections/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/elections/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/elections/models/candidacy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:41.426411 opencivicdata-3.3.1/opencivicdata/elections/models/contests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/elections/models/contests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/elections/models/contests/ballot_measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/elections/models/contests/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/elections/models/contests/candidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/elections/models/contests/party.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/elections/models/election.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:41.426411 opencivicdata-3.3.1/opencivicdata/legislative/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/legislative/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:41.426411 opencivicdata-3.3.1/opencivicdata/legislative/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/legislative/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/legislative/admin/bill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/legislative/admin/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/legislative/admin/vote.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/legislative/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:41.426411 opencivicdata-3.3.1/opencivicdata/legislative/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    44134 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/legislative/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/legislative/migrations/0002_more_extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/legislative/migrations/0003_time_changes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/legislative/migrations/0004_auto_20171005_2027.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/legislative/migrations/0005_auto_20171005_2028.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/legislative/migrations/0006_billversion_extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/legislative/migrations/0007_auto_20181029_1527.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/legislative/migrations/0008_longer_event_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/legislative/migrations/0009_searchablebill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/legislative/migrations/0010_auto_20191031_1507.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/legislative/migrations/0011_auto_20191124_1658.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/legislative/migrations/0012_billdocument_extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/legislative/migrations/0013_auto_20200326_0458.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/legislative/migrations/0014_bill_last_seen_event_last_seen_voteevent_last_seen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/legislative/migrations/0015_auto_20221215_1132.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/legislative/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:41.430410 opencivicdata-3.3.1/opencivicdata/legislative/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/legislative/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/legislative/models/bill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/legislative/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/legislative/models/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/legislative/models/vote.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:41.430410 opencivicdata-3.3.1/opencivicdata/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6647 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/tests/test_division.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/tests/test_elections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/tests/test_loaddivisions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14560 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/opencivicdata/tests/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:41.418411 opencivicdata-3.3.1/opencivicdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-15 18:54:41.000000 opencivicdata-3.3.1/opencivicdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-05-15 18:54:41.000000 opencivicdata-3.3.1/opencivicdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 18:54:41.000000 opencivicdata-3.3.1/opencivicdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-15 18:54:41.000000 opencivicdata-3.3.1/opencivicdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 18:54:41.000000 opencivicdata-3.3.1/opencivicdata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-15 18:54:41.430410 opencivicdata-3.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-15 18:54:34.000000 opencivicdata-3.3.1/setup.py
```

### Comparing `opencivicdata-3.3.0/PKG-INFO` & `opencivicdata-3.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencivicdata
-Version: 3.3.0
+Version: 3.3.1
 Summary: python opencivicdata library
 Home-page: UNKNOWN
 Author: James Turk
 Author-email: james@openstates.org
 License: BSD
 Description: UNKNOWN
 Platform: any
```

### Comparing `opencivicdata-3.3.0/README.md` & `opencivicdata-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/common.py` & `opencivicdata-3.3.1/opencivicdata/common.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/core/admin/base.py` & `opencivicdata-3.3.1/opencivicdata/core/admin/base.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/core/admin/organization.py` & `opencivicdata-3.3.1/opencivicdata/core/admin/organization.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/core/admin/other.py` & `opencivicdata-3.3.1/opencivicdata/core/admin/other.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/core/admin/person.py` & `opencivicdata-3.3.1/opencivicdata/core/admin/person.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/core/management/commands/loaddivisions.py` & `opencivicdata-3.3.1/opencivicdata/core/management/commands/loaddivisions.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     """ convert a FileDivision to a Division """
     args, _ = Division.subtypes_from_id(fd.id)
     if fd.sameAs:
         args["redirect_id"] = fd.sameAs
     return Division(id=fd.id, name=fd.name, **args)
 
 
-def load_divisions(country, bulk=False):
+def load_divisions(country, bulk=False, sync=False):
     existing_divisions = Division.objects.filter(country=country)
 
     country_division = FileDivision.get("ocd-division/country:{}".format(country))
     objects = [to_db(country_division)]
 
     for child in country_division.children(levels=100):
         objects.append(to_db(child))
@@ -31,15 +31,15 @@
     )
 
     objects_set = set(objects)
     existing_divisions_set = set(existing_divisions)
 
     if objects_set == existing_divisions_set:
         print("The CSV and the DB contents are exactly the same; no work to be done!")
-    elif objects_set.issubset(existing_divisions_set):
+    elif not sync and objects_set.issubset(existing_divisions_set):
         print("The DB contains all CSV contents; no work to be done!")
     else:
         if bulk:
             # delete old ids and add new ones all at once
             with transaction.atomic():
                 Division.objects.filter(country=country).delete()
                 Division.objects.bulk_create(objects, batch_size=10000)
@@ -61,13 +61,19 @@
     help = "initialize a pupa database"
 
     def add_arguments(self, parser):
         parser.add_argument("countries", nargs="+", type=str)
         parser.add_argument(
             "--bulk",
             action="store_true",
-            help="Use bulk_create to add divisions. *Warning* This deletes any existing divisions",
+            help="Use bulk_create to add divisions. *Warning* This deletes any existing divisions.",
+        )
+        parser.add_argument(
+            "--sync",
+            action="store_true",
+            help="Add divisions from a CSV file, and delete existing divisions that are not in the "
+            "CSV file. This option only makes sense with a single country.",
         )
 
     def handle(self, *args, **options):
         for country in options["countries"]:
-            load_divisions(country, options["bulk"])
+            load_divisions(country, options["bulk"], options["sync"])
```

### Comparing `opencivicdata-3.3.0/opencivicdata/core/migrations/0001_initial.py` & `opencivicdata-3.3.1/opencivicdata/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/core/migrations/0003_field_docs.py` & `opencivicdata-3.3.1/opencivicdata/core/migrations/0003_field_docs.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/core/migrations/0004_auto_20171005_2028.py` & `opencivicdata-3.3.1/opencivicdata/core/migrations/0004_auto_20171005_2028.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/core/migrations/0005_auto_20191031_1507.py` & `opencivicdata-3.3.1/opencivicdata/core/migrations/0005_auto_20191031_1507.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/core/migrations/0005_auto_20191124_1658.py` & `opencivicdata-3.3.1/opencivicdata/core/migrations/0005_auto_20191124_1658.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/core/migrations/0007_jurisdiction_last_seen_membership_last_seen_and_more.py` & `opencivicdata-3.3.1/opencivicdata/core/migrations/0007_jurisdiction_last_seen_membership_last_seen_and_more.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/core/migrations/0008_auto_20221215_1132.py` & `opencivicdata-3.3.1/opencivicdata/core/migrations/0008_auto_20221215_1132.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/core/models/base.py` & `opencivicdata-3.3.1/opencivicdata/core/models/base.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/core/models/division.py` & `opencivicdata-3.3.1/opencivicdata/core/models/division.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/core/models/jurisdiction.py` & `opencivicdata-3.3.1/opencivicdata/core/models/jurisdiction.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/core/models/people_orgs.py` & `opencivicdata-3.3.1/opencivicdata/core/models/people_orgs.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/divisions.py` & `opencivicdata-3.3.1/opencivicdata/divisions.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/elections/admin/candidacy.py` & `opencivicdata-3.3.1/opencivicdata/elections/admin/candidacy.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/elections/admin/contests/ballot_measure.py` & `opencivicdata-3.3.1/opencivicdata/elections/admin/contests/ballot_measure.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/elections/admin/contests/candidate.py` & `opencivicdata-3.3.1/opencivicdata/elections/admin/contests/candidate.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/elections/admin/contests/party.py` & `opencivicdata-3.3.1/opencivicdata/elections/admin/contests/party.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/elections/admin/election.py` & `opencivicdata-3.3.1/opencivicdata/elections/admin/election.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/elections/migrations/0001_initial.py` & `opencivicdata-3.3.1/opencivicdata/elections/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/elections/migrations/0002_auto_20170731_2047.py` & `opencivicdata-3.3.1/opencivicdata/elections/migrations/0002_auto_20170731_2047.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/elections/migrations/0004_field_docs.py` & `opencivicdata-3.3.1/opencivicdata/elections/migrations/0004_field_docs.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/elections/migrations/0005_auto_20170823_1648.py` & `opencivicdata-3.3.1/opencivicdata/elections/migrations/0005_auto_20170823_1648.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/elections/migrations/0006_auto_20171005_2029.py` & `opencivicdata-3.3.1/opencivicdata/elections/migrations/0006_auto_20171005_2029.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/elections/migrations/0007_auto_20171022_0234.py` & `opencivicdata-3.3.1/opencivicdata/elections/migrations/0007_auto_20171022_0234.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/elections/migrations/0008_auto_20181029_1527.py` & `opencivicdata-3.3.1/opencivicdata/elections/migrations/0008_auto_20181029_1527.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/elections/migrations/0009_auto_20221208_1041.py` & `opencivicdata-3.3.1/opencivicdata/elections/migrations/0009_auto_20221208_1041.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/elections/migrations/0010_auto_20221215_1132.py` & `opencivicdata-3.3.1/opencivicdata/elections/migrations/0010_auto_20221215_1132.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/elections/models/__init__.py` & `opencivicdata-3.3.1/opencivicdata/elections/models/__init__.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/elections/models/candidacy.py` & `opencivicdata-3.3.1/opencivicdata/elections/models/candidacy.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/elections/models/contests/ballot_measure.py` & `opencivicdata-3.3.1/opencivicdata/elections/models/contests/ballot_measure.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/elections/models/contests/base.py` & `opencivicdata-3.3.1/opencivicdata/elections/models/contests/base.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/elections/models/contests/candidate.py` & `opencivicdata-3.3.1/opencivicdata/elections/models/contests/candidate.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/elections/models/contests/party.py` & `opencivicdata-3.3.1/opencivicdata/elections/models/contests/party.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/elections/models/election.py` & `opencivicdata-3.3.1/opencivicdata/elections/models/election.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/legislative/admin/bill.py` & `opencivicdata-3.3.1/opencivicdata/legislative/admin/bill.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/legislative/admin/event.py` & `opencivicdata-3.3.1/opencivicdata/legislative/admin/event.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/legislative/admin/vote.py` & `opencivicdata-3.3.1/opencivicdata/legislative/admin/vote.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/legislative/migrations/0001_initial.py` & `opencivicdata-3.3.1/opencivicdata/legislative/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/legislative/migrations/0002_more_extras.py` & `opencivicdata-3.3.1/opencivicdata/legislative/migrations/0002_more_extras.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/legislative/migrations/0003_time_changes.py` & `opencivicdata-3.3.1/opencivicdata/legislative/migrations/0003_time_changes.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/legislative/migrations/0004_auto_20171005_2027.py` & `opencivicdata-3.3.1/opencivicdata/legislative/migrations/0004_auto_20171005_2027.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/legislative/migrations/0005_auto_20171005_2028.py` & `opencivicdata-3.3.1/opencivicdata/legislative/migrations/0005_auto_20171005_2028.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/legislative/migrations/0009_searchablebill.py` & `opencivicdata-3.3.1/opencivicdata/legislative/migrations/0009_searchablebill.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/legislative/migrations/0010_auto_20191031_1507.py` & `opencivicdata-3.3.1/opencivicdata/legislative/migrations/0010_auto_20191031_1507.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/legislative/migrations/0011_auto_20191124_1658.py` & `opencivicdata-3.3.1/opencivicdata/legislative/migrations/0011_auto_20191124_1658.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/legislative/migrations/0014_bill_last_seen_event_last_seen_voteevent_last_seen.py` & `opencivicdata-3.3.1/opencivicdata/legislative/migrations/0014_bill_last_seen_event_last_seen_voteevent_last_seen.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/legislative/migrations/0015_auto_20221215_1132.py` & `opencivicdata-3.3.1/opencivicdata/legislative/migrations/0015_auto_20221215_1132.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/legislative/models/__init__.py` & `opencivicdata-3.3.1/opencivicdata/legislative/models/__init__.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/legislative/models/bill.py` & `opencivicdata-3.3.1/opencivicdata/legislative/models/bill.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/legislative/models/event.py` & `opencivicdata-3.3.1/opencivicdata/legislative/models/event.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/legislative/models/session.py` & `opencivicdata-3.3.1/opencivicdata/legislative/models/session.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/legislative/models/vote.py` & `opencivicdata-3.3.1/opencivicdata/legislative/models/vote.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/tests/conftest.py` & `opencivicdata-3.3.1/opencivicdata/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/tests/test_elections.py` & `opencivicdata-3.3.1/opencivicdata/tests/test_elections.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/tests/test_loaddivisions.py` & `opencivicdata-3.3.1/opencivicdata/tests/test_loaddivisions.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata/tests/test_models.py` & `opencivicdata-3.3.1/opencivicdata/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/opencivicdata.egg-info/PKG-INFO` & `opencivicdata-3.3.1/opencivicdata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencivicdata
-Version: 3.3.0
+Version: 3.3.1
 Summary: python opencivicdata library
 Home-page: UNKNOWN
 Author: James Turk
 Author-email: james@openstates.org
 License: BSD
 Description: UNKNOWN
 Platform: any
```

### Comparing `opencivicdata-3.3.0/opencivicdata.egg-info/SOURCES.txt` & `opencivicdata-3.3.1/opencivicdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opencivicdata-3.3.0/setup.py` & `opencivicdata-3.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 extras_require = {
     "dev": ["pytest>=3.6", "pytest-cov", "pytest-django", "coveralls==3.2.0", "flake8"]
 }
 
 setup(
     name="opencivicdata",
-    version="3.3.0",
+    version="3.3.1",
     author="James Turk",
     author_email="james@openstates.org",
     license="BSD",
     description="python opencivicdata library",
     long_description="",
     url="",
     packages=find_packages(),
```

