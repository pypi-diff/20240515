# Comparing `tmp/facexformer_pipeline-0.2.1.tar.gz` & `tmp/facexformer_pipeline-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facexformer_pipeline-0.2.1.tar", last modified: Mon May 13 15:15:57 2024, max compression
+gzip compressed data, was "facexformer_pipeline-0.2.2.tar", last modified: Wed May 15 15:41:43 2024, max compression
```

## Comparing `facexformer_pipeline-0.2.1.tar` & `facexformer_pipeline-0.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:15:57.310484 facexformer_pipeline-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-13 15:15:57.310484 facexformer_pipeline-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-13 15:15:53.000000 facexformer_pipeline-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:15:57.310484 facexformer_pipeline-0.2.1/facexformer_pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-13 15:15:53.000000 facexformer_pipeline-0.2.1/facexformer_pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-13 15:15:53.000000 facexformer_pipeline-0.2.1/facexformer_pipeline/facexformer_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:15:57.310484 facexformer_pipeline-0.2.1/facexformer_pipeline/network/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-13 15:15:53.000000 facexformer_pipeline-0.2.1/facexformer_pipeline/network/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:15:57.310484 facexformer_pipeline-0.2.1/facexformer_pipeline/network/models/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-13 15:15:53.000000 facexformer_pipeline-0.2.1/facexformer_pipeline/network/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11176 2024-05-13 15:15:53.000000 facexformer_pipeline-0.2.1/facexformer_pipeline/network/models/facexformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9587 2024-05-13 15:15:53.000000 facexformer_pipeline-0.2.1/facexformer_pipeline/network/models/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-13 15:15:53.000000 facexformer_pipeline-0.2.1/facexformer_pipeline/task_postprocesser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-13 15:15:53.000000 facexformer_pipeline-0.2.1/facexformer_pipeline/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:15:57.310484 facexformer_pipeline-0.2.1/facexformer_pipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-13 15:15:57.000000 facexformer_pipeline-0.2.1/facexformer_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-13 15:15:57.000000 facexformer_pipeline-0.2.1/facexformer_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 15:15:57.000000 facexformer_pipeline-0.2.1/facexformer_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-13 15:15:57.000000 facexformer_pipeline-0.2.1/facexformer_pipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-13 15:15:57.000000 facexformer_pipeline-0.2.1/facexformer_pipeline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 15:15:57.310484 facexformer_pipeline-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-13 15:15:53.000000 facexformer_pipeline-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:41:43.759518 facexformer_pipeline-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-15 15:41:43.759518 facexformer_pipeline-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-15 15:41:38.000000 facexformer_pipeline-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:41:43.755518 facexformer_pipeline-0.2.2/facexformer_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-15 15:41:38.000000 facexformer_pipeline-0.2.2/facexformer_pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7437 2024-05-15 15:41:38.000000 facexformer_pipeline-0.2.2/facexformer_pipeline/facexformer_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:41:43.755518 facexformer_pipeline-0.2.2/facexformer_pipeline/network/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-15 15:41:38.000000 facexformer_pipeline-0.2.2/facexformer_pipeline/network/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:41:43.755518 facexformer_pipeline-0.2.2/facexformer_pipeline/network/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-15 15:41:38.000000 facexformer_pipeline-0.2.2/facexformer_pipeline/network/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11176 2024-05-15 15:41:38.000000 facexformer_pipeline-0.2.2/facexformer_pipeline/network/models/facexformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9587 2024-05-15 15:41:38.000000 facexformer_pipeline-0.2.2/facexformer_pipeline/network/models/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-15 15:41:38.000000 facexformer_pipeline-0.2.2/facexformer_pipeline/task_postprocesser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-15 15:41:38.000000 facexformer_pipeline-0.2.2/facexformer_pipeline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:41:43.759518 facexformer_pipeline-0.2.2/facexformer_pipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-15 15:41:43.000000 facexformer_pipeline-0.2.2/facexformer_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-15 15:41:43.000000 facexformer_pipeline-0.2.2/facexformer_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 15:41:43.000000 facexformer_pipeline-0.2.2/facexformer_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-15 15:41:43.000000 facexformer_pipeline-0.2.2/facexformer_pipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-15 15:41:43.000000 facexformer_pipeline-0.2.2/facexformer_pipeline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 15:41:43.759518 facexformer_pipeline-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-15 15:41:38.000000 facexformer_pipeline-0.2.2/setup.py
```

### Comparing `facexformer_pipeline-0.2.1/PKG-INFO` & `facexformer_pipeline-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facexformer_pipeline
-Version: 0.2.1
+Version: 0.2.2
 Summary: A module to run facexformer model as pipeline
 Author: Enes Kuzucu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `facexformer_pipeline-0.2.1/README.md` & `facexformer_pipeline-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `facexformer_pipeline-0.2.1/facexformer_pipeline/facexformer_pipeline.py` & `facexformer_pipeline-0.2.2/facexformer_pipeline/facexformer_pipeline.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from torchvision.transforms import InterpolationMode
 import argparse
 from math import cos, sin
 from PIL import Image
 from network import FaceXFormer
 from facenet_pytorch import MTCNN
 from image_input_handler import  UniversalImageInputHandler
-from utils import denorm_points, unnormalize, adjust_bbox, visualize_head_pose, visualize_landmarks, visualize_mask
+from facexformer_pipeline.utils import denorm_points, unnormalize, adjust_bbox, visualize_head_pose, visualize_landmarks, visualize_mask
 from task_postprocesser import task_faceparsing,  process_landmarks, task_headpose , task_attributes, task_gender, process_visibility
 import torchvision.transforms as transforms
 from huggingface_hub import hf_hub_download
 import numpy as np
 import torch
 
 class FacexformerPipeline:
@@ -120,17 +120,40 @@
             results['headpose'] = task_headpose(output[1], images)
         elif task_id == 3:
             results['attributes'] = task_attributes(output[2])
         elif task_id == 4:
             results['age_gender_race_dict'] = task_gender(output[4], output[5], output[6])
         elif task_id == 5:
             results['visibility'] = process_visibility(output[3])
+
+    # from PIL import Image, ImageDraw
+    # import numpy as np
+
+    def scale_landmarks_to_original_image(self, original_image, landmarks, resized_image_size=(224, 224)):
+        # print("landmarks[0]:", landmarks[0])
+        original_width, original_height = original_image.shape[1],  original_image.shape[0]
+        # print("original_width:", original_width, "original_height:", original_height)
+        resized_width, resized_height = resized_image_size
+        scale_x = original_width / resized_width
+        scale_y = original_height / resized_height
+
+        # Scale landmarks back to original image dimensions
+
+
+        scaled_landmarks = [(x * scale_x, y * scale_y) for (x, y) in landmarks]
+        scaled_landmarks_int = [(int(round(x)), int(round(y))) for (x, y) in scaled_landmarks]
+
+        # print("scaled_landmarks[0]:", scaled_landmarks[0])
+
+        return scaled_landmarks_int
+
+
     def run_model(self, image, image_is_cropped=True):
         results = {}
-
+        original_image=image.copy()
         image = Image.fromarray(image)
         if not image_is_cropped:
             image = self.crop_face_area_from_image(image)
         image = self.transform_image(image)
         model_ready_image, labels = self.prepare_for_model(image, self.labels)
 
         for i in self.active_tasks:
@@ -139,14 +162,17 @@
             self.process_task_output(i, output, results, model_ready_image)
 
         image = unnormalize(model_ready_image[0].detach().cpu())
         image = image.permute(1, 2, 0).numpy()
         image = (image * 255).astype(np.uint8)
         image = image[:, :, ::-1]
         results['image'] = image
+        results['transformed_image'] = model_ready_image[0]
+
+        results['scaled_landmarks'] =self.scale_landmarks_to_original_image(original_image,results['landmark_list'] )
         return results
 
 def main():
     image_path = "sample_image.jpg"
     uih = UniversalImageInputHandler(image_path, debug=False)
     COMPATIBLE, img = uih.COMPATIBLE, uih.img
     pipeline = FacexformerPipeline(debug=False, tasks=['headpose', 'landmark', 'attributes'])
```

### Comparing `facexformer_pipeline-0.2.1/facexformer_pipeline/network/models/facexformer.py` & `facexformer_pipeline-0.2.2/facexformer_pipeline/network/models/facexformer.py`

 * *Files identical despite different names*

### Comparing `facexformer_pipeline-0.2.1/facexformer_pipeline/network/models/transformer.py` & `facexformer_pipeline-0.2.2/facexformer_pipeline/network/models/transformer.py`

 * *Files identical despite different names*

### Comparing `facexformer_pipeline-0.2.1/facexformer_pipeline/task_postprocesser.py` & `facexformer_pipeline-0.2.2/facexformer_pipeline/task_postprocesser.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import argparse
 from math import cos, sin
 from PIL import Image
 from network import FaceXFormer
 from facenet_pytorch import MTCNN
 import os
 # from argparse import  args
-from utils import denorm_points, unnormalize, adjust_bbox, visualize_head_pose, visualize_landmarks, visualize_mask
+from facexformer_pipeline.utils import denorm_points, unnormalize, adjust_bbox, visualize_head_pose, visualize_landmarks, visualize_mask
 
 def process_visibility(visibility_output):
     probs = torch.sigmoid(visibility_output[0])
     preds = (probs >= 0.5).float()
     pred = preds.tolist()
     pred_str = [str(int(b)) for b in pred]
     return pred_str
@@ -77,19 +77,15 @@
     denorm_landmarks = denorm_points(landmark_output.view(-1, 68, 2)[0], 224, 224)
     denorm_landmarks=denorm_landmarks.detach().cpu()
     image = unnormalize(images[0].detach().cpu())
 
     landmarks_list = []
     for landmark in denorm_landmarks[0]:
         x, y = landmark[0], landmark[1]
-        landmarks_list.append((int(x.item()), int(y.item())))
+        # landmarks_list.append((int(x.item()), int(y.item())))
+        landmarks_list.append((int(round(x.item())), int(round(y.item()))))
 
-    # landmarks_dict = {}
-    # for index, landmark in enumerate(denorm_landmarks[0]):
-    #     x, y = landmark[0], landmark[1]
-    #     landmarks_dict[f"landmark_{index}"] = (x.item(), y.item())
-
-    im = visualize_landmarks(image, denorm_landmarks, (255, 255, 0))
+    # im = visualize_landmarks(image, denorm_landmarks, (255, 255, 0))
     # save_path_viz = os.path.join(args.results_path, "landmarks.png")
-    cv2.imwrite("./landmarks.png", im[:, :, ::-1])
+    # cv2.imwrite("./landmarks.png", im[:, :, ::-1])
 
     return landmarks_list
```

### Comparing `facexformer_pipeline-0.2.1/facexformer_pipeline/utils.py` & `facexformer_pipeline-0.2.2/facexformer_pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `facexformer_pipeline-0.2.1/facexformer_pipeline.egg-info/PKG-INFO` & `facexformer_pipeline-0.2.2/facexformer_pipeline.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facexformer_pipeline
-Version: 0.2.1
+Version: 0.2.2
 Summary: A module to run facexformer model as pipeline
 Author: Enes Kuzucu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `facexformer_pipeline-0.2.1/facexformer_pipeline.egg-info/SOURCES.txt` & `facexformer_pipeline-0.2.2/facexformer_pipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `facexformer_pipeline-0.2.1/setup.py` & `facexformer_pipeline-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 import subprocess
 import os
 
 
 setup(
     name='facexformer_pipeline',  # Package name
-    version='0.2.1',  # Version of your package
+    version='0.2.2',  # Version of your package
     author='Enes Kuzucu',  # Your name
 
     description='A module to run facexformer model as pipeline',  # Short description
     long_description=open('README.md').read(),  # Long description from a README file
     long_description_content_type='text/markdown',  # Type of the long description
 #     url='https://github.com/karaposu/image-input-handler',  # URL to the repository
     packages=find_packages(),  # Automatically find packages in the directory
```

