# Comparing `tmp/modflow-devtools-1.4.0.tar.gz` & `tmp/modflow_devtools-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modflow-devtools-1.4.0.tar", last modified: Mon Feb 19 16:19:08 2024, max compression
+gzip compressed data, was "modflow_devtools-1.5.0.tar", last modified: Wed May 15 17:57:28 2024, max compression
```

## Comparing `modflow-devtools-1.4.0.tar` & `modflow_devtools-1.5.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:19:08.282908 modflow-devtools-1.4.0/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1627 2024-02-19 16:18:51.000000 modflow-devtools-1.4.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-02-19 16:18:51.000000 modflow-devtools-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-02-19 16:19:08.282908 modflow-devtools-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-02-19 16:18:51.000000 modflow-devtools-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:19:08.278908 modflow-devtools-1.4.0/modflow_devtools/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-19 16:18:51.000000 modflow-devtools-1.4.0/modflow_devtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-02-19 16:18:51.000000 modflow-devtools-1.4.0/modflow_devtools/build.py
--rw-r--r--   0 runner    (1001) docker     (127)    17652 2024-02-19 16:18:51.000000 modflow-devtools-1.4.0/modflow_devtools/download.py
--rw-r--r--   0 runner    (1001) docker     (127)    12945 2024-02-19 16:18:51.000000 modflow-devtools-1.4.0/modflow_devtools/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-02-19 16:18:51.000000 modflow-devtools-1.4.0/modflow_devtools/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-02-19 16:18:51.000000 modflow-devtools-1.4.0/modflow_devtools/latex.py
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-02-19 16:18:51.000000 modflow-devtools-1.4.0/modflow_devtools/markers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14278 2024-02-19 16:18:51.000000 modflow-devtools-1.4.0/modflow_devtools/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-02-19 16:18:51.000000 modflow-devtools-1.4.0/modflow_devtools/ostags.py
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-02-19 16:18:51.000000 modflow-devtools-1.4.0/modflow_devtools/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:19:08.278908 modflow-devtools-1.4.0/modflow_devtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-02-19 16:19:08.000000 modflow-devtools-1.4.0/modflow_devtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-02-19 16:19:08.000000 modflow-devtools-1.4.0/modflow_devtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 16:19:08.000000 modflow-devtools-1.4.0/modflow_devtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 16:19:01.000000 modflow-devtools-1.4.0/modflow_devtools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-02-19 16:19:08.000000 modflow-devtools-1.4.0/modflow_devtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-19 16:19:08.000000 modflow-devtools-1.4.0/modflow_devtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-02-19 16:18:51.000000 modflow-devtools-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 16:19:08.282908 modflow-devtools-1.4.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       61 2024-02-19 16:18:51.000000 modflow-devtools-1.4.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-19 16:18:51.000000 modflow-devtools-1.4.0/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:57:28.781448 modflow_devtools-1.5.0/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1627 2024-05-15 17:57:14.000000 modflow_devtools-1.5.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-15 17:57:14.000000 modflow_devtools-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-05-15 17:57:28.781448 modflow_devtools-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-05-15 17:57:14.000000 modflow_devtools-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:57:28.777448 modflow_devtools-1.5.0/modflow_devtools/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-15 17:57:14.000000 modflow_devtools-1.5.0/modflow_devtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-15 17:57:14.000000 modflow_devtools-1.5.0/modflow_devtools/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17465 2024-05-15 17:57:14.000000 modflow_devtools-1.5.0/modflow_devtools/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12376 2024-05-15 17:57:14.000000 modflow_devtools-1.5.0/modflow_devtools/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-05-15 17:57:14.000000 modflow_devtools-1.5.0/modflow_devtools/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-15 17:57:14.000000 modflow_devtools-1.5.0/modflow_devtools/latex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-15 17:57:14.000000 modflow_devtools-1.5.0/modflow_devtools/markers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15187 2024-05-15 17:57:14.000000 modflow_devtools-1.5.0/modflow_devtools/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-05-15 17:57:14.000000 modflow_devtools-1.5.0/modflow_devtools/ostags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-15 17:57:14.000000 modflow_devtools-1.5.0/modflow_devtools/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-05-15 17:57:14.000000 modflow_devtools-1.5.0/modflow_devtools/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:57:28.781448 modflow_devtools-1.5.0/modflow_devtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-05-15 17:57:28.000000 modflow_devtools-1.5.0/modflow_devtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-15 17:57:28.000000 modflow_devtools-1.5.0/modflow_devtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 17:57:28.000000 modflow_devtools-1.5.0/modflow_devtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 17:57:24.000000 modflow_devtools-1.5.0/modflow_devtools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-15 17:57:28.000000 modflow_devtools-1.5.0/modflow_devtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-15 17:57:28.000000 modflow_devtools-1.5.0/modflow_devtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-15 17:57:14.000000 modflow_devtools-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 17:57:28.781448 modflow_devtools-1.5.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       61 2024-05-15 17:57:14.000000 modflow_devtools-1.5.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 17:57:14.000000 modflow_devtools-1.5.0/version.txt
```

### Comparing `modflow-devtools-1.4.0/LICENSE.md` & `modflow_devtools-1.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `modflow-devtools-1.4.0/PKG-INFO` & `modflow_devtools-1.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modflow-devtools
-Version: 1.4.0
+Version: 1.5.0
 Summary: Python tools for MODFLOW development
 Author-email: "Joseph D. Hughes" <modflow@usgs.gov>, Michael Reno <mreno@ucar.edu>, Mike Taves <mwtoews@gmail.com>, Wes Bonelli <wbonelli@ucar.edu>
 Maintainer-email: "Joseph D. Hughes" <modflow@usgs.gov>
 License: CC0
 Project-URL: Documentation, https://modflow-devtools.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/MODFLOW-USGS/modflow-devtools/issues
 Project-URL: Source Code, https://github.com/MODFLOW-USGS/modflow-devtools
@@ -20,32 +20,30 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Provides-Extra: lint
-Requires-Dist: black; extra == "lint"
-Requires-Dist: cffconvert; extra == "lint"
-Requires-Dist: flake8; extra == "lint"
-Requires-Dist: isort; extra == "lint"
-Requires-Dist: pylint; extra == "lint"
+Requires-Dist: ruff; extra == "lint"
 Provides-Extra: test
 Requires-Dist: modflow-devtools[lint]; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: flaky; extra == "test"
 Requires-Dist: filelock; extra == "test"
 Requires-Dist: meson!=0.63.0; extra == "test"
 Requires-Dist: ninja; extra == "test"
 Requires-Dist: numpy; extra == "test"
-Requires-Dist: pytest; extra == "test"
+Requires-Dist: pandas; extra == "test"
+Requires-Dist: pytest!=8.1.0; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-dotenv; extra == "test"
 Requires-Dist: pytest-xdist; extra == "test"
 Requires-Dist: PyYaml; extra == "test"
+Requires-Dist: syrupy; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 
 # MODFLOW developer tools
 
@@ -101,32 +99,33 @@
 
 ## Requirements
 
 Python3.8+, dependency-free, but pairs well with `pytest` and select plugins, e.g.
 
 - [`pytest-dotenv`](https://github.com/quiqua/pytest-dotenv)
 - [`pytest-xdist`](https://github.com/pytest-dev/pytest-xdist)
+- [`syrupy`](https://github.com/tophat/syrupy)
 
 ## Installation
 
 `modflow-devtools` is available on PyPI and can be installed with pip:
 
 ```shell
 pip install modflow-devtools
 ```
 
-Pytest, pytest plugins, and other optional dependencies can be installed with:
+Pytest, pytest plugins, and other testing-related dependencies can be installed with:
 
 ```shell
 pip install "modflow-devtools[test]"
 ```
 
 To install from source and set up a development environment please see the [developer documentation](DEVELOPER.md).
 
-To import `pytest` fixtures in a project consuming `modflow-devtools`, add the following to a `conftest.py` file:
+To import `pytest` fixtures in a project consuming `modflow-devtools`, add the following to a test file or `conftest.py` file:
 
 ```python
 pytest_plugins = [ "modflow_devtools.fixtures" ]
 ```
 
 **Note**: this must be a top-level `conftest.py`, which nested `conftest.py` files may then override or extend.
```

### Comparing `modflow-devtools-1.4.0/README.md` & `modflow_devtools-1.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -52,32 +52,33 @@
 
 ## Requirements
 
 Python3.8+, dependency-free, but pairs well with `pytest` and select plugins, e.g.
 
 - [`pytest-dotenv`](https://github.com/quiqua/pytest-dotenv)
 - [`pytest-xdist`](https://github.com/pytest-dev/pytest-xdist)
+- [`syrupy`](https://github.com/tophat/syrupy)
 
 ## Installation
 
 `modflow-devtools` is available on PyPI and can be installed with pip:
 
 ```shell
 pip install modflow-devtools
 ```
 
-Pytest, pytest plugins, and other optional dependencies can be installed with:
+Pytest, pytest plugins, and other testing-related dependencies can be installed with:
 
 ```shell
 pip install "modflow-devtools[test]"
 ```
 
 To install from source and set up a development environment please see the [developer documentation](DEVELOPER.md).
 
-To import `pytest` fixtures in a project consuming `modflow-devtools`, add the following to a `conftest.py` file:
+To import `pytest` fixtures in a project consuming `modflow-devtools`, add the following to a test file or `conftest.py` file:
 
 ```python
 pytest_plugins = [ "modflow_devtools.fixtures" ]
 ```
 
 **Note**: this must be a top-level `conftest.py`, which nested `conftest.py` files may then override or extend.
```

### Comparing `modflow-devtools-1.4.0/modflow_devtools/build.py` & `modflow_devtools-1.5.0/modflow_devtools/build.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-1.4.0/modflow_devtools/download.py` & `modflow_devtools-1.5.0/modflow_devtools/download.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,18 +54,18 @@
     retries : int
         The maximum number of retries for each request
     verbose : bool
         Whether to suppress verbose output
     """
 
     if "/" not in repo:
-        raise ValueError(f"repo format must be owner/name")
+        raise ValueError("repo format must be owner/name")
 
     if not isinstance(retries, int) or retries < 1:
-        raise ValueError(f"retries must be a positive int")
+        raise ValueError("retries must be a positive int")
 
     params = {}
     if per_page is not None:
         if per_page < 1 or per_page > 100:
             raise ValueError("per_page must be between 1 and 100")
         params["per_page"] = per_page
 
@@ -77,32 +77,33 @@
         params["page"] = page
         request = get_request(req_url, params=params)
         while True:
             tries += 1
             try:
                 if verbose:
                     print(
-                        f"Fetching releases for repo {repo} (page {page}, {per_page} per page)"
+                        f"Fetching releases for "
+                        f"repo {repo} "
+                        f"(page {page}, "
+                        f"{per_page} per page)"
                     )
                 with urllib.request.urlopen(request, timeout=10) as resp:
                     return json.loads(resp.read().decode())
             except urllib.error.HTTPError as err:
                 if err.code == 401 and os.environ.get("GITHUB_TOKEN"):
                     raise ValueError("GITHUB_TOKEN is invalid") from err
                 elif err.code == 403 and "rate limit exceeded" in err.reason:
                     raise ValueError(
                         f"use GITHUB_TOKEN env to bypass rate limit ({err})"
                     ) from err
                 elif err.code in (404, 503) and tries < retries:
                     # GitHub sometimes returns this error for valid URLs, so retry
                     warn(f"URL request try {tries} failed ({err})")
                     continue
-                raise RuntimeError(
-                    f"cannot retrieve data from {req_url}"
-                ) from err
+                raise RuntimeError(f"cannot retrieve data from {req_url}") from err
 
     releases = []
     max_pages = max_pages if max_pages else sys.maxsize
     while page <= max_pages:
         rels = get_response_json()
         page += 1
         releases.extend(rels)
@@ -128,21 +129,21 @@
     retries : int
         The maximum number of retries for each request
     verbose : bool
         Whether to suppress verbose output
     """
 
     if "/" not in repo:
-        raise ValueError(f"repo format must be owner/name")
+        raise ValueError("repo format must be owner/name")
 
     if not isinstance(tag, str) or not any(tag):
-        raise ValueError(f"tag must be a non-empty string")
+        raise ValueError("tag must be a non-empty string")
 
     if not isinstance(retries, int) or retries < 1:
-        raise ValueError(f"retries must be a positive int")
+        raise ValueError("retries must be a positive int")
 
     req_url = f"https://api.github.com/repos/{repo}"
     req_url = (
         f"{req_url}/releases/latest"
         if tag == "latest"
         else f"{req_url}/releases/tags/{tag}"
     )
@@ -205,18 +206,18 @@
 
     Returns
     -------
         The latest release tag name (a string).
     """
 
     if "/" not in repo:
-        raise ValueError(f"repo format must be owner/name")
+        raise ValueError("repo format must be owner/name")
 
     if not isinstance(retries, int) or retries < 1:
-        raise ValueError(f"retries must be a positive int")
+        raise ValueError("retries must be a positive int")
 
     release = get_release(repo, retries=retries, verbose=verbose)
     return release["tag_name"]
 
 
 def get_release_assets(
     repo, tag="latest", simple=False, retries=3, verbose=False
@@ -241,21 +242,21 @@
     Returns
     -------
         A list of dicts if simple is False, one per release asset.
         If simple is True, a dict mapping asset names to download URLs.
     """
 
     if "/" not in repo:
-        raise ValueError(f"repo format must be owner/name")
+        raise ValueError("repo format must be owner/name")
 
     if not isinstance(tag, str) or not any(tag):
-        raise ValueError(f"tag must be a non-empty string")
+        raise ValueError("tag must be a non-empty string")
 
     if not isinstance(retries, int) or retries < 1:
-        raise ValueError(f"retries must be a positive int")
+        raise ValueError("retries must be a positive int")
 
     release = get_release(repo, tag=tag, retries=retries, verbose=verbose)
     return (
         {a["name"]: a["browser_download_url"] for a in release["assets"]}
         if simple
         else release["assets"]
     )
@@ -283,34 +284,32 @@
     retries : int
         The maximum number of retries for each request
     verbose : bool
         Whether to show verbose output
 
     Returns
     -------
-        A list of dictionaries, each containing information about an artifact as returned
-        by the GitHub API.
+        A list of dictionaries, each containing information
+        about an artifact as returned by the GitHub API.
     """
 
     if "/" not in repo:
-        raise ValueError(f"repo format must be owner/name")
+        raise ValueError("repo format must be owner/name")
 
     if not isinstance(retries, int) or retries < 1:
-        raise ValueError(f"retries must be a positive int")
+        raise ValueError("retries must be a positive int")
 
-    msg = f"artifact(s) for {repo}" + (
-        f" matching name {name}" if name else ""
-    )
+    msg = f"artifact(s) for {repo}" + (f" matching name {name}" if name else "")
     req_url = f"https://api.github.com/repos/{repo}/actions/artifacts"
     page = 1
     params = {}
 
     if name is not None:
         if not isinstance(name, str) or len(name) == 0:
-            raise ValueError(f"name must be a non-empty string")
+            raise ValueError("name must be a non-empty string")
         params["name"] = name
 
     if per_page is not None:
         if per_page < 1 or per_page > 100:
             raise ValueError("per_page must be between 1 and 100")
         params["per_page"] = int(per_page)
 
@@ -332,17 +331,15 @@
                     raise ValueError(
                         f"use GITHUB_TOKEN env to bypass rate limit ({err})"
                     ) from err
                 elif err.code in (404, 503) and tries < retries:
                     # GitHub sometimes returns this error for valid URLs, so retry
                     warn(f"URL request try {tries} failed ({err})")
                     continue
-                raise RuntimeError(
-                    f"cannot retrieve data from {req_url}"
-                ) from err
+                raise RuntimeError(f"cannot retrieve data from {req_url}") from err
 
     artifacts = []
     diff = 1
     max_pages = max_pages if max_pages else sys.maxsize
     while diff > 0 and page <= max_pages:
         result = get_response_json()
         total = result["total_count"]
@@ -383,18 +380,18 @@
     retries : int
         The maximum number of retries for each request
     verbose : bool
         Whether to show verbose output
     """
 
     if "/" not in repo:
-        raise ValueError(f"repo format must be owner/name")
+        raise ValueError("repo format must be owner/name")
 
     if not isinstance(retries, int) or retries < 1:
-        raise ValueError(f"retries must be a positive int")
+        raise ValueError("retries must be a positive int")
 
     req_url = f"https://api.github.com/repos/{repo}/actions/artifacts/{id}/zip"
     request = urllib.request.Request(req_url)
     if "github.com" in req_url:
         github_token = os.environ.get("GITHUB_TOKEN", None)
         if github_token:
             request.add_header("Authorization", f"Bearer {github_token}")
@@ -411,17 +408,15 @@
                 out_file.write(content)
                 break
         except urllib.error.HTTPError as err:
             if tries < retries:
                 warn(f"URL request try {tries} failed ({err})")
                 continue
             else:
-                raise RuntimeError(
-                    f"cannot retrieve data from {req_url}"
-                ) from err
+                raise RuntimeError(f"cannot retrieve data from {req_url}") from err
 
     if verbose:
         print(f"Uncompressing: {zip_path}")
 
     z = MFZipFile(zip_path)
     z.extractall(str(path))
     z.close()
@@ -492,22 +487,16 @@
                 tag = "Content-length"
                 if verbose and tag in url_file.headers:
                     file_size = url_file.headers[tag]
                     len_file_size = len(file_size)
                     file_size = int(file_size)
 
                     bfmt = "{:" + f"{len_file_size}" + ",d}"
-                    sbfmt = (
-                        "{:>"
-                        + f"{len(bfmt.format(int(file_size)))}"
-                        + "s} bytes"
-                    )
-                    print(
-                        f"   file size: {sbfmt.format(bfmt.format(int(file_size)))}"
-                    )
+                    sbfmt = "{:>" + f"{len(bfmt.format(int(file_size)))}" + "s} bytes"
+                    print(f"   file size: {sbfmt.format(bfmt.format(int(file_size)))}")
 
                 break
         except urllib.error.HTTPError as err:
             if tries < retries:
                 warn(f"URL request try {tries} failed ({err})")
                 continue
 
@@ -522,15 +511,15 @@
         z = MFZipFile(file_path)
         try:
             if verbose:
                 print(f"Uncompressing: {file_path}")
 
             # extract the files
             z.extractall(str(path))
-        except:
+        except:  # noqa: E722
             p = "Could not unzip the file. Stopping."
             raise Exception(p)
         z.close()
 
         # delete the zipfile
         if delete_zip:
             if verbose:
```

### Comparing `modflow-devtools-1.4.0/modflow_devtools/fixtures.py` & `modflow_devtools-1.5.0/modflow_devtools/fixtures.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,26 @@
-import random
 from collections import OrderedDict
 from itertools import groupby
 from os import PathLike, environ
 from pathlib import Path
 from shutil import copytree, rmtree
-from typing import Dict, List, Optional
+from typing import Dict, Generator, List, Optional
 
 from modflow_devtools.imports import import_optional_dependency
 from modflow_devtools.misc import get_namefile_paths, get_packages
 
 pytest = import_optional_dependency("pytest")
 
 
 # fixtures
 
 
 @pytest.fixture(scope="function")
-def function_tmpdir(tmpdir_factory, request) -> Path:
-    node = (
-        request.node.name.replace("/", "_")
-        .replace("\\", "_")
-        .replace(":", "_")
-    )
+def function_tmpdir(tmpdir_factory, request) -> Generator[Path, None, None]:
+    node = request.node.name.replace("/", "_").replace("\\", "_").replace(":", "_")
     temp = Path(tmpdir_factory.mktemp(node))
     yield Path(temp)
 
     keep = request.config.option.KEEP
     if keep:
         path = Path(keep) / temp.name
         if path.is_dir():
@@ -37,15 +32,15 @@
         path = Path(keep_failed) / temp.name
         if path.is_dir():
             rmtree(path)
         copytree(temp, path)
 
 
 @pytest.fixture(scope="class")
-def class_tmpdir(tmpdir_factory, request) -> Path:
+def class_tmpdir(tmpdir_factory, request) -> Generator[Path, None, None]:
     assert (
         request.cls is not None
     ), "Class-scoped temp dir fixture must be used on class"
     temp = Path(tmpdir_factory.mktemp(request.cls.__name__))
     yield temp
 
     keep = request.config.option.KEEP
@@ -53,28 +48,28 @@
         path = Path(keep) / temp.name
         if path.is_dir():
             rmtree(path)
         copytree(temp, path)
 
 
 @pytest.fixture(scope="module")
-def module_tmpdir(tmpdir_factory, request) -> Path:
+def module_tmpdir(tmpdir_factory, request) -> Generator[Path, None, None]:
     temp = Path(tmpdir_factory.mktemp(request.module.__name__))
     yield temp
 
     keep = request.config.option.KEEP
     if keep:
         path = Path(keep) / temp.name
         if path.is_dir():
             rmtree(path)
         copytree(temp, path)
 
 
 @pytest.fixture(scope="session")
-def session_tmpdir(tmpdir_factory, request) -> Path:
+def session_tmpdir(tmpdir_factory, request) -> Generator[Path, None, None]:
     temp = Path(tmpdir_factory.mktemp(request.config.rootpath.name))
     yield temp
 
     keep = request.config.option.KEEP
     if keep:
         path = Path(keep) / temp.name
         if path.is_dir():
@@ -85,28 +80,15 @@
 @pytest.fixture
 def repos_path() -> Optional[Path]:
     """Path to directory containing test model and example repositories"""
     return environ.get("REPOS_PATH", None)
 
 
 @pytest.fixture
-def use_pandas(request):
-    pandas = request.config.option.PANDAS
-    if pandas == "yes":
-        return True
-    elif pandas == "no":
-        return False
-    elif pandas == "random":
-        return random.randint(0, 1) == 0
-    else:
-        raise ValueError(f"Unsupported value for --pandas: {pandas}")
-
-
-@pytest.fixture
-def tabular(request):
+def tabular(request) -> str:
     tab = request.config.option.TABULAR
     if tab not in ["raw", "recarray", "dataframe"]:
         raise ValueError(f"Unsupported value for --tabular: {tab}")
     return tab
 
 
 # configuration hooks
@@ -115,27 +97,33 @@
 def pytest_addoption(parser):
     parser.addoption(
         "-K",
         "--keep",
         action="store",
         default=None,
         dest="KEEP",
-        help="Move the contents of temporary test directories to correspondingly named subdirectories at the given "
-        "location after tests complete. This option can be used to exclude test results from automatic cleanup, "
-        "e.g. for manual inspection. The provided path is created if it does not already exist. An error is "
+        help="Move the contents of temporary test directories to "
+        "correspondingly named subdirectories at the given "
+        "location after tests complete. This option can be used "
+        "to exclude test results from automatic cleanup, "
+        "e.g. for manual inspection. The provided path is "
+        "created if it does not already exist. An error is "
         "thrown if any matching files already exist.",
     )
 
     parser.addoption(
         "--keep-failed",
         action="store",
         default=None,
-        help="Move the contents of temporary test directories to correspondingly named subdirectories at the given "
-        "location if the test case fails. This option automatically saves the outputs of failed tests in the "
-        "given location. The path is created if it doesn't already exist. An error is thrown if files with the "
+        help="Move the contents of temporary test directories to "
+        "correspondingly named subdirectories at the given "
+        "location if the test case fails. This option saves "
+        "the outputs of failed tests in the "
+        "given location. The path is created if it doesn't "
+        "already exist. An error is thrown if files with the "
         "same names already exist in the given location.",
     )
 
     parser.addoption(
         "-S",
         "--smoke",
         action="store_true",
@@ -144,15 +132,16 @@
     )
 
     parser.addoption(
         "-M",
         "--meta",
         action="store",
         metavar="NAME",
-        help="Indicates a test should only be run by other tests (e.g., to test framework or fixtures).",
+        help="Indicates a test should only be run by other tests (e.g., "
+        "to test framework or fixtures).",
     )
 
     parser.addoption(
         "--model",
         action="append",
         type=str,
         help="Select a subset of models to run.",
@@ -162,29 +151,21 @@
         "--package",
         action="append",
         type=str,
         help="Select a subset of packages to run.",
     )
 
     parser.addoption(
-        "-P",
-        "--pandas",
-        action="store",
-        default="yes",
-        dest="PANDAS",
-        help="Indicates whether to use pandas, where multiple approaches are available. Select 'yes', 'no', or 'random'.",
-    )
-
-    parser.addoption(
         "-T",
         "--tabular",
         action="store",
         default="raw",
         dest="TABULAR",
-        help="Configure tabular data representation for model input. Select 'raw', 'recarray', or 'dataframe'.",
+        help="Configure tabular data representation for model input. "
+        "Select 'raw', 'recarray', or 'dataframe'.",
     )
 
 
 def pytest_configure(config):
     config.addinivalue_line(
         "markers",
         "meta(name): run only by other tests",
@@ -265,17 +246,15 @@
                 excluded=[],
                 selected=models_selected,
                 packages=packages_selected,
             )
             if repo_path
             else []
         )
-        metafunc.parametrize(
-            key, namefile_paths, ids=[str(m) for m in namefile_paths]
-        )
+        metafunc.parametrize(key, namefile_paths, ids=[str(m) for m in namefile_paths])
 
     key = "test_model_mf5to6"
     if key in metafunc.fixturenames:
         repo_path = get_repo_path("modflow6-testmodels")
         namefile_paths = (
             get_namefile_paths(
                 repo_path / "mf5to6",
@@ -284,17 +263,15 @@
                 excluded=[],
                 selected=models_selected,
                 packages=packages_selected,
             )
             if repo_path
             else []
         )
-        metafunc.parametrize(
-            key, namefile_paths, ids=[str(m) for m in namefile_paths]
-        )
+        metafunc.parametrize(key, namefile_paths, ids=[str(m) for m in namefile_paths])
 
     key = "large_test_model"
     if key in metafunc.fixturenames:
         repo_path = get_repo_path("modflow6-largetestmodels")
         namefile_paths = (
             get_namefile_paths(
                 repo_path,
@@ -303,17 +280,15 @@
                 excluded=[],
                 selected=models_selected,
                 packages=packages_selected,
             )
             if repo_path
             else []
         )
-        metafunc.parametrize(
-            key, namefile_paths, ids=[str(m) for m in namefile_paths]
-        )
+        metafunc.parametrize(key, namefile_paths, ids=[str(m) for m in namefile_paths])
 
     key = "example_scenario"
     if key in metafunc.fixturenames:
         repo_path = get_repo_path("modflow6-examples")
 
         def is_nested(namfile_path: PathLike) -> bool:
             p = Path(namfile_path)
@@ -380,17 +355,15 @@
                     if len(ftypes) > 0:
                         ftypes = [item.upper() for item in ftypes]
                         for pkg in packages_selected:
                             if pkg in ftypes:
                                 filtered.append(name)
                                 break
                 examples = {
-                    name: nfps
-                    for name, nfps in examples.items()
-                    if name in filtered
+                    name: nfps for name, nfps in examples.items() if name in filtered
                 }
 
             # exclude mf6gwf and mf6gwt subdirs
             examples = {
                 name: nfps
                 for name, nfps in examples.items()
                 if name not in ["mf6gwf", "mf6gwt"]
@@ -398,9 +371,9 @@
 
             return examples
 
         example_scenarios = get_examples() if repo_path else dict()
         metafunc.parametrize(
             key,
             [(name, nfps) for name, nfps in example_scenarios.items()],
-            ids=[name for name, ex in example_scenarios.items()],
+            ids=list(example_scenarios.keys()),
         )
```

### Comparing `modflow-devtools-1.4.0/modflow_devtools/imports.py` & `modflow_devtools-1.5.0/modflow_devtools/imports.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Adapted from https://github.com/pandas-dev/pandas/blob/master/pandas/compat/_optional.py
 
 # This file is dual licensed under the terms of the BSD 3-Clause License.
 # BSD 3-Clause License
 #
-# Copyright (c) 2008-2011, AQR Capital Management, LLC, Lambda Foundry, Inc. and PyData Development Team
+# Copyright (c) 2008-2011, AQR Capital Management, LLC, Lambda Foundry, Inc. and PyData Development Team  # noqa: E501
 # All rights reserved.
 #
 # Copyright (c) 2011-2021, Open source contributors.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
@@ -126,17 +126,15 @@
     # Handle submodules: if we have submodule, grab parent module from sys.modules
     parent = name.split(".")[0]
     if parent != name:
         install_name = parent
         module_to_get = sys.modules[install_name]
     else:
         module_to_get = module
-    minimum_version = (
-        min_version if min_version is not None else VERSIONS.get(parent)
-    )
+    minimum_version = min_version if min_version is not None else VERSIONS.get(parent)
     if minimum_version:
         version = get_version(module_to_get)
         if Version(version) < Version(minimum_version):
             msg = (
                 f"Version '{minimum_version}' "
                 f"or newer of '{parent}' required"
                 f"('{version}' currently installed)."
```

### Comparing `modflow-devtools-1.4.0/modflow_devtools/markers.py` & `modflow_devtools-1.5.0/modflow_devtools/markers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 Pytest markers to toggle tests based on environment conditions.
 Occasionally useful to directly assert environment expectations.
 """
 
+from os import environ
 from platform import python_version, system
+from typing import Dict, Optional
 
 from packaging.version import Version
 
 from modflow_devtools.imports import import_optional_dependency
 from modflow_devtools.misc import (
     get_current_branch,
     has_exe,
@@ -27,68 +29,69 @@
         reason=f"missing executable{'s' if len(missing) != 1 else ''}: "
         + ", ".join(missing),
     )
 
 
 def requires_python(version, bound="lower"):
     if not isinstance(version, str):
-        raise ValueError(f"Version must a string")
+        raise ValueError("Version must a string")
 
     py_tgt = Version(version)
     if bound == "lower":
         return py_ver >= py_tgt
     elif bound == "upper":
         return py_ver <= py_tgt
     elif bound == "exact":
         return py_ver == py_tgt
     else:
         return ValueError(
             f"Invalid bound type: {bound} (use 'upper', 'lower', or 'exact')"
         )
 
 
-def requires_pkg(*pkgs):
-    missing = {pkg for pkg in pkgs if not has_pkg(pkg, strict=True)}
+def requires_pkg(*pkgs, name_map: Optional[Dict[str, str]] = None):
+    missing = {pkg for pkg in pkgs if not has_pkg(pkg, strict=True, name_map=name_map)}
     return pytest.mark.skipif(
         missing,
         reason=f"missing package{'s' if len(missing) != 1 else ''}: "
         + ", ".join(missing),
     )
 
 
 def requires_platform(platform, ci_only=False):
     return pytest.mark.skipif(
-        system().lower() != platform.lower()
-        and (is_in_ci() if ci_only else True),
+        system().lower() != platform.lower() and (is_in_ci() if ci_only else True),
         reason=f"only compatible with platform: {platform.lower()}",
     )
 
 
 def excludes_platform(platform, ci_only=False):
     return pytest.mark.skipif(
-        system().lower() == platform.lower()
-        and (is_in_ci() if ci_only else True),
+        system().lower() == platform.lower() and (is_in_ci() if ci_only else True),
         reason=f"not compatible with platform: {platform.lower()}",
     )
 
 
 def requires_branch(branch):
     current = get_current_branch()
-    return pytest.mark.skipif(
-        current != branch, reason=f"must run on branch: {branch}"
-    )
+    return pytest.mark.skipif(current != branch, reason=f"must run on branch: {branch}")
 
 
 def excludes_branch(branch):
     current = get_current_branch()
     return pytest.mark.skipif(
         current == branch, reason=f"can't run on branch: {branch}"
     )
 
 
+no_parallel = pytest.mark.skipif(
+    environ.get("PYTEST_XDIST_WORKER_COUNT"), reason="can't run in parallel"
+)
+
+
 requires_github = pytest.mark.skipif(
     not is_connected("github.com"), reason="github.com is required."
 )
 
 
 requires_spatial_reference = pytest.mark.skipif(
     not is_connected("spatialreference.org"),
```

### Comparing `modflow-devtools-1.4.0/modflow_devtools/misc.py` & `modflow_devtools-1.5.0/modflow_devtools/misc.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 from importlib import metadata
 from os import PathLike, chdir, environ, getcwd
 from os.path import basename, normpath
 from pathlib import Path
 from shutil import which
 from subprocess import PIPE, Popen
 from timeit import timeit
-from typing import List, Optional, Tuple
+from typing import Dict, List, Optional, Tuple
 from urllib import request
+from urllib.error import URLError
 
 from _warnings import warn
 
 
 @contextmanager
 def set_dir(path: PathLike):
     origin = Path(getcwd()).absolute()
@@ -66,15 +67,16 @@
     elif sys.platform.startswith("darwin"):
         return "mac"
     raise ValueError(f"platform {sys.platform!r} not supported")
 
 
 def get_suffixes(ostag) -> Tuple[str, str]:
     """
-    Returns executable and library suffixes for the given OS (as returned by sys.platform)
+    Returns executable and library suffixes for the
+    given OS (as returned by sys.platform)
 
     .. deprecated:: 1.1.0
         Use ``ostags.get_binary_suffixes()`` instead.
     """
 
     tag = ostag.lower()
 
@@ -146,73 +148,72 @@
     if code == 0 and stdout:
         return stdout.strip().lower()
     raise ValueError(f"Could not determine current branch: {stderr}")
 
 
 def get_packages(namefile_path: PathLike) -> List[str]:
     """
-    Return a list of packages used by the simulation or model defined in the given namefile.
-    The namefile may be for an entire simulation or for a GWF or GWT model. If a simulation
-    namefile is given, packages used in its component model namefiles will be included.
+    Return a list of packages used by the simulation
+    or model defined in the given namefile. The namefile
+    may be for an entire simulation or  for a GWF or GWT
+    model. If a simulation namefile is given, packages
+    used in its component  model namefiles will be included.
 
     Parameters
     ----------
     namefile_path : PathLike
         path to MODFLOW 6 simulation or model name file
 
     Returns
     -------
         a list of packages used by the simulation or model
     """
 
     packages = []
     path = Path(namefile_path).expanduser().absolute()
     lines = open(path, "r").readlines()
-    gwf_lines = [l for l in lines if l.strip().lower().startswith("gwf6 ")]
-    gwt_lines = [l for l in lines if l.strip().lower().startswith("gwt6 ")]
+    gwf_lines = [ln for ln in lines if ln.strip().lower().startswith("gwf6 ")]
+    gwt_lines = [ln for ln in lines if ln.strip().lower().startswith("gwt6 ")]
 
     def parse_model_namefile(line):
         nf_path = [path.parent / s for s in line.split(" ") if s != ""][1]
         if nf_path.suffix != ".nam":
             raise ValueError(
-                f"Failed to parse GWF or GWT model namefile from simulation namefile line: {line}"
+                "Failed to parse GWF or GWT model namefile "
+                f"from simulation namefile line: {line}"
             )
         return nf_path
 
     # load model namefiles
     try:
         for line in gwf_lines:
-            packages = (
-                packages + get_packages(parse_model_namefile(line)) + ["gwf"]
-            )
+            packages = packages + get_packages(parse_model_namefile(line)) + ["gwf"]
         for line in gwt_lines:
-            packages = (
-                packages + get_packages(parse_model_namefile(line)) + ["gwt"]
-            )
-    except:
+            packages = packages + get_packages(parse_model_namefile(line)) + ["gwt"]
+    except:  # noqa: E722
         warn(f"Invalid namefile format: {traceback.format_exc()}")
 
     for line in lines:
         # Skip over blank and commented lines
-        ll = line.strip().split()
-        if len(ll) < 2:
+        line = line.strip().split()
+        if len(line) < 2:
             continue
 
-        l = ll[0].lower()
-        if any(l.startswith(c) for c in ["#", "!", "data", "list"]) or l in [
+        line = line[0].lower()
+        if any(line.startswith(c) for c in ["#", "!", "data", "list"]) or line in [
             "begin",
             "end",
             "memory_print_option",
         ]:
             continue
 
         # strip "6" from package name
-        l = l.replace("6", "")
+        line = line.replace("6", "")
 
-        packages.append(l.lower())
+        packages.append(line.lower())
 
     return list(set(packages))
 
 
 def has_package(namefile_path: PathLike, package: str) -> bool:
     """
     Determines whether the model with the given namefile contains the selected package.
@@ -238,46 +239,37 @@
 
     # if path doesn't exist, return empty list
     if not Path(path).is_dir():
         return []
 
     # find simulation namefiles
     paths = [
-        p
-        for p in Path(path).rglob(
-            f"{prefix}*/**/{namefile}" if prefix else namefile
-        )
+        p for p in Path(path).rglob(f"{prefix}*/**/{namefile}" if prefix else namefile)
     ]
 
     # remove excluded
     paths = [
-        p
-        for p in paths
-        if (not excluded or not any(e in str(p) for e in excluded))
+        p for p in paths if (not excluded or not any(e in str(p) for e in excluded))
     ]
 
     # filter by package
     if packages:
         filtered = []
         for nfp in paths:
             nf_pkgs = get_packages(nfp)
-            shared = set(nf_pkgs).intersection(
-                set([p.lower() for p in packages])
-            )
+            shared = set(nf_pkgs).intersection(set([p.lower() for p in packages]))
             if any(shared):
                 filtered.append(nfp)
         paths = filtered
 
     # filter by model name
     if selected:
         paths = [
             namfile_path
-            for (namfile_path, model_path) in zip(
-                paths, [p.parent for p in paths]
-            )
+            for (namfile_path, model_path) in zip(paths, [p.parent for p in paths])
             if any(s in model_path.name for s in selected)
         ]
 
     return sorted(paths)
 
 
 def get_model_paths(
@@ -294,17 +286,15 @@
     namefiles. Model directories can be filtered or excluded,
     by prefix, pattern, namefile name, or packages used.
     """
 
     namefile_paths = get_namefile_paths(
         path, prefix, namefile, excluded, selected, packages
     )
-    model_paths = sorted(
-        list(set([p.parent for p in namefile_paths if p.parent.name]))
-    )
+    model_paths = sorted(list(set([p.parent for p in namefile_paths if p.parent.name])))
     return model_paths
 
 
 def is_connected(hostname):
     """
     Tests whether the given URL is accessible.
     See https://stackoverflow.com/a/20913928/.
@@ -334,27 +324,27 @@
 def is_github_rate_limited() -> Optional[bool]:
     """
     Determines if a GitHub API rate limit is applied to the current IP.
     Calling this function will consume an API request!
 
     Returns
     -------
-        True if rate-limiting is applied, otherwise False (or None if the connection fails).
+        True if rate-limiting is applied, otherwise False
+        (or None if the connection fails).
     """
     try:
-        with request.urlopen(
-            "https://api.github.com/users/octocat"
-        ) as response:
+        with request.urlopen("https://api.github.com/users/octocat") as response:
             remaining = int(response.headers["x-ratelimit-remaining"])
             if remaining < 10:
                 warn(
-                    f"Only {remaining} GitHub API requests remaining before rate-limiting"
+                    f"Only {remaining} GitHub API requests "
+                    "remaining before rate-limiting"
                 )
             return remaining > 0
-    except:
+    except (ValueError, URLError):
         return None
 
 
 _has_exe_cache = {}
 _has_pkg_cache = {}
 
 
@@ -365,58 +355,73 @@
     Originally written by Mike Toews (mwtoews@gmail.com) for FloPy.
     """
     if exe not in _has_exe_cache:
         _has_exe_cache[exe] = bool(which(exe))
     return _has_exe_cache[exe]
 
 
-def has_pkg(pkg: str, strict: bool = False) -> bool:
+def has_pkg(
+    pkg: str, strict: bool = False, name_map: Optional[Dict[str, str]] = None
+) -> bool:
     """
     Determines if the given Python package is installed.
 
     Parameters
     ----------
     pkg : str
         Name of the package to check.
     strict : bool
-        If False, only check if package metadata is available.
+        If False, only check if the package is cached or metadata is available.
         If True, try to import the package (all dependencies must be present).
+    name_map : dict, optional
+        Custom mapping between package names (as provided to `metadata.distribution`)
+        and module names (as used in import statements or `importlib.import_module`).
+        Useful for packages whose package names do not match the module name, e.g.
+        `pytest-xdist` and `xdist`, respectively, or `mfpymake` and `pymake`.
 
     Returns
     -------
     bool
         True if the package is installed, otherwise False.
 
     Notes
     -----
+    If `strict=True` and a package name differs from its top-level module name, a
+    `name_map` must be provided, otherwise this function will return False even if
+    the package is installed.
+
     Originally written by Mike Toews (mwtoews@gmail.com) for FloPy.
     """
 
-    def try_import():
+    def get_module_name() -> str:
+        return pkg if name_map is None else name_map.get(pkg, pkg)
+
+    def try_import() -> bool:
         try:  # import name, e.g. "import shapefile"
-            importlib.import_module(pkg)
+            importlib.import_module(get_module_name())
             return True
         except ModuleNotFoundError:
             return False
 
     def try_metadata() -> bool:
         try:  # package name, e.g. pyshp
             metadata.distribution(pkg)
             return True
         except metadata.PackageNotFoundError:
             return False
 
-    found = False
-    if not strict:
-        found = pkg in _has_pkg_cache or try_metadata()
-    if not found:
-        found = try_import()
+    is_cached = pkg in _has_pkg_cache
+    has_metadata = try_metadata()
+    can_import = try_import()
+    if strict:
+        found = has_metadata and can_import
+    else:
+        found = has_metadata or is_cached
     _has_pkg_cache[pkg] = found
-
-    return _has_pkg_cache[pkg]
+    return found
 
 
 def timed(f):
     """
     Decorator for estimating runtime of any function.
     Prints estimated time to stdout, in milliseconds.
 
@@ -477,15 +482,22 @@
     otherwise the default value if the environment variable is not set.
     """
     try:
         v = environ.get(name)
         if isinstance(default, bool):
             v = v.lower().title()
         v = literal_eval(v)
-    except:
+    except (
+        AttributeError,
+        ValueError,
+        TypeError,
+        SyntaxError,
+        MemoryError,
+        RecursionError,
+    ):
         return default
     if default is None:
         return v
     return v if isinstance(v, type(default)) else default
 
 
 @contextmanager
```

### Comparing `modflow-devtools-1.4.0/modflow_devtools/ostags.py` & `modflow_devtools-1.5.0/modflow_devtools/ostags.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,18 +69,18 @@
         elif tag == "darwin" or "mac" in tag:
             return "", ".dylib"
         else:
             raise KeyError(f"Invalid OS tag: {tag!r}")
 
     try:
         return _suffixes(ostag.lower())
-    except:
+    except KeyError:
         try:
             return _suffixes(python_to_modflow_ostag(ostag))
-        except:
+        except KeyError:
             return _suffixes(github_to_modflow_ostag(ostag))
 
 
 def python_to_modflow_ostag(tag: str) -> str:
     """
     Convert a platform.system() string to an ostag as expected
     by MODFLOW 6.
```

### Comparing `modflow-devtools-1.4.0/modflow_devtools/zip.py` & `modflow_devtools-1.5.0/modflow_devtools/zip.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-1.4.0/modflow_devtools.egg-info/PKG-INFO` & `modflow_devtools-1.5.0/modflow_devtools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modflow-devtools
-Version: 1.4.0
+Version: 1.5.0
 Summary: Python tools for MODFLOW development
 Author-email: "Joseph D. Hughes" <modflow@usgs.gov>, Michael Reno <mreno@ucar.edu>, Mike Taves <mwtoews@gmail.com>, Wes Bonelli <wbonelli@ucar.edu>
 Maintainer-email: "Joseph D. Hughes" <modflow@usgs.gov>
 License: CC0
 Project-URL: Documentation, https://modflow-devtools.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/MODFLOW-USGS/modflow-devtools/issues
 Project-URL: Source Code, https://github.com/MODFLOW-USGS/modflow-devtools
@@ -20,32 +20,30 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Provides-Extra: lint
-Requires-Dist: black; extra == "lint"
-Requires-Dist: cffconvert; extra == "lint"
-Requires-Dist: flake8; extra == "lint"
-Requires-Dist: isort; extra == "lint"
-Requires-Dist: pylint; extra == "lint"
+Requires-Dist: ruff; extra == "lint"
 Provides-Extra: test
 Requires-Dist: modflow-devtools[lint]; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: flaky; extra == "test"
 Requires-Dist: filelock; extra == "test"
 Requires-Dist: meson!=0.63.0; extra == "test"
 Requires-Dist: ninja; extra == "test"
 Requires-Dist: numpy; extra == "test"
-Requires-Dist: pytest; extra == "test"
+Requires-Dist: pandas; extra == "test"
+Requires-Dist: pytest!=8.1.0; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-dotenv; extra == "test"
 Requires-Dist: pytest-xdist; extra == "test"
 Requires-Dist: PyYaml; extra == "test"
+Requires-Dist: syrupy; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 
 # MODFLOW developer tools
 
@@ -101,32 +99,33 @@
 
 ## Requirements
 
 Python3.8+, dependency-free, but pairs well with `pytest` and select plugins, e.g.
 
 - [`pytest-dotenv`](https://github.com/quiqua/pytest-dotenv)
 - [`pytest-xdist`](https://github.com/pytest-dev/pytest-xdist)
+- [`syrupy`](https://github.com/tophat/syrupy)
 
 ## Installation
 
 `modflow-devtools` is available on PyPI and can be installed with pip:
 
 ```shell
 pip install modflow-devtools
 ```
 
-Pytest, pytest plugins, and other optional dependencies can be installed with:
+Pytest, pytest plugins, and other testing-related dependencies can be installed with:
 
 ```shell
 pip install "modflow-devtools[test]"
 ```
 
 To install from source and set up a development environment please see the [developer documentation](DEVELOPER.md).
 
-To import `pytest` fixtures in a project consuming `modflow-devtools`, add the following to a `conftest.py` file:
+To import `pytest` fixtures in a project consuming `modflow-devtools`, add the following to a test file or `conftest.py` file:
 
 ```python
 pytest_plugins = [ "modflow_devtools.fixtures" ]
 ```
 
 **Note**: this must be a top-level `conftest.py`, which nested `conftest.py` files may then override or extend.
```

### Comparing `modflow-devtools-1.4.0/modflow_devtools.egg-info/SOURCES.txt` & `modflow_devtools-1.5.0/modflow_devtools.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 modflow_devtools/download.py
 modflow_devtools/fixtures.py
 modflow_devtools/imports.py
 modflow_devtools/latex.py
 modflow_devtools/markers.py
 modflow_devtools/misc.py
 modflow_devtools/ostags.py
+modflow_devtools/snapshots.py
 modflow_devtools/zip.py
 modflow_devtools.egg-info/PKG-INFO
 modflow_devtools.egg-info/SOURCES.txt
 modflow_devtools.egg-info/dependency_links.txt
 modflow_devtools.egg-info/not-zip-safe
 modflow_devtools.egg-info/requires.txt
 modflow_devtools.egg-info/top_level.txt
```

### Comparing `modflow-devtools-1.4.0/pyproject.toml` & `modflow_devtools-1.5.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -40,58 +40,56 @@
     "Topic :: Scientific/Engineering :: Hydrology"
 ]
 requires-python = ">=3.8"
 dynamic = ["version"]
 
 [project.optional-dependencies]
 lint = [
-    "black",
-    "cffconvert",
-    "flake8",
-    "isort",
-    "pylint"
+    "ruff"
 ]
 test = [
     "modflow-devtools[lint]",
     "coverage",
     "flaky",
     "filelock",
     "meson!=0.63.0",
     "ninja",
     "numpy",
-    "pytest",
+    "pandas",
+    "pytest!=8.1.0",
     "pytest-cov",
     "pytest-dotenv",
     "pytest-xdist",
-    "PyYaml"
+    "PyYaml",
+    "syrupy"
 ]
 docs = [
     "sphinx",
     "sphinx-rtd-theme",
     "myst-parser"
 ]
 
 [project.urls]
 "Documentation" = "https://modflow-devtools.readthedocs.io/en/latest/"
 "Bug Tracker" = "https://github.com/MODFLOW-USGS/modflow-devtools/issues"
 "Source Code" = "https://github.com/MODFLOW-USGS/modflow-devtools"
 
+[tool.ruff]
+target-version = "py38"
+include = [
+    "pyproject.toml",
+    "modflow_devtools/**/*.py",
+    "autotest/**/*.py",
+    "docs/**/*.py",
+    "scripts/**/*.py",
+    ".github/**/*.py",
+]
 
-[tool.black]
-line-length = 79
-target_version = ["py37"]
-
-[tool.flynt]
-line-length = 79
-verbose = true
-
-[tool.isort]
-profile = "black"
-src_paths = ["modflow_devtools"]
-line_length = 79
+[tool.ruff.lint]
+select = ["F", "E", "I001"]
 
 [tool.setuptools]
 packages = ["modflow_devtools"]
 include-package-data = true
 zip-safe = false
 
 [tool.setuptools.dynamic]
```

