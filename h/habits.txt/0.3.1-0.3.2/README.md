# Comparing `tmp/habits_txt-0.3.1.tar.gz` & `tmp/habits_txt-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "habits_txt-0.3.1.tar", max compression
+gzip compressed data, was "habits_txt-0.3.2.tar", max compression
```

## Comparing `habits_txt-0.3.1.tar` & `habits_txt-0.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     3109 2024-05-14 20:37:42.341037 habits_txt-0.3.1/README.md
--rwxr-xr-x   0        0        0      788 2024-05-15 17:43:14.132064 habits_txt-0.3.1/bin/hbtxt.py
--rw-r--r--   0        0        0        0 2024-05-14 20:25:35.415585 habits_txt-0.3.1/habits_txt/__init__.py
--rw-r--r--   0        0        0    13971 2024-05-15 17:43:14.132064 habits_txt-0.3.1/habits_txt/builder.py
--rw-r--r--   0        0        0     7593 2024-05-15 17:43:14.132064 habits_txt-0.3.1/habits_txt/cli.py
--rw-r--r--   0        0        0     2154 2024-05-14 20:25:35.415585 habits_txt-0.3.1/habits_txt/config.py
--rw-r--r--   0        0        0      224 2024-05-14 20:25:35.415585 habits_txt-0.3.1/habits_txt/defaults.py
--rw-r--r--   0        0        0     2323 2024-05-15 17:43:14.132064 habits_txt-0.3.1/habits_txt/directives.py
--rw-r--r--   0        0        0      380 2024-05-14 20:25:35.415585 habits_txt-0.3.1/habits_txt/exceptions.py
--rw-r--r--   0        0        0     7655 2024-05-15 17:43:14.132064 habits_txt-0.3.1/habits_txt/journal.py
--rw-r--r--   0        0        0     2940 2024-05-15 17:43:14.132064 habits_txt-0.3.1/habits_txt/models.py
--rw-r--r--   0        0        0     9037 2024-05-15 17:43:14.132064 habits_txt-0.3.1/habits_txt/parser.py
--rw-r--r--   0        0        0      952 2024-05-14 20:25:35.415585 habits_txt-0.3.1/habits_txt/records_query.py
--rw-r--r--   0        0        0      627 2024-05-15 17:45:51.087127 habits_txt-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3482 1970-01-01 00:00:00.000000 habits_txt-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     3109 2024-05-14 20:37:42.341037 habits_txt-0.3.2/README.md
+-rwxr-xr-x   0        0        0      788 2024-05-15 17:43:14.132064 habits_txt-0.3.2/bin/hbtxt.py
+-rw-r--r--   0        0        0        0 2024-05-14 20:25:35.415585 habits_txt-0.3.2/habits_txt/__init__.py
+-rw-r--r--   0        0        0    13971 2024-05-15 17:43:14.132064 habits_txt-0.3.2/habits_txt/builder.py
+-rw-r--r--   0        0        0     7842 2024-05-15 17:57:35.675452 habits_txt-0.3.2/habits_txt/cli.py
+-rw-r--r--   0        0        0     2154 2024-05-14 20:25:35.415585 habits_txt-0.3.2/habits_txt/config.py
+-rw-r--r--   0        0        0      224 2024-05-14 20:25:35.415585 habits_txt-0.3.2/habits_txt/defaults.py
+-rw-r--r--   0        0        0     2323 2024-05-15 17:43:14.132064 habits_txt-0.3.2/habits_txt/directives.py
+-rw-r--r--   0        0        0      380 2024-05-14 20:25:35.415585 habits_txt-0.3.2/habits_txt/exceptions.py
+-rw-r--r--   0        0        0     8107 2024-05-15 17:57:35.675452 habits_txt-0.3.2/habits_txt/journal.py
+-rw-r--r--   0        0        0     2940 2024-05-15 17:43:14.132064 habits_txt-0.3.2/habits_txt/models.py
+-rw-r--r--   0        0        0     9037 2024-05-15 17:43:14.132064 habits_txt-0.3.2/habits_txt/parser.py
+-rw-r--r--   0        0        0      952 2024-05-14 20:25:35.415585 habits_txt-0.3.2/habits_txt/records_query.py
+-rw-r--r--   0        0        0      627 2024-05-15 17:57:35.675452 habits_txt-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3482 1970-01-01 00:00:00.000000 habits_txt-0.3.2/PKG-INFO
```

### Comparing `habits_txt-0.3.1/README.md` & `habits_txt-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `habits_txt-0.3.1/bin/hbtxt.py` & `habits_txt-0.3.2/bin/hbtxt.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.3.1/habits_txt/builder.py` & `habits_txt-0.3.2/habits_txt/builder.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.3.1/habits_txt/cli.py` & `habits_txt-0.3.2/habits_txt/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,18 @@
     "--write-bottom",
     is_flag=True,
     help="Write output to the bottom of the journal file",
 )
 def fill(file, date, interactive, write_top, write_bottom):
     """
     Fill habits on a given date using FILE.
+
+    Interactive mode allows you to be prompted to fill each habit.
+    If you want to skip a habit while in interactive mode, just press 's'.
+    If you want to skip a habit but still append it to the journal (for manual filling later), press 'a'.
     """
     records = journal_.fill_day(
         file.name,
         date,
         interactive,
     )
     if records:
```

### Comparing `habits_txt-0.3.1/habits_txt/config.py` & `habits_txt-0.3.2/habits_txt/config.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.3.1/habits_txt/directives.py` & `habits_txt-0.3.2/habits_txt/directives.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.3.1/habits_txt/journal.py` & `habits_txt-0.3.2/habits_txt/journal.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,28 +75,39 @@
             most_recent_and_completed_record = (
                 records_query.get_most_recent_and_completed_record(habit, habit_records)
             )
             next_due_date = habit.frequency.get_next_date(
                 most_recent_and_completed_record.date
             )
         if next_due_date <= date:
+            append = True
             if interactive:
                 value_is_valid = False
                 parsed_value = None
                 while not value_is_valid:
                     value = input(f"{habit.name} ({next_due_date}): ")
+                    if value == "s":
+                        append = False
+                        break
+                    elif value == "a":
+                        break
                     try:
                         parsed_value = parser.parse_value_str(value)
                         value_is_valid = True
-                    except exceptions.ParseError as e:
-                        logging.error(e)
+                    except exceptions.ParseError:
+                        logging.error(
+                            f"Value must be a {"number" if habit.is_measurable else "boolean"}.\n"
+                            f"(or 's' to skip, or 'a' to append to the journal but fill manually later)"
+                        )
                 record = models.HabitRecord(date, habit.name, parsed_value)
             else:
                 record = models.HabitRecord(date, habit.name, None)
-            records_fill.append(record)
+
+            if append:
+                records_fill.append(record)
 
     return records_fill
 
 
 def _filter_state(
     journal_file: str,
     start_date: dt.date | None,
```

### Comparing `habits_txt-0.3.1/habits_txt/models.py` & `habits_txt-0.3.2/habits_txt/models.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.3.1/habits_txt/parser.py` & `habits_txt-0.3.2/habits_txt/parser.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.3.1/habits_txt/records_query.py` & `habits_txt-0.3.2/habits_txt/records_query.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.3.1/pyproject.toml` & `habits_txt-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "habits.txt"
-version = "0.3.1"
+version = "0.3.2"
 description = ""
 authors = ["estebanthi <esteban.thilliez@gmail.com>"]
 readme = "README.md"
 packages = [
     {include = "habits_txt"}, {include = "bin"}
 ]
```

### Comparing `habits_txt-0.3.1/PKG-INFO` & `habits_txt-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: habits.txt
-Version: 0.3.1
+Version: 0.3.2
 Summary: 
 Author: estebanthi
 Author-email: esteban.thilliez@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
```

