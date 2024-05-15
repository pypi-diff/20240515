# Comparing `tmp/pythfinder-0.0.3.8.tar.gz` & `tmp/pythfinder-0.0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythfinder-0.0.3.8.tar", last modified: Wed May 15 04:54:14 2024, max compression
+gzip compressed data, was "pythfinder-0.0.3.9.tar", last modified: Wed May 15 05:22:49 2024, max compression
```

## Comparing `pythfinder-0.0.3.8.tar` & `pythfinder-0.0.3.9.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 04:54:14.107154 pythfinder-0.0.3.8/
--rw-rw-rw-   0        0        0     1295 2024-05-14 05:43:57.000000 pythfinder-0.0.3.8/LICENSE.txt
--rw-rw-rw-   0        0        0       99 2024-05-15 04:25:24.000000 pythfinder-0.0.3.8/MANIFEST.in
--rw-rw-rw-   0        0        0      310 2024-05-15 04:54:14.107154 pythfinder-0.0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0      344 2024-05-14 18:26:37.000000 pythfinder-0.0.3.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 04:54:13.636992 pythfinder-0.0.3.8/pythfinder/
-drwxrwxrwx   0        0        0        0 2024-05-15 04:54:13.690387 pythfinder-0.0.3.8/pythfinder/Components/
-drwxrwxrwx   0        0        0        0 2024-05-15 04:54:13.721639 pythfinder-0.0.3.8/pythfinder/Components/BetterClasses/
--rw-rw-rw-   0        0        0      102 2024-05-14 05:32:56.000000 pythfinder-0.0.3.8/pythfinder/Components/BetterClasses/__init__.py
--rw-rw-rw-   0        0        0     1168 2024-05-13 14:52:24.000000 pythfinder-0.0.3.8/pythfinder/Components/BetterClasses/booleanEx.py
--rw-rw-rw-   0        0        0      627 2024-05-13 14:52:55.000000 pythfinder-0.0.3.8/pythfinder/Components/BetterClasses/edgeDetectorEx.py
--rw-rw-rw-   0        0        0     1140 2024-05-13 15:07:55.000000 pythfinder-0.0.3.8/pythfinder/Components/BetterClasses/errorEx.py
--rw-rw-rw-   0        0        0     4862 2024-05-13 14:45:33.000000 pythfinder-0.0.3.8/pythfinder/Components/BetterClasses/mathEx.py
-drwxrwxrwx   0        0        0        0 2024-05-15 04:54:13.752895 pythfinder-0.0.3.8/pythfinder/Components/Constants/
--rw-rw-rw-   0        0        0       78 2024-05-14 05:33:11.000000 pythfinder-0.0.3.8/pythfinder/Components/Constants/__init__.py
--rw-rw-rw-   0        0        0    20838 2024-05-15 04:53:47.000000 pythfinder-0.0.3.8/pythfinder/Components/Constants/constants.py
--rw-rw-rw-   0        0        0     2905 2024-05-13 15:08:14.000000 pythfinder-0.0.3.8/pythfinder/Components/Constants/constrains.py
--rw-rw-rw-   0        0        0     2705 2024-05-13 15:11:03.000000 pythfinder-0.0.3.8/pythfinder/Components/Constants/screenSize.py
-drwxrwxrwx   0        0        0        0 2024-05-15 04:54:13.759412 pythfinder-0.0.3.8/pythfinder/Components/Controllers/
--rw-rw-rw-   0        0        0      642 2024-05-13 15:12:44.000000 pythfinder-0.0.3.8/pythfinder/Components/Controllers/PIDCoefficients.py
--rw-rw-rw-   0        0        0     1163 2024-05-14 16:07:14.000000 pythfinder-0.0.3.8/pythfinder/Components/Controllers/PIDController.py
--rw-rw-rw-   0        0        0       60 2024-05-14 05:33:22.000000 pythfinder-0.0.3.8/pythfinder/Components/Controllers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 04:54:13.790678 pythfinder-0.0.3.8/pythfinder/Components/Menu/
--rw-rw-rw-   0        0        0       87 2024-05-14 05:33:37.000000 pythfinder-0.0.3.8/pythfinder/Components/Menu/__init__.py
--rw-rw-rw-   0        0        0    22248 2024-05-14 16:06:43.000000 pythfinder-0.0.3.8/pythfinder/Components/Menu/buttons.py
--rw-rw-rw-   0        0        0     1583 2024-05-13 16:09:13.000000 pythfinder-0.0.3.8/pythfinder/Components/Menu/enums.py
--rw-rw-rw-   0        0        0    22448 2024-05-14 16:06:48.000000 pythfinder-0.0.3.8/pythfinder/Components/Menu/main.py
--rw-rw-rw-   0        0        0     4103 2024-05-14 16:07:01.000000 pythfinder-0.0.3.8/pythfinder/Components/Menu/menus.py
--rw-rw-rw-   0        0        0      244 2024-05-14 05:35:39.000000 pythfinder-0.0.3.8/pythfinder/Components/__init__.py
--rw-rw-rw-   0        0        0     5720 2024-05-14 16:04:43.000000 pythfinder-0.0.3.8/pythfinder/Components/background.py
--rw-rw-rw-   0        0        0     9569 2024-05-14 16:05:08.000000 pythfinder-0.0.3.8/pythfinder/Components/controls.py
--rw-rw-rw-   0        0        0     1853 2024-05-14 16:05:12.000000 pythfinder-0.0.3.8/pythfinder/Components/fade.py
--rw-rw-rw-   0        0        0     9861 2024-05-14 15:58:30.000000 pythfinder-0.0.3.8/pythfinder/Components/robot.py
--rw-rw-rw-   0        0        0     1975 2024-05-14 16:05:20.000000 pythfinder-0.0.3.8/pythfinder/Components/table.py
--rw-rw-rw-   0        0        0     4633 2024-05-14 16:05:37.000000 pythfinder-0.0.3.8/pythfinder/Components/trail.py
-drwxrwxrwx   0        0        0        0 2024-05-15 04:54:13.790678 pythfinder-0.0.3.8/pythfinder/Images/
-drwxrwxrwx   0        0        0        0 2024-05-15 04:54:13.837560 pythfinder-0.0.3.8/pythfinder/Images/Controls/
--rw-rw-rw-   0        0        0        0 2024-05-14 18:17:56.000000 pythfinder-0.0.3.8/pythfinder/Images/Controls/__init__.py
--rw-rw-rw-   0        0        0   525562 2024-03-31 07:01:14.000000 pythfinder-0.0.3.8/pythfinder/Images/Controls/btn_backwards.png
--rw-rw-rw-   0        0        0   530916 2024-03-31 07:01:10.000000 pythfinder-0.0.3.8/pythfinder/Images/Controls/btn_forwards.png
--rw-rw-rw-   0        0        0   533042 2024-03-31 07:01:19.000000 pythfinder-0.0.3.8/pythfinder/Images/Controls/btn_hide_trail.png
--rw-rw-rw-   0        0        0   561920 2024-03-31 14:58:53.000000 pythfinder-0.0.3.8/pythfinder/Images/Controls/btn_selecting_off.png
--rw-rw-rw-   0        0        0   558616 2024-03-31 14:58:49.000000 pythfinder-0.0.3.8/pythfinder/Images/Controls/btn_selecting_on.png
--rw-rw-rw-   0        0        0   531856 2024-03-31 07:00:59.000000 pythfinder-0.0.3.8/pythfinder/Images/Controls/btn_show_trail.png
-drwxrwxrwx   0        0        0        0 2024-05-15 04:54:13.837560 pythfinder-0.0.3.8/pythfinder/Images/Menu/
-drwxrwxrwx   0        0        0        0 2024-05-15 04:54:13.853183 pythfinder-0.0.3.8/pythfinder/Images/Menu/General/
-drwxrwxrwx   0        0        0        0 2024-05-15 04:54:13.590114 pythfinder-0.0.3.8/pythfinder/Images/Menu/General/Arrows/
-drwxrwxrwx   0        0        0        0 2024-05-15 04:54:13.859700 pythfinder-0.0.3.8/pythfinder/Images/Menu/General/Arrows/Left/
--rw-rw-rw-   0        0        0     5149 2024-04-07 08:30:53.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/General/Arrows/Left/left_arrow.png
--rw-rw-rw-   0        0        0     5334 2024-04-07 08:30:48.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/General/Arrows/Left/selected_left_arrow.png
-drwxrwxrwx   0        0        0        0 2024-05-15 04:54:13.859700 pythfinder-0.0.3.8/pythfinder/Images/Menu/General/Arrows/Right/
--rw-rw-rw-   0        0        0     5181 2024-04-07 08:31:22.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/General/Arrows/Right/right_arrow.png
--rw-rw-rw-   0        0        0     5279 2024-04-07 08:31:21.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/General/Arrows/Right/selected_right_arrow.png
--rw-rw-rw-   0        0        0        0 2024-05-14 18:18:26.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/General/__init__.py
--rw-rw-rw-   0        0        0   467492 2024-04-07 08:30:13.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/General/general_menu.png
-drwxrwxrwx   0        0        0        0 2024-05-15 04:54:13.890967 pythfinder-0.0.3.8/pythfinder/Images/Menu/Main/
--rw-rw-rw-   0        0        0     8011 2024-04-05 16:14:53.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Main/menu_button.png
--rw-rw-rw-   0        0        0     6208 2024-04-05 16:14:57.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Main/menu_home_button.png
--rw-rw-rw-   0        0        0  1606752 2024-04-05 16:15:02.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Main/menu_main.png
--rw-rw-rw-   0        0        0     8399 2024-04-06 11:39:50.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Main/selected_menu_button.png
--rw-rw-rw-   0        0        0     6451 2024-04-06 11:39:46.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Main/selected_menu_home_button.png
-drwxrwxrwx   0        0        0        0 2024-05-15 04:54:13.906595 pythfinder-0.0.3.8/pythfinder/Images/Menu/Other/
-drwxrwxrwx   0        0        0        0 2024-05-15 04:54:13.922221 pythfinder-0.0.3.8/pythfinder/Images/Menu/Other/FieldCentric/
--rw-rw-rw-   0        0        0    33821 2024-04-07 08:27:04.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Other/FieldCentric/field_centric_off.png
--rw-rw-rw-   0        0        0    34053 2024-04-07 08:27:04.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Other/FieldCentric/field_centric_on.png
--rw-rw-rw-   0        0        0    35325 2024-04-07 08:27:04.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Other/FieldCentric/selected_field_centric_off.png
--rw-rw-rw-   0        0        0    35522 2024-04-07 08:27:04.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Other/FieldCentric/selected_field_centric_on.png
-drwxrwxrwx   0        0        0        0 2024-05-15 04:54:13.937848 pythfinder-0.0.3.8/pythfinder/Images/Menu/Other/RobotBorder/
--rw-rw-rw-   0        0        0    32516 2024-04-07 08:27:48.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Other/RobotBorder/robot_border_off.png
--rw-rw-rw-   0        0        0    32757 2024-04-07 08:27:49.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Other/RobotBorder/robot_border_on.png
--rw-rw-rw-   0        0        0    33964 2024-04-07 08:27:48.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Other/RobotBorder/selected_robot_border_off.png
--rw-rw-rw-   0        0        0    34153 2024-04-07 08:27:48.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Other/RobotBorder/selected_robot_border_on.png
-drwxrwxrwx   0        0        0        0 2024-05-15 04:54:13.959983 pythfinder-0.0.3.8/pythfinder/Images/Menu/Other/ScreenBorder/
--rw-rw-rw-   0        0        0    34863 2024-04-07 08:28:53.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Other/ScreenBorder/screen_border_off.png
--rw-rw-rw-   0        0        0    35031 2024-04-07 08:28:53.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Other/ScreenBorder/screen_border_on.png
--rw-rw-rw-   0        0        0    36547 2024-04-07 08:28:53.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Other/ScreenBorder/selected_screen_border_off.png
--rw-rw-rw-   0        0        0    36670 2024-04-07 08:28:53.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Other/ScreenBorder/selected_screen_border_on.png
--rw-rw-rw-   0        0        0    20270 2024-04-09 17:13:50.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Other/other_indicator.png
--rw-rw-rw-   0        0        0    13339 2024-04-07 08:29:32.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Other/other_quadrant.png
-drwxrwxrwx   0        0        0        0 2024-05-15 04:54:14.006870 pythfinder-0.0.3.8/pythfinder/Images/Menu/Robot/
--rw-rw-rw-   0        0        0    28975 2024-04-08 04:32:03.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Robot/height.png
--rw-rw-rw-   0        0        0    20193 2024-04-08 04:32:07.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Robot/robot_indicator.png
--rw-rw-rw-   0        0        0    39077 2024-04-08 04:32:04.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Robot/robot_path.png
--rw-rw-rw-   0        0        0   138988 2024-04-08 04:32:10.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Robot/robot_path_quadrant.png
--rw-rw-rw-   0        0        0   115045 2024-04-08 04:32:12.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Robot/robot_specs_quadrant.png
--rw-rw-rw-   0        0        0    20716 2024-04-08 04:32:17.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Robot/scale.png
--rw-rw-rw-   0        0        0    30701 2024-04-08 04:32:20.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Robot/selected_height.png
--rw-rw-rw-   0        0        0    40956 2024-04-08 04:32:22.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Robot/selected_robot_path.png
--rw-rw-rw-   0        0        0    21855 2024-04-08 04:32:24.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Robot/selected_scale.png
--rw-rw-rw-   0        0        0    21917 2024-04-08 04:32:27.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Robot/selected_width.png
--rw-rw-rw-   0        0        0    20843 2024-04-08 04:32:30.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Robot/width.png
-drwxrwxrwx   0        0        0        0 2024-05-15 04:54:14.060269 pythfinder-0.0.3.8/pythfinder/Images/Menu/Selection/
--rw-rw-rw-   0        0        0    19651 2024-04-06 15:09:11.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Selection/interface_button.png
--rw-rw-rw-   0        0        0    14899 2024-04-06 15:09:15.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Selection/other_button.png
--rw-rw-rw-   0        0        0    20750 2024-04-06 15:09:19.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Selection/pathing_button.png
--rw-rw-rw-   0        0        0    13645 2024-04-06 15:09:23.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Selection/robot_button.png
--rw-rw-rw-   0        0        0    16954 2024-04-06 15:09:26.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Selection/selected_interface_button.png
--rw-rw-rw-   0        0        0    13205 2024-04-06 15:09:28.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Selection/selected_other_button.png
--rw-rw-rw-   0        0        0    17797 2024-04-06 15:09:31.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Selection/selected_pathing_button.png
--rw-rw-rw-   0        0        0    12126 2024-04-06 15:09:33.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Selection/selected_robot_button.png
--rw-rw-rw-   0        0        0    11787 2024-04-06 15:09:36.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Selection/selected_trail_button.png
--rw-rw-rw-   0        0        0    79511 2024-04-06 15:09:38.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Selection/selection_menu.png
--rw-rw-rw-   0        0        0    13448 2024-04-06 15:09:41.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/Selection/trail_button.png
--rw-rw-rw-   0        0        0        0 2024-05-14 18:18:10.000000 pythfinder-0.0.3.8/pythfinder/Images/Menu/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 04:54:14.060269 pythfinder-0.0.3.8/pythfinder/Images/Robot/
--rw-rw-rw-   0        0        0        0 2024-05-14 18:18:58.000000 pythfinder-0.0.3.8/pythfinder/Images/Robot/__init__.py
--rw-rw-rw-   0        0        0   600926 2024-03-18 18:10:12.000000 pythfinder-0.0.3.8/pythfinder/Images/Robot/bot_from_above.png
-drwxrwxrwx   0        0        0        0 2024-05-15 04:54:14.075903 pythfinder-0.0.3.8/pythfinder/Images/Table/
--rw-rw-rw-   0        0        0  1025907 2024-04-29 12:07:29.000000 pythfinder-0.0.3.8/pythfinder/Images/Table/FLL_table_MP.jpg
--rw-rw-rw-   0        0        0        0 2024-05-14 18:19:06.000000 pythfinder-0.0.3.8/pythfinder/Images/Table/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-14 18:17:47.000000 pythfinder-0.0.3.8/pythfinder/Images/__init__.py
--rw-rw-rw-   0        0        0    16718 2024-04-07 11:58:49.000000 pythfinder-0.0.3.8/pythfinder/Images/none.png
--rw-rw-rw-   0        0        0    17665 2024-04-07 11:58:46.000000 pythfinder-0.0.3.8/pythfinder/Images/selected_none.png
-drwxrwxrwx   0        0        0        0 2024-05-15 04:54:14.107154 pythfinder-0.0.3.8/pythfinder/Trajectory/
--rw-rw-rw-   0        0        0      126 2024-05-14 05:34:50.000000 pythfinder-0.0.3.8/pythfinder/Trajectory/__init__.py
--rw-rw-rw-   0        0        0    52721 2024-05-14 16:09:04.000000 pythfinder-0.0.3.8/pythfinder/Trajectory/builder.py
--rw-rw-rw-   0        0        0     1709 2024-05-14 16:06:07.000000 pythfinder-0.0.3.8/pythfinder/Trajectory/feedback.py
--rw-rw-rw-   0        0        0     4366 2024-05-14 16:06:12.000000 pythfinder-0.0.3.8/pythfinder/Trajectory/feedforward.py
--rw-rw-rw-   0        0        0     1564 2024-05-14 16:06:17.000000 pythfinder-0.0.3.8/pythfinder/Trajectory/kinematics.py
--rw-rw-rw-   0        0        0     5914 2024-05-14 16:06:21.000000 pythfinder-0.0.3.8/pythfinder/Trajectory/splines.py
--rw-rw-rw-   0        0        0       98 2024-05-14 05:35:53.000000 pythfinder-0.0.3.8/pythfinder/__init__.py
--rw-rw-rw-   0        0        0    11119 2024-05-14 16:29:39.000000 pythfinder-0.0.3.8/pythfinder/core.py
-drwxrwxrwx   0        0        0        0 2024-05-15 04:54:13.674760 pythfinder-0.0.3.8/pythfinder.egg-info/
--rw-rw-rw-   0        0        0      310 2024-05-15 04:54:13.000000 pythfinder-0.0.3.8/pythfinder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4635 2024-05-15 04:54:13.000000 pythfinder-0.0.3.8/pythfinder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 04:54:13.000000 pythfinder-0.0.3.8/pythfinder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-15 04:54:13.000000 pythfinder-0.0.3.8/pythfinder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 04:54:14.107154 pythfinder-0.0.3.8/setup.cfg
--rw-rw-rw-   0        0        0      539 2024-05-15 04:54:05.000000 pythfinder-0.0.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 05:22:49.073823 pythfinder-0.0.3.9/
+-rw-rw-rw-   0        0        0     1295 2024-05-14 05:43:57.000000 pythfinder-0.0.3.9/LICENSE.txt
+-rw-rw-rw-   0        0        0       99 2024-05-15 04:25:24.000000 pythfinder-0.0.3.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      310 2024-05-15 05:22:49.073823 pythfinder-0.0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2024-05-14 18:26:37.000000 pythfinder-0.0.3.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 05:22:48.610583 pythfinder-0.0.3.9/pythfinder/
+drwxrwxrwx   0        0        0        0 2024-05-15 05:22:48.679597 pythfinder-0.0.3.9/pythfinder/Components/
+drwxrwxrwx   0        0        0        0 2024-05-15 05:22:48.695231 pythfinder-0.0.3.9/pythfinder/Components/BetterClasses/
+-rw-rw-rw-   0        0        0      102 2024-05-14 05:32:56.000000 pythfinder-0.0.3.9/pythfinder/Components/BetterClasses/__init__.py
+-rw-rw-rw-   0        0        0     1168 2024-05-13 14:52:24.000000 pythfinder-0.0.3.9/pythfinder/Components/BetterClasses/booleanEx.py
+-rw-rw-rw-   0        0        0      627 2024-05-13 14:52:55.000000 pythfinder-0.0.3.9/pythfinder/Components/BetterClasses/edgeDetectorEx.py
+-rw-rw-rw-   0        0        0     1140 2024-05-13 15:07:55.000000 pythfinder-0.0.3.9/pythfinder/Components/BetterClasses/errorEx.py
+-rw-rw-rw-   0        0        0     4862 2024-05-13 14:45:33.000000 pythfinder-0.0.3.9/pythfinder/Components/BetterClasses/mathEx.py
+drwxrwxrwx   0        0        0        0 2024-05-15 05:22:48.726483 pythfinder-0.0.3.9/pythfinder/Components/Constants/
+-rw-rw-rw-   0        0        0       78 2024-05-14 05:33:11.000000 pythfinder-0.0.3.9/pythfinder/Components/Constants/__init__.py
+-rw-rw-rw-   0        0        0    21294 2024-05-15 05:21:56.000000 pythfinder-0.0.3.9/pythfinder/Components/Constants/constants.py
+-rw-rw-rw-   0        0        0     2905 2024-05-13 15:08:14.000000 pythfinder-0.0.3.9/pythfinder/Components/Constants/constrains.py
+-rw-rw-rw-   0        0        0     2705 2024-05-13 15:11:03.000000 pythfinder-0.0.3.9/pythfinder/Components/Constants/screenSize.py
+drwxrwxrwx   0        0        0        0 2024-05-15 05:22:48.742108 pythfinder-0.0.3.9/pythfinder/Components/Controllers/
+-rw-rw-rw-   0        0        0      642 2024-05-13 15:12:44.000000 pythfinder-0.0.3.9/pythfinder/Components/Controllers/PIDCoefficients.py
+-rw-rw-rw-   0        0        0     1163 2024-05-14 16:07:14.000000 pythfinder-0.0.3.9/pythfinder/Components/Controllers/PIDController.py
+-rw-rw-rw-   0        0        0       60 2024-05-14 05:33:22.000000 pythfinder-0.0.3.9/pythfinder/Components/Controllers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 05:22:48.757735 pythfinder-0.0.3.9/pythfinder/Components/Menu/
+-rw-rw-rw-   0        0        0       87 2024-05-14 05:33:37.000000 pythfinder-0.0.3.9/pythfinder/Components/Menu/__init__.py
+-rw-rw-rw-   0        0        0    22248 2024-05-14 16:06:43.000000 pythfinder-0.0.3.9/pythfinder/Components/Menu/buttons.py
+-rw-rw-rw-   0        0        0     1583 2024-05-13 16:09:13.000000 pythfinder-0.0.3.9/pythfinder/Components/Menu/enums.py
+-rw-rw-rw-   0        0        0    22448 2024-05-14 16:06:48.000000 pythfinder-0.0.3.9/pythfinder/Components/Menu/main.py
+-rw-rw-rw-   0        0        0     4103 2024-05-14 16:07:01.000000 pythfinder-0.0.3.9/pythfinder/Components/Menu/menus.py
+-rw-rw-rw-   0        0        0      244 2024-05-14 05:35:39.000000 pythfinder-0.0.3.9/pythfinder/Components/__init__.py
+-rw-rw-rw-   0        0        0     5720 2024-05-14 16:04:43.000000 pythfinder-0.0.3.9/pythfinder/Components/background.py
+-rw-rw-rw-   0        0        0     9569 2024-05-14 16:05:08.000000 pythfinder-0.0.3.9/pythfinder/Components/controls.py
+-rw-rw-rw-   0        0        0     1853 2024-05-14 16:05:12.000000 pythfinder-0.0.3.9/pythfinder/Components/fade.py
+-rw-rw-rw-   0        0        0     9861 2024-05-14 15:58:30.000000 pythfinder-0.0.3.9/pythfinder/Components/robot.py
+-rw-rw-rw-   0        0        0     1975 2024-05-14 16:05:20.000000 pythfinder-0.0.3.9/pythfinder/Components/table.py
+-rw-rw-rw-   0        0        0     4633 2024-05-14 16:05:37.000000 pythfinder-0.0.3.9/pythfinder/Components/trail.py
+drwxrwxrwx   0        0        0        0 2024-05-15 05:22:48.773362 pythfinder-0.0.3.9/pythfinder/Images/
+drwxrwxrwx   0        0        0        0 2024-05-15 05:22:48.811132 pythfinder-0.0.3.9/pythfinder/Images/Controls/
+-rw-rw-rw-   0        0        0        0 2024-05-14 18:17:56.000000 pythfinder-0.0.3.9/pythfinder/Images/Controls/__init__.py
+-rw-rw-rw-   0        0        0   525562 2024-03-31 07:01:14.000000 pythfinder-0.0.3.9/pythfinder/Images/Controls/btn_backwards.png
+-rw-rw-rw-   0        0        0   530916 2024-03-31 07:01:10.000000 pythfinder-0.0.3.9/pythfinder/Images/Controls/btn_forwards.png
+-rw-rw-rw-   0        0        0   533042 2024-03-31 07:01:19.000000 pythfinder-0.0.3.9/pythfinder/Images/Controls/btn_hide_trail.png
+-rw-rw-rw-   0        0        0   561920 2024-03-31 14:58:53.000000 pythfinder-0.0.3.9/pythfinder/Images/Controls/btn_selecting_off.png
+-rw-rw-rw-   0        0        0   558616 2024-03-31 14:58:49.000000 pythfinder-0.0.3.9/pythfinder/Images/Controls/btn_selecting_on.png
+-rw-rw-rw-   0        0        0   531856 2024-03-31 07:00:59.000000 pythfinder-0.0.3.9/pythfinder/Images/Controls/btn_show_trail.png
+drwxrwxrwx   0        0        0        0 2024-05-15 05:22:48.811132 pythfinder-0.0.3.9/pythfinder/Images/Menu/
+drwxrwxrwx   0        0        0        0 2024-05-15 05:22:48.811132 pythfinder-0.0.3.9/pythfinder/Images/Menu/General/
+drwxrwxrwx   0        0        0        0 2024-05-15 05:22:48.574285 pythfinder-0.0.3.9/pythfinder/Images/Menu/General/Arrows/
+drwxrwxrwx   0        0        0        0 2024-05-15 05:22:48.826758 pythfinder-0.0.3.9/pythfinder/Images/Menu/General/Arrows/Left/
+-rw-rw-rw-   0        0        0     5149 2024-04-07 08:30:53.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/General/Arrows/Left/left_arrow.png
+-rw-rw-rw-   0        0        0     5334 2024-04-07 08:30:48.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/General/Arrows/Left/selected_left_arrow.png
+drwxrwxrwx   0        0        0        0 2024-05-15 05:22:48.842384 pythfinder-0.0.3.9/pythfinder/Images/Menu/General/Arrows/Right/
+-rw-rw-rw-   0        0        0     5181 2024-04-07 08:31:22.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/General/Arrows/Right/right_arrow.png
+-rw-rw-rw-   0        0        0     5279 2024-04-07 08:31:21.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/General/Arrows/Right/selected_right_arrow.png
+-rw-rw-rw-   0        0        0        0 2024-05-14 18:18:26.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/General/__init__.py
+-rw-rw-rw-   0        0        0   467492 2024-04-07 08:30:13.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/General/general_menu.png
+drwxrwxrwx   0        0        0        0 2024-05-15 05:22:48.858011 pythfinder-0.0.3.9/pythfinder/Images/Menu/Main/
+-rw-rw-rw-   0        0        0     8011 2024-04-05 16:14:53.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Main/menu_button.png
+-rw-rw-rw-   0        0        0     6208 2024-04-05 16:14:57.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Main/menu_home_button.png
+-rw-rw-rw-   0        0        0  1606752 2024-04-05 16:15:02.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Main/menu_main.png
+-rw-rw-rw-   0        0        0     8399 2024-04-06 11:39:50.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Main/selected_menu_button.png
+-rw-rw-rw-   0        0        0     6451 2024-04-06 11:39:46.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Main/selected_menu_home_button.png
+drwxrwxrwx   0        0        0        0 2024-05-15 05:22:48.873635 pythfinder-0.0.3.9/pythfinder/Images/Menu/Other/
+drwxrwxrwx   0        0        0        0 2024-05-15 05:22:48.895791 pythfinder-0.0.3.9/pythfinder/Images/Menu/Other/FieldCentric/
+-rw-rw-rw-   0        0        0    33821 2024-04-07 08:27:04.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Other/FieldCentric/field_centric_off.png
+-rw-rw-rw-   0        0        0    34053 2024-04-07 08:27:04.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Other/FieldCentric/field_centric_on.png
+-rw-rw-rw-   0        0        0    35325 2024-04-07 08:27:04.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Other/FieldCentric/selected_field_centric_off.png
+-rw-rw-rw-   0        0        0    35522 2024-04-07 08:27:04.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Other/FieldCentric/selected_field_centric_on.png
+drwxrwxrwx   0        0        0        0 2024-05-15 05:22:48.911415 pythfinder-0.0.3.9/pythfinder/Images/Menu/Other/RobotBorder/
+-rw-rw-rw-   0        0        0    32516 2024-04-07 08:27:48.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Other/RobotBorder/robot_border_off.png
+-rw-rw-rw-   0        0        0    32757 2024-04-07 08:27:49.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Other/RobotBorder/robot_border_on.png
+-rw-rw-rw-   0        0        0    33964 2024-04-07 08:27:48.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Other/RobotBorder/selected_robot_border_off.png
+-rw-rw-rw-   0        0        0    34153 2024-04-07 08:27:48.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Other/RobotBorder/selected_robot_border_on.png
+drwxrwxrwx   0        0        0        0 2024-05-15 05:22:48.927043 pythfinder-0.0.3.9/pythfinder/Images/Menu/Other/ScreenBorder/
+-rw-rw-rw-   0        0        0    34863 2024-04-07 08:28:53.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Other/ScreenBorder/screen_border_off.png
+-rw-rw-rw-   0        0        0    35031 2024-04-07 08:28:53.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Other/ScreenBorder/screen_border_on.png
+-rw-rw-rw-   0        0        0    36547 2024-04-07 08:28:53.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Other/ScreenBorder/selected_screen_border_off.png
+-rw-rw-rw-   0        0        0    36670 2024-04-07 08:28:53.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Other/ScreenBorder/selected_screen_border_on.png
+-rw-rw-rw-   0        0        0    20270 2024-04-09 17:13:50.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Other/other_indicator.png
+-rw-rw-rw-   0        0        0    13339 2024-04-07 08:29:32.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Other/other_quadrant.png
+drwxrwxrwx   0        0        0        0 2024-05-15 05:22:48.980050 pythfinder-0.0.3.9/pythfinder/Images/Menu/Robot/
+-rw-rw-rw-   0        0        0    28975 2024-04-08 04:32:03.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Robot/height.png
+-rw-rw-rw-   0        0        0    20193 2024-04-08 04:32:07.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Robot/robot_indicator.png
+-rw-rw-rw-   0        0        0    39077 2024-04-08 04:32:04.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Robot/robot_path.png
+-rw-rw-rw-   0        0        0   138988 2024-04-08 04:32:10.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Robot/robot_path_quadrant.png
+-rw-rw-rw-   0        0        0   115045 2024-04-08 04:32:12.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Robot/robot_specs_quadrant.png
+-rw-rw-rw-   0        0        0    20716 2024-04-08 04:32:17.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Robot/scale.png
+-rw-rw-rw-   0        0        0    30701 2024-04-08 04:32:20.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Robot/selected_height.png
+-rw-rw-rw-   0        0        0    40956 2024-04-08 04:32:22.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Robot/selected_robot_path.png
+-rw-rw-rw-   0        0        0    21855 2024-04-08 04:32:24.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Robot/selected_scale.png
+-rw-rw-rw-   0        0        0    21917 2024-04-08 04:32:27.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Robot/selected_width.png
+-rw-rw-rw-   0        0        0    20843 2024-04-08 04:32:30.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Robot/width.png
+drwxrwxrwx   0        0        0        0 2024-05-15 05:22:49.026947 pythfinder-0.0.3.9/pythfinder/Images/Menu/Selection/
+-rw-rw-rw-   0        0        0    19651 2024-04-06 15:09:11.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Selection/interface_button.png
+-rw-rw-rw-   0        0        0    14899 2024-04-06 15:09:15.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Selection/other_button.png
+-rw-rw-rw-   0        0        0    20750 2024-04-06 15:09:19.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Selection/pathing_button.png
+-rw-rw-rw-   0        0        0    13645 2024-04-06 15:09:23.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Selection/robot_button.png
+-rw-rw-rw-   0        0        0    16954 2024-04-06 15:09:26.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Selection/selected_interface_button.png
+-rw-rw-rw-   0        0        0    13205 2024-04-06 15:09:28.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Selection/selected_other_button.png
+-rw-rw-rw-   0        0        0    17797 2024-04-06 15:09:31.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Selection/selected_pathing_button.png
+-rw-rw-rw-   0        0        0    12126 2024-04-06 15:09:33.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Selection/selected_robot_button.png
+-rw-rw-rw-   0        0        0    11787 2024-04-06 15:09:36.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Selection/selected_trail_button.png
+-rw-rw-rw-   0        0        0    79511 2024-04-06 15:09:38.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Selection/selection_menu.png
+-rw-rw-rw-   0        0        0    13448 2024-04-06 15:09:41.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/Selection/trail_button.png
+-rw-rw-rw-   0        0        0        0 2024-05-14 18:18:10.000000 pythfinder-0.0.3.9/pythfinder/Images/Menu/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 05:22:49.026947 pythfinder-0.0.3.9/pythfinder/Images/Robot/
+-rw-rw-rw-   0        0        0        0 2024-05-14 18:18:58.000000 pythfinder-0.0.3.9/pythfinder/Images/Robot/__init__.py
+-rw-rw-rw-   0        0        0   600926 2024-03-18 18:10:12.000000 pythfinder-0.0.3.9/pythfinder/Images/Robot/bot_from_above.png
+drwxrwxrwx   0        0        0        0 2024-05-15 05:22:49.042571 pythfinder-0.0.3.9/pythfinder/Images/Table/
+-rw-rw-rw-   0        0        0  1025907 2024-04-29 12:07:29.000000 pythfinder-0.0.3.9/pythfinder/Images/Table/FLL_table_MP.jpg
+-rw-rw-rw-   0        0        0        0 2024-05-14 18:19:06.000000 pythfinder-0.0.3.9/pythfinder/Images/Table/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-14 18:17:47.000000 pythfinder-0.0.3.9/pythfinder/Images/__init__.py
+-rw-rw-rw-   0        0        0    16718 2024-04-07 11:58:49.000000 pythfinder-0.0.3.9/pythfinder/Images/none.png
+-rw-rw-rw-   0        0        0    17665 2024-04-07 11:58:46.000000 pythfinder-0.0.3.9/pythfinder/Images/selected_none.png
+drwxrwxrwx   0        0        0        0 2024-05-15 05:22:49.058200 pythfinder-0.0.3.9/pythfinder/Trajectory/
+-rw-rw-rw-   0        0        0      126 2024-05-14 05:34:50.000000 pythfinder-0.0.3.9/pythfinder/Trajectory/__init__.py
+-rw-rw-rw-   0        0        0    52721 2024-05-14 16:09:04.000000 pythfinder-0.0.3.9/pythfinder/Trajectory/builder.py
+-rw-rw-rw-   0        0        0     1709 2024-05-14 16:06:07.000000 pythfinder-0.0.3.9/pythfinder/Trajectory/feedback.py
+-rw-rw-rw-   0        0        0     4366 2024-05-14 16:06:12.000000 pythfinder-0.0.3.9/pythfinder/Trajectory/feedforward.py
+-rw-rw-rw-   0        0        0     1564 2024-05-14 16:06:17.000000 pythfinder-0.0.3.9/pythfinder/Trajectory/kinematics.py
+-rw-rw-rw-   0        0        0     5914 2024-05-14 16:06:21.000000 pythfinder-0.0.3.9/pythfinder/Trajectory/splines.py
+-rw-rw-rw-   0        0        0       98 2024-05-14 05:35:53.000000 pythfinder-0.0.3.9/pythfinder/__init__.py
+-rw-rw-rw-   0        0        0    11119 2024-05-14 16:29:39.000000 pythfinder-0.0.3.9/pythfinder/core.py
+drwxrwxrwx   0        0        0        0 2024-05-15 05:22:48.641836 pythfinder-0.0.3.9/pythfinder.egg-info/
+-rw-rw-rw-   0        0        0      310 2024-05-15 05:22:48.000000 pythfinder-0.0.3.9/pythfinder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4635 2024-05-15 05:22:48.000000 pythfinder-0.0.3.9/pythfinder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 05:22:48.000000 pythfinder-0.0.3.9/pythfinder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-15 05:22:48.000000 pythfinder-0.0.3.9/pythfinder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 05:22:49.073823 pythfinder-0.0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0      539 2024-05-15 05:22:31.000000 pythfinder-0.0.3.9/setup.py
```

### Comparing `pythfinder-0.0.3.8/LICENSE.txt` & `pythfinder-0.0.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Components/BetterClasses/booleanEx.py` & `pythfinder-0.0.3.9/pythfinder/Components/BetterClasses/booleanEx.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Components/BetterClasses/edgeDetectorEx.py` & `pythfinder-0.0.3.9/pythfinder/Components/BetterClasses/edgeDetectorEx.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Components/BetterClasses/errorEx.py` & `pythfinder-0.0.3.9/pythfinder/Components/BetterClasses/errorEx.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Components/BetterClasses/mathEx.py` & `pythfinder-0.0.3.9/pythfinder/Components/BetterClasses/mathEx.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Components/Constants/constants.py` & `pythfinder-0.0.3.9/pythfinder/Components/Constants/constants.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,25 +2,28 @@
 from pythfinder.Components.BetterClasses.booleanEx import *
 from pythfinder.Components.Constants.screenSize import *
 from pythfinder.Components.Constants.constrains import *
 from pythfinder.Components.BetterClasses.mathEx import *
 
 import pygame
 import math
+import os
 
 # file containing:
 #           - default constant values, image manipulation for the interface and Constants class
 #           - default keys for joystick control
 #           - helper methods for conversion
 
+script_dir = os.path.dirname(__file__)
+script_dir = os.path.join(script_dir, '..', '..', 'Images')
 
 default_robot_image_name = 'bot_from_above'
-default_robot_image_path = '/pythfinder/Images/Robot/'
+default_robot_image_path = 'Robot/'
 default_robot_image_extension = 'png'
-default_robot_image_source = '/pythfinder/Images/Robot/bot_from_above.png'
+default_robot_image_source = 'Robot/bot_from_above.png'
 
 default_robot_scaling_factor = 1
 default_robot_height_cm = 20
 default_robot_width_cm = 15 
 default_robot_real_max_velocity = 27.7 # cm/s
 
 default_coordinate_system_color = "white"
@@ -326,149 +329,149 @@
 
 
 
 
 
 
 
-img_main_menu_source = "/pythfinder/Images/Menu/Main/menu_main.png"
-img_forwards_source = "/pythfinder/Images/Controls/btn_forwards.png"
-img_backwards_source = "/pythfinder/Images/Controls/btn_backwards.png"
-img_menu_button_source = "/pythfinder/Images/Menu/Main/menu_button.png"
-img_show_trail_source = "/pythfinder/Images/Controls/btn_show_trail.png"
-img_hide_trail_source = "/pythfinder/Images/Controls/btn_hide_trail.png"
-img_home_button_source = "/pythfinder/Images/Menu/Main/menu_home_button.png"
-img_selecting_on_source = "/pythfinder/Images/Controls/btn_selecting_on.png"
-img_selecting_off_source = "/pythfinder/Images/Controls/btn_selecting_off.png"
-img_selected_menu_button_source = "/pythfinder/Images/Menu/Main/selected_menu_button.png"
-img_selected_home_button_source = "/pythfinder/Images/Menu/Main/selected_menu_home_button.png"
-
-
-img_other_button_source = "/pythfinder/Images/Menu/Selection/other_button.png"
-img_robot_button_source = "/pythfinder/Images/Menu/Selection/robot_button.png"
-img_trail_button_source = "/pythfinder/Images/Menu/Selection/trail_button.png"
-img_selection_menu_source = "/pythfinder/Images/Menu/Selection/selection_menu.png"
-img_pathing_button_source = "/pythfinder/Images/Menu/Selection/pathing_button.png"
-img_interface_button_source = "/pythfinder/Images/Menu/Selection/interface_button.png"
-img_selected_other_button_source = "/pythfinder/Images/Menu/Selection/selected_other_button.png"
-img_selected_robot_button_source = "/pythfinder/Images/Menu/Selection/selected_robot_button.png"
-img_selected_trail_button_source = "/pythfinder/Images/Menu/Selection/selected_trail_button.png"
-img_selected_pathing_button_source = "/pythfinder/Images/Menu/Selection/selected_pathing_button.png"
-img_selected_interface_button_source = "/pythfinder/Images/Menu/Selection/selected_interface_button.png"
-
-
-img_general_menu_source = "/pythfinder/Images/Menu/General/general_menu.png"
-img_left_arrow_source = "/pythfinder/Images/Menu/General/Arrows/Left/left_arrow.png"
-img_right_arrow_source = "/pythfinder/Images/Menu/General/Arrows/Right/right_arrow.png"
-img_selected_left_arrow_source = "/pythfinder/Images/Menu/General/Arrows/Left/selected_left_arrow.png"
-img_selected_right_arrow_source = "/pythfinder/Images/Menu/General/Arrows/Right/selected_right_arrow.png"
-
-
-img_other_quadrant_source = "/pythfinder/Images/Menu/Other/other_quadrant.png"
-img_selected_none_source = "/pythfinder/Images/selected_none.png"
-img_none_source = "/pythfinder/Images/none.png"
-
-
-img_field_centric_on_source = "/pythfinder/Images/Menu/Other/FieldCentric/field_centric_on.png"
-img_field_centric_off_source = "/pythfinder/Images/Menu/Other/FieldCentric/field_centric_off.png"
-img_selected_field_centric_on_source = "/pythfinder/Images/Menu/Other/FieldCentric/selected_field_centric_on.png"
-img_selected_field_centric_off_source = "/pythfinder/Images/Menu/Other/FieldCentric/selected_field_centric_off.png"
-
-
-img_robot_border_on_source = "/pythfinder/Images/Menu/Other/RobotBorder/robot_border_on.png"
-img_robot_border_off_source = "/pythfinder/Images/Menu/Other/RobotBorder/robot_border_off.png"
-img_selected_robot_border_on_source = "/pythfinder/Images/Menu/Other/RobotBorder/selected_robot_border_on.png"
-img_selected_robot_border_off_source = "/pythfinder/Images/Menu/Other/RobotBorder/selected_robot_border_off.png"
-
-
-img_screen_border_on_source = "/pythfinder/Images/Menu/Other/ScreenBorder/screen_border_on.png"
-img_screen_border_off_source = "/pythfinder/Images/Menu/Other/ScreenBorder/screen_border_off.png"
-img_selected_screen_border_on_source = "/pythfinder/Images/Menu/Other/ScreenBorder/selected_screen_border_on.png"
-img_selected_screen_border_off_source = "/pythfinder/Images/Menu/Other/ScreenBorder/selected_screen_border_off.png"
-
-
-img_scale_source = "/pythfinder/Images/Menu/Robot/scale.png"
-img_width_source = "/pythfinder/Images/Menu/Robot/width.png"
-img_height_source = "/pythfinder/Images/Menu/Robot/height.png"
-img_robot_image_path_source = "/pythfinder/Images/Menu/Robot/robot_path.png"
-img_selected_scale_source = "/pythfinder/Images/Menu/Robot/selected_scale.png"
-img_selected_width_source = "/pythfinder/Images/Menu/Robot/selected_width.png"
-img_selected_height_source = "/pythfinder/Images/Menu/Robot/selected_height.png"
-img_path_quadrant_source = "/pythfinder/Images/Menu/Robot/robot_path_quadrant.png"
-img_specs_quadrant_source = "/pythfinder/Images/Menu/Robot/robot_specs_quadrant.png"
-img_selected_robot_image_path_source = "/pythfinder/Images/Menu/Robot/selected_robot_path.png"
-
-img_robot_indicator_source = "/pythfinder/Images/Menu/Robot/robot_indicator.png"
-img_other_indicator_source = "/pythfinder/Images/Menu/Other/other_indicator.png"
-
-
-img_forwards = pygame.image.load(img_forwards_source)
-img_main_menu = pygame.image.load(img_main_menu_source)
-img_backwards = pygame.image.load(img_backwards_source)
-img_show_trail = pygame.image.load(img_show_trail_source)
-img_hide_trail = pygame.image.load(img_hide_trail_source)
-img_menu_button = pygame.image.load(img_menu_button_source)
-img_home_button = pygame.image.load(img_home_button_source)
-img_selecting_on = pygame.image.load(img_selecting_on_source)
-img_selecting_off = pygame.image.load(img_selecting_off_source)
-img_selected_menu_button = pygame.image.load(img_selected_menu_button_source)
-img_selected_home_button = pygame.image.load(img_selected_home_button_source)
-
-
-img_other_button = pygame.image.load(img_other_button_source)
-img_robot_button = pygame.image.load(img_robot_button_source)
-img_trail_button = pygame.image.load(img_trail_button_source)
-img_pathing_button= pygame.image.load(img_pathing_button_source)
-img_selection_menu = pygame.image.load(img_selection_menu_source)
-img_interface_button = pygame.image.load(img_interface_button_source)
-img_selected_other_button= pygame.image.load(img_selected_other_button_source)
-img_selected_robot_button = pygame.image.load(img_selected_robot_button_source)
-img_selected_trail_button = pygame.image.load(img_selected_trail_button_source)
-img_selected_pathing_button = pygame.image.load(img_selected_pathing_button_source)
-img_selected_interface_button= pygame.image.load(img_selected_interface_button_source)
-
-
-img_general_menu = pygame.image.load(img_general_menu_source)
-img_left_arrow = pygame.image.load(img_left_arrow_source)
-img_right_arrow = pygame.image.load(img_right_arrow_source)
-img_selected_left_arrow = pygame.image.load(img_selected_left_arrow_source)
-img_selected_right_arrow = pygame.image.load(img_selected_right_arrow_source)
-
-img_other_quadrant = pygame.image.load(img_other_quadrant_source)
-img_selected_none = pygame.image.load(img_selected_none_source)
-img_none = pygame.image.load(img_none_source)
-
-img_field_centric_on = pygame.image.load(img_field_centric_on_source)
-img_field_centric_off = pygame.image.load(img_field_centric_off_source)
-img_selected_field_centric_on = pygame.image.load(img_selected_field_centric_on_source)
-img_selected_field_centric_off = pygame.image.load(img_selected_field_centric_off_source)
-
-img_robot_border_on = pygame.image.load(img_robot_border_on_source)
-img_robot_border_off = pygame.image.load(img_robot_border_off_source)
-img_selected_robot_border_on = pygame.image.load(img_selected_robot_border_on_source)
-img_selected_robot_border_off = pygame.image.load(img_selected_robot_border_off_source)
-
-img_screen_border_on = pygame.image.load(img_screen_border_on_source)
-img_screen_border_off = pygame.image.load(img_screen_border_off_source)
-img_selected_screen_border_on = pygame.image.load(img_selected_screen_border_on_source)
-img_selected_screen_border_off = pygame.image.load(img_selected_screen_border_off_source)
-
-img_scale = pygame.image.load(img_scale_source)
-img_width = pygame.image.load(img_width_source)
-img_height = pygame.image.load(img_height_source)
-img_path_quadrant = pygame.image.load(img_path_quadrant_source)
-img_specs_quadrant = pygame.image.load(img_specs_quadrant_source)
-img_selected_scale = pygame.image.load(img_selected_scale_source)
-img_selected_width = pygame.image.load(img_selected_width_source)
-img_selected_height = pygame.image.load(img_selected_height_source)
-img_robot_image_path = pygame.image.load(img_robot_image_path_source)
-img_selected_robot_image_path = pygame.image.load(img_selected_robot_image_path_source)
+img_main_menu_source = "Menu/Main/menu_main.png"
+img_forwards_source = "Controls/btn_forwards.png"
+img_backwards_source = "Controls/btn_backwards.png"
+img_menu_button_source = "Menu/Main/menu_button.png"
+img_show_trail_source = "Controls/btn_show_trail.png"
+img_hide_trail_source = "Controls/btn_hide_trail.png"
+img_home_button_source = "Menu/Main/menu_home_button.png"
+img_selecting_on_source = "Controls/btn_selecting_on.png"
+img_selecting_off_source = "Controls/btn_selecting_off.png"
+img_selected_menu_button_source = "Menu/Main/selected_menu_button.png"
+img_selected_home_button_source = "Menu/Main/selected_menu_home_button.png"
+
+
+img_other_button_source = "Menu/Selection/other_button.png"
+img_robot_button_source = "Menu/Selection/robot_button.png"
+img_trail_button_source = "Menu/Selection/trail_button.png"
+img_selection_menu_source = "Menu/Selection/selection_menu.png"
+img_pathing_button_source = "Menu/Selection/pathing_button.png"
+img_interface_button_source = "Menu/Selection/interface_button.png"
+img_selected_other_button_source = "Menu/Selection/selected_other_button.png"
+img_selected_robot_button_source = "Menu/Selection/selected_robot_button.png"
+img_selected_trail_button_source = "Menu/Selection/selected_trail_button.png"
+img_selected_pathing_button_source = "Menu/Selection/selected_pathing_button.png"
+img_selected_interface_button_source = "Menu/Selection/selected_interface_button.png"
+
+
+img_general_menu_source = "Menu/General/general_menu.png"
+img_left_arrow_source = "Menu/General/Arrows/Left/left_arrow.png"
+img_right_arrow_source = "Menu/General/Arrows/Right/right_arrow.png"
+img_selected_left_arrow_source = "Menu/General/Arrows/Left/selected_left_arrow.png"
+img_selected_right_arrow_source = "Menu/General/Arrows/Right/selected_right_arrow.png"
+
+
+img_other_quadrant_source = "Menu/Other/other_quadrant.png"
+img_selected_none_source = "selected_none.png"
+img_none_source = "none.png"
+
+
+img_field_centric_on_source = "Menu/Other/FieldCentric/field_centric_on.png"
+img_field_centric_off_source = "Menu/Other/FieldCentric/field_centric_off.png"
+img_selected_field_centric_on_source = "Menu/Other/FieldCentric/selected_field_centric_on.png"
+img_selected_field_centric_off_source = "Menu/Other/FieldCentric/selected_field_centric_off.png"
+
+
+img_robot_border_on_source = "Menu/Other/RobotBorder/robot_border_on.png"
+img_robot_border_off_source = "Menu/Other/RobotBorder/robot_border_off.png"
+img_selected_robot_border_on_source = "Menu/Other/RobotBorder/selected_robot_border_on.png"
+img_selected_robot_border_off_source = "Menu/Other/RobotBorder/selected_robot_border_off.png"
+
+
+img_screen_border_on_source = "Menu/Other/ScreenBorder/screen_border_on.png"
+img_screen_border_off_source = "Menu/Other/ScreenBorder/screen_border_off.png"
+img_selected_screen_border_on_source = "Menu/Other/ScreenBorder/selected_screen_border_on.png"
+img_selected_screen_border_off_source = "Menu/Other/ScreenBorder/selected_screen_border_off.png"
+
+
+img_scale_source = "Menu/Robot/scale.png"
+img_width_source = "Menu/Robot/width.png"
+img_height_source = "Menu/Robot/height.png"
+img_robot_image_path_source = "Menu/Robot/robot_path.png"
+img_selected_scale_source = "Menu/Robot/selected_scale.png"
+img_selected_width_source = "Menu/Robot/selected_width.png"
+img_selected_height_source = "Menu/Robot/selected_height.png"
+img_path_quadrant_source = "Menu/Robot/robot_path_quadrant.png"
+img_specs_quadrant_source = "Menu/Robot/robot_specs_quadrant.png"
+img_selected_robot_image_path_source = "Menu/Robot/selected_robot_path.png"
+
+img_robot_indicator_source = "Menu/Robot/robot_indicator.png"
+img_other_indicator_source = "Menu/Other/other_indicator.png"
+
+
+img_forwards = pygame.image.load(os.path.join(script_dir, img_forwards_source))
+img_main_menu = pygame.image.load(os.path.join(script_dir, img_main_menu_source))
+img_backwards = pygame.image.load(os.path.join(script_dir, img_backwards_source))
+img_show_trail = pygame.image.load(os.path.join(script_dir, img_show_trail_source))
+img_hide_trail = pygame.image.load(os.path.join(script_dir, img_hide_trail_source))
+img_menu_button = pygame.image.load(os.path.join(script_dir, img_menu_button_source))
+img_home_button = pygame.image.load(os.path.join(script_dir, img_home_button_source))
+img_selecting_on = pygame.image.load(os.path.join(script_dir, img_selecting_on_source))
+img_selecting_off = pygame.image.load(os.path.join(script_dir, img_selecting_off_source))
+img_selected_menu_button = pygame.image.load(os.path.join(script_dir, img_selected_menu_button_source))
+img_selected_home_button = pygame.image.load(os.path.join(script_dir, img_selected_home_button_source))
+
+
+img_other_button = pygame.image.load(os.path.join(script_dir, img_other_button_source))
+img_robot_button = pygame.image.load(os.path.join(script_dir, img_robot_button_source))
+img_trail_button = pygame.image.load(os.path.join(script_dir, img_trail_button_source))
+img_pathing_button= pygame.image.load(os.path.join(script_dir, img_pathing_button_source))
+img_selection_menu = pygame.image.load(os.path.join(script_dir, img_selection_menu_source))
+img_interface_button = pygame.image.load(os.path.join(script_dir, img_interface_button_source))
+img_selected_other_button= pygame.image.load(os.path.join(script_dir, img_selected_other_button_source))
+img_selected_robot_button = pygame.image.load(os.path.join(script_dir, img_selected_robot_button_source))
+img_selected_trail_button = pygame.image.load(os.path.join(script_dir, img_selected_trail_button_source))
+img_selected_pathing_button = pygame.image.load(os.path.join(script_dir, img_selected_pathing_button_source))
+img_selected_interface_button= pygame.image.load(os.path.join(script_dir, img_selected_interface_button_source))
+
+
+img_general_menu = pygame.image.load(os.path.join(script_dir, img_general_menu_source))
+img_left_arrow = pygame.image.load(os.path.join(script_dir, img_left_arrow_source))
+img_right_arrow = pygame.image.load(os.path.join(script_dir, img_right_arrow_source))
+img_selected_left_arrow = pygame.image.load(os.path.join(script_dir, img_selected_left_arrow_source))
+img_selected_right_arrow = pygame.image.load(os.path.join(script_dir, img_selected_right_arrow_source))
+
+img_other_quadrant = pygame.image.load(os.path.join(script_dir, img_other_quadrant_source))
+img_selected_none = pygame.image.load(os.path.join(script_dir, img_selected_none_source))
+img_none = pygame.image.load(os.path.join(script_dir, img_none_source))
+
+img_field_centric_on = pygame.image.load(os.path.join(script_dir, img_field_centric_on_source))
+img_field_centric_off = pygame.image.load(os.path.join(script_dir, img_field_centric_off_source))
+img_selected_field_centric_on = pygame.image.load(os.path.join(script_dir, img_selected_field_centric_on_source))
+img_selected_field_centric_off = pygame.image.load(os.path.join(script_dir, img_selected_field_centric_off_source))
+
+img_robot_border_on = pygame.image.load(os.path.join(script_dir, img_robot_border_on_source))
+img_robot_border_off = pygame.image.load(os.path.join(script_dir, img_robot_border_off_source))
+img_selected_robot_border_on = pygame.image.load(os.path.join(script_dir, img_selected_robot_border_on_source))
+img_selected_robot_border_off = pygame.image.load(os.path.join(script_dir, img_selected_robot_border_off_source))
+
+img_screen_border_on = pygame.image.load(os.path.join(script_dir, img_screen_border_on_source))
+img_screen_border_off = pygame.image.load(os.path.join(script_dir, img_screen_border_off_source))
+img_selected_screen_border_on = pygame.image.load(os.path.join(script_dir, img_selected_screen_border_on_source))
+img_selected_screen_border_off = pygame.image.load(os.path.join(script_dir, img_selected_screen_border_off_source))
+
+img_scale = pygame.image.load(os.path.join(script_dir, img_scale_source))
+img_width = pygame.image.load(os.path.join(script_dir, img_width_source))
+img_height = pygame.image.load(os.path.join(script_dir, img_height_source))
+img_path_quadrant = pygame.image.load(os.path.join(script_dir, img_path_quadrant_source))
+img_specs_quadrant = pygame.image.load(os.path.join(script_dir, img_specs_quadrant_source))
+img_selected_scale = pygame.image.load(os.path.join(script_dir, img_selected_scale_source))
+img_selected_width = pygame.image.load(os.path.join(script_dir, img_selected_width_source))
+img_selected_height = pygame.image.load(os.path.join(script_dir, img_selected_height_source))
+img_robot_image_path = pygame.image.load(os.path.join(script_dir, img_robot_image_path_source))
+img_selected_robot_image_path = pygame.image.load(os.path.join(script_dir, img_selected_robot_image_path_source))
 
-img_robot_indicator = pygame.image.load(img_robot_indicator_source)
-img_other_indicator = pygame.image.load(img_other_indicator_source)
+img_robot_indicator = pygame.image.load(os.path.join(script_dir, img_robot_indicator_source))
+img_other_indicator = pygame.image.load(os.path.join(script_dir, img_other_indicator_source))
 
 
 
 
 
 
 img_main_menu = pygame.transform.scale(img_main_menu, (900, 700))
@@ -533,16 +536,16 @@
 img_selected_scale = pygame.transform.scale(img_selected_scale, (170, 85))
 
 
 
 fll_table_width_cm = 227 # og - 93in
 fll_table_height_cm = 120 # og - 45in
 
-fll_table_source = '/pythfinder/Images/Table/FLL_table_MP.jpg'
-fll_table_image = pygame.image.load(fll_table_source)
+fll_table_source = 'Table/FLL_table_MP.jpg'
+fll_table_image = pygame.image.load(os.path.join(script_dir, fll_table_source))
 
 
 
 
 #pathing constants
 kP_head = 30
 kD_head = 1
```

### Comparing `pythfinder-0.0.3.8/pythfinder/Components/Constants/constrains.py` & `pythfinder-0.0.3.9/pythfinder/Components/Constants/constrains.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Components/Constants/screenSize.py` & `pythfinder-0.0.3.9/pythfinder/Components/Constants/screenSize.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Components/Controllers/PIDCoefficients.py` & `pythfinder-0.0.3.9/pythfinder/Components/Controllers/PIDCoefficients.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Components/Controllers/PIDController.py` & `pythfinder-0.0.3.9/pythfinder/Components/Controllers/PIDController.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Components/Menu/buttons.py` & `pythfinder-0.0.3.9/pythfinder/Components/Menu/buttons.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Components/Menu/enums.py` & `pythfinder-0.0.3.9/pythfinder/Components/Menu/enums.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Components/Menu/main.py` & `pythfinder-0.0.3.9/pythfinder/Components/Menu/main.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Components/Menu/menus.py` & `pythfinder-0.0.3.9/pythfinder/Components/Menu/menus.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Components/background.py` & `pythfinder-0.0.3.9/pythfinder/Components/background.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Components/controls.py` & `pythfinder-0.0.3.9/pythfinder/Components/controls.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Components/fade.py` & `pythfinder-0.0.3.9/pythfinder/Components/fade.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Components/robot.py` & `pythfinder-0.0.3.9/pythfinder/Components/robot.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Components/table.py` & `pythfinder-0.0.3.9/pythfinder/Components/table.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Components/trail.py` & `pythfinder-0.0.3.9/pythfinder/Components/trail.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Controls/btn_backwards.png` & `pythfinder-0.0.3.9/pythfinder/Images/Controls/btn_backwards.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Controls/btn_forwards.png` & `pythfinder-0.0.3.9/pythfinder/Images/Controls/btn_forwards.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Controls/btn_hide_trail.png` & `pythfinder-0.0.3.9/pythfinder/Images/Controls/btn_hide_trail.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Controls/btn_selecting_off.png` & `pythfinder-0.0.3.9/pythfinder/Images/Controls/btn_selecting_off.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Controls/btn_selecting_on.png` & `pythfinder-0.0.3.9/pythfinder/Images/Controls/btn_selecting_on.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Controls/btn_show_trail.png` & `pythfinder-0.0.3.9/pythfinder/Images/Controls/btn_show_trail.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/General/Arrows/Left/left_arrow.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/General/Arrows/Left/left_arrow.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/General/Arrows/Left/selected_left_arrow.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/General/Arrows/Left/selected_left_arrow.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/General/Arrows/Right/right_arrow.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/General/Arrows/Right/right_arrow.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/General/Arrows/Right/selected_right_arrow.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/General/Arrows/Right/selected_right_arrow.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/General/general_menu.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/General/general_menu.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Main/menu_button.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Main/menu_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Main/menu_home_button.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Main/menu_home_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Main/menu_main.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Main/menu_main.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Main/selected_menu_button.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Main/selected_menu_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Main/selected_menu_home_button.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Main/selected_menu_home_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Other/FieldCentric/field_centric_off.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Other/FieldCentric/field_centric_off.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Other/FieldCentric/field_centric_on.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Other/FieldCentric/field_centric_on.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Other/FieldCentric/selected_field_centric_off.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Other/FieldCentric/selected_field_centric_off.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Other/FieldCentric/selected_field_centric_on.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Other/FieldCentric/selected_field_centric_on.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Other/RobotBorder/robot_border_off.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Other/RobotBorder/robot_border_off.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Other/RobotBorder/robot_border_on.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Other/RobotBorder/robot_border_on.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Other/RobotBorder/selected_robot_border_off.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Other/RobotBorder/selected_robot_border_off.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Other/RobotBorder/selected_robot_border_on.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Other/RobotBorder/selected_robot_border_on.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Other/ScreenBorder/screen_border_off.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Other/ScreenBorder/screen_border_off.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Other/ScreenBorder/screen_border_on.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Other/ScreenBorder/screen_border_on.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Other/ScreenBorder/selected_screen_border_off.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Other/ScreenBorder/selected_screen_border_off.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Other/ScreenBorder/selected_screen_border_on.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Other/ScreenBorder/selected_screen_border_on.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Other/other_indicator.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Other/other_indicator.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Other/other_quadrant.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Other/other_quadrant.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Robot/height.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Robot/height.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Robot/robot_indicator.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Robot/robot_indicator.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Robot/robot_path.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Robot/robot_path.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Robot/robot_path_quadrant.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Robot/robot_path_quadrant.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Robot/robot_specs_quadrant.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Robot/robot_specs_quadrant.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Robot/scale.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Robot/scale.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Robot/selected_height.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Robot/selected_height.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Robot/selected_robot_path.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Robot/selected_robot_path.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Robot/selected_scale.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Robot/selected_scale.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Robot/selected_width.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Robot/selected_width.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Robot/width.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Robot/width.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Selection/interface_button.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Selection/interface_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Selection/other_button.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Selection/other_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Selection/pathing_button.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Selection/pathing_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Selection/robot_button.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Selection/robot_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Selection/selected_interface_button.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Selection/selected_interface_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Selection/selected_other_button.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Selection/selected_other_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Selection/selected_pathing_button.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Selection/selected_pathing_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Selection/selected_robot_button.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Selection/selected_robot_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Selection/selected_trail_button.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Selection/selected_trail_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Selection/selection_menu.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Selection/selection_menu.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Menu/Selection/trail_button.png` & `pythfinder-0.0.3.9/pythfinder/Images/Menu/Selection/trail_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Robot/bot_from_above.png` & `pythfinder-0.0.3.9/pythfinder/Images/Robot/bot_from_above.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/Table/FLL_table_MP.jpg` & `pythfinder-0.0.3.9/pythfinder/Images/Table/FLL_table_MP.jpg`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/none.png` & `pythfinder-0.0.3.9/pythfinder/Images/none.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Images/selected_none.png` & `pythfinder-0.0.3.9/pythfinder/Images/selected_none.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Trajectory/builder.py` & `pythfinder-0.0.3.9/pythfinder/Trajectory/builder.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Trajectory/feedback.py` & `pythfinder-0.0.3.9/pythfinder/Trajectory/feedback.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Trajectory/feedforward.py` & `pythfinder-0.0.3.9/pythfinder/Trajectory/feedforward.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Trajectory/kinematics.py` & `pythfinder-0.0.3.9/pythfinder/Trajectory/kinematics.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/Trajectory/splines.py` & `pythfinder-0.0.3.9/pythfinder/Trajectory/splines.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder/core.py` & `pythfinder-0.0.3.9/pythfinder/core.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/pythfinder.egg-info/SOURCES.txt` & `pythfinder-0.0.3.9/pythfinder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.8/setup.py` & `pythfinder-0.0.3.9/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pythfinder',
-    version='0.0.3.8',
+    version='0.0.3.9',
     license='MIT',
     author='Contraș Adrian',
     author_email='omegacoresincai@gmail.com',
     description='Motion Planning library designed for FLL teams',
     packages=find_packages(),
     keywords=[
         'motion-planning',
```

