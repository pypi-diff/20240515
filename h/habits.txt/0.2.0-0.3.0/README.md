# Comparing `tmp/habits_txt-0.2.0.tar.gz` & `tmp/habits_txt-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "habits_txt-0.2.0.tar", max compression
+gzip compressed data, was "habits_txt-0.3.0.tar", max compression
```

## Comparing `habits_txt-0.2.0.tar` & `habits_txt-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     2476 2024-05-14 20:25:35.415585 habits_txt-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-05-14 20:25:35.415585 habits_txt-0.2.0/habits_txt/__init__.py
--rw-r--r--   0        0        0    10111 2024-05-14 20:25:35.415585 habits_txt-0.2.0/habits_txt/builder.py
--rw-r--r--   0        0        0     3343 2024-05-14 20:25:35.415585 habits_txt-0.2.0/habits_txt/cli.py
--rw-r--r--   0        0        0     2154 2024-05-14 20:25:35.415585 habits_txt-0.2.0/habits_txt/config.py
--rw-r--r--   0        0        0      224 2024-05-14 20:25:35.415585 habits_txt-0.2.0/habits_txt/defaults.py
--rw-r--r--   0        0        0     2030 2024-05-14 20:25:35.415585 habits_txt-0.2.0/habits_txt/directives.py
--rw-r--r--   0        0        0      380 2024-05-14 20:25:35.415585 habits_txt-0.2.0/habits_txt/exceptions.py
--rw-r--r--   0        0        0     3768 2024-05-14 20:25:35.415585 habits_txt-0.2.0/habits_txt/journal.py
--rw-r--r--   0        0        0     1855 2024-05-14 20:25:35.415585 habits_txt-0.2.0/habits_txt/models.py
--rw-r--r--   0        0        0     9233 2024-05-14 20:25:35.415585 habits_txt-0.2.0/habits_txt/parser.py
--rw-r--r--   0        0        0      952 2024-05-14 20:25:35.415585 habits_txt-0.2.0/habits_txt/records_query.py
--rw-r--r--   0        0        0      585 2024-05-14 20:25:35.415585 habits_txt-0.2.0/main.py
--rw-r--r--   0        0        0      654 2024-05-14 20:26:18.389436 habits_txt-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2907 1970-01-01 00:00:00.000000 habits_txt-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3109 2024-05-14 20:37:42.341037 habits_txt-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-14 20:25:35.415585 habits_txt-0.3.0/habits_txt/__init__.py
+-rw-r--r--   0        0        0    13971 2024-05-15 17:43:14.132064 habits_txt-0.3.0/habits_txt/builder.py
+-rw-r--r--   0        0        0     7593 2024-05-15 17:43:14.132064 habits_txt-0.3.0/habits_txt/cli.py
+-rw-r--r--   0        0        0     2154 2024-05-14 20:25:35.415585 habits_txt-0.3.0/habits_txt/config.py
+-rw-r--r--   0        0        0      224 2024-05-14 20:25:35.415585 habits_txt-0.3.0/habits_txt/defaults.py
+-rw-r--r--   0        0        0     2323 2024-05-15 17:43:14.132064 habits_txt-0.3.0/habits_txt/directives.py
+-rw-r--r--   0        0        0      380 2024-05-14 20:25:35.415585 habits_txt-0.3.0/habits_txt/exceptions.py
+-rw-r--r--   0        0        0     7655 2024-05-15 17:43:14.132064 habits_txt-0.3.0/habits_txt/journal.py
+-rw-r--r--   0        0        0     2940 2024-05-15 17:43:14.132064 habits_txt-0.3.0/habits_txt/models.py
+-rw-r--r--   0        0        0     9037 2024-05-15 17:43:14.132064 habits_txt-0.3.0/habits_txt/parser.py
+-rw-r--r--   0        0        0      952 2024-05-14 20:25:35.415585 habits_txt-0.3.0/habits_txt/records_query.py
+-rw-r--r--   0        0        0      609 2024-05-15 17:43:14.135397 habits_txt-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3482 1970-01-01 00:00:00.000000 habits_txt-0.3.0/PKG-INFO
```

### Comparing `habits_txt-0.2.0/README.md` & `habits_txt-0.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # habits.txt
 
 [![PyPI version](https://badge.fury.io/py/habits.txt.svg)](https://badge.fury.io/py/habits.txt)
 
 habits.txt is a plain text habit tracker.
 
-[Installation](#installation) | [Concepts](#concepts) | [Format](#format) | [Directives](#directives)
+[Installation](#installation) | [Concepts](#concepts) | [Format](#format) | [Directives](#directives) | [Examples](examples)
 
 ## Installation
 
 ```bash
 pip install habits.txt
 ```
 
@@ -88,7 +88,37 @@
 Example:
 
 ```
 2024-01-01 record "Read 5 pages a day" 5
 2024-01-01 record "Workout" yes
 2024-01-01 "Weight" 70.5
 ```
+
+## Examples
+
+`habits.journal`:
+
+```txt
+2024-01-01 track "Reading" (* * *)
+2024-01-01 track "Exercise" (* * 1,3,5)
+2024-01-01 track "Weight" (* * 1) measurable
+
+# Record habits
+2024-01-01 record "Reading" yes
+2024-01-01 record "Exercise" no
+2024-01-01 record "Weight" 70.5
+```
+
+Once your journal is ready, you can use the CLI to interact with it.
+
+```bash
+# Set the journal file as default journal
+hbtxt config set journal /path/to/habits.journal
+
+# Fill the habits for today interactively
+hbtxt fill -i
+Exercise (2024-01-01): yes
+
+# Filter habit records
+hbtxt filter -n "Exercise"
+2024-01-01 Exercise yes
+```
```

### Comparing `habits_txt-0.2.0/habits_txt/config.py` & `habits_txt-0.3.0/habits_txt/config.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.2.0/habits_txt/models.py` & `habits_txt-0.3.0/habits_txt/models.py`

 * *Files 27% similar despite different names*

```diff
@@ -28,14 +28,33 @@
         :param date: Current date.
         :return: Next date.
         """
         cron_str = f"0 0 {self.day} {self.month} {self.day_of_week}"
         cron = croniter.croniter(cron_str, dt.datetime.combine(date, dt.time()))
         return cron.get_next(dt.datetime).date()
 
+    def get_n_dates(self, start_date: dt.date, end_date: dt.date) -> int:
+        """
+        Get the number of dates between two dates based on the frequency.
+
+        :param start_date: Start date.
+        :param end_date: End date.
+        :return: Number of dates.
+        """
+        n_dates = 1
+        date = start_date
+        while date <= end_date:
+            date = self.get_next_date(date)
+            if date <= end_date:
+                n_dates += 1
+        return n_dates
+
+    def __repr__(self) -> str:
+        return f"{self.day} {self.month} {self.day_of_week}"
+
 
 @dataclass
 class Habit:
     """
     Habit tracked by the user.
 
     Example:
@@ -65,15 +84,15 @@
 
     date: dt.date
     habit_name: str
     value: bool | float | None
 
     @property
     def is_complete(self) -> bool:
-        return bool(self.value)
+        return self.value is not None
 
     def __str__(self) -> str:
         return (
             f"{dt.datetime.strftime(self.date, defaults.DATE_FMT)} "
             f'"{self.habit_name}" {self._str_value()}'
         )
 
@@ -81,7 +100,34 @@
         if self.value is True:
             return defaults.BOOLEAN_TRUE
         elif self.value is False:
             return defaults.BOOLEAN_FALSE
         elif self.value is None:
             return ""
         return str(self.value)
+
+
+@dataclass
+class HabitCompletionInfo:
+    """
+    Information about the completion of a habit.
+    """
+
+    habit: Habit
+    n_records: int
+    n_records_expected: int
+    average_total: float
+    average_present: float
+    start_date: dt.date
+    end_date: dt.date | None
+
+
+@dataclass
+class HabitRecordMatch:
+    """
+    Match between a habit and its records.
+    """
+
+    habit: Habit
+    habit_records: list[HabitRecord]
+    tracking_start_date: dt.date
+    tracking_end_date: dt.date | None
```

### Comparing `habits_txt-0.2.0/habits_txt/parser.py` & `habits_txt-0.3.0/habits_txt/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,36 +64,31 @@
     Example:
     >>> directive_line = '2024-01-01 track "Sample habit" (* * *)'
     >>> parsed_directive = _parse_directive(directive_line, 1)
     """
     if not directive_line or directive_line.startswith(defaults.COMMENT_CHAR):
         return None
     directive_line = re.sub(r"\s+", " ", directive_line)  # Remove extra spaces
-    try:
-        date = _parse_date(directive_line)
-        directive_type = _parse_directive_type(directive_line)
-        habit_name = _parse_habit_name(directive_line)
+    date = _parse_date(directive_line)
+    directive_type = _parse_directive_type(directive_line)
+    habit_name = _parse_habit_name(directive_line)
 
-        if directive_type == directives.DirectiveType.TRACK:
-            frequency = _parse_frequency(directive_line)
-            is_measurable = (
-                re.search(rf"{defaults.MEASURABLE_KEYWORD}$", directive_line)
-                is not None
-            )
-            return directives.TrackDirective(
-                date, habit_name, lineno, frequency, is_measurable
-            )
-        elif directive_type == directives.DirectiveType.UNTRACK:
-            return directives.UntrackDirective(date, habit_name, lineno)
-        elif directive_type == directives.DirectiveType.RECORD:
-            value = _parse_value(directive_line)
-            return directives.RecordDirective(date, habit_name, lineno, value)
-
-    except IndexError:
-        raise exceptions.ParseError(f"Invalid directive format: {directive_line}")
+    if directive_type == directives.DirectiveType.TRACK:
+        frequency = _parse_frequency(directive_line)
+        is_measurable = (
+            re.search(rf"{defaults.MEASURABLE_KEYWORD}$", directive_line) is not None
+        )
+        return directives.TrackDirective(
+            date, habit_name, lineno, frequency, is_measurable
+        )
+    elif directive_type == directives.DirectiveType.UNTRACK:
+        return directives.UntrackDirective(date, habit_name, lineno)
+    elif directive_type == directives.DirectiveType.RECORD:
+        value = _parse_value(directive_line)
+        return directives.RecordDirective(date, habit_name, lineno, value)
 
     return None
 
 
 def _handle_index_error_decorator(name):
     """
     Handle IndexError exceptions in the wrapped function.
```

### Comparing `habits_txt-0.2.0/habits_txt/records_query.py` & `habits_txt-0.3.0/habits_txt/records_query.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.2.0/pyproject.toml` & `habits_txt-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "habits.txt"
-version = "0.2.0"
+version = "0.3.0"
 description = ""
 authors = ["estebanthi <esteban.thilliez@gmail.com>"]
 readme = "README.md"
-packages = [{include = "habits_txt"},{include = "main.py"}]
+packages = [
+    {include = "habits_txt"},
+]
 
 [tool.poetry.dependencies]
 python = "^3.12"
 croniter = "^2.0.5"
-types-croniter = "^2.0.0.20240423"
 click = "^8.1.7"
 
 [tool.poetry.scripts]
-hbtxt = "main:main"
+hbtxt = "bin.hbtxt:main"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.2.0"
 coverage = "^7.5.1"
 isort = "^5.13.2"
 flake8 = "^7.0.0"
```

### Comparing `habits_txt-0.2.0/PKG-INFO` & `habits_txt-0.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: habits.txt
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 Author: estebanthi
 Author-email: esteban.thilliez@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: croniter (>=2.0.5,<3.0.0)
-Requires-Dist: types-croniter (>=2.0.0.20240423,<3.0.0.0)
 Description-Content-Type: text/markdown
 
 # habits.txt
 
 [![PyPI version](https://badge.fury.io/py/habits.txt.svg)](https://badge.fury.io/py/habits.txt)
 
 habits.txt is a plain text habit tracker.
 
-[Installation](#installation) | [Concepts](#concepts) | [Format](#format) | [Directives](#directives)
+[Installation](#installation) | [Concepts](#concepts) | [Format](#format) | [Directives](#directives) | [Examples](examples)
 
 ## Installation
 
 ```bash
 pip install habits.txt
 ```
 
@@ -103,7 +102,37 @@
 
 ```
 2024-01-01 record "Read 5 pages a day" 5
 2024-01-01 record "Workout" yes
 2024-01-01 "Weight" 70.5
 ```
 
+## Examples
+
+`habits.journal`:
+
+```txt
+2024-01-01 track "Reading" (* * *)
+2024-01-01 track "Exercise" (* * 1,3,5)
+2024-01-01 track "Weight" (* * 1) measurable
+
+# Record habits
+2024-01-01 record "Reading" yes
+2024-01-01 record "Exercise" no
+2024-01-01 record "Weight" 70.5
+```
+
+Once your journal is ready, you can use the CLI to interact with it.
+
+```bash
+# Set the journal file as default journal
+hbtxt config set journal /path/to/habits.journal
+
+# Fill the habits for today interactively
+hbtxt fill -i
+Exercise (2024-01-01): yes
+
+# Filter habit records
+hbtxt filter -n "Exercise"
+2024-01-01 Exercise yes
+```
+
```

