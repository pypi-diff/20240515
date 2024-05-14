# Comparing `tmp/CausalEGM-0.3.3.tar.gz` & `tmp/CausalEGM-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/CausalEGM-0.3.3.tar", last modified: Tue Mar 14 07:53:24 2023, max compression
+gzip compressed data, was "dist/CausalEGM-0.4.0.tar", last modified: Tue May 14 22:14:47 2024, max compression
```

## Comparing `CausalEGM-0.3.3.tar` & `CausalEGM-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrws---   0 liuqiao  (363861) oak_whwong (1005771)        0 2023-03-14 07:53:24.000000 CausalEGM-0.3.3/
-drwxrws---   0 liuqiao  (363861) oak_whwong (1005771)        0 2023-03-14 07:53:24.000000 CausalEGM-0.3.3/CausalEGM/
--rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)      213 2023-03-14 07:43:56.000000 CausalEGM-0.3.3/CausalEGM/__init__.py
--rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)       69 2022-12-14 18:32:13.000000 CausalEGM-0.3.3/CausalEGM/__main__.py
--rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)    38069 2023-03-14 07:40:29.000000 CausalEGM-0.3.3/CausalEGM/causalEGM.py
--rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)     4983 2023-02-10 20:13:55.000000 CausalEGM-0.3.3/CausalEGM/cli.py
--rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)     3883 2023-01-20 02:32:21.000000 CausalEGM-0.3.3/CausalEGM/model.py
--rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)    13579 2023-03-10 03:57:47.000000 CausalEGM-0.3.3/CausalEGM/util.py
-drwxrws---   0 liuqiao  (363861) oak_whwong (1005771)        0 2023-03-14 07:53:24.000000 CausalEGM-0.3.3/CausalEGM.egg-info/
--rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)     2016 2023-03-14 07:53:22.000000 CausalEGM-0.3.3/CausalEGM.egg-info/PKG-INFO
--rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)      337 2023-03-14 07:53:22.000000 CausalEGM-0.3.3/CausalEGM.egg-info/SOURCES.txt
--rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)        1 2023-03-14 07:53:22.000000 CausalEGM-0.3.3/CausalEGM.egg-info/dependency_links.txt
--rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)       49 2023-03-14 07:53:22.000000 CausalEGM-0.3.3/CausalEGM.egg-info/entry_points.txt
--rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)       54 2023-03-14 07:53:22.000000 CausalEGM-0.3.3/CausalEGM.egg-info/requires.txt
--rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)       10 2023-03-14 07:53:22.000000 CausalEGM-0.3.3/CausalEGM.egg-info/top_level.txt
--rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)     1068 2022-10-05 07:52:35.000000 CausalEGM-0.3.3/LICENSE
--rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)     2016 2023-03-14 07:53:24.000000 CausalEGM-0.3.3/PKG-INFO
--rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)       38 2023-03-14 07:53:24.000000 CausalEGM-0.3.3/setup.cfg
--rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)     2350 2023-03-14 07:43:43.000000 CausalEGM-0.3.3/setup.py
+drwxrws---   0 liuqiao  (363861) oak_whwong (1005771)        0 2024-05-14 22:14:47.000000 CausalEGM-0.4.0/
+drwxrws---   0 liuqiao  (363861) oak_whwong (1005771)        0 2024-05-14 22:14:45.000000 CausalEGM-0.4.0/CausalEGM/
+-rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)      213 2024-05-14 22:12:12.000000 CausalEGM-0.4.0/CausalEGM/__init__.py
+-rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)       69 2022-12-14 18:32:13.000000 CausalEGM-0.4.0/CausalEGM/__main__.py
+-rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)    37754 2024-05-14 06:00:43.000000 CausalEGM-0.4.0/CausalEGM/causalEGM.py
+-rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)     5162 2024-05-14 22:12:39.000000 CausalEGM-0.4.0/CausalEGM/cli.py
+-rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)     3883 2023-01-20 02:32:21.000000 CausalEGM-0.4.0/CausalEGM/model.py
+-rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)    13579 2023-03-10 03:57:47.000000 CausalEGM-0.4.0/CausalEGM/util.py
+drwxrws---   0 liuqiao  (363861) oak_whwong (1005771)        0 2024-05-14 22:14:47.000000 CausalEGM-0.4.0/CausalEGM.egg-info/
+-rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)     1891 2024-05-14 22:14:44.000000 CausalEGM-0.4.0/CausalEGM.egg-info/PKG-INFO
+-rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)      337 2024-05-14 22:14:45.000000 CausalEGM-0.4.0/CausalEGM.egg-info/SOURCES.txt
+-rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)        1 2024-05-14 22:14:44.000000 CausalEGM-0.4.0/CausalEGM.egg-info/dependency_links.txt
+-rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)       49 2024-05-14 22:14:44.000000 CausalEGM-0.4.0/CausalEGM.egg-info/entry_points.txt
+-rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)       54 2024-05-14 22:14:44.000000 CausalEGM-0.4.0/CausalEGM.egg-info/requires.txt
+-rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)       10 2024-05-14 22:14:44.000000 CausalEGM-0.4.0/CausalEGM.egg-info/top_level.txt
+-rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)     1068 2022-10-05 07:52:35.000000 CausalEGM-0.4.0/LICENSE
+-rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)     1891 2024-05-14 22:14:47.000000 CausalEGM-0.4.0/PKG-INFO
+-rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)       38 2024-05-14 22:14:47.000000 CausalEGM-0.4.0/setup.cfg
+-rw-rw----   0 liuqiao  (363861) oak_whwong (1005771)     2225 2024-05-14 22:12:49.000000 CausalEGM-0.4.0/setup.py
```

### Comparing `CausalEGM-0.3.3/CausalEGM/causalEGM.py` & `CausalEGM-0.4.0/CausalEGM/causalEGM.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,17 +40,17 @@
         self.e_net = BaseFullyConnectedNet(input_dim=params['v_dim'],output_dim = sum(params['z_dims']), 
                                         model_name='e_net', nb_units=params['e_units'])
         self.dz_net = Discriminator(input_dim=sum(params['z_dims']),model_name='dz_net',
                                         nb_units=params['dz_units'])
         self.dv_net = Discriminator(input_dim=params['v_dim'],model_name='dv_net',
                                         nb_units=params['dv_units'])
 
-        self.f_net = BaseFullyConnectedNet(input_dim=1+params['z_dims'][0]+params['z_dims'][2],
+        self.f_net = BaseFullyConnectedNet(input_dim=1+params['z_dims'][0]+params['z_dims'][1],
                                         output_dim = 1, model_name='f_net', nb_units=params['f_units'])
-        self.h_net = BaseFullyConnectedNet(input_dim=params['z_dims'][0]+params['z_dims'][1],
+        self.h_net = BaseFullyConnectedNet(input_dim=params['z_dims'][0]+params['z_dims'][2],
                                         output_dim = 1, model_name='h_net', nb_units=params['h_units'])
 
         self.g_e_optimizer = tf.keras.optimizers.Adam(params['lr'], beta_1=0.5, beta_2=0.9)
         self.d_optimizer = tf.keras.optimizers.Adam(params['lr'], beta_1=0.5, beta_2=0.9)
         self.z_sampler = Gaussian_sampler(mean=np.zeros(sum(params['z_dims'])), sd=1.0)
 
         self.initialize_nets()
@@ -94,16 +94,16 @@
     def initialize_nets(self, print_summary = False):
         """Initialize all the networks in CausalEGM."""
 
         self.g_net(np.zeros((1, sum(self.params['z_dims']))))
         self.e_net(np.zeros((1, self.params['v_dim'])))
         self.dz_net(np.zeros((1, sum(self.params['z_dims']))))
         self.dv_net(np.zeros((1, self.params['v_dim'])))
-        self.f_net(np.zeros((1, 1+self.params['z_dims'][0]+self.params['z_dims'][2])))
-        self.h_net(np.zeros((1, self.params['z_dims'][0]+self.params['z_dims'][1])))
+        self.f_net(np.zeros((1, 1+self.params['z_dims'][0]+self.params['z_dims'][1])))
+        self.h_net(np.zeros((1, self.params['z_dims'][0]+self.params['z_dims'][2])))
         if print_summary:
             print(self.g_net.summary())
             print(self.h_net.summary())
             print(self.dz_net.summary())
             print(self.f_net.summary())    
             print(self.h_net.summary()) 
 
@@ -157,16 +157,16 @@
             
             l2_loss_v = tf.reduce_mean((data_v - data_v__)**2)
             l2_loss_z = tf.reduce_mean((data_z - data_z__)**2)
             
             g_loss_adv = -tf.reduce_mean(data_dv_)
             e_loss_adv = -tf.reduce_mean(data_dz_)
 
-            data_y_ = self.f_net(tf.concat([data_z0, data_z2, data_x], axis=-1))
-            data_x_ = self.h_net(tf.concat([data_z0, data_z1], axis=-1))
+            data_y_ = self.f_net(tf.concat([data_z0, data_z1, data_x], axis=-1))
+            data_x_ = self.h_net(tf.concat([data_z0, data_z2], axis=-1))
             if self.params['binary_treatment']:
                 data_x_ = tf.sigmoid(data_x_)
             l2_loss_x = tf.reduce_mean((data_x_ - data_x)**2)
             l2_loss_y = tf.reduce_mean((data_y_ - data_y)**2)
             g_e_loss = self.params['use_v_gan']*g_loss_adv+e_loss_adv+self.params['alpha']*(l2_loss_v + self.params['use_z_rec']*l2_loss_z) \
                         + self.params['beta']*(l2_loss_x+l2_loss_y)
 
@@ -200,35 +200,40 @@
             Float denoting combined discrinimator(s) loss.
         """ 
         epsilon_z = tf.random.uniform([],minval=0., maxval=1.)
         epsilon_v = tf.random.uniform([],minval=0., maxval=1.)
         with tf.GradientTape(persistent=True) as disc_tape:
             data_v_ = self.g_net(data_z)
             data_z_ = self.e_net(data_v)
+            data_z_hat = data_z*epsilon_z + data_z_*(1-epsilon_z)
+            data_v_hat = data_v*epsilon_v + data_v_*(1-epsilon_v)
             
+            with tf.GradientTape() as gp_tape_z:
+                gp_tape_z.watch(data_z_hat)
+                data_dz_hat = self.dz_net(data_z_hat)
+            with tf.GradientTape() as gp_tape_v:
+                gp_tape_v.watch(data_v_hat)
+                data_dv_hat = self.dv_net(data_v_hat)
+                
             data_dv_ = self.dv_net(data_v_)
             data_dz_ = self.dz_net(data_z_)
             
             data_dv = self.dv_net(data_v)
             data_dz = self.dz_net(data_z)
             
             dz_loss = -tf.reduce_mean(data_dz) + tf.reduce_mean(data_dz_)
             dv_loss = -tf.reduce_mean(data_dv) + tf.reduce_mean(data_dv_)
             
             #gradient penalty for z
-            data_z_hat = data_z*epsilon_z + data_z_*(1-epsilon_z)
-            data_dz_hat = self.dz_net(data_z_hat)
-            grad_z = tf.gradients(data_dz_hat, data_z_hat)[0] #(bs,z_dim)
+            grad_z = gp_tape_z.gradient(data_dz_hat, data_z_hat) #(bs,z_dim)
             grad_norm_z = tf.sqrt(tf.reduce_sum(tf.square(grad_z), axis=1))#(bs,) 
             gpz_loss = tf.reduce_mean(tf.square(grad_norm_z - 1.0))
             
             #gradient penalty for v
-            data_v_hat = data_v*epsilon_v + data_v_*(1-epsilon_v)
-            data_dv_hat = self.dv_net(data_v_hat)
-            grad_v = tf.gradients(data_dv_hat, data_v_hat)[0] #(bs,v_dim)
+            grad_v = gp_tape_v.gradient(data_dv_hat, data_v_hat) #(bs,v_dim)
             grad_norm_v = tf.sqrt(tf.reduce_sum(tf.square(grad_v), axis=1))#(bs,) 
             gpv_loss = tf.reduce_mean(tf.square(grad_norm_v - 1.0))
             
             d_loss = self.params['use_v_gan']*dv_loss + dz_loss + \
                     self.params['gamma']*(gpz_loss + self.params['use_v_gan']*gpv_loss)
 
         # Calculate the gradients for generators and discriminators
@@ -266,16 +271,16 @@
             Int object denoting the number of iterations per save. Default: ``10000``.
         startoff
             Int object denoting the beginning iterations to jump without save and evaluation. Defalt: ``0``.
         verbose
             Bool object denoting whether showing the progress bar. Default: ``False``.
         save_format
             Str object denoting the format (csv, txt, npz) to save the results. Default: ``txt``.
-        
         """
+        
         if self.params['save_res']:
             f_params = open('{}/params.txt'.format(self.save_dir),'w')
             f_params.write(str(self.params))
             f_params.close()
         if data is None and data_file is None:
             self.data_sampler = Dataset_selector(self.params['dataset'])(batch_size=batch_size)
         elif data is not None:
@@ -312,21 +317,21 @@
                     best_loss = mse_y
                     self.best_causal_pre = causal_pre
                     self.best_batch_idx = batch_idx
                     if self.params['save_model']:
                         ckpt_save_path = self.ckpt_manager.save(batch_idx)
                         #print('Saving checkpoint for iteration {} at {}'.format(batch_idx, ckpt_save_path))
                 if self.params['save_res'] and batch_idx > 0 and batch_idx % batches_per_save == 0:
-                    self.save('{}/causal_pre_at_{}.{}'.format(self.save_dir, batch_idx, save_format), self.best_causal_pre)
+                    self.save('{}/causal_pre_at_{}.{}'.format(self.save_dir, batch_idx, save_format), causal_pre)
         if self.params['save_res']:
             self.save('{}/causal_pre_final.{}'.format(self.save_dir,save_format), self.best_causal_pre)
 
         if self.params['binary_treatment']:
             self.ATE = np.mean(self.best_causal_pre)
-            print('The average treatment effect (ATE) is ', self.ATE)
+            print('The average treatment effect (ATE) is', self.ATE)
 
     def evaluate(self, data, nb_intervals=200):
         """Internal evaluation in the training process of CausalEGM.
 
         Parameters
         ----------
         data
@@ -341,37 +346,36 @@
             values of average dose response function (ADRF).
         mse_x
             Float denoting treatment reconstruction loss.
         mse_y
             Float denoting outcome reconstruction loss.
         """ 
         data_x, data_y, data_v = data
-        data_z = self.z_sampler.get_batch(len(data_x))
         data_z_ = self.e_net.predict(data_v,verbose=0)
         data_z0 = data_z_[:,:self.params['z_dims'][0]]
         data_z1 = data_z_[:,self.params['z_dims'][0]:sum(self.params['z_dims'][:2])]
         data_z2 = data_z_[:,sum(self.params['z_dims'][:2]):sum(self.params['z_dims'][:3])]
-        data_y_pred = self.f_net.predict(tf.concat([data_z0, data_z2, data_x], axis=-1),verbose=0)
-        data_x_pred = self.h_net.predict(tf.concat([data_z0, data_z1], axis=-1),verbose=0)
+        data_y_pred = self.f_net.predict(tf.concat([data_z0, data_z1, data_x], axis=-1),verbose=0)
+        data_x_pred = self.h_net.predict(tf.concat([data_z0, data_z2], axis=-1),verbose=0)
         if self.params['binary_treatment']:
             data_x_pred = tf.sigmoid(data_x_pred)
         mse_x = np.mean((data_x-data_x_pred)**2)
         mse_y = np.mean((data_y-data_y_pred)**2)
         if self.params['binary_treatment']:
             #individual treatment effect (ITE) && average treatment effect (ATE)
-            y_pred_pos = self.f_net.predict(tf.concat([data_z0, data_z2, np.ones((len(data_x),1))], axis=-1),verbose=0)
-            y_pred_neg = self.f_net.predict(tf.concat([data_z0, data_z2, np.zeros((len(data_x),1))], axis=-1),verbose=0)
+            y_pred_pos = self.f_net.predict(tf.concat([data_z0, data_z1, np.ones((len(data_x),1))], axis=-1),verbose=0)
+            y_pred_neg = self.f_net.predict(tf.concat([data_z0, data_z1, np.zeros((len(data_x),1))], axis=-1),verbose=0)
             ite_pre = y_pred_pos-y_pred_neg
             return ite_pre, mse_x, mse_y
         else:
             #average dose response function (ADRF)
             dose_response = []
             for x in np.linspace(self.params['x_min'], self.params['x_max'], nb_intervals):
                 data_x = np.tile(x, (len(data_x), 1))
-                y_pred = self.f_net.predict(tf.concat([data_z0, data_z2, data_x], axis=-1),verbose=0)
+                y_pred = self.f_net.predict(tf.concat([data_z0, data_z1, data_x], axis=-1),verbose=0)
                 dose_response.append(np.mean(y_pred))
             return np.array(dose_response), mse_x, mse_y
         
     def predict(self, data_x, data_v):
         """Predict the outcome given treatment and covariates in CausalEGM.
 
         Parameters
@@ -385,20 +389,18 @@
         -------
         causal_pre
             Numpy.ndarray denoting the predicted potential outcome with shape [nb_sample, ].
         """ 
         assert len(data_x) == len(data_v)
         if len(data_x.shape)==1:
             data_x = data_x.reshape(-1,1)
-        data_z = self.z_sampler.get_batch(len(data_x))
         data_z_ = self.e_net.predict(data_v,verbose=0)
         data_z0 = data_z_[:,:self.params['z_dims'][0]]
         data_z1 = data_z_[:,self.params['z_dims'][0]:sum(self.params['z_dims'][:2])]
-        data_z2 = data_z_[:,sum(self.params['z_dims'][:2]):sum(self.params['z_dims'][:3])]
-        data_y_pred = self.f_net.predict(tf.concat([data_z0, data_z2, data_x], axis=-1),verbose=0)
+        data_y_pred = self.f_net.predict(tf.concat([data_z0, data_z1, data_x], axis=-1),verbose=0)
         return np.squeeze(data_y_pred)
     
     def getADRF(self, x_list, data_v=None):
         """Get average dosage response function (ADRF) in CausalEGM.
 
         Parameters
         ----------
@@ -411,24 +413,22 @@
         Returns
         -------
         causal_pre
             Numpy.ndarray denoting the predicted ADRF values with shape [nb_sample, ].
         """ 
         if data_v is None:
             data_v = self.data_sampler.load_all()[-1]
-        data_z = self.z_sampler.get_batch(len(data_v))
         data_z_ = self.e_net.predict(data_v,verbose=0)
         data_z0 = data_z_[:,:self.params['z_dims'][0]]
         data_z1 = data_z_[:,self.params['z_dims'][0]:sum(self.params['z_dims'][:2])]
-        data_z2 = data_z_[:,sum(self.params['z_dims'][:2]):sum(self.params['z_dims'][:3])]
         if not self.params['binary_treatment']:
             dose_response = []
             for x in x_list:
                 data_x = np.tile(x, (len(data_v), 1))
-                y_pred = self.f_net.predict(tf.concat([data_z0, data_z2, data_x], axis=-1),verbose=0)
+                y_pred = self.f_net.predict(tf.concat([data_z0, data_z1, data_x], axis=-1),verbose=0)
                 dose_response.append(np.mean(y_pred))
             return np.array(dose_response)
         else:
             print('ADRF is only applicable in continuous treatment setting!')
             sys.exit()
     
     def getCATE(self,data_v):
@@ -442,22 +442,21 @@
 
         Returns
         -------
         cate_pre
             Numpy.ndarray (1-D) denoting the predicted CATE values with shape [nb_sample, ].
         """ 
         assert data_v.shape[1] == self.params['v_dim']
-        data_z = self.z_sampler.get_batch(len(data_v))
         data_z_ = self.e_net.predict(data_v,verbose=0)
         data_z0 = data_z_[:,:self.params['z_dims'][0]]
         data_z1 = data_z_[:,self.params['z_dims'][0]:sum(self.params['z_dims'][:2])]
         data_z2 = data_z_[:,sum(self.params['z_dims'][:2]):sum(self.params['z_dims'][:3])]
         if self.params['binary_treatment']:
-            y_pred_pos = self.f_net.predict(tf.concat([data_z0, data_z2, np.ones((len(data_v),1))], axis=-1),verbose=0)
-            y_pred_neg = self.f_net.predict(tf.concat([data_z0, data_z2, np.zeros((len(data_v),1))], axis=-1),verbose=0)
+            y_pred_pos = self.f_net.predict(tf.concat([data_z0, data_z1, np.ones((len(data_v),1))], axis=-1),verbose=0)
+            y_pred_neg = self.f_net.predict(tf.concat([data_z0, data_z1, np.zeros((len(data_v),1))], axis=-1),verbose=0)
             cate_pre = y_pred_pos-y_pred_neg
             return np.squeeze(cate_pre)
         else:
             print('CATE is only applicable in binary treatment setting!')
             sys.exit()
     
 
@@ -504,17 +503,17 @@
             tf.keras.utils.set_random_seed(random_seed)
             os.environ['TF_DETERMINISTIC_OPS'] = '1'
         self.g_net = BaseFullyConnectedNet(input_dim=sum(params['z_dims']),output_dim = params['v_dim'], 
                                         model_name='g_net', nb_units=params['g_units'])
         self.e_net = BaseFullyConnectedNet(input_dim=params['v_dim'],output_dim = 2*sum(params['z_dims']), 
                                         model_name='e_net', nb_units=params['e_units'])
 
-        self.f_net = BaseFullyConnectedNet(input_dim=1+params['z_dims'][0]+params['z_dims'][2],
+        self.f_net = BaseFullyConnectedNet(input_dim=1+params['z_dims'][0]+params['z_dims'][1],
                                         output_dim = 1, model_name='f_net', nb_units=params['f_units'])
-        self.h_net = BaseFullyConnectedNet(input_dim=params['z_dims'][0]+params['z_dims'][1],
+        self.h_net = BaseFullyConnectedNet(input_dim=params['z_dims'][0]+params['z_dims'][2],
                                         output_dim = 1, model_name='h_net', nb_units=params['h_units'])
 
         self.g_e_optimizer = tf.keras.optimizers.Adam(params['lr'], beta_1=0.5, beta_2=0.9)
         self.d_optimizer = tf.keras.optimizers.Adam(params['lr'], beta_1=0.5, beta_2=0.9)
         self.z_sampler = Gaussian_sampler(mean=np.zeros(sum(params['z_dims'])), sd=1.0)
 
         self.initialize_nets()
@@ -554,16 +553,16 @@
         }
     
     def initialize_nets(self, print_summary = False):
         """Initialize all the networks in CausalEGM."""
 
         self.g_net(np.zeros((1, sum(self.params['z_dims']))))
         self.e_net(np.zeros((1, self.params['v_dim'])))
-        self.f_net(np.zeros((1, 1+self.params['z_dims'][0]+self.params['z_dims'][2])))
-        self.h_net(np.zeros((1, self.params['z_dims'][0]+self.params['z_dims'][1])))
+        self.f_net(np.zeros((1, 1+self.params['z_dims'][0]+self.params['z_dims'][1])))
+        self.h_net(np.zeros((1, self.params['z_dims'][0]+self.params['z_dims'][2])))
         if print_summary:
             print(self.g_net.summary())
             print(self.h_net.summary())
             print(self.f_net.summary())    
             print(self.h_net.summary()) 
 
     @tf.function
@@ -608,18 +607,17 @@
             logpz = self.log_normal_pdf(data_z_, 0., 0.)
             kl_loss = logqz_v-logpz # here it is not the formula of KL_loss, so will result in negative values
             elbo = tf.reduce_mean(logpv_z - kl_loss)
             
             data_z0 = data_z_[:,:self.params['z_dims'][0]]
             data_z1 = data_z_[:,self.params['z_dims'][0]:sum(self.params['z_dims'][:2])]
             data_z2 = data_z_[:,sum(self.params['z_dims'][:2]):sum(self.params['z_dims'][:3])]
-            data_z3 = data_z_[:-self.params['z_dims'][3]:]
 
-            data_y_ = self.f_net(tf.concat([data_z0, data_z2, data_x], axis=-1))
-            data_x_ = self.h_net(tf.concat([data_z0, data_z1], axis=-1))
+            data_y_ = self.f_net(tf.concat([data_z0, data_z1, data_x], axis=-1))
+            data_x_ = self.h_net(tf.concat([data_z0, data_z2], axis=-1))
             if self.params['binary_treatment']:
                 data_x_ = tf.sigmoid(data_x_)
             l2_loss_x = tf.reduce_mean((data_x_ - data_x)**2)
             l2_loss_y = tf.reduce_mean((data_y_ - data_y)**2)
             g_e_loss = -elbo + self.params['beta']*(l2_loss_x+l2_loss_y)
 
         # Calculate the gradients for generators and discriminators
@@ -631,15 +629,15 @@
                                             self.f_net.trainable_variables+self.h_net.trainable_variables))
         return tf.reduce_mean(logpv_z), tf.reduce_mean(kl_loss), elbo, l2_loss_x, l2_loss_y, g_e_loss
 
     @tf.function
     def sample(self, eps=None):
         """Generate data by decoder."""
         if eps is None:
-            eps = tf.random.normal(shape=(100, sum(params['z_dims'])))
+            eps = tf.random.normal(shape=(100, sum(self.params['z_dims'])))
         return self.g_net(eps)
 
     def encode(self, v):
         """Encode process and get both mean and variance."""
         mean, logvar = tf.split(self.e_net(v), num_or_size_splits=2, axis=1)
         return mean, logvar
 
@@ -720,15 +718,15 @@
                     best_loss = mse_y
                     self.best_causal_pre = causal_pre
                     self.best_batch_idx = batch_idx
                     if self.params['save_model']:
                         ckpt_save_path = self.ckpt_manager.save(batch_idx)
                         #print('Saving checkpoint for iteration {} at {}'.format(batch_idx, ckpt_save_path))
                 if self.params['save_res'] and batch_idx > 0 and batch_idx % batches_per_save == 0:
-                    self.save('{}/causal_pre_at_{}.{}'.format(self.save_dir, batch_idx, save_format), self.best_causal_pre)
+                    self.save('{}/causal_pre_at_{}.{}'.format(self.save_dir, batch_idx, save_format), causal_pre)
         if self.params['save_res']:
             self.save('{}/causal_pre_final.{}'.format(self.save_dir,save_format), self.best_causal_pre)
         if self.params['binary_treatment']:
             self.ATE = np.mean(self.best_causal_pre)
             print('The average treatment effect (ATE) is ', self.ATE)
 
     def evaluate(self, data, nb_intervals=200):
@@ -748,38 +746,37 @@
             values of average dose response function (ADRF).
         mse_x
             Float denoting treatment reconstruction loss.
         mse_y
             Float denoting outcome reconstruction loss.
         """ 
         data_x, data_y, data_v = data
-        data_z = self.z_sampler.get_batch(len(data_x))
         mean, logvar = self.encode(data_v)
         data_z_ = self.reparameterize(mean, logvar)
         data_z0 = data_z_[:,:self.params['z_dims'][0]]
         data_z1 = data_z_[:,self.params['z_dims'][0]:sum(self.params['z_dims'][:2])]
         data_z2 = data_z_[:,sum(self.params['z_dims'][:2]):sum(self.params['z_dims'][:3])]
-        data_y_pred = self.f_net.predict(tf.concat([data_z0, data_z2, data_x], axis=-1),verbose=0)
-        data_x_pred = self.h_net.predict(tf.concat([data_z0, data_z1], axis=-1),verbose=0)
+        data_y_pred = self.f_net.predict(tf.concat([data_z0, data_z1, data_x], axis=-1),verbose=0)
+        data_x_pred = self.h_net.predict(tf.concat([data_z0, data_z2], axis=-1),verbose=0)
         if self.params['binary_treatment']:
             data_x_pred = tf.sigmoid(data_x_pred)
         mse_x = np.mean((data_x-data_x_pred)**2)
         mse_y = np.mean((data_y-data_y_pred)**2)
         if self.params['binary_treatment']:
             #individual treatment effect (ITE) && average treatment effect (ATE)
-            y_pred_pos = self.f_net.predict(tf.concat([data_z0, data_z2, np.ones((len(data_x),1))], axis=-1),verbose=0)
-            y_pred_neg = self.f_net.predict(tf.concat([data_z0, data_z2, np.zeros((len(data_x),1))], axis=-1),verbose=0)
+            y_pred_pos = self.f_net.predict(tf.concat([data_z0, data_z1, np.ones((len(data_x),1))], axis=-1),verbose=0)
+            y_pred_neg = self.f_net.predict(tf.concat([data_z0, data_z1, np.zeros((len(data_x),1))], axis=-1),verbose=0)
             ite_pre = y_pred_pos-y_pred_neg
             return ite_pre, mse_x, mse_y
         else:
             #average dose response function (ADRF)
             dose_response = []
             for x in np.linspace(self.params['x_min'], self.params['x_max'], nb_intervals):
                 data_x = np.tile(x, (len(data_x), 1))
-                y_pred = self.f_net.predict(tf.concat([data_z0, data_z2, data_x], axis=-1),verbose=0)
+                y_pred = self.f_net.predict(tf.concat([data_z0, data_z1, data_x], axis=-1),verbose=0)
                 dose_response.append(np.mean(y_pred))
             return np.array(dose_response), mse_x, mse_y
 
     def save(self, fname, data):
         """Save the data to the specified path."""
         if fname[-3:] == 'npy':
             np.save(fname, data)
```

### Comparing `CausalEGM-0.3.3/CausalEGM/cli.py` & `CausalEGM-0.4.0/CausalEGM/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,22 +16,22 @@
                         help="Dataset name")
     parser.add_argument('--save-model', default=True, action=argparse.BooleanOptionalAction,
                         help="whether to save model.")
     parser.add_argument('--binary-treatment', default=True, action=argparse.BooleanOptionalAction,
                         help="whether use binary treatment setting.")
 
     #model hypterparameters
-    parser.add_argument('-z_dims', dest='z_dims', type=int, nargs='+', default=[3,3,6,6],
+    parser.add_argument('-z_dims', dest='z_dims', type=int, nargs='+', default=[3,6,3,6],
                         help='Latent dimensions of the four encoder outputs e(V)_0~3.')
     parser.add_argument('-lr', dest='lr', type=float, default=0.0002,
                         help="Learning rate for the optimizer (default: 0.0002).")
     parser.add_argument('-alpha', dest='alpha', type=float, default=1.,
-                        help="Coefficient for reconstruction loss (default: 10).")
+                        help="Coefficient for reconstruction loss (default: 1).")
     parser.add_argument('-beta', dest='beta', type=float, default=1.,
-                        help="Coefficient for roundtrip loss (default: 10).")
+                        help="Coefficient for treatment and outcome MSE loss (default: 1).")
     parser.add_argument('-gamma', dest='gamma', type=float, default=10.,
                         help="Coefficient for gradient penalty loss (default: 10).")
     parser.add_argument('-g_d_freq', dest='g_d_freq', type=int, default=5,
                         help="Frequency for updating discriminators and generators (default: 5).")
     #network hyperparameters
     parser.add_argument('-g_units', dest='g_units', type=int, nargs='+', default=[64,64,64,64,64],
                         help='Number of units for generator/decoder network (default: [64,64,64,64,64]).')
@@ -56,21 +56,23 @@
                         help="Number of iterations (default: 30000).")
     parser.add_argument('-startoff', dest='startoff', type=int, default=0,
                         help="Iteration for starting evaluation (default: 0).")
     parser.add_argument('-batches_per_eval', dest='batches_per_eval', type=int, default=500,
                         help="Number of iterations per evaluation (default: 500).")
     parser.add_argument('-save_format', dest='save_format', type=str,default='txt',
                         help="Saving format (default: txt)")
+    parser.add_argument('--save_res', default=True, action=argparse.BooleanOptionalAction,
+                        help="Whether to save results during training.")
     #Random seed control
     parser.add_argument('-seed', dest='seed', type=int, default=123,
                         help="Random seed for reproduction (default: 123).")
     args = parser.parse_args()
     params = vars(args)
     data = parse_file(args.input)
     params['v_dim'] = data[-1].shape[1]
     model = CausalEGM(params,random_seed=args.seed)
     print('Start training...')
     model.train(data=data, batch_size=args.batch_size, n_iter=args.n_iter, batches_per_eval=args.batches_per_eval, 
                 startoff=args.startoff, save_format=args.save_format)
 
 if __name__ == "__main__":
-   main()
+    main()
```

### Comparing `CausalEGM-0.3.3/CausalEGM/model.py` & `CausalEGM-0.4.0/CausalEGM/model.py`

 * *Files identical despite different names*

### Comparing `CausalEGM-0.3.3/CausalEGM/util.py` & `CausalEGM-0.4.0/CausalEGM/util.py`

 * *Files identical despite different names*

### Comparing `CausalEGM-0.3.3/LICENSE` & `CausalEGM-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CausalEGM-0.3.3/setup.py` & `CausalEGM-0.4.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import setuptools
 
 setuptools.setup(
     name="CausalEGM", 
-    version="0.3.3",
+    version="0.4.0",
     author="Qiao Liu",
     author_email="liuqiao@stanford.edu",
-    description="CausalEGM: a general causal inference framework by encoding generative modeling",
-    long_description="Understanding and characterizing causal effect has become essential in observational studies while it is still challenging if the confounders are high-dimensional. In this article, we develop a general framework CausalEGM, for estimating causal effect by encoding generative modeling, which can be applied in both binary and continuous treatment settings. In the potential outcome framework with unconfoundedness, we build a bidirectional transformation between the high-dimensional confounders space and a low-dimensional latent space where the density is known (e.g., Gaussian). Through this, CausalEGM enables simultaneously decoupling the dependencies of confounders on both treatment and outcome, and mapping the confounders to the low-dimensional latent space. By conditioning on the low-dimensional latent features, CausalEGM is able to estimate the causal effect for each individual or estimate the average causal effect within a population. Our theoretical analysis shows that the excess risk for CausalEGM can be bounded through empirical process theory. Under an assumption on encoder-decoder networks, the consistency of the estimate can also be guaranteed. In a series of experiments, CausalEGM demonstrates superior performance against existing methods in both binary and continuous settings. Specifically, we find CausalEGM to be substantially more powerful than competing methods in the presence of large sample size and high dimensional confounders. CausalEGM is freely available at https://github.com/SUwonglab/CausalEGM.",
+    description="CausalEGM: an encoding generative modeling approach to dimension reduction and covariate adjustment in causal inference with observational studies",
+    long_description="In this article, we develop CausalEGM, a deep learning framework for nonlinear dimension reduction and generative modeling of the dependency among covariate features affecting treatment and response. CausalEGM can be used for estimating causal effects in both binary and continuous treatment settings. By learning a bidirectional transformation between the high-dimensional covariate space and a low-dimensional latent space and then modeling the dependencies of different subsets of the latent variables on the treatment and response, CausalEGM can extract the latent covariate features that affect both treatment and response. By conditioning on these features, one can mitigate the confounding effect of the high dimensional covariate on the estimation of the causal relation between treatment and response. In a series of experiments, the proposed method is shown to achieve superior performance over existing methods in both binary and continuous treatment settings. The improvement is substantial when the sample size is large and the covariate is of high dimension. Finally, we established excess risk bounds and consistency results for our method, and discuss how our approach is related to and improves upon other dimension reduction approaches in causal inference. CausalEGM is freely available at https://github.com/SUwonglab/CausalEGM.",
     long_description_content_type="text/markdown",
     url="https://github.com/SUwonglab/CausalEGM",
     packages=setuptools.find_packages(),
     install_requires=[
    'tensorflow>=2.8.0',
    'scikit-learn',
    'pandas',
```

