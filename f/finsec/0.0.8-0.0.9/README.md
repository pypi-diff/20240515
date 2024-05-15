# Comparing `tmp/finsec-0.0.8.tar.gz` & `tmp/finsec-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finsec-0.0.8.tar", last modified: Tue Dec 20 09:15:45 2022, max compression
+gzip compressed data, was "finsec-0.0.9.tar", last modified: Wed Oct 18 09:29:17 2023, max compression
```

## Comparing `finsec-0.0.8.tar` & `finsec-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 09:15:45.952252 finsec-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2022-12-20 09:15:36.000000 finsec-0.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2022-12-20 09:15:36.000000 finsec-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7697 2022-12-20 09:15:45.952252 finsec-0.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 09:15:45.948252 finsec-0.0.8/finsec/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2022-12-20 09:15:36.000000 finsec-0.0.8/finsec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10998 2022-12-20 09:15:36.000000 finsec-0.0.8/finsec/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2022-12-20 09:15:36.000000 finsec-0.0.8/finsec/filing.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2022-12-20 09:15:36.000000 finsec-0.0.8/finsec/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 09:15:45.952252 finsec-0.0.8/finsec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7697 2022-12-20 09:15:45.000000 finsec-0.0.8/finsec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      250 2022-12-20 09:15:45.000000 finsec-0.0.8/finsec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 09:15:45.000000 finsec-0.0.8/finsec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2022-12-20 09:15:45.000000 finsec-0.0.8/finsec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-20 09:15:45.000000 finsec-0.0.8/finsec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-20 09:15:45.952252 finsec-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2022-12-20 09:15:36.000000 finsec-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:29:17.434821 finsec-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-10-18 09:29:02.000000 finsec-0.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2023-10-18 09:29:02.000000 finsec-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10156 2023-10-18 09:29:17.434821 finsec-0.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:29:17.434821 finsec-0.0.9/finsec/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2023-10-18 09:29:02.000000 finsec-0.0.9/finsec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15054 2023-10-18 09:29:02.000000 finsec-0.0.9/finsec/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2023-10-18 09:29:02.000000 finsec-0.0.9/finsec/filing.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2023-10-18 09:29:02.000000 finsec-0.0.9/finsec/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:29:17.434821 finsec-0.0.9/finsec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10156 2023-10-18 09:29:17.000000 finsec-0.0.9/finsec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2023-10-18 09:29:17.000000 finsec-0.0.9/finsec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-18 09:29:17.000000 finsec-0.0.9/finsec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2023-10-18 09:29:17.000000 finsec-0.0.9/finsec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-10-18 09:29:17.000000 finsec-0.0.9/finsec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-18 09:29:17.434821 finsec-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2023-10-18 09:29:02.000000 finsec-0.0.9/setup.py
```

### Comparing `finsec-0.0.8/LICENSE.txt` & `finsec-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `finsec-0.0.8/finsec/base.py` & `finsec-0.0.9/finsec/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,44 +1,38 @@
 import requests
 from bs4 import BeautifulSoup as bs
 from datetime import datetime
 import pandas as pd
 import pdb
+import os
 
 _BASE_URL_ = 'https://www.sec.gov'
 _13F_SEARCH_URL_ = 'https://www.sec.gov/cgi-bin/browse-edgar?action=getcompany&CIK={}&type=13F-HR&count=100'
 _REQ_HEADERS_ = {
                     'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/97.0.4692.99 Safari/537.36',
                     'Accept-Encoding': 'gzip, deflate, br',
                     'HOST': 'www.sec.gov',
                 }
 
 class FilingBase():
     def __init__(self, cik):
         
         self.cik = self._validate_cik(cik)
-
-        self.latest_13f_cover_page = None
-
-        self.latest_13f_value = None  # !!!
-        self.latest_13f_num_holdings = None   # !!!
-
-        self.latest_holdings_table = pd.DataFrame()
-        self.latest_simplified_holdings_table = pd.DataFrame()
+        self.manager = None
         self._last_100_13f_filings_url = None
         
         self.filings = {}
 
     def _validate_cik(self, cik):
         """Check if CIK is 10 digit string."""
         if not (isinstance(cik, str) and len(cik) == 10 and cik.isdigit()):
             raise Exception("""Invalid CIK Provided""")
         return cik
 
-    def _get_13f_filings(self):
+    def _get_last_100_13f_filings_url(self):
         """Returns list of last 100 13F-HR filings."""
         if self._last_100_13f_filings_url:
             return
 
         webpage = requests.get(_13F_SEARCH_URL_.format(self.cik),headers=_REQ_HEADERS_)
         soup = bs(webpage.text,"html.parser")
         results_table = soup.find(lambda table: table.has_attr('summary') and table['summary']=="Results")
@@ -67,52 +61,66 @@
     
     def _get_bs4_text(self, bs4_obj):
         try:
             return bs4_obj.text
         except:
             return "N/A"
 
-    def _recent_qtr_year(self):
-        datetime_obj = datetime.today()
+    def _recent_qtr_year(self, datetime_o):
+        datetime_obj = datetime.strptime(datetime_o, '%Y-%m-%d')
         quarter_dict = {1:4, 2:1, 3:2, 4:3} # Every statement released is for the previous quarter.
         release_qtr = quarter_dict[(datetime_obj.month - 1)//3 + 1]
         year = datetime_obj.year
         return "Q{}-{}".format(release_qtr, year)
 
-    def _parse_13f_url(self, url):
+    def _parse_13f_url(self, url, date):
         response = requests.get(_BASE_URL_+url, headers=_REQ_HEADERS_)
         soup = bs(response.text, "html.parser")
         import re
-
-        url_primary_document = soup.find_all('a', attrs = {'href': re.compile('xml')})[1]['href'] # Primary doc is always 2nd in the list.
+        url_primary_html_document = soup.find_all('a', attrs = {'href': re.compile('xml')})[0]['href']  # Html primary doc is 1st int the list, this contains the detail on whether the dollars listed are nearest dollar or thousand dollar.
+        url_primary_document = soup.find_all('a', attrs = {'href': re.compile('xml')})[1]['href'] # XML Primary doc is always 2nd in the list.
         url_list_document = soup.find_all('a', attrs = {'href': re.compile('xml')})[3]['href'] # xml list is always 4th in the list.
 
+        response = requests.get(_BASE_URL_+url_primary_html_document, headers=_REQ_HEADERS_)
+        primary_html_doc = bs(response.text, "xml")
+
         response = requests.get(_BASE_URL_+url_primary_document, headers=_REQ_HEADERS_)
         primary_doc = bs(response.text, "xml")
 
         response = requests.get(_BASE_URL_ + url_list_document, headers=_REQ_HEADERS_)
         list_doc = bs(response.text, "xml")
 
+        # Check if the documentation is to the nearest dollar or thousand dollars. This new reporting rule came into effect in 2023 (reference: https://www.sec.gov/info/edgar/specifications/form13fxmltechspec)
+        datetime_obj = datetime.strptime(date, '%Y-%m-%d')
+        if datetime_obj.year < 2023:
+            dollar_value_multiplier = 1000
+        elif datetime_obj.year > 2023:
+            dollar_value_multiplier = 1
+        else:
+            temp_list = primary_html_doc.findAll(text=re.compile('nearest dollar'))
+            if len(temp_list)>0:
+                dollar_value_multiplier = 1
+            else:
+                dollar_value_multiplier = 1000
+
         # Get primary doc detail
         filing_manager = self._get_bs4_text(primary_doc.find("filingManager").find("name"))
         business_address = self._get_bs4_text(primary_doc.find("street1")) + ", " + self._get_bs4_text(primary_doc.find("city")) + ", " + self._get_bs4_text(primary_doc.find("stateOrCountry")) + ", " + self._get_bs4_text(primary_doc.find("zipCode"))
         submission_type = self._get_bs4_text(primary_doc.find("submissionType"))
         period_of_report = self._get_bs4_text(primary_doc.find("periodOfReport"))
 
         signature_name = self._get_bs4_text(primary_doc.find("signatureBlock").find("name"))
         signature_title = self._get_bs4_text(primary_doc.find("signatureBlock").find("title"))
         signature_phone = self._get_bs4_text(primary_doc.find("signatureBlock").find("phone"))
         signature_city = self._get_bs4_text(primary_doc.find("signatureBlock").find("city"))
         signature_state = self._get_bs4_text(primary_doc.find("signatureBlock").find("stateOrCountry"))
         signature_date = self._get_bs4_text(primary_doc.find("signatureBlock").find("signatureDate"))
 
-        portfolio_value = int(self._get_bs4_text(primary_doc.find("summaryPage").find("tableValueTotal"))) * 1000
+        portfolio_value = int(self._get_bs4_text(primary_doc.find("summaryPage").find("tableValueTotal"))) * dollar_value_multiplier
         count_holdings = int(self._get_bs4_text(primary_doc.find("summaryPage").find("tableEntryTotal")))
-        
-        
 
         filing_cover_page = {
             "filing_manager":filing_manager, 
             "business_address":business_address, 
             "submission_type":submission_type, 
             "period_of_report":period_of_report, 
             "signature_name":signature_name, 
@@ -125,95 +133,142 @@
             "count_holdings":count_holdings, 
         }
 
         # Get list doc detail
         list_of_holdings = list_doc.findAll("infoTable")
         result = []
         for each_holding in list_of_holdings:
-            name_of_issuer = each_holding.find("nameOfIssuer").text
-            title_of_class = each_holding.find("titleOfClass").text
-            cusip = each_holding.find("cusip").text
-            holding_value = int(each_holding.find("value").text) * 1000
-            share_or_principal_amount = each_holding.find("shrsOrPrnAmt").find("sshPrnamtType").text
+            name_of_issuer = self._get_bs4_text(each_holding.find("nameOfIssuer"))
+            title_of_class = self._get_bs4_text(each_holding.find("titleOfClass"))
+            cusip = self._get_bs4_text(each_holding.find("cusip"))
+            holding_value = int(each_holding.find("value").text) * dollar_value_multiplier
+            share_or_principal_amount = self._get_bs4_text(each_holding.find("shrsOrPrnAmt").find("sshPrnamtType"))
             share_or_principal_amount_count = int(each_holding.find("shrsOrPrnAmt").find("sshPrnamt").text)
             # put_or_call = each_holding.find("SOMETHING").text
-            investment_discretion = each_holding.find("investmentDiscretion").text
-            other_manager = each_holding.find("otherManager").text
+            investment_discretion = self._get_bs4_text(each_holding.find("investmentDiscretion"))
+            other_manager = self._get_bs4_text(each_holding.find("otherManager"))
             voting_authority_share_or_principal_amount_count_sole = int(each_holding.find("votingAuthority").find("Sole").text)
             voting_authority_share_or_principal_amount_count_shared = int(each_holding.find("votingAuthority").find("Shared").text)
             voting_authority_share_or_principal_amount_count_none = int(each_holding.find("votingAuthority").find("None").text)
 
             result.append({"Name of issuer":name_of_issuer, "Title of class":title_of_class, "CUSIP":cusip,"Holding value":holding_value,"Share or principal type":share_or_principal_amount,"Share or principal amount count":share_or_principal_amount_count,"Put or call":None, "Investment discretion":investment_discretion, "Other manager":other_manager, "Voting authority sole count":voting_authority_share_or_principal_amount_count_sole, "Voting authority shared count":voting_authority_share_or_principal_amount_count_shared, "Voting authority none count":voting_authority_share_or_principal_amount_count_none})
         
         holdings_table = pd.DataFrame.from_dict(result)
 
         simplified_columns = ['Name of issuer', 'Title of class', 'CUSIP', 'Share or principal type', 'Put or call','Holding value', 'Share or principal amount count']
         holdings_table_dropped_na = holdings_table[simplified_columns].dropna(axis=1)
         simplified_holdings_table = holdings_table_dropped_na.groupby(holdings_table_dropped_na.columns[:-2].to_list(), sort=False,as_index=False).sum()
 
+        if self.manager == None:
+            self.manager = filing_cover_page.get('filing_manager')
+
         return filing_cover_page, holdings_table, simplified_holdings_table
 
+    def convert_filings_to_excel(self, simplified=True, inc_cover_page_tabs=False):
+        """Outputs existing 'self.filings' dictionary to excel. Note that this will overwrite any existing files that may be present."""
+        table_type = "Simplified Holdings Table" if simplified == True else "Holdings Table"
+        if len(self.filings)>0:
+            if os.path.exists('{}.xlsx'.format(self.cik)):
+                os.remove('{}.xlsx'.format(self.cik))
+            with pd.ExcelWriter('{}.xlsx'.format(self.cik)) as writer: 
+                for qtr_year in self.filings:
+                    if inc_cover_page_tabs == True:
+                        pd.DataFrame.from_dict(self.filings[qtr_year]['Cover Page'],orient='index').to_excel(writer,sheet_name="{}_cover_pg".format(qtr_year))
+                    pd.read_json(self.filings[qtr_year][table_type]).to_excel(writer,sheet_name="{}_holdings".format(qtr_year))
+        return        
+
     def get_latest_13f_filing(self, simplified=True):
         """Returns the latest 13F-HR filing."""
-        self._get_13f_filings()
+        self._get_last_100_13f_filings_url()
+
         latest_url_date = self._last_100_13f_filings_url[0]
-        if (len(self.latest_holdings_table)>0) & (len(self.latest_simplified_holdings_table)>0):
-            if simplified==True:
-                return self.latest_simplified_holdings_table
-            else:
-                return self.latest_holdings_table
 
-        self.latest_13f_cover_page, self.latest_holdings_table, self.latest_simplified_holdings_table = self._parse_13f_url(latest_url_date[0])
-        self.latest_13f_value = self.latest_13f_cover_page['portfolio_value']
-        self.latest_13f_num_holdings = self.latest_13f_cover_page['count_holdings']
+        latest_13f_cover_page, latest_holdings_table, latest_simplified_holdings_table = self._parse_13f_url(latest_url_date[0], latest_url_date[1])
 
-        qtr_year_str = self._recent_qtr_year()
-        self.filings.update({qtr_year_str:{"Cover Page":self.latest_13f_cover_page, "Holdings Table":self.latest_holdings_table.to_json(), "Simplified Holdings Table":self.latest_simplified_holdings_table.to_json()}})
+        qtr_year_str = self._recent_qtr_year(latest_url_date[1])
+        self.filings.update({
+                        qtr_year_str:{
+                            "Cover Page":latest_13f_cover_page, 
+                            "Period of Report":latest_13f_cover_page['period_of_report'],
+                            "Holdings Table":latest_holdings_table.to_json(), 
+                            "Simplified Holdings Table":latest_simplified_holdings_table.to_json(), 
+                            "Fund Value":latest_13f_cover_page['portfolio_value'], 
+                            "Holdings Count":latest_13f_cover_page['count_holdings'],
+                            "Simplified Holdings Count":len(latest_simplified_holdings_table),
+                            "Latest 13F":True
+                            }})
         
         if simplified==True: 
-            return self.latest_simplified_holdings_table
+            return latest_simplified_holdings_table
         else: 
-            return self.latest_holdings_table
+            return latest_holdings_table
         
     def get_latest_13f_filing_cover_page(self):
         """Returns the latest 13F-HR filing cover page."""
-        if self.latest_13f_cover_page != None:
-            return self.latest_13f_cover_page
+        latest_qtr_year = [x for x in self.filings.keys() if self.filings[x]['Latest 13F']]
+        if len(latest_qtr_year) >0:
+            return self.filings[latest_qtr_year[0]]['Cover Page']
         else:
             self.get_latest_13f_filing()
+            latest_qtr_year = [x for x in self.filings.keys() if self.filings[x]['Latest 13F']]
+            return self.filings[latest_qtr_year[0]]['Cover Page']
 
     def get_latest_13f_value(self):
-        """Returns the latest 13F-HR value of holdings"""
-        if self.latest_13f_value != None:
-            return self.latest_13f_value
+        """Returns the latest 13F-HR value of fund value"""
+        latest_qtr_year = [x for x in self.filings.keys() if self.filings[x]['Latest 13F']]
+        if len(latest_qtr_year) >0:
+            return self.filings[latest_qtr_year[0]]['Fund Value']
         else:
             self.get_latest_13f_filing()
+            latest_qtr_year = [x for x in self.filings.keys() if self.filings[x]['Latest 13F']]
+            return self.filings[latest_qtr_year[0]]['Fund Value']
 
-    def get_latest_13f_num_holdings(self):
+    def get_latest_13f_num_holdings(self, holdings_type='Simplified Holdings Count'):
         """Returns the latest 13F-HR number of holdings"""
-        if self.latest_13f_num_holdings != None:
-            return self.latest_13f_num_holdings
+        latest_qtr_year = [x for x in self.filings.keys() if self.filings[x]['Latest 13F']]
+        if len(latest_qtr_year) >0:
+            return self.filings[latest_qtr_year[0]][holdings_type]
         else:
             self.get_latest_13f_filing()
+            latest_qtr_year = [x for x in self.filings.keys() if self.filings[x]['Latest 13F']]
+            return self.filings[latest_qtr_year[0]][holdings_type]
 
     def get_13f_filing(self, qtr_year: str):
         """Returns the requested 13F-HR filing."""
-        self._get_13f_filings()
+        self._get_last_100_13f_filings_url()
         if len(self.filings) != 0:
             if qtr_year in self.filings:
                 return self.filings[qtr_year]["Cover Page"], pd.read_json(self.filings[qtr_year]["Holdings Table"]), pd.read_json(self.filings[qtr_year]["Simplified Holdings Table"])
-
-        for filing in self._last_100_13f_filings_url:
+        filing_url_date = None
+        latest_13_f_filing = False
+        for index, filing in enumerate(self._last_100_13f_filings_url):
             datetime_obj = datetime.strptime(filing[1], '%Y-%m-%d')
             quarter_dict = {1:4, 2:1, 3:2, 4:3} # Every statement released is for the previous quarter.
             release_qtr = quarter_dict[(datetime_obj.month - 1)//3 + 1]
             year = datetime_obj.year
+            if release_qtr == 4:    # Anything released in the previous quarter will have a year of last year (e.g. report is for 31st Dec 2022, yet report was released on the 1st Feb 2023)
+                year = year - 1 
+
             if "Q{}-{}".format(release_qtr, year) == qtr_year:
                 filing_url_date = filing
-        
-        cover_page, holdings_table, simplified_holdings_table = self._parse_13f_url(filing_url_date[0])
-        self.filings.update({qtr_year:{"Cover Page":cover_page, "Holdings Table":holdings_table.to_json(), "Simplified Holdings Table":simplified_holdings_table.to_json()}})
+                if index == 0:
+                    latest_13_f_filing = True
+        if filing_url_date == None:
+            raise Exception("No filing could be found for the period {}".format(qtr_year))
+
+        cover_page, holdings_table, simplified_holdings_table = self._parse_13f_url(filing_url_date[0], filing_url_date[1])
+        
+        self.filings.update({
+                        qtr_year:{
+                            "Cover Page":cover_page, 
+                            "Period of Report":cover_page['period_of_report'],
+                            "Holdings Table":holdings_table.to_json(), 
+                            "Simplified Holdings Table":simplified_holdings_table.to_json(), 
+                            "Fund Value":cover_page['portfolio_value'], 
+                            "Holdings Count":cover_page['count_holdings'],
+                            "Simplified Holdings Count":len(simplified_holdings_table),
+                            "Latest 13F":latest_13_f_filing}})
 
         return cover_page, holdings_table, simplified_holdings_table
```

### Comparing `finsec-0.0.8/finsec/filing.py` & `finsec-0.0.9/finsec/filing.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 from .base import FilingBase
 
 class Filing(FilingBase):
 
     def get_a_13f_filing(self, qtr_year):
         return self.get_13f_filing(qtr_year)
 
+    def filings_to_excel(self, simplified=True, inc_cover_page_tabs=False):
+        return self.convert_filings_to_excel(simplified, inc_cover_page_tabs)
+
     @property
     def latest_13f_filing(self):
         return self.get_latest_13f_filing()
     
     @property
     def latest_13f_portfolio_value(self):
         return self.get_latest_13f_value()
@@ -24,7 +27,9 @@
     def latest_13f_filing_detailed(self):
         return self.get_latest_13f_filing(simplified=False)
 
     @property
     def latest_13f_filing_cover_page(self):
         return self.get_latest_13f_filing_cover_page()
     
+    
+
```

### Comparing `finsec-0.0.8/setup.py` & `finsec-0.0.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 import setuptools
 import io
-from os import path, walk
+from os import path
 
 # Version
 version = "unknown"
 with open("finsec/version.py") as f:
     line = f.read().strip()
     version = line.replace("version = ", "").replace('"', '')
 
 # Long Description (i.e. README file)
 here = path.abspath(path.dirname(__file__))
-# print(here)
-# for (dirpath, dirnames, filenames) in walk(here):
-#     print(filenames)
-
-# here = path.join(path.dirname(__file__))
 with io.open(path.join(here, 'README.MD'), encoding='utf-8') as f:
     long_description = f.read()
-# with open("README.md", "r") as file:
-#     long_description = file.read()
+
 # Setup
 setuptools.setup(
     name='finsec',
     version=version,
     description='Download historical filing data directly from the United States Securities Exchange Commission (SEC)!',
     long_description=long_description,
     long_description_content_type='text/markdown',
@@ -44,17 +38,21 @@
         'Topic :: Software Development :: Libraries :: Python Modules',
 
         'Programming Language :: Python :: 3.10',
     ],
     platforms=['any'],
     keywords='pandas, sec, securities exchange commission, finance, pandas datareader',
     # packages=find_packages(exclude=['contrib', 'docs', 'tests', 'examples']),
-    install_requires=['beautifulsoup4==4.11.1', 
-                        'pandas==1.3.5', 
-                        'requests==2.27.1'],
+    install_requires=['beautifulsoup4>=4.11.1', 
+                        'pandas>=1.3.5', 
+                        'requests>=2.27.1',
+                        'lxml>=4.8.0',
+                        'openpyxl>=3.0.9',
+                        ],
+
     packages=["finsec"]
     # entry_points={
     #     'console_scripts': [
     #         'sample=sample:main',
     #     ],
     # },
 )
```

