# Comparing `tmp/tokun-0.3.4.tar.gz` & `tmp/tokun-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokun-0.3.4.tar", max compression
+gzip compressed data, was "tokun-0.3.5.tar", max compression
```

## Comparing `tokun-0.3.4.tar` & `tokun-0.3.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     3777 2024-05-07 18:10:25.714470 tokun-0.3.4/.github/README.md
--rw-r--r--   0        0        0      456 2024-05-14 10:33:23.506310 tokun-0.3.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-04 12:49:41.836303 tokun-0.3.4/tokun/__init__.py
--rw-r--r--   0        0        0     4935 2024-05-14 09:58:07.313626 tokun-0.3.4/tokun/export.py
--rw-r--r--   0        0        0     5973 2024-05-14 09:58:32.170076 tokun-0.3.4/tokun/layers.py
--rw-r--r--   0        0        0      338 2024-05-14 10:02:24.638598 tokun-0.3.4/tokun/meta.py
--rw-r--r--   0        0        0     5403 2024-05-14 10:01:14.502286 tokun-0.3.4/tokun/model.py
--rw-r--r--   0        0        0     4416 2024-05-14 10:22:07.757130 tokun-0.3.4/tokun/pipeline.py
--rw-r--r--   0        0        0     4998 2024-05-14 10:00:29.565885 tokun-0.3.4/tokun/test.py
--rw-r--r--   0        0        0     4638 2024-05-14 09:58:55.776550 tokun-0.3.4/tokun/train.py
--rw-r--r--   0        0        0     4290 1970-01-01 00:00:00.000000 tokun-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     3777 2024-05-07 18:10:25.714470 tokun-0.3.5/.github/README.md
+-rw-r--r--   0        0        0      455 2024-05-15 12:36:35.310608 tokun-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-04 12:49:41.836303 tokun-0.3.5/tokun/__init__.py
+-rw-r--r--   0        0        0     4823 2024-05-15 09:55:48.930122 tokun-0.3.5/tokun/export.py
+-rw-r--r--   0        0        0     5973 2024-05-14 09:58:32.170076 tokun-0.3.5/tokun/layers.py
+-rw-r--r--   0        0        0      525 2024-05-14 13:01:51.377336 tokun-0.3.5/tokun/meta.py
+-rw-r--r--   0        0        0     5403 2024-05-14 10:01:14.502286 tokun-0.3.5/tokun/model.py
+-rw-r--r--   0        0        0     4938 2024-05-14 14:24:21.768802 tokun-0.3.5/tokun/pipeline.py
+-rw-r--r--   0        0        0     3644 2024-05-15 09:58:00.690031 tokun-0.3.5/tokun/test.py
+-rw-r--r--   0        0        0     5088 2024-05-14 14:10:26.351042 tokun-0.3.5/tokun/train.py
+-rw-r--r--   0        0        0     4289 1970-01-01 00:00:00.000000 tokun-0.3.5/PKG-INFO
```

### Comparing `tokun-0.3.4/.github/README.md` & `tokun-0.3.5/.github/README.md`

 * *Files identical despite different names*

### Comparing `tokun-0.3.4/tokun/export.py` & `tokun-0.3.5/tokun/export.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,81 +23,79 @@
 N_TOKEN_DIM = [4, 4, 4] # G, for each block
 
 N_BATCH = 128 # number of samples per batch
 N_SAMPLE = 128 # number of characters per sample (=> N_TOKEN_DIM * N_SAMPLE integers per sample)
 
 # DERIVED #####################################################################
 
-TOKEN_LENGTH = math.prod(N_TOKEN_DIM) # in bytes
-OFFSET_TICKS = [2 ** __i for __i in range(int(math.log(TOKEN_LENGTH // 4, 2)))] # in characters
+TOKEN_SIZES = list(itertools.accumulate(N_TOKEN_DIM, lambda x, y: x * y)) # in bytes
+OFFSET_TICKS = [2 ** __i for __i in range(int(math.log(TOKEN_SIZES[-1] // 4, 2)))] # in characters
 
-# LOG #########################################################################
+# IMPORT ######################################################################
 
 VERSION = tokun.meta.version(groups=N_TOKEN_DIM, attention=ATTENTION, normalization=NORMALIZATION)
-DATETIME = '20240509-211600'
+LABEL = '0.99996'
 
-PATH_MODEL = os.path.join('models/', *VERSION, DATETIME + '.keras')
+PATH_IMPORT = os.path.join('models/', *VERSION, '{}.keras'.format(LABEL))
+
+MODEL = keras.models.load_model(PATH_IMPORT)
 
 # DATA ########################################################################
 
 LANG = ['ar', 'de', 'en', 'es', 'hi', 'vi', 'zh']
 TRAIN = {__l: tfds.load('mlqa/' + __l, split='test', as_supervised=False, shuffle_files=True, data_dir='~/.cache/tensorflow/', batch_size=N_BATCH) for __l in LANG}
 TEST = {__l: tfds.load('mlqa/' + __l, split='validation', as_supervised=False, shuffle_files=True, data_dir='~/.cache/tensorflow/', batch_size=N_BATCH) for __l in LANG}
 
 # PREPROCESS ##################################################################
 
 PIPELINE = [
     # offset by 1 to 15 character => (B, 1) bytes
     *[(functools.partial(tokun.pipeline.offset, ticks=__t), False) for __t in OFFSET_TICKS], # (offsets 0, ..., (2 ^ i) - 1) + (offsets 2 ^ i, ..., 2 ^ (i+1) - 1)
     # encode => (B, G * S,) int
-    (functools.partial(tokun.pipeline.encode, token_size=TOKEN_LENGTH, sample_size=N_SAMPLE), True),
+    (functools.partial(tokun.pipeline.encode, token_size=TOKEN_SIZES[-1], sample_size=N_SAMPLE), True),
     # reshape => (B * G * S,) int
     (functools.partial(tokun.pipeline.reshape, groups=N_TOKEN_DIM, flatten=True), True),
     # one-hot encoding => (B * G * S, E) int (bool)
     (functools.partial(tf.one_hot, depth=N_ENCODING_DIM, axis=-1), True),
     # replace sample inputs with (input, target) for supervised learning
     ((lambda x: (x, x)), True)]
 
 OPERATIONS, REPLACE = zip(*PIPELINE)
 
 TRAIN = {__l: tokun.pipeline.process(dataset=__d, feature='context', pipeline=OPERATIONS, replace=REPLACE) for __l, __d in TRAIN.items()}
 TEST = {__l: tokun.pipeline.process(dataset=__d, feature='context', pipeline=OPERATIONS, replace=REPLACE) for __l, __d in TEST.items()}
 
-# LOAD ########################################################################
-
-MODEL = keras.models.load_model(PATH_MODEL)
-
 # SAMPLES #####################################################################
 
 SAMPLES = {}
-TOKENS = {__i // 4: {} for __i in itertools.accumulate(N_TOKEN_DIM, lambda x, y: x * y)}
-EMBEDDINGS = {__i // 4: {} for __i in itertools.accumulate(N_TOKEN_DIM, lambda x, y: x * y)}
+TOKENS = {__i: {} for __i in TOKEN_SIZES} # in bytes
+EMBEDDINGS = {__i: {} for __i in TOKEN_SIZES} # in bytes
 
 for __lang in TEST:
     # compute predictions
     __batch = iter(TEST[__lang]) # iterate over batches of samples
     __input = next(__batch)[0] # take input only
     __output = MODEL(__input)
     # sample predictions (inputs, outputs)
     SAMPLES[__lang] = (__input, __output)
 
 # TOKENS ######################################################################
 
 # unique (G ^ i)-tokens
 for __lang, __sample in SAMPLES.items():
     for __size in TOKENS:
-        TOKENS[__size][__lang] = tokun.pipeline.chunk(sequence=tokun.pipeline.postprocess(__sample[0]), size=__size, repeats=False)
+        TOKENS[__size][__lang] = tokun.pipeline.chunk(sequence=tokun.pipeline.postprocess(__sample[0]), size=__size // 4, repeats=False)
 
 # unique tokens, for all languages
 for __size in TOKENS:
     TOKENS[__size]['all'] = list(set(__t for _, __s in TOKENS[__size].items() for __t in __s))
 
 # EMBEDDINGS ##################################################################
 
-for __depth, __size in enumerate(TOKENS.keys()):
+for __depth, __size in enumerate(TOKEN_SIZES):
     for __lang, __tokens in TOKENS[__size].items():
         # re-encode without token repeats
         __input = tokun.pipeline.preprocess(text=''.join(__tokens), groups=N_TOKEN_DIM, flatten=True)
         # UTF-32 embedding
         __embedding = MODEL._encoder._encoder.layers[0](__input)
         # iterative CNN tokenization
         for __i in range(__depth + 1):
```

### Comparing `tokun-0.3.4/tokun/layers.py` & `tokun-0.3.5/tokun/layers.py`

 * *Files identical despite different names*

### Comparing `tokun-0.3.4/tokun/model.py` & `tokun-0.3.5/tokun/model.py`

 * *Files identical despite different names*

### Comparing `tokun-0.3.4/tokun/pipeline.py` & `tokun-0.3.5/tokun/pipeline.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,14 +7,19 @@
 import tensorflow as tf
 
 # GENERIC #####################################################################
 
 def compare(left: str, right: str) -> float:
     return sum(__l == __r for __l, __r in zip(left, right)) / max(1, len(left))
 
+def intersection(left: str, right: str) -> float:
+    __intersection = len(set(left).intersection(set(right)))
+    __reference = min(len(set(left)), len(set(right)))
+    return __intersection / max(1., __reference)
+
 # ENCODE ######################################################################
 
 def _encode_scalar(text: str, token_size: int) -> tf.Tensor:
     # encode the string
     __bytes = list(text.encode('utf-32-be'))
     # pad until the encodeed text has length multiple of the token length
     __padding = (-len(__bytes) % token_size) * [0]
@@ -97,7 +102,16 @@
 # < ###########################################################################
 
 def postprocess(output: tf.Tensor) -> str:
     # from one-hot to UTF-32 bytes
     __output = interpret(output=output)
     # flatten the groups of 4 bytes
     return decode(tokens=__output)
+
+# SAMPLING ####################################################################
+
+def sample(model: tf.keras.models.Model, text: str, **kwargs) -> tuple:
+    __x = preprocess(text=text, **kwargs)
+    __e = model._encoder(__x)
+    __p = model(__x)
+    __y = postprocess(__p)
+    return (__x, __e, __p, __y)
```

### Comparing `tokun-0.3.4/tokun/train.py` & `tokun-0.3.5/tokun/train.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 """Train tokun from scratch or from a checkpoint."""
 
 import datetime
 import functools
+import itertools
 import math
 import os
 
 import tensorflow as tf
 import tensorflow_datasets as tfds
 
 import mlable.tensorflow.optimizers as _mto
 
 import tokun.meta
 import tokun.model
 import tokun.pipeline
 
+# TOGGLE ######################################################################
+
+IMPORT = True
+TRAINING = True
+
 # META ########################################################################
 
 ATTENTION = True
 NORMALIZATION = True
 
 N_TOKEN_DIM = [4, 4, 4] # G, for each block
 N_ENCODING_DIM = 256 # U
@@ -25,78 +31,83 @@
 N_LATENT_DIM = N_EMBEDDING_DIM # L
 
 N_EPOCHS = 8
 N_EPOCHS_RAMPUP = 0
 N_EPOCHS_SUSTAIN = 0
 
 N_BATCH = 128 # number of samples per batch
-N_SAMPLE = 128 # number of characters per sample (=> N_TOKEN_DIM * N_SAMPLE integers per sample)
+N_SAMPLE = 256 # number of characters per sample (=> N_TOKEN_DIM * N_SAMPLE integers per sample)
 
-R_MIN, R_MAX, R_EXP = tokun.meta.rates(normalization=NORMALIZATION)
+R_MIN, R_MAX, R_EXP = tokun.meta.rates(pretrained=IMPORT, normalization=NORMALIZATION, base=0.001)
 
 # DERIVED #####################################################################
 
-TOKEN_LENGTH = math.prod(N_TOKEN_DIM) # in bytes
-OFFSET_TICKS = [2 ** __i for __i in range(int(math.log(TOKEN_LENGTH // 4, 2)))] # in characters
+TOKEN_SIZES = list(itertools.accumulate(N_TOKEN_DIM, lambda x, y: x * y)) # in bytes
+OFFSET_TICKS = [2 ** __i for __i in range(int(math.log(TOKEN_SIZES[-1] // 4, 2)))] # in characters
+
+# IMPORT ######################################################################
+
+PATH_IMPORT = os.path.join('models/4x4x4/True/True/0.99996.keras')
 
 # LOG #########################################################################
 
 VERSION = tokun.meta.version(groups=N_TOKEN_DIM, attention=ATTENTION, normalization=NORMALIZATION)
 DATETIME = datetime.datetime.now().strftime("%Y%m%d-%H%M%S")
 
 PATH_LOG = os.path.join('.logs/', *VERSION, DATETIME)
-PATH_MODEL = os.path.join('models/', *VERSION, DATETIME + '.keras')
+PATH_EXPORT = os.path.join('models/', *VERSION, DATETIME + '.keras')
 
 # DATA ########################################################################
 
 LANG = ['ar', 'de', 'en', 'es', 'hi', 'vi', 'zh']
 TRAIN = {__l: tfds.load('mlqa/' + __l, split='test', as_supervised=False, shuffle_files=True, data_dir='~/.cache/tensorflow/', batch_size=N_BATCH) for __l in LANG}
 TEST = {__l: tfds.load('mlqa/' + __l, split='validation', as_supervised=False, shuffle_files=True, data_dir='~/.cache/tensorflow/', batch_size=N_BATCH) for __l in LANG}
 
 # PREPROCESS ##################################################################
 
 PIPELINE = [
     # offset by 1 to 15 character => (B, 1) bytes
     *[(functools.partial(tokun.pipeline.offset, ticks=__t), False) for __t in OFFSET_TICKS], # (offsets 0, ..., (2 ^ i) - 1) + (offsets 2 ^ i, ..., 2 ^ (i+1) - 1)
     # encode => (B, G * S,) int
-    (functools.partial(tokun.pipeline.encode, token_size=TOKEN_LENGTH, sample_size=N_SAMPLE), True),
+    (functools.partial(tokun.pipeline.encode, token_size=TOKEN_SIZES[-1], sample_size=N_SAMPLE), True),
     # reshape => (B * G * S,) int
     (functools.partial(tokun.pipeline.reshape, groups=N_TOKEN_DIM, flatten=True), True),
     # one-hot encoding => (B * G * S, E) int (bool)
     (functools.partial(tf.one_hot, depth=N_ENCODING_DIM, axis=-1), True),
     # replace sample inputs with (input, target) for supervised learning
     ((lambda x: (x, x)), True)]
 
 OPERATIONS, REPLACE = zip(*PIPELINE)
 
 TRAIN = {__l: tokun.pipeline.process(dataset=__d, feature='context', pipeline=OPERATIONS, replace=REPLACE) for __l, __d in TRAIN.items()}
 TEST = {__l: tokun.pipeline.process(dataset=__d, feature='context', pipeline=OPERATIONS, replace=REPLACE) for __l, __d in TEST.items()}
 
 # INIT ########################################################################
 
-MODEL = tokun.model.AutoEncoder(token_dim=N_TOKEN_DIM, encoding_dim=N_ENCODING_DIM, embedding_dim=N_EMBEDDING_DIM, latent_dim=N_LATENT_DIM, batch_dim=None, attention=ATTENTION, normalization=NORMALIZATION)
+if IMPORT and os.path.isfile(PATH_IMPORT):
+    MODEL = tf.keras.models.load_model(PATH_IMPORT)
+else:
+    MODEL = tokun.model.AutoEncoder(token_dim=N_TOKEN_DIM, encoding_dim=N_ENCODING_DIM, embedding_dim=N_EMBEDDING_DIM, latent_dim=N_LATENT_DIM, batch_dim=None, attention=ATTENTION, normalization=NORMALIZATION)
+
+# COMPILE #####################################################################
 
-# compile
 MODEL.compile(
     optimizer=tf.keras.optimizers.Adam(learning_rate=R_MAX),
     loss=tf.keras.losses.CategoricalCrossentropy(from_logits=False, label_smoothing=0., axis=-1, reduction=tf.keras.losses.Reduction.SUM_OVER_BATCH_SIZE, name='loss'),
     metrics=['accuracy'])
 
 # TRAIN #######################################################################
 
 tb_callback = tf.keras.callbacks.TensorBoard(log_dir=PATH_LOG)
-cp_callback = tf.keras.callbacks.ModelCheckpoint(PATH_MODEL, monitor='val_accuracy', verbose=1, save_best_only=True, save_weights_only=False, mode='auto', save_freq='epoch')
+cp_callback = tf.keras.callbacks.ModelCheckpoint(PATH_EXPORT, monitor='val_accuracy', verbose=1, save_best_only=True, save_weights_only=False, mode='auto', save_freq='epoch')
 lr_callback = tf.keras.callbacks.LearningRateScheduler(functools.partial(_mto.learning_rate_hokusai, lr_min=R_MIN, lr_max=R_MAX, lr_exp=R_EXP, rampup=N_EPOCHS_RAMPUP, sustain=N_EPOCHS_SUSTAIN), verbose=True)
 
-HISTORY = MODEL.fit(
-    x=TRAIN['ar'].concatenate(TRAIN['en']).concatenate(TRAIN['es']).concatenate(TRAIN['de']).concatenate(TRAIN['hi']).concatenate(TRAIN['vi']).concatenate(TRAIN['zh']),
-    batch_size=N_BATCH,
-    epochs=N_EPOCHS,
-    validation_split=None,
-    validation_data=TEST['zh'], # full of glyphs
-    validation_freq=list(range(1, N_EPOCHS + 1, N_EPOCHS // 8)),
-    verbose=2,
-    callbacks=[lr_callback, cp_callback, tb_callback])
-
-# SAVE ########################################################################
-
-# MODEL.save(PATH_MODEL, save_format='keras')
+if TRAINING:
+    HISTORY = MODEL.fit(
+        x=TRAIN['ar'].concatenate(TRAIN['en']).concatenate(TRAIN['es']).concatenate(TRAIN['de']).concatenate(TRAIN['hi']).concatenate(TRAIN['vi']).concatenate(TRAIN['zh']),
+        batch_size=N_BATCH,
+        epochs=N_EPOCHS,
+        validation_split=None,
+        validation_data=TEST['zh'], # full of glyphs
+        validation_freq=list(range(1, N_EPOCHS + 1, N_EPOCHS // 8)),
+        verbose=2,
+        callbacks=[lr_callback, cp_callback, tb_callback])
```

### Comparing `tokun-0.3.4/PKG-INFO` & `tokun-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: tokun
-Version: 0.3.4
+Version: 0.3.5
 Summary: NN model specialized in text tokenization.
 Author: apehex
 Author-email: apehex@protonmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: mlable (>=0.1.3)
+Requires-Dist: mlable (>0.1.3)
 Requires-Dist: tensorflow (>=2.14)
 Requires-Dist: tensorflow-datasets (>=4.9)
 Requires-Dist: torch (>=2.2)
 Description-Content-Type: text/markdown
 
 # tokun
```

