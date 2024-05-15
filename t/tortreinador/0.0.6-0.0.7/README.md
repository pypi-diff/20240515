# Comparing `tmp/tortreinador-0.0.6.tar.gz` & `tmp/tortreinador-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tortreinador-0.0.6.tar", last modified: Tue Jan 16 11:04:09 2024, max compression
+gzip compressed data, was "tortreinador-0.0.7.tar", last modified: Wed May 15 14:02:21 2024, max compression
```

## Comparing `tortreinador-0.0.6.tar` & `tortreinador-0.0.7.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-01-16 11:04:09.788872 tortreinador-0.0.6/
--rw-rw-rw-   0        0        0     1088 2023-12-08 19:44:58.000000 tortreinador-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     6712 2024-01-16 11:04:09.787926 tortreinador-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     5776 2023-12-09 20:35:38.000000 tortreinador-0.0.6/README.md
--rw-rw-rw-   0        0        0      889 2024-01-16 11:03:30.000000 tortreinador-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-16 11:04:09.788872 tortreinador-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      544 2024-01-16 11:03:30.000000 tortreinador-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-16 11:04:09.732926 tortreinador-0.0.6/test/
--rw-rw-rw-   0        0        0     1633 2024-01-16 11:01:39.000000 tortreinador-0.0.6/test/test.py
-drwxrwxrwx   0        0        0        0 2024-01-16 11:04:09.734926 tortreinador-0.0.6/tortreinador/
--rw-rw-rw-   0        0        0        0 2023-11-29 07:39:26.000000 tortreinador-0.0.6/tortreinador/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 11:04:09.766408 tortreinador-0.0.6/tortreinador/models/
--rw-rw-rw-   0        0        0     3728 2023-11-22 12:48:11.000000 tortreinador-0.0.6/tortreinador/models/MDN.py
--rw-rw-rw-   0        0        0        0 2023-12-09 18:01:34.000000 tortreinador-0.0.6/tortreinador/models/__init__.py
--rw-rw-rw-   0        0        0     7003 2024-01-16 10:56:17.000000 tortreinador-0.0.6/tortreinador/train.py
-drwxrwxrwx   0        0        0        0 2024-01-16 11:04:09.785924 tortreinador-0.0.6/tortreinador/utils/
--rw-rw-rw-   0        0        0      282 2023-10-18 13:20:23.000000 tortreinador-0.0.6/tortreinador/utils/Recorder.py
--rw-rw-rw-   0        0        0     4482 2023-10-20 11:18:43.000000 tortreinador-0.0.6/tortreinador/utils/View.py
--rw-rw-rw-   0        0        0      660 2023-08-17 14:59:13.000000 tortreinador-0.0.6/tortreinador/utils/WarmUpLR.py
--rw-rw-rw-   0        0        0        0 2023-12-09 18:01:50.000000 tortreinador-0.0.6/tortreinador/utils/__init__.py
--rw-rw-rw-   0        0        0      898 2024-01-16 09:21:31.000000 tortreinador-0.0.6/tortreinador/utils/metrics.py
--rw-rw-rw-   0        0        0      687 2024-01-16 09:27:59.000000 tortreinador-0.0.6/tortreinador/utils/plot.py
--rw-rw-rw-   0        0        0     4798 2024-01-16 09:27:59.000000 tortreinador-0.0.6/tortreinador/utils/preprocessing.py
-drwxrwxrwx   0        0        0        0 2024-01-16 11:04:09.786926 tortreinador-0.0.6/tortreinador.egg-info/
--rw-rw-rw-   0        0        0     6712 2024-01-16 11:04:09.000000 tortreinador-0.0.6/tortreinador.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      552 2024-01-16 11:04:09.000000 tortreinador-0.0.6/tortreinador.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-16 11:04:09.000000 tortreinador-0.0.6/tortreinador.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      123 2024-01-16 11:04:09.000000 tortreinador-0.0.6/tortreinador.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-01-16 11:04:09.000000 tortreinador-0.0.6/tortreinador.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 14:02:21.731856 tortreinador-0.0.7/
+-rw-rw-rw-   0        0        0     1088 2023-12-08 19:44:58.000000 tortreinador-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     6890 2024-05-15 14:02:21.731856 tortreinador-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5956 2024-05-15 14:01:33.000000 tortreinador-0.0.7/README.md
+-rw-rw-rw-   0        0        0      887 2024-05-15 13:42:21.000000 tortreinador-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-15 14:02:21.732856 tortreinador-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      544 2024-05-15 14:01:33.000000 tortreinador-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:02:21.641969 tortreinador-0.0.7/test/
+-rw-rw-rw-   0        0        0     2526 2024-04-17 11:54:01.000000 tortreinador-0.0.7/test/test.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:02:21.659188 tortreinador-0.0.7/tortreinador/
+-rw-rw-rw-   0        0        0        0 2023-11-29 07:39:26.000000 tortreinador-0.0.7/tortreinador/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:02:21.687400 tortreinador-0.0.7/tortreinador/models/
+-rw-rw-rw-   0        0        0     3728 2023-11-22 12:48:11.000000 tortreinador-0.0.7/tortreinador/models/MDN.py
+-rw-rw-rw-   0        0        0        0 2023-12-09 18:01:34.000000 tortreinador-0.0.7/tortreinador/models/__init__.py
+-rw-rw-rw-   0        0        0    10064 2024-05-15 13:59:48.000000 tortreinador-0.0.7/tortreinador/train.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:02:21.728402 tortreinador-0.0.7/tortreinador/utils/
+-rw-rw-rw-   0        0        0      282 2023-10-18 13:20:23.000000 tortreinador-0.0.7/tortreinador/utils/Recorder.py
+-rw-rw-rw-   0        0        0     4499 2024-05-15 13:42:21.000000 tortreinador-0.0.7/tortreinador/utils/View.py
+-rw-rw-rw-   0        0        0      660 2023-08-17 14:59:13.000000 tortreinador-0.0.7/tortreinador/utils/WarmUpLR.py
+-rw-rw-rw-   0        0        0        0 2023-12-09 18:01:50.000000 tortreinador-0.0.7/tortreinador/utils/__init__.py
+-rw-rw-rw-   0        0        0     1420 2024-04-17 16:37:42.000000 tortreinador-0.0.7/tortreinador/utils/metrics.py
+-rw-rw-rw-   0        0        0     1590 2024-05-07 15:30:28.000000 tortreinador-0.0.7/tortreinador/utils/plot.py
+-rw-rw-rw-   0        0        0     4798 2024-01-16 09:27:59.000000 tortreinador-0.0.7/tortreinador/utils/preprocessing.py
+-rw-rw-rw-   0        0        0     1197 2024-05-15 13:42:21.000000 tortreinador-0.0.7/tortreinador/utils/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:02:21.730849 tortreinador-0.0.7/tortreinador.egg-info/
+-rw-rw-rw-   0        0        0     6890 2024-05-15 14:02:21.000000 tortreinador-0.0.7/tortreinador.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      580 2024-05-15 14:02:21.000000 tortreinador-0.0.7/tortreinador.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 14:02:21.000000 tortreinador-0.0.7/tortreinador.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      123 2024-05-15 14:02:21.000000 tortreinador-0.0.7/tortreinador.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-15 14:02:21.000000 tortreinador-0.0.7/tortreinador.egg-info/top_level.txt
```

### Comparing `tortreinador-0.0.6/LICENSE` & `tortreinador-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tortreinador-0.0.6/PKG-INFO` & `tortreinador-0.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: tortreinador
-Version: 0.0.6
+Version: 0.0.7
 Summary: A trainer based on Pytorch
 Home-page: https://github.com/ArdenteX/tortreinador
 Author: Xavier
-Author-email: Xavier <zephramxu@example.com>
+Author-email: Xavier <zephramxu@gmail.com>
 Project-URL: Homepage, https://github.com/ArdenteX/tortreinador
 Project-URL: Issues, https://github.com/ArdenteX/tortreinador/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.2
@@ -33,16 +33,20 @@
 This package needs Python>=3.7 and the version of Pytorch used in development is 1.13.1 and cuda11.2, considering the different version of cuda, the package will
 not install Pytorch automatically. You should check your cuda's version, install the suitable [pytorch](https://pytorch.org/get-started/previous-versions/) first. Then, run the command below:
 ```
 pip install tortreinador 
 ```
 ## Quick Start
 ```python
-from tortreinador import train
+from tortreinador.utils.plot import plot_line_2
+from tortreinador.utils.preprocessing import load_data
+from tortreinador.train import TorchTrainer
 from tortreinador.models.MDN import mdn, Mixture, NLLLoss
+from tortreinador.utils.tools import xavier_init
+from tortreinador.utils.View import init_weights, split_weights
 import torch
 import pandas as pd
 
 data = pd.read_excel('D:\\Resource\\Gas_Giants_Core_Earth20W.xlsx')
 data['M_total (M_E)'] = data['Mcore (M_J/10^3)'] + data['Menv (M_E)']
 
 # Support index, e.g input_parameters = [0, 1, 2]
@@ -54,42 +58,46 @@
 
 output_parameters = [
     'M_total (M_E)',
     'T_int (K)',
     'P_CEB (Mbar)',
     'T_CEB (K)'
 ]
-
-trainer = train.TorchTrainer()
-
 # Load Data
-t_loader, v_loader, test_x, test_y, s_x, s_y = trainer.load_data(data=data, input_parameters=input_parameters,
-                                                                 output_parameters=output_parameters,
-                                                                 if_normal=True, if_shuffle=True)
-
-# Model
-model = mdn(len(input_parameters), len(output_parameters), 10, 256)
+t_loader, v_loader, t_x, t_y, m_x, m_y = load_data(data, input_parameters, output_parameters, batch_size=256)
 
-# Loss
+model = mdn(len(input_parameters), len(output_parameters), 20, 512)
 criterion = NLLLoss()
-pdf = Mixture()
+optim = torch.optim.Adam(xavier_init(model), lr=0.0001, weight_decay=0.001)
 
-# Optimizer
-optim = torch.optim.Adam(trainer.xavier_init(model), lr=0.0001984, weight_decay=0.001)
+trainer = TorchTrainer(is_gpu=True, epoch=50, optimizer=optim, model=model, criterion=criterion)
 
+'''
+        kwargs: model_save_path -> m_p, warmup_epoch(option) -> w_e, lr_milestones and gamma(option) -> l_m, best_metric(eg: r2) -> b_m
+'''
+config = {
+    'b_m': 0.8,
+    'm_p': 'D:\\Resource\\MDN\\PackageTest\\savedModel\\',
+    'w_e': 5,
+    'l_m': {
+        's_l': [20, 40],
+        'gamma': 0.7
+    }
+}
 # Training
-t_l, v_l, val_r2, train_r2, mse = trainer.fit_for_MDN(t_loader, v_loader, criterion, model=model, mixture=pdf,
-                                                      model_save_path='D:\\Resource\\MDN\\', optim=optim, best_r2=0.5)
+result = trainer.fit(t_loader, v_loader, **config)
+
+
 # Plot line chart
 result_pd = pd.DataFrame()
-result_pd['epoch'] = range(150)
-result_pd['train_r2_avg'] = train_r2
-result_pd['val_r2_avg'] = val_r2
+result_pd['epoch'] = len(result[0])
+result_pd['train_r2_avg'] = result[4]
+result_pd['val_r2_avg'] = result[3]
 
-trainer.plot_line_2(y_1='train_r2_avg', y_2='val_r2_avg', df=result_pd, fig_size=(10, 6), output_path="your save path", dpi=300)
+plot_line_2(y_1='train_r2_avg', y_2='val_r2_avg', df=result_pd, fig_size=(10, 6), output_path=".\\imgs\\GasGiants_MDN20240116_TrainValR2_2.png", dpi=300)
 ```
 ## Functions
 This package just support MDN for now, but the ```load_data``` is suitable for every condition as long as the type of data is Dataframe
 
 - tortreinador.train.TorchTrainer():
    + Parameters:
      + batch_size: int = 512
@@ -138,26 +146,28 @@
          + model: Any,
          + pdf: Any,
          + x: Any,
          + y: Any,
          + criterion: Any,
          + t: str = 'train'
        ```python
-         def _calculate(self, model, pdf, x, y, criterion, t='train'):
-             pi, mu, sigma = model(x)
+       # Please call self._standard_return() at the end
+       def calculate(self, x, y, mode='t'):
+
+            pi, mu, sigma = self.model(x)
 
-             mixture = pdf(pi, mu, sigma)
+            loss = self.criterion(pi, mu, sigma, y)
 
-             y_pred = mixture.sample()
+            pdf = mixture(pi, mu, sigma)
 
-             if t == 'train':
-               return criterion(pi, mu, sigma, y), y_pred.cpu().numpy(), y.cpu().numpy()
+            y_pred = pdf.sample()
 
-             else:
-               return criterion(pi, mu, sigma, y), self.mse(y_pred, y), y_pred.cpu().numpy(), y.cpu().numpy()
+            metric_per = r2_score(y, y_pred)
+            
+            return self._standard_return(loss, metric_per, mode, y, y_pred)
          ```
      + fit_for_MDN()
        + Describe: ***Train loop for MDN(Mixture Density Network)*** 
        + Parameters:
          + t_l: Dataloader
          + v_l: Dataloader
          + criterion: Module
```

### Comparing `tortreinador-0.0.6/README.md` & `tortreinador-0.0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,20 @@
 This package needs Python>=3.7 and the version of Pytorch used in development is 1.13.1 and cuda11.2, considering the different version of cuda, the package will
 not install Pytorch automatically. You should check your cuda's version, install the suitable [pytorch](https://pytorch.org/get-started/previous-versions/) first. Then, run the command below:
 ```
 pip install tortreinador 
 ```
 ## Quick Start
 ```python
-from tortreinador import train
+from tortreinador.utils.plot import plot_line_2
+from tortreinador.utils.preprocessing import load_data
+from tortreinador.train import TorchTrainer
 from tortreinador.models.MDN import mdn, Mixture, NLLLoss
+from tortreinador.utils.tools import xavier_init
+from tortreinador.utils.View import init_weights, split_weights
 import torch
 import pandas as pd
 
 data = pd.read_excel('D:\\Resource\\Gas_Giants_Core_Earth20W.xlsx')
 data['M_total (M_E)'] = data['Mcore (M_J/10^3)'] + data['Menv (M_E)']
 
 # Support index, e.g input_parameters = [0, 1, 2]
@@ -28,42 +32,46 @@
 
 output_parameters = [
     'M_total (M_E)',
     'T_int (K)',
     'P_CEB (Mbar)',
     'T_CEB (K)'
 ]
-
-trainer = train.TorchTrainer()
-
 # Load Data
-t_loader, v_loader, test_x, test_y, s_x, s_y = trainer.load_data(data=data, input_parameters=input_parameters,
-                                                                 output_parameters=output_parameters,
-                                                                 if_normal=True, if_shuffle=True)
-
-# Model
-model = mdn(len(input_parameters), len(output_parameters), 10, 256)
+t_loader, v_loader, t_x, t_y, m_x, m_y = load_data(data, input_parameters, output_parameters, batch_size=256)
 
-# Loss
+model = mdn(len(input_parameters), len(output_parameters), 20, 512)
 criterion = NLLLoss()
-pdf = Mixture()
+optim = torch.optim.Adam(xavier_init(model), lr=0.0001, weight_decay=0.001)
 
-# Optimizer
-optim = torch.optim.Adam(trainer.xavier_init(model), lr=0.0001984, weight_decay=0.001)
+trainer = TorchTrainer(is_gpu=True, epoch=50, optimizer=optim, model=model, criterion=criterion)
 
+'''
+        kwargs: model_save_path -> m_p, warmup_epoch(option) -> w_e, lr_milestones and gamma(option) -> l_m, best_metric(eg: r2) -> b_m
+'''
+config = {
+    'b_m': 0.8,
+    'm_p': 'D:\\Resource\\MDN\\PackageTest\\savedModel\\',
+    'w_e': 5,
+    'l_m': {
+        's_l': [20, 40],
+        'gamma': 0.7
+    }
+}
 # Training
-t_l, v_l, val_r2, train_r2, mse = trainer.fit_for_MDN(t_loader, v_loader, criterion, model=model, mixture=pdf,
-                                                      model_save_path='D:\\Resource\\MDN\\', optim=optim, best_r2=0.5)
+result = trainer.fit(t_loader, v_loader, **config)
+
+
 # Plot line chart
 result_pd = pd.DataFrame()
-result_pd['epoch'] = range(150)
-result_pd['train_r2_avg'] = train_r2
-result_pd['val_r2_avg'] = val_r2
+result_pd['epoch'] = len(result[0])
+result_pd['train_r2_avg'] = result[4]
+result_pd['val_r2_avg'] = result[3]
 
-trainer.plot_line_2(y_1='train_r2_avg', y_2='val_r2_avg', df=result_pd, fig_size=(10, 6), output_path="your save path", dpi=300)
+plot_line_2(y_1='train_r2_avg', y_2='val_r2_avg', df=result_pd, fig_size=(10, 6), output_path=".\\imgs\\GasGiants_MDN20240116_TrainValR2_2.png", dpi=300)
 ```
 ## Functions
 This package just support MDN for now, but the ```load_data``` is suitable for every condition as long as the type of data is Dataframe
 
 - tortreinador.train.TorchTrainer():
    + Parameters:
      + batch_size: int = 512
@@ -112,26 +120,28 @@
          + model: Any,
          + pdf: Any,
          + x: Any,
          + y: Any,
          + criterion: Any,
          + t: str = 'train'
        ```python
-         def _calculate(self, model, pdf, x, y, criterion, t='train'):
-             pi, mu, sigma = model(x)
+       # Please call self._standard_return() at the end
+       def calculate(self, x, y, mode='t'):
+
+            pi, mu, sigma = self.model(x)
 
-             mixture = pdf(pi, mu, sigma)
+            loss = self.criterion(pi, mu, sigma, y)
 
-             y_pred = mixture.sample()
+            pdf = mixture(pi, mu, sigma)
 
-             if t == 'train':
-               return criterion(pi, mu, sigma, y), y_pred.cpu().numpy(), y.cpu().numpy()
+            y_pred = pdf.sample()
 
-             else:
-               return criterion(pi, mu, sigma, y), self.mse(y_pred, y), y_pred.cpu().numpy(), y.cpu().numpy()
+            metric_per = r2_score(y, y_pred)
+            
+            return self._standard_return(loss, metric_per, mode, y, y_pred)
          ```
      + fit_for_MDN()
        + Describe: ***Train loop for MDN(Mixture Density Network)*** 
        + Parameters:
          + t_l: Dataloader
          + v_l: Dataloader
          + criterion: Module
```

### Comparing `tortreinador-0.0.6/pyproject.toml` & `tortreinador-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tortreinador"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
-  { name="Xavier", email="zephramxu@example.com" },
+  { name="Xavier", email="zephramxu@gmail.com" },
 ]
 description = "A trainer based on Pytorch"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
```

### Comparing `tortreinador-0.0.6/setup.py` & `tortreinador-0.0.7/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='tortreinador',
-    version='0.0.6',
+    version='0.0.7',
     author='Xavier',
     author_email='zephramxu@gmail.com',
     url='https://github.com/ArdenteX/tortreinador',
     packages=['tortreinador', 'tortreinador.models', 'tortreinador.utils'],
     install_requires=[
         'pandas>=1.4.2',
         'seaborn>=0.11.2',
```

### Comparing `tortreinador-0.0.6/tortreinador/models/MDN.py` & `tortreinador-0.0.7/tortreinador/models/MDN.py`

 * *Files identical despite different names*

### Comparing `tortreinador-0.0.6/tortreinador/utils/View.py` & `tortreinador-0.0.7/tortreinador/utils/View.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,22 +129,24 @@
 
 
 def visualize_learning_rate(writer, lr, epoch):
     """visualize learning rate"""
     writer.add_scalar('Train/LearningRate', lr, epoch)
 
 
+# Xavier init
+
+
 # device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 # net = eca_resnet50(num_classes=2)
 # net = nn.DataParallel(net)
 # net.to(device)
 # # split_weights(net)
 # a = []
 # for m in net.modules():
 #     if isinstance(m, nn.Conv1d):
 #         print("Yes")
 #         # for sub in m.modules():
 #         #     a.append(sub)
 #         #     print(sub)
 #
 #         break
-
```

### Comparing `tortreinador-0.0.6/tortreinador/utils/WarmUpLR.py` & `tortreinador-0.0.7/tortreinador/utils/WarmUpLR.py`

 * *Files identical despite different names*

### Comparing `tortreinador-0.0.6/tortreinador/utils/preprocessing.py` & `tortreinador-0.0.7/tortreinador/utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `tortreinador-0.0.6/tortreinador.egg-info/PKG-INFO` & `tortreinador-0.0.7/tortreinador.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: tortreinador
-Version: 0.0.6
+Version: 0.0.7
 Summary: A trainer based on Pytorch
 Home-page: https://github.com/ArdenteX/tortreinador
 Author: Xavier
-Author-email: Xavier <zephramxu@example.com>
+Author-email: Xavier <zephramxu@gmail.com>
 Project-URL: Homepage, https://github.com/ArdenteX/tortreinador
 Project-URL: Issues, https://github.com/ArdenteX/tortreinador/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.2
@@ -33,16 +33,20 @@
 This package needs Python>=3.7 and the version of Pytorch used in development is 1.13.1 and cuda11.2, considering the different version of cuda, the package will
 not install Pytorch automatically. You should check your cuda's version, install the suitable [pytorch](https://pytorch.org/get-started/previous-versions/) first. Then, run the command below:
 ```
 pip install tortreinador 
 ```
 ## Quick Start
 ```python
-from tortreinador import train
+from tortreinador.utils.plot import plot_line_2
+from tortreinador.utils.preprocessing import load_data
+from tortreinador.train import TorchTrainer
 from tortreinador.models.MDN import mdn, Mixture, NLLLoss
+from tortreinador.utils.tools import xavier_init
+from tortreinador.utils.View import init_weights, split_weights
 import torch
 import pandas as pd
 
 data = pd.read_excel('D:\\Resource\\Gas_Giants_Core_Earth20W.xlsx')
 data['M_total (M_E)'] = data['Mcore (M_J/10^3)'] + data['Menv (M_E)']
 
 # Support index, e.g input_parameters = [0, 1, 2]
@@ -54,42 +58,46 @@
 
 output_parameters = [
     'M_total (M_E)',
     'T_int (K)',
     'P_CEB (Mbar)',
     'T_CEB (K)'
 ]
-
-trainer = train.TorchTrainer()
-
 # Load Data
-t_loader, v_loader, test_x, test_y, s_x, s_y = trainer.load_data(data=data, input_parameters=input_parameters,
-                                                                 output_parameters=output_parameters,
-                                                                 if_normal=True, if_shuffle=True)
-
-# Model
-model = mdn(len(input_parameters), len(output_parameters), 10, 256)
+t_loader, v_loader, t_x, t_y, m_x, m_y = load_data(data, input_parameters, output_parameters, batch_size=256)
 
-# Loss
+model = mdn(len(input_parameters), len(output_parameters), 20, 512)
 criterion = NLLLoss()
-pdf = Mixture()
+optim = torch.optim.Adam(xavier_init(model), lr=0.0001, weight_decay=0.001)
 
-# Optimizer
-optim = torch.optim.Adam(trainer.xavier_init(model), lr=0.0001984, weight_decay=0.001)
+trainer = TorchTrainer(is_gpu=True, epoch=50, optimizer=optim, model=model, criterion=criterion)
 
+'''
+        kwargs: model_save_path -> m_p, warmup_epoch(option) -> w_e, lr_milestones and gamma(option) -> l_m, best_metric(eg: r2) -> b_m
+'''
+config = {
+    'b_m': 0.8,
+    'm_p': 'D:\\Resource\\MDN\\PackageTest\\savedModel\\',
+    'w_e': 5,
+    'l_m': {
+        's_l': [20, 40],
+        'gamma': 0.7
+    }
+}
 # Training
-t_l, v_l, val_r2, train_r2, mse = trainer.fit_for_MDN(t_loader, v_loader, criterion, model=model, mixture=pdf,
-                                                      model_save_path='D:\\Resource\\MDN\\', optim=optim, best_r2=0.5)
+result = trainer.fit(t_loader, v_loader, **config)
+
+
 # Plot line chart
 result_pd = pd.DataFrame()
-result_pd['epoch'] = range(150)
-result_pd['train_r2_avg'] = train_r2
-result_pd['val_r2_avg'] = val_r2
+result_pd['epoch'] = len(result[0])
+result_pd['train_r2_avg'] = result[4]
+result_pd['val_r2_avg'] = result[3]
 
-trainer.plot_line_2(y_1='train_r2_avg', y_2='val_r2_avg', df=result_pd, fig_size=(10, 6), output_path="your save path", dpi=300)
+plot_line_2(y_1='train_r2_avg', y_2='val_r2_avg', df=result_pd, fig_size=(10, 6), output_path=".\\imgs\\GasGiants_MDN20240116_TrainValR2_2.png", dpi=300)
 ```
 ## Functions
 This package just support MDN for now, but the ```load_data``` is suitable for every condition as long as the type of data is Dataframe
 
 - tortreinador.train.TorchTrainer():
    + Parameters:
      + batch_size: int = 512
@@ -138,26 +146,28 @@
          + model: Any,
          + pdf: Any,
          + x: Any,
          + y: Any,
          + criterion: Any,
          + t: str = 'train'
        ```python
-         def _calculate(self, model, pdf, x, y, criterion, t='train'):
-             pi, mu, sigma = model(x)
+       # Please call self._standard_return() at the end
+       def calculate(self, x, y, mode='t'):
+
+            pi, mu, sigma = self.model(x)
 
-             mixture = pdf(pi, mu, sigma)
+            loss = self.criterion(pi, mu, sigma, y)
 
-             y_pred = mixture.sample()
+            pdf = mixture(pi, mu, sigma)
 
-             if t == 'train':
-               return criterion(pi, mu, sigma, y), y_pred.cpu().numpy(), y.cpu().numpy()
+            y_pred = pdf.sample()
 
-             else:
-               return criterion(pi, mu, sigma, y), self.mse(y_pred, y), y_pred.cpu().numpy(), y.cpu().numpy()
+            metric_per = r2_score(y, y_pred)
+            
+            return self._standard_return(loss, metric_per, mode, y, y_pred)
          ```
      + fit_for_MDN()
        + Describe: ***Train loop for MDN(Mixture Density Network)*** 
        + Parameters:
          + t_l: Dataloader
          + v_l: Dataloader
          + criterion: Module
```

### Comparing `tortreinador-0.0.6/tortreinador.egg-info/SOURCES.txt` & `tortreinador-0.0.7/tortreinador.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -14,8 +14,9 @@
 tortreinador/models/__init__.py
 tortreinador/utils/Recorder.py
 tortreinador/utils/View.py
 tortreinador/utils/WarmUpLR.py
 tortreinador/utils/__init__.py
 tortreinador/utils/metrics.py
 tortreinador/utils/plot.py
-tortreinador/utils/preprocessing.py
+tortreinador/utils/preprocessing.py
+tortreinador/utils/tools.py
```

