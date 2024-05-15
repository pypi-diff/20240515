# Comparing `tmp/imt_ring-1.3.4.tar.gz` & `tmp/imt_ring-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imt_ring-1.3.4.tar", last modified: Mon Apr 29 22:14:10 2024, max compression
+gzip compressed data, was "imt_ring-1.3.5.tar", last modified: Wed May 15 14:41:38 2024, max compression
```

## Comparing `imt_ring-1.3.4.tar` & `imt_ring-1.3.5.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:14:10.213203 imt_ring-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-29 22:14:10.213203 imt_ring-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-29 22:14:06.000000 imt_ring-1.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-29 22:14:06.000000 imt_ring-1.3.4/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-29 22:14:10.213203 imt_ring-1.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:14:10.181203 imt_ring-1.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:14:10.213203 imt_ring-1.3.4/src/imt_ring.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-29 22:14:10.000000 imt_ring-1.3.4/src/imt_ring.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-29 22:14:10.000000 imt_ring-1.3.4/src/imt_ring.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 22:14:10.000000 imt_ring-1.3.4/src/imt_ring.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-29 22:14:10.000000 imt_ring-1.3.4/src/imt_ring.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-29 22:14:10.000000 imt_ring-1.3.4/src/imt_ring.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:14:10.185203 imt_ring-1.3.4/src/ring/
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/algebra.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:14:10.185203 imt_ring-1.3.4/src/ring/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13340 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/algorithms/_random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:14:10.189203 imt_ring-1.3.4/src/ring/algorithms/custom_joints/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/algorithms/custom_joints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/algorithms/custom_joints/rr_imp_joint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/algorithms/custom_joints/rr_joint.py
--rw-r--r--   0 runner    (1001) docker     (127)    15858 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/algorithms/custom_joints/suntay.py
--rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/algorithms/dynamics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:14:10.189203 imt_ring-1.3.4/src/ring/algorithms/generator/
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/algorithms/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14771 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/algorithms/generator/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9019 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/algorithms/generator/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/algorithms/generator/motion_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/algorithms/generator/pd_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/algorithms/generator/randomize.py
--rw-r--r--   0 runner    (1001) docker     (127)    12782 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/algorithms/generator/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/algorithms/generator/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    28213 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/algorithms/jcalc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7422 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/algorithms/kinematics.py
--rw-r--r--   0 runner    (1001) docker     (127)    18005 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/algorithms/sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)    33705 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:14:10.189203 imt_ring-1.3.4/src/ring/io/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:14:10.193203 imt_ring-1.3.4/src/ring/io/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/io/examples/branched.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:14:10.193203 imt_ring-1.3.4/src/ring/io/examples/exclude/
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/io/examples/exclude/knee_trans_dof.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/io/examples/exclude/standard_sys.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9015 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/io/examples/exclude/standard_sys_rr_imp.xml
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/io/examples/inv_pendulum.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/io/examples/knee_flexible_imus.xml
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/io/examples/spherical_stiff.xml
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/io/examples/symmetric.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/io/examples/test_all_1.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/io/examples/test_all_2.xml
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/io/examples/test_ang0_pos0.xml
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/io/examples/test_control.xml
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/io/examples/test_double_pendulum.xml
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/io/examples/test_free.xml
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/io/examples/test_kinematics.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:14:10.193203 imt_ring-1.3.4/src/ring/io/examples/test_morph_system/
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/io/examples/test_morph_system/four_seg_seg1.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/io/examples/test_morph_system/four_seg_seg3.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/io/examples/test_randomize_position.xml
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/io/examples/test_sensors.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/io/examples/test_three_seg_seg2.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/io/examples.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/io/test_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:14:10.193203 imt_ring-1.3.4/src/ring/io/xml/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/io/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/io/xml/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     9234 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/io/xml/from_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/io/xml/test_from_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/io/xml/test_to_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/io/xml/to_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)    12193 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/maths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:14:10.193203 imt_ring-1.3.4/src/ring/ml/
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/ml/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13253 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/ml/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/ml/ml_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/ml/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:14:10.193203 imt_ring-1.3.4/src/ring/ml/params/
--rw-r--r--   0 runner    (1001) docker     (127)  9355838 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/ml/params/0x13e3518065c21cd8.pickle
--rw-r--r--   0 runner    (1001) docker     (127)     8521 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/ml/ringnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    10872 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/ml/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/ml/training_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:14:10.205203 imt_ring-1.3.4/src/ring/rendering/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/rendering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/rendering/base_render.py
--rw-r--r--   0 runner    (1001) docker     (127)     7770 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/rendering/mujoco_render.py
--rw-r--r--   0 runner    (1001) docker     (127)    10260 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/rendering/vispy_render.py
--rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/rendering/vispy_visuals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:14:10.205203 imt_ring-1.3.4/src/ring/sim2real/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/sim2real/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/sim2real/sim2real.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/spatial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:14:10.209203 imt_ring-1.3.4/src/ring/sys_composer/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/sys_composer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/sys_composer/delete_sys.py
--rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/sys_composer/inject_sys.py
--rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/sys_composer/morph_sys.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:14:10.209203 imt_ring-1.3.4/src/ring/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/utils/batchsize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/utils/colab.py
--rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/utils/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/utils/normalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     5303 2024-04-29 22:14:06.000000 imt_ring-1.3.4/src/ring/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:14:10.213203 imt_ring-1.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-04-29 22:14:06.000000 imt_ring-1.3.4/tests/test_algebra.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-29 22:14:06.000000 imt_ring-1.3.4/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-29 22:14:06.000000 imt_ring-1.3.4/tests/test_custom_joints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-29 22:14:06.000000 imt_ring-1.3.4/tests/test_dynamics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-04-29 22:14:06.000000 imt_ring-1.3.4/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-29 22:14:06.000000 imt_ring-1.3.4/tests/test_jcalc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-29 22:14:06.000000 imt_ring-1.3.4/tests/test_jit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-04-29 22:14:06.000000 imt_ring-1.3.4/tests/test_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-29 22:14:06.000000 imt_ring-1.3.4/tests/test_maths.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-29 22:14:06.000000 imt_ring-1.3.4/tests/test_ml_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-29 22:14:06.000000 imt_ring-1.3.4/tests/test_motion_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-29 22:14:06.000000 imt_ring-1.3.4/tests/test_pd_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-29 22:14:06.000000 imt_ring-1.3.4/tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-29 22:14:06.000000 imt_ring-1.3.4/tests/test_randomize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-04-29 22:14:06.000000 imt_ring-1.3.4/tests/test_rcmg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-29 22:14:06.000000 imt_ring-1.3.4/tests/test_render.py
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-04-29 22:14:06.000000 imt_ring-1.3.4/tests/test_sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-04-29 22:14:06.000000 imt_ring-1.3.4/tests/test_sim2real.py
--rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-04-29 22:14:06.000000 imt_ring-1.3.4/tests/test_sys_composer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-29 22:14:06.000000 imt_ring-1.3.4/tests/test_train.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-29 22:14:06.000000 imt_ring-1.3.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.063777 imt_ring-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-15 14:41:38.063777 imt_ring-1.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-15 14:41:34.000000 imt_ring-1.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-15 14:41:34.000000 imt_ring-1.3.5/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-15 14:41:38.063777 imt_ring-1.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.027776 imt_ring-1.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.059776 imt_ring-1.3.5/src/imt_ring.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-15 14:41:38.000000 imt_ring-1.3.5/src/imt_ring.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-15 14:41:38.000000 imt_ring-1.3.5/src/imt_ring.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:41:38.000000 imt_ring-1.3.5/src/imt_ring.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-15 14:41:38.000000 imt_ring-1.3.5/src/imt_ring.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 14:41:38.000000 imt_ring-1.3.5/src/imt_ring.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.031776 imt_ring-1.3.5/src/ring/
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algebra.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.031776 imt_ring-1.3.5/src/ring/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13805 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algorithms/_random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.031776 imt_ring-1.3.5/src/ring/algorithms/custom_joints/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algorithms/custom_joints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algorithms/custom_joints/rr_imp_joint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algorithms/custom_joints/rr_joint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16215 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algorithms/custom_joints/suntay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algorithms/dynamics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.035776 imt_ring-1.3.5/src/ring/algorithms/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algorithms/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14771 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algorithms/generator/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9161 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algorithms/generator/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algorithms/generator/motion_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algorithms/generator/pd_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algorithms/generator/randomize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12782 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algorithms/generator/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algorithms/generator/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28260 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algorithms/jcalc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7422 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algorithms/kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18005 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algorithms/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33913 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.035776 imt_ring-1.3.5/src/ring/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.035776 imt_ring-1.3.5/src/ring/io/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/branched.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.039776 imt_ring-1.3.5/src/ring/io/examples/exclude/
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/exclude/knee_trans_dof.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/exclude/standard_sys.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9015 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/exclude/standard_sys_rr_imp.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/inv_pendulum.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/knee_flexible_imus.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/spherical_stiff.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/symmetric.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/test_all_1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/test_all_2.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/test_ang0_pos0.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/test_control.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/test_double_pendulum.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/test_free.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/test_kinematics.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.039776 imt_ring-1.3.5/src/ring/io/examples/test_morph_system/
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/test_morph_system/four_seg_seg1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/test_morph_system/four_seg_seg3.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/test_randomize_position.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/test_sensors.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/test_three_seg_seg2.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.039776 imt_ring-1.3.5/src/ring/io/xml/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/xml/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9234 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/xml/from_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/xml/test_from_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/xml/test_to_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/xml/to_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12193 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/maths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.039776 imt_ring-1.3.5/src/ring/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/ml/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13253 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/ml/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/ml/ml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/ml/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.039776 imt_ring-1.3.5/src/ring/ml/params/
+-rw-r--r--   0 runner    (1001) docker     (127)  9355838 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/ml/params/0x13e3518065c21cd8.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)     8521 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/ml/ringnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10872 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/ml/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/ml/training_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.055776 imt_ring-1.3.5/src/ring/rendering/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/rendering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/rendering/base_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7770 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/rendering/mujoco_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10260 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/rendering/vispy_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/rendering/vispy_visuals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.055776 imt_ring-1.3.5/src/ring/sim2real/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/sim2real/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/sim2real/sim2real.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/spatial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.055776 imt_ring-1.3.5/src/ring/sys_composer/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/sys_composer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/sys_composer/delete_sys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/sys_composer/inject_sys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/sys_composer/morph_sys.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.055776 imt_ring-1.3.5/src/ring/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/utils/batchsize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/utils/colab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/utils/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/utils/normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5303 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.059776 imt_ring-1.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_custom_joints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_jcalc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_jit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_maths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_ml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_motion_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_pd_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_randomize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_rcmg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_sim2real.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_sys_composer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_train.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_utils.py
```

### Comparing `imt_ring-1.3.4/PKG-INFO` & `imt_ring-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imt-ring
-Version: 1.3.4
+Version: 1.3.5
 Summary: RING: Recurrent Inertial Graph-based Estimator
 Author-email: Simon Bachhuber <simon.bachhuber@fau.de>
 Project-URL: Homepage, https://github.com/SimiPixel/ring
 Project-URL: Issues, https://github.com/SimiPixel/ring/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `imt_ring-1.3.4/pyproject.toml` & `imt_ring-1.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "imt-ring"
-version = "1.3.4"
+version = "1.3.5"
 authors = [
   { name="Simon Bachhuber", email="simon.bachhuber@fau.de" },
 ]
 description = "RING: Recurrent Inertial Graph-based Estimator"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `imt_ring-1.3.4/readme.md` & `imt_ring-1.3.5/readme.md`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/imt_ring.egg-info/PKG-INFO` & `imt_ring-1.3.5/src/imt_ring.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imt-ring
-Version: 1.3.4
+Version: 1.3.5
 Summary: RING: Recurrent Inertial Graph-based Estimator
 Author-email: Simon Bachhuber <simon.bachhuber@fau.de>
 Project-URL: Homepage, https://github.com/SimiPixel/ring
 Project-URL: Issues, https://github.com/SimiPixel/ring/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `imt_ring-1.3.4/src/imt_ring.egg-info/SOURCES.txt` & `imt_ring-1.3.5/src/imt_ring.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/__init__.py` & `imt_ring-1.3.5/src/ring/__init__.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/algebra.py` & `imt_ring-1.3.5/src/ring/algebra.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/algorithms/__init__.py` & `imt_ring-1.3.5/src/ring/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/algorithms/_random.py` & `imt_ring-1.3.5/src/ring/algorithms/_random.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Callable, Optional
 import warnings
 
 import jax
 from jax import random
 import jax.numpy as jnp
+
 from ring import maths
 
 Float = jax.Array
 TimeDependentFloat = Callable[[Float], Float]
 
 
 def _to_float(scalar: Float | TimeDependentFloat, t: Float) -> Float:
@@ -36,28 +37,28 @@
     cdf_bins_min: int = 5,
     cdf_bins_max: Optional[int] = None,
     interpolation_method: str = "cosine",
 ) -> jax.Array:
     def body_fn_outer(val):
         i, t, phi, key_t, key_ang, ANG = val
 
-        key_t, consume = random.split(key_t)
-        dt = random.uniform(consume, minval=t_min, maxval=_to_float(t_max, t))
-
-        key_ang, consume = random.split(key_ang)
-        phi = _resolve_range_of_motion(
+        key_t, consume_t = random.split(key_t)
+        key_ang, consume_ang = random.split(key_ang)
+        dt, phi = _resolve_range_of_motion(
             range_of_motion,
             range_of_motion_method,
             _to_float(dang_min, t),
             _to_float(dang_max, t),
             _to_float(delta_ang_min, t),
             _to_float(delta_ang_max, t),
-            dt,
+            t_min,
+            _to_float(t_max, t),
             phi,
-            consume,
+            consume_t,
+            consume_ang,
             max_iter,
         )
         t += dt
 
         # TODO do we really need the `jnp.floor(t / Ts) * Ts` since we resample later
         # anyways
         ANG_i = jnp.array([[jnp.floor(t / Ts) * Ts, phi]])
@@ -242,20 +243,22 @@
 def _resolve_range_of_motion(
     range_of_motion,
     range_of_motion_method,
     dang_min,
     dang_max,
     delta_ang_min,
     delta_ang_max,
-    dt,
+    t_min,
+    t_max,
     prev_phi,
-    key,
+    key_t,
+    key_ang,
     max_iter,
 ):
-    def _next_phi(key):
+    def _next_phi(key, dt):
         key, consume = random.split(key)
 
         if range_of_motion:
             if range_of_motion_method == "coinflip":
                 probs = jnp.array([0.5, 0.5])
             elif range_of_motion_method == "uniform":
                 p = 0.5 * (1 - prev_phi / jnp.pi)
@@ -290,29 +293,41 @@
         else:
             dphi = random.uniform(consume, minval=dang_min, maxval=dang_max) * dt
             key, consume = random.split(key)
             sign = random.choice(consume, jnp.array([1.0, -1.0]))
             return prev_phi + sign * dphi
 
     def body_fn(val):
-        key, _, i = val
-        key, consume = jax.random.split(key)
-        next_phi = _next_phi(consume)
-        return key, next_phi, i + 1
+        key_t, key_ang, _, _, i = val
+
+        key_t, consume_t = jax.random.split(key_t)
+        dt = jax.random.uniform(consume_t, minval=t_min, maxval=t_max)
+
+        key_ang, consume_ang = jax.random.split(key_ang)
+        next_phi = _next_phi(consume_ang, dt)
+
+        return key_t, key_ang, dt, next_phi, i + 1
 
     def cond_fn(val):
-        _, next_phi, i = val
+        *_, dt, next_phi, i = val
         delta_phi = jnp.abs(next_phi - prev_phi)
-        # delta is in bounds
-        break_if_true1 = (delta_phi >= delta_ang_min) & (delta_phi <= delta_ang_max)
+        # delta_ang is in bounds
+        cond_delta_ang = (delta_phi >= delta_ang_min) & (delta_phi <= delta_ang_max)
+        # dang is in bounds
+        dang = delta_phi / dt
+        cond_dang = (dang >= dang_min) & (dang <= dang_max)
+
+        break_if_true1 = jnp.logical_and(cond_delta_ang, cond_dang)
+        # break out of loop
         break_if_true2 = i > max_iter
         return (i == 0) | (jnp.logical_not(break_if_true1 | break_if_true2))
 
-    # the `prev_phi` here is unused
-    return jax.lax.while_loop(cond_fn, body_fn, (key, prev_phi, 0))[1]
+    init_val = (key_t, key_ang, 1.0, prev_phi, 0)
+    *_, dt, next_phi, _ = jax.lax.while_loop(cond_fn, body_fn, init_val)
+    return dt, next_phi
 
 
 def cosInterpolate(x, xp, fp):
     i = jnp.clip(jnp.searchsorted(xp, x, side="right"), 1, len(xp) - 1)
     dx = xp[i] - xp[i - 1]
     alpha = (x - xp[i - 1]) / dx
```

### Comparing `imt_ring-1.3.4/src/ring/algorithms/custom_joints/rr_imp_joint.py` & `imt_ring-1.3.5/src/ring/algorithms/custom_joints/rr_imp_joint.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/algorithms/custom_joints/rr_joint.py` & `imt_ring-1.3.5/src/ring/algorithms/custom_joints/rr_joint.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/algorithms/custom_joints/suntay.py` & `imt_ring-1.3.5/src/ring/algorithms/custom_joints/suntay.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,19 +292,25 @@
     )
     ring.register_new_joint_type(name, joint_model, 1, overwrite=True)
 
 
 def Polynomial_DrawnFnPair(
     order: int = 2,
     center: bool = False,
-    flexion_center: Optional[float] = None,
+    flexion_center_deg: Optional[float] = None,
     include_bias: bool = True,
+    enable_scale_delta: bool = True,
 ) -> DrawnFnPairFactory:
     assert not (order == 0 and not include_bias)
 
+    flexion_center = (
+        jnp.deg2rad(flexion_center_deg) if flexion_center_deg is not None else None
+    )
+    del flexion_center_deg
+
     # because 0-th order is also counted
     order += 1
     powers = jnp.arange(order) if include_bias else jnp.arange(1, order)
 
     def factory(xs, mn, mx):
         nonlocal flexion_center
 
@@ -312,38 +318,44 @@
         flexion_mx = jnp.max(xs)
 
         def _apply_poly_factors(poly_factors, q):
             return poly_factors @ jnp.power(q, powers)
 
         if flexion_center is None:
             flexion_center = (flexion_mn + flexion_mx) / 2
+
+        if (order - 1) == 0:
+            method = "clip"
+            minval, maxval = mn, mx
         else:
-            flexion_center = jnp.array(flexion_center)
+            method = "minmax"
+            minval, maxval = -1.0, 1.0
 
         def init(key):
             c1, c2, c3 = jax.random.split(key, 3)
             poly_factors = jax.random.uniform(
-                c1, shape=(len(powers),), minval=-1.0, maxval=1.0
+                c1, shape=(len(powers),), minval=minval, maxval=maxval
             )
             q0 = jax.random.uniform(c2, minval=flexion_mn, maxval=flexion_mx)
             values = jax.vmap(_apply_poly_factors, in_axes=(None, 0))(
                 poly_factors, xs - q0
             )
             eps = 1e-6
             amin, amax = jnp.min(values), jnp.max(values) + eps
-            delta = amax - amin
-            scale_delta = jnp.clip(jax.random.normal(c3) + 0.5, 1.0)
-            amax = amin + delta * scale_delta
+            if enable_scale_delta:
+                delta = amax - amin
+                scale_delta = jnp.clip(jax.random.normal(c3) + 0.5, 1.0)
+                amax = amin + delta * scale_delta
             return amin, amax, poly_factors, q0
 
         def _apply(params, q):
             amin, amax, poly_factors, q0 = params
             q = q - q0
             value = _apply_poly_factors(poly_factors, q)
-            return restrict(value, mn, mx, amin, amax)
+            return restrict(value, mn, mx, amin, amax, method=method)
 
         if center:
 
             def apply(params, q):
                 return _apply(params, q) - _apply(params, flexion_center)
 
         else:
```

### Comparing `imt_ring-1.3.4/src/ring/algorithms/dynamics.py` & `imt_ring-1.3.5/src/ring/algorithms/dynamics.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/algorithms/generator/__init__.py` & `imt_ring-1.3.5/src/ring/algorithms/generator/__init__.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/algorithms/generator/base.py` & `imt_ring-1.3.5/src/ring/algorithms/generator/base.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/algorithms/generator/batch.py` & `imt_ring-1.3.5/src/ring/algorithms/generator/batch.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,16 +93,18 @@
         size = int(size / n_calls)
         jit = True if n_calls > 1 else False
         gen_jit = batch_generators_lazy(gen, size, jit=jit)
 
         for _ in range(n_calls):
             key, consume = jax.random.split(key)
             sample = gen_jit(consume)
-            # converts also to numpy
+            # converts also to numpy; but with np.array.flags.writeable = False
             sample = jax.device_get(sample)
+            # this then sets this flag to True
+            sample = jax.tree_map(np.array, sample)
             data.extend([jax.tree_map(lambda a: a[i], sample) for i in range(size)])
 
     return data
 
 
 def _is_nan(ele: tree_utils.PyTree, i: int, verbose: bool = False):
     isnan = np.any([np.any(np.isnan(arr)) for arr in jax.tree_util.tree_leaves(ele)])
```

### Comparing `imt_ring-1.3.4/src/ring/algorithms/generator/motion_artifacts.py` & `imt_ring-1.3.5/src/ring/algorithms/generator/motion_artifacts.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/algorithms/generator/pd_control.py` & `imt_ring-1.3.5/src/ring/algorithms/generator/pd_control.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/algorithms/generator/randomize.py` & `imt_ring-1.3.5/src/ring/algorithms/generator/randomize.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/algorithms/generator/transforms.py` & `imt_ring-1.3.5/src/ring/algorithms/generator/transforms.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/algorithms/generator/types.py` & `imt_ring-1.3.5/src/ring/algorithms/generator/types.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/algorithms/jcalc.py` & `imt_ring-1.3.5/src/ring/algorithms/jcalc.py`

 * *Files 1% similar despite different names*

```diff
@@ -420,22 +420,22 @@
     key_t: jax.random.PRNGKey,
     key_value: jax.random.PRNGKey,
     dt: float,
     _: jax.Array,
     # TODO, delete these args and pass a modifified `config` with `replace` instead
     enable_range_of_motion: bool = True,
     free_spherical: bool = False,
+    # how often it should try to fullfill the dang_min/max and delta_ang_min/max conds
+    max_iter: int = 5,
 ) -> jax.Array:
     key_value, consume = jax.random.split(key_value)
     ANG_0 = jax.random.uniform(consume, minval=config.ang0_min, maxval=config.ang0_max)
     # `random_angle_over_time` always returns wrapped angles, thus it would be
     # inconsistent to allow an initial value that is not wrapped
     ANG_0 = maths.wrap_to_pi(ANG_0)
-    # only used for `delta_ang_min_max` logic
-    max_iter = 5
     return _random.random_angle_over_time(
         key_t,
         key_value,
         ANG_0,
         config.dang_min_free_spherical if free_spherical else config.dang_min,
         config.dang_max_free_spherical if free_spherical else config.dang_max,
         config.delta_ang_min_free_spherical if free_spherical else config.delta_ang_min,
```

### Comparing `imt_ring-1.3.4/src/ring/algorithms/kinematics.py` & `imt_ring-1.3.5/src/ring/algorithms/kinematics.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/algorithms/sensors.py` & `imt_ring-1.3.5/src/ring/algorithms/sensors.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/base.py` & `imt_ring-1.3.5/src/ring/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -569,14 +569,16 @@
         new_joint_type: str,
         new_arma: Optional[jax.Array] = None,
         new_damp: Optional[jax.Array] = None,
         new_stif: Optional[jax.Array] = None,
         new_zero: Optional[jax.Array] = None,
     ):
         "By default damping, stiffness are set to zero."
+        from ring.algorithms import get_joint_model
+
         q_size, qd_size = Q_WIDTHS[new_joint_type], QD_WIDTHS[new_joint_type]
 
         def logic_unfreeze_to_spherical(link_name, olt, ola, old, ols, olz):
             nlt, nla, nld, nls, nlz = olt, ola, old, ols, olz
 
             if link_name == name:
                 nlt = new_joint_type
@@ -590,15 +592,21 @@
 
                 # unit quaternion
                 if new_joint_type in ["spherical", "free", "cor"] and new_zero is None:
                     nlz = nlz.at[0].set(1.0)
 
             return nlt, nla, nld, nls, nlz
 
-        return _update_sys_if_replace_joint_type(self, logic_unfreeze_to_spherical)
+        sys = _update_sys_if_replace_joint_type(self, logic_unfreeze_to_spherical)
+
+        jm = get_joint_model(new_joint_type)
+        if jm.init_joint_params is not None:
+            sys = sys.from_str(sys.to_str())
+
+        return sys
 
     def findall_imus(self) -> list[str]:
         return [name for name in self.link_names if name[:3] == "imu"]
 
     def findall_segments(self) -> list[str]:
         imus = self.findall_imus()
         return [name for name in self.link_names if name not in imus]
```

### Comparing `imt_ring-1.3.4/src/ring/io/examples/branched.xml` & `imt_ring-1.3.5/src/ring/io/examples/branched.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/io/examples/exclude/knee_trans_dof.xml` & `imt_ring-1.3.5/src/ring/io/examples/exclude/knee_trans_dof.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/io/examples/exclude/standard_sys.xml` & `imt_ring-1.3.5/src/ring/io/examples/exclude/standard_sys.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/io/examples/exclude/standard_sys_rr_imp.xml` & `imt_ring-1.3.5/src/ring/io/examples/exclude/standard_sys_rr_imp.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/io/examples/inv_pendulum.xml` & `imt_ring-1.3.5/src/ring/io/examples/inv_pendulum.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/io/examples/knee_flexible_imus.xml` & `imt_ring-1.3.5/src/ring/io/examples/knee_flexible_imus.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/io/examples/test_all_1.xml` & `imt_ring-1.3.5/src/ring/io/examples/test_all_1.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/io/examples/test_all_2.xml` & `imt_ring-1.3.5/src/ring/io/examples/test_all_2.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/io/examples/test_control.xml` & `imt_ring-1.3.5/src/ring/io/examples/test_control.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/io/examples/test_double_pendulum.xml` & `imt_ring-1.3.5/src/ring/io/examples/test_double_pendulum.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/io/examples/test_kinematics.xml` & `imt_ring-1.3.5/src/ring/io/examples/test_kinematics.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/io/examples/test_morph_system/four_seg_seg1.xml` & `imt_ring-1.3.5/src/ring/io/examples/test_morph_system/four_seg_seg1.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/io/examples/test_morph_system/four_seg_seg3.xml` & `imt_ring-1.3.5/src/ring/io/examples/test_morph_system/four_seg_seg3.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/io/examples/test_randomize_position.xml` & `imt_ring-1.3.5/src/ring/io/examples/test_randomize_position.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/io/examples/test_three_seg_seg2.xml` & `imt_ring-1.3.5/src/ring/io/examples/test_three_seg_seg2.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/io/examples.py` & `imt_ring-1.3.5/src/ring/io/examples.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/io/xml/abstract.py` & `imt_ring-1.3.5/src/ring/io/xml/abstract.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/io/xml/from_xml.py` & `imt_ring-1.3.5/src/ring/io/xml/from_xml.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/io/xml/test_from_xml.py` & `imt_ring-1.3.5/src/ring/io/xml/test_from_xml.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/io/xml/test_to_xml.py` & `imt_ring-1.3.5/src/ring/io/xml/test_to_xml.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/io/xml/to_xml.py` & `imt_ring-1.3.5/src/ring/io/xml/to_xml.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/maths.py` & `imt_ring-1.3.5/src/ring/maths.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/ml/__init__.py` & `imt_ring-1.3.5/src/ring/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/ml/base.py` & `imt_ring-1.3.5/src/ring/ml/base.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/ml/callbacks.py` & `imt_ring-1.3.5/src/ring/ml/callbacks.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/ml/ml_utils.py` & `imt_ring-1.3.5/src/ring/ml/ml_utils.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/ml/optimizer.py` & `imt_ring-1.3.5/src/ring/ml/optimizer.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/ml/params/0x13e3518065c21cd8.pickle` & `imt_ring-1.3.5/src/ring/ml/params/0x13e3518065c21cd8.pickle`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/ml/ringnet.py` & `imt_ring-1.3.5/src/ring/ml/ringnet.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/ml/train.py` & `imt_ring-1.3.5/src/ring/ml/train.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/ml/training_loop.py` & `imt_ring-1.3.5/src/ring/ml/training_loop.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/rendering/base_render.py` & `imt_ring-1.3.5/src/ring/rendering/base_render.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/rendering/mujoco_render.py` & `imt_ring-1.3.5/src/ring/rendering/mujoco_render.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/rendering/vispy_render.py` & `imt_ring-1.3.5/src/ring/rendering/vispy_render.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/rendering/vispy_visuals.py` & `imt_ring-1.3.5/src/ring/rendering/vispy_visuals.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/sim2real/sim2real.py` & `imt_ring-1.3.5/src/ring/sim2real/sim2real.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/spatial.py` & `imt_ring-1.3.5/src/ring/spatial.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/sys_composer/delete_sys.py` & `imt_ring-1.3.5/src/ring/sys_composer/delete_sys.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/sys_composer/inject_sys.py` & `imt_ring-1.3.5/src/ring/sys_composer/inject_sys.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/sys_composer/morph_sys.py` & `imt_ring-1.3.5/src/ring/sys_composer/morph_sys.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/utils/__init__.py` & `imt_ring-1.3.5/src/ring/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/utils/batchsize.py` & `imt_ring-1.3.5/src/ring/utils/batchsize.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/utils/colab.py` & `imt_ring-1.3.5/src/ring/utils/colab.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/utils/hdf5.py` & `imt_ring-1.3.5/src/ring/utils/hdf5.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/utils/normalizer.py` & `imt_ring-1.3.5/src/ring/utils/normalizer.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/utils/path.py` & `imt_ring-1.3.5/src/ring/utils/path.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/src/ring/utils/utils.py` & `imt_ring-1.3.5/src/ring/utils/utils.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/tests/test_algebra.py` & `imt_ring-1.3.5/tests/test_algebra.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/tests/test_base.py` & `imt_ring-1.3.5/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/tests/test_custom_joints.py` & `imt_ring-1.3.5/tests/test_custom_joints.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/tests/test_dynamics.py` & `imt_ring-1.3.5/tests/test_dynamics.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/tests/test_generator.py` & `imt_ring-1.3.5/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/tests/test_jcalc.py` & `imt_ring-1.3.5/tests/test_jcalc.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/tests/test_jit.py` & `imt_ring-1.3.5/tests/test_jit.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/tests/test_kinematics.py` & `imt_ring-1.3.5/tests/test_kinematics.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/tests/test_maths.py` & `imt_ring-1.3.5/tests/test_maths.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/tests/test_ml_utils.py` & `imt_ring-1.3.5/tests/test_ml_utils.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/tests/test_motion_artifacts.py` & `imt_ring-1.3.5/tests/test_motion_artifacts.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/tests/test_pd_control.py` & `imt_ring-1.3.5/tests/test_pd_control.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/tests/test_random.py` & `imt_ring-1.3.5/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/tests/test_randomize.py` & `imt_ring-1.3.5/tests/test_randomize.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/tests/test_rcmg.py` & `imt_ring-1.3.5/tests/test_rcmg.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/tests/test_render.py` & `imt_ring-1.3.5/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/tests/test_sensors.py` & `imt_ring-1.3.5/tests/test_sensors.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/tests/test_sim2real.py` & `imt_ring-1.3.5/tests/test_sim2real.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/tests/test_sys_composer.py` & `imt_ring-1.3.5/tests/test_sys_composer.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/tests/test_train.py` & `imt_ring-1.3.5/tests/test_train.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.4/tests/test_utils.py` & `imt_ring-1.3.5/tests/test_utils.py`

 * *Files identical despite different names*

