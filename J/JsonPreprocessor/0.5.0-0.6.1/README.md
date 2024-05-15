# Comparing `tmp/JsonPreprocessor-0.5.0.tar.gz` & `tmp/JsonPreprocessor-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JsonPreprocessor-0.5.0.tar", last modified: Thu Apr 11 15:45:51 2024, max compression
+gzip compressed data, was "JsonPreprocessor-0.6.1.tar", last modified: Wed May 15 12:40:15 2024, max compression
```

## Comparing `JsonPreprocessor-0.5.0.tar` & `JsonPreprocessor-0.6.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:45:51.780022 JsonPreprocessor-0.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:45:51.780022 JsonPreprocessor-0.5.0/JsonPreprocessor/
--rw-r--r--   0 runner    (1001) docker     (127)    62065 2024-04-11 15:43:58.000000 JsonPreprocessor-0.5.0/JsonPreprocessor/CJsonPreprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)   324420 2024-04-11 15:45:51.000000 JsonPreprocessor-0.5.0/JsonPreprocessor/JsonPreprocessor.pdf
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-11 15:43:58.000000 JsonPreprocessor-0.5.0/JsonPreprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-11 15:43:58.000000 JsonPreprocessor-0.5.0/JsonPreprocessor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:45:51.780022 JsonPreprocessor-0.5.0/JsonPreprocessor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-11 15:45:51.000000 JsonPreprocessor-0.5.0/JsonPreprocessor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-11 15:45:51.000000 JsonPreprocessor-0.5.0/JsonPreprocessor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:45:51.000000 JsonPreprocessor-0.5.0/JsonPreprocessor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-11 15:45:51.000000 JsonPreprocessor-0.5.0/JsonPreprocessor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-11 15:43:58.000000 JsonPreprocessor-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-11 15:45:51.780022 JsonPreprocessor-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-04-11 15:43:58.000000 JsonPreprocessor-0.5.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 15:45:51.784021 JsonPreprocessor-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     9117 2024-04-11 15:43:58.000000 JsonPreprocessor-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:15.161312 JsonPreprocessor-0.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:15.161312 JsonPreprocessor-0.6.1/JsonPreprocessor/
+-rw-r--r--   0 runner    (1001) docker     (127)    67196 2024-05-15 12:38:31.000000 JsonPreprocessor-0.6.1/JsonPreprocessor/CJsonPreprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)   321294 2024-05-15 12:40:14.000000 JsonPreprocessor-0.6.1/JsonPreprocessor/JsonPreprocessor.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-15 12:38:31.000000 JsonPreprocessor-0.6.1/JsonPreprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-15 12:38:31.000000 JsonPreprocessor-0.6.1/JsonPreprocessor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:15.161312 JsonPreprocessor-0.6.1/JsonPreprocessor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-15 12:40:15.000000 JsonPreprocessor-0.6.1/JsonPreprocessor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-15 12:40:15.000000 JsonPreprocessor-0.6.1/JsonPreprocessor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 12:40:15.000000 JsonPreprocessor-0.6.1/JsonPreprocessor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 12:40:15.000000 JsonPreprocessor-0.6.1/JsonPreprocessor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-15 12:40:15.000000 JsonPreprocessor-0.6.1/JsonPreprocessor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-15 12:38:31.000000 JsonPreprocessor-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-15 12:40:15.161312 JsonPreprocessor-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-15 12:38:31.000000 JsonPreprocessor-0.6.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 12:40:15.165312 JsonPreprocessor-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     9117 2024-05-15 12:38:31.000000 JsonPreprocessor-0.6.1/setup.py
```

### Comparing `JsonPreprocessor-0.5.0/JsonPreprocessor/CJsonPreprocessor.py` & `JsonPreprocessor-0.6.1/JsonPreprocessor/CJsonPreprocessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 import sys
 import copy
 import shlex
 
 from PythonExtensionsCollection.String.CString import CString
 from enum import Enum
 from JsonPreprocessor.version import VERSION, VERSION_DATE
+from pydotdict import DotDict
 
 class CSyntaxType():
     python = "python"
     json = "json"
 
 class CNameMangling(Enum):
     AVOIDDATATYPE    = "JPavoidDataType_"
@@ -192,14 +193,16 @@
         self.currentCfg = currentCfg
         self.dUpdatedParams = {}
         self.lNestedParams = []
         self.lDotInParamName = []
         self.bDuplicatedKeys = True
         self.jsonCheck = {}
         self.JPGlobals = {}
+        self.pythonTypeError = ["object is not subscriptable", \
+                                "string indices must be integers"]
 
     def __getFailedJsonDoc(self, jsonDecodeError=None, areaBeforePosition=50, areaAfterPosition=20, oneLine=True):
         failedJsonDoc = None
         if jsonDecodeError is None:
             return failedJsonDoc
         try:
             jsonDoc = jsonDecodeError.doc
@@ -500,17 +503,25 @@
                     if int(element)<len(oTmpObj) and (isinstance(oTmpObj[int(element)], dict) or \
                                                       isinstance(oTmpObj[int(element)], list)):
                         oTmpObj = oTmpObj[int(element)]
             try:
                 ldict = {}
                 exec(sExec, locals(), ldict)
                 tmpValue = ldict['value']
-            except:
+            except Exception as error:
                 self.__reset()
-                raise Exception(f"The variable '{sNestedParam.replace('$$', '$')}' is not available!")
+                errorMsg = ''
+                for errorType in self.pythonTypeError:
+                    if errorType in str(error):
+                        errorMsg = f"Could not resolve expression '{sNestedParam.replace('$$', '$')}'."
+                if errorMsg != '':
+                    errorMsg = errorMsg + f" Reason: {error}"
+                else:
+                    errorMsg = f"The parameter '{sNestedParam.replace('$$', '$')}' is not available!"
+                raise Exception(errorMsg)
             if bKey and (isinstance(tmpValue, list) or isinstance(tmpValue, dict)):
                 self.__reset()
                 errorMsg = f"Found expression '{sNestedParam.replace('$$', '$')}' with at least one parameter of composite data type \
 ('{sNestedParam.replace('$$', '$')}' is of type {type(tmpValue)}). Because of this expression is the name of a parameter, \
 only simple data types are allowed to be substituted inside."
                 raise Exception(errorMsg)
             return tmpValue
@@ -518,15 +529,20 @@
         def __handleDotInNestedParam(sNestedParam : str) -> str:
             ddVar = re.sub(r'\$\${\s*(.*?)\s*}', '\\1', sNestedParam, re.UNICODE)
             lddVar = ddVar.split(".")
             lElements = self.__handleDotdictFormat(lddVar, [])
             sVar = '$${' + lElements[0] + '}'
             lElements.pop(0)
             for item in lElements:
-                sVar = sVar + "[" + item + "]" if re.match(r'^\d+$', item) else sVar + "['" + item + "']"
+                if re.match(r'^\d+$', item):
+                    sVar = sVar + "[" + item + "]"
+                elif re.search(r'[{}\[\]\(\)]+', item) and "${" not in item:
+                    sVar = sVar + "[" + item + "]"
+                else:
+                    sVar = sVar + "['" + item + "']"
             return sVar
 
         pattern = rf'\$\${{\s*[^{re.escape(self.specialCharacters)}]+\s*}}'
         referVars = re.findall("(" + pattern + ")", sInputStr, re.UNICODE)
         # Resolve dotdict in sInputStr
         for var in referVars:
             if var not in sInputStr:
@@ -540,14 +556,20 @@
             sLoopCheck = sInputStr
             referVars = re.findall(r'(' + tmpPattern + r')[^\[]', sInputStr, re.UNICODE)
             if len(referVars)==0:
                 referVars = re.findall(r'(' + tmpPattern + r')$', sInputStr, re.UNICODE)
             for var in referVars:
                 sVar = __handleDotInNestedParam(var[0]) if "." in var[0] else var[0]
                 tmpValue = __getNestedValue(sVar)
+                if (isinstance(tmpValue, list) or isinstance(tmpValue, dict)) and bConvertToStr:
+                    dataType = re.sub(r"^.+'([a-zA-Z]+)'.*$", "\\1", str(type(tmpValue)))
+                    self.__reset()
+                    raise Exception(f"The substitution of parameter '{sVar.replace('$$', '$')}' inside the string \
+value '{sInputStr.replace('$$', '$')}' is not supported! Composite data types like lists and dictionaries cannot \
+be substituted inside strings.")
                 while var[0] in sInputStr:
                     sLoopCheck1 = sInputStr
                     dReplacements = {"$" : "\$", "[" : "\[", "]" : "\]"}
                     varPattern = self.__multipleReplace(var[0], dReplacements)
                     if re.search(r"\[['\s]*" + varPattern + r"['\s]*\]", sInputStr):
                         if re.search(r"\[\s*'\s*" + varPattern + r"\s*'\s*\]", sInputStr):
                             sInputStr = re.sub(r"\[\s*'\s*" + varPattern + r"\s*'\s*\]", "['" + str(tmpValue) + "']", sInputStr)
@@ -556,14 +578,15 @@
                         elif isinstance(tmpValue, int):
                             sInputStr = re.sub(r"\[['\s]*" + varPattern + r"['\s]*\]", "[" + str(tmpValue) + "]", sInputStr)
                         else:
                             sInputStr = sInputStr.replace("$$", "$")
                             var = var[0].replace("$$", "$")
                             errorMsg = f"Invalid index or dictionary key in parameter '{sInputStr}'. The datatype of variable \
 '{var}' have to 'int' or 'str'."
+                            self.__reset()
                             raise Exception(errorMsg)
                     else:
                         sInputStr = sInputStr.replace(var[0], str(tmpValue))
                     if sInputStr==sLoopCheck1:
                         self.__reset()
                         raise Exception(f"Invalid expression found: '{sNestedParam}'.")
                     elif re.search(r"\[\s*\-\d+\s*\]", sInputStr):
@@ -578,26 +601,53 @@
             if re.match("^" + tmpPattern + "$", sInputStr.strip(), re.UNICODE) and bKey and not bConvertToStr:
                 rootVar = re.search(pattern, sInputStr, re.UNICODE)[0]
                 sRootVar = __handleDotInNestedParam(rootVar) if "." in rootVar else rootVar
                 sInputStr = sInputStr.replace(rootVar, sRootVar)
                 dReplacements = {"$${" : "", "}" : ""}
                 return self.__multipleReplace(sInputStr, dReplacements)
             var = re.search(tmpPattern, sInputStr, re.UNICODE)
-            rootVar = re.search(pattern, var[0], re.UNICODE)[0]
-            sRootVar = __handleDotInNestedParam(rootVar) if "." in rootVar else rootVar
-            sVar = var[0].replace(rootVar, sRootVar)
+            if var==None:
+                sVar = __handleDotInNestedParam(sInputStr) if "." in sInputStr else sInputStr
+                sVar = re.sub(r'^\s*\$\${\s*([^}]+)}', "['\\1']", sVar)
+                sExec = "value = self.JPGlobals" + sVar
+                try:
+                    ldict = {}
+                    exec(sExec, locals(), ldict)
+                    tmpValue = ldict['value']
+                except Exception as error:
+                    self.__reset()
+                    errorMsg = ''
+                    for errorType in self.pythonTypeError:
+                        if errorType in str(error):
+                            errorMsg = f"Could not resolve expression '{sNestedParam.replace('$$', '$')}'."
+                    if errorMsg != '':
+                        errorMsg = errorMsg + f" Reason: {error}"
+                    else:
+                        errorMsg = f"The parameter '{sNestedParam.replace('$$', '$')}' is not available!"
+                    raise Exception(errorMsg)
+                return tmpValue
+            else:
+                rootVar = re.search(pattern, var[0], re.UNICODE)[0]
+                sRootVar = __handleDotInNestedParam(rootVar) if "." in rootVar else rootVar
+                sVar = var[0].replace(rootVar, sRootVar)
             if re.search(r"\[\s*'[\s\-]*\d+\s*'\s*\]", sVar):
                 try:
                     tmpValue = __getNestedValue(sVar)
                 except:
                     errorMsg = f"{rootVar.replace('$$', '$')} expects integer as index. Got string instead in {sNestedParam}"
                     self.__reset()
                     raise Exception(errorMsg)
             else:
                 tmpValue = __getNestedValue(sVar)
+            if bConvertToStr and (isinstance(tmpValue, list) or isinstance(tmpValue, dict)):
+                dataType = re.sub(r"^.+'([a-zA-Z]+)'.*$", "\\1", str(type(tmpValue)))
+                self.__reset()
+                raise Exception(f"The substitution of parameter '{sVar.replace('$$', '$')}' inside the string \
+value '{sInputStr.replace('$$', '$')}' is not supported! Composite data types like lists and dictionaries cannot \
+be substituted inside strings.")
             if re.match(r"^\s*" + tmpPattern + r"\s*$", sInputStr, re.UNICODE) and not bKey:
                 return tmpValue
             else:
                 sInputStr = sInputStr.replace(var[0], str(tmpValue))
         return sInputStr.replace("$$", "$") if "$$" in sInputStr else sInputStr
 
     def __handleDotdictFormat(self, lInputListParams : list, lParams: list = []) -> list:
@@ -657,20 +707,22 @@
                 if re.match(r"^[\s\-]*\d+$", element) or \
                     re.match(rf"^'\s*[^{re.escape(self.specialCharacters)}]+\s*'$", element.strip()):
                     sExec = sExec + f"[{element}]"
                 else:
                     sExec = sExec + f"['{element}']"
                 try:
                     exec(sExec)
-                except Exception as error:
+                except Exception as error: 
                     if "list indices must be integers" in str(error):
                         if keyNested != '':
-                            errorMsg = f"Could not set variable '{keyNested}' with value '{value}'! Reason: {error}"
+                            errorMsg = f"Could not set variable '{keyNested}' with value '{value}'! \
+Reason: {str(error).replace(' or slices', '')}"
                         else:
-                            errorMsg = f"Could not set variable '{sKey}' with value '{value}'! Reason: {error}"
+                            errorMsg = f"Could not set variable '{sKey}' with value '{value}'! \
+Reason: {str(error).replace(' or slices', '')}"
                         self.__reset()
                         raise Exception(errorMsg)
                     if bCheck==True:
                         return False   # Return 'False' when detected implicit creation of data structures based on nested parameters.
                     else:
                         index = sExec.index("=")
                         sExec1 = sExec[index+1:].strip() + " = {}"
@@ -771,14 +823,33 @@
             sInputStr = self.__checkParamName(sInputStr)
             handledValue = self.__nestedParamHandler(sInputStr) if not bValueConvertString else \
                                     self.__nestedParamHandler(sInputStr, bKey=bKey, bConvertToStr=bValueConvertString)
             if bValueConvertString and not isinstance(handledValue, str):
                 handledValue = str(handledValue)
             return handledValue
 
+        def __handleList(lInput : list, bNested : bool) -> list:
+            tmpValue = []
+            for item in lInput:
+                if isinstance(item, str) and re.search(pattern, item, re.UNICODE):
+                    bNested = True
+                    initItem = item
+                    while isinstance(item, str) and "${" in item:
+                        sLoopCheck = item
+                        item = __loadNestedValue(initItem, item)
+                        if item==sLoopCheck:
+                            self.__reset()
+                            raise Exception(f"Invalid expression found: '{initItem}'.")
+                elif isinstance(item, list) and "${" in str(item):
+                    item = __handleList(item, bNested)
+                elif isinstance(item, dict) and "${" in str(item):
+                    item, bNested = self.__updateAndReplaceNestedParam(item, bNested, recursive=True)
+                tmpValue.append(item)
+            return tmpValue
+
         if bool(self.currentCfg) and not recursive:
             for k, v in self.currentCfg.items():
                 if k in self.lDataTypes:
                     k = CNameMangling.AVOIDDATATYPE.value + k
                 self.JPGlobals.update({k:v})
 
         tmpJson = copy.deepcopy(oJson)
@@ -815,43 +886,59 @@
                 while "${" in k:
                     sLoopCheck = k
                     k = __loadNestedValue(keyNested, k, bKey=True, key=keyNested)
                     if k == sLoopCheck:
                         self.__reset()
                         raise Exception(f"Invalid expression found: '{keyNested}'.")
             elif re.match(r"^\s*" + pattern + r"\s*$", k, re.UNICODE):
+                bCheckDynamicKey = False
                 keyNested = k
+                if k.count("${")>1:
+                    bCheckDynamicKey = True
                 if re.search(r"\[\s*'*" + pattern + r"'*\s*\]", keyNested, re.UNICODE) or \
                     re.search(r"\." + pattern + r"[\.}]+", keyNested, re.UNICODE):
                     bImplicitCreation = True
                 k = re.sub("\$", "$$", k)
                 k = self.__checkParamName(k)
                 k = self.__nestedParamHandler(k, bKey=True)
+                sExec = 'dummyData = self.JPGlobals'
+                dReplacements = {"[":"\[", "]":"\]", ".":"\.", "-":"\-"}
+                tmpPattern = self.__multipleReplace(parentParams, dReplacements)
+                if parentParams != '' and not re.match(r'^'+tmpPattern+r'.+$', k):
+                    tmpParam = re.sub(r'^\s*([^\[]+)', "${\\1}", parentParams) + re.sub(r'^\s*([^\[]+)', "['\\1']", k)
+                    sExec = sExec + re.sub(r'^\s*([^\[]+)', "['\\1']", parentParams) + \
+                                    re.sub(r'^\s*([^\[]+)\[*.*$', "['\\1']", k)
+                    k = parentParams + re.sub(r'^\s*([^\[]+)', "['\\1']", k) # Update absolute path of nested key
+                    try:
+                        exec(sExec)
+                    except:
+                        self.__reset()
+                        raise Exception(f"Could not set the value for parameter '{keyNested}'.\nPlease set this parameter with \
+an absolute path, for example: '{tmpParam}'")
+                elif bCheckDynamicKey:
+                    sExec = sExec + re.sub(r'^\s*([^\[]+)', "['\\1']", parentParams) + \
+                                    re.sub(r'^\s*([^\[]+)', "['\\1']", k)
+                    try:
+                        exec(sExec)
+                    except Exception as error:
+                        if 'list indices must be integers' in str(error):
+                            pass
+                        else:
+                            self.__reset()
+                            raise Exception(f"Identified dynamic name of key '{keyNested}' that does not exist. But new keys can \
+only be created based on hard code names.")
                 if bImplicitCreation and not self.__checkAndCreateNewElement(k, v, bCheck=True, keyNested=keyNested):
                     self.__reset()
                     raise Exception(f"The implicit creation of data structures based on parameter is not supported. \
 New parameter '{k}' could not be created by the expression '{keyNested}'")
             
             if isinstance(v, dict):
                 v, bNested = self.__updateAndReplaceNestedParam(v, bNested, recursive=True, parentParams=parentParams)
             elif isinstance(v, list):
-                tmpValue = []
-                for item in v:
-                    if isinstance(item, str) and re.search(pattern, item, re.UNICODE):
-                        bNested = True
-                        initItem = item
-                        while isinstance(item, str) and "${" in item:
-                            sLoopCheck = item
-                            item = __loadNestedValue(initItem, item)
-                            if item==sLoopCheck:
-                                self.__reset()
-                                raise Exception(f"Invalid expression found: '{initItem}'.")
-                    tmpValue.append(item)
-                v = tmpValue
-                del tmpValue
+                v = __handleList(v, bNested)
             elif isinstance(v, str) and self.__checkNestedParam(v):
                 if re.search(pattern, v, re.UNICODE):
                     bNested = True
                     initValue = v
                     while isinstance(v, str) and "${" in v:
                         sLoopCheck = v
                         v = __loadNestedValue(initValue, v)
@@ -974,14 +1061,16 @@
                 errorMsg = f"Expression '{sInput.replace(CNameMangling.STRINGCONVERT.value, '')}' cannot be evaluated. \
 Reason: A pair of curly brackets is empty or contains not allowed characters."
                 self.__reset()
                 raise Exception(errorMsg)
             else:
                 return True
         elif re.search(pattern2, sInput) or re.search(r"\[\s*\-\s*\d+\s*\]", sInput):
+            if CNameMangling.STRINGCONVERT.value in sInput:
+                sInput = sInput.replace(CNameMangling.STRINGCONVERT.value, '')
             errorMsg = f"Slicing is not supported! Please update the expression '{sInput}'."
             self.__reset()
             raise Exception(errorMsg)
         elif CNameMangling.STRINGCONVERT.value in sInput:
             if sInput.count("${") > sInput.count("}"):
                 sInput = re.sub(CNameMangling.STRINGCONVERT.value, "", sInput)
                 errorMsg = f"Invalid syntax! One or more than one opened or closed curly bracket is missing in expression '{sInput.strip()}'."
@@ -1055,20 +1144,17 @@
 
   / *Condition*: required / *Type*: str /
 
 **Returns:**
 
   *No return value*
         """
-        pattern = r'[\x00-\x1F\x7F]' # This pattern uses to detect double quotes and control characters.
-        if re.search(pattern, sInput) or "\\" in sInput:
-            if CNameMangling.STRINGCONVERT.value in sInput:
-                sInput = sInput.replace(CNameMangling.STRINGCONVERT.value, '')
-            errorMsg = f"Invalid key name detected: {repr(sInput)}. Key names in JSON objects must adhere to \
-the following rules: they must be strings enclosed in double quotes, must not contain control characters."
+        if CNameMangling.STRINGCONVERT.value in sInput:
+            sInput = sInput.replace(CNameMangling.STRINGCONVERT.value, '')
+            errorMsg = f"A substitution in key names is not allowed! Please update the key name {sInput}"
             self.__reset()
             raise Exception(errorMsg)
 
     def jsonLoad(self, jFile : str, masterFile : bool = True):
         """
 This method is the entry point of JsonPreprocessor.
 
@@ -1236,15 +1322,17 @@
                                 subItems = item.split(',')
                                 iSubItems = len(subItems) -1 if subItems[-1]=='' else len(subItems)
                                 newSubItem = ""
                                 j=1
                                 for subItem in subItems:
                                     if "${" in subItem:
                                         if iSubItems>1 and j<iSubItems:
-                                            if re.match(r'^\${.+$', subItem.strip()):
+                                            if subItem.count("${") < subItem.count("}") or subItem.count("[") < subItem.count("]"):
+                                                subItem = __handleLastElement(subItem)
+                                            elif re.match(r'^\${.+$', subItem.strip()):
                                                 subItem = '"' + subItem.strip() + '"'
                                             else:
                                                 subItem = re.sub(r'(\${.+$)', '"\\1"', subItem.strip())
                                         else:
                                             subItem = __handleLastElement(subItem)   
                                     if j < iSubItems:
                                         newSubItem = newSubItem + subItem + ', '
@@ -1360,14 +1448,15 @@
                 try:
                     exec(sExec)
                 except:
                     pass
                 
             self.__reset()
             __removeDuplicatedKey(oJson)
+            oJson = DotDict(oJson)
         return oJson
 
     def jsonDump(self, oJson : dict, outFile : str) -> str:
         """
 This method writes the content of a Python dictionary to a file in JSON format and returns a normalized path to this JSON file.
 
 **Arguments:**
```

### Comparing `JsonPreprocessor-0.5.0/JsonPreprocessor/JsonPreprocessor.pdf` & `JsonPreprocessor-0.6.1/JsonPreprocessor/JsonPreprocessor.pdf`

 * *Files 18% similar despite different names*

#### Comparing `JsonPreprocessor-0.5.0/JsonPreprocessor/JsonPreprocessor.pdf` & `JsonPreprocessor-0.6.1/JsonPreprocessor/JsonPreprocessor.pdf`

 * *Document info*

```diff
@@ -1,10 +1,10 @@
 Author: ''
-CreationDate: 'D:20240411154550Z'
+CreationDate: 'D:20240515124013Z'
 Creator: 'LaTeX with hyperref'
 Keywords: ''
-ModDate: 'D:20240411154550Z'
+ModDate: 'D:20240515124013Z'
 PTEX.Fullbanner: 'This is pdfTeX, Version 3.141592653-2.6-1.40.22 (TeX Live 2022/dev/Debian) kpathsea version 6.3.4/dev'
 Producer: 'pdfTeX-1.40.22'
 Subject: ''
 Title: ''
 Trapped: '/False'
```

#### pdftotext {} -

```diff
@@ -1,11 +1,11 @@
 JsonPreprocessor
-v. 0.5.0
+v. 0.6.1
 Mai Dinh Nam Son
-10.04.2024
+14.05.2024
 
 CONTENTS
 
 CONTENTS
 
 Contents
 1 Introduction
@@ -66,96 +66,90 @@
 
 dotdict notation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 18
 
 3.7
 
-Substitution of dollar operator expressions . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+Dynamic key names . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 20
 
 3.8
 
-Overwriting vs. substitution . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+Implicit creation of dictionaries . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-22
-
-3.9
-
-Implicite creation of dictionaries . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-23
+21
 
 4 CJsonPreprocessor.py
 
-25
+23
 
 4.1
 
 Class: CSyntaxType . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-25
+23
 
 4.2
 
 Class: CNameMangling . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-25
+23
 
 4.3
 
 Class: CPythonJSONDecoder . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-25
+23
 
 Method: custom scan once . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-25
+23
 
 Class: CJsonPreprocessor . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-25
+23
 
 4.4.1
 
 Method: getVersion . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-26
+24
 
 4.4.2
 
 Method: getVersionDate . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-26
+24
 
 4.4.3
 
 Method: jsonLoad . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-26
+24
 
 4.4.4
 
 Method: jsonDump
 
-26
+24
 
 4.3.1
 4.4
 
 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 5 Appendix
 
-27
+25
 
 6 History
 
-28
+26
 
 A
 
 CHAPTER 1. INTRODUCTION
 
 Chapter 1
 
@@ -293,14 +287,17 @@
 This content produces the following output:
 {'param_01': 'string',
 'param_02': 123,
 'param_03': 4.56,
 'param_04': ['A', 'B', 'C'],
 'param_05': {'A': 1, 'B': 2, 'C': 3}}
 
+This output is of a certain dictionary type (named dotdict) that allows to access elements also with an object oriented
+dot notation (details about this format can be found in section dotdict notation).
+
 5
 
 CHAPTER 3. THE JSONP FORMAT
 
 3.2
 
 3.2. BOOLEAN AND NULL VALUES
@@ -599,17 +596,25 @@
 We introduce another JSON file componentB.2.jsonp in which we import the JSON file componentB.jsonp .
 In this file we also add content to work with simple and composite data types to answer the questions above.
 
 11
 
 CHAPTER 3. THE JSONP FORMAT
 
+We introduce a new file componentB.2.jsonp
+based on already existing parameters:
+
 3.5. OVERWRITE PARAMETERS
 
-This is the initial content of componentB.2.jsonp :
+that imports
+
+componentB.jsonp
+
+and creates new parameters
+
 {
 // import of componentB parameters
 "[import]" : "./componentB.jsonp",
 //
 // some additional parameters of simple data type
 "string_val" : "ABC",
 "int_val"
@@ -631,22 +636,14 @@
 "null_val_b"
 : ${null_val},
 "common_param_1_b"
 : ${common_param_1},
 "componentB_param_2_b" : ${componentB_param_2}
 }
 
-The rules for accessing parameters are:
- Existing parameters are accessed by a dollar operator and a pair of curly brackets ( ${...} ) with the parameter
-name inside.
- If the entire expression of the right hand side of the colon is such a dollar operator expression, it is not required
-any more to encapsulate this expression in quotes.
- Without quotes, the dollar operator keeps the data type of the referenced parameter. If you use quotes, the
-value of the used parameter will be of type str .
-
 Outcome:
 {'bool_val': True,
 'bool_val_b': True,
 'common_param_1': ['common value 1.1', 'common value 1.2'],
 'common_param_1_b': ['common value 1.1', 'common value 1.2'],
 'common_param_2': {'common_key_2_1': 'common value 2.1',
 'common_key_2_2': 'common value 2.2'},
@@ -660,46 +657,108 @@
 'int_val': 123,
 'int_val_b': 123,
 'null_val': None,
 'null_val_b': None,
 'string_val': 'ABC',
 'string_val_b': 'ABC'}
 
-Let’s take a deeper look at the following line:
-"int_val_b"
-
-: ${int_val},
-
-Like mentioned in the rules above, the dollar operator keeps the data type of the referenced parameter: In case of
-int_val is of type int , also int_val_b will be of type int .
+The rules for accessing parameters are:
+ Existing parameters are accessed by a dollar operator and a pair of curly brackets ( ${...} ) with the parameter
+name inside.
+ If the entire expression of the right hand side of the colon is such a dollar operator expression, it is not required
+any more to encapsulate this expression in quotes.
+ Without quotes, the dollar operator keeps the data type of the referenced parameter. If you use quotes, the
+value of the used parameter will be converted to type str . This implicit string conversion is limited to
+parameters of simple data types like integers and floats. Composite data types like lists and dictionaries cannot
+be used for that.
 
 12
 
 CHAPTER 3. THE JSONP FORMAT
 
 3.5. OVERWRITE PARAMETERS
 
-Like mentioned in the rules above, it is not required any more to encapsulate dollar operator expressions at the right
-hand side of the colon in quotes. But nevertheless it is possible to use quotes. In case of:
+In more detail:
+The dollar operator keeps the data type of the referenced parameter. In case of
+int_val_b is of type int :
+"int_val_b"
+
+int_val
+
+is of type
+
+int , also
+
+: ${int_val},
+
+It is not required any more to encapsulate dollar operator expressions at the right hand side of the colon in quotes.
+But nevertheless, it is possible to use quotes. In case of:
 "int_val_b"
 
 : "${int_val}",
 
-the parameter int_val_b is of type string .
+the parameter int_val_b is of type str .
+Further content can be added between the double quotes. This can be used to create composite strings:
+"str_val"
+: "ABC",
+"int_val"
+: 1,
+"float_val" : 2.3,
+"bool_val"
+: True,
+"none_val"
+: None,
+"list_val"
+: [1,2,3],
+"dict_val"
+: {"A" : "B"},
+"newparam1" : "prefix_${str_val}_suffix",
+"newparam2" : "prefix_${int_val}_suffix",
+"newparam3" : "prefix_${float_val}_suffix",
+"newparam4" : "prefix_${bool_val}_suffix",
+"newparam5" : "prefix_${none_val}_suffix"
+
+Outcome:
+{'bool_val': True,
+'dict_val': {'A': 'B'},
+'float_val': 2.3,
+'int_val': 1,
+'list_val': [1, 2, 3],
+'newparam1': 'prefix_ABC_suffix',
+'newparam2': 'prefix_1_suffix',
+'newparam3': 'prefix_2.3_suffix',
+'newparam4': 'prefix_True_suffix',
+'newparam5': 'prefix_None_suffix',
+'none_val': None,
+'str_val': 'ABC'}
+
+Using composite data types inside strings causes errors:
+"newparam6" : "prefix_${listval}_suffix"
+
+or:
+"newparam7" : "prefix_${dictval}_suffix"
+
+TODO: Parameter substitution needs to be limited
 Value of a single element of a parameter of nested data type
 To access an element of a list and a key of a dictionary, we change the content of file componentB.2.jsonp to:
 {
 // import of componentB parameters
 "[import]" : "./componentB.jsonp",
 //
 "list_element_0" : ${componentB_param_1}[0],
 "dict_key_2_2"
 : ${common_param_2}['common_key_2_2']
 }
 
+13
+
+CHAPTER 3. THE JSONP FORMAT
+
+3.5. OVERWRITE PARAMETERS
+
 Outcome:
 {'common_param_1': ['common value 1.1', 'common value 1.2'],
 'common_param_2': {'common_key_2_1': 'common value 2.1',
 'common_key_2_2': 'common value 2.2'},
 'componentB_param_1': ['componentB value 1.1', 'componentB value 1.2'],
 'componentB_param_2': {'componentB_key_2_1': 'componentB value 2.1',
 'componentB_key_2_2': 'componentB value 2.2'},
@@ -725,15 +784,15 @@
 {'common_param_1': ['common value 1.1', 'common value 1.2'],
 'common_param_2': {'common_key_2_1': 'common value 2.1 (new)',
 'common_key_2_2': 'common value 2.2'},
 'componentB_param_1': ['componentB value 1.1 (new)', 'componentB value 1.2'],
 'componentB_param_2': {'componentB_key_2_1': 'componentB value 2.1',
 'componentB_key_2_2': 'componentB value 2.2'}}
 
-13
+14
 
 CHAPTER 3. THE JSONP FORMAT
 
 3.5. OVERWRITE PARAMETERS
 
 Add an element to a parameter of nested data type
 Adding further elements to an already existing list is not possible in JSON! But it is possible to add keys to an already
@@ -789,25 +848,25 @@
 'key1': 'keyA',
 'key2': 'keyB',
 'testdict': {'keyA': 'B', 'keyB': 'A'},
 'testlist': ['B', 'A'],
 'tmp1': 'A',
 'tmp2': 'A'}
 
-14
+15
 
 CHAPTER 3. THE JSONP FORMAT
 
 3.5. OVERWRITE PARAMETERS
 
 Meaning of single quotes in square brackets
 Single quotes are used to convert the content inside to a string.
- In case of the parameter param is of type string, the expressions [${param}] and ['${param}'] have
+ In case of the parameter param is of type str , the expressions [${param}] and ['${param}'] have
 the same outcome: The content inside the square brackets is a string. The single quotes have no meaning in
-this case (because the parameter is already of type string).
+this case (because the parameter is already of type str ).
  In case of the parameter param is of type integer, the quotes in ['${param}'] convert the integer value
 to a string. Without the quotes ( [${param}] ), the content inside the square brackets is an integer.
 
 In the context of JsonPreprocessor JSON files, only strings and integers are expected to be inside square brackets
 (except the brackets are used to define a list). Other data types are not supported here.
 Whether a string or an integer is expected, depends on the data type of the parameter, the square bracket expression
 belongs to. Dictionaries require a string (a key name), lists require an integer (an index). Deviations will cause an
@@ -828,74 +887,64 @@
  They belong together and therefore they are all imported into a main JSON file that is the file that is handed
 over to the JsonPreprocessor.
  Every imported JSON file introduces a certain bunch of parameters. All parameters need to be a part of a
 common dictionary.
  Outcome is that finally only one single dictionary is used to access the parameters from all JSON files imported
 in the main JSON file.
 
-To realize this, it is necessary to separate the initialization of the dictionary from all positions where keys are added
-to this dictionary.
-
-15
+16
 
 CHAPTER 3. THE JSONP FORMAT
 
 3.5. OVERWRITE PARAMETERS
 
 These are the JSON files:
  project.jsonp
 {
-// initialization
-"project_values" : {},
-//
-// add some common values
+// define some common values
 ${project_values}['common_project_param_1'] : "common project value 1",
 ${project_values}['common_project_param_2'] : "common project value 2",
 //
 // import feature parameters
 "[import]" : "./featureA.jsonp",
 "[import]" : "./featureB.jsonp",
 "[import]" : "./featureC.jsonp"
 }
 
  featureA.jsonp
 {
 // parameters required for feature A
-${project_values}['featureA_params'] : {},
 ${project_values}['featureA_params']['featureA_param_1'] : "featureA param 1 value",
 ${project_values}['featureA_params']['featureA_param_2'] : "featureA param 2 value"
 }
 
  featureB.jsonp
 {
 // parameters required for feature B
-${project_values}['featureB_params'] : {},
 ${project_values}['featureB_params']['featureB_param_1'] : "featureB param 1 value",
 ${project_values}['featureB_params']['featureB_param_2'] : "featureB param 2 value"
 }
 
  featureC.jsonp
 {
 // parameters required for feature C
-${project_values}['featureC_params'] : {},
 ${project_values}['featureC_params']['featureC_param_1'] : "featureC param 1 value",
 ${project_values}['featureC_params']['featureC_param_2'] : "featureC param 2 value"
 }
 
-16
-
-CHAPTER 3. THE JSONP FORMAT
-
-3.5. OVERWRITE PARAMETERS
+It is not required to start the code listed above, with dictionary initializations like
+"project_values" : {},
+${project_values}['featureA_params'] : {},
+${project_values}['featureB_params'] : {},
+${project_values}['featureC_params'] : {},
 
-Explanation:
-Every feature*.jsonp file refer to the dictionary inizialized within project.jsonp .
-Important is that the initialization "project_values" : {}, happens at top level ( project.jsonp ), and not
-within the imported files ( feature*.jsonp ), otherwise follow up initializations would delete previously added keys
-of this dictionary!
+These initializations are done implicitly by the JsonPreprocessor. Further details about the implicit creation of
+dictionaries can be found in section Implicit creation of dictionaries.
+It is for sure still possible to do the initialization of a dictionary explicitly with {} . But keep in mind: This deletes
+all already existing keys in this dictionary!
 Outcome:
 {'project_values': {'common_project_param_1': 'common project value 1',
 'common_project_param_2': 'common project value 2',
 'featureA_params': {'featureA_param_1': 'featureA param 1 value',
 'featureA_param_2': 'featureA param 2 value'},
 'featureB_params': {'featureB_param_1': 'featureB param 1 value',
 'featureB_param_2': 'featureB param 2 value'},
@@ -979,158 +1028,61 @@
 
 19
 
 CHAPTER 3. THE JSONP FORMAT
 
 3.7
 
-3.7. SUBSTITUTION OF DOLLAR OPERATOR EXPRESSIONS
+3.7. DYNAMIC KEY NAMES
 
-Substitution of dollar operator expressions
+Dynamic key names
 
-Like shown in previous examples, existing parameters are accessed by a dollar operator and a pair of curly brackets
-( ${...} ) with the parameter name inside.
-We discussed use cases, where the entire expression of the left hand side of the colon and also the entire expression
-of the right hand side of the colon have been either hard coded strings, encapsulated in quotes, or dollar operator
-expressions, not encapsulated in quotes.
-Also a mix of both is possible!
-Outcome is a hard coded string, encapsulated in quotes, with parts represented by one or more than one dollar
-operator expression. This can be used to create new content very dynamically: On the right hand side of the colon
-new string values can be created; on the left hand side of the colon this mechanism generates dynamic parameter
-names.
- JSON file:
-{
-"project"
-: "Test",
-"version"
-: 1.23,
-"item_number" : 1,
-"component"
-: "componentA",
-//
-"${project}_message_${item_number}" : "Component '${component}' has version ${version}"
-}
+In section Overwrite parameters we mentioned the possibility to define the value of string parameters dynamically,
+e.g. in this way:
+"str_val"
+: "ABC",
+"newparam1" : "prefix_${str_val}_suffix",
 
-Outcome:
-{'component': 'componentA',
-'item_number': 1,
-'project': 'Test',
-'Test_message_1': "Component 'componentA' has version 1.23",
-'version': 1.23}
-
-We recommend to use simple data types for this kind of substitution only!
-But nevertheless, on the right hand side of the colon also composite data types are possible. Here it might makes
-sense to use them. But on the left hand side of the colon only simple data types are allowed for substitution. Because
-it makes no sense to create parameter names based on composite data types. Most probably this would cause invalid
-key names.
-To demonstrate this, we change the JSON file to:
-{
-"component"
-: "componentA",
-"composite_data" : ["AB", 12, True, null, {"kA" : "kAval", "kB" : "kBval"}],
-//
-"test_parameter" : "Key values of component '${component}' are: ${composite_data}"
-}
+The value of newparam1 is defined by an expression that is encapsulated in quotes and contains - beneath hard
+coded parts - a dollar operator expression that is the dynamic part.
+The same is also possible on the left hand side of the colon. In this case the name of a parameter is created dynamically.
+Example:
+"strval" : "A",
+"dictval" : {"A_2" : 1},
+${dictval}['${strval}_2'] : 2
 
+In second line a new dictionary with key A_2 is defined. In third line we overwrite the initial value of this key with
+another value. The name of this key is defined with the help of parameter strval .
 Outcome:
-{'component': 'componentA',
-'composite_data': ['AB', 12, True, None, {'kA': 'kAval', 'kB': 'kBval'}],
-'test_parameter': "Key values of component 'componentA' are: ['AB', 12, True, "
-"None, {'kA': 'kAval', 'kB': 'kBval'}]"}
-
-20
-
-CHAPTER 3. THE JSONP FORMAT
-
-3.7. SUBSTITUTION OF DOLLAR OPERATOR EXPRESSIONS
-
-Now we try to do the same on the left hand side of the colon:
-{
-"param"
-: "string value",
-"composite_data" : ["AB", 12, True, null, {"kA" : "kAval", "kB" : "kBval"}],
-//
-"test_parameter_${composite_data}" : ${param}
-}
+{'dictval': {'A_2': 2}, 'strval': 'A'}
 
-If this would be allowed, the last line would cause a parameter with this name:
-"test_parameter_['AB', 12, True, None, {'kA': 'kAval', 'kB': 'kBval'}]"
+The same in dotdict notation:
+"strval" : "A",
+"dictval" : {"A_2" : 1},
+${dictval.${strval}_2} : 3
+
+The precondition for using dynamic key names is that a key with the resulting name (here A_2 )
+does exist already. Therefore this mechanism can be used to overwrite the value of existing keys, but
+cannot be used to create new keys!
+This will not work:
+"strval" : "A",
+"dictval" : {"${strval}_2" : 1}
 
-And this is absolutely not a valid name!
-To prevent the users from generating invalid parameter names, the JsonPreprocessor throws an error:
-"Error: 'Found expression '...' with at least one parameter of composite data type ...
-Because of this expression is the name of a parameter, only simple data types are ←,→ allowed to be substituted inside.'!"
+Outcome:
+TODO: error message
 
-21
+20
 
 CHAPTER 3. THE JSONP FORMAT
 
 3.8
 
-3.8. OVERWRITING VS. SUBSTITUTION
-
-Overwriting vs. substitution
-
-In this section we take a deeper look at the syntax difference between overwriting and substitution explained above.
-1. Overwriting:
-With
-
-${param2} : ${param1}
-
-"ABC"
-
-of parameter param1 .
+3.8. IMPLICIT CREATION OF DICTIONARIES
 
-the initial value
-
-"XYZ"
-
-of parameter
-
-param2
-
-is overwritten with the value
-
-{
-"param1" : "ABC",
-"param2" : "XYZ",
-//
-${param2} : ${param1},
-}
-
-Result:
-{"param1" : "ABC",
-"param2" : "ABC"}
-
-2. Substitution:
-With "${param2}" : ${param1} a new parameter with name XYZ (the value of param2 ) and value "ABC"
-is created.
-{
-"param1"
-: "ABC",
-"param2"
-: "XYZ",
-//
-"${param2}" : ${param1},
-}
-
-Result:
-{"param1" : "ABC",
-"param2" : "XYZ",
-"XYZ" : "ABC"}
-
-22
-
-CHAPTER 3. THE JSONP FORMAT
-
-3.9
-
-3.9. IMPLICITE CREATION OF DICTIONARIES
-
-Implicite creation of dictionaries
+Implicit creation of dictionaries
 
 Up to now we have discussed two different ways of creating nested dictionaries.
 The first one is “on the fly”, like:
 {
 "project_values" : {"keyA" : "keyA value",
 "keyB" : {"keyB1" : "keyB1 value",
 "keyB2" : {"keyB21" : "keyB21 value",
@@ -1178,19 +1130,19 @@
 }
 
 you will not get an error message! The entire data structure will be created implicitly. The impact is that this method
 is very susceptible to typing mistakes.
 The implicite creation of data structures does not work with lists! In case you use a list index out of range, you will
 get a corresponding error message.
 
-23
+21
 
 CHAPTER 3. THE JSONP FORMAT
 
-3.9. IMPLICITE CREATION OF DICTIONARIES
+3.8. IMPLICIT CREATION OF DICTIONARIES
 
 Key names
 The implicit creation of data structures is only possible with hard coded key names. Parameters are not supported.
 Example:
 {
 "paramA" : "ABC",
 "subKey" : "ABC",
@@ -1237,15 +1189,15 @@
 
 The same error will happen in case of the standard notation is used:
 {
 // usage of keyName 4 is not possible here
 ${testdict}['subKey_1']['subKey_2']['subKey_3'][${keyName_4}] : "XYZ"
 }
 
-24
+22
 
 CHAPTER 4. CJSONPREPROCESSOR.PY
 
 Chapter 4
 
 CJsonPreprocessor.py
 4.1
@@ -1287,15 +1239,15 @@
 from JsonPreprocessor.CJsonPreprocessor import CJsonPreprocessor
 CJsonPreprocessor extends the JSON syntax by the following features:
  Allow c/c++-style comments within JSON files
  Allow to import JSON files into JSON files
  Allow to define and use parameters within JSON files
  Allow Python keywords True, False and None
 
-25
+23
 
 CHAPTER 4. CJSONPREPROCESSOR.PY
 
 4.4.1
 
 4.4. CLASS: CJSONPREPROCESSOR
 
@@ -1344,15 +1296,15 @@
 environment variables.
 Returns:
  outFile (string)
 
 / Type: str /
 Normalized path and name of the JSON output file.
 
-26
+24
 
 CHAPTER 5. APPENDIX
 
 Chapter 5
 
 Appendix
 About this package:
@@ -1363,19 +1315,19 @@
 
 Name
 
 JsonPreprocessor
 
 Version
 
-0.5.0
+0.6.1
 
 Date
 
-10.04.2024
+14.05.2024
 
 Description
 
 Preprocessor for json files
 
 Package URL
 
@@ -1413,15 +1365,15 @@
 
 Intended Audience :: Developers
 
 Topic
 
 Topic :: Software Development
 
-27
+25
 
 CHAPTER 6. HISTORY
 
 Chapter 6
 
 History
 0.1.0
@@ -1485,18 +1437,32 @@
 0.5.0
 
 04/2024
 
 Extended debugging support. In case of JSON syntax errors, the JsonPreprocessor exception contains an extract of the JSON content nearby the position,
 where the error occurred.
 
-28
+26
 
 CHAPTER 6. HISTORY
 
+0.6.0
+
+05/2024
+
+- JsonPreprocessor returns a dotdict
+- Blocked dynamic key names
+- Improved error messages
+- Fixed bugs
+0.6.1
+
+05/2024
+
+Add pydotdict package as dependencies
+
 JsonPreprocessor.pdf
-Created at 11.04.2024 - 15:45:48
+Created at 15.05.2024 - 12:40:12
 by GenPackageDoc v. 0.41.1
 
-29
+27
```

### Comparing `JsonPreprocessor-0.5.0/JsonPreprocessor/__init__.py` & `JsonPreprocessor-0.6.1/JsonPreprocessor/__init__.py`

 * *Files identical despite different names*

### Comparing `JsonPreprocessor-0.5.0/JsonPreprocessor/version.py` & `JsonPreprocessor-0.6.1/JsonPreprocessor/version.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,10 +14,10 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # **************************************************************************************************************
 #
 # Version and date of JsonPreprocessor
 #
-VERSION      = "0.5.0"
-VERSION_DATE = "10.04.2024"
+VERSION      = "0.6.1"
+VERSION_DATE = "14.05.2024"
```

### Comparing `JsonPreprocessor-0.5.0/JsonPreprocessor.egg-info/PKG-INFO` & `JsonPreprocessor-0.6.1/JsonPreprocessor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JsonPreprocessor
-Version: 0.5.0
+Version: 0.6.1
 Summary: Preprocessor for json files
 Home-page: https://github.com/test-fullautomation/python-jsonpreprocessor
 Author: Mai Dinh Nam Son
 Author-email: son.maidinhnam@vn.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `JsonPreprocessor-0.5.0/LICENSE` & `JsonPreprocessor-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `JsonPreprocessor-0.5.0/PKG-INFO` & `JsonPreprocessor-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JsonPreprocessor
-Version: 0.5.0
+Version: 0.6.1
 Summary: Preprocessor for json files
 Home-page: https://github.com/test-fullautomation/python-jsonpreprocessor
 Author: Mai Dinh Nam Son
 Author-email: son.maidinhnam@vn.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `JsonPreprocessor-0.5.0/README.rst` & `JsonPreprocessor-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `JsonPreprocessor-0.5.0/setup.py` & `JsonPreprocessor-0.6.1/setup.py`

 * *Files identical despite different names*

