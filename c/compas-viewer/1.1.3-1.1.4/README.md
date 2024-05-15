# Comparing `tmp/compas_viewer-1.1.3.tar.gz` & `tmp/compas_viewer-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compas_viewer-1.1.3.tar", last modified: Tue May 14 18:30:34 2024, max compression
+gzip compressed data, was "compas_viewer-1.1.4.tar", last modified: Tue May 14 20:54:20 2024, max compression
```

## Comparing `compas_viewer-1.1.3.tar` & `compas_viewer-1.1.4.tar`

### file list

```diff
@@ -1,145 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:30:34.486638 compas_viewer-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-05-14 18:30:34.486638 compas_viewer-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 18:30:34.486638 compas_viewer-1.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:30:34.462638 compas_viewer-1.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:30:34.466638 compas_viewer-1.1.3/src/compas_viewer/
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:30:34.466638 compas_viewer-1.1.3/src/compas_viewer/actions/
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/actions/action.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/actions/delete_selected.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/actions/info.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/actions/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/actions/select_all.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/actions/viewmode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/actions/zoom_selected.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:30:34.470638 compas_viewer-1.1.3/src/compas_viewer/components/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/button_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/component_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:30:34.470638 compas_viewer-1.1.3/src/compas_viewer/components/renderer/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/renderer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14195 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/renderer/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)    22069 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/renderer/renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8427 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/renderer/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:30:34.470638 compas_viewer-1.1.3/src/compas_viewer/components/renderer/shaders/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/renderer/shaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/renderer/shaders/arrow.frag
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/renderer/shaders/arrow.vert
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/renderer/shaders/grid.frag
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/renderer/shaders/grid.vert
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/renderer/shaders/instance.frag
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/renderer/shaders/instance.vert
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/renderer/shaders/model.frag
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/renderer/shaders/model.vert
--rw-r--r--   0 runner    (1001) docker     (127)    10418 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/renderer/shaders/shader.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/renderer/shaders/tag.frag
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/renderer/shaders/tag.vert
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/setting_components.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/treeform_components.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/widget_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/config.json
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:30:34.474638 compas_viewer-1.1.3/src/compas_viewer/configurations/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/configurations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/configurations/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/configurations/controller_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:30:34.474638 compas_viewer-1.1.3/src/compas_viewer/configurations/default_config/
--rw-r--r--   0 runner    (1001) docker     (127)   714456 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/configurations/default_config/FreeSans.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/configurations/default_config/controller.json
--rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/configurations/default_config/layout.json
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/configurations/default_config/renderer.json
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/configurations/default_config/viewer.json
--rw-r--r--   0 runner    (1001) docker     (127)     9158 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/configurations/layout_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/configurations/renderer_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/configurations/viewer_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:30:34.474638 compas_viewer-1.1.3/src/compas_viewer/controller/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8682 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/controller/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/controller/mouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/gl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:30:34.478639 compas_viewer-1.1.3/src/compas_viewer/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/icons/camera_info.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/icons/compas_icon_white.png
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/icons/delete_selected.svg
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/icons/export_file.svg
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/icons/gl_info.svg
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/icons/import_file.svg
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/icons/selection_info.svg
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/icons/view_front.svg
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/icons/view_perspective.svg
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/icons/view_right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/icons/view_top.svg
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/icons/zoom_selected.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:30:34.478639 compas_viewer-1.1.3/src/compas_viewer/layout/
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/layout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/layout/collapsiblebox.py
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/layout/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/layout/menubar.py
--rw-r--r--   0 runner    (1001) docker     (127)    14986 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/layout/propertyform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/layout/sidedock.py
--rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/layout/slider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/layout/statusbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/layout/toolbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/layout/treeform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/layout/viewport.py
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/layout/window.py
--rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/qt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:30:34.482638 compas_viewer-1.1.3/src/compas_viewer/scene/
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/boxobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/brepobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/capsuleobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/circleobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/collectionobject.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/coneobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/cylinderobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/ellipseobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/frameobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/geometryobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/graphobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/gridobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/groupobject.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/lineobject.py
--rw-r--r--   0 runner    (1001) docker     (127)    13222 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/meshobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/nurbscurveobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/nurbssurfaceobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/planeobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/pointcloudobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/pointobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/polygonobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/polyhedronobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/polylineobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/scene.py
--rw-r--r--   0 runner    (1001) docker     (127)    18821 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/sceneobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/sphereobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     7747 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/tagobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/torusobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/vectorobject.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:30:34.486638 compas_viewer-1.1.3/src/compas_viewer/ui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/ui/mainwindow.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/ui/menubar.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/ui/statusbar.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/ui/toolbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/ui/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/ui/viewport.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:30:34.486638 compas_viewer-1.1.3/src/compas_viewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-05-14 18:30:34.000000 compas_viewer-1.1.3/src/compas_viewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-05-14 18:30:34.000000 compas_viewer-1.1.3/src/compas_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 18:30:34.000000 compas_viewer-1.1.3/src/compas_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 18:30:34.000000 compas_viewer-1.1.3/src/compas_viewer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-14 18:30:34.000000 compas_viewer-1.1.3/src/compas_viewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 18:30:34.000000 compas_viewer-1.1.3/src/compas_viewer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:30:34.486638 compas_viewer-1.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/tests/test_placeholder.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/tests/test_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:54:20.868795 compas_viewer-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-05-14 20:54:20.868795 compas_viewer-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 20:54:20.868795 compas_viewer-1.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:54:20.836795 compas_viewer-1.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:54:20.844795 compas_viewer-1.1.4/src/compas_viewer/
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:54:20.844795 compas_viewer-1.1.4/src/compas_viewer/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/actions/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/actions/delete_selected.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/actions/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/actions/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/actions/select_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/actions/viewmode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/actions/zoom_selected.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:54:20.844795 compas_viewer-1.1.4/src/compas_viewer/components/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/components/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/components/double_edit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:54:20.848795 compas_viewer-1.1.4/src/compas_viewer/components/renderer/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/components/renderer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14195 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/components/renderer/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22069 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/components/renderer/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8427 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/components/renderer/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:54:20.848795 compas_viewer-1.1.4/src/compas_viewer/components/renderer/shaders/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/components/renderer/shaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/components/renderer/shaders/arrow.frag
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/components/renderer/shaders/arrow.vert
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/components/renderer/shaders/grid.frag
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/components/renderer/shaders/grid.vert
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/components/renderer/shaders/instance.frag
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/components/renderer/shaders/instance.vert
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/components/renderer/shaders/model.frag
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/components/renderer/shaders/model.vert
+-rw-r--r--   0 runner    (1001) docker     (127)    10418 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/components/renderer/shaders/shader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/components/renderer/shaders/tag.frag
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/components/renderer/shaders/tag.vert
+-rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/components/treeform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/components/widget_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:54:20.848795 compas_viewer-1.1.4/src/compas_viewer/configurations/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/configurations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/configurations/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/configurations/controller_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:54:20.852795 compas_viewer-1.1.4/src/compas_viewer/configurations/default_config/
+-rw-r--r--   0 runner    (1001) docker     (127)   714456 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/configurations/default_config/FreeSans.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/configurations/default_config/controller.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/configurations/default_config/layout.json
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/configurations/default_config/renderer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/configurations/default_config/viewer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9158 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/configurations/layout_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/configurations/renderer_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/configurations/viewer_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:54:20.852795 compas_viewer-1.1.4/src/compas_viewer/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8682 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/controller/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/controller/mouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/gl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:54:20.856795 compas_viewer-1.1.4/src/compas_viewer/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/icons/camera_info.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/icons/compas_icon_white.png
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/icons/delete_selected.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/icons/export_file.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/icons/gl_info.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/icons/import_file.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/icons/selection_info.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/icons/view_front.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/icons/view_perspective.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/icons/view_right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/icons/view_top.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/icons/zoom_selected.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:54:20.856795 compas_viewer-1.1.4/src/compas_viewer/layout/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/layout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/layout/collapsiblebox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/layout/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/layout/menubar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14986 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/layout/propertyform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/layout/sidedock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/layout/slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/layout/statusbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/layout/toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/layout/treeform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/layout/viewport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/layout/window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/qt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:54:20.864795 compas_viewer-1.1.4/src/compas_viewer/scene/
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/scene/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/scene/boxobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/scene/brepobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/scene/capsuleobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/scene/circleobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/scene/collectionobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/scene/coneobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/scene/cylinderobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/scene/ellipseobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/scene/frameobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/scene/geometryobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/scene/graphobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/scene/gridobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/scene/groupobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/scene/lineobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13222 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/scene/meshobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/scene/nurbscurveobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/scene/nurbssurfaceobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/scene/planeobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/scene/pointcloudobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/scene/pointobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/scene/polygonobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/scene/polyhedronobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/scene/polylineobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/scene/scene.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18821 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/scene/sceneobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/scene/sphereobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7747 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/scene/tagobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/scene/torusobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/scene/vectorobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:54:20.864795 compas_viewer-1.1.4/src/compas_viewer/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/ui/mainwindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/ui/menubar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/ui/statusbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/ui/toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/ui/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/ui/viewport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/src/compas_viewer/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:54:20.864795 compas_viewer-1.1.4/src/compas_viewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-05-14 20:54:20.000000 compas_viewer-1.1.4/src/compas_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-14 20:54:20.000000 compas_viewer-1.1.4/src/compas_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 20:54:20.000000 compas_viewer-1.1.4/src/compas_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 20:54:20.000000 compas_viewer-1.1.4/src/compas_viewer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-14 20:54:20.000000 compas_viewer-1.1.4/src/compas_viewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 20:54:20.000000 compas_viewer-1.1.4/src/compas_viewer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:54:20.864795 compas_viewer-1.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/tests/test_placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 20:54:10.000000 compas_viewer-1.1.4/tests/test_viewer.py
```

### Comparing `compas_viewer-1.1.3/LICENSE` & `compas_viewer-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/PKG-INFO` & `compas_viewer-1.1.4/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compas_viewer
-Version: 1.1.3
+Version: 1.1.4
 Summary: Standalone viewer for COMPAS 2 based on PyOpenGL and PyQt6.
 Author-email: tom van mele <tom.v.mele@gmail.com>, Li Chen <li.chen@arch.ethz.ch>, Zac Zhuo Zhang <zhuo.zhang@arch.ethz.ch>
 License: MIT License
         
         COMPAS Association
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `compas_viewer-1.1.3/README.md` & `compas_viewer-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/pyproject.toml` & `compas_viewer-1.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 ]
 
 # ============================================================================
 # replace bumpversion.cfg
 # ============================================================================
 
 [tool.bumpversion]
-current_version = "1.1.3"
+current_version = "1.1.4"
 message = "Bump version to {new_version}"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "src/compas_viewer/__init__.py"
 search = "{current_version}"
```

### Comparing `compas_viewer-1.1.3/src/compas_viewer/__init__.py` & `compas_viewer-1.1.4/src/compas_viewer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import os
 
 
 __author__ = ["Li Chen"]
 __copyright__ = "COMPAS Association"
 __license__ = "MIT License"
 __email__ = "li.chen@arch.ethz.ch"
-__version__ = "1.1.3"
+__version__ = "1.1.4"
 
 
 HERE = os.path.dirname(__file__)
 
 HOME = os.path.abspath(os.path.join(HERE, "../../"))
 DATA = os.path.abspath(os.path.join(HOME, "data"))
 DOCS = os.path.abspath(os.path.join(HOME, "docs"))
```

### Comparing `compas_viewer-1.1.3/src/compas_viewer/__main__.py` & `compas_viewer-1.1.4/src/compas_viewer/__main__.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/actions/__init__.py` & `compas_viewer-1.1.4/src/compas_viewer/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/actions/action.py` & `compas_viewer-1.1.4/src/compas_viewer/actions/action.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/actions/info.py` & `compas_viewer-1.1.4/src/compas_viewer/actions/info.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/actions/io.py` & `compas_viewer-1.1.4/src/compas_viewer/actions/io.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/actions/viewmode.py` & `compas_viewer-1.1.4/src/compas_viewer/actions/viewmode.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/actions/zoom_selected.py` & `compas_viewer-1.1.4/src/compas_viewer/actions/zoom_selected.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/components/button_factory.py` & `compas_viewer-1.1.4/src/compas_viewer/components/button.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,14 +7,14 @@
 
 
 def set_icon_path(icon_name: str) -> str:
     path = QtGui.QIcon(str(pathlib.Path(__file__).parent.parent / "icons" / icon_name))
     return path
 
 
-class ButtonFactory(QtWidgets.QPushButton):
+class Button(QtWidgets.QPushButton):
     def __init__(self, icon_name: str, tooltip: str, action: Callable[[], None], parent=None):
-        super().__init__(parent)
+        super().__init__()
         self.setIcon(QtGui.QIcon(set_icon_path(icon_name)))
         self.setToolTip(tooltip)
         self.setIconSize(QtCore.QSize(12, 12))
         self.clicked.connect(action)
```

### Comparing `compas_viewer-1.1.3/src/compas_viewer/components/renderer/camera.py` & `compas_viewer-1.1.4/src/compas_viewer/components/renderer/camera.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/components/renderer/renderer.py` & `compas_viewer-1.1.4/src/compas_viewer/components/renderer/renderer.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/components/renderer/selector.py` & `compas_viewer-1.1.4/src/compas_viewer/components/renderer/selector.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/components/renderer/shaders/model.frag` & `compas_viewer-1.1.4/src/compas_viewer/components/renderer/shaders/model.frag`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/components/renderer/shaders/shader.py` & `compas_viewer-1.1.4/src/compas_viewer/components/renderer/shaders/shader.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/components/widget_tools.py` & `compas_viewer-1.1.4/src/compas_viewer/components/widget_tools.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/config.py` & `compas_viewer-1.1.4/src/compas_viewer/config.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/configurations/__init__.py` & `compas_viewer-1.1.4/src/compas_viewer/configurations/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/configurations/controller_config.py` & `compas_viewer-1.1.4/src/compas_viewer/configurations/controller_config.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/configurations/default_config/FreeSans.ttf` & `compas_viewer-1.1.4/src/compas_viewer/configurations/default_config/FreeSans.ttf`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/configurations/default_config/controller.json` & `compas_viewer-1.1.4/src/compas_viewer/configurations/default_config/controller.json`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/configurations/default_config/layout.json` & `compas_viewer-1.1.4/src/compas_viewer/configurations/default_config/layout.json`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/configurations/default_config/renderer.json` & `compas_viewer-1.1.4/src/compas_viewer/configurations/default_config/renderer.json`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/configurations/default_config/viewer.json` & `compas_viewer-1.1.4/src/compas_viewer/configurations/default_config/viewer.json`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/configurations/layout_config.py` & `compas_viewer-1.1.4/src/compas_viewer/configurations/layout_config.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/configurations/renderer_config.py` & `compas_viewer-1.1.4/src/compas_viewer/configurations/renderer_config.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/configurations/viewer_config.py` & `compas_viewer-1.1.4/src/compas_viewer/configurations/viewer_config.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/controller/controller.py` & `compas_viewer-1.1.4/src/compas_viewer/controller/controller.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/controller/mouse.py` & `compas_viewer-1.1.4/src/compas_viewer/controller/mouse.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/gl.py` & `compas_viewer-1.1.4/src/compas_viewer/gl.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/icons/compas_icon_white.png` & `compas_viewer-1.1.4/src/compas_viewer/icons/compas_icon_white.png`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/icons/export_file.svg` & `compas_viewer-1.1.4/src/compas_viewer/icons/export_file.svg`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/icons/import_file.svg` & `compas_viewer-1.1.4/src/compas_viewer/icons/import_file.svg`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/icons/selection_info.svg` & `compas_viewer-1.1.4/src/compas_viewer/icons/selection_info.svg`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/icons/view_right.svg` & `compas_viewer-1.1.4/src/compas_viewer/icons/view_right.svg`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/layout/collapsiblebox.py` & `compas_viewer-1.1.4/src/compas_viewer/layout/collapsiblebox.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/layout/layout.py` & `compas_viewer-1.1.4/src/compas_viewer/layout/layout.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/layout/menubar.py` & `compas_viewer-1.1.4/src/compas_viewer/layout/menubar.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/layout/propertyform.py` & `compas_viewer-1.1.4/src/compas_viewer/layout/propertyform.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/layout/sidedock.py` & `compas_viewer-1.1.4/src/compas_viewer/layout/sidedock.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/layout/slider.py` & `compas_viewer-1.1.4/src/compas_viewer/layout/slider.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/layout/statusbar.py` & `compas_viewer-1.1.4/src/compas_viewer/layout/statusbar.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/layout/toolbar.py` & `compas_viewer-1.1.4/src/compas_viewer/layout/toolbar.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/layout/treeform.py` & `compas_viewer-1.1.4/src/compas_viewer/components/treeform.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/layout/viewport.py` & `compas_viewer-1.1.4/src/compas_viewer/layout/viewport.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/layout/window.py` & `compas_viewer-1.1.4/src/compas_viewer/layout/window.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/qt.py` & `compas_viewer-1.1.4/src/compas_viewer/qt.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/scene/__init__.py` & `compas_viewer-1.1.4/src/compas_viewer/scene/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/scene/boxobject.py` & `compas_viewer-1.1.4/src/compas_viewer/scene/boxobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/scene/brepobject.py` & `compas_viewer-1.1.4/src/compas_viewer/scene/brepobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/scene/capsuleobject.py` & `compas_viewer-1.1.4/src/compas_viewer/scene/capsuleobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/scene/circleobject.py` & `compas_viewer-1.1.4/src/compas_viewer/scene/circleobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/scene/collectionobject.py` & `compas_viewer-1.1.4/src/compas_viewer/scene/collectionobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/scene/coneobject.py` & `compas_viewer-1.1.4/src/compas_viewer/scene/coneobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/scene/cylinderobject.py` & `compas_viewer-1.1.4/src/compas_viewer/scene/cylinderobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/scene/ellipseobject.py` & `compas_viewer-1.1.4/src/compas_viewer/scene/ellipseobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/scene/frameobject.py` & `compas_viewer-1.1.4/src/compas_viewer/scene/frameobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/scene/geometryobject.py` & `compas_viewer-1.1.4/src/compas_viewer/scene/geometryobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/scene/graphobject.py` & `compas_viewer-1.1.4/src/compas_viewer/scene/graphobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/scene/gridobject.py` & `compas_viewer-1.1.4/src/compas_viewer/scene/gridobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/scene/groupobject.py` & `compas_viewer-1.1.4/src/compas_viewer/scene/groupobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/scene/lineobject.py` & `compas_viewer-1.1.4/src/compas_viewer/scene/lineobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/scene/meshobject.py` & `compas_viewer-1.1.4/src/compas_viewer/scene/meshobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/scene/nurbscurveobject.py` & `compas_viewer-1.1.4/src/compas_viewer/scene/nurbscurveobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/scene/nurbssurfaceobject.py` & `compas_viewer-1.1.4/src/compas_viewer/scene/nurbssurfaceobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/scene/planeobject.py` & `compas_viewer-1.1.4/src/compas_viewer/scene/planeobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/scene/pointcloudobject.py` & `compas_viewer-1.1.4/src/compas_viewer/scene/pointcloudobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/scene/pointobject.py` & `compas_viewer-1.1.4/src/compas_viewer/scene/pointobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/scene/polygonobject.py` & `compas_viewer-1.1.4/src/compas_viewer/scene/polygonobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/scene/polyhedronobject.py` & `compas_viewer-1.1.4/src/compas_viewer/scene/polyhedronobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/scene/polylineobject.py` & `compas_viewer-1.1.4/src/compas_viewer/scene/polylineobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/scene/scene.py` & `compas_viewer-1.1.4/src/compas_viewer/scene/scene.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/scene/sceneobject.py` & `compas_viewer-1.1.4/src/compas_viewer/scene/sceneobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/scene/sphereobject.py` & `compas_viewer-1.1.4/src/compas_viewer/scene/sphereobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/scene/tagobject.py` & `compas_viewer-1.1.4/src/compas_viewer/scene/tagobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/scene/torusobject.py` & `compas_viewer-1.1.4/src/compas_viewer/scene/torusobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/scene/vectorobject.py` & `compas_viewer-1.1.4/src/compas_viewer/scene/vectorobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/singleton.py` & `compas_viewer-1.1.4/src/compas_viewer/singleton.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/ui/mainwindow.py` & `compas_viewer-1.1.4/src/compas_viewer/ui/mainwindow.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer/ui/toolbar.py` & `compas_viewer-1.1.4/src/compas_viewer/ui/toolbar.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from compas_viewer.base import Base
-from compas_viewer.components.button_factory import ButtonFactory
+from compas_viewer.components.button import Button
 
 
 def test_action() -> None:
     pass
 
 
 class ToolBar(Base):
@@ -11,8 +11,8 @@
         self.widget = None
 
     def lazy_init(self):
         self.widget = self.viewer.ui.window.addToolBar("Tools")
         self.widget.setMovable(False)
         self.widget.setObjectName("Tools")
         self.widget.setHidden(not self.viewer.config.ui.toolbar.show)
-        self.widget.addWidget(ButtonFactory("zoom_selected.svg", "zoom", test_action()))
+        self.widget.addWidget(Button("zoom_selected.svg", "zoom", test_action()))
```

### Comparing `compas_viewer-1.1.3/src/compas_viewer/ui/ui.py` & `compas_viewer-1.1.4/src/compas_viewer/ui/ui.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 from compas_viewer.base import Base
-from compas_viewer.components.component_manager import ComponentsManager
 
 from .mainwindow import MainWindow
 from .menubar import MenuBar
 from .statusbar import SatusBar
 from .toolbar import ToolBar
 from .viewport import ViewPort
 
 
 class UI(Base):
     def __init__(self) -> None:
-        self.components_manager = ComponentsManager()
         self.window = MainWindow()
         self.menubar = MenuBar()
         self.statusbar = SatusBar()
         self.toolbar = ToolBar()
         self.viewport = ViewPort()
 
     def lazy_init(self):
         width = self.viewer.config.window.width
         height = self.viewer.config.window.height
 
         self.resize(width, height)
-        self.components_manager.lazy_init()
         self.window.lazy_init()
         self.menubar.lazy_init()
         self.statusbar.lazy_init()
         self.toolbar.lazy_init()
         self.viewport.lazy_init()
 
     def show(self):
```

### Comparing `compas_viewer-1.1.3/src/compas_viewer/ui/viewport.py` & `compas_viewer-1.1.4/src/compas_viewer/ui/viewport.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 from PySide6 import QtCore
 from PySide6 import QtWidgets
 
 from compas_viewer.base import Base
+from compas_viewer.components.treeform import Treeform
 
 
 class SideBarRight(Base):
     def __init__(self) -> None:
         super().__init__()
         self.side_right_widget = None
-        self.default_widgets: list[str] = ["TreeForm"]
-        self.custom_widgets: list[str] = []  # TODO(pitsai): self.viewer.config.ui.sidebar.items
-        self.widget_list: list = self.default_widgets + self.custom_widgets
 
     def setup_sidebar_right(self) -> None:
         self.side_right_widget = QtWidgets.QSplitter(QtCore.Qt.Orientation.Vertical)
         self.side_right_widget.setChildrenCollapsible(True)
-        self.viewer.ui.components_manager.add_widgets(self.widget_list)
-        self.side_right_widget = self.viewer.ui.components_manager.setup_widgets(self.side_right_widget)
+        self.side_right_widget.addWidget(Treeform(self.viewer.scene, {"Name": (lambda o: o.name), "Object": (lambda o: o)}))
+        self.side_right_widget.setSizes([800, 200])
         self.side_right_widget.setHidden(not self.viewer.config.ui.sidebar.show)
 
 
 class ViewPort(Base):
     def __init__(self):
         self.sidebar_right = SideBarRight()
 
     def lazy_init(self) -> None:
         self.sidebar_right.setup_sidebar_right()
 
         self.viewport_widget = QtWidgets.QSplitter()
         self.viewport_widget.addWidget(self.viewer.renderer)
         self.viewport_widget.addWidget(self.sidebar_right.side_right_widget)
+        self.viewport_widget.setSizes([800, 200])
         self.viewer.ui.window.centralWidget().layout().addWidget(self.viewport_widget)
```

### Comparing `compas_viewer-1.1.3/src/compas_viewer/viewer.py` & `compas_viewer-1.1.4/src/compas_viewer/viewer.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.3/src/compas_viewer.egg-info/PKG-INFO` & `compas_viewer-1.1.4/src/compas_viewer.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compas_viewer
-Version: 1.1.3
+Version: 1.1.4
 Summary: Standalone viewer for COMPAS 2 based on PyOpenGL and PyQt6.
 Author-email: tom van mele <tom.v.mele@gmail.com>, Li Chen <li.chen@arch.ethz.ch>, Zac Zhuo Zhang <zhuo.zhang@arch.ethz.ch>
 License: MIT License
         
         COMPAS Association
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `compas_viewer-1.1.3/src/compas_viewer.egg-info/SOURCES.txt` & `compas_viewer-1.1.4/src/compas_viewer.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,17 @@
 src/compas_viewer/actions/delete_selected.py
 src/compas_viewer/actions/info.py
 src/compas_viewer/actions/io.py
 src/compas_viewer/actions/select_all.py
 src/compas_viewer/actions/viewmode.py
 src/compas_viewer/actions/zoom_selected.py
 src/compas_viewer/components/__init__.py
-src/compas_viewer/components/button_factory.py
-src/compas_viewer/components/component_manager.py
-src/compas_viewer/components/setting_components.py
-src/compas_viewer/components/treeform_components.py
+src/compas_viewer/components/button.py
+src/compas_viewer/components/double_edit.py
+src/compas_viewer/components/treeform.py
 src/compas_viewer/components/widget_tools.py
 src/compas_viewer/components/renderer/__init__.py
 src/compas_viewer/components/renderer/camera.py
 src/compas_viewer/components/renderer/renderer.py
 src/compas_viewer/components/renderer/selector.py
 src/compas_viewer/components/renderer/shaders/__init__.py
 src/compas_viewer/components/renderer/shaders/arrow.frag
```

