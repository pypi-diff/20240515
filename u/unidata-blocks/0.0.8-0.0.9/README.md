# Comparing `tmp/unidata_blocks-0.0.8.tar.gz` & `tmp/unidata_blocks-0.0.9.tar.gz`

## Comparing `unidata_blocks-0.0.8.tar` & `unidata_blocks-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 unidata_blocks-0.0.8/requirements.txt
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 unidata_blocks-0.0.8/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 unidata_blocks-0.0.8/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     3674 2020-02-02 00:00:00.000000 unidata_blocks-0.0.8/src/unidata_blocks/__init__.py
--rw-r--r--   0        0        0    10995 2020-02-02 00:00:00.000000 unidata_blocks-0.0.8/src/unidata_blocks/unidata/Blocks.txt
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 unidata_blocks-0.0.8/src/unidata_blocks/unidata/lang-codes.txt
--rw-r--r--   0        0        0    10964 2020-02-02 00:00:00.000000 unidata_blocks-0.0.8/src/unidata_blocks/unidata/translations/zh-hans.txt
--rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 unidata_blocks-0.0.8/tests/test_.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unidata_blocks-0.0.8/tools/__init__.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 unidata_blocks-0.0.8/tools/update.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 unidata_blocks-0.0.8/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 unidata_blocks-0.0.8/LICENSE
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 unidata_blocks-0.0.8/README.md
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 unidata_blocks-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 unidata_blocks-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 unidata_blocks-0.0.9/requirements.txt
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 unidata_blocks-0.0.9/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 unidata_blocks-0.0.9/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     3659 2020-02-02 00:00:00.000000 unidata_blocks-0.0.9/src/unidata_blocks/__init__.py
+-rw-r--r--   0        0        0    10995 2020-02-02 00:00:00.000000 unidata_blocks-0.0.9/src/unidata_blocks/unidata/Blocks.txt
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 unidata_blocks-0.0.9/src/unidata_blocks/unidata/languages.txt
+-rw-r--r--   0        0        0    10964 2020-02-02 00:00:00.000000 unidata_blocks-0.0.9/src/unidata_blocks/unidata/translations/zh-Hans.txt
+-rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 unidata_blocks-0.0.9/tests/test_.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unidata_blocks-0.0.9/tools/__init__.py
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 unidata_blocks-0.0.9/tools/update.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 unidata_blocks-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 unidata_blocks-0.0.9/LICENSE
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 unidata_blocks-0.0.9/README.md
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 unidata_blocks-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 unidata_blocks-0.0.9/PKG-INFO
```

### Comparing `unidata_blocks-0.0.8/src/unidata_blocks/__init__.py` & `unidata_blocks-0.0.9/src/unidata_blocks/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,52 +10,52 @@
 
 
 def _parse_blocks(text: str) -> tuple[str, list['UnicodeBlock']]:
     blocks = []
     lines = re.split(r'\r\n|\r|\n', text)
     version = lines[0].removeprefix('# Blocks-').removesuffix('.txt')
     for line in lines:
-        line = line.split('#', 1)[0].strip()
-        if line == '':
+        line = line.strip()
+        if line == '' or line.startswith('#'):
             continue
         tokens = re.split(r'\.\.|;\s', line)
         code_start = int(tokens[0], 16)
         code_end = int(tokens[1], 16)
         name = tokens[2]
         blocks.append(UnicodeBlock(code_start, code_end, name))
     return version, blocks
 
 
-def _parse_lang_codes(text: str) -> list[str]:
-    lang_codes = []
+def _parse_languages(text: str) -> list[str]:
+    languages = []
     lines = re.split(r'\r\n|\r|\n', text)
     for line in lines:
         line = line.strip()
         if line == '':
             continue
-        lang_codes.append(line)
-    return lang_codes
+        languages.append(line)
+    return languages
 
 
-def _parse_translations(text: str) -> dict[str, str]:
-    translations = {}
+def _parse_translation(text: str) -> dict[str, str]:
+    translation = {}
     lines = re.split(r'\r\n|\r|\n', text)
     for line in lines:
-        line = line.split('#', 1)[0].strip()
-        if line == '':
+        line = line.strip()
+        if line == '' or line.startswith('#'):
             continue
         tokens = line.split(':')
         if len(tokens) == 2:
-            translations[tokens[0].strip()] = tokens[1].strip()
-    return translations
+            translation[tokens[0].strip()] = tokens[1].strip()
+    return translation
 
 
 class UnicodeBlock:
-    _supported_languages: Final[list[str]] = _parse_lang_codes(_load_data_text('unidata/lang-codes.txt'))
-    _translations_registry: Final[dict[str, dict[str, str]]] = {}
+    _supported_languages: Final[list[str]] = _parse_languages(_load_data_text('unidata/languages.txt'))
+    _translation_registry: Final[dict[str, dict[str, str]]] = {}
 
     def __init__(self, code_start: int, code_end: int, name: str):
         self.code_start = code_start
         self.code_end = code_end
         self.name = name
         self.capacity = code_end - code_start + 1
         self.printable_count = 0
@@ -63,26 +63,26 @@
             c = chr(code_point)
             if c.isprintable():
                 self.printable_count += 1
 
     def __str__(self):
         return f'{self.code_start:04X}..{self.code_end:04X}; {self.name}'
 
-    def name_localized(self, lang_code: str, __default: str = None) -> str | None:
-        closest_language = langcodes.closest_supported_match(lang_code, UnicodeBlock._supported_languages)
+    def name_localized(self, language: str, __default: str = None) -> str | None:
+        closest_language = langcodes.closest_supported_match(language, UnicodeBlock._supported_languages)
         if closest_language is None:
             return __default
         if closest_language == 'en':
             return self.name
-        if closest_language in UnicodeBlock._translations_registry:
-            translations = UnicodeBlock._translations_registry[closest_language]
+        if closest_language in UnicodeBlock._translation_registry:
+            translation = UnicodeBlock._translation_registry[closest_language]
         else:
-            translations = _parse_translations(_load_data_text(f'unidata/translations/{closest_language.lower()}.txt'))
-            UnicodeBlock._translations_registry[closest_language] = translations
-        return translations.get(self.name, __default)
+            translation = _parse_translation(_load_data_text(f'unidata/translations/{closest_language}.txt'))
+            UnicodeBlock._translation_registry[closest_language] = translation
+        return translation.get(self.name, __default)
 
 
 def _standardize_block_name(name: str) -> str:
     return name.strip().lower().replace('-', ' ').replace('_', ' ')
 
 
 unicode_version, _blocks = _parse_blocks(_load_data_text('unidata/Blocks.txt'))
```

### Comparing `unidata_blocks-0.0.8/src/unidata_blocks/unidata/Blocks.txt` & `unidata_blocks-0.0.9/src/unidata_blocks/unidata/Blocks.txt`

 * *Files identical despite different names*

### Comparing `unidata_blocks-0.0.8/src/unidata_blocks/unidata/translations/zh-hans.txt` & `unidata_blocks-0.0.9/src/unidata_blocks/unidata/translations/zh-Hans.txt`

 * *Files identical despite different names*

### Comparing `unidata_blocks-0.0.8/tests/test_.py` & `unidata_blocks-0.0.9/tests/test_.py`

 * *Files identical despite different names*

### Comparing `unidata_blocks-0.0.8/tools/update.py` & `unidata_blocks-0.0.9/tools/update.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,57 +9,56 @@
 blocks_doc_url = 'https://www.unicode.org/Public/UNIDATA/Blocks.txt'
 
 project_root_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), '..'))
 unidata_dir = os.path.join(project_root_dir, 'src', 'unidata_blocks', 'unidata')
 blocks_file_name = 'Blocks.txt'
 blocks_file_path = os.path.join(unidata_dir, blocks_file_name)
 translations_dir = os.path.join(unidata_dir, 'translations')
-translations_tmp_dir = os.path.join(project_root_dir, 'build', 'tmp', 'translations')
-lang_codes_file_path = os.path.join(unidata_dir, 'lang-codes.txt')
+translations_tmp_dir = os.path.join(project_root_dir, 'build', 'translations')
+languages_file_path = os.path.join(unidata_dir, 'languages.txt')
 
 
 def main():
     response = requests.get(blocks_doc_url)
     assert response.ok
     assert 'text/plain' in response.headers['Content-Type']
     with open(blocks_file_path, 'w', encoding='utf-8') as file:
         file.write(response.text)
     unicode_version, blocks = unidata_blocks._parse_blocks(response.text)
 
     if os.path.exists(translations_tmp_dir):
         shutil.rmtree(translations_tmp_dir)
     os.makedirs(translations_tmp_dir)
 
-    lang_codes = ['en']
+    languages = ['en']
 
-    for lang_file_name in os.listdir(translations_dir):
-        if not lang_file_name.endswith('.txt'):
+    for translation_file_name in os.listdir(translations_dir):
+        if not translation_file_name.endswith('.txt'):
             continue
-        lang_code = langcodes.standardize_tag(lang_file_name.removesuffix('.txt'))
-        assert f'{lang_code.lower()}.txt' == lang_file_name, f"Illegal file name: '{lang_file_name}'"
-        lang_codes.append(lang_code)
-
-        lang_file_path = os.path.join(translations_dir, lang_file_name)
-        with open(lang_file_path, 'r', encoding='utf-8') as file:
-            translations = unidata_blocks._parse_translations(file.read())
+        language = langcodes.standardize_tag(translation_file_name.removesuffix('.txt'))
+        languages.append(language)
 
-        lang_tmp_file_path = os.path.join(translations_tmp_dir, lang_file_name)
-        with open(lang_tmp_file_path, 'w', encoding='utf-8') as file:
+        translation_file_path = os.path.join(translations_dir, translation_file_name)
+        with open(translation_file_path, 'r', encoding='utf-8') as file:
+            translation = unidata_blocks._parse_translation(file.read())
+
+        translation_tmp_file_path = os.path.join(translations_tmp_dir, translation_file_name)
+        with open(translation_tmp_file_path, 'w', encoding='utf-8') as file:
             file.write(f'# Unicode: {unicode_version}\n')
-            file.write(f'# {lang_code}\n\n')
+            file.write(f'# {language}\n\n')
             for block in blocks:
-                localized_name = translations.get(block.name, None)
+                localized_name = translation.get(block.name, None)
                 if localized_name is None:
                     file.write(f'# TODO # {block.name}:\n')
                 else:
                     file.write(f'{block.name}: {localized_name}\n')
     shutil.rmtree(translations_dir)
     os.rename(translations_tmp_dir, translations_dir)
 
-    lang_codes.sort()
-    with open(lang_codes_file_path, 'w', encoding='utf-8') as file:
-        file.write('\n'.join(lang_codes))
+    languages.sort()
+    with open(languages_file_path, 'w', encoding='utf-8') as file:
+        file.write('\n'.join(languages))
         file.write('\n')
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `unidata_blocks-0.0.8/.gitignore` & `unidata_blocks-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `unidata_blocks-0.0.8/LICENSE` & `unidata_blocks-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `unidata_blocks-0.0.8/README.md` & `unidata_blocks-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `unidata_blocks-0.0.8/pyproject.toml` & `unidata_blocks-0.0.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "unidata-blocks"
-version = "0.0.8"
+version = "0.0.9"
 description = "A library that helps query unicode blocks by Blocks.txt."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.10"
 authors = [
     { name = "TakWolf" },
 ]
```

### Comparing `unidata_blocks-0.0.8/PKG-INFO` & `unidata_blocks-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unidata-blocks
-Version: 0.0.8
+Version: 0.0.9
 Summary: A library that helps query unicode blocks by Blocks.txt.
 Project-URL: homepage, https://github.com/TakWolf/unidata-blocks
 Project-URL: source, https://github.com/TakWolf/unidata-blocks
 Project-URL: issues, https://github.com/TakWolf/unidata-blocks/issues
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
```

