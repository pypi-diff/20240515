# Comparing `tmp/comfy_script-0.5.0a4.tar.gz` & `tmp/comfy_script-0.5.0a5.tar.gz`

## Comparing `comfy_script-0.5.0a4.tar` & `comfy_script-0.5.0a5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/__init__.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/requirements.txt
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/settings.example.toml
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/.vscode/launch.json
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/docs/README.md
--rw-r--r--   0        0        0    18293 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/docs/Runtime.md
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/docs/Transpiler.md
--rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/docs/Image/README.md
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/docs/Latent/README.md
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/docs/Models/README.md
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/docs/Nodes/README.md
--rw-r--r--   0        0        0   839054 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/docs/images/README/auto-queue.png
--rw-r--r--   0        0        0    41490 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/docs/images/README/diff.png
--rw-r--r--   0        0        0   908632 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/docs/images/README/plot.png
--rw-r--r--   0        0        0  2677075 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/docs/images/README/select.png
--rw-r--r--   0        0        0    74672 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/docs/images/README/type-stubs.png
--rw-r--r--   0        0        0    51995 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/docs/images/README/type-stubs2.png
--rw-r--r--   0        0        0    89265 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/docs/images/README/workflow.png
--rw-r--r--   0        0        0   170300 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/docs/images/README/workflow2.png
--rw-r--r--   0        0        0   199246 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/docs/images/Runtime/load-api-format.png
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/__init__.py
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/astutil.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/config.py
--rw-r--r--   0        0        0     7619 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/client/__init__.py
--rw-r--r--   0        0        0     8525 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/nodes/__init__.py
--rw-r--r--   0        0        0    44839 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/runtime/__init__.py
--rw-r--r--   0        0        0    20573 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/runtime/factory.py
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/runtime/nodes.py
--rw-r--r--   0        0        0     4442 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/runtime/data/Images.py
--rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/runtime/data/__init__.py
--rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/runtime/real/__init__.py
--rw-r--r--   0        0        0     7291 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/runtime/real/nodes.py
--rw-r--r--   0        0        0    14763 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/transpile/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/transpile/__main__.py
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/transpile/prompt.py
--rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/transpile/passes/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/ui/__init__.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/ui/solara/__init__.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/ui/solara/metadata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/tests/__init__.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/tests/test_astutil.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/tests/transpile/__init__.py
--rw-r--r--   0        0        0    23060 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/tests/transpile/bypass.json
--rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/tests/transpile/default.json
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/tests/transpile/test_transpiler.py
--rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/LICENSE.txt
--rw-r--r--   0        0        0    14619 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/README.md
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/pyproject.toml
--rw-r--r--   0        0        0    16502 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/PKG-INFO
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/__init__.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/requirements.txt
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/settings.example.toml
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/.vscode/launch.json
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/docs/README.md
+-rw-r--r--   0        0        0    18291 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/docs/Runtime.md
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/docs/Transpiler.md
+-rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/docs/Images/README.md
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/docs/Latent/README.md
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/docs/Models/README.md
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/docs/Nodes/README.md
+-rw-r--r--   0        0        0   839054 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/docs/imgs/README/auto-queue.png
+-rw-r--r--   0        0        0    41490 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/docs/imgs/README/diff.png
+-rw-r--r--   0        0        0   908632 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/docs/imgs/README/plot.png
+-rw-r--r--   0        0        0  2677075 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/docs/imgs/README/select.png
+-rw-r--r--   0        0        0    74672 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/docs/imgs/README/type-stubs.png
+-rw-r--r--   0        0        0    51995 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/docs/imgs/README/type-stubs2.png
+-rw-r--r--   0        0        0    89265 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/docs/imgs/README/workflow.png
+-rw-r--r--   0        0        0   170300 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/docs/imgs/README/workflow2.png
+-rw-r--r--   0        0        0   199246 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/docs/imgs/Runtime/load-api-format.png
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/src/comfy_script/__init__.py
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/src/comfy_script/astutil.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/src/comfy_script/config.py
+-rw-r--r--   0        0        0     7619 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/src/comfy_script/client/__init__.py
+-rw-r--r--   0        0        0     8525 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/src/comfy_script/nodes/__init__.py
+-rw-r--r--   0        0        0    44839 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/src/comfy_script/runtime/__init__.py
+-rw-r--r--   0        0        0    20573 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/src/comfy_script/runtime/factory.py
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/src/comfy_script/runtime/nodes.py
+-rw-r--r--   0        0        0     4442 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/src/comfy_script/runtime/data/Images.py
+-rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/src/comfy_script/runtime/data/__init__.py
+-rw-r--r--   0        0        0     6497 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/src/comfy_script/runtime/real/__init__.py
+-rw-r--r--   0        0        0     8228 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/src/comfy_script/runtime/real/nodes.py
+-rw-r--r--   0        0        0    14763 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/src/comfy_script/transpile/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/src/comfy_script/transpile/__main__.py
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/src/comfy_script/transpile/prompt.py
+-rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/src/comfy_script/transpile/passes/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/src/comfy_script/ui/__init__.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/src/comfy_script/ui/solara/__init__.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/src/comfy_script/ui/solara/metadata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/tests/__init__.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/tests/test_astutil.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/tests/transpile/__init__.py
+-rw-r--r--   0        0        0    23060 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/tests/transpile/bypass.json
+-rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/tests/transpile/default.json
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/tests/transpile/test_transpiler.py
+-rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/LICENSE.txt
+-rw-r--r--   0        0        0    14602 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/README.md
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/pyproject.toml
+-rw-r--r--   0        0        0    16485 2020-02-02 00:00:00.000000 comfy_script-0.5.0a5/PKG-INFO
```

### Comparing `comfy_script-0.5.0a4/__init__.py` & `comfy_script-0.5.0a5/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a4/settings.example.toml` & `comfy_script-0.5.0a5/settings.example.toml`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a4/docs/README.md` & `comfy_script-0.5.0a5/docs/README.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a4/docs/Runtime.md` & `comfy_script-0.5.0a5/docs/Runtime.md`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
 json = wf.api_format_json()
 with open('prompt.json', 'w') as f:
     f.write(json)
 ```
 This only generates workflows in the API format. But ComfyUI can automically convert API format workflows to the web UI format when you load them ([#1932](https://github.com/comfyanonymous/ComfyUI/pull/1932)):
 
-![](images/Runtime/load-api-format.png)
+![](imgs/Runtime/load-api-format.png)
 
 You can also load workflows from images generated by ComfyScript.
 
 Note: You may get slightly different results when using the generated workflow in the web UI compared to using it in ComfyScript. See [differences from ComfyUI's web UI](#differences-from-comfyuis-web-ui) for the reason.
 
 ### Async support
 Virtual mode is internally asynchronous, but only exposes synchronous APIs for the following reasons:
```

### Comparing `comfy_script-0.5.0a4/docs/Image/README.md` & `comfy_script-0.5.0a5/docs/Images/README.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a4/docs/Latent/README.md` & `comfy_script-0.5.0a5/docs/Latent/README.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a4/docs/Models/README.md` & `comfy_script-0.5.0a5/docs/Models/README.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a4/docs/Nodes/README.md` & `comfy_script-0.5.0a5/docs/Nodes/README.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a4/docs/images/README/auto-queue.png` & `comfy_script-0.5.0a5/docs/imgs/README/auto-queue.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a4/docs/images/README/diff.png` & `comfy_script-0.5.0a5/docs/imgs/README/diff.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a4/docs/images/README/plot.png` & `comfy_script-0.5.0a5/docs/imgs/README/plot.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a4/docs/images/README/select.png` & `comfy_script-0.5.0a5/docs/imgs/README/select.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a4/docs/images/README/type-stubs.png` & `comfy_script-0.5.0a5/docs/imgs/README/type-stubs.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a4/docs/images/README/type-stubs2.png` & `comfy_script-0.5.0a5/docs/imgs/README/type-stubs2.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a4/docs/images/README/workflow.png` & `comfy_script-0.5.0a5/docs/imgs/README/workflow.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a4/docs/images/README/workflow2.png` & `comfy_script-0.5.0a5/docs/imgs/README/workflow2.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a4/docs/images/Runtime/load-api-format.png` & `comfy_script-0.5.0a5/docs/imgs/Runtime/load-api-format.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a4/src/comfy_script/astutil.py` & `comfy_script-0.5.0a5/src/comfy_script/astutil.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a4/src/comfy_script/client/__init__.py` & `comfy_script-0.5.0a5/src/comfy_script/client/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a4/src/comfy_script/nodes/__init__.py` & `comfy_script-0.5.0a5/src/comfy_script/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a4/src/comfy_script/runtime/__init__.py` & `comfy_script-0.5.0a5/src/comfy_script/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a4/src/comfy_script/runtime/factory.py` & `comfy_script-0.5.0a5/src/comfy_script/runtime/factory.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a4/src/comfy_script/runtime/nodes.py` & `comfy_script-0.5.0a5/src/comfy_script/runtime/nodes.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a4/src/comfy_script/runtime/data/Images.py` & `comfy_script-0.5.0a5/src/comfy_script/runtime/data/Images.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a4/src/comfy_script/runtime/data/__init__.py` & `comfy_script-0.5.0a5/src/comfy_script/runtime/data/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a4/src/comfy_script/runtime/real/__init__.py` & `comfy_script-0.5.0a5/src/comfy_script/runtime/real/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 import asyncio
 from dataclasses import dataclass
 from pathlib import Path
+from typing import Callable, MutableMapping
 
 def load(comfyui: Path | str = None, args: ComfyUIArgs | None = None, vars: dict | None = None, naked: bool = False, config: RealModeConfig | None = None, no_server: bool = True):
     '''
     - `comfyui`: Path to ComfyUI directory.
     
       The default path is `ComfyScript/../..`, which only works if ComfyScript is installed at `ComfyUI/custom_nodes/ComfyScript`.
 
@@ -33,33 +34,73 @@
     if naked:
         config = RealModeConfig.naked()
     elif config is None:
         config = RealModeConfig()
     asyncio.run(nodes.load(nodes_info, vars, config))
 
 class Workflow:
-    def __init__(self):
+    # TODO: Thread-safe
+    _instance: Workflow = None
+
+    def __init__(
+        self,
+        *,
+        cache: MutableMapping | Callable[[str], MutableMapping] | None = None
+    ):
+        '''
+        - `cache`: Use `dict` (`{}`) for simple unbounded cache. For advanced cache, [cachetools](https://github.com/tkem/cachetools) or other libraries can be used.
+
+          To use different cache for different types of nodes, pass a callable that accepts the node name and returns a cache. For example:
+          ```
+          cache=lambda node: {}
+          ```
+          or:
+          ```
+          node_cache = {}
+          cache=lambda node: node_cache.setdefault(node, {})
+          ```
+
+          Note that for node output, any changes made by user code instead of nodes will be ignored.
+        '''
         import torch
 
         self.inference_mode = torch.inference_mode()
+        self._cache = cache
+        self._node_cache = {}
 
     def __enter__(self) -> Workflow:
+        Workflow._instance = self
+
         import comfy.model_management
 
         self.inference_mode.__enter__()
 
         comfy.model_management.cleanup_models()
 
         return self
     
     def __exit__(self, exc_type, exc_value, traceback):
         # TODO: DISABLE_SMART_MEMORY
 
         self.inference_mode.__exit__(exc_type, exc_value, traceback)
 
+        Workflow._instance = None
+    
+    def _get_cache(self, node: str) -> MutableMapping | None:
+        if self._cache is None:
+            return None
+        elif isinstance(self._cache, MutableMapping):
+            return self._cache
+        else:
+            cache = self._node_cache.get(node, None)
+            if cache is None:
+                cache = self._cache(node)
+                self._node_cache[node] = cache
+            return cache
+
 @dataclass
 class RealModeConfig:
     callable: bool = True
     '''Make the nodes callable. Such that
       
     ```
     obj = MyNode()
```

### Comparing `comfy_script-0.5.0a4/src/comfy_script/runtime/real/nodes.py` & `comfy_script-0.5.0a5/src/comfy_script/runtime/real/nodes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 from pathlib import Path
 import traceback
 from typing import Any, Iterable
+from warnings import warn
 import wrapt
 
-from . import RealModeConfig
+from . import RealModeConfig, Workflow
 from .. import factory
 from ..nodes import _positional_args_to_keyword, Node as VirtualNode
 
 async def load(nodes_info: dict, vars: dict | None, config: RealModeConfig) -> None:
     fact = RealRuntimeFactory(config)
     await fact.init()
 
@@ -126,14 +127,30 @@
                                     kwds[k] = prompt
                                 elif v == 'UNIQUE_ID':
                                     if prompt is None:
                                         prompt, id = virtual_outputs[0]._get_prompt_and_id()
                                         unique_id = id.get_id(virtual_outputs[0].node_prompt)
                                     kwds[k] = unique_id
                                 # TODO: EXTRA_PNGINFO: ComfyScriptSource
+                
+                # Lookup cache
+                cache = None
+                wf = Workflow._instance
+                if wf is not None:
+                    cache = wf._get_cache(info['name'])
+                    if cache is not None:
+                        if not config.track_workflow:
+                            warn('Workflow cache requires `track_workflow` to work')
+                            cache = None
+                        else:
+                            # TODO: Or FrozenDict?
+                            prompt = virtual_outputs[0].api_format_json()
+                            outputs = cache.get(prompt, None)
+                            if outputs is not None:
+                                return outputs
 
                 # Call the node
                 outputs = getattr(obj, obj.FUNCTION)(*args, **kwds)
 
                 if config.track_workflow and virtual_outputs is not None:
                     if isinstance(outputs, Iterable) and not isinstance(outputs, dict):
                         if len(outputs) != len(virtual_outputs):
@@ -143,15 +160,19 @@
                             wrapped_output = RealNodeOutputWrapper(output)
                             wrapped_output._self_virtual_output = virtual_output
                             wrapped_outputs.append(wrapped_output)
                         outputs = wrapped_outputs
 
                 # See ComfyUI's `get_output_data()`
                 if config.unpack_single_output and isinstance(outputs, Iterable) and not isinstance(outputs, dict) and len(outputs) == 1:
-                    return outputs[0]
+                    outputs = outputs[0]
+                
+                # Cache outputs
+                if cache is not None:
+                    cache[prompt] = outputs
                 
                 return outputs
             
             if not config.wrapper:
                 cls.__new__ = new
                 if not hasattr(cls, 'create'):
                     setattr(cls, 'create', create)
```

### Comparing `comfy_script-0.5.0a4/src/comfy_script/transpile/__init__.py` & `comfy_script-0.5.0a5/src/comfy_script/transpile/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a4/src/comfy_script/transpile/prompt.py` & `comfy_script-0.5.0a5/src/comfy_script/transpile/prompt.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a4/src/comfy_script/transpile/passes/__init__.py` & `comfy_script-0.5.0a5/src/comfy_script/transpile/passes/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a4/src/comfy_script/ui/solara/metadata.py` & `comfy_script-0.5.0a5/src/comfy_script/ui/solara/metadata.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a4/tests/test_astutil.py` & `comfy_script-0.5.0a5/tests/test_astutil.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a4/tests/transpile/bypass.json` & `comfy_script-0.5.0a5/tests/transpile/bypass.json`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a4/tests/transpile/default.json` & `comfy_script-0.5.0a5/tests/transpile/default.json`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a4/tests/transpile/test_transpiler.py` & `comfy_script-0.5.0a5/tests/transpile/test_transpiler.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a4/.gitignore` & `comfy_script-0.5.0a5/.gitignore`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a4/LICENSE.txt` & `comfy_script-0.5.0a5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a4/README.md` & `comfy_script-0.5.0a5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # ComfyScript
 [![PyPI - Version](https://img.shields.io/pypi/v/comfy-script)](https://pypi.org/project/comfy-script) ![Python Version from PEP 621 TOML](https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2FChaoses-Ib%2FComfyScript%2Fmain%2Fpyproject.toml) [![License](https://img.shields.io/pypi/l/comfy-script)](LICENSE.txt)
 
 A Python front end and library for [ComfyUI](https://github.com/comfyanonymous/ComfyUI).
 
-![](docs/images/README/plot.png)
+![](docs/imgs/README/plot.png)
 
 It has the following use cases:
 - Serving as a [human-readable format](https://github.com/comfyanonymous/ComfyUI/issues/612) for ComfyUI's workflows.
 
   This makes it easy to compare and reuse different parts of one's workflows.
   
   It is also possible to train LLMs to generate workflows, since many LLMs can handle Python code relatively well. This approach can be more powerful than just asking LLMs for some hardcoded parameters.
@@ -86,30 +86,30 @@
 ## Transpiler
 The transpiler can translate ComfyUI's workflows to ComfyScript.
 
 When ComfyScript is installed as custom nodes, `SaveImage` and similar nodes will be hooked to automatically save the script as the image's metadata. The script will also be printed to the terminal.
 
 For example, here is a workflow in ComfyUI:
 
-![](docs/images/README/workflow.png)
+![](docs/imgs/README/workflow.png)
 
 ComfyScript translated from it:
 ```python
 model, clip, vae = CheckpointLoaderSimple('v1-5-pruned-emaonly.ckpt')
 conditioning = CLIPTextEncode('beautiful scenery nature glass bottle landscape, , purple galaxy bottle,', clip)
 conditioning2 = CLIPTextEncode('text, watermark', clip)
 latent = EmptyLatentImage(512, 512, 1)
 latent = KSampler(model, 156680208700286, 20, 8, 'euler', 'normal', conditioning, conditioning2, latent, 1)
 image = VAEDecode(latent, vae)
 SaveImage(image, 'ComfyUI')
 ```
 
 If there two or more `SaveImage` nodes in one workflow, only the necessary inputs of each node will be translated to scripts. For example, here is a 2 pass txt2img (hires fix) workflow:
 
-![](docs/images/README/workflow2.png)
+![](docs/imgs/README/workflow2.png)
 
 ComfyScript saved for each of the two saved image are respectively:
 1. ```python
    model, clip, vae = CheckpointLoaderSimple('v2-1_768-ema-pruned.ckpt')
    conditioning = CLIPTextEncode('masterpiece HDR victorian portrait painting of woman, blonde hair, mountain nature, blue sky', clip)
    conditioning2 = CLIPTextEncode('bad hands, text, watermark', clip)
    latent = EmptyLatentImage(768, 768, 1)
@@ -127,15 +127,15 @@
    latent2 = KSampler(model, 469771404043268, 14, 8, 'dpmpp_2m', 'simple', conditioning, conditioning2, latent2, 0.5)
    image = VAEDecode(latent2, vae)
    SaveImage(image, 'ComfyUI')
    ```
 
 Comparing scripts:
 
-![](docs/images/README/diff.png)
+![](docs/imgs/README/diff.png)
 
 To control these features, see [settings.example.toml](settings.example.toml).
 
 You can also use the transpiler via the [CLI](docs/Transpiler.md#cli).
 
 ## Runtime
 With the runtime, one can run ComfyScript like this:
@@ -156,15 +156,15 @@
 
 A Jupyter Notebook example is available at [`examples/runtime.ipynb`](examples/runtime.ipynb). (Files under `examples` directory will be ignored by Git and you can put your personal notebooks there.)
 
 - [Type stubs](https://typing.readthedocs.io/en/latest/source/stubs.html) will be generated at `comfy_script/runtime/nodes.pyi` after loading. Mainstream code editors (e.g. [VS Code](https://code.visualstudio.com/docs/languages/python)) can use them to help with coding:
 
   | | |
   | --- | --- |
-  | ![](docs/images/README/type-stubs.png) | ![](docs/images/README/type-stubs2.png) |
+  | ![](docs/imgs/README/type-stubs.png) | ![](docs/imgs/README/type-stubs2.png) |
 
   [Python enumerations](https://docs.python.org/3/howto/enum.html) are generated for all arguments provding the value list. So instead of copying and pasting strings like `'v1-5-pruned-emaonly.ckpt'`, you can use:
   ```python
   Checkpoints.v1_5_pruned_emaonly
   # or
   CheckpointLoaderSimple.ckpt_name.v1_5_pruned_emaonly
   ```
@@ -219,15 +219,15 @@
         latent = LatentUpscaleBy(latent, scale_by=2)
         latent = KSampler(model2, seed, steps=15, cfg=6, sampler_name='uni_pc',
                           positive=CLIPTextEncode(f'{color}, {pos}', clip2), negative=CLIPTextEncode(neg, clip2),
                           latent_image=latent, denoise=0.6)
         SaveImage(VAEDecode(latent, vae2), f'{seed} {color} hires')
 ```
 
-![](docs/images/README/plot.png)
+![](docs/imgs/README/plot.png)
 
 #### Auto queue
 Automatically queue new workflows when the queue becomes empty.
 
 For example, one can use [comfyui-photoshop](https://github.com/NimaNzrii/comfyui-photoshop) (currently a bit buggy) to automatically do img2img with the image in Photoshop when it changes:
 ```python
 def f(wf):
@@ -242,15 +242,15 @@
                         positive=CLIPTextEncode(pos, clip), negative=CLIPTextEncode(neg, clip),
                         latent_image=latent, denoise=0.8)
     PreviewImage(VAEDecode(latent, vae))
 queue.when_empty(f)
 ```
 Screenshot:
 
-![](docs/images/README/auto-queue.png)
+![](docs/imgs/README/auto-queue.png)
 
 #### Select and process
 For example, to generate 3 images at once, and then let the user decide which ones they want to hires fix:
 ```python
 import ipywidgets as widgets
 
 queue.watch_display(False, False)
@@ -291,18 +291,18 @@
     grid[0, i] = widgets.VBox(children=(image, button))
 display(grid)
 ```
 This example uses [ipywidgets](https://github.com/jupyter-widgets/ipywidgets) for the GUI, but other GUI frameworks can be used as well.
 
 Screenshot:
 
-![](docs/images/README/select.png)
+![](docs/imgs/README/select.png)
 
 ## [Documentation](docs/README.md)
 - [Runtime](docs/Runtime.md)
-- [Images](docs/Image/README.md)
+- [Images](docs/Images/README.md)
 - [Models](docs/Models/README.md)
 - [Additional Nodes](docs/Nodes/README.md)
 - [Transpiler](docs/Transpiler.md)
 
 
 [^graph-gui]: [I hate nodes. (No offense comfyui) : StableDiffusion](https://www.reddit.com/r/StableDiffusion/comments/15cr5xx/i_hate_nodes_no_offense_comfyui/)
```

### Comparing `comfy_script-0.5.0a4/pyproject.toml` & `comfy_script-0.5.0a5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "comfy-script"
-version = "0.5.0a4"
+version = "0.5.0a5"
 description = "A Python front end and library for ComfyUI"
 readme = "README.md"
 # ComfyUI: >=3.8
 # comfyui: >=3.9
 # >=3.6 is required to preserve insertion order of input types
 requires-python = ">=3.9"
 authors = [
```

### Comparing `comfy_script-0.5.0a4/PKG-INFO` & `comfy_script-0.5.0a5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comfy-script
-Version: 0.5.0a4
+Version: 0.5.0a5
 Summary: A Python front end and library for ComfyUI
 Project-URL: Homepage, https://github.com/Chaoses-Ib/ComfyScript
 Project-URL: Issues, https://github.com/Chaoses-Ib/ComfyScript/issues
 Author-email: Chaoses-Ib <Chaos-es@outlook.com>
 License-File: LICENSE.txt
 Keywords: comfyui
 Classifier: License :: OSI Approved :: MIT License
@@ -51,15 +51,15 @@
 Description-Content-Type: text/markdown
 
 # ComfyScript
 [![PyPI - Version](https://img.shields.io/pypi/v/comfy-script)](https://pypi.org/project/comfy-script) ![Python Version from PEP 621 TOML](https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2FChaoses-Ib%2FComfyScript%2Fmain%2Fpyproject.toml) [![License](https://img.shields.io/pypi/l/comfy-script)](LICENSE.txt)
 
 A Python front end and library for [ComfyUI](https://github.com/comfyanonymous/ComfyUI).
 
-![](docs/images/README/plot.png)
+![](docs/imgs/README/plot.png)
 
 It has the following use cases:
 - Serving as a [human-readable format](https://github.com/comfyanonymous/ComfyUI/issues/612) for ComfyUI's workflows.
 
   This makes it easy to compare and reuse different parts of one's workflows.
   
   It is also possible to train LLMs to generate workflows, since many LLMs can handle Python code relatively well. This approach can be more powerful than just asking LLMs for some hardcoded parameters.
@@ -138,30 +138,30 @@
 ## Transpiler
 The transpiler can translate ComfyUI's workflows to ComfyScript.
 
 When ComfyScript is installed as custom nodes, `SaveImage` and similar nodes will be hooked to automatically save the script as the image's metadata. The script will also be printed to the terminal.
 
 For example, here is a workflow in ComfyUI:
 
-![](docs/images/README/workflow.png)
+![](docs/imgs/README/workflow.png)
 
 ComfyScript translated from it:
 ```python
 model, clip, vae = CheckpointLoaderSimple('v1-5-pruned-emaonly.ckpt')
 conditioning = CLIPTextEncode('beautiful scenery nature glass bottle landscape, , purple galaxy bottle,', clip)
 conditioning2 = CLIPTextEncode('text, watermark', clip)
 latent = EmptyLatentImage(512, 512, 1)
 latent = KSampler(model, 156680208700286, 20, 8, 'euler', 'normal', conditioning, conditioning2, latent, 1)
 image = VAEDecode(latent, vae)
 SaveImage(image, 'ComfyUI')
 ```
 
 If there two or more `SaveImage` nodes in one workflow, only the necessary inputs of each node will be translated to scripts. For example, here is a 2 pass txt2img (hires fix) workflow:
 
-![](docs/images/README/workflow2.png)
+![](docs/imgs/README/workflow2.png)
 
 ComfyScript saved for each of the two saved image are respectively:
 1. ```python
    model, clip, vae = CheckpointLoaderSimple('v2-1_768-ema-pruned.ckpt')
    conditioning = CLIPTextEncode('masterpiece HDR victorian portrait painting of woman, blonde hair, mountain nature, blue sky', clip)
    conditioning2 = CLIPTextEncode('bad hands, text, watermark', clip)
    latent = EmptyLatentImage(768, 768, 1)
@@ -179,15 +179,15 @@
    latent2 = KSampler(model, 469771404043268, 14, 8, 'dpmpp_2m', 'simple', conditioning, conditioning2, latent2, 0.5)
    image = VAEDecode(latent2, vae)
    SaveImage(image, 'ComfyUI')
    ```
 
 Comparing scripts:
 
-![](docs/images/README/diff.png)
+![](docs/imgs/README/diff.png)
 
 To control these features, see [settings.example.toml](settings.example.toml).
 
 You can also use the transpiler via the [CLI](docs/Transpiler.md#cli).
 
 ## Runtime
 With the runtime, one can run ComfyScript like this:
@@ -208,15 +208,15 @@
 
 A Jupyter Notebook example is available at [`examples/runtime.ipynb`](examples/runtime.ipynb). (Files under `examples` directory will be ignored by Git and you can put your personal notebooks there.)
 
 - [Type stubs](https://typing.readthedocs.io/en/latest/source/stubs.html) will be generated at `comfy_script/runtime/nodes.pyi` after loading. Mainstream code editors (e.g. [VS Code](https://code.visualstudio.com/docs/languages/python)) can use them to help with coding:
 
   | | |
   | --- | --- |
-  | ![](docs/images/README/type-stubs.png) | ![](docs/images/README/type-stubs2.png) |
+  | ![](docs/imgs/README/type-stubs.png) | ![](docs/imgs/README/type-stubs2.png) |
 
   [Python enumerations](https://docs.python.org/3/howto/enum.html) are generated for all arguments provding the value list. So instead of copying and pasting strings like `'v1-5-pruned-emaonly.ckpt'`, you can use:
   ```python
   Checkpoints.v1_5_pruned_emaonly
   # or
   CheckpointLoaderSimple.ckpt_name.v1_5_pruned_emaonly
   ```
@@ -271,15 +271,15 @@
         latent = LatentUpscaleBy(latent, scale_by=2)
         latent = KSampler(model2, seed, steps=15, cfg=6, sampler_name='uni_pc',
                           positive=CLIPTextEncode(f'{color}, {pos}', clip2), negative=CLIPTextEncode(neg, clip2),
                           latent_image=latent, denoise=0.6)
         SaveImage(VAEDecode(latent, vae2), f'{seed} {color} hires')
 ```
 
-![](docs/images/README/plot.png)
+![](docs/imgs/README/plot.png)
 
 #### Auto queue
 Automatically queue new workflows when the queue becomes empty.
 
 For example, one can use [comfyui-photoshop](https://github.com/NimaNzrii/comfyui-photoshop) (currently a bit buggy) to automatically do img2img with the image in Photoshop when it changes:
 ```python
 def f(wf):
@@ -294,15 +294,15 @@
                         positive=CLIPTextEncode(pos, clip), negative=CLIPTextEncode(neg, clip),
                         latent_image=latent, denoise=0.8)
     PreviewImage(VAEDecode(latent, vae))
 queue.when_empty(f)
 ```
 Screenshot:
 
-![](docs/images/README/auto-queue.png)
+![](docs/imgs/README/auto-queue.png)
 
 #### Select and process
 For example, to generate 3 images at once, and then let the user decide which ones they want to hires fix:
 ```python
 import ipywidgets as widgets
 
 queue.watch_display(False, False)
@@ -343,18 +343,18 @@
     grid[0, i] = widgets.VBox(children=(image, button))
 display(grid)
 ```
 This example uses [ipywidgets](https://github.com/jupyter-widgets/ipywidgets) for the GUI, but other GUI frameworks can be used as well.
 
 Screenshot:
 
-![](docs/images/README/select.png)
+![](docs/imgs/README/select.png)
 
 ## [Documentation](docs/README.md)
 - [Runtime](docs/Runtime.md)
-- [Images](docs/Image/README.md)
+- [Images](docs/Images/README.md)
 - [Models](docs/Models/README.md)
 - [Additional Nodes](docs/Nodes/README.md)
 - [Transpiler](docs/Transpiler.md)
 
 
 [^graph-gui]: [I hate nodes. (No offense comfyui) : StableDiffusion](https://www.reddit.com/r/StableDiffusion/comments/15cr5xx/i_hate_nodes_no_offense_comfyui/)
```

