# Comparing `tmp/wcmatch-8.5.1.tar.gz` & `tmp/wcmatch-8.5.2.tar.gz`

## Comparing `wcmatch-8.5.1.tar` & `wcmatch-8.5.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 wcmatch-8.5.1/.coveragerc
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 wcmatch-8.5.1/.pyspelling.yml
--rw-r--r--   0        0        0     4142 2020-02-02 00:00:00.000000 wcmatch-8.5.1/mkdocs.yml
--rw-r--r--   0        0        0    17334 2020-02-02 00:00:00.000000 wcmatch-8.5.1/docs/src/markdown/fnmatch.md
--rw-r--r--   0        0        0    52675 2020-02-02 00:00:00.000000 wcmatch-8.5.1/docs/src/markdown/glob.md
--rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 wcmatch-8.5.1/docs/src/markdown/index.md
--rw-r--r--   0        0        0    34205 2020-02-02 00:00:00.000000 wcmatch-8.5.1/docs/src/markdown/pathlib.md
--rw-r--r--   0        0        0    18670 2020-02-02 00:00:00.000000 wcmatch-8.5.1/docs/src/markdown/wcmatch.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wcmatch-8.5.1/docs/src/markdown/.snippets/abbr.md
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 wcmatch-8.5.1/docs/src/markdown/.snippets/links.md
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 wcmatch-8.5.1/docs/src/markdown/.snippets/posix.md
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 wcmatch-8.5.1/docs/src/markdown/.snippets/refs.md
--rw-r--r--   0        0        0    21718 2020-02-02 00:00:00.000000 wcmatch-8.5.1/docs/src/markdown/about/changelog.md
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 wcmatch-8.5.1/docs/src/markdown/about/contributing.md
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 wcmatch-8.5.1/docs/src/markdown/about/license.md
--rw-r--r--   0        0        0    11943 2020-02-02 00:00:00.000000 wcmatch-8.5.1/docs/src/markdown/about/release.md
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 wcmatch-8.5.1/docs/theme/announce.html
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 wcmatch-8.5.1/requirements/docs.txt
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 wcmatch-8.5.1/requirements/lint.txt
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 wcmatch-8.5.1/requirements/setup.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 wcmatch-8.5.1/requirements/test.txt
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 wcmatch-8.5.1/tests/__init__.py
--rw-r--r--   0        0        0    29587 2020-02-02 00:00:00.000000 wcmatch-8.5.1/tests/test_fnmatch.py
--rw-r--r--   0        0        0    61082 2020-02-02 00:00:00.000000 wcmatch-8.5.1/tests/test_glob.py
--rw-r--r--   0        0        0    69199 2020-02-02 00:00:00.000000 wcmatch-8.5.1/tests/test_globmatch.py
--rw-r--r--   0        0        0    12362 2020-02-02 00:00:00.000000 wcmatch-8.5.1/tests/test_pathlib.py
--rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 wcmatch-8.5.1/tests/test_versions.py
--rw-r--r--   0        0        0    16584 2020-02-02 00:00:00.000000 wcmatch-8.5.1/tests/test_wcmatch.py
--rw-r--r--   0        0        0     6716 2020-02-02 00:00:00.000000 wcmatch-8.5.1/tests/test_wcparse.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 wcmatch-8.5.1/wcmatch/__init__.py
--rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 wcmatch-8.5.1/wcmatch/__meta__.py
--rw-r--r--   0        0        0    10935 2020-02-02 00:00:00.000000 wcmatch-8.5.1/wcmatch/_wcmatch.py
--rw-r--r--   0        0        0    56020 2020-02-02 00:00:00.000000 wcmatch-8.5.1/wcmatch/_wcparse.py
--rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 wcmatch-8.5.1/wcmatch/fnmatch.py
--rw-r--r--   0        0        0    35154 2020-02-02 00:00:00.000000 wcmatch-8.5.1/wcmatch/glob.py
--rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 wcmatch-8.5.1/wcmatch/pathlib.py
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 wcmatch-8.5.1/wcmatch/posix.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wcmatch-8.5.1/wcmatch/py.typed
--rw-r--r--   0        0        0     6855 2020-02-02 00:00:00.000000 wcmatch-8.5.1/wcmatch/util.py
--rw-r--r--   0        0        0    10077 2020-02-02 00:00:00.000000 wcmatch-8.5.1/wcmatch/wcmatch.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 wcmatch-8.5.1/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 wcmatch-8.5.1/LICENSE.md
--rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 wcmatch-8.5.1/README.md
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 wcmatch-8.5.1/hatch_build.py
--rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 wcmatch-8.5.1/pyproject.toml
--rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 wcmatch-8.5.1/PKG-INFO
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 wcmatch-8.5.2/.coveragerc
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 wcmatch-8.5.2/.pyspelling.yml
+-rw-r--r--   0        0        0     4142 2020-02-02 00:00:00.000000 wcmatch-8.5.2/mkdocs.yml
+-rw-r--r--   0        0        0    17334 2020-02-02 00:00:00.000000 wcmatch-8.5.2/docs/src/markdown/fnmatch.md
+-rw-r--r--   0        0        0    52675 2020-02-02 00:00:00.000000 wcmatch-8.5.2/docs/src/markdown/glob.md
+-rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 wcmatch-8.5.2/docs/src/markdown/index.md
+-rw-r--r--   0        0        0    34205 2020-02-02 00:00:00.000000 wcmatch-8.5.2/docs/src/markdown/pathlib.md
+-rw-r--r--   0        0        0    18673 2020-02-02 00:00:00.000000 wcmatch-8.5.2/docs/src/markdown/wcmatch.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wcmatch-8.5.2/docs/src/markdown/.snippets/abbr.md
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 wcmatch-8.5.2/docs/src/markdown/.snippets/links.md
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 wcmatch-8.5.2/docs/src/markdown/.snippets/posix.md
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 wcmatch-8.5.2/docs/src/markdown/.snippets/refs.md
+-rw-r--r--   0        0        0    21874 2020-02-02 00:00:00.000000 wcmatch-8.5.2/docs/src/markdown/about/changelog.md
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 wcmatch-8.5.2/docs/src/markdown/about/contributing.md
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 wcmatch-8.5.2/docs/src/markdown/about/license.md
+-rw-r--r--   0        0        0    11943 2020-02-02 00:00:00.000000 wcmatch-8.5.2/docs/src/markdown/about/release.md
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 wcmatch-8.5.2/docs/theme/announce.html
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 wcmatch-8.5.2/requirements/docs.txt
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 wcmatch-8.5.2/requirements/lint.txt
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 wcmatch-8.5.2/requirements/setup.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 wcmatch-8.5.2/requirements/test.txt
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 wcmatch-8.5.2/tests/__init__.py
+-rw-r--r--   0        0        0    29753 2020-02-02 00:00:00.000000 wcmatch-8.5.2/tests/test_fnmatch.py
+-rw-r--r--   0        0        0    61082 2020-02-02 00:00:00.000000 wcmatch-8.5.2/tests/test_glob.py
+-rw-r--r--   0        0        0    69199 2020-02-02 00:00:00.000000 wcmatch-8.5.2/tests/test_globmatch.py
+-rw-r--r--   0        0        0    12362 2020-02-02 00:00:00.000000 wcmatch-8.5.2/tests/test_pathlib.py
+-rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 wcmatch-8.5.2/tests/test_versions.py
+-rw-r--r--   0        0        0    16584 2020-02-02 00:00:00.000000 wcmatch-8.5.2/tests/test_wcmatch.py
+-rw-r--r--   0        0        0     6716 2020-02-02 00:00:00.000000 wcmatch-8.5.2/tests/test_wcparse.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 wcmatch-8.5.2/wcmatch/__init__.py
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 wcmatch-8.5.2/wcmatch/__meta__.py
+-rw-r--r--   0        0        0    10935 2020-02-02 00:00:00.000000 wcmatch-8.5.2/wcmatch/_wcmatch.py
+-rw-r--r--   0        0        0    56044 2020-02-02 00:00:00.000000 wcmatch-8.5.2/wcmatch/_wcparse.py
+-rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 wcmatch-8.5.2/wcmatch/fnmatch.py
+-rw-r--r--   0        0        0    35154 2020-02-02 00:00:00.000000 wcmatch-8.5.2/wcmatch/glob.py
+-rw-r--r--   0        0        0     7567 2020-02-02 00:00:00.000000 wcmatch-8.5.2/wcmatch/pathlib.py
+-rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 wcmatch-8.5.2/wcmatch/posix.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wcmatch-8.5.2/wcmatch/py.typed
+-rw-r--r--   0        0        0     6891 2020-02-02 00:00:00.000000 wcmatch-8.5.2/wcmatch/util.py
+-rw-r--r--   0        0        0    10077 2020-02-02 00:00:00.000000 wcmatch-8.5.2/wcmatch/wcmatch.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 wcmatch-8.5.2/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 wcmatch-8.5.2/LICENSE.md
+-rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 wcmatch-8.5.2/README.md
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 wcmatch-8.5.2/hatch_build.py
+-rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 wcmatch-8.5.2/pyproject.toml
+-rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 wcmatch-8.5.2/PKG-INFO
```

### Comparing `wcmatch-8.5.1/.pyspelling.yml` & `wcmatch-8.5.2/.pyspelling.yml`

 * *Files identical despite different names*

### Comparing `wcmatch-8.5.1/mkdocs.yml` & `wcmatch-8.5.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `wcmatch-8.5.1/docs/src/markdown/fnmatch.md` & `wcmatch-8.5.2/docs/src/markdown/fnmatch.md`

 * *Files identical despite different names*

### Comparing `wcmatch-8.5.1/docs/src/markdown/glob.md` & `wcmatch-8.5.2/docs/src/markdown/glob.md`

 * *Files identical despite different names*

### Comparing `wcmatch-8.5.1/docs/src/markdown/index.md` & `wcmatch-8.5.2/docs/src/markdown/index.md`

 * *Files identical despite different names*

### Comparing `wcmatch-8.5.1/docs/src/markdown/pathlib.md` & `wcmatch-8.5.2/docs/src/markdown/pathlib.md`

 * *Files identical despite different names*

### Comparing `wcmatch-8.5.1/docs/src/markdown/wcmatch.md` & `wcmatch-8.5.2/docs/src/markdown/wcmatch.md`

 * *Files 0% similar despite different names*

```diff
@@ -306,17 +306,17 @@
 `RECURSIVE` forces a recursive search that will crawl all subdirectories.
 
 #### `wcmatch.HIDDEN, wcmatch.HD` {: #hidden}
 
 `HIDDEN` enables the crawling of hidden directories and will return hidden files if the wildcard pattern matches. This
 enables not just dot files, but system hidden files as well.
 
-#### `wcmatch.SYMLINK, wcmatch.SL` {: #symlink}
+#### `wcmatch.SYMLINKS, wcmatch.SL` {: #symlinks}
 
-`SYMLINK` enables the crawling of symlink directories. By default, symlink directories are ignored during the file
+`SYMLINKS` enables the crawling of symlink directories. By default, symlink directories are ignored during the file
 crawl.
 
 #### `wcmatch.CASE, wcmatch.C` {: #case}
 
 `CASE` forces case sensitivity. `CASE` has higher priority than [`IGNORECASE`](#ignorecase).
 
 #### `wcmatch.IGNORECASE, wcmatch.I` {: #ignorecase}
```

### Comparing `wcmatch-8.5.1/docs/src/markdown/.snippets/posix.md` & `wcmatch-8.5.2/docs/src/markdown/.snippets/posix.md`

 * *Files identical despite different names*

### Comparing `wcmatch-8.5.1/docs/src/markdown/about/changelog.md` & `wcmatch-8.5.2/docs/src/markdown/about/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Changelog
 
+## 8.5.2
+
+-   **FIX**: Fix `pathlib` issue with inheritance on Python versions greater than 3.12.
+-   **FIX**: Fix `EXTMATCH` case with `!(...)` patterns.
+
 ## 8.5.1
 
 -   **FIX**: Fix issue with type check failure in `wcmatch.glob`.
 
 ## 8.5
 
 -   **NEW**: Formally support Python 3.11 (no change).
```

### Comparing `wcmatch-8.5.1/docs/src/markdown/about/contributing.md` & `wcmatch-8.5.2/docs/src/markdown/about/contributing.md`

 * *Files identical despite different names*

### Comparing `wcmatch-8.5.1/docs/src/markdown/about/release.md` & `wcmatch-8.5.2/docs/src/markdown/about/release.md`

 * *Files identical despite different names*

### Comparing `wcmatch-8.5.1/tests/test_fnmatch.py` & `wcmatch-8.5.2/tests/test_fnmatch.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,14 +144,18 @@
         ['a*(?)bc', 'a.bc', True, fnmatch.E | fnmatch.D],
         ['a*(?|.)bc', 'a.bc', True, fnmatch.E | fnmatch.D],
         ['a*(?|*)bc', 'a.bc', True, fnmatch.E | fnmatch.D],
         ['!(test)', '.abc', False, fnmatch.D | fnmatch.E],
         ['!(test)', 'abc', True, fnmatch.D | fnmatch.E],
         ['!(test)', '..', False, fnmatch.D | fnmatch.E],
 
+        # Negation list followed by extended list
+        ['!(2)_@(foo|bar)', '1_foo', True, fnmatch.E],
+        ['!(!(2|3))_@(foo|bar)', '2_foo', True, fnmatch.E],
+
         # POSIX style character classes
         ['[[:alnum:]]bc', 'zbc', True, 0],
         ['[[:alnum:]]bc', '1bc', True, 0],
         ['[a[:alnum:]]bc', 'zbc', True, 0],
         ['[[:alnum:][:blank:]]bc', ' bc', True, 0],
         ['*([[:word:]])', 'WoRD5_', True, fnmatch.E],
```

### Comparing `wcmatch-8.5.1/tests/test_glob.py` & `wcmatch-8.5.2/tests/test_glob.py`

 * *Files identical despite different names*

### Comparing `wcmatch-8.5.1/tests/test_globmatch.py` & `wcmatch-8.5.2/tests/test_globmatch.py`

 * *Files identical despite different names*

### Comparing `wcmatch-8.5.1/tests/test_pathlib.py` & `wcmatch-8.5.2/tests/test_pathlib.py`

 * *Files identical despite different names*

### Comparing `wcmatch-8.5.1/tests/test_versions.py` & `wcmatch-8.5.2/tests/test_versions.py`

 * *Files identical despite different names*

### Comparing `wcmatch-8.5.1/tests/test_wcmatch.py` & `wcmatch-8.5.2/tests/test_wcmatch.py`

 * *Files identical despite different names*

### Comparing `wcmatch-8.5.1/tests/test_wcparse.py` & `wcmatch-8.5.2/tests/test_wcparse.py`

 * *Files identical despite different names*

### Comparing `wcmatch-8.5.1/wcmatch/__meta__.py` & `wcmatch-8.5.2/wcmatch/__meta__.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,9 +190,9 @@
 
     # Handle post
     post = int(m.group('post')) if m.group('post') else 0
 
     return Version(major, minor, micro, release, pre, post, dev)
 
 
-__version_info__ = Version(8, 5, 1, "final")
+__version_info__ = Version(8, 5, 2, "final")
 __version__ = __version_info__._get_canonical()
```

### Comparing `wcmatch-8.5.1/wcmatch/_wcmatch.py` & `wcmatch-8.5.2/wcmatch/_wcmatch.py`

 * *Files identical despite different names*

### Comparing `wcmatch-8.5.1/wcmatch/_wcparse.py` & `wcmatch-8.5.2/wcmatch/_wcparse.py`

 * *Files 0% similar despite different names*

```diff
@@ -1431,15 +1431,16 @@
                 elif c == '?':
                     extended.append(self._restrict_sequence() + _QMARK)
                 elif c == '/':
                     if self.pathname:
                         extended.append(self._restrict_extended_slash())
                     extended.append(self.sep)
                 elif c == "|":
-                    self.clean_up_inverse(extended, temp_inv_nest and self.inv_nest)
+                    if self.inv_nest:
+                        self.clean_up_inverse(extended, temp_inv_nest)
                     extended.append(c)
                     if temp_after_start:
                         self.set_start_dir()
                 elif c == '\\':
                     try:
                         extended.append(self._references(i))
                     except DotException:
```

### Comparing `wcmatch-8.5.1/wcmatch/fnmatch.py` & `wcmatch-8.5.2/wcmatch/fnmatch.py`

 * *Files identical despite different names*

### Comparing `wcmatch-8.5.1/wcmatch/glob.py` & `wcmatch-8.5.2/wcmatch/glob.py`

 * *Files identical despite different names*

### Comparing `wcmatch-8.5.1/wcmatch/pathlib.py` & `wcmatch-8.5.2/wcmatch/pathlib.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Pathlib implementation that uses our own glob."""
 from __future__ import annotations
-import ntpath
-import posixpath
 import pathlib
 import os
 from . import glob
 from . import _wcparse
 from . import util
 from typing import Iterable, Any, Sequence
 
@@ -105,15 +103,15 @@
 
     def _translate_path(self) -> str:
         """Translate the object to a path string and ensure trailing slash for non-pure paths that are directories."""
 
         sep = ''
         name = str(self)
         if isinstance(self, Path) and name and self.is_dir():
-            sep = self._flavour.sep
+            sep = self.parser.sep if util.PY313 else self._flavour.sep
 
         return name + sep
 
     def match(  # type: ignore[override, unused-ignore]
         self,
         patterns: str | Sequence[str],
         *,
@@ -223,25 +221,23 @@
         `GLOBSTAR` is enabled by default in order match the default behavior of `pathlib`.
 
         """
 
         yield from self.glob(patterns, flags=flags | _EXTMATCHBASE, limit=limit, exclude=exclude)
 
 
-class PurePosixPath(PurePath):
+class PurePosixPath(PurePath, pathlib.PurePosixPath):
     """Pure Posix path."""
 
-    _flavour = pathlib._posix_flavour if not util.PY312 else posixpath  # type: ignore[attr-defined]
     __slots__ = ()
 
 
-class PureWindowsPath(PurePath):
+class PureWindowsPath(PurePath, pathlib.PureWindowsPath):
     """Pure Windows path."""
 
-    _flavour = pathlib._windows_flavour if not util.PY312 else ntpath  # type: ignore[attr-defined]
     __slots__ = ()
 
 
 class PosixPath(Path, PurePosixPath):
     """Posix path."""
 
     __slots__ = ()
```

### Comparing `wcmatch-8.5.1/wcmatch/posix.py` & `wcmatch-8.5.2/wcmatch/posix.py`

 * *Files identical despite different names*

### Comparing `wcmatch-8.5.1/wcmatch/util.py` & `wcmatch-8.5.2/wcmatch/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import unicodedata
 from functools import wraps
 import warnings
 from typing import Any, Callable, AnyStr, Match, Pattern, cast
 
 PY310 = (3, 10) <= sys.version_info
 PY312 = (3, 12) <= sys.version_info
+PY313 = (3, 13) <= sys.version_info
 
 UNICODE = 0
 BYTES = 1
 
 CASE_FS = os.path.normcase('A') != os.path.normcase('a')
 
 RE_NORM = re.compile(
```

### Comparing `wcmatch-8.5.1/wcmatch/wcmatch.py` & `wcmatch-8.5.2/wcmatch/wcmatch.py`

 * *Files identical despite different names*

### Comparing `wcmatch-8.5.1/.gitignore` & `wcmatch-8.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `wcmatch-8.5.1/LICENSE.md` & `wcmatch-8.5.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `wcmatch-8.5.1/README.md` & `wcmatch-8.5.2/README.md`

 * *Files identical despite different names*

### Comparing `wcmatch-8.5.1/hatch_build.py` & `wcmatch-8.5.2/hatch_build.py`

 * *Files identical despite different names*

### Comparing `wcmatch-8.5.1/pyproject.toml` & `wcmatch-8.5.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 show_error_codes = true
 
 [tool.hatch.metadata.hooks.custom]
 
 [tool.ruff]
 line-length = 120
 
-select = [
+lint.select = [
     "A",    # flake8-builtins
     "B",    # flake8-bugbear
     "D",    # pydocstyle
     "C4",   # flake8-comprehensions
     "N",    # pep8-naming
     "E",    # pycodestyle
     "F",    # pyflakes
@@ -83,15 +83,15 @@
     "RUF",  # ruff
     # "UP",   # pyupgrade
     "W",    # pycodestyle
     "YTT",  # flake8-2020,
     "PERF"  # Perflint
 ]
 
-ignore = [
+lint.ignore = [
     "E741",
     "D202",
     "D401",
     "D212",
     "D203",
     "D417",
     "N802",
```

### Comparing `wcmatch-8.5.1/PKG-INFO` & `wcmatch-8.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: wcmatch
-Version: 8.5.1
+Version: 8.5.2
 Summary: Wildcard/glob file name matcher.
 Project-URL: Homepage, https://github.com/facelessuser/wcmatch
 Author-email: Isaac Muse <Isaac.Muse@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.md
 Keywords: fnmatch,glob,search,wildcard
 Classifier: Development Status :: 5 - Production/Stable
```

