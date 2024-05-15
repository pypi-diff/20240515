# Comparing `tmp/vbpy-1.0.tar.gz` & `tmp/vbpy-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbpy-1.0.tar", last modified: Tue May 14 10:57:45 2024, max compression
+gzip compressed data, was "vbpy-1.1.tar", last modified: Wed May 15 08:47:10 2024, max compression
```

## Comparing `vbpy-1.0.tar` & `vbpy-1.1.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 10:57:45.250000 vbpy-1.0/
--rw-rw-rw-   0        0        0      120 2024-05-14 10:57:46.000000 vbpy-1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-14 10:57:46.000000 vbpy-1.0/setup.cfg
--rw-rw-rw-   0        0        0      534 2024-05-14 10:22:54.000000 vbpy-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 10:57:45.280000 vbpy-1.0/vbpy/
--rw-rw-rw-   0        0        0       51 2024-05-14 10:54:58.000000 vbpy-1.0/vbpy/__init__.py
--rw-rw-rw-   0        0        0    31915 2024-05-14 10:33:48.000000 vbpy-1.0/vbpy/vbpy.py
-drwxrwxrwx   0        0        0        0 2024-05-14 10:57:45.320000 vbpy-1.0/vbpy.egg-info/
--rw-rw-rw-   0        0        0      120 2024-05-14 10:57:46.000000 vbpy-1.0/vbpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      150 2024-05-14 10:57:46.000000 vbpy-1.0/vbpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 10:57:46.000000 vbpy-1.0/vbpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-14 10:57:46.000000 vbpy-1.0/vbpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 08:47:10.350000 vbpy-1.1/
+-rw-rw-rw-   0        0        0      120 2024-05-15 08:47:12.000000 vbpy-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-15 08:47:12.000000 vbpy-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      534 2024-05-15 08:46:58.000000 vbpy-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 08:47:10.390000 vbpy-1.1/vbpy/
+-rw-rw-rw-   0        0        0      134 2024-05-15 08:43:06.000000 vbpy-1.1/vbpy/__init__.py
+-rw-rw-rw-   0        0        0     2553 2024-05-15 08:43:08.000000 vbpy-1.1/vbpy/combine_data.py
+-rw-rw-rw-   0        0        0    18131 2024-05-15 08:27:34.000000 vbpy-1.1/vbpy/load_claim_auto.py
+-rw-rw-rw-   0        0        0    13907 2024-05-15 08:19:46.000000 vbpy-1.1/vbpy/load_revenue_auto.py
+drwxrwxrwx   0        0        0        0 2024-05-15 08:47:10.430000 vbpy-1.1/vbpy.egg-info/
+-rw-rw-rw-   0        0        0      120 2024-05-15 08:47:12.000000 vbpy-1.1/vbpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2024-05-15 08:47:12.000000 vbpy-1.1/vbpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 08:47:12.000000 vbpy-1.1/vbpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-15 08:47:12.000000 vbpy-1.1/vbpy.egg-info/top_level.txt
```

### Comparing `vbpy-1.0/setup.py` & `vbpy-1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     
     name='vbpy',
-    version='1.0',
+    version='1.1',
     packages=find_packages(),
     # description='Your library description',
     # long_description=open('README.md').read(),
     # long_description_content_type='text/markdown',
     author='Nguyen Ha Tuan Long',
     author_email='tuanlongnguyenha@gmail.com',
     # url='https://github.com/yourusername/your_library_name',
```

### Comparing `vbpy-1.0/vbpy/vbpy.py` & `vbpy-1.1/vbpy/load_claim_auto.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,270 +1,16 @@
 import pandas as pd
 import numpy as np
 pd.set_option('display.max_rows', None) 
 pd.set_option('display.max_columns', None)  
-
-
-import pandas as pd
 import os
 import re
 from tqdm import tqdm
 
-def load_revenue_auto(directory, skip_rows=13, lhnv = None):
-    # Regular expression to find a four-digit year in the file name
-    year_pattern = re.compile(r'\b(\d{4})\b')
-
-    # List to keep track of the names of the DataFrames stored as globals
-    global_df_names = []
-
-    # Iterate through each file in the specified directory
-    for file in sorted(os.listdir(directory)):
-        if file.endswith('.xlsx') and not file.startswith('~$'):
-            
-            # Find the year in the file name
-            match = year_pattern.search(file)
-            if match:
-                year = match.group(1)
-                file_path = os.path.join(directory, file)
-                try:
-                    """ IMPORT DATA"""
-                    print(f"\n\n\nxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx\n--------------------------------------------------------------------------\nImporting: {file}")
-                    # Load and clean data specifying the engine
-                    df = pd.read_excel(file_path, header=None, skiprows=skip_rows, engine='openpyxl')
-                    df.drop(df.columns[-1], axis = 1, inplace = True)  # remove na col at the end
-
-                    # Dynamically determine headers based on the first non-empty cell per column
-                    headers = []
-                    for col in df.columns:
-                        if pd.notna(df.iloc[1, col]):
-                            headers.append(df.iloc[1, col])
-                        elif pd.notna(df.iloc[0, col]) and pd.isna(df.iloc[1, col]):
-                            headers.append(df.iloc[0, col])
-                        else:
-                            print(f'No headers found for {col}')
-
-                    # Set the determined headers as column names
-                    df.columns = headers
-                    df = df.drop([0, 1])
-                    df.reset_index(drop = True, inplace=True)
-                    print(f'   Rows = {df.shape[0]}')
-                    # print(f'Columns = {df.shape[1]}')
-            
-            
-                    """ RENAME COLUMNS"""
-                    print("--------------------------------------------------------------------------\nRenaming Columns:")
-                    df_rev_dict = {
-                        'Mã đơn vị': 'MA_DVI',
-                        'Mã đơn vị quản lý hợp đồng': 'MA_DVI_QL',
-                        'Số hợp đồng': 'SO_HD',
-                        'Đối tượng bảo hiểm': 'SO_BIEN_XE',
-                        'Giấy chứng nhận': 'SO_GCN',
-                        'Giấy chứng nhận gốc': 'SO_GCN_GOC',
-                        'Tuổi xe': 'TUOI_XE',
-                        'Phòng': 'PHONG_BT',
-                        'Ngày cấp': 'NGAY_CAP',
-                        'Ngày HL': 'NGAY_HL',
-                        'Ngày kết thúc': 'NGAY_KT',
-                        'Mã khách hàng': 'MA_KH',
-                        'Tên khách hàng': 'TEN_KH',
-                        'Nguồn KT': 'NGUON_KT',
-                        'LHNV': 'MA_LHNV',
-                        'Tên LHNV': 'TEN_LHNV',
-                        'Nguyên tệ số tiền BH': 'NGUYEN_TE',
-                        'Số tiền bảo hiểm': 'STBH',
-                        'Phí doanh thu': 'PHI_BH',
-                        'Mã đối tượng': 'NHOM_XE',
-                        'Loại': 'NHOM_XE_2',
-                        'Nhóm': 'LOAI_XE',
-                        'Loại KH': 'LOAI_KH',
-                        'Phân khúc': 'PHAN_KHUC_KH',
-                        'Số CMT/MST': 'SO_CMT/MST',
-                        'Đại lý': 'DAI_LY',
-                        'CBQL': 'CAN_BO_QL',
-                        'Giá trị xe': 'GIA_TRI_XE'
-                    }
-
-                    df.rename(columns={col: df_rev_dict[col] for col in df.columns if col in df_rev_dict}, inplace=True)
-
-
-                    """ REMOVE UNNECESSARY COLUMNS"""
-                    print("--------------------------------------------------------------------------\nRemoving Unneeded Columns:")
-                    removed_cols = [
-                        'Nhóm KH',
-                        'Người thụ hưởng',
-                        'Ngày bán hàng',
-                        'Ngày kỳ thanh toán',
-                        'Kiểu ĐBH', 
-                        'TL của VBI',
-                        'STT'
-                    ]
-
-                    # Removing columns, check if the columns exist
-                    columns_to_remove = [col for col in removed_cols if col in df.columns]
-                    df.drop(columns=columns_to_remove, inplace=True)
-                    
-                    # Remove Reins Columns
-                    try:
-                        phi_bh_index = df.columns.get_loc("PHI_BH")
-                    except KeyError:
-                        print("Column 'PHI_BH' not found in DataFrame")
-                        raise
-
-                    # Step 2: Drop from the next column after "PHI_BH" onwards
-                    df.drop(df.columns[phi_bh_index + 1:], axis=1, inplace=True)
-
-
-                    """ FILTER FOR LHNV"""
-                    if lhnv:
-                        print("--------------------------------------------------------------------------\nFiltering for LHNV:")    
-                        rows_b4 = df.shape[0]    
-                        df = df[df['MA_LHNV'] == lhnv]
-                        print(f'   Removed: {(rows_b4 - df.shape[0]):,.0f} Rows, ({((rows_b4 - df.shape[0])/rows_b4*100):.2f}%)')
-
-
-                    """ CONVERT DATE COLUMNS"""           
-                    print("--------------------------------------------------------------------------\nReformatting Date Cols:")
-                    dates_columns = [
-                        "NGAY_CAP",
-                        "NGAY_HL",
-                        "NGAY_KT"
-                    ]
-
-                    for dates_col in dates_columns:
-                        if dates_col in df.columns:  # Ensure column exists before converting
-                            original_na_count = df[dates_col].isna().sum()
-                            df[dates_col] = pd.to_datetime(df[dates_col], errors='coerce', dayfirst=True)
-                            new_na_count = df[dates_col].isna().sum()
-                            detected_errors = new_na_count - original_na_count
-                            if detected_errors > 0:
-                                print(f"   Detected {detected_errors} Incorrect Dates in {dates_col}")
-                        else:
-                            print(f"   Column {dates_col} not found in DataFrame.")
-
-
-                    """ CONVERT NUMERICAL COLUMNS"""
-                    print("--------------------------------------------------------------------------\nReformatting Num Cols:")
-                    num_columns = [
-                        'TUOI_XE',
-                        'STBH',
-                        'PHI_BH',
-                        'GIA_TRI_XE'
-                    ]
-                    
-                    for num_col in num_columns:
-                        if num_col in df.columns:  # Ensure column exists before converting
-                            original_na_count = df[num_col].isna().sum()
-                            df[num_col] = pd.to_numeric(df[num_col], errors='coerce')
-                            new_na_count = df[num_col].isna().sum()
-                            detected_errors = new_na_count - original_na_count
-                            if detected_errors > 0:
-                                print(f"   Detected {detected_errors} Incorrect Values in {num_col}")
-                        else:
-                            print(f"   Column {num_col} not found in DataFrame.")
-                    
-                    """ PROCESS DUPLICATED/COINSURED ROWS """
-                    if year != '2020':  #SO_GCN was not recorded before 2021.
-                        print("--------------------------------------------------------------------------\nProcessing Dup/Coins Rows:")
-
-                        """ Step 1 - Remove Duplicated Policies """  # Result - Removed Policies with multiple Premium Transactions
-                        _nrows_bf1 = df.shape[0]
-                        _rev_bf1 = df['PHI_BH'].sum()
-                        df = df[~df.duplicated(subset = ['MA_DVI', 'SO_HD', 'SO_GCN', 'SO_BIEN_XE', 'STBH'])] # Policies with the same Pol ID, Department ID, GCN, and SI amount are duplicates
-
-                        print(f"Step 1 - Remove Duplicates\n   -Removed {(_nrows_bf1 - df.shape[0]):,.0f} Rows\n   -Change in Tot Revenue = {(_rev_bf1 - df['PHI_BH'].sum()):,.0f} ({((_rev_bf1 - df['PHI_BH'].sum())/_rev_bf1*100):,.0f}%)")
-
-                        """ Step 2 - Aggregate Claims with Multiple Department IDs """  # Poclies with same Claim ID, different Department ID
-                        _nrows_bf2 = df.shape[0]
-                        _rev_bf2 = df['PHI_BH'].sum()
-                        df["IS_MAIN"] = df.apply(lambda x: x["SO_HD"][:3] == x["MA_DVI"], axis=1)
-                        df = df[df["IS_MAIN"]]
-                        df.drop('IS_MAIN', axis = 1, inplace = True)
-
-                        print(f"Step 2 - Adjust for Internal Coinsurance\n   -Removed {(_nrows_bf2 - df.shape[0]):,.0f} Rows\n   -Change in Tot Revenue = {(_rev_bf2 - df['PHI_BH'].sum()):,.0f} ({((_rev_bf2 - df['PHI_BH'].sum())/_rev_bf2*100):,.0f}%)")
-
-                        """ Step 3 - Remove the rest of the Dups """ 
-                        _nrows_bf3 = df.shape[0] 
-                        _rev_bf3 = df['PHI_BH'].sum()
-                        df = df[~df.duplicated(subset = ['NGAY_HL', 'SO_GCN', 'SO_BIEN_XE', 'SO_HD', 'STBH'])]
-        
-                        print(f"Step 3 - Remove Rest of Duplicates\n   -Removed {(_nrows_bf3 - df.shape[0]):,.0f} Rows\n   -Change in Tot Revenue = {(_rev_bf3 - df['PHI_BH'].sum()):,.0f} ({((_rev_bf3 - df['PHI_BH'].sum())/_rev_bf3*100):,.0f}%)")
-                        
-                    
-                    """ REMOVE ROWs WITH MISSING EFF DATE """
-                    print("--------------------------------------------------------------------------\nRemove Rows Missing NGAY_HL:")    
-                    rows_b4 = df.shape[0]    
-                    df = df[df['NGAY_HL'].notna()]
-                    print(f'   Removed: {(rows_b4 - df.shape[0]):,.0f} Rows, ({((rows_b4 - df.shape[0])/rows_b4*100):.2f}%)')
-                    
-                    
-                    " STANDARDIZE PLATE IDs"
-                    print("--------------------------------------------------------------------------\nStandardizing SO_BIEN_XE:")    
-                    pattern = r'^\d+\d+[A-Za-z].*$' #Number-Number-Letter... (eg, 29A)
-                    _copy = df['SO_BIEN_XE'].copy()
-                    df['SO_BIEN_XE'][~df['SO_BIEN_XE'].str.match(pattern, na = False)] = np.nan # Converted 7253 Inccorect values to NaN
-                    df['SO_BIEN_XE'] = df['SO_BIEN_XE'].str.replace('[^a-zA-Z0-9]', '', regex=True).upper()
-                    
-                    print(f'   Changed: {(df['SO_BIEN_XE'] == _copy)} values')
-                    print(f'   Converted: {df['SO_BIEN_XE'].isna().sum() - _copy.isna().sum()} to NAs')
-                    del _copy
-                    
-                    
-                    """ PRINT EFF_YEAR COUNTS IN EACH DF"""
-                    print("--------------------------------------------------------------------------\nEff Year Count:")
-                    df['NAM_HL'] = df['NGAY_HL'].dt.year 
-                    print(f"Effective Year Count in CY{year}: {df['NAM_HL'].value_counts()}")
-                    
-                    
-                    """ SAVE DF TO GLOBAL VARIABLE"""
-                    print("--------------------------------------------------------------------------\nSaving DF:")
-                    # Assign DataFrame to a global variable dynamically using the year
-                    df_name = f'df_rev_{year}'
-                    globals()[df_name] = df
-                    global_df_names.append(df_name)
-                    print(f"Summary of CY{year}:\n   -NUM POLS = {df.shape[0]:,.0f}\n   -TOTAL REVENUE = {df['PHI_BH'].sum():,.0f}")
-                    print('--------------------------------------------------------------------------\nxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx')
-                except Exception as e:
-                    print(f"Failed to process {file}: {e}")
-            else:
-                print(f"No year found in the file name {file}")
-
-    # Print all global DataFrame names created
-    print("\n\n\n==========================================================================\n==========================================================================\nSuccessfully Imported:", ", ".join(global_df_names))
-    
-    """ CONCAT INTO ONE DF"""
-    all_dataframes = [globals()[name] for name in global_df_names if name in globals()]
-    df_rev = pd.concat(all_dataframes, ignore_index=True)
-    print(f"   -NUM POLS = {df_rev.shape[0]:,.0f}\n   -TOTAL REVENUE = {df_rev['PHI_BH'].sum():,.0f}")
-    
-    print("==========================================================================\n==========================================================================")
-    for name in global_df_names:
-        del globals()[name]
-        
-    global_df_names.clear()
-    
-    return df_rev
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-def load_claim_data(directory, skip_rows=13, lhnv = None):
+def load_claim_auto(directory, skip_rows=13, lhnv = None):
     # Regular expression to find a four-digit year in the file name
     year_pattern = re.compile(r'\b(\d{4})\b')
 
     # List to keep track of the names of the DataFrames stored as globals
     global_df_names = []
 
     # Iterate through each file in the specified directory
@@ -566,8 +312,9 @@
     
     print("==========================================================================\n==========================================================================")
     for name in global_df_names:
         del globals()[name]
         
     global_df_names.clear()
     
-    return df_clm
+    return df_clm
+
```

