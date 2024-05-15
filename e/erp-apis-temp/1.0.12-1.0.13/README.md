# Comparing `tmp/erp_apis_temp-1.0.12-py3-none-any.whl.zip` & `tmp/erp_apis_temp-1.0.13-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 18855 bytes, number of entries: 16
--rw-rw-rw-  2.0 fat     2345 b- defN 24-May-13 01:43 erp_apis/config.py
+Zip file size: 18891 bytes, number of entries: 16
+-rw-rw-rw-  2.0 fat     2347 b- defN 24-May-15 02:53 erp_apis/config.py
 -rw-rw-rw-  2.0 fat     3636 b- defN 24-May-13 01:43 erp_apis/erpRequest.py
 -rw-rw-rw-  2.0 fat    12874 b- defN 24-May-10 07:54 erp_apis/apis/1.py
 -rw-rw-rw-  2.0 fat     4737 b- defN 24-May-12 12:09 erp_apis/apis/afterSales.py
--rw-rw-rw-  2.0 fat     4380 b- defN 24-May-13 06:59 erp_apis/apis/aftersale_test.py
+-rw-rw-rw-  2.0 fat     4471 b- defN 24-May-13 09:46 erp_apis/apis/aftersale_test.py
 -rw-rw-rw-  2.0 fat     1538 b- defN 24-May-09 01:56 erp_apis/apis/goods.py
 -rw-rw-rw-  2.0 fat     1013 b- defN 24-May-09 01:56 erp_apis/apis/inventory.py
 -rw-rw-rw-  2.0 fat     4371 b- defN 24-May-13 01:43 erp_apis/apis/order.py
 -rw-rw-rw-  2.0 fat     3093 b- defN 24-May-12 12:12 erp_apis/apis/refund.py
 -rw-rw-rw-  2.0 fat     2499 b- defN 24-May-13 01:44 erp_apis/apis/test.py
 -rw-rw-rw-  2.0 fat     1139 b- defN 24-May-09 01:56 erp_apis/apis/user.py
 -rw-rw-rw-  2.0 fat     2163 b- defN 24-May-13 07:20 erp_apis/utils/util.py
--rw-rw-rw-  2.0 fat     1530 b- defN 24-May-13 08:12 erp_apis_temp-1.0.12.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-13 08:12 erp_apis_temp-1.0.12.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       38 b- defN 24-May-13 08:12 erp_apis_temp-1.0.12.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1284 b- defN 24-May-13 08:12 erp_apis_temp-1.0.12.dist-info/RECORD
-16 files, 46732 bytes uncompressed, 16759 bytes compressed:  64.1%
+-rw-rw-rw-  2.0 fat     1530 b- defN 24-May-15 02:53 erp_apis_temp-1.0.13.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-15 02:53 erp_apis_temp-1.0.13.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       38 b- defN 24-May-15 02:53 erp_apis_temp-1.0.13.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1284 b- defN 24-May-15 02:53 erp_apis_temp-1.0.13.dist-info/RECORD
+16 files, 46825 bytes uncompressed, 16795 bytes compressed:  64.1%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: erp_apis/apis/user.py
 Comment: 
 
 Filename: erp_apis/utils/util.py
 Comment: 
 
-Filename: erp_apis_temp-1.0.12.dist-info/METADATA
+Filename: erp_apis_temp-1.0.13.dist-info/METADATA
 Comment: 
 
-Filename: erp_apis_temp-1.0.12.dist-info/WHEEL
+Filename: erp_apis_temp-1.0.13.dist-info/WHEEL
 Comment: 
 
-Filename: erp_apis_temp-1.0.12.dist-info/top_level.txt
+Filename: erp_apis_temp-1.0.13.dist-info/top_level.txt
 Comment: 
 
-Filename: erp_apis_temp-1.0.12.dist-info/RECORD
+Filename: erp_apis_temp-1.0.13.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## erp_apis/config.py

```diff
@@ -8,15 +8,15 @@
 Erp321BaseUrl = 'https://www.erp321.com'
 ErpApiBaseUrl = 'https://api.erp321.com'
 
 
 
 DEFAULT_HEADERS = {
     'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/237.84.2.178 Safari/537.36 Edg/109.0.1518.78',
-    'cookie': 'acw_tc=2760779b17154951601776467e2eaae3707f13160901b36135bd350c5c0636; _ati=2632320813015; j_d_3=3ZEUHZ3LD6TF2GRXTWSSJ6LVEZIAKQE7XTZO5II3AI23TRQYIQ2RLBFPPHLVXCO7YVXQXAL36AGJ2C5RQMV7RAGT74; u_ssi=; u_drp=; u_r=12%2c13%2c14%2c15%2c17%2c18%2c22%2c23%2c27%2c28%2c29%2c30%2c31%2c32%2c33%2c34%2c35%2c36%2c39%2c40%2c41%2c52%2c53%2c54%2c61%2c62%2c101%2c1001%2c109; u_shop=-1; u_lastLoginType=ap; tfstk=fP2koMDya7lSpJ-dr-D53zgD_v1xFUMI1ypKJv3FgquXyUp8YpcUADiE4k77-J0qUXN-J43nKkaGDNBOBuZSdx7OWOIUOX6jd2WKLiurgfDFWNBxX-cS2vPd8MOQmoujxUuETyWqgqir4vurTERqbquELvze0Iotb2orT4-qMARrWJPa3GEdPKE0TP2mqb5Y4qJEc-moZVrzEpJUb0co7uucWF37yjrItJtBKfEz1yiazU7tNkP0o0DhHQkamWzic8W9rmN80ygqgHJQmX0ug8lDYpr4m4cgtzbkN4P8ofiqgHXsDP34V8PcAErzW4Dr0jBNjolUM8G_eZJoQ5Z-eWzC6IMuY7kc4fO2_so6dmSLnBOIamim5gRoxaMJO6PPmiATAbojfVIcmBMjamimUijD1DlrccyC.; 3AB9D23F7A4B3C9B=3ZEUHZ3LD6TF2GRXTWSSJ6LVEZIAKQE7XTZO5II3AI23TRQYIQ2RLBFPPHLVXCO7YVXQXAL36AGJ2C5RQMV7RAGT74; u_name=%e6%9d%8e%e7%a6%8f%e6%88%90; u_lid=18986680202; u_json=%7b%22t%22%3a%222024-5-12+14%3a49%3a03%22%2c%22co_type%22%3a%22%e6%a0%87%e5%87%86%e5%95%86%e5%ae%b6%22%2c%22proxy%22%3anull%2c%22ug_id%22%3a%2211003725%22%2c%22dbc%22%3a%221149%22%2c%22tt%22%3a%2295%22%2c%22apps%22%3a%221.4.7.150.152.168.169%22%2c%22pwd_valid%22%3a%220%22%2c%22ssi%22%3anull%2c%22sign%22%3a%224001967.1EA70FE2D4EB480D859D91A98D86E11F%2cd566f976b2c825e4ca410ee0754bcf2b%22%7d; u_co_name=%e6%ad%a6%e6%b1%89%e5%b0%8f%e5%b8%83%e7%94%b5%e5%ad%90%e5%95%86%e5%8a%a1%e6%9c%89%e9%99%90%e5%85%ac%e5%8f%b8; v_d_144=1715496538498_f488932826196e289944b013be36a727; u_cid=133599701439643594; u_sso_token=CS@e1903f92c5c7459fbbe381ba85d75c00; u_id=15424700; u_co_id=10174711; p_50=5DA09A8DA5EF6EC4DE5BE6D6A0231599638511221439646836%7c10174711; u_env=www'
+    # 'cookie': 'acw_tc=2760779b17154951601776467e2eaae3707f13160901b36135bd350c5c0636; _ati=2632320813015; j_d_3=3ZEUHZ3LD6TF2GRXTWSSJ6LVEZIAKQE7XTZO5II3AI23TRQYIQ2RLBFPPHLVXCO7YVXQXAL36AGJ2C5RQMV7RAGT74; u_ssi=; u_drp=; u_r=12%2c13%2c14%2c15%2c17%2c18%2c22%2c23%2c27%2c28%2c29%2c30%2c31%2c32%2c33%2c34%2c35%2c36%2c39%2c40%2c41%2c52%2c53%2c54%2c61%2c62%2c101%2c1001%2c109; u_shop=-1; u_lastLoginType=ap; tfstk=fP2koMDya7lSpJ-dr-D53zgD_v1xFUMI1ypKJv3FgquXyUp8YpcUADiE4k77-J0qUXN-J43nKkaGDNBOBuZSdx7OWOIUOX6jd2WKLiurgfDFWNBxX-cS2vPd8MOQmoujxUuETyWqgqir4vurTERqbquELvze0Iotb2orT4-qMARrWJPa3GEdPKE0TP2mqb5Y4qJEc-moZVrzEpJUb0co7uucWF37yjrItJtBKfEz1yiazU7tNkP0o0DhHQkamWzic8W9rmN80ygqgHJQmX0ug8lDYpr4m4cgtzbkN4P8ofiqgHXsDP34V8PcAErzW4Dr0jBNjolUM8G_eZJoQ5Z-eWzC6IMuY7kc4fO2_so6dmSLnBOIamim5gRoxaMJO6PPmiATAbojfVIcmBMjamimUijD1DlrccyC.; 3AB9D23F7A4B3C9B=3ZEUHZ3LD6TF2GRXTWSSJ6LVEZIAKQE7XTZO5II3AI23TRQYIQ2RLBFPPHLVXCO7YVXQXAL36AGJ2C5RQMV7RAGT74; u_name=%e6%9d%8e%e7%a6%8f%e6%88%90; u_lid=18986680202; u_json=%7b%22t%22%3a%222024-5-12+14%3a49%3a03%22%2c%22co_type%22%3a%22%e6%a0%87%e5%87%86%e5%95%86%e5%ae%b6%22%2c%22proxy%22%3anull%2c%22ug_id%22%3a%2211003725%22%2c%22dbc%22%3a%221149%22%2c%22tt%22%3a%2295%22%2c%22apps%22%3a%221.4.7.150.152.168.169%22%2c%22pwd_valid%22%3a%220%22%2c%22ssi%22%3anull%2c%22sign%22%3a%224001967.1EA70FE2D4EB480D859D91A98D86E11F%2cd566f976b2c825e4ca410ee0754bcf2b%22%7d; u_co_name=%e6%ad%a6%e6%b1%89%e5%b0%8f%e5%b8%83%e7%94%b5%e5%ad%90%e5%95%86%e5%8a%a1%e6%9c%89%e9%99%90%e5%85%ac%e5%8f%b8; v_d_144=1715496538498_f488932826196e289944b013be36a727; u_cid=133599701439643594; u_sso_token=CS@e1903f92c5c7459fbbe381ba85d75c00; u_id=15424700; u_co_id=10174711; p_50=5DA09A8DA5EF6EC4DE5BE6D6A0231599638511221439646836%7c10174711; u_env=www'
 }
 '''
   //生成唯一SessionCode
   if (!$.cookie('SessionCode')) {
     let guid = newJstTraceGuid();
     $.cookie('SessionCode', guid);
     params.SessionCode = guid;
```

## erp_apis/apis/aftersale_test.py

```diff
@@ -2,15 +2,15 @@
 # Project：erp_out_of_stock
 # File：test.py
 # Author：李福成
 # Date ：2024-04-28 18:24
 # IDE：PyCharm
 from json import dumps
 
-from afterSales import *
+from afterSales import aftersaleList, unconfirms, save, aftersaleCommon, confirmReturnQty, confirmGoods
 from apis.user import login
 from refund import refundListByafterId, unfinish, finish, confirm
 from erp_apis.erpRequest import Session
 
 def get_after_sale_order(code):
     resp = session.erp321Send(aftersaleList(
         queryData=[
@@ -111,15 +111,15 @@
 if __name__ == '__main__':
     session = Session()
     session.erpSend(login(
         username="17671271393",
         password="Wh1761393@"
     ))
 
-    code = 'asd'
+    code = '776389719299358'
 
     # 根据 退回快递单号 和 原快递单号 搜索售后单
     after_sale_order = get_after_sale_order(code)
 
     # if after_sale_order is None:
     #     # 创建无信息件，填写快递单号
     #     create_empty()
```

## Comparing `erp_apis_temp-1.0.12.dist-info/METADATA` & `erp_apis_temp-1.0.13.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erp_apis_temp
-Version: 1.0.12
+Version: 1.0.13
 Summary: erp_apis
 Author: 李福成
 Author-email: lfct@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://gitee.com/li_fucheng/erp_sdk_python/issues
 Project-URL: Documentation, https://gitee.com/li_fucheng/erp_sdk_python
 Project-URL: Source Code, https://gitee.com/li_fucheng/erp_sdk_python
```

## Comparing `erp_apis_temp-1.0.12.dist-info/RECORD` & `erp_apis_temp-1.0.13.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-erp_apis/config.py,sha256=WaD81d7mmUcon0SWjrFqjghfYrsa_49rTFmcvUePO1I,2345
+erp_apis/config.py,sha256=RVm2hs1j0J_Kb8sYbd-r29bzNRWSpR-gJcYnNc3RNPY,2347
 erp_apis/erpRequest.py,sha256=b_6Z9glqi0wkvSG4LKgRx-Z53CXgK2ihycN61D8g20A,3636
 erp_apis/apis/1.py,sha256=7gx9NDJBnZK5a0ki1weU4itAc3S7Ds8C6W4BbUYVQXg,12874
 erp_apis/apis/afterSales.py,sha256=8QvKlnKY3R1BJnAk6D09vjZ9sYA620wcDb8zMg4jD2o,4737
-erp_apis/apis/aftersale_test.py,sha256=1dLKOsJ-aZOkWOYQWZSDK-ozS4iB5HOKUFKRgH1Dizo,4380
+erp_apis/apis/aftersale_test.py,sha256=FjsYknNWL-It4otccyMtqNmcNqLgLIgXG3RqWxcgUdo,4471
 erp_apis/apis/goods.py,sha256=3HplLv-feqNMiV46ANuzhRfL9RDiOovF8RAAvNydmdI,1538
 erp_apis/apis/inventory.py,sha256=ktCBMrKRdHKSOKZIgCCWan0cTYNKm-ddpFNe1hkxgGk,1013
 erp_apis/apis/order.py,sha256=yCw8OhCJjvGjOMmI_gY9p4C_xROQWs062-iaJ9L7evw,4371
 erp_apis/apis/refund.py,sha256=oUvhwQ3JOj-0XS2DZDPEfZWtJGVFtXty0CcpRMd9_B4,3093
 erp_apis/apis/test.py,sha256=XrWoVqJFoZxm1MTZcQ8h5kn341VWjPNGfvxg12mUXkE,2499
 erp_apis/apis/user.py,sha256=vosgBp1QNesLIRMQyafe9y9PDFJyIjpPdmiE1jvVzOA,1139
 erp_apis/utils/util.py,sha256=Jb9GOlGrYJDLuE8EjsjUbKb_L-VzdqTZkIN4Mgm18Yc,2163
-erp_apis_temp-1.0.12.dist-info/METADATA,sha256=eX-oeHUSwYtwlq1S8hO9cWIjsZ1z1KkBIzAVr56l_o0,1530
-erp_apis_temp-1.0.12.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-erp_apis_temp-1.0.12.dist-info/top_level.txt,sha256=vqDQIzqoC9jLUmJwUdHu1qRTGhYD1SxQ5BsetWAnMrs,38
-erp_apis_temp-1.0.12.dist-info/RECORD,,
+erp_apis_temp-1.0.13.dist-info/METADATA,sha256=o3aAl65Ev-pEa4YzmgHatwpDB-pFzkR9j9mwwcFtZAI,1530
+erp_apis_temp-1.0.13.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+erp_apis_temp-1.0.13.dist-info/top_level.txt,sha256=vqDQIzqoC9jLUmJwUdHu1qRTGhYD1SxQ5BsetWAnMrs,38
+erp_apis_temp-1.0.13.dist-info/RECORD,,
```

