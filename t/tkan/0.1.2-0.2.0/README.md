# Comparing `tmp/tkan-0.1.2.tar.gz` & `tmp/tkan-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkan-0.1.2.tar", max compression
+gzip compressed data, was "tkan-0.2.0.tar", max compression
```

## Comparing `tkan-0.1.2.tar` & `tkan-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2303 2024-05-13 19:32:19.328997 tkan-0.1.2/README.md
--rw-r--r--   0        0        0      370 2024-05-13 21:03:00.988072 tkan-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      115 2024-05-09 15:54:41.624393 tkan-0.1.2/tkan/__init__.py
--rw-r--r--   0        0        0    11439 2024-05-09 15:49:06.996207 tkan-0.1.2/tkan/spline.py
--rw-r--r--   0        0        0    11040 2024-05-13 21:02:56.088030 tkan-0.1.2/tkan/tkan.py
--rw-r--r--   0        0        0     2740 1970-01-01 00:00:00.000000 tkan-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2458 2024-05-15 13:14:09.075662 tkan-0.2.0/README.md
+-rw-r--r--   0        0        0      457 2024-05-14 21:53:45.791069 tkan-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      115 2024-05-09 15:54:41.624393 tkan-0.2.0/tkan/__init__.py
+-rw-r--r--   0        0        0    11768 2024-05-15 09:25:46.027355 tkan-0.2.0/tkan/spline.py
+-rw-r--r--   0        0        0    27712 2024-05-14 18:37:43.241551 tkan-0.2.0/tkan/tkan.py
+-rw-r--r--   0        0        0     2895 1970-01-01 00:00:00.000000 tkan-0.2.0/PKG-INFO
```

### Comparing `tkan-0.1.2/tkan/spline.py` & `tkan-0.2.0/tkan/spline.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,14 +57,18 @@
         """
         config = super(FixedSplineActivation, self).get_config()
         config.update({
             'exponent': self.exponent.numpy(),  # Convert to native Python type for serialization
             'max_exponent': self.max_exponent.numpy(),
         })
         return config
+        
+    @classmethod
+    def from_config(cls, config):
+        return cls(**config)
 
 @tf.keras.utils.register_keras_serializable(package='tkan', name='PowerSplineActivation')
 class PowerSplineActivation(Layer):
     """
     A custom Keras Layer implementing a power spline activation function with trainable exponent and bias.
     The activation function transforms the input values using a power law modification, where the exponent can be
     adjusted during training.
@@ -145,14 +149,17 @@
             'initial_exponent': self.initial_exponent.numpy(),
             'epsilon': self.epsilon,
             'max_exponent': self.max_exponent.numpy(),
             'trainable': self.trainable,
         })
         return config
 
+    @classmethod
+    def from_config(cls, config):
+        return cls(**config)
 
 @tf.keras.utils.register_keras_serializable(package='tkan', name='LinspaceInitializer')
 class LinspaceInitializer(tf.keras.initializers.Initializer):
     """
     A custom TensorFlow initializer that generates values linearly spaced between a specified start and stop value.
     """
     def __init__(self, start: float, stop: float, num: int):
@@ -191,14 +198,17 @@
         Returns the configuration of the initializer.
 
         Returns:
             dict: Configuration dictionary.
         """
         return {'start': self.start, 'stop': self.stop, 'num': self.num}
 
+    @classmethod
+    def from_config(cls, config):
+        return cls(**config)
 
 @tf.keras.utils.register_keras_serializable(package='tkan', name='BSplineActivation')
 class BSplineActivation(Layer):
     """
     A custom Keras Layer implementing a B-Spline activation function with trainable coefficients,
     coupled with a SiLU activation for hybrid functionality.
     """
@@ -273,7 +283,11 @@
 
         Returns:
             dict: Configuration dictionary containing settings for number of bases and spline order.
         """
         config = super(BSplineActivation, self).get_config()
         config.update({"num_bases": self.num_bases, "order": self.order})
         return config
+
+    @classmethod
+    def from_config(cls, config):
+        return cls(**config)
```

### Comparing `tkan-0.1.2/PKG-INFO` & `tkan-0.2.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,50 +1,54 @@
 Metadata-Version: 2.1
 Name: tkan
-Version: 0.1.2
+Version: 0.2.0
 Summary: Temporal KAN model
 Author: Rémi Genet
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy (>=1.2,<2)
 Requires-Dist: tensorflow (>=2.8,<3)
 Description-Content-Type: text/markdown
 
 # TKAN: Temporal Kolmogorov-Arnold Networks
 
-TKAN (Temporal Kolmogorov-Arnold Networks) is a neural network architecture designed to enhance multi-horizon time series forecasting. This TensorFlow implementation integrates TKAN as a layer within sequential models, facilitating the use of advanced neural network techniques in practical applications. It is the original implementation of the [paper](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4824002)
+TKAN (Temporal Kolmogorov-Arnold Networks) is a neural network architecture designed to enhance multi-horizon time series forecasting. This TensorFlow implementation integrates TKAN as a layer within sequential models, facilitating the use of advanced neural network techniques in practical applications. It is the original implementation of the [paper](https://arxiv.org/abs/2405.07344)
+
+![TKAN representation](image/TKAN.drawio.png)
 
 ## Installation
 
 Install TKAN directly from PyPI:
 
 ```bash
 pip install tkan
 ```
 
 Dependencies are managed using pyproject.toml.
 
 ## Usage
 
-TKAN can be used within TensorFlow models to handle complex sequential patterns in data. Here is an example that demonstrates how to use TKAN with B-spline activations in a sequential model:
+TKAN can be used within TensorFlow models to handle complex sequential patterns in data.
+It's implementation reproduce architecture of RNN in tensorflow with Cell class and Layer that inherits from RNN in order to provide a perfect integrations with tensorflow.
+Here is an example that demonstrates how to use TKAN with B-spline activations in a sequential model:
 
 ```python
 from temporal_kan import TKAN, BSplineActivation
 import tensorflow as tf
 
 # Example model using TKAN with B-spline activations
 model = tf.keras.Sequential([
-    tf.keras.layers.InputLayer(input_shape=X_train.shape[1:]),
-    TKAN(activation_funcs=[BSplineActivation(i) for i in range(5)], num_outputs=100, return_sequences=True),
-    TKAN(activation_funcs=[BSplineActivation(i) for i in range(1, 4)], num_outputs=100, return_sequences=False),
-    tf.keras.layers.Dense(y_train.shape[1], activation='linear')
-], name=f'Sequential_Bspline')
+      tf.keras.layers.InputLayer(input_shape=X_train_seq.shape[1:]),
+      TKAN(100, tkan_activations=[BSplineActivation(3)], return_sequences=True, use_bias=True),
+      TKAN(100, tkan_activations=[BSplineActivation(3)], return_sequences=False, use_bias=True),
+      tf.keras.layers.Dense(y_train_seq.shape[1], activation=signed_softmax),
+])
 ```
 
 ### Activation Function Flexibility
 
 TKAN layers are highly flexible with regards to activation functions. They can be configured using various types of activations:
 - *Callable classes*: Custom classes like BSplineActivation allow for sophisticated configurations.
 - *Integers or floats*: Specify an initial exponent for a simple power spline activation.
```

