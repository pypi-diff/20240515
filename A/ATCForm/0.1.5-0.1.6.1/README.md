# Comparing `tmp/atcform-0.1.5.tar.gz` & `tmp/atcform-0.1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atcform-0.1.5.tar", last modified: Wed May 15 12:27:08 2024, max compression
+gzip compressed data, was "atcform-0.1.6.1.tar", last modified: Wed May 15 16:32:23 2024, max compression
```

## Comparing `atcform-0.1.5.tar` & `atcform-0.1.6.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 12:27:08.608526 atcform-0.1.5/
--rw-rw-rw-   0        0        0     1082 2024-05-14 15:47:09.000000 atcform-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     1824 2024-05-15 12:27:08.606017 atcform-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1129 2024-05-15 12:25:39.000000 atcform-0.1.5/README.md
--rw-rw-rw-   0        0        0       86 2024-05-14 11:46:25.000000 atcform-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-15 12:27:08.608526 atcform-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1050 2024-05-15 12:26:49.000000 atcform-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 12:27:08.566082 atcform-0.1.5/src/
-drwxrwxrwx   0        0        0        0 2024-05-15 12:27:08.585639 atcform-0.1.5/src/ATCForm/
--rw-rw-rw-   0        0        0    23874 2024-05-15 12:22:05.000000 atcform-0.1.5/src/ATCForm/AUTO_FORM.py
--rw-rw-rw-   0        0        0      140 2024-05-14 16:38:01.000000 atcform-0.1.5/src/ATCForm/__init__.py
--rw-rw-rw-   0        0        0     1873 2024-05-14 16:37:56.000000 atcform-0.1.5/src/ATCForm/examlpe.py
-drwxrwxrwx   0        0        0        0 2024-05-15 12:27:08.602296 atcform-0.1.5/src/ATCForm.egg-info/
--rw-rw-rw-   0        0        0     1824 2024-05-15 12:27:08.000000 atcform-0.1.5/src/ATCForm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2024-05-15 12:27:08.000000 atcform-0.1.5/src/ATCForm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 12:27:08.000000 atcform-0.1.5/src/ATCForm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-15 12:27:08.000000 atcform-0.1.5/src/ATCForm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-15 12:27:08.000000 atcform-0.1.5/src/ATCForm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 16:32:23.775226 atcform-0.1.6.1/
+-rw-rw-rw-   0        0        0     1082 2024-05-14 15:47:09.000000 atcform-0.1.6.1/LICENSE
+-rw-rw-rw-   0        0        0     1826 2024-05-15 16:32:23.774116 atcform-0.1.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1129 2024-05-15 12:25:39.000000 atcform-0.1.6.1/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-14 11:46:25.000000 atcform-0.1.6.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-15 16:32:23.776230 atcform-0.1.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     1052 2024-05-15 16:31:49.000000 atcform-0.1.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:32:23.753662 atcform-0.1.6.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-15 16:32:23.763971 atcform-0.1.6.1/src/ATCForm/
+-rw-rw-rw-   0        0        0    23319 2024-05-15 16:31:16.000000 atcform-0.1.6.1/src/ATCForm/AUTO_FORM.py
+-rw-rw-rw-   0        0        0      140 2024-05-14 16:38:01.000000 atcform-0.1.6.1/src/ATCForm/__init__.py
+-rw-rw-rw-   0        0        0     1873 2024-05-14 16:37:56.000000 atcform-0.1.6.1/src/ATCForm/examlpe.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:32:23.772929 atcform-0.1.6.1/src/ATCForm.egg-info/
+-rw-rw-rw-   0        0        0     1826 2024-05-15 16:32:23.000000 atcform-0.1.6.1/src/ATCForm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2024-05-15 16:32:23.000000 atcform-0.1.6.1/src/ATCForm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 16:32:23.000000 atcform-0.1.6.1/src/ATCForm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-15 16:32:23.000000 atcform-0.1.6.1/src/ATCForm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-15 16:32:23.000000 atcform-0.1.6.1/src/ATCForm.egg-info/top_level.txt
```

### Comparing `atcform-0.1.5/LICENSE` & `atcform-0.1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `atcform-0.1.5/PKG-INFO` & `atcform-0.1.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ATCForm
-Version: 0.1.5
+Version: 0.1.6.1
 Summary: ATCFrom - Automatically fill in the collection form 自动化表单填写工具
 Home-page: https://github.com/YKONGCO/ATCForm
 Author: YKONGCO
 Author-email: 1570585752@qq.com
 Maintainer: YKONGCO
 Maintainer-email: 1570585752@qq.com
 License: MIT License
```

### Comparing `atcform-0.1.5/README.md` & `atcform-0.1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `atcform-0.1.5/setup.py` & `atcform-0.1.6.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ATCForm",
-    version="0.1.5",
+    version="0.1.6.1",
     description="ATCFrom - Automatically fill in the collection form 自动化表单填写工具",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/YKONGCO/ATCForm",
     author="YKONGCO",
     author_email="1570585752@qq.com",
     maintainer="YKONGCO",
```

### Comparing `atcform-0.1.5/src/ATCForm/AUTO_FORM.py` & `atcform-0.1.6.1/src/ATCForm/AUTO_FORM.py`

 * *Files 9% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             option=input("请输入你需要的勾选的选项(输入exit：退出)：")
             if(option=="exit"):
                 return
             self.select_list.append(option)        
     
     
     def display_all_qus(self):
-        print("问题列表")
+        print("----问题列表----")
         elements=self.driver.find_elements(By.CSS_SELECTOR, ".ant-col.field-container.field")
         for element in elements:
             class_names = element.get_attribute("class")
             if "MobileField" not in class_names:
                 print(element.text.replace("\n","").replace("*",""))
         print("-----------------------------")
         return elements
@@ -87,15 +87,15 @@
     
     
       
     
     
     
     def get_questions_input(self):
-        print("input列表")
+        print("----input列表----")
         elements = self.driver.find_elements(By.CSS_SELECTOR, ".ant-col.field-container.field")
         filtered_elements = []
         for element in elements:
             # 检查元素的 class 名称
             class_names = element.get_attribute("class")
             if "MobileField" in class_names:
                 print(element.text.replace("\n", "").replace("*", ""))
@@ -107,15 +107,15 @@
                 print(element.text.replace("\n", "").replace("*", ""))
                 filtered_elements.append(element)
         return filtered_elements
     
     
     
     def get_questions_select(self):
-        print("select列表")
+        print("----select列表----")
         elements = self.driver.find_elements(By.CSS_SELECTOR, ".ant-col.field-container.field") #ant-col.field-container.field SectionBreak
         filtered_elements = []
         for element in elements:
             class_names = element.get_attribute("class")
             if "MobileField" in class_names:
                 pass
             elif "NameField" in class_names: 
@@ -149,38 +149,32 @@
         :return: True
         """
         if(input_time=="" and self.wait_time=="" ):
             input_time=input("请输入等待时间：")
         elif(input_time=="" and self.wait_time!=""):
             input_time=self.wait_time
         
-        # 当前时间
         try:
-            # 将输入时间字符串转换为时间元组
             time_tuple = time.strptime(input_time, "%Y%m%d%H%M")
-            # 将时间元组转换为时间戳
             start_timestamp  = time.mktime(time_tuple)
-    
             if(start_timestamp<time.time()):
                 print("收集表已经开始")
                 return True
             
             cnt=0
             while(1):
                 cnt+=1
                 current_timestamp = time.time()
                 current_time_str = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(current_timestamp))
                 if(cnt%200000==0):
-                    # os.system("cls")
                     print("正在等待当前时间为",current_time_str)
             
                 if(current_timestamp >= start_timestamp+1):
                     self.driver.refresh()
                     return True
-                # os.system("cls")
         except ValueError:
             print("输入时间格式不正确，请输入正确的时间格式，例如：202405101328") 
         
        
             
     def Initializes_the_answer_list(self):
         elements=self.get_questions_input()
@@ -206,30 +200,30 @@
     def auto_input(self):
         """自动输入值到具有指定名称的输入框中。
 
         Args:
             INPUT_NAME (str): 输入框的名称
             val (str): 要输入的值
         """
-        # data_qid="formlw0lalc7-SIMPLE1715339748648lw0kzwvc"
-        
         try: 
+            print("----自动输入-----")
             elements=self.get_questions_input()
             index=0
             for element in elements:
                 input_element=element.find_element(By.CSS_SELECTOR, "input")
                 self.driver.execute_script("arguments[0].scrollIntoView(true);", input_element)
                 input_element.send_keys(self.answer_list[index])
                 input_element.submit()
                 index+=1
         except:
             print("填写失败")
             exit()
 
-    def auto_click_button(self):
+    def auto_button(self):
+        print("----自动选择-----")
         for item in self.select_list:
             buttons = self.driver.find_elements(By.XPATH, f"//span[text()='{item}']")
             print(buttons)
             for button in buttons:
                 self.driver.execute_script("arguments[0].scrollIntoView(true);", button)
                 # self.actions.click(button).perform()
                 button.click()
@@ -237,15 +231,16 @@
         
                 
                 
 
 
 
 
-    def auto_submit_click_JSJ(self):
+    def auto_submit(self):
+        print("----自动提交-----")
         self.driver.execute_script("window.scrollTo(0, document.body.scrollHeight);")   
         button = self.driver.find_element(By.CSS_SELECTOR,".ant-btn.ant-btn-primary.ant-btn-two-chinese-chars.form-theme--submit-button.published-form__submit.FooterButton_button__vJkWw")
         button.click()
         try:
             print("动作已经全部执行")
             time.sleep(1)
             if(self.is_submit()):
@@ -264,20 +259,17 @@
     info_data={}
     select_list=[]
     wait_time :str 
     answer_list=[]
     
     def __init__(self,url : str ):
         options = webdriver.EdgeOptions()
- 
-        # 处理SSL证书错误问题
         options.add_argument('--ignore-certificate-errors')
         options.add_argument('--ignore-ssl-errors')
         options.add_argument("--guest")
-        # 忽略无用的日志
         options.add_experimental_option("excludeSwitches", ['enable-automation', 'enable-logging'])   
         try:
             self.driver=webdriver.Edge(options)
         except:
             download_driver()
             self.driver=webdriver.Edge(options)
         self.actions = ActionChains(self.driver)
@@ -304,15 +296,15 @@
                 exit()
             options_list = option.split()
             self.select_list.append(options_list)
             print("用户选择的选项列表：", options_list)        
     
     
     def display_all_qus(self):
-        print("问题列表")
+        print("----问题列表----")
         elements=self.driver.find_elements(By.CSS_SELECTOR, ".question")
         for element in elements:
             value=element.text.replace("\n","").replace(" ","").replace("*","")
             print(value)
         print("-----------------------------")
         return elements
         
@@ -361,35 +353,35 @@
             
             
            
     
     
     
     def get_questions_input(self):
-        """获取表单的data-qid
-
+        """
         Args:
             driver (webdriver): selenium的webdriver
-
         Returns:
         elements
         """
+        print("----输入列表----")
         elements=self.driver.find_elements(By.CSS_SELECTOR, ".question[data-type='simple']")
         for element in elements:
             value=element.text.replace("\n","").replace(" ","").replace("*","")
             print(value)       
         return elements
     
     
     
     def get_questions_select(self):
         """
         Returns:
         elements
         """
+        print("----选择列表----")
         first_elements=self.driver.find_elements(By.CSS_SELECTOR, ".question")
         elements=[]
         for element in first_elements:
             if(element.get_attribute("data-type")=="radio" or element.get_attribute("data-type")=="checkbox"):
                 elements.append(element)
         for element in elements:
             value=element.text.replace("\n","").replace(" ","").replace("*","")
@@ -428,26 +420,25 @@
                 return True
             
             cnt=0
             while(1):
                 current_timestamp = time.time()
                 current_time_str = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(current_timestamp))
                 if(cnt%200000==0):
-                    # os.system("cls")
                     print("正在等待当前时间为",current_time_str)
-            
                 if(current_timestamp >= start_timestamp-0.02):
                     self.driver.refresh()
                     return True
         except ValueError:
             print("输入时间格式不正确，请输入正确的时间格式，例如：202405101328") 
         
        
             
     def Initializes_the_answer_list(self):
+        print("----初始化答案列表----")
         elements=self.get_questions_input()
         for element in elements:
             question=element.text.replace("\n","").replace(" ","")
             flag=0
             
             for item_key in self.info_data:
                 if(re.search(item_key,question)):
@@ -462,14 +453,15 @@
         print("-----------------------------")        
     
     def auto_input(self):
         """
         自动输入值到具有指定名称的输入框中。
         """
         try: 
+            print("----自动输入----")
             elements=self.get_questions_input()
             index=0
             for element in elements:
                 data_qid=element.get_attribute("data-qid")
                 css_path=f'[data-qid="{data_qid}"]  textarea'
                 print(css_path)
                 textarea = self.driver.find_element(By.CSS_SELECTOR, css_path)
@@ -480,48 +472,32 @@
                 
                 
                 index+=1
         except Exception as e:
             print("填写失败",e)
     
 
-    def auto_click_button(self):
-        """
-        """
-        # for item in self.select_list:
-        #     button=self.driver.find_element(By.XPATH,f"//span[text()='{item}']")
-        #     self.driver.execute_script("arguments[0].scrollIntoView(true);", button)
-        #     button.click() 
+    def auto_button(self):
         try: 
+            print("----自动点击----")
             elements = self.get_questions_select()
             index=0
             for element in elements:
                 for a in self.select_list[index]:
                     button = element.find_element(By.XPATH, f".//span[text()='{a}']")  # 使用"."表示在当前元素下搜索
                     self.driver.execute_script("arguments[0].scrollIntoView(true);", button)
-                    time.sleep(0.5)
                     button.click()
                 index+=1
         except Exception as e:
             print("填写失败",e)
         
         
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
 
 
-    def auto_submit_click_tx(self):
+    def auto_submit(self):
         blank_area = self.driver.find_element(By.CLASS_NAME, "form-header-title-content")
         self.actions.move_to_element(blank_area).click().perform()
         self.driver.execute_script("window.scrollTo(0, document.body.scrollHeight);")   
         button=self.driver.find_element(By.XPATH,"//button[text()='提交']")
         button.click()
         try:
             time.sleep(0.03)
@@ -566,33 +542,32 @@
         self.is_enable=is_enable
         if(is_enable==False):
             self.SELECT_LIST=SELECT_LIST
 
     def run(self):
         self.AT1.wait_for_time()
         self.AT1.auto_input()
-        self.AT1.auto_click_button()
-        self.AT1.auto_submit_click_tx()
+        self.AT1.auto_button()
+        self.AT1.auto_submit()
         
     def init(self):
         self.AT1=AUTO_TX_FORM(self.url)
         self.AT1.set_wait_time(input_time=self.start_time)
         self.AT1.wait_for_login()
         self.AT1.set_base_data(self.data_path)
         if(self.is_enable==False):
             self.AT1.select_list+=self.SELECT_LIST
         self.AT1.display_all_qus()
         self.AT1.Initializes_the_answer_list()
         if(self.AT1.get_questions_select()!=[]):
             self.AT1.set_select_list()
         current_timestamp = time.time()
         time_tuple = time.strptime(self.start_time, "%Y%m%d%H%M")
-        # 将时间元组转换为时间戳
         start_timestamp  = time.mktime(time_tuple)
-        print("任务初始化完成")
+        print("----任务初始化完成----")
         if(current_timestamp < start_timestamp-8):
             print("---------------------")
             print("进入等待时间(5s)，请确认输入结果")
             print("input信息：",self.AT1.answer_list)
             print("select信息：",self.AT1.select_list)
             time.sleep(5)
             
@@ -633,16 +608,16 @@
         self.start_time=start_time
         self.is_enable=is_enable
         if(is_enable==False):
             self.SELECT_LIST=SELECT_LIST
     def run(self):
         self.AJ1.wait_for_time()
         self.AJ1.auto_input()
-        self.AJ1.auto_click_button()
-        self.AJ1.auto_submit_click_JSJ()
+        self.AJ1.auto_button()
+        self.AJ1.auto_submit()
         
     def init(self):
         self.AJ1=AUTO_JSJ_FORM(self.url)
         time.sleep(1)
         self.AJ1.set_wait_time(input_time=self.start_time)
         self.AJ1.set_base_data(self.data_path)
         if(self.is_enable==False):
@@ -650,15 +625,15 @@
         self.AJ1.display_all_qus()
         self.AJ1.Initializes_the_answer_list()
         if(self.AJ1.get_questions_select()!=[] and self.is_enable):
             self.AJ1.set_select_list()
         current_timestamp = time.time()
         time_tuple = time.strptime(self.start_time, "%Y%m%d%H%M")
         start_timestamp  = time.mktime(time_tuple)
-        print("任务初始化完成")
+        print("----任务初始化完成----")
         if(current_timestamp < start_timestamp-8):
             print("---------------------")
             print("进入等待时间(5s)，请确认输入结果")
             print("input信息：",self.AJ1.answer_list)
             print("select信息：",self.AJ1.select_list)
             time.sleep(5)
```

### Comparing `atcform-0.1.5/src/ATCForm/examlpe.py` & `atcform-0.1.6.1/src/ATCForm/examlpe.py`

 * *Files identical despite different names*

### Comparing `atcform-0.1.5/src/ATCForm.egg-info/PKG-INFO` & `atcform-0.1.6.1/src/ATCForm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ATCForm
-Version: 0.1.5
+Version: 0.1.6.1
 Summary: ATCFrom - Automatically fill in the collection form 自动化表单填写工具
 Home-page: https://github.com/YKONGCO/ATCForm
 Author: YKONGCO
 Author-email: 1570585752@qq.com
 Maintainer: YKONGCO
 Maintainer-email: 1570585752@qq.com
 License: MIT License
```

