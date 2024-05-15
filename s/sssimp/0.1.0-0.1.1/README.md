# Comparing `tmp/sssimp-0.1.0.tar.gz` & `tmp/sssimp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sssimp-0.1.0.tar", last modified: Sat Apr 27 06:07:27 2024, max compression
+gzip compressed data, was "sssimp-0.1.1.tar", last modified: Wed May 15 04:35:16 2024, max compression
```

## Comparing `sssimp-0.1.0.tar` & `sssimp-0.1.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.647998 sssimp-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-27 06:07:22.000000 sssimp-0.1.0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.639998 sssimp-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.643998 sssimp-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-27 06:07:22.000000 sssimp-0.1.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-27 06:07:22.000000 sssimp-0.1.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-27 06:07:22.000000 sssimp-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-27 06:07:22.000000 sssimp-0.1.0/DEVELOPER_README.md
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-27 06:07:22.000000 sssimp-0.1.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-27 06:07:22.000000 sssimp-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-27 06:07:22.000000 sssimp-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-27 06:07:27.647998 sssimp-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-04-27 06:07:22.000000 sssimp-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.639998 sssimp-0.1.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.639998 sssimp-0.1.0/examples/01-basic/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.639998 sssimp-0.1.0/examples/01-basic/input/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.643998 sssimp-0.1.0/examples/01-basic/input/content/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-27 06:07:22.000000 sssimp-0.1.0/examples/01-basic/input/content/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.643998 sssimp-0.1.0/examples/01-basic/input/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-27 06:07:22.000000 sssimp-0.1.0/examples/01-basic/input/templates/base.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.643998 sssimp-0.1.0/examples/01-basic/output/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-27 06:07:22.000000 sssimp-0.1.0/examples/01-basic/output/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.639998 sssimp-0.1.0/examples/02-blog-with-markdown-pages/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.639998 sssimp-0.1.0/examples/02-blog-with-markdown-pages/input/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.643998 sssimp-0.1.0/examples/02-blog-with-markdown-pages/input/content/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-27 06:07:22.000000 sssimp-0.1.0/examples/02-blog-with-markdown-pages/input/content/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.643998 sssimp-0.1.0/examples/02-blog-with-markdown-pages/input/content/post/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-27 06:07:22.000000 sssimp-0.1.0/examples/02-blog-with-markdown-pages/input/content/post/first.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.643998 sssimp-0.1.0/examples/02-blog-with-markdown-pages/input/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-27 06:07:22.000000 sssimp-0.1.0/examples/02-blog-with-markdown-pages/input/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-27 06:07:22.000000 sssimp-0.1.0/examples/02-blog-with-markdown-pages/input/templates/post.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.643998 sssimp-0.1.0/examples/02-blog-with-markdown-pages/output/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-27 06:07:22.000000 sssimp-0.1.0/examples/02-blog-with-markdown-pages/output/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.643998 sssimp-0.1.0/examples/02-blog-with-markdown-pages/output/post/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-27 06:07:22.000000 sssimp-0.1.0/examples/02-blog-with-markdown-pages/output/post/first.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.639998 sssimp-0.1.0/examples/03-emojis/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.639998 sssimp-0.1.0/examples/03-emojis/input/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.643998 sssimp-0.1.0/examples/03-emojis/input/content/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-27 06:07:22.000000 sssimp-0.1.0/examples/03-emojis/input/content/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.643998 sssimp-0.1.0/examples/03-emojis/input/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-27 06:07:22.000000 sssimp-0.1.0/examples/03-emojis/input/templates/content.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.643998 sssimp-0.1.0/examples/03-emojis/output/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-27 06:07:22.000000 sssimp-0.1.0/examples/03-emojis/output/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-27 06:07:22.000000 sssimp-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 06:07:27.647998 sssimp-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.639998 sssimp-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.643998 sssimp-0.1.0/src/sssimp/
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-27 06:07:22.000000 sssimp-0.1.0/src/sssimp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-27 06:07:22.000000 sssimp-0.1.0/src/sssimp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-27 06:07:22.000000 sssimp-0.1.0/src/sssimp/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-27 06:07:22.000000 sssimp-0.1.0/src/sssimp/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.647998 sssimp-0.1.0/src/sssimp/generators/
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-27 06:07:22.000000 sssimp-0.1.0/src/sssimp/generators/css.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-27 06:07:22.000000 sssimp-0.1.0/src/sssimp/generators/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-27 06:07:22.000000 sssimp-0.1.0/src/sssimp/generators/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-04-27 06:07:22.000000 sssimp-0.1.0/src/sssimp/generators/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-27 06:07:22.000000 sssimp-0.1.0/src/sssimp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.647998 sssimp-0.1.0/src/sssimp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-27 06:07:27.000000 sssimp-0.1.0/src/sssimp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-27 06:07:27.000000 sssimp-0.1.0/src/sssimp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 06:07:27.000000 sssimp-0.1.0/src/sssimp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-27 06:07:27.000000 sssimp-0.1.0/src/sssimp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-27 06:07:27.000000 sssimp-0.1.0/src/sssimp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-27 06:07:27.000000 sssimp-0.1.0/src/sssimp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:07:27.647998 sssimp-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-27 06:07:22.000000 sssimp-0.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-27 06:07:22.000000 sssimp-0.1.0/tests/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:35:16.331137 sssimp-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-15 04:35:07.000000 sssimp-0.1.1/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:35:16.323137 sssimp-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:35:16.327137 sssimp-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-15 04:35:07.000000 sssimp-0.1.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-15 04:35:07.000000 sssimp-0.1.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-15 04:35:07.000000 sssimp-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-15 04:35:07.000000 sssimp-0.1.1/DEVELOPER_README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-15 04:35:07.000000 sssimp-0.1.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-15 04:35:07.000000 sssimp-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-15 04:35:07.000000 sssimp-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-05-15 04:35:16.331137 sssimp-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-05-15 04:35:07.000000 sssimp-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:35:16.323137 sssimp-0.1.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:35:16.323137 sssimp-0.1.1/examples/01-basic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:35:16.323137 sssimp-0.1.1/examples/01-basic/input/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:35:16.327137 sssimp-0.1.1/examples/01-basic/input/content/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-15 04:35:07.000000 sssimp-0.1.1/examples/01-basic/input/content/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:35:16.327137 sssimp-0.1.1/examples/01-basic/input/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-15 04:35:07.000000 sssimp-0.1.1/examples/01-basic/input/templates/base.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:35:16.327137 sssimp-0.1.1/examples/01-basic/output/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-15 04:35:07.000000 sssimp-0.1.1/examples/01-basic/output/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:35:16.323137 sssimp-0.1.1/examples/02-blog-with-markdown-pages/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:35:16.323137 sssimp-0.1.1/examples/02-blog-with-markdown-pages/input/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:35:16.327137 sssimp-0.1.1/examples/02-blog-with-markdown-pages/input/content/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-15 04:35:07.000000 sssimp-0.1.1/examples/02-blog-with-markdown-pages/input/content/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:35:16.327137 sssimp-0.1.1/examples/02-blog-with-markdown-pages/input/content/post/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-15 04:35:07.000000 sssimp-0.1.1/examples/02-blog-with-markdown-pages/input/content/post/first.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:35:16.327137 sssimp-0.1.1/examples/02-blog-with-markdown-pages/input/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-15 04:35:07.000000 sssimp-0.1.1/examples/02-blog-with-markdown-pages/input/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-15 04:35:07.000000 sssimp-0.1.1/examples/02-blog-with-markdown-pages/input/templates/post.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:35:16.327137 sssimp-0.1.1/examples/02-blog-with-markdown-pages/output/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-15 04:35:07.000000 sssimp-0.1.1/examples/02-blog-with-markdown-pages/output/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:35:16.327137 sssimp-0.1.1/examples/02-blog-with-markdown-pages/output/post/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-15 04:35:07.000000 sssimp-0.1.1/examples/02-blog-with-markdown-pages/output/post/first.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:35:16.323137 sssimp-0.1.1/examples/03-emojis/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:35:16.323137 sssimp-0.1.1/examples/03-emojis/input/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:35:16.327137 sssimp-0.1.1/examples/03-emojis/input/content/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 04:35:07.000000 sssimp-0.1.1/examples/03-emojis/input/content/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:35:16.327137 sssimp-0.1.1/examples/03-emojis/input/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 04:35:07.000000 sssimp-0.1.1/examples/03-emojis/input/templates/content.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:35:16.327137 sssimp-0.1.1/examples/03-emojis/output/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-15 04:35:07.000000 sssimp-0.1.1/examples/03-emojis/output/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-15 04:35:07.000000 sssimp-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 04:35:16.331137 sssimp-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:35:16.323137 sssimp-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:35:16.327137 sssimp-0.1.1/src/sssimp/
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-15 04:35:07.000000 sssimp-0.1.1/src/sssimp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-15 04:35:07.000000 sssimp-0.1.1/src/sssimp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-15 04:35:07.000000 sssimp-0.1.1/src/sssimp/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-15 04:35:07.000000 sssimp-0.1.1/src/sssimp/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:35:16.331137 sssimp-0.1.1/src/sssimp/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-15 04:35:07.000000 sssimp-0.1.1/src/sssimp/generators/css.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-15 04:35:07.000000 sssimp-0.1.1/src/sssimp/generators/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-15 04:35:07.000000 sssimp-0.1.1/src/sssimp/generators/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-05-15 04:35:07.000000 sssimp-0.1.1/src/sssimp/generators/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-15 04:35:07.000000 sssimp-0.1.1/src/sssimp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:35:16.331137 sssimp-0.1.1/src/sssimp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-05-15 04:35:16.000000 sssimp-0.1.1/src/sssimp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-15 04:35:16.000000 sssimp-0.1.1/src/sssimp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 04:35:16.000000 sssimp-0.1.1/src/sssimp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-15 04:35:16.000000 sssimp-0.1.1/src/sssimp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-15 04:35:16.000000 sssimp-0.1.1/src/sssimp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 04:35:16.000000 sssimp-0.1.1/src/sssimp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:35:16.331137 sssimp-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-15 04:35:07.000000 sssimp-0.1.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-15 04:35:07.000000 sssimp-0.1.1/tests/test_examples.py
```

### Comparing `sssimp-0.1.0/.github/workflows/ci.yml` & `sssimp-0.1.1/.github/workflows/ci.yml`

 * *Files 9% similar despite different names*

```diff
@@ -27,15 +27,17 @@
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
         cache: pip
 
     - name: Install package
-      run: pip install -e .
+      run: |
+        pip install -U pip
+        pip install -e .
 
     - name: Check Python version
       run: python -V
 
     - name: List Python dependencies
       run: pip freeze
```

### Comparing `sssimp-0.1.0/.github/workflows/release.yml` & `sssimp-0.1.1/.github/workflows/release.yml`

 * *Files 20% similar despite different names*

```diff
@@ -21,25 +21,24 @@
   release:
     name: Release ${{ github.event.release.tag_name || inputs.version_name }}
     permissions:
       id-token: write
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
+        with:
+          fetch-depth: 0
 
       - name: Set up Python
         uses: actions/setup-python@v5
-        with:
-          cache: pip
 
       - name: Build
         env:
           SETUPTOOLS_SCM_PRETEND_VERSION: ${{ inputs.version_name }}
         run: |
-          echo Got env version: $SETUPTOOLS_SCM_PRETEND_VERSION
           python -m pip install --upgrade pip
           pip install build
           python -m build
 
       - name: Store build artifact
         uses: actions/upload-artifact@v4
         with:
```

### Comparing `sssimp-0.1.0/DEVELOPER_README.md` & `sssimp-0.1.1/DEVELOPER_README.md`

 * *Files identical despite different names*

### Comparing `sssimp-0.1.0/LICENSE` & `sssimp-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sssimp-0.1.0/PKG-INFO` & `sssimp-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sssimp
-Version: 0.1.0
+Version: 0.1.1
 Summary: The Static Site Solution In Modern Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jinja2
 Requires-Dist: markdown
 Requires-Dist: pymdown-extensions
 Requires-Dist: pyyaml
```

### Comparing `sssimp-0.1.0/README.md` & `sssimp-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sssimp-0.1.0/src/sssimp/__init__.py` & `sssimp-0.1.1/src/sssimp/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 from jinja2 import Environment, FileSystemLoader
 
 from . import config
 
 __pkg__ = __name__.split(".")[-1]
 __version__ = importlib.metadata.version(__pkg__)
-print(f"sssimp version {__version__}")
 
 APP_DIR = Path(__file__).parent
 INPUT_DIR = Path(config.INPUT_PATH)
 OUTPUT_DIR = Path(config.OUTPUT_PATH)
 IGNORE_ASSETS = set()
 
 CONTENT_DIR = None
```

### Comparing `sssimp-0.1.0/src/sssimp/__main__.py` & `sssimp-0.1.1/src/sssimp/__main__.py`

 * *Files identical despite different names*

### Comparing `sssimp-0.1.0/src/sssimp/config.py` & `sssimp-0.1.1/src/sssimp/config.py`

 * *Files identical despite different names*

### Comparing `sssimp-0.1.0/src/sssimp/generators/css.py` & `sssimp-0.1.1/src/sssimp/generators/css.py`

 * *Files identical despite different names*

### Comparing `sssimp-0.1.0/src/sssimp/generators/data.py` & `sssimp-0.1.1/src/sssimp/generators/data.py`

 * *Files identical despite different names*

### Comparing `sssimp-0.1.0/src/sssimp/generators/html.py` & `sssimp-0.1.1/src/sssimp/generators/html.py`

 * *Files identical despite different names*

### Comparing `sssimp-0.1.0/src/sssimp/generators/markdown.py` & `sssimp-0.1.1/src/sssimp/generators/markdown.py`

 * *Files identical despite different names*

### Comparing `sssimp-0.1.0/src/sssimp/utils.py` & `sssimp-0.1.1/src/sssimp/utils.py`

 * *Files identical despite different names*

### Comparing `sssimp-0.1.0/src/sssimp.egg-info/PKG-INFO` & `sssimp-0.1.1/src/sssimp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sssimp
-Version: 0.1.0
+Version: 0.1.1
 Summary: The Static Site Solution In Modern Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jinja2
 Requires-Dist: markdown
 Requires-Dist: pymdown-extensions
 Requires-Dist: pyyaml
```

### Comparing `sssimp-0.1.0/src/sssimp.egg-info/SOURCES.txt` & `sssimp-0.1.1/src/sssimp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sssimp-0.1.0/tests/test_examples.py` & `sssimp-0.1.1/tests/test_examples.py`

 * *Files identical despite different names*

