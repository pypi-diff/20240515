# Comparing `tmp/beangrep-0.1.1.tar.gz` & `tmp/beangrep-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beangrep-0.1.1.tar", last modified: Mon May 13 08:29:49 2024, max compression
+gzip compressed data, was "beangrep-0.2.0.tar", last modified: Tue May 14 20:34:04 2024, max compression
```

## Comparing `beangrep-0.1.1.tar` & `beangrep-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-13 08:29:49.113628 beangrep-0.1.1/
-drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-13 08:29:49.109629 beangrep-0.1.1/.github/
-drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-13 08:29:49.113628 beangrep-0.1.1/.github/workflows/
--rw-r--r--   0 zack      (1000) zack      (1000)     1377 2024-05-13 07:53:11.000000 beangrep-0.1.1/.github/workflows/python-package.yml
--rw-r--r--   0 zack      (1000) zack      (1000)       80 2024-05-12 11:48:06.000000 beangrep-0.1.1/.gitignore
--rw-r--r--   0 zack      (1000) zack      (1000)    18092 2024-05-12 10:30:41.000000 beangrep-0.1.1/LICENSE-GPL-2.0-or-later
--rw-r--r--   0 zack      (1000) zack      (1000)     7607 2024-05-13 08:29:49.113628 beangrep-0.1.1/PKG-INFO
--rw-r--r--   0 zack      (1000) zack      (1000)     6576 2024-05-12 12:00:47.000000 beangrep-0.1.1/README.md
-drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-13 08:29:49.113628 beangrep-0.1.1/bin/
--rwxr-xr-x   0 zack      (1000) zack      (1000)      308 2024-05-12 10:30:41.000000 beangrep-0.1.1/bin/bean-grep
--rw-r--r--   0 zack      (1000) zack      (1000)     1159 2024-05-13 08:03:05.000000 beangrep-0.1.1/pyproject.toml
--rw-r--r--   0 zack      (1000) zack      (1000)       38 2024-05-13 08:29:49.113628 beangrep-0.1.1/setup.cfg
--rw-r--r--   0 zack      (1000) zack      (1000)      259 2024-05-12 10:30:41.000000 beangrep-0.1.1/setup.py
-drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-13 08:29:49.109629 beangrep-0.1.1/src/
-drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-13 08:29:49.113628 beangrep-0.1.1/src/beangrep/
--rw-r--r--   0 zack      (1000) zack      (1000)      263 2024-05-12 10:30:41.000000 beangrep-0.1.1/src/beangrep/__init__.py
--rw-r--r--   0 zack      (1000) zack      (1000)      284 2024-05-12 10:30:41.000000 beangrep-0.1.1/src/beangrep/__main__.py
--rw-r--r--   0 zack      (1000) zack      (1000)    28450 2024-05-12 10:30:41.000000 beangrep-0.1.1/src/beangrep/beangrep.py
-drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-13 08:29:49.113628 beangrep-0.1.1/src/beangrep.egg-info/
--rw-r--r--   0 zack      (1000) zack      (1000)     7607 2024-05-13 08:29:49.000000 beangrep-0.1.1/src/beangrep.egg-info/PKG-INFO
--rw-r--r--   0 zack      (1000) zack      (1000)      465 2024-05-13 08:29:49.000000 beangrep-0.1.1/src/beangrep.egg-info/SOURCES.txt
--rw-r--r--   0 zack      (1000) zack      (1000)        1 2024-05-13 08:29:49.000000 beangrep-0.1.1/src/beangrep.egg-info/dependency_links.txt
--rw-r--r--   0 zack      (1000) zack      (1000)       43 2024-05-13 08:29:49.000000 beangrep-0.1.1/src/beangrep.egg-info/entry_points.txt
--rw-r--r--   0 zack      (1000) zack      (1000)       91 2024-05-13 08:29:49.000000 beangrep-0.1.1/src/beangrep.egg-info/requires.txt
--rw-r--r--   0 zack      (1000) zack      (1000)        9 2024-05-13 08:29:49.000000 beangrep-0.1.1/src/beangrep.egg-info/top_level.txt
-drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-13 08:29:49.113628 beangrep-0.1.1/tests/
-drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-13 08:29:49.113628 beangrep-0.1.1/tests/data/
--rw-r--r--   0 zack      (1000) zack      (1000)   347280 2024-05-12 10:30:41.000000 beangrep-0.1.1/tests/data/example.beancount
--rw-r--r--   0 zack      (1000) zack      (1000)    13998 2024-05-12 10:30:41.000000 beangrep-0.1.1/tests/test_beangrep.py
+drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-14 20:34:04.252516 beangrep-0.2.0/
+drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-14 20:34:04.248516 beangrep-0.2.0/.github/
+drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-14 20:34:04.248516 beangrep-0.2.0/.github/workflows/
+-rw-r--r--   0 zack      (1000) zack      (1000)     1377 2024-05-13 07:53:11.000000 beangrep-0.2.0/.github/workflows/python-package.yml
+-rw-r--r--   0 zack      (1000) zack      (1000)       81 2024-05-14 12:58:05.000000 beangrep-0.2.0/.gitignore
+-rw-r--r--   0 zack      (1000) zack      (1000)      651 2024-05-14 13:14:24.000000 beangrep-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 zack      (1000) zack      (1000)    18092 2024-05-12 10:30:41.000000 beangrep-0.2.0/LICENSE-GPL-2.0-or-later
+-rw-r--r--   0 zack      (1000) zack      (1000)     8031 2024-05-14 20:34:04.252516 beangrep-0.2.0/PKG-INFO
+-rw-r--r--   0 zack      (1000) zack      (1000)     6958 2024-05-14 13:26:18.000000 beangrep-0.2.0/README.md
+drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-14 20:34:04.248516 beangrep-0.2.0/bin/
+-rwxr-xr-x   0 zack      (1000) zack      (1000)      308 2024-05-12 10:30:41.000000 beangrep-0.2.0/bin/bean-grep
+drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-14 20:34:04.248516 beangrep-0.2.0/dev/
+-rwxr-xr-x   0 zack      (1000) zack      (1000)      571 2024-05-14 13:26:37.000000 beangrep-0.2.0/dev/update_readme.sh
+-rw-r--r--   0 zack      (1000) zack      (1000)     1177 2024-05-14 13:31:36.000000 beangrep-0.2.0/pyproject.toml
+-rw-r--r--   0 zack      (1000) zack      (1000)       38 2024-05-14 20:34:04.252516 beangrep-0.2.0/setup.cfg
+-rw-r--r--   0 zack      (1000) zack      (1000)      259 2024-05-12 10:30:41.000000 beangrep-0.2.0/setup.py
+drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-14 20:34:04.248516 beangrep-0.2.0/src/
+drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-14 20:34:04.248516 beangrep-0.2.0/src/beangrep/
+-rw-r--r--   0 zack      (1000) zack      (1000)      263 2024-05-12 10:30:41.000000 beangrep-0.2.0/src/beangrep/__init__.py
+-rw-r--r--   0 zack      (1000) zack      (1000)      284 2024-05-12 10:30:41.000000 beangrep-0.2.0/src/beangrep/__main__.py
+-rw-r--r--   0 zack      (1000) zack      (1000)    29505 2024-05-14 20:07:37.000000 beangrep-0.2.0/src/beangrep/beangrep.py
+drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-14 20:34:04.252516 beangrep-0.2.0/src/beangrep.egg-info/
+-rw-r--r--   0 zack      (1000) zack      (1000)     8031 2024-05-14 20:34:04.000000 beangrep-0.2.0/src/beangrep.egg-info/PKG-INFO
+-rw-r--r--   0 zack      (1000) zack      (1000)      510 2024-05-14 20:34:04.000000 beangrep-0.2.0/src/beangrep.egg-info/SOURCES.txt
+-rw-r--r--   0 zack      (1000) zack      (1000)        1 2024-05-14 20:34:04.000000 beangrep-0.2.0/src/beangrep.egg-info/dependency_links.txt
+-rw-r--r--   0 zack      (1000) zack      (1000)       43 2024-05-14 20:34:04.000000 beangrep-0.2.0/src/beangrep.egg-info/entry_points.txt
+-rw-r--r--   0 zack      (1000) zack      (1000)      102 2024-05-14 20:34:04.000000 beangrep-0.2.0/src/beangrep.egg-info/requires.txt
+-rw-r--r--   0 zack      (1000) zack      (1000)        9 2024-05-14 20:34:04.000000 beangrep-0.2.0/src/beangrep.egg-info/top_level.txt
+drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-14 20:34:04.248516 beangrep-0.2.0/tests/
+drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-14 20:34:04.248516 beangrep-0.2.0/tests/data/
+-rw-r--r--   0 zack      (1000) zack      (1000)   347380 2024-05-14 09:41:00.000000 beangrep-0.2.0/tests/data/example.beancount
+-rw-r--r--   0 zack      (1000) zack      (1000)    16054 2024-05-14 20:14:47.000000 beangrep-0.2.0/tests/test_beangrep.py
```

### Comparing `beangrep-0.1.1/.github/workflows/python-package.yml` & `beangrep-0.2.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `beangrep-0.1.1/LICENSE-GPL-2.0-or-later` & `beangrep-0.2.0/LICENSE-GPL-2.0-or-later`

 * *Files identical despite different names*

### Comparing `beangrep-0.1.1/PKG-INFO` & `beangrep-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beangrep
-Version: 0.1.1
+Version: 0.2.0
 Summary: Grep-like filter for the Beancount plain text accounting system
 Author-email: Stefano Zacchiroli <zack@upsilon.cc>
 License: GPL-2.0-or-later
 Project-URL: Homepage, https://github.com/zacchiro/beangrep
 Project-URL: Issues, https://github.com/zacchiro/beangrep/issues
 Keywords: accounting,beancount,grep,ledger,plaintext,plaintext-accounting
 Classifier: Programming Language :: Python :: 3
@@ -16,14 +16,15 @@
 License-File: LICENSE-GPL-2.0-or-later
 Requires-Dist: beancount>=2.3.5
 Requires-Dist: click>=8.1
 Provides-Extra: dev
 Requires-Dist: black==23.1; extra == "dev"
 Requires-Dist: flake8>=5; extra == "dev"
 Requires-Dist: mypy>=1; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest>=7.2; extra == "dev"
 Requires-Dist: pytest-cov>=4; extra == "dev"
 
 ![CI status](https://github.com/zacchiro/beangrep/actions/workflows/python-package.yml/badge.svg)
 
 
 Beangrep - grep-like filter for Beancount
@@ -34,24 +35,40 @@
 [beangrep-home]: https://github.com/zacchiro/beangrep
 [beancount-home]: http://beancount.github.io/
 
 
 Installation
 ------------
 
-### Installing from source
+### Prebuilt package
+
+```console
+$ python3 -m venv ./venv    # optional but recommended
+$ source venv/bin/activate
+
+$ pip install beangrep
+[...]
+Successfully installed beancount-2.3.6 beangrep-...
+
+$ bean-grep --help
+Usage: bean-grep [OPTIONS] FILENAME
+[...]
+```
+
+### From source
 
 ```console
 $ git clone https://github.com/zacchiro/beangrep
 $ cd beangrep
 
 $ python3 -m venv ./venv    # optional but recommended
 $ source venv/bin/activate
-(venv) $ pip install -e .
-...
+
+$ pip install -e .
+[...]
 Successfully installed beancount-2.3.6 beangrep-...
 
 $ bean-grep --help
 Usage: bean-grep [OPTIONS] FILENAME
 [...]
 ```
 
@@ -91,14 +108,16 @@
                                   given date predicate. A date predicate start
                                   with an optional comparison operator (one of
                                   '<', '<=', '=', '>=', '>', with '=' being
                                   the default), and is followed by a date in
                                   the form YYYY-[MM[-DD]]. Multiple date
                                   predicates can be given to express complex
                                   date ranges.
+  -l, --link REGEX                Only return entries with at least one link
+                                  matching given regex.
   -m, --meta, --metadata REGEX[:REGEX]
                                   Only return entries with at least one
                                   metadata key/value pair matching given
                                   pattern. A pattern is a pair of regexs
                                   separated by ':', the former matching on
                                   metadata key, the latter on metadata value.
                                   The second regex is optional and defaults to
```

### Comparing `beangrep-0.1.1/README.md` & `beangrep-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -9,24 +9,40 @@
 [beangrep-home]: https://github.com/zacchiro/beangrep
 [beancount-home]: http://beancount.github.io/
 
 
 Installation
 ------------
 
-### Installing from source
+### Prebuilt package
+
+```console
+$ python3 -m venv ./venv    # optional but recommended
+$ source venv/bin/activate
+
+$ pip install beangrep
+[...]
+Successfully installed beancount-2.3.6 beangrep-...
+
+$ bean-grep --help
+Usage: bean-grep [OPTIONS] FILENAME
+[...]
+```
+
+### From source
 
 ```console
 $ git clone https://github.com/zacchiro/beangrep
 $ cd beangrep
 
 $ python3 -m venv ./venv    # optional but recommended
 $ source venv/bin/activate
-(venv) $ pip install -e .
-...
+
+$ pip install -e .
+[...]
 Successfully installed beancount-2.3.6 beangrep-...
 
 $ bean-grep --help
 Usage: bean-grep [OPTIONS] FILENAME
 [...]
 ```
 
@@ -66,14 +82,16 @@
                                   given date predicate. A date predicate start
                                   with an optional comparison operator (one of
                                   '<', '<=', '=', '>=', '>', with '=' being
                                   the default), and is followed by a date in
                                   the form YYYY-[MM[-DD]]. Multiple date
                                   predicates can be given to express complex
                                   date ranges.
+  -l, --link REGEX                Only return entries with at least one link
+                                  matching given regex.
   -m, --meta, --metadata REGEX[:REGEX]
                                   Only return entries with at least one
                                   metadata key/value pair matching given
                                   pattern. A pattern is a pair of regexs
                                   separated by ':', the former matching on
                                   metadata key, the latter on metadata value.
                                   The second regex is optional and defaults to
```

### Comparing `beangrep-0.1.1/pyproject.toml` & `beangrep-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -40,12 +40,13 @@
 bean-grep = "beangrep:cli"
 
 [project.optional-dependencies]
 dev = [
     "black==23.1",
     "flake8>=5",
     "mypy>=1",
+    "pre-commit",
     "pytest>=7.2",
     "pytest-cov>=4",
 ]
 
 [tool.setuptools_scm]
```

### Comparing `beangrep-0.1.1/src/beangrep/beangrep.py` & `beangrep-0.2.0/src/beangrep/beangrep.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # SPDX-FileCopyrightText: 2024 Stefano Zacchiroli <zack@upsilon.cc>
 # SPDX-License-Identifier: GPL-2.0-or-later
 __copyright__ = "Copyright (C) 2024  Stefano Zacchiroli <zack@upsilon.cc>"
 __license__ = "GPL-2.0-or-later"
 
-import beancount.loader  # type: ignore
 import calendar
-import click
 import logging
 import re
 import shutil
 import sys
-
-from beancount.core import data  # type: ignore
-from beancount.core.amount import Amount  # type: ignore
-from beancount.parser import printer  # type: ignore
 from collections.abc import Iterable
 from dataclasses import dataclass
 from datetime import date, timedelta
 from decimal import Decimal
 from enum import Enum
 from tempfile import NamedTemporaryFile
-from typing import cast, Optional, Self
+from typing import Optional, Self, cast
+
+import beancount.loader  # type: ignore
+import click
+from beancount.core import data  # type: ignore
+from beancount.core.amount import Amount  # type: ignore
+from beancount.parser import printer  # type: ignore
 
 KEY_VAL_SEP = ":"
 INTERNALS_META = set(["filename", "lineno"])
 META_VAL_RE = ".*"
 POSTING_TAGS_META = "tags"
 POSTING_TAGS_SEP = ","
 SKIP_INTERNALS = True
-TYPE_SEP = "|"
+TYPE_SEP = ","
 
 
 class RelOp(Enum):
     """Relational comparison operator."""
 
     EQ = 1  # =
     LT = 2  # <
@@ -228,22 +228,73 @@
 @dataclass
 class Criteria:
     """Criteria to select matching Beancount entries."""
 
     account: Optional[re.Pattern] = None
     amount: Optional[list[AmountPredicate]] = None
     date: Optional[list[DatePredicate]] = None
+    link: Optional[re.Pattern] = None
     metadata: Optional[tuple[re.Pattern, re.Pattern]] = None
     narration: Optional[re.Pattern] = None
     payee: Optional[re.Pattern] = None
     somewhere: Optional[re.Pattern] = None
     tag: Optional[re.Pattern] = None
-    types: Optional[set[type]] = None
+    types: Optional[frozenset[type]] = frozenset([data.Transaction])
+
+    @classmethod
+    def build(
+        cls,
+        account_re,
+        amount_preds,
+        date_preds,
+        link_re,
+        metadata_pat,
+        narration_re,
+        payee_re,
+        somewhere_re,
+        tag_re,
+        type_pat,
+        ignore_case,
+    ) -> Self:
+        """Build a Criteria object from command line arguments."""
+        re_flags = 0
+        if ignore_case:
+            re_flags = re.IGNORECASE
+
+        def re_compile(s):
+            return re.compile(s, flags=re_flags)
+
+        criteria = cls()
+
+        if account_re is not None:
+            criteria.account = re_compile(account_re)
+        if amount_preds is not None:
+            criteria.amount = list(map(AmountPredicate.parse, amount_preds))
+        if date_preds is not None:
+            criteria.date = list(map(DatePredicate.parse, date_preds))
+        if link_re is not None:
+            criteria.link = re_compile(link_re)
+        if metadata_pat is not None:
+            if KEY_VAL_SEP in metadata_pat:
+                (key_re, val_re) = metadata_pat.split(KEY_VAL_SEP, maxsplit=1)
+            else:
+                (key_re, val_re) = (metadata_pat, META_VAL_RE)
+            criteria.metadata = (re_compile(key_re), re_compile(val_re))
+        if narration_re is not None:
+            criteria.narration = re_compile(narration_re)
+        if payee_re is not None:
+            criteria.payee = re_compile(payee_re)
+        if somewhere_re is not None:
+            criteria.somewhere = re_compile(somewhere_re)
+        if tag_re is not None:
+            criteria.tag = re_compile(tag_re)
+        if type_pat is not None:
+            criteria.types = parse_types(type_pat)
 
-    # TODO add a criteria matching on ^links
+        return criteria
 
 
 def get_accounts(entry: data.Directive) -> set[str]:
     """Extract account names referenced from a Beancount entry.
 
     - For transactions, return the name of all accounts in postings.
 
@@ -275,15 +326,15 @@
     - Transaction (one amount per Posting)
     - Balance
     - Price
 
     """
     amounts = []
     match type(entry):
-        case (data.Balance | data.Price):
+        case data.Balance | data.Price:
             if hasattr(entry, "amount"):
                 amounts.append(entry.amount)
         case data.Transaction:
             amounts.extend(p.units for p in entry.postings)
 
     return set(amounts)
 
@@ -294,14 +345,20 @@
     Currently this is always a singleton with the entry date, but other dates can be
     returned in the future (e.g., those stored in custom metadata).
 
     """
     return set((entry.date,))
 
 
+def get_links(entry: data.Directive) -> set[str]:
+    """Return the links of an entry, or the empty set if missing."""
+    return set(getattr(entry, "links", set()))
+    # note: without outer `set()` in some cases we would return frozenset-s
+
+
 def get_narration(entry: data.Directive) -> Optional[str]:
     """Return the narration of an entry, or None if missing."""
     return getattr(entry, "narration", None)
 
 
 def get_metadata(
     entry: data.Directive,
@@ -374,14 +431,15 @@
 
     """
     strings: set[str] = set()
 
     strings = strings.union(get_accounts(entry))
     strings = strings.union(str(a) for a in get_amounts(entry))
     strings = strings.union(str(d) for d in get_dates(entry))
+    strings = strings.union(get_links(entry))
     strings = strings.union(
         set(
             str(s)
             for pair in get_metadata(entry, skip_internals=skip_internals)
             for s in pair
         )
     )
@@ -430,14 +488,19 @@
     return bool(  # there is at least one date...
         dates := get_dates(entry)
     ) and any(  # ... that matches all amount predicates
         all(date_pred.match(a) for date_pred in criteria) for a in dates
     )
 
 
+def link_matches(entry: data.Directive, criteria: re.Pattern) -> bool:
+    """Check if a Beancount entry matches links criteria."""
+    return any(criteria.search(link) for link in get_links(entry))
+
+
 def metadata_matches(
     entry: data.Directive,
     criteria: tuple[re.Pattern, re.Pattern],
     skip_internals: bool = SKIP_INTERNALS,
 ) -> bool:
     """Check if a Beancount entry matches metadata criteria."""
     (key_re, val_re) = criteria
@@ -498,14 +561,16 @@
     # inside lambdas, in spite of the explicit `is not None` guard
     if criteria.account is not None:
         predicates.append(lambda e: account_matches(e, criteria.account))  # type: ignore  # noqa:E501
     if criteria.amount is not None:
         predicates.append(lambda e: amount_matches(e, criteria.amount))  # type: ignore
     if criteria.date is not None:
         predicates.append(lambda e: date_matches(e, criteria.date))  # type: ignore
+    if criteria.link is not None:
+        predicates.append(lambda e: link_matches(e, criteria.link))  # type: ignore
     if criteria.metadata is not None:
         predicates.append(
             lambda e: metadata_matches(
                 e, criteria.metadata, skip_internals=skip_internals  # type: ignore
             )
         )
     if criteria.narration is not None:
@@ -540,15 +605,15 @@
     "price": data.Price,
     "query": data.Query,
     "transaction": data.Transaction,
 }
 TYPE_TO_STR: dict[type, str] = dict((v, k) for (k, v) in STR_TO_TYPE.items())
 
 
-def parse_types(types_pat: str) -> set[type]:
+def parse_types(types_pat: str) -> frozenset[type]:
     """Parse a directive type pattern.
 
     A type pattern is a list of type names separated by TYPE_SEP, or the special value
     "all" to mean all directive types.
 
     """
 
@@ -560,64 +625,15 @@
 
     types: list[type] = []
     if types_pat == "all":
         types = data.ALL_DIRECTIVES
     else:
         types = [parse_type(s) for s in types_pat.strip().split(TYPE_SEP)]
 
-    return set(types)
-
-
-def _build_criteria(
-    account_re,
-    amount_preds,
-    date_preds,
-    narration_re,
-    metadata_pat,
-    payee_re,
-    somewhere_re,
-    tag_re,
-    type_pat,
-    ignore_case,
-) -> Criteria:
-    """Build a Criteria object from command line arguments."""
-
-    re_flags = 0
-    if ignore_case:
-        re_flags = re.IGNORECASE
-
-    def re_compile(s):
-        return re.compile(s, flags=re_flags)
-
-    criteria = Criteria()
-
-    if account_re is not None:
-        criteria.account = re_compile(account_re)
-    if amount_preds is not None:
-        criteria.amount = list(map(AmountPredicate.parse, amount_preds))
-    if date_preds is not None:
-        criteria.date = list(map(DatePredicate.parse, date_preds))
-    if metadata_pat is not None:
-        if KEY_VAL_SEP in metadata_pat:
-            (key_re, val_re) = metadata_pat.split(KEY_VAL_SEP, maxsplit=1)
-        else:
-            (key_re, val_re) = (metadata_pat, META_VAL_RE)
-        criteria.metadata = (re_compile(key_re), re_compile(val_re))
-    if narration_re is not None:
-        criteria.narration = re_compile(narration_re)
-    if payee_re is not None:
-        criteria.payee = re_compile(payee_re)
-    if somewhere_re is not None:
-        criteria.somewhere = re_compile(somewhere_re)
-    if tag_re is not None:
-        criteria.tag = re_compile(tag_re)
-    if type_pat is not None:
-        criteria.types = parse_types(type_pat)
-
-    return criteria
+    return frozenset(types)
 
 
 def filter_entries(
     entries,
     criteria,
     posting_tags_meta=POSTING_TAGS_META,
     skip_internals=SKIP_INTERNALS,
@@ -675,14 +691,21 @@
     help="Only return entries with dates matching the given date predicate. "
     "A date predicate start with an optional comparison operator "
     "(one of '<', '<=', '=', '>=', '>', with '=' being the default), "
     "and is followed by a date in the form YYYY-[MM[-DD]]. "
     "Multiple date predicates can be given to express complex date ranges.",
 )
 @click.option(
+    "--link",
+    "-l",
+    "link_re",
+    metavar="REGEX",
+    help="Only return entries with at least one link matching given regex.",
+)
+@click.option(
     "--meta",
     "--metadata",
     "-m",
     "metadata_pat",
     metavar="REGEX[:REGEX]",
     help="Only return entries with at least one metadata key/value pair matching "
     "given pattern. A pattern is a pair of regexs separated by ':', "
@@ -719,22 +742,21 @@
     help="Only return entries with at least one tag matching given regex. "
     "The tag can be located anywhere.",
 )
 @click.option(
     "--type",
     "-T",
     "type_pat",
-    default="transaction",
-    show_default=True,
     metavar="TYPE(S)",
     help="Only return entries of certain types. "
     f"Types are specified as a '{TYPE_SEP}'-separated list of type names; "
     "type names are: open, close, commodity, pad, balance, transaction, "
     "note, event, query, price, document, custom. "
-    "The special value 'all' means: all directive types.",
+    "The special value 'all' means: all directive types. "
+    "[default: transaction]",
 )
 @click.option(
     "--ignore-case/--no-ignore-case",
     "-i",
     "ignore_case",
     default=False,
     show_default=True,
@@ -773,16 +795,17 @@
     "twice or more (e.g., -vv) to DEBUG.",
 )
 def cli(
     filename,
     account_re,
     amount_preds,
     date_preds,
-    narration_re,
+    link_re,
     metadata_pat,
+    narration_re,
     payee_re,
     somewhere_re,
     tag_re,
     type_pat,
     ignore_case,
     posting_tags_meta,
     quiet,
@@ -814,20 +837,21 @@
     if ledger[1]:  # fail upon Beancount loading error(s)
         raise click.FileError(
             filename,
             "\nBeancount load error(s):\n" + "\n".join(str(err) for err in ledger[1]),
         )
 
     try:
-        criteria = _build_criteria(
+        criteria = Criteria.build(
             account_re=account_re,
-            amount_preds=(amount_preds if amount_preds else None),
-            date_preds=(date_preds if amount_preds else None),
-            narration_re=narration_re,
+            amount_preds=(amount_preds or None),
+            date_preds=(date_preds or None),
+            link_re=link_re,
             metadata_pat=metadata_pat,
+            narration_re=narration_re,
             payee_re=payee_re,
             somewhere_re=somewhere_re,
             tag_re=tag_re,
             type_pat=type_pat,
             ignore_case=ignore_case,
         )
     except ValueError as e:
```

### Comparing `beangrep-0.1.1/src/beangrep.egg-info/PKG-INFO` & `beangrep-0.2.0/src/beangrep.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beangrep
-Version: 0.1.1
+Version: 0.2.0
 Summary: Grep-like filter for the Beancount plain text accounting system
 Author-email: Stefano Zacchiroli <zack@upsilon.cc>
 License: GPL-2.0-or-later
 Project-URL: Homepage, https://github.com/zacchiro/beangrep
 Project-URL: Issues, https://github.com/zacchiro/beangrep/issues
 Keywords: accounting,beancount,grep,ledger,plaintext,plaintext-accounting
 Classifier: Programming Language :: Python :: 3
@@ -16,14 +16,15 @@
 License-File: LICENSE-GPL-2.0-or-later
 Requires-Dist: beancount>=2.3.5
 Requires-Dist: click>=8.1
 Provides-Extra: dev
 Requires-Dist: black==23.1; extra == "dev"
 Requires-Dist: flake8>=5; extra == "dev"
 Requires-Dist: mypy>=1; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest>=7.2; extra == "dev"
 Requires-Dist: pytest-cov>=4; extra == "dev"
 
 ![CI status](https://github.com/zacchiro/beangrep/actions/workflows/python-package.yml/badge.svg)
 
 
 Beangrep - grep-like filter for Beancount
@@ -34,24 +35,40 @@
 [beangrep-home]: https://github.com/zacchiro/beangrep
 [beancount-home]: http://beancount.github.io/
 
 
 Installation
 ------------
 
-### Installing from source
+### Prebuilt package
+
+```console
+$ python3 -m venv ./venv    # optional but recommended
+$ source venv/bin/activate
+
+$ pip install beangrep
+[...]
+Successfully installed beancount-2.3.6 beangrep-...
+
+$ bean-grep --help
+Usage: bean-grep [OPTIONS] FILENAME
+[...]
+```
+
+### From source
 
 ```console
 $ git clone https://github.com/zacchiro/beangrep
 $ cd beangrep
 
 $ python3 -m venv ./venv    # optional but recommended
 $ source venv/bin/activate
-(venv) $ pip install -e .
-...
+
+$ pip install -e .
+[...]
 Successfully installed beancount-2.3.6 beangrep-...
 
 $ bean-grep --help
 Usage: bean-grep [OPTIONS] FILENAME
 [...]
 ```
 
@@ -91,14 +108,16 @@
                                   given date predicate. A date predicate start
                                   with an optional comparison operator (one of
                                   '<', '<=', '=', '>=', '>', with '=' being
                                   the default), and is followed by a date in
                                   the form YYYY-[MM[-DD]]. Multiple date
                                   predicates can be given to express complex
                                   date ranges.
+  -l, --link REGEX                Only return entries with at least one link
+                                  matching given regex.
   -m, --meta, --metadata REGEX[:REGEX]
                                   Only return entries with at least one
                                   metadata key/value pair matching given
                                   pattern. A pattern is a pair of regexs
                                   separated by ':', the former matching on
                                   metadata key, the latter on metadata value.
                                   The second regex is optional and defaults to
```

### Comparing `beangrep-0.1.1/tests/data/example.beancount` & `beangrep-0.2.0/tests/data/example.beancount`

 * *Files 0% similar despite different names*

```diff
@@ -1257,19 +1257,19 @@
   Liabilities:US:Chase:Slate                       -52.03 USD
   Expenses:Food:Restaurant                          52.03 USD
 
 2013-06-19 * "Starbucks" "" #trip-san-francisco-2013
   Liabilities:US:Chase:Slate                        -5.98 USD
   Expenses:Food:Coffee                               5.98 USD
 
-2013-06-20 * "Pizza Delfina" "" #trip-san-francisco-2013
+2013-06-20 * "Pizza Delfina" "" #trip-san-francisco-2013 ^a-day-in-sfo
   Liabilities:US:Chase:Slate                       -17.65 USD
   Expenses:Food:Restaurant                          17.65 USD
 
-2013-06-20 * "Mission Chinese Food" "" #trip-san-francisco-2013
+2013-06-20 * "Mission Chinese Food" "" #trip-san-francisco-2013 ^a-day-in-sfo
   Liabilities:US:Chase:Slate                       -30.97 USD
   Expenses:Food:Restaurant                          30.97 USD
 
 2013-06-22 * "Pizza Delfina" "" #trip-san-francisco-2013
   Liabilities:US:Chase:Slate                       -15.34 USD
   Expenses:Food:Restaurant                          15.34 USD
 
@@ -2667,27 +2667,27 @@
   Liabilities:US:Chase:Slate                       -20.04 USD
   Expenses:Food:Restaurant                          20.04 USD
 
 2015-02-20 * "Argo Tea" "" #trip-chicago-2015
   Liabilities:US:Chase:Slate                        -5.31 USD
   Expenses:Food:Coffee                               5.31 USD
 
-2015-02-21 * "Mercadito" "" #trip-chicago-2015
+2015-02-21 * "Mercadito" "" #trip-chicago-2015 ^a-day-in-chicago
   Liabilities:US:Chase:Slate                       -43.53 USD
   Expenses:Food:Restaurant                          43.53 USD
 
-2015-02-21 * "25 Degrees Burger Bar" "" #trip-chicago-2015
+2015-02-21 * "25 Degrees Burger Bar" "" #trip-chicago-2015 ^a-day-in-chicago
   Liabilities:US:Chase:Slate                       -22.76 USD
   Expenses:Food:Restaurant                          22.76 USD
 
-2015-02-21 * "Another Sports Pub" "" #trip-chicago-2015
+2015-02-21 * "Another Sports Pub" "" #trip-chicago-2015 ^a-day-in-chicago
   Liabilities:US:Chase:Slate                       -10.57 USD
   Expenses:Food:Alcohol                             10.57 USD
 
-2015-02-21 * "Argo Tea" "" #trip-chicago-2015
+2015-02-21 * "Argo Tea" "" #trip-chicago-2015 ^a-day-in-chicago
   Liabilities:US:Chase:Slate                        -6.12 USD
   Expenses:Food:Coffee                               6.12 USD
 
 2015-02-23 * "25 Degrees Burger Bar" "" #trip-chicago-2015
   Liabilities:US:Chase:Slate                       -22.44 USD
   Expenses:Food:Restaurant                          22.44 USD
```

### Comparing `beangrep-0.1.1/tests/test_beangrep.py` & `beangrep-0.2.0/tests/test_beangrep.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 # SPDX-FileCopyrightText: 2024 Stefano Zacchiroli <zack@upsilon.cc>
 # SPDX-License-Identifier: GPL-2.0-or-later
 __copyright__ = "Copyright (C) 2024  Stefano Zacchiroli <zack@upsilon.cc>"
 __license__ = "GPL-2.0-or-later"
 
-import beancount.loader  # type: ignore
-import beangrep
 import re
-import pytest
+from datetime import date
+from decimal import Decimal
+from pathlib import Path
 
+import beancount.loader  # type: ignore
+import pytest
 from beancount.core import data  # type: ignore
 from beancount.core.amount import Amount  # type: ignore
+from click.testing import CliRunner
+
+import beangrep
 from beangrep import (
+    TYPE_SEP,
     AmountPredicate,
     Criteria,
     DatePredicate,
     RelOp,
-    TYPE_SEP,
     cli,
     filter_entries,
     parse_types,
 )
-from click.testing import CliRunner
-from datetime import date
-from decimal import Decimal
-from pathlib import Path
 
 SAMPLE_LEDGER = str(
     Path(beangrep.__file__).parents[2] / "tests" / "data" / "example.beancount"
 )
 DIRECTIVES_IN_SAMPLE = 2247  # `bean-quey example.beancount` shows this
 
 _META = data.new_metadata("beangrep/test_beangrep.py", 1234)
@@ -142,131 +143,180 @@
 
 
 def grep_len(entries, criteria):
     """Shorthand to count the number of bean-grep results."""
     return len(list(filter_entries(entries, criteria)))
 
 
+def mk_criteria(**kwargs):
+    """Create a Criteria object overriding the entry types default (unless explicitly
+    present in kwargs), so that transactions are not selected by default.
+
+    """
+    if "types" not in kwargs:
+        kwargs["types"] = None
+    return Criteria(**kwargs)
+
+
 def test_account_filtering():
     l = load_sample_ledger()  # noqa:E741
-    assert grep_len(l, Criteria(account=re.compile("Y2013:US:State"))) == 28
-    assert grep_len(l, Criteria(account=re.compile("US:Federal"))) == 94
-    assert grep_len(l, Criteria(account=re.compile("^US:Federal$"))) == 0
+    assert grep_len(l, mk_criteria(account=re.compile("Y2013:US:State"))) == 28
+    assert grep_len(l, mk_criteria(account=re.compile("US:Federal"))) == 94
+    assert grep_len(l, mk_criteria(account=re.compile("^US:Federal$"))) == 0
 
 
 def test_amount_filtering():
     l = load_sample_ledger()  # noqa:E741
-    assert grep_len(l, Criteria(amount=[AmountPredicate.parse("=3219.17 USD")])) == 2
-    assert grep_len(l, Criteria(amount=[AmountPredicate.parse("3219.17")])) == 2
-    assert grep_len(l, Criteria(amount=[AmountPredicate.parse("=3219.17 EUR")])) == 0
-    assert grep_len(l, Criteria(amount=[AmountPredicate.parse("76.81 USD")])) == 1
-    assert grep_len(l, Criteria(amount=[AmountPredicate.parse(">3000 USD")])) == 29
-    assert grep_len(l, Criteria(amount=[AmountPredicate.parse("<1 USD")])) == 1177
-    # TODO add tests for multiple amount predicates
+    assert grep_len(l, mk_criteria(amount=[AmountPredicate.parse("=3219.17 USD")])) == 2
+    assert grep_len(l, mk_criteria(amount=[AmountPredicate.parse("3219.17")])) == 2
+    assert grep_len(l, mk_criteria(amount=[AmountPredicate.parse("=3219.17 EUR")])) == 0
+    assert grep_len(l, mk_criteria(amount=[AmountPredicate.parse("76.81 USD")])) == 1
+    assert grep_len(l, mk_criteria(amount=[AmountPredicate.parse(">3000 USD")])) == 29
+    assert grep_len(l, mk_criteria(amount=[AmountPredicate.parse("<1 USD")])) == 1177
+    assert (
+        grep_len(
+            l,
+            mk_criteria(
+                amount=[
+                    AmountPredicate.parse(">2800 USD"),
+                    AmountPredicate.parse("<3000 USD"),
+                ]
+            ),
+        )
+        == 8
+    )
 
 
 def test_date_filtering():
     l = load_sample_ledger()  # noqa:E741
-    assert grep_len(l, Criteria(date=[DatePredicate.parse("<1700")])) == 0
-    assert grep_len(l, Criteria(date=[DatePredicate.parse("2013")])) == 739
-    assert grep_len(l, Criteria(date=[DatePredicate.parse("2013-03")])) == 67
-    assert grep_len(l, Criteria(date=[DatePredicate.parse("<=2013-12")])) == 765
-    assert grep_len(l, Criteria(date=[DatePredicate.parse("2014")])) == 750
-    assert grep_len(l, Criteria(date=[DatePredicate.parse("=2015")])) == 731
-    assert grep_len(l, Criteria(date=[DatePredicate.parse("=2015-05-01")])) == 6
-    assert grep_len(l, Criteria(date=[DatePredicate.parse("=2030")])) == 1
-    assert grep_len(l, Criteria(date=[DatePredicate.parse(">=2029-08")])) == 1
-    assert grep_len(l, Criteria(date=[DatePredicate.parse(">2015-12-17")])) == 9
-    assert grep_len(l, Criteria(date=[DatePredicate.parse(">2031")])) == 0
+    assert grep_len(l, mk_criteria(date=[DatePredicate.parse("<1700")])) == 0
+    assert grep_len(l, mk_criteria(date=[DatePredicate.parse("2013")])) == 739
+    assert grep_len(l, mk_criteria(date=[DatePredicate.parse("2013-03")])) == 67
+    assert grep_len(l, mk_criteria(date=[DatePredicate.parse("<=2013-12")])) == 765
+    assert grep_len(l, mk_criteria(date=[DatePredicate.parse("2014")])) == 750
+    assert grep_len(l, mk_criteria(date=[DatePredicate.parse("=2015")])) == 731
+    assert grep_len(l, mk_criteria(date=[DatePredicate.parse("=2015-05-01")])) == 6
+    assert grep_len(l, mk_criteria(date=[DatePredicate.parse("=2030")])) == 1
+    assert grep_len(l, mk_criteria(date=[DatePredicate.parse(">=2029-08")])) == 1
+    assert grep_len(l, mk_criteria(date=[DatePredicate.parse(">2015-12-17")])) == 9
+    assert grep_len(l, mk_criteria(date=[DatePredicate.parse(">2031")])) == 0
 
     assert (
         grep_len(
             l,
-            Criteria(
+            mk_criteria(
                 date=[DatePredicate.parse(">=2014"), DatePredicate.parse("<=2015")]
             ),
         )
         == 750 + 731
     )
     assert (
         grep_len(
             l,
-            Criteria(date=[DatePredicate.parse(">2013"), DatePredicate.parse("<2013")]),
+            mk_criteria(
+                date=[DatePredicate.parse(">2013"), DatePredicate.parse("<2013")]
+            ),
         )
         == 0
     )
 
 
+def test_link_filtering():
+    l = load_sample_ledger()  # noqa:E741
+    assert grep_len(l, mk_criteria(link=re.compile("day-in-sfo"))) == 2
+    assert grep_len(l, mk_criteria(link=re.compile("day-in-chicago"))) == 4
+    assert grep_len(l, mk_criteria(link=re.compile("^a-day-in-"))) == 2 + 4
+
+
 def test_metadata_filtering():
     l = load_sample_ledger()  # noqa:E741
     assert (
-        grep_len(l, Criteria(metadata=(re.compile("^name$"), re.compile("US Dollar"))))
+        grep_len(
+            l, mk_criteria(metadata=(re.compile("^name$"), re.compile("US Dollar")))
+        )
         == 1
     )
-    assert grep_len(l, Criteria(metadata=(re.compile("^name$"), re.compile(".*")))) == 9
     assert (
-        grep_len(l, Criteria(metadata=(re.compile("^name$"), re.compile("Vanguard"))))
+        grep_len(l, mk_criteria(metadata=(re.compile("^name$"), re.compile(".*")))) == 9
+    )
+    assert (
+        grep_len(
+            l, mk_criteria(metadata=(re.compile("^name$"), re.compile("Vanguard")))
+        )
         == 3
     )
     assert (  # filename metadata are skipped by default, hence this returns 0
-        grep_len(l, Criteria(metadata=(re.compile("filename"), re.compile(".*")))) == 0
+        grep_len(l, mk_criteria(metadata=(re.compile("filename"), re.compile(".*"))))
+        == 0
     )
     assert (  # passing skip_internals=False explicitly this time, to match on filename
         len(
             list(
                 filter_entries(
                     l,
-                    Criteria(metadata=(re.compile("filename"), re.compile(".*"))),
+                    mk_criteria(metadata=(re.compile("filename"), re.compile(".*"))),
                     skip_internals=False,
                 )
             )
         )
         == DIRECTIVES_IN_SAMPLE
     )
     assert (
-        grep_len(l, Criteria(metadata=(re.compile(".*"), re.compile("NYSEARC")))) == 4
+        grep_len(l, mk_criteria(metadata=(re.compile(".*"), re.compile("NYSEARC"))))
+        == 4
     )
 
 
 def test_narration_filtering():
     l = load_sample_ledger()  # noqa:E741
-    assert grep_len(l, Criteria(narration=re.compile("Paying the rent"))) == 35
-    assert grep_len(l, Criteria(narration=re.compile("paying the rent"))) == 0
-    assert grep_len(l, Criteria(narration=re.compile("Transfering"))) == 9
-    assert grep_len(l, Criteria(narration=re.compile("one year$"))) == 3
-    assert grep_len(l, Criteria(narration=re.compile("^STATE"))) == 2
+    assert grep_len(l, mk_criteria(narration=re.compile("Paying the rent"))) == 35
+    assert grep_len(l, mk_criteria(narration=re.compile("paying the rent"))) == 0
+    assert grep_len(l, mk_criteria(narration=re.compile("Transfering"))) == 9
+    assert grep_len(l, mk_criteria(narration=re.compile("one year$"))) == 3
+    assert grep_len(l, mk_criteria(narration=re.compile("^STATE"))) == 2
 
 
 def test_payee_filtering():
     l = load_sample_ledger()  # noqa:E741
-    assert grep_len(l, Criteria(payee=re.compile("^Cafe"))) == 59
-    assert grep_len(l, Criteria(payee=re.compile("Cafe Modagor"))) == 51
-    assert grep_len(l, Criteria(payee=re.compile("Cafe Select$"))) == 8
+    assert grep_len(l, mk_criteria(payee=re.compile("^Cafe"))) == 59
+    assert grep_len(l, mk_criteria(payee=re.compile("Cafe Modagor"))) == 51
+    assert grep_len(l, mk_criteria(payee=re.compile("Cafe Select$"))) == 8
 
 
 def test_somewhere_filtering():
     l = load_sample_ledger()  # noqa:E741
-    assert grep_len(l, Criteria(somewhere=re.compile("trip-san"))) == 21
-    assert grep_len(l, Criteria(somewhere=re.compile("San Francisco"))) == 1
+    assert (
+        grep_len(l, mk_criteria(somewhere=re.compile("^Transfering"))) == 9
+    )  # txn narration
+    assert grep_len(l, mk_criteria(somewhere=re.compile("^Cafe"))) == 59  # txn payee
+    assert grep_len(l, mk_criteria(somewhere=re.compile("trip-san"))) == 21  # txn tag
+    assert grep_len(l, mk_criteria(somewhere=re.compile("^a-day-in"))) == 6  # txn link
+    assert grep_len(l, mk_criteria(somewhere=re.compile("2015-05-01"))) == 6  # txn date
+    assert (
+        grep_len(l, mk_criteria(somewhere=re.compile("3219.17 USD"))) == 2
+    )  # txn amount
+    assert (
+        grep_len(l, mk_criteria(somewhere=re.compile("San Francisco"))) == 1
+    )  # event description
 
 
 def test_tag_filtering():
     l = load_sample_ledger()  # noqa:E741
-    assert grep_len(l, Criteria(tag=re.compile("^trip-new-york-2014$"))) == 45
-    assert grep_len(l, Criteria(tag=re.compile("^trip"))) == 92
-    assert grep_len(l, Criteria(tag=re.compile("asfgkjashfg"))) == 0
+    assert grep_len(l, mk_criteria(tag=re.compile("^trip-new-york-2014$"))) == 45
+    assert grep_len(l, mk_criteria(tag=re.compile("^trip"))) == 92
+    assert grep_len(l, mk_criteria(tag=re.compile("asfgkjashfg"))) == 0
 
 
 def test_type_filtering():
     l = load_sample_ledger()  # noqa:E741
-    assert grep_len(l, Criteria(types=data.ALL_DIRECTIVES)) == DIRECTIVES_IN_SAMPLE
-    assert grep_len(l, Criteria(types=[data.Transaction])) == 1146
-    assert grep_len(l, Criteria(types=[data.Open])) == 60
-    assert grep_len(l, Criteria(types=[data.Transaction, data.Open])) == 1146 + 60
-    assert grep_len(l, Criteria(types=[data.Pad])) == 0
+    assert grep_len(l, mk_criteria(types=data.ALL_DIRECTIVES)) == DIRECTIVES_IN_SAMPLE
+    assert grep_len(l, mk_criteria(types=[data.Transaction])) == 1146
+    assert grep_len(l, mk_criteria(types=[data.Open])) == 60
+    assert grep_len(l, mk_criteria(types=[data.Transaction, data.Open])) == 1146 + 60
+    assert grep_len(l, mk_criteria(types=[data.Pad])) == 0
 
 
 def test_parse_types():
     """Test parsing of entry type names."""
     assert set(parse_types("all")) == set(data.ALL_DIRECTIVES)
     assert set(parse_types(TYPE_SEP.join(["open", "close"]))) == set(
         [data.Open, data.Close]
@@ -316,20 +366,26 @@
     assert result.exit_code == 0
     assert "Verizon Wireless" in result.output
 
     result = runner.invoke(cli, ["--date", "=2014-03-28", SAMPLE_LEDGER])
     assert result.exit_code == 0
     assert "Buying groceries" in result.output
 
+    result = runner.invoke(cli, ["--link", "^a-day-in", SAMPLE_LEDGER])
+    assert result.exit_code == 0
+    assert "Mercadito" in result.output
+
     result = runner.invoke(
         cli, ["--metadata", "export:CASH", "--type", "commodity", SAMPLE_LEDGER]
     )
     assert result.exit_code == 0
     assert "US Dollar" in result.output
 
+    result = runner.invoke(cli, ["--metadata", "export", SAMPLE_LEDGER])
+    assert result.exit_code == 1
     result = runner.invoke(
         cli, ["--metadata", "export", "--type", "commodity", SAMPLE_LEDGER]
     )
     assert result.exit_code == 0
     assert "MUTF:VMMXX" in result.output
 
     result = runner.invoke(cli, ["--narration", "24kjhkg8sfjh2kjhkjh", SAMPLE_LEDGER])
@@ -350,15 +406,15 @@
     result = runner.invoke(cli, ["--type", "open", SAMPLE_LEDGER])
     assert result.exit_code == 0
     assert "Federal:PreTax401k" in result.output
 
     result = runner.invoke(cli, ["--type", "custom", SAMPLE_LEDGER])
     assert result.exit_code == 1
 
-    result = runner.invoke(cli, ["--type", "balance|query", SAMPLE_LEDGER])
+    result = runner.invoke(cli, ["--type", "balance,query", SAMPLE_LEDGER])
     assert result.exit_code == 0
     assert "taxes" in result.output
     assert "PreTax401k" in result.output
 
 
 def test_cli_ignore_case():
     """Test --ignore-case flag."""
@@ -387,7 +443,13 @@
     assert runner.invoke(cli, ["-p", "Uncle Boons", SAMPLE_LEDGER]).exit_code == 0
     with open(SAMPLE_LEDGER) as f:
         ledger_text = f.read()
         assert (
             runner.invoke(cli, ["-p", "Uncle Boons", "-"], input=ledger_text).exit_code
             == 0
         )
+
+
+@pytest.mark.skip(reason="should override click exit code when exceptions bubble up")
+def test_cli_file_error():
+    runner = CliRunner()
+    assert runner.invoke(cli, ["does_not_exist_asklahkj15.beancount"]).exit_code == 2
```

