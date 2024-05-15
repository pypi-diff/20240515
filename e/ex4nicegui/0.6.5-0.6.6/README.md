# Comparing `tmp/ex4nicegui-0.6.5.tar.gz` & `tmp/ex4nicegui-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ex4nicegui-0.6.5.tar", last modified: Sat Apr 27 11:46:49 2024, max compression
+gzip compressed data, was "ex4nicegui-0.6.6.tar", last modified: Wed May 15 16:42:52 2024, max compression
```

## Comparing `ex4nicegui-0.6.5.tar` & `ex4nicegui-0.6.6.tar`

### file list

```diff
@@ -1,179 +1,183 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.941689 ex4nicegui-0.6.5/
--rw-rw-rw-   0        0        0     1094 2023-06-30 08:17:10.000000 ex4nicegui-0.6.5/LICENSE
--rw-rw-rw-   0        0        0    27491 2024-04-27 11:46:49.941689 ex4nicegui-0.6.5/PKG-INFO
--rw-rw-rw-   0        0        0    25989 2024-03-05 13:06:09.000000 ex4nicegui-0.6.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.088757 ex4nicegui-0.6.5/ex4nicegui/
--rw-rw-rw-   0        0        0      818 2024-04-27 11:46:30.000000 ex4nicegui-0.6.5/ex4nicegui/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.123763 ex4nicegui-0.6.5/ex4nicegui/bi/
--rw-rw-rw-   0        0        0      315 2023-10-18 15:44:54.000000 ex4nicegui-0.6.5/ex4nicegui/bi/__init__.py
--rw-rw-rw-   0        0        0     7644 2024-04-26 16:54:25.000000 ex4nicegui-0.6.5/ex4nicegui/bi/dataSource.py
--rw-rw-rw-   0        0        0     8186 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/bi/dataSourceFacade.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.179173 ex4nicegui-0.6.5/ex4nicegui/bi/elements/
--rw-rw-rw-   0        0        0        0 2023-10-18 15:44:54.000000 ex4nicegui-0.6.5/ex4nicegui/bi/elements/__init__.py
--rw-rw-rw-   0        0        0      358 2023-10-18 15:44:54.000000 ex4nicegui-0.6.5/ex4nicegui/bi/elements/containers.py
--rw-rw-rw-   0        0        0      898 2023-10-18 15:44:54.000000 ex4nicegui-0.6.5/ex4nicegui/bi/elements/layouts.py
--rw-rw-rw-   0        0        0     1534 2023-12-04 18:30:56.000000 ex4nicegui-0.6.5/ex4nicegui/bi/elements/models.py
--rw-rw-rw-   0        0        0      808 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/bi/elements/text.py
--rw-rw-rw-   0        0        0     2009 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/bi/elements/ui_aggrid.py
--rw-rw-rw-   0        0        0      852 2023-10-18 15:44:54.000000 ex4nicegui-0.6.5/ex4nicegui/bi/elements/ui_date_picker.js
--rw-rw-rw-   0        0        0     2260 2023-12-06 09:33:56.000000 ex4nicegui-0.6.5/ex4nicegui/bi/elements/ui_date_picker.py
--rw-rw-rw-   0        0        0     2302 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/bi/elements/ui_echarts.py
--rw-rw-rw-   0        0        0     5447 2023-12-06 09:33:56.000000 ex4nicegui-0.6.5/ex4nicegui/bi/elements/ui_radio.py
--rw-rw-rw-   0        0        0     4128 2023-12-06 09:33:56.000000 ex4nicegui-0.6.5/ex4nicegui/bi/elements/ui_range.py
--rw-rw-rw-   0        0        0     3872 2023-12-08 12:43:57.000000 ex4nicegui-0.6.5/ex4nicegui/bi/elements/ui_select.py
--rw-rw-rw-   0        0        0     2165 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/bi/elements/ui_slider.py
--rw-rw-rw-   0        0        0     1810 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/bi/elements/ui_table.py
--rw-rw-rw-   0        0        0     2067 2024-01-07 17:28:53.000000 ex4nicegui-0.6.5/ex4nicegui/bi/index.py
--rw-rw-rw-   0        0        0     4529 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/bi/protocols.py
--rw-rw-rw-   0        0        0      355 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/bi/types.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.182931 ex4nicegui-0.6.5/ex4nicegui/experimental_/
--rw-rw-rw-   0        0        0       69 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/experimental_/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.201132 ex4nicegui-0.6.5/ex4nicegui/experimental_/gridLayout/
--rw-rw-rw-   0        0        0      125 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/experimental_/gridLayout/__init__.py
--rw-rw-rw-   0        0        0     4737 2023-10-18 15:44:54.000000 ex4nicegui-0.6.5/ex4nicegui/experimental_/gridLayout/index.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.226755 ex4nicegui-0.6.5/ex4nicegui/gsap/
--rw-rw-rw-   0        0        0      218 2024-02-27 20:13:02.000000 ex4nicegui-0.6.5/ex4nicegui/gsap/__init__.py
--rw-rw-rw-   0        0        0     4638 2024-04-26 16:54:25.000000 ex4nicegui-0.6.5/ex4nicegui/gsap/gsap.py
--rw-rw-rw-   0        0        0     1241 2024-02-27 20:13:02.000000 ex4nicegui-0.6.5/ex4nicegui/gsap/timeline.js
--rw-rw-rw-   0        0        0     2390 2024-04-26 16:54:25.000000 ex4nicegui-0.6.5/ex4nicegui/gsap/timeline.py
--rw-rw-rw-   0        0        0     1045 2024-02-02 15:27:35.000000 ex4nicegui-0.6.5/ex4nicegui/gsap/wrapGsap.js
-drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.288398 ex4nicegui-0.6.5/ex4nicegui/layout/
--rw-rw-rw-   0        0        0      278 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/layout/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.305360 ex4nicegui-0.6.5/ex4nicegui/layout/gridFlex/
--rw-rw-rw-   0        0        0     4468 2023-10-18 15:44:54.000000 ex4nicegui-0.6.5/ex4nicegui/layout/gridFlex/GridFlex.js
--rw-rw-rw-   0        0        0        2 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/layout/gridFlex/__init__.py
--rw-rw-rw-   0        0        0     7194 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/layout/gridFlex/gridFlex.py
--rw-rw-rw-   0        0        0     1236 2023-10-18 15:44:54.000000 ex4nicegui-0.6.5/ex4nicegui/layout/gridFlex/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.309360 ex4nicegui-0.6.5/ex4nicegui/layout/rxFlex/
--rw-rw-rw-   0        0        0        0 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/layout/rxFlex/__init__.py
--rw-rw-rw-   0        0        0     3672 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/layout/rxFlex/index.py
--rw-rw-rw-   0        0        0     1411 2023-10-18 15:44:54.000000 ex4nicegui-0.6.5/ex4nicegui/layout/rxFlex/types.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.309360 ex4nicegui-0.6.5/ex4nicegui/libs/
--rw-rw-rw-   0        0        0        0 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.464670 ex4nicegui-0.6.5/ex4nicegui/libs/d3/
--rw-rw-rw-   0        0        0        0 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/d3/__init__.py
--rw-rw-rw-   0        0        0    12795 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/d3/d3-color.ems.js
--rw-rw-rw-   0        0        0     2148 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/d3/d3-dispatch.ems.js
--rw-rw-rw-   0        0        0     4822 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/d3/d3-drag.ems.js
--rw-rw-rw-   0        0        0     3883 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/d3/d3-ease.ems.js
--rw-rw-rw-   0        0        0     9903 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/d3/d3-interpolate.ems.js
--rw-rw-rw-   0        0        0    16007 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/d3/d3-selection.ems.js
--rw-rw-rw-   0        0        0     2320 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/d3/d3-timer.ems.js
--rw-rw-rw-   0        0        0    14024 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/d3/d3-transition.ems.js
--rw-rw-rw-   0        0        0    11599 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/d3/d3-zoom.ems.js
-drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.668386 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/
--rw-rw-rw-   0        0        0    64907 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/CSSPlugin.js
--rw-rw-rw-   0        0        0     3674 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/CSSRulePlugin.js
--rw-rw-rw-   0        0        0    11588 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/CustomEase.js
--rw-rw-rw-   0        0        0   103102 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/Draggable.js
--rw-rw-rw-   0        0        0     5530 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/EasePack.js
--rw-rw-rw-   0        0        0     9125 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/EaselPlugin.js
--rw-rw-rw-   0        0        0    48981 2024-03-07 20:18:40.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/Flip.js
--rw-rw-rw-   0        0        0    12852 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/MotionPathPlugin.js
--rw-rw-rw-   0        0        0    26112 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/Observer.js
--rw-rw-rw-   0        0        0    15404 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/PixiPlugin.js
--rw-rw-rw-   0        0        0     9217 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/ScrollToPlugin.js
--rw-rw-rw-   0        0        0   112584 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/ScrollTrigger.js
--rw-rw-rw-   0        0        0     4877 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/TextPlugin.js
--rw-rw-rw-   0        0        0        0 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/__init__.py
--rw-rw-rw-   0        0        0     1585 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/all.js
--rw-rw-rw-   0        0        0   175009 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/gsap-core.js
-drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.709381 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/utils/
--rw-rw-rw-   0        0        0        0 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/utils/__init__.py
--rw-rw-rw-   0        0        0    15235 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/utils/matrix.js
--rw-rw-rw-   0        0        0    49314 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/utils/paths.js
--rw-rw-rw-   0        0        0    10472 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/utils/strings.js
-drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.755703 ex4nicegui-0.6.5/ex4nicegui/reactive/
-drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.762172 ex4nicegui-0.6.5/ex4nicegui/reactive/EChartsComponent/
--rw-rw-rw-   0        0        0     3326 2024-04-23 06:45:41.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/EChartsComponent/ECharts.js
--rw-rw-rw-   0        0        0     6313 2024-04-26 16:54:25.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/EChartsComponent/ECharts.py
--rw-rw-rw-   0        0        0        0 2023-07-31 07:50:52.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/EChartsComponent/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.791785 ex4nicegui-0.6.5/ex4nicegui/reactive/UseDraggable/
--rw-rw-rw-   0        0        0     5473 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/UseDraggable/UseDraggable.js
--rw-rw-rw-   0        0        0     3929 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/UseDraggable/UseDraggable.py
--rw-rw-rw-   0        0        0        0 2023-07-17 16:36:22.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/UseDraggable/__init__.py
--rw-rw-rw-   0        0        0     3714 2024-03-25 14:45:22.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.807772 ex4nicegui-0.6.5/ex4nicegui/reactive/dropZone/
--rw-rw-rw-   0        0        0        0 2023-07-31 07:45:08.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/dropZone/__init__.py
--rw-rw-rw-   0        0        0     2713 2023-07-29 10:16:25.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/dropZone/dropZone.js
--rw-rw-rw-   0        0        0     2590 2023-10-18 15:44:54.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/dropZone/dropZone.py
--rw-rw-rw-   0        0        0       50 2024-03-21 14:24:33.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/empty.js
--rw-rw-rw-   0        0        0      132 2024-03-21 14:24:33.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/empty.py
--rw-rw-rw-   0        0        0     1472 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/fileWatcher.py
--rw-rw-rw-   0        0        0     6225 2024-03-05 13:06:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/local_file_picker.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.824726 ex4nicegui-0.6.5/ex4nicegui/reactive/mermaid/
--rw-rw-rw-   0        0        0        0 2023-10-23 17:41:12.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/mermaid/__init__.py
--rw-rw-rw-   0        0        0     2308 2023-10-29 08:33:17.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/mermaid/mermaid.js
--rw-rw-rw-   0        0        0     2144 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/mermaid/mermaid.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.901962 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/
--rw-rw-rw-   0        0        0        2 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/__init__.py
--rw-rw-rw-   0        0        0     2929 2024-03-07 20:18:40.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/aggrid.py
--rw-rw-rw-   0        0        0    10440 2024-03-21 14:24:33.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/base.py
--rw-rw-rw-   0        0        0     1660 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/button.py
--rw-rw-rw-   0        0        0     1275 2023-07-21 14:29:40.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/card.py
--rw-rw-rw-   0        0        0     1562 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/checkbox.py
--rw-rw-rw-   0        0        0     1787 2024-02-29 13:12:44.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/circular_progress.py
--rw-rw-rw-   0        0        0     3402 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/color_picker.py
--rw-rw-rw-   0        0        0     1040 2024-02-29 12:25:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/column.py
--rw-rw-rw-   0        0        0     2681 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/date.py
--rw-rw-rw-   0        0        0     2370 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/drawer.py
--rw-rw-rw-   0        0        0     9696 2024-03-21 14:24:33.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/echarts.py
--rw-rw-rw-   0        0        0      412 2024-03-21 14:24:33.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/element.py
--rw-rw-rw-   0        0        0     1873 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/expansion.py
--rw-rw-rw-   0        0        0      865 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/grid.py
--rw-rw-rw-   0        0        0      119 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/html.js
--rw-rw-rw-   0        0        0      675 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/html.py
--rw-rw-rw-   0        0        0     1559 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/icon.py
--rw-rw-rw-   0        0        0     1120 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/image.py
--rw-rw-rw-   0        0        0     4030 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/input.py
--rw-rw-rw-   0        0        0     2153 2024-02-29 11:46:48.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/knob.py
--rw-rw-rw-   0        0        0     1398 2024-03-04 19:14:43.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/label.py
--rw-rw-rw-   0        0        0     2128 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/linear_progress.py
--rw-rw-rw-   0        0        0     2201 2024-02-29 13:12:44.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/number.py
--rw-rw-rw-   0        0        0     1929 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/radio.py
--rw-rw-rw-   0        0        0     1029 2024-02-29 12:25:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/row.py
--rw-rw-rw-   0        0        0     2980 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/select.py
--rw-rw-rw-   0        0        0     2954 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/slider.py
--rw-rw-rw-   0        0        0     1605 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/switch.py
--rw-rw-rw-   0        0        0     1796 2024-03-21 14:24:33.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/tab.py
--rw-rw-rw-   0        0        0      630 2024-03-21 14:24:33.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/tab_panel.py
--rw-rw-rw-   0        0        0     1375 2024-03-21 14:24:33.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/tab_panels.py
--rw-rw-rw-   0        0        0     6042 2024-03-21 14:24:33.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/table.py
--rw-rw-rw-   0        0        0     1232 2024-03-21 14:24:33.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/tabs.py
--rw-rw-rw-   0        0        0     3044 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/textarea.py
--rw-rw-rw-   0        0        0     2360 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/upload.py
--rw-rw-rw-   0        0        0      213 2024-02-21 13:27:29.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/utils.py
--rw-rw-rw-   0        0        0     1505 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/q_pagination.py
--rw-rw-rw-   0        0        0       31 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/rxui.py
--rw-rw-rw-   0        0        0      898 2024-03-21 14:24:33.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/transitionGroup.js
--rw-rw-rw-   0        0        0      597 2024-03-21 14:24:33.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/transitionGroup.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.918558 ex4nicegui-0.6.5/ex4nicegui/reactive/useMouse/
--rw-rw-rw-   0        0        0     2722 2023-07-17 15:14:14.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/useMouse/UseMouse.js
--rw-rw-rw-   0        0        0     2122 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/useMouse/UseMouse.py
--rw-rw-rw-   0        0        0        0 2023-07-08 17:55:18.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/useMouse/__init__.py
--rw-rw-rw-   0        0        0     2598 2024-03-07 10:39:11.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/usePagination.py
--rw-rw-rw-   0        0        0     4360 2024-03-07 20:18:40.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/utils.py
--rw-rw-rw-   0        0        0      282 2024-03-21 14:24:33.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/vfor.js
--rw-rw-rw-   0        0        0     5778 2024-04-26 16:54:25.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/vfor.py
--rw-rw-rw-   0        0        0     5091 2024-03-05 13:12:27.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/vmodel.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.922558 ex4nicegui-0.6.5/ex4nicegui/tools/
--rw-rw-rw-   0        0        0        0 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/tools/__init__.py
--rw-rw-rw-   0        0        0     4868 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/tools/debug.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.938831 ex4nicegui-0.6.5/ex4nicegui/utils/
--rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.6.5/ex4nicegui/utils/__init__.py
--rw-rw-rw-   0        0        0     2527 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/utils/apiEffect.py
--rw-rw-rw-   0        0        0     1505 2024-03-05 13:06:09.000000 ex4nicegui-0.6.5/ex4nicegui/utils/asyncComputed.py
--rw-rw-rw-   0        0        0     1267 2024-04-26 16:54:25.000000 ex4nicegui-0.6.5/ex4nicegui/utils/clientScope.py
--rw-rw-rw-   0        0        0      994 2024-02-20 10:06:17.000000 ex4nicegui-0.6.5/ex4nicegui/utils/common.py
--rw-rw-rw-   0        0        0     2310 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/utils/effect.py
--rw-rw-rw-   0        0        0     1218 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/utils/scheduler.py
--rw-rw-rw-   0        0        0    11346 2024-03-21 14:24:33.000000 ex4nicegui-0.6.5/ex4nicegui/utils/signals.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.106607 ex4nicegui-0.6.5/ex4nicegui.egg-info/
--rw-rw-rw-   0        0        0    27491 2024-04-27 11:46:48.000000 ex4nicegui-0.6.5/ex4nicegui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5460 2024-04-27 11:46:48.000000 ex4nicegui-0.6.5/ex4nicegui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 11:46:48.000000 ex4nicegui-0.6.5/ex4nicegui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-27 11:46:48.000000 ex4nicegui-0.6.5/ex4nicegui.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       58 2024-04-27 11:46:48.000000 ex4nicegui-0.6.5/ex4nicegui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-27 11:46:48.000000 ex4nicegui-0.6.5/ex4nicegui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-27 11:46:49.941689 ex4nicegui-0.6.5/setup.cfg
--rw-rw-rw-   0        0        0     1576 2024-04-26 16:54:25.000000 ex4nicegui-0.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:42:52.057506 ex4nicegui-0.6.6/
+-rw-rw-rw-   0        0        0     1094 2023-06-30 08:17:10.000000 ex4nicegui-0.6.6/LICENSE
+-rw-rw-rw-   0        0        0    28006 2024-05-15 16:42:52.057506 ex4nicegui-0.6.6/PKG-INFO
+-rw-rw-rw-   0        0        0    26470 2024-05-14 17:54:39.000000 ex4nicegui-0.6.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.213421 ex4nicegui-0.6.6/ex4nicegui/
+-rw-rw-rw-   0        0        0      886 2024-05-15 16:42:30.000000 ex4nicegui-0.6.6/ex4nicegui/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.235826 ex4nicegui-0.6.6/ex4nicegui/bi/
+-rw-rw-rw-   0        0        0      315 2023-10-18 15:44:54.000000 ex4nicegui-0.6.6/ex4nicegui/bi/__init__.py
+-rw-rw-rw-   0        0        0     7644 2024-04-26 16:54:25.000000 ex4nicegui-0.6.6/ex4nicegui/bi/dataSource.py
+-rw-rw-rw-   0        0        0     8186 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/bi/dataSourceFacade.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.289755 ex4nicegui-0.6.6/ex4nicegui/bi/elements/
+-rw-rw-rw-   0        0        0        0 2023-10-18 15:44:54.000000 ex4nicegui-0.6.6/ex4nicegui/bi/elements/__init__.py
+-rw-rw-rw-   0        0        0      358 2023-10-18 15:44:54.000000 ex4nicegui-0.6.6/ex4nicegui/bi/elements/containers.py
+-rw-rw-rw-   0        0        0      898 2023-10-18 15:44:54.000000 ex4nicegui-0.6.6/ex4nicegui/bi/elements/layouts.py
+-rw-rw-rw-   0        0        0     1534 2023-12-04 18:30:56.000000 ex4nicegui-0.6.6/ex4nicegui/bi/elements/models.py
+-rw-rw-rw-   0        0        0      808 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/bi/elements/text.py
+-rw-rw-rw-   0        0        0     2009 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/bi/elements/ui_aggrid.py
+-rw-rw-rw-   0        0        0      852 2023-10-18 15:44:54.000000 ex4nicegui-0.6.6/ex4nicegui/bi/elements/ui_date_picker.js
+-rw-rw-rw-   0        0        0     2260 2023-12-06 09:33:56.000000 ex4nicegui-0.6.6/ex4nicegui/bi/elements/ui_date_picker.py
+-rw-rw-rw-   0        0        0     2248 2024-05-15 16:41:01.000000 ex4nicegui-0.6.6/ex4nicegui/bi/elements/ui_echarts.py
+-rw-rw-rw-   0        0        0     5447 2023-12-06 09:33:56.000000 ex4nicegui-0.6.6/ex4nicegui/bi/elements/ui_radio.py
+-rw-rw-rw-   0        0        0     4128 2023-12-06 09:33:56.000000 ex4nicegui-0.6.6/ex4nicegui/bi/elements/ui_range.py
+-rw-rw-rw-   0        0        0     3872 2023-12-08 12:43:57.000000 ex4nicegui-0.6.6/ex4nicegui/bi/elements/ui_select.py
+-rw-rw-rw-   0        0        0     2165 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/bi/elements/ui_slider.py
+-rw-rw-rw-   0        0        0     1810 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/bi/elements/ui_table.py
+-rw-rw-rw-   0        0        0     2067 2024-01-07 17:28:53.000000 ex4nicegui-0.6.6/ex4nicegui/bi/index.py
+-rw-rw-rw-   0        0        0     4529 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/bi/protocols.py
+-rw-rw-rw-   0        0        0      355 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/bi/types.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.291984 ex4nicegui-0.6.6/ex4nicegui/experimental_/
+-rw-rw-rw-   0        0        0       69 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/experimental_/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.291984 ex4nicegui-0.6.6/ex4nicegui/experimental_/gridLayout/
+-rw-rw-rw-   0        0        0      125 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/experimental_/gridLayout/__init__.py
+-rw-rw-rw-   0        0        0     4737 2023-10-18 15:44:54.000000 ex4nicegui-0.6.6/ex4nicegui/experimental_/gridLayout/index.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.340497 ex4nicegui-0.6.6/ex4nicegui/gsap/
+-rw-rw-rw-   0        0        0      218 2024-02-27 20:13:02.000000 ex4nicegui-0.6.6/ex4nicegui/gsap/__init__.py
+-rw-rw-rw-   0        0        0     4638 2024-04-26 16:54:25.000000 ex4nicegui-0.6.6/ex4nicegui/gsap/gsap.py
+-rw-rw-rw-   0        0        0     1241 2024-02-27 20:13:02.000000 ex4nicegui-0.6.6/ex4nicegui/gsap/timeline.js
+-rw-rw-rw-   0        0        0     2390 2024-04-26 16:54:25.000000 ex4nicegui-0.6.6/ex4nicegui/gsap/timeline.py
+-rw-rw-rw-   0        0        0     1045 2024-02-02 15:27:35.000000 ex4nicegui-0.6.6/ex4nicegui/gsap/wrapGsap.js
+drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.350914 ex4nicegui-0.6.6/ex4nicegui/layout/
+-rw-rw-rw-   0        0        0      278 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/layout/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.367467 ex4nicegui-0.6.6/ex4nicegui/layout/gridFlex/
+-rw-rw-rw-   0        0        0     4468 2023-10-18 15:44:54.000000 ex4nicegui-0.6.6/ex4nicegui/layout/gridFlex/GridFlex.js
+-rw-rw-rw-   0        0        0        2 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/layout/gridFlex/__init__.py
+-rw-rw-rw-   0        0        0     7194 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/layout/gridFlex/gridFlex.py
+-rw-rw-rw-   0        0        0     1236 2023-10-18 15:44:54.000000 ex4nicegui-0.6.6/ex4nicegui/layout/gridFlex/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.373543 ex4nicegui-0.6.6/ex4nicegui/layout/rxFlex/
+-rw-rw-rw-   0        0        0        0 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/layout/rxFlex/__init__.py
+-rw-rw-rw-   0        0        0     3672 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/layout/rxFlex/index.py
+-rw-rw-rw-   0        0        0     1411 2023-10-18 15:44:54.000000 ex4nicegui-0.6.6/ex4nicegui/layout/rxFlex/types.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.375941 ex4nicegui-0.6.6/ex4nicegui/libs/
+-rw-rw-rw-   0        0        0        0 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.485988 ex4nicegui-0.6.6/ex4nicegui/libs/d3/
+-rw-rw-rw-   0        0        0        0 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/d3/__init__.py
+-rw-rw-rw-   0        0        0    12795 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/d3/d3-color.ems.js
+-rw-rw-rw-   0        0        0     2148 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/d3/d3-dispatch.ems.js
+-rw-rw-rw-   0        0        0     4822 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/d3/d3-drag.ems.js
+-rw-rw-rw-   0        0        0     3883 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/d3/d3-ease.ems.js
+-rw-rw-rw-   0        0        0     9903 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/d3/d3-interpolate.ems.js
+-rw-rw-rw-   0        0        0    16007 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/d3/d3-selection.ems.js
+-rw-rw-rw-   0        0        0     2320 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/d3/d3-timer.ems.js
+-rw-rw-rw-   0        0        0    14024 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/d3/d3-transition.ems.js
+-rw-rw-rw-   0        0        0    11599 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/d3/d3-zoom.ems.js
+drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.633712 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/
+-rw-rw-rw-   0        0        0    64907 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/CSSPlugin.js
+-rw-rw-rw-   0        0        0     3674 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/CSSRulePlugin.js
+-rw-rw-rw-   0        0        0    11588 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/CustomEase.js
+-rw-rw-rw-   0        0        0   103102 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/Draggable.js
+-rw-rw-rw-   0        0        0     5530 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/EasePack.js
+-rw-rw-rw-   0        0        0     9125 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/EaselPlugin.js
+-rw-rw-rw-   0        0        0    48981 2024-03-07 20:18:40.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/Flip.js
+-rw-rw-rw-   0        0        0    12852 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/MotionPathPlugin.js
+-rw-rw-rw-   0        0        0    26112 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/Observer.js
+-rw-rw-rw-   0        0        0    15404 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/PixiPlugin.js
+-rw-rw-rw-   0        0        0     9217 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/ScrollToPlugin.js
+-rw-rw-rw-   0        0        0   112584 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/ScrollTrigger.js
+-rw-rw-rw-   0        0        0     4877 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/TextPlugin.js
+-rw-rw-rw-   0        0        0        0 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/__init__.py
+-rw-rw-rw-   0        0        0     1585 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/all.js
+-rw-rw-rw-   0        0        0   175009 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/gsap-core.js
+drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.667907 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/utils/__init__.py
+-rw-rw-rw-   0        0        0    15235 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/utils/matrix.js
+-rw-rw-rw-   0        0        0    49314 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/utils/paths.js
+-rw-rw-rw-   0        0        0    10472 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/utils/strings.js
+drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.733449 ex4nicegui-0.6.6/ex4nicegui/reactive/
+drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.746480 ex4nicegui-0.6.6/ex4nicegui/reactive/EChartsComponent/
+-rw-rw-rw-   0        0        0     3164 2024-05-15 16:41:01.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/EChartsComponent/ECharts.js
+-rw-rw-rw-   0        0        0     4490 2024-05-15 16:41:01.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/EChartsComponent/ECharts.py
+-rw-rw-rw-   0        0        0        0 2023-07-31 07:50:52.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/EChartsComponent/__init__.py
+-rw-rw-rw-   0        0        0      570 2024-05-15 16:41:01.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/EChartsComponent/events.py
+-rw-rw-rw-   0        0        0     1001 2024-05-15 16:41:01.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/EChartsComponent/types.py
+-rw-rw-rw-   0        0        0     1463 2024-05-15 16:41:01.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/EChartsComponent/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.764733 ex4nicegui-0.6.6/ex4nicegui/reactive/UseDraggable/
+-rw-rw-rw-   0        0        0     5473 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/UseDraggable/UseDraggable.js
+-rw-rw-rw-   0        0        0     3929 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/UseDraggable/UseDraggable.py
+-rw-rw-rw-   0        0        0        0 2023-07-17 16:36:22.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/UseDraggable/__init__.py
+-rw-rw-rw-   0        0        0     3714 2024-03-25 14:45:22.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/__init__.py
+-rw-rw-rw-   0        0        0      824 2024-05-15 08:33:29.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/deferredTask.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.801508 ex4nicegui-0.6.6/ex4nicegui/reactive/dropZone/
+-rw-rw-rw-   0        0        0        0 2023-07-31 07:45:08.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/dropZone/__init__.py
+-rw-rw-rw-   0        0        0     2713 2023-07-29 10:16:25.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/dropZone/dropZone.js
+-rw-rw-rw-   0        0        0     2590 2023-10-18 15:44:54.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/dropZone/dropZone.py
+-rw-rw-rw-   0        0        0       50 2024-03-21 14:24:33.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/empty.js
+-rw-rw-rw-   0        0        0      132 2024-03-21 14:24:33.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/empty.py
+-rw-rw-rw-   0        0        0     1472 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/fileWatcher.py
+-rw-rw-rw-   0        0        0     6225 2024-03-05 13:06:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/local_file_picker.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.821293 ex4nicegui-0.6.6/ex4nicegui/reactive/mermaid/
+-rw-rw-rw-   0        0        0        0 2023-10-23 17:41:12.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/mermaid/__init__.py
+-rw-rw-rw-   0        0        0     2308 2023-10-29 08:33:17.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/mermaid/mermaid.js
+-rw-rw-rw-   0        0        0     2144 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/mermaid/mermaid.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:42:52.001860 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/
+-rw-rw-rw-   0        0        0        2 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/__init__.py
+-rw-rw-rw-   0        0        0     2929 2024-03-07 20:18:40.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/aggrid.py
+-rw-rw-rw-   0        0        0    10440 2024-03-21 14:24:33.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/base.py
+-rw-rw-rw-   0        0        0     1660 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/button.py
+-rw-rw-rw-   0        0        0     1275 2023-07-21 14:29:40.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/card.py
+-rw-rw-rw-   0        0        0     1562 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/checkbox.py
+-rw-rw-rw-   0        0        0     1787 2024-02-29 13:12:44.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/circular_progress.py
+-rw-rw-rw-   0        0        0     3402 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/color_picker.py
+-rw-rw-rw-   0        0        0     1040 2024-02-29 12:25:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/column.py
+-rw-rw-rw-   0        0        0     2681 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/date.py
+-rw-rw-rw-   0        0        0     2370 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/drawer.py
+-rw-rw-rw-   0        0        0     9495 2024-05-15 16:41:01.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/echarts.py
+-rw-rw-rw-   0        0        0      412 2024-03-21 14:24:33.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/element.py
+-rw-rw-rw-   0        0        0     1873 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/expansion.py
+-rw-rw-rw-   0        0        0      865 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/grid.py
+-rw-rw-rw-   0        0        0      119 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/html.js
+-rw-rw-rw-   0        0        0      675 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/html.py
+-rw-rw-rw-   0        0        0     1559 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/icon.py
+-rw-rw-rw-   0        0        0     1120 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/image.py
+-rw-rw-rw-   0        0        0     4030 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/input.py
+-rw-rw-rw-   0        0        0     2153 2024-02-29 11:46:48.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/knob.py
+-rw-rw-rw-   0        0        0     1398 2024-03-04 19:14:43.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/label.py
+-rw-rw-rw-   0        0        0     2128 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/linear_progress.py
+-rw-rw-rw-   0        0        0     2236 2024-05-14 19:43:06.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/number.py
+-rw-rw-rw-   0        0        0     1929 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/radio.py
+-rw-rw-rw-   0        0        0     1029 2024-02-29 12:25:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/row.py
+-rw-rw-rw-   0        0        0     2980 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/select.py
+-rw-rw-rw-   0        0        0     2954 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/slider.py
+-rw-rw-rw-   0        0        0     1605 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/switch.py
+-rw-rw-rw-   0        0        0     1796 2024-03-21 14:24:33.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/tab.py
+-rw-rw-rw-   0        0        0      630 2024-03-21 14:24:33.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/tab_panel.py
+-rw-rw-rw-   0        0        0     1375 2024-03-21 14:24:33.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/tab_panels.py
+-rw-rw-rw-   0        0        0     6042 2024-03-21 14:24:33.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/table.py
+-rw-rw-rw-   0        0        0     1232 2024-03-21 14:24:33.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/tabs.py
+-rw-rw-rw-   0        0        0     3044 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/textarea.py
+-rw-rw-rw-   0        0        0     2360 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/upload.py
+-rw-rw-rw-   0        0        0      213 2024-02-21 13:27:29.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/utils.py
+-rw-rw-rw-   0        0        0     1505 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/q_pagination.py
+-rw-rw-rw-   0        0        0       31 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/rxui.py
+-rw-rw-rw-   0        0        0      898 2024-03-21 14:24:33.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/transitionGroup.js
+-rw-rw-rw-   0        0        0      597 2024-03-21 14:24:33.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/transitionGroup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:42:52.025198 ex4nicegui-0.6.6/ex4nicegui/reactive/useMouse/
+-rw-rw-rw-   0        0        0     2722 2023-07-17 15:14:14.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/useMouse/UseMouse.js
+-rw-rw-rw-   0        0        0     2122 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/useMouse/UseMouse.py
+-rw-rw-rw-   0        0        0        0 2023-07-08 17:55:18.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/useMouse/__init__.py
+-rw-rw-rw-   0        0        0     2598 2024-03-07 10:39:11.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/usePagination.py
+-rw-rw-rw-   0        0        0     4360 2024-03-07 20:18:40.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/utils.py
+-rw-rw-rw-   0        0        0      282 2024-03-21 14:24:33.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/vfor.js
+-rw-rw-rw-   0        0        0     5778 2024-04-26 16:54:25.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/vfor.py
+-rw-rw-rw-   0        0        0     5091 2024-03-05 13:12:27.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/vmodel.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:42:52.028669 ex4nicegui-0.6.6/ex4nicegui/tools/
+-rw-rw-rw-   0        0        0        0 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/tools/__init__.py
+-rw-rw-rw-   0        0        0     4868 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/tools/debug.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:42:52.052490 ex4nicegui-0.6.6/ex4nicegui/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.6.6/ex4nicegui/utils/__init__.py
+-rw-rw-rw-   0        0        0     2527 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/utils/apiEffect.py
+-rw-rw-rw-   0        0        0     1505 2024-03-05 13:06:09.000000 ex4nicegui-0.6.6/ex4nicegui/utils/asyncComputed.py
+-rw-rw-rw-   0        0        0     1719 2024-05-14 17:54:39.000000 ex4nicegui-0.6.6/ex4nicegui/utils/clientScope.py
+-rw-rw-rw-   0        0        0      994 2024-02-20 10:06:17.000000 ex4nicegui-0.6.6/ex4nicegui/utils/common.py
+-rw-rw-rw-   0        0        0     2310 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/utils/effect.py
+-rw-rw-rw-   0        0        0     1218 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/utils/scheduler.py
+-rw-rw-rw-   0        0        0    11346 2024-05-14 18:10:44.000000 ex4nicegui-0.6.6/ex4nicegui/utils/signals.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.224370 ex4nicegui-0.6.6/ex4nicegui.egg-info/
+-rw-rw-rw-   0        0        0    28006 2024-05-15 16:42:50.000000 ex4nicegui-0.6.6/ex4nicegui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5635 2024-05-15 16:42:50.000000 ex4nicegui-0.6.6/ex4nicegui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 16:42:50.000000 ex4nicegui-0.6.6/ex4nicegui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-15 16:42:50.000000 ex4nicegui-0.6.6/ex4nicegui.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       58 2024-05-15 16:42:50.000000 ex4nicegui-0.6.6/ex4nicegui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-15 16:42:50.000000 ex4nicegui-0.6.6/ex4nicegui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 16:42:52.057506 ex4nicegui-0.6.6/setup.cfg
+-rw-rw-rw-   0        0        0     1576 2024-04-26 16:54:25.000000 ex4nicegui-0.6.6/setup.py
```

### Comparing `ex4nicegui-0.6.5/LICENSE` & `ex4nicegui-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/PKG-INFO` & `ex4nicegui-0.6.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ex4nicegui
-Version: 0.6.5
+Version: 0.6.6
 Summary: Extension library based on nicegui, providing data responsive,BI functionality modules
 Home-page: 
 Author: carson_jia
 Author-email: 568166495@qq.com
 License: MIT license
 Keywords: nicegui,ex4nicegui,webui
 Classifier: Intended Audience :: Developers
@@ -416,14 +416,39 @@
 
 - If the parameter `onchanges` is True (the default value is False), the specified function will not be executed at binding time.
 
 > Never spread a lot of data processing logic across multiple `on`s or `effects`s, which should be mostly interface manipulation logic rather than responsive data processing logic
 
 ---
 
+### `new_scope`
+
+By default, all watch functions are automatically destroyed when the client connection is disconnected. For finer-grained control, the `new_scope` function can be utilized.
+
+```python
+from nicegui import ui
+from ex4nicegui import rxui, to_ref, effect, new_scope
+
+a = to_ref(0.0)
+
+scope1 = new_scope()
+
+@scope1.run
+def _():
+    @effect
+    def _():
+        print(f"scope 1:{a.value}")
+
+
+rxui.number(value=a)
+rxui.button("dispose scope 1", on_click=scope1.dispose)
+```
+
+---
+
 ## functionality
 
 ### vmodel
 Create two-way bindings on form input elements or components.
 
 Bidirectional bindings are supported by default for `ref` simple value types
 ```python
```

### Comparing `ex4nicegui-0.6.5/README.md` & `ex4nicegui-0.6.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -410,14 +410,39 @@
 - 参数 `onchanges` 为 True 时(默认值为 False),指定的函数不会在绑定时执行 
 
 
 > 切忌把大量数据处理逻辑分散在多个 `on` 或 `effect` 中，`on` 或 `effect` 中应该大部分为界面操作逻辑，而非响应式数据处理逻辑
 
 ---
 
+### `new_scope`
+
+默认情况下，所有检测函数在客户端连接断开时自动销毁。如果需要更细粒度的控制，可以使用 `new_scope`
+
+```python
+from nicegui import ui
+from ex4nicegui import rxui, to_ref, effect, new_scope
+
+a = to_ref(0.0)
+
+scope1 = new_scope()
+
+@scope1.run
+def _():
+    @effect
+    def _():
+        print(f"scope 1:{a.value}")
+
+
+rxui.number(value=a)
+rxui.button("dispose scope 1", on_click=scope1.dispose)
+```
+
+---
+
 
 ## 组件功能
 
 ### vmodel
 在表单输入元素或组件上创建双向绑定。
 
 简单值类型的 `ref` 默认支持双向绑定
```

### Comparing `ex4nicegui-0.6.5/ex4nicegui/__init__.py` & `ex4nicegui-0.6.6/ex4nicegui/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     reactive,
     deep_ref,
     is_setter_ref,
     batch,
     is_reactive,
 )
 from ex4nicegui.utils.asyncComputed import async_computed
-
+from ex4nicegui.utils.clientScope import new_scope
 
 __all__ = [
     "async_computed",
     "is_reactive",
     "rxui",
     "ref_computed",
     "effect",
@@ -39,10 +39,11 @@
     "Ref",
     "ReadonlyRef",
     "reactive",
     "deep_ref",
     "batch",
     "to_raw",
     "is_setter_ref",
+    "new_scope",
 ]
 
-__version__ = "0.6.5"
+__version__ = "0.6.6"
```

### Comparing `ex4nicegui-0.6.5/ex4nicegui/bi/dataSource.py` & `ex4nicegui-0.6.6/ex4nicegui/bi/dataSource.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/bi/dataSourceFacade.py` & `ex4nicegui-0.6.6/ex4nicegui/bi/dataSourceFacade.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/bi/elements/layouts.py` & `ex4nicegui-0.6.6/ex4nicegui/bi/elements/layouts.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/bi/elements/models.py` & `ex4nicegui-0.6.6/ex4nicegui/bi/elements/models.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/bi/elements/text.py` & `ex4nicegui-0.6.6/ex4nicegui/bi/elements/text.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/bi/elements/ui_aggrid.py` & `ex4nicegui-0.6.6/ex4nicegui/bi/elements/ui_aggrid.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/bi/elements/ui_date_picker.js` & `ex4nicegui-0.6.6/ex4nicegui/bi/elements/ui_date_picker.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/bi/elements/ui_date_picker.py` & `ex4nicegui-0.6.6/ex4nicegui/bi/elements/ui_date_picker.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/bi/elements/ui_echarts.py` & `ex4nicegui-0.6.6/ex4nicegui/bi/elements/ui_echarts.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING, Any, Callable, Dict, Union, cast
 from nicegui.events import UiEventArguments
 from ex4nicegui.reactive import rxui
-from ex4nicegui.reactive.EChartsComponent.ECharts import (
-    EChartsMouseEventArguments,
-    echarts,
-)
+from ex4nicegui.reactive.EChartsComponent.ECharts import echarts
 from nicegui import ui
 from ex4nicegui.bi.dataSource import DataSource
 from .models import UiResult
 
 if TYPE_CHECKING:
     from ex4nicegui.bi.dataSourceFacade import DataSourceFacade
 
@@ -17,15 +14,15 @@
 class EChartsResult(UiResult[echarts]):
     def __init__(
         self, element: echarts, dataSource: DataSource, chart_update: Callable
     ) -> None:
         super().__init__(element, dataSource)
         self.chart_update = chart_update
 
-    def on_chart_click(self, handler: Callable[[EChartsMouseEventArguments], Any]):
+    def on_chart_click(self, handler: Callable[[UiEventArguments], Any]):
         return self.element.echarts_on("click", handler)
 
     def on_chart_click_blank(self, handler: Callable[[UiEventArguments], Any]):
         return self.element.on_click_blank(handler)
 
     def cancel_linkage(self, *source: Union[ui.element, "UiResult"]):
         super().cancel_linkage(*source)
```

### Comparing `ex4nicegui-0.6.5/ex4nicegui/bi/elements/ui_radio.py` & `ex4nicegui-0.6.6/ex4nicegui/bi/elements/ui_radio.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/bi/elements/ui_range.py` & `ex4nicegui-0.6.6/ex4nicegui/bi/elements/ui_range.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/bi/elements/ui_select.py` & `ex4nicegui-0.6.6/ex4nicegui/bi/elements/ui_select.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/bi/elements/ui_slider.py` & `ex4nicegui-0.6.6/ex4nicegui/bi/elements/ui_slider.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/bi/elements/ui_table.py` & `ex4nicegui-0.6.6/ex4nicegui/bi/elements/ui_table.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/bi/index.py` & `ex4nicegui-0.6.6/ex4nicegui/bi/index.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/bi/protocols.py` & `ex4nicegui-0.6.6/ex4nicegui/bi/protocols.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/experimental_/gridLayout/index.py` & `ex4nicegui-0.6.6/ex4nicegui/experimental_/gridLayout/index.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/gsap/gsap.py` & `ex4nicegui-0.6.6/ex4nicegui/gsap/gsap.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/gsap/timeline.js` & `ex4nicegui-0.6.6/ex4nicegui/gsap/timeline.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/gsap/timeline.py` & `ex4nicegui-0.6.6/ex4nicegui/gsap/timeline.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/gsap/wrapGsap.js` & `ex4nicegui-0.6.6/ex4nicegui/gsap/wrapGsap.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/layout/gridFlex/GridFlex.js` & `ex4nicegui-0.6.6/ex4nicegui/layout/gridFlex/GridFlex.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/layout/gridFlex/gridFlex.py` & `ex4nicegui-0.6.6/ex4nicegui/layout/gridFlex/gridFlex.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/layout/gridFlex/utils.py` & `ex4nicegui-0.6.6/ex4nicegui/layout/gridFlex/utils.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/layout/rxFlex/index.py` & `ex4nicegui-0.6.6/ex4nicegui/layout/rxFlex/index.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/layout/rxFlex/types.py` & `ex4nicegui-0.6.6/ex4nicegui/layout/rxFlex/types.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/libs/d3/d3-color.ems.js` & `ex4nicegui-0.6.6/ex4nicegui/libs/d3/d3-color.ems.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/libs/d3/d3-dispatch.ems.js` & `ex4nicegui-0.6.6/ex4nicegui/libs/d3/d3-dispatch.ems.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/libs/d3/d3-drag.ems.js` & `ex4nicegui-0.6.6/ex4nicegui/libs/d3/d3-drag.ems.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/libs/d3/d3-ease.ems.js` & `ex4nicegui-0.6.6/ex4nicegui/libs/d3/d3-ease.ems.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/libs/d3/d3-interpolate.ems.js` & `ex4nicegui-0.6.6/ex4nicegui/libs/d3/d3-interpolate.ems.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/libs/d3/d3-selection.ems.js` & `ex4nicegui-0.6.6/ex4nicegui/libs/d3/d3-selection.ems.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/libs/d3/d3-timer.ems.js` & `ex4nicegui-0.6.6/ex4nicegui/libs/d3/d3-timer.ems.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/libs/d3/d3-transition.ems.js` & `ex4nicegui-0.6.6/ex4nicegui/libs/d3/d3-transition.ems.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/libs/d3/d3-zoom.ems.js` & `ex4nicegui-0.6.6/ex4nicegui/libs/d3/d3-zoom.ems.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/libs/gsap/CSSPlugin.js` & `ex4nicegui-0.6.6/ex4nicegui/libs/gsap/CSSPlugin.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/libs/gsap/CSSRulePlugin.js` & `ex4nicegui-0.6.6/ex4nicegui/libs/gsap/CSSRulePlugin.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/libs/gsap/CustomEase.js` & `ex4nicegui-0.6.6/ex4nicegui/libs/gsap/CustomEase.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/libs/gsap/Draggable.js` & `ex4nicegui-0.6.6/ex4nicegui/libs/gsap/Draggable.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/libs/gsap/EasePack.js` & `ex4nicegui-0.6.6/ex4nicegui/libs/gsap/EasePack.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/libs/gsap/EaselPlugin.js` & `ex4nicegui-0.6.6/ex4nicegui/libs/gsap/EaselPlugin.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/libs/gsap/Flip.js` & `ex4nicegui-0.6.6/ex4nicegui/libs/gsap/Flip.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/libs/gsap/MotionPathPlugin.js` & `ex4nicegui-0.6.6/ex4nicegui/libs/gsap/MotionPathPlugin.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/libs/gsap/Observer.js` & `ex4nicegui-0.6.6/ex4nicegui/libs/gsap/Observer.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/libs/gsap/PixiPlugin.js` & `ex4nicegui-0.6.6/ex4nicegui/libs/gsap/PixiPlugin.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/libs/gsap/ScrollToPlugin.js` & `ex4nicegui-0.6.6/ex4nicegui/libs/gsap/ScrollToPlugin.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/libs/gsap/ScrollTrigger.js` & `ex4nicegui-0.6.6/ex4nicegui/libs/gsap/ScrollTrigger.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/libs/gsap/TextPlugin.js` & `ex4nicegui-0.6.6/ex4nicegui/libs/gsap/TextPlugin.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/libs/gsap/all.js` & `ex4nicegui-0.6.6/ex4nicegui/libs/gsap/all.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/libs/gsap/gsap-core.js` & `ex4nicegui-0.6.6/ex4nicegui/libs/gsap/gsap-core.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/libs/gsap/utils/matrix.js` & `ex4nicegui-0.6.6/ex4nicegui/libs/gsap/utils/matrix.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/libs/gsap/utils/paths.js` & `ex4nicegui-0.6.6/ex4nicegui/libs/gsap/utils/paths.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/libs/gsap/utils/strings.js` & `ex4nicegui-0.6.6/ex4nicegui/libs/gsap/utils/strings.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/EChartsComponent/ECharts.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/EChartsComponent/ECharts.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,83 +1,40 @@
 import os
 from typing import (
     Any,
     Callable,
     Dict,
-    List,
     Optional,
     Union,
 )
-from typing_extensions import Literal
-from dataclasses import dataclass
-from nicegui.dataclasses import KWONLY_SLOTS
-from nicegui.events import (
-    handle_event,
-    UiEventArguments,
-)
+
+from nicegui.events import handle_event, UiEventArguments, GenericEventArguments
 from nicegui.element import Element
 from nicegui.awaitable_response import AwaitableResponse
-from nicegui import ui
 from pathlib import Path
 import nicegui
-import uuid
+
+from .types import (
+    _T_event_name,
+)
+from ex4nicegui.reactive.deferredTask import DeferredTask
+from .utils import get_bound_event_args, create_event_handler_args
 
 NG_ROOT = Path(nicegui.__file__).parent / "elements"
 libraries = [NG_ROOT / "lib/echarts/echarts.min.js"]
 
 
-_Chart_Click_Args = [
-    "componentType",
-    "seriesType",
-    "seriesIndex",
-    "seriesName",
-    "name",
-    "dataIndex",
-    "data",
-    "dataType",
-    "value",
-    "color",
-]
-
-
-@dataclass(**KWONLY_SLOTS)
-class EChartsMouseEventArguments(UiEventArguments):
-    componentType: str
-    seriesType: str
-    seriesIndex: int
-    seriesName: str
-    name: str
-    dataIndex: int
-    data: dict
-    dataType: Optional[str]
-    value: Any
-    color: str
-
-
-_T_echats_on_callback = Callable[[EChartsMouseEventArguments], Any]
-_T_mouse_event_name = Literal[
-    "click",
-    "dblclick",
-    "mousedown",
-    "mousemove",
-    "mouseup",
-    "mouseover",
-    "mouseout",
-    "globalout",
-    "contextmenu",
-]
-
-
 class echarts(Element, component="ECharts.js", libraries=libraries):  # type: ignore
     def __init__(
         self,
         options: Optional[dict] = None,
         code: Optional[str] = None,
     ) -> None:
         super().__init__()
+        self.__deferred_task = DeferredTask()
 
         if (options is None) and (bool(code) is False):
             raise ValueError("At least one of options and code must be valid.")
 
         if code:
             code = os.linesep.join([s for s in code.splitlines() if s])
 
@@ -85,44 +42,14 @@
                 self._props["options"] = e.args
 
             self.on("__update_options_from_client", on__update_options_from_client)
 
         self._props["options"] = options
         self._props["code"] = code
 
-        self._echarts_on_tasks: List[Callable] = []
-        self._echarts_on_callback_map: Dict[str, _T_echats_on_callback] = {}
-
-        async def on_client_connect(
-            client: nicegui.Client,
-        ) -> Any:
-            await client.connected()
-
-            for func in self._echarts_on_tasks:
-                func()
-
-            client.connect_handlers.remove(on_client_connect)  # type: ignore
-
-        ui.context.client.on_connect(on_client_connect)
-
-        def echartsOn_handler(e):
-            callbackId = e.args["callbackId"]
-            params: Dict = e.args["params"]
-            params["dataType"] = params.get("dataType")
-
-            if callbackId in self._echarts_on_callback_map:
-                event_args = EChartsMouseEventArguments(
-                    sender=e.sender, client=e.client, **params
-                )
-                handler = self._echarts_on_callback_map[callbackId]
-
-                handle_event(handler, event_args)
-
-        self.on("event_on", echartsOn_handler)
-
     def update_chart(
         self,
         merge_opts: Optional[dict] = None,
     ):
         self.run_method("update_chart", merge_opts)
         self.update()
         return self
@@ -160,42 +87,32 @@
                 handler,
                 UiEventArguments(
                     sender=self,
                     client=self.client,
                 ),
             )
 
-        self.on(
-            "clickBlank",
-            inner_handler,
-            _Chart_Click_Args,
-        )
+        self.on("clickBlank", inner_handler)
 
     def echarts_on(
         self,
-        event_name: _T_mouse_event_name,
-        handler: _T_echats_on_callback,
+        event_name: _T_event_name,
+        handler: Callable[[UiEventArguments], None],
         query: Optional[Union[str, Dict]] = None,
     ):
-        if not ui.context.client.has_socket_connection:
-
-            def task_func():
-                self.echarts_on(event_name, handler, query)
-
-            self._echarts_on_tasks.append(task_func)
-            return
-
-        callback_id = uuid.uuid4().hex
-        self.run_method(
-            "echarts_on",
-            event_name,
-            query,
-            callback_id,
-        )
-        self._echarts_on_callback_map[callback_id] = handler
+        def org_handler(e: GenericEventArguments) -> None:
+            event_args = create_event_handler_args(event_name, e)
+            handle_event(handler, event_args)
+
+        ui_event_name = f"chart:{event_name}"
+        super().on(ui_event_name, org_handler, args=get_bound_event_args(event_name))
+
+        @self.__deferred_task.register
+        def _():
+            self.run_method("echarts_on", ui_event_name, query)
 
     def run_chart_method(
         self, name: str, *args, timeout: float = 1, check_interval: float = 0.01
     ) -> AwaitableResponse:
         """Run a method of the JSONEditor instance.
 
         See the `ECharts documentation <https://echarts.apache.org/en/api.html#echartsInstance>`_ for a list of methods.
```

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/UseDraggable/UseDraggable.js` & `ex4nicegui-0.6.6/ex4nicegui/reactive/UseDraggable/UseDraggable.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/UseDraggable/UseDraggable.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/UseDraggable/UseDraggable.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/__init__.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/__init__.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/dropZone/dropZone.js` & `ex4nicegui-0.6.6/ex4nicegui/reactive/dropZone/dropZone.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/dropZone/dropZone.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/dropZone/dropZone.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/fileWatcher.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/fileWatcher.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/local_file_picker.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/local_file_picker.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/mermaid/mermaid.js` & `ex4nicegui-0.6.6/ex4nicegui/reactive/mermaid/mermaid.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/mermaid/mermaid.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/mermaid/mermaid.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/aggrid.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/aggrid.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/base.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/base.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/button.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/button.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/card.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/card.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/checkbox.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/checkbox.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/circular_progress.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/circular_progress.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/color_picker.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/color_picker.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/column.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/column.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/date.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/date.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/drawer.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/drawer.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/echarts.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/echarts.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,27 @@
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Union, cast, Optional
-from typing_extensions import Literal
 from ex4nicegui.reactive.utils import ParameterClassifier
-from ex4nicegui.utils.signals import on
-
 from ex4nicegui.utils.signals import (
     ReadonlyRef,
     is_ref,
     ref_computed,
     _TMaybeRef as TMaybeRef,
     to_value,
     to_raw,
+    on,
 )
 from .base import BindableUi
-from ex4nicegui.reactive.EChartsComponent.ECharts import (
-    echarts,
-    EChartsMouseEventArguments,
-)
+from ex4nicegui.reactive.EChartsComponent.ECharts import echarts
+from ex4nicegui.reactive.EChartsComponent.types import _T_event_name
+from ex4nicegui.reactive.EChartsComponent.events import EChartsMouseEventArguments
 
 from nicegui.awaitable_response import AwaitableResponse
 from nicegui import ui, app
 
-_TEventName = Literal[
-    "click",
-    "dblclick",
-    "mousedown",
-    "mousemove",
-    "mouseup",
-    "mouseover",
-    "mouseout",
-    "globalout",
-    "contextmenu",
-]
-
 
 class EChartsBindableUi(BindableUi[echarts]):
     EChartsMouseEventArguments = EChartsMouseEventArguments
 
     def __init__(
         self,
         options: Optional[TMaybeRef[Dict]] = None,
@@ -46,14 +31,15 @@
         pc = ParameterClassifier(
             locals(), maybeRefs=["options", "code"], exclude=["not_merge"]
         )
 
         value_kws = pc.get_values_kws()
 
         element = echarts(**value_kws).classes("grow self-stretch h-[16rem]")
+
         super().__init__(element)  # type: ignore
 
         self.__update_setting = None
         if not_merge is not None:
             self.__update_setting = {"notMerge": not_merge}
 
         for key, value in pc.get_bindings().items():
@@ -74,25 +60,25 @@
             src = app.add_static_file(local_file=src)
 
         assert isinstance(src, str)
 
         ui.add_body_html(
             rf"""
             <script>
-                window.addEventListener('DOMContentLoaded', () => {{
-                    fetch("{src}")
-                        .then((response) => response.json())
-                        .then((data) => {{
-                            echarts.registerMap('{map_name}', data);
-                        }});
-                }});
+                if (typeof window.ex4ngEchartsMapTasks === "undefined") {{ 
+                    window.ex4ngEchartsMapTasks = new Map();
+                }}
+
+                window.ex4ngEchartsMapTasks.set('{map_name}', '{src}');
             </script>
         """
         )
 
+        return cls
+
     @classmethod
     def from_pyecharts(cls, chart: TMaybeRef):
         if is_ref(chart):
 
             @ref_computed
             def chart_opt():
                 if not bool(chart.value):
@@ -143,15 +129,15 @@
             ele.update_options(to_raw(to_value(ref_ui)), self.__update_setting)
             ele.update()
 
         return self
 
     def on(
         self,
-        event_name: _TEventName,
+        event_name: _T_event_name,
         handler: Callable[..., Any],
         query: Optional[Union[str, Dict]] = None,
     ):
         """echart instance event on.
 
         [English Documentation](https://echarts.apache.org/handbook/en/concepts/event/)
 
@@ -220,14 +206,15 @@
 
         bar.on("mouseover", on_first_series_mouseover, query={"seriesName": "first"})
         ```
 
         ---
         """
         self.element.echarts_on(event_name, handler, query)
+        return self
 
     def run_chart_method(
         self, name: str, *args, timeout: float = 1, check_interval: float = 0.01
     ) -> AwaitableResponse:
         """Run a method of the JSONEditor instance.
 
         See the `ECharts documentation <https://echarts.apache.org/en/api.html#echartsInstance>`_ for a list of methods.
```

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/expansion.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/expansion.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/grid.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/grid.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/html.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/html.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/icon.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/icon.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/image.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/image.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/input.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/input.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/knob.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/knob.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/label.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/label.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/linear_progress.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/linear_progress.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/number.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/number.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import (
     Any,
     Callable,
     Optional,
     TypeVar,
     Dict,
+    Union,
 )
 from ex4nicegui.reactive.utils import ParameterClassifier
 from ex4nicegui.utils.apiEffect import ui_effect
 
 from ex4nicegui.utils.signals import (
     ReadonlyRef,
     _TMaybeRef as TMaybeRef,
@@ -21,15 +22,15 @@
 
 class NumberBindableUi(BindableUi[ui.number]):
     def __init__(
         self,
         label: Optional[TMaybeRef[str]] = None,
         *,
         placeholder: Optional[TMaybeRef[str]] = None,
-        value: Optional[TMaybeRef[float]] = None,
+        value: Optional[Union[TMaybeRef[float], TMaybeRef[int]]] = None,
         min: Optional[TMaybeRef[float]] = None,
         max: Optional[TMaybeRef[float]] = None,
         step: Optional[TMaybeRef[float]] = None,
         prefix: Optional[TMaybeRef[str]] = None,
         suffix: Optional[TMaybeRef[str]] = None,
         format: Optional[TMaybeRef[str]] = None,
         on_change: Optional[Callable[..., Any]] = None,
```

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/radio.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/radio.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/row.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/row.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/select.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/select.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/slider.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/slider.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/switch.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/switch.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/tab.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/tab.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/tab_panel.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/tab_panel.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/tab_panels.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/tab_panels.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/table.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/table.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/tabs.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/tabs.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/textarea.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/textarea.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/upload.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/upload.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/q_pagination.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/q_pagination.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/transitionGroup.js` & `ex4nicegui-0.6.6/ex4nicegui/reactive/transitionGroup.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/transitionGroup.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/transitionGroup.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/useMouse/UseMouse.js` & `ex4nicegui-0.6.6/ex4nicegui/reactive/useMouse/UseMouse.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/useMouse/UseMouse.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/useMouse/UseMouse.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/usePagination.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/usePagination.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/utils.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/utils.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/vfor.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/vfor.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/reactive/vmodel.py` & `ex4nicegui-0.6.6/ex4nicegui/reactive/vmodel.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/tools/debug.py` & `ex4nicegui-0.6.6/ex4nicegui/tools/debug.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/utils/apiEffect.py` & `ex4nicegui-0.6.6/ex4nicegui/utils/apiEffect.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/utils/asyncComputed.py` & `ex4nicegui-0.6.6/ex4nicegui/utils/asyncComputed.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/utils/clientScope.py` & `ex4nicegui-0.6.6/ex4nicegui/utils/clientScope.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Dict
 from signe.core.scope import ScopeSuite
 from nicegui import Client, ui
 
-
 _TClientID = str
 
 
 class NgScopeSuite(ScopeSuite):
     def __init__(self) -> None:
         super().__init__()
         self._top_scope = self.scope()
@@ -14,31 +13,40 @@
 
 
 class NgClientScopeManager:
     def __init__(self) -> None:
         self._client_scope_map: Dict[_TClientID, NgScopeSuite] = {}
 
     def new_scope(self, detached: bool = False):
-        return self.get_current_scope().scope(detached)
+        """Create a scope that can collect all reactive watch functions within it, allowing for a unified destruction process.
 
-    def get_current_scope(self):
-        # if len(ng_context.get_slot_stack()) <= 0:
-        #     return
+        @see - https://github.com/CrystalWindSnake/ex4nicegui/blob/main/README.en.md#new_scope
+        @中文文档 - https://gitee.com/carson_add/ex4nicegui/tree/main/#new_scope
+
+        Args:
+            detached (bool, optional): Whether the scope should be detached from the client. Defaults to False.
+
+        """
+        return self.get_current_scope().scope(detached=detached)
 
+    def get_current_scope(self):
         client = ui.context.client
 
         if client.id not in self._client_scope_map:
             self._client_scope_map[client.id] = NgScopeSuite()
 
             # shared clients always not dispose their scope
             if not client.shared:
 
                 @client.on_disconnect
                 def _(e: Client):
                     if e.id in self._client_scope_map:
-                        self._client_scope_map[e.id]._top_scope.dispose()
+                        self._client_scope_map[e.id]._top_scope.dispose()  # type: ignore
                         del self._client_scope_map[e.id]
 
         return self._client_scope_map[client.id]
 
 
 _CLIENT_SCOPE_MANAGER = NgClientScopeManager()
+
+
+new_scope = _CLIENT_SCOPE_MANAGER.new_scope
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ex4nicegui-0.6.5/ex4nicegui/utils/common.py` & `ex4nicegui-0.6.6/ex4nicegui/utils/common.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/utils/effect.py` & `ex4nicegui-0.6.6/ex4nicegui/utils/effect.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/utils/scheduler.py` & `ex4nicegui-0.6.6/ex4nicegui/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui/utils/signals.py` & `ex4nicegui-0.6.6/ex4nicegui/utils/signals.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.5/ex4nicegui.egg-info/PKG-INFO` & `ex4nicegui-0.6.6/ex4nicegui.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ex4nicegui
-Version: 0.6.5
+Version: 0.6.6
 Summary: Extension library based on nicegui, providing data responsive,BI functionality modules
 Home-page: 
 Author: carson_jia
 Author-email: 568166495@qq.com
 License: MIT license
 Keywords: nicegui,ex4nicegui,webui
 Classifier: Intended Audience :: Developers
@@ -416,14 +416,39 @@
 
 - If the parameter `onchanges` is True (the default value is False), the specified function will not be executed at binding time.
 
 > Never spread a lot of data processing logic across multiple `on`s or `effects`s, which should be mostly interface manipulation logic rather than responsive data processing logic
 
 ---
 
+### `new_scope`
+
+By default, all watch functions are automatically destroyed when the client connection is disconnected. For finer-grained control, the `new_scope` function can be utilized.
+
+```python
+from nicegui import ui
+from ex4nicegui import rxui, to_ref, effect, new_scope
+
+a = to_ref(0.0)
+
+scope1 = new_scope()
+
+@scope1.run
+def _():
+    @effect
+    def _():
+        print(f"scope 1:{a.value}")
+
+
+rxui.number(value=a)
+rxui.button("dispose scope 1", on_click=scope1.dispose)
+```
+
+---
+
 ## functionality
 
 ### vmodel
 Create two-way bindings on form input elements or components.
 
 Bidirectional bindings are supported by default for `ref` simple value types
 ```python
```

### Comparing `ex4nicegui-0.6.5/ex4nicegui.egg-info/SOURCES.txt` & `ex4nicegui-0.6.6/ex4nicegui.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -72,14 +72,15 @@
 ex4nicegui/libs/gsap/all.js
 ex4nicegui/libs/gsap/gsap-core.js
 ex4nicegui/libs/gsap/utils/__init__.py
 ex4nicegui/libs/gsap/utils/matrix.js
 ex4nicegui/libs/gsap/utils/paths.js
 ex4nicegui/libs/gsap/utils/strings.js
 ex4nicegui/reactive/__init__.py
+ex4nicegui/reactive/deferredTask.py
 ex4nicegui/reactive/empty.js
 ex4nicegui/reactive/empty.py
 ex4nicegui/reactive/fileWatcher.py
 ex4nicegui/reactive/local_file_picker.py
 ex4nicegui/reactive/q_pagination.py
 ex4nicegui/reactive/rxui.py
 ex4nicegui/reactive/transitionGroup.js
@@ -88,14 +89,17 @@
 ex4nicegui/reactive/utils.py
 ex4nicegui/reactive/vfor.js
 ex4nicegui/reactive/vfor.py
 ex4nicegui/reactive/vmodel.py
 ex4nicegui/reactive/EChartsComponent/ECharts.js
 ex4nicegui/reactive/EChartsComponent/ECharts.py
 ex4nicegui/reactive/EChartsComponent/__init__.py
+ex4nicegui/reactive/EChartsComponent/events.py
+ex4nicegui/reactive/EChartsComponent/types.py
+ex4nicegui/reactive/EChartsComponent/utils.py
 ex4nicegui/reactive/UseDraggable/UseDraggable.js
 ex4nicegui/reactive/UseDraggable/UseDraggable.py
 ex4nicegui/reactive/UseDraggable/__init__.py
 ex4nicegui/reactive/dropZone/__init__.py
 ex4nicegui/reactive/dropZone/dropZone.js
 ex4nicegui/reactive/dropZone/dropZone.py
 ex4nicegui/reactive/mermaid/__init__.py
```

### Comparing `ex4nicegui-0.6.5/setup.py` & `ex4nicegui-0.6.6/setup.py`

 * *Files identical despite different names*

