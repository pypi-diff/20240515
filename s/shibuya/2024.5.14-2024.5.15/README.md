# Comparing `tmp/shibuya-2024.5.14.tar.gz` & `tmp/shibuya-2024.5.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shibuya-2024.5.14.tar", last modified: Tue May 14 12:21:34 2024, max compression
+gzip compressed data, was "shibuya-2024.5.15.tar", last modified: Wed May 15 13:17:21 2024, max compression
```

## Comparing `shibuya-2024.5.14.tar` & `shibuya-2024.5.15.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.771084 shibuya-2024.5.14/
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-14 12:21:23.000000 shibuya-2024.5.14/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-14 12:21:23.000000 shibuya-2024.5.14/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-14 12:21:34.771084 shibuya-2024.5.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-14 12:21:23.000000 shibuya-2024.5.14/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-14 12:21:23.000000 shibuya-2024.5.14/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 12:21:34.771084 shibuya-2024.5.14/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-14 12:21:23.000000 shibuya-2024.5.14/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.755084 shibuya-2024.5.14/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.759084 shibuya-2024.5.14/src/shibuya/
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/_sphinx.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.755084 shibuya-2024.5.14/src/shibuya/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.755084 shibuya-2024.5.14/src/shibuya/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.759084 shibuya-2024.5.14/src/shibuya/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/locale/de/LC_MESSAGES/sphinx.mo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.755084 shibuya-2024.5.14/src/shibuya/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.759084 shibuya-2024.5.14/src/shibuya/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/locale/es/LC_MESSAGES/sphinx.mo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.755084 shibuya-2024.5.14/src/shibuya/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.759084 shibuya-2024.5.14/src/shibuya/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/locale/fr/LC_MESSAGES/sphinx.mo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.755084 shibuya-2024.5.14/src/shibuya/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.759084 shibuya-2024.5.14/src/shibuya/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/locale/ja/LC_MESSAGES/sphinx.mo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.755084 shibuya-2024.5.14/src/shibuya/locale/ko/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.759084 shibuya-2024.5.14/src/shibuya/locale/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/locale/ko/LC_MESSAGES/sphinx.mo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.755084 shibuya-2024.5.14/src/shibuya/locale/pt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.759084 shibuya-2024.5.14/src/shibuya/locale/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/locale/pt/LC_MESSAGES/sphinx.mo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.755084 shibuya-2024.5.14/src/shibuya/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.759084 shibuya-2024.5.14/src/shibuya/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/locale/pt_BR/LC_MESSAGES/sphinx.mo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.755084 shibuya-2024.5.14/src/shibuya/locale/zh/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.759084 shibuya-2024.5.14/src/shibuya/locale/zh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/locale/zh/LC_MESSAGES/sphinx.mo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.755084 shibuya-2024.5.14/src/shibuya/locale/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.763084 shibuya-2024.5.14/src/shibuya/locale/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/locale/zh_TW/LC_MESSAGES/sphinx.mo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.755084 shibuya-2024.5.14/src/shibuya/theme/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.763084 shibuya-2024.5.14/src/shibuya/theme/shibuya/
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/base.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.767084 shibuya-2024.5.14/src/shibuya/theme/shibuya/components/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/components/alternate-links.html
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/components/back-to-top.html
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/components/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/components/discussion-link.html
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/components/foot-copyright.html
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/components/foot-socials.html
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/components/meta-opengraph.html
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/components/nav-languages.html
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/components/nav-links.html
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/components/nav-socials.html
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/components/nav-versions.html
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/components/navigation.html
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/components/searchbox.html
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/components/site-foot.html
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/components/site-head.html
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/components/theme-switch.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.767084 shibuya-2024.5.14/src/shibuya/theme/shibuya/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/extensions/buysellads.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.767084 shibuya-2024.5.14/src/shibuya/theme/shibuya/layout/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/layout/404.html
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/layout/compact.html
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/layout/default.html
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/layout/landing.html
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/layout/simple.html
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/localtoc.html
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/page.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.767084 shibuya-2024.5.14/src/shibuya/theme/shibuya/partials/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/partials/article-bottom.html
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/partials/banner.html
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/partials/extra-head.html
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/partials/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/partials/globaltoc-above.html
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/partials/page-bottom.html
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/partials/webfonts.html
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/relations.html
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/search.html
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/searchbox.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.767084 shibuya-2024.5.14/src/shibuya/theme/shibuya/sidebars/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/sidebars/carbon-ads.html
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/sidebars/edit-this-page.html
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/sidebars/ethical-ads.html
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/sidebars/localtoc.html
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/sidebars/repo-stats.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.767084 shibuya-2024.5.14/src/shibuya/theme/shibuya/static/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/static/print.css
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (127)   229960 2024-05-14 12:21:31.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/static/shibuya.css
--rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-05-14 12:21:29.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/static/shibuya.js
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/theme.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.771084 shibuya-2024.5.14/src/shibuya.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-14 12:21:34.000000 shibuya-2024.5.14/src/shibuya.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-14 12:21:34.000000 shibuya-2024.5.14/src/shibuya.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 12:21:34.000000 shibuya-2024.5.14/src/shibuya.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-14 12:21:34.000000 shibuya-2024.5.14/src/shibuya.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 12:21:34.000000 shibuya-2024.5.14/src/shibuya.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 12:21:34.000000 shibuya-2024.5.14/src/shibuya.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:17:21.399531 shibuya-2024.5.15/
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-15 13:17:06.000000 shibuya-2024.5.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-15 13:17:06.000000 shibuya-2024.5.15/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-15 13:17:21.399531 shibuya-2024.5.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-15 13:17:06.000000 shibuya-2024.5.15/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-15 13:17:06.000000 shibuya-2024.5.15/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 13:17:21.399531 shibuya-2024.5.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-15 13:17:06.000000 shibuya-2024.5.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:17:21.387531 shibuya-2024.5.15/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:17:21.391531 shibuya-2024.5.15/src/shibuya/
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/_sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:17:21.387531 shibuya-2024.5.15/src/shibuya/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:17:21.387531 shibuya-2024.5.15/src/shibuya/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:17:21.391531 shibuya-2024.5.15/src/shibuya/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/locale/de/LC_MESSAGES/sphinx.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:17:21.387531 shibuya-2024.5.15/src/shibuya/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:17:21.391531 shibuya-2024.5.15/src/shibuya/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/locale/es/LC_MESSAGES/sphinx.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:17:21.387531 shibuya-2024.5.15/src/shibuya/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:17:21.391531 shibuya-2024.5.15/src/shibuya/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/locale/fr/LC_MESSAGES/sphinx.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:17:21.387531 shibuya-2024.5.15/src/shibuya/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:17:21.391531 shibuya-2024.5.15/src/shibuya/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/locale/ja/LC_MESSAGES/sphinx.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:17:21.387531 shibuya-2024.5.15/src/shibuya/locale/ko/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:17:21.391531 shibuya-2024.5.15/src/shibuya/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/locale/ko/LC_MESSAGES/sphinx.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:17:21.387531 shibuya-2024.5.15/src/shibuya/locale/pt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:17:21.391531 shibuya-2024.5.15/src/shibuya/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/locale/pt/LC_MESSAGES/sphinx.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:17:21.387531 shibuya-2024.5.15/src/shibuya/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:17:21.391531 shibuya-2024.5.15/src/shibuya/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/locale/pt_BR/LC_MESSAGES/sphinx.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:17:21.387531 shibuya-2024.5.15/src/shibuya/locale/zh/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:17:21.391531 shibuya-2024.5.15/src/shibuya/locale/zh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/locale/zh/LC_MESSAGES/sphinx.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:17:21.387531 shibuya-2024.5.15/src/shibuya/locale/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:17:21.391531 shibuya-2024.5.15/src/shibuya/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/locale/zh_TW/LC_MESSAGES/sphinx.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:17:21.387531 shibuya-2024.5.15/src/shibuya/theme/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:17:21.391531 shibuya-2024.5.15/src/shibuya/theme/shibuya/
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/base.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:17:21.395531 shibuya-2024.5.15/src/shibuya/theme/shibuya/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/components/alternate-links.html
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/components/back-to-top.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/components/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/components/discussion-link.html
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/components/foot-copyright.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/components/foot-socials.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/components/meta-opengraph.html
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/components/nav-languages.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/components/nav-links.html
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/components/nav-socials.html
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/components/nav-versions.html
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/components/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/components/searchbox.html
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/components/site-foot.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/components/site-head.html
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/components/theme-switch.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:17:21.395531 shibuya-2024.5.15/src/shibuya/theme/shibuya/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/extensions/buysellads.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:17:21.395531 shibuya-2024.5.15/src/shibuya/theme/shibuya/layout/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/layout/404.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/layout/compact.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/layout/default.html
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/layout/landing.html
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/layout/simple.html
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/localtoc.html
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/page.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:17:21.395531 shibuya-2024.5.15/src/shibuya/theme/shibuya/partials/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/partials/article-bottom.html
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/partials/banner.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/partials/extra-head.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/partials/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/partials/globaltoc-above.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/partials/page-bottom.html
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/partials/webfonts.html
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/relations.html
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/search.html
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/searchbox.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:17:21.399531 shibuya-2024.5.15/src/shibuya/theme/shibuya/sidebars/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/sidebars/carbon-ads.html
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/sidebars/edit-this-page.html
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/sidebars/ethical-ads.html
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/sidebars/localtoc.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/sidebars/repo-stats.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:17:21.399531 shibuya-2024.5.15/src/shibuya/theme/shibuya/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/static/print.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (127)   229995 2024-05-15 13:17:17.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/static/shibuya.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-05-15 13:17:15.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/static/shibuya.js
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-15 13:17:06.000000 shibuya-2024.5.15/src/shibuya/theme/shibuya/theme.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:17:21.399531 shibuya-2024.5.15/src/shibuya.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-15 13:17:21.000000 shibuya-2024.5.15/src/shibuya.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-15 13:17:21.000000 shibuya-2024.5.15/src/shibuya.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 13:17:21.000000 shibuya-2024.5.15/src/shibuya.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-15 13:17:21.000000 shibuya-2024.5.15/src/shibuya.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 13:17:21.000000 shibuya-2024.5.15/src/shibuya.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 13:17:21.000000 shibuya-2024.5.15/src/shibuya.egg-info/top_level.txt
```

### Comparing `shibuya-2024.5.14/LICENSE` & `shibuya-2024.5.15/LICENSE`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.14/PKG-INFO` & `shibuya-2024.5.15/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shibuya
-Version: 2024.5.14
+Version: 2024.5.15
 Summary: A clean, responsive, and customizable Sphinx documentation theme with light/dark mode.
 Author-email: Hsiaoming Yang <me@lepture.com>
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/lepture/shibuya
 Project-URL: Documentation, https://shibuya.lepture.com/
 Project-URL: Sponsors, https://github.com/sponsors/lepture
 Classifier: Framework :: Sphinx
```

### Comparing `shibuya-2024.5.14/README.md` & `shibuya-2024.5.15/README.md`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.14/pyproject.toml` & `shibuya-2024.5.15/pyproject.toml`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.14/src/shibuya/__init__.py` & `shibuya-2024.5.15/src/shibuya/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     create_edit_source_link,
 )
 from ._sphinx import (
     WrapperPostTransform,
     WrapLineFormatter,
 )
 
-__version__ = "2024.5.14"
+__version__ = "2024.5.15"
 
 shibuya_version = __version__
 
 ROOT_PATH = Path(__file__).parent
 THEME_PATH = (ROOT_PATH / "theme" / "shibuya").resolve()
```

### Comparing `shibuya-2024.5.14/src/shibuya/_sphinx.py` & `shibuya-2024.5.15/src/shibuya/_sphinx.py`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.14/src/shibuya/context.py` & `shibuya-2024.5.15/src/shibuya/context.py`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.14/src/shibuya/locale/de/LC_MESSAGES/sphinx.mo` & `shibuya-2024.5.15/src/shibuya/locale/de/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.14/src/shibuya/locale/es/LC_MESSAGES/sphinx.mo` & `shibuya-2024.5.15/src/shibuya/locale/es/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.14/src/shibuya/locale/fr/LC_MESSAGES/sphinx.mo` & `shibuya-2024.5.15/src/shibuya/locale/fr/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.14/src/shibuya/locale/ja/LC_MESSAGES/sphinx.mo` & `shibuya-2024.5.15/src/shibuya/locale/ja/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.14/src/shibuya/locale/ko/LC_MESSAGES/sphinx.mo` & `shibuya-2024.5.15/src/shibuya/locale/ko/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.14/src/shibuya/locale/pt/LC_MESSAGES/sphinx.mo` & `shibuya-2024.5.15/src/shibuya/locale/pt/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.14/src/shibuya/locale/pt_BR/LC_MESSAGES/sphinx.mo` & `shibuya-2024.5.15/src/shibuya/locale/pt_BR/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.14/src/shibuya/locale/zh/LC_MESSAGES/sphinx.mo` & `shibuya-2024.5.15/src/shibuya/locale/zh/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.14/src/shibuya/locale/zh_TW/LC_MESSAGES/sphinx.mo` & `shibuya-2024.5.15/src/shibuya/locale/zh_TW/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.14/src/shibuya/theme/shibuya/base.html` & `shibuya-2024.5.15/src/shibuya/theme/shibuya/base.html`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.14/src/shibuya/theme/shibuya/components/breadcrumbs.html` & `shibuya-2024.5.15/src/shibuya/theme/shibuya/components/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.14/src/shibuya/theme/shibuya/components/discussion-link.html` & `shibuya-2024.5.15/src/shibuya/theme/shibuya/components/discussion-link.html`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.14/src/shibuya/theme/shibuya/components/foot-socials.html` & `shibuya-2024.5.15/src/shibuya/theme/shibuya/components/foot-socials.html`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.14/src/shibuya/theme/shibuya/components/meta-opengraph.html` & `shibuya-2024.5.15/src/shibuya/theme/shibuya/components/meta-opengraph.html`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.14/src/shibuya/theme/shibuya/components/nav-links.html` & `shibuya-2024.5.15/src/shibuya/theme/shibuya/components/nav-links.html`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.14/src/shibuya/theme/shibuya/components/nav-socials.html` & `shibuya-2024.5.15/src/shibuya/theme/shibuya/components/nav-socials.html`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.14/src/shibuya/theme/shibuya/components/nav-versions.html` & `shibuya-2024.5.15/src/shibuya/theme/shibuya/components/nav-versions.html`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.14/src/shibuya/theme/shibuya/components/navigation.html` & `shibuya-2024.5.15/src/shibuya/theme/shibuya/components/navigation.html`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.14/src/shibuya/theme/shibuya/components/site-head.html` & `shibuya-2024.5.15/src/shibuya/theme/shibuya/components/site-head.html`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.14/src/shibuya/theme/shibuya/extensions/buysellads.html` & `shibuya-2024.5.15/src/shibuya/theme/shibuya/extensions/buysellads.html`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.14/src/shibuya/theme/shibuya/layout/compact.html` & `shibuya-2024.5.15/src/shibuya/theme/shibuya/layout/compact.html`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.14/src/shibuya/theme/shibuya/layout/default.html` & `shibuya-2024.5.15/src/shibuya/theme/shibuya/layout/default.html`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.14/src/shibuya/theme/shibuya/layout.html` & `shibuya-2024.5.15/src/shibuya/theme/shibuya/layout.html`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.14/src/shibuya/theme/shibuya/sidebars/repo-stats.html` & `shibuya-2024.5.15/src/shibuya/theme/shibuya/sidebars/repo-stats.html`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.14/src/shibuya/theme/shibuya/static/print.css` & `shibuya-2024.5.15/src/shibuya/theme/shibuya/static/print.css`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.14/src/shibuya/theme/shibuya/static/pygments.css` & `shibuya-2024.5.15/src/shibuya/theme/shibuya/static/pygments.css`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.14/src/shibuya/theme/shibuya/static/shibuya.css` & `shibuya-2024.5.15/src/shibuya/theme/shibuya/static/shibuya.css`

 * *Files 0% similar despite different names*

```diff
@@ -12416,1958 +12416,1960 @@
 000307f0: 6f72 2d31 3a76 6172 282d 2d63 6f6c 6f72  or-1:var(--color
 00030800: 2d73 7572 6661 6365 2d61 6363 656e 7429  -surface-accent)
 00030810: 3b2d 2d63 6f6c 6f72 2d32 3a76 6172 282d  ;--color-2:var(-
 00030820: 2d61 6363 656e 742d 6133 293b 2d2d 636f  -accent-a3);--co
 00030830: 6c6f 722d 333a 7661 7228 2d2d 6163 6365  lor-3:var(--acce
 00030840: 6e74 2d39 293b 2d2d 636f 6c6f 722d 343a  nt-9);--color-4:
 00030850: 7661 7228 2d2d 6163 6365 6e74 2d61 3131  var(--accent-a11
-00030860: 293b 706f 7369 7469 6f6e 3a72 656c 6174  );position:relat
-00030870: 6976 653b 7061 6464 696e 673a 3020 3136  ive;padding:0 16
-00030880: 7078 202e 3872 656d 3b6d 6172 6769 6e2d  px .8rem;margin-
-00030890: 746f 703a 3172 656d 3b6d 6172 6769 6e2d  top:1rem;margin-
-000308a0: 626f 7474 6f6d 3a31 7265 6d3b 626f 7264  bottom:1rem;bord
-000308b0: 6572 2d6c 6566 743a 3470 7820 736f 6c69  er-left:4px soli
-000308c0: 6420 7661 7228 2d2d 636f 6c6f 722d 3329  d var(--color-3)
-000308d0: 3b62 6163 6b67 726f 756e 642d 636f 6c6f  ;background-colo
-000308e0: 723a 7661 7228 2d2d 636f 6c6f 722d 3129  r:var(--color-1)
-000308f0: 7d2e 6164 6d6f 6e69 7469 6f6e 3a62 6566  }.admonition:bef
-00030900: 6f72 657b 706f 7369 7469 6f6e 3a61 6273  ore{position:abs
-00030910: 6f6c 7574 653b 636f 6e74 656e 743a 2222  olute;content:""
-00030920: 3b74 6f70 3a36 7078 3b6c 6566 743a 2d31  ;top:6px;left:-1
-00030930: 3270 783b 7769 6474 683a 3230 7078 3b68  2px;width:20px;h
-00030940: 6569 6768 743a 3230 7078 3b62 6f72 6465  eight:20px;borde
-00030950: 722d 7261 6469 7573 3a31 3030 253b 6261  r-radius:100%;ba
-00030960: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3a76  ckground-color:v
-00030970: 6172 282d 2d63 6f6c 6f72 2d33 297d 2e61  ar(--color-3)}.a
-00030980: 646d 6f6e 6974 696f 6e20 702e 6164 6d6f  dmonition p.admo
-00030990: 6e69 7469 6f6e 2d74 6974 6c65 7b70 6f73  nition-title{pos
-000309a0: 6974 696f 6e3a 7265 6c61 7469 7665 3b6d  ition:relative;m
-000309b0: 6172 6769 6e3a 3020 2d31 3670 7820 2e38  argin:0 -16px .8
-000309c0: 7265 6d20 2d31 3970 783b 7061 6464 696e  rem -19px;paddin
-000309d0: 673a 3470 7820 3138 7078 3b66 6f6e 742d  g:4px 18px;font-
-000309e0: 7369 7a65 3a2e 3835 7265 6d3b 666f 6e74  size:.85rem;font
-000309f0: 2d77 6569 6768 743a 3630 303b 6c69 6e65  -weight:600;line
-00030a00: 2d68 6569 6768 743a 312e 3732 3b63 6f6c  -height:1.72;col
-00030a10: 6f72 3a76 6172 282d 2d63 6f6c 6f72 2d34  or:var(--color-4
-00030a20: 293b 6261 636b 6772 6f75 6e64 2d63 6f6c  );background-col
-00030a30: 6f72 3a76 6172 282d 2d63 6f6c 6f72 2d32  or:var(--color-2
-00030a40: 293b 2d2d 7975 652d 632d 636f 6465 3a76  );--yue-c-code:v
-00030a50: 6172 282d 2d63 6f6c 6f72 2d34 293b 2d2d  ar(--color-4);--
-00030a60: 7975 652d 632d 626f 6c64 3a76 6172 282d  yue-c-bold:var(-
-00030a70: 2d63 6f6c 6f72 2d34 297d 2e61 646d 6f6e  -color-4)}.admon
-00030a80: 6974 696f 6e20 702e 6164 6d6f 6e69 7469  ition p.admoniti
-00030a90: 6f6e 2d74 6974 6c65 2073 7667 7b64 6973  on-title svg{dis
-00030aa0: 706c 6179 3a69 6e6c 696e 652d 626c 6f63  play:inline-bloc
-00030ab0: 6b7d 2e61 646d 6f6e 6974 696f 6e2d 7469  k}.admonition-ti
-00030ac0: 746c 653a 6265 666f 7265 7b70 6f73 6974  tle:before{posit
-00030ad0: 696f 6e3a 6162 736f 6c75 7465 3b63 6f6e  ion:absolute;con
-00030ae0: 7465 6e74 3a22 223b 746f 703a 3130 7078  tent:"";top:10px
-00030af0: 3b6c 6566 743a 2d35 7078 3b2d 7765 626b  ;left:-5px;-webk
-00030b00: 6974 2d6d 6173 6b3a 7661 7228 2d2d 6963  it-mask:var(--ic
-00030b10: 6f6e 2d75 726c 2920 6e6f 2d72 6570 6561  on-url) no-repea
-00030b20: 743b 6d61 736b 3a76 6172 282d 2d69 636f  t;mask:var(--ico
-00030b30: 6e2d 7572 6c29 206e 6f2d 7265 7065 6174  n-url) no-repeat
-00030b40: 3b2d 7765 626b 6974 2d6d 6173 6b2d 7369  ;-webkit-mask-si
-00030b50: 7a65 3a31 3030 2520 3130 3025 3b6d 6173  ze:100% 100%;mas
-00030b60: 6b2d 7369 7a65 3a31 3030 2520 3130 3025  k-size:100% 100%
-00030b70: 3b66 6f6e 742d 7374 796c 653a 6e6f 726d  ;font-style:norm
-00030b80: 616c 3b77 6964 7468 3a31 3270 783b 6865  al;width:12px;he
-00030b90: 6967 6874 3a31 3270 783b 6261 636b 6772  ight:12px;backgr
-00030ba0: 6f75 6e64 2d63 6f6c 6f72 3a23 6666 667d  ound-color:#fff}
-00030bb0: 2e61 646d 6f6e 6974 696f 6e2e 6174 7465  .admonition.atte
-00030bc0: 6e74 696f 6e7b 2d2d 6963 6f6e 2d75 726c  ntion{--icon-url
-00030bd0: 3a76 6172 282d 2d61 7474 656e 7469 6f6e  :var(--attention
-00030be0: 2d69 636f 6e29 3b2d 2d63 6f6c 6f72 2d31  -icon);--color-1
-00030bf0: 3a76 6172 282d 2d61 7474 656e 7469 6f6e  :var(--attention
-00030c00: 2d31 293b 2d2d 636f 6c6f 722d 323a 7661  -1);--color-2:va
-00030c10: 7228 2d2d 6174 7465 6e74 696f 6e2d 3229  r(--attention-2)
-00030c20: 3b2d 2d63 6f6c 6f72 2d33 3a76 6172 282d  ;--color-3:var(-
-00030c30: 2d61 7474 656e 7469 6f6e 2d33 293b 2d2d  -attention-3);--
-00030c40: 636f 6c6f 722d 343a 7661 7228 2d2d 6174  color-4:var(--at
-00030c50: 7465 6e74 696f 6e2d 3429 7d2e 6164 6d6f  tention-4)}.admo
-00030c60: 6e69 7469 6f6e 2e63 6175 7469 6f6e 7b2d  nition.caution{-
-00030c70: 2d69 636f 6e2d 7572 6c3a 7661 7228 2d2d  -icon-url:var(--
-00030c80: 6361 7574 696f 6e2d 6963 6f6e 293b 2d2d  caution-icon);--
-00030c90: 636f 6c6f 722d 313a 7661 7228 2d2d 6361  color-1:var(--ca
-00030ca0: 7574 696f 6e2d 3129 3b2d 2d63 6f6c 6f72  ution-1);--color
-00030cb0: 2d32 3a76 6172 282d 2d63 6175 7469 6f6e  -2:var(--caution
-00030cc0: 2d32 293b 2d2d 636f 6c6f 722d 333a 7661  -2);--color-3:va
-00030cd0: 7228 2d2d 6361 7574 696f 6e2d 3329 3b2d  r(--caution-3);-
-00030ce0: 2d63 6f6c 6f72 2d34 3a76 6172 282d 2d63  -color-4:var(--c
-00030cf0: 6175 7469 6f6e 2d34 297d 2e61 646d 6f6e  aution-4)}.admon
-00030d00: 6974 696f 6e2e 6461 6e67 6572 7b2d 2d69  ition.danger{--i
-00030d10: 636f 6e2d 7572 6c3a 7661 7228 2d2d 6461  con-url:var(--da
-00030d20: 6e67 6572 2d69 636f 6e29 3b2d 2d63 6f6c  nger-icon);--col
-00030d30: 6f72 2d31 3a76 6172 282d 2d64 616e 6765  or-1:var(--dange
-00030d40: 722d 3129 3b2d 2d63 6f6c 6f72 2d32 3a76  r-1);--color-2:v
-00030d50: 6172 282d 2d64 616e 6765 722d 3229 3b2d  ar(--danger-2);-
-00030d60: 2d63 6f6c 6f72 2d33 3a76 6172 282d 2d64  -color-3:var(--d
-00030d70: 616e 6765 722d 3329 3b2d 2d63 6f6c 6f72  anger-3);--color
-00030d80: 2d34 3a76 6172 282d 2d64 616e 6765 722d  -4:var(--danger-
-00030d90: 3429 7d2e 6164 6d6f 6e69 7469 6f6e 2e65  4)}.admonition.e
-00030da0: 7272 6f72 7b2d 2d69 636f 6e2d 7572 6c3a  rror{--icon-url:
-00030db0: 7661 7228 2d2d 6572 726f 722d 6963 6f6e  var(--error-icon
-00030dc0: 293b 2d2d 636f 6c6f 722d 313a 7661 7228  );--color-1:var(
-00030dd0: 2d2d 6572 726f 722d 3129 3b2d 2d63 6f6c  --error-1);--col
-00030de0: 6f72 2d32 3a76 6172 282d 2d65 7272 6f72  or-2:var(--error
-00030df0: 2d32 293b 2d2d 636f 6c6f 722d 333a 7661  -2);--color-3:va
-00030e00: 7228 2d2d 6572 726f 722d 3329 3b2d 2d63  r(--error-3);--c
-00030e10: 6f6c 6f72 2d34 3a76 6172 282d 2d65 7272  olor-4:var(--err
-00030e20: 6f72 2d34 297d 2e61 646d 6f6e 6974 696f  or-4)}.admonitio
-00030e30: 6e2e 6869 6e74 7b2d 2d69 636f 6e2d 7572  n.hint{--icon-ur
-00030e40: 6c3a 7661 7228 2d2d 6869 6e74 2d69 636f  l:var(--hint-ico
-00030e50: 6e29 3b2d 2d63 6f6c 6f72 2d31 3a76 6172  n);--color-1:var
-00030e60: 282d 2d68 696e 742d 3129 3b2d 2d63 6f6c  (--hint-1);--col
-00030e70: 6f72 2d32 3a76 6172 282d 2d68 696e 742d  or-2:var(--hint-
-00030e80: 3229 3b2d 2d63 6f6c 6f72 2d33 3a76 6172  2);--color-3:var
-00030e90: 282d 2d68 696e 742d 3329 3b2d 2d63 6f6c  (--hint-3);--col
-00030ea0: 6f72 2d34 3a76 6172 282d 2d68 696e 742d  or-4:var(--hint-
-00030eb0: 3429 7d2e 6164 6d6f 6e69 7469 6f6e 2e69  4)}.admonition.i
-00030ec0: 6d70 6f72 7461 6e74 7b2d 2d69 636f 6e2d  mportant{--icon-
-00030ed0: 7572 6c3a 7661 7228 2d2d 696d 706f 7274  url:var(--import
-00030ee0: 616e 742d 6963 6f6e 293b 2d2d 636f 6c6f  ant-icon);--colo
-00030ef0: 722d 313a 7661 7228 2d2d 696d 706f 7274  r-1:var(--import
-00030f00: 616e 742d 3129 3b2d 2d63 6f6c 6f72 2d32  ant-1);--color-2
-00030f10: 3a76 6172 282d 2d69 6d70 6f72 7461 6e74  :var(--important
-00030f20: 2d32 293b 2d2d 636f 6c6f 722d 333a 7661  -2);--color-3:va
-00030f30: 7228 2d2d 696d 706f 7274 616e 742d 3329  r(--important-3)
-00030f40: 3b2d 2d63 6f6c 6f72 2d34 3a76 6172 282d  ;--color-4:var(-
-00030f50: 2d69 6d70 6f72 7461 6e74 2d34 297d 2e61  -important-4)}.a
-00030f60: 646d 6f6e 6974 696f 6e2e 6e6f 7465 7b2d  dmonition.note{-
-00030f70: 2d69 636f 6e2d 7572 6c3a 7661 7228 2d2d  -icon-url:var(--
-00030f80: 6e6f 7465 2d69 636f 6e29 3b2d 2d63 6f6c  note-icon);--col
-00030f90: 6f72 2d31 3a76 6172 282d 2d6e 6f74 652d  or-1:var(--note-
-00030fa0: 3129 3b2d 2d63 6f6c 6f72 2d32 3a76 6172  1);--color-2:var
-00030fb0: 282d 2d6e 6f74 652d 3229 3b2d 2d63 6f6c  (--note-2);--col
-00030fc0: 6f72 2d33 3a76 6172 282d 2d6e 6f74 652d  or-3:var(--note-
-00030fd0: 3329 3b2d 2d63 6f6c 6f72 2d34 3a76 6172  3);--color-4:var
-00030fe0: 282d 2d6e 6f74 652d 3429 7d2e 6164 6d6f  (--note-4)}.admo
-00030ff0: 6e69 7469 6f6e 2e74 6970 7b2d 2d69 636f  nition.tip{--ico
-00031000: 6e2d 7572 6c3a 7661 7228 2d2d 7469 702d  n-url:var(--tip-
-00031010: 6963 6f6e 293b 2d2d 636f 6c6f 722d 313a  icon);--color-1:
-00031020: 7661 7228 2d2d 7469 702d 3129 3b2d 2d63  var(--tip-1);--c
-00031030: 6f6c 6f72 2d32 3a76 6172 282d 2d74 6970  olor-2:var(--tip
-00031040: 2d32 293b 2d2d 636f 6c6f 722d 333a 7661  -2);--color-3:va
-00031050: 7228 2d2d 7469 702d 3329 3b2d 2d63 6f6c  r(--tip-3);--col
-00031060: 6f72 2d34 3a76 6172 282d 2d74 6970 2d34  or-4:var(--tip-4
-00031070: 297d 2e61 646d 6f6e 6974 696f 6e2e 7761  )}.admonition.wa
-00031080: 726e 696e 677b 2d2d 6963 6f6e 2d75 726c  rning{--icon-url
-00031090: 3a76 6172 282d 2d77 6172 6e69 6e67 2d69  :var(--warning-i
-000310a0: 636f 6e29 3b2d 2d63 6f6c 6f72 2d31 3a76  con);--color-1:v
-000310b0: 6172 282d 2d77 6172 6e69 6e67 2d31 293b  ar(--warning-1);
-000310c0: 2d2d 636f 6c6f 722d 323a 7661 7228 2d2d  --color-2:var(--
-000310d0: 7761 726e 696e 672d 3229 3b2d 2d63 6f6c  warning-2);--col
-000310e0: 6f72 2d33 3a76 6172 282d 2d77 6172 6e69  or-3:var(--warni
-000310f0: 6e67 2d33 293b 2d2d 636f 6c6f 722d 343a  ng-3);--color-4:
-00031100: 7661 7228 2d2d 7761 726e 696e 672d 3429  var(--warning-4)
-00031110: 7d2e 6164 6d6f 6e69 7469 6f6e 2e73 6565  }.admonition.see
-00031120: 616c 736f 7b2d 2d69 636f 6e2d 7572 6c3a  also{--icon-url:
-00031130: 7661 7228 2d2d 7365 6561 6c73 6f2d 6963  var(--seealso-ic
-00031140: 6f6e 293b 2d2d 636f 6c6f 722d 313a 7661  on);--color-1:va
-00031150: 7228 2d2d 7365 6561 6c73 6f2d 3129 3b2d  r(--seealso-1);-
-00031160: 2d63 6f6c 6f72 2d32 3a76 6172 282d 2d73  -color-2:var(--s
-00031170: 6565 616c 736f 2d32 293b 2d2d 636f 6c6f  eealso-2);--colo
-00031180: 722d 333a 7661 7228 2d2d 7365 6561 6c73  r-3:var(--seeals
-00031190: 6f2d 3329 3b2d 2d63 6f6c 6f72 2d34 3a76  o-3);--color-4:v
-000311a0: 6172 282d 2d73 6565 616c 736f 2d34 297d  ar(--seealso-4)}
-000311b0: 2e61 646d 6f6e 6974 696f 6e2e 6164 6d6f  .admonition.admo
-000311c0: 6e69 7469 6f6e 2d74 6f64 6f7b 2d2d 6963  nition-todo{--ic
-000311d0: 6f6e 2d75 726c 3a76 6172 282d 2d74 6f64  on-url:var(--tod
-000311e0: 6f2d 6963 6f6e 293b 2d2d 636f 6c6f 722d  o-icon);--color-
-000311f0: 313a 7661 7228 2d2d 746f 646f 2d31 293b  1:var(--todo-1);
-00031200: 2d2d 636f 6c6f 722d 323a 7661 7228 2d2d  --color-2:var(--
-00031210: 746f 646f 2d32 293b 2d2d 636f 6c6f 722d  todo-2);--color-
-00031220: 333a 7661 7228 2d2d 746f 646f 2d33 293b  3:var(--todo-3);
-00031230: 2d2d 636f 6c6f 722d 343a 7661 7228 2d2d  --color-4:var(--
-00031240: 746f 646f 2d34 297d 2e61 646d 6f6e 6974  todo-4)}.admonit
-00031250: 696f 6e20 702e 6164 6d6f 6e69 7469 6f6e  ion p.admonition
-00031260: 2d74 6974 6c65 2b70 7b6d 6172 6769 6e2d  -title+p{margin-
-00031270: 746f 703a 307d 2e61 646d 6f6e 6974 696f  top:0}.admonitio
-00031280: 6e3e 3a6c 6173 742d 6368 696c 647b 6d61  n>:last-child{ma
-00031290: 7267 696e 2d62 6f74 746f 6d3a 307d 7370  rgin-bottom:0}sp
-000312a0: 616e 2e76 6572 7369 6f6e 6d6f 6469 6669  an.versionmodifi
-000312b0: 6564 7b63 6f6c 6f72 3a76 6172 282d 2d73  ed{color:var(--s
-000312c0: 792d 632d 626f 6c64 293b 666f 6e74 2d77  y-c-bold);font-w
-000312d0: 6569 6768 743a 3630 307d 6469 762e 6465  eight:600}div.de
-000312e0: 7072 6563 6174 6564 2c64 6976 2e76 6572  precated,div.ver
-000312f0: 7369 6f6e 6164 6465 642c 6469 762e 7665  sionadded,div.ve
-00031300: 7273 696f 6e63 6861 6e67 6564 7b70 6f73  rsionchanged{pos
-00031310: 6974 696f 6e3a 7265 6c61 7469 7665 3b70  ition:relative;p
-00031320: 6164 6469 6e67 3a36 7078 2031 7265 6d3b  adding:6px 1rem;
-00031330: 6d61 7267 696e 3a31 7265 6d20 303b 626f  margin:1rem 0;bo
-00031340: 7264 6572 2d6c 6566 743a 3470 7820 736f  rder-left:4px so
-00031350: 6c69 6420 7661 7228 2d2d 636f 6c6f 722d  lid var(--color-
-00031360: 3229 3b62 6163 6b67 726f 756e 642d 636f  2);background-co
-00031370: 6c6f 723a 7661 7228 2d2d 636f 6c6f 722d  lor:var(--color-
-00031380: 3129 3b6c 696e 652d 6865 6967 6874 3a31  1);line-height:1
-00031390: 2e37 327d 6469 762e 6465 7072 6563 6174  .72}div.deprecat
-000313a0: 6564 3a62 6566 6f72 652c 6469 762e 7665  ed:before,div.ve
-000313b0: 7273 696f 6e61 6464 6564 3a62 6566 6f72  rsionadded:befor
-000313c0: 652c 6469 762e 7665 7273 696f 6e63 6861  e,div.versioncha
-000313d0: 6e67 6564 3a62 6566 6f72 657b 706f 7369  nged:before{posi
-000313e0: 7469 6f6e 3a61 6273 6f6c 7574 653b 636f  tion:absolute;co
-000313f0: 6e74 656e 743a 7661 7228 2d2d 7665 7273  ntent:var(--vers
-00031400: 696f 6e2d 6963 6f6e 293b 746f 703a 3130  ion-icon);top:10
-00031410: 7078 3b6c 6566 743a 2d31 3270 783b 636f  px;left:-12px;co
-00031420: 6c6f 723a 2366 6666 3b77 6964 7468 3a32  lor:#fff;width:2
-00031430: 3070 783b 6865 6967 6874 3a32 3070 783b  0px;height:20px;
-00031440: 626f 7264 6572 2d72 6164 6975 733a 3130  border-radius:10
-00031450: 3025 3b62 6163 6b67 726f 756e 642d 636f  0%;background-co
-00031460: 6c6f 723a 7661 7228 2d2d 636f 6c6f 722d  lor:var(--color-
-00031470: 3229 3b74 6578 742d 616c 6967 6e3a 6365  2);text-align:ce
-00031480: 6e74 6572 3b66 6f6e 743a 6e6f 726d 616c  nter;font:normal
-00031490: 2037 3030 2031 3470 782f 3230 7078 2076   700 14px/20px v
-000314a0: 6172 282d 2d73 792d 662d 6d6f 6e6f 297d  ar(--sy-f-mono)}
-000314b0: 6469 762e 7665 7273 696f 6e61 6464 6564  div.versionadded
-000314c0: 7b2d 2d63 6f6c 6f72 2d31 3a76 6172 282d  {--color-1:var(-
-000314d0: 2d76 6572 7369 6f6e 6164 6465 642d 3129  -versionadded-1)
-000314e0: 3b2d 2d63 6f6c 6f72 2d32 3a76 6172 282d  ;--color-2:var(-
-000314f0: 2d76 6572 7369 6f6e 6164 6465 642d 3229  -versionadded-2)
-00031500: 3b2d 2d76 6572 7369 6f6e 2d69 636f 6e3a  ;--version-icon:
-00031510: 2223 227d 6469 762e 7665 7273 696f 6e63  "#"}div.versionc
-00031520: 6861 6e67 6564 7b2d 2d63 6f6c 6f72 2d31  hanged{--color-1
-00031530: 3a76 6172 282d 2d76 6572 7369 6f6e 6368  :var(--versionch
-00031540: 616e 6765 642d 3129 3b2d 2d63 6f6c 6f72  anged-1);--color
-00031550: 2d32 3a76 6172 282d 2d76 6572 7369 6f6e  -2:var(--version
-00031560: 6368 616e 6765 642d 3229 3b2d 2d76 6572  changed-2);--ver
-00031570: 7369 6f6e 2d69 636f 6e3a 2225 227d 6469  sion-icon:"%"}di
-00031580: 762e 6465 7072 6563 6174 6564 7b2d 2d63  v.deprecated{--c
-00031590: 6f6c 6f72 2d31 3a76 6172 282d 2d64 6570  olor-1:var(--dep
-000315a0: 7265 6361 7465 642d 3129 3b2d 2d63 6f6c  recated-1);--col
-000315b0: 6f72 2d32 3a76 6172 282d 2d64 6570 7265  or-2:var(--depre
-000315c0: 6361 7465 642d 3229 3b2d 2d76 6572 7369  cated-2);--versi
-000315d0: 6f6e 2d69 636f 6e3a 2221 227d 6469 762e  on-icon:"!"}div.
-000315e0: 6465 7072 6563 6174 6564 3e70 2c64 6976  deprecated>p,div
-000315f0: 2e76 6572 7369 6f6e 6164 6465 643e 702c  .versionadded>p,
-00031600: 6469 762e 7665 7273 696f 6e63 6861 6e67  div.versionchang
-00031610: 6564 3e70 7b6d 6172 6769 6e3a 307d 2e79  ed>p{margin:0}.y
-00031620: 7565 2062 6c6f 636b 7175 6f74 652e 6570  ue blockquote.ep
-00031630: 6967 7261 7068 7b70 6164 6469 6e67 3a31  igraph{padding:1
-00031640: 7265 6d20 322e 3472 656d 3b62 6f72 6465  rem 2.4rem;borde
-00031650: 722d 6c65 6674 3a30 3b74 6578 742d 616c  r-left:0;text-al
-00031660: 6967 6e3a 6365 6e74 6572 7d2e 7975 6520  ign:center}.yue 
-00031670: 626c 6f63 6b71 756f 7465 2e68 6967 686c  blockquote.highl
-00031680: 6967 6874 737b 626f 7264 6572 2d6c 6566  ights{border-lef
-00031690: 742d 7769 6474 683a 3470 783b 7061 6464  t-width:4px;padd
-000316a0: 696e 672d 746f 703a 2e32 7265 6d3b 7061  ing-top:.2rem;pa
-000316b0: 6464 696e 672d 626f 7474 6f6d 3a2e 3272  dding-bottom:.2r
-000316c0: 656d 3b62 6163 6b67 726f 756e 642d 636f  em;background-co
-000316d0: 6c6f 723a 7661 7228 2d2d 7379 2d63 2d73  lor:var(--sy-c-s
-000316e0: 7572 6661 6365 297d 2e79 7565 2062 6c6f  urface)}.yue blo
-000316f0: 636b 7175 6f74 652e 7075 6c6c 2d71 756f  ckquote.pull-quo
-00031700: 7465 7b70 6f73 6974 696f 6e3a 7265 6c61  te{position:rela
-00031710: 7469 7665 3b66 6f6e 742d 7369 7a65 3a31  tive;font-size:1
-00031720: 2e32 3472 656d 3b70 6164 6469 6e67 3a32  .24rem;padding:2
-00031730: 2e34 7265 6d20 332e 3672 656d 2031 2e32  .4rem 3.6rem 1.2
-00031740: 7265 6d3b 626f 7264 6572 2d6c 6566 743a  rem;border-left:
-00031750: 307d 2e79 7565 2062 6c6f 636b 7175 6f74  0}.yue blockquot
-00031760: 652e 7075 6c6c 2d71 756f 7465 3a62 6566  e.pull-quote:bef
-00031770: 6f72 657b 636f 6e74 656e 743a 225c 3230  ore{content:"\20
-00031780: 3163 223b 706f 7369 7469 6f6e 3a61 6273  1c";position:abs
-00031790: 6f6c 7574 653b 746f 703a 303b 6c65 6674  olute;top:0;left
-000317a0: 3a2e 3572 656d 3b63 6f6c 6f72 3a76 6172  :.5rem;color:var
-000317b0: 282d 2d79 7565 2d63 2d71 756f 7465 2d73  (--yue-c-quote-s
-000317c0: 796d 626f 6c29 3b66 6f6e 743a 3730 3020  ymbol);font:700 
-000317d0: 3472 656d 2f31 2054 696d 6573 204e 6577  4rem/1 Times New
-000317e0: 2052 6f6d 616e 2c47 656f 7267 6961 2c50   Roman,Georgia,P
-000317f0: 616c 6174 696e 6f2c 5469 6d65 732c 7365  alatino,Times,se
-00031800: 7269 667d 2e79 7565 2062 6c6f 636b 7175  rif}.yue blockqu
-00031810: 6f74 652e 7075 6c6c 2d71 756f 7465 202e  ote.pull-quote .
-00031820: 6174 7472 6962 7574 696f 6e7b 7465 7874  attribution{text
-00031830: 2d61 6c69 676e 3a72 6967 6874 7d70 7265  -align:right}pre
-00031840: 2e6c 6974 6572 616c 2d62 6c6f 636b 7b6c  .literal-block{l
-00031850: 696e 652d 6865 6967 6874 3a31 2e34 383b  ine-height:1.48;
-00031860: 7061 6464 696e 673a 3172 656d 3b66 6f6e  padding:1rem;fon
-00031870: 742d 7369 7a65 3a2e 3936 7265 6d3b 6261  t-size:.96rem;ba
-00031880: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3a76  ckground-color:v
-00031890: 6172 282d 2d73 796e 7461 782d 7072 652d  ar(--syntax-pre-
-000318a0: 6267 293b 626f 7264 6572 2d72 6164 6975  bg);border-radiu
-000318b0: 733a 3670 783b 6f76 6572 666c 6f77 3a61  s:6px;overflow:a
-000318c0: 7574 6f7d 2e68 6967 686c 6967 6874 2c2e  uto}.highlight,.
-000318d0: 6c69 7465 7261 6c2d 626c 6f63 6b2d 7772  literal-block-wr
-000318e0: 6170 7065 727b 2d2d 6d61 7267 696e 3a31  apper{--margin:1
-000318f0: 7265 6d3b 2d2d 7261 6469 7573 3a36 7078  rem;--radius:6px
-00031900: 7d2e 6c69 7465 7261 6c2d 626c 6f63 6b2d  }.literal-block-
-00031910: 7772 6170 7065 7220 6469 765b 636c 6173  wrapper div[clas
-00031920: 735e 3d68 6967 686c 6967 6874 2d5d 7b64  s^=highlight-]{d
-00031930: 6973 706c 6179 3a66 6c65 787d 2e6c 6974  isplay:flex}.lit
-00031940: 6572 616c 2d62 6c6f 636b 2d77 7261 7070  eral-block-wrapp
-00031950: 6572 202e 6869 6768 6c69 6768 747b 7769  er .highlight{wi
-00031960: 6474 683a 3130 3025 7d2e 6869 6768 6c69  dth:100%}.highli
-00031970: 6768 743e 7072 657b 6c69 6e65 2d68 6569  ght>pre{line-hei
-00031980: 6768 743a 312e 3438 3b70 6164 6469 6e67  ght:1.48;padding
-00031990: 3a76 6172 282d 2d6d 6172 6769 6e29 3b66  :var(--margin);f
-000319a0: 6f6e 742d 7369 7a65 3a2e 3936 7265 6d3b  ont-size:.96rem;
-000319b0: 666f 6e74 2d66 616d 696c 793a 7661 7228  font-family:var(
-000319c0: 2d2d 7379 2d66 2d6d 6f6e 6f29 3b62 6163  --sy-f-mono);bac
-000319d0: 6b67 726f 756e 642d 636f 6c6f 723a 7661  kground-color:va
-000319e0: 7228 2d2d 7379 6e74 6178 2d70 7265 2d62  r(--syntax-pre-b
-000319f0: 6729 3b62 6f72 6465 722d 7261 6469 7573  g);border-radius
-00031a00: 3a76 6172 282d 2d72 6164 6975 7329 3b6f  :var(--radius);o
-00031a10: 7665 7266 6c6f 773a 6175 746f 7d2e 7769  verflow:auto}.wi
-00031a20: 6e20 2e68 6967 686c 6967 6874 3e70 7265  n .highlight>pre
-00031a30: 7b66 6f6e 742d 6661 6d69 6c79 3a22 5477  {font-family:"Tw
-00031a40: 656d 6f6a 6920 436f 756e 7472 7920 466c  emoji Country Fl
-00031a50: 6167 7322 2c76 6172 282d 2d73 792d 662d  ags",var(--sy-f-
-00031a60: 6d6f 6e6f 297d 2e68 6967 686c 6967 6874  mono)}.highlight
-00031a70: 202e 6c69 6e65 6e6f 737b 6469 7370 6c61   .linenos{displa
-00031a80: 793a 696e 6c69 6e65 2d62 6c6f 636b 3b62  y:inline-block;b
-00031a90: 6f78 2d73 6861 646f 773a 2d2e 3035 7265  ox-shadow:-.05re
-00031aa0: 6d20 3020 7661 7228 2d2d 7379 6e74 6178  m 0 var(--syntax
-00031ab0: 2d6c 696e 656e 6f73 2d64 6976 6964 6572  -linenos-divider
-00031ac0: 2920 696e 7365 743b 2d77 6562 6b69 742d  ) inset;-webkit-
-00031ad0: 7573 6572 2d73 656c 6563 743a 6e6f 6e65  user-select:none
-00031ae0: 3b2d 6d6f 7a2d 7573 6572 2d73 656c 6563  ;-moz-user-selec
-00031af0: 743a 6e6f 6e65 3b75 7365 722d 7365 6c65  t:none;user-sele
-00031b00: 6374 3a6e 6f6e 653b 6d61 7267 696e 2d72  ct:none;margin-r
-00031b10: 6967 6874 3a2e 3872 656d 3b70 6164 6469  ight:.8rem;paddi
-00031b20: 6e67 2d72 6967 6874 3a2e 3872 656d 3b6f  ng-right:.8rem;o
-00031b30: 7061 6369 7479 3a2e 367d 2e68 6967 686c  pacity:.6}.highl
-00031b40: 6967 6874 202e 686c 6c7b 6d61 7267 696e  ight .hll{margin
-00031b50: 2d6c 6566 743a 6361 6c63 2830 7265 6d20  -left:calc(0rem 
-00031b60: 2d20 7661 7228 2d2d 6d61 7267 696e 2929  - var(--margin))
-00031b70: 3b6d 6172 6769 6e2d 7269 6768 743a 6361  ;margin-right:ca
-00031b80: 6c63 2830 7265 6d20 2d20 7661 7228 2d2d  lc(0rem - var(--
-00031b90: 6d61 7267 696e 2929 3b70 6164 6469 6e67  margin));padding
-00031ba0: 3a30 2076 6172 282d 2d6d 6172 6769 6e29  :0 var(--margin)
-00031bb0: 7d2e 636f 6465 2d62 6c6f 636b 2d63 6170  }.code-block-cap
-00031bc0: 7469 6f6e 7b64 6973 706c 6179 3a66 6c65  tion{display:fle
-00031bd0: 783b 666f 6e74 2d73 697a 653a 2e38 3472  x;font-size:.84r
-00031be0: 656d 3b66 6f6e 742d 7765 6967 6874 3a36  em;font-weight:6
-00031bf0: 3030 3b63 6f6c 6f72 3a76 6172 282d 2d73  00;color:var(--s
-00031c00: 796e 7461 782d 7465 7874 293b 6261 636b  yntax-text);back
-00031c10: 6772 6f75 6e64 2d63 6f6c 6f72 3a76 6172  ground-color:var
-00031c20: 282d 2d73 796e 7461 782d 6361 702d 6267  (--syntax-cap-bg
-00031c30: 293b 7061 6464 696e 673a 2e34 7265 6d20  );padding:.4rem 
-00031c40: 7661 7228 2d2d 6d61 7267 696e 293b 626f  var(--margin);bo
-00031c50: 7264 6572 2d72 6164 6975 733a 7661 7228  rder-radius:var(
-00031c60: 2d2d 7261 6469 7573 2920 7661 7228 2d2d  --radius) var(--
-00031c70: 7261 6469 7573 2920 3020 307d 2e63 6f64  radius) 0 0}.cod
-00031c80: 652d 626c 6f63 6b2d 6361 7074 696f 6e2b  e-block-caption+
-00031c90: 6469 763e 2e68 6967 686c 6967 6874 3e70  div>.highlight>p
-00031ca0: 7265 7b62 6f72 6465 722d 746f 702d 6c65  re{border-top-le
-00031cb0: 6674 2d72 6164 6975 733a 303b 626f 7264  ft-radius:0;bord
-00031cc0: 6572 2d74 6f70 2d72 6967 6874 2d72 6164  er-top-right-rad
-00031cd0: 6975 733a 307d 6469 765b 636c 6173 735e  ius:0}div[class^
-00031ce0: 3d68 6967 686c 6967 6874 5d3e 2e68 6967  =highlight]>.hig
-00031cf0: 686c 6967 6874 3e70 7265 7b64 6973 706c  hlight>pre{displ
-00031d00: 6179 3a67 7269 647d 2e79 7565 202e 7461  ay:grid}.yue .ta
-00031d10: 626c 652d 7772 6170 7065 727b 7769 6474  ble-wrapper{widt
-00031d20: 683a 3130 3025 3b6f 7665 7266 6c6f 772d  h:100%;overflow-
-00031d30: 783a 6175 746f 3b6d 6172 6769 6e2d 746f  x:auto;margin-to
-00031d40: 703a 3272 656d 3b6d 6172 6769 6e2d 626f  p:2rem;margin-bo
-00031d50: 7474 6f6d 3a32 7265 6d3b 626f 7264 6572  ttom:2rem;border
-00031d60: 3a31 7078 2073 6f6c 6964 2076 6172 282d  :1px solid var(-
-00031d70: 2d79 7565 2d63 2d74 6162 6c65 2d62 6f72  -yue-c-table-bor
-00031d80: 6465 7229 3b62 6f72 6465 722d 7261 6469  der);border-radi
-00031d90: 7573 3a36 7078 7d2e 7975 6520 2e74 6162  us:6px}.yue .tab
-00031da0: 6c65 2d77 7261 7070 6572 3e74 6162 6c65  le-wrapper>table
-00031db0: 7b6d 6172 6769 6e3a 307d 2e79 7565 202e  {margin:0}.yue .
-00031dc0: 7461 626c 652d 7772 6170 7065 7220 7468  table-wrapper th
-00031dd0: 6561 6420 7472 7b62 6f72 6465 722d 746f  ead tr{border-to
-00031de0: 703a 3170 7820 736f 6c69 6420 7661 7228  p:1px solid var(
-00031df0: 2d2d 7975 652d 632d 7464 2d62 6f72 6465  --yue-c-td-borde
-00031e00: 7229 7d2e 7975 6520 2e74 6162 6c65 2d77  r)}.yue .table-w
-00031e10: 7261 7070 6572 2074 6865 6164 2074 723a  rapper thead tr:
-00031e20: 6669 7273 742d 6368 696c 647b 626f 7264  first-child{bord
-00031e30: 6572 2d74 6f70 3a30 7d2e 7975 6520 2e74  er-top:0}.yue .t
-00031e40: 6162 6c65 2d77 7261 7070 6572 2074 687b  able-wrapper th{
-00031e50: 6261 636b 6772 6f75 6e64 2d63 6f6c 6f72  background-color
-00031e60: 3a76 6172 282d 2d79 7565 2d63 2d74 682d  :var(--yue-c-th-
-00031e70: 6261 636b 6772 6f75 6e64 293b 626f 7264  background);bord
-00031e80: 6572 2d6c 6566 743a 3170 7820 736f 6c69  er-left:1px soli
-00031e90: 6420 7661 7228 2d2d 7975 652d 632d 7464  d var(--yue-c-td
-00031ea0: 2d62 6f72 6465 7229 3b70 6164 6469 6e67  -border);padding
-00031eb0: 3a2e 3732 3572 656d 2031 7265 6d7d 2e79  :.725rem 1rem}.y
-00031ec0: 7565 202e 7461 626c 652d 7772 6170 7065  ue .table-wrappe
-00031ed0: 7220 7464 7b62 6f72 6465 722d 6c65 6674  r td{border-left
-00031ee0: 3a31 7078 2073 6f6c 6964 2076 6172 282d  :1px solid var(-
-00031ef0: 2d79 7565 2d63 2d74 642d 626f 7264 6572  -yue-c-td-border
-00031f00: 293b 7061 6464 696e 673a 2e35 7265 6d20  );padding:.5rem 
-00031f10: 3172 656d 7d2e 7975 6520 2e74 6162 6c65  1rem}.yue .table
-00031f20: 2d77 7261 7070 6572 2074 723e 7464 3a66  -wrapper tr>td:f
-00031f30: 6972 7374 2d63 6869 6c64 2c2e 7975 6520  irst-child,.yue 
-00031f40: 2e74 6162 6c65 2d77 7261 7070 6572 2074  .table-wrapper t
-00031f50: 723e 7468 3a66 6972 7374 2d63 6869 6c64  r>th:first-child
-00031f60: 7b62 6f72 6465 722d 6c65 6674 3a30 7d2e  {border-left:0}.
-00031f70: 7975 6520 2e74 6162 6c65 2d77 7261 7070  yue .table-wrapp
-00031f80: 6572 2063 6170 7469 6f6e 7b70 6164 6469  er caption{paddi
-00031f90: 6e67 3a2e 3572 656d 3b6d 6172 6769 6e3a  ng:.5rem;margin:
-00031fa0: 303b 626f 7264 6572 2d62 6f74 746f 6d3a  0;border-bottom:
-00031fb0: 3170 7820 736f 6c69 6420 7661 7228 2d2d  1px solid var(--
-00031fc0: 7975 652d 632d 7468 2d62 6f72 6465 7229  yue-c-th-border)
-00031fd0: 7d2e 7975 6520 2e74 6162 6c65 2d77 7261  }.yue .table-wra
-00031fe0: 7070 6572 2074 626f 6479 2074 722e 726f  pper tbody tr.ro
-00031ff0: 772d 6f64 647b 6261 636b 6772 6f75 6e64  w-odd{background
-00032000: 2d63 6f6c 6f72 3a76 6172 282d 2d79 7565  -color:var(--yue
-00032010: 2d63 2d72 6f77 2d62 6163 6b67 726f 756e  -c-row-backgroun
-00032020: 6429 7d2e 7975 6520 7461 626c 652e 686c  d)}.yue table.hl
-00032030: 6973 7420 7464 7b76 6572 7469 6361 6c2d  ist td{vertical-
-00032040: 616c 6967 6e3a 746f 707d 2e74 6162 6c65  align:top}.table
-00032050: 2d77 7261 7070 6572 7b6f 7665 7266 6c6f  -wrapper{overflo
-00032060: 772d 783a 6175 746f 3b73 6372 6f6c 6c62  w-x:auto;scrollb
-00032070: 6172 2d67 7574 7465 723a 6175 746f 7d2e  ar-gutter:auto}.
-00032080: 7461 626c 652d 7772 6170 7065 723a 3a2d  table-wrapper::-
-00032090: 7765 626b 6974 2d73 6372 6f6c 6c62 6172  webkit-scrollbar
-000320a0: 7b68 6569 6768 743a 2e37 3572 656d 3b77  {height:.75rem;w
-000320b0: 6964 7468 3a2e 3735 7265 6d7d 2e74 6162  idth:.75rem}.tab
-000320c0: 6c65 2d77 7261 7070 6572 3a3a 2d77 6562  le-wrapper::-web
-000320d0: 6b69 742d 7363 726f 6c6c 6261 722d 7468  kit-scrollbar-th
-000320e0: 756d 627b 626f 7264 6572 2d72 6164 6975  umb{border-radiu
-000320f0: 733a 3130 7078 7d2e 7461 626c 652d 7772  s:10px}.table-wr
-00032100: 6170 7065 723a 3a2d 7765 626b 6974 2d73  apper::-webkit-s
-00032110: 6372 6f6c 6c62 6172 2d74 7261 636b 7b62  crollbar-track{b
-00032120: 6163 6b67 726f 756e 642d 636f 6c6f 723a  ackground-color:
-00032130: 696e 6974 6961 6c7d 2e74 6162 6c65 2d77  initial}.table-w
-00032140: 7261 7070 6572 3a68 6f76 6572 3a3a 2d77  rapper:hover::-w
-00032150: 6562 6b69 742d 7363 726f 6c6c 6261 722d  ebkit-scrollbar-
-00032160: 7468 756d 627b 6261 636b 6772 6f75 6e64  thumb{background
-00032170: 2d63 6f6c 6f72 3a23 3962 3962 3962 3333  -color:#9b9b9b33
-00032180: 3b62 6163 6b67 726f 756e 642d 636c 6970  ;background-clip
-00032190: 3a63 6f6e 7465 6e74 2d62 6f78 3b62 6f72  :content-box;bor
-000321a0: 6465 723a 3370 7820 736f 6c69 6420 2330  der:3px solid #0
-000321b0: 3030 307d 2e79 7565 2074 6162 6c65 2e67  000}.yue table.g
-000321c0: 686f 7374 2074 642c 2e79 7565 2074 6162  host td,.yue tab
-000321d0: 6c65 2e67 686f 7374 2074 687b 626f 7264  le.ghost th{bord
-000321e0: 6572 2d6c 6566 743a 303b 626f 7264 6572  er-left:0;border
-000321f0: 2d72 6967 6874 3a30 3b62 6163 6b67 726f  -right:0;backgro
-00032200: 756e 642d 636f 6c6f 723a 696e 6974 6961  und-color:initia
-00032210: 6c7d 2e79 7565 2074 6162 6c65 2e67 686f  l}.yue table.gho
-00032220: 7374 2063 6170 7469 6f6e 7b6d 6172 6769  st caption{margi
-00032230: 6e2d 626f 7474 6f6d 3a30 3b70 6164 6469  n-bottom:0;paddi
-00032240: 6e67 2d62 6f74 746f 6d3a 2e35 7265 6d3b  ng-bottom:.5rem;
-00032250: 626f 7264 6572 2d62 6f74 746f 6d3a 3370  border-bottom:3p
-00032260: 7820 736f 6c69 6420 7661 7228 2d2d 7975  x solid var(--yu
-00032270: 652d 632d 7464 2d62 6f72 6465 7229 7d2e  e-c-td-border)}.
-00032280: 7975 6520 7461 626c 652e 6768 6f73 7420  yue table.ghost 
-00032290: 7468 6561 6420 7472 3a66 6972 7374 2d63  thead tr:first-c
-000322a0: 6869 6c64 7b62 6f72 6465 722d 746f 703a  hild{border-top:
-000322b0: 303b 626f 7264 6572 2d62 6f74 746f 6d2d  0;border-bottom-
-000322c0: 7769 6474 683a 3370 787d 2e79 7565 202e  width:3px}.yue .
-000322d0: 7461 626c 652d 7772 6170 7065 722e 6768  table-wrapper.gh
-000322e0: 6f73 747b 626f 7264 6572 3a30 7d3a 726f  ost{border:0}:ro
-000322f0: 6f74 7b2d 2d73 6967 2d70 726f 7065 7274  ot{--sig-propert
-00032300: 793a 7661 7228 2d2d 7379 6e74 6178 2d6b  y:var(--syntax-k
-00032310: 6579 776f 7264 293b 2d2d 7369 672d 6e61  eyword);--sig-na
-00032320: 6d65 3a76 6172 282d 2d73 796e 7461 782d  me:var(--syntax-
-00032330: 7072 6f70 6572 7479 293b 2d2d 7369 672d  property);--sig-
-00032340: 7479 7065 6869 6e74 3a76 6172 282d 2d73  typehint:var(--s
-00032350: 796e 7461 782d 636f 6e73 7461 6e74 293b  yntax-constant);
-00032360: 2d2d 7369 672d 7061 7261 6d3a 7661 7228  --sig-param:var(
-00032370: 2d2d 7379 6e74 6178 2d6d 6574 6129 7d64  --syntax-meta)}d
-00032380: 742e 7369 677b 706f 7369 7469 6f6e 3a72  t.sig{position:r
-00032390: 656c 6174 6976 653b 666f 6e74 2d73 697a  elative;font-siz
-000323a0: 653a 2e39 3272 656d 3b70 6164 6469 6e67  e:.92rem;padding
-000323b0: 3a2e 3235 7265 6d20 2e35 7265 6d20 2e32  :.25rem .5rem .2
-000323c0: 3572 656d 2033 7265 6d3b 7465 7874 2d69  5rem 3rem;text-i
-000323d0: 6e64 656e 743a 2d32 2e34 7265 6d3b 626f  ndent:-2.4rem;bo
-000323e0: 7264 6572 2d72 6164 6975 733a 3670 787d  rder-radius:6px}
-000323f0: 6474 2e73 6967 3a61 6674 6572 7b63 6f6e  dt.sig:after{con
-00032400: 7465 6e74 3a22 223b 6469 7370 6c61 793a  tent:"";display:
-00032410: 7461 626c 653b 636c 6561 723a 626f 7468  table;clear:both
-00032420: 7d64 742e 7369 673a 686f 7665 727b 6261  }dt.sig:hover{ba
-00032430: 636b 6772 6f75 6e64 3a76 6172 282d 2d73  ckground:var(--s
-00032440: 792d 632d 7375 7266 6163 6529 7d64 742e  y-c-surface)}dt.
-00032450: 7369 672b 6464 7b66 6f6e 742d 7369 7a65  sig+dd{font-size
-00032460: 3a2e 3932 7265 6d3b 6d61 7267 696e 2d6c  :.92rem;margin-l
-00032470: 6566 743a 3272 656d 7d64 742e 7369 673e  eft:2rem}dt.sig>
-00032480: 656d 2e70 726f 7065 7274 793a 6669 7273  em.property:firs
-00032490: 742d 6368 696c 647b 636f 6c6f 723a 7661  t-child{color:va
-000324a0: 7228 2d2d 7369 672d 7072 6f70 6572 7479  r(--sig-property
-000324b0: 297d 646c 2e66 6965 6c64 2d6c 6973 7420  )}dl.field-list 
-000324c0: 617b 666f 6e74 2d77 6569 6768 743a 3430  a{font-weight:40
-000324d0: 307d 6474 2e73 6967 2b64 643e 6469 767b  0}dt.sig+dd>div{
-000324e0: 6d61 7267 696e 2d62 6f74 746f 6d3a 3172  margin-bottom:1r
-000324f0: 656d 7d64 742e 7369 672b 6464 3e64 6c2e  em}dt.sig+dd>dl.
-00032500: 6669 656c 642d 6c69 7374 3e64 747b 7465  field-list>dt{te
-00032510: 7874 2d74 7261 6e73 666f 726d 3a75 7070  xt-transform:upp
-00032520: 6572 6361 7365 3b66 6f6e 742d 7369 7a65  ercase;font-size
-00032530: 3a2e 3736 7265 6d7d 656d 2e70 726f 7065  :.76rem}em.prope
-00032540: 7274 792c 656d 2e73 6967 2d70 6172 616d  rty,em.sig-param
-00032550: 7b66 6f6e 742d 7374 796c 653a 6e6f 726d  {font-style:norm
-00032560: 616c 7d65 6d2e 7369 672d 7061 7261 6d7b  al}em.sig-param{
-00032570: 636f 6c6f 723a 7661 7228 2d2d 7379 2d63  color:var(--sy-c
-00032580: 2d6c 6967 6874 297d 7370 616e 2e73 6967  -light)}span.sig
-00032590: 2d6e 616d 652c 7370 616e 2e73 6967 2d70  -name,span.sig-p
-000325a0: 7265 6e61 6d65 7b63 6f6c 6f72 3a76 6172  rename{color:var
-000325b0: 282d 2d73 6967 2d6e 616d 6529 7d73 7061  (--sig-name)}spa
-000325c0: 6e2e 7369 672d 6e61 6d65 7b66 6f6e 742d  n.sig-name{font-
-000325d0: 7765 6967 6874 3a36 3030 7d73 7061 6e2e  weight:600}span.
-000325e0: 7369 672d 7265 7475 726e 2d69 636f 6e7b  sig-return-icon{
-000325f0: 636f 6c6f 723a 7661 7228 2d2d 7379 2d63  color:var(--sy-c
-00032600: 2d6c 6967 6874 297d 7370 616e 2e73 6967  -light)}span.sig
-00032610: 2d72 6574 7572 6e2d 7479 7065 6869 6e74  -return-typehint
-00032620: 2c73 7061 6e2e 7369 672d 7265 7475 726e  ,span.sig-return
-00032630: 2d74 7970 6568 696e 743e 617b 636f 6c6f  -typehint>a{colo
-00032640: 723a 7661 7228 2d2d 7369 672d 7479 7065  r:var(--sig-type
-00032650: 6869 6e74 297d 7370 616e 2e70 7265 2c73  hint)}span.pre,s
-00032660: 7061 6e2e 7369 672d 7061 7265 6e7b 666f  pan.sig-paren{fo
-00032670: 6e74 2d66 616d 696c 793a 7661 7228 2d2d  nt-family:var(--
-00032680: 7379 2d66 2d6d 6f6e 6f29 7d64 742e 7369  sy-f-mono)}dt.si
-00032690: 673e 612e 696e 7465 726e 616c 7b66 6f6e  g>a.internal{fon
-000326a0: 742d 7369 7a65 3a2e 3832 7265 6d3b 626f  t-size:.82rem;bo
-000326b0: 7264 6572 3a30 3b63 6f6c 6f72 3a76 6172  rder:0;color:var
-000326c0: 282d 2d73 792d 632d 6c69 6768 7429 7d64  (--sy-c-light)}d
-000326d0: 742e 7369 673e 612e 696e 7465 726e 616c  t.sig>a.internal
-000326e0: 3a62 6566 6f72 657b 636f 6e74 656e 743a  :before{content:
-000326f0: 225c 6122 3b77 6869 7465 2d73 7061 6365  "\a";white-space
-00032700: 3a70 7265 7d2e 7669 6577 636f 6465 2d62  :pre}.viewcode-b
-00032710: 6c6f 636b 7b70 6f73 6974 696f 6e3a 7265  lock{position:re
-00032720: 6c61 7469 7665 7d2e 7669 6577 636f 6465  lative}.viewcode
-00032730: 2d62 6163 6b7b 706f 7369 7469 6f6e 3a61  -back{position:a
-00032740: 6273 6f6c 7574 653b 746f 703a 2d31 2e35  bsolute;top:-1.5
-00032750: 7265 6d3b 666f 6e74 2d73 697a 653a 2e38  rem;font-size:.8
-00032760: 7265 6d7d 2e63 6c61 7373 6966 6965 727b  rem}.classifier{
-00032770: 666f 6e74 2d73 7479 6c65 3a6f 626c 6971  font-style:obliq
-00032780: 7565 3b66 6f6e 742d 7765 6967 6874 3a34  ue;font-weight:4
-00032790: 3030 7d2e 636c 6173 7369 6669 6572 3a62  00}.classifier:b
-000327a0: 6566 6f72 657b 666f 6e74 2d73 7479 6c65  efore{font-style
-000327b0: 3a6e 6f72 6d61 6c3b 6d61 7267 696e 2d6c  :normal;margin-l
-000327c0: 6566 743a 2e31 7265 6d3b 6d61 7267 696e  eft:.1rem;margin
-000327d0: 2d72 6967 6874 3a2e 3572 656d 3b63 6f6e  -right:.5rem;con
-000327e0: 7465 6e74 3a22 3a22 3b64 6973 706c 6179  tent:":";display
-000327f0: 3a69 6e6c 696e 652d 626c 6f63 6b7d 2e79  :inline-block}.y
-00032800: 7565 202e 7461 626c 652d 7772 6170 7065  ue .table-wrappe
-00032810: 722e 6175 746f 7375 6d6d 6172 797b 626f  r.autosummary{bo
-00032820: 7264 6572 2d6c 6566 743a 303b 626f 7264  rder-left:0;bord
-00032830: 6572 2d72 6967 6874 3a30 3b62 6f72 6465  er-right:0;borde
-00032840: 722d 7261 6469 7573 3a30 7d2e 7975 6520  r-radius:0}.yue 
-00032850: 2e74 6162 6c65 2d77 7261 7070 6572 2074  .table-wrapper t
-00032860: 6162 6c65 2e61 7574 6f73 756d 6d61 7279  able.autosummary
-00032870: 2074 647b 626f 7264 6572 3a6e 6f6e 653b   td{border:none;
-00032880: 7061 6464 696e 672d 746f 703a 2e32 3572  padding-top:.25r
-00032890: 656d 3b70 6164 6469 6e67 2d62 6f74 746f  em;padding-botto
-000328a0: 6d3a 2e32 3572 656d 7d2e 7975 6520 702e  m:.25rem}.yue p.
-000328b0: 7275 6272 6963 2b64 6976 2e61 7574 6f73  rubric+div.autos
-000328c0: 756d 6d61 7279 7b6d 6172 6769 6e2d 746f  ummary{margin-to
-000328d0: 703a 307d 3a72 6f6f 747b 2d2d 7379 6e74  p:0}:root{--synt
-000328e0: 6178 2d70 7265 2d62 673a 7661 7228 2d2d  ax-pre-bg:var(--
-000328f0: 6163 6365 6e74 2d61 3229 3b2d 2d73 796e  accent-a2);--syn
-00032900: 7461 782d 6361 702d 6267 3a76 6172 282d  tax-cap-bg:var(-
-00032910: 2d61 6363 656e 742d 6133 293b 2d2d 7379  -accent-a3);--sy
-00032920: 6e74 6178 2d68 6967 686c 6967 6874 2d62  ntax-highlight-b
-00032930: 673a 7661 7228 2d2d 6163 6365 6e74 2d61  g:var(--accent-a
-00032940: 3329 3b2d 2d73 796e 7461 782d 6c69 6e65  3);--syntax-line
-00032950: 6e6f 732d 6469 7669 6465 723a 7661 7228  nos-divider:var(
-00032960: 2d2d 6772 6179 2d61 3629 3b2d 2d73 796e  --gray-a6);--syn
-00032970: 7461 782d 6c69 6768 742d 7465 7874 3a23  tax-light-text:#
-00032980: 3234 3239 3266 3b2d 2d73 796e 7461 782d  24292f;--syntax-
-00032990: 6c69 6768 742d 6d65 7461 3a23 3830 3763  light-meta:#807c
-000329a0: 3837 3b2d 2d73 796e 7461 782d 6c69 6768  87;--syntax-ligh
-000329b0: 742d 636f 6d6d 656e 743a 2336 6537 3738  t-comment:#6e778
-000329c0: 313b 2d2d 7379 6e74 6178 2d6c 6967 6874  1;--syntax-light
-000329d0: 2d63 6f6e 7374 616e 743a 2330 3535 3061  -constant:#0550a
-000329e0: 653b 2d2d 7379 6e74 6178 2d6c 6967 6874  e;--syntax-light
-000329f0: 2d65 6e74 6974 793a 2332 3638 6264 323b  -entity:#268bd2;
-00032a00: 2d2d 7379 6e74 6178 2d6c 6967 6874 2d70  --syntax-light-p
-00032a10: 726f 7065 7274 793a 2338 3235 3064 663b  roperty:#8250df;
-00032a20: 2d2d 7379 6e74 6178 2d6c 6967 6874 2d64  --syntax-light-d
-00032a30: 6566 696e 6974 696f 6e3a 2332 3432 3932  efinition:#24292
-00032a40: 663b 2d2d 7379 6e74 6178 2d6c 6967 6874  f;--syntax-light
-00032a50: 2d74 6167 3a23 3038 353b 2d2d 7379 6e74  -tag:#085;--synt
-00032a60: 6178 2d6c 6967 6874 2d62 7569 6c74 696e  ax-light-builtin
-00032a70: 3a23 6235 3839 3030 3b2d 2d73 796e 7461  :#b58900;--synta
-00032a80: 782d 6c69 6768 742d 6b65 7977 6f72 643a  x-light-keyword:
-00032a90: 2363 6632 3232 653b 2d2d 7379 6e74 6178  #cf222e;--syntax
-00032aa0: 2d6c 6967 6874 2d65 7863 6570 7469 6f6e  -light-exception
-00032ab0: 3a23 6536 3231 3265 3b2d 2d73 796e 7461  :#e6212e;--synta
-00032ac0: 782d 6c69 6768 742d 7374 7269 6e67 3a23  x-light-string:#
-00032ad0: 3061 3330 3639 3b2d 2d73 796e 7461 782d  0a3069;--syntax-
-00032ae0: 6c69 6768 742d 7265 6765 7870 3a23 6534  light-regexp:#e4
-00032af0: 303b 2d2d 7379 6e74 6178 2d6c 6967 6874  0;--syntax-light
-00032b00: 2d76 6172 6961 626c 653a 2361 3434 3830  -variable:#a4480
-00032b10: 663b 2d2d 7379 6e74 6178 2d6c 6967 6874  f;--syntax-light
-00032b20: 2d69 6e76 616c 6964 2d69 6c6c 6567 616c  -invalid-illegal
-00032b30: 2d74 6578 743a 2366 3666 3866 613b 2d2d  -text:#f6f8fa;--
-00032b40: 7379 6e74 6178 2d6c 6967 6874 2d69 6e76  syntax-light-inv
-00032b50: 616c 6964 2d69 6c6c 6567 616c 2d62 673a  alid-illegal-bg:
-00032b60: 2338 3230 3731 653b 2d2d 7379 6e74 6178  #82071e;--syntax
-00032b70: 2d6c 6967 6874 2d6d 6172 6b75 702d 6865  -light-markup-he
-00032b80: 6164 696e 673a 2330 3535 3061 653b 2d2d  ading:#0550ae;--
-00032b90: 7379 6e74 6178 2d6c 6967 6874 2d6d 6172  syntax-light-mar
-00032ba0: 6b75 702d 6974 616c 6963 3a23 3234 3239  kup-italic:#2429
-00032bb0: 3266 3b2d 2d73 796e 7461 782d 6c69 6768  2f;--syntax-ligh
-00032bc0: 742d 6d61 726b 7570 2d62 6f6c 643a 2332  t-markup-bold:#2
+00030860: 293b 6469 7370 6c61 793a 666c 6578 3b66  );display:flex;f
+00030870: 6c65 782d 6469 7265 6374 696f 6e3a 636f  lex-direction:co
+00030880: 6c75 6d6e 3b70 6f73 6974 696f 6e3a 7265  lumn;position:re
+00030890: 6c61 7469 7665 3b70 6164 6469 6e67 3a30  lative;padding:0
+000308a0: 2031 3670 7820 2e38 7265 6d3b 6d61 7267   16px .8rem;marg
+000308b0: 696e 2d74 6f70 3a31 7265 6d3b 6d61 7267  in-top:1rem;marg
+000308c0: 696e 2d62 6f74 746f 6d3a 3172 656d 3b62  in-bottom:1rem;b
+000308d0: 6f72 6465 722d 6c65 6674 3a34 7078 2073  order-left:4px s
+000308e0: 6f6c 6964 2076 6172 282d 2d63 6f6c 6f72  olid var(--color
+000308f0: 2d33 293b 6261 636b 6772 6f75 6e64 2d63  -3);background-c
+00030900: 6f6c 6f72 3a76 6172 282d 2d63 6f6c 6f72  olor:var(--color
+00030910: 2d31 297d 2e61 646d 6f6e 6974 696f 6e3a  -1)}.admonition:
+00030920: 6265 666f 7265 7b70 6f73 6974 696f 6e3a  before{position:
+00030930: 6162 736f 6c75 7465 3b63 6f6e 7465 6e74  absolute;content
+00030940: 3a22 223b 746f 703a 3670 783b 6c65 6674  :"";top:6px;left
+00030950: 3a2d 3132 7078 3b77 6964 7468 3a32 3070  :-12px;width:20p
+00030960: 783b 6865 6967 6874 3a32 3070 783b 626f  x;height:20px;bo
+00030970: 7264 6572 2d72 6164 6975 733a 3130 3025  rder-radius:100%
+00030980: 3b62 6163 6b67 726f 756e 642d 636f 6c6f  ;background-colo
+00030990: 723a 7661 7228 2d2d 636f 6c6f 722d 3329  r:var(--color-3)
+000309a0: 7d2e 6164 6d6f 6e69 7469 6f6e 2070 2e61  }.admonition p.a
+000309b0: 646d 6f6e 6974 696f 6e2d 7469 746c 657b  dmonition-title{
+000309c0: 706f 7369 7469 6f6e 3a72 656c 6174 6976  position:relativ
+000309d0: 653b 6d61 7267 696e 3a30 202d 3136 7078  e;margin:0 -16px
+000309e0: 202e 3872 656d 202d 3139 7078 3b70 6164   .8rem -19px;pad
+000309f0: 6469 6e67 3a34 7078 2031 3870 783b 666f  ding:4px 18px;fo
+00030a00: 6e74 2d73 697a 653a 2e38 3572 656d 3b66  nt-size:.85rem;f
+00030a10: 6f6e 742d 7765 6967 6874 3a36 3030 3b6c  ont-weight:600;l
+00030a20: 696e 652d 6865 6967 6874 3a31 2e37 323b  ine-height:1.72;
+00030a30: 636f 6c6f 723a 7661 7228 2d2d 636f 6c6f  color:var(--colo
+00030a40: 722d 3429 3b62 6163 6b67 726f 756e 642d  r-4);background-
+00030a50: 636f 6c6f 723a 7661 7228 2d2d 636f 6c6f  color:var(--colo
+00030a60: 722d 3229 3b2d 2d79 7565 2d63 2d63 6f64  r-2);--yue-c-cod
+00030a70: 653a 7661 7228 2d2d 636f 6c6f 722d 3429  e:var(--color-4)
+00030a80: 3b2d 2d79 7565 2d63 2d62 6f6c 643a 7661  ;--yue-c-bold:va
+00030a90: 7228 2d2d 636f 6c6f 722d 3429 7d2e 6164  r(--color-4)}.ad
+00030aa0: 6d6f 6e69 7469 6f6e 2070 2e61 646d 6f6e  monition p.admon
+00030ab0: 6974 696f 6e2d 7469 746c 6520 7376 677b  ition-title svg{
+00030ac0: 6469 7370 6c61 793a 696e 6c69 6e65 2d62  display:inline-b
+00030ad0: 6c6f 636b 7d2e 6164 6d6f 6e69 7469 6f6e  lock}.admonition
+00030ae0: 2d74 6974 6c65 3a62 6566 6f72 657b 706f  -title:before{po
+00030af0: 7369 7469 6f6e 3a61 6273 6f6c 7574 653b  sition:absolute;
+00030b00: 636f 6e74 656e 743a 2222 3b74 6f70 3a31  content:"";top:1
+00030b10: 3070 783b 6c65 6674 3a2d 3570 783b 2d77  0px;left:-5px;-w
+00030b20: 6562 6b69 742d 6d61 736b 3a76 6172 282d  ebkit-mask:var(-
+00030b30: 2d69 636f 6e2d 7572 6c29 206e 6f2d 7265  -icon-url) no-re
+00030b40: 7065 6174 3b6d 6173 6b3a 7661 7228 2d2d  peat;mask:var(--
+00030b50: 6963 6f6e 2d75 726c 2920 6e6f 2d72 6570  icon-url) no-rep
+00030b60: 6561 743b 2d77 6562 6b69 742d 6d61 736b  eat;-webkit-mask
+00030b70: 2d73 697a 653a 3130 3025 2031 3030 253b  -size:100% 100%;
+00030b80: 6d61 736b 2d73 697a 653a 3130 3025 2031  mask-size:100% 1
+00030b90: 3030 253b 666f 6e74 2d73 7479 6c65 3a6e  00%;font-style:n
+00030ba0: 6f72 6d61 6c3b 7769 6474 683a 3132 7078  ormal;width:12px
+00030bb0: 3b68 6569 6768 743a 3132 7078 3b62 6163  ;height:12px;bac
+00030bc0: 6b67 726f 756e 642d 636f 6c6f 723a 2366  kground-color:#f
+00030bd0: 6666 7d2e 6164 6d6f 6e69 7469 6f6e 2e61  ff}.admonition.a
+00030be0: 7474 656e 7469 6f6e 7b2d 2d69 636f 6e2d  ttention{--icon-
+00030bf0: 7572 6c3a 7661 7228 2d2d 6174 7465 6e74  url:var(--attent
+00030c00: 696f 6e2d 6963 6f6e 293b 2d2d 636f 6c6f  ion-icon);--colo
+00030c10: 722d 313a 7661 7228 2d2d 6174 7465 6e74  r-1:var(--attent
+00030c20: 696f 6e2d 3129 3b2d 2d63 6f6c 6f72 2d32  ion-1);--color-2
+00030c30: 3a76 6172 282d 2d61 7474 656e 7469 6f6e  :var(--attention
+00030c40: 2d32 293b 2d2d 636f 6c6f 722d 333a 7661  -2);--color-3:va
+00030c50: 7228 2d2d 6174 7465 6e74 696f 6e2d 3329  r(--attention-3)
+00030c60: 3b2d 2d63 6f6c 6f72 2d34 3a76 6172 282d  ;--color-4:var(-
+00030c70: 2d61 7474 656e 7469 6f6e 2d34 297d 2e61  -attention-4)}.a
+00030c80: 646d 6f6e 6974 696f 6e2e 6361 7574 696f  dmonition.cautio
+00030c90: 6e7b 2d2d 6963 6f6e 2d75 726c 3a76 6172  n{--icon-url:var
+00030ca0: 282d 2d63 6175 7469 6f6e 2d69 636f 6e29  (--caution-icon)
+00030cb0: 3b2d 2d63 6f6c 6f72 2d31 3a76 6172 282d  ;--color-1:var(-
+00030cc0: 2d63 6175 7469 6f6e 2d31 293b 2d2d 636f  -caution-1);--co
+00030cd0: 6c6f 722d 323a 7661 7228 2d2d 6361 7574  lor-2:var(--caut
+00030ce0: 696f 6e2d 3229 3b2d 2d63 6f6c 6f72 2d33  ion-2);--color-3
+00030cf0: 3a76 6172 282d 2d63 6175 7469 6f6e 2d33  :var(--caution-3
+00030d00: 293b 2d2d 636f 6c6f 722d 343a 7661 7228  );--color-4:var(
+00030d10: 2d2d 6361 7574 696f 6e2d 3429 7d2e 6164  --caution-4)}.ad
+00030d20: 6d6f 6e69 7469 6f6e 2e64 616e 6765 727b  monition.danger{
+00030d30: 2d2d 6963 6f6e 2d75 726c 3a76 6172 282d  --icon-url:var(-
+00030d40: 2d64 616e 6765 722d 6963 6f6e 293b 2d2d  -danger-icon);--
+00030d50: 636f 6c6f 722d 313a 7661 7228 2d2d 6461  color-1:var(--da
+00030d60: 6e67 6572 2d31 293b 2d2d 636f 6c6f 722d  nger-1);--color-
+00030d70: 323a 7661 7228 2d2d 6461 6e67 6572 2d32  2:var(--danger-2
+00030d80: 293b 2d2d 636f 6c6f 722d 333a 7661 7228  );--color-3:var(
+00030d90: 2d2d 6461 6e67 6572 2d33 293b 2d2d 636f  --danger-3);--co
+00030da0: 6c6f 722d 343a 7661 7228 2d2d 6461 6e67  lor-4:var(--dang
+00030db0: 6572 2d34 297d 2e61 646d 6f6e 6974 696f  er-4)}.admonitio
+00030dc0: 6e2e 6572 726f 727b 2d2d 6963 6f6e 2d75  n.error{--icon-u
+00030dd0: 726c 3a76 6172 282d 2d65 7272 6f72 2d69  rl:var(--error-i
+00030de0: 636f 6e29 3b2d 2d63 6f6c 6f72 2d31 3a76  con);--color-1:v
+00030df0: 6172 282d 2d65 7272 6f72 2d31 293b 2d2d  ar(--error-1);--
+00030e00: 636f 6c6f 722d 323a 7661 7228 2d2d 6572  color-2:var(--er
+00030e10: 726f 722d 3229 3b2d 2d63 6f6c 6f72 2d33  ror-2);--color-3
+00030e20: 3a76 6172 282d 2d65 7272 6f72 2d33 293b  :var(--error-3);
+00030e30: 2d2d 636f 6c6f 722d 343a 7661 7228 2d2d  --color-4:var(--
+00030e40: 6572 726f 722d 3429 7d2e 6164 6d6f 6e69  error-4)}.admoni
+00030e50: 7469 6f6e 2e68 696e 747b 2d2d 6963 6f6e  tion.hint{--icon
+00030e60: 2d75 726c 3a76 6172 282d 2d68 696e 742d  -url:var(--hint-
+00030e70: 6963 6f6e 293b 2d2d 636f 6c6f 722d 313a  icon);--color-1:
+00030e80: 7661 7228 2d2d 6869 6e74 2d31 293b 2d2d  var(--hint-1);--
+00030e90: 636f 6c6f 722d 323a 7661 7228 2d2d 6869  color-2:var(--hi
+00030ea0: 6e74 2d32 293b 2d2d 636f 6c6f 722d 333a  nt-2);--color-3:
+00030eb0: 7661 7228 2d2d 6869 6e74 2d33 293b 2d2d  var(--hint-3);--
+00030ec0: 636f 6c6f 722d 343a 7661 7228 2d2d 6869  color-4:var(--hi
+00030ed0: 6e74 2d34 297d 2e61 646d 6f6e 6974 696f  nt-4)}.admonitio
+00030ee0: 6e2e 696d 706f 7274 616e 747b 2d2d 6963  n.important{--ic
+00030ef0: 6f6e 2d75 726c 3a76 6172 282d 2d69 6d70  on-url:var(--imp
+00030f00: 6f72 7461 6e74 2d69 636f 6e29 3b2d 2d63  ortant-icon);--c
+00030f10: 6f6c 6f72 2d31 3a76 6172 282d 2d69 6d70  olor-1:var(--imp
+00030f20: 6f72 7461 6e74 2d31 293b 2d2d 636f 6c6f  ortant-1);--colo
+00030f30: 722d 323a 7661 7228 2d2d 696d 706f 7274  r-2:var(--import
+00030f40: 616e 742d 3229 3b2d 2d63 6f6c 6f72 2d33  ant-2);--color-3
+00030f50: 3a76 6172 282d 2d69 6d70 6f72 7461 6e74  :var(--important
+00030f60: 2d33 293b 2d2d 636f 6c6f 722d 343a 7661  -3);--color-4:va
+00030f70: 7228 2d2d 696d 706f 7274 616e 742d 3429  r(--important-4)
+00030f80: 7d2e 6164 6d6f 6e69 7469 6f6e 2e6e 6f74  }.admonition.not
+00030f90: 657b 2d2d 6963 6f6e 2d75 726c 3a76 6172  e{--icon-url:var
+00030fa0: 282d 2d6e 6f74 652d 6963 6f6e 293b 2d2d  (--note-icon);--
+00030fb0: 636f 6c6f 722d 313a 7661 7228 2d2d 6e6f  color-1:var(--no
+00030fc0: 7465 2d31 293b 2d2d 636f 6c6f 722d 323a  te-1);--color-2:
+00030fd0: 7661 7228 2d2d 6e6f 7465 2d32 293b 2d2d  var(--note-2);--
+00030fe0: 636f 6c6f 722d 333a 7661 7228 2d2d 6e6f  color-3:var(--no
+00030ff0: 7465 2d33 293b 2d2d 636f 6c6f 722d 343a  te-3);--color-4:
+00031000: 7661 7228 2d2d 6e6f 7465 2d34 297d 2e61  var(--note-4)}.a
+00031010: 646d 6f6e 6974 696f 6e2e 7469 707b 2d2d  dmonition.tip{--
+00031020: 6963 6f6e 2d75 726c 3a76 6172 282d 2d74  icon-url:var(--t
+00031030: 6970 2d69 636f 6e29 3b2d 2d63 6f6c 6f72  ip-icon);--color
+00031040: 2d31 3a76 6172 282d 2d74 6970 2d31 293b  -1:var(--tip-1);
+00031050: 2d2d 636f 6c6f 722d 323a 7661 7228 2d2d  --color-2:var(--
+00031060: 7469 702d 3229 3b2d 2d63 6f6c 6f72 2d33  tip-2);--color-3
+00031070: 3a76 6172 282d 2d74 6970 2d33 293b 2d2d  :var(--tip-3);--
+00031080: 636f 6c6f 722d 343a 7661 7228 2d2d 7469  color-4:var(--ti
+00031090: 702d 3429 7d2e 6164 6d6f 6e69 7469 6f6e  p-4)}.admonition
+000310a0: 2e77 6172 6e69 6e67 7b2d 2d69 636f 6e2d  .warning{--icon-
+000310b0: 7572 6c3a 7661 7228 2d2d 7761 726e 696e  url:var(--warnin
+000310c0: 672d 6963 6f6e 293b 2d2d 636f 6c6f 722d  g-icon);--color-
+000310d0: 313a 7661 7228 2d2d 7761 726e 696e 672d  1:var(--warning-
+000310e0: 3129 3b2d 2d63 6f6c 6f72 2d32 3a76 6172  1);--color-2:var
+000310f0: 282d 2d77 6172 6e69 6e67 2d32 293b 2d2d  (--warning-2);--
+00031100: 636f 6c6f 722d 333a 7661 7228 2d2d 7761  color-3:var(--wa
+00031110: 726e 696e 672d 3329 3b2d 2d63 6f6c 6f72  rning-3);--color
+00031120: 2d34 3a76 6172 282d 2d77 6172 6e69 6e67  -4:var(--warning
+00031130: 2d34 297d 2e61 646d 6f6e 6974 696f 6e2e  -4)}.admonition.
+00031140: 7365 6561 6c73 6f7b 2d2d 6963 6f6e 2d75  seealso{--icon-u
+00031150: 726c 3a76 6172 282d 2d73 6565 616c 736f  rl:var(--seealso
+00031160: 2d69 636f 6e29 3b2d 2d63 6f6c 6f72 2d31  -icon);--color-1
+00031170: 3a76 6172 282d 2d73 6565 616c 736f 2d31  :var(--seealso-1
+00031180: 293b 2d2d 636f 6c6f 722d 323a 7661 7228  );--color-2:var(
+00031190: 2d2d 7365 6561 6c73 6f2d 3229 3b2d 2d63  --seealso-2);--c
+000311a0: 6f6c 6f72 2d33 3a76 6172 282d 2d73 6565  olor-3:var(--see
+000311b0: 616c 736f 2d33 293b 2d2d 636f 6c6f 722d  also-3);--color-
+000311c0: 343a 7661 7228 2d2d 7365 6561 6c73 6f2d  4:var(--seealso-
+000311d0: 3429 7d2e 6164 6d6f 6e69 7469 6f6e 2e61  4)}.admonition.a
+000311e0: 646d 6f6e 6974 696f 6e2d 746f 646f 7b2d  dmonition-todo{-
+000311f0: 2d69 636f 6e2d 7572 6c3a 7661 7228 2d2d  -icon-url:var(--
+00031200: 746f 646f 2d69 636f 6e29 3b2d 2d63 6f6c  todo-icon);--col
+00031210: 6f72 2d31 3a76 6172 282d 2d74 6f64 6f2d  or-1:var(--todo-
+00031220: 3129 3b2d 2d63 6f6c 6f72 2d32 3a76 6172  1);--color-2:var
+00031230: 282d 2d74 6f64 6f2d 3229 3b2d 2d63 6f6c  (--todo-2);--col
+00031240: 6f72 2d33 3a76 6172 282d 2d74 6f64 6f2d  or-3:var(--todo-
+00031250: 3329 3b2d 2d63 6f6c 6f72 2d34 3a76 6172  3);--color-4:var
+00031260: 282d 2d74 6f64 6f2d 3429 7d2e 6164 6d6f  (--todo-4)}.admo
+00031270: 6e69 7469 6f6e 2070 2e61 646d 6f6e 6974  nition p.admonit
+00031280: 696f 6e2d 7469 746c 652b 707b 6d61 7267  ion-title+p{marg
+00031290: 696e 2d74 6f70 3a30 7d2e 6164 6d6f 6e69  in-top:0}.admoni
+000312a0: 7469 6f6e 3e3a 6c61 7374 2d63 6869 6c64  tion>:last-child
+000312b0: 7b6d 6172 6769 6e2d 626f 7474 6f6d 3a30  {margin-bottom:0
+000312c0: 7d73 7061 6e2e 7665 7273 696f 6e6d 6f64  }span.versionmod
+000312d0: 6966 6965 647b 636f 6c6f 723a 7661 7228  ified{color:var(
+000312e0: 2d2d 7379 2d63 2d62 6f6c 6429 3b66 6f6e  --sy-c-bold);fon
+000312f0: 742d 7765 6967 6874 3a36 3030 7d64 6976  t-weight:600}div
+00031300: 2e64 6570 7265 6361 7465 642c 6469 762e  .deprecated,div.
+00031310: 7665 7273 696f 6e61 6464 6564 2c64 6976  versionadded,div
+00031320: 2e76 6572 7369 6f6e 6368 616e 6765 647b  .versionchanged{
+00031330: 706f 7369 7469 6f6e 3a72 656c 6174 6976  position:relativ
+00031340: 653b 7061 6464 696e 673a 3670 7820 3172  e;padding:6px 1r
+00031350: 656d 3b6d 6172 6769 6e3a 3172 656d 2030  em;margin:1rem 0
+00031360: 3b62 6f72 6465 722d 6c65 6674 3a34 7078  ;border-left:4px
+00031370: 2073 6f6c 6964 2076 6172 282d 2d63 6f6c   solid var(--col
+00031380: 6f72 2d32 293b 6261 636b 6772 6f75 6e64  or-2);background
+00031390: 2d63 6f6c 6f72 3a76 6172 282d 2d63 6f6c  -color:var(--col
+000313a0: 6f72 2d31 293b 6c69 6e65 2d68 6569 6768  or-1);line-heigh
+000313b0: 743a 312e 3732 7d64 6976 2e64 6570 7265  t:1.72}div.depre
+000313c0: 6361 7465 643a 6265 666f 7265 2c64 6976  cated:before,div
+000313d0: 2e76 6572 7369 6f6e 6164 6465 643a 6265  .versionadded:be
+000313e0: 666f 7265 2c64 6976 2e76 6572 7369 6f6e  fore,div.version
+000313f0: 6368 616e 6765 643a 6265 666f 7265 7b70  changed:before{p
+00031400: 6f73 6974 696f 6e3a 6162 736f 6c75 7465  osition:absolute
+00031410: 3b63 6f6e 7465 6e74 3a76 6172 282d 2d76  ;content:var(--v
+00031420: 6572 7369 6f6e 2d69 636f 6e29 3b74 6f70  ersion-icon);top
+00031430: 3a31 3070 783b 6c65 6674 3a2d 3132 7078  :10px;left:-12px
+00031440: 3b63 6f6c 6f72 3a23 6666 663b 7769 6474  ;color:#fff;widt
+00031450: 683a 3230 7078 3b68 6569 6768 743a 3230  h:20px;height:20
+00031460: 7078 3b62 6f72 6465 722d 7261 6469 7573  px;border-radius
+00031470: 3a31 3030 253b 6261 636b 6772 6f75 6e64  :100%;background
+00031480: 2d63 6f6c 6f72 3a76 6172 282d 2d63 6f6c  -color:var(--col
+00031490: 6f72 2d32 293b 7465 7874 2d61 6c69 676e  or-2);text-align
+000314a0: 3a63 656e 7465 723b 666f 6e74 3a6e 6f72  :center;font:nor
+000314b0: 6d61 6c20 3730 3020 3134 7078 2f32 3070  mal 700 14px/20p
+000314c0: 7820 7661 7228 2d2d 7379 2d66 2d6d 6f6e  x var(--sy-f-mon
+000314d0: 6f29 7d64 6976 2e76 6572 7369 6f6e 6164  o)}div.versionad
+000314e0: 6465 647b 2d2d 636f 6c6f 722d 313a 7661  ded{--color-1:va
+000314f0: 7228 2d2d 7665 7273 696f 6e61 6464 6564  r(--versionadded
+00031500: 2d31 293b 2d2d 636f 6c6f 722d 323a 7661  -1);--color-2:va
+00031510: 7228 2d2d 7665 7273 696f 6e61 6464 6564  r(--versionadded
+00031520: 2d32 293b 2d2d 7665 7273 696f 6e2d 6963  -2);--version-ic
+00031530: 6f6e 3a22 2322 7d64 6976 2e76 6572 7369  on:"#"}div.versi
+00031540: 6f6e 6368 616e 6765 647b 2d2d 636f 6c6f  onchanged{--colo
+00031550: 722d 313a 7661 7228 2d2d 7665 7273 696f  r-1:var(--versio
+00031560: 6e63 6861 6e67 6564 2d31 293b 2d2d 636f  nchanged-1);--co
+00031570: 6c6f 722d 323a 7661 7228 2d2d 7665 7273  lor-2:var(--vers
+00031580: 696f 6e63 6861 6e67 6564 2d32 293b 2d2d  ionchanged-2);--
+00031590: 7665 7273 696f 6e2d 6963 6f6e 3a22 2522  version-icon:"%"
+000315a0: 7d64 6976 2e64 6570 7265 6361 7465 647b  }div.deprecated{
+000315b0: 2d2d 636f 6c6f 722d 313a 7661 7228 2d2d  --color-1:var(--
+000315c0: 6465 7072 6563 6174 6564 2d31 293b 2d2d  deprecated-1);--
+000315d0: 636f 6c6f 722d 323a 7661 7228 2d2d 6465  color-2:var(--de
+000315e0: 7072 6563 6174 6564 2d32 293b 2d2d 7665  precated-2);--ve
+000315f0: 7273 696f 6e2d 6963 6f6e 3a22 2122 7d64  rsion-icon:"!"}d
+00031600: 6976 2e64 6570 7265 6361 7465 643e 702c  iv.deprecated>p,
+00031610: 6469 762e 7665 7273 696f 6e61 6464 6564  div.versionadded
+00031620: 3e70 2c64 6976 2e76 6572 7369 6f6e 6368  >p,div.versionch
+00031630: 616e 6765 643e 707b 6d61 7267 696e 3a30  anged>p{margin:0
+00031640: 7d2e 7975 6520 626c 6f63 6b71 756f 7465  }.yue blockquote
+00031650: 2e65 7069 6772 6170 687b 7061 6464 696e  .epigraph{paddin
+00031660: 673a 3172 656d 2032 2e34 7265 6d3b 626f  g:1rem 2.4rem;bo
+00031670: 7264 6572 2d6c 6566 743a 303b 7465 7874  rder-left:0;text
+00031680: 2d61 6c69 676e 3a63 656e 7465 727d 2e79  -align:center}.y
+00031690: 7565 2062 6c6f 636b 7175 6f74 652e 6869  ue blockquote.hi
+000316a0: 6768 6c69 6768 7473 7b62 6f72 6465 722d  ghlights{border-
+000316b0: 6c65 6674 2d77 6964 7468 3a34 7078 3b70  left-width:4px;p
+000316c0: 6164 6469 6e67 2d74 6f70 3a2e 3272 656d  adding-top:.2rem
+000316d0: 3b70 6164 6469 6e67 2d62 6f74 746f 6d3a  ;padding-bottom:
+000316e0: 2e32 7265 6d3b 6261 636b 6772 6f75 6e64  .2rem;background
+000316f0: 2d63 6f6c 6f72 3a76 6172 282d 2d73 792d  -color:var(--sy-
+00031700: 632d 7375 7266 6163 6529 7d2e 7975 6520  c-surface)}.yue 
+00031710: 626c 6f63 6b71 756f 7465 2e70 756c 6c2d  blockquote.pull-
+00031720: 7175 6f74 657b 706f 7369 7469 6f6e 3a72  quote{position:r
+00031730: 656c 6174 6976 653b 666f 6e74 2d73 697a  elative;font-siz
+00031740: 653a 312e 3234 7265 6d3b 7061 6464 696e  e:1.24rem;paddin
+00031750: 673a 322e 3472 656d 2033 2e36 7265 6d20  g:2.4rem 3.6rem 
+00031760: 312e 3272 656d 3b62 6f72 6465 722d 6c65  1.2rem;border-le
+00031770: 6674 3a30 7d2e 7975 6520 626c 6f63 6b71  ft:0}.yue blockq
+00031780: 756f 7465 2e70 756c 6c2d 7175 6f74 653a  uote.pull-quote:
+00031790: 6265 666f 7265 7b63 6f6e 7465 6e74 3a22  before{content:"
+000317a0: 5c32 3031 6322 3b70 6f73 6974 696f 6e3a  \201c";position:
+000317b0: 6162 736f 6c75 7465 3b74 6f70 3a30 3b6c  absolute;top:0;l
+000317c0: 6566 743a 2e35 7265 6d3b 636f 6c6f 723a  eft:.5rem;color:
+000317d0: 7661 7228 2d2d 7975 652d 632d 7175 6f74  var(--yue-c-quot
+000317e0: 652d 7379 6d62 6f6c 293b 666f 6e74 3a37  e-symbol);font:7
+000317f0: 3030 2034 7265 6d2f 3120 5469 6d65 7320  00 4rem/1 Times 
+00031800: 4e65 7720 526f 6d61 6e2c 4765 6f72 6769  New Roman,Georgi
+00031810: 612c 5061 6c61 7469 6e6f 2c54 696d 6573  a,Palatino,Times
+00031820: 2c73 6572 6966 7d2e 7975 6520 626c 6f63  ,serif}.yue bloc
+00031830: 6b71 756f 7465 2e70 756c 6c2d 7175 6f74  kquote.pull-quot
+00031840: 6520 2e61 7474 7269 6275 7469 6f6e 7b74  e .attribution{t
+00031850: 6578 742d 616c 6967 6e3a 7269 6768 747d  ext-align:right}
+00031860: 7072 652e 6c69 7465 7261 6c2d 626c 6f63  pre.literal-bloc
+00031870: 6b7b 6c69 6e65 2d68 6569 6768 743a 312e  k{line-height:1.
+00031880: 3438 3b70 6164 6469 6e67 3a31 7265 6d3b  48;padding:1rem;
+00031890: 666f 6e74 2d73 697a 653a 2e39 3672 656d  font-size:.96rem
+000318a0: 3b62 6163 6b67 726f 756e 642d 636f 6c6f  ;background-colo
+000318b0: 723a 7661 7228 2d2d 7379 6e74 6178 2d70  r:var(--syntax-p
+000318c0: 7265 2d62 6729 3b62 6f72 6465 722d 7261  re-bg);border-ra
+000318d0: 6469 7573 3a36 7078 3b6f 7665 7266 6c6f  dius:6px;overflo
+000318e0: 773a 6175 746f 7d2e 6869 6768 6c69 6768  w:auto}.highligh
+000318f0: 742c 2e6c 6974 6572 616c 2d62 6c6f 636b  t,.literal-block
+00031900: 2d77 7261 7070 6572 7b2d 2d6d 6172 6769  -wrapper{--margi
+00031910: 6e3a 3172 656d 3b2d 2d72 6164 6975 733a  n:1rem;--radius:
+00031920: 3670 787d 2e6c 6974 6572 616c 2d62 6c6f  6px}.literal-blo
+00031930: 636b 2d77 7261 7070 6572 2064 6976 5b63  ck-wrapper div[c
+00031940: 6c61 7373 5e3d 6869 6768 6c69 6768 742d  lass^=highlight-
+00031950: 5d7b 6469 7370 6c61 793a 666c 6578 7d2e  ]{display:flex}.
+00031960: 6c69 7465 7261 6c2d 626c 6f63 6b2d 7772  literal-block-wr
+00031970: 6170 7065 7220 2e68 6967 686c 6967 6874  apper .highlight
+00031980: 7b77 6964 7468 3a31 3030 257d 2e68 6967  {width:100%}.hig
+00031990: 686c 6967 6874 3e70 7265 7b6c 696e 652d  hlight>pre{line-
+000319a0: 6865 6967 6874 3a31 2e34 383b 7061 6464  height:1.48;padd
+000319b0: 696e 673a 7661 7228 2d2d 6d61 7267 696e  ing:var(--margin
+000319c0: 293b 666f 6e74 2d73 697a 653a 2e39 3672  );font-size:.96r
+000319d0: 656d 3b66 6f6e 742d 6661 6d69 6c79 3a76  em;font-family:v
+000319e0: 6172 282d 2d73 792d 662d 6d6f 6e6f 293b  ar(--sy-f-mono);
+000319f0: 6261 636b 6772 6f75 6e64 2d63 6f6c 6f72  background-color
+00031a00: 3a76 6172 282d 2d73 796e 7461 782d 7072  :var(--syntax-pr
+00031a10: 652d 6267 293b 626f 7264 6572 2d72 6164  e-bg);border-rad
+00031a20: 6975 733a 7661 7228 2d2d 7261 6469 7573  ius:var(--radius
+00031a30: 293b 6f76 6572 666c 6f77 3a61 7574 6f7d  );overflow:auto}
+00031a40: 2e77 696e 202e 6869 6768 6c69 6768 743e  .win .highlight>
+00031a50: 7072 657b 666f 6e74 2d66 616d 696c 793a  pre{font-family:
+00031a60: 2254 7765 6d6f 6a69 2043 6f75 6e74 7279  "Twemoji Country
+00031a70: 2046 6c61 6773 222c 7661 7228 2d2d 7379   Flags",var(--sy
+00031a80: 2d66 2d6d 6f6e 6f29 7d2e 6869 6768 6c69  -f-mono)}.highli
+00031a90: 6768 7420 2e6c 696e 656e 6f73 7b64 6973  ght .linenos{dis
+00031aa0: 706c 6179 3a69 6e6c 696e 652d 626c 6f63  play:inline-bloc
+00031ab0: 6b3b 626f 782d 7368 6164 6f77 3a2d 2e30  k;box-shadow:-.0
+00031ac0: 3572 656d 2030 2076 6172 282d 2d73 796e  5rem 0 var(--syn
+00031ad0: 7461 782d 6c69 6e65 6e6f 732d 6469 7669  tax-linenos-divi
+00031ae0: 6465 7229 2069 6e73 6574 3b2d 7765 626b  der) inset;-webk
+00031af0: 6974 2d75 7365 722d 7365 6c65 6374 3a6e  it-user-select:n
+00031b00: 6f6e 653b 2d6d 6f7a 2d75 7365 722d 7365  one;-moz-user-se
+00031b10: 6c65 6374 3a6e 6f6e 653b 7573 6572 2d73  lect:none;user-s
+00031b20: 656c 6563 743a 6e6f 6e65 3b6d 6172 6769  elect:none;margi
+00031b30: 6e2d 7269 6768 743a 2e38 7265 6d3b 7061  n-right:.8rem;pa
+00031b40: 6464 696e 672d 7269 6768 743a 2e38 7265  dding-right:.8re
+00031b50: 6d3b 6f70 6163 6974 793a 2e36 7d2e 6869  m;opacity:.6}.hi
+00031b60: 6768 6c69 6768 7420 2e68 6c6c 7b6d 6172  ghlight .hll{mar
+00031b70: 6769 6e2d 6c65 6674 3a63 616c 6328 3072  gin-left:calc(0r
+00031b80: 656d 202d 2076 6172 282d 2d6d 6172 6769  em - var(--margi
+00031b90: 6e29 293b 6d61 7267 696e 2d72 6967 6874  n));margin-right
+00031ba0: 3a63 616c 6328 3072 656d 202d 2076 6172  :calc(0rem - var
+00031bb0: 282d 2d6d 6172 6769 6e29 293b 7061 6464  (--margin));padd
+00031bc0: 696e 673a 3020 7661 7228 2d2d 6d61 7267  ing:0 var(--marg
+00031bd0: 696e 297d 2e63 6f64 652d 626c 6f63 6b2d  in)}.code-block-
+00031be0: 6361 7074 696f 6e7b 6469 7370 6c61 793a  caption{display:
+00031bf0: 666c 6578 3b66 6f6e 742d 7369 7a65 3a2e  flex;font-size:.
+00031c00: 3834 7265 6d3b 666f 6e74 2d77 6569 6768  84rem;font-weigh
+00031c10: 743a 3630 303b 636f 6c6f 723a 7661 7228  t:600;color:var(
+00031c20: 2d2d 7379 6e74 6178 2d74 6578 7429 3b62  --syntax-text);b
+00031c30: 6163 6b67 726f 756e 642d 636f 6c6f 723a  ackground-color:
+00031c40: 7661 7228 2d2d 7379 6e74 6178 2d63 6170  var(--syntax-cap
+00031c50: 2d62 6729 3b70 6164 6469 6e67 3a2e 3472  -bg);padding:.4r
+00031c60: 656d 2076 6172 282d 2d6d 6172 6769 6e29  em var(--margin)
+00031c70: 3b62 6f72 6465 722d 7261 6469 7573 3a76  ;border-radius:v
+00031c80: 6172 282d 2d72 6164 6975 7329 2076 6172  ar(--radius) var
+00031c90: 282d 2d72 6164 6975 7329 2030 2030 7d2e  (--radius) 0 0}.
+00031ca0: 636f 6465 2d62 6c6f 636b 2d63 6170 7469  code-block-capti
+00031cb0: 6f6e 2b64 6976 3e2e 6869 6768 6c69 6768  on+div>.highligh
+00031cc0: 743e 7072 657b 626f 7264 6572 2d74 6f70  t>pre{border-top
+00031cd0: 2d6c 6566 742d 7261 6469 7573 3a30 3b62  -left-radius:0;b
+00031ce0: 6f72 6465 722d 746f 702d 7269 6768 742d  order-top-right-
+00031cf0: 7261 6469 7573 3a30 7d64 6976 5b63 6c61  radius:0}div[cla
+00031d00: 7373 5e3d 6869 6768 6c69 6768 745d 3e2e  ss^=highlight]>.
+00031d10: 6869 6768 6c69 6768 743e 7072 657b 6469  highlight>pre{di
+00031d20: 7370 6c61 793a 6772 6964 7d2e 7975 6520  splay:grid}.yue 
+00031d30: 2e74 6162 6c65 2d77 7261 7070 6572 7b77  .table-wrapper{w
+00031d40: 6964 7468 3a31 3030 253b 6f76 6572 666c  idth:100%;overfl
+00031d50: 6f77 2d78 3a61 7574 6f3b 6d61 7267 696e  ow-x:auto;margin
+00031d60: 2d74 6f70 3a32 7265 6d3b 6d61 7267 696e  -top:2rem;margin
+00031d70: 2d62 6f74 746f 6d3a 3272 656d 3b62 6f72  -bottom:2rem;bor
+00031d80: 6465 723a 3170 7820 736f 6c69 6420 7661  der:1px solid va
+00031d90: 7228 2d2d 7975 652d 632d 7461 626c 652d  r(--yue-c-table-
+00031da0: 626f 7264 6572 293b 626f 7264 6572 2d72  border);border-r
+00031db0: 6164 6975 733a 3670 787d 2e79 7565 202e  adius:6px}.yue .
+00031dc0: 7461 626c 652d 7772 6170 7065 723e 7461  table-wrapper>ta
+00031dd0: 626c 657b 6d61 7267 696e 3a30 7d2e 7975  ble{margin:0}.yu
+00031de0: 6520 2e74 6162 6c65 2d77 7261 7070 6572  e .table-wrapper
+00031df0: 2074 6865 6164 2074 727b 626f 7264 6572   thead tr{border
+00031e00: 2d74 6f70 3a31 7078 2073 6f6c 6964 2076  -top:1px solid v
+00031e10: 6172 282d 2d79 7565 2d63 2d74 642d 626f  ar(--yue-c-td-bo
+00031e20: 7264 6572 297d 2e79 7565 202e 7461 626c  rder)}.yue .tabl
+00031e30: 652d 7772 6170 7065 7220 7468 6561 6420  e-wrapper thead 
+00031e40: 7472 3a66 6972 7374 2d63 6869 6c64 7b62  tr:first-child{b
+00031e50: 6f72 6465 722d 746f 703a 307d 2e79 7565  order-top:0}.yue
+00031e60: 202e 7461 626c 652d 7772 6170 7065 7220   .table-wrapper 
+00031e70: 7468 7b62 6163 6b67 726f 756e 642d 636f  th{background-co
+00031e80: 6c6f 723a 7661 7228 2d2d 7975 652d 632d  lor:var(--yue-c-
+00031e90: 7468 2d62 6163 6b67 726f 756e 6429 3b62  th-background);b
+00031ea0: 6f72 6465 722d 6c65 6674 3a31 7078 2073  order-left:1px s
+00031eb0: 6f6c 6964 2076 6172 282d 2d79 7565 2d63  olid var(--yue-c
+00031ec0: 2d74 642d 626f 7264 6572 293b 7061 6464  -td-border);padd
+00031ed0: 696e 673a 2e37 3235 7265 6d20 3172 656d  ing:.725rem 1rem
+00031ee0: 7d2e 7975 6520 2e74 6162 6c65 2d77 7261  }.yue .table-wra
+00031ef0: 7070 6572 2074 647b 626f 7264 6572 2d6c  pper td{border-l
+00031f00: 6566 743a 3170 7820 736f 6c69 6420 7661  eft:1px solid va
+00031f10: 7228 2d2d 7975 652d 632d 7464 2d62 6f72  r(--yue-c-td-bor
+00031f20: 6465 7229 3b70 6164 6469 6e67 3a2e 3572  der);padding:.5r
+00031f30: 656d 2031 7265 6d7d 2e79 7565 202e 7461  em 1rem}.yue .ta
+00031f40: 626c 652d 7772 6170 7065 7220 7472 3e74  ble-wrapper tr>t
+00031f50: 643a 6669 7273 742d 6368 696c 642c 2e79  d:first-child,.y
+00031f60: 7565 202e 7461 626c 652d 7772 6170 7065  ue .table-wrappe
+00031f70: 7220 7472 3e74 683a 6669 7273 742d 6368  r tr>th:first-ch
+00031f80: 696c 647b 626f 7264 6572 2d6c 6566 743a  ild{border-left:
+00031f90: 307d 2e79 7565 202e 7461 626c 652d 7772  0}.yue .table-wr
+00031fa0: 6170 7065 7220 6361 7074 696f 6e7b 7061  apper caption{pa
+00031fb0: 6464 696e 673a 2e35 7265 6d3b 6d61 7267  dding:.5rem;marg
+00031fc0: 696e 3a30 3b62 6f72 6465 722d 626f 7474  in:0;border-bott
+00031fd0: 6f6d 3a31 7078 2073 6f6c 6964 2076 6172  om:1px solid var
+00031fe0: 282d 2d79 7565 2d63 2d74 682d 626f 7264  (--yue-c-th-bord
+00031ff0: 6572 297d 2e79 7565 202e 7461 626c 652d  er)}.yue .table-
+00032000: 7772 6170 7065 7220 7462 6f64 7920 7472  wrapper tbody tr
+00032010: 2e72 6f77 2d6f 6464 7b62 6163 6b67 726f  .row-odd{backgro
+00032020: 756e 642d 636f 6c6f 723a 7661 7228 2d2d  und-color:var(--
+00032030: 7975 652d 632d 726f 772d 6261 636b 6772  yue-c-row-backgr
+00032040: 6f75 6e64 297d 2e79 7565 2074 6162 6c65  ound)}.yue table
+00032050: 2e68 6c69 7374 2074 647b 7665 7274 6963  .hlist td{vertic
+00032060: 616c 2d61 6c69 676e 3a74 6f70 7d2e 7461  al-align:top}.ta
+00032070: 626c 652d 7772 6170 7065 727b 6f76 6572  ble-wrapper{over
+00032080: 666c 6f77 2d78 3a61 7574 6f3b 7363 726f  flow-x:auto;scro
+00032090: 6c6c 6261 722d 6775 7474 6572 3a61 7574  llbar-gutter:aut
+000320a0: 6f7d 2e74 6162 6c65 2d77 7261 7070 6572  o}.table-wrapper
+000320b0: 3a3a 2d77 6562 6b69 742d 7363 726f 6c6c  ::-webkit-scroll
+000320c0: 6261 727b 6865 6967 6874 3a2e 3735 7265  bar{height:.75re
+000320d0: 6d3b 7769 6474 683a 2e37 3572 656d 7d2e  m;width:.75rem}.
+000320e0: 7461 626c 652d 7772 6170 7065 723a 3a2d  table-wrapper::-
+000320f0: 7765 626b 6974 2d73 6372 6f6c 6c62 6172  webkit-scrollbar
+00032100: 2d74 6875 6d62 7b62 6f72 6465 722d 7261  -thumb{border-ra
+00032110: 6469 7573 3a31 3070 787d 2e74 6162 6c65  dius:10px}.table
+00032120: 2d77 7261 7070 6572 3a3a 2d77 6562 6b69  -wrapper::-webki
+00032130: 742d 7363 726f 6c6c 6261 722d 7472 6163  t-scrollbar-trac
+00032140: 6b7b 6261 636b 6772 6f75 6e64 2d63 6f6c  k{background-col
+00032150: 6f72 3a69 6e69 7469 616c 7d2e 7461 626c  or:initial}.tabl
+00032160: 652d 7772 6170 7065 723a 686f 7665 723a  e-wrapper:hover:
+00032170: 3a2d 7765 626b 6974 2d73 6372 6f6c 6c62  :-webkit-scrollb
+00032180: 6172 2d74 6875 6d62 7b62 6163 6b67 726f  ar-thumb{backgro
+00032190: 756e 642d 636f 6c6f 723a 2339 6239 6239  und-color:#9b9b9
+000321a0: 6233 333b 6261 636b 6772 6f75 6e64 2d63  b33;background-c
+000321b0: 6c69 703a 636f 6e74 656e 742d 626f 783b  lip:content-box;
+000321c0: 626f 7264 6572 3a33 7078 2073 6f6c 6964  border:3px solid
+000321d0: 2023 3030 3030 7d2e 7975 6520 7461 626c   #0000}.yue tabl
+000321e0: 652e 6768 6f73 7420 7464 2c2e 7975 6520  e.ghost td,.yue 
+000321f0: 7461 626c 652e 6768 6f73 7420 7468 7b62  table.ghost th{b
+00032200: 6f72 6465 722d 6c65 6674 3a30 3b62 6f72  order-left:0;bor
+00032210: 6465 722d 7269 6768 743a 303b 6261 636b  der-right:0;back
+00032220: 6772 6f75 6e64 2d63 6f6c 6f72 3a69 6e69  ground-color:ini
+00032230: 7469 616c 7d2e 7975 6520 7461 626c 652e  tial}.yue table.
+00032240: 6768 6f73 7420 6361 7074 696f 6e7b 6d61  ghost caption{ma
+00032250: 7267 696e 2d62 6f74 746f 6d3a 303b 7061  rgin-bottom:0;pa
+00032260: 6464 696e 672d 626f 7474 6f6d 3a2e 3572  dding-bottom:.5r
+00032270: 656d 3b62 6f72 6465 722d 626f 7474 6f6d  em;border-bottom
+00032280: 3a33 7078 2073 6f6c 6964 2076 6172 282d  :3px solid var(-
+00032290: 2d79 7565 2d63 2d74 642d 626f 7264 6572  -yue-c-td-border
+000322a0: 297d 2e79 7565 2074 6162 6c65 2e67 686f  )}.yue table.gho
+000322b0: 7374 2074 6865 6164 2074 723a 6669 7273  st thead tr:firs
+000322c0: 742d 6368 696c 647b 626f 7264 6572 2d74  t-child{border-t
+000322d0: 6f70 3a30 3b62 6f72 6465 722d 626f 7474  op:0;border-bott
+000322e0: 6f6d 2d77 6964 7468 3a33 7078 7d2e 7975  om-width:3px}.yu
+000322f0: 6520 2e74 6162 6c65 2d77 7261 7070 6572  e .table-wrapper
+00032300: 2e67 686f 7374 7b62 6f72 6465 723a 307d  .ghost{border:0}
+00032310: 3a72 6f6f 747b 2d2d 7369 672d 7072 6f70  :root{--sig-prop
+00032320: 6572 7479 3a76 6172 282d 2d73 796e 7461  erty:var(--synta
+00032330: 782d 6b65 7977 6f72 6429 3b2d 2d73 6967  x-keyword);--sig
+00032340: 2d6e 616d 653a 7661 7228 2d2d 7379 6e74  -name:var(--synt
+00032350: 6178 2d70 726f 7065 7274 7929 3b2d 2d73  ax-property);--s
+00032360: 6967 2d74 7970 6568 696e 743a 7661 7228  ig-typehint:var(
+00032370: 2d2d 7379 6e74 6178 2d63 6f6e 7374 616e  --syntax-constan
+00032380: 7429 3b2d 2d73 6967 2d70 6172 616d 3a76  t);--sig-param:v
+00032390: 6172 282d 2d73 796e 7461 782d 6d65 7461  ar(--syntax-meta
+000323a0: 297d 6474 2e73 6967 7b70 6f73 6974 696f  )}dt.sig{positio
+000323b0: 6e3a 7265 6c61 7469 7665 3b66 6f6e 742d  n:relative;font-
+000323c0: 7369 7a65 3a2e 3932 7265 6d3b 7061 6464  size:.92rem;padd
+000323d0: 696e 673a 2e32 3572 656d 202e 3572 656d  ing:.25rem .5rem
+000323e0: 202e 3235 7265 6d20 3372 656d 3b74 6578   .25rem 3rem;tex
+000323f0: 742d 696e 6465 6e74 3a2d 322e 3472 656d  t-indent:-2.4rem
+00032400: 3b62 6f72 6465 722d 7261 6469 7573 3a36  ;border-radius:6
+00032410: 7078 7d64 742e 7369 673a 6166 7465 727b  px}dt.sig:after{
+00032420: 636f 6e74 656e 743a 2222 3b64 6973 706c  content:"";displ
+00032430: 6179 3a74 6162 6c65 3b63 6c65 6172 3a62  ay:table;clear:b
+00032440: 6f74 687d 6474 2e73 6967 3a68 6f76 6572  oth}dt.sig:hover
+00032450: 7b62 6163 6b67 726f 756e 643a 7661 7228  {background:var(
+00032460: 2d2d 7379 2d63 2d73 7572 6661 6365 297d  --sy-c-surface)}
+00032470: 6474 2e73 6967 2b64 647b 666f 6e74 2d73  dt.sig+dd{font-s
+00032480: 697a 653a 2e39 3272 656d 3b6d 6172 6769  ize:.92rem;margi
+00032490: 6e2d 6c65 6674 3a32 7265 6d7d 6474 2e73  n-left:2rem}dt.s
+000324a0: 6967 3e65 6d2e 7072 6f70 6572 7479 3a66  ig>em.property:f
+000324b0: 6972 7374 2d63 6869 6c64 7b63 6f6c 6f72  irst-child{color
+000324c0: 3a76 6172 282d 2d73 6967 2d70 726f 7065  :var(--sig-prope
+000324d0: 7274 7929 7d64 6c2e 6669 656c 642d 6c69  rty)}dl.field-li
+000324e0: 7374 2061 7b66 6f6e 742d 7765 6967 6874  st a{font-weight
+000324f0: 3a34 3030 7d64 742e 7369 672b 6464 3e64  :400}dt.sig+dd>d
+00032500: 6976 7b6d 6172 6769 6e2d 626f 7474 6f6d  iv{margin-bottom
+00032510: 3a31 7265 6d7d 6474 2e73 6967 2b64 643e  :1rem}dt.sig+dd>
+00032520: 646c 2e66 6965 6c64 2d6c 6973 743e 6474  dl.field-list>dt
+00032530: 7b74 6578 742d 7472 616e 7366 6f72 6d3a  {text-transform:
+00032540: 7570 7065 7263 6173 653b 666f 6e74 2d73  uppercase;font-s
+00032550: 697a 653a 2e37 3672 656d 7d65 6d2e 7072  ize:.76rem}em.pr
+00032560: 6f70 6572 7479 2c65 6d2e 7369 672d 7061  operty,em.sig-pa
+00032570: 7261 6d7b 666f 6e74 2d73 7479 6c65 3a6e  ram{font-style:n
+00032580: 6f72 6d61 6c7d 656d 2e73 6967 2d70 6172  ormal}em.sig-par
+00032590: 616d 7b63 6f6c 6f72 3a76 6172 282d 2d73  am{color:var(--s
+000325a0: 792d 632d 6c69 6768 7429 7d73 7061 6e2e  y-c-light)}span.
+000325b0: 7369 672d 6e61 6d65 2c73 7061 6e2e 7369  sig-name,span.si
+000325c0: 672d 7072 656e 616d 657b 636f 6c6f 723a  g-prename{color:
+000325d0: 7661 7228 2d2d 7369 672d 6e61 6d65 297d  var(--sig-name)}
+000325e0: 7370 616e 2e73 6967 2d6e 616d 657b 666f  span.sig-name{fo
+000325f0: 6e74 2d77 6569 6768 743a 3630 307d 7370  nt-weight:600}sp
+00032600: 616e 2e73 6967 2d72 6574 7572 6e2d 6963  an.sig-return-ic
+00032610: 6f6e 7b63 6f6c 6f72 3a76 6172 282d 2d73  on{color:var(--s
+00032620: 792d 632d 6c69 6768 7429 7d73 7061 6e2e  y-c-light)}span.
+00032630: 7369 672d 7265 7475 726e 2d74 7970 6568  sig-return-typeh
+00032640: 696e 742c 7370 616e 2e73 6967 2d72 6574  int,span.sig-ret
+00032650: 7572 6e2d 7479 7065 6869 6e74 3e61 7b63  urn-typehint>a{c
+00032660: 6f6c 6f72 3a76 6172 282d 2d73 6967 2d74  olor:var(--sig-t
+00032670: 7970 6568 696e 7429 7d73 7061 6e2e 7072  ypehint)}span.pr
+00032680: 652c 7370 616e 2e73 6967 2d70 6172 656e  e,span.sig-paren
+00032690: 7b66 6f6e 742d 6661 6d69 6c79 3a76 6172  {font-family:var
+000326a0: 282d 2d73 792d 662d 6d6f 6e6f 297d 6474  (--sy-f-mono)}dt
+000326b0: 2e73 6967 3e61 2e69 6e74 6572 6e61 6c7b  .sig>a.internal{
+000326c0: 666f 6e74 2d73 697a 653a 2e38 3272 656d  font-size:.82rem
+000326d0: 3b62 6f72 6465 723a 303b 636f 6c6f 723a  ;border:0;color:
+000326e0: 7661 7228 2d2d 7379 2d63 2d6c 6967 6874  var(--sy-c-light
+000326f0: 297d 6474 2e73 6967 3e61 2e69 6e74 6572  )}dt.sig>a.inter
+00032700: 6e61 6c3a 6265 666f 7265 7b63 6f6e 7465  nal:before{conte
+00032710: 6e74 3a22 5c61 223b 7768 6974 652d 7370  nt:"\a";white-sp
+00032720: 6163 653a 7072 657d 2e76 6965 7763 6f64  ace:pre}.viewcod
+00032730: 652d 626c 6f63 6b7b 706f 7369 7469 6f6e  e-block{position
+00032740: 3a72 656c 6174 6976 657d 2e76 6965 7763  :relative}.viewc
+00032750: 6f64 652d 6261 636b 7b70 6f73 6974 696f  ode-back{positio
+00032760: 6e3a 6162 736f 6c75 7465 3b74 6f70 3a2d  n:absolute;top:-
+00032770: 312e 3572 656d 3b66 6f6e 742d 7369 7a65  1.5rem;font-size
+00032780: 3a2e 3872 656d 7d2e 636c 6173 7369 6669  :.8rem}.classifi
+00032790: 6572 7b66 6f6e 742d 7374 796c 653a 6f62  er{font-style:ob
+000327a0: 6c69 7175 653b 666f 6e74 2d77 6569 6768  lique;font-weigh
+000327b0: 743a 3430 307d 2e63 6c61 7373 6966 6965  t:400}.classifie
+000327c0: 723a 6265 666f 7265 7b66 6f6e 742d 7374  r:before{font-st
+000327d0: 796c 653a 6e6f 726d 616c 3b6d 6172 6769  yle:normal;margi
+000327e0: 6e2d 6c65 6674 3a2e 3172 656d 3b6d 6172  n-left:.1rem;mar
+000327f0: 6769 6e2d 7269 6768 743a 2e35 7265 6d3b  gin-right:.5rem;
+00032800: 636f 6e74 656e 743a 223a 223b 6469 7370  content:":";disp
+00032810: 6c61 793a 696e 6c69 6e65 2d62 6c6f 636b  lay:inline-block
+00032820: 7d2e 7975 6520 2e74 6162 6c65 2d77 7261  }.yue .table-wra
+00032830: 7070 6572 2e61 7574 6f73 756d 6d61 7279  pper.autosummary
+00032840: 7b62 6f72 6465 722d 6c65 6674 3a30 3b62  {border-left:0;b
+00032850: 6f72 6465 722d 7269 6768 743a 303b 626f  order-right:0;bo
+00032860: 7264 6572 2d72 6164 6975 733a 307d 2e79  rder-radius:0}.y
+00032870: 7565 202e 7461 626c 652d 7772 6170 7065  ue .table-wrappe
+00032880: 7220 7461 626c 652e 6175 746f 7375 6d6d  r table.autosumm
+00032890: 6172 7920 7464 7b62 6f72 6465 723a 6e6f  ary td{border:no
+000328a0: 6e65 3b70 6164 6469 6e67 2d74 6f70 3a2e  ne;padding-top:.
+000328b0: 3235 7265 6d3b 7061 6464 696e 672d 626f  25rem;padding-bo
+000328c0: 7474 6f6d 3a2e 3235 7265 6d7d 2e79 7565  ttom:.25rem}.yue
+000328d0: 2070 2e72 7562 7269 632b 6469 762e 6175   p.rubric+div.au
+000328e0: 746f 7375 6d6d 6172 797b 6d61 7267 696e  tosummary{margin
+000328f0: 2d74 6f70 3a30 7d3a 726f 6f74 7b2d 2d73  -top:0}:root{--s
+00032900: 796e 7461 782d 7072 652d 6267 3a76 6172  yntax-pre-bg:var
+00032910: 282d 2d61 6363 656e 742d 6132 293b 2d2d  (--accent-a2);--
+00032920: 7379 6e74 6178 2d63 6170 2d62 673a 7661  syntax-cap-bg:va
+00032930: 7228 2d2d 6163 6365 6e74 2d61 3329 3b2d  r(--accent-a3);-
+00032940: 2d73 796e 7461 782d 6869 6768 6c69 6768  -syntax-highligh
+00032950: 742d 6267 3a76 6172 282d 2d61 6363 656e  t-bg:var(--accen
+00032960: 742d 6133 293b 2d2d 7379 6e74 6178 2d6c  t-a3);--syntax-l
+00032970: 696e 656e 6f73 2d64 6976 6964 6572 3a76  inenos-divider:v
+00032980: 6172 282d 2d67 7261 792d 6136 293b 2d2d  ar(--gray-a6);--
+00032990: 7379 6e74 6178 2d6c 6967 6874 2d74 6578  syntax-light-tex
+000329a0: 743a 2332 3432 3932 663b 2d2d 7379 6e74  t:#24292f;--synt
+000329b0: 6178 2d6c 6967 6874 2d6d 6574 613a 2338  ax-light-meta:#8
+000329c0: 3037 6338 373b 2d2d 7379 6e74 6178 2d6c  07c87;--syntax-l
+000329d0: 6967 6874 2d63 6f6d 6d65 6e74 3a23 3665  ight-comment:#6e
+000329e0: 3737 3831 3b2d 2d73 796e 7461 782d 6c69  7781;--syntax-li
+000329f0: 6768 742d 636f 6e73 7461 6e74 3a23 3035  ght-constant:#05
+00032a00: 3530 6165 3b2d 2d73 796e 7461 782d 6c69  50ae;--syntax-li
+00032a10: 6768 742d 656e 7469 7479 3a23 3236 3862  ght-entity:#268b
+00032a20: 6432 3b2d 2d73 796e 7461 782d 6c69 6768  d2;--syntax-ligh
+00032a30: 742d 7072 6f70 6572 7479 3a23 3832 3530  t-property:#8250
+00032a40: 6466 3b2d 2d73 796e 7461 782d 6c69 6768  df;--syntax-ligh
+00032a50: 742d 6465 6669 6e69 7469 6f6e 3a23 3234  t-definition:#24
+00032a60: 3239 3266 3b2d 2d73 796e 7461 782d 6c69  292f;--syntax-li
+00032a70: 6768 742d 7461 673a 2330 3835 3b2d 2d73  ght-tag:#085;--s
+00032a80: 796e 7461 782d 6c69 6768 742d 6275 696c  yntax-light-buil
+00032a90: 7469 6e3a 2362 3538 3930 303b 2d2d 7379  tin:#b58900;--sy
+00032aa0: 6e74 6178 2d6c 6967 6874 2d6b 6579 776f  ntax-light-keywo
+00032ab0: 7264 3a23 6366 3232 3265 3b2d 2d73 796e  rd:#cf222e;--syn
+00032ac0: 7461 782d 6c69 6768 742d 6578 6365 7074  tax-light-except
+00032ad0: 696f 6e3a 2365 3632 3132 653b 2d2d 7379  ion:#e6212e;--sy
+00032ae0: 6e74 6178 2d6c 6967 6874 2d73 7472 696e  ntax-light-strin
+00032af0: 673a 2330 6133 3036 393b 2d2d 7379 6e74  g:#0a3069;--synt
+00032b00: 6178 2d6c 6967 6874 2d72 6567 6578 703a  ax-light-regexp:
+00032b10: 2365 3430 3b2d 2d73 796e 7461 782d 6c69  #e40;--syntax-li
+00032b20: 6768 742d 7661 7269 6162 6c65 3a23 6134  ght-variable:#a4
+00032b30: 3438 3066 3b2d 2d73 796e 7461 782d 6c69  480f;--syntax-li
+00032b40: 6768 742d 696e 7661 6c69 642d 696c 6c65  ght-invalid-ille
+00032b50: 6761 6c2d 7465 7874 3a23 6636 6638 6661  gal-text:#f6f8fa
+00032b60: 3b2d 2d73 796e 7461 782d 6c69 6768 742d  ;--syntax-light-
+00032b70: 696e 7661 6c69 642d 696c 6c65 6761 6c2d  invalid-illegal-
+00032b80: 6267 3a23 3832 3037 3165 3b2d 2d73 796e  bg:#82071e;--syn
+00032b90: 7461 782d 6c69 6768 742d 6d61 726b 7570  tax-light-markup
+00032ba0: 2d68 6561 6469 6e67 3a23 3035 3530 6165  -heading:#0550ae
+00032bb0: 3b2d 2d73 796e 7461 782d 6c69 6768 742d  ;--syntax-light-
+00032bc0: 6d61 726b 7570 2d69 7461 6c69 633a 2332  markup-italic:#2
 00032bd0: 3432 3932 663b 2d2d 7379 6e74 6178 2d6c  4292f;--syntax-l
-00032be0: 6967 6874 2d6d 6172 6b75 702d 6465 6c65  ight-markup-dele
-00032bf0: 7465 642d 7465 7874 3a23 3832 3037 3165  ted-text:#82071e
-00032c00: 3b2d 2d73 796e 7461 782d 6c69 6768 742d  ;--syntax-light-
-00032c10: 6d61 726b 7570 2d64 656c 6574 6564 2d62  markup-deleted-b
-00032c20: 673a 2366 6665 6265 393b 2d2d 7379 6e74  g:#ffebe9;--synt
-00032c30: 6178 2d6c 6967 6874 2d6d 6172 6b75 702d  ax-light-markup-
-00032c40: 696e 7365 7274 6564 2d74 6578 743a 2331  inserted-text:#1
-00032c50: 3136 3332 393b 2d2d 7379 6e74 6178 2d6c  16329;--syntax-l
-00032c60: 6967 6874 2d6d 6172 6b75 702d 696e 7365  ight-markup-inse
-00032c70: 7274 6564 2d62 673a 2364 6166 6265 313b  rted-bg:#dafbe1;
-00032c80: 2d2d 7379 6e74 6178 2d6c 6967 6874 2d6d  --syntax-light-m
-00032c90: 6172 6b75 702d 6368 616e 6765 642d 7465  arkup-changed-te
-00032ca0: 7874 3a23 3935 3338 3030 3b2d 2d73 796e  xt:#953800;--syn
-00032cb0: 7461 782d 6c69 6768 742d 6d61 726b 7570  tax-light-markup
-00032cc0: 2d63 6861 6e67 6564 2d62 673a 2366 6664  -changed-bg:#ffd
-00032cd0: 3862 353b 2d2d 7379 6e74 6178 2d6c 6967  8b5;--syntax-lig
-00032ce0: 6874 2d6d 6172 6b75 702d 6967 6e6f 7265  ht-markup-ignore
-00032cf0: 642d 7465 7874 3a23 6561 6565 6632 3b2d  d-text:#eaeef2;-
-00032d00: 2d73 796e 7461 782d 6c69 6768 742d 6d61  -syntax-light-ma
-00032d10: 726b 7570 2d69 676e 6f72 6564 2d62 673a  rkup-ignored-bg:
-00032d20: 2330 3535 3061 653b 2d2d 7379 6e74 6178  #0550ae;--syntax
-00032d30: 2d6c 6967 6874 2d6d 6574 612d 6469 6666  -light-meta-diff
-00032d40: 2d72 616e 6765 3a23 3832 3530 6466 3b2d  -range:#8250df;-
-00032d50: 2d73 796e 7461 782d 6c69 6768 742d 7370  -syntax-light-sp
-00032d60: 6563 6961 6c2d 6267 3a23 6463 6361 6661  ecial-bg:#dccafa
-00032d70: 3b2d 2d73 796e 7461 782d 6461 726b 2d74  ;--syntax-dark-t
-00032d80: 6578 743a 2363 3964 3164 393b 2d2d 7379  ext:#c9d1d9;--sy
-00032d90: 6e74 6178 2d64 6172 6b2d 6d65 7461 3a23  ntax-dark-meta:#
-00032da0: 3665 3737 3831 3b2d 2d73 796e 7461 782d  6e7781;--syntax-
-00032db0: 6461 726b 2d63 6f6d 6d65 6e74 3a23 3862  dark-comment:#8b
-00032dc0: 3934 3965 3b2d 2d73 796e 7461 782d 6461  949e;--syntax-da
-00032dd0: 726b 2d63 6f6e 7374 616e 743a 2337 3963  rk-constant:#79c
-00032de0: 3066 663b 2d2d 7379 6e74 6178 2d64 6172  0ff;--syntax-dar
-00032df0: 6b2d 656e 7469 7479 3a23 3437 6230 6661  k-entity:#47b0fa
-00032e00: 3b2d 2d73 796e 7461 782d 6461 726b 2d70  ;--syntax-dark-p
-00032e10: 726f 7065 7274 793a 2364 3261 3866 663b  roperty:#d2a8ff;
-00032e20: 2d2d 7379 6e74 6178 2d64 6172 6b2d 6465  --syntax-dark-de
-00032e30: 6669 6e69 7469 6f6e 3a23 6339 6431 6439  finition:#c9d1d9
-00032e40: 3b2d 2d73 796e 7461 782d 6461 726b 2d74  ;--syntax-dark-t
-00032e50: 6167 3a23 3765 6537 3837 3b2d 2d73 796e  ag:#7ee787;--syn
-00032e60: 7461 782d 6461 726b 2d62 7569 6c74 696e  tax-dark-builtin
-00032e70: 3a23 6666 6433 3463 3b2d 2d73 796e 7461  :#ffd34c;--synta
-00032e80: 782d 6461 726b 2d6b 6579 776f 7264 3a23  x-dark-keyword:#
-00032e90: 6666 3762 3732 3b2d 2d73 796e 7461 782d  ff7b72;--syntax-
-00032ea0: 6461 726b 2d65 7863 6570 7469 6f6e 3a23  dark-exception:#
-00032eb0: 6461 3437 3363 3b2d 2d73 796e 7461 782d  da473c;--syntax-
-00032ec0: 6461 726b 2d73 7472 696e 673a 2361 3564  dark-string:#a5d
-00032ed0: 3666 663b 2d2d 7379 6e74 6178 2d64 6172  6ff;--syntax-dar
-00032ee0: 6b2d 7265 6765 7870 3a23 6566 3935 3465  k-regexp:#ef954e
-00032ef0: 3b2d 2d73 796e 7461 782d 6461 726b 2d76  ;--syntax-dark-v
-00032f00: 6172 6961 626c 653a 2366 6661 3635 373b  ariable:#ffa657;
-00032f10: 2d2d 7379 6e74 6178 2d64 6172 6b2d 696e  --syntax-dark-in
-00032f20: 7661 6c69 642d 696c 6c65 6761 6c2d 7465  valid-illegal-te
-00032f30: 7874 3a23 6630 6636 6663 3b2d 2d73 796e  xt:#f0f6fc;--syn
-00032f40: 7461 782d 6461 726b 2d69 6e76 616c 6964  tax-dark-invalid
-00032f50: 2d69 6c6c 6567 616c 2d62 673a 2338 6531  -illegal-bg:#8e1
-00032f60: 3531 393b 2d2d 7379 6e74 6178 2d64 6172  519;--syntax-dar
-00032f70: 6b2d 6d61 726b 7570 2d68 6561 6469 6e67  k-markup-heading
-00032f80: 3a23 3166 3666 6562 3b2d 2d73 796e 7461  :#1f6feb;--synta
-00032f90: 782d 6461 726b 2d6d 6172 6b75 702d 6974  x-dark-markup-it
-00032fa0: 616c 6963 3a23 6339 6431 6439 3b2d 2d73  alic:#c9d1d9;--s
-00032fb0: 796e 7461 782d 6461 726b 2d6d 6172 6b75  yntax-dark-marku
-00032fc0: 702d 626f 6c64 3a23 6339 6431 6439 3b2d  p-bold:#c9d1d9;-
-00032fd0: 2d73 796e 7461 782d 6461 726b 2d6d 6172  -syntax-dark-mar
-00032fe0: 6b75 702d 6465 6c65 7465 642d 7465 7874  kup-deleted-text
-00032ff0: 3a23 6666 6463 6437 3b2d 2d73 796e 7461  :#ffdcd7;--synta
-00033000: 782d 6461 726b 2d6d 6172 6b75 702d 6465  x-dark-markup-de
-00033010: 6c65 7465 642d 6267 3a23 3637 3036 3063  leted-bg:#67060c
-00033020: 3b2d 2d73 796e 7461 782d 6461 726b 2d6d  ;--syntax-dark-m
-00033030: 6172 6b75 702d 696e 7365 7274 6564 2d74  arkup-inserted-t
-00033040: 6578 743a 2361 6666 3562 343b 2d2d 7379  ext:#aff5b4;--sy
-00033050: 6e74 6178 2d64 6172 6b2d 6d61 726b 7570  ntax-dark-markup
-00033060: 2d69 6e73 6572 7465 642d 6267 3a23 3033  -inserted-bg:#03
-00033070: 3361 3136 3b2d 2d73 796e 7461 782d 6461  3a16;--syntax-da
-00033080: 726b 2d6d 6172 6b75 702d 6368 616e 6765  rk-markup-change
-00033090: 642d 7465 7874 3a23 6666 6466 6236 3b2d  d-text:#ffdfb6;-
-000330a0: 2d73 796e 7461 782d 6461 726b 2d6d 6172  -syntax-dark-mar
-000330b0: 6b75 702d 6368 616e 6765 642d 6267 3a23  kup-changed-bg:#
-000330c0: 3561 3165 3032 3b2d 2d73 796e 7461 782d  5a1e02;--syntax-
-000330d0: 6461 726b 2d6d 6172 6b75 702d 6967 6e6f  dark-markup-igno
-000330e0: 7265 642d 7465 7874 3a23 6339 6431 6439  red-text:#c9d1d9
-000330f0: 3b2d 2d73 796e 7461 782d 6461 726b 2d6d  ;--syntax-dark-m
-00033100: 6172 6b75 702d 6967 6e6f 7265 642d 6267  arkup-ignored-bg
-00033110: 3a23 3131 3538 6337 3b2d 2d73 796e 7461  :#1158c7;--synta
-00033120: 782d 6461 726b 2d6d 6574 612d 6469 6666  x-dark-meta-diff
-00033130: 2d72 616e 6765 3a23 6432 6138 6666 3b2d  -range:#d2a8ff;-
-00033140: 2d73 796e 7461 782d 6461 726b 2d73 7065  -syntax-dark-spe
-00033150: 6369 616c 2d62 673a 2334 6634 3235 647d  cial-bg:#4f425d}
-00033160: 3a72 6f6f 742c 6874 6d6c 2e6c 6967 6874  :root,html.light
-00033170: 7b2d 2d73 796e 7461 782d 7465 7874 3a76  {--syntax-text:v
-00033180: 6172 282d 2d73 796e 7461 782d 6c69 6768  ar(--syntax-ligh
-00033190: 742d 7465 7874 293b 2d2d 7379 6e74 6178  t-text);--syntax
-000331a0: 2d6d 6574 613a 7661 7228 2d2d 7379 6e74  -meta:var(--synt
-000331b0: 6178 2d6c 6967 6874 2d6d 6574 6129 3b2d  ax-light-meta);-
-000331c0: 2d73 796e 7461 782d 636f 6d6d 656e 743a  -syntax-comment:
-000331d0: 7661 7228 2d2d 7379 6e74 6178 2d6c 6967  var(--syntax-lig
-000331e0: 6874 2d63 6f6d 6d65 6e74 293b 2d2d 7379  ht-comment);--sy
-000331f0: 6e74 6178 2d63 6f6e 7374 616e 743a 7661  ntax-constant:va
-00033200: 7228 2d2d 7379 6e74 6178 2d6c 6967 6874  r(--syntax-light
-00033210: 2d63 6f6e 7374 616e 7429 3b2d 2d73 796e  -constant);--syn
-00033220: 7461 782d 656e 7469 7479 3a76 6172 282d  tax-entity:var(-
-00033230: 2d73 796e 7461 782d 6c69 6768 742d 656e  -syntax-light-en
-00033240: 7469 7479 293b 2d2d 7379 6e74 6178 2d70  tity);--syntax-p
-00033250: 726f 7065 7274 793a 7661 7228 2d2d 7379  roperty:var(--sy
-00033260: 6e74 6178 2d6c 6967 6874 2d70 726f 7065  ntax-light-prope
-00033270: 7274 7929 3b2d 2d73 796e 7461 782d 6465  rty);--syntax-de
-00033280: 6669 6e69 7469 6f6e 3a76 6172 282d 2d73  finition:var(--s
-00033290: 796e 7461 782d 6c69 6768 742d 6465 6669  yntax-light-defi
-000332a0: 6e69 7469 6f6e 293b 2d2d 7379 6e74 6178  nition);--syntax
-000332b0: 2d74 6167 3a76 6172 282d 2d73 796e 7461  -tag:var(--synta
-000332c0: 782d 6c69 6768 742d 7461 6729 3b2d 2d73  x-light-tag);--s
-000332d0: 796e 7461 782d 6275 696c 7469 6e3a 7661  yntax-builtin:va
-000332e0: 7228 2d2d 7379 6e74 6178 2d6c 6967 6874  r(--syntax-light
-000332f0: 2d62 7569 6c74 696e 293b 2d2d 7379 6e74  -builtin);--synt
-00033300: 6178 2d6b 6579 776f 7264 3a76 6172 282d  ax-keyword:var(-
-00033310: 2d73 796e 7461 782d 6c69 6768 742d 6b65  -syntax-light-ke
-00033320: 7977 6f72 6429 3b2d 2d73 796e 7461 782d  yword);--syntax-
-00033330: 6578 6365 7074 696f 6e3a 7661 7228 2d2d  exception:var(--
-00033340: 7379 6e74 6178 2d6c 6967 6874 2d65 7863  syntax-light-exc
-00033350: 6570 7469 6f6e 293b 2d2d 7379 6e74 6178  eption);--syntax
-00033360: 2d73 7472 696e 673a 7661 7228 2d2d 7379  -string:var(--sy
-00033370: 6e74 6178 2d6c 6967 6874 2d73 7472 696e  ntax-light-strin
-00033380: 6729 3b2d 2d73 796e 7461 782d 7265 6765  g);--syntax-rege
-00033390: 7870 3a76 6172 282d 2d73 796e 7461 782d  xp:var(--syntax-
-000333a0: 6c69 6768 742d 7265 6765 7870 293b 2d2d  light-regexp);--
-000333b0: 7379 6e74 6178 2d76 6172 6961 626c 653a  syntax-variable:
-000333c0: 7661 7228 2d2d 7379 6e74 6178 2d6c 6967  var(--syntax-lig
-000333d0: 6874 2d76 6172 6961 626c 6529 3b2d 2d73  ht-variable);--s
-000333e0: 796e 7461 782d 696e 7661 6c69 642d 696c  yntax-invalid-il
-000333f0: 6c65 6761 6c2d 7465 7874 3a76 6172 282d  legal-text:var(-
-00033400: 2d73 796e 7461 782d 6c69 6768 742d 696e  -syntax-light-in
-00033410: 7661 6c69 642d 696c 6c65 6761 6c2d 7465  valid-illegal-te
-00033420: 7874 293b 2d2d 7379 6e74 6178 2d69 6e76  xt);--syntax-inv
-00033430: 616c 6964 2d69 6c6c 6567 616c 2d62 673a  alid-illegal-bg:
-00033440: 7661 7228 2d2d 7379 6e74 6178 2d6c 6967  var(--syntax-lig
-00033450: 6874 2d69 6e76 616c 6964 2d69 6c6c 6567  ht-invalid-illeg
-00033460: 616c 2d62 6729 3b2d 2d73 796e 7461 782d  al-bg);--syntax-
-00033470: 6d61 726b 7570 2d68 6561 6469 6e67 3a76  markup-heading:v
-00033480: 6172 282d 2d73 796e 7461 782d 6c69 6768  ar(--syntax-ligh
-00033490: 742d 6d61 726b 7570 2d68 6561 6469 6e67  t-markup-heading
-000334a0: 293b 2d2d 7379 6e74 6178 2d6d 6172 6b75  );--syntax-marku
-000334b0: 702d 6974 616c 6963 3a76 6172 282d 2d73  p-italic:var(--s
-000334c0: 796e 7461 782d 6c69 6768 742d 6d61 726b  yntax-light-mark
-000334d0: 7570 2d69 7461 6c69 6329 3b2d 2d73 796e  up-italic);--syn
-000334e0: 7461 782d 6d61 726b 7570 2d62 6f6c 643a  tax-markup-bold:
-000334f0: 7661 7228 2d2d 7379 6e74 6178 2d6c 6967  var(--syntax-lig
-00033500: 6874 2d6d 6172 6b75 702d 626f 6c64 293b  ht-markup-bold);
-00033510: 2d2d 7379 6e74 6178 2d6d 6172 6b75 702d  --syntax-markup-
-00033520: 6465 6c65 7465 642d 7465 7874 3a76 6172  deleted-text:var
-00033530: 282d 2d73 796e 7461 782d 6c69 6768 742d  (--syntax-light-
-00033540: 6d61 726b 7570 2d64 656c 6574 6564 2d74  markup-deleted-t
-00033550: 6578 7429 3b2d 2d73 796e 7461 782d 6d61  ext);--syntax-ma
-00033560: 726b 7570 2d64 656c 6574 6564 2d62 673a  rkup-deleted-bg:
-00033570: 7661 7228 2d2d 7379 6e74 6178 2d6c 6967  var(--syntax-lig
-00033580: 6874 2d6d 6172 6b75 702d 6465 6c65 7465  ht-markup-delete
-00033590: 642d 6267 293b 2d2d 7379 6e74 6178 2d6d  d-bg);--syntax-m
-000335a0: 6172 6b75 702d 696e 7365 7274 6564 2d74  arkup-inserted-t
-000335b0: 6578 743a 7661 7228 2d2d 7379 6e74 6178  ext:var(--syntax
-000335c0: 2d6c 6967 6874 2d6d 6172 6b75 702d 696e  -light-markup-in
-000335d0: 7365 7274 6564 2d74 6578 7429 3b2d 2d73  serted-text);--s
-000335e0: 796e 7461 782d 6d61 726b 7570 2d69 6e73  yntax-markup-ins
-000335f0: 6572 7465 642d 6267 3a76 6172 282d 2d73  erted-bg:var(--s
-00033600: 796e 7461 782d 6c69 6768 742d 6d61 726b  yntax-light-mark
-00033610: 7570 2d69 6e73 6572 7465 642d 6267 293b  up-inserted-bg);
-00033620: 2d2d 7379 6e74 6178 2d6d 6172 6b75 702d  --syntax-markup-
-00033630: 6368 616e 6765 642d 7465 7874 3a76 6172  changed-text:var
-00033640: 282d 2d73 796e 7461 782d 6c69 6768 742d  (--syntax-light-
-00033650: 6d61 726b 7570 2d63 6861 6e67 6564 2d74  markup-changed-t
-00033660: 6578 7429 3b2d 2d73 796e 7461 782d 6d61  ext);--syntax-ma
-00033670: 726b 7570 2d63 6861 6e67 6564 2d62 673a  rkup-changed-bg:
-00033680: 7661 7228 2d2d 7379 6e74 6178 2d6c 6967  var(--syntax-lig
-00033690: 6874 2d6d 6172 6b75 702d 6368 616e 6765  ht-markup-change
-000336a0: 642d 6267 293b 2d2d 7379 6e74 6178 2d6d  d-bg);--syntax-m
-000336b0: 6172 6b75 702d 6967 6e6f 7265 642d 7465  arkup-ignored-te
-000336c0: 7874 3a76 6172 282d 2d73 796e 7461 782d  xt:var(--syntax-
-000336d0: 6c69 6768 742d 6d61 726b 7570 2d69 676e  light-markup-ign
-000336e0: 6f72 6564 2d74 6578 7429 3b2d 2d73 796e  ored-text);--syn
-000336f0: 7461 782d 6d61 726b 7570 2d69 676e 6f72  tax-markup-ignor
-00033700: 6564 2d62 673a 7661 7228 2d2d 7379 6e74  ed-bg:var(--synt
-00033710: 6178 2d6c 6967 6874 2d6d 6172 6b75 702d  ax-light-markup-
-00033720: 6967 6e6f 7265 642d 6267 293b 2d2d 7379  ignored-bg);--sy
-00033730: 6e74 6178 2d6d 6574 612d 6469 6666 2d72  ntax-meta-diff-r
-00033740: 616e 6765 3a76 6172 282d 2d73 796e 7461  ange:var(--synta
-00033750: 782d 6c69 6768 742d 6d65 7461 2d64 6966  x-light-meta-dif
-00033760: 662d 7261 6e67 6529 3b2d 2d73 796e 7461  f-range);--synta
-00033770: 782d 7370 6563 6961 6c2d 6267 3a76 6172  x-special-bg:var
-00033780: 282d 2d73 796e 7461 782d 6c69 6768 742d  (--syntax-light-
-00033790: 7370 6563 6961 6c2d 6267 297d 406d 6564  special-bg)}@med
-000337a0: 6961 2028 7072 6566 6572 732d 636f 6c6f  ia (prefers-colo
-000337b0: 722d 7363 6865 6d65 3a64 6172 6b29 7b3a  r-scheme:dark){:
-000337c0: 726f 6f74 7b2d 2d73 796e 7461 782d 7465  root{--syntax-te
-000337d0: 7874 3a76 6172 282d 2d73 796e 7461 782d  xt:var(--syntax-
-000337e0: 6461 726b 2d74 6578 7429 3b2d 2d73 796e  dark-text);--syn
-000337f0: 7461 782d 6d65 7461 3a76 6172 282d 2d73  tax-meta:var(--s
-00033800: 796e 7461 782d 6461 726b 2d6d 6574 6129  yntax-dark-meta)
-00033810: 3b2d 2d73 796e 7461 782d 636f 6d6d 656e  ;--syntax-commen
-00033820: 743a 7661 7228 2d2d 7379 6e74 6178 2d64  t:var(--syntax-d
-00033830: 6172 6b2d 636f 6d6d 656e 7429 3b2d 2d73  ark-comment);--s
-00033840: 796e 7461 782d 636f 6e73 7461 6e74 3a76  yntax-constant:v
-00033850: 6172 282d 2d73 796e 7461 782d 6461 726b  ar(--syntax-dark
-00033860: 2d63 6f6e 7374 616e 7429 3b2d 2d73 796e  -constant);--syn
-00033870: 7461 782d 656e 7469 7479 3a76 6172 282d  tax-entity:var(-
-00033880: 2d73 796e 7461 782d 6461 726b 2d65 6e74  -syntax-dark-ent
-00033890: 6974 7929 3b2d 2d73 796e 7461 782d 7072  ity);--syntax-pr
-000338a0: 6f70 6572 7479 3a76 6172 282d 2d73 796e  operty:var(--syn
-000338b0: 7461 782d 6461 726b 2d70 726f 7065 7274  tax-dark-propert
-000338c0: 7929 3b2d 2d73 796e 7461 782d 6465 6669  y);--syntax-defi
-000338d0: 6e69 7469 6f6e 3a76 6172 282d 2d73 796e  nition:var(--syn
-000338e0: 7461 782d 6461 726b 2d64 6566 696e 6974  tax-dark-definit
-000338f0: 696f 6e29 3b2d 2d73 796e 7461 782d 7461  ion);--syntax-ta
-00033900: 673a 7661 7228 2d2d 7379 6e74 6178 2d64  g:var(--syntax-d
-00033910: 6172 6b2d 7461 6729 3b2d 2d73 796e 7461  ark-tag);--synta
-00033920: 782d 6275 696c 7469 6e3a 7661 7228 2d2d  x-builtin:var(--
-00033930: 7379 6e74 6178 2d64 6172 6b2d 6275 696c  syntax-dark-buil
-00033940: 7469 6e29 3b2d 2d73 796e 7461 782d 6b65  tin);--syntax-ke
-00033950: 7977 6f72 643a 7661 7228 2d2d 7379 6e74  yword:var(--synt
-00033960: 6178 2d64 6172 6b2d 6b65 7977 6f72 6429  ax-dark-keyword)
-00033970: 3b2d 2d73 796e 7461 782d 6578 6365 7074  ;--syntax-except
-00033980: 696f 6e3a 7661 7228 2d2d 7379 6e74 6178  ion:var(--syntax
-00033990: 2d64 6172 6b2d 6578 6365 7074 696f 6e29  -dark-exception)
-000339a0: 3b2d 2d73 796e 7461 782d 7374 7269 6e67  ;--syntax-string
-000339b0: 3a76 6172 282d 2d73 796e 7461 782d 6461  :var(--syntax-da
-000339c0: 726b 2d73 7472 696e 6729 3b2d 2d73 796e  rk-string);--syn
-000339d0: 7461 782d 7265 6765 7870 3a76 6172 282d  tax-regexp:var(-
-000339e0: 2d73 796e 7461 782d 6461 726b 2d72 6567  -syntax-dark-reg
-000339f0: 6578 7029 3b2d 2d73 796e 7461 782d 7661  exp);--syntax-va
-00033a00: 7269 6162 6c65 3a76 6172 282d 2d73 796e  riable:var(--syn
-00033a10: 7461 782d 6461 726b 2d76 6172 6961 626c  tax-dark-variabl
-00033a20: 6529 3b2d 2d73 796e 7461 782d 696e 7661  e);--syntax-inva
-00033a30: 6c69 642d 696c 6c65 6761 6c2d 7465 7874  lid-illegal-text
-00033a40: 3a76 6172 282d 2d73 796e 7461 782d 6461  :var(--syntax-da
-00033a50: 726b 2d69 6e76 616c 6964 2d69 6c6c 6567  rk-invalid-illeg
-00033a60: 616c 2d74 6578 7429 3b2d 2d73 796e 7461  al-text);--synta
-00033a70: 782d 696e 7661 6c69 642d 696c 6c65 6761  x-invalid-illega
-00033a80: 6c2d 6267 3a76 6172 282d 2d73 796e 7461  l-bg:var(--synta
-00033a90: 782d 6461 726b 2d69 6e76 616c 6964 2d69  x-dark-invalid-i
-00033aa0: 6c6c 6567 616c 2d62 6729 3b2d 2d73 796e  llegal-bg);--syn
-00033ab0: 7461 782d 6d61 726b 7570 2d68 6561 6469  tax-markup-headi
-00033ac0: 6e67 3a76 6172 282d 2d73 796e 7461 782d  ng:var(--syntax-
-00033ad0: 6461 726b 2d6d 6172 6b75 702d 6865 6164  dark-markup-head
-00033ae0: 696e 6729 3b2d 2d73 796e 7461 782d 6d61  ing);--syntax-ma
-00033af0: 726b 7570 2d69 7461 6c69 633a 7661 7228  rkup-italic:var(
-00033b00: 2d2d 7379 6e74 6178 2d64 6172 6b2d 6d61  --syntax-dark-ma
-00033b10: 726b 7570 2d69 7461 6c69 6329 3b2d 2d73  rkup-italic);--s
-00033b20: 796e 7461 782d 6d61 726b 7570 2d62 6f6c  yntax-markup-bol
-00033b30: 643a 7661 7228 2d2d 7379 6e74 6178 2d64  d:var(--syntax-d
-00033b40: 6172 6b2d 6d61 726b 7570 2d62 6f6c 6429  ark-markup-bold)
-00033b50: 3b2d 2d73 796e 7461 782d 6d61 726b 7570  ;--syntax-markup
-00033b60: 2d64 656c 6574 6564 2d74 6578 743a 7661  -deleted-text:va
-00033b70: 7228 2d2d 7379 6e74 6178 2d64 6172 6b2d  r(--syntax-dark-
-00033b80: 6d61 726b 7570 2d64 656c 6574 6564 2d74  markup-deleted-t
-00033b90: 6578 7429 3b2d 2d73 796e 7461 782d 6d61  ext);--syntax-ma
-00033ba0: 726b 7570 2d64 656c 6574 6564 2d62 673a  rkup-deleted-bg:
-00033bb0: 7661 7228 2d2d 7379 6e74 6178 2d64 6172  var(--syntax-dar
-00033bc0: 6b2d 6d61 726b 7570 2d64 656c 6574 6564  k-markup-deleted
-00033bd0: 2d62 6729 3b2d 2d73 796e 7461 782d 6d61  -bg);--syntax-ma
-00033be0: 726b 7570 2d69 6e73 6572 7465 642d 7465  rkup-inserted-te
-00033bf0: 7874 3a76 6172 282d 2d73 796e 7461 782d  xt:var(--syntax-
-00033c00: 6461 726b 2d6d 6172 6b75 702d 696e 7365  dark-markup-inse
-00033c10: 7274 6564 2d74 6578 7429 3b2d 2d73 796e  rted-text);--syn
-00033c20: 7461 782d 6d61 726b 7570 2d69 6e73 6572  tax-markup-inser
-00033c30: 7465 642d 6267 3a76 6172 282d 2d73 796e  ted-bg:var(--syn
-00033c40: 7461 782d 6461 726b 2d6d 6172 6b75 702d  tax-dark-markup-
-00033c50: 696e 7365 7274 6564 2d62 6729 3b2d 2d73  inserted-bg);--s
-00033c60: 796e 7461 782d 6d61 726b 7570 2d63 6861  yntax-markup-cha
-00033c70: 6e67 6564 2d74 6578 743a 7661 7228 2d2d  nged-text:var(--
-00033c80: 7379 6e74 6178 2d64 6172 6b2d 6d61 726b  syntax-dark-mark
-00033c90: 7570 2d63 6861 6e67 6564 2d74 6578 7429  up-changed-text)
-00033ca0: 3b2d 2d73 796e 7461 782d 6d61 726b 7570  ;--syntax-markup
-00033cb0: 2d63 6861 6e67 6564 2d62 673a 7661 7228  -changed-bg:var(
-00033cc0: 2d2d 7379 6e74 6178 2d64 6172 6b2d 6d61  --syntax-dark-ma
-00033cd0: 726b 7570 2d63 6861 6e67 6564 2d62 6729  rkup-changed-bg)
-00033ce0: 3b2d 2d73 796e 7461 782d 6d61 726b 7570  ;--syntax-markup
-00033cf0: 2d69 676e 6f72 6564 2d74 6578 743a 7661  -ignored-text:va
-00033d00: 7228 2d2d 7379 6e74 6178 2d64 6172 6b2d  r(--syntax-dark-
-00033d10: 6d61 726b 7570 2d69 676e 6f72 6564 2d74  markup-ignored-t
-00033d20: 6578 7429 3b2d 2d73 796e 7461 782d 6d61  ext);--syntax-ma
-00033d30: 726b 7570 2d69 676e 6f72 6564 2d62 673a  rkup-ignored-bg:
-00033d40: 7661 7228 2d2d 7379 6e74 6178 2d64 6172  var(--syntax-dar
-00033d50: 6b2d 6d61 726b 7570 2d69 676e 6f72 6564  k-markup-ignored
-00033d60: 2d62 6729 3b2d 2d73 796e 7461 782d 6d65  -bg);--syntax-me
-00033d70: 7461 2d64 6966 662d 7261 6e67 653a 7661  ta-diff-range:va
-00033d80: 7228 2d2d 7379 6e74 6178 2d64 6172 6b2d  r(--syntax-dark-
-00033d90: 6d65 7461 2d64 6966 662d 7261 6e67 6529  meta-diff-range)
-00033da0: 3b2d 2d73 796e 7461 782d 7370 6563 6961  ;--syntax-specia
-00033db0: 6c2d 6267 3a76 6172 282d 2d73 796e 7461  l-bg:var(--synta
-00033dc0: 782d 6461 726b 2d73 7065 6369 616c 2d62  x-dark-special-b
-00033dd0: 6729 7d7d 6874 6d6c 2e64 6172 6b7b 2d2d  g)}}html.dark{--
-00033de0: 7379 6e74 6178 2d74 6578 743a 7661 7228  syntax-text:var(
-00033df0: 2d2d 7379 6e74 6178 2d64 6172 6b2d 7465  --syntax-dark-te
-00033e00: 7874 293b 2d2d 7379 6e74 6178 2d6d 6574  xt);--syntax-met
-00033e10: 613a 7661 7228 2d2d 7379 6e74 6178 2d64  a:var(--syntax-d
-00033e20: 6172 6b2d 6d65 7461 293b 2d2d 7379 6e74  ark-meta);--synt
-00033e30: 6178 2d63 6f6d 6d65 6e74 3a76 6172 282d  ax-comment:var(-
-00033e40: 2d73 796e 7461 782d 6461 726b 2d63 6f6d  -syntax-dark-com
-00033e50: 6d65 6e74 293b 2d2d 7379 6e74 6178 2d63  ment);--syntax-c
-00033e60: 6f6e 7374 616e 743a 7661 7228 2d2d 7379  onstant:var(--sy
-00033e70: 6e74 6178 2d64 6172 6b2d 636f 6e73 7461  ntax-dark-consta
-00033e80: 6e74 293b 2d2d 7379 6e74 6178 2d65 6e74  nt);--syntax-ent
-00033e90: 6974 793a 7661 7228 2d2d 7379 6e74 6178  ity:var(--syntax
-00033ea0: 2d64 6172 6b2d 656e 7469 7479 293b 2d2d  -dark-entity);--
-00033eb0: 7379 6e74 6178 2d70 726f 7065 7274 793a  syntax-property:
-00033ec0: 7661 7228 2d2d 7379 6e74 6178 2d64 6172  var(--syntax-dar
-00033ed0: 6b2d 7072 6f70 6572 7479 293b 2d2d 7379  k-property);--sy
-00033ee0: 6e74 6178 2d64 6566 696e 6974 696f 6e3a  ntax-definition:
-00033ef0: 7661 7228 2d2d 7379 6e74 6178 2d64 6172  var(--syntax-dar
-00033f00: 6b2d 6465 6669 6e69 7469 6f6e 293b 2d2d  k-definition);--
-00033f10: 7379 6e74 6178 2d74 6167 3a76 6172 282d  syntax-tag:var(-
-00033f20: 2d73 796e 7461 782d 6461 726b 2d74 6167  -syntax-dark-tag
-00033f30: 293b 2d2d 7379 6e74 6178 2d62 7569 6c74  );--syntax-built
-00033f40: 696e 3a76 6172 282d 2d73 796e 7461 782d  in:var(--syntax-
-00033f50: 6461 726b 2d62 7569 6c74 696e 293b 2d2d  dark-builtin);--
-00033f60: 7379 6e74 6178 2d6b 6579 776f 7264 3a76  syntax-keyword:v
-00033f70: 6172 282d 2d73 796e 7461 782d 6461 726b  ar(--syntax-dark
-00033f80: 2d6b 6579 776f 7264 293b 2d2d 7379 6e74  -keyword);--synt
-00033f90: 6178 2d65 7863 6570 7469 6f6e 3a76 6172  ax-exception:var
-00033fa0: 282d 2d73 796e 7461 782d 6461 726b 2d65  (--syntax-dark-e
-00033fb0: 7863 6570 7469 6f6e 293b 2d2d 7379 6e74  xception);--synt
-00033fc0: 6178 2d73 7472 696e 673a 7661 7228 2d2d  ax-string:var(--
-00033fd0: 7379 6e74 6178 2d64 6172 6b2d 7374 7269  syntax-dark-stri
-00033fe0: 6e67 293b 2d2d 7379 6e74 6178 2d72 6567  ng);--syntax-reg
-00033ff0: 6578 703a 7661 7228 2d2d 7379 6e74 6178  exp:var(--syntax
-00034000: 2d64 6172 6b2d 7265 6765 7870 293b 2d2d  -dark-regexp);--
-00034010: 7379 6e74 6178 2d76 6172 6961 626c 653a  syntax-variable:
-00034020: 7661 7228 2d2d 7379 6e74 6178 2d64 6172  var(--syntax-dar
-00034030: 6b2d 7661 7269 6162 6c65 293b 2d2d 7379  k-variable);--sy
-00034040: 6e74 6178 2d69 6e76 616c 6964 2d69 6c6c  ntax-invalid-ill
-00034050: 6567 616c 2d74 6578 743a 7661 7228 2d2d  egal-text:var(--
-00034060: 7379 6e74 6178 2d64 6172 6b2d 696e 7661  syntax-dark-inva
-00034070: 6c69 642d 696c 6c65 6761 6c2d 7465 7874  lid-illegal-text
-00034080: 293b 2d2d 7379 6e74 6178 2d69 6e76 616c  );--syntax-inval
-00034090: 6964 2d69 6c6c 6567 616c 2d62 673a 7661  id-illegal-bg:va
-000340a0: 7228 2d2d 7379 6e74 6178 2d64 6172 6b2d  r(--syntax-dark-
-000340b0: 696e 7661 6c69 642d 696c 6c65 6761 6c2d  invalid-illegal-
-000340c0: 6267 293b 2d2d 7379 6e74 6178 2d6d 6172  bg);--syntax-mar
-000340d0: 6b75 702d 6865 6164 696e 673a 7661 7228  kup-heading:var(
-000340e0: 2d2d 7379 6e74 6178 2d64 6172 6b2d 6d61  --syntax-dark-ma
-000340f0: 726b 7570 2d68 6561 6469 6e67 293b 2d2d  rkup-heading);--
-00034100: 7379 6e74 6178 2d6d 6172 6b75 702d 6974  syntax-markup-it
-00034110: 616c 6963 3a76 6172 282d 2d73 796e 7461  alic:var(--synta
-00034120: 782d 6461 726b 2d6d 6172 6b75 702d 6974  x-dark-markup-it
-00034130: 616c 6963 293b 2d2d 7379 6e74 6178 2d6d  alic);--syntax-m
-00034140: 6172 6b75 702d 626f 6c64 3a76 6172 282d  arkup-bold:var(-
-00034150: 2d73 796e 7461 782d 6461 726b 2d6d 6172  -syntax-dark-mar
-00034160: 6b75 702d 626f 6c64 293b 2d2d 7379 6e74  kup-bold);--synt
-00034170: 6178 2d6d 6172 6b75 702d 6465 6c65 7465  ax-markup-delete
-00034180: 642d 7465 7874 3a76 6172 282d 2d73 796e  d-text:var(--syn
-00034190: 7461 782d 6461 726b 2d6d 6172 6b75 702d  tax-dark-markup-
-000341a0: 6465 6c65 7465 642d 7465 7874 293b 2d2d  deleted-text);--
-000341b0: 7379 6e74 6178 2d6d 6172 6b75 702d 6465  syntax-markup-de
-000341c0: 6c65 7465 642d 6267 3a76 6172 282d 2d73  leted-bg:var(--s
-000341d0: 796e 7461 782d 6461 726b 2d6d 6172 6b75  yntax-dark-marku
-000341e0: 702d 6465 6c65 7465 642d 6267 293b 2d2d  p-deleted-bg);--
-000341f0: 7379 6e74 6178 2d6d 6172 6b75 702d 696e  syntax-markup-in
-00034200: 7365 7274 6564 2d74 6578 743a 7661 7228  serted-text:var(
-00034210: 2d2d 7379 6e74 6178 2d64 6172 6b2d 6d61  --syntax-dark-ma
-00034220: 726b 7570 2d69 6e73 6572 7465 642d 7465  rkup-inserted-te
-00034230: 7874 293b 2d2d 7379 6e74 6178 2d6d 6172  xt);--syntax-mar
-00034240: 6b75 702d 696e 7365 7274 6564 2d62 673a  kup-inserted-bg:
-00034250: 7661 7228 2d2d 7379 6e74 6178 2d64 6172  var(--syntax-dar
-00034260: 6b2d 6d61 726b 7570 2d69 6e73 6572 7465  k-markup-inserte
-00034270: 642d 6267 293b 2d2d 7379 6e74 6178 2d6d  d-bg);--syntax-m
-00034280: 6172 6b75 702d 6368 616e 6765 642d 7465  arkup-changed-te
-00034290: 7874 3a76 6172 282d 2d73 796e 7461 782d  xt:var(--syntax-
-000342a0: 6461 726b 2d6d 6172 6b75 702d 6368 616e  dark-markup-chan
-000342b0: 6765 642d 7465 7874 293b 2d2d 7379 6e74  ged-text);--synt
-000342c0: 6178 2d6d 6172 6b75 702d 6368 616e 6765  ax-markup-change
-000342d0: 642d 6267 3a76 6172 282d 2d73 796e 7461  d-bg:var(--synta
-000342e0: 782d 6461 726b 2d6d 6172 6b75 702d 6368  x-dark-markup-ch
-000342f0: 616e 6765 642d 6267 293b 2d2d 7379 6e74  anged-bg);--synt
-00034300: 6178 2d6d 6172 6b75 702d 6967 6e6f 7265  ax-markup-ignore
-00034310: 642d 7465 7874 3a76 6172 282d 2d73 796e  d-text:var(--syn
-00034320: 7461 782d 6461 726b 2d6d 6172 6b75 702d  tax-dark-markup-
-00034330: 6967 6e6f 7265 642d 7465 7874 293b 2d2d  ignored-text);--
-00034340: 7379 6e74 6178 2d6d 6172 6b75 702d 6967  syntax-markup-ig
-00034350: 6e6f 7265 642d 6267 3a76 6172 282d 2d73  nored-bg:var(--s
-00034360: 796e 7461 782d 6461 726b 2d6d 6172 6b75  yntax-dark-marku
-00034370: 702d 6967 6e6f 7265 642d 6267 293b 2d2d  p-ignored-bg);--
-00034380: 7379 6e74 6178 2d6d 6574 612d 6469 6666  syntax-meta-diff
-00034390: 2d72 616e 6765 3a76 6172 282d 2d73 796e  -range:var(--syn
-000343a0: 7461 782d 6461 726b 2d6d 6574 612d 6469  tax-dark-meta-di
-000343b0: 6666 2d72 616e 6765 293b 2d2d 7379 6e74  ff-range);--synt
-000343c0: 6178 2d73 7065 6369 616c 2d62 673a 7661  ax-special-bg:va
-000343d0: 7228 2d2d 7379 6e74 6178 2d64 6172 6b2d  r(--syntax-dark-
-000343e0: 7370 6563 6961 6c2d 6267 297d 2e6c 6967  special-bg)}.lig
-000343f0: 6874 202e 6461 726b 2d63 6f64 657b 2d2d  ht .dark-code{--
-00034400: 7379 6e74 6178 2d70 7265 2d62 673a 7661  syntax-pre-bg:va
-00034410: 7228 2d2d 626c 6163 6b2d 6131 3229 3b2d  r(--black-a12);-
-00034420: 2d73 796e 7461 782d 6361 702d 6267 3a23  -syntax-cap-bg:#
-00034430: 3163 3230 3234 3b2d 2d73 796e 7461 782d  1c2024;--syntax-
-00034440: 6869 6768 6c69 6768 742d 6267 3a76 6172  highlight-bg:var
-00034450: 282d 2d77 6869 7465 2d61 3229 3b2d 2d73  (--white-a2);--s
-00034460: 796e 7461 782d 6c69 6e65 6e6f 732d 6469  yntax-linenos-di
-00034470: 7669 6465 723a 7661 7228 2d2d 7768 6974  vider:var(--whit
-00034480: 652d 6134 293b 2d2d 7379 6e74 6178 2d74  e-a4);--syntax-t
-00034490: 6578 743a 7661 7228 2d2d 7379 6e74 6178  ext:var(--syntax
-000344a0: 2d64 6172 6b2d 7465 7874 293b 2d2d 7379  -dark-text);--sy
-000344b0: 6e74 6178 2d6d 6574 613a 7661 7228 2d2d  ntax-meta:var(--
-000344c0: 7379 6e74 6178 2d64 6172 6b2d 6d65 7461  syntax-dark-meta
-000344d0: 293b 2d2d 7379 6e74 6178 2d63 6f6d 6d65  );--syntax-comme
-000344e0: 6e74 3a76 6172 282d 2d73 796e 7461 782d  nt:var(--syntax-
-000344f0: 6461 726b 2d63 6f6d 6d65 6e74 293b 2d2d  dark-comment);--
-00034500: 7379 6e74 6178 2d63 6f6e 7374 616e 743a  syntax-constant:
-00034510: 7661 7228 2d2d 7379 6e74 6178 2d64 6172  var(--syntax-dar
-00034520: 6b2d 636f 6e73 7461 6e74 293b 2d2d 7379  k-constant);--sy
-00034530: 6e74 6178 2d65 6e74 6974 793a 7661 7228  ntax-entity:var(
-00034540: 2d2d 7379 6e74 6178 2d64 6172 6b2d 656e  --syntax-dark-en
-00034550: 7469 7479 293b 2d2d 7379 6e74 6178 2d70  tity);--syntax-p
-00034560: 726f 7065 7274 793a 7661 7228 2d2d 7379  roperty:var(--sy
-00034570: 6e74 6178 2d64 6172 6b2d 7072 6f70 6572  ntax-dark-proper
-00034580: 7479 293b 2d2d 7379 6e74 6178 2d64 6566  ty);--syntax-def
-00034590: 696e 6974 696f 6e3a 7661 7228 2d2d 7379  inition:var(--sy
-000345a0: 6e74 6178 2d64 6172 6b2d 6465 6669 6e69  ntax-dark-defini
-000345b0: 7469 6f6e 293b 2d2d 7379 6e74 6178 2d74  tion);--syntax-t
-000345c0: 6167 3a76 6172 282d 2d73 796e 7461 782d  ag:var(--syntax-
-000345d0: 6461 726b 2d74 6167 293b 2d2d 7379 6e74  dark-tag);--synt
-000345e0: 6178 2d62 7569 6c74 696e 3a76 6172 282d  ax-builtin:var(-
-000345f0: 2d73 796e 7461 782d 6461 726b 2d62 7569  -syntax-dark-bui
-00034600: 6c74 696e 293b 2d2d 7379 6e74 6178 2d6b  ltin);--syntax-k
-00034610: 6579 776f 7264 3a76 6172 282d 2d73 796e  eyword:var(--syn
-00034620: 7461 782d 6461 726b 2d6b 6579 776f 7264  tax-dark-keyword
-00034630: 293b 2d2d 7379 6e74 6178 2d65 7863 6570  );--syntax-excep
-00034640: 7469 6f6e 3a76 6172 282d 2d73 796e 7461  tion:var(--synta
-00034650: 782d 6461 726b 2d65 7863 6570 7469 6f6e  x-dark-exception
-00034660: 293b 2d2d 7379 6e74 6178 2d73 7472 696e  );--syntax-strin
-00034670: 673a 7661 7228 2d2d 7379 6e74 6178 2d64  g:var(--syntax-d
-00034680: 6172 6b2d 7374 7269 6e67 293b 2d2d 7379  ark-string);--sy
-00034690: 6e74 6178 2d72 6567 6578 703a 7661 7228  ntax-regexp:var(
-000346a0: 2d2d 7379 6e74 6178 2d64 6172 6b2d 7265  --syntax-dark-re
-000346b0: 6765 7870 293b 2d2d 7379 6e74 6178 2d76  gexp);--syntax-v
-000346c0: 6172 6961 626c 653a 7661 7228 2d2d 7379  ariable:var(--sy
-000346d0: 6e74 6178 2d64 6172 6b2d 7661 7269 6162  ntax-dark-variab
-000346e0: 6c65 293b 2d2d 7379 6e74 6178 2d69 6e76  le);--syntax-inv
-000346f0: 616c 6964 2d69 6c6c 6567 616c 2d74 6578  alid-illegal-tex
-00034700: 743a 7661 7228 2d2d 7379 6e74 6178 2d64  t:var(--syntax-d
-00034710: 6172 6b2d 696e 7661 6c69 642d 696c 6c65  ark-invalid-ille
-00034720: 6761 6c2d 7465 7874 293b 2d2d 7379 6e74  gal-text);--synt
-00034730: 6178 2d69 6e76 616c 6964 2d69 6c6c 6567  ax-invalid-illeg
-00034740: 616c 2d62 673a 7661 7228 2d2d 7379 6e74  al-bg:var(--synt
-00034750: 6178 2d64 6172 6b2d 696e 7661 6c69 642d  ax-dark-invalid-
-00034760: 696c 6c65 6761 6c2d 6267 293b 2d2d 7379  illegal-bg);--sy
-00034770: 6e74 6178 2d6d 6172 6b75 702d 6865 6164  ntax-markup-head
-00034780: 696e 673a 7661 7228 2d2d 7379 6e74 6178  ing:var(--syntax
-00034790: 2d64 6172 6b2d 6d61 726b 7570 2d68 6561  -dark-markup-hea
-000347a0: 6469 6e67 293b 2d2d 7379 6e74 6178 2d6d  ding);--syntax-m
-000347b0: 6172 6b75 702d 6974 616c 6963 3a76 6172  arkup-italic:var
-000347c0: 282d 2d73 796e 7461 782d 6461 726b 2d6d  (--syntax-dark-m
-000347d0: 6172 6b75 702d 6974 616c 6963 293b 2d2d  arkup-italic);--
-000347e0: 7379 6e74 6178 2d6d 6172 6b75 702d 626f  syntax-markup-bo
-000347f0: 6c64 3a76 6172 282d 2d73 796e 7461 782d  ld:var(--syntax-
-00034800: 6461 726b 2d6d 6172 6b75 702d 626f 6c64  dark-markup-bold
-00034810: 293b 2d2d 7379 6e74 6178 2d6d 6172 6b75  );--syntax-marku
-00034820: 702d 6465 6c65 7465 642d 7465 7874 3a76  p-deleted-text:v
-00034830: 6172 282d 2d73 796e 7461 782d 6461 726b  ar(--syntax-dark
-00034840: 2d6d 6172 6b75 702d 6465 6c65 7465 642d  -markup-deleted-
-00034850: 7465 7874 293b 2d2d 7379 6e74 6178 2d6d  text);--syntax-m
-00034860: 6172 6b75 702d 6465 6c65 7465 642d 6267  arkup-deleted-bg
-00034870: 3a76 6172 282d 2d73 796e 7461 782d 6461  :var(--syntax-da
-00034880: 726b 2d6d 6172 6b75 702d 6465 6c65 7465  rk-markup-delete
-00034890: 642d 6267 293b 2d2d 7379 6e74 6178 2d6d  d-bg);--syntax-m
-000348a0: 6172 6b75 702d 696e 7365 7274 6564 2d74  arkup-inserted-t
-000348b0: 6578 743a 7661 7228 2d2d 7379 6e74 6178  ext:var(--syntax
-000348c0: 2d64 6172 6b2d 6d61 726b 7570 2d69 6e73  -dark-markup-ins
-000348d0: 6572 7465 642d 7465 7874 293b 2d2d 7379  erted-text);--sy
-000348e0: 6e74 6178 2d6d 6172 6b75 702d 696e 7365  ntax-markup-inse
-000348f0: 7274 6564 2d62 673a 7661 7228 2d2d 7379  rted-bg:var(--sy
-00034900: 6e74 6178 2d64 6172 6b2d 6d61 726b 7570  ntax-dark-markup
-00034910: 2d69 6e73 6572 7465 642d 6267 293b 2d2d  -inserted-bg);--
-00034920: 7379 6e74 6178 2d6d 6172 6b75 702d 6368  syntax-markup-ch
-00034930: 616e 6765 642d 7465 7874 3a76 6172 282d  anged-text:var(-
-00034940: 2d73 796e 7461 782d 6461 726b 2d6d 6172  -syntax-dark-mar
-00034950: 6b75 702d 6368 616e 6765 642d 7465 7874  kup-changed-text
-00034960: 293b 2d2d 7379 6e74 6178 2d6d 6172 6b75  );--syntax-marku
-00034970: 702d 6368 616e 6765 642d 6267 3a76 6172  p-changed-bg:var
-00034980: 282d 2d73 796e 7461 782d 6461 726b 2d6d  (--syntax-dark-m
-00034990: 6172 6b75 702d 6368 616e 6765 642d 6267  arkup-changed-bg
-000349a0: 293b 2d2d 7379 6e74 6178 2d6d 6172 6b75  );--syntax-marku
-000349b0: 702d 6967 6e6f 7265 642d 7465 7874 3a76  p-ignored-text:v
-000349c0: 6172 282d 2d73 796e 7461 782d 6461 726b  ar(--syntax-dark
-000349d0: 2d6d 6172 6b75 702d 6967 6e6f 7265 642d  -markup-ignored-
-000349e0: 7465 7874 293b 2d2d 7379 6e74 6178 2d6d  text);--syntax-m
-000349f0: 6172 6b75 702d 6967 6e6f 7265 642d 6267  arkup-ignored-bg
-00034a00: 3a76 6172 282d 2d73 796e 7461 782d 6461  :var(--syntax-da
-00034a10: 726b 2d6d 6172 6b75 702d 6967 6e6f 7265  rk-markup-ignore
-00034a20: 642d 6267 293b 2d2d 7379 6e74 6178 2d6d  d-bg);--syntax-m
-00034a30: 6574 612d 6469 6666 2d72 616e 6765 3a76  eta-diff-range:v
-00034a40: 6172 282d 2d73 796e 7461 782d 6461 726b  ar(--syntax-dark
-00034a50: 2d6d 6574 612d 6469 6666 2d72 616e 6765  -meta-diff-range
-00034a60: 293b 2d2d 7379 6e74 6178 2d73 7065 6369  );--syntax-speci
-00034a70: 616c 2d62 673a 7661 7228 2d2d 7379 6e74  al-bg:var(--synt
-00034a80: 6178 2d64 6172 6b2d 7370 6563 6961 6c2d  ax-dark-special-
-00034a90: 6267 297d 6874 6d6c 2e6c 6967 6874 202e  bg)}html.light .
-00034aa0: 6a75 7079 7465 725f 636f 6e74 6169 6e65  jupyter_containe
-00034ab0: 7220 2e63 656c 6c5f 6f75 7470 7574 2c68  r .cell_output,h
-00034ac0: 746d 6c2e 6c69 6768 7420 2e73 642d 7461  tml.light .sd-ta
-00034ad0: 622d 636f 6e74 656e 747b 2d2d 7379 6e74  b-content{--synt
-00034ae0: 6178 2d70 7265 2d62 673a 7661 7228 2d2d  ax-pre-bg:var(--
-00034af0: 636f 6c6f 722d 7375 7266 6163 652d 6163  color-surface-ac
-00034b00: 6365 6e74 293b 2d2d 7379 6e74 6178 2d63  cent);--syntax-c
-00034b10: 6170 2d62 673a 7661 7228 2d2d 6163 6365  ap-bg:var(--acce
-00034b20: 6e74 2d33 293b 2d2d 7379 6e74 6178 2d68  nt-3);--syntax-h
-00034b30: 6967 686c 6967 6874 2d62 673a 7661 7228  ighlight-bg:var(
-00034b40: 2d2d 6163 6365 6e74 2d61 3329 3b2d 2d73  --accent-a3);--s
-00034b50: 796e 7461 782d 7465 7874 3a76 6172 282d  yntax-text:var(-
-00034b60: 2d73 796e 7461 782d 6c69 6768 742d 7465  -syntax-light-te
-00034b70: 7874 293b 2d2d 7379 6e74 6178 2d6d 6574  xt);--syntax-met
-00034b80: 613a 7661 7228 2d2d 7379 6e74 6178 2d6c  a:var(--syntax-l
-00034b90: 6967 6874 2d6d 6574 6129 3b2d 2d73 796e  ight-meta);--syn
-00034ba0: 7461 782d 636f 6d6d 656e 743a 7661 7228  tax-comment:var(
-00034bb0: 2d2d 7379 6e74 6178 2d6c 6967 6874 2d63  --syntax-light-c
-00034bc0: 6f6d 6d65 6e74 293b 2d2d 7379 6e74 6178  omment);--syntax
-00034bd0: 2d63 6f6e 7374 616e 743a 7661 7228 2d2d  -constant:var(--
-00034be0: 7379 6e74 6178 2d6c 6967 6874 2d63 6f6e  syntax-light-con
-00034bf0: 7374 616e 7429 3b2d 2d73 796e 7461 782d  stant);--syntax-
-00034c00: 656e 7469 7479 3a76 6172 282d 2d73 796e  entity:var(--syn
-00034c10: 7461 782d 6c69 6768 742d 656e 7469 7479  tax-light-entity
-00034c20: 293b 2d2d 7379 6e74 6178 2d70 726f 7065  );--syntax-prope
-00034c30: 7274 793a 7661 7228 2d2d 7379 6e74 6178  rty:var(--syntax
-00034c40: 2d6c 6967 6874 2d70 726f 7065 7274 7929  -light-property)
-00034c50: 3b2d 2d73 796e 7461 782d 6465 6669 6e69  ;--syntax-defini
-00034c60: 7469 6f6e 3a76 6172 282d 2d73 796e 7461  tion:var(--synta
-00034c70: 782d 6c69 6768 742d 6465 6669 6e69 7469  x-light-definiti
-00034c80: 6f6e 293b 2d2d 7379 6e74 6178 2d74 6167  on);--syntax-tag
-00034c90: 3a76 6172 282d 2d73 796e 7461 782d 6c69  :var(--syntax-li
-00034ca0: 6768 742d 7461 6729 3b2d 2d73 796e 7461  ght-tag);--synta
-00034cb0: 782d 6275 696c 7469 6e3a 7661 7228 2d2d  x-builtin:var(--
-00034cc0: 7379 6e74 6178 2d6c 6967 6874 2d62 7569  syntax-light-bui
-00034cd0: 6c74 696e 293b 2d2d 7379 6e74 6178 2d6b  ltin);--syntax-k
-00034ce0: 6579 776f 7264 3a76 6172 282d 2d73 796e  eyword:var(--syn
-00034cf0: 7461 782d 6c69 6768 742d 6b65 7977 6f72  tax-light-keywor
-00034d00: 6429 3b2d 2d73 796e 7461 782d 6578 6365  d);--syntax-exce
-00034d10: 7074 696f 6e3a 7661 7228 2d2d 7379 6e74  ption:var(--synt
-00034d20: 6178 2d6c 6967 6874 2d65 7863 6570 7469  ax-light-excepti
-00034d30: 6f6e 293b 2d2d 7379 6e74 6178 2d73 7472  on);--syntax-str
-00034d40: 696e 673a 7661 7228 2d2d 7379 6e74 6178  ing:var(--syntax
-00034d50: 2d6c 6967 6874 2d73 7472 696e 6729 3b2d  -light-string);-
-00034d60: 2d73 796e 7461 782d 7265 6765 7870 3a76  -syntax-regexp:v
-00034d70: 6172 282d 2d73 796e 7461 782d 6c69 6768  ar(--syntax-ligh
-00034d80: 742d 7265 6765 7870 293b 2d2d 7379 6e74  t-regexp);--synt
-00034d90: 6178 2d76 6172 6961 626c 653a 7661 7228  ax-variable:var(
-00034da0: 2d2d 7379 6e74 6178 2d6c 6967 6874 2d76  --syntax-light-v
-00034db0: 6172 6961 626c 6529 3b2d 2d73 796e 7461  ariable);--synta
-00034dc0: 782d 696e 7661 6c69 642d 696c 6c65 6761  x-invalid-illega
-00034dd0: 6c2d 7465 7874 3a76 6172 282d 2d73 796e  l-text:var(--syn
-00034de0: 7461 782d 6c69 6768 742d 696e 7661 6c69  tax-light-invali
-00034df0: 642d 696c 6c65 6761 6c2d 7465 7874 293b  d-illegal-text);
-00034e00: 2d2d 7379 6e74 6178 2d69 6e76 616c 6964  --syntax-invalid
-00034e10: 2d69 6c6c 6567 616c 2d62 673a 7661 7228  -illegal-bg:var(
-00034e20: 2d2d 7379 6e74 6178 2d6c 6967 6874 2d69  --syntax-light-i
-00034e30: 6e76 616c 6964 2d69 6c6c 6567 616c 2d62  nvalid-illegal-b
-00034e40: 6729 3b2d 2d73 796e 7461 782d 6d61 726b  g);--syntax-mark
-00034e50: 7570 2d68 6561 6469 6e67 3a76 6172 282d  up-heading:var(-
-00034e60: 2d73 796e 7461 782d 6c69 6768 742d 6d61  -syntax-light-ma
-00034e70: 726b 7570 2d68 6561 6469 6e67 293b 2d2d  rkup-heading);--
-00034e80: 7379 6e74 6178 2d6d 6172 6b75 702d 6974  syntax-markup-it
-00034e90: 616c 6963 3a76 6172 282d 2d73 796e 7461  alic:var(--synta
-00034ea0: 782d 6c69 6768 742d 6d61 726b 7570 2d69  x-light-markup-i
-00034eb0: 7461 6c69 6329 3b2d 2d73 796e 7461 782d  talic);--syntax-
-00034ec0: 6d61 726b 7570 2d62 6f6c 643a 7661 7228  markup-bold:var(
-00034ed0: 2d2d 7379 6e74 6178 2d6c 6967 6874 2d6d  --syntax-light-m
-00034ee0: 6172 6b75 702d 626f 6c64 293b 2d2d 7379  arkup-bold);--sy
-00034ef0: 6e74 6178 2d6d 6172 6b75 702d 6465 6c65  ntax-markup-dele
-00034f00: 7465 642d 7465 7874 3a76 6172 282d 2d73  ted-text:var(--s
-00034f10: 796e 7461 782d 6c69 6768 742d 6d61 726b  yntax-light-mark
-00034f20: 7570 2d64 656c 6574 6564 2d74 6578 7429  up-deleted-text)
-00034f30: 3b2d 2d73 796e 7461 782d 6d61 726b 7570  ;--syntax-markup
-00034f40: 2d64 656c 6574 6564 2d62 673a 7661 7228  -deleted-bg:var(
-00034f50: 2d2d 7379 6e74 6178 2d6c 6967 6874 2d6d  --syntax-light-m
-00034f60: 6172 6b75 702d 6465 6c65 7465 642d 6267  arkup-deleted-bg
-00034f70: 293b 2d2d 7379 6e74 6178 2d6d 6172 6b75  );--syntax-marku
-00034f80: 702d 696e 7365 7274 6564 2d74 6578 743a  p-inserted-text:
-00034f90: 7661 7228 2d2d 7379 6e74 6178 2d6c 6967  var(--syntax-lig
-00034fa0: 6874 2d6d 6172 6b75 702d 696e 7365 7274  ht-markup-insert
-00034fb0: 6564 2d74 6578 7429 3b2d 2d73 796e 7461  ed-text);--synta
-00034fc0: 782d 6d61 726b 7570 2d69 6e73 6572 7465  x-markup-inserte
-00034fd0: 642d 6267 3a76 6172 282d 2d73 796e 7461  d-bg:var(--synta
-00034fe0: 782d 6c69 6768 742d 6d61 726b 7570 2d69  x-light-markup-i
-00034ff0: 6e73 6572 7465 642d 6267 293b 2d2d 7379  nserted-bg);--sy
-00035000: 6e74 6178 2d6d 6172 6b75 702d 6368 616e  ntax-markup-chan
-00035010: 6765 642d 7465 7874 3a76 6172 282d 2d73  ged-text:var(--s
-00035020: 796e 7461 782d 6c69 6768 742d 6d61 726b  yntax-light-mark
-00035030: 7570 2d63 6861 6e67 6564 2d74 6578 7429  up-changed-text)
-00035040: 3b2d 2d73 796e 7461 782d 6d61 726b 7570  ;--syntax-markup
-00035050: 2d63 6861 6e67 6564 2d62 673a 7661 7228  -changed-bg:var(
-00035060: 2d2d 7379 6e74 6178 2d6c 6967 6874 2d6d  --syntax-light-m
-00035070: 6172 6b75 702d 6368 616e 6765 642d 6267  arkup-changed-bg
-00035080: 293b 2d2d 7379 6e74 6178 2d6d 6172 6b75  );--syntax-marku
-00035090: 702d 6967 6e6f 7265 642d 7465 7874 3a76  p-ignored-text:v
-000350a0: 6172 282d 2d73 796e 7461 782d 6c69 6768  ar(--syntax-ligh
-000350b0: 742d 6d61 726b 7570 2d69 676e 6f72 6564  t-markup-ignored
-000350c0: 2d74 6578 7429 3b2d 2d73 796e 7461 782d  -text);--syntax-
-000350d0: 6d61 726b 7570 2d69 676e 6f72 6564 2d62  markup-ignored-b
-000350e0: 673a 7661 7228 2d2d 7379 6e74 6178 2d6c  g:var(--syntax-l
-000350f0: 6967 6874 2d6d 6172 6b75 702d 6967 6e6f  ight-markup-igno
-00035100: 7265 642d 6267 293b 2d2d 7379 6e74 6178  red-bg);--syntax
-00035110: 2d6d 6574 612d 6469 6666 2d72 616e 6765  -meta-diff-range
-00035120: 3a76 6172 282d 2d73 796e 7461 782d 6c69  :var(--syntax-li
-00035130: 6768 742d 6d65 7461 2d64 6966 662d 7261  ght-meta-diff-ra
-00035140: 6e67 6529 3b2d 2d73 796e 7461 782d 6869  nge);--syntax-hi
-00035150: 6768 6c69 6768 742d 6267 3a76 6172 282d  ghlight-bg:var(-
-00035160: 2d73 796e 7461 782d 6c69 6768 742d 6869  -syntax-light-hi
-00035170: 6768 6c69 6768 742d 6267 293b 2d2d 7379  ghlight-bg);--sy
-00035180: 6e74 6178 2d73 7065 6369 616c 2d62 673a  ntax-special-bg:
-00035190: 7661 7228 2d2d 7379 6e74 6178 2d6c 6967  var(--syntax-lig
-000351a0: 6874 2d73 7065 6369 616c 2d62 6729 7d2e  ht-special-bg)}.
-000351b0: 7379 2d6c 7369 6465 7b2d 2d68 6569 6768  sy-lside{--heigh
-000351c0: 743a 3432 7078 7d2e 7379 2d6c 7369 6465  t:42px}.sy-lside
-000351d0: 2d62 6f74 746f 6d7b 706f 7369 7469 6f6e  -bottom{position
-000351e0: 3a73 7469 636b 793b 626f 7474 6f6d 3a30  :sticky;bottom:0
-000351f0: 3b70 6164 6469 6e67 3a30 3b62 6f72 6465  ;padding:0;borde
-00035200: 722d 746f 703a 3170 7820 736f 6c69 6420  r-top:1px solid 
-00035210: 7661 7228 2d2d 7379 2d63 2d64 6976 6964  var(--sy-c-divid
-00035220: 6572 293b 6261 636b 6772 6f75 6e64 2d63  er);background-c
-00035230: 6f6c 6f72 3a76 6172 282d 2d73 792d 632d  olor:var(--sy-c-
-00035240: 6261 636b 6772 6f75 6e64 293b 2d2d 7477  background);--tw
-00035250: 2d73 6861 646f 773a 3020 2d31 3270 7820  -shadow:0 -12px 
-00035260: 3136 7078 2076 6172 282d 2d73 792d 632d  16px var(--sy-c-
-00035270: 6261 636b 6772 6f75 6e64 293b 626f 782d  background);box-
-00035280: 7368 6164 6f77 3a76 6172 282d 2d74 772d  shadow:var(--tw-
-00035290: 7269 6e67 2d6f 6666 7365 742d 7368 6164  ring-offset-shad
-000352a0: 6f77 2c30 2030 2023 3030 3030 292c 7661  ow,0 0 #0000),va
-000352b0: 7228 2d2d 7477 2d72 696e 672d 7368 6164  r(--tw-ring-shad
-000352c0: 6f77 2c30 2030 2023 3030 3030 292c 7661  ow,0 0 #0000),va
-000352d0: 7228 2d2d 7477 2d73 6861 646f 7729 7d2e  r(--tw-shadow)}.
-000352e0: 7379 2d6c 7369 6465 202e 7273 742d 7665  sy-lside .rst-ve
-000352f0: 7273 696f 6e73 7b70 6f73 6974 696f 6e3a  rsions{position:
-00035300: 7374 6174 6963 3b77 6964 7468 3a31 3030  static;width:100
-00035310: 253b 6261 636b 6772 6f75 6e64 2d63 6f6c  %;background-col
-00035320: 6f72 3a76 6172 282d 2d73 792d 632d 7375  or:var(--sy-c-su
-00035330: 7266 6163 6529 3b66 6f6e 742d 6661 6d69  rface);font-fami
-00035340: 6c79 3a76 6172 282d 2d73 792d 662d 7465  ly:var(--sy-f-te
-00035350: 7874 297d 2e73 792d 6c73 6964 6520 2e72  xt)}.sy-lside .r
-00035360: 7374 2d76 6572 7369 6f6e 7320 617b 636f  st-versions a{co
-00035370: 6c6f 723a 7661 7228 2d2d 7379 2d63 2d6c  lor:var(--sy-c-l
-00035380: 696e 6b29 7d2e 7379 2d6c 7369 6465 202e  ink)}.sy-lside .
-00035390: 7273 742d 7665 7273 696f 6e73 2061 3a68  rst-versions a:h
-000353a0: 6f76 6572 7b63 6f6c 6f72 3a76 6172 282d  over{color:var(-
-000353b0: 2d73 792d 632d 6c69 6e6b 2d68 6f76 6572  -sy-c-link-hover
-000353c0: 297d 2e73 792d 6c73 6964 6520 2e72 7374  )}.sy-lside .rst
-000353d0: 2d76 6572 7369 6f6e 7320 2e72 7374 2d63  -versions .rst-c
-000353e0: 7572 7265 6e74 2d76 6572 7369 6f6e 7b62  urrent-version{b
-000353f0: 6163 6b67 726f 756e 642d 636f 6c6f 723a  ackground-color:
-00035400: 7661 7228 2d2d 7379 2d63 2d62 6163 6b67  var(--sy-c-backg
-00035410: 726f 756e 6429 3b63 6f6c 6f72 3a76 6172  round);color:var
-00035420: 282d 2d73 792d 632d 7465 7874 293b 7061  (--sy-c-text);pa
-00035430: 6464 696e 673a 3020 3172 656d 3b68 6569  dding:0 1rem;hei
-00035440: 6768 743a 7661 7228 2d2d 6865 6967 6874  ght:var(--height
-00035450: 293b 6c69 6e65 2d68 6569 6768 743a 7661  );line-height:va
-00035460: 7228 2d2d 6865 6967 6874 297d 2e73 792d  r(--height)}.sy-
-00035470: 6c73 6964 6520 2e72 7374 2d76 6572 7369  lside .rst-versi
-00035480: 6f6e 732e 7273 742d 6261 6467 6520 2e72  ons.rst-badge .r
-00035490: 7374 2d63 7572 7265 6e74 2d76 6572 7369  st-current-versi
-000354a0: 6f6e 7b74 6578 742d 616c 6967 6e3a 6c65  on{text-align:le
-000354b0: 6674 3b66 6f6e 742d 7369 7a65 3a2e 3934  ft;font-size:.94
-000354c0: 7265 6d3b 7061 6464 696e 673a 3020 3172  rem;padding:0 1r
-000354d0: 656d 3b68 6569 6768 743a 7661 7228 2d2d  em;height:var(--
-000354e0: 6865 6967 6874 293b 6c69 6e65 2d68 6569  height);line-hei
-000354f0: 6768 743a 7661 7228 2d2d 6865 6967 6874  ght:var(--height
-00035500: 297d 2e73 792d 6c73 6964 6520 2e72 7374  )}.sy-lside .rst
-00035510: 2d76 6572 7369 6f6e 7320 2e72 7374 2d63  -versions .rst-c
-00035520: 7572 7265 6e74 2d76 6572 7369 6f6e 202e  urrent-version .
-00035530: 6661 7b63 6f6c 6f72 3a76 6172 282d 2d73  fa{color:var(--s
-00035540: 792d 632d 7465 7874 297d 2e73 792d 6c73  y-c-text)}.sy-ls
-00035550: 6964 6520 2e72 7374 2d76 6572 7369 6f6e  ide .rst-version
-00035560: 732e 7273 742d 6261 6467 652e 7368 6966  s.rst-badge.shif
-00035570: 742d 7570 202e 7273 742d 6375 7272 656e  t-up .rst-curren
-00035580: 742d 7665 7273 696f 6e7b 7465 7874 2d61  t-version{text-a
-00035590: 6c69 676e 3a6c 6566 747d 2e73 792d 6c73  lign:left}.sy-ls
-000355a0: 6964 6520 2e72 7374 2d76 6572 7369 6f6e  ide .rst-version
-000355b0: 732e 7273 742d 6261 6467 652e 7368 6966  s.rst-badge.shif
-000355c0: 742d 7570 202e 7273 742d 6375 7272 656e  t-up .rst-curren
-000355d0: 742d 7665 7273 696f 6e20 2e66 612d 626f  t-version .fa-bo
-000355e0: 6f6b 7b66 6c6f 6174 3a6e 6f6e 657d 2e73  ok{float:none}.s
-000355f0: 792d 6c73 6964 6520 2e72 7374 2d6f 7468  y-lside .rst-oth
-00035600: 6572 2d76 6572 7369 6f6e 737b 666f 6e74  er-versions{font
-00035610: 2d73 697a 653a 2e38 3672 656d 3b62 6f72  -size:.86rem;bor
-00035620: 6465 722d 746f 703a 3170 7820 736f 6c69  der-top:1px soli
-00035630: 6420 7661 7228 2d2d 7379 2d63 2d64 6976  d var(--sy-c-div
-00035640: 6964 6572 297d 2e73 792d 6c73 6964 6520  ider)}.sy-lside 
-00035650: 2e72 7374 2d6f 7468 6572 2d76 6572 7369  .rst-other-versi
-00035660: 6f6e 7320 6474 7b66 6f6e 742d 7369 7a65  ons dt{font-size
-00035670: 3a2e 3638 7265 6d3b 666f 6e74 2d77 6569  :.68rem;font-wei
-00035680: 6768 743a 3530 303b 7061 6464 696e 673a  ght:500;padding:
-00035690: 3470 7820 3670 783b 636f 6c6f 723a 7661  4px 6px;color:va
-000356a0: 7228 2d2d 7379 2d63 2d6c 6967 6874 297d  r(--sy-c-light)}
-000356b0: 2e73 792d 6c73 6964 6520 2e72 7374 2d76  .sy-lside .rst-v
-000356c0: 6572 7369 6f6e 7320 2e72 7374 2d6f 7468  ersions .rst-oth
-000356d0: 6572 2d76 6572 7369 6f6e 7320 6464 2061  er-versions dd a
-000356e0: 7b63 6f6c 6f72 3a76 6172 282d 2d73 792d  {color:var(--sy-
-000356f0: 632d 7465 7874 297d 2e73 792d 6c73 6964  c-text)}.sy-lsid
-00035700: 6520 2e72 7374 2d76 6572 7369 6f6e 7320  e .rst-versions 
-00035710: 2e72 7374 2d6f 7468 6572 2d76 6572 7369  .rst-other-versi
-00035720: 6f6e 7320 6464 2061 3a68 6f76 6572 7b74  ons dd a:hover{t
-00035730: 6578 742d 6465 636f 7261 7469 6f6e 3a75  ext-decoration:u
-00035740: 6e64 6572 6c69 6e65 3b63 6f6c 6f72 3a76  nderline;color:v
-00035750: 6172 282d 2d73 792d 632d 6c69 6e6b 2d68  ar(--sy-c-link-h
-00035760: 6f76 6572 297d 2e73 792d 6c73 6964 6520  over)}.sy-lside 
-00035770: 2e72 7374 2d76 6572 7369 6f6e 7320 696e  .rst-versions in
-00035780: 7075 747b 7769 6474 683a 3130 3025 3b70  put{width:100%;p
-00035790: 6164 6469 6e67 3a36 7078 2031 3270 783b  adding:6px 12px;
-000357a0: 666f 6e74 2d73 697a 653a 2e39 3272 656d  font-size:.92rem
-000357b0: 3b66 6f6e 742d 6661 6d69 6c79 3a76 6172  ;font-family:var
-000357c0: 282d 2d73 792d 662d 7465 7874 293b 626f  (--sy-f-text);bo
-000357d0: 7264 6572 2d72 6164 6975 733a 3670 783b  rder-radius:6px;
-000357e0: 6f75 746c 696e 653a 303b 6261 636b 6772  outline:0;backgr
-000357f0: 6f75 6e64 3a76 6172 282d 2d73 792d 632d  ound:var(--sy-c-
-00035800: 6261 636b 6772 6f75 6e64 293b 626f 7264  background);bord
-00035810: 6572 3a31 7078 2073 6f6c 6964 2076 6172  er:1px solid var
-00035820: 282d 2d73 792d 632d 626f 7264 6572 297d  (--sy-c-border)}
-00035830: 2e73 792d 6c73 6964 6520 2e72 7374 2d76  .sy-lside .rst-v
-00035840: 6572 7369 6f6e 7320 2e72 7374 2d6f 7468  ersions .rst-oth
-00035850: 6572 2d76 6572 7369 6f6e 7320 6872 7b62  er-versions hr{b
-00035860: 6f72 6465 722d 636f 6c6f 723a 7661 7228  order-color:var(
-00035870: 2d2d 7379 2d63 2d64 6976 6964 6572 297d  --sy-c-divider)}
-00035880: 406d 6564 6961 2028 6d69 6e2d 7769 6474  @media (min-widt
-00035890: 683a 3930 7265 6d29 7b2e 7379 2d6c 7369  h:90rem){.sy-lsi
-000358a0: 6465 202e 7273 742d 7665 7273 696f 6e73  de .rst-versions
-000358b0: 7b62 6163 6b67 726f 756e 643a 7661 7228  {background:var(
-000358c0: 2d2d 7379 2d63 2d62 6163 6b67 726f 756e  --sy-c-backgroun
-000358d0: 6429 7d7d 2e79 7565 2062 7574 746f 6e2e  d)}}.yue button.
-000358e0: 636f 7079 6274 6e7b 616c 6967 6e2d 6974  copybtn{align-it
-000358f0: 656d 733a 6365 6e74 6572 3b6a 7573 7469  ems:center;justi
-00035900: 6679 2d63 6f6e 7465 6e74 3a63 656e 7465  fy-content:cente
-00035910: 723b 6261 636b 6772 6f75 6e64 2d63 6f6c  r;background-col
-00035920: 6f72 3a69 6e69 7469 616c 3b62 6f72 6465  or:initial;borde
-00035930: 723a 6e6f 6e65 3b63 6f6c 6f72 3a76 6172  r:none;color:var
-00035940: 282d 2d73 796e 7461 782d 7465 7874 297d  (--syntax-text)}
-00035950: 2e79 7565 2062 7574 746f 6e2e 636f 7079  .yue button.copy
-00035960: 6274 6e3e 7376 677b 7769 6474 683a 312e  btn>svg{width:1.
-00035970: 3472 656d 3b68 6569 6768 743a 312e 3472  4rem;height:1.4r
-00035980: 656d 7d2e 7975 6520 6275 7474 6f6e 2e63  em}.yue button.c
-00035990: 6f70 7962 746e 3a68 6f76 6572 7b63 6f6c  opybtn:hover{col
-000359a0: 6f72 3a76 6172 282d 2d73 796e 7461 782d  or:var(--syntax-
-000359b0: 6d65 7461 297d 2e79 7565 202e 6869 6768  meta)}.yue .high
-000359c0: 6c69 6768 7420 6275 7474 6f6e 2e63 6f70  light button.cop
-000359d0: 7962 746e 3a68 6f76 6572 7b62 6163 6b67  ybtn:hover{backg
-000359e0: 726f 756e 642d 636f 6c6f 723a 696e 6974  round-color:init
-000359f0: 6961 6c7d 2e79 7565 2062 7574 746f 6e2e  ial}.yue button.
-00035a00: 636f 7079 6274 6e3a 6166 7465 727b 6261  copybtn:after{ba
-00035a10: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3a69  ckground-color:i
-00035a20: 6e69 7469 616c 3b63 6f6c 6f72 3a76 6172  nitial;color:var
-00035a30: 282d 2d73 796e 7461 782d 7465 7874 297d  (--syntax-text)}
-00035a40: 2e79 7565 2062 7574 746f 6e2e 636f 7079  .yue button.copy
-00035a50: 6274 6e2e 7375 6363 6573 737b 626f 7264  btn.success{bord
-00035a60: 6572 2d63 6f6c 6f72 3a76 6172 282d 2d67  er-color:var(--g
-00035a70: 7265 656e 2d61 3130 293b 636f 6c6f 723a  reen-a10);color:
-00035a80: 7661 7228 2d2d 6772 6565 6e2d 6131 3029  var(--green-a10)
-00035a90: 7d2e 7975 6520 6275 7474 6f6e 2e63 6f70  }.yue button.cop
-00035aa0: 7962 746e 2e73 7563 6365 7373 3a61 6674  ybtn.success:aft
-00035ab0: 6572 7b63 6f6c 6f72 3a76 6172 282d 2d67  er{color:var(--g
-00035ac0: 7265 656e 2d61 3130 297d 2e79 7565 7b2d  reen-a10)}.yue{-
-00035ad0: 2d73 642d 636f 6c6f 722d 7072 696d 6172  -sd-color-primar
-00035ae0: 793a 7661 7228 2d2d 6163 6365 6e74 2d61  y:var(--accent-a
-00035af0: 3131 293b 2d2d 7364 2d63 6f6c 6f72 2d73  11);--sd-color-s
-00035b00: 6563 6f6e 6461 7279 3a76 6172 282d 2d67  econdary:var(--g
-00035b10: 6f6c 642d 6131 3129 3b2d 2d73 642d 636f  old-a11);--sd-co
-00035b20: 6c6f 722d 7375 6363 6573 733a 7661 7228  lor-success:var(
-00035b30: 2d2d 6772 6565 6e2d 6131 3129 3b2d 2d73  --green-a11);--s
-00035b40: 642d 636f 6c6f 722d 696e 666f 3a76 6172  d-color-info:var
-00035b50: 282d 2d62 6c75 652d 6131 3129 3b2d 2d73  (--blue-a11);--s
-00035b60: 642d 636f 6c6f 722d 7761 726e 696e 673a  d-color-warning:
-00035b70: 7661 7228 2d2d 6f72 616e 6765 2d61 3131  var(--orange-a11
-00035b80: 293b 2d2d 7364 2d63 6f6c 6f72 2d64 616e  );--sd-color-dan
-00035b90: 6765 723a 7661 7228 2d2d 7265 642d 6131  ger:var(--red-a1
-00035ba0: 3129 3b2d 2d73 642d 636f 6c6f 722d 6c69  1);--sd-color-li
-00035bb0: 6768 743a 7661 7228 2d2d 7361 6e64 2d61  ght:var(--sand-a
-00035bc0: 3229 3b2d 2d73 642d 636f 6c6f 722d 6d75  2);--sd-color-mu
-00035bd0: 7465 643a 7661 7228 2d2d 6772 6179 2d38  ted:var(--gray-8
-00035be0: 293b 2d2d 7364 2d63 6f6c 6f72 2d64 6172  );--sd-color-dar
-00035bf0: 6b3a 2332 3132 3132 323b 2d2d 7364 2d63  k:#212122;--sd-c
-00035c00: 6f6c 6f72 2d62 6c61 636b 3a23 3030 303b  olor-black:#000;
-00035c10: 2d2d 7364 2d63 6f6c 6f72 2d77 6869 7465  --sd-color-white
-00035c20: 3a23 6666 663b 2d2d 7364 2d63 6f6c 6f72  :#fff;--sd-color
-00035c30: 2d70 7269 6d61 7279 2d68 6967 686c 6967  -primary-highlig
-00035c40: 6874 3a76 6172 282d 2d61 6363 656e 742d  ht:var(--accent-
-00035c50: 6138 293b 2d2d 7364 2d63 6f6c 6f72 2d73  a8);--sd-color-s
-00035c60: 6563 6f6e 6461 7279 2d68 6967 686c 6967  econdary-highlig
-00035c70: 6874 3a76 6172 282d 2d67 6f6c 642d 6138  ht:var(--gold-a8
-00035c80: 293b 2d2d 7364 2d63 6f6c 6f72 2d73 7563  );--sd-color-suc
-00035c90: 6365 7373 2d68 6967 686c 6967 6874 3a76  cess-highlight:v
-00035ca0: 6172 282d 2d67 7265 656e 2d61 3829 3b2d  ar(--green-a8);-
-00035cb0: 2d73 642d 636f 6c6f 722d 696e 666f 2d68  -sd-color-info-h
-00035cc0: 6967 686c 6967 6874 3a76 6172 282d 2d62  ighlight:var(--b
-00035cd0: 6c75 652d 6138 293b 2d2d 7364 2d63 6f6c  lue-a8);--sd-col
-00035ce0: 6f72 2d77 6172 6e69 6e67 2d68 6967 686c  or-warning-highl
-00035cf0: 6967 6874 3a76 6172 282d 2d6f 7261 6e67  ight:var(--orang
-00035d00: 652d 6138 293b 2d2d 7364 2d63 6f6c 6f72  e-a8);--sd-color
-00035d10: 2d64 616e 6765 722d 6869 6768 6c69 6768  -danger-highligh
-00035d20: 743a 7661 7228 2d2d 7265 642d 6138 293b  t:var(--red-a8);
-00035d30: 2d2d 7364 2d63 6f6c 6f72 2d6c 6967 6874  --sd-color-light
-00035d40: 2d68 6967 686c 6967 6874 3a76 6172 282d  -highlight:var(-
-00035d50: 2d67 7261 792d 3429 3b2d 2d73 642d 636f  -gray-4);--sd-co
-00035d60: 6c6f 722d 6d75 7465 642d 6869 6768 6c69  lor-muted-highli
-00035d70: 6768 743a 7661 7228 2d2d 6772 6179 2d31  ght:var(--gray-1
-00035d80: 3129 3b2d 2d73 642d 636f 6c6f 722d 6461  1);--sd-color-da
-00035d90: 726b 2d68 6967 686c 6967 6874 3a23 3132  rk-highlight:#12
-00035da0: 3132 3131 3b2d 2d73 642d 636f 6c6f 722d  1211;--sd-color-
-00035db0: 626c 6163 6b2d 6869 6768 6c69 6768 743a  black-highlight:
-00035dc0: 2330 3030 3b2d 2d73 642d 636f 6c6f 722d  #000;--sd-color-
-00035dd0: 7768 6974 652d 6869 6768 6c69 6768 743a  white-highlight:
-00035de0: 2364 3964 3964 393b 2d2d 7364 2d63 6f6c  #d9d9d9;--sd-col
-00035df0: 6f72 2d70 7269 6d61 7279 2d74 6578 743a  or-primary-text:
-00035e00: 7661 7228 2d2d 6163 6365 6e74 2d39 2d63  var(--accent-9-c
-00035e10: 6f6e 7472 6173 7429 3b2d 2d73 642d 636f  ontrast);--sd-co
-00035e20: 6c6f 722d 7365 636f 6e64 6172 792d 7465  lor-secondary-te
-00035e30: 7874 3a76 6172 282d 2d67 6f6c 642d 392d  xt:var(--gold-9-
-00035e40: 636f 6e74 7261 7374 293b 2d2d 7364 2d63  contrast);--sd-c
-00035e50: 6f6c 6f72 2d73 7563 6365 7373 2d74 6578  olor-success-tex
-00035e60: 743a 7661 7228 2d2d 6772 6565 6e2d 392d  t:var(--green-9-
-00035e70: 636f 6e74 7261 7374 293b 2d2d 7364 2d63  contrast);--sd-c
-00035e80: 6f6c 6f72 2d69 6e66 6f2d 7465 7874 3a76  olor-info-text:v
-00035e90: 6172 282d 2d62 6c75 652d 392d 636f 6e74  ar(--blue-9-cont
-00035ea0: 7261 7374 293b 2d2d 7364 2d63 6f6c 6f72  rast);--sd-color
-00035eb0: 2d77 6172 6e69 6e67 2d74 6578 743a 7661  -warning-text:va
-00035ec0: 7228 2d2d 6f72 616e 6765 2d39 2d63 6f6e  r(--orange-9-con
-00035ed0: 7472 6173 7429 3b2d 2d73 642d 636f 6c6f  trast);--sd-colo
-00035ee0: 722d 6461 6e67 6572 2d74 6578 743a 7661  r-danger-text:va
-00035ef0: 7228 2d2d 7265 642d 392d 636f 6e74 7261  r(--red-9-contra
-00035f00: 7374 293b 2d2d 7364 2d63 6f6c 6f72 2d6c  st);--sd-color-l
-00035f10: 6967 6874 2d74 6578 743a 7661 7228 2d2d  ight-text:var(--
-00035f20: 7379 2d63 2d74 6578 7429 3b2d 2d73 642d  sy-c-text);--sd-
-00035f30: 636f 6c6f 722d 6d75 7465 642d 7465 7874  color-muted-text
-00035f40: 3a23 6666 663b 2d2d 7364 2d63 6f6c 6f72  :#fff;--sd-color
-00035f50: 2d64 6172 6b2d 7465 7874 3a23 6666 663b  -dark-text:#fff;
-00035f60: 2d2d 7364 2d63 6f6c 6f72 2d62 6c61 636b  --sd-color-black
-00035f70: 2d74 6578 743a 2366 6666 3b2d 2d73 642d  -text:#fff;--sd-
-00035f80: 636f 6c6f 722d 7768 6974 652d 7465 7874  color-white-text
-00035f90: 3a23 3231 3235 3239 3b2d 2d73 642d 636f  :#212529;--sd-co
-00035fa0: 6c6f 722d 7368 6164 6f77 3a76 6172 282d  lor-shadow:var(-
-00035fb0: 2d67 7261 792d 3129 3b2d 2d73 642d 636f  -gray-1);--sd-co
-00035fc0: 6c6f 722d 6361 7264 2d62 6f72 6465 723a  lor-card-border:
-00035fd0: 7661 7228 2d2d 7379 2d63 2d62 6f72 6465  var(--sy-c-borde
-00035fe0: 7229 3b2d 2d73 642d 636f 6c6f 722d 6361  r);--sd-color-ca
-00035ff0: 7264 2d62 6f72 6465 722d 686f 7665 723a  rd-border-hover:
-00036000: 7661 7228 2d2d 6163 6365 6e74 2d61 3929  var(--accent-a9)
-00036010: 3b2d 2d73 642d 636f 6c6f 722d 7461 6273  ;--sd-color-tabs
-00036020: 2d6c 6162 656c 2d69 6e61 6374 6976 653a  -label-inactive:
-00036030: 7661 7228 2d2d 7379 2d63 2d62 6f6c 6429  var(--sy-c-bold)
-00036040: 3b2d 2d73 642d 636f 6c6f 722d 7461 6273  ;--sd-color-tabs
-00036050: 2d6c 6162 656c 2d61 6374 6976 653a 7661  -label-active:va
-00036060: 7228 2d2d 7364 2d63 6f6c 6f72 2d70 7269  r(--sd-color-pri
-00036070: 6d61 7279 293b 2d2d 7364 2d63 6f6c 6f72  mary);--sd-color
-00036080: 2d74 6162 732d 756e 6465 726c 696e 652d  -tabs-underline-
-00036090: 6163 7469 7665 3a76 6172 282d 2d73 642d  active:var(--sd-
-000360a0: 636f 6c6f 722d 7072 696d 6172 7929 3b2d  color-primary);-
-000360b0: 2d73 642d 636f 6c6f 722d 7461 6273 2d6c  -sd-color-tabs-l
-000360c0: 6162 656c 2d68 6f76 6572 3a76 6172 282d  abel-hover:var(-
-000360d0: 2d61 6363 656e 742d 3929 3b2d 2d73 642d  -accent-9);--sd-
-000360e0: 636f 6c6f 722d 7461 6273 2d75 6e64 6572  color-tabs-under
-000360f0: 6c69 6e65 2d68 6f76 6572 3a76 6172 282d  line-hover:var(-
-00036100: 2d61 6363 656e 742d 3929 7d2e 7975 6520  -accent-9)}.yue 
-00036110: 2e73 7572 6661 6365 7b2d 2d73 642d 636f  .surface{--sd-co
-00036120: 6c6f 722d 6361 7264 2d74 6578 743a 7661  lor-card-text:va
-00036130: 7228 2d2d 7379 2d63 2d6c 6967 6874 293b  r(--sy-c-light);
-00036140: 2d2d 7364 2d63 6f6c 6f72 2d63 6172 642d  --sd-color-card-
-00036150: 626f 7264 6572 3a23 3030 3030 3b2d 2d73  border:#0000;--s
-00036160: 642d 636f 6c6f 722d 6361 7264 2d62 6163  d-color-card-bac
-00036170: 6b67 726f 756e 643a 7661 7228 2d2d 7379  kground:var(--sy
-00036180: 2d63 2d73 7572 6661 6365 297d 2e79 7565  -c-surface)}.yue
-00036190: 2061 2e73 642d 6261 6467 652c 2e79 7565   a.sd-badge,.yue
-000361a0: 2061 2e73 642d 6261 6467 653a 686f 7665   a.sd-badge:hove
-000361b0: 727b 626f 7264 6572 2d62 6f74 746f 6d3a  r{border-bottom:
-000361c0: 307d 2e79 7565 202e 7364 2d62 6164 6765  0}.yue .sd-badge
-000361d0: 7b66 6f6e 742d 7765 6967 6874 3a36 3030  {font-weight:600
-000361e0: 3b62 6f72 6465 722d 7261 6469 7573 3a33  ;border-radius:3
-000361f0: 7078 7d2e 7975 6520 2e73 642d 6274 6e7b  px}.yue .sd-btn{
-00036200: 626f 7264 6572 2d63 6f6c 6f72 3a76 6172  border-color:var
-00036210: 282d 2d73 792d 632d 626f 7264 6572 297d  (--sy-c-border)}
-00036220: 2e79 7565 202e 7364 2d74 6162 2d73 6574  .yue .sd-tab-set
-00036230: 3e6c 6162 656c 7b70 6164 6469 6e67 3a31  >label{padding:1
-00036240: 7265 6d20 2e32 3572 656d 202e 3572 656d  rem .25rem .5rem
-00036250: 3b66 6f6e 742d 7369 7a65 3a2e 3834 7265  ;font-size:.84re
-00036260: 6d3b 666f 6e74 2d77 6569 6768 743a 3530  m;font-weight:50
-00036270: 307d 2e79 7565 202e 7364 2d74 6162 2d73  0}.yue .sd-tab-s
-00036280: 6574 3e6c 6162 656c 7e6c 6162 656c 7b6d  et>label~label{m
-00036290: 6172 6769 6e2d 6c65 6674 3a31 7265 6d7d  argin-left:1rem}
-000362a0: 2e79 7565 202e 7364 2d74 6162 2d63 6f6e  .yue .sd-tab-con
-000362b0: 7465 6e74 7b70 6164 6469 6e67 3a30 3b62  tent{padding:0;b
-000362c0: 6f78 2d73 6861 646f 773a 3020 2d2e 3036  ox-shadow:0 -.06
-000362d0: 3235 7265 6d20 7661 7228 2d2d 7379 2d63  25rem var(--sy-c
-000362e0: 2d64 6976 6964 6572 297d 2e79 7565 202e  -divider)}.yue .
-000362f0: 7364 2d74 6162 2d63 6f6e 7465 6e74 202e  sd-tab-content .
-00036300: 636f 6465 2d62 6c6f 636b 2d63 6170 7469  code-block-capti
-00036310: 6f6e 2c2e 7975 6520 2e73 642d 7461 622d  on,.yue .sd-tab-
-00036320: 636f 6e74 656e 7420 2e68 6967 686c 6967  content .highlig
-00036330: 6874 2070 7265 7b62 6f72 6465 722d 7261  ht pre{border-ra
-00036340: 6469 7573 3a30 7d2e 7975 6520 2e73 642d  dius:0}.yue .sd-
-00036350: 6361 7264 2d74 6974 6c65 7b63 6f6c 6f72  card-title{color
-00036360: 3a76 6172 282d 2d73 792d 632d 7465 7874  :var(--sy-c-text
-00036370: 297d 2e79 7565 202e 7364 2d63 6172 642d  )}.yue .sd-card-
-00036380: 7469 746c 653e 7376 677b 706f 7369 7469  title>svg{positi
-00036390: 6f6e 3a72 656c 6174 6976 653b 746f 703a  on:relative;top:
-000363a0: 2d31 7078 3b6d 6172 6769 6e2d 7269 6768  -1px;margin-righ
-000363b0: 743a 2e32 3572 656d 7d2e 7975 6520 2e73  t:.25rem}.yue .s
-000363c0: 642d 6361 7264 2d68 6f76 6572 3a68 6f76  d-card-hover:hov
-000363d0: 6572 7b74 7261 6e73 666f 726d 3a73 6361  er{transform:sca
-000363e0: 6c65 2831 297d 2e79 7565 202e 7364 2d63  le(1)}.yue .sd-c
-000363f0: 6172 642d 686f 7665 723a 686f 7665 7220  ard-hover:hover 
-00036400: 2e73 642d 6361 7264 2d74 6974 6c65 7b63  .sd-card-title{c
-00036410: 6f6c 6f72 3a76 6172 282d 2d73 792d 632d  olor:var(--sy-c-
-00036420: 6c69 6e6b 2d68 6f76 6572 297d 2e79 7565  link-hover)}.yue
-00036430: 202e 7364 2d63 6172 6420 612c 2e79 7565   .sd-card a,.yue
-00036440: 202e 7364 2d63 6172 6420 613a 686f 7665   .sd-card a:hove
-00036450: 727b 626f 7264 6572 2d62 6f74 746f 6d3a  r{border-bottom:
-00036460: 307d 2e79 7565 202e 7375 7266 6163 6520  0}.yue .surface 
-00036470: 2e73 642d 6361 7264 2d62 6f64 792c 2e79  .sd-card-body,.y
-00036480: 7565 202e 7375 7266 6163 6520 2e73 642d  ue .surface .sd-
-00036490: 6361 7264 2d66 6f6f 7465 722c 2e79 7565  card-footer,.yue
-000364a0: 202e 7375 7266 6163 6520 2e73 642d 6361   .surface .sd-ca
-000364b0: 7264 2d68 6561 6465 727b 7061 6464 696e  rd-header{paddin
-000364c0: 672d 6c65 6674 3a31 2e35 7265 6d3b 7061  g-left:1.5rem;pa
-000364d0: 6464 696e 672d 7269 6768 743a 312e 3572  dding-right:1.5r
-000364e0: 656d 7d2e 7975 6520 2e73 7572 6661 6365  em}.yue .surface
-000364f0: 202e 7364 2d63 6172 642d 666f 6f74 6572   .sd-card-footer
-00036500: 2c2e 7975 6520 2e73 7572 6661 6365 202e  ,.yue .surface .
-00036510: 7364 2d63 6172 642d 6865 6164 6572 7b62  sd-card-header{b
-00036520: 6f72 6465 722d 636f 6c6f 723a 7661 7228  order-color:var(
-00036530: 2d2d 7379 2d63 2d62 6f72 6465 7229 7d40  --sy-c-border)}@
-00036540: 6d65 6469 6120 2870 7269 6e74 297b 2e79  media (print){.y
-00036550: 7565 202e 7364 2d63 6172 647b 7061 6765  ue .sd-card{page
-00036560: 2d62 7265 616b 2d69 6e73 6964 653a 6176  -break-inside:av
-00036570: 6f69 647d 7d2e 7975 6520 612e 7364 2d74  oid}}.yue a.sd-t
-00036580: 6578 742d 7772 6170 3a68 6f76 6572 7b62  ext-wrap:hover{b
-00036590: 6f72 6465 722d 626f 7474 6f6d 2d77 6964  order-bottom-wid
-000365a0: 7468 3a31 7078 7d2e 7370 6869 6e78 2d74  th:1px}.sphinx-t
-000365b0: 6162 7320 5b72 6f6c 653d 7461 626c 6973  abs [role=tablis
-000365c0: 745d 7b62 6f72 6465 722d 636f 6c6f 723a  t]{border-color:
-000365d0: 7661 7228 2d2d 7379 2d63 2d64 6976 6964  var(--sy-c-divid
-000365e0: 6572 297d 2e79 7565 202e 7370 6869 6e78  er)}.yue .sphinx
-000365f0: 2d74 6162 732d 7461 627b 636f 6c6f 723a  -tabs-tab{color:
-00036600: 7661 7228 2d2d 7379 2d63 2d74 6578 7429  var(--sy-c-text)
-00036610: 3b6c 696e 652d 6865 6967 6874 3a69 6e68  ;line-height:inh
-00036620: 6572 6974 3b70 6164 6469 6e67 3a31 7265  erit;padding:1re
-00036630: 6d20 2e32 3572 656d 202e 3572 656d 3b66  m .25rem .5rem;f
-00036640: 6f6e 742d 7369 7a65 3a2e 3834 7265 6d3b  ont-size:.84rem;
-00036650: 666f 6e74 2d77 6569 6768 743a 3530 303b  font-weight:500;
-00036660: 626f 7264 6572 3a6e 6f6e 653b 626f 7264  border:none;bord
-00036670: 6572 2d62 6f74 746f 6d3a 2e31 3235 7265  er-bottom:.125re
-00036680: 6d20 736f 6c69 6420 2330 3030 307d 2e79  m solid #0000}.y
-00036690: 7565 202e 7370 6869 6e78 2d74 6162 732d  ue .sphinx-tabs-
-000366a0: 7461 623a 686f 7665 727b 636f 6c6f 723a  tab:hover{color:
-000366b0: 7661 7228 2d2d 7364 2d63 6f6c 6f72 2d74  var(--sd-color-t
-000366c0: 6162 732d 6c61 6265 6c2d 686f 7665 7229  abs-label-hover)
-000366d0: 3b62 6f72 6465 722d 636f 6c6f 723a 7661  ;border-color:va
-000366e0: 7228 2d2d 7364 2d63 6f6c 6f72 2d74 6162  r(--sd-color-tab
-000366f0: 732d 756e 6465 726c 696e 652d 686f 7665  s-underline-hove
-00036700: 7229 7d2e 7975 6520 2e73 7068 696e 782d  r)}.yue .sphinx-
-00036710: 7461 6273 2d74 6162 5b61 7269 612d 7365  tabs-tab[aria-se
-00036720: 6c65 6374 6564 3d74 7275 655d 7b62 6f72  lected=true]{bor
-00036730: 6465 723a 6e6f 6e65 3b62 6f72 6465 722d  der:none;border-
-00036740: 626f 7474 6f6d 3a2e 3132 3572 656d 2073  bottom:.125rem s
-00036750: 6f6c 6964 2076 6172 282d 2d73 642d 636f  olid var(--sd-co
-00036760: 6c6f 722d 7461 6273 2d75 6e64 6572 6c69  lor-tabs-underli
-00036770: 6e65 2d61 6374 6976 6529 3b63 6f6c 6f72  ne-active);color
-00036780: 3a76 6172 282d 2d73 642d 636f 6c6f 722d  :var(--sd-color-
-00036790: 7461 6273 2d6c 6162 656c 2d61 6374 6976  tabs-label-activ
-000367a0: 6529 3b62 6163 6b67 726f 756e 642d 636f  e);background-co
-000367b0: 6c6f 723a 696e 6974 6961 6c7d 2e79 7565  lor:initial}.yue
-000367c0: 202e 7370 6869 6e78 2d74 6162 732d 7461   .sphinx-tabs-ta
-000367d0: 622b 2e73 7068 696e 782d 7461 6273 2d74  b+.sphinx-tabs-t
-000367e0: 6162 7b6d 6172 6769 6e2d 6c65 6674 3a31  ab{margin-left:1
-000367f0: 7265 6d7d 2e79 7565 202e 7370 6869 6e78  rem}.yue .sphinx
-00036800: 2d74 6162 732d 7061 6e65 6c7b 626f 7264  -tabs-panel{bord
-00036810: 6572 3a6e 6f6e 653b 7061 6464 696e 673a  er:none;padding:
-00036820: 303b 6d61 7267 696e 3a30 3b62 6f72 6465  0;margin:0;borde
-00036830: 722d 7261 6469 7573 3a30 3b62 6163 6b67  r-radius:0;backg
-00036840: 726f 756e 642d 636f 6c6f 723a 696e 6974  round-color:init
-00036850: 6961 6c7d 2e79 7565 202e 7370 6869 6e78  ial}.yue .sphinx
-00036860: 2d74 6162 732d 7061 6e65 6c2e 636f 6465  -tabs-panel.code
-00036870: 2d74 6162 7b70 6164 6469 6e67 3a30 7d2e  -tab{padding:0}.
-00036880: 7975 6520 2e73 7068 696e 782d 7461 6273  yue .sphinx-tabs
-00036890: 2d70 616e 656c 2e63 6f64 652d 7461 6220  -panel.code-tab 
-000368a0: 2e63 6f64 652d 626c 6f63 6b2d 6361 7074  .code-block-capt
-000368b0: 696f 6e2c 2e79 7565 202e 7370 6869 6e78  ion,.yue .sphinx
-000368c0: 2d74 6162 732d 7061 6e65 6c2e 636f 6465  -tabs-panel.code
-000368d0: 2d74 6162 202e 6869 6768 6c69 6768 7420  -tab .highlight 
-000368e0: 7072 657b 626f 7264 6572 2d72 6164 6975  pre{border-radiu
-000368f0: 733a 307d 2e79 7565 7b2d 2d6a 702d 7769  s:0}.yue{--jp-wi
-00036900: 6467 6574 732d 696e 7075 742d 626f 7264  dgets-input-bord
-00036910: 6572 2d63 6f6c 6f72 3a76 6172 282d 2d67  er-color:var(--g
-00036920: 7261 792d 3529 3b2d 2d6a 702d 7769 6467  ray-5);--jp-widg
-00036930: 6574 732d 696e 7075 742d 666f 6375 732d  ets-input-focus-
-00036940: 626f 7264 6572 2d63 6f6c 6f72 3a76 6172  border-color:var
-00036950: 282d 2d67 7261 792d 3829 3b2d 2d6a 702d  (--gray-8);--jp-
-00036960: 7769 6467 6574 732d 736c 6964 6572 2d61  widgets-slider-a
-00036970: 6374 6976 652d 6861 6e64 6c65 2d63 6f6c  ctive-handle-col
-00036980: 6f72 3a76 6172 282d 2d67 7261 792d 3429  or:var(--gray-4)
-00036990: 3b2d 2d6a 702d 7769 6467 6574 732d 736c  ;--jp-widgets-sl
-000369a0: 6964 6572 2d68 616e 646c 652d 626f 7264  ider-handle-bord
-000369b0: 6572 2d63 6f6c 6f72 3a76 6172 282d 2d73  er-color:var(--s
-000369c0: 792d 632d 626f 7264 6572 297d 2e79 7565  y-c-border)}.yue
-000369d0: 202e 6a75 7079 7465 725f 636f 6e74 6169   .jupyter_contai
-000369e0: 6e65 727b 6261 636b 6772 6f75 6e64 2d63  ner{background-c
-000369f0: 6f6c 6f72 3a76 6172 282d 2d73 792d 632d  olor:var(--sy-c-
-00036a00: 6261 636b 6772 6f75 6e64 293b 626f 7264  background);bord
-00036a10: 6572 3a33 7078 2073 6f6c 6964 2076 6172  er:3px solid var
-00036a20: 282d 2d73 792d 632d 626f 7264 6572 293b  (--sy-c-border);
-00036a30: 626f 7264 6572 2d72 6164 6975 733a 3670  border-radius:6p
-00036a40: 783b 6f76 6572 666c 6f77 3a68 6964 6465  x;overflow:hidde
-00036a50: 6e3b 626f 782d 7368 6164 6f77 3a6e 6f6e  n;box-shadow:non
-00036a60: 657d 2e64 6f63 756d 656e 7420 2e79 7565  e}.document .yue
-00036a70: 202e 6a75 7079 7465 725f 636f 6e74 6169   .jupyter_contai
-00036a80: 6e65 7220 6469 765b 636c 6173 735e 3d68  ner div[class^=h
-00036a90: 6967 686c 6967 6874 5d7b 7061 6464 696e  ighlight]{paddin
-00036aa0: 673a 307d 2e79 7565 202e 6a75 7079 7465  g:0}.yue .jupyte
-00036ab0: 725f 636f 6e74 6169 6e65 7220 6469 762e  r_container div.
-00036ac0: 6365 6c6c 5f69 6e70 7574 7b62 6163 6b67  cell_input{backg
-00036ad0: 726f 756e 642d 636f 6c6f 723a 7661 7228  round-color:var(
-00036ae0: 2d2d 7379 6e74 6178 2d70 7265 2d62 6729  --syntax-pre-bg)
-00036af0: 3b62 6f72 6465 723a 303b 626f 7264 6572  ;border:0;border
-00036b00: 2d72 6164 6975 733a 307d 2e79 7565 202e  -radius:0}.yue .
-00036b10: 6a75 7079 7465 725f 636f 6e74 6169 6e65  jupyter_containe
-00036b20: 7220 6469 762e 636f 6465 5f63 656c 6c20  r div.code_cell 
-00036b30: 7072 657b 7061 6464 696e 673a 307d 2e6a  pre{padding:0}.j
-00036b40: 7570 7974 6572 5f63 6f6e 7461 696e 6572  upyter_container
-00036b50: 2064 6976 2e63 656c 6c5f 6f75 7470 7574   div.cell_output
-00036b60: 202e 6f75 7470 7574 2c2e 6a75 7079 7465   .output,.jupyte
-00036b70: 725f 636f 6e74 6169 6e65 7220 6469 762e  r_container div.
-00036b80: 6365 6c6c 5f6f 7574 7075 7420 2e73 7464  cell_output .std
-00036b90: 6572 722c 2e6a 7570 7974 6572 5f63 6f6e  err,.jupyter_con
-00036ba0: 7461 696e 6572 2064 6976 2e63 656c 6c5f  tainer div.cell_
-00036bb0: 6f75 7470 7574 202e 7769 6467 6574 2d73  output .widget-s
-00036bc0: 7562 6172 6561 7b70 6164 6469 6e67 3a2e  ubarea{padding:.
-00036bd0: 3572 656d 7d2e 6a75 7079 7465 725f 636f  5rem}.jupyter_co
-00036be0: 6e74 6169 6e65 7220 6469 762e 6365 6c6c  ntainer div.cell
-00036bf0: 5f6f 7574 7075 7420 2e73 7464 6572 7220  _output .stderr 
-00036c00: 2e73 7464 6572 727b 7061 6464 696e 673a  .stderr{padding:
-00036c10: 307d 2e6a 7570 7974 6572 2d77 6964 6765  0}.jupyter-widge
-00036c20: 742d 6873 6c69 6465 7220 2e73 6c69 6465  t-hslider .slide
-00036c30: 722d 636f 6e74 6169 6e65 722c 2e77 6964  r-container,.wid
-00036c40: 6765 742d 6873 6c69 6465 7220 2e73 6c69  get-hslider .sli
-00036c50: 6465 722d 636f 6e74 6169 6e65 727b 6469  der-container{di
-00036c60: 7370 6c61 793a 666c 6578 3b61 6c69 676e  splay:flex;align
-00036c70: 2d69 7465 6d73 3a63 656e 7465 727d 2e6a  -items:center}.j
-00036c80: 7570 7974 6572 2d77 6964 6765 742d 736c  upyter-widget-sl
-00036c90: 6964 6572 202e 6e6f 5569 2d74 6172 6765  ider .noUi-targe
-00036ca0: 742c 2e77 6964 6765 742d 736c 6964 6572  t,.widget-slider
-00036cb0: 202e 6e6f 5569 2d74 6172 6765 747b 7769   .noUi-target{wi
-00036cc0: 6474 683a 3130 3025 7d2e 6a75 7079 7465  dth:100%}.jupyte
-00036cd0: 725f 636f 6e74 6169 6e65 7220 6469 762e  r_container div.
-00036ce0: 636f 6465 5f63 656c 6c20 2e68 6967 686c  code_cell .highl
-00036cf0: 6967 6874 3e70 7265 7b70 6164 6469 6e67  ight>pre{padding
-00036d00: 3a31 7265 6d7d 2e6a 7570 7974 6572 5f63  :1rem}.jupyter_c
-00036d10: 6f6e 7461 696e 6572 2064 6976 2e63 6f64  ontainer div.cod
-00036d20: 655f 6365 6c6c 202e 6869 6768 6c69 6768  e_cell .highligh
-00036d30: 7420 2e68 6c6c 7b6d 6172 6769 6e2d 6c65  t .hll{margin-le
-00036d40: 6674 3a2d 3172 656d 3b6d 6172 6769 6e2d  ft:-1rem;margin-
-00036d50: 7269 6768 743a 2d31 7265 6d3b 7061 6464  right:-1rem;padd
-00036d60: 696e 673a 3020 3172 656d 7d2e 6a75 7079  ing:0 1rem}.jupy
-00036d70: 7465 725f 636f 6e74 6169 6e65 7220 6469  ter_container di
-00036d80: 762e 636f 6465 5f63 656c 6c20 2e68 6967  v.code_cell .hig
-00036d90: 686c 6967 6874 202e 6c69 6e65 6e6f 737b  hlight .linenos{
-00036da0: 6d61 7267 696e 2d72 6967 6874 3a2e 3872  margin-right:.8r
-00036db0: 656d 7d2e 7975 6520 2e6a 7570 7974 6572  em}.yue .jupyter
-00036dc0: 5f63 6f6e 7461 696e 6572 202e 7374 6465  _container .stde
-00036dd0: 7272 7b63 6f6c 6f72 3a76 6172 282d 2d72  rr{color:var(--r
-00036de0: 6564 2d61 3131 293b 6261 636b 6772 6f75  ed-a11);backgrou
-00036df0: 6e64 2d63 6f6c 6f72 3a76 6172 282d 2d72  nd-color:var(--r
-00036e00: 6564 2d61 3329 7d2e 7975 6520 2e6a 7570  ed-a3)}.yue .jup
-00036e10: 7974 6572 5f63 6f6e 7461 696e 6572 202e  yter_container .
-00036e20: 7374 6465 7272 202e 7374 6465 7272 7b62  stderr .stderr{b
-00036e30: 6163 6b67 726f 756e 642d 636f 6c6f 723a  ackground-color:
-00036e40: 696e 6974 6961 6c7d 2e6e 6269 6e70 7574  initial}.nbinput
-00036e50: 202e 6869 6768 6c69 6768 747b 2d2d 7261   .highlight{--ra
-00036e60: 6469 7573 3a31 7078 7d2e 7975 6520 6469  dius:1px}.yue di
-00036e70: 762e 6e62 6c61 7374 2e63 6f6e 7461 696e  v.nblast.contain
-00036e80: 6572 7b70 6164 6469 6e67 2d74 6f70 3a35  er{padding-top:5
-00036e90: 7078 7d2e 7975 6520 6469 762e 6e62 696e  px}.yue div.nbin
-00036ea0: 7075 742e 636f 6e74 6169 6e65 7220 6469  put.container di
-00036eb0: 762e 696e 7075 745f 6172 6561 7b62 6f72  v.input_area{bor
-00036ec0: 6465 722d 636f 6c6f 723a 7661 7228 2d2d  der-color:var(--
-00036ed0: 7379 2d63 2d62 6f72 6465 7229 7d2e 7975  sy-c-border)}.yu
-00036ee0: 6520 6469 762e 6e62 6f75 7470 7574 2e63  e div.nboutput.c
-00036ef0: 6f6e 7461 696e 6572 2064 6976 2e6f 7574  ontainer div.out
-00036f00: 7075 745f 6172 6561 2e73 7464 6572 727b  put_area.stderr{
-00036f10: 636f 6c6f 723a 7661 7228 2d2d 7265 642d  color:var(--red-
-00036f20: 6131 3129 3b62 6163 6b67 726f 756e 642d  a11);background-
-00036f30: 636f 6c6f 723a 7661 7228 2d2d 7265 642d  color:var(--red-
-00036f40: 6133 297d 2e79 7565 2064 6976 2e6e 626f  a3)}.yue div.nbo
-00036f50: 7574 7075 742e 636f 6e74 6169 6e65 7220  utput.container 
-00036f60: 6469 762e 6f75 7470 7574 5f61 7265 613e  div.output_area>
-00036f70: 2e6d 6174 682d 7772 6170 7065 723e 6469  .math-wrapper>di
-00036f80: 762e 6d61 7468 7b70 6164 6469 6e67 2d74  v.math{padding-t
-00036f90: 6f70 3a30 7d2e 7975 6520 2e6a 702d 5265  op:0}.yue .jp-Re
-00036fa0: 6e64 6572 6564 4854 4d4c 436f 6d6d 6f6e  nderedHTMLCommon
-00036fb0: 2074 6865 6164 2c2e 7975 6520 6469 762e   thead,.yue div.
-00036fc0: 7265 6e64 6572 6564 5f68 746d 6c20 7468  rendered_html th
-00036fd0: 6561 647b 626f 7264 6572 2d63 6f6c 6f72  ead{border-color
-00036fe0: 3a76 6172 282d 2d73 792d 632d 626f 7264  :var(--sy-c-bord
-00036ff0: 6572 297d 2e79 7565 202e 6a70 2d52 656e  er)}.yue .jp-Ren
-00037000: 6465 7265 6448 544d 4c43 6f6d 6d6f 6e20  deredHTMLCommon 
-00037010: 7462 6f64 7920 7472 2c2e 7975 6520 6469  tbody tr,.yue di
-00037020: 762e 7265 6e64 6572 6564 5f68 746d 6c20  v.rendered_html 
-00037030: 7462 6f64 7920 7472 7b63 6f6c 6f72 3a76  tbody tr{color:v
-00037040: 6172 282d 2d73 792d 632d 7465 7874 297d  ar(--sy-c-text)}
-00037050: 2e79 7565 202e 6a70 2d52 656e 6465 7265  .yue .jp-Rendere
-00037060: 6448 544d 4c43 6f6d 6d6f 6e20 7462 6f64  dHTMLCommon tbod
-00037070: 7920 7472 3a6e 7468 2d63 6869 6c64 286f  y tr:nth-child(o
-00037080: 6464 292c 2e79 7565 2064 6976 2e72 656e  dd),.yue div.ren
-00037090: 6465 7265 645f 6874 6d6c 2074 626f 6479  dered_html tbody
-000370a0: 2074 723a 6e74 682d 6368 696c 6428 6f64   tr:nth-child(od
-000370b0: 6429 7b62 6163 6b67 726f 756e 642d 636f  d){background-co
-000370c0: 6c6f 723a 7661 7228 2d2d 7379 2d63 2d73  lor:var(--sy-c-s
-000370d0: 7572 6661 6365 297d 2e79 7565 202e 6a70  urface)}.yue .jp
-000370e0: 2d52 656e 6465 7265 6448 544d 4c43 6f6d  -RenderedHTMLCom
-000370f0: 6d6f 6e20 7462 6f64 7920 7472 3a68 6f76  mon tbody tr:hov
-00037100: 6572 2c2e 7975 6520 6469 762e 7265 6e64  er,.yue div.rend
-00037110: 6572 6564 5f68 746d 6c20 7462 6f64 7920  ered_html tbody 
-00037120: 7472 3a68 6f76 6572 7b62 6163 6b67 726f  tr:hover{backgro
-00037130: 756e 642d 636f 6c6f 723a 7661 7228 2d2d  und-color:var(--
-00037140: 636f 6c6f 722d 7375 7266 6163 652d 6163  color-surface-ac
-00037150: 6365 6e74 297d 2e79 7565 7b2d 2d73 672d  cent)}.yue{--sg-
-00037160: 7465 7874 2d63 6f6c 6f72 3a76 6172 282d  text-color:var(-
-00037170: 2d73 792d 632d 7465 7874 293b 2d2d 7367  -sy-c-text);--sg
-00037180: 2d62 6163 6b67 726f 756e 642d 636f 6c6f  -background-colo
-00037190: 723a 7661 7228 2d2d 7379 2d63 2d62 6163  r:var(--sy-c-bac
-000371a0: 6b67 726f 756e 6429 3b2d 2d73 672d 636f  kground);--sg-co
-000371b0: 6465 2d62 6163 6b67 726f 756e 642d 636f  de-background-co
-000371c0: 6c6f 723a 7661 7228 2d2d 7379 6e74 6178  lor:var(--syntax
-000371d0: 2d70 7265 2d62 6729 3b2d 2d73 672d 7472  -pre-bg);--sg-tr
-000371e0: 2d68 6f76 6572 2d63 6f6c 6f72 3a76 6172  -hover-color:var
-000371f0: 282d 2d61 6363 656e 742d 6133 293b 2d2d  (--accent-a3);--
-00037200: 7367 2d74 722d 6f64 642d 636f 6c6f 723a  sg-tr-odd-color:
-00037210: 7661 7228 2d2d 7379 2d63 2d73 7572 6661  var(--sy-c-surfa
-00037220: 6365 293b 2d2d 7367 2d74 6f6f 6c74 6970  ce);--sg-tooltip
-00037230: 2d66 6f72 6567 726f 756e 643a 7661 7228  -foreground:var(
-00037240: 2d2d 7379 2d63 2d62 6163 6b67 726f 756e  --sy-c-backgroun
-00037250: 642d 636f 6e74 7261 7374 293b 2d2d 7367  d-contrast);--sg
-00037260: 2d74 6f6f 6c74 6970 2d62 6163 6b67 726f  -tooltip-backgro
-00037270: 756e 643a 7661 7228 2d2d 7379 2d63 2d62  und:var(--sy-c-b
-00037280: 6163 6b67 726f 756e 6429 3b2d 2d73 672d  ackground);--sg-
-00037290: 746f 6f6c 7469 702d 626f 7264 6572 3a76  tooltip-border:v
-000372a0: 6172 282d 2d67 7261 792d 3729 2023 3030  ar(--gray-7) #00
-000372b0: 3030 3b2d 2d73 672d 7468 756d 622d 626f  00;--sg-thumb-bo
-000372c0: 782d 7368 6164 6f77 2d63 6f6c 6f72 3a76  x-shadow-color:v
-000372d0: 6172 282d 2d67 7261 792d 6134 293b 2d2d  ar(--gray-a4);--
-000372e0: 7367 2d74 6875 6d62 2d68 6f76 6572 2d62  sg-thumb-hover-b
-000372f0: 6f72 6465 723a 7661 7228 2d2d 6163 6365  order:var(--acce
-00037300: 6e74 2d61 3929 3b2d 2d73 672d 7363 7269  nt-a9);--sg-scri
-00037310: 7074 2d6f 7574 3a76 6172 282d 2d73 792d  pt-out:var(--sy-
-00037320: 632d 6c69 6768 7429 3b2d 2d73 672d 7363  c-light);--sg-sc
-00037330: 7269 7074 2d70 7265 3a76 6172 282d 2d73  ript-pre:var(--s
-00037340: 796e 7461 782d 7072 652d 6267 293b 2d2d  yntax-pre-bg);--
-00037350: 7367 2d70 7974 622d 666f 7265 6772 6f75  sg-pytb-foregrou
-00037360: 6e64 3a76 6172 282d 2d73 796e 7461 782d  nd:var(--syntax-
-00037370: 7465 7874 293b 2d2d 7367 2d70 7974 622d  text);--sg-pytb-
-00037380: 6261 636b 6772 6f75 6e64 3a76 6172 282d  background:var(-
-00037390: 2d72 6564 2d61 3229 3b2d 2d73 672d 7079  -red-a2);--sg-py
-000373a0: 7462 2d62 6f72 6465 722d 636f 6c6f 723a  tb-border-color:
-000373b0: 7661 7228 2d2d 7265 642d 6138 293b 2d2d  var(--red-a8);--
-000373c0: 7367 2d64 6f77 6e6c 6f61 642d 612d 6261  sg-download-a-ba
-000373d0: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3a76  ckground-color:v
-000373e0: 6172 282d 2d61 6363 656e 742d 6133 293b  ar(--accent-a3);
-000373f0: 2d2d 7367 2d64 6f77 6e6c 6f61 642d 612d  --sg-download-a-
-00037400: 6261 636b 6772 6f75 6e64 2d69 6d61 6765  background-image
-00037410: 3a6e 6f6e 653b 2d2d 7367 2d64 6f77 6e6c  :none;--sg-downl
-00037420: 6f61 642d 612d 626f 7264 6572 2d63 6f6c  oad-a-border-col
-00037430: 6f72 3a31 7078 2073 6f6c 6964 2076 6172  or:1px solid var
-00037440: 282d 2d61 6363 656e 742d 6133 293b 2d2d  (--accent-a3);--
-00037450: 7367 2d64 6f77 6e6c 6f61 642d 612d 636f  sg-download-a-co
-00037460: 6c6f 723a 7661 7228 2d2d 6163 6365 6e74  lor:var(--accent
-00037470: 2d61 3131 293b 2d2d 7367 2d64 6f77 6e6c  -a11);--sg-downl
-00037480: 6f61 642d 612d 686f 7665 722d 6261 636b  oad-a-hover-back
-00037490: 6772 6f75 6e64 2d63 6f6c 6f72 3a76 6172  ground-color:var
-000374a0: 282d 2d61 6363 656e 742d 6134 293b 2d2d  (--accent-a4);--
-000374b0: 7367 2d64 6f77 6e6c 6f61 642d 612d 686f  sg-download-a-ho
-000374c0: 7665 722d 626f 782d 7368 6164 6f77 2d31  ver-box-shadow-1
-000374d0: 3a23 3030 3030 3b2d 2d73 672d 646f 776e  :#0000;--sg-down
-000374e0: 6c6f 6164 2d61 2d68 6f76 6572 2d62 6f78  load-a-hover-box
-000374f0: 2d73 6861 646f 772d 323a 2330 3030 307d  -shadow-2:#0000}
-00037500: 2e79 7565 202e 7370 6878 2d67 6c72 2d64  .yue .sphx-glr-d
-00037510: 6f77 6e6c 6f61 6420 612c 2e79 7565 202e  ownload a,.yue .
-00037520: 7370 6878 2d67 6c72 2d64 6f77 6e6c 6f61  sphx-glr-downloa
-00037530: 6420 613a 686f 7665 722c 2e79 7565 202e  d a:hover,.yue .
-00037540: 7370 6878 2d67 6c72 2d74 6875 6d62 6e61  sphx-glr-thumbna
-00037550: 696c 7320 617b 626f 7264 6572 2d62 6f74  ils a{border-bot
-00037560: 746f 6d3a 307d 2e79 7565 2070 2e73 7068  tom:0}.yue p.sph
-00037570: 782d 676c 722d 7369 676e 6174 7572 6520  x-glr-signature 
-00037580: 617b 626f 7264 6572 2d72 6164 6975 733a  a{border-radius:
-00037590: 303b 626f 7264 6572 2d62 6f74 746f 6d3a  0;border-bottom:
-000375a0: 303b 7465 7874 2d64 6563 6f72 6174 696f  0;text-decoratio
-000375b0: 6e3a 756e 6465 726c 696e 657d 2e79 7565  n:underline}.yue
-000375c0: 2070 2e73 7068 782d 676c 722d 7369 676e   p.sphx-glr-sign
-000375d0: 6174 7572 6520 613a 686f 7665 727b 636f  ature a:hover{co
-000375e0: 6c6f 723a 7661 7228 2d2d 7379 2d63 2d6c  lor:var(--sy-c-l
-000375f0: 696e 6b2d 686f 7665 7229 7d2e 7975 6520  ink-hover)}.yue 
-00037600: 2e73 7068 782d 676c 722d 666f 6f74 6572  .sphx-glr-footer
-00037610: 2069 6d67 7b64 6973 706c 6179 3a69 6e6c   img{display:inl
-00037620: 696e 653b 6d61 7267 696e 3a30 7d68 746d  ine;margin:0}htm
-00037630: 6c2e 6461 726b 2c68 746d 6c2e 6c69 6768  l.dark,html.ligh
-00037640: 747b 2d2d 646f 6373 6561 7263 682d 7072  t{--docsearch-pr
-00037650: 696d 6172 792d 636f 6c6f 723a 7661 7228  imary-color:var(
-00037660: 2d2d 6163 6365 6e74 2d39 293b 2d2d 646f  --accent-9);--do
-00037670: 6373 6561 7263 682d 7465 7874 2d63 6f6c  csearch-text-col
-00037680: 6f72 3a76 6172 282d 2d73 792d 632d 7465  or:var(--sy-c-te
-00037690: 7874 293b 2d2d 646f 6373 6561 7263 682d  xt);--docsearch-
-000376a0: 6d6f 6461 6c2d 6261 636b 6772 6f75 6e64  modal-background
-000376b0: 3a76 6172 282d 2d73 792d 632d 6261 636b  :var(--sy-c-back
-000376c0: 6772 6f75 6e64 293b 2d2d 646f 6373 6561  ground);--docsea
-000376d0: 7263 682d 666f 6f74 6572 2d62 6163 6b67  rch-footer-backg
-000376e0: 726f 756e 643a 7661 7228 2d2d 7379 2d63  round:var(--sy-c
-000376f0: 2d73 7572 6661 6365 293b 2d2d 646f 6373  -surface);--docs
-00037700: 6561 7263 682d 7365 6172 6368 626f 782d  earch-searchbox-
-00037710: 6261 636b 6772 6f75 6e64 3a76 6172 282d  background:var(-
-00037720: 2d73 792d 632d 7375 7266 6163 6529 3b2d  -sy-c-surface);-
-00037730: 2d64 6f63 7365 6172 6368 2d73 6561 7263  -docsearch-searc
-00037740: 6862 6f78 2d66 6f63 7573 2d62 6163 6b67  hbox-focus-backg
-00037750: 726f 756e 643a 7661 7228 2d2d 7379 2d63  round:var(--sy-c
-00037760: 2d62 6163 6b67 726f 756e 6429 3b2d 2d64  -background);--d
-00037770: 6f63 7365 6172 6368 2d6d 7574 6564 2d63  ocsearch-muted-c
-00037780: 6f6c 6f72 3a76 6172 282d 2d73 792d 632d  olor:var(--sy-c-
-00037790: 6c69 6768 7429 3b2d 2d64 6f63 7365 6172  light);--docsear
-000377a0: 6368 2d68 6974 2d63 6f6c 6f72 3a76 6172  ch-hit-color:var
-000377b0: 282d 2d73 792d 632d 7465 7874 293b 2d2d  (--sy-c-text);--
-000377c0: 646f 6373 6561 7263 682d 6869 742d 6261  docsearch-hit-ba
-000377d0: 636b 6772 6f75 6e64 3a76 6172 282d 2d73  ckground:var(--s
-000377e0: 792d 632d 7375 7266 6163 6529 3b2d 2d64  y-c-surface);--d
-000377f0: 6f63 7365 6172 6368 2d68 6974 2d61 6374  ocsearch-hit-act
-00037800: 6976 652d 636f 6c6f 723a 7661 7228 2d2d  ive-color:var(--
-00037810: 6163 6365 6e74 2d39 2d63 6f6e 7472 6173  accent-9-contras
-00037820: 7429 3b2d 2d64 6f63 7365 6172 6368 2d68  t);--docsearch-h
-00037830: 6974 2d73 6861 646f 773a 696e 7365 7420  it-shadow:inset 
-00037840: 3020 3020 3170 7820 3020 7661 7228 2d2d  0 0 1px 0 var(--
-00037850: 6772 6179 2d61 3131 293b 2d2d 646f 6373  gray-a11);--docs
-00037860: 6561 7263 682d 636f 6e74 6169 6e65 722d  earch-container-
-00037870: 6261 636b 6772 6f75 6e64 3a76 6172 282d  background:var(-
-00037880: 2d73 792d 632d 6f76 6572 6c61 7929 7d68  -sy-c-overlay)}h
-00037890: 746d 6c2e 6c69 6768 747b 2d2d 646f 6373  tml.light{--docs
-000378a0: 6561 7263 682d 6b65 792d 6772 6164 6965  earch-key-gradie
-000378b0: 6e74 3a6c 696e 6561 722d 6772 6164 6965  nt:linear-gradie
-000378c0: 6e74 282d 3232 3564 6567 2c23 6536 6536  nt(-225deg,#e6e6
-000378d0: 6536 2c23 6638 6638 6638 293b 2d2d 646f  e6,#f8f8f8);--do
-000378e0: 6373 6561 7263 682d 6b65 792d 7368 6164  csearch-key-shad
-000378f0: 6f77 3a69 6e73 6574 2030 202d 3270 7820  ow:inset 0 -2px 
-00037900: 2364 6264 6264 622c 696e 7365 7420 3020  #dbdbdb,inset 0 
-00037910: 3020 3170 7820 3170 7820 2366 6666 2c30  0 1px 1px #fff,0
-00037920: 2031 7078 2032 7078 2031 7078 2023 3530   1px 2px 1px #50
-00037930: 3530 3530 3636 7d68 746d 6c2e 6461 726b  505066}html.dark
-00037940: 7b2d 2d64 6f63 7365 6172 6368 2d6b 6579  {--docsearch-key
-00037950: 2d67 7261 6469 656e 743a 6c69 6e65 6172  -gradient:linear
-00037960: 2d67 7261 6469 656e 7428 2d32 3235 6465  -gradient(-225de
-00037970: 672c 2333 3533 3433 342c 2331 3431 3431  g,#353434,#14141
-00037980: 3429 3b2d 2d64 6f63 7365 6172 6368 2d6b  4);--docsearch-k
-00037990: 6579 2d73 6861 646f 773a 696e 7365 7420  ey-shadow:inset 
-000379a0: 3020 2d32 7078 2023 3337 3337 3337 2c69  0 -2px #373737,i
-000379b0: 6e73 6574 2030 2030 2031 7078 2031 7078  nset 0 0 1px 1px
-000379c0: 2023 3232 322c 3020 3170 7820 3270 7820   #222,0 1px 2px 
-000379d0: 3170 7820 2330 3030 3b2d 2d64 6f63 7365  1px #000;--docse
-000379e0: 6172 6368 2d66 6f6f 7465 722d 7368 6164  arch-footer-shad
-000379f0: 6f77 3a30 202d 3170 7820 3020 3020 2333  ow:0 -1px 0 0 #3
-00037a00: 3733 3733 372c 3020 2d33 7078 2036 7078  73737,0 -3px 6px
-00037a10: 2030 2023 3134 3134 3134 3b2d 2d64 6f63   0 #141414;--doc
-00037a20: 7365 6172 6368 2d6d 6f64 616c 2d73 6861  search-modal-sha
-00037a30: 646f 773a 696e 7365 7420 3170 7820 3170  dow:inset 1px 1p
-00037a40: 7820 3020 3020 2333 3733 3733 372c 3020  x 0 0 #373737,0 
-00037a50: 3370 7820 3870 7820 3020 2331 3431 3431  3px 8px 0 #14141
-00037a60: 347d 2364 6f63 7365 6172 6368 202e 446f  4}#docsearch .Do
-00037a70: 6353 6561 7263 682d 4275 7474 6f6e 7b62  cSearch-Button{b
-00037a80: 6f72 6465 722d 7261 6469 7573 3a36 7078  order-radius:6px
-00037a90: 7d23 646f 6373 6561 7263 6820 2e44 6f63  }#docsearch .Doc
-00037aa0: 5365 6172 6368 2d42 7574 746f 6e2d 4b65  Search-Button-Ke
-00037ab0: 792c 2364 6f63 7365 6172 6368 202e 446f  y,#docsearch .Do
-00037ac0: 6353 6561 7263 682d 4275 7474 6f6e 2d50  cSearch-Button-P
-00037ad0: 6c61 6365 686f 6c64 6572 7b66 6f6e 742d  laceholder{font-
-00037ae0: 7369 7a65 3a2e 3832 3572 656d 7d23 646f  size:.825rem}#do
-00037af0: 6373 6561 7263 6820 2e44 6f63 5365 6172  csearch .DocSear
-00037b00: 6368 2d42 7574 746f 6e2d 4b65 7973 2c23  ch-Button-Keys,#
-00037b10: 646f 6373 6561 7263 6820 2e44 6f63 5365  docsearch .DocSe
-00037b20: 6172 6368 2d42 7574 746f 6e2d 506c 6163  arch-Button-Plac
-00037b30: 6568 6f6c 6465 727b 6469 7370 6c61 793a  eholder{display:
-00037b40: 666c 6578 2169 6d70 6f72 7461 6e74 7d23  flex!important}#
-00037b50: 646f 6373 6561 7263 6820 2e44 6f63 5365  docsearch .DocSe
-00037b60: 6172 6368 2d53 6561 7263 682d 4963 6f6e  arch-Search-Icon
-00037b70: 7b77 6964 7468 3a2e 3837 3572 656d 2169  {width:.875rem!i
-00037b80: 6d70 6f72 7461 6e74 3b68 6569 6768 743a  mportant;height:
-00037b90: 2e38 3735 7265 6d21 696d 706f 7274 616e  .875rem!importan
-00037ba0: 747d 406d 6564 6961 2028 6d61 782d 7769  t}@media (max-wi
-00037bb0: 6474 683a 3736 3770 7829 7b23 646f 6373  dth:767px){#docs
-00037bc0: 6561 7263 687b 706f 7369 7469 6f6e 3a61  earch{position:a
-00037bd0: 6273 6f6c 7574 653b 746f 703a 3172 656d  bsolute;top:1rem
-00037be0: 3b6c 6566 743a 312e 3872 656d 3b72 6967  ;left:1.8rem;rig
-00037bf0: 6874 3a31 2e38 7265 6d7d 2364 6f63 7365  ht:1.8rem}#docse
-00037c00: 6172 6368 202e 446f 6353 6561 7263 682d  arch .DocSearch-
-00037c10: 4275 7474 6f6e 7b6d 6172 6769 6e2d 6c65  Button{margin-le
-00037c20: 6674 3a30 3b77 6964 7468 3a31 3030 257d  ft:0;width:100%}
-00037c30: 7d64 6c2e 7371 6c61 2064 747b 636f 6c6f  }dl.sqla dt{colo
-00037c40: 723a 7661 7228 2d2d 7369 672d 6e61 6d65  r:var(--sig-name
-00037c50: 293b 6d61 7267 696e 2d62 6f74 746f 6d3a  );margin-bottom:
-00037c60: 2e35 7265 6d7d 646c 2e73 716c 6120 6474  .5rem}dl.sqla dt
-00037c70: 3e65 6d7b 666f 6e74 2d77 6569 6768 743a  >em{font-weight:
-00037c80: 3430 303b 666f 6e74 2d73 7479 6c65 3a6e  400;font-style:n
-00037c90: 6f72 6d61 6c3b 636f 6c6f 723a 7661 7228  ormal;color:var(
-00037ca0: 2d2d 7369 672d 7061 7261 6d29 7d64 6c2e  --sig-param)}dl.
-00037cb0: 7371 6c61 2064 643e 702e 7275 6272 6963  sqla dd>p.rubric
-00037cc0: 7b6d 6172 6769 6e2d 746f 703a 312e 3572  {margin-top:1.5r
-00037cd0: 656d 3b74 6578 742d 7472 616e 7366 6f72  em;text-transfor
-00037ce0: 6d3a 7570 7065 7263 6173 653b 666f 6e74  m:uppercase;font
-00037cf0: 2d73 697a 653a 2e37 3672 656d 7d64 6c2e  -size:.76rem}dl.
-00037d00: 7371 6c61 2064 643e 702e 7275 6272 6963  sqla dd>p.rubric
-00037d10: 2b2e 7461 626c 652d 7772 6170 7065 727b  +.table-wrapper{
-00037d20: 6d61 7267 696e 2d74 6f70 3a2e 3735 7265  margin-top:.75re
-00037d30: 6d3b 626f 7264 6572 2d6c 6566 743a 303b  m;border-left:0;
-00037d40: 626f 7264 6572 2d72 6967 6874 3a30 3b62  border-right:0;b
-00037d50: 6f72 6465 722d 7261 6469 7573 3a30 7d64  order-radius:0}d
-00037d60: 6c2e 7371 6c61 2070 2e72 7562 7269 632b  l.sqla p.rubric+
-00037d70: 2e74 6162 6c65 2d77 7261 7070 6572 2074  .table-wrapper t
-00037d80: 642c 646c 2e73 716c 6120 702e 7275 6272  d,dl.sqla p.rubr
+00032be0: 6967 6874 2d6d 6172 6b75 702d 626f 6c64  ight-markup-bold
+00032bf0: 3a23 3234 3239 3266 3b2d 2d73 796e 7461  :#24292f;--synta
+00032c00: 782d 6c69 6768 742d 6d61 726b 7570 2d64  x-light-markup-d
+00032c10: 656c 6574 6564 2d74 6578 743a 2338 3230  eleted-text:#820
+00032c20: 3731 653b 2d2d 7379 6e74 6178 2d6c 6967  71e;--syntax-lig
+00032c30: 6874 2d6d 6172 6b75 702d 6465 6c65 7465  ht-markup-delete
+00032c40: 642d 6267 3a23 6666 6562 6539 3b2d 2d73  d-bg:#ffebe9;--s
+00032c50: 796e 7461 782d 6c69 6768 742d 6d61 726b  yntax-light-mark
+00032c60: 7570 2d69 6e73 6572 7465 642d 7465 7874  up-inserted-text
+00032c70: 3a23 3131 3633 3239 3b2d 2d73 796e 7461  :#116329;--synta
+00032c80: 782d 6c69 6768 742d 6d61 726b 7570 2d69  x-light-markup-i
+00032c90: 6e73 6572 7465 642d 6267 3a23 6461 6662  nserted-bg:#dafb
+00032ca0: 6531 3b2d 2d73 796e 7461 782d 6c69 6768  e1;--syntax-ligh
+00032cb0: 742d 6d61 726b 7570 2d63 6861 6e67 6564  t-markup-changed
+00032cc0: 2d74 6578 743a 2339 3533 3830 303b 2d2d  -text:#953800;--
+00032cd0: 7379 6e74 6178 2d6c 6967 6874 2d6d 6172  syntax-light-mar
+00032ce0: 6b75 702d 6368 616e 6765 642d 6267 3a23  kup-changed-bg:#
+00032cf0: 6666 6438 6235 3b2d 2d73 796e 7461 782d  ffd8b5;--syntax-
+00032d00: 6c69 6768 742d 6d61 726b 7570 2d69 676e  light-markup-ign
+00032d10: 6f72 6564 2d74 6578 743a 2365 6165 6566  ored-text:#eaeef
+00032d20: 323b 2d2d 7379 6e74 6178 2d6c 6967 6874  2;--syntax-light
+00032d30: 2d6d 6172 6b75 702d 6967 6e6f 7265 642d  -markup-ignored-
+00032d40: 6267 3a23 3035 3530 6165 3b2d 2d73 796e  bg:#0550ae;--syn
+00032d50: 7461 782d 6c69 6768 742d 6d65 7461 2d64  tax-light-meta-d
+00032d60: 6966 662d 7261 6e67 653a 2338 3235 3064  iff-range:#8250d
+00032d70: 663b 2d2d 7379 6e74 6178 2d6c 6967 6874  f;--syntax-light
+00032d80: 2d73 7065 6369 616c 2d62 673a 2364 6363  -special-bg:#dcc
+00032d90: 6166 613b 2d2d 7379 6e74 6178 2d64 6172  afa;--syntax-dar
+00032da0: 6b2d 7465 7874 3a23 6339 6431 6439 3b2d  k-text:#c9d1d9;-
+00032db0: 2d73 796e 7461 782d 6461 726b 2d6d 6574  -syntax-dark-met
+00032dc0: 613a 2336 6537 3738 313b 2d2d 7379 6e74  a:#6e7781;--synt
+00032dd0: 6178 2d64 6172 6b2d 636f 6d6d 656e 743a  ax-dark-comment:
+00032de0: 2338 6239 3439 653b 2d2d 7379 6e74 6178  #8b949e;--syntax
+00032df0: 2d64 6172 6b2d 636f 6e73 7461 6e74 3a23  -dark-constant:#
+00032e00: 3739 6330 6666 3b2d 2d73 796e 7461 782d  79c0ff;--syntax-
+00032e10: 6461 726b 2d65 6e74 6974 793a 2334 3762  dark-entity:#47b
+00032e20: 3066 613b 2d2d 7379 6e74 6178 2d64 6172  0fa;--syntax-dar
+00032e30: 6b2d 7072 6f70 6572 7479 3a23 6432 6138  k-property:#d2a8
+00032e40: 6666 3b2d 2d73 796e 7461 782d 6461 726b  ff;--syntax-dark
+00032e50: 2d64 6566 696e 6974 696f 6e3a 2363 3964  -definition:#c9d
+00032e60: 3164 393b 2d2d 7379 6e74 6178 2d64 6172  1d9;--syntax-dar
+00032e70: 6b2d 7461 673a 2337 6565 3738 373b 2d2d  k-tag:#7ee787;--
+00032e80: 7379 6e74 6178 2d64 6172 6b2d 6275 696c  syntax-dark-buil
+00032e90: 7469 6e3a 2366 6664 3334 633b 2d2d 7379  tin:#ffd34c;--sy
+00032ea0: 6e74 6178 2d64 6172 6b2d 6b65 7977 6f72  ntax-dark-keywor
+00032eb0: 643a 2366 6637 6237 323b 2d2d 7379 6e74  d:#ff7b72;--synt
+00032ec0: 6178 2d64 6172 6b2d 6578 6365 7074 696f  ax-dark-exceptio
+00032ed0: 6e3a 2364 6134 3733 633b 2d2d 7379 6e74  n:#da473c;--synt
+00032ee0: 6178 2d64 6172 6b2d 7374 7269 6e67 3a23  ax-dark-string:#
+00032ef0: 6135 6436 6666 3b2d 2d73 796e 7461 782d  a5d6ff;--syntax-
+00032f00: 6461 726b 2d72 6567 6578 703a 2365 6639  dark-regexp:#ef9
+00032f10: 3534 653b 2d2d 7379 6e74 6178 2d64 6172  54e;--syntax-dar
+00032f20: 6b2d 7661 7269 6162 6c65 3a23 6666 6136  k-variable:#ffa6
+00032f30: 3537 3b2d 2d73 796e 7461 782d 6461 726b  57;--syntax-dark
+00032f40: 2d69 6e76 616c 6964 2d69 6c6c 6567 616c  -invalid-illegal
+00032f50: 2d74 6578 743a 2366 3066 3666 633b 2d2d  -text:#f0f6fc;--
+00032f60: 7379 6e74 6178 2d64 6172 6b2d 696e 7661  syntax-dark-inva
+00032f70: 6c69 642d 696c 6c65 6761 6c2d 6267 3a23  lid-illegal-bg:#
+00032f80: 3865 3135 3139 3b2d 2d73 796e 7461 782d  8e1519;--syntax-
+00032f90: 6461 726b 2d6d 6172 6b75 702d 6865 6164  dark-markup-head
+00032fa0: 696e 673a 2331 6636 6665 623b 2d2d 7379  ing:#1f6feb;--sy
+00032fb0: 6e74 6178 2d64 6172 6b2d 6d61 726b 7570  ntax-dark-markup
+00032fc0: 2d69 7461 6c69 633a 2363 3964 3164 393b  -italic:#c9d1d9;
+00032fd0: 2d2d 7379 6e74 6178 2d64 6172 6b2d 6d61  --syntax-dark-ma
+00032fe0: 726b 7570 2d62 6f6c 643a 2363 3964 3164  rkup-bold:#c9d1d
+00032ff0: 393b 2d2d 7379 6e74 6178 2d64 6172 6b2d  9;--syntax-dark-
+00033000: 6d61 726b 7570 2d64 656c 6574 6564 2d74  markup-deleted-t
+00033010: 6578 743a 2366 6664 6364 373b 2d2d 7379  ext:#ffdcd7;--sy
+00033020: 6e74 6178 2d64 6172 6b2d 6d61 726b 7570  ntax-dark-markup
+00033030: 2d64 656c 6574 6564 2d62 673a 2336 3730  -deleted-bg:#670
+00033040: 3630 633b 2d2d 7379 6e74 6178 2d64 6172  60c;--syntax-dar
+00033050: 6b2d 6d61 726b 7570 2d69 6e73 6572 7465  k-markup-inserte
+00033060: 642d 7465 7874 3a23 6166 6635 6234 3b2d  d-text:#aff5b4;-
+00033070: 2d73 796e 7461 782d 6461 726b 2d6d 6172  -syntax-dark-mar
+00033080: 6b75 702d 696e 7365 7274 6564 2d62 673a  kup-inserted-bg:
+00033090: 2330 3333 6131 363b 2d2d 7379 6e74 6178  #033a16;--syntax
+000330a0: 2d64 6172 6b2d 6d61 726b 7570 2d63 6861  -dark-markup-cha
+000330b0: 6e67 6564 2d74 6578 743a 2366 6664 6662  nged-text:#ffdfb
+000330c0: 363b 2d2d 7379 6e74 6178 2d64 6172 6b2d  6;--syntax-dark-
+000330d0: 6d61 726b 7570 2d63 6861 6e67 6564 2d62  markup-changed-b
+000330e0: 673a 2335 6131 6530 323b 2d2d 7379 6e74  g:#5a1e02;--synt
+000330f0: 6178 2d64 6172 6b2d 6d61 726b 7570 2d69  ax-dark-markup-i
+00033100: 676e 6f72 6564 2d74 6578 743a 2363 3964  gnored-text:#c9d
+00033110: 3164 393b 2d2d 7379 6e74 6178 2d64 6172  1d9;--syntax-dar
+00033120: 6b2d 6d61 726b 7570 2d69 676e 6f72 6564  k-markup-ignored
+00033130: 2d62 673a 2331 3135 3863 373b 2d2d 7379  -bg:#1158c7;--sy
+00033140: 6e74 6178 2d64 6172 6b2d 6d65 7461 2d64  ntax-dark-meta-d
+00033150: 6966 662d 7261 6e67 653a 2364 3261 3866  iff-range:#d2a8f
+00033160: 663b 2d2d 7379 6e74 6178 2d64 6172 6b2d  f;--syntax-dark-
+00033170: 7370 6563 6961 6c2d 6267 3a23 3466 3432  special-bg:#4f42
+00033180: 3564 7d3a 726f 6f74 2c68 746d 6c2e 6c69  5d}:root,html.li
+00033190: 6768 747b 2d2d 7379 6e74 6178 2d74 6578  ght{--syntax-tex
+000331a0: 743a 7661 7228 2d2d 7379 6e74 6178 2d6c  t:var(--syntax-l
+000331b0: 6967 6874 2d74 6578 7429 3b2d 2d73 796e  ight-text);--syn
+000331c0: 7461 782d 6d65 7461 3a76 6172 282d 2d73  tax-meta:var(--s
+000331d0: 796e 7461 782d 6c69 6768 742d 6d65 7461  yntax-light-meta
+000331e0: 293b 2d2d 7379 6e74 6178 2d63 6f6d 6d65  );--syntax-comme
+000331f0: 6e74 3a76 6172 282d 2d73 796e 7461 782d  nt:var(--syntax-
+00033200: 6c69 6768 742d 636f 6d6d 656e 7429 3b2d  light-comment);-
+00033210: 2d73 796e 7461 782d 636f 6e73 7461 6e74  -syntax-constant
+00033220: 3a76 6172 282d 2d73 796e 7461 782d 6c69  :var(--syntax-li
+00033230: 6768 742d 636f 6e73 7461 6e74 293b 2d2d  ght-constant);--
+00033240: 7379 6e74 6178 2d65 6e74 6974 793a 7661  syntax-entity:va
+00033250: 7228 2d2d 7379 6e74 6178 2d6c 6967 6874  r(--syntax-light
+00033260: 2d65 6e74 6974 7929 3b2d 2d73 796e 7461  -entity);--synta
+00033270: 782d 7072 6f70 6572 7479 3a76 6172 282d  x-property:var(-
+00033280: 2d73 796e 7461 782d 6c69 6768 742d 7072  -syntax-light-pr
+00033290: 6f70 6572 7479 293b 2d2d 7379 6e74 6178  operty);--syntax
+000332a0: 2d64 6566 696e 6974 696f 6e3a 7661 7228  -definition:var(
+000332b0: 2d2d 7379 6e74 6178 2d6c 6967 6874 2d64  --syntax-light-d
+000332c0: 6566 696e 6974 696f 6e29 3b2d 2d73 796e  efinition);--syn
+000332d0: 7461 782d 7461 673a 7661 7228 2d2d 7379  tax-tag:var(--sy
+000332e0: 6e74 6178 2d6c 6967 6874 2d74 6167 293b  ntax-light-tag);
+000332f0: 2d2d 7379 6e74 6178 2d62 7569 6c74 696e  --syntax-builtin
+00033300: 3a76 6172 282d 2d73 796e 7461 782d 6c69  :var(--syntax-li
+00033310: 6768 742d 6275 696c 7469 6e29 3b2d 2d73  ght-builtin);--s
+00033320: 796e 7461 782d 6b65 7977 6f72 643a 7661  yntax-keyword:va
+00033330: 7228 2d2d 7379 6e74 6178 2d6c 6967 6874  r(--syntax-light
+00033340: 2d6b 6579 776f 7264 293b 2d2d 7379 6e74  -keyword);--synt
+00033350: 6178 2d65 7863 6570 7469 6f6e 3a76 6172  ax-exception:var
+00033360: 282d 2d73 796e 7461 782d 6c69 6768 742d  (--syntax-light-
+00033370: 6578 6365 7074 696f 6e29 3b2d 2d73 796e  exception);--syn
+00033380: 7461 782d 7374 7269 6e67 3a76 6172 282d  tax-string:var(-
+00033390: 2d73 796e 7461 782d 6c69 6768 742d 7374  -syntax-light-st
+000333a0: 7269 6e67 293b 2d2d 7379 6e74 6178 2d72  ring);--syntax-r
+000333b0: 6567 6578 703a 7661 7228 2d2d 7379 6e74  egexp:var(--synt
+000333c0: 6178 2d6c 6967 6874 2d72 6567 6578 7029  ax-light-regexp)
+000333d0: 3b2d 2d73 796e 7461 782d 7661 7269 6162  ;--syntax-variab
+000333e0: 6c65 3a76 6172 282d 2d73 796e 7461 782d  le:var(--syntax-
+000333f0: 6c69 6768 742d 7661 7269 6162 6c65 293b  light-variable);
+00033400: 2d2d 7379 6e74 6178 2d69 6e76 616c 6964  --syntax-invalid
+00033410: 2d69 6c6c 6567 616c 2d74 6578 743a 7661  -illegal-text:va
+00033420: 7228 2d2d 7379 6e74 6178 2d6c 6967 6874  r(--syntax-light
+00033430: 2d69 6e76 616c 6964 2d69 6c6c 6567 616c  -invalid-illegal
+00033440: 2d74 6578 7429 3b2d 2d73 796e 7461 782d  -text);--syntax-
+00033450: 696e 7661 6c69 642d 696c 6c65 6761 6c2d  invalid-illegal-
+00033460: 6267 3a76 6172 282d 2d73 796e 7461 782d  bg:var(--syntax-
+00033470: 6c69 6768 742d 696e 7661 6c69 642d 696c  light-invalid-il
+00033480: 6c65 6761 6c2d 6267 293b 2d2d 7379 6e74  legal-bg);--synt
+00033490: 6178 2d6d 6172 6b75 702d 6865 6164 696e  ax-markup-headin
+000334a0: 673a 7661 7228 2d2d 7379 6e74 6178 2d6c  g:var(--syntax-l
+000334b0: 6967 6874 2d6d 6172 6b75 702d 6865 6164  ight-markup-head
+000334c0: 696e 6729 3b2d 2d73 796e 7461 782d 6d61  ing);--syntax-ma
+000334d0: 726b 7570 2d69 7461 6c69 633a 7661 7228  rkup-italic:var(
+000334e0: 2d2d 7379 6e74 6178 2d6c 6967 6874 2d6d  --syntax-light-m
+000334f0: 6172 6b75 702d 6974 616c 6963 293b 2d2d  arkup-italic);--
+00033500: 7379 6e74 6178 2d6d 6172 6b75 702d 626f  syntax-markup-bo
+00033510: 6c64 3a76 6172 282d 2d73 796e 7461 782d  ld:var(--syntax-
+00033520: 6c69 6768 742d 6d61 726b 7570 2d62 6f6c  light-markup-bol
+00033530: 6429 3b2d 2d73 796e 7461 782d 6d61 726b  d);--syntax-mark
+00033540: 7570 2d64 656c 6574 6564 2d74 6578 743a  up-deleted-text:
+00033550: 7661 7228 2d2d 7379 6e74 6178 2d6c 6967  var(--syntax-lig
+00033560: 6874 2d6d 6172 6b75 702d 6465 6c65 7465  ht-markup-delete
+00033570: 642d 7465 7874 293b 2d2d 7379 6e74 6178  d-text);--syntax
+00033580: 2d6d 6172 6b75 702d 6465 6c65 7465 642d  -markup-deleted-
+00033590: 6267 3a76 6172 282d 2d73 796e 7461 782d  bg:var(--syntax-
+000335a0: 6c69 6768 742d 6d61 726b 7570 2d64 656c  light-markup-del
+000335b0: 6574 6564 2d62 6729 3b2d 2d73 796e 7461  eted-bg);--synta
+000335c0: 782d 6d61 726b 7570 2d69 6e73 6572 7465  x-markup-inserte
+000335d0: 642d 7465 7874 3a76 6172 282d 2d73 796e  d-text:var(--syn
+000335e0: 7461 782d 6c69 6768 742d 6d61 726b 7570  tax-light-markup
+000335f0: 2d69 6e73 6572 7465 642d 7465 7874 293b  -inserted-text);
+00033600: 2d2d 7379 6e74 6178 2d6d 6172 6b75 702d  --syntax-markup-
+00033610: 696e 7365 7274 6564 2d62 673a 7661 7228  inserted-bg:var(
+00033620: 2d2d 7379 6e74 6178 2d6c 6967 6874 2d6d  --syntax-light-m
+00033630: 6172 6b75 702d 696e 7365 7274 6564 2d62  arkup-inserted-b
+00033640: 6729 3b2d 2d73 796e 7461 782d 6d61 726b  g);--syntax-mark
+00033650: 7570 2d63 6861 6e67 6564 2d74 6578 743a  up-changed-text:
+00033660: 7661 7228 2d2d 7379 6e74 6178 2d6c 6967  var(--syntax-lig
+00033670: 6874 2d6d 6172 6b75 702d 6368 616e 6765  ht-markup-change
+00033680: 642d 7465 7874 293b 2d2d 7379 6e74 6178  d-text);--syntax
+00033690: 2d6d 6172 6b75 702d 6368 616e 6765 642d  -markup-changed-
+000336a0: 6267 3a76 6172 282d 2d73 796e 7461 782d  bg:var(--syntax-
+000336b0: 6c69 6768 742d 6d61 726b 7570 2d63 6861  light-markup-cha
+000336c0: 6e67 6564 2d62 6729 3b2d 2d73 796e 7461  nged-bg);--synta
+000336d0: 782d 6d61 726b 7570 2d69 676e 6f72 6564  x-markup-ignored
+000336e0: 2d74 6578 743a 7661 7228 2d2d 7379 6e74  -text:var(--synt
+000336f0: 6178 2d6c 6967 6874 2d6d 6172 6b75 702d  ax-light-markup-
+00033700: 6967 6e6f 7265 642d 7465 7874 293b 2d2d  ignored-text);--
+00033710: 7379 6e74 6178 2d6d 6172 6b75 702d 6967  syntax-markup-ig
+00033720: 6e6f 7265 642d 6267 3a76 6172 282d 2d73  nored-bg:var(--s
+00033730: 796e 7461 782d 6c69 6768 742d 6d61 726b  yntax-light-mark
+00033740: 7570 2d69 676e 6f72 6564 2d62 6729 3b2d  up-ignored-bg);-
+00033750: 2d73 796e 7461 782d 6d65 7461 2d64 6966  -syntax-meta-dif
+00033760: 662d 7261 6e67 653a 7661 7228 2d2d 7379  f-range:var(--sy
+00033770: 6e74 6178 2d6c 6967 6874 2d6d 6574 612d  ntax-light-meta-
+00033780: 6469 6666 2d72 616e 6765 293b 2d2d 7379  diff-range);--sy
+00033790: 6e74 6178 2d73 7065 6369 616c 2d62 673a  ntax-special-bg:
+000337a0: 7661 7228 2d2d 7379 6e74 6178 2d6c 6967  var(--syntax-lig
+000337b0: 6874 2d73 7065 6369 616c 2d62 6729 7d40  ht-special-bg)}@
+000337c0: 6d65 6469 6120 2870 7265 6665 7273 2d63  media (prefers-c
+000337d0: 6f6c 6f72 2d73 6368 656d 653a 6461 726b  olor-scheme:dark
+000337e0: 297b 3a72 6f6f 747b 2d2d 7379 6e74 6178  ){:root{--syntax
+000337f0: 2d74 6578 743a 7661 7228 2d2d 7379 6e74  -text:var(--synt
+00033800: 6178 2d64 6172 6b2d 7465 7874 293b 2d2d  ax-dark-text);--
+00033810: 7379 6e74 6178 2d6d 6574 613a 7661 7228  syntax-meta:var(
+00033820: 2d2d 7379 6e74 6178 2d64 6172 6b2d 6d65  --syntax-dark-me
+00033830: 7461 293b 2d2d 7379 6e74 6178 2d63 6f6d  ta);--syntax-com
+00033840: 6d65 6e74 3a76 6172 282d 2d73 796e 7461  ment:var(--synta
+00033850: 782d 6461 726b 2d63 6f6d 6d65 6e74 293b  x-dark-comment);
+00033860: 2d2d 7379 6e74 6178 2d63 6f6e 7374 616e  --syntax-constan
+00033870: 743a 7661 7228 2d2d 7379 6e74 6178 2d64  t:var(--syntax-d
+00033880: 6172 6b2d 636f 6e73 7461 6e74 293b 2d2d  ark-constant);--
+00033890: 7379 6e74 6178 2d65 6e74 6974 793a 7661  syntax-entity:va
+000338a0: 7228 2d2d 7379 6e74 6178 2d64 6172 6b2d  r(--syntax-dark-
+000338b0: 656e 7469 7479 293b 2d2d 7379 6e74 6178  entity);--syntax
+000338c0: 2d70 726f 7065 7274 793a 7661 7228 2d2d  -property:var(--
+000338d0: 7379 6e74 6178 2d64 6172 6b2d 7072 6f70  syntax-dark-prop
+000338e0: 6572 7479 293b 2d2d 7379 6e74 6178 2d64  erty);--syntax-d
+000338f0: 6566 696e 6974 696f 6e3a 7661 7228 2d2d  efinition:var(--
+00033900: 7379 6e74 6178 2d64 6172 6b2d 6465 6669  syntax-dark-defi
+00033910: 6e69 7469 6f6e 293b 2d2d 7379 6e74 6178  nition);--syntax
+00033920: 2d74 6167 3a76 6172 282d 2d73 796e 7461  -tag:var(--synta
+00033930: 782d 6461 726b 2d74 6167 293b 2d2d 7379  x-dark-tag);--sy
+00033940: 6e74 6178 2d62 7569 6c74 696e 3a76 6172  ntax-builtin:var
+00033950: 282d 2d73 796e 7461 782d 6461 726b 2d62  (--syntax-dark-b
+00033960: 7569 6c74 696e 293b 2d2d 7379 6e74 6178  uiltin);--syntax
+00033970: 2d6b 6579 776f 7264 3a76 6172 282d 2d73  -keyword:var(--s
+00033980: 796e 7461 782d 6461 726b 2d6b 6579 776f  yntax-dark-keywo
+00033990: 7264 293b 2d2d 7379 6e74 6178 2d65 7863  rd);--syntax-exc
+000339a0: 6570 7469 6f6e 3a76 6172 282d 2d73 796e  eption:var(--syn
+000339b0: 7461 782d 6461 726b 2d65 7863 6570 7469  tax-dark-excepti
+000339c0: 6f6e 293b 2d2d 7379 6e74 6178 2d73 7472  on);--syntax-str
+000339d0: 696e 673a 7661 7228 2d2d 7379 6e74 6178  ing:var(--syntax
+000339e0: 2d64 6172 6b2d 7374 7269 6e67 293b 2d2d  -dark-string);--
+000339f0: 7379 6e74 6178 2d72 6567 6578 703a 7661  syntax-regexp:va
+00033a00: 7228 2d2d 7379 6e74 6178 2d64 6172 6b2d  r(--syntax-dark-
+00033a10: 7265 6765 7870 293b 2d2d 7379 6e74 6178  regexp);--syntax
+00033a20: 2d76 6172 6961 626c 653a 7661 7228 2d2d  -variable:var(--
+00033a30: 7379 6e74 6178 2d64 6172 6b2d 7661 7269  syntax-dark-vari
+00033a40: 6162 6c65 293b 2d2d 7379 6e74 6178 2d69  able);--syntax-i
+00033a50: 6e76 616c 6964 2d69 6c6c 6567 616c 2d74  nvalid-illegal-t
+00033a60: 6578 743a 7661 7228 2d2d 7379 6e74 6178  ext:var(--syntax
+00033a70: 2d64 6172 6b2d 696e 7661 6c69 642d 696c  -dark-invalid-il
+00033a80: 6c65 6761 6c2d 7465 7874 293b 2d2d 7379  legal-text);--sy
+00033a90: 6e74 6178 2d69 6e76 616c 6964 2d69 6c6c  ntax-invalid-ill
+00033aa0: 6567 616c 2d62 673a 7661 7228 2d2d 7379  egal-bg:var(--sy
+00033ab0: 6e74 6178 2d64 6172 6b2d 696e 7661 6c69  ntax-dark-invali
+00033ac0: 642d 696c 6c65 6761 6c2d 6267 293b 2d2d  d-illegal-bg);--
+00033ad0: 7379 6e74 6178 2d6d 6172 6b75 702d 6865  syntax-markup-he
+00033ae0: 6164 696e 673a 7661 7228 2d2d 7379 6e74  ading:var(--synt
+00033af0: 6178 2d64 6172 6b2d 6d61 726b 7570 2d68  ax-dark-markup-h
+00033b00: 6561 6469 6e67 293b 2d2d 7379 6e74 6178  eading);--syntax
+00033b10: 2d6d 6172 6b75 702d 6974 616c 6963 3a76  -markup-italic:v
+00033b20: 6172 282d 2d73 796e 7461 782d 6461 726b  ar(--syntax-dark
+00033b30: 2d6d 6172 6b75 702d 6974 616c 6963 293b  -markup-italic);
+00033b40: 2d2d 7379 6e74 6178 2d6d 6172 6b75 702d  --syntax-markup-
+00033b50: 626f 6c64 3a76 6172 282d 2d73 796e 7461  bold:var(--synta
+00033b60: 782d 6461 726b 2d6d 6172 6b75 702d 626f  x-dark-markup-bo
+00033b70: 6c64 293b 2d2d 7379 6e74 6178 2d6d 6172  ld);--syntax-mar
+00033b80: 6b75 702d 6465 6c65 7465 642d 7465 7874  kup-deleted-text
+00033b90: 3a76 6172 282d 2d73 796e 7461 782d 6461  :var(--syntax-da
+00033ba0: 726b 2d6d 6172 6b75 702d 6465 6c65 7465  rk-markup-delete
+00033bb0: 642d 7465 7874 293b 2d2d 7379 6e74 6178  d-text);--syntax
+00033bc0: 2d6d 6172 6b75 702d 6465 6c65 7465 642d  -markup-deleted-
+00033bd0: 6267 3a76 6172 282d 2d73 796e 7461 782d  bg:var(--syntax-
+00033be0: 6461 726b 2d6d 6172 6b75 702d 6465 6c65  dark-markup-dele
+00033bf0: 7465 642d 6267 293b 2d2d 7379 6e74 6178  ted-bg);--syntax
+00033c00: 2d6d 6172 6b75 702d 696e 7365 7274 6564  -markup-inserted
+00033c10: 2d74 6578 743a 7661 7228 2d2d 7379 6e74  -text:var(--synt
+00033c20: 6178 2d64 6172 6b2d 6d61 726b 7570 2d69  ax-dark-markup-i
+00033c30: 6e73 6572 7465 642d 7465 7874 293b 2d2d  nserted-text);--
+00033c40: 7379 6e74 6178 2d6d 6172 6b75 702d 696e  syntax-markup-in
+00033c50: 7365 7274 6564 2d62 673a 7661 7228 2d2d  serted-bg:var(--
+00033c60: 7379 6e74 6178 2d64 6172 6b2d 6d61 726b  syntax-dark-mark
+00033c70: 7570 2d69 6e73 6572 7465 642d 6267 293b  up-inserted-bg);
+00033c80: 2d2d 7379 6e74 6178 2d6d 6172 6b75 702d  --syntax-markup-
+00033c90: 6368 616e 6765 642d 7465 7874 3a76 6172  changed-text:var
+00033ca0: 282d 2d73 796e 7461 782d 6461 726b 2d6d  (--syntax-dark-m
+00033cb0: 6172 6b75 702d 6368 616e 6765 642d 7465  arkup-changed-te
+00033cc0: 7874 293b 2d2d 7379 6e74 6178 2d6d 6172  xt);--syntax-mar
+00033cd0: 6b75 702d 6368 616e 6765 642d 6267 3a76  kup-changed-bg:v
+00033ce0: 6172 282d 2d73 796e 7461 782d 6461 726b  ar(--syntax-dark
+00033cf0: 2d6d 6172 6b75 702d 6368 616e 6765 642d  -markup-changed-
+00033d00: 6267 293b 2d2d 7379 6e74 6178 2d6d 6172  bg);--syntax-mar
+00033d10: 6b75 702d 6967 6e6f 7265 642d 7465 7874  kup-ignored-text
+00033d20: 3a76 6172 282d 2d73 796e 7461 782d 6461  :var(--syntax-da
+00033d30: 726b 2d6d 6172 6b75 702d 6967 6e6f 7265  rk-markup-ignore
+00033d40: 642d 7465 7874 293b 2d2d 7379 6e74 6178  d-text);--syntax
+00033d50: 2d6d 6172 6b75 702d 6967 6e6f 7265 642d  -markup-ignored-
+00033d60: 6267 3a76 6172 282d 2d73 796e 7461 782d  bg:var(--syntax-
+00033d70: 6461 726b 2d6d 6172 6b75 702d 6967 6e6f  dark-markup-igno
+00033d80: 7265 642d 6267 293b 2d2d 7379 6e74 6178  red-bg);--syntax
+00033d90: 2d6d 6574 612d 6469 6666 2d72 616e 6765  -meta-diff-range
+00033da0: 3a76 6172 282d 2d73 796e 7461 782d 6461  :var(--syntax-da
+00033db0: 726b 2d6d 6574 612d 6469 6666 2d72 616e  rk-meta-diff-ran
+00033dc0: 6765 293b 2d2d 7379 6e74 6178 2d73 7065  ge);--syntax-spe
+00033dd0: 6369 616c 2d62 673a 7661 7228 2d2d 7379  cial-bg:var(--sy
+00033de0: 6e74 6178 2d64 6172 6b2d 7370 6563 6961  ntax-dark-specia
+00033df0: 6c2d 6267 297d 7d68 746d 6c2e 6461 726b  l-bg)}}html.dark
+00033e00: 7b2d 2d73 796e 7461 782d 7465 7874 3a76  {--syntax-text:v
+00033e10: 6172 282d 2d73 796e 7461 782d 6461 726b  ar(--syntax-dark
+00033e20: 2d74 6578 7429 3b2d 2d73 796e 7461 782d  -text);--syntax-
+00033e30: 6d65 7461 3a76 6172 282d 2d73 796e 7461  meta:var(--synta
+00033e40: 782d 6461 726b 2d6d 6574 6129 3b2d 2d73  x-dark-meta);--s
+00033e50: 796e 7461 782d 636f 6d6d 656e 743a 7661  yntax-comment:va
+00033e60: 7228 2d2d 7379 6e74 6178 2d64 6172 6b2d  r(--syntax-dark-
+00033e70: 636f 6d6d 656e 7429 3b2d 2d73 796e 7461  comment);--synta
+00033e80: 782d 636f 6e73 7461 6e74 3a76 6172 282d  x-constant:var(-
+00033e90: 2d73 796e 7461 782d 6461 726b 2d63 6f6e  -syntax-dark-con
+00033ea0: 7374 616e 7429 3b2d 2d73 796e 7461 782d  stant);--syntax-
+00033eb0: 656e 7469 7479 3a76 6172 282d 2d73 796e  entity:var(--syn
+00033ec0: 7461 782d 6461 726b 2d65 6e74 6974 7929  tax-dark-entity)
+00033ed0: 3b2d 2d73 796e 7461 782d 7072 6f70 6572  ;--syntax-proper
+00033ee0: 7479 3a76 6172 282d 2d73 796e 7461 782d  ty:var(--syntax-
+00033ef0: 6461 726b 2d70 726f 7065 7274 7929 3b2d  dark-property);-
+00033f00: 2d73 796e 7461 782d 6465 6669 6e69 7469  -syntax-definiti
+00033f10: 6f6e 3a76 6172 282d 2d73 796e 7461 782d  on:var(--syntax-
+00033f20: 6461 726b 2d64 6566 696e 6974 696f 6e29  dark-definition)
+00033f30: 3b2d 2d73 796e 7461 782d 7461 673a 7661  ;--syntax-tag:va
+00033f40: 7228 2d2d 7379 6e74 6178 2d64 6172 6b2d  r(--syntax-dark-
+00033f50: 7461 6729 3b2d 2d73 796e 7461 782d 6275  tag);--syntax-bu
+00033f60: 696c 7469 6e3a 7661 7228 2d2d 7379 6e74  iltin:var(--synt
+00033f70: 6178 2d64 6172 6b2d 6275 696c 7469 6e29  ax-dark-builtin)
+00033f80: 3b2d 2d73 796e 7461 782d 6b65 7977 6f72  ;--syntax-keywor
+00033f90: 643a 7661 7228 2d2d 7379 6e74 6178 2d64  d:var(--syntax-d
+00033fa0: 6172 6b2d 6b65 7977 6f72 6429 3b2d 2d73  ark-keyword);--s
+00033fb0: 796e 7461 782d 6578 6365 7074 696f 6e3a  yntax-exception:
+00033fc0: 7661 7228 2d2d 7379 6e74 6178 2d64 6172  var(--syntax-dar
+00033fd0: 6b2d 6578 6365 7074 696f 6e29 3b2d 2d73  k-exception);--s
+00033fe0: 796e 7461 782d 7374 7269 6e67 3a76 6172  yntax-string:var
+00033ff0: 282d 2d73 796e 7461 782d 6461 726b 2d73  (--syntax-dark-s
+00034000: 7472 696e 6729 3b2d 2d73 796e 7461 782d  tring);--syntax-
+00034010: 7265 6765 7870 3a76 6172 282d 2d73 796e  regexp:var(--syn
+00034020: 7461 782d 6461 726b 2d72 6567 6578 7029  tax-dark-regexp)
+00034030: 3b2d 2d73 796e 7461 782d 7661 7269 6162  ;--syntax-variab
+00034040: 6c65 3a76 6172 282d 2d73 796e 7461 782d  le:var(--syntax-
+00034050: 6461 726b 2d76 6172 6961 626c 6529 3b2d  dark-variable);-
+00034060: 2d73 796e 7461 782d 696e 7661 6c69 642d  -syntax-invalid-
+00034070: 696c 6c65 6761 6c2d 7465 7874 3a76 6172  illegal-text:var
+00034080: 282d 2d73 796e 7461 782d 6461 726b 2d69  (--syntax-dark-i
+00034090: 6e76 616c 6964 2d69 6c6c 6567 616c 2d74  nvalid-illegal-t
+000340a0: 6578 7429 3b2d 2d73 796e 7461 782d 696e  ext);--syntax-in
+000340b0: 7661 6c69 642d 696c 6c65 6761 6c2d 6267  valid-illegal-bg
+000340c0: 3a76 6172 282d 2d73 796e 7461 782d 6461  :var(--syntax-da
+000340d0: 726b 2d69 6e76 616c 6964 2d69 6c6c 6567  rk-invalid-illeg
+000340e0: 616c 2d62 6729 3b2d 2d73 796e 7461 782d  al-bg);--syntax-
+000340f0: 6d61 726b 7570 2d68 6561 6469 6e67 3a76  markup-heading:v
+00034100: 6172 282d 2d73 796e 7461 782d 6461 726b  ar(--syntax-dark
+00034110: 2d6d 6172 6b75 702d 6865 6164 696e 6729  -markup-heading)
+00034120: 3b2d 2d73 796e 7461 782d 6d61 726b 7570  ;--syntax-markup
+00034130: 2d69 7461 6c69 633a 7661 7228 2d2d 7379  -italic:var(--sy
+00034140: 6e74 6178 2d64 6172 6b2d 6d61 726b 7570  ntax-dark-markup
+00034150: 2d69 7461 6c69 6329 3b2d 2d73 796e 7461  -italic);--synta
+00034160: 782d 6d61 726b 7570 2d62 6f6c 643a 7661  x-markup-bold:va
+00034170: 7228 2d2d 7379 6e74 6178 2d64 6172 6b2d  r(--syntax-dark-
+00034180: 6d61 726b 7570 2d62 6f6c 6429 3b2d 2d73  markup-bold);--s
+00034190: 796e 7461 782d 6d61 726b 7570 2d64 656c  yntax-markup-del
+000341a0: 6574 6564 2d74 6578 743a 7661 7228 2d2d  eted-text:var(--
+000341b0: 7379 6e74 6178 2d64 6172 6b2d 6d61 726b  syntax-dark-mark
+000341c0: 7570 2d64 656c 6574 6564 2d74 6578 7429  up-deleted-text)
+000341d0: 3b2d 2d73 796e 7461 782d 6d61 726b 7570  ;--syntax-markup
+000341e0: 2d64 656c 6574 6564 2d62 673a 7661 7228  -deleted-bg:var(
+000341f0: 2d2d 7379 6e74 6178 2d64 6172 6b2d 6d61  --syntax-dark-ma
+00034200: 726b 7570 2d64 656c 6574 6564 2d62 6729  rkup-deleted-bg)
+00034210: 3b2d 2d73 796e 7461 782d 6d61 726b 7570  ;--syntax-markup
+00034220: 2d69 6e73 6572 7465 642d 7465 7874 3a76  -inserted-text:v
+00034230: 6172 282d 2d73 796e 7461 782d 6461 726b  ar(--syntax-dark
+00034240: 2d6d 6172 6b75 702d 696e 7365 7274 6564  -markup-inserted
+00034250: 2d74 6578 7429 3b2d 2d73 796e 7461 782d  -text);--syntax-
+00034260: 6d61 726b 7570 2d69 6e73 6572 7465 642d  markup-inserted-
+00034270: 6267 3a76 6172 282d 2d73 796e 7461 782d  bg:var(--syntax-
+00034280: 6461 726b 2d6d 6172 6b75 702d 696e 7365  dark-markup-inse
+00034290: 7274 6564 2d62 6729 3b2d 2d73 796e 7461  rted-bg);--synta
+000342a0: 782d 6d61 726b 7570 2d63 6861 6e67 6564  x-markup-changed
+000342b0: 2d74 6578 743a 7661 7228 2d2d 7379 6e74  -text:var(--synt
+000342c0: 6178 2d64 6172 6b2d 6d61 726b 7570 2d63  ax-dark-markup-c
+000342d0: 6861 6e67 6564 2d74 6578 7429 3b2d 2d73  hanged-text);--s
+000342e0: 796e 7461 782d 6d61 726b 7570 2d63 6861  yntax-markup-cha
+000342f0: 6e67 6564 2d62 673a 7661 7228 2d2d 7379  nged-bg:var(--sy
+00034300: 6e74 6178 2d64 6172 6b2d 6d61 726b 7570  ntax-dark-markup
+00034310: 2d63 6861 6e67 6564 2d62 6729 3b2d 2d73  -changed-bg);--s
+00034320: 796e 7461 782d 6d61 726b 7570 2d69 676e  yntax-markup-ign
+00034330: 6f72 6564 2d74 6578 743a 7661 7228 2d2d  ored-text:var(--
+00034340: 7379 6e74 6178 2d64 6172 6b2d 6d61 726b  syntax-dark-mark
+00034350: 7570 2d69 676e 6f72 6564 2d74 6578 7429  up-ignored-text)
+00034360: 3b2d 2d73 796e 7461 782d 6d61 726b 7570  ;--syntax-markup
+00034370: 2d69 676e 6f72 6564 2d62 673a 7661 7228  -ignored-bg:var(
+00034380: 2d2d 7379 6e74 6178 2d64 6172 6b2d 6d61  --syntax-dark-ma
+00034390: 726b 7570 2d69 676e 6f72 6564 2d62 6729  rkup-ignored-bg)
+000343a0: 3b2d 2d73 796e 7461 782d 6d65 7461 2d64  ;--syntax-meta-d
+000343b0: 6966 662d 7261 6e67 653a 7661 7228 2d2d  iff-range:var(--
+000343c0: 7379 6e74 6178 2d64 6172 6b2d 6d65 7461  syntax-dark-meta
+000343d0: 2d64 6966 662d 7261 6e67 6529 3b2d 2d73  -diff-range);--s
+000343e0: 796e 7461 782d 7370 6563 6961 6c2d 6267  yntax-special-bg
+000343f0: 3a76 6172 282d 2d73 796e 7461 782d 6461  :var(--syntax-da
+00034400: 726b 2d73 7065 6369 616c 2d62 6729 7d2e  rk-special-bg)}.
+00034410: 6c69 6768 7420 2e64 6172 6b2d 636f 6465  light .dark-code
+00034420: 7b2d 2d73 796e 7461 782d 7072 652d 6267  {--syntax-pre-bg
+00034430: 3a76 6172 282d 2d62 6c61 636b 2d61 3132  :var(--black-a12
+00034440: 293b 2d2d 7379 6e74 6178 2d63 6170 2d62  );--syntax-cap-b
+00034450: 673a 2331 6332 3032 343b 2d2d 7379 6e74  g:#1c2024;--synt
+00034460: 6178 2d68 6967 686c 6967 6874 2d62 673a  ax-highlight-bg:
+00034470: 7661 7228 2d2d 7768 6974 652d 6132 293b  var(--white-a2);
+00034480: 2d2d 7379 6e74 6178 2d6c 696e 656e 6f73  --syntax-linenos
+00034490: 2d64 6976 6964 6572 3a76 6172 282d 2d77  -divider:var(--w
+000344a0: 6869 7465 2d61 3429 3b2d 2d73 796e 7461  hite-a4);--synta
+000344b0: 782d 7465 7874 3a76 6172 282d 2d73 796e  x-text:var(--syn
+000344c0: 7461 782d 6461 726b 2d74 6578 7429 3b2d  tax-dark-text);-
+000344d0: 2d73 796e 7461 782d 6d65 7461 3a76 6172  -syntax-meta:var
+000344e0: 282d 2d73 796e 7461 782d 6461 726b 2d6d  (--syntax-dark-m
+000344f0: 6574 6129 3b2d 2d73 796e 7461 782d 636f  eta);--syntax-co
+00034500: 6d6d 656e 743a 7661 7228 2d2d 7379 6e74  mment:var(--synt
+00034510: 6178 2d64 6172 6b2d 636f 6d6d 656e 7429  ax-dark-comment)
+00034520: 3b2d 2d73 796e 7461 782d 636f 6e73 7461  ;--syntax-consta
+00034530: 6e74 3a76 6172 282d 2d73 796e 7461 782d  nt:var(--syntax-
+00034540: 6461 726b 2d63 6f6e 7374 616e 7429 3b2d  dark-constant);-
+00034550: 2d73 796e 7461 782d 656e 7469 7479 3a76  -syntax-entity:v
+00034560: 6172 282d 2d73 796e 7461 782d 6461 726b  ar(--syntax-dark
+00034570: 2d65 6e74 6974 7929 3b2d 2d73 796e 7461  -entity);--synta
+00034580: 782d 7072 6f70 6572 7479 3a76 6172 282d  x-property:var(-
+00034590: 2d73 796e 7461 782d 6461 726b 2d70 726f  -syntax-dark-pro
+000345a0: 7065 7274 7929 3b2d 2d73 796e 7461 782d  perty);--syntax-
+000345b0: 6465 6669 6e69 7469 6f6e 3a76 6172 282d  definition:var(-
+000345c0: 2d73 796e 7461 782d 6461 726b 2d64 6566  -syntax-dark-def
+000345d0: 696e 6974 696f 6e29 3b2d 2d73 796e 7461  inition);--synta
+000345e0: 782d 7461 673a 7661 7228 2d2d 7379 6e74  x-tag:var(--synt
+000345f0: 6178 2d64 6172 6b2d 7461 6729 3b2d 2d73  ax-dark-tag);--s
+00034600: 796e 7461 782d 6275 696c 7469 6e3a 7661  yntax-builtin:va
+00034610: 7228 2d2d 7379 6e74 6178 2d64 6172 6b2d  r(--syntax-dark-
+00034620: 6275 696c 7469 6e29 3b2d 2d73 796e 7461  builtin);--synta
+00034630: 782d 6b65 7977 6f72 643a 7661 7228 2d2d  x-keyword:var(--
+00034640: 7379 6e74 6178 2d64 6172 6b2d 6b65 7977  syntax-dark-keyw
+00034650: 6f72 6429 3b2d 2d73 796e 7461 782d 6578  ord);--syntax-ex
+00034660: 6365 7074 696f 6e3a 7661 7228 2d2d 7379  ception:var(--sy
+00034670: 6e74 6178 2d64 6172 6b2d 6578 6365 7074  ntax-dark-except
+00034680: 696f 6e29 3b2d 2d73 796e 7461 782d 7374  ion);--syntax-st
+00034690: 7269 6e67 3a76 6172 282d 2d73 796e 7461  ring:var(--synta
+000346a0: 782d 6461 726b 2d73 7472 696e 6729 3b2d  x-dark-string);-
+000346b0: 2d73 796e 7461 782d 7265 6765 7870 3a76  -syntax-regexp:v
+000346c0: 6172 282d 2d73 796e 7461 782d 6461 726b  ar(--syntax-dark
+000346d0: 2d72 6567 6578 7029 3b2d 2d73 796e 7461  -regexp);--synta
+000346e0: 782d 7661 7269 6162 6c65 3a76 6172 282d  x-variable:var(-
+000346f0: 2d73 796e 7461 782d 6461 726b 2d76 6172  -syntax-dark-var
+00034700: 6961 626c 6529 3b2d 2d73 796e 7461 782d  iable);--syntax-
+00034710: 696e 7661 6c69 642d 696c 6c65 6761 6c2d  invalid-illegal-
+00034720: 7465 7874 3a76 6172 282d 2d73 796e 7461  text:var(--synta
+00034730: 782d 6461 726b 2d69 6e76 616c 6964 2d69  x-dark-invalid-i
+00034740: 6c6c 6567 616c 2d74 6578 7429 3b2d 2d73  llegal-text);--s
+00034750: 796e 7461 782d 696e 7661 6c69 642d 696c  yntax-invalid-il
+00034760: 6c65 6761 6c2d 6267 3a76 6172 282d 2d73  legal-bg:var(--s
+00034770: 796e 7461 782d 6461 726b 2d69 6e76 616c  yntax-dark-inval
+00034780: 6964 2d69 6c6c 6567 616c 2d62 6729 3b2d  id-illegal-bg);-
+00034790: 2d73 796e 7461 782d 6d61 726b 7570 2d68  -syntax-markup-h
+000347a0: 6561 6469 6e67 3a76 6172 282d 2d73 796e  eading:var(--syn
+000347b0: 7461 782d 6461 726b 2d6d 6172 6b75 702d  tax-dark-markup-
+000347c0: 6865 6164 696e 6729 3b2d 2d73 796e 7461  heading);--synta
+000347d0: 782d 6d61 726b 7570 2d69 7461 6c69 633a  x-markup-italic:
+000347e0: 7661 7228 2d2d 7379 6e74 6178 2d64 6172  var(--syntax-dar
+000347f0: 6b2d 6d61 726b 7570 2d69 7461 6c69 6329  k-markup-italic)
+00034800: 3b2d 2d73 796e 7461 782d 6d61 726b 7570  ;--syntax-markup
+00034810: 2d62 6f6c 643a 7661 7228 2d2d 7379 6e74  -bold:var(--synt
+00034820: 6178 2d64 6172 6b2d 6d61 726b 7570 2d62  ax-dark-markup-b
+00034830: 6f6c 6429 3b2d 2d73 796e 7461 782d 6d61  old);--syntax-ma
+00034840: 726b 7570 2d64 656c 6574 6564 2d74 6578  rkup-deleted-tex
+00034850: 743a 7661 7228 2d2d 7379 6e74 6178 2d64  t:var(--syntax-d
+00034860: 6172 6b2d 6d61 726b 7570 2d64 656c 6574  ark-markup-delet
+00034870: 6564 2d74 6578 7429 3b2d 2d73 796e 7461  ed-text);--synta
+00034880: 782d 6d61 726b 7570 2d64 656c 6574 6564  x-markup-deleted
+00034890: 2d62 673a 7661 7228 2d2d 7379 6e74 6178  -bg:var(--syntax
+000348a0: 2d64 6172 6b2d 6d61 726b 7570 2d64 656c  -dark-markup-del
+000348b0: 6574 6564 2d62 6729 3b2d 2d73 796e 7461  eted-bg);--synta
+000348c0: 782d 6d61 726b 7570 2d69 6e73 6572 7465  x-markup-inserte
+000348d0: 642d 7465 7874 3a76 6172 282d 2d73 796e  d-text:var(--syn
+000348e0: 7461 782d 6461 726b 2d6d 6172 6b75 702d  tax-dark-markup-
+000348f0: 696e 7365 7274 6564 2d74 6578 7429 3b2d  inserted-text);-
+00034900: 2d73 796e 7461 782d 6d61 726b 7570 2d69  -syntax-markup-i
+00034910: 6e73 6572 7465 642d 6267 3a76 6172 282d  nserted-bg:var(-
+00034920: 2d73 796e 7461 782d 6461 726b 2d6d 6172  -syntax-dark-mar
+00034930: 6b75 702d 696e 7365 7274 6564 2d62 6729  kup-inserted-bg)
+00034940: 3b2d 2d73 796e 7461 782d 6d61 726b 7570  ;--syntax-markup
+00034950: 2d63 6861 6e67 6564 2d74 6578 743a 7661  -changed-text:va
+00034960: 7228 2d2d 7379 6e74 6178 2d64 6172 6b2d  r(--syntax-dark-
+00034970: 6d61 726b 7570 2d63 6861 6e67 6564 2d74  markup-changed-t
+00034980: 6578 7429 3b2d 2d73 796e 7461 782d 6d61  ext);--syntax-ma
+00034990: 726b 7570 2d63 6861 6e67 6564 2d62 673a  rkup-changed-bg:
+000349a0: 7661 7228 2d2d 7379 6e74 6178 2d64 6172  var(--syntax-dar
+000349b0: 6b2d 6d61 726b 7570 2d63 6861 6e67 6564  k-markup-changed
+000349c0: 2d62 6729 3b2d 2d73 796e 7461 782d 6d61  -bg);--syntax-ma
+000349d0: 726b 7570 2d69 676e 6f72 6564 2d74 6578  rkup-ignored-tex
+000349e0: 743a 7661 7228 2d2d 7379 6e74 6178 2d64  t:var(--syntax-d
+000349f0: 6172 6b2d 6d61 726b 7570 2d69 676e 6f72  ark-markup-ignor
+00034a00: 6564 2d74 6578 7429 3b2d 2d73 796e 7461  ed-text);--synta
+00034a10: 782d 6d61 726b 7570 2d69 676e 6f72 6564  x-markup-ignored
+00034a20: 2d62 673a 7661 7228 2d2d 7379 6e74 6178  -bg:var(--syntax
+00034a30: 2d64 6172 6b2d 6d61 726b 7570 2d69 676e  -dark-markup-ign
+00034a40: 6f72 6564 2d62 6729 3b2d 2d73 796e 7461  ored-bg);--synta
+00034a50: 782d 6d65 7461 2d64 6966 662d 7261 6e67  x-meta-diff-rang
+00034a60: 653a 7661 7228 2d2d 7379 6e74 6178 2d64  e:var(--syntax-d
+00034a70: 6172 6b2d 6d65 7461 2d64 6966 662d 7261  ark-meta-diff-ra
+00034a80: 6e67 6529 3b2d 2d73 796e 7461 782d 7370  nge);--syntax-sp
+00034a90: 6563 6961 6c2d 6267 3a76 6172 282d 2d73  ecial-bg:var(--s
+00034aa0: 796e 7461 782d 6461 726b 2d73 7065 6369  yntax-dark-speci
+00034ab0: 616c 2d62 6729 7d68 746d 6c2e 6c69 6768  al-bg)}html.ligh
+00034ac0: 7420 2e6a 7570 7974 6572 5f63 6f6e 7461  t .jupyter_conta
+00034ad0: 696e 6572 202e 6365 6c6c 5f6f 7574 7075  iner .cell_outpu
+00034ae0: 742c 6874 6d6c 2e6c 6967 6874 202e 7364  t,html.light .sd
+00034af0: 2d74 6162 2d63 6f6e 7465 6e74 7b2d 2d73  -tab-content{--s
+00034b00: 796e 7461 782d 7072 652d 6267 3a76 6172  yntax-pre-bg:var
+00034b10: 282d 2d63 6f6c 6f72 2d73 7572 6661 6365  (--color-surface
+00034b20: 2d61 6363 656e 7429 3b2d 2d73 796e 7461  -accent);--synta
+00034b30: 782d 6361 702d 6267 3a76 6172 282d 2d61  x-cap-bg:var(--a
+00034b40: 6363 656e 742d 3329 3b2d 2d73 796e 7461  ccent-3);--synta
+00034b50: 782d 6869 6768 6c69 6768 742d 6267 3a76  x-highlight-bg:v
+00034b60: 6172 282d 2d61 6363 656e 742d 6133 293b  ar(--accent-a3);
+00034b70: 2d2d 7379 6e74 6178 2d74 6578 743a 7661  --syntax-text:va
+00034b80: 7228 2d2d 7379 6e74 6178 2d6c 6967 6874  r(--syntax-light
+00034b90: 2d74 6578 7429 3b2d 2d73 796e 7461 782d  -text);--syntax-
+00034ba0: 6d65 7461 3a76 6172 282d 2d73 796e 7461  meta:var(--synta
+00034bb0: 782d 6c69 6768 742d 6d65 7461 293b 2d2d  x-light-meta);--
+00034bc0: 7379 6e74 6178 2d63 6f6d 6d65 6e74 3a76  syntax-comment:v
+00034bd0: 6172 282d 2d73 796e 7461 782d 6c69 6768  ar(--syntax-ligh
+00034be0: 742d 636f 6d6d 656e 7429 3b2d 2d73 796e  t-comment);--syn
+00034bf0: 7461 782d 636f 6e73 7461 6e74 3a76 6172  tax-constant:var
+00034c00: 282d 2d73 796e 7461 782d 6c69 6768 742d  (--syntax-light-
+00034c10: 636f 6e73 7461 6e74 293b 2d2d 7379 6e74  constant);--synt
+00034c20: 6178 2d65 6e74 6974 793a 7661 7228 2d2d  ax-entity:var(--
+00034c30: 7379 6e74 6178 2d6c 6967 6874 2d65 6e74  syntax-light-ent
+00034c40: 6974 7929 3b2d 2d73 796e 7461 782d 7072  ity);--syntax-pr
+00034c50: 6f70 6572 7479 3a76 6172 282d 2d73 796e  operty:var(--syn
+00034c60: 7461 782d 6c69 6768 742d 7072 6f70 6572  tax-light-proper
+00034c70: 7479 293b 2d2d 7379 6e74 6178 2d64 6566  ty);--syntax-def
+00034c80: 696e 6974 696f 6e3a 7661 7228 2d2d 7379  inition:var(--sy
+00034c90: 6e74 6178 2d6c 6967 6874 2d64 6566 696e  ntax-light-defin
+00034ca0: 6974 696f 6e29 3b2d 2d73 796e 7461 782d  ition);--syntax-
+00034cb0: 7461 673a 7661 7228 2d2d 7379 6e74 6178  tag:var(--syntax
+00034cc0: 2d6c 6967 6874 2d74 6167 293b 2d2d 7379  -light-tag);--sy
+00034cd0: 6e74 6178 2d62 7569 6c74 696e 3a76 6172  ntax-builtin:var
+00034ce0: 282d 2d73 796e 7461 782d 6c69 6768 742d  (--syntax-light-
+00034cf0: 6275 696c 7469 6e29 3b2d 2d73 796e 7461  builtin);--synta
+00034d00: 782d 6b65 7977 6f72 643a 7661 7228 2d2d  x-keyword:var(--
+00034d10: 7379 6e74 6178 2d6c 6967 6874 2d6b 6579  syntax-light-key
+00034d20: 776f 7264 293b 2d2d 7379 6e74 6178 2d65  word);--syntax-e
+00034d30: 7863 6570 7469 6f6e 3a76 6172 282d 2d73  xception:var(--s
+00034d40: 796e 7461 782d 6c69 6768 742d 6578 6365  yntax-light-exce
+00034d50: 7074 696f 6e29 3b2d 2d73 796e 7461 782d  ption);--syntax-
+00034d60: 7374 7269 6e67 3a76 6172 282d 2d73 796e  string:var(--syn
+00034d70: 7461 782d 6c69 6768 742d 7374 7269 6e67  tax-light-string
+00034d80: 293b 2d2d 7379 6e74 6178 2d72 6567 6578  );--syntax-regex
+00034d90: 703a 7661 7228 2d2d 7379 6e74 6178 2d6c  p:var(--syntax-l
+00034da0: 6967 6874 2d72 6567 6578 7029 3b2d 2d73  ight-regexp);--s
+00034db0: 796e 7461 782d 7661 7269 6162 6c65 3a76  yntax-variable:v
+00034dc0: 6172 282d 2d73 796e 7461 782d 6c69 6768  ar(--syntax-ligh
+00034dd0: 742d 7661 7269 6162 6c65 293b 2d2d 7379  t-variable);--sy
+00034de0: 6e74 6178 2d69 6e76 616c 6964 2d69 6c6c  ntax-invalid-ill
+00034df0: 6567 616c 2d74 6578 743a 7661 7228 2d2d  egal-text:var(--
+00034e00: 7379 6e74 6178 2d6c 6967 6874 2d69 6e76  syntax-light-inv
+00034e10: 616c 6964 2d69 6c6c 6567 616c 2d74 6578  alid-illegal-tex
+00034e20: 7429 3b2d 2d73 796e 7461 782d 696e 7661  t);--syntax-inva
+00034e30: 6c69 642d 696c 6c65 6761 6c2d 6267 3a76  lid-illegal-bg:v
+00034e40: 6172 282d 2d73 796e 7461 782d 6c69 6768  ar(--syntax-ligh
+00034e50: 742d 696e 7661 6c69 642d 696c 6c65 6761  t-invalid-illega
+00034e60: 6c2d 6267 293b 2d2d 7379 6e74 6178 2d6d  l-bg);--syntax-m
+00034e70: 6172 6b75 702d 6865 6164 696e 673a 7661  arkup-heading:va
+00034e80: 7228 2d2d 7379 6e74 6178 2d6c 6967 6874  r(--syntax-light
+00034e90: 2d6d 6172 6b75 702d 6865 6164 696e 6729  -markup-heading)
+00034ea0: 3b2d 2d73 796e 7461 782d 6d61 726b 7570  ;--syntax-markup
+00034eb0: 2d69 7461 6c69 633a 7661 7228 2d2d 7379  -italic:var(--sy
+00034ec0: 6e74 6178 2d6c 6967 6874 2d6d 6172 6b75  ntax-light-marku
+00034ed0: 702d 6974 616c 6963 293b 2d2d 7379 6e74  p-italic);--synt
+00034ee0: 6178 2d6d 6172 6b75 702d 626f 6c64 3a76  ax-markup-bold:v
+00034ef0: 6172 282d 2d73 796e 7461 782d 6c69 6768  ar(--syntax-ligh
+00034f00: 742d 6d61 726b 7570 2d62 6f6c 6429 3b2d  t-markup-bold);-
+00034f10: 2d73 796e 7461 782d 6d61 726b 7570 2d64  -syntax-markup-d
+00034f20: 656c 6574 6564 2d74 6578 743a 7661 7228  eleted-text:var(
+00034f30: 2d2d 7379 6e74 6178 2d6c 6967 6874 2d6d  --syntax-light-m
+00034f40: 6172 6b75 702d 6465 6c65 7465 642d 7465  arkup-deleted-te
+00034f50: 7874 293b 2d2d 7379 6e74 6178 2d6d 6172  xt);--syntax-mar
+00034f60: 6b75 702d 6465 6c65 7465 642d 6267 3a76  kup-deleted-bg:v
+00034f70: 6172 282d 2d73 796e 7461 782d 6c69 6768  ar(--syntax-ligh
+00034f80: 742d 6d61 726b 7570 2d64 656c 6574 6564  t-markup-deleted
+00034f90: 2d62 6729 3b2d 2d73 796e 7461 782d 6d61  -bg);--syntax-ma
+00034fa0: 726b 7570 2d69 6e73 6572 7465 642d 7465  rkup-inserted-te
+00034fb0: 7874 3a76 6172 282d 2d73 796e 7461 782d  xt:var(--syntax-
+00034fc0: 6c69 6768 742d 6d61 726b 7570 2d69 6e73  light-markup-ins
+00034fd0: 6572 7465 642d 7465 7874 293b 2d2d 7379  erted-text);--sy
+00034fe0: 6e74 6178 2d6d 6172 6b75 702d 696e 7365  ntax-markup-inse
+00034ff0: 7274 6564 2d62 673a 7661 7228 2d2d 7379  rted-bg:var(--sy
+00035000: 6e74 6178 2d6c 6967 6874 2d6d 6172 6b75  ntax-light-marku
+00035010: 702d 696e 7365 7274 6564 2d62 6729 3b2d  p-inserted-bg);-
+00035020: 2d73 796e 7461 782d 6d61 726b 7570 2d63  -syntax-markup-c
+00035030: 6861 6e67 6564 2d74 6578 743a 7661 7228  hanged-text:var(
+00035040: 2d2d 7379 6e74 6178 2d6c 6967 6874 2d6d  --syntax-light-m
+00035050: 6172 6b75 702d 6368 616e 6765 642d 7465  arkup-changed-te
+00035060: 7874 293b 2d2d 7379 6e74 6178 2d6d 6172  xt);--syntax-mar
+00035070: 6b75 702d 6368 616e 6765 642d 6267 3a76  kup-changed-bg:v
+00035080: 6172 282d 2d73 796e 7461 782d 6c69 6768  ar(--syntax-ligh
+00035090: 742d 6d61 726b 7570 2d63 6861 6e67 6564  t-markup-changed
+000350a0: 2d62 6729 3b2d 2d73 796e 7461 782d 6d61  -bg);--syntax-ma
+000350b0: 726b 7570 2d69 676e 6f72 6564 2d74 6578  rkup-ignored-tex
+000350c0: 743a 7661 7228 2d2d 7379 6e74 6178 2d6c  t:var(--syntax-l
+000350d0: 6967 6874 2d6d 6172 6b75 702d 6967 6e6f  ight-markup-igno
+000350e0: 7265 642d 7465 7874 293b 2d2d 7379 6e74  red-text);--synt
+000350f0: 6178 2d6d 6172 6b75 702d 6967 6e6f 7265  ax-markup-ignore
+00035100: 642d 6267 3a76 6172 282d 2d73 796e 7461  d-bg:var(--synta
+00035110: 782d 6c69 6768 742d 6d61 726b 7570 2d69  x-light-markup-i
+00035120: 676e 6f72 6564 2d62 6729 3b2d 2d73 796e  gnored-bg);--syn
+00035130: 7461 782d 6d65 7461 2d64 6966 662d 7261  tax-meta-diff-ra
+00035140: 6e67 653a 7661 7228 2d2d 7379 6e74 6178  nge:var(--syntax
+00035150: 2d6c 6967 6874 2d6d 6574 612d 6469 6666  -light-meta-diff
+00035160: 2d72 616e 6765 293b 2d2d 7379 6e74 6178  -range);--syntax
+00035170: 2d68 6967 686c 6967 6874 2d62 673a 7661  -highlight-bg:va
+00035180: 7228 2d2d 7379 6e74 6178 2d6c 6967 6874  r(--syntax-light
+00035190: 2d68 6967 686c 6967 6874 2d62 6729 3b2d  -highlight-bg);-
+000351a0: 2d73 796e 7461 782d 7370 6563 6961 6c2d  -syntax-special-
+000351b0: 6267 3a76 6172 282d 2d73 796e 7461 782d  bg:var(--syntax-
+000351c0: 6c69 6768 742d 7370 6563 6961 6c2d 6267  light-special-bg
+000351d0: 297d 2e73 792d 6c73 6964 657b 2d2d 6865  )}.sy-lside{--he
+000351e0: 6967 6874 3a34 3270 787d 2e73 792d 6c73  ight:42px}.sy-ls
+000351f0: 6964 652d 626f 7474 6f6d 7b70 6f73 6974  ide-bottom{posit
+00035200: 696f 6e3a 7374 6963 6b79 3b62 6f74 746f  ion:sticky;botto
+00035210: 6d3a 303b 7061 6464 696e 673a 303b 626f  m:0;padding:0;bo
+00035220: 7264 6572 2d74 6f70 3a31 7078 2073 6f6c  rder-top:1px sol
+00035230: 6964 2076 6172 282d 2d73 792d 632d 6469  id var(--sy-c-di
+00035240: 7669 6465 7229 3b62 6163 6b67 726f 756e  vider);backgroun
+00035250: 642d 636f 6c6f 723a 7661 7228 2d2d 7379  d-color:var(--sy
+00035260: 2d63 2d62 6163 6b67 726f 756e 6429 3b2d  -c-background);-
+00035270: 2d74 772d 7368 6164 6f77 3a30 202d 3132  -tw-shadow:0 -12
+00035280: 7078 2031 3670 7820 7661 7228 2d2d 7379  px 16px var(--sy
+00035290: 2d63 2d62 6163 6b67 726f 756e 6429 3b62  -c-background);b
+000352a0: 6f78 2d73 6861 646f 773a 7661 7228 2d2d  ox-shadow:var(--
+000352b0: 7477 2d72 696e 672d 6f66 6673 6574 2d73  tw-ring-offset-s
+000352c0: 6861 646f 772c 3020 3020 2330 3030 3029  hadow,0 0 #0000)
+000352d0: 2c76 6172 282d 2d74 772d 7269 6e67 2d73  ,var(--tw-ring-s
+000352e0: 6861 646f 772c 3020 3020 2330 3030 3029  hadow,0 0 #0000)
+000352f0: 2c76 6172 282d 2d74 772d 7368 6164 6f77  ,var(--tw-shadow
+00035300: 297d 2e73 792d 6c73 6964 6520 2e72 7374  )}.sy-lside .rst
+00035310: 2d76 6572 7369 6f6e 737b 706f 7369 7469  -versions{positi
+00035320: 6f6e 3a73 7461 7469 633b 7769 6474 683a  on:static;width:
+00035330: 3130 3025 3b62 6163 6b67 726f 756e 642d  100%;background-
+00035340: 636f 6c6f 723a 7661 7228 2d2d 7379 2d63  color:var(--sy-c
+00035350: 2d73 7572 6661 6365 293b 666f 6e74 2d66  -surface);font-f
+00035360: 616d 696c 793a 7661 7228 2d2d 7379 2d66  amily:var(--sy-f
+00035370: 2d74 6578 7429 7d2e 7379 2d6c 7369 6465  -text)}.sy-lside
+00035380: 202e 7273 742d 7665 7273 696f 6e73 2061   .rst-versions a
+00035390: 7b63 6f6c 6f72 3a76 6172 282d 2d73 792d  {color:var(--sy-
+000353a0: 632d 6c69 6e6b 297d 2e73 792d 6c73 6964  c-link)}.sy-lsid
+000353b0: 6520 2e72 7374 2d76 6572 7369 6f6e 7320  e .rst-versions 
+000353c0: 613a 686f 7665 727b 636f 6c6f 723a 7661  a:hover{color:va
+000353d0: 7228 2d2d 7379 2d63 2d6c 696e 6b2d 686f  r(--sy-c-link-ho
+000353e0: 7665 7229 7d2e 7379 2d6c 7369 6465 202e  ver)}.sy-lside .
+000353f0: 7273 742d 7665 7273 696f 6e73 202e 7273  rst-versions .rs
+00035400: 742d 6375 7272 656e 742d 7665 7273 696f  t-current-versio
+00035410: 6e7b 6261 636b 6772 6f75 6e64 2d63 6f6c  n{background-col
+00035420: 6f72 3a76 6172 282d 2d73 792d 632d 6261  or:var(--sy-c-ba
+00035430: 636b 6772 6f75 6e64 293b 636f 6c6f 723a  ckground);color:
+00035440: 7661 7228 2d2d 7379 2d63 2d74 6578 7429  var(--sy-c-text)
+00035450: 3b70 6164 6469 6e67 3a30 2031 7265 6d3b  ;padding:0 1rem;
+00035460: 6865 6967 6874 3a76 6172 282d 2d68 6569  height:var(--hei
+00035470: 6768 7429 3b6c 696e 652d 6865 6967 6874  ght);line-height
+00035480: 3a76 6172 282d 2d68 6569 6768 7429 7d2e  :var(--height)}.
+00035490: 7379 2d6c 7369 6465 202e 7273 742d 7665  sy-lside .rst-ve
+000354a0: 7273 696f 6e73 2e72 7374 2d62 6164 6765  rsions.rst-badge
+000354b0: 202e 7273 742d 6375 7272 656e 742d 7665   .rst-current-ve
+000354c0: 7273 696f 6e7b 7465 7874 2d61 6c69 676e  rsion{text-align
+000354d0: 3a6c 6566 743b 666f 6e74 2d73 697a 653a  :left;font-size:
+000354e0: 2e39 3472 656d 3b70 6164 6469 6e67 3a30  .94rem;padding:0
+000354f0: 2031 7265 6d3b 6865 6967 6874 3a76 6172   1rem;height:var
+00035500: 282d 2d68 6569 6768 7429 3b6c 696e 652d  (--height);line-
+00035510: 6865 6967 6874 3a76 6172 282d 2d68 6569  height:var(--hei
+00035520: 6768 7429 7d2e 7379 2d6c 7369 6465 202e  ght)}.sy-lside .
+00035530: 7273 742d 7665 7273 696f 6e73 202e 7273  rst-versions .rs
+00035540: 742d 6375 7272 656e 742d 7665 7273 696f  t-current-versio
+00035550: 6e20 2e66 617b 636f 6c6f 723a 7661 7228  n .fa{color:var(
+00035560: 2d2d 7379 2d63 2d74 6578 7429 7d2e 7379  --sy-c-text)}.sy
+00035570: 2d6c 7369 6465 202e 7273 742d 7665 7273  -lside .rst-vers
+00035580: 696f 6e73 2e72 7374 2d62 6164 6765 2e73  ions.rst-badge.s
+00035590: 6869 6674 2d75 7020 2e72 7374 2d63 7572  hift-up .rst-cur
+000355a0: 7265 6e74 2d76 6572 7369 6f6e 7b74 6578  rent-version{tex
+000355b0: 742d 616c 6967 6e3a 6c65 6674 7d2e 7379  t-align:left}.sy
+000355c0: 2d6c 7369 6465 202e 7273 742d 7665 7273  -lside .rst-vers
+000355d0: 696f 6e73 2e72 7374 2d62 6164 6765 2e73  ions.rst-badge.s
+000355e0: 6869 6674 2d75 7020 2e72 7374 2d63 7572  hift-up .rst-cur
+000355f0: 7265 6e74 2d76 6572 7369 6f6e 202e 6661  rent-version .fa
+00035600: 2d62 6f6f 6b7b 666c 6f61 743a 6e6f 6e65  -book{float:none
+00035610: 7d2e 7379 2d6c 7369 6465 202e 7273 742d  }.sy-lside .rst-
+00035620: 6f74 6865 722d 7665 7273 696f 6e73 7b66  other-versions{f
+00035630: 6f6e 742d 7369 7a65 3a2e 3836 7265 6d3b  ont-size:.86rem;
+00035640: 626f 7264 6572 2d74 6f70 3a31 7078 2073  border-top:1px s
+00035650: 6f6c 6964 2076 6172 282d 2d73 792d 632d  olid var(--sy-c-
+00035660: 6469 7669 6465 7229 7d2e 7379 2d6c 7369  divider)}.sy-lsi
+00035670: 6465 202e 7273 742d 6f74 6865 722d 7665  de .rst-other-ve
+00035680: 7273 696f 6e73 2064 747b 666f 6e74 2d73  rsions dt{font-s
+00035690: 697a 653a 2e36 3872 656d 3b66 6f6e 742d  ize:.68rem;font-
+000356a0: 7765 6967 6874 3a35 3030 3b70 6164 6469  weight:500;paddi
+000356b0: 6e67 3a34 7078 2036 7078 3b63 6f6c 6f72  ng:4px 6px;color
+000356c0: 3a76 6172 282d 2d73 792d 632d 6c69 6768  :var(--sy-c-ligh
+000356d0: 7429 7d2e 7379 2d6c 7369 6465 202e 7273  t)}.sy-lside .rs
+000356e0: 742d 7665 7273 696f 6e73 202e 7273 742d  t-versions .rst-
+000356f0: 6f74 6865 722d 7665 7273 696f 6e73 2064  other-versions d
+00035700: 6420 617b 636f 6c6f 723a 7661 7228 2d2d  d a{color:var(--
+00035710: 7379 2d63 2d74 6578 7429 7d2e 7379 2d6c  sy-c-text)}.sy-l
+00035720: 7369 6465 202e 7273 742d 7665 7273 696f  side .rst-versio
+00035730: 6e73 202e 7273 742d 6f74 6865 722d 7665  ns .rst-other-ve
+00035740: 7273 696f 6e73 2064 6420 613a 686f 7665  rsions dd a:hove
+00035750: 727b 7465 7874 2d64 6563 6f72 6174 696f  r{text-decoratio
+00035760: 6e3a 756e 6465 726c 696e 653b 636f 6c6f  n:underline;colo
+00035770: 723a 7661 7228 2d2d 7379 2d63 2d6c 696e  r:var(--sy-c-lin
+00035780: 6b2d 686f 7665 7229 7d2e 7379 2d6c 7369  k-hover)}.sy-lsi
+00035790: 6465 202e 7273 742d 7665 7273 696f 6e73  de .rst-versions
+000357a0: 2069 6e70 7574 7b77 6964 7468 3a31 3030   input{width:100
+000357b0: 253b 7061 6464 696e 673a 3670 7820 3132  %;padding:6px 12
+000357c0: 7078 3b66 6f6e 742d 7369 7a65 3a2e 3932  px;font-size:.92
+000357d0: 7265 6d3b 666f 6e74 2d66 616d 696c 793a  rem;font-family:
+000357e0: 7661 7228 2d2d 7379 2d66 2d74 6578 7429  var(--sy-f-text)
+000357f0: 3b62 6f72 6465 722d 7261 6469 7573 3a36  ;border-radius:6
+00035800: 7078 3b6f 7574 6c69 6e65 3a30 3b62 6163  px;outline:0;bac
+00035810: 6b67 726f 756e 643a 7661 7228 2d2d 7379  kground:var(--sy
+00035820: 2d63 2d62 6163 6b67 726f 756e 6429 3b62  -c-background);b
+00035830: 6f72 6465 723a 3170 7820 736f 6c69 6420  order:1px solid 
+00035840: 7661 7228 2d2d 7379 2d63 2d62 6f72 6465  var(--sy-c-borde
+00035850: 7229 7d2e 7379 2d6c 7369 6465 202e 7273  r)}.sy-lside .rs
+00035860: 742d 7665 7273 696f 6e73 202e 7273 742d  t-versions .rst-
+00035870: 6f74 6865 722d 7665 7273 696f 6e73 2068  other-versions h
+00035880: 727b 626f 7264 6572 2d63 6f6c 6f72 3a76  r{border-color:v
+00035890: 6172 282d 2d73 792d 632d 6469 7669 6465  ar(--sy-c-divide
+000358a0: 7229 7d40 6d65 6469 6120 286d 696e 2d77  r)}@media (min-w
+000358b0: 6964 7468 3a39 3072 656d 297b 2e73 792d  idth:90rem){.sy-
+000358c0: 6c73 6964 6520 2e72 7374 2d76 6572 7369  lside .rst-versi
+000358d0: 6f6e 737b 6261 636b 6772 6f75 6e64 3a76  ons{background:v
+000358e0: 6172 282d 2d73 792d 632d 6261 636b 6772  ar(--sy-c-backgr
+000358f0: 6f75 6e64 297d 7d2e 7975 6520 6275 7474  ound)}}.yue butt
+00035900: 6f6e 2e63 6f70 7962 746e 7b61 6c69 676e  on.copybtn{align
+00035910: 2d69 7465 6d73 3a63 656e 7465 723b 6a75  -items:center;ju
+00035920: 7374 6966 792d 636f 6e74 656e 743a 6365  stify-content:ce
+00035930: 6e74 6572 3b62 6163 6b67 726f 756e 642d  nter;background-
+00035940: 636f 6c6f 723a 696e 6974 6961 6c3b 626f  color:initial;bo
+00035950: 7264 6572 3a6e 6f6e 653b 636f 6c6f 723a  rder:none;color:
+00035960: 7661 7228 2d2d 7379 6e74 6178 2d74 6578  var(--syntax-tex
+00035970: 7429 7d2e 7975 6520 6275 7474 6f6e 2e63  t)}.yue button.c
+00035980: 6f70 7962 746e 3e73 7667 7b77 6964 7468  opybtn>svg{width
+00035990: 3a31 2e34 7265 6d3b 6865 6967 6874 3a31  :1.4rem;height:1
+000359a0: 2e34 7265 6d7d 2e79 7565 2062 7574 746f  .4rem}.yue butto
+000359b0: 6e2e 636f 7079 6274 6e3a 686f 7665 727b  n.copybtn:hover{
+000359c0: 636f 6c6f 723a 7661 7228 2d2d 7379 6e74  color:var(--synt
+000359d0: 6178 2d6d 6574 6129 7d2e 7975 6520 2e68  ax-meta)}.yue .h
+000359e0: 6967 686c 6967 6874 2062 7574 746f 6e2e  ighlight button.
+000359f0: 636f 7079 6274 6e3a 686f 7665 727b 6261  copybtn:hover{ba
+00035a00: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3a69  ckground-color:i
+00035a10: 6e69 7469 616c 7d2e 7975 6520 6275 7474  nitial}.yue butt
+00035a20: 6f6e 2e63 6f70 7962 746e 3a61 6674 6572  on.copybtn:after
+00035a30: 7b62 6163 6b67 726f 756e 642d 636f 6c6f  {background-colo
+00035a40: 723a 696e 6974 6961 6c3b 636f 6c6f 723a  r:initial;color:
+00035a50: 7661 7228 2d2d 7379 6e74 6178 2d74 6578  var(--syntax-tex
+00035a60: 7429 7d2e 7975 6520 6275 7474 6f6e 2e63  t)}.yue button.c
+00035a70: 6f70 7962 746e 2e73 7563 6365 7373 7b62  opybtn.success{b
+00035a80: 6f72 6465 722d 636f 6c6f 723a 7661 7228  order-color:var(
+00035a90: 2d2d 6772 6565 6e2d 6131 3029 3b63 6f6c  --green-a10);col
+00035aa0: 6f72 3a76 6172 282d 2d67 7265 656e 2d61  or:var(--green-a
+00035ab0: 3130 297d 2e79 7565 2062 7574 746f 6e2e  10)}.yue button.
+00035ac0: 636f 7079 6274 6e2e 7375 6363 6573 733a  copybtn.success:
+00035ad0: 6166 7465 727b 636f 6c6f 723a 7661 7228  after{color:var(
+00035ae0: 2d2d 6772 6565 6e2d 6131 3029 7d2e 7975  --green-a10)}.yu
+00035af0: 657b 2d2d 7364 2d63 6f6c 6f72 2d70 7269  e{--sd-color-pri
+00035b00: 6d61 7279 3a76 6172 282d 2d61 6363 656e  mary:var(--accen
+00035b10: 742d 6131 3129 3b2d 2d73 642d 636f 6c6f  t-a11);--sd-colo
+00035b20: 722d 7365 636f 6e64 6172 793a 7661 7228  r-secondary:var(
+00035b30: 2d2d 676f 6c64 2d61 3131 293b 2d2d 7364  --gold-a11);--sd
+00035b40: 2d63 6f6c 6f72 2d73 7563 6365 7373 3a76  -color-success:v
+00035b50: 6172 282d 2d67 7265 656e 2d61 3131 293b  ar(--green-a11);
+00035b60: 2d2d 7364 2d63 6f6c 6f72 2d69 6e66 6f3a  --sd-color-info:
+00035b70: 7661 7228 2d2d 626c 7565 2d61 3131 293b  var(--blue-a11);
+00035b80: 2d2d 7364 2d63 6f6c 6f72 2d77 6172 6e69  --sd-color-warni
+00035b90: 6e67 3a76 6172 282d 2d6f 7261 6e67 652d  ng:var(--orange-
+00035ba0: 6131 3129 3b2d 2d73 642d 636f 6c6f 722d  a11);--sd-color-
+00035bb0: 6461 6e67 6572 3a76 6172 282d 2d72 6564  danger:var(--red
+00035bc0: 2d61 3131 293b 2d2d 7364 2d63 6f6c 6f72  -a11);--sd-color
+00035bd0: 2d6c 6967 6874 3a76 6172 282d 2d73 616e  -light:var(--san
+00035be0: 642d 6132 293b 2d2d 7364 2d63 6f6c 6f72  d-a2);--sd-color
+00035bf0: 2d6d 7574 6564 3a76 6172 282d 2d67 7261  -muted:var(--gra
+00035c00: 792d 3829 3b2d 2d73 642d 636f 6c6f 722d  y-8);--sd-color-
+00035c10: 6461 726b 3a23 3231 3231 3232 3b2d 2d73  dark:#212122;--s
+00035c20: 642d 636f 6c6f 722d 626c 6163 6b3a 2330  d-color-black:#0
+00035c30: 3030 3b2d 2d73 642d 636f 6c6f 722d 7768  00;--sd-color-wh
+00035c40: 6974 653a 2366 6666 3b2d 2d73 642d 636f  ite:#fff;--sd-co
+00035c50: 6c6f 722d 7072 696d 6172 792d 6869 6768  lor-primary-high
+00035c60: 6c69 6768 743a 7661 7228 2d2d 6163 6365  light:var(--acce
+00035c70: 6e74 2d61 3829 3b2d 2d73 642d 636f 6c6f  nt-a8);--sd-colo
+00035c80: 722d 7365 636f 6e64 6172 792d 6869 6768  r-secondary-high
+00035c90: 6c69 6768 743a 7661 7228 2d2d 676f 6c64  light:var(--gold
+00035ca0: 2d61 3829 3b2d 2d73 642d 636f 6c6f 722d  -a8);--sd-color-
+00035cb0: 7375 6363 6573 732d 6869 6768 6c69 6768  success-highligh
+00035cc0: 743a 7661 7228 2d2d 6772 6565 6e2d 6138  t:var(--green-a8
+00035cd0: 293b 2d2d 7364 2d63 6f6c 6f72 2d69 6e66  );--sd-color-inf
+00035ce0: 6f2d 6869 6768 6c69 6768 743a 7661 7228  o-highlight:var(
+00035cf0: 2d2d 626c 7565 2d61 3829 3b2d 2d73 642d  --blue-a8);--sd-
+00035d00: 636f 6c6f 722d 7761 726e 696e 672d 6869  color-warning-hi
+00035d10: 6768 6c69 6768 743a 7661 7228 2d2d 6f72  ghlight:var(--or
+00035d20: 616e 6765 2d61 3829 3b2d 2d73 642d 636f  ange-a8);--sd-co
+00035d30: 6c6f 722d 6461 6e67 6572 2d68 6967 686c  lor-danger-highl
+00035d40: 6967 6874 3a76 6172 282d 2d72 6564 2d61  ight:var(--red-a
+00035d50: 3829 3b2d 2d73 642d 636f 6c6f 722d 6c69  8);--sd-color-li
+00035d60: 6768 742d 6869 6768 6c69 6768 743a 7661  ght-highlight:va
+00035d70: 7228 2d2d 6772 6179 2d34 293b 2d2d 7364  r(--gray-4);--sd
+00035d80: 2d63 6f6c 6f72 2d6d 7574 6564 2d68 6967  -color-muted-hig
+00035d90: 686c 6967 6874 3a76 6172 282d 2d67 7261  hlight:var(--gra
+00035da0: 792d 3131 293b 2d2d 7364 2d63 6f6c 6f72  y-11);--sd-color
+00035db0: 2d64 6172 6b2d 6869 6768 6c69 6768 743a  -dark-highlight:
+00035dc0: 2331 3231 3231 313b 2d2d 7364 2d63 6f6c  #121211;--sd-col
+00035dd0: 6f72 2d62 6c61 636b 2d68 6967 686c 6967  or-black-highlig
+00035de0: 6874 3a23 3030 303b 2d2d 7364 2d63 6f6c  ht:#000;--sd-col
+00035df0: 6f72 2d77 6869 7465 2d68 6967 686c 6967  or-white-highlig
+00035e00: 6874 3a23 6439 6439 6439 3b2d 2d73 642d  ht:#d9d9d9;--sd-
+00035e10: 636f 6c6f 722d 7072 696d 6172 792d 7465  color-primary-te
+00035e20: 7874 3a76 6172 282d 2d61 6363 656e 742d  xt:var(--accent-
+00035e30: 392d 636f 6e74 7261 7374 293b 2d2d 7364  9-contrast);--sd
+00035e40: 2d63 6f6c 6f72 2d73 6563 6f6e 6461 7279  -color-secondary
+00035e50: 2d74 6578 743a 7661 7228 2d2d 676f 6c64  -text:var(--gold
+00035e60: 2d39 2d63 6f6e 7472 6173 7429 3b2d 2d73  -9-contrast);--s
+00035e70: 642d 636f 6c6f 722d 7375 6363 6573 732d  d-color-success-
+00035e80: 7465 7874 3a76 6172 282d 2d67 7265 656e  text:var(--green
+00035e90: 2d39 2d63 6f6e 7472 6173 7429 3b2d 2d73  -9-contrast);--s
+00035ea0: 642d 636f 6c6f 722d 696e 666f 2d74 6578  d-color-info-tex
+00035eb0: 743a 7661 7228 2d2d 626c 7565 2d39 2d63  t:var(--blue-9-c
+00035ec0: 6f6e 7472 6173 7429 3b2d 2d73 642d 636f  ontrast);--sd-co
+00035ed0: 6c6f 722d 7761 726e 696e 672d 7465 7874  lor-warning-text
+00035ee0: 3a76 6172 282d 2d6f 7261 6e67 652d 392d  :var(--orange-9-
+00035ef0: 636f 6e74 7261 7374 293b 2d2d 7364 2d63  contrast);--sd-c
+00035f00: 6f6c 6f72 2d64 616e 6765 722d 7465 7874  olor-danger-text
+00035f10: 3a76 6172 282d 2d72 6564 2d39 2d63 6f6e  :var(--red-9-con
+00035f20: 7472 6173 7429 3b2d 2d73 642d 636f 6c6f  trast);--sd-colo
+00035f30: 722d 6c69 6768 742d 7465 7874 3a76 6172  r-light-text:var
+00035f40: 282d 2d73 792d 632d 7465 7874 293b 2d2d  (--sy-c-text);--
+00035f50: 7364 2d63 6f6c 6f72 2d6d 7574 6564 2d74  sd-color-muted-t
+00035f60: 6578 743a 2366 6666 3b2d 2d73 642d 636f  ext:#fff;--sd-co
+00035f70: 6c6f 722d 6461 726b 2d74 6578 743a 2366  lor-dark-text:#f
+00035f80: 6666 3b2d 2d73 642d 636f 6c6f 722d 626c  ff;--sd-color-bl
+00035f90: 6163 6b2d 7465 7874 3a23 6666 663b 2d2d  ack-text:#fff;--
+00035fa0: 7364 2d63 6f6c 6f72 2d77 6869 7465 2d74  sd-color-white-t
+00035fb0: 6578 743a 2332 3132 3532 393b 2d2d 7364  ext:#212529;--sd
+00035fc0: 2d63 6f6c 6f72 2d73 6861 646f 773a 7661  -color-shadow:va
+00035fd0: 7228 2d2d 6772 6179 2d31 293b 2d2d 7364  r(--gray-1);--sd
+00035fe0: 2d63 6f6c 6f72 2d63 6172 642d 626f 7264  -color-card-bord
+00035ff0: 6572 3a76 6172 282d 2d73 792d 632d 626f  er:var(--sy-c-bo
+00036000: 7264 6572 293b 2d2d 7364 2d63 6f6c 6f72  rder);--sd-color
+00036010: 2d63 6172 642d 626f 7264 6572 2d68 6f76  -card-border-hov
+00036020: 6572 3a76 6172 282d 2d61 6363 656e 742d  er:var(--accent-
+00036030: 6139 293b 2d2d 7364 2d63 6f6c 6f72 2d74  a9);--sd-color-t
+00036040: 6162 732d 6c61 6265 6c2d 696e 6163 7469  abs-label-inacti
+00036050: 7665 3a76 6172 282d 2d73 792d 632d 626f  ve:var(--sy-c-bo
+00036060: 6c64 293b 2d2d 7364 2d63 6f6c 6f72 2d74  ld);--sd-color-t
+00036070: 6162 732d 6c61 6265 6c2d 6163 7469 7665  abs-label-active
+00036080: 3a76 6172 282d 2d73 642d 636f 6c6f 722d  :var(--sd-color-
+00036090: 7072 696d 6172 7929 3b2d 2d73 642d 636f  primary);--sd-co
+000360a0: 6c6f 722d 7461 6273 2d75 6e64 6572 6c69  lor-tabs-underli
+000360b0: 6e65 2d61 6374 6976 653a 7661 7228 2d2d  ne-active:var(--
+000360c0: 7364 2d63 6f6c 6f72 2d70 7269 6d61 7279  sd-color-primary
+000360d0: 293b 2d2d 7364 2d63 6f6c 6f72 2d74 6162  );--sd-color-tab
+000360e0: 732d 6c61 6265 6c2d 686f 7665 723a 7661  s-label-hover:va
+000360f0: 7228 2d2d 6163 6365 6e74 2d39 293b 2d2d  r(--accent-9);--
+00036100: 7364 2d63 6f6c 6f72 2d74 6162 732d 756e  sd-color-tabs-un
+00036110: 6465 726c 696e 652d 686f 7665 723a 7661  derline-hover:va
+00036120: 7228 2d2d 6163 6365 6e74 2d39 297d 2e79  r(--accent-9)}.y
+00036130: 7565 202e 7375 7266 6163 657b 2d2d 7364  ue .surface{--sd
+00036140: 2d63 6f6c 6f72 2d63 6172 642d 7465 7874  -color-card-text
+00036150: 3a76 6172 282d 2d73 792d 632d 6c69 6768  :var(--sy-c-ligh
+00036160: 7429 3b2d 2d73 642d 636f 6c6f 722d 6361  t);--sd-color-ca
+00036170: 7264 2d62 6f72 6465 723a 2330 3030 303b  rd-border:#0000;
+00036180: 2d2d 7364 2d63 6f6c 6f72 2d63 6172 642d  --sd-color-card-
+00036190: 6261 636b 6772 6f75 6e64 3a76 6172 282d  background:var(-
+000361a0: 2d73 792d 632d 7375 7266 6163 6529 7d2e  -sy-c-surface)}.
+000361b0: 7975 6520 612e 7364 2d62 6164 6765 2c2e  yue a.sd-badge,.
+000361c0: 7975 6520 612e 7364 2d62 6164 6765 3a68  yue a.sd-badge:h
+000361d0: 6f76 6572 7b62 6f72 6465 722d 626f 7474  over{border-bott
+000361e0: 6f6d 3a30 7d2e 7975 6520 2e73 642d 6261  om:0}.yue .sd-ba
+000361f0: 6467 657b 666f 6e74 2d77 6569 6768 743a  dge{font-weight:
+00036200: 3630 303b 626f 7264 6572 2d72 6164 6975  600;border-radiu
+00036210: 733a 3370 787d 2e79 7565 202e 7364 2d62  s:3px}.yue .sd-b
+00036220: 746e 7b62 6f72 6465 722d 636f 6c6f 723a  tn{border-color:
+00036230: 7661 7228 2d2d 7379 2d63 2d62 6f72 6465  var(--sy-c-borde
+00036240: 7229 7d2e 7975 6520 2e73 642d 7461 622d  r)}.yue .sd-tab-
+00036250: 7365 743e 6c61 6265 6c7b 7061 6464 696e  set>label{paddin
+00036260: 673a 3172 656d 202e 3235 7265 6d20 2e35  g:1rem .25rem .5
+00036270: 7265 6d3b 666f 6e74 2d73 697a 653a 2e38  rem;font-size:.8
+00036280: 3472 656d 3b66 6f6e 742d 7765 6967 6874  4rem;font-weight
+00036290: 3a35 3030 7d2e 7975 6520 2e73 642d 7461  :500}.yue .sd-ta
+000362a0: 622d 7365 743e 6c61 6265 6c7e 6c61 6265  b-set>label~labe
+000362b0: 6c7b 6d61 7267 696e 2d6c 6566 743a 3172  l{margin-left:1r
+000362c0: 656d 7d2e 7975 6520 2e73 642d 7461 622d  em}.yue .sd-tab-
+000362d0: 636f 6e74 656e 747b 7061 6464 696e 673a  content{padding:
+000362e0: 303b 626f 782d 7368 6164 6f77 3a30 202d  0;box-shadow:0 -
+000362f0: 2e30 3632 3572 656d 2076 6172 282d 2d73  .0625rem var(--s
+00036300: 792d 632d 6469 7669 6465 7229 7d2e 7975  y-c-divider)}.yu
+00036310: 6520 2e73 642d 7461 622d 636f 6e74 656e  e .sd-tab-conten
+00036320: 7420 2e63 6f64 652d 626c 6f63 6b2d 6361  t .code-block-ca
+00036330: 7074 696f 6e2c 2e79 7565 202e 7364 2d74  ption,.yue .sd-t
+00036340: 6162 2d63 6f6e 7465 6e74 202e 6869 6768  ab-content .high
+00036350: 6c69 6768 7420 7072 657b 626f 7264 6572  light pre{border
+00036360: 2d72 6164 6975 733a 307d 2e79 7565 202e  -radius:0}.yue .
+00036370: 7364 2d63 6172 642d 7469 746c 657b 636f  sd-card-title{co
+00036380: 6c6f 723a 7661 7228 2d2d 7379 2d63 2d74  lor:var(--sy-c-t
+00036390: 6578 7429 7d2e 7975 6520 2e73 642d 6361  ext)}.yue .sd-ca
+000363a0: 7264 2d74 6974 6c65 3e73 7667 7b70 6f73  rd-title>svg{pos
+000363b0: 6974 696f 6e3a 7265 6c61 7469 7665 3b74  ition:relative;t
+000363c0: 6f70 3a2d 3170 783b 6d61 7267 696e 2d72  op:-1px;margin-r
+000363d0: 6967 6874 3a2e 3235 7265 6d7d 2e79 7565  ight:.25rem}.yue
+000363e0: 202e 7364 2d63 6172 642d 686f 7665 723a   .sd-card-hover:
+000363f0: 686f 7665 727b 7472 616e 7366 6f72 6d3a  hover{transform:
+00036400: 7363 616c 6528 3129 7d2e 7975 6520 2e73  scale(1)}.yue .s
+00036410: 642d 6361 7264 2d68 6f76 6572 3a68 6f76  d-card-hover:hov
+00036420: 6572 202e 7364 2d63 6172 642d 7469 746c  er .sd-card-titl
+00036430: 657b 636f 6c6f 723a 7661 7228 2d2d 7379  e{color:var(--sy
+00036440: 2d63 2d6c 696e 6b2d 686f 7665 7229 7d2e  -c-link-hover)}.
+00036450: 7975 6520 2e73 642d 6361 7264 2061 2c2e  yue .sd-card a,.
+00036460: 7975 6520 2e73 642d 6361 7264 2061 3a68  yue .sd-card a:h
+00036470: 6f76 6572 7b62 6f72 6465 722d 626f 7474  over{border-bott
+00036480: 6f6d 3a30 7d2e 7975 6520 2e73 7572 6661  om:0}.yue .surfa
+00036490: 6365 202e 7364 2d63 6172 642d 626f 6479  ce .sd-card-body
+000364a0: 2c2e 7975 6520 2e73 7572 6661 6365 202e  ,.yue .surface .
+000364b0: 7364 2d63 6172 642d 666f 6f74 6572 2c2e  sd-card-footer,.
+000364c0: 7975 6520 2e73 7572 6661 6365 202e 7364  yue .surface .sd
+000364d0: 2d63 6172 642d 6865 6164 6572 7b70 6164  -card-header{pad
+000364e0: 6469 6e67 2d6c 6566 743a 312e 3572 656d  ding-left:1.5rem
+000364f0: 3b70 6164 6469 6e67 2d72 6967 6874 3a31  ;padding-right:1
+00036500: 2e35 7265 6d7d 2e79 7565 202e 7375 7266  .5rem}.yue .surf
+00036510: 6163 6520 2e73 642d 6361 7264 2d66 6f6f  ace .sd-card-foo
+00036520: 7465 722c 2e79 7565 202e 7375 7266 6163  ter,.yue .surfac
+00036530: 6520 2e73 642d 6361 7264 2d68 6561 6465  e .sd-card-heade
+00036540: 727b 626f 7264 6572 2d63 6f6c 6f72 3a76  r{border-color:v
+00036550: 6172 282d 2d73 792d 632d 626f 7264 6572  ar(--sy-c-border
+00036560: 297d 406d 6564 6961 2028 7072 696e 7429  )}@media (print)
+00036570: 7b2e 7975 6520 2e73 642d 6361 7264 7b70  {.yue .sd-card{p
+00036580: 6167 652d 6272 6561 6b2d 696e 7369 6465  age-break-inside
+00036590: 3a61 766f 6964 7d7d 2e79 7565 2061 2e73  :avoid}}.yue a.s
+000365a0: 642d 7465 7874 2d77 7261 703a 686f 7665  d-text-wrap:hove
+000365b0: 727b 626f 7264 6572 2d62 6f74 746f 6d2d  r{border-bottom-
+000365c0: 7769 6474 683a 3170 787d 2e73 7068 696e  width:1px}.sphin
+000365d0: 782d 7461 6273 205b 726f 6c65 3d74 6162  x-tabs [role=tab
+000365e0: 6c69 7374 5d7b 626f 7264 6572 2d63 6f6c  list]{border-col
+000365f0: 6f72 3a76 6172 282d 2d73 792d 632d 6469  or:var(--sy-c-di
+00036600: 7669 6465 7229 7d2e 7975 6520 2e73 7068  vider)}.yue .sph
+00036610: 696e 782d 7461 6273 2d74 6162 7b63 6f6c  inx-tabs-tab{col
+00036620: 6f72 3a76 6172 282d 2d73 792d 632d 7465  or:var(--sy-c-te
+00036630: 7874 293b 6c69 6e65 2d68 6569 6768 743a  xt);line-height:
+00036640: 696e 6865 7269 743b 7061 6464 696e 673a  inherit;padding:
+00036650: 3172 656d 202e 3235 7265 6d20 2e35 7265  1rem .25rem .5re
+00036660: 6d3b 666f 6e74 2d73 697a 653a 2e38 3472  m;font-size:.84r
+00036670: 656d 3b66 6f6e 742d 7765 6967 6874 3a35  em;font-weight:5
+00036680: 3030 3b62 6f72 6465 723a 6e6f 6e65 3b62  00;border:none;b
+00036690: 6f72 6465 722d 626f 7474 6f6d 3a2e 3132  order-bottom:.12
+000366a0: 3572 656d 2073 6f6c 6964 2023 3030 3030  5rem solid #0000
+000366b0: 7d2e 7975 6520 2e73 7068 696e 782d 7461  }.yue .sphinx-ta
+000366c0: 6273 2d74 6162 3a68 6f76 6572 7b63 6f6c  bs-tab:hover{col
+000366d0: 6f72 3a76 6172 282d 2d73 642d 636f 6c6f  or:var(--sd-colo
+000366e0: 722d 7461 6273 2d6c 6162 656c 2d68 6f76  r-tabs-label-hov
+000366f0: 6572 293b 626f 7264 6572 2d63 6f6c 6f72  er);border-color
+00036700: 3a76 6172 282d 2d73 642d 636f 6c6f 722d  :var(--sd-color-
+00036710: 7461 6273 2d75 6e64 6572 6c69 6e65 2d68  tabs-underline-h
+00036720: 6f76 6572 297d 2e79 7565 202e 7370 6869  over)}.yue .sphi
+00036730: 6e78 2d74 6162 732d 7461 625b 6172 6961  nx-tabs-tab[aria
+00036740: 2d73 656c 6563 7465 643d 7472 7565 5d7b  -selected=true]{
+00036750: 626f 7264 6572 3a6e 6f6e 653b 626f 7264  border:none;bord
+00036760: 6572 2d62 6f74 746f 6d3a 2e31 3235 7265  er-bottom:.125re
+00036770: 6d20 736f 6c69 6420 7661 7228 2d2d 7364  m solid var(--sd
+00036780: 2d63 6f6c 6f72 2d74 6162 732d 756e 6465  -color-tabs-unde
+00036790: 726c 696e 652d 6163 7469 7665 293b 636f  rline-active);co
+000367a0: 6c6f 723a 7661 7228 2d2d 7364 2d63 6f6c  lor:var(--sd-col
+000367b0: 6f72 2d74 6162 732d 6c61 6265 6c2d 6163  or-tabs-label-ac
+000367c0: 7469 7665 293b 6261 636b 6772 6f75 6e64  tive);background
+000367d0: 2d63 6f6c 6f72 3a69 6e69 7469 616c 7d2e  -color:initial}.
+000367e0: 7975 6520 2e73 7068 696e 782d 7461 6273  yue .sphinx-tabs
+000367f0: 2d74 6162 2b2e 7370 6869 6e78 2d74 6162  -tab+.sphinx-tab
+00036800: 732d 7461 627b 6d61 7267 696e 2d6c 6566  s-tab{margin-lef
+00036810: 743a 3172 656d 7d2e 7975 6520 2e73 7068  t:1rem}.yue .sph
+00036820: 696e 782d 7461 6273 2d70 616e 656c 7b62  inx-tabs-panel{b
+00036830: 6f72 6465 723a 6e6f 6e65 3b70 6164 6469  order:none;paddi
+00036840: 6e67 3a30 3b6d 6172 6769 6e3a 303b 626f  ng:0;margin:0;bo
+00036850: 7264 6572 2d72 6164 6975 733a 303b 6261  rder-radius:0;ba
+00036860: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3a69  ckground-color:i
+00036870: 6e69 7469 616c 7d2e 7975 6520 2e73 7068  nitial}.yue .sph
+00036880: 696e 782d 7461 6273 2d70 616e 656c 2e63  inx-tabs-panel.c
+00036890: 6f64 652d 7461 627b 7061 6464 696e 673a  ode-tab{padding:
+000368a0: 307d 2e79 7565 202e 7370 6869 6e78 2d74  0}.yue .sphinx-t
+000368b0: 6162 732d 7061 6e65 6c2e 636f 6465 2d74  abs-panel.code-t
+000368c0: 6162 202e 636f 6465 2d62 6c6f 636b 2d63  ab .code-block-c
+000368d0: 6170 7469 6f6e 2c2e 7975 6520 2e73 7068  aption,.yue .sph
+000368e0: 696e 782d 7461 6273 2d70 616e 656c 2e63  inx-tabs-panel.c
+000368f0: 6f64 652d 7461 6220 2e68 6967 686c 6967  ode-tab .highlig
+00036900: 6874 2070 7265 7b62 6f72 6465 722d 7261  ht pre{border-ra
+00036910: 6469 7573 3a30 7d2e 7975 657b 2d2d 6a70  dius:0}.yue{--jp
+00036920: 2d77 6964 6765 7473 2d69 6e70 7574 2d62  -widgets-input-b
+00036930: 6f72 6465 722d 636f 6c6f 723a 7661 7228  order-color:var(
+00036940: 2d2d 6772 6179 2d35 293b 2d2d 6a70 2d77  --gray-5);--jp-w
+00036950: 6964 6765 7473 2d69 6e70 7574 2d66 6f63  idgets-input-foc
+00036960: 7573 2d62 6f72 6465 722d 636f 6c6f 723a  us-border-color:
+00036970: 7661 7228 2d2d 6772 6179 2d38 293b 2d2d  var(--gray-8);--
+00036980: 6a70 2d77 6964 6765 7473 2d73 6c69 6465  jp-widgets-slide
+00036990: 722d 6163 7469 7665 2d68 616e 646c 652d  r-active-handle-
+000369a0: 636f 6c6f 723a 7661 7228 2d2d 6772 6179  color:var(--gray
+000369b0: 2d34 293b 2d2d 6a70 2d77 6964 6765 7473  -4);--jp-widgets
+000369c0: 2d73 6c69 6465 722d 6861 6e64 6c65 2d62  -slider-handle-b
+000369d0: 6f72 6465 722d 636f 6c6f 723a 7661 7228  order-color:var(
+000369e0: 2d2d 7379 2d63 2d62 6f72 6465 7229 7d2e  --sy-c-border)}.
+000369f0: 7975 6520 2e6a 7570 7974 6572 5f63 6f6e  yue .jupyter_con
+00036a00: 7461 696e 6572 7b62 6163 6b67 726f 756e  tainer{backgroun
+00036a10: 642d 636f 6c6f 723a 7661 7228 2d2d 7379  d-color:var(--sy
+00036a20: 2d63 2d62 6163 6b67 726f 756e 6429 3b62  -c-background);b
+00036a30: 6f72 6465 723a 3370 7820 736f 6c69 6420  order:3px solid 
+00036a40: 7661 7228 2d2d 7379 2d63 2d62 6f72 6465  var(--sy-c-borde
+00036a50: 7229 3b62 6f72 6465 722d 7261 6469 7573  r);border-radius
+00036a60: 3a36 7078 3b6f 7665 7266 6c6f 773a 6869  :6px;overflow:hi
+00036a70: 6464 656e 3b62 6f78 2d73 6861 646f 773a  dden;box-shadow:
+00036a80: 6e6f 6e65 7d2e 646f 6375 6d65 6e74 202e  none}.document .
+00036a90: 7975 6520 2e6a 7570 7974 6572 5f63 6f6e  yue .jupyter_con
+00036aa0: 7461 696e 6572 2064 6976 5b63 6c61 7373  tainer div[class
+00036ab0: 5e3d 6869 6768 6c69 6768 745d 7b70 6164  ^=highlight]{pad
+00036ac0: 6469 6e67 3a30 7d2e 7975 6520 2e6a 7570  ding:0}.yue .jup
+00036ad0: 7974 6572 5f63 6f6e 7461 696e 6572 2064  yter_container d
+00036ae0: 6976 2e63 656c 6c5f 696e 7075 747b 6261  iv.cell_input{ba
+00036af0: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3a76  ckground-color:v
+00036b00: 6172 282d 2d73 796e 7461 782d 7072 652d  ar(--syntax-pre-
+00036b10: 6267 293b 626f 7264 6572 3a30 3b62 6f72  bg);border:0;bor
+00036b20: 6465 722d 7261 6469 7573 3a30 7d2e 7975  der-radius:0}.yu
+00036b30: 6520 2e6a 7570 7974 6572 5f63 6f6e 7461  e .jupyter_conta
+00036b40: 696e 6572 2064 6976 2e63 6f64 655f 6365  iner div.code_ce
+00036b50: 6c6c 2070 7265 7b70 6164 6469 6e67 3a30  ll pre{padding:0
+00036b60: 7d2e 6a75 7079 7465 725f 636f 6e74 6169  }.jupyter_contai
+00036b70: 6e65 7220 6469 762e 6365 6c6c 5f6f 7574  ner div.cell_out
+00036b80: 7075 7420 2e6f 7574 7075 742c 2e6a 7570  put .output,.jup
+00036b90: 7974 6572 5f63 6f6e 7461 696e 6572 2064  yter_container d
+00036ba0: 6976 2e63 656c 6c5f 6f75 7470 7574 202e  iv.cell_output .
+00036bb0: 7374 6465 7272 2c2e 6a75 7079 7465 725f  stderr,.jupyter_
+00036bc0: 636f 6e74 6169 6e65 7220 6469 762e 6365  container div.ce
+00036bd0: 6c6c 5f6f 7574 7075 7420 2e77 6964 6765  ll_output .widge
+00036be0: 742d 7375 6261 7265 617b 7061 6464 696e  t-subarea{paddin
+00036bf0: 673a 2e35 7265 6d7d 2e6a 7570 7974 6572  g:.5rem}.jupyter
+00036c00: 5f63 6f6e 7461 696e 6572 2064 6976 2e63  _container div.c
+00036c10: 656c 6c5f 6f75 7470 7574 202e 7374 6465  ell_output .stde
+00036c20: 7272 202e 7374 6465 7272 7b70 6164 6469  rr .stderr{paddi
+00036c30: 6e67 3a30 7d2e 6a75 7079 7465 722d 7769  ng:0}.jupyter-wi
+00036c40: 6467 6574 2d68 736c 6964 6572 202e 736c  dget-hslider .sl
+00036c50: 6964 6572 2d63 6f6e 7461 696e 6572 2c2e  ider-container,.
+00036c60: 7769 6467 6574 2d68 736c 6964 6572 202e  widget-hslider .
+00036c70: 736c 6964 6572 2d63 6f6e 7461 696e 6572  slider-container
+00036c80: 7b64 6973 706c 6179 3a66 6c65 783b 616c  {display:flex;al
+00036c90: 6967 6e2d 6974 656d 733a 6365 6e74 6572  ign-items:center
+00036ca0: 7d2e 6a75 7079 7465 722d 7769 6467 6574  }.jupyter-widget
+00036cb0: 2d73 6c69 6465 7220 2e6e 6f55 692d 7461  -slider .noUi-ta
+00036cc0: 7267 6574 2c2e 7769 6467 6574 2d73 6c69  rget,.widget-sli
+00036cd0: 6465 7220 2e6e 6f55 692d 7461 7267 6574  der .noUi-target
+00036ce0: 7b77 6964 7468 3a31 3030 257d 2e6a 7570  {width:100%}.jup
+00036cf0: 7974 6572 5f63 6f6e 7461 696e 6572 2064  yter_container d
+00036d00: 6976 2e63 6f64 655f 6365 6c6c 202e 6869  iv.code_cell .hi
+00036d10: 6768 6c69 6768 743e 7072 657b 7061 6464  ghlight>pre{padd
+00036d20: 696e 673a 3172 656d 7d2e 6a75 7079 7465  ing:1rem}.jupyte
+00036d30: 725f 636f 6e74 6169 6e65 7220 6469 762e  r_container div.
+00036d40: 636f 6465 5f63 656c 6c20 2e68 6967 686c  code_cell .highl
+00036d50: 6967 6874 202e 686c 6c7b 6d61 7267 696e  ight .hll{margin
+00036d60: 2d6c 6566 743a 2d31 7265 6d3b 6d61 7267  -left:-1rem;marg
+00036d70: 696e 2d72 6967 6874 3a2d 3172 656d 3b70  in-right:-1rem;p
+00036d80: 6164 6469 6e67 3a30 2031 7265 6d7d 2e6a  adding:0 1rem}.j
+00036d90: 7570 7974 6572 5f63 6f6e 7461 696e 6572  upyter_container
+00036da0: 2064 6976 2e63 6f64 655f 6365 6c6c 202e   div.code_cell .
+00036db0: 6869 6768 6c69 6768 7420 2e6c 696e 656e  highlight .linen
+00036dc0: 6f73 7b6d 6172 6769 6e2d 7269 6768 743a  os{margin-right:
+00036dd0: 2e38 7265 6d7d 2e79 7565 202e 6a75 7079  .8rem}.yue .jupy
+00036de0: 7465 725f 636f 6e74 6169 6e65 7220 2e73  ter_container .s
+00036df0: 7464 6572 727b 636f 6c6f 723a 7661 7228  tderr{color:var(
+00036e00: 2d2d 7265 642d 6131 3129 3b62 6163 6b67  --red-a11);backg
+00036e10: 726f 756e 642d 636f 6c6f 723a 7661 7228  round-color:var(
+00036e20: 2d2d 7265 642d 6133 297d 2e79 7565 202e  --red-a3)}.yue .
+00036e30: 6a75 7079 7465 725f 636f 6e74 6169 6e65  jupyter_containe
+00036e40: 7220 2e73 7464 6572 7220 2e73 7464 6572  r .stderr .stder
+00036e50: 727b 6261 636b 6772 6f75 6e64 2d63 6f6c  r{background-col
+00036e60: 6f72 3a69 6e69 7469 616c 7d2e 6e62 696e  or:initial}.nbin
+00036e70: 7075 7420 2e68 6967 686c 6967 6874 7b2d  put .highlight{-
+00036e80: 2d72 6164 6975 733a 3170 787d 2e79 7565  -radius:1px}.yue
+00036e90: 2064 6976 2e6e 626c 6173 742e 636f 6e74   div.nblast.cont
+00036ea0: 6169 6e65 727b 7061 6464 696e 672d 746f  ainer{padding-to
+00036eb0: 703a 3570 787d 2e79 7565 2064 6976 2e6e  p:5px}.yue div.n
+00036ec0: 6269 6e70 7574 2e63 6f6e 7461 696e 6572  binput.container
+00036ed0: 2064 6976 2e69 6e70 7574 5f61 7265 617b   div.input_area{
+00036ee0: 626f 7264 6572 2d63 6f6c 6f72 3a76 6172  border-color:var
+00036ef0: 282d 2d73 792d 632d 626f 7264 6572 297d  (--sy-c-border)}
+00036f00: 2e79 7565 2064 6976 2e6e 626f 7574 7075  .yue div.nboutpu
+00036f10: 742e 636f 6e74 6169 6e65 7220 6469 762e  t.container div.
+00036f20: 6f75 7470 7574 5f61 7265 612e 7374 6465  output_area.stde
+00036f30: 7272 7b63 6f6c 6f72 3a76 6172 282d 2d72  rr{color:var(--r
+00036f40: 6564 2d61 3131 293b 6261 636b 6772 6f75  ed-a11);backgrou
+00036f50: 6e64 2d63 6f6c 6f72 3a76 6172 282d 2d72  nd-color:var(--r
+00036f60: 6564 2d61 3329 7d2e 7975 6520 6469 762e  ed-a3)}.yue div.
+00036f70: 6e62 6f75 7470 7574 2e63 6f6e 7461 696e  nboutput.contain
+00036f80: 6572 2064 6976 2e6f 7574 7075 745f 6172  er div.output_ar
+00036f90: 6561 3e2e 6d61 7468 2d77 7261 7070 6572  ea>.math-wrapper
+00036fa0: 3e64 6976 2e6d 6174 687b 7061 6464 696e  >div.math{paddin
+00036fb0: 672d 746f 703a 307d 2e79 7565 202e 6a70  g-top:0}.yue .jp
+00036fc0: 2d52 656e 6465 7265 6448 544d 4c43 6f6d  -RenderedHTMLCom
+00036fd0: 6d6f 6e20 7468 6561 642c 2e79 7565 2064  mon thead,.yue d
+00036fe0: 6976 2e72 656e 6465 7265 645f 6874 6d6c  iv.rendered_html
+00036ff0: 2074 6865 6164 7b62 6f72 6465 722d 636f   thead{border-co
+00037000: 6c6f 723a 7661 7228 2d2d 7379 2d63 2d62  lor:var(--sy-c-b
+00037010: 6f72 6465 7229 7d2e 7975 6520 2e6a 702d  order)}.yue .jp-
+00037020: 5265 6e64 6572 6564 4854 4d4c 436f 6d6d  RenderedHTMLComm
+00037030: 6f6e 2074 626f 6479 2074 722c 2e79 7565  on tbody tr,.yue
+00037040: 2064 6976 2e72 656e 6465 7265 645f 6874   div.rendered_ht
+00037050: 6d6c 2074 626f 6479 2074 727b 636f 6c6f  ml tbody tr{colo
+00037060: 723a 7661 7228 2d2d 7379 2d63 2d74 6578  r:var(--sy-c-tex
+00037070: 7429 7d2e 7975 6520 2e6a 702d 5265 6e64  t)}.yue .jp-Rend
+00037080: 6572 6564 4854 4d4c 436f 6d6d 6f6e 2074  eredHTMLCommon t
+00037090: 626f 6479 2074 723a 6e74 682d 6368 696c  body tr:nth-chil
+000370a0: 6428 6f64 6429 2c2e 7975 6520 6469 762e  d(odd),.yue div.
+000370b0: 7265 6e64 6572 6564 5f68 746d 6c20 7462  rendered_html tb
+000370c0: 6f64 7920 7472 3a6e 7468 2d63 6869 6c64  ody tr:nth-child
+000370d0: 286f 6464 297b 6261 636b 6772 6f75 6e64  (odd){background
+000370e0: 2d63 6f6c 6f72 3a76 6172 282d 2d73 792d  -color:var(--sy-
+000370f0: 632d 7375 7266 6163 6529 7d2e 7975 6520  c-surface)}.yue 
+00037100: 2e6a 702d 5265 6e64 6572 6564 4854 4d4c  .jp-RenderedHTML
+00037110: 436f 6d6d 6f6e 2074 626f 6479 2074 723a  Common tbody tr:
+00037120: 686f 7665 722c 2e79 7565 2064 6976 2e72  hover,.yue div.r
+00037130: 656e 6465 7265 645f 6874 6d6c 2074 626f  endered_html tbo
+00037140: 6479 2074 723a 686f 7665 727b 6261 636b  dy tr:hover{back
+00037150: 6772 6f75 6e64 2d63 6f6c 6f72 3a76 6172  ground-color:var
+00037160: 282d 2d63 6f6c 6f72 2d73 7572 6661 6365  (--color-surface
+00037170: 2d61 6363 656e 7429 7d2e 7975 657b 2d2d  -accent)}.yue{--
+00037180: 7367 2d74 6578 742d 636f 6c6f 723a 7661  sg-text-color:va
+00037190: 7228 2d2d 7379 2d63 2d74 6578 7429 3b2d  r(--sy-c-text);-
+000371a0: 2d73 672d 6261 636b 6772 6f75 6e64 2d63  -sg-background-c
+000371b0: 6f6c 6f72 3a76 6172 282d 2d73 792d 632d  olor:var(--sy-c-
+000371c0: 6261 636b 6772 6f75 6e64 293b 2d2d 7367  background);--sg
+000371d0: 2d63 6f64 652d 6261 636b 6772 6f75 6e64  -code-background
+000371e0: 2d63 6f6c 6f72 3a76 6172 282d 2d73 796e  -color:var(--syn
+000371f0: 7461 782d 7072 652d 6267 293b 2d2d 7367  tax-pre-bg);--sg
+00037200: 2d74 722d 686f 7665 722d 636f 6c6f 723a  -tr-hover-color:
+00037210: 7661 7228 2d2d 6163 6365 6e74 2d61 3329  var(--accent-a3)
+00037220: 3b2d 2d73 672d 7472 2d6f 6464 2d63 6f6c  ;--sg-tr-odd-col
+00037230: 6f72 3a76 6172 282d 2d73 792d 632d 7375  or:var(--sy-c-su
+00037240: 7266 6163 6529 3b2d 2d73 672d 746f 6f6c  rface);--sg-tool
+00037250: 7469 702d 666f 7265 6772 6f75 6e64 3a76  tip-foreground:v
+00037260: 6172 282d 2d73 792d 632d 6261 636b 6772  ar(--sy-c-backgr
+00037270: 6f75 6e64 2d63 6f6e 7472 6173 7429 3b2d  ound-contrast);-
+00037280: 2d73 672d 746f 6f6c 7469 702d 6261 636b  -sg-tooltip-back
+00037290: 6772 6f75 6e64 3a76 6172 282d 2d73 792d  ground:var(--sy-
+000372a0: 632d 6261 636b 6772 6f75 6e64 293b 2d2d  c-background);--
+000372b0: 7367 2d74 6f6f 6c74 6970 2d62 6f72 6465  sg-tooltip-borde
+000372c0: 723a 7661 7228 2d2d 6772 6179 2d37 2920  r:var(--gray-7) 
+000372d0: 2330 3030 303b 2d2d 7367 2d74 6875 6d62  #0000;--sg-thumb
+000372e0: 2d62 6f78 2d73 6861 646f 772d 636f 6c6f  -box-shadow-colo
+000372f0: 723a 7661 7228 2d2d 6772 6179 2d61 3429  r:var(--gray-a4)
+00037300: 3b2d 2d73 672d 7468 756d 622d 686f 7665  ;--sg-thumb-hove
+00037310: 722d 626f 7264 6572 3a76 6172 282d 2d61  r-border:var(--a
+00037320: 6363 656e 742d 6139 293b 2d2d 7367 2d73  ccent-a9);--sg-s
+00037330: 6372 6970 742d 6f75 743a 7661 7228 2d2d  cript-out:var(--
+00037340: 7379 2d63 2d6c 6967 6874 293b 2d2d 7367  sy-c-light);--sg
+00037350: 2d73 6372 6970 742d 7072 653a 7661 7228  -script-pre:var(
+00037360: 2d2d 7379 6e74 6178 2d70 7265 2d62 6729  --syntax-pre-bg)
+00037370: 3b2d 2d73 672d 7079 7462 2d66 6f72 6567  ;--sg-pytb-foreg
+00037380: 726f 756e 643a 7661 7228 2d2d 7379 6e74  round:var(--synt
+00037390: 6178 2d74 6578 7429 3b2d 2d73 672d 7079  ax-text);--sg-py
+000373a0: 7462 2d62 6163 6b67 726f 756e 643a 7661  tb-background:va
+000373b0: 7228 2d2d 7265 642d 6132 293b 2d2d 7367  r(--red-a2);--sg
+000373c0: 2d70 7974 622d 626f 7264 6572 2d63 6f6c  -pytb-border-col
+000373d0: 6f72 3a76 6172 282d 2d72 6564 2d61 3829  or:var(--red-a8)
+000373e0: 3b2d 2d73 672d 646f 776e 6c6f 6164 2d61  ;--sg-download-a
+000373f0: 2d62 6163 6b67 726f 756e 642d 636f 6c6f  -background-colo
+00037400: 723a 7661 7228 2d2d 6163 6365 6e74 2d61  r:var(--accent-a
+00037410: 3329 3b2d 2d73 672d 646f 776e 6c6f 6164  3);--sg-download
+00037420: 2d61 2d62 6163 6b67 726f 756e 642d 696d  -a-background-im
+00037430: 6167 653a 6e6f 6e65 3b2d 2d73 672d 646f  age:none;--sg-do
+00037440: 776e 6c6f 6164 2d61 2d62 6f72 6465 722d  wnload-a-border-
+00037450: 636f 6c6f 723a 3170 7820 736f 6c69 6420  color:1px solid 
+00037460: 7661 7228 2d2d 6163 6365 6e74 2d61 3329  var(--accent-a3)
+00037470: 3b2d 2d73 672d 646f 776e 6c6f 6164 2d61  ;--sg-download-a
+00037480: 2d63 6f6c 6f72 3a76 6172 282d 2d61 6363  -color:var(--acc
+00037490: 656e 742d 6131 3129 3b2d 2d73 672d 646f  ent-a11);--sg-do
+000374a0: 776e 6c6f 6164 2d61 2d68 6f76 6572 2d62  wnload-a-hover-b
+000374b0: 6163 6b67 726f 756e 642d 636f 6c6f 723a  ackground-color:
+000374c0: 7661 7228 2d2d 6163 6365 6e74 2d61 3429  var(--accent-a4)
+000374d0: 3b2d 2d73 672d 646f 776e 6c6f 6164 2d61  ;--sg-download-a
+000374e0: 2d68 6f76 6572 2d62 6f78 2d73 6861 646f  -hover-box-shado
+000374f0: 772d 313a 2330 3030 303b 2d2d 7367 2d64  w-1:#0000;--sg-d
+00037500: 6f77 6e6c 6f61 642d 612d 686f 7665 722d  ownload-a-hover-
+00037510: 626f 782d 7368 6164 6f77 2d32 3a23 3030  box-shadow-2:#00
+00037520: 3030 7d2e 7975 6520 2e73 7068 782d 676c  00}.yue .sphx-gl
+00037530: 722d 646f 776e 6c6f 6164 2061 2c2e 7975  r-download a,.yu
+00037540: 6520 2e73 7068 782d 676c 722d 646f 776e  e .sphx-glr-down
+00037550: 6c6f 6164 2061 3a68 6f76 6572 2c2e 7975  load a:hover,.yu
+00037560: 6520 2e73 7068 782d 676c 722d 7468 756d  e .sphx-glr-thum
+00037570: 626e 6169 6c73 2061 7b62 6f72 6465 722d  bnails a{border-
+00037580: 626f 7474 6f6d 3a30 7d2e 7975 6520 702e  bottom:0}.yue p.
+00037590: 7370 6878 2d67 6c72 2d73 6967 6e61 7475  sphx-glr-signatu
+000375a0: 7265 2061 7b62 6f72 6465 722d 7261 6469  re a{border-radi
+000375b0: 7573 3a30 3b62 6f72 6465 722d 626f 7474  us:0;border-bott
+000375c0: 6f6d 3a30 3b74 6578 742d 6465 636f 7261  om:0;text-decora
+000375d0: 7469 6f6e 3a75 6e64 6572 6c69 6e65 7d2e  tion:underline}.
+000375e0: 7975 6520 702e 7370 6878 2d67 6c72 2d73  yue p.sphx-glr-s
+000375f0: 6967 6e61 7475 7265 2061 3a68 6f76 6572  ignature a:hover
+00037600: 7b63 6f6c 6f72 3a76 6172 282d 2d73 792d  {color:var(--sy-
+00037610: 632d 6c69 6e6b 2d68 6f76 6572 297d 2e79  c-link-hover)}.y
+00037620: 7565 202e 7370 6878 2d67 6c72 2d66 6f6f  ue .sphx-glr-foo
+00037630: 7465 7220 696d 677b 6469 7370 6c61 793a  ter img{display:
+00037640: 696e 6c69 6e65 3b6d 6172 6769 6e3a 307d  inline;margin:0}
+00037650: 6874 6d6c 2e64 6172 6b2c 6874 6d6c 2e6c  html.dark,html.l
+00037660: 6967 6874 7b2d 2d64 6f63 7365 6172 6368  ight{--docsearch
+00037670: 2d70 7269 6d61 7279 2d63 6f6c 6f72 3a76  -primary-color:v
+00037680: 6172 282d 2d61 6363 656e 742d 3929 3b2d  ar(--accent-9);-
+00037690: 2d64 6f63 7365 6172 6368 2d74 6578 742d  -docsearch-text-
+000376a0: 636f 6c6f 723a 7661 7228 2d2d 7379 2d63  color:var(--sy-c
+000376b0: 2d74 6578 7429 3b2d 2d64 6f63 7365 6172  -text);--docsear
+000376c0: 6368 2d6d 6f64 616c 2d62 6163 6b67 726f  ch-modal-backgro
+000376d0: 756e 643a 7661 7228 2d2d 7379 2d63 2d62  und:var(--sy-c-b
+000376e0: 6163 6b67 726f 756e 6429 3b2d 2d64 6f63  ackground);--doc
+000376f0: 7365 6172 6368 2d66 6f6f 7465 722d 6261  search-footer-ba
+00037700: 636b 6772 6f75 6e64 3a76 6172 282d 2d73  ckground:var(--s
+00037710: 792d 632d 7375 7266 6163 6529 3b2d 2d64  y-c-surface);--d
+00037720: 6f63 7365 6172 6368 2d73 6561 7263 6862  ocsearch-searchb
+00037730: 6f78 2d62 6163 6b67 726f 756e 643a 7661  ox-background:va
+00037740: 7228 2d2d 7379 2d63 2d73 7572 6661 6365  r(--sy-c-surface
+00037750: 293b 2d2d 646f 6373 6561 7263 682d 7365  );--docsearch-se
+00037760: 6172 6368 626f 782d 666f 6375 732d 6261  archbox-focus-ba
+00037770: 636b 6772 6f75 6e64 3a76 6172 282d 2d73  ckground:var(--s
+00037780: 792d 632d 6261 636b 6772 6f75 6e64 293b  y-c-background);
+00037790: 2d2d 646f 6373 6561 7263 682d 6d75 7465  --docsearch-mute
+000377a0: 642d 636f 6c6f 723a 7661 7228 2d2d 7379  d-color:var(--sy
+000377b0: 2d63 2d6c 6967 6874 293b 2d2d 646f 6373  -c-light);--docs
+000377c0: 6561 7263 682d 6869 742d 636f 6c6f 723a  earch-hit-color:
+000377d0: 7661 7228 2d2d 7379 2d63 2d74 6578 7429  var(--sy-c-text)
+000377e0: 3b2d 2d64 6f63 7365 6172 6368 2d68 6974  ;--docsearch-hit
+000377f0: 2d62 6163 6b67 726f 756e 643a 7661 7228  -background:var(
+00037800: 2d2d 7379 2d63 2d73 7572 6661 6365 293b  --sy-c-surface);
+00037810: 2d2d 646f 6373 6561 7263 682d 6869 742d  --docsearch-hit-
+00037820: 6163 7469 7665 2d63 6f6c 6f72 3a76 6172  active-color:var
+00037830: 282d 2d61 6363 656e 742d 392d 636f 6e74  (--accent-9-cont
+00037840: 7261 7374 293b 2d2d 646f 6373 6561 7263  rast);--docsearc
+00037850: 682d 6869 742d 7368 6164 6f77 3a69 6e73  h-hit-shadow:ins
+00037860: 6574 2030 2030 2031 7078 2030 2076 6172  et 0 0 1px 0 var
+00037870: 282d 2d67 7261 792d 6131 3129 3b2d 2d64  (--gray-a11);--d
+00037880: 6f63 7365 6172 6368 2d63 6f6e 7461 696e  ocsearch-contain
+00037890: 6572 2d62 6163 6b67 726f 756e 643a 7661  er-background:va
+000378a0: 7228 2d2d 7379 2d63 2d6f 7665 726c 6179  r(--sy-c-overlay
+000378b0: 297d 6874 6d6c 2e6c 6967 6874 7b2d 2d64  )}html.light{--d
+000378c0: 6f63 7365 6172 6368 2d6b 6579 2d67 7261  ocsearch-key-gra
+000378d0: 6469 656e 743a 6c69 6e65 6172 2d67 7261  dient:linear-gra
+000378e0: 6469 656e 7428 2d32 3235 6465 672c 2365  dient(-225deg,#e
+000378f0: 3665 3665 362c 2366 3866 3866 3829 3b2d  6e6e6,#f8f8f8);-
+00037900: 2d64 6f63 7365 6172 6368 2d6b 6579 2d73  -docsearch-key-s
+00037910: 6861 646f 773a 696e 7365 7420 3020 2d32  hadow:inset 0 -2
+00037920: 7078 2023 6462 6462 6462 2c69 6e73 6574  px #dbdbdb,inset
+00037930: 2030 2030 2031 7078 2031 7078 2023 6666   0 0 1px 1px #ff
+00037940: 662c 3020 3170 7820 3270 7820 3170 7820  f,0 1px 2px 1px 
+00037950: 2335 3035 3035 3036 367d 6874 6d6c 2e64  #50505066}html.d
+00037960: 6172 6b7b 2d2d 646f 6373 6561 7263 682d  ark{--docsearch-
+00037970: 6b65 792d 6772 6164 6965 6e74 3a6c 696e  key-gradient:lin
+00037980: 6561 722d 6772 6164 6965 6e74 282d 3232  ear-gradient(-22
+00037990: 3564 6567 2c23 3335 3334 3334 2c23 3134  5deg,#353434,#14
+000379a0: 3134 3134 293b 2d2d 646f 6373 6561 7263  1414);--docsearc
+000379b0: 682d 6b65 792d 7368 6164 6f77 3a69 6e73  h-key-shadow:ins
+000379c0: 6574 2030 202d 3270 7820 2333 3733 3733  et 0 -2px #37373
+000379d0: 372c 696e 7365 7420 3020 3020 3170 7820  7,inset 0 0 1px 
+000379e0: 3170 7820 2332 3232 2c30 2031 7078 2032  1px #222,0 1px 2
+000379f0: 7078 2031 7078 2023 3030 303b 2d2d 646f  px 1px #000;--do
+00037a00: 6373 6561 7263 682d 666f 6f74 6572 2d73  csearch-footer-s
+00037a10: 6861 646f 773a 3020 2d31 7078 2030 2030  hadow:0 -1px 0 0
+00037a20: 2023 3337 3337 3337 2c30 202d 3370 7820   #373737,0 -3px 
+00037a30: 3670 7820 3020 2331 3431 3431 343b 2d2d  6px 0 #141414;--
+00037a40: 646f 6373 6561 7263 682d 6d6f 6461 6c2d  docsearch-modal-
+00037a50: 7368 6164 6f77 3a69 6e73 6574 2031 7078  shadow:inset 1px
+00037a60: 2031 7078 2030 2030 2023 3337 3337 3337   1px 0 0 #373737
+00037a70: 2c30 2033 7078 2038 7078 2030 2023 3134  ,0 3px 8px 0 #14
+00037a80: 3134 3134 7d23 646f 6373 6561 7263 6820  1414}#docsearch 
+00037a90: 2e44 6f63 5365 6172 6368 2d42 7574 746f  .DocSearch-Butto
+00037aa0: 6e7b 626f 7264 6572 2d72 6164 6975 733a  n{border-radius:
+00037ab0: 3670 787d 2364 6f63 7365 6172 6368 202e  6px}#docsearch .
+00037ac0: 446f 6353 6561 7263 682d 4275 7474 6f6e  DocSearch-Button
+00037ad0: 2d4b 6579 2c23 646f 6373 6561 7263 6820  -Key,#docsearch 
+00037ae0: 2e44 6f63 5365 6172 6368 2d42 7574 746f  .DocSearch-Butto
+00037af0: 6e2d 506c 6163 6568 6f6c 6465 727b 666f  n-Placeholder{fo
+00037b00: 6e74 2d73 697a 653a 2e38 3235 7265 6d7d  nt-size:.825rem}
+00037b10: 2364 6f63 7365 6172 6368 202e 446f 6353  #docsearch .DocS
+00037b20: 6561 7263 682d 4275 7474 6f6e 2d4b 6579  earch-Button-Key
+00037b30: 732c 2364 6f63 7365 6172 6368 202e 446f  s,#docsearch .Do
+00037b40: 6353 6561 7263 682d 4275 7474 6f6e 2d50  cSearch-Button-P
+00037b50: 6c61 6365 686f 6c64 6572 7b64 6973 706c  laceholder{displ
+00037b60: 6179 3a66 6c65 7821 696d 706f 7274 616e  ay:flex!importan
+00037b70: 747d 2364 6f63 7365 6172 6368 202e 446f  t}#docsearch .Do
+00037b80: 6353 6561 7263 682d 5365 6172 6368 2d49  cSearch-Search-I
+00037b90: 636f 6e7b 7769 6474 683a 2e38 3735 7265  con{width:.875re
+00037ba0: 6d21 696d 706f 7274 616e 743b 6865 6967  m!important;heig
+00037bb0: 6874 3a2e 3837 3572 656d 2169 6d70 6f72  ht:.875rem!impor
+00037bc0: 7461 6e74 7d40 6d65 6469 6120 286d 6178  tant}@media (max
+00037bd0: 2d77 6964 7468 3a37 3637 7078 297b 2364  -width:767px){#d
+00037be0: 6f63 7365 6172 6368 7b70 6f73 6974 696f  ocsearch{positio
+00037bf0: 6e3a 6162 736f 6c75 7465 3b74 6f70 3a31  n:absolute;top:1
+00037c00: 7265 6d3b 6c65 6674 3a31 2e38 7265 6d3b  rem;left:1.8rem;
+00037c10: 7269 6768 743a 312e 3872 656d 7d23 646f  right:1.8rem}#do
+00037c20: 6373 6561 7263 6820 2e44 6f63 5365 6172  csearch .DocSear
+00037c30: 6368 2d42 7574 746f 6e7b 6d61 7267 696e  ch-Button{margin
+00037c40: 2d6c 6566 743a 303b 7769 6474 683a 3130  -left:0;width:10
+00037c50: 3025 7d7d 646c 2e73 716c 6120 6474 7b63  0%}}dl.sqla dt{c
+00037c60: 6f6c 6f72 3a76 6172 282d 2d73 6967 2d6e  olor:var(--sig-n
+00037c70: 616d 6529 3b6d 6172 6769 6e2d 626f 7474  ame);margin-bott
+00037c80: 6f6d 3a2e 3572 656d 7d64 6c2e 7371 6c61  om:.5rem}dl.sqla
+00037c90: 2064 743e 656d 7b66 6f6e 742d 7765 6967   dt>em{font-weig
+00037ca0: 6874 3a34 3030 3b66 6f6e 742d 7374 796c  ht:400;font-styl
+00037cb0: 653a 6e6f 726d 616c 3b63 6f6c 6f72 3a76  e:normal;color:v
+00037cc0: 6172 282d 2d73 6967 2d70 6172 616d 297d  ar(--sig-param)}
+00037cd0: 646c 2e73 716c 6120 6464 3e70 2e72 7562  dl.sqla dd>p.rub
+00037ce0: 7269 637b 6d61 7267 696e 2d74 6f70 3a31  ric{margin-top:1
+00037cf0: 2e35 7265 6d3b 7465 7874 2d74 7261 6e73  .5rem;text-trans
+00037d00: 666f 726d 3a75 7070 6572 6361 7365 3b66  form:uppercase;f
+00037d10: 6f6e 742d 7369 7a65 3a2e 3736 7265 6d7d  ont-size:.76rem}
+00037d20: 646c 2e73 716c 6120 6464 3e70 2e72 7562  dl.sqla dd>p.rub
+00037d30: 7269 632b 2e74 6162 6c65 2d77 7261 7070  ric+.table-wrapp
+00037d40: 6572 7b6d 6172 6769 6e2d 746f 703a 2e37  er{margin-top:.7
+00037d50: 3572 656d 3b62 6f72 6465 722d 6c65 6674  5rem;border-left
+00037d60: 3a30 3b62 6f72 6465 722d 7269 6768 743a  :0;border-right:
+00037d70: 303b 626f 7264 6572 2d72 6164 6975 733a  0;border-radius:
+00037d80: 307d 646c 2e73 716c 6120 702e 7275 6272  0}dl.sqla p.rubr
 00037d90: 6963 2b2e 7461 626c 652d 7772 6170 7065  ic+.table-wrappe
-00037da0: 7220 7468 7b62 6f72 6465 722d 6c65 6674  r th{border-left
-00037db0: 3a30 3b62 6f72 6465 722d 7269 6768 743a  :0;border-right:
-00037dc0: 303b 6261 636b 6772 6f75 6e64 2d63 6f6c  0;background-col
-00037dd0: 6f72 3a69 6e69 7469 616c 7d64 6c2e 7371  or:initial}dl.sq
-00037de0: 6c61 2070 2e72 7562 7269 632b 2e74 6162  la p.rubric+.tab
-00037df0: 6c65 2d77 7261 7070 6572 2074 643e 707b  le-wrapper td>p{
-00037e00: 6d61 7267 696e 3a30 7d64 6c2e 7371 6c61  margin:0}dl.sqla
-00037e10: 2070 2e72 7562 7269 632b 2e74 6162 6c65   p.rubric+.table
-00037e20: 2d77 7261 7070 6572 2074 722e 726f 772d  -wrapper tr.row-
-00037e30: 6f64 647b 6261 636b 6772 6f75 6e64 2d63  odd{background-c
-00037e40: 6f6c 6f72 3a69 6e69 7469 616c 7d64 6c2e  olor:initial}dl.
-00037e50: 7371 6c61 2070 2e72 7562 7269 632b 2e74  sqla p.rubric+.t
-00037e60: 6162 6c65 2d77 7261 7070 6572 2074 722e  able-wrapper tr.
-00037e70: 726f 772d 6576 656e 7b62 6163 6b67 726f  row-even{backgro
-00037e80: 756e 642d 636f 6c6f 723a 7661 7228 2d2d  und-color:var(--
-00037e90: 7975 652d 632d 726f 772d 6261 636b 6772  yue-c-row-backgr
-00037ea0: 6f75 6e64 297d 2e79 7565 7b2d 2d78 722d  ound)}.yue{--xr-
-00037eb0: 666f 6e74 2d63 6f6c 6f72 303a 7661 7228  font-color0:var(
-00037ec0: 2d2d 7379 2d63 2d68 6561 6469 6e67 293b  --sy-c-heading);
-00037ed0: 2d2d 7872 2d66 6f6e 742d 636f 6c6f 7232  --xr-font-color2
-00037ee0: 3a76 6172 282d 2d73 792d 632d 7465 7874  :var(--sy-c-text
-00037ef0: 293b 2d2d 7872 2d66 6f6e 742d 636f 6c6f  );--xr-font-colo
-00037f00: 7233 3a76 6172 282d 2d73 792d 632d 6c69  r3:var(--sy-c-li
-00037f10: 6768 7429 3b2d 2d78 722d 626f 7264 6572  ght);--xr-border
-00037f20: 2d63 6f6c 6f72 3a76 6172 282d 2d73 792d  -color:var(--sy-
-00037f30: 632d 626f 7264 6572 293b 2d2d 7872 2d64  c-border);--xr-d
-00037f40: 6973 6162 6c65 642d 636f 6c6f 723a 7661  isabled-color:va
-00037f50: 7228 2d2d 6772 6179 2d61 3629 3b2d 2d78  r(--gray-a6);--x
-00037f60: 722d 6261 636b 6772 6f75 6e64 2d63 6f6c  r-background-col
-00037f70: 6f72 3a76 6172 282d 2d73 792d 632d 6261  or:var(--sy-c-ba
-00037f80: 636b 6772 6f75 6e64 293b 2d2d 7872 2d62  ckground);--xr-b
-00037f90: 6163 6b67 726f 756e 642d 636f 6c6f 722d  ackground-color-
-00037fa0: 726f 772d 6576 656e 3a76 6172 282d 2d73  row-even:var(--s
-00037fb0: 792d 632d 6261 636b 6772 6f75 6e64 293b  y-c-background);
-00037fc0: 2d2d 7872 2d62 6163 6b67 726f 756e 642d  --xr-background-
-00037fd0: 636f 6c6f 722d 726f 772d 6f64 643a 7661  color-row-odd:va
-00037fe0: 7228 2d2d 6772 6179 2d32 297d 2e79 7565  r(--gray-2)}.yue
-00037ff0: 202e 7872 2d61 7272 6179 2d64 6174 6120   .xr-array-data 
-00038000: 7072 657b 6d61 7267 696e 3a30 7d2e 7975  pre{margin:0}.yu
-00038010: 6520 6465 7461 696c 732e 746f 6767 6c65  e details.toggle
-00038020: 2d64 6574 6169 6c73 2073 756d 6d61 7279  -details summary
-00038030: 7b62 6f72 6465 722d 6c65 6674 2d63 6f6c  {border-left-col
-00038040: 6f72 3a76 6172 282d 2d61 6363 656e 742d  or:var(--accent-
-00038050: 6139 297d 406d 6564 6961 206e 6f74 2061  a9)}@media not a
-00038060: 6c6c 2061 6e64 2028 6d69 6e2d 7769 6474  ll and (min-widt
-00038070: 683a 3634 3070 7829 7b2e 6d61 782d 736d  h:640px){.max-sm
-00038080: 5c3a 6d61 782d 772d 6675 6c6c 7b6d 6178  \:max-w-full{max
-00038090: 2d77 6964 7468 3a31 3030 257d 7d40 6d65  -width:100%}}@me
-000380a0: 6469 6120 286d 696e 2d77 6964 7468 3a37  dia (min-width:7
-000380b0: 3638 7078 297b 2e6d 645c 3a73 7469 636b  68px){.md\:stick
-000380c0: 797b 706f 7369 7469 6f6e 3a73 7469 636b  y{position:stick
-000380d0: 797d 2e6d 645c 3a69 6e6c 696e 657b 6469  y}.md\:inline{di
-000380e0: 7370 6c61 793a 696e 6c69 6e65 7d2e 6d64  splay:inline}.md
-000380f0: 5c3a 666c 6578 7b64 6973 706c 6179 3a66  \:flex{display:f
-00038100: 6c65 787d 2e6d 645c 3a68 6964 6465 6e7b  lex}.md\:hidden{
-00038110: 6469 7370 6c61 793a 6e6f 6e65 7d2e 6d64  display:none}.md
-00038120: 5c3a 772d 3732 7b77 6964 7468 3a31 3872  \:w-72{width:18r
-00038130: 656d 7d2e 6d64 5c3a 7368 7269 6e6b 2d30  em}.md\:shrink-0
-00038140: 7b66 6c65 782d 7368 7269 6e6b 3a30 7d7d  {flex-shrink:0}}
-00038150: 406d 6564 6961 2028 6d69 6e2d 7769 6474  @media (min-widt
-00038160: 683a 3132 3830 7078 297b 2e78 6c5c 3a73  h:1280px){.xl\:s
-00038170: 7469 636b 797b 706f 7369 7469 6f6e 3a73  ticky{position:s
-00038180: 7469 636b 797d 2e78 6c5c 3a74 6f70 2d31  ticky}.xl\:top-1
-00038190: 367b 746f 703a 3472 656d 7d2e 786c 5c3a  6{top:4rem}.xl\:
-000381a0: 6869 6464 656e 7b64 6973 706c 6179 3a6e  hidden{display:n
-000381b0: 6f6e 657d 2e78 6c5c 3a70 782d 3132 7b70  one}.xl\:px-12{p
-000381c0: 6164 6469 6e67 2d6c 6566 743a 3372 656d  adding-left:3rem
-000381d0: 3b70 6164 6469 6e67 2d72 6967 6874 3a33  ;padding-right:3
-000381e0: 7265 6d7d 2e78 6c5c 3a70 6c2d 307b 7061  rem}.xl\:pl-0{pa
-000381f0: 6464 696e 672d 6c65 6674 3a30 7d7d 406d  dding-left:0}}@m
-00038200: 6564 6961 2070 7269 6e74 7b2e 7072 696e  edia print{.prin
-00038210: 745c 3a68 6964 6465 6e7b 6469 7370 6c61  t\:hidden{displa
-00038220: 793a 6e6f 6e65 7d2e 7072 696e 745c 3a70  y:none}.print\:p
-00038230: 742d 367b 7061 6464 696e 672d 746f 703a  t-6{padding-top:
-00038240: 312e 3572 656d 7d7d                      1.5rem}}
+00037da0: 7220 7464 2c64 6c2e 7371 6c61 2070 2e72  r td,dl.sqla p.r
+00037db0: 7562 7269 632b 2e74 6162 6c65 2d77 7261  ubric+.table-wra
+00037dc0: 7070 6572 2074 687b 626f 7264 6572 2d6c  pper th{border-l
+00037dd0: 6566 743a 303b 626f 7264 6572 2d72 6967  eft:0;border-rig
+00037de0: 6874 3a30 3b62 6163 6b67 726f 756e 642d  ht:0;background-
+00037df0: 636f 6c6f 723a 696e 6974 6961 6c7d 646c  color:initial}dl
+00037e00: 2e73 716c 6120 702e 7275 6272 6963 2b2e  .sqla p.rubric+.
+00037e10: 7461 626c 652d 7772 6170 7065 7220 7464  table-wrapper td
+00037e20: 3e70 7b6d 6172 6769 6e3a 307d 646c 2e73  >p{margin:0}dl.s
+00037e30: 716c 6120 702e 7275 6272 6963 2b2e 7461  qla p.rubric+.ta
+00037e40: 626c 652d 7772 6170 7065 7220 7472 2e72  ble-wrapper tr.r
+00037e50: 6f77 2d6f 6464 7b62 6163 6b67 726f 756e  ow-odd{backgroun
+00037e60: 642d 636f 6c6f 723a 696e 6974 6961 6c7d  d-color:initial}
+00037e70: 646c 2e73 716c 6120 702e 7275 6272 6963  dl.sqla p.rubric
+00037e80: 2b2e 7461 626c 652d 7772 6170 7065 7220  +.table-wrapper 
+00037e90: 7472 2e72 6f77 2d65 7665 6e7b 6261 636b  tr.row-even{back
+00037ea0: 6772 6f75 6e64 2d63 6f6c 6f72 3a76 6172  ground-color:var
+00037eb0: 282d 2d79 7565 2d63 2d72 6f77 2d62 6163  (--yue-c-row-bac
+00037ec0: 6b67 726f 756e 6429 7d2e 7975 657b 2d2d  kground)}.yue{--
+00037ed0: 7872 2d66 6f6e 742d 636f 6c6f 7230 3a76  xr-font-color0:v
+00037ee0: 6172 282d 2d73 792d 632d 6865 6164 696e  ar(--sy-c-headin
+00037ef0: 6729 3b2d 2d78 722d 666f 6e74 2d63 6f6c  g);--xr-font-col
+00037f00: 6f72 323a 7661 7228 2d2d 7379 2d63 2d74  or2:var(--sy-c-t
+00037f10: 6578 7429 3b2d 2d78 722d 666f 6e74 2d63  ext);--xr-font-c
+00037f20: 6f6c 6f72 333a 7661 7228 2d2d 7379 2d63  olor3:var(--sy-c
+00037f30: 2d6c 6967 6874 293b 2d2d 7872 2d62 6f72  -light);--xr-bor
+00037f40: 6465 722d 636f 6c6f 723a 7661 7228 2d2d  der-color:var(--
+00037f50: 7379 2d63 2d62 6f72 6465 7229 3b2d 2d78  sy-c-border);--x
+00037f60: 722d 6469 7361 626c 6564 2d63 6f6c 6f72  r-disabled-color
+00037f70: 3a76 6172 282d 2d67 7261 792d 6136 293b  :var(--gray-a6);
+00037f80: 2d2d 7872 2d62 6163 6b67 726f 756e 642d  --xr-background-
+00037f90: 636f 6c6f 723a 7661 7228 2d2d 7379 2d63  color:var(--sy-c
+00037fa0: 2d62 6163 6b67 726f 756e 6429 3b2d 2d78  -background);--x
+00037fb0: 722d 6261 636b 6772 6f75 6e64 2d63 6f6c  r-background-col
+00037fc0: 6f72 2d72 6f77 2d65 7665 6e3a 7661 7228  or-row-even:var(
+00037fd0: 2d2d 7379 2d63 2d62 6163 6b67 726f 756e  --sy-c-backgroun
+00037fe0: 6429 3b2d 2d78 722d 6261 636b 6772 6f75  d);--xr-backgrou
+00037ff0: 6e64 2d63 6f6c 6f72 2d72 6f77 2d6f 6464  nd-color-row-odd
+00038000: 3a76 6172 282d 2d67 7261 792d 3229 7d2e  :var(--gray-2)}.
+00038010: 7975 6520 2e78 722d 6172 7261 792d 6461  yue .xr-array-da
+00038020: 7461 2070 7265 7b6d 6172 6769 6e3a 307d  ta pre{margin:0}
+00038030: 2e79 7565 2064 6574 6169 6c73 2e74 6f67  .yue details.tog
+00038040: 676c 652d 6465 7461 696c 7320 7375 6d6d  gle-details summ
+00038050: 6172 797b 626f 7264 6572 2d6c 6566 742d  ary{border-left-
+00038060: 636f 6c6f 723a 7661 7228 2d2d 6163 6365  color:var(--acce
+00038070: 6e74 2d61 3929 7d40 6d65 6469 6120 6e6f  nt-a9)}@media no
+00038080: 7420 616c 6c20 616e 6420 286d 696e 2d77  t all and (min-w
+00038090: 6964 7468 3a36 3430 7078 297b 2e6d 6178  idth:640px){.max
+000380a0: 2d73 6d5c 3a6d 6178 2d77 2d66 756c 6c7b  -sm\:max-w-full{
+000380b0: 6d61 782d 7769 6474 683a 3130 3025 7d7d  max-width:100%}}
+000380c0: 406d 6564 6961 2028 6d69 6e2d 7769 6474  @media (min-widt
+000380d0: 683a 3736 3870 7829 7b2e 6d64 5c3a 7374  h:768px){.md\:st
+000380e0: 6963 6b79 7b70 6f73 6974 696f 6e3a 7374  icky{position:st
+000380f0: 6963 6b79 7d2e 6d64 5c3a 696e 6c69 6e65  icky}.md\:inline
+00038100: 7b64 6973 706c 6179 3a69 6e6c 696e 657d  {display:inline}
+00038110: 2e6d 645c 3a66 6c65 787b 6469 7370 6c61  .md\:flex{displa
+00038120: 793a 666c 6578 7d2e 6d64 5c3a 6869 6464  y:flex}.md\:hidd
+00038130: 656e 7b64 6973 706c 6179 3a6e 6f6e 657d  en{display:none}
+00038140: 2e6d 645c 3a77 2d37 327b 7769 6474 683a  .md\:w-72{width:
+00038150: 3138 7265 6d7d 2e6d 645c 3a73 6872 696e  18rem}.md\:shrin
+00038160: 6b2d 307b 666c 6578 2d73 6872 696e 6b3a  k-0{flex-shrink:
+00038170: 307d 7d40 6d65 6469 6120 286d 696e 2d77  0}}@media (min-w
+00038180: 6964 7468 3a31 3238 3070 7829 7b2e 786c  idth:1280px){.xl
+00038190: 5c3a 7374 6963 6b79 7b70 6f73 6974 696f  \:sticky{positio
+000381a0: 6e3a 7374 6963 6b79 7d2e 786c 5c3a 746f  n:sticky}.xl\:to
+000381b0: 702d 3136 7b74 6f70 3a34 7265 6d7d 2e78  p-16{top:4rem}.x
+000381c0: 6c5c 3a68 6964 6465 6e7b 6469 7370 6c61  l\:hidden{displa
+000381d0: 793a 6e6f 6e65 7d2e 786c 5c3a 7078 2d31  y:none}.xl\:px-1
+000381e0: 327b 7061 6464 696e 672d 6c65 6674 3a33  2{padding-left:3
+000381f0: 7265 6d3b 7061 6464 696e 672d 7269 6768  rem;padding-righ
+00038200: 743a 3372 656d 7d2e 786c 5c3a 706c 2d30  t:3rem}.xl\:pl-0
+00038210: 7b70 6164 6469 6e67 2d6c 6566 743a 307d  {padding-left:0}
+00038220: 7d40 6d65 6469 6120 7072 696e 747b 2e70  }@media print{.p
+00038230: 7269 6e74 5c3a 6869 6464 656e 7b64 6973  rint\:hidden{dis
+00038240: 706c 6179 3a6e 6f6e 657d 2e70 7269 6e74  play:none}.print
+00038250: 5c3a 7074 2d36 7b70 6164 6469 6e67 2d74  \:pt-6{padding-t
+00038260: 6f70 3a31 2e35 7265 6d7d 7d              op:1.5rem}}
```

### Comparing `shibuya-2024.5.14/src/shibuya/theme/shibuya/static/shibuya.js` & `shibuya-2024.5.15/src/shibuya/theme/shibuya/static/shibuya.js`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.14/src/shibuya/theme/shibuya/theme.conf` & `shibuya-2024.5.15/src/shibuya/theme/shibuya/theme.conf`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.14/src/shibuya.egg-info/PKG-INFO` & `shibuya-2024.5.15/src/shibuya.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shibuya
-Version: 2024.5.14
+Version: 2024.5.15
 Summary: A clean, responsive, and customizable Sphinx documentation theme with light/dark mode.
 Author-email: Hsiaoming Yang <me@lepture.com>
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/lepture/shibuya
 Project-URL: Documentation, https://shibuya.lepture.com/
 Project-URL: Sponsors, https://github.com/sponsors/lepture
 Classifier: Framework :: Sphinx
```

### Comparing `shibuya-2024.5.14/src/shibuya.egg-info/SOURCES.txt` & `shibuya-2024.5.15/src/shibuya.egg-info/SOURCES.txt`

 * *Files identical despite different names*

