# Comparing `tmp/ClammingPy-1.7-py3-none-any.whl.zip` & `tmp/ClammingPy-1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,17 @@
-Zip file size: 48026 bytes, number of entries: 14
--rw-r--r--  2.0 unx      572 b- defN 24-Mar-30 06:54 clamming/__init__.py
--rw-r--r--  2.0 unx     5527 b- defN 24-Mar-30 07:00 clamming/claminfo.py
--rw-r--r--  2.0 unx    17620 b- defN 24-Apr-20 05:56 clamming/claminfomd.py
--rw-r--r--  2.0 unx    13875 b- defN 24-Apr-07 07:52 clamming/clamsclass.py
--rw-r--r--  2.0 unx    12849 b- defN 24-Apr-07 07:47 clamming/clamspack.py
--rw-r--r--  2.0 unx     2441 b- defN 24-Mar-30 07:00 clamming/clamutils.py
--rw-r--r--  2.0 unx     5232 b- defN 24-Mar-30 07:00 clamming/classparser.py
--rw-r--r--  2.0 unx    18785 b- defN 24-Apr-07 07:56 clamming/html_export.py
--rw-r--r--  2.0 unx      742 b- defN 24-Apr-20 06:02 ClammingPy-1.7.dist-info/AUTHORS
--rw-r--r--  2.0 unx    35147 b- defN 24-Apr-20 06:02 ClammingPy-1.7.dist-info/LICENSE
--rw-r--r--  2.0 unx    47059 b- defN 24-Apr-20 06:02 ClammingPy-1.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-20 06:02 ClammingPy-1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 24-Apr-20 06:02 ClammingPy-1.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1111 b- defN 24-Apr-20 06:02 ClammingPy-1.7.dist-info/RECORD
-14 files, 161061 bytes uncompressed, 46204 bytes compressed:  71.3%
+Zip file size: 52152 bytes, number of entries: 15
+-rw-r--r--  2.0 unx     1832 b- defN 24-May-15 10:04 clamming/__init__.py
+-rw-r--r--  2.0 unx     5728 b- defN 24-May-12 14:43 clamming/claminfo.py
+-rw-r--r--  2.0 unx    17906 b- defN 24-May-15 10:04 clamming/claminfomd.py
+-rw-r--r--  2.0 unx    12017 b- defN 24-May-15 10:04 clamming/clamsclass.py
+-rw-r--r--  2.0 unx     6815 b- defN 24-May-15 10:04 clamming/clamsmodules.py
+-rw-r--r--  2.0 unx    11824 b- defN 24-May-15 12:04 clamming/clamspack.py
+-rw-r--r--  2.0 unx     7778 b- defN 24-May-15 10:04 clamming/clamutils.py
+-rw-r--r--  2.0 unx     6670 b- defN 24-May-12 15:10 clamming/classparser.py
+-rw-r--r--  2.0 unx    20596 b- defN 24-May-15 12:30 clamming/exportoptions.py
+-rw-r--r--  2.0 unx     1856 b- defN 24-May-15 12:34 ClammingPy-1.8.dist-info/AUTHORS
+-rw-r--r--  2.0 unx    34523 b- defN 24-May-15 12:34 ClammingPy-1.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx    48117 b- defN 24-May-15 12:34 ClammingPy-1.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-15 12:34 ClammingPy-1.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-May-15 12:34 ClammingPy-1.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1196 b- defN 24-May-15 12:34 ClammingPy-1.8.dist-info/RECORD
+15 files, 176959 bytes uncompressed, 50202 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -6,38 +6,41 @@
 
 Filename: clamming/claminfomd.py
 Comment: 
 
 Filename: clamming/clamsclass.py
 Comment: 
 
+Filename: clamming/clamsmodules.py
+Comment: 
+
 Filename: clamming/clamspack.py
 Comment: 
 
 Filename: clamming/clamutils.py
 Comment: 
 
 Filename: clamming/classparser.py
 Comment: 
 
-Filename: clamming/html_export.py
+Filename: clamming/exportoptions.py
 Comment: 
 
-Filename: ClammingPy-1.7.dist-info/AUTHORS
+Filename: ClammingPy-1.8.dist-info/AUTHORS
 Comment: 
 
-Filename: ClammingPy-1.7.dist-info/LICENSE
+Filename: ClammingPy-1.8.dist-info/LICENSE
 Comment: 
 
-Filename: ClammingPy-1.7.dist-info/METADATA
+Filename: ClammingPy-1.8.dist-info/METADATA
 Comment: 
 
-Filename: ClammingPy-1.7.dist-info/WHEEL
+Filename: ClammingPy-1.8.dist-info/WHEEL
 Comment: 
 
-Filename: ClammingPy-1.7.dist-info/top_level.txt
+Filename: ClammingPy-1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: ClammingPy-1.7.dist-info/RECORD
+Filename: ClammingPy-1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## clamming/__init__.py

```diff
@@ -1,20 +1,54 @@
+"""
+:filename: clamming.__init__.py
+:author: Brigitte Bigi
+:contact: contact@sppas.org
+:summary: Generate documentation in Markdown or HTML.
+
+.. _This file is part of ClammingPy: https://clamming.sourceforge.io
+..
+    -------------------------------------------------------------------------
+
+    Copyright (C) 2023-2024 Brigitte Bigi
+    Laboratoire Parole et Langage, Aix-en-Provence, France
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU Affero General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU Affero General Public License for more details.
+
+    You should have received a copy of the GNU Affero General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+    This banner notice must not be removed.
+
+    -------------------------------------------------------------------------
+
+"""
+
 from .clamutils import ClamUtils
 from .claminfo import ClamInfo
 from .claminfomd import ClamInfoMarkdown
 from .classparser import ClammingClassParser
 from .clamsclass import ClamsClass
 from .clamspack import ClamsPack
-from .html_export import HTMLDocExport
+from .clamsmodules import ClamsModules
+from .exportoptions import ExportOptions
 
 __author__ = "Brigitte Bigi"
 __copyright__ = "Copyright (C) 2023-2024 Brigitte Bigi, Laboratoire Parole et Langage, Aix-en-Provence, France"
-__version__ = "1.7"
+__version__ = "1.8"
 __all__ = (
     "ClamUtils",
     "ClamInfo",
     "ClamInfoMarkdown",
     "ClammingClassParser",
     "ClamsClass",
     "ClamsPack",
-    "HTMLDocExport"
+    "ClamsModules",
+    "ExportOptions"
 )
```

## clamming/claminfo.py

```diff
@@ -1,31 +1,38 @@
-# clamming.claminfo.py
-#
-# This file is part of ClammingPy tool.
-# (C) 2023-2024 Brigitte Bigi, Laboratoire Parole et Langage,
-# Aix-en-Provence, France.
-#
-# Use of this software is governed by the GNU Public License, version 3.
-#
-# ClammingPy is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# ClammingPy is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with ClammingPy.
-# If not, see <https://www.gnu.org/licenses/licenses.en.html>.
-#
-# This banner notice must not be removed.
-# ---------------------------------------------------------------------------
+"""
+:filename: clamming.claminfo.py
+:author: Brigitte Bigi
+:contact: contact@sppas.org
+:summary: Data class to store information about a clam.
+
+.. _This file is part of ClammingPy: https://clamming.sourceforge.io
+..
+    -------------------------------------------------------------------------
+
+    Copyright (C) 2023-2024 Brigitte Bigi
+    Laboratoire Parole et Langage, Aix-en-Provence, France
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU Affero General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU Affero General Public License for more details.
+
+    You should have received a copy of the GNU Affero General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+    This banner notice must not be removed.
+
+    -------------------------------------------------------------------------
+
+"""
 
 from __future__ import annotations
 from typing import NoReturn
 
 # -----------------------------------------------------------------------
```

## clamming/claminfomd.py

```diff
@@ -1,34 +1,39 @@
-# clamming.claminfomd.py
-#
-# This file is part of ClammingPy tool.
-# (C) 2023-2024 Brigitte Bigi, Laboratoire Parole et Langage,
-# Aix-en-Provence, France.
-#
-# Use of this software is governed by the GNU Public License, version 3.
-#
-# ClammingPy is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# ClammingPy is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with ClammingPy.
-# If not, see <https://www.gnu.org/licenses/licenses.en.html>.
-#
-# This banner notice must not be removed.
-# ---------------------------------------------------------------------------
+"""
+:filename: clamming.claminfomd.py
+:author: Brigitte Bigi
+:contact: contact@sppas.org
+:summary: Convert and store ClamInfo data into Markdown format.
+
+.. _This file is part of ClammingPy: https://clamming.sourceforge.io
+..
+    -------------------------------------------------------------------------
+
+    Copyright (C) 2023-2024 Brigitte Bigi
+    Laboratoire Parole et Langage, Aix-en-Provence, France
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU Affero General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU Affero General Public License for more details.
 
+    You should have received a copy of the GNU Affero General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+    This banner notice must not be removed.
+
+    -------------------------------------------------------------------------
+
+"""
 
-import logging
 import builtins
 
 from .claminfo import ClamInfo
 
 # ---------------------------------------------------------------------------
 
 
@@ -118,15 +123,15 @@
     def convert_name(name: str) -> str:
         """Convert the given name into markdown.
 
         :param name: (str) Name of a function or class
         :return: (str) The name in Markdown
 
         """
-        return "##### {:s}".format(str(name))
+        return "#### {:s}".format(str(name))
 
     # -----------------------------------------------------------------------
 
     @staticmethod
     def convert_source(source: str) -> str:
         """Convert source code into markdown.
 
@@ -477,10 +482,12 @@
                 return "- **{:s}**: {:s}".format(item, descr)
             else:
                 return "- **{:s}**".format(item)
         else:
             return text
 
     # -----------------------------------------------------------------------
+    # Overloads
+    # -----------------------------------------------------------------------
 
     def __str__(self):
         return "{:s}\n{:s}\n{:s}\n".format(self.name, self.source, self.docstring)
```

## clamming/clamsclass.py

```diff
@@ -1,48 +1,43 @@
-# clamming.clamsclass.py
-#
-# This file is part of ClammingPy tool.
-# (C) 2023-2024 Brigitte Bigi, Laboratoire Parole et Langage,
-# Aix-en-Provence, France.
-#
-# Use of this software is governed by the GNU Public License, version 3.
-#
-# ClammingPy is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# ClammingPy is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with ClammingPy. If not, see <http://www.gnu.org/licenses/>.
-#
-# This banner notice must not be removed.
-# ---------------------------------------------------------------------------
+"""
+:filename: clamming.clamsclass.py
+:author: Brigitte Bigi
+:contact: contact@sppas.org
+:summary: Convert a parsed class object into Markdown or HTML content.
 
-# Python standard libraries
-import logging
-import random
-from typing import NoReturn
+.. _This file is part of ClammingPy: https://clamming.sourceforge.io
+..
+    -------------------------------------------------------------------------
+
+    Copyright (C) 2023-2024 Brigitte Bigi
+    Laboratoire Parole et Langage, Aix-en-Provence, France
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU Affero General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU Affero General Public License for more details.
 
-# Libraries in requirements.txt
-try:
-    from pygments import highlight as pygments_highlight
-    from pygments import formatters as pygments_formatter
-    from pygments import lexers as pygments_lexers
-    import markdown2
-    HTML = ""
-except ImportError as e:
-    HTML = str(e)
+    You should have received a copy of the GNU Affero General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+    This banner notice must not be removed.
+
+    -------------------------------------------------------------------------
+
+"""
+
+import logging
 
-# Local classes
 from .claminfo import ClamInfo
+from .clamutils import ClamUtils
 from .classparser import ClammingClassParser
 from .claminfomd import ClamInfoMarkdown
 
 # ---------------------------------------------------------------------------
 
 
 class ClamsClass:
@@ -51,22 +46,14 @@
     :example:
     >>> clamming = ClammingClassParser(Vehicle)
     >>> clams = ClamsClass(clamming)
     >>> md = clams.markdown()
 
     """
 
-    # Keyword arguments of Pygments HtmlFormatter
-    HTML_FORMATTER_ARGS = {
-        "linenos": False,
-        "full": False,
-        "nobackground": True,
-        "wrapcode": True,
-        "style": 'colorful'}
-
     def __init__(self, parsed_obj: ClammingClassParser):
         """Create documentation from the given parsed class object.
 
         HTML conversion depends on external libraries. It could be disabled
         if any of them is missing. If not, customizing the HTML export can
         be done by assigning different values to members or by changing their
         optional parameters.
@@ -80,22 +67,19 @@
         >>> self.markdowner = markdown2.Markdown()
         >>> self.formatter = pygments_formatter.HtmlFormatter(**ClamsClass.HTML_FORMATTER_ARGS)
         >>> self.lexer = pygments_lexers.PythonLexer()
 
         :param parsed_obj: A parsed object.
 
         """
-        self.markdowner = None
-        self.lexer = None
-        self.formatter = None
-        self.__set_html_members()
+        self.__utils = ClamUtils()
 
         # Grabbed information about the class itself: name and docstring.
-        self.__info_class_name = parsed_obj.obj_clams.name
-        self.__info_class_description = parsed_obj.obj_clams
+        self.__info_class_name = parsed_obj.get_obj_clams().name
+        self.__info_class_description = parsed_obj.get_obj_clams()
 
         # Grabbed information about the class constructor: name, args, source
         # and docstring. They have empty values if the class has no constructor.
         self.__info_constructor = parsed_obj.init_clams
 
         # Grabbed information about the class functions: name, args, source
         # and docstring. To increase documentation readability, they are
@@ -127,29 +111,14 @@
         """Return the name of the documented class."""
         return self.__info_class_name
 
     name = property(get_name, None)
 
     # -----------------------------------------------------------------------
 
-    def __set_html_members(self) -> NoReturn:
-        """Set the class members for HTML export if available."""
-        if len(HTML) == 0:
-            # Use markdown2 library to convert docstrings
-            self.markdowner = markdown2.Markdown()
-            # Use pygments library to convert source code
-            # https://pygments.org/docs/formatters/#HtmlFormatter
-            self.formatter = pygments_formatter.HtmlFormatter(**ClamsClass.HTML_FORMATTER_ARGS)
-            # https://pygments.org/docs/lexers/#pygments.lexers.python.PythonLexer
-            self.lexer = pygments_lexers.PythonLexer()
-        else:
-            logging.warning("ClamsClass: HTML conversion is disabled: {:s}".format(HTML))
-
-    # -----------------------------------------------------------------------
-
     def markdown(self) -> str:
         """Get Markdown content of the parsed object.
 
         :return: (str) Content in Markdown format
 
         """
         md = list()
@@ -198,16 +167,17 @@
         """Get HTML content of the parsed object.
 
         :return: (str) Content in HTML format
         :raises: ImportError: if one of the requirements is not installed
 
         """
         # Can we export to HTML?
-        if len(HTML) > 0:
-            raise ImportError(HTML)
+        if self.__utils.markdowner is None:
+            logging.warning("Markdown to HTML conversion is disabled.")
+            return ""
 
         hd = list()
         cid = self.__info_class_name
         hd.append('<section id="#{:s}">'.format(cid))
         hd.append('<h2>Class {:s}</h2>\n'.format(self.__info_class_name))
 
         if self.__info_class_description.docstring is not None:
@@ -243,51 +213,37 @@
             hd.append('<h3 id="#protected_fct_{:s}">Protected functions</h3>'.format(cid))
             for info in self.__info_protected_fcts:
                 hd.append(self.__claminfo_to_html(info))
             hd.append("</section>")
 
         if len(self.__info_overloads) > 0:
             hd.append("<section>")
-            hd.append('<h3 id="#overloads_{:s}">Overloads</h3>')
+            hd.append('<h3 id="#overloads_{:s}">Overloads</h3>'.format(cid))
             for info in self.__info_overloads:
                 hd.append(self.__claminfo_to_html(info))
             hd.append("</section>")
 
         hd.append('</section>')
 
         html_result = "\n".join(hd)
         return html_result.replace("<p></p>", "")
 
     # -----------------------------------------------------------------------
+    # Private
+    # -----------------------------------------------------------------------
 
     def __docstring_to_html(self, docstring: str) -> str:
         """Return the HTML of the given docstring.
 
         :param docstring: (str)
         :return: (str) HTML
 
         """
         _md = ClamInfoMarkdown.convert_docstring(docstring)
-        h = list()
-        code = list()
-        for line in _md.split("\n"):
-            if line.startswith("    >>> ") is True:
-                code.append(line[4:])
-            elif line.startswith("    > ") is True:
-                code.append(line[6:])
-            else:
-                if len(code) > 0:
-                    h.append(pygments_highlight("\n".join(code), self.lexer, self.formatter))
-                    code = list()
-                h.append(self.markdowner.convert(line))
-        if len(code) > 0:
-            h.append(pygments_highlight("\n".join(code), self.lexer, self.formatter))
-
-        html_result = "\n".join(h)
-        return html_result.replace("<p></p>", "")
+        return self.__utils.markdown_to_html(_md)
 
     # -----------------------------------------------------------------------
 
     def __claminfo_to_html(self, claminfo: ClamInfo, with_name=True) -> str:
         """Return the HTML of the given ClamInfo instance.
 
         :return: (str) HTML
@@ -306,43 +262,38 @@
         # Docstring: operated by markdown2, and pygments if example
         if claminfo.docstring is not None:
             _html = self.__docstring_to_html(claminfo.docstring)
             # Force arguments to be in a Parameters section
             if len(params) > 0 and "<h5>Parameters</h5>" not in _html:
                 _md = "\n\n##### Parameters\n"
                 _md += "\n".join(["- **{:s}**".format(p) for p in params])
-                _html += self.markdowner.convert(_md)
+                _html += self.__utils.markdown_convert(_md)
             h.append(ClamsClass._docstring_article(_html))
             h.append("\n")
 
         # Source code: operated by pygments
         if len(claminfo.source) > 0:
-            _html = pygments_highlight(claminfo.source, self.lexer, self.formatter)
-            h.append(ClamsClass._source_article("View Source", _html))
+            _html = ClamUtils().source_to_html(claminfo.source)
+            h.append(ClamsClass._source_accordion("View Source", _html))
         h.append("\n")
 
         html_result = "\n".join(h)
         return html_result.replace("<p></p>", "")
 
 # ---------------------------------------------------------------------------
 
     @staticmethod
-    def _source_article(header_content: str, main_content: str) -> str:
-        """Return the given content embedded into an article.
-
-        With CSS+JS, this article can be turned into an *accessible* accordion.
+    def _source_accordion(header_content: str, main_content: str) -> str:
+        """Return the given content embedded into a details element.
 
         :param header_content: (str) Content of the collapsed part
         :param main_content: (str) Content of the expanded part
         :return: (str) HTML-5 of an article
 
         """
-        nb = random.randint(10000, 99999)
-        id_btn = "{:d}_collapse_id".format(nb)
-        id_main = "{:d}_expand_id".format(nb)
         h = list()
         h.append('    <details>')
         h.append('    <summary>')
         h.append(header_content)
         h.append('    </summary>')
         h.append(main_content)
         h.append('    </details>')
```

## clamming/clamspack.py

```diff
@@ -1,42 +1,55 @@
-# clamming.clamspack.py
-#
-# This file is part of ClammingPy tool.
-# (C) 2023-2024 Brigitte Bigi, Laboratoire Parole et Langage,
-# Aix-en-Provence, France.
-#
-# Use of this software is governed by the GNU Public License, version 3.
-#
-# ClammingPy is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# ClammingPy is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with ClammingPy. If not, see <http://www.gnu.org/licenses/>.
-#
-# This banner notice must not be removed.
-# ---------------------------------------------------------------------------
+"""
+:filename: clamming.clamspack.py
+:author: Brigitte Bigi
+:contact: contact@sppas.org
+:summary: Create documentation of a module into Markdown or HTML.
+
+.. _This file is part of ClammingPy: https://clamming.sourceforge.io
+..
+    -------------------------------------------------------------------------
+
+    Copyright (C) 2023-2024 Brigitte Bigi
+    Laboratoire Parole et Langage, Aix-en-Provence, France
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU Affero General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU Affero General Public License for more details.
+
+    You should have received a copy of the GNU Affero General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+    This banner notice must not be removed.
+
+    -------------------------------------------------------------------------
+
+"""
 
 from __future__ import annotations
 import inspect
 import codecs
 import os
 import logging
 from typing import Any
+try:
+    import markdown2
+    HTML = ""
+except ImportError as e:
+    HTML = str(e)
 
 import clamming
 from clamming.clamsclass import ClamsClass
 from clamming.classparser import ClammingClassParser
-from clamming.html_export import HTMLDocExport
+from clamming.exportoptions import ExportOptions
 from clamming.clamutils import ClamUtils
 
 # ---------------------------------------------------------------------------
 
 
 class ClamsPack:
     """Create documentation of a module into Markdown or HTML.
@@ -53,76 +66,134 @@
         :param pack: (module) A Python module
         :raises: TypeError: given 'pack' is not a module
 
         """
         if inspect.ismodule(pack) is False:
             raise TypeError("Expected a Python module. Got {:s} instead.".format(str(pack)))
 
-        self.__name = pack.__name__
+        self.__pack = pack
         self.__clams = list()
         try:
             for class_name in pack.__all__:
                 # Turn class_name into an instance name
-                class_inst = ClamUtils.get_class(class_name, self.__name)
+                class_inst = ClamUtils.get_class(class_name, self.__pack.__name__)
                 if class_inst is not None:
                     # Parse the object and store collected information = clamming
                     clammer = ClammingClassParser(class_inst)
                     # Store the collected clams
                     self.__clams.append(ClamsClass(clammer))
         except AttributeError:
             logging.warning("Attribute __all__ is missing in package {:s} => No auto documentation."
-                            "".format(self.__name))
+                            "".format(self.__pack.__name__))
 
     # -----------------------------------------------------------------------
 
     def get_name(self) -> str:
         """Return the name of the package."""
-        return self.__name
+        return self.__pack.__name__
 
     name = property(get_name, None)
 
     # -----------------------------------------------------------------------
 
-    def markdown(self) -> str:
-        """Return the documentation of the package as a standalone Markdown content."""
+    def get_readme(self) -> str:
+        """Return the content of the README file of the package, if any."""
+        path_to_readme = os.path.dirname(self.__pack.__file__)
+        readme_content = ""
+        for f in os.listdir(path_to_readme):
+            if "readme" in f.lower():
+                readme_file = os.path.join(path_to_readme, f)
+                try:
+                    with open(readme_file, "r", encoding="utf-8") as f:
+                        readme_content = f.read()
+                except Exception as e:
+                    logging.warning("A README file was found but could not be read: {:s}".format(str(e)))
+                break
+
+        return readme_content
+
+    readme = property(get_readme, None)
+
+    # -----------------------------------------------------------------------
+
+    def markdown(self, exporter: ExportOptions | None = None) -> str:
+        """Return the documentation of the package as a standalone Markdown content.
+
+        """
         md = list()
-        md.append("## Package `{:s}`\n".format(self.__name))
+        md.append("# {:s} module\n".format(self.name))
+
+        # Module README content - if any
+        if exporter is not None:
+            if exporter.readme is True and len(HTML) == 0:
+                readme_content = self.get_readme()
+                if len(readme_content) > 0:
+                    md.append(readme_content)
+
+        # Classes
+        md.append("## List of classes\n")
+
         for clams in self.__clams:
             md.append(clams.markdown())
         md.append("\n\n~ Created using [Clamming](https://clamming.sf.net) version {:s} ~\n"
                   "".format(clamming.__version__))
 
         return "\n".join(md)
 
     # -----------------------------------------------------------------------
 
-    def html(self) -> str:
+    def html(self, exporter: ExportOptions | None = None) -> str:
         """Return the documentation of the package as an HTML content."""
         html = list()
-        html.append("<h1> Package `{:s}` </h1>\n".format(self.__name))
+        html.append("<h1>{:s} module</h1>\n".format(self.name))
+
+        # Module README content - if any
+        if exporter is not None:
+            if exporter.readme is True and len(HTML) == 0:
+                readme_content = self.get_readme()
+                if len(readme_content) > 0:
+                    html.append("    <section id=\"readme\">\n")
+                    html.append(ClamUtils().markdown_to_html(readme_content))
+                    html.append("    </section>\n")
+
+        html.append("<h2>List of classes</h2>\n")
         for clams in self.__clams:
             html.append(clams.html())
-        html.append("\n\n<p>~ Created using <a href=\"https://clamming.sf.net\">Clamming</a> version {:s} ~</p>\n"
+        html.append("\n\n<p>~ Created using <a href=\"https://clamming.sf.net\">ClammingPy</a> version {:s} ~</p>\n"
                     "".format(clamming.__version__))
+
         return "\n".join(html)
 
     # -----------------------------------------------------------------------
 
-    def html_index(self, path_name: str | None = None) -> str:
+    def html_index(self,
+                   path_name: str | None = None,
+                   exporter: ExportOptions | None = None) -> str:
         """Create the HTML content of an index for the package.
 
         :param path_name: (str) Path where the exported HTML files are, or None for a standalone content.
+        :param exporter: (HTMLDocExport) Options for HTML output files
         :return: (str) HTML code
 
         """
         out = list()
-        out.append("    <section id=\"#{:s}\">".format(self.__name))
-        out.append("    <h1>Module {:s}</h1>".format(self.__name))
-        out.append('        <section class="cards-panel">')
+        out.append("    <section id=\"#{:s}\">".format(self.name))
+        out.append("    <h1>{:s} module</h1>".format(self.name))
 
+        # Module README content - if any
+        if exporter is not None:
+            if exporter.readme is True and len(HTML) == 0:
+                readme_content = self.get_readme()
+                if len(readme_content) > 0:
+                    out.append("    <section id=\"readme\">\n")
+                    out.append(ClamUtils().markdown_to_html(readme_content))
+                    out.append("    </section>\n")
+
+        out.append("<h2>List of classes</h2>\n")
+        out.append('        <section class="cards-panel">')
         for i in range(len(self.__clams)):
             clams = self.__clams[i]
             out.append('        <article class="card">')
             out.append('            <header><span>{:d}</span></header>'.format(i + 1))
             out.append('            <main>')
             out.append('                <h3>{:s}</h3>'.format(clams.name))
             out.append('            </main>')
@@ -141,167 +212,88 @@
         out.append("        </section>")
         out.append("    </section>")
 
         return "\n".join(out)
 
     # -----------------------------------------------------------------------
 
-    def html_export_clams(self, path_name: str, html_exporter: HTMLDocExport) -> list[str]:
+    def html_export_clams(self, path_name: str, exporter: ExportOptions) -> list[str]:
         """Create the HTML pages of all classes of the package.
 
         :param path_name: (str) Path where to add the exported HTML files
-        :param html_exporter: (HTMLDocExport) Options for HTML output files
+        :param exporter: (HTMLDocExport) Options for HTML output files
         :return: (list) Exported file names
 
         """
-        out_html = os.path.join(path_name, self.__name + ".html")
+        out = list()
         if os.path.exists(path_name) is False:
             os.mkdir(path_name)
 
-        with codecs.open(out_html, "w", "utf-8") as fp:
-            fp.write("<!DOCTYPE html>\n")
-            fp.write("<html>\n")
-            fp.write(html_exporter.get_head())
-            fp.write("<body class=\"{:s}\">\n".format(html_exporter.get_theme()))
-            fp.write("    {:s}\n".format(html_exporter.get_header()))
-            fp.write("    {:s}\n".format(html_exporter.get_nav()))
-            fp.write("    <main id=\"main-content\" class=\"toc-shift\">\n")
-            fp.write("    <div id=\"toc-content\">\n")
-            fp.write(self.html_index(path_name=""))
-            fp.write("    </div>\n")
-            fp.write("    </main>\n")
-            fp.write("    {:s}\n".format(html_exporter.get_footer()))
-            fp.write("</body>\n")
-            fp.write("</html>\n")
-
-        out = list()
+        out_html = os.path.join(path_name, self.name + ".html")
+        self.__module_index(out_html, exporter)
         out.append(out_html)
 
         for i in range(len(self.__clams)):
             clams = self.__clams[i]
             out_html = os.path.join(path_name, clams.name + ".html")
             logging.info("Export {:s}".format(out_html))
 
-            html_exporter.prev_class = None if i == 0 else self.__clams[i - 1].name + ".html"
-            html_exporter.next_class = None if i + 1 == len(self.__clams) else self.__clams[i + 1].name + ".html"
+            exporter.prev_class = None if i == 0 else self.__clams[i - 1].name + ".html"
+            exporter.next_class = None if i + 1 == len(self.__clams) else self.__clams[i + 1].name + ".html"
             html_content = clams.html()
-
-            with codecs.open(out_html, "w", "utf-8") as fp:
-                fp.write("<!DOCTYPE html>\n")
-                fp.write("<html>\n")
-                fp.write(html_exporter.get_head())
-                fp.write("<body class=\"{:s}\">\n".format(html_exporter.get_theme()))
-                fp.write("    {:s}\n".format(html_exporter.get_header()))
-                fp.write("    {:s}\n".format(html_exporter.get_nav()))
-                fp.write("    <main id=\"main-content\" class=\"toc-shift\">\n")
-                fp.write("    <div id=\"toc-content\">\n")
-                fp.write("    <section id=\"#{:s}\">".format(self.__name))
-                fp.write("    <h1>Module {:s}</h1>\n".format(self.__name))
-                fp.write(html_content)
-                fp.write("    </section>")
-                fp.write("    </div>\n")
-                fp.write("    </main>\n")
-                fp.write("    {:s}\n".format(html_exporter.get_footer()))
-                fp.write("</body>\n")
-                fp.write("</html>\n")
+            self.__module_class(out_html, exporter, html_content)
 
         return out
 
-    # -----------------------------------------------------------------------
-    # Documentation for a list of modules.
-    # -----------------------------------------------------------------------
-
-    @staticmethod
-    def markdown_export_packages(clams_packs: list[ClamsPack], path_name: str, html_exporter: HTMLDocExport) -> list[str]:
-        """Create a Markdown file for each of the given packages.
-
-        :param clams_packs: (list) List of ClamsPack
-        :param path_name: (str) Path where to add the exported md files
-        :param html_exporter: (HTMLDocExport) Options for output files
-        :return: (list) Exported file names
-
-        """
-        out = list()
-
-        for clams_pack in clams_packs:
-            out_md = os.path.join(path_name, clams_pack.name + ".md")
-            if os.path.exists(path_name) is False:
-                os.mkdir(path_name)
-
-            logging.info("Export {:s}".format(out_md))
-            with codecs.open(out_md, "w", "utf-8") as fp:
-                fp.write(clams_pack.markdown())
-            out.append(out_md)
-
-        return out
-
-    # -----------------------------------------------------------------------
+    # ---------------------------------------------------------------------------
+    # Private
+    # ---------------------------------------------------------------------------
 
-    @staticmethod
-    def html_export_index(clams_packs: list[ClamsPack], path_name: str, html_exporter: HTMLDocExport) -> str:
-        """Write the index.html file from the given list of packages.
-
-        :param clams_packs: (list) List of ClamsPack
-        :param path_name: (str) Path where to add the exported index.html file
-        :param html_exporter: (HTMLDocExport) Options for HTML output files
-        :return: (str) Filename of the created HTML index file
+    def __module_index(self, out_html, exporter):
+        """Export an index for the module.
 
         """
-        out = os.path.join(path_name, "index.html")
-        if os.path.exists(path_name) is False:
-            os.mkdir(path_name)
-
-        with codecs.open(out, "w", "utf-8") as fp:
+        # The module file index: links to each class file
+        with codecs.open(out_html, "w", "utf-8") as fp:
             fp.write("<!DOCTYPE html>\n")
             fp.write("<html>\n")
-            fp.write(html_exporter.get_head())
-            fp.write("<body class=\"{:s}\">\n".format(html_exporter.get_theme()))
-            fp.write("    {:s}\n".format(html_exporter.get_header()))
-            fp.write("    {:s}\n".format(html_exporter.get_nav()))
-            fp.write("    <main id=\"main-content\" class=\"toc-shift\">\n")
-            fp.write("    <div id=\"toc-content\">\n")
-            for clams_pack in clams_packs:
-                # path_name argument is a relative path of the pages to the index
-                fp.write(clams_pack.html_index(path_name="."))
-            fp.write("    </div>\n")
+            fp.write(exporter.get_head())
+            fp.write("<body class=\"{:s}\">\n".format(exporter.get_theme()))
+            fp.write("    {:s}\n".format(exporter.get_header()))
+            fp.write("    {:s}\n".format(exporter.get_nav()))
+            fp.write("    <main id=\"main-content\">\n")
+            # Module index: list of classes in the module
+            fp.write(self.html_index(path_name="", exporter=exporter))
             fp.write("    </main>\n")
-            fp.write("    {:s}\n".format(html_exporter.get_footer()))
+            fp.write("    {:s}\n".format(exporter.get_footer()))
             fp.write("</body>\n")
             fp.write("</html>\n")
-        return out
 
-    # -----------------------------------------------------------------------
+    # ---------------------------------------------------------------------------
 
-    @staticmethod
-    def html_export_packages(clams_packs: list[ClamsPack], path_name: str, html_exporter: HTMLDocExport) -> list:
-        """Create all the HTML files from the given list of packages.
-
-        - create the HTML file for each class of each given module;
-        - create an index.html file.
-
-        :param clams_packs: (list) List of ClamsPack
-        :param path_name: (str) Path where to add the exported index.html file
-        :param html_exporter: (HTMLDocExport) Options for HTML output files
+    def __module_class(self, out_html, exporter, content):
+        """Export a content for the module.
 
         """
-        out = list()
-
-        # Create the index.html page. It's a table of content.
-        out_index = ClamsPack.html_export_index(clams_packs, path_name, html_exporter)
-        out.append(out_index)
-
-        # Create an HTML page for each class of each module
-        for i in range(len(clams_packs)):
-            clams_pack = clams_packs[i]
-            html_exporter.prev_module = None if i == 0 else clams_packs[i - 1].name + ".html"
-            html_exporter.next_module = None if i + 1 == len(clams_packs) else clams_packs[i + 1].name + ".html"
-            out_html = clams_pack.html_export_clams(path_name, html_exporter)
-            out.extend(out_html)
-
-        return out
+        with codecs.open(out_html, "w", "utf-8") as fp:
+            fp.write("<!DOCTYPE html>\n")
+            fp.write("<html>\n")
+            fp.write(exporter.get_head())
+            fp.write("<body class=\"{:s}\">\n".format(exporter.get_theme()))
+            fp.write("    {:s}\n".format(exporter.get_header()))
+            fp.write("    {:s}\n".format(exporter.get_nav()))
+            fp.write("    <main id=\"main-content\">\n")
+            fp.write("    <section id=\"#{:s}\">".format(self.name))
+            fp.write("    <h1>Module {:s}</h1>\n".format(self.name))
+            fp.write(content)
+            fp.write("    </section>")
+            fp.write("    </main>\n")
+            fp.write("    {:s}\n".format(exporter.get_footer()))
+            fp.write("</body>\n")
+            fp.write("</html>\n")
 
     # ---------------------------------------------------------------------------
     # Overloads
     # ---------------------------------------------------------------------------
 
     def __len__(self):
         """Return the number of documented pages of the package."""
```

## clamming/clamutils.py

```diff
@@ -1,44 +1,89 @@
-# clamming.clamutils.py
-#
-# This file is part of ClammingPy tool.
-# (C) 2023-2024 Brigitte Bigi, Laboratoire Parole et Langage,
-# Aix-en-Provence, France.
-#
-# Use of this software is governed by the GNU Public License, version 3.
-#
-# ClammingPy is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# ClammingPy is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with ClammingPy. If not, see <http://www.gnu.org/licenses/>.
-#
-# This banner notice must not be removed.
-# ---------------------------------------------------------------------------
+"""
+:filename: clamming.clamsutils.py
+:author: Brigitte Bigi
+:contact: contact@sppas.org
+:summary: Utilities for working with CLAMS data.
+
+.. _This file is part of ClammingPy: https://clamming.sourceforge.io
+..
+    -------------------------------------------------------------------------
+
+    Copyright (C) 2023-2024 Brigitte Bigi
+    Laboratoire Parole et Langage, Aix-en-Provence, France
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU Affero General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU Affero General Public License for more details.
+
+    You should have received a copy of the GNU Affero General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+    This banner notice must not be removed.
+
+    -------------------------------------------------------------------------
+
+"""
 
 from __future__ import annotations
 import inspect
 import importlib
+import logging
 from typing import Any
+# Libraries in requirements.txt
+try:
+    from pygments import highlight as pygments_highlight
+    from pygments import formatters as pygments_formatter
+    from pygments import lexers as pygments_lexers
+    import markdown2
+    HTML = ""
+except ImportError as e:
+    HTML = str(e)
 
 # ---------------------------------------------------------------------------
 
 
 class ClamUtils:
-    """Some utilities for Clamming.
+    """Some utilities for ClammingPy.
 
     """
 
+    # Keyword arguments of Pygments HtmlFormatter
+    HTML_FORMATTER_ARGS = {
+        "linenos": False,
+        "full": False,
+        "nobackground": True,
+        "wrapcode": True,
+        "style": 'colorful'}
+
+    # ---------------------------------------------------------------------------
+
+    def __init__(self, ):
+        """Create a ClamUtils instance."""
+        self.markdowner = None
+        self.lexer = None
+        self.formatter = None
+
+        if len(HTML) == 0:
+            # Use markdown2 library to convert docstrings
+            self.markdowner = markdown2.Markdown()
+            # Use pygments library to convert source code
+            # https://pygments.org/docs/formatters/#HtmlFormatter
+            self.formatter = pygments_formatter.HtmlFormatter(**ClamUtils.HTML_FORMATTER_ARGS)
+            # https://pygments.org/docs/lexers/#pygments.lexers.python.PythonLexer
+            self.lexer = pygments_lexers.PythonLexer()
+
+    # ---------------------------------------------------------------------------
+
     @staticmethod
     def get_class(class_name: str, module_name: str | None = None) -> Any:
         """Return the class matching the given class name or None if invalid.
 
         :example:
         >>> c = ClamUtils.get_class("ClamsPack", "clamming")
         >>> print(c)
@@ -62,7 +107,116 @@
         # Returns None if class with given name doesn't exist in the module
         class_inst = getattr(module, class_name, None)
         if class_inst is not None and inspect.isclass(class_inst) is False:
             # Returns None if given class_name does not match a valid class
             return None
 
         return class_inst
+
+    # ---------------------------------------------------------------------------
+
+    def markdown_convert(self, md):
+        """Return HTML of the given markdown content.
+
+        :param md: (str) A standard-limited markdown content
+        :return: (str) The HTML content
+
+        """
+        if len(HTML) > 0:
+            logging.warning("Markdown to HTML conversion is disabled: {:s}".format(HTML))
+            return ""
+        return self.markdowner.convert(md)
+
+    # ---------------------------------------------------------------------------
+
+    def markdown_to_html(self, content):
+        """Turn a markdown content into HTML.
+
+        :param content: (str) A complex markdown content
+        :return: (str) The HTML content
+
+        """
+        if len(HTML) > 0:
+            logging.warning("Markdown to HTML conversion is disabled: {:s}".format(HTML))
+            return ""
+
+        h = list()
+        code = list()
+        md = list()
+        i = 0
+        all_lines = content.split("\n")
+        while i < len(all_lines):
+            line = all_lines[i]
+
+            # a new code block
+            if line.strip().startswith("```") is True:
+                has_language = len(line.strip()) == 3
+                if len(md) > 0:
+                    h.append(self.markdowner.convert("\n".join(md)))
+                    md = list()
+                line = ""
+                while line.strip().startswith("```") is False:
+                    code.append(line)
+                    i = i + 1
+                    if i > len(all_lines):
+                        break
+                    line = all_lines[i]
+
+                if len(code) > 0:
+                    if has_language is True:
+                        h.append("<pre>")
+                        h.append("\n".join(code))
+                        h.append("</pre>")
+                    else:
+                        h.append(pygments_highlight("\n".join(code), self.lexer, self.formatter))
+                    code = list()
+            else:
+                idx = self.__is_code(line)
+                if idx != -1:
+                    # a code part is starting or is continued.
+                    if len(md) > 0:
+                        h.append(self.markdowner.convert("\n".join(md)))
+                        md = list()
+                    if idx > 0:
+                        code.append(line[idx:])
+                    else:
+                        code.append(line)
+                else:
+                    if len(code) > 0:
+                        h.append(pygments_highlight("\n".join(code), self.lexer, self.formatter))
+                        code = list()
+                    md.append(line)
+            i = i + 1
+
+        if len(code) > 0:
+            h.append(pygments_highlight("\n".join(code), self.lexer, self.formatter))
+        if len(md) > 0:
+            h.append(self.markdowner.convert("\n".join(md)))
+
+        html_result = "\n".join(h)
+        return html_result.replace("<p></p>", "")
+
+    # -----------------------------------------------------------------------
+
+    @staticmethod
+    def __is_code(line):
+        entry = line.strip()
+        if entry.startswith(">>>") is True:
+            return line.index(">") - 1
+        if entry.startswith("> ") is True:
+            return line.index(">") - 1
+
+        return -1
+
+    # -----------------------------------------------------------------------
+
+    def source_to_html(self, source):
+        """Turn a source code content into HTML.
+
+        :param source: (str) The source code content
+        :return: (str) The HTML content
+
+        """
+        if len(HTML) > 0:
+            logging.warning("Source code to HTML conversion is disabled: {:s}".format(HTML))
+            return ""
+        return pygments_highlight(source, self.lexer, self.formatter)
```

## clamming/classparser.py

```diff
@@ -1,30 +1,38 @@
-# clamming.classparser.py
-#
-# This file is part of ClammingPy tool.
-# (C) 2023-2024 Brigitte Bigi, Laboratoire Parole et Langage,
-# Aix-en-Provence, France.
-#
-# Use of this software is governed by the GNU Public License, version 3.
-#
-# ClammingPy is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# ClammingPy is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with ClammingPy. If not, see <http://www.gnu.org/licenses/>.
-#
-# This banner notice must not be removed.
-# ---------------------------------------------------------------------------
+"""
+:filename: clamming.clamsparser.py
+:author: Brigitte Bigi
+:contact: contact@sppas.org
+:summary: Inspect a python class and store relevant information for further doc.
+
+.. _This file is part of ClammingPy: https://clamming.sourceforge.io
+..
+    -------------------------------------------------------------------------
+
+    Copyright (C) 2023-2024 Brigitte Bigi
+    Laboratoire Parole et Langage, Aix-en-Provence, France
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU Affero General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU Affero General Public License for more details.
+
+    You should have received a copy of the GNU Affero General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+    This banner notice must not be removed.
+
+    -------------------------------------------------------------------------
+
+"""
 
 # Python standard libraries
 import inspect
 import ast
 import textwrap
 from typing import Any
 
@@ -60,23 +68,63 @@
             self.__obj_src = textwrap.dedent(inspect.getsource(obj))
             #self.__obj_src = inspect.getsource(obj)
             self.__obj = obj
         except TypeError:
             raise TypeError("Expected a class object for clamming but not a built-in one.")
 
         # Parse and store the information of the class
-        self.obj_clams = self._inspect_class()
-        self.init_clams = self._inspect_constructor()
+        self.__obj_clams = self._inspect_class()
+        self.__init_clams = self._inspect_constructor()
 
         # Parse and store all the documented functions, with their arguments,
         # docstrings and source code
-        self.fct_clams = self._inspect_functions()
+        self.__fct_clams = self._inspect_functions()
+
+    # -----------------------------------------------------------------------
+    # Getters and properties
+    # -----------------------------------------------------------------------
+
+    def get_obj_clams(self) -> ClamInfo:
+        """Parse the information of the class.
+
+        :return: (ClamInfo) Information of the object.
+
+        """
+        return self.__obj_clams
+
+    obj_clams = property(get_obj_clams, None, None)
 
     # -----------------------------------------------------------------------
 
+    def get_init_clams(self) -> ClamInfo:
+        """Inspect constructor of the given object.
+
+        :return: (ClamInfo) Information of the constructor of the object.
+
+        """
+        return self.__init_clams
+
+    init_clams = property(get_init_clams, None, None)
+
+    # -----------------------------------------------------------------------
+
+    def get_fct_clams(self) -> dict:
+        """Inspect functions of the given object.
+
+        :return: (dict) key=function name, value=ClamInfo()
+
+        """
+        return self.__fct_clams
+
+    fct_clams = property(get_fct_clams, None, None)
+
+    # -----------------------------------------------------------------------
+    # Parsers
+    # -----------------------------------------------------------------------
+
     def _inspect_class(self) -> ClamInfo:
         """Inspect constructor of the given object.
 
         """
         class_name = self.__obj.__name__
         tree = ast.parse(self.__obj_src)
         for node in ast.walk(tree):
@@ -84,17 +132,15 @@
                 return ClamInfo(class_name, [], "", ast.get_docstring(node))
 
         return ClamInfo(class_name, [], "", None)
 
     # -----------------------------------------------------------------------
 
     def _inspect_constructor(self) -> ClamInfo:
-        """Inspect constructor of the given object.
-
-        """
+        """Inspect constructor of the given object."""
         try:
             # Get the source code of the Python object into str.
             #init_src = inspect.getsource(self.__obj.__init__)
             init_src = textwrap.dedent(inspect.getsource(self.__obj.__init__))
         except OSError:
             # There's no constructor for the given object.
             return ClamInfo("")
```

## Comparing `clamming/html_export.py` & `clamming/exportoptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,56 @@
-# clamming.html_export.py
-#
-# This file is part of ClammingPy tool.
-# (C) 2023-2024 Brigitte Bigi, Laboratoire Parole et Langage,
-# Aix-en-Provence, France.
-#
-# Use of this software is governed by the GNU Public License, version 3.
-#
-# ClammingPy is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# ClammingPy is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with ClammingPy. If not, see <http://www.gnu.org/licenses/>.
-#
-# This banner notice must not be removed.
-# ---------------------------------------------------------------------------
+"""
+:filename: clamming.exportoptions.py
+:author: Brigitte Bigi
+:contact: contact@sppas.org
+:summary: Store the options and content for an export.
+
+.. _This file is part of ClammingPy: https://clamming.sourceforge.io
+..
+    -------------------------------------------------------------------------
+
+    Copyright (C) 2023-2024 Brigitte Bigi
+    Laboratoire Parole et Langage, Aix-en-Provence, France
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU Affero General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU Affero General Public License for more details.
+
+    You should have received a copy of the GNU Affero General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+    This banner notice must not be removed.
+
+    -------------------------------------------------------------------------
+
+"""
 
 from __future__ import annotations
 from typing import NoReturn
 
 # ---------------------------------------------------------------------------
 
 
-class HTMLDocExport:
-    """Store the options and content for an export to a standalone HTML file.
+class ExportOptions:
+    """Store the options and content for an export to documented files.
 
-    HTMLDocExport is a data class, used to store options and content for exporting
-    a standalone HTML file. It provides methods to set and get various HTML
+    ExportOptions is a data class, used to store options and content for
+    exporting a documented file. It provides methods to set and get various
     information such as software name, copyright, icon, title, favicon, and
     theme. It also allows setting the names of the next and previous classes
-    or modules for generating a table of contents.
+    or modules for generating a table of contents (HTML only).
 
     :example:
-    >>> h = HTMLDocExport()
+    >>> h = ExportOptions()
     >>> h.software = "Clamming"
     >>> h.theme = "light"
     >>> html_head = h.get_head()
     >>> html_nav = h.get_nav()
     >>> html_footer = h.get_footer()
 
     """
@@ -61,33 +69,48 @@
             <link rel="stylesheet" href="{WEXA_STATICS}/css/wexa.css" type="text/css" />
             <link rel="stylesheet" href="{WEXA_STATICS}/css/layout.css" type="text/css" />
             <link rel="stylesheet" href="{WEXA_STATICS}/css/book.css" type="text/css" />
             <link rel="stylesheet" href="{WEXA_STATICS}/css/menu.css" type="text/css" />
             <link rel="stylesheet" href="{WEXA_STATICS}/css/code.css" type="text/css" />
             <link rel="stylesheet" href="{STATICS}/clamming.css" type="text/css" />
 
-            <script src="{WEXA_STATICS}/js/purejs-tools/OnLoadManager.js"  type="application/javascript"></script>
+            <script src="{WEXA_STATICS}/js/purejs-tools/OnLoadManager.js" type="application/javascript"></script>
+            <script src="{WEXA_STATICS}/js/whakerpy/request.js" type="text/javascript"></script>
+            <script src="{WEXA_STATICS}/js/accessibility.js" type="text/javascript"></script>
             <script src="{WEXA_STATICS}/js/book.js" type="application/javascript"></script>
             <script type="application/javascript">
                 OnLoadManager.addLoadFunction(() => {{
                     let book = new Book("main-content");
                     book.fill_table(false);
                 }});
             </script>
        </head>
        
        """
 
-    HTML_BUTTON_SKIP = \
+    HTML_BUTTONS_ACCESSIBILITY = \
         """
-                <a role="button" class="skip" href="#main-content" aria-label="Go to main content">
+            <a role="button" class="skip" href="#main-content" aria-label="Go to main content">
                 Go to main content
-                </a>
+            </a>
+            <nav>
+                <ul>
+                    <li>
+                        <button role="menuitem" class="print-off" onclick="accessibility_manager.switch_contrast_scheme()" aria-label="Change contrast">
+                            <img class="nav-item-img" src="{WEXA_STATICS}/icons/contrast_switcher.jpg" alt="Contrast" id="img-contrast"/>
+                        </button>
+                    </li>
+                    <li>
+                        <button class="print-off" role="menuitem" onclick="accessibility_manager.switch_color_scheme()" aria-label="Change theme color" >
+                            <img class="nav-item-img" src="{WEXA_STATICS}/icons/theme_switcher.png" alt="Theme" id="img-theme"/>
+                        </button>
+                    </li>
+                </ul>
+            </nav>
         """
-
     HTML_FOOTER = \
         """
             <footer>
                 <p class="copyright">{COPYRIGHT}</p>
             </footer>
         """
 
@@ -97,53 +120,70 @@
 
     # About the documented software
     DEFAULT_SOFTWARE = ""
     DEFAULT_COPYRIGHT = ""
     DEFAULT_ICON = ""
     DEFAULT_URL = ""
 
-    # For the created HTML pages
+    # For creating HTML pages
     DEFAULT_WEXA_STATICS = "./wexa_statics"
     DEFAULT_STATICS = "./statics"
     DEFAULT_TITLE = ""
     DEFAULT_FAVICON = "clamming32x32.ico"
     DEFAULT_THEME = "light"
 
     # ----------------------------------------------------------------------------
 
     def __init__(self):
-        """Create an HTML documentation export system for a ClamsPack.
+        """Create a documentation export system for a ClamsPack.
 
         Main functionalities:
 
-        - Store options and content for exporting a standalone HTML file;
+        - Store options and content for exporting a standalone file;
         - Set and get HTML information such as software name, copyright, icon, title, favicon, and theme;
         - Set the names of the next and previous classes or modules for generating a table of contents.
 
         """
+        self.__readme = True
 
         # HTML information
-        self.__software = HTMLDocExport.DEFAULT_SOFTWARE
-        self.__copyright = HTMLDocExport.DEFAULT_COPYRIGHT
-        self.__url = HTMLDocExport.DEFAULT_URL
-        self.__icon = HTMLDocExport.DEFAULT_ICON
-        self.__title = HTMLDocExport.DEFAULT_TITLE
-        self.__favicon = HTMLDocExport.DEFAULT_FAVICON
-        self.__theme = HTMLDocExport.DEFAULT_THEME
-        self.__statics = HTMLDocExport.DEFAULT_STATICS
-        self.__wexa_statics = HTMLDocExport.DEFAULT_WEXA_STATICS
+        self.__software = ExportOptions.DEFAULT_SOFTWARE
+        self.__copyright = ExportOptions.DEFAULT_COPYRIGHT
+        self.__url = ExportOptions.DEFAULT_URL
+        self.__icon = ExportOptions.DEFAULT_ICON
+        self.__title = ExportOptions.DEFAULT_TITLE
+        self.__favicon = ExportOptions.DEFAULT_FAVICON
+        self.__theme = ExportOptions.DEFAULT_THEME
+        self.__statics = ExportOptions.DEFAULT_STATICS
+        self.__wexa_statics = ExportOptions.DEFAULT_WEXA_STATICS
 
         # Previous and next class and module names for the TOC
         self.__next_class = None
         self.__prev_class = None
         self.__next_pack = None
         self.__prev_pack = None
 
     # ----------------------------------------------------------------------------
 
+    def get_add_readme(self) -> bool:
+        """Return whether the README of library is added or not."""
+        return self.__readme
+
+    def set_add_readme(self, readme: bool) -> NoReturn:
+        """Set whether the README of library is added or not.
+
+        :param readme: (bool) whether the README is added or not.
+
+        """
+        self.__readme = bool(readme)
+
+    readme = property(get_add_readme, set_add_readme)
+
+    # ----------------------------------------------------------------------------
+
     def get_software(self) -> str:
         """Return the name of the software."""
         return self.__software
 
     def set_software(self, name: str = DEFAULT_SOFTWARE) -> NoReturn:
         """Set a software name.
 
@@ -400,29 +440,29 @@
 
     # ----------------------------------------------------------------------------
     # Export of the HTML contents
     # ----------------------------------------------------------------------------
 
     def get_head(self) -> str:
         """Return the HTML 'head' of the page."""
-        return HTMLDocExport.HTML_HEAD.format(
+        return ExportOptions.HTML_HEAD.format(
             TITLE=self.__title,
             FAVICON=self.__favicon,
             THEME=self.__theme,
             STATICS=self.__statics,
             WEXA_STATICS=self.__wexa_statics
         )
 
     # ----------------------------------------------------------------------------
 
     def get_header(self) -> str:
         """Return the 'header' of the HTML->body of the page."""
         h = list()
         h.append("    <header>")
-        h.append(HTMLDocExport.HTML_BUTTON_SKIP)
+        h.append(ExportOptions.HTML_BUTTONS_ACCESSIBILITY.format(WEXA_STATICS=self.__wexa_statics))
         if len(self.__software) > 0:
             h.append("    <h1>{SOFTWARE}</h1>".format(SOFTWARE=self.__software))
         if len(self.__icon) > 0:
             h.append('        <p><img class="small-logo" src="{STATICS}/{ICON}" '
                      'alt="Software logo"/></p>'.format(STATICS=self.__statics, ICON=self.__icon))
         if len(self.__url) > 0:
             h.append('        <p><a class="external-link" href="{URL}">{URL}</a></p>'.format(URL=self.__url))
@@ -431,42 +471,42 @@
 
     # ----------------------------------------------------------------------------
 
     def get_nav(self) -> str:
         """Return the 'nav' of the HTML->body of the page."""
         nav = list()
         nav.append("<nav id=\"nav-book\" class=\"side-nav\">")
-        if self.__software == HTMLDocExport.DEFAULT_SOFTWARE:
+        if self.__software == ExportOptions.DEFAULT_SOFTWARE:
             nav.append("    <h1>Documentation</h1>")
         else:
             nav.append("    <h1>{SOFTWARE}</h1>".format(SOFTWARE=self.__software))
         if len(self.__icon) > 0:
             nav.append("    <img class=\"small-logo center\" src=\"{STATICS}/{ICON}\" alt=\"\"/>"
                        "".format(STATICS=self.__statics, ICON=self.__icon))
         if len(self.__url) > 0:
             nav.append('        <p><a class="external-link" href="{URL}">{URL}</a></p>'.format(URL=self.__url))
         nav.append("    <ul>")
-        nav.append(HTMLDocExport.__nav_link("&crarr; Prev. Module", self.__prev_pack))
-        nav.append(HTMLDocExport.__nav_link("&uarr; Prev. Class", self.__prev_class))
-        nav.append(HTMLDocExport.__nav_link("&#8962; Index", "index.html"))
-        nav.append(HTMLDocExport.__nav_link("&darr; Next Class", self.__next_class))
-        nav.append(HTMLDocExport.__nav_link("&rdsh; Next Module", self.__next_pack))
+        nav.append(ExportOptions.__nav_link("&crarr; Prev. Module", self.__prev_pack))
+        nav.append(ExportOptions.__nav_link("&uarr; Prev. Class", self.__prev_class))
+        nav.append(ExportOptions.__nav_link("&#8962; Index", "index.html"))
+        nav.append(ExportOptions.__nav_link("&darr; Next Class", self.__next_class))
+        nav.append(ExportOptions.__nav_link("&rdsh; Next Module", self.__next_pack))
         nav.append("    </ul>")
         nav.append("    <h2>Table of Contents</h2>")
         nav.append("    <ul id=\"toc\"></ul>")
         nav.append("    <hr>")
-        nav.append("    <p><small>Automatically created</small></p><p><small>by <a class=\"external-link\" href=\"https://clamming.sf.net\">Clamming</a></small></p>")
+        nav.append("    <p><small>Automatically created</small></p><p><small>by <a class=\"external-link\" href=\"https://clamming.sf.net\">ClammingPy</a></small></p>")
         nav.append("</nav>")
         return "\n".join(nav)
 
     # -----------------------------------------------------------------------
 
     def get_footer(self) -> str:
         """Return the 'footer' of the HTML->body of the page."""
-        return HTMLDocExport.HTML_FOOTER.format(COPYRIGHT=self.__copyright)
+        return ExportOptions.HTML_FOOTER.format(COPYRIGHT=self.__copyright)
 
     # -----------------------------------------------------------------------
     # Private
     # -----------------------------------------------------------------------
 
     @staticmethod
     def __nav_link(text: str, link: str | None) -> str:
```

## Comparing `ClammingPy-1.7.dist-info/LICENSE` & `ClammingPy-1.8.dist-info/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,82 +1,70 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
+                    GNU AFFERO GENERAL PUBLIC LICENSE
+                       Version 3, 19 November 2007
 
- Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
  Everyone is permitted to copy and distribute verbatim copies
  of this license document, but changing it is not allowed.
 
                             Preamble
 
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
+  The GNU Affero General Public License is a free, copyleft license for
+software and other kinds of works, specifically designed to ensure
+cooperation with the community in the case of network server software.
 
   The licenses for most software and other practical works are designed
 to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
+our General Public Licenses are intended to guarantee your freedom to
 share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
+software for all its users.
 
   When we speak of free software, we are referring to freedom, not
 price.  Our General Public Licenses are designed to make sure that you
 have the freedom to distribute copies of free software (and charge for
 them if you wish), that you receive source code or can get it if you
 want it, that you can change the software or use pieces of it in new
 free programs, and that you know you can do these things.
 
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
+  Developers that use our General Public Licenses protect your rights
+with two steps: (1) assert copyright on the software, and (2) offer
+you this License which gives you legal permission to copy, distribute
+and/or modify the software.
+
+  A secondary benefit of defending all users' freedom is that
+improvements made in alternate versions of the program, if they
+receive widespread use, become available for other developers to
+incorporate.  Many developers of free software are heartened and
+encouraged by the resulting cooperation.  However, in the case of
+software used on network servers, this result may fail to come about.
+The GNU General Public License permits making a modified version and
+letting the public access it on a server without ever releasing its
+source code to the public.
+
+  The GNU Affero General Public License is designed specifically to
+ensure that, in such cases, the modified source code becomes available
+to the community.  It requires the operator of a network server to
+provide the source code of the modified version running there to the
+users of that server.  Therefore, public use of a modified version, on
+a publicly accessible server, gives the public access to the source
+code of the modified version.
+
+  An older license, called the Affero General Public License and
+published by Affero, was designed to accomplish similar goals.  This is
+a different license, not a version of the Affero GPL, but Affero has
+released a new version of the Affero GPL which permits relicensing under
+this license.
 
   The precise terms and conditions for copying, distribution and
 modification follow.
 
                        TERMS AND CONDITIONS
 
   0. Definitions.
 
-  "This License" refers to version 3 of the GNU General Public License.
+  "This License" refers to version 3 of the GNU Affero General Public License.
 
   "Copyright" also means copyright-like laws that apply to other kinds of
 works, such as semiconductor masks.
 
   "The Program" refers to any copyrightable work licensed under this
 License.  Each licensee is addressed as "you".  "Licensees" and
 "recipients" may be individuals or organizations.
@@ -545,43 +533,53 @@
 covered work so as to satisfy simultaneously your obligations under this
 License and any other pertinent obligations, then as a consequence you may
 not convey it at all.  For example, if you agree to terms that obligate you
 to collect a royalty for further conveying from those to whom you convey
 the Program, the only way you could satisfy both those terms and this
 License would be to refrain entirely from conveying the Program.
 
-  13. Use with the GNU Affero General Public License.
+  13. Remote Network Interaction; Use with the GNU General Public License.
+
+  Notwithstanding any other provision of this License, if you modify the
+Program, your modified version must prominently offer all users
+interacting with it remotely through a computer network (if your version
+supports such interaction) an opportunity to receive the Corresponding
+Source of your version by providing access to the Corresponding Source
+from a network server at no charge, through some standard or customary
+means of facilitating copying of software.  This Corresponding Source
+shall include the Corresponding Source for any work covered by version 3
+of the GNU General Public License that is incorporated pursuant to the
+following paragraph.
 
   Notwithstanding any other provision of this License, you have
 permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
+under version 3 of the GNU General Public License into a single
 combined work, and to convey the resulting work.  The terms of this
 License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
+but the work with which it is combined will remain governed by version
+3 of the GNU General Public License.
 
   14. Revised Versions of this License.
 
   The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
+the GNU Affero General Public License from time to time.  Such new versions
+will be similar in spirit to the present version, but may differ in detail to
 address new problems or concerns.
 
   Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
+Program specifies that a certain numbered version of the GNU Affero General
 Public License "or any later version" applies to it, you have the
 option of following the terms and conditions either of that numbered
 version or of any later version published by the Free Software
 Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
+GNU Affero General Public License, you may choose any version ever published
 by the Free Software Foundation.
 
   If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
+versions of the GNU Affero General Public License can be used, that proxy's
 public statement of acceptance of a version permanently authorizes you
 to choose that version for the Program.
 
   Later license versions may give you additional or different
 permissions.  However, no additional obligations are imposed on any
 author or copyright holder as a result of your choosing to follow a
 later version.
@@ -631,44 +629,33 @@
 state the exclusion of warranty; and each file should have at least
 the "copyright" line and a pointer to where the full notice is found.
 
     <one line to give the program's name and a brief idea of what it does.>
     Copyright (C) <year>  <name of author>
 
     This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
+    it under the terms of the GNU Affero General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
 
     This program is distributed in the hope that it will be useful,
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
+    GNU Affero General Public License for more details.
 
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <http://www.gnu.org/licenses/>.
+    You should have received a copy of the GNU Affero General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 Also add information on how to contact you by electronic and paper mail.
 
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
+  If your software can interact with users remotely through a computer
+network, you should also make sure that it provides a way for users to
+get its source.  For example, if your program is a web application, its
+interface could display a "Source" link that leads users to an archive
+of the code.  There are many ways you could offer source, and different
+solutions will be better for different programs; see section 13 for the
+specific requirements.
 
   You should also get your employer (if you work as a programmer) or school,
 if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<http://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<http://www.gnu.org/philosophy/why-not-lgpl.html>.
+For more information on this, and how to apply and follow the GNU AGPL, see
+<https://www.gnu.org/licenses/>.
```

## Comparing `ClammingPy-1.7.dist-info/METADATA` & `ClammingPy-1.8.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,87 +1,75 @@
 Metadata-Version: 2.1
 Name: ClammingPy
-Version: 1.7
+Version: 1.8
 Summary: Light Python-API Documentation in Markdown and HTML
 Author-email: Brigitte Bigi <contact@sppas.org>
-License: GNU GENERAL PUBLIC LICENSE
-                               Version 3, 29 June 2007
+License: GNU AFFERO GENERAL PUBLIC LICENSE
+                               Version 3, 19 November 2007
         
-         Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
+         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
         
                                     Preamble
         
-          The GNU General Public License is a free, copyleft license for
-        software and other kinds of works.
+          The GNU Affero General Public License is a free, copyleft license for
+        software and other kinds of works, specifically designed to ensure
+        cooperation with the community in the case of network server software.
         
           The licenses for most software and other practical works are designed
         to take away your freedom to share and change the works.  By contrast,
-        the GNU General Public License is intended to guarantee your freedom to
+        our General Public Licenses are intended to guarantee your freedom to
         share and change all versions of a program--to make sure it remains free
-        software for all its users.  We, the Free Software Foundation, use the
-        GNU General Public License for most of our software; it applies also to
-        any other work released this way by its authors.  You can apply it to
-        your programs, too.
+        software for all its users.
         
           When we speak of free software, we are referring to freedom, not
         price.  Our General Public Licenses are designed to make sure that you
         have the freedom to distribute copies of free software (and charge for
         them if you wish), that you receive source code or can get it if you
         want it, that you can change the software or use pieces of it in new
         free programs, and that you know you can do these things.
         
-          To protect your rights, we need to prevent others from denying you
-        these rights or asking you to surrender the rights.  Therefore, you have
-        certain responsibilities if you distribute copies of the software, or if
-        you modify it: responsibilities to respect the freedom of others.
-        
-          For example, if you distribute copies of such a program, whether
-        gratis or for a fee, you must pass on to the recipients the same
-        freedoms that you received.  You must make sure that they, too, receive
-        or can get the source code.  And you must show them these terms so they
-        know their rights.
-        
-          Developers that use the GNU GPL protect your rights with two steps:
-        (1) assert copyright on the software, and (2) offer you this License
-        giving you legal permission to copy, distribute and/or modify it.
-        
-          For the developers' and authors' protection, the GPL clearly explains
-        that there is no warranty for this free software.  For both users' and
-        authors' sake, the GPL requires that modified versions be marked as
-        changed, so that their problems will not be attributed erroneously to
-        authors of previous versions.
-        
-          Some devices are designed to deny users access to install or run
-        modified versions of the software inside them, although the manufacturer
-        can do so.  This is fundamentally incompatible with the aim of
-        protecting users' freedom to change the software.  The systematic
-        pattern of such abuse occurs in the area of products for individuals to
-        use, which is precisely where it is most unacceptable.  Therefore, we
-        have designed this version of the GPL to prohibit the practice for those
-        products.  If such problems arise substantially in other domains, we
-        stand ready to extend this provision to those domains in future versions
-        of the GPL, as needed to protect the freedom of users.
-        
-          Finally, every program is threatened constantly by software patents.
-        States should not allow patents to restrict development and use of
-        software on general-purpose computers, but in those that do, we wish to
-        avoid the special danger that patents applied to a free program could
-        make it effectively proprietary.  To prevent this, the GPL assures that
-        patents cannot be used to render the program non-free.
+          Developers that use our General Public Licenses protect your rights
+        with two steps: (1) assert copyright on the software, and (2) offer
+        you this License which gives you legal permission to copy, distribute
+        and/or modify the software.
+        
+          A secondary benefit of defending all users' freedom is that
+        improvements made in alternate versions of the program, if they
+        receive widespread use, become available for other developers to
+        incorporate.  Many developers of free software are heartened and
+        encouraged by the resulting cooperation.  However, in the case of
+        software used on network servers, this result may fail to come about.
+        The GNU General Public License permits making a modified version and
+        letting the public access it on a server without ever releasing its
+        source code to the public.
+        
+          The GNU Affero General Public License is designed specifically to
+        ensure that, in such cases, the modified source code becomes available
+        to the community.  It requires the operator of a network server to
+        provide the source code of the modified version running there to the
+        users of that server.  Therefore, public use of a modified version, on
+        a publicly accessible server, gives the public access to the source
+        code of the modified version.
+        
+          An older license, called the Affero General Public License and
+        published by Affero, was designed to accomplish similar goals.  This is
+        a different license, not a version of the Affero GPL, but Affero has
+        released a new version of the Affero GPL which permits relicensing under
+        this license.
         
           The precise terms and conditions for copying, distribution and
         modification follow.
         
                                TERMS AND CONDITIONS
         
           0. Definitions.
         
-          "This License" refers to version 3 of the GNU General Public License.
+          "This License" refers to version 3 of the GNU Affero General Public License.
         
           "Copyright" also means copyright-like laws that apply to other kinds of
         works, such as semiconductor masks.
         
           "The Program" refers to any copyrightable work licensed under this
         License.  Each licensee is addressed as "you".  "Licensees" and
         "recipients" may be individuals or organizations.
@@ -550,43 +538,53 @@
         covered work so as to satisfy simultaneously your obligations under this
         License and any other pertinent obligations, then as a consequence you may
         not convey it at all.  For example, if you agree to terms that obligate you
         to collect a royalty for further conveying from those to whom you convey
         the Program, the only way you could satisfy both those terms and this
         License would be to refrain entirely from conveying the Program.
         
-          13. Use with the GNU Affero General Public License.
+          13. Remote Network Interaction; Use with the GNU General Public License.
+        
+          Notwithstanding any other provision of this License, if you modify the
+        Program, your modified version must prominently offer all users
+        interacting with it remotely through a computer network (if your version
+        supports such interaction) an opportunity to receive the Corresponding
+        Source of your version by providing access to the Corresponding Source
+        from a network server at no charge, through some standard or customary
+        means of facilitating copying of software.  This Corresponding Source
+        shall include the Corresponding Source for any work covered by version 3
+        of the GNU General Public License that is incorporated pursuant to the
+        following paragraph.
         
           Notwithstanding any other provision of this License, you have
         permission to link or combine any covered work with a work licensed
-        under version 3 of the GNU Affero General Public License into a single
+        under version 3 of the GNU General Public License into a single
         combined work, and to convey the resulting work.  The terms of this
         License will continue to apply to the part which is the covered work,
-        but the special requirements of the GNU Affero General Public License,
-        section 13, concerning interaction through a network will apply to the
-        combination as such.
+        but the work with which it is combined will remain governed by version
+        3 of the GNU General Public License.
         
           14. Revised Versions of this License.
         
           The Free Software Foundation may publish revised and/or new versions of
-        the GNU General Public License from time to time.  Such new versions will
-        be similar in spirit to the present version, but may differ in detail to
+        the GNU Affero General Public License from time to time.  Such new versions
+        will be similar in spirit to the present version, but may differ in detail to
         address new problems or concerns.
         
           Each version is given a distinguishing version number.  If the
-        Program specifies that a certain numbered version of the GNU General
+        Program specifies that a certain numbered version of the GNU Affero General
         Public License "or any later version" applies to it, you have the
         option of following the terms and conditions either of that numbered
         version or of any later version published by the Free Software
         Foundation.  If the Program does not specify a version number of the
-        GNU General Public License, you may choose any version ever published
+        GNU Affero General Public License, you may choose any version ever published
         by the Free Software Foundation.
         
           If the Program specifies that a proxy can decide which future
-        versions of the GNU General Public License can be used, that proxy's
+        versions of the GNU Affero General Public License can be used, that proxy's
         public statement of acceptance of a version permanently authorizes you
         to choose that version for the Program.
         
           Later license versions may give you additional or different
         permissions.  However, no additional obligations are imposed on any
         author or copyright holder as a result of your choosing to follow a
         later version.
@@ -636,128 +634,128 @@
         state the exclusion of warranty; and each file should have at least
         the "copyright" line and a pointer to where the full notice is found.
         
             <one line to give the program's name and a brief idea of what it does.>
             Copyright (C) <year>  <name of author>
         
             This program is free software: you can redistribute it and/or modify
-            it under the terms of the GNU General Public License as published by
+            it under the terms of the GNU Affero General Public License as published by
             the Free Software Foundation, either version 3 of the License, or
             (at your option) any later version.
         
             This program is distributed in the hope that it will be useful,
             but WITHOUT ANY WARRANTY; without even the implied warranty of
             MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-            GNU General Public License for more details.
+            GNU Affero General Public License for more details.
         
-            You should have received a copy of the GNU General Public License
-            along with this program.  If not, see <http://www.gnu.org/licenses/>.
+            You should have received a copy of the GNU Affero General Public License
+            along with this program.  If not, see <https://www.gnu.org/licenses/>.
         
         Also add information on how to contact you by electronic and paper mail.
         
-          If the program does terminal interaction, make it output a short
-        notice like this when it starts in an interactive mode:
-        
-            <program>  Copyright (C) <year>  <name of author>
-            This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-            This is free software, and you are welcome to redistribute it
-            under certain conditions; type `show c' for details.
-        
-        The hypothetical commands `show w' and `show c' should show the appropriate
-        parts of the General Public License.  Of course, your program's commands
-        might be different; for a GUI interface, you would use an "about box".
+          If your software can interact with users remotely through a computer
+        network, you should also make sure that it provides a way for users to
+        get its source.  For example, if your program is a web application, its
+        interface could display a "Source" link that leads users to an archive
+        of the code.  There are many ways you could offer source, and different
+        solutions will be better for different programs; see section 13 for the
+        specific requirements.
         
           You should also get your employer (if you work as a programmer) or school,
         if any, to sign a "copyright disclaimer" for the program, if necessary.
-        For more information on this, and how to apply and follow the GNU GPL, see
-        <http://www.gnu.org/licenses/>.
-        
-          The GNU General Public License does not permit incorporating your program
-        into proprietary programs.  If your program is a subroutine library, you
-        may consider it more useful to permit linking proprietary applications with
-        the library.  If this is what you want to do, use the GNU Lesser General
-        Public License instead of this License.  But first, please read
-        <http://www.gnu.org/philosophy/why-not-lgpl.html>.
+        For more information on this, and how to apply and follow the GNU AGPL, see
+        <https://www.gnu.org/licenses/>.
         
 Project-URL: Homepage, https://clamming.sf.net/
 Keywords: python,class,module,documentation,doc,docstring,markdown,html,reST,epydoc
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
+Requires-Dist: pygments
+Requires-Dist: markdown2
 Provides-Extra: dev
 Requires-Dist: pylint ~=2.14.0 ; extra == 'dev'
 Requires-Dist: toml ~=0.10.2 ; extra == 'dev'
 Provides-Extra: tests
 Requires-Dist: coverage ~=7.3.0 ; extra == 'tests'
-Requires-Dist: selenium ~=4.13.0 ; extra == 'tests'
 Requires-Dist: python-dotenv ~=1.0.0 ; extra == 'tests'
 
-# ClammingPy - Light Python-API Documentation in Markdown and HTML
+# ClammingPy Description
 
 ## Overview
 
-`ClammingPy` is an open-source library useful to export a Python `class` into
-a Markdown or HTML file, for documentation purpose. `ClammingPy` mainly
-supports reStructured format, however, docstrings are analyzed with 
-**flexibility rather than completeness...**
+> ClammingPy is a Light Python-API Documentation in Markdown and HTML
+
+### Typical use
+
+You have a Python API you documented with docstrings, and you want to share documentation in either Markdown or HTML.
+ClammingPy is the documentation generator you may need: it is generating Markdown or HTML from the docstrings within the source code of any Python library.
+
+> ClammingPy generates HTML-5 with a high level of WCAG 2.1 conformity.
+
+### Features
 
-> Both ReST and Epydoc field styles are supported. It means that either
-> :field: or @field: can be used indifferently, with upper- or lower- cases.
+Python modules are usually documented using docstrings. They typically use plain text markup formats such as reStructuredText (reST, the markup used for writing the official Python documentation) and/or Markdown.
+`ClammingPy` is a Python, free, open-source, self-hosted library to export a Python class or module into a Markdown and/or HTML files, for documentation purpose. Contrariwise to other documentation tools, docstrings are analyzed with **flexibility rather than completeness...**
 
-Two very useful non-standard "field list" items are added: `:example:` 
-and `:code:`. Finally, some variants in field names are supported:
+> Both ReST and Epydoc field styles are supported. It means that either ':field:' or '@field:' can be used indifferently, with upper- or lower- cases.
+
+Two very useful reST non-standard field items can also be used in the docstrings: `:example:` and `:code:`. 
+Finally, some variants in field names are supported:
 
 - `:return:` or `:returns:` are both interpreted the same way;
-- `:raise:` or `:raises:` or `:catch:` or `:except:` are all interpreted 
-the same way.
+- `:raise:` or `:raises:` or `:catch:` or `:except:` are all interpreted the same way.
+
+
+### Main advantages
 
-> Notice that we expect to generate HTML-5 with a high level of WCAG 2.1 conformity.
+- easily customizable: it's a pure python library in Object-Oriented Programming
+- open-source: easily add new features and functionalities 
+- scalable: no limit to support numerous modules
+- inclusive: the documentation is highly WCAG 2.1 compliant
 
 
 ## Install ClammingPy
 
-ClammingPy requires Whakerexa to be installed; it can be downloaded from:
-<https://whakerexa.sf.net>. Unpack it into the ClammingPy package.
+Get it here: <https://sourceforge.net/projects/clamming/>.
+
+ClammingPy requires Whakerexa to be installed; it can be downloaded from: <https://whakerexa.sf.net>. Get its documentation here: <https://whakerexa.sourceforge.io>.
+Unpack it into the `ClammingPy/docs` folder.
 
 ### From the repo:
 
 Download the repository and unpack it. ClammingPy tool includes the following folders and files:
 
 1. `clamming`: the source code of `ClammingPy` library
 2. `docs`: the documentation of clamming library in HTML, already including "wexa_statics".
 3. `tests`: unittest of `Clamming` library
 4. `sample`: a sample class `Vehicle` to illustrate `clamming` use
 5. `makedoc.py`: create the ClammingPy documentation, using `clamming` library
 6. `etc`: etcetera!
 
-
 ### From the package:
 
 Install it in your python environment from the local wheel with:
 
 ```bash
 > python -m pip install dist/<clamming.whl>
 ```
 
-## License
-
-This is the implementation of the `ClammingPy` library, under the terms of the GNU General Public License version 3.
 
+## Quick start
 
-# Usage
-
-## Documenting a single class
+### Documenting a single class
 
 The `sample` folder contains a Python class example and the simplest solution to get access to the documentation either in Markdown or HTML. The `Vehicle` class is illustrating the supported format and its flexibility. Try it with:
 
 ```bash
 > cd sample
 > python makedoc_vehicle.py > vehicle.html
 > python makedoc_vehicle.py --md > vehicle.md
@@ -783,15 +781,15 @@
 >>> import Vehicle  # Or any other Python class to be documented
 >>> parser = clamming.ClammingClassParser(Vehicle)
 >>> clams = clamming.ClamsClass(parser)
 >>> print(clams.html())
 >>> print(clams.markdown())
 ```
 
-## Documenting all classes of a package
+### Documenting all classes of a module
 
 Below are two examples with the main program:
 ```bash
 > python main.py -m clamming > clamming.html
 > python main.py -m http.server --md | grep "### Class "
 ### Class `HTTPServer`
 ### Class `ThreadingHTTPServer`
@@ -809,56 +807,80 @@
 >>> print(clams_pack.markdown())
 >>> print(clams_pack.html())
 ```
 
 Here is a summary of the main steps to generate an HTML documentation, in a bunch of HTML files:
 
 ```python
->>> import clamming
->>> # Options for HTML exportation
->>> html_export = clamming.HTMLDocExport()
->>> html_export.software = 'ClammingPy ' + clamming.__version__
->>> # Create an HTML page for each class of the module
->>> clams_pack = clamming.ClamsPack(clamming)
->>> clams_pack.html_export_clams("docs", html_export)
+>> > import clamming
+>> >  # Options for HTML exportation
+>> > html_export = clamming.ExportOptions()
+>> > html_export.software = 'ClammingPy ' + clamming.__version__
+>> >  # Create an HTML page for each class of the module
+>> > clams_pack = clamming.ClamsPack(clamming)
+>> > clams_pack.html_export_clams("docs", html_export)
 ```
 
-## Documenting all classes of a list of packages
+### Documenting all classes of a list of modules
 
 There is an all-in-one function to generate the HTML documentation of a list of packages. It requires to define the followings:
 
 1. The list of ClamsPack instances of the modules to be documented;
 2. The HTMLDocExport allowing to fix the HTML options for files exportation.
 
 ```python
->>> import clamming
->>> # List of modules to be documented.
->>> packages = list()
->>> packages.append(clamming.ClamsPack(clamming))
->>> # Options for HTML exportation
->>> html_export = clamming.HTMLDocExport()
->>> html_export.wexa_statics = '../Whakerexa-0.2/wexa_statics'
->>> html_export.software = 'ClammingPy ' + clamming.__version__
->>> # Export documentation to HTML files into the "docs" folder.
->>> clamming.ClamsPack.html_export_packages(packages, "docs", html_export)
->>> # Export documentation to Markdown files into the "docs" folder.
->>> clamming.ClamsPack.markdown_export_packages(packages, "docs", html_export)
+>> > import clamming
+>> >  # List of modules to be documented.
+>> > packages = list()
+>> > packages.append(clamming)
+>> >  # Options for HTML exportation
+>> > html_export = clamming.ExportOptions()
+>> > html_export.wexa_statics = '../Whakerexa-0.4/wexa_statics'
+>> > html_export.software = 'ClammingPy ' + clamming.__version__
+>> >  # Export documentation to HTML files into the "docs" folder.
+>> > m = clamming.ClamsModules(packages)
+>> > m.html_export_packages("docs", html_export)
+>> >  # Export documentation to Markdown files into the "docs" folder.
+>> > m.markdown_export_packages("docs")
 ```
 
 See `makedoc.py` Python script for details.
 
 > See the ClammingPy documentation in `docs` folder for extended usages.
 
 
-## Projects using `ClammingPy`
+## Projects using ClammingPy
 
 - WhakerPy: <https://whakerpy.sf.net>
+- WhintPy: <https://whintpy.sourceforge.io>
 - AudiooPy: <https://audioopy.sf.net>
 - PyMancala: <https://pymancala.sf.net>
-- SPPAS: <https://sppas.org>
+- SPPAS: <https://sppas.org/api/index.html>
 - *contact the author if you want to add a project here*
 
 
-# Author/Copyright
+## Help / How to contribute
+
+If you plan to contribute to the code or to report a bug, please send an e-mail to the author.
+Any and all constructive comments are welcome.
+
+
+## License/Copyright
+
+See the accompanying LICENSE and AUTHORS files for the full list of contributors.
+
+Copyright (C) 2023-2024  - [Brigitte Bigi](https://sppas.org/bigi/) - <contact@sppas.org>
+Laboratoire Parole et Langage, Aix-en-Provence, France
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU Affero General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU Affero General Public License for more details.
+
+You should have received a copy of the GNU Affero General Public License
+along with this program. If not, see <https://www.gnu.org/licenses/>.
 
-Copyright (C) 2023-2024 - [Brigitte Bigi](https://sppas.org/bigi/) - 
-<contact@sppas.org>, Laboratoire Parole et Langage, Aix-en-Provence, France.
```

## Comparing `ClammingPy-1.7.dist-info/RECORD` & `ClammingPy-1.8.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-clamming/__init__.py,sha256=ENa5WZptKJLTLoJte1T8HdahVcIriFpgdrkRD3uOk_o,572
-clamming/claminfo.py,sha256=vBAktH7emcitIk79LQZtvH2SL_D1Gx6URzKY8ykLcQU,5527
-clamming/claminfomd.py,sha256=c6XicQ903j3vNPEumk5zSEcv30H2QyF9CQ-REqJrhsU,17620
-clamming/clamsclass.py,sha256=sNshG52yN6ennn0Oy09kdhAh-IjL2JUVQkrm1mdIcmA,13875
-clamming/clamspack.py,sha256=Q7H_3244MfHC_WeW5aPLqgP9QK5RRsIAm8s1S-TWtmA,12849
-clamming/clamutils.py,sha256=q_UA8cjbryAMYjNwJpi8_toMQZ1FntsS7npz8BVDsrs,2441
-clamming/classparser.py,sha256=Ea6Pyv8I5njnCZh97q8mT_f0LWS4FRZztrM28yRehPY,5232
-clamming/html_export.py,sha256=VnEf7BTPWs8d7DDDYiXT4S_Fxmnl0XYyP-WoRWk0K9I,18785
-ClammingPy-1.7.dist-info/AUTHORS,sha256=3g6U4D_SDnBcnY-H9tBdsM0wj4KMtHrOC-zdUp9_V1M,742
-ClammingPy-1.7.dist-info/LICENSE,sha256=jOtLnuWt7d5Hsx6XXB2QxzrSe2sWWh3NgMfFRetluQM,35147
-ClammingPy-1.7.dist-info/METADATA,sha256=TPAuDyg1OOE4Z9seRTHLbPXCS0WvG2xbHa1LQpSYgzk,47059
-ClammingPy-1.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-ClammingPy-1.7.dist-info/top_level.txt,sha256=OQf97OKpmnkcWYrLkZCQBOteq0d89GkQ-Ux1gmidsn4,9
-ClammingPy-1.7.dist-info/RECORD,,
+clamming/__init__.py,sha256=b7elN4DjINQujL_BOV4AScXvDWtcw1-YQ7tcz27C0LI,1832
+clamming/claminfo.py,sha256=UcEL-XWSoRLBNAcc5TeE7s2NPkdYsf5cafH98_4Z7AA,5728
+clamming/claminfomd.py,sha256=Jv_AGTO4Ni9eHn1tRhpNBeTUKvKSsU8YkUliqcu6K2A,17906
+clamming/clamsclass.py,sha256=BdPIv-tT_h1Q7A5dIN_obPPLeFd_p8JlTy4ewdj9tWo,12017
+clamming/clamsmodules.py,sha256=JavLxr-Zu8nb8Bwragx8mSXg_qBGTTqWWXxSxQm9EWI,6815
+clamming/clamspack.py,sha256=lf1N7PAKMWm1XuQQky_yxUkCxDb04SsjBl9OUUPyhPY,11824
+clamming/clamutils.py,sha256=amoC3fIAkJvBvEoRSBWQ-K83DGlkMSv7HGq2df8P2qA,7778
+clamming/classparser.py,sha256=vZzz8EavLORfJse8ZcaJvODhqYKlTYTT6Kfq-4y4Rwo,6670
+clamming/exportoptions.py,sha256=le4ckKwts7ngnMVsWPVPseURBbjjlN7HcEGcDO6LJNk,20596
+ClammingPy-1.8.dist-info/AUTHORS,sha256=J-KN-3Yie3kgPuONEWzA3GHOue34J64Heu8TLiX0PoE,1856
+ClammingPy-1.8.dist-info/LICENSE,sha256=DZak_2itbUtvHzD3E7GNUYSRK6jdOJ-GqncQ2weavLA,34523
+ClammingPy-1.8.dist-info/METADATA,sha256=WNKtfAjzlcXAaPHNblXT3jv9e5c01J0H4_NlC77DkoE,48117
+ClammingPy-1.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+ClammingPy-1.8.dist-info/top_level.txt,sha256=OQf97OKpmnkcWYrLkZCQBOteq0d89GkQ-Ux1gmidsn4,9
+ClammingPy-1.8.dist-info/RECORD,,
```

