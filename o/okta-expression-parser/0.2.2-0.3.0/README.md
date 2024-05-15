# Comparing `tmp/okta_expression_parser-0.2.2.tar.gz` & `tmp/okta_expression_parser-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "okta_expression_parser-0.2.2.tar", max compression
+gzip compressed data, was "okta_expression_parser-0.3.0.tar", max compression
```

## Comparing `okta_expression_parser-0.2.2.tar` & `okta_expression_parser-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       25 2024-02-07 18:36:50.904598 okta_expression_parser-0.2.2/README.md
--rw-r--r--   0        0        0        0 2024-01-24 17:39:56.968382 okta_expression_parser-0.2.2/okta_expression_parser/__init__.py
--rw-r--r--   0        0        0      153 2024-02-14 17:13:57.668654 okta_expression_parser-0.2.2/okta_expression_parser/expression_classes/__init__.py
--rw-r--r--   0        0        0     1737 2024-02-14 17:13:57.680267 okta_expression_parser-0.2.2/okta_expression_parser/expression_classes/arrays.py
--rw-r--r--   0        0        0      344 2024-02-14 14:53:37.731479 okta_expression_parser-0.2.2/okta_expression_parser/expression_classes/convert.py
--rw-r--r--   0        0        0      818 2024-02-14 17:13:57.677989 okta_expression_parser-0.2.2/okta_expression_parser/expression_classes/groups.py
--rw-r--r--   0        0        0    22766 2024-02-14 17:13:57.838616 okta_expression_parser-0.2.2/okta_expression_parser/expression_classes/iso3166convert.py
--rw-r--r--   0        0        0     3259 2024-05-13 17:46:42.187846 okta_expression_parser-0.2.2/okta_expression_parser/expression_classes/string.py
--rw-r--r--   0        0        0     1447 2024-02-14 15:49:07.639688 okta_expression_parser-0.2.2/okta_expression_parser/lexer.py
--rw-r--r--   0        0        0     9565 2024-05-13 19:08:57.708638 okta_expression_parser-0.2.2/okta_expression_parser/parser.py
--rw-r--r--   0        0        0      561 2024-05-13 19:10:13.534078 okta_expression_parser-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      505 1970-01-01 00:00:00.000000 okta_expression_parser-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       25 2024-02-07 18:36:50.904598 okta_expression_parser-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-01-24 17:39:56.968382 okta_expression_parser-0.3.0/okta_expression_parser/__init__.py
+-rw-r--r--   0        0        0      153 2024-02-14 17:13:57.668654 okta_expression_parser-0.3.0/okta_expression_parser/expression_classes/__init__.py
+-rw-r--r--   0        0        0     1737 2024-02-14 17:13:57.680267 okta_expression_parser-0.3.0/okta_expression_parser/expression_classes/arrays.py
+-rw-r--r--   0        0        0      344 2024-02-14 14:53:37.731479 okta_expression_parser-0.3.0/okta_expression_parser/expression_classes/convert.py
+-rw-r--r--   0        0        0      818 2024-02-14 17:13:57.677989 okta_expression_parser-0.3.0/okta_expression_parser/expression_classes/groups.py
+-rw-r--r--   0        0        0    22766 2024-02-14 17:13:57.838616 okta_expression_parser-0.3.0/okta_expression_parser/expression_classes/iso3166convert.py
+-rw-r--r--   0        0        0     3259 2024-05-13 17:46:42.187846 okta_expression_parser-0.3.0/okta_expression_parser/expression_classes/string.py
+-rw-r--r--   0        0        0     1529 2024-05-15 19:10:10.059731 okta_expression_parser-0.3.0/okta_expression_parser/lexer.py
+-rw-r--r--   0        0        0    11021 2024-05-15 19:52:03.971338 okta_expression_parser-0.3.0/okta_expression_parser/parser.py
+-rw-r--r--   0        0        0      561 2024-05-15 19:10:29.554666 okta_expression_parser-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      505 1970-01-01 00:00:00.000000 okta_expression_parser-0.3.0/PKG-INFO
```

### Comparing `okta_expression_parser-0.2.2/okta_expression_parser/expression_classes/arrays.py` & `okta_expression_parser-0.3.0/okta_expression_parser/expression_classes/arrays.py`

 * *Files identical despite different names*

### Comparing `okta_expression_parser-0.2.2/okta_expression_parser/expression_classes/groups.py` & `okta_expression_parser-0.3.0/okta_expression_parser/expression_classes/groups.py`

 * *Files identical despite different names*

### Comparing `okta_expression_parser-0.2.2/okta_expression_parser/expression_classes/iso3166convert.py` & `okta_expression_parser-0.3.0/okta_expression_parser/expression_classes/iso3166convert.py`

 * *Files identical despite different names*

### Comparing `okta_expression_parser-0.2.2/okta_expression_parser/expression_classes/string.py` & `okta_expression_parser-0.3.0/okta_expression_parser/expression_classes/string.py`

 * *Files identical despite different names*

### Comparing `okta_expression_parser-0.2.2/okta_expression_parser/lexer.py` & `okta_expression_parser-0.3.0/okta_expression_parser/lexer.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,14 +20,16 @@
         LT,
         EQ,
         AND,
         OR,
         NOT,
         NULL,
         BOOL,
+        COLON,
+        QUESTION_MARK,
         MEMBEROF,
         MEMBEROFANY,
         USER,
         CLASS,
     }
 
     # Set of literal characters
@@ -45,14 +47,16 @@
     LTE = "<="
     OR = r"or|OR|Or"
     EQ = r"(==|eq|EQ|Eq)"
     BOOL = r"(true|false|True|False|TRUE|FALSE)"
     MEMBEROFANY = "isMemberOfAnyGroup"
     MEMBEROF = "isMemberOfGroup"
     USER = r"user\b"
+    COLON = r"\:"
+    QUESTION_MARK = r"\?"
 
     NULL = r"null|NULL|Null"
     CLASS = r"String|Arrays|Convert|Iso3166Convert|Groups"
     INT = r"\d+"
     STRING = r""""([^"\\]*(\\.[^"\\]*)*)"|\'([^\'\\]*(\\.[^\'\\]*)*)\'|''|\"\""""
     NAME = r"[a-zA-Z_][a-zA-Z0-9\-_]*"
```

### Comparing `okta_expression_parser-0.2.2/okta_expression_parser/parser.py` & `okta_expression_parser-0.3.0/okta_expression_parser/parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 
 from . import expression_classes as _default_expression_classes
 from .expression_classes.arrays import _ArrayType
 from .lexer import ExpressionLexer
 
 
 class ExpressionParser(sly.Parser):
-    if debug_file := environ.get("OKTA_EXPRESSION_PARSER_LOG_FILE"):
-        #: Writes grammar rules to a file for debugging
-        debugfile: str = environ.get(debug_file)
+    #: Writes grammar rules to a file for debugging
+    debugfile = environ.get("OKTA_EXPRESSION_PARSER_LOG_FILE")
 
     #: Gets the token list from the lexer (required)
     tokens: Sequence = ExpressionLexer.tokens
 
     #: Defines precendence of operators
     precedence = (
         ("left", OR),  # noqa: 821
@@ -60,14 +59,20 @@
 
         if log_to_stdout:
             self.logger.addHandler(logging.StreamHandler(stream=stdout))
 
     def parse(self, expression: str):
         return super().parse(ExpressionLexer().tokenize(expression))
 
+    @_("operand")  # noqa: 821
+    @_("condition")  # noqa: 821
+    def result(self, p: YaccProduction) -> bool:  # noqa: 811
+        res = p.condition if hasattr(p, "condition") else p.operand
+        return res
+
     @_("operand EQ operand")  # noqa: 821
     def condition(self, p: YaccProduction) -> bool:
         operand0 = p.operand0
         operand1 = p.operand1
         return operand0 == operand1
 
     @_("path EQ operand")  # noqa: 821
@@ -103,51 +108,62 @@
 
     @_("operand GT operand")  # noqa: 821
     def condition(self, p: YaccProduction) -> bool:  # noqa: 811
         operand0 = p.operand0
         operand1 = p.operand1
         return type(operand0) == type(operand1) and operand0 > operand1
 
+    @_('"(" condition ")"')  # noqa: 821
+    def condition(self, p: YaccProduction) -> bool:  # noqa: 811
+        return p.condition
+
+    @_('"(" operand ")"')  # noqa: 821
+    def operand(self, p: YaccProduction) -> bool:  # noqa: 811
+        return p.operand
+
     @_("condition AND condition")  # noqa: 821
     def condition(self, p: YaccProduction) -> bool:  # noqa: 811
-        condition0 = p.condition0
-        condition1 = p.condition1
-        return condition0 and condition1
+        return p.condition0 and p.condition1
+
+    @_("operand AND operand")  # noqa: 821
+    def condition(self, p: YaccProduction) -> bool:  # noqa: 811
+        return p.operand0 and p.operand1
+
+    @_("operand AND condition")  # noqa: 821
+    @_("condition AND operand")  # noqa: 821
+    def condition(self, p: YaccProduction) -> bool:  # noqa: 811
+        return p.condition and p.operand
 
     @_("condition OR condition")  # noqa: 821
     def condition(self, p: YaccProduction) -> bool:  # noqa: 811
-        condition0 = p.condition0
-        condition1 = p.condition1
-        return condition0 or condition1
+        return p.condition0 or p.condition1
+
+    @_("operand OR operand")  # noqa: 821
+    def condition(self, p: YaccProduction) -> bool:  # noqa: 811
+        return p.operand0 or p.operand1
+
+    @_("operand OR condition")  # noqa: 821
+    @_("condition OR operand")  # noqa: 821
+    def condition(self, p: YaccProduction) -> bool:  # noqa: 811
+        return p.condition or p.operand
 
     @_("NOT condition")  # noqa: 821
     def condition(self, p: YaccProduction) -> bool:  # noqa: 811
         condition = p.condition
         return not condition
 
     @_("NOT operand")  # noqa: 821
     def condition(self, p: YaccProduction) -> bool:  # noqa: 811
         return not p.operand
 
-    @_('"(" condition ")"')  # noqa: 821
-    def condition(self, p: YaccProduction) -> bool:  # noqa: 811
-        condition = p.condition
-        return condition
-
     @_('operand "," operand')  # noqa: 821
     def operand(self, p: YaccProduction) -> List[Any]:  # noqa: 811
         operand0 = p.operand0
         operand1 = p.operand1
 
-        # if not isinstance(operand0, tuple):
-        #    return (operand0, operand1)
-        #
-        # else:
-        #    return operand0 + (operand1,)
-
         if isinstance(operand0, tuple) and isinstance(operand1, tuple):
             res = operand0 + operand1
         elif isinstance(operand0, tuple) and not isinstance(operand1, tuple):
             res = operand0 + (operand1,)
         elif not isinstance(operand0, tuple) and isinstance(operand1, tuple):
             res = (operand0,) + operand1
         else:
@@ -305,12 +321,32 @@
         """Tests if a user is a member of a specific group"""
 
         if not self.__group_ids:
             return False
 
         return p.operand in self.__group_ids
 
+    #@_("turnary")  # noqa: 821
+    #def operand(self, p: YaccProduction) -> Any:
+    #    condition = p.turnary[0]
+    #    if_true = p.turnary[1]
+    #    if_false = p.turnary[2]
+    #    if condition:
+    #        return if_true
+    #    else:
+    #        return if_false
+
+    @_("operand QUESTION_MARK operand COLON operand")  # noqa: 821
+    @_("condition QUESTION_MARK operand COLON operand")  # noqa: 821
+    def operand(self, p: YaccProduction) -> Any:  # noqa: 811
+        condition = p.condition if hasattr(p, "condition") else p.operand0
+        if_true = p.operand0 if hasattr(p, "condition") else p.operand1
+        if_false = p.operand1 if hasattr(p, "condition") else p.operand2
+
+        return if_true if condition else if_false
+        #return (condition, p.operand0, p.operand1)
+
     @_("condition error")  # noqa: 821
     def operand(self, x):  # noqa: 811
         raise SyntaxError(
             f"Unexpected token '{x.error.value}' on line {x.error.lineno}"
         )
```

### Comparing `okta_expression_parser-0.2.2/pyproject.toml` & `okta_expression_parser-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "okta-expression-parser"
-version = "0.2.2"
+version = "0.3.0"
 description = "Returns a boolean by passing Okta profile data to an Okta Expression using Okta Expression Language"
 authors = ["Mathew Moon <me@mathewmoon.net>"]
 readme = "README.md"
 packages = [{include = "okta_expression_parser", from = "."}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

