# Comparing `tmp/lavis_gml-1.0.2.post3-py3-none-any.whl.zip` & `tmp/lavis_gml-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,61 +1,1066 @@
-Zip file size: 1828201 bytes, number of entries: 339
+Zip file size: 9880079 bytes, number of entries: 1790
 -rw-rw-r--  2.0 unx      666 b- defN 24-May-09 20:37 app/__init__.py
 -rw-rw-r--  2.0 unx     2380 b- defN 24-May-09 20:37 app/calculate_coco_features.py
 -rw-rw-r--  2.0 unx     2771 b- defN 24-May-09 20:37 app/caption.py
 -rw-rw-r--  2.0 unx     8076 b- defN 24-May-09 20:37 app/classification.py
 -rw-rw-r--  2.0 unx     7375 b- defN 24-May-09 20:37 app/dataset_browser.py
 -rw-rw-r--  2.0 unx     2825 b- defN 24-May-09 20:37 app/image_text_match.py
 -rw-rw-r--  2.0 unx      819 b- defN 24-May-09 20:37 app/main.py
 -rw-rw-r--  2.0 unx     7818 b- defN 24-May-09 20:37 app/multimodal_search.py
 -rw-rw-r--  2.0 unx     1318 b- defN 24-May-09 20:37 app/multipage.py
 -rw-rw-r--  2.0 unx     3457 b- defN 24-May-09 20:37 app/text_localization.py
 -rw-rw-r--  2.0 unx     2226 b- defN 24-May-09 20:37 app/utils.py
 -rw-rw-r--  2.0 unx     1967 b- defN 24-May-09 20:37 app/vqa.py
+-rw-rw-r--  2.0 unx      666 b- defN 24-May-09 20:37 build/lib/app/__init__.py
+-rw-rw-r--  2.0 unx     2380 b- defN 24-May-09 20:37 build/lib/app/calculate_coco_features.py
+-rw-rw-r--  2.0 unx     2771 b- defN 24-May-09 20:37 build/lib/app/caption.py
+-rw-rw-r--  2.0 unx     8076 b- defN 24-May-09 20:37 build/lib/app/classification.py
+-rw-rw-r--  2.0 unx     7375 b- defN 24-May-09 20:37 build/lib/app/dataset_browser.py
+-rw-rw-r--  2.0 unx     2825 b- defN 24-May-09 20:37 build/lib/app/image_text_match.py
+-rw-rw-r--  2.0 unx      819 b- defN 24-May-09 20:37 build/lib/app/main.py
+-rw-rw-r--  2.0 unx     7818 b- defN 24-May-09 20:37 build/lib/app/multimodal_search.py
+-rw-rw-r--  2.0 unx     1318 b- defN 24-May-09 20:37 build/lib/app/multipage.py
+-rw-rw-r--  2.0 unx     3457 b- defN 24-May-09 20:37 build/lib/app/text_localization.py
+-rw-rw-r--  2.0 unx     2226 b- defN 24-May-09 20:37 build/lib/app/utils.py
+-rw-rw-r--  2.0 unx     1967 b- defN 24-May-09 20:37 build/lib/app/vqa.py
+-rw-rw-r--  2.0 unx     1974 b- defN 24-May-09 20:37 build/lib/docs/conf.py
+-rw-rw-r--  2.0 unx      930 b- defN 24-May-09 20:37 build/lib/lavis/__init__.py
+-rw-rw-r--  2.0 unx    15070 b- defN 24-May-09 20:37 build/lib/lavis/common/config.py
+-rw-rw-r--  2.0 unx     3614 b- defN 24-May-09 20:37 build/lib/lavis/common/dist_utils.py
+-rw-rw-r--  2.0 unx      815 b- defN 24-May-09 20:37 build/lib/lavis/common/gradcam.py
+-rw-rw-r--  2.0 unx     5992 b- defN 24-May-09 20:37 build/lib/lavis/common/logger.py
+-rw-rw-r--  2.0 unx     4158 b- defN 24-May-09 20:37 build/lib/lavis/common/optims.py
+-rw-rw-r--  2.0 unx     9870 b- defN 24-May-09 20:37 build/lib/lavis/common/registry.py
+-rw-rw-r--  2.0 unx    14658 b- defN 24-May-09 20:37 build/lib/lavis/common/utils.py
+-rw-rw-r--  2.0 unx      980 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/util.py
+-rw-rw-r--  2.0 unx      155 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/canny/__init__.py
+-rw-rw-r--  2.0 unx     6585 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/hed/__init__.py
+-rw-rw-r--  2.0 unx     1400 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/midas/__init__.py
+-rw-rw-r--  2.0 unx     5229 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/midas/api.py
+-rw-rw-r--  2.0 unx     4582 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/midas/utils.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/midas/midas/__init__.py
+-rw-rw-r--  2.0 unx      367 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/midas/midas/base_model.py
+-rw-rw-r--  2.0 unx     9242 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/midas/midas/blocks.py
+-rw-rw-r--  2.0 unx     3154 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/midas/midas/dpt_depth.py
+-rw-rw-r--  2.0 unx     2709 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/midas/midas/midas_net.py
+-rw-rw-r--  2.0 unx     5207 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/midas/midas/midas_net_custom.py
+-rw-rw-r--  2.0 unx     7869 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/midas/midas/transforms.py
+-rw-rw-r--  2.0 unx    14625 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/midas/midas/vit.py
+-rw-rw-r--  2.0 unx     1458 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/mlsd/__init__.py
+-rw-rw-r--  2.0 unx    24049 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/mlsd/utils.py
+-rw-rw-r--  2.0 unx     9678 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/mlsd/models/mbv2_mlsd_large.py
+-rw-rw-r--  2.0 unx     9180 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/mlsd/models/mbv2_mlsd_tiny.py
+-rw-rw-r--  2.0 unx     1957 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/openpose/__init__.py
+-rw-rw-r--  2.0 unx    10994 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/openpose/body.py
+-rw-rw-r--  2.0 unx     3438 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/openpose/hand.py
+-rw-rw-r--  2.0 unx     8745 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/openpose/model.py
+-rw-rw-r--  2.0 unx     7507 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/openpose/util.py
+-rw-rw-r--  2.0 unx     1070 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/__init__.py
+-rw-rw-r--  2.0 unx      321 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/default_runtime.py
+-rw-rw-r--  2.0 unx     1844 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/datasets/ade20k.py
+-rw-rw-r--  2.0 unx     1924 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/datasets/chase_db1.py
+-rw-rw-r--  2.0 unx     1780 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/datasets/cityscapes.py
+-rw-rw-r--  2.0 unx     1281 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/datasets/cityscapes_769x769.py
+-rw-rw-r--  2.0 unx     1915 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/datasets/drive.py
+-rw-rw-r--  2.0 unx     1915 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/datasets/hrf.py
+-rw-rw-r--  2.0 unx     1998 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/datasets/pascal_context.py
+-rw-rw-r--  2.0 unx     2024 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/datasets/pascal_context_59.py
+-rw-rw-r--  2.0 unx     1930 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/datasets/pascal_voc12.py
+-rw-rw-r--  2.0 unx      261 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/datasets/pascal_voc12_aug.py
+-rw-rw-r--  2.0 unx     1917 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/datasets/stare.py
+-rw-rw-r--  2.0 unx     1346 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/models/ann_r50-d8.py
+-rw-rw-r--  2.0 unx     1302 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/models/apcnet_r50-d8.py
+-rw-rw-r--  2.0 unx     1258 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/models/ccnet_r50-d8.py
+-rw-rw-r--  2.0 unx     1110 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/models/cgnet.py
+-rw-rw-r--  2.0 unx     1261 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/models/danet_r50-d8.py
+-rw-rw-r--  2.0 unx     1273 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/models/deeplabv3_r50-d8.py
+-rw-rw-r--  2.0 unx     1499 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py
+-rw-rw-r--  2.0 unx     1343 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py
+-rw-rw-r--  2.0 unx     1302 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/models/dmnet_r50-d8.py
+-rw-rw-r--  2.0 unx     1316 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/models/dnl_r50-d8.py
+-rw-rw-r--  2.0 unx     1329 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/models/emanet_r50-d8.py
+-rw-rw-r--  2.0 unx     1435 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/models/encnet_r50-d8.py
+-rw-rw-r--  2.0 unx     1761 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/models/fast_scnn.py
+-rw-rw-r--  2.0 unx     1646 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/models/fcn_hr18.py
+-rw-rw-r--  2.0 unx     1285 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/models/fcn_r50-d8.py
+-rw-rw-r--  2.0 unx     1512 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/models/fcn_unet_s5-d16.py
+-rw-rw-r--  2.0 unx     1056 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/models/fpn_r50.py
+-rw-rw-r--  2.0 unx      977 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/models/fpn_uniformer.py
+-rw-rw-r--  2.0 unx     1326 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/models/gcnet_r50-d8.py
+-rw-rw-r--  2.0 unx      766 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/models/lraspp_m-v3-d8.py
+-rw-rw-r--  2.0 unx     1315 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/models/nonlocal_r50-d8.py
+-rw-rw-r--  2.0 unx     2196 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/models/ocrnet_hr18.py
+-rw-rw-r--  2.0 unx     1385 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/models/ocrnet_r50-d8.py
+-rw-rw-r--  2.0 unx     1704 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/models/pointrend_r50.py
+-rw-rw-r--  2.0 unx     1406 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/models/psanet_r50-d8.py
+-rw-rw-r--  2.0 unx     1271 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/models/pspnet_r50-d8.py
+-rw-rw-r--  2.0 unx     1497 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py
+-rw-rw-r--  2.0 unx     1301 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/models/upernet_r50.py
+-rw-rw-r--  2.0 unx     1235 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/models/upernet_uniformer.py
+-rw-rw-r--  2.0 unx      382 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/schedules/schedule_160k.py
+-rw-rw-r--  2.0 unx      379 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/schedules/schedule_20k.py
+-rw-rw-r--  2.0 unx      379 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/schedules/schedule_40k.py
+-rw-rw-r--  2.0 unx      379 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/configs/_base_/schedules/schedule_80k.py
+-rw-rw-r--  2.0 unx     1316 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/exp/upernet_global_small/config.py
+-rw-rw-r--  2.0 unx     1317 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/exp/upernet_global_small/test_config_g.py
+-rw-rw-r--  2.0 unx     1339 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/exp/upernet_global_small/test_config_h32.py
+-rw-rw-r--  2.0 unx     1339 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/exp/upernet_global_small/test_config_w32.py
+-rw-rw-r--  2.0 unx      352 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/__init__.py
+-rw-rw-r--  2.0 unx     1177 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/version.py
+-rw-rw-r--  2.0 unx      133 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/arraymisc/__init__.py
+-rw-rw-r--  2.0 unx     1824 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/arraymisc/quantization.py
+-rw-rw-r--  2.0 unx     2438 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/cnn/__init__.py
+-rw-rw-r--  2.0 unx     1990 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/cnn/alexnet.py
+-rw-rw-r--  2.0 unx     1089 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/cnn/builder.py
+-rw-rw-r--  2.0 unx     9955 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/cnn/resnet.py
+-rw-rw-r--  2.0 unx     6053 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/cnn/vgg.py
+-rw-rw-r--  2.0 unx     1732 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/__init__.py
+-rw-rw-r--  2.0 unx     2508 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/activation.py
+-rw-rw-r--  2.0 unx     4681 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/context_block.py
+-rw-rw-r--  2.0 unx     1446 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/conv.py
+-rw-rw-r--  2.0 unx     2514 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py
+-rw-rw-r--  2.0 unx     8760 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/conv_module.py
+-rw-rw-r--  2.0 unx     5417 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/conv_ws.py
+-rw-rw-r--  2.0 unx     4142 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py
+-rw-rw-r--  2.0 unx     2172 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/drop.py
+-rw-rw-r--  2.0 unx    15999 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/generalized_attention.py
+-rw-rw-r--  2.0 unx     1097 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/hsigmoid.py
+-rw-rw-r--  2.0 unx      651 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/hswish.py
+-rw-rw-r--  2.0 unx    11012 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/non_local.py
+-rw-rw-r--  2.0 unx     5154 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/norm.py
+-rw-rw-r--  2.0 unx     1127 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/padding.py
+-rw-rw-r--  2.0 unx     2487 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/plugin.py
+-rw-rw-r--  2.0 unx      658 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/registry.py
+-rw-rw-r--  2.0 unx      577 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/scale.py
+-rw-rw-r--  2.0 unx      485 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/swish.py
+-rw-rw-r--  2.0 unx    24639 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/transformer.py
+-rw-rw-r--  2.0 unx     2880 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/upsample.py
+-rw-rw-r--  2.0 unx     6961 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/wrappers.py
+-rw-rw-r--  2.0 unx     1023 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/cnn/utils/__init__.py
+-rw-rw-r--  2.0 unx    22104 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/cnn/utils/flops_counter.py
+-rw-rw-r--  2.0 unx     1881 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/cnn/utils/fuse_conv_bn.py
+-rw-rw-r--  2.0 unx     2327 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/cnn/utils/sync_bn.py
+-rw-rw-r--  2.0 unx    26006 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/cnn/utils/weight_init.py
+-rw-rw-r--  2.0 unx      266 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/engine/__init__.py
+-rw-rw-r--  2.0 unx     7196 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/engine/test.py
+-rw-rw-r--  2.0 unx      478 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/fileio/__init__.py
+-rw-rw-r--  2.0 unx    41933 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/fileio/file_client.py
+-rw-rw-r--  2.0 unx     5520 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/fileio/io.py
+-rw-rw-r--  2.0 unx     3458 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/fileio/parse.py
+-rw-rw-r--  2.0 unx      278 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/fileio/handlers/__init__.py
+-rw-rw-r--  2.0 unx      993 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/fileio/handlers/base.py
+-rw-rw-r--  2.0 unx     1068 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/fileio/handlers/json_handler.py
+-rw-rw-r--  2.0 unx      817 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/fileio/handlers/pickle_handler.py
+-rw-rw-r--  2.0 unx      665 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/fileio/handlers/yaml_handler.py
+-rw-rw-r--  2.0 unx     1725 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/image/__init__.py
+-rw-rw-r--  2.0 unx     9907 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/image/colorspace.py
+-rw-rw-r--  2.0 unx    25196 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/image/geometric.py
+-rw-rw-r--  2.0 unx     9572 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/image/io.py
+-rw-rw-r--  2.0 unx     1410 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/image/misc.py
+-rw-rw-r--  2.0 unx    14999 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/image/photometric.py
+-rw-rw-r--  2.0 unx     4506 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/__init__.py
+-rw-rw-r--  2.0 unx     4344 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/assign_score_withk.py
+-rw-rw-r--  2.0 unx     1695 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/ball_query.py
+-rw-rw-r--  2.0 unx     2508 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/bbox.py
+-rw-rw-r--  2.0 unx     3725 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/border_align.py
+-rw-rw-r--  2.0 unx     1609 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/box_iou_rotated.py
+-rw-rw-r--  2.0 unx     9873 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/carafe.py
+-rw-rw-r--  2.0 unx     3041 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/cc_attention.py
+-rw-rw-r--  2.0 unx     1795 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/contour_expand.py
+-rw-rw-r--  2.0 unx     4697 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/corner_pool.py
+-rw-rw-r--  2.0 unx     6697 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/correlation.py
+-rw-rw-r--  2.0 unx    15603 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/deform_conv.py
+-rw-rw-r--  2.0 unx     7410 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/deform_roi_pool.py
+-rw-rw-r--  2.0 unx     1467 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/deprecated_wrappers.py
+-rw-rw-r--  2.0 unx     6582 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/focal_loss.py
+-rw-rw-r--  2.0 unx     2550 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/furthest_point_sample.py
+-rw-rw-r--  2.0 unx    10031 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/fused_bias_leakyrelu.py
+-rw-rw-r--  2.0 unx     1607 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/gather_points.py
+-rw-rw-r--  2.0 unx     8135 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/group_points.py
+-rw-rw-r--  2.0 unx      887 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/info.py
+-rw-rw-r--  2.0 unx     2988 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/iou3d.py
+-rw-rw-r--  2.0 unx     2599 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/knn.py
+-rw-rw-r--  2.0 unx     3761 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/masked_conv.py
+-rw-rw-r--  2.0 unx     5403 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/merge_cells.py
+-rw-rw-r--  2.0 unx    10574 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/modulated_deform_conv.py
+-rw-rw-r--  2.0 unx    15175 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/multi_scale_deform_attn.py
+-rw-rw-r--  2.0 unx    16237 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/nms.py
+-rw-rw-r--  2.0 unx     3113 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/pixel_group.py
+-rw-rw-r--  2.0 unx    12291 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/point_sample.py
+-rw-rw-r--  2.0 unx     5241 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/points_in_boxes.py
+-rw-rw-r--  2.0 unx     6063 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/points_sampler.py
+-rw-rw-r--  2.0 unx     2773 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/psa_mask.py
+-rw-rw-r--  2.0 unx     8519 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/roi_align.py
+-rw-rw-r--  2.0 unx     6434 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/roi_align_rotated.py
+-rw-rw-r--  2.0 unx     2517 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/roi_pool.py
+-rw-rw-r--  2.0 unx     4256 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/roiaware_pool3d.py
+-rw-rw-r--  2.0 unx     2990 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/roipoint_pool3d.py
+-rw-rw-r--  2.0 unx     5804 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/saconv.py
+-rw-rw-r--  2.0 unx     5201 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/scatter_points.py
+-rw-rw-r--  2.0 unx    11267 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/sync_bn.py
+-rw-rw-r--  2.0 unx     2147 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/three_interpolate.py
+-rw-rw-r--  2.0 unx     1515 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/three_nn.py
+-rw-rw-r--  2.0 unx     2141 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/tin_shift.py
+-rw-rw-r--  2.0 unx    11804 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/upfirdn2d.py
+-rw-rw-r--  2.0 unx     5286 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/ops/voxelize.py
+-rw-rw-r--  2.0 unx      505 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/parallel/__init__.py
+-rw-rw-r--  2.0 unx     2830 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/parallel/_functions.py
+-rw-rw-r--  2.0 unx     3665 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/parallel/collate.py
+-rw-rw-r--  2.0 unx     2365 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/parallel/data_container.py
+-rw-rw-r--  2.0 unx     3912 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/parallel/data_parallel.py
+-rw-rw-r--  2.0 unx     4857 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/parallel/distributed.py
+-rw-rw-r--  2.0 unx     2837 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/parallel/distributed_deprecated.py
+-rw-rw-r--  2.0 unx      332 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/parallel/registry.py
+-rw-rw-r--  2.0 unx     2307 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/parallel/scatter_gather.py
+-rw-rw-r--  2.0 unx      708 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/parallel/utils.py
+-rw-rw-r--  2.0 unx     2859 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/__init__.py
+-rw-rw-r--  2.0 unx     7502 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/base_module.py
+-rw-rw-r--  2.0 unx    20846 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/base_runner.py
+-rw-rw-r--  2.0 unx      666 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/builder.py
+-rw-rw-r--  2.0 unx    25136 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/checkpoint.py
+-rw-rw-r--  2.0 unx     1928 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/default_constructor.py
+-rw-rw-r--  2.0 unx     5395 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/dist_utils.py
+-rw-rw-r--  2.0 unx     7565 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/epoch_based_runner.py
+-rw-rw-r--  2.0 unx    15784 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/fp16_utils.py
+-rw-rw-r--  2.0 unx    11062 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/iter_based_runner.py
+-rw-rw-r--  2.0 unx     1192 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/log_buffer.py
+-rw-rw-r--  2.0 unx     1598 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/priority.py
+-rw-rw-r--  2.0 unx     2936 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/utils.py
+-rw-rw-r--  2.0 unx     1396 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/__init__.py
+-rw-rw-r--  2.0 unx     7317 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/checkpoint.py
+-rw-rw-r--  2.0 unx      269 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/closure.py
+-rw-rw-r--  2.0 unx     3599 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/ema.py
+-rw-rw-r--  2.0 unx    22448 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/evaluation.py
+-rw-rw-r--  2.0 unx     2761 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/hook.py
+-rw-rw-r--  2.0 unx      446 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/iter_timer.py
+-rw-rw-r--  2.0 unx    26034 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/lr_updater.py
+-rw-rw-r--  2.0 unx      657 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/memory.py
+-rw-rw-r--  2.0 unx    21296 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/momentum_updater.py
+-rw-rw-r--  2.0 unx    21654 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/optimizer.py
+-rw-rw-r--  2.0 unx     8041 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/profiler.py
+-rw-rw-r--  2.0 unx      847 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/sampler_seed.py
+-rw-rw-r--  2.0 unx      707 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/sync_buffer.py
+-rw-rw-r--  2.0 unx      522 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/logger/__init__.py
+-rw-rw-r--  2.0 unx     5451 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/logger/base.py
+-rw-rw-r--  2.0 unx     1761 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/logger/dvclive.py
+-rw-rw-r--  2.0 unx     2838 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/logger/mlflow.py
+-rw-rw-r--  2.0 unx     3077 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/logger/neptune.py
+-rw-rw-r--  2.0 unx     4378 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/logger/pavi.py
+-rw-rw-r--  2.0 unx     2077 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/logger/tensorboard.py
+-rw-rw-r--  2.0 unx    10684 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/logger/text.py
+-rw-rw-r--  2.0 unx     1694 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/logger/wandb.py
+-rw-rw-r--  2.0 unx      370 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/optimizer/__init__.py
+-rw-rw-r--  2.0 unx     1346 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/optimizer/builder.py
+-rw-rw-r--  2.0 unx    11803 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/runner/optimizer/default_constructor.py
+-rw-rw-r--  2.0 unx     3915 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/utils/__init__.py
+-rw-rw-r--  2.0 unx    26263 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/utils/config.py
+-rw-rw-r--  2.0 unx     3367 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/utils/env.py
+-rw-rw-r--  2.0 unx     2021 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/utils/ext_loader.py
+-rw-rw-r--  2.0 unx     3986 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/utils/logging.py
+-rw-rw-r--  2.0 unx    11447 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/utils/misc.py
+-rw-rw-r--  2.0 unx      899 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/utils/parrots_jit.py
+-rw-rw-r--  2.0 unx     3536 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/utils/parrots_wrapper.py
+-rw-rw-r--  2.0 unx     3414 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/utils/path.py
+-rw-rw-r--  2.0 unx     7105 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/utils/progressbar.py
+-rw-rw-r--  2.0 unx    11041 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/utils/registry.py
+-rw-rw-r--  2.0 unx     4289 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/utils/testing.py
+-rw-rw-r--  2.0 unx     2993 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/utils/timer.py
+-rw-rw-r--  2.0 unx      795 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/utils/trace.py
+-rw-rw-r--  2.0 unx     2673 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/utils/version_utils.py
+-rw-rw-r--  2.0 unx      570 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/video/__init__.py
+-rw-rw-r--  2.0 unx    10209 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/video/io.py
+-rw-rw-r--  2.0 unx     9728 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/video/optflow.py
+-rw-rw-r--  2.0 unx     5291 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/video/processing.py
+-rw-rw-r--  2.0 unx      338 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/visualization/__init__.py
+-rw-rw-r--  2.0 unx     1381 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/visualization/color.py
+-rw-rw-r--  2.0 unx     5145 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/visualization/image.py
+-rw-rw-r--  2.0 unx     3389 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv/visualization/optflow.py
+-rw-rw-r--  2.0 unx       95 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv_custom/__init__.py
+-rw-rw-r--  2.0 unx    19091 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmcv_custom/checkpoint.py
+-rw-rw-r--  2.0 unx      381 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/apis/__init__.py
+-rw-rw-r--  2.0 unx     4729 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/apis/inference.py
+-rw-rw-r--  2.0 unx     8288 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/apis/test.py
+-rw-rw-r--  2.0 unx     4035 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/apis/train.py
+-rw-rw-r--  2.0 unx      126 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/core/__init__.py
+-rw-rw-r--  2.0 unx      301 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/core/evaluation/__init__.py
+-rw-rw-r--  2.0 unx     7305 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/core/evaluation/class_names.py
+-rw-rw-r--  2.0 unx     3873 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/core/evaluation/eval_hooks.py
+-rw-rw-r--  2.0 unx    13079 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/core/evaluation/metrics.py
+-rw-rw-r--  2.0 unx      172 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/core/seg/__init__.py
+-rw-rw-r--  2.0 unx      273 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/core/seg/builder.py
+-rw-rw-r--  2.0 unx      150 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/core/seg/sampler/__init__.py
+-rw-rw-r--  2.0 unx      284 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/core/seg/sampler/base_pixel_sampler.py
+-rw-rw-r--  2.0 unx     3155 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py
+-rw-rw-r--  2.0 unx       55 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/core/utils/__init__.py
+-rw-rw-r--  2.0 unx      371 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/core/utils/misc.py
+-rw-rw-r--  2.0 unx      798 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/datasets/__init__.py
+-rw-rw-r--  2.0 unx     5185 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/datasets/ade.py
+-rw-rw-r--  2.0 unx     5951 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/datasets/builder.py
+-rw-rw-r--  2.0 unx      781 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/datasets/chase_db1.py
+-rw-rw-r--  2.0 unx     8494 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/datasets/cityscapes.py
+-rw-rw-r--  2.0 unx    14882 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/datasets/custom.py
+-rw-rw-r--  2.0 unx     1499 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/datasets/dataset_wrappers.py
+-rw-rw-r--  2.0 unx      771 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/datasets/drive.py
+-rw-rw-r--  2.0 unx      747 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/datasets/hrf.py
+-rw-rw-r--  2.0 unx     5202 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/datasets/pascal_context.py
+-rw-rw-r--  2.0 unx      761 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/datasets/stare.py
+-rw-rw-r--  2.0 unx     1130 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/datasets/voc.py
+-rw-rw-r--  2.0 unx      813 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/datasets/pipelines/__init__.py
+-rw-rw-r--  2.0 unx     1484 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/datasets/pipelines/compose.py
+-rw-rw-r--  2.0 unx     9276 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/datasets/pipelines/formating.py
+-rw-rw-r--  2.0 unx     5901 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/datasets/pipelines/loading.py
+-rw-rw-r--  2.0 unx     5201 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/datasets/pipelines/test_time_aug.py
+-rw-rw-r--  2.0 unx    30993 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/datasets/pipelines/transforms.py
+-rw-rw-r--  2.0 unx      489 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/__init__.py
+-rw-rw-r--  2.0 unx     1205 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/builder.py
+-rw-rw-r--  2.0 unx      532 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/backbones/__init__.py
+-rw-rw-r--  2.0 unx    13183 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/backbones/cgnet.py
+-rw-rw-r--  2.0 unx    14436 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/backbones/fast_scnn.py
+-rw-rw-r--  2.0 unx    21226 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/backbones/hrnet.py
+-rw-rw-r--  2.0 unx     6981 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/backbones/mobilenet_v2.py
+-rw-rw-r--  2.0 unx    10390 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/backbones/mobilenet_v3.py
+-rw-rw-r--  2.0 unx    10110 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/backbones/resnest.py
+-rw-rw-r--  2.0 unx    24310 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/backbones/resnet.py
+-rw-rw-r--  2.0 unx     5161 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/backbones/resnext.py
+-rw-rw-r--  2.0 unx    18269 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/backbones/unet.py
+-rw-rw-r--  2.0 unx    18476 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/backbones/uniformer.py
+-rw-rw-r--  2.0 unx    18085 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/backbones/vit.py
+-rw-rw-r--  2.0 unx      969 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/__init__.py
+-rw-rw-r--  2.0 unx     9194 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/ann_head.py
+-rw-rw-r--  2.0 unx     5572 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/apc_head.py
+-rw-rw-r--  2.0 unx     3459 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/aspp_head.py
+-rw-rw-r--  2.0 unx     2351 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/cascade_decode_head.py
+-rw-rw-r--  2.0 unx     1303 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/cc_head.py
+-rw-rw-r--  2.0 unx     5585 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/da_head.py
+-rw-rw-r--  2.0 unx     9240 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/decode_head.py
+-rw-rw-r--  2.0 unx     5004 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/dm_head.py
+-rw-rw-r--  2.0 unx     4591 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/dnl_head.py
+-rw-rw-r--  2.0 unx     5796 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/ema_head.py
+-rw-rw-r--  2.0 unx     6784 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/enc_head.py
+-rw-rw-r--  2.0 unx     2817 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/fcn_head.py
+-rw-rw-r--  2.0 unx     2422 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/fpn_head.py
+-rw-rw-r--  2.0 unx     1611 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/gc_head.py
+-rw-rw-r--  2.0 unx     3098 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/lraspp_head.py
+-rw-rw-r--  2.0 unx     1577 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/nl_head.py
+-rw-rw-r--  2.0 unx     4319 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/ocr_head.py
+-rw-rw-r--  2.0 unx    14754 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/point_head.py
+-rw-rw-r--  2.0 unx     7544 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/psa_head.py
+-rw-rw-r--  2.0 unx     3352 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/psp_head.py
+-rw-rw-r--  2.0 unx     3527 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/sep_aspp_head.py
+-rw-rw-r--  2.0 unx     2024 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/sep_fcn_head.py
+-rw-rw-r--  2.0 unx     4012 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/uper_head.py
+-rw-rw-r--  2.0 unx      529 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/losses/__init__.py
+-rw-rw-r--  2.0 unx     2970 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/losses/accuracy.py
+-rw-rw-r--  2.0 unx     7437 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/losses/cross_entropy_loss.py
+-rw-rw-r--  2.0 unx     4239 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/losses/dice_loss.py
+-rw-rw-r--  2.0 unx    11419 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/losses/lovasz_loss.py
+-rw-rw-r--  2.0 unx     3718 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/losses/utils.py
+-rw-rw-r--  2.0 unx      102 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/necks/__init__.py
+-rw-rw-r--  2.0 unx     9159 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/necks/fpn.py
+-rw-rw-r--  2.0 unx     2454 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/necks/multilevel_neck.py
+-rw-rw-r--  2.0 unx      207 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/segmentors/__init__.py
+-rw-rw-r--  2.0 unx    10398 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/segmentors/base.py
+-rw-rw-r--  2.0 unx     3708 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py
+-rw-rw-r--  2.0 unx    11344 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/segmentors/encoder_decoder.py
+-rw-rw-r--  2.0 unx      502 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/utils/__init__.py
+-rw-rw-r--  2.0 unx     1015 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/utils/drop.py
+-rw-rw-r--  2.0 unx     7025 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/utils/inverted_residual.py
+-rw-rw-r--  2.0 unx     1231 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/utils/make_divisible.py
+-rw-rw-r--  2.0 unx     3335 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/utils/res_layer.py
+-rw-rw-r--  2.0 unx     2151 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/utils/se_layer.py
+-rw-rw-r--  2.0 unx     6145 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/utils/self_attention_block.py
+-rw-rw-r--  2.0 unx     3988 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/utils/up_conv_block.py
+-rw-rw-r--  2.0 unx     2327 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/models/utils/weight_init.py
+-rw-rw-r--  2.0 unx      116 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/ops/__init__.py
+-rw-rw-r--  2.0 unx     2788 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/ops/encoding.py
+-rw-rw-r--  2.0 unx     1827 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/ops/wrappers.py
+-rw-rw-r--  2.0 unx      119 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/utils/__init__.py
+-rw-rw-r--  2.0 unx      505 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/utils/collect_env.py
+-rw-rw-r--  2.0 unx      919 b- defN 24-May-09 20:37 build/lib/lavis/common/annotator/uniformer/mmseg/utils/logger.py
+-rw-rw-r--  2.0 unx      246 b- defN 24-May-09 20:37 build/lib/lavis/common/vqa_tools/__init__.py
+-rw-rw-r--  2.0 unx     8634 b- defN 24-May-09 20:37 build/lib/lavis/common/vqa_tools/vqa.py
+-rw-rw-r--  2.0 unx    11016 b- defN 24-May-09 20:37 build/lib/lavis/common/vqa_tools/vqa_eval.py
+-rw-rw-r--  2.0 unx    11995 b- defN 24-May-09 20:37 build/lib/lavis/datasets/data_utils.py
+-rw-rw-r--  2.0 unx     7773 b- defN 24-May-09 20:37 build/lib/lavis/datasets/builders/__init__.py
+-rw-rw-r--  2.0 unx     3881 b- defN 24-May-09 20:37 build/lib/lavis/datasets/builders/audio_caption_builder.py
+-rw-rw-r--  2.0 unx      968 b- defN 24-May-09 20:37 build/lib/lavis/datasets/builders/audio_qa_builder.py
+-rw-rw-r--  2.0 unx    11771 b- defN 24-May-09 20:37 build/lib/lavis/datasets/builders/base_dataset_builder.py
+-rw-rw-r--  2.0 unx    10617 b- defN 24-May-09 20:37 build/lib/lavis/datasets/builders/caption_builder.py
+-rw-rw-r--  2.0 unx     3189 b- defN 24-May-09 20:37 build/lib/lavis/datasets/builders/classification_builder.py
+-rw-rw-r--  2.0 unx     2467 b- defN 24-May-09 20:37 build/lib/lavis/datasets/builders/dialogue_builder.py
+-rw-rw-r--  2.0 unx      988 b- defN 24-May-09 20:37 build/lib/lavis/datasets/builders/discrn_builders.py
+-rw-rw-r--  2.0 unx     3917 b- defN 24-May-09 20:37 build/lib/lavis/datasets/builders/image_text_pair_builder.py
+-rw-rw-r--  2.0 unx    20539 b- defN 24-May-09 20:37 build/lib/lavis/datasets/builders/imagefolder_builder.py
+-rw-rw-r--  2.0 unx     2349 b- defN 24-May-09 20:37 build/lib/lavis/datasets/builders/object3d_caption_builder.py
+-rw-rw-r--  2.0 unx      784 b- defN 24-May-09 20:37 build/lib/lavis/datasets/builders/object3d_classification_builder.py
+-rw-rw-r--  2.0 unx      712 b- defN 24-May-09 20:37 build/lib/lavis/datasets/builders/object3d_qa_builder.py
+-rw-rw-r--  2.0 unx     1579 b- defN 24-May-09 20:37 build/lib/lavis/datasets/builders/retrieval_builder.py
+-rw-rw-r--  2.0 unx     1255 b- defN 24-May-09 20:37 build/lib/lavis/datasets/builders/text_to_image_generation_builder.py
+-rw-rw-r--  2.0 unx     2632 b- defN 24-May-09 20:37 build/lib/lavis/datasets/builders/video_qa_builder.py
+-rw-rw-r--  2.0 unx     5581 b- defN 24-May-09 20:37 build/lib/lavis/datasets/builders/vqa_builder.py
+-rw-rw-r--  2.0 unx     5344 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/aok_vqa_datasets.py
+-rw-rw-r--  2.0 unx    17282 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/audio_captioning_datasets.py
+-rw-rw-r--  2.0 unx     3468 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/audio_classification_datasets.py
+-rw-rw-r--  2.0 unx     4832 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/audio_qa_datasets.py
+-rw-rw-r--  2.0 unx     8472 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/avsd_dialogue_datasets.py
+-rw-rw-r--  2.0 unx     3387 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/base_dataset.py
+-rw-rw-r--  2.0 unx     1899 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/capfilt_dataset.py
+-rw-rw-r--  2.0 unx     2880 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/caption_datasets.py
+-rw-rw-r--  2.0 unx     2167 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/coco_caption_datasets.py
+-rw-rw-r--  2.0 unx     3607 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/coco_vqa_datasets.py
+-rw-rw-r--  2.0 unx     5330 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/dataloader_utils.py
+-rw-rw-r--  2.0 unx     4225 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/dialogue_datasets.py
+-rw-rw-r--  2.0 unx     8778 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/discriminatory_reasoning_datasets.py
+-rw-rw-r--  2.0 unx     3315 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/gqa_datasets.py
+-rw-rw-r--  2.0 unx     4613 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/iconqa_datasets.py
+-rw-rw-r--  2.0 unx     1807 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/image_text_pair_datasets.py
+-rw-rw-r--  2.0 unx     1669 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/imagefolder_dataset.py
+-rw-rw-r--  2.0 unx     2600 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/laion_dataset.py
+-rw-rw-r--  2.0 unx     1370 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/llava150k_dataset.py
+-rw-rw-r--  2.0 unx      624 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/multimodal_classification_datasets.py
+-rw-rw-r--  2.0 unx     3098 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/music_avqa.py
+-rw-rw-r--  2.0 unx     2850 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/nlvr_datasets.py
+-rw-rw-r--  2.0 unx     6997 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/object3d_captioning_datasets.py
+-rw-rw-r--  2.0 unx     6068 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/object3d_classification_datasets.py
+-rw-rw-r--  2.0 unx     2948 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/object3d_qa_datasets.py
+-rw-rw-r--  2.0 unx     2327 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/ocr_datasets.py
+-rw-rw-r--  2.0 unx     5123 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/retrieval_datasets.py
+-rw-rw-r--  2.0 unx     2461 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/snli_ve_datasets.py
+-rw-rw-r--  2.0 unx     2190 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/subject_driven_t2i_dataset.py
+-rw-rw-r--  2.0 unx     2392 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/textcaps_datasets.py
+-rw-rw-r--  2.0 unx     3439 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/valor_caption.py
+-rw-rw-r--  2.0 unx     3230 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/vatex_captioning_datasets.py
+-rw-rw-r--  2.0 unx     1438 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/vg_vqa_datasets.py
+-rw-rw-r--  2.0 unx     5929 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/video_caption_datasets.py
+-rw-rw-r--  2.0 unx     2482 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/video_vqa_datasets.py
+-rw-rw-r--  2.0 unx     3900 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/violin_dataset.py
+-rw-rw-r--  2.0 unx     4682 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/visdial_dialogue_datasets.py
+-rw-rw-r--  2.0 unx     1953 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/vizwiz_vqa_datasets.py
+-rw-rw-r--  2.0 unx     2589 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/vlep_dataset.py
+-rw-rw-r--  2.0 unx     1739 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/vqa_datasets.py
+-rw-rw-r--  2.0 unx     3502 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/vsr_datasets.py
+-rw-rw-r--  2.0 unx     3011 b- defN 24-May-09 20:37 build/lib/lavis/datasets/datasets/yt8m_video_dialogue_datasets.py
+-rw-rw-r--  2.0 unx      813 b- defN 24-May-09 20:37 build/lib/lavis/datasets/download_scripts/download_charade.py
+-rw-rw-r--  2.0 unx     1782 b- defN 24-May-09 20:37 build/lib/lavis/datasets/download_scripts/download_coco.py
+-rw-rw-r--  2.0 unx     1826 b- defN 24-May-09 20:37 build/lib/lavis/datasets/download_scripts/download_coin.py
+-rw-rw-r--  2.0 unx     1978 b- defN 24-May-09 20:37 build/lib/lavis/datasets/download_scripts/download_didemo.py
+-rw-rw-r--  2.0 unx     1939 b- defN 24-May-09 20:37 build/lib/lavis/datasets/download_scripts/download_flickr.py
+-rw-rw-r--  2.0 unx     1370 b- defN 24-May-09 20:37 build/lib/lavis/datasets/download_scripts/download_gqa.py
+-rw-rw-r--  2.0 unx     1089 b- defN 24-May-09 20:37 build/lib/lavis/datasets/download_scripts/download_iconqa.py
+-rw-rw-r--  2.0 unx     3179 b- defN 24-May-09 20:37 build/lib/lavis/datasets/download_scripts/download_msrvtt.py
+-rw-rw-r--  2.0 unx     1810 b- defN 24-May-09 20:37 build/lib/lavis/datasets/download_scripts/download_msvd.py
+-rw-rw-r--  2.0 unx     3962 b- defN 24-May-09 20:37 build/lib/lavis/datasets/download_scripts/download_nocaps.py
+-rw-rw-r--  2.0 unx     2341 b- defN 24-May-09 20:37 build/lib/lavis/datasets/download_scripts/download_sbu.py
+-rw-rw-r--  2.0 unx     1514 b- defN 24-May-09 20:37 build/lib/lavis/datasets/download_scripts/download_vg.py
+-rw-rw-r--  2.0 unx      608 b- defN 24-May-09 20:37 build/lib/lavis/datasets/download_scripts/download_violin.py
+-rw-rw-r--  2.0 unx     6597 b- defN 24-May-09 20:37 build/lib/lavis/datasets/download_scripts/DownloadConceptualCaptions/download_data_cc12m.py
+-rw-rw-r--  2.0 unx     6546 b- defN 24-May-09 20:37 build/lib/lavis/datasets/download_scripts/DownloadConceptualCaptions/download_data_cc3m.py
+-rw-rw-r--  2.0 unx     8440 b- defN 24-May-09 20:37 build/lib/lavis/models/__init__.py
+-rw-rw-r--  2.0 unx     8638 b- defN 24-May-09 20:37 build/lib/lavis/models/base_model.py
+-rw-rw-r--  2.0 unx     1624 b- defN 24-May-09 20:37 build/lib/lavis/models/beats_encoder.py
+-rw-rw-r--  2.0 unx    10106 b- defN 24-May-09 20:37 build/lib/lavis/models/clip_vit.py
+-rw-rw-r--  2.0 unx    20008 b- defN 24-May-09 20:37 build/lib/lavis/models/eva_vit.py
+-rw-rw-r--  2.0 unx    54570 b- defN 24-May-09 20:37 build/lib/lavis/models/med.py
+-rw-rw-r--  2.0 unx    19740 b- defN 24-May-09 20:37 build/lib/lavis/models/vit.py
+-rw-rw-r--  2.0 unx     7181 b- defN 24-May-09 20:37 build/lib/lavis/models/albef_models/__init__.py
+-rw-rw-r--  2.0 unx     5910 b- defN 24-May-09 20:37 build/lib/lavis/models/albef_models/albef_classification.py
+-rw-rw-r--  2.0 unx     7564 b- defN 24-May-09 20:37 build/lib/lavis/models/albef_models/albef_feature_extractor.py
+-rw-rw-r--  2.0 unx     9516 b- defN 24-May-09 20:37 build/lib/lavis/models/albef_models/albef_nlvr.py
+-rw-rw-r--  2.0 unx     3236 b- defN 24-May-09 20:37 build/lib/lavis/models/albef_models/albef_outputs.py
+-rw-rw-r--  2.0 unx    14875 b- defN 24-May-09 20:37 build/lib/lavis/models/albef_models/albef_pretrain.py
+-rw-rw-r--  2.0 unx    12731 b- defN 24-May-09 20:37 build/lib/lavis/models/albef_models/albef_retrieval.py
+-rw-rw-r--  2.0 unx    17038 b- defN 24-May-09 20:37 build/lib/lavis/models/albef_models/albef_vqa.py
+-rw-rw-r--  2.0 unx     3673 b- defN 24-May-09 20:37 build/lib/lavis/models/alpro_models/__init__.py
+-rw-rw-r--  2.0 unx     1664 b- defN 24-May-09 20:37 build/lib/lavis/models/alpro_models/alpro_outputs.py
+-rw-rw-r--  2.0 unx     4457 b- defN 24-May-09 20:37 build/lib/lavis/models/alpro_models/alpro_qa.py
+-rw-rw-r--  2.0 unx    14417 b- defN 24-May-09 20:37 build/lib/lavis/models/alpro_models/alpro_retrieval.py
+-rw-rw-r--  2.0 unx     6926 b- defN 24-May-09 20:37 build/lib/lavis/models/beats/BEATs.py
+-rw-rw-r--  2.0 unx     6468 b- defN 24-May-09 20:37 build/lib/lavis/models/beats/Tokenizers.py
+-rw-rw-r--  2.0 unx    30762 b- defN 24-May-09 20:37 build/lib/lavis/models/beats/backbone.py
+-rw-rw-r--  2.0 unx     7387 b- defN 24-May-09 20:37 build/lib/lavis/models/beats/modules.py
+-rw-rw-r--  2.0 unx     8172 b- defN 24-May-09 20:37 build/lib/lavis/models/beats/quantizer.py
+-rw-rw-r--  2.0 unx    48386 b- defN 24-May-09 20:37 build/lib/lavis/models/blip2_models/Qformer.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-May-09 20:37 build/lib/lavis/models/blip2_models/__init__.py
+-rw-rw-r--  2.0 unx    11260 b- defN 24-May-09 20:37 build/lib/lavis/models/blip2_models/blip2.py
+-rw-rw-r--  2.0 unx     3945 b- defN 24-May-09 20:37 build/lib/lavis/models/blip2_models/blip2_image_text_matching.py
+-rw-rw-r--  2.0 unx    15863 b- defN 24-May-09 20:37 build/lib/lavis/models/blip2_models/blip2_opt.py
+-rw-rw-r--  2.0 unx    20633 b- defN 24-May-09 20:37 build/lib/lavis/models/blip2_models/blip2_qformer.py
+-rw-rw-r--  2.0 unx    13665 b- defN 24-May-09 20:37 build/lib/lavis/models/blip2_models/blip2_t5.py
+-rw-rw-r--  2.0 unx    30599 b- defN 24-May-09 20:37 build/lib/lavis/models/blip2_models/blip2_t5_instruct.py
+-rw-rw-r--  2.0 unx    28892 b- defN 24-May-09 20:37 build/lib/lavis/models/blip2_models/blip2_vicuna_instruct.py
+-rw-rw-r--  2.0 unx   138338 b- defN 24-May-09 20:37 build/lib/lavis/models/blip2_models/blip2_vicuna_xinstruct.py
+-rw-rw-r--  2.0 unx    39363 b- defN 24-May-09 20:37 build/lib/lavis/models/blip2_models/modeling_llama.py
+-rw-rw-r--  2.0 unx    47286 b- defN 24-May-09 20:37 build/lib/lavis/models/blip2_models/modeling_opt.py
+-rw-rw-r--  2.0 unx    86219 b- defN 24-May-09 20:37 build/lib/lavis/models/blip2_models/modeling_t5.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-May-09 20:37 build/lib/lavis/models/blip_diffusion_models/__init__.py
+-rw-rw-r--  2.0 unx    33706 b- defN 24-May-09 20:37 build/lib/lavis/models/blip_diffusion_models/blip_diffusion.py
+-rw-rw-r--  2.0 unx     8775 b- defN 24-May-09 20:37 build/lib/lavis/models/blip_diffusion_models/modeling_ctx_clip.py
+-rw-rw-r--  2.0 unx    22314 b- defN 24-May-09 20:37 build/lib/lavis/models/blip_diffusion_models/ptp_utils.py
+-rw-rw-r--  2.0 unx     3332 b- defN 24-May-09 20:37 build/lib/lavis/models/blip_diffusion_models/utils.py
+-rw-rw-r--  2.0 unx     3916 b- defN 24-May-09 20:37 build/lib/lavis/models/blip_models/__init__.py
+-rw-rw-r--  2.0 unx     2566 b- defN 24-May-09 20:37 build/lib/lavis/models/blip_models/blip.py
+-rw-rw-r--  2.0 unx     8732 b- defN 24-May-09 20:37 build/lib/lavis/models/blip_models/blip_caption.py
+-rw-rw-r--  2.0 unx     5773 b- defN 24-May-09 20:37 build/lib/lavis/models/blip_models/blip_classification.py
+-rw-rw-r--  2.0 unx     7902 b- defN 24-May-09 20:37 build/lib/lavis/models/blip_models/blip_feature_extractor.py
+-rw-rw-r--  2.0 unx     7444 b- defN 24-May-09 20:37 build/lib/lavis/models/blip_models/blip_image_text_matching.py
+-rw-rw-r--  2.0 unx     7091 b- defN 24-May-09 20:37 build/lib/lavis/models/blip_models/blip_nlvr.py
+-rw-rw-r--  2.0 unx     4276 b- defN 24-May-09 20:37 build/lib/lavis/models/blip_models/blip_outputs.py
+-rw-rw-r--  2.0 unx    14988 b- defN 24-May-09 20:37 build/lib/lavis/models/blip_models/blip_pretrain.py
+-rw-rw-r--  2.0 unx    14591 b- defN 24-May-09 20:37 build/lib/lavis/models/blip_models/blip_retrieval.py
+-rw-rw-r--  2.0 unx    14250 b- defN 24-May-09 20:37 build/lib/lavis/models/blip_models/blip_vqa.py
+-rw-rw-r--  2.0 unx    38056 b- defN 24-May-09 20:37 build/lib/lavis/models/blip_models/nlvr_encoder.py
+-rw-rw-r--  2.0 unx      462 b- defN 24-May-09 20:37 build/lib/lavis/models/clip_models/__init__.py
+-rw-rw-r--  2.0 unx     1345 b- defN 24-May-09 20:37 build/lib/lavis/models/clip_models/clip_outputs.py
+-rw-rw-r--  2.0 unx     5165 b- defN 24-May-09 20:37 build/lib/lavis/models/clip_models/loss.py
+-rw-rw-r--  2.0 unx    43435 b- defN 24-May-09 20:37 build/lib/lavis/models/clip_models/model.py
+-rw-rw-r--  2.0 unx     6937 b- defN 24-May-09 20:37 build/lib/lavis/models/clip_models/pretrained.py
+-rw-rw-r--  2.0 unx    19038 b- defN 24-May-09 20:37 build/lib/lavis/models/clip_models/timm_model.py
+-rw-rw-r--  2.0 unx     6673 b- defN 24-May-09 20:37 build/lib/lavis/models/clip_models/tokenizer.py
+-rw-rw-r--  2.0 unx     3292 b- defN 24-May-09 20:37 build/lib/lavis/models/clip_models/transform.py
+-rw-rw-r--  2.0 unx     2138 b- defN 24-May-09 20:37 build/lib/lavis/models/clip_models/utils.py
+-rw-rw-r--  2.0 unx     3902 b- defN 24-May-09 20:37 build/lib/lavis/models/gpt_models/gpt_dialogue.py
+-rw-rw-r--  2.0 unx      238 b- defN 24-May-09 20:37 build/lib/lavis/models/img2prompt_models/__init__.py
+-rw-rw-r--  2.0 unx    24631 b- defN 24-May-09 20:42 build/lib/lavis/models/img2prompt_models/img2prompt_vqa.py
+-rw-rw-r--  2.0 unx     1251 b- defN 24-May-09 20:37 build/lib/lavis/models/pnp_vqa_models/__init__.py
+-rw-rw-r--  2.0 unx     3113 b- defN 24-May-09 20:37 build/lib/lavis/models/pnp_vqa_models/pnp_unifiedqav2_fid.py
+-rw-rw-r--  2.0 unx    16521 b- defN 24-May-09 20:37 build/lib/lavis/models/pnp_vqa_models/pnp_vqa.py
+-rw-rw-r--  2.0 unx      280 b- defN 24-May-09 20:37 build/lib/lavis/models/timesformer/__init__.py
+-rw-rw-r--  2.0 unx     3621 b- defN 24-May-09 20:37 build/lib/lavis/models/timesformer/conv2d_same.py
+-rw-rw-r--  2.0 unx    12320 b- defN 24-May-09 20:37 build/lib/lavis/models/timesformer/features.py
+-rw-rw-r--  2.0 unx    15418 b- defN 24-May-09 20:37 build/lib/lavis/models/timesformer/helpers.py
+-rw-rw-r--  2.0 unx      702 b- defN 24-May-09 20:37 build/lib/lavis/models/timesformer/linear.py
+-rw-rw-r--  2.0 unx    20265 b- defN 24-May-09 20:37 build/lib/lavis/models/timesformer/vit.py
+-rw-rw-r--  2.0 unx     6686 b- defN 24-May-09 20:37 build/lib/lavis/models/timesformer/vit_utils.py
+-rw-rw-r--  2.0 unx     9903 b- defN 24-May-09 20:37 build/lib/lavis/models/ulip_models/ULIP_models.py
+-rw-rw-r--  2.0 unx     2524 b- defN 24-May-09 20:37 build/lib/lavis/models/ulip_models/losses.py
+-rw-rw-r--  2.0 unx     3910 b- defN 24-May-09 20:37 build/lib/lavis/models/ulip_models/pointbert/checkpoint.py
+-rw-rw-r--  2.0 unx    13216 b- defN 24-May-09 20:37 build/lib/lavis/models/ulip_models/pointbert/dvae.py
+-rw-rw-r--  2.0 unx     4922 b- defN 24-May-09 20:37 build/lib/lavis/models/ulip_models/pointbert/logger.py
+-rw-rw-r--  2.0 unx     9292 b- defN 24-May-09 20:37 build/lib/lavis/models/ulip_models/pointbert/misc.py
+-rw-rw-r--  2.0 unx     8783 b- defN 24-May-09 20:37 build/lib/lavis/models/ulip_models/pointbert/point_encoder.py
+-rw-rw-r--  2.0 unx      242 b- defN 24-May-09 20:37 build/lib/lavis/models/ulip_models/utils/__init__.py
+-rw-rw-r--  2.0 unx      362 b- defN 24-May-09 20:37 build/lib/lavis/models/ulip_models/utils/build.py
+-rw-rw-r--  2.0 unx     2360 b- defN 24-May-09 20:37 build/lib/lavis/models/ulip_models/utils/config.py
+-rw-rw-r--  2.0 unx     1280 b- defN 24-May-09 20:37 build/lib/lavis/models/ulip_models/utils/io.py
+-rw-rw-r--  2.0 unx     4922 b- defN 24-May-09 20:37 build/lib/lavis/models/ulip_models/utils/logger.py
+-rw-rw-r--  2.0 unx    10818 b- defN 24-May-09 20:37 build/lib/lavis/models/ulip_models/utils/registry.py
+-rw-rw-r--  2.0 unx     5301 b- defN 24-May-09 20:37 build/lib/lavis/models/ulip_models/utils/tokenizer.py
+-rw-rw-r--  2.0 unx     7432 b- defN 24-May-09 20:37 build/lib/lavis/models/ulip_models/utils/utils.py
+-rw-rw-r--  2.0 unx     1897 b- defN 24-May-09 20:37 build/lib/lavis/processors/__init__.py
+-rw-rw-r--  2.0 unx     8633 b- defN 24-May-09 20:37 build/lib/lavis/processors/alpro_processors.py
+-rw-rw-r--  2.0 unx     5283 b- defN 24-May-09 20:37 build/lib/lavis/processors/audio_processors.py
+-rw-rw-r--  2.0 unx      604 b- defN 24-May-09 20:37 build/lib/lavis/processors/base_processor.py
+-rw-rw-r--  2.0 unx     2319 b- defN 24-May-09 20:37 build/lib/lavis/processors/blip_diffusion_processors.py
+-rw-rw-r--  2.0 unx     6690 b- defN 24-May-09 20:37 build/lib/lavis/processors/blip_processors.py
+-rw-rw-r--  2.0 unx     2570 b- defN 24-May-09 20:37 build/lib/lavis/processors/clip_processors.py
+-rw-rw-r--  2.0 unx     3924 b- defN 24-May-09 20:37 build/lib/lavis/processors/functional_video.py
+-rw-rw-r--  2.0 unx     5489 b- defN 24-May-09 20:37 build/lib/lavis/processors/gpt_processors.py
+-rw-rw-r--  2.0 unx    22739 b- defN 24-May-09 20:37 build/lib/lavis/processors/instruction_text_processors.py
+-rw-rw-r--  2.0 unx    11292 b- defN 24-May-09 20:37 build/lib/lavis/processors/randaugment.py
+-rw-rw-r--  2.0 unx     5013 b- defN 24-May-09 20:37 build/lib/lavis/processors/transforms_video.py
+-rw-rw-r--  2.0 unx     9297 b- defN 24-May-09 20:37 build/lib/lavis/processors/ulip_processors.py
+-rw-rw-r--  2.0 unx      360 b- defN 24-May-09 20:37 build/lib/lavis/runners/__init__.py
+-rw-rw-r--  2.0 unx    23509 b- defN 24-May-09 20:37 build/lib/lavis/runners/runner_base.py
+-rw-rw-r--  2.0 unx    13601 b- defN 24-May-09 20:37 build/lib/lavis/runners/runner_iter.py
+-rw-rw-r--  2.0 unx     1444 b- defN 24-May-09 20:37 build/lib/lavis/tasks/__init__.py
+-rw-rw-r--  2.0 unx     9274 b- defN 24-May-09 20:37 build/lib/lavis/tasks/base_task.py
+-rw-rw-r--  2.0 unx    11009 b- defN 24-May-09 20:37 build/lib/lavis/tasks/captioning.py
+-rw-rw-r--  2.0 unx     3919 b- defN 24-May-09 20:37 build/lib/lavis/tasks/dialogue.py
+-rw-rw-r--  2.0 unx      526 b- defN 24-May-09 20:37 build/lib/lavis/tasks/image_text_pretrain.py
+-rw-rw-r--  2.0 unx     4287 b- defN 24-May-09 20:37 build/lib/lavis/tasks/multimodal_classification.py
+-rw-rw-r--  2.0 unx     3208 b- defN 24-May-09 20:37 build/lib/lavis/tasks/retrieval.py
+-rw-rw-r--  2.0 unx      586 b- defN 24-May-09 20:37 build/lib/lavis/tasks/text_to_image_generation.py
+-rw-rw-r--  2.0 unx    17116 b- defN 24-May-09 20:37 build/lib/lavis/tasks/vqa.py
+-rw-rw-r--  2.0 unx     8745 b- defN 24-May-09 20:37 build/lib/lavis/tasks/vqa_reading_comprehension.py
+-rw-rw-r--  2.0 unx     5184 b- defN 24-May-09 20:37 build/lib/projects/img2llm-vqa/img2llm_vqa.py
+-rw-rw-r--  2.0 unx     3039 b- defN 24-May-09 20:37 build/lib/projects/instructblip/run_demo.py
+-rw-rw-r--  2.0 unx     4986 b- defN 24-May-09 20:37 build/lib/projects/xinstructblip/data_aug/3d_qa_data_generation.py
+-rw-rw-r--  2.0 unx     3608 b- defN 24-May-09 20:37 build/lib/projects/xinstructblip/data_aug/audio_qa_data_generation.py
+-rw-rw-r--  2.0 unx     8920 b- defN 24-May-09 20:37 build/lib/projects/xinstructblip/demo/run_demo.py
+-rw-rw-r--  2.0 unx     2052 b- defN 24-May-09 20:37 build/lib/projects/xinstructblip/discrn/caption_baseline/predict_audio.py
+-rw-rw-r--  2.0 unx     6447 b- defN 24-May-09 20:37 build/lib/projects/xinstructblip/discrn/caption_baseline/predict_image.py
+-rw-rw-r--  2.0 unx     6436 b- defN 24-May-09 20:37 build/lib/projects/xinstructblip/discrn/caption_baseline/predict_pc.py
+-rw-rw-r--  2.0 unx     6652 b- defN 24-May-09 20:37 build/lib/projects/xinstructblip/discrn/caption_baseline/predict_video.py
+-rw-rw-r--  2.0 unx     2030 b- defN 24-May-09 20:37 build/lib/projects/xinstructblip/discrn/caption_baseline/render_images.py
+-rw-rw-r--  2.0 unx     8764 b- defN 24-May-09 20:37 build/lib/projects/xinstructblip/discrn/data_generation/audiocaps_video_audio.py
+-rw-rw-r--  2.0 unx     9302 b- defN 24-May-09 20:37 build/lib/projects/xinstructblip/discrn/data_generation/objaverse_img_3d.py
+-rw-rw-r--  2.0 unx     1483 b- defN 24-May-09 20:37 build/lib/projects/xinstructblip/modelnet_baseline/render_images.py
+-rw-rw-r--  2.0 unx     5126 b- defN 24-May-09 20:37 build/lib/tests/models/test_albef.py
+-rw-rw-r--  2.0 unx    11612 b- defN 24-May-09 20:37 build/lib/tests/models/test_blip.py
+-rw-rw-r--  2.0 unx     5216 b- defN 24-May-09 20:37 build/lib/tests/models/test_blip2.py
+-rw-rw-r--  2.0 unx     4235 b- defN 24-May-09 20:37 build/lib/tests/models/test_pnp_vqa.py
 -rw-rw-r--  2.0 unx     1974 b- defN 24-May-09 20:37 docs/conf.py
 -rw-rw-r--  2.0 unx      930 b- defN 24-May-09 20:37 lavis/__init__.py
 -rw-rw-r--  2.0 unx    15070 b- defN 24-May-09 20:37 lavis/common/config.py
 -rw-rw-r--  2.0 unx     3614 b- defN 24-May-09 20:37 lavis/common/dist_utils.py
 -rw-rw-r--  2.0 unx      815 b- defN 24-May-09 20:37 lavis/common/gradcam.py
 -rw-rw-r--  2.0 unx     5992 b- defN 24-May-09 20:37 lavis/common/logger.py
--rw-rw-r--  2.0 unx     3374 b- defN 24-May-09 21:02 lavis/common/optims.py
+-rw-rw-r--  2.0 unx     4158 b- defN 24-May-09 20:37 lavis/common/optims.py
 -rw-rw-r--  2.0 unx     9870 b- defN 24-May-09 20:37 lavis/common/registry.py
--rw-rw-r--  2.0 unx    13798 b- defN 24-May-09 21:02 lavis/common/utils.py
+-rw-rw-r--  2.0 unx    14658 b- defN 24-May-09 20:37 lavis/common/utils.py
+-rw-rw-r--  2.0 unx      980 b- defN 24-May-09 20:37 lavis/common/annotator/util.py
+-rw-rw-r--  2.0 unx      155 b- defN 24-May-09 20:37 lavis/common/annotator/canny/__init__.py
+-rw-rw-r--  2.0 unx     6585 b- defN 24-May-09 20:37 lavis/common/annotator/hed/__init__.py
+-rw-rw-r--  2.0 unx     1400 b- defN 24-May-09 20:37 lavis/common/annotator/midas/__init__.py
+-rw-rw-r--  2.0 unx     5229 b- defN 24-May-09 20:37 lavis/common/annotator/midas/api.py
+-rw-rw-r--  2.0 unx     4582 b- defN 24-May-09 20:37 lavis/common/annotator/midas/utils.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-May-09 20:37 lavis/common/annotator/midas/midas/__init__.py
+-rw-rw-r--  2.0 unx      367 b- defN 24-May-09 20:37 lavis/common/annotator/midas/midas/base_model.py
+-rw-rw-r--  2.0 unx     9242 b- defN 24-May-09 20:37 lavis/common/annotator/midas/midas/blocks.py
+-rw-rw-r--  2.0 unx     3154 b- defN 24-May-09 20:37 lavis/common/annotator/midas/midas/dpt_depth.py
+-rw-rw-r--  2.0 unx     2709 b- defN 24-May-09 20:37 lavis/common/annotator/midas/midas/midas_net.py
+-rw-rw-r--  2.0 unx     5207 b- defN 24-May-09 20:37 lavis/common/annotator/midas/midas/midas_net_custom.py
+-rw-rw-r--  2.0 unx     7869 b- defN 24-May-09 20:37 lavis/common/annotator/midas/midas/transforms.py
+-rw-rw-r--  2.0 unx    14625 b- defN 24-May-09 20:37 lavis/common/annotator/midas/midas/vit.py
+-rw-rw-r--  2.0 unx     1458 b- defN 24-May-09 20:37 lavis/common/annotator/mlsd/__init__.py
+-rw-rw-r--  2.0 unx    24049 b- defN 24-May-09 20:37 lavis/common/annotator/mlsd/utils.py
+-rw-rw-r--  2.0 unx     9678 b- defN 24-May-09 20:37 lavis/common/annotator/mlsd/models/mbv2_mlsd_large.py
+-rw-rw-r--  2.0 unx     9180 b- defN 24-May-09 20:37 lavis/common/annotator/mlsd/models/mbv2_mlsd_tiny.py
+-rw-rw-r--  2.0 unx     1957 b- defN 24-May-09 20:37 lavis/common/annotator/openpose/__init__.py
+-rw-rw-r--  2.0 unx    10994 b- defN 24-May-09 20:37 lavis/common/annotator/openpose/body.py
+-rw-rw-r--  2.0 unx     3438 b- defN 24-May-09 20:37 lavis/common/annotator/openpose/hand.py
+-rw-rw-r--  2.0 unx     8745 b- defN 24-May-09 20:37 lavis/common/annotator/openpose/model.py
+-rw-rw-r--  2.0 unx     7507 b- defN 24-May-09 20:37 lavis/common/annotator/openpose/util.py
+-rw-rw-r--  2.0 unx     1070 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/__init__.py
+-rw-rw-r--  2.0 unx      321 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/default_runtime.py
+-rw-rw-r--  2.0 unx     1844 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/datasets/ade20k.py
+-rw-rw-r--  2.0 unx     1924 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/datasets/chase_db1.py
+-rw-rw-r--  2.0 unx     1780 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/datasets/cityscapes.py
+-rw-rw-r--  2.0 unx     1281 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/datasets/cityscapes_769x769.py
+-rw-rw-r--  2.0 unx     1915 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/datasets/drive.py
+-rw-rw-r--  2.0 unx     1915 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/datasets/hrf.py
+-rw-rw-r--  2.0 unx     1998 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/datasets/pascal_context.py
+-rw-rw-r--  2.0 unx     2024 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/datasets/pascal_context_59.py
+-rw-rw-r--  2.0 unx     1930 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/datasets/pascal_voc12.py
+-rw-rw-r--  2.0 unx      261 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/datasets/pascal_voc12_aug.py
+-rw-rw-r--  2.0 unx     1917 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/datasets/stare.py
+-rw-rw-r--  2.0 unx     1346 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/models/ann_r50-d8.py
+-rw-rw-r--  2.0 unx     1302 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/models/apcnet_r50-d8.py
+-rw-rw-r--  2.0 unx     1258 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/models/ccnet_r50-d8.py
+-rw-rw-r--  2.0 unx     1110 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/models/cgnet.py
+-rw-rw-r--  2.0 unx     1261 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/models/danet_r50-d8.py
+-rw-rw-r--  2.0 unx     1273 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/models/deeplabv3_r50-d8.py
+-rw-rw-r--  2.0 unx     1499 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py
+-rw-rw-r--  2.0 unx     1343 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py
+-rw-rw-r--  2.0 unx     1302 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/models/dmnet_r50-d8.py
+-rw-rw-r--  2.0 unx     1316 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/models/dnl_r50-d8.py
+-rw-rw-r--  2.0 unx     1329 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/models/emanet_r50-d8.py
+-rw-rw-r--  2.0 unx     1435 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/models/encnet_r50-d8.py
+-rw-rw-r--  2.0 unx     1761 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/models/fast_scnn.py
+-rw-rw-r--  2.0 unx     1646 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/models/fcn_hr18.py
+-rw-rw-r--  2.0 unx     1285 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/models/fcn_r50-d8.py
+-rw-rw-r--  2.0 unx     1512 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/models/fcn_unet_s5-d16.py
+-rw-rw-r--  2.0 unx     1056 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/models/fpn_r50.py
+-rw-rw-r--  2.0 unx      977 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/models/fpn_uniformer.py
+-rw-rw-r--  2.0 unx     1326 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/models/gcnet_r50-d8.py
+-rw-rw-r--  2.0 unx      766 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/models/lraspp_m-v3-d8.py
+-rw-rw-r--  2.0 unx     1315 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/models/nonlocal_r50-d8.py
+-rw-rw-r--  2.0 unx     2196 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/models/ocrnet_hr18.py
+-rw-rw-r--  2.0 unx     1385 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/models/ocrnet_r50-d8.py
+-rw-rw-r--  2.0 unx     1704 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/models/pointrend_r50.py
+-rw-rw-r--  2.0 unx     1406 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/models/psanet_r50-d8.py
+-rw-rw-r--  2.0 unx     1271 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/models/pspnet_r50-d8.py
+-rw-rw-r--  2.0 unx     1497 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py
+-rw-rw-r--  2.0 unx     1301 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/models/upernet_r50.py
+-rw-rw-r--  2.0 unx     1235 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/models/upernet_uniformer.py
+-rw-rw-r--  2.0 unx      382 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/schedules/schedule_160k.py
+-rw-rw-r--  2.0 unx      379 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/schedules/schedule_20k.py
+-rw-rw-r--  2.0 unx      379 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/schedules/schedule_40k.py
+-rw-rw-r--  2.0 unx      379 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/configs/_base_/schedules/schedule_80k.py
+-rw-rw-r--  2.0 unx     1316 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/exp/upernet_global_small/config.py
+-rw-rw-r--  2.0 unx     1317 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/exp/upernet_global_small/test_config_g.py
+-rw-rw-r--  2.0 unx     1339 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/exp/upernet_global_small/test_config_h32.py
+-rw-rw-r--  2.0 unx     1339 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/exp/upernet_global_small/test_config_w32.py
+-rw-rw-r--  2.0 unx      352 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/__init__.py
+-rw-rw-r--  2.0 unx     1177 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/version.py
+-rw-rw-r--  2.0 unx      133 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/arraymisc/__init__.py
+-rw-rw-r--  2.0 unx     1824 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/arraymisc/quantization.py
+-rw-rw-r--  2.0 unx     2438 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/cnn/__init__.py
+-rw-rw-r--  2.0 unx     1990 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/cnn/alexnet.py
+-rw-rw-r--  2.0 unx     1089 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/cnn/builder.py
+-rw-rw-r--  2.0 unx     9955 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/cnn/resnet.py
+-rw-rw-r--  2.0 unx     6053 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/cnn/vgg.py
+-rw-rw-r--  2.0 unx     1732 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/cnn/bricks/__init__.py
+-rw-rw-r--  2.0 unx     2508 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/cnn/bricks/activation.py
+-rw-rw-r--  2.0 unx     4681 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/cnn/bricks/context_block.py
+-rw-rw-r--  2.0 unx     1446 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/cnn/bricks/conv.py
+-rw-rw-r--  2.0 unx     2514 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py
+-rw-rw-r--  2.0 unx     8760 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/cnn/bricks/conv_module.py
+-rw-rw-r--  2.0 unx     5417 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/cnn/bricks/conv_ws.py
+-rw-rw-r--  2.0 unx     4142 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py
+-rw-rw-r--  2.0 unx     2172 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/cnn/bricks/drop.py
+-rw-rw-r--  2.0 unx    15999 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/cnn/bricks/generalized_attention.py
+-rw-rw-r--  2.0 unx     1097 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/cnn/bricks/hsigmoid.py
+-rw-rw-r--  2.0 unx      651 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/cnn/bricks/hswish.py
+-rw-rw-r--  2.0 unx    11012 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/cnn/bricks/non_local.py
+-rw-rw-r--  2.0 unx     5154 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/cnn/bricks/norm.py
+-rw-rw-r--  2.0 unx     1127 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/cnn/bricks/padding.py
+-rw-rw-r--  2.0 unx     2487 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/cnn/bricks/plugin.py
+-rw-rw-r--  2.0 unx      658 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/cnn/bricks/registry.py
+-rw-rw-r--  2.0 unx      577 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/cnn/bricks/scale.py
+-rw-rw-r--  2.0 unx      485 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/cnn/bricks/swish.py
+-rw-rw-r--  2.0 unx    24639 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/cnn/bricks/transformer.py
+-rw-rw-r--  2.0 unx     2880 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/cnn/bricks/upsample.py
+-rw-rw-r--  2.0 unx     6961 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/cnn/bricks/wrappers.py
+-rw-rw-r--  2.0 unx     1023 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/cnn/utils/__init__.py
+-rw-rw-r--  2.0 unx    22104 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/cnn/utils/flops_counter.py
+-rw-rw-r--  2.0 unx     1881 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/cnn/utils/fuse_conv_bn.py
+-rw-rw-r--  2.0 unx     2327 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/cnn/utils/sync_bn.py
+-rw-rw-r--  2.0 unx    26006 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/cnn/utils/weight_init.py
+-rw-rw-r--  2.0 unx      266 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/engine/__init__.py
+-rw-rw-r--  2.0 unx     7196 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/engine/test.py
+-rw-rw-r--  2.0 unx      478 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/fileio/__init__.py
+-rw-rw-r--  2.0 unx    41933 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/fileio/file_client.py
+-rw-rw-r--  2.0 unx     5520 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/fileio/io.py
+-rw-rw-r--  2.0 unx     3458 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/fileio/parse.py
+-rw-rw-r--  2.0 unx      278 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/fileio/handlers/__init__.py
+-rw-rw-r--  2.0 unx      993 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/fileio/handlers/base.py
+-rw-rw-r--  2.0 unx     1068 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/fileio/handlers/json_handler.py
+-rw-rw-r--  2.0 unx      817 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/fileio/handlers/pickle_handler.py
+-rw-rw-r--  2.0 unx      665 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/fileio/handlers/yaml_handler.py
+-rw-rw-r--  2.0 unx     1725 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/image/__init__.py
+-rw-rw-r--  2.0 unx     9907 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/image/colorspace.py
+-rw-rw-r--  2.0 unx    25196 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/image/geometric.py
+-rw-rw-r--  2.0 unx     9572 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/image/io.py
+-rw-rw-r--  2.0 unx     1410 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/image/misc.py
+-rw-rw-r--  2.0 unx    14999 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/image/photometric.py
+-rw-rw-r--  2.0 unx     4506 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/__init__.py
+-rw-rw-r--  2.0 unx     4344 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/assign_score_withk.py
+-rw-rw-r--  2.0 unx     1695 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/ball_query.py
+-rw-rw-r--  2.0 unx     2508 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/bbox.py
+-rw-rw-r--  2.0 unx     3725 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/border_align.py
+-rw-rw-r--  2.0 unx     1609 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/box_iou_rotated.py
+-rw-rw-r--  2.0 unx     9873 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/carafe.py
+-rw-rw-r--  2.0 unx     3041 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/cc_attention.py
+-rw-rw-r--  2.0 unx     1795 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/contour_expand.py
+-rw-rw-r--  2.0 unx     4697 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/corner_pool.py
+-rw-rw-r--  2.0 unx     6697 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/correlation.py
+-rw-rw-r--  2.0 unx    15603 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/deform_conv.py
+-rw-rw-r--  2.0 unx     7410 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/deform_roi_pool.py
+-rw-rw-r--  2.0 unx     1467 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/deprecated_wrappers.py
+-rw-rw-r--  2.0 unx     6582 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/focal_loss.py
+-rw-rw-r--  2.0 unx     2550 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/furthest_point_sample.py
+-rw-rw-r--  2.0 unx    10031 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/fused_bias_leakyrelu.py
+-rw-rw-r--  2.0 unx     1607 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/gather_points.py
+-rw-rw-r--  2.0 unx     8135 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/group_points.py
+-rw-rw-r--  2.0 unx      887 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/info.py
+-rw-rw-r--  2.0 unx     2988 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/iou3d.py
+-rw-rw-r--  2.0 unx     2599 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/knn.py
+-rw-rw-r--  2.0 unx     3761 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/masked_conv.py
+-rw-rw-r--  2.0 unx     5403 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/merge_cells.py
+-rw-rw-r--  2.0 unx    10574 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/modulated_deform_conv.py
+-rw-rw-r--  2.0 unx    15175 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/multi_scale_deform_attn.py
+-rw-rw-r--  2.0 unx    16237 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/nms.py
+-rw-rw-r--  2.0 unx     3113 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/pixel_group.py
+-rw-rw-r--  2.0 unx    12291 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/point_sample.py
+-rw-rw-r--  2.0 unx     5241 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/points_in_boxes.py
+-rw-rw-r--  2.0 unx     6063 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/points_sampler.py
+-rw-rw-r--  2.0 unx     2773 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/psa_mask.py
+-rw-rw-r--  2.0 unx     8519 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/roi_align.py
+-rw-rw-r--  2.0 unx     6434 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/roi_align_rotated.py
+-rw-rw-r--  2.0 unx     2517 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/roi_pool.py
+-rw-rw-r--  2.0 unx     4256 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/roiaware_pool3d.py
+-rw-rw-r--  2.0 unx     2990 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/roipoint_pool3d.py
+-rw-rw-r--  2.0 unx     5804 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/saconv.py
+-rw-rw-r--  2.0 unx     5201 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/scatter_points.py
+-rw-rw-r--  2.0 unx    11267 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/sync_bn.py
+-rw-rw-r--  2.0 unx     2147 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/three_interpolate.py
+-rw-rw-r--  2.0 unx     1515 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/three_nn.py
+-rw-rw-r--  2.0 unx     2141 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/tin_shift.py
+-rw-rw-r--  2.0 unx    11804 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/upfirdn2d.py
+-rw-rw-r--  2.0 unx     5286 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/ops/voxelize.py
+-rw-rw-r--  2.0 unx      505 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/parallel/__init__.py
+-rw-rw-r--  2.0 unx     2830 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/parallel/_functions.py
+-rw-rw-r--  2.0 unx     3665 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/parallel/collate.py
+-rw-rw-r--  2.0 unx     2365 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/parallel/data_container.py
+-rw-rw-r--  2.0 unx     3912 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/parallel/data_parallel.py
+-rw-rw-r--  2.0 unx     4857 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/parallel/distributed.py
+-rw-rw-r--  2.0 unx     2837 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/parallel/distributed_deprecated.py
+-rw-rw-r--  2.0 unx      332 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/parallel/registry.py
+-rw-rw-r--  2.0 unx     2307 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/parallel/scatter_gather.py
+-rw-rw-r--  2.0 unx      708 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/parallel/utils.py
+-rw-rw-r--  2.0 unx     2859 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/__init__.py
+-rw-rw-r--  2.0 unx     7502 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/base_module.py
+-rw-rw-r--  2.0 unx    20846 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/base_runner.py
+-rw-rw-r--  2.0 unx      666 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/builder.py
+-rw-rw-r--  2.0 unx    25136 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/checkpoint.py
+-rw-rw-r--  2.0 unx     1928 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/default_constructor.py
+-rw-rw-r--  2.0 unx     5395 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/dist_utils.py
+-rw-rw-r--  2.0 unx     7565 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/epoch_based_runner.py
+-rw-rw-r--  2.0 unx    15784 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/fp16_utils.py
+-rw-rw-r--  2.0 unx    11062 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/iter_based_runner.py
+-rw-rw-r--  2.0 unx     1192 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/log_buffer.py
+-rw-rw-r--  2.0 unx     1598 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/priority.py
+-rw-rw-r--  2.0 unx     2936 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/utils.py
+-rw-rw-r--  2.0 unx     1396 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/hooks/__init__.py
+-rw-rw-r--  2.0 unx     7317 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/hooks/checkpoint.py
+-rw-rw-r--  2.0 unx      269 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/hooks/closure.py
+-rw-rw-r--  2.0 unx     3599 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/hooks/ema.py
+-rw-rw-r--  2.0 unx    22448 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/hooks/evaluation.py
+-rw-rw-r--  2.0 unx     2761 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/hooks/hook.py
+-rw-rw-r--  2.0 unx      446 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/hooks/iter_timer.py
+-rw-rw-r--  2.0 unx    26034 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/hooks/lr_updater.py
+-rw-rw-r--  2.0 unx      657 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/hooks/memory.py
+-rw-rw-r--  2.0 unx    21296 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/hooks/momentum_updater.py
+-rw-rw-r--  2.0 unx    21654 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/hooks/optimizer.py
+-rw-rw-r--  2.0 unx     8041 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/hooks/profiler.py
+-rw-rw-r--  2.0 unx      847 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/hooks/sampler_seed.py
+-rw-rw-r--  2.0 unx      707 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/hooks/sync_buffer.py
+-rw-rw-r--  2.0 unx      522 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/hooks/logger/__init__.py
+-rw-rw-r--  2.0 unx     5451 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/hooks/logger/base.py
+-rw-rw-r--  2.0 unx     1761 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/hooks/logger/dvclive.py
+-rw-rw-r--  2.0 unx     2838 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/hooks/logger/mlflow.py
+-rw-rw-r--  2.0 unx     3077 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/hooks/logger/neptune.py
+-rw-rw-r--  2.0 unx     4378 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/hooks/logger/pavi.py
+-rw-rw-r--  2.0 unx     2077 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/hooks/logger/tensorboard.py
+-rw-rw-r--  2.0 unx    10684 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/hooks/logger/text.py
+-rw-rw-r--  2.0 unx     1694 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/hooks/logger/wandb.py
+-rw-rw-r--  2.0 unx      370 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/optimizer/__init__.py
+-rw-rw-r--  2.0 unx     1346 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/optimizer/builder.py
+-rw-rw-r--  2.0 unx    11803 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/runner/optimizer/default_constructor.py
+-rw-rw-r--  2.0 unx     3915 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/utils/__init__.py
+-rw-rw-r--  2.0 unx    26263 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/utils/config.py
+-rw-rw-r--  2.0 unx     3367 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/utils/env.py
+-rw-rw-r--  2.0 unx     2021 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/utils/ext_loader.py
+-rw-rw-r--  2.0 unx     3986 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/utils/logging.py
+-rw-rw-r--  2.0 unx    11447 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/utils/misc.py
+-rw-rw-r--  2.0 unx      899 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/utils/parrots_jit.py
+-rw-rw-r--  2.0 unx     3536 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/utils/parrots_wrapper.py
+-rw-rw-r--  2.0 unx     3414 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/utils/path.py
+-rw-rw-r--  2.0 unx     7105 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/utils/progressbar.py
+-rw-rw-r--  2.0 unx    11041 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/utils/registry.py
+-rw-rw-r--  2.0 unx     4289 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/utils/testing.py
+-rw-rw-r--  2.0 unx     2993 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/utils/timer.py
+-rw-rw-r--  2.0 unx      795 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/utils/trace.py
+-rw-rw-r--  2.0 unx     2673 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/utils/version_utils.py
+-rw-rw-r--  2.0 unx      570 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/video/__init__.py
+-rw-rw-r--  2.0 unx    10209 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/video/io.py
+-rw-rw-r--  2.0 unx     9728 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/video/optflow.py
+-rw-rw-r--  2.0 unx     5291 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/video/processing.py
+-rw-rw-r--  2.0 unx      338 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/visualization/__init__.py
+-rw-rw-r--  2.0 unx     1381 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/visualization/color.py
+-rw-rw-r--  2.0 unx     5145 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/visualization/image.py
+-rw-rw-r--  2.0 unx     3389 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv/visualization/optflow.py
+-rw-rw-r--  2.0 unx       95 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv_custom/__init__.py
+-rw-rw-r--  2.0 unx    19091 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmcv_custom/checkpoint.py
+-rw-rw-r--  2.0 unx      381 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/apis/__init__.py
+-rw-rw-r--  2.0 unx     4729 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/apis/inference.py
+-rw-rw-r--  2.0 unx     8288 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/apis/test.py
+-rw-rw-r--  2.0 unx     4035 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/apis/train.py
+-rw-rw-r--  2.0 unx      126 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/core/__init__.py
+-rw-rw-r--  2.0 unx      301 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/core/evaluation/__init__.py
+-rw-rw-r--  2.0 unx     7305 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/core/evaluation/class_names.py
+-rw-rw-r--  2.0 unx     3873 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/core/evaluation/eval_hooks.py
+-rw-rw-r--  2.0 unx    13079 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/core/evaluation/metrics.py
+-rw-rw-r--  2.0 unx      172 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/core/seg/__init__.py
+-rw-rw-r--  2.0 unx      273 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/core/seg/builder.py
+-rw-rw-r--  2.0 unx      150 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/core/seg/sampler/__init__.py
+-rw-rw-r--  2.0 unx      284 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/core/seg/sampler/base_pixel_sampler.py
+-rw-rw-r--  2.0 unx     3155 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py
+-rw-rw-r--  2.0 unx       55 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/core/utils/__init__.py
+-rw-rw-r--  2.0 unx      371 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/core/utils/misc.py
+-rw-rw-r--  2.0 unx      798 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/datasets/__init__.py
+-rw-rw-r--  2.0 unx     5185 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/datasets/ade.py
+-rw-rw-r--  2.0 unx     5951 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/datasets/builder.py
+-rw-rw-r--  2.0 unx      781 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/datasets/chase_db1.py
+-rw-rw-r--  2.0 unx     8494 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/datasets/cityscapes.py
+-rw-rw-r--  2.0 unx    14882 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/datasets/custom.py
+-rw-rw-r--  2.0 unx     1499 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/datasets/dataset_wrappers.py
+-rw-rw-r--  2.0 unx      771 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/datasets/drive.py
+-rw-rw-r--  2.0 unx      747 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/datasets/hrf.py
+-rw-rw-r--  2.0 unx     5202 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/datasets/pascal_context.py
+-rw-rw-r--  2.0 unx      761 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/datasets/stare.py
+-rw-rw-r--  2.0 unx     1130 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/datasets/voc.py
+-rw-rw-r--  2.0 unx      813 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/datasets/pipelines/__init__.py
+-rw-rw-r--  2.0 unx     1484 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/datasets/pipelines/compose.py
+-rw-rw-r--  2.0 unx     9276 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/datasets/pipelines/formating.py
+-rw-rw-r--  2.0 unx     5901 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/datasets/pipelines/loading.py
+-rw-rw-r--  2.0 unx     5201 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/datasets/pipelines/test_time_aug.py
+-rw-rw-r--  2.0 unx    30993 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/datasets/pipelines/transforms.py
+-rw-rw-r--  2.0 unx      489 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/__init__.py
+-rw-rw-r--  2.0 unx     1205 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/builder.py
+-rw-rw-r--  2.0 unx      532 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/backbones/__init__.py
+-rw-rw-r--  2.0 unx    13183 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/backbones/cgnet.py
+-rw-rw-r--  2.0 unx    14436 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/backbones/fast_scnn.py
+-rw-rw-r--  2.0 unx    21226 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/backbones/hrnet.py
+-rw-rw-r--  2.0 unx     6981 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/backbones/mobilenet_v2.py
+-rw-rw-r--  2.0 unx    10390 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/backbones/mobilenet_v3.py
+-rw-rw-r--  2.0 unx    10110 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/backbones/resnest.py
+-rw-rw-r--  2.0 unx    24310 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/backbones/resnet.py
+-rw-rw-r--  2.0 unx     5161 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/backbones/resnext.py
+-rw-rw-r--  2.0 unx    18269 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/backbones/unet.py
+-rw-rw-r--  2.0 unx    18476 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/backbones/uniformer.py
+-rw-rw-r--  2.0 unx    18085 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/backbones/vit.py
+-rw-rw-r--  2.0 unx      969 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/decode_heads/__init__.py
+-rw-rw-r--  2.0 unx     9194 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/decode_heads/ann_head.py
+-rw-rw-r--  2.0 unx     5572 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/decode_heads/apc_head.py
+-rw-rw-r--  2.0 unx     3459 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/decode_heads/aspp_head.py
+-rw-rw-r--  2.0 unx     2351 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/decode_heads/cascade_decode_head.py
+-rw-rw-r--  2.0 unx     1303 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/decode_heads/cc_head.py
+-rw-rw-r--  2.0 unx     5585 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/decode_heads/da_head.py
+-rw-rw-r--  2.0 unx     9240 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/decode_heads/decode_head.py
+-rw-rw-r--  2.0 unx     5004 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/decode_heads/dm_head.py
+-rw-rw-r--  2.0 unx     4591 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/decode_heads/dnl_head.py
+-rw-rw-r--  2.0 unx     5796 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/decode_heads/ema_head.py
+-rw-rw-r--  2.0 unx     6784 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/decode_heads/enc_head.py
+-rw-rw-r--  2.0 unx     2817 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/decode_heads/fcn_head.py
+-rw-rw-r--  2.0 unx     2422 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/decode_heads/fpn_head.py
+-rw-rw-r--  2.0 unx     1611 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/decode_heads/gc_head.py
+-rw-rw-r--  2.0 unx     3098 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/decode_heads/lraspp_head.py
+-rw-rw-r--  2.0 unx     1577 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/decode_heads/nl_head.py
+-rw-rw-r--  2.0 unx     4319 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/decode_heads/ocr_head.py
+-rw-rw-r--  2.0 unx    14754 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/decode_heads/point_head.py
+-rw-rw-r--  2.0 unx     7544 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/decode_heads/psa_head.py
+-rw-rw-r--  2.0 unx     3352 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/decode_heads/psp_head.py
+-rw-rw-r--  2.0 unx     3527 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/decode_heads/sep_aspp_head.py
+-rw-rw-r--  2.0 unx     2024 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/decode_heads/sep_fcn_head.py
+-rw-rw-r--  2.0 unx     4012 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/decode_heads/uper_head.py
+-rw-rw-r--  2.0 unx      529 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/losses/__init__.py
+-rw-rw-r--  2.0 unx     2970 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/losses/accuracy.py
+-rw-rw-r--  2.0 unx     7437 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/losses/cross_entropy_loss.py
+-rw-rw-r--  2.0 unx     4239 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/losses/dice_loss.py
+-rw-rw-r--  2.0 unx    11419 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/losses/lovasz_loss.py
+-rw-rw-r--  2.0 unx     3718 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/losses/utils.py
+-rw-rw-r--  2.0 unx      102 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/necks/__init__.py
+-rw-rw-r--  2.0 unx     9159 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/necks/fpn.py
+-rw-rw-r--  2.0 unx     2454 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/necks/multilevel_neck.py
+-rw-rw-r--  2.0 unx      207 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/segmentors/__init__.py
+-rw-rw-r--  2.0 unx    10398 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/segmentors/base.py
+-rw-rw-r--  2.0 unx     3708 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py
+-rw-rw-r--  2.0 unx    11344 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/segmentors/encoder_decoder.py
+-rw-rw-r--  2.0 unx      502 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/utils/__init__.py
+-rw-rw-r--  2.0 unx     1015 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/utils/drop.py
+-rw-rw-r--  2.0 unx     7025 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/utils/inverted_residual.py
+-rw-rw-r--  2.0 unx     1231 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/utils/make_divisible.py
+-rw-rw-r--  2.0 unx     3335 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/utils/res_layer.py
+-rw-rw-r--  2.0 unx     2151 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/utils/se_layer.py
+-rw-rw-r--  2.0 unx     6145 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/utils/self_attention_block.py
+-rw-rw-r--  2.0 unx     3988 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/utils/up_conv_block.py
+-rw-rw-r--  2.0 unx     2327 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/models/utils/weight_init.py
+-rw-rw-r--  2.0 unx      116 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/ops/__init__.py
+-rw-rw-r--  2.0 unx     2788 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/ops/encoding.py
+-rw-rw-r--  2.0 unx     1827 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/ops/wrappers.py
+-rw-rw-r--  2.0 unx      119 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/utils/__init__.py
+-rw-rw-r--  2.0 unx      505 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/utils/collect_env.py
+-rw-rw-r--  2.0 unx      919 b- defN 24-May-09 20:37 lavis/common/annotator/uniformer/mmseg/utils/logger.py
 -rw-rw-r--  2.0 unx      246 b- defN 24-May-09 20:37 lavis/common/vqa_tools/__init__.py
 -rw-rw-r--  2.0 unx     8634 b- defN 24-May-09 20:37 lavis/common/vqa_tools/vqa.py
 -rw-rw-r--  2.0 unx    11016 b- defN 24-May-09 20:37 lavis/common/vqa_tools/vqa_eval.py
 -rw-rw-r--  2.0 unx      360 b- defN 24-May-09 20:37 lavis/configs/default.yaml
 -rw-rw-r--  2.0 unx     1630 b- defN 24-May-09 20:37 lavis/configs/datasets/aokvqa/defaults.yaml
+-rw-rw-r--  2.0 unx     2060 b- defN 24-May-09 20:37 lavis/configs/datasets/aokvqa/defaults_instruct.yaml
+-rw-rw-r--  2.0 unx     1487 b- defN 24-May-09 20:37 lavis/configs/datasets/audiocaps/defaults_mm_cap.yaml
+-rw-rw-r--  2.0 unx     1649 b- defN 24-May-09 20:37 lavis/configs/datasets/audiocaps/defaults_mm_cap_instruct.yaml
+-rw-rw-r--  2.0 unx     1961 b- defN 24-May-09 20:37 lavis/configs/datasets/audiocaps/defaults_mm_qa.yaml
+-rw-rw-r--  2.0 unx     1750 b- defN 24-May-09 20:37 lavis/configs/datasets/audioset/defaults_mm_cap.yaml
+-rw-rw-r--  2.0 unx     1780 b- defN 24-May-09 20:37 lavis/configs/datasets/audioset/defaults_mm_cap_instruct.yaml
 -rw-rw-r--  2.0 unx     1086 b- defN 24-May-09 20:37 lavis/configs/datasets/avsd/defaults_dial.yaml
+-rw-rw-r--  2.0 unx     1845 b- defN 24-May-09 20:37 lavis/configs/datasets/avsd/defaults_mm_dial_instruct.yaml
+-rw-rw-r--  2.0 unx      510 b- defN 24-May-09 20:37 lavis/configs/datasets/blip_diffusion_datasets/defaults.yaml
+-rw-rw-r--  2.0 unx     1082 b- defN 24-May-09 20:37 lavis/configs/datasets/capfilt14m/defaults_cap.yaml
+-rw-rw-r--  2.0 unx     1147 b- defN 24-May-09 20:37 lavis/configs/datasets/capfilt14m/defaults_cap_instruct.yaml
+-rw-rw-r--  2.0 unx     1756 b- defN 24-May-09 20:37 lavis/configs/datasets/charade/defaults_cap.yaml
+-rw-rw-r--  2.0 unx     1813 b- defN 24-May-09 20:37 lavis/configs/datasets/charade/defaults_cap_instruct.yaml
+-rw-rw-r--  2.0 unx     1189 b- defN 24-May-09 20:37 lavis/configs/datasets/clotho/defaults_mm_cap.yaml
+-rw-rw-r--  2.0 unx     1255 b- defN 24-May-09 20:37 lavis/configs/datasets/clotho/defaults_mm_cap_instruct.yaml
+-rw-rw-r--  2.0 unx     1217 b- defN 24-May-09 20:37 lavis/configs/datasets/clotho/defaults_mm_qa.yaml
 -rw-rw-r--  2.0 unx     1266 b- defN 24-May-09 20:37 lavis/configs/datasets/coco/defaults_cap.yaml
+-rw-rw-r--  2.0 unx     1652 b- defN 24-May-09 20:37 lavis/configs/datasets/coco/defaults_cap_instruct.yaml
 -rw-rw-r--  2.0 unx     1193 b- defN 24-May-09 20:37 lavis/configs/datasets/coco/defaults_ret.yaml
 -rw-rw-r--  2.0 unx     2073 b- defN 24-May-09 20:37 lavis/configs/datasets/coco/defaults_vqa.yaml
+-rw-rw-r--  2.0 unx     2460 b- defN 24-May-09 20:37 lavis/configs/datasets/coco/defaults_vqa_instruct.yaml
 -rw-rw-r--  2.0 unx     1338 b- defN 24-May-09 20:37 lavis/configs/datasets/coco/eval_vqa.yaml
+-rw-rw-r--  2.0 unx     1770 b- defN 24-May-09 20:37 lavis/configs/datasets/coin/defaults_cap.yaml
+-rw-rw-r--  2.0 unx     1833 b- defN 24-May-09 20:37 lavis/configs/datasets/coin/defaults_cap_instruct.yaml
 -rw-rw-r--  2.0 unx      693 b- defN 24-May-09 20:37 lavis/configs/datasets/conceptual_caption/defaults_12m.yaml
+-rw-rw-r--  2.0 unx     1140 b- defN 24-May-09 20:37 lavis/configs/datasets/conceptual_caption/defaults_12m_instruct.yaml
 -rw-rw-r--  2.0 unx      686 b- defN 24-May-09 20:37 lavis/configs/datasets/conceptual_caption/defaults_3m.yaml
+-rw-rw-r--  2.0 unx     1007 b- defN 24-May-09 20:37 lavis/configs/datasets/conceptual_caption/defaults_3m_instruct.yaml
 -rw-rw-r--  2.0 unx     1171 b- defN 24-May-09 20:37 lavis/configs/datasets/didemo/defaults_ret.yaml
+-rw-rw-r--  2.0 unx     1965 b- defN 24-May-09 20:37 lavis/configs/datasets/discriminatory_reasoning/defaults_mm_audio_video.yaml
+-rw-rw-r--  2.0 unx     1593 b- defN 24-May-09 20:37 lavis/configs/datasets/discriminatory_reasoning/defaults_mm_image_pc.yaml
+-rw-rw-r--  2.0 unx  7901851 b- defN 24-May-09 20:37 lavis/configs/datasets/discriminatory_reasoning/discriminatory_dataset/audiocaps_discrn.json
+-rw-rw-r--  2.0 unx 21624268 b- defN 24-May-09 20:37 lavis/configs/datasets/discriminatory_reasoning/discriminatory_dataset/objaverse_discrn.json
+-rw-rw-r--  2.0 unx     1012 b- defN 24-May-09 20:37 lavis/configs/datasets/esc50/defaults_mm_cls.yaml
 -rw-rw-r--  2.0 unx      962 b- defN 24-May-09 20:37 lavis/configs/datasets/flickr30k/defaults.yaml
+-rw-rw-r--  2.0 unx     1334 b- defN 24-May-09 20:37 lavis/configs/datasets/flickr30k/defaults_cap.yaml
+-rw-rw-r--  2.0 unx     1395 b- defN 24-May-09 20:37 lavis/configs/datasets/flickr30k/defaults_cap_instruct.yaml
 -rw-rw-r--  2.0 unx     1193 b- defN 24-May-09 20:37 lavis/configs/datasets/gqa/balanced_testdev.yaml
+-rw-rw-r--  2.0 unx     1539 b- defN 24-May-09 20:37 lavis/configs/datasets/gqa/balanced_testdev_instruct.yaml
 -rw-rw-r--  2.0 unx     1189 b- defN 24-May-09 20:37 lavis/configs/datasets/gqa/balanced_val.yaml
+-rw-rw-r--  2.0 unx     1549 b- defN 24-May-09 20:37 lavis/configs/datasets/gqa/balanced_val_instruct.yaml
 -rw-rw-r--  2.0 unx     1678 b- defN 24-May-09 20:37 lavis/configs/datasets/gqa/defaults.yaml
+-rw-rw-r--  2.0 unx     2264 b- defN 24-May-09 20:37 lavis/configs/datasets/gqa/defaults_instruct.yaml
+-rw-rw-r--  2.0 unx     1923 b- defN 24-May-09 20:37 lavis/configs/datasets/iconqa/defaults.yaml
+-rw-rw-r--  2.0 unx     2005 b- defN 24-May-09 20:37 lavis/configs/datasets/iconqa/defaults_instruct.yaml
 -rw-rw-r--  2.0 unx      525 b- defN 24-May-09 20:37 lavis/configs/datasets/imagenet/defaults.yaml
 -rw-rw-r--  2.0 unx      442 b- defN 24-May-09 20:37 lavis/configs/datasets/laion/defaults_2B_multi.yaml
+-rw-rw-r--  2.0 unx      685 b- defN 24-May-09 20:37 lavis/configs/datasets/laion/defaults_400M.yaml
+-rw-rw-r--  2.0 unx      907 b- defN 24-May-09 20:37 lavis/configs/datasets/laion/defaults_400M_instruct.yaml
+-rw-rw-r--  2.0 unx      969 b- defN 24-May-09 20:37 lavis/configs/datasets/llava150k/defaults_dial.yaml
+-rw-rw-r--  2.0 unx     2290 b- defN 24-May-09 20:37 lavis/configs/datasets/modelnet40/defaults_cls.yaml
 -rw-rw-r--  2.0 unx     1058 b- defN 24-May-09 20:37 lavis/configs/datasets/msrvtt/defaults_cap.yaml
+-rw-rw-r--  2.0 unx     1571 b- defN 24-May-09 20:37 lavis/configs/datasets/msrvtt/defaults_cap_instruct.yaml
 -rw-rw-r--  2.0 unx     1244 b- defN 24-May-09 20:37 lavis/configs/datasets/msrvtt/defaults_qa.yaml
+-rw-rw-r--  2.0 unx     1757 b- defN 24-May-09 20:37 lavis/configs/datasets/msrvtt/defaults_qa_instruct.yaml
 -rw-rw-r--  2.0 unx     1100 b- defN 24-May-09 20:37 lavis/configs/datasets/msrvtt/defaults_ret.yaml
 -rw-rw-r--  2.0 unx     1042 b- defN 24-May-09 20:37 lavis/configs/datasets/msvd/defaults_cap.yaml
+-rw-rw-r--  2.0 unx     1618 b- defN 24-May-09 20:37 lavis/configs/datasets/msvd/defaults_cap_instruct.yaml
 -rw-rw-r--  2.0 unx     1260 b- defN 24-May-09 20:37 lavis/configs/datasets/msvd/defaults_qa.yaml
+-rw-rw-r--  2.0 unx     1804 b- defN 24-May-09 20:37 lavis/configs/datasets/msvd/defaults_qa_instruct.yaml
+-rw-rw-r--  2.0 unx     2119 b- defN 24-May-09 20:37 lavis/configs/datasets/music_avqa/defaults_mm_qa.yaml
+-rw-rw-r--  2.0 unx     2177 b- defN 24-May-09 20:37 lavis/configs/datasets/music_avqa/defaults_mm_qa_instruct.yaml
 -rw-rw-r--  2.0 unx     1025 b- defN 24-May-09 20:37 lavis/configs/datasets/nlvr/defaults.yaml
 -rw-rw-r--  2.0 unx      918 b- defN 24-May-09 20:37 lavis/configs/datasets/nocaps/defaults.yaml
+-rw-rw-r--  2.0 unx     1979 b- defN 24-May-09 20:37 lavis/configs/datasets/objaverse/defaults_mm_cap.yaml
+-rw-rw-r--  2.0 unx     2056 b- defN 24-May-09 20:37 lavis/configs/datasets/objaverse/defaults_mm_cap_instruct.yaml
+-rw-rw-r--  2.0 unx     1896 b- defN 24-May-09 20:37 lavis/configs/datasets/objaverse/defaults_mm_qa.yaml
+-rw-rw-r--  2.0 unx     1114 b- defN 24-May-09 20:37 lavis/configs/datasets/ocrvqa/defaults.yaml
+-rw-rw-r--  2.0 unx     1135 b- defN 24-May-09 20:37 lavis/configs/datasets/ocrvqa/defaults_instruct.yaml
 -rw-rw-r--  2.0 unx     2028 b- defN 24-May-09 20:37 lavis/configs/datasets/okvqa/defaults.yaml
+-rw-rw-r--  2.0 unx     2394 b- defN 24-May-09 20:37 lavis/configs/datasets/okvqa/defaults_instruct.yaml
 -rw-rw-r--  2.0 unx      856 b- defN 24-May-09 20:37 lavis/configs/datasets/sbu_caption/defaults.yaml
+-rw-rw-r--  2.0 unx     1173 b- defN 24-May-09 20:37 lavis/configs/datasets/sbu_caption/defaults_instruct.yaml
+-rw-rw-r--  2.0 unx     1980 b- defN 24-May-09 20:37 lavis/configs/datasets/scienceqa/defaults.yaml
+-rw-rw-r--  2.0 unx     2058 b- defN 24-May-09 20:37 lavis/configs/datasets/scienceqa/defaults_instruct.yaml
+-rw-rw-r--  2.0 unx     1903 b- defN 24-May-09 20:37 lavis/configs/datasets/shapenet/defaults_mm_cap.yaml
+-rw-rw-r--  2.0 unx     1971 b- defN 24-May-09 20:37 lavis/configs/datasets/shapenet/defaults_mm_cap_instruct.yaml
 -rw-rw-r--  2.0 unx     1017 b- defN 24-May-09 20:37 lavis/configs/datasets/snli_ve/defaults.yaml
--rw-rw-r--  2.0 unx     1078 b- defN 24-May-09 21:02 lavis/configs/datasets/vatex/defaults_cap.yaml
+-rw-rw-r--  2.0 unx     1658 b- defN 24-May-09 20:37 lavis/configs/datasets/snli_ve/defaults_instruct.yaml
+-rw-rw-r--  2.0 unx     1428 b- defN 24-May-09 20:37 lavis/configs/datasets/textcaps/defaults.yaml
+-rw-rw-r--  2.0 unx     1482 b- defN 24-May-09 20:37 lavis/configs/datasets/textcaps/defaults_instruct.yaml
+-rw-rw-r--  2.0 unx     2077 b- defN 24-May-09 20:37 lavis/configs/datasets/valor/defaults_mm_cap.yaml
+-rw-rw-r--  2.0 unx     2140 b- defN 24-May-09 20:37 lavis/configs/datasets/valor/defaults_mm_cap_instruct.yaml
+-rw-rw-r--  2.0 unx     1078 b- defN 24-May-09 20:37 lavis/configs/datasets/vatex/defaults_cap.yaml
+-rw-rw-r--  2.0 unx     1837 b- defN 24-May-09 20:37 lavis/configs/datasets/vatex/defaults_cap_instruct.yaml
 -rw-rw-r--  2.0 unx      679 b- defN 24-May-09 20:37 lavis/configs/datasets/vg/defaults_caption.yaml
+-rw-rw-r--  2.0 unx     1046 b- defN 24-May-09 20:37 lavis/configs/datasets/vg/defaults_caption_instruct.yaml
 -rw-rw-r--  2.0 unx      665 b- defN 24-May-09 20:37 lavis/configs/datasets/vg/defaults_vqa.yaml
+-rw-rw-r--  2.0 unx     1028 b- defN 24-May-09 20:37 lavis/configs/datasets/vg/defaults_vqa_instruct.yaml
+-rw-rw-r--  2.0 unx     1773 b- defN 24-May-09 20:37 lavis/configs/datasets/violin/defaults_cap.yaml
+-rw-rw-r--  2.0 unx     1832 b- defN 24-May-09 20:37 lavis/configs/datasets/violin/defaults_cap_instruct.yaml
+-rw-rw-r--  2.0 unx     1753 b- defN 24-May-09 20:37 lavis/configs/datasets/violin/defaults_entail.yaml
+-rw-rw-r--  2.0 unx     1759 b- defN 24-May-09 20:37 lavis/configs/datasets/violin/defaults_entail_instruct.yaml
+-rw-rw-r--  2.0 unx     1452 b- defN 24-May-09 20:37 lavis/configs/datasets/visdial/defaults_dial.yaml
+-rw-rw-r--  2.0 unx     1453 b- defN 24-May-09 20:37 lavis/configs/datasets/visdial/defaults_dial_instruct.yaml
+-rw-rw-r--  2.0 unx     1484 b- defN 24-May-09 20:37 lavis/configs/datasets/vizwiz/defaults.yaml
+-rw-rw-r--  2.0 unx     1869 b- defN 24-May-09 20:37 lavis/configs/datasets/vlep/defaults_cap.yaml
+-rw-rw-r--  2.0 unx     1928 b- defN 24-May-09 20:37 lavis/configs/datasets/vlep/defaults_cap_instruct.yaml
+-rw-rw-r--  2.0 unx     2015 b- defN 24-May-09 20:37 lavis/configs/datasets/vsr/defaults.yaml
+-rw-rw-r--  2.0 unx     2006 b- defN 24-May-09 20:37 lavis/configs/datasets/vsr/defaults_classification.yaml
+-rw-rw-r--  2.0 unx     2012 b- defN 24-May-09 20:37 lavis/configs/datasets/vsr/defaults_classification_instruct.yaml
+-rw-rw-r--  2.0 unx     2078 b- defN 24-May-09 20:37 lavis/configs/datasets/vsr/defaults_instruct.yaml
+-rw-rw-r--  2.0 unx     2836 b- defN 24-May-09 20:37 lavis/configs/datasets/wavcaps/defaults_mm_cap.yaml
+-rw-rw-r--  2.0 unx     2873 b- defN 24-May-09 20:37 lavis/configs/datasets/wavcaps/defaults_mm_cap_instruct.yaml
+-rw-rw-r--  2.0 unx     1353 b- defN 24-May-09 20:37 lavis/configs/datasets/webvid/defaults_cap.yaml
+-rw-rw-r--  2.0 unx     1416 b- defN 24-May-09 20:37 lavis/configs/datasets/webvid/defaults_cap_instruct.yaml
+-rw-rw-r--  2.0 unx     1861 b- defN 24-May-09 20:37 lavis/configs/datasets/youcook/defaults_cap.yaml
+-rw-rw-r--  2.0 unx     1924 b- defN 24-May-09 20:37 lavis/configs/datasets/youcook/defaults_cap_instruct.yaml
+-rw-rw-r--  2.0 unx     1801 b- defN 24-May-09 20:37 lavis/configs/datasets/yt8m/defaults_mm_dial.yaml
 -rw-rw-r--  2.0 unx      979 b- defN 24-May-09 20:37 lavis/configs/models/albef_classification_ve.yaml
 -rw-rw-r--  2.0 unx      739 b- defN 24-May-09 20:37 lavis/configs/models/albef_feature_extractor.yaml
 -rw-rw-r--  2.0 unx     1028 b- defN 24-May-09 20:37 lavis/configs/models/albef_nlvr.yaml
 -rw-rw-r--  2.0 unx      866 b- defN 24-May-09 20:37 lavis/configs/models/albef_pretrain_base.yaml
 -rw-rw-r--  2.0 unx     1104 b- defN 24-May-09 20:37 lavis/configs/models/albef_retrieval_coco.yaml
 -rw-rw-r--  2.0 unx     1104 b- defN 24-May-09 20:37 lavis/configs/models/albef_retrieval_flickr.yaml
 -rw-rw-r--  2.0 unx      998 b- defN 24-May-09 20:37 lavis/configs/models/albef_vqav2.yaml
@@ -84,25 +1089,36 @@
 -rw-rw-r--  2.0 unx     1114 b- defN 24-May-09 20:37 lavis/configs/models/clip_vit_base32.yaml
 -rw-rw-r--  2.0 unx     1114 b- defN 24-May-09 20:37 lavis/configs/models/clip_vit_large14.yaml
 -rw-rw-r--  2.0 unx     1118 b- defN 24-May-09 20:37 lavis/configs/models/clip_vit_large14_336.yaml
 -rw-rw-r--  2.0 unx      892 b- defN 24-May-09 20:37 lavis/configs/models/gpt_dialogue_base.yaml
 -rw-rw-r--  2.0 unx      489 b- defN 24-May-09 20:37 lavis/configs/models/med_config.json
 -rw-rw-r--  2.0 unx      510 b- defN 24-May-09 20:37 lavis/configs/models/med_config_albef.json
 -rw-rw-r--  2.0 unx      490 b- defN 24-May-09 20:37 lavis/configs/models/med_large_config.json
+-rw-rw-r--  2.0 unx      670 b- defN 24-May-09 20:37 lavis/configs/models/blip-diffusion/blip_diffusion_base.yaml
+-rw-rw-r--  2.0 unx      748 b- defN 24-May-09 20:37 lavis/configs/models/blip-diffusion/blip_diffusion_controlnet_canny.yaml
+-rw-rw-r--  2.0 unx      758 b- defN 24-May-09 20:37 lavis/configs/models/blip-diffusion/blip_diffusion_controlnet_depth.yaml
+-rw-rw-r--  2.0 unx      756 b- defN 24-May-09 20:37 lavis/configs/models/blip-diffusion/blip_diffusion_controlnet_hed.yaml
 -rw-rw-r--  2.0 unx     1074 b- defN 24-May-09 20:37 lavis/configs/models/blip2/blip2_caption_flant5xl.yaml
 -rw-rw-r--  2.0 unx     1073 b- defN 24-May-09 20:37 lavis/configs/models/blip2/blip2_caption_opt2.7b.yaml
 -rw-rw-r--  2.0 unx     1073 b- defN 24-May-09 20:37 lavis/configs/models/blip2/blip2_caption_opt6.7b.yaml
 -rw-rw-r--  2.0 unx      957 b- defN 24-May-09 20:37 lavis/configs/models/blip2/blip2_coco.yaml
+-rw-rw-r--  2.0 unx      980 b- defN 24-May-09 20:37 lavis/configs/models/blip2/blip2_instruct_flant5xl.yaml
+-rw-rw-r--  2.0 unx      983 b- defN 24-May-09 20:37 lavis/configs/models/blip2/blip2_instruct_flant5xxl.yaml
+-rw-rw-r--  2.0 unx     1017 b- defN 24-May-09 20:37 lavis/configs/models/blip2/blip2_instruct_vicuna13b.yaml
+-rw-rw-r--  2.0 unx     1014 b- defN 24-May-09 20:37 lavis/configs/models/blip2/blip2_instruct_vicuna7b.yaml
 -rw-rw-r--  2.0 unx      860 b- defN 24-May-09 20:37 lavis/configs/models/blip2/blip2_pretrain.yaml
 -rw-rw-r--  2.0 unx      955 b- defN 24-May-09 20:37 lavis/configs/models/blip2/blip2_pretrain_flant5xl.yaml
 -rw-rw-r--  2.0 unx      982 b- defN 24-May-09 20:37 lavis/configs/models/blip2/blip2_pretrain_flant5xl_vitL.yaml
 -rw-rw-r--  2.0 unx      958 b- defN 24-May-09 20:37 lavis/configs/models/blip2/blip2_pretrain_flant5xxl.yaml
+-rw-rw-r--  2.0 unx      973 b- defN 24-May-09 20:37 lavis/configs/models/blip2/blip2_pretrain_llama7b.yaml
 -rw-rw-r--  2.0 unx      955 b- defN 24-May-09 20:37 lavis/configs/models/blip2/blip2_pretrain_opt2.7b.yaml
 -rw-rw-r--  2.0 unx      955 b- defN 24-May-09 20:37 lavis/configs/models/blip2/blip2_pretrain_opt6.7b.yaml
 -rw-rw-r--  2.0 unx      887 b- defN 24-May-09 20:37 lavis/configs/models/blip2/blip2_pretrain_vitL.yaml
+-rw-rw-r--  2.0 unx     2856 b- defN 24-May-09 20:37 lavis/configs/models/blip2/blip2_xinstruct_vicuna13b.yaml
+-rw-rw-r--  2.0 unx     3045 b- defN 24-May-09 20:37 lavis/configs/models/blip2/blip2_xinstruct_vicuna7b.yaml
 -rw-rw-r--  2.0 unx      389 b- defN 24-May-09 20:37 lavis/configs/models/clip/RN101-quickgelu.json
 -rw-rw-r--  2.0 unx      365 b- defN 24-May-09 20:37 lavis/configs/models/clip/RN101.json
 -rw-rw-r--  2.0 unx      389 b- defN 24-May-09 20:37 lavis/configs/models/clip/RN50-quickgelu.json
 -rw-rw-r--  2.0 unx      365 b- defN 24-May-09 20:37 lavis/configs/models/clip/RN50.json
 -rw-rw-r--  2.0 unx      366 b- defN 24-May-09 20:37 lavis/configs/models/clip/RN50x16.json
 -rw-rw-r--  2.0 unx      366 b- defN 24-May-09 20:37 lavis/configs/models/clip/RN50x4.json
 -rw-rw-r--  2.0 unx      296 b- defN 24-May-09 20:37 lavis/configs/models/clip/ViT-B-16-plus-240.json
@@ -130,85 +1146,133 @@
 -rw-rw-r--  2.0 unx     1441 b- defN 24-May-09 20:37 lavis/configs/models/img2prompt-vqa/img2prompt_vqa_base.yaml
 -rw-rw-r--  2.0 unx     1465 b- defN 24-May-09 20:37 lavis/configs/models/pnp-vqa/pnp_vqa_3b.yaml
 -rw-rw-r--  2.0 unx     1470 b- defN 24-May-09 20:37 lavis/configs/models/pnp-vqa/pnp_vqa_base.yaml
 -rw-rw-r--  2.0 unx     1474 b- defN 24-May-09 20:37 lavis/configs/models/pnp-vqa/pnp_vqa_large.yaml
 -rw-rw-r--  2.0 unx     1482 b- defN 24-May-09 20:37 lavis/configs/models/pnp-vqa/unifiedqav2_3b_config.json
 -rw-rw-r--  2.0 unx     1451 b- defN 24-May-09 20:37 lavis/configs/models/pnp-vqa/unifiedqav2_base_config.json
 -rw-rw-r--  2.0 unx     1452 b- defN 24-May-09 20:37 lavis/configs/models/pnp-vqa/unifiedqav2_large_config.json
--rw-rw-r--  2.0 unx     9510 b- defN 24-May-09 21:02 lavis/datasets/data_utils.py
--rw-rw-r--  2.0 unx     3179 b- defN 24-May-09 21:02 lavis/datasets/builders/__init__.py
--rw-rw-r--  2.0 unx     8099 b- defN 24-May-09 21:02 lavis/datasets/builders/base_dataset_builder.py
--rw-rw-r--  2.0 unx     1904 b- defN 24-May-09 21:02 lavis/datasets/builders/caption_builder.py
--rw-rw-r--  2.0 unx     1009 b- defN 24-May-09 21:02 lavis/datasets/builders/classification_builder.py
--rw-rw-r--  2.0 unx      705 b- defN 24-May-09 21:02 lavis/datasets/builders/dialogue_builder.py
--rw-rw-r--  2.0 unx     2320 b- defN 24-May-09 21:02 lavis/datasets/builders/image_text_pair_builder.py
+-rw-rw-r--  2.0 unx    11995 b- defN 24-May-09 20:37 lavis/datasets/data_utils.py
+-rw-rw-r--  2.0 unx     7773 b- defN 24-May-09 20:37 lavis/datasets/builders/__init__.py
+-rw-rw-r--  2.0 unx     3881 b- defN 24-May-09 20:37 lavis/datasets/builders/audio_caption_builder.py
+-rw-rw-r--  2.0 unx      968 b- defN 24-May-09 20:37 lavis/datasets/builders/audio_qa_builder.py
+-rw-rw-r--  2.0 unx    11771 b- defN 24-May-09 20:37 lavis/datasets/builders/base_dataset_builder.py
+-rw-rw-r--  2.0 unx    10617 b- defN 24-May-09 20:37 lavis/datasets/builders/caption_builder.py
+-rw-rw-r--  2.0 unx     3189 b- defN 24-May-09 20:37 lavis/datasets/builders/classification_builder.py
+-rw-rw-r--  2.0 unx     2467 b- defN 24-May-09 20:37 lavis/datasets/builders/dialogue_builder.py
+-rw-rw-r--  2.0 unx      988 b- defN 24-May-09 20:37 lavis/datasets/builders/discrn_builders.py
+-rw-rw-r--  2.0 unx     3917 b- defN 24-May-09 20:37 lavis/datasets/builders/image_text_pair_builder.py
 -rw-rw-r--  2.0 unx    20539 b- defN 24-May-09 20:37 lavis/datasets/builders/imagefolder_builder.py
+-rw-rw-r--  2.0 unx     2349 b- defN 24-May-09 20:37 lavis/datasets/builders/object3d_caption_builder.py
+-rw-rw-r--  2.0 unx      784 b- defN 24-May-09 20:37 lavis/datasets/builders/object3d_classification_builder.py
+-rw-rw-r--  2.0 unx      712 b- defN 24-May-09 20:37 lavis/datasets/builders/object3d_qa_builder.py
 -rw-rw-r--  2.0 unx     1579 b- defN 24-May-09 20:37 lavis/datasets/builders/retrieval_builder.py
--rw-rw-r--  2.0 unx     1333 b- defN 24-May-09 21:02 lavis/datasets/builders/video_qa_builder.py
--rw-rw-r--  2.0 unx     1955 b- defN 24-May-09 21:02 lavis/datasets/builders/vqa_builder.py
--rw-rw-r--  2.0 unx     4960 b- defN 24-May-09 21:02 lavis/datasets/datasets/aok_vqa_datasets.py
--rw-rw-r--  2.0 unx     5679 b- defN 24-May-09 21:02 lavis/datasets/datasets/avsd_dialogue_datasets.py
--rw-rw-r--  2.0 unx     2046 b- defN 24-May-09 21:02 lavis/datasets/datasets/base_dataset.py
--rw-rw-r--  2.0 unx     2539 b- defN 24-May-09 21:02 lavis/datasets/datasets/caption_datasets.py
--rw-rw-r--  2.0 unx     2095 b- defN 24-May-09 21:02 lavis/datasets/datasets/coco_caption_datasets.py
--rw-rw-r--  2.0 unx     3215 b- defN 24-May-09 21:02 lavis/datasets/datasets/coco_vqa_datasets.py
--rw-rw-r--  2.0 unx     5249 b- defN 24-May-09 21:02 lavis/datasets/datasets/dataloader_utils.py
+-rw-rw-r--  2.0 unx     1255 b- defN 24-May-09 20:37 lavis/datasets/builders/text_to_image_generation_builder.py
+-rw-rw-r--  2.0 unx     2632 b- defN 24-May-09 20:37 lavis/datasets/builders/video_qa_builder.py
+-rw-rw-r--  2.0 unx     5581 b- defN 24-May-09 20:37 lavis/datasets/builders/vqa_builder.py
+-rw-rw-r--  2.0 unx     5344 b- defN 24-May-09 20:37 lavis/datasets/datasets/aok_vqa_datasets.py
+-rw-rw-r--  2.0 unx    17282 b- defN 24-May-09 20:37 lavis/datasets/datasets/audio_captioning_datasets.py
+-rw-rw-r--  2.0 unx     3468 b- defN 24-May-09 20:37 lavis/datasets/datasets/audio_classification_datasets.py
+-rw-rw-r--  2.0 unx     4832 b- defN 24-May-09 20:37 lavis/datasets/datasets/audio_qa_datasets.py
+-rw-rw-r--  2.0 unx     8472 b- defN 24-May-09 20:37 lavis/datasets/datasets/avsd_dialogue_datasets.py
+-rw-rw-r--  2.0 unx     3387 b- defN 24-May-09 20:37 lavis/datasets/datasets/base_dataset.py
+-rw-rw-r--  2.0 unx     1899 b- defN 24-May-09 20:37 lavis/datasets/datasets/capfilt_dataset.py
+-rw-rw-r--  2.0 unx     2880 b- defN 24-May-09 20:37 lavis/datasets/datasets/caption_datasets.py
+-rw-rw-r--  2.0 unx     2167 b- defN 24-May-09 20:37 lavis/datasets/datasets/coco_caption_datasets.py
+-rw-rw-r--  2.0 unx     3607 b- defN 24-May-09 20:37 lavis/datasets/datasets/coco_vqa_datasets.py
+-rw-rw-r--  2.0 unx     5330 b- defN 24-May-09 20:37 lavis/datasets/datasets/dataloader_utils.py
 -rw-rw-r--  2.0 unx     4225 b- defN 24-May-09 20:37 lavis/datasets/datasets/dialogue_datasets.py
--rw-rw-r--  2.0 unx     2936 b- defN 24-May-09 21:02 lavis/datasets/datasets/gqa_datasets.py
--rw-rw-r--  2.0 unx     1461 b- defN 24-May-09 21:02 lavis/datasets/datasets/image_text_pair_datasets.py
+-rw-rw-r--  2.0 unx     8778 b- defN 24-May-09 20:37 lavis/datasets/datasets/discriminatory_reasoning_datasets.py
+-rw-rw-r--  2.0 unx     3315 b- defN 24-May-09 20:37 lavis/datasets/datasets/gqa_datasets.py
+-rw-rw-r--  2.0 unx     4613 b- defN 24-May-09 20:37 lavis/datasets/datasets/iconqa_datasets.py
+-rw-rw-r--  2.0 unx     1807 b- defN 24-May-09 20:37 lavis/datasets/datasets/image_text_pair_datasets.py
 -rw-rw-r--  2.0 unx     1669 b- defN 24-May-09 20:37 lavis/datasets/datasets/imagefolder_dataset.py
--rw-rw-r--  2.0 unx     2012 b- defN 24-May-09 21:02 lavis/datasets/datasets/laion_dataset.py
+-rw-rw-r--  2.0 unx     2600 b- defN 24-May-09 20:37 lavis/datasets/datasets/laion_dataset.py
+-rw-rw-r--  2.0 unx     1370 b- defN 24-May-09 20:37 lavis/datasets/datasets/llava150k_dataset.py
 -rw-rw-r--  2.0 unx      624 b- defN 24-May-09 20:37 lavis/datasets/datasets/multimodal_classification_datasets.py
+-rw-rw-r--  2.0 unx     3098 b- defN 24-May-09 20:37 lavis/datasets/datasets/music_avqa.py
 -rw-rw-r--  2.0 unx     2850 b- defN 24-May-09 20:37 lavis/datasets/datasets/nlvr_datasets.py
+-rw-rw-r--  2.0 unx     6997 b- defN 24-May-09 20:37 lavis/datasets/datasets/object3d_captioning_datasets.py
+-rw-rw-r--  2.0 unx     6068 b- defN 24-May-09 20:37 lavis/datasets/datasets/object3d_classification_datasets.py
+-rw-rw-r--  2.0 unx     2948 b- defN 24-May-09 20:37 lavis/datasets/datasets/object3d_qa_datasets.py
+-rw-rw-r--  2.0 unx     2327 b- defN 24-May-09 20:37 lavis/datasets/datasets/ocr_datasets.py
 -rw-rw-r--  2.0 unx     5123 b- defN 24-May-09 20:37 lavis/datasets/datasets/retrieval_datasets.py
--rw-rw-r--  2.0 unx     1728 b- defN 24-May-09 21:02 lavis/datasets/datasets/snli_ve_datasets.py
--rw-rw-r--  2.0 unx     1055 b- defN 24-May-09 21:02 lavis/datasets/datasets/vg_vqa_datasets.py
--rw-rw-r--  2.0 unx     1993 b- defN 24-May-09 21:02 lavis/datasets/datasets/video_caption_datasets.py
--rw-rw-r--  2.0 unx     1840 b- defN 24-May-09 21:02 lavis/datasets/datasets/video_vqa_datasets.py
--rw-rw-r--  2.0 unx     1384 b- defN 24-May-09 21:02 lavis/datasets/datasets/vqa_datasets.py
+-rw-rw-r--  2.0 unx     2461 b- defN 24-May-09 20:37 lavis/datasets/datasets/snli_ve_datasets.py
+-rw-rw-r--  2.0 unx     2190 b- defN 24-May-09 20:37 lavis/datasets/datasets/subject_driven_t2i_dataset.py
+-rw-rw-r--  2.0 unx     2392 b- defN 24-May-09 20:37 lavis/datasets/datasets/textcaps_datasets.py
+-rw-rw-r--  2.0 unx     3439 b- defN 24-May-09 20:37 lavis/datasets/datasets/valor_caption.py
+-rw-rw-r--  2.0 unx     3230 b- defN 24-May-09 20:37 lavis/datasets/datasets/vatex_captioning_datasets.py
+-rw-rw-r--  2.0 unx     1438 b- defN 24-May-09 20:37 lavis/datasets/datasets/vg_vqa_datasets.py
+-rw-rw-r--  2.0 unx     5929 b- defN 24-May-09 20:37 lavis/datasets/datasets/video_caption_datasets.py
+-rw-rw-r--  2.0 unx     2482 b- defN 24-May-09 20:37 lavis/datasets/datasets/video_vqa_datasets.py
+-rw-rw-r--  2.0 unx     3900 b- defN 24-May-09 20:37 lavis/datasets/datasets/violin_dataset.py
+-rw-rw-r--  2.0 unx     4682 b- defN 24-May-09 20:37 lavis/datasets/datasets/visdial_dialogue_datasets.py
+-rw-rw-r--  2.0 unx     1953 b- defN 24-May-09 20:37 lavis/datasets/datasets/vizwiz_vqa_datasets.py
+-rw-rw-r--  2.0 unx     2589 b- defN 24-May-09 20:37 lavis/datasets/datasets/vlep_dataset.py
+-rw-rw-r--  2.0 unx     1739 b- defN 24-May-09 20:37 lavis/datasets/datasets/vqa_datasets.py
+-rw-rw-r--  2.0 unx     3502 b- defN 24-May-09 20:37 lavis/datasets/datasets/vsr_datasets.py
+-rw-rw-r--  2.0 unx     3011 b- defN 24-May-09 20:37 lavis/datasets/datasets/yt8m_video_dialogue_datasets.py
+-rw-rw-r--  2.0 unx      813 b- defN 24-May-09 20:37 lavis/datasets/download_scripts/download_charade.py
 -rw-rw-r--  2.0 unx     1782 b- defN 24-May-09 20:37 lavis/datasets/download_scripts/download_coco.py
+-rw-rw-r--  2.0 unx     1826 b- defN 24-May-09 20:37 lavis/datasets/download_scripts/download_coin.py
 -rw-rw-r--  2.0 unx     1978 b- defN 24-May-09 20:37 lavis/datasets/download_scripts/download_didemo.py
 -rw-rw-r--  2.0 unx     1939 b- defN 24-May-09 20:37 lavis/datasets/download_scripts/download_flickr.py
 -rw-rw-r--  2.0 unx     1370 b- defN 24-May-09 20:37 lavis/datasets/download_scripts/download_gqa.py
+-rw-rw-r--  2.0 unx     1089 b- defN 24-May-09 20:37 lavis/datasets/download_scripts/download_iconqa.py
 -rw-rw-r--  2.0 unx     3179 b- defN 24-May-09 20:37 lavis/datasets/download_scripts/download_msrvtt.py
 -rw-rw-r--  2.0 unx     1810 b- defN 24-May-09 20:37 lavis/datasets/download_scripts/download_msvd.py
 -rw-rw-r--  2.0 unx     3962 b- defN 24-May-09 20:37 lavis/datasets/download_scripts/download_nocaps.py
 -rw-rw-r--  2.0 unx     2341 b- defN 24-May-09 20:37 lavis/datasets/download_scripts/download_sbu.py
 -rw-rw-r--  2.0 unx     1514 b- defN 24-May-09 20:37 lavis/datasets/download_scripts/download_vg.py
+-rw-rw-r--  2.0 unx      608 b- defN 24-May-09 20:37 lavis/datasets/download_scripts/download_violin.py
 -rw-rw-r--  2.0 unx     6597 b- defN 24-May-09 20:37 lavis/datasets/download_scripts/DownloadConceptualCaptions/download_data_cc12m.py
 -rw-rw-r--  2.0 unx     6546 b- defN 24-May-09 20:37 lavis/datasets/download_scripts/DownloadConceptualCaptions/download_data_cc3m.py
--rw-rw-r--  2.0 unx     8029 b- defN 24-May-09 21:02 lavis/models/__init__.py
--rw-rw-r--  2.0 unx     7853 b- defN 24-May-09 21:02 lavis/models/base_model.py
--rw-rw-r--  2.0 unx     9737 b- defN 24-May-09 21:02 lavis/models/clip_vit.py
--rw-rw-r--  2.0 unx    19526 b- defN 24-May-09 21:02 lavis/models/eva_vit.py
+-rw-rw-r--  2.0 unx     8440 b- defN 24-May-09 20:37 lavis/models/__init__.py
+-rw-rw-r--  2.0 unx     8638 b- defN 24-May-09 20:37 lavis/models/base_model.py
+-rw-rw-r--  2.0 unx     1624 b- defN 24-May-09 20:37 lavis/models/beats_encoder.py
+-rw-rw-r--  2.0 unx    10106 b- defN 24-May-09 20:37 lavis/models/clip_vit.py
+-rw-rw-r--  2.0 unx    20008 b- defN 24-May-09 20:37 lavis/models/eva_vit.py
 -rw-rw-r--  2.0 unx    54570 b- defN 24-May-09 20:37 lavis/models/med.py
 -rw-rw-r--  2.0 unx    19740 b- defN 24-May-09 20:37 lavis/models/vit.py
 -rw-rw-r--  2.0 unx     7181 b- defN 24-May-09 20:37 lavis/models/albef_models/__init__.py
 -rw-rw-r--  2.0 unx     5910 b- defN 24-May-09 20:37 lavis/models/albef_models/albef_classification.py
 -rw-rw-r--  2.0 unx     7564 b- defN 24-May-09 20:37 lavis/models/albef_models/albef_feature_extractor.py
 -rw-rw-r--  2.0 unx     9516 b- defN 24-May-09 20:37 lavis/models/albef_models/albef_nlvr.py
 -rw-rw-r--  2.0 unx     3236 b- defN 24-May-09 20:37 lavis/models/albef_models/albef_outputs.py
 -rw-rw-r--  2.0 unx    14875 b- defN 24-May-09 20:37 lavis/models/albef_models/albef_pretrain.py
 -rw-rw-r--  2.0 unx    12731 b- defN 24-May-09 20:37 lavis/models/albef_models/albef_retrieval.py
 -rw-rw-r--  2.0 unx    17038 b- defN 24-May-09 20:37 lavis/models/albef_models/albef_vqa.py
 -rw-rw-r--  2.0 unx     3673 b- defN 24-May-09 20:37 lavis/models/alpro_models/__init__.py
 -rw-rw-r--  2.0 unx     1664 b- defN 24-May-09 20:37 lavis/models/alpro_models/alpro_outputs.py
 -rw-rw-r--  2.0 unx     4457 b- defN 24-May-09 20:37 lavis/models/alpro_models/alpro_qa.py
 -rw-rw-r--  2.0 unx    14417 b- defN 24-May-09 20:37 lavis/models/alpro_models/alpro_retrieval.py
+-rw-rw-r--  2.0 unx     6926 b- defN 24-May-09 20:37 lavis/models/beats/BEATs.py
+-rw-rw-r--  2.0 unx     6468 b- defN 24-May-09 20:37 lavis/models/beats/Tokenizers.py
+-rw-rw-r--  2.0 unx    30762 b- defN 24-May-09 20:37 lavis/models/beats/backbone.py
+-rw-rw-r--  2.0 unx     7387 b- defN 24-May-09 20:37 lavis/models/beats/modules.py
+-rw-rw-r--  2.0 unx     8172 b- defN 24-May-09 20:37 lavis/models/beats/quantizer.py
 -rw-rw-r--  2.0 unx    48386 b- defN 24-May-09 20:37 lavis/models/blip2_models/Qformer.py
 -rw-rw-r--  2.0 unx        0 b- defN 24-May-09 20:37 lavis/models/blip2_models/__init__.py
--rw-rw-r--  2.0 unx     8014 b- defN 24-May-09 21:02 lavis/models/blip2_models/blip2.py
+-rw-rw-r--  2.0 unx    11260 b- defN 24-May-09 20:37 lavis/models/blip2_models/blip2.py
 -rw-rw-r--  2.0 unx     3945 b- defN 24-May-09 20:37 lavis/models/blip2_models/blip2_image_text_matching.py
--rw-rw-r--  2.0 unx    10176 b- defN 24-May-09 21:02 lavis/models/blip2_models/blip2_opt.py
--rw-rw-r--  2.0 unx    19667 b- defN 24-May-09 21:02 lavis/models/blip2_models/blip2_qformer.py
+-rw-rw-r--  2.0 unx    15863 b- defN 24-May-09 20:37 lavis/models/blip2_models/blip2_opt.py
+-rw-rw-r--  2.0 unx    20633 b- defN 24-May-09 20:37 lavis/models/blip2_models/blip2_qformer.py
 -rw-rw-r--  2.0 unx    13665 b- defN 24-May-09 20:37 lavis/models/blip2_models/blip2_t5.py
+-rw-rw-r--  2.0 unx    30599 b- defN 24-May-09 20:37 lavis/models/blip2_models/blip2_t5_instruct.py
+-rw-rw-r--  2.0 unx    28892 b- defN 24-May-09 20:37 lavis/models/blip2_models/blip2_vicuna_instruct.py
+-rw-rw-r--  2.0 unx   138338 b- defN 24-May-09 20:37 lavis/models/blip2_models/blip2_vicuna_xinstruct.py
+-rw-rw-r--  2.0 unx    39363 b- defN 24-May-09 20:37 lavis/models/blip2_models/modeling_llama.py
 -rw-rw-r--  2.0 unx    47286 b- defN 24-May-09 20:37 lavis/models/blip2_models/modeling_opt.py
 -rw-rw-r--  2.0 unx    86219 b- defN 24-May-09 20:37 lavis/models/blip2_models/modeling_t5.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-May-09 20:37 lavis/models/blip_diffusion_models/__init__.py
+-rw-rw-r--  2.0 unx    33706 b- defN 24-May-09 20:37 lavis/models/blip_diffusion_models/blip_diffusion.py
+-rw-rw-r--  2.0 unx     8775 b- defN 24-May-09 20:37 lavis/models/blip_diffusion_models/modeling_ctx_clip.py
+-rw-rw-r--  2.0 unx    22314 b- defN 24-May-09 20:37 lavis/models/blip_diffusion_models/ptp_utils.py
+-rw-rw-r--  2.0 unx     3332 b- defN 24-May-09 20:37 lavis/models/blip_diffusion_models/utils.py
 -rw-rw-r--  2.0 unx     3916 b- defN 24-May-09 20:37 lavis/models/blip_models/__init__.py
--rw-rw-r--  2.0 unx     2219 b- defN 24-May-09 21:02 lavis/models/blip_models/blip.py
+-rw-rw-r--  2.0 unx     2566 b- defN 24-May-09 20:37 lavis/models/blip_models/blip.py
 -rw-rw-r--  2.0 unx     8732 b- defN 24-May-09 20:37 lavis/models/blip_models/blip_caption.py
 -rw-rw-r--  2.0 unx     5773 b- defN 24-May-09 20:37 lavis/models/blip_models/blip_classification.py
 -rw-rw-r--  2.0 unx     7902 b- defN 24-May-09 20:37 lavis/models/blip_models/blip_feature_extractor.py
 -rw-rw-r--  2.0 unx     7444 b- defN 24-May-09 20:37 lavis/models/blip_models/blip_image_text_matching.py
 -rw-rw-r--  2.0 unx     7091 b- defN 24-May-09 20:37 lavis/models/blip_models/blip_nlvr.py
 -rw-rw-r--  2.0 unx     4276 b- defN 24-May-09 20:37 lavis/models/blip_models/blip_outputs.py
 -rw-rw-r--  2.0 unx    14988 b- defN 24-May-09 20:37 lavis/models/blip_models/blip_pretrain.py
@@ -223,34 +1287,53 @@
 -rw-rw-r--  2.0 unx     6937 b- defN 24-May-09 20:37 lavis/models/clip_models/pretrained.py
 -rw-rw-r--  2.0 unx    19038 b- defN 24-May-09 20:37 lavis/models/clip_models/timm_model.py
 -rw-rw-r--  2.0 unx     6673 b- defN 24-May-09 20:37 lavis/models/clip_models/tokenizer.py
 -rw-rw-r--  2.0 unx     3292 b- defN 24-May-09 20:37 lavis/models/clip_models/transform.py
 -rw-rw-r--  2.0 unx     2138 b- defN 24-May-09 20:37 lavis/models/clip_models/utils.py
 -rw-rw-r--  2.0 unx     3902 b- defN 24-May-09 20:37 lavis/models/gpt_models/gpt_dialogue.py
 -rw-rw-r--  2.0 unx      238 b- defN 24-May-09 20:37 lavis/models/img2prompt_models/__init__.py
--rw-rw-r--  2.0 unx    24363 b- defN 24-May-09 21:51 lavis/models/img2prompt_models/img2prompt_vqa.py
+-rw-rw-r--  2.0 unx    24631 b- defN 24-May-09 20:42 lavis/models/img2prompt_models/img2prompt_vqa.py
 -rw-rw-r--  2.0 unx     1251 b- defN 24-May-09 20:37 lavis/models/pnp_vqa_models/__init__.py
 -rw-rw-r--  2.0 unx     3113 b- defN 24-May-09 20:37 lavis/models/pnp_vqa_models/pnp_unifiedqav2_fid.py
 -rw-rw-r--  2.0 unx    16521 b- defN 24-May-09 20:37 lavis/models/pnp_vqa_models/pnp_vqa.py
 -rw-rw-r--  2.0 unx      280 b- defN 24-May-09 20:37 lavis/models/timesformer/__init__.py
 -rw-rw-r--  2.0 unx     3621 b- defN 24-May-09 20:37 lavis/models/timesformer/conv2d_same.py
 -rw-rw-r--  2.0 unx    12320 b- defN 24-May-09 20:37 lavis/models/timesformer/features.py
 -rw-rw-r--  2.0 unx    15418 b- defN 24-May-09 20:37 lavis/models/timesformer/helpers.py
 -rw-rw-r--  2.0 unx      702 b- defN 24-May-09 20:37 lavis/models/timesformer/linear.py
 -rw-rw-r--  2.0 unx    20265 b- defN 24-May-09 20:37 lavis/models/timesformer/vit.py
 -rw-rw-r--  2.0 unx     6686 b- defN 24-May-09 20:37 lavis/models/timesformer/vit_utils.py
--rw-rw-r--  2.0 unx     1336 b- defN 24-May-09 21:02 lavis/processors/__init__.py
--rw-rw-r--  2.0 unx     6263 b- defN 24-May-09 21:02 lavis/processors/alpro_processors.py
+-rw-rw-r--  2.0 unx     9903 b- defN 24-May-09 20:37 lavis/models/ulip_models/ULIP_models.py
+-rw-rw-r--  2.0 unx     2524 b- defN 24-May-09 20:37 lavis/models/ulip_models/losses.py
+-rw-rw-r--  2.0 unx     3910 b- defN 24-May-09 20:37 lavis/models/ulip_models/pointbert/checkpoint.py
+-rw-rw-r--  2.0 unx    13216 b- defN 24-May-09 20:37 lavis/models/ulip_models/pointbert/dvae.py
+-rw-rw-r--  2.0 unx     4922 b- defN 24-May-09 20:37 lavis/models/ulip_models/pointbert/logger.py
+-rw-rw-r--  2.0 unx     9292 b- defN 24-May-09 20:37 lavis/models/ulip_models/pointbert/misc.py
+-rw-rw-r--  2.0 unx     8783 b- defN 24-May-09 20:37 lavis/models/ulip_models/pointbert/point_encoder.py
+-rw-rw-r--  2.0 unx      242 b- defN 24-May-09 20:37 lavis/models/ulip_models/utils/__init__.py
+-rw-rw-r--  2.0 unx      362 b- defN 24-May-09 20:37 lavis/models/ulip_models/utils/build.py
+-rw-rw-r--  2.0 unx     2360 b- defN 24-May-09 20:37 lavis/models/ulip_models/utils/config.py
+-rw-rw-r--  2.0 unx     1280 b- defN 24-May-09 20:37 lavis/models/ulip_models/utils/io.py
+-rw-rw-r--  2.0 unx     4922 b- defN 24-May-09 20:37 lavis/models/ulip_models/utils/logger.py
+-rw-rw-r--  2.0 unx    10818 b- defN 24-May-09 20:37 lavis/models/ulip_models/utils/registry.py
+-rw-rw-r--  2.0 unx     5301 b- defN 24-May-09 20:37 lavis/models/ulip_models/utils/tokenizer.py
+-rw-rw-r--  2.0 unx     7432 b- defN 24-May-09 20:37 lavis/models/ulip_models/utils/utils.py
+-rw-rw-r--  2.0 unx     1897 b- defN 24-May-09 20:37 lavis/processors/__init__.py
+-rw-rw-r--  2.0 unx     8633 b- defN 24-May-09 20:37 lavis/processors/alpro_processors.py
+-rw-rw-r--  2.0 unx     5283 b- defN 24-May-09 20:37 lavis/processors/audio_processors.py
 -rw-rw-r--  2.0 unx      604 b- defN 24-May-09 20:37 lavis/processors/base_processor.py
+-rw-rw-r--  2.0 unx     2319 b- defN 24-May-09 20:37 lavis/processors/blip_diffusion_processors.py
 -rw-rw-r--  2.0 unx     6690 b- defN 24-May-09 20:37 lavis/processors/blip_processors.py
 -rw-rw-r--  2.0 unx     2570 b- defN 24-May-09 20:37 lavis/processors/clip_processors.py
 -rw-rw-r--  2.0 unx     3924 b- defN 24-May-09 20:37 lavis/processors/functional_video.py
 -rw-rw-r--  2.0 unx     5489 b- defN 24-May-09 20:37 lavis/processors/gpt_processors.py
+-rw-rw-r--  2.0 unx    22739 b- defN 24-May-09 20:37 lavis/processors/instruction_text_processors.py
 -rw-rw-r--  2.0 unx    11292 b- defN 24-May-09 20:37 lavis/processors/randaugment.py
 -rw-rw-r--  2.0 unx     5013 b- defN 24-May-09 20:37 lavis/processors/transforms_video.py
+-rw-rw-r--  2.0 unx     9297 b- defN 24-May-09 20:37 lavis/processors/ulip_processors.py
 -rw-rw-r--  2.0 unx      773 b- defN 24-May-09 20:37 lavis/projects/albef/eval/nlvr_eval.yaml
 -rw-rw-r--  2.0 unx      857 b- defN 24-May-09 20:37 lavis/projects/albef/eval/ret_coco_eval.yaml
 -rw-rw-r--  2.0 unx      859 b- defN 24-May-09 20:37 lavis/projects/albef/eval/ret_flickr30k_eval.yaml
 -rw-rw-r--  2.0 unx      786 b- defN 24-May-09 20:37 lavis/projects/albef/eval/snli_ve_eval.yaml
 -rw-rw-r--  2.0 unx      939 b- defN 24-May-09 20:37 lavis/projects/albef/eval/vqa_test.yaml
 -rw-rw-r--  2.0 unx      926 b- defN 24-May-09 20:37 lavis/projects/albef/eval/vqa_val.yaml
 -rw-rw-r--  2.0 unx     1237 b- defN 24-May-09 20:37 lavis/projects/albef/train/aokvqa_ft.yaml
@@ -287,55 +1370,423 @@
 -rw-rw-r--  2.0 unx     1886 b- defN 24-May-09 20:37 lavis/projects/blip/train/pretrain_14m.yaml
 -rw-rw-r--  2.0 unx     1279 b- defN 24-May-09 20:37 lavis/projects/blip/train/retrieval_coco_ft.yaml
 -rw-rw-r--  2.0 unx     1263 b- defN 24-May-09 20:37 lavis/projects/blip/train/retrieval_flickr_ft.yaml
 -rw-rw-r--  2.0 unx     1429 b- defN 24-May-09 20:37 lavis/projects/blip/train/vqav2_ft.yaml
 -rw-rw-r--  2.0 unx        0 b- defN 24-May-09 20:37 lavis/projects/blip2/eval/caption_coco_flant5xl_eval.yaml
 -rw-rw-r--  2.0 unx     1081 b- defN 24-May-09 20:37 lavis/projects/blip2/eval/caption_coco_opt2.7b_eval.yaml
 -rw-rw-r--  2.0 unx     1081 b- defN 24-May-09 20:37 lavis/projects/blip2/eval/caption_coco_opt6.7b_eval.yaml
+-rw-rw-r--  2.0 unx    10083 b- defN 24-May-09 20:37 lavis/projects/blip2/eval/caption_nocaps_out_domain_flant5xl_eval.yaml
+-rw-rw-r--  2.0 unx    10085 b- defN 24-May-09 20:37 lavis/projects/blip2/eval/caption_nocaps_out_domain_flant5xxl_eval.yaml
 -rw-rw-r--  2.0 unx     1096 b- defN 24-May-09 20:37 lavis/projects/blip2/eval/gqa_zeroshot_flant5xl_eval.yaml
 -rw-rw-r--  2.0 unx     1134 b- defN 24-May-09 20:37 lavis/projects/blip2/eval/okvqa_zeroshot_flant5xl_eval.yaml
 -rw-rw-r--  2.0 unx     1151 b- defN 24-May-09 20:37 lavis/projects/blip2/eval/ret_coco_eval.yaml
 -rw-rw-r--  2.0 unx      875 b- defN 24-May-09 20:37 lavis/projects/blip2/eval/ret_flickr_eval.yaml
 -rw-rw-r--  2.0 unx     1192 b- defN 24-May-09 20:37 lavis/projects/blip2/eval/vqav2_zeroshot_flant5xl_eval.yaml
+-rw-rw-r--  2.0 unx     1191 b- defN 24-May-09 20:37 lavis/projects/blip2/eval/vqav2_zeroshot_opt_eval.yaml
 -rw-rw-r--  2.0 unx     1394 b- defN 24-May-09 20:37 lavis/projects/blip2/train/caption_coco_ft.yaml
--rw-rw-r--  2.0 unx     1510 b- defN 24-May-09 21:02 lavis/projects/blip2/train/pretrain_stage1.yaml
+-rw-rw-r--  2.0 unx     1427 b- defN 24-May-09 20:37 lavis/projects/blip2/train/pretrain_stage1.yaml
 -rw-rw-r--  2.0 unx     1595 b- defN 24-May-09 20:37 lavis/projects/blip2/train/pretrain_stage2.yaml
+-rw-rw-r--  2.0 unx     1633 b- defN 24-May-09 20:37 lavis/projects/blip2/train/retrieval_coco_ft.yaml
+-rw-rw-r--  2.0 unx     1522 b- defN 24-May-09 20:37 lavis/projects/blip_diffusion/finetune-db-dog.yaml
+-rw-rw-r--  2.0 unx     1530 b- defN 24-May-09 20:37 lavis/projects/blip_diffusion/finetune-db-pink-dress.yaml
+-rw-rw-r--  2.0 unx     1536 b- defN 24-May-09 20:37 lavis/projects/blip_diffusion/finetune-db-shein-jacket.yaml
+-rw-rw-r--  2.0 unx     1454 b- defN 24-May-09 20:37 lavis/projects/blip_diffusion/finetune-db-template.yaml
 -rw-rw-r--  2.0 unx      942 b- defN 24-May-09 20:37 lavis/projects/clip/exp_coco_ret_eval.yaml
 -rw-rw-r--  2.0 unx      939 b- defN 24-May-09 20:37 lavis/projects/clip/exp_flickr_ret_eval.yaml
 -rw-rw-r--  2.0 unx      756 b- defN 24-May-09 20:37 lavis/projects/clip/exp_imnet_zs_eval.yaml
 -rw-rw-r--  2.0 unx      898 b- defN 24-May-09 20:37 lavis/projects/gpt/eval/dialogue_avsd_eval.yaml
 -rw-rw-r--  2.0 unx     1287 b- defN 24-May-09 20:37 lavis/projects/gpt/train/dialogue_avsd_ft.yaml
+-rw-rw-r--  2.0 unx     2340 b- defN 24-May-09 20:37 lavis/projects/instructblip/caption_coco_flant5xl_eval_test.yaml
+-rw-rw-r--  2.0 unx     2338 b- defN 24-May-09 20:37 lavis/projects/instructblip/caption_coco_flant5xl_eval_val.yaml
+-rw-rw-r--  2.0 unx     2342 b- defN 24-May-09 20:37 lavis/projects/instructblip/caption_coco_flant5xxl_eval_test.yaml
+-rw-rw-r--  2.0 unx     2340 b- defN 24-May-09 20:37 lavis/projects/instructblip/caption_coco_flant5xxl_eval_val.yaml
+-rw-rw-r--  2.0 unx     2346 b- defN 24-May-09 20:37 lavis/projects/instructblip/caption_coco_vicuna13b_eval_test.yaml
+-rw-rw-r--  2.0 unx     2344 b- defN 24-May-09 20:37 lavis/projects/instructblip/caption_coco_vicuna13b_eval_val.yaml
+-rw-rw-r--  2.0 unx     2343 b- defN 24-May-09 20:37 lavis/projects/instructblip/caption_coco_vicuna7b_eval_test.yaml
+-rw-rw-r--  2.0 unx     2341 b- defN 24-May-09 20:37 lavis/projects/instructblip/caption_coco_vicuna7b_eval_val.yaml
+-rw-rw-r--  2.0 unx     2466 b- defN 24-May-09 20:37 lavis/projects/instructblip/caption_msrvtt_flant5xl_eval_test.yaml
+-rw-rw-r--  2.0 unx     2497 b- defN 24-May-09 20:37 lavis/projects/instructblip/caption_msrvtt_flant5xl_eval_val.yaml
+-rw-rw-r--  2.0 unx     2499 b- defN 24-May-09 20:37 lavis/projects/instructblip/caption_msrvtt_flant5xxl_eval_test.yaml
+-rw-rw-r--  2.0 unx     2497 b- defN 24-May-09 20:37 lavis/projects/instructblip/caption_msrvtt_flant5xxl_eval_val.yaml
+-rw-rw-r--  2.0 unx     2471 b- defN 24-May-09 20:37 lavis/projects/instructblip/caption_msrvtt_vicuna13b_eval_test.yaml
+-rw-rw-r--  2.0 unx     2500 b- defN 24-May-09 20:37 lavis/projects/instructblip/caption_msrvtt_vicuna13b_eval_val.yaml
+-rw-rw-r--  2.0 unx     2472 b- defN 24-May-09 20:37 lavis/projects/instructblip/caption_msrvtt_vicuna7b_eval_test.yaml
+-rw-rw-r--  2.0 unx     2469 b- defN 24-May-09 20:37 lavis/projects/instructblip/caption_msrvtt_vicuna7b_eval_val.yaml
+-rw-rw-r--  2.0 unx    19231 b- defN 24-May-09 20:37 lavis/projects/instructblip/caption_msvd_flant5xl_eval.yaml
+-rw-rw-r--  2.0 unx    19233 b- defN 24-May-09 20:37 lavis/projects/instructblip/caption_msvd_flant5xxl_eval.yaml
+-rw-rw-r--  2.0 unx    19238 b- defN 24-May-09 20:37 lavis/projects/instructblip/caption_msvd_vicuna13b_eval.yaml
+-rw-rw-r--  2.0 unx    19236 b- defN 24-May-09 20:37 lavis/projects/instructblip/caption_msvd_vicuna7b_eval.yaml
+-rw-rw-r--  2.0 unx    10120 b- defN 24-May-09 20:37 lavis/projects/instructblip/caption_nocaps_out_domain_flant5xl_eval.yaml
+-rw-rw-r--  2.0 unx    10122 b- defN 24-May-09 20:37 lavis/projects/instructblip/caption_nocaps_out_domain_flant5xxl_eval.yaml
+-rw-rw-r--  2.0 unx    10126 b- defN 24-May-09 20:37 lavis/projects/instructblip/caption_nocaps_out_domain_vicuna13b_eval.yaml
+-rw-rw-r--  2.0 unx    10124 b- defN 24-May-09 20:37 lavis/projects/instructblip/caption_nocaps_out_domain_vicuna7b_eval.yaml
+-rw-rw-r--  2.0 unx     2439 b- defN 24-May-09 20:37 lavis/projects/instructblip/caption_vatex_flant5xl_eval.yaml
+-rw-rw-r--  2.0 unx     2441 b- defN 24-May-09 20:37 lavis/projects/instructblip/caption_vatex_flant5xxl_eval.yaml
+-rw-rw-r--  2.0 unx     2443 b- defN 24-May-09 20:37 lavis/projects/instructblip/caption_vatex_vicuna13b_eval.yaml
+-rw-rw-r--  2.0 unx     2445 b- defN 24-May-09 20:37 lavis/projects/instructblip/caption_vatex_vicuna7b_eval.yaml
+-rw-rw-r--  2.0 unx     3078 b- defN 24-May-09 20:37 lavis/projects/instructblip/classification_modelnet40_vicuna13b.yaml
+-rw-rw-r--  2.0 unx     3075 b- defN 24-May-09 20:37 lavis/projects/instructblip/classification_modelnet40_vicuna7b.yaml
+-rw-rw-r--  2.0 unx     2298 b- defN 24-May-09 20:37 lavis/projects/instructblip/classification_snlive_flant5xl.yaml
+-rw-rw-r--  2.0 unx     2302 b- defN 24-May-09 20:37 lavis/projects/instructblip/classification_snlive_flant5xxl.yaml
+-rw-rw-r--  2.0 unx     2268 b- defN 24-May-09 20:37 lavis/projects/instructblip/classification_snlive_vicuna13b.yaml
+-rw-rw-r--  2.0 unx     2270 b- defN 24-May-09 20:37 lavis/projects/instructblip/classification_snlive_vicuna13b_test.yaml
+-rw-rw-r--  2.0 unx     2270 b- defN 24-May-09 20:37 lavis/projects/instructblip/classification_snlive_vicuna7b_test.yaml
+-rw-rw-r--  2.0 unx     2268 b- defN 24-May-09 20:37 lavis/projects/instructblip/classification_snlive_vicuna7b_val.yaml
+-rw-rw-r--  2.0 unx     3050 b- defN 24-May-09 20:37 lavis/projects/instructblip/completion_modelnet40_vicuna13b.yaml
+-rw-rw-r--  2.0 unx     3074 b- defN 24-May-09 20:37 lavis/projects/instructblip/completion_modelnet40_vicuna7b.yaml
+-rw-rw-r--  2.0 unx     2478 b- defN 24-May-09 20:37 lavis/projects/instructblip/qa_msrvtt_flant5xl_eval_test.yaml
+-rw-rw-r--  2.0 unx     2480 b- defN 24-May-09 20:37 lavis/projects/instructblip/qa_msrvtt_flant5xxl_eval_test.yaml
+-rw-rw-r--  2.0 unx     2484 b- defN 24-May-09 20:37 lavis/projects/instructblip/qa_msrvtt_vicuna13b_eval_test.yaml
+-rw-rw-r--  2.0 unx     2482 b- defN 24-May-09 20:37 lavis/projects/instructblip/qa_msrvtt_vicuna7b_eval_test.yaml
+-rw-rw-r--  2.0 unx     3118 b- defN 24-May-09 20:37 lavis/projects/instructblip/qa_msvd_flant5xl_eval.yaml
+-rw-rw-r--  2.0 unx     3119 b- defN 24-May-09 20:37 lavis/projects/instructblip/qa_msvd_flant5xxl_eval.yaml
+-rw-rw-r--  2.0 unx     3123 b- defN 24-May-09 20:37 lavis/projects/instructblip/qa_msvd_vicuna13b_eval.yaml
+-rw-rw-r--  2.0 unx     3121 b- defN 24-May-09 20:37 lavis/projects/instructblip/qa_msvd_vicuna7b_eval.yaml
+-rw-rw-r--  2.0 unx     3039 b- defN 24-May-09 20:37 lavis/projects/instructblip/qa_okvqa_flant5xl_eval.yaml
+-rw-rw-r--  2.0 unx     3041 b- defN 24-May-09 20:37 lavis/projects/instructblip/qa_okvqa_flant5xxl_eval.yaml
+-rw-rw-r--  2.0 unx     3045 b- defN 24-May-09 20:37 lavis/projects/instructblip/qa_okvqa_vicuna13b_eval.yaml
+-rw-rw-r--  2.0 unx     3043 b- defN 24-May-09 20:37 lavis/projects/instructblip/qa_okvqa_vicuna7b_eval.yaml
 -rw-rw-r--  2.0 unx     1203 b- defN 24-May-09 20:37 lavis/projects/pnp-vqa/eval/gqa_eval.yaml
 -rw-rw-r--  2.0 unx     1202 b- defN 24-May-09 20:37 lavis/projects/pnp-vqa/eval/gqa_eval_3b.yaml
 -rw-rw-r--  2.0 unx     1210 b- defN 24-May-09 20:37 lavis/projects/pnp-vqa/eval/gqa_eval_large.yaml
 -rw-rw-r--  2.0 unx     1182 b- defN 24-May-09 20:37 lavis/projects/pnp-vqa/eval/okvqa_eval.yaml
 -rw-rw-r--  2.0 unx     1181 b- defN 24-May-09 20:37 lavis/projects/pnp-vqa/eval/okvqa_eval_3b.yaml
 -rw-rw-r--  2.0 unx     1189 b- defN 24-May-09 20:37 lavis/projects/pnp-vqa/eval/okvqa_eval_large.yaml
 -rw-rw-r--  2.0 unx     1202 b- defN 24-May-09 20:37 lavis/projects/pnp-vqa/eval/vqav2_eval.yaml
 -rw-rw-r--  2.0 unx     1201 b- defN 24-May-09 20:37 lavis/projects/pnp-vqa/eval/vqav2_eval_3b.yaml
 -rw-rw-r--  2.0 unx     1209 b- defN 24-May-09 20:37 lavis/projects/pnp-vqa/eval/vqav2_eval_large.yaml
 -rw-rw-r--  2.0 unx     1207 b- defN 24-May-09 20:37 lavis/projects/pnp-vqa/eval/vqav2_test_eval.yaml
 -rw-rw-r--  2.0 unx     1206 b- defN 24-May-09 20:37 lavis/projects/pnp-vqa/eval/vqav2_test_eval_3b.yaml
 -rw-rw-r--  2.0 unx     1214 b- defN 24-May-09 20:37 lavis/projects/pnp-vqa/eval/vqav2_test_eval_large.yaml
+-rw-rw-r--  2.0 unx     5353 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/discrn/audio_video_caption.yaml
+-rw-rw-r--  2.0 unx     5363 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/discrn/audio_video_caption_13b.yaml
+-rw-rw-r--  2.0 unx     5356 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/discrn/audio_video_describe.yaml
+-rw-rw-r--  2.0 unx     5394 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/discrn/audio_video_describe_13b.yaml
+-rw-rw-r--  2.0 unx     5387 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/discrn/audio_video_describe_nocue.yaml
+-rw-rw-r--  2.0 unx     5582 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/discrn/audio_video_describe_proj copy.yaml
+-rw-rw-r--  2.0 unx     5582 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/discrn/audio_video_describe_proj.yaml
+-rw-rw-r--  2.0 unx     5374 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/discrn/audio_video_describe_rand_init.yaml
+-rw-rw-r--  2.0 unx     4891 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/discrn/image_3d_caption.yaml
+-rw-rw-r--  2.0 unx     4900 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/discrn/image_3d_caption_13b.yaml
+-rw-rw-r--  2.0 unx     4892 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/discrn/image_3d_describe.yaml
+-rw-rw-r--  2.0 unx     4893 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/discrn/image_3d_describe_13b.yaml
+-rw-rw-r--  2.0 unx     4900 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/discrn/image_3d_describe_no_init.yaml
+-rw-rw-r--  2.0 unx     4925 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/discrn/image_3d_describe_nocue.yaml
+-rw-rw-r--  2.0 unx     5009 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/discrn/image_3d_describe_proj.yaml
+-rw-rw-r--  2.0 unx     5222 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/audio/audiocaps_captioning_qa.yaml
+-rw-rw-r--  2.0 unx     5064 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/audio/audiocaps_captioning_test.yaml
+-rw-rw-r--  2.0 unx     5062 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/audio/audiocaps_captioning_val.yaml
+-rw-rw-r--  2.0 unx     4755 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/audio/clothoQA_captioning.yaml
+-rw-rw-r--  2.0 unx     4730 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/audio/clothov1_captioning.yaml
+-rw-rw-r--  2.0 unx     4778 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/audio/clothov2_captioning.yaml
+-rw-rw-r--  2.0 unx     4569 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/audio/esc50_classification.yaml
+-rw-rw-r--  2.0 unx     4569 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/audio/esc50_classification_completion.yaml
+-rw-rw-r--  2.0 unx     5528 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/crossmodal/musicavqa/musicavqa_audio_eval.yaml
+-rw-rw-r--  2.0 unx     5526 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/crossmodal/musicavqa/musicavqa_joint_eval.yaml
+-rw-rw-r--  2.0 unx     5544 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/crossmodal/musicavqa/musicavqa_video_eval.yaml
+-rw-rw-r--  2.0 unx     5483 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/crossmodal/vatex/vatex_audio_captioning.yaml
+-rw-rw-r--  2.0 unx     5417 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/crossmodal/vatex/vatex_captioning.yaml
+-rw-rw-r--  2.0 unx     5496 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/crossmodal/vatex/vatex_joint_captioning.yaml
+-rw-rw-r--  2.0 unx     5533 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/crossmodal/vatex/vatex_joint_captioning_interleave.yaml
+-rw-rw-r--  2.0 unx     4931 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/image/coco_captioning_test.yaml
+-rw-rw-r--  2.0 unx     4929 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/image/coco_captioning_val.yaml
+-rw-rw-r--  2.0 unx     4719 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/image/flickr30k_captioning.yaml
+-rw-rw-r--  2.0 unx     4872 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/image/gqa_qa.yaml
+-rw-rw-r--  2.0 unx     4434 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/image/nocaps_captioning.yaml
+-rw-rw-r--  2.0 unx    12566 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/image/nocaps_out_domain_captioning.yaml
+-rw-rw-r--  2.0 unx     5706 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/image/okvqa_qa.yaml
+-rw-rw-r--  2.0 unx     4767 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/image/snlive_classification_test.yaml
+-rw-rw-r--  2.0 unx     4765 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/image/snlive_classification_val.yaml
+-rw-rw-r--  2.0 unx     4814 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/image/vizwiz_qa.yaml
+-rw-rw-r--  2.0 unx     4919 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/image_with_coco/coco_captioning_test.yaml
+-rw-rw-r--  2.0 unx     4917 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/image_with_coco/coco_captioning_val.yaml
+-rw-rw-r--  2.0 unx     4584 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/image_with_coco/flickr30k_captioning.yaml
+-rw-rw-r--  2.0 unx     4737 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/image_with_coco/gqa_qa.yaml
+-rw-rw-r--  2.0 unx     4436 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/image_with_coco/nocaps_captioning.yaml
+-rw-rw-r--  2.0 unx    12568 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/image_with_coco/nocaps_out_domain_captioning.yaml
+-rw-rw-r--  2.0 unx     5571 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/image_with_coco/okvqa_qa.yaml
+-rw-rw-r--  2.0 unx     4632 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/image_with_coco/snlive_classification_test.yaml
+-rw-rw-r--  2.0 unx     4630 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/image_with_coco/snlive_classification_val.yaml
+-rw-rw-r--  2.0 unx     4816 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/image_with_coco/vizwiz_qa.yaml
+-rw-rw-r--  2.0 unx     5384 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/pc/modelnet40_classification.yaml
+-rw-rw-r--  2.0 unx     5223 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/pc/modelnet40_completion.yaml
+-rw-rw-r--  2.0 unx     5486 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/pc/objaverse_captioning.yaml
+-rw-rw-r--  2.0 unx     5281 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/pc/objaverse_qa.yaml
+-rw-rw-r--  2.0 unx     4955 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/video/msrvtt_captioning.yaml
+-rw-rw-r--  2.0 unx     5101 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/video/msrvtt_captioning_test.yaml
+-rw-rw-r--  2.0 unx     5098 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/video/msrvtt_captioning_val.yaml
+-rw-rw-r--  2.0 unx     5138 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/video/msrvtt_qa_test.yaml
+-rw-rw-r--  2.0 unx     5136 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/video/msrvtt_qa_val.yaml
+-rw-rw-r--  2.0 unx    21887 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/video/msvd_captioning.yaml
+-rw-rw-r--  2.0 unx    22644 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/video/msvd_qa.yaml
+-rw-rw-r--  2.0 unx     5483 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/video/vatex_audio_captioning.yaml
+-rw-rw-r--  2.0 unx     5417 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/video/vatex_captioning.yaml
+-rw-rw-r--  2.0 unx     5496 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/video/vatex_joint_captioning.yaml
+-rw-rw-r--  2.0 unx     5533 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/video/vatex_joint_captioning_interleave.yaml
+-rw-rw-r--  2.0 unx    21893 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/video_image/msvd_captioning.yaml
+-rw-rw-r--  2.0 unx    22648 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/video_image/msvd_qa.yaml
+-rw-rw-r--  2.0 unx     5428 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna13b/video_image/vatex_captioning.yaml
+-rw-rw-r--  2.0 unx     4746 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/audio/audiocaps_captioning_qa.yaml
+-rw-rw-r--  2.0 unx     5021 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/audio/audiocaps_captioning_test.yaml
+-rw-rw-r--  2.0 unx     5019 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/audio/audiocaps_captioning_val.yaml
+-rw-rw-r--  2.0 unx     4775 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/audio/clothoQA_captioning.yaml
+-rw-rw-r--  2.0 unx     4586 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/audio/clothov1_captioning.yaml
+-rw-rw-r--  2.0 unx     4587 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/audio/clothov2_captioning.yaml
+-rw-rw-r--  2.0 unx     4496 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/audio/esc50_classification.yaml
+-rw-rw-r--  2.0 unx     4506 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/audio/esc50_classification_completion.yaml
+-rw-rw-r--  2.0 unx     5236 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/audio_no_init/audiocaps_captioning_qa.yaml
+-rw-rw-r--  2.0 unx     5059 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/audio_no_init/audiocaps_captioning_test.yaml
+-rw-rw-r--  2.0 unx     5057 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/audio_no_init/audiocaps_captioning_val.yaml
+-rw-rw-r--  2.0 unx     4782 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/audio_no_init/clothoQA_captioning.yaml
+-rw-rw-r--  2.0 unx     4757 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/audio_no_init/clothov1_captioning.yaml
+-rw-rw-r--  2.0 unx     4757 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/audio_no_init/clothov2_captioning.yaml
+-rw-rw-r--  2.0 unx     4596 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/audio_no_init/esc50_classification.yaml
+-rw-rw-r--  2.0 unx     4608 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/audio_no_init/esc50_classification_completion.yaml
+-rw-rw-r--  2.0 unx     5149 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/audio_projection_only/audiocaps_captioning_qa.yaml
+-rw-rw-r--  2.0 unx     5083 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/audio_projection_only/audiocaps_captioning_test.yaml
+-rw-rw-r--  2.0 unx     5081 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/audio_projection_only/audiocaps_captioning_val.yaml
+-rw-rw-r--  2.0 unx     4776 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/audio_projection_only/clothoQA_captioning.yaml
+-rw-rw-r--  2.0 unx     4677 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/audio_projection_only/clothov1_captioning.yaml
+-rw-rw-r--  2.0 unx     4677 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/audio_projection_only/clothov2_captioning.yaml
+-rw-rw-r--  2.0 unx     4661 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/audio_projection_only/esc50_classification.yaml
+-rw-rw-r--  2.0 unx     4676 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/audio_projection_only/esc50_classification_completion.yaml
+-rw-rw-r--  2.0 unx     5260 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/audio_projection_only_nocue/audiocaps_captioning_qa.yaml
+-rw-rw-r--  2.0 unx     5083 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/audio_projection_only_nocue/audiocaps_captioning_test.yaml
+-rw-rw-r--  2.0 unx     5081 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/audio_projection_only_nocue/audiocaps_captioning_val.yaml
+-rw-rw-r--  2.0 unx     4723 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/audio_projection_only_nocue/clothoQA_captioning.yaml
+-rw-rw-r--  2.0 unx     4677 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/audio_projection_only_nocue/clothov1_captioning.yaml
+-rw-rw-r--  2.0 unx     4677 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/audio_projection_only_nocue/clothov2_captioning.yaml
+-rw-rw-r--  2.0 unx     4668 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/audio_projection_only_nocue/esc50_classification.yaml
+-rw-rw-r--  2.0 unx     4676 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/audio_projection_only_nocue/esc50_classification_completion.yaml
+-rw-rw-r--  2.0 unx     5517 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/crossmodal/musicavqa/musicavqa_audio_eval.yaml
+-rw-rw-r--  2.0 unx     5548 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/crossmodal/musicavqa/musicavqa_joint_eval.yaml
+-rw-rw-r--  2.0 unx     5533 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/crossmodal/musicavqa/musicavqa_video_eval.yaml
+-rw-rw-r--  2.0 unx     5482 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/crossmodal/vatex/vatex_audio_captioning.yaml
+-rw-rw-r--  2.0 unx     5466 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/crossmodal/vatex/vatex_captioning.yaml
+-rw-rw-r--  2.0 unx     5500 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/crossmodal/vatex/vatex_joint_captioning.yaml
+-rw-rw-r--  2.0 unx     5537 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/crossmodal/vatex/vatex_joint_captioning_interleave.yaml
+-rw-rw-r--  2.0 unx     4921 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image/coco_captioning_test.yaml
+-rw-rw-r--  2.0 unx     4919 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image/coco_captioning_val.yaml
+-rw-rw-r--  2.0 unx     4709 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image/flickr30k_captioning.yaml
+-rw-rw-r--  2.0 unx     4870 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image/gqa_qa.yaml
+-rw-rw-r--  2.0 unx     4870 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image/gqa_qa_val.yaml
+-rw-rw-r--  2.0 unx     4563 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image/nocaps_captioning.yaml
+-rw-rw-r--  2.0 unx    12694 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image/nocaps_out_domain_captioning.yaml
+-rw-rw-r--  2.0 unx     5696 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image/okvqa_qa.yaml
+-rw-rw-r--  2.0 unx     4754 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image/snlive_classification_test.yaml
+-rw-rw-r--  2.0 unx     4752 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image/snlive_classification_val.yaml
+-rw-rw-r--  2.0 unx     4945 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image/vizwiz_qa.yaml
+-rw-rw-r--  2.0 unx     4931 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_full_init/coco_captioning_test.yaml
+-rw-rw-r--  2.0 unx     4919 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_full_init/coco_captioning_val.yaml
+-rw-rw-r--  2.0 unx     4729 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_full_init/flickr30k_captioning.yaml
+-rw-rw-r--  2.0 unx     4890 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_full_init/gqa_qa.yaml
+-rw-rw-r--  2.0 unx     4870 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_full_init/gqa_qa_val.yaml
+-rw-rw-r--  2.0 unx     4563 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_full_init/nocaps_captioning.yaml
+-rw-rw-r--  2.0 unx    12694 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_full_init/nocaps_out_domain_captioning.yaml
+-rw-rw-r--  2.0 unx     5696 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_full_init/okvqa_qa.yaml
+-rw-rw-r--  2.0 unx     4754 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_full_init/snlive_classification_test.yaml
+-rw-rw-r--  2.0 unx     4752 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_full_init/snlive_classification_val.yaml
+-rw-rw-r--  2.0 unx     4945 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_full_init/vizwiz_qa.yaml
+-rw-rw-r--  2.0 unx     4931 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_no_init/coco_captioning_test.yaml
+-rw-rw-r--  2.0 unx     4919 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_no_init/coco_captioning_val.yaml
+-rw-rw-r--  2.0 unx     4725 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_no_init/flickr30k_captioning.yaml
+-rw-rw-r--  2.0 unx     4886 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_no_init/gqa_qa.yaml
+-rw-rw-r--  2.0 unx     4870 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_no_init/gqa_qa_val.yaml
+-rw-rw-r--  2.0 unx     4579 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_no_init/nocaps_captioning.yaml
+-rw-rw-r--  2.0 unx    12694 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_no_init/nocaps_out_domain_captioning.yaml
+-rw-rw-r--  2.0 unx     5696 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_no_init/okvqa_qa.yaml
+-rw-rw-r--  2.0 unx     4754 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_no_init/snlive_classification_test.yaml
+-rw-rw-r--  2.0 unx     4752 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_no_init/snlive_classification_val.yaml
+-rw-rw-r--  2.0 unx     4953 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_no_init/vizwiz_qa.yaml
+-rw-rw-r--  2.0 unx     4793 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_pre_coco/coco_captioning_test.yaml
+-rw-rw-r--  2.0 unx     4792 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_pre_coco/coco_captioning_val.yaml
+-rw-rw-r--  2.0 unx     4583 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_pre_coco/flickr30k_captioning.yaml
+-rw-rw-r--  2.0 unx     4744 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_pre_coco/gqa_qa.yaml
+-rw-rw-r--  2.0 unx     4437 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_pre_coco/nocaps_captioning.yaml
+-rw-rw-r--  2.0 unx    12568 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_pre_coco/nocaps_out_domain_captioning.yaml
+-rw-rw-r--  2.0 unx     5570 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_pre_coco/okvqa_qa.yaml
+-rw-rw-r--  2.0 unx     4628 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_pre_coco/snlive_classification_test.yaml
+-rw-rw-r--  2.0 unx     4626 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_pre_coco/snlive_classification_val.yaml
+-rw-rw-r--  2.0 unx     4817 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_pre_coco/vizwiz_qa.yaml
+-rw-rw-r--  2.0 unx     4931 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_projection_only/coco_captioning_test.yaml
+-rw-rw-r--  2.0 unx     4919 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_projection_only/coco_captioning_val.yaml
+-rw-rw-r--  2.0 unx     4658 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_projection_only/flickr30k_captioning.yaml
+-rw-rw-r--  2.0 unx     4817 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_projection_only/gqa_qa.yaml
+-rw-rw-r--  2.0 unx     4870 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_projection_only/gqa_qa_val.yaml
+-rw-rw-r--  2.0 unx     4510 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_projection_only/nocaps_captioning.yaml
+-rw-rw-r--  2.0 unx    12621 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_projection_only/nocaps_out_domain_captioning.yaml
+-rw-rw-r--  2.0 unx     5696 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_projection_only/okvqa_qa.yaml
+-rw-rw-r--  2.0 unx     4754 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_projection_only/snlive_classification_test.yaml
+-rw-rw-r--  2.0 unx     4752 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_projection_only/snlive_classification_val.yaml
+-rw-rw-r--  2.0 unx     4889 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/image_projection_only/vizwiz_qa.yaml
+-rw-rw-r--  2.0 unx     5380 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/pc/modelnet40_classification.yaml
+-rw-rw-r--  2.0 unx     5494 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/pc/modelnet40_completion.yaml
+-rw-rw-r--  2.0 unx     5475 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/pc/objaverse_captioning.yaml
+-rw-rw-r--  2.0 unx     5271 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/pc/objaverse_qa.yaml
+-rw-rw-r--  2.0 unx     5396 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/pc_no_init/modelnet40_classification.yaml
+-rw-rw-r--  2.0 unx     5502 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/pc_no_init/modelnet40_completion.yaml
+-rw-rw-r--  2.0 unx     5475 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/pc_no_init/objaverse_captioning.yaml
+-rw-rw-r--  2.0 unx     5271 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/pc_no_init/objaverse_qa.yaml
+-rw-rw-r--  2.0 unx     5492 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/pc_projection_only/modelnet40_classification.yaml
+-rw-rw-r--  2.0 unx     5767 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/pc_projection_only/modelnet40_completion.yaml
+-rw-rw-r--  2.0 unx     5544 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/pc_projection_only/objaverse_captioning.yaml
+-rw-rw-r--  2.0 unx     5297 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/pc_projection_only/objaverse_qa.yaml
+-rw-rw-r--  2.0 unx     5405 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip1/modelnet40_classification.yaml
+-rw-rw-r--  2.0 unx     5635 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip1/modelnet40_completion.yaml
+-rw-rw-r--  2.0 unx     5484 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip1/objaverse_captioning.yaml
+-rw-rw-r--  2.0 unx     5278 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip1/objaverse_qa.yaml
+-rw-rw-r--  2.0 unx     5428 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip2_scaled_up/modelnet40_classification.yaml
+-rw-rw-r--  2.0 unx     5657 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip2_scaled_up/modelnet40_completion.yaml
+-rw-rw-r--  2.0 unx     5639 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip2_scaled_up/objaverse_captioning.yaml
+-rw-rw-r--  2.0 unx     5292 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip2_scaled_up/objaverse_qa.yaml
+-rw-rw-r--  2.0 unx     5413 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip_objaverse/modelnet40_classification.yaml
+-rw-rw-r--  2.0 unx     5643 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip_objaverse/modelnet40_completion.yaml
+-rw-rw-r--  2.0 unx     5491 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip_objaverse/objaverse_captioning.yaml
+-rw-rw-r--  2.0 unx     5285 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip_objaverse/objaverse_qa.yaml
+-rw-rw-r--  2.0 unx     5481 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip_objaverse_shapenet/modelnet40_classification.yaml
+-rw-rw-r--  2.0 unx     5710 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip_objaverse_shapenet/modelnet40_completion.yaml
+-rw-rw-r--  2.0 unx     5536 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip_objaverse_shapenet/objaverse_captioning.yaml
+-rw-rw-r--  2.0 unx     5330 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip_objaverse_shapenet/objaverse_qa.yaml
+-rw-rw-r--  2.0 unx     5460 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip_shapenet/modelnet40_classification.yaml
+-rw-rw-r--  2.0 unx     5786 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip_shapenet/modelnet40_completion.yaml
+-rw-rw-r--  2.0 unx     5520 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip_shapenet/objaverse_captioning.yaml
+-rw-rw-r--  2.0 unx     5314 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip_shapenet/objaverse_qa.yaml
+-rw-rw-r--  2.0 unx     5090 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/video/msrvtt_captioning_test.yaml
+-rw-rw-r--  2.0 unx     5088 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/video/msrvtt_captioning_val.yaml
+-rw-rw-r--  2.0 unx     5164 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/video/msrvtt_qa_test.yaml
+-rw-rw-r--  2.0 unx     5126 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/video/msrvtt_qa_val.yaml
+-rw-rw-r--  2.0 unx    21882 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/video/msvd_captioning.yaml
+-rw-rw-r--  2.0 unx    22590 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/video/msvd_qa.yaml
+-rw-rw-r--  2.0 unx     5466 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/video/vatex_captioning.yaml
+-rw-rw-r--  2.0 unx    21882 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/video_image/msvd_captioning.yaml
+-rw-rw-r--  2.0 unx    22626 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/video_image/msvd_qa.yaml
+-rw-rw-r--  2.0 unx     5335 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/video_image/vatex_captioning.yaml
+-rw-rw-r--  2.0 unx    21755 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/video_image_pre_coco/msvd_captioning.yaml
+-rw-rw-r--  2.0 unx    22499 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/video_image_pre_coco/msvd_qa.yaml
+-rw-rw-r--  2.0 unx     4966 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/video_image_pre_coco/vatex_captioning.yaml
+-rw-rw-r--  2.0 unx     5105 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/video_no_upsample/msrvtt_captioning_test.yaml
+-rw-rw-r--  2.0 unx     5115 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/video_no_upsample/msrvtt_captioning_val.yaml
+-rw-rw-r--  2.0 unx     5173 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/video_no_upsample/msrvtt_qa_test.yaml
+-rw-rw-r--  2.0 unx     5141 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/video_no_upsample/msrvtt_qa_val.yaml
+-rw-rw-r--  2.0 unx    21874 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/video_no_upsample/msvd_captioning.yaml
+-rw-rw-r--  2.0 unx    21903 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/video_no_upsample/msvd_captioning_up.yaml
+-rw-rw-r--  2.0 unx    22759 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/video_no_upsample/msvd_qa.yaml
+-rw-rw-r--  2.0 unx    22755 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/video_no_upsample/msvd_qa_up.yaml
+-rw-rw-r--  2.0 unx     5101 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/video_no_upsample/vatex_captioning.yaml
+-rw-rw-r--  2.0 unx     5099 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b/video_no_upsample/vatex_captioning_up.yaml
+-rw-rw-r--  2.0 unx     5250 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/audio/audiocaps_captioning_qa.yaml
+-rw-rw-r--  2.0 unx     5096 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/audio/audiocaps_captioning_test.yaml
+-rw-rw-r--  2.0 unx     5094 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/audio/audiocaps_captioning_val.yaml
+-rw-rw-r--  2.0 unx     4787 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/audio/clothoQA_captioning.yaml
+-rw-rw-r--  2.0 unx     4762 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/audio/clothov1_captioning.yaml
+-rw-rw-r--  2.0 unx     4758 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/audio/clothov2_captioning.yaml
+-rw-rw-r--  2.0 unx     4601 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/audio/esc50_classification.yaml
+-rw-rw-r--  2.0 unx     4612 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/audio/esc50_classification_completion.yaml
+-rw-rw-r--  2.0 unx     5555 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/crossmodal/musicavqa/musicavqa_audio_eval.yaml
+-rw-rw-r--  2.0 unx     5585 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/crossmodal/musicavqa/musicavqa_joint_eval.yaml
+-rw-rw-r--  2.0 unx     5570 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/crossmodal/musicavqa/musicavqa_video_eval.yaml
+-rw-rw-r--  2.0 unx     5501 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/crossmodal/vatex/vatex_audio_captioning.yaml
+-rw-rw-r--  2.0 unx     5449 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/crossmodal/vatex/vatex_captioning.yaml
+-rw-rw-r--  2.0 unx     5517 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/crossmodal/vatex/vatex_joint_captioning.yaml
+-rw-rw-r--  2.0 unx     4958 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/image/coco_captioning_test.yaml
+-rw-rw-r--  2.0 unx     4956 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/image/coco_captioning_val.yaml
+-rw-rw-r--  2.0 unx     4746 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/image/flickr30k_captioning.yaml
+-rw-rw-r--  2.0 unx     4907 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/image/gqa_qa.yaml
+-rw-rw-r--  2.0 unx     4601 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/image/nocaps_captioning.yaml
+-rw-rw-r--  2.0 unx    12731 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/image/nocaps_out_domain_captioning.yaml
+-rw-rw-r--  2.0 unx     5737 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/image/okvqa_qa.yaml
+-rw-rw-r--  2.0 unx     4754 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/image/snlive_classification_test.yaml
+-rw-rw-r--  2.0 unx     4752 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/image/snlive_classification_val.yaml
+-rw-rw-r--  2.0 unx     4981 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/image/vizwiz_qa.yaml
+-rw-rw-r--  2.0 unx     5410 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/pc/modelnet40_classification.yaml
+-rw-rw-r--  2.0 unx     5282 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/pc/modelnet40_completion.yaml
+-rw-rw-r--  2.0 unx     5507 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/pc/objaverse_captioning.yaml
+-rw-rw-r--  2.0 unx     5297 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/pc/objaverse_qa.yaml
+-rw-rw-r--  2.0 unx     5128 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/video/msrvtt_captioning_test.yaml
+-rw-rw-r--  2.0 unx     5125 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/video/msrvtt_captioning_val.yaml
+-rw-rw-r--  2.0 unx     5159 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/video/msrvtt_qa_test.yaml
+-rw-rw-r--  2.0 unx     5163 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/video/msrvtt_qa_val.yaml
+-rw-rw-r--  2.0 unx    21843 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/video/msvd_captioning.yaml
+-rw-rw-r--  2.0 unx     5750 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/video/msvd_qa.yaml
+-rw-rw-r--  2.0 unx     5449 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/video/vatex_captioning.yaml
+-rw-rw-r--  2.0 unx    21863 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/video_image/msvd_captioning.yaml
+-rw-rw-r--  2.0 unx     5808 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/video_image/msvd_qa.yaml
+-rw-rw-r--  2.0 unx     5454 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/video_image/vatex_captioning.yaml
+-rw-rw-r--  2.0 unx     2123 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/prompt_variation/nocaps/instructblip/original.yaml
+-rw-rw-r--  2.0 unx     2188 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/prompt_variation/nocaps/instructblip/template_1.yaml
+-rw-rw-r--  2.0 unx     2179 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/prompt_variation/nocaps/instructblip/template_2.yaml
+-rw-rw-r--  2.0 unx     2210 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/prompt_variation/nocaps/instructblip/template_3.yaml
+-rw-rw-r--  2.0 unx     2194 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/prompt_variation/nocaps/instructblip/template_4.yaml
+-rw-rw-r--  2.0 unx     2190 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/prompt_variation/nocaps/instructblip/template_5.yaml
+-rw-rw-r--  2.0 unx     4623 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/prompt_variation/nocaps/xinstructblip/template_1.yaml
+-rw-rw-r--  2.0 unx     4616 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/prompt_variation/nocaps/xinstructblip/template_2.yaml
+-rw-rw-r--  2.0 unx     4645 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/prompt_variation/nocaps/xinstructblip/template_3.yaml
+-rw-rw-r--  2.0 unx     4629 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/prompt_variation/nocaps/xinstructblip/template_4.yaml
+-rw-rw-r--  2.0 unx     4621 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/prompt_variation/nocaps/xinstructblip/template_5.yaml
+-rw-rw-r--  2.0 unx     6012 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/train/vicuna13b/audio_training.yaml
+-rw-rw-r--  2.0 unx     9947 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/train/vicuna13b/audio_training_continue.yaml
+-rw-rw-r--  2.0 unx     8815 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/train/vicuna13b/image_train.yaml
+-rw-rw-r--  2.0 unx    18084 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/train/vicuna13b/image_train_continue.yaml
+-rw-rw-r--  2.0 unx     4897 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/train/vicuna13b/pc_training.yaml
+-rw-rw-r--  2.0 unx     5542 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/train/vicuna13b/video_training.yaml
+-rw-rw-r--  2.0 unx     5998 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/train/vicuna7b/audio_training.yaml
+-rw-rw-r--  2.0 unx     6052 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/train/vicuna7b/audio_training_improved.yaml
+-rw-rw-r--  2.0 unx     7213 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/train/vicuna7b/audio_training_no_init.yaml
+-rw-rw-r--  2.0 unx     5960 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/train/vicuna7b/audio_training_projection_only.yaml
+-rw-rw-r--  2.0 unx     5968 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/train/vicuna7b/audio_training_projection_only_nocue.yaml
+-rw-rw-r--  2.0 unx     8918 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/train/vicuna7b/image_train.yaml
+-rw-rw-r--  2.0 unx     8963 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/train/vicuna7b/image_train_improved.yaml
+-rw-rw-r--  2.0 unx     8829 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/train/vicuna7b/image_train_no_init.yaml
+-rw-rw-r--  2.0 unx     8864 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/train/vicuna7b/image_train_projection_only.yaml
+-rw-rw-r--  2.0 unx    32089 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/train/vicuna7b/lora_training.yaml
+-rw-rw-r--  2.0 unx     4893 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/train/vicuna7b/pc_training.yaml
+-rw-rw-r--  2.0 unx     4922 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/train/vicuna7b/pc_training_improved.yaml
+-rw-rw-r--  2.0 unx     4797 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/train/vicuna7b/pc_training_no_init.yaml
+-rw-rw-r--  2.0 unx     4839 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/train/vicuna7b/pc_training_projection_only.yaml
+-rw-rw-r--  2.0 unx     4840 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/train/vicuna7b/pc_training_projection_only_nocue.yaml
+-rw-rw-r--  2.0 unx     4892 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/train/vicuna7b/pc_training_scaled_up.yaml
+-rw-rw-r--  2.0 unx     4900 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/train/vicuna7b/pc_training_ulip1.yaml
+-rw-rw-r--  2.0 unx     4926 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/train/vicuna7b/pc_training_ulip2_objaverse_shapenet_k_1.yaml
+-rw-rw-r--  2.0 unx     4905 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/train/vicuna7b/pc_training_ulip_objaverse.yaml
+-rw-rw-r--  2.0 unx     4900 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/train/vicuna7b/pc_training_ulip_shapenet.yaml
+-rw-rw-r--  2.0 unx     5535 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/train/vicuna7b/video_training.yaml
+-rw-rw-r--  2.0 unx     5554 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/train/vicuna7b/video_training_no_msrvtt_upsample.yaml
+-rw-rw-r--  2.0 unx     5911 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/train/vicuna7b_nocue/audio_training.yaml
+-rw-rw-r--  2.0 unx     8854 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/train/vicuna7b_nocue/image_train.yaml
+-rw-rw-r--  2.0 unx     4901 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/train/vicuna7b_nocue/pc_training.yaml
+-rw-rw-r--  2.0 unx     5560 b- defN 24-May-09 20:37 lavis/projects/xinstruct_blip/train/vicuna7b_nocue/video_training.yaml
 -rw-rw-r--  2.0 unx      360 b- defN 24-May-09 20:37 lavis/runners/__init__.py
--rw-rw-r--  2.0 unx    22634 b- defN 24-May-09 21:02 lavis/runners/runner_base.py
--rw-rw-r--  2.0 unx    12507 b- defN 24-May-09 21:02 lavis/runners/runner_iter.py
--rw-rw-r--  2.0 unx     1307 b- defN 24-May-09 21:02 lavis/tasks/__init__.py
--rw-rw-r--  2.0 unx     8759 b- defN 24-May-09 21:02 lavis/tasks/base_task.py
--rw-rw-r--  2.0 unx     4463 b- defN 24-May-09 21:02 lavis/tasks/captioning.py
+-rw-rw-r--  2.0 unx    23509 b- defN 24-May-09 20:37 lavis/runners/runner_base.py
+-rw-rw-r--  2.0 unx    13601 b- defN 24-May-09 20:37 lavis/runners/runner_iter.py
+-rw-rw-r--  2.0 unx     1444 b- defN 24-May-09 20:37 lavis/tasks/__init__.py
+-rw-rw-r--  2.0 unx     9274 b- defN 24-May-09 20:37 lavis/tasks/base_task.py
+-rw-rw-r--  2.0 unx    11009 b- defN 24-May-09 20:37 lavis/tasks/captioning.py
 -rw-rw-r--  2.0 unx     3919 b- defN 24-May-09 20:37 lavis/tasks/dialogue.py
 -rw-rw-r--  2.0 unx      526 b- defN 24-May-09 20:37 lavis/tasks/image_text_pretrain.py
--rw-rw-r--  2.0 unx     2458 b- defN 24-May-09 21:02 lavis/tasks/multimodal_classification.py
+-rw-rw-r--  2.0 unx     4287 b- defN 24-May-09 20:37 lavis/tasks/multimodal_classification.py
 -rw-rw-r--  2.0 unx     3208 b- defN 24-May-09 20:37 lavis/tasks/retrieval.py
--rw-rw-r--  2.0 unx    10072 b- defN 24-May-09 21:02 lavis/tasks/vqa.py
+-rw-rw-r--  2.0 unx      586 b- defN 24-May-09 20:37 lavis/tasks/text_to_image_generation.py
+-rw-rw-r--  2.0 unx    17116 b- defN 24-May-09 20:37 lavis/tasks/vqa.py
 -rw-rw-r--  2.0 unx     8745 b- defN 24-May-09 20:37 lavis/tasks/vqa_reading_comprehension.py
--rw-rw-r--  2.0 unx     5184 b- defN 24-May-09 21:02 projects/img2prompt-vqa/img2prompt_vqa.py
+-rw-rw-r--  2.0 unx     5184 b- defN 24-May-09 20:37 projects/img2llm-vqa/img2llm_vqa.py
+-rw-rw-r--  2.0 unx     3039 b- defN 24-May-09 20:37 projects/instructblip/run_demo.py
+-rw-rw-r--  2.0 unx     4986 b- defN 24-May-09 20:37 projects/xinstructblip/data_aug/3d_qa_data_generation.py
+-rw-rw-r--  2.0 unx     3608 b- defN 24-May-09 20:37 projects/xinstructblip/data_aug/audio_qa_data_generation.py
+-rw-rw-r--  2.0 unx     8920 b- defN 24-May-09 20:37 projects/xinstructblip/demo/run_demo.py
+-rw-rw-r--  2.0 unx     2052 b- defN 24-May-09 20:37 projects/xinstructblip/discrn/caption_baseline/predict_audio.py
+-rw-rw-r--  2.0 unx     6447 b- defN 24-May-09 20:37 projects/xinstructblip/discrn/caption_baseline/predict_image.py
+-rw-rw-r--  2.0 unx     6436 b- defN 24-May-09 20:37 projects/xinstructblip/discrn/caption_baseline/predict_pc.py
+-rw-rw-r--  2.0 unx     6652 b- defN 24-May-09 20:37 projects/xinstructblip/discrn/caption_baseline/predict_video.py
+-rw-rw-r--  2.0 unx     2030 b- defN 24-May-09 20:37 projects/xinstructblip/discrn/caption_baseline/render_images.py
+-rw-rw-r--  2.0 unx     8764 b- defN 24-May-09 20:37 projects/xinstructblip/discrn/data_generation/audiocaps_video_audio.py
+-rw-rw-r--  2.0 unx     9302 b- defN 24-May-09 20:37 projects/xinstructblip/discrn/data_generation/objaverse_img_3d.py
+-rw-rw-r--  2.0 unx     1483 b- defN 24-May-09 20:37 projects/xinstructblip/modelnet_baseline/render_images.py
 -rw-rw-r--  2.0 unx     5126 b- defN 24-May-09 20:37 tests/models/test_albef.py
 -rw-rw-r--  2.0 unx    11612 b- defN 24-May-09 20:37 tests/models/test_blip.py
 -rw-rw-r--  2.0 unx     5216 b- defN 24-May-09 20:37 tests/models/test_blip2.py
 -rw-rw-r--  2.0 unx     4235 b- defN 24-May-09 20:37 tests/models/test_pnp_vqa.py
--rw-rw-r--  2.0 unx     1502 b- defN 24-May-09 21:52 lavis_gml-1.0.2.post3.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx    18606 b- defN 24-May-09 21:52 lavis_gml-1.0.2.post3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-May-09 21:52 lavis_gml-1.0.2.post3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       76 b- defN 24-May-09 21:52 lavis_gml-1.0.2.post3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    33202 b- defN 24-May-09 21:52 lavis_gml-1.0.2.post3.dist-info/RECORD
-339 files, 2775296 bytes uncompressed, 1774391 bytes compressed:  36.1%
+-rw-rw-r--  2.0 unx     1502 b- defN 24-May-09 20:55 lavis_gml-1.0.3.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx    21582 b- defN 24-May-09 20:55 lavis_gml-1.0.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-09 20:55 lavis_gml-1.0.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       82 b- defN 24-May-09 20:54 lavis_gml-1.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx   209588 b- defN 24-May-09 20:55 lavis_gml-1.0.3.dist-info/RECORD
+1790 files, 40925671 bytes uncompressed, 9528675 bytes compressed:  76.7%
```

## zipnote {}

```diff
@@ -30,14 +30,1748 @@
 
 Filename: app/utils.py
 Comment: 
 
 Filename: app/vqa.py
 Comment: 
 
+Filename: build/lib/app/__init__.py
+Comment: 
+
+Filename: build/lib/app/calculate_coco_features.py
+Comment: 
+
+Filename: build/lib/app/caption.py
+Comment: 
+
+Filename: build/lib/app/classification.py
+Comment: 
+
+Filename: build/lib/app/dataset_browser.py
+Comment: 
+
+Filename: build/lib/app/image_text_match.py
+Comment: 
+
+Filename: build/lib/app/main.py
+Comment: 
+
+Filename: build/lib/app/multimodal_search.py
+Comment: 
+
+Filename: build/lib/app/multipage.py
+Comment: 
+
+Filename: build/lib/app/text_localization.py
+Comment: 
+
+Filename: build/lib/app/utils.py
+Comment: 
+
+Filename: build/lib/app/vqa.py
+Comment: 
+
+Filename: build/lib/docs/conf.py
+Comment: 
+
+Filename: build/lib/lavis/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/config.py
+Comment: 
+
+Filename: build/lib/lavis/common/dist_utils.py
+Comment: 
+
+Filename: build/lib/lavis/common/gradcam.py
+Comment: 
+
+Filename: build/lib/lavis/common/logger.py
+Comment: 
+
+Filename: build/lib/lavis/common/optims.py
+Comment: 
+
+Filename: build/lib/lavis/common/registry.py
+Comment: 
+
+Filename: build/lib/lavis/common/utils.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/util.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/canny/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/hed/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/midas/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/midas/api.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/midas/utils.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/midas/midas/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/midas/midas/base_model.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/midas/midas/blocks.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/midas/midas/dpt_depth.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/midas/midas/midas_net.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/midas/midas/midas_net_custom.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/midas/midas/transforms.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/midas/midas/vit.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/mlsd/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/mlsd/utils.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/mlsd/models/mbv2_mlsd_large.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/mlsd/models/mbv2_mlsd_tiny.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/openpose/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/openpose/body.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/openpose/hand.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/openpose/model.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/openpose/util.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/default_runtime.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/datasets/ade20k.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/datasets/chase_db1.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/datasets/cityscapes.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/datasets/cityscapes_769x769.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/datasets/drive.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/datasets/hrf.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/datasets/pascal_context.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/datasets/pascal_context_59.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/datasets/pascal_voc12.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/datasets/pascal_voc12_aug.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/datasets/stare.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/models/ann_r50-d8.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/models/apcnet_r50-d8.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/models/ccnet_r50-d8.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/models/cgnet.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/models/danet_r50-d8.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/models/deeplabv3_r50-d8.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/models/dmnet_r50-d8.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/models/dnl_r50-d8.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/models/emanet_r50-d8.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/models/encnet_r50-d8.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/models/fast_scnn.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/models/fcn_hr18.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/models/fcn_r50-d8.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/models/fcn_unet_s5-d16.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/models/fpn_r50.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/models/fpn_uniformer.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/models/gcnet_r50-d8.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/models/lraspp_m-v3-d8.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/models/nonlocal_r50-d8.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/models/ocrnet_hr18.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/models/ocrnet_r50-d8.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/models/pointrend_r50.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/models/psanet_r50-d8.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/models/pspnet_r50-d8.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/models/upernet_r50.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/models/upernet_uniformer.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/schedules/schedule_160k.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/schedules/schedule_20k.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/schedules/schedule_40k.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/configs/_base_/schedules/schedule_80k.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/exp/upernet_global_small/config.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/exp/upernet_global_small/test_config_g.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/exp/upernet_global_small/test_config_h32.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/exp/upernet_global_small/test_config_w32.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/version.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/arraymisc/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/arraymisc/quantization.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/cnn/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/cnn/alexnet.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/cnn/builder.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/cnn/resnet.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/cnn/vgg.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/activation.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/context_block.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/conv.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/conv_module.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/conv_ws.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/drop.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/generalized_attention.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/hsigmoid.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/hswish.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/non_local.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/norm.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/padding.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/plugin.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/registry.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/scale.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/swish.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/transformer.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/upsample.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/cnn/bricks/wrappers.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/cnn/utils/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/cnn/utils/flops_counter.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/cnn/utils/fuse_conv_bn.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/cnn/utils/sync_bn.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/cnn/utils/weight_init.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/engine/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/engine/test.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/fileio/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/fileio/file_client.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/fileio/io.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/fileio/parse.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/fileio/handlers/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/fileio/handlers/base.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/fileio/handlers/json_handler.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/fileio/handlers/pickle_handler.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/fileio/handlers/yaml_handler.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/image/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/image/colorspace.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/image/geometric.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/image/io.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/image/misc.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/image/photometric.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/assign_score_withk.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/ball_query.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/bbox.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/border_align.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/box_iou_rotated.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/carafe.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/cc_attention.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/contour_expand.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/corner_pool.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/correlation.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/deform_conv.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/deform_roi_pool.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/deprecated_wrappers.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/focal_loss.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/furthest_point_sample.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/fused_bias_leakyrelu.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/gather_points.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/group_points.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/info.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/iou3d.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/knn.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/masked_conv.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/merge_cells.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/modulated_deform_conv.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/multi_scale_deform_attn.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/nms.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/pixel_group.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/point_sample.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/points_in_boxes.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/points_sampler.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/psa_mask.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/roi_align.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/roi_align_rotated.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/roi_pool.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/roiaware_pool3d.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/roipoint_pool3d.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/saconv.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/scatter_points.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/sync_bn.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/three_interpolate.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/three_nn.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/tin_shift.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/upfirdn2d.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/ops/voxelize.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/parallel/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/parallel/_functions.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/parallel/collate.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/parallel/data_container.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/parallel/data_parallel.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/parallel/distributed.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/parallel/distributed_deprecated.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/parallel/registry.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/parallel/scatter_gather.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/parallel/utils.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/base_module.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/base_runner.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/builder.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/checkpoint.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/default_constructor.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/dist_utils.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/epoch_based_runner.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/fp16_utils.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/iter_based_runner.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/log_buffer.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/priority.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/utils.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/checkpoint.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/closure.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/ema.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/evaluation.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/hook.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/iter_timer.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/lr_updater.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/memory.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/momentum_updater.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/optimizer.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/profiler.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/sampler_seed.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/sync_buffer.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/logger/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/logger/base.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/logger/dvclive.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/logger/mlflow.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/logger/neptune.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/logger/pavi.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/logger/tensorboard.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/logger/text.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/hooks/logger/wandb.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/optimizer/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/optimizer/builder.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/runner/optimizer/default_constructor.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/utils/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/utils/config.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/utils/env.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/utils/ext_loader.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/utils/logging.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/utils/misc.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/utils/parrots_jit.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/utils/parrots_wrapper.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/utils/path.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/utils/progressbar.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/utils/registry.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/utils/testing.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/utils/timer.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/utils/trace.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/utils/version_utils.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/video/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/video/io.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/video/optflow.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/video/processing.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/visualization/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/visualization/color.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/visualization/image.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv/visualization/optflow.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv_custom/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmcv_custom/checkpoint.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/apis/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/apis/inference.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/apis/test.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/apis/train.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/core/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/core/evaluation/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/core/evaluation/class_names.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/core/evaluation/eval_hooks.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/core/evaluation/metrics.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/core/seg/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/core/seg/builder.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/core/seg/sampler/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/core/seg/sampler/base_pixel_sampler.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/core/utils/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/core/utils/misc.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/datasets/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/datasets/ade.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/datasets/builder.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/datasets/chase_db1.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/datasets/cityscapes.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/datasets/custom.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/datasets/dataset_wrappers.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/datasets/drive.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/datasets/hrf.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/datasets/pascal_context.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/datasets/stare.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/datasets/voc.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/datasets/pipelines/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/datasets/pipelines/compose.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/datasets/pipelines/formating.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/datasets/pipelines/loading.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/datasets/pipelines/test_time_aug.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/datasets/pipelines/transforms.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/builder.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/backbones/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/backbones/cgnet.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/backbones/fast_scnn.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/backbones/hrnet.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/backbones/mobilenet_v2.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/backbones/mobilenet_v3.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/backbones/resnest.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/backbones/resnet.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/backbones/resnext.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/backbones/unet.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/backbones/uniformer.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/backbones/vit.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/ann_head.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/apc_head.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/aspp_head.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/cascade_decode_head.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/cc_head.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/da_head.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/decode_head.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/dm_head.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/dnl_head.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/ema_head.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/enc_head.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/fcn_head.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/fpn_head.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/gc_head.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/lraspp_head.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/nl_head.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/ocr_head.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/point_head.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/psa_head.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/psp_head.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/sep_aspp_head.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/sep_fcn_head.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/decode_heads/uper_head.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/losses/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/losses/accuracy.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/losses/cross_entropy_loss.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/losses/dice_loss.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/losses/lovasz_loss.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/losses/utils.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/necks/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/necks/fpn.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/necks/multilevel_neck.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/segmentors/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/segmentors/base.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/segmentors/encoder_decoder.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/utils/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/utils/drop.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/utils/inverted_residual.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/utils/make_divisible.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/utils/res_layer.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/utils/se_layer.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/utils/self_attention_block.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/utils/up_conv_block.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/models/utils/weight_init.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/ops/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/ops/encoding.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/ops/wrappers.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/utils/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/utils/collect_env.py
+Comment: 
+
+Filename: build/lib/lavis/common/annotator/uniformer/mmseg/utils/logger.py
+Comment: 
+
+Filename: build/lib/lavis/common/vqa_tools/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/common/vqa_tools/vqa.py
+Comment: 
+
+Filename: build/lib/lavis/common/vqa_tools/vqa_eval.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/data_utils.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/builders/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/builders/audio_caption_builder.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/builders/audio_qa_builder.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/builders/base_dataset_builder.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/builders/caption_builder.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/builders/classification_builder.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/builders/dialogue_builder.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/builders/discrn_builders.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/builders/image_text_pair_builder.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/builders/imagefolder_builder.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/builders/object3d_caption_builder.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/builders/object3d_classification_builder.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/builders/object3d_qa_builder.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/builders/retrieval_builder.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/builders/text_to_image_generation_builder.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/builders/video_qa_builder.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/builders/vqa_builder.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/aok_vqa_datasets.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/audio_captioning_datasets.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/audio_classification_datasets.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/audio_qa_datasets.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/avsd_dialogue_datasets.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/base_dataset.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/capfilt_dataset.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/caption_datasets.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/coco_caption_datasets.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/coco_vqa_datasets.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/dataloader_utils.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/dialogue_datasets.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/discriminatory_reasoning_datasets.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/gqa_datasets.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/iconqa_datasets.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/image_text_pair_datasets.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/imagefolder_dataset.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/laion_dataset.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/llava150k_dataset.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/multimodal_classification_datasets.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/music_avqa.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/nlvr_datasets.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/object3d_captioning_datasets.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/object3d_classification_datasets.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/object3d_qa_datasets.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/ocr_datasets.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/retrieval_datasets.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/snli_ve_datasets.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/subject_driven_t2i_dataset.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/textcaps_datasets.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/valor_caption.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/vatex_captioning_datasets.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/vg_vqa_datasets.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/video_caption_datasets.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/video_vqa_datasets.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/violin_dataset.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/visdial_dialogue_datasets.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/vizwiz_vqa_datasets.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/vlep_dataset.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/vqa_datasets.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/vsr_datasets.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/datasets/yt8m_video_dialogue_datasets.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/download_scripts/download_charade.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/download_scripts/download_coco.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/download_scripts/download_coin.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/download_scripts/download_didemo.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/download_scripts/download_flickr.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/download_scripts/download_gqa.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/download_scripts/download_iconqa.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/download_scripts/download_msrvtt.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/download_scripts/download_msvd.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/download_scripts/download_nocaps.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/download_scripts/download_sbu.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/download_scripts/download_vg.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/download_scripts/download_violin.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/download_scripts/DownloadConceptualCaptions/download_data_cc12m.py
+Comment: 
+
+Filename: build/lib/lavis/datasets/download_scripts/DownloadConceptualCaptions/download_data_cc3m.py
+Comment: 
+
+Filename: build/lib/lavis/models/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/models/base_model.py
+Comment: 
+
+Filename: build/lib/lavis/models/beats_encoder.py
+Comment: 
+
+Filename: build/lib/lavis/models/clip_vit.py
+Comment: 
+
+Filename: build/lib/lavis/models/eva_vit.py
+Comment: 
+
+Filename: build/lib/lavis/models/med.py
+Comment: 
+
+Filename: build/lib/lavis/models/vit.py
+Comment: 
+
+Filename: build/lib/lavis/models/albef_models/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/models/albef_models/albef_classification.py
+Comment: 
+
+Filename: build/lib/lavis/models/albef_models/albef_feature_extractor.py
+Comment: 
+
+Filename: build/lib/lavis/models/albef_models/albef_nlvr.py
+Comment: 
+
+Filename: build/lib/lavis/models/albef_models/albef_outputs.py
+Comment: 
+
+Filename: build/lib/lavis/models/albef_models/albef_pretrain.py
+Comment: 
+
+Filename: build/lib/lavis/models/albef_models/albef_retrieval.py
+Comment: 
+
+Filename: build/lib/lavis/models/albef_models/albef_vqa.py
+Comment: 
+
+Filename: build/lib/lavis/models/alpro_models/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/models/alpro_models/alpro_outputs.py
+Comment: 
+
+Filename: build/lib/lavis/models/alpro_models/alpro_qa.py
+Comment: 
+
+Filename: build/lib/lavis/models/alpro_models/alpro_retrieval.py
+Comment: 
+
+Filename: build/lib/lavis/models/beats/BEATs.py
+Comment: 
+
+Filename: build/lib/lavis/models/beats/Tokenizers.py
+Comment: 
+
+Filename: build/lib/lavis/models/beats/backbone.py
+Comment: 
+
+Filename: build/lib/lavis/models/beats/modules.py
+Comment: 
+
+Filename: build/lib/lavis/models/beats/quantizer.py
+Comment: 
+
+Filename: build/lib/lavis/models/blip2_models/Qformer.py
+Comment: 
+
+Filename: build/lib/lavis/models/blip2_models/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/models/blip2_models/blip2.py
+Comment: 
+
+Filename: build/lib/lavis/models/blip2_models/blip2_image_text_matching.py
+Comment: 
+
+Filename: build/lib/lavis/models/blip2_models/blip2_opt.py
+Comment: 
+
+Filename: build/lib/lavis/models/blip2_models/blip2_qformer.py
+Comment: 
+
+Filename: build/lib/lavis/models/blip2_models/blip2_t5.py
+Comment: 
+
+Filename: build/lib/lavis/models/blip2_models/blip2_t5_instruct.py
+Comment: 
+
+Filename: build/lib/lavis/models/blip2_models/blip2_vicuna_instruct.py
+Comment: 
+
+Filename: build/lib/lavis/models/blip2_models/blip2_vicuna_xinstruct.py
+Comment: 
+
+Filename: build/lib/lavis/models/blip2_models/modeling_llama.py
+Comment: 
+
+Filename: build/lib/lavis/models/blip2_models/modeling_opt.py
+Comment: 
+
+Filename: build/lib/lavis/models/blip2_models/modeling_t5.py
+Comment: 
+
+Filename: build/lib/lavis/models/blip_diffusion_models/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/models/blip_diffusion_models/blip_diffusion.py
+Comment: 
+
+Filename: build/lib/lavis/models/blip_diffusion_models/modeling_ctx_clip.py
+Comment: 
+
+Filename: build/lib/lavis/models/blip_diffusion_models/ptp_utils.py
+Comment: 
+
+Filename: build/lib/lavis/models/blip_diffusion_models/utils.py
+Comment: 
+
+Filename: build/lib/lavis/models/blip_models/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/models/blip_models/blip.py
+Comment: 
+
+Filename: build/lib/lavis/models/blip_models/blip_caption.py
+Comment: 
+
+Filename: build/lib/lavis/models/blip_models/blip_classification.py
+Comment: 
+
+Filename: build/lib/lavis/models/blip_models/blip_feature_extractor.py
+Comment: 
+
+Filename: build/lib/lavis/models/blip_models/blip_image_text_matching.py
+Comment: 
+
+Filename: build/lib/lavis/models/blip_models/blip_nlvr.py
+Comment: 
+
+Filename: build/lib/lavis/models/blip_models/blip_outputs.py
+Comment: 
+
+Filename: build/lib/lavis/models/blip_models/blip_pretrain.py
+Comment: 
+
+Filename: build/lib/lavis/models/blip_models/blip_retrieval.py
+Comment: 
+
+Filename: build/lib/lavis/models/blip_models/blip_vqa.py
+Comment: 
+
+Filename: build/lib/lavis/models/blip_models/nlvr_encoder.py
+Comment: 
+
+Filename: build/lib/lavis/models/clip_models/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/models/clip_models/clip_outputs.py
+Comment: 
+
+Filename: build/lib/lavis/models/clip_models/loss.py
+Comment: 
+
+Filename: build/lib/lavis/models/clip_models/model.py
+Comment: 
+
+Filename: build/lib/lavis/models/clip_models/pretrained.py
+Comment: 
+
+Filename: build/lib/lavis/models/clip_models/timm_model.py
+Comment: 
+
+Filename: build/lib/lavis/models/clip_models/tokenizer.py
+Comment: 
+
+Filename: build/lib/lavis/models/clip_models/transform.py
+Comment: 
+
+Filename: build/lib/lavis/models/clip_models/utils.py
+Comment: 
+
+Filename: build/lib/lavis/models/gpt_models/gpt_dialogue.py
+Comment: 
+
+Filename: build/lib/lavis/models/img2prompt_models/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/models/img2prompt_models/img2prompt_vqa.py
+Comment: 
+
+Filename: build/lib/lavis/models/pnp_vqa_models/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/models/pnp_vqa_models/pnp_unifiedqav2_fid.py
+Comment: 
+
+Filename: build/lib/lavis/models/pnp_vqa_models/pnp_vqa.py
+Comment: 
+
+Filename: build/lib/lavis/models/timesformer/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/models/timesformer/conv2d_same.py
+Comment: 
+
+Filename: build/lib/lavis/models/timesformer/features.py
+Comment: 
+
+Filename: build/lib/lavis/models/timesformer/helpers.py
+Comment: 
+
+Filename: build/lib/lavis/models/timesformer/linear.py
+Comment: 
+
+Filename: build/lib/lavis/models/timesformer/vit.py
+Comment: 
+
+Filename: build/lib/lavis/models/timesformer/vit_utils.py
+Comment: 
+
+Filename: build/lib/lavis/models/ulip_models/ULIP_models.py
+Comment: 
+
+Filename: build/lib/lavis/models/ulip_models/losses.py
+Comment: 
+
+Filename: build/lib/lavis/models/ulip_models/pointbert/checkpoint.py
+Comment: 
+
+Filename: build/lib/lavis/models/ulip_models/pointbert/dvae.py
+Comment: 
+
+Filename: build/lib/lavis/models/ulip_models/pointbert/logger.py
+Comment: 
+
+Filename: build/lib/lavis/models/ulip_models/pointbert/misc.py
+Comment: 
+
+Filename: build/lib/lavis/models/ulip_models/pointbert/point_encoder.py
+Comment: 
+
+Filename: build/lib/lavis/models/ulip_models/utils/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/models/ulip_models/utils/build.py
+Comment: 
+
+Filename: build/lib/lavis/models/ulip_models/utils/config.py
+Comment: 
+
+Filename: build/lib/lavis/models/ulip_models/utils/io.py
+Comment: 
+
+Filename: build/lib/lavis/models/ulip_models/utils/logger.py
+Comment: 
+
+Filename: build/lib/lavis/models/ulip_models/utils/registry.py
+Comment: 
+
+Filename: build/lib/lavis/models/ulip_models/utils/tokenizer.py
+Comment: 
+
+Filename: build/lib/lavis/models/ulip_models/utils/utils.py
+Comment: 
+
+Filename: build/lib/lavis/processors/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/processors/alpro_processors.py
+Comment: 
+
+Filename: build/lib/lavis/processors/audio_processors.py
+Comment: 
+
+Filename: build/lib/lavis/processors/base_processor.py
+Comment: 
+
+Filename: build/lib/lavis/processors/blip_diffusion_processors.py
+Comment: 
+
+Filename: build/lib/lavis/processors/blip_processors.py
+Comment: 
+
+Filename: build/lib/lavis/processors/clip_processors.py
+Comment: 
+
+Filename: build/lib/lavis/processors/functional_video.py
+Comment: 
+
+Filename: build/lib/lavis/processors/gpt_processors.py
+Comment: 
+
+Filename: build/lib/lavis/processors/instruction_text_processors.py
+Comment: 
+
+Filename: build/lib/lavis/processors/randaugment.py
+Comment: 
+
+Filename: build/lib/lavis/processors/transforms_video.py
+Comment: 
+
+Filename: build/lib/lavis/processors/ulip_processors.py
+Comment: 
+
+Filename: build/lib/lavis/runners/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/runners/runner_base.py
+Comment: 
+
+Filename: build/lib/lavis/runners/runner_iter.py
+Comment: 
+
+Filename: build/lib/lavis/tasks/__init__.py
+Comment: 
+
+Filename: build/lib/lavis/tasks/base_task.py
+Comment: 
+
+Filename: build/lib/lavis/tasks/captioning.py
+Comment: 
+
+Filename: build/lib/lavis/tasks/dialogue.py
+Comment: 
+
+Filename: build/lib/lavis/tasks/image_text_pretrain.py
+Comment: 
+
+Filename: build/lib/lavis/tasks/multimodal_classification.py
+Comment: 
+
+Filename: build/lib/lavis/tasks/retrieval.py
+Comment: 
+
+Filename: build/lib/lavis/tasks/text_to_image_generation.py
+Comment: 
+
+Filename: build/lib/lavis/tasks/vqa.py
+Comment: 
+
+Filename: build/lib/lavis/tasks/vqa_reading_comprehension.py
+Comment: 
+
+Filename: build/lib/projects/img2llm-vqa/img2llm_vqa.py
+Comment: 
+
+Filename: build/lib/projects/instructblip/run_demo.py
+Comment: 
+
+Filename: build/lib/projects/xinstructblip/data_aug/3d_qa_data_generation.py
+Comment: 
+
+Filename: build/lib/projects/xinstructblip/data_aug/audio_qa_data_generation.py
+Comment: 
+
+Filename: build/lib/projects/xinstructblip/demo/run_demo.py
+Comment: 
+
+Filename: build/lib/projects/xinstructblip/discrn/caption_baseline/predict_audio.py
+Comment: 
+
+Filename: build/lib/projects/xinstructblip/discrn/caption_baseline/predict_image.py
+Comment: 
+
+Filename: build/lib/projects/xinstructblip/discrn/caption_baseline/predict_pc.py
+Comment: 
+
+Filename: build/lib/projects/xinstructblip/discrn/caption_baseline/predict_video.py
+Comment: 
+
+Filename: build/lib/projects/xinstructblip/discrn/caption_baseline/render_images.py
+Comment: 
+
+Filename: build/lib/projects/xinstructblip/discrn/data_generation/audiocaps_video_audio.py
+Comment: 
+
+Filename: build/lib/projects/xinstructblip/discrn/data_generation/objaverse_img_3d.py
+Comment: 
+
+Filename: build/lib/projects/xinstructblip/modelnet_baseline/render_images.py
+Comment: 
+
+Filename: build/lib/tests/models/test_albef.py
+Comment: 
+
+Filename: build/lib/tests/models/test_blip.py
+Comment: 
+
+Filename: build/lib/tests/models/test_blip2.py
+Comment: 
+
+Filename: build/lib/tests/models/test_pnp_vqa.py
+Comment: 
+
 Filename: docs/conf.py
 Comment: 
 
 Filename: lavis/__init__.py
 Comment: 
 
 Filename: lavis/common/config.py
@@ -57,14 +1791,1049 @@
 
 Filename: lavis/common/registry.py
 Comment: 
 
 Filename: lavis/common/utils.py
 Comment: 
 
+Filename: lavis/common/annotator/util.py
+Comment: 
+
+Filename: lavis/common/annotator/canny/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/hed/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/midas/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/midas/api.py
+Comment: 
+
+Filename: lavis/common/annotator/midas/utils.py
+Comment: 
+
+Filename: lavis/common/annotator/midas/midas/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/midas/midas/base_model.py
+Comment: 
+
+Filename: lavis/common/annotator/midas/midas/blocks.py
+Comment: 
+
+Filename: lavis/common/annotator/midas/midas/dpt_depth.py
+Comment: 
+
+Filename: lavis/common/annotator/midas/midas/midas_net.py
+Comment: 
+
+Filename: lavis/common/annotator/midas/midas/midas_net_custom.py
+Comment: 
+
+Filename: lavis/common/annotator/midas/midas/transforms.py
+Comment: 
+
+Filename: lavis/common/annotator/midas/midas/vit.py
+Comment: 
+
+Filename: lavis/common/annotator/mlsd/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/mlsd/utils.py
+Comment: 
+
+Filename: lavis/common/annotator/mlsd/models/mbv2_mlsd_large.py
+Comment: 
+
+Filename: lavis/common/annotator/mlsd/models/mbv2_mlsd_tiny.py
+Comment: 
+
+Filename: lavis/common/annotator/openpose/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/openpose/body.py
+Comment: 
+
+Filename: lavis/common/annotator/openpose/hand.py
+Comment: 
+
+Filename: lavis/common/annotator/openpose/model.py
+Comment: 
+
+Filename: lavis/common/annotator/openpose/util.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/default_runtime.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/datasets/ade20k.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/datasets/chase_db1.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/datasets/cityscapes.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/datasets/cityscapes_769x769.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/datasets/drive.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/datasets/hrf.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/datasets/pascal_context.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/datasets/pascal_context_59.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/datasets/pascal_voc12.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/datasets/pascal_voc12_aug.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/datasets/stare.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/models/ann_r50-d8.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/models/apcnet_r50-d8.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/models/ccnet_r50-d8.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/models/cgnet.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/models/danet_r50-d8.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/models/deeplabv3_r50-d8.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/models/dmnet_r50-d8.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/models/dnl_r50-d8.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/models/emanet_r50-d8.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/models/encnet_r50-d8.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/models/fast_scnn.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/models/fcn_hr18.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/models/fcn_r50-d8.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/models/fcn_unet_s5-d16.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/models/fpn_r50.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/models/fpn_uniformer.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/models/gcnet_r50-d8.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/models/lraspp_m-v3-d8.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/models/nonlocal_r50-d8.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/models/ocrnet_hr18.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/models/ocrnet_r50-d8.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/models/pointrend_r50.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/models/psanet_r50-d8.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/models/pspnet_r50-d8.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/models/upernet_r50.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/models/upernet_uniformer.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/schedules/schedule_160k.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/schedules/schedule_20k.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/schedules/schedule_40k.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/configs/_base_/schedules/schedule_80k.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/exp/upernet_global_small/config.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/exp/upernet_global_small/test_config_g.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/exp/upernet_global_small/test_config_h32.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/exp/upernet_global_small/test_config_w32.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/version.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/arraymisc/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/arraymisc/quantization.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/cnn/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/cnn/alexnet.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/cnn/builder.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/cnn/resnet.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/cnn/vgg.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/cnn/bricks/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/cnn/bricks/activation.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/cnn/bricks/context_block.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/cnn/bricks/conv.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/cnn/bricks/conv_module.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/cnn/bricks/conv_ws.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/cnn/bricks/drop.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/cnn/bricks/generalized_attention.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/cnn/bricks/hsigmoid.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/cnn/bricks/hswish.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/cnn/bricks/non_local.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/cnn/bricks/norm.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/cnn/bricks/padding.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/cnn/bricks/plugin.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/cnn/bricks/registry.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/cnn/bricks/scale.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/cnn/bricks/swish.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/cnn/bricks/transformer.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/cnn/bricks/upsample.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/cnn/bricks/wrappers.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/cnn/utils/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/cnn/utils/flops_counter.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/cnn/utils/fuse_conv_bn.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/cnn/utils/sync_bn.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/cnn/utils/weight_init.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/engine/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/engine/test.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/fileio/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/fileio/file_client.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/fileio/io.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/fileio/parse.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/fileio/handlers/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/fileio/handlers/base.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/fileio/handlers/json_handler.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/fileio/handlers/pickle_handler.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/fileio/handlers/yaml_handler.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/image/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/image/colorspace.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/image/geometric.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/image/io.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/image/misc.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/image/photometric.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/assign_score_withk.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/ball_query.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/bbox.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/border_align.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/box_iou_rotated.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/carafe.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/cc_attention.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/contour_expand.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/corner_pool.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/correlation.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/deform_conv.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/deform_roi_pool.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/deprecated_wrappers.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/focal_loss.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/furthest_point_sample.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/fused_bias_leakyrelu.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/gather_points.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/group_points.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/info.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/iou3d.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/knn.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/masked_conv.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/merge_cells.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/modulated_deform_conv.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/multi_scale_deform_attn.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/nms.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/pixel_group.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/point_sample.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/points_in_boxes.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/points_sampler.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/psa_mask.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/roi_align.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/roi_align_rotated.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/roi_pool.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/roiaware_pool3d.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/roipoint_pool3d.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/saconv.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/scatter_points.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/sync_bn.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/three_interpolate.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/three_nn.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/tin_shift.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/upfirdn2d.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/ops/voxelize.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/parallel/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/parallel/_functions.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/parallel/collate.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/parallel/data_container.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/parallel/data_parallel.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/parallel/distributed.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/parallel/distributed_deprecated.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/parallel/registry.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/parallel/scatter_gather.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/parallel/utils.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/base_module.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/base_runner.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/builder.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/checkpoint.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/default_constructor.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/dist_utils.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/epoch_based_runner.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/fp16_utils.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/iter_based_runner.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/log_buffer.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/priority.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/utils.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/hooks/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/hooks/checkpoint.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/hooks/closure.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/hooks/ema.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/hooks/evaluation.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/hooks/hook.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/hooks/iter_timer.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/hooks/lr_updater.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/hooks/memory.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/hooks/momentum_updater.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/hooks/optimizer.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/hooks/profiler.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/hooks/sampler_seed.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/hooks/sync_buffer.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/hooks/logger/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/hooks/logger/base.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/hooks/logger/dvclive.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/hooks/logger/mlflow.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/hooks/logger/neptune.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/hooks/logger/pavi.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/hooks/logger/tensorboard.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/hooks/logger/text.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/hooks/logger/wandb.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/optimizer/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/optimizer/builder.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/runner/optimizer/default_constructor.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/utils/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/utils/config.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/utils/env.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/utils/ext_loader.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/utils/logging.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/utils/misc.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/utils/parrots_jit.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/utils/parrots_wrapper.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/utils/path.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/utils/progressbar.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/utils/registry.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/utils/testing.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/utils/timer.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/utils/trace.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/utils/version_utils.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/video/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/video/io.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/video/optflow.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/video/processing.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/visualization/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/visualization/color.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/visualization/image.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv/visualization/optflow.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv_custom/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmcv_custom/checkpoint.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/apis/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/apis/inference.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/apis/test.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/apis/train.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/core/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/core/evaluation/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/core/evaluation/class_names.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/core/evaluation/eval_hooks.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/core/evaluation/metrics.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/core/seg/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/core/seg/builder.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/core/seg/sampler/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/core/seg/sampler/base_pixel_sampler.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/core/utils/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/core/utils/misc.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/datasets/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/datasets/ade.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/datasets/builder.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/datasets/chase_db1.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/datasets/cityscapes.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/datasets/custom.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/datasets/dataset_wrappers.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/datasets/drive.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/datasets/hrf.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/datasets/pascal_context.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/datasets/stare.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/datasets/voc.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/datasets/pipelines/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/datasets/pipelines/compose.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/datasets/pipelines/formating.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/datasets/pipelines/loading.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/datasets/pipelines/test_time_aug.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/datasets/pipelines/transforms.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/builder.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/backbones/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/backbones/cgnet.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/backbones/fast_scnn.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/backbones/hrnet.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/backbones/mobilenet_v2.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/backbones/mobilenet_v3.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/backbones/resnest.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/backbones/resnet.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/backbones/resnext.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/backbones/unet.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/backbones/uniformer.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/backbones/vit.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/decode_heads/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/decode_heads/ann_head.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/decode_heads/apc_head.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/decode_heads/aspp_head.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/decode_heads/cascade_decode_head.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/decode_heads/cc_head.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/decode_heads/da_head.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/decode_heads/decode_head.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/decode_heads/dm_head.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/decode_heads/dnl_head.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/decode_heads/ema_head.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/decode_heads/enc_head.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/decode_heads/fcn_head.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/decode_heads/fpn_head.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/decode_heads/gc_head.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/decode_heads/lraspp_head.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/decode_heads/nl_head.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/decode_heads/ocr_head.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/decode_heads/point_head.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/decode_heads/psa_head.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/decode_heads/psp_head.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/decode_heads/sep_aspp_head.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/decode_heads/sep_fcn_head.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/decode_heads/uper_head.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/losses/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/losses/accuracy.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/losses/cross_entropy_loss.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/losses/dice_loss.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/losses/lovasz_loss.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/losses/utils.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/necks/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/necks/fpn.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/necks/multilevel_neck.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/segmentors/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/segmentors/base.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/segmentors/encoder_decoder.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/utils/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/utils/drop.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/utils/inverted_residual.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/utils/make_divisible.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/utils/res_layer.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/utils/se_layer.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/utils/self_attention_block.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/utils/up_conv_block.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/models/utils/weight_init.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/ops/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/ops/encoding.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/ops/wrappers.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/utils/__init__.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/utils/collect_env.py
+Comment: 
+
+Filename: lavis/common/annotator/uniformer/mmseg/utils/logger.py
+Comment: 
+
 Filename: lavis/common/vqa_tools/__init__.py
 Comment: 
 
 Filename: lavis/common/vqa_tools/vqa.py
 Comment: 
 
 Filename: lavis/common/vqa_tools/vqa_eval.py
@@ -72,95 +2841,341 @@
 
 Filename: lavis/configs/default.yaml
 Comment: 
 
 Filename: lavis/configs/datasets/aokvqa/defaults.yaml
 Comment: 
 
+Filename: lavis/configs/datasets/aokvqa/defaults_instruct.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/audiocaps/defaults_mm_cap.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/audiocaps/defaults_mm_cap_instruct.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/audiocaps/defaults_mm_qa.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/audioset/defaults_mm_cap.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/audioset/defaults_mm_cap_instruct.yaml
+Comment: 
+
 Filename: lavis/configs/datasets/avsd/defaults_dial.yaml
 Comment: 
 
+Filename: lavis/configs/datasets/avsd/defaults_mm_dial_instruct.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/blip_diffusion_datasets/defaults.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/capfilt14m/defaults_cap.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/capfilt14m/defaults_cap_instruct.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/charade/defaults_cap.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/charade/defaults_cap_instruct.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/clotho/defaults_mm_cap.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/clotho/defaults_mm_cap_instruct.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/clotho/defaults_mm_qa.yaml
+Comment: 
+
 Filename: lavis/configs/datasets/coco/defaults_cap.yaml
 Comment: 
 
+Filename: lavis/configs/datasets/coco/defaults_cap_instruct.yaml
+Comment: 
+
 Filename: lavis/configs/datasets/coco/defaults_ret.yaml
 Comment: 
 
 Filename: lavis/configs/datasets/coco/defaults_vqa.yaml
 Comment: 
 
+Filename: lavis/configs/datasets/coco/defaults_vqa_instruct.yaml
+Comment: 
+
 Filename: lavis/configs/datasets/coco/eval_vqa.yaml
 Comment: 
 
+Filename: lavis/configs/datasets/coin/defaults_cap.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/coin/defaults_cap_instruct.yaml
+Comment: 
+
 Filename: lavis/configs/datasets/conceptual_caption/defaults_12m.yaml
 Comment: 
 
+Filename: lavis/configs/datasets/conceptual_caption/defaults_12m_instruct.yaml
+Comment: 
+
 Filename: lavis/configs/datasets/conceptual_caption/defaults_3m.yaml
 Comment: 
 
+Filename: lavis/configs/datasets/conceptual_caption/defaults_3m_instruct.yaml
+Comment: 
+
 Filename: lavis/configs/datasets/didemo/defaults_ret.yaml
 Comment: 
 
+Filename: lavis/configs/datasets/discriminatory_reasoning/defaults_mm_audio_video.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/discriminatory_reasoning/defaults_mm_image_pc.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/discriminatory_reasoning/discriminatory_dataset/audiocaps_discrn.json
+Comment: 
+
+Filename: lavis/configs/datasets/discriminatory_reasoning/discriminatory_dataset/objaverse_discrn.json
+Comment: 
+
+Filename: lavis/configs/datasets/esc50/defaults_mm_cls.yaml
+Comment: 
+
 Filename: lavis/configs/datasets/flickr30k/defaults.yaml
 Comment: 
 
+Filename: lavis/configs/datasets/flickr30k/defaults_cap.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/flickr30k/defaults_cap_instruct.yaml
+Comment: 
+
 Filename: lavis/configs/datasets/gqa/balanced_testdev.yaml
 Comment: 
 
+Filename: lavis/configs/datasets/gqa/balanced_testdev_instruct.yaml
+Comment: 
+
 Filename: lavis/configs/datasets/gqa/balanced_val.yaml
 Comment: 
 
+Filename: lavis/configs/datasets/gqa/balanced_val_instruct.yaml
+Comment: 
+
 Filename: lavis/configs/datasets/gqa/defaults.yaml
 Comment: 
 
+Filename: lavis/configs/datasets/gqa/defaults_instruct.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/iconqa/defaults.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/iconqa/defaults_instruct.yaml
+Comment: 
+
 Filename: lavis/configs/datasets/imagenet/defaults.yaml
 Comment: 
 
 Filename: lavis/configs/datasets/laion/defaults_2B_multi.yaml
 Comment: 
 
+Filename: lavis/configs/datasets/laion/defaults_400M.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/laion/defaults_400M_instruct.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/llava150k/defaults_dial.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/modelnet40/defaults_cls.yaml
+Comment: 
+
 Filename: lavis/configs/datasets/msrvtt/defaults_cap.yaml
 Comment: 
 
+Filename: lavis/configs/datasets/msrvtt/defaults_cap_instruct.yaml
+Comment: 
+
 Filename: lavis/configs/datasets/msrvtt/defaults_qa.yaml
 Comment: 
 
+Filename: lavis/configs/datasets/msrvtt/defaults_qa_instruct.yaml
+Comment: 
+
 Filename: lavis/configs/datasets/msrvtt/defaults_ret.yaml
 Comment: 
 
 Filename: lavis/configs/datasets/msvd/defaults_cap.yaml
 Comment: 
 
+Filename: lavis/configs/datasets/msvd/defaults_cap_instruct.yaml
+Comment: 
+
 Filename: lavis/configs/datasets/msvd/defaults_qa.yaml
 Comment: 
 
+Filename: lavis/configs/datasets/msvd/defaults_qa_instruct.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/music_avqa/defaults_mm_qa.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/music_avqa/defaults_mm_qa_instruct.yaml
+Comment: 
+
 Filename: lavis/configs/datasets/nlvr/defaults.yaml
 Comment: 
 
 Filename: lavis/configs/datasets/nocaps/defaults.yaml
 Comment: 
 
+Filename: lavis/configs/datasets/objaverse/defaults_mm_cap.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/objaverse/defaults_mm_cap_instruct.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/objaverse/defaults_mm_qa.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/ocrvqa/defaults.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/ocrvqa/defaults_instruct.yaml
+Comment: 
+
 Filename: lavis/configs/datasets/okvqa/defaults.yaml
 Comment: 
 
+Filename: lavis/configs/datasets/okvqa/defaults_instruct.yaml
+Comment: 
+
 Filename: lavis/configs/datasets/sbu_caption/defaults.yaml
 Comment: 
 
+Filename: lavis/configs/datasets/sbu_caption/defaults_instruct.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/scienceqa/defaults.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/scienceqa/defaults_instruct.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/shapenet/defaults_mm_cap.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/shapenet/defaults_mm_cap_instruct.yaml
+Comment: 
+
 Filename: lavis/configs/datasets/snli_ve/defaults.yaml
 Comment: 
 
+Filename: lavis/configs/datasets/snli_ve/defaults_instruct.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/textcaps/defaults.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/textcaps/defaults_instruct.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/valor/defaults_mm_cap.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/valor/defaults_mm_cap_instruct.yaml
+Comment: 
+
 Filename: lavis/configs/datasets/vatex/defaults_cap.yaml
 Comment: 
 
+Filename: lavis/configs/datasets/vatex/defaults_cap_instruct.yaml
+Comment: 
+
 Filename: lavis/configs/datasets/vg/defaults_caption.yaml
 Comment: 
 
+Filename: lavis/configs/datasets/vg/defaults_caption_instruct.yaml
+Comment: 
+
 Filename: lavis/configs/datasets/vg/defaults_vqa.yaml
 Comment: 
 
+Filename: lavis/configs/datasets/vg/defaults_vqa_instruct.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/violin/defaults_cap.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/violin/defaults_cap_instruct.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/violin/defaults_entail.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/violin/defaults_entail_instruct.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/visdial/defaults_dial.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/visdial/defaults_dial_instruct.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/vizwiz/defaults.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/vlep/defaults_cap.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/vlep/defaults_cap_instruct.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/vsr/defaults.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/vsr/defaults_classification.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/vsr/defaults_classification_instruct.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/vsr/defaults_instruct.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/wavcaps/defaults_mm_cap.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/wavcaps/defaults_mm_cap_instruct.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/webvid/defaults_cap.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/webvid/defaults_cap_instruct.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/youcook/defaults_cap.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/youcook/defaults_cap_instruct.yaml
+Comment: 
+
+Filename: lavis/configs/datasets/yt8m/defaults_mm_dial.yaml
+Comment: 
+
 Filename: lavis/configs/models/albef_classification_ve.yaml
 Comment: 
 
 Filename: lavis/configs/models/albef_feature_extractor.yaml
 Comment: 
 
 Filename: lavis/configs/models/albef_nlvr.yaml
@@ -261,47 +3276,80 @@
 
 Filename: lavis/configs/models/med_config_albef.json
 Comment: 
 
 Filename: lavis/configs/models/med_large_config.json
 Comment: 
 
+Filename: lavis/configs/models/blip-diffusion/blip_diffusion_base.yaml
+Comment: 
+
+Filename: lavis/configs/models/blip-diffusion/blip_diffusion_controlnet_canny.yaml
+Comment: 
+
+Filename: lavis/configs/models/blip-diffusion/blip_diffusion_controlnet_depth.yaml
+Comment: 
+
+Filename: lavis/configs/models/blip-diffusion/blip_diffusion_controlnet_hed.yaml
+Comment: 
+
 Filename: lavis/configs/models/blip2/blip2_caption_flant5xl.yaml
 Comment: 
 
 Filename: lavis/configs/models/blip2/blip2_caption_opt2.7b.yaml
 Comment: 
 
 Filename: lavis/configs/models/blip2/blip2_caption_opt6.7b.yaml
 Comment: 
 
 Filename: lavis/configs/models/blip2/blip2_coco.yaml
 Comment: 
 
+Filename: lavis/configs/models/blip2/blip2_instruct_flant5xl.yaml
+Comment: 
+
+Filename: lavis/configs/models/blip2/blip2_instruct_flant5xxl.yaml
+Comment: 
+
+Filename: lavis/configs/models/blip2/blip2_instruct_vicuna13b.yaml
+Comment: 
+
+Filename: lavis/configs/models/blip2/blip2_instruct_vicuna7b.yaml
+Comment: 
+
 Filename: lavis/configs/models/blip2/blip2_pretrain.yaml
 Comment: 
 
 Filename: lavis/configs/models/blip2/blip2_pretrain_flant5xl.yaml
 Comment: 
 
 Filename: lavis/configs/models/blip2/blip2_pretrain_flant5xl_vitL.yaml
 Comment: 
 
 Filename: lavis/configs/models/blip2/blip2_pretrain_flant5xxl.yaml
 Comment: 
 
+Filename: lavis/configs/models/blip2/blip2_pretrain_llama7b.yaml
+Comment: 
+
 Filename: lavis/configs/models/blip2/blip2_pretrain_opt2.7b.yaml
 Comment: 
 
 Filename: lavis/configs/models/blip2/blip2_pretrain_opt6.7b.yaml
 Comment: 
 
 Filename: lavis/configs/models/blip2/blip2_pretrain_vitL.yaml
 Comment: 
 
+Filename: lavis/configs/models/blip2/blip2_xinstruct_vicuna13b.yaml
+Comment: 
+
+Filename: lavis/configs/models/blip2/blip2_xinstruct_vicuna7b.yaml
+Comment: 
+
 Filename: lavis/configs/models/clip/RN101-quickgelu.json
 Comment: 
 
 Filename: lavis/configs/models/clip/RN101.json
 Comment: 
 
 Filename: lavis/configs/models/clip/RN50-quickgelu.json
@@ -405,50 +3453,83 @@
 
 Filename: lavis/datasets/data_utils.py
 Comment: 
 
 Filename: lavis/datasets/builders/__init__.py
 Comment: 
 
+Filename: lavis/datasets/builders/audio_caption_builder.py
+Comment: 
+
+Filename: lavis/datasets/builders/audio_qa_builder.py
+Comment: 
+
 Filename: lavis/datasets/builders/base_dataset_builder.py
 Comment: 
 
 Filename: lavis/datasets/builders/caption_builder.py
 Comment: 
 
 Filename: lavis/datasets/builders/classification_builder.py
 Comment: 
 
 Filename: lavis/datasets/builders/dialogue_builder.py
 Comment: 
 
+Filename: lavis/datasets/builders/discrn_builders.py
+Comment: 
+
 Filename: lavis/datasets/builders/image_text_pair_builder.py
 Comment: 
 
 Filename: lavis/datasets/builders/imagefolder_builder.py
 Comment: 
 
+Filename: lavis/datasets/builders/object3d_caption_builder.py
+Comment: 
+
+Filename: lavis/datasets/builders/object3d_classification_builder.py
+Comment: 
+
+Filename: lavis/datasets/builders/object3d_qa_builder.py
+Comment: 
+
 Filename: lavis/datasets/builders/retrieval_builder.py
 Comment: 
 
+Filename: lavis/datasets/builders/text_to_image_generation_builder.py
+Comment: 
+
 Filename: lavis/datasets/builders/video_qa_builder.py
 Comment: 
 
 Filename: lavis/datasets/builders/vqa_builder.py
 Comment: 
 
 Filename: lavis/datasets/datasets/aok_vqa_datasets.py
 Comment: 
 
+Filename: lavis/datasets/datasets/audio_captioning_datasets.py
+Comment: 
+
+Filename: lavis/datasets/datasets/audio_classification_datasets.py
+Comment: 
+
+Filename: lavis/datasets/datasets/audio_qa_datasets.py
+Comment: 
+
 Filename: lavis/datasets/datasets/avsd_dialogue_datasets.py
 Comment: 
 
 Filename: lavis/datasets/datasets/base_dataset.py
 Comment: 
 
+Filename: lavis/datasets/datasets/capfilt_dataset.py
+Comment: 
+
 Filename: lavis/datasets/datasets/caption_datasets.py
 Comment: 
 
 Filename: lavis/datasets/datasets/coco_caption_datasets.py
 Comment: 
 
 Filename: lavis/datasets/datasets/coco_vqa_datasets.py
@@ -456,62 +3537,125 @@
 
 Filename: lavis/datasets/datasets/dataloader_utils.py
 Comment: 
 
 Filename: lavis/datasets/datasets/dialogue_datasets.py
 Comment: 
 
+Filename: lavis/datasets/datasets/discriminatory_reasoning_datasets.py
+Comment: 
+
 Filename: lavis/datasets/datasets/gqa_datasets.py
 Comment: 
 
+Filename: lavis/datasets/datasets/iconqa_datasets.py
+Comment: 
+
 Filename: lavis/datasets/datasets/image_text_pair_datasets.py
 Comment: 
 
 Filename: lavis/datasets/datasets/imagefolder_dataset.py
 Comment: 
 
 Filename: lavis/datasets/datasets/laion_dataset.py
 Comment: 
 
+Filename: lavis/datasets/datasets/llava150k_dataset.py
+Comment: 
+
 Filename: lavis/datasets/datasets/multimodal_classification_datasets.py
 Comment: 
 
+Filename: lavis/datasets/datasets/music_avqa.py
+Comment: 
+
 Filename: lavis/datasets/datasets/nlvr_datasets.py
 Comment: 
 
+Filename: lavis/datasets/datasets/object3d_captioning_datasets.py
+Comment: 
+
+Filename: lavis/datasets/datasets/object3d_classification_datasets.py
+Comment: 
+
+Filename: lavis/datasets/datasets/object3d_qa_datasets.py
+Comment: 
+
+Filename: lavis/datasets/datasets/ocr_datasets.py
+Comment: 
+
 Filename: lavis/datasets/datasets/retrieval_datasets.py
 Comment: 
 
 Filename: lavis/datasets/datasets/snli_ve_datasets.py
 Comment: 
 
+Filename: lavis/datasets/datasets/subject_driven_t2i_dataset.py
+Comment: 
+
+Filename: lavis/datasets/datasets/textcaps_datasets.py
+Comment: 
+
+Filename: lavis/datasets/datasets/valor_caption.py
+Comment: 
+
+Filename: lavis/datasets/datasets/vatex_captioning_datasets.py
+Comment: 
+
 Filename: lavis/datasets/datasets/vg_vqa_datasets.py
 Comment: 
 
 Filename: lavis/datasets/datasets/video_caption_datasets.py
 Comment: 
 
 Filename: lavis/datasets/datasets/video_vqa_datasets.py
 Comment: 
 
+Filename: lavis/datasets/datasets/violin_dataset.py
+Comment: 
+
+Filename: lavis/datasets/datasets/visdial_dialogue_datasets.py
+Comment: 
+
+Filename: lavis/datasets/datasets/vizwiz_vqa_datasets.py
+Comment: 
+
+Filename: lavis/datasets/datasets/vlep_dataset.py
+Comment: 
+
 Filename: lavis/datasets/datasets/vqa_datasets.py
 Comment: 
 
+Filename: lavis/datasets/datasets/vsr_datasets.py
+Comment: 
+
+Filename: lavis/datasets/datasets/yt8m_video_dialogue_datasets.py
+Comment: 
+
+Filename: lavis/datasets/download_scripts/download_charade.py
+Comment: 
+
 Filename: lavis/datasets/download_scripts/download_coco.py
 Comment: 
 
+Filename: lavis/datasets/download_scripts/download_coin.py
+Comment: 
+
 Filename: lavis/datasets/download_scripts/download_didemo.py
 Comment: 
 
 Filename: lavis/datasets/download_scripts/download_flickr.py
 Comment: 
 
 Filename: lavis/datasets/download_scripts/download_gqa.py
 Comment: 
 
+Filename: lavis/datasets/download_scripts/download_iconqa.py
+Comment: 
+
 Filename: lavis/datasets/download_scripts/download_msrvtt.py
 Comment: 
 
 Filename: lavis/datasets/download_scripts/download_msvd.py
 Comment: 
 
 Filename: lavis/datasets/download_scripts/download_nocaps.py
@@ -519,26 +3663,32 @@
 
 Filename: lavis/datasets/download_scripts/download_sbu.py
 Comment: 
 
 Filename: lavis/datasets/download_scripts/download_vg.py
 Comment: 
 
+Filename: lavis/datasets/download_scripts/download_violin.py
+Comment: 
+
 Filename: lavis/datasets/download_scripts/DownloadConceptualCaptions/download_data_cc12m.py
 Comment: 
 
 Filename: lavis/datasets/download_scripts/DownloadConceptualCaptions/download_data_cc3m.py
 Comment: 
 
 Filename: lavis/models/__init__.py
 Comment: 
 
 Filename: lavis/models/base_model.py
 Comment: 
 
+Filename: lavis/models/beats_encoder.py
+Comment: 
+
 Filename: lavis/models/clip_vit.py
 Comment: 
 
 Filename: lavis/models/eva_vit.py
 Comment: 
 
 Filename: lavis/models/med.py
@@ -579,14 +3729,29 @@
 
 Filename: lavis/models/alpro_models/alpro_qa.py
 Comment: 
 
 Filename: lavis/models/alpro_models/alpro_retrieval.py
 Comment: 
 
+Filename: lavis/models/beats/BEATs.py
+Comment: 
+
+Filename: lavis/models/beats/Tokenizers.py
+Comment: 
+
+Filename: lavis/models/beats/backbone.py
+Comment: 
+
+Filename: lavis/models/beats/modules.py
+Comment: 
+
+Filename: lavis/models/beats/quantizer.py
+Comment: 
+
 Filename: lavis/models/blip2_models/Qformer.py
 Comment: 
 
 Filename: lavis/models/blip2_models/__init__.py
 Comment: 
 
 Filename: lavis/models/blip2_models/blip2.py
@@ -600,20 +3765,47 @@
 
 Filename: lavis/models/blip2_models/blip2_qformer.py
 Comment: 
 
 Filename: lavis/models/blip2_models/blip2_t5.py
 Comment: 
 
+Filename: lavis/models/blip2_models/blip2_t5_instruct.py
+Comment: 
+
+Filename: lavis/models/blip2_models/blip2_vicuna_instruct.py
+Comment: 
+
+Filename: lavis/models/blip2_models/blip2_vicuna_xinstruct.py
+Comment: 
+
+Filename: lavis/models/blip2_models/modeling_llama.py
+Comment: 
+
 Filename: lavis/models/blip2_models/modeling_opt.py
 Comment: 
 
 Filename: lavis/models/blip2_models/modeling_t5.py
 Comment: 
 
+Filename: lavis/models/blip_diffusion_models/__init__.py
+Comment: 
+
+Filename: lavis/models/blip_diffusion_models/blip_diffusion.py
+Comment: 
+
+Filename: lavis/models/blip_diffusion_models/modeling_ctx_clip.py
+Comment: 
+
+Filename: lavis/models/blip_diffusion_models/ptp_utils.py
+Comment: 
+
+Filename: lavis/models/blip_diffusion_models/utils.py
+Comment: 
+
 Filename: lavis/models/blip_models/__init__.py
 Comment: 
 
 Filename: lavis/models/blip_models/blip.py
 Comment: 
 
 Filename: lavis/models/blip_models/blip_caption.py
@@ -711,41 +3903,98 @@
 
 Filename: lavis/models/timesformer/vit.py
 Comment: 
 
 Filename: lavis/models/timesformer/vit_utils.py
 Comment: 
 
+Filename: lavis/models/ulip_models/ULIP_models.py
+Comment: 
+
+Filename: lavis/models/ulip_models/losses.py
+Comment: 
+
+Filename: lavis/models/ulip_models/pointbert/checkpoint.py
+Comment: 
+
+Filename: lavis/models/ulip_models/pointbert/dvae.py
+Comment: 
+
+Filename: lavis/models/ulip_models/pointbert/logger.py
+Comment: 
+
+Filename: lavis/models/ulip_models/pointbert/misc.py
+Comment: 
+
+Filename: lavis/models/ulip_models/pointbert/point_encoder.py
+Comment: 
+
+Filename: lavis/models/ulip_models/utils/__init__.py
+Comment: 
+
+Filename: lavis/models/ulip_models/utils/build.py
+Comment: 
+
+Filename: lavis/models/ulip_models/utils/config.py
+Comment: 
+
+Filename: lavis/models/ulip_models/utils/io.py
+Comment: 
+
+Filename: lavis/models/ulip_models/utils/logger.py
+Comment: 
+
+Filename: lavis/models/ulip_models/utils/registry.py
+Comment: 
+
+Filename: lavis/models/ulip_models/utils/tokenizer.py
+Comment: 
+
+Filename: lavis/models/ulip_models/utils/utils.py
+Comment: 
+
 Filename: lavis/processors/__init__.py
 Comment: 
 
 Filename: lavis/processors/alpro_processors.py
 Comment: 
 
+Filename: lavis/processors/audio_processors.py
+Comment: 
+
 Filename: lavis/processors/base_processor.py
 Comment: 
 
+Filename: lavis/processors/blip_diffusion_processors.py
+Comment: 
+
 Filename: lavis/processors/blip_processors.py
 Comment: 
 
 Filename: lavis/processors/clip_processors.py
 Comment: 
 
 Filename: lavis/processors/functional_video.py
 Comment: 
 
 Filename: lavis/processors/gpt_processors.py
 Comment: 
 
+Filename: lavis/processors/instruction_text_processors.py
+Comment: 
+
 Filename: lavis/processors/randaugment.py
 Comment: 
 
 Filename: lavis/processors/transforms_video.py
 Comment: 
 
+Filename: lavis/processors/ulip_processors.py
+Comment: 
+
 Filename: lavis/projects/albef/eval/nlvr_eval.yaml
 Comment: 
 
 Filename: lavis/projects/albef/eval/ret_coco_eval.yaml
 Comment: 
 
 Filename: lavis/projects/albef/eval/ret_flickr30k_eval.yaml
@@ -870,14 +4119,20 @@
 
 Filename: lavis/projects/blip2/eval/caption_coco_opt2.7b_eval.yaml
 Comment: 
 
 Filename: lavis/projects/blip2/eval/caption_coco_opt6.7b_eval.yaml
 Comment: 
 
+Filename: lavis/projects/blip2/eval/caption_nocaps_out_domain_flant5xl_eval.yaml
+Comment: 
+
+Filename: lavis/projects/blip2/eval/caption_nocaps_out_domain_flant5xxl_eval.yaml
+Comment: 
+
 Filename: lavis/projects/blip2/eval/gqa_zeroshot_flant5xl_eval.yaml
 Comment: 
 
 Filename: lavis/projects/blip2/eval/okvqa_zeroshot_flant5xl_eval.yaml
 Comment: 
 
 Filename: lavis/projects/blip2/eval/ret_coco_eval.yaml
@@ -885,23 +4140,41 @@
 
 Filename: lavis/projects/blip2/eval/ret_flickr_eval.yaml
 Comment: 
 
 Filename: lavis/projects/blip2/eval/vqav2_zeroshot_flant5xl_eval.yaml
 Comment: 
 
+Filename: lavis/projects/blip2/eval/vqav2_zeroshot_opt_eval.yaml
+Comment: 
+
 Filename: lavis/projects/blip2/train/caption_coco_ft.yaml
 Comment: 
 
 Filename: lavis/projects/blip2/train/pretrain_stage1.yaml
 Comment: 
 
 Filename: lavis/projects/blip2/train/pretrain_stage2.yaml
 Comment: 
 
+Filename: lavis/projects/blip2/train/retrieval_coco_ft.yaml
+Comment: 
+
+Filename: lavis/projects/blip_diffusion/finetune-db-dog.yaml
+Comment: 
+
+Filename: lavis/projects/blip_diffusion/finetune-db-pink-dress.yaml
+Comment: 
+
+Filename: lavis/projects/blip_diffusion/finetune-db-shein-jacket.yaml
+Comment: 
+
+Filename: lavis/projects/blip_diffusion/finetune-db-template.yaml
+Comment: 
+
 Filename: lavis/projects/clip/exp_coco_ret_eval.yaml
 Comment: 
 
 Filename: lavis/projects/clip/exp_flickr_ret_eval.yaml
 Comment: 
 
 Filename: lavis/projects/clip/exp_imnet_zs_eval.yaml
@@ -909,14 +4182,164 @@
 
 Filename: lavis/projects/gpt/eval/dialogue_avsd_eval.yaml
 Comment: 
 
 Filename: lavis/projects/gpt/train/dialogue_avsd_ft.yaml
 Comment: 
 
+Filename: lavis/projects/instructblip/caption_coco_flant5xl_eval_test.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/caption_coco_flant5xl_eval_val.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/caption_coco_flant5xxl_eval_test.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/caption_coco_flant5xxl_eval_val.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/caption_coco_vicuna13b_eval_test.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/caption_coco_vicuna13b_eval_val.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/caption_coco_vicuna7b_eval_test.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/caption_coco_vicuna7b_eval_val.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/caption_msrvtt_flant5xl_eval_test.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/caption_msrvtt_flant5xl_eval_val.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/caption_msrvtt_flant5xxl_eval_test.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/caption_msrvtt_flant5xxl_eval_val.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/caption_msrvtt_vicuna13b_eval_test.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/caption_msrvtt_vicuna13b_eval_val.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/caption_msrvtt_vicuna7b_eval_test.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/caption_msrvtt_vicuna7b_eval_val.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/caption_msvd_flant5xl_eval.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/caption_msvd_flant5xxl_eval.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/caption_msvd_vicuna13b_eval.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/caption_msvd_vicuna7b_eval.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/caption_nocaps_out_domain_flant5xl_eval.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/caption_nocaps_out_domain_flant5xxl_eval.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/caption_nocaps_out_domain_vicuna13b_eval.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/caption_nocaps_out_domain_vicuna7b_eval.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/caption_vatex_flant5xl_eval.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/caption_vatex_flant5xxl_eval.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/caption_vatex_vicuna13b_eval.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/caption_vatex_vicuna7b_eval.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/classification_modelnet40_vicuna13b.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/classification_modelnet40_vicuna7b.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/classification_snlive_flant5xl.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/classification_snlive_flant5xxl.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/classification_snlive_vicuna13b.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/classification_snlive_vicuna13b_test.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/classification_snlive_vicuna7b_test.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/classification_snlive_vicuna7b_val.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/completion_modelnet40_vicuna13b.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/completion_modelnet40_vicuna7b.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/qa_msrvtt_flant5xl_eval_test.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/qa_msrvtt_flant5xxl_eval_test.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/qa_msrvtt_vicuna13b_eval_test.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/qa_msrvtt_vicuna7b_eval_test.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/qa_msvd_flant5xl_eval.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/qa_msvd_flant5xxl_eval.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/qa_msvd_vicuna13b_eval.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/qa_msvd_vicuna7b_eval.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/qa_okvqa_flant5xl_eval.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/qa_okvqa_flant5xxl_eval.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/qa_okvqa_vicuna13b_eval.yaml
+Comment: 
+
+Filename: lavis/projects/instructblip/qa_okvqa_vicuna7b_eval.yaml
+Comment: 
+
 Filename: lavis/projects/pnp-vqa/eval/gqa_eval.yaml
 Comment: 
 
 Filename: lavis/projects/pnp-vqa/eval/gqa_eval_3b.yaml
 Comment: 
 
 Filename: lavis/projects/pnp-vqa/eval/gqa_eval_large.yaml
@@ -945,14 +4368,905 @@
 
 Filename: lavis/projects/pnp-vqa/eval/vqav2_test_eval_3b.yaml
 Comment: 
 
 Filename: lavis/projects/pnp-vqa/eval/vqav2_test_eval_large.yaml
 Comment: 
 
+Filename: lavis/projects/xinstruct_blip/eval/discrn/audio_video_caption.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/discrn/audio_video_caption_13b.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/discrn/audio_video_describe.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/discrn/audio_video_describe_13b.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/discrn/audio_video_describe_nocue.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/discrn/audio_video_describe_proj copy.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/discrn/audio_video_describe_proj.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/discrn/audio_video_describe_rand_init.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/discrn/image_3d_caption.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/discrn/image_3d_caption_13b.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/discrn/image_3d_describe.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/discrn/image_3d_describe_13b.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/discrn/image_3d_describe_no_init.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/discrn/image_3d_describe_nocue.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/discrn/image_3d_describe_proj.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/audio/audiocaps_captioning_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/audio/audiocaps_captioning_test.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/audio/audiocaps_captioning_val.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/audio/clothoQA_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/audio/clothov1_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/audio/clothov2_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/audio/esc50_classification.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/audio/esc50_classification_completion.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/crossmodal/musicavqa/musicavqa_audio_eval.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/crossmodal/musicavqa/musicavqa_joint_eval.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/crossmodal/musicavqa/musicavqa_video_eval.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/crossmodal/vatex/vatex_audio_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/crossmodal/vatex/vatex_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/crossmodal/vatex/vatex_joint_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/crossmodal/vatex/vatex_joint_captioning_interleave.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/image/coco_captioning_test.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/image/coco_captioning_val.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/image/flickr30k_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/image/gqa_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/image/nocaps_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/image/nocaps_out_domain_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/image/okvqa_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/image/snlive_classification_test.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/image/snlive_classification_val.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/image/vizwiz_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/image_with_coco/coco_captioning_test.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/image_with_coco/coco_captioning_val.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/image_with_coco/flickr30k_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/image_with_coco/gqa_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/image_with_coco/nocaps_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/image_with_coco/nocaps_out_domain_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/image_with_coco/okvqa_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/image_with_coco/snlive_classification_test.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/image_with_coco/snlive_classification_val.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/image_with_coco/vizwiz_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/pc/modelnet40_classification.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/pc/modelnet40_completion.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/pc/objaverse_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/pc/objaverse_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/video/msrvtt_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/video/msrvtt_captioning_test.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/video/msrvtt_captioning_val.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/video/msrvtt_qa_test.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/video/msrvtt_qa_val.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/video/msvd_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/video/msvd_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/video/vatex_audio_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/video/vatex_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/video/vatex_joint_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/video/vatex_joint_captioning_interleave.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/video_image/msvd_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/video_image/msvd_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna13b/video_image/vatex_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/audio/audiocaps_captioning_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/audio/audiocaps_captioning_test.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/audio/audiocaps_captioning_val.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/audio/clothoQA_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/audio/clothov1_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/audio/clothov2_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/audio/esc50_classification.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/audio/esc50_classification_completion.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/audio_no_init/audiocaps_captioning_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/audio_no_init/audiocaps_captioning_test.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/audio_no_init/audiocaps_captioning_val.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/audio_no_init/clothoQA_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/audio_no_init/clothov1_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/audio_no_init/clothov2_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/audio_no_init/esc50_classification.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/audio_no_init/esc50_classification_completion.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/audio_projection_only/audiocaps_captioning_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/audio_projection_only/audiocaps_captioning_test.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/audio_projection_only/audiocaps_captioning_val.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/audio_projection_only/clothoQA_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/audio_projection_only/clothov1_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/audio_projection_only/clothov2_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/audio_projection_only/esc50_classification.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/audio_projection_only/esc50_classification_completion.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/audio_projection_only_nocue/audiocaps_captioning_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/audio_projection_only_nocue/audiocaps_captioning_test.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/audio_projection_only_nocue/audiocaps_captioning_val.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/audio_projection_only_nocue/clothoQA_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/audio_projection_only_nocue/clothov1_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/audio_projection_only_nocue/clothov2_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/audio_projection_only_nocue/esc50_classification.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/audio_projection_only_nocue/esc50_classification_completion.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/crossmodal/musicavqa/musicavqa_audio_eval.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/crossmodal/musicavqa/musicavqa_joint_eval.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/crossmodal/musicavqa/musicavqa_video_eval.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/crossmodal/vatex/vatex_audio_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/crossmodal/vatex/vatex_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/crossmodal/vatex/vatex_joint_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/crossmodal/vatex/vatex_joint_captioning_interleave.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image/coco_captioning_test.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image/coco_captioning_val.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image/flickr30k_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image/gqa_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image/gqa_qa_val.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image/nocaps_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image/nocaps_out_domain_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image/okvqa_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image/snlive_classification_test.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image/snlive_classification_val.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image/vizwiz_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_full_init/coco_captioning_test.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_full_init/coco_captioning_val.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_full_init/flickr30k_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_full_init/gqa_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_full_init/gqa_qa_val.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_full_init/nocaps_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_full_init/nocaps_out_domain_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_full_init/okvqa_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_full_init/snlive_classification_test.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_full_init/snlive_classification_val.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_full_init/vizwiz_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_no_init/coco_captioning_test.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_no_init/coco_captioning_val.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_no_init/flickr30k_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_no_init/gqa_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_no_init/gqa_qa_val.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_no_init/nocaps_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_no_init/nocaps_out_domain_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_no_init/okvqa_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_no_init/snlive_classification_test.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_no_init/snlive_classification_val.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_no_init/vizwiz_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_pre_coco/coco_captioning_test.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_pre_coco/coco_captioning_val.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_pre_coco/flickr30k_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_pre_coco/gqa_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_pre_coco/nocaps_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_pre_coco/nocaps_out_domain_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_pre_coco/okvqa_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_pre_coco/snlive_classification_test.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_pre_coco/snlive_classification_val.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_pre_coco/vizwiz_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_projection_only/coco_captioning_test.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_projection_only/coco_captioning_val.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_projection_only/flickr30k_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_projection_only/gqa_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_projection_only/gqa_qa_val.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_projection_only/nocaps_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_projection_only/nocaps_out_domain_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_projection_only/okvqa_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_projection_only/snlive_classification_test.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_projection_only/snlive_classification_val.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/image_projection_only/vizwiz_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/pc/modelnet40_classification.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/pc/modelnet40_completion.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/pc/objaverse_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/pc/objaverse_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/pc_no_init/modelnet40_classification.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/pc_no_init/modelnet40_completion.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/pc_no_init/objaverse_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/pc_no_init/objaverse_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/pc_projection_only/modelnet40_classification.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/pc_projection_only/modelnet40_completion.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/pc_projection_only/objaverse_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/pc_projection_only/objaverse_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip1/modelnet40_classification.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip1/modelnet40_completion.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip1/objaverse_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip1/objaverse_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip2_scaled_up/modelnet40_classification.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip2_scaled_up/modelnet40_completion.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip2_scaled_up/objaverse_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip2_scaled_up/objaverse_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip_objaverse/modelnet40_classification.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip_objaverse/modelnet40_completion.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip_objaverse/objaverse_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip_objaverse/objaverse_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip_objaverse_shapenet/modelnet40_classification.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip_objaverse_shapenet/modelnet40_completion.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip_objaverse_shapenet/objaverse_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip_objaverse_shapenet/objaverse_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip_shapenet/modelnet40_classification.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip_shapenet/modelnet40_completion.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip_shapenet/objaverse_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/pc_ulip_shapenet/objaverse_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/video/msrvtt_captioning_test.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/video/msrvtt_captioning_val.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/video/msrvtt_qa_test.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/video/msrvtt_qa_val.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/video/msvd_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/video/msvd_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/video/vatex_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/video_image/msvd_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/video_image/msvd_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/video_image/vatex_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/video_image_pre_coco/msvd_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/video_image_pre_coco/msvd_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/video_image_pre_coco/vatex_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/video_no_upsample/msrvtt_captioning_test.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/video_no_upsample/msrvtt_captioning_val.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/video_no_upsample/msrvtt_qa_test.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/video_no_upsample/msrvtt_qa_val.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/video_no_upsample/msvd_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/video_no_upsample/msvd_captioning_up.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/video_no_upsample/msvd_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/video_no_upsample/msvd_qa_up.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/video_no_upsample/vatex_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b/video_no_upsample/vatex_captioning_up.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/audio/audiocaps_captioning_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/audio/audiocaps_captioning_test.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/audio/audiocaps_captioning_val.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/audio/clothoQA_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/audio/clothov1_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/audio/clothov2_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/audio/esc50_classification.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/audio/esc50_classification_completion.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/crossmodal/musicavqa/musicavqa_audio_eval.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/crossmodal/musicavqa/musicavqa_joint_eval.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/crossmodal/musicavqa/musicavqa_video_eval.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/crossmodal/vatex/vatex_audio_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/crossmodal/vatex/vatex_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/crossmodal/vatex/vatex_joint_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/image/coco_captioning_test.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/image/coco_captioning_val.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/image/flickr30k_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/image/gqa_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/image/nocaps_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/image/nocaps_out_domain_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/image/okvqa_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/image/snlive_classification_test.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/image/snlive_classification_val.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/image/vizwiz_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/pc/modelnet40_classification.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/pc/modelnet40_completion.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/pc/objaverse_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/pc/objaverse_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/video/msrvtt_captioning_test.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/video/msrvtt_captioning_val.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/video/msrvtt_qa_test.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/video/msrvtt_qa_val.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/video/msvd_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/video/msvd_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/video/vatex_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/video_image/msvd_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/video_image/msvd_qa.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/eval/vicuna7b_nocue/video_image/vatex_captioning.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/prompt_variation/nocaps/instructblip/original.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/prompt_variation/nocaps/instructblip/template_1.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/prompt_variation/nocaps/instructblip/template_2.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/prompt_variation/nocaps/instructblip/template_3.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/prompt_variation/nocaps/instructblip/template_4.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/prompt_variation/nocaps/instructblip/template_5.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/prompt_variation/nocaps/xinstructblip/template_1.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/prompt_variation/nocaps/xinstructblip/template_2.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/prompt_variation/nocaps/xinstructblip/template_3.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/prompt_variation/nocaps/xinstructblip/template_4.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/prompt_variation/nocaps/xinstructblip/template_5.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/train/vicuna13b/audio_training.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/train/vicuna13b/audio_training_continue.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/train/vicuna13b/image_train.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/train/vicuna13b/image_train_continue.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/train/vicuna13b/pc_training.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/train/vicuna13b/video_training.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/train/vicuna7b/audio_training.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/train/vicuna7b/audio_training_improved.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/train/vicuna7b/audio_training_no_init.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/train/vicuna7b/audio_training_projection_only.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/train/vicuna7b/audio_training_projection_only_nocue.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/train/vicuna7b/image_train.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/train/vicuna7b/image_train_improved.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/train/vicuna7b/image_train_no_init.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/train/vicuna7b/image_train_projection_only.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/train/vicuna7b/lora_training.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/train/vicuna7b/pc_training.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/train/vicuna7b/pc_training_improved.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/train/vicuna7b/pc_training_no_init.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/train/vicuna7b/pc_training_projection_only.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/train/vicuna7b/pc_training_projection_only_nocue.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/train/vicuna7b/pc_training_scaled_up.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/train/vicuna7b/pc_training_ulip1.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/train/vicuna7b/pc_training_ulip2_objaverse_shapenet_k_1.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/train/vicuna7b/pc_training_ulip_objaverse.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/train/vicuna7b/pc_training_ulip_shapenet.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/train/vicuna7b/video_training.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/train/vicuna7b/video_training_no_msrvtt_upsample.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/train/vicuna7b_nocue/audio_training.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/train/vicuna7b_nocue/image_train.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/train/vicuna7b_nocue/pc_training.yaml
+Comment: 
+
+Filename: lavis/projects/xinstruct_blip/train/vicuna7b_nocue/video_training.yaml
+Comment: 
+
 Filename: lavis/runners/__init__.py
 Comment: 
 
 Filename: lavis/runners/runner_base.py
 Comment: 
 
 Filename: lavis/runners/runner_iter.py
@@ -975,44 +5289,83 @@
 
 Filename: lavis/tasks/multimodal_classification.py
 Comment: 
 
 Filename: lavis/tasks/retrieval.py
 Comment: 
 
+Filename: lavis/tasks/text_to_image_generation.py
+Comment: 
+
 Filename: lavis/tasks/vqa.py
 Comment: 
 
 Filename: lavis/tasks/vqa_reading_comprehension.py
 Comment: 
 
-Filename: projects/img2prompt-vqa/img2prompt_vqa.py
+Filename: projects/img2llm-vqa/img2llm_vqa.py
+Comment: 
+
+Filename: projects/instructblip/run_demo.py
+Comment: 
+
+Filename: projects/xinstructblip/data_aug/3d_qa_data_generation.py
+Comment: 
+
+Filename: projects/xinstructblip/data_aug/audio_qa_data_generation.py
+Comment: 
+
+Filename: projects/xinstructblip/demo/run_demo.py
+Comment: 
+
+Filename: projects/xinstructblip/discrn/caption_baseline/predict_audio.py
+Comment: 
+
+Filename: projects/xinstructblip/discrn/caption_baseline/predict_image.py
+Comment: 
+
+Filename: projects/xinstructblip/discrn/caption_baseline/predict_pc.py
+Comment: 
+
+Filename: projects/xinstructblip/discrn/caption_baseline/predict_video.py
+Comment: 
+
+Filename: projects/xinstructblip/discrn/caption_baseline/render_images.py
+Comment: 
+
+Filename: projects/xinstructblip/discrn/data_generation/audiocaps_video_audio.py
+Comment: 
+
+Filename: projects/xinstructblip/discrn/data_generation/objaverse_img_3d.py
+Comment: 
+
+Filename: projects/xinstructblip/modelnet_baseline/render_images.py
 Comment: 
 
 Filename: tests/models/test_albef.py
 Comment: 
 
 Filename: tests/models/test_blip.py
 Comment: 
 
 Filename: tests/models/test_blip2.py
 Comment: 
 
 Filename: tests/models/test_pnp_vqa.py
 Comment: 
 
-Filename: lavis_gml-1.0.2.post3.dist-info/LICENSE.txt
+Filename: lavis_gml-1.0.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: lavis_gml-1.0.2.post3.dist-info/METADATA
+Filename: lavis_gml-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: lavis_gml-1.0.2.post3.dist-info/WHEEL
+Filename: lavis_gml-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: lavis_gml-1.0.2.post3.dist-info/top_level.txt
+Filename: lavis_gml-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: lavis_gml-1.0.2.post3.dist-info/RECORD
+Filename: lavis_gml-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lavis/common/optims.py

```diff
@@ -90,14 +90,36 @@
                 optimizer=self.optimizer,
                 max_epoch=self.max_epoch,
                 init_lr=self.init_lr,
                 min_lr=self.min_lr,
             )
 
 
+@registry.register_lr_scheduler("constant_lr")
+class ConstantLRScheduler:
+    def __init__(self, optimizer, init_lr, warmup_start_lr=-1, warmup_steps=0, **kwargs):
+        self.optimizer = optimizer
+        self.lr = init_lr
+        self.warmup_start_lr = warmup_start_lr if warmup_start_lr >= 0 else init_lr
+        self.warmup_steps = warmup_steps
+    
+    def step(self, cur_epoch, cur_step):
+        if cur_epoch == 0:
+            warmup_lr_schedule(
+                step=cur_step,
+                optimizer=self.optimizer,
+                max_step=self.warmup_steps,
+                init_lr=self.warmup_start_lr,
+                max_lr=self.lr,
+            )
+        else:
+            for param_group in self.optimizer.param_groups:
+                param_group["lr"] = self.lr
+
+
 def cosine_lr_schedule(optimizer, epoch, max_epoch, init_lr, min_lr):
     """Decay the learning rate"""
     lr = (init_lr - min_lr) * 0.5 * (
         1.0 + math.cos(math.pi * epoch / max_epoch)
     ) + min_lr
     for param_group in optimizer.param_groups:
         param_group["lr"] = lr
```

## lavis/common/utils.py

```diff
@@ -1,32 +1,34 @@
 """
- Copyright (c) 2022, salesforce.com, inc.
+ Copyright (c) 2023, salesforce.com, inc.
  All rights reserved.
  SPDX-License-Identifier: BSD-3-Clause
  For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 """
 
 import io
 import json
 import logging
 import os
 import pickle
 import re
 import shutil
+import tarfile
 import urllib
 import urllib.error
 import urllib.request
 from typing import Optional
 from urllib.parse import urlparse
 
 import numpy as np
 import pandas as pd
 import yaml
 from iopath.common.download import download
 from iopath.common.file_io import file_lock, g_pathmgr
+from lavis.common.dist_utils import download_cached_file
 from lavis.common.registry import registry
 from torch.utils.model_zoo import tqdm
 from torchvision.datasets.utils import (
     check_integrity,
     download_file_from_google_drive,
     extract_archive,
 )
@@ -401,14 +403,30 @@
     """
     Check if an input string is a url. look for http(s):// and ignoring the case
     """
     is_url = re.match(r"^(?:http)s?://", input_url, re.IGNORECASE) is not None
     return is_url
 
 
+def download_and_untar(url):
+    cached_file = download_cached_file(
+        url, check_hash=False, progress=True
+    )
+    # get path to untarred directory
+    untarred_dir = os.path.basename(url).split(".")[0]
+    parent_dir = os.path.dirname(cached_file)
+
+    full_dir = os.path.join(parent_dir, untarred_dir)
+
+    if not os.path.exists(full_dir):
+        with tarfile.open(cached_file) as tar:
+            tar.extractall(parent_dir)
+
+    return full_dir
+
 def cleanup_dir(dir):
     """
     Utility for deleting a directory. Useful for cleaning the storage space
     that contains various training artifacts like checkpoints, data etc.
     """
     if os.path.exists(dir):
         logging.info(f"Deleting directory: {dir}")
@@ -418,7 +436,20 @@
 
 def get_file_size(filename):
     """
     Given a file, get the size of file in MB
     """
     size_in_mb = os.path.getsize(filename) / float(1024**2)
     return size_in_mb
+
+def is_serializable(value):
+    """
+    This function checks if the provided value can be serialized into a JSON string.
+    """
+    try:
+        json.dumps(value)
+        return True
+    except (TypeError, OverflowError):
+        return False
+
+def is_convertible_to_int(value):
+    return bool(re.match(r'^-?\d+$', str(value)))
```

## lavis/configs/datasets/vatex/defaults_cap.yaml

```diff
@@ -1,8 +1,8 @@
- # Copyright (c) 2022, salesforce.com, inc.
+ # Copyright (c) 2023, salesforce.com, inc.
  # All rights reserved.
  # SPDX-License-Identifier: BSD-3-Clause
  # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 
 datasets:
   msvd_cap: # name of the dataset builder
     # data_dir: ${env.data_dir}/datasets
```

## lavis/datasets/data_utils.py

```diff
@@ -7,14 +7,15 @@
 
 import gzip
 import logging
 import os
 import random as rnd
 import tarfile
 import zipfile
+import cv2
 
 import decord
 import webdataset as wds
 import numpy as np
 import torch
 from torch.utils.data.dataset import IterableDataset, ChainDataset
 from decord import VideoReader
@@ -46,15 +47,16 @@
     # get_batch -> T, H, W, C
     frms = vr.get_batch(indices).permute(3, 0, 1, 2).float()  # (C, T, H, W)
 
     return frms
 
 
 def apply_to_sample(f, sample):
-    if len(sample) == 0:
+    ## add check for datasets that return none samples for missing items
+    if sample == None or len(sample) == 0:
         return {}
 
     def _apply(x):
         if torch.is_tensor(x):
             return f(x)
         elif isinstance(x, dict):
             return {key: _apply(value) for key, value in x.items()}
@@ -278,7 +280,72 @@
 
     grid = make_grid(img_array)
     ndarr = grid.permute(1, 2, 0).to("cpu", torch.uint8).numpy()
 
     img = Image.fromarray(ndarr)
 
     img.save(out_path)
+
+
+def uniform_frame_sampling(video_path, num_frames, target_height, target_width, start_time=None, end_time=None):
+    cap = cv2.VideoCapture(video_path)
+    total_frames = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
+    frame_rate = cap.get(cv2.CAP_PROP_FPS)
+
+    if start_time is None:
+        start_time = 0
+    if end_time is None:
+        end_time = total_frames / frame_rate
+
+    start_frame = int(start_time * frame_rate)
+    end_frame = int(end_time * frame_rate)
+    frame_indices = list(range(start_frame, end_frame + 1, (end_frame - start_frame + 1) // num_frames))
+
+    frames = []
+    for frame_index in frame_indices:
+        cap.set(cv2.CAP_PROP_POS_FRAMES, frame_index)
+        ret, frame = cap.read()
+        if not ret:
+            break
+        frame = cv2.resize(frame, (target_width, target_height))
+        frames.append(frame)
+
+    cap.release()
+    return frames
+
+
+def head_tail_frame_sampling(video_path, num_frames, target_height, target_width, start_time=None, end_time=None):
+    cap = cv2.VideoCapture(video_path)
+    total_frames = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
+    frame_rate = cap.get(cv2.CAP_PROP_FPS)
+
+    if start_time is None:
+        start_time = 0
+    if end_time is None:
+        end_time = total_frames / frame_rate
+
+    start_frame = int(start_time * frame_rate)
+    end_frame = int(end_time * frame_rate)
+    frame_indices = [start_frame] + [start_frame + (end_frame - start_frame) // (num_frames - 1) * i for i in range(1, num_frames - 1)] + [end_frame]
+
+    frames = []
+    for frame_index in frame_indices:
+        cap.set(cv2.CAP_PROP_POS_FRAMES, frame_index)
+        ret, frame = cap.read()
+        if not ret:
+            break
+        frame = cv2.resize(frame, (target_width, target_height))
+        frames.append(frame)
+
+    cap.release()
+    if len(frames) == 0:
+        return None
+    return torch.stack([torch.tensor(f).permute(2,0,1).float() for f in frames], dim=1)
+
+
+def load_clip(video_path, num_frames, target_height, target_width, start_time=None, end_time=None, sampling="headtail"):
+    if sampling == "headtail":
+        return head_tail_frame_sampling(video_path, num_frames, target_height, target_width, start_time, end_time)
+    elif sampling == "uniform":
+        return uniform_frame_sampling(video_path, num_frames, target_height, target_width, start_time, end_time)
+    else:
+        raise NotImplementedError
```

## lavis/datasets/builders/__init__.py

```diff
@@ -7,44 +7,129 @@
 
 from lavis.datasets.builders.base_dataset_builder import load_dataset_config
 from lavis.datasets.builders.caption_builder import (
     COCOCapBuilder,
     MSRVTTCapBuilder,
     MSVDCapBuilder,
     VATEXCapBuilder,
+    MSRVTTCapInstructBuilder,
+    MSVDCapInstructBuilder,
+    VATEXCapInstructBuilder,
+    WebVid2MCapBuilder,
+    WebVid2MCapInstructBuilder,
+    VALORCaptionBuilder,
+    VALORCaptionInstructBuilder,
+    ViolinCapBuilder,
+    ViolinCapInstructBuilder,
+    VlepCaptionInstructBuilder, 
+    VlepCaptionBuilder,
+    YouCookCaptionBuilder,
+    YouCookCaptionInstructBuilder,
+    COINCaptionBuilder,
+    COINCaptionInstructBuilder,
+    CharadeCaptionBuilder,
+    CharadeCaptionInstructBuilder,
+    TextCapsCapBuilder,
+    TextCapsCapInstructBuilder,
+    Flickr30kCapBuilder,
+    Flickr30kCapInstructBuilder
+
 )
 from lavis.datasets.builders.image_text_pair_builder import (
     ConceptualCaption12MBuilder,
+    ConceptualCaption12MInstructBuilder,
     ConceptualCaption3MBuilder,
+    ConceptualCaption3MInstructBuilder,
     VGCaptionBuilder,
+    VGCaptionInstructBuilder,
     SBUCaptionBuilder,
+    SBUCaptionInstructBuilder,
+    Laion400MBuilder,
+    Laion400MInstructBuilder
 )
 from lavis.datasets.builders.classification_builder import (
     NLVRBuilder,
     SNLIVisualEntailmentBuilder,
+    SNLIVisualEntailmentInstructBuilder,
+    ViolinEntailmentInstructBuilder,
+    ViolinEntailmentBuilder,
+    ESC50ClassificationBuilder
 )
 from lavis.datasets.builders.imagefolder_builder import ImageNetBuilder
-from lavis.datasets.builders.video_qa_builder import MSRVTTQABuilder, MSVDQABuilder
+from lavis.datasets.builders.video_qa_builder import (
+    MSRVTTQABuilder, 
+    MSVDQABuilder,
+    MSRVTTQAInstructBuilder,
+    MSVDQAInstructBuilder,
+    MusicAVQABuilder,
+    MusicAVQAInstructBuilder
+)
+
 from lavis.datasets.builders.vqa_builder import (
     COCOVQABuilder,
+    COCOVQAInstructBuilder,
     OKVQABuilder,
+    OKVQAInstructBuilder,
+    AOKVQABuilder,
+    AOKVQAInstructBuilder,
     VGVQABuilder,
+    VGVQAInstructBuilder,
     GQABuilder,
+    GQAInstructBuilder,
+    IconQABuilder,
+    IconQAInstructBuilder,
+    ScienceQABuilder,
+    ScienceQAInstructBuilder,
+    OCRVQABuilder,
+    OCRVQAInstructBuilder,
+    VizWizVQABuilder
 )
 from lavis.datasets.builders.retrieval_builder import (
     MSRVTTRetrievalBuilder,
     DiDeMoRetrievalBuilder,
     COCORetrievalBuilder,
     Flickr30kBuilder,
 )
-from lavis.datasets.builders.dialogue_builder import AVSDDialBuilder
+
+from lavis.datasets.builders.audio_caption_builder import (
+    AudioSetBuilder,
+    AudioCapsCapBuilder,
+    AudioSetInstructBuilder,
+    AudioCapsInstructCapBuilder,
+    WavCapsCapInstructBuilder,
+    WavCapsCapBuilder
+)
+
+from lavis.datasets.builders.object3d_caption_builder import (
+    ObjaverseCaptionInstructBuilder,
+    ShapenetCaptionInstructBuilder,
+    ObjaverseCaptionBuilder,
+    ShapenetCaptionBuilder
+)
+from lavis.datasets.builders.object3d_qa_builder import ObjaverseQABuilder
+from lavis.datasets.builders.object3d_classification_builder import ModelNetClassificationBuilder
+
+from lavis.datasets.builders.audio_qa_builder import AudioCapsQABuilder, ClothoQABuilder
+
+from lavis.datasets.builders.dialogue_builder import (
+    AVSDDialBuilder, 
+    AVSDDialInstructBuilder,
+    YT8MDialBuilder,
+    LLaVA150kDialInstructBuilder,
+    VisDialBuilder,
+    VisDialInstructBuilder
+)
+from lavis.datasets.builders.text_to_image_generation_builder import BlipDiffusionFinetuneBuilder
+
+from lavis.datasets.builders.discrn_builders import DiscrnImagePcBuilder, DiscrnAudioVideoBuilder
 
 from lavis.common.registry import registry
 
 __all__ = [
+    "BlipDiffusionFinetuneBuilder",
     "COCOCapBuilder",
     "COCORetrievalBuilder",
     "COCOVQABuilder",
     "ConceptualCaption12MBuilder",
     "ConceptualCaption3MBuilder",
     "DiDeMoRetrievalBuilder",
     "Flickr30kBuilder",
@@ -53,20 +138,96 @@
     "MSRVTTCapBuilder",
     "MSRVTTQABuilder",
     "MSRVTTRetrievalBuilder",
     "MSVDCapBuilder",
     "MSVDQABuilder",
     "NLVRBuilder",
     "OKVQABuilder",
+    "AOKVQABuilder",
     "SBUCaptionBuilder",
     "SNLIVisualEntailmentBuilder",
     "VATEXCapBuilder",
     "VGCaptionBuilder",
     "VGVQABuilder",
     "AVSDDialBuilder",
+    "Laion400MBuilder",
+
+    "ViolinCapBuilder",
+    "ViolinEntailmentBuilder",
+    "VlepCaptionBuilder",
+    "YouCookCaptionBuilder",
+    "COINCaptionBuilder",
+    "CharadeCaptionBuilder",
+    "YT8MDialBuilder",
+    "IconQABuilder",
+    "ScienceQABuilder",
+    "VisDialBuilder",
+    "OCRVQABuilder",
+    "VizWizVQABuilder",
+    "TextCapsCapBuilder",
+    "Flickr30kCapBuilder",
+    "AudioSetBuilder",
+    "AudioCapsCapBuilder",
+    "WavCapsCapBuilder",
+    "WebVid2MCapBuilder",
+    "VALORCaptionBuilder",
+    "ObjaverseCaptionBuilder",
+    "ShapenetCaptionBuilder",
+    "ObjaverseQABuilder",
+    "MusicAVQABuilder",
+    "ESC50ClassificationBuilder",
+
+    ## Instruction Builders
+    "AOKVQAInstructBuilder",
+    "OKVQAInstructBuilder",
+    "AudioSetInstructBuilder",
+    "AudioCapsInstructCapBuilder",
+    "AudioCapsQABuilder",
+    "WavCapsCapInstructBuilder",
+    "ObjaverseCaptionInstructBuilder",
+    "ShapenetCaptionInstructBuilder",
+    "ModelNetClassificationBuilder",
+    "ObjaverseCaptionInstructBuilder",
+    "MSRVTTCapInstructBuilder",
+    "MSVDCapInstructBuilder",
+    "VATEXCapInstructBuilder",
+    "WebVid2MCapInstructBuilder",
+    "MSRVTTQAInstructBuilder",
+    "MSVDQAInstructBuilder",
+    "VALORCaptionInstructBuilder",
+    "AVSDDialInstructBuilder",
+    "VisDialInstructBuilder",
+    "MusicAVQAInstructBuilder",
+    "ViolinCapInstructBuilder",
+    "ViolinEntailmentInstructBuilder",
+    "VlepCaptionInstructBuilder", 
+    "YouCookCaptionInstructBuilder",
+    "COINCaptionInstructBuilder",
+    "CharadeCaptionInstructBuilder",
+    "COCOVQAInstructBuilder",
+    "VGVQAInstructBuilder",
+    "GQAInstructBuilder",
+    "IconQAInstructBuilder",
+    "SNLIVisualEntailmentInstructBuilder",
+    "Laion400MInstructBuilder",
+    "LLaVA150kDialInstructBuilder",
+    "ScienceQAInstructBuilder",
+    "OCRVQAInstructBuilder",
+    "TextCapsCapInstructBuilder",
+    "Flickr30kCapInstructBuilder",
+    "ConceptualCaption12MInstructBuilder",
+    "ConceptualCaption3MInstructBuilder",
+    "VGCaptionInstructBuilder",
+    "SBUCaptionInstructBuilder",
+    "ClothoQABuilder",
+
+    # DisCRN
+    "DiscrnImagePcBuilder",
+    "DiscrnAudioVideoBuilder"
+
 ]
 
 
 def load_dataset(name, cfg_path=None, vis_path=None, data_type=None):
     """
     Example
```

## lavis/datasets/builders/base_dataset_builder.py

```diff
@@ -36,14 +36,17 @@
             self.config = cfg
 
         self.data_type = self.config.data_type
 
         self.vis_processors = {"train": BaseProcessor(), "eval": BaseProcessor()}
         self.text_processors = {"train": BaseProcessor(), "eval": BaseProcessor()}
 
+        # additional processors, each specified by a name in string.
+        self.kw_processors = {}
+
     def build_datasets(self):
         # download, split, etc...
         # only called on 1 GPU/TPU in distributed
 
         if is_main_process():
             self._download_data()
 
@@ -69,15 +72,20 @@
 
         if txt_proc_cfg is not None:
             txt_train_cfg = txt_proc_cfg.get("train")
             txt_eval_cfg = txt_proc_cfg.get("eval")
 
             self.text_processors["train"] = self._build_proc_from_cfg(txt_train_cfg)
             self.text_processors["eval"] = self._build_proc_from_cfg(txt_eval_cfg)
-
+        
+        kw_proc_cfg = self.config.get("kw_processor")
+        if kw_proc_cfg is not None:
+            for name, cfg in kw_proc_cfg.items():
+                self.kw_processors[name] = self._build_proc_from_cfg(cfg)
+        
     @staticmethod
     def _build_proc_from_cfg(cfg):
         return (
             registry.get_processor_class(cfg.name).from_config(cfg)
             if cfg is not None
             else None
         )
@@ -223,12 +231,97 @@
                 ann_paths=ann_paths,
                 vis_root=vis_path,
             )
 
         return datasets
 
 
+class MultiModalDatasetBuilder(BaseDatasetBuilder):
+    """
+    MultiModalDatasetBuilder is a utility class designed to construct datasets
+    suitable for multi-modal tasks. This class simplifies the creation of 
+    datasets that incorporate data of multiple modalities, such as text, 
+    images, video, or audio.
+    """
+    train_dataset_cls, eval_dataset_cls = None, None
+
+    def __init__(self, cfg=None):
+        super().__init__(cfg)
+        if isinstance(self.data_type, str):
+            self.data_type = [self.data_type]
+
+    def _build_processor(self, cfg_name):
+        cfg = self.config.get(cfg_name)
+        return {
+            split: self._build_proc_from_cfg(cfg.get(split)) 
+            if cfg is not None 
+            else None
+            for split in ['train', 'eval']
+        }
+
+    def build_processors(self):
+        self.text_processors = self._build_processor("text_processor")
+        
+        self.processors = {
+            split: {
+                modality: self._build_proc_from_cfg(
+                    self.config.get(f"{'vis' if 'image' in modality else modality}_processor").get(split)
+                )
+                for modality in self.data_type
+            }
+            for split in ['train', 'eval']
+        }
+
+    def _download_multimodal(self, modality):
+        storage_path = utils.get_cache_path(self.config.build_info.get(modality).storage)
+        if not os.path.exists(storage_path):
+            warnings.warn(f"The specified path {storage_path} for {modality} inputs does not exist.")
+
+    def _download_data(self):
+        self._download_ann()
+        for modality in self.data_type:
+            self._download_multimodal(modality)
+
+    def _get_absolute_path(self, path):
+        if not os.path.isabs(path):
+            return utils.get_cache_path(path)
+        return path
+
+    def build(self):
+        self.build_processors()
+        build_info = self.config.build_info
+        datasets = {}
+        
+        for split, info in build_info.annotations.items():
+            if split not in ["train", "val", "test"]:
+                continue
+
+            is_train = split == "train"
+            dataset_args = self._get_dataset_args(info, is_train)
+            
+            dataset_cls = self.train_dataset_cls if is_train else self.eval_dataset_cls
+            datasets[split] = dataset_cls(**dataset_args)
+
+        return datasets
+
+    def _get_dataset_args(self, info, is_train):
+        dataset_args = dict(self.config.build_info.get('kwargs', {}))
+        
+        for modality in self.data_type:
+            proc_name = f"{'vis' if 'image' in modality else modality}_processor"
+            dataset_args[proc_name] = self.processors["train" if is_train else "eval"][modality]
+            mm_path = self._get_absolute_path(self.config.build_info.get(modality).storage)
+            dataset_args[f"{'vis' if 'image' in modality  else modality}_root"] = mm_path
+        
+        dataset_args['text_processor'] = self.text_processors["train" if is_train else "eval"]
+        dataset_args["ann_paths"] = [self._get_absolute_path(path) for path in info.storage]
+        dataset_args['modalities'] = self.data_type
+        
+        # Conform to base
+        for key in ['vis_processor', 'vis_root', 'test_processor']:
+            dataset_args.setdefault(key, None)
+        
+        return dataset_args
+
 def load_dataset_config(cfg_path):
     cfg = OmegaConf.load(cfg_path).datasets
-    cfg = cfg[list(cfg.keys())[0]]
-
-    return cfg
+    return next(iter(cfg.values()))
```

## lavis/datasets/builders/caption_builder.py

```diff
@@ -1,46 +1,141 @@
 """
  Copyright (c) 2022, salesforce.com, inc.
  All rights reserved.
  SPDX-License-Identifier: BSD-3-Clause
  For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 """
 
-from lavis.datasets.builders.base_dataset_builder import BaseDatasetBuilder
+from lavis.datasets.builders.base_dataset_builder import BaseDatasetBuilder, MultiModalDatasetBuilder
+from lavis.datasets.datasets.capfilt_dataset import CapFiltCaptionInstructDataset, CapFiltCaptionDataset
 from lavis.datasets.datasets.coco_caption_datasets import (
     COCOCapDataset,
+    COCOCapInstructDataset,
     COCOCapEvalDataset,
     NoCapsEvalDataset,
 )
 
 from lavis.common.registry import registry
 from lavis.datasets.datasets.video_caption_datasets import (
     VideoCaptionDataset,
     VideoCaptionEvalDataset,
+    ClipCaptionDataset,
+    ClipCaptionInstructDataset,
+    ClipCaptionEvalDataset,
+    VideoCaptionInstructDataset,
+    WebVideoCaptionDataset,
+    WebVideoCaptionInstructDataset,
 )
-
+from lavis.datasets.datasets.violin_dataset import (
+    ViolinVideoCaptionDataset,
+    ViolinVideoCaptionInstructDataset,
+    ViolinVideoCaptionEvalDataset
+)
+from lavis.datasets.datasets.valor_caption import VALORCaptionInstuctDataset, VALORCaptionEvalDataset, VALORCaptionDataset
+from lavis.datasets.datasets.vatex_captioning_datasets import VATEXCaptionInstuctDataset, VATEXCaptionEvalDataset, VATEXCaptionDataset
+from lavis.datasets.datasets.vlep_dataset import VlepVideoDataset, VlepVideoInstructDataset, VlepVideoEvalDataset
+from lavis.datasets.datasets.vsr_datasets import VSRCaptionDataset, VSRCaptionInstructDataset, VSRCaptionEvalDataset
+from lavis.datasets.datasets.textcaps_datasets import TextCapsCapDataset, TextCapsCapInstructDataset, TextCapsCapEvalDataset
 
 @registry.register_builder("coco_caption")
 class COCOCapBuilder(BaseDatasetBuilder):
     train_dataset_cls = COCOCapDataset
     eval_dataset_cls = COCOCapEvalDataset
 
     DATASET_CONFIG_DICT = {
         "default": "configs/datasets/coco/defaults_cap.yaml",
     }
 
+@registry.register_builder("coco_caption_instruct")
+class COCOCapInstructBuilder(BaseDatasetBuilder):
+    train_dataset_cls = COCOCapInstructDataset
+    eval_dataset_cls = COCOCapEvalDataset
+
+    DATASET_CONFIG_DICT = {
+        "default": "configs/datasets/coco/defaults_cap_instruct.yaml",
+    }
+
+
+@registry.register_builder("flickr30k_caption")
+class Flickr30kCapBuilder(BaseDatasetBuilder):
+    train_dataset_cls = COCOCapDataset
+    eval_dataset_cls = COCOCapEvalDataset
+    DATASET_CONFIG_DICT = {
+        "default": "configs/datasets/flickr30k/defaults_cap.yaml",
+    }
+
+@registry.register_builder("flickr30k_caption_instruct")
+class Flickr30kCapInstructBuilder(BaseDatasetBuilder):
+    train_dataset_cls = COCOCapInstructDataset
+    eval_dataset_cls = COCOCapEvalDataset
+    DATASET_CONFIG_DICT = {
+        "default": "configs/datasets/flickr30k/defaults_cap_instuct.yaml",
+    }
 
 @registry.register_builder("nocaps")
 class COCOCapBuilder(BaseDatasetBuilder):
     eval_dataset_cls = NoCapsEvalDataset
 
     DATASET_CONFIG_DICT = {
         "default": "configs/datasets/nocaps/defaults.yaml",
     }
 
+@registry.register_builder("vsr_caption")
+class VSRCapBuilder(BaseDatasetBuilder):
+    train_dataset_cls = VSRCaptionDataset
+    eval_dataset_cls = VSRCaptionEvalDataset
+
+    DATASET_CONFIG_DICT = {
+        "default": "configs/datasets/vsr/defaults.yaml",
+    }
+
+@registry.register_builder("vsr_caption_instruct")
+class VSRCapInstructBuilder(BaseDatasetBuilder):
+    train_dataset_cls = VSRCaptionInstructDataset
+    eval_dataset_cls = VSRCaptionEvalDataset
+
+    DATASET_CONFIG_DICT = {
+        "default": "configs/datasets/vsr/defaults.yaml",
+    }
+
+@registry.register_builder("textcaps_caption")
+class TextCapsCapBuilder(BaseDatasetBuilder):
+    train_dataset_cls = TextCapsCapDataset
+    eval_dataset_cls = TextCapsCapEvalDataset
+
+    DATASET_CONFIG_DICT = {
+        "default": "configs/datasets/textcaps/defaults.yaml",
+    }
+
+@registry.register_builder("textcaps_caption_instruct")
+class TextCapsCapInstructBuilder(BaseDatasetBuilder):
+    train_dataset_cls = TextCapsCapInstructDataset
+    eval_dataset_cls = TextCapsCapEvalDataset
+
+    DATASET_CONFIG_DICT = {
+        "default": "configs/datasets/textcaps/defaults_instruct.yaml",
+    }
+
+
+@registry.register_builder("capfilt14m")
+class CapFiltCapBuilder(BaseDatasetBuilder):
+    train_dataset_cls = CapFiltCaptionDataset
+
+    DATASET_CONFIG_DICT = {
+        "default": "configs/datasets/capfilt14m/defaults_cap.yaml",
+    }
+
+@registry.register_builder("capfilt14m_instruct")
+class CapFiltCapBuilder(BaseDatasetBuilder):
+    train_dataset_cls = CapFiltCaptionInstructDataset
+
+    DATASET_CONFIG_DICT = {
+        "default": "configs/datasets/capfilt14m/defaults_cap_instruct.yaml",
+    }
+
 
 @registry.register_builder("msrvtt_caption")
 class MSRVTTCapBuilder(BaseDatasetBuilder):
     train_dataset_cls = VideoCaptionDataset
     eval_dataset_cls = VideoCaptionEvalDataset
 
     DATASET_CONFIG_DICT = {
@@ -55,14 +150,172 @@
 
     DATASET_CONFIG_DICT = {
         "default": "configs/datasets/msvd/defaults_cap.yaml",
     }
 
 
 @registry.register_builder("vatex_caption")
-class VATEXCapBuilder(BaseDatasetBuilder):
-    train_dataset_cls = VideoCaptionDataset
-    eval_dataset_cls = VideoCaptionEvalDataset
+class VATEXCapBuilder(MultiModalDatasetBuilder):
+    train_dataset_cls = VATEXCaptionDataset
+    eval_dataset_cls = VATEXCaptionEvalDataset
 
     DATASET_CONFIG_DICT = {
         "default": "configs/datasets/vatex/defaults_cap.yaml",
     }
+
+@registry.register_builder("msrvtt_caption_instruct")
+class MSRVTTCapInstructBuilder(BaseDatasetBuilder):
+    train_dataset_cls = VideoCaptionInstructDataset
+    eval_dataset_cls = VideoCaptionEvalDataset
+
+    DATASET_CONFIG_DICT = {
+        "default": "configs/datasets/msrvtt/defaults_cap_instruct.yaml",
+    }
+
+@registry.register_builder("msvd_caption_instruct")
+class MSVDCapInstructBuilder(BaseDatasetBuilder):
+    train_dataset_cls = VideoCaptionInstructDataset
+    eval_dataset_cls = VideoCaptionEvalDataset
+
+
+    DATASET_CONFIG_DICT = {
+        "default": "configs/datasets/msvd/defaults_cap_instruct.yaml",
+    }
+
+
+@registry.register_builder("vatex_caption_instruct")
+class VATEXCapInstructBuilder(MultiModalDatasetBuilder):
+    train_dataset_cls = VATEXCaptionInstuctDataset
+    eval_dataset_cls = VATEXCaptionEvalDataset
+
+    DATASET_CONFIG_DICT = {
+        "default": "configs/datasets/vatex/defaults_cap_instruct.yaml",
+    }
+
+
+@registry.register_builder("webvid2m_caption")
+class WebVid2MCapBuilder(BaseDatasetBuilder):
+    train_dataset_cls = WebVideoCaptionDataset
+
+    DATASET_CONFIG_DICT = {
+        "default": "configs/datasets/webvid/defaults_cap.yaml",
+    }
+
+@registry.register_builder("webvid2m_caption_instruct")
+class WebVid2MCapInstructBuilder(BaseDatasetBuilder):
+    train_dataset_cls = WebVideoCaptionInstructDataset
+
+    DATASET_CONFIG_DICT = {
+        "default": "configs/datasets/webvid/defaults_cap_instruct.yaml",
+    }
+
+@registry.register_builder("violin_caption")
+class ViolinCapBuilder(BaseDatasetBuilder):
+    train_dataset_cls = ViolinVideoCaptionDataset
+    eval_dataset_cls = ViolinVideoCaptionEvalDataset
+
+    DATASET_CONFIG_DICT = {
+        "default": "configs/datasets/violin/defaults_cap.yaml",
+    }
+
+
+@registry.register_builder("violin_caption_instruct")
+class ViolinCapInstructBuilder(BaseDatasetBuilder):
+    train_dataset_cls = ViolinVideoCaptionInstructDataset
+    eval_dataset_cls = ViolinVideoCaptionEvalDataset
+
+    DATASET_CONFIG_DICT = {
+        "default": "configs/datasets/violin/defaults_cap_instruct.yaml",
+    }
+
+@registry.register_builder("valor_mm_caption")
+class VALORCaptionBuilder(MultiModalDatasetBuilder):
+    train_dataset_cls = VALORCaptionDataset
+    eval_dataset_cls = VALORCaptionEvalDataset
+
+    DATASET_CONFIG_DICT = {
+        "default": "configs/datasets/valor/defaults_mm_cap.yaml"
+    }
+
+@registry.register_builder("valor_mm_caption_instruct")
+class VALORCaptionInstructBuilder(MultiModalDatasetBuilder):
+    train_dataset_cls = VALORCaptionInstuctDataset
+    eval_dataset_cls = VALORCaptionEvalDataset
+
+    DATASET_CONFIG_DICT = {
+        "default": "configs/datasets/valor/defaults_mm_cap_instruct.yaml"
+    }
+
+@registry.register_builder("vlep_caption")
+class VlepCaptionBuilder(BaseDatasetBuilder):
+    train_dataset_cls = VlepVideoDataset
+    eval_dataset_cls = VlepVideoEvalDataset
+
+    DATASET_CONFIG_DICT = {
+        "default": "configs/datasets/vlep/defaults_cap.yaml"
+    }
+
+
+@registry.register_builder("vlep_caption_instruct")
+class VlepCaptionInstructBuilder(BaseDatasetBuilder):
+    train_dataset_cls = VlepVideoInstructDataset
+    eval_dataset_cls = VlepVideoEvalDataset
+
+    DATASET_CONFIG_DICT = {
+        "default": "configs/datasets/vlep/defaults_cap_instruct.yaml"
+    }
+
+@registry.register_builder("youcook_caption")
+class YouCookCaptionBuilder(BaseDatasetBuilder):
+    train_dataset_cls = ClipCaptionDataset
+    eval_dataset_cls = ClipCaptionEvalDataset
+
+    DATASET_CONFIG_DICT = {
+        "default": "configs/datasets/youcook/defaults_cap.yaml",
+    }
+
+@registry.register_builder("youcook_caption_instruct")
+class YouCookCaptionInstructBuilder(BaseDatasetBuilder):
+    train_dataset_cls = ClipCaptionInstructDataset
+    eval_dataset_cls = ClipCaptionEvalDataset
+
+    DATASET_CONFIG_DICT = {
+        "default": "configs/datasets/youcook/defaults_cap_instruct.yaml",
+    }
+
+@registry.register_builder("coin_caption")
+class COINCaptionBuilder(BaseDatasetBuilder):
+    train_dataset_cls = ClipCaptionDataset
+    eval_dataset_cls = ClipCaptionEvalDataset
+
+    DATASET_CONFIG_DICT = {
+        "default": "configs/datasets/coin/defaults_cap.yaml",
+    }
+
+
+@registry.register_builder("coin_caption_instruct")
+class COINCaptionInstructBuilder(BaseDatasetBuilder):
+    train_dataset_cls = ClipCaptionInstructDataset
+    eval_dataset_cls = ClipCaptionEvalDataset
+
+    DATASET_CONFIG_DICT = {
+        "default": "configs/datasets/coin/defaults_cap_instruct.yaml",
+    }
+
+
+@registry.register_builder("charade_caption")
+class CharadeCaptionBuilder(BaseDatasetBuilder):
+    train_dataset_cls = ClipCaptionDataset
+    eval_dataset_cls = ClipCaptionEvalDataset
+
+    DATASET_CONFIG_DICT = {
+        "default": "configs/datasets/charade/defaults_cap.yaml",
+    }
+
+@registry.register_builder("charade_caption_instruct")
+class CharadeCaptionInstructBuilder(BaseDatasetBuilder):
+    train_dataset_cls = ClipCaptionInstructDataset
+    eval_dataset_cls = ClipCaptionEvalDataset
+
+    DATASET_CONFIG_DICT = {
+        "default": "configs/datasets/charade/defaults_cap_instruct.yaml",
+    }
```

## lavis/datasets/builders/classification_builder.py

```diff
@@ -2,18 +2,38 @@
  Copyright (c) 2022, salesforce.com, inc.
  All rights reserved.
  SPDX-License-Identifier: BSD-3-Clause
  For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 """
 
 from lavis.common.registry import registry
-from lavis.datasets.builders.base_dataset_builder import BaseDatasetBuilder
+from lavis.datasets.builders.base_dataset_builder import BaseDatasetBuilder, MultiModalDatasetBuilder
 from lavis.datasets.datasets.nlvr_datasets import NLVRDataset, NLVREvalDataset
-from lavis.datasets.datasets.snli_ve_datasets import SNLIVisualEntialmentDataset
-
+from lavis.datasets.datasets.snli_ve_datasets import SNLIVisualEntialmentDataset, SNLIVisualEntialmentInstructDataset
+from lavis.datasets.datasets.violin_dataset import ViolinVideoEntailmentDataset, ViolinVideoEntailmentInstructDataset
+from lavis.datasets.datasets.vsr_datasets import VSRClassificationDataset, VSRClassificationInstructDataset
+from lavis.datasets.datasets.audio_classification_datasets import ESC50
+@registry.register_builder("violin_entailment")
+class ViolinEntailmentBuilder(BaseDatasetBuilder):
+    train_dataset_cls = ViolinVideoEntailmentDataset
+    eval_dataset_cls = ViolinVideoEntailmentDataset
+
+    DATASET_CONFIG_DICT = {
+        "default": "configs/datasets/violin/defaults_entail.yaml",
+    }
+
+
+@registry.register_builder("violin_entailment_instruct")
+class ViolinEntailmentInstructBuilder(BaseDatasetBuilder):
+    train_dataset_cls = ViolinVideoEntailmentInstructDataset
+    eval_dataset_cls = ViolinVideoEntailmentInstructDataset
+
+    DATASET_CONFIG_DICT = {
+        "default": "configs/datasets/violin/defaults_entail_instruct.yaml",
+    }
 
 @registry.register_builder("nlvr")
 class NLVRBuilder(BaseDatasetBuilder):
     train_dataset_cls = NLVRDataset
     eval_dataset_cls = NLVREvalDataset
 
     DATASET_CONFIG_DICT = {"default": "configs/datasets/nlvr/defaults.yaml"}
@@ -21,7 +41,35 @@
 
 @registry.register_builder("snli_ve")
 class SNLIVisualEntailmentBuilder(BaseDatasetBuilder):
     train_dataset_cls = SNLIVisualEntialmentDataset
     eval_dataset_cls = SNLIVisualEntialmentDataset
 
     DATASET_CONFIG_DICT = {"default": "configs/datasets/snli_ve/defaults.yaml"}
+
+@registry.register_builder("snli_ve_instruct")
+class SNLIVisualEntailmentInstructBuilder(BaseDatasetBuilder):
+    train_dataset_cls = SNLIVisualEntialmentInstructDataset
+    eval_dataset_cls = SNLIVisualEntialmentInstructDataset
+
+    DATASET_CONFIG_DICT = {"default": "configs/datasets/snli_ve/defaults_instruct.yaml"}
+
+
+@registry.register_builder("vsr_classification")
+class VSRClassificationBuilder(BaseDatasetBuilder):
+    train_dataset_cls = VSRClassificationDataset
+    eval_dataset_cls = VSRClassificationDataset
+
+    DATASET_CONFIG_DICT = {"default": "configs/datasets/vsr/defaults_classification.yaml"}
+
+@registry.register_builder("vsr_classification_instruct")
+class SNLIVisualEntailmentInstructBuilder(BaseDatasetBuilder):
+    train_dataset_cls = VSRClassificationInstructDataset
+    eval_dataset_cls = VSRClassificationInstructDataset
+
+    DATASET_CONFIG_DICT = {"default": "configs/datasets/vsr/defaults_classification_instruct.yaml"}
+
+@registry.register_builder("esc50_cls")
+class ESC50ClassificationBuilder(MultiModalDatasetBuilder):
+    eval_dataset_cls = ESC50
+
+    DATASET_CONFIG_DICT = {"default": "configs/datasets/esc50/defaults_mm_cls.yaml"}
```

## lavis/datasets/builders/dialogue_builder.py

```diff
@@ -2,20 +2,65 @@
  Copyright (c) 2022, salesforce.com, inc.
  All rights reserved.
  SPDX-License-Identifier: BSD-3-Clause
  For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 """
 
 from lavis.common.registry import registry
-from lavis.datasets.builders.base_dataset_builder import BaseDatasetBuilder
+from lavis.datasets.builders.base_dataset_builder import BaseDatasetBuilder, MultiModalDatasetBuilder
 from lavis.datasets.datasets.avsd_dialogue_datasets import (
     AVSDDialDataset,
     AVSDDialEvalDataset,
+    AVSDDialInstructEvalDataset
 )
+from lavis.datasets.datasets.visdial_dialogue_datasets import (
+    VisDialDataset,
+    VisDialInstructDataset,
+    VisDialEvalDataset,
+)
+
+from lavis.datasets.datasets.yt8m_video_dialogue_datasets import YT8MDialDataset
+from lavis.datasets.datasets.llava150k_dataset import LLaVA150kInstructDataset
 
 
 @registry.register_builder("avsd_dialogue")
 class AVSDDialBuilder(BaseDatasetBuilder):
     train_dataset_cls = AVSDDialDataset
     eval_dataset_cls = AVSDDialEvalDataset
 
     DATASET_CONFIG_DICT = {"default": "configs/datasets/avsd/defaults_dial.yaml"}
+
+@registry.register_builder("visdial")
+class VisDialBuilder(BaseDatasetBuilder):
+    train_dataset_cls = VisDialDataset
+    eval_dataset_cls = VisDialEvalDataset
+
+    DATASET_CONFIG_DICT = {"default": "configs/datasets/visdial/defaults_dial.yaml"}
+
+@registry.register_builder("visdial_instruct")
+class VisDialInstructBuilder(BaseDatasetBuilder):
+    train_dataset_cls = VisDialInstructDataset
+    eval_dataset_cls = VisDialEvalDataset
+
+    DATASET_CONFIG_DICT = {"default": "configs/datasets/visdial/defaults_dial_instruct.yaml"}
+
+@registry.register_builder("avsd_mm_dialogue_instruct")
+class AVSDDialInstructBuilder(MultiModalDatasetBuilder):
+    train_dataset_cls = AVSDDialInstructEvalDataset
+    eval_dataset_cls = AVSDDialInstructEvalDataset
+
+    DATASET_CONFIG_DICT = {"default": "configs/datasets/avsd/defaults_mm_dial_instruct.yaml"}
+
+@registry.register_builder("llava150k_dialogue_instruct")
+class LLaVA150kDialInstructBuilder(BaseDatasetBuilder):
+    train_dataset_cls = LLaVA150kInstructDataset
+    eval_dataset_cls = LLaVA150kInstructDataset
+
+    DATASET_CONFIG_DICT = {"default": "configs/datasets/llava150k/defaults_dial.yaml"}
+
+@registry.register_builder("yt8m_mm_dialogue")
+class YT8MDialBuilder(MultiModalDatasetBuilder):
+    train_dataset_cls = YT8MDialDataset
+    eval_dataset_cls = YT8MDialDataset
+
+    DATASET_CONFIG_DICT = {"default": "configs/datasets/yt8m/defaults_mm_dial.yaml"}
+
```

## lavis/datasets/builders/image_text_pair_builder.py

```diff
@@ -5,50 +5,79 @@
  For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 """
 
 import os
 from lavis.common.registry import registry
 
 from lavis.datasets.builders.base_dataset_builder import BaseDatasetBuilder
-from lavis.datasets.datasets.image_text_pair_datasets import ImageTextPairDataset
-from lavis.datasets.datasets.laion_dataset import LaionDataset
-
+from lavis.datasets.datasets.image_text_pair_datasets import ImageTextPairDataset, ImageTextPairInstructDataset
+from lavis.datasets.datasets.laion_dataset import LaionDataset, LaionInstructDataset
 
 @registry.register_builder("conceptual_caption_3m")
 class ConceptualCaption3MBuilder(BaseDatasetBuilder):
     train_dataset_cls = ImageTextPairDataset
 
     DATASET_CONFIG_DICT = {
         "default": "configs/datasets/conceptual_caption/defaults_3m.yaml"
     }
 
+@registry.register_builder("conceptual_caption_3m_instruct")
+class ConceptualCaption3MInstructBuilder(BaseDatasetBuilder):
+    train_dataset_cls = ImageTextPairInstructDataset
+
+    DATASET_CONFIG_DICT = {
+        "default": "configs/datasets/conceptual_caption/defaults_3m_instruct.yaml"
+    }
+
 
 @registry.register_builder("conceptual_caption_12m")
 class ConceptualCaption12MBuilder(BaseDatasetBuilder):
     train_dataset_cls = ImageTextPairDataset
 
     DATASET_CONFIG_DICT = {
         "default": "configs/datasets/conceptual_caption/defaults_12m.yaml"
     }
 
+@registry.register_builder("conceptual_caption_12m_instruct")
+class ConceptualCaption12MInstructBuilder(BaseDatasetBuilder):
+    train_dataset_cls = ImageTextPairInstructDataset
+
+    DATASET_CONFIG_DICT = {
+        "default": "configs/datasets/conceptual_caption/defaults_12m_instruct.yaml"
+    }
 
 @registry.register_builder("sbu_caption")
 class SBUCaptionBuilder(BaseDatasetBuilder):
     train_dataset_cls = ImageTextPairDataset
 
     DATASET_CONFIG_DICT = {"default": "configs/datasets/sbu_caption/defaults.yaml"}
 
 
+@registry.register_builder("sbu_caption_instruct")
+class SBUCaptionInstructBuilder(BaseDatasetBuilder):
+    train_dataset_cls = ImageTextPairInstructDataset
+
+    DATASET_CONFIG_DICT = {"default": "configs/datasets/sbu_caption/defaults_instruct.yaml"}
+
+
 @registry.register_builder("vg_caption")
 class VGCaptionBuilder(BaseDatasetBuilder):
     train_dataset_cls = ImageTextPairDataset
 
     DATASET_CONFIG_DICT = {"default": "configs/datasets/vg/defaults_caption.yaml"}
 
 
+@registry.register_builder("vg_caption_instruct")
+class VGCaptionInstructBuilder(BaseDatasetBuilder):
+    train_dataset_cls = ImageTextPairInstructDataset
+
+    DATASET_CONFIG_DICT = {"default": "configs/datasets/vg/defaults_caption_instruct.yaml"}
+
+
+
 @registry.register_builder("laion2B_multi")
 class Laion2BMultiBuilder(BaseDatasetBuilder):
     train_dataset_cls = LaionDataset
 
     DATASET_CONFIG_DICT = {"default": "configs/datasets/laion/defaults_2B_multi.yaml"}
 
     def _download_ann(self):
@@ -71,7 +100,21 @@
         datasets[split] = dataset_cls(
             vis_processor=self.vis_processors[split],
             text_processor=self.text_processors[split],
             location=build_info.storage,
         ).inner_dataset
 
         return datasets
+
+@registry.register_builder("laion400M")
+class Laion400MBuilder(Laion2BMultiBuilder):
+    train_dataset_cls = LaionDataset
+
+    DATASET_CONFIG_DICT = {"default": "configs/datasets/laion/defaults_400M.yaml"}
+
+
+@registry.register_builder("laion400M_instruct")
+class Laion400MInstructBuilder(Laion2BMultiBuilder):
+    train_dataset_cls = LaionInstructDataset
+
+    DATASET_CONFIG_DICT = {"default": "configs/datasets/laion/defaults_400M_instruct.yaml"}
+
```

## lavis/datasets/builders/video_qa_builder.py

```diff
@@ -3,16 +3,17 @@
  All rights reserved.
  SPDX-License-Identifier: BSD-3-Clause
  For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 """
 
 from lavis.common.registry import registry
 from lavis.common.utils import get_cache_path
-from lavis.datasets.builders.base_dataset_builder import BaseDatasetBuilder
-from lavis.datasets.datasets.video_vqa_datasets import VideoQADataset
+from lavis.datasets.builders.base_dataset_builder import BaseDatasetBuilder, MultiModalDatasetBuilder
+from lavis.datasets.datasets.video_vqa_datasets import VideoQADataset, VideoQAInstructDataset
+from lavis.datasets.datasets.music_avqa import MusicAVQAInstructDataset, MusicAVQADataset
 
 
 class VideoQABuilder(BaseDatasetBuilder):
     train_dataset_cls = VideoQADataset
     eval_dataset_cls = VideoQADataset
 
     def build(self):
@@ -38,7 +39,39 @@
 
 
 @registry.register_builder("msvd_qa")
 class MSVDQABuilder(VideoQABuilder):
     DATASET_CONFIG_DICT = {
         "default": "configs/datasets/msvd/defaults_qa.yaml",
     }
+
+
+@registry.register_builder("msrvtt_qa_instruct")
+class MSRVTTQAInstructBuilder(VideoQABuilder):
+    train_dataset_cls = VideoQAInstructDataset
+    eval_dataset_cls = VideoQAInstructDataset
+    DATASET_CONFIG_DICT = {
+        "default": "configs/datasets/msrvtt/defaults_qa_instruct.yaml",
+    }
+
+
+@registry.register_builder("msvd_qa_instruct")
+class MSVDQAInstructBuilder(VideoQABuilder):
+    train_dataset_cls = VideoQAInstructDataset
+    eval_dataset_cls = VideoQAInstructDataset
+    DATASET_CONFIG_DICT = {
+        "default": "configs/datasets/msvd/defaults_qa_instruct.yaml",
+    }
+
+@registry.register_builder("musicavqa_mm")
+class MusicAVQABuilder(MultiModalDatasetBuilder):
+    train_dataset_cls = MusicAVQADataset
+    eval_dataset_cls = MusicAVQADataset
+
+    DATASET_CONFIG_DICT = {"default": "configs/datasets/music_avqa/defaults_mm_qa.yaml"}
+
+@registry.register_builder("musicavqa_mm_instruct")
+class MusicAVQAInstructBuilder(MultiModalDatasetBuilder):
+    train_dataset_cls = MusicAVQAInstructDataset
+    eval_dataset_cls = MusicAVQAInstructDataset
+
+    DATASET_CONFIG_DICT = {"default": "configs/datasets/music_avqa/defaults_mm_qa_instruct.yaml"}
```

## lavis/datasets/builders/vqa_builder.py

```diff
@@ -4,55 +4,149 @@
  SPDX-License-Identifier: BSD-3-Clause
  For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 """
 
 from lavis.datasets.builders.base_dataset_builder import BaseDatasetBuilder
 
 from lavis.common.registry import registry
-from lavis.datasets.datasets.aok_vqa_datasets import AOKVQADataset, AOKVQAEvalDataset
-from lavis.datasets.datasets.coco_vqa_datasets import COCOVQADataset, COCOVQAEvalDataset
-from lavis.datasets.datasets.vg_vqa_datasets import VGVQADataset
-from lavis.datasets.datasets.gqa_datasets import GQADataset, GQAEvalDataset
-
+from lavis.datasets.datasets.aok_vqa_datasets import AOKVQADataset, AOKVQAEvalDataset, AOKVQAInstructDataset
+from lavis.datasets.datasets.coco_vqa_datasets import COCOVQADataset, COCOVQAEvalDataset, COCOVQAInstructDataset
+from lavis.datasets.datasets.vg_vqa_datasets import VGVQADataset, VGVQAInstructDataset
+from lavis.datasets.datasets.gqa_datasets import GQADataset, GQAEvalDataset, GQAInstructDataset
+from lavis.datasets.datasets.iconqa_datasets import IconQADataset, IconQAEvalDataset, IconQAInstructDataset
+from lavis.datasets.datasets.ocr_datasets import OCRVQADataset, OCRVQAInstructDataset
+from lavis.datasets.datasets.vizwiz_vqa_datasets import VizWizEvalDataset
 
 @registry.register_builder("coco_vqa")
 class COCOVQABuilder(BaseDatasetBuilder):
     train_dataset_cls = COCOVQADataset
     eval_dataset_cls = COCOVQAEvalDataset
 
     DATASET_CONFIG_DICT = {
         "default": "configs/datasets/coco/defaults_vqa.yaml",
         "eval": "configs/datasets/coco/eval_vqa.yaml",
     }
 
+@registry.register_builder("coco_vqa_instruct")
+class COCOVQAInstructBuilder(BaseDatasetBuilder):
+    train_dataset_cls = COCOVQAInstructDataset
+    eval_dataset_cls = COCOVQAEvalDataset
+
+    DATASET_CONFIG_DICT = {
+        "default": "configs/datasets/coco/defaults_vqa_instruct.yaml",
+        "eval": "configs/datasets/coco/eval_vqa.yaml",
+    }
 
 @registry.register_builder("vg_vqa")
 class VGVQABuilder(BaseDatasetBuilder):
     train_dataset_cls = VGVQADataset
     DATASET_CONFIG_DICT = {"default": "configs/datasets/vg/defaults_vqa.yaml"}
 
+@registry.register_builder("vg_vqa_instruct")
+class VGVQAInstructBuilder(BaseDatasetBuilder):
+    train_dataset_cls = VGVQAInstructDataset
+    DATASET_CONFIG_DICT = {"default": "configs/datasets/vg/defaults_vqa_instruct.yaml"}
 
 @registry.register_builder("ok_vqa")
 class OKVQABuilder(COCOVQABuilder):
     DATASET_CONFIG_DICT = {
         "default": "configs/datasets/okvqa/defaults.yaml",
     }
 
+@registry.register_builder("ok_vqa_instruct")
+class OKVQAInstructBuilder(COCOVQAInstructBuilder):
+    DATASET_CONFIG_DICT = {
+        "default": "configs/datasets/okvqa/defaults_instruct.yaml",
+    }
 
 @registry.register_builder("aok_vqa")
 class AOKVQABuilder(BaseDatasetBuilder):
     train_dataset_cls = AOKVQADataset
     eval_dataset_cls = AOKVQAEvalDataset
 
     DATASET_CONFIG_DICT = {"default": "configs/datasets/aokvqa/defaults.yaml"}
 
+@registry.register_builder("aok_vqa_instruct")
+class AOKVQAInstructBuilder(BaseDatasetBuilder):
+    train_dataset_cls = AOKVQAInstructDataset
+    eval_dataset_cls = AOKVQAEvalDataset
+
+    DATASET_CONFIG_DICT = {"default": "configs/datasets/aokvqa/defaults_instruct.yaml"}
+
 
 @registry.register_builder("gqa")
 class GQABuilder(BaseDatasetBuilder):
     train_dataset_cls = GQADataset
     eval_dataset_cls = GQAEvalDataset
 
     DATASET_CONFIG_DICT = {
         "default": "configs/datasets/gqa/defaults.yaml",
         "balanced_val": "configs/datasets/gqa/balanced_val.yaml",
         "balanced_testdev": "configs/datasets/gqa/balanced_testdev.yaml",
-    }
+    }
+
+@registry.register_builder("gqa_instruct")
+class GQAInstructBuilder(BaseDatasetBuilder):
+    train_dataset_cls = GQAInstructDataset
+    eval_dataset_cls = GQAEvalDataset
+
+    DATASET_CONFIG_DICT = {
+        "default": "configs/datasets/gqa/defaults_instruct.yaml",
+        "balanced_val": "configs/datasets/gqa/balanced_val_instruct.yaml",
+        "balanced_testdev": "configs/datasets/gqa/balanced_testdev_instruct.yaml",
+    }
+
+@registry.register_builder("iconqa")
+class IconQABuilder(BaseDatasetBuilder):
+    train_dataset_cls = IconQADataset
+    eval_dataset_cls = IconQAEvalDataset
+
+    DATASET_CONFIG_DICT = {
+        "default": "configs/datasets/iconqa/defaults.yaml",
+    }
+
+@registry.register_builder("iconqa_instruct")
+class IconQAInstructBuilder(BaseDatasetBuilder):
+    train_dataset_cls = IconQAInstructDataset
+    eval_dataset_cls = IconQAEvalDataset
+
+    DATASET_CONFIG_DICT = {
+        "default": "configs/datasets/iconqa/defaults_instruct.yaml",
+    }
+
+@registry.register_builder("scienceqa")
+class ScienceQABuilder(BaseDatasetBuilder):
+    train_dataset_cls = IconQADataset
+    eval_dataset_cls = IconQAEvalDataset
+
+    DATASET_CONFIG_DICT = {"default": "configs/datasets/scienceqa/defaults.yaml"}
+
+@registry.register_builder("scienceqa_instruct")
+class ScienceQAInstructBuilder(BaseDatasetBuilder):
+    train_dataset_cls = IconQAInstructDataset
+    eval_dataset_cls = IconQAEvalDataset
+
+    DATASET_CONFIG_DICT = {"default": "configs/datasets/scienceqa/defaults_instruct.yaml"}
+
+@registry.register_builder("ocr_vqa")
+class OCRVQABuilder(BaseDatasetBuilder):
+    train_dataset_cls = OCRVQADataset
+    eval_dataset_cls = OCRVQADataset
+
+    DATASET_CONFIG_DICT = {"default": "configs/datasets/ocrvqa/defaults.yaml"}
+
+@registry.register_builder("ocr_vqa_instruct")
+class OCRVQAInstructBuilder(BaseDatasetBuilder):
+    train_dataset_cls = OCRVQAInstructDataset
+    eval_dataset_cls = OCRVQAInstructDataset
+
+    DATASET_CONFIG_DICT = {"default": "configs/datasets/ocrvqa/defaults_instruct.yaml"}
+
+
+@registry.register_builder("vizwiz_vqa")
+class VizWizVQABuilder(BaseDatasetBuilder):
+    eval_dataset_cls = VizWizEvalDataset
+
+    DATASET_CONFIG_DICT = {"default": "configs/datasets/vizwiz/defaults.yaml"}
+
+
+
```

## lavis/datasets/datasets/aok_vqa_datasets.py

```diff
@@ -5,14 +5,15 @@
  For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 """
 
 from collections import OrderedDict
 import json
 import os
 import torch
+import random
 
 from PIL import Image
 
 from lavis.datasets.datasets.vqa_datasets import VQADataset, VQAEvalDataset
 
 
 class __DisplMixin:
@@ -59,14 +60,26 @@
         return {
             "image": image,
             "text_input": question,
             "answers": answers,
             "weights": weights,
         }
 
+class AOKVQAInstructDataset(AOKVQADataset):
+    def __getitem__(self, index):
+        data = super().__getitem__(index)
+        if data != None:
+            data["text_output"] = random.choice(data['answers'])
+        return data
+
+    def collater(self, samples):
+        data = super().collater(samples)
+        data['text_output'] = data['answer']
+        return data
+
 
 class AOKVQAEvalDataset(VQAEvalDataset, __DisplMixin):
     def __init__(self, vis_processor, text_processor, vis_root, ann_paths):
         """
         vis_root (string): Root directory of images (e.g. coco/images/)
         ann_root (string): directory to store the annotation file
         """
@@ -147,8 +160,8 @@
             "image": image,
             "text_input": question,
             "question_id": ann["question_id"],
             "instance_id": ann["instance_id"],
             "choices": choices,
             "correct_choice_idx": correct_choice_idx,
             "direct_answers": direct_answers,
-        }
+        }
```

## lavis/datasets/datasets/avsd_dialogue_datasets.py

```diff
@@ -2,14 +2,18 @@
  Copyright (c) 2022, salesforce.com, inc.
  All rights reserved.
  SPDX-License-Identifier: BSD-3-Clause
  For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 """
 
 import torch
+import os
+import copy
+import random
+from PIL import Image
 from lavis.datasets.datasets.dialogue_datasets import (
     DialogueDataset,
     DialogueEvalDataset,
 )
 
 
 class AVSDDialDataset(DialogueDataset):
@@ -160,7 +164,64 @@
         samples["input_ids"] = input_ids
         samples["token_type_ids"] = token_type_ids
         samples["labels"] = labels
         samples["video_fts"] = video_fts
         samples["attn_mask"] = attn_mask
 
         return samples
+
+
+class AVSDDialInstructEvalDataset(DialogueDataset):
+    def __init__(self, **kwargs):
+        super().__init__(kwargs['vis_processor'], kwargs['text_processor'], kwargs['vis_root'], kwargs['ann_paths'])
+
+        self.modalities = kwargs['modalities']
+
+        for modality in self.modalities:
+            if 'image' in modality:
+                setattr(self, f"existing_{modality}_annotation",getattr(self, f'get_existing_{modality}_annotations')())
+                continue
+            setattr(self, f"{modality}_root", kwargs[f"{modality}_root"])
+            setattr(self, f"{modality}_processor", kwargs[f"{modality}_processor"])
+            setattr(self, f"existing_{modality}_annotation",getattr(self, f'get_existing_{modality}_annotations')())
+        self.sample_ids = set.intersection(*[set(getattr(self, f"existing_{modality}_annotation")) for modality in self.modalities])
+        self.annotation = [ann for ann in self.annotation if ann['image_id'] in self.sample_ids]
+        if 'test' in kwargs['ann_paths'][0]:
+             self.annotation = [ann for ann in self.annotation if ann['answer'] == '__UNDISCLOSED__']
+    
+    def get_existing_audio_annotations(self):
+        return [f.split('.')[0] for f in os.listdir(self.audio_root)]
+    
+    def get_existing_video_annotations(self):
+        return [f.split('.')[0] for f in os.listdir(self.video_root)]
+    
+    def get_audio_path(self, sample_key):
+        return os.path.join(self.audio_root, sample_key) + '.mp4'
+    
+    def get_video_path(self, sample_key):
+        return os.path.join(self.video_root, sample_key) + '.mp4'
+
+    def __getitem__(self, index):
+        ann = copy.deepcopy(self.annotation[index])
+        for modality in self.modalities:
+            ann[f"{modality}_path"] = getattr(self, f"get_{modality}_path")(ann['image_id'])
+            
+            if type(ann[f"{modality}_path"]) == list:
+                ann[f"{modality}_path"] = random.choice(ann[f"{modality}_path"])
+            if 'image' in modality:
+                ann['image'] = self.vis_processor(Image.open(ann[f"images_path"]))
+            else:
+                ann[modality] = getattr(self, f"{modality}_processor")(ann[f"{modality}_path"]).to(torch.float32)
+        
+        ann["sample_id"] = ann["image_id"]
+        dialog = ""
+        for t in ann['dialog']:
+            dialog += f"{t['question']} {t['answer']} "
+        ann['dialog'] = dialog
+        ann['text_output'] = self.text_processor(ann['answer'])
+        ann['text_input'] =  self.text_processor(ann['question'])
+        ann["question_id"] = index
+        # ann['captions'] = ann[ann['answer']] # commented out for test dataset
+        return ann
+    
+    def __len__(self):
+        return len(self.annotation)
```

## lavis/datasets/datasets/base_dataset.py

```diff
@@ -3,53 +3,80 @@
  All rights reserved.
  SPDX-License-Identifier: BSD-3-Clause
  For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 """
 
 import json
 from typing import Iterable
+import pandas as pd
+import torch
 
 from torch.utils.data import Dataset, ConcatDataset
 from torch.utils.data.dataloader import default_collate
 
 
 class BaseDataset(Dataset):
     def __init__(
         self, vis_processor=None, text_processor=None, vis_root=None, ann_paths=[]
     ):
         """
         vis_root (string): Root directory of images (e.g. coco/images/)
         ann_root (string): directory to store the annotation file
         """
         self.vis_root = vis_root
-
         self.annotation = []
         for ann_path in ann_paths:
-            self.annotation.extend(json.load(open(ann_path, "r")))
+            if any(ext in ann_path for ext in ['csv', 'tsv']):
+                df = pd.read_csv(ann_path)
+                self.annotation.extend(df.to_dict(orient="records"))
+                
+            elif 'jsonl' in ann_path:
+                with open(ann_path, "r") as f:
+                    self.annotation.extend([json.loads(line) for line in f])
+
+            else:
+                with open(ann_path, "r") as f:
+                    loaded = json.load(f)
+                    if isinstance(loaded, list):
+                        self.annotation.extend(loaded)
+                    elif isinstance(loaded, dict):
+                       self.annotation.extend([{"sample_id": k, **v} if isinstance(v, dict) else {"sample_id": k, "data": v} for k, v in loaded.items()])
+
 
         self.vis_processor = vis_processor
         self.text_processor = text_processor
 
         self._add_instance_ids()
 
     def __len__(self):
         return len(self.annotation)
 
     def collater(self, samples):
-        return default_collate(samples)
+        # Filter out None samples
+        samples = [s for s in samples if s is not None]
+        # Check if samples is empty after filtering
+        if not samples:
+            return {}
+        collated_dict = {}
+        keys = samples[0].keys() # Use the keys of the first sample as a reference
+        for k in keys:
+            values = [sample[k] for sample in samples]
+            # If the value type for the key is torch.Tensor, stack them else return list
+            collated_dict[k] = torch.stack(values, dim=0) if isinstance(values[0], torch.Tensor) else values
+        return collated_dict
+        # return default_collate(samples)
 
     def set_processors(self, vis_processor, text_processor):
         self.vis_processor = vis_processor
         self.text_processor = text_processor
 
     def _add_instance_ids(self, key="instance_id"):
         for idx, ann in enumerate(self.annotation):
             ann[key] = str(idx)
 
-
 class ConcatDataset(ConcatDataset):
     def __init__(self, datasets: Iterable[Dataset]) -> None:
         super().__init__(datasets)
 
     def collater(self, samples):
         # TODO For now only supports datasets with same underlying collater implementations
```

## lavis/datasets/datasets/caption_datasets.py

```diff
@@ -43,26 +43,28 @@
 
     def __getitem__(self, index):
 
         # TODO this assumes image input, not general enough
         ann = self.annotation[index]
 
         image_path = os.path.join(self.vis_root, ann["image"])
-        image = Image.open(image_path).convert("RGB")
+        try:
+            image = Image.open(image_path).convert("RGB")
+        except:
+            return None # image does not exist
 
         image = self.vis_processor(image)
         caption = self.text_processor(ann["caption"])
 
         return {
             "image": image,
             "text_input": caption,
-            "image_id": self.img_ids[ann["image_id"]],
+            "image_id": ann["image_id"]
         }
 
-
 class CaptionEvalDataset(BaseDataset, __DisplMixin):
     def __init__(self, vis_processor, text_processor, vis_root, ann_paths):
         """
         vis_root (string): Root directory of images (e.g. coco/images/)
         ann_root (string): directory to store the annotation file
         split (string): val or test
         """
@@ -78,7 +80,15 @@
         image = self.vis_processor(image)
 
         return {
             "image": image,
             "image_id": ann["image_id"],
             "instance_id": ann["instance_id"],
         }
+
+class CaptionInstructDataset(CaptionDataset):
+    def __getitem__(self, index):
+        data = super().__getitem__(index)
+        if data != None:
+            data['text_output'] = data["text_input"]
+            data['text_input'] = self.text_processor("")
+        return data
```

## lavis/datasets/datasets/coco_caption_datasets.py

```diff
@@ -9,17 +9,18 @@
 import json
 
 from PIL import Image
 from PIL import ImageFile
 
 ImageFile.LOAD_TRUNCATED_IMAGES = True
 
-from lavis.datasets.datasets.caption_datasets import CaptionDataset, CaptionEvalDataset
+from lavis.datasets.datasets.caption_datasets import CaptionDataset, CaptionInstructDataset, CaptionEvalDataset
 
 COCOCapDataset = CaptionDataset
+COCOCapInstructDataset = CaptionInstructDataset
 
 
 class COCOCapEvalDataset(CaptionEvalDataset):
     def __init__(self, vis_processor, text_processor, vis_root, ann_paths):
         """
         vis_root (string): Root directory of images (e.g. coco/images/)
         ann_root (string): directory to store the annotation file
@@ -40,14 +41,15 @@
         return {
             "image": image,
             "image_id": img_id,
             "instance_id": ann["instance_id"],
         }
 
 
+
 class NoCapsEvalDataset(CaptionEvalDataset):
     def __init__(self, vis_processor, text_processor, vis_root, ann_paths):
         """
         vis_root (string): Root directory of images (e.g. coco/images/)
         ann_root (string): directory to store the annotation file
         split (string): val or test
         """
@@ -63,8 +65,8 @@
 
         img_id = ann["img_id"]
 
         return {
             "image": image,
             "image_id": img_id,
             "instance_id": ann["instance_id"],
-        }
+        }
```

## lavis/datasets/datasets/coco_vqa_datasets.py

```diff
@@ -3,15 +3,15 @@
  All rights reserved.
  SPDX-License-Identifier: BSD-3-Clause
  For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 """
 
 import os
 import json
-
+import random
 from PIL import Image
 
 from lavis.datasets.datasets.vqa_datasets import VQADataset, VQAEvalDataset
 
 from collections import OrderedDict
 
 
@@ -57,14 +57,28 @@
             "image": image,
             "text_input": question,
             "answers": answers,
             "weights": weights,
         }
 
 
+class COCOVQAInstructDataset(COCOVQADataset):
+    def __getitem__(self, index):
+        data = super().__getitem__(index)
+        if data != None:
+            data['text_output'] = random.choice(data["answers"])
+        return data
+
+    def collater(self, samples):
+        data = super().collater(samples)
+        data['text_output'] = data['answer']
+        return data
+
+    
+
 class COCOVQAEvalDataset(VQAEvalDataset, __DisplMixin):
     def __init__(self, vis_processor, text_processor, vis_root, ann_paths):
         """
         vis_root (string): Root directory of images (e.g. coco/images/)
         ann_root (string): directory to store the annotation file
         """
```

## lavis/datasets/datasets/dataloader_utils.py

```diff
@@ -23,15 +23,14 @@
 
     def __init__(self, loaders, ratios=None):
         # assert all loaders has __next__ method
         for loader in loaders:
             assert hasattr(
                 loader, "__next__"
             ), "Loader {} has no __next__ method.".format(loader)
-
         if ratios is None:
             ratios = [1.0] * len(loaders)
         else:
             assert len(ratios) == len(loaders)
             ratios = [float(ratio) / sum(ratios) for ratio in ratios]
 
         self.loaders = loaders
@@ -97,18 +96,21 @@
             # self.next_target_gpu.copy_(self.next_target, non_blocking=True)
             # self.next_input = self.next_input_gpu
             # self.next_target = self.next_target_gpu
 
     def next(self, it):
         torch.cuda.current_stream().wait_stream(self.stream)
         batch = self.batch
-        if batch is not None:
+        if batch is not None and batch is not {}:
             record_cuda_stream(batch)
         self.preload(it)
         return batch
+    
+    def __next__(self, it):
+        return self.next(it)
 
     def __getattr__(self, name):
         method = self.loader.__getattribute__(name)
         return method
 
 
 def record_cuda_stream(batch):
```

## lavis/datasets/datasets/gqa_datasets.py

```diff
@@ -3,14 +3,15 @@
  All rights reserved.
  SPDX-License-Identifier: BSD-3-Clause
  For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 """
 
 import os
 import json
+import random
 
 from PIL import Image
 
 from lavis.datasets.datasets.vqa_datasets import VQADataset, VQAEvalDataset
 
 from collections import OrderedDict
 
@@ -49,14 +50,26 @@
         return {
             "image": image,
             "text_input": question,
             "answers": answers,
             "weights": weights,
         }
 
+class GQAInstructDataset(GQADataset):
+    def __getitem__(self, index):
+        data = super().__getitem__(index)
+        if data != None:
+            data['text_output'] = random.choice(data["answers"])
+        return data
+
+    def collater(self, samples):
+        data = super().collater(samples)
+        data['text_output'] = data['answer']
+        return data
+
 
 class GQAEvalDataset(VQAEvalDataset, __DisplMixin):
     def __init__(self, vis_processor, text_processor, vis_root, ann_paths):
         """
         vis_root (string): Root directory of images (e.g. gqa/images/)
         ann_root (string): directory to store the annotation file
         """
```

## lavis/datasets/datasets/image_text_pair_datasets.py

```diff
@@ -35,13 +35,24 @@
 
     def __getitem__(self, index):
 
         # TODO this assumes image input, not general enough
         ann = self.annotation[index]
 
         image_path = os.path.join(self.vis_root, ann["image"])
-        image = Image.open(image_path).convert("RGB")
+        try:
+            image = Image.open(image_path).convert("RGB")
+        except:
+            return None
 
         image = self.vis_processor(image)
         caption = self.text_processor(ann["caption"])
 
         return {"image": image, "text_input": caption}
+
+class ImageTextPairInstructDataset(ImageTextPairDataset):
+    def __getitem__(self, index):
+        data = super().__getitem__(index)
+        if data != None:
+            data['text_output'] = data["text_input"]
+            data['text_input'] = self.text_processor("")
+        return data
```

## lavis/datasets/datasets/laion_dataset.py

```diff
@@ -3,15 +3,15 @@
  All rights reserved.
  SPDX-License-Identifier: BSD-3-Clause
  For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 """
 
 import webdataset as wds
 from lavis.datasets.datasets.base_dataset import BaseDataset
-
+import random
 
 class LaionDataset(BaseDataset):
     def __init__(self, vis_processor, text_processor, location):
         super().__init__(vis_processor=vis_processor, text_processor=text_processor)
 
         self.inner_dataset = wds.DataPipeline(
             wds.ResampledShards(location),
@@ -20,20 +20,33 @@
             wds.decode("pilrgb", handler=wds.warn_and_continue),
             wds.to_tuple("jpg", "json", handler=wds.warn_and_continue),
             wds.map_tuple(self.vis_processor, handler=wds.warn_and_continue),
             wds.map(self.to_dict, handler=wds.warn_and_continue),
         )
 
     def to_dict(self, sample):
+        if type(sample[1]) == list:
+            caption = random.choice(sample[1][:2])
+        else:
+            caption = sample[1]["caption"]
+
         return {
             "image": sample[0],
-            "text_input": self.text_processor(sample[1]["caption"]),
+            "text_input": self.text_processor(caption),
         }
 
 
+class LaionInstructDataset(LaionDataset):
+    def to_dict(self, sample):
+        data = super().to_dict(sample)
+        if data != None:
+            data['text_output'] = data["text_input"]
+            data['text_input'] = self.text_processor("")
+        return data
+
 if __name__ == "__main__":
     from torchvision import transforms
 
     def to_image_text_pair(sample):
         return sample[0], sample[1]["caption"]
 
     normalize = transforms.Normalize(
@@ -48,14 +61,16 @@
             normalize,
         ]
     )
 
     dataset = LaionDataset(
         vis_processor=transform_train,
         text_processor=lambda x: x,
+        # location="/export/laion400m-data-ssd/laion115m_capfilt_20220817/{part0/part0,part1/part1,part2/part2}_node{"
+        #          "00..15}_shard{000000..000118}.tar",
         location="/export/laion/laion2B-multi/part-00000/{00000..01743}.tar",
     )
 
     import torch
 
     loader = torch.utils.data.DataLoader(dataset.inner_dataset, batch_size=2)
```

## lavis/datasets/datasets/snli_ve_datasets.py

```diff
@@ -27,16 +27,16 @@
             }
         )
 
 
 class SNLIVisualEntialmentDataset(MultimodalClassificationDataset, __DisplMixin):
     def __init__(self, vis_processor, text_processor, vis_root, ann_paths):
         super().__init__(vis_processor, text_processor, vis_root, ann_paths)
-
         self.class_labels = self._build_class_labels()
+        self.classnames = list(self.class_labels.keys())
 
     def _build_class_labels(self):
         return {"contradiction": 0, "neutral": 1, "entailment": 2}
 
     def __getitem__(self, index):
         ann = self.annotation[index]
 
@@ -50,7 +50,21 @@
         return {
             "image": image,
             "text_input": sentence,
             "label": self.class_labels[ann["label"]],
             "image_id": image_id,
             "instance_id": ann["instance_id"],
         }
+
+class SNLIVisualEntialmentInstructDataset(SNLIVisualEntialmentDataset, __DisplMixin):
+    def __init__(self, vis_processor, text_processor, vis_root, ann_paths):
+        super().__init__(vis_processor, text_processor, vis_root, ann_paths)
+        self.classnames = ['no', 'maybe', 'yes']
+
+    def __getitem__(self, index):
+        data = super().__getitem__(index)
+        if data != None:
+            data["prompt"] = self.text_processor("based on the given the image is {} true?")
+            data["answer"] = self.classnames[data["label"]]
+            data["label"] = self.classnames[data["label"]]
+            data["question_id"] = data["instance_id"]
+        return data
```

## lavis/datasets/datasets/vg_vqa_datasets.py

```diff
@@ -2,14 +2,15 @@
  Copyright (c) 2022, salesforce.com, inc.
  All rights reserved.
  SPDX-License-Identifier: BSD-3-Clause
  For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 """
 
 import os
+import random
 
 from PIL import Image
 
 from lavis.datasets.datasets.vqa_datasets import VQADataset
 
 
 class VGVQADataset(VQADataset):
@@ -23,15 +24,28 @@
         image = Image.open(image_path).convert("RGB")
 
         image = self.vis_processor(image)
         question = self.text_processor(ann["question"])
 
         answers = [ann["answer"]]
         # TODO this should be configured better
-        weights = [0.2]
+        weights = [1.]
 
         return {
             "image": image,
             "text_input": question,
             "answers": answers,
             "weights": weights,
         }
+
+
+class VGVQAInstructDataset(VGVQADataset):
+    def __getitem__(self, index):
+        data = super().__getitem__(index)
+        if data != None:
+            data['text_output'] = random.choice(data["answers"])
+        return data
+    def collater(self, samples):
+        data = super().collater(samples)
+        data['text_output'] = data['answer']
+        return data
+
```

## lavis/datasets/datasets/video_caption_datasets.py

```diff
@@ -2,16 +2,16 @@
  Copyright (c) 2022, salesforce.com, inc.
  All rights reserved.
  SPDX-License-Identifier: BSD-3-Clause
  For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 """
 
 import os
+import math
 from lavis.datasets.datasets.base_dataset import BaseDataset
-
 from lavis.datasets.datasets.caption_datasets import CaptionDataset
 
 
 class VideoCaptionDataset(CaptionDataset):
     def __init__(self, vis_processor, text_processor, vis_root, ann_paths):
         """
         vis_root (string): Root directory of images (e.g. coco/images/)
@@ -22,16 +22,23 @@
 
     def __getitem__(self, index):
 
         ann = self.annotation[index]
 
         vname = ann["video"]
         video_path = os.path.join(self.vis_root, vname)
-
-        video = self.vis_processor(video_path)
+        
+        try:
+            video = self.vis_processor(video_path)
+        except:
+            print(f"Could not load {video_path}")
+            return None
+        if video==None:
+            return None
+        
         caption = self.text_processor(ann["caption"])
 
         # "image_id" is kept to stay compatible with the COCO evaluation format
         return {
             "video": video,
             "text_input": caption,
             "image_id": self.img_ids[ann["image_id"]],
@@ -42,22 +49,129 @@
     def __init__(self, vis_processor, text_processor, vis_root, ann_paths):
         """
         vis_root (string): Root directory of images (e.g. coco/images/)
         ann_root (string): directory to store the annotation file
         split (string): val or test
         """
         super().__init__(vis_processor, text_processor, vis_root, ann_paths)
+        # videos set. do not repeat videos in inference
+        ## todo: make it deduplicated because creating annotation file makes 
+        seen = set()
+        self.annotation = [x for x in self.annotation if x["video"] not in seen and not seen.add(x["image_id"])]
+    
+    def __len__(self):
+        return len(self.annotation)
 
     def __getitem__(self, index):
-
         ann = self.annotation[index]
 
         vname = ann["video"]
         video_path = os.path.join(self.vis_root, vname)
 
-        video = self.vis_processor(video_path)
+        try:
+            video = self.vis_processor(video_path)
+        except:
+            print(f"Could not load {video_path}")
+            return None
 
         return {
             "video": video,
             "image_id": ann["image_id"],
             "instance_id": ann["instance_id"],
         }
+
+
+class VideoCaptionInstructDataset(VideoCaptionDataset):
+    def __getitem__(self, index):
+        data = super().__getitem__(index)
+        if data != None:
+            data['text_output'] = data["text_input"]
+            data['text_input'] = self.text_processor("")
+        return data
+
+
+
+class ClipCaptionDataset(BaseDataset):
+    """
+    Handles video datasets where subclip of full video needs to be loaded. 
+    """
+    def __init__(self, vis_processor, text_processor, vis_root, ann_paths):
+        super().__init__(vis_processor, text_processor, vis_root, ann_paths)
+
+    def __getitem__(self, index):
+
+        ann = self.annotation[index]
+
+        vname = ann["video_path"]
+        video_path = os.path.join(self.vis_root, vname)
+        try:
+            video = self.vis_processor(video_path, start_sec=math.floor(ann['ts'][0]), end_sec=math.ceil(ann['ts'][1]))
+        except:
+            return None
+
+
+        caption = ann["caption"] if 'caption' in ann else ann["query"]
+
+        image_id = ann['youtube_id'] if 'youtube_id' in ann else ann["video_id"] if "video_id" in ann else vname
+
+        # "image_id" is kept to stay compatible with the COCO evaluation format
+        return {
+            "video": video,
+            "text_input": self.text_processor(caption),
+            "image_id": image_id,
+            "instance_id": ann['instance_id'],
+        }
+
+class ClipCaptionInstructDataset(ClipCaptionDataset):
+    def __getitem__(self, index):
+        data = super().__getitem__(index)
+        if data != None:
+            data['text_output'] = data["text_input"]
+            data['text_input'] = self.text_processor("")
+        return data
+
+class ClipCaptionEvalDataset(ClipCaptionDataset):
+    def __getitem__(self, index):
+        data = super().__getitem__(index)
+        if data != None:
+            del data["text_input"]
+        return data
+
+
+class WebVideoCaptionDataset(BaseDataset):
+    def __init__(self, vis_processor, text_processor, vis_root, ann_paths):
+        super().__init__(vis_processor, text_processor, vis_root, ann_paths)
+    
+    def _get_video(self, index):
+        """
+        If video does not exist, loop to the next one.
+        """
+        max_retries = 3
+        for _ in range(max_retries):
+            ann = self.annotation[index]
+            video_path = os.path.join(self.vis_root, f"{ann['videoid']}.mp4")
+            try:
+                video = self.vis_processor(video_path)
+                return video, video_path, ann
+            except:
+                index = (index + 1) % len(self.annotation)  # Safely loop back to start of annotations
+        return None
+
+    def __getitem__(self, index):
+        video, video_path, ann = self._get_video(index)
+        caption = self.text_processor(ann["name"])
+
+        # "image_id" is kept for compatibility with the COCO evaluation format
+        return {
+            "video": video,
+            "text_input": caption,
+            "image_id": ann["videoid"],
+            "instance_id": ann["instance_id"],
+        }
+
+class WebVideoCaptionInstructDataset(WebVideoCaptionDataset):
+    def __getitem__(self, index):
+        data = super().__getitem__(index)
+        if data != None:
+            data['text_output'] = data["text_input"]
+            data['text_input'] = self.text_processor("")
+        return data
```

## lavis/datasets/datasets/video_vqa_datasets.py

```diff
@@ -57,7 +57,28 @@
         return {
             "video": frms,
             "text_input": question,
             "answers": self._get_answer_label(ann["answer"]),
             "question_id": ann["question_id"],
             "instance_id": ann["instance_id"],
         }
+
+class VideoQAInstructDataset(VideoQADataset):
+    def __getitem__(self, index):
+        ann = self.annotation[index]
+
+        vname = ann["video"]
+        vpath = os.path.join(self.vis_root, vname)
+
+        frms = self.vis_processor(vpath)
+        question = self.text_processor(ann["question"])
+
+        return {
+            "video": frms,
+            "text_input": question,
+            "answer": ann["answer"],
+            "text_output": ann["answer"],
+            "question_id": ann["question_id"],
+            "instance_id": ann["instance_id"],
+            ## add weight to use with vqa eval script
+            "weight": [1.]
+        }
```

## lavis/datasets/datasets/vqa_datasets.py

```diff
@@ -11,14 +11,19 @@
 
 
 class VQADataset(BaseDataset):
     def __init__(self, vis_processor, text_processor, vis_root, ann_paths):
         super().__init__(vis_processor, text_processor, vis_root, ann_paths)
 
     def collater(self, samples):
+        # Filter out None samples
+        samples = [s for s in samples if s is not None]
+        # Check if samples is empty after filtering
+        if not samples:
+            return None
         image_list, question_list, answer_list, weight_list = [], [], [], []
 
         num_answers = []
 
         for sample in samples:
             image_list.append(sample["image"])
             question_list.append(sample["text_input"])
@@ -30,15 +35,21 @@
             answer_list.extend(answers)
             num_answers.append(len(answers))
 
         return {
             "image": torch.stack(image_list, dim=0),
             "text_input": question_list,
             "answer": answer_list,
-            "weight": torch.Tensor(weight_list),
+            "weight": weight_list,
             "n_answers": torch.LongTensor(num_answers),
         }
 
+class VQAInstructDataset(VQADataset):
+     def collater(self, samples):
+        data = super().collater(samples)
+        data['text_output'] = data['answer']
+        return data
 
 class VQAEvalDataset(BaseDataset):
     def __init__(self, vis_processor, text_processor, vis_root, ann_paths):
         super().__init__(vis_processor, text_processor, vis_root, ann_paths)
+
```

## lavis/models/__init__.py

```diff
@@ -33,14 +33,20 @@
 
 from lavis.models.blip2_models.blip2 import Blip2Base
 from lavis.models.blip2_models.blip2_opt import Blip2OPT
 from lavis.models.blip2_models.blip2_t5 import Blip2T5
 from lavis.models.blip2_models.blip2_qformer import Blip2Qformer
 from lavis.models.blip2_models.blip2_image_text_matching import Blip2ITM
 
+from lavis.models.blip2_models.blip2_t5_instruct import Blip2T5Instruct
+from lavis.models.blip2_models.blip2_vicuna_instruct import Blip2VicunaInstruct
+from lavis.models.blip2_models.blip2_vicuna_xinstruct import Blip2VicunaXInstruct
+
+from lavis.models.blip_diffusion_models.blip_diffusion import BlipDiffusion
+
 from lavis.models.pnp_vqa_models.pnp_vqa import PNPVQA
 from lavis.models.pnp_vqa_models.pnp_unifiedqav2_fid import PNPUnifiedQAv2FiD
 from lavis.models.img2prompt_models.img2prompt_vqa import Img2PromptVQA
 from lavis.models.med import XBertLMHeadDecoder
 from lavis.models.vit import VisionTransformerEncoder
 from lavis.models.clip_models.model import CLIP
 
@@ -60,24 +66,28 @@
     "AlproQA",
     "AlproRetrieval",
     "BaseModel",
     "BlipBase",
     "BlipFeatureExtractor",
     "BlipCaption",
     "BlipClassification",
+    "BlipDiffusion",
     "BlipITM",
     "BlipNLVR",
     "BlipPretrain",
     "BlipRetrieval",
     "BlipVQA",
     "Blip2Qformer",
     "Blip2Base",
     "Blip2ITM",
     "Blip2OPT",
     "Blip2T5",
+    "Blip2T5Instruct",
+    "Blip2VicunaInstruct",
+    "Blip2VicunaXInstruct",
     "PNPVQA",
     "Img2PromptVQA",
     "PNPUnifiedQAv2FiD",
     "CLIP",
     "VisionTransformerEncoder",
     "XBertLMHeadDecoder",
     "GPTDialogue",
```

## lavis/models/base_model.py

```diff
@@ -90,19 +90,39 @@
         if load_finetuned:
             finetune_path = cfg.get("finetuned", None)
             assert (
                 finetune_path is not None
             ), "Found load_finetuned is True, but finetune_path is None."
             self.load_checkpoint(url_or_filename=finetune_path)
         else:
-            # load pre-trained weights
-            pretrain_path = cfg.get("pretrained", None)
-            assert "Found load_finetuned is False, but pretrain_path is None."
-            self.load_from_pretrained(url_or_filename=pretrain_path, **kwargs)
+            load_pretrained = cfg.get("load_pretrained", True)
+            if load_pretrained:
+                # load pre-trained weights
+                pretrain_path = cfg.get("pretrained", None)
+                assert "Found load_finetuned is False, but pretrain_path is None."
+                self.load_from_pretrained(url_or_filename=pretrain_path, **kwargs)
 
+    def before_training(self, **kwargs):
+        pass
+
+    def get_optimizer_params(self, weight_decay, lr_scale=1):
+        p_wd, p_non_wd = [], []
+        for n, p in self.named_parameters():
+            if not p.requires_grad:
+                continue  # frozen weights
+            if p.ndim < 2 or "bias" in n or "ln" in n or "bn" in n:
+                p_non_wd.append(p)
+            else:
+                p_wd.append(p)        
+        optim_params = [
+            {"params": p_wd, "weight_decay": weight_decay, "lr_scale": lr_scale},
+            {"params": p_non_wd, "weight_decay": 0, "lr_scale": lr_scale},
+        ]                
+        return optim_params
+    
     def before_evaluation(self, **kwargs):
         pass
 
     def show_n_params(self, return_str=True):
         tot = 0
         for p in self.parameters():
             w = 1
```

## lavis/models/clip_vit.py

```diff
@@ -160,15 +160,15 @@
         self.conv1 = nn.Conv2d(in_channels=3, out_channels=width, kernel_size=patch_size, stride=patch_size, bias=False)
 
         scale = width ** -0.5
         self.class_embedding = nn.Parameter(scale * torch.randn(width))
         self.positional_embedding = nn.Parameter(scale * torch.randn(self.num_patches + 1, width))
         self.ln_pre = LayerNorm(width)
         
-        self.transformer = Transformer(width, layers-1, heads, use_grad_checkpointing=use_grad_checkpointing)
+        self.transformer = Transformer(width, layers, heads, use_grad_checkpointing=use_grad_checkpointing)
            
 #         self.ln_final = LayerNorm(width)
 
     def forward(self, x: torch.Tensor):
 
         x = self.conv1(x)  # shape = [*, width, grid, grid]
         x = x.reshape(x.shape[0], x.shape[1], -1)  # shape = [*, width, grid ** 2]
@@ -180,24 +180,33 @@
         x = x.permute(1, 0, 2)  # NLD -> LND
         x = self.transformer(x)
         x = x.permute(1, 0, 2)  # LND -> NLD
         
 #         x = self.ln_final(x)
         return x
     
-    
+    def get_num_layer(self, var_name=""):
+        if var_name in ("class_embedding", "positional_embedding", "conv1", "ln_pre"):
+            return 0
+        elif var_name.startswith("transformer.resblocks"):
+            layer_id = int(var_name.split('.')[2])
+            return layer_id + 1
+        else:
+            return len(self.transformer.resblocks)    
+            
             
 # From PyTorch internals
 def _ntuple(n):
     def parse(x):
         if isinstance(x, collections.abc.Iterable):
             return x
         return tuple(repeat(x, n))
     return parse
-to_2tuple = _ntuple(2)        
+to_2tuple = _ntuple(2)    
+    
 def interpolate_pos_embed(model, state_dict, interpolation: str = 'bicubic', seq_dim=1):
     # Rescale the grid of position embeddings when loading from state_dict
     old_pos_embed = state_dict.get('positional_embedding', None)
     
     grid_size = round((model.positional_embedding.shape[0] - 1) ** 0.5)
     if old_pos_embed is None:
         return
@@ -231,15 +240,15 @@
     
     
 def create_clip_vit_L(img_size=224,use_checkpoint=False,precision="fp16"):
     model = VisionTransformer(
             input_resolution=img_size,
             patch_size=14,
             width=1024,
-            layers=22,
+            layers=23,
             heads=16,
             use_grad_checkpointing=use_checkpoint,
         )         
     url = "https://storage.googleapis.com/sfr-vision-language-research/LAVIS/models/BLIP2/clip_vit_L.pth"
     cached_file = download_cached_file(
         url, check_hash=False, progress=True
     )
@@ -247,8 +256,8 @@
     interpolate_pos_embed(model,state_dict)
     
     incompatible_keys = model.load_state_dict(state_dict, strict=False)
     # print(incompatible_keys)
     
     if precision == "fp16":
         convert_weights_to_fp16(model)
-    return model
+    return model
```

## lavis/models/eva_vit.py

```diff
@@ -365,15 +365,28 @@
         rel_pos_bias = self.rel_pos_bias() if self.rel_pos_bias is not None else None
         for blk in self.blocks:
             x = blk(x, rel_pos_bias)
             features.append(x)
 
         return features
     
-    
+    def get_num_layer(self, var_name=""):
+        if var_name in ("cls_token", "mask_token", "pos_embed"):
+            return 0
+        elif var_name.startswith("patch_embed"):
+            return 0
+        elif var_name.startswith("rel_pos_bias"):
+            return len(self.blocks) - 1
+        elif var_name.startswith("blocks"):
+            layer_id = int(var_name.split('.')[1])
+            return layer_id + 1
+        else:
+            return len(self.blocks)
+        
+            
 def interpolate_pos_embed(model, checkpoint_model):
     if 'pos_embed' in checkpoint_model:
         pos_embed_checkpoint = checkpoint_model['pos_embed'].float()
         embedding_size = pos_embed_checkpoint.shape[-1]
         num_patches = model.patch_embed.num_patches
         num_extra_tokens = model.pos_embed.shape[-2] - num_patches
         # height (== width) for the checkpoint position embedding
```

## lavis/models/blip2_models/blip2.py

```diff
@@ -24,16 +24,16 @@
 from lavis.models.eva_vit import create_eva_vit_g
 from lavis.models.clip_vit import create_clip_vit_L
 from transformers import BertTokenizer
 
 
 class Blip2Base(BaseModel):
     @classmethod
-    def init_tokenizer(cls):
-        tokenizer = BertTokenizer.from_pretrained("bert-base-uncased")
+    def init_tokenizer(cls, truncation_side="right"):
+        tokenizer = BertTokenizer.from_pretrained("bert-base-uncased", truncation_side=truncation_side)
         tokenizer.add_special_tokens({"bos_token": "[DEC]"})
         return tokenizer
 
     def maybe_autocast(self, dtype=torch.float16):
         # if on cpu, don't use autocast
         # if on gpu, use autocast with dtype if provided, otherwise use torch.float16
         enable_autocast = self.device != torch.device("cpu")
@@ -56,29 +56,34 @@
         )
         query_tokens = nn.Parameter(
             torch.zeros(1, num_query_token, encoder_config.hidden_size)
         )
         query_tokens.data.normal_(mean=0.0, std=encoder_config.initializer_range)
         return Qformer, query_tokens
 
-    @classmethod
     def init_vision_encoder(
-        cls, model_name, img_size, drop_path_rate, use_grad_checkpoint, precision
+        self, model_name, img_size, drop_path_rate, use_grad_checkpoint, precision
     ):
         assert model_name in [
             "eva_clip_g",
+            "eva2_clip_L",
             "clip_L",
-        ], "vit model must be eva_clip_g or clip_L"
+        ], "vit model must be eva_clip_g, eva2_clip_L or clip_L"
         if model_name == "eva_clip_g":
             visual_encoder = create_eva_vit_g(
                 img_size, drop_path_rate, use_grad_checkpoint, precision
             )
+#         elif model_name == "eva2_clip_L":
+#             visual_encoder = create_eva2_vit_L(
+#                 img_size, drop_path_rate, use_grad_checkpoint, precision
+#             )
         elif model_name == "clip_L":
             visual_encoder = create_clip_vit_L(img_size, use_grad_checkpoint, precision)
         ln_vision = LayerNorm(visual_encoder.num_features)
+        self.vit_name = model_name
         return visual_encoder, ln_vision
 
     def load_from_pretrained(self, url_or_filename):
         if is_url(url_or_filename):
             cached_file = download_cached_file(
                 url_or_filename, check_hash=False, progress=True
             )
@@ -93,14 +98,95 @@
         msg = self.load_state_dict(state_dict, strict=False)
 
         # logging.info("Missing keys {}".format(msg.missing_keys))
         logging.info("load checkpoint from %s" % url_or_filename)
 
         return msg
 
+    def get_optimizer_params(self, weight_decay, lr_scale=1):
+
+        vit_num_layers = self.visual_encoder.get_num_layer()
+        lr_scales = list(lr_scale ** (vit_num_layers + 1 - i) for i in range(vit_num_layers + 2))
+
+        parameter_group_names = {}
+        parameter_group_vars = {}
+
+        for name, param in self.named_parameters():
+            if not param.requires_grad:
+                continue  # frozen weights
+            if len(param.shape) == 1 or name.endswith(".bias"):
+                group_name = "no_decay"
+                this_weight_decay = 0.
+            else:
+                group_name = "decay"
+                this_weight_decay = weight_decay
+            if 'visual_encoder' in name:
+                layer_id = self.visual_encoder.get_num_layer(name.replace('visual_encoder.',''))
+                group_name = "vit_layer_%d_%s" % (layer_id, group_name)
+            else:
+                layer_id = None
+
+            if group_name not in parameter_group_names:
+                if layer_id is not None:
+                    scale = lr_scales[layer_id]
+                else:
+                    scale = 1
+                parameter_group_names[group_name] = {
+                    "weight_decay": this_weight_decay,
+                    "params": [],
+                    "lr_scale": scale
+                }
+                parameter_group_vars[group_name] = {
+                    "weight_decay": this_weight_decay,
+                    "params": [],
+                    "lr_scale": scale
+                }
+            parameter_group_vars[group_name]["params"].append(param)
+            parameter_group_names[group_name]["params"].append(name)
+        # import json
+        # print("Param groups = %s" % json.dumps(parameter_group_names, indent=2))
+        optim_params = list(parameter_group_vars.values())
+        return optim_params
+
+    def _lemmatize(self, answers):
+        def apply(answer):
+            doc = self.lemmatizer(answer)
+
+            words = []
+            for token in doc:
+                if token.pos_ in ["NOUN", "VERB"]:
+                    words.append(token.lemma_)
+                else:
+                    words.append(token.text)
+            answer = " ".join(words)
+
+            return answer
+
+        return [apply(answer) for answer in answers]
+
+    @property
+    def lemmatizer(self):
+        if self._lemmatizer is None:
+            try:
+                import spacy
+
+                self._lemmatizer = spacy.load("en_core_web_sm")
+            except ImportError:
+                logging.error(
+                    """
+                    Please install spacy and en_core_web_sm model to apply lemmatization.
+                    python -m spacy download en_core_web_sm
+                    OR
+                    import spacy.cli
+                    spacy.cli.download("en_core_web_sm")
+                    """
+                )
+                exit(1)
+
+        return self._lemmatizer
 
 def disabled_train(self, mode=True):
     """Overwrite model.train with this function to make sure train/eval mode
     does not change anymore."""
     return self
```

## lavis/models/blip2_models/blip2_opt.py

```diff
@@ -1,23 +1,25 @@
 """
  Copyright (c) 2023, salesforce.com, inc.
  All rights reserved.
  SPDX-License-Identifier: BSD-3-Clause
  For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 """
 import logging
+from packaging import version
 
 import torch
 from torch.cuda.amp import autocast as autocast
 import torch.nn as nn
 
 from lavis.common.registry import registry
 from lavis.models.blip2_models.blip2 import Blip2Base, disabled_train
-from lavis.models.blip2_models.modeling_opt import OPTForCausalLM, OPTConfig
-from transformers import AutoTokenizer
+# from lavis.models.blip2_models.modeling_opt import OPTForCausalLM, OPTConfig
+from transformers import AutoTokenizer, OPTForCausalLM, OPTConfig
+import transformers
 
 
 @registry.register_model("blip2_opt")
 class Blip2OPT(Blip2Base):
     """
     BLIP2 OPT model.
     Supported model types:
@@ -45,17 +47,23 @@
         use_grad_checkpoint=False,
         vit_precision="fp16",
         freeze_vit=True,
         num_query_token=32,
         opt_model="facebook/opt-2.7b",
         prompt="",
         max_txt_len=32,
+        apply_lemmatizer=False,
     ):
+        """
+        apply_lemmatizer: when set to True, postprocess predict_answers() result with lemmas.
+        """
         super().__init__()
-
+        transformers_version = version.parse(transformers.__version__)
+        assert transformers_version >= version.parse("4.27"), "BLIP-2 OPT requires transformers>=4.27"
+        
         self.tokenizer = self.init_tokenizer()
 
         self.visual_encoder, self.ln_vision = self.init_vision_encoder(
             vit_model, img_size, drop_path_rate, use_grad_checkpoint, vit_precision
         )
         if freeze_vit:
             for name, param in self.visual_encoder.named_parameters():
@@ -88,14 +96,17 @@
             self.Qformer.config.hidden_size, self.opt_model.config.hidden_size
         )
 
         self.max_txt_len = max_txt_len
         self.prompt = prompt
         prompt_tokens = self.opt_tokenizer(self.prompt, return_tensors="pt")
         self.prompt_length = prompt_tokens.attention_mask.sum(1)
+        
+        self._apply_lemmatizer = apply_lemmatizer
+        self._lemmatizer = None       
 
     def forward(self, samples):
         image = samples["image"]
         with self.maybe_autocast():
             image_embeds = self.ln_vision(self.visual_encoder(image))
         image_atts = torch.ones(image_embeds.size()[:-1], dtype=torch.long).to(
             image.device
@@ -201,72 +212,214 @@
             if "prompt" in samples.keys():
                 prompt = samples["prompt"]
             else:
                 prompt = self.prompt
 
             prompt = [prompt] * image.size(0)
 
-            opt_tokens = self.opt_tokenizer(prompt, return_tensors="pt").to(
-                image.device
-            )
-            input_ids = opt_tokens.input_ids
+            opt_tokens = self.opt_tokenizer(
+                prompt,
+                return_tensors="pt",
+                padding="longest",
+                truncation=True,
+                max_length=self.max_txt_len,
+            ).to(image.device)
             attention_mask = torch.cat([atts_opt, opt_tokens.attention_mask], dim=1)
-
-            if use_nucleus_sampling:
-                query_embeds = inputs_opt.repeat_interleave(num_captions, dim=0)
-                num_beams = 1
-            else:
-                query_embeds = inputs_opt.repeat_interleave(num_beams, dim=0)
-
+            
+            # new version for transformers>=4.27
+            inputs_embeds = self.opt_model.get_input_embeddings()(opt_tokens.input_ids)
+            inputs_embeds = torch.cat([inputs_opt,inputs_embeds],dim=1)
+            
             outputs = self.opt_model.generate(
-                input_ids=input_ids,
-                query_embeds=query_embeds,
+                inputs_embeds=inputs_embeds, 
                 attention_mask=attention_mask,
                 do_sample=use_nucleus_sampling,
                 top_p=top_p,
                 temperature=temperature,
                 num_beams=num_beams,
-                max_new_tokens=max_length,
+                max_length=max_length,
                 min_length=min_length,
                 eos_token_id=self.eos_token_id,
                 repetition_penalty=repetition_penalty,
                 length_penalty=length_penalty,
                 num_return_sequences=num_captions,
             )
-
-            prompt_length = opt_tokens.input_ids.shape[1]
             output_text = self.opt_tokenizer.batch_decode(
-                outputs[:, prompt_length:], skip_special_tokens=True
+                outputs, skip_special_tokens=True
             )
+                            
+            # previous version for transformers<4.27
+            # if use_nucleus_sampling:
+            #     query_embeds = inputs_opt.repeat_interleave(num_captions, dim=0)
+            #     num_beams = 1
+            # else:
+            #     query_embeds = inputs_opt.repeat_interleave(num_beams, dim=0)
+
+            # outputs = self.opt_model.generate(
+            #     input_ids=input_ids,
+            #     query_embeds=query_embeds,
+            #     attention_mask=attention_mask,
+            #     do_sample=use_nucleus_sampling,
+            #     top_p=top_p,
+            #     temperature=temperature,
+            #     num_beams=num_beams,
+            #     max_new_tokens=max_length,
+            #     min_length=min_length,
+            #     eos_token_id=self.eos_token_id,
+            #     repetition_penalty=repetition_penalty,
+            #     length_penalty=length_penalty,
+            #     num_return_sequences=num_captions,
+            # )
+
+            # prompt_length = opt_tokens.input_ids.shape[1]
+            # output_text = self.opt_tokenizer.batch_decode(
+            #     outputs[:, prompt_length:], skip_special_tokens=True
+            # )
+            
             output_text = [text.strip() for text in output_text]
             return output_text
+        
+        
+    def predict_answers(
+        self,
+        samples,
+        num_beams=5,
+        inference_method="generate",
+        max_len=10,
+        min_len=1,
+        num_ans_candidates=128,
+        answer_list=None,
+        prompt="",
+        length_penalty=0,
+        **kwargs
+    ):
+        image = samples["image"]
+        with self.maybe_autocast():
+            image_embeds = self.ln_vision(self.visual_encoder(image))
+            image_atts = torch.ones(image_embeds.size()[:-1], dtype=torch.long).to(
+                image.device
+            )
+
+            query_tokens = self.query_tokens.expand(image_embeds.shape[0], -1, -1)
+            query_output = self.Qformer.bert(
+                query_embeds=query_tokens,
+                encoder_hidden_states=image_embeds,
+                encoder_attention_mask=image_atts,
+                return_dict=True,
+            )
+
+            inputs_opt = self.opt_proj(query_output.last_hidden_state)
+            atts_opt = torch.ones(inputs_opt.size()[:-1], dtype=torch.long).to(
+                image.device
+            )
+
+            if isinstance(samples["text_input"], str):
+                samples["text_input"] = [samples["text_input"]]
+            if prompt:
+                text_input = [prompt.format(question) for question in samples["text_input"]]
+            else:
+                text_input = samples["text_input"]
+
+            self.opt_tokenizer.padding_side = "left"
+            opt_tokens = self.opt_tokenizer(
+                text_input,
+                return_tensors="pt",
+                padding="longest",
+                truncation=True,
+                max_length=self.max_txt_len,
+            ).to(image.device)
+        
+            attention_mask = torch.cat([atts_opt, opt_tokens.attention_mask], dim=1)
+            
+            # require transformers>=4.27
+            inputs_embeds = self.opt_model.get_input_embeddings()(opt_tokens.input_ids)
+            inputs_embeds = torch.cat([inputs_opt,inputs_embeds],dim=1)
+            
+            outputs = self.opt_model.generate(
+                inputs_embeds=inputs_embeds,
+                attention_mask=attention_mask,
+                do_sample=False,
+                num_beams=num_beams,
+                max_new_tokens=max_len,
+                min_length=min_len,
+                eos_token_id=self.eos_token_id,
+                length_penalty=length_penalty,
+            )
+            output_text = self.opt_tokenizer.batch_decode(
+                outputs, skip_special_tokens=True
+            )
+            output_text = [text.strip() for text in output_text]
+        if self._apply_lemmatizer or ("apply_lemmatizer" in samples.keys() and samples["apply_lemmatizer"]):
+            output_text = self._lemmatize(output_text)
+
+        return output_text
+    
+    def _lemmatize(self, answers):
+        def apply(answer):
+            doc = self.lemmatizer(answer)
+
+            words = []
+            for token in doc:
+                if token.pos_ in ["NOUN", "VERB"]:
+                    words.append(token.lemma_)
+                else:
+                    words.append(token.text)
+            answer = " ".join(words)
+
+            return answer
+
+        return [apply(answer) for answer in answers]
+
+    @property
+    def lemmatizer(self):
+        if self._lemmatizer is None:
+            try:
+                import spacy
+
+                self._lemmatizer = spacy.load("en_core_web_sm")
+            except ImportError:
+                logging.error(
+                    """
+                    Please install spacy and en_core_web_sm model to apply lemmatization.
+                    python -m spacy download en_core_web_sm
+                    OR
+                    import spacy.cli
+                    spacy.cli.download("en_core_web_sm")
+                    """
+                )
+                exit(1)
 
+        return self._lemmatizer
+        
     @classmethod
     def from_config(cls, cfg):
         vit_model = cfg.get("vit_model", "eva_clip_g")
         img_size = cfg.get("image_size")
         num_query_token = cfg.get("num_query_token")
         opt_model = cfg.get("opt_model")
 
         drop_path_rate = cfg.get("drop_path_rate", 0)
         use_grad_checkpoint = cfg.get("use_grad_checkpoint", False)
         vit_precision = cfg.get("vit_precision", "fp16")
         freeze_vit = cfg.get("freeze_vit", True)
 
         prompt = cfg.get("prompt", "")
         max_txt_len = cfg.get("max_txt_len", 32)
+        
+        apply_lemmatizer = cfg.get("apply_lemmatizer", False)
 
         model = cls(
             vit_model=vit_model,
             img_size=img_size,
             drop_path_rate=drop_path_rate,
             use_grad_checkpoint=use_grad_checkpoint,
             vit_precision=vit_precision,
             freeze_vit=freeze_vit,
             num_query_token=num_query_token,
             opt_model=opt_model,
             prompt=prompt,
             max_txt_len=max_txt_len,
+            apply_lemmatizer=apply_lemmatizer,
         )
         model.load_checkpoint_from_config(cfg)
 
         return model
```

## lavis/models/blip2_models/blip2_qformer.py

```diff
@@ -152,28 +152,45 @@
 
         rank = dist.get_rank()
         bs = image.size(0)
         targets = torch.linspace(rank * bs, rank * bs + bs - 1, bs, dtype=int).to(
             image.device
         )
 
-        loss_itc = (
-            F.cross_entropy(sim_i2t, targets, label_smoothing=0.1)
-            + F.cross_entropy(sim_t2i, targets, label_smoothing=0.1)
-        ) / 2
+        if "image_id" in samples.keys(): #coco retrieval finetuning
+            image_ids = samples["image_id"].view(-1,1)
+            image_ids_all = concat_all_gather(image_ids)
+            pos_idx = torch.eq(image_ids, image_ids_all.t()).float()       
+            sim_targets = pos_idx / pos_idx.sum(1,keepdim=True)   
+            sim_targets = 0.9 * sim_targets + 0.1 * torch.ones_like(sim_targets) / sim_targets.size(1)
+
+            loss_t2i = -torch.sum(F.log_softmax(sim_t2i, dim=1)*sim_targets,dim=1).mean()
+            loss_i2t = -torch.sum(F.log_softmax(sim_i2t, dim=1)*sim_targets,dim=1).mean()     
+            loss_itc = (loss_t2i+loss_i2t)/2  
+        else:                     
+            loss_itc = (
+                F.cross_entropy(sim_i2t, targets, label_smoothing=0.1)
+                + F.cross_entropy(sim_t2i, targets, label_smoothing=0.1)
+            ) / 2
 
         ###============== Image-text Matching ===================###
         text_input_ids_world = concat_all_gather(text_tokens.input_ids)
         text_attention_mask_world = concat_all_gather(text_tokens.attention_mask)
         image_embeds_world = all_gather_with_grad(image_embeds)
         with torch.no_grad():
-            weights_t2i = F.softmax(sim_t2i, dim=1) + 1e-4
-            weights_t2i[:, rank * bs : rank * bs + bs].fill_diagonal_(0)
-            weights_i2t = F.softmax(sim_i2t, dim=1) + 1e-4
-            weights_i2t[:, rank * bs : rank * bs + bs].fill_diagonal_(0)
+            if "image_id" in samples.keys():
+                mask = torch.eq(image_ids, image_ids_all.t())
+                sim_t2i.masked_fill_(mask, -10000)
+                sim_i2t.masked_fill_(mask, -10000)
+            else:    
+                sim_t2i[:, rank * bs : rank * bs + bs].fill_diagonal_(-10000)
+                sim_i2t[:, rank * bs : rank * bs + bs].fill_diagonal_(-10000)            
+                
+            weights_t2i = F.softmax(sim_t2i, dim=1)
+            weights_i2t = F.softmax(sim_i2t, dim=1)
 
         # select a negative image for each text
         image_embeds_neg = []
         for b in range(bs):
             neg_idx = torch.multinomial(weights_t2i[b], 1).item()
             image_embeds_neg.append(image_embeds_world[neg_idx])
         image_embeds_neg = torch.stack(image_embeds_neg, dim=0)
```

## lavis/models/blip_models/blip.py

```diff
@@ -3,24 +3,30 @@
  All rights reserved.
  SPDX-License-Identifier: BSD-3-Clause
  For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 """
 
 import logging
 import os
+from packaging import version
 
 import torch
 from lavis.common.dist_utils import download_cached_file
 from lavis.common.utils import is_url
 from lavis.models.base_model import BaseModel
 from lavis.models.vit import interpolate_pos_embed
 from transformers import BertTokenizer
-
+import transformers
 
 class BlipBase(BaseModel):
+    def __init__(self):
+        super().__init__()
+        transformers_version = version.parse(transformers.__version__)
+        assert transformers_version < version.parse("4.27"), "BLIP models are not compatible with transformers>=4.27, run pip install transformers==4.25 to downgrade"
+        
     @classmethod
     def init_tokenizer(cls):
         tokenizer = BertTokenizer.from_pretrained("bert-base-uncased")
         tokenizer.add_special_tokens({"bos_token": "[DEC]"})
         tokenizer.add_special_tokens({"additional_special_tokens": ["[ENC]"]})
         tokenizer.enc_token_id = tokenizer.additional_special_tokens_ids[0]
         return tokenizer
```

## lavis/models/img2prompt_models/img2prompt_vqa.py

```diff
@@ -1,17 +1,23 @@
 """
  Copyright (c) 2022, salesforce.com, inc.
  All rights reserved.
  SPDX-License-Identifier: BSD-3-Clause
  For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
+
+ (CVPR 23') From Images to Textual Prompts: Zero-shot VQA with Frozen Large Language Models,
+ by Jiaxian Guo, Junnan Li, Dongxu Li, Anthony Meng Huat Tiong, Boyang Li, Dacheng Tao, Steven CH Hoi
+
+ Initially referred as Img2prompt_vqa, later Img2LLM_vqa.
 """
 
 import logging
 import random
 
+import spacy
 import torch
 import torch.nn.functional as F
 from transformers import T5ForConditionalGeneration, T5Tokenizer
 
 from lavis.common.dist_utils import download_cached_file
 from lavis.common.registry import registry
 from lavis.models.base_model import BaseModel
```

## lavis/processors/__init__.py

```diff
@@ -13,36 +13,52 @@
 )
 from lavis.processors.blip_processors import (
     BlipImageTrainProcessor,
     Blip2ImageTrainProcessor,
     BlipImageEvalProcessor,
     BlipCaptionProcessor,
 )
+from lavis.processors.blip_diffusion_processors import (
+    BlipDiffusionInputImageProcessor,
+    BlipDiffusionTargetImageProcessor,
+)
 from lavis.processors.gpt_processors import (
     GPTVideoFeatureProcessor,
     GPTDialogueProcessor,
 )
 from lavis.processors.clip_processors import ClipImageTrainProcessor
+from lavis.processors.audio_processors import BeatsAudioProcessor
+from lavis.processors.ulip_processors import ULIPPCProcessor
+from lavis.processors.instruction_text_processors import BlipInstructionProcessor
 
 from lavis.common.registry import registry
 
 __all__ = [
     "BaseProcessor",
     # ALPRO
     "AlproVideoTrainProcessor",
     "AlproVideoEvalProcessor",
     # BLIP
     "BlipImageTrainProcessor",
     "Blip2ImageTrainProcessor",
     "BlipImageEvalProcessor",
     "BlipCaptionProcessor",
+    "BlipInstructionProcessor",
+    # BLIP-Diffusion
+    "BlipDiffusionInputImageProcessor",
+    "BlipDiffusionTargetImageProcessor",
+    # CLIP
     "ClipImageTrainProcessor",
     # GPT
     "GPTVideoFeatureProcessor",
     "GPTDialogueProcessor",
+    # AUDIO
+    "BeatsAudioProcessor",
+    # 3D
+    "ULIPPCProcessor",
 ]
 
 
 def load_processor(name, cfg=None):
     """
     Example
```

## lavis/processors/alpro_processors.py

```diff
@@ -3,15 +3,15 @@
  All rights reserved.
  SPDX-License-Identifier: BSD-3-Clause
  For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 """
 
 import torch
 from lavis.common.registry import registry
-from lavis.datasets.data_utils import load_video
+from lavis.datasets.data_utils import load_video, load_clip
 from lavis.processors import transforms_video
 from lavis.processors.base_processor import BaseProcessor
 from lavis.processors.randaugment import VideoRandomAugment
 from lavis.processors import functional_video as F
 from omegaconf import OmegaConf
 from torchvision import transforms
 
@@ -84,18 +84,20 @@
         self,
         image_size=384,
         mean=None,
         std=None,
         min_scale=0.5,
         max_scale=1.0,
         n_frms=MAX_INT,
+        full_video=True,
     ):
         super().__init__(mean=mean, std=std, n_frms=n_frms)
 
         self.image_size = image_size
+        self.full_video=full_video
 
         self.transform = transforms.Compose(
             [
                 # Video size is (C, T, H, W)
                 transforms_video.RandomResizedCropVideo(
                     image_size,
                     scale=(min_scale, max_scale),
@@ -104,15 +106,15 @@
                 transforms_video.RandomHorizontalFlipVideo(),
                 ToTHWC(),  # C, T, H, W -> T, H, W, C
                 VideoRandomAugment(
                     2,
                     5,
                     augs=[
                         "Identity",
-                        "AutoContrast",
+                        # "AutoContrast",
                         "Brightness",
                         "Sharpness",
                         "Equalize",
                         "ShearX",
                         "ShearY",
                         "TranslateX",
                         "TranslateY",
@@ -121,30 +123,58 @@
                 ),
                 ToUint8(),
                 transforms_video.ToTensorVideo(),  # T, H, W, C -> C, T, H, W
                 self.normalize,
             ]
         )
 
-    def __call__(self, vpath):
+    def __call__(self, vpath, start_sec=None, end_sec=None):
         """
         Args:
             clip (torch.tensor): Video clip to be cropped. Size is (C, T, H, W)
         Returns:
             torch.tensor: video clip after transforms. Size is (C, T, size, size).
         """
-        clip = load_video(
-            video_path=vpath,
-            n_frms=self.n_frms,
-            height=self.image_size,
-            width=self.image_size,
-            sampling="headtail",
-        )
+        if self.full_video:
+            clip = load_video( ## initial LAVIS code has errors when loading video.
+                video_path=vpath,
+                n_frms=self.n_frms,
+                height=self.image_size,
+                width=self.image_size,
+                sampling="headtail",
+            )
+            # clip = load_clip(
+            #     video_path=vpath, 
+            #     num_frames=self.n_frms, 
+            #     target_height=self.image_size, 
+            #     target_width=self.image_size,
+            #     start_time=start_sec,
+            #     end_time=end_sec, 
+            #     sampling="headtail"
+            #     )
+        else:
+            clip = load_clip(
+                video_path=vpath, 
+                num_frames=self.n_frms, 
+                target_height=self.image_size, 
+                target_width=self.image_size,
+                start_time=start_sec,
+                end_time=end_sec, 
+                sampling="headtail"
+                )
+        transformed = self.transform(clip)
+
+        ## repeat last frame for padding
+        pad_size = self.n_frms - transformed.shape[1]
+        if pad_size>0:
+            last_frame = transformed[:, -1, :, :].unsqueeze(1)
+            repeat_frames = last_frame.repeat(1, pad_size, 1, 1)
+            transformed = torch.cat([transformed, repeat_frames], dim=1)
 
-        return self.transform(clip)
+        return transformed
 
     @classmethod
     def from_config(cls, cfg=None):
         if cfg is None:
             cfg = OmegaConf.create()
 
         image_size = cfg.get("image_size", 256)
@@ -152,65 +182,91 @@
         mean = cfg.get("mean", None)
         std = cfg.get("std", None)
 
         min_scale = cfg.get("min_scale", 0.5)
         max_scale = cfg.get("max_scale", 1.0)
 
         n_frms = cfg.get("n_frms", MAX_INT)
+        full_video = cfg.get("full_video", True)
 
         return cls(
             image_size=image_size,
             mean=mean,
             std=std,
             min_scale=min_scale,
             max_scale=max_scale,
             n_frms=n_frms,
+            full_video=full_video
         )
 
 
 @registry.register_processor("alpro_video_eval")
 class AlproVideoEvalProcessor(AlproVideoBaseProcessor):
-    def __init__(self, image_size=256, mean=None, std=None, n_frms=MAX_INT):
+    def __init__(self, image_size=256, mean=None, std=None, n_frms=MAX_INT,  full_video=True):
         super().__init__(mean=mean, std=std, n_frms=n_frms)
 
         self.image_size = image_size
+        self.full_video=full_video
 
         # Input video size is (C, T, H, W)
         self.transform = transforms.Compose(
             [
                 # frames will be resized during decord loading.
                 ToUint8(),  # C, T, H, W
                 ToTHWC(),  # T, H, W, C
                 transforms_video.ToTensorVideo(),  # C, T, H, W
                 self.normalize,  # C, T, H, W
             ]
         )
 
-    def __call__(self, vpath):
+    def __call__(self, vpath, start_sec=None, end_sec=None):
         """
         Args:
             clip (torch.tensor): Video clip to be cropped. Size is (C, T, H, W)
         Returns:
             torch.tensor: video clip after transforms. Size is (C, T, size, size).
         """
-        clip = load_video(
-            video_path=vpath,
-            n_frms=self.n_frms,
-            height=self.image_size,
-            width=self.image_size,
-        )
+        if self.full_video:
+            clip = load_clip(
+                video_path=vpath, 
+                num_frames=self.n_frms, 
+                target_height=self.image_size, 
+                target_width=self.image_size,
+                start_time=start_sec,
+                end_time=end_sec, 
+                sampling="headtail"
+                )
+        else:
+            clip = load_clip(
+                video_path=vpath, 
+                num_frames=self.n_frms, 
+                target_height=self.image_size, 
+                target_width=self.image_size,
+                start_time=start_sec,
+                end_time=end_sec, 
+                sampling="headtail"
+                )
+        transformed = self.transform(clip)
+
+        ## repeat last frame for padding
+        pad_size = self.n_frms - transformed.shape[1]
+        if pad_size>0:
+            last_frame = transformed[:, -1, :, :].unsqueeze(1)
+            repeat_frames = last_frame.repeat(1, pad_size, 1, 1)
+            transformed = torch.cat([transformed, repeat_frames], dim=1)
 
-        return self.transform(clip)
+        return transformed
 
     @classmethod
     def from_config(cls, cfg=None):
         if cfg is None:
             cfg = OmegaConf.create()
 
         image_size = cfg.get("image_size", 256)
+        full_video = cfg.get("full_video", True)
 
         mean = cfg.get("mean", None)
         std = cfg.get("std", None)
 
         n_frms = cfg.get("n_frms", MAX_INT)
 
-        return cls(image_size=image_size, mean=mean, std=std, n_frms=n_frms)
+        return cls(image_size=image_size, mean=mean, std=std, n_frms=n_frms, full_video=full_video)
```

## lavis/projects/blip2/train/pretrain_stage1.yaml

```diff
@@ -2,16 +2,15 @@
  # All rights reserved.
  # SPDX-License-Identifier: BSD-3-Clause
  # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 
 model:
   arch: blip2
   model_type: pretrain
-  # TODO: support stage 1 pretraining from scratch (load_pretrained=False does not have effect as of now)
-  load_pretrained: False
+  load_pretrained: False #pretrain from scratch
   freeze_vit: True
 
 
 datasets:
   coco_caption:
     vis_processor:
         train:
```

## lavis/runners/runner_base.py

```diff
@@ -96,40 +96,31 @@
 
         return self._wrapped_model
 
     @property
     def optimizer(self):
         # TODO make optimizer class and configurations
         if self._optimizer is None:
+            lr_scale = self.config.run_cfg.get("lr_layer_decay", 1)
+            weight_decay = self.config.run_cfg.get("weight_decay", 0.05)
+            optim_params = self._model.get_optimizer_params(weight_decay,lr_scale)
+
             num_parameters = 0
-            p_wd, p_non_wd = [], []
-            for n, p in self.model.named_parameters():
-                if not p.requires_grad:
-                    continue  # frozen weights
-                if p.ndim < 2 or "bias" in n or "ln" in n or "bn" in n:
-                    p_non_wd.append(p)
-                else:
-                    p_wd.append(p)
-                num_parameters += p.data.nelement()
-            logging.info("number of trainable parameters: %d" % num_parameters)
-            optim_params = [
-                {
-                    "params": p_wd,
-                    "weight_decay": float(self.config.run_cfg.weight_decay),
-                },
-                {"params": p_non_wd, "weight_decay": 0},
-            ]
+            for p_group in optim_params:
+                for p in p_group["params"]:
+                    num_parameters += p.data.nelement()    
+            logging.info("number of trainable parameters: {}".format(num_parameters))      
+                  
             beta2 = self.config.run_cfg.get("beta2", 0.999)
+
             self._optimizer = torch.optim.AdamW(
                 optim_params,
                 lr=float(self.config.run_cfg.init_lr),
-                weight_decay=float(self.config.run_cfg.weight_decay),
                 betas=(0.9, beta2),
-            )
-
+            )    
         return self._optimizer
 
     @property
     def scaler(self):
         amp = self.config.run_cfg.get("amp", False)
 
         if amp:
@@ -277,14 +268,29 @@
     def max_epoch(self):
         return int(self.config.run_cfg.max_epoch)
 
     @property
     def log_freq(self):
         log_freq = self.config.run_cfg.get("log_freq", 50)
         return int(log_freq)
+    
+    @property
+    def save_freq(self):
+        save_freq = self.config.run_cfg.get("save_freq", 5)
+        return int(save_freq)
+
+    @property
+    def val_freq(self):
+        val_freq = self.config.run_cfg.get("val_freq", 1)
+        return int(val_freq)
+    
+    @property
+    def save_last(self):
+        save_last = self.config.run_cfg.get("save_last", True)
+        return int(save_last)
 
     @property
     def init_lr(self):
         return float(self.config.run_cfg.init_lr)
 
     @property
     def min_lr(self):
@@ -365,50 +371,64 @@
         if not self.evaluate_only and self.resume_ckpt_path is not None:
             self._load_checkpoint(self.resume_ckpt_path)
 
         for cur_epoch in range(self.start_epoch, self.max_epoch):
             # training phase
             if not self.evaluate_only:
                 logging.info("Start training")
+                # See https://github.com/salesforce/LAVIS/issues/449
+                # if cur_epoch == self.start_epoch:
+                #     self.task.before_training(
+                #         model=self.unwrap_dist_model(self.model),
+                #         dataset=self.datasets["train"],
+                #     )
                 train_stats = self.train_epoch(cur_epoch)
                 self.log_stats(split_name="train", stats=train_stats)
 
             # evaluation phase
-            if len(self.valid_splits) > 0:
+            if len(self.valid_splits) > 0 and (self.evaluate_only or cur_epoch%self.val_freq == 0):
                 for split_name in self.valid_splits:
                     logging.info("Evaluating on {}.".format(split_name))
-
+                    
                     val_log = self.eval_epoch(
                         split_name=split_name, cur_epoch=cur_epoch
                     )
                     if val_log is not None:
                         if is_main_process():
                             assert (
                                 "agg_metrics" in val_log
                             ), "No agg_metrics found in validation log."
 
                             agg_metrics = val_log["agg_metrics"]
                             if agg_metrics > best_agg_metric and split_name == "val":
                                 best_epoch, best_agg_metric = cur_epoch, agg_metrics
-
-                                self._save_checkpoint(cur_epoch, is_best=True)
+                                if not self.evaluate_only:
+                                    self._save_checkpoint(cur_epoch, is_best=True)
 
                             val_log.update({"best_epoch": best_epoch})
                             self.log_stats(val_log, split_name)
 
             else:
                 # if no validation split is provided, we just save the checkpoint at the end of each epoch.
                 if not self.evaluate_only:
                     self._save_checkpoint(cur_epoch, is_best=False)
 
             if self.evaluate_only:
                 break
 
+            # save checkpoint according to save freq
+            if self.save_freq>0 and cur_epoch%self.save_freq == 0:
+                self._save_checkpoint(cur_epoch, is_best=False)
+
             dist.barrier()
 
+        # save last checkpoint
+        if self.save_last and not self.evaluate_only:
+            self._save_checkpoint(cur_epoch, is_best=False)
+
         # testing phase
         test_epoch = "best" if len(self.valid_splits) > 0 else cur_epoch
         self.evaluate(cur_epoch=test_epoch, skip_reload=self.evaluate_only)
 
         total_time = time.time() - start_time
         total_time_str = str(datetime.timedelta(seconds=int(total_time)))
         logging.info("Training time {}".format(total_time_str))
@@ -572,14 +592,15 @@
             k: v.requires_grad for (k, v) in model_no_ddp.named_parameters()
         }
         state_dict = model_no_ddp.state_dict()
         for k in list(state_dict.keys()):
             if k in param_grad_dic.keys() and not param_grad_dic[k]:
                 # delete parameters that do not require gradient
                 del state_dict[k]
+
         save_obj = {
             "model": state_dict,
             "optimizer": self.optimizer.state_dict(),
             "config": self.config.to_dict(),
             "scaler": self.scaler.state_dict() if self.scaler else None,
             "epoch": cur_epoch,
         }
```

## lavis/runners/runner_iter.py

```diff
@@ -87,20 +87,24 @@
             # training phase
             if not self.evaluate_only:
                 logging.info(
                     "Start training, max_iters={}, in total {} inner epochs.".format(
                         self.max_iters, int(self.max_iters / self.iters_per_inner_epoch)
                     )
                 )
-
+                if start_iters == self.start_iters:
+                    self.task.before_training(
+                        model=self.unwrap_dist_model(self.model),
+                        dataset=self.datasets,
+                    )
                 train_stats = self.train_iters(self.cur_epoch, start_iters)
                 self.log_stats(split_name="train", stats=train_stats)
 
             # evaluation phase
-            if len(self.valid_splits) > 0:
+            if len(self.valid_splits) > 0 and (self.evaluate_only or (end_iters//self.iters_per_inner_epoch)%self.val_freq == 0):
                 for split_name in self.valid_splits:
                     logging.info("Evaluating on {}.".format(split_name))
 
                     val_log = self.eval_epoch(
                         split_name=split_name, cur_epoch=self._progress(end_iters)
                     )
                     if val_log is not None:
@@ -121,16 +125,25 @@
             else:
                 # if no validation split is provided, we just save the checkpoint at the end of each inner epoch.
                 if not self.evaluate_only:
                     self._save_checkpoint(end_iters, is_best=False)
 
             if self.evaluate_only:
                 break
+
+            # save checkpoint according to save freq
+            # if self.save_freq>0 and (end_iters//self.iters_per_inner_epoch)%self.save_freq == 0:
+            self._save_checkpoint(end_iters, is_best=False)
+
             dist.barrier()
 
+        # save last checkpoint
+        if self.save_last and not self.evaluate_only:
+            self._save_checkpoint(end_iters, is_best=False)
+
         # testing phase
         self.evaluate(cur_epoch=self.cur_epoch)
 
         total_time = time.time() - start_time
         total_time_str = str(datetime.timedelta(seconds=int(total_time)))
         logging.info("Training time {}".format(total_time_str))
 
@@ -149,17 +162,28 @@
             lr_scheduler=self.lr_scheduler,
             cuda_enabled=self.cuda_enabled,
             log_freq=self.log_freq,
             accum_grad_iters=self.accum_grad_iters,
         )
 
     @main_process
-    def _save_checkpoint(self, cur_iters, is_best=False):
+    def _save_checkpoint(self, cur_iters, is_best=False, is_last=False):
+        model_no_ddp = self.unwrap_dist_model(self.model)
+        param_grad_dic = {
+            k: v.requires_grad for (k, v) in model_no_ddp.named_parameters()
+        }
+
+        state_dict = model_no_ddp.state_dict()
+        for k in list(state_dict.keys()):
+            if k in param_grad_dic.keys() and not param_grad_dic[k]:
+                # delete parameters that do not require gradient
+                del state_dict[k]
+
         save_obj = {
-            "model": self.unwrap_dist_model(self.model).state_dict(),
+            "model": state_dict,
             "optimizer": self.optimizer.state_dict(),
             "config": self.config.to_dict(),
             "scaler": self.scaler.state_dict() if self.scaler else None,
             "iters": cur_iters,
         }
         save_to = os.path.join(
             self.output_dir,
@@ -243,15 +267,15 @@
                         )
                     )
 
                 dataset_ratios = [float(dataset_ratios[k]) for k in self.datasets]
                 self.datasets = reorg_datasets_by_split(self.datasets)
                 # to keep the same structure as return value of concat_datasets
                 self.datasets = {
-                    k: v[0] if len(v) == 1 else v for k, v in datasets.items()
+                    k: v[0] if len(v) == 1 else v for k, v in self.datasets.items()
                 }
 
             # print dataset statistics after concatenation/chaining
             for split_name in self.datasets:
                 if isinstance(self.datasets[split_name], tuple) or isinstance(
                     self.datasets[split_name], list
                 ):
```

## lavis/tasks/__init__.py

```diff
@@ -9,17 +9,18 @@
 from lavis.tasks.base_task import BaseTask
 from lavis.tasks.captioning import CaptionTask
 from lavis.tasks.image_text_pretrain import ImageTextPretrainTask
 from lavis.tasks.multimodal_classification import (
     MultimodalClassificationTask,
 )
 from lavis.tasks.retrieval import RetrievalTask
-from lavis.tasks.vqa import VQATask, GQATask, AOKVQATask
+from lavis.tasks.vqa import VQATask, GQATask, AOKVQATask, DisCRNTask
 from lavis.tasks.vqa_reading_comprehension import VQARCTask, GQARCTask
 from lavis.tasks.dialogue import DialogueTask
+from lavis.tasks.text_to_image_generation import TextToImageGenerationTask
 
 
 def setup_task(cfg):
     assert "task" in cfg.run_cfg, "Task name must be provided."
 
     task_name = cfg.run_cfg.task
     task = registry.get_task_class(task_name).setup_task(cfg=cfg)
@@ -38,8 +39,10 @@
     "VQARCTask",
     "GQARCTask",
     "MultimodalClassificationTask",
     # "VideoQATask",
     # "VisualEntailmentTask",
     "ImageTextPretrainTask",
     "DialogueTask",
+    "TextToImageGenerationTask",
+    "DisCRNTask"
 ]
```

## lavis/tasks/base_task.py

```diff
@@ -48,28 +48,34 @@
 
         datasets_config = cfg.datasets_cfg
 
         assert len(datasets_config) > 0, "At least one dataset has to be specified."
 
         for name in datasets_config:
             dataset_config = datasets_config[name]
-
             builder = registry.get_builder_class(name)(dataset_config)
             dataset = builder.build_datasets()
 
             datasets[name] = dataset
 
         return datasets
 
     def train_step(self, model, samples):
-        loss = model(samples)["loss"]
-        return loss
+        output = model(samples)
+        loss_dict = {}
+        for k,v in output.items():
+            if "loss" in k:
+                loss_dict[k] = v
+        return output["loss"], loss_dict
 
     def valid_step(self, model, samples):
         raise NotImplementedError
+    
+    def before_training(self, model, dataset, **kwargs):
+        model.before_training(dataset=dataset, task_type=type(self))
 
     def before_evaluation(self, model, dataset, **kwargs):
         model.before_evaluation(dataset=dataset, task_type=type(self))
 
     def after_evaluation(self, **kwargs):
         pass
 
@@ -197,26 +203,32 @@
             # if using iter-based runner, we stop after iters_per_epoch iterations.
             if i >= iters_per_epoch:
                 break
 
             samples = next(data_loader)
 
             samples = prepare_sample(samples, cuda_enabled=cuda_enabled)
+
+            ## notify model that sample is empty (error occured)
+            if not isinstance(samples, dict):
+                samples = {"is_empty":True}
+
             samples.update(
                 {
                     "epoch": inner_epoch,
                     "num_iters_per_epoch": iters_per_epoch,
                     "iters": i,
                 }
             )
 
             lr_scheduler.step(cur_epoch=inner_epoch, cur_step=i)
 
             with torch.cuda.amp.autocast(enabled=use_amp):
-                loss = self.train_step(model=model, samples=samples)
+                loss, loss_dict = self.train_step(model=model, samples=samples)
+                loss /= accum_grad_iters #TODO: not affect loss_dict values for logging
 
             # after_train_step()
             if use_amp:
                 scaler.scale(loss).backward()
             else:
                 loss.backward()
 
@@ -225,15 +237,15 @@
                 if use_amp:
                     scaler.step(optimizer)
                     scaler.update()                     
                 else:    
                     optimizer.step()
                 optimizer.zero_grad()
 
-            metric_logger.update(loss=loss.item())
+            metric_logger.update(**loss_dict)
             metric_logger.update(lr=optimizer.param_groups[0]["lr"])
 
         # after train_epoch()
         # gather the stats from all processes
         metric_logger.synchronize_between_processes()
         logging.info("Averaged stats: " + str(metric_logger.global_avg()))
         return {
```

## lavis/tasks/captioning.py

```diff
@@ -3,66 +3,126 @@
  All rights reserved.
  SPDX-License-Identifier: BSD-3-Clause
  For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 """
 
 import json
 import os
-
-from lavis.common.dist_utils import main_process
+import pandas as pd
+from tqdm import tqdm
+from lavis.common.dist_utils import main_process, get_rank
 from lavis.common.registry import registry
 from lavis.tasks.base_task import BaseTask
-
+from lavis.common.utils import is_convertible_to_int, is_url, cache_url
 
 @registry.register_task("captioning")
 class CaptionTask(BaseTask):
-    def __init__(self, num_beams, max_len, min_len, evaluate, report_metric=True):
+    def __init__(self, num_beams, max_len, min_len, repetition_penalty, length_penalty, top_p, temperature, evaluate, report_metric=True, annotation_file=None, sample_id_key="image_id", caption_key="caption", split=["val"], load_gt_from_file=False, img_ids = []):
         super().__init__()
 
         self.num_beams = num_beams
         self.max_len = max_len
         self.min_len = min_len
+        self.repetition_penalty = repetition_penalty
+        self.length_penalty = length_penalty
+        self.top_p = top_p
+        self.temperature = temperature
         self.evaluate = evaluate
 
         self.report_metric = report_metric
+        self.annotation_file = annotation_file
+        self.sample_id_key = sample_id_key
+        self.caption_key = caption_key
+        assert len(split) == 1, "Only support one split for evaluation."
+        self.split = split[0]
+        self.load_gt_from_file = load_gt_from_file
+        self.img_ids = img_ids
 
     @classmethod
     def setup_task(cls, cfg):
         run_cfg = cfg.run_cfg
 
-        num_beams = run_cfg.num_beams
-        max_len = run_cfg.max_len
-        min_len = run_cfg.min_len
+        num_beams = run_cfg.get("num_beams", 5)
+        max_len = run_cfg.get("max_len", 30)
+        min_len = run_cfg.get("min_len", 1)
+        repetition_penalty = run_cfg.get("repetition_penalty", 1.15)
+        length_penalty = run_cfg.get("length_penalty", 0.)
+        top_p = run_cfg.get("top_p", 0.9)
+        temperature = run_cfg.get("temperature", 1.)
         evaluate = run_cfg.evaluate
 
         report_metric = run_cfg.get("report_metric", True)
+        annotation_file = run_cfg.get("annotation_file", None)
+        sample_id_key = run_cfg.get("sample_id_key", "image_id")
+        caption_key = run_cfg.get("caption_key", "caption")
+        load_gt_from_file = run_cfg.get("load_gt_from_file", False)
+        split = run_cfg.get("valid_splits", ["val"])
+        img_ids = run_cfg.get("img_ids", []) # evaluate only subset of imgs
 
         return cls(
             num_beams=num_beams,
             max_len=max_len,
             min_len=min_len,
+            repetition_penalty=repetition_penalty,
+            length_penalty=length_penalty,
+            top_p=top_p,
+            temperature=temperature,
             evaluate=evaluate,
             report_metric=report_metric,
+            annotation_file=annotation_file,
+            sample_id_key=sample_id_key,
+            caption_key=caption_key,
+            split=split,
+            load_gt_from_file=load_gt_from_file,
+            img_ids=img_ids
         )
 
+    def build_datasets(self, cfg):
+        datasets = super().build_datasets(cfg)
+
+        # get validation dataset name
+        val_ds_name = []
+        for name,d in datasets.items():
+            if self.split in d:
+                val_ds_name.append(name)
+        if not val_ds_name:
+            return datasets # no validation sets
+        assert len(val_ds_name) == 1, "Only support one dataset for validation"
+        val_ds_name = val_ds_name[0]
+
+        # get question file, annotation file and anwser list in COCO format
+        if self.annotation_file == None:
+            if 'coco' not in val_ds_name: # coco is already precomputed in dataset
+                self.annotation_file = os.path.join(registry.get_path("cache_root"),f'{val_ds_name}_gt', f'{val_ds_name}_{self.split}_annotations.json')
+                if get_rank() == 0:
+                    os.makedirs(os.path.join(registry.get_path("cache_root"),f'{val_ds_name}_gt'), exist_ok=True)
+                    convert_to_coco_gt(datasets[val_ds_name], self.annotation_file, self.caption_key, self.sample_id_key, self.split, load_gt_from_file=self.load_gt_from_file, img_ids=self.img_ids)
+        return datasets
+
     def valid_step(self, model, samples):
         results = []
-
         # run_cfg = slf.cfg.run_cfg
         captions = model.generate(
             samples,
             use_nucleus_sampling=False,
             num_beams=self.num_beams,
             max_length=self.max_len,
             min_length=self.min_len,
+            repetition_penalty=self.repetition_penalty,
+            length_penalty=self.length_penalty,
+            top_p=self.top_p,
+            temperature=self.temperature,
         )
-
-        img_ids = samples["image_id"]
+        img_ids = samples[self.sample_id_key]
         for caption, img_id in zip(captions, img_ids):
-            results.append({"caption": caption, "image_id": int(img_id)})
+            # not all img_ids are ints
+            img_id = int(img_id) if is_convertible_to_int(img_id) else img_id
+            if self.img_ids and img_id not in self.img_ids: # only include specified img_ids if specified
+                continue
+            results.append({"caption": caption, "image_id": img_id})
 
         return results
 
     def after_evaluation(self, val_result, split_name, epoch, **kwargs):
         eval_result_file = self.save_result(
             result=val_result,
             result_dir=registry.get_path("result_dir"),
@@ -78,60 +138,118 @@
             metrics = {"agg_metrics": 0.0}
 
         return metrics
 
     @main_process
     def _report_metrics(self, eval_result_file, split_name):
 
-        # TODO better way to define this
-        coco_gt_root = os.path.join(registry.get_path("cache_root"), "coco_gt")
-        coco_val = coco_caption_eval(coco_gt_root, eval_result_file, split_name)
+        if self.annotation_file == None:
+            # TODO better way to define this
+            coco_gt_root = os.path.join(registry.get_path("cache_root"), "coco_gt")
+            coco_val = coco_caption_eval(coco_gt_root, eval_result_file, split_name, img_ids=self.img_ids)
+        else:
+            coco_val = coco_caption_eval(None, eval_result_file, split_name, annotation_file=self.annotation_file, img_ids=self.img_ids)
 
         agg_metrics = coco_val.eval["CIDEr"] + coco_val.eval["Bleu_4"]
         log_stats = {split_name: {k: v for k, v in coco_val.eval.items()}}
 
         with open(
             os.path.join(registry.get_path("output_dir"), "evaluate.txt"), "a"
         ) as f:
             f.write(json.dumps(log_stats) + "\n")
 
         coco_res = {k: v for k, v in coco_val.eval.items()}
         coco_res["agg_metrics"] = agg_metrics
 
         return coco_res
 
+def load_gt_file(file_path):
+    if is_url(file_path):
+        file_path = cache_url(file_path, registry.get_path("cache_root"))
+    data = []
+    if any(ext in file_path for ext in ['csv', 'tsv']):
+        df = pd.read_csv(file_path)
+        data.extend(df.to_dict(orient="records"))
+        
+    elif 'jsonl' in file_path:
+        with open(file_path, "r") as f:
+            data.extend([json.loads(line) for line in f])
+    else:
+        with open(file_path, "r") as f:
+            loaded = json.load(f)
+            if isinstance(loaded, list):
+                data.extend(loaded)
+            elif isinstance(loaded, dict):
+                # assume that loaded data in file  is the corresponding caption to the key
+                data.extend([{"sample_id": k, **v} if isinstance(v, dict) else {"sample_id": k, "caption": v} for k, v in loaded.items()])
+    return data
+
+def convert_to_coco_gt(data, outpath, caption_key, sample_id_key, split, load_gt_from_file=False, img_ids=[]):
+    gt_data = {"annotations":[], "images":[]}
+    if load_gt_from_file:
+        print(f"Generating ground truth file for evaluation from {load_gt_from_file}....")
+        data = load_gt_file(load_gt_from_file)
+        for ann in data:
+            captions = ann[caption_key]
+            img_id = int(ann[sample_id_key]) if is_convertible_to_int(ann[sample_id_key]) else ann[sample_id_key]
+            if img_ids and img_id not in img_ids: # only include specified img_ids if specified
+                continue
+            gt_data["images"].append({"id":img_id})
+            if isinstance(captions, str):
+                gt_data["annotations"].append({"image_id":img_id, "caption":captions, "id":img_id})
+            else:   
+                gt_data["annotations"].extend([{"image_id":img_id, "caption":c, "id":img_id} for c in captions])
+    else:
+        print(f"Generating ground truth file for evaluation....")
+        for i,ann in tqdm(enumerate(data[split])):
+            captions = data[split].annotation[i][caption_key]
+            img_id = int(ann[sample_id_key]) if is_convertible_to_int(ann[sample_id_key]) else ann[sample_id_key]
+            if img_ids and img_id not in img_ids: # only include specified img_ids if specified
+                continue
+            gt_data["images"].append({"id":img_id})
+            if isinstance(captions, str):
+                gt_data["annotations"].append({"image_id":img_id, "caption":captions, "id":img_id})
+            else:   
+                gt_data["annotations"].extend([{"image_id":img_id, "caption":c, "id":img_id} for c in captions])
+    json.dump(gt_data, open(outpath, 'w'))
+    print(f"Saved annotations at {outpath}")
 
 # TODO better structure for this.
 from pycocoevalcap.eval import COCOEvalCap
 from pycocotools.coco import COCO
 from torchvision.datasets.utils import download_url
 
 
-def coco_caption_eval(coco_gt_root, results_file, split):
-    urls = {
-        "val": "https://storage.googleapis.com/sfr-vision-language-research/datasets/coco_karpathy_val_gt.json",
-        "test": "https://storage.googleapis.com/sfr-vision-language-research/datasets/coco_karpathy_test_gt.json",
-    }
-    filenames = {
-        "val": "coco_karpathy_val_gt.json",
-        "test": "coco_karpathy_test_gt.json",
-    }
-
-    download_url(urls[split], coco_gt_root)
-    annotation_file = os.path.join(coco_gt_root, filenames[split])
+def coco_caption_eval(coco_gt_root, results_file, split, annotation_file=None, img_ids=[]):
 
+    if annotation_file == None:
+        urls = {
+            "val": "https://storage.googleapis.com/sfr-vision-language-research/datasets/coco_karpathy_val_gt.json",
+            "test": "https://storage.googleapis.com/sfr-vision-language-research/datasets/coco_karpathy_test_gt.json",
+        }
+        filenames = {
+            "val": "coco_karpathy_val_gt.json",
+            "test": "coco_karpathy_test_gt.json",
+        }
+
+        download_url(urls[split], coco_gt_root)
+        annotation_file = os.path.join(coco_gt_root, filenames[split])
+    if is_url(annotation_file):
+        annotation_file = cache_url(annotation_file, registry.get_path("cache_root"))
+        
     # create coco object and coco_result object
     coco = COCO(annotation_file)
     coco_result = coco.loadRes(results_file)
 
     # create coco_eval object by taking coco and coco_result
     coco_eval = COCOEvalCap(coco, coco_result)
 
     # evaluate on a subset of images by setting
-    # coco_eval.params['image_id'] = coco_result.getImgIds()
+    if img_ids:
+        coco_eval.params['image_id'] = coco_result.getImgIds()
     # please remove this line when evaluating the full validation set
     # coco_eval.params['image_id'] = coco_result.getImgIds()
 
     # evaluate results
     # SPICE will take a few minutes the first time, but speeds up due to caching
     coco_eval.evaluate()
```

## lavis/tasks/multimodal_classification.py

```diff
@@ -4,51 +4,101 @@
  SPDX-License-Identifier: BSD-3-Clause
  For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 """
 
 import json
 import os
 import logging
+import inspect
 
 import numpy as np
 import torch
 from lavis.common.dist_utils import main_process
 from lavis.common.registry import registry
 from lavis.tasks.base_task import BaseTask
 
 
 @registry.register_task("multimodal_classification")
 class MultimodalClassificationTask(BaseTask):
-    def __init__(self):
+    def __init__(self,
+                 max_len,
+                 min_len,
+                 length_penalty,
+                 segments):
         super().__init__()
+        self.max_len = max_len
+        self.min_len = min_len
+        self.length_penalty = length_penalty
+        self.segments = segments
+    
+    
+    @classmethod
+    def setup_task(cls, cfg):
+        run_cfg = cfg.run_cfg
+
+        max_len = run_cfg.get("max_len", 30)
+        min_len = run_cfg.get("min_len", 1)
+        length_penalty = run_cfg.get("length_penalty", -1.)
+        segments = run_cfg.get("segments", 1)
+
+        return cls(
+            max_len=max_len,
+            min_len=min_len,
+            length_penalty=length_penalty,
+            segments=segments
+        )
 
     def valid_step(self, model, samples):
         results = []
 
-        outputs = model.predict(samples)
+        argspec = inspect.getargspec(model.predict)
+        # check if model allows for generation arguments in classification 
+        if all([k in argspec.args for k in ['max_length', "min_length", "length_penalty"]]):
+             outputs = model.predict(samples,
+                                    max_length=self.max_len,
+                                    min_length=self.min_len,
+                                    length_penalty=self.length_penalty,
+                                    )
+        else:
+            outputs = model.predict(samples, n_segments=self.segments)
+        
+        if outputs == None: # missing data
+            return {} 
 
         predictions = outputs["predictions"]
-        targets = outputs["targets"]
 
-        predictions = predictions.max(1)[1].cpu().numpy()
-        targets = targets.cpu().numpy()
-
-        indices = samples[self.inst_id_key]
-
-        for pred, tgt, index in zip(predictions, targets, indices):
-            if isinstance(index, torch.Tensor):
-                index = index.item()
-
-            results.append(
-                {
-                    self.inst_id_key: index,
-                    "prediction": pred.item(),
-                    "target": tgt.item(),
-                }
-            )
+        if isinstance(predictions[0], str):
+            targets = samples["label"]
+            indices = samples[self.inst_id_key]
+            for pred, tgt, index in zip(predictions, targets, indices):
+                results.append(
+                    {
+                        self.inst_id_key: index,
+                        "prediction": pred,
+                        "target": tgt,
+                    }
+                )
+        else:
+            targets = outputs["targets"]
+            predictions = predictions.max(1)[1].cpu().numpy()
+            targets = targets.cpu().numpy()
+
+            indices = samples[self.inst_id_key]
+
+            for pred, tgt, index in zip(predictions, targets, indices):
+                if isinstance(index, torch.Tensor):
+                    index = index.item()
+
+                results.append(
+                    {
+                        self.inst_id_key: index,
+                        "prediction": pred.item(),
+                        "target": tgt.item(),
+                    }
+                )
 
         return results
 
     def after_evaluation(self, val_result, split_name, epoch, **kwargs):
         eval_result_file = self.save_result(
             result=val_result,
             result_dir=registry.get_path("result_dir"),
```

## lavis/tasks/vqa.py

```diff
@@ -4,15 +4,18 @@
  SPDX-License-Identifier: BSD-3-Clause
  For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 """
 
 import logging
 import json
 import os
+import torch
+from tqdm import tqdm
 
+from lavis.common.utils import is_convertible_to_int
 import lavis.common.dist_utils as dist_utils
 from lavis.common.registry import registry
 from lavis.common.vqa_tools.vqa import VQA
 from lavis.common.vqa_tools.vqa_eval import VQAEval
 from lavis.tasks.base_task import BaseTask
 
 
@@ -23,68 +26,100 @@
         num_beams,
         max_len,
         min_len,
         evaluate,
         num_ans_candidates,
         inference_method="rank",
         prompt="",
+        sample_id_key = "",
+        ques_files=dict(),
+        anno_files=dict(),
+        valid_splits=['val']
     ):
         super().__init__()
 
         self.num_beams = num_beams
         self.max_len = max_len
         self.min_len = min_len
 
         self.evaluate = evaluate
         self.inference_method = inference_method
         self.num_ans_candidates = num_ans_candidates
         self.prompt = prompt
 
         self.answer_list = None
 
-        self.ques_files = dict()
-        self.anno_files = dict()
+        self.ques_files = ques_files
+        self.anno_files = anno_files
+
+        # generalize to non coco data
+        self.sample_id_key = sample_id_key
+
+        self.valid_splits = valid_splits
 
     @classmethod
     def setup_task(cls, cfg):
         run_cfg = cfg.run_cfg
 
         num_beams = run_cfg.get("num_beams", 3)
         max_len = run_cfg.get("max_len", 10)
         min_len = run_cfg.get("min_len", 1)
 
         evaluate = run_cfg.get("evaluate", False)
 
         inference_method = run_cfg.get("inference_method", "rank")
         num_ans_candidates = run_cfg.get("num_ans_candidates", 128)
+
         prompt = run_cfg.get("prompt", "")
 
+        # generalize to non coco data
+        sample_id_key = run_cfg.get("sample_id_key", "instance_id")
+        ques_files = run_cfg.get("ques_files", dict())
+        anno_files = run_cfg.get("anno_files", dict())
+        valid_splits = run_cfg.get("valid_splits", ["val"])
+
+
         return cls(
             num_beams=num_beams,
             max_len=max_len,
             min_len=min_len,
             evaluate=evaluate,
             num_ans_candidates=num_ans_candidates,
             inference_method=inference_method,
             prompt=prompt,
+            sample_id_key = sample_id_key,
+            ques_files=ques_files,
+            anno_files=anno_files,
+            valid_splits=valid_splits
         )
 
     def build_datasets(self, cfg):
         datasets = super().build_datasets(cfg)
 
         # get question file, annotation file and anwser list in COCO format
-        for dataset in datasets.values():
-            for split in dataset:
+        for ds_name, dataset in datasets.items():
+            for split in self.valid_splits:
+                if split not in dataset:
+                    print(f"Split {split} not found in {ds_name}.")
                 if (
                     hasattr(dataset[split], "coco_fmt_qust_file")
                     and dataset[split].coco_fmt_qust_file is not None
                 ):
                     self.ques_files[split] = dataset[split].coco_fmt_qust_file
                     self.anno_files[split] = dataset[split].coco_fmt_anno_file
-
+                else:
+                    if split not in self.ques_files: # precomputed and passed in task builder
+                        self.ques_files[split] = os.path.join(registry.get_path("cache_root"),f'{ds_name}_gt', f'{ds_name}_{split}_questions.json')
+                        self.anno_files[split] = os.path.join(registry.get_path("cache_root"), f'{ds_name}_gt', f'{ds_name}_{split}_annotations.json')
+                        if dist_utils.get_rank() == 0:
+                            os.makedirs(os.path.join(registry.get_path("cache_root"),f'{ds_name}_gt'), exist_ok=True)
+                            try:
+                                convert_to_coco_gt(dataset, self.ques_files[split], self.anno_files[split], split, self.sample_id_key)
+                            except:
+                                pass # tasks like vizwiz with no gt answer
                 try:
                     self.answer_list = dataset[split].answer_list
                 except AttributeError:
                     # if answer_list is not provided, then set it to None
                     pass
 
         if len(self.ques_files) > 0:
@@ -105,15 +140,17 @@
             num_ans_candidates=self.num_ans_candidates,
             prompt=self.prompt,
         )
         pred_qa_pairs = []
 
         question_id = samples["question_id"]
         for answer, ques_id in zip(answers, question_id):
-            ques_id = int(ques_id.item())
+            ques_id = int(ques_id.item()) if isinstance(ques_id, torch.Tensor) else ques_id
+            if ques_id != int and is_convertible_to_int(ques_id):
+                ques_id = int(ques_id)
             pred_qa_pairs.append({"question_id": ques_id, "answer": answer})
 
         return pred_qa_pairs
 
     def after_evaluation(self, val_result, split_name, **kwargs):
         result_file = self.save_result(
             val_result,
@@ -134,15 +171,14 @@
         metrics = {}
 
         if split in self.ques_files and split in self.anno_files:
             vqa = VQA(self.anno_files[split], self.ques_files[split])
             vqa_result = vqa.loadRes(
                 resFile=result_file, quesFile=self.ques_files[split]
             )
-
             # create vqaEval object by taking vqa and vqaRes
             # n is precision of accuracy (number of places after decimal), default is 2
             vqa_scorer = VQAEval(vqa, vqa_result, n=2)
             logging.info("Start VQA evaluation.")
             vqa_scorer.evaluate()
 
             # print accuracies
@@ -159,128 +195,205 @@
                 )
                 metrics[ans_type] = vqa_scorer.accuracy["perAnswerType"][ans_type]
 
             with open(
                 os.path.join(registry.get_path("output_dir"), "evaluate.txt"), "a"
             ) as f:
                 f.write(json.dumps(metrics) + "\n")
-
         return metrics
 
-@registry.register_task("gqa")
-class GQATask(VQATask):
+def convert_to_coco_gt(data, outpath_questions, outpath_annotations, split, sample_id_key):
+    if split not in data:
+        return
+    questions_data = {'info':"", 'task_type':"", 'data_type':"", 'license':"", 'data_subtype':"", 'questions':[]}
+    annotations_data = {'info':"", 'task_type':"", 'data_type':"", 'license':"", 'data_subtype':"", 'annotations':[]}
+    print("Generating ground truth annotations...")
+    for ann in tqdm(data[split]):
+        if ann == None:
+            continue
+        # if ann[sample_id_key] not in img_ids:
+        #     continue
+        ques_id = ann["question_id"]
+        ques_id = int(ques_id.item()) if isinstance(ques_id, torch.Tensor) else ques_id
+        if ques_id != int and is_convertible_to_int(ques_id):
+            ques_id = int(ques_id)
+        questions_data["questions"].append({"question": ann["text_input"], "image_id": ann[sample_id_key], "question_id": ques_id})
+        annotations_data["annotations"].append({
+            "question_type": "" if "question_type" not in ann else ann["question_type"],
+            "multiple_choice_answer": ann["answers"][0] if isinstance(ann["answers"], list) else ann["answers"],
+            "answers": [{"answer":ans, "answer_id":i} for i,ans in enumerate(ann["answers"])] if isinstance(ann["answers"], list) else [{"answer":ann["answers"], "answer_id":0}], 
+            "image_id": ann[sample_id_key], 
+            "question_id": ques_id,
+            "answer_type": "" if "answer_type" not in ann else ann["answer_type"],
+        })
+       
+    json.dump(questions_data, open(outpath_questions, 'w'))
+    print(f"Saved questions data at {outpath_questions}")
+    json.dump(annotations_data, open(outpath_annotations, 'w'))
+    print(f"Saved annotation data at {outpath_annotations}")
+
+        
+
+@registry.register_task("aok_vqa")
+class AOKVQATask(VQATask):
     def valid_step(self, model, samples):
         answers = model.predict_answers(
             samples=samples,
             answer_list=self.answer_list,
             inference_method=self.inference_method,
             num_beams=self.num_beams,
             max_len=self.max_len,
             min_len=self.min_len,
             num_ans_candidates=self.num_ans_candidates,
-            prompt=self.prompt,
         )
+
         pred_qa_pairs = []
 
         question_id = samples["question_id"]
-        gt_answers = samples["answer"]
-        
-        for answer, ques_id, gt_answer in zip(answers, question_id, gt_answers):
-            ques_id = int(ques_id.item())
-            pred_qa_pairs.append({"question_id": ques_id, "pred_ans": answer, "gt_ans": gt_answer})
+        gt_answers = samples["direct_answers"]
+
+        for pred_answer, ques_id, gt_answer in zip(answers, question_id, gt_answers):
+            pred_qa_pairs.append(
+                {"question_id": ques_id, "pred_ans": pred_answer, "gt_ans": gt_answer}
+            )
 
         return pred_qa_pairs
-        
+
     @dist_utils.main_process
     def _report_metrics(self, result_file, split):
         """
-        TODO: add other evaluation metrics for GQA
+        Implementing accuracy computation for AOKVQA, see
+        https://github.com/allenai/aokvqa/blob/main/evaluation/eval_predictions.py#L45 for details.
         """
+        # TODO add evaluation for multi-choice
 
         results = json.load(open(result_file, "r"))
         acc = []
-        vqa_tool = VQAEval()
 
         for res in results:
             if res["gt_ans"] is None:
                 # prepare test results for leaderboard evaluation
                 self._save_result_leaderboard(results)
                 return
 
-            gt_ans = res["gt_ans"]
             pred = res["pred_ans"]
+            gt_ans = res["gt_ans"]
 
-            if self.inference_method == "generate":
-                pred = vqa_tool.processPunctuation(pred)
-                pred = vqa_tool.processDigitArticle(pred)
-
-            vqa_acc = 1 if pred == gt_ans else 0
+            num_match = sum([pred == gt for gt in gt_ans])
+            vqa_acc = min(1.0, num_match / 3.0)
 
             acc.append(vqa_acc)
 
         accuracy = sum(acc) / len(acc) * 100
         metrics = {"agg_metrics": accuracy, "acc": accuracy}
 
         with open(
             os.path.join(registry.get_path("output_dir"), "evaluate.txt"), "a"
         ) as f:
             f.write(json.dumps(metrics) + "\n")
 
         logging.info(metrics)
 
         return metrics
-        
 
-@registry.register_task("aok_vqa")
-class AOKVQATask(VQATask):
+    @dist_utils.main_process
+    def _save_result_leaderboard(self, results):
+        """
+        Saving the results in the format required for leaderboard evaluation.
+
+        [TODO] add support for multi-choice.
+        """
+        result_leaderboard = dict()
+        for res in results:
+            result_leaderboard[res["question_id"]] = {
+                "direct_answer": res["pred_ans"],
+                "multiple_choice": "",
+            }
+
+        result_file = registry.get_path("result_dir") + "_leaderboard.json"
+
+        with open(result_file, "w") as f:
+            json.dump(result_leaderboard, f)
+
+        logging.info(f"Saved results for leaderboard evaluation at {result_file}")
+
+
+
+@registry.register_task("gqa")
+class GQATask(VQATask):
     def valid_step(self, model, samples):
         answers = model.predict_answers(
             samples=samples,
             answer_list=self.answer_list,
             inference_method=self.inference_method,
             num_beams=self.num_beams,
             max_len=self.max_len,
             min_len=self.min_len,
             num_ans_candidates=self.num_ans_candidates,
+            prompt=self.prompt,
         )
-
         pred_qa_pairs = []
 
         question_id = samples["question_id"]
-        gt_answers = samples["direct_answers"]
-
-        for pred_answer, ques_id, gt_answer in zip(answers, question_id, gt_answers):
-            pred_qa_pairs.append(
-                {"question_id": ques_id, "pred_ans": pred_answer, "gt_ans": gt_answer}
-            )
+        gt_answers = samples["answer"]
+        
+        for answer, ques_id, gt_answer in zip(answers, question_id, gt_answers):
+            ques_id = int(ques_id.item()) if isinstance(ques_id, torch.Tensor) else ques_id
+            pred_qa_pairs.append({"question_id": ques_id, "pred_ans": answer, "gt_ans": gt_answer})
 
         return pred_qa_pairs
+    
+    def build_datasets(self, cfg):
+        datasets = BaseTask.build_datasets(self,cfg)
 
+        # get question file, annotation file and anwser list in COCO format
+        for ds_name, dataset in datasets.items():
+            for split in dataset:
+                if (
+                    hasattr(dataset[split], "coco_fmt_qust_file")
+                    and dataset[split].coco_fmt_qust_file is not None
+                ):
+                    self.ques_files[split] = dataset[split].coco_fmt_qust_file
+                    self.anno_files[split] = dataset[split].coco_fmt_anno_file
+
+        if len(self.ques_files) > 0:
+            assert len(self.ques_files) == len(
+                self.anno_files
+            ), "Only support one split for evaluation."
+
+        return datasets
+        
     @dist_utils.main_process
     def _report_metrics(self, result_file, split):
         """
-        Implementing accuracy computation for AOKVQA, see
-        https://github.com/allenai/aokvqa/blob/main/evaluation/eval_predictions.py#L45 for details.
+        TODO: add other evaluation metrics for GQA
         """
-        # TODO add evaluation for multi-choice
 
         results = json.load(open(result_file, "r"))
         acc = []
+        vqa_tool = VQAEval()
 
         for res in results:
             if res["gt_ans"] is None:
                 # prepare test results for leaderboard evaluation
                 self._save_result_leaderboard(results)
                 return
 
-            pred = res["pred_ans"]
             gt_ans = res["gt_ans"]
+            pred = res["pred_ans"]
 
-            num_match = sum([pred == gt for gt in gt_ans])
-            vqa_acc = min(1.0, num_match / 3.0)
+            # if self.inference_method == "generate":
+            pred = vqa_tool.processPunctuation(pred)
+            pred = vqa_tool.processDigitArticle(pred)
+
+            # added to ensure that the ground truth format of answers is as expected for non-gqa but similar tasks
+            gt_ans = vqa_tool.processPunctuation(gt_ans)
+            gt_ans = vqa_tool.processDigitArticle(gt_ans)
+
+            vqa_acc = 1 if pred == gt_ans else 0
 
             acc.append(vqa_acc)
 
         accuracy = sum(acc) / len(acc) * 100
         metrics = {"agg_metrics": accuracy, "acc": accuracy}
 
         with open(
@@ -288,27 +401,79 @@
         ) as f:
             f.write(json.dumps(metrics) + "\n")
 
         logging.info(metrics)
 
         return metrics
 
+
+@registry.register_task("discrn_qa")
+class DisCRNTask(VQATask):
+    def valid_step(self, model, samples):
+        answers = model.predict_answers(
+            samples=samples,
+            answer_list=self.answer_list,
+            inference_method=self.inference_method,
+            num_beams=self.num_beams,
+            max_len=self.max_len,
+            min_len=self.min_len,
+            num_ans_candidates=self.num_ans_candidates,
+            prompt=self.prompt,
+        )
+
+        if answers == None: # corrupt videos
+            return []
+            
+        pred_qa_pairs = []
+
+        question_id = samples["question_id"]
+        gt_answers = samples["answer"]
+        
+        for answer, ques_id, gt_answer in zip(answers, question_id, gt_answers):
+            ques_id = int(ques_id.item()) if isinstance(ques_id, torch.Tensor) else ques_id
+            pred_qa_pairs.append({"question_id": ques_id, "pred_ans": answer, "gt_ans": gt_answer})
+
+        return pred_qa_pairs
+
+
+    def build_datasets(self, cfg):
+        datasets = BaseTask.build_datasets(self, cfg)
+        return datasets
+        
     @dist_utils.main_process
-    def _save_result_leaderboard(self, results):
-        """
-        Saving the results in the format required for leaderboard evaluation.
+    def _report_metrics(self, result_file, split):
+        results = json.load(open(result_file, "r"))
+        acc = []
+        vqa_tool = VQAEval()
 
-        [TODO] add support for multi-choice.
-        """
-        result_leaderboard = dict()
         for res in results:
-            result_leaderboard[res["question_id"]] = {
-                "direct_answer": res["pred_ans"],
-                "multiple_choice": "",
-            }
+            gt_ans = res["gt_ans"]
+            pred = res["pred_ans"]
+            
+            # gt_ans = [vqa_tool.processPunctuation(g) for g in gt_ans]
+            # gt_ans = [vqa_tool.processDigitArticle(g) for g in gt_ans]
+
+            # if self.inference_method == "generate":
+            pred = vqa_tool.processPunctuation(pred)
+            pred = vqa_tool.processDigitArticle(pred)
+
+            tokenized_pred = pred.strip().split(" ")
+            for ans in gt_ans:
+                if ans in tokenized_pred:
+                    pred = ans
+                    break
 
-        result_file = registry.get_path("result_dir") + "_leaderboard.json"
+            vqa_acc = 1 if pred in gt_ans else 0
 
-        with open(result_file, "w") as f:
-            json.dump(result_leaderboard, f)
+            acc.append(vqa_acc)
 
-        logging.info(f"Saved results for leaderboard evaluation at {result_file}")
+        accuracy = sum(acc) / len(acc) * 100
+        metrics = {"agg_metrics": accuracy, "acc": accuracy}
+
+        with open(
+            os.path.join(registry.get_path("output_dir"), "evaluate.txt"), "a"
+        ) as f:
+            f.write(json.dumps(metrics) + "\n")
+
+        logging.info(metrics)
+
+        return metrics
```

## Comparing `projects/img2prompt-vqa/img2prompt_vqa.py` & `build/lib/projects/img2llm-vqa/img2llm_vqa.py`

 * *Files identical despite different names*

## Comparing `lavis_gml-1.0.2.post3.dist-info/LICENSE.txt` & `lavis_gml-1.0.3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `lavis_gml-1.0.2.post3.dist-info/METADATA` & `lavis_gml-1.0.3.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: lavis-gml
-Version: 1.0.2.post3
+Version: 1.0.3
 Summary: LAVIS - A One-stop Library for Language-Vision Intelligence
 Home-page: https://github.com/gimletlabs/LAVIS
 Author: Dongxu Li, Junnan Li, Hung Le, Guangsen Wang, Silvio Savarese, Steven C.H. Hoi
 License: 3-Clause BSD
 Keywords: Vision-Language,Multimodal,Image Captioning,Generative AI,Deep Learning,Library,PyTorch
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: contexttimer
 Requires-Dist: decord
+Requires-Dist: diffusers <=0.16.0
 Requires-Dist: einops >=0.4.1
 Requires-Dist: fairscale ==0.4.4
 Requires-Dist: ftfy
 Requires-Dist: iopath
 Requires-Dist: ipython
 Requires-Dist: omegaconf
 Requires-Dist: opencv-python-headless ==4.5.5.64
@@ -29,17 +30,26 @@
 Requires-Dist: scikit-image
 Requires-Dist: sentencepiece
 Requires-Dist: streamlit
 Requires-Dist: timm ==0.4.12
 Requires-Dist: torch >=1.10.0
 Requires-Dist: torchvision
 Requires-Dist: tqdm
-Requires-Dist: transformers <4.27,>=4.25.0
+Requires-Dist: transformers ==4.33.2
 Requires-Dist: webdataset
 Requires-Dist: wheel
+Requires-Dist: torchaudio
+Requires-Dist: soundfile
+Requires-Dist: moviepy
+Requires-Dist: nltk
+Requires-Dist: peft
+Requires-Dist: easydict ==1.9
+Requires-Dist: pyyaml-env-tag ==0.1
+Requires-Dist: open3d ==0.13.0
+Requires-Dist: h5py
 
 <p align="center">
     <br>
     <img src="docs/_static/logo_final.png" width="400"/>
     <br>
 <p>
 
@@ -62,25 +72,59 @@
 <a href="https://github.com/salesforce/LAVIS/tree/main/examples">Jupyter Notebook Examples</a>,
 <a href="https://blog.salesforceairesearch.com/lavis-language-vision-library/">Blog</a>
 </div>
 
 # LAVIS - A Library for Language-Vision Intelligence
 
 ## What's New: 🎉 
+  * [Model Release] November 2023, released implementation of **X-InstructBLIP** <br>
+  [Paper](https://arxiv.org/pdf/2311.18799.pdf), [Project Page](https://github.com/salesforce/LAVIS/tree/main/projects/xinstructblip), [Website](https://artemisp.github.io/X-InstructBLIP-page/), [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/salesforce/LAVIS/blob/main/projects/xinstructblip/demo/run_demo.ipynb)
+  > A simple, yet effective, cross-modality framework built atop frozen LLMs that allows the integration of various modalities (image, video, audio, 3D) without extensive modality-specific customization.
+  * [Model Release] July 2023, released implementation of **BLIP-Diffusion** <br>
+  [Paper](https://arxiv.org/abs/2305.06500), [Project Page](https://github.com/salesforce/LAVIS/tree/main/projects/blip-diffusion), [Website](https://dxli94.github.io/BLIP-Diffusion-website/)
+  > A text-to-image generation model that trains 20x than DreamBooth. Also facilitates zero-shot subject-driven generation and editing.
+  * [Model Release] May 2023, released implementation of **InstructBLIP** <br>
+  [Paper](https://arxiv.org/abs/2305.06500), [Project Page](https://github.com/salesforce/LAVIS/tree/main/projects/instructblip)    
+  > A new vision-language instruction-tuning framework using BLIP-2 models, achieving state-of-the-art zero-shot generalization performance on a wide range of vision-language tasks.
   * [Model Release] Jan 2023, released implementation of **BLIP-2** <br>
-  [Paper](https://arxiv.org/abs/2301.12597), [Project Page](https://github.com/salesforce/LAVIS/tree/main/projects/blip2), [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/Salesforce/BLIP2), [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/salesforce/LAVIS/blob/main/examples/blip2_instructed_generation.ipynb)
+  [Paper](https://arxiv.org/abs/2301.12597), [Project Page](https://github.com/salesforce/LAVIS/tree/main/projects/blip2), [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/salesforce/LAVIS/blob/main/examples/blip2_instructed_generation.ipynb)
   > A generic and efficient pre-training strategy that easily harvests development of pretrained vision models and large language models (LLMs) for vision-language pretraining. BLIP-2 beats Flamingo on zero-shot VQAv2 (**65.0** vs **56.3**), establishing new state-of-the-art on zero-shot captioning (on NoCaps **121.6** CIDEr score vs previous best **113.2**). In addition, equipped with powerful LLMs (e.g. OPT, FlanT5), BLIP-2 also unlocks the new **zero-shot instructed vision-to-language generation** capabilities for various interesting applications!
   * Jan 2023, LAVIS is now available on [PyPI](https://pypi.org/project/salesforce-lavis/) for installation!
-  * [Model Release] Dec 2022, released implementation of **Img2prompt-VQA** <br>
-  [Paper](https://arxiv.org/pdf/2212.10846.pdf), [Project Page](https://github.com/salesforce/LAVIS/tree/main/projects/img2prompt-vqa), [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/salesforce/LAVIS/blob/main/projects/img2prompt-vqa/img2prompt_vqa.ipynb)
-  > A plug-and-play module that enables off-the-shelf use of Large Language Models (LLMs) for visual question answering (VQA). Img2Prompt-VQA surpasses Flamingo on zero-shot VQA on VQAv2 (61.9 vs 56.3), while in contrast requiring no end-to-end training! 
+  * [Model Release] Dec 2022, released implementation of **Img2LLM-VQA** (**CVPR 2023**, _"From Images to Textual Prompts: Zero-shot VQA with Frozen Large Language Models"_, by Jiaxian Guo et al) <br>
+  [Paper](https://arxiv.org/pdf/2212.10846.pdf), [Project Page](https://github.com/salesforce/LAVIS/tree/main/projects/img2llm-vqa), [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/salesforce/LAVIS/blob/main/projects/img2llm-vqa/img2llm_vqa.ipynb)
+  > A plug-and-play module that enables off-the-shelf use of Large Language Models (LLMs) for visual question answering (VQA). Img2LLM-VQA surpasses Flamingo on zero-shot VQA on VQAv2 (61.9 vs 56.3), while in contrast requiring no end-to-end training! 
   * [Model Release] Oct 2022, released implementation of **PNP-VQA** (**EMNLP Findings 2022**, _"Plug-and-Play VQA: Zero-shot VQA by Conjoining Large Pretrained Models with Zero Training"_, by Anthony T.M.H. et al), <br> 
   [Paper](https://arxiv.org/abs/2210.08773), [Project Page](https://github.com/salesforce/LAVIS/tree/main/projects/pnp-vqa), [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/salesforce/LAVIS/blob/main/projects/pnp-vqa/pnp_vqa.ipynb))
   >  A modular zero-shot VQA framework that requires no PLMs training, achieving SoTA zero-shot VQA performance. 
-    
+
+## Technical Report and Citing LAVIS
+You can find more details in our [technical report](https://arxiv.org/abs/2209.09019).
+
+**If you're using LAVIS in your research or applications, please cite it using this BibTeX**:
+```bibtex
+@inproceedings{li-etal-2023-lavis,
+    title = "{LAVIS}: A One-stop Library for Language-Vision Intelligence",
+    author = "Li, Dongxu  and
+      Li, Junnan  and
+      Le, Hung  and
+      Wang, Guangsen  and
+      Savarese, Silvio  and
+      Hoi, Steven C.H.",
+    booktitle = "Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 3: System Demonstrations)",
+    month = jul,
+    year = "2023",
+    address = "Toronto, Canada",
+    publisher = "Association for Computational Linguistics",
+    url = "https://aclanthology.org/2023.acl-demo.3",
+    pages = "31--41",
+    abstract = "We introduce LAVIS, an open-source deep learning library for LAnguage-VISion research and applications. LAVIS aims to serve as a one-stop comprehensive library that brings recent advancements in the language-vision field accessible for researchers and practitioners, as well as fertilizing future research and development. It features a unified interface to easily access state-of-the-art image-language, video-language models and common datasets. LAVIS supports training, evaluation and benchmarking on a rich variety of tasks, including multimodal classification, retrieval, captioning, visual question answering, dialogue and pre-training. In the meantime, the library is also highly extensible and configurable, facilitating future development and customization. In this technical report, we describe design principles, key components and functionalities of the library, and also present benchmarking results across common language-vision tasks.",
+}
+```
+
+
 ## Table of Contents
   - [Introduction](#introduction)
   - [Installation](#installation)
   - [Getting Started](#getting-started)
     - [Model Zoo](#model-zoo)
     - [Image Captioning](#image-captioning)
     - [Visual question answering (VQA)](#visual-question-answering-vqa)
@@ -322,27 +366,12 @@
 [documentation](https://opensource.salesforce.com/LAVIS//latest/index.html#).
 
 ## Ethical and Responsible Use
 We note that models in LAVIS provide no guarantees on their multimodal abilities; incorrect or biased predictions may be observed. In particular, the datasets and pretrained models utilized in LAVIS may contain socioeconomic biases which could result in misclassification and other unwanted behaviors such as offensive or inappropriate speech. We strongly recommend that users review the pre-trained models and overall system in LAVIS before practical adoption. We plan to improve the library by investigating and mitigating these potential biases and
 inappropriate behaviors in the future.
 
 
-## Technical Report and Citing LAVIS
-You can find more details in our [technical report](https://arxiv.org/abs/2209.09019).
-
-If you're using LAVIS in your research or applications, please cite using this BibTeX:
-```bibtex
-@misc{li2022lavis,
-      title={LAVIS: A Library for Language-Vision Intelligence}, 
-      author={Dongxu Li and Junnan Li and Hung Le and Guangsen Wang and Silvio Savarese and Steven C. H. Hoi},
-      year={2022},
-      eprint={2209.09019},
-      archivePrefix={arXiv},
-      primaryClass={cs.CV}
-}
-```
-
 ## Contact us
 If you have any questions, comments or suggestions, please do not hesitate to contact us at lavis@salesforce.com.
 
 ## License
 [BSD 3-Clause License](LICENSE.txt)
```

### html2text {}

```diff
@@ -1,82 +1,127 @@
-Metadata-Version: 2.1 Name: lavis-gml Version: 1.0.2.post3 Summary: LAVIS - A
-One-stop Library for Language-Vision Intelligence Home-page: https://
-github.com/gimletlabs/LAVIS Author: Dongxu Li, Junnan Li, Hung Le, Guangsen
-Wang, Silvio Savarese, Steven C.H. Hoi License: 3-Clause BSD Keywords: Vision-
+Metadata-Version: 2.1 Name: lavis-gml Version: 1.0.3 Summary: LAVIS - A One-
+stop Library for Language-Vision Intelligence Home-page: https://github.com/
+gimletlabs/LAVIS Author: Dongxu Li, Junnan Li, Hung Le, Guangsen Wang, Silvio
+Savarese, Steven C.H. Hoi License: 3-Clause BSD Keywords: Vision-
 Language,Multimodal,Image Captioning,Generative AI,Deep
 Learning,Library,PyTorch Requires-Python: >=3.7.0 Description-Content-Type:
 text/markdown License-File: LICENSE.txt Requires-Dist: contexttimer Requires-
-Dist: decord Requires-Dist: einops >=0.4.1 Requires-Dist: fairscale ==0.4.4
-Requires-Dist: ftfy Requires-Dist: iopath Requires-Dist: ipython Requires-Dist:
-omegaconf Requires-Dist: opencv-python-headless ==4.5.5.64 Requires-Dist:
-opendatasets Requires-Dist: packaging Requires-Dist: pandas Requires-Dist:
-plotly Requires-Dist: pre-commit Requires-Dist: pycocoevalcap Requires-Dist:
-pycocotools Requires-Dist: python-magic Requires-Dist: scikit-image Requires-
-Dist: sentencepiece Requires-Dist: streamlit Requires-Dist: timm ==0.4.12
-Requires-Dist: torch >=1.10.0 Requires-Dist: torchvision Requires-Dist: tqdm
-Requires-Dist: transformers <4.27,>=4.25.0 Requires-Dist: webdataset Requires-
-Dist: wheel
+Dist: decord Requires-Dist: diffusers <=0.16.0 Requires-Dist: einops >=0.4.1
+Requires-Dist: fairscale ==0.4.4 Requires-Dist: ftfy Requires-Dist: iopath
+Requires-Dist: ipython Requires-Dist: omegaconf Requires-Dist: opencv-python-
+headless ==4.5.5.64 Requires-Dist: opendatasets Requires-Dist: packaging
+Requires-Dist: pandas Requires-Dist: plotly Requires-Dist: pre-commit Requires-
+Dist: pycocoevalcap Requires-Dist: pycocotools Requires-Dist: python-magic
+Requires-Dist: scikit-image Requires-Dist: sentencepiece Requires-Dist:
+streamlit Requires-Dist: timm ==0.4.12 Requires-Dist: torch >=1.10.0 Requires-
+Dist: torchvision Requires-Dist: tqdm Requires-Dist: transformers ==4.33.2
+Requires-Dist: webdataset Requires-Dist: wheel Requires-Dist: torchaudio
+Requires-Dist: soundfile Requires-Dist: moviepy Requires-Dist: nltk Requires-
+Dist: peft Requires-Dist: easydict ==1.9 Requires-Dist: pyyaml-env-tag ==0.1
+Requires-Dist: open3d ==0.13.0 Requires-Dist: h5py
 
                          [docs/_static/logo_final.png]
                   _[_L_a_t_e_s_t_ _R_e_l_e_a_s_e_]_[_d_o_c_s_]_[_l_i_c_e_n_s_e_]_[_D_o_w_n_l_o_a_d_s_]
   _B_e_n_c_h_m_a_r_k, _T_e_c_h_n_i_c_a_l_ _R_e_p_o_r_t, _D_o_c_u_m_e_n_t_a_t_i_o_n, _J_u_p_y_t_e_r_ _N_o_t_e_b_o_o_k_ _E_x_a_m_p_l_e_s, _B_l_o_g
 # LAVIS - A Library for Language-Vision Intelligence ## What's New: ð *
-[Model Release] Jan 2023, released implementation of **BLIP-2**
+[Model Release] November 2023, released implementation of **X-InstructBLIP**
+[Paper](https://arxiv.org/pdf/2311.18799.pdf), [Project Page](https://
+github.com/salesforce/LAVIS/tree/main/projects/xinstructblip), [Website](https:
+//artemisp.github.io/X-InstructBLIP-page/), [![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/github/salesforce/LAVIS/blob/main/projects/
+xinstructblip/demo/run_demo.ipynb) > A simple, yet effective, cross-modality
+framework built atop frozen LLMs that allows the integration of various
+modalities (image, video, audio, 3D) without extensive modality-specific
+customization. * [Model Release] July 2023, released implementation of **BLIP-
+Diffusion**
+[Paper](https://arxiv.org/abs/2305.06500), [Project Page](https://github.com/
+salesforce/LAVIS/tree/main/projects/blip-diffusion), [Website](https://
+dxli94.github.io/BLIP-Diffusion-website/) > A text-to-image generation model
+that trains 20x than DreamBooth. Also facilitates zero-shot subject-driven
+generation and editing. * [Model Release] May 2023, released implementation of
+**InstructBLIP**
+[Paper](https://arxiv.org/abs/2305.06500), [Project Page](https://github.com/
+salesforce/LAVIS/tree/main/projects/instructblip) > A new vision-language
+instruction-tuning framework using BLIP-2 models, achieving state-of-the-art
+zero-shot generalization performance on a wide range of vision-language tasks.
+* [Model Release] Jan 2023, released implementation of **BLIP-2**
 [Paper](https://arxiv.org/abs/2301.12597), [Project Page](https://github.com/
-salesforce/LAVIS/tree/main/projects/blip2), [![Hugging Face Spaces](https://
-img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://
-huggingface.co/spaces/Salesforce/BLIP2), [![Open In Colab](https://
+salesforce/LAVIS/tree/main/projects/blip2), [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/salesforce/LAVIS/blob/main/examples/
 blip2_instructed_generation.ipynb) > A generic and efficient pre-training
 strategy that easily harvests development of pretrained vision models and large
 language models (LLMs) for vision-language pretraining. BLIP-2 beats Flamingo
 on zero-shot VQAv2 (**65.0** vs **56.3**), establishing new state-of-the-art on
 zero-shot captioning (on NoCaps **121.6** CIDEr score vs previous best
 **113.2**). In addition, equipped with powerful LLMs (e.g. OPT, FlanT5), BLIP-
 2 also unlocks the new **zero-shot instructed vision-to-language generation**
 capabilities for various interesting applications! * Jan 2023, LAVIS is now
 available on [PyPI](https://pypi.org/project/salesforce-lavis/) for
-installation! * [Model Release] Dec 2022, released implementation of
-**Img2prompt-VQA**
+installation! * [Model Release] Dec 2022, released implementation of **Img2LLM-
+VQA** (**CVPR 2023**, _"From Images to Textual Prompts: Zero-shot VQA with
+Frozen Large Language Models"_, by Jiaxian Guo et al)
 [Paper](https://arxiv.org/pdf/2212.10846.pdf), [Project Page](https://
-github.com/salesforce/LAVIS/tree/main/projects/img2prompt-vqa), [![Open In
-Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/github/salesforce/LAVIS/blob/main/projects/
-img2prompt-vqa/img2prompt_vqa.ipynb) > A plug-and-play module that enables off-
-the-shelf use of Large Language Models (LLMs) for visual question answering
-(VQA). Img2Prompt-VQA surpasses Flamingo on zero-shot VQA on VQAv2 (61.9 vs
-56.3), while in contrast requiring no end-to-end training! * [Model Release]
-Oct 2022, released implementation of **PNP-VQA** (**EMNLP Findings 2022**,
-_"Plug-and-Play VQA: Zero-shot VQA by Conjoining Large Pretrained Models with
-Zero Training"_, by Anthony T.M.H. et al),
+github.com/salesforce/LAVIS/tree/main/projects/img2llm-vqa), [![Open In Colab]
+(https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/github/salesforce/LAVIS/blob/main/projects/img2llm-
+vqa/img2llm_vqa.ipynb) > A plug-and-play module that enables off-the-shelf use
+of Large Language Models (LLMs) for visual question answering (VQA). Img2LLM-
+VQA surpasses Flamingo on zero-shot VQA on VQAv2 (61.9 vs 56.3), while in
+contrast requiring no end-to-end training! * [Model Release] Oct 2022, released
+implementation of **PNP-VQA** (**EMNLP Findings 2022**, _"Plug-and-Play VQA:
+Zero-shot VQA by Conjoining Large Pretrained Models with Zero Training"_, by
+Anthony T.M.H. et al),
 [Paper](https://arxiv.org/abs/2210.08773), [Project Page](https://github.com/
 salesforce/LAVIS/tree/main/projects/pnp-vqa), [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/salesforce/LAVIS/blob/main/projects/pnp-vqa/
 pnp_vqa.ipynb)) > A modular zero-shot VQA framework that requires no PLMs
-training, achieving SoTA zero-shot VQA performance. ## Table of Contents -
-[Introduction](#introduction) - [Installation](#installation) - [Getting
-Started](#getting-started) - [Model Zoo](#model-zoo) - [Image Captioning]
-(#image-captioning) - [Visual question answering (VQA)](#visual-question-
-answering-vqa) - [Unified Feature Extraction Interface](#unified-feature-
-extraction-interface) - [Load Datasets](#load-datasets) - [Jupyter Notebook
-Examples](#jupyter-notebook-examples) - [Resources and Tools](#resources-and-
-tools) - [Documentations](#documentations) - [Ethical and Responsible Use]
-(#ethical-and-responsible-use) - [Technical Report and Citing LAVIS]
-(#technical-report-and-citing-lavis) - [License](#license) ## Introduction
-LAVIS is a Python deep learning library for LAnguage-and-VISion intelligence
-research and applications. This library aims to provide engineers and
-researchers with a one-stop solution to rapidly develop models for their
-specific multimodal scenarios, and benchmark them across standard and
-customized datasets. It features a unified interface design to access - **10+**
-tasks (retrieval, captioning, visual question answering, multimodal
-classification etc.); - **20+** datasets (COCO, Flickr, Nocaps, Conceptual
-Commons, SBU, etc.); - **30+** pretrained weights of state-of-the-art
-foundation language-vision models and their task-specific adaptations,
+training, achieving SoTA zero-shot VQA performance. ## Technical Report and
+Citing LAVIS You can find more details in our [technical report](https://
+arxiv.org/abs/2209.09019). **If you're using LAVIS in your research or
+applications, please cite it using this BibTeX**: ```bibtex @inproceedings{li-
+etal-2023-lavis, title = "{LAVIS}: A One-stop Library for Language-Vision
+Intelligence", author = "Li, Dongxu and Li, Junnan and Le, Hung and Wang,
+Guangsen and Savarese, Silvio and Hoi, Steven C.H.", booktitle = "Proceedings
+of the 61st Annual Meeting of the Association for Computational Linguistics
+(Volume 3: System Demonstrations)", month = jul, year = "2023", address =
+"Toronto, Canada", publisher = "Association for Computational Linguistics", url
+= "https://aclanthology.org/2023.acl-demo.3", pages = "31--41", abstract = "We
+introduce LAVIS, an open-source deep learning library for LAnguage-VISion
+research and applications. LAVIS aims to serve as a one-stop comprehensive
+library that brings recent advancements in the language-vision field accessible
+for researchers and practitioners, as well as fertilizing future research and
+development. It features a unified interface to easily access state-of-the-art
+image-language, video-language models and common datasets. LAVIS supports
+training, evaluation and benchmarking on a rich variety of tasks, including
+multimodal classification, retrieval, captioning, visual question answering,
+dialogue and pre-training. In the meantime, the library is also highly
+extensible and configurable, facilitating future development and customization.
+In this technical report, we describe design principles, key components and
+functionalities of the library, and also present benchmarking results across
+common language-vision tasks.", } ``` ## Table of Contents - [Introduction]
+(#introduction) - [Installation](#installation) - [Getting Started](#getting-
+started) - [Model Zoo](#model-zoo) - [Image Captioning](#image-captioning) -
+[Visual question answering (VQA)](#visual-question-answering-vqa) - [Unified
+Feature Extraction Interface](#unified-feature-extraction-interface) - [Load
+Datasets](#load-datasets) - [Jupyter Notebook Examples](#jupyter-notebook-
+examples) - [Resources and Tools](#resources-and-tools) - [Documentations]
+(#documentations) - [Ethical and Responsible Use](#ethical-and-responsible-use)
+- [Technical Report and Citing LAVIS](#technical-report-and-citing-lavis) -
+[License](#license) ## Introduction LAVIS is a Python deep learning library for
+LAnguage-and-VISion intelligence research and applications. This library aims
+to provide engineers and researchers with a one-stop solution to rapidly
+develop models for their specific multimodal scenarios, and benchmark them
+across standard and customized datasets. It features a unified interface design
+to access - **10+** tasks (retrieval, captioning, visual question answering,
+multimodal classification etc.); - **20+** datasets (COCO, Flickr, Nocaps,
+Conceptual Commons, SBU, etc.); - **30+** pretrained weights of state-of-the-
+art foundation language-vision models and their task-specific adaptations,
 including [ALBEF](https://arxiv.org/pdf/2107.07651.pdf), [BLIP](https://
 arxiv.org/pdf/2201.12086.pdf), [ALPRO](https://arxiv.org/pdf/2112.09583.pdf),
 [CLIP](https://arxiv.org/pdf/2103.00020.pdf).
 
                               [assets/demo-6.png]
 Key features of LAVIS include: - **Unified and Modular Interface**:
 facilitating to easily leverage and repurpose existing modules (datasets,
@@ -206,16 +251,10 @@
 multimodal abilities; incorrect or biased predictions may be observed. In
 particular, the datasets and pretrained models utilized in LAVIS may contain
 socioeconomic biases which could result in misclassification and other unwanted
 behaviors such as offensive or inappropriate speech. We strongly recommend that
 users review the pre-trained models and overall system in LAVIS before
 practical adoption. We plan to improve the library by investigating and
 mitigating these potential biases and inappropriate behaviors in the future. ##
-Technical Report and Citing LAVIS You can find more details in our [technical
-report](https://arxiv.org/abs/2209.09019). If you're using LAVIS in your
-research or applications, please cite using this BibTeX: ```bibtex @misc
-{li2022lavis, title={LAVIS: A Library for Language-Vision Intelligence},
-author={Dongxu Li and Junnan Li and Hung Le and Guangsen Wang and Silvio
-Savarese and Steven C. H. Hoi}, year={2022}, eprint={2209.09019},
-archivePrefix={arXiv}, primaryClass={cs.CV} } ``` ## Contact us If you have any
-questions, comments or suggestions, please do not hesitate to contact us at
-lavis@salesforce.com. ## License [BSD 3-Clause License](LICENSE.txt)
+Contact us If you have any questions, comments or suggestions, please do not
+hesitate to contact us at lavis@salesforce.com. ## License [BSD 3-Clause
+License](LICENSE.txt)
```

