# Comparing `tmp/karp_lex_types-0.6.2.tar.gz` & `tmp/karp_lex_types-0.6.4.tar.gz`

## Comparing `karp_lex_types-0.6.2.tar` & `karp_lex_types-0.6.4.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 karp_lex_types-0.6.2/.bumpversion.cfg
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 karp_lex_types-0.6.2/CHANGELOG.md
--rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 karp_lex_types-0.6.2/Makefile
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 karp_lex_types-0.6.2/mypy.ini
--rw-r--r--   0        0        0    31930 2020-02-02 00:00:00.000000 karp_lex_types-0.6.2/pdm.lock
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 karp_lex_types-0.6.2/ruff.toml
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 karp_lex_types-0.6.2/src/karp_lex_types/__init__.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 karp_lex_types-0.6.2/src/karp_lex_types/alias_generators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 karp_lex_types-0.6.2/src/karp_lex_types/py.typed
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 karp_lex_types-0.6.2/src/karp_lex_types/commands/__init__.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 karp_lex_types-0.6.2/src/karp_lex_types/commands/base.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 karp_lex_types-0.6.2/src/karp_lex_types/commands/entry_commands.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 karp_lex_types-0.6.2/src/karp_lex_types/commands/entry_repo_commands.py
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 karp_lex_types-0.6.2/src/karp_lex_types/commands/resource_commands.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 karp_lex_types-0.6.2/src/karp_lex_types/dtos/__init__.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 karp_lex_types-0.6.2/src/karp_lex_types/dtos/entry_dto.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 karp_lex_types-0.6.2/src/karp_lex_types/value_objects/__init__.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 karp_lex_types-0.6.2/src/karp_lex_types/value_objects/unique_id.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 karp_lex_types-0.6.2/tests/conftest.py
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 karp_lex_types-0.6.2/tests/entry_dto_unit_test.py
--rw-r--r--   0        0        0    13123 2020-02-02 00:00:00.000000 karp_lex_types-0.6.2/tests/requirements-testing.lock
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 karp_lex_types-0.6.2/tests/test_entry_commands.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 karp_lex_types-0.6.2/tests/test_entry_repo_commands.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 karp_lex_types-0.6.2/tests/test_resource_commands.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 karp_lex_types-0.6.2/tests/test_unique_id.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 karp_lex_types-0.6.2/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 karp_lex_types-0.6.2/LICENSE
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 karp_lex_types-0.6.2/README.md
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 karp_lex_types-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 karp_lex_types-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 karp_lex_types-0.6.4/.bumpversion.toml
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 karp_lex_types-0.6.4/CHANGELOG.md
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 karp_lex_types-0.6.4/Makefile
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 karp_lex_types-0.6.4/cliff.toml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 karp_lex_types-0.6.4/mypy.ini
+-rw-r--r--   0        0        0    38432 2020-02-02 00:00:00.000000 karp_lex_types-0.6.4/pdm.lock
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 karp_lex_types-0.6.4/ruff.toml
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 karp_lex_types-0.6.4/src/karp_lex_types/__init__.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 karp_lex_types-0.6.4/src/karp_lex_types/alias_generators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 karp_lex_types-0.6.4/src/karp_lex_types/py.typed
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 karp_lex_types-0.6.4/src/karp_lex_types/commands/__init__.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 karp_lex_types-0.6.4/src/karp_lex_types/commands/base.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 karp_lex_types-0.6.4/src/karp_lex_types/commands/entry_commands.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 karp_lex_types-0.6.4/src/karp_lex_types/commands/entry_repo_commands.py
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 karp_lex_types-0.6.4/src/karp_lex_types/commands/resource_commands.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 karp_lex_types-0.6.4/src/karp_lex_types/dtos/__init__.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 karp_lex_types-0.6.4/src/karp_lex_types/dtos/entry_dto.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 karp_lex_types-0.6.4/src/karp_lex_types/value_objects/__init__.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 karp_lex_types-0.6.4/src/karp_lex_types/value_objects/unique_id.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 karp_lex_types-0.6.4/tests/conftest.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 karp_lex_types-0.6.4/tests/entry_dto_unit_test.py
+-rw-r--r--   0        0        0    15783 2020-02-02 00:00:00.000000 karp_lex_types-0.6.4/tests/requirements-testing.lock
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 karp_lex_types-0.6.4/tests/test_entry_commands.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 karp_lex_types-0.6.4/tests/test_entry_repo_commands.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 karp_lex_types-0.6.4/tests/test_resource_commands.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 karp_lex_types-0.6.4/tests/test_unique_id.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 karp_lex_types-0.6.4/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 karp_lex_types-0.6.4/LICENSE
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 karp_lex_types-0.6.4/README.md
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 karp_lex_types-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 karp_lex_types-0.6.4/PKG-INFO
```

### Comparing `karp_lex_types-0.6.2/CHANGELOG.md` & `karp_lex_types-0.6.4/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## [0.6.3] - 2024-05-14
+
+### Miscellaneous Tasks
+
+- Rename project to karp-lex-types
+
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
 
 ## Latest Changes
 
 ## 0.6.0
 
 - Update pydantic to V2.
```

### Comparing `karp_lex_types-0.6.2/Makefile` & `karp_lex_types-0.6.4/Makefile`

 * *Files 0% similar despite different names*

```diff
@@ -152,14 +152,15 @@
 # we use lock extension so that dependabot doesn't pick up changes in this file
 tests/requirements-testing.lock: pyproject.toml pdm.lock
 	pdm export --dev --format requirements --output $@
 
 .PHONY: update-changelog
 update-changelog: CHANGELOG.md
 
+.PHONY: CHANGELOG.md
 CHANGELOG.md:
 	git cliff --unreleased --prepend $@
 
 # update snapshots for `syrupy`
 .PHONY: snapshot-update
 snapshot-update:
 	${INVENV} pytest --snapshot-update
```

### Comparing `karp_lex_types-0.6.2/pdm.lock` & `karp_lex_types-0.6.4/pdm.lock`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,80 @@
 # This file is @generated by PDM.
 # It is not intended for manual editing.
 
 [metadata]
 groups = ["default", "dev"]
 strategy = ["cross_platform", "inherit_metadata"]
 lock_version = "4.4.1"
-content_hash = "sha256:17a38999607b0e801b53142c32b17b3e39e50c38b9d8346480f2a9db8223ef3e"
+content_hash = "sha256:e40ce2d2f35abe5e0aff464f3cd12f3843d3017fb9b4ec4e84845112a0a2ee5b"
 
 [[package]]
 name = "annotated-types"
 version = "0.6.0"
 requires_python = ">=3.8"
 summary = "Reusable constraint types to use with typing.Annotated"
-groups = ["default"]
+groups = ["default", "dev"]
 files = [
     {file = "annotated_types-0.6.0-py3-none-any.whl", hash = "sha256:0641064de18ba7a25dee8f96403ebc39113d0cb953a01429249d5c7564666a43"},
     {file = "annotated_types-0.6.0.tar.gz", hash = "sha256:563339e807e53ffd9c267e99fc6d9ea23eb8443c08f112651963e24e22f84a5d"},
 ]
 
 [[package]]
-name = "bump2version"
-version = "1.0.1"
-requires_python = ">=3.5"
-summary = "Version-bump your software with a single command!"
+name = "bracex"
+version = "2.4"
+requires_python = ">=3.8"
+summary = "Bash style brace expander."
 groups = ["dev"]
 files = [
-    {file = "bump2version-1.0.1-py2.py3-none-any.whl", hash = "sha256:37f927ea17cde7ae2d7baf832f8e80ce3777624554a653006c9144f8017fe410"},
-    {file = "bump2version-1.0.1.tar.gz", hash = "sha256:762cb2bfad61f4ec8e2bdf452c7c267416f8c70dd9ecb1653fd0bbb01fa936e6"},
+    {file = "bracex-2.4-py3-none-any.whl", hash = "sha256:efdc71eff95eaff5e0f8cfebe7d01adf2c8637c8c92edaf63ef348c241a82418"},
+    {file = "bracex-2.4.tar.gz", hash = "sha256:a27eaf1df42cf561fed58b7a8f3fdf129d1ea16a81e1fadd1d17989bc6384beb"},
+]
+
+[[package]]
+name = "bump-my-version"
+version = "0.21.0"
+requires_python = ">=3.8"
+summary = "Version bump your Python project"
+groups = ["dev"]
+dependencies = [
+    "click",
+    "pydantic-settings",
+    "pydantic>=2.0.0",
+    "questionary",
+    "rich",
+    "rich-click",
+    "tomlkit",
+    "wcmatch>=8.5.1",
+]
+files = [
+    {file = "bump_my_version-0.21.0-py3-none-any.whl", hash = "sha256:a614d8176b5ac0e644239c9a8a246b696d316f68406fd78b8486a9e13fc93266"},
+    {file = "bump_my_version-0.21.0.tar.gz", hash = "sha256:c3f1a31e32345679b517cbba99a0875457ee45d7ba6189fcd2a74d3ddae41515"},
+]
+
+[[package]]
+name = "click"
+version = "8.1.7"
+requires_python = ">=3.7"
+summary = "Composable command line interface toolkit"
+groups = ["dev"]
+dependencies = [
+    "colorama; platform_system == \"Windows\"",
+]
+files = [
+    {file = "click-8.1.7-py3-none-any.whl", hash = "sha256:ae74fb96c20a0277a1d615f1e4d73c8414f5a98db8b799a7931d1582f3390c28"},
+    {file = "click-8.1.7.tar.gz", hash = "sha256:ca9853ad459e787e2192211578cc907e7594e294c7ccc834310722b41b9ca6de"},
 ]
 
 [[package]]
 name = "colorama"
 version = "0.4.6"
 requires_python = "!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,!=3.6.*,>=2.7"
 summary = "Cross-platform colored terminal text."
 groups = ["dev"]
-marker = "sys_platform == \"win32\""
+marker = "sys_platform == \"win32\" or platform_system == \"Windows\""
 files = [
     {file = "colorama-0.4.6-py2.py3-none-any.whl", hash = "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"},
     {file = "colorama-0.4.6.tar.gz", hash = "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44"},
 ]
 
 [[package]]
 name = "coverage"
@@ -148,14 +183,39 @@
 groups = ["dev"]
 files = [
     {file = "iniconfig-2.0.0-py3-none-any.whl", hash = "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"},
     {file = "iniconfig-2.0.0.tar.gz", hash = "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3"},
 ]
 
 [[package]]
+name = "markdown-it-py"
+version = "3.0.0"
+requires_python = ">=3.8"
+summary = "Python port of markdown-it. Markdown parsing, done right!"
+groups = ["dev"]
+dependencies = [
+    "mdurl~=0.1",
+]
+files = [
+    {file = "markdown-it-py-3.0.0.tar.gz", hash = "sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb"},
+    {file = "markdown_it_py-3.0.0-py3-none-any.whl", hash = "sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1"},
+]
+
+[[package]]
+name = "mdurl"
+version = "0.1.2"
+requires_python = ">=3.7"
+summary = "Markdown URL utilities"
+groups = ["dev"]
+files = [
+    {file = "mdurl-0.1.2-py3-none-any.whl", hash = "sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8"},
+    {file = "mdurl-0.1.2.tar.gz", hash = "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"},
+]
+
+[[package]]
 name = "mypy"
 version = "1.10.0"
 requires_python = ">=3.8"
 summary = "Optional static typing for Python"
 groups = ["dev"]
 dependencies = [
     "mypy-extensions>=1.0.0",
@@ -202,29 +262,43 @@
 files = [
     {file = "packaging-23.2-py3-none-any.whl", hash = "sha256:8c491190033a9af7e1d931d0b5dacc2ef47509b34dd0de67ed209b5203fc88c7"},
     {file = "packaging-23.2.tar.gz", hash = "sha256:048fb0e9405036518eaaf48a55953c750c11e1a1b68e0dd1a9d62ed0c092cfc5"},
 ]
 
 [[package]]
 name = "pluggy"
-version = "1.4.0"
+version = "1.5.0"
 requires_python = ">=3.8"
 summary = "plugin and hook calling mechanisms for python"
 groups = ["dev"]
 files = [
-    {file = "pluggy-1.4.0-py3-none-any.whl", hash = "sha256:7db9f7b503d67d1c5b95f59773ebb58a8c1c288129a88665838012cfb07b8981"},
-    {file = "pluggy-1.4.0.tar.gz", hash = "sha256:8c85c2876142a764e5b7548e7d9a0e0ddb46f5185161049a79b7e974454223be"},
+    {file = "pluggy-1.5.0-py3-none-any.whl", hash = "sha256:44e1ad92c8ca002de6377e165f3e0f1be63266ab4d554740532335b9d75ea669"},
+    {file = "pluggy-1.5.0.tar.gz", hash = "sha256:2cffa88e94fdc978c4c574f15f9e59b7f4201d439195c3715ca9e2486f1d0cf1"},
+]
+
+[[package]]
+name = "prompt-toolkit"
+version = "3.0.36"
+requires_python = ">=3.6.2"
+summary = "Library for building powerful interactive command lines in Python"
+groups = ["dev"]
+dependencies = [
+    "wcwidth",
+]
+files = [
+    {file = "prompt_toolkit-3.0.36-py3-none-any.whl", hash = "sha256:aa64ad242a462c5ff0363a7b9cfe696c20d55d9fc60c11fd8e632d064804d305"},
+    {file = "prompt_toolkit-3.0.36.tar.gz", hash = "sha256:3e163f254bef5a03b146397d7c1963bd3e2812f0964bb9a24e6ec761fd28db63"},
 ]
 
 [[package]]
 name = "pydantic"
 version = "2.6.3"
 requires_python = ">=3.8"
 summary = "Data validation using Python type hints"
-groups = ["default"]
+groups = ["default", "dev"]
 dependencies = [
     "annotated-types>=0.4.0",
     "pydantic-core==2.16.3",
     "typing-extensions>=4.6.1",
 ]
 files = [
     {file = "pydantic-2.6.3-py3-none-any.whl", hash = "sha256:72c6034df47f46ccdf81869fddb81aade68056003900a8724a4f160700016a2a"},
@@ -232,15 +306,15 @@
 ]
 
 [[package]]
 name = "pydantic-core"
 version = "2.16.3"
 requires_python = ">=3.8"
 summary = ""
-groups = ["default"]
+groups = ["default", "dev"]
 dependencies = [
     "typing-extensions!=4.7.0,>=4.6.0",
 ]
 files = [
     {file = "pydantic_core-2.16.3-cp310-cp310-macosx_10_12_x86_64.whl", hash = "sha256:75b81e678d1c1ede0785c7f46690621e4c6e63ccd9192af1f0bd9d504bbb6bf4"},
     {file = "pydantic_core-2.16.3-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:9c865a7ee6f93783bd5d781af5a4c43dadc37053a5b42f7d18dc019f8c9d2bd1"},
     {file = "pydantic_core-2.16.3-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:162e498303d2b1c036b957a1278fa0899d02b2842f1ff901b6395104c5554a45"},
@@ -295,71 +369,153 @@
     {file = "pydantic_core-2.16.3-pp39-pypy39_pp73-musllinux_1_1_aarch64.whl", hash = "sha256:287073c66748f624be4cef893ef9174e3eb88fe0b8a78dc22e88eca4bc357ca6"},
     {file = "pydantic_core-2.16.3-pp39-pypy39_pp73-musllinux_1_1_x86_64.whl", hash = "sha256:ed25e1835c00a332cb10c683cd39da96a719ab1dfc08427d476bce41b92531fc"},
     {file = "pydantic_core-2.16.3-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:86b3d0033580bd6bbe07590152007275bd7af95f98eaa5bd36f3da219dcd93da"},
     {file = "pydantic_core-2.16.3.tar.gz", hash = "sha256:1cac689f80a3abab2d3c0048b29eea5751114054f032a941a32de4c852c59cad"},
 ]
 
 [[package]]
+name = "pydantic-settings"
+version = "2.2.1"
+requires_python = ">=3.8"
+summary = "Settings management using Pydantic"
+groups = ["dev"]
+dependencies = [
+    "pydantic>=2.3.0",
+    "python-dotenv>=0.21.0",
+]
+files = [
+    {file = "pydantic_settings-2.2.1-py3-none-any.whl", hash = "sha256:0235391d26db4d2190cb9b31051c4b46882d28a51533f97440867f012d4da091"},
+    {file = "pydantic_settings-2.2.1.tar.gz", hash = "sha256:00b9f6a5e95553590434c0fa01ead0b216c3e10bc54ae02e37f359948643c5ed"},
+]
+
+[[package]]
+name = "pygments"
+version = "2.18.0"
+requires_python = ">=3.8"
+summary = "Pygments is a syntax highlighting package written in Python."
+groups = ["dev"]
+files = [
+    {file = "pygments-2.18.0-py3-none-any.whl", hash = "sha256:b8e6aca0523f3ab76fee51799c488e38782ac06eafcf95e7ba832985c8e7b13a"},
+    {file = "pygments-2.18.0.tar.gz", hash = "sha256:786ff802f32e91311bff3889f6e9a86e81505fe99f2735bb6d60ae0c5004f199"},
+]
+
+[[package]]
 name = "pytest"
-version = "7.4.4"
-requires_python = ">=3.7"
+version = "8.2.0"
+requires_python = ">=3.8"
 summary = "pytest: simple powerful testing with Python"
 groups = ["dev"]
 dependencies = [
     "colorama; sys_platform == \"win32\"",
     "exceptiongroup>=1.0.0rc8; python_version < \"3.11\"",
     "iniconfig",
     "packaging",
-    "pluggy<2.0,>=0.12",
-    "tomli>=1.0.0; python_version < \"3.11\"",
+    "pluggy<2.0,>=1.5",
+    "tomli>=1; python_version < \"3.11\"",
 ]
 files = [
-    {file = "pytest-7.4.4-py3-none-any.whl", hash = "sha256:b090cdf5ed60bf4c45261be03239c2c1c22df034fbffe691abe93cd80cea01d8"},
-    {file = "pytest-7.4.4.tar.gz", hash = "sha256:2cf0005922c6ace4a3e2ec8b4080eb0d9753fdc93107415332f50ce9e7994280"},
+    {file = "pytest-8.2.0-py3-none-any.whl", hash = "sha256:1733f0620f6cda4095bbf0d9ff8022486e91892245bb9e7d5542c018f612f233"},
+    {file = "pytest-8.2.0.tar.gz", hash = "sha256:d507d4482197eac0ba2bae2e9babf0672eb333017bcedaa5fb1a3d42c1174b3f"},
 ]
 
 [[package]]
 name = "pytest-cov"
-version = "4.1.0"
-requires_python = ">=3.7"
+version = "5.0.0"
+requires_python = ">=3.8"
 summary = "Pytest plugin for measuring coverage."
 groups = ["dev"]
 dependencies = [
     "coverage[toml]>=5.2.1",
     "pytest>=4.6",
 ]
 files = [
-    {file = "pytest-cov-4.1.0.tar.gz", hash = "sha256:3904b13dfbfec47f003b8e77fd5b589cd11904a21ddf1ab38a64f204d6a10ef6"},
-    {file = "pytest_cov-4.1.0-py3-none-any.whl", hash = "sha256:6ba70b9e97e69fcc3fb45bfeab2d0a138fb65c4d0d6a41ef33983ad114be8c3a"},
+    {file = "pytest-cov-5.0.0.tar.gz", hash = "sha256:5837b58e9f6ebd335b0f8060eecce69b662415b16dc503883a02f45dfeb14857"},
+    {file = "pytest_cov-5.0.0-py3-none-any.whl", hash = "sha256:4f0764a1219df53214206bf1feea4633c3b558a2925c8b59f144f682861ce652"},
+]
+
+[[package]]
+name = "python-dotenv"
+version = "1.0.1"
+requires_python = ">=3.8"
+summary = "Read key-value pairs from a .env file and set them as environment variables"
+groups = ["dev"]
+files = [
+    {file = "python-dotenv-1.0.1.tar.gz", hash = "sha256:e324ee90a023d808f1959c46bcbc04446a10ced277783dc6ee09987c37ec10ca"},
+    {file = "python_dotenv-1.0.1-py3-none-any.whl", hash = "sha256:f7b63ef50f1b690dddf550d03497b66d609393b40b564ed0d674909a68ebf16a"},
+]
+
+[[package]]
+name = "questionary"
+version = "2.0.1"
+requires_python = ">=3.8"
+summary = "Python library to build pretty command line user prompts ⭐️"
+groups = ["dev"]
+dependencies = [
+    "prompt-toolkit<=3.0.36,>=2.0",
+]
+files = [
+    {file = "questionary-2.0.1-py3-none-any.whl", hash = "sha256:8ab9a01d0b91b68444dff7f6652c1e754105533f083cbe27597c8110ecc230a2"},
+    {file = "questionary-2.0.1.tar.gz", hash = "sha256:bcce898bf3dbb446ff62830c86c5c6fb9a22a54146f0f5597d3da43b10d8fc8b"},
+]
+
+[[package]]
+name = "rich"
+version = "13.7.1"
+requires_python = ">=3.7.0"
+summary = "Render rich text, tables, progress bars, syntax highlighting, markdown and more to the terminal"
+groups = ["dev"]
+dependencies = [
+    "markdown-it-py>=2.2.0",
+    "pygments<3.0.0,>=2.13.0",
+]
+files = [
+    {file = "rich-13.7.1-py3-none-any.whl", hash = "sha256:4edbae314f59eb482f54e9e30bf00d33350aaa94f4bfcd4e9e3110e64d0d7222"},
+    {file = "rich-13.7.1.tar.gz", hash = "sha256:9be308cb1fe2f1f57d67ce99e95af38a1e2bc71ad9813b0e247cf7ffbcc3a432"},
+]
+
+[[package]]
+name = "rich-click"
+version = "1.8.1"
+requires_python = ">=3.7"
+summary = "Format click help output nicely with rich"
+groups = ["dev"]
+dependencies = [
+    "click>=7",
+    "rich>=10.7",
+    "typing-extensions",
+]
+files = [
+    {file = "rich_click-1.8.1-py3-none-any.whl", hash = "sha256:0cf0bf84404e78379bd2722db88cb07ffd0535440e20a05943d5b02249d90f8a"},
+    {file = "rich_click-1.8.1.tar.gz", hash = "sha256:73c2ec88a66d7bf6b8c32783539d1c9c92c7c75847f14186092d27f83b206e8a"},
 ]
 
 [[package]]
 name = "ruff"
-version = "0.3.0"
+version = "0.4.4"
 requires_python = ">=3.7"
 summary = "An extremely fast Python linter and code formatter, written in Rust."
 groups = ["dev"]
 files = [
-    {file = "ruff-0.3.0-py3-none-macosx_10_12_x86_64.macosx_11_0_arm64.macosx_10_12_universal2.whl", hash = "sha256:7deb528029bacf845bdbb3dbb2927d8ef9b4356a5e731b10eef171e3f0a85944"},
-    {file = "ruff-0.3.0-py3-none-macosx_10_12_x86_64.whl", hash = "sha256:e1e0d4381ca88fb2b73ea0766008e703f33f460295de658f5467f6f229658c19"},
-    {file = "ruff-0.3.0-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:2f7dbba46e2827dfcb0f0cc55fba8e96ba7c8700e0a866eb8cef7d1d66c25dcb"},
-    {file = "ruff-0.3.0-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:23dbb808e2f1d68eeadd5f655485e235c102ac6f12ad31505804edced2a5ae77"},
-    {file = "ruff-0.3.0-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:3ef655c51f41d5fa879f98e40c90072b567c666a7114fa2d9fe004dffba00932"},
-    {file = "ruff-0.3.0-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:d0d3d7ef3d4f06433d592e5f7d813314a34601e6c5be8481cccb7fa760aa243e"},
-    {file = "ruff-0.3.0-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:b08b356d06a792e49a12074b62222f9d4ea2a11dca9da9f68163b28c71bf1dd4"},
-    {file = "ruff-0.3.0-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:9343690f95710f8cf251bee1013bf43030072b9f8d012fbed6ad702ef70d360a"},
-    {file = "ruff-0.3.0-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a1f3ed501a42f60f4dedb7805fa8d4534e78b4e196f536bac926f805f0743d49"},
-    {file = "ruff-0.3.0-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:cc30a9053ff2f1ffb505a585797c23434d5f6c838bacfe206c0e6cf38c921a1e"},
-    {file = "ruff-0.3.0-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:5da894a29ec018a8293d3d17c797e73b374773943e8369cfc50495573d396933"},
-    {file = "ruff-0.3.0-py3-none-musllinux_1_2_i686.whl", hash = "sha256:755c22536d7f1889be25f2baf6fedd019d0c51d079e8417d4441159f3bcd30c2"},
-    {file = "ruff-0.3.0-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:dd73fe7f4c28d317855da6a7bc4aa29a1500320818dd8f27df95f70a01b8171f"},
-    {file = "ruff-0.3.0-py3-none-win32.whl", hash = "sha256:19eacceb4c9406f6c41af806418a26fdb23120dfe53583df76d1401c92b7c14b"},
-    {file = "ruff-0.3.0-py3-none-win_amd64.whl", hash = "sha256:128265876c1d703e5f5e5a4543bd8be47c73a9ba223fd3989d4aa87dd06f312f"},
-    {file = "ruff-0.3.0-py3-none-win_arm64.whl", hash = "sha256:e3a4a6d46aef0a84b74fcd201a4401ea9a6cd85614f6a9435f2d33dd8cefbf83"},
-    {file = "ruff-0.3.0.tar.gz", hash = "sha256:0886184ba2618d815067cf43e005388967b67ab9c80df52b32ec1152ab49f53a"},
+    {file = "ruff-0.4.4-py3-none-macosx_10_12_x86_64.whl", hash = "sha256:29d44ef5bb6a08e235c8249294fa8d431adc1426bfda99ed493119e6f9ea1bf6"},
+    {file = "ruff-0.4.4-py3-none-macosx_11_0_arm64.whl", hash = "sha256:c4efe62b5bbb24178c950732ddd40712b878a9b96b1d02b0ff0b08a090cbd891"},
+    {file = "ruff-0.4.4-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:4c8e2f1e8fc12d07ab521a9005d68a969e167b589cbcaee354cb61e9d9de9c15"},
+    {file = "ruff-0.4.4-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:60ed88b636a463214905c002fa3eaab19795679ed55529f91e488db3fe8976ab"},
+    {file = "ruff-0.4.4-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:b90fc5e170fc71c712cc4d9ab0e24ea505c6a9e4ebf346787a67e691dfb72e85"},
+    {file = "ruff-0.4.4-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:8e7e6ebc10ef16dcdc77fd5557ee60647512b400e4a60bdc4849468f076f6eef"},
+    {file = "ruff-0.4.4-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:b9ddb2c494fb79fc208cd15ffe08f32b7682519e067413dbaf5f4b01a6087bcd"},
+    {file = "ruff-0.4.4-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:c51c928a14f9f0a871082603e25a1588059b7e08a920f2f9fa7157b5bf08cfe9"},
+    {file = "ruff-0.4.4-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b5eb0a4bfd6400b7d07c09a7725e1a98c3b838be557fee229ac0f84d9aa49c36"},
+    {file = "ruff-0.4.4-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:b1867ee9bf3acc21778dcb293db504692eda5f7a11a6e6cc40890182a9f9e595"},
+    {file = "ruff-0.4.4-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:1aecced1269481ef2894cc495647392a34b0bf3e28ff53ed95a385b13aa45768"},
+    {file = "ruff-0.4.4-py3-none-musllinux_1_2_i686.whl", hash = "sha256:9da73eb616b3241a307b837f32756dc20a0b07e2bcb694fec73699c93d04a69e"},
+    {file = "ruff-0.4.4-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:958b4ea5589706a81065e2a776237de2ecc3e763342e5cc8e02a4a4d8a5e6f95"},
+    {file = "ruff-0.4.4-py3-none-win32.whl", hash = "sha256:cb53473849f011bca6e754f2cdf47cafc9c4f4ff4570003a0dad0b9b6890e876"},
+    {file = "ruff-0.4.4-py3-none-win_amd64.whl", hash = "sha256:424e5b72597482543b684c11def82669cc6b395aa8cc69acc1858b5ef3e5daae"},
+    {file = "ruff-0.4.4-py3-none-win_arm64.whl", hash = "sha256:39df0537b47d3b597293edbb95baf54ff5b49589eb7ff41926d8243caa995ea6"},
+    {file = "ruff-0.4.4.tar.gz", hash = "sha256:f87ea42d5cdebdc6a69761a9d0bc83ae9b3b30d0ad78952005ba6568d6c022af"},
 ]
 
 [[package]]
 name = "tomli"
 version = "2.0.1"
 requires_python = ">=3.7"
 summary = "A lil' TOML parser"
@@ -367,14 +523,25 @@
 marker = "python_version < \"3.11\""
 files = [
     {file = "tomli-2.0.1-py3-none-any.whl", hash = "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc"},
     {file = "tomli-2.0.1.tar.gz", hash = "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"},
 ]
 
 [[package]]
+name = "tomlkit"
+version = "0.12.5"
+requires_python = ">=3.7"
+summary = "Style preserving TOML library"
+groups = ["dev"]
+files = [
+    {file = "tomlkit-0.12.5-py3-none-any.whl", hash = "sha256:af914f5a9c59ed9d0762c7b64d3b5d5df007448eb9cd2edc8a46b1eafead172f"},
+    {file = "tomlkit-0.12.5.tar.gz", hash = "sha256:eef34fba39834d4d6b73c9ba7f3e4d1c417a4e56f89a7e96e090dd0d24b8fb3c"},
+]
+
+[[package]]
 name = "typing-extensions"
 version = "4.9.0"
 requires_python = ">=3.8"
 summary = "Backported and Experimental Type Hints for Python 3.8+"
 groups = ["default", "dev"]
 files = [
     {file = "typing_extensions-4.9.0-py3-none-any.whl", hash = "sha256:af72aea155e91adfc61c3ae9e0e342dbc0cba726d6cba4b6c72c1f34e47291cd"},
@@ -386,7 +553,31 @@
 version = "1.1.0"
 summary = "Universally Unique Lexicographically Sortable Identifier"
 groups = ["default"]
 files = [
     {file = "ulid-py-1.1.0.tar.gz", hash = "sha256:dc6884be91558df077c3011b9fb0c87d1097cb8fc6534b11f310161afd5738f0"},
     {file = "ulid_py-1.1.0-py2.py3-none-any.whl", hash = "sha256:b56a0f809ef90d6020b21b89a87a48edc7c03aea80e5ed5174172e82d76e3987"},
 ]
+
+[[package]]
+name = "wcmatch"
+version = "8.5.1"
+requires_python = ">=3.8"
+summary = "Wildcard/glob file name matcher."
+groups = ["dev"]
+dependencies = [
+    "bracex>=2.1.1",
+]
+files = [
+    {file = "wcmatch-8.5.1-py3-none-any.whl", hash = "sha256:24c19cedc92bc9c9e27f39db4e1824d72f95bd2cea32b254a47a45b1a1b227ed"},
+    {file = "wcmatch-8.5.1.tar.gz", hash = "sha256:c0088c7f6426cf6bf27e530e2b7b734031905f7e490475fd83c7c5008ab581b3"},
+]
+
+[[package]]
+name = "wcwidth"
+version = "0.2.13"
+summary = "Measures the displayed width of unicode strings in a terminal"
+groups = ["dev"]
+files = [
+    {file = "wcwidth-0.2.13-py2.py3-none-any.whl", hash = "sha256:3da69048e4540d84af32131829ff948f1e022c1c6bdb8d6102117aac784f6859"},
+    {file = "wcwidth-0.2.13.tar.gz", hash = "sha256:72ea0c06399eb286d978fdedb6923a9eb47e1c486ce63e9b4e64fc18303972b5"},
+]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `karp_lex_types-0.6.2/ruff.toml` & `karp_lex_types-0.6.4/ruff.toml`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.6.2/src/karp_lex_types/commands/__init__.py` & `karp_lex_types-0.6.4/src/karp_lex_types/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.6.2/src/karp_lex_types/commands/base.py` & `karp_lex_types-0.6.4/src/karp_lex_types/commands/base.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.6.2/src/karp_lex_types/commands/entry_commands.py` & `karp_lex_types-0.6.4/src/karp_lex_types/commands/entry_commands.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.6.2/src/karp_lex_types/commands/entry_repo_commands.py` & `karp_lex_types-0.6.4/src/karp_lex_types/commands/entry_repo_commands.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.6.2/src/karp_lex_types/commands/resource_commands.py` & `karp_lex_types-0.6.4/src/karp_lex_types/commands/resource_commands.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.6.2/src/karp_lex_types/dtos/entry_dto.py` & `karp_lex_types-0.6.4/src/karp_lex_types/dtos/entry_dto.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.6.2/src/karp_lex_types/value_objects/unique_id.py` & `karp_lex_types-0.6.4/src/karp_lex_types/value_objects/unique_id.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.6.2/tests/entry_dto_unit_test.py` & `karp_lex_types-0.6.4/tests/entry_dto_unit_test.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.6.2/tests/requirements-testing.lock` & `karp_lex_types-0.6.4/tests/requirements-testing.lock`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 # This file is @generated by PDM.
 # Please do not edit it manually.
 
 annotated-types==0.6.0 \
     --hash=sha256:0641064de18ba7a25dee8f96403ebc39113d0cb953a01429249d5c7564666a43 \
     --hash=sha256:563339e807e53ffd9c267e99fc6d9ea23eb8443c08f112651963e24e22f84a5d
-bump2version==1.0.1 \
-    --hash=sha256:37f927ea17cde7ae2d7baf832f8e80ce3777624554a653006c9144f8017fe410 \
-    --hash=sha256:762cb2bfad61f4ec8e2bdf452c7c267416f8c70dd9ecb1653fd0bbb01fa936e6
-colorama==0.4.6; sys_platform == "win32" \
+bracex==2.4 \
+    --hash=sha256:a27eaf1df42cf561fed58b7a8f3fdf129d1ea16a81e1fadd1d17989bc6384beb \
+    --hash=sha256:efdc71eff95eaff5e0f8cfebe7d01adf2c8637c8c92edaf63ef348c241a82418
+bump-my-version==0.21.0 \
+    --hash=sha256:a614d8176b5ac0e644239c9a8a246b696d316f68406fd78b8486a9e13fc93266 \
+    --hash=sha256:c3f1a31e32345679b517cbba99a0875457ee45d7ba6189fcd2a74d3ddae41515
+click==8.1.7 \
+    --hash=sha256:ae74fb96c20a0277a1d615f1e4d73c8414f5a98db8b799a7931d1582f3390c28 \
+    --hash=sha256:ca9853ad459e787e2192211578cc907e7594e294c7ccc834310722b41b9ca6de
+colorama==0.4.6; sys_platform == "win32" or platform_system == "Windows" \
     --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
 coverage==7.4.1 \
     --hash=sha256:0193657651f5399d433c92f8ae264aff31fc1d066deee4b831549526433f3f61 \
     --hash=sha256:02f2edb575d62172aa28fe00efe821ae31f25dc3d589055b3fb64d51e52e4ab1 \
     --hash=sha256:077d366e724f24fc02dbfe9d946534357fda71af9764ff99d73c3c596001bbd7 \
     --hash=sha256:18e961aa13b6d47f758cc5879383d27b5b3f3dcd9ce8cdbfdc2571fe86feb4dd \
@@ -45,126 +51,162 @@
     --hash=sha256:fe558371c1bdf3b8fa03e097c523fb9645b8730399c14fe7721ee9c9e2a545d3
 exceptiongroup==1.2.0; python_version < "3.11" \
     --hash=sha256:4bfd3996ac73b41e9b9628b04e079f193850720ea5945fc96a08633c66912f14 \
     --hash=sha256:91f5c769735f051a4290d52edd0858999b57e5876e9f85937691bd4c9fa3ed68
 iniconfig==2.0.0 \
     --hash=sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3 \
     --hash=sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374
-mypy==1.8.0 \
-    --hash=sha256:2afecd6354bbfb6e0160f4e4ad9ba6e4e003b767dd80d85516e71f2e955ab50d \
-    --hash=sha256:42c6680d256ab35637ef88891c6bd02514ccb7e1122133ac96055ff458f93fc3 \
-    --hash=sha256:485a8942f671120f76afffff70f259e1cd0f0cfe08f81c05d8816d958d4577d3 \
-    --hash=sha256:4c886c6cce2d070bd7df4ec4a05a13ee20c0aa60cb587e8d1265b6c03cf91da3 \
-    --hash=sha256:51720c776d148bad2372ca21ca29256ed483aa9a4cdefefcef49006dff2a6835 \
-    --hash=sha256:52825b01f5c4c1c4eb0db253ec09c7aa17e1a7304d247c48b6f3599ef40db8bd \
-    --hash=sha256:538fd81bb5e430cc1381a443971c0475582ff9f434c16cd46d2c66763ce85d9d \
-    --hash=sha256:6ff8b244d7085a0b425b56d327b480c3b29cafbd2eff27316a004f9a7391ae07 \
-    --hash=sha256:720a5ca70e136b675af3af63db533c1c8c9181314d207568bbe79051f122669e \
-    --hash=sha256:855fe27b80375e5c5878492f0729540db47b186509c98dae341254c8f45f42ae \
-    --hash=sha256:8963b83d53ee733a6e4196954502b33567ad07dfd74851f32be18eb932fb1cb9 \
-    --hash=sha256:9261ed810972061388918c83c3f5cd46079d875026ba97380f3e3978a72f503d \
-    --hash=sha256:afe3fe972c645b4632c563d3f3eff1cdca2fa058f730df2b93a35e3b0c538218 \
-    --hash=sha256:d19c413b3c07cbecf1f991e2221746b0d2a9410b59cb3f4fb9557f0365a1a817 \
-    --hash=sha256:df9824ac11deaf007443e7ed2a4a26bebff98d2bc43c6da21b2b64185da011c4 \
-    --hash=sha256:e46f44b54ebddbeedbd3d5b289a893219065ef805d95094d16a0af6630f5d410 \
-    --hash=sha256:f5ac9a4eeb1ec0f1ccdc6f326bcdb464de5f80eb07fb38b5ddd7b0de6bc61e55
+markdown-it-py==3.0.0 \
+    --hash=sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1 \
+    --hash=sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb
+mdurl==0.1.2 \
+    --hash=sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8 \
+    --hash=sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba
+mypy==1.10.0 \
+    --hash=sha256:12b6bfc1b1a66095ab413160a6e520e1dc076a28f3e22f7fb25ba3b000b4ef99 \
+    --hash=sha256:1ec404a7cbe9fc0e92cb0e67f55ce0c025014e26d33e54d9e506a0f2d07fe5de \
+    --hash=sha256:2b0695d605ddcd3eb2f736cd8b4e388288c21e7de85001e9f85df9187f2b50f9 \
+    --hash=sha256:3be66771aa5c97602f382230165b856c231d1277c511c9a8dd058be4784472e1 \
+    --hash=sha256:3d087fcbec056c4ee34974da493a826ce316947485cef3901f511848e687c131 \
+    --hash=sha256:4cf18f9d0efa1b16478c4c129eabec36148032575391095f73cae2e722fcf9d5 \
+    --hash=sha256:8b2cbaca148d0754a54d44121b5825ae71868c7592a53b7292eeb0f3fdae95ee \
+    --hash=sha256:8f55583b12156c399dce2df7d16f8a5095291354f1e839c252ec6c0611e86e2e \
+    --hash=sha256:9e36fb078cce9904c7989b9693e41cb9711e0600139ce3970c6ef814b6ebc2b2 \
+    --hash=sha256:a781f6ad4bab20eef8b65174a57e5203f4be627b46291f4589879bf4e257b97b \
+    --hash=sha256:a87dbfa85971e8d59c9cc1fcf534efe664d8949e4c0b6b44e8ca548e746a8d53 \
+    --hash=sha256:b808e12113505b97d9023b0b5e0c0705a90571c6feefc6f215c1df9381256e30 \
+    --hash=sha256:bc6ac273b23c6b82da3bb25f4136c4fd42665f17f2cd850771cb600bdd2ebeda \
+    --hash=sha256:cd777b780312ddb135bceb9bc8722a73ec95e042f911cc279e2ec3c667076051 \
+    --hash=sha256:da1cbf08fb3b851ab3b9523a884c232774008267b1f83371ace57f412fe308c2 \
+    --hash=sha256:e22e1527dc3d4aa94311d246b59e47f6455b8729f4968765ac1eacf9a4760bc7 \
+    --hash=sha256:f8c083976eb530019175aabadb60921e73b4f45736760826aa1689dda8208aee
 mypy-extensions==1.0.0 \
     --hash=sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d \
     --hash=sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782
 packaging==23.2 \
     --hash=sha256:048fb0e9405036518eaaf48a55953c750c11e1a1b68e0dd1a9d62ed0c092cfc5 \
     --hash=sha256:8c491190033a9af7e1d931d0b5dacc2ef47509b34dd0de67ed209b5203fc88c7
-pluggy==1.4.0 \
-    --hash=sha256:7db9f7b503d67d1c5b95f59773ebb58a8c1c288129a88665838012cfb07b8981 \
-    --hash=sha256:8c85c2876142a764e5b7548e7d9a0e0ddb46f5185161049a79b7e974454223be
-pydantic==2.6.1 \
-    --hash=sha256:0b6a909df3192245cb736509a92ff69e4fef76116feffec68e93a567347bae6f \
-    --hash=sha256:4fd5c182a2488dc63e6d32737ff19937888001e2a6d86e94b3f233104a5d1fa9
-pydantic-core==2.16.2 \
-    --hash=sha256:02906e7306cb8c5901a1feb61f9ab5e5c690dbbeaa04d84c1b9ae2a01ebe9379 \
-    --hash=sha256:0ba503850d8b8dcc18391f10de896ae51d37fe5fe43dbfb6a35c5c5cad271a06 \
-    --hash=sha256:16aa02e7a0f539098e215fc193c8926c897175d64c7926d00a36188917717a05 \
-    --hash=sha256:22c5f022799f3cd6741e24f0443ead92ef42be93ffda0d29b2597208c94c3753 \
-    --hash=sha256:2924b89b16420712e9bb8192396026a8fbd6d8726224f918353ac19c4c043d2a \
-    --hash=sha256:308974fdf98046db28440eb3377abba274808bf66262e042c412eb2adf852731 \
-    --hash=sha256:396fdf88b1b503c9c59c84a08b6833ec0c3b5ad1a83230252a9e17b7dfb4cffc \
-    --hash=sha256:3ac426704840877a285d03a445e162eb258924f014e2f074e209d9b4ff7bf380 \
-    --hash=sha256:3fab4e75b8c525a4776e7630b9ee48aea50107fea6ca9f593c98da3f4d11bf7c \
-    --hash=sha256:406fac1d09edc613020ce9cf3f2ccf1a1b2f57ab00552b4c18e3d5276c67eb11 \
-    --hash=sha256:40a0bd0bed96dae5712dab2aba7d334a6c67cbcac2ddfca7dbcc4a8176445990 \
-    --hash=sha256:459c0d338cc55d099798618f714b21b7ece17eb1a87879f2da20a3ff4c7628e2 \
-    --hash=sha256:459d6be6134ce3b38e0ef76f8a672924460c455d45f1ad8fdade36796df1ddc8 \
-    --hash=sha256:46b0d5520dbcafea9a8645a8164658777686c5c524d381d983317d29687cce97 \
-    --hash=sha256:47924039e785a04d4a4fa49455e51b4eb3422d6eaacfde9fc9abf8fdef164e8a \
-    --hash=sha256:4bfcbde6e06c56b30668a0c872d75a7ef3025dc3c1823a13cf29a0e9b33f67e8 \
-    --hash=sha256:4f9ee4febb249c591d07b2d4dd36ebcad0ccd128962aaa1801508320896575ef \
-    --hash=sha256:5f60f920691a620b03082692c378661947d09415743e437a7478c309eb0e4f82 \
-    --hash=sha256:60eb8ceaa40a41540b9acae6ae7c1f0a67d233c40dc4359c256ad2ad85bdf5e5 \
-    --hash=sha256:6db58c22ac6c81aeac33912fb1af0e930bc9774166cdd56eade913d5f2fff35e \
-    --hash=sha256:70651ff6e663428cea902dac297066d5c6e5423fda345a4ca62430575364d62b \
-    --hash=sha256:72f7919af5de5ecfaf1eba47bf9a5d8aa089a3340277276e5636d16ee97614d7 \
-    --hash=sha256:7b883af50eaa6bb3299780651e5be921e88050ccf00e3e583b1e92020333304b \
-    --hash=sha256:7beec26729d496a12fd23cf8da9944ee338c8b8a17035a560b585c36fe81af20 \
-    --hash=sha256:7bf26c2e2ea59d32807081ad51968133af3025c4ba5753e6a794683d2c91bf6e \
-    --hash=sha256:7c31669e0c8cc68400ef0c730c3a1e11317ba76b892deeefaf52dcb41d56ed5d \
-    --hash=sha256:870dbfa94de9b8866b37b867a2cb37a60c401d9deb4a9ea392abf11a1f98037b \
-    --hash=sha256:88646cae28eb1dd5cd1e09605680c2b043b64d7481cdad7f5003ebef401a3039 \
-    --hash=sha256:8aafeedb6597a163a9c9727d8a8bd363a93277701b7bfd2749fbefee2396469e \
-    --hash=sha256:8bde5b48c65b8e807409e6f20baee5d2cd880e0fad00b1a811ebc43e39a00ab2 \
-    --hash=sha256:8f9142a6ed83d90c94a3efd7af8873bf7cefed2d3d44387bf848888482e2d25f \
-    --hash=sha256:936a787f83db1f2115ee829dd615c4f684ee48ac4de5779ab4300994d8af325b \
-    --hash=sha256:98dc6f4f2095fc7ad277782a7c2c88296badcad92316b5a6e530930b1d475ebc \
-    --hash=sha256:9957433c3a1b67bdd4c63717eaf174ebb749510d5ea612cd4e83f2d9142f3fc8 \
-    --hash=sha256:99af961d72ac731aae2a1b55ccbdae0733d816f8bfb97b41909e143de735f522 \
-    --hash=sha256:9b5f13857da99325dcabe1cc4e9e6a3d7b2e2c726248ba5dd4be3e8e4a0b6d0e \
-    --hash=sha256:9d776d30cde7e541b8180103c3f294ef7c1862fd45d81738d156d00551005784 \
-    --hash=sha256:a3b7352b48fbc8b446b75f3069124e87f599d25afb8baa96a550256c031bb890 \
-    --hash=sha256:a477932664d9611d7a0816cc3c0eb1f8856f8a42435488280dfbf4395e141485 \
-    --hash=sha256:a7e41e3ada4cca5f22b478c08e973c930e5e6c7ba3588fb8e35f2398cdcc1545 \
-    --hash=sha256:a90fec23b4b05a09ad988e7a4f4e081711a90eb2a55b9c984d8b74597599180f \
-    --hash=sha256:a9e523474998fb33f7c1a4d55f5504c908d57add624599e095c20fa575b8d943 \
-    --hash=sha256:b0d7a9165167269758145756db43a133608a531b1e5bb6a626b9ee24bc38a8f7 \
-    --hash=sha256:b94cbda27267423411c928208e89adddf2ea5dd5f74b9528513f0358bba019cb \
-    --hash=sha256:ce232a6170dd6532096cadbf6185271e4e8c70fc9217ebe105923ac105da9978 \
-    --hash=sha256:cf903310a34e14651c9de056fcc12ce090560864d5a2bb0174b971685684e1d8 \
-    --hash=sha256:d5362d099c244a2d2f9659fb3c9db7c735f0004765bbe06b99be69fbd87c3f15 \
-    --hash=sha256:dffaf740fe2e147fedcb6b561353a16243e654f7fe8e701b1b9db148242e1272 \
-    --hash=sha256:e6294e76b0380bb7a61eb8a39273c40b20beb35e8c87ee101062834ced19c545 \
-    --hash=sha256:eca58e319f4fd6df004762419612122b2c7e7d95ffafc37e890252f869f3fb2a \
-    --hash=sha256:ed957db4c33bc99895f3a1672eca7e80e8cda8bd1e29a80536b4ec2153fa9804 \
-    --hash=sha256:ef6113cd31411eaf9b39fc5a8848e71c72656fd418882488598758b2c8c6dfa0 \
-    --hash=sha256:f8ed79883b4328b7f0bd142733d99c8e6b22703e908ec63d930b06be3a0e7113 \
-    --hash=sha256:fe56851c3f1d6f5384b3051c536cc81b3a93a73faf931f404fef95217cf1e10d \
-    --hash=sha256:ff7c97eb7a29aba230389a2661edf2e9e06ce616c7e35aa764879b6894a44b25
-pytest==7.4.4 \
-    --hash=sha256:2cf0005922c6ace4a3e2ec8b4080eb0d9753fdc93107415332f50ce9e7994280 \
-    --hash=sha256:b090cdf5ed60bf4c45261be03239c2c1c22df034fbffe691abe93cd80cea01d8
-pytest-cov==4.1.0 \
-    --hash=sha256:3904b13dfbfec47f003b8e77fd5b589cd11904a21ddf1ab38a64f204d6a10ef6 \
-    --hash=sha256:6ba70b9e97e69fcc3fb45bfeab2d0a138fb65c4d0d6a41ef33983ad114be8c3a
-ruff==0.2.1 \
-    --hash=sha256:0034d5b6323e6e8fe91b2a1e55b02d92d0b582d2953a2b37a67a2d7dedbb7acc \
-    --hash=sha256:00a818e2db63659570403e44383ab03c529c2b9678ba4ba6c105af7854008105 \
-    --hash=sha256:0a725823cb2a3f08ee743a534cb6935727d9e47409e4ad72c10a3faf042ad5ba \
-    --hash=sha256:13471684694d41ae0f1e8e3a7497e14cd57ccb7dd72ae08d56a159d6c9c3e30e \
-    --hash=sha256:3b42b5d8677cd0c72b99fcaf068ffc62abb5a19e71b4a3b9cfa50658a0af02f1 \
-    --hash=sha256:6b95ac9ce49b4fb390634d46d6ece32ace3acdd52814671ccaf20b7f60adb232 \
-    --hash=sha256:7022d66366d6fded4ba3889f73cd791c2d5621b2ccf34befc752cb0df70f5fad \
-    --hash=sha256:a11567e20ea39d1f51aebd778685582d4c56ccb082c1161ffc10f79bebe6df35 \
-    --hash=sha256:be60592f9d218b52f03384d1325efa9d3b41e4c4d55ea022cd548547cc42cd2b \
-    --hash=sha256:c92db7101ef5bfc18e96777ed7bc7c822d545fa5977e90a585accac43d22f18a \
-    --hash=sha256:dc586724a95b7d980aa17f671e173df00f0a2eef23f8babbeee663229a938fec \
-    --hash=sha256:dd81b911d28925e7e8b323e8d06951554655021df8dd4ac3045d7212ac4ba080 \
-    --hash=sha256:e3affdcbc2afb6f5bd0eb3130139ceedc5e3f28d206fe49f63073cb9e65988e0 \
-    --hash=sha256:e5cb5526d69bb9143c2e4d2a115d08ffca3d8e0fddc84925a7b54931c96f5c02 \
-    --hash=sha256:efababa8e12330aa94a53e90a81eb6e2d55f348bc2e71adbf17d9cad23c03ee6 \
-    --hash=sha256:f3ef052283da7dec1987bba8d8733051c2325654641dfe5877a4022108098683 \
-    --hash=sha256:fbd2288890b88e8aab4499e55148805b58ec711053588cc2f0196a44f6e3d855
+pluggy==1.5.0 \
+    --hash=sha256:2cffa88e94fdc978c4c574f15f9e59b7f4201d439195c3715ca9e2486f1d0cf1 \
+    --hash=sha256:44e1ad92c8ca002de6377e165f3e0f1be63266ab4d554740532335b9d75ea669
+prompt-toolkit==3.0.36 \
+    --hash=sha256:3e163f254bef5a03b146397d7c1963bd3e2812f0964bb9a24e6ec761fd28db63 \
+    --hash=sha256:aa64ad242a462c5ff0363a7b9cfe696c20d55d9fc60c11fd8e632d064804d305
+pydantic==2.6.3 \
+    --hash=sha256:72c6034df47f46ccdf81869fddb81aade68056003900a8724a4f160700016a2a \
+    --hash=sha256:e07805c4c7f5c6826e33a1d4c9d47950d7eaf34868e2690f8594d2e30241f11f
+pydantic-core==2.16.3 \
+    --hash=sha256:00ee1c97b5364b84cb0bd82e9bbf645d5e2871fb8c58059d158412fee2d33d8a \
+    --hash=sha256:0d32576b1de5a30d9a97f300cc6a3f4694c428d956adbc7e6e2f9cad279e45ed \
+    --hash=sha256:0df446663464884297c793874573549229f9eca73b59360878f382a0fc085979 \
+    --hash=sha256:0f56ae86b60ea987ae8bcd6654a887238fd53d1384f9b222ac457070b7ac4cff \
+    --hash=sha256:162e498303d2b1c036b957a1278fa0899d02b2842f1ff901b6395104c5554a45 \
+    --hash=sha256:1b662180108c55dfbf1280d865b2d116633d436cfc0bba82323554873967b340 \
+    --hash=sha256:1cac689f80a3abab2d3c0048b29eea5751114054f032a941a32de4c852c59cad \
+    --hash=sha256:287073c66748f624be4cef893ef9174e3eb88fe0b8a78dc22e88eca4bc357ca6 \
+    --hash=sha256:2a72fb9963cba4cd5793854fd12f4cfee731e86df140f59ff52a49b3552db241 \
+    --hash=sha256:2acca2be4bb2f2147ada8cac612f8a98fc09f41c89f87add7256ad27332c2fda \
+    --hash=sha256:2f583bd01bbfbff4eaee0868e6fc607efdfcc2b03c1c766b06a707abbc856187 \
+    --hash=sha256:33809aebac276089b78db106ee692bdc9044710e26f24a9a2eaa35a0f9fa70ba \
+    --hash=sha256:36fa178aacbc277bc6b62a2c3da95226520da4f4e9e206fdf076484363895d2c \
+    --hash=sha256:4204e773b4b408062960e65468d5346bdfe139247ee5f1ca2a378983e11388a2 \
+    --hash=sha256:456855f57b413f077dff513a5a28ed838dbbb15082ba00f80750377eed23d132 \
+    --hash=sha256:49d5d58abd4b83fb8ce763be7794d09b2f50f10aa65c0f0c1696c677edeb7cbf \
+    --hash=sha256:4df8a199d9f6afc5ae9a65f8f95ee52cae389a8c6b20163762bde0426275b7db \
+    --hash=sha256:500960cb3a0543a724a81ba859da816e8cf01b0e6aaeedf2c3775d12ee49cade \
+    --hash=sha256:519ae0312616026bf4cedc0fe459e982734f3ca82ee8c7246c19b650b60a5ee4 \
+    --hash=sha256:5c5cbc703168d1b7a838668998308018a2718c2130595e8e190220238addc96f \
+    --hash=sha256:6162f8d2dc27ba21027f261e4fa26f8bcb3cf9784b7f9499466a311ac284b5b9 \
+    --hash=sha256:716b542728d4c742353448765aa7cdaa519a7b82f9564130e2b3f6766018c9ec \
+    --hash=sha256:732da3243e1b8d3eab8c6ae23ae6a58548849d2e4a4e03a1924c8ddf71a387cb \
+    --hash=sha256:75b81e678d1c1ede0785c7f46690621e4c6e63ccd9192af1f0bd9d504bbb6bf4 \
+    --hash=sha256:75f76ee558751746d6a38f89d60b6228fa174e5172d143886af0f85aa306fd89 \
+    --hash=sha256:86b3d0033580bd6bbe07590152007275bd7af95f98eaa5bd36f3da219dcd93da \
+    --hash=sha256:8d62da299c6ecb04df729e4b5c52dc0d53f4f8430b4492b93aa8de1f541c4aac \
+    --hash=sha256:8e47755d8152c1ab5b55928ab422a76e2e7b22b5ed8e90a7d584268dd49e9c6b \
+    --hash=sha256:936e5db01dd49476fa8f4383c259b8b1303d5dd5fb34c97de194560698cc2c5e \
+    --hash=sha256:99b6add4c0b39a513d323d3b93bc173dac663c27b99860dd5bf491b240d26137 \
+    --hash=sha256:9c865a7ee6f93783bd5d781af5a4c43dadc37053a5b42f7d18dc019f8c9d2bd1 \
+    --hash=sha256:a425479ee40ff021f8216c9d07a6a3b54b31c8267c6e17aa88b70d7ebd0e5e5b \
+    --hash=sha256:a6b1bb0827f56654b4437955555dc3aeeebeddc47c2d7ed575477f082622c49e \
+    --hash=sha256:aaf09e615a0bf98d406657e0008e4a8701b11481840be7d31755dc9f97c44053 \
+    --hash=sha256:b29eeb887aa931c2fcef5aa515d9d176d25006794610c264ddc114c053bf96fe \
+    --hash=sha256:b3992a322a5617ded0a9f23fd06dbc1e4bd7cf39bc4ccf344b10f80af58beacd \
+    --hash=sha256:b60cc1a081f80a2105a59385b92d82278b15d80ebb3adb200542ae165cd7d183 \
+    --hash=sha256:b926dd38db1519ed3043a4de50214e0d600d404099c3392f098a7f9d75029ff8 \
+    --hash=sha256:bd87f48924f360e5d1c5f770d6155ce0e7d83f7b4e10c2f9ec001c73cf475c99 \
+    --hash=sha256:c9bd22a2a639e26171068f8ebb5400ce2c1bc7d17959f60a3b753ae13c632975 \
+    --hash=sha256:cbcc558401de90a746d02ef330c528f2e668c83350f045833543cd57ecead1ad \
+    --hash=sha256:cf6204fe865da605285c34cf1172879d0314ff267b1c35ff59de7154f35fdc2e \
+    --hash=sha256:d33dd21f572545649f90c38c227cc8631268ba25c460b5569abebdd0ec5974ca \
+    --hash=sha256:d89ca19cdd0dd5f31606a9329e309d4fcbb3df860960acec32630297d61820df \
+    --hash=sha256:dcca5d2bf65c6fb591fff92da03f94cd4f315972f97c21975398bd4bd046854a \
+    --hash=sha256:ded1c35f15c9dea16ead9bffcde9bb5c7c031bff076355dc58dcb1cb436c4721 \
+    --hash=sha256:e56f8186d6210ac7ece503193ec84104da7ceb98f68ce18c07282fcc2452e76f \
+    --hash=sha256:e7c6ed0dc9d8e65f24f5824291550139fe6f37fac03788d4580da0d33bc00c97 \
+    --hash=sha256:ec08be75bb268473677edb83ba71e7e74b43c008e4a7b1907c6d57e940bf34b6 \
+    --hash=sha256:ed25e1835c00a332cb10c683cd39da96a719ab1dfc08427d476bce41b92531fc \
+    --hash=sha256:f4cb85f693044e0f71f394ff76c98ddc1bc0953e48c061725e540396d5c8a2e1 \
+    --hash=sha256:f53aace168a2a10582e570b7736cc5bef12cae9cf21775e3eafac597e8551fbe \
+    --hash=sha256:f651dd19363c632f4abe3480a7c87a9773be27cfe1341aef06e8759599454120 \
+    --hash=sha256:fc4ad7f7ee1a13d9cb49d8198cd7d7e3aa93e425f371a68235f784e99741561f \
+    --hash=sha256:fee427241c2d9fb7192b658190f9f5fd6dfe41e02f3c1489d2ec1e6a5ab1e04a
+pydantic-settings==2.2.1 \
+    --hash=sha256:00b9f6a5e95553590434c0fa01ead0b216c3e10bc54ae02e37f359948643c5ed \
+    --hash=sha256:0235391d26db4d2190cb9b31051c4b46882d28a51533f97440867f012d4da091
+pygments==2.18.0 \
+    --hash=sha256:786ff802f32e91311bff3889f6e9a86e81505fe99f2735bb6d60ae0c5004f199 \
+    --hash=sha256:b8e6aca0523f3ab76fee51799c488e38782ac06eafcf95e7ba832985c8e7b13a
+pytest==8.2.0 \
+    --hash=sha256:1733f0620f6cda4095bbf0d9ff8022486e91892245bb9e7d5542c018f612f233 \
+    --hash=sha256:d507d4482197eac0ba2bae2e9babf0672eb333017bcedaa5fb1a3d42c1174b3f
+pytest-cov==5.0.0 \
+    --hash=sha256:4f0764a1219df53214206bf1feea4633c3b558a2925c8b59f144f682861ce652 \
+    --hash=sha256:5837b58e9f6ebd335b0f8060eecce69b662415b16dc503883a02f45dfeb14857
+python-dotenv==1.0.1 \
+    --hash=sha256:e324ee90a023d808f1959c46bcbc04446a10ced277783dc6ee09987c37ec10ca \
+    --hash=sha256:f7b63ef50f1b690dddf550d03497b66d609393b40b564ed0d674909a68ebf16a
+questionary==2.0.1 \
+    --hash=sha256:8ab9a01d0b91b68444dff7f6652c1e754105533f083cbe27597c8110ecc230a2 \
+    --hash=sha256:bcce898bf3dbb446ff62830c86c5c6fb9a22a54146f0f5597d3da43b10d8fc8b
+rich==13.7.1 \
+    --hash=sha256:4edbae314f59eb482f54e9e30bf00d33350aaa94f4bfcd4e9e3110e64d0d7222 \
+    --hash=sha256:9be308cb1fe2f1f57d67ce99e95af38a1e2bc71ad9813b0e247cf7ffbcc3a432
+rich-click==1.8.1 \
+    --hash=sha256:0cf0bf84404e78379bd2722db88cb07ffd0535440e20a05943d5b02249d90f8a \
+    --hash=sha256:73c2ec88a66d7bf6b8c32783539d1c9c92c7c75847f14186092d27f83b206e8a
+ruff==0.4.4 \
+    --hash=sha256:1aecced1269481ef2894cc495647392a34b0bf3e28ff53ed95a385b13aa45768 \
+    --hash=sha256:29d44ef5bb6a08e235c8249294fa8d431adc1426bfda99ed493119e6f9ea1bf6 \
+    --hash=sha256:39df0537b47d3b597293edbb95baf54ff5b49589eb7ff41926d8243caa995ea6 \
+    --hash=sha256:424e5b72597482543b684c11def82669cc6b395aa8cc69acc1858b5ef3e5daae \
+    --hash=sha256:4c8e2f1e8fc12d07ab521a9005d68a969e167b589cbcaee354cb61e9d9de9c15 \
+    --hash=sha256:60ed88b636a463214905c002fa3eaab19795679ed55529f91e488db3fe8976ab \
+    --hash=sha256:8e7e6ebc10ef16dcdc77fd5557ee60647512b400e4a60bdc4849468f076f6eef \
+    --hash=sha256:958b4ea5589706a81065e2a776237de2ecc3e763342e5cc8e02a4a4d8a5e6f95 \
+    --hash=sha256:9da73eb616b3241a307b837f32756dc20a0b07e2bcb694fec73699c93d04a69e \
+    --hash=sha256:b1867ee9bf3acc21778dcb293db504692eda5f7a11a6e6cc40890182a9f9e595 \
+    --hash=sha256:b5eb0a4bfd6400b7d07c09a7725e1a98c3b838be557fee229ac0f84d9aa49c36 \
+    --hash=sha256:b90fc5e170fc71c712cc4d9ab0e24ea505c6a9e4ebf346787a67e691dfb72e85 \
+    --hash=sha256:b9ddb2c494fb79fc208cd15ffe08f32b7682519e067413dbaf5f4b01a6087bcd \
+    --hash=sha256:c4efe62b5bbb24178c950732ddd40712b878a9b96b1d02b0ff0b08a090cbd891 \
+    --hash=sha256:c51c928a14f9f0a871082603e25a1588059b7e08a920f2f9fa7157b5bf08cfe9 \
+    --hash=sha256:cb53473849f011bca6e754f2cdf47cafc9c4f4ff4570003a0dad0b9b6890e876 \
+    --hash=sha256:f87ea42d5cdebdc6a69761a9d0bc83ae9b3b30d0ad78952005ba6568d6c022af
 tomli==2.0.1; python_version < "3.11" \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
+tomlkit==0.12.5 \
+    --hash=sha256:af914f5a9c59ed9d0762c7b64d3b5d5df007448eb9cd2edc8a46b1eafead172f \
+    --hash=sha256:eef34fba39834d4d6b73c9ba7f3e4d1c417a4e56f89a7e96e090dd0d24b8fb3c
 typing-extensions==4.9.0 \
     --hash=sha256:23478f88c37f27d76ac8aee6c905017a143b0b1b886c3c9f66bc2fd94f9f5783 \
     --hash=sha256:af72aea155e91adfc61c3ae9e0e342dbc0cba726d6cba4b6c72c1f34e47291cd
 ulid-py==1.1.0 \
     --hash=sha256:b56a0f809ef90d6020b21b89a87a48edc7c03aea80e5ed5174172e82d76e3987 \
     --hash=sha256:dc6884be91558df077c3011b9fb0c87d1097cb8fc6534b11f310161afd5738f0
+wcmatch==8.5.1 \
+    --hash=sha256:24c19cedc92bc9c9e27f39db4e1824d72f95bd2cea32b254a47a45b1a1b227ed \
+    --hash=sha256:c0088c7f6426cf6bf27e530e2b7b734031905f7e490475fd83c7c5008ab581b3
+wcwidth==0.2.13 \
+    --hash=sha256:3da69048e4540d84af32131829ff948f1e022c1c6bdb8d6102117aac784f6859 \
+    --hash=sha256:72ea0c06399eb286d978fdedb6923a9eb47e1c486ce63e9b4e64fc18303972b5
```

### Comparing `karp_lex_types-0.6.2/tests/test_entry_commands.py` & `karp_lex_types-0.6.4/tests/test_entry_commands.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.6.2/tests/test_resource_commands.py` & `karp_lex_types-0.6.4/tests/test_resource_commands.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.6.2/tests/test_unique_id.py` & `karp_lex_types-0.6.4/tests/test_unique_id.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.6.2/.gitignore` & `karp_lex_types-0.6.4/.gitignore`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.6.2/LICENSE` & `karp_lex_types-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.6.2/pyproject.toml` & `karp_lex_types-0.6.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 authors = [
-    { name = "Språkbanken at the University of Gothenburg", email = "sb-info@svenska.gu.se" },
+    { name = "Språkbanken Text", email = "sb-info@svenska.gu.se" },
     { name = "Kristoffer Andersson", email = "kristoffer.andersson@gu.se" },
 ]
 license = { text = "MIT" }
 requires-python = ">=3.10"
-dependencies = ["pydantic<3.0.0,>=2.5.3", "ulid-py<2.0.0,>=1.1.0"]
+dependencies = ["pydantic>=2.5.3", "ulid-py>=1.1.0"]
 name = "karp-lex-types"
-version = "0.6.2"
+version = "0.6.4"
 description = "The types of karp-lex"
 readme = "README.md"
 
 [project.urls]
 "Bug Tracker" = "https://github.com/spraakbanken/karp-lex-types/issues"
 homepage = "https://spraakbanken.gu.se"
 repository = "https://github.com/spraakbanken/karp-lex-types"
@@ -29,17 +29,16 @@
 exclude = ["/.github", "/docs"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/karp_lex_types"]
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "pytest<8.0.0,>=7.2.1",
-    "pytest-cov<5.0.0,>=4.0.0",
-    "bump2version<2.0.0,>=1.0.1",
+    "pytest>=8.2.0",
+    "pytest-cov>=5.0.0",
     "mypy>=1.10.0",
-    "ruff<1.0.0,>=0.1.14",
+    "ruff>=0.4.4",
+    "bump-my-version>=0.21.0",
 ]
 
 [tool.pdm.build]
 includes = ["src/karp_lex_types"]
-
```

### Comparing `karp_lex_types-0.6.2/PKG-INFO` & `karp_lex_types-0.6.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.3
 Name: karp-lex-types
-Version: 0.6.2
+Version: 0.6.4
 Summary: The types of karp-lex
 Project-URL: Bug Tracker, https://github.com/spraakbanken/karp-lex-types/issues
 Project-URL: homepage, https://spraakbanken.gu.se
 Project-URL: repository, https://github.com/spraakbanken/karp-lex-types
 Project-URL: documentation, https://github.com/spraakbanken/karp-lex-types
-Author-email: Språkbanken at the University of Gothenburg <sb-info@svenska.gu.se>, Kristoffer Andersson <kristoffer.andersson@gu.se>
+Author-email: Språkbanken Text <sb-info@svenska.gu.se>, Kristoffer Andersson <kristoffer.andersson@gu.se>
 License: MIT
 License-File: LICENSE
 Requires-Python: >=3.10
-Requires-Dist: pydantic<3.0.0,>=2.5.3
-Requires-Dist: ulid-py<2.0.0,>=1.1.0
+Requires-Dist: pydantic>=2.5.3
+Requires-Dist: ulid-py>=1.1.0
 Description-Content-Type: text/markdown
 
 # karp-lex-core
 
 - **karp-lex-core** [![PyPI version](https://badge.fury.io/py/karp-lex-core.svg)](https://badge.fury.io/py/karp-lex-core)
 
 The core for karp-lex
```

