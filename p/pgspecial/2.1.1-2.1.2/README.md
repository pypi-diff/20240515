# Comparing `tmp/pgspecial-2.1.1.tar.gz` & `tmp/pgspecial-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgspecial-2.1.1.tar", last modified: Sun Oct 29 23:08:44 2023, max compression
+gzip compressed data, was "pgspecial-2.1.2.tar", last modified: Wed May 15 20:57:30 2024, max compression
```

## Comparing `pgspecial-2.1.1.tar` & `pgspecial-2.1.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2023-10-29 23:08:44.172156 pgspecial-2.1.1/
--rw-r--r--   0 jbennet    (501) staff       (20)     5254 2023-10-28 23:32:24.000000 pgspecial-2.1.1/DEVELOP.rst
--rw-r--r--   0 jbennet    (501) staff       (20)     1472 2023-10-28 23:32:24.000000 pgspecial-2.1.1/License.txt
--rw-r--r--   0 jbennet    (501) staff       (20)     3180 2023-10-29 23:08:44.170875 pgspecial-2.1.1/PKG-INFO
--rw-r--r--   0 jbennet    (501) staff       (20)     2160 2023-10-28 23:32:24.000000 pgspecial-2.1.1/README.rst
--rw-r--r--   0 jbennet    (501) staff       (20)     7905 2023-10-29 23:07:30.000000 pgspecial-2.1.1/changelog.rst
-drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2023-10-29 23:08:44.159670 pgspecial-2.1.1/pgspecial/
--rw-r--r--   0 jbennet    (501) staff       (20)      269 2023-10-29 23:06:46.000000 pgspecial-2.1.1/pgspecial/__init__.py
--rw-r--r--   0 jbennet    (501) staff       (20)    73763 2023-10-28 23:32:24.000000 pgspecial-2.1.1/pgspecial/dbcommands.py
-drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2023-10-29 23:08:44.162451 pgspecial-2.1.1/pgspecial/help/
--rw-r--r--   0 jbennet    (501) staff       (20)        0 2023-10-28 23:32:24.000000 pgspecial-2.1.1/pgspecial/help/__init__.py
--rw-r--r--   0 jbennet    (501) staff       (20)    77881 2023-10-28 23:32:24.000000 pgspecial-2.1.1/pgspecial/help/commands.py
--rw-r--r--   0 jbennet    (501) staff       (20)    10256 2023-10-28 23:32:24.000000 pgspecial-2.1.1/pgspecial/iocommands.py
--rw-r--r--   0 jbennet    (501) staff       (20)     9853 2023-10-28 23:32:24.000000 pgspecial-2.1.1/pgspecial/main.py
--rw-r--r--   0 jbennet    (501) staff       (20)     1647 2023-10-28 23:32:24.000000 pgspecial-2.1.1/pgspecial/namedqueries.py
-drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2023-10-29 23:08:44.161724 pgspecial-2.1.1/pgspecial.egg-info/
--rw-r--r--   0 jbennet    (501) staff       (20)     3180 2023-10-29 23:08:44.000000 pgspecial-2.1.1/pgspecial.egg-info/PKG-INFO
--rw-r--r--   0 jbennet    (501) staff       (20)      582 2023-10-29 23:08:44.000000 pgspecial-2.1.1/pgspecial.egg-info/SOURCES.txt
--rw-r--r--   0 jbennet    (501) staff       (20)        1 2023-10-29 23:08:44.000000 pgspecial-2.1.1/pgspecial.egg-info/dependency_links.txt
--rw-r--r--   0 jbennet    (501) staff       (20)       44 2023-10-29 23:08:44.000000 pgspecial-2.1.1/pgspecial.egg-info/requires.txt
--rw-r--r--   0 jbennet    (501) staff       (20)       10 2023-10-29 23:08:44.000000 pgspecial-2.1.1/pgspecial.egg-info/top_level.txt
--rw-r--r--   0 jbennet    (501) staff       (20)      458 2023-10-28 23:32:24.000000 pgspecial-2.1.1/pyproject.toml
--rw-r--r--   0 jbennet    (501) staff       (20)      155 2023-10-29 23:05:57.000000 pgspecial-2.1.1/requirements-dev.txt
-drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2023-10-29 23:08:44.164094 pgspecial-2.1.1/scripts/
--rw-r--r--   0 jbennet    (501) staff       (20)      745 2023-10-28 23:32:24.000000 pgspecial-2.1.1/scripts/README.rst
--rw-r--r--   0 jbennet    (501) staff       (20)     1431 2023-10-28 23:32:24.000000 pgspecial-2.1.1/scripts/docparser.py
--rw-r--r--   0 jbennet    (501) staff       (20)       38 2023-10-29 23:08:44.172471 pgspecial-2.1.1/setup.cfg
--rw-r--r--   0 jbennet    (501) staff       (20)     1458 2023-10-28 23:32:24.000000 pgspecial-2.1.1/setup.py
-drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2023-10-29 23:08:44.168726 pgspecial-2.1.1/tests/
--rw-r--r--   0 jbennet    (501) staff       (20)      956 2023-10-28 23:42:00.000000 pgspecial-2.1.1/tests/conftest.py
--rw-r--r--   0 jbennet    (501) staff       (20)     5897 2023-10-28 23:32:24.000000 pgspecial-2.1.1/tests/dbutils.py
--rw-r--r--   0 jbennet    (501) staff       (20)     4072 2023-10-28 23:32:24.000000 pgspecial-2.1.1/tests/test_internal.py
--rw-r--r--   0 jbennet    (501) staff       (20)     1331 2023-10-28 23:32:24.000000 pgspecial-2.1.1/tests/test_named_queries.py
--rwxr-xr-x   0 jbennet    (501) staff       (20)    31683 2023-10-28 23:42:00.000000 pgspecial-2.1.1/tests/test_specials.py
--rw-r--r--   0 jbennet    (501) staff       (20)      114 2023-10-28 23:32:24.000000 pgspecial-2.1.1/tox.ini
+drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2024-05-15 20:57:30.775221 pgspecial-2.1.2/
+-rw-r--r--   0 jbennet    (501) staff       (20)     5254 2024-05-15 17:50:58.000000 pgspecial-2.1.2/DEVELOP.rst
+-rw-r--r--   0 jbennet    (501) staff       (20)     1472 2024-05-15 17:50:58.000000 pgspecial-2.1.2/License.txt
+-rw-r--r--   0 jbennet    (501) staff       (20)     3180 2024-05-15 20:57:30.775046 pgspecial-2.1.2/PKG-INFO
+-rw-r--r--   0 jbennet    (501) staff       (20)     2160 2024-05-15 17:50:58.000000 pgspecial-2.1.2/README.rst
+-rw-r--r--   0 jbennet    (501) staff       (20)     8003 2024-05-15 20:56:03.000000 pgspecial-2.1.2/changelog.rst
+drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2024-05-15 20:57:30.772805 pgspecial-2.1.2/pgspecial/
+-rw-r--r--   0 jbennet    (501) staff       (20)      256 2024-05-15 20:56:52.000000 pgspecial-2.1.2/pgspecial/__init__.py
+-rw-r--r--   0 jbennet    (501) staff       (20)    73937 2024-05-15 17:50:58.000000 pgspecial-2.1.2/pgspecial/dbcommands.py
+drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2024-05-15 20:57:30.773674 pgspecial-2.1.2/pgspecial/help/
+-rw-r--r--   0 jbennet    (501) staff       (20)        0 2024-05-15 17:50:58.000000 pgspecial-2.1.2/pgspecial/help/__init__.py
+-rw-r--r--   0 jbennet    (501) staff       (20)    77881 2024-05-15 17:50:58.000000 pgspecial-2.1.2/pgspecial/help/commands.py
+-rw-r--r--   0 jbennet    (501) staff       (20)    10256 2024-05-15 17:50:58.000000 pgspecial-2.1.2/pgspecial/iocommands.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     9853 2024-05-15 17:50:58.000000 pgspecial-2.1.2/pgspecial/main.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     1647 2024-05-15 17:50:58.000000 pgspecial-2.1.2/pgspecial/namedqueries.py
+drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2024-05-15 20:57:30.774839 pgspecial-2.1.2/pgspecial.egg-info/
+-rw-r--r--   0 jbennet    (501) staff       (20)     3180 2024-05-15 20:57:30.000000 pgspecial-2.1.2/pgspecial.egg-info/PKG-INFO
+-rw-r--r--   0 jbennet    (501) staff       (20)      582 2024-05-15 20:57:30.000000 pgspecial-2.1.2/pgspecial.egg-info/SOURCES.txt
+-rw-r--r--   0 jbennet    (501) staff       (20)        1 2024-05-15 20:57:30.000000 pgspecial-2.1.2/pgspecial.egg-info/dependency_links.txt
+-rw-r--r--   0 jbennet    (501) staff       (20)       44 2024-05-15 20:57:30.000000 pgspecial-2.1.2/pgspecial.egg-info/requires.txt
+-rw-r--r--   0 jbennet    (501) staff       (20)       10 2024-05-15 20:57:30.000000 pgspecial-2.1.2/pgspecial.egg-info/top_level.txt
+-rw-r--r--   0 jbennet    (501) staff       (20)      458 2024-05-15 17:50:58.000000 pgspecial-2.1.2/pyproject.toml
+-rw-r--r--   0 jbennet    (501) staff       (20)      155 2024-05-15 17:50:58.000000 pgspecial-2.1.2/requirements-dev.txt
+drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2024-05-15 20:57:30.773977 pgspecial-2.1.2/scripts/
+-rw-r--r--   0 jbennet    (501) staff       (20)      745 2024-05-15 17:50:58.000000 pgspecial-2.1.2/scripts/README.rst
+-rw-r--r--   0 jbennet    (501) staff       (20)     1431 2024-05-15 17:50:58.000000 pgspecial-2.1.2/scripts/docparser.py
+-rw-r--r--   0 jbennet    (501) staff       (20)       38 2024-05-15 20:57:30.775263 pgspecial-2.1.2/setup.cfg
+-rw-r--r--   0 jbennet    (501) staff       (20)     1458 2024-05-15 17:50:58.000000 pgspecial-2.1.2/setup.py
+drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2024-05-15 20:57:30.774627 pgspecial-2.1.2/tests/
+-rw-r--r--   0 jbennet    (501) staff       (20)      956 2024-05-15 17:50:58.000000 pgspecial-2.1.2/tests/conftest.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     5897 2024-05-15 17:50:58.000000 pgspecial-2.1.2/tests/dbutils.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     4072 2024-05-15 17:50:58.000000 pgspecial-2.1.2/tests/test_internal.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     1331 2024-05-15 17:50:58.000000 pgspecial-2.1.2/tests/test_named_queries.py
+-rwxr-xr-x   0 jbennet    (501) staff       (20)    31683 2024-05-15 17:50:58.000000 pgspecial-2.1.2/tests/test_specials.py
+-rw-r--r--   0 jbennet    (501) staff       (20)      114 2024-05-15 17:50:58.000000 pgspecial-2.1.2/tox.ini
```

### Comparing `pgspecial-2.1.1/DEVELOP.rst` & `pgspecial-2.1.2/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `pgspecial-2.1.1/License.txt` & `pgspecial-2.1.2/License.txt`

 * *Files identical despite different names*

### Comparing `pgspecial-2.1.1/PKG-INFO` & `pgspecial-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgspecial
-Version: 2.1.1
+Version: 2.1.2
 Summary: Meta-commands handler for Postgres Database.
 Home-page: https://www.dbcli.com
 Author: Pgcli Core Team
 Author-email: pgcli-dev@googlegroups.com
 License: LICENSE.txt
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pgspecial-2.1.1/README.rst` & `pgspecial-2.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `pgspecial-2.1.1/changelog.rst` & `pgspecial-2.1.2/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+2.1.2 (2024-05-15)
+==================
+
+Bug fixes:
+----------
+* Fix `\d` when used with a pattern
+
 2.1.1 (2023-10-29)
 ==================
 
 * Added `build-system` section to `pyproject.toml` to use the modern setuptools backend.
 * Fix SyntaxWarning with Python 3.12.
 * Fix test_slash_l* to support non-en_US locales (https://github.com/dbcli/pgspecial/issues/140).
 * Release script uses `build` module.
```

### Comparing `pgspecial-2.1.1/pgspecial/dbcommands.py` & `pgspecial-2.1.2/pgspecial/dbcommands.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,50 +13,50 @@
     [
         "checks",
         "relkind",
         "hasindex",
         "hasrules",
         "hastriggers",
         "hasoids",
-        "tablespace",
         "reloptions",
+        "tablespace",
         "reloftype",
         "relpersistence",
         "relispartition",
     ],
 )
 
 log = logging.getLogger(__name__)
 
 
 @special_command("\\l", "\\l[+] [pattern]", "List databases.", aliases=("\\list",))
 def list_databases(cur, pattern, verbose):
     params = {}
     query = SQL(
-        """SELECT d.datname as "Name",
-        pg_catalog.pg_get_userbyid(d.datdba) as "Owner",
-        pg_catalog.pg_encoding_to_char(d.encoding) as "Encoding",
-        d.datcollate as "Collate",
-        d.datctype as "Ctype",
-        pg_catalog.array_to_string(d.datacl, E'\n') AS "Access privileges"
+        """SELECT d.datname as name,
+        pg_catalog.pg_get_userbyid(d.datdba) as owner,
+        pg_catalog.pg_encoding_to_char(d.encoding) as encoding,
+        d.datcollate as collate,
+        d.datctype as ctype,
+        pg_catalog.array_to_string(d.datacl, E'\n') AS access_privileges
         {verbose_fields}
         FROM pg_catalog.pg_database d
         {verbose_tables}
         {pattern_where}
         ORDER BY 1"""
     )
     if verbose:
         params["verbose_fields"] = SQL(
-            ''',
+            """,
             CASE WHEN pg_catalog.has_database_privilege(d.datname, 'CONNECT')
                     THEN pg_catalog.pg_size_pretty(pg_catalog.pg_database_size(d.datname))
                     ELSE 'No Access'
-            END as "Size",
+            END as size,
             t.spcname as "Tablespace",
-            pg_catalog.shobj_description(d.oid, 'pg_database') as "Description"'''
+            pg_catalog.shobj_description(d.oid, 'pg_database') as description"""
         )
         params["verbose_tables"] = SQL(
             """JOIN pg_catalog.pg_tablespace t on d.dattablespace = t.oid"""
         )
     else:
         params["verbose_fields"] = SQL("")
         params["verbose_tables"] = SQL("")
@@ -66,15 +66,15 @@
         params["pattern_where"] = SQL("""WHERE d.datname ~ {}""").format(schema)
     else:
         params["pattern_where"] = SQL("")
     formatted_query = query.format(**params)
     log.debug(formatted_query.as_string(cur))
     cur.execute(formatted_query)
     if cur.description:
-        headers = [x.name for x in cur.description]
+        headers = [titleize(x.name) for x in cur.description]
         return [(None, cur, headers, cur.statusmessage)]
     else:
         return [(None, None, None, cur.statusmessage)]
 
 
 @special_command("\\du", "\\du[+] [pattern]", "List roles.")
 def list_roles(cur, pattern, verbose):
@@ -140,28 +140,29 @@
 
 
 @special_command("\\dp", "\\dp [pattern]", "List privileges.", aliases=("\\z",))
 def list_privileges(cur, pattern, verbose):
     """Returns (title, rows, headers, status)"""
     sql = SQL(
         """
-        SELECT n.nspname as "Schema",
-          c.relname as "Name",
+        SELECT n.nspname as schema,
+          c.relname as name,
           CASE c.relkind WHEN 'r' THEN 'table'
                          WHEN 'v' THEN 'view'
                          WHEN 'm' THEN 'materialized view'
                          WHEN 'S' THEN 'sequence'
                          WHEN 'f' THEN 'foreign table'
-                         WHEN 'p' THEN 'partitioned table' END as "Type",
-          pg_catalog.array_to_string(c.relacl, E'\n') AS "Access privileges",
+                         WHEN 'p' THEN 'partitioned table' END as type,
+          pg_catalog.array_to_string(c.relacl, E'\n') AS access_privileges,
+
           pg_catalog.array_to_string(ARRAY(
             SELECT attname || E':\n  ' || pg_catalog.array_to_string(attacl, E'\n  ')
             FROM pg_catalog.pg_attribute a
             WHERE attrelid = c.oid AND NOT attisdropped AND attacl IS NOT NULL
-          ), E'\n') AS "Column privileges",
+          ), E'\n') AS column_privileges,
           pg_catalog.array_to_string(ARRAY(
             SELECT polname
             || CASE WHEN NOT polpermissive THEN
                E' (RESTRICTIVE)'
                ELSE '' END
             || CASE WHEN polcmd != '*' THEN
                    E' (' || polcmd::pg_catalog.text || E'):'
@@ -182,15 +183,15 @@
                            WHERE oid = ANY (polroles)
                            ORDER BY 1
                        ), E', ')
                ELSE E''
                END
             FROM pg_catalog.pg_policy pol
             WHERE polrelid = c.oid), E'\n')
-            AS "Policies"
+            AS policies
         FROM pg_catalog.pg_class c
              LEFT JOIN pg_catalog.pg_namespace n ON n.oid = c.relnamespace
     """
     )
 
     if pattern:
         schema, table = sql_name_pattern(pattern)
@@ -214,31 +215,31 @@
     ).format(pattern=pattern)
 
     sql += where_clause + SQL(" ORDER BY 1, 2 ")
 
     log.debug(sql.as_string(cur))
     cur.execute(sql)
     if cur.description:
-        headers = [x.name for x in cur.description]
+        headers = [titleize(x.name) for x in cur.description]
         return [(None, cur, headers, cur.statusmessage)]
 
 
 @special_command("\\ddp", "\\ddp [pattern]", "Lists default access privilege settings.")
 def list_default_privileges(cur, pattern, verbose):
     """Returns (title, rows, headers, status)"""
     sql = SQL(
         """
-    SELECT pg_catalog.pg_get_userbyid(d.defaclrole) AS "Owner",
-    n.nspname AS "Schema",
+    SELECT pg_catalog.pg_get_userbyid(d.defaclrole) AS owner,
+    n.nspname AS schema,
     CASE d.defaclobjtype WHEN 'r' THEN 'table'
                          WHEN 'S' THEN 'sequence'
                          WHEN 'f' THEN 'function'
                          WHEN 'T' THEN 'type'
-                         WHEN 'n' THEN 'schema' END AS "Type",
-    pg_catalog.array_to_string(d.defaclacl, E'\n') AS "Access privileges"
+                         WHEN 'n' THEN 'schema' END as type,
+    pg_catalog.array_to_string(d.defaclacl, E'\n') AS access_privileges
     FROM pg_catalog.pg_default_acl d
         LEFT JOIN pg_catalog.pg_namespace n ON n.oid = d.defaclnamespace
         {where_clause}
     ORDER BY 1, 2, 3
     """
     )
 
@@ -252,15 +253,15 @@
         ).format(pattern=f"^({pattern})$")
     else:
         params["where_clause"] = SQL("")
 
     log.debug(sql.format(**params).as_string(cur))
     cur.execute(sql.format(**params))
     if cur.description:
-        headers = [x.name for x in cur.description]
+        headers = [titleize(x.name) for x in cur.description]
         return [(None, cur, headers, cur.statusmessage)]
 
 
 @special_command("\\db", "\\db[+] [pattern]", "List tablespaces.")
 def list_tablespaces(cur, pattern, **_):
     """
     Returns (title, rows, headers, status)
@@ -269,16 +270,16 @@
     params = {}
     cur.execute(
         "SELECT EXISTS(SELECT * FROM pg_proc WHERE proname = 'pg_tablespace_location')"
     )
     (is_location,) = cur.fetchone()
 
     sql = SQL(
-        """SELECT n.spcname AS "Name", pg_catalog.pg_get_userbyid(n.spcowner) AS "Owner",
-                {location} AS "Location" FROM pg_catalog.pg_tablespace n
+        """SELECT n.spcname AS name, pg_catalog.pg_get_userbyid(n.spcowner) AS owner,
+                {location} AS location FROM pg_catalog.pg_tablespace n
                 {pattern}
                 ORDER BY 1
               """
     )
 
     if is_location:
         params["location"] = SQL(" pg_catalog.pg_tablespace_location(n.oid)")
@@ -291,62 +292,63 @@
     else:
         params["pattern"] = SQL("")
 
     formatted_query = sql.format(**params)
     log.debug(formatted_query.as_string(cur))
     cur.execute(formatted_query)
 
-    headers = [x.name for x in cur.description] if cur.description else None
+    headers = [titleize(x.name) for x in cur.description] if cur.description else None
     return [(None, cur, headers, cur.statusmessage)]
 
 
 @special_command("\\dn", "\\dn[+] [pattern]", "List schemas.")
 def list_schemas(cur, pattern, verbose):
     """
     Returns (title, rows, headers, status)
     """
 
     params = {}
     sql = SQL(
-        """SELECT n.nspname AS "Name", pg_catalog.pg_get_userbyid(n.nspowner) AS "Owner"
+        """SELECT n.nspname AS name, pg_catalog.pg_get_userbyid(n.nspowner) AS owner
                 {verbose}
               FROM pg_catalog.pg_namespace n WHERE n.nspname
                 {pattern}
               ORDER BY 1
               """
     )
 
     if verbose:
         params["verbose"] = SQL(
-            ''', pg_catalog.array_to_string(n.nspacl, E'\\n') AS "Access privileges", pg_catalog.obj_description(n.oid, 'pg_namespace') AS "Description"'''
+            """, pg_catalog.array_to_string(n.nspacl, E'\\n') AS access_privileges, pg_catalog.obj_description(n.oid, 'pg_namespace') AS description"""
         )
     else:
         params["verbose"] = SQL("")
 
     if pattern:
         _, schema = sql_name_pattern(pattern)
         params["pattern"] = SQL("~ {}").format(schema)
     else:
         params["pattern"] = SQL("!~ '^pg_' AND n.nspname <> 'information_schema'")
 
     formatted_query = sql.format(**params)
     log.debug(formatted_query.as_string(cur))
     cur.execute(formatted_query)
     if cur.description:
-        headers = [x.name for x in cur.description]
+        headers = [titleize(x.name) for x in cur.description]
         return [(None, cur, headers, cur.statusmessage)]
 
 
 # https://github.com/postgres/postgres/blob/master/src/bin/psql/describe.c#L5471-L5638
 @special_command("\\dx", "\\dx[+] [pattern]", "List extensions.")
 def list_extensions(cur, pattern, verbose):
     def _find_extensions(cur, pattern):
         sql = SQL(
             """
-            SELECT e.extname, e.oid FROM pg_catalog.pg_extension e
+            SELECT e.extname, e.oid
+            FROM pg_catalog.pg_extension e
             {pattern}
             ORDER BY 1, 2;
         """
         )
 
         params = {}
         if pattern:
@@ -360,25 +362,25 @@
         cur.execute(formatted_query)
         return cur.fetchall()
 
     def _describe_extension(cur, oid):
         sql = SQL(
             """
             SELECT  pg_catalog.pg_describe_object(classid, objid, 0)
-                    AS "Object Description"
+                    AS object_description
             FROM    pg_catalog.pg_depend
             WHERE   refclassid = 'pg_catalog.pg_extension'::pg_catalog.regclass
                     AND refobjid = {}
                     AND deptype = 'e'
             ORDER BY 1"""
         ).format(oid)
         log.debug(sql.as_string(cur))
         cur.execute(sql)
 
-        headers = [x.name for x in cur.description]
+        headers = [titleize(x.name) for x in cur.description]
         return cur, headers, cur.statusmessage
 
     if cur.connection.info.server_version < 90100:
         not_supported = "Server versions below 9.1 do not support extensions."
         cur, headers = [], []
         yield None, cur, None, not_supported
         return
@@ -393,18 +395,18 @@
                 yield title, cur, headers, status
         else:
             yield None, None, None, f"""Did not find any extension named "{pattern}"."""
         return
 
     sql = SQL(
         """
-      SELECT e.extname AS "Name",
-             e.extversion AS "Version",
-             n.nspname AS "Schema",
-             c.description AS "Description"
+      SELECT e.extname AS name,
+             e.extversion AS version,
+             n.nspname AS schema,
+             c.description AS description
       FROM pg_catalog.pg_extension e
            LEFT JOIN pg_catalog.pg_namespace n
              ON n.oid = e.extnamespace
            LEFT JOIN pg_catalog.pg_description c
              ON c.objoid = e.oid
                 AND c.classoid = 'pg_catalog.pg_extension'::pg_catalog.regclass
         {where_clause}
@@ -419,15 +421,15 @@
     else:
         params["where_clause"] = SQL("")
 
     formatted_query = sql.format(**params)
     log.debug(formatted_query.as_string(cur))
     cur.execute(formatted_query)
     if cur.description:
-        headers = [x.name for x in cur.description]
+        headers = [titleize(x.name) for x in cur.description]
         yield None, cur, headers, cur.statusmessage
 
 
 def list_objects(cur, pattern, verbose, relkinds):
     """
     Returns (title, rows, header, status)
 
@@ -439,31 +441,31 @@
     """
     schema_pattern, table_pattern = sql_name_pattern(pattern)
 
     params = {"relkind": relkinds}
     if verbose:
         params["verbose_columns"] = SQL(
             """
-            ,pg_catalog.pg_size_pretty(pg_catalog.pg_table_size(c.oid)) as "Size",
-            pg_catalog.obj_description(c.oid, 'pg_class') as "Description" """
+            ,pg_catalog.pg_size_pretty(pg_catalog.pg_table_size(c.oid)) as size,
+            pg_catalog.obj_description(c.oid, 'pg_class') as description """
         )
     else:
         params["verbose_columns"] = SQL("")
 
     sql = SQL(
-        """SELECT n.nspname as "Schema",
-                    c.relname as "Name",
+        """SELECT n.nspname as schema,
+                    c.relname as name,
                     CASE c.relkind
                       WHEN 'r' THEN 'table' WHEN 'v' THEN 'view'
                       WHEN 'p' THEN 'partitioned table'
                       WHEN 'm' THEN 'materialized view' WHEN 'i' THEN 'index'
                       WHEN 'S' THEN 'sequence' WHEN 's' THEN 'special'
                       WHEN 'f' THEN 'foreign table' END
-                    as "Type",
-                    pg_catalog.pg_get_userbyid(c.relowner) as "Owner"
+                    as type,
+                    pg_catalog.pg_get_userbyid(c.relowner) as owner
                     {verbose_columns}
             FROM    pg_catalog.pg_class c
                     LEFT JOIN pg_catalog.pg_namespace n
                       ON n.oid = c.relnamespace
             WHERE   c.relkind = ANY({relkind})
                 {schema_pattern}
                 {table_pattern}
@@ -488,15 +490,15 @@
         params["table_pattern"] = SQL("")
 
     formatted_query = sql.format(**params)
     log.debug(formatted_query.as_string(cur))
     cur.execute(formatted_query)
 
     if cur.description:
-        headers = [x.name for x in cur.description]
+        headers = [titleize(x.name) for x in cur.description]
         return [(None, cur, headers, cur.statusmessage)]
 
 
 @special_command("\\dt", "\\dt[+] [pattern]", "List tables.")
 def list_tables(cur, pattern, verbose):
     return list_objects(cur, pattern, verbose, ["r", "p", ""])
 
@@ -526,86 +528,86 @@
     if verbose:
         verbose_columns = """
             ,CASE
                  WHEN p.provolatile = 'i' THEN 'immutable'
                  WHEN p.provolatile = 's' THEN 'stable'
                  WHEN p.provolatile = 'v' THEN 'volatile'
             END as "Volatility",
-            pg_catalog.pg_get_userbyid(p.proowner) as "Owner",
+            pg_catalog.pg_get_userbyid(p.proowner) as owner,
           l.lanname as "Language",
           p.prosrc as "Source code",
-          pg_catalog.obj_description(p.oid, 'pg_proc') as "Description" """
+          pg_catalog.obj_description(p.oid, 'pg_proc') as description """
 
         verbose_table = """ LEFT JOIN pg_catalog.pg_language l
                                 ON l.oid = p.prolang"""
     else:
         verbose_columns = verbose_table = ""
 
     if cur.connection.info.server_version >= 110000:
         sql = (
             """
-            SELECT  n.nspname as "Schema",
-                    p.proname as "Name",
+            SELECT  n.nspname as schema,
+                    p.proname as name,
                     pg_catalog.pg_get_function_result(p.oid)
                       as "Result data type",
                     pg_catalog.pg_get_function_arguments(p.oid)
                       as "Argument data types",
                      CASE
                         WHEN p.prokind = 'a' THEN 'agg'
                         WHEN p.prokind = 'w' THEN 'window'
                         WHEN p.prorettype = 'pg_catalog.trigger'::pg_catalog.regtype
                             THEN 'trigger'
                         ELSE 'normal'
-                    END as "Type" """
+                    END as type """
             + verbose_columns
             + """
             FROM    pg_catalog.pg_proc p
                     LEFT JOIN pg_catalog.pg_namespace n ON n.oid = p.pronamespace
                             """
             + verbose_table
             + """
             WHERE  """
         )
     elif cur.connection.info.server_version > 90000:
         sql = (
             """
-            SELECT  n.nspname as "Schema",
-                    p.proname as "Name",
+            SELECT  n.nspname as schema,
+                    p.proname as name,
                     pg_catalog.pg_get_function_result(p.oid)
                       as "Result data type",
                     pg_catalog.pg_get_function_arguments(p.oid)
                       as "Argument data types",
                      CASE
                         WHEN p.proisagg THEN 'agg'
                         WHEN p.proiswindow THEN 'window'
                         WHEN p.prorettype = 'pg_catalog.trigger'::pg_catalog.regtype
                             THEN 'trigger'
                         ELSE 'normal'
-                    END as "Type" """
+                    END as type """
             + verbose_columns
             + """
             FROM    pg_catalog.pg_proc p
                     LEFT JOIN pg_catalog.pg_namespace n ON n.oid = p.pronamespace
                             """
             + verbose_table
             + """
             WHERE  """
         )
     else:
         sql = (
             """
-            SELECT  n.nspname as "Schema",
-                    p.proname as "Name",
+            SELECT  n.nspname as schema,
+                    p.proname as name,
                     pg_catalog.format_type(p.prorettype, NULL) as "Result data type",
                     pg_catalog.oidvectortypes(p.proargtypes) as "Argument data types",
                      CASE
                         WHEN p.proisagg THEN 'agg'
                         WHEN p.prorettype = 'pg_catalog.trigger'::pg_catalog.regtype THEN 'trigger'
                         ELSE 'normal'
-                    END as "Type" """
+                    END as type """
             + verbose_columns
             + """
             FROM    pg_catalog.pg_proc p
                     LEFT JOIN pg_catalog.pg_namespace n ON n.oid = p.pronamespace
                             """
             + verbose_table
             + """
@@ -631,46 +633,46 @@
 
     sql += " ORDER BY 1, 2, 4"
 
     log.debug("%s, %s", sql, params)
     cur.execute(sql, params)
 
     if cur.description:
-        headers = [x.name for x in cur.description]
+        headers = [titleize(x.name) for x in cur.description]
         return [(None, cur, headers, cur.statusmessage)]
 
 
 @special_command("\\dT", "\\dT[S+] [pattern]", "List data types")
 def list_datatypes(cur, pattern, verbose):
-    sql = """SELECT n.nspname as "Schema",
-                    pg_catalog.format_type(t.oid, NULL) AS "Name", """
+    sql = """SELECT n.nspname as schema,
+                    pg_catalog.format_type(t.oid, NULL) AS name, """
 
     if verbose:
-        sql += r''' t.typname AS "Internal name",
+        sql += r""" t.typname AS internal_name,
                     CASE
                         WHEN t.typrelid != 0
                             THEN CAST('tuple' AS pg_catalog.text)
                         WHEN t.typlen < 0
                             THEN CAST('var' AS pg_catalog.text)
                         ELSE CAST(t.typlen AS pg_catalog.text)
-                    END AS "Size",
+                    END AS size,
                     pg_catalog.array_to_string(
                         ARRAY(
                               SELECT e.enumlabel
                               FROM pg_catalog.pg_enum e
                               WHERE e.enumtypid = t.oid
                               ORDER BY e.enumsortorder
-                          ), E'\n') AS "Elements",
+                          ), E'\n') AS elements,
                     pg_catalog.array_to_string(t.typacl, E'\n')
-                        AS "Access privileges",
+                        AS access_privileges,
                     pg_catalog.obj_description(t.oid, 'pg_type')
-                        AS "Description"'''
+                        AS description"""
     else:
         sql += """  pg_catalog.obj_description(t.oid, 'pg_type')
-                        as "Description" """
+                        as description """
 
     if cur.connection.info.server_version > 90000:
         sql += """  FROM    pg_catalog.pg_type t
                             LEFT JOIN pg_catalog.pg_namespace n
                               ON n.oid = t.typnamespace
                     WHERE   (t.typrelid = 0 OR
                               ( SELECT c.relkind = 'c'
@@ -708,53 +710,53 @@
         sql += """ AND n.nspname <> 'pg_catalog'
                    AND n.nspname <> 'information_schema' """
 
     sql += " ORDER BY 1, 2"
     log.debug("%s, %s", sql, params)
     cur.execute(sql, params)
     if cur.description:
-        headers = [x.name for x in cur.description]
+        headers = [titleize(x.name) for x in cur.description]
         return [(None, cur, headers, cur.statusmessage)]
 
 
 @special_command("\\dD", "\\dD[+] [pattern]", "List or describe domains.")
 def list_domains(cur, pattern, verbose):
     if verbose:
-        extra_cols = r''',
-               pg_catalog.array_to_string(t.typacl, E'\n') AS "Access privileges",
-               d.description as "Description"'''
+        extra_cols = r""",
+               pg_catalog.array_to_string(t.typacl, E'\n') AS access_privileges,
+               d.description as description"""
         extra_joins = """
            LEFT JOIN pg_catalog.pg_description d ON d.classoid = t.tableoid
                                                 AND d.objoid = t.oid AND d.objsubid = 0"""
     else:
         extra_cols = extra_joins = ""
 
     sql = f"""\
-        SELECT n.nspname AS "Schema",
-               t.typname AS "Name",
-               pg_catalog.format_type(t.typbasetype, t.typtypmod) AS "Type",
+        SELECT n.nspname AS schema,
+               t.typname AS name,
+               pg_catalog.format_type(t.typbasetype, t.typtypmod) as type,
                pg_catalog.ltrim((COALESCE((SELECT (' collate ' || c.collname)
                                            FROM pg_catalog.pg_collation AS c,
                                                 pg_catalog.pg_type AS bt
                                            WHERE c.oid = t.typcollation
                                              AND bt.oid = t.typbasetype
                                              AND t.typcollation <> bt.typcollation) , '')
                                 || CASE
                                      WHEN t.typnotnull
                                        THEN ' not null'
                                      ELSE ''
                                    END) || CASE
                                              WHEN t.typdefault IS NOT NULL
                                                THEN(' default ' || t.typdefault)
                                              ELSE ''
-                                           END) AS "Modifier",
+                                           END) AS modifier,
                pg_catalog.array_to_string(ARRAY(
                  SELECT pg_catalog.pg_get_constraintdef(r.oid, TRUE)
                  FROM pg_catalog.pg_constraint AS r
-                 WHERE t.oid = r.contypid), ' ') AS "Check"{extra_cols}
+                 WHERE t.oid = r.contypid), ' ') AS check {extra_cols}
         FROM pg_catalog.pg_type AS t
            LEFT JOIN pg_catalog.pg_namespace AS n ON n.oid = t.typnamespace{extra_joins}
         WHERE t.typtype = 'd' """
 
     schema_pattern, name_pattern = sql_name_pattern(pattern)
     params = {}
     if schema_pattern or name_pattern:
@@ -770,15 +772,15 @@
           AND (n.nspname <> 'information_schema')
           AND pg_catalog.pg_type_is_visible(t.oid)"""
 
     sql += " ORDER BY 1, 2"
     log.debug("%s, %s", sql, params)
     cur.execute(sql, params)
     if cur.description:
-        headers = [x.name for x in cur.description]
+        headers = [titleize(x.name) for x in cur.description]
         return [(None, cur, headers, cur.statusmessage)]
 
 
 @special_command("\\dF", "\\dF[+] [pattern]", "List text search configurations.")
 def list_text_search_configurations(cur, pattern, verbose):
     def _find_text_search_configs(cur, pattern):
         sql = """
@@ -807,35 +809,35 @@
 
     def _fetch_oid_details(cur, oid):
         params = {"oid": oid}
         sql = """
             SELECT
               (SELECT t.alias
                FROM pg_catalog.ts_token_type(c.cfgparser) AS t
-               WHERE t.tokid = m.maptokentype ) AS "Token",
+               WHERE t.tokid = m.maptokentype ) AS token,
                    pg_catalog.btrim(ARRAY
                                       (SELECT mm.mapdict::pg_catalog.regdictionary
                                        FROM pg_catalog.pg_ts_config_map AS mm
                                        WHERE mm.mapcfg = m.mapcfg
                                          AND mm.maptokentype = m.maptokentype
-                                       ORDER BY mapcfg, maptokentype, mapseqno) :: pg_catalog.text, '{}') AS "Dictionaries"
+                                       ORDER BY mapcfg, maptokentype, mapseqno) :: pg_catalog.text, '{}') AS dictionaries
             FROM pg_catalog.pg_ts_config AS c,
                  pg_catalog.pg_ts_config_map AS m
             WHERE c.oid = %(oid)s
               AND m.mapcfg = c.oid
             GROUP BY m.mapcfg,
                      m.maptokentype,
                      c.cfgparser
             ORDER BY 1;
         """
 
         log.debug("%s, %s", sql, params)
         cur.execute(sql, params)
 
-        headers = [x.name for x in cur.description]
+        headers = [titleize(x.name) for x in cur.description]
         return cur, headers, cur.statusmessage
 
     if cur.connection.info.server_version < 80300:
         not_supported = "Server versions below 8.3 do not support full text search."
         cur, headers = [], []
         yield None, cur, None, not_supported
         return
@@ -847,38 +849,41 @@
             for oid, cfgname, nspname, prsname, pnspname in configs:
                 extension = f'''\nText search configuration "{nspname}.{cfgname}"'''
                 parser = f'''\nParser: "{pnspname}.{prsname}"'''
                 title = extension + parser
                 cur, headers, status = _fetch_oid_details(cur, oid)
                 yield title, cur, headers, status
         else:
-            yield None, None, None, 'Did not find any results for pattern "{}".'.format(
-                pattern
+            yield (
+                None,
+                None,
+                None,
+                'Did not find any results for pattern "{}".'.format(pattern),
             )
         return
 
     sql = """
-        SELECT n.nspname AS "Schema",
-               c.cfgname AS "Name",
-               pg_catalog.obj_description(c.oid, 'pg_ts_config') AS "Description"
+        SELECT n.nspname AS schema,
+               c.cfgname AS name,
+               pg_catalog.obj_description(c.oid, 'pg_ts_config') AS description
         FROM pg_catalog.pg_ts_config c
         LEFT JOIN pg_catalog.pg_namespace n ON n.oid = c.cfgnamespace
         """
 
     params = {}
     if pattern:
         _, schema = sql_name_pattern(pattern)
         sql += "WHERE c.cfgname ~ %(cfgname)s"
         params["cfgname"] = schema
 
     sql += " ORDER BY 1, 2"
     log.debug("%s, %s", sql, params)
     cur.execute(sql, params)
     if cur.description:
-        headers = [x.name for x in cur.description]
+        headers = [titleize(x.name) for x in cur.description]
         yield None, cur, headers, cur.statusmessage
 
 
 @special_command(
     "describe", "DESCRIBE [pattern]", "", hidden=True, case_sensitive=False
 )
 @special_command(
@@ -976,15 +981,15 @@
                     c.relkind,
                     c.relhasindex,
                     c.relhasrules,
                     c.relhastriggers,
                     c.relhasoids,
                     {suffix},
                     c.reltablespace,
-                    0 AS reloftype,
+                    '' AS reloftype,
                     'p' AS relpersistence,
                     false as relispartition
                  FROM pg_catalog.pg_class c
                  LEFT JOIN pg_catalog.pg_class tc ON (c.reltoastrelid = tc.oid)
                  WHERE c.oid = '{oid}'"""
 
     else:
@@ -992,15 +997,15 @@
                     c.relkind,
                     c.relhasindex,
                     c.relhasrules,
                     c.reltriggers > 0 AS relhastriggers,
                     c.relhasoids,
                     {suffix},
                     c.reltablespace,
-                    0 AS reloftype,
+                    '' AS reloftype,
                     'p' AS relpersistence,
                     false as relispartition
                  FROM pg_catalog.pg_class c
                  LEFT JOIN pg_catalog.pg_class tc ON (c.reltoastrelid = tc.oid)
                  WHERE c.oid = '{oid}'"""
 
     # Create a namedtuple called tableinfo and match what's in describe.c
@@ -1060,16 +1065,16 @@
         sql += ",\n  ''::pg_catalog.char AS attgenerated"
     att_cols["attgenerated"] = cols
     cols += 1
     # index, or partitioned index
     if tableinfo.relkind == "i" or tableinfo.relkind == "I":
         if cur.connection.info.server_version >= 110000:
             sql += (
-                f",\n CASE WHEN a.attnum <= (SELECT i.indnkeyatts FROM pg_catalog.pg_index i "
-                "WHERE i.indexrelid = '{oid}') THEN 'yes' ELSE 'no' END AS is_key"
+                ",\n CASE WHEN a.attnum <= (SELECT i.indnkeyatts FROM pg_catalog.pg_index i "
+                f"WHERE i.indexrelid = '{oid}') THEN 'yes' ELSE 'no' END AS is_key"
             )
             att_cols["indexkey"] = cols
             cols += 1
         sql += ",\n pg_catalog.pg_get_indexdef(a.attrelid, a.attnum, TRUE) AS indexdef"
     else:
         sql += """,\n NULL AS indexdef"""
     att_cols["indexdef"] = cols
@@ -1433,15 +1438,15 @@
 
             log.debug(sql)
             result = cur.execute(sql)
 
             if cur.rowcount > 0:
                 status.append("Indexes:\n")
             for row in cur:
-                # /* untranslated index name */
+                # /* untranslated indextname */
                 status.append(f'''    "{row[0]}"''')
 
                 # /* If exclusion constraint, print the constraintdef */
                 if row[7] == "x":
                     status.append(" ")
                     status.append(row[6])
                 else:
@@ -1911,15 +1916,15 @@
     (foid,) = cur.fetchone()
 
     params = {"foid": foid}
     sql = "SELECT pg_catalog.pg_get_functiondef(%(foid)s) as source"
     log.debug("%s, %s", sql, params)
     cur.execute(sql, params)
     if cur.description:
-        headers = [x.name for x in cur.description]
+        headers = [titleize(x.name) for x in cur.description]
         if verbose:
             (source,) = cur.fetchone()
             rows = _FakeCursor()
             rown = None
             for row in source.splitlines():
                 if rown is None:
                     if row.startswith("AS "):
@@ -1942,18 +1947,18 @@
 
 
 @special_command("\\dE", "\\dE[+] [pattern]", "List foreign tables.", aliases=())
 def list_foreign_tables(cur, pattern, verbose):
     params = {}
     query = SQL(
         """
-        SELECT n.nspname as "Schema",
-        c.relname as "Name",
-        CASE c.relkind WHEN 'r' THEN 'table' WHEN 'v' THEN 'view' WHEN 'm' THEN 'materialized view' WHEN 'i' THEN 'index' WHEN 'S' THEN 'sequence' WHEN 's' THEN 'special' WHEN 'f' THEN 'foreign table' WHEN 'p' THEN 'table' WHEN 'I' THEN 'index' END as "Type",
-        pg_catalog.pg_get_userbyid(c.relowner) as "Owner"
+        SELECT n.nspname as schema,
+        c.relname as name,
+        CASE c.relkind WHEN 'r' THEN 'table' WHEN 'v' THEN 'view' WHEN 'm' THEN 'materialized view' WHEN 'i' THEN 'index' WHEN 'S' THEN 'sequence' WHEN 's' THEN 'special' WHEN 'f' THEN 'foreign table' WHEN 'p' THEN 'table' WHEN 'I' THEN 'index' END as type,
+        pg_catalog.pg_get_userbyid(c.relowner) as owner
         {verbose_cols}
         FROM pg_catalog.pg_class c
             LEFT JOIN pg_catalog.pg_namespace n ON n.oid = c.relnamespace
         WHERE c.relkind IN ('f','')
             AND n.nspname <> 'pg_catalog'
             AND n.nspname <> 'information_schema'
             AND n.nspname !~ '^pg_toast'
@@ -1962,16 +1967,16 @@
         ORDER BY 1,2;
         """
     )
 
     if verbose:
         params["verbose_cols"] = SQL(
             """
-            , pg_catalog.pg_size_pretty(pg_catalog.pg_table_size(c.oid)) as "Size",
-            pg_catalog.obj_description(c.oid, 'pg_class') as "Description" """
+            , pg_catalog.pg_size_pretty(pg_catalog.pg_table_size(c.oid)) as size,
+            pg_catalog.obj_description(c.oid, 'pg_class') as description """
         )
     else:
         params["verbose_cols"] = SQL("")
 
     if pattern:
         _, tbl_name = sql_name_pattern(pattern)
         params["filter"] = SQL(" AND c.relname OPERATOR(pg_catalog.~) {} ").format(
@@ -1980,11 +1985,15 @@
     else:
         params["filter"] = SQL("")
 
     formatted_query = query.format(**params)
     log.debug(formatted_query.as_string(cur))
     cur.execute(formatted_query)
     if cur.description:
-        headers = [x.name for x in cur.description]
+        headers = [titleize(x.name) for x in cur.description]
         return [(None, cur, headers, cur.statusmessage)]
     else:
         return [(None, None, None, cur.statusmessage)]
+
+
+def titleize(column):
+    return column[0].capitalize() + " ".join(c for c in column[1:].split("_"))
```

### Comparing `pgspecial-2.1.1/pgspecial/help/commands.py` & `pgspecial-2.1.2/pgspecial/help/commands.py`

 * *Files identical despite different names*

### Comparing `pgspecial-2.1.1/pgspecial/iocommands.py` & `pgspecial-2.1.2/pgspecial/iocommands.py`

 * *Files identical despite different names*

### Comparing `pgspecial-2.1.1/pgspecial/main.py` & `pgspecial-2.1.2/pgspecial/main.py`

 * *Files identical despite different names*

### Comparing `pgspecial-2.1.1/pgspecial/namedqueries.py` & `pgspecial-2.1.2/pgspecial/namedqueries.py`

 * *Files identical despite different names*

### Comparing `pgspecial-2.1.1/pgspecial.egg-info/PKG-INFO` & `pgspecial-2.1.2/pgspecial.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgspecial
-Version: 2.1.1
+Version: 2.1.2
 Summary: Meta-commands handler for Postgres Database.
 Home-page: https://www.dbcli.com
 Author: Pgcli Core Team
 Author-email: pgcli-dev@googlegroups.com
 License: LICENSE.txt
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pgspecial-2.1.1/pgspecial.egg-info/SOURCES.txt` & `pgspecial-2.1.2/pgspecial.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pgspecial-2.1.1/scripts/README.rst` & `pgspecial-2.1.2/scripts/README.rst`

 * *Files identical despite different names*

### Comparing `pgspecial-2.1.1/scripts/docparser.py` & `pgspecial-2.1.2/scripts/docparser.py`

 * *Files identical despite different names*

### Comparing `pgspecial-2.1.1/setup.py` & `pgspecial-2.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `pgspecial-2.1.1/tests/conftest.py` & `pgspecial-2.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pgspecial-2.1.1/tests/dbutils.py` & `pgspecial-2.1.2/tests/dbutils.py`

 * *Files identical despite different names*

### Comparing `pgspecial-2.1.1/tests/test_internal.py` & `pgspecial-2.1.2/tests/test_internal.py`

 * *Files identical despite different names*

### Comparing `pgspecial-2.1.1/tests/test_named_queries.py` & `pgspecial-2.1.2/tests/test_named_queries.py`

 * *Files identical despite different names*

### Comparing `pgspecial-2.1.1/tests/test_specials.py` & `pgspecial-2.1.2/tests/test_specials.py`

 * *Files 0% similar despite different names*

```diff
@@ -627,15 +627,15 @@
     title = '\nObjects in extension "plpgsql"'
     row = [
         ("function plpgsql_call_handler()",),
         ("function plpgsql_inline_handler(internal)",),
         ("function plpgsql_validator(oid)",),
         ("language plpgsql",),
     ]
-    headers = ["Object Description"]
+    headers = ["Object description"]
     status = "SELECT %s" % len(row)
     expected = [title, row, headers, status]
     assert results == expected
 
 
 @dbtest
 def test_slash_dT(executor):
@@ -1042,15 +1042,15 @@
         (
             "CREATE OR REPLACE FUNCTION public.func1()\n"
             " RETURNS integer\n"
             " LANGUAGE sql\n"
             "AS $function$select 1$function$\n",
         ),
     ]
-    headers = ["source"]
+    headers = ["Source"]
     status = None
     expected = [title, rows, headers, status]
     assert results == expected
 
 
 @dbtest
 def test_slash_sf_unknown(executor):
@@ -1070,15 +1070,15 @@
         (
             "CREATE OR REPLACE FUNCTION public.func1()\n"
             " RETURNS integer\n"
             " LANGUAGE sql\n"
             "AS $function$select 1$function$\n",
         ),
     ]
-    headers = ["source"]
+    headers = ["Source"]
     status = None
     expected = [title, rows, headers, status]
     assert results == expected
 
 
 @dbtest
 def test_slash_sf_verbose(executor):
@@ -1088,15 +1088,15 @@
         (
             "        CREATE OR REPLACE FUNCTION schema1.s1_func1()\n"
             "         RETURNS integer\n"
             "         LANGUAGE sql\n"
             "1       AS $function$select 2$function$\n",
         ),
     ]
-    headers = ["source"]
+    headers = ["Source"]
     status = None
     expected = [title, rows, headers, status]
     assert results == expected
 
 
 @fdw_test
 def test_slash_dE(executor):
```

