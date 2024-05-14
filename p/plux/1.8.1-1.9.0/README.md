# Comparing `tmp/plux-1.8.1.tar.gz` & `tmp/plux-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plux-1.8.1.tar", last modified: Sat Mar 16 23:17:48 2024, max compression
+gzip compressed data, was "plux-1.9.0.tar", last modified: Sun Mar 24 20:37:02 2024, max compression
```

## Comparing `plux-1.8.1.tar` & `plux-1.9.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-16 23:17:48.140304 plux-1.8.1/
--rw-r--r--   0 thomas    (1000) thomas    (1000)    11358 2023-02-17 21:14:38.000000 plux-1.8.1/LICENSE
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     9708 2024-03-16 23:17:48.140304 plux-1.8.1/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8766 2024-02-22 23:08:11.000000 plux-1.8.1/README.md
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-16 23:17:48.136304 plux-1.8.1/plugin/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      613 2024-02-22 23:08:11.000000 plux-1.8.1/plugin/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      484 2024-02-22 23:08:11.000000 plux-1.8.1/plugin/core.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      198 2024-02-22 23:08:11.000000 plux-1.8.1/plugin/discovery.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      410 2024-02-22 23:08:11.000000 plux-1.8.1/plugin/entrypoint.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      303 2024-02-22 23:08:11.000000 plux-1.8.1/plugin/metadata.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      303 2024-03-16 22:27:36.000000 plux-1.8.1/plugin/setuptools.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-16 23:17:48.136304 plux-1.8.1/plux/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      739 2024-03-16 23:17:27.000000 plux-1.8.1/plux/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      133 2024-02-22 23:08:11.000000 plux-1.8.1/plux/__main__.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-16 23:17:48.140304 plux-1.8.1/plux/build/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      159 2024-02-22 23:08:11.000000 plux-1.8.1/plux/build/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1534 2024-03-16 22:19:49.000000 plux-1.8.1/plux/build/discovery.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    12153 2024-03-16 22:32:26.000000 plux-1.8.1/plux/build/setuptools.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-16 23:17:48.140304 plux-1.8.1/plux/cli/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2024-02-22 23:08:11.000000 plux-1.8.1/plux/cli/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2518 2024-03-16 23:17:09.000000 plux-1.8.1/plux/cli/cli.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-16 23:17:48.140304 plux-1.8.1/plux/core/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2024-02-22 23:08:11.000000 plux-1.8.1/plux/core/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1314 2024-02-22 23:08:11.000000 plux-1.8.1/plux/core/entrypoint.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8620 2024-02-22 23:08:11.000000 plux-1.8.1/plux/core/plugin.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-16 23:17:48.140304 plux-1.8.1/plux/runtime/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2024-02-22 23:08:11.000000 plux-1.8.1/plux/runtime/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    11726 2024-02-22 23:08:11.000000 plux-1.8.1/plux/runtime/manager.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1963 2024-02-22 23:08:11.000000 plux-1.8.1/plux/runtime/metadata.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2295 2024-02-22 23:08:11.000000 plux-1.8.1/plux/runtime/resolve.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-16 23:17:48.136304 plux-1.8.1/plux.egg-info/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     9708 2024-03-16 23:17:48.000000 plux-1.8.1/plux.egg-info/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      670 2024-03-16 23:17:48.000000 plux-1.8.1/plux.egg-info/SOURCES.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2024-03-16 23:17:48.000000 plux-1.8.1/plux.egg-info/dependency_links.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      137 2024-03-16 23:17:48.000000 plux-1.8.1/plux.egg-info/entry_points.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2024-03-16 23:17:45.000000 plux-1.8.1/plux.egg-info/not-zip-safe
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      126 2024-03-16 23:17:48.000000 plux-1.8.1/plux.egg-info/requires.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       12 2024-03-16 23:17:48.000000 plux-1.8.1/plux.egg-info/top_level.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      212 2024-02-22 23:08:11.000000 plux-1.8.1/pyproject.toml
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1426 2024-03-16 23:17:48.140304 plux-1.8.1/setup.cfg
--rw-r--r--   0 thomas    (1000) thomas    (1000)       60 2023-02-17 21:14:38.000000 plux-1.8.1/setup.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 20:37:02.649589 plux-1.9.0/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    11358 2023-02-17 21:14:38.000000 plux-1.9.0/LICENSE
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     9708 2024-03-24 20:37:02.649589 plux-1.9.0/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8766 2024-02-22 23:08:11.000000 plux-1.9.0/README.md
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 20:37:02.645589 plux-1.9.0/plugin/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      613 2024-02-22 23:08:11.000000 plux-1.9.0/plugin/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      484 2024-02-22 23:08:11.000000 plux-1.9.0/plugin/core.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      198 2024-02-22 23:08:11.000000 plux-1.9.0/plugin/discovery.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      410 2024-02-22 23:08:11.000000 plux-1.9.0/plugin/entrypoint.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      303 2024-02-22 23:08:11.000000 plux-1.9.0/plugin/metadata.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      303 2024-03-16 22:27:36.000000 plux-1.9.0/plugin/setuptools.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 20:37:02.645589 plux-1.9.0/plux/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      779 2024-03-24 20:36:41.000000 plux-1.9.0/plux/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      133 2024-02-22 23:08:11.000000 plux-1.9.0/plux/__main__.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 20:37:02.649589 plux-1.9.0/plux/build/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      159 2024-02-22 23:08:11.000000 plux-1.9.0/plux/build/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1534 2024-03-16 22:19:49.000000 plux-1.9.0/plux/build/discovery.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    12153 2024-03-16 22:32:26.000000 plux-1.9.0/plux/build/setuptools.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 20:37:02.649589 plux-1.9.0/plux/cli/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2024-02-22 23:08:11.000000 plux-1.9.0/plux/cli/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2518 2024-03-16 23:17:09.000000 plux-1.9.0/plux/cli/cli.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 20:37:02.649589 plux-1.9.0/plux/core/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2024-02-22 23:08:11.000000 plux-1.9.0/plux/core/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1314 2024-02-22 23:08:11.000000 plux-1.9.0/plux/core/entrypoint.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8666 2024-03-24 20:36:36.000000 plux-1.9.0/plux/core/plugin.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 20:37:02.649589 plux-1.9.0/plux/runtime/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2024-02-22 23:08:11.000000 plux-1.9.0/plux/runtime/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    12491 2024-03-24 20:36:36.000000 plux-1.9.0/plux/runtime/manager.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1963 2024-02-22 23:08:11.000000 plux-1.9.0/plux/runtime/metadata.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2295 2024-02-22 23:08:11.000000 plux-1.9.0/plux/runtime/resolve.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 20:37:02.645589 plux-1.9.0/plux.egg-info/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     9708 2024-03-24 20:37:02.000000 plux-1.9.0/plux.egg-info/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      670 2024-03-24 20:37:02.000000 plux-1.9.0/plux.egg-info/SOURCES.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2024-03-24 20:37:02.000000 plux-1.9.0/plux.egg-info/dependency_links.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      137 2024-03-24 20:37:02.000000 plux-1.9.0/plux.egg-info/entry_points.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2024-03-24 20:36:57.000000 plux-1.9.0/plux.egg-info/not-zip-safe
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      126 2024-03-24 20:37:02.000000 plux-1.9.0/plux.egg-info/requires.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       12 2024-03-24 20:37:02.000000 plux-1.9.0/plux.egg-info/top_level.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      212 2024-02-22 23:08:11.000000 plux-1.9.0/pyproject.toml
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1426 2024-03-24 20:37:02.649589 plux-1.9.0/setup.cfg
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       60 2023-02-17 21:14:38.000000 plux-1.9.0/setup.py
```

### Comparing `plux-1.8.1/LICENSE` & `plux-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plux-1.8.1/PKG-INFO` & `plux-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plux
-Version: 1.8.1
+Version: 1.9.0
 Summary: A dynamic code loading framework for building pluggable Python distributions
 Home-page: https://github.com/localstack/plux
 Author: Thomas Rausch
 Author-email: thomas@localstack.cloud
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `plux-1.8.1/README.md` & `plux-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `plux-1.8.1/plugin/__init__.py` & `plux-1.9.0/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `plux-1.8.1/plux/__init__.py` & `plux-1.9.0/plux/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,24 +13,25 @@
     PluginType,
     plugin,
 )
 from plux.runtime.manager import PluginContainer, PluginManager
 
 name = "plux"
 
-__version__ = "1.8.1"
+__version__ = "1.9.0"
 
 __all__ = [
     "FunctionPlugin",
     "Plugin",
     "PluginDisabled",
     "PluginException",
     "PluginFactory",
     "PluginFinder",
     "PluginLifecycleListener",
+    "CompositePluginLifecycleListener",
     "PluginManager",
     "PluginContainer",
     "PluginSpec",
     "PluginSpecResolver",
     "PluginType",
     "plugin",
 ]
```

### Comparing `plux-1.8.1/plux/build/discovery.py` & `plux-1.9.0/plux/build/discovery.py`

 * *Files identical despite different names*

### Comparing `plux-1.8.1/plux/build/setuptools.py` & `plux-1.9.0/plux/build/setuptools.py`

 * *Files identical despite different names*

### Comparing `plux-1.8.1/plux/cli/cli.py` & `plux-1.9.0/plux/cli/cli.py`

 * *Files identical despite different names*

### Comparing `plux-1.8.1/plux/core/entrypoint.py` & `plux-1.9.0/plux/core/entrypoint.py`

 * *Files identical despite different names*

### Comparing `plux-1.8.1/plux/core/plugin.py` & `plux-1.9.0/plux/core/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,21 +8,24 @@
     def __init__(self, message, namespace: str = None, name: str = None) -> None:
         super().__init__(message)
         self.namespace = namespace
         self.name = name
 
 
 class PluginDisabled(PluginException):
+    reason: str
+
     def __init__(self, namespace: str, name: str, reason: str = None):
         message = f"plugin {namespace}:{name} is disabled"
         if reason:
             message = f"{message}, reason: {reason}"
         super(PluginDisabled, self).__init__(message)
         self.namespace = namespace
         self.name = name
+        self.reason = reason
 
 
 class Plugin(abc.ABC):
     """A generic LocalStack plugin.
 
     A Plugin's purpose is to be loaded dynamically at runtime and defer code imports into the Plugin::load method.
     Abstract subtypes of plugins (e.g., a LocalstackCliPlugin) may overwrite the load method with concrete call
```

### Comparing `plux-1.8.1/plux/runtime/manager.py` & `plux-1.9.0/plux/runtime/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,24 +17,27 @@
 LOG = logging.getLogger(__name__)
 
 P = t.TypeVar("P", bound=Plugin)
 
 
 def _call_safe(func: t.Callable, args: t.Tuple, exception_message: str):
     """
-    Call the given function with the given arguments, and if it fails, log the given exception_message.
-    If logging.DEBUG is set for the logger, then we also log the traceback.
+    Call the given function with the given arguments, and if it fails, log the given exception_message. If
+    logging.DEBUG is set for the logger, then we also log the traceback. An exception is made for any
+    ``PluginException``, which should be handled by the caller.
 
     :param func: function to call
     :param args: arguments to pass
     :param exception_message: message to log on exception
     :return: whatever the func returns
     """
     try:
         return func(*args)
+    except PluginException:
+        raise
     except Exception as e:
         if LOG.isEnabledFor(logging.DEBUG):
             LOG.exception(exception_message)
         else:
             LOG.error("%s: %s", exception_message, e)
 
 
@@ -119,14 +122,17 @@
 
     is_init: bool = False
     is_loaded: bool = False
 
     init_error: Exception = None
     load_error: Exception = None
 
+    is_disabled: bool = False
+    disabled_reason = str = None
+
     @property
     def distribution(self) -> Distribution:
         """
         Uses metadata from importlib to resolve the distribution information for this plugin.
 
         :return: the importlib.metadata.Distribution object
         """
@@ -188,16 +194,24 @@
         Loads the Plugin with the given name using the load args and kwargs set in the plugin manager constructor.
         If at any point in the lifecycle the plugin loading fails, the load method will raise the respective exception.
 
         Load is idempotent, so once the plugin is loaded, load will return the same instance again.
         """
         container = self._require_plugin(name)
 
+        if container.is_disabled:
+            raise PluginDisabled(container.plugin_spec.namespace, name, container.disabled_reason)
+
         if not container.is_loaded:
-            self._load_plugin(container)
+            try:
+                self._load_plugin(container)
+            except PluginDisabled as e:
+                container.is_disabled = True
+                container.disabled_reason = e.reason
+                raise
 
         if container.init_error:
             raise container.init_error
 
         if container.load_error:
             raise container.load_error
 
@@ -273,39 +287,47 @@
             # instantiate Plugin from spec if necessary
             if not container.is_init:
                 try:
                     LOG.debug("instantiating plugin %s", plugin_spec)
                     container.plugin = self._plugin_from_spec(plugin_spec)
                     container.is_init = True
                     self._fire_on_init_after(plugin_spec, container.plugin)
+                except PluginDisabled:
+                    raise
                 except Exception as e:
                     # TODO: maybe we should move these logging blocks to `load_all`, since this is the only instance
                     #  where exceptions messages may get lost.
                     if LOG.isEnabledFor(logging.DEBUG):
                         LOG.exception("error instantiating plugin %s", plugin_spec)
 
                     self._fire_on_init_exception(plugin_spec, e)
                     container.init_error = e
                     return
 
             plugin = container.plugin
 
             if not plugin.should_load():
-                raise PluginDisabled(namespace=self.namespace, name=container.plugin_spec.name)
+                raise PluginDisabled(
+                    namespace=self.namespace,
+                    name=container.plugin_spec.name,
+                    reason="Load condition for plugin was false",
+                )
 
             args = self.load_args
             kwargs = self.load_kwargs
 
-            self._fire_on_load_before(plugin_spec, plugin, args, kwargs)
             try:
+                self._fire_on_load_before(plugin_spec, plugin, args, kwargs)
                 LOG.debug("loading plugin %s:%s", self.namespace, plugin_spec.name)
                 result = plugin.load(*args, **kwargs)
                 self._fire_on_load_after(plugin_spec, plugin, result)
                 container.load_value = result
                 container.is_loaded = True
+            except PluginDisabled:
+                raise
             except Exception as e:
                 if LOG.isEnabledFor(logging.DEBUG):
                     LOG.exception("error loading plugin %s", plugin_spec)
                 self._fire_on_load_exception(plugin_spec, plugin, e)
                 container.load_error = e
 
     def _plugin_from_spec(self, plugin_spec: PluginSpec) -> P:
```

### Comparing `plux-1.8.1/plux/runtime/metadata.py` & `plux-1.9.0/plux/runtime/metadata.py`

 * *Files identical despite different names*

### Comparing `plux-1.8.1/plux/runtime/resolve.py` & `plux-1.9.0/plux/runtime/resolve.py`

 * *Files identical despite different names*

### Comparing `plux-1.8.1/plux.egg-info/PKG-INFO` & `plux-1.9.0/plux.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plux
-Version: 1.8.1
+Version: 1.9.0
 Summary: A dynamic code loading framework for building pluggable Python distributions
 Home-page: https://github.com/localstack/plux
 Author: Thomas Rausch
 Author-email: thomas@localstack.cloud
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `plux-1.8.1/plux.egg-info/SOURCES.txt` & `plux-1.9.0/plux.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plux-1.8.1/setup.cfg` & `plux-1.9.0/setup.cfg`

 * *Files identical despite different names*

