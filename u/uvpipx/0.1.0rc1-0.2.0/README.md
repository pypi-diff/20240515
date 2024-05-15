# Comparing `tmp/uvpipx-0.1.0rc1.tar.gz` & `tmp/uvpipx-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uvpipx-0.1.0rc1.tar", max compression
+gzip compressed data, was "uvpipx-0.2.0.tar", max compression
```

## Comparing `uvpipx-0.1.0rc1.tar` & `uvpipx-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35143 2024-05-14 20:47:29.583233 uvpipx-0.1.0rc1/LICENSE
--rw-r--r--   0        0        0     1083 2024-05-14 20:47:29.583233 uvpipx-0.1.0rc1/README.md
--rw-r--r--   0        0        0      768 2024-05-14 20:47:29.583233 uvpipx-0.1.0rc1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-14 20:47:29.625233 uvpipx-0.1.0rc1/uvpipx/__init__.py
--rw-r--r--   0        0        0     1948 2024-05-14 20:47:29.584233 uvpipx-0.1.0rc1/uvpipx/__main__.py
--rw-r--r--   0        0        0     1868 2024-05-14 20:47:29.584233 uvpipx-0.1.0rc1/uvpipx/cmd_launcher.py
--rw-r--r--   0        0        0     1162 2024-05-14 20:47:29.585233 uvpipx-0.1.0rc1/uvpipx/config.py
--rw-r--r--   0        0        0        0 2024-05-14 20:47:29.625233 uvpipx-0.1.0rc1/uvpipx/internal_libs/__init__.py
--rw-r--r--   0        0        0     7482 2024-05-14 20:47:29.585233 uvpipx-0.1.0rc1/uvpipx/internal_libs/args.py
--rw-r--r--   0        0        0     3229 2024-05-14 20:47:29.585233 uvpipx-0.1.0rc1/uvpipx/internal_libs/colors.py
--rw-r--r--   0        0        0      979 2024-05-14 20:47:29.585233 uvpipx-0.1.0rc1/uvpipx/internal_libs/http_utils.py
--rw-r--r--   0        0        0     6973 2024-05-14 20:47:29.585233 uvpipx-0.1.0rc1/uvpipx/internal_libs/misc.py
--rw-r--r--   0        0        0     3330 2024-05-14 20:47:29.585233 uvpipx-0.1.0rc1/uvpipx/internal_libs/print.py
--rwxr-xr-x   0        0        0     6389 2024-05-14 20:47:29.585233 uvpipx-0.1.0rc1/uvpipx/uvpipx.py
--rw-r--r--   0        0        0     2462 2024-05-14 20:47:29.586233 uvpipx-0.1.0rc1/uvpipx/uvpipx_args.py
--rw-r--r--   0        0        0     2568 2024-05-14 20:47:29.586233 uvpipx-0.1.0rc1/uvpipx/uvpipx_infos.py
--rw-r--r--   0        0        0     1868 1970-01-01 00:00:00.000000 uvpipx-0.1.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    35143 2024-05-15 20:16:15.404575 uvpipx-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1083 2024-05-15 20:16:15.405576 uvpipx-0.2.0/README.md
+-rw-r--r--   0        0        0      763 2024-05-15 20:16:15.405576 uvpipx-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-15 20:16:15.448575 uvpipx-0.2.0/uvpipx/__init__.py
+-rw-r--r--   0        0        0     2186 2024-05-15 20:16:15.406576 uvpipx-0.2.0/uvpipx/__main__.py
+-rw-r--r--   0        0        0     1995 2024-05-15 20:16:15.406576 uvpipx-0.2.0/uvpipx/cmd_launcher.py
+-rw-r--r--   0        0        0     1157 2024-05-15 20:16:15.406576 uvpipx-0.2.0/uvpipx/config.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:16:15.448575 uvpipx-0.2.0/uvpipx/internal_libs/__init__.py
+-rw-r--r--   0        0        0     7673 2024-05-15 20:16:15.407575 uvpipx-0.2.0/uvpipx/internal_libs/args.py
+-rw-r--r--   0        0        0     3550 2024-05-15 20:16:15.407575 uvpipx-0.2.0/uvpipx/internal_libs/colors.py
+-rw-r--r--   0        0        0      979 2024-05-15 20:16:15.407575 uvpipx-0.2.0/uvpipx/internal_libs/http_utils.py
+-rw-r--r--   0        0        0     6971 2024-05-15 20:16:15.407575 uvpipx-0.2.0/uvpipx/internal_libs/misc.py
+-rw-r--r--   0        0        0     3326 2024-05-15 20:16:15.407575 uvpipx-0.2.0/uvpipx/internal_libs/print.py
+-rwxr-xr-x   0        0        0     6577 2024-05-15 20:16:15.407575 uvpipx-0.2.0/uvpipx/uvpipx.py
+-rw-r--r--   0        0        0     2457 2024-05-15 20:16:15.407575 uvpipx-0.2.0/uvpipx/uvpipx_args.py
+-rw-r--r--   0        0        0     2580 2024-05-15 20:16:15.408576 uvpipx-0.2.0/uvpipx/uvpipx_infos.py
+-rw-r--r--   0        0        0     1865 1970-01-01 00:00:00.000000 uvpipx-0.2.0/PKG-INFO
```

### Comparing `uvpipx-0.1.0rc1/LICENSE` & `uvpipx-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uvpipx-0.1.0rc1/README.md` & `uvpipx-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `uvpipx-0.1.0rc1/pyproject.toml` & `uvpipx-0.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "uvpipx"
 description = "A small tool like pipx using uv behind the scene. Fast, Small ..."
-version = "0.1.0-rc.1"  # to bump
+version = "0.2.0"  # to bump
 authors = ["Pytgaen <32298455+pytgaen@users.noreply.github.com>"]
 readme = "README.md"
 license = "GPL"
 
 homepage = "https://gitlab.com/pytgaen-group/uvpipx"
 repository = "https://gitlab.com/pytgaen-group/uvpipx"
 # documentation = "https://gitlab.com/pytgaen-group/uvpipx" # gitlab page
```

### Comparing `uvpipx-0.1.0rc1/uvpipx/__main__.py` & `uvpipx-0.2.0/uvpipx/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,52 @@
 import sys
 
+from uvpipx.internal_libs.colors import Painter
+
 __author__ = "Gaëtan Montury"
 __copyright__ = "Copyright (c) 2024-2024 Gaëtan Montury"
 __license__ = """GNU GENERAL PUBLIC LICENSE refer to file LICENSE in repo"""
-__version__ = "0.1.0-rc.1"  # to bump
+__version__ = "0.2.0"  # to bump
 __maintainer__ = "Gaëtan Montury"
 __email__ = "#"
 __status__ = "Development"
 
 from uvpipx.cmd_launcher import ensurepath, info, install, uninstall, uvpipx_list, venv
 from uvpipx.internal_libs.print import max_string_length_per_column, wrap_text_in_table
 from uvpipx.uvpipx_args import arg_parser
 
 
 def show_main_help() -> None:
-    print("uvpipx general help\n")
+    print(
+        Painter.parse_color_tags("<ST_UNDERLINE>uvpipx general help</ST_UNDERLINE>\n"),
+    )
 
     print("uvpipx cmd [--help] ... parameters ...\n\ncmd can be:")
     help_ = [[f"{k}", f"{v.help}"] for k, v in arg_parser.items()]
     size_col = max_string_length_per_column(help_)
 
     wrapped = wrap_text_in_table(help_, [size_col[0], 100 - size_col[0]])
     for row in wrapped:
         for ss in [list(sub_row) for sub_row in zip(*row)]:
-            print(" | ".join(ss))
+            print("  " + (" | ".join(ss)).rstrip())
         # print()
 
     print()
 
 
 def main() -> None:
     """uv pipx
 
     like pipx but with uv ... intent to be miniamist, small and so fast !
     """
-    print(f"uvpipx version {__version__}\n")
+    print(
+        Painter.parse_color_tags(
+            f"<BRIGHT_WHITE>uvpipx</BRIGHT_WHITE> version <CYAN>{__version__}</CYAN>\n",
+        ),
+    )
     if len(sys.argv) <= 1 or (len(sys.argv) == 2 and sys.argv[1] in ["-h", "--help"]):
         show_main_help()
         sys.exit(0)
 
     if sys.argv[1] == "install":
         install(arg_parser["install"])
```

### Comparing `uvpipx-0.1.0rc1/uvpipx/cmd_launcher.py` & `uvpipx-0.2.0/uvpipx/cmd_launcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 __author__ = "Gaëtan Montury"
 __copyright__ = "Copyright (c) 2024-2024 Gaëtan Montury"
 __license__ = """GNU GENERAL PUBLIC LICENSE refer to file LICENSE in repo"""
-__version__ = "0.1.0-rc.1"  # to bump
+__version__ = "0.2.0"  # to bump
 __maintainer__ = "Gaëtan Montury"
 __email__ = "#"
 __status__ = "Development"
 
 import os
 import sys
 
 from uvpipx import uvpipx, uvpipx_infos
 from uvpipx.internal_libs.args import ArgParser
-from uvpipx.internal_libs.misc import log_debug
+from uvpipx.internal_libs.misc import Elapser, log_debug, log_info
 
 
 def common_args(argp: ArgParser) -> None:
     argp.parse(sys.argv[2:])
     os.environ["UVPIPX_SHOW_DEBUG_LEVEL"] = str(
         argp.args["--verbose"].defaulted_value(),
     )
@@ -27,34 +27,37 @@
 
 
 def install(argp: ArgParser) -> None:
     """install package locally in their own venv"""
 
     common_args(argp)
 
-    uvpipx.install(
-        argp.args["python_pkg"].value,
-        expose_bin_names=argp.args["--expose"].defaulted_value(),
-    )
+    with Elapser() as ela:
+        uvpipx.install(
+            argp.args["python_pkg"].value,
+            expose_bin_names=argp.args["--expose"].defaulted_value(),
+        )
+
+    log_info(f"\n 🏁 Finish install  ⏱️  {ela.elapsed_second}")
 
 
 def ensurepath(argp: ArgParser) -> None:
     """help to define PATH"""
 
     common_args(argp)
 
-    uvpipx.uvpipx_infos.ensurepath()
+    uvpipx_infos.ensurepath()
 
 
 def uvpipx_list(argp: ArgParser) -> None:
     """show the list of uvpipx venv"""
 
     common_args(argp)
 
-    uvpipx.uvpipx_list()
+    uvpipx_infos.uvpipx_list()
 
 
 def info(
     argp: ArgParser,
 ) -> None:
     """show the list of uvpipx venv"""
```

### Comparing `uvpipx-0.1.0rc1/uvpipx/config.py` & `uvpipx-0.2.0/uvpipx/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 __author__ = "Gaëtan Montury"
 __copyright__ = "Copyright (c) 2024-2024 Gaëtan Montury"
 __license__ = """GNU GENERAL PUBLIC LICENSE refer to file LICENSE in repo"""
-__version__ = "0.1.0-rc.1"  # to bump
+__version__ = "0.2.0"  # to bump
 __maintainer__ = "Gaëtan Montury"
 __email__ = "#"
 __status__ = "Development"
 
 
 import os
 from pathlib import Path
```

### Comparing `uvpipx-0.1.0rc1/uvpipx/internal_libs/args.py` & `uvpipx-0.2.0/uvpipx/internal_libs/args.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """intend to be independent(internal one file) args parser ... be cool enougth"""
 
 from __future__ import annotations
 
+from uvpipx.internal_libs.colors import Painter
+
 __author__ = "Gaëtan Montury"
 __copyright__ = "Copyright (c) 2024-2024 Gaëtan Montury"
 __license__ = """GNU GENERAL PUBLIC LICENSE refer to file LICENSE in repo"""
-__version__ = "0.1.0-rc.1"  # to bump
+__version__ = "0.2.0"  # to bump
 __maintainer__ = "Gaëtan Montury"
 __email__ = "#"
 __status__ = "Development"
 
 
 from dataclasses import dataclass, field
 from enum import Enum
@@ -182,15 +184,19 @@
         return 1, self.args[i_pos_name]
 
         # TODO finish check
         # all positional have a value
 
     def print_help(self) -> None:
         if self.help:
-            print(self.help + "\n")
+            print(
+                Painter.parse_color_tags(f"<ST_UNDERLINE>{self.help}</ST_UNDERLINE>\n"),
+            )
+
+        # TODO show command line argument
 
         info_not_option = []
         info_option = []
         for arg in self.args_def:
             if arg.name.startswith("-"):
                 opt = ", ".join([arg.name, *arg.alternate_name])
                 next_value = (
@@ -205,9 +211,9 @@
         infos = info_not_option + info_option
 
         size_col = max_string_length_per_column(infos)
 
         wrapped = wrap_text_in_table(infos, [size_col[0], 100 - size_col[0]])
         for row in wrapped:
             for ss in [list(sub_row) for sub_row in zip(*row)]:
-                print(" | ".join(ss))
+                print("  " + (" | ".join(ss)).rstrip())
             print()
```

### Comparing `uvpipx-0.1.0rc1/uvpipx/internal_libs/colors.py` & `uvpipx-0.2.0/uvpipx/internal_libs/colors.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import annotations
 
 __author__ = "Gaëtan Montury"
 __copyright__ = "Copyright (c) 2024-2024 Gaëtan Montury"
 __license__ = """GNU GENERAL PUBLIC LICENSE refer to file LICENSE in repo"""
-__version__ = "0.1.0-rc.1"  # to bump
+__version__ = "0.2.0"  # to bump
 __maintainer__ = "Gaëtan Montury"
 __email__ = "#"
 __status__ = "Development"
 
 
+import os
 import re
 from enum import Enum
 from typing import List
 
 
 class Color(Enum):
     # Foreground colors
@@ -68,31 +69,40 @@
             return f"\033[38;2;{r};{g};{b}m"  # ANSI escape for foreground color
 
 
 class Painter:
     @staticmethod
     def hex_color(hexcode: str, background: bool = False) -> str:
         """Generates an ANSI escape sequence from a hex color code."""
+        if os.getenv("NO_ANSI_COLOR", "false").lower() not in ["false", "0"]:
+            return ""
+
         hexcode = hexcode.strip("#")
         r, g, b = int(hexcode[:2], 16), int(hexcode[2:4], 16), int(hexcode[4:6], 16)
         return Color.rgb_color(r, g, b, background)
 
     @staticmethod
     def color_str(message: str, *styles: List[Color]) -> str:
+        if os.getenv("NO_ANSI_COLOR", "false").lower() not in ["false", "0"]:
+            return message
+
         style_codes = "".join(style.value for style in styles)
         return f"{style_codes}{message}{Color.ST_RESET.value}"
 
     @staticmethod
     def parse_color_tags(message: str) -> str:
         pattern = re.compile(r"</?([A-Z_]+)>")
         styles_set = set()
         message_ = message
 
         # Function to process each match
         def replace_tag(tag: str) -> str:
+            if os.getenv("NO_ANSI_COLOR", "false").lower() not in ["false", "0"]:
+                return ""
+
             tag_ = tag[1:-1]
             if not tag_.startswith("/"):
                 styles_set.add(tag_)
                 return Color[tag_].value
 
             styles_set.remove(tag_[1:])
             ansi_style = Color["ST_RESET"].value
```

### Comparing `uvpipx-0.1.0rc1/uvpipx/internal_libs/http_utils.py` & `uvpipx-0.2.0/uvpipx/internal_libs/http_utils.py`

 * *Files identical despite different names*

### Comparing `uvpipx-0.1.0rc1/uvpipx/internal_libs/misc.py` & `uvpipx-0.2.0/uvpipx/internal_libs/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 __author__ = "Gaëtan Montury"
 __copyright__ = "Copyright (c) 2024-2024 Gaëtan Montury"
 __license__ = """GNU GENERAL PUBLIC LICENSE refer to file LICENSE in repo"""
-__version__ = "0.1.0-rc.1"  # to bump
+__version__ = "0.2.0"  # to bump
 __maintainer__ = "Gaëtan Montury"
 __email__ = "#"
 __status__ = "Development"
 
 
 import os
 from pathlib import Path
@@ -247,12 +247,12 @@
     return encoding
 
 
 def shell_run_elapse(command: str, message: str) -> None:
     with Elapser() as ela:
         o, e, rc = shell_run(command)
 
-    log_info(f"⏱️ {message} {ela.elapsed_second}")
+    log_info(f"{message}   ⏱️  {ela.elapsed_second}")
 
 
 def command_exists(cmd: str) -> bool:
     return shutil.which(cmd) is not None
```

### Comparing `uvpipx-0.1.0rc1/uvpipx/internal_libs/print.py` & `uvpipx-0.2.0/uvpipx/internal_libs/print.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from __future__ import annotations
 
 __author__ = "Gaëtan Montury"
 __copyright__ = "Copyright (c) 2024-2024 Gaëtan Montury"
 __license__ = """GNU GENERAL PUBLIC LICENSE refer to file LICENSE in repo"""
-__version__ = "0.1.0-rc.1"  # to bump
+__version__ = "0.2.0"  # to bump
 __maintainer__ = "Gaëtan Montury"
 __email__ = "#"
 __status__ = "Development"
 
 import textwrap
 from typing import List
 
+
 class NewLinePreservingWrapper(textwrap.TextWrapper):
     def wrap(self, text: str) -> List[str]:
         # Split the original text by new lines, process each part, then combine
         wrapped_lines = []
         for part in text.split("\n"):
             wrapped_lines.extend(super().wrap(part))
         return wrapped_lines
```

### Comparing `uvpipx-0.1.0rc1/uvpipx/uvpipx.py` & `uvpipx-0.2.0/uvpipx/uvpipx.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 from __future__ import annotations
 
 __author__ = "Gaëtan Montury"
 __copyright__ = "Copyright (c) 2024-2024 Gaëtan Montury"
 __license__ = """GNU GENERAL PUBLIC LICENSE refer to file LICENSE in repo"""
-__version__ = "0.1.0-rc.1"  # to bump
+__version__ = "0.2.0"  # to bump
 __maintainer__ = "Gaëtan Montury"
 __email__ = "#"
 __status__ = "Development"
 
 
 import json
 import os
@@ -33,15 +33,15 @@
 
 def install(
     package_name_ref: str,
     *,
     expose_bin_names: Optional[List[str]] = None,
     venv_name: Union[None, str] = None,
 ) -> None:
-    package_name = re.search(r"([^=<>]+)(==|>)*", package_name_ref)[0]
+    package_name = re.search(r"([^=<>]+)(==|>)*", package_name_ref)[1]
     venv_name_ = venv_name or package_name
     expose_bin_names_ = expose_bin_names
     if expose_bin_names_ is None:
         expose_bin_names_ = ["*"]
 
     uvpipx_dict = {
         "package_name_ref": package_name_ref,
@@ -57,24 +57,26 @@
     (config.uvpipx_venvs / venv_name_).mkdir(exist_ok=True, parents=True)
     pck_venv = config.uvpipx_venvs / venv_name_
     uvpipx_dict["uvpipx_package_path"] = pck_venv
 
     if not (pck_venv / ".venv").exists():
         shell_run_elapse(
             f"uv venv {pck_venv / '.venv'}",
-            f"uv venv {pck_venv} created",
+            f" 📦 uv venv {pck_venv} created",
         )
 
     shell_run_elapse(
         f"cd {pck_venv}; uv pip install {package_name_ref}",
-        f"uv pip install {package_name_ref} in uvpipx venv {venv_name_}",
+        f" 📥 uv pip install {package_name_ref} in uvpipx venv {venv_name_}",
     )
-    log_info(f"uvpipx venv {venv_name_} with {package_name} ready")
+    log_info(f" 🟢 uvpipx venv {venv_name_} with {package_name} ready")
     shell_run(f"cd {pck_venv}; uv pip freeze > requirements.txt")
+    print()
 
+    log_info(" 🎯 Exposing program")
     if len(expose_bin_names_) == 1:
         if expose_bin_names_[0] == "*":
             exe = find_executable(pck_venv / ".venv" / "bin")
             expose_bin_names_ = [s.name for s in exe if not s.name.startswith("python")]
         elif expose_bin_names_[0] == "_":
             expose_bin_names_ = []
 
@@ -91,19 +93,19 @@
         link_dest = config.uvpipx_local_bin / local_bin_name
         uvpipx_dict["exposed_bins"].append(
             (pck_venv / ".venv" / "bin" / venv_bin_name, link_dest),
         )
         if (pck_venv / ".venv" / "bin" / venv_bin_name).exists():
             if not link_dest.exists():
                 os.symlink(pck_venv / ".venv" / "bin" / venv_bin_name, link_dest)
-                log_info(f"Exposing program {venv_bin_name} to {link_dest}")
+                log_info(f"  📁 Exposing program {venv_bin_name} to {link_dest}")
             else:
-                log_warm(f"Link {pck_venv} already exist. Skipping {local_bin_name}!")
+                log_warm(f"  🟡 Link for {local_bin_name} already exist. Skipping !")
         else:
-            msg = f"Program {venv_bin_name} not exist in package {package_name_ref}"
+            msg = f" 🔴 Program {venv_bin_name} not exist in package {package_name_ref}"
             raise RuntimeError(
                 msg,
             )
 
     with (pck_venv / "uvpipx.json").open("w") as outfile:
         json.dump(uvpipx_dict, outfile, indent=4, default=str)
 
@@ -139,14 +141,20 @@
         raw_pipe=True,
     )
     # print(stdo)
     # print(stde, file=sys.stderr)
     sys.exit(rc)
 
 
+# TODO upgrade
+# uv pip install --upgrade jc
+# after upgrade check bin to link or unlink
+
+# TODO upgrade-all
+
 # def venv(package_name, cmdline, *, venv_name: Union[None, str] = None):
 #     """venv is specific to uvpipx. it will replace inject, runpip, uninject
 
 #     in fact runpip should be replace by uvpipx venv "truc" uv -- pip install me
 #     """
 #     venv_name_ = venv_name or package_name
 #     pck_venv = config.uvpipx_venvs / venv_name_
```

### Comparing `uvpipx-0.1.0rc1/uvpipx/uvpipx_args.py` & `uvpipx-0.2.0/uvpipx/uvpipx_args.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 __author__ = "Gaëtan Montury"
 __copyright__ = "Copyright (c) 2024-2024 Gaëtan Montury"
 __license__ = """GNU GENERAL PUBLIC LICENSE refer to file LICENSE in repo"""
-__version__ = "0.1.0-rc.1"  # to bump
+__version__ = "0.2.0"  # to bump
 __maintainer__ = "Gaëtan Montury"
 __email__ = "#"
 __status__ = "Development"
 
 
 from uvpipx.internal_libs.args import Arg, ArgParser
```

### Comparing `uvpipx-0.1.0rc1/uvpipx/uvpipx_infos.py` & `uvpipx-0.2.0/uvpipx/uvpipx_infos.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 __author__ = "Gaëtan Montury"
 __copyright__ = "Copyright (c) 2024-2024 Gaëtan Montury"
 __license__ = """GNU GENERAL PUBLIC LICENSE refer to file LICENSE in repo"""
-__version__ = "0.1.0-rc.1"  # to bump
+__version__ = "0.2.0"  # to bump
 __maintainer__ = "Gaëtan Montury"
 __email__ = "#"
 __status__ = "Development"
 
 
 import json
 import os
@@ -85,14 +85,16 @@
 def uvpipx_list() -> None:
     infos = f"""uvpipx venvs are in {config.uvpipx_venvs}
 apps are exposed at {config.uvpipx_local_bin} 
 
 """
     nb = 0
     if config.uvpipx_venvs.exists():
-        for nb, pck_venv in enumerate(config.uvpipx_venvs.iterdir()):  # noqa: B007
+        for pck_venv in config.uvpipx_venvs.iterdir():
             infos += _info(pck_venv)
+            infos += "\n"
+            nb += 1
 
     if nb == 0:
         infos += "Nothing is installed !"
 
     print(infos)
```

### Comparing `uvpipx-0.1.0rc1/PKG-INFO` & `uvpipx-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uvpipx
-Version: 0.1.0rc1
+Version: 0.2.0
 Summary: A small tool like pipx using uv behind the scene. Fast, Small ...
 Home-page: https://gitlab.com/pytgaen-group/uvpipx
 License: GPL
 Author: Pytgaen
 Author-email: 32298455+pytgaen@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

