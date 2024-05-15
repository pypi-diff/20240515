# Comparing `tmp/signapse-1.0.18.tar.gz` & `tmp/signapse-1.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signapse-1.0.18.tar", last modified: Mon Apr 15 13:16:10 2024, max compression
+gzip compressed data, was "signapse-1.0.19.tar", last modified: Wed May 15 15:40:03 2024, max compression
```

## Comparing `signapse-1.0.18.tar` & `signapse-1.0.19.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-15 13:16:10.881825 signapse-1.0.18/
--rw-r--r--   0 basheer   (1000) basheer   (1000)     2157 2024-04-15 13:16:10.881825 signapse-1.0.18/PKG-INFO
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     1637 2024-04-05 09:17:43.000000 signapse-1.0.18/README.md
--rw-rw-r--   0 basheer   (1000) basheer   (1000)       38 2024-04-15 13:16:10.881825 signapse-1.0.18/setup.cfg
--rw-rw-r--   0 basheer   (1000) basheer   (1000)      779 2024-04-15 13:15:51.000000 signapse-1.0.18/setup.py
-drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-15 13:16:10.881825 signapse-1.0.18/signapse/
--rw-rw-r--   0 basheer   (1000) basheer   (1000)      521 2024-04-15 11:23:11.000000 signapse-1.0.18/signapse/__init__.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     6566 2024-04-09 10:40:55.000000 signapse-1.0.18/signapse/build_opt.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     9366 2024-04-08 14:49:55.000000 signapse-1.0.18/signapse/compute.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     2662 2024-04-04 10:51:14.000000 signapse-1.0.18/signapse/constants.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     8315 2024-04-15 12:44:08.000000 signapse-1.0.18/signapse/create.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     1225 2024-04-04 11:11:01.000000 signapse-1.0.18/signapse/create_model.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)    21925 2024-04-15 13:11:54.000000 signapse-1.0.18/signapse/heatmaps.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     4652 2023-12-03 23:04:06.000000 signapse-1.0.18/signapse/lang_sam.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     4444 2024-04-08 10:09:21.000000 signapse-1.0.18/signapse/lang_utils.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)    17696 2023-12-03 23:04:06.000000 signapse-1.0.18/signapse/models_utils.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     3888 2024-04-04 14:23:34.000000 signapse-1.0.18/signapse/mp_utils.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     5793 2024-04-09 10:56:58.000000 signapse-1.0.18/signapse/poses.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     3403 2024-04-09 10:57:12.000000 signapse-1.0.18/signapse/preprocessing.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     1364 2024-04-13 16:24:05.000000 signapse-1.0.18/signapse/train_anno.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     2610 2023-12-03 23:04:06.000000 signapse-1.0.18/signapse/utils.py
-drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-15 13:16:10.881825 signapse-1.0.18/signapse.egg-info/
--rw-r--r--   0 basheer   (1000) basheer   (1000)     2157 2024-04-15 13:16:10.000000 signapse-1.0.18/signapse.egg-info/PKG-INFO
--rw-rw-r--   0 basheer   (1000) basheer   (1000)      471 2024-04-15 13:16:10.000000 signapse-1.0.18/signapse.egg-info/SOURCES.txt
--rw-rw-r--   0 basheer   (1000) basheer   (1000)        1 2024-04-15 13:16:10.000000 signapse-1.0.18/signapse.egg-info/dependency_links.txt
--rw-rw-r--   0 basheer   (1000) basheer   (1000)        9 2024-04-15 13:16:10.000000 signapse-1.0.18/signapse.egg-info/top_level.txt
+drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-05-15 15:40:03.170634 signapse-1.0.19/
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     2157 2024-05-15 15:40:03.170634 signapse-1.0.19/PKG-INFO
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     1637 2024-04-05 09:17:43.000000 signapse-1.0.19/README.md
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)       38 2024-05-15 15:40:03.170634 signapse-1.0.19/setup.cfg
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)      779 2024-05-15 15:39:54.000000 signapse-1.0.19/setup.py
+drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-05-15 15:40:03.170634 signapse-1.0.19/signapse/
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)      521 2024-04-15 11:23:11.000000 signapse-1.0.19/signapse/__init__.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     6566 2024-04-09 10:40:55.000000 signapse-1.0.19/signapse/build_opt.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     9366 2024-04-08 14:49:55.000000 signapse-1.0.19/signapse/compute.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     2662 2024-04-04 10:51:14.000000 signapse-1.0.19/signapse/constants.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     8232 2024-05-11 10:38:52.000000 signapse-1.0.19/signapse/create.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     1225 2024-04-04 11:11:01.000000 signapse-1.0.19/signapse/create_model.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)    23670 2024-05-15 10:32:31.000000 signapse-1.0.19/signapse/heatmaps.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     4652 2023-12-03 23:04:06.000000 signapse-1.0.19/signapse/lang_sam.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     4535 2024-05-15 08:09:49.000000 signapse-1.0.19/signapse/lang_utils.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)    17696 2023-12-03 23:04:06.000000 signapse-1.0.19/signapse/models_utils.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     3888 2024-04-04 14:23:34.000000 signapse-1.0.19/signapse/mp_utils.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     5793 2024-04-09 10:56:58.000000 signapse-1.0.19/signapse/poses.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     3403 2024-04-09 10:57:12.000000 signapse-1.0.19/signapse/preprocessing.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     1364 2024-04-13 16:24:05.000000 signapse-1.0.19/signapse/train_anno.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     2610 2023-12-03 23:04:06.000000 signapse-1.0.19/signapse/utils.py
+drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-05-15 15:40:03.170634 signapse-1.0.19/signapse.egg-info/
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     2157 2024-05-15 15:40:03.000000 signapse-1.0.19/signapse.egg-info/PKG-INFO
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)      471 2024-05-15 15:40:03.000000 signapse-1.0.19/signapse.egg-info/SOURCES.txt
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)        1 2024-05-15 15:40:03.000000 signapse-1.0.19/signapse.egg-info/dependency_links.txt
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)        9 2024-05-15 15:40:03.000000 signapse-1.0.19/signapse.egg-info/top_level.txt
```

### Comparing `signapse-1.0.18/PKG-INFO` & `signapse-1.0.19/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signapse
-Version: 1.0.18
+Version: 1.0.19
 Summary: Signapse_synthetic_signer
 Home-page: https://github.com/signapse/signapse
 Author: Basheer Alwaely
 Author-email: basheer@signapse.ai
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `signapse-1.0.18/README.md` & `signapse-1.0.19/README.md`

 * *Files identical despite different names*

### Comparing `signapse-1.0.18/setup.py` & `signapse-1.0.19/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md","r") as ofile:
     long_description_file = ofile.read()
     
 setup(
     name='signapse',
-    version='1.0.18',
+    version='1.0.19',
     description='Signapse_synthetic_signer',
     long_description=long_description_file,
     long_description_content_type="text/markdown",
     author='Basheer Alwaely',
     author_email='basheer@signapse.ai',
     url='https://github.com/signapse/signapse',
     packages=find_packages(),
```

### Comparing `signapse-1.0.18/signapse/__init__.py` & `signapse-1.0.19/signapse/__init__.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.18/signapse/build_opt.py` & `signapse-1.0.19/signapse/build_opt.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.18/signapse/compute.py` & `signapse-1.0.19/signapse/compute.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.18/signapse/constants.py` & `signapse-1.0.19/signapse/constants.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.18/signapse/create.py` & `signapse-1.0.19/signapse/create.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,30 +100,30 @@
                   
             if counter==0 and (self.args.opt.num_frames)>0:
                 for _ in range(self.args.opt.num_frames):
                     maps.append(heat_maps)
                     crops.append(hand_crops)
                     
             maps.append(heat_maps)
-            crops.append(hand_crops)
+            crops.append(hand_crops) 
             
             if (self.args.opt.num_frames)>counter:
                 mid_input_frame = copy.deepcopy(input_frame)
                 continue
             
             if not self.args.opt.multi_frames:
                 mid_input_frame = input_frame
         
             frame = HEATMAPS().generate_GAN_frame_maps_crops(mid_input_frame,
-                                                           maps,
-                                                           crops,
-                                                           GAN_model= GAN_model,
-                                                           opt=self.args.opt,
-                                                           detailed_video=self.args.detailed_video                                                                                                
-                                                           )
+                                                             maps,
+                                                             crops,
+                                                             GAN_model= GAN_model,
+                                                             opt=self.args.opt,
+                                                             detailed_video=self.args.detailed_video
+                                                             )
                 
             
 
             # Write each generated frame to the output video
             output_video.append_data(frame)
             maps = maps[1:]
             crops =crops[1:]
```

### Comparing `signapse-1.0.18/signapse/create_model.py` & `signapse-1.0.19/signapse/create_model.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.18/signapse/heatmaps.py` & `signapse-1.0.19/signapse/heatmaps.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,78 +98,98 @@
             mask = mask.astype(bool)
             cropped_frame[mask] = image[mask]
             if gray:
                 cropped_frame = cv2.cvtColor(cropped_frame, cv2.COLOR_BGR2GRAY)
             return cropped_frame 
     
         
-    def skin_detection(self,frame,signer):    
+    def skin_detection(self,frame,signer,include_hair= False):  
         space = cv2.cvtColor(frame, cv2.COLOR_RGB2YCrCb)
+
         if signer =="Marcel":
             lower_skin = np.array([60, 150, 77])   
             upper_skin = np.array([255, 190, 120])  
         elif signer =="Jay":
+            
             lower_skin = np.array([30, 127, 77])   
             upper_skin = np.array([255, 190, 125]) 
         elif signer =="Rachel":
-            lower_skin = np.array([128, 141, 107])   
-            upper_skin = np.array([255, 190, 120]) 
-            # lower_skin = np.array([30, 130, 90])   
-            # upper_skin = np.array([255, 190, 125])    
+            # sharp to seprate the hair
+            if include_hair:
+                lower_skin = np.array([50, 130, 90])  
+                upper_skin = np.array([220, 190, 125]) 
+            else:                
+                lower_skin = np.array([135, 131, 103])   
+                upper_skin = np.array([255, 190, 120]) 
+   
         else:
             raise TypeError("Please set the signer into Marcel, Rachel or Jay. Skin_detection function in utils.py") 
         
         mask = cv2.inRange(space, lower_skin, upper_skin)
         # remove noise
         #mask = cv2.erode(mask, np.ones((3,3), np.uint8), iterations=2)
         mask = cv2.dilate(mask, np.ones((5,5), np.uint8), iterations=1)
         skin = cv2.cvtColor(cv2.bitwise_and(frame, frame, mask=mask), cv2.COLOR_BGR2GRAY)
         return skin 
     
-    def get_edge(self,cropped_frame):                
-        blurred = cropped_frame #cv2.GaussianBlur(cropped_frame, (3, 3), 0)
-        
-        grad_x = cv2.Sobel(blurred, cv2.CV_64F, 1, 0, ksize=3)
-        grad_y = cv2.Sobel(blurred, cv2.CV_64F, 0, 1, ksize=3)
+    def get_edge(self,input_img):
+        input_array = torch.clamp((input_img + 1) * 127.5, 0, 255).byte()
+        np_img = input_array[0].cpu().numpy()       
+        grad_x = cv2.Sobel(np_img, cv2.CV_64F, 1, 0, ksize=3)
+        grad_y = cv2.Sobel(np_img, cv2.CV_64F, 0, 1, ksize=3)
         abs_grad_x = cv2.convertScaleAbs(grad_x)
         abs_grad_y = cv2.convertScaleAbs(grad_y)
-        cropped_frame = cv2.addWeighted(abs_grad_x, 0.5, abs_grad_y, 0.5, 0)  
-        return cropped_frame
+        edges = cv2.addWeighted(abs_grad_x, 0.5, abs_grad_y, 0.5, 0) 
+        edge_tensor =  torch.tensor(edges, dtype=torch.float32) / 255.0 * 2.0 - 1.0
+        return edge_tensor.unsqueeze(0)
+
+    # def get_edge(self,blurred):                
+    #     #blurred = cv2.GaussianBlur(blurred, (3, 3), 0)        
+    #     grad_x = cv2.Sobel(blurred, cv2.CV_64F, 1, 0, ksize=3)
+    #     grad_y = cv2.Sobel(blurred, cv2.CV_64F, 0, 1, ksize=3)
+    #     abs_grad_x = cv2.convertScaleAbs(grad_x)
+    #     abs_grad_y = cv2.convertScaleAbs(grad_y)
+    #     cropped_frame = cv2.addWeighted(abs_grad_x, 0.5, abs_grad_y, 0.5, 0)  
+    #     return cropped_frame
 
     def Rachel_hair_removal(self,face,hand,skin):
         face[face !=0] = 1
         hand[hand !=0] = 1
         mask = hand + face
         mask[mask > 1] = 1
         mask = cv2.dilate(mask[0], np.ones((5,5), np.uint8), iterations=1)
         mask = cv2.erode(mask, np.ones((5,5), np.uint8), iterations=1)[np.newaxis,...]
         return mask * skin
 
     def crop_hand_gray_normalised(self,signer,frame,hand,face_mask,SAM_hand=False, SAM_face=False, SAM_skin=False,SAM_hand_edge = False, SAM_face_edge = False, SAM_skin_edge = False):
         if SAM_hand:
             gray = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)
-            hand = (gray*hand).astype('uint8')[0]    
+            hand = (gray*hand).astype('uint8')[0] /255
+            hand_mask = np.expand_dims(hand,axis=0)
             if SAM_hand_edge:
-                hand = self.get_edge(hand)                      
-            hand = np.expand_dims(hand,axis=0)/255
+                hand = np.array(self.get_edge(torch.from_numpy(hand_mask)))                     
+            
                     
         if SAM_face:
-            face = self.get_face_crop(frame,face_mask)            
+            face = self.get_face_crop(frame,face_mask) /255 
+            face_mask = np.expand_dims(face,axis=0)       
             if SAM_face_edge:
-                face = self.get_edge(face)
-            face = np.expand_dims(face,axis=0)/255
+                face = np.array(self.get_edge(torch.from_numpy(face_mask)))
+            
             
         if SAM_skin:
-            skin = self.skin_detection(frame,signer)
+            skin = self.skin_detection(frame,signer,include_hair = (SAM_hand and SAM_face and SAM_skin)) /255
+            skin_mask = np.expand_dims(skin,axis=0)
             if SAM_skin_edge:
-                skin = self.get_edge(skin)                   
-            skin = np.expand_dims(skin,axis=0)/255
+                skin = np.array(self.get_edge(torch.from_numpy(skin_mask)))           
+            
             
         if SAM_hand and SAM_face and SAM_skin:
-            skin = self.Rachel_hair_removal(face,hand,skin)
+            skin = self.Rachel_hair_removal(face_mask,hand_mask,skin_mask)
+            skin = np.array(self.get_edge(torch.from_numpy(skin)))            
             return skin 
             
         if SAM_hand and SAM_face:
             return (np.concatenate((hand, face)))
         elif SAM_skin:
             return skin  
         elif SAM_hand:
@@ -323,39 +343,52 @@
         for frame in heat_map:
             full_heatmap = np.add(full_heatmap,frame)  #full_heatmap + frame
         full_heatmap = ((full_heatmap != 0) == False)*255
         return full_heatmap.astype(imtype)
     
     
     def get_pose_image(self,opt,input_frame,generated,heat_map,crops):
-        if opt.hand_crop and opt.face_crop:
+        if opt.sam:            
             if opt.multi_frames:
                 total_maps_per_sample = (len(heat_map)//((opt.num_frames*2)+1)) - len(crops[0])
                 input_label = self.convert_limb_heatmap(heat_map[opt.num_frames*total_maps_per_sample:(opt.num_frames+1)*total_maps_per_sample,:,:]).reshape((heat_map.shape[1], heat_map.shape[2], 1))
-            else:             
-                input_label = self.convert_limb_heatmap(heat_map[:-2]).reshape((heat_map.shape[1], heat_map.shape[2], 1))
+            
+            elif (opt.hand_crop and opt.face_crop) and not opt.skin_crop:
+                input_label = self.convert_limb_heatmap(heat_map[:-2]).reshape((heat_map.shape[1], heat_map.shape[2], 1))            
+            else:
+                input_label = self.convert_limb_heatmap(heat_map[:-1]).reshape((heat_map.shape[1], heat_map.shape[2], 1))
+            
+                
 
             if  opt.crop_normalise:
+                avg_bg = -int(crops[0][0][:10,:10].mean()) # to keep the background zeros
                 if opt.erusion:
-                    hand = (crops[0][0].numpy() +1 ) * 255
+                    hand = (crops[0][0].numpy() + avg_bg ) * 255
                     if not opt.merge_crops:
-                        body = (crops[0][1].numpy() +1 ) * 255
+                        body = (crops[0][1].numpy() + avg_bg ) * 255
                 else:
-                    hand = crops[0][0].numpy() * 255
-                    if not opt.merge_crops:
-                        body = crops[0][1].numpy() * 255
-                hand[hand==0]=255
-                if not opt.merge_crops:
-                    body[body==0]=255
-                if opt.merge_crops:
-                    input_label[:,:,0] = (input_label[:,:,0]) + (255 - (hand).astype(np.uint8)) 
-                else:                
+                    hand = (crops[0][0].numpy()+ avg_bg) * 255
+                    if (opt.hand_crop and opt.face_crop) and not opt.skin_crop :
+                        body = (crops[0][1].numpy()+ avg_bg) * 255
+                        body[body==0]=255
+                hand[hand==0]=255             
+ 
+                
+                if (opt.hand_crop and opt.face_crop) and not (opt.skin_crop or opt.merge_crops):
                     input_label[:,:,0] = (input_label[:,:,0]) + (255 - (hand).astype(np.uint8))  + (255-(body).astype(np.uint8)) 
-            else:            
-                input_label[:,:,0] = input_label[:,:,0] + (heat_map[-2]*255).numpy().astype(np.uint8) + (heat_map[-1]*255).numpy().astype(np.uint8)
+                else:
+                    input_label[:,:,0] = (input_label[:,:,0]) + (255 - (hand).astype(np.uint8)) 
+                             
+                    
+            else: 
+                if (opt.hand_crop and opt.face_crop) and not (opt.skin_crop or opt.merge_crops):                              
+                    input_label[:,:,0] = input_label[:,:,0] + (heat_map[-2]*255).numpy().astype(np.uint8) + (heat_map[-1]*255).numpy().astype(np.uint8)
+                else:
+                    input_label[:,:,0] = input_label[:,:,0] + (heat_map[-1]*255).numpy().astype(np.uint8)
+                    
                 
         elif opt.hand_crop or opt.face_crop or opt.skin_crop:
             if opt.N2N:
                 input_label = self.convert_limb_heatmap(heat_map).reshape((heat_map.shape[1], heat_map.shape[2], 1))
             elif opt.multi_frames:
                 total_maps_per_sample = (len(heat_map)//((opt.num_frames*2)+1)) - len(crops[0])
                 input_label = self.convert_limb_heatmap(heat_map[opt.num_frames*total_maps_per_sample:(opt.num_frames+1)*total_maps_per_sample,:,:]).reshape((heat_map.shape[1], heat_map.shape[2], 1))
```

### Comparing `signapse-1.0.18/signapse/lang_sam.py` & `signapse-1.0.19/signapse/lang_sam.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.18/signapse/lang_utils.py` & `signapse-1.0.19/signapse/lang_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,16 @@
             mask =  torch.Tensor()
             mask2=[]
             for i, frame in enumerate(reader): 
                 if i < self.args.start:
                     continue     
                 if i% 50==0:
                     logging.info("Frame: {}".format(i))
+                if self.args.stop != -1 and i >= self.args.stop:
+                    break
                 
                 frame = IMAGE_PROCESSING().apply_norm(frame,img_centre,self.args.opt.loadSize)
                 image_pil = array2pil(frame,enhance=True)
                     
                     
                 masks, _, _, _ = model.predict(image_pil, "hand", box_threshold=0.2, text_threshold=0.2, padding = None)
                 if len(masks) ==0:
```

### Comparing `signapse-1.0.18/signapse/models_utils.py` & `signapse-1.0.19/signapse/models_utils.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.18/signapse/mp_utils.py` & `signapse-1.0.19/signapse/mp_utils.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.18/signapse/poses.py` & `signapse-1.0.19/signapse/poses.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.18/signapse/preprocessing.py` & `signapse-1.0.19/signapse/preprocessing.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.18/signapse/train_anno.py` & `signapse-1.0.19/signapse/train_anno.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.18/signapse/utils.py` & `signapse-1.0.19/signapse/utils.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.18/signapse.egg-info/PKG-INFO` & `signapse-1.0.19/signapse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signapse
-Version: 1.0.18
+Version: 1.0.19
 Summary: Signapse_synthetic_signer
 Home-page: https://github.com/signapse/signapse
 Author: Basheer Alwaely
 Author-email: basheer@signapse.ai
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

