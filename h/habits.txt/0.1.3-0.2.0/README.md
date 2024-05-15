# Comparing `tmp/habits_txt-0.1.3.tar.gz` & `tmp/habits_txt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "habits_txt-0.1.3.tar", max compression
+gzip compressed data, was "habits_txt-0.2.0.tar", max compression
```

## Comparing `habits_txt-0.1.3.tar` & `habits_txt-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     2165 2024-05-14 18:39:14.295454 habits_txt-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-05-14 18:39:14.295454 habits_txt-0.1.3/habits_txt/__init__.py
--rw-r--r--   0        0        0    10111 2024-05-14 18:39:14.295454 habits_txt-0.1.3/habits_txt/builder.py
--rw-r--r--   0        0        0     3419 2024-05-11 15:56:18.089263 habits_txt-0.1.3/habits_txt/cli.py
--rw-r--r--   0        0        0      145 2024-05-14 18:39:14.295454 habits_txt-0.1.3/habits_txt/defaults.py
--rw-r--r--   0        0        0     2030 2024-05-14 18:39:14.295454 habits_txt-0.1.3/habits_txt/directives.py
--rw-r--r--   0        0        0      380 2024-05-14 18:39:14.295454 habits_txt-0.1.3/habits_txt/exceptions.py
--rw-r--r--   0        0        0     3768 2024-05-14 18:39:14.295454 habits_txt-0.1.3/habits_txt/journal.py
--rw-r--r--   0        0        0     1855 2024-05-14 18:39:14.295454 habits_txt-0.1.3/habits_txt/models.py
--rw-r--r--   0        0        0     9233 2024-05-14 18:39:14.295454 habits_txt-0.1.3/habits_txt/parser.py
--rw-r--r--   0        0        0      952 2024-05-14 18:39:14.295454 habits_txt-0.1.3/habits_txt/records_query.py
--rw-r--r--   0        0        0      243 2024-05-11 15:56:18.089263 habits_txt-0.1.3/main.py
--rw-r--r--   0        0        0      637 2024-05-14 18:39:44.895715 habits_txt-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2558 1970-01-01 00:00:00.000000 habits_txt-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2476 2024-05-14 20:25:35.415585 habits_txt-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-14 20:25:35.415585 habits_txt-0.2.0/habits_txt/__init__.py
+-rw-r--r--   0        0        0    10111 2024-05-14 20:25:35.415585 habits_txt-0.2.0/habits_txt/builder.py
+-rw-r--r--   0        0        0     3343 2024-05-14 20:25:35.415585 habits_txt-0.2.0/habits_txt/cli.py
+-rw-r--r--   0        0        0     2154 2024-05-14 20:25:35.415585 habits_txt-0.2.0/habits_txt/config.py
+-rw-r--r--   0        0        0      224 2024-05-14 20:25:35.415585 habits_txt-0.2.0/habits_txt/defaults.py
+-rw-r--r--   0        0        0     2030 2024-05-14 20:25:35.415585 habits_txt-0.2.0/habits_txt/directives.py
+-rw-r--r--   0        0        0      380 2024-05-14 20:25:35.415585 habits_txt-0.2.0/habits_txt/exceptions.py
+-rw-r--r--   0        0        0     3768 2024-05-14 20:25:35.415585 habits_txt-0.2.0/habits_txt/journal.py
+-rw-r--r--   0        0        0     1855 2024-05-14 20:25:35.415585 habits_txt-0.2.0/habits_txt/models.py
+-rw-r--r--   0        0        0     9233 2024-05-14 20:25:35.415585 habits_txt-0.2.0/habits_txt/parser.py
+-rw-r--r--   0        0        0      952 2024-05-14 20:25:35.415585 habits_txt-0.2.0/habits_txt/records_query.py
+-rw-r--r--   0        0        0      585 2024-05-14 20:25:35.415585 habits_txt-0.2.0/main.py
+-rw-r--r--   0        0        0      654 2024-05-14 20:26:18.389436 habits_txt-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2907 1970-01-01 00:00:00.000000 habits_txt-0.2.0/PKG-INFO
```

### Comparing `habits_txt-0.1.3/README.md` & `habits_txt-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,27 @@
 # habits.txt
 
+[![PyPI version](https://badge.fury.io/py/habits.txt.svg)](https://badge.fury.io/py/habits.txt)
+
 habits.txt is a plain text habit tracker.
 
+[Installation](#installation) | [Concepts](#concepts) | [Format](#format) | [Directives](#directives)
+
+## Installation
+
+```bash
+pip install habits.txt
+```
+
+You can then use the CLI with:
+
+```bash
+hbtxt --help
+```
+
 ## Concepts
 
 ### Time-bound
 
 A habit is time-bound. It has a start date, and eventually an end date.
 It means with habits.txt, you can track habits for a specific period of time. When you want to stop tracking a habit, you can just stop tracking it.
```

### Comparing `habits_txt-0.1.3/habits_txt/builder.py` & `habits_txt-0.2.0/habits_txt/builder.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.1.3/habits_txt/cli.py` & `habits_txt-0.2.0/habits_txt/journal.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,113 +1,120 @@
-import argparse
 import datetime as dt
 import logging
+import typing
 
+import habits_txt.builder as builder
 import habits_txt.defaults as defaults
-import habits_txt.journal as journal
+import habits_txt.exceptions as exceptions
+import habits_txt.models as models
+import habits_txt.parser as parser
+import habits_txt.records_query as records_query
 
 
-def parse_args(args: list[str]) -> argparse.Namespace:
+def get_state_at_date(
+    journal_file: str, date: dt.date
+) -> typing.Tuple[set[models.Habit], list[models.HabitRecord]]:
     """
-    Parse arguments.
+    Get the state of the habits at a given date.
 
-    :param args: List of arguments.
-    :return: Parsed arguments.
-    """
-    parser = argparse.ArgumentParser()
-
-    command_subparsers = parser.add_subparsers(dest="command")
-
-    fill_parser = command_subparsers.add_parser(
-        "fill",
-        help="Fill habits on a given date",
-        description="Fill habits on a given date",
-    )
-    fill_parser.add_argument(
-        "--date",
-        help="Date to use (defaults to today)",
-        default=dt.date.today().strftime(defaults.DATE_FMT),
-    )
-    fill_parser.add_argument(
-        "--interactive", help="Interactive mode", action="store_true"
-    )
-    fill_parser.add_argument(
-        "--write-top",
-        help="Write output to the top of the journal file",
-        action="store_true",
-    )
-    fill_parser.add_argument(
-        "--write-bottom",
-        help="Write output to the bottom of the journal file",
-        action="store_true",
-    )
-
-    filter_parser = command_subparsers.add_parser(
-        "filter", help="Filter habit records", description="Filter habit records"
-    )
-    filter_parser.add_argument("--start", help="Start date", default=None)
-    filter_parser.add_argument(
-        "--end", help="End date", default=dt.date.today().strftime(defaults.DATE_FMT)
-    )
-    filter_parser.add_argument("--habit", help="Habit to filter", default=None)
-
-    parser.add_argument("file", help="Journal file to read")
-    return parser.parse_args(args)
-
-
-def run_command(args: argparse.Namespace):
-    """
-    Run a command.
-
-    :param args: Parsed arguments.
-    """
-
-    def run_fill():
-        records = journal.fill_day(
-            args.file,
-            dt.datetime.strptime(args.date, defaults.DATE_FMT).date(),
-            args.interactive,
-        )
-        if records:
-            records_str = (
-                "\n".join([str(record) for record in records]) if records else ""
-            )
-            output(args.file, records_str, args.write_top, args.write_bottom)
+    :param journal_file: Path to the journal file.
+    :param date: Date to check.
+    :return: Tracked habits, records.
+    """
+    directives, parse_errors = parser.parse_file(journal_file)
+    _log_errors(parse_errors)
+    try:
+        tracked_habits, records = builder.get_state_at_date(directives, date)
+    except exceptions.ConsistencyError as e:
+        logging.error(e)
+        logging.error("Cannot continue due to consistency errors")
+        exit(1)
 
-    if not args.command:
-        run_fill()
-    if args.command == "fill":
-        run_fill()
-    if args.command == "filter":
-        start_date = (
-            dt.datetime.strptime(args.start, defaults.DATE_FMT).date()
-            if args.start
-            else None
-        )
-        end_date = dt.datetime.strptime(args.end, defaults.DATE_FMT).date()
-        records = journal.filter(args.file, start_date, end_date, args.habit)
-        if records:
-            records_str = "\n".join([str(record) for record in records])
-            logging.info(records_str)
-        else:
-            logging.info("No records found")
+    return tracked_habits, records
+
+
+def _log_errors(errors: list[str]):
+    """
+    Log errors.
+
+    :param errors: List of errors.
+    """
+    for error in errors:
+        logging.error(error)
 
 
-def output(file: str, string: str, write_top: bool, write_bottom: bool):
+def fill_day(
+    journal_file: str, date: dt.date, interactive: bool = False
+) -> list[models.HabitRecord]:
     """
-    Output a string to the console or a file.
+    Fill a day in the journal.
 
-    :param file: File to write to.
-    :param string: String to write.
-    :param write_top: Write to the top of the file.
-    :param write_bottom: Write to the bottom of the file.
-    """
-    if write_top:
-        with open(file, "r") as f:
-            content = f.read()
-        with open(file, "w") as f:
-            f.write(string + "\n\n" + content)
-    elif write_bottom:
-        with open(file, "a") as f:
-            f.write("\n" + string + "\n")
-    else:
-        print(string)
+    :param journal_file: Path to the journal file.
+    :param date: Date to fill.
+    :param interactive: Interactive mode.
+    :return: Journal file.
+    """
+    records_fill = []
+    tracked_habits, records = get_state_at_date(journal_file, date)
+    if not tracked_habits:
+        logging.info(f"{defaults.COMMENT_CHAR} No habits tracked")
+        return []
+    for habit in tracked_habits:
+        habit_records = [
+            record for record in records if record.habit_name == habit.name
+        ]
+        if not habit_records:
+            # because we can have a record directive the day we start to track a habit
+            next_due_date = habit.frequency.get_next_date(date - dt.timedelta(days=1))
+        else:
+            most_recent_and_completed_record = (
+                records_query.get_most_recent_and_completed_record(habit, habit_records)
+            )
+            next_due_date = habit.frequency.get_next_date(
+                most_recent_and_completed_record.date
+            )
+        if next_due_date <= date:
+            if interactive:
+                value_is_valid = False
+                parsed_value = None
+                while not value_is_valid:
+                    value = input(f"{habit.name} ({next_due_date}): ")
+                    try:
+                        parsed_value = parser.parse_value_str(value)
+                        value_is_valid = True
+                    except exceptions.ParseError as e:
+                        logging.error(e)
+                record = models.HabitRecord(date, habit.name, parsed_value)
+            else:
+                record = models.HabitRecord(date, habit.name, None)
+            records_fill.append(record)
+
+    return records_fill
+
+
+def filter(
+    journal_file: str,
+    start_date: dt.date | None,
+    end_date: dt.date,
+    habit_name: str | None,
+) -> list[models.HabitRecord]:
+    """
+    Filter records.
+
+    :param journal_file: Path to the journal file.
+    :param start_date: Start date.
+    :param end_date: End date.
+    :param habit_name: Habit name.
+    :return: Filtered records.
+    """
+    tracked_habits, records = get_state_at_date(journal_file, end_date)
+    if not start_date:
+        try:
+            start_date = min(record.date for record in records)
+        except ValueError:
+            return []
+    return [
+        record
+        for record in records
+        if start_date <= record.date <= end_date
+        and (not habit_name or record.habit_name == habit_name)
+    ]
```

### Comparing `habits_txt-0.1.3/habits_txt/directives.py` & `habits_txt-0.2.0/habits_txt/directives.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.1.3/habits_txt/models.py` & `habits_txt-0.2.0/habits_txt/models.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.1.3/habits_txt/parser.py` & `habits_txt-0.2.0/habits_txt/parser.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.1.3/habits_txt/records_query.py` & `habits_txt-0.2.0/habits_txt/records_query.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.1.3/pyproject.toml` & `habits_txt-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [tool.poetry]
 name = "habits.txt"
-version = "0.1.3"
+version = "0.2.0"
 description = ""
 authors = ["estebanthi <esteban.thilliez@gmail.com>"]
 readme = "README.md"
 packages = [{include = "habits_txt"},{include = "main.py"}]
 
 [tool.poetry.dependencies]
 python = "^3.12"
 croniter = "^2.0.5"
 types-croniter = "^2.0.0.20240423"
+click = "^8.1.7"
 
 [tool.poetry.scripts]
 hbtxt = "main:main"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.2.0"
```

### Comparing `habits_txt-0.1.3/PKG-INFO` & `habits_txt-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,41 @@
 Metadata-Version: 2.1
 Name: habits.txt
-Version: 0.1.3
+Version: 0.2.0
 Summary: 
 Author: estebanthi
 Author-email: esteban.thilliez@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: croniter (>=2.0.5,<3.0.0)
 Requires-Dist: types-croniter (>=2.0.0.20240423,<3.0.0.0)
 Description-Content-Type: text/markdown
 
 # habits.txt
 
+[![PyPI version](https://badge.fury.io/py/habits.txt.svg)](https://badge.fury.io/py/habits.txt)
+
 habits.txt is a plain text habit tracker.
 
+[Installation](#installation) | [Concepts](#concepts) | [Format](#format) | [Directives](#directives)
+
+## Installation
+
+```bash
+pip install habits.txt
+```
+
+You can then use the CLI with:
+
+```bash
+hbtxt --help
+```
+
 ## Concepts
 
 ### Time-bound
 
 A habit is time-bound. It has a start date, and eventually an end date.
 It means with habits.txt, you can track habits for a specific period of time. When you want to stop tracking a habit, you can just stop tracking it.
```

