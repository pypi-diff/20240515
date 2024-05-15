# Comparing `tmp/pythfinder-0.0.3.6.tar.gz` & `tmp/pythfinder-0.0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythfinder-0.0.3.6.tar", last modified: Tue May 14 18:34:03 2024, max compression
+gzip compressed data, was "pythfinder-0.0.3.7.tar", last modified: Wed May 15 04:33:46 2024, max compression
```

## Comparing `pythfinder-0.0.3.6.tar` & `pythfinder-0.0.3.7.tar`

### file list

```diff
@@ -1,62 +1,129 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 18:34:03.015740 pythfinder-0.0.3.6/
--rw-rw-rw-   0        0        0     1295 2024-05-14 05:43:57.000000 pythfinder-0.0.3.6/LICENSE.txt
--rw-rw-rw-   0        0        0      310 2024-05-14 18:34:03.015740 pythfinder-0.0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0      344 2024-05-14 18:26:37.000000 pythfinder-0.0.3.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 18:34:02.862066 pythfinder-0.0.3.6/pythfinder/
-drwxrwxrwx   0        0        0        0 2024-05-14 18:34:02.915465 pythfinder-0.0.3.6/pythfinder/Components/
-drwxrwxrwx   0        0        0        0 2024-05-14 18:34:02.931091 pythfinder-0.0.3.6/pythfinder/Components/BetterClasses/
--rw-rw-rw-   0        0        0      102 2024-05-14 05:32:56.000000 pythfinder-0.0.3.6/pythfinder/Components/BetterClasses/__init__.py
--rw-rw-rw-   0        0        0     1168 2024-05-13 14:52:24.000000 pythfinder-0.0.3.6/pythfinder/Components/BetterClasses/booleanEx.py
--rw-rw-rw-   0        0        0      627 2024-05-13 14:52:55.000000 pythfinder-0.0.3.6/pythfinder/Components/BetterClasses/edgeDetectorEx.py
--rw-rw-rw-   0        0        0     1140 2024-05-13 15:07:55.000000 pythfinder-0.0.3.6/pythfinder/Components/BetterClasses/errorEx.py
--rw-rw-rw-   0        0        0     4862 2024-05-13 14:45:33.000000 pythfinder-0.0.3.6/pythfinder/Components/BetterClasses/mathEx.py
-drwxrwxrwx   0        0        0        0 2024-05-14 18:34:02.946717 pythfinder-0.0.3.6/pythfinder/Components/Constants/
--rw-rw-rw-   0        0        0       78 2024-05-14 05:33:11.000000 pythfinder-0.0.3.6/pythfinder/Components/Constants/__init__.py
--rw-rw-rw-   0        0        0    20781 2024-05-14 18:06:58.000000 pythfinder-0.0.3.6/pythfinder/Components/Constants/constants.py
--rw-rw-rw-   0        0        0     2905 2024-05-13 15:08:14.000000 pythfinder-0.0.3.6/pythfinder/Components/Constants/constrains.py
--rw-rw-rw-   0        0        0     2705 2024-05-13 15:11:03.000000 pythfinder-0.0.3.6/pythfinder/Components/Constants/screenSize.py
-drwxrwxrwx   0        0        0        0 2024-05-14 18:34:02.962344 pythfinder-0.0.3.6/pythfinder/Components/Controllers/
--rw-rw-rw-   0        0        0      642 2024-05-13 15:12:44.000000 pythfinder-0.0.3.6/pythfinder/Components/Controllers/PIDCoefficients.py
--rw-rw-rw-   0        0        0     1163 2024-05-14 16:07:14.000000 pythfinder-0.0.3.6/pythfinder/Components/Controllers/PIDController.py
--rw-rw-rw-   0        0        0       60 2024-05-14 05:33:22.000000 pythfinder-0.0.3.6/pythfinder/Components/Controllers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 18:34:02.984478 pythfinder-0.0.3.6/pythfinder/Components/Menu/
--rw-rw-rw-   0        0        0       87 2024-05-14 05:33:37.000000 pythfinder-0.0.3.6/pythfinder/Components/Menu/__init__.py
--rw-rw-rw-   0        0        0    22248 2024-05-14 16:06:43.000000 pythfinder-0.0.3.6/pythfinder/Components/Menu/buttons.py
--rw-rw-rw-   0        0        0     1583 2024-05-13 16:09:13.000000 pythfinder-0.0.3.6/pythfinder/Components/Menu/enums.py
--rw-rw-rw-   0        0        0    22448 2024-05-14 16:06:48.000000 pythfinder-0.0.3.6/pythfinder/Components/Menu/main.py
--rw-rw-rw-   0        0        0     4103 2024-05-14 16:07:01.000000 pythfinder-0.0.3.6/pythfinder/Components/Menu/menus.py
--rw-rw-rw-   0        0        0      244 2024-05-14 05:35:39.000000 pythfinder-0.0.3.6/pythfinder/Components/__init__.py
--rw-rw-rw-   0        0        0     5720 2024-05-14 16:04:43.000000 pythfinder-0.0.3.6/pythfinder/Components/background.py
--rw-rw-rw-   0        0        0     9569 2024-05-14 16:05:08.000000 pythfinder-0.0.3.6/pythfinder/Components/controls.py
--rw-rw-rw-   0        0        0     1853 2024-05-14 16:05:12.000000 pythfinder-0.0.3.6/pythfinder/Components/fade.py
--rw-rw-rw-   0        0        0     9861 2024-05-14 15:58:30.000000 pythfinder-0.0.3.6/pythfinder/Components/robot.py
--rw-rw-rw-   0        0        0     1975 2024-05-14 16:05:20.000000 pythfinder-0.0.3.6/pythfinder/Components/table.py
--rw-rw-rw-   0        0        0     4633 2024-05-14 16:05:37.000000 pythfinder-0.0.3.6/pythfinder/Components/trail.py
-drwxrwxrwx   0        0        0        0 2024-05-14 18:34:02.984478 pythfinder-0.0.3.6/pythfinder/Images/
-drwxrwxrwx   0        0        0        0 2024-05-14 18:34:02.984478 pythfinder-0.0.3.6/pythfinder/Images/Controls/
--rw-rw-rw-   0        0        0        0 2024-05-14 18:17:56.000000 pythfinder-0.0.3.6/pythfinder/Images/Controls/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 18:34:03.000114 pythfinder-0.0.3.6/pythfinder/Images/Menu/
-drwxrwxrwx   0        0        0        0 2024-05-14 18:34:03.000114 pythfinder-0.0.3.6/pythfinder/Images/Menu/General/
--rw-rw-rw-   0        0        0        0 2024-05-14 18:18:26.000000 pythfinder-0.0.3.6/pythfinder/Images/Menu/General/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-14 18:18:10.000000 pythfinder-0.0.3.6/pythfinder/Images/Menu/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 18:34:03.000114 pythfinder-0.0.3.6/pythfinder/Images/Robot/
--rw-rw-rw-   0        0        0        0 2024-05-14 18:18:58.000000 pythfinder-0.0.3.6/pythfinder/Images/Robot/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 18:34:03.000114 pythfinder-0.0.3.6/pythfinder/Images/Table/
--rw-rw-rw-   0        0        0        0 2024-05-14 18:19:06.000000 pythfinder-0.0.3.6/pythfinder/Images/Table/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-14 18:17:47.000000 pythfinder-0.0.3.6/pythfinder/Images/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 18:34:03.015740 pythfinder-0.0.3.6/pythfinder/Trajectory/
--rw-rw-rw-   0        0        0      126 2024-05-14 05:34:50.000000 pythfinder-0.0.3.6/pythfinder/Trajectory/__init__.py
--rw-rw-rw-   0        0        0    52721 2024-05-14 16:09:04.000000 pythfinder-0.0.3.6/pythfinder/Trajectory/builder.py
--rw-rw-rw-   0        0        0     1709 2024-05-14 16:06:07.000000 pythfinder-0.0.3.6/pythfinder/Trajectory/feedback.py
--rw-rw-rw-   0        0        0     4366 2024-05-14 16:06:12.000000 pythfinder-0.0.3.6/pythfinder/Trajectory/feedforward.py
--rw-rw-rw-   0        0        0     1564 2024-05-14 16:06:17.000000 pythfinder-0.0.3.6/pythfinder/Trajectory/kinematics.py
--rw-rw-rw-   0        0        0     5914 2024-05-14 16:06:21.000000 pythfinder-0.0.3.6/pythfinder/Trajectory/splines.py
--rw-rw-rw-   0        0        0       98 2024-05-14 05:35:53.000000 pythfinder-0.0.3.6/pythfinder/__init__.py
--rw-rw-rw-   0        0        0    11119 2024-05-14 16:29:39.000000 pythfinder-0.0.3.6/pythfinder/core.py
-drwxrwxrwx   0        0        0        0 2024-05-14 18:34:02.884207 pythfinder-0.0.3.6/pythfinder.egg-info/
--rw-rw-rw-   0        0        0      310 2024-05-14 18:34:02.000000 pythfinder-0.0.3.6/pythfinder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1620 2024-05-14 18:34:02.000000 pythfinder-0.0.3.6/pythfinder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 18:34:02.000000 pythfinder-0.0.3.6/pythfinder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-14 18:34:02.000000 pythfinder-0.0.3.6/pythfinder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 18:34:03.015740 pythfinder-0.0.3.6/setup.cfg
--rw-rw-rw-   0        0        0      938 2024-05-14 18:33:37.000000 pythfinder-0.0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 04:30:36.674509 pythfinder-0.0.3.7/
+-rw-rw-rw-   0        0        0     1295 2024-05-14 05:43:57.000000 pythfinder-0.0.3.7/LICENSE.txt
+-rw-rw-rw-   0        0        0       99 2024-05-15 04:25:24.000000 pythfinder-0.0.3.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      310 2024-05-15 04:33:46.538623 pythfinder-0.0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2024-05-14 18:26:37.000000 pythfinder-0.0.3.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 04:30:36.025891 pythfinder-0.0.3.7/pythfinder/
+drwxrwxrwx   0        0        0        0 2024-05-15 04:30:36.141846 pythfinder-0.0.3.7/pythfinder/Components/
+drwxrwxrwx   0        0        0        0 2024-05-15 04:30:36.157474 pythfinder-0.0.3.7/pythfinder/Components/BetterClasses/
+-rw-rw-rw-   0        0        0      102 2024-05-14 05:32:56.000000 pythfinder-0.0.3.7/pythfinder/Components/BetterClasses/__init__.py
+-rw-rw-rw-   0        0        0     1168 2024-05-13 14:52:24.000000 pythfinder-0.0.3.7/pythfinder/Components/BetterClasses/booleanEx.py
+-rw-rw-rw-   0        0        0      627 2024-05-13 14:52:55.000000 pythfinder-0.0.3.7/pythfinder/Components/BetterClasses/edgeDetectorEx.py
+-rw-rw-rw-   0        0        0     1140 2024-05-13 15:07:55.000000 pythfinder-0.0.3.7/pythfinder/Components/BetterClasses/errorEx.py
+-rw-rw-rw-   0        0        0     4862 2024-05-13 14:45:33.000000 pythfinder-0.0.3.7/pythfinder/Components/BetterClasses/mathEx.py
+drwxrwxrwx   0        0        0        0 2024-05-15 04:30:36.173102 pythfinder-0.0.3.7/pythfinder/Components/Constants/
+-rw-rw-rw-   0        0        0       78 2024-05-14 05:33:11.000000 pythfinder-0.0.3.7/pythfinder/Components/Constants/__init__.py
+-rw-rw-rw-   0        0        0    20781 2024-05-14 18:06:58.000000 pythfinder-0.0.3.7/pythfinder/Components/Constants/constants.py
+-rw-rw-rw-   0        0        0     2905 2024-05-13 15:08:14.000000 pythfinder-0.0.3.7/pythfinder/Components/Constants/constrains.py
+-rw-rw-rw-   0        0        0     2705 2024-05-13 15:11:03.000000 pythfinder-0.0.3.7/pythfinder/Components/Constants/screenSize.py
+drwxrwxrwx   0        0        0        0 2024-05-15 04:30:36.204351 pythfinder-0.0.3.7/pythfinder/Components/Controllers/
+-rw-rw-rw-   0        0        0      642 2024-05-13 15:12:44.000000 pythfinder-0.0.3.7/pythfinder/Components/Controllers/PIDCoefficients.py
+-rw-rw-rw-   0        0        0     1163 2024-05-14 16:07:14.000000 pythfinder-0.0.3.7/pythfinder/Components/Controllers/PIDController.py
+-rw-rw-rw-   0        0        0       60 2024-05-14 05:33:22.000000 pythfinder-0.0.3.7/pythfinder/Components/Controllers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 04:30:36.226498 pythfinder-0.0.3.7/pythfinder/Components/Menu/
+-rw-rw-rw-   0        0        0       87 2024-05-14 05:33:37.000000 pythfinder-0.0.3.7/pythfinder/Components/Menu/__init__.py
+-rw-rw-rw-   0        0        0    22248 2024-05-14 16:06:43.000000 pythfinder-0.0.3.7/pythfinder/Components/Menu/buttons.py
+-rw-rw-rw-   0        0        0     1583 2024-05-13 16:09:13.000000 pythfinder-0.0.3.7/pythfinder/Components/Menu/enums.py
+-rw-rw-rw-   0        0        0    22448 2024-05-14 16:06:48.000000 pythfinder-0.0.3.7/pythfinder/Components/Menu/main.py
+-rw-rw-rw-   0        0        0     4103 2024-05-14 16:07:01.000000 pythfinder-0.0.3.7/pythfinder/Components/Menu/menus.py
+-rw-rw-rw-   0        0        0      244 2024-05-14 05:35:39.000000 pythfinder-0.0.3.7/pythfinder/Components/__init__.py
+-rw-rw-rw-   0        0        0     5720 2024-05-14 16:04:43.000000 pythfinder-0.0.3.7/pythfinder/Components/background.py
+-rw-rw-rw-   0        0        0     9569 2024-05-14 16:05:08.000000 pythfinder-0.0.3.7/pythfinder/Components/controls.py
+-rw-rw-rw-   0        0        0     1853 2024-05-14 16:05:12.000000 pythfinder-0.0.3.7/pythfinder/Components/fade.py
+-rw-rw-rw-   0        0        0     9861 2024-05-14 15:58:30.000000 pythfinder-0.0.3.7/pythfinder/Components/robot.py
+-rw-rw-rw-   0        0        0     1975 2024-05-14 16:05:20.000000 pythfinder-0.0.3.7/pythfinder/Components/table.py
+-rw-rw-rw-   0        0        0     4633 2024-05-14 16:05:37.000000 pythfinder-0.0.3.7/pythfinder/Components/trail.py
+drwxrwxrwx   0        0        0        0 2024-05-15 04:30:36.242118 pythfinder-0.0.3.7/pythfinder/Images/
+drwxrwxrwx   0        0        0        0 2024-05-15 04:30:36.288998 pythfinder-0.0.3.7/pythfinder/Images/Controls/
+-rw-rw-rw-   0        0        0        0 2024-05-14 18:17:56.000000 pythfinder-0.0.3.7/pythfinder/Images/Controls/__init__.py
+-rw-rw-rw-   0        0        0   525562 2024-03-31 07:01:14.000000 pythfinder-0.0.3.7/pythfinder/Images/Controls/btn_backwards.png
+-rw-rw-rw-   0        0        0   530916 2024-03-31 07:01:10.000000 pythfinder-0.0.3.7/pythfinder/Images/Controls/btn_forwards.png
+-rw-rw-rw-   0        0        0   533042 2024-03-31 07:01:19.000000 pythfinder-0.0.3.7/pythfinder/Images/Controls/btn_hide_trail.png
+-rw-rw-rw-   0        0        0   561920 2024-03-31 14:58:53.000000 pythfinder-0.0.3.7/pythfinder/Images/Controls/btn_selecting_off.png
+-rw-rw-rw-   0        0        0   558616 2024-03-31 14:58:49.000000 pythfinder-0.0.3.7/pythfinder/Images/Controls/btn_selecting_on.png
+-rw-rw-rw-   0        0        0   531856 2024-03-31 07:00:59.000000 pythfinder-0.0.3.7/pythfinder/Images/Controls/btn_show_trail.png
+drwxrwxrwx   0        0        0        0 2024-05-15 04:30:36.304628 pythfinder-0.0.3.7/pythfinder/Images/Menu/
+drwxrwxrwx   0        0        0        0 2024-05-15 04:30:36.311143 pythfinder-0.0.3.7/pythfinder/Images/Menu/General/
+drwxrwxrwx   0        0        0        0 2024-05-15 04:30:35.956873 pythfinder-0.0.3.7/pythfinder/Images/Menu/General/Arrows/
+drwxrwxrwx   0        0        0        0 2024-05-15 04:30:36.311143 pythfinder-0.0.3.7/pythfinder/Images/Menu/General/Arrows/Left/
+-rw-rw-rw-   0        0        0     5149 2024-04-07 08:30:53.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/General/Arrows/Left/left_arrow.png
+-rw-rw-rw-   0        0        0     5334 2024-04-07 08:30:48.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/General/Arrows/Left/selected_left_arrow.png
+drwxrwxrwx   0        0        0        0 2024-05-15 04:30:36.326777 pythfinder-0.0.3.7/pythfinder/Images/Menu/General/Arrows/Right/
+-rw-rw-rw-   0        0        0     5181 2024-04-07 08:31:22.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/General/Arrows/Right/right_arrow.png
+-rw-rw-rw-   0        0        0     5279 2024-04-07 08:31:21.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/General/Arrows/Right/selected_right_arrow.png
+-rw-rw-rw-   0        0        0        0 2024-05-14 18:18:26.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/General/__init__.py
+-rw-rw-rw-   0        0        0   467492 2024-04-07 08:30:13.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/General/general_menu.png
+drwxrwxrwx   0        0        0        0 2024-05-15 04:30:36.373661 pythfinder-0.0.3.7/pythfinder/Images/Menu/Main/
+-rw-rw-rw-   0        0        0     8011 2024-04-05 16:14:53.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Main/menu_button.png
+-rw-rw-rw-   0        0        0     6208 2024-04-05 16:14:57.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Main/menu_home_button.png
+-rw-rw-rw-   0        0        0  1606752 2024-04-05 16:15:02.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Main/menu_main.png
+-rw-rw-rw-   0        0        0     8399 2024-04-06 11:39:50.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Main/selected_menu_button.png
+-rw-rw-rw-   0        0        0     6451 2024-04-06 11:39:46.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Main/selected_menu_home_button.png
+drwxrwxrwx   0        0        0        0 2024-05-15 04:30:36.373661 pythfinder-0.0.3.7/pythfinder/Images/Menu/Other/
+drwxrwxrwx   0        0        0        0 2024-05-15 04:30:36.411414 pythfinder-0.0.3.7/pythfinder/Images/Menu/Other/FieldCentric/
+-rw-rw-rw-   0        0        0    33821 2024-04-07 08:27:04.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Other/FieldCentric/field_centric_off.png
+-rw-rw-rw-   0        0        0    34053 2024-04-07 08:27:04.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Other/FieldCentric/field_centric_on.png
+-rw-rw-rw-   0        0        0    35325 2024-04-07 08:27:04.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Other/FieldCentric/selected_field_centric_off.png
+-rw-rw-rw-   0        0        0    35522 2024-04-07 08:27:04.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Other/FieldCentric/selected_field_centric_on.png
+drwxrwxrwx   0        0        0        0 2024-05-15 04:30:36.427048 pythfinder-0.0.3.7/pythfinder/Images/Menu/Other/RobotBorder/
+-rw-rw-rw-   0        0        0    32516 2024-04-07 08:27:48.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Other/RobotBorder/robot_border_off.png
+-rw-rw-rw-   0        0        0    32757 2024-04-07 08:27:49.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Other/RobotBorder/robot_border_on.png
+-rw-rw-rw-   0        0        0    33964 2024-04-07 08:27:48.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Other/RobotBorder/selected_robot_border_off.png
+-rw-rw-rw-   0        0        0    34153 2024-04-07 08:27:48.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Other/RobotBorder/selected_robot_border_on.png
+drwxrwxrwx   0        0        0        0 2024-05-15 04:30:36.442676 pythfinder-0.0.3.7/pythfinder/Images/Menu/Other/ScreenBorder/
+-rw-rw-rw-   0        0        0    34863 2024-04-07 08:28:53.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Other/ScreenBorder/screen_border_off.png
+-rw-rw-rw-   0        0        0    35031 2024-04-07 08:28:53.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Other/ScreenBorder/screen_border_on.png
+-rw-rw-rw-   0        0        0    36547 2024-04-07 08:28:53.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Other/ScreenBorder/selected_screen_border_off.png
+-rw-rw-rw-   0        0        0    36670 2024-04-07 08:28:53.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Other/ScreenBorder/selected_screen_border_on.png
+-rw-rw-rw-   0        0        0    20270 2024-04-09 17:13:50.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Other/other_indicator.png
+-rw-rw-rw-   0        0        0    13339 2024-04-07 08:29:32.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Other/other_quadrant.png
+drwxrwxrwx   0        0        0        0 2024-05-15 04:30:36.511706 pythfinder-0.0.3.7/pythfinder/Images/Menu/Robot/
+-rw-rw-rw-   0        0        0    28975 2024-04-08 04:32:03.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Robot/height.png
+-rw-rw-rw-   0        0        0    20193 2024-04-08 04:32:07.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Robot/robot_indicator.png
+-rw-rw-rw-   0        0        0    39077 2024-04-08 04:32:04.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Robot/robot_path.png
+-rw-rw-rw-   0        0        0   138988 2024-04-08 04:32:10.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Robot/robot_path_quadrant.png
+-rw-rw-rw-   0        0        0   115045 2024-04-08 04:32:12.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Robot/robot_specs_quadrant.png
+-rw-rw-rw-   0        0        0    20716 2024-04-08 04:32:17.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Robot/scale.png
+-rw-rw-rw-   0        0        0    30701 2024-04-08 04:32:20.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Robot/selected_height.png
+-rw-rw-rw-   0        0        0    40956 2024-04-08 04:32:22.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Robot/selected_robot_path.png
+-rw-rw-rw-   0        0        0    21855 2024-04-08 04:32:24.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Robot/selected_scale.png
+-rw-rw-rw-   0        0        0    21917 2024-04-08 04:32:27.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Robot/selected_width.png
+-rw-rw-rw-   0        0        0    20843 2024-04-08 04:32:30.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Robot/width.png
+drwxrwxrwx   0        0        0        0 2024-05-15 04:30:36.589847 pythfinder-0.0.3.7/pythfinder/Images/Menu/Selection/
+-rw-rw-rw-   0        0        0    19651 2024-04-06 15:09:11.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Selection/interface_button.png
+-rw-rw-rw-   0        0        0    14899 2024-04-06 15:09:15.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Selection/other_button.png
+-rw-rw-rw-   0        0        0    20750 2024-04-06 15:09:19.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Selection/pathing_button.png
+-rw-rw-rw-   0        0        0    13645 2024-04-06 15:09:23.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Selection/robot_button.png
+-rw-rw-rw-   0        0        0    16954 2024-04-06 15:09:26.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Selection/selected_interface_button.png
+-rw-rw-rw-   0        0        0    13205 2024-04-06 15:09:28.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Selection/selected_other_button.png
+-rw-rw-rw-   0        0        0    17797 2024-04-06 15:09:31.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Selection/selected_pathing_button.png
+-rw-rw-rw-   0        0        0    12126 2024-04-06 15:09:33.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Selection/selected_robot_button.png
+-rw-rw-rw-   0        0        0    11787 2024-04-06 15:09:36.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Selection/selected_trail_button.png
+-rw-rw-rw-   0        0        0    79511 2024-04-06 15:09:38.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Selection/selection_menu.png
+-rw-rw-rw-   0        0        0    13448 2024-04-06 15:09:41.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/Selection/trail_button.png
+-rw-rw-rw-   0        0        0        0 2024-05-14 18:18:10.000000 pythfinder-0.0.3.7/pythfinder/Images/Menu/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 04:30:36.611993 pythfinder-0.0.3.7/pythfinder/Images/Robot/
+-rw-rw-rw-   0        0        0        0 2024-05-14 18:18:58.000000 pythfinder-0.0.3.7/pythfinder/Images/Robot/__init__.py
+-rw-rw-rw-   0        0        0   600926 2024-03-18 18:10:12.000000 pythfinder-0.0.3.7/pythfinder/Images/Robot/bot_from_above.png
+drwxrwxrwx   0        0        0        0 2024-05-15 04:30:36.643255 pythfinder-0.0.3.7/pythfinder/Images/Table/
+-rw-rw-rw-   0        0        0  1025907 2024-04-29 12:07:29.000000 pythfinder-0.0.3.7/pythfinder/Images/Table/FLL_table_MP.jpg
+-rw-rw-rw-   0        0        0        0 2024-05-14 18:19:06.000000 pythfinder-0.0.3.7/pythfinder/Images/Table/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-14 18:17:47.000000 pythfinder-0.0.3.7/pythfinder/Images/__init__.py
+-rw-rw-rw-   0        0        0    16718 2024-04-07 11:58:49.000000 pythfinder-0.0.3.7/pythfinder/Images/none.png
+-rw-rw-rw-   0        0        0    17665 2024-04-07 11:58:46.000000 pythfinder-0.0.3.7/pythfinder/Images/selected_none.png
+drwxrwxrwx   0        0        0        0 2024-05-15 04:30:36.674509 pythfinder-0.0.3.7/pythfinder/Trajectory/
+-rw-rw-rw-   0        0        0      126 2024-05-14 05:34:50.000000 pythfinder-0.0.3.7/pythfinder/Trajectory/__init__.py
+-rw-rw-rw-   0        0        0    52721 2024-05-14 16:09:04.000000 pythfinder-0.0.3.7/pythfinder/Trajectory/builder.py
+-rw-rw-rw-   0        0        0     1709 2024-05-14 16:06:07.000000 pythfinder-0.0.3.7/pythfinder/Trajectory/feedback.py
+-rw-rw-rw-   0        0        0     4366 2024-05-14 16:06:12.000000 pythfinder-0.0.3.7/pythfinder/Trajectory/feedforward.py
+-rw-rw-rw-   0        0        0     1564 2024-05-14 16:06:17.000000 pythfinder-0.0.3.7/pythfinder/Trajectory/kinematics.py
+-rw-rw-rw-   0        0        0     5914 2024-05-14 16:06:21.000000 pythfinder-0.0.3.7/pythfinder/Trajectory/splines.py
+-rw-rw-rw-   0        0        0       98 2024-05-14 05:35:53.000000 pythfinder-0.0.3.7/pythfinder/__init__.py
+-rw-rw-rw-   0        0        0    11119 2024-05-14 16:29:39.000000 pythfinder-0.0.3.7/pythfinder/core.py
+drwxrwxrwx   0        0        0        0 2024-05-15 04:33:46.486842 pythfinder-0.0.3.7/pythfinder.egg-info/
+-rw-rw-rw-   0        0        0      310 2024-05-15 04:33:46.000000 pythfinder-0.0.3.7/pythfinder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4635 2024-05-15 04:33:46.000000 pythfinder-0.0.3.7/pythfinder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 04:33:46.000000 pythfinder-0.0.3.7/pythfinder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-15 04:33:46.000000 pythfinder-0.0.3.7/pythfinder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 04:33:46.552957 pythfinder-0.0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0      539 2024-05-15 04:30:15.000000 pythfinder-0.0.3.7/setup.py
```

### Comparing `pythfinder-0.0.3.6/LICENSE.txt` & `pythfinder-0.0.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.6/pythfinder/Components/BetterClasses/booleanEx.py` & `pythfinder-0.0.3.7/pythfinder/Components/BetterClasses/booleanEx.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.6/pythfinder/Components/BetterClasses/edgeDetectorEx.py` & `pythfinder-0.0.3.7/pythfinder/Components/BetterClasses/edgeDetectorEx.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.6/pythfinder/Components/BetterClasses/errorEx.py` & `pythfinder-0.0.3.7/pythfinder/Components/BetterClasses/errorEx.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.6/pythfinder/Components/BetterClasses/mathEx.py` & `pythfinder-0.0.3.7/pythfinder/Components/BetterClasses/mathEx.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.6/pythfinder/Components/Constants/constants.py` & `pythfinder-0.0.3.7/pythfinder/Components/Constants/constants.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.6/pythfinder/Components/Constants/constrains.py` & `pythfinder-0.0.3.7/pythfinder/Components/Constants/constrains.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.6/pythfinder/Components/Constants/screenSize.py` & `pythfinder-0.0.3.7/pythfinder/Components/Constants/screenSize.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.6/pythfinder/Components/Controllers/PIDCoefficients.py` & `pythfinder-0.0.3.7/pythfinder/Components/Controllers/PIDCoefficients.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.6/pythfinder/Components/Controllers/PIDController.py` & `pythfinder-0.0.3.7/pythfinder/Components/Controllers/PIDController.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.6/pythfinder/Components/Menu/buttons.py` & `pythfinder-0.0.3.7/pythfinder/Components/Menu/buttons.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.6/pythfinder/Components/Menu/enums.py` & `pythfinder-0.0.3.7/pythfinder/Components/Menu/enums.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.6/pythfinder/Components/Menu/main.py` & `pythfinder-0.0.3.7/pythfinder/Components/Menu/main.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.6/pythfinder/Components/Menu/menus.py` & `pythfinder-0.0.3.7/pythfinder/Components/Menu/menus.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.6/pythfinder/Components/background.py` & `pythfinder-0.0.3.7/pythfinder/Components/background.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.6/pythfinder/Components/controls.py` & `pythfinder-0.0.3.7/pythfinder/Components/controls.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.6/pythfinder/Components/fade.py` & `pythfinder-0.0.3.7/pythfinder/Components/fade.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.6/pythfinder/Components/robot.py` & `pythfinder-0.0.3.7/pythfinder/Components/robot.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.6/pythfinder/Components/table.py` & `pythfinder-0.0.3.7/pythfinder/Components/table.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.6/pythfinder/Components/trail.py` & `pythfinder-0.0.3.7/pythfinder/Components/trail.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.6/pythfinder/Trajectory/builder.py` & `pythfinder-0.0.3.7/pythfinder/Trajectory/builder.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.6/pythfinder/Trajectory/feedback.py` & `pythfinder-0.0.3.7/pythfinder/Trajectory/feedback.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.6/pythfinder/Trajectory/feedforward.py` & `pythfinder-0.0.3.7/pythfinder/Trajectory/feedforward.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.6/pythfinder/Trajectory/kinematics.py` & `pythfinder-0.0.3.7/pythfinder/Trajectory/kinematics.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.6/pythfinder/Trajectory/splines.py` & `pythfinder-0.0.3.7/pythfinder/Trajectory/splines.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.6/pythfinder/core.py` & `pythfinder-0.0.3.7/pythfinder/core.py`

 * *Files identical despite different names*

