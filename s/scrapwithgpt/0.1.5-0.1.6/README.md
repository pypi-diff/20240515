# Comparing `tmp/scrapwithgpt-0.1.5.tar.gz` & `tmp/scrapwithgpt-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapwithgpt-0.1.5.tar", last modified: Thu May  9 16:33:37 2024, max compression
+gzip compressed data, was "scrapwithgpt-0.1.6.tar", last modified: Wed May 15 08:55:43 2024, max compression
```

## Comparing `scrapwithgpt-0.1.5.tar` & `scrapwithgpt-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 16:33:37.879351 scrapwithgpt-0.1.5/
--rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 16:33:37.879133 scrapwithgpt-0.1.5/PKG-INFO
--rw-r--r--   0 henry      (501) staff       (20)      278 2024-05-09 12:31:59.000000 scrapwithgpt-0.1.5/README.md
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 16:33:37.877956 scrapwithgpt-0.1.5/scrapwithgpt/
--rw-r--r--   0 henry      (501) staff       (20)      159 2024-05-09 12:31:09.000000 scrapwithgpt-0.1.5/scrapwithgpt/__init__.py
--rw-r--r--   0 henry      (501) staff       (20)     3716 2024-05-09 16:31:32.000000 scrapwithgpt-0.1.5/scrapwithgpt/config.py
--rw-r--r--   0 henry      (501) staff       (20)     7885 2024-05-09 13:31:23.000000 scrapwithgpt-0.1.5/scrapwithgpt/oai.py
--rw-r--r--   0 henry      (501) staff       (20)     4354 2024-05-09 16:33:28.000000 scrapwithgpt-0.1.5/scrapwithgpt/prompts.py
--rw-r--r--   0 henry      (501) staff       (20)     5122 2024-05-09 13:47:50.000000 scrapwithgpt-0.1.5/scrapwithgpt/scrap.py
--rw-r--r--   0 henry      (501) staff       (20)     3262 2024-05-09 13:51:07.000000 scrapwithgpt-0.1.5/scrapwithgpt/utils.py
--rw-r--r--   0 henry      (501) staff       (20)    16221 2024-05-09 14:22:24.000000 scrapwithgpt-0.1.5/scrapwithgpt/web.py
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 16:33:37.878904 scrapwithgpt-0.1.5/scrapwithgpt.egg-info/
--rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 16:33:37.000000 scrapwithgpt-0.1.5/scrapwithgpt.egg-info/PKG-INFO
--rw-r--r--   0 henry      (501) staff       (20)      353 2024-05-09 16:33:37.000000 scrapwithgpt-0.1.5/scrapwithgpt.egg-info/SOURCES.txt
--rw-r--r--   0 henry      (501) staff       (20)        1 2024-05-09 16:33:37.000000 scrapwithgpt-0.1.5/scrapwithgpt.egg-info/dependency_links.txt
--rw-r--r--   0 henry      (501) staff       (20)       51 2024-05-09 16:33:37.000000 scrapwithgpt-0.1.5/scrapwithgpt.egg-info/requires.txt
--rw-r--r--   0 henry      (501) staff       (20)       13 2024-05-09 16:33:37.000000 scrapwithgpt-0.1.5/scrapwithgpt.egg-info/top_level.txt
--rw-r--r--   0 henry      (501) staff       (20)       38 2024-05-09 16:33:37.879394 scrapwithgpt-0.1.5/setup.cfg
--rw-r--r--   0 henry      (501) staff       (20)      566 2024-05-09 16:33:32.000000 scrapwithgpt-0.1.5/setup.py
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-15 08:55:43.679392 scrapwithgpt-0.1.6/
+-rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-15 08:55:43.679094 scrapwithgpt-0.1.6/PKG-INFO
+-rw-r--r--   0 henry      (501) staff       (20)      278 2024-05-09 12:31:59.000000 scrapwithgpt-0.1.6/README.md
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-15 08:55:43.677933 scrapwithgpt-0.1.6/scrapwithgpt/
+-rw-r--r--   0 henry      (501) staff       (20)      159 2024-05-09 12:31:09.000000 scrapwithgpt-0.1.6/scrapwithgpt/__init__.py
+-rw-r--r--   0 henry      (501) staff       (20)     3691 2024-05-15 08:53:39.000000 scrapwithgpt-0.1.6/scrapwithgpt/config.py
+-rw-r--r--   0 henry      (501) staff       (20)     7885 2024-05-09 13:31:23.000000 scrapwithgpt-0.1.6/scrapwithgpt/oai.py
+-rw-r--r--   0 henry      (501) staff       (20)     4413 2024-05-15 08:54:53.000000 scrapwithgpt-0.1.6/scrapwithgpt/prompts.py
+-rw-r--r--   0 henry      (501) staff       (20)     5237 2024-05-15 08:52:30.000000 scrapwithgpt-0.1.6/scrapwithgpt/scrap.py
+-rw-r--r--   0 henry      (501) staff       (20)     3262 2024-05-09 13:51:07.000000 scrapwithgpt-0.1.6/scrapwithgpt/utils.py
+-rw-r--r--   0 henry      (501) staff       (20)    16221 2024-05-09 14:22:24.000000 scrapwithgpt-0.1.6/scrapwithgpt/web.py
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-15 08:55:43.678861 scrapwithgpt-0.1.6/scrapwithgpt.egg-info/
+-rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-15 08:55:43.000000 scrapwithgpt-0.1.6/scrapwithgpt.egg-info/PKG-INFO
+-rw-r--r--   0 henry      (501) staff       (20)      353 2024-05-15 08:55:43.000000 scrapwithgpt-0.1.6/scrapwithgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 henry      (501) staff       (20)        1 2024-05-15 08:55:43.000000 scrapwithgpt-0.1.6/scrapwithgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 henry      (501) staff       (20)       51 2024-05-15 08:55:43.000000 scrapwithgpt-0.1.6/scrapwithgpt.egg-info/requires.txt
+-rw-r--r--   0 henry      (501) staff       (20)       13 2024-05-15 08:55:43.000000 scrapwithgpt-0.1.6/scrapwithgpt.egg-info/top_level.txt
+-rw-r--r--   0 henry      (501) staff       (20)       38 2024-05-15 08:55:43.679446 scrapwithgpt-0.1.6/setup.cfg
+-rw-r--r--   0 henry      (501) staff       (20)      566 2024-05-15 08:55:37.000000 scrapwithgpt-0.1.6/setup.py
```

### Comparing `scrapwithgpt-0.1.5/PKG-INFO` & `scrapwithgpt-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapwithgpt
-Version: 0.1.5
+Version: 0.1.6
 Home-page: https://github.com/HenryObj/scrapwithgpt
 Description-Content-Type: text/markdown
 Requires-Dist: openai>=1.9.0
 Requires-Dist: tiktoken>=0.5.2
 Requires-Dist: requests>=2.31.0
 Requires-Dist: bs4
```

### Comparing `scrapwithgpt-0.1.5/scrapwithgpt/config.py` & `scrapwithgpt-0.1.6/scrapwithgpt/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,20 +43,20 @@
 MAX_TOKEN_OUTPUT_GPT3 = 4096
 
 
 # ***** Default Prompts and output - can be transformed into objects / pull from a json file in the future.
 DEFAULT_FILTERING_CRITERIA = """
 ### Criteria ###
 The VC fund / investor should:
-a. Primarily invest in companies at early stages (pre-revenue or very early revenues).
+a. Primarily invest in companies at early stages (pre-revenue or early revenues).
 b. Invest in startups with a valuation of approximately $3M to $15M. Check that the fund does NOT typically invest small amounts for disproportionately large equity. For example investing $100K against 10% of equity.
-c. Have already invested in Edtech. The VC fund / investor should have experience with SaaS and AI.
+c. The VC fund / investor should have experience with SaaS, Edtech or AI.
 d. Not finance companies that are direct competitors in the space of 'training with simulation of interaction with fake clients'.
-e. Have made at least 5-10 investments.
-f. Be located in the US or the GCC (Gulf Cooperation Council) countries.
+e. Have made at least 5 investments.
+f. The fund is located in the US or the GCC (Gulf Cooperation Council) countries.
 ### end of the Criteria ###
 """
 
 JSON_OUTPUT_VC = """{
   "Name of the fund": "string",
   "Country": "string",
   "Number of investments": "integer",
```

### Comparing `scrapwithgpt-0.1.5/scrapwithgpt/oai.py` & `scrapwithgpt-0.1.6/scrapwithgpt/oai.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.1.5/scrapwithgpt/prompts.py` & `scrapwithgpt-0.1.6/scrapwithgpt/prompts.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         4. If the information is NOT in the content, put NA.
         {example}
         ### Important considerations:
         - Follow strictly the Instructions. 
         - You must construct a JSON object with the provided keys, populated with the relevant information. 
         - If an information is not available at ALL or does not apply, use 'NA' for those fields. Do not invent anything. ALWAYS be truthful.
         - Return the JSON and the JSON only. Do not preface by anything not even ```json before. 
-        - Do your utmost best! My job depends on the quality of your output!
+        - Do your utmost best! My job depends on the quality of your output! You will be tipped $200 for the most complete reply.
         {additional_consideration}
         """)
 
 def gen_role_summarizer() -> str:
     """
     Quick prompt for summarization. 
     """
@@ -61,15 +61,15 @@
     You take the text submitted by the user and return a detailed summary.
     You MUST ensure that you keep ALL relevant information about the main topic of the content.
                         
     ### Important Considerations: 
     - Do not include anything that is not in the provided text. ALWAYS be truthfull.
     - Do not include any recommendation. IMPORTANT, do not add useless suggestions like 'individuals can subscribe to their monthly newsletter'.
     - Do not preface the summary with anything. Do not put a title. Only return the summary and nothing else.
-    - Ensure you keep ALL contact details (email or phone number). Do not consider a website URL as a contact information.
+    - Ensure you keep ALL contact details (ALL emails and linkedin URL). Do not consider a website URL as a contact information.
     - Ensure you keep ALL numbers and factual informations.
     Do your best, my job depends on the quality of your work.
     """)
 
 # *************************************************************
 if __name__ == "__main__":
     pass
```

### Comparing `scrapwithgpt-0.1.5/scrapwithgpt/scrap.py` & `scrapwithgpt-0.1.6/scrapwithgpt/scrap.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 
     Returns:
         - The content or None if issue. The content will also be put in a file named "gptscrapper_url.txt" in the current dir. 
 
     Note:    
     full_website is True by default. We scrap the full website up to 30 pages by default. Put it to False if you want to scrap ONLY the page.
     Change the crawl_website params to scrap more (or less) pages
+
+    Model currently used is "gpt-4o" - TBD have it as a param - quick fix for now
     """
     start = time.time()
     try:
         final_content, summary = "", ""
         if full_website:
             if verbose: print(f"👷‍♂️ Crawling the full website {url}. Please be patient...")
             content = str(crawl_website(url))
@@ -45,24 +47,24 @@
             buffer_tok = MAX_TOKEN_WINDOW_GPT35_TURBO - calculate_token(role_filter) - calculate_token(content)
             if buffer_tok < MAX_TOKEN_OUTPUT_GPT3-100: # Adding -100 as security
                 print(f"The website content is too large for a single prompt - remains only {buffer_tok}\nTBD // TODO for Henry next version\nFor now we will take a subset of the content\n🔴 Information might be missing!")
                 safe_removal = int((MAX_TOKEN_OUTPUT_GPT3 - buffer_tok) * 4) * 1.362 # Adding 36% buffer on top
                 content = content[:-safe_removal]
             else:
                 buffer_tok = max(min(buffer_tok, MAX_TOKEN_OUTPUT_GPT3-100), MAX_TOKEN_OUTPUT_DEFAULT_HUGE) # basically between 3K and 4K
-            answer_from_filtergpt = ask_question_gpt(content, role_filter, max_tokens= buffer_tok, verbose=False)
+            answer_from_filtergpt = ask_question_gpt(content, role_filter, model="gpt-4o", max_tokens= buffer_tok, verbose=False)
             if not answer_from_filtergpt:
                 if verbose: print("Couldn't check the Criteria - END")
                 return
             elif "false" in answer_from_filtergpt[:10].lower(): 
                 if verbose: print(f"The website is NOT relevant according to the Criteria. Response: {answer_from_filtergpt} - END")
                 return
         if summarization:
             if verbose: print(f"👷‍♂️ Generating a summary of the website content")   
-            summary = ask_question_gpt(content, gen_role_summarizer(), max_tokens=MAX_TOKEN_OUTPUT_DEFAULT_HUGE,  verbose=False)
+            summary = ask_question_gpt(content, gen_role_summarizer(), model="gpt-4o", max_tokens=MAX_TOKEN_OUTPUT_DEFAULT_HUGE,  verbose=False)
         
         if verbose: print(f"👷‍♂️ Using GPT 4 to get the requested data")  
         result = ask_question_gpt4(content, gen_prompt_result(desired_output, example_output, additional_consideration), max_tokens=MAX_TOKEN_GPT4_RESULT,  verbose=False)
         if result:
             title = f"scrapwithgpt_{clean_url_to_filename(url)}.txt"
             if os.path.exists(title):
                 title = f"scrapwithgpt_{clean_url_to_filename(url)}_{get_now(True)}.txt" # To avoid overwriting
```

### Comparing `scrapwithgpt-0.1.5/scrapwithgpt/utils.py` & `scrapwithgpt-0.1.6/scrapwithgpt/utils.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.1.5/scrapwithgpt/web.py` & `scrapwithgpt-0.1.6/scrapwithgpt/web.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.1.5/scrapwithgpt.egg-info/PKG-INFO` & `scrapwithgpt-0.1.6/scrapwithgpt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapwithgpt
-Version: 0.1.5
+Version: 0.1.6
 Home-page: https://github.com/HenryObj/scrapwithgpt
 Description-Content-Type: text/markdown
 Requires-Dist: openai>=1.9.0
 Requires-Dist: tiktoken>=0.5.2
 Requires-Dist: requests>=2.31.0
 Requires-Dist: bs4
```

### Comparing `scrapwithgpt-0.1.5/setup.py` & `scrapwithgpt-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="scrapwithgpt",
-    version="0.1.5", # need to increment this everytime otherwise Pypi will not accept the new version
+    version="0.1.6", # need to increment this everytime otherwise Pypi will not accept the new version
      url='https://github.com/HenryObj/scrapwithgpt',
     packages=find_packages(),
     install_requires=[
         "openai>=1.9.0",
         "tiktoken>=0.5.2",
         "requests>=2.31.0",
         "bs4",
```

