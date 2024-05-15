# Comparing `tmp/rc3-0.0.4.tar.gz` & `tmp/rc3-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rc3-0.0.4.tar", last modified: Wed May  8 19:50:09 2024, max compression
+gzip compressed data, was "rc3-0.0.5.tar", last modified: Wed May 15 20:05:03 2024, max compression
```

## Comparing `rc3-0.0.4.tar` & `rc3-0.0.5.tar`

### file list

```diff
@@ -1,152 +1,152 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.352792 rc3-0.0.4/
--rw-rw-rw-   0        0        0     3141 2024-05-06 19:59:38.000000 rc3-0.0.4/.gitignore
--rw-rw-rw-   0        0        0     1087 2024-05-06 20:36:33.000000 rc3-0.0.4/LICENSE
--rw-rw-rw-   0        0        0    11429 2024-05-08 19:50:09.351793 rc3-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     9378 2024-05-08 19:25:58.000000 rc3-0.0.4/README.md
--rw-rw-rw-   0        0        0     1044 2024-05-07 23:16:04.000000 rc3-0.0.4/WINDOWS_SETUP.md
--rw-rw-rw-   0        0        0      823 2024-05-08 19:40:54.000000 rc3-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      475 2024-05-06 20:07:47.000000 rc3-0.0.4/rc3.iml
--rw-rw-rw-   0        0        0       42 2024-05-08 19:50:09.352792 rc3-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.192160 rc3-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.210349 rc3-0.0.4/src/rc3/
--rw-rw-rw-   0        0        0      246 2024-05-06 19:59:38.000000 rc3-0.0.4/src/rc3/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.222689 rc3-0.0.4/src/rc3/archive/
--rw-rw-rw-   0        0        0        0 2024-05-06 19:59:38.000000 rc3-0.0.4/src/rc3/archive/__init__.py
--rw-rw-rw-   0        0        0      406 2024-05-06 20:00:31.000000 rc3-0.0.4/src/rc3/archive/cmd_home.py
--rw-rw-rw-   0        0        0      637 2024-05-06 20:00:31.000000 rc3-0.0.4/src/rc3/archive/cmd_root.py
--rw-rw-rw-   0        0        0     1125 2024-05-06 20:00:31.000000 rc3-0.0.4/src/rc3/archive/cmd_subs.py
--rw-rw-rw-   0        0        0     1924 2024-05-07 23:36:03.000000 rc3-0.0.4/src/rc3/cli.py
-drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.234641 rc3-0.0.4/src/rc3/commands/
--rw-rw-rw-   0        0        0        0 2024-05-06 19:59:38.000000 rc3-0.0.4/src/rc3/commands/__init__.py
--rw-rw-rw-   0        0        0     3415 2024-05-06 22:52:43.000000 rc3-0.0.4/src/rc3/commands/cmd_collection.py
--rw-rw-rw-   0        0        0     5467 2024-05-07 23:33:42.000000 rc3-0.0.4/src/rc3/commands/cmd_environment.py
--rw-rw-rw-   0        0        0     1454 2024-05-07 23:35:00.000000 rc3-0.0.4/src/rc3/commands/cmd_global.py
--rw-rw-rw-   0        0        0      524 2024-05-06 19:59:38.000000 rc3-0.0.4/src/rc3/commands/cmd_hello.py
--rw-rw-rw-   0        0        0     2559 2024-05-06 23:00:33.000000 rc3-0.0.4/src/rc3/commands/cmd_init.py
--rw-rw-rw-   0        0        0     2136 2024-05-08 19:24:17.000000 rc3-0.0.4/src/rc3/commands/cmd_list.py
--rw-rw-rw-   0        0        0     4322 2024-05-06 20:00:31.000000 rc3-0.0.4/src/rc3/commands/cmd_request.py
--rw-rw-rw-   0        0        0     9478 2024-05-08 18:59:18.000000 rc3-0.0.4/src/rc3/commands/cmd_send.py
--rw-rw-rw-   0        0        0     1368 2024-05-08 18:10:08.000000 rc3-0.0.4/src/rc3/commands/cmd_settings.py
-drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.244942 rc3-0.0.4/src/rc3/common/
--rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.4/src/rc3/common/__init__.py
--rw-rw-rw-   0        0        0      524 2024-05-06 19:59:39.000000 rc3-0.0.4/src/rc3/common/config_helper.py
--rw-rw-rw-   0        0        0      869 2024-05-06 22:59:13.000000 rc3-0.0.4/src/rc3/common/data_helper.py
--rw-rw-rw-   0        0        0      936 2024-05-06 19:59:39.000000 rc3-0.0.4/src/rc3/common/decorators.py
--rw-rw-rw-   0        0        0     2670 2024-05-06 20:00:31.000000 rc3-0.0.4/src/rc3/common/env_helper.py
--rw-rw-rw-   0        0        0     1364 2024-05-06 22:52:57.000000 rc3-0.0.4/src/rc3/common/inherit_helper.py
--rw-rw-rw-   0        0        0    10723 2024-05-08 18:47:05.000000 rc3-0.0.4/src/rc3/common/json_helper.py
--rw-rw-rw-   0        0        0     2503 2024-05-08 19:08:29.000000 rc3-0.0.4/src/rc3/common/print_helper.py
--rw-rw-rw-   0        0        0       86 2024-05-06 19:59:39.000000 rc3-0.0.4/src/rc3/common/rc_globals.py
-drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.245941 rc3-0.0.4/src/rc3/data/
--rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.4/src/rc3/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.246940 rc3-0.0.4/src/rc3/data/collection/
-drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.249938 rc3-0.0.4/src/rc3/data/collection/environments/
--rw-rw-rw-   0        0        0      277 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/environments/dev.json
--rw-rw-rw-   0        0        0      307 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/environments/localhost.json
-drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.263930 rc3-0.0.4/src/rc3/data/collection/examples/
--rw-rw-rw-   0        0        0      247 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/examples/example_Auth_Basic.request
--rw-rw-rw-   0        0        0      914 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/examples/example_Auth_Bearer.request
--rw-rw-rw-   0        0        0      960 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/examples/example_Auth_Token.request
--rw-rw-rw-   0        0        0      436 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/examples/example_Extract_JsonPath.request
--rw-rw-rw-   0        0        0      455 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/examples/example_Extract_Regex.request
--rw-rw-rw-   0        0        0      190 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/examples/example_GET.request
--rw-rw-rw-   0        0        0      799 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/examples/example_KitchenSink.request
--rw-rw-rw-   0        0        0      401 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/examples/example_MintOauth2Token.request
--rw-rw-rw-   0        0        0      275 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/examples/example_POST_json.request
--rw-rw-rw-   0        0        0      231 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/examples/example_POST_text-plain.request
--rw-rw-rw-   0        0        0      240 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/examples/example_QueryParams.request
--rw-rw-rw-   0        0        0      227 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/examples/example_UseOauth2Token.request
--rw-rw-rw-   0        0        0      272 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/examples/folder.json
-drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.270926 rc3-0.0.4/src/rc3/data/collection/greetings-basic/
--rw-rw-rw-   0        0        0      384 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/greetings-basic/greeting.request
--rw-rw-rw-   0        0        0      180 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/greetings-basic/greetings.request
--rw-rw-rw-   0        0        0      291 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/greetings-basic/new-greeting.request
--rw-rw-rw-   0        0        0      297 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/greetings-basic/rc-folder.json
--rw-rw-rw-   0        0        0      185 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/greetings-basic/remove-greeting.request
--rw-rw-rw-   0        0        0      313 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/greetings-basic/update-greeting.request
-drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.274922 rc3-0.0.4/src/rc3/data/collection/greetings-oauth2/
--rw-rw-rw-   0        0        0      218 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/greetings-oauth2/greeting.request
--rw-rw-rw-   0        0        0      466 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/greetings-oauth2/mint-admin-token.request
--rw-rw-rw-   0        0        0      465 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/greetings-oauth2/mint-token.request
--rw-rw-rw-   0        0        0      247 2024-05-08 14:58:01.000000 rc3-0.0.4/src/rc3/data/collection/rc-collection.json
-drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.276922 rc3-0.0.4/src/rc3/data/home/
--rw-rw-rw-   0        0        0      130 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/home/rc-global.json
--rw-rw-rw-   0        0        0      354 2024-05-07 23:02:39.000000 rc3-0.0.4/src/rc3/data/home/rc-settings.json
-drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.284917 rc3-0.0.4/src/rc3/data/home/schemas/
--rw-rw-rw-   0        0        0     1151 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/home/schemas/rc3-auth-0.0.3.json
--rw-rw-rw-   0        0        0      918 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/home/schemas/rc3-collection-0.0.3.json
--rw-rw-rw-   0        0        0      473 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/home/schemas/rc3-environment-0.0.3.json
--rw-rw-rw-   0        0        0      605 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/home/schemas/rc3-folder-0.0.3.json
--rw-rw-rw-   0        0        0     3241 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/home/schemas/rc3-request-0.0.3.json
--rw-rw-rw-   0        0        0     2259 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/home/schemas/rc3-settings-0.0.3.json
-drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.349590 rc3-0.0.4/src/rc3.egg-info/
--rw-rw-rw-   0        0        0    11429 2024-05-08 19:50:08.000000 rc3-0.0.4/src/rc3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5183 2024-05-08 19:50:09.000000 rc3-0.0.4/src/rc3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 19:50:08.000000 rc3-0.0.4/src/rc3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-05-08 19:50:08.000000 rc3-0.0.4/src/rc3.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      100 2024-05-08 19:50:08.000000 rc3-0.0.4/src/rc3.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-08 19:50:08.000000 rc3-0.0.4/src/rc3.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.285915 rc3-0.0.4/temp-collection/
-drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.287915 rc3-0.0.4/temp-collection/environments/
--rw-rw-rw-   0        0        0      277 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/environments/dev.json
--rw-rw-rw-   0        0        0      307 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/environments/localhost.json
-drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.304921 rc3-0.0.4/temp-collection/examples/
--rw-rw-rw-   0        0        0      247 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/examples/example_Auth_Basic.request
--rw-rw-rw-   0        0        0      914 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/examples/example_Auth_Bearer.request
--rw-rw-rw-   0        0        0      960 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/examples/example_Auth_Token.request
--rw-rw-rw-   0        0        0      436 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/examples/example_Extract_JsonPath.request
--rw-rw-rw-   0        0        0      455 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/examples/example_Extract_Regex.request
--rw-rw-rw-   0        0        0      190 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/examples/example_GET.request
--rw-rw-rw-   0        0        0      799 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/examples/example_KitchenSink.request
--rw-rw-rw-   0        0        0      401 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/examples/example_MintOauth2Token.request
--rw-rw-rw-   0        0        0      275 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/examples/example_POST_json.request
--rw-rw-rw-   0        0        0      231 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/examples/example_POST_text-plain.request
--rw-rw-rw-   0        0        0      240 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/examples/example_QueryParams.request
--rw-rw-rw-   0        0        0      227 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/examples/example_UseOauth2Token.request
--rw-rw-rw-   0        0        0      272 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/examples/folder.json
-drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.315029 rc3-0.0.4/temp-collection/greetings-basic/
--rw-rw-rw-   0        0        0      384 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/greetings-basic/greeting.request
--rw-rw-rw-   0        0        0     1038 2024-05-08 19:32:46.000000 rc3-0.0.4/temp-collection/greetings-basic/greeting.response
--rw-rw-rw-   0        0        0      180 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/greetings-basic/greetings.request
--rw-rw-rw-   0        0        0     1480 2024-05-08 19:32:39.000000 rc3-0.0.4/temp-collection/greetings-basic/greetings.response
--rw-rw-rw-   0        0        0      291 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/greetings-basic/new-greeting.request
--rw-rw-rw-   0        0        0      297 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/greetings-basic/rc-folder.json
--rw-rw-rw-   0        0        0      185 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/greetings-basic/remove-greeting.request
--rw-rw-rw-   0        0        0      313 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/greetings-basic/update-greeting.request
-drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.318027 rc3-0.0.4/temp-collection/greetings-oauth2/
--rw-rw-rw-   0        0        0      218 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/greetings-oauth2/greeting.request
--rw-rw-rw-   0        0        0      466 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/greetings-oauth2/mint-admin-token.request
--rw-rw-rw-   0        0        0      465 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/greetings-oauth2/mint-token.request
--rw-rw-rw-   0        0        0      255 2024-05-08 19:32:46.000000 rc3-0.0.4/temp-collection/rc-collection.json
-drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.321878 rc3-0.0.4/tests/
--rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.4/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.329602 rc3-0.0.4/tests/commands/
--rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.4/tests/commands/__init__.py
--rw-rw-rw-   0        0        0      599 2024-05-06 20:00:31.000000 rc3-0.0.4/tests/commands/test_collection.py
--rw-rw-rw-   0        0        0     5698 2024-05-06 20:00:31.000000 rc3-0.0.4/tests/commands/test_environment.py
--rw-rw-rw-   0        0        0     1856 2024-05-08 19:17:23.000000 rc3-0.0.4/tests/commands/test_init.py
--rw-rw-rw-   0        0        0      427 2024-05-06 20:00:31.000000 rc3-0.0.4/tests/commands/test_list.py
--rw-rw-rw-   0        0        0     5923 2024-05-06 20:00:31.000000 rc3-0.0.4/tests/commands/test_request.py
--rw-rw-rw-   0        0        0     6322 2024-05-06 20:00:31.000000 rc3-0.0.4/tests/commands/test_send.py
-drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.339597 rc3-0.0.4/tests/commands/test_send_files/
--rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.4/tests/commands/test_send_files/test_is_verbose.yaml
--rw-rw-rw-   0        0        0     1178 2024-05-06 19:59:39.000000 rc3-0.0.4/tests/commands/test_send_files/test_mint_extract_use_token.yaml
--rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.4/tests/commands/test_send_files/test_not_verbose.yaml
--rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.4/tests/commands/test_send_files/test_request_no_responses.yaml
--rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.4/tests/commands/test_send_files/test_send_1.yaml
--rw-rw-rw-   0        0        0      663 2024-05-06 19:59:39.000000 rc3-0.0.4/tests/commands/test_send_files/test_send_2.yaml
--rw-rw-rw-   0        0        0     1098 2024-05-06 19:59:39.000000 rc3-0.0.4/tests/commands/test_send_files/test_send_basics.yaml
--rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.4/tests/commands/test_send_files/test_settings_no_responses.yaml
--rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.4/tests/commands/test_send_files/test_settings_with_responses.yaml
-drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.342594 rc3-0.0.4/tests/common/
--rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.4/tests/common/__init__.py
--rw-rw-rw-   0        0        0     5211 2024-05-06 20:00:31.000000 rc3-0.0.4/tests/common/test_env_helper.py
--rw-rw-rw-   0        0        0     3345 2024-05-06 22:51:48.000000 rc3-0.0.4/tests/common/test_inherit_helper.py
--rw-rw-rw-   0        0        0     1124 2024-05-06 20:00:31.000000 rc3-0.0.4/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.345591 rc3-0.0.4/tests/learning/
--rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.4/tests/learning/__init__.py
--rw-rw-rw-   0        0        0      518 2024-05-06 19:59:39.000000 rc3-0.0.4/tests/learning/test_sample.py
--rw-rw-rw-   0        0        0     1665 2024-05-06 20:00:31.000000 rc3-0.0.4/tests/test_cli.py
-drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.347591 rc3-0.0.4/tests/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.4/tests/util/__init__.py
--rw-rw-rw-   0        0        0     1407 2024-05-06 19:59:39.000000 rc3-0.0.4/tests/util/decorators.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.944085 rc3-0.0.5/
+-rw-rw-rw-   0        0        0     3141 2024-05-06 19:59:38.000000 rc3-0.0.5/.gitignore
+-rw-rw-rw-   0        0        0     1087 2024-05-06 20:36:33.000000 rc3-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0    11488 2024-05-15 20:05:03.942087 rc3-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     9437 2024-05-15 20:01:38.000000 rc3-0.0.5/README.md
+-rw-rw-rw-   0        0        0     1044 2024-05-07 23:16:04.000000 rc3-0.0.5/WINDOWS_SETUP.md
+-rw-rw-rw-   0        0        0      823 2024-05-15 20:04:21.000000 rc3-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      475 2024-05-06 20:07:47.000000 rc3-0.0.5/rc3.iml
+-rw-rw-rw-   0        0        0       42 2024-05-15 20:05:03.945086 rc3-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.749005 rc3-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.772041 rc3-0.0.5/src/rc3/
+-rw-rw-rw-   0        0        0      246 2024-05-06 19:59:38.000000 rc3-0.0.5/src/rc3/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.793028 rc3-0.0.5/src/rc3/archive/
+-rw-rw-rw-   0        0        0        0 2024-05-06 19:59:38.000000 rc3-0.0.5/src/rc3/archive/__init__.py
+-rw-rw-rw-   0        0        0      406 2024-05-06 20:00:31.000000 rc3-0.0.5/src/rc3/archive/cmd_home.py
+-rw-rw-rw-   0        0        0      637 2024-05-06 20:00:31.000000 rc3-0.0.5/src/rc3/archive/cmd_root.py
+-rw-rw-rw-   0        0        0     1125 2024-05-06 20:00:31.000000 rc3-0.0.5/src/rc3/archive/cmd_subs.py
+-rw-rw-rw-   0        0        0     1924 2024-05-07 23:36:03.000000 rc3-0.0.5/src/rc3/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.815156 rc3-0.0.5/src/rc3/commands/
+-rw-rw-rw-   0        0        0        0 2024-05-06 19:59:38.000000 rc3-0.0.5/src/rc3/commands/__init__.py
+-rw-rw-rw-   0        0        0     3415 2024-05-06 22:52:43.000000 rc3-0.0.5/src/rc3/commands/cmd_collection.py
+-rw-rw-rw-   0        0        0     5467 2024-05-07 23:33:42.000000 rc3-0.0.5/src/rc3/commands/cmd_environment.py
+-rw-rw-rw-   0        0        0     1454 2024-05-07 23:35:00.000000 rc3-0.0.5/src/rc3/commands/cmd_global.py
+-rw-rw-rw-   0        0        0      524 2024-05-06 19:59:38.000000 rc3-0.0.5/src/rc3/commands/cmd_hello.py
+-rw-rw-rw-   0        0        0     3414 2024-05-15 20:01:43.000000 rc3-0.0.5/src/rc3/commands/cmd_init.py
+-rw-rw-rw-   0        0        0     2136 2024-05-08 19:24:17.000000 rc3-0.0.5/src/rc3/commands/cmd_list.py
+-rw-rw-rw-   0        0        0     4322 2024-05-06 20:00:31.000000 rc3-0.0.5/src/rc3/commands/cmd_request.py
+-rw-rw-rw-   0        0        0     9478 2024-05-08 18:59:18.000000 rc3-0.0.5/src/rc3/commands/cmd_send.py
+-rw-rw-rw-   0        0        0     1368 2024-05-08 18:10:08.000000 rc3-0.0.5/src/rc3/commands/cmd_settings.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.828203 rc3-0.0.5/src/rc3/common/
+-rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.5/src/rc3/common/__init__.py
+-rw-rw-rw-   0        0        0      524 2024-05-06 19:59:39.000000 rc3-0.0.5/src/rc3/common/config_helper.py
+-rw-rw-rw-   0        0        0      869 2024-05-06 22:59:13.000000 rc3-0.0.5/src/rc3/common/data_helper.py
+-rw-rw-rw-   0        0        0      936 2024-05-06 19:59:39.000000 rc3-0.0.5/src/rc3/common/decorators.py
+-rw-rw-rw-   0        0        0     2670 2024-05-06 20:00:31.000000 rc3-0.0.5/src/rc3/common/env_helper.py
+-rw-rw-rw-   0        0        0     1364 2024-05-06 22:52:57.000000 rc3-0.0.5/src/rc3/common/inherit_helper.py
+-rw-rw-rw-   0        0        0    10723 2024-05-08 18:47:05.000000 rc3-0.0.5/src/rc3/common/json_helper.py
+-rw-rw-rw-   0        0        0     2503 2024-05-08 19:08:29.000000 rc3-0.0.5/src/rc3/common/print_helper.py
+-rw-rw-rw-   0        0        0       86 2024-05-06 19:59:39.000000 rc3-0.0.5/src/rc3/common/rc_globals.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.829202 rc3-0.0.5/src/rc3/data/
+-rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.5/src/rc3/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.830201 rc3-0.0.5/src/rc3/data/collection/
+drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.834936 rc3-0.0.5/src/rc3/data/collection/environments/
+-rw-rw-rw-   0        0        0        6 2024-05-15 19:30:06.000000 rc3-0.0.5/src/rc3/data/collection/environments/.gitignore
+-rw-rw-rw-   0        0        0      277 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/environments/dev.defaults
+-rw-rw-rw-   0        0        0      307 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/environments/localhost.defaults
+drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.850927 rc3-0.0.5/src/rc3/data/collection/examples/
+-rw-rw-rw-   0        0        0      247 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/examples/example_Auth_Basic.request
+-rw-rw-rw-   0        0        0      914 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/examples/example_Auth_Bearer.request
+-rw-rw-rw-   0        0        0      960 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/examples/example_Auth_Token.request
+-rw-rw-rw-   0        0        0      436 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/examples/example_Extract_JsonPath.request
+-rw-rw-rw-   0        0        0      455 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/examples/example_Extract_Regex.request
+-rw-rw-rw-   0        0        0      190 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/examples/example_GET.request
+-rw-rw-rw-   0        0        0      799 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/examples/example_KitchenSink.request
+-rw-rw-rw-   0        0        0      401 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/examples/example_MintOauth2Token.request
+-rw-rw-rw-   0        0        0      275 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/examples/example_POST_json.request
+-rw-rw-rw-   0        0        0      231 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/examples/example_POST_text-plain.request
+-rw-rw-rw-   0        0        0      240 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/examples/example_QueryParams.request
+-rw-rw-rw-   0        0        0      227 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/examples/example_UseOauth2Token.request
+-rw-rw-rw-   0        0        0      272 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/examples/folder.json
+drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.858548 rc3-0.0.5/src/rc3/data/collection/greetings-basic/
+-rw-rw-rw-   0        0        0      384 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/greetings-basic/greeting.request
+-rw-rw-rw-   0        0        0      180 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/greetings-basic/greetings.request
+-rw-rw-rw-   0        0        0      291 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/greetings-basic/new-greeting.request
+-rw-rw-rw-   0        0        0      297 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/greetings-basic/rc-folder.json
+-rw-rw-rw-   0        0        0      185 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/greetings-basic/remove-greeting.request
+-rw-rw-rw-   0        0        0      313 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/greetings-basic/update-greeting.request
+drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.861546 rc3-0.0.5/src/rc3/data/collection/greetings-oauth2/
+-rw-rw-rw-   0        0        0      218 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/greetings-oauth2/greeting.request
+-rw-rw-rw-   0        0        0      466 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/greetings-oauth2/mint-admin-token.request
+-rw-rw-rw-   0        0        0      465 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/greetings-oauth2/mint-token.request
+-rw-rw-rw-   0        0        0      247 2024-05-08 14:58:01.000000 rc3-0.0.5/src/rc3/data/collection/rc-collection.json
+drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.864543 rc3-0.0.5/src/rc3/data/home/
+-rw-rw-rw-   0        0        0      130 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/home/rc-global.json
+-rw-rw-rw-   0        0        0      354 2024-05-07 23:02:39.000000 rc3-0.0.5/src/rc3/data/home/rc-settings.json
+drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.873014 rc3-0.0.5/src/rc3/data/home/schemas/
+-rw-rw-rw-   0        0        0     1151 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/home/schemas/rc3-auth-0.0.3.json
+-rw-rw-rw-   0        0        0      918 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/home/schemas/rc3-collection-0.0.3.json
+-rw-rw-rw-   0        0        0      473 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/home/schemas/rc3-environment-0.0.3.json
+-rw-rw-rw-   0        0        0      605 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/home/schemas/rc3-folder-0.0.3.json
+-rw-rw-rw-   0        0        0     3241 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/home/schemas/rc3-request-0.0.3.json
+-rw-rw-rw-   0        0        0     2259 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/home/schemas/rc3-settings-0.0.3.json
+drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.939088 rc3-0.0.5/src/rc3.egg-info/
+-rw-rw-rw-   0        0        0    11488 2024-05-15 20:05:03.000000 rc3-0.0.5/src/rc3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5186 2024-05-15 20:05:03.000000 rc3-0.0.5/src/rc3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 20:05:03.000000 rc3-0.0.5/src/rc3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-05-15 20:05:03.000000 rc3-0.0.5/src/rc3.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      100 2024-05-15 20:05:03.000000 rc3-0.0.5/src/rc3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-15 20:05:03.000000 rc3-0.0.5/src/rc3.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.874013 rc3-0.0.5/temp-collection/
+drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.878014 rc3-0.0.5/temp-collection/environments/
+-rw-rw-rw-   0        0        0        6 2024-05-15 19:30:06.000000 rc3-0.0.5/temp-collection/environments/.gitignore
+-rw-rw-rw-   0        0        0      277 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/environments/dev.defaults
+-rw-rw-rw-   0        0        0      307 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/environments/localhost.defaults
+drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.893486 rc3-0.0.5/temp-collection/examples/
+-rw-rw-rw-   0        0        0      247 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/examples/example_Auth_Basic.request
+-rw-rw-rw-   0        0        0      914 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/examples/example_Auth_Bearer.request
+-rw-rw-rw-   0        0        0      960 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/examples/example_Auth_Token.request
+-rw-rw-rw-   0        0        0      436 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/examples/example_Extract_JsonPath.request
+-rw-rw-rw-   0        0        0      455 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/examples/example_Extract_Regex.request
+-rw-rw-rw-   0        0        0      190 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/examples/example_GET.request
+-rw-rw-rw-   0        0        0      799 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/examples/example_KitchenSink.request
+-rw-rw-rw-   0        0        0      401 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/examples/example_MintOauth2Token.request
+-rw-rw-rw-   0        0        0      275 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/examples/example_POST_json.request
+-rw-rw-rw-   0        0        0      231 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/examples/example_POST_text-plain.request
+-rw-rw-rw-   0        0        0      240 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/examples/example_QueryParams.request
+-rw-rw-rw-   0        0        0      227 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/examples/example_UseOauth2Token.request
+-rw-rw-rw-   0        0        0      272 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/examples/folder.json
+drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.900482 rc3-0.0.5/temp-collection/greetings-basic/
+-rw-rw-rw-   0        0        0      384 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/greetings-basic/greeting.request
+-rw-rw-rw-   0        0        0      180 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/greetings-basic/greetings.request
+-rw-rw-rw-   0        0        0      291 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/greetings-basic/new-greeting.request
+-rw-rw-rw-   0        0        0      297 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/greetings-basic/rc-folder.json
+-rw-rw-rw-   0        0        0      185 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/greetings-basic/remove-greeting.request
+-rw-rw-rw-   0        0        0      313 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/greetings-basic/update-greeting.request
+drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.904479 rc3-0.0.5/temp-collection/greetings-oauth2/
+-rw-rw-rw-   0        0        0      218 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/greetings-oauth2/greeting.request
+-rw-rw-rw-   0        0        0      466 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/greetings-oauth2/mint-admin-token.request
+-rw-rw-rw-   0        0        0      465 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/greetings-oauth2/mint-token.request
+-rw-rw-rw-   0        0        0      247 2024-05-08 14:58:01.000000 rc3-0.0.5/temp-collection/rc-collection.json
+drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.907480 rc3-0.0.5/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.5/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.918470 rc3-0.0.5/tests/commands/
+-rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.5/tests/commands/__init__.py
+-rw-rw-rw-   0        0        0      599 2024-05-06 20:00:31.000000 rc3-0.0.5/tests/commands/test_collection.py
+-rw-rw-rw-   0        0        0     5698 2024-05-06 20:00:31.000000 rc3-0.0.5/tests/commands/test_environment.py
+-rw-rw-rw-   0        0        0     1856 2024-05-08 19:17:23.000000 rc3-0.0.5/tests/commands/test_init.py
+-rw-rw-rw-   0        0        0      427 2024-05-06 20:00:31.000000 rc3-0.0.5/tests/commands/test_list.py
+-rw-rw-rw-   0        0        0     5923 2024-05-06 20:00:31.000000 rc3-0.0.5/tests/commands/test_request.py
+-rw-rw-rw-   0        0        0     6322 2024-05-06 20:00:31.000000 rc3-0.0.5/tests/commands/test_send.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.930460 rc3-0.0.5/tests/commands/test_send_files/
+-rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.5/tests/commands/test_send_files/test_is_verbose.yaml
+-rw-rw-rw-   0        0        0     1178 2024-05-06 19:59:39.000000 rc3-0.0.5/tests/commands/test_send_files/test_mint_extract_use_token.yaml
+-rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.5/tests/commands/test_send_files/test_not_verbose.yaml
+-rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.5/tests/commands/test_send_files/test_request_no_responses.yaml
+-rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.5/tests/commands/test_send_files/test_send_1.yaml
+-rw-rw-rw-   0        0        0      663 2024-05-06 19:59:39.000000 rc3-0.0.5/tests/commands/test_send_files/test_send_2.yaml
+-rw-rw-rw-   0        0        0     1098 2024-05-06 19:59:39.000000 rc3-0.0.5/tests/commands/test_send_files/test_send_basics.yaml
+-rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.5/tests/commands/test_send_files/test_settings_no_responses.yaml
+-rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.5/tests/commands/test_send_files/test_settings_with_responses.yaml
+drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.932972 rc3-0.0.5/tests/common/
+-rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.5/tests/common/__init__.py
+-rw-rw-rw-   0        0        0     5211 2024-05-06 20:00:31.000000 rc3-0.0.5/tests/common/test_env_helper.py
+-rw-rw-rw-   0        0        0     3345 2024-05-06 22:51:48.000000 rc3-0.0.5/tests/common/test_inherit_helper.py
+-rw-rw-rw-   0        0        0     1124 2024-05-06 20:00:31.000000 rc3-0.0.5/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.935091 rc3-0.0.5/tests/learning/
+-rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.5/tests/learning/__init__.py
+-rw-rw-rw-   0        0        0      518 2024-05-06 19:59:39.000000 rc3-0.0.5/tests/learning/test_sample.py
+-rw-rw-rw-   0        0        0     1665 2024-05-06 20:00:31.000000 rc3-0.0.5/tests/test_cli.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.937090 rc3-0.0.5/tests/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.5/tests/util/__init__.py
+-rw-rw-rw-   0        0        0     1407 2024-05-06 19:59:39.000000 rc3-0.0.5/tests/util/decorators.py
```

### Comparing `rc3-0.0.4/.gitignore` & `rc3-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/LICENSE` & `rc3-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/PKG-INFO` & `rc3-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rc3
-Version: 0.0.4
+Version: 0.0.5
 Summary: Rest CLI (rc)
 Author-email: Gary Wilcox <gary@dugan-wilcox.com>
 License: MIT License
         
         Copyright (c) 2018 Real Python
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -80,14 +80,15 @@
   ```
   $ rc init
   Creating C:\Users\Gary\.rc\rc-settings.json
   Creating C:\Users\Gary\.rc\rc-global.json                            
   Creating C:\Users\Gary\.rc\schemas                                   
   CWD is empty, creating sample Collection here: C:\dev\temp-collection
   Importing collection from: C:\dev\temp-collection
+  2 default environment(s) initialized in your collection
   Adding collection to global settings: example-collection
   ```
 * Next send the "greeting" request with the rc send command
   * Wait for it…
     * A greetings-demo project is running on Google Cloud Run
     * And it scales down to 0 instances when there is no demand (i.e. your first few requests will be SLOW…)  
   ```
```

### Comparing `rc3-0.0.4/README.md` & `rc3-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
   ```
   $ rc init
   Creating C:\Users\Gary\.rc\rc-settings.json
   Creating C:\Users\Gary\.rc\rc-global.json                            
   Creating C:\Users\Gary\.rc\schemas                                   
   CWD is empty, creating sample Collection here: C:\dev\temp-collection
   Importing collection from: C:\dev\temp-collection
+  2 default environment(s) initialized in your collection
   Adding collection to global settings: example-collection
   ```
 * Next send the "greeting" request with the rc send command
   * Wait for it…
     * A greetings-demo project is running on Google Cloud Run
     * And it scales down to 0 instances when there is no demand (i.e. your first few requests will be SLOW…)  
   ```
```

### Comparing `rc3-0.0.4/WINDOWS_SETUP.md` & `rc3-0.0.5/WINDOWS_SETUP.md`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/pyproject.toml` & `rc3-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","setuptools-scm","wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rc3"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Gary Wilcox", email="gary@dugan-wilcox.com" },
 ]
 readme = "README.md"
 license = { file = "LICENSE" }
 description = "Rest CLI (rc)"
 requires-python = ">=3.12"
```

### Comparing `rc3-0.0.4/src/rc3/archive/cmd_root.py` & `rc3-0.0.5/src/rc3/archive/cmd_root.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/src/rc3/archive/cmd_subs.py` & `rc3-0.0.5/src/rc3/archive/cmd_subs.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/src/rc3/cli.py` & `rc3-0.0.5/src/rc3/cli.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/src/rc3/commands/cmd_collection.py` & `rc3-0.0.5/src/rc3/commands/cmd_collection.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/src/rc3/commands/cmd_environment.py` & `rc3-0.0.5/src/rc3/commands/cmd_environment.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/src/rc3/commands/cmd_global.py` & `rc3-0.0.5/src/rc3/commands/cmd_global.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/src/rc3/commands/cmd_hello.py` & `rc3-0.0.5/src/rc3/commands/cmd_hello.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/src/rc3/commands/cmd_init.py` & `rc3-0.0.5/src/rc3/commands/cmd_init.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import os
+import shutil
+
 import click
 from rc3.common import config_helper, json_helper, data_helper
 from rc3.common.data_helper import SETTINGS_FILENAME, COLLECTION_FILENAME, GLOBAL_ENV_FILENAME
 
 
 @click.command("init", short_help="Init RC settings, and Collection files.")
 def cli():
@@ -32,14 +34,30 @@
 def import_collection():
     cwd = os.getcwd()
     print("Importing collection from: " + cwd)
     collection_dict = json_helper.load_and_validate(COLLECTION_FILENAME, _dir=cwd)
     if collection_dict is None:
         return
 
+    # for any .defaults environments in the collection, copy them to .json (i.e. make a real environment)
+    # note: there should also be a .gitignore in the env folder, so .json doesn't get committed
+    env_folder = os.path.join(cwd, 'environments')
+    defaults_counter = 0
+    for dirpath, dirnames, files in os.walk(env_folder):
+        for file in files:
+            if file.endswith('.defaults'):
+                name = file.split('.')[-2]
+                default_file = os.path.join(dirpath, file)
+                new_file = os.path.join(dirpath, name + ".json")
+                if not os.path.exists(new_file):
+                    defaults_counter += 1
+                    shutil.copy(default_file, new_file)
+    if defaults_counter > 0:
+        print(f"{defaults_counter} default environment(s) initialized in your collection")
+
     # get "name" from json, or use cwd directory name
     parts = os.path.split(cwd)
     name = collection_dict.get("name", parts[-1])
 
     settings = json_helper.read_settings()
     settings["current_collection"] = name
     # ONLY add to the collections list if name is NOT already there!
```

### Comparing `rc3-0.0.4/src/rc3/commands/cmd_list.py` & `rc3-0.0.5/src/rc3/commands/cmd_list.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/src/rc3/commands/cmd_request.py` & `rc3-0.0.5/src/rc3/commands/cmd_request.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/src/rc3/commands/cmd_send.py` & `rc3-0.0.5/src/rc3/commands/cmd_send.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/src/rc3/commands/cmd_settings.py` & `rc3-0.0.5/src/rc3/commands/cmd_settings.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/src/rc3/common/config_helper.py` & `rc3-0.0.5/src/rc3/common/config_helper.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/src/rc3/common/data_helper.py` & `rc3-0.0.5/src/rc3/common/data_helper.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/src/rc3/common/decorators.py` & `rc3-0.0.5/src/rc3/common/decorators.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/src/rc3/common/env_helper.py` & `rc3-0.0.5/src/rc3/common/env_helper.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/src/rc3/common/inherit_helper.py` & `rc3-0.0.5/src/rc3/common/inherit_helper.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/src/rc3/common/json_helper.py` & `rc3-0.0.5/src/rc3/common/json_helper.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/src/rc3/common/print_helper.py` & `rc3-0.0.5/src/rc3/common/print_helper.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/src/rc3/data/collection/examples/example_Auth_Bearer.request` & `rc3-0.0.5/src/rc3/data/collection/examples/example_Auth_Bearer.request`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/src/rc3/data/collection/examples/example_Auth_Token.request` & `rc3-0.0.5/src/rc3/data/collection/examples/example_Auth_Token.request`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/src/rc3/data/collection/examples/example_KitchenSink.request` & `rc3-0.0.5/src/rc3/data/collection/examples/example_KitchenSink.request`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/src/rc3/data/home/schemas/rc3-auth-0.0.3.json` & `rc3-0.0.5/src/rc3/data/home/schemas/rc3-auth-0.0.3.json`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/src/rc3/data/home/schemas/rc3-collection-0.0.3.json` & `rc3-0.0.5/src/rc3/data/home/schemas/rc3-collection-0.0.3.json`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/src/rc3/data/home/schemas/rc3-folder-0.0.3.json` & `rc3-0.0.5/src/rc3/data/home/schemas/rc3-folder-0.0.3.json`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/src/rc3/data/home/schemas/rc3-request-0.0.3.json` & `rc3-0.0.5/src/rc3/data/home/schemas/rc3-request-0.0.3.json`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/src/rc3/data/home/schemas/rc3-settings-0.0.3.json` & `rc3-0.0.5/src/rc3/data/home/schemas/rc3-settings-0.0.3.json`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/src/rc3.egg-info/PKG-INFO` & `rc3-0.0.5/src/rc3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rc3
-Version: 0.0.4
+Version: 0.0.5
 Summary: Rest CLI (rc)
 Author-email: Gary Wilcox <gary@dugan-wilcox.com>
 License: MIT License
         
         Copyright (c) 2018 Real Python
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -80,14 +80,15 @@
   ```
   $ rc init
   Creating C:\Users\Gary\.rc\rc-settings.json
   Creating C:\Users\Gary\.rc\rc-global.json                            
   Creating C:\Users\Gary\.rc\schemas                                   
   CWD is empty, creating sample Collection here: C:\dev\temp-collection
   Importing collection from: C:\dev\temp-collection
+  2 default environment(s) initialized in your collection
   Adding collection to global settings: example-collection
   ```
 * Next send the "greeting" request with the rc send command
   * Wait for it…
     * A greetings-demo project is running on Google Cloud Run
     * And it scales down to 0 instances when there is no demand (i.e. your first few requests will be SLOW…)  
   ```
```

### Comparing `rc3-0.0.4/src/rc3.egg-info/SOURCES.txt` & `rc3-0.0.5/src/rc3.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -33,16 +33,17 @@
 src/rc3/common/env_helper.py
 src/rc3/common/inherit_helper.py
 src/rc3/common/json_helper.py
 src/rc3/common/print_helper.py
 src/rc3/common/rc_globals.py
 src/rc3/data/__init__.py
 src/rc3/data/collection/rc-collection.json
-src/rc3/data/collection/environments/dev.json
-src/rc3/data/collection/environments/localhost.json
+src/rc3/data/collection/environments/.gitignore
+src/rc3/data/collection/environments/dev.defaults
+src/rc3/data/collection/environments/localhost.defaults
 src/rc3/data/collection/examples/example_Auth_Basic.request
 src/rc3/data/collection/examples/example_Auth_Bearer.request
 src/rc3/data/collection/examples/example_Auth_Token.request
 src/rc3/data/collection/examples/example_Extract_JsonPath.request
 src/rc3/data/collection/examples/example_Extract_Regex.request
 src/rc3/data/collection/examples/example_GET.request
 src/rc3/data/collection/examples/example_KitchenSink.request
@@ -66,33 +67,32 @@
 src/rc3/data/home/schemas/rc3-auth-0.0.3.json
 src/rc3/data/home/schemas/rc3-collection-0.0.3.json
 src/rc3/data/home/schemas/rc3-environment-0.0.3.json
 src/rc3/data/home/schemas/rc3-folder-0.0.3.json
 src/rc3/data/home/schemas/rc3-request-0.0.3.json
 src/rc3/data/home/schemas/rc3-settings-0.0.3.json
 temp-collection/rc-collection.json
-temp-collection/environments/dev.json
-temp-collection/environments/localhost.json
+temp-collection/environments/.gitignore
+temp-collection/environments/dev.defaults
+temp-collection/environments/localhost.defaults
 temp-collection/examples/example_Auth_Basic.request
 temp-collection/examples/example_Auth_Bearer.request
 temp-collection/examples/example_Auth_Token.request
 temp-collection/examples/example_Extract_JsonPath.request
 temp-collection/examples/example_Extract_Regex.request
 temp-collection/examples/example_GET.request
 temp-collection/examples/example_KitchenSink.request
 temp-collection/examples/example_MintOauth2Token.request
 temp-collection/examples/example_POST_json.request
 temp-collection/examples/example_POST_text-plain.request
 temp-collection/examples/example_QueryParams.request
 temp-collection/examples/example_UseOauth2Token.request
 temp-collection/examples/folder.json
 temp-collection/greetings-basic/greeting.request
-temp-collection/greetings-basic/greeting.response
 temp-collection/greetings-basic/greetings.request
-temp-collection/greetings-basic/greetings.response
 temp-collection/greetings-basic/new-greeting.request
 temp-collection/greetings-basic/rc-folder.json
 temp-collection/greetings-basic/remove-greeting.request
 temp-collection/greetings-basic/update-greeting.request
 temp-collection/greetings-oauth2/greeting.request
 temp-collection/greetings-oauth2/mint-admin-token.request
 temp-collection/greetings-oauth2/mint-token.request
```

### Comparing `rc3-0.0.4/temp-collection/examples/example_Auth_Bearer.request` & `rc3-0.0.5/temp-collection/examples/example_Auth_Bearer.request`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/temp-collection/examples/example_Auth_Token.request` & `rc3-0.0.5/temp-collection/examples/example_Auth_Token.request`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/temp-collection/examples/example_KitchenSink.request` & `rc3-0.0.5/temp-collection/examples/example_KitchenSink.request`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/tests/commands/test_collection.py` & `rc3-0.0.5/tests/commands/test_collection.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/tests/commands/test_environment.py` & `rc3-0.0.5/tests/commands/test_environment.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/tests/commands/test_init.py` & `rc3-0.0.5/tests/commands/test_init.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/tests/commands/test_request.py` & `rc3-0.0.5/tests/commands/test_request.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/tests/commands/test_send.py` & `rc3-0.0.5/tests/commands/test_send.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/tests/commands/test_send_files/test_mint_extract_use_token.yaml` & `rc3-0.0.5/tests/commands/test_send_files/test_mint_extract_use_token.yaml`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/tests/commands/test_send_files/test_send_2.yaml` & `rc3-0.0.5/tests/commands/test_send_files/test_send_2.yaml`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/tests/commands/test_send_files/test_send_basics.yaml` & `rc3-0.0.5/tests/commands/test_send_files/test_send_basics.yaml`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/tests/common/test_env_helper.py` & `rc3-0.0.5/tests/common/test_env_helper.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/tests/common/test_inherit_helper.py` & `rc3-0.0.5/tests/common/test_inherit_helper.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/tests/conftest.py` & `rc3-0.0.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/tests/learning/test_sample.py` & `rc3-0.0.5/tests/learning/test_sample.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/tests/test_cli.py` & `rc3-0.0.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.4/tests/util/decorators.py` & `rc3-0.0.5/tests/util/decorators.py`

 * *Files identical despite different names*

