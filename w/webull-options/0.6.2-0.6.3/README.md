# Comparing `tmp/webull_options-0.6.2.tar.gz` & `tmp/webull_options-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webull_options-0.6.2.tar", last modified: Sun Mar 17 00:03:40 2024, max compression
+gzip compressed data, was "webull_options-0.6.3.tar", last modified: Wed May 15 16:01:00 2024, max compression
```

## Comparing `webull_options-0.6.2.tar` & `webull_options-0.6.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-03-17 00:03:40.311317 webull_options-0.6.2/
--rw-rw-rw-   0        0        0     7368 2024-03-17 00:03:40.310313 webull_options-0.6.2/PKG-INFO
--rw-rw-rw-   0        0        0       55 2024-01-06 17:03:12.000000 webull_options-0.6.2/README.md
--rw-rw-rw-   0        0        0       42 2024-03-17 00:03:40.311317 webull_options-0.6.2/setup.cfg
--rw-rw-rw-   0        0        0      370 2024-03-16 23:56:34.000000 webull_options-0.6.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-17 00:03:40.292020 webull_options-0.6.2/webull_options/
--rw-rw-rw-   0        0        0        0 2024-01-06 17:03:12.000000 webull_options-0.6.2/webull_options/__init__.py
--rw-rw-rw-   0        0        0    15129 2024-01-06 17:03:12.000000 webull_options-0.6.2/webull_options/helpers.py
-drwxrwxrwx   0        0        0        0 2024-03-17 00:03:40.302147 webull_options-0.6.2/webull_options/models/
--rw-rw-rw-   0        0        0        0 2024-01-06 17:03:12.000000 webull_options-0.6.2/webull_options/models/__init__.py
--rw-rw-rw-   0        0        0    36853 2024-02-06 07:52:04.000000 webull_options-0.6.2/webull_options/models/db_manager.py
--rw-rw-rw-   0        0        0    23420 2024-02-27 21:35:02.000000 webull_options-0.6.2/webull_options/models/options_data.py
--rw-rw-rw-   0        0        0    46124 2024-02-29 08:45:54.000000 webull_options-0.6.2/webull_options/webull_options.py
--rw-rw-rw-   0        0        0      957 2024-02-06 07:52:33.000000 webull_options-0.6.2/webull_options/webull_trader.py
-drwxrwxrwx   0        0        0        0 2024-03-17 00:03:40.300148 webull_options-0.6.2/webull_options.egg-info/
--rw-rw-rw-   0        0        0     7368 2024-03-17 00:03:40.000000 webull_options-0.6.2/webull_options.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      433 2024-03-17 00:03:40.000000 webull_options-0.6.2/webull_options.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-17 00:03:40.000000 webull_options-0.6.2/webull_options.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     3867 2024-03-17 00:03:40.000000 webull_options-0.6.2/webull_options.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-03-17 00:03:40.000000 webull_options-0.6.2/webull_options.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 16:01:00.265092 webull_options-0.6.3/
+-rw-rw-rw-   0        0        0     7368 2024-05-15 16:01:00.265092 webull_options-0.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0       55 2024-01-06 17:03:12.000000 webull_options-0.6.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-15 16:01:00.265092 webull_options-0.6.3/setup.cfg
+-rw-rw-rw-   0        0        0      370 2024-05-15 16:00:43.000000 webull_options-0.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:01:00.255088 webull_options-0.6.3/webull_options/
+-rw-rw-rw-   0        0        0        0 2024-01-06 17:03:12.000000 webull_options-0.6.3/webull_options/__init__.py
+-rw-rw-rw-   0        0        0    15129 2024-01-06 17:03:12.000000 webull_options-0.6.3/webull_options/helpers.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:01:00.255088 webull_options-0.6.3/webull_options/models/
+-rw-rw-rw-   0        0        0        0 2024-01-06 17:03:12.000000 webull_options-0.6.3/webull_options/models/__init__.py
+-rw-rw-rw-   0        0        0    36853 2024-02-06 07:52:04.000000 webull_options-0.6.3/webull_options/models/db_manager.py
+-rw-rw-rw-   0        0        0    23420 2024-04-23 23:48:07.000000 webull_options-0.6.3/webull_options/models/options_data.py
+-rw-rw-rw-   0        0        0    47390 2024-05-15 16:00:35.000000 webull_options-0.6.3/webull_options/webull_options.py
+-rw-rw-rw-   0        0        0      957 2024-02-06 07:52:33.000000 webull_options-0.6.3/webull_options/webull_trader.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:01:00.255088 webull_options-0.6.3/webull_options.egg-info/
+-rw-rw-rw-   0        0        0     7368 2024-05-15 16:01:00.000000 webull_options-0.6.3/webull_options.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2024-05-15 16:01:00.000000 webull_options-0.6.3/webull_options.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 16:01:00.000000 webull_options-0.6.3/webull_options.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     3867 2024-05-15 16:01:00.000000 webull_options-0.6.3/webull_options.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-15 16:01:00.000000 webull_options-0.6.3/webull_options.egg-info/top_level.txt
```

### Comparing `webull_options-0.6.2/PKG-INFO` & `webull_options-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webull_options
-Version: 0.6.2
+Version: 0.6.3
 Requires-Dist: absl-py==2.0.0
 Requires-Dist: aiofiles==23.2.1
 Requires-Dist: aiohttp==3.9.3
 Requires-Dist: aiosignal==1.3.1
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: anyio==3.7.1
 Requires-Dist: appdirs==1.4.4
```

### Comparing `webull_options-0.6.2/webull_options/helpers.py` & `webull_options-0.6.3/webull_options/helpers.py`

 * *Files identical despite different names*

### Comparing `webull_options-0.6.2/webull_options/models/db_manager.py` & `webull_options-0.6.3/webull_options/models/db_manager.py`

 * *Files identical despite different names*

### Comparing `webull_options-0.6.2/webull_options/models/options_data.py` & `webull_options-0.6.3/webull_options/models/options_data.py`

 * *Files identical despite different names*

### Comparing `webull_options-0.6.2/webull_options/webull_options.py` & `webull_options-0.6.3/webull_options/webull_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,23 +37,55 @@
         self.thirty_days_from_now = (datetime.now() + timedelta(days=30)).strftime('%Y-%m-%d')
         self.fifteen_days_ago = (datetime.now() - timedelta(days=15)).strftime('%Y-%m-%d')
         self.fifteen_days_from_now = (datetime.now() + timedelta(days=15)).strftime('%Y-%m-%d')
         self.eight_days_from_now = (datetime.now() + timedelta(days=8)).strftime('%Y-%m-%d')
         self.eight_days_ago = (datetime.now() - timedelta(days=8)).strftime('%Y-%m-%d')
         self.opts = PolygonOptions(host='localhost', user='chuck', database='markets', password='fud', port=5432)
         self.most_active_tickers = ['SPY', 'QQQ', 'SPX', 'TSLA', 'AMZN', 'IWM', 'NVDA', 'VIX', 'AAPL', 'F', 'META', 'MSFT', 'GOOGL', 'HYG', 'INTC', 'SQQQ', 'AMD', 'TQQQ', 'XLF', 'BAC', 'XLI', 'TLT', 'GOOG', 'GLD', 'SOFI', 'EEM', 'EFA', 'UVXY', 'NFLX', 'ENPH', 'SQ', 'COIN', 'CVX', 'PLTR', 'XBI', 'FXI', 'XOM', 'VXX', 'PYPL', 'GDX', 'AAL', 'MARA', 'JPM', 'XLE', 'EWZ', 'PFE', 'BABA', 'AMC', 'SLV', 'SOXL', 'DIS', 'UBER', 'DIA', 'GM', 'CVNA', 'RIVN', 'RIOT', 'VALE', 'KRE', 'C', 'VZ', 'USO', 'BA', 'ARKK', 'X', 'MPW', 'XSP', 'NIO', 'SNAP', 'RUT', 'KVUE', 'EDR', 'SHOP', 'SMH', 'BMY', 'JNJ', 'KWEB', 'CHPT', 'MRNA', 'BITO', 'GOLD', 'ZM', 'T', 'NEM', 'ET', 'KO', 'PBR', 'MS', 'SCHW', 'OXY', 'MU', 'DKNG', 'RIG', 'MO', 'WFC', 'NDX', 'VFS', 'XLU', 'BKLN', 'MCD', 'ABBV', 'JBLU', 'FSLR', 'AI', 'LCID', 'SNOW', 'ABNB', 'TNA', 'DVN', 'DAL', 'RTX', 'JD', 'UNG', 'RBLX', 'TGT', 'ADBE', 'UPS', 'WDC', 'LUV', 'TSM', 'UAL', 'PAA', 'ORCL', 'PLUG', 'GS', 'LQD', 'CCL', 'LABU', 'EPD', 'WE', 'AFRM', 'XPO', 'MSOS', 'IBM', 'XLV', 'NKE', 'MSTR', 'COST', 'QCOM', 'HD', 'CSCO', 'AVGO', 'SPXS', 'CLF', 'TFC', 'GME', 'ON', 'CVS', 'CMG', 'SPXU', 'AGNC', 'XLY', 'COF', 'FCX', 'PDD', 'WMT', 'MTCH', 'NEE', 'XOP', 'CRM', 'ROKU', 'MA', 'RUN', 'SBUX', 'PARA', 'SE', 'V', 'SAVE', 'UPST', 'DXCM', 'LLY', 'NCLH', 'ABT', 'AXP', 'ABR', 'CHWY', 'AA', 'DDOG', 'SVXY', 'LYFT', 'RCL', 'HOOD', 'BEKE', 'IBB', 'LI', 'PINS', 'PANW', 'ETSY', 'YINN', 'SAVA', 'OIH', 'WBA', 'TXN', 'FEZ', 'PG', 'CCJ', 'BOIL', 'SMCI', 'ALGN', 'XLP', 'CRWD', 'GE', 'MRVL', 'BX', 'WBD', 'SOXS', 'MRK', 'W', 'UVIX', 'SPXL', 'FSR', 'TZA', 'URNM', 'CAT', 'PEP', 'IMGN', 'XPEV', 'LULU', 'CVE', 'TTD', 'CMCSA', 'BIDU', 'NLY', 'AX', 'XRT', 'AG', 'BYND', 'BRK B', 'HL', 'M', 'NWL', 'SEDG', 'SIRI', 'EBAY', 'FLEX', 'BTU', 'NKLA', 'DISH', 'MDT', 'PSEC', 'VMW', 'ZS', 'COP', 'DG', 'AMAT', 'UCO', 'MDB', 'SLB', 'PTON', 'OKTA', 'U', 'HSBC', 'XHB', 'TMUS', 'UNH', 'OSTK', 'CGC', 'NOW', 'TLRY', 'DOCU', 'TDOC', 'MMM', 'HPQ', 'PCG', 'CHTR', 'Z', 'LOW', 'PENN', 'LMT', 'WOLF', 'KMI', 'VLO', 'SPWR', 'XLK', 'DLTR', 'WHR', 'NVAX', 'ARM', 'JETS', 'VNQ', 'DE', 'DLR', 'NET', 'FAS', 'WPM', 'DASH', 'ACN', 'ASHR', 'FUBO', 'CLX', 'ADM', 'SRPT', 'MRO', 'KGC', 'DPST', 'TWLO', 'AR', 'CNC', 'FDX', 'AMGN', 'VRT', 'CLSK', 'EMB', 'KOLD', 'CD', 'HES', 'SPOT', 'XLC', 'ZIM', 'GILD', 'EQT', 'CRSP', 'GDXJ', 'STNG', 'NAT', 'HAL', 'SGEN', 'GPS', 'USB', 'QS', 'UPRO', 'KSS', 'IDXX', 'FTNT', 'BALL', 'TMF', 'PACW', 'EL', 'MULN', 'NVO', 'GDDY', 'BBY', 'SPCE', 'SNY', 'KEY', 'MGM', 'FREY', 'CZR', 'LVS', 'TTWO', 'LRCX', 'MXEF', 'PAGP', 'ANET', 'VFC', 'GRPN', 'EW', 'BKNG', 'EOSE', 'TMO', 'SPY', 'SPX', 'QQQ', 'VIX', 'IWM', 'TSLA', 'HYG', 'AMZN', 'AAPL', 'BAC', 'XLF', 'TLT', 'SLV', 'EEM', 'F', 'NVDA', 'GOOGL', 'AMD', 'AAL', 'META', 'INTC', 'PLTR', 'C', 'GLD', 'MSFT', 'GDX', 'FXI', 'VALE', 'GOOG', 'XLE', 'SOFI', 'BABA', 'NIO', 'PFE', 'EWZ', 'PYPL', 'T', 'CCL', 'SNAP', 'DIS', 'GM', 'NKLA', 'WFC', 'TQQQ', 'AMC', 'UBER', 'RIVN', 'KRE', 'PBR', 'XOM', 'LCID', 'MARA', 'JPM', 'GOLD', 'ET', 'PLUG', 'JD', 'VZ', 'WBD', 'EFA', 'KVUE', 'RIG', 'SQ', 'CHPT', 'KWEB', 'KO', 'MU', 'BITO', 'TSM', 'SQQQ', 'SHOP', 'DKNG', 'CSCO', 'XLU', 'COIN', 'MPW', 'OXY', 'SOXL', 'FCX', 'RIOT', 'DAL', 'SCHW', 'TLRY', 'BA', 'NFLX', 'UAL', 'SIRI', 'MS', 'AGNC', 'UVXY', 'XBI', 'PARA', 'ARKK', 'CMCSA', 'DVN', 'UNG', 'VXX', 'CVX', 'CLF', 'RBLX', 'PINS', 'XLI', 'SE', 'CVNA', 'QCOM', 'SGEN', 'USO', 'TMF', 'BMY', 'RTX', 'XSP', 'ORCL', 'WBA', 'NKE', 'PDD', 'X', 'KMI', 'GME', 'NCLH', 'NEM', 'SMH', 'MSOS', 'TEVA', 'M', 'XPEV', 'ABBV', 'JETS', 'ABNB', 'MULN', 'JNJ', 'MO', 'CVS', 'AFRM', 'LUV', 'NEE', 'FSR', 'AI', 'SAVE', 'JBLU', 'HOOD', 'ENPH', 'DIA', 'WMT', 'LYFT', 'NU', 'BP', 'XOP', 'ENVX', 'SPCE', 'NOK', 'GRAB', 'BYND', 'ZM', 'SLB', 'NVAX', 'U', 'MRVL', 'CCJ', 'OPEN', 'CRM', 'CGC', 'AA', 'V', 'IBM', 'PTON', 'SBUX', 'LABU', 'TGT', 'STNE', 'BRK B', 'ASHR', 'UPST', 'QS', 'MRK', 'MRNA', 'VFS', 'XHB', 'TMUS', 'SNOW', 'PANW', 'VFC', 'UPS', 'BX', 'DISH', 'USB', 'TFC', 'GE', 'COP', 'LI', 'MET', 'XRT', 'ROKU', 'XLP', 'CHWY', 'FSLR', 'PG', 'XLK', 'FUBO', 'XLV', 'W', 'AMAT', 'GOEV', 'TXN', 'PEP', 'RUN', 'SWN', 'DOW', 'HD', 'GS', 'KGC', 'Z', 'AG', 'ABR', 'CAT', 'UUP', 'AXP', 'ZIM', 'KHC', 'RCL', 'LAZR', 'BOIL', 'DDOG', 'PENN', 'TTD', 'TELL', 'XLY', 'EPD', 'CRWD', 'VMW', 'NYCB', 'HUT', 'BTU', 'DOCU', 'NET', 'BKLN', 'SU', 'BAX', 'ETSY', 'HE', 'BTG', 'NLY', 'BHC', 'TDOC', 'LUMN', 'CLSK', 'MCD', 'LVS', 'MMM', 'DM', 'ALLY', 'SPWR', 'VRT', 'ABT', 'DASH', 'ADBE', 'TNA', 'MA', 'ACB', 'MDT', 'MGM', 'COST', 'WDC', 'GSAT', 'GPS', 'ON', 'MRO', 'PAAS', 'EOSE', 'LQD', 'BILI', 'AR', 'ONON', 'HTZ', 'TWLO', 'GILD', 'MMAT', 'ASTS', 'STLA', 'LLY', 'SABR', 'BIDU', 'EDR', 'AVGO', 'HAL', 'DG', 'WYNN', 'AEM', 'PATH', 'DB', 'IYR', 'UNH', 'HL', 'IEF', 'SPXS', 'CPNG', 'URA', 'NVO', 'BITF', 'URNM', 'KSS', 'FTCH', 'KEY', 'TH', 'GEO', 'FDX', 'CL', 'AZN', 'HPQ', 'DNN', 'BSX', 'SHEL', 'DXCM', 'PCG', 'BEKE', 'DNA', 'PM', 'TTWO', 'IQ', 'WE', 'ALB', 'SAVA', 'GDXJ', 'SPXU', 'OSTK', 'COF', 'SNDL', 'OKTA', 'BXMT', 'UEC', 'VLO', 'KR', 'ZION', 'WW', 'RSP', 'XP', 'IAU', 'LULU', 'ARCC', 'SOXS', 'VOD', 'TJX', 'MOS', 'EQT', 'IONQ', 'STNG', 'NOVA', 'HLF', 'HSBC', 'ARM']
-        self.headers =  { 
-            'Access_token': os.environ.get('ACCESS_TOKEN'),
-            "Content-Type": "application/json;charset=UTF-8",
-            'Device-Type': 'Web', #
-            'Did': os.environ.get('DID'),
-            'Osv': os.environ.get('OSV'), #
-            "Hl": "en",
-            "Os": "web",
-            }
+        self.headers  = {
+        "Accept": os.getenv("ACCEPT"),
+        "Accept-Encoding": os.getenv("ACCEPT_ENCODING"),
+        "Accept-Language": "en-US,en;q=0.9",
+        'Content-Type': 'application/json',
+        "App": os.getenv("APP"),
+        "App-Group": os.getenv("APP_GROUP"),
+        "Appid": os.getenv("APPID"),
+        "Device-Type": os.getenv("DEVICE_TYPE"),
+        "Did": 'gldaboazf4y28thligawz4a7xamqu91g',
+        "Hl": os.getenv("HL"),
+        "Locale": os.getenv("LOCALE"),
+        "Origin": os.getenv("ORIGIN"),
+        "Os": os.getenv("OS"),
+        "Osv": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/124.0.0.0 Safari/537.36",
+        "Ph": os.getenv("PH"),
+        "Platform": os.getenv("PLATFORM"),
+        "Priority": os.getenv("PRIORITY"),
+        "Referer": os.getenv("REFERER"),
+        "Reqid": os.getenv("REQID"),
+        "T_time": os.getenv("T_TIME"),
+        "Tz": os.getenv("TZ"),
+        "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/124.0.0.0 Safari/537.36",
+        "Ver": os.getenv("VER"),
+        "X-S": os.getenv("X_S"),
+        "X-Sv": os.getenv("X_SV")
+    }
+        #miscellaenous
+                #sessions
+        self._account_id = ''
+        self._trade_token = ''
+        self._access_token = ''
+        self._refresh_token = ''
+        self._token_expire = ''
+        self._uuid = ''
+
+        self._region_code = 6
+        self.zone_var = 'dc_core_r001'
+        self.timeout = 15
+        self.device_id = "gldaboazf4y28thligawz4a7xamqu91g"
+        
 
         self.db_manager = DBManager(host='localhost', user=self.user, password='fud', database=self.database, port=5432)
 
 
     def human_readable(self, string):
         try:
             match = re.search(r'(\w{1,5})(\d{2})(\d{2})(\d{2})([CP])(\d+)', string) #looks for the options symbol in O: format
```

### Comparing `webull_options-0.6.2/webull_options/webull_trader.py` & `webull_options-0.6.3/webull_options/webull_trader.py`

 * *Files identical despite different names*

### Comparing `webull_options-0.6.2/webull_options.egg-info/PKG-INFO` & `webull_options-0.6.3/webull_options.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webull-options
-Version: 0.6.2
+Version: 0.6.3
 Requires-Dist: absl-py==2.0.0
 Requires-Dist: aiofiles==23.2.1
 Requires-Dist: aiohttp==3.9.3
 Requires-Dist: aiosignal==1.3.1
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: anyio==3.7.1
 Requires-Dist: appdirs==1.4.4
```

### Comparing `webull_options-0.6.2/webull_options.egg-info/requires.txt` & `webull_options-0.6.3/webull_options.egg-info/requires.txt`

 * *Files identical despite different names*

