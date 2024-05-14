# Comparing `tmp/jupyterhub-fancy-profiles-0.2.0.tar.gz` & `tmp/jupyterhub_fancy_profiles-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterhub-fancy-profiles-0.2.0.tar", last modified: Tue Nov 14 10:06:46 2023, max compression
+gzip compressed data, was "jupyterhub_fancy_profiles-0.3.0.tar", last modified: Tue May 14 16:10:36 2024, max compression
```

## Comparing `jupyterhub-fancy-profiles-0.2.0.tar` & `jupyterhub_fancy_profiles-0.3.0.tar`

### file list

```diff
@@ -1,31 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 10:06:46.021006 jupyterhub-fancy-profiles-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2023-11-14 10:06:19.000000 jupyterhub-fancy-profiles-0.2.0/.eslintrc.js
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-11-14 10:06:19.000000 jupyterhub-fancy-profiles-0.2.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 10:06:46.009006 jupyterhub-fancy-profiles-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 10:06:46.013006 jupyterhub-fancy-profiles-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      995 2023-11-14 10:06:19.000000 jupyterhub-fancy-profiles-0.2.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2023-11-14 10:06:19.000000 jupyterhub-fancy-profiles-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-14 10:06:19.000000 jupyterhub-fancy-profiles-0.2.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2023-11-14 10:06:19.000000 jupyterhub-fancy-profiles-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-11-14 10:06:19.000000 jupyterhub-fancy-profiles-0.2.0/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2023-11-14 10:06:19.000000 jupyterhub-fancy-profiles-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      612 2023-11-14 10:06:19.000000 jupyterhub-fancy-profiles-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2023-11-14 10:06:46.021006 jupyterhub-fancy-profiles-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2023-11-14 10:06:19.000000 jupyterhub-fancy-profiles-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 10:06:46.013006 jupyterhub-fancy-profiles-0.2.0/jupyterhub_fancy_profiles/
--rw-r--r--   0 runner    (1001) docker     (127)      753 2023-11-14 10:06:19.000000 jupyterhub-fancy-profiles-0.2.0/jupyterhub_fancy_profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-11-14 10:06:29.000000 jupyterhub-fancy-profiles-0.2.0/jupyterhub_fancy_profiles/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 10:06:46.009006 jupyterhub-fancy-profiles-0.2.0/jupyterhub_fancy_profiles/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 10:06:46.017006 jupyterhub-fancy-profiles-0.2.0/jupyterhub_fancy_profiles/static/dist/
--rw-r--r--   0 runner    (1001) docker     (127)  2064952 2023-11-14 10:06:45.000000 jupyterhub-fancy-profiles-0.2.0/jupyterhub_fancy_profiles/static/dist/form.js
--rw-r--r--   0 runner    (1001) docker     (127)  2285368 2023-11-14 10:06:45.000000 jupyterhub-fancy-profiles-0.2.0/jupyterhub_fancy_profiles/static/dist/form.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 10:06:46.017006 jupyterhub-fancy-profiles-0.2.0/jupyterhub_fancy_profiles/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2023-11-14 10:06:19.000000 jupyterhub-fancy-profiles-0.2.0/jupyterhub_fancy_profiles/templates/form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 10:06:46.013006 jupyterhub-fancy-profiles-0.2.0/jupyterhub_fancy_profiles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2023-11-14 10:06:45.000000 jupyterhub-fancy-profiles-0.2.0/jupyterhub_fancy_profiles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-11-14 10:06:46.000000 jupyterhub-fancy-profiles-0.2.0/jupyterhub_fancy_profiles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-14 10:06:45.000000 jupyterhub-fancy-profiles-0.2.0/jupyterhub_fancy_profiles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-11-14 10:06:45.000000 jupyterhub-fancy-profiles-0.2.0/jupyterhub_fancy_profiles.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      661 2023-11-14 10:06:19.000000 jupyterhub-fancy-profiles-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 10:06:46.021006 jupyterhub-fancy-profiles-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      891 2023-11-14 10:06:19.000000 jupyterhub-fancy-profiles-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:10:36.017636 jupyterhub_fancy_profiles-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/.eslintrc.js
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:10:36.005636 jupyterhub_fancy_profiles-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:10:36.013636 jupyterhub_fancy_profiles-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/.github/workflows/checks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/.github/workflows/docker-build.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-05-14 16:10:36.017636 jupyterhub_fancy_profiles-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/babel.config.js
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/binderhub_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/jupyterhub_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:10:36.013636 jupyterhub_fancy_profiles-0.3.0/jupyterhub_fancy_profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/jupyterhub_fancy_profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 16:10:20.000000 jupyterhub_fancy_profiles-0.3.0/jupyterhub_fancy_profiles/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:10:36.013636 jupyterhub_fancy_profiles-0.3.0/jupyterhub_fancy_profiles/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/jupyterhub_fancy_profiles/templates/form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:10:36.017636 jupyterhub_fancy_profiles-0.3.0/jupyterhub_fancy_profiles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-05-14 16:10:35.000000 jupyterhub_fancy_profiles-0.3.0/jupyterhub_fancy_profiles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-14 16:10:36.000000 jupyterhub_fancy_profiles-0.3.0/jupyterhub_fancy_profiles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:10:35.000000 jupyterhub_fancy_profiles-0.3.0/jupyterhub_fancy_profiles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 16:10:35.000000 jupyterhub_fancy_profiles-0.3.0/jupyterhub_fancy_profiles.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   925273 2024-05-14 16:10:32.000000 jupyterhub_fancy_profiles-0.3.0/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    67598 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 16:10:36.017636 jupyterhub_fancy_profiles-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/setupTests.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:10:36.013636 jupyterhub_fancy_profiles-0.3.0/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/src/ImageBuilder.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/src/ProfileForm.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/src/ProfileForm.test.js
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/src/ProfileOptions.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/src/ResourceSelect.jsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:10:36.005636 jupyterhub_fancy_profiles-0.3.0/src/components/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:10:36.017636 jupyterhub_fancy_profiles-0.3.0/src/components/form/
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/src/components/form/CustomSelect.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/src/components/form/fields.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/src/components/form/fields.test.js
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/src/components/form/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/src/form.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:10:36.017636 jupyterhub_fancy_profiles-0.3.0/src/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/src/hooks/useSelectOptions.js
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/src/index.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/src/state.js
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-14 16:10:15.000000 jupyterhub_fancy_profiles-0.3.0/webpack.config.js
```

### Comparing `jupyterhub-fancy-profiles-0.2.0/.eslintrc.js` & `jupyterhub_fancy_profiles-0.3.0/.eslintrc.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -26,9 +26,15 @@
         "no-unused-vars": ["error", {
             args: "after-used"
         }],
     },
     ignorePatterns: [
         "jupyterhub_fancy_profiles/static/*.js",
         "webpack.config.js",
+        "babel.config.js",
     ],
+    settings: {
+        react: {
+            version: "detect",
+        },
+    },
 };
```

### Comparing `jupyterhub-fancy-profiles-0.2.0/.github/workflows/release.yaml` & `jupyterhub_fancy_profiles-0.3.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `jupyterhub-fancy-profiles-0.2.0/.gitignore` & `jupyterhub_fancy_profiles-0.3.0/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -160,7 +160,16 @@
 #.idea/
 
 # JS is everywhere
 node_modules/
 
 # Built files should not be in the package
 static/dist/
+
+#Jupytherhub configs
+bin
+jupyterhub_fancy_profiles
+share
+jupyterhub_cookie_secret
+jupyterhub-proxy.pid
+jupyterhub.sqlite
+pyvenv.cfg
```

### Comparing `jupyterhub-fancy-profiles-0.2.0/.pre-commit-config.yaml` & `jupyterhub_fancy_profiles-0.3.0/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -7,63 +7,68 @@
 #
 # - Run on all files:   pre-commit run --all-files
 # - Register git hooks: pre-commit install --install-hooks
 #
 repos:
   # Autoformat: Python code, syntax patterns are modernized
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.10.1
+    rev: v3.15.2
     hooks:
       - id: pyupgrade
         args:
           - --py38-plus
 
   # Autoformat: Python code
   - repo: https://github.com/psf/black
-    rev: 23.7.0
+    rev: 24.3.0
     hooks:
       - id: black
         # args are not passed, but see the config in pyproject.toml
 
   # Autoformat: Python code
   - repo: https://github.com/pycqa/isort
-    rev: 5.12.0
+    rev: 5.13.2
     hooks:
       - id: isort
         # args are not passed, but see the config in pyproject.toml
 
   # Autoformat: js, html, markdown, yaml, json
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v3.0.3
+    rev: v4.0.0-alpha.8
     hooks:
       - id: prettier
         exclude: jupyterhub_fancy_profiles/static
 
   # Misc autoformatting and linting
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.5.0
     hooks:
       - id: end-of-file-fixer
         exclude_types: [svg]
         exclude: jupyterhub_fancy_profiles/static
       - id: check-case-conflict
       - id: check-executables-have-shebangs
       - id: requirements-txt-fixer
 
   # Lint: Python code
   - repo: https://github.com/PyCQA/flake8
-    rev: "6.1.0"
+    rev: "7.0.0"
     hooks:
       - id: flake8
 
   # Lint: JS code
   - repo: https://github.com/pre-commit/mirrors-eslint
-    rev: "v8.53.0" # Use the sha / tag you want to point at
+    rev: "v8.56.0" # Use the sha / tag you want to point at
     hooks:
       - id: eslint
         files: \.jsx?$
         types: [file]
         exclude: jupyterhub_fancy_profiles/static
+        additional_dependencies:
+          # Duplicated from package.json's devDependencies, otherwise pre-commit.ci
+          # does not like it
+          - eslint@8.56.0
+          - eslint-plugin-react
 
 # pre-commit.ci config reference: https://pre-commit.ci/#configuration
 ci:
   autoupdate_schedule: monthly
```

### Comparing `jupyterhub-fancy-profiles-0.2.0/LICENSE` & `jupyterhub_fancy_profiles-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterhub-fancy-profiles-0.2.0/README.md` & `jupyterhub_fancy_profiles-0.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: jupyterhub-fancy-profiles
+Version: 0.3.0
+Summary: Fancy Profile UI for jupyterhub-kubespawner
+Author-email: Yuvi <yuvipanda@gmail.com>
+Keywords: jupyterhub
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # `jupyterhub-fancy-profiles`
 
 A react based, fancy implementation of user selectable profiles
 for use with [jupyterhub-kubespawner](https://github.com/jupyterhub/kubespawner).
 
 ![Screenshot showing an image selector](screenshot.png)
 
@@ -20,15 +32,45 @@
 1. While multiple `profile_options` are supported, only a single `profile` is
    supported.
 
 2. The forms values don't remember their previous state upon refresh
 
 ## How to use
 
-Once installed, you can have kubespawner use the templates shipped
+### Using with z2jh
+
+This package can be used with any installation of KubeSpawner, but is most
+commonly used with an installation of z2jh. It requires installing `jupyterhub-fancy-profiles`
+in the `hub` image used by z2jh.
+
+As a convenience, we build and push docker images that can be automatically
+used with z2jh!
+
+1. Look at the [list of available tags](https://quay.io/repository/yuvipanda/z2jh-hub-with-fancy-profiles?tab=tags)
+   and find a tag that matches the version of z2jh you are using.
+
+2. Use this image in the z2jh config. In the `values.yaml` file you pass to
+   `helm`, use the following:
+
+   ```yaml
+   hub:
+     image:
+       name: quay.io/yuvipanda/z2jh-hub-with-fancy-profiles
+       tag: <tag-from-the-list>
+     extraConfig:
+       01-enable-fancy-profiles: |
+         from jupyterhub_fancy_profiles import setup_ui
+         setup_ui(c)
+   ```
+
+3. Run a `helm upgrade` and you should have fancy profiles enabled!
+
+### Using directly with KubeSpawner
+
+After the package is installed, you can have kubespawner use the templates shipped
 with this package to provide appropriate UI, by adding the following snippet
 to your `jupyterhub_config.py` file:
 
 ```python
 from jupyterhub_fancy_profiles import setup_ui
 setup_ui(c)
 ```
@@ -62,7 +104,13 @@
 time to start using a framework. Lesson learnt from that is we should use a
 _very lightweight_ framework right from the start, something mainstream that
 can attract frontend devs without being so fancy that nobody else can work on
 it. Given the size and complexity of this - a complex UI but only a single page -
 plain react without typescript seems the correct choice. We will _not_ make
 this into a super-heavy, complex application - just a fairly simple one that
 uses react.
+
+## Funding
+
+Funded in part by [GESIS](http://notebooks.gesis.org) in cooperation with
+NFDI4DS [460234259](https://gepris.dfg.de/gepris/projekt/460234259?context=projekt&task=showDetail&id=460234259&)
+and [CESSDA](https://www.cessda.eu).
```

### Comparing `jupyterhub-fancy-profiles-0.2.0/jupyterhub_fancy_profiles/__init__.py` & `jupyterhub_fancy_profiles-0.3.0/jupyterhub_fancy_profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-fancy-profiles-0.2.0/pyproject.toml` & `jupyterhub_fancy_profiles-0.3.0/pyproject.toml`

 * *Files identical despite different names*

