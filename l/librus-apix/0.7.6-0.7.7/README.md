# Comparing `tmp/librus_apix-0.7.6.tar.gz` & `tmp/librus_apix-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "librus_apix-0.7.6.tar", last modified: Wed May  1 08:55:56 2024, max compression
+gzip compressed data, was "librus_apix-0.7.7.tar", last modified: Wed May 15 20:50:12 2024, max compression
```

## Comparing `librus_apix-0.7.6.tar` & `librus_apix-0.7.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:55:56.669954 librus_apix-0.7.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-01 08:55:54.000000 librus_apix-0.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-01 08:55:56.669954 librus_apix-0.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-05-01 08:55:54.000000 librus_apix-0.7.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:55:56.669954 librus_apix-0.7.6/librus_apix/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-01 08:55:54.000000 librus_apix-0.7.6/librus_apix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-01 08:55:54.000000 librus_apix-0.7.6/librus_apix/announcements.py
--rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-05-01 08:55:54.000000 librus_apix-0.7.6/librus_apix/attendance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-05-01 08:55:54.000000 librus_apix-0.7.6/librus_apix/completed_lessons.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-01 08:55:54.000000 librus_apix-0.7.6/librus_apix/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-05-01 08:55:54.000000 librus_apix-0.7.6/librus_apix/get_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     9740 2024-05-01 08:55:54.000000 librus_apix-0.7.6/librus_apix/grades.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-01 08:55:54.000000 librus_apix-0.7.6/librus_apix/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-01 08:55:54.000000 librus_apix-0.7.6/librus_apix/homework.py
--rw-r--r--   0 runner    (1001) docker     (127)     6041 2024-05-01 08:55:54.000000 librus_apix-0.7.6/librus_apix/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-05-01 08:55:54.000000 librus_apix-0.7.6/librus_apix/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-01 08:55:54.000000 librus_apix-0.7.6/librus_apix/student_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-01 08:55:54.000000 librus_apix-0.7.6/librus_apix/timetable.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-01 08:55:54.000000 librus_apix-0.7.6/librus_apix/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:55:56.669954 librus_apix-0.7.6/librus_apix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-01 08:55:56.000000 librus_apix-0.7.6/librus_apix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-01 08:55:56.000000 librus_apix-0.7.6/librus_apix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 08:55:56.000000 librus_apix-0.7.6/librus_apix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-01 08:55:56.000000 librus_apix-0.7.6/librus_apix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-01 08:55:56.000000 librus_apix-0.7.6/librus_apix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-01 08:55:54.000000 librus_apix-0.7.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-01 08:55:56.673955 librus_apix-0.7.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 08:55:54.000000 librus_apix-0.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:50:12.086392 librus_apix-0.7.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-15 20:50:04.000000 librus_apix-0.7.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-15 20:50:12.086392 librus_apix-0.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-05-15 20:50:04.000000 librus_apix-0.7.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:50:12.082392 librus_apix-0.7.7/librus_apix/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-15 20:50:04.000000 librus_apix-0.7.7/librus_apix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-15 20:50:04.000000 librus_apix-0.7.7/librus_apix/announcements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-05-15 20:50:04.000000 librus_apix-0.7.7/librus_apix/attendance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-05-15 20:50:04.000000 librus_apix-0.7.7/librus_apix/completed_lessons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-15 20:50:04.000000 librus_apix-0.7.7/librus_apix/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-05-15 20:50:04.000000 librus_apix-0.7.7/librus_apix/get_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9740 2024-05-15 20:50:04.000000 librus_apix-0.7.7/librus_apix/grades.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-15 20:50:04.000000 librus_apix-0.7.7/librus_apix/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-15 20:50:04.000000 librus_apix-0.7.7/librus_apix/homework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6711 2024-05-15 20:50:04.000000 librus_apix-0.7.7/librus_apix/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-05-15 20:50:04.000000 librus_apix-0.7.7/librus_apix/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-15 20:50:04.000000 librus_apix-0.7.7/librus_apix/student_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-15 20:50:04.000000 librus_apix-0.7.7/librus_apix/timetable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-15 20:50:04.000000 librus_apix-0.7.7/librus_apix/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:50:12.086392 librus_apix-0.7.7/librus_apix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-15 20:50:12.000000 librus_apix-0.7.7/librus_apix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-15 20:50:12.000000 librus_apix-0.7.7/librus_apix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 20:50:12.000000 librus_apix-0.7.7/librus_apix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 20:50:12.000000 librus_apix-0.7.7/librus_apix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 20:50:12.000000 librus_apix-0.7.7/librus_apix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-15 20:50:04.000000 librus_apix-0.7.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-15 20:50:12.086392 librus_apix-0.7.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 20:50:04.000000 librus_apix-0.7.7/setup.py
```

### Comparing `librus_apix-0.7.6/README.md` & `librus_apix-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.6/librus_apix/announcements.py` & `librus_apix-0.7.7/librus_apix/announcements.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.6/librus_apix/attendance.py` & `librus_apix-0.7.7/librus_apix/attendance.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.6/librus_apix/completed_lessons.py` & `librus_apix-0.7.7/librus_apix/completed_lessons.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.6/librus_apix/get_token.py` & `librus_apix-0.7.7/librus_apix/get_token.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.6/librus_apix/grades.py` & `librus_apix-0.7.7/librus_apix/grades.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.6/librus_apix/homework.py` & `librus_apix-0.7.7/librus_apix/homework.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.6/librus_apix/messages.py` & `librus_apix-0.7.7/librus_apix/messages.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,22 @@
 from librus_apix.exceptions import ParseError
 from librus_apix.helpers import no_access_check
 from dataclasses import dataclass
 import re
 
 
 @dataclass
+class MessageData:
+    author: str
+    title: str
+    content: str
+    date: str
+
+
+@dataclass
 class Message:
     author: str
     title: str
     date: str
     href: str
     unread: bool
     has_attachment: bool
@@ -78,22 +86,39 @@
     if "nie zostala" in result.text:
         return {False, result}
     if sent_message.status_code == 200:
         return {True, result}
     return {False, result}
 
 
-def message_content(token: Token, content_url: str) -> str:
+def unwrap_message_data(tr):
+    value = tr.select_one("td[class='left']")
+    return value.text if value is not None else ""
+
+
+def message_content(token: Token, content_url: str) -> MessageData:
     soup = no_access_check(
         BeautifulSoup(token.get(token.MESSAGE_URL + "/" + content_url).text, "lxml")
     )
+    message_data = soup.select_one("table[class='stretch']")
+    if message_data is None:
+        raise ParseError("Error in parsing message data.")
+    trs = message_data.select("tr")
+    if len(trs) < 3:
+        raise ParseError("Not enough values to unpack from message_data")
+    author, title, date = trs[:3]
     content = soup.find("div", attrs={"class": "container-message-content"})
     if content is None:
         raise ParseError("Error in parsing message content.")
-    return str(content.text)
+    return MessageData(
+        unwrap_message_data(author),
+        unwrap_message_data(title),
+        content,
+        unwrap_message_data(date),
+    )
 
 
 def parse_sent(message_soup: BeautifulSoup) -> List[Message]:
     msgs: List[Message] = []
     hasAttachment = False
     soup = message_soup.find("table", attrs={"class": "decorated stretch"})
     if soup is None:
```

### Comparing `librus_apix-0.7.6/librus_apix/schedule.py` & `librus_apix-0.7.7/librus_apix/schedule.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.6/librus_apix/student_information.py` & `librus_apix-0.7.7/librus_apix/student_information.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.6/librus_apix/timetable.py` & `librus_apix-0.7.7/librus_apix/timetable.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.6/librus_apix/urls.py` & `librus_apix-0.7.7/librus_apix/urls.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.6/librus_apix.egg-info/SOURCES.txt` & `librus_apix-0.7.7/librus_apix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.6/setup.cfg` & `librus_apix-0.7.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [darglint]
 strictness = long
 docstring_style = google
 
 [metadata]
 name = librus_apix
-version = 0.7.6
+version = v0.7.7
 license = MIT
 description = Web Scraper for Librus Synergia
 long_description = ""
 author = Pascal Jodłowski
 url = https://github.com/poroknights/librus-apix
 keywords = librus, scraper, api, synergia
 classifiers =
```

