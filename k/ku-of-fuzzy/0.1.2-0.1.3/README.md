# Comparing `tmp/ku_of_fuzzy-0.1.2-py3-none-any.whl.zip` & `tmp/ku_of_fuzzy-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 12893 bytes, number of entries: 7
+Zip file size: 13698 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat        2 b- defN 24-May-13 01:06 ku_of_fuzzy/__init__.py
--rw-rw-rw-  2.0 fat    31944 b- defN 24-May-14 06:44 ku_of_fuzzy/fuzzy_calculate.py
--rw-rw-rw-  2.0 fat     1089 b- defN 24-May-14 06:58 ku_of_fuzzy-0.1.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    15028 b- defN 24-May-14 06:58 ku_of_fuzzy-0.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-14 06:58 ku_of_fuzzy-0.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 24-May-14 06:58 ku_of_fuzzy-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      572 b- defN 24-May-14 06:58 ku_of_fuzzy-0.1.2.dist-info/RECORD
-7 files, 48739 bytes uncompressed, 11875 bytes compressed:  75.6%
+-rw-rw-rw-  2.0 fat    34100 b- defN 24-May-14 09:18 ku_of_fuzzy/fuzzy_calculate.py
+-rw-rw-rw-  2.0 fat     1089 b- defN 24-May-14 09:28 ku_of_fuzzy-0.1.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    15580 b- defN 24-May-14 09:28 ku_of_fuzzy-0.1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-14 09:28 ku_of_fuzzy-0.1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 24-May-14 09:28 ku_of_fuzzy-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      572 b- defN 24-May-14 09:28 ku_of_fuzzy-0.1.3.dist-info/RECORD
+7 files, 51447 bytes uncompressed, 12680 bytes compressed:  75.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: ku_of_fuzzy/__init__.py
 Comment: 
 
 Filename: ku_of_fuzzy/fuzzy_calculate.py
 Comment: 
 
-Filename: ku_of_fuzzy-0.1.2.dist-info/LICENSE
+Filename: ku_of_fuzzy-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: ku_of_fuzzy-0.1.2.dist-info/METADATA
+Filename: ku_of_fuzzy-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: ku_of_fuzzy-0.1.2.dist-info/WHEEL
+Filename: ku_of_fuzzy-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: ku_of_fuzzy-0.1.2.dist-info/top_level.txt
+Filename: ku_of_fuzzy-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: ku_of_fuzzy-0.1.2.dist-info/RECORD
+Filename: ku_of_fuzzy-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ku_of_fuzzy/fuzzy_calculate.py

```diff
@@ -546,15 +546,15 @@
 augmented_dendrogram(Z)
 plt.show()'''
 
 
 # 根据模糊等价矩阵生成动态聚类图
 
 
-def draw(df,width=6.4,height=4.8):
+def draw(df, width=6.4, height=4.8):
     """
     绘制基于模糊链接矩阵的动态聚类树状图。
 
     参数:
     df (DataFrame): 用于聚类的数据框。
     width (float): 图形的宽度，默认为6.4英寸。
     height (float): 图形的高度，默认为4.8英寸。
@@ -583,14 +583,71 @@
 df = fuzzy_matrix_transitive_closure(df)
 print(df)
 draw(df)
 plt.show()
 '''
 
 
+# 聚类和阈值寻找函数
+def num_clusters(df, num):
+    """
+    寻找合适的阈值并进行聚类。
+    参数:
+        df (DataFrame): 需要聚类的pandas DataFrame。
+        num (int): 期望的聚类数量。
+    返回:
+        tuple: (找到的阈值, 聚类结果的列表)。
+    """
+    # 获取矩阵中的所有唯一值并降序排序
+    unique_values = np.sort(pd.unique(df.values.flatten()))[::-1]
+
+    # 遍历所有可能的阈值
+    for threshold in unique_values:
+        # 生成截矩阵
+        binary_matrix = threshold_matrix(df, threshold)
+        # 初始化聚类列表
+        cluster_list = []
+        # 遍历截矩阵的每一行
+        for i, row in binary_matrix.iterrows():
+            # 找到数值为1的元素对应的列名
+            connected_points = list(row[row == 1].index)
+            # 如果当前行的元素还没有被分配到任何聚类中
+            if not any(i in sublist for sublist in cluster_list):
+                # 创建新的聚类
+                new_cluster = [i] + connected_points
+                # 添加到聚类列表中
+                cluster_list.append(new_cluster)
+
+        # 清理聚类列表，合并重叠的聚类
+        cleaned_cluster_list = []
+        while len(cluster_list) > 0:
+            first, *rest = cluster_list
+            first = set(first)
+            lf = -1
+            while len(first) > lf:
+                lf = len(first)
+                rest2 = []
+                for r in rest:
+                    if len(first.intersection(set(r))) > 0:
+                        first |= set(r)
+                    else:
+                        rest2.append(r)
+                rest = rest2
+            cleaned_cluster_list.append(list(first))
+            cluster_list = rest
+
+        # 检查聚类数量是否符合要求
+        if len(cleaned_cluster_list) == num:
+            # 返回找到的阈值和聚类结果
+            return threshold, cleaned_cluster_list
+
+    # 如果没有找到符合条件的阈值和聚类
+    raise ValueError("没有找到符合条件的阈值和聚类")
+
+
 # 模糊统计量与最佳阈值的判读
 # 模糊统计量F的求解
 def fuzzy_statistic(df0, df1, lambda_level):
     """
     df0是原始元素-属性矩阵
     df1是归一化、相似后的矩阵
     lambda_level表示对应的截矩阵选择的界限
```

## Comparing `ku_of_fuzzy-0.1.2.dist-info/LICENSE` & `ku_of_fuzzy-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ku_of_fuzzy-0.1.2.dist-info/METADATA` & `ku_of_fuzzy-0.1.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ku_of_fuzzy
-Version: 0.1.2
+Version: 0.1.3
 Summary: 用于模糊数学计算的Python库
 Home-page: https://github.com/YueorLekai/ku_of_fuzzy
 Author: Yuekai
 Author-email: 1977269004@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -237,15 +237,24 @@
   - `width` (float): 图形的宽度，以英寸为单位，默认为6.4。
   - `height` (float): 图形的高度，以英寸为单位，默认为4.8。
 - **注意**: 在绘制完聚类图后，使用`plt.show()`来显示图像。
 
 ### 模糊统计量F的求解
 - **函数**: `fuzzy_statistic(df0, df1, lambda_level)`
 - **描述**: 输入原始元素-属性矩阵和归一化、相似后的矩阵，返回对应λ的F值。
+### 聚类阈值确定
 
+- **函数**: `num_clusters(df, num)`
+- **描述**: 根据给定的相似度矩阵和期望的聚类数量，找到一个阈值，使得在该阈值下，矩阵中相似度高于阈值的元素被划分为同一类，从而达到指定的聚类数量。
+- **参数**:
+  - `df` (DataFrame): 需要聚类的pandas DataFrame。
+  - `num` (int): 期望的聚类数量。
+- **返回**: 
+  - `threshold` (float): 确定的聚类阈值。
+  - `cluster_list` (list of lists): 每个子列表包含属于同一类的元素名。
 ### 最优分类λ值求解
 - **函数**: `best_F(df0, df1)`
 - **描述**: 输入原始元素-属性矩阵和归一化、相似后的矩阵，返回最优F时的λ值和最优的F值。
 ## 第四部分：模糊识别
 `ku_of_fuzzy`库提供了一系列函数来处理模糊集的识别问题。以下是可用的模糊识别相关函数：
 
 ### 模糊集内积
```

