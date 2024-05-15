# Comparing `tmp/domjudge_tool_cli-0.2.4.tar.gz` & `tmp/domjudge_tool_cli-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domjudge_tool_cli-0.2.4.tar", max compression
+gzip compressed data, was "domjudge_tool_cli-0.2.5.tar", max compression
```

## Comparing `domjudge_tool_cli-0.2.4.tar` & `domjudge_tool_cli-0.2.5.tar`

### file list

```diff
@@ -1,49 +1,48 @@
--rw-r--r--   0        0        0      870 2022-03-24 09:50:32.804104 domjudge_tool_cli-0.2.4/domjudge_tool_cli/__init__.py
--rw-r--r--   0        0        0      185 2022-11-17 07:17:25.351702 domjudge_tool_cli-0.2.4/domjudge_tool_cli/commands/__init__.py
--rw-r--r--   0        0        0     1518 2022-10-14 08:56:15.706036 domjudge_tool_cli-0.2.4/domjudge_tool_cli/commands/emails/__init__.py
--rw-r--r--   0        0        0     4972 2022-11-17 07:17:25.441065 domjudge_tool_cli-0.2.4/domjudge_tool_cli/commands/general/__init__.py
--rw-r--r--   0        0        0     2460 2022-10-27 05:41:55.681585 domjudge_tool_cli-0.2.4/domjudge_tool_cli/commands/general/_check.py
--rw-r--r--   0        0        0      875 2022-11-17 07:17:25.371350 domjudge_tool_cli-0.2.4/domjudge_tool_cli/commands/problems/__init__.py
--rw-r--r--   0        0        0     1397 2022-10-14 09:01:41.801917 domjudge_tool_cli-0.2.4/domjudge_tool_cli/commands/problems/_problems.py
--rw-r--r--   0        0        0     3188 2023-01-12 07:20:01.951457 domjudge_tool_cli-0.2.4/domjudge_tool_cli/commands/scoreboard/__init__.py
--rw-r--r--   0        0        0     2705 2022-11-17 07:17:25.388239 domjudge_tool_cli-0.2.4/domjudge_tool_cli/commands/submissions/__init__.py
--rw-r--r--   0        0        0     5378 2022-11-17 07:17:25.446114 domjudge_tool_cli-0.2.4/domjudge_tool_cli/commands/submissions/_submissions.py
--rw-r--r--   0        0        0     3330 2022-11-17 07:17:25.420711 domjudge_tool_cli-0.2.4/domjudge_tool_cli/commands/users/__init__.py
--rw-r--r--   0        0        0     7925 2022-11-29 10:26:36.491907 domjudge_tool_cli-0.2.4/domjudge_tool_cli/commands/users/_users.py
--rw-r--r--   0        0        0      515 2022-04-26 09:07:01.357656 domjudge_tool_cli-0.2.4/domjudge_tool_cli/models/__init__.py
--rw-r--r--   0        0        0      200 2022-01-22 04:32:55.930327 domjudge_tool_cli-0.2.4/domjudge_tool_cli/models/affiliation.py
--rw-r--r--   0        0        0     1347 2022-10-14 07:30:22.997902 domjudge_tool_cli-0.2.4/domjudge_tool_cli/models/domserver.py
--rw-r--r--   0        0        0      253 2022-10-14 09:07:28.771624 domjudge_tool_cli-0.2.4/domjudge_tool_cli/models/judgement_types.py
--rw-r--r--   0        0        0      776 2022-11-20 07:29:40.922508 domjudge_tool_cli-0.2.4/domjudge_tool_cli/models/judgements.py
--rw-r--r--   0        0        0      432 2022-04-26 07:23:55.506919 domjudge_tool_cli-0.2.4/domjudge_tool_cli/models/problem.py
--rw-r--r--   0        0        0      563 2022-01-22 04:32:55.923460 domjudge_tool_cli-0.2.4/domjudge_tool_cli/models/submission.py
--rw-r--r--   0        0        0      325 2022-01-22 04:32:55.926390 domjudge_tool_cli-0.2.4/domjudge_tool_cli/models/team.py
--rw-r--r--   0        0        0     1241 2022-03-24 09:50:32.811429 domjudge_tool_cli-0.2.4/domjudge_tool_cli/models/user.py
--rw-r--r--   0        0        0       87 2022-10-14 07:49:45.282148 domjudge_tool_cli-0.2.4/domjudge_tool_cli/services/__init__.py
--rw-r--r--   0        0        0        0 2022-10-14 07:22:43.523028 domjudge_tool_cli-0.2.4/domjudge_tool_cli/services/api/__init__.py
--rw-r--r--   0        0        0      395 2022-10-14 08:53:06.127513 domjudge_tool_cli-0.2.4/domjudge_tool_cli/services/api/v4/__init__.py
--rw-r--r--   0        0        0      241 2022-10-14 08:57:19.443161 domjudge_tool_cli-0.2.4/domjudge_tool_cli/services/api/v4/base.py
--rw-r--r--   0        0        0      211 2021-10-28 08:31:35.241459 domjudge_tool_cli-0.2.4/domjudge_tool_cli/services/api/v4/general.py
--rw-r--r--   0        0        0     1152 2022-10-14 09:07:28.811982 domjudge_tool_cli-0.2.4/domjudge_tool_cli/services/api/v4/judgement_types.py
--rw-r--r--   0        0        0     1136 2022-10-14 09:07:28.817133 domjudge_tool_cli-0.2.4/domjudge_tool_cli/services/api/v4/judgements.py
--rw-r--r--   0        0        0      637 2022-10-14 09:01:41.831886 domjudge_tool_cli-0.2.4/domjudge_tool_cli/services/api/v4/problems.py
--rw-r--r--   0        0        0     2664 2022-11-17 07:17:25.407362 domjudge_tool_cli-0.2.4/domjudge_tool_cli/services/api/v4/submissions.py
--rw-r--r--   0        0        0      607 2022-10-14 09:01:41.829054 domjudge_tool_cli-0.2.4/domjudge_tool_cli/services/api/v4/teams.py
--rw-r--r--   0        0        0      833 2022-10-14 09:01:41.828106 domjudge_tool_cli-0.2.4/domjudge_tool_cli/services/api/v4/users.py
--rw-r--r--   0        0        0     2991 2022-11-20 09:06:10.532030 domjudge_tool_cli-0.2.4/domjudge_tool_cli/services/api_client.py
--rw-r--r--   0        0        0      465 2022-11-04 08:06:54.884400 domjudge_tool_cli-0.2.4/domjudge_tool_cli/services/web/__init__.py
--rw-r--r--   0        0        0     2632 2022-10-17 08:29:34.055819 domjudge_tool_cli-0.2.4/domjudge_tool_cli/services/web/base.py
--rw-r--r--   0        0        0     8945 2022-11-20 09:06:19.965167 domjudge_tool_cli-0.2.4/domjudge_tool_cli/services/web/v7.py
--rw-r--r--   0        0        0     9173 2022-11-17 07:17:25.533815 domjudge_tool_cli-0.2.4/domjudge_tool_cli/services/web/v8.py
--rw-r--r--   0        0        0       90 2021-11-29 04:31:33.889585 domjudge_tool_cli-0.2.4/domjudge_tool_cli/templates/csv/import-users-teams.csv
--rw-r--r--   0        0        0        0 2022-02-18 06:22:16.326848 domjudge_tool_cli-0.2.4/domjudge_tool_cli/templates/email/body.html
--rw-r--r--   0        0        0        0 2022-02-18 06:22:25.459693 domjudge_tool_cli-0.2.4/domjudge_tool_cli/templates/email/body.txt
--rw-r--r--   0        0        0        0 2022-02-18 05:59:06.177187 domjudge_tool_cli-0.2.4/domjudge_tool_cli/templates/email/subject.txt
--rw-r--r--   0        0        0        0 2021-10-27 14:14:10.957061 domjudge_tool_cli-0.2.4/domjudge_tool_cli/utils/__init__.py
--rw-r--r--   0        0        0        0 2022-02-18 06:26:32.696696 domjudge_tool_cli-0.2.4/domjudge_tool_cli/utils/email/__init__.py
--rw-r--r--   0        0        0     2336 2022-03-24 09:50:32.808438 domjudge_tool_cli-0.2.4/domjudge_tool_cli/utils/email/helper.py
--rw-r--r--   0        0        0     2134 2022-10-14 09:00:22.080674 domjudge_tool_cli-0.2.4/domjudge_tool_cli/utils/email/smtp.py
--rw-r--r--   0        0        0      252 2022-01-22 04:32:55.919386 domjudge_tool_cli-0.2.4/domjudge_tool_cli/utils/password.py
--rw-r--r--   0        0        0      675 2023-01-12 07:20:45.190243 domjudge_tool_cli-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1500 1970-01-01 00:00:00.000000 domjudge_tool_cli-0.2.4/setup.py
--rw-r--r--   0        0        0      734 1970-01-01 00:00:00.000000 domjudge_tool_cli-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      870 2022-03-24 09:50:32.804104 domjudge_tool_cli-0.2.5/domjudge_tool_cli/__init__.py
+-rw-r--r--   0        0        0      185 2022-11-17 07:17:25.351702 domjudge_tool_cli-0.2.5/domjudge_tool_cli/commands/__init__.py
+-rw-r--r--   0        0        0     1518 2022-10-14 08:56:15.706036 domjudge_tool_cli-0.2.5/domjudge_tool_cli/commands/emails/__init__.py
+-rw-r--r--   0        0        0     4972 2022-11-17 07:17:25.441065 domjudge_tool_cli-0.2.5/domjudge_tool_cli/commands/general/__init__.py
+-rw-r--r--   0        0        0     2460 2022-10-27 05:41:55.681585 domjudge_tool_cli-0.2.5/domjudge_tool_cli/commands/general/_check.py
+-rw-r--r--   0        0        0      875 2022-11-17 07:17:25.371350 domjudge_tool_cli-0.2.5/domjudge_tool_cli/commands/problems/__init__.py
+-rw-r--r--   0        0        0     1397 2022-10-14 09:01:41.801917 domjudge_tool_cli-0.2.5/domjudge_tool_cli/commands/problems/_problems.py
+-rw-r--r--   0        0        0     3188 2023-01-14 14:54:59.840626 domjudge_tool_cli-0.2.5/domjudge_tool_cli/commands/scoreboard/__init__.py
+-rw-r--r--   0        0        0     2705 2022-11-17 07:17:25.388239 domjudge_tool_cli-0.2.5/domjudge_tool_cli/commands/submissions/__init__.py
+-rw-r--r--   0        0        0     5378 2022-11-17 07:17:25.446114 domjudge_tool_cli-0.2.5/domjudge_tool_cli/commands/submissions/_submissions.py
+-rw-r--r--   0        0        0     3402 2024-04-09 08:50:11.468391 domjudge_tool_cli-0.2.5/domjudge_tool_cli/commands/users/__init__.py
+-rw-r--r--   0        0        0     8036 2024-04-09 08:50:11.460040 domjudge_tool_cli-0.2.5/domjudge_tool_cli/commands/users/_users.py
+-rw-r--r--   0        0        0      515 2022-04-26 09:07:01.357656 domjudge_tool_cli-0.2.5/domjudge_tool_cli/models/__init__.py
+-rw-r--r--   0        0        0      200 2022-01-22 04:32:55.930327 domjudge_tool_cli-0.2.5/domjudge_tool_cli/models/affiliation.py
+-rw-r--r--   0        0        0     1347 2022-10-14 07:30:22.997902 domjudge_tool_cli-0.2.5/domjudge_tool_cli/models/domserver.py
+-rw-r--r--   0        0        0      253 2022-10-14 09:07:28.771624 domjudge_tool_cli-0.2.5/domjudge_tool_cli/models/judgement_types.py
+-rw-r--r--   0        0        0      776 2022-11-20 07:29:40.922508 domjudge_tool_cli-0.2.5/domjudge_tool_cli/models/judgements.py
+-rw-r--r--   0        0        0      432 2022-04-26 07:23:55.506919 domjudge_tool_cli-0.2.5/domjudge_tool_cli/models/problem.py
+-rw-r--r--   0        0        0      563 2022-01-22 04:32:55.923460 domjudge_tool_cli-0.2.5/domjudge_tool_cli/models/submission.py
+-rw-r--r--   0        0        0      325 2022-01-22 04:32:55.926390 domjudge_tool_cli-0.2.5/domjudge_tool_cli/models/team.py
+-rw-r--r--   0        0        0     1241 2022-03-24 09:50:32.811429 domjudge_tool_cli-0.2.5/domjudge_tool_cli/models/user.py
+-rw-r--r--   0        0        0       87 2022-10-14 07:49:45.282148 domjudge_tool_cli-0.2.5/domjudge_tool_cli/services/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-14 07:22:43.523028 domjudge_tool_cli-0.2.5/domjudge_tool_cli/services/api/__init__.py
+-rw-r--r--   0        0        0      395 2022-10-14 08:53:06.127513 domjudge_tool_cli-0.2.5/domjudge_tool_cli/services/api/v4/__init__.py
+-rw-r--r--   0        0        0      241 2022-10-14 08:57:19.443161 domjudge_tool_cli-0.2.5/domjudge_tool_cli/services/api/v4/base.py
+-rw-r--r--   0        0        0      211 2021-10-28 08:31:35.241459 domjudge_tool_cli-0.2.5/domjudge_tool_cli/services/api/v4/general.py
+-rw-r--r--   0        0        0     1152 2022-10-14 09:07:28.811982 domjudge_tool_cli-0.2.5/domjudge_tool_cli/services/api/v4/judgement_types.py
+-rw-r--r--   0        0        0     1136 2022-10-14 09:07:28.817133 domjudge_tool_cli-0.2.5/domjudge_tool_cli/services/api/v4/judgements.py
+-rw-r--r--   0        0        0      637 2022-10-14 09:01:41.831886 domjudge_tool_cli-0.2.5/domjudge_tool_cli/services/api/v4/problems.py
+-rw-r--r--   0        0        0     2838 2024-04-17 01:25:07.460904 domjudge_tool_cli-0.2.5/domjudge_tool_cli/services/api/v4/submissions.py
+-rw-r--r--   0        0        0      607 2022-10-14 09:01:41.829054 domjudge_tool_cli-0.2.5/domjudge_tool_cli/services/api/v4/teams.py
+-rw-r--r--   0        0        0      833 2022-10-14 09:01:41.828106 domjudge_tool_cli-0.2.5/domjudge_tool_cli/services/api/v4/users.py
+-rw-r--r--   0        0        0     2991 2022-11-20 09:06:10.532030 domjudge_tool_cli-0.2.5/domjudge_tool_cli/services/api_client.py
+-rw-r--r--   0        0        0      465 2022-11-04 08:06:54.884400 domjudge_tool_cli-0.2.5/domjudge_tool_cli/services/web/__init__.py
+-rw-r--r--   0        0        0     2632 2022-10-17 08:29:34.055819 domjudge_tool_cli-0.2.5/domjudge_tool_cli/services/web/base.py
+-rw-r--r--   0        0        0     8945 2024-01-08 09:56:38.532736 domjudge_tool_cli-0.2.5/domjudge_tool_cli/services/web/v7.py
+-rw-r--r--   0        0        0     9173 2022-11-17 07:17:25.533815 domjudge_tool_cli-0.2.5/domjudge_tool_cli/services/web/v8.py
+-rw-r--r--   0        0        0       90 2021-11-29 04:31:33.889585 domjudge_tool_cli-0.2.5/domjudge_tool_cli/templates/csv/import-users-teams.csv
+-rw-r--r--   0        0        0        0 2022-02-18 06:22:16.326848 domjudge_tool_cli-0.2.5/domjudge_tool_cli/templates/email/body.html
+-rw-r--r--   0        0        0        0 2022-02-18 06:22:25.459693 domjudge_tool_cli-0.2.5/domjudge_tool_cli/templates/email/body.txt
+-rw-r--r--   0        0        0        0 2022-02-18 05:59:06.177187 domjudge_tool_cli-0.2.5/domjudge_tool_cli/templates/email/subject.txt
+-rw-r--r--   0        0        0        0 2021-10-27 14:14:10.957061 domjudge_tool_cli-0.2.5/domjudge_tool_cli/utils/__init__.py
+-rw-r--r--   0        0        0        0 2022-02-18 06:26:32.696696 domjudge_tool_cli-0.2.5/domjudge_tool_cli/utils/email/__init__.py
+-rw-r--r--   0        0        0     2336 2022-03-24 09:50:32.808438 domjudge_tool_cli-0.2.5/domjudge_tool_cli/utils/email/helper.py
+-rw-r--r--   0        0        0     2134 2022-10-14 09:00:22.080674 domjudge_tool_cli-0.2.5/domjudge_tool_cli/utils/email/smtp.py
+-rw-r--r--   0        0        0      252 2022-01-22 04:32:55.919386 domjudge_tool_cli-0.2.5/domjudge_tool_cli/utils/password.py
+-rw-r--r--   0        0        0      675 2024-05-15 09:46:14.550991 domjudge_tool_cli-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      785 1970-01-01 00:00:00.000000 domjudge_tool_cli-0.2.5/PKG-INFO
```

### Comparing `domjudge_tool_cli-0.2.4/domjudge_tool_cli/__init__.py` & `domjudge_tool_cli-0.2.5/domjudge_tool_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `domjudge_tool_cli-0.2.4/domjudge_tool_cli/commands/emails/__init__.py` & `domjudge_tool_cli-0.2.5/domjudge_tool_cli/commands/emails/__init__.py`

 * *Files identical despite different names*

### Comparing `domjudge_tool_cli-0.2.4/domjudge_tool_cli/commands/general/__init__.py` & `domjudge_tool_cli-0.2.5/domjudge_tool_cli/commands/general/__init__.py`

 * *Files identical despite different names*

### Comparing `domjudge_tool_cli-0.2.4/domjudge_tool_cli/commands/general/_check.py` & `domjudge_tool_cli-0.2.5/domjudge_tool_cli/commands/general/_check.py`

 * *Files identical despite different names*

### Comparing `domjudge_tool_cli-0.2.4/domjudge_tool_cli/commands/problems/__init__.py` & `domjudge_tool_cli-0.2.5/domjudge_tool_cli/commands/problems/__init__.py`

 * *Files identical despite different names*

### Comparing `domjudge_tool_cli-0.2.4/domjudge_tool_cli/commands/problems/_problems.py` & `domjudge_tool_cli-0.2.5/domjudge_tool_cli/commands/problems/_problems.py`

 * *Files identical despite different names*

### Comparing `domjudge_tool_cli-0.2.4/domjudge_tool_cli/commands/scoreboard/__init__.py` & `domjudge_tool_cli-0.2.5/domjudge_tool_cli/commands/scoreboard/__init__.py`

 * *Files identical despite different names*

### Comparing `domjudge_tool_cli-0.2.4/domjudge_tool_cli/commands/submissions/__init__.py` & `domjudge_tool_cli-0.2.5/domjudge_tool_cli/commands/submissions/__init__.py`

 * *Files identical despite different names*

### Comparing `domjudge_tool_cli-0.2.4/domjudge_tool_cli/commands/submissions/_submissions.py` & `domjudge_tool_cli-0.2.5/domjudge_tool_cli/commands/submissions/_submissions.py`

 * *Files identical despite different names*

### Comparing `domjudge_tool_cli-0.2.4/domjudge_tool_cli/commands/users/__init__.py` & `domjudge_tool_cli-0.2.5/domjudge_tool_cli/commands/users/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,15 @@
     format: Optional[UserExportFormat] = None,
     ignore_existing: bool = typer.Option(False),
     delete_existing: bool = typer.Option(False),
     password_length: Optional[int] = typer.Option(None),
     password_pattern: Optional[str] = typer.Option(
         None, help="Random charset, ex: 0123456789"
     ),
+    new_password: bool = typer.Option(False),
 ):
     client = get_or_ask_config(general_state["config"])
     asyncio.run(
         create_teams_and_users(
             client,
             file,
             category_id,
@@ -115,14 +116,15 @@
             user_roles,
             enabled,
             format,
             ignore_existing,
             delete_existing,
             password_length,
             password_pattern,
+            new_password,
         ),
     )
 
 
 @app.command()
 def rm_teams_and_users(
     include: Optional[List[str]] = typer.Option(None),
```

### Comparing `domjudge_tool_cli-0.2.4/domjudge_tool_cli/commands/users/_users.py` & `domjudge_tool_cli-0.2.5/domjudge_tool_cli/commands/users/_users.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,23 +89,25 @@
     user: Union[CreateUser, User],
     category_id: Optional[int] = None,
     affiliation_id: Optional[int] = None,
     user_roles: Optional[List[int]] = None,
     enabled: bool = True,
     password_length: Optional[int] = None,
     password_pattern: Optional[str] = None,
+    new_password: bool = False,
 ) -> CreateUser:
     if not category_id:
         category_id = client.category_id
 
     if not user_roles:
         user_roles = client.user_roles
 
-    if not user.password:
+    if not user.password or new_password:
         user.password = gen_password(password_length, password_pattern)
+
     DomServerWeb = DomServerWebGateway(client.version)
     async with DomServerWeb(**client.api_params) as web:
         await web.login()
         if not affiliation_id and not user.affiliation:
             affiliation_id = client.affiliation_id
         elif user.affiliation:
             affiliation = await web.get_affiliation(user.affiliation)
@@ -150,14 +152,15 @@
     user_roles: Optional[List[int]] = None,
     enabled: bool = True,
     format: Optional[UserExportFormat] = None,
     ignore_existing: bool = False,
     delete_existing: bool = False,
     password_length: Optional[int] = None,
     password_pattern: Optional[str] = None,
+    new_password: bool = False,
 ) -> None:
     async with UsersAPI(**client.api_params) as api:
         users = await api.all_users()
 
     existing_users: Dict[str, User] = {it.username: it for it in users}
 
     if not format:
@@ -215,14 +218,15 @@
                 user,
                 category_id,
                 affiliation_id,
                 user_roles,
                 enabled,
                 password_length,
                 password_pattern,
+                new_password,
             )
             new_users.append(new_user)
 
     if new_users:
         file_name = format.export(new_users, name="import-users-teams-out")
         typer.echo(file_name)
```

### Comparing `domjudge_tool_cli-0.2.4/domjudge_tool_cli/models/__init__.py` & `domjudge_tool_cli-0.2.5/domjudge_tool_cli/models/__init__.py`

 * *Files identical despite different names*

### Comparing `domjudge_tool_cli-0.2.4/domjudge_tool_cli/models/domserver.py` & `domjudge_tool_cli-0.2.5/domjudge_tool_cli/models/domserver.py`

 * *Files identical despite different names*

### Comparing `domjudge_tool_cli-0.2.4/domjudge_tool_cli/models/judgements.py` & `domjudge_tool_cli-0.2.5/domjudge_tool_cli/models/judgements.py`

 * *Files identical despite different names*

### Comparing `domjudge_tool_cli-0.2.4/domjudge_tool_cli/models/submission.py` & `domjudge_tool_cli-0.2.5/domjudge_tool_cli/models/submission.py`

 * *Files identical despite different names*

### Comparing `domjudge_tool_cli-0.2.4/domjudge_tool_cli/models/user.py` & `domjudge_tool_cli-0.2.5/domjudge_tool_cli/models/user.py`

 * *Files identical despite different names*

### Comparing `domjudge_tool_cli-0.2.4/domjudge_tool_cli/services/api/v4/judgement_types.py` & `domjudge_tool_cli-0.2.5/domjudge_tool_cli/services/api/v4/judgement_types.py`

 * *Files identical despite different names*

### Comparing `domjudge_tool_cli-0.2.4/domjudge_tool_cli/services/api/v4/judgements.py` & `domjudge_tool_cli-0.2.5/domjudge_tool_cli/services/api/v4/judgements.py`

 * *Files identical despite different names*

### Comparing `domjudge_tool_cli-0.2.4/domjudge_tool_cli/services/api/v4/problems.py` & `domjudge_tool_cli-0.2.5/domjudge_tool_cli/services/api/v4/problems.py`

 * *Files identical despite different names*

### Comparing `domjudge_tool_cli-0.2.4/domjudge_tool_cli/services/api/v4/submissions.py` & `domjudge_tool_cli-0.2.5/domjudge_tool_cli/services/api/v4/submissions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import logging
 import shutil
 from glob import glob
 from pathlib import Path
 from typing import List, Optional
 
 import aiofiles
 from aiofiles import os as aio_os
@@ -64,15 +65,19 @@
         zip_path = Path(file_path) / file_name
         async with aiofiles.open(zip_path, "wb") as f:
             await f.write(result)
 
         if is_extract:
             async with aiofiles.tempfile.TemporaryDirectory() as temp_dir:
                 await unpack_archive(zip_path, temp_dir, "zip")
-                file = glob(str(temp_dir) + "/*")[0]
+                files = list(glob(str(temp_dir) + "/*"))
+                if not files:
+                    logging.warning(f"{zip_path} unzip fail!")
+                    return ""
+                file = files[0]
                 file_ex = os.path.splitext(file)[-1]
                 await aio_os.rename(
                     file,
                     Path(file_path) / f"{filename}_{id}{file_ex}",
                 )
                 await aio_os.remove(zip_path)
```

### Comparing `domjudge_tool_cli-0.2.4/domjudge_tool_cli/services/api/v4/teams.py` & `domjudge_tool_cli-0.2.5/domjudge_tool_cli/services/api/v4/teams.py`

 * *Files identical despite different names*

### Comparing `domjudge_tool_cli-0.2.4/domjudge_tool_cli/services/api/v4/users.py` & `domjudge_tool_cli-0.2.5/domjudge_tool_cli/services/api/v4/users.py`

 * *Files identical despite different names*

### Comparing `domjudge_tool_cli-0.2.4/domjudge_tool_cli/services/api_client.py` & `domjudge_tool_cli-0.2.5/domjudge_tool_cli/services/api_client.py`

 * *Files identical despite different names*

### Comparing `domjudge_tool_cli-0.2.4/domjudge_tool_cli/services/web/base.py` & `domjudge_tool_cli-0.2.5/domjudge_tool_cli/services/web/base.py`

 * *Files identical despite different names*

### Comparing `domjudge_tool_cli-0.2.4/domjudge_tool_cli/services/web/v7.py` & `domjudge_tool_cli-0.2.5/domjudge_tool_cli/services/web/v7.py`

 * *Files identical despite different names*

### Comparing `domjudge_tool_cli-0.2.4/domjudge_tool_cli/services/web/v8.py` & `domjudge_tool_cli-0.2.5/domjudge_tool_cli/services/web/v8.py`

 * *Files identical despite different names*

### Comparing `domjudge_tool_cli-0.2.4/domjudge_tool_cli/utils/email/helper.py` & `domjudge_tool_cli-0.2.5/domjudge_tool_cli/utils/email/helper.py`

 * *Files identical despite different names*

### Comparing `domjudge_tool_cli-0.2.4/domjudge_tool_cli/utils/email/smtp.py` & `domjudge_tool_cli-0.2.5/domjudge_tool_cli/utils/email/smtp.py`

 * *Files identical despite different names*

### Comparing `domjudge_tool_cli-0.2.4/pyproject.toml` & `domjudge_tool_cli-0.2.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "domjudge-tool-cli"
-version = "0.2.4"
+version = "0.2.5"
 description = "DomJudge dom server cli tool."
 authors = ["Jason Xie <x5758x@gmail.com>"]
 
 [tool.poetry.scripts]
 domjudge-tool-cli = "domjudge_tool_cli:app"
```

### Comparing `domjudge_tool_cli-0.2.4/PKG-INFO` & `domjudge_tool_cli-0.2.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: domjudge-tool-cli
-Version: 0.2.4
+Version: 0.2.5
 Summary: DomJudge dom server cli tool.
 Author: Jason Xie
 Author-email: x5758x@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiofiles (>=0.8.0,<0.9.0)
 Requires-Dist: beautifulsoup4 (>=4.10.0,<5.0.0)
 Requires-Dist: httpx (>=0.19.0,<0.20.0)
 Requires-Dist: openpyxl (>=3.0.9,<4.0.0)
 Requires-Dist: pydantic[dotenv,email] (>=1.8.2,<2.0.0)
 Requires-Dist: tablib[all] (>=3.0.0,<4.0.0)
 Requires-Dist: typer (>=0.4.0,<0.5.0)
```

