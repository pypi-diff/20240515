# Comparing `tmp/pyproject_fmt-2.0.4.tar.gz` & `tmp/pyproject_fmt-2.1.0.tar.gz`

## Comparing `pyproject_fmt-2.0.4.tar` & `pyproject_fmt-2.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.4/tox.ini
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.4/src/pyproject_fmt/__init__.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.4/src/pyproject_fmt/__main__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.4/src/pyproject_fmt/_version.py
--rw-r--r--   0        0        0     5639 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.4/src/pyproject_fmt/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.4/src/pyproject_fmt/py.typed
--rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.4/tests/test_cli.py
--rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.4/tests/test_main.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.4/tests/test_pyproject_toml_fmt.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.4/.gitignore
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.4/LICENSE.txt
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.4/README.md
--rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.4/pyproject.toml
--rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.0/tox.ini
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.0/src/pyproject_fmt/__init__.py
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.0/src/pyproject_fmt/__main__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.0/src/pyproject_fmt/_version.py
+-rw-r--r--   0        0        0     6105 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.0/src/pyproject_fmt/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.0/src/pyproject_fmt/py.typed
+-rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.0/tests/test_cli.py
+-rw-r--r--   0        0        0     6747 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.0/tests/test_main.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.0/tests/test_pyproject_toml_fmt.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.0/.gitignore
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.0/LICENSE.txt
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.0/README.md
+-rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.0/PKG-INFO
```

### Comparing `pyproject_fmt-2.0.4/tox.ini` & `pyproject_fmt-2.1.0/tox.ini`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-2.0.4/src/pyproject_fmt/__main__.py` & `pyproject_fmt-2.1.0/src/pyproject_fmt/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,14 +40,16 @@
     changed = before != formatted
     if config.stdout:  # stdout just prints new format to stdout
         print(formatted, end="")  # noqa: T201
         return changed
 
     if before != formatted and not config.check:
         config.pyproject_toml.write_text(formatted, encoding="utf-8")
+    if config.no_print_diff:
+        return changed
     try:
         name = str(config.pyproject_toml.relative_to(Path.cwd()))
     except ValueError:
         name = str(config.pyproject_toml)
     diff: Iterable[str] = []
     if changed:
         diff = difflib.unified_diff(before.splitlines(), formatted.splitlines(), fromfile=name, tofile=name)
@@ -60,16 +62,16 @@
     return changed
 
 
 def run(args: Sequence[str] | None = None) -> int:
     """
     Run the formatter.
 
-    :param args: CLI arguments
-    :return: exit code
+    :param args: command line arguments, by default use sys.argv[1:]
+    :return: exit code - 0 means already formatted correctly, otherwise 1
     """
     configs = cli_args(sys.argv[1:] if args is None else args)
     results = [_handle_one(config) for config in configs]
     return 1 if any(results) else 0  # exit with non success on change
 
 
 if __name__ == "__main__":
```

### Comparing `pyproject_fmt-2.0.4/src/pyproject_fmt/cli.py` & `pyproject_fmt-2.1.0/src/pyproject_fmt/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,28 +25,30 @@
 
 class PyProjectFmtNamespace(Namespace):
     """Options for pyproject-fmt tool."""
 
     inputs: list[Path]
     stdout: bool
     check: bool
+    no_print_diff: bool
 
     column_width: int
     indent: int
     keep_full_version: bool
     max_supported_python: tuple[int, int]
 
 
 @dataclass(frozen=True)
 class Config:
     """Configuration flags for the formatting."""
 
     pyproject_toml: Path
     stdout: bool  # push to standard out
     check: bool  # check only
+    no_print_diff: bool  # don't print diff
     settings: Settings
 
     @property
     def toml(self) -> str:
         """:return: the toml files content"""
         return self.pyproject_toml.read_text(encoding="utf-8")
 
@@ -96,44 +98,60 @@
     parser.add_argument(
         "-V",
         "--version",
         action="version",
         help="print package version of pyproject_fmt",
         version=f"%(prog)s ({version('pyproject-fmt')})",
     )
-    group = parser.add_mutually_exclusive_group()
-    msg = "print the formatted text to the stdout (instead of update in-place)"
-    group.add_argument("-s", "--stdout", action="store_true", help=msg)
+
+    mode_group = parser.add_argument_group("run mode")
+    mode = mode_group.add_mutually_exclusive_group()
+    msg = "print the formatted TOML to the stdout"
+    mode.add_argument("-s", "--stdout", action="store_true", help=msg)
     msg = "check and fail if any input would be formatted, printing any diffs"
-    group.add_argument("--check", action="store_true", help=msg)
-    parser.add_argument(
+    mode.add_argument("--check", action="store_true", help=msg)
+    mode_group.add_argument(
+        "-n",
+        "--no-print-diff",
+        action="store_true",
+        help="Flag indicating to print diff for the check mode",
+    )
+
+    format_group = parser.add_argument_group("formatting behavior")
+    format_group.add_argument(
         "--column-width",
         type=int,
         default=1,
-        help="max column width in the file",
+        help="max column width in the TOML file",
         metavar="count",
     )
-    parser.add_argument(
+    format_group.add_argument(
         "--indent",
         type=int,
         default=2,
-        help="number of spaces to indent",
+        help="number of spaces to use for indentation",
         metavar="count",
     )
-    parser.add_argument(
+    msg = "keep full dependency versions - do not remove redundant .0 from versions"
+    format_group.add_argument("--keep-full-version", action="store_true", help=msg)
+    format_group.add_argument(
         "--max-supported-python",
         metavar="minor.major",
         type=_version_argument,
         default=(3, 12),
         help="latest Python version the project supports (e.g. 3.13)",
     )
-    msg = "keep full dependency versions - do not remove redundant .0 from versions"
-    parser.add_argument("--keep-full-version", action="store_true", help=msg)
+
     msg = "pyproject.toml file(s) to format"
-    parser.add_argument("inputs", nargs="+", type=pyproject_toml_path_creator, help=msg)
+    parser.add_argument(
+        "inputs",
+        nargs="+",
+        type=pyproject_toml_path_creator,
+        help=msg,
+    )
     return parser
 
 
 def cli_args(args: Sequence[str]) -> list[Config]:
     """
     Load the tools options.
 
@@ -162,14 +180,15 @@
                     elif key == "max_supported_python":
                         max_supported_python = _version_argument(entry)
         res.append(
             Config(
                 pyproject_toml=pyproject_toml,
                 stdout=opt.stdout,
                 check=opt.check,
+                no_print_diff=opt.no_print_diff,
                 settings=Settings(
                     column_width=column_width,
                     indent=indent,
                     keep_full_version=keep_full_version,
                     max_supported_python=max_supported_python,
                     min_supported_python=(3, 8),  # default for when the user did not specify via requires-python
                 ),
```

### Comparing `pyproject_fmt-2.0.4/tests/test_cli.py` & `pyproject_fmt-2.1.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-2.0.4/tests/test_main.py` & `pyproject_fmt-2.1.0/tests/test_main.py`

 * *Files 14% similar despite different names*

```diff
@@ -245,7 +245,58 @@
     ignore_extra = true
     """
     got = filename.read_text()
     assert got == dedent(expected)
     out, err = capsys.readouterr()
     assert out
     assert not err
+
+
+def test_pyproject_ftm_api_changed(tmp_path: Path, capsys: pytest.CaptureFixture[str]) -> None:
+    txt = """
+    [project]
+    requires-python = "==3.12"
+    """
+    filename = tmp_path / "pyproject.toml"
+    filename.write_text(dedent(txt))
+    res = run([str(filename), "--no-print-diff"])
+
+    assert res == 1
+
+    got = filename.read_text()
+    expected = """\
+    [project]
+    requires-python = "==3.12"
+    classifiers = [
+      "Programming Language :: Python :: 3 :: Only",
+      "Programming Language :: Python :: 3.12",
+    ]
+    """
+    assert got == dedent(expected)
+
+    out, err = capsys.readouterr()
+    assert not out
+    assert not err
+
+
+def test_pyproject_ftm_api_no_change(tmp_path: Path, capsys: pytest.CaptureFixture[str]) -> None:
+    txt = """\
+    [project]
+    requires-python = "==3.12"
+    classifiers = [
+      "Programming Language :: Python :: 3 :: Only",
+      "Programming Language :: Python :: 3.12",
+    ]
+    """
+    filename = tmp_path / "pyproject.toml"
+    filename.write_text(dedent(txt))
+    res = run([str(filename), "--no-print-diff"])
+
+    assert res == 0
+
+    got = filename.read_text()
+
+    assert got == dedent(txt)
+
+    out, err = capsys.readouterr()
+    assert not out
+    assert not err
```

### Comparing `pyproject_fmt-2.0.4/LICENSE.txt` & `pyproject_fmt-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-2.0.4/README.md` & `pyproject_fmt-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-2.0.4/pyproject.toml` & `pyproject_fmt-2.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
-  "pyproject-fmt-rust==1.0.6",
+  "pyproject-fmt-rust==1.1",
   "tomli>=2.0.1; python_version<'3.11'",
 ]
 optional-dependencies.docs = [
   "furo>=2024.5.6",
   "sphinx>=7.3.7",
   "sphinx-argparse-cli>=1.15",
   "sphinx-autodoc-typehints>=2.1",
@@ -127,11 +127,12 @@
   "**\\src",
 ]
 report.fail_under = 100
 run.parallel = true
 run.plugins = [
   "covdefaults",
 ]
+covdefaults.subtract_omit = "*/__main__.py"
 
 [tool.mypy]
 show_error_codes = true
 strict = true
```

### Comparing `pyproject_fmt-2.0.4/PKG-INFO` & `pyproject_fmt-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyproject-fmt
-Version: 2.0.4
+Version: 2.1.0
 Summary: Format your pyproject.toml file
 Project-URL: Bug Tracker, https://github.com/tox-dev/pyproject-fmt/issues
 Project-URL: Changelog, https://github.com/tox-dev/pyproject-fmt/releases
 Project-URL: Documentation, https://github.com/tox-dev/pyproject-fmt/
 Project-URL: Source Code, https://github.com/tox-dev/pyproject-fmt
 Author-email: Bernat Gabor <gaborjbernat@gmail.com>
 License: Permission is hereby granted, free of charge, to any person obtaining a
@@ -33,15 +33,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
-Requires-Dist: pyproject-fmt-rust==1.0.6
+Requires-Dist: pyproject-fmt-rust==1.1
 Requires-Dist: tomli>=2.0.1; python_version < '3.11'
 Provides-Extra: docs
 Requires-Dist: furo>=2024.5.6; extra == 'docs'
 Requires-Dist: sphinx-argparse-cli>=1.15; extra == 'docs'
 Requires-Dist: sphinx-autodoc-typehints>=2.1; extra == 'docs'
 Requires-Dist: sphinx-copybutton>=0.5.2; extra == 'docs'
 Requires-Dist: sphinx>=7.3.7; extra == 'docs'
```

