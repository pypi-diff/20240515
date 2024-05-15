# Comparing `tmp/mp2c-0.0.2.tar.gz` & `tmp/mp2c-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mp2c-0.0.2.tar", last modified: Sun May  5 15:01:06 2024, max compression
+gzip compressed data, was "mp2c-0.1.0.tar", last modified: Wed May 15 11:57:18 2024, max compression
```

## Comparing `mp2c-0.0.2.tar` & `mp2c-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 15:01:06.909753 mp2c-0.0.2/
--rw-rw-rw-   0        0        0      117 2024-05-05 15:01:06.908262 mp2c-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       14 2024-03-30 02:15:52.000000 mp2c-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 15:01:06.903206 mp2c-0.0.2/mp2c/
--rw-rw-rw-   0        0        0      168 2024-05-05 14:30:01.000000 mp2c-0.0.2/mp2c/__init__.py
--rw-rw-rw-   0        0        0    12644 2024-04-13 09:26:13.000000 mp2c-0.0.2/mp2c/compiler.py
--rw-rw-rw-   0        0        0     4818 2024-05-05 13:04:09.000000 mp2c-0.0.2/mp2c/context.py
--rw-rw-rw-   0        0        0      685 2024-05-05 14:30:00.000000 mp2c-0.0.2/mp2c/converter.py
--rw-rw-rw-   0        0        0     4691 2024-05-04 03:46:19.000000 mp2c-0.0.2/mp2c/rules.py
--rw-rw-rw-   0        0        0     1492 2024-05-05 14:24:40.000000 mp2c-0.0.2/mp2c/utils.py
--rw-rw-rw-   0        0        0    31962 2024-05-05 14:42:11.000000 mp2c-0.0.2/mp2c/visitors.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:01:06.907085 mp2c-0.0.2/mp2c.egg-info/
--rw-rw-rw-   0        0        0      117 2024-05-05 15:01:06.000000 mp2c-0.0.2/mp2c.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-05-05 15:01:06.000000 mp2c-0.0.2/mp2c.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 15:01:06.000000 mp2c-0.0.2/mp2c.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-05 15:01:06.000000 mp2c-0.0.2/mp2c.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-05 15:01:06.909753 mp2c-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      430 2024-05-05 14:59:10.000000 mp2c-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:01:06.907085 mp2c-0.0.2/test/
--rw-rw-rw-   0        0        0        0 2024-04-13 14:05:25.000000 mp2c-0.0.2/test/test_visitors.py
+drwxrwxrwx   0        0        0        0 2024-05-15 11:57:18.272651 mp2c-0.1.0/
+-rw-rw-rw-   0        0        0      117 2024-05-15 11:57:18.271652 mp2c-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2024-03-30 02:15:52.000000 mp2c-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 11:57:18.262999 mp2c-0.1.0/mp2c/
+-rw-rw-rw-   0        0        0      242 2024-05-15 03:43:02.000000 mp2c-0.1.0/mp2c/__init__.py
+-rw-rw-rw-   0        0        0     5940 2024-05-15 09:04:47.000000 mp2c-0.1.0/mp2c/context.py
+-rw-rw-rw-   0        0        0     1534 2024-05-15 09:19:19.000000 mp2c-0.1.0/mp2c/converter.py
+-rw-rw-rw-   0        0        0      144 2024-05-13 03:49:03.000000 mp2c-0.1.0/mp2c/errors.py
+-rw-rw-rw-   0        0        0      473 2024-05-15 09:06:52.000000 mp2c-0.1.0/mp2c/result.py
+-rw-rw-rw-   0        0        0     9312 2024-05-15 03:05:30.000000 mp2c-0.1.0/mp2c/rules.py
+-rw-rw-rw-   0        0        0     5144 2024-05-15 08:50:25.000000 mp2c-0.1.0/mp2c/utils.py
+-rw-rw-rw-   0        0        0    36586 2024-05-15 08:10:06.000000 mp2c-0.1.0/mp2c/visitors.py
+drwxrwxrwx   0        0        0        0 2024-05-15 11:57:18.266662 mp2c-0.1.0/mp2c.egg-info/
+-rw-rw-rw-   0        0        0      117 2024-05-15 11:57:18.000000 mp2c-0.1.0/mp2c.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2024-05-15 11:57:18.000000 mp2c-0.1.0/mp2c.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 11:57:18.000000 mp2c-0.1.0/mp2c.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-15 11:57:18.000000 mp2c-0.1.0/mp2c.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 11:57:18.272651 mp2c-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      430 2024-05-15 11:57:12.000000 mp2c-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 11:57:18.270651 mp2c-0.1.0/test/
+-rw-rw-rw-   0        0        0        0 2024-05-10 01:57:03.000000 mp2c-0.1.0/test/__init__.py
+-rw-rw-rw-   0        0        0      528 2024-05-15 03:32:03.000000 mp2c-0.1.0/test/test_array.py
+-rw-rw-rw-   0        0        0     1594 2024-05-15 04:07:28.000000 mp2c-0.1.0/test/test_control.py
+-rw-rw-rw-   0        0        0      693 2024-05-15 03:37:24.000000 mp2c-0.1.0/test/test_gcd.py
+-rw-rw-rw-   0        0        0     2912 2024-05-15 08:11:36.000000 mp2c-0.1.0/test/test_lexical.py
+-rw-rw-rw-   0        0        0     1087 2024-05-15 04:07:03.000000 mp2c-0.1.0/test/test_scope.py
+-rw-rw-rw-   0        0        0     3228 2024-05-15 03:58:34.000000 mp2c-0.1.0/test/test_visitors.py
```

### Comparing `mp2c-0.0.2/mp2c/context.py` & `mp2c-0.1.0/mp2c/context.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,113 +1,139 @@
 from collections import deque
 
+
 class Context:
     def __init__(self):
         self.current_scope_index = -1
         self.symbol_table = deque()
+        self.on_error = False
+        self.error_messages = []
 
     def enter_scope(self):
-        self.symbol_table.append({"value" : {}, "array" : {}, "subprogram" : {}})
+        self.symbol_table.append({"value": {}, "array": {}, "subprogram": {}})
         self.current_scope_index += 1
 
     def exit_scope(self):
         self.symbol_table.pop()
         self.current_scope_index -= 1
 
-    def register_func(self, name, header, tokens):
-        if self.current_scope_index < 0 or self.current_scope_index >= len(self.symbol_table) :
+    def register_func(self, name, header, parameter_list):
+        if self.current_scope_index < 0 or self.current_scope_index >= len(self.symbol_table):
             raise Exception("try to register function {} in no scope ".format(name))
-        functions_in_top_smbltab = self.symbol_table[self.current_scope_index-1]["subprogram"]
-        functions_in_top_smbltab[name] = FunctionSymbol(name,header,tokens)
+        functions_in_top_smbltab = self.symbol_table[self.current_scope_index - 1]["subprogram"]
+        functions_in_top_smbltab[name] = FunctionSymbol(name, header, None, parameter_list)
 
     def declare_func(self, name, tokens):
-        self.symbol_table[self.current_scope_index-1]["subprogram"][name].tokens = tokens
-        
-    
-    def register_value(self, name, type, mutable, value = None):
+        self.symbol_table[self.current_scope_index - 1]["subprogram"][name].tokens = tokens
+
+    def register_value(self, name, value_type, mutable, value = None):
         if self.current_scope_index < 0 or self.current_scope_index >= len(self.symbol_table):
             raise Exception("try to register value {} in no scope ".format(name))
         values_in_top_smbltab = self.symbol_table[self.current_scope_index]["value"]
-        values_in_top_smbltab[name] = ValueSymbol(name, type, mutable, value)
+        values_in_top_smbltab[name] = ValueSymbol(name, value_type, mutable, value)
 
-    def register_array(self, name, type, periods):   # periods(start, last) : [[1, 5], [2, 4]]  
+    def register_array(self, name, array_type, periods):  # periods(start, last) : [[1, 5], [2, 4]]
         if self.current_scope_index < 0 or self.current_scope_index >= len(self.symbol_table):
             raise Exception("try to register array {} in no scope ".format(name))
         arrays_in_top_smbltab = self.symbol_table[self.current_scope_index]["array"]
         dimensions = []
         for dimension in periods:
-            dimensions = [dimension[1] - dimension[0] + 1, dimension[0]]
-        arrays_in_top_smbltab[name] = ArraySymbol(name, type, dimensions)   # dimensions(length, start) : [[5, 1], [3, 2]]
-        
+            dimensions.append([dimension[1] - dimension[0] + 1, dimension[0]])
+        arrays_in_top_smbltab[name] = ArraySymbol(name, array_type,
+                                                  dimensions)  # dimensions(length, start) : [[5, 1], [3, 2]]
+
     def get_funcs(self):
         if self.current_scope_index < 0 or self.current_scope_index >= len(self.symbol_table):
             raise Exception("try to get functions in no scope ")
         return self.symbol_table[self.current_scope_index]["subprogram"]
-    
+
     def get_values(self):
         if self.current_scope_index < 0 or self.current_scope_index >= len(self.symbol_table):
             raise Exception("try to get values in no scope ")
         return self.symbol_table[self.current_scope_index]["value"]
-    
+
     def get_arrays(self):
         if self.current_scope_index < 0 or self.current_scope_index >= len(self.symbol_table):
             raise Exception("try to get arrays in no scope ")
         return self.symbol_table[self.current_scope_index]["array"]
-    
+
     def get_value(self, name):
-        return self.get_values().get(name)
-    
+        value_symbol = self.get_values().get(name)
+        context_index = self.current_scope_index
+        while value_symbol is None and context_index >= 0:
+            value_symbol = self.symbol_table[context_index]["value"].get(name)
+            context_index -= 1
+        return value_symbol
+
     def get_array(self, name):
-        return self.get_arrays().get(name)
-    
+        array_symbol = self.get_arrays().get(name)
+        context_index = self.current_scope_index
+        while array_symbol is None and context_index >= 0:
+            array_symbol = self.symbol_table[context_index]["array"].get(name)
+            context_index -= 1
+        return array_symbol
+
     def get_func(self, name):
-        func= self.get_funcs().get(name)
-        if func is None and self.current_scope_index > 0:
-            func = self.symbol_table[0]["subprogram"].get(name)
+        index = self.current_scope_index
+        func = None
+        while func is None and index >= 0:
+            func = self.symbol_table[index]["subprogram"].get(name)
+            index -= 1
         return func
-    
+
+    def record_error(self, message):
+        self.on_error = True
+        self.error_messages.append(message)
+
     # def cname_to_type(self, name):
     #     res = int
     #     if name == "float" :
     #         res = float
     #     elif name == "char" or name == "char*":
     #         res = str
     #     elif name == "bool":
     #         res = bool
     #     return res
 
 
 class FunctionSymbol:
-    def __init__(self, name, header, tokens):
+    def __init__(self, name, header, tokens, parameter_list):
         self.name = name
         self.header = header
         self.tokens = tokens
-    
+        self.parameter_list = parameter_list
+
     def __repr__(self) -> str:
-        return self.name
+        description = "Function: " + self.name + "\n"
+        description += "Header: " + " ".join(self.header) + "\n"
+        description += "Tokens: " + str(self.tokens) + "\n"
+        description += "Parameters: " + str(self.parameter_list) + "\n"
+        return description
+
 
 class ValueSymbol:
-    def __init__(self, name, type, mutable, value):
+    def __init__(self, name, value_type, mutable, value):
         self.name = name
-        self.type = type
+        self.type = value_type
         self.mutable = mutable
         self.value = value
-        
+
     def __repr__(self) -> str:
         description = "Value: " + self.name + "\n"
         description += "Type: " + self.type + "\n"
         description += "Mutable: " + str(self.mutable) + "\n"
         description += "Value: " + str(self.value) + "\n"
         return description
 
+
 class ArraySymbol:
-    def __init__(self, name, type, dimensions):
+    def __init__(self, name, array_type, dimensions):
         self.name = name
-        self.type = type
-        self.dimensions = dimensions    # [[length1, start1], [length2, start2]...]
+        self.type = array_type
+        self.dimensions = dimensions  # [[length1, start1], [length2, start2]...]
         length_sum = 0
         for dimension in self.dimensions:
             length_sum += dimension[0]
         self.value = [None] * length_sum
 
     def __repr__(self) -> str:
         description = "Array: " + self.name + "\n"
```

### Comparing `mp2c-0.0.2/mp2c/rules.py` & `mp2c-0.1.0/mp2c/rules.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,70 +1,174 @@
-rules = r"""
+# rules = r"""
+# programstruct            : program_head ";" program_body "."
+# program_head             : "program" id "(" idlist ")"
+#                          | "program" id
+# idlist                   : id ("," id)*
+# program_body             : const_declarations var_declarations subprogram_declarations compound_statement
+# const_declarations       : empty
+#                          | "const" const_declaration ";"
+# const_declaration        : id "=" const_value (";" id "=" const_value)*
+# const_value              : PLUS num
+#                          | MINUS num
+#                          | num
+#                          | "'" LETTER "'"
+# PLUS                     : "+"
+# MINUS                    : "-"
+# var_declarations         : empty
+#                          | "var" var_declaration ";"
+# var_declaration          : idlist ":" type (";" idlist ":" type)*
+# type                     : basic_type
+#                          | "array" "[" period "]" "of" basic_type
+# basic_type               : INTEGER
+#                          | REAL
+#                          | BOOLEAN
+#                          | CHAR
+# period                   : DIGITS ".." DIGITS
+#                          | period "," DIGITS ".." DIGITS
+# subprogram_declarations  : (subprogram ";")*
+# subprogram               : subprogram_head ";" subprogram_body
+# subprogram_head          : "procedure" id formal_parameter
+#                          | "function" id formal_parameter ":" basic_type
+# formal_parameter         : "(" parameter_list ")"
+#                          | empty
+# parameter_list           : empty
+#                          | parameter (";" parameter)*
+# parameter                : var_parameter
+#                          | value_parameter
+# var_parameter            : "var" value_parameter
+# value_parameter          : idlist ":" basic_type
+# subprogram_body          : const_declarations var_declarations compound_statement
+# compound_statement       : "begin" statement_list "end"
+# statement_list           : statement (";" statement)*
+# statement                : empty
+#                          | assign_statement
+#                          | procedure_call
+#                          | compound_statement
+#                          | if_else_statement
+#                          | for_statement
+#                          | while_statement
+# assign_statement         : variable ASSIGNOP expression
+#                          | func_id ASSIGNOP expression
+# if_else_statement        : "if" expression "then" statement else_part
+# for_statement            : "for" id ASSIGNOP expression "to" expression "do" statement
+# while_statement          : "while" expression "do" statement
+# variable_list            : variable ("," variable)*
+# variable                 : id id_varpart
+# id_varpart               : empty
+#                          | "[" expression_list "]"
+# procedure_call           : id
+#                          | id "(" expression_list ")"
+# else_part                : empty
+#                          | "else" statement
+# expression_list          : expression ("," expression)*
+# expression               : simple_expression
+#                          | simple_expression RELOP simple_expression
+# simple_expression        : term
+#                          | simple_expression ADDOP term
+# term                     : factor
+#                          | term MULOP factor
+# factor                   : num
+#                          | variable
+#                          | "(" expression ")"
+#                          | NOT factor
+#                          | UMINUS factor
+#                          | function_call
+# function_call            : func_id "(" expression_list ")"
+# NOT                      : "not"
+# DIGITS                   : DIGIT+
+# id                       : IDENTIFIER_TOKEN
+# optional_fraction        : "." DIGITS
+# num                      : DIGITS optional_fraction?
+# RELOP                    : "="
+#                          | "<>"
+#                          | "<"
+#                          | "<="
+#                          | ">"
+#                          | ">="
+# ADDOP                    : "+"
+#                          | "-"
+#                          | "or"
+# MULOP                    : "*"
+#                          | "/"
+#                          | "div"
+#                          | "mod"
+#                          | "and"
+# ASSIGNOP                 : ":="
+# empty                    : WS*
+# func_id                  : id
+# UMINUS                   : "-"
+# IDENTIFIER_TOKEN         : /[a-zA-Z_][a-zA-Z0-9_]*/
+# INTEGER                  : "integer"
+# REAL                     : "real"
+# BOOLEAN                  : "boolean"
+# CHAR                     : "char"
+# %import common.DIGIT
+# %import common.LETTER
+# %import common.WS
+# %ignore WS
+# """
+
+rules= r"""
 programstruct            : program_head ";" program_body "."
 program_head             : "program" id "(" idlist ")"
                          | "program" id
 idlist                   : id
                          | idlist "," id
-program_body             : const_declarations var_declarations subprogram_declarations compound_statement
-const_declarations       : empty
-                         | "const" const_declaration ";"
+program_body             : const_declarations? var_declarations? subprogram_declarations compound_statement
+const_declarations       : "const" const_declaration ";"
 const_declaration        : id "=" const_value (";" id "=" const_value)*
 const_value              : PLUS num
                          | MINUS num
                          | num
                          | "'" LETTER "'"
 PLUS                     : "+"
 MINUS                    : "-"        
-var_declarations         : empty
-                         | "var" var_declaration ";"
-var_declaration          : idlist ":" type
-                         | var_declaration ";" idlist ":" type
+var_declarations         : "var" var_declaration ";"
+var_declaration          : idlist ":" type (";" idlist ":" type)*
 type                     : basic_type
                          | "array" "[" period "]" "of" basic_type
 basic_type               : INTEGER
                          | REAL
                          | BOOLEAN
                          | CHAR
 period                   : DIGITS ".." DIGITS
                          | period "," DIGITS ".." DIGITS
-subprogram_declarations  : empty
-                         | subprogram_declarations subprogram ";"
+subprogram_declarations  : (subprogram ";")*
 subprogram               : subprogram_head ";" subprogram_body
 subprogram_head          : "procedure" id formal_parameter
                          | "function" id formal_parameter ":" basic_type
 formal_parameter         : "(" parameter_list ")"
+                         | empty
 parameter_list           : empty
                          | parameter (";" parameter)*
 parameter                : var_parameter
                          | value_parameter
 var_parameter            : "var" value_parameter
 value_parameter          : idlist ":" basic_type
-subprogram_body          : const_declarations var_declarations compound_statement
+subprogram_body          : const_declarations? var_declarations? compound_statement
 compound_statement       : "begin" statement_list "end"
 statement_list           : statement (";" statement)*
 statement                : empty
                          | assign_statement
                          | procedure_call
                          | compound_statement
                          | if_else_statement
                          | for_statement
                          | while_statement
 assign_statement         : variable ASSIGNOP expression
                          | func_id ASSIGNOP expression
-if_else_statement        : "if" expression "then" statement else_part
+if_else_statement        : "if" expression "then" statement else_part?
 for_statement            : "for" id ASSIGNOP expression "to" expression "do" statement
 while_statement          : "while" expression "do" statement
 variable_list            : variable ("," variable)*
-variable                 : id id_varpart
-id_varpart               : empty
-                         | "[" expression_list "]"
+variable                 : id id_varpart?
+id_varpart               : "[" expression_list "]"
 procedure_call           : id
                          | id "(" expression_list ")"
-else_part                : empty
-                         | "else" statement
+else_part                : "else" statement
 expression_list          : expression ("," expression)*
 expression               : simple_expression
                          | simple_expression RELOP simple_expression
 simple_expression        : term
                          | simple_expression ADDOP term
 term                     : factor
                          | term MULOP factor
```

### Comparing `mp2c-0.0.2/mp2c/visitors.py` & `mp2c-0.1.0/mp2c/visitors.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,289 +1,331 @@
-import lark
+from lark.lark import Token
 
-from .context import Context
 from .utils import *
 
 
-def visit_empty(node: lark.tree.Tree, context: Context):
+def visit_empty(node: Tree, context: Context):
     tokens = []
     return tokens
 
 
-def visit_optional_fraction(node: lark.tree.Tree, context: Context):
+def visit_optional_fraction(node: Tree, context: Context):
     return node.children[0].value
 
 
-def visit_num(node: lark.tree.Tree, context: Context):
+def visit_num(node: Tree, context: Context):
     tokens = []
     typename = ""
     for child in node.children:
-        if isinstance(child, lark.lexer.Token):
+        if isinstance(child, Token):
             typename = "int"
             tokens.append(child.value)
 
         elif child.data == "optional_fraction":
             typename = "float"
             optional_fraction_part = visit_optional_fraction(child, context)
             tokens[-1] += "."
             tokens[-1] += optional_fraction_part
         else:
             raise Exception("Unknown num child data: {}".format(child.data))
 
     return [tokens, typename]
 
 
-def visit_period(node: lark.tree.Tree, context: Context):
+def visit_period(node: Tree, context: Context):
     periods = []
     current_period = []
     for child in node.children:
-        if isinstance(child, lark.lexer.Token):
+        if isinstance(child, Token):
             current_period.append(int(child.value))
         elif child.data == "period":
             current_period = visit_period(child, context)
             periods.append(current_period)
             current_period = []
         else:
             raise Exception("Unknown period child data: {}".format(child.data))
     periods.append(current_period)
     return periods
 
 
-def visit_basic_type(node: lark.tree.Tree, context: Context):
+def visit_basic_type(node: Tree, context: Context):
     return type_map[node.children[0].value]
 
 
-def visit_type(node: lark.tree.Tree, context: Context):
-    type = {"basic_type": None, "is_array": False, "period": []}
+def visit_type(node: Tree, context: Context):
+    type_ = {"basic_type": None, "is_array": False, "period": []}
     for child in node.children:
         if child.data == "basic_type":
-            type["basic_type"] = visit_basic_type(child, context)
+            type_["basic_type"] = visit_basic_type(child, context)
         elif child.data == "period":
-            type["period"] = visit_period(child, context)
-            type["is_array"] = True
+            type_["period"] = visit_period(child, context)
+            type_["is_array"] = True
         else:
             raise Exception("Unknown type child data: {}".format(child.data))
-    return type
+    return type_
 
 
-def visit_id(node, context, func_name):
+def visit_id(node: Tree, context: Context, func_name: str):
     name = node.children[0].value
     if name == func_name:
         return "_" + name
     else:
         return node.children[0].value
 
 
-def visit_idlist(node: lark.tree.Tree, context: Context):
+def visit_idlist(node: Tree, context: Context):
     ids = []
     for child in node.children:
         if child.data == "id":
             # 从idlist得到的id不需要考虑func_name修正
-            ids.append(visit_id(child, context, None))
+            ids.append(visit_id(child, context, ""))
         elif child.data == "idlist":
             ids.extend(visit_idlist(child, context))
         else:
             raise Exception("Unknown idlist child data: {}".format(child.data))
     return ids
 
 
-def visit_value_parameter(node: lark.tree.Tree, context: Context):
+def visit_value_parameter(node: Tree, context: Context):
     ids = []
     type_ = None
     for child in node.children:
         if child.data == "idlist":
             # 函数形参不需要考虑名称修正
             # ids = visit_idlist(child, context, None)
             ids = visit_idlist(child, context)
         elif child.data == "basic_type":
             type_ = visit_basic_type(child, context)
         else:
             raise Exception("Unknown value_parameter child data: {}".format(child.data))
     return {"ids": ids, "type": type_}
 
 
-def visit_var_parameter(node: lark.tree.Tree, context: Context):
-    tokens = []
+def visit_var_parameter(node: Tree, context: Context):
     value_parameter = visit_value_parameter(node.children[0], context)
+    tokens = construct_parameter_tokens(value_parameter, context)
+    return tokens, value_parameter
+
+
+def construct_parameter_tokens(value_parameter, context):
+    tokens = []
     first = True
-    for id in value_parameter["ids"]:
+    for id_ in value_parameter["ids"]:
         if first:
             first = False
         else:
             tokens.append(",")
         id_type = value_parameter["type"]
-        context.register_value(id, id_type, True)
+        context.register_value(id_, id_type, True)
         tokens.append(id_type)
-        tokens.append(id)
+        tokens.append(id_)
     return tokens
 
 
-def visit_parameter(node: lark.tree.Tree, context: Context):
+def visit_parameter(node: Tree, context: Context):
     tokens = []
+    parameter = None
     for child in node.children:
         if child.data == "var_parameter":
-            return visit_var_parameter(child, context)
+            tokens, parameter = visit_var_parameter(child, context)
         elif child.data == "value_parameter":
-            value_parameter = visit_value_parameter(child, context)
-            first = True
-            for id in value_parameter["ids"]:
-                if first:
-                    first = False
-                else:
-                    tokens.append(",")
-                id_type = value_parameter["type"]
-                context.register_value(id, id_type, True)
-                tokens.append(id_type)
-                tokens.append(id)
+            parameter = visit_value_parameter(child, context)
+            tokens = construct_parameter_tokens(parameter, context)
         else:
             raise Exception("Unknown parameter child data: {}".format(child.data))
-    return tokens
+    return tokens, parameter
 
 
-def visit_parameter_list(node: lark.tree.Tree, context: Context):
+def visit_parameter_list(node: Tree, context: Context):
     tokens = []
     first = True
+    parameter_list = []
     for child in node.children:
         assert child.data == "parameter"
         if first:
             first = False
         else:
             tokens.append(",")
-        tokens.extend(visit_parameter(child, context))
-    return tokens
+        parameter_tokens, parameter = visit_parameter(child, context)
+        tokens.extend(parameter_tokens)
+        parameter_list.append(parameter)
+    return tokens, parameter_list
 
 
-def visit_formal_parameter(node: lark.tree.Tree, context: Context):
+def visit_formal_parameter(node: Tree, context: Context):
     tokens = ["("]
-    parameter_list = visit_parameter_list(node.children[0], context)
-    tokens.extend(parameter_list)
+    parameter_list_tokens, parameter_list = visit_parameter_list(node.children[0], context)
+    tokens.extend(parameter_list_tokens)
     tokens.append(")")
-    return tokens
+    return tokens, parameter_list
 
 
-def visit_subprogram_head(node: lark.tree.Tree, context: Context):
+def visit_subprogram_head(node: Tree, context: Context):
     tokens = []
     basic_type = None
     id_ = None
-    formal_parameter = None
+    formal_parameter_tokens = None
+    parameter_info_list = None
+    parameter_list = []
     for child in node.children:
         if child.data == "basic_type":
             basic_type = visit_basic_type(child, context)
         elif child.data == "id":
             # subprogram_head中的id不需要考虑func_name修正
-            id_ = visit_id(child, context, None)
+            id_ = visit_id(child, context, "")
         elif child.data == "formal_parameter":
-            formal_parameter = visit_formal_parameter(child, context)
+            formal_parameter_tokens, parameter_info_list = visit_formal_parameter(child, context)
         else:
             raise Exception("Unknown subprogram_head child data: {}".format(child.data))
     if basic_type:
         tokens.append(basic_type)
     else:
         tokens.append("void")
     tokens.append(id_)
-    tokens.extend(formal_parameter)
-    context.register_func(id_, tokens, None)
+    tokens.extend(formal_parameter_tokens)
+    for id_group in parameter_info_list:
+        for _ in id_group["ids"]:
+            parameter_list.append(id_group["type"])
+    context.register_func(id_, tokens, parameter_list)
     return tokens
 
 
-def visit_func_id(node, context, func_name):
+def visit_func_id(node):
     tokens = []
     for child in node.children:
         assert child.data == "id"
         for grandchild in child.children:
             if grandchild.type == "IDENTIFIER_TOKEN":
                 tokens.append(grandchild.value)
             else:
                 raise Exception("Unknown func_id grandchild type: {}".format(grandchild.type))
     return tokens
 
 
-def visit_id_varpart(node, context, func_name):
+def visit_id_varpart(node: Tree, context: Context, func_name: str, id_token):
     tokens = []
     for child in node.children:
         if child.data == "empty":
             return tokens
         elif child.data == "expression_list":
             tokens.append("[")
-            expression_list = visit_expression_list(child, context, func_name)
-            tokens.extend(expression_list)
+            expression_list, expression_types = visit_expression_list(child, context, func_name)
+            # check if all elements in expression_types are the integer type
+            for expression_type in expression_types:
+                if expression_type != "int":
+                    # raise Exception("Array index must be integer")
+                    error_message = "Array index must be integer, but got {}".format(expression_type)
+                    context.record_error(error_message)
+            array_symbol = context.get_array(id_token)
+            # split expression_list by ','
+            count = 0
+            for expression_token in expression_list:
+                if expression_token == ",":
+                    offset = array_symbol.dimensions[count][1]
+                    tokens.extend(['-', str(offset)])
+                    count += 1
+                tokens.append(expression_token)
+            offset = array_symbol.dimensions[count][1]
+            tokens.extend(['-', str(offset)])
+            count += 1
             tokens.append("]")
         else:
             raise Exception("Unknown id_varpart child data: {}".format(child.data))
     return tokens
 
 
-def visit_variable(node, context, func_name):
+def visit_variable(node: Tree, context: Context, func_name: str):
     tokens = []
     isArray = False
-    id_varpart = None
-    variable_type = None
+    id_varpart = []
     id_token = None
     for child in node.children:
         if child.data == "id":
             id_token = visit_id(child, context, func_name)
         elif child.data == "id_varpart":
-            id_varpart = visit_id_varpart(child, context, func_name)
+            id_varpart = visit_id_varpart(child, context, func_name, id_token)
             if len(id_varpart) > 0:
                 isArray = True
         else:
             raise Exception("Unknown variable child data: {}".format(child.data))
-    values = context.get_values()
     if isArray:
         array = context.get_array(id_token)
+        if array is None:
+            # raise Exception("Array not declared: {}".format(id_token))
+            error_message = "Array used but not declared: {}".format(id_token)
+            context.record_error(error_message)
         variable_type = array.type
     else:
         value = context.get_value(id_token)
+        if value is None:
+            # raise Exception("Variable not declared: {}".format(id_token))
+            error_message = "Variable not declared: {}".format(id_token)
+            context.record_error(error_message)
         variable_type = value.type
     tokens.append(id_token)
     tokens.extend(id_varpart)
     return tokens, variable_type
 
 
-def visit_variable_list(node, context, func_name):
+def visit_variable_list(node: Tree, context: Context, func_name: str):
     tokens = []
     first = True
     for child in node.children:
         if first:
             first = False
         else:
             tokens.append(",")
         variable_token, variable_type = visit_variable(child, context, func_name)
         tokens.extend(variable_token)
     return tokens
 
 
-def visit_function_call(node, context, func_name):
+def visit_function_call(node: Tree, context: Context, func_name: str):
     tokens = []
     function_type = None
+    function = None
+    function_name = None
     for child in node.children:
         if child.data == "func_id":
-            function_token = visit_func_id(child, context, func_name)
+            function_token = visit_func_id(child)
             function_name = function_token[0]
-            functions = context.get_funcs()
             function = context.get_func(function_name)
+            if function is None:
+                # raise Exception("Function not declared: {}".format(function_name))
+                error_message = "Function not declared: {}".format(function_name)
+                context.record_error(error_message)
             function_type = function.header[0]
             tokens.extend(function_token)
         elif child.data == "expression_list":
             tokens.append("(")
-            expression_list_tokens = ""
-            expression_list_tokens = visit_expression_list(child, context, func_name)
+            expression_list_tokens, expression_types = visit_expression_list(child, context, func_name)
+            # check if the number of parameters is correct
+            if len(expression_types) != len(function.parameter_list):
+                # raise Exception("Number of parameters does not match")
+                error_message = "Number of parameters while calling function {} does not match:".format(function_name)
+                error_message += " expected {}, got {}".format(len(function.parameter_list), len(expression_types))
+                context.record_error(error_message)
+            if expression_types != function.parameter_list:
+                # raise Exception("Parameter types do not match")
+                error_message = "Parameter types while calling function {} do not match:".format(function_name)
+                error_message += " expected {}, got {}".format(function.parameter_list, expression_types)
+                context.record_error(error_message)
             tokens.extend(expression_list_tokens)
             tokens.append(")")
         else:
             raise Exception("Unknown procedure_call child data: {}".format(child.data))
 
     return tokens, function_type
 
 
-def visit_factor(node, context, func_name):
+def visit_factor(node: Tree, context: Context, func_name: str):
     tokens = []
     factor_type = None
     for child in node.children:
-        if isinstance(child, lark.lexer.Token):
+        if isinstance(child, Token):
             token_type = child.type
             token_value = child.value
             if token_type == "NOT":
                 tokens.append("!")
             elif token_type == "UMINUS":
                 tokens.append(uminus_map[token_value])
         elif child.data == "num":
@@ -305,37 +347,37 @@
             function_call_token, factor_type = visit_function_call(child, context, func_name)
             tokens.extend(function_call_token)
         else:
             raise Exception("Unknown factor child data: {}".format(child.data))
     return tokens, factor_type
 
 
-def visit_term(node, context, func_name):
+def visit_term(node: Tree, context: Context, func_name: str):
     term_type = None
     tokens = []
     for child in node.children:
-        if isinstance(child, lark.lexer.Token):
+        if isinstance(child, Token):
             tokens.append(mulop_map[child.value])
         elif child.data == "factor":
             factor_token, factor_type = visit_factor(child, context, func_name)
             tokens.extend(factor_token)
             term_type = factor_type
         elif child.data == "term":
             term_token, term_type = visit_term(child, context, func_name)
             tokens.extend(term_token)
         else:
             raise Exception("Unknown term child data: {}".format(child.data))
     return tokens, term_type
 
 
-def visit_simple_expression(node, context, func_name):
+def visit_simple_expression(node: Tree, context: Context, func_name: str):
     tokens = []
     simple_expression_type = None
     for child in node.children:
-        if isinstance(child, lark.lexer.Token):
+        if isinstance(child, Token):
             tokens.append(addop_map[child.value])
         elif child.data == "term":
             term_token, term_type = visit_term(child, context, func_name)
             tokens.extend(term_token)
             simple_expression_type = term_type
         elif child.data == "simple_expression":
             simple_expression_token, simple_expression_type = visit_simple_expression(child, context, func_name)
@@ -343,71 +385,78 @@
         else:
             raise Exception(
                 "Unknown simple_expression child data: {}".format(child.data)
             )
     return tokens, simple_expression_type
 
 
-def visit_expression(node, context, func_name):
+def visit_expression(node: Tree, context: Context, func_name: str):
     tokens = []
-    expression_type = None
     isBool = False
     simple_expression_type = None
     for child in node.children:
-        if isinstance(child, lark.lexer.Token):
+        if isinstance(child, Token):
             tokens.append(relop_map[child.value])
             isBool = True
         elif child.data == "simple_expression":
             simple_expression_token, simple_expression_type = visit_simple_expression(child, context, func_name)
             tokens.extend(simple_expression_token)
         else:
             raise Exception("Unknown expression child data: {}".format(child.data))
     if isBool:
         expression_type = "bool"
     else:
         expression_type = simple_expression_type
     return tokens, expression_type
 
 
-def visit_expression_list(node, context, func_name):
+def visit_expression_list(node: Tree, context: Context, func_name: str):
     tokens = []
     first = True
+    expression_types = []
     for child in node.children:
         if first:
             first = False
         else:
             tokens.append(",")
-        expression_tokens, _ = visit_expression(child, context, func_name)
+        expression_tokens, expression_type = visit_expression(child, context, func_name)
+        expression_types.append(expression_type)
         tokens.extend(expression_tokens)
-    # test if all members of tokens are string
-    for token in tokens:
-        if not isinstance(token, str):
-            raise Exception("Token is not string: {}".format(token))
-    return tokens
+    return tokens, expression_types
 
 
-def visit_assign_statement(node, context, func_name):
+def visit_assign_statement(node: Tree, context: Context, func_name: str):
     tokens = []
+    variable_type = None
+    expression_type = None
+    variable_tokens = []
+    expression_tokens = []
     for child in node.children:
-        if isinstance(child, lark.lexer.Token):
+        if isinstance(child, Token):
             tokens.append(assignop_map[child.value])
         elif child.data == "expression":
-            expression_tokens, _ = visit_expression(child, context, func_name)
+            expression_tokens, expression_type = visit_expression(child, context, func_name)
             tokens.extend(expression_tokens)
         elif child.data == "variable":
             variable_tokens, variable_type = visit_variable(child, context, func_name)
             tokens.extend(variable_tokens)
         else:
             raise Exception(
                 "Unknown assignment_statement child data: {}".format(child.data)
             )
+    if variable_type != expression_type:
+        raise Exception("Type mismatch in assignment: {},{} != {}, {}".
+                        format("".join(variable_tokens),
+                               variable_type,
+                               "".join(expression_tokens),
+                               expression_type))
     return tokens
 
 
-def visit_if_else_statement(node, context, func_name):
+def visit_if_else_statement(node: Tree, context: Context, func_name: str):
     tokens = []
     for child in node.children:
         if child.data == "expression":
             tokens.append("if")
             tokens.append("(")
             expression_tokens, expression_type = visit_expression(child, context, func_name)
             tokens.extend(expression_tokens)
@@ -423,15 +472,15 @@
         else:
             raise Exception(
                 "Unknown if_else_statement child data: {}".format(child.data)
             )
     return tokens
 
 
-def visit_else_part(node, context, func_name):
+def visit_else_part(node: Tree, context: Context, func_name: str):
     tokens = []
     for child in node.children:
         if child.data == "empty":
             return tokens
         elif child.data == "statement":
             tokens.append("else")
             tokens.append("{")
@@ -439,179 +488,214 @@
             tokens.extend(statement_tokens)
             tokens.append("}")
         else:
             raise Exception("Unknown else_part child data: {}".format(child.data))
     return tokens
 
 
-def construct_read_params(node, context, func_name):
+def construct_read_params(node: Tree, context: Context, func_name: str):
     tokens = []
     ids = []
     types = []
     for child in node.children:
         if child.data == "expression":
             expression_tokens, expression_type = visit_expression(child, context, func_name)
             assert len(expression_tokens) == 1
             id_ = expression_tokens[0]
             ids.append(id_)
             value = context.get_value(id_)
+            if value is None:
+                raise Exception("Variable not declared: {}".format(id_))
             types.append(value.type)
         else:
             raise Exception("Unknown read_params child data: {}".format(child.data))
     format_ = types_to_format(types)
     tokens.append(format_)
     for id_ in ids:
         tokens.append(",")
         tokens.append("&")
         tokens.append(id_)
     return tokens
 
 
-def types_to_format(types):
+def types_to_format(types, line = False):
     format_ = '"'
     for id_type in types:
         if id_type == "int":
             format_ += r"%d"
         elif id_type == "float":
             format_ += r"%f"
         elif id_type == "char":
             format_ += r"%c"
         else:
             raise Exception("Unknown type: {}".format(id_type))
+    if line:
+        format_ += r"\n"
     format_ += '"'
     return format_
 
 
-def construct_write_params(node, context, func_name):
+def construct_write_params(node: Tree, context: Context, func_name: str, line = False):
     tokens = []
     expressions = []
     types = []
     for child in node.children:
         if child.data == "expression":
             expression_token, expression_type = visit_expression(child, context, func_name)
             expressions.append(expression_token)
             types.append(expression_type)
         else:
             raise Exception("Unknown write_params child data: {}".format(child.data))
-    format_ = types_to_format(types)
+    format_ = types_to_format(types, line)
     tokens.append(format_)
     for expression in expressions:
         tokens.append(",")
         tokens.extend(expression)
+
     return tokens
 
 
-def visit_procedure_call(node, context, func_name):
+def visit_procedure_call(node: Tree, context: Context, func_name: str):
     tokens = []
     isRead = False
     isWrite = False
+    isWriteLn = False
+    procedure_name = None
+    flag = False
     for child in node.children:
         if child.data == "id":
             if child.children[0].value == "read":
                 isRead = True
                 tokens.append("scanf")
             elif child.children[0].value == "write":
                 isWrite = True
                 tokens.append("printf")
+            elif child.children[0].value == "writeln":
+                isWriteLn = True
+                tokens.append("printf")
             else:
                 # 过程调用不进行func_name修正
-                tokens.append(visit_id(child, context, None))
+                procedure_name = visit_id(child, context, "")
+                tokens.append(procedure_name)
         elif child.data == "expression_list":
+            flag = True
             tokens.append("(")
             if isRead:
                 expression_list_tokens = construct_read_params(
                     child, context, func_name
                 )
             elif isWrite:
                 expression_list_tokens = construct_write_params(
                     child, context, func_name
                 )
+            elif isWriteLn:
+                expression_list_tokens = construct_write_params(
+                    child, context, func_name, True
+                )
             else:
-                expression_list_tokens = visit_expression_list(
+                expression_list_tokens, expression_types = visit_expression_list(
                     child, context, func_name
                 )
+                function = context.get_func(procedure_name)
+                if function is None:
+                    raise Exception("Procedure not declared: {}".format(procedure_name))
+                if len(expression_types) != len(function.parameter_list):
+                    raise Exception("Number of parameters does not match")
+                if expression_types != function.parameter_list:
+                    raise Exception("Parameter types do not match")
             tokens.extend(expression_list_tokens)
             tokens.append(")")
         else:
             raise Exception("Unknown procedure_call child data: {}".format(child.data))
+    if not flag:
+        tokens.extend(["(", ")"])
     return tokens
 
 
-def visit_statement_list(node, context, func_name):
+def visit_statement_list(node: Tree, context: Context, func_name: str):
     tokens = []
     for child in node.children:
         assert child.data == "statement"
         statement_tokens = visit_statement(child, context, func_name)
         tokens.extend(statement_tokens)
         tokens.append(";")
     return tokens
 
 
-def visit_compound_statement(node, context, func_name):
+def visit_compound_statement(node: Tree, context: Context, func_name: str):
     tokens = []
     assert node.children[0].data == "statement_list"
     statement_list_tokens = visit_statement_list(node.children[0], context, func_name)
     tokens.extend(statement_list_tokens)
     return tokens
 
 
-def visit_for_statement(node, context, func_name):
+def visit_for_statement(node: Tree, context: Context, func_name: str):
     tokens = []
-    id_tokens = []
+    id_token = []
     from_tokens = []
     to_tokens = []
     statement_tokens = []
+    first = True
     for child in node.children:
-        if child.data == "id":
-            tokens.append(visit_id(child, context, func_name))
+        if isinstance(child, Token):
+            if child.type != "ASSIGNOP":
+                raise Exception("Unknown for_statement child type: {}".format(child.type))
+        elif child.data == "id":
+            context.enter_scope()
+            id_token = visit_id(child, context, func_name)
+            context.register_value(id_token, "int", True)
         elif child.data == "expression":
-            if id_tokens:
-                from_tokens = visit_expression(child, context, func_name)
+            if first:
+                from_tokens, from_type = visit_expression(child, context, func_name)
+                first = False
             else:
-                to_tokens = visit_expression(child, context, func_name)
+                to_tokens, to_type = visit_expression(child, context, func_name)
         elif child.data == "statement":
             statement_tokens = visit_statement(child, context, func_name)
         else:
             raise Exception("Unknown for_statement child data: {}".format(child.data))
     tokens.extend(["for", "("])
-    tokens.extend(id_tokens)
+    tokens.extend(id_token)
     tokens.append("=")
     tokens.extend(from_tokens)
     tokens.append(";")
-    tokens.extend(id_tokens)
+    tokens.extend(id_token)
     tokens.append("<=")
     tokens.extend(to_tokens)
     tokens.append(";")
-    tokens.extend(id_tokens)
+    tokens.extend(id_token)
     tokens.extend(["++", ")"])
+    tokens.append("{")
     tokens.extend(statement_tokens)
     tokens.append("}")
+    context.exit_scope()
     return tokens
 
 
-def visit_while_statement(node, context, func_name):
+def visit_while_statement(node: Tree, context: Context, func_name: str):
     tokens = []
     for child in node.children:
         if child.data == "expression":
             tokens.append("while")
             tokens.append("(")
-            expression_tokens = visit_expression(child, context, func_name)
+            expression_tokens, expression_type = visit_expression(child, context, func_name)
             tokens.extend(expression_tokens)
             tokens.append(")")
         elif child.data == "statement":
             tokens.append("{")
             statement_tokens = visit_statement(child, context, func_name)
             tokens.extend(statement_tokens)
             tokens.append("}")
         else:
             raise Exception("Unknown while_statement child data: {}".format(child.data))
     return tokens
 
 
-def visit_statement(node, context, func_name):
+def visit_statement(node: Tree, context: Context, func_name: str):
     tokens = []
     for child in node.children:
         if child.data == "procedure_call":
             procedure_call_tokens = visit_procedure_call(child, context, func_name)
             tokens.extend(procedure_call_tokens)
         elif child.data == "compound_statement":
             compound_statement_tokens = visit_compound_statement(
@@ -639,19 +723,19 @@
         else:
             raise Exception("Unknown statement child data: {}".format(child.data))
     if len(tokens) > 0 and tokens[-1] != ";":
         tokens.append(";")
     return tokens
 
 
-def visit_const_value(node: lark.tree.Tree, context: Context):
+def visit_const_value(node: Tree, context: Context):
     tokens = []
     typename = ""
     for child in node.children:
-        if isinstance(child, lark.lexer.Token):
+        if isinstance(child, Token):
             if child.type == "PLUS":
                 tokens.append("+")
             elif child.type == "MINUS":
                 tokens.append("-")
             elif child.type == "LETTER":
                 typename = "char"
                 tokens.append("'" + child.value + "'")
@@ -665,141 +749,137 @@
             tokens.extend(num_tokens)
         else:
             raise Exception("Unknown const_value child data: {}".format(child.data))
 
     return [tokens, typename]
 
 
-def visit_const_declaration(node: lark.tree.Tree, context: Context):
+def visit_const_declaration(node: Tree, context: Context):
     tokens = []
+    const_id = ""
     for child in node.children:
-        id = ""
         if child.data == "id":
             tokens.append("const")
             # 定义const_declaration时不进行id修正
-            id = visit_id(child, context, None)
+            const_id = visit_id(child, context, "")
         elif child.data == "const_value":
             res = visit_const_value(
                 child, context
             )  # [123.456, "float"] 或 ["test", "char*"] ...
             tokens.append(res[1])
-            tokens.append(id)
+            tokens.append(const_id)
             tokens.append("=")
             tokens.extend(res[0])
             tokens.append(";")
             # 符号表注册
             # type = context.cname_to_type(res[1])
-            context.register_value(id, res[1], False, res[0])
+            context.register_value(const_id, res[1], False, res[0])
         elif child.data == "const_declaration":
             tokens.extend(visit_const_declaration(child, context))
         else:
             raise Exception(
                 "Unknown const_declaration child data: {}".format(child.data)
             )
     return tokens
 
 
-def visit_const_declarations(node: lark.tree.Tree, context: Context):
+def visit_const_declarations(node: Tree, context: Context):
     tokens = []
     for child in node.children:
         if child.data == "const_declaration":
             tokens.extend(visit_const_declaration(child, context))
         elif child.data == "empty":
             return tokens
         else:
             raise Exception(
                 "Unknown const_declarations child data: {}".format(child.data)
             )
     return tokens
 
 
-def visit_var_declaration(node: lark.tree.Tree, context: Context):
+def visit_var_declaration(node: Tree, context: Context):
     tokens = []
-    idlist = []
-    id_type = None
+    id_lists = []
+    id_types = []
     for child in node.children:
         if child.data == "idlist":
-            idlist = visit_idlist(child, context)
+            id_lists.append(visit_idlist(child, context))
         elif child.data == "type":
-            id_type = visit_type(child, context)
-        elif child.data == "var_declaration":
-            tokens.extend(visit_var_declaration(child, context))
+            id_types.append(visit_type(child, context))
         else:
             raise Exception("Unknown var_declaration child data: {}".format(child.data))
+    for id_list, id_type in zip(id_lists, id_types):
+        for id_ in id_list:
+            tokens.append(id_type["basic_type"])
+            tokens.append(id_)
+            if id_type["is_array"]:
+                for period in id_type["period"]:
+                    tokens.append("[")
+                    tokens.append(str(period[0]))
+                    tokens.append("]")
+                context.register_array(id_, id_type["basic_type"], id_type["period"])
+            else:
+                context.register_value(id_, id_type["basic_type"], True)
+            tokens.append(";")
 
-    for id in idlist:
-        tokens.append(id_type["basic_type"])
-        tokens.append(id)
-
-        if id_type["is_array"]:
-            for period in id_type["period"]:
-                tokens.append("[")
-                tokens.append(str(period[0]))
-                tokens.append("]")
-                tokens.append("[")
-                tokens.append(str(period[1]))
-                tokens.append("]")
-            context.register_array(id, id_type["basic_type"], id_type["period"])
-        else:
-            context.register_value(id, id_type["basic_type"], True)
-        tokens.append(";")
     return tokens
 
 
-def visit_var_declarations(node: lark.tree.Tree, context: Context):
+def visit_var_declarations(node: Tree, context: Context):
     tokens = []
     for child in node.children:
         if child.data == "var_declaration":
             tokens.extend(visit_var_declaration(child, context))
         elif child.data == "empty":
             return tokens
         else:
             raise Exception(
                 "Unknown var_declarations child data: {}".format(child.data)
             )
     return tokens
 
 
-def visit_program_head(node: lark.tree.Tree, context: Context):
+def visit_program_head(node: Tree, context: Context):
     # tokens = []
     # for child in node.children:
     #     if child.data == "id":
     #         id_tokens = visit_id(child,context)
     #         tokens.extend(id_tokens)
     #         tokens.append(";\n")
     #     elif child.data == "idlist":
     #         tokens.append("int ")
     #         idlist_tokens = visit_idlist(child,context)
 
     #         tokens.append(";")
     #     else:
     #         raise Exception("Unknown program_head child data: {}".format(child.data))
-    tokens = ['#include "mp2c.h"']
+    tokens = ['#include "stdio.h"']
     return tokens
 
 
-def visit_subprogram_body(node, context, subprogram_head_tokens):
+def visit_subprogram_body(node: Tree, context: Context, subprogram_head_tokens: list[str]):
     func_name = subprogram_head_tokens[1]
     ret_type = subprogram_head_tokens[0]
-    context.register_value("_" + func_name, ret_type, True)
+    if ret_type != "void":
+        context.register_value("_" + func_name, ret_type, True)
     tokens = []
     for child in node.children:
         if child.data == "const_declarations":
             tokens.extend(visit_const_declarations(child, context))
         elif child.data == "var_declarations":
             tokens.extend(visit_var_declarations(child, context))
         elif child.data == "compound_statement":
             # compound_statement中如果遇到对func_name符号的引用且并非函数递归调用，则前面加一个_
             tokens.extend(visit_compound_statement(child, context, func_name))
         else:
             raise Exception("Unknown subprogram_body child data: {}".format(child.data))
     return tokens
 
 
-def visit_subprogram(node: lark.tree.Tree, context: Context):
+def visit_subprogram(node: Tree, context: Context):
     context.enter_scope()
     tokens = []
     subprogram_head_tokens = []
     subprogram_body_tokens = []
     for child in node.children:
         if child.data == "subprogram_head":
             subprogram_head_tokens = visit_subprogram_head(child, context)
@@ -808,42 +888,41 @@
                 child, context, subprogram_head_tokens
             )
         else:
             raise Exception("Unknown subprogram child data: {}".format(child.data))
     ret_type = subprogram_head_tokens[0]
     function_name = subprogram_head_tokens[1]
     function_header = subprogram_head_tokens
-    function_tokens = ["{", ret_type, "_" + function_name, ";"]
+    function_tokens = ["{"]
+    if ret_type != "void":
+        function_tokens.extend([ret_type, "_" + function_name, ";"])
     function_tokens.extend(subprogram_body_tokens)
-    function_tokens.append("return")
-    function_tokens.append("_" + function_name)
-    function_tokens.append(";")
+    if ret_type != "void":
+        function_tokens.append("return")
+        function_tokens.append("_" + function_name)
+        function_tokens.append(";")
     function_tokens.append("}")
     context.declare_func(function_name, function_tokens)
     context.exit_scope()
     return tokens
 
 
-def visit_subprogram_declarations(node: lark.tree.Tree, context: Context):
+def visit_subprogram_declarations(node: Tree, context: Context):
     tokens = []
     for child in node.children:
         if child.data == "subprogram":
             tokens.extend(visit_subprogram(child, context))
-        elif child.data == "subprogram_declarations":
-            tokens.extend(visit_subprogram_declarations(child, context))
-        elif child.data == "empty":
-            return tokens
         else:
             raise Exception(
                 "Unknown subprogram_declarations child data: {}".format(child.data)
             )
     return tokens
 
 
-def visit_program_body(node: lark.tree.Tree, context: Context):
+def visit_program_body(node: Tree, context: Context):
     tokens = []
     for child in node.children:
         if child.data == "const_declarations":
             tokens.extend(visit_const_declarations(child, context))
         elif child.data == "var_declarations":
             tokens.extend(visit_var_declarations(child, context))
         elif child.data == "subprogram_declarations":
@@ -854,15 +933,15 @@
             tokens.extend(visit_compound_statement(child, context, "main"))
             tokens.append("}")
         else:
             raise Exception("Unknown program_body child data: {}".format(child.data))
     return tokens
 
 
-def visit_programstruct(node: lark.tree.Tree, context: Context):
+def visit_programstruct(node: Tree, context: Context):
     # 进入全局作用域
     context.enter_scope()
     tokens = []
     program_head_tokens = []
     program_body_tokens = []
     for child in node.children:
         if child.data == "program_head":
```

