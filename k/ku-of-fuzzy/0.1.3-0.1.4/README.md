# Comparing `tmp/ku_of_fuzzy-0.1.3-py3-none-any.whl.zip` & `tmp/ku_of_fuzzy-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 13698 bytes, number of entries: 7
+Zip file size: 13992 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat        2 b- defN 24-May-13 01:06 ku_of_fuzzy/__init__.py
--rw-rw-rw-  2.0 fat    34100 b- defN 24-May-14 09:18 ku_of_fuzzy/fuzzy_calculate.py
--rw-rw-rw-  2.0 fat     1089 b- defN 24-May-14 09:28 ku_of_fuzzy-0.1.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    15580 b- defN 24-May-14 09:28 ku_of_fuzzy-0.1.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-14 09:28 ku_of_fuzzy-0.1.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 24-May-14 09:28 ku_of_fuzzy-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      572 b- defN 24-May-14 09:28 ku_of_fuzzy-0.1.3.dist-info/RECORD
-7 files, 51447 bytes uncompressed, 12680 bytes compressed:  75.4%
+-rw-rw-rw-  2.0 fat    35917 b- defN 24-May-15 09:06 ku_of_fuzzy/fuzzy_calculate.py
+-rw-rw-rw-  2.0 fat     1089 b- defN 24-May-15 09:20 ku_of_fuzzy-0.1.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    16686 b- defN 24-May-15 09:20 ku_of_fuzzy-0.1.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-15 09:20 ku_of_fuzzy-0.1.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 24-May-15 09:20 ku_of_fuzzy-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      572 b- defN 24-May-15 09:20 ku_of_fuzzy-0.1.4.dist-info/RECORD
+7 files, 54370 bytes uncompressed, 12974 bytes compressed:  76.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: ku_of_fuzzy/__init__.py
 Comment: 
 
 Filename: ku_of_fuzzy/fuzzy_calculate.py
 Comment: 
 
-Filename: ku_of_fuzzy-0.1.3.dist-info/LICENSE
+Filename: ku_of_fuzzy-0.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: ku_of_fuzzy-0.1.3.dist-info/METADATA
+Filename: ku_of_fuzzy-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: ku_of_fuzzy-0.1.3.dist-info/WHEEL
+Filename: ku_of_fuzzy-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: ku_of_fuzzy-0.1.3.dist-info/top_level.txt
+Filename: ku_of_fuzzy-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: ku_of_fuzzy-0.1.3.dist-info/RECORD
+Filename: ku_of_fuzzy-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ku_of_fuzzy/fuzzy_calculate.py

```diff
@@ -72,20 +72,21 @@
     df = df / max_values
     return df
 
 
 # 第二部分：建立相似度矩阵
 
 # 余弦相似度法
-def cosine_similarity(dataframe1):
+def cosine_similarity(dataframe1, decimals=3):
     """
     计算dataframe1中每一行与其他行之间的余弦相似度，并返回一个m*m的DataFrame。
 
     Args:
         dataframe1 (pd.DataFrame): 输入的m*n的DataFrame，元素值在[0, 1]之间。
+        decimals (int): 四舍五入到小数点后的位数，默认为3。
 
     Returns:
         pd.DataFrame: 一个m*m的DataFrame，其中Xij表示dataframe1的第i行和第j行之间的余弦相似度。
     """
     # 将DataFrame转换为NumPy数组
     array1 = dataframe1.values
 
@@ -98,145 +99,163 @@
 
     # 计算余弦相似度
     for i in range(m):
         for j in range(m):
             dot_product = np.dot(array1[i], array1[j])
             cosine_matrix[i][j] = dot_product / (norms[i] * norms[j])
 
+    # 四舍五入余弦相似度矩阵中的值
+    cosine_matrix_rounded = np.round(cosine_matrix, decimals=decimals)
+
     # 创建一个m*m的DataFrame来存储结果
-    dataframe2 = pd.DataFrame(cosine_matrix, index=dataframe1.index, columns=dataframe1.index)
+    dataframe2 = pd.DataFrame(cosine_matrix_rounded, index=dataframe1.index, columns=dataframe1.index)
 
     return dataframe2
 
 
-def pearson_similarity(dataframe1):
+# 皮尔逊相关系数法
+def pearson_similarity(dataframe1, decimals=3):
     """
     计算dataframe1中每一行与其他行之间的皮尔逊相关系数，并返回一个m*m的DataFrame。
 
     Args:
         dataframe1 (pd.DataFrame): 输入的m*n的DataFrame。
+        decimals (int): 四舍五入到小数点后的位数，默认为3。
 
     Returns:
         pd.DataFrame: 一个m*m的DataFrame，其中Xij表示dataframe1的第i行和第j行之间的皮尔逊相关系数。
     """
     # 计算每一行的平均值
     row_means = dataframe1.mean(axis=1)
 
     # 初始化相关系数矩阵
     m = len(dataframe1)
     pearson_matrix = np.zeros((m, m))
 
     # 计算皮尔逊相关系数
     for i in range(m):
         for j in range(m):
-            # 计算分子
             numerator = np.sum(abs((dataframe1.iloc[i] - row_means[i]) * (dataframe1.iloc[j] - row_means[j])))
-            # 计算分母
             denominator = np.sqrt(
                 np.sum((dataframe1.iloc[i] - row_means[i]) ** 2) * np.sum((dataframe1.iloc[j] - row_means[j]) ** 2))
-            # 计算相关系数
             if denominator != 0:
                 pearson_matrix[i][j] = numerator / denominator
             else:
-                raise ValueError("计算系数分母为0")
+                pearson_matrix[i][j] = np.nan  # 如果分母为0，则赋值为NaN
+
+    # 四舍五入相关系数矩阵中的值
+    pearson_matrix_rounded = np.round(pearson_matrix, decimals=decimals)
+
     # 创建一个m*m的DataFrame来存储结果
-    dataframe2 = pd.DataFrame(pearson_matrix, index=dataframe1.index, columns=dataframe1.index)
+    dataframe2 = pd.DataFrame(pearson_matrix_rounded, index=dataframe1.index, columns=dataframe1.index)
 
     return dataframe2
 
 
 # 距离法求相似度r_ij
 # r_ij=1-c*d_ij
 # 欧式距离
-
-def euclidean_distance(dataframe1):
+def euclidean_distance(dataframe1, decimals=3):
     """
     计算dataframe1中每一行与其他行之间的欧氏距离，并返回一个m*m的DataFrame。
 
     Args:
         dataframe1 (pd.DataFrame): 输入的m*n的DataFrame。
+        decimals (int): 四舍五入到小数点后的位数，默认为3。
 
     Returns:
         pd.DataFrame: 一个m*m的DataFrame，其中Xij表示dataframe1的第i行和第j行之间的欧氏距离。
     """
     # 初始化距离矩阵
     m = len(dataframe1)
     euclidean_matrix = np.zeros((m, m))
 
     # 计算欧氏距离
     for i in range(m):
         for j in range(m):
             euclidean_matrix[i][j] = np.linalg.norm(dataframe1.iloc[i] - dataframe1.iloc[j])
 
+    # 四舍五入距离矩阵中的值
+    euclidean_matrix_rounded = np.round(euclidean_matrix, decimals=decimals)
+
     # 创建一个m*m的DataFrame来存储结果
-    dataframe2 = pd.DataFrame(euclidean_matrix, index=dataframe1.index, columns=dataframe1.index)
+    dataframe2 = pd.DataFrame(euclidean_matrix_rounded, index=dataframe1.index, columns=dataframe1.index)
 
     return dataframe2
 
 
 # Hamming距离
-def hamming_distance(dataframe1):
+def hamming_distance(dataframe1, decimals=3):
     """
     计算dataframe1中每一行与其他行之间的自定义距离，并返回一个m*m的DataFrame。
 
     参数:
         dataframe1 (pd.DataFrame): 输入的m*n的DataFrame。
+        decimals (int): 四舍五入到小数点后的位数，默认为3。
 
     返回:
         pd.DataFrame: 一个m*m的DataFrame，其中Xij表示dataframe1的第i行和第j行之间的自定义距离。
     """
     # 初始化距离矩阵
     m = len(dataframe1)
     hamming_matrix = np.zeros((m, m))
 
     # 计算自定义距离
     for i in range(m):
         for j in range(m):
             hamming_matrix[i][j] = np.sum(np.abs(dataframe1.iloc[i] - dataframe1.iloc[j]))
 
+    # 四舍五入距离矩阵中的值
+    hamming_matrix_rounded = np.round(hamming_matrix, decimals=decimals)
+
     # 创建一个m*m的DataFrame来存储结果
-    dataframe2 = pd.DataFrame(hamming_matrix, index=dataframe1.index, columns=dataframe1.index)
+    dataframe2 = pd.DataFrame(hamming_matrix_rounded, index=dataframe1.index, columns=dataframe1.index)
 
     return dataframe2
 
 
 # Chebyshev距离
-def Chebyshev_distance(dataframe1):
+def Chebyshev_distance(dataframe1, decimals=3):
     """
     计算dataframe1中每一行与其他行之间的最大距离，并返回一个m*m的DataFrame。
 
     参数:
         dataframe1 (pd.DataFrame): 输入的m*n的DataFrame。
+        decimals (int): 四舍五入到小数点后的位数，默认为3。
 
     返回:
         pd.DataFrame: 一个m*m的DataFrame，其中Xij表示dataframe1的第i行和第j行之间的最大距离。
     """
     # 初始化距离矩阵
     m = len(dataframe1)
     Chebyshev_matrix = np.zeros((m, m))
 
     # 计算最大距离
     for i in range(m):
         for j in range(m):
             Chebyshev_matrix[i][j] = np.max(np.abs(dataframe1.iloc[i] - dataframe1.iloc[j]))
 
+    # 四舍五入距离矩阵中的值
+    Chebyshev_matrix_rounded = np.round(Chebyshev_matrix, decimals=decimals)
+
     # 创建一个m*m的DataFrame来存储结果
-    dataframe2 = pd.DataFrame(Chebyshev_matrix, index=dataframe1.index, columns=dataframe1.index)
+    dataframe2 = pd.DataFrame(Chebyshev_matrix_rounded, index=dataframe1.index, columns=dataframe1.index)
 
     return dataframe2
 
 
 # 贴近度法求相似矩阵
 # 最大最小法
-def maximum_minimum(dataframe1):
+def maximum_minimum(dataframe1, decimals=3):
     """
     计算dataframe1中每一行与其他行之间的比率距离，并返回一个m*m的DataFrame。
 
     参数:
         dataframe1 (pd.DataFrame): 输入的m*n的DataFrame。
+        decimals (int): 四舍五入到小数点后的位数，默认为3。
 
     返回:
         pd.DataFrame: 一个m*m的DataFrame，其中rij表示dataframe1的第i行和第j行之间的比率距离。
     """
     # 初始化距离矩阵
     m = len(dataframe1)
     maxmin_matrix = np.zeros((m, m))
@@ -244,27 +263,31 @@
     # 计算比率距离
     for i in range(m):
         for j in range(m):
             numerator = np.sum(np.minimum(dataframe1.iloc[i], dataframe1.iloc[j]))
             denominator = np.sum(np.maximum(dataframe1.iloc[i], dataframe1.iloc[j]))
             maxmin_matrix[i][j] = numerator / denominator if denominator != 0 else 0
 
+    # 四舍五入距离矩阵中的值
+    maxmin_matrix_rounded = np.round(maxmin_matrix, decimals=decimals)
+
     # 创建一个m*m的DataFrame来存储结果
-    dataframe2 = pd.DataFrame(maxmin_matrix, index=dataframe1.index, columns=dataframe1.index)
+    dataframe2 = pd.DataFrame(maxmin_matrix_rounded, index=dataframe1.index, columns=dataframe1.index)
 
     return dataframe2
 
 
 # 算术平均最小法
-def arithmetic_mean_minimum(dataframe1):
+def arithmetic_mean_minimum(dataframe1, decimals=3):
     """
     计算dataframe1中每一行与其他行之间的修改后的比率距离，并返回一个m*m的DataFrame。
 
     参数:
         dataframe1 (pd.DataFrame): 输入的m*n的DataFrame。
+        decimals (int): 四舍五入到小数点后的位数，默认为3。
 
     返回:
         pd.DataFrame: 一个m*m的DataFrame，其中rij表示dataframe1的第i行和第j行之间的修改后的比率距离。
     """
     # 初始化距离矩阵
     m = len(dataframe1)
     arithmetic_mean_minimum_matrix = np.zeros((m, m))
@@ -272,27 +295,31 @@
     # 计算修改后的比率距离
     for i in range(m):
         for j in range(m):
             numerator = np.sum(np.minimum(dataframe1.iloc[i], dataframe1.iloc[j]))
             denominator = 0.5 * np.sum(dataframe1.iloc[i] + dataframe1.iloc[j])
             arithmetic_mean_minimum_matrix[i][j] = numerator / denominator if denominator != 0 else 0
 
+    # 四舍五入距离矩阵中的值
+    arithmetic_mean_minimum_matrix_rounded = np.round(arithmetic_mean_minimum_matrix, decimals=decimals)
+
     # 创建一个m*m的DataFrame来存储结果
-    dataframe2 = pd.DataFrame(arithmetic_mean_minimum_matrix, index=dataframe1.index, columns=dataframe1.index)
+    dataframe2 = pd.DataFrame(arithmetic_mean_minimum_matrix_rounded, index=dataframe1.index, columns=dataframe1.index)
 
     return dataframe2
 
 
 # 几何平均最小法
-def geometric_mean_minimum(dataframe1):
+def geometric_mean_minimum(dataframe1, decimals=3):
     """
     计算dataframe1中每一行与其他行之间的几何平均距离，并返回一个m*m的DataFrame。
 
     参数:
         dataframe1 (pd.DataFrame): 输入的m*n的DataFrame。
+        decimals (int): 四舍五入到小数点后的位数，默认为3。
 
     返回:
         pd.DataFrame: 一个m*m的DataFrame，其中rij表示dataframe1的第i行和第j行之间的几何平均距离。
     """
     # 初始化距离矩阵
     m = len(dataframe1)
     geometric_mean_matrix = np.zeros((m, m))
@@ -300,16 +327,19 @@
     # 计算几何平均距离
     for i in range(m):
         for j in range(m):
             numerator = np.sum(np.minimum(dataframe1.iloc[i], dataframe1.iloc[j]))
             denominator = np.sum(np.sqrt(dataframe1.iloc[i] * dataframe1.iloc[j]))
             geometric_mean_matrix[i][j] = numerator / denominator if denominator != 0 else 0
 
+    # 四舍五入距离矩阵中的值
+    geometric_mean_matrix_rounded = np.round(geometric_mean_matrix, decimals=decimals)
+
     # 创建一个m*m的DataFrame来存储结果
-    dataframe2 = pd.DataFrame(geometric_mean_matrix, index=dataframe1.index, columns=dataframe1.index)
+    dataframe2 = pd.DataFrame(geometric_mean_matrix_rounded, index=dataframe1.index, columns=dataframe1.index)
 
     return dataframe2
 
 
 # 第三部分：模糊矩阵的聚类
 
 # 矩阵的合成
@@ -661,43 +691,48 @@
     threshold_df = threshold_matrix(df1, lambda_level)
 
     # 计算唯一行的数量，表示不同的类别
     unique_rows = len(threshold_df.drop_duplicates(keep='first'))
 
     # 查找类别的数量以及每个类别中的对象数量
     r = unique_rows  # 类别的数量
+    n = df0.shape[0]  # 总对象数
     n_i = threshold_df.sum(axis=0)  # 每个类别中的对象数量
 
+    # 如果类别数为1或总对象数等于类别数，则F值为0
+    if r == 1 or n == r:
+        return 0
+
     # 计算全局中心
     global_center = df0.mean(axis=0)  # 所有对象的均值
 
     # 初始化分子和分母
     numerator = 0
     denominator = 0
 
     # 计算模糊统计量的分子和分母
     for i in range(r):
         # 获取属于类别 i 的对象
         class_objects = df0.iloc[threshold_df.iloc[:, i].astype(bool).values]
         # 计算类别 i 的中心
         class_center = class_objects.mean(axis=0)
         # 在分子中累积
-        numerator += n_i[i] * np.linalg.norm(class_center - global_center) ** 2
+        numerator += n_i.iloc[i] * np.linalg.norm(class_center - global_center) ** 2
 
         # 对类别 i 中的每个对象进行累积
-        for j in range(n_i[i]):
+        for j in class_objects.index:
             # 在分母中累积
-            denominator += np.linalg.norm(class_objects.iloc[j] - class_center) ** 2
+            denominator += np.linalg.norm(class_objects.loc[j] - class_center) ** 2
 
     # 调整自由度
-    numerator /= (r - 1)  # 将分子除以（类别数 - 1）
-    denominator /= (df0.shape[0] - r)  # 将分母除以（总对象数 - 类别数）
+    numerator /= (r - 1) if r > 1 else 1  # 避免除以0
+    denominator /= (n - r) if n > r else 1  # 避免除以0
 
     # 计算模糊统计量 F
-    F = numerator / denominator if denominator != 0 else 0  # 如果分母不为0，则计算 F
+    F = numerator / denominator
 
     return F
 
 
 # 最优的分类λ值
 def best_F(df0, df1):
     """
```

## Comparing `ku_of_fuzzy-0.1.3.dist-info/LICENSE` & `ku_of_fuzzy-0.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ku_of_fuzzy-0.1.3.dist-info/METADATA` & `ku_of_fuzzy-0.1.4.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ku_of_fuzzy
-Version: 0.1.3
+Version: 0.1.4
 Summary: 用于模糊数学计算的Python库
 Home-page: https://github.com/YueorLekai/ku_of_fuzzy
 Author: Yuekai
 Author-email: 1977269004@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -97,69 +97,78 @@
 - **参数**:
   - `df` (DataFrame): 需要规格化的pandas DataFrame。
 - **返回**: 规格化后的DataFrame。
 ## 第二部分：建立相似度矩阵
 `ku_of_fuzzy`库提供了多种方法来建立相似度矩阵。以下是可用的建立相似度矩阵的函数：
 
 ### 余弦相似度法
-- **函数**: `cosine_similarity(dataframe1)`
-- **描述**: 计算DataFrame中每一行与其他行之间的余弦相似度。
+- **函数**: `cosine_similarity(dataframe1, decimals=3)`
+- **描述**: 计算DataFrame中每一行与其他行之间的余弦相似度，并四舍五入到指定的小数位数。
 - **参数**:
   - `dataframe1` (pd.DataFrame): 输入的m*n的DataFrame，元素值在[0, 1]之间。
+  - `decimals` (int, 可选): 四舍五入到小数点后的位数，默认为3。
 - **返回**: 一个m*m的DataFrame，其中Xij表示第i行和第j行之间的余弦相似度。
 
 ### 皮尔逊相关系数法
-- **函数**: `pearson_similarity(dataframe1)`
-- **描述**: 计算DataFrame中每一行与其他行之间的皮尔逊相关系数。
+- **函数**: `pearson_similarity(dataframe1, decimals=3)`
+- **描述**: 计算DataFrame中每一行与其他行之间的皮尔逊相关系数，并四舍五入到指定的小数位数。
 - **参数**:
   - `dataframe1` (pd.DataFrame): 输入的m*n的DataFrame。
+  - `decimals` (int, 可选): 四舍五入到小数点后的位数，默认为3。
 - **返回**: 一个m*m的DataFrame，其中Xij表示第i行和第j行之间的皮尔逊相关系数。
 
 ### 欧氏距离法
-- **函数**: `euclidean_distance(dataframe1)`
-- **描述**: 计算DataFrame中每一行与其他行之间的欧氏距离。
+- **函数**: `euclidean_distance(dataframe1, decimals=3)`
+- **描述**: 计算DataFrame中每一行与其他行之间的欧氏距离，并四舍五入到指定的小数位数。
 - **参数**:
   - `dataframe1` (pd.DataFrame): 输入的m*n的DataFrame。
+  - `decimals` (int, 可选): 四舍五入到小数点后的位数，默认为3。
 - **返回**: 一个m*m的DataFrame，其中Xij表示第i行和第j行之间的欧氏距离。
 
 ### Hamming距离法
-- **函数**: `hamming_distance(dataframe1)`
-- **描述**: 计算DataFrame中每一行与其他行之间的Hamming距离。
+- **函数**: `hamming_distance(dataframe1, decimals=3)`
+- **描述**: 计算DataFrame中每一行与其他行之间的Hamming距离，并四舍五入到指定的小数位数。
 - **参数**:
   - `dataframe1` (pd.DataFrame): 输入的m*n的DataFrame。
+  - `decimals` (int, 可选): 四舍五入到小数点后的位数，默认为3。
 - **返回**: 一个m*m的DataFrame，其中Xij表示第i行和第j行之间的Hamming距离。
 
 ### Chebyshev距离法
-- **函数**: `Chebyshev_distance(dataframe1)`
-- **描述**: 计算DataFrame中每一行与其他行之间的Chebyshev距离。
+- **函数**: `Chebyshev_distance(dataframe1, decimals=3)`
+- **描述**: 计算DataFrame中每一行与其他行之间的Chebyshev距离，并四舍五入到指定的小数位数。
 - **参数**:
   - `dataframe1` (pd.DataFrame): 输入的m*n的DataFrame。
+  - `decimals` (int, 可选): 四舍五入到小数点后的位数，默认为3。
 - **返回**: 一个m*m的DataFrame，其中Xij表示第i行和第j行之间的Chebyshev距离。
 
 ### 最大最小法
-- **函数**: `maximum_minimum(dataframe1)`
-- **描述**: 计算DataFrame中每一行与其他行之间的最大最小比率距离。
+- **函数**: `maximum_minimum(dataframe1, decimals=3)`
+- **描述**: 计算DataFrame中每一行与其他行之间的最大最小比率距离，并四舍五入到指定的小数位数。
 - **参数**:
   - `dataframe1` (pd.DataFrame): 输入的m*n的DataFrame。
+  - `decimals` (int, 可选): 四舍五入到小数点后的位数，默认为3。
 - **返回**: 一个m*m的DataFrame，其中rij表示第i行和第j行之间的最大最小比率距离。
 
 ### 算术平均最小法
-- **函数**: `arithmetic_mean_minimum(dataframe1)`
-- **描述**: 计算DataFrame中每一行与其他行之间的算术平均最小比率距离。
+- **函数**: `arithmetic_mean_minimum(dataframe1, decimals=3)`
+- **描述**: 计算DataFrame中每一行与其他行之间的算术平均最小比率距离，并四舍五入到指定的小数位数。
 - **参数**:
   - `dataframe1` (pd.DataFrame): 输入的m*n的DataFrame。
+  - `decimals` (int, 可选): 四舍五入到小数点后的位数，默认为3。
 - **返回**: 一个m*m的DataFrame，其中rij表示第i行和第j行之间的算术平均最小比率距离。
 
 ### 几何平均最小法
-- **函数**: `geometric_mean_minimum(dataframe1)`
-- **描述**: 计算DataFrame中每一行与其他行之间的几何平均最小比率距离。
+- **函数**: `geometric_mean_minimum(dataframe1, decimals=3)`
+- **描述**: 计算DataFrame中每一行与其他行之间的几何平均最小比率距离，并四舍五入到指定的小数位数。
 - **参数**:
   - `dataframe1` (pd.DataFrame): 输入的m*n的DataFrame。
+  - `decimals` (int, 可选): 四舍五入到小数点后的位数，默认为3。
 - **返回**: 一个m*m的DataFrame，其中rij表示第i行和第j行之间的几何平均最小比率距离。
 
+
 ## 第三部分：模糊矩阵的聚类
 `ku_of_fuzzy`库提供了一系列函数来处理模糊矩阵的聚类问题。以下是可用的聚类相关函数：
 
 ### 矩阵的合成
 - **函数**: `fuzzy_matrix_composition(df1, df2)`
 - **描述**: 计算两个DataFrame的模糊矩阵合成。
 - **参数**:
```

