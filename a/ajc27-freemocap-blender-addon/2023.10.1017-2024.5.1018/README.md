# Comparing `tmp/ajc27_freemocap_blender_addon-2023.10.1017.tar.gz` & `tmp/ajc27_freemocap_blender_addon-2024.5.1018.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ajc27_freemocap_blender_addon-2023.10.1017.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ajc27_freemocap_blender_addon-2024.5.1018.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ajc27_freemocap_blender_addon-2023.10.1017.tar` & `ajc27_freemocap_blender_addon-2024.5.1018.tar`

### file list

```diff
@@ -1,146 +1,146 @@
--rw-r--r--   0        0        0     1114 2024-04-25 16:27:55.573934 ajc27_freemocap_blender_addon-2023.10.1017/.github/workflows/flit_publish_to_pypi.yml
--rw-r--r--   0        0        0     1113 2024-04-25 16:27:55.573934 ajc27_freemocap_blender_addon-2023.10.1017/.github/workflows/publish_to_pypi_on_version_bump.yml
--rw-r--r--   0        0        0     1871 2024-04-25 16:27:55.573934 ajc27_freemocap_blender_addon-2023.10.1017/.gitignore
--rw-r--r--   0        0        0    34523 2024-04-25 16:27:55.573934 ajc27_freemocap_blender_addon-2023.10.1017/LICENSE
--rw-r--r--   0        0        0      693 2024-04-25 16:27:55.573934 ajc27_freemocap_blender_addon-2023.10.1017/README.md
--rw-r--r--   0        0        0      176 2024-04-25 16:27:55.573934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/.idea/.gitignore
--rw-r--r--   0        0        0      441 2024-04-25 16:27:55.573934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/.idea/ajc27_freemocap_blender_addon.iml
--rw-r--r--   0        0        0      174 2024-04-25 16:27:55.573934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      278 2024-04-25 16:27:55.573934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/.idea/misc.xml
--rw-r--r--   0        0        0      310 2024-04-25 16:27:55.573934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/.idea/modules.xml
--rw-r--r--   0        0        0      183 2024-04-25 16:27:55.573934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/.idea/vcs.xml
--rw-r--r--   0        0        0     2870 2024-04-25 16:27:55.573934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/__init__.py
--rw-r--r--   0        0        0   235277 2024-04-25 16:27:55.573934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/assets/body_mesh.ply
--rw-r--r--   0        0        0    44734 2024-04-25 16:27:55.573934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/assets/charuco_board.png
--rw-r--r--   0        0        0    44729 2024-04-25 16:27:55.573934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/assets/freemocap_logo_white_outline.png
--rw-r--r--   0        0        0   705884 2024-04-25 16:27:55.577934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/assets/skelly_lowpoly_mesh.fbx
--rw-r--r--   0        0        0      511 2024-04-25 16:27:55.577934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/__init__.py
--rw-r--r--   0        0        0     7989 2024-04-25 16:27:55.577934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/main_view3d_panel.py
--rw-r--r--   0        0        0     1742 2024-04-25 16:27:55.577934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/__init__.py
--rw-r--r--   0        0        0     2532 2024-04-25 16:27:55.577934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_add_body_mesh.py
--rw-r--r--   0        0        0     2675 2024-04-25 16:27:55.577934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_add_rig.py
--rw-r--r--   0        0        0      359 2024-04-25 16:27:55.577934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_clear_scene.py
--rw-r--r--   0        0        0      849 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_create_video.py
--rw-r--r--   0        0        0      398 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_download_sample_data.py
--rw-r--r--   0        0        0     1094 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_export_fbx.py
--rw-r--r--   0        0        0     2027 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_load_freemocap_data.py
--rw-r--r--   0        0        0      670 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_load_videos.py
--rw-r--r--   0        0        0     1615 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_reduce_bone_length_dispersion.py
--rw-r--r--   0        0        0      954 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_reduce_shakiness.py
--rw-r--r--   0        0        0     2320 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_reorient_empties.py
--rw-r--r--   0        0        0     1388 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_run_all.py
--rw-r--r--   0        0        0     1463 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_save_out_data.py
--rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/properties/__init__.py
--rw-r--r--   0        0        0     6418 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/properties/properties.py
--rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/sub_panels/__init__.py
--rw-r--r--   0        0        0      881 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/sub_panels/video_export_panel.py
--rw-r--r--   0        0        0       67 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/create_video/__init__.py
--rw-r--r--   0        0        0     1263 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/create_video/create_video.py
--rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/__init__.py
--rw-r--r--   0        0        0     1390 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/add_render_background.py
--rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/overlay_components/__init__.py
--rw-r--r--   0        0        0      303 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/overlay_components/frame_information_dataclass.py
--rw-r--r--   0        0        0     1240 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/overlay_components/frame_number_overlay.py
--rw-r--r--   0        0        0     3029 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/overlay_components/image_overlays.py
--rw-r--r--   0        0        0     3542 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/overlay_components/json_table_overlays.py
--rw-r--r--   0        0        0    18216 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/overlay_components/matplotlib_plot_overlays.py
--rw-r--r--   0        0        0      941 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/rearrange_background_videos.py
--rw-r--r--   0        0        0     2657 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/save_video.py
--rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/empties/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/empties/creation/__init__.py
--rw-r--r--   0        0        0     2041 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/empties/creation/create_empty_from_trajectory.py
--rw-r--r--   0        0        0     2272 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/empties/creation/create_freemocap_empties.py
--rw-r--r--   0        0        0     4187 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/empties/creation/create_virtual_trajectories.py
--rw-r--r--   0        0        0     4801 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/empties/hands.py
--rw-r--r--   0        0        0     3578 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/empties/reduce_shakiness.py
--rw-r--r--   0        0        0     9042 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/empties/reorient_empties.py
--rw-r--r--   0        0        0     1704 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/empties/translate_empty_and_its_children.py
--rw-r--r--   0        0        0     3860 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/empties/update_empty_positions.py
--rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/fbx_export/__init__.py
--rw-r--r--   0        0        0    29592 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/fbx_export/fbx.py
--rw-r--r--   0        0        0     1873 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/fbx_export/get_io_scene_fbx_addon.py
--rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/load_videos/__init__.py
--rw-r--r--   0        0        0     3094 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/load_videos/load_videos.py
--rw-r--r--   0        0        0      905 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/load_videos/rearrange_background_videos.py
--rw-r--r--   0        0        0    14085 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/main_controller.py
--rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/materials/__init__.py
--rw-r--r--   0        0        0     3319 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/materials/create_checkerboard_material.py
--rw-r--r--   0        0        0     6136 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/materials/create_material.py
--rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/__init__.py
--rw-r--r--   0        0        0    13248 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/attach_mesh_to_rig.py
--rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/center_of_mass/__init__.py
--rw-r--r--   0        0        0     1379 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/center_of_mass/center_of_mass_mesh.py
--rw-r--r--   0        0        0     4739 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/center_of_mass/center_of_mass_trails.py
--rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/__init__.py
--rw-r--r--   0        0        0      942 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/create_bone_stick.py
--rw-r--r--   0        0        0      690 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/get_edit_bones.py
--rw-r--r--   0        0        0     5051 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/make_bone_mesh.py
--rw-r--r--   0        0        0      853 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/parent_mesh_to_rig.py
--rw-r--r--   0        0        0     5222 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/put_meshes_on_empties.py
--rw-r--r--   0        0        0     1460 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/put_sphere_at_location.py
--rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/skelly_mesh/__init__.py
--rw-r--r--   0        0        0     3448 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/skelly_mesh/attach_skelly_mesh.py
--rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/rig/__init__.py
--rw-r--r--   0        0        0    42581 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/rig/add_rig.py
--rw-r--r--   0        0        0     5589 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/rig/save_bone_and_joint_angles_from_rig.py
--rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/setup_scene/__init__.py
--rw-r--r--   0        0        0      528 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/setup_scene/clear_scene.py
--rw-r--r--   0        0        0     1221 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/setup_scene/get_path_to_sample_data.py
--rw-r--r--   0        0        0      594 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/setup_scene/make_parent_empties.py
--rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/setup_scene/scene_objects/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/setup_scene/scene_objects/cameras/__init__.py
--rw-r--r--   0        0        0     4046 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/setup_scene/scene_objects/cameras/create_cameras.py
--rw-r--r--   0        0        0      951 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/setup_scene/scene_objects/create_scene_objects.py
--rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/setup_scene/scene_objects/ground_plane/__init__.py
--rw-r--r--   0        0        0     1553 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/setup_scene/scene_objects/ground_plane/create_ground_plane.py
--rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/setup_scene/scene_objects/lights/__init__.py
--rw-r--r--   0        0        0      894 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/setup_scene/scene_objects/lights/create_lights.py
--rw-r--r--   0        0        0      316 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/setup_scene/set_start_end_frame.py
--rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/bones/__init__.py
--rw-r--r--   0        0        0    14652 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/bones/bone_constraints.py
--rw-r--r--   0        0        0    10402 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/bones/bone_definitions.py
--rw-r--r--   0        0        0        0 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/freemocap_data/__init__.py
--rw-r--r--   0        0        0     9923 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/freemocap_data/freemocap_data_model.py
--rw-r--r--   0        0        0        0 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/freemocap_data/helpers/__init__.py
--rw-r--r--   0        0        0     1179 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/freemocap_data/helpers/freemocap_component_data.py
--rw-r--r--   0        0        0     1874 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/freemocap_data/helpers/freemocap_data_paths.py
--rw-r--r--   0        0        0     2201 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/freemocap_data/helpers/freemocap_data_stats.py
--rw-r--r--   0        0        0        0 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/mediapipe_names/__init__.py
--rw-r--r--   0        0        0     5533 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/mediapipe_names/mediapipe_heirarchy.py
--rw-r--r--   0        0        0     4434 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/mediapipe_names/mediapipe_trajectory_names.py
--rw-r--r--   0        0        0      828 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/mediapipe_names/virtual_trajectories.py
--rw-r--r--   0        0        0        0 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/parameter_models/__init__.py
--rw-r--r--   0        0        0      652 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/parameter_models/default_parameters.json
--rw-r--r--   0        0        0     1132 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/parameter_models/load_parameters_config.py
--rw-r--r--   0        0        0     1197 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/parameter_models/parameter_models.py
--rw-r--r--   0        0        0     5284 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/parameter_models/video_config.py
--rw-r--r--   0        0        0        0 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/__init__.py
--rw-r--r--   0        0        0    26905 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/handler.py
--rw-r--r--   0        0        0        0 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/helpers/__init__.py
--rw-r--r--   0        0        0    11082 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/helpers/saver.py
--rw-r--r--   0        0        0     9328 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/helpers/transformer.py
--rw-r--r--   0        0        0        0 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/enforce_rigid_bones/__init__.py
--rw-r--r--   0        0        0     2987 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/enforce_rigid_bones/calculate_body_dimensions.py
--rw-r--r--   0        0        0     2093 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/enforce_rigid_bones/calculate_bone_length_statistics.py
--rw-r--r--   0        0        0     5759 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/enforce_rigid_bones/enforce_rigid_bones.py
--rw-r--r--   0        0        0     3604 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/estimate_good_frame.py
--rw-r--r--   0        0        0     6119 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/fix_hand_data.py
--rw-r--r--   0        0        0      209 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/freemocap_empties_from_parent_object.py
--rw-r--r--   0        0        0     5587 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/put_skeleton_on_ground.py
--rw-r--r--   0        0        0        0 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/utilities/__init__.py
--rw-r--r--   0        0        0      630 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/utilities/get_or_create_freemocap_data_handler.py
--rw-r--r--   0        0        0      762 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/utilities/load_data.py
--rw-r--r--   0        0        0     2424 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/main.py
--rw-r--r--   0        0        0        0 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/system/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/system/configure_logging/__init__.py
--rw-r--r--   0        0        0     6838 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/system/configure_logging/configure_logging.py
--rw-r--r--   0        0        0     1115 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/system/configure_logging/utilities.py
--rw-r--r--   0        0        0        0 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/utilities/__init__.py
--rw-r--r--   0        0        0     1567 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/utilities/install_dependencies.py
--rw-r--r--   0        0        0      241 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/poetry.lock
--rw-r--r--   0        0        0      931 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/pyproject.toml
--rw-r--r--   0        0        0     1176 1970-01-01 00:00:00.000000 ajc27_freemocap_blender_addon-2023.10.1017/PKG-INFO
+-rw-r--r--   0        0        0     1114 2024-05-15 20:03:15.818378 ajc27_freemocap_blender_addon-2024.5.1018/.github/workflows/flit_publish_to_pypi.yml
+-rw-r--r--   0        0        0     1113 2024-05-15 20:03:15.818378 ajc27_freemocap_blender_addon-2024.5.1018/.github/workflows/publish_to_pypi_on_version_bump.yml
+-rw-r--r--   0        0        0     1871 2024-05-15 20:03:15.818378 ajc27_freemocap_blender_addon-2024.5.1018/.gitignore
+-rw-r--r--   0        0        0    34523 2024-05-15 20:03:15.818378 ajc27_freemocap_blender_addon-2024.5.1018/LICENSE
+-rw-r--r--   0        0        0      693 2024-05-15 20:03:15.818378 ajc27_freemocap_blender_addon-2024.5.1018/README.md
+-rw-r--r--   0        0        0      176 2024-05-15 20:03:15.818378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/.idea/.gitignore
+-rw-r--r--   0        0        0      441 2024-05-15 20:03:15.818378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/.idea/ajc27_freemocap_blender_addon.iml
+-rw-r--r--   0        0        0      174 2024-05-15 20:03:15.818378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      278 2024-05-15 20:03:15.818378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/.idea/misc.xml
+-rw-r--r--   0        0        0      310 2024-05-15 20:03:15.818378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/.idea/modules.xml
+-rw-r--r--   0        0        0      183 2024-05-15 20:03:15.818378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/.idea/vcs.xml
+-rw-r--r--   0        0        0     2870 2024-05-15 20:03:15.818378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/__init__.py
+-rw-r--r--   0        0        0   235277 2024-05-15 20:03:15.822378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/assets/body_mesh.ply
+-rw-r--r--   0        0        0    44734 2024-05-15 20:03:15.822378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/assets/charuco_board.png
+-rw-r--r--   0        0        0    44729 2024-05-15 20:03:15.822378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/assets/freemocap_logo_white_outline.png
+-rw-r--r--   0        0        0   705884 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/assets/skelly_lowpoly_mesh.fbx
+-rw-r--r--   0        0        0      511 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/blender_interface/__init__.py
+-rw-r--r--   0        0        0     7989 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/blender_interface/main_view3d_panel.py
+-rw-r--r--   0        0        0     1742 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/blender_interface/operators/__init__.py
+-rw-r--r--   0        0        0     2532 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/blender_interface/operators/_add_body_mesh.py
+-rw-r--r--   0        0        0     2675 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/blender_interface/operators/_add_rig.py
+-rw-r--r--   0        0        0      359 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/blender_interface/operators/_clear_scene.py
+-rw-r--r--   0        0        0      849 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/blender_interface/operators/_create_video.py
+-rw-r--r--   0        0        0      398 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/blender_interface/operators/_download_sample_data.py
+-rw-r--r--   0        0        0     1094 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/blender_interface/operators/_export_fbx.py
+-rw-r--r--   0        0        0     2027 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/blender_interface/operators/_load_freemocap_data.py
+-rw-r--r--   0        0        0      670 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/blender_interface/operators/_load_videos.py
+-rw-r--r--   0        0        0     1615 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/blender_interface/operators/_reduce_bone_length_dispersion.py
+-rw-r--r--   0        0        0      954 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/blender_interface/operators/_reduce_shakiness.py
+-rw-r--r--   0        0        0     2320 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/blender_interface/operators/_reorient_empties.py
+-rw-r--r--   0        0        0     1388 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/blender_interface/operators/_run_all.py
+-rw-r--r--   0        0        0     1463 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/blender_interface/operators/_save_out_data.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/blender_interface/properties/__init__.py
+-rw-r--r--   0        0        0     6418 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/blender_interface/properties/properties.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/blender_interface/sub_panels/__init__.py
+-rw-r--r--   0        0        0      881 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/blender_interface/sub_panels/video_export_panel.py
+-rw-r--r--   0        0        0       67 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/create_video/__init__.py
+-rw-r--r--   0        0        0     1263 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/create_video/create_video.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/__init__.py
+-rw-r--r--   0        0        0     1390 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/add_render_background.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/overlay_components/__init__.py
+-rw-r--r--   0        0        0      303 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/overlay_components/frame_information_dataclass.py
+-rw-r--r--   0        0        0     1240 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/overlay_components/frame_number_overlay.py
+-rw-r--r--   0        0        0     3029 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/overlay_components/image_overlays.py
+-rw-r--r--   0        0        0     3542 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/overlay_components/json_table_overlays.py
+-rw-r--r--   0        0        0    18216 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/overlay_components/matplotlib_plot_overlays.py
+-rw-r--r--   0        0        0      941 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/rearrange_background_videos.py
+-rw-r--r--   0        0        0     2657 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/save_video.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/empties/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/empties/creation/__init__.py
+-rw-r--r--   0        0        0     2041 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/empties/creation/create_empty_from_trajectory.py
+-rw-r--r--   0        0        0     2272 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/empties/creation/create_freemocap_empties.py
+-rw-r--r--   0        0        0     4187 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/empties/creation/create_virtual_trajectories.py
+-rw-r--r--   0        0        0     4801 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/empties/hands.py
+-rw-r--r--   0        0        0     3578 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/empties/reduce_shakiness.py
+-rw-r--r--   0        0        0     9042 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/empties/reorient_empties.py
+-rw-r--r--   0        0        0     1704 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/empties/translate_empty_and_its_children.py
+-rw-r--r--   0        0        0     3860 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/empties/update_empty_positions.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/fbx_export/__init__.py
+-rw-r--r--   0        0        0    29592 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/fbx_export/fbx.py
+-rw-r--r--   0        0        0     1873 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/fbx_export/get_io_scene_fbx_addon.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/load_videos/__init__.py
+-rw-r--r--   0        0        0     3094 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/load_videos/load_videos.py
+-rw-r--r--   0        0        0      905 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/load_videos/rearrange_background_videos.py
+-rw-r--r--   0        0        0    14085 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/main_controller.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/materials/__init__.py
+-rw-r--r--   0        0        0     3319 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/materials/create_checkerboard_material.py
+-rw-r--r--   0        0        0     6136 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/materials/create_material.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/meshes/__init__.py
+-rw-r--r--   0        0        0    13248 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/meshes/attach_mesh_to_rig.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/meshes/center_of_mass/__init__.py
+-rw-r--r--   0        0        0     1379 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/meshes/center_of_mass/center_of_mass_mesh.py
+-rw-r--r--   0        0        0     4739 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/meshes/center_of_mass/center_of_mass_trails.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/__init__.py
+-rw-r--r--   0        0        0      942 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/create_bone_stick.py
+-rw-r--r--   0        0        0      690 2024-05-15 20:03:15.826378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/get_edit_bones.py
+-rw-r--r--   0        0        0     5051 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/make_bone_mesh.py
+-rw-r--r--   0        0        0      853 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/parent_mesh_to_rig.py
+-rw-r--r--   0        0        0     5222 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/put_meshes_on_empties.py
+-rw-r--r--   0        0        0     1460 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/put_sphere_at_location.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/meshes/skelly_mesh/__init__.py
+-rw-r--r--   0        0        0     3448 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/meshes/skelly_mesh/attach_skelly_mesh.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/rig/__init__.py
+-rw-r--r--   0        0        0    42651 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/rig/add_rig.py
+-rw-r--r--   0        0        0     5589 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/rig/save_bone_and_joint_angles_from_rig.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/setup_scene/__init__.py
+-rw-r--r--   0        0        0      528 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/setup_scene/clear_scene.py
+-rw-r--r--   0        0        0     1221 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/setup_scene/get_path_to_sample_data.py
+-rw-r--r--   0        0        0      594 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/setup_scene/make_parent_empties.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/setup_scene/scene_objects/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/setup_scene/scene_objects/cameras/__init__.py
+-rw-r--r--   0        0        0     4046 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/setup_scene/scene_objects/cameras/create_cameras.py
+-rw-r--r--   0        0        0      951 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/setup_scene/scene_objects/create_scene_objects.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/setup_scene/scene_objects/ground_plane/__init__.py
+-rw-r--r--   0        0        0     1553 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/setup_scene/scene_objects/ground_plane/create_ground_plane.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/setup_scene/scene_objects/lights/__init__.py
+-rw-r--r--   0        0        0      894 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/setup_scene/scene_objects/lights/create_lights.py
+-rw-r--r--   0        0        0      316 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/setup_scene/set_start_end_frame.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/data_models/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/data_models/bones/__init__.py
+-rw-r--r--   0        0        0    14652 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/data_models/bones/bone_constraints.py
+-rw-r--r--   0        0        0    10402 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/data_models/bones/bone_definitions.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/data_models/freemocap_data/__init__.py
+-rw-r--r--   0        0        0     9923 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/data_models/freemocap_data/freemocap_data_model.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/data_models/freemocap_data/helpers/__init__.py
+-rw-r--r--   0        0        0     1179 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/data_models/freemocap_data/helpers/freemocap_component_data.py
+-rw-r--r--   0        0        0     1874 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/data_models/freemocap_data/helpers/freemocap_data_paths.py
+-rw-r--r--   0        0        0     2201 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/data_models/freemocap_data/helpers/freemocap_data_stats.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/data_models/mediapipe_names/__init__.py
+-rw-r--r--   0        0        0     5533 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/data_models/mediapipe_names/mediapipe_heirarchy.py
+-rw-r--r--   0        0        0     4434 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/data_models/mediapipe_names/mediapipe_trajectory_names.py
+-rw-r--r--   0        0        0      828 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/data_models/mediapipe_names/virtual_trajectories.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/data_models/parameter_models/__init__.py
+-rw-r--r--   0        0        0      652 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/data_models/parameter_models/default_parameters.json
+-rw-r--r--   0        0        0     1132 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/data_models/parameter_models/load_parameters_config.py
+-rw-r--r--   0        0        0     1197 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/data_models/parameter_models/parameter_models.py
+-rw-r--r--   0        0        0     5284 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/data_models/parameter_models/video_config.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/freemocap_data_handler/__init__.py
+-rw-r--r--   0        0        0    26905 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/freemocap_data_handler/handler.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/freemocap_data_handler/helpers/__init__.py
+-rw-r--r--   0        0        0    11082 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/freemocap_data_handler/helpers/saver.py
+-rw-r--r--   0        0        0     9328 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/freemocap_data_handler/helpers/transformer.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/enforce_rigid_bones/__init__.py
+-rw-r--r--   0        0        0     2987 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/enforce_rigid_bones/calculate_body_dimensions.py
+-rw-r--r--   0        0        0     2093 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/enforce_rigid_bones/calculate_bone_length_statistics.py
+-rw-r--r--   0        0        0     5840 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/enforce_rigid_bones/enforce_rigid_bones.py
+-rw-r--r--   0        0        0     3604 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/estimate_good_frame.py
+-rw-r--r--   0        0        0     6119 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/fix_hand_data.py
+-rw-r--r--   0        0        0      209 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/freemocap_empties_from_parent_object.py
+-rw-r--r--   0        0        0     5587 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/put_skeleton_on_ground.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/freemocap_data_handler/utilities/__init__.py
+-rw-r--r--   0        0        0      630 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/freemocap_data_handler/utilities/get_or_create_freemocap_data_handler.py
+-rw-r--r--   0        0        0      762 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/freemocap_data_handler/utilities/load_data.py
+-rw-r--r--   0        0        0     2424 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/main.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/system/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/system/configure_logging/__init__.py
+-rw-r--r--   0        0        0     6838 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/system/configure_logging/configure_logging.py
+-rw-r--r--   0        0        0     1115 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/system/configure_logging/utilities.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/utilities/__init__.py
+-rw-r--r--   0        0        0     1567 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/utilities/install_dependencies.py
+-rw-r--r--   0        0        0      241 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/poetry.lock
+-rw-r--r--   0        0        0      927 2024-05-15 20:03:15.830378 ajc27_freemocap_blender_addon-2024.5.1018/pyproject.toml
+-rw-r--r--   0        0        0     1175 1970-01-01 00:00:00.000000 ajc27_freemocap_blender_addon-2024.5.1018/PKG-INFO
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/.github/workflows/flit_publish_to_pypi.yml` & `ajc27_freemocap_blender_addon-2024.5.1018/.github/workflows/flit_publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/.github/workflows/publish_to_pypi_on_version_bump.yml` & `ajc27_freemocap_blender_addon-2024.5.1018/.github/workflows/publish_to_pypi_on_version_bump.yml`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/.gitignore` & `ajc27_freemocap_blender_addon-2024.5.1018/.gitignore`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/LICENSE` & `ajc27_freemocap_blender_addon-2024.5.1018/LICENSE`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/README.md` & `ajc27_freemocap_blender_addon-2024.5.1018/README.md`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/__init__.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 __author__ = """Skelly FreeMoCap"""
 __email__ = "info@freemocap.org"
-__version__ = "v2023.10.1017"
+__version__ = "v2024.05.1018"
 
 #######################################################################
 ### Add-on to adapt the Freemocap Blender output. It can adjust the
 ### empties position, add a rig and a body mesh. The resulting rig
 ### and animation can be imported in platforms like Unreal Engine.
 ### The rig has a TPose as rest pose for easier retargeting.
 ### For best results, when the script is ran the empties should be
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/assets/body_mesh.ply` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/assets/body_mesh.ply`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/assets/charuco_board.png` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/assets/charuco_board.png`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/assets/freemocap_logo_white_outline.png` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/assets/freemocap_logo_white_outline.png`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/assets/skelly_lowpoly_mesh.fbx` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/assets/skelly_lowpoly_mesh.fbx`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/main_view3d_panel.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/blender_interface/main_view3d_panel.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/__init__.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/blender_interface/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_add_body_mesh.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/blender_interface/operators/_add_body_mesh.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_add_rig.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/blender_interface/operators/_add_rig.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_create_video.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/blender_interface/operators/_create_video.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_export_fbx.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/blender_interface/operators/_export_fbx.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_load_freemocap_data.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/blender_interface/operators/_load_freemocap_data.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_load_videos.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/blender_interface/operators/_load_videos.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_reduce_bone_length_dispersion.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/blender_interface/operators/_reduce_bone_length_dispersion.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_reduce_shakiness.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/blender_interface/operators/_reduce_shakiness.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_reorient_empties.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/blender_interface/operators/_reorient_empties.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_run_all.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/blender_interface/operators/_run_all.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_save_out_data.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/blender_interface/operators/_save_out_data.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/properties/properties.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/blender_interface/properties/properties.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/sub_panels/video_export_panel.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/blender_interface/sub_panels/video_export_panel.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/create_video/create_video.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/create_video/create_video.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/add_render_background.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/add_render_background.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/overlay_components/frame_number_overlay.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/overlay_components/frame_number_overlay.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/overlay_components/image_overlays.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/overlay_components/image_overlays.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/overlay_components/json_table_overlays.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/overlay_components/json_table_overlays.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/overlay_components/matplotlib_plot_overlays.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/overlay_components/matplotlib_plot_overlays.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/rearrange_background_videos.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/rearrange_background_videos.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/save_video.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/save_video.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/empties/creation/create_empty_from_trajectory.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/empties/creation/create_empty_from_trajectory.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/empties/creation/create_freemocap_empties.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/empties/creation/create_freemocap_empties.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/empties/creation/create_virtual_trajectories.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/empties/creation/create_virtual_trajectories.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/empties/hands.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/empties/hands.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/empties/reduce_shakiness.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/empties/reduce_shakiness.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/empties/reorient_empties.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/empties/reorient_empties.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/empties/translate_empty_and_its_children.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/empties/translate_empty_and_its_children.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/empties/update_empty_positions.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/empties/update_empty_positions.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/fbx_export/fbx.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/fbx_export/fbx.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/fbx_export/get_io_scene_fbx_addon.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/fbx_export/get_io_scene_fbx_addon.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/load_videos/load_videos.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/load_videos/load_videos.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/load_videos/rearrange_background_videos.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/load_videos/rearrange_background_videos.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/main_controller.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/main_controller.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/materials/create_checkerboard_material.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/materials/create_checkerboard_material.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/materials/create_material.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/materials/create_material.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/attach_mesh_to_rig.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/meshes/attach_mesh_to_rig.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/center_of_mass/center_of_mass_mesh.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/meshes/center_of_mass/center_of_mass_mesh.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/center_of_mass/center_of_mass_trails.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/meshes/center_of_mass/center_of_mass_trails.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/create_bone_stick.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/create_bone_stick.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/get_edit_bones.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/get_edit_bones.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/make_bone_mesh.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/make_bone_mesh.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/parent_mesh_to_rig.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/parent_mesh_to_rig.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/put_meshes_on_empties.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/put_meshes_on_empties.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/put_sphere_at_location.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/put_sphere_at_location.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/skelly_mesh/attach_skelly_mesh.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/meshes/skelly_mesh/attach_skelly_mesh.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/rig/add_rig.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/rig/add_rig.py`

 * *Files 0% similar despite different names*

```diff
@@ -710,21 +710,24 @@
         if add_fingers_constraints:
             hand_locked_track_target = 'hand_thumb_cmc'
         else:
             hand_locked_track_target = 'thumb'
 
         # Create each constraint
         for bone_name, constraint_definitions in ALL_BONES_CONSTRAINT_DEFINITIONS.items():
+            if bone_name not in rig.pose.bones:
+                continue
+
             if not isinstance(constraint_definitions, list):
                 raise Exception(f'Constraint definitions for {bone_name} must be a list')
             
             # If it is a finger bone amd add_fingers_constraints is False continue with the next bone
             if not add_fingers_constraints and len(
                     [finger_part for finger_part in ['palm', 'thumb', 'index', 'middle', 'ring', 'pinky'] if
-                     finger_part in bone_constraint_definition]) > 0:
+                     finger_part in constraint_definitions]) > 0:
                 continue
 
             for constraint in constraint_definitions:
                 # if "target" in constraint.keys():
                 #     base_target_name = constraint["target"]
                 #     actual_target_name = get_actual_empty_target_name(empty_names = empty_names,
                 #                                                       base_target_name = base_target_name)
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/rig/save_bone_and_joint_angles_from_rig.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/rig/save_bone_and_joint_angles_from_rig.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/setup_scene/clear_scene.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/setup_scene/clear_scene.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/setup_scene/get_path_to_sample_data.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/setup_scene/get_path_to_sample_data.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/setup_scene/make_parent_empties.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/setup_scene/make_parent_empties.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/setup_scene/scene_objects/cameras/create_cameras.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/setup_scene/scene_objects/cameras/create_cameras.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/setup_scene/scene_objects/create_scene_objects.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/setup_scene/scene_objects/create_scene_objects.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/setup_scene/scene_objects/ground_plane/create_ground_plane.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/setup_scene/scene_objects/ground_plane/create_ground_plane.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/setup_scene/scene_objects/lights/create_lights.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/core_functions/setup_scene/scene_objects/lights/create_lights.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/bones/bone_constraints.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/data_models/bones/bone_constraints.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/bones/bone_definitions.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/data_models/bones/bone_definitions.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/freemocap_data/freemocap_data_model.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/data_models/freemocap_data/freemocap_data_model.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/freemocap_data/helpers/freemocap_component_data.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/data_models/freemocap_data/helpers/freemocap_component_data.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/freemocap_data/helpers/freemocap_data_paths.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/data_models/freemocap_data/helpers/freemocap_data_paths.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/freemocap_data/helpers/freemocap_data_stats.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/data_models/freemocap_data/helpers/freemocap_data_stats.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/mediapipe_names/mediapipe_heirarchy.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/data_models/mediapipe_names/mediapipe_heirarchy.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/mediapipe_names/mediapipe_trajectory_names.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/data_models/mediapipe_names/mediapipe_trajectory_names.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/mediapipe_names/virtual_trajectories.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/data_models/mediapipe_names/virtual_trajectories.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/parameter_models/default_parameters.json` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/data_models/parameter_models/default_parameters.json`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/parameter_models/load_parameters_config.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/data_models/parameter_models/load_parameters_config.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/parameter_models/parameter_models.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/data_models/parameter_models/parameter_models.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/parameter_models/video_config.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/data_models/parameter_models/video_config.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/handler.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/freemocap_data_handler/handler.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/helpers/saver.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/freemocap_data_handler/helpers/saver.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/helpers/transformer.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/freemocap_data_handler/helpers/transformer.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/enforce_rigid_bones/calculate_body_dimensions.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/enforce_rigid_bones/calculate_body_dimensions.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/enforce_rigid_bones/calculate_bone_length_statistics.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/enforce_rigid_bones/calculate_bone_length_statistics.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/enforce_rigid_bones/enforce_rigid_bones.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/enforce_rigid_bones/enforce_rigid_bones.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,11 +103,14 @@
     log_string = f'\n\n[{type}] Bone Length Statistics:\n'
     header_string = f"{'BONE':<15} {'MEDIAN (cm)':>12} {'STDEV (cm)':>12} {'CV (%)':>12}"
     log_string += header_string + '\n'
     for name, bone in bones.items():
         # Get the statistic values
         median_string = str(round(bone['median'] * 100, 7))
         stdev_string = str(round(bone['stdev'] * 100, 7))
-        cv_string = str(round(bone['stdev'] / bone['median'] * 100, 4))
+        try:
+            cv_string = str(round(bone['stdev'] / bone['median'] * 100, 4))
+        except ZeroDivisionError:
+            cv_string = 'N/A'
         log_string += f"{name:<15} {median_string:>12} {stdev_string:>12} {cv_string:>12}\n"
 
     print(log_string)
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/estimate_good_frame.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/estimate_good_frame.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/fix_hand_data.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/fix_hand_data.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/put_skeleton_on_ground.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/put_skeleton_on_ground.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/utilities/get_or_create_freemocap_data_handler.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/freemocap_data_handler/utilities/get_or_create_freemocap_data_handler.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/utilities/load_data.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/freemocap_data_handler/utilities/load_data.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/main.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/main.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/system/configure_logging/configure_logging.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/system/configure_logging/configure_logging.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/system/configure_logging/utilities.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/system/configure_logging/utilities.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/utilities/install_dependencies.py` & `ajc27_freemocap_blender_addon-2024.5.1018/ajc27_freemocap_blender_addon/utilities/install_dependencies.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/pyproject.toml` & `ajc27_freemocap_blender_addon-2024.5.1018/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 [project.urls]
 Homepage = "https://freemocap.org"
 Documentation = "https://freemocap.github.io/documentation/"
 Github = "https://github.com/freemocap/ajc27_freemocap_blender_addon"
 
 
 [tool.bumpver]
-current_version = "v2023.10.1017"
+current_version = "v2024.05.1018"
 
-version_pattern = "vMAJOR.MINOR.PATCH[-TAG]"
+version_pattern = "vYYYY.0M.BUILD[-TAG]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = true
 [tool.bumpver.file_patterns]
 "ajc27_freemocap_blender_addon/__init__.py" = ["{version}"]
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1017/PKG-INFO` & `ajc27_freemocap_blender_addon-2024.5.1018/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ajc27_freemocap_blender_addon
-Version: 2023.10.1017
+Version: 2024.5.1018
 Summary: A Blender Add-on for working with Freemocap Data (based on @ajc27's addon)
 Author-email: Skelly FreeMoCap <info@freemocap.org>
 Requires-Python: >=3.9,<3.12
 Description-Content-Type: text/markdown
 Project-URL: Documentation, https://freemocap.github.io/documentation/
 Project-URL: Github, https://github.com/freemocap/ajc27_freemocap_blender_addon
 Project-URL: Homepage, https://freemocap.org
```

