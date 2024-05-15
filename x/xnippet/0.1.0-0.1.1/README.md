# Comparing `tmp/xnippet-0.1.0.tar.gz` & `tmp/xnippet-0.1.1.tar.gz`

## Comparing `xnippet-0.1.0.tar` & `xnippet-0.1.1.tar`

### file list

```diff
@@ -1,52 +1,36 @@
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 xnippet-0.1.0/pytest.ini
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 xnippet-0.1.0/examples/example_config.yaml
--rw-r--r--   0        0        0     3258 2020-02-02 00:00:00.000000 xnippet-0.1.0/examples/docs/PLUGIN.md
--rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 xnippet-0.1.0/examples/docs/PRESET.md
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 xnippet-0.1.0/examples/docs/PROJECT_CONFIG.md
--rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 xnippet-0.1.0/examples/docs/RECIPE.md
--rw-r--r--   0        0        0     3554 2020-02-02 00:00:00.000000 xnippet-0.1.0/examples/docs/SPEC.md
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 xnippet-0.1.0/examples/plugin/plugin_example/manifest.yaml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 xnippet-0.1.0/examples/plugin/plugin_example/plugin_example.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 xnippet-0.1.0/examples/plugin/plugin_example/utils.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 xnippet-0.1.0/examples/plugin/plugin_example/preset/preset_snippet.yaml
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 xnippet-0.1.0/examples/plugin/plugin_example/recipe/recipe_snippet.yaml
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 xnippet-0.1.0/examples/plugin/plugin_example/spec/spec_snippet.yaml
--rw-r--r--   0        0        0     3413 2020-02-02 00:00:00.000000 xnippet-0.1.0/tests/01_main_test.py
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 xnippet-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 xnippet-0.1.0/xnippet/__init__.py
--rw-r--r--   0        0        0    10198 2020-02-02 00:00:00.000000 xnippet-0.1.0/xnippet/main.py
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 xnippet-0.1.0/xnippet/types.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 xnippet-0.1.0/xnippet/fetcher/__init__.py
--rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 xnippet-0.1.0/xnippet/fetcher/base.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 xnippet-0.1.0/xnippet/fetcher/plugins.py
--rw-r--r--   0        0        0     7949 2020-02-02 00:00:00.000000 xnippet-0.1.0/xnippet/fetcher/snippets.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 xnippet-0.1.0/xnippet/formatter/__init__.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 xnippet-0.1.0/xnippet/formatter/bytes.py
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 xnippet-0.1.0/xnippet/formatter/datetime.py
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 xnippet-0.1.0/xnippet/formatter/io.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 xnippet-0.1.0/xnippet/formatter/path.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 xnippet-0.1.0/xnippet/formatter/string.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 xnippet-0.1.0/xnippet/module/__init__.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 xnippet-0.1.0/xnippet/module/commander.py
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 xnippet-0.1.0/xnippet/module/installer.py
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 xnippet-0.1.0/xnippet/module/loader.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 xnippet-0.1.0/xnippet/parser/__init__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 xnippet-0.1.0/xnippet/parser/classifier.py
--rw-r--r--   0        0        0     4730 2020-02-02 00:00:00.000000 xnippet-0.1.0/xnippet/parser/recipe.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 xnippet-0.1.0/xnippet/raiser/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xnippet-0.1.0/xnippet/raiser/error.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xnippet-0.1.0/xnippet/raiser/except.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 xnippet-0.1.0/xnippet/raiser/types.py
--rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 xnippet-0.1.0/xnippet/raiser/warn.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 xnippet-0.1.0/xnippet/snippet/__init__.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 xnippet-0.1.0/xnippet/snippet/base.py
--rw-r--r--   0        0        0    11279 2020-02-02 00:00:00.000000 xnippet-0.1.0/xnippet/snippet/plugin.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 xnippet-0.1.0/xnippet/snippet/preset.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 xnippet-0.1.0/xnippet/snippet/recipe.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 xnippet-0.1.0/xnippet/snippet/spec.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 xnippet-0.1.0/xnippet/yaml/config.yaml
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 xnippet-0.1.0/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 xnippet-0.1.0/LICENSE
--rw-r--r--   0        0        0     4093 2020-02-02 00:00:00.000000 xnippet-0.1.0/README.md
--rwxr-xr-x   0        0        0     1338 2020-02-02 00:00:00.000000 xnippet-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5286 2020-02-02 00:00:00.000000 xnippet-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 xnippet-0.1.1/src/xnippet/__init__.py
+-rw-r--r--   0        0        0    12381 2020-02-02 00:00:00.000000 xnippet-0.1.1/src/xnippet/manager.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 xnippet-0.1.1/src/xnippet/types.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 xnippet-0.1.1/src/xnippet/config/__init__.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 xnippet-0.1.1/src/xnippet/config/logging.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 xnippet-0.1.1/src/xnippet/config/main.yaml
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 xnippet-0.1.1/src/xnippet/fetcher/__init__.py
+-rw-r--r--   0        0        0     9939 2020-02-02 00:00:00.000000 xnippet-0.1.1/src/xnippet/fetcher/base.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 xnippet-0.1.1/src/xnippet/fetcher/plugins.py
+-rw-r--r--   0        0        0     8039 2020-02-02 00:00:00.000000 xnippet-0.1.1/src/xnippet/fetcher/snippets.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 xnippet-0.1.1/src/xnippet/formatter/__init__.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 xnippet-0.1.1/src/xnippet/formatter/bytes.py
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 xnippet-0.1.1/src/xnippet/formatter/datetime.py
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 xnippet-0.1.1/src/xnippet/formatter/io.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 xnippet-0.1.1/src/xnippet/formatter/path.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 xnippet-0.1.1/src/xnippet/formatter/string.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 xnippet-0.1.1/src/xnippet/formatter/version/LICENSE
+-rw-r--r--   0        0        0    10173 2020-02-02 00:00:00.000000 xnippet-0.1.1/src/xnippet/formatter/version/LICENSE.APACHE
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 xnippet-0.1.1/src/xnippet/formatter/version/LICENSE.BSD
+-rw-r--r--   0        0        0    17501 2020-02-02 00:00:00.000000 xnippet-0.1.1/src/xnippet/formatter/version/__init__.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 xnippet-0.1.1/src/xnippet/module/__init__.py
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 xnippet-0.1.1/src/xnippet/module/installer.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 xnippet-0.1.1/src/xnippet/module/loader.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 xnippet-0.1.1/src/xnippet/raiser/__init__.py
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 xnippet-0.1.1/src/xnippet/raiser/types.py
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 xnippet-0.1.1/src/xnippet/raiser/warn.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 xnippet-0.1.1/src/xnippet/snippet/__init__.py
+-rw-r--r--   0        0        0    12431 2020-02-02 00:00:00.000000 xnippet-0.1.1/src/xnippet/snippet/plugin.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 xnippet-0.1.1/src/xnippet/snippet/simple.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 xnippet-0.1.1/src/xnippet/utils/__init__.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 xnippet-0.1.1/src/xnippet/utils/timer.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 xnippet-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 xnippet-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 xnippet-0.1.1/README.md
+-rwxr-xr-x   0        0        0     1515 2020-02-02 00:00:00.000000 xnippet-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 xnippet-0.1.1/PKG-INFO
```

### Comparing `xnippet-0.1.0/xnippet/main.py` & `xnippet-0.1.1/src/xnippet/manager.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,92 +2,120 @@
 
 This module facilitates the management of configuration settings within the application, 
 allowing configurations to be handled internally without file creation unless specifically 
 requested by the user through CLI to create them in the home folder.
 """
 
 from __future__ import annotations
+import logging
 import yaml
 import shutil
-from packaging import version
 from pathlib import Path
 from .fetcher import PlugInFetcher
 from typing import TYPE_CHECKING
 from .formatter import PathFormatter
 from .formatter import IOFormatter
+from .formatter import version
 from .raiser import WarnRaiser
 if TYPE_CHECKING:
     from .types import SnippetMode, StorageMode, SnippetPath, PlugInSnippetType
     from .types import PlugInFetcherType, VersionType
     from typing import List, Union, Optional
+    from logging import Logger
+    
 
 class Manager(PathFormatter):
     """Manages the configuration settings for the application.
 
     This class ensures the existence of the configuration directory, loads or creates the configuration file,
     sets configuration values, and retrieves configuration values. It operates both globally and locally
     depending on the user's choice and the operational context.
     """ 
     config: dict = {}
     _home_dir: 'Path'
-    _default_dir: 'Path'
+    _package_dir: 'Path'
     _local_dir: 'Path'
     _global_dir: 'Path'
     _config_dir: 'Path'
     _fname: str
     _package_name: str
     _package_version: VersionType
     _fetcher: PlugInFetcherType
     _compatible_snippets: List[SnippetMode] = ['plugin']
+    _logger: Logger = logging.getLogger(__name__)
     
     def __init__(self, 
                  package_name: str, 
-                 package_version: str, 
+                 package_version: str,
                  package__file__: Union['Path', str],
                  config_path: Optional[str] = None,
                  config_filename: str = 'config.yaml') -> None:
         """Initializes the configuration manager.
 
         This constructor sets up paths for the home directory, global and local configuration directories,
         and configuration file. It ensures the configuration directory exists and loads or creates the
         configuration based on its presence.
 
         Args:
             tmpdir (Optional[Path]): Temporary directory for storing configurations, defaults to the home directory.
         """
         self._package_name = package_name
         self._home_dir = self._resolve('~')
-        self._default_dir = self._resolve(package__file__).parent / config_path if config_path else self._resolve(package__file__).parent
+        self._package_dir = self._resolve(package__file__).parent / config_path if config_path else self._resolve(package__file__).parent
         self._local_dir = self._resolve(Path.cwd() / f'.{self._package_name}')
         self._global_dir = self._resolve(self._home_dir / f'.{self._package_name}')
         self._fname = config_filename
         self._package_version = version.parse(package_version)
         self.reload()
 
     ## Initiation step
     def reload(self) -> None:
         """Loads an existing configuration file or creates a new one if it does not exist, filling the 'config' dictionary with settings."""
         self._set_config_dir()
         config_file = self.config_dir / self._fname
-        if not config_file.exists() and self.config_dir == self._default_dir:
-            
-            comment = "Preparing default configuration. Use 'create_config' method to initialize."
-            WarnRaiser(self.reload).config_not_found(self.config_dir, comment=comment)
-            config_file = self._resolve(__file__).parent / 'yaml/config.yaml'
+        if not config_file.exists() and self.config_dir == self._package_dir:
+            WarnRaiser(self.reload).config_file(self.config_dir, 
+                                                exists=False, 
+                                                comment="Import xnippet's default config file.")
+            config_file = self._resolve(__file__).parent / 'config/main.yaml'
         with open(config_file, 'r') as f:
             self.config = yaml.safe_load(f)
+            self._logger.debug("Configuration imported from: %s", config_file)
         self._reload_plugin_fetcher()
-        
+    
     def _set_config_dir(self):
+        """Sets the configuration directory based on the existence and type of configuration files.
+
+        This method determines the appropriate configuration directory by checking the type and presence of configuration files.
+        If both local and global configuration files exist (indicated by a list), the local directory is used.
+        If only one type of configuration file exists (indicated by a string), the directory is set based on the type ('local' or 'global').
+        If no configuration files exist, a warning is issued, and the default configuration directory is used.
+
+        Attributes:
+            config_created: Can be a list, string, or None. A list indicates both local and global configurations are available,
+                            a string indicates only one configuration is available, and None indicates no configurations are found.
+        
+        Side Effects:
+            Sets self._config_dir to the appropriate directory based on the existing configuration.
+            Logs debug messages about the configuration status and actions taken.
+            Raises a warning if no configuration files are found, advising the creation of a configuration file.
+
+        Raises:
+            WarnRaiser: If no configuration file exists, this raises a configurable warning through the WarnRaiser class.
+        """
         if isinstance(self.config_created, list):
+            self._logger.debug("Config folders have been created for both %s and %s exist.", *self.config_created)
             self._config_dir = self._local_dir
         elif isinstance(self.config_created, str):
+            self._logger.debug("The '%s' config folder has been created.", self.config_created.capitalize())
             self._config_dir = self._local_dir if self.config_created == 'local' else self._global_dir
         else:
-            self._config_dir = self._default_dir
+            self._logger.debug("Config folder was not created, "
+                               "using package directory (%s) and search config file.", self._package_dir)
+            self._config_dir = self._package_dir
 
     def _reload_plugin_fetcher(self) -> None:
         """Retrieves a configured SnippetsFetcher for the specified mode to handle fetching of snippets.
 
         Args:
             mode (str): The mode that determines which type of fetcher to return. Valid modes are 'plugin', 'preset', 'spec', and 'recipe'.
 
@@ -133,15 +161,17 @@
             bool: Returns True if the file was successfully created, otherwise False.
         """
         config_dir = self._local_dir if target == 'local' else self._global_dir
         config_dir.mkdir(exist_ok=True)
         config_file = config_dir / self._fname
         if config_file.exists():
             if not force:
-                WarnRaiser(self.create_config).config_exist_when_create()
+                WarnRaiser(self.create_config).config_file(config_dir=config_dir, 
+                                                           exists=True, 
+                                                           comment="Use the force option to overwrite.")
                 return False
         with open(config_file, 'w') as f:
             yaml.safe_dump(self.config, f, sort_keys=False)
         self.reload()
     
     def delete_config(self, target: StorageMode, yes: bool = False):
         path = self._local_dir if target == 'local' else self._global_dir
@@ -199,22 +229,22 @@
     def is_installed(self, plugin_name: str, version: Optional[str] = None):
         return True if self.get(plugin_name, version) else False
     
     def install(self, plugin_name: str, 
                 plugin_version: Optional[str] = None, 
                 yes: bool = False, target: StorageMode = 'local'):
         if not self.config_created:
-            WarnRaiser(self.install).config_not_found(self.config_dir)
-            if yes or IOFormatter.yes_or_no(f"Do you want to proceed creating '{target}' configuration?"):
+            WarnRaiser(self.install).config_file(self.config_dir, exists=False)
+            if yes or IOFormatter.ask_yes_or_no(f"Do you want to proceed creating '{target}' configuration?"):
                 self.create_config(target=target)
         
         plugin = self.get(plugin_name=plugin_name, plugin_version=plugin_version, remote=True)
         plugin_dir, _ = self._check_dir()
         plugin_name = f'{plugin_name}_{plugin_version}' if plugin_name else plugin_name
         if (plugin_dir / plugin_name).exists():
-            WarnRaiser(self.install).file_exist()
-            if yes or IOFormatter.yes_or_no(f"Do you want to overwrite plugin '{target}' configuration?"):
+            WarnRaiser(self.install).config_file(self.config_dir, exists=True)
+            if yes or IOFormatter.ask_yes_or_no(f"Do you want to overwrite plugin '{target}' configuration?"):
                 plugin.download(dest=plugin_dir, force=yes)
                 return True
             return False
         plugin.download(dest=plugin_dir)
         self.reload()
```

### Comparing `xnippet-0.1.0/xnippet/types.py` & `xnippet-0.1.1/src/xnippet/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,45 @@
 from typing import Type, Optional, Union
 from typing import Literal, Tuple, List
 from pathlib import Path
-from .main import Manager
-from .fetcher import SnippetFetcher
+from .manager import Manager
+from .fetcher import SnippetsFetcher
 from .fetcher import PlugInFetcher
 from .fetcher.base import Fetcher
-from .snippet.base import Snippet
+from .snippet import SimpleSnippet
 from .snippet import PlugInSnippet
-from .snippet import PresetSnippet
-from .snippet import RecipeSnippet
-from .snippet import SpecSnippet
 from packaging.version import _Version as VersionType
 
 class Resource:
     def to_dict(self):
         return self.__dict__
 
 ResourceType = Type[Union[Resource, List[Resource]]]
 
 XnippetManagerType = Type[Manager]
 
 StorageMode = Literal['local', 'global']
 
 FetcherType = Type[Fetcher]
 
-SnippetsFetcherType = Type[SnippetFetcher]
+SnippetsFetcherType = Type[SnippetsFetcher]
 
 PlugInFetcherType = Type[PlugInFetcher]
 
-SnippetType = Type[Snippet]
-
 SnippetPath = Tuple[Optional[Path], bool]
 
 SnippetMode = Literal[
     'plugin', 'preset', 'spec', 'recipe'
     ]
 
-PlugInSnippetType = Type[PlugInSnippet]
-
-PresetSnippetType = Type[PresetSnippet]
+SimpleSnippetType = Type[SimpleSnippet]
 
-RecipeSnippetType = Type[RecipeSnippet]
+PlugInSnippetType = Type[PlugInSnippet]
 
-SpecSnippetType = Type[SpecSnippet]
 
 __all__ = [
     'ResourceType', 'VersionType',
     'XnippetManagerType', 'StorageMode',
-    'FetcherType', 'SnippetsFetcherType', 'PlugInFetcherType',
-    'SnippetType', 'SnippetPath', 'SnippetMode',
+    'FetcherType', 'SnippetsFetcherType', 'PlugInFetcherType', 'SnippetPath', 'SnippetMode',
+    'SimpleSnippetType', 
     'PlugInSnippetType', 
-    'PresetSnippetType', 
-    'RecipeSnippetType', 
-    'SpecSnippetType',
     ]
```

### Comparing `xnippet-0.1.0/xnippet/fetcher/__init__.py` & `xnippet-0.1.1/src/xnippet/fetcher/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,11 +5,12 @@
 
 Exposes:
     SnippetsFetcher: A class derived from the Snippets module, tailored to handle the fetching,
                      storage, and synchronization of code snippets or configurations from
                      designated sources.
 """
 
-from .snippets import Snippets as SnippetFetcher
+from .base import Fetcher as BaseFetcher
+from .snippets import Snippets as SnippetsFetcher
 from .plugins import PlugIns as PlugInFetcher
 
-__all__ = ['SnippetFetcher', 'PlugInFetcher']
+__all__ = ['BaseFetcher', 'SnippetsFetcher', 'PlugInFetcher']
```

### Comparing `xnippet-0.1.0/xnippet/fetcher/base.py` & `xnippet-0.1.1/src/xnippet/fetcher/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,22 +7,24 @@
 
 Classes:
     Fetcher: A base class for fetching content from remote repositories with GitHub API integration.
 """
 
 from __future__ import annotations
 import re
+import logging
 import warnings
 import requests
 from xnippet.formatter import PathFormatter
+from xnippet.raiser import WarnRaiser
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from typing import Optional, Union
     from typing import List, Tuple, Generator
-
+    from logging import Logger
 
 class Fetcher(PathFormatter):
     """Base class for fetching remote content with methods to authenticate and navigate repositories.
 
     The Fetcher class extends the functionality of PathResolver to include methods that handle
     the authentication and retrieval of data from remote GitHub repositories. It provides
     utilities to walk through repository directories, fetch file and directory contents,
@@ -30,27 +32,29 @@
 
     Attributes:
         _auth (Union[List[Tuple[str, str]], Tuple[str, str]]): Authentication credentials for the repository.
         repos (dict): Configuration for the repositories to be accessed.
     """
     _auth: Union[List[Tuple[str, str]], Tuple[str, str]]
     _repos: dict
+    _logger: Logger = logging.getLogger(__name__)
     
     @staticmethod
     def is_connected():
         """Check if there is an internet connection available by pinging a known URL.
 
         Returns:
             bool: True if the connection is successful, False otherwise.
         """
         try:
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore", UserWarning)
                 Fetcher._fetch_from_url("https://api.github.com") # this will get status code 403
-        except (requests.ConnectTimeout, requests.ConnectionError, requests.RequestException):
+        except (requests.ConnectTimeout, requests.ConnectionError, requests.RequestException) as e:
+            WarnRaiser(Fetcher.is_connected).connection_failed(comment=e)
             return False
         return True
     
     def _set_auth(self):
         """Set up authentication credentials for accessing configured repositories.
 
         Extracts and sets authentication details for each repository from the provided configurations.
@@ -71,41 +75,45 @@
         if 'auth' in repo_dict:
             username = repo_dict['auth']['username']
             token = repo_dict['auth']['token']
             return (username, token) if username and token else None
         return None
     
     @staticmethod
-    def _walk_github_repo(repo_url: dict, path: Optional['str'] = None, auth: Tuple[str, str] = None):
+    def _walk_github_repo(repo_url: dict, path: Optional['str'] = None, auth: Optional[Tuple[str, str]] = None):
         """Recursively walk through directories in a GitHub repository to fetch directory and file structure.
 
         Args:
             repo_url (dict): URL of the GitHub repository.
             path (Optional[str]): Specific path in the repository to start the walk.
             auth (Tuple[str, str]): Authentication credentials for accessing the repository.
 
         Yields:
             dict: A dictionary containing 'path', 'dirs', and 'files' with their respective URLs.
         """
+        Fetcher._logger.debug(" + Entered to Fetcher._walk_github_repo")
+        Fetcher._logger.debug(" - repo_url: %s. path: %s, auth=%s", repo_url, path, True if auth else False)
         base_url = Fetcher._decode_github_repo(repo_url=repo_url, path=path)
         return Fetcher._walk_dir(url=base_url, auth=auth)
     
     @staticmethod
-    def _walk_dir(url, path='', auth: Tuple[str, str] = None):
+    def _walk_dir(url, path='', auth: Optional[Tuple[str, str]] = None):
         """Walk through a specific directory in a repository.
 
         Args:
             url (str): URL of the directory to walk through.
             path (str): Path relative to the repository root.
             auth (Tuple[str, str]): Authentication credentials for accessing the repository.
 
         Yields:
             dict: A dictionary containing the path, directories, and files within the directory.
         """
+        Fetcher._logger.debug(" + Entered to Fetcher._walk_dir_repo, auth=%s", True if auth else False)
         if contents := Fetcher._fetch_from_url(url=url, auth=auth):
+            Fetcher._logger.debug(" - Fetched contents from url: %s", url)
             dirs, files = Fetcher._fetch_directory_contents(contents.json())
             yield {'path':path, 
                     'dirs':{d['name']:d['url'] for d in dirs}, 
                     'files':{f['name']:f['download_url'] for f in files}}
 
             for dir in dirs:
                 new_path = f"{path}/{dir['name']}" if path else dir['name']
@@ -118,20 +126,24 @@
 
         Args:
             contents (list): List of contents from a directory.
 
         Returns:
             tuple: A tuple containing lists of directories and files.
         """
+        logger = Fetcher._logger
+        logger.debug(" + Fetching contents in directory, and classify them into dirs and files")
         dirs, files = [], []
         for item in contents:
             if item['type'] == 'dir':
                 dirs.append(item)
             elif item['type'] == 'file':
                 files.append(item)
+            logger.debug("  + itemName: %s, type: %s", item['name'], item['type'])
+        logger.debug("  :: dirs: %s, files: %s", [d['name'] for d in dirs], [f['name'] for f in files])
         return dirs, files
     
     @staticmethod
     def _decode_github_repo(repo_url: dict, path: Optional['str'] = None):
         """Decode a GitHub repository URL to construct an API endpoint URL.
 
         Args:
@@ -139,58 +151,69 @@
             path (Optional[str]): An optional path within the repository.
 
         Returns:
             str: A constructed API endpoint URL based on the repository details.
         """
         ptrn_github = r'https://(?:[^/]+\.)?github\.com/(?P<owner>[^/]+)/(?P<repo>[^/.]+)(?:\.git)?(?:/(?P<path>.*))?'
         if matched := re.match(ptrn_github, repo_url):
+            Fetcher._logger.debug(" + Repo URL pattern matched: %s", matched)
             owner = matched['owner']
             repo = matched['repo']
             if matched['path']:
                 path_ = matched['path']
                 path = '/'.join([path_, path]) if path_ else path
             url = f"https://api.github.com/repos/{owner}/{repo}/contents"
+            Fetcher._logger.debug(" - Decoded URL: %s", url)
             return f"{url}/{path}" if path else url
+        Fetcher._logger.debug(" + Repo URL pattern does not match: %s", repo_url)
     
     @staticmethod
     def _fetch_from_url(url: str, auth: Tuple[str, str] = None) -> Optional[requests.Response]:
         """Fetch data from a given URL using optional authentication.
 
         Args:
             url (str): The URL from which to fetch data.
             auth (Tuple[str, str]): Optional authentication credentials.
 
         Returns:
             Optional[requests.Response]: The response object if successful, otherwise None.
         """
+        Fetcher._logger.debug(" + Sending request to %s", url)
         response = requests.get(url, auth=auth)
+        Fetcher._logger.debug(" - Request Status Code: %s", response.status_code)
         if response.status_code == 200:
+            Fetcher._logger.debug(" - Returning response object.")
             return response
         else:
-            warnings.warn(f"Failed to retrieve contents: {response.status_code}.", UserWarning)
+            warner = WarnRaiser(Fetcher._fetch_from_url)
+            comment = [f"Status Code: {response.status_code}"]
             if response.status_code == 403:
-                warnings.warn(f"It potentially due to incorect repo address or exceed limit of request."
-                              " Try use API token for giigle", UserWarning)
-            
+                comment.append("This may be due to an incorrect repository address or exceeding the request limit. "
+                               "Consider using an API token for authentication.")
+                warner.data_fetch_failed(comment=' '.join(comment))
+            Fetcher._logger.debug(" - Returning 'None'.")
             return None
 
     @staticmethod
-    def _download_buffer(url: dict,
+    def _download_buffer(url: str,
                          chunk_size: int = 8192,
-                         auth: Tuple[str, str] = None) -> Union[Generator, bool]:
+                         auth: Optional[Tuple[str, str]] = None) -> Union[Generator, bool]:
         """Download file content from a URL in buffered chunks.
 
         Args:
-            url (dict): The URL of the file to download.
+            url (str): The URL of the file to download.
             chunk_size (int): The size of each chunk in bytes.
             auth (Tuple[str, str]): Optional authentication credentials.
 
         Returns:
             Union[Generator, bool]: A generator yielding file chunks if successful, False on error.
         """
         try:
+            Fetcher._logger.debug(" + Downloading %s [ChunkSize: %s ;auth=%s]", url, chunk_size, True if auth else False)
             response = requests.get(url, stream=True, auth=auth)
             response.raise_for_status()
+            Fetcher._logger.debug(" - Success")
             return response.iter_content(chunk_size=chunk_size)
         except requests.RequestException as e:
-            warnings.warn(f'Error downloading the file: {e}')
+            
+            WarnRaiser(Fetcher._download_buffer).custom(f'Error downloading the file: {e}')
             return False
```

### Comparing `xnippet-0.1.0/xnippet/fetcher/snippets.py` & `xnippet-0.1.1/src/xnippet/fetcher/snippets.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 """Provides functionality to manage and synchronize snippets across local and remote sources.
 
 This module defines a `Snippets` class which aggregates snippets from various sources,
 handles their synchronization, and ensures that the snippets are up-to-date according to
-user-specified modes (plugin, preset, bids, app). It supports operations on snippets
+user-specified modes (plugin, preset, recipe, schema). It supports operations on snippets
 fetched from both local file systems and remote repositories, offering features to check
 connectivity, fetch content, and validate snippet integrity.
 
 Classes:
     Snippets: Manages the aggregation and synchronization of snippets based on specified modes.
 """
 
 from __future__ import annotations
 import os
 import warnings
+import logging
 from pathlib import Path
 from .base import Fetcher
 from xnippet.raiser import WarnRaiser
-from xnippet.snippet import PlugInSnippet, RecipeSnippet, SpecSnippet, PresetSnippet
+from xnippet.snippet import SimpleSnippet, PlugInSnippet
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from typing import Optional
     from typing import List
-    from xnippet.types import SnippetType, SnippetMode, SnippetPath, StorageMode, VersionType
-
+    from xnippet.types import SimpleSnippetType, SnippetMode, SnippetPath, StorageMode, VersionType
+    from logging import Logger
+    
 
 class Snippets(Fetcher):
     """Manages the aggregation of snippets from various sources based on the specified mode.
 
     This class integrates local and remote snippet sources, handling their fetching, storing,
     and updating based on connectivity and cache settings.
     """
     path: Optional[Path]
     mode: SnippetMode
     package_name: str
     package_version: VersionType
     is_cache: bool
     _fetched: bool = False
-    _remote_snippets: List[SnippetType] = []
-    _local_snippets: List[SnippetType] = []
+    _remote_snippets: List[SimpleSnippetType] = []
+    _local_snippets: List[SimpleSnippetType] = []
+    _logger: Logger = logging.getLogger(__name__)
     
     def __init__(self, 
                  repos: dict,
                  package_name: str,
                  package_version: VersionType,
                  mode: SnippetMode,
                  path: SnippetPath = (None, False)
@@ -58,33 +61,35 @@
         self.package_version = package_version
         self.mode = mode
         self.path = self._resolve(path[0]) if path[0] else path[0]
         self.is_cache = path[1]
         self._set_auth()
         self._fetch_local_contents()
         
-    def _inspect_repos(self, repos):
+    @staticmethod
+    def _inspect_repos(repos):
         inspected = {}
-        for repo in repos:
-            # Check if both 'name' and 'url' keys exist in the repo dictionary
+        for i, repo in enumerate(repos):
+            Snippets._logger.debug(" + Check repo id: %d", i)
             name = repo.get('name')
             url = repo.get('url')
             
             if not name or not url:
-                message = f"Given repo '{name}' in configuration file does not comply with the expected configuration."
-                WarnRaiser(self._inspect_repos).custom(message, UserWarning)
+                message = f" Given repo '{name}' in configuration file does not comply with the expected configuration."
+                WarnRaiser(Snippets._inspect_repos).custom(message, UserWarning)
                 inspected[name] = None
             else:
+                Snippets._logger.debug(" + name: %s, url: %s", name, url)
                 inspected[name] = repo
 
         # Filter out None values and return the list of valid repos
         filtered_repo = [repo for repo in inspected.values() if repo is not None]
         if not filtered_repo:
-            message = "No valid repo configurations remain; nothing to download."
-            WarnRaiser(self._inspect_repos).custom(message, UserWarning)
+            message = "No valid repo configurations found; nothing to download."
+            WarnRaiser(Snippets._inspect_repos).custom(message, UserWarning)
         return filtered_repo
         
     def _fetch_local_contents(self) -> Optional[list]:
         """Fetches snippets from local storage based on the current mode and path settings.
 
         Gathers contents from the specified directory and converts them into snippets. This operation
         is skipped if caching mode is enabled. (This means the Xnippet initiated with dedicate space to download Sneppits.)
@@ -125,38 +130,34 @@
             contents (list): List of contents fetched from either local or remote sources.
             remote (bool, optional): Flag indicating whether the contents are from remote sources.
         """
         snippets = []
         for repo_id, content in enumerate(contents):
             for c in content:
                 if remote:
-                    snippets.append(self._snippet(contents=c, auth=self._auth[repo_id], remote=remote))
+                    snippets.append(self._snippet(contents=c, auth=self._auth[repo_id], remote=remote, repository=self._repos[repo_id]['name']))
                     storage = self._remote_snippets
                 else:
                     snippets.append(self._snippet(contents=c, remote=remote))
                     storage = self._local_snippets
         for s in snippets:            
             if s.is_valid and s.name not in [s_.name for s_ in storage]:
                 storage.append(s)
                         
     @property
     def _snippet(self):
         """Determines the snippet class based on the operational mode.
 
         Returns:
-            Type[Snippet]: Returns the class type corresponding to the operational mode (Plugin, Preset, Spec, Recipe, App).
+            Type[Snippet]: Returns the class type corresponding to the operational mode (Plugin, Preset, Schema, Recipe).
         """
         if self.mode == 'plugin':
             return PlugInSnippet
-        elif self.mode == 'preset':
-            return PresetSnippet
-        elif self.mode == 'spec':
-            return SpecSnippet
-        elif self.mode == 'recipe':
-            return RecipeSnippet
+        elif self.mode == 'simple':
+            return SimpleSnippet
     
     @property
     def remote(self):
         """Access the remote snippets if available. Fetches the snippets from a remote source if not already fetched
         and if a network connection is available.
 
         Returns:
```

### Comparing `xnippet-0.1.0/xnippet/formatter/bytes.py` & `xnippet-0.1.1/src/xnippet/formatter/bytes.py`

 * *Files 13% similar despite different names*

```diff
@@ -43,16 +43,7 @@
                     1: 'KB',
                     2: 'MB',
                     3: 'GB'}
         file_size = os.path.getsize(file_path)
 
         unit = int(len(str(file_size)) / 3)
         return Bytes.convert_unit(file_size, unit), unit_dict[unit]
-
-    @staticmethod
-    def print_internal_error(io_handler=None):
-        import traceback
-        import sys
-        if io_handler is None:
-            io_handler = sys.stderr
-        traceback.print_exception(*sys.exc_info(),
-                                file=io_handler)
```

### Comparing `xnippet-0.1.0/xnippet/formatter/string.py` & `xnippet-0.1.1/src/xnippet/formatter/string.py`

 * *Files identical despite different names*

### Comparing `xnippet-0.1.0/xnippet/module/installer.py` & `xnippet-0.1.1/src/xnippet/module/installer.py`

 * *Files identical despite different names*

### Comparing `xnippet-0.1.0/xnippet/module/loader.py` & `xnippet-0.1.1/src/xnippet/module/loader.py`

 * *Files identical despite different names*

### Comparing `xnippet-0.1.0/xnippet/raiser/types.py` & `xnippet-0.1.1/src/xnippet/raiser/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-class ConfigNotFound(UserWarning):
+class ConfigFileWarning(UserWarning):
     """Custom warning to indicate that a configuration file was not found."""
     pass
 
 class FileExistsWarning(UserWarning):
     """Custom warning to indicate that the configuration file exists, subject to overwrite."""
     pass
 
 class DownloadFailedWarning(UserWarning):
     """Custom warning to indicate that attempt download is failed."""
     pass
 
+class FetchFailedWarning(UserWarning):
+    pass
+
 class InvalidApproachWarning(UserWarning):
     """Custom warning to indicate that attemp of invalid approach."""
     pass
     
-class ComplianceWarning(UserWarning):
+class ManifestStandardWarning(UserWarning):
     """Warning raised when the manifest does not comply with the required standards.
 
     This warning is used to indicate deviations from expected configuration standards
     in the manifest file. It helps in identifying and debugging issues related to
     compliance with predefined specifications or requirements.
     """
     pass
```

### Comparing `xnippet-0.1.0/xnippet/raiser/warn.py` & `xnippet-0.1.1/src/xnippet/raiser/warn.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,67 +1,52 @@
-"""This module provide several warning cases and pre-written message to use xnippy easy to handle cases
+"""
+This module provides various warning cases with pre-written messages to facilitate easy handling of cases in xnippy.
 """
 from __future__ import annotations
+import logging
 from functools import partial
 from warnings import warn
 from .types import *
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
-    from typing import Any
-    from typing import Optional
+    from typing import Any, Optional, Literal
 
 
 class Warn:
-    def __init__(self, 
-                 object: Any, 
-                 stacklevel: int = 1):
+    def __init__(self, object: Any, stacklevel: int = 1):
         self._warn = partial(warn, stacklevel=stacklevel, source=object)
+        self._logger = logging.getLogger(object.__name__)
     
-    def _wrap_message(self, message:str, comment: Optional[str] = None):
+    def _wrap_message(self, message: str, comment: Optional[str] = None):
+        self._logger.warning("++ %s %s", message, comment)
         return f"{message} {comment}" if comment else message
     
     def custom(self, message: str, category: Warning = UserWarning):
         return self._warn(message=message, category=category)
         
-    def config_not_found(self, config_dir: str, comment: Optional[str] = None) -> None:
-        """Handles the absence of a configuration file by preparing a default configuration.
-
-        Args:
-            config_dir (str): The path to the directory where the configuration file is expected.
-
-        Raises:
-            ConfigNotFound: Warns that the configuration file was not found and defaults are being used.
-        """
-        message = f"Configuration file not found in '{config_dir}'."
-        return self._warn(message=self._wrap_message(message, comment), category=ConfigNotFound)
-    
-    def config_exist_when_create(self, comment: Optional[str] = None):
-        message = "Config folder already exists, Skipping creation. Use 'force' argument to overwrite."
-        return self._warn(message=self._wrap_message(message, comment), category=FileExistsWarning)
+    def config_file(self, config_dir: str, exists: bool, comment: Optional[str] = None) -> None:
+        message = f"Configuration file '{config_dir}' already exists." if exists else f"Configuration file '{config_dir}' not found."
+        return self._warn(message=self._wrap_message(message, comment), category=ConfigFileWarning)
     
-    def file_exist(self, filename: str, comment: Optional[str] = None):
+    def file_exists(self, filename: str, comment: Optional[str] = None):
         message = f"File '{filename}' already exists."
         return self._warn(message=self._wrap_message(message, comment), category=FileExistsWarning)
 
     def connection_failed(self, comment: Optional[str] = None):
-        message = "Connection failed."
+        message = "Connection to repository failed."
         return self._warn(message=self._wrap_message(message, comment), category=ConnectionFailedWarning)
 
-    def download_failed(self, comment: Optional[str] = None):
-        message = "Download failed."
+    def data_fetch_failed(self, comment: Optional[str] = None):
+        message = "Data fetch operation failed."
+        return self._warn(message=self._wrap_message(message, comment), category=FetchFailedWarning)
+
+    def download_error(self, comment: Optional[str] = None):
+        message = "Download operation failed."
         return self._warn(message=self._wrap_message(message, comment), category=DownloadFailedWarning)
     
-    def invalid_approach(self, comment: Optional[str] = None):
-        message = "Invalid approach."
+    def invalid_method(self, comment: Optional[str] = None):
+        message = "The approach used is invalid."
         return self._warn(message=self._wrap_message(message, comment), category=InvalidApproachWarning)
     
-    def compliance_warning(self, comment: Optional[str] = None):
-        """Issues a compliance warning with an optional custom comment.
-
-        Args:
-            comment (Optional[str]): Additional details about the compliance issue, default is None.
-        """
-        # Default message for compliance issues
-        message = "The manifest does not comply with the required standards."
-        return self._warn(message=self._wrap_message(message, comment), category=ComplianceWarning)
-
-
+    def manifest_noncompliance(self, comment: Optional[str] = None):
+        message = "Manifest file does not meet the required standards."
+        return self._warn(message=self._wrap_message(message, comment), category=ManifestStandardWarning)
```

### Comparing `xnippet-0.1.0/xnippet/snippet/base.py` & `xnippet-0.1.1/src/xnippet/fetcher/plugins.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-"""BaseSnippet for provide platform for developing Snippet to configure and/or interface with integrated apps's ecosystem.
-"""
-
 from __future__ import annotations
-from xnippet.fetcher.base import Fetcher
+from .snippets import Snippets as SnippetsFetcher
 from typing import TYPE_CHECKING
-from packaging.version import parse
 if TYPE_CHECKING:
-    from packaging.version import _Version as VersionType
-
+    from typing import List
+    from xnippet.types import SnippetPath
 
-class Snippet(Fetcher):
-    package_name: str
-    package_version: str
-    name: str
-    version: VersionType
-    type: str
-    is_valid: bool
-    
-    def parse_version(self, version_string):
-        self.version = parse(version_string)
+class PlugIns(SnippetsFetcher):
+    """Manages the aggregation of PlugIn snippets."""
+    def __init__(self,
+                 repos: List[dict],
+                 package_name: str,
+                 package_version: str,
+                 path: SnippetPath = (None, False)):
+        super().__init__(repos=repos, 
+                         package_name=package_name, 
+                         package_version=package_version, 
+                         mode='plugin', 
+                         path=path)
+        
+
```

### Comparing `xnippet-0.1.0/xnippet/snippet/plugin.py` & `xnippet-0.1.1/src/xnippet/snippet/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,35 +12,36 @@
 
 from __future__ import annotations
 import re
 import yaml
 import inspect
 from pathlib import Path
 from tqdm import tqdm
-from .base import Snippet
+from .simple import Simple
 from xnippet.raiser import WarnRaiser
 from xnippet.module import ModuleLoader
 from xnippet.module import ModuleInstaller
+from xnippet.formatter import StringFormatter
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from typing import Tuple, Dict, Optional, Union
     
 
-class PlugIn(Snippet):
+class PlugIn(Simple):
     """Handles the inspection and management of plugins, either locally or from remote sources.
     
     This class supports dynamic loading of plugins into memory for immediate use without the need for disk storage,
     facilitating rapid development and testing of plugin functionalities.
     
     Attributes:
         _contents: Dict = {"path": path of currnet plugin,
                            "files": list of paths or download urls of file contents,
                            "dirs": list of paths or access urls of diretory contents}
     """
-    _required_key: list = ['plugin', 'source', 'dependencies'] #, 'package']
+    _required_key: list = ['package', 'type', 'name', 'source', 'version', 'description', 'dependencies']
     _remote: bool
     _activated: bool
     _dependencies_tested: bool = False 
     _auth: Tuple[str, str]
     _data: Dict = {}
     _contents: Dict
     _repository: Optional[str]
@@ -105,18 +106,19 @@
             WarnRaiser('self._load_manifest').compliance_warning(comment=''.join(comment))
             self.is_valid = False
         else:
             self.is_valid = True
             
     def _set_params(self):
         try:
-            info = self._manifest['plugin']
+            info = self._manifest
             self.parse_version(info['version'])
             self.name = info['name']
             self.package = info['package'] if 'package' in info.keys() else None
+            self.type = info['type']
             self.is_valid = True
         except (KeyError, AttributeError):
             self.is_valid = False
         self._activated = False if self._remote else True
     ## Preperation step: ends
 
     ## Execution step: starts
@@ -133,16 +135,14 @@
 
         Returns:
             The result of calling the imported module with provided arguments.
 
         Raises:
             ValueError: If the provided arguments do not match the required function signature.
         """
-        if not self._activated:
-            self.download()
         sig = inspect.signature(self._imported_object)
         try:
             # This will raise a TypeError if the arguments do not match the function signature
             sig.bind(*args, **kwargs)
         except TypeError as e:
             raise TypeError(f"Argument mismatch for the imported module: {e}")
         if not self._dependencies_tested and not skip_dependency_check:
@@ -204,14 +204,16 @@
         """Dynamically imports the module from loaded data.
 
         This method uses the information from the manifest to import the specified module and method dynamically.
 
         Returns:
             The imported method from the module.
         """
+        if not self._activated:
+            self.download()
         # run include dependency
         if include := self._manifest['source']['include'] if 'include' in self._manifest['source'] else None:
             if isinstance(include, str):
                 include = [include]
             for filename in include:
                 if filename.endswith('.py'):
                     mloc = self._data[filename] if self._remote else self._contents['files'][filename]
@@ -227,15 +229,33 @@
             filename, target = matched.groups()
             mloc = self._data[filename] if self._remote else self._contents['files'][filename]
             loader = ModuleLoader(mloc)
             module = loader.get_module(self.name)
             self._include[self.name] = module
             return getattr(module, target)
         
+    def help(self, drop: Union[list, str, None] = None):
+        sigs = inspect.signature(self._imported_object).parameters.items()
+        if isinstance(drop, str):
+            drop = [drop]
+        sigs = {s:v for s, v in sigs if s not in drop}.items() if drop else sigs
+        
+        max_char = StringFormatter.calc_max_char([s for s, _ in sigs]) + 2
+        max_type = StringFormatter.calc_max_char([v.annotation for _, v in sigs]) + 2
+        max_default = StringFormatter.calc_max_char([v.default for _, v in sigs]) + 4
+        docstring = [f"{'Keyword'.center(max_char)}|{'Type'.center(max_type)}|{'Default'.center(max_default)}"]
+        docstring.append("-"*max_char + "+" + "-"*max_type + "+" + "-"*max_default)
+        for k, v in sigs:
+            default = f" '{v.default}'" if v.default else ' None'
+            value_type = f" {v.annotation}"
+            docstring.append(f"{k.ljust(max_char)}|{value_type.ljust(max_type)}|"
+                             f"{default.ljust(max_default)}")
+        print("\n".join(docstring))
+        
     def __repr__(self):
         if self.is_valid:
-            repr = f"PlugInSnippet<{self.package}>::{self.name}=={self.version}"
+            repr = f"PlugInSnippet[{self.package}]::{self.name}=={self.version}"
             if self._remote:
-                repr += '+InMemory' if self._activated else f'+Remote[{self._repository}]'
+                repr += '+InMemory' if self._activated else f'+Remote @{self._repository}'
             return repr
         else:
             return "PlugInSnippet<?>::InValidPlugin"
```

### Comparing `xnippet-0.1.0/.gitignore` & `xnippet-0.1.1/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -158,11 +158,13 @@
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 .idea/
 
 # OSX cache
 .DS_Store
 
-# xnippy config dir
-.xnippy
+# xnippet config dir
+.xnippet
 tests/*.ipynb
-.vscode
+.vscode
+*.log
+.python-version
```

### Comparing `xnippet-0.1.0/LICENSE` & `xnippet-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xnippet-0.1.0/pyproject.toml` & `xnippet-0.1.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -25,25 +25,35 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10"
 ]
 keywords = ["code snippets", "extensible", "plugin", "dynamic loading"]
 requires-python = ">=3.7"
 dependencies = [
     "pyyaml>=6.0.1",
-    "packaging>=23.0",
     "tqdm>=4.66.1",
     "requests>=2.31.0"
 ]
-urls = {Homepage = "https://xoani.github.io"}
+urls = {Homepage = "https://dvm-shlee.github.io"}
 
 [project.optional-dependencies]
 dev = [
+    "numpy",
     "flake8",
     "pytest",
     "nbmake",
     "types-PyYAML"
 ]
 
 # Additional configuration specific to hatch can go under 'tool.hatch.*'
 [tool.hatch.version]
-path = "xnippet/__init__.py"
+path = "src/xnippet/__init__.py"
 style = "pep440"
+
+[tool.hatch.build.targets.sdist]
+include = ["src"]
+
+[tool.hatch.build.targets.wheel]
+packages = ["src/xnippet"]
+
+[tool.pytest.ini_options]
+log_cli = true
+log_cli_level = "DEBUG"
```

### Comparing `xnippet-0.1.0/PKG-INFO` & `xnippet-0.1.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.3
 Name: xnippet
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python module for dynamic integration and management of extensible code snippets.
-Project-URL: Homepage, https://xoani.github.io
+Project-URL: Homepage, https://dvm-shlee.github.io
 Author-email: SungHo Lee <shlee@unc.edu>
 Maintainer-email: SungHo Lee <shlee@unc.edu>
 License: MIT
 License-File: LICENSE
 Keywords: code snippets,dynamic loading,extensible,plugin
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -14,62 +14,52 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
-Requires-Dist: packaging>=23.0
 Requires-Dist: pyyaml>=6.0.1
 Requires-Dist: requests>=2.31.0
 Requires-Dist: tqdm>=4.66.1
 Provides-Extra: dev
 Requires-Dist: flake8; extra == 'dev'
 Requires-Dist: nbmake; extra == 'dev'
+Requires-Dist: numpy; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: types-pyyaml; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # Xnippet - Extendable Plugin Architecture with Snippets for Python
 
-Welcome to `xnippet`, a robust framework designed to facilitate the integration of a plugin architecture into your projects. This system allows for the dynamic enhancement and customization of applications through plugins, enhancing project sustainability without expanding the core codebase. `xnippet` is ideal for those looking to add features for specific use cases or develop community-driven extensions while maintaining backward compatibility and minimizing dependencies.
+**Xnippet** is a standalone module designed to enhance the extensibility of Python-based projects, particularly in data analysis. Its key features include:
 
-This initiative stems from the need to evolve project features without the overhead of managing growing dependencies, thereby reducing maintenance challenges and allowing developers to focus on stabilizing and enriching the main codebase.
+- **Extensibility**: Functions as a new type of package manager that uses your GitHub repository for code version control, allowing the addition of features without modifying the existing codebase or increasing dependencies.
+- **Standardized Configuration**: Facilitates consistent settings across various environments and projects. Configurations and snippets can be inherited by subdirectories, maintaining uniformity across projects within the same directory. This feature is inspired by tools like pyenv.
+- **Sharing Code Snippets**: Enables a live searchable interface for code snippets stored in specified GitHub repositories. This feature supports the importing and direct use of snippets without local installation, enhancing online plugin functionality.
+- **Dependencies Control**: Manages dependencies on a per-snippet basis, checking and resolving dependencies during download or online import. This includes resolving Python dependencies via PyPI, managing snippet dependencies within your repository, and verifying the availability of external executables.
 
-## **Plugins**
-- **Independence**: Plugins can function as standalone applications, useful for personal data analysis projects. For dynamic functionality extension, your project should specify integration specifications, which ensure seamless plugin adoption.
-- **Example**: For a practical implementation, see [BrkRaw](https://github.com/brkraw/brkraw.git), which utilizes `xnippet` for enhanced plugin integration.
-- **Documentation**: Learn more about setting up and configuring plugins in our [Plugin Documentation](examples/docs/PLUGIN.md).
-
-## Features of xnippet's Plugin Architecture
-- **Snippets**: Unlike traditional plugin systems that require separate package installations, `xnippet` uses snippets, allowing for instant updates and modifications without restarting Python kernels. This approach saves significant development time and simplifies testing.
-- **GitHub Integration**: `xnippet` leverages GitHub as a repository server, enabling real-time updates and collaboration without the need for repackaging and redistributing through channels like PyPi. This feature ensures that new functionalities are instantly available without the need for updating the main package.
-- **Simplicity**: Our plugin architecture avoids the complexities of `setup.py`, `setup.cfg`, or `pyproject.toml` files, focusing instead on straightforward GitHub-based sharing and version control.
-
-### **Presets** -- WIP
-- **Functionality**: Presets simplify configuring plugins with multiple input arguments, ensuring consistent setups and facilitating hyperparameter testing in machine learning projects.
-- **Documentation**: Detailed information is available in our [Preset Documentation](examples/docs/PRESET.md).
-
-### **Specifications (Specs)** -- WIP
-- **Purpose**: Tailored for data analysis projects, specifications help define and validate data types and structures, ensuring data integrity and facilitating detailed inspections and validations similar to systems like Pydantic.
-- **Documentation**: Explore our [Specification Documentation](examples/docs/SPEC.md) for more details.
-
-### **Recipes**  -- WIP
-- **Utility**: Recipes allow for the automation of data preprocessing and metadata remapping, streamlining the integration and manipulation of datasets.
-- **Documentation**: Learn how to create and use recipes with our [Recipe Documentation](examples/docs/RECIPE.md).
+## **Types of Snippets**
+### Simple Snippets:
 
+- Python code that can be seamlessly imported and used within any module without specific entry-points.
+
+### **Plugin Snippets**:
+
+- Builds on Simple Snippets by adding entry-points to serve specific roles, ideal for developing Python packages with a straightforward plugin architecture.
+- Employs YAML for manifest packaging, with each snippet consisting of a single Python file and an accompanying manifest.
 ## Getting Started
 To begin integrating `xnippet` into your project, refer to our comprehensive [Project Configuration Guide](examples/docs/PROJECT_CONFIG.md).
 
 ## Documentation
 For detailed documentation on each component of the `xnippet` system, please visit the following links:
 - [Project Configuration](examples/docs/PROJECT_CONFIG.md)
 - [Plugins](examples/docs/PLUGIN.md)
   - [Presets](examples/docs/PRESET.md)
-  - [Specifications for Dataset](examples/docs/SPEC.md)
+  - [Data Schema](examples/docs/SCHEMA.md)
   - [Recipes for Parsing and Remapping MetaData](examples/docs/RECIPE.md)
 
 Explore these documents to fully understand how each module can be utilized and configured to enrich your project with our versatile plugin architecture.
 
 ## Contributing
 Contributions are welcome! If you have suggestions or improvements, please fork the repository and submit a pull request.
```

