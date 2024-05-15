# Comparing `tmp/Fr1997v011-1.5.3.tar.gz` & `tmp/Fr1997v011-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fr1997v011-1.5.3.tar", last modified: Sat May 11 08:38:26 2024, max compression
+gzip compressed data, was "Fr1997v011-1.5.4.tar", last modified: Wed May 15 09:56:29 2024, max compression
```

## Comparing `Fr1997v011-1.5.3.tar` & `Fr1997v011-1.5.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 08:38:26.973842 Fr1997v011-1.5.3/
-drwxrwxrwx   0        0        0        0 2024-05-11 08:38:26.935323 Fr1997v011-1.5.3/Fr1997v011.egg-info/
--rw-rw-rw-   0        0        0      182 2024-05-11 08:38:26.000000 Fr1997v011-1.5.3/Fr1997v011.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-05-11 08:38:26.000000 Fr1997v011-1.5.3/Fr1997v011.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 08:38:26.000000 Fr1997v011-1.5.3/Fr1997v011.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-11 08:38:26.000000 Fr1997v011-1.5.3/Fr1997v011.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2024-05-11 08:38:26.000000 Fr1997v011-1.5.3/Fr1997v011.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.5.3/LICENSE
--rw-rw-rw-   0        0        0      182 2024-05-11 08:38:26.958325 Fr1997v011-1.5.3/PKG-INFO
--rw-rw-rw-   0        0        0      773 2024-05-11 06:06:25.000000 Fr1997v011-1.5.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 08:38:26.939323 Fr1997v011-1.5.3/fr1997_mode/
--rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.5.3/fr1997_mode/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 08:38:26.946325 Fr1997v011-1.5.3/fr1997_mode/mode_func/
--rw-rw-rw-   0        0        0       29 2024-04-25 01:03:20.000000 Fr1997v011-1.5.3/fr1997_mode/mode_func/__init__.py
--rw-rw-rw-   0        0        0   178059 2024-05-11 08:38:24.000000 Fr1997v011-1.5.3/fr1997_mode/mode_func/all_func.py
-drwxrwxrwx   0        0        0        0 2024-05-11 08:38:26.949325 Fr1997v011-1.5.3/fr1997_mode/mode_static/
--rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.5.3/fr1997_mode/mode_static/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-11 08:38:26.973842 Fr1997v011-1.5.3/setup.cfg
--rw-rw-rw-   0        0        0      322 2024-05-11 08:38:24.000000 Fr1997v011-1.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 09:56:29.424118 Fr1997v011-1.5.4/
+drwxrwxrwx   0        0        0        0 2024-05-15 09:56:29.404499 Fr1997v011-1.5.4/Fr1997v011.egg-info/
+-rw-rw-rw-   0        0        0      182 2024-05-15 09:56:29.000000 Fr1997v011-1.5.4/Fr1997v011.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-05-15 09:56:29.000000 Fr1997v011-1.5.4/Fr1997v011.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 09:56:29.000000 Fr1997v011-1.5.4/Fr1997v011.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-14 11:04:08.000000 Fr1997v011-1.5.4/Fr1997v011.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2024-05-15 09:56:29.000000 Fr1997v011-1.5.4/Fr1997v011.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.5.4/LICENSE
+-rw-rw-rw-   0        0        0      182 2024-05-15 09:56:29.421110 Fr1997v011-1.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0      773 2024-05-14 11:04:15.000000 Fr1997v011-1.5.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 09:56:29.409019 Fr1997v011-1.5.4/fr1997_mode/
+-rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.5.4/fr1997_mode/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 09:56:29.413535 Fr1997v011-1.5.4/fr1997_mode/mode_func/
+-rw-rw-rw-   0        0        0       29 2024-04-25 01:03:20.000000 Fr1997v011-1.5.4/fr1997_mode/mode_func/__init__.py
+-rw-rw-rw-   0        0        0   181260 2024-05-15 09:56:27.000000 Fr1997v011-1.5.4/fr1997_mode/mode_func/all_func.py
+drwxrwxrwx   0        0        0        0 2024-05-15 09:56:29.418049 Fr1997v011-1.5.4/fr1997_mode/mode_static/
+-rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.5.4/fr1997_mode/mode_static/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-15 09:56:29.424118 Fr1997v011-1.5.4/setup.cfg
+-rw-rw-rw-   0        0        0      322 2024-05-14 11:04:05.000000 Fr1997v011-1.5.4/setup.py
```

### Comparing `Fr1997v011-1.5.3/LICENSE` & `Fr1997v011-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Fr1997v011-1.5.3/README.md` & `Fr1997v011-1.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ```sh
 python setup.py sdist
 ```
 
 ### （本地）安装包
 
 ```sh
-pip install dist/Fr1997v011-1.5.2.tar.gz
+pip install dist/Fr1997v011-1.5.4.tar.gz
 ```
 
 ### 下载包
 
 ```sh
 pip install Fr1997v011
 ```
```

### Comparing `Fr1997v011-1.5.3/fr1997_mode/mode_func/all_func.py` & `Fr1997v011-1.5.4/fr1997_mode/mode_func/all_func.py`

 * *Files 2% similar despite different names*

```diff
@@ -385,14 +385,22 @@
         cookies_list = [cookie.split(';')[0] for cookie in cookies_list]
 
         # 拼接所有的Cookie
         cookie_str = ";".join(cookies_list)
 
         return cookie_str
 
+    # 增长率
+    @staticmethod
+    def add_rate(v_new, v_old):
+        if v_new == 0 or v_old == 0:
+            rate = 0
+        else:
+            rate = round((v_new - v_old) / v_old * 100, 2)
+        return rate
 
 # requests 封装
 class HttpJike(object):
 
     def __init__(self):
         self.status_code = 500
         self.msg = 'ok'
@@ -2192,14 +2200,111 @@
             else:
                 result = ""
         except:
             print("err ttwid_cookie获取失败")
         if result:
             return result
 
+    # 千川指数
+    def qianchuan_index_req(self, cookie_use, word):
+        cookies = []
+        all_cookie = mode_pro.qianchuan_index_cookie()  # 具有缓存性
+        for cookie in all_cookie:
+            if cookie['id_id'] in cookie_use:
+                cookies.append(cookie)
+
+        cookie = random.choice(cookies)
+        acc = cookie['id_id']
+
+        t0 = mode_time.zero_clock()
+        t30 = t0 - 86400 * 30
+        data = {"word": word, "start_datetime": t30, "end_datetime": t0}
+
+        try:
+            response = requests.post(
+                f'https://ad.oceanengine.com/platform/api/v1/search_ad/search_trend_v2/?aadvid={cookie["aadvid"]}',
+                # 监控
+                headers=cookie['headers'],
+                cookies=cookie['cookies'],
+                data=json.dumps(data)
+            )
+            if response.status_code == 200:
+                data_data = response.json()
+                code = data_data.get('code')
+                data = data_data.get('data')
+                if code == 0 and data:
+                    return {'code': 200, 'msg': 'ok', 'data': mode_pro.keyword_day_index_get(data=data), 'acc': acc}
+                else:
+                    return {'code': 500, 'msg': f'err 1', 'acc': acc}
+            else:
+                return {'code': 500, 'msg': f'err:{response.status_code}', 'acc': acc}
+        except Exception as E:
+            return {'code': 500, 'msg': 'err 2', 'acc': acc}
+
+    # 千川指数
+    def qianchuan_index_data_do(self, day_index, _id):
+        # 日均值
+        day_index_new = [i['v'] for i in day_index]
+        day_index_new.sort()
+        day_index_new = day_index_new[1:][:-1]
+        index_avg = mode_data.list_avg(day_index_new)
+        if index_avg is None:
+            index_avg = 0
+
+        # 计算中位数
+        if day_index:
+            day_index_new = [i['v'] for i in day_index]
+            median = mode_data.list_median(day_index_new)
+        else:
+            median = 0
+
+        return {
+            'is_open': 1,
+            'keyword': _id,
+            'day_index': day_index,  # 日指数
+            'median': median,  # 中位数
+            'index_avg': index_avg,  # 平均数
+        }
+
+    # 千川指数 批量存储
+    def qianchuan_index_save(self, save_data):
+        should_keyword = []
+        keyword_index_doc = []
+        keyword_index_sign_doc = []
+        if save_data:
+            for i in save_data:
+                _id = i['keyword']
+                should_keyword.append(_id)
+            is_in, is_in_data, shoulds_not = mode_pro.es_in_or_notins('dso_douyin_keyword_alias', should_keyword)
+            for i in save_data:
+                _id = i['keyword']
+                keyword_index_doc.append({"index": {"_id": f"{_id}"}})
+                keyword_index_doc.append({
+                    'is_open': i['is_open'],
+                    'keyword': _id,  # 平均指数
+                    'day_index': i['day_index'],  # 日指数
+                    'median': i['median'],  # 中位数
+                    'index_avg': i['index_avg'],  # 平均数
+                    'create_time': int(time.time()),
+                    'update_time': int(time.time()),
+                })
+
+                # 同步到关键词表
+                if _id in is_in_data:
+                    keyword_pinyin = mode_pro.chinese_to_pinyin(chinese=_id, ret=3)
+                    keyword_index_sign_doc.append(
+                        {'update': {'_index': f"dso_douyin_keyword_{keyword_pinyin}", '_id': _id}})
+                    keyword_index_sign_doc.append({'doc': {
+                        'index_avg_new': i['index_avg'],
+                        'median_new': i.get('median', 0),
+                        'update_index_time': int(time.time()),
+                    }})
+        mode_pro.es_create_update(doc=keyword_index_doc, index='douyin_keyword_index')
+        mode_pro.es_create_update_noIndex(doc=keyword_index_sign_doc)
+
 
 # 小红书
 class XhsJike:
 
     def xhs_web_video_main_data(self, data_json, note_id):
         def ret_json(code=200, msg=None, data=None):
             return {'code': code, 'msg': msg, 'data': data}
@@ -3274,50 +3379,27 @@
             cache_set('jike_qianchuan_ad_cookie', data_list, 200)
         return data_list
 
     # 关键词日数据 数据分析
     @staticmethod
     def keyword_day_index_get(data):
         """
-        [{'t': 1691164800, 'v': 2595}, {'t': 1691251200, 'v': 2292}, {'t': 1691337600, 'v': 2048}, {'t': 1691424000, 'v': 1965}, {'t': 1691510400, 'v': 2095}, {'t': 1691596800, 'v': 2503}, {'t': 1691683200, 'v': 2177}, {'t': 1691769600, 'v': 2166}, {'t': 1691856000, 'v': 1997}, {'t': 1691942400, 'v': 2025}, {'t': 1692028800, 'v': 2030}, {'t': 1692115200, 'v': 2159}, {'t': 1692201600, 'v': 2648}, {'t': 1692288000, 'v': 2107}, {'t': 1692374400, 'v': 2392}, {'t': 1692460800, 'v': 2378}, {'t': 1692547200, 'v': 2173}, {'t': 1692633600, 'v': 2093}, {'t': 1692720000, 'v': 2020}, {'t': 1692806400, 'v': 1969}, {'t': 1692892800, 'v': 2244}, {'t': 1692979200, 'v': 2924}, {'t': 1693065600, 'v': 2697}, {'t': 1693152000, 'v': 2454}, {'t': 1693238400, 'v': 2431}, {'t': 1693324800, 'v': 2221}, {'t': 1693411200, 'v': 2254}, {'t': 1693497600, 'v': 1748}, {'t': 1693584000, 'v': 2087}, {'t': 1693670400, 'v': 1912}]
+        原：[{'date': '2024-04-14', 'pv': 39078}, {'date': '2024-04-15', 'pv': 20346},
+        变：[{'t': 1691164800, 'v': 2595}, {'t': 1691251200, 'v': 2292}, {'t': 1691337600, 'v': 2048}, {'t': 1691424000, 'v': 1965}, {'t': 1691510400, 'v': 2095}, {'t': 1691596800, 'v': 2503}, {'t': 1691683200, 'v': 2177}, {'t': 1691769600, 'v': 2166}, {'t': 1691856000, 'v': 1997}, {'t': 1691942400, 'v': 2025}, {'t': 1692028800, 'v': 2030}, {'t': 1692115200, 'v': 2159}, {'t': 1692201600, 'v': 2648}, {'t': 1692288000, 'v': 2107}, {'t': 1692374400, 'v': 2392}, {'t': 1692460800, 'v': 2378}, {'t': 1692547200, 'v': 2173}, {'t': 1692633600, 'v': 2093}, {'t': 1692720000, 'v': 2020}, {'t': 1692806400, 'v': 1969}, {'t': 1692892800, 'v': 2244}, {'t': 1692979200, 'v': 2924}, {'t': 1693065600, 'v': 2697}, {'t': 1693152000, 'v': 2454}, {'t': 1693238400, 'v': 2431}, {'t': 1693324800, 'v': 2221}, {'t': 1693411200, 'v': 2254}, {'t': 1693497600, 'v': 1748}, {'t': 1693584000, 'v': 2087}, {'t': 1693670400, 'v': 1912}]
         """
         day_index = []
         keyword_pv_trend = data.get('keyword_pv_trend')
         if keyword_pv_trend:
             for i in keyword_pv_trend:
                 t = i['date']
                 v = i['pv']
                 timestamp1 = int(time.mktime(time.strptime(t, '%Y-%m-%d')))
                 day_index.append({'t': timestamp1, 'v': v})
         return day_index
 
-    # 关键词日数据 存储
-    def keyword_day_index_save(self, save_data):
-        should_keyword = []
-        keyword_index_doc = []
-        keyword_index_sign_doc = []
-        if save_data:
-            for i in save_data:
-                _id = i['keyword']
-                should_keyword.append(_id)
-            is_in, is_in_data, shoulds_not = self.es_in_or_notins('dso_douyin_keyword_alias', should_keyword)
-            for i in save_data:
-                _id = i['keyword']
-                i['index_avg'] = mode_data.list_avg(i['day_index'])
-                keyword_index_doc.append({"index": {"_id": f"{_id}"}})
-                keyword_index_doc.append(i)
-
-                # 同步到关键词表
-                if _id in is_in_data:
-                    _index = is_in_data[_id]['_index']
-                    keyword_index_sign_doc.append({'update': {'_index': _index, '_id': _id}})
-                    keyword_index_sign_doc.append({'doc': {'index_avg': i['index_avg']}})
-        self.es_create_update(doc=keyword_index_doc, index='douyin_keyword_index')
-        self.es_create_update_noIndex(doc=keyword_index_sign_doc)
-
     # ip 信息
     def get_user_ip(self, ip):
         url = f'http://whois.pconline.com.cn/ipJson.jsp?ip={ip}&json=true'
         Default_return = {
             'ip': ip,
             'country': '',
             'province': '',
@@ -4488,8 +4570,7 @@
 mode_xhs = XhsJike()  # douyin配置
 mode_pros = ModeStatic()  # 其它函数
 mode_cos = Cos()  # cos
 mode_fr_cos = Cos(server_select='personal')  # cos 高阳
 mode_myself = MyGy()
 
 mode_pro = ModeFunc()  # main
-
```

