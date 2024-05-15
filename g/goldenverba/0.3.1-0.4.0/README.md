# Comparing `tmp/goldenverba-0.3.1.tar.gz` & `tmp/goldenverba-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goldenverba-0.3.1.tar", last modified: Thu Nov 30 15:10:23 2023, max compression
+gzip compressed data, was "goldenverba-0.4.0.tar", last modified: Fri Apr 12 08:31:49 2024, max compression
```

## Comparing `goldenverba-0.3.1.tar` & `goldenverba-0.4.0.tar`

### file list

```diff
@@ -1,309 +1,310 @@
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.493913 goldenverba-0.3.1/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     1503 2023-08-28 22:41:46.000000 goldenverba-0.3.1/LICENSE
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)       51 2023-09-03 01:59:31.000000 goldenverba-0.3.1/MANIFEST.in
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)    21264 2023-11-30 15:10:23.493655 goldenverba-0.3.1/PKG-INFO
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)    19498 2023-11-24 13:27:33.000000 goldenverba-0.3.1/README.md
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.445860 goldenverba-0.3.1/goldenverba/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)        0 2023-08-24 22:33:30.000000 goldenverba-0.3.1/goldenverba/__init__.py
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.447107 goldenverba-0.3.1/goldenverba/components/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)        0 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/components/__init__.py
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.448182 goldenverba-0.3.1/goldenverba/components/chunking/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)        0 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/components/chunking/__init__.py
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     2231 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/components/chunking/chunk.py
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     1041 2023-11-24 13:42:44.000000 goldenverba-0.3.1/goldenverba/components/chunking/interface.py
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     2574 2023-11-24 13:43:44.000000 goldenverba-0.3.1/goldenverba/components/chunking/manager.py
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3067 2023-11-24 13:39:05.000000 goldenverba-0.3.1/goldenverba/components/chunking/sentencechunker.py
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     2995 2023-11-24 13:39:05.000000 goldenverba-0.3.1/goldenverba/components/chunking/tiktokenchunker.py
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     2932 2023-11-24 13:39:05.000000 goldenverba-0.3.1/goldenverba/components/chunking/wordchunker.py
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      265 2023-11-24 13:39:05.000000 goldenverba-0.3.1/goldenverba/components/component.py
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.449032 goldenverba-0.3.1/goldenverba/components/embedding/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     1011 2023-11-24 13:39:05.000000 goldenverba-0.3.1/goldenverba/components/embedding/ADAEmbedder.py
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     1021 2023-11-24 13:39:05.000000 goldenverba-0.3.1/goldenverba/components/embedding/CohereEmbedder.py
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     4181 2023-11-24 14:02:23.000000 goldenverba-0.3.1/goldenverba/components/embedding/MiniLMEmbedder.py
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)        0 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/components/embedding/__init__.py
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)    14208 2023-11-29 11:00:54.000000 goldenverba-0.3.1/goldenverba/components/embedding/interface.py
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     1567 2023-11-24 13:39:05.000000 goldenverba-0.3.1/goldenverba/components/embedding/manager.py
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.449941 goldenverba-0.3.1/goldenverba/components/generation/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     5770 2023-11-24 13:39:05.000000 goldenverba-0.3.1/goldenverba/components/generation/CohereGenerator.py
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      362 2023-11-24 13:39:05.000000 goldenverba-0.3.1/goldenverba/components/generation/GPT3Generator.py
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     5262 2023-11-29 11:00:54.000000 goldenverba-0.3.1/goldenverba/components/generation/GPT4Generator.py
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     7442 2023-11-24 13:39:05.000000 goldenverba-0.3.1/goldenverba/components/generation/Llama2Generator.py
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)        0 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/components/generation/__init__.py
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     2972 2023-11-24 13:39:05.000000 goldenverba-0.3.1/goldenverba/components/generation/interface.py
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     5185 2023-11-24 13:39:05.000000 goldenverba-0.3.1/goldenverba/components/generation/manager.py
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.450901 goldenverba-0.3.1/goldenverba/components/reader/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)        0 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/components/reader/__init__.py
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     2359 2023-11-24 13:39:05.000000 goldenverba-0.3.1/goldenverba/components/reader/document.py
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     5380 2023-11-24 13:39:05.000000 goldenverba-0.3.1/goldenverba/components/reader/githubreader.py
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     1268 2023-11-24 13:39:05.000000 goldenverba-0.3.1/goldenverba/components/reader/interface.py
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     2057 2023-11-24 13:39:05.000000 goldenverba-0.3.1/goldenverba/components/reader/manager.py
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     5103 2023-11-24 13:39:05.000000 goldenverba-0.3.1/goldenverba/components/reader/pdfreader.py
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     6551 2023-11-24 13:39:05.000000 goldenverba-0.3.1/goldenverba/components/reader/simplereader.py
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     7169 2023-11-24 13:39:05.000000 goldenverba-0.3.1/goldenverba/components/reader/unstructuredpdf.py
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.451902 goldenverba-0.3.1/goldenverba/components/retriever/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     2937 2023-11-24 13:39:05.000000 goldenverba-0.3.1/goldenverba/components/retriever/SimpleRetriever.py
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     7145 2023-11-24 13:39:05.000000 goldenverba-0.3.1/goldenverba/components/retriever/WindowRetriever.py
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)        0 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/components/retriever/__init__.py
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     1753 2023-11-24 13:39:05.000000 goldenverba-0.3.1/goldenverba/components/retriever/interface.py
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     1808 2023-11-24 13:39:05.000000 goldenverba-0.3.1/goldenverba/components/retriever/manager.py
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.452170 goldenverba-0.3.1/goldenverba/components/schema/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)        0 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/components/schema/__init__.py
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)    11548 2023-11-29 11:00:54.000000 goldenverba-0.3.1/goldenverba/components/schema/schema_generation.py
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.452823 goldenverba-0.3.1/goldenverba/server/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3111 2023-11-24 13:56:08.000000 goldenverba-0.3.1/goldenverba/server/ConfigManager.py
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)        0 2023-08-28 20:08:33.000000 goldenverba-0.3.1/goldenverba/server/__init__.py
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)    21511 2023-11-29 11:11:56.000000 goldenverba-0.3.1/goldenverba/server/api.py
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     1688 2023-11-24 13:51:36.000000 goldenverba-0.3.1/goldenverba/server/cli.py
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.441119 goldenverba-0.3.1/goldenverba/server/frontend/
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.454700 goldenverba-0.3.1/goldenverba/server/frontend/out/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3292 2023-11-30 15:07:15.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/404.html
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.441275 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.444799 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.455004 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/0Hcan7GeSF1TuouAgzveb/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      604 2023-08-30 04:02:48.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/0Hcan7GeSF1TuouAgzveb/_buildManifest.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-08-30 04:02:48.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/0Hcan7GeSF1TuouAgzveb/_ssgManifest.js
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.455299 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/1NMt8wGsnxJQdeutSmA9v/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      497 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/1NMt8wGsnxJQdeutSmA9v/_buildManifest.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/1NMt8wGsnxJQdeutSmA9v/_ssgManifest.js
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.455717 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/5fzR3LERKY5UlE9ayIEWy/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      604 2023-08-30 19:29:26.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/5fzR3LERKY5UlE9ayIEWy/_buildManifest.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-08-30 19:29:26.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/5fzR3LERKY5UlE9ayIEWy/_ssgManifest.js
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.456117 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/6c9k90mH-rjwK1B9LzHsB/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      497 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/6c9k90mH-rjwK1B9LzHsB/_buildManifest.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/6c9k90mH-rjwK1B9LzHsB/_ssgManifest.js
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.456451 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/9WTnC4rG27AkPhupgE6uD/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      497 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/9WTnC4rG27AkPhupgE6uD/_buildManifest.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/9WTnC4rG27AkPhupgE6uD/_ssgManifest.js
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.456768 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/A4tVXjpGyJ80L5yK9Jv_a/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      497 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/A4tVXjpGyJ80L5yK9Jv_a/_buildManifest.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/A4tVXjpGyJ80L5yK9Jv_a/_ssgManifest.js
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.457058 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/BrKix8hVmzKkq4nA40XDY/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      604 2023-08-31 19:36:39.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/BrKix8hVmzKkq4nA40XDY/_buildManifest.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-08-31 19:36:39.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/BrKix8hVmzKkq4nA40XDY/_ssgManifest.js
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.457345 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/E3xJxzpNDa7hQ9ErbEuyX/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      604 2023-08-28 21:11:00.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/E3xJxzpNDa7hQ9ErbEuyX/_buildManifest.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-08-28 21:11:00.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/E3xJxzpNDa7hQ9ErbEuyX/_ssgManifest.js
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.457622 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/Ej9O_hZ3RDAnJYJlOxclF/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      604 2023-08-30 04:08:48.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/Ej9O_hZ3RDAnJYJlOxclF/_buildManifest.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-08-30 04:08:48.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/Ej9O_hZ3RDAnJYJlOxclF/_ssgManifest.js
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.457900 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/GGmsoX3roagotCYtIHhEK/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      536 2023-08-29 00:36:02.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/GGmsoX3roagotCYtIHhEK/_buildManifest.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-08-29 00:36:02.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/GGmsoX3roagotCYtIHhEK/_ssgManifest.js
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.458186 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/ILMNARBNbGt2yq7ZzMBNx/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      497 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/ILMNARBNbGt2yq7ZzMBNx/_buildManifest.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/ILMNARBNbGt2yq7ZzMBNx/_ssgManifest.js
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.458451 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/LOGPBr3YJGwfR-CjPs6Bv/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      426 2023-09-03 02:03:37.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/LOGPBr3YJGwfR-CjPs6Bv/_buildManifest.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-09-03 02:03:37.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/LOGPBr3YJGwfR-CjPs6Bv/_ssgManifest.js
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.458720 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/LgB67yeDij4th8wsrC2eS/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      497 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/LgB67yeDij4th8wsrC2eS/_buildManifest.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/LgB67yeDij4th8wsrC2eS/_ssgManifest.js
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.458975 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/NnjBs5HkyOiVgbYuj7tdV/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      604 2023-08-30 23:41:07.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/NnjBs5HkyOiVgbYuj7tdV/_buildManifest.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-08-30 23:41:07.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/NnjBs5HkyOiVgbYuj7tdV/_ssgManifest.js
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.459262 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/RwEhtmsT64md9fQr26tCz/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      604 2023-09-01 01:08:31.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/RwEhtmsT64md9fQr26tCz/_buildManifest.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-09-01 01:08:31.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/RwEhtmsT64md9fQr26tCz/_ssgManifest.js
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.459548 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/S-_u12TvmUTLlw1RLiYOf/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      497 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/S-_u12TvmUTLlw1RLiYOf/_buildManifest.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/S-_u12TvmUTLlw1RLiYOf/_ssgManifest.js
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.459821 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/Uqm0JJ5Jfn42pkmmXyi8G/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      497 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/Uqm0JJ5Jfn42pkmmXyi8G/_buildManifest.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/Uqm0JJ5Jfn42pkmmXyi8G/_ssgManifest.js
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.460097 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/YWcefBRkmSyHlQU9oZZh2/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      604 2023-08-28 21:11:16.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/YWcefBRkmSyHlQU9oZZh2/_buildManifest.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-08-28 21:11:16.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/YWcefBRkmSyHlQU9oZZh2/_ssgManifest.js
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.460375 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/YrNhgjW3p56rd3HOLzh1M/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      497 2023-11-24 14:34:07.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/YrNhgjW3p56rd3HOLzh1M/_buildManifest.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-11-24 14:34:07.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/YrNhgjW3p56rd3HOLzh1M/_ssgManifest.js
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.460660 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/a4aifz2A_sNzaC7VcEnF8/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      497 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/a4aifz2A_sNzaC7VcEnF8/_buildManifest.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/a4aifz2A_sNzaC7VcEnF8/_ssgManifest.js
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.470171 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     9309 2023-08-30 04:08:48.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/172-06f3679cd389db14.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8335 2023-08-28 21:14:44.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/172-11387f2fea15f8f4.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     9650 2023-09-01 01:08:31.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/172-2aea64d5cb024338.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     9578 2023-08-30 23:41:07.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/172-50c469fb388350d4.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8356 2023-08-29 00:48:28.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/172-742d06afbbb76b32.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     9289 2023-08-30 04:02:48.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/172-a717b482738a1ff0.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8371 2023-08-29 00:36:02.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/172-a88687749eea2f07.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8374 2023-08-29 00:18:31.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/172-ac22d29ac37ed486.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8789 2023-08-29 02:45:18.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/172-c660cbf18f8cc710.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     9308 2023-08-30 19:29:26.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/172-f543cedc6ac6c1ac.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)   930959 2023-08-29 02:45:18.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/243-f34295e3a57adcf7.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)    52330 2023-11-30 15:07:15.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/246-8cba9c3e138a3cf5.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     9703 2023-09-03 02:03:37.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/280-52c3b45a7bca32e8.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     9703 2023-10-17 13:43:24.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/280-74dc7793334d9da5.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     9703 2023-08-29 00:36:02.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/280-a161d7ce2cd7eb6e.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     9703 2023-08-29 02:45:18.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/280-e826f6179b5d8b6c.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)   942984 2023-09-01 01:08:31.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/611-ee9176c9cb6e0276.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)   927573 2023-08-29 00:36:02.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/866-b84c52f36b76def1.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)   927573 2023-08-29 00:48:28.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/866-cfe4bf209f60b238.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)   160772 2023-11-30 15:07:15.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/fd9d1056-c06adc43b46a9300.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)   141000 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/framework-2a1230696ef28269.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)   140987 2023-09-01 01:08:31.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/framework-5d6069c3c7124ee8.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)   141000 2023-11-30 15:07:15.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/framework-7b01e204987c8f43.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)   141000 2023-09-03 02:03:37.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/framework-a57e57d99425abb1.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)   140987 2023-08-29 02:45:18.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/framework-cae5c8fdcf4818e7.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)   140987 2023-08-29 00:36:02.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/framework-fe67c9122aecf131.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)    99362 2023-10-17 13:43:24.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/main-2ecc162bcf5a8331.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)    99362 2023-08-29 00:36:02.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/main-4d54ae8f14f9d7c6.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)    99362 2023-08-29 02:45:18.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/main-8d39882388fd6605.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)    99362 2023-09-03 02:03:37.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/main-a7f2fdd54fd24f53.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)    98439 2023-11-30 15:07:15.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/main-app-a515e76320e72f2c.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)    99362 2023-11-30 15:07:15.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/main-c9732fa3c1d6d1d5.js
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.486134 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)  1005651 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-097dde0f604a216d.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8224 2023-08-30 23:41:07.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-2e4b2bc90e8e9cf0.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)  1005762 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-2f0b49097296ab3b.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)   999343 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-44bc0a53432c2305.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8224 2023-08-30 04:08:48.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-4ad389329d5c5db0.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)  1010133 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-4b7391532c7f4bd1.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8234 2023-09-01 01:08:31.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-4b7688a8f49a037e.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8224 2023-08-30 19:29:26.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-555bac3d60ed6cce.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8047 2023-08-29 00:48:28.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-5914f88957706be3.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)  1008816 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-5d055a73ecc2e4bb.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8047 2023-08-29 00:36:02.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-73b84b7c4b745f50.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)   978446 2023-11-30 15:07:15.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-7a548c247b0896b0.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)   978446 2023-11-24 14:34:07.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-7b8d7f1c795cadf6.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8047 2023-08-29 02:45:18.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-877f2c40f1814452.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)  1010283 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-8ae9faf463bff6e8.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8209 2023-08-30 04:02:48.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-905162599335727d.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8047 2023-08-28 21:11:16.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-93747ea226addaf4.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)  1005664 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-95b570e3c384ee1a.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)   961579 2023-09-03 02:03:37.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-a0957af8bafb5c75.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)  1005648 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-a5604af5bf4aeb92.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)  1010624 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-b7fba87b2821fa1b.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)  1010665 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-d6fe3ed4752599cf.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)  1003159 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-f48f66f2530dcab1.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      250 2023-11-30 15:07:15.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_error-b190518070b21757.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      537 2023-09-01 01:08:31.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/about-5eabeb8efb0f0a5d.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      537 2023-08-29 02:45:18.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/about-772e84e976153ce1.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     6431 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-0e4cc95fa680cb1b.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     6804 2023-11-30 15:07:15.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-16e4de29624eb562.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3803 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-3b64a7f4f0744605.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3591 2023-08-30 19:29:26.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-55171382bcb992de.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3803 2023-09-03 02:03:37.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-6dcac899c9312be7.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     6804 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-896e2841c08a0cf2.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     2905 2023-08-29 02:45:18.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-8dc7615e9ee51133.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     6431 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-a675a1f7ad7744a6.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     6378 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-abac488ca017417d.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     2820 2023-08-29 00:48:28.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-bb1f65e19dfc1c0e.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     2811 2023-08-29 00:18:31.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-c8a428b01649242c.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     6795 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-ccca135591a6180e.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     2820 2023-08-29 00:36:02.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-f2b168e3e47ba8a4.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3811 2023-09-01 01:08:31.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-ff456efe0bddd068.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      252 2023-08-29 00:36:02.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/index-1c4e2fc04775023d.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      244 2023-11-30 15:07:15.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/index-491c7585514c00a2.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      244 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/index-4987ba5705ee324e.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      252 2023-08-29 00:18:31.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/index-56e8765bfd3090f9.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      252 2023-09-01 01:08:31.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/index-587c8a189d07a085.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      244 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/index-9f6e98911fb8574f.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      244 2023-09-03 02:03:37.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/index-a73625c90fdfb416.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      252 2023-08-29 02:45:18.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/index-d05849ff4daf0f98.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      244 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/index-e13c92a1e1e5cdf5.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      252 2023-08-29 00:48:28.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/index-e8085669191fdd83.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     6771 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/status-03d0ba488ee360ad.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     5582 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/status-36bfa2eb3ce44652.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8624 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/status-3e09625e9decd386.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8615 2023-11-30 15:07:15.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/status-5eecffe6be63ff44.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8589 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/status-7d60916a01bd3f1e.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     6771 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/status-ca571a484838e88c.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8630 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/status-f1bcadfcd1e3bb61.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     5706 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/status-fdb704cca997e4eb.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)    91381 2023-11-30 15:07:15.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3264 2023-09-03 02:03:37.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/webpack-4231116f672e6062.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3264 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/webpack-49c0ce1495d0fca6.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3264 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/webpack-4c9086a613e9f796.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3264 2023-11-30 15:07:15.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/webpack-67916544a50891e6.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3264 2023-08-30 19:29:26.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/webpack-7dec9f7d48b7e6f8.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3264 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/webpack-929d3d7cef65c790.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3264 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/webpack-962cf26a2870754f.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3264 2023-08-29 02:45:18.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/webpack-973edf575a1afde9.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3264 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/webpack-ad6a98aa3061f47c.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3264 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/webpack-b82d5cfb9ad31867.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3264 2023-08-29 00:48:28.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/webpack-d9150ed736d780c1.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3264 2023-08-30 23:41:07.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/webpack-e3fb025be7fc31b6.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3264 2023-08-30 04:08:48.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/webpack-e8ca2e84678d9188.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3264 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/webpack-f137e28ede23552f.js
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.486471 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/ciXFpmau1SdpuSwnS4h7-/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      604 2023-08-29 00:48:28.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/ciXFpmau1SdpuSwnS4h7-/_buildManifest.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-08-29 00:48:28.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/ciXFpmau1SdpuSwnS4h7-/_ssgManifest.js
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.488578 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/css/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)    14848 2023-08-29 00:48:28.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/css/0498f7c446a726e9.css
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)    21227 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/css/1d3dba75de6e341d.css
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)    21398 2023-11-30 15:07:15.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/css/230b09fe1800464e.css
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)    21793 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/css/29fa82f47e877363.css
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)    21479 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/css/5eae4c2ec3051cd7.css
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)    21377 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/css/5f29c576294b8875.css
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)    15894 2023-08-30 19:29:26.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/css/6b9a855a65274a9d.css
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)    19665 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/css/8e73cf102487ac8c.css
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)    16143 2023-09-03 02:03:37.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/css/ba3601c7d877a774.css
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)    15373 2023-08-29 02:45:18.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/css/da2f78b33f664c71.css
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)    22183 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/css/ddc29201eb54d38e.css
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)    15849 2023-08-30 23:41:07.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/css/eb3caac5e60c1076.css
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)    21879 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/css/eb98ddacea444f62.css
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)    15826 2023-08-30 04:08:48.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/css/f27c22d149b2a6fe.css
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.488867 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/dFAJVlvKY7TnN7l9nf2qs/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      497 2023-11-30 15:07:15.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/dFAJVlvKY7TnN7l9nf2qs/_buildManifest.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-11-30 15:07:15.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/dFAJVlvKY7TnN7l9nf2qs/_ssgManifest.js
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.489292 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/dfMAlIoliIRpjDLblym_G/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      497 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/dfMAlIoliIRpjDLblym_G/_buildManifest.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/dfMAlIoliIRpjDLblym_G/_ssgManifest.js
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.489634 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/gUcs07ZbtynTe2mkLh-Xl/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      497 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/gUcs07ZbtynTe2mkLh-Xl/_buildManifest.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/gUcs07ZbtynTe2mkLh-Xl/_ssgManifest.js
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.489905 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/iEUc8h1kuYG09fdVawI1I/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      426 2023-09-01 16:56:21.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/iEUc8h1kuYG09fdVawI1I/_buildManifest.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-09-01 16:56:21.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/iEUc8h1kuYG09fdVawI1I/_ssgManifest.js
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.490173 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/jvIZeMAH6w8GF8zRcPJET/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      604 2023-08-29 00:18:31.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/jvIZeMAH6w8GF8zRcPJET/_buildManifest.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-08-29 00:18:31.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/jvIZeMAH6w8GF8zRcPJET/_ssgManifest.js
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.490455 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/kBlJ9ovXshnAFh_k1E86k/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      604 2023-08-29 02:45:18.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/kBlJ9ovXshnAFh_k1E86k/_buildManifest.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-08-29 02:45:18.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/kBlJ9ovXshnAFh_k1E86k/_ssgManifest.js
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.490996 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/media/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     9948 2023-11-30 15:07:15.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/media/4049f3f580e14086-s.p.woff2
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     6148 2023-11-30 15:07:15.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/media/84a5d21698cdcea6-s.woff2
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     6036 2023-11-30 15:07:15.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/media/a1471ccaedd577d0-s.woff2
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     7560 2023-11-30 15:07:15.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/media/df5e9368d28a76aa-s.woff2
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.491266 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/omi7_40LiFc7ffqeF9LU9/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      497 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/omi7_40LiFc7ffqeF9LU9/_buildManifest.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/omi7_40LiFc7ffqeF9LU9/_ssgManifest.js
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.491585 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/sM8hBealmuWXY2gB-kAfp/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      497 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/sM8hBealmuWXY2gB-kAfp/_buildManifest.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/sM8hBealmuWXY2gB-kAfp/_ssgManifest.js
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.491839 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/snAppvnalMWaRCvQfPtCc/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      497 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/snAppvnalMWaRCvQfPtCc/_buildManifest.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/snAppvnalMWaRCvQfPtCc/_ssgManifest.js
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.492093 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/ubExhBPJs8XjBl3DLyfkW/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      497 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/ubExhBPJs8XjBl3DLyfkW/_buildManifest.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/ubExhBPJs8XjBl3DLyfkW/_ssgManifest.js
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.492344 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/vv1EB3RpwUwq255x5fhm7/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      604 2023-08-28 21:14:44.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/vv1EB3RpwUwq255x5fhm7/_buildManifest.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-08-28 21:14:44.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/vv1EB3RpwUwq255x5fhm7/_ssgManifest.js
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.492612 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/xRSGMqhmPvAA9Z6NGYvwF/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      497 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/xRSGMqhmPvAA9Z6NGYvwF/_buildManifest.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/xRSGMqhmPvAA9Z6NGYvwF/_ssgManifest.js
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     2337 2023-09-01 01:08:31.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/about.html
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)    39992 2023-11-30 15:07:15.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/background.png
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     6137 2023-11-30 15:07:15.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/document_explorer.html
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)    25931 2023-11-30 15:07:15.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/favicon.ico
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)    80645 2023-11-30 15:07:15.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/favicon.png
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8338 2023-11-30 15:07:15.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/index.html
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     1375 2023-11-30 15:07:15.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/next.svg
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     6418 2023-11-30 15:07:15.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/status.html
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)    87366 2023-11-30 15:07:15.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/verba.png
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      629 2023-11-30 15:07:15.000000 goldenverba-0.3.1/goldenverba/server/frontend/out/vercel.svg
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     5033 2023-11-13 09:29:47.000000 goldenverba-0.3.1/goldenverba/server/util.py
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)    22686 2023-11-29 11:20:43.000000 goldenverba-0.3.1/goldenverba/verba_manager.py
-drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2023-11-30 15:10:23.446843 goldenverba-0.3.1/goldenverba.egg-info/
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)    21264 2023-11-30 15:10:23.000000 goldenverba-0.3.1/goldenverba.egg-info/PKG-INFO
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)    18200 2023-11-30 15:10:23.000000 goldenverba-0.3.1/goldenverba.egg-info/SOURCES.txt
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)        1 2023-11-30 15:10:23.000000 goldenverba-0.3.1/goldenverba.egg-info/dependency_links.txt
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)       53 2023-11-30 15:10:23.000000 goldenverba-0.3.1/goldenverba.egg-info/entry_points.txt
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)      333 2023-11-30 15:10:23.000000 goldenverba-0.3.1/goldenverba.egg-info/requires.txt
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)       12 2023-11-30 15:10:23.000000 goldenverba-0.3.1/goldenverba.egg-info/top_level.txt
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     1989 2023-11-24 13:57:52.000000 goldenverba-0.3.1/pyproject.toml
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)       38 2023-11-30 15:10:23.493962 goldenverba-0.3.1/setup.cfg
--rw-r--r--   0 edwardschmuhl   (501) staff       (20)     1885 2023-11-30 15:09:26.000000 goldenverba-0.3.1/setup.py
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.702812 goldenverba-0.4.0/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     1503 2023-08-28 22:41:46.000000 goldenverba-0.4.0/LICENSE
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       51 2023-09-03 01:59:31.000000 goldenverba-0.4.0/MANIFEST.in
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)    22982 2024-04-12 08:31:49.702558 goldenverba-0.4.0/PKG-INFO
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)    21360 2024-04-12 08:24:34.000000 goldenverba-0.4.0/README.md
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.597705 goldenverba-0.4.0/goldenverba/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)        0 2023-08-24 22:33:30.000000 goldenverba-0.4.0/goldenverba/__init__.py
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.599039 goldenverba-0.4.0/goldenverba/components/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)        0 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/components/__init__.py
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.600155 goldenverba-0.4.0/goldenverba/components/chunking/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)        0 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/components/chunking/__init__.py
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     2231 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/components/chunking/chunk.py
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     1041 2023-11-24 13:42:44.000000 goldenverba-0.4.0/goldenverba/components/chunking/interface.py
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     2338 2024-04-11 12:37:54.000000 goldenverba-0.4.0/goldenverba/components/chunking/manager.py
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     2995 2023-11-24 13:39:05.000000 goldenverba-0.4.0/goldenverba/components/chunking/tiktokenchunker.py
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      265 2023-11-24 13:39:05.000000 goldenverba-0.4.0/goldenverba/components/component.py
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.602482 goldenverba-0.4.0/goldenverba/components/embedding/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     1011 2023-11-24 13:39:05.000000 goldenverba-0.4.0/goldenverba/components/embedding/ADAEmbedder.py
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     1021 2023-11-24 13:39:05.000000 goldenverba-0.4.0/goldenverba/components/embedding/CohereEmbedder.py
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     4181 2023-11-24 14:02:23.000000 goldenverba-0.4.0/goldenverba/components/embedding/MiniLMEmbedder.py
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)        0 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/components/embedding/__init__.py
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)    14524 2024-02-08 19:27:35.000000 goldenverba-0.4.0/goldenverba/components/embedding/interface.py
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     1567 2023-11-24 13:39:05.000000 goldenverba-0.4.0/goldenverba/components/embedding/manager.py
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.604115 goldenverba-0.4.0/goldenverba/components/generation/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     5770 2023-11-24 13:39:05.000000 goldenverba-0.4.0/goldenverba/components/generation/CohereGenerator.py
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      362 2023-11-24 13:39:05.000000 goldenverba-0.4.0/goldenverba/components/generation/GPT3Generator.py
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     7118 2024-04-11 12:01:41.000000 goldenverba-0.4.0/goldenverba/components/generation/GPT4Generator.py
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     7450 2023-12-05 10:45:19.000000 goldenverba-0.4.0/goldenverba/components/generation/Llama2Generator.py
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)        0 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/components/generation/__init__.py
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     2972 2023-11-24 13:39:05.000000 goldenverba-0.4.0/goldenverba/components/generation/interface.py
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     5185 2023-11-24 13:39:05.000000 goldenverba-0.4.0/goldenverba/components/generation/manager.py
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.606387 goldenverba-0.4.0/goldenverba/components/reader/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)        0 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/components/reader/__init__.py
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     2359 2023-11-24 13:39:05.000000 goldenverba-0.4.0/goldenverba/components/reader/document.py
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     5452 2024-02-08 19:27:35.000000 goldenverba-0.4.0/goldenverba/components/reader/githubreader.py
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     1268 2023-11-24 13:39:05.000000 goldenverba-0.4.0/goldenverba/components/reader/interface.py
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     2057 2023-11-24 13:39:05.000000 goldenverba-0.4.0/goldenverba/components/reader/manager.py
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     5103 2023-11-24 13:39:05.000000 goldenverba-0.4.0/goldenverba/components/reader/pdfreader.py
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     6551 2023-11-24 13:39:05.000000 goldenverba-0.4.0/goldenverba/components/reader/simplereader.py
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     7169 2023-11-24 13:39:05.000000 goldenverba-0.4.0/goldenverba/components/reader/unstructuredpdf.py
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.607643 goldenverba-0.4.0/goldenverba/components/retriever/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     2937 2023-11-24 13:39:05.000000 goldenverba-0.4.0/goldenverba/components/retriever/SimpleRetriever.py
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     7145 2023-11-24 13:39:05.000000 goldenverba-0.4.0/goldenverba/components/retriever/WindowRetriever.py
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)        0 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/components/retriever/__init__.py
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     1753 2023-11-24 13:39:05.000000 goldenverba-0.4.0/goldenverba/components/retriever/interface.py
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     1808 2023-11-24 13:39:05.000000 goldenverba-0.4.0/goldenverba/components/retriever/manager.py
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.607913 goldenverba-0.4.0/goldenverba/components/schema/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)        0 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/components/schema/__init__.py
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)    12419 2024-02-08 19:27:35.000000 goldenverba-0.4.0/goldenverba/components/schema/schema_generation.py
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.609247 goldenverba-0.4.0/goldenverba/server/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3111 2023-11-24 13:56:08.000000 goldenverba-0.4.0/goldenverba/server/ConfigManager.py
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)        0 2023-08-28 20:08:33.000000 goldenverba-0.4.0/goldenverba/server/__init__.py
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)    21511 2023-11-29 11:11:56.000000 goldenverba-0.4.0/goldenverba/server/api.py
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     1686 2023-12-01 12:03:15.000000 goldenverba-0.4.0/goldenverba/server/cli.py
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.593121 goldenverba-0.4.0/goldenverba/server/frontend/
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.611323 goldenverba-0.4.0/goldenverba/server/frontend/out/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3292 2024-04-12 07:53:46.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/404.html
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.593262 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.596722 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.611712 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/0Hcan7GeSF1TuouAgzveb/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      604 2023-08-30 04:02:48.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/0Hcan7GeSF1TuouAgzveb/_buildManifest.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-08-30 04:02:48.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/0Hcan7GeSF1TuouAgzveb/_ssgManifest.js
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.612225 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/1NMt8wGsnxJQdeutSmA9v/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      497 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/1NMt8wGsnxJQdeutSmA9v/_buildManifest.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/1NMt8wGsnxJQdeutSmA9v/_ssgManifest.js
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.612746 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/5fzR3LERKY5UlE9ayIEWy/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      604 2023-08-30 19:29:26.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/5fzR3LERKY5UlE9ayIEWy/_buildManifest.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-08-30 19:29:26.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/5fzR3LERKY5UlE9ayIEWy/_ssgManifest.js
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.613206 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/6c9k90mH-rjwK1B9LzHsB/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      497 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/6c9k90mH-rjwK1B9LzHsB/_buildManifest.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/6c9k90mH-rjwK1B9LzHsB/_ssgManifest.js
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.613548 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/9WTnC4rG27AkPhupgE6uD/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      497 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/9WTnC4rG27AkPhupgE6uD/_buildManifest.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/9WTnC4rG27AkPhupgE6uD/_ssgManifest.js
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.613849 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/A4tVXjpGyJ80L5yK9Jv_a/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      497 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/A4tVXjpGyJ80L5yK9Jv_a/_buildManifest.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/A4tVXjpGyJ80L5yK9Jv_a/_ssgManifest.js
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.614272 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/BrKix8hVmzKkq4nA40XDY/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      604 2023-08-31 19:36:39.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/BrKix8hVmzKkq4nA40XDY/_buildManifest.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-08-31 19:36:39.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/BrKix8hVmzKkq4nA40XDY/_ssgManifest.js
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.614756 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/E3xJxzpNDa7hQ9ErbEuyX/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      604 2023-08-28 21:11:00.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/E3xJxzpNDa7hQ9ErbEuyX/_buildManifest.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-08-28 21:11:00.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/E3xJxzpNDa7hQ9ErbEuyX/_ssgManifest.js
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.615248 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/Ej9O_hZ3RDAnJYJlOxclF/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      604 2023-08-30 04:08:48.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/Ej9O_hZ3RDAnJYJlOxclF/_buildManifest.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-08-30 04:08:48.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/Ej9O_hZ3RDAnJYJlOxclF/_ssgManifest.js
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.615771 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/GGmsoX3roagotCYtIHhEK/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      536 2023-08-29 00:36:02.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/GGmsoX3roagotCYtIHhEK/_buildManifest.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-08-29 00:36:02.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/GGmsoX3roagotCYtIHhEK/_ssgManifest.js
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.616332 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/ILMNARBNbGt2yq7ZzMBNx/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      497 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/ILMNARBNbGt2yq7ZzMBNx/_buildManifest.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/ILMNARBNbGt2yq7ZzMBNx/_ssgManifest.js
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.616781 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/LOGPBr3YJGwfR-CjPs6Bv/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      426 2023-09-03 02:03:37.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/LOGPBr3YJGwfR-CjPs6Bv/_buildManifest.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-09-03 02:03:37.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/LOGPBr3YJGwfR-CjPs6Bv/_ssgManifest.js
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.617157 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/LgB67yeDij4th8wsrC2eS/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      497 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/LgB67yeDij4th8wsrC2eS/_buildManifest.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/LgB67yeDij4th8wsrC2eS/_ssgManifest.js
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.617567 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/NnjBs5HkyOiVgbYuj7tdV/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      604 2023-08-30 23:41:07.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/NnjBs5HkyOiVgbYuj7tdV/_buildManifest.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-08-30 23:41:07.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/NnjBs5HkyOiVgbYuj7tdV/_ssgManifest.js
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.618106 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/RwEhtmsT64md9fQr26tCz/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      604 2023-09-01 01:08:31.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/RwEhtmsT64md9fQr26tCz/_buildManifest.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-09-01 01:08:31.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/RwEhtmsT64md9fQr26tCz/_ssgManifest.js
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.618595 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/S-_u12TvmUTLlw1RLiYOf/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      497 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/S-_u12TvmUTLlw1RLiYOf/_buildManifest.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/S-_u12TvmUTLlw1RLiYOf/_ssgManifest.js
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.618933 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/Uqm0JJ5Jfn42pkmmXyi8G/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      497 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/Uqm0JJ5Jfn42pkmmXyi8G/_buildManifest.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/Uqm0JJ5Jfn42pkmmXyi8G/_ssgManifest.js
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.619412 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/YWcefBRkmSyHlQU9oZZh2/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      604 2023-08-28 21:11:16.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/YWcefBRkmSyHlQU9oZZh2/_buildManifest.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-08-28 21:11:16.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/YWcefBRkmSyHlQU9oZZh2/_ssgManifest.js
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.619946 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/YrNhgjW3p56rd3HOLzh1M/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      497 2023-11-24 14:34:07.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/YrNhgjW3p56rd3HOLzh1M/_buildManifest.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-11-24 14:34:07.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/YrNhgjW3p56rd3HOLzh1M/_ssgManifest.js
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.620307 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/_A-piGxRm1B_OMIwQ_tPn/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      497 2024-04-12 07:53:46.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/_A-piGxRm1B_OMIwQ_tPn/_buildManifest.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2024-04-12 07:53:46.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/_A-piGxRm1B_OMIwQ_tPn/_ssgManifest.js
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.620701 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/a4aifz2A_sNzaC7VcEnF8/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      497 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/a4aifz2A_sNzaC7VcEnF8/_buildManifest.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/a4aifz2A_sNzaC7VcEnF8/_ssgManifest.js
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.646312 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     9309 2023-08-30 04:08:48.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/172-06f3679cd389db14.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8335 2023-08-28 21:14:44.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/172-11387f2fea15f8f4.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     9650 2023-09-01 01:08:31.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/172-2aea64d5cb024338.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     9578 2023-08-30 23:41:07.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/172-50c469fb388350d4.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8356 2023-08-29 00:48:28.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/172-742d06afbbb76b32.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     9289 2023-08-30 04:02:48.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/172-a717b482738a1ff0.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8371 2023-08-29 00:36:02.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/172-a88687749eea2f07.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8374 2023-08-29 00:18:31.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/172-ac22d29ac37ed486.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8789 2023-08-29 02:45:18.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/172-c660cbf18f8cc710.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     9308 2023-08-30 19:29:26.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/172-f543cedc6ac6c1ac.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)   930959 2023-08-29 02:45:18.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/243-f34295e3a57adcf7.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)    52330 2024-04-12 07:53:46.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/246-8cba9c3e138a3cf5.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     9703 2023-09-03 02:03:37.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/280-52c3b45a7bca32e8.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     9703 2023-10-17 13:43:24.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/280-74dc7793334d9da5.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     9703 2023-08-29 00:36:02.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/280-a161d7ce2cd7eb6e.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     9703 2023-08-29 02:45:18.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/280-e826f6179b5d8b6c.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)   942984 2023-09-01 01:08:31.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/611-ee9176c9cb6e0276.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)   927573 2023-08-29 00:36:02.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/866-b84c52f36b76def1.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)   927573 2023-08-29 00:48:28.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/866-cfe4bf209f60b238.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)   160772 2024-04-12 07:53:46.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/fd9d1056-c06adc43b46a9300.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)   141000 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/framework-2a1230696ef28269.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)   140987 2023-09-01 01:08:31.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/framework-5d6069c3c7124ee8.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)   141000 2024-04-12 07:53:46.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/framework-7b01e204987c8f43.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)   141000 2023-09-03 02:03:37.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/framework-a57e57d99425abb1.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)   140987 2023-08-29 02:45:18.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/framework-cae5c8fdcf4818e7.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)   140987 2023-08-29 00:36:02.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/framework-fe67c9122aecf131.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)    99362 2023-10-17 13:43:24.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/main-2ecc162bcf5a8331.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)    99362 2023-08-29 00:36:02.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/main-4d54ae8f14f9d7c6.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)    99362 2023-08-29 02:45:18.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/main-8d39882388fd6605.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)    99362 2023-09-03 02:03:37.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/main-a7f2fdd54fd24f53.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)    98439 2024-04-12 07:53:46.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/main-app-a515e76320e72f2c.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)    99362 2024-04-12 07:53:46.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/main-c9732fa3c1d6d1d5.js
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.691148 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)  1005651 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-097dde0f604a216d.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8224 2023-08-30 23:41:07.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-2e4b2bc90e8e9cf0.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)  1005762 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-2f0b49097296ab3b.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)   999343 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-44bc0a53432c2305.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8224 2023-08-30 04:08:48.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-4ad389329d5c5db0.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)  1010133 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-4b7391532c7f4bd1.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8234 2023-09-01 01:08:31.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-4b7688a8f49a037e.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8224 2023-08-30 19:29:26.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-555bac3d60ed6cce.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8047 2023-08-29 00:48:28.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-5914f88957706be3.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)  1008816 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-5d055a73ecc2e4bb.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8047 2023-08-29 00:36:02.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-73b84b7c4b745f50.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)   978446 2023-11-30 15:07:15.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-7a548c247b0896b0.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)   978446 2023-11-24 14:34:07.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-7b8d7f1c795cadf6.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8047 2023-08-29 02:45:18.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-877f2c40f1814452.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)  1010283 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-8ae9faf463bff6e8.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8209 2023-08-30 04:02:48.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-905162599335727d.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8047 2023-08-28 21:11:16.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-93747ea226addaf4.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)  1005664 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-95b570e3c384ee1a.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)   961579 2023-09-03 02:03:37.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-a0957af8bafb5c75.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)  1005648 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-a5604af5bf4aeb92.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)  1010624 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-b7fba87b2821fa1b.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)   978446 2024-04-12 07:53:46.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-c1589fca75958036.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)  1010665 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-d6fe3ed4752599cf.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)  1003159 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-f48f66f2530dcab1.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      250 2024-04-12 07:53:46.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_error-b190518070b21757.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      537 2023-09-01 01:08:31.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/about-5eabeb8efb0f0a5d.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      537 2023-08-29 02:45:18.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/about-772e84e976153ce1.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     6431 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-0e4cc95fa680cb1b.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     6804 2024-04-12 07:53:46.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-16e4de29624eb562.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3803 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-3b64a7f4f0744605.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3591 2023-08-30 19:29:26.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-55171382bcb992de.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3803 2023-09-03 02:03:37.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-6dcac899c9312be7.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     6804 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-896e2841c08a0cf2.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     2905 2023-08-29 02:45:18.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-8dc7615e9ee51133.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     6431 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-a675a1f7ad7744a6.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     6378 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-abac488ca017417d.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     2820 2023-08-29 00:48:28.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-bb1f65e19dfc1c0e.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     2811 2023-08-29 00:18:31.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-c8a428b01649242c.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     6795 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-ccca135591a6180e.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     2820 2023-08-29 00:36:02.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-f2b168e3e47ba8a4.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3811 2023-09-01 01:08:31.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-ff456efe0bddd068.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      252 2023-08-29 00:36:02.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/index-1c4e2fc04775023d.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      244 2024-04-12 07:53:46.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/index-491c7585514c00a2.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      244 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/index-4987ba5705ee324e.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      252 2023-08-29 00:18:31.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/index-56e8765bfd3090f9.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      252 2023-09-01 01:08:31.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/index-587c8a189d07a085.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      244 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/index-9f6e98911fb8574f.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      244 2023-09-03 02:03:37.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/index-a73625c90fdfb416.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      252 2023-08-29 02:45:18.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/index-d05849ff4daf0f98.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      244 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/index-e13c92a1e1e5cdf5.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      252 2023-08-29 00:48:28.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/index-e8085669191fdd83.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     6771 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/status-03d0ba488ee360ad.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     5582 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/status-36bfa2eb3ce44652.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8624 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/status-3e09625e9decd386.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8615 2024-04-12 07:53:46.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/status-5eecffe6be63ff44.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8589 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/status-7d60916a01bd3f1e.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     6771 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/status-ca571a484838e88c.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8630 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/status-f1bcadfcd1e3bb61.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     5706 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/status-fdb704cca997e4eb.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)    91381 2024-04-12 07:53:46.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3264 2023-09-03 02:03:37.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/webpack-4231116f672e6062.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3264 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/webpack-49c0ce1495d0fca6.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3264 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/webpack-4c9086a613e9f796.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3264 2024-04-12 07:53:46.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/webpack-67916544a50891e6.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3264 2023-08-30 19:29:26.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/webpack-7dec9f7d48b7e6f8.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3264 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/webpack-929d3d7cef65c790.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3264 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/webpack-962cf26a2870754f.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3264 2023-08-29 02:45:18.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/webpack-973edf575a1afde9.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3264 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/webpack-ad6a98aa3061f47c.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3264 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/webpack-b82d5cfb9ad31867.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3264 2023-08-29 00:48:28.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/webpack-d9150ed736d780c1.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3264 2023-08-30 23:41:07.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/webpack-e3fb025be7fc31b6.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3264 2023-08-30 04:08:48.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/webpack-e8ca2e84678d9188.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     3264 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/webpack-f137e28ede23552f.js
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.691608 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/ciXFpmau1SdpuSwnS4h7-/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      604 2023-08-29 00:48:28.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/ciXFpmau1SdpuSwnS4h7-/_buildManifest.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-08-29 00:48:28.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/ciXFpmau1SdpuSwnS4h7-/_ssgManifest.js
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.695445 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/css/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)    14848 2023-08-29 00:48:28.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/css/0498f7c446a726e9.css
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)    21227 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/css/1d3dba75de6e341d.css
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)    21398 2024-04-12 07:53:46.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/css/230b09fe1800464e.css
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)    21793 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/css/29fa82f47e877363.css
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)    21479 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/css/5eae4c2ec3051cd7.css
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)    21377 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/css/5f29c576294b8875.css
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)    15894 2023-08-30 19:29:26.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/css/6b9a855a65274a9d.css
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)    19665 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/css/8e73cf102487ac8c.css
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)    16143 2023-09-03 02:03:37.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/css/ba3601c7d877a774.css
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)    15373 2023-08-29 02:45:18.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/css/da2f78b33f664c71.css
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)    22183 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/css/ddc29201eb54d38e.css
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)    15849 2023-08-30 23:41:07.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/css/eb3caac5e60c1076.css
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)    21879 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/css/eb98ddacea444f62.css
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)    15826 2023-08-30 04:08:48.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/css/f27c22d149b2a6fe.css
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.696008 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/dFAJVlvKY7TnN7l9nf2qs/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      497 2023-11-30 15:07:15.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/dFAJVlvKY7TnN7l9nf2qs/_buildManifest.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-11-30 15:07:15.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/dFAJVlvKY7TnN7l9nf2qs/_ssgManifest.js
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.696399 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/dfMAlIoliIRpjDLblym_G/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      497 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/dfMAlIoliIRpjDLblym_G/_buildManifest.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/dfMAlIoliIRpjDLblym_G/_ssgManifest.js
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.696705 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/gUcs07ZbtynTe2mkLh-Xl/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      497 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/gUcs07ZbtynTe2mkLh-Xl/_buildManifest.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/gUcs07ZbtynTe2mkLh-Xl/_ssgManifest.js
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.697123 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/iEUc8h1kuYG09fdVawI1I/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      426 2023-09-01 16:56:21.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/iEUc8h1kuYG09fdVawI1I/_buildManifest.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-09-01 16:56:21.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/iEUc8h1kuYG09fdVawI1I/_ssgManifest.js
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.697605 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/jvIZeMAH6w8GF8zRcPJET/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      604 2023-08-29 00:18:31.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/jvIZeMAH6w8GF8zRcPJET/_buildManifest.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-08-29 00:18:31.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/jvIZeMAH6w8GF8zRcPJET/_ssgManifest.js
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.698189 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/kBlJ9ovXshnAFh_k1E86k/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      604 2023-08-29 02:45:18.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/kBlJ9ovXshnAFh_k1E86k/_buildManifest.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-08-29 02:45:18.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/kBlJ9ovXshnAFh_k1E86k/_ssgManifest.js
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.698998 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/media/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     9948 2024-04-12 07:53:46.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/media/4049f3f580e14086-s.p.woff2
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     6148 2024-04-12 07:53:46.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/media/84a5d21698cdcea6-s.woff2
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     6036 2024-04-12 07:53:46.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/media/a1471ccaedd577d0-s.woff2
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     7560 2024-04-12 07:53:46.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/media/df5e9368d28a76aa-s.woff2
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.699427 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/omi7_40LiFc7ffqeF9LU9/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      497 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/omi7_40LiFc7ffqeF9LU9/_buildManifest.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/omi7_40LiFc7ffqeF9LU9/_ssgManifest.js
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.699988 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/sM8hBealmuWXY2gB-kAfp/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      497 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/sM8hBealmuWXY2gB-kAfp/_buildManifest.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/sM8hBealmuWXY2gB-kAfp/_ssgManifest.js
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.700361 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/snAppvnalMWaRCvQfPtCc/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      497 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/snAppvnalMWaRCvQfPtCc/_buildManifest.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/snAppvnalMWaRCvQfPtCc/_ssgManifest.js
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.700643 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/ubExhBPJs8XjBl3DLyfkW/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      497 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/ubExhBPJs8XjBl3DLyfkW/_buildManifest.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/ubExhBPJs8XjBl3DLyfkW/_ssgManifest.js
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.701081 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/vv1EB3RpwUwq255x5fhm7/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      604 2023-08-28 21:14:44.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/vv1EB3RpwUwq255x5fhm7/_buildManifest.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-08-28 21:14:44.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/vv1EB3RpwUwq255x5fhm7/_ssgManifest.js
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.701532 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/xRSGMqhmPvAA9Z6NGYvwF/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      497 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/xRSGMqhmPvAA9Z6NGYvwF/_buildManifest.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       80 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/xRSGMqhmPvAA9Z6NGYvwF/_ssgManifest.js
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     2337 2023-09-01 01:08:31.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/about.html
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)    39992 2024-04-12 07:53:46.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/background.png
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     6137 2024-04-12 07:53:46.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/document_explorer.html
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)    25931 2024-04-12 07:53:46.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/favicon.ico
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)    80645 2024-04-12 07:53:46.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/favicon.png
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     8338 2024-04-12 07:53:46.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/index.html
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     1375 2024-04-12 07:53:46.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/next.svg
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     6418 2024-04-12 07:53:46.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/status.html
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)    87366 2024-04-12 07:53:46.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/verba.png
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      629 2024-04-12 07:53:46.000000 goldenverba-0.4.0/goldenverba/server/frontend/out/vercel.svg
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     5033 2023-11-13 09:29:47.000000 goldenverba-0.4.0/goldenverba/server/util.py
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)    25358 2024-04-11 12:39:24.000000 goldenverba-0.4.0/goldenverba/verba_manager.py
+drwxr-xr-x   0 edwardschmuhl   (501) staff       (20)        0 2024-04-12 08:31:49.701734 goldenverba-0.4.0/goldenverba.egg-info/
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)    22982 2024-04-12 08:31:49.000000 goldenverba-0.4.0/goldenverba.egg-info/PKG-INFO
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)    18338 2024-04-12 08:31:49.000000 goldenverba-0.4.0/goldenverba.egg-info/SOURCES.txt
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)        1 2024-04-12 08:31:49.000000 goldenverba-0.4.0/goldenverba.egg-info/dependency_links.txt
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       53 2024-04-12 08:31:49.000000 goldenverba-0.4.0/goldenverba.egg-info/entry_points.txt
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)      309 2024-04-12 08:31:49.000000 goldenverba-0.4.0/goldenverba.egg-info/requires.txt
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       12 2024-04-12 08:31:49.000000 goldenverba-0.4.0/goldenverba.egg-info/top_level.txt
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)       38 2024-04-12 08:31:49.702858 goldenverba-0.4.0/setup.cfg
+-rw-r--r--   0 edwardschmuhl   (501) staff       (20)     1767 2024-04-11 12:35:17.000000 goldenverba-0.4.0/setup.py
```

### Comparing `goldenverba-0.3.1/LICENSE` & `goldenverba-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/PKG-INFO` & `goldenverba-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 Metadata-Version: 2.1
 Name: goldenverba
-Version: 0.3.1
+Version: 0.4.0
 Summary: Welcome to Verba: The Golden RAGtriever, an open-source initiative designed to offer a streamlined, user-friendly interface for Retrieval-Augmented Generation (RAG) applications. In just a few easy steps, dive into your data and make meaningful interactions!
 Home-page: https://github.com/weaviate/Verba
 Author: Weaviate
 Author-email: edward@weaviate.io
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: weaviate-client==3.23.1
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: openai==0.27.9
 Requires-Dist: wasabi==1.1.2
-Requires-Dist: spacy==3.6.1
 Requires-Dist: fastapi==0.102.0
 Requires-Dist: uvicorn[standard]
 Requires-Dist: click==8.1.7
 Requires-Dist: asyncio
 Requires-Dist: tiktoken==0.5.1
 Requires-Dist: cohere==4.33
 Requires-Dist: requests
 Requires-Dist: pypdf2
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: black>=23.7.0; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
 Provides-Extra: huggingface
 Requires-Dist: sentence-transformers; extra == "huggingface"
 Requires-Dist: transformers; extra == "huggingface"
 Requires-Dist: torch; extra == "huggingface"
 Requires-Dist: huggingface_hub; extra == "huggingface"
 Requires-Dist: accelerate; extra == "huggingface"
 
@@ -52,65 +49,65 @@
 
 [![Weaviate](https://img.shields.io/static/v1?label=powered%20by&message=Weaviate%20%E2%9D%A4&color=green&style=flat-square)](https://weaviate.io/) 
 [![PyPi downloads](https://static.pepy.tech/personalized-badge/goldenverba?period=total&units=international_system&left_color=grey&right_color=orange&left_text=pip%20downloads)](https://pypi.org/project/goldenverba/) [![Docker support](https://img.shields.io/badge/Docker_support-%E2%9C%93-4c1?style=flat-square&logo=docker&logoColor=white)](https://docs.docker.com/get-started/) [![Demo](https://img.shields.io/badge/Check%20out%20the%20demo!-yellow?&style=flat-square&logo=react&logoColor=white)](https://verba.weaviate.io/)
 
 ![Demo of Verba](https://github.com/weaviate/Verba/blob/dev/img/verba.gif)
 
 - [Verba](#verba)
-  - [🎯 What Is Verba?](#🎯-what-is-verba)
-  - [⚙️ Under the Hood](#️⚙️-under-the-hood)
-  - [💡 Effortless Data Import with Weaviate](#💡-effortless-data-import-with-weaviate)
-  - [💥 Advanced Query Resolution with Hybrid Search](#💥-advanced-query-resolution-with-hybrid-search)
-  - [🔥 Accelerate Queries with Semantic Cache](#🔥-accelerate-queries-with-semantic-cache)
-- [✨ Getting Started with Verba](#✨-getting-started-with-verba)
-- [🐍 Installing Python and Setting Up a Virtual Environment](#🐍-installing-python-and-setting-up-a-virtual-environment)
+  - [🎯 What Is Verba?](#what-is-verba)
+  - [⚙️ Under the Hood](#️under-the-hood)
+  - [💡 Effortless Data Import with Weaviate](#effortless-data-import-with-weaviate)
+  - [💥 Advanced Query Resolution with Hybrid Search](#advanced-query-resolution-with-hybrid-search)
+  - [🔥 Accelerate Queries with Semantic Cache](#accelerate-queries-with-semantic-cache)
+- [✨ Getting Started with Verba](#getting-started-with-verba)
+- [🐍 Installing Python and Setting Up a Virtual Environment](#installing-python-and-setting-up-a-virtual-environment)
   - [Installing Python](#installing-python)
   - [Setting Up a Virtual Environment](#setting-up-a-virtual-environment)
-- [📦 Choosing the Right Verba Installation Package](#📦-choosing-the-right-verba-installation-package)
+- [📦 Choosing the Right Verba Installation Package](#choosing-the-right-verba-installation-package)
   - [Default Package](#default-package)
   - [HuggingFace Version](#huggingface-version)
   - [Development Version](#development-version)
-- [🚀 Quickstart: Deploy with pip](#🚀-quickstart-deploy-with-pip)
-- [🛠️ Quickstart: Build from Source](#️🛠️-quickstart-build-from-source)
-- [🔑 API Keys](#🔑-api-keys)
+- [🚀 Quickstart: Deploy with pip](#quickstart-deploy-with-pip)
+- [🛠️ Quickstart: Build from Source](#️quickstart-build-from-source)
+- [🔑 API Keys](#api-keys)
   - [Weaviate](#weaviate)
   - [OpenAI](#openai)
   - [Cohere](#cohere)
   - [HuggingFace](#huggingface)
     - [Llama2](#llama2)
   - [Unstructured](#unstructured)
   - [Github](#github)
-- [🐳 Quickstart: Deploy with Docker](#🐳-quickstart-deploy-with-docker)
-  - [Large Language Model (LLM) Costs](#-large-language-model-llm-costs)
-- [💾 Importing Your Data into Verba](#️💾-Importing-Your-Data-into-Verba)
-- [🛠️ Project Architecture](#️🛠️-project-architecture)
-- [💖 Open Source Contribution](#💖-open-source-contribution)
+- [🐳 Quickstart: Deploy with Docker](#quickstart-deploy-with-docker)
+  - [Large Language Model (LLM) Costs](#large-language-model-llm-costs)
+- [💾 Importing Your Data into Verba](#️importing-your-data-into-verba)
+- [🛠️ Project Architecture](#️project-architecture)
+- [💖 Open Source Contribution](#open-source-contribution)
 
-## 🎯 What Is Verba?
+## What Is Verba?
 Verba is more than just a tool—it's a personal assistant for querying and interacting with your data, **either locally or deployed via cloud**. Have questions about your documents? Need to cross-reference multiple data points? Want to gain insights from your existing knowledge base? Verba empowers you with the combined capabilities of Weaviate's context-aware database and the analytical power of Large Language Models (LLMs). Interact with your data through an intuitive chat interface that refines search results by using the ongoing conversation context to deliver even more accurate and relevant information.
 
 ![Demo of Verba](https://github.com/weaviate/Verba/blob/dev/img/verba_screen.png)
 
-### ⚙️ Under the Hood
+### Under the Hood
 Verba is engineered with Weaviate's cutting-edge Generative Search technology at its core, extracting relevant context from your pool of documents to resolve queries with precision. By utilizing the power of Large Language Models, Verba doesn't just search for answers—it understands and provides responses that are contextually rich and informed by the content of your documents, all through an intuitive user interface designed for simplicity and efficiency.
 
-### 💡 Effortless Data Import with Weaviate
+### Effortless Data Import with Weaviate
 Verba offers seamless data import functionality through its frontend, supporting a diverse range of file types including `.txt`, `.md`, `.pdf` and more. Before feeding your data into Weaviate, Verba handles chunking and vectorization to optimize it for search and retrieval. Together with collaborative partners we support popular libraries such as [HuggingFace](https://github.com/huggingface), [Haystack](https://github.com/deepset-ai/haystack), [Unstructured](https://github.com/Unstructured-IO/unstructured) and many more!
 
 ![Demo of Verba](https://github.com/weaviate/Verba/blob/dev/img/verba_import.png)
 
-### 💥 Advanced Query Resolution with Hybrid Search
+### Advanced Query Resolution with Hybrid Search
 Experience the hybrid search capabilities of Weaviate within Verba, which merges vector and lexical search methodologies for even greater precision. This dual approach not only navigates through your documents to pinpoint exact matches but also understands the nuance of context, enabling the Large Language Models to craft responses that are both comprehensive and contextually aware. It's an advanced technique that redefines document retrieval, providing you with precisely what you need, when you need it.
 
-### 🔥 Accelerate Queries with Semantic Cache
+### Accelerate Queries with Semantic Cache
 Verba enhances search efficiency with Weaviate's Semantic Cache, a sophisticated system that retains the essence of your queries, results, and dialogues. This proactive feature means that Verba anticipates your needs, using cached data to expedite future inquiries. With semantic matching, it quickly determines if your question has been asked before, delivering instant results, and even suggests auto-completions based on historical interactions, streamlining your search experience to be faster and more intuitive.
 
 ---
 
-# ✨ Getting Started with Verba
+# Getting Started with Verba
 
 Starting your Verba journey is super easy, with multiple deployment options tailored to your preferences. Follow these simple steps to get Verba up and running:
 
 - Deploy with pip [(Quickstart)](##🚀-Quickstart:-Deploy-with-pip)
 ```
 pip install goldenverba
 ```
@@ -118,18 +115,18 @@
 ```
 git clone https://github.com/weaviate/Verba
 
 pip install -e .
 ```
 - Use Docker for Deployment [(Quickstart)](##🐳-Quickstart:-Deploy-with-Docker)
 
-**Prerequisites**: If you're not using Docker, ensure that you have `Python >=3.9.0` installed on your system.
+**Prerequisites**: If you're not using Docker, ensure that you have `Python >=3.10.0` installed on your system.
 
-# 🐍 Installing Python and Setting Up a Virtual Environment
-Before you can use Verba, you'll need to ensure that `Python >=3.9.0` is installed on your system and that you can create a virtual environment for a safer and cleaner project setup.
+# Installing Python and Setting Up a Virtual Environment
+Before you can use Verba, you'll need to ensure that `Python >=3.10.0` is installed on your system and that you can create a virtual environment for a safer and cleaner project setup.
 
 ## Installing Python
 Python is required to run Verba. If you don't have Python installed, follow these steps:
 
 ### For Windows:
 Download the latest Python installer from the official Python website.
 Run the installer and make sure to check the box that says `Add Python to PATH` during installation.
@@ -176,29 +173,15 @@
 source venv/bin/activate
 ```
 
 Once your virtual environment is activated, you'll see its name in the terminal prompt. Now you're ready to install Verba using the steps provided in the Quickstart sections.
 
 > Remember to deactivate the virtual environment when you're done working with Verba by simply running deactivate in the terminal.
 
-## Linting
-We use [ruff](https://github.com/astral-sh/ruff) for automatic code formation and linting.
-The process is automated with a pre-commit hook. To install the hook, run:
-```
-pre-commit install
-```
-or for shorthand:
-```bash 
-make pre-commit
-```
-After that all your commits will be automatically linted and formatted. The linting will happen only on the files you changed.
-
-`make pre-commit` formats all files in the repository and install the hooks if needed.
-
-# 📦 Choosing the Right Verba Installation Package
+# Choosing the Right Verba Installation Package
 Verba comes in several installation packages, each tailored for specific use cases and environments. Choose the package that aligns with your requirements:
 
 ## Default Package
 The default package is perfect for getting started quickly and includes support for popular models and services like OpenAI, Cohere, and spaCy. This package is suitable for general use and can be installed easily via pip:
 
 ```
 pip install goldenverba
@@ -220,15 +203,15 @@
 
 ```
 pip install goldenverba[dev]
 ```
 
 > Keep in mind that this version is intended for development purposes and may contain experimental features.
 
-# 🚀 Quickstart: Deploy with pip
+# Quickstart: Deploy with pip
 
 1. **Initialize a new Python Environment**
 ```
 python3 -m virtualenv venv
 ```
 
 2. **Install Verba**
@@ -244,15 +227,15 @@
 4. **Access Verba**
 ```
 Visit localhost:8000
 ```
 
 5. **Create .env file and add environment variables**
 
-# 🛠️ Quickstart: Build from Source
+# Quickstart: Build from Source
 
 1. **Clone the Verba repos**
 ```
 git clone https://github.com/weaviate/Verba.git
 ```
 
 2. **Initialize a new Python Environment**
@@ -273,17 +256,20 @@
 5. **Access Verba**
 ```
 Visit localhost:8000
 ```
 
 6. **Create .env file and add environment variables**
 
-# 🔑 API Keys
+# API Keys
+
+Before diving into Verba's capabilities, you'll need to configure access to various components depending on your chosen technologies, such as OpenAI, Cohere, and HuggingFace. Start by obtaining the necessary API keys and setting them up through a `.env` file based on our provided [example](./goldenverba/.env.example) , or by declaring them as environment variables on your system. If you're building from source or using Docker, make sure your `.env` file is within the goldenverba directory.
+Please make sure to only include environment variables you really need.
 
-Before diving into Verba's capabilities, you'll need to configure access to various components depending on your chosen technologies, such as OpenAI, Cohere, and HuggingFace. Start by obtaining the necessary API keys and setting them up through a `.env` file based on our provided [example](./.env.example) , or by declaring them as environment variables on your system. Below is a comprehensive list of the API keys and variables you may require:
+Below is a comprehensive list of the API keys and variables you may require:
 
 ## Weaviate
 Verba provides flexibility in connecting to Weaviate instances based on your needs. By default, Verba opts for [Weaviate Embedded](https://weaviate.io/developers/weaviate/installation/embedded) if it doesn't detect the `WEAVIATE_URL_VERBA` and `WEAVIATE_API_KEY_VERBA` environment variables. This local deployment is the most straightforward way to launch your Weaviate database for prototyping and testing.
 
 However, you have other compelling options to consider:
 
 **🌩️ Weaviate Cloud Service (WCS)**
@@ -303,14 +289,54 @@
 
 Verba supports OpenAI Models such as Ada, GPT3, and GPT4. To use them, you need to specify the `OPENAI_API_KEY` environment variable. You can get it from [OpenAI](https://openai.com/)
 
 ```
 OPENAI_API_KEY=YOUR-OPENAI-KEY
 ```
 
+You can also add a `OPENAI_BASE_URL` to use proxies such as LiteLLM (https://github.com/BerriAI/litellm)
+
+```
+OPENAI_BASE_URL=YOUR-OPENAI_BASE_URL
+```
+
+## Azure OpenAI
+
+To use Azure OpenAI, you need to set 
+
+- The API type:
+```
+OPENAI_API_TYPE="azure"
+```
+
+- The key and the endpoint:
+
+```
+OPENAI_API_KEY=<YOUR_KEY>
+OPENAI_BASE_URL=http://XXX.openai.azure.com
+```
+
+- Azure OpenAI ressource name, which is XXX if your endpoint is XXX.openai.azure.com
+
+```
+AZURE_OPENAI_RESOURCE_NAME=<YOUR_AZURE_RESOURCE_NAME>
+```
+- You need to set the models, for the embeddings and for the query.
+```
+AZURE_OPENAI_EMBEDDING_MODEL="text-embedding-ada-002"
+OPENAI_MODEL="gpt-4" 
+```
+
+- Finally, as Azure is using per-minute quota, you might need to add a waiting time between each chunk upload. For example, if you have a limit of 240k tokens per minute, if your chunks are 
+400 tokens max, then 100ms between queries should be fine. If you get error 429 from weaviate, then increase this value.
+
+```
+WAIT_TIME_BETWEEN_INGESTION_QUERIES_MS="100"
+```
+
 ## Cohere
 
 Verba supports Cohere Models, to use them, you need to specify the `COHERE_API_KEY` environment variable. You can get it from [Cohere](https://dashboard.cohere.com/)
 
 ```
 COHERE_API_KEY=YOUR-COHERE-KEY
 ```
@@ -351,15 +377,15 @@
 
 ## Status Page
 
 Once configured, you can monitor your Verba installation's health and status via the 'Status Verba' page. This dashboard provides insights into your deployment type, libraries, environment settings, Weaviate schema counts, and more. It's also your go-to for maintenance tasks like resetting Verba, clearing the cache, or managing auto-complete suggestions.
 
 ![Demo of Verba](https://github.com/weaviate/Verba/blob/dev/img/verba_status.png)
 
-# 🐳 Quickstart: Deploy with Docker
+# Quickstart: Deploy with Docker
 
 Docker is a set of platform-as-a-service products that use OS-level virtualization to deliver software in packages called containers. Containers are isolated from one another and bundle their own software, libraries, and configuration files; they can communicate with each other through well-defined channels. All containers are run by a single operating system kernel and are thus more lightweight than virtual machines. Docker provides an additional layer of abstraction and automation of operating-system-level virtualization on Windows and Linux.
 
 Docker's use of containers to package software means that the application and its dependencies, libraries, and other binaries are packaged together and can be moved between environments easily. This makes it incredibly useful for developers looking to create predictable environments that are isolated from other applications. 
 
 To get started with deploying Verba using Docker, follow the steps below. If you need more detailed instructions on Docker usage, check out the [Docker Curriculum](https://docker-curriculum.com/).
 
@@ -368,25 +394,47 @@
 0. **Clone the Verba repos**
 Ensure you have Git installed on your system. Then, open a terminal or command prompt and run the following command to clone the Verba repository:
 
 ```
 git clone https://github.com/weaviate/Verba.git
 ```
 
-1. **Deploy using Docker**
+1. **Set neccessary environment variables**
+Make sure to set your required environment variables in the ```.env``` file. You can read more about how to set them up in the [API Keys Section](#api-keys)
+
+2. **Adjust the docker-compose file**
+You can use the ```docker-compose.yml``` to add required environment variables under the ```verba``` service and can also adjust the Weaviate Docker settings to enable Authentification or change other settings of your database instance. You can read more about the Weaviate configuration in our [docker-compose documentation](https://weaviate.io/developers/weaviate/installation/docker-compose)
+
+> Please make sure to only add environment variables that you really need. If have no authentifcation enabled in your Weaviate Cluster, make sure to not include the ```WEAVIATE_API_KEY_VERBA``` enviroment variable
+
+2. **Deploy using Docker**
 With Docker installed and the Verba repository cloned, navigate to the directory containing the Docker Compose file in your terminal or command prompt. Run the following command to start the Verba application in detached mode, which allows it to run in the background:
 
 ```
 docker compose up -d
 ```
 
 This command will download the necessary Docker images, create containers, and start Verba.
 Remember, Docker must be installed on your system to use this method. For installation instructions and more details about Docker, visit the official Docker documentation. 
 
-## 💾 Importing Your Data into Verba
+4. **Access Verba**
+
+- You can access your local Weaviate instance at ```localhost:8080```
+
+- You can access the Verba frontend at ```localhost:8000```
+
+
+If you want your Docker Instance to install a specific version of Verba (as described in the [package section](#choosing-the-right-verba-installation-package)) you can edit the ```Dockerfile``` and change the installation line.
+
+```
+RUN pip install -e '.'
+```
+
+
+## Importing Your Data into Verba
 
 With Verba configured, you're ready to import your data and start exploring. Follow these simple steps to get your data into Verba:
 
 ![Demo of Verba](https://github.com/weaviate/Verba/blob/dev/img/verba_data.gif)
 
 1. **Initiate the Import Process**
    - Click on "Add Documents" to begin.
@@ -412,18 +460,18 @@
      - `CohereEmbedder`: Uses Cohere for embedding.
 
 6. **Commence Data Ingestion**
    - After setting up your preferences, click on "Import" to ingest your data into Verba.
 
 Now your data is ready to be used within Verba, enabling you to leverage its powerful search and retrieval capabilities.
 
-## 💰 Large Language Model (LLM) Costs
+## Large Language Model (LLM) Costs
 
 Verba utilizes LLM models through APIs. Be advised that the usage costs for these models will be billed to the API access key you provide. Primarily, costs are incurred during data embedding and answer generation processes.
 
-## 💖 Open Source Contribution
+## Open Source Contribution
 
 Your contributions are always welcome! Feel free to contribute ideas, feedback, or create issues and bug reports if you find any! Before contributing, please read the [Contribution Guide](./CONTRIBUTING.md). Visit our [Weaviate Community Forum](https://forum.weaviate.io/) if you need any help!
 
-### 🛠️ Project Architecture
+### Project Architecture
 You can learn more about Verba's architecture and implementation in its [technical documentation](./TECHNICAL.md) and [frontend documentation](./FRONTEND.md). It's recommended to read them before making any contributions.
```

### Comparing `goldenverba-0.3.1/README.md` & `goldenverba-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,65 +9,65 @@
 
 [![Weaviate](https://img.shields.io/static/v1?label=powered%20by&message=Weaviate%20%E2%9D%A4&color=green&style=flat-square)](https://weaviate.io/) 
 [![PyPi downloads](https://static.pepy.tech/personalized-badge/goldenverba?period=total&units=international_system&left_color=grey&right_color=orange&left_text=pip%20downloads)](https://pypi.org/project/goldenverba/) [![Docker support](https://img.shields.io/badge/Docker_support-%E2%9C%93-4c1?style=flat-square&logo=docker&logoColor=white)](https://docs.docker.com/get-started/) [![Demo](https://img.shields.io/badge/Check%20out%20the%20demo!-yellow?&style=flat-square&logo=react&logoColor=white)](https://verba.weaviate.io/)
 
 ![Demo of Verba](https://github.com/weaviate/Verba/blob/dev/img/verba.gif)
 
 - [Verba](#verba)
-  - [🎯 What Is Verba?](#🎯-what-is-verba)
-  - [⚙️ Under the Hood](#️⚙️-under-the-hood)
-  - [💡 Effortless Data Import with Weaviate](#💡-effortless-data-import-with-weaviate)
-  - [💥 Advanced Query Resolution with Hybrid Search](#💥-advanced-query-resolution-with-hybrid-search)
-  - [🔥 Accelerate Queries with Semantic Cache](#🔥-accelerate-queries-with-semantic-cache)
-- [✨ Getting Started with Verba](#✨-getting-started-with-verba)
-- [🐍 Installing Python and Setting Up a Virtual Environment](#🐍-installing-python-and-setting-up-a-virtual-environment)
+  - [🎯 What Is Verba?](#what-is-verba)
+  - [⚙️ Under the Hood](#️under-the-hood)
+  - [💡 Effortless Data Import with Weaviate](#effortless-data-import-with-weaviate)
+  - [💥 Advanced Query Resolution with Hybrid Search](#advanced-query-resolution-with-hybrid-search)
+  - [🔥 Accelerate Queries with Semantic Cache](#accelerate-queries-with-semantic-cache)
+- [✨ Getting Started with Verba](#getting-started-with-verba)
+- [🐍 Installing Python and Setting Up a Virtual Environment](#installing-python-and-setting-up-a-virtual-environment)
   - [Installing Python](#installing-python)
   - [Setting Up a Virtual Environment](#setting-up-a-virtual-environment)
-- [📦 Choosing the Right Verba Installation Package](#📦-choosing-the-right-verba-installation-package)
+- [📦 Choosing the Right Verba Installation Package](#choosing-the-right-verba-installation-package)
   - [Default Package](#default-package)
   - [HuggingFace Version](#huggingface-version)
   - [Development Version](#development-version)
-- [🚀 Quickstart: Deploy with pip](#🚀-quickstart-deploy-with-pip)
-- [🛠️ Quickstart: Build from Source](#️🛠️-quickstart-build-from-source)
-- [🔑 API Keys](#🔑-api-keys)
+- [🚀 Quickstart: Deploy with pip](#quickstart-deploy-with-pip)
+- [🛠️ Quickstart: Build from Source](#️quickstart-build-from-source)
+- [🔑 API Keys](#api-keys)
   - [Weaviate](#weaviate)
   - [OpenAI](#openai)
   - [Cohere](#cohere)
   - [HuggingFace](#huggingface)
     - [Llama2](#llama2)
   - [Unstructured](#unstructured)
   - [Github](#github)
-- [🐳 Quickstart: Deploy with Docker](#🐳-quickstart-deploy-with-docker)
-  - [Large Language Model (LLM) Costs](#-large-language-model-llm-costs)
-- [💾 Importing Your Data into Verba](#️💾-Importing-Your-Data-into-Verba)
-- [🛠️ Project Architecture](#️🛠️-project-architecture)
-- [💖 Open Source Contribution](#💖-open-source-contribution)
+- [🐳 Quickstart: Deploy with Docker](#quickstart-deploy-with-docker)
+  - [Large Language Model (LLM) Costs](#large-language-model-llm-costs)
+- [💾 Importing Your Data into Verba](#️importing-your-data-into-verba)
+- [🛠️ Project Architecture](#️project-architecture)
+- [💖 Open Source Contribution](#open-source-contribution)
 
-## 🎯 What Is Verba?
+## What Is Verba?
 Verba is more than just a tool—it's a personal assistant for querying and interacting with your data, **either locally or deployed via cloud**. Have questions about your documents? Need to cross-reference multiple data points? Want to gain insights from your existing knowledge base? Verba empowers you with the combined capabilities of Weaviate's context-aware database and the analytical power of Large Language Models (LLMs). Interact with your data through an intuitive chat interface that refines search results by using the ongoing conversation context to deliver even more accurate and relevant information.
 
 ![Demo of Verba](https://github.com/weaviate/Verba/blob/dev/img/verba_screen.png)
 
-### ⚙️ Under the Hood
+### Under the Hood
 Verba is engineered with Weaviate's cutting-edge Generative Search technology at its core, extracting relevant context from your pool of documents to resolve queries with precision. By utilizing the power of Large Language Models, Verba doesn't just search for answers—it understands and provides responses that are contextually rich and informed by the content of your documents, all through an intuitive user interface designed for simplicity and efficiency.
 
-### 💡 Effortless Data Import with Weaviate
+### Effortless Data Import with Weaviate
 Verba offers seamless data import functionality through its frontend, supporting a diverse range of file types including `.txt`, `.md`, `.pdf` and more. Before feeding your data into Weaviate, Verba handles chunking and vectorization to optimize it for search and retrieval. Together with collaborative partners we support popular libraries such as [HuggingFace](https://github.com/huggingface), [Haystack](https://github.com/deepset-ai/haystack), [Unstructured](https://github.com/Unstructured-IO/unstructured) and many more!
 
 ![Demo of Verba](https://github.com/weaviate/Verba/blob/dev/img/verba_import.png)
 
-### 💥 Advanced Query Resolution with Hybrid Search
+### Advanced Query Resolution with Hybrid Search
 Experience the hybrid search capabilities of Weaviate within Verba, which merges vector and lexical search methodologies for even greater precision. This dual approach not only navigates through your documents to pinpoint exact matches but also understands the nuance of context, enabling the Large Language Models to craft responses that are both comprehensive and contextually aware. It's an advanced technique that redefines document retrieval, providing you with precisely what you need, when you need it.
 
-### 🔥 Accelerate Queries with Semantic Cache
+### Accelerate Queries with Semantic Cache
 Verba enhances search efficiency with Weaviate's Semantic Cache, a sophisticated system that retains the essence of your queries, results, and dialogues. This proactive feature means that Verba anticipates your needs, using cached data to expedite future inquiries. With semantic matching, it quickly determines if your question has been asked before, delivering instant results, and even suggests auto-completions based on historical interactions, streamlining your search experience to be faster and more intuitive.
 
 ---
 
-# ✨ Getting Started with Verba
+# Getting Started with Verba
 
 Starting your Verba journey is super easy, with multiple deployment options tailored to your preferences. Follow these simple steps to get Verba up and running:
 
 - Deploy with pip [(Quickstart)](##🚀-Quickstart:-Deploy-with-pip)
 ```
 pip install goldenverba
 ```
@@ -75,18 +75,18 @@
 ```
 git clone https://github.com/weaviate/Verba
 
 pip install -e .
 ```
 - Use Docker for Deployment [(Quickstart)](##🐳-Quickstart:-Deploy-with-Docker)
 
-**Prerequisites**: If you're not using Docker, ensure that you have `Python >=3.9.0` installed on your system.
+**Prerequisites**: If you're not using Docker, ensure that you have `Python >=3.10.0` installed on your system.
 
-# 🐍 Installing Python and Setting Up a Virtual Environment
-Before you can use Verba, you'll need to ensure that `Python >=3.9.0` is installed on your system and that you can create a virtual environment for a safer and cleaner project setup.
+# Installing Python and Setting Up a Virtual Environment
+Before you can use Verba, you'll need to ensure that `Python >=3.10.0` is installed on your system and that you can create a virtual environment for a safer and cleaner project setup.
 
 ## Installing Python
 Python is required to run Verba. If you don't have Python installed, follow these steps:
 
 ### For Windows:
 Download the latest Python installer from the official Python website.
 Run the installer and make sure to check the box that says `Add Python to PATH` during installation.
@@ -133,29 +133,15 @@
 source venv/bin/activate
 ```
 
 Once your virtual environment is activated, you'll see its name in the terminal prompt. Now you're ready to install Verba using the steps provided in the Quickstart sections.
 
 > Remember to deactivate the virtual environment when you're done working with Verba by simply running deactivate in the terminal.
 
-## Linting
-We use [ruff](https://github.com/astral-sh/ruff) for automatic code formation and linting.
-The process is automated with a pre-commit hook. To install the hook, run:
-```
-pre-commit install
-```
-or for shorthand:
-```bash 
-make pre-commit
-```
-After that all your commits will be automatically linted and formatted. The linting will happen only on the files you changed.
-
-`make pre-commit` formats all files in the repository and install the hooks if needed.
-
-# 📦 Choosing the Right Verba Installation Package
+# Choosing the Right Verba Installation Package
 Verba comes in several installation packages, each tailored for specific use cases and environments. Choose the package that aligns with your requirements:
 
 ## Default Package
 The default package is perfect for getting started quickly and includes support for popular models and services like OpenAI, Cohere, and spaCy. This package is suitable for general use and can be installed easily via pip:
 
 ```
 pip install goldenverba
@@ -177,15 +163,15 @@
 
 ```
 pip install goldenverba[dev]
 ```
 
 > Keep in mind that this version is intended for development purposes and may contain experimental features.
 
-# 🚀 Quickstart: Deploy with pip
+# Quickstart: Deploy with pip
 
 1. **Initialize a new Python Environment**
 ```
 python3 -m virtualenv venv
 ```
 
 2. **Install Verba**
@@ -201,15 +187,15 @@
 4. **Access Verba**
 ```
 Visit localhost:8000
 ```
 
 5. **Create .env file and add environment variables**
 
-# 🛠️ Quickstart: Build from Source
+# Quickstart: Build from Source
 
 1. **Clone the Verba repos**
 ```
 git clone https://github.com/weaviate/Verba.git
 ```
 
 2. **Initialize a new Python Environment**
@@ -230,17 +216,20 @@
 5. **Access Verba**
 ```
 Visit localhost:8000
 ```
 
 6. **Create .env file and add environment variables**
 
-# 🔑 API Keys
+# API Keys
+
+Before diving into Verba's capabilities, you'll need to configure access to various components depending on your chosen technologies, such as OpenAI, Cohere, and HuggingFace. Start by obtaining the necessary API keys and setting them up through a `.env` file based on our provided [example](./goldenverba/.env.example) , or by declaring them as environment variables on your system. If you're building from source or using Docker, make sure your `.env` file is within the goldenverba directory.
+Please make sure to only include environment variables you really need.
 
-Before diving into Verba's capabilities, you'll need to configure access to various components depending on your chosen technologies, such as OpenAI, Cohere, and HuggingFace. Start by obtaining the necessary API keys and setting them up through a `.env` file based on our provided [example](./.env.example) , or by declaring them as environment variables on your system. Below is a comprehensive list of the API keys and variables you may require:
+Below is a comprehensive list of the API keys and variables you may require:
 
 ## Weaviate
 Verba provides flexibility in connecting to Weaviate instances based on your needs. By default, Verba opts for [Weaviate Embedded](https://weaviate.io/developers/weaviate/installation/embedded) if it doesn't detect the `WEAVIATE_URL_VERBA` and `WEAVIATE_API_KEY_VERBA` environment variables. This local deployment is the most straightforward way to launch your Weaviate database for prototyping and testing.
 
 However, you have other compelling options to consider:
 
 **🌩️ Weaviate Cloud Service (WCS)**
@@ -260,14 +249,54 @@
 
 Verba supports OpenAI Models such as Ada, GPT3, and GPT4. To use them, you need to specify the `OPENAI_API_KEY` environment variable. You can get it from [OpenAI](https://openai.com/)
 
 ```
 OPENAI_API_KEY=YOUR-OPENAI-KEY
 ```
 
+You can also add a `OPENAI_BASE_URL` to use proxies such as LiteLLM (https://github.com/BerriAI/litellm)
+
+```
+OPENAI_BASE_URL=YOUR-OPENAI_BASE_URL
+```
+
+## Azure OpenAI
+
+To use Azure OpenAI, you need to set 
+
+- The API type:
+```
+OPENAI_API_TYPE="azure"
+```
+
+- The key and the endpoint:
+
+```
+OPENAI_API_KEY=<YOUR_KEY>
+OPENAI_BASE_URL=http://XXX.openai.azure.com
+```
+
+- Azure OpenAI ressource name, which is XXX if your endpoint is XXX.openai.azure.com
+
+```
+AZURE_OPENAI_RESOURCE_NAME=<YOUR_AZURE_RESOURCE_NAME>
+```
+- You need to set the models, for the embeddings and for the query.
+```
+AZURE_OPENAI_EMBEDDING_MODEL="text-embedding-ada-002"
+OPENAI_MODEL="gpt-4" 
+```
+
+- Finally, as Azure is using per-minute quota, you might need to add a waiting time between each chunk upload. For example, if you have a limit of 240k tokens per minute, if your chunks are 
+400 tokens max, then 100ms between queries should be fine. If you get error 429 from weaviate, then increase this value.
+
+```
+WAIT_TIME_BETWEEN_INGESTION_QUERIES_MS="100"
+```
+
 ## Cohere
 
 Verba supports Cohere Models, to use them, you need to specify the `COHERE_API_KEY` environment variable. You can get it from [Cohere](https://dashboard.cohere.com/)
 
 ```
 COHERE_API_KEY=YOUR-COHERE-KEY
 ```
@@ -308,15 +337,15 @@
 
 ## Status Page
 
 Once configured, you can monitor your Verba installation's health and status via the 'Status Verba' page. This dashboard provides insights into your deployment type, libraries, environment settings, Weaviate schema counts, and more. It's also your go-to for maintenance tasks like resetting Verba, clearing the cache, or managing auto-complete suggestions.
 
 ![Demo of Verba](https://github.com/weaviate/Verba/blob/dev/img/verba_status.png)
 
-# 🐳 Quickstart: Deploy with Docker
+# Quickstart: Deploy with Docker
 
 Docker is a set of platform-as-a-service products that use OS-level virtualization to deliver software in packages called containers. Containers are isolated from one another and bundle their own software, libraries, and configuration files; they can communicate with each other through well-defined channels. All containers are run by a single operating system kernel and are thus more lightweight than virtual machines. Docker provides an additional layer of abstraction and automation of operating-system-level virtualization on Windows and Linux.
 
 Docker's use of containers to package software means that the application and its dependencies, libraries, and other binaries are packaged together and can be moved between environments easily. This makes it incredibly useful for developers looking to create predictable environments that are isolated from other applications. 
 
 To get started with deploying Verba using Docker, follow the steps below. If you need more detailed instructions on Docker usage, check out the [Docker Curriculum](https://docker-curriculum.com/).
 
@@ -325,25 +354,47 @@
 0. **Clone the Verba repos**
 Ensure you have Git installed on your system. Then, open a terminal or command prompt and run the following command to clone the Verba repository:
 
 ```
 git clone https://github.com/weaviate/Verba.git
 ```
 
-1. **Deploy using Docker**
+1. **Set neccessary environment variables**
+Make sure to set your required environment variables in the ```.env``` file. You can read more about how to set them up in the [API Keys Section](#api-keys)
+
+2. **Adjust the docker-compose file**
+You can use the ```docker-compose.yml``` to add required environment variables under the ```verba``` service and can also adjust the Weaviate Docker settings to enable Authentification or change other settings of your database instance. You can read more about the Weaviate configuration in our [docker-compose documentation](https://weaviate.io/developers/weaviate/installation/docker-compose)
+
+> Please make sure to only add environment variables that you really need. If have no authentifcation enabled in your Weaviate Cluster, make sure to not include the ```WEAVIATE_API_KEY_VERBA``` enviroment variable
+
+2. **Deploy using Docker**
 With Docker installed and the Verba repository cloned, navigate to the directory containing the Docker Compose file in your terminal or command prompt. Run the following command to start the Verba application in detached mode, which allows it to run in the background:
 
 ```
 docker compose up -d
 ```
 
 This command will download the necessary Docker images, create containers, and start Verba.
 Remember, Docker must be installed on your system to use this method. For installation instructions and more details about Docker, visit the official Docker documentation. 
 
-## 💾 Importing Your Data into Verba
+4. **Access Verba**
+
+- You can access your local Weaviate instance at ```localhost:8080```
+
+- You can access the Verba frontend at ```localhost:8000```
+
+
+If you want your Docker Instance to install a specific version of Verba (as described in the [package section](#choosing-the-right-verba-installation-package)) you can edit the ```Dockerfile``` and change the installation line.
+
+```
+RUN pip install -e '.'
+```
+
+
+## Importing Your Data into Verba
 
 With Verba configured, you're ready to import your data and start exploring. Follow these simple steps to get your data into Verba:
 
 ![Demo of Verba](https://github.com/weaviate/Verba/blob/dev/img/verba_data.gif)
 
 1. **Initiate the Import Process**
    - Click on "Add Documents" to begin.
@@ -369,18 +420,18 @@
      - `CohereEmbedder`: Uses Cohere for embedding.
 
 6. **Commence Data Ingestion**
    - After setting up your preferences, click on "Import" to ingest your data into Verba.
 
 Now your data is ready to be used within Verba, enabling you to leverage its powerful search and retrieval capabilities.
 
-## 💰 Large Language Model (LLM) Costs
+## Large Language Model (LLM) Costs
 
 Verba utilizes LLM models through APIs. Be advised that the usage costs for these models will be billed to the API access key you provide. Primarily, costs are incurred during data embedding and answer generation processes.
 
-## 💖 Open Source Contribution
+## Open Source Contribution
 
 Your contributions are always welcome! Feel free to contribute ideas, feedback, or create issues and bug reports if you find any! Before contributing, please read the [Contribution Guide](./CONTRIBUTING.md). Visit our [Weaviate Community Forum](https://forum.weaviate.io/) if you need any help!
 
-### 🛠️ Project Architecture
+### Project Architecture
 You can learn more about Verba's architecture and implementation in its [technical documentation](./TECHNICAL.md) and [frontend documentation](./FRONTEND.md). It's recommended to read them before making any contributions.
```

### Comparing `goldenverba-0.3.1/goldenverba/components/chunking/chunk.py` & `goldenverba-0.4.0/goldenverba/components/chunking/chunk.py`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/components/chunking/interface.py` & `goldenverba-0.4.0/goldenverba/components/chunking/interface.py`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/components/chunking/manager.py` & `goldenverba-0.4.0/goldenverba/components/chunking/manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 import tiktoken
 from wasabi import msg
 
 from goldenverba.components.chunking.interface import Chunker
-from goldenverba.components.chunking.sentencechunker import SentenceChunker
 from goldenverba.components.chunking.tiktokenchunker import TokenChunker
-from goldenverba.components.chunking.wordchunker import WordChunker
 from goldenverba.components.reader.document import Document
 
 
 class ChunkerManager:
     def __init__(self):
         self.chunker: dict[str, Chunker] = {
             "TokenChunker": TokenChunker(),
-            "WordChunker": WordChunker(),
-            "SentenceChunker": SentenceChunker(),
         }
         self.selected_chunker: Chunker = self.chunker["TokenChunker"]
 
     def chunk(
         self, documents: list[Document], units: int, overlap: int
     ) -> list[Document]:
         """Chunk verba documents into chunks based on n and overlap.
```

### Comparing `goldenverba-0.3.1/goldenverba/components/chunking/sentencechunker.py` & `goldenverba-0.4.0/goldenverba/components/chunking/tiktokenchunker.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,33 @@
 import contextlib
 
 from tqdm import tqdm
 from wasabi import msg
 
 with contextlib.suppress(Exception):
-    import spacy
+    import tiktoken
 
 from goldenverba.components.chunking.chunk import Chunk
 from goldenverba.components.chunking.interface import Chunker
 from goldenverba.components.reader.document import Document
-from goldenverba.components.reader.interface import InputForm
 
 
-class SentenceChunker(Chunker):
+class TokenChunker(Chunker):
     """
-    SentenceChunker for Verba built with spaCy.
+    TokenChunker for Verba built with tiktoken.
     """
 
     def __init__(self):
         super().__init__()
-        self.name = "WordChunker"
-        self.requires_library = ["spacy"]
-        self.default_units = 3
-        self.default_overlap = 2
-        self.description = "Chunk documents by sentences. You can specify how many sentences should overlap between chunks to improve retrieval."
-        try:
-            self.nlp = spacy.blank("en")
-            self.nlp.add_pipe("sentencizer")
-        except:
-            self.nlp = None
+        self.name = "TokenChunker"
+        self.requires_library = ["tiktoken"]
+        self.default_units = 250
+        self.default_overlap = 50
+        self.description = "Chunk documents by tokens powered by tiktoken. You can specify how many tokens should overlap between chunks to improve retrieval."
+        self.encoding = tiktoken.encoding_for_model("gpt-3.5-turbo")
 
     def chunk(
         self, documents: list[Document], units: int, overlap: int
     ) -> list[Document]:
         """Chunk verba documents into chunks based on units and overlap
         @parameter: documents : list[Document] - List of Verba documents
         @parameter: units : int - How many units per chunk (words, sentences, etc.)
@@ -42,50 +37,49 @@
         for document in tqdm(
             documents, total=len(documents), desc="Chunking documents"
         ):
             # Skip if document already contains chunks
             if len(document.chunks) > 0:
                 continue
 
-            doc = list(self.nlp(document.text).sents)
+            encoded_tokens = self.encoding.encode(document.text, disallowed_special=())
 
-            if units > len(doc) or units < 1:
-                msg.warn(
-                    f"Unit value either exceeds length of actual document or is below 1 ({units}/{len(doc)})"
+            if units > len(encoded_tokens) or units < 1:
+                doc_chunk = Chunk(
+                    text=document.text,
+                    doc_name=document.name,
+                    doc_type=document.type,
+                    chunk_id=0,
                 )
-                continue
 
             if overlap >= units:
                 msg.warn(
                     f"Overlap value is greater than unit (Units {units}/ Overlap {overlap})"
                 )
                 continue
 
             i = 0
             split_id_counter = 0
-            while i < len(doc):
+            while i < len(encoded_tokens):
                 # Overlap
                 start_i = i
-                end_i = i + units
-                if end_i > len(doc):
-                    end_i = len(doc)  # Adjust for the last chunk
-
-                text = ""
-                for sent in doc[start_i:end_i]:
-                    text += sent.text
+                end_i = min(i + units, len(encoded_tokens))
+
+                chunk_tokens = encoded_tokens[start_i:end_i]
+                chunk_text = self.encoding.decode(chunk_tokens)
 
                 doc_chunk = Chunk(
-                    text=text,
+                    text=chunk_text,
                     doc_name=document.name,
                     doc_type=document.type,
                     chunk_id=split_id_counter,
                 )
                 document.chunks.append(doc_chunk)
                 split_id_counter += 1
 
                 # Exit loop if this was the last possible chunk
-                if end_i == len(doc):
+                if end_i == len(encoded_tokens):
                     break
 
                 i += units - overlap  # Step forward, considering overlap
 
         return documents
```

### Comparing `goldenverba-0.3.1/goldenverba/components/embedding/ADAEmbedder.py` & `goldenverba-0.4.0/goldenverba/components/embedding/ADAEmbedder.py`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/components/embedding/CohereEmbedder.py` & `goldenverba-0.4.0/goldenverba/components/embedding/CohereEmbedder.py`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/components/embedding/MiniLMEmbedder.py` & `goldenverba-0.4.0/goldenverba/components/embedding/MiniLMEmbedder.py`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/components/embedding/interface.py` & `goldenverba-0.4.0/goldenverba/components/embedding/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 import re
+import os
+import time
+from dotenv import load_dotenv
 
 from tqdm import tqdm
 from wasabi import msg
 from weaviate import Client
 
 from goldenverba.components.component import VerbaComponent
 from goldenverba.components.reader.document import Document
 from goldenverba.components.reader.interface import InputForm
 from goldenverba.components.schema.schema_generation import (
     EMBEDDINGS,
     VECTORIZERS,
     strip_non_letters,
 )
 
+load_dotenv()
 
 class Embedder(VerbaComponent):
     """
     Interface for Verba Embedding.
     """
 
     def __init__(self):
@@ -109,14 +113,18 @@
                             # Check if vector already exists
                             if chunk.vector is None:
                                 client.batch.add_data_object(properties, class_name)
                             else:
                                 client.batch.add_data_object(
                                     properties, class_name, vector=chunk.vector
                                 )
+                            
+                            wait_time_ms = int(os.getenv("WAIT_TIME_BETWEEN_INGESTION_QUERIES_MS","0"))
+                            if wait_time_ms>0:
+                                time.sleep(float(wait_time_ms)/1000)
 
                 self.check_document_status(
                     client,
                     uuid,
                     document.name,
                     "Document_" + strip_non_letters(self.vectorizer),
                     "Chunk_" + strip_non_letters(self.vectorizer),
```

### Comparing `goldenverba-0.3.1/goldenverba/components/embedding/manager.py` & `goldenverba-0.4.0/goldenverba/components/embedding/manager.py`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/components/generation/CohereGenerator.py` & `goldenverba-0.4.0/goldenverba/components/generation/CohereGenerator.py`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/components/generation/Llama2Generator.py` & `goldenverba-0.4.0/goldenverba/components/generation/Llama2Generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         self.requires_library = ["huggingface_hub", "transformers"]
         self.requires_env = ["HF_TOKEN", "LLAMA2-7B-CHAT-HF"]
         self.streamable = True
         self.model = None
         self.tokenizer = None
         self.device = None
         self.context_window = 3000
-        if os.environ.get("LLAMA2-7B-CHAT-HF", "") == "True":
+        if os.environ.get("LLAMA2-7B-CHAT-HF", "").lower() == "true":
             try:
                 import torch
                 from transformers import AutoModelForCausalLM, AutoTokenizer
 
                 def get_device():
                     if torch.cuda.is_available():
                         return torch.device("cuda")
```

### Comparing `goldenverba-0.3.1/goldenverba/components/generation/interface.py` & `goldenverba-0.4.0/goldenverba/components/generation/interface.py`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/components/generation/manager.py` & `goldenverba-0.4.0/goldenverba/components/generation/manager.py`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/components/reader/document.py` & `goldenverba-0.4.0/goldenverba/components/reader/document.py`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/components/reader/githubreader.py` & `goldenverba-0.4.0/goldenverba/components/reader/githubreader.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     The GithubReader downloads files from Github and ingests them into Weaviate.
     """
 
     def __init__(self):
         super().__init__()
         self.name = "GithubReader"
         self.requires_env = ["GITHUB_TOKEN"]
-        self.description = "Downloads only text files from a GitHub repository and ingests it into Verba. Use this format {owner}/{repo}/{folder}"
+        self.description = "Downloads only text files from a GitHub repository and ingests it into Verba. Use this format {owner}/{repo}/{branch}/{folder}"
         self.input_form = InputForm.INPUT.value
 
     def load(
         self,
         bytes: list[str] = None,
         contents: list[str] = None,
         paths: list[str] = None,
@@ -89,20 +89,18 @@
         """Fetch filenames from Github
         @parameter path : str - Path to a GitHub repository
         @returns list - List of document names.
         """
         split = path.split("/")
         owner = split[0]
         repo = split[1]
-        folder_path = ""
-        if len(split) > 2:
-            folder_path = "/".join(split[2:])
+        branch = split[2] if len(split) > 2 else "main"
+        folder_path = "/".join(split[3:]) if len(split) > 3 else ""
 
-        # Path should be owner/repo
-        url = f"https://api.github.com/repos/{owner}/{repo}/git/trees/main?recursive=1"
+        url = f"https://api.github.com/repos/{owner}/{repo}/git/trees/{branch}?recursive=1"
         headers = {
             "Authorization": f"token {os.environ.get('GITHUB_TOKEN', '')}",
             "Accept": "application/vnd.github.v3+json",
         }
         response = requests.get(url, headers=headers)
         response.raise_for_status()  # Raise an exception for HTTP errors
 
@@ -127,16 +125,17 @@
         @parameter path : str - Path to a GitHub repository
         @parameter file_path : str - Path of the file in repo
         @returns str - Content of the file.
         """
         split = path.split("/")
         owner = split[0]
         repo = split[1]
+        branch = split[2] if len(split) > 2 else "main"
 
-        url = f"https://api.github.com/repos/{owner}/{repo}/contents/{file_path}"
+        url = f"https://api.github.com/repos/{owner}/{repo}/contents/{file_path}?ref={branch}"
         headers = {
             "Authorization": f"token {os.environ.get('GITHUB_TOKEN', '')}",
             "Accept": "application/vnd.github.v3+json",
         }
         response = requests.get(url, headers=headers)
         response.raise_for_status()
```

### Comparing `goldenverba-0.3.1/goldenverba/components/reader/interface.py` & `goldenverba-0.4.0/goldenverba/components/reader/interface.py`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/components/reader/manager.py` & `goldenverba-0.4.0/goldenverba/components/reader/manager.py`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/components/reader/pdfreader.py` & `goldenverba-0.4.0/goldenverba/components/reader/pdfreader.py`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/components/reader/simplereader.py` & `goldenverba-0.4.0/goldenverba/components/reader/simplereader.py`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/components/reader/unstructuredpdf.py` & `goldenverba-0.4.0/goldenverba/components/reader/unstructuredpdf.py`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/components/retriever/SimpleRetriever.py` & `goldenverba-0.4.0/goldenverba/components/retriever/SimpleRetriever.py`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/components/retriever/WindowRetriever.py` & `goldenverba-0.4.0/goldenverba/components/retriever/WindowRetriever.py`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/components/retriever/interface.py` & `goldenverba-0.4.0/goldenverba/components/retriever/interface.py`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/components/retriever/manager.py` & `goldenverba-0.4.0/goldenverba/components/retriever/manager.py`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/components/schema/schema_generation.py` & `goldenverba-0.4.0/goldenverba/components/schema/schema_generation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import re
-
+import os
+from dotenv import load_dotenv
 from wasabi import msg  # type: ignore[import]
 from weaviate import Client
 
+load_dotenv()
+
 VECTORIZERS = {"text2vec-openai", "text2vec-cohere"}  # Needs to match with Weaviate modules
 EMBEDDINGS = {"MiniLM"}  # Custom Vectors
 
 
 def strip_non_letters(s: str):
     return re.sub(r"[^a-zA-Z0-9]", "_", s)
 
@@ -19,18 +22,34 @@
     @parameter vectorizer : str - Name of the vectorizer
     @parameter skip_properties: list[str] - List of property names that should not get vectorized
     @returns dict - Modified schema if vectorizer is available.
     """
     if skip_properties is None:
         skip_properties = []
     modified_schema = schema.copy()
+
+    #adding specific config for Azure OpenAI
+    vectorizer_config = None
+    if os.getenv("OPENAI_API_TYPE") == "azure" and vectorizer=="text2vec-openai":
+        resourceName = os.getenv("AZURE_OPENAI_RESOURCE_NAME")
+        model = os.getenv("AZURE_OPENAI_EMBEDDING_MODEL")
+        if resourceName is None or model is None:
+            raise Exception("AZURE_OPENAI_RESOURCE_NAME and AZURE_OPENAI_EMBEDDING_MODEL should be set when OPENAI_API_TYPE is azure. Resource name is XXX in http://XXX.openai.azure.com")
+        vectorizer_config = { 
+            "text2vec-openai": {
+                    "deploymentId": model,
+                    "resourceName": resourceName
+            }
+        }
+
     # Verify Vectorizer
     if vectorizer in VECTORIZERS:
         modified_schema["classes"][0]["vectorizer"] = vectorizer
-
+        if vectorizer_config is not None:
+            modified_schema["classes"][0]["moduleConfig"] = vectorizer_config
         for property in modified_schema["classes"][0]["properties"]:
             if property["name"] in skip_properties:
                 moduleConfig = {
                     vectorizer: {
                         "skip": True,
                         "vectorizePropertyName": False,
                     }
```

### Comparing `goldenverba-0.3.1/goldenverba/server/ConfigManager.py` & `goldenverba-0.4.0/goldenverba/server/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/api.py` & `goldenverba-0.4.0/goldenverba/server/api.py`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/cli.py` & `goldenverba-0.4.0/goldenverba/server/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     default=8000,
     help="FastAPI Port",
 )
 def start(port):
     """
     Run the FastAPI application.
     """
-    uvicorn.run("goldenverba.server.api:app", host="127.0.0.1", port=port, reload=True)
+    uvicorn.run("goldenverba.server.api:app", host="0.0.0.0", port=port, reload=True)
 
 
 @cli.command()
 @click.option(
     "--reader",
     default="SimpleReader",
     help="Reader",
```

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/404.html` & `goldenverba-0.4.0/goldenverba/server/frontend/out/404.html`

 * *Files 6% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><link rel="icon" type="image/png" href="static/favicon.png"/><title>404: This page could not be found</title><meta name="next-head-count" content="4"/><link rel="preload" href="/static/_next/static/media/4049f3f580e14086-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/static/_next/static/css/230b09fe1800464e.css" as="style"/><link rel="stylesheet" href="/static/_next/static/css/230b09fe1800464e.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/static/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/static/_next/static/chunks/webpack-67916544a50891e6.js" defer=""></script><script src="/static/_next/static/chunks/framework-7b01e204987c8f43.js" defer=""></script><script src="/static/_next/static/chunks/main-c9732fa3c1d6d1d5.js" defer=""></script><script src="/static/_next/static/chunks/pages/_app-7a548c247b0896b0.js" defer=""></script><script src="/static/_next/static/chunks/pages/_error-b190518070b21757.js" defer=""></script><script src="/static/_next/static/dFAJVlvKY7TnN7l9nf2qs/_buildManifest.js" defer=""></script><script src="/static/_next/static/dFAJVlvKY7TnN7l9nf2qs/_ssgManifest.js" defer=""></script></head><body><div id="__next"><div class="__className_320369"><nav class="fixed bottom-0 left-0 right-0 z-50 bg-gray-100 p-2 shadow-md"><div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8"><div class="flex justify-center items-center py-2"><a class="mx-4 p-3 w-28 text-center rounded-lg text-black text-sm shadow-sm border-2 bg-gray-300 border-gray-400 hover:bg-gray-200 transition-colors duration-300" href="/">Search</a><a class="mx-4 p-3 w-28 text-center rounded-lg text-black text-sm shadow-sm border-2 bg-gray-300 border-gray-400 hover:bg-gray-200 transition-colors duration-300" href="/document_explorer">Documents</a><a class="mx-4 p-3 w-28 text-center rounded-lg text-black text-sm shadow-sm border-2 bg-gray-300 border-gray-400 hover:bg-gray-200 transition-colors duration-300" href="/status">Status</a></div></div></nav><div style="font-family:system-ui,&quot;Segoe UI&quot;,Roboto,Helvetica,Arial,sans-serif,&quot;Apple Color Emoji&quot;,&quot;Segoe UI Emoji&quot;;height:100vh;text-align:center;display:flex;flex-direction:column;align-items:center;justify-content:center"><div style="line-height:48px"><style>body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}</style><h1 class="next-error-h1" style="display:inline-block;margin:0 20px 0 0;padding-right:23px;font-size:24px;font-weight:500;vertical-align:top">404</h1><div style="display:inline-block"><h2 style="font-size:14px;font-weight:400;line-height:28px">This page could not be found<!-- -->.</h2></div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{"statusCode":404}},"page":"/_error","query":{},"buildId":"dFAJVlvKY7TnN7l9nf2qs","assetPrefix":"/static","nextExport":true,"isFallback":false,"gip":true,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><link rel="icon" type="image/png" href="static/favicon.png"/><title>404: This page could not be found</title><meta name="next-head-count" content="4"/><link rel="preload" href="/static/_next/static/media/4049f3f580e14086-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/static/_next/static/css/230b09fe1800464e.css" as="style"/><link rel="stylesheet" href="/static/_next/static/css/230b09fe1800464e.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/static/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/static/_next/static/chunks/webpack-67916544a50891e6.js" defer=""></script><script src="/static/_next/static/chunks/framework-7b01e204987c8f43.js" defer=""></script><script src="/static/_next/static/chunks/main-c9732fa3c1d6d1d5.js" defer=""></script><script src="/static/_next/static/chunks/pages/_app-c1589fca75958036.js" defer=""></script><script src="/static/_next/static/chunks/pages/_error-b190518070b21757.js" defer=""></script><script src="/static/_next/static/_A-piGxRm1B_OMIwQ_tPn/_buildManifest.js" defer=""></script><script src="/static/_next/static/_A-piGxRm1B_OMIwQ_tPn/_ssgManifest.js" defer=""></script></head><body><div id="__next"><div class="__className_320369"><nav class="fixed bottom-0 left-0 right-0 z-50 bg-gray-100 p-2 shadow-md"><div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8"><div class="flex justify-center items-center py-2"><a class="mx-4 p-3 w-28 text-center rounded-lg text-black text-sm shadow-sm border-2 bg-gray-300 border-gray-400 hover:bg-gray-200 transition-colors duration-300" href="/">Search</a><a class="mx-4 p-3 w-28 text-center rounded-lg text-black text-sm shadow-sm border-2 bg-gray-300 border-gray-400 hover:bg-gray-200 transition-colors duration-300" href="/document_explorer">Documents</a><a class="mx-4 p-3 w-28 text-center rounded-lg text-black text-sm shadow-sm border-2 bg-gray-300 border-gray-400 hover:bg-gray-200 transition-colors duration-300" href="/status">Status</a></div></div></nav><div style="font-family:system-ui,&quot;Segoe UI&quot;,Roboto,Helvetica,Arial,sans-serif,&quot;Apple Color Emoji&quot;,&quot;Segoe UI Emoji&quot;;height:100vh;text-align:center;display:flex;flex-direction:column;align-items:center;justify-content:center"><div style="line-height:48px"><style>body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}</style><h1 class="next-error-h1" style="display:inline-block;margin:0 20px 0 0;padding-right:23px;font-size:24px;font-weight:500;vertical-align:top">404</h1><div style="display:inline-block"><h2 style="font-size:14px;font-weight:400;line-height:28px">This page could not be found<!-- -->.</h2></div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{"statusCode":404}},"page":"/_error","query":{},"buildId":"_A-piGxRm1B_OMIwQ_tPn","assetPrefix":"/static","nextExport":true,"isFallback":false,"gip":true,"scriptLoader":[]}</script></body></html>
```

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/0Hcan7GeSF1TuouAgzveb/_buildManifest.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/0Hcan7GeSF1TuouAgzveb/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/5fzR3LERKY5UlE9ayIEWy/_buildManifest.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/5fzR3LERKY5UlE9ayIEWy/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/BrKix8hVmzKkq4nA40XDY/_buildManifest.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/BrKix8hVmzKkq4nA40XDY/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/E3xJxzpNDa7hQ9ErbEuyX/_buildManifest.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/E3xJxzpNDa7hQ9ErbEuyX/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/Ej9O_hZ3RDAnJYJlOxclF/_buildManifest.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/Ej9O_hZ3RDAnJYJlOxclF/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/GGmsoX3roagotCYtIHhEK/_buildManifest.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/GGmsoX3roagotCYtIHhEK/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/NnjBs5HkyOiVgbYuj7tdV/_buildManifest.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/NnjBs5HkyOiVgbYuj7tdV/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/RwEhtmsT64md9fQr26tCz/_buildManifest.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/RwEhtmsT64md9fQr26tCz/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/YWcefBRkmSyHlQU9oZZh2/_buildManifest.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/YWcefBRkmSyHlQU9oZZh2/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/172-06f3679cd389db14.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/172-06f3679cd389db14.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/172-11387f2fea15f8f4.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/172-11387f2fea15f8f4.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/172-2aea64d5cb024338.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/172-2aea64d5cb024338.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/172-50c469fb388350d4.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/172-50c469fb388350d4.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/172-742d06afbbb76b32.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/172-742d06afbbb76b32.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/172-a717b482738a1ff0.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/172-a717b482738a1ff0.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/172-a88687749eea2f07.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/172-a88687749eea2f07.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/172-ac22d29ac37ed486.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/172-ac22d29ac37ed486.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/172-c660cbf18f8cc710.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/172-c660cbf18f8cc710.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/172-f543cedc6ac6c1ac.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/172-f543cedc6ac6c1ac.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/243-f34295e3a57adcf7.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/243-f34295e3a57adcf7.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/246-8cba9c3e138a3cf5.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/246-8cba9c3e138a3cf5.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/280-52c3b45a7bca32e8.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/280-52c3b45a7bca32e8.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/280-74dc7793334d9da5.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/280-74dc7793334d9da5.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/280-a161d7ce2cd7eb6e.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/280-a161d7ce2cd7eb6e.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/280-e826f6179b5d8b6c.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/280-e826f6179b5d8b6c.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/611-ee9176c9cb6e0276.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/611-ee9176c9cb6e0276.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/866-b84c52f36b76def1.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/866-b84c52f36b76def1.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/866-cfe4bf209f60b238.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/866-cfe4bf209f60b238.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/fd9d1056-c06adc43b46a9300.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/fd9d1056-c06adc43b46a9300.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/framework-2a1230696ef28269.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/framework-2a1230696ef28269.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/framework-5d6069c3c7124ee8.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/framework-5d6069c3c7124ee8.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/framework-7b01e204987c8f43.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/framework-7b01e204987c8f43.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/framework-a57e57d99425abb1.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/framework-a57e57d99425abb1.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/framework-cae5c8fdcf4818e7.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/framework-cae5c8fdcf4818e7.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/framework-fe67c9122aecf131.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/framework-fe67c9122aecf131.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/main-2ecc162bcf5a8331.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/main-2ecc162bcf5a8331.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/main-4d54ae8f14f9d7c6.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/main-4d54ae8f14f9d7c6.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/main-8d39882388fd6605.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/main-8d39882388fd6605.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/main-a7f2fdd54fd24f53.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/main-a7f2fdd54fd24f53.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/main-app-a515e76320e72f2c.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/main-app-a515e76320e72f2c.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/main-c9732fa3c1d6d1d5.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/main-c9732fa3c1d6d1d5.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-097dde0f604a216d.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-097dde0f604a216d.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-2e4b2bc90e8e9cf0.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-2e4b2bc90e8e9cf0.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-2f0b49097296ab3b.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-2f0b49097296ab3b.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-44bc0a53432c2305.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-44bc0a53432c2305.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-4ad389329d5c5db0.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-4ad389329d5c5db0.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-4b7391532c7f4bd1.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-4b7391532c7f4bd1.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-4b7688a8f49a037e.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-4b7688a8f49a037e.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-555bac3d60ed6cce.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-555bac3d60ed6cce.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-5914f88957706be3.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-5914f88957706be3.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-5d055a73ecc2e4bb.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-5d055a73ecc2e4bb.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-73b84b7c4b745f50.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-73b84b7c4b745f50.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-7a548c247b0896b0.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-7a548c247b0896b0.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-7b8d7f1c795cadf6.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-7b8d7f1c795cadf6.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-877f2c40f1814452.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-877f2c40f1814452.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-8ae9faf463bff6e8.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-8ae9faf463bff6e8.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-905162599335727d.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-905162599335727d.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-93747ea226addaf4.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-93747ea226addaf4.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-95b570e3c384ee1a.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-95b570e3c384ee1a.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-a0957af8bafb5c75.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-a0957af8bafb5c75.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-a5604af5bf4aeb92.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-a5604af5bf4aeb92.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-b7fba87b2821fa1b.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-b7fba87b2821fa1b.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-d6fe3ed4752599cf.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-d6fe3ed4752599cf.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-f48f66f2530dcab1.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/_app-f48f66f2530dcab1.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/about-5eabeb8efb0f0a5d.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/about-5eabeb8efb0f0a5d.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/about-772e84e976153ce1.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/about-772e84e976153ce1.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-0e4cc95fa680cb1b.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-0e4cc95fa680cb1b.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-16e4de29624eb562.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-16e4de29624eb562.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-3b64a7f4f0744605.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-3b64a7f4f0744605.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-55171382bcb992de.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-55171382bcb992de.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-6dcac899c9312be7.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-6dcac899c9312be7.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-896e2841c08a0cf2.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-896e2841c08a0cf2.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-8dc7615e9ee51133.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-8dc7615e9ee51133.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-a675a1f7ad7744a6.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-a675a1f7ad7744a6.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-abac488ca017417d.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-abac488ca017417d.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-bb1f65e19dfc1c0e.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-bb1f65e19dfc1c0e.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-c8a428b01649242c.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-c8a428b01649242c.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-ccca135591a6180e.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-ccca135591a6180e.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-f2b168e3e47ba8a4.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-f2b168e3e47ba8a4.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-ff456efe0bddd068.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-ff456efe0bddd068.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/status-03d0ba488ee360ad.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/status-03d0ba488ee360ad.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/status-36bfa2eb3ce44652.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/status-36bfa2eb3ce44652.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/status-3e09625e9decd386.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/status-3e09625e9decd386.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/status-5eecffe6be63ff44.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/status-5eecffe6be63ff44.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/status-7d60916a01bd3f1e.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/status-7d60916a01bd3f1e.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/status-ca571a484838e88c.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/status-ca571a484838e88c.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/status-f1bcadfcd1e3bb61.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/status-f1bcadfcd1e3bb61.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/pages/status-fdb704cca997e4eb.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/pages/status-fdb704cca997e4eb.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/webpack-4231116f672e6062.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/webpack-4231116f672e6062.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/webpack-49c0ce1495d0fca6.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/webpack-49c0ce1495d0fca6.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/webpack-4c9086a613e9f796.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/webpack-4c9086a613e9f796.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/webpack-67916544a50891e6.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/webpack-67916544a50891e6.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/webpack-7dec9f7d48b7e6f8.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/webpack-7dec9f7d48b7e6f8.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/webpack-929d3d7cef65c790.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/webpack-929d3d7cef65c790.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/webpack-962cf26a2870754f.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/webpack-962cf26a2870754f.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/webpack-973edf575a1afde9.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/webpack-973edf575a1afde9.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/webpack-ad6a98aa3061f47c.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/webpack-ad6a98aa3061f47c.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/webpack-b82d5cfb9ad31867.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/webpack-b82d5cfb9ad31867.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/webpack-d9150ed736d780c1.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/webpack-d9150ed736d780c1.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/webpack-e3fb025be7fc31b6.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/webpack-e3fb025be7fc31b6.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/webpack-e8ca2e84678d9188.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/webpack-e8ca2e84678d9188.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/chunks/webpack-f137e28ede23552f.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/chunks/webpack-f137e28ede23552f.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/ciXFpmau1SdpuSwnS4h7-/_buildManifest.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/ciXFpmau1SdpuSwnS4h7-/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/css/0498f7c446a726e9.css` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/css/0498f7c446a726e9.css`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/css/1d3dba75de6e341d.css` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/css/1d3dba75de6e341d.css`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/css/230b09fe1800464e.css` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/css/230b09fe1800464e.css`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/css/29fa82f47e877363.css` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/css/29fa82f47e877363.css`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/css/5eae4c2ec3051cd7.css` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/css/5eae4c2ec3051cd7.css`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/css/5f29c576294b8875.css` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/css/5f29c576294b8875.css`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/css/6b9a855a65274a9d.css` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/css/6b9a855a65274a9d.css`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/css/8e73cf102487ac8c.css` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/css/8e73cf102487ac8c.css`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/css/ba3601c7d877a774.css` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/css/ba3601c7d877a774.css`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/css/da2f78b33f664c71.css` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/css/da2f78b33f664c71.css`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/css/ddc29201eb54d38e.css` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/css/ddc29201eb54d38e.css`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/css/eb3caac5e60c1076.css` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/css/eb3caac5e60c1076.css`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/css/eb98ddacea444f62.css` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/css/eb98ddacea444f62.css`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/css/f27c22d149b2a6fe.css` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/css/f27c22d149b2a6fe.css`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/jvIZeMAH6w8GF8zRcPJET/_buildManifest.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/jvIZeMAH6w8GF8zRcPJET/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/kBlJ9ovXshnAFh_k1E86k/_buildManifest.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/kBlJ9ovXshnAFh_k1E86k/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/media/4049f3f580e14086-s.p.woff2` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/media/4049f3f580e14086-s.p.woff2`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/media/84a5d21698cdcea6-s.woff2` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/media/84a5d21698cdcea6-s.woff2`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/media/a1471ccaedd577d0-s.woff2` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/media/a1471ccaedd577d0-s.woff2`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/media/df5e9368d28a76aa-s.woff2` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/media/df5e9368d28a76aa-s.woff2`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/_next/static/vv1EB3RpwUwq255x5fhm7/_buildManifest.js` & `goldenverba-0.4.0/goldenverba/server/frontend/out/_next/static/vv1EB3RpwUwq255x5fhm7/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/about.html` & `goldenverba-0.4.0/goldenverba/server/frontend/out/about.html`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/background.png` & `goldenverba-0.4.0/goldenverba/server/frontend/out/background.png`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/document_explorer.html` & `goldenverba-0.4.0/goldenverba/server/frontend/out/document_explorer.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><link rel="icon" type="image/png" href="static/favicon.png"/><meta name="next-head-count" content="3"/><link rel="preload" href="/static/_next/static/media/4049f3f580e14086-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/static/_next/static/css/230b09fe1800464e.css" as="style"/><link rel="stylesheet" href="/static/_next/static/css/230b09fe1800464e.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/static/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/static/_next/static/chunks/webpack-67916544a50891e6.js" defer=""></script><script src="/static/_next/static/chunks/framework-7b01e204987c8f43.js" defer=""></script><script src="/static/_next/static/chunks/main-c9732fa3c1d6d1d5.js" defer=""></script><script src="/static/_next/static/chunks/pages/_app-7a548c247b0896b0.js" defer=""></script><script src="/static/_next/static/chunks/246-8cba9c3e138a3cf5.js" defer=""></script><script src="/static/_next/static/chunks/pages/document_explorer-16e4de29624eb562.js" defer=""></script><script src="/static/_next/static/dFAJVlvKY7TnN7l9nf2qs/_buildManifest.js" defer=""></script><script src="/static/_next/static/dFAJVlvKY7TnN7l9nf2qs/_ssgManifest.js" defer=""></script></head><body><div id="__next"><div class="__className_320369"><nav class="fixed bottom-0 left-0 right-0 z-50 bg-gray-100 p-2 shadow-md"><div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8"><div class="flex justify-center items-center py-2"><a class="mx-4 p-3 w-28 text-center rounded-lg text-black text-sm shadow-sm border-2 bg-gray-300 border-gray-400 hover:bg-gray-200 transition-colors duration-300" href="/">Search</a><a class="mx-4 p-3 w-28 text-center rounded-lg text-black text-sm shadow-sm border-2 bg-green-300 border-white hover:bg-gray-200 transition-colors duration-300" href="/document_explorer">Documents</a><a class="mx-4 p-3 w-28 text-center rounded-lg text-black text-sm shadow-sm border-2 bg-gray-300 border-gray-400 hover:bg-gray-200 transition-colors duration-300" href="/status">Status</a></div></div></nav><main class="flex min-h-screen flex-col items-center justify-between p-10 text-gray-900"><div class="flex flex-col w-full items-start"><div class="mb-2"><div class="flex justify-between items-center w-full"> <div class="flex-none"><div class="bg-yellow-200 border-2 border-gray-800 rounded-lg shadow-lg animate-pop-in hover-container mr-4 "><img src="static/verba.png" alt="Verba Logo" class=" w-24 h-24 shadow-lg"/></div></div><div class="flex-1"><h1 class=" text-6xl font-bold">Verba</h1><div class="flex text-lg"><span class="bg-opacity-0 rounded px-2 py-1 hover-container animate-pop-in">The</span><span class="bg-opacity-0 rounded font-bold px-2 py-1 hover-container animate-pop-in-late">Golden</span><span class="bg-yellow-200 rounded px-2 py-1 hover-container animate-pop-more-late">RAGtriever</span></div></div><div class="flex justify-between items-center mx-auto p-4 ml-10"><button class="flex items-center animate-pop-in space-x-2 mr-8 bg-gray-200 text-black p-3  rounded-lg  hover:bg-green-400 border-2 border-black hover:border-white hover-container shadow-md"><svg stroke="currentColor" fill="currentColor" stroke-width="0" viewBox="0 0 448 512" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><path d="M416 208H272V64c0-17.67-14.33-32-32-32h-32c-17.67 0-32 14.33-32 32v144H32c-17.67 0-32 14.33-32 32v32c0 17.67 14.33 32 32 32h144v144c0 17.67 14.33 32 32 32h32c17.67 0 32-14.33 32-32V304h144c17.67 0 32-14.33 32-32v-32c0-17.67-14.33-32-32-32z"></path></svg><span>Add Documents</span></button><div class="ml-5 animate-pop-in"><div class="flex items-center"> <button class="flex items-center md:w-44 sm:w-32 space-x-2 bg-gray-200 text-black p-3 rounded-lg hover:bg-fuchsia-300 border-2 border-black hover:border-white hover-container shadow-md"><svg stroke="currentColor" fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><path stroke="none" d="M0 0h24v24H0z" fill="none"></path><path d="M10 4m0 1a1 1 0 0 1 1 -1h2a1 1 0 0 1 1 1v2a1 1 0 0 1 -1 1h-2a1 1 0 0 1 -1 -1z"></path><path d="M3 17m0 1a1 1 0 0 1 1 -1h2a1 1 0 0 1 1 1v2a1 1 0 0 1 -1 1h-2a1 1 0 0 1 -1 -1z"></path><path d="M17 17m0 1a1 1 0 0 1 1 -1h2a1 1 0 0 1 1 1v2a1 1 0 0 1 -1 1h-2a1 1 0 0 1 -1 -1z"></path><path d="M6.5 17.1l5 -9.1"></path><path d="M17.5 17.1l-5 -9.1"></path><path d="M7 19l10 0"></path></svg><span class="truncate">None</span></button><div class="relative ml-2"><button class="w-8 h-8 bg-gray-100 rounded-full flex items-center justify-center text-gray-400 border-2 border-gray-400 hover:border-white hover-container shadow-md">?</button></div></div></div></div></div></div><div class="flex w-full space-x-4 mt-28"><div class="flex-1 bg-white border-2 overflow-y-auto border-black bg-opacity-20 rounded-lg shadow-md backdrop-filter min-h-[50vh] backdrop-blur-md p-4 w-1/3 animate-pop-in"><div class="p-2"><div class="flex justify-between items-center mb-4"> <h2 class="text-lg font-bold mb-4">📚 Documents</h2></div><p class="text-xs font-bold mb-4 text-gray-600">Search through all your <!-- -->0<!-- --> imported documents embedded by </p><div class="rounded-lg flex justify- between items-center"><form class="rounded-b-xl p-2 w-full"><input type="text" name="searchInput" placeholder="Search for documents" class="w-full p-2 rounded-md bg-white text-gray-900 placeholder-gray-400"/></form><select class="mr-2 bg-white text-gray-900 p-2 rounded-md"><option value="All types" selected="">All types</option></select></div><hr/></div></div><div class="w-2/3 space-y-4"><div class=""></div></div></div></div></main></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/document_explorer","query":{},"buildId":"dFAJVlvKY7TnN7l9nf2qs","assetPrefix":"/static","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><link rel="icon" type="image/png" href="static/favicon.png"/><meta name="next-head-count" content="3"/><link rel="preload" href="/static/_next/static/media/4049f3f580e14086-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/static/_next/static/css/230b09fe1800464e.css" as="style"/><link rel="stylesheet" href="/static/_next/static/css/230b09fe1800464e.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/static/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/static/_next/static/chunks/webpack-67916544a50891e6.js" defer=""></script><script src="/static/_next/static/chunks/framework-7b01e204987c8f43.js" defer=""></script><script src="/static/_next/static/chunks/main-c9732fa3c1d6d1d5.js" defer=""></script><script src="/static/_next/static/chunks/pages/_app-c1589fca75958036.js" defer=""></script><script src="/static/_next/static/chunks/246-8cba9c3e138a3cf5.js" defer=""></script><script src="/static/_next/static/chunks/pages/document_explorer-16e4de29624eb562.js" defer=""></script><script src="/static/_next/static/_A-piGxRm1B_OMIwQ_tPn/_buildManifest.js" defer=""></script><script src="/static/_next/static/_A-piGxRm1B_OMIwQ_tPn/_ssgManifest.js" defer=""></script></head><body><div id="__next"><div class="__className_320369"><nav class="fixed bottom-0 left-0 right-0 z-50 bg-gray-100 p-2 shadow-md"><div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8"><div class="flex justify-center items-center py-2"><a class="mx-4 p-3 w-28 text-center rounded-lg text-black text-sm shadow-sm border-2 bg-gray-300 border-gray-400 hover:bg-gray-200 transition-colors duration-300" href="/">Search</a><a class="mx-4 p-3 w-28 text-center rounded-lg text-black text-sm shadow-sm border-2 bg-green-300 border-white hover:bg-gray-200 transition-colors duration-300" href="/document_explorer">Documents</a><a class="mx-4 p-3 w-28 text-center rounded-lg text-black text-sm shadow-sm border-2 bg-gray-300 border-gray-400 hover:bg-gray-200 transition-colors duration-300" href="/status">Status</a></div></div></nav><main class="flex min-h-screen flex-col items-center justify-between p-10 text-gray-900"><div class="flex flex-col w-full items-start"><div class="mb-2"><div class="flex justify-between items-center w-full"> <div class="flex-none"><div class="bg-yellow-200 border-2 border-gray-800 rounded-lg shadow-lg animate-pop-in hover-container mr-4 "><img src="static/verba.png" alt="Verba Logo" class=" w-24 h-24 shadow-lg"/></div></div><div class="flex-1"><h1 class=" text-6xl font-bold">Verba</h1><div class="flex text-lg"><span class="bg-opacity-0 rounded px-2 py-1 hover-container animate-pop-in">The</span><span class="bg-opacity-0 rounded font-bold px-2 py-1 hover-container animate-pop-in-late">Golden</span><span class="bg-yellow-200 rounded px-2 py-1 hover-container animate-pop-more-late">RAGtriever</span></div></div><div class="flex justify-between items-center mx-auto p-4 ml-10"><button class="flex items-center animate-pop-in space-x-2 mr-8 bg-gray-200 text-black p-3  rounded-lg  hover:bg-green-400 border-2 border-black hover:border-white hover-container shadow-md"><svg stroke="currentColor" fill="currentColor" stroke-width="0" viewBox="0 0 448 512" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><path d="M416 208H272V64c0-17.67-14.33-32-32-32h-32c-17.67 0-32 14.33-32 32v144H32c-17.67 0-32 14.33-32 32v32c0 17.67 14.33 32 32 32h144v144c0 17.67 14.33 32 32 32h32c17.67 0 32-14.33 32-32V304h144c17.67 0 32-14.33 32-32v-32c0-17.67-14.33-32-32-32z"></path></svg><span>Add Documents</span></button><div class="ml-5 animate-pop-in"><div class="flex items-center"> <button class="flex items-center md:w-44 sm:w-32 space-x-2 bg-gray-200 text-black p-3 rounded-lg hover:bg-fuchsia-300 border-2 border-black hover:border-white hover-container shadow-md"><svg stroke="currentColor" fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><path stroke="none" d="M0 0h24v24H0z" fill="none"></path><path d="M10 4m0 1a1 1 0 0 1 1 -1h2a1 1 0 0 1 1 1v2a1 1 0 0 1 -1 1h-2a1 1 0 0 1 -1 -1z"></path><path d="M3 17m0 1a1 1 0 0 1 1 -1h2a1 1 0 0 1 1 1v2a1 1 0 0 1 -1 1h-2a1 1 0 0 1 -1 -1z"></path><path d="M17 17m0 1a1 1 0 0 1 1 -1h2a1 1 0 0 1 1 1v2a1 1 0 0 1 -1 1h-2a1 1 0 0 1 -1 -1z"></path><path d="M6.5 17.1l5 -9.1"></path><path d="M17.5 17.1l-5 -9.1"></path><path d="M7 19l10 0"></path></svg><span class="truncate">None</span></button><div class="relative ml-2"><button class="w-8 h-8 bg-gray-100 rounded-full flex items-center justify-center text-gray-400 border-2 border-gray-400 hover:border-white hover-container shadow-md">?</button></div></div></div></div></div></div><div class="flex w-full space-x-4 mt-28"><div class="flex-1 bg-white border-2 overflow-y-auto border-black bg-opacity-20 rounded-lg shadow-md backdrop-filter min-h-[50vh] backdrop-blur-md p-4 w-1/3 animate-pop-in"><div class="p-2"><div class="flex justify-between items-center mb-4"> <h2 class="text-lg font-bold mb-4">📚 Documents</h2></div><p class="text-xs font-bold mb-4 text-gray-600">Search through all your <!-- -->0<!-- --> imported documents embedded by </p><div class="rounded-lg flex justify- between items-center"><form class="rounded-b-xl p-2 w-full"><input type="text" name="searchInput" placeholder="Search for documents" class="w-full p-2 rounded-md bg-white text-gray-900 placeholder-gray-400"/></form><select class="mr-2 bg-white text-gray-900 p-2 rounded-md"><option value="All types" selected="">All types</option></select></div><hr/></div></div><div class="w-2/3 space-y-4"><div class=""></div></div></div></div></main></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/document_explorer","query":{},"buildId":"_A-piGxRm1B_OMIwQ_tPn","assetPrefix":"/static","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/favicon.ico` & `goldenverba-0.4.0/goldenverba/server/frontend/out/favicon.ico`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/favicon.png` & `goldenverba-0.4.0/goldenverba/server/frontend/out/favicon.png`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/index.html` & `goldenverba-0.4.0/goldenverba/server/frontend/out/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><link rel="icon" type="image/png" href="static/favicon.png"/><meta name="next-head-count" content="3"/><link rel="preload" href="/static/_next/static/media/4049f3f580e14086-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/static/_next/static/css/230b09fe1800464e.css" as="style"/><link rel="stylesheet" href="/static/_next/static/css/230b09fe1800464e.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/static/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/static/_next/static/chunks/webpack-67916544a50891e6.js" defer=""></script><script src="/static/_next/static/chunks/framework-7b01e204987c8f43.js" defer=""></script><script src="/static/_next/static/chunks/main-c9732fa3c1d6d1d5.js" defer=""></script><script src="/static/_next/static/chunks/pages/_app-7a548c247b0896b0.js" defer=""></script><script src="/static/_next/static/chunks/pages/index-491c7585514c00a2.js" defer=""></script><script src="/static/_next/static/dFAJVlvKY7TnN7l9nf2qs/_buildManifest.js" defer=""></script><script src="/static/_next/static/dFAJVlvKY7TnN7l9nf2qs/_ssgManifest.js" defer=""></script></head><body><div id="__next"><div class="__className_320369"><nav class="fixed bottom-0 left-0 right-0 z-50 bg-gray-100 p-2 shadow-md"><div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8"><div class="flex justify-center items-center py-2"><a class="mx-4 p-3 w-28 text-center rounded-lg text-black text-sm shadow-sm border-2 bg-green-300 border-white hover:bg-gray-200 transition-colors duration-300" href="/">Search</a><a class="mx-4 p-3 w-28 text-center rounded-lg text-black text-sm shadow-sm border-2 bg-gray-300 border-gray-400 hover:bg-gray-200 transition-colors duration-300" href="/document_explorer">Documents</a><a class="mx-4 p-3 w-28 text-center rounded-lg text-black text-sm shadow-sm border-2 bg-gray-300 border-gray-400 hover:bg-gray-200 transition-colors duration-300" href="/status">Status</a></div></div></nav><main class="flex min-h-screen flex-col items-center justify-between p-10 text-gray-900"><div class="flex flex-col w-full items-start"><div class="mb-2"><div class="flex justify-between items-center w-full"> <div class="flex-none"><div class="bg-yellow-200 border-2 border-gray-800 rounded-lg shadow-lg animate-pop-in hover-container mr-4 "><img src="static/verba.png" alt="Verba Logo" class=" w-24 h-24 shadow-lg"/></div></div><div class="flex-1"><h1 class=" text-6xl font-bold">Verba</h1><div class="flex text-lg"><span class="bg-opacity-0 rounded px-2 py-1 hover-container animate-pop-in">The</span><span class="bg-opacity-0 rounded font-bold px-2 py-1 hover-container animate-pop-in-late">Golden</span><span class="bg-yellow-200 rounded px-2 py-1 hover-container animate-pop-more-late">RAGtriever</span></div></div><div class="lg:flex sm:grid sm:grid-cols-2 sm:gap-y-2 md:grid md:grid-cols-2 md:gap-x-4 md:gap-y-4 justify-between items-center mx-auto p-4 ml-10"><div class="ml-5 animate-pop-in"><div class="flex items-center"><button class="flex items-center sm:w-32 md:w-44 space-x-2 mr-8 bg-gray-200 text-black p-3  rounded-lg  hover:bg-green-400 border-2 border-black hover:border-white hover-container shadow-md"><svg stroke="currentColor" fill="currentColor" stroke-width="0" viewBox="0 0 448 512" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><path d="M416 208H272V64c0-17.67-14.33-32-32-32h-32c-17.67 0-32 14.33-32 32v144H32c-17.67 0-32 14.33-32 32v32c0 17.67 14.33 32 32 32h144v144c0 17.67 14.33 32 32 32h32c17.67 0 32-14.33 32-32V304h144c17.67 0 32-14.33 32-32v-32c0-17.67-14.33-32-32-32z"></path></svg><span class="truncate">Add Documents</span></button></div></div><div class="ml-5 animate-pop-in"><div class="flex items-center"> <button class="flex items-center md:w-44 sm:w-32 space-x-2 bg-gray-200 text-black p-3 rounded-lg hover:bg-fuchsia-300 border-2 border-black hover:border-white hover-container shadow-md"><svg stroke="currentColor" fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><path stroke="none" d="M0 0h24v24H0z" fill="none"></path><path d="M10 4m0 1a1 1 0 0 1 1 -1h2a1 1 0 0 1 1 1v2a1 1 0 0 1 -1 1h-2a1 1 0 0 1 -1 -1z"></path><path d="M3 17m0 1a1 1 0 0 1 1 -1h2a1 1 0 0 1 1 1v2a1 1 0 0 1 -1 1h-2a1 1 0 0 1 -1 -1z"></path><path d="M17 17m0 1a1 1 0 0 1 1 -1h2a1 1 0 0 1 1 1v2a1 1 0 0 1 -1 1h-2a1 1 0 0 1 -1 -1z"></path><path d="M6.5 17.1l5 -9.1"></path><path d="M17.5 17.1l-5 -9.1"></path><path d="M7 19l10 0"></path></svg><span class="truncate">None</span></button><div class="relative ml-2"><button class="w-8 h-8 bg-gray-100 rounded-full flex items-center justify-center text-gray-400 border-2 border-gray-400 hover:border-white hover-container shadow-md">?</button></div></div></div><div class="ml-5 animate-pop-in"><div class="flex items-center"> <button class="flex items-center md:w-44 sm:w-32 space-x-2 bg-gray-200 text-black p-3 rounded-lg hover:bg-indigo-300 border-2 border-black hover:border-white hover-container shadow-md"><svg stroke="currentColor" fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><path d="M4 22h14a2 2 0 0 0 2-2V7.5L14.5 2H6a2 2 0 0 0-2 2v4"></path><polyline points="14 2 14 8 20 8"></polyline><path d="M2 15h10"></path><path d="m5 12-3 3 3 3"></path></svg><span class="truncate">None</span></button><div class="relative ml-2"><button class="w-8 h-8 bg-gray-100 rounded-full flex items-center justify-center text-gray-400 border-2 border-gray-400 hover:border-white hover-container shadow-md">?</button></div></div></div><div class="ml-5 animate-pop-in"><div class="flex items-center"> <button class="flex items-center md:w-44 sm:w-32 space-x-2 bg-gray-200 text-black p-3 rounded-lg hover:bg-lime-400 border-2 border-black hover:border-white hover-container shadow-md"><svg stroke="currentColor" fill="currentColor" stroke-width="0" viewBox="0 0 24 24" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><path fill="none" d="M0 0h24v24H0V0z"></path><path d="M15 4v7H5.17l-.59.59-.58.58V4h11m1-2H3c-.55 0-1 .45-1 1v14l4-4h10c.55 0 1-.45 1-1V3c0-.55-.45-1-1-1zm5 4h-2v9H6v2c0 .55.45 1 1 1h11l4 4V7c0-.55-.45-1-1-1z"></path></svg><span class="truncate">None</span></button><div class="relative ml-2"><button class="w-8 h-8 bg-gray-100 rounded-full flex items-center justify-center text-gray-400 border-2 border-gray-400 hover:border-white hover-container shadow-md">?</button></div></div></div></div></div></div><div class="lg:flex md:flex full:justify-center justify-items-start overflow-x-auto h-36 w-full mb-2 hidden"></div><div class="flex w-full space-x-4 overflow-y-auto mb-20"><div class="lg:w-1/2 md:w-full sm:w-full p-2 border-2 shadow-lg border-gray-900 rounded-xl animate-pop-in"><div class="rounded-t-xl bg-gray-200 p-4 flex justify-between items-center">🐕 RAGtriever Chat<div class="text-xs text-white font-mono flex justify-center"><a href="https://github.com/weaviate/Verba" target="_blank" rel="noopener noreferrer"><span class="rounded-indicator hover-container text-white p-2 bg-red-500 hover:bg-red-400">Offline v0.3.1</span></a><a href="https://www.weaviate.io" target="_blank" rel="noopener noreferrer"><span class="rounded-indicator text-white bg-gray-400 hover:bg-gray-300 ml-2 p-2 hover-container">Powered by Weaviate ❤️</span></a></div></div><div class="bg-gray-100 p-4 overflow-y-auto h-[35vh]"></div><form class="rounded-b-xl bg-gray-500 p-4 relative"><input type="text" placeholder="What is a vector database?" class="w-full p-2 rounded-md bg-white text-gray-900 placeholder-gray-400" value=""/></form><div class="absolute mt-2 p-2 z-10 w-1/2 left-5 text-center justify-center flex flex-wrap"></div></div><div class="w-1/2 space-y-4 hidden lg:block md:block"><div class=""></div></div></div></div></main></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"dFAJVlvKY7TnN7l9nf2qs","assetPrefix":"/static","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><link rel="icon" type="image/png" href="static/favicon.png"/><meta name="next-head-count" content="3"/><link rel="preload" href="/static/_next/static/media/4049f3f580e14086-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/static/_next/static/css/230b09fe1800464e.css" as="style"/><link rel="stylesheet" href="/static/_next/static/css/230b09fe1800464e.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/static/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/static/_next/static/chunks/webpack-67916544a50891e6.js" defer=""></script><script src="/static/_next/static/chunks/framework-7b01e204987c8f43.js" defer=""></script><script src="/static/_next/static/chunks/main-c9732fa3c1d6d1d5.js" defer=""></script><script src="/static/_next/static/chunks/pages/_app-c1589fca75958036.js" defer=""></script><script src="/static/_next/static/chunks/pages/index-491c7585514c00a2.js" defer=""></script><script src="/static/_next/static/_A-piGxRm1B_OMIwQ_tPn/_buildManifest.js" defer=""></script><script src="/static/_next/static/_A-piGxRm1B_OMIwQ_tPn/_ssgManifest.js" defer=""></script></head><body><div id="__next"><div class="__className_320369"><nav class="fixed bottom-0 left-0 right-0 z-50 bg-gray-100 p-2 shadow-md"><div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8"><div class="flex justify-center items-center py-2"><a class="mx-4 p-3 w-28 text-center rounded-lg text-black text-sm shadow-sm border-2 bg-green-300 border-white hover:bg-gray-200 transition-colors duration-300" href="/">Search</a><a class="mx-4 p-3 w-28 text-center rounded-lg text-black text-sm shadow-sm border-2 bg-gray-300 border-gray-400 hover:bg-gray-200 transition-colors duration-300" href="/document_explorer">Documents</a><a class="mx-4 p-3 w-28 text-center rounded-lg text-black text-sm shadow-sm border-2 bg-gray-300 border-gray-400 hover:bg-gray-200 transition-colors duration-300" href="/status">Status</a></div></div></nav><main class="flex min-h-screen flex-col items-center justify-between p-10 text-gray-900"><div class="flex flex-col w-full items-start"><div class="mb-2"><div class="flex justify-between items-center w-full"> <div class="flex-none"><div class="bg-yellow-200 border-2 border-gray-800 rounded-lg shadow-lg animate-pop-in hover-container mr-4 "><img src="static/verba.png" alt="Verba Logo" class=" w-24 h-24 shadow-lg"/></div></div><div class="flex-1"><h1 class=" text-6xl font-bold">Verba</h1><div class="flex text-lg"><span class="bg-opacity-0 rounded px-2 py-1 hover-container animate-pop-in">The</span><span class="bg-opacity-0 rounded font-bold px-2 py-1 hover-container animate-pop-in-late">Golden</span><span class="bg-yellow-200 rounded px-2 py-1 hover-container animate-pop-more-late">RAGtriever</span></div></div><div class="lg:flex sm:grid sm:grid-cols-2 sm:gap-y-2 md:grid md:grid-cols-2 md:gap-x-4 md:gap-y-4 justify-between items-center mx-auto p-4 ml-10"><div class="ml-5 animate-pop-in"><div class="flex items-center"><button class="flex items-center sm:w-32 md:w-44 space-x-2 mr-8 bg-gray-200 text-black p-3  rounded-lg  hover:bg-green-400 border-2 border-black hover:border-white hover-container shadow-md"><svg stroke="currentColor" fill="currentColor" stroke-width="0" viewBox="0 0 448 512" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><path d="M416 208H272V64c0-17.67-14.33-32-32-32h-32c-17.67 0-32 14.33-32 32v144H32c-17.67 0-32 14.33-32 32v32c0 17.67 14.33 32 32 32h144v144c0 17.67 14.33 32 32 32h32c17.67 0 32-14.33 32-32V304h144c17.67 0 32-14.33 32-32v-32c0-17.67-14.33-32-32-32z"></path></svg><span class="truncate">Add Documents</span></button></div></div><div class="ml-5 animate-pop-in"><div class="flex items-center"> <button class="flex items-center md:w-44 sm:w-32 space-x-2 bg-gray-200 text-black p-3 rounded-lg hover:bg-fuchsia-300 border-2 border-black hover:border-white hover-container shadow-md"><svg stroke="currentColor" fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><path stroke="none" d="M0 0h24v24H0z" fill="none"></path><path d="M10 4m0 1a1 1 0 0 1 1 -1h2a1 1 0 0 1 1 1v2a1 1 0 0 1 -1 1h-2a1 1 0 0 1 -1 -1z"></path><path d="M3 17m0 1a1 1 0 0 1 1 -1h2a1 1 0 0 1 1 1v2a1 1 0 0 1 -1 1h-2a1 1 0 0 1 -1 -1z"></path><path d="M17 17m0 1a1 1 0 0 1 1 -1h2a1 1 0 0 1 1 1v2a1 1 0 0 1 -1 1h-2a1 1 0 0 1 -1 -1z"></path><path d="M6.5 17.1l5 -9.1"></path><path d="M17.5 17.1l-5 -9.1"></path><path d="M7 19l10 0"></path></svg><span class="truncate">None</span></button><div class="relative ml-2"><button class="w-8 h-8 bg-gray-100 rounded-full flex items-center justify-center text-gray-400 border-2 border-gray-400 hover:border-white hover-container shadow-md">?</button></div></div></div><div class="ml-5 animate-pop-in"><div class="flex items-center"> <button class="flex items-center md:w-44 sm:w-32 space-x-2 bg-gray-200 text-black p-3 rounded-lg hover:bg-indigo-300 border-2 border-black hover:border-white hover-container shadow-md"><svg stroke="currentColor" fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><path d="M4 22h14a2 2 0 0 0 2-2V7.5L14.5 2H6a2 2 0 0 0-2 2v4"></path><polyline points="14 2 14 8 20 8"></polyline><path d="M2 15h10"></path><path d="m5 12-3 3 3 3"></path></svg><span class="truncate">None</span></button><div class="relative ml-2"><button class="w-8 h-8 bg-gray-100 rounded-full flex items-center justify-center text-gray-400 border-2 border-gray-400 hover:border-white hover-container shadow-md">?</button></div></div></div><div class="ml-5 animate-pop-in"><div class="flex items-center"> <button class="flex items-center md:w-44 sm:w-32 space-x-2 bg-gray-200 text-black p-3 rounded-lg hover:bg-lime-400 border-2 border-black hover:border-white hover-container shadow-md"><svg stroke="currentColor" fill="currentColor" stroke-width="0" viewBox="0 0 24 24" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><path fill="none" d="M0 0h24v24H0V0z"></path><path d="M15 4v7H5.17l-.59.59-.58.58V4h11m1-2H3c-.55 0-1 .45-1 1v14l4-4h10c.55 0 1-.45 1-1V3c0-.55-.45-1-1-1zm5 4h-2v9H6v2c0 .55.45 1 1 1h11l4 4V7c0-.55-.45-1-1-1z"></path></svg><span class="truncate">None</span></button><div class="relative ml-2"><button class="w-8 h-8 bg-gray-100 rounded-full flex items-center justify-center text-gray-400 border-2 border-gray-400 hover:border-white hover-container shadow-md">?</button></div></div></div></div></div></div><div class="lg:flex md:flex full:justify-center justify-items-start overflow-x-auto h-36 w-full mb-2 hidden"></div><div class="flex w-full space-x-4 overflow-y-auto mb-20"><div class="lg:w-1/2 md:w-full sm:w-full p-2 border-2 shadow-lg border-gray-900 rounded-xl animate-pop-in"><div class="rounded-t-xl bg-gray-200 p-4 flex justify-between items-center">🐕 RAGtriever Chat<div class="text-xs text-white font-mono flex justify-center"><a href="https://github.com/weaviate/Verba" target="_blank" rel="noopener noreferrer"><span class="rounded-indicator hover-container text-white p-2 bg-red-500 hover:bg-red-400">Offline v0.4.0</span></a><a href="https://www.weaviate.io" target="_blank" rel="noopener noreferrer"><span class="rounded-indicator text-white bg-gray-400 hover:bg-gray-300 ml-2 p-2 hover-container">Powered by Weaviate ❤️</span></a></div></div><div class="bg-gray-100 p-4 overflow-y-auto h-[35vh]"></div><form class="rounded-b-xl bg-gray-500 p-4 relative"><input type="text" placeholder="What is a vector database?" class="w-full p-2 rounded-md bg-white text-gray-900 placeholder-gray-400" value=""/></form><div class="absolute mt-2 p-2 z-10 w-1/2 left-5 text-center justify-center flex flex-wrap"></div></div><div class="w-1/2 space-y-4 hidden lg:block md:block"><div class=""></div></div></div></div></main></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"_A-piGxRm1B_OMIwQ_tPn","assetPrefix":"/static","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

#### html2text {}

```diff
@@ -6,9 +6,9 @@
 None
 ?
 None
 ?
 None
 ?
 🐕 RAGtriever Chat
-_O_f_f_l_i_n_e_ _v_0_._3_._1_P_o_w_e_r_e_d_ _b_y_ _W_e_a_v_i_a_t_e_ _❤_️
+_O_f_f_l_i_n_e_ _v_0_._4_._0_P_o_w_e_r_e_d_ _b_y_ _W_e_a_v_i_a_t_e_ _❤_️
 [                    ]
```

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/next.svg` & `goldenverba-0.4.0/goldenverba/server/frontend/out/next.svg`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/status.html` & `goldenverba-0.4.0/goldenverba/server/frontend/out/status.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><link rel="icon" type="image/png" href="static/favicon.png"/><meta name="next-head-count" content="3"/><link rel="preload" href="/static/_next/static/media/4049f3f580e14086-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/static/_next/static/css/230b09fe1800464e.css" as="style"/><link rel="stylesheet" href="/static/_next/static/css/230b09fe1800464e.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/static/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/static/_next/static/chunks/webpack-67916544a50891e6.js" defer=""></script><script src="/static/_next/static/chunks/framework-7b01e204987c8f43.js" defer=""></script><script src="/static/_next/static/chunks/main-c9732fa3c1d6d1d5.js" defer=""></script><script src="/static/_next/static/chunks/pages/_app-7a548c247b0896b0.js" defer=""></script><script src="/static/_next/static/chunks/pages/status-5eecffe6be63ff44.js" defer=""></script><script src="/static/_next/static/dFAJVlvKY7TnN7l9nf2qs/_buildManifest.js" defer=""></script><script src="/static/_next/static/dFAJVlvKY7TnN7l9nf2qs/_ssgManifest.js" defer=""></script></head><body><div id="__next"><div class="__className_320369"><nav class="fixed bottom-0 left-0 right-0 z-50 bg-gray-100 p-2 shadow-md"><div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8"><div class="flex justify-center items-center py-2"><a class="mx-4 p-3 w-28 text-center rounded-lg text-black text-sm shadow-sm border-2 bg-gray-300 border-gray-400 hover:bg-gray-200 transition-colors duration-300" href="/">Search</a><a class="mx-4 p-3 w-28 text-center rounded-lg text-black text-sm shadow-sm border-2 bg-gray-300 border-gray-400 hover:bg-gray-200 transition-colors duration-300" href="/document_explorer">Documents</a><a class="mx-4 p-3 w-28 text-center rounded-lg text-black text-sm shadow-sm border-2 bg-green-300 border-white hover:bg-gray-200 transition-colors duration-300" href="/status">Status</a></div></div></nav><main class="flex min-h-screen flex-col items-center justify-between p-10 text-gray-900"><div class="flex flex-col w-full items-start"><div class="mb-2"><div class="flex justify-between items-center w-full"> <div class="flex-none"><div class="bg-yellow-200 border-2 border-gray-800 rounded-lg shadow-lg animate-pop-in hover-container mr-4 "><img src="static/verba.png" alt="Verba Logo" class=" w-24 h-24 shadow-lg"/></div></div><div class="flex-1"><h1 class=" text-6xl font-bold">Verba</h1><div class="flex text-lg"><span class="bg-opacity-0 rounded px-2 py-1 hover-container animate-pop-in">The</span><span class="bg-opacity-0 rounded font-bold px-2 py-1 hover-container animate-pop-in-late">Golden</span><span class="bg-yellow-200 rounded px-2 py-1 hover-container animate-pop-more-late">RAGtriever</span></div></div></div></div><div class="flex mt-16 space-x-4 w-full justify-center items-start"> <div class="flex-1 border-2 border-black bg-white bg-opacity-20 rounded-lg shadow-md backdrop-filter max-h-[50vh] backdrop-blur-md p-4 w-full overflow-y-auto animate-pop-in"><h2 class="text-lg font-bold mb-4">🐕 Verba Status</h2><p class="text-xs font-bold mb-4 text-gray-600">This view shows whether your Verba Client is connected to the Backend and which Deployment of Weaviate you are using</p><hr/><div class="grid grid-rows-2 gap-2 mt-4"><button title="" class="relative flex items-center justify-center text-black text-lg mt-4 bg-gray-300 rounded-lg font-bold border-2 border-black animate-pop-in-late p-4 w-full shadow-md mr-6 hover:bg-gray-200 hover:border-white"><span class="block truncate">Backend</span><span class="block absolute top-2/3 mt-3 text-sm bg-red-300 rounded-lg px-2 truncate text-xs">Offline</span></button><button title="" class="relative flex items-center justify-center text-black text-lg mt-4 bg-gray-300 rounded-lg font-bold border-2 border-black animate-pop-in-late p-4 w-full shadow-md mr-6 hover:bg-gray-200 hover:border-white"><span class="block truncate">Weaviate</span><span class="block absolute top-2/3 mt-3 text-sm bg-red-300 rounded-lg px-2 truncate text-xs">Offline</span></button></div></div><div class="flex-1 border-2 border-black bg-white bg-opacity-20 rounded-lg shadow-md backdrop-filter max-h-[50vh] backdrop-blur-md p-4 overflow-y-auto w-full animate-pop-in"><h2 class="text-lg font-bold mb-4">📚 Libraries &amp; Variables</h2><p class="text-xs font-bold mb-4 text-gray-600">This interface lists all available libraries and defined variables.</p><p class="text-xs font-bold mb-4 text-gray-600 mt-2">To set environment variables, create a <code>.env</code> file and define your variables (e.g., <code>OPENAI_API_KEY=Your-Key</code>). Alternatively, you may configure them system-wide. <a href="https://github.com/weaviate/Verba/blob/main/README.md" class="text-sm text-blue-400">Click here</a> for detailed instructions.</p><p class="text-xs font-bold mb-4 text-gray-600 mt-2">To install any required libraries that are not present, use the command <code>pip install Your-Library</code> (for example, <code>pip install spacy</code>).</p><hr/><div class="grid grid-rows-2 gap-2 mt-4"></div></div><div class="flex-1 bg-white border-2 border-black bg-opacity-20 rounded-lg shadow-md backdrop-filter max-h-[50vh] backdrop-blur-md p-4 w-full overflow-y-auto animate-pop-in"><div class="flex justify-between items-center mb-4"> <h2 class="text-lg font-bold">📝 Schemas &amp; Objects</h2></div><p class="text-xs font-bold mb-4 text-gray-600">This view shows all schemas and their object count</p><button class="text-xs bg-gray-400 text-white hover:bg-red-400 hover-container px-3 py-2 rounded-lg mr-2">❌ Reset Verba</button><button class="text-xs bg-gray-400 text-white hover:bg-red-400 hover-container px-3 py-2 rounded-lg mr-2">❌ Reset Cache</button><button class="text-xs bg-gray-400 text-white hover:bg-red-400 hover-container px-3 py-2 rounded-lg">❌ Reset Suggestion</button><hr/><div class="grid grid-rows-2 gap-2 mt-4"></div></div></div></div></main></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/status","query":{},"buildId":"dFAJVlvKY7TnN7l9nf2qs","assetPrefix":"/static","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><link rel="icon" type="image/png" href="static/favicon.png"/><meta name="next-head-count" content="3"/><link rel="preload" href="/static/_next/static/media/4049f3f580e14086-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/static/_next/static/css/230b09fe1800464e.css" as="style"/><link rel="stylesheet" href="/static/_next/static/css/230b09fe1800464e.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/static/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/static/_next/static/chunks/webpack-67916544a50891e6.js" defer=""></script><script src="/static/_next/static/chunks/framework-7b01e204987c8f43.js" defer=""></script><script src="/static/_next/static/chunks/main-c9732fa3c1d6d1d5.js" defer=""></script><script src="/static/_next/static/chunks/pages/_app-c1589fca75958036.js" defer=""></script><script src="/static/_next/static/chunks/pages/status-5eecffe6be63ff44.js" defer=""></script><script src="/static/_next/static/_A-piGxRm1B_OMIwQ_tPn/_buildManifest.js" defer=""></script><script src="/static/_next/static/_A-piGxRm1B_OMIwQ_tPn/_ssgManifest.js" defer=""></script></head><body><div id="__next"><div class="__className_320369"><nav class="fixed bottom-0 left-0 right-0 z-50 bg-gray-100 p-2 shadow-md"><div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8"><div class="flex justify-center items-center py-2"><a class="mx-4 p-3 w-28 text-center rounded-lg text-black text-sm shadow-sm border-2 bg-gray-300 border-gray-400 hover:bg-gray-200 transition-colors duration-300" href="/">Search</a><a class="mx-4 p-3 w-28 text-center rounded-lg text-black text-sm shadow-sm border-2 bg-gray-300 border-gray-400 hover:bg-gray-200 transition-colors duration-300" href="/document_explorer">Documents</a><a class="mx-4 p-3 w-28 text-center rounded-lg text-black text-sm shadow-sm border-2 bg-green-300 border-white hover:bg-gray-200 transition-colors duration-300" href="/status">Status</a></div></div></nav><main class="flex min-h-screen flex-col items-center justify-between p-10 text-gray-900"><div class="flex flex-col w-full items-start"><div class="mb-2"><div class="flex justify-between items-center w-full"> <div class="flex-none"><div class="bg-yellow-200 border-2 border-gray-800 rounded-lg shadow-lg animate-pop-in hover-container mr-4 "><img src="static/verba.png" alt="Verba Logo" class=" w-24 h-24 shadow-lg"/></div></div><div class="flex-1"><h1 class=" text-6xl font-bold">Verba</h1><div class="flex text-lg"><span class="bg-opacity-0 rounded px-2 py-1 hover-container animate-pop-in">The</span><span class="bg-opacity-0 rounded font-bold px-2 py-1 hover-container animate-pop-in-late">Golden</span><span class="bg-yellow-200 rounded px-2 py-1 hover-container animate-pop-more-late">RAGtriever</span></div></div></div></div><div class="flex mt-16 space-x-4 w-full justify-center items-start"> <div class="flex-1 border-2 border-black bg-white bg-opacity-20 rounded-lg shadow-md backdrop-filter max-h-[50vh] backdrop-blur-md p-4 w-full overflow-y-auto animate-pop-in"><h2 class="text-lg font-bold mb-4">🐕 Verba Status</h2><p class="text-xs font-bold mb-4 text-gray-600">This view shows whether your Verba Client is connected to the Backend and which Deployment of Weaviate you are using</p><hr/><div class="grid grid-rows-2 gap-2 mt-4"><button title="" class="relative flex items-center justify-center text-black text-lg mt-4 bg-gray-300 rounded-lg font-bold border-2 border-black animate-pop-in-late p-4 w-full shadow-md mr-6 hover:bg-gray-200 hover:border-white"><span class="block truncate">Backend</span><span class="block absolute top-2/3 mt-3 text-sm bg-red-300 rounded-lg px-2 truncate text-xs">Offline</span></button><button title="" class="relative flex items-center justify-center text-black text-lg mt-4 bg-gray-300 rounded-lg font-bold border-2 border-black animate-pop-in-late p-4 w-full shadow-md mr-6 hover:bg-gray-200 hover:border-white"><span class="block truncate">Weaviate</span><span class="block absolute top-2/3 mt-3 text-sm bg-red-300 rounded-lg px-2 truncate text-xs">Offline</span></button></div></div><div class="flex-1 border-2 border-black bg-white bg-opacity-20 rounded-lg shadow-md backdrop-filter max-h-[50vh] backdrop-blur-md p-4 overflow-y-auto w-full animate-pop-in"><h2 class="text-lg font-bold mb-4">📚 Libraries &amp; Variables</h2><p class="text-xs font-bold mb-4 text-gray-600">This interface lists all available libraries and defined variables.</p><p class="text-xs font-bold mb-4 text-gray-600 mt-2">To set environment variables, create a <code>.env</code> file and define your variables (e.g., <code>OPENAI_API_KEY=Your-Key</code>). Alternatively, you may configure them system-wide. <a href="https://github.com/weaviate/Verba/blob/main/README.md" class="text-sm text-blue-400">Click here</a> for detailed instructions.</p><p class="text-xs font-bold mb-4 text-gray-600 mt-2">To install any required libraries that are not present, use the command <code>pip install Your-Library</code> (for example, <code>pip install spacy</code>).</p><hr/><div class="grid grid-rows-2 gap-2 mt-4"></div></div><div class="flex-1 bg-white border-2 border-black bg-opacity-20 rounded-lg shadow-md backdrop-filter max-h-[50vh] backdrop-blur-md p-4 w-full overflow-y-auto animate-pop-in"><div class="flex justify-between items-center mb-4"> <h2 class="text-lg font-bold">📝 Schemas &amp; Objects</h2></div><p class="text-xs font-bold mb-4 text-gray-600">This view shows all schemas and their object count</p><button class="text-xs bg-gray-400 text-white hover:bg-red-400 hover-container px-3 py-2 rounded-lg mr-2">❌ Reset Verba</button><button class="text-xs bg-gray-400 text-white hover:bg-red-400 hover-container px-3 py-2 rounded-lg mr-2">❌ Reset Cache</button><button class="text-xs bg-gray-400 text-white hover:bg-red-400 hover-container px-3 py-2 rounded-lg">❌ Reset Suggestion</button><hr/><div class="grid grid-rows-2 gap-2 mt-4"></div></div></div></div></main></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/status","query":{},"buildId":"_A-piGxRm1B_OMIwQ_tPn","assetPrefix":"/static","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/verba.png` & `goldenverba-0.4.0/goldenverba/server/frontend/out/verba.png`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/frontend/out/vercel.svg` & `goldenverba-0.4.0/goldenverba/server/frontend/out/vercel.svg`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/server/util.py` & `goldenverba-0.4.0/goldenverba/server/util.py`

 * *Files identical despite different names*

### Comparing `goldenverba-0.3.1/goldenverba/verba_manager.py` & `goldenverba-0.4.0/goldenverba/verba_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -149,30 +149,42 @@
         else:
             msg.warn(message)
             return False
 
     def generator_get_generator(self) -> dict[str, Generator]:
         return self.generator_manager.get_generators()
 
-    def setup_client(self) -> Client | None:
+    def setup_client(self):
         """
         @returns Optional[Client] - The Weaviate Client.
         """
         msg.info("Setting up client")
 
         additional_header = {}
         client = None
 
+        openai_header_key_name = "X-OpenAI-Api-Key"
+
         # Check OpenAI ENV KEY
         try:
             import openai
 
             openai_key = os.environ.get("OPENAI_API_KEY", "")
+            if "OPENAI_API_TYPE" in os.environ:
+                openai.api_type = os.getenv("OPENAI_API_TYPE")
+            if "OPENAI_BASE_URL" in os.environ:
+                openai.api_base = os.getenv("OPENAI_BASE_URL")
+            if "OPENAI_API_VERSION" in os.environ:
+                openai.api_version = os.getenv("OPENAI_API_VERSION")
+
+            if os.getenv("OPENAI_API_TYPE") == "azure":
+                openai_header_key_name = "X-Azure-Api-Key"            
+
             if openai_key != "":
-                additional_header["X-OpenAI-Api-Key"] = openai_key
+                additional_header[openai_header_key_name] = openai_key
                 self.environment_variables["OPENAI_API_KEY"] = True
                 openai.api_key = openai_key
             else:
                 self.environment_variables["OPENAI_API_KEY"] = False
 
         except Exception:
             self.environment_variables["OPENAI_API_KEY"] = False
@@ -237,22 +249,14 @@
 
         return client
 
     def verify_installed_libraries(self) -> None:
         """
         Checks which libraries are installed and fills out the self.installed_libraries dictionary for the frontend to access, this will be displayed in the status page.
         """
-        # spaCy, used for Chunking
-        try:
-            import spacy
-
-            self.installed_libraries["spacy"] = True
-        except Exception:
-            self.installed_libraries["spacy"] = False
-
         try:
             import PyPDF2
 
             self.installed_libraries["PyPDF2"] = True
         except Exception:
             self.installed_libraries["PyPDF2"] = False
 
@@ -314,14 +318,19 @@
         """
         # OpenAI API Key
         if os.environ.get("OPENAI_API_KEY", "") != "":
             self.environment_variables["OPENAI_API_KEY"] = True
         else:
             self.environment_variables["OPENAI_API_KEY"] = False
 
+        if os.environ.get("OPENAI_BASE_URL", "") != "":
+            self.environment_variables["OPENAI_BASE_URL"] = True
+        else:
+            self.environment_variables["OPENAI_BASE_URL"] = False
+
         # Cohere API Key
         if os.environ.get("COHERE_API_KEY", "") != "":
             self.environment_variables["COHERE_API_KEY"] = True
         else:
             self.environment_variables["COHERE_API_KEY"] = False
 
         # HuggingFace Key
@@ -343,14 +352,53 @@
             self.environment_variables["UNSTRUCTURED_API_KEY"] = False
 
         # LLAMA2-7B-CHAT-HF
         if os.environ.get("LLAMA2-7B-CHAT-HF", "") == "True":
             self.environment_variables["LLAMA2-7B-CHAT-HF"] = True
         else:
             self.environment_variables["LLAMA2-7B-CHAT-HF"] = False
+        
+        # OpenAI API Type, should be set to "azure" if using Azure OpenAI
+        if os.environ.get("OPENAI_API_TYPE", "") != "":
+            self.environment_variables["OPENAI_API_TYPE"] = True
+        else:
+            self.environment_variables["OPENAI_API_TYPE"] = False
+
+        # OpenAI API Version
+        if os.environ.get("OPENAI_API_VERSION", "") != "":
+            self.environment_variables["OPENAI_API_VERSION"] = True
+        else:
+            self.environment_variables["OPENAI_API_VERSION"] = False
+
+        # Azure openai ressource name, mandatory when using Azure, should be XXX when endpoint is https://XXX.openai.azure.com
+        if os.environ.get("AZURE_OPENAI_RESOURCE_NAME", "") != "":
+            self.environment_variables["AZURE_OPENAI_RESOURCE_NAME"] = True
+        else:
+            self.environment_variables["AZURE_OPENAI_RESOURCE_NAME"] = False
+
+        #Model used for embeddings. mandatory when using Azure. Typically "text-embedding-ada-002"
+        if os.environ.get("AZURE_OPENAI_EMBEDDING_MODEL", "") != "":
+            self.environment_variables["AZURE_OPENAI_EMBEDDING_MODEL"] = True
+        else:
+            self.environment_variables["AZURE_OPENAI_EMBEDDING_MODEL"] = False
+
+        #Model used for queries. mandatory when using Azure, but can also be used to change the model used for queries when using OpenAI.
+        if os.environ.get("OPENAI_MODEL", "") != "":
+            self.environment_variables["OPENAI_MODEL"] = True
+        else:
+            self.environment_variables["OPENAI_MODEL"] = False
+
+        if os.environ.get("OPENAI_API_TYPE", "")=="azure":
+            if not(
+                self.environment_variables["OPENAI_BASE_URL"] and
+                self.environment_variables["AZURE_OPENAI_RESOURCE_NAME"] and
+                self.environment_variables["AZURE_OPENAI_EMBEDDING_MODEL"] and
+                self.environment_variables["OPENAI_MODEL"]
+            ):
+                raise EnvironmentError("Missing environment variables. When using Azure OpenAI, you need to set OPENAI_BASE_URL, AZURE_OPENAI_RESOURCE_NAME, AZURE_OPENAI_EMBEDDING_MODEL and OPENAI_MODEL. Please check documentation.")
 
     def get_schemas(self) -> dict:
         """
         @returns dict - A dictionary with the schema names and their object count.
         """
         schema_info = self.client.schema.get()
         schemas = {}
```

### Comparing `goldenverba-0.3.1/goldenverba.egg-info/PKG-INFO` & `goldenverba-0.4.0/goldenverba.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 Metadata-Version: 2.1
 Name: goldenverba
-Version: 0.3.1
+Version: 0.4.0
 Summary: Welcome to Verba: The Golden RAGtriever, an open-source initiative designed to offer a streamlined, user-friendly interface for Retrieval-Augmented Generation (RAG) applications. In just a few easy steps, dive into your data and make meaningful interactions!
 Home-page: https://github.com/weaviate/Verba
 Author: Weaviate
 Author-email: edward@weaviate.io
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: weaviate-client==3.23.1
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: openai==0.27.9
 Requires-Dist: wasabi==1.1.2
-Requires-Dist: spacy==3.6.1
 Requires-Dist: fastapi==0.102.0
 Requires-Dist: uvicorn[standard]
 Requires-Dist: click==8.1.7
 Requires-Dist: asyncio
 Requires-Dist: tiktoken==0.5.1
 Requires-Dist: cohere==4.33
 Requires-Dist: requests
 Requires-Dist: pypdf2
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: black>=23.7.0; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
 Provides-Extra: huggingface
 Requires-Dist: sentence-transformers; extra == "huggingface"
 Requires-Dist: transformers; extra == "huggingface"
 Requires-Dist: torch; extra == "huggingface"
 Requires-Dist: huggingface_hub; extra == "huggingface"
 Requires-Dist: accelerate; extra == "huggingface"
 
@@ -52,65 +49,65 @@
 
 [![Weaviate](https://img.shields.io/static/v1?label=powered%20by&message=Weaviate%20%E2%9D%A4&color=green&style=flat-square)](https://weaviate.io/) 
 [![PyPi downloads](https://static.pepy.tech/personalized-badge/goldenverba?period=total&units=international_system&left_color=grey&right_color=orange&left_text=pip%20downloads)](https://pypi.org/project/goldenverba/) [![Docker support](https://img.shields.io/badge/Docker_support-%E2%9C%93-4c1?style=flat-square&logo=docker&logoColor=white)](https://docs.docker.com/get-started/) [![Demo](https://img.shields.io/badge/Check%20out%20the%20demo!-yellow?&style=flat-square&logo=react&logoColor=white)](https://verba.weaviate.io/)
 
 ![Demo of Verba](https://github.com/weaviate/Verba/blob/dev/img/verba.gif)
 
 - [Verba](#verba)
-  - [🎯 What Is Verba?](#🎯-what-is-verba)
-  - [⚙️ Under the Hood](#️⚙️-under-the-hood)
-  - [💡 Effortless Data Import with Weaviate](#💡-effortless-data-import-with-weaviate)
-  - [💥 Advanced Query Resolution with Hybrid Search](#💥-advanced-query-resolution-with-hybrid-search)
-  - [🔥 Accelerate Queries with Semantic Cache](#🔥-accelerate-queries-with-semantic-cache)
-- [✨ Getting Started with Verba](#✨-getting-started-with-verba)
-- [🐍 Installing Python and Setting Up a Virtual Environment](#🐍-installing-python-and-setting-up-a-virtual-environment)
+  - [🎯 What Is Verba?](#what-is-verba)
+  - [⚙️ Under the Hood](#️under-the-hood)
+  - [💡 Effortless Data Import with Weaviate](#effortless-data-import-with-weaviate)
+  - [💥 Advanced Query Resolution with Hybrid Search](#advanced-query-resolution-with-hybrid-search)
+  - [🔥 Accelerate Queries with Semantic Cache](#accelerate-queries-with-semantic-cache)
+- [✨ Getting Started with Verba](#getting-started-with-verba)
+- [🐍 Installing Python and Setting Up a Virtual Environment](#installing-python-and-setting-up-a-virtual-environment)
   - [Installing Python](#installing-python)
   - [Setting Up a Virtual Environment](#setting-up-a-virtual-environment)
-- [📦 Choosing the Right Verba Installation Package](#📦-choosing-the-right-verba-installation-package)
+- [📦 Choosing the Right Verba Installation Package](#choosing-the-right-verba-installation-package)
   - [Default Package](#default-package)
   - [HuggingFace Version](#huggingface-version)
   - [Development Version](#development-version)
-- [🚀 Quickstart: Deploy with pip](#🚀-quickstart-deploy-with-pip)
-- [🛠️ Quickstart: Build from Source](#️🛠️-quickstart-build-from-source)
-- [🔑 API Keys](#🔑-api-keys)
+- [🚀 Quickstart: Deploy with pip](#quickstart-deploy-with-pip)
+- [🛠️ Quickstart: Build from Source](#️quickstart-build-from-source)
+- [🔑 API Keys](#api-keys)
   - [Weaviate](#weaviate)
   - [OpenAI](#openai)
   - [Cohere](#cohere)
   - [HuggingFace](#huggingface)
     - [Llama2](#llama2)
   - [Unstructured](#unstructured)
   - [Github](#github)
-- [🐳 Quickstart: Deploy with Docker](#🐳-quickstart-deploy-with-docker)
-  - [Large Language Model (LLM) Costs](#-large-language-model-llm-costs)
-- [💾 Importing Your Data into Verba](#️💾-Importing-Your-Data-into-Verba)
-- [🛠️ Project Architecture](#️🛠️-project-architecture)
-- [💖 Open Source Contribution](#💖-open-source-contribution)
+- [🐳 Quickstart: Deploy with Docker](#quickstart-deploy-with-docker)
+  - [Large Language Model (LLM) Costs](#large-language-model-llm-costs)
+- [💾 Importing Your Data into Verba](#️importing-your-data-into-verba)
+- [🛠️ Project Architecture](#️project-architecture)
+- [💖 Open Source Contribution](#open-source-contribution)
 
-## 🎯 What Is Verba?
+## What Is Verba?
 Verba is more than just a tool—it's a personal assistant for querying and interacting with your data, **either locally or deployed via cloud**. Have questions about your documents? Need to cross-reference multiple data points? Want to gain insights from your existing knowledge base? Verba empowers you with the combined capabilities of Weaviate's context-aware database and the analytical power of Large Language Models (LLMs). Interact with your data through an intuitive chat interface that refines search results by using the ongoing conversation context to deliver even more accurate and relevant information.
 
 ![Demo of Verba](https://github.com/weaviate/Verba/blob/dev/img/verba_screen.png)
 
-### ⚙️ Under the Hood
+### Under the Hood
 Verba is engineered with Weaviate's cutting-edge Generative Search technology at its core, extracting relevant context from your pool of documents to resolve queries with precision. By utilizing the power of Large Language Models, Verba doesn't just search for answers—it understands and provides responses that are contextually rich and informed by the content of your documents, all through an intuitive user interface designed for simplicity and efficiency.
 
-### 💡 Effortless Data Import with Weaviate
+### Effortless Data Import with Weaviate
 Verba offers seamless data import functionality through its frontend, supporting a diverse range of file types including `.txt`, `.md`, `.pdf` and more. Before feeding your data into Weaviate, Verba handles chunking and vectorization to optimize it for search and retrieval. Together with collaborative partners we support popular libraries such as [HuggingFace](https://github.com/huggingface), [Haystack](https://github.com/deepset-ai/haystack), [Unstructured](https://github.com/Unstructured-IO/unstructured) and many more!
 
 ![Demo of Verba](https://github.com/weaviate/Verba/blob/dev/img/verba_import.png)
 
-### 💥 Advanced Query Resolution with Hybrid Search
+### Advanced Query Resolution with Hybrid Search
 Experience the hybrid search capabilities of Weaviate within Verba, which merges vector and lexical search methodologies for even greater precision. This dual approach not only navigates through your documents to pinpoint exact matches but also understands the nuance of context, enabling the Large Language Models to craft responses that are both comprehensive and contextually aware. It's an advanced technique that redefines document retrieval, providing you with precisely what you need, when you need it.
 
-### 🔥 Accelerate Queries with Semantic Cache
+### Accelerate Queries with Semantic Cache
 Verba enhances search efficiency with Weaviate's Semantic Cache, a sophisticated system that retains the essence of your queries, results, and dialogues. This proactive feature means that Verba anticipates your needs, using cached data to expedite future inquiries. With semantic matching, it quickly determines if your question has been asked before, delivering instant results, and even suggests auto-completions based on historical interactions, streamlining your search experience to be faster and more intuitive.
 
 ---
 
-# ✨ Getting Started with Verba
+# Getting Started with Verba
 
 Starting your Verba journey is super easy, with multiple deployment options tailored to your preferences. Follow these simple steps to get Verba up and running:
 
 - Deploy with pip [(Quickstart)](##🚀-Quickstart:-Deploy-with-pip)
 ```
 pip install goldenverba
 ```
@@ -118,18 +115,18 @@
 ```
 git clone https://github.com/weaviate/Verba
 
 pip install -e .
 ```
 - Use Docker for Deployment [(Quickstart)](##🐳-Quickstart:-Deploy-with-Docker)
 
-**Prerequisites**: If you're not using Docker, ensure that you have `Python >=3.9.0` installed on your system.
+**Prerequisites**: If you're not using Docker, ensure that you have `Python >=3.10.0` installed on your system.
 
-# 🐍 Installing Python and Setting Up a Virtual Environment
-Before you can use Verba, you'll need to ensure that `Python >=3.9.0` is installed on your system and that you can create a virtual environment for a safer and cleaner project setup.
+# Installing Python and Setting Up a Virtual Environment
+Before you can use Verba, you'll need to ensure that `Python >=3.10.0` is installed on your system and that you can create a virtual environment for a safer and cleaner project setup.
 
 ## Installing Python
 Python is required to run Verba. If you don't have Python installed, follow these steps:
 
 ### For Windows:
 Download the latest Python installer from the official Python website.
 Run the installer and make sure to check the box that says `Add Python to PATH` during installation.
@@ -176,29 +173,15 @@
 source venv/bin/activate
 ```
 
 Once your virtual environment is activated, you'll see its name in the terminal prompt. Now you're ready to install Verba using the steps provided in the Quickstart sections.
 
 > Remember to deactivate the virtual environment when you're done working with Verba by simply running deactivate in the terminal.
 
-## Linting
-We use [ruff](https://github.com/astral-sh/ruff) for automatic code formation and linting.
-The process is automated with a pre-commit hook. To install the hook, run:
-```
-pre-commit install
-```
-or for shorthand:
-```bash 
-make pre-commit
-```
-After that all your commits will be automatically linted and formatted. The linting will happen only on the files you changed.
-
-`make pre-commit` formats all files in the repository and install the hooks if needed.
-
-# 📦 Choosing the Right Verba Installation Package
+# Choosing the Right Verba Installation Package
 Verba comes in several installation packages, each tailored for specific use cases and environments. Choose the package that aligns with your requirements:
 
 ## Default Package
 The default package is perfect for getting started quickly and includes support for popular models and services like OpenAI, Cohere, and spaCy. This package is suitable for general use and can be installed easily via pip:
 
 ```
 pip install goldenverba
@@ -220,15 +203,15 @@
 
 ```
 pip install goldenverba[dev]
 ```
 
 > Keep in mind that this version is intended for development purposes and may contain experimental features.
 
-# 🚀 Quickstart: Deploy with pip
+# Quickstart: Deploy with pip
 
 1. **Initialize a new Python Environment**
 ```
 python3 -m virtualenv venv
 ```
 
 2. **Install Verba**
@@ -244,15 +227,15 @@
 4. **Access Verba**
 ```
 Visit localhost:8000
 ```
 
 5. **Create .env file and add environment variables**
 
-# 🛠️ Quickstart: Build from Source
+# Quickstart: Build from Source
 
 1. **Clone the Verba repos**
 ```
 git clone https://github.com/weaviate/Verba.git
 ```
 
 2. **Initialize a new Python Environment**
@@ -273,17 +256,20 @@
 5. **Access Verba**
 ```
 Visit localhost:8000
 ```
 
 6. **Create .env file and add environment variables**
 
-# 🔑 API Keys
+# API Keys
+
+Before diving into Verba's capabilities, you'll need to configure access to various components depending on your chosen technologies, such as OpenAI, Cohere, and HuggingFace. Start by obtaining the necessary API keys and setting them up through a `.env` file based on our provided [example](./goldenverba/.env.example) , or by declaring them as environment variables on your system. If you're building from source or using Docker, make sure your `.env` file is within the goldenverba directory.
+Please make sure to only include environment variables you really need.
 
-Before diving into Verba's capabilities, you'll need to configure access to various components depending on your chosen technologies, such as OpenAI, Cohere, and HuggingFace. Start by obtaining the necessary API keys and setting them up through a `.env` file based on our provided [example](./.env.example) , or by declaring them as environment variables on your system. Below is a comprehensive list of the API keys and variables you may require:
+Below is a comprehensive list of the API keys and variables you may require:
 
 ## Weaviate
 Verba provides flexibility in connecting to Weaviate instances based on your needs. By default, Verba opts for [Weaviate Embedded](https://weaviate.io/developers/weaviate/installation/embedded) if it doesn't detect the `WEAVIATE_URL_VERBA` and `WEAVIATE_API_KEY_VERBA` environment variables. This local deployment is the most straightforward way to launch your Weaviate database for prototyping and testing.
 
 However, you have other compelling options to consider:
 
 **🌩️ Weaviate Cloud Service (WCS)**
@@ -303,14 +289,54 @@
 
 Verba supports OpenAI Models such as Ada, GPT3, and GPT4. To use them, you need to specify the `OPENAI_API_KEY` environment variable. You can get it from [OpenAI](https://openai.com/)
 
 ```
 OPENAI_API_KEY=YOUR-OPENAI-KEY
 ```
 
+You can also add a `OPENAI_BASE_URL` to use proxies such as LiteLLM (https://github.com/BerriAI/litellm)
+
+```
+OPENAI_BASE_URL=YOUR-OPENAI_BASE_URL
+```
+
+## Azure OpenAI
+
+To use Azure OpenAI, you need to set 
+
+- The API type:
+```
+OPENAI_API_TYPE="azure"
+```
+
+- The key and the endpoint:
+
+```
+OPENAI_API_KEY=<YOUR_KEY>
+OPENAI_BASE_URL=http://XXX.openai.azure.com
+```
+
+- Azure OpenAI ressource name, which is XXX if your endpoint is XXX.openai.azure.com
+
+```
+AZURE_OPENAI_RESOURCE_NAME=<YOUR_AZURE_RESOURCE_NAME>
+```
+- You need to set the models, for the embeddings and for the query.
+```
+AZURE_OPENAI_EMBEDDING_MODEL="text-embedding-ada-002"
+OPENAI_MODEL="gpt-4" 
+```
+
+- Finally, as Azure is using per-minute quota, you might need to add a waiting time between each chunk upload. For example, if you have a limit of 240k tokens per minute, if your chunks are 
+400 tokens max, then 100ms between queries should be fine. If you get error 429 from weaviate, then increase this value.
+
+```
+WAIT_TIME_BETWEEN_INGESTION_QUERIES_MS="100"
+```
+
 ## Cohere
 
 Verba supports Cohere Models, to use them, you need to specify the `COHERE_API_KEY` environment variable. You can get it from [Cohere](https://dashboard.cohere.com/)
 
 ```
 COHERE_API_KEY=YOUR-COHERE-KEY
 ```
@@ -351,15 +377,15 @@
 
 ## Status Page
 
 Once configured, you can monitor your Verba installation's health and status via the 'Status Verba' page. This dashboard provides insights into your deployment type, libraries, environment settings, Weaviate schema counts, and more. It's also your go-to for maintenance tasks like resetting Verba, clearing the cache, or managing auto-complete suggestions.
 
 ![Demo of Verba](https://github.com/weaviate/Verba/blob/dev/img/verba_status.png)
 
-# 🐳 Quickstart: Deploy with Docker
+# Quickstart: Deploy with Docker
 
 Docker is a set of platform-as-a-service products that use OS-level virtualization to deliver software in packages called containers. Containers are isolated from one another and bundle their own software, libraries, and configuration files; they can communicate with each other through well-defined channels. All containers are run by a single operating system kernel and are thus more lightweight than virtual machines. Docker provides an additional layer of abstraction and automation of operating-system-level virtualization on Windows and Linux.
 
 Docker's use of containers to package software means that the application and its dependencies, libraries, and other binaries are packaged together and can be moved between environments easily. This makes it incredibly useful for developers looking to create predictable environments that are isolated from other applications. 
 
 To get started with deploying Verba using Docker, follow the steps below. If you need more detailed instructions on Docker usage, check out the [Docker Curriculum](https://docker-curriculum.com/).
 
@@ -368,25 +394,47 @@
 0. **Clone the Verba repos**
 Ensure you have Git installed on your system. Then, open a terminal or command prompt and run the following command to clone the Verba repository:
 
 ```
 git clone https://github.com/weaviate/Verba.git
 ```
 
-1. **Deploy using Docker**
+1. **Set neccessary environment variables**
+Make sure to set your required environment variables in the ```.env``` file. You can read more about how to set them up in the [API Keys Section](#api-keys)
+
+2. **Adjust the docker-compose file**
+You can use the ```docker-compose.yml``` to add required environment variables under the ```verba``` service and can also adjust the Weaviate Docker settings to enable Authentification or change other settings of your database instance. You can read more about the Weaviate configuration in our [docker-compose documentation](https://weaviate.io/developers/weaviate/installation/docker-compose)
+
+> Please make sure to only add environment variables that you really need. If have no authentifcation enabled in your Weaviate Cluster, make sure to not include the ```WEAVIATE_API_KEY_VERBA``` enviroment variable
+
+2. **Deploy using Docker**
 With Docker installed and the Verba repository cloned, navigate to the directory containing the Docker Compose file in your terminal or command prompt. Run the following command to start the Verba application in detached mode, which allows it to run in the background:
 
 ```
 docker compose up -d
 ```
 
 This command will download the necessary Docker images, create containers, and start Verba.
 Remember, Docker must be installed on your system to use this method. For installation instructions and more details about Docker, visit the official Docker documentation. 
 
-## 💾 Importing Your Data into Verba
+4. **Access Verba**
+
+- You can access your local Weaviate instance at ```localhost:8080```
+
+- You can access the Verba frontend at ```localhost:8000```
+
+
+If you want your Docker Instance to install a specific version of Verba (as described in the [package section](#choosing-the-right-verba-installation-package)) you can edit the ```Dockerfile``` and change the installation line.
+
+```
+RUN pip install -e '.'
+```
+
+
+## Importing Your Data into Verba
 
 With Verba configured, you're ready to import your data and start exploring. Follow these simple steps to get your data into Verba:
 
 ![Demo of Verba](https://github.com/weaviate/Verba/blob/dev/img/verba_data.gif)
 
 1. **Initiate the Import Process**
    - Click on "Add Documents" to begin.
@@ -412,18 +460,18 @@
      - `CohereEmbedder`: Uses Cohere for embedding.
 
 6. **Commence Data Ingestion**
    - After setting up your preferences, click on "Import" to ingest your data into Verba.
 
 Now your data is ready to be used within Verba, enabling you to leverage its powerful search and retrieval capabilities.
 
-## 💰 Large Language Model (LLM) Costs
+## Large Language Model (LLM) Costs
 
 Verba utilizes LLM models through APIs. Be advised that the usage costs for these models will be billed to the API access key you provide. Primarily, costs are incurred during data embedding and answer generation processes.
 
-## 💖 Open Source Contribution
+## Open Source Contribution
 
 Your contributions are always welcome! Feel free to contribute ideas, feedback, or create issues and bug reports if you find any! Before contributing, please read the [Contribution Guide](./CONTRIBUTING.md). Visit our [Weaviate Community Forum](https://forum.weaviate.io/) if you need any help!
 
-### 🛠️ Project Architecture
+### Project Architecture
 You can learn more about Verba's architecture and implementation in its [technical documentation](./TECHNICAL.md) and [frontend documentation](./FRONTEND.md). It's recommended to read them before making any contributions.
```

### Comparing `goldenverba-0.3.1/goldenverba.egg-info/SOURCES.txt` & `goldenverba-0.4.0/goldenverba.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 MANIFEST.in
 README.md
-pyproject.toml
 setup.py
 goldenverba/__init__.py
 goldenverba/verba_manager.py
 goldenverba.egg-info/PKG-INFO
 goldenverba.egg-info/SOURCES.txt
 goldenverba.egg-info/dependency_links.txt
 goldenverba.egg-info/entry_points.txt
@@ -13,17 +12,15 @@
 goldenverba.egg-info/top_level.txt
 goldenverba/components/__init__.py
 goldenverba/components/component.py
 goldenverba/components/chunking/__init__.py
 goldenverba/components/chunking/chunk.py
 goldenverba/components/chunking/interface.py
 goldenverba/components/chunking/manager.py
-goldenverba/components/chunking/sentencechunker.py
 goldenverba/components/chunking/tiktokenchunker.py
-goldenverba/components/chunking/wordchunker.py
 goldenverba/components/embedding/ADAEmbedder.py
 goldenverba/components/embedding/CohereEmbedder.py
 goldenverba/components/embedding/MiniLMEmbedder.py
 goldenverba/components/embedding/__init__.py
 goldenverba/components/embedding/interface.py
 goldenverba/components/embedding/manager.py
 goldenverba/components/generation/CohereGenerator.py
@@ -98,14 +95,16 @@
 goldenverba/server/frontend/out/_next/static/S-_u12TvmUTLlw1RLiYOf/_ssgManifest.js
 goldenverba/server/frontend/out/_next/static/Uqm0JJ5Jfn42pkmmXyi8G/_buildManifest.js
 goldenverba/server/frontend/out/_next/static/Uqm0JJ5Jfn42pkmmXyi8G/_ssgManifest.js
 goldenverba/server/frontend/out/_next/static/YWcefBRkmSyHlQU9oZZh2/_buildManifest.js
 goldenverba/server/frontend/out/_next/static/YWcefBRkmSyHlQU9oZZh2/_ssgManifest.js
 goldenverba/server/frontend/out/_next/static/YrNhgjW3p56rd3HOLzh1M/_buildManifest.js
 goldenverba/server/frontend/out/_next/static/YrNhgjW3p56rd3HOLzh1M/_ssgManifest.js
+goldenverba/server/frontend/out/_next/static/_A-piGxRm1B_OMIwQ_tPn/_buildManifest.js
+goldenverba/server/frontend/out/_next/static/_A-piGxRm1B_OMIwQ_tPn/_ssgManifest.js
 goldenverba/server/frontend/out/_next/static/a4aifz2A_sNzaC7VcEnF8/_buildManifest.js
 goldenverba/server/frontend/out/_next/static/a4aifz2A_sNzaC7VcEnF8/_ssgManifest.js
 goldenverba/server/frontend/out/_next/static/chunks/172-06f3679cd389db14.js
 goldenverba/server/frontend/out/_next/static/chunks/172-11387f2fea15f8f4.js
 goldenverba/server/frontend/out/_next/static/chunks/172-2aea64d5cb024338.js
 goldenverba/server/frontend/out/_next/static/chunks/172-50c469fb388350d4.js
 goldenverba/server/frontend/out/_next/static/chunks/172-742d06afbbb76b32.js
@@ -168,14 +167,15 @@
 goldenverba/server/frontend/out/_next/static/chunks/pages/_app-8ae9faf463bff6e8.js
 goldenverba/server/frontend/out/_next/static/chunks/pages/_app-905162599335727d.js
 goldenverba/server/frontend/out/_next/static/chunks/pages/_app-93747ea226addaf4.js
 goldenverba/server/frontend/out/_next/static/chunks/pages/_app-95b570e3c384ee1a.js
 goldenverba/server/frontend/out/_next/static/chunks/pages/_app-a0957af8bafb5c75.js
 goldenverba/server/frontend/out/_next/static/chunks/pages/_app-a5604af5bf4aeb92.js
 goldenverba/server/frontend/out/_next/static/chunks/pages/_app-b7fba87b2821fa1b.js
+goldenverba/server/frontend/out/_next/static/chunks/pages/_app-c1589fca75958036.js
 goldenverba/server/frontend/out/_next/static/chunks/pages/_app-d6fe3ed4752599cf.js
 goldenverba/server/frontend/out/_next/static/chunks/pages/_app-f48f66f2530dcab1.js
 goldenverba/server/frontend/out/_next/static/chunks/pages/_error-b190518070b21757.js
 goldenverba/server/frontend/out/_next/static/chunks/pages/about-5eabeb8efb0f0a5d.js
 goldenverba/server/frontend/out/_next/static/chunks/pages/about-772e84e976153ce1.js
 goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-0e4cc95fa680cb1b.js
 goldenverba/server/frontend/out/_next/static/chunks/pages/document_explorer-16e4de29624eb562.js
```

