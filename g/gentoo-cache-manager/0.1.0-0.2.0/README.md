# Comparing `tmp/gentoo_cache_manager-0.1.0.tar.gz` & `tmp/gentoo_cache_manager-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gentoo_cache_manager-0.1.0.tar", last modified: Tue May 14 08:20:13 2024, max compression
+gzip compressed data, was "gentoo_cache_manager-0.2.0.tar", last modified: Wed May 15 11:11:17 2024, max compression
```

## Comparing `gentoo_cache_manager-0.1.0.tar` & `gentoo_cache_manager-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,39 @@
--rw-r--r--   0        0        0     1074 2024-05-14 08:19:56.061717 gentoo_cache_manager-0.1.0/LICENSE
--rw-r--r--   0        0        0     1417 2024-05-14 08:19:56.061717 gentoo_cache_manager-0.1.0/README.md
--rw-r--r--   0        0        0     2185 2024-05-14 08:20:13.598104 gentoo_cache_manager-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      118 2024-05-14 08:19:56.061717 gentoo_cache_manager-0.1.0/src/gcm/__init__.py
--rw-r--r--   0        0        0      239 2024-05-14 08:19:56.061717 gentoo_cache_manager-0.1.0/src/gcm/cli.py
--rw-r--r--   0        0        0      124 2024-05-14 08:19:56.061717 gentoo_cache_manager-0.1.0/src/gcm/commands/__init__.py
--rw-r--r--   0        0        0     2278 2024-05-14 08:19:56.061717 gentoo_cache_manager-0.1.0/src/gcm/commands/base.py
--rw-r--r--   0        0        0      207 2024-05-14 08:19:56.061717 gentoo_cache_manager-0.1.0/src/gcm/commands/context.py
--rw-r--r--   0        0        0      587 2024-05-14 08:19:56.061717 gentoo_cache_manager-0.1.0/src/gcm/commands/disable.py
--rw-r--r--   0        0        0     2235 2024-05-14 08:19:56.061717 gentoo_cache_manager-0.1.0/src/gcm/commands/enable.py
--rw-r--r--   0        0        0       84 2024-05-14 08:19:56.061717 gentoo_cache_manager-0.1.0/src/gcm/commands/exit_codes.py
--rw-r--r--   0        0        0     2625 2024-05-14 08:19:56.061717 gentoo_cache_manager-0.1.0/src/gcm/commands/stats.py
--rw-r--r--   0        0        0      874 2024-05-14 08:19:56.061717 gentoo_cache_manager-0.1.0/src/gcm/commands/validators.py
--rw-r--r--   0        0        0      622 2024-05-14 08:19:56.061717 gentoo_cache_manager-0.1.0/src/gcm/utils.py
--rw-r--r--   0        0        0     2809 2024-05-14 08:19:56.061717 gentoo_cache_manager-0.1.0/tests/commands/test_base.py
--rw-r--r--   0        0        0      347 2024-05-14 08:19:56.061717 gentoo_cache_manager-0.1.0/tests/commands/test_context.py
--rw-r--r--   0        0        0      646 2024-05-14 08:19:56.061717 gentoo_cache_manager-0.1.0/tests/commands/test_disable.py
--rw-r--r--   0        0        0     1888 2024-05-14 08:19:56.061717 gentoo_cache_manager-0.1.0/tests/commands/test_enable.py
--rw-r--r--   0        0        0     4055 2024-05-14 08:19:56.061717 gentoo_cache_manager-0.1.0/tests/commands/test_stats.py
--rw-r--r--   0        0        0     1415 2024-05-14 08:19:56.061717 gentoo_cache_manager-0.1.0/tests/commands/test_validators.py
--rw-r--r--   0        0        0       43 2024-05-14 08:19:56.061717 gentoo_cache_manager-0.1.0/tests/data/etc/portage/repos.conf
--rw-r--r--   0        0        0      182 2024-05-14 08:19:56.065718 gentoo_cache_manager-0.1.0/tests/data/repos/dummy/app-misc/bar/bar-1.0.ebuild
--rw-r--r--   0        0        0      182 2024-05-14 08:19:56.065718 gentoo_cache_manager-0.1.0/tests/data/repos/dummy/app-misc/foo/foo-1.0.ebuild
--rw-r--r--   0        0        0     1517 2024-05-14 08:19:56.065718 gentoo_cache_manager-0.1.0/tests/data/repos/dummy/licenses/MIT
--rw-r--r--   0        0        0       45 2024-05-14 08:19:56.065718 gentoo_cache_manager-0.1.0/tests/data/repos/dummy/metadata/layout.conf
--rw-r--r--   0        0        0      136 2024-05-14 08:19:56.065718 gentoo_cache_manager-0.1.0/tests/data/repos/dummy/metadata/md5-cache/app-misc/bar-1.0
--rw-r--r--   0        0        0       63 2024-05-14 08:19:56.065718 gentoo_cache_manager-0.1.0/tests/data/repos/dummy/metadata/md5-cache/app-misc/foo-1.0
--rw-r--r--   0        0        0      182 2024-05-14 08:19:56.065718 gentoo_cache_manager-0.1.0/tests/data/repos/dummy/net-misc/bar/bar-1.0.ebuild
--rw-r--r--   0        0        0       18 2024-05-14 08:19:56.065718 gentoo_cache_manager-0.1.0/tests/data/repos/dummy/profiles/categories
--rw-r--r--   0        0        0        7 2024-05-14 08:19:56.065718 gentoo_cache_manager-0.1.0/tests/data/repos/dummy/profiles/repo_name
--rw-r--r--   0        0        0     1137 2024-05-14 08:19:56.065718 gentoo_cache_manager-0.1.0/tests/test_cli.py
--rw-r--r--   0        0        0      331 2024-05-14 08:19:56.065718 gentoo_cache_manager-0.1.0/tests/test_init.py
--rw-r--r--   0        0        0     1041 2024-05-14 08:19:56.065718 gentoo_cache_manager-0.1.0/tests/test_utils.py
--rw-r--r--   0        0        0     2664 1970-01-01 00:00:00.000000 gentoo_cache_manager-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-15 11:11:05.431915 gentoo_cache_manager-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1417 2024-05-15 11:11:05.431915 gentoo_cache_manager-0.2.0/README.md
+-rw-r--r--   0        0        0     2232 2024-05-15 11:11:16.999969 gentoo_cache_manager-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      118 2024-05-15 11:11:05.431915 gentoo_cache_manager-0.2.0/src/gcm/__init__.py
+-rw-r--r--   0        0        0      239 2024-05-15 11:11:05.431915 gentoo_cache_manager-0.2.0/src/gcm/cli.py
+-rw-r--r--   0        0        0      177 2024-05-15 11:11:05.431915 gentoo_cache_manager-0.2.0/src/gcm/commands/__init__.py
+-rw-r--r--   0        0        0     2484 2024-05-15 11:11:05.431915 gentoo_cache_manager-0.2.0/src/gcm/commands/base.py
+-rw-r--r--   0        0        0     1468 2024-05-15 11:11:05.431915 gentoo_cache_manager-0.2.0/src/gcm/commands/clear.py
+-rw-r--r--   0        0        0      207 2024-05-15 11:11:05.431915 gentoo_cache_manager-0.2.0/src/gcm/commands/context.py
+-rw-r--r--   0        0        0      587 2024-05-15 11:11:05.431915 gentoo_cache_manager-0.2.0/src/gcm/commands/disable.py
+-rw-r--r--   0        0        0     2135 2024-05-15 11:11:05.431915 gentoo_cache_manager-0.2.0/src/gcm/commands/enable.py
+-rw-r--r--   0        0        0      125 2024-05-15 11:11:05.431915 gentoo_cache_manager-0.2.0/src/gcm/commands/exit_codes.py
+-rw-r--r--   0        0        0     2616 2024-05-15 11:11:05.431915 gentoo_cache_manager-0.2.0/src/gcm/commands/stats.py
+-rw-r--r--   0        0        0      874 2024-05-15 11:11:05.431915 gentoo_cache_manager-0.2.0/src/gcm/commands/validators.py
+-rw-r--r--   0        0        0      622 2024-05-15 11:11:05.431915 gentoo_cache_manager-0.2.0/src/gcm/utils.py
+-rw-r--r--   0        0        0        0 2024-05-15 11:11:05.431915 gentoo_cache_manager-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0       69 2024-05-15 11:11:05.431915 gentoo_cache_manager-0.2.0/tests/base.py
+-rw-r--r--   0        0        0        0 2024-05-15 11:11:05.431915 gentoo_cache_manager-0.2.0/tests/commands/__init__.py
+-rw-r--r--   0        0        0     3286 2024-05-15 11:11:05.431915 gentoo_cache_manager-0.2.0/tests/commands/test_base.py
+-rw-r--r--   0        0        0     2442 2024-05-15 11:11:05.431915 gentoo_cache_manager-0.2.0/tests/commands/test_clear.py
+-rw-r--r--   0        0        0      347 2024-05-15 11:11:05.431915 gentoo_cache_manager-0.2.0/tests/commands/test_context.py
+-rw-r--r--   0        0        0      646 2024-05-15 11:11:05.431915 gentoo_cache_manager-0.2.0/tests/commands/test_disable.py
+-rw-r--r--   0        0        0     1945 2024-05-15 11:11:05.431915 gentoo_cache_manager-0.2.0/tests/commands/test_enable.py
+-rw-r--r--   0        0        0     4311 2024-05-15 11:11:05.431915 gentoo_cache_manager-0.2.0/tests/commands/test_stats.py
+-rw-r--r--   0        0        0     1415 2024-05-15 11:11:05.431915 gentoo_cache_manager-0.2.0/tests/commands/test_validators.py
+-rw-r--r--   0        0        0       43 2024-05-15 11:11:05.435915 gentoo_cache_manager-0.2.0/tests/data/etc/portage/repos.conf
+-rw-r--r--   0        0        0      182 2024-05-15 11:11:05.435915 gentoo_cache_manager-0.2.0/tests/data/repos/dummy/app-misc/bar/bar-1.0.ebuild
+-rw-r--r--   0        0        0      182 2024-05-15 11:11:05.435915 gentoo_cache_manager-0.2.0/tests/data/repos/dummy/app-misc/foo/foo-1.0.ebuild
+-rw-r--r--   0        0        0     1517 2024-05-15 11:11:05.435915 gentoo_cache_manager-0.2.0/tests/data/repos/dummy/licenses/MIT
+-rw-r--r--   0        0        0       45 2024-05-15 11:11:05.435915 gentoo_cache_manager-0.2.0/tests/data/repos/dummy/metadata/layout.conf
+-rw-r--r--   0        0        0      136 2024-05-15 11:11:05.435915 gentoo_cache_manager-0.2.0/tests/data/repos/dummy/metadata/md5-cache/app-misc/bar-1.0
+-rw-r--r--   0        0        0       63 2024-05-15 11:11:05.435915 gentoo_cache_manager-0.2.0/tests/data/repos/dummy/metadata/md5-cache/app-misc/foo-1.0
+-rw-r--r--   0        0        0      182 2024-05-15 11:11:05.435915 gentoo_cache_manager-0.2.0/tests/data/repos/dummy/net-misc/bar/bar-1.0.ebuild
+-rw-r--r--   0        0        0       18 2024-05-15 11:11:05.435915 gentoo_cache_manager-0.2.0/tests/data/repos/dummy/profiles/categories
+-rw-r--r--   0        0        0        7 2024-05-15 11:11:05.435915 gentoo_cache_manager-0.2.0/tests/data/repos/dummy/profiles/repo_name
+-rw-r--r--   0        0        0     1110 2024-05-15 11:11:05.435915 gentoo_cache_manager-0.2.0/tests/test_cli.py
+-rw-r--r--   0        0        0      331 2024-05-15 11:11:05.435915 gentoo_cache_manager-0.2.0/tests/test_init.py
+-rw-r--r--   0        0        0     1041 2024-05-15 11:11:05.435915 gentoo_cache_manager-0.2.0/tests/test_utils.py
+-rw-r--r--   0        0        0     2664 1970-01-01 00:00:00.000000 gentoo_cache_manager-0.2.0/PKG-INFO
```

### Comparing `gentoo_cache_manager-0.1.0/LICENSE` & `gentoo_cache_manager-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gentoo_cache_manager-0.1.0/README.md` & `gentoo_cache_manager-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `gentoo_cache_manager-0.1.0/pyproject.toml` & `gentoo_cache_manager-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 readme = "README.md"
 keywords = [
     "gentoo",
     "cache",
     "manager",
     "ccache",
 ]
-version = "0.1.0"
+version = "0.2.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Repository = "https://github.com/Jamim/gentoo-cache-manager"
 Issues = "https://github.com/Jamim/gentoo-cache-manager/issues"
@@ -68,14 +68,17 @@
 ]
 test = [
     "pytest",
     "pytest-cov",
     "pytest-env",
 ]
 
+[tool.pdm.scripts]
+lint-ruff = "scripts/ruff"
+
 [tool.ruff]
 line-length = 79
 
 [tool.ruff.format]
 quote-style = "single"
 
 [tool.ruff.lint]
```

### Comparing `gentoo_cache_manager-0.1.0/src/gcm/commands/base.py` & `gentoo_cache_manager-0.2.0/src/gcm/commands/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 
 ENABLE_TEXT = '{package}\t{package}/ccache.env\n'
 DISABLE_TEXT = f'# {ENABLE_TEXT}'
 
 PACKAGE_NAME = pretty_name('{package}')
 
 
+def ccache_dir_env(package: str) -> dict[str, str]:
+    return {'CCACHE_DIR': str(CCACHE_DIR / package)}
+
+
 def get_package_env_path() -> Path:
     if not PACKAGE_ENV_PATH.exists():
         PACKAGE_ENV_PATH.mkdir()
     elif PACKAGE_ENV_PATH.is_file():
         return PACKAGE_ENV_PATH
 
     return PACKAGE_ENV_PATH / 'ccache'
@@ -56,17 +60,20 @@
     def callback(package: str) -> int | None:  # type: ignore[override]
         raise NotImplementedError
 
     def __init__(self) -> None:
         name = self.__class__.__name__.lower()
         click.BaseCommand.__init__(self, name)
 
-        self.params = [
+        params = list(self.params) if hasattr(self, 'params') else []
+        params.append(
             click.Argument(['package'], callback=validate_package_name)
-        ]
+        )
+
+        self.params = params
         self.help = self.__class__.__doc__
         self.epilog = None
         self.options_metavar = '[OPTIONS]'
         self.short_help = None
         self.add_help_option = True
         self.no_args_is_help = False
         self.hidden = False
```

### Comparing `gentoo_cache_manager-0.1.0/src/gcm/commands/disable.py` & `gentoo_cache_manager-0.2.0/src/gcm/commands/disable.py`

 * *Files identical despite different names*

### Comparing `gentoo_cache_manager-0.1.0/src/gcm/commands/enable.py` & `gentoo_cache_manager-0.2.0/src/gcm/commands/enable.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,23 @@
 
     See https://wiki.gentoo.org/wiki//etc/portage/package.env
     for better understanding.
     """
 
     INVOKE_MESSAGE = f'Enabling ccache for {PACKAGE_NAME}'
 
+    params = [
+        click.Option(
+            ['-m', '--max-size'],
+            default='1.0GiB',
+            show_default=True,
+            help='Maximum ccache size for a package.',
+        )
+    ]
+
     @staticmethod  # type: ignore[override]
     def callback(package: str, max_size: str) -> None:
         ensure_file(
             file_dir=CCACHE_DIR / package,
             file_name='ccache.conf',
             content=CCACHE_CONF.format(max_size=max_size),
         )
@@ -65,18 +74,7 @@
             file_name='ccache.env',
             content=ENV_CCACHE_CONF.format(package=package),
         )
         ensure_desired_env_line(
             desired=ENABLE_TEXT.format(package=package),
             undesired=DISABLE_TEXT.format(package=package),
         )
-
-    def __init__(self) -> None:
-        super().__init__()
-        self.params.append(
-            click.Option(
-                ['-m', '--max-size'],
-                default='1.0GiB',
-                show_default=True,
-                help='Maximum ccache size for a package.',
-            )
-        )
```

### Comparing `gentoo_cache_manager-0.1.0/src/gcm/commands/stats.py` & `gentoo_cache_manager-0.2.0/src/gcm/commands/stats.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import io
 import re
 import subprocess
 
 import click
 
 from ..utils import warn
-from .base import CCACHE_DIR, PACKAGE_NAME, Command
+from .base import PACKAGE_NAME, Command, ccache_dir_env
 from .exit_codes import CCACHE_BINARY_NOT_FOUND, OK
 
 COLORS = {
     'Cacheable calls': ('yellow', 'magenta'),
     'Hits': ('green', 'yellow'),
     'Direct': ('bright_green', 'green'),
     'Preprocessed': ('bright_green', 'green'),
@@ -46,15 +46,15 @@
     return DATA_TEMPLATE.format(**values)
 
 
 def show_stats(package: str) -> int:
     try:
         stdout: io.TextIOWrapper = subprocess.Popen(
             ['ccache', '-s'],
-            env={'CCACHE_DIR': CCACHE_DIR / package},
+            env=ccache_dir_env(package),
             stdout=subprocess.PIPE,
             text=True,
         ).stdout  # type: ignore[assignment]
     except FileNotFoundError:
         warn('Unable to show stats due to missing ccache binary')
         return CCACHE_BINARY_NOT_FOUND
```

### Comparing `gentoo_cache_manager-0.1.0/src/gcm/commands/validators.py` & `gentoo_cache_manager-0.2.0/src/gcm/commands/validators.py`

 * *Files identical despite different names*

### Comparing `gentoo_cache_manager-0.1.0/src/gcm/utils.py` & `gentoo_cache_manager-0.2.0/src/gcm/utils.py`

 * *Files identical despite different names*

### Comparing `gentoo_cache_manager-0.1.0/tests/commands/test_base.py` & `gentoo_cache_manager-0.2.0/tests/commands/test_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 import io
-from unittest.mock import call, patch
+from unittest.mock import patch
 
 import pytest
+from click.testing import CliRunner
 
 from gcm.commands.base import (
+    CCACHE_DIR,
     PACKAGE_NAME,
     Command,
+    ccache_dir_env,
     ensure_desired_env_line,
     get_package_env_path,
 )
 
+from ..base import ABORTED, DONE
+
 DUMMY_ENV = """# foo
 bar
 # foo
 # baz
 """
 
 
+def test_ccache_dir_env():
+    package = 'app-misc/foo'
+    env = ccache_dir_env(package)
+    assert env == {'CCACHE_DIR': str(CCACHE_DIR / package)}
+
+
 @pytest.mark.parametrize(
     'exists,is_file',
     (
         (True, True),
         (True, False),
         (False, None),
     ),
@@ -92,21 +103,26 @@
     INVOKE_MESSAGE = f'Doing nothing with {PACKAGE_NAME}'
 
     callback_is_called = False
 
     def callback(self, package):
         self.callback_is_called = True
         assert package == 'app-misc/foo'
+        return self.exit_code
+
+    def __init__(self, exit_code=0) -> None:
+        super().__init__()
+        self.exit_code = exit_code
+
+
+OUTPUT = 'Doing nothing with \x1b[32m\x1b[1mapp-misc/foo\x1b[0m\n{}\n'
 
 
-@patch('click.echo')
-def test_command_invoke(echo):
-    command = DummyCommand()
+@pytest.mark.parametrize('exit_code,outcome', ((0, DONE), (1, ABORTED)))
+def test_command_invoke(exit_code, outcome):
+    command = DummyCommand(exit_code)
 
-    with pytest.raises(SystemExit):
-        command(['foo'])
+    result = CliRunner().invoke(command, ['foo'], color=True)
 
     assert command.callback_is_called
-    assert echo.call_args_list == [
-        call('Doing nothing with \x1b[32m\x1b[1mapp-misc/foo\x1b[0m'),
-        call('\x1b[32mDone :-)\x1b[0m'),
-    ]
+    assert result.exit_code == exit_code
+    assert result.output == OUTPUT.format(outcome)
```

### Comparing `gentoo_cache_manager-0.1.0/tests/commands/test_disable.py` & `gentoo_cache_manager-0.2.0/tests/commands/test_disable.py`

 * *Files identical despite different names*

### Comparing `gentoo_cache_manager-0.1.0/tests/commands/test_enable.py` & `gentoo_cache_manager-0.2.0/tests/commands/test_enable.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from unittest.mock import MagicMock, call, patch
 
 import pytest
+from click.testing import CliRunner
 
 from gcm.commands.base import CCACHE_DIR, DISABLE_TEXT, ENABLE_TEXT, ENV_DIR
 from gcm.commands.enable import (
     CCACHE_CONF,
     ENV_CCACHE_CONF,
     Enable,
     ensure_file,
 )
 
+from ..base import DONE
+
 
 def test_ensure_file():
     file_dir = MagicMock()
     file_name = 'dummy.txt'
     content = 'Lorem ipsum dolor sit amet'
 
     ensure_file(file_dir, file_name, content)
@@ -25,31 +28,29 @@
     file_path.open.assert_called_once_with('w')
 
     out = file_path.open.return_value.__enter__.return_value
     out.write.assert_called_once_with(content)
 
 
 @pytest.mark.parametrize('max_size', ('512MiB', '2.0G', None))
-@patch('click.echo')
 @patch('gcm.commands.enable.ensure_desired_env_line')
 @patch('gcm.commands.enable.ensure_file')
-def test_disable(ensure_file, ensure_desired_env_line, echo, max_size):
-    command = Enable()
+def test_enable(ensure_file, ensure_desired_env_line, max_size):
     if max_size:
         args = ['foo', '--max-size', max_size]
     else:
         args = ['foo']
         max_size = '1.0GiB'
 
-    with pytest.raises(SystemExit):
-        command(args)
+    result = CliRunner().invoke(Enable(), args, color=True)
 
     package = 'app-misc/foo'
-    echo.assert_any_call(
-        'Enabling ccache for \x1b[32m\x1b[1mapp-misc/foo\x1b[0m'
+    assert result.exit_code == 0
+    assert result.output == (
+        f'Enabling ccache for \x1b[32m\x1b[1m{package}\x1b[0m\n{DONE}\n'
     )
     assert ensure_file.call_args_list == [
         call(
             file_dir=CCACHE_DIR / package,
             file_name='ccache.conf',
             content=CCACHE_CONF.format(max_size=max_size),
         ),
```

### Comparing `gentoo_cache_manager-0.1.0/tests/commands/test_stats.py` & `gentoo_cache_manager-0.2.0/tests/commands/test_stats.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+import subprocess
 from unittest.mock import patch
 
 import pytest
 from click.testing import CliRunner
 
+from gcm.commands.base import ccache_dir_env
 from gcm.commands.exit_codes import CCACHE_BINARY_NOT_FOUND
 from gcm.commands.stats import Stats
 
 MODERN_STATS = """Cacheable calls:   101 / 235 (42.98%)
   Hits:              8 / 101 ( 7.92%)
     Direct:          6 /   8 (75.00%)
     Preprocessed:    2 /   8 (25.00%)
@@ -80,23 +82,30 @@
 def test_stats_ok(popen, stats, output):
     popen.return_value.stdout.readlines.return_value = [
         f'{line}\n' for line in stats.split('\n')
     ]
 
     result = CliRunner().invoke(Stats(), ['foo'], color=True)
 
+    popen.assert_called_once_with(
+        ['ccache', '-s'],
+        env=ccache_dir_env('app-misc/foo'),
+        stdout=subprocess.PIPE,
+        text=True,
+    )
     assert result.exit_code == 0
     assert result.output == output
 
 
 NO_CCACHE_OUTPUT = """Showing ccache stats for \x1b[32m\x1b[1mapp-misc/foo\x1b[0m
 \x1b[33mUnable to show stats due to missing ccache binary\x1b[0m
 \x1b[31mAborted!\x1b[0m
 """  # noqa: E501
 
 
 @patch('subprocess.Popen', side_effect=FileNotFoundError)
 def test_stats_no_ccache(popen):
     result = CliRunner().invoke(Stats(), ['foo'], color=True)
 
+    popen.assert_called_once()
     assert result.exit_code == CCACHE_BINARY_NOT_FOUND
     assert result.output == NO_CCACHE_OUTPUT
```

### Comparing `gentoo_cache_manager-0.1.0/tests/commands/test_validators.py` & `gentoo_cache_manager-0.2.0/tests/commands/test_validators.py`

 * *Files identical despite different names*

### Comparing `gentoo_cache_manager-0.1.0/tests/data/repos/dummy/licenses/MIT` & `gentoo_cache_manager-0.2.0/tests/data/repos/dummy/licenses/MIT`

 * *Files identical despite different names*

### Comparing `gentoo_cache_manager-0.1.0/tests/test_cli.py` & `gentoo_cache_manager-0.2.0/tests/test_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 
 import pytest
 from click.testing import CliRunner
 
 import gcm
 from gcm.cli import cli
 
+from .base import ABORTED, DONE
+
 
 @pytest.mark.parametrize(
     'exit_code,outcome',
     (
-        (None, call('\x1b[32mDone :-)\x1b[0m')),
-        (0, call('\x1b[32mDone :-)\x1b[0m')),
-        (1, call('\x1b[31mAborted!\x1b[0m', err=True)),
+        (None, call(DONE)),
+        (0, call(DONE)),
+        (1, call(ABORTED, err=True)),
     ),
 )
 @patch.dict(sys.modules)
 @patch('sys.argv', ['gcm', 'enable', 'foo'])
 @patch('click.echo')
 @patch('gcm.commands.enable.Enable.callback')
 def test_main(callback, echo, exit_code, outcome):
```

### Comparing `gentoo_cache_manager-0.1.0/tests/test_utils.py` & `gentoo_cache_manager-0.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gentoo_cache_manager-0.1.0/PKG-INFO` & `gentoo_cache_manager-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gentoo-cache-manager
-Version: 0.1.0
+Version: 0.2.0
 Summary: 🗃️ Helps tweaking build cache settings for individual packages
 Keywords: gentoo,cache,manager,ccache
 Author-Email: Aliaksei Urbanski <aliaksei.urbanski@gmail.com>
 Maintainer-Email: Aliaksei Urbanski <aliaksei.urbanski@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
```

