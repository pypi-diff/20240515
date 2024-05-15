# Comparing `tmp/pasta_eln-2.5.2b2.tar.gz` & `tmp/pasta_eln-2.5.3b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pasta_eln-2.5.2b2.tar", last modified: Wed Apr 17 12:19:47 2024, max compression
+gzip compressed data, was "pasta_eln-2.5.3b1.tar", last modified: Wed May 15 20:21:23 2024, max compression
```

## Comparing `pasta_eln-2.5.2b2.tar` & `pasta_eln-2.5.3b1.tar`

### file list

```diff
@@ -1,179 +1,191 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:47.897585 pasta_eln-2.5.2b2/
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-17 12:19:47.897585 pasta_eln-2.5.2b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/README_PYPI.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:47.865585 pasta_eln-2.5.2b2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:47.865585 pasta_eln-2.5.2b2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:47.873585 pasta_eln-2.5.2b2/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)  2003429 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/source/_static/Data_Hierarchy_Editor_Manual.odp
--rw-r--r--   0 runner    (1001) docker     (127)  1695262 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/source/_static/Data_Hierarchy_Editor_Manual.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/source/_static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   225801 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/source/_static/data_hierarchy_editor.png
--rw-r--r--   0 runner    (1001) docker     (127)   985134 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/source/_static/metadata_group_combobox.png
--rw-r--r--   0 runner    (1001) docker     (127)    11481 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/source/_static/pasta_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   100504 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/source/_static/pyside.png
--rw-r--r--   0 runner    (1001) docker     (127)   846253 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/source/_static/types_combo_box.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:47.861585 pasta_eln-2.5.2b2/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:47.873585 pasta_eln-2.5.2b2/docs/source/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/source/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/source/data_hierarchy_configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/source/dodonts.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9683 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/source/extractors.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/source/faqs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/source/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11238 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/source/motivation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/docs/source/userstory.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:47.877585 pasta_eln-2.5.2b2/pasta_eln/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:47.881585 pasta_eln-2.5.2b2/pasta_eln/Extractors/
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/Extractors/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/Extractors/extractor_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/Extractors/extractor_jpeg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/Extractors/extractor_jpg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/Extractors/extractor_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/Extractors/extractor_md.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/Extractors/extractor_png.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/Extractors/extractor_py.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:47.881585 pasta_eln-2.5.2b2/pasta_eln/GUI/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/_contextMenu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/body.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/configAuthors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/configGUI.py
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/configSetupLinux.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7874 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/configSetupWindows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:47.885585 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/attachments_tableview_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/create_type_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/create_type_dialog_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/create_type_dialog_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)    23214 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    21471 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    21656 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/delete_column_delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/document_null_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/generic_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/iri_column_delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/key_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/lookup_iri_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/mandatory_column_delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/metadata_tableview_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/reorder_column_delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7616 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/tableview_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/terminology_lookup_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/terminology_lookup_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    19014 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/utility_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:47.889585 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/completed_upload_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/completed_upload_task.ui
--rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/completed_uploads.py
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/completed_uploads_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/completed_uploads_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/config_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/config_dialog_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8740 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/config_dialog_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)     7415 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/controlled_vocab_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/dialog_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)    10081 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/edit_metadata_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5920 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/edit_metadata_dialog_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/edit_metadata_dialog_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/main_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/main_dialog_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9608 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/main_dialog_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/primitive_compound_controlled_frame_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/primitive_compound_controlled_frame_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)    21062 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/primitive_compound_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/project_item_frame_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/project_item_frame_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)     6550 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/upload_config_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/upload_config_dialog_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/upload_config_dialog_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/upload_widget_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/upload_widget_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/details.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/docTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    30419 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/form.py
--rw-r--r--   0 runner    (1001) docker     (127)    19027 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/projectGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)    10059 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/projectLeafRenderer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10674 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/projectTreeView.py
--rw-r--r--   0 runner    (1001) docker     (127)     9617 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/sidebar.py
--rw-r--r--   0 runner    (1001) docker     (127)    19486 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/GUI/tableHeader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:47.861585 pasta_eln-2.5.2b2/pasta_eln/Resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:47.893585 pasta_eln-2.5.2b2/pasta_eln/Resources/ExampleMeasurements/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/Resources/ExampleMeasurements/simple.csv
--rw-r--r--   0 runner    (1001) docker     (127)     9450 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/Resources/ExampleMeasurements/simple.png
--rw-r--r--   0 runner    (1001) docker     (127)     8417 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/Resources/ExampleMeasurements/story.odt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:47.893585 pasta_eln-2.5.2b2/pasta_eln/Resources/Icons/
--rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/Resources/Icons/favicon64.ico
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/Resources/Icons/favicon64.png
--rw-r--r--   0 runner    (1001) docker     (127)    20226 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/Resources/Icons/ols.png
--rw-r--r--   0 runner    (1001) docker     (127)    17206 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/Resources/Icons/tib.png
--rw-r--r--   0 runner    (1001) docker     (127)     8673 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/Resources/Icons/wikidata.png
--rw-r--r--   0 runner    (1001) docker     (127)    17310 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/Resources/Icons/wikipedia.png
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35665 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/backend.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14107 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    43862 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:47.897585 pasta_eln-2.5.2b2/pasta_eln/dataverse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/dataverse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12850 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/dataverse/base_database_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/dataverse/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    31059 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/dataverse/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/dataverse/config_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/dataverse/config_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/dataverse/data_upload_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/dataverse/database_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/dataverse/database_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    49819 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/dataverse/dataset-create-new-all-default-fields.json
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/dataverse/generic_task_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/dataverse/incorrect_parameter_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     8623 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/dataverse/project_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/dataverse/task_thread_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)    10671 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/dataverse/upload_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6157 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/dataverse/upload_queue_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/dataverse/upload_status_values.py
--rw-r--r--   0 runner    (1001) docker     (127)    21590 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/dataverse/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    29212 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/fixedStringsJson.py
--rw-r--r--   0 runner    (1001) docker     (127)    11124 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/guiCommunicate.py
--rw-r--r--   0 runner    (1001) docker     (127)    13065 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/guiStyle.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8622 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/handleDictionaries.py
--rw-r--r--   0 runner    (1001) docker     (127)    23440 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/inputOutput.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22498 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/installationTools.py
--rw-r--r--   0 runner    (1001) docker     (127)    10811 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/miscTools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/mixin_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/printer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23753 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/serverActions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:47.897585 pasta_eln-2.5.2b2/pasta_eln/webclient/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/webclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pasta_eln/webclient/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:47.897585 pasta_eln-2.5.2b2/pasta_eln.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-17 12:19:47.000000 pasta_eln-2.5.2b2/pasta_eln.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-04-17 12:19:47.000000 pasta_eln-2.5.2b2/pasta_eln.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 12:19:47.000000 pasta_eln-2.5.2b2/pasta_eln.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-17 12:19:47.000000 pasta_eln-2.5.2b2/pasta_eln.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-17 12:19:47.000000 pasta_eln-2.5.2b2/pasta_eln.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-17 12:19:47.000000 pasta_eln-2.5.2b2/pasta_eln.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-17 12:19:47.897585 pasta_eln-2.5.2b2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-04-17 12:19:47.000000 pasta_eln-2.5.2b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:19:47.897585 pasta_eln-2.5.2b2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7792 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/tests/test_01_3Projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/tests/test_02_3Projects_ExportImport.py
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/tests/test_50_importOthers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-04-17 12:19:45.000000 pasta_eln-2.5.2b2/tests/test_99_3Projects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:21:23.646142 pasta_eln-2.5.3b1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-15 20:21:23.646142 pasta_eln-2.5.3b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/README_PYPI.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:21:23.610141 pasta_eln-2.5.3b1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:21:23.614142 pasta_eln-2.5.3b1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:21:23.618142 pasta_eln-2.5.3b1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)  2003429 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/docs/source/_static/Data_Hierarchy_Editor_Manual.odp
+-rw-r--r--   0 runner    (1001) docker     (127)  1695262 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/docs/source/_static/Data_Hierarchy_Editor_Manual.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/docs/source/_static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   225801 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/docs/source/_static/data_hierarchy_editor.png
+-rw-r--r--   0 runner    (1001) docker     (127)   985134 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/docs/source/_static/metadata_group_combobox.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11481 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/docs/source/_static/pasta_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   100504 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/docs/source/_static/pyside.png
+-rw-r--r--   0 runner    (1001) docker     (127)   846253 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/docs/source/_static/types_combo_box.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:21:23.606141 pasta_eln-2.5.3b1/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:21:23.622141 pasta_eln-2.5.3b1/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/docs/source/data_hierarchy_configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/docs/source/dodonts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9683 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/docs/source/extractors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/docs/source/faqs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/docs/source/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11238 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/docs/source/motivation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/docs/source/userstory.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:21:23.622141 pasta_eln-2.5.3b1/pasta_eln/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:21:23.626142 pasta_eln-2.5.3b1/pasta_eln/Extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/Extractors/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/Extractors/extractor_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/Extractors/extractor_jpeg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/Extractors/extractor_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/Extractors/extractor_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/Extractors/extractor_md.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/Extractors/extractor_png.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/Extractors/extractor_py.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:21:23.630142 pasta_eln-2.5.3b1/pasta_eln/GUI/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/_contextMenu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6766 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/configAuthors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/configGUI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/configSetupLinux.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7874 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/configSetupWindows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:21:23.634142 pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/attachments_tableview_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/create_type_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/create_type_dialog_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/create_type_dialog_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    23214 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21471 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21656 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/delete_column_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/document_null_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/generic_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/iri_column_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/key_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/lookup_iri_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/mandatory_column_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/metadata_tableview_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/reorder_column_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7616 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/tableview_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19014 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/utility_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:21:23.638142 pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/completed_upload_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/completed_upload_task.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/completed_uploads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/completed_uploads_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/completed_uploads_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/config_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7759 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/config_dialog_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/config_dialog_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     7415 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/controlled_vocab_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/dialog_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11228 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/edit_metadata_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/edit_metadata_dialog_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/edit_metadata_dialog_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/edit_metadata_summary_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/edit_metadata_summary_dialog_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/edit_metadata_summary_dialog_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    17726 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/main_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9695 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/main_dialog_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9615 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/main_dialog_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/primitive_compound_controlled_frame_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/primitive_compound_controlled_frame_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    21062 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/primitive_compound_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/project_item_frame_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/project_item_frame_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/upload_config_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/upload_config_dialog_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/upload_config_dialog_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/upload_widget_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/upload_widget_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    11275 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/docTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30765 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19027 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11366 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/projectGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10078 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/projectLeafRenderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10674 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/projectTreeView.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9617 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/sidebar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19510 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/GUI/tableHeader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:21:23.610141 pasta_eln-2.5.3b1/pasta_eln/Resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:21:23.638142 pasta_eln-2.5.3b1/pasta_eln/Resources/ExampleMeasurements/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/Resources/ExampleMeasurements/simple.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9450 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/Resources/ExampleMeasurements/simple.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8417 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/Resources/ExampleMeasurements/story.odt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:21:23.638142 pasta_eln-2.5.3b1/pasta_eln/Resources/Icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/Resources/Icons/favicon64.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/Resources/Icons/favicon64.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20226 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/Resources/Icons/ols.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17206 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/Resources/Icons/tib.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8673 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/Resources/Icons/wikidata.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17310 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/Resources/Icons/wikipedia.png
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35665 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/backend.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14304 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43862 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:21:23.642142 pasta_eln-2.5.3b1/pasta_eln/dataverse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/dataverse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12952 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/dataverse/base_database_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/dataverse/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33985 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/dataverse/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/dataverse/config_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/dataverse/config_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16697 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/dataverse/data_upload_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14524 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/dataverse/database_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/dataverse/database_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49819 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/dataverse/dataset-create-new-all-default-fields.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/dataverse/generic_task_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/dataverse/incorrect_parameter_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/dataverse/progress_updater_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8623 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/dataverse/project_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/dataverse/task_thread_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/dataverse/upload_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7778 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/dataverse/upload_queue_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/dataverse/upload_status_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28351 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/dataverse/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29212 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/fixedStringsJson.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12622 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/guiCommunicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13065 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/guiStyle.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8622 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/handleDictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24115 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/inputOutput.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22576 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/installationTools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:21:23.642142 pasta_eln-2.5.3b1/pasta_eln/minisign/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/minisign/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/minisign/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/minisign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/minisign/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/minisign/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15791 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/minisign/minisign.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/minisign/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13888 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/miscTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/mixin_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/printer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23817 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/serverActions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:21:23.642142 pasta_eln-2.5.3b1/pasta_eln/webclient/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/webclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pasta_eln/webclient/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:21:23.642142 pasta_eln-2.5.3b1/pasta_eln.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-15 20:21:23.000000 pasta_eln-2.5.3b1/pasta_eln.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6575 2024-05-15 20:21:23.000000 pasta_eln-2.5.3b1/pasta_eln.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 20:21:23.000000 pasta_eln-2.5.3b1/pasta_eln.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-15 20:21:23.000000 pasta_eln-2.5.3b1/pasta_eln.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-15 20:21:23.000000 pasta_eln-2.5.3b1/pasta_eln.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 20:21:23.000000 pasta_eln-2.5.3b1/pasta_eln.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-15 20:21:23.646142 pasta_eln-2.5.3b1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-05-15 20:21:23.000000 pasta_eln-2.5.3b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:21:23.642142 pasta_eln-2.5.3b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7792 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/tests/test_01_3Projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/tests/test_02_3Projects_ExportImport1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8540 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/tests/test_03_3Projects_ExportImport3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-05-15 20:21:21.000000 pasta_eln-2.5.3b1/tests/test_99_3Projects.py
```

### Comparing `pasta_eln-2.5.2b2/LICENSE` & `pasta_eln-2.5.3b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/PKG-INFO` & `pasta_eln-2.5.3b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasta_eln
-Version: 2.5.2b2
+Version: 2.5.3b1
 Summary: The favorite ELN for experimental scientists
 Home-page: https://pasta-eln.github.io/
 Author: The PASTA-ELN Team and Steffen Brinckmann
 Author-email: sbrinckm@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pasta_eln-2.5.2b2/README.md` & `pasta_eln-2.5.3b1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 
 > :warning: **Users: all documentation can be found at [Github-pages](https://pasta-eln.github.io/pasta-eln/)**
 >
 > **This page / area is for developers and contains some helpful information for them**
 
 ---
 
-## Developers: notes on windows installation
+## Developers: Windows
 
 ### How to start Pasta ELN
 - Anaconda
   - python -m pasta_eln.gui
   - DOES NOT WORK "pastaELN"
 
-### Installation location windows:
+### Installation location:
 - Default installation
   - C:\Users\...\AppData\Local\Programs\Python\Python311\Scripts
   - C:\Users\...\AppData\Local\Programs\Python\Python311\Lib\site-packages\pasta_eln
 - Anaconda
   - C:\Users\...\anaconda3\envs\...\Scripts>
   - C:\Users\...\anaconda3\envs\...\Lib\site-packages\pasta_eln
 
@@ -40,30 +40,39 @@
 - remove shortcut on Windows desktop
 - restart Windows
 - **python -m pasta_eln.gui**
 - go through steps and wait for restart
 - after restart go to System->Configuration (ctrl-0) ->Setup-> start again
   - or have a separate button for that
 
+### Create an installer using pyInstaller
+- Anacoda -> new environment and install "pip install pyinstaller" and dependencies
+- In terminal
+  - cd Documents\PastaELN_src: all files in pasta-eln
+  - pyinstaller pastaELN.py -F
+- File is in /dist/ folder
+
+
 ---
 
-## Developers: notes on linux installation
+## Developers: Linux
 ### Installation location:
 - Default
   - /usr/local/lib/python3.10/dist-packages/pasta_eln
 
-### Restart installation on linux / ubuntu
+### Restart installation
 ``` bash
 rm .pastaELN.json pastaELN.log
 rm -rf pastaELN/PastasExampleProject pastaELN/StandardOperatingProcedures
 sudo snap stop couchdb
 sudo snap remove couchdb
 ```
 
 ---
+
 ## Test couchDB running
 - CouchDB at HTTP! [http://127.0.0.1:5984/_utils/#login](http://127.0.0.1:5984/_utils/#login)
 - curl -f http://127.0.0.1:5984/
 - curl -X POST -H "Content-Type: application/json; charset=utf-8" -d '{"name": "*+*", "password": "*+*"}' http://127.0.0.1:5984/_session
 
 
 ## Notes on all systems
@@ -125,27 +134,49 @@
 doc = backend.db.getDoc("m-3a43570c4fd84b1ab81a8863ae058fb0")
 dialog = Form(comm, doc)
 dialog.show()
 sys.exit(app.exec())
 ```
 and execute "python -m pasta_eln.test"
 
-#### Profiling
+---
+
+### Profiling
 Begin...
+
       from cProfile import Profile
       from pstats import SortKey, Stats
       with Profile() as profile:
 
 End...
-      (Stats(profile).strip_dirs().sort_stats(SortKey.CUMULATIVE).print_stats()) #end cProfile
 
-#### Debugging on a conventional install: linux
+      (Stats(profile).strip_dirs().sort_stats(SortKey.CUMULATIVE).print_stats(100)) #end cProfile
+
+For example: to profile the start of the program
+
+      def startMain() -> None:
+        """
+        Main function to start GUI. Extra function is required to allow starting in module fashion
+        """
+        from cProfile import Profile
+        from pstats import SortKey, Stats
+        with Profile() as profile:
+          app, window = mainGUI()
+          window.show()
+        (Stats(profile).strip_dirs().sort_stats(SortKey.CUMULATIVE).print_stats(100)) #end cProfile
+        # if app:
+        #   app.exec()
+
+
+### Debugging on a conventional install: linux
 - 'sudo apt install python3-pudb' (not pip install)
 - create small 'temp.py' into any folder, with this content
   from pasta_eln.gui import startMain
   startMain()
 - start with 'pudb3 temp.py'
 
+### Running pytests (3.12)
+- python3 -m tests.test_01_3Projects
 
-#### General notes
+### General notes
 - Find qt-awesome icons: qta-browser
-- print works great in frondend and backend
+- print works great in frontend and backend
```

### Comparing `pasta_eln-2.5.2b2/README_PYPI.md` & `pasta_eln-2.5.3b1/README_PYPI.md`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/docs/Makefile` & `pasta_eln-2.5.3b1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/docs/README.md` & `pasta_eln-2.5.3b1/docs/README.md`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/docs/source/_static/Data_Hierarchy_Editor_Manual.odp` & `pasta_eln-2.5.3b1/docs/source/_static/Data_Hierarchy_Editor_Manual.odp`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/docs/source/_static/Data_Hierarchy_Editor_Manual.pdf` & `pasta_eln-2.5.3b1/docs/source/_static/Data_Hierarchy_Editor_Manual.pdf`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/docs/source/_static/data_hierarchy_editor.png` & `pasta_eln-2.5.3b1/docs/source/_static/data_hierarchy_editor.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/docs/source/_static/metadata_group_combobox.png` & `pasta_eln-2.5.3b1/docs/source/_static/metadata_group_combobox.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/docs/source/_static/pasta_logo.svg` & `pasta_eln-2.5.3b1/docs/source/_static/pasta_logo.svg`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/docs/source/_static/pyside.png` & `pasta_eln-2.5.3b1/docs/source/_static/pyside.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/docs/source/_static/types_combo_box.png` & `pasta_eln-2.5.3b1/docs/source/_static/types_combo_box.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/docs/source/conf.py` & `pasta_eln-2.5.3b1/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 project = u'PASTA-ELN'
 copyright = u'2022-{}, PASTA-ELN team'.format(datetime.datetime.now().year)
 author = u'PASTA-ELN team'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
-version = "2.5.2b1"
+version = "2.5.2"
 release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
```

### Comparing `pasta_eln-2.5.2b2/docs/source/data_hierarchy_configuration.rst` & `pasta_eln-2.5.3b1/docs/source/data_hierarchy_configuration.rst`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/docs/source/dodonts.rst` & `pasta_eln-2.5.3b1/docs/source/dodonts.rst`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/docs/source/extractors.rst` & `pasta_eln-2.5.3b1/docs/source/extractors.rst`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/docs/source/faqs.rst` & `pasta_eln-2.5.3b1/docs/source/faqs.rst`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/docs/source/index.rst` & `pasta_eln-2.5.3b1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/docs/source/install.rst` & `pasta_eln-2.5.3b1/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/docs/source/motivation.rst` & `pasta_eln-2.5.3b1/docs/source/motivation.rst`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/docs/source/userstory.rst` & `pasta_eln-2.5.3b1/docs/source/userstory.rst`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/Extractors/extractor_csv.py` & `pasta_eln-2.5.3b1/pasta_eln/Extractors/extractor_csv.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/Extractors/extractor_jpeg.py` & `pasta_eln-2.5.3b1/pasta_eln/Extractors/extractor_jpeg.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/Extractors/extractor_jpg.py` & `pasta_eln-2.5.3b1/pasta_eln/Extractors/extractor_jpg.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/Extractors/extractor_json.py` & `pasta_eln-2.5.3b1/pasta_eln/Extractors/extractor_json.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 """extract data from vendor
 - javascript object notion
 """
 import json
+import os
 
 def use(filePath, recipe='', saveFileName=None):
   """
   Args:
     filePath (Path): full path file name
     recipe (string): supplied to guide recipes
                      recipe is / separated hierarchical elements parent->child
     saveFileName (string): if given, save the image to this file-name
 
   Returns:
     dict: containing image, metaVendor, metaUser, recipe
   """
   # Extractor for fancy instrument
   content = ''
-  with open(filePath,'r', encoding='utf-8') as jsonFile:
-    jsonContent = jsonFile.read()
-    content = json.loads(jsonContent)
-    if not isinstance(content, dict):
-      content= {'content': json.loads(jsonContent)}
+  fileSize = os.stat(filePath).st_size / (1024*1024)  #in MB
+  if fileSize<0.3:
+    with open(filePath,'r', encoding='utf-8') as jsonFile:
+      jsonContent = jsonFile.read()
+      content = json.loads(jsonContent)
+      if not isinstance(content, dict):
+        content= {'content': json.loads(jsonContent)}
+    content= f'```json\n{json.dumps(content, indent=2)}\n```'
+  else:
+    content= 'Too large json file'
   recipe = 'procedure/json'
-  content= f'```json\n{json.dumps(content, indent=2)}\n```'
 
   # return everything
   return {'content':content, 'recipe':recipe, 'metaVendor':{}, 'metaUser':{}}
 
   #other datatypes follow here
   #...
   #final return if nothing successful
```

### Comparing `pasta_eln-2.5.2b2/pasta_eln/Extractors/extractor_md.py` & `pasta_eln-2.5.3b1/pasta_eln/Extractors/extractor_md.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/Extractors/extractor_png.py` & `pasta_eln-2.5.3b1/pasta_eln/Extractors/extractor_png.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/Extractors/extractor_py.py` & `pasta_eln-2.5.3b1/pasta_eln/Extractors/extractor_py.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/_contextMenu.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/_contextMenu.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/body.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/body.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/config.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/config.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/configAuthors.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/configAuthors.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,22 +83,20 @@
   def changedID(self) -> None:
     """
     Autofill based on orcid and rorid
     """
     sender = self.sender().accessibleName()
     if sender == 'rorid':
       if re.match(r'^\w{9}$', self.userRorid.text().strip() ) is not None:
-        reply = requests.get(
-            f'https://api.ror.org/organizations/{self.userRorid.text().strip()}')
+        reply = requests.get(f'https://api.ror.org/organizations/{self.userRorid.text().strip()}', timeout=10)
         self.userOrg.setText(reply.json()['name'])
         self.orgaCB.setItemText(self.orgaCB.currentIndex(), reply.json()['name'])
     elif sender == 'orcid':
       if re.match(r'^\w{4}-\w{4}-\w{4}-\w{4}$', self.userOrcid.text().strip() ) is not None:
-        reply = requests.get(
-            f'https://pub.orcid.org/v3.0/{self.userOrcid.text().strip()}')
+        reply = requests.get(f'https://pub.orcid.org/v3.0/{self.userOrcid.text().strip()}', timeout=10)
         text = reply.content.decode()
         first = text.split('<personal-details:given-names>')[1].split('</personal-details:given-names>')[0]
         last = text.split('<personal-details:family-name>')[1].split('</personal-details:family-name>')[0]
         self.userFirst.setText(first)
         self.userLast.setText(last)
     elif sender == 'organization':
       self.orgaCB.setItemText(self.orgaCB.currentIndex(), self.userOrg.text())
```

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/configGUI.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/configGUI.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/configSetupLinux.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/configSetupLinux.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/configSetupWindows.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/configSetupWindows.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/attachments_tableview_data_model.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/attachments_tableview_data_model.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/constants.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/constants.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/create_type_dialog.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/create_type_dialog.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/create_type_dialog_base.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/create_type_dialog_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/create_type_dialog_base.ui` & `pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/create_type_dialog_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog_base.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog_base.ui` & `pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/delete_column_delegate.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/delete_column_delegate.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/document_null_exception.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/document_null_exception.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/generic_exception.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/generic_exception.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/iri_column_delegate.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/iri_column_delegate.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/key_not_found_exception.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/key_not_found_exception.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/lookup_iri_action.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/lookup_iri_action.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/mandatory_column_delegate.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/mandatory_column_delegate.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/metadata_tableview_data_model.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/metadata_tableview_data_model.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/reorder_column_delegate.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/reorder_column_delegate.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/tableview_data_model.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/tableview_data_model.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/terminology_lookup_config.json` & `pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_config.json`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog_base.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog_base.ui` & `pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/terminology_lookup_service.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_service.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/data_hierarchy/utility_functions.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/data_hierarchy/utility_functions.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/completed_upload_task.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/completed_upload_task.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/completed_upload_task.ui` & `pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/completed_upload_task.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/completed_uploads.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/completed_uploads.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/completed_uploads_base.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/completed_uploads_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/completed_uploads_base.ui` & `pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/completed_uploads_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/config_dialog.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/config_dialog.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,21 +10,24 @@
 
 import logging
 import webbrowser
 from asyncio import get_event_loop
 from typing import Any
 
 from PySide6 import QtCore, QtWidgets
+from PySide6.QtCore import QRegularExpression
+from PySide6.QtGui import QRegularExpressionValidator
 from PySide6.QtWidgets import QDialog, QMessageBox
 
 from pasta_eln.GUI.dataverse.config_dialog_base import Ui_ConfigDialogBase
 from pasta_eln.dataverse.client import DataverseClient
+from pasta_eln.dataverse.config_error import ConfigError
 from pasta_eln.dataverse.config_model import ConfigModel
 from pasta_eln.dataverse.database_api import DatabaseAPI
-from pasta_eln.dataverse.utils import check_login_credentials, decrypt_data, encrypt_data, get_encrypt_key
+from pasta_eln.dataverse.utils import check_login_credentials, log_and_create_error
 
 
 class ConfigDialog(Ui_ConfigDialogBase):
   """
   Creates a new instance of the ConfigDialog class.
 
   Explanation:
@@ -79,70 +82,40 @@
 
     Explanation:
         This method initializes the ConfigDialog class.
 
         It sets up the logger and creates an instance of QDialog.
 
     """
-    self.encrypt_key: bytes | None = None
     self.logger = logging.getLogger(f"{__name__}.{self.__class__.__name__}")
     self.instance: QDialog = QDialog()
     super().setupUi(self.instance)
     self.db_api = DatabaseAPI()
-    self.config_model: ConfigModel = self.db_api.get_model(self.db_api.config_doc_id,
-                                                           ConfigModel)  # type: ignore[assignment]
+    self.config_model = self.db_api.get_config_model() or ConfigModel()
+    if self.config_model.id is None:
+      raise log_and_create_error(self.logger, ConfigError, "Config not found, Corrupt installation!")
     self.config_model.dataverse_login_info = self.config_model.dataverse_login_info or {}
-    self.decrypt_api_token()
+    self.dataverseServerLineEdit.setValidator(QRegularExpressionValidator(QRegularExpression("\\S*")))
 
     # Initialize UI elements
     self.dataverseServerLineEdit.setText(self.config_model.dataverse_login_info.get("server_url", ""))
     self.apiTokenLineEdit.setText(self.config_model.dataverse_login_info.get("api_token", ""))
     self.dataverseListComboBox.setCurrentText(self.config_model.dataverse_login_info.get("dataverse_id", ""))
     self.dataverseLineEdit.setText(self.config_model.dataverse_login_info.get("dataverse_id", ""))
 
     # Setup slots
     self.dataverseServerLineEdit.textChanged[str].connect(self.update_dataverse_server)
     self.apiTokenLineEdit.textChanged[str].connect(self.update_api_token)
     self.dataverseLineEdit.textChanged[str].connect(self.update_dataverse_id)
     self.dataverseListComboBox.currentTextChanged.connect(self.update_dataverse_line_edit)
     self.buttonBox.button(QtWidgets.QDialogButtonBox.Save).clicked.connect(self.save_config)
-    self.apiTokenVerifyPushButton.clicked.connect(self.verify_server_url_and_api_token)
-    self.dataverseLoadPushButton.clicked.connect(self.load_dataverse_list)
+    self.dataverseVerifyLoadPushButton.clicked.connect(self.verify_and_load_dataverse_list)
     self.apiTokenHelpPushButton.clicked.connect(
       lambda: webbrowser.open("https://data.fz-juelich.de/guide/api/auth.html"))
 
-    # Load dataverse list
-    if self.dataverseServerLineEdit.text() and self.apiTokenLineEdit.text():
-      self.dataverseLoadPushButton.click()
-
-  def decrypt_api_token(self) -> None:
-    """
-    Decrypts the API token using the encryption key.
-
-    Explanation:
-        This method decrypts the API token using the encryption key.
-        If the encryption key is not found, it removes the API token and dataverse ID from the configuration.
-
-    Args:
-        self: The instance of the class.
-    """
-    key_exists, self.encrypt_key = get_encrypt_key(self.logger)
-    if key_exists:
-      self.config_model.dataverse_login_info["api_token"] = decrypt_data(self.logger,  # type: ignore[index]
-                                                                         self.encrypt_key,
-                                                                         self.config_model.dataverse_login_info[
-                                                                           # type: ignore[index]
-                                                                           "api_token"])
-    else:
-      self.logger.warning(
-        "No encryption key found. Hence if any API key exists, it will be removed and the user needs to re-enter it.")
-      self.config_model.dataverse_login_info["api_token"] = None  # type: ignore[index]
-      self.config_model.dataverse_login_info["dataverse_id"] = None  # type: ignore[index]
-      self.save_config()
-
   def update_dataverse_server(self, new_value: str) -> None:
     """
     Updates the server URL in the dataverse login info.
 
     Explanation:
         This method updates the server URL in the dataverse login info with the provided new value.
 
@@ -189,54 +162,55 @@
     """
     Saves the configuration in database.
 
     Explanation:
         This method saves the configuration by encrypting the API token.
     """
     self.logger.info("Saving config..")
-    self.config_model.dataverse_login_info["api_token"] = encrypt_data(  # type:ignore[index]
-      self.logger,
-      self.encrypt_key,
-      self.config_model.dataverse_login_info[
-        # type: ignore[index]
-        "api_token"])
-    self.db_api.update_model_document(self.config_model)
+    self.db_api.save_config_model(self.config_model)
 
-  def verify_server_url_and_api_token(self) -> None:
+  def verify_server_url_and_api_token(self) -> bool:
     """
     Verifies the server URL and API token.
 
     Explanation:
         This method verifies the server URL and API token by checking if they are both provided.
         If they are not provided, it shows a warning message.
+
+    Returns:
+        bool: True if the server URL and API token are valid, False otherwise.
     """
     self.logger.info("Verifying server URL and API token..")
     server_url = self.dataverseServerLineEdit.text()
     api_token = self.apiTokenLineEdit.text()
     if not (server_url and api_token):
       QMessageBox.warning(self.instance, "Error", "Please enter both server URL and API token")
-      return
+      return False
     success, message = check_login_credentials(self.logger, api_token, server_url)
     if success:
       QMessageBox.information(self.instance, "Credentials Valid", message)
+      return True
     else:
       QMessageBox.warning(self.instance, "Credentials Invalid", message)
+      return False
 
-  def load_dataverse_list(self) -> None:
+  def verify_and_load_dataverse_list(self) -> None:
     """
     Loads the dataverse list.
 
     Explanation:
         This method loads the dataverse list by making a request to the server and populating the dataverse list combo box with the retrieved dataverses.
     """
     self.logger.info("Loading dataverse list..")
     saved_id = self.config_model.dataverse_login_info.get("dataverse_id", "")  # type: ignore[union-attr]
     self.dataverseListComboBox.clear()
     server_url = self.dataverseServerLineEdit.text()
     api_token = self.apiTokenLineEdit.text()
+    if not self.verify_server_url_and_api_token():
+      return
     if not (server_url and api_token):
       QMessageBox.warning(self.instance, "Error", "Please enter both server URL and API token")
       return
     dataverse_client = DataverseClient(server_url, api_token)
     event_loop = get_event_loop()
     if dataverses := event_loop.run_until_complete(dataverse_client.get_dataverse_list()):
       if isinstance(dataverses, list) and isinstance(dataverses[0], dict):
@@ -257,14 +231,17 @@
     """
     Shows the instance.
 
     Explanation:
         This method shows the instance by calling its show method.
     """
     self.instance.show()
+    # Load dataverse list
+    if self.dataverseServerLineEdit.text() and self.apiTokenLineEdit.text():
+      self.dataverseVerifyLoadPushButton.click()
 
 
 if __name__ == "__main__":
   import sys
 
   app = QtWidgets.QApplication(sys.argv)
```

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/config_dialog_base.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/config_dialog_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     self.dataverseServerLabel.setMinimumSize(QtCore.QSize(200, 0))
     self.dataverseServerLabel.setObjectName("dataverseServerLabel")
     self.serverHorizontalLayout.addWidget(self.dataverseServerLabel)
     self.dataverseServerLineEdit = QtWidgets.QLineEdit(parent=ConfigDialogBase)
     self.dataverseServerLineEdit.setClearButtonEnabled(True)
     self.dataverseServerLineEdit.setObjectName("dataverseServerLineEdit")
     self.serverHorizontalLayout.addWidget(self.dataverseServerLineEdit)
-    spacerItem = QtWidgets.QSpacerItem(213, 20, QtWidgets.QSizePolicy.Policy.Preferred, QtWidgets.QSizePolicy.Policy.Minimum)
+    spacerItem = QtWidgets.QSpacerItem(155, 20, QtWidgets.QSizePolicy.Policy.Preferred, QtWidgets.QSizePolicy.Policy.Minimum)
     self.serverHorizontalLayout.addItem(spacerItem)
     self.mainVerticalLayout.addLayout(self.serverHorizontalLayout)
     spacerItem1 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Fixed)
     self.mainVerticalLayout.addItem(spacerItem1)
     self.apiTokenHorizontalLayout = QtWidgets.QHBoxLayout()
     self.apiTokenHorizontalLayout.setObjectName("apiTokenHorizontalLayout")
     self.apiTokenLabel = QtWidgets.QLabel(parent=ConfigDialogBase)
@@ -44,20 +44,16 @@
     self.apiTokenLabel.setObjectName("apiTokenLabel")
     self.apiTokenHorizontalLayout.addWidget(self.apiTokenLabel)
     self.apiTokenLineEdit = QtWidgets.QLineEdit(parent=ConfigDialogBase)
     self.apiTokenLineEdit.setEchoMode(QtWidgets.QLineEdit.EchoMode.Password)
     self.apiTokenLineEdit.setClearButtonEnabled(True)
     self.apiTokenLineEdit.setObjectName("apiTokenLineEdit")
     self.apiTokenHorizontalLayout.addWidget(self.apiTokenLineEdit)
-    self.apiTokenVerifyPushButton = QtWidgets.QPushButton(parent=ConfigDialogBase)
-    self.apiTokenVerifyPushButton.setMinimumSize(QtCore.QSize(100, 0))
-    self.apiTokenVerifyPushButton.setObjectName("apiTokenVerifyPushButton")
-    self.apiTokenHorizontalLayout.addWidget(self.apiTokenVerifyPushButton)
     self.apiTokenHelpPushButton = QtWidgets.QPushButton(parent=ConfigDialogBase)
-    self.apiTokenHelpPushButton.setMinimumSize(QtCore.QSize(100, 0))
+    self.apiTokenHelpPushButton.setMinimumSize(QtCore.QSize(150, 0))
     self.apiTokenHelpPushButton.setObjectName("apiTokenHelpPushButton")
     self.apiTokenHorizontalLayout.addWidget(self.apiTokenHelpPushButton)
     self.mainVerticalLayout.addLayout(self.apiTokenHorizontalLayout)
     spacerItem2 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Fixed)
     self.mainVerticalLayout.addItem(spacerItem2)
     self.dataverseListHorizontalLayout = QtWidgets.QHBoxLayout()
     self.dataverseListHorizontalLayout.setObjectName("dataverseListHorizontalLayout")
@@ -74,23 +70,21 @@
     self.dataverseListComboBox.setSizeAdjustPolicy(QtWidgets.QComboBox.SizeAdjustPolicy.AdjustToMinimumContentsLengthWithIcon)
     self.dataverseListComboBox.setObjectName("dataverseListComboBox")
     self.dataverseListHorizontalLayout.addWidget(self.dataverseListComboBox)
     self.dataverseLineEdit = QtWidgets.QLineEdit(parent=ConfigDialogBase)
     self.dataverseLineEdit.setClearButtonEnabled(True)
     self.dataverseLineEdit.setObjectName("dataverseLineEdit")
     self.dataverseListHorizontalLayout.addWidget(self.dataverseLineEdit)
-    self.dataverseLoadPushButton = QtWidgets.QPushButton(parent=ConfigDialogBase)
-    self.dataverseLoadPushButton.setMinimumSize(QtCore.QSize(100, 0))
-    self.dataverseLoadPushButton.setObjectName("dataverseLoadPushButton")
-    self.dataverseListHorizontalLayout.addWidget(self.dataverseLoadPushButton)
-    spacerItem3 = QtWidgets.QSpacerItem(105, 20, QtWidgets.QSizePolicy.Policy.Preferred, QtWidgets.QSizePolicy.Policy.Minimum)
-    self.dataverseListHorizontalLayout.addItem(spacerItem3)
+    self.dataverseVerifyLoadPushButton = QtWidgets.QPushButton(parent=ConfigDialogBase)
+    self.dataverseVerifyLoadPushButton.setMinimumSize(QtCore.QSize(150, 0))
+    self.dataverseVerifyLoadPushButton.setObjectName("dataverseVerifyLoadPushButton")
+    self.dataverseListHorizontalLayout.addWidget(self.dataverseVerifyLoadPushButton)
     self.mainVerticalLayout.addLayout(self.dataverseListHorizontalLayout)
-    spacerItem4 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Fixed)
-    self.mainVerticalLayout.addItem(spacerItem4)
+    spacerItem3 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Fixed)
+    self.mainVerticalLayout.addItem(spacerItem3)
     self.gridLayout.addLayout(self.mainVerticalLayout, 0, 0, 1, 1)
 
     self.retranslateUi(ConfigDialogBase)
     self.buttonBox.accepted.connect(ConfigDialogBase.accept) # type: ignore
     self.buttonBox.rejected.connect(ConfigDialogBase.reject) # type: ignore
     QtCore.QMetaObject.connectSlotsByName(ConfigDialogBase)
 
@@ -99,24 +93,22 @@
     ConfigDialogBase.setWindowTitle(_translate("ConfigDialogBase", "Dataverse configuration"))
     self.dataverseServerLabel.setText(_translate("ConfigDialogBase", "Dataverse URL"))
     self.dataverseServerLineEdit.setToolTip(_translate("ConfigDialogBase", "Enter the dataverse server URL."))
     self.dataverseServerLineEdit.setPlaceholderText(_translate("ConfigDialogBase", "Enter the dataverse server URL, e.g. https://data.fz-juelich.de/"))
     self.apiTokenLabel.setText(_translate("ConfigDialogBase", "API token"))
     self.apiTokenLineEdit.setToolTip(_translate("ConfigDialogBase", "Enter the API token."))
     self.apiTokenLineEdit.setPlaceholderText(_translate("ConfigDialogBase", "Enter the API token, e.g. c6527048-5bdc-48b0-a1d5-ed1b62c4513b"))
-    self.apiTokenVerifyPushButton.setToolTip(_translate("ConfigDialogBase", "Verify if the given dataverse server and api token are reachable."))
-    self.apiTokenVerifyPushButton.setText(_translate("ConfigDialogBase", "Verify"))
     self.apiTokenHelpPushButton.setToolTip(_translate("ConfigDialogBase", "Navigate to the help page for generating dataverse API token."))
     self.apiTokenHelpPushButton.setText(_translate("ConfigDialogBase", "Help"))
     self.dataverseListLabel.setText(_translate("ConfigDialogBase", "Dataverse list"))
     self.dataverseListComboBox.setToolTip(_translate("ConfigDialogBase", "Displays the dataverse list from the server."))
     self.dataverseLineEdit.setToolTip(_translate("ConfigDialogBase", "Displays the ID of the selected dataverse from the list."))
     self.dataverseLineEdit.setPlaceholderText(_translate("ConfigDialogBase", "Selected Dataverse ID"))
-    self.dataverseLoadPushButton.setToolTip(_translate("ConfigDialogBase", "Loads available dataverse list from the server."))
-    self.dataverseLoadPushButton.setText(_translate("ConfigDialogBase", "Load"))
+    self.dataverseVerifyLoadPushButton.setToolTip(_translate("ConfigDialogBase", "Verify API credentials and load available dataverse list from the server."))
+    self.dataverseVerifyLoadPushButton.setText(_translate("ConfigDialogBase", "Verify && Load"))
 
 
 if __name__ == "__main__":
     import sys
     app = QtWidgets.QApplication(sys.argv)
     ConfigDialogBase = QtWidgets.QDialog()
     ui = Ui_ConfigDialogBase()
```

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/config_dialog_base.ui` & `pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/config_dialog_base.ui`

 * *Files 5% similar despite different names*

#### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/config_dialog_base.ui` & `pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/config_dialog_base.ui`

```diff
@@ -51,33 +51,33 @@
                   </property>
                   <property name="clearButtonEnabled">
                     <bool>true</bool>
                   </property>
                 </widget>
               </item>
               <item>
-                <spacer name="horizontalSpacer_3">
+                <spacer name="dataverseUrlHorizontalSpacer">
                   <property name="orientation">
                     <enum>Qt::Horizontal</enum>
                   </property>
                   <property name="sizeType">
                     <enum>QSizePolicy::Preferred</enum>
                   </property>
                   <property name="sizeHint" stdset="0">
                     <size>
-                      <width>213</width>
+                      <width>155</width>
                       <height>20</height>
                     </size>
                   </property>
                 </spacer>
               </item>
             </layout>
           </item>
           <item>
-            <spacer name="verticalSpacer">
+            <spacer name="verticalSpacer_1">
               <property name="orientation">
                 <enum>Qt::Vertical</enum>
               </property>
               <property name="sizeType">
                 <enum>QSizePolicy::Fixed</enum>
               </property>
               <property name="sizeHint" stdset="0">
@@ -116,34 +116,18 @@
                   </property>
                   <property name="clearButtonEnabled">
                     <bool>true</bool>
                   </property>
                 </widget>
               </item>
               <item>
-                <widget class="QPushButton" name="apiTokenVerifyPushButton">
-                  <property name="minimumSize">
-                    <size>
-                      <width>100</width>
-                      <height>0</height>
-                    </size>
-                  </property>
-                  <property name="toolTip">
-                    <string>Verify if the given dataverse server and api token are reachable.</string>
-                  </property>
-                  <property name="text">
-                    <string>Verify</string>
-                  </property>
-                </widget>
-              </item>
-              <item>
                 <widget class="QPushButton" name="apiTokenHelpPushButton">
                   <property name="minimumSize">
                     <size>
-                      <width>100</width>
+                      <width>150</width>
                       <height>0</height>
                     </size>
                   </property>
                   <property name="toolTip">
                     <string>Navigate to the help page for generating dataverse API token.</string>
                   </property>
                   <property name="text">
@@ -210,45 +194,29 @@
                   </property>
                   <property name="clearButtonEnabled">
                     <bool>true</bool>
                   </property>
                 </widget>
               </item>
               <item>
-                <widget class="QPushButton" name="dataverseLoadPushButton">
+                <widget class="QPushButton" name="dataverseVerifyLoadPushButton">
                   <property name="minimumSize">
                     <size>
-                      <width>100</width>
+                      <width>150</width>
                       <height>0</height>
                     </size>
                   </property>
                   <property name="toolTip">
-                    <string>Loads available dataverse list from the server.</string>
+                    <string>Verify API credentials and load available dataverse list from the server.</string>
                   </property>
                   <property name="text">
-                    <string>Load</string>
+                    <string>Verify &amp;&amp; Load</string>
                   </property>
                 </widget>
               </item>
-              <item>
-                <spacer name="dataverserListhorizontalSpacer">
-                  <property name="orientation">
-                    <enum>Qt::Horizontal</enum>
-                  </property>
-                  <property name="sizeType">
-                    <enum>QSizePolicy::Preferred</enum>
-                  </property>
-                  <property name="sizeHint" stdset="0">
-                    <size>
-                      <width>105</width>
-                      <height>20</height>
-                    </size>
-                  </property>
-                </spacer>
-              </item>
             </layout>
           </item>
           <item>
             <spacer name="verticalSpacer_3">
               <property name="orientation">
                 <enum>Qt::Vertical</enum>
               </property>
```

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/controlled_vocab_frame.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/controlled_vocab_frame.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/dialog_extension.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/dialog_extension.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """ Represents QT dialog extension. """
+
 #  PASTA-ELN and all its sub-parts are covered by the MIT license.
 #
 #  Copyright (c) 2024
 #
 #  Author: Jithu Murugan
 #  Filename: dialog_extension.py
 #
@@ -24,15 +25,14 @@
       None
 
   Returns:
       None
   """
   closed = QtCore.Signal()
 
-
   def closeEvent(self, close_event: QCloseEvent) -> None:
     """
     Overrides the close event method.
 
     Explanation:
         This method is called when the close event is triggered.
         It emits a closed signal.
```

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/edit_metadata_dialog.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/edit_metadata_dialog.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 """ Represents the edit metadata dialog. """
 #  PASTA-ELN and all its sub-parts are covered by the MIT license.
 #
 #  Copyright (c) 2024
 #
 #  Author: Jithu Murugan
-#  Filename: dataverse_edit_full_metadata.py
+#  Filename: edit_metadata_dialog.py
 #
 #  You should have received a copy of the license with this file. Please refer the license file for more information.
 
+import copy
 import logging
 from typing import Any
 
 from PySide6 import QtCore, QtWidgets
 from PySide6.QtWidgets import QDialog
 
 from pasta_eln.GUI.dataverse.controlled_vocab_frame import ControlledVocabFrame
 from pasta_eln.GUI.dataverse.edit_metadata_dialog_base import Ui_EditMetadataDialog
+from pasta_eln.GUI.dataverse.edit_metadata_summary_dialog import EditMetadataSummaryDialog
 from pasta_eln.GUI.dataverse.primitive_compound_frame import PrimitiveCompoundFrame
 from pasta_eln.dataverse.config_model import ConfigModel
 from pasta_eln.dataverse.database_api import DatabaseAPI
-from pasta_eln.dataverse.utils import adjust_type_name
+from pasta_eln.dataverse.utils import adjust_type_name, get_formatted_metadata_message
 
 
 class EditMetadataDialog(Ui_EditMetadataDialog):
   """
   Represents the edit metadata dialog.
 
   This class provides methods to handle the UI and save the changes in the edit metadata dialog.
@@ -57,46 +59,42 @@
     Explanation:
         This method initializes a new instance of the EditMetadataDialog class.
 
     """
     self.logger = logging.getLogger(f"{__name__}.{self.__class__.__name__}")
     self.primitive_compound_frame: PrimitiveCompoundFrame | None = None
     self.controlled_vocab_frame: ControlledVocabFrame | None = None
+    self.metadata_summary_dialog: EditMetadataSummaryDialog = EditMetadataSummaryDialog(self.save_config)
     self.instance = QDialog()
     super().setupUi(self.instance)
     self.instance.setWindowModality(QtCore.Qt.ApplicationModal)
 
     # Database API instance
     self.db_api = DatabaseAPI()
     self.config_model: ConfigModel = self.db_api.get_model(self.db_api.config_doc_id,
                                                            ConfigModel)  # type: ignore[assignment]
 
     # Initialize metadata
-    self.metadata = self.config_model.metadata
+    self.metadata = copy.deepcopy(self.config_model.metadata)
     self.metadata_types = self.get_metadata_types()
     self.minimal_metadata = [
       {"name": "subject", "displayName": "Subject"},
       {"name": "author", "displayName": "Author"},
       {"name": "datasetContact", "displayName": "Dataset contact"},
       {"name": "dsDescription", "displayName": "Ds Description"}
     ]
 
     # Connect slots
     self.metadataBlockComboBox.currentTextChanged.connect(self.change_metadata_block)
     self.typesComboBox.currentTextChanged.connect(self.change_metadata_type)
     self.minimalFullComboBox.currentTextChanged[str].connect(self.toggle_minimal_full)
     self.buttonBox.button(QtWidgets.QDialogButtonBox.Save).clicked.connect(self.save_ui)
-    self.licenseNameLineEdit.textChanged[str].connect(
-      lambda name: self.config_model.metadata['datasetVersion']['license'].update(  # type: ignore[index]
-        {"name": name}))
-    self.licenseURLLineEdit.textChanged[str].connect(
-      lambda uri: self.config_model.metadata['datasetVersion']['license'].update({"uri": uri}))  # type: ignore[index]
-
-    # Initialize UI elements
-    self.load_ui()
+    self.licenseNameLineEdit.textChanged[str].connect(self.update_license_name)
+    self.licenseURLLineEdit.textChanged[str].connect(self.update_license_uri)
+    self.buttonBox.accepted.disconnect()
 
   def get_metadata_types(self) -> dict[str, list[dict[str, str]]]:
     """Get the metadata types mapping.
 
     Retrieves the metadata types mapping from the loaded metadata model.
     The mapping is a dictionary where the keys are the display names of the metadata blocks,
     and the values are lists of dictionaries containing the name and display name of each field type.
@@ -209,46 +207,82 @@
     Load the UI for the EditMetadataDialog.
 
     This method initializes the UI elements for the EditMetadataDialog.
     It adds items to combo boxes, sets text in line edits, and configures the UI based on the metadata.
 
     """
     self.logger.info("Loading UI...")
-    self.metadataBlockComboBox.addItems(self.metadata_types.keys())
+    self.metadata = copy.deepcopy(self.config_model.metadata)
+    self.metadata_types = self.get_metadata_types()
+
+    self.metadataBlockComboBox.clear()
+    self.minimalFullComboBox.clear()
     self.minimalFullComboBox.addItems(["Full", "Minimal"])
-    dataset_version = self.config_model.metadata.get('datasetVersion', {})  # type: ignore[union-attr]
+    dataset_version = self.metadata.get('datasetVersion', {})  # type: ignore[union-attr]
     dataset_license = dataset_version.get('license', {})
     self.licenseNameLineEdit.setText(dataset_license.get('name', ''))
     self.licenseURLLineEdit.setText(dataset_license.get('uri', ''))
 
   def save_ui(self) -> None:
     """
     Save the UI changes.
 
-    Saves the changes made in the UI to the metadata.
-    Updates the metadata in the config model and updates the model document in the database.
-
+    Saves the changes made in the UI to the metadata, updates the metadata in the config model,
+    and displays the updated metadata in the summary dialog.
     """
     self.logger.info("Saving Config Model...")
     if self.controlled_vocab_frame:
       self.controlled_vocab_frame.save_modifications()
     if self.primitive_compound_frame:
       self.primitive_compound_frame.save_modifications()
+    message = get_formatted_metadata_message(self.metadata or {})
+    self.metadata_summary_dialog.summaryTextEdit.setText(message)
+    self.metadata_summary_dialog.show()
+
+  def save_config(self) -> None:
+    """
+    Save the configuration changes.
+
+    Updates the metadata in the config model, updates the model document in the database, and closes the instance.
+    """
+
     self.config_model.metadata = self.metadata
     self.db_api.update_model_document(self.config_model)
+    self.instance.close()
 
   def show(self) -> None:
     """
     Shows the instance.
 
     Explanation:
         This method shows the instance by calling its show method.
     """
+    self.load_ui()
     self.instance.show()
 
+  def update_license_name(self, name: str) -> None:
+    """
+    Updates the license name in the metadata.
+
+    Args:
+        name (str): The new license name to update in the metadata.
+    """
+    if self.metadata:
+      self.metadata['datasetVersion']['license'].update({"name": name})
+
+  def update_license_uri(self, uri: str) -> None:
+    """
+    Updates the license URI in the metadata.
+
+    Args:
+        uri (str): The new license URI to update in the metadata.
+    """
+    if self.metadata:
+      self.metadata['datasetVersion']['license'].update({"uri": uri})
+
 
 if __name__ == "__main__":
   import sys
 
   app = QtWidgets.QApplication(sys.argv)
 
   ui = EditMetadataDialog()
```

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/edit_metadata_dialog_base.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/edit_metadata_dialog_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from PySide6 import QtCore, QtGui, QtWidgets
 
 
 class Ui_EditMetadataDialog(object):
   def setupUi(self, EditMetadataDialog):
     EditMetadataDialog.setObjectName("EditMetadataDialog")
-    EditMetadataDialog.resize(950, 273)
+    EditMetadataDialog.resize(950, 428)
     self.verticalLayout = QtWidgets.QVBoxLayout(EditMetadataDialog)
     self.verticalLayout.setObjectName("verticalLayout")
     self.mainVerticalLayout = QtWidgets.QVBoxLayout()
     self.mainVerticalLayout.setObjectName("mainVerticalLayout")
     self.minimalFullComboBox = QtWidgets.QComboBox(parent=EditMetadataDialog)
     self.minimalFullComboBox.setObjectName("minimalFullComboBox")
     self.mainVerticalLayout.addWidget(self.minimalFullComboBox)
@@ -46,15 +46,15 @@
     self.typesComboBox = QtWidgets.QComboBox(parent=EditMetadataDialog)
     self.typesComboBox.setObjectName("typesComboBox")
     self.mainVerticalLayout.addWidget(self.typesComboBox)
     self.metadataScrollArea = QtWidgets.QScrollArea(parent=EditMetadataDialog)
     self.metadataScrollArea.setWidgetResizable(True)
     self.metadataScrollArea.setObjectName("metadataScrollArea")
     self.scrollAreaWidgetContents = QtWidgets.QWidget()
-    self.scrollAreaWidgetContents.setGeometry(QtCore.QRect(0, 0, 928, 94))
+    self.scrollAreaWidgetContents.setGeometry(QtCore.QRect(0, 0, 928, 249))
     self.scrollAreaWidgetContents.setObjectName("scrollAreaWidgetContents")
     self.verticalLayout_3 = QtWidgets.QVBoxLayout(self.scrollAreaWidgetContents)
     self.verticalLayout_3.setObjectName("verticalLayout_3")
     self.metadataScrollVerticalLayout = QtWidgets.QVBoxLayout()
     self.metadataScrollVerticalLayout.setObjectName("metadataScrollVerticalLayout")
     self.verticalLayout_3.addLayout(self.metadataScrollVerticalLayout)
     self.metadataScrollArea.setWidget(self.scrollAreaWidgetContents)
```

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/edit_metadata_dialog_base.ui` & `pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/edit_metadata_dialog_base.ui`

 * *Files 0% similar despite different names*

#### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/edit_metadata_dialog_base.ui` & `pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/edit_metadata_dialog_base.ui`

```diff
@@ -3,15 +3,15 @@
   <class>EditMetadataDialog</class>
   <widget class="QDialog" name="EditMetadataDialog">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>950</width>
-        <height>273</height>
+        <height>428</height>
       </rect>
     </property>
     <property name="windowTitle">
       <string>Edit metadata</string>
     </property>
     <property name="toolTip">
       <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;&lt;span style=&quot; font-style:italic;&quot;&gt;Edit the full/minimal set of metadata information for the datasets created in dataverse. Datasets corresponds to PASTA projects and needs to be mapped to the appropriate PASTA level properties as needed.&lt;/span&gt;&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
@@ -96,15 +96,15 @@
               </property>
               <widget class="QWidget" name="scrollAreaWidgetContents">
                 <property name="geometry">
                   <rect>
                     <x>0</x>
                     <y>0</y>
                     <width>928</width>
-                    <height>94</height>
+                    <height>249</height>
                   </rect>
                 </property>
                 <layout class="QVBoxLayout" name="verticalLayout_3">
                   <item>
                     <layout class="QVBoxLayout" name="metadataScrollVerticalLayout"/>
                   </item>
                 </layout>
```

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/main_dialog_base.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/main_dialog_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,16 +118,16 @@
     self.configureUploadPushButton.setToolTip(_translate("MainDialogBase", "Configure the contents of projects which need to be uploaded to dataverse."))
     self.configureUploadPushButton.setText(_translate("MainDialogBase", "Configure"))
     self.editFullMetadataPushButton.setToolTip(_translate("MainDialogBase", "Click to edit full/minimal list of metadata to be used for dataverse upload."))
     self.editFullMetadataPushButton.setText(_translate("MainDialogBase", "Edit metadata"))
     self.uploadPushButton.setToolTip(_translate("MainDialogBase", "Start uploading the above selected projects to dataverse."))
     self.uploadPushButton.setText(_translate("MainDialogBase", "Start upload"))
     self.uploadQueueScrollArea.setToolTip(_translate("MainDialogBase", "<html><head/><body><p><span style=\" font-style:italic;\">Displays the enqueued lists of PASTA projects to be uploaded to dataverse.</span><span style=\" font-style:italic;\">Users can view individual logs for each project upload, cancel each or all of them and also clear all the finished items anytime.</span></p></body></html>"))
-    self.clearFinishedPushButton.setToolTip(_translate("MainDialogBase", "Clear all finished uploads."))
-    self.clearFinishedPushButton.setText(_translate("MainDialogBase", "Clear finished"))
+    self.clearFinishedPushButton.setToolTip(_translate("MainDialogBase", "Clear all finished/cancelled/error uploads."))
+    self.clearFinishedPushButton.setText(_translate("MainDialogBase", "Clear"))
     self.cancelAllPushButton.setToolTip(_translate("MainDialogBase", "Cancel all the ongoing uploads."))
     self.cancelAllPushButton.setText(_translate("MainDialogBase", "Cancel all"))
     self.showCompletedPushButton.setToolTip(_translate("MainDialogBase", "Show uploaded projects history."))
     self.showCompletedPushButton.setText(_translate("MainDialogBase", "Show completed"))
 
 
 if __name__ == "__main__":
```

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/main_dialog_base.ui` & `pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/main_dialog_base.ui`

 * *Files 0% similar despite different names*

#### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/main_dialog_base.ui` & `pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/main_dialog_base.ui`

```diff
@@ -198,18 +198,18 @@
                           <property name="minimumSize">
                             <size>
                               <width>150</width>
                               <height>0</height>
                             </size>
                           </property>
                           <property name="toolTip">
-                            <string>Clear all finished uploads.</string>
+                            <string>Clear all finished/cancelled/error uploads.</string>
                           </property>
                           <property name="text">
-                            <string>Clear finished</string>
+                            <string>Clear</string>
                           </property>
                         </widget>
                       </item>
                       <item>
                         <widget class="QPushButton" name="cancelAllPushButton">
                           <property name="minimumSize">
                             <size>
```

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/primitive_compound_controlled_frame_base.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/primitive_compound_controlled_frame_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/primitive_compound_controlled_frame_base.ui` & `pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/primitive_compound_controlled_frame_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/primitive_compound_frame.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/primitive_compound_frame.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/project_item_frame_base.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/project_item_frame_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,18 @@
     self.projectNameLabel.setWordWrap(True)
     self.projectNameLabel.setObjectName("projectNameLabel")
     self.horizontalLayout.addWidget(self.projectNameLabel)
     self.modifiedDateTimeLabel = QtWidgets.QLabel(parent=ProjectItemFrame)
     self.modifiedDateTimeLabel.setAlignment(QtCore.Qt.AlignmentFlag.AlignLeading|QtCore.Qt.AlignmentFlag.AlignLeft|QtCore.Qt.AlignmentFlag.AlignVCenter)
     self.modifiedDateTimeLabel.setObjectName("modifiedDateTimeLabel")
     self.horizontalLayout.addWidget(self.modifiedDateTimeLabel)
+    self.projectDocIdLabel = QtWidgets.QLabel(parent=ProjectItemFrame)
+    self.projectDocIdLabel.setText("")
+    self.projectDocIdLabel.setObjectName("projectDocIdLabel")
+    self.horizontalLayout.addWidget(self.projectDocIdLabel)
     self.horizontalLayout_2.addLayout(self.horizontalLayout)
 
     self.retranslateUi(ProjectItemFrame)
     QtCore.QMetaObject.connectSlotsByName(ProjectItemFrame)
 
   def retranslateUi(self, ProjectItemFrame):
     _translate = QtCore.QCoreApplication.translate
```

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/project_item_frame_base.ui` & `pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/project_item_frame_base.ui`

 * *Files 1% similar despite different names*

#### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/project_item_frame_base.ui` & `pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/project_item_frame_base.ui`

```diff
@@ -87,14 +87,21 @@
                 <string>2024-01-16T10:52:15Z</string>
               </property>
               <property name="alignment">
                 <set>Qt::AlignLeading|Qt::AlignLeft|Qt::AlignVCenter</set>
               </property>
             </widget>
           </item>
+          <item>
+            <widget class="QLabel" name="projectDocIdLabel">
+              <property name="text">
+                <string/>
+              </property>
+            </widget>
+          </item>
         </layout>
       </item>
     </layout>
   </widget>
   <resources/>
   <connections/>
 </ui>
```

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/upload_config_dialog.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/upload_config_dialog.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #  Copyright (c) 2024
 #
 #  Author: Jithu Murugan
 #  Filename: upload_config_dialog.py
 #
 #  You should have received a copy of the license with this file. Please refer the license file for more information.
 import logging
-from typing import Any
+from typing import Any, Callable
 
 from PySide6 import QtCore, QtWidgets
 from PySide6.QtCore import QObject
 from PySide6.QtWidgets import QCheckBox, QDialog
 
 from pasta_eln.GUI.dataverse.upload_config_dialog_base import Ui_UploadConfigDialog
 from pasta_eln.dataverse.config_model import ConfigModel
@@ -24,15 +24,14 @@
   Represents the upload configuration dialog.
 
   Explanation:
       This class represents the upload configuration dialog.
       It provides methods to load and save the configuration settings.
 
   """
-  config_reloaded = QtCore.Signal()
 
   def __new__(cls, *_: Any, **__: Any) -> Any:
     """
     Creates a new instance of the UploadConfigDialog class.
 
     Explanation:
         This method creates a new instance of the UploadConfigDialog class.
@@ -42,48 +41,50 @@
         **__: Arbitrary keyword arguments.
 
     Returns:
         Any: The new instance of the UploadConfigDialog class.
     """
     return super(UploadConfigDialog, cls).__new__(cls)
 
-  def __init__(self) -> None:
+  def __init__(self, config_reloaded_callback: Callable[[], None]) -> None:
     """
     Initializes the UploadConfigDialog.
 
     Explanation:
         This method initializes the UploadConfigDialog class.
         It sets up the UI and initializes the necessary attributes.
     """
     super().__init__()
     self.logger = logging.getLogger(f"{__name__}.{self.__class__.__name__}")
     self.instance = QDialog()
     super().setupUi(self.instance)
     self.db_api = DatabaseAPI()
+    self.db_api.initialize_database()
     self.numParallelComboBox.addItems(map(str, range(2, 6)))
     self.numParallelComboBox.setCurrentIndex(2)
     self.instance.setWindowModality(QtCore.Qt.ApplicationModal)
     self.config_model: ConfigModel | None = None
     self.data_hierarchy_types: list[str] = []
     self.buttonBox.button(QtWidgets.QDialogButtonBox.Save).clicked.connect(self.save_ui)
     (self.numParallelComboBox.currentTextChanged[str]
      .connect(lambda num: setattr(self.config_model, "parallel_uploads_count", int(num))))
     self.set_data_hierarchy_types()
+    self.config_reloaded_callback = config_reloaded_callback
     self.load_ui()
 
   def load_ui(self) -> None:
     """
     Loads the UI for the UploadConfigDialog.
 
     Explanation:
         This method loads the UI for the UploadConfigDialog.
         It retrieves the config model from the database and sets up the UI elements based on the model data.
     """
     self.logger.info("Loading data and initializing UI...")
-    self.config_model = self.db_api.get_model(self.db_api.config_doc_id, ConfigModel)  # type: ignore[assignment]
+    self.config_model = self.db_api.get_config_model()
     if self.config_model is None:
       self.logger.error("Failed to load config model!")
       return
     for widget_pos in reversed(range(self.projectItemsVerticalLayout.count())):
       self.projectItemsVerticalLayout.itemAt(widget_pos).widget().setParent(None)
     for data_type in self.data_hierarchy_types:
       is_set = self.config_model.project_upload_items and self.config_model.project_upload_items.get(data_type, False)
@@ -143,30 +144,21 @@
         It retrieves the current settings from the UI elements and updates the configuration model.
         It then emits the config_reloaded signal to notify other components of the updated configuration.
     """
     self.logger.info("Saving config model...")
     if self.config_model is None:
       self.logger.error("Failed to load config model!")
       return
-    self.db_api.update_model_document(self.config_model)
-    self.config_reloaded.emit()
+    self.db_api.save_config_model(self.config_model)
+    self.config_reloaded_callback()
 
   def show(self) -> None:
     """
     Shows the instance.
 
     Explanation:
         This method shows the instance by calling its show() method.
 
     Args:
         self: The instance of the class.
     """
     self.instance.show()
-
-
-if __name__ == "__main__":
-  import sys
-
-  app = QtWidgets.QApplication(sys.argv)
-  ui = UploadConfigDialog()
-  ui.instance.show()
-  sys.exit(app.exec())
```

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/upload_config_dialog_base.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/upload_config_dialog_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/upload_config_dialog_base.ui` & `pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/upload_config_dialog_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/upload_widget_base.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/upload_widget_base.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,20 +28,26 @@
     sizePolicy.setHeightForWidth(self.uploadProjectLabel.sizePolicy().hasHeightForWidth())
     self.uploadProjectLabel.setSizePolicy(sizePolicy)
     self.uploadProjectLabel.setMinimumSize(QtCore.QSize(300, 0))
     self.uploadProjectLabel.setMaximumSize(QtCore.QSize(300, 100))
     self.uploadProjectLabel.setObjectName("uploadProjectLabel")
     self.uploadWidgetHorizontalLayout.addWidget(self.uploadProjectLabel)
     self.uploadProgressBar = QtWidgets.QProgressBar(parent=UploadWidgetFrame)
+    sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Fixed, QtWidgets.QSizePolicy.Policy.Fixed)
+    sizePolicy.setHorizontalStretch(0)
+    sizePolicy.setVerticalStretch(0)
+    sizePolicy.setHeightForWidth(self.uploadProgressBar.sizePolicy().hasHeightForWidth())
+    self.uploadProgressBar.setSizePolicy(sizePolicy)
+    self.uploadProgressBar.setMinimumSize(QtCore.QSize(400, 0))
     self.uploadProgressBar.setProperty("value", 0)
     self.uploadProgressBar.setObjectName("uploadProgressBar")
     self.uploadWidgetHorizontalLayout.addWidget(self.uploadProgressBar)
     self.statusIconLabel = QtWidgets.QLabel(parent=UploadWidgetFrame)
-    sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Preferred, QtWidgets.QSizePolicy.Policy.Preferred)
-    sizePolicy.setHorizontalStretch(0)
+    sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Fixed, QtWidgets.QSizePolicy.Policy.Preferred)
+    sizePolicy.setHorizontalStretch(50)
     sizePolicy.setVerticalStretch(0)
     sizePolicy.setHeightForWidth(self.statusIconLabel.sizePolicy().hasHeightForWidth())
     self.statusIconLabel.setSizePolicy(sizePolicy)
     self.statusIconLabel.setMinimumSize(QtCore.QSize(25, 25))
     self.statusIconLabel.setText("")
     self.statusIconLabel.setObjectName("statusIconLabel")
     self.uploadWidgetHorizontalLayout.addWidget(self.statusIconLabel)
```

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/upload_widget_base.ui` & `pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/upload_widget_base.ui`

 * *Files 5% similar despite different names*

#### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/dataverse/upload_widget_base.ui` & `pasta_eln-2.5.3b1/pasta_eln/GUI/dataverse/upload_widget_base.ui`

```diff
@@ -50,27 +50,39 @@
                   <property name="text">
                     <string>Example Project 1</string>
                   </property>
                 </widget>
               </item>
               <item>
                 <widget class="QProgressBar" name="uploadProgressBar">
+                  <property name="sizePolicy">
+                    <sizepolicy hsizetype="Fixed" vsizetype="Fixed">
+                      <horstretch>0</horstretch>
+                      <verstretch>0</verstretch>
+                    </sizepolicy>
+                  </property>
+                  <property name="minimumSize">
+                    <size>
+                      <width>400</width>
+                      <height>0</height>
+                    </size>
+                  </property>
                   <property name="toolTip">
                     <string>Shows the upload progress.</string>
                   </property>
                   <property name="value">
                     <number>0</number>
                   </property>
                 </widget>
               </item>
               <item>
                 <widget class="QLabel" name="statusIconLabel">
                   <property name="sizePolicy">
-                    <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
-                      <horstretch>0</horstretch>
+                    <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
+                      <horstretch>50</horstretch>
                       <verstretch>0</verstretch>
                     </sizepolicy>
                   </property>
                   <property name="minimumSize">
                     <size>
                       <width>25</width>
                       <height>25</height>
```

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/details.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/details.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,21 +169,21 @@
           text.document().setTextWidth(labelW.width())
           self.rescaleTexts.append(text)
           height:int = text.document().size().toTuple()[1] # type: ignore[index]
           text.setFixedHeight(height)
           text.setReadOnly(True)
           labelL.addWidget(text, stretch=1) # type: ignore[call-arg]
         else:
-          if len(dataHierarchyItem)==1 and 'list' in dataHierarchyItem[0]:
-            if not isinstance(dataHierarchyItem[0]['list'], list):                #choice among docType
-              table  = self.comm.backend.db.getView('viewDocType/'+dataHierarchyItem[0]['list'])
-              choices= [i for i in table if i['id']==self.doc[key]]
-              if len(choices)==1:
-                value = '\u260D '+choices[0]['value'][0]
-                link = True
+          if len(dataHierarchyItem)==1 and 'list' in dataHierarchyItem[0] and \
+              not isinstance(dataHierarchyItem[0]['list'], list):                #choice among docType
+            table  = self.comm.backend.db.getView('viewDocType/'+dataHierarchyItem[0]['list'])
+            choices= [i for i in table if i['id']==self.doc[key]]
+            if len(choices)==1:
+              value = '\u260D '+choices[0]['value'][0]
+              link = True
           elif isinstance(self.doc[key], list):
             value = ', '.join(self.doc[key])
           else:
             value = self.doc[key]
           label = Label(f'{key.capitalize()}: {value}', function=self.clickLink if link else None, docID=self.doc[key])
           label.setTextInteractionFlags(Qt.TextSelectableByMouse)
           self.metaDetailsL.addWidget(label)
```

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/docTypes.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/docTypes.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/form.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/form.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,16 +169,16 @@
             if isinstance(dataHierarchyItem[0]['list'], list):            #dataHierarchy-defined choices
               getattr(self, f'key_{key}').addItems(dataHierarchyItem[0]['list'])
             else:                                                    #choice among docType
               listDocType = dataHierarchyItem[0]['list']
               getattr(self, f'key_{key}').addItem('- no link -', userData='')
               for line in self.db.getView(f'viewDocType/{listDocType}'):
                 getattr(self, f'key_{key}').addItem(line['value'][0], userData=line['id'])
-                if line['value'][0] == value:
-                  getattr(self, f'key_{key}').setCurrentText(line['value'][0])
+                if line['id'] == value:
+                  getattr(self, f'key_{key}').setCurrentIndex(getattr(self, f'key_{key}').count()-1)
           else:                                   #text area
             setattr(self, f'key_{key}', QLineEdit(value))
           formL.addRow(QLabel(key.capitalize()), getattr(self, f'key_{key}'))
         else:
           print(f"**WARNING dialogForm: unknown value type. key:{key}, type:{type(value)}")
       if group == 'default':
         # individual key-value items
@@ -198,23 +198,29 @@
           self.projectComboBox = QComboBox()
           self.projectComboBox.addItem(label, userData='')
           for line in self.db.getView('viewDocType/x0'):
             # add all projects but the one that is present
             if '-branch' not in self.doc or all( not(len(branch['stack'])>0 and line['id']==branch['stack'][0])
                                                 for branch in self.doc['-branch']):
               self.projectComboBox.addItem(line['value'][0], userData=line['id'])
+              if self.doc.get('_projectID','') == line['id']:
+                self.projectComboBox.setCurrentIndex(self.projectComboBox.count()-1)
           formL.addRow(QLabel('Project'), self.projectComboBox)
+          if '_projectID' in self.doc:
+            del self.doc['_projectID']
         if allowProjectAndDocTypeChange: #if not-new and non-folder
           self.docTypeComboBox = QComboBox()
           self.docTypeComboBox.addItem(label, userData='')
           for key, value in self.db.dataLabels.items():
             if key[0]!='x':
               self.docTypeComboBox.addItem(value, userData=key)
           self.docTypeComboBox.addItem('_UNIDENTIFIED_', userData='-')
           formL.addRow(QLabel('Data type'), self.docTypeComboBox)
+    if [i for i in self.doc.keys() if i.startswith('_')]:
+      logging.error('There should not be "_" in a doc: '+str(self.doc))
     # final button box
     _, buttonLineL = widgetAndLayout('H', mainL, 'm')
     if '-branch' in self.doc:
       visibilityIcon = all(all(branch['show']) for branch in self.doc['-branch'])
       self.visibilityText = QLabel('' if visibilityIcon else 'HIDDEN     \U0001F441')
       buttonLineL.addWidget(self.visibilityText)
     buttonLineL.addStretch(1)
@@ -222,15 +228,15 @@
                                     'Add key-value pair', style='border-width:1')
     IconButton('fa5s.poll-h',      self, [Command.FORM_SHOW_DOC], buttonLineL, 'Show all information',
                style='border-width:1')
     TextButton('Save',             self, [Command.FORM_SAVE],     buttonLineL, 'Save changes')
     TextButton('Cancel',           self, [Command.FORM_CANCEL],   buttonLineL, 'Discard changes')
     if self.flagNewDoc: #new dataset
       TextButton('Save && Next', self, [Command.FORM_SAVE_NEXT], buttonLineL, 'Save this and handle next')
-    # autosave
+    # end of creating form autosave
     if (Path.home()/'.pastaELN.temp').is_file():
       with open(Path.home()/'.pastaELN.temp', 'r', encoding='utf-8') as fTemp:
         content = json.loads(fTemp.read())
         if self.doc.get('_id', '') in content:
           ret = QMessageBox.information(self, 'Information', 'There is unsaved information from a prematurely '+
                     'closed form. Do you want to restore it?\n If you decline, the unsaved information will be'+
                     ' removed.',
@@ -356,20 +362,21 @@
         if ret==QMessageBox.StandardButton.Yes:
           self.autosave()
       self.checkThreadTimer.stop()
       self.reject()
     elif command[0] in (Command.FORM_SAVE, Command.FORM_SAVE_NEXT):
       # create the data that has to be saved
       self.checkThreadTimer.stop()
-      with open(Path.home()/'.pastaELN.temp', 'r', encoding='utf-8') as fTemp:
-        content = json.loads(fTemp.read())
-        if self.doc.get('_id', '') in content:
-          del content[self.doc.get('_id', '')]
-      with open(Path.home()/'.pastaELN.temp', 'w', encoding='utf-8') as fTemp:
-        fTemp.write(json.dumps(content))
+      if (Path.home()/'.pastaELN.temp').is_file():
+        with open(Path.home()/'.pastaELN.temp', 'r', encoding='utf-8') as fTemp:
+          content = json.loads(fTemp.read())
+          if self.doc.get('_id', '') in content:
+            del content[self.doc.get('_id', '')]
+        with open(Path.home()/'.pastaELN.temp', 'w', encoding='utf-8') as fTemp:
+          fTemp.write(json.dumps(content))
       if hasattr(self, 'key_-name'):
         self.doc['-name'] = getattr(self, 'key_-name').text().strip()
         if self.doc['-name'] == '':
           showMessage(self, 'Error', 'A created item has to have a valid name')
           return
         if self.doc['-type'][0]=='x0':  #prevent project-directory names that are identical
           others = self.comm.backend.db.getView('viewDocType/x0All')
@@ -402,23 +409,20 @@
                   else:
                     showMessage(self, 'Information', 'Did update the database but not the file on harddisk, since PASTA-ELN cannot write this format')
         elif isinstance(valueOld, list):  #items that are comma separated in the text-field
           self.doc[key] = getattr(self, f'key_{key}').text().strip().split(' ')
         elif isinstance(valueOld, str):
           if isinstance(getattr(self, f'key_{key}'), QComboBox):
             valueNew = getattr(self, f'key_{key}').currentText()
-            if (valueNew != '- no link -'
-                and getattr(self, f'key_{key}').currentData() is not None
-                and re.search(
-                    r"^[a-z\-]-[a-z0-9]{32}$",
-                    getattr(self, f'key_{key}').currentData(),
-                ) is not None):
+            dataNew  = getattr(self,f'key_{key}').currentData()
+            if ((dataNew is not None and re.search(r"^[a-z\-]-[a-z0-9]{32}$",dataNew) is not None)
+                or dataNew==''):
               #if docID is stored in currentData
-              self.doc[key] = getattr(self, f'key_{key}').currentData()
-            elif valueNew!='- no link -' :
+              self.doc[key] = dataNew
+            elif valueNew!='- no link -' or dataNew is None:
               self.doc[key] = valueNew
           else:                          #normal text field
             self.doc[key] = getattr(self, f'key_{key}').text().strip()
         elif valueOld is None and key in self.doc:  #important entry, set to empty string
           self.doc[key]=''
         else:
           print("**ERROR dialogForm unknown value type",key, valueOld)
```

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/project.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/project.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/projectGroup.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/projectGroup.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,15 @@
     Args:
       btn (QButton): save or cancel button
     """
     if btn.text().endswith('Cancel'):
       self.reject()
     elif 'Save' in btn.text() and self.checkEntries():
       name = self.projectGroupName.text() if self.selectGroup.isHidden() else self.selectGroup.currentText()
+      local = remote = {}
       if btn.text().endswith('Save'):
         localPath = self.pathL.text()
         if localPath.startswith('~'):
           localPath = (Path.home()/localPath[1:]).as_posix()
         local = {'user':self.userNameL.text(), 'password':self.passwordL.text(), \
                   'database':self.databaseL.text(), 'path':localPath}
         remote = {'user':self.userNameR.text(), 'password':self.passwordR.text(), \
```

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/projectLeafRenderer.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/projectLeafRenderer.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,14 +92,15 @@
       tags = ['\u2605'*int(i[2]) if i[:2]=='#_' else i for i in tags]
       painter.drawStaticText(x0, y0+y, QStaticText(f'Tags: {" ".join(tags)}'))
     for key in doc:
       if key in _DO_NOT_RENDER_ or key[0] in ['-','_']:
         continue
       y += self.lineSep
       if isinstance(doc[key], str):
+        value = ''
         if re.match(r'^[a-z\-]-[a-z0-9]{32}$',doc[key]) is None:  #normal text
           value = doc[key]
         elif self.comm is not None:                     #link
           table = self.comm.backend.db.getView(f'viewDocType/{key}All')
           choices= [i for i in table if i['id']==doc[key]]
           if len(choices)==1:
             value = '\u260D '+choices[0]['value'][0]
```

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/projectTreeView.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/projectTreeView.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/sidebar.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/sidebar.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/table.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,16 +127,16 @@
       if self.projID=='':
         self.data = self.comm.backend.db.getView(path)
       else:
         self.data = self.comm.backend.db.getView(path, preciseKey=self.projID)
       # filter multiple lines of the same item: #https://stackoverflow.com/questions/11092511/list-of-unique-dictionaries
       self.data = list({v['id']:v for v in self.data}.values())
       self.showState.setText('(show all rows)' if self.showAll else '(hide hidden rows)')
+      docLabel = 'Unidentified'
       if self.docType=='-':
-        docLabel = 'Unidentified'
         self.actionChangeColums.setVisible(False)
       else:
         self.actionChangeColums.setVisible(True)
         if self.docType in self.comm.backend.db.dataLabels:
           docLabel = self.comm.backend.db.dataLabels[self.docType]
       if self.projID:
         self.headline.setText(docLabel)
@@ -209,15 +209,15 @@
     """
     Event if user clicks button in the center
 
     Args:
       command (list): list of commands
     """
     if command[0] is Command.ADD_ITEM:
-      self.comm.formDoc.emit({'-type':[self.docType]})
+      self.comm.formDoc.emit({'-type':[self.docType], '_projectID':self.projID})
       self.comm.changeTable.emit(self.docType, self.projID)
       if self.docType=='x0':
         self.comm.changeSidebar.emit('redraw')
     elif command[0] is Command.ADD_FILTER:
       # gui
       _, rowL = widgetAndLayout('H', self.filterL, 'm', 'xl', '0', 'xl')
       text = QLineEdit('')
```

### Comparing `pasta_eln-2.5.2b2/pasta_eln/GUI/tableHeader.py` & `pasta_eln-2.5.3b1/pasta_eln/GUI/tableHeader.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/Resources/ExampleMeasurements/simple.png` & `pasta_eln-2.5.3b1/pasta_eln/Resources/ExampleMeasurements/simple.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/Resources/ExampleMeasurements/story.odt` & `pasta_eln-2.5.3b1/pasta_eln/Resources/ExampleMeasurements/story.odt`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/Resources/Icons/favicon64.ico` & `pasta_eln-2.5.3b1/pasta_eln/Resources/Icons/favicon64.ico`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/Resources/Icons/favicon64.png` & `pasta_eln-2.5.3b1/pasta_eln/Resources/Icons/favicon64.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/Resources/Icons/ols.png` & `pasta_eln-2.5.3b1/pasta_eln/Resources/Icons/ols.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/Resources/Icons/tib.png` & `pasta_eln-2.5.3b1/pasta_eln/Resources/Icons/tib.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/Resources/Icons/wikidata.png` & `pasta_eln-2.5.3b1/pasta_eln/Resources/Icons/wikidata.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/Resources/Icons/wikipedia.png` & `pasta_eln-2.5.3b1/pasta_eln/Resources/Icons/wikipedia.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/backend.py` & `pasta_eln-2.5.3b1/pasta_eln/backend.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/cli.py` & `pasta_eln-2.5.3b1/pasta_eln/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -133,23 +133,24 @@
               print('CouchDB server',url,'is working: username and password test upcoming')
         except Exception:
           print('**ERROR pma01: CouchDB server not working |',url)
           if url=='http://127.0.0.1:5984':
             raise NameError('**ERROR pma01a: Wrong local server.') from None
 
     #open backend
+    be = None
     if not getDocu:
       try:
         be = Backend(defaultProjectGroup=args.database, initViews=initViews, initConfig=initConfig,
                   resetDataHierarchy=resetDataHierarchy)
       except Exception:
         print('**ERROR pma20: backend could not be started.\n'+traceback.format_exc()+'\n\n')
         return ''
 
-    if not getDocu and args.command.startswith('test') and be:
+    if not getDocu and args.command.startswith('test') and be is not None:
       #PART 2 of test: main test
       print('database server:',be.db.db.client.server_url)
       print('default project group:',be.configuration['defaultProjectGroup'])
       print('database name:',be.db.db.database_name)
       designDocuments = be.db.db.design_documents()
       print('Design documents')
       for item in designDocuments:
@@ -164,15 +165,15 @@
       print(f'software version: {__version__}')
       return '1'
 
     if getDocu:
       doc += '  verifyDB: test PASTA database\n'
       doc += '    example: pastaELN_CLI.py verifyDB\n'
       doc += '    example: pastaELN_CLI.py verifyDBdev (repair function)\n'
-    elif args.command.startswith('verifyDB'):
+    elif args.command.startswith('verifyDB') and be is not None:
       repair = args.command=='verifyDBdev'
       output = be.checkDB(outputStyle='', repair=repair)
       print(output)
       return '1'
 
     if getDocu:
       doc += '  exampleData: create example data by DELETING ALL DATA\n'
@@ -182,28 +183,28 @@
       #prints directly to screen
       exampleData(True)
       return '1'
 
     if getDocu:
       doc += '  syncLR / syncRL: synchronize with / from remote server\n'
       doc += '    example: pastaELN_CLI.py syncLR\n'
-    elif args.command=='syncLR':
+    elif args.command=='syncLR' and be is not None:
       progressBar = DummyProgressBar()
       success = be.replicateDB(progressBar)
       return '1' if success else '-1'
-    elif args.command=='syncRL':
+    elif args.command=='syncRL' and be is not None:
       be.exit()
       print('**ERROR pma03: syncRL not implemented yet')
       return '-1'
 
     if getDocu:
       doc += '  print: print overview\n'
       doc += "    label: possible docLabels 'Projects', 'Samples', 'Measurements', 'Procedures'\n"
       doc += "    example: pastaELN_CLI.py print -d instruments -l instrument\n"
-    elif args.command=='print':
+    elif args.command=='print' and be is not None:
       print(be.output(args.label,True))
       return '1'
 
     # if getDocu:
     #   doc += '  saveBackup,loadBackup: save to file.zip / load from file.zip\n'
     #   doc += '    - docId is optional as it reduces the scope of the backup\n'
     #   doc += '    - database is optional as otherwise the default is used\n'
@@ -218,15 +219,15 @@
     # elif args.command=='loadBackup':   #load from backup file.zip
     #   be.backup('restore')
     #   return '1'
 
     if getDocu:
       doc += '  extractorTest: test extractor on individual datafile\n'
       doc += '    example: pastaELN_CLI.py extractorTest -i ~/[long-path]/Zeiss.tif\n'
-    elif args.command=='extractorTest':
+    elif args.command=='extractorTest' and be is not None:
       be.testExtractor(args.docID)
       return '1'
 
     # if getDocu:
     #   doc += '  importXLS: import first sheet of excel file into database\n'
     #   doc += '    before: ensure database configuration and project exist\n'
     #   doc += '    example: pastaELN_CLI.py importXLS -d instruments -i x-123456 -c "~/path/to.xls" -l instrument\n'
@@ -268,44 +269,44 @@
     #     data = dict((k.lower(), v) for k, v in row.items())
     #     be.addData(args.label, data )
     #   return '1'
 
     if getDocu:
       doc += '  redo: recreate thumbnail / use-extractor\n'
       doc += '    example: pastaELN_CLI.py redo -i m-1234567890abcdefghijklmnopqrstuv -c type/test/subtest\n'
-    elif args.command=='redo':
+    elif args.command=='redo' and be is not None:
       data = dict(be.db.getDoc(args.docID))
       if args.content is not None:
         data['-type'] = args.content.split('/')
       be.useExtractors(be.basePath/data['-branch'][0]['path'], data['shasum'], data)  #any path is good since the file is the same everywhere; data-changed by reference
       if len(data['-type'])>1 and len(data['image'])>1:
         be.db.updateDoc({'image':data['image'], '-type':data['-type']},args.docID)
         return '1'
       else:
         print('**ERROR pma06: error after redo-extraction')
         return '-1'
 
     if getDocu:
       doc += '  scanProject: scan project with docID\n'
       doc += '    example: pastaELN_CLI.py scanProject -i ....\n'
-    elif args.command=='scanProject':
+    elif args.command=='scanProject' and be is not None:
       progressBar = DummyProgressBar()
       be.scanProject(progressBar, args.docID)
       return '1'
 
     ##################################################
     ## Commands that require open database and open project
     doc += '\n-- Commands that interact with a special project --\n'
-    if not getDocu and args.docID!='':
+    if not getDocu and args.docID!='' and be is not None:
       be.changeHierarchy(args.docID)
 
     if getDocu:
       doc += '  hierarchy: print document hierarchy\n'
       doc += '    example: pastaELN_CLI.py hierarchy -i x-1234567890abc'
-    elif args.command=='hierarchy':
+    elif args.command=='hierarchy' and be is not None:
       print(be.outputHierarchy(True,True))
       return '1'
 
   except:
     print(
         f"**ERROR pma10: exception thrown during pastaELN_CLI.py{traceback.format_exc()}"
         + "\n")
```

### Comparing `pasta_eln-2.5.2b2/pasta_eln/database.py` & `pasta_eln-2.5.3b1/pasta_eln/database.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """ Class for interaction with couchDB """
 import traceback, logging, time, json, os, re, base64, io
 from typing import Any, Optional, Union
 from pathlib import Path
 from anytree import Node
-from anytree.search import find_by_attr
 from PIL import Image
 from cloudant.client import CouchDB
 from cloudant.replicator import Replicator
 from .fixedStringsJson import defaultDataHierarchy, defaultDataHierarchyNode
 from .handleDictionaries import dataHierarchy_pre_to_V4
 from .miscTools import tracebackString, outputString
 
@@ -49,23 +48,14 @@
       logging.info('Convert data hierarchy to V4.0')
       dataHierarchy_pre_to_V4(self.dataHierarchy)
       if '-dataHierarchy-' in self.db:
         self.db['-dataHierarchy-'].delete()
       self.db.create_document(self.dataHierarchy)
       if '-ontology-' in self.db:
         self.db['-ontology-'].delete()
-    # temporary changes for version 2.5: remove afterwards: code does not harm but would be legacy then
-    testDocIDs = [doc['_id'] for doc in self.db if doc['_id'].startswith('x-')]
-    if testDocIDs and '-gui' not in self.db[testDocIDs[0]]:
-      for doc in self.db:
-        if doc['_id'].startswith('_') or doc['_id'].endswith('-'):
-          continue
-        if '-gui' not in doc:
-          doc['-gui'] = [True, True]
-          doc.save()
     if '-version' not in self.dataHierarchy or self.dataHierarchy['-version']!=4:
       print(F"**ERROR wrong dataHierarchy version: {self.dataHierarchy['-version']}")
       raise ValueError(f"Wrong dataHierarchy version {self.dataHierarchy['-version']}")
     self.dataLabels = {k:v['title'] for k,v in self.dataHierarchy.items() if k[0] not in ['_','-']}
     self.basePath   = basePath
     return
 
@@ -280,14 +270,18 @@
     """
     Update document by
     - saving changes to oldDoc (revision document)
     - updating new-document concurrently
     - create a docID for oldDoc
     - Bonus: save '_rev' from newDoc to oldDoc in order to track that updates cannot happen by accident
 
+    Key:Value
+    - if value is None: do not change it;
+    - if key does not exist: change it to empty, aka remove it
+
     Args:
         change (dict): item to update
         docID (string):  id of document to change
 
     Returns:
         dict: json representation of updated document
     """
@@ -336,15 +330,17 @@
             newDoc['-branch'] = [branch for branch in newDoc['-branch'] if branch['path']!=change['-branch']['path']]
             # originalLength = len(newDoc['-branch'])
             # if originalLength!=len(newDoc['-branch']):
             #   nothingChanged = False
           else:
             logging.warning('database.update.1: unknown branch op: '+newDoc['_id']+' '+newDoc['-name'])
             return newDoc
-      #handle other items
+      #handle other items: remove those that disappeared, aka were set as ''
+      for key in [i for i in set(newDoc.keys()).difference(change) if not i.startswith('_')]:
+        del newDoc[key]
       # change has to be dict, not Document
       for item in change:
         if item in ['_id','_rev','-branch']:                #skip items cannot do not result in change
           continue
         if item=='-type' and change['-type']==['--']:          #skip non-set type
           continue
         if item=='image' and change['image']=='':          #skip if non-change in image
@@ -605,44 +601,44 @@
     Returns:
       Node: hierarchy in an anytree
     """
     if not allItems:
       view = self.getView('viewHierarchy/viewHierarchy',    startKey=start)
     if allItems or len(view)==0:
       view = self.getView('viewHierarchy/viewHierarchyAll', startKey=start)
-    # for item in view:
-    #   print(item)
-    # Reorganize data into lists
-    childNum = {i['id']:i['value'][0] for i in view}
-    # ids = [i['id'] for i in view]
-    keys = [i['key'] for i in view]
-    values = [i['value'] for i in view]
-    for k,v in childNum.items():
-      keys = [i.replace(k,f'{v} {k}') for i in keys]
-    values = [x for _, x in sorted(zip(keys, values))]
-    keys   = sorted(keys)
+    # create tree of folders: these are the only ones that have children
     dataTree = None
-    hierarchy = []
-    for idx, value in enumerate(values):
-      docType = value[1]
-      name    = value[2]
-      gui     = value[3]
-      _id     = keys[idx].split()[-1]
-      level   = int(len(keys[idx].split())/2)
-      if idx==0:
-        dataTree = Node(id=_id, docType=docType, name=name, gui=gui)
-        hierarchy.append(dataTree)
+    nonFolders = []
+    id2Node = {}
+    for item in view:
+      docType = item['value'][1]
+      if docType[0][0] != 'x':
+        nonFolders.append(item)
+        continue
+      _id     = item['id']
+      childNum, docType, name, gui, _ = item['value']
+      if dataTree is None:
+        dataTree = Node(id=_id, docType=docType, name=name, gui=gui, childNum=childNum)
+        id2Node[_id] = dataTree
       else:
-        parentNode = hierarchy[level-2]
-        subNode = Node(id=_id, parent=parentNode, docType=docType, name=name, gui=gui)
-        if len(hierarchy)<level:
-          hierarchy.append('')
-        elif len(hierarchy)>level:
-          hierarchy.pop()
-        hierarchy[-1] = subNode
+        parent = item['key'].split()[-2]
+        subNode = Node(id=_id, parent=id2Node[parent], docType=docType, name=name, gui=gui, childNum=childNum)
+        id2Node[_id] = subNode
+    # add non-folders into tree
+    # print(len(nonFolders),'length: crop if too long')
+    for item in nonFolders:
+      _id     = item['id']
+      childNum, docType, name, gui, _ = item['value']
+      parentId = item['key'].split()[-2]
+      Node(id=_id, parent=id2Node[parentId], docType=docType, name=name, gui=gui, childNum=childNum)
+    # sort children
+    for parentNode in id2Node.values():
+      children = parentNode.children
+      childNums= [f'{i.childNum}{i.id}' for i in children]
+      parentNode.children = [x for _, x in sorted(zip(childNums, children))]
     return dataTree
 
 
   def hideShow(self, stack:Union[str,list[str]]) -> None:
     """
     Toggle hide/show indicator of branch
```

### Comparing `pasta_eln-2.5.2b2/pasta_eln/dataverse/base_database_api.py` & `pasta_eln-2.5.3b1/pasta_eln/dataverse/base_database_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 #  Copyright (c) 2024
 #
 #  Author: Jithu Murugan
 #  Filename: base_database_api.py
 #
 #  You should have received a copy of the license with this file. Please refer the license file for more information.
 import logging
+from threading import Lock
 from typing import Any
 
 from cloudant import couchdb
 from cloudant.design_document import DesignDocument
 from cloudant.document import Document
 from cloudant.error import CloudantDatabaseException
 from cloudant.view import View
@@ -56,14 +57,15 @@
     self.logger = logging.getLogger(f"{__name__}.{self.__class__.__name__}")
     config = read_pasta_config_file(self.logger)
     if 'defaultProjectGroup' in config:
       self.db_name = config['defaultProjectGroup']
     else:
       raise log_and_create_error(self.logger, ConfigError, "Incorrect config file, defaultProjectGroup not found!")
     self.set_username_password(config)
+    self.update_lock = Lock()
 
   def set_username_password(self, config: dict[str, Any]) -> None:
     """
     Sets the username and password based on the provided config.
 
     Args:
         config (dict[str, Any]): The configuration dictionary.
@@ -146,23 +148,24 @@
     Make sure to use the `_id` and `_rev` keys in the data to identify the document to update otherwise a new document will be created.
 
     Args:
         data (dict[str, Any]): The data to update the document with.
 
     """
     self.logger.info("Updating document with data: %s", data)
-    with couchdb(self.username,
-                 self.password,
-                 url=self.url,
-                 connect=True) as client:
-      pasta_db = client[self.db_name]
-      with Document(pasta_db, data['_id']) as document:
-        for key, value in data.items():
-          if key not in ['_id', '_rev']:
-            document[key] = value
+    with self.update_lock:
+      with couchdb(self.username,
+                   self.password,
+                   url=self.url,
+                   connect=True) as client:
+        pasta_db = client[self.db_name]
+        with Document(pasta_db, data['_id']) as document:
+          for key, value in data.items():
+            if key not in ['_id', '_rev']:
+              document[key] = value
 
   def add_view(self,
                design_document_name: str,
                view_name: str,
                map_func: str,
                reduce_func: str | None = None) -> None:
     """
```

### Comparing `pasta_eln-2.5.2b2/pasta_eln/dataverse/base_model.py` & `pasta_eln-2.5.3b1/pasta_eln/dataverse/base_model.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/dataverse/client.py` & `pasta_eln-2.5.3b1/pasta_eln/dataverse/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,22 @@
   Client for communicating with Dataverse Server via REST API
   """
 
   def __init__(self,
                server_url: str,
                api_token: str,
                client_session_timeout: int = 10) -> None:
+    """
+    Initializes the dataverse client.
+
+    Args:
+        server_url (str): The URL of the server.
+        api_token (str): The API token for authentication.
+        client_session_timeout (int): The timeout value for the client session in seconds.
+    """
     self.logger = logging.getLogger(f"{__name__}.{self.__class__.__name__}")
     self.api_token = api_token
     self.server_url = server_url
     self.http_client = AsyncHttpClient(client_session_timeout)
 
   @handle_dataverse_exception_async
   async def check_if_token_expired(self) -> bool:
@@ -294,14 +302,42 @@
              f"Id: {identifier}, "
              f"Reason: {resp['reason']}, "
              f"Info: {resp['result']}")
     self.logger.error(error)
     return error
 
   @handle_dataverse_exception_async
+  async def get_dataverse_info(self,
+                               identifier: str) -> str | Any:
+    """
+    Retrieves information about a dataverse.
+
+    Args:
+        identifier (str): The identifier of the dataverse.
+
+    Returns:
+        str | Any: The data associated with the dataverse if the request is successful, otherwise an error message.
+    """
+
+    self.logger.info("Retrieving dataverse info, Server: %s, Dataverse identifier: %s", self.server_url, identifier)
+    resp = await self.http_client.get(
+      f"{self.server_url}/api/dataverses/{identifier}",
+      request_headers={'Accept': 'application/json', 'X-Dataverse-key': self.api_token})
+    if not resp and self.http_client.session_request_errors:
+      return self.http_client.session_request_errors
+    if resp["status"] == 200 and resp["reason"] == 'OK':
+      return resp["result"].get("data")
+    error = (f"Error retrieving the info for data verse, "
+             f"Id: {identifier}, "
+             f"Reason: {resp['reason']}, "
+             f"Info: {resp['result']}")
+    self.logger.error(error)
+    return error
+
+  @handle_dataverse_exception_async
   async def create_and_publish_dataset(self,
                                        parent_dataverse_id: str,
                                        ds_metadata: dict[str, Any],
                                        ds_validate_metadata: bool = False
                                        ) -> dict[Any, Any] | Any:
     """
     Creates and publishes a dataset to the parent dataverse.
@@ -388,15 +424,15 @@
 
     self.logger.info("Uploading file: %s to Dataset: %s on server: %s",
                      df_file_path,
                      ds_pid,
                      self.server_url)
     filename = basename(df_file_path)
     metadata = dumps({"description": df_description, "categories": df_categories})
-    data = FormData()
+    data = FormData(quote_fields=False)
     with open(df_file_path, 'rb') as file_stream:
       data.add_field('file',
                      file_stream,
                      filename=filename,
                      content_type='multipart/form-data')
       data.add_field('jsonData', metadata, content_type='application/json')
       # Request to add the file to dataset
@@ -496,14 +532,47 @@
              f"on server: {self.server_url}, "
              f"Reason: {resp['reason']}, "
              f"Info: {resp['result']}")
     self.logger.error(error)
     return error
 
   @handle_dataverse_exception_async
+  async def get_dataset_locks(self,
+                              ds_persistent_id: str) -> dict[Any, Any] | Any:
+    """
+    Fetches locks for a dataset.
+
+    Explanation:
+        This method fetches the locks for a dataset identified by the persistent ID.
+        It makes an asynchronous HTTP GET request to retrieve the locks information and handles exceptions.
+
+    Args:
+        ds_persistent_id (str): The persistent ID of the dataset to fetch locks for.
+
+    Returns:
+        dict[Any, Any] | Any: A dictionary containing the locks information if successful, or an error message.
+    """
+    self.logger.info("Fetching locks for dataset: %s for server: %s", ds_persistent_id,
+                     self.server_url)
+    resp = await self.http_client.get(
+      f"{self.server_url}/api/datasets/:persistentId/locks?persistentId={ds_persistent_id}",
+      request_params={'Accept': 'application/json'},
+      request_headers={'Content-Type': 'application/json', 'X-Dataverse-key': self.api_token})
+    if not resp and self.http_client.session_request_errors:
+      return self.http_client.session_request_errors
+    if resp["status"] == 200 and resp["reason"] == 'OK':
+      return {'locks': resp.get('result').get('data')}
+    error = (f"Error fetching locks for dataset: {ds_persistent_id} "
+             f"on server: {self.server_url}, "
+             f"Reason: {resp['reason']}, "
+             f"Info: {resp['result']}")
+    self.logger.error(error)
+    return error
+
+  @handle_dataverse_exception_async
   async def get_dataset_files(self,
                               ds_persistent_id: str,
                               version: str = ":latest-published") -> dict[Any, Any] | Any:
     """
     Fetch the file list for dataset.
     Args:
       ds_persistent_id (str): The identifier of the dataset.
```

### Comparing `pasta_eln-2.5.2b2/pasta_eln/dataverse/config_error.py` & `pasta_eln-2.5.3b1/pasta_eln/dataverse/config_error.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/dataverse/config_model.py` & `pasta_eln-2.5.3b1/pasta_eln/dataverse/config_model.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/dataverse/database_api.py` & `pasta_eln-2.5.3b1/pasta_eln/dataverse/database_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 
 from cloudant.document import Document
 
 from pasta_eln.dataverse.base_database_api import BaseDatabaseAPI
 from pasta_eln.dataverse.config_model import ConfigModel
 from pasta_eln.dataverse.project_model import ProjectModel
 from pasta_eln.dataverse.upload_model import UploadModel
-from pasta_eln.dataverse.utils import log_and_create_error, set_authors, set_template_values
+from pasta_eln.dataverse.utils import decrypt_data, encrypt_data, get_encrypt_key, log_and_create_error, set_authors, \
+  set_template_values
 
 
 class DatabaseAPI:
   """
   Provides an interface to interact with the database for dataverse specific operations.
 
   Explanation:
@@ -48,17 +49,17 @@
     """
     super().__init__()
     self.logger = logging.getLogger(f"{__name__}.{self.__class__.__name__}")
     self.db_api = BaseDatabaseAPI()
     self.design_doc_name = '_design/viewDataverse'
     self.config_doc_id = '-dataverseConfig-'
     self.data_hierarchy_doc_id = '-dataHierarchy-'
-    self.upload_model_view_name = "dvUploadView"
-    self.project_model_view_name = "dvProjectsView"
-    self.initialize_database()
+    self.upload_model_view_name = 'dvUploadView'
+    self.project_model_view_name = 'dvProjectsView'
+    _, self.encrypt_key = get_encrypt_key(self.logger)
 
   def create_dataverse_design_document(self) -> Document:
     """
     Creates a design document for the dataverse in the database.
 
     Explanation:
         This method creates a design document for the dataverse in the database
@@ -224,14 +225,73 @@
     self.logger.info("Getting model with id: %s, type: %s", model_id, model_type)
     if model_type not in (UploadModel, ProjectModel, ConfigModel):
       raise log_and_create_error(self.logger, TypeError, f"Unsupported model type {model_type}")
     if model_id is None:
       raise log_and_create_error(self.logger, ValueError, "model_id cannot be None")
     return model_type(**self.db_api.get_document(model_id))
 
+  def get_config_model(self) -> ConfigModel | None:
+    """
+    Retrieves the config model from the database.
+
+    Explanation:
+        This method retrieves the config model from the database using the appropriate document ID.
+        It performs the necessary validations and returns the retrieved config model.
+
+    Args:
+        self: The DatabaseAPI instance.
+
+    Returns:
+        ConfigModel: The retrieved config model.dataverse_login_info = {dict: 2} {'api_token': 'encrypted_token', 'dataverse_id': 'some_id'}
+    """
+    self.logger.info("Getting config model...")
+    config_model = self.get_model(self.config_doc_id, ConfigModel)
+    if config_model is None or not isinstance(config_model, ConfigModel):
+      self.logger.error("Fatal error, Failed to load config model!")
+      return None
+    if not isinstance(config_model.dataverse_login_info, dict):
+      self.logger.error("Fatal Error, Invalid dataverse login info!")
+      return None
+    api_token = config_model.dataverse_login_info.get("api_token")
+    if self.encrypt_key and api_token:
+      config_model.dataverse_login_info["api_token"] = decrypt_data(self.logger, self.encrypt_key, api_token)
+    if not self.encrypt_key and api_token:
+      self.logger.warning(
+        "No encryption key found. Hence if any API key exists, it will be removed and the user needs to re-enter it.")
+      config_model.dataverse_login_info["api_token"] = None
+      config_model.dataverse_login_info["dataverse_id"] = None
+      self.update_model_document(config_model)
+    return config_model
+
+  def save_config_model(self, config_model: ConfigModel) -> None:
+    """
+    Saves the config model to the database.
+
+    Explanation:
+        This method saves the config model to the database using the appropriate document ID.
+
+    Args:
+        self: The DatabaseAPI instance.
+        config_model (ConfigModel): The config model to save.
+    """
+    self.logger.info("Saving config model...")
+    if (not config_model
+        or not isinstance(config_model, ConfigModel)
+        or not isinstance(config_model.dataverse_login_info, dict)):
+      self.logger.error("Invalid config model!")
+      return
+    if not self.encrypt_key:
+      raise log_and_create_error(self.logger, ValueError,
+                                 "Fatal Error, No encryption key found! Make sure to initialize the database!")
+    if api_token := config_model.dataverse_login_info["api_token"]:
+      config_model.dataverse_login_info["api_token"] = encrypt_data(self.logger, self.encrypt_key, api_token)
+    if server_url := config_model.dataverse_login_info["server_url"]:
+      config_model.dataverse_login_info["server_url"] = server_url.strip("/").strip("\\")
+    self.update_model_document(config_model)
+
   def get_data_hierarchy(self) -> dict[str, Any] | None:
     """
     Retrieves the data hierarchy from the database.
 
     Explanation:
         This method retrieves the data hierarchy from the database using the appropriate document ID.
         It performs the necessary validations and returns the retrieved data hierarchy.
```

### Comparing `pasta_eln-2.5.2b2/pasta_eln/dataverse/database_error.py` & `pasta_eln-2.5.3b1/pasta_eln/dataverse/database_error.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/dataverse/dataset-create-new-all-default-fields.json` & `pasta_eln-2.5.3b1/pasta_eln/dataverse/dataset-create-new-all-default-fields.json`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/dataverse/generic_task_object.py` & `pasta_eln-2.5.3b1/pasta_eln/dataverse/generic_task_object.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
   Explanation:
       This class represents a generic task object and provides methods for managing the task.
       It includes methods for cancelling the task, starting the task, and cleaning up the task.
   """
   cancel = QtCore.Signal()
   start = QtCore.Signal()
-  finished = QtCore.Signal()
+  finish = QtCore.Signal()
   id_iterator = itertools.count()
 
   def __init__(self) -> None:
     """
     Initializes the GenericTaskObject instance.
 
     Explanation:
@@ -44,15 +44,17 @@
     """
     super().__init__()
     self.logger = logging.getLogger(f"{__name__}.{self.__class__.__name__}")
     self.id = next(self.id_iterator)
     self.cancelled = False
     self.started = False
     self.cleaned = False
+    self.finished = False
     self.cancel.connect(lambda: self.cancel_task())  # pylint: disable=unnecessary-lambda
+    self.finish.connect(lambda: self.finish_task())  # pylint: disable=unnecessary-lambda
     self.start.connect(self.start_task)
 
   def cancel_task(self) -> None:
     """
     Cancels the task.
 
     Explanation:
@@ -89,7 +91,21 @@
 
     Args:
         self: The GenericTaskObject instance.
 
     """
     self.logger.info("Cleaning up task, id: %s", self.id)
     self.cleaned = True
+    self.cancel.disconnect()
+    self.finish.disconnect()
+    self.start.disconnect()
+
+  def finish_task(self) -> None:
+    """
+    Finish up the task.
+
+    Args:
+        self: The instance of the class.
+    """
+
+    self.logger.info("Finishing up the task, id: %s", self.id)
+    self.finished = True
```

### Comparing `pasta_eln-2.5.2b2/pasta_eln/dataverse/incorrect_parameter_error.py` & `pasta_eln-2.5.3b1/pasta_eln/dataverse/incorrect_parameter_error.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/dataverse/project_model.py` & `pasta_eln-2.5.3b1/pasta_eln/dataverse/project_model.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/dataverse/task_thread_extension.py` & `pasta_eln-2.5.3b1/pasta_eln/dataverse/task_thread_extension.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/dataverse/upload_model.py` & `pasta_eln-2.5.3b1/pasta_eln/dataverse/upload_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     else:
       raise IncorrectParameterError(f"Expected string type for status but got {type(status)}")
     if isinstance(finished_date_time, str | None):
       self._finished_date_time: str | None = finished_date_time
     else:
       raise IncorrectParameterError(f"Expected string type for finished_date_time but got {type(finished_date_time)}")
     if isinstance(log, str):
-      self._log: str = log
+      self._log: str = f"{log}\n" if log and not log.endswith('\n') else log
     else:
       raise IncorrectParameterError(f"Expected string type for log but got {type(log)}")
     if isinstance(dataverse_url, str | None):
       self._dataverse_url: str | None = dataverse_url
     else:
       raise IncorrectParameterError(f"Expected string type for dataverse_url but got {type(dataverse_url)}")
 
@@ -311,18 +311,18 @@
     Args:
         value (str): The log message to be appended.
 
     Raises:
         IncorrectParameterError: If the value is not of type str.
 
     """
-    if isinstance(value, str):
-      self._log += f"{value}\n"
-    else:
+    if not isinstance(value, str):
       raise IncorrectParameterError(f"Expected string type for log but got {type(value)}")
+    if value != "":
+      self._log += value if value.endswith('\n') else f"{value}\n"
 
   @log.deleter
   def log(self) -> None:
     """
     Deletes the log of the upload.
 
     """
```

### Comparing `pasta_eln-2.5.2b2/pasta_eln/dataverse/upload_queue_manager.py` & `pasta_eln-2.5.3b1/pasta_eln/dataverse/upload_queue_manager.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 #  Author: Jithu Murugan
 #  Filename: upload_manager_task_thread.py
 #
 #  You should have received a copy of the license with this file. Please refer the license file for more information.
 import logging
 from time import sleep
 
+from PySide6 import QtCore
+from PySide6.QtCore import QTimer
+
 from pasta_eln.dataverse.config_model import ConfigModel
 from pasta_eln.dataverse.database_api import DatabaseAPI
 from pasta_eln.dataverse.generic_task_object import GenericTaskObject
 from pasta_eln.dataverse.task_thread_extension import TaskThreadExtension
 
 
 class UploadQueueManager(GenericTaskObject):
@@ -22,14 +25,15 @@
 
   Explanation:
       This class handles the management of an upload queue.
       It provides methods to add tasks to the queue, remove tasks from the queue,
       start the task execution, clean up resources, and cancel the task.
 
   """
+  cancel_all_tasks = QtCore.Signal()
 
   def __init__(self) -> None:
     """
     Initializes the UploadQueueManager instance.
 
     Explanation:
         This method initializes the UploadQueueManager instance by setting up the logger,
@@ -46,14 +50,16 @@
     super().__init__()
     self.logger = logging.getLogger(f"{__name__}.{self.__class__.__name__}")
     self.number_of_concurrent_uploads: int | None = None
     self.config_model: ConfigModel | None = None
     self.upload_queue: list[TaskThreadExtension] = []
     self.running_queue: list[TaskThreadExtension] = []
     self.db_api: DatabaseAPI = DatabaseAPI()
+    self.cancel_all_tasks.connect(
+      lambda: self.cancel_all_queued_tasks_and_empty_queue())  # pylint: disable=unnecessary-lambda
     self.set_concurrent_uploads()
 
   def set_concurrent_uploads(self) -> None:
     """
     Resets the number of concurrent uploads.
 
     Explanation:
@@ -61,33 +67,32 @@
         number_of_concurrent_uploads attribute.
 
     Args:
         None
 
     """
     self.logger.info("Resetting number of concurrent uploads..")
-    model = self.db_api.get_model(self.db_api.config_doc_id, ConfigModel)
-    self.config_model = model if isinstance(model, ConfigModel) else None
+    self.config_model = self.db_api.get_config_model()
     self.number_of_concurrent_uploads = self.config_model.parallel_uploads_count if self.config_model else None
 
   def add_to_queue(self, upload_task_thread: TaskThreadExtension) -> None:
     """
     Adds a thread task to the upload queue.
 
     Explanation:
         This method adds the given upload_task_thread to the upload queue.
-        It also connects the finished signal of the task to the remove_from_queue method.
+        It also connects the finish signal of the task to the remove_from_queue method.
 
     Args:
         upload_task_thread (TaskThreadExtension): The thread task to be added to the upload queue.
 
     """
     self.logger.info("Adding thread task to upload queue, id: %s", upload_task_thread.task.id)
     self.upload_queue.append(upload_task_thread)
-    upload_task_thread.task.finished.connect(lambda: self.remove_from_queue(upload_task_thread))
+    upload_task_thread.task.finish.connect(lambda: self.remove_from_queue(upload_task_thread))
 
   def remove_from_queue(self, upload_task_thread: TaskThreadExtension) -> None:
     """
     Removes a thread task from the upload queue.
 
     Explanation:
         This method removes the given upload_task_thread from the upload queue.
@@ -99,14 +104,15 @@
     """
     self.logger.info("Removing thread task from upload queue, id: %s", upload_task_thread.task.id)
     if upload_task_thread in self.upload_queue:
       self.upload_queue.remove(upload_task_thread)
     if upload_task_thread in self.running_queue:
       self.running_queue.remove(upload_task_thread)
     upload_task_thread.worker_thread.quit()
+    upload_task_thread.task.cleanup()
 
   def start_task(self) -> None:
     """
     Starts the upload queue task.
 
     Explanation:
         This method starts the upload queue task by calling the super-class's start_task method.
@@ -120,15 +126,18 @@
     self.logger.info("Starting upload queue..")
     super().start_task()
     while not self.cancelled:
       if self.number_of_concurrent_uploads and len(self.running_queue) < self.number_of_concurrent_uploads:
         for upload_task_thread in self.upload_queue:
           if self.cancelled or len(self.running_queue) >= self.number_of_concurrent_uploads:
             break
-          if not upload_task_thread.task.started and not upload_task_thread.task.cancelled:
+          if (not upload_task_thread.task.started
+              and not upload_task_thread.task.cancelled
+              and not upload_task_thread.task.finished
+              and upload_task_thread not in self.running_queue):
             self.running_queue.append(upload_task_thread)
             upload_task_thread.task.start.emit()
       sleep(0.5)
 
   def cleanup(self) -> None:
     """
     Cleans up the upload manager.
@@ -147,34 +156,59 @@
 
   def empty_upload_queue(self) -> None:
     """
     Empties the upload queue.
 
     Explanation:
         This method empties the upload queue by quitting each upload task thread and clearing the upload queue.
-
-    Args:
-        None
-
     """
     self.logger.info("Emptying upload queue..")
     for upload_task_thread in self.upload_queue:
-      upload_task_thread.quit()
+      upload_task_thread.worker_thread.quit()
     self.upload_queue.clear()
 
+  def remove_cancelled_tasks(self) -> None:
+    """
+    Removes cancelled tasks from the upload queue.
+
+    Explanation:
+        This method identifies tasks in the upload queue that have been cancelled and removes them from the queue.
+        It also logs the removal of each cancelled task.
+
+    Args:
+        self: The instance of the UploadQueueManager.
+    """
+    self.logger.info("Removing cancelled tasks from the queue..")
+    cancelled_tasks = [upload_task_thread for upload_task_thread in self.upload_queue if
+                       upload_task_thread.task.cancelled]
+    for upload_task_thread in cancelled_tasks:
+      self.remove_from_queue(upload_task_thread)
+
   def cancel_task(self) -> None:
     """
     Cancels the upload queue manager completely.
 
     Explanation:
         This method cancels the upload queue by calling the super-class's cancel_task method.
         It emits the cancel signal for each task in the running queue and empties the upload queue.
+    """
+    self.logger.info("Cancelling upload manager..")
+    super().cancel_task()
+    # Cancel all the tasks in the pool and remove them all from the queue
+    self.cancel_all_queued_tasks_and_empty_queue()
 
-    Args:
-        None
+  def cancel_all_queued_tasks_and_empty_queue(self) -> None:
+    """
+    Cancels all queued tasks and empties the upload queue.
 
+    Explanation:
+        This function iterates through the upload queue, cancelling each task thread by emitting a cancel signal.
+        It then empties the upload queue.
+
+    Args:
+        self: The instance of the class.
     """
-    self.logger.info("Cancelling upload queue..")
-    super().cancel_task()
-    for upload_task_thread in self.running_queue:
+    self.logger.info("Cancelling upload queue and the empty the upload queue..")
+    for upload_task_thread in self.upload_queue:
       upload_task_thread.task.cancel.emit()
-    self.empty_upload_queue()
+    if self.upload_queue:
+      QTimer.singleShot(500, lambda: self.remove_cancelled_tasks())  # pylint: disable=unnecessary-lambda
```

### Comparing `pasta_eln-2.5.2b2/pasta_eln/dataverse/upload_status_values.py` & `pasta_eln-2.5.3b1/pasta_eln/dataverse/upload_status_values.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/dataverse/utils.py` & `pasta_eln-2.5.3b1/pasta_eln/dataverse/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,52 +12,59 @@
 import re
 from asyncio import get_event_loop
 from base64 import b64decode, b64encode
 from json import dump, load
 from logging import Logger
 from os.path import exists, join
 from pathlib import Path
-from typing import Any, Type
+from typing import Any, Callable, Type
 
-from PySide6.QtWidgets import QBoxLayout, QLabel
+from PySide6.QtCore import QSize
+from PySide6.QtGui import QImage, QPixmap
+from PySide6.QtWidgets import QBoxLayout
 from cryptography.fernet import Fernet, InvalidToken
 from qtawesome import icon
 
 from pasta_eln.dataverse.client import DataverseClient
 from pasta_eln.dataverse.config_error import ConfigError
 from pasta_eln.dataverse.upload_status_values import UploadStatusValues
 
 
-def update_status(status: str, statusIconLabel: QLabel, statusLabel: QLabel) -> None:
+def update_status(status: str,
+                  status_label_set_text_callback: Callable[[str], None],
+                  status_icon_set_pixmap_callback: Callable[[QPixmap | QImage | str], None]) -> None:
   """
-  Updates the status and status icon of the upload.
-
-  Explanation:
-      This function updates the status and status icon of the upload based on the given status.
-      It sets the text of the statusLabel and the pixmap of the statusIconLabel based on the status value.
+  Updates the status with the corresponding label and icon.
 
   Args:
-      status (str): The status of the upload.
-      statusIconLabel (QLabel): The label to display the status icon.
-      statusLabel (QLabel): The label to display the status text.
+      status (str): The status value.
+      status_label_set_text_callback (Callable[[str], None]): The callback function to set the status label text.
+      status_icon_set_pixmap_callback (Callable[[QPixmap | QImage | str], None]): The callback function to set the status icon pixmap.
+
+  Explanation:
+      This function updates the status with the corresponding label and icon based on the given status value.
+      It uses the provided callback functions to set the status label text and status icon pixmap.
   """
-  statusLabel.setText(status)
   match status:
     case UploadStatusValues.Queued.name:
-      statusIconLabel.setPixmap(icon('ph.queue-bold').pixmap(statusIconLabel.size()))
+      icon_name = 'fa.circle-o-notch'
     case UploadStatusValues.Uploading.name:
-      statusIconLabel.setPixmap(icon('mdi6.progress-upload').pixmap(statusIconLabel.size()))
+      icon_name = 'fa.cloud-upload'
     case UploadStatusValues.Cancelled.name:
-      statusIconLabel.setPixmap(icon('mdi.cancel').pixmap(statusIconLabel.size()))
+      icon_name = 'fa.minus-circle'
     case UploadStatusValues.Finished.name:
-      statusIconLabel.setPixmap(icon('fa.check-circle-o').pixmap(statusIconLabel.size()))
+      icon_name = 'fa.check-circle-o'
     case UploadStatusValues.Error.name:
-      statusIconLabel.setPixmap(icon('msc.error-small').pixmap(statusIconLabel.size()))
+      icon_name = 'fa.times-circle-o'
     case UploadStatusValues.Warning.name:
-      statusIconLabel.setPixmap(icon('fa.warning').pixmap(statusIconLabel.size()))
+      icon_name = 'fa.warning'
+    case _:
+      icon_name = 'fa.times-circle-o'
+  status_label_set_text_callback(status)
+  status_icon_set_pixmap_callback(icon(icon_name).pixmap(QSize(30, 30)))
 
 
 def set_authors(logger: Logger, metadata: dict[str, Any]) -> None:
   """
   Sets the authors in the metadata.
 
   Explanation:
@@ -86,14 +93,42 @@
     author_copy['authorName']['value'] = ', '.join(filter(None, [author['last'], author['first']]))
     author_copy['authorIdentifierScheme']['value'] = "ORCID"
     author_copy['authorIdentifier']['value'] = author['orcid']
     author_copy['authorAffiliation']['value'] = ', '.join([o['organization'] for o in author['organizations']])
     authors_list.append(author_copy)
 
 
+def get_flattened_metadata(metadata: dict[str, Any]) -> dict[str, Any]:
+  """
+  Returns a flattened version of the metadata.
+
+  Args:
+      metadata (dict[str, Any]): The metadata to be flattened.
+
+  Returns:
+      dict[str, Any]: The flattened metadata.
+
+  Explanation:
+      This function takes a nested metadata dictionary and returns a flattened version of the metadata.
+      It extracts the values from the nested structure and creates a new dictionary with a flattened structure.
+      The resulting dictionary contains the field names as keys and their corresponding values.
+
+  Exceptions:
+      KeyError: If a field name is not found in the metadata dictionary.
+  """
+  adjusted_metadata = {}
+  if metadata['datasetVersion']['license']:
+    adjusted_metadata['license'] = metadata['datasetVersion']['license']
+  for _, metablock in metadata['datasetVersion']['metadataBlocks'].items():
+    for field in metablock['fields']:
+      if field['value']:
+        adjusted_metadata[field['typeName']] = field['value']
+  return adjusted_metadata
+
+
 def set_template_values(logger: Logger, metadata: dict[str, Any]) -> None:
   """
   Set template values in the metadata.
 
   This function sets template values in the metadata dictionary based on the type of each field.
   If the metadata is empty, a warning is logged.
   The function iterates through the metadata blocks
@@ -148,14 +183,21 @@
       logger (Logger): The logger object for logging warnings.
       metadata (dict[str, Any]): The metadata dictionary.
       check_title (bool, optional): Flag to indicate if the title should be checked.
       Defaults to True.
 
   Returns:
       dict[str, list[str]] | None: The missing information dictionary or None if metadata is empty.
+      missing_information = {
+                              'title': [],
+                              'author': [],
+                              'datasetContact': [],
+                              'dsDescription': [],
+                              'subject': []
+                            }
 
   """
   if not metadata:
     logger.warning("Empty metadata, make sure the metadata is loaded correctly...")
     return None
   missing_information: dict[str, list[str]] = {
     'title': [],
@@ -265,15 +307,15 @@
       field (dict[str, Any]): The field dictionary.
       missing_information (dict[str, list[str]]): The dictionary to track missing information.
       missing_field_name (str): The name of the missing field.
       check (bool, optional): Flag to indicate if the check should be performed. Defaults to True.
 
   """
   if check and not field.get('value'):
-    missing_message = f"{missing_field_name.capitalize()} field is missing!"
+    missing_message = f"Add at-least a single entry for {missing_field_name.capitalize()}!"
     if missing_message not in missing_information[missing_field_name]:
       missing_information[missing_field_name].append(missing_message)
 
 
 def get_encrypt_key(logger: Logger) -> tuple[bool, bytes]:
   """
   Gets the dataverse encryption key.
@@ -466,14 +508,40 @@
     logger.warning("Data server is reachable but API token is invalid: %s", message)
   else:
     result = False, "Data server is not reachable"
     logger.warning("Data server is not reachable: %s", message)
   return result
 
 
+def check_if_dataverse_exists(logger: Logger, api_token: str, server_url: str, dataverse_id: str) -> bool:
+  """
+  Checks if a Dataverse exists based on the provided server URL, API token, and Dataverse ID.
+
+  Args:
+      logger (Logger): The logger object for logging information.
+      api_token (str): The API token for authentication.
+      server_url (str): The URL of the Dataverse server.
+      dataverse_id (str): The ID of the Dataverse to check existence for.
+
+  Returns:
+      bool: True if the Dataverse exists, False otherwise.
+  """
+  logger.info("Checking if login info is valid, server_url: %s", server_url)
+  dataverse_client = DataverseClient(server_url, api_token)
+  event_loop = get_event_loop()
+  info = event_loop.run_until_complete(dataverse_client.get_dataverse_info(dataverse_id))
+  result = False
+  if isinstance(info, dict):
+    result = (info.get("id", None) is not None
+              and info.get("alias", None) == dataverse_id)
+  else:
+    logger.warning("Data verse with id %s does not exist, Server message: %s", dataverse_id, info)
+  return result
+
+
 def adjust_type_name(camel_case_string: str) -> str:
   """
   Adjusts the type name from camel case to title case.
 
   Splits the camel case string into individual words and capitalizes the first letter of each word.
   If a word starts with an uppercase letter, it is left as is.
 
@@ -542,7 +610,108 @@
   """
   if layout is None:
     return
   for widget_pos in reversed(range(layout.count())):
     if item := layout.itemAt(widget_pos):
       item.widget().setParent(None)  # type: ignore[call-overload]
   layout.setParent(None)  # type: ignore[arg-type]
+
+
+def get_formatted_message(missing_metadata: dict[str, list[str]]) -> str:
+  """
+  Returns a formatted message with missing metadata information.
+
+  Args:
+      missing_metadata (dict[str, list[str]]): A dictionary containing missing metadata information.
+
+  Returns:
+      str: A formatted message with the missing metadata information.
+
+  Explanation:
+      This function takes a dictionary of missing metadata information and returns a formatted message
+      with the missing information. The message is formatted as an HTML string and includes a list of missing
+      metadata items grouped by their corresponding metadata names.
+  """
+  if not any(missing_metadata.values()):
+    return ""
+  name_mapping = {
+    'author': 'Author',
+    'datasetContact': "Dataset Contact",
+    'dsDescription': "Dataset Description",
+    'subject': "Subject"
+  }
+  message = (
+    "<html><p><i>Goto 'Edit Metadata' dialog, enter the below given missing information and retry the upload!</i></p>"
+  )
+  for metadata_name, missing_list in missing_metadata.items():
+    if missing_list:
+      message += f"<br></br><b><i>{name_mapping[metadata_name]}:</i></b><ul>"
+      for missing in missing_list:
+        message += f"<i style=\"color:Crimson\"><li>{missing}</li></i>"
+      message += "</ul>"
+  message += "</html>"
+  return message
+
+
+def get_formatted_metadata_message(metadata: dict[str, Any]) -> str:
+  """
+  Formats metadata into an HTML message for display.
+
+  Args:
+      metadata (dict): A dictionary containing metadata information.
+
+  Returns:
+      str: An HTML-formatted message representing the metadata.
+
+  Examples:
+      >>> metadata = {
+      ...     'datasetVersion': {
+      ...         'license': {'name': 'CC0', 'uri': 'https://creativecommons.org/publicdomain/zero/1.0/'},
+      ...         'metadataBlocks': {
+      ...             'citation': {
+      ...                 'displayName': 'Citation Metadata',
+      ...                 'fields': [
+      ...                     {'typeName': 'title', 'value': 'Test Title', 'multiple': False, 'typeClass': 'primitive'}
+      ...                 ]
+      ...             }
+      ...         }
+      ...     }
+      ... }
+      >>> get_formatted_metadata_message(metadata)
+      '<html>...</html>'
+  """
+
+  message = "<html>"
+  if metadata['datasetVersion']['license']:
+    message += "<b style=\"color:Black\">License Metadata:</b><ul>"
+    message += f"<li style=\"color:Gray\">Name: <i>{metadata['datasetVersion']['license']['name']}</i></li>"
+    message += f"<li style=\"color:Gray\">URI: <i>{metadata['datasetVersion']['license']['uri']}</i></li>"
+    message += "</ul>"
+  for _, metablock in metadata['datasetVersion']['metadataBlocks'].items():
+    message += f"<b style=\"color:Black\">{metablock['displayName']}:</b><ul>"
+    has_value = False
+    for field in metablock['fields']:
+      if field['value']:
+        has_value = has_value or len(field['value']) > 0
+        message += f"<b style=\"color:#737373\"><li>{adjust_type_name(field['typeName'])}:</li></b><ul>"
+        if field["multiple"] and field["typeClass"] == "compound":
+          for index, field_value in enumerate(field['value']):
+            message += f"<li style=\"color:Gray\">Item {index + 1}:</li><ul>"
+            for _, value in field_value.items():
+              message += f"<li style=\"color:Gray\">{adjust_type_name(value['typeName'])}: <i>{value['value']}</li></i>"
+            message += "</ul>"
+          message += "</ul>"
+        elif field["multiple"] and field["typeClass"] == "controlledVocabulary":
+          for field_value in field['value']:
+            message += f"<i style=\"color:Gray\"><li>{field_value}</li></i>"
+          message += "</ul>"
+        elif field["multiple"] and field["typeClass"] == "primitive":
+          for field_value in field['value']:
+            message += f"<i style=\"color:Gray\"><li>{field_value}</li></i>"
+          message += "</ul>"
+        else:
+          message += f"<i style=\"color:Gray\"><li>{field['value']}</li></i></ul>"
+    if not has_value:
+      message += "<li style=\"color:#737373\">No value</li></ul>"
+    message += "</ul>"
+  message += "</html>"
+  return message
```

### Comparing `pasta_eln-2.5.2b2/pasta_eln/fixedStringsJson.py` & `pasta_eln-2.5.3b1/pasta_eln/fixedStringsJson.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/gui.py` & `pasta_eln-2.5.3b1/pasta_eln/gui.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 from PySide6.QtCore import Qt, Slot, QCoreApplication  # pylint: disable=no-name-in-module
 from PySide6.QtGui import QIcon, QPixmap, QShortcut  # pylint: disable=no-name-in-module
 from PySide6.QtWidgets import QMainWindow, QApplication, QFileDialog, QMessageBox  # pylint: disable=no-name-in-module
 from qt_material import apply_stylesheet  # of https://github.com/UN-GCPDS/qt-material
 
 from pasta_eln import __version__
+from pasta_eln.GUI.dataverse.config_dialog import ConfigDialog
+from pasta_eln.GUI.dataverse.main_dialog import MainDialog
 from .GUI.body import Body
 from .GUI.config import Configuration
 from .GUI.form import Form
 from .GUI.projectGroup import ProjectGroup
 from .GUI.sidebar import Sidebar
 from .backend import Backend
 from .fixedStringsJson import shortcuts
@@ -35,27 +37,29 @@
   """ Graphical user interface includes all widgets """
 
   def __init__(self) -> None:
     # global setting
     super().__init__()
     venv = ' without venv' if sys.prefix == sys.base_prefix and 'CONDA_PREFIX' not in os.environ else ' in venv'
     self.setWindowTitle(f"PASTA-ELN {__version__}{venv}")
-    self.setWindowState(Qt.WindowMaximized)  # type: ignore
     resourcesDir = Path(__file__).parent / 'Resources'
     self.setWindowIcon(QIcon(QPixmap(resourcesDir / 'Icons' / 'favicon64.png')))
     self.backend = Backend()
     self.comm = Communicate(self.backend)
     self.comm.formDoc.connect(self.formDoc)
+    self.dataverseMainDialog: MainDialog | None = None
+    self.dataverseConfig: ConfigDialog | None = None
 
     # Menubar
     menu = self.menuBar()
     projectMenu = menu.addMenu("&Project")
-    Action('&Export .eln',                   self, [Command.EXPORT],         projectMenu)
-    Action('&Import .eln',                   self, [Command.IMPORT],         projectMenu)
+    Action('&Export project to .eln',        self, [Command.EXPORT],         projectMenu)
+    Action('&Import .eln',                   self, [Command.IMPORT],         projectMenu, shortcut='Ctrl+A')
     projectMenu.addSeparator()
+    Action('&Export all projects to .eln',   self, [Command.EXPORT_ALL],     projectMenu)
     Action('&Exit',                          self, [Command.EXIT],           projectMenu)
 
     viewMenu = menu.addMenu("&Lists")
     if hasattr(self.backend, 'db'):
       for docType, docLabel in self.comm.backend.db.dataLabels.items():
         if docType[0] == 'x' and docType[1] != '0':
           continue
@@ -72,14 +76,16 @@
     Action('&Project groups',                self, [Command.PROJECT_GROUP],   systemMenu)
     changeProjectGroups = systemMenu.addMenu("&Change project group")
     if hasattr(self.backend, 'configuration'):                            # not case in fresh install
       for name in self.backend.configuration['projectGroups'].keys():
         Action(name,                         self, [Command.CHANGE_PG, name], changeProjectGroups)
     Action('&Synchronize',                   self, [Command.SYNC],            systemMenu, shortcut='F5')
     Action('&Data hierarchy editor',         self, [Command.DATAHIERARCHY],        systemMenu, shortcut='F8')
+    Action('&Dataverse Configuration',         self, [Command.DATAVERSE_CONFIG],        systemMenu, shortcut='F10')
+    Action('&Upload to Dataverse',         self, [Command.DATAVERSE_MAIN],        systemMenu, shortcut='F11')
     systemMenu.addSeparator()
     Action('&Test extraction from a file',   self, [Command.TEST1],           systemMenu)
     Action('Test &selected item extraction', self, [Command.TEST2],           systemMenu, shortcut='F2')
     Action('Update &Extractor list',         self, [Command.UPDATE],          systemMenu)
     systemMenu.addSeparator()
     Action('&Configuration',                 self, [Command.CONFIG],          systemMenu, shortcut='Ctrl+0')
 
@@ -131,17 +137,25 @@
     action after clicking menu item
     """
     # file menu
     if command[0] is Command.EXPORT:
       if self.comm.projectID == '':
         showMessage(self, 'Error', 'You have to open a project to export', 'Warning')
         return
-      fileName = QFileDialog.getSaveFileName(self, 'Save data into .eln file', str(Path.home()), '*.eln')[0]
-      if fileName != '':
-        status = exportELN(self.comm.backend, self.comm.projectID, fileName)
+      fileName = QFileDialog.getSaveFileName(self, 'Save project into .eln file', str(Path.home()), '*.eln')[0]
+      if fileName != '' and hasattr(self.backend, 'db'):
+        docTypes = [i for i in self.comm.backend.db.dataLabels.keys() if i[0]!='x']
+        status = exportELN(self.comm.backend, [self.comm.projectID], fileName, docTypes)
+        showMessage(self, 'Finished', status, 'Information')
+    elif command[0] is Command.EXPORT_ALL:
+      fileName = QFileDialog.getSaveFileName(self, 'Save everything to .eln file', str(Path.home()), '*.eln')[0]
+      if fileName != '' and hasattr(self.backend, 'db'):
+        docTypes = [i for i in self.comm.backend.db.dataLabels.keys() if i[0]!='x']
+        allProjects = [i['id'] for i in self.comm.backend.db.getView('viewDocType/x0')]
+        status = exportELN(self.comm.backend, allProjects, fileName, docTypes)
         showMessage(self, 'Finished', status, 'Information')
     elif command[0] is Command.IMPORT:
       fileName = QFileDialog.getOpenFileName(self, 'Load data from .eln file', str(Path.home()), '*.eln')[0]
       if fileName != '':
         status = importELN(self.comm.backend, fileName)
         showMessage(self, 'Finished', status, 'Information')
         self.comm.changeSidebar.emit('redraw')
@@ -163,14 +177,20 @@
     elif command[0] is Command.SYNC:
       report = self.comm.backend.replicateDB(progressBar=self.sidebar.progress)
       showMessage(self, 'Report of syncronization', report, style='QLabel {min-width: 450px}')
     elif command[0] is Command.DATAHIERARCHY:
       dataHierarchyForm = DataHierarchyEditorDialog(self.comm.backend.db)
       dataHierarchyForm.instance.exec()
       restart()
+    elif command[0] is Command.DATAVERSE_CONFIG:
+      self.dataverseConfig = ConfigDialog()
+      self.dataverseConfig.show()
+    elif command[0] is Command.DATAVERSE_MAIN:
+      self.dataverseMainDialog = MainDialog(self.comm.backend)
+      self.dataverseMainDialog.show()
     elif command[0] is Command.TEST1:
       fileName = QFileDialog.getOpenFileName(self, 'Open file for extractor test', str(Path.home()), '*.*')[0]
       report = self.comm.backend.testExtractor(fileName, outputStyle='html')
       showMessage(self, 'Report of extractor test', report)
     elif command[0] is Command.TEST2:
       self.comm.testExtractor.emit()
     elif command[0] is Command.UPDATE:
@@ -186,15 +206,14 @@
     elif command[0] is Command.WEBSITE:
       webbrowser.open('https://pasta-eln.github.io/pasta-eln/')
     elif command[0] is Command.VERIFY_DB:
       report = self.comm.backend.checkDB(outputStyle='html', minimal=True)
       showMessage(self, 'Report of database verification', report, style='QLabel {min-width: 800px}')
     elif command[0] is Command.SHORTCUTS:
       showMessage(self, 'Keyboard shortcuts', shortcuts)
-
     elif command[0] is Command.RESTART:
       restart()
     else:
       print("**ERROR gui menu unknown:", command)
     return
 
 
@@ -247,14 +266,17 @@
   TEST2     = 10
   UPDATE    = 11
   CONFIG    = 12
   WEBSITE   = 13
   VERIFY_DB = 14
   SHORTCUTS = 15
   RESTART   = 16
+  EXPORT_ALL= 17
+  DATAVERSE_CONFIG = 18
+  DATAVERSE_MAIN = 19
 
 
 def startMain() -> None:
   """
   Main function to start GUI. Extra function is required to allow starting in module fashion
   """
   app, window = mainGUI()
```

### Comparing `pasta_eln-2.5.2b2/pasta_eln/guiCommunicate.py` & `pasta_eln-2.5.3b1/pasta_eln/guiCommunicate.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/guiStyle.py` & `pasta_eln-2.5.3b1/pasta_eln/guiStyle.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/handleDictionaries.py` & `pasta_eln-2.5.3b1/pasta_eln/handleDictionaries.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/inputOutput.py` & `pasta_eln-2.5.3b1/pasta_eln/inputOutput.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """Input and output functions towards the .eln file-format"""
-import os, json, shutil, logging, hashlib, copy
+import os, json, shutil, logging, hashlib, copy, uuid
 from typing import Any, Optional
 from pathlib import Path
 from datetime import datetime
 from zipfile import ZipFile, ZIP_DEFLATED
 import requests
 from anytree import Node
-from pasta_eln import __version__
+from pasta_eln import __version__, minisign
 from .backend import Backend
-from .miscTools import createDirName, generic_hash
-
+from .miscTools import createDirName, generic_hash, flatten, hierarchy
 # to discuss
 # - genre:docType, simulation, experiment/measurement;  status = Done, finished
-# - cathegory: project
+# - category: project
 # - root entry: authors list, single: @id; multiple authors
 #    - add several authors
 #    - one creator, multiple authors
 # - where to store additional metadata, not in ro-crate-metadata, separate files for each entry?
 #    - https://github.com/TheELNConsortium/TheELNFileFormat/issues/58
 # - how to store different versions?
 #    - history: last version
@@ -36,22 +35,24 @@
   '_attachments': None,
   '-attachment' : None,
   '-branch'     : None,
   '-client'     : None,
   '-date'       : 'dateModified',
   '-name'       : 'name',
   '-tags'       : 'keywords',
+  '-type'       : 'genre',
   'image'       : None,
   'comment'     : 'description',
   'content'     : 'text',
   'links'       : 'mentions',
   'shasum'      : None,
 }
 json2pasta:dict[str,Any] = {v:k for k,v in pasta2json.items() if v is not None}
 
+pastaNameTranslation = {'Rev':'Revision'}
 
 # Special terms in other ELNs: only add the ones that are required for function for PASTA
 specialTerms:dict[str,dict[str,str]] = {
     'elabFTW': {
       # 'elabid':'_id',
       # 'title':'-name',
       # 'tags':'-tags',
@@ -69,27 +70,27 @@
 }
 
 
 renameELN = {
   'https://kadi.iam.kit.edu':'Kadi4Mat'
 }
 
+METADATA_FILE = 'ro-crate-metadata.json'
+
 
 def tree(graph:dict[Any,Any]) -> str:
   """
   use metadata to create hierarchical tree structure in ascii
 
   Args:
     graph (dict): tree-graph to be plotted
 
   Returns:
     str: output of graph as a nice tree
   """
-  METADATA_FILE = 'ro-crate-metadata.json'
-
   def process_part(part:dict[Any,Any], level:int) -> str:
     """
     recursive function call to process this node of the tree-graph
 
     Args:
       part (dict): dictionary entry of this hasPart=part of a parent node; is a node by-itself
       level (int): hierarchy level
@@ -204,78 +205,42 @@
       Returns:
         bool: success of this function
       """
       addedDocs = 1
       if not isinstance(part, dict): #leave these tests in since other .elns might do funky stuff
         print("**ERROR in part",part)
         return False
-      logging.info('\nProcess: '+part['@id'])
+      print('\nProcess: '+part['@id'])
       # find next node to process
       docS = [i for i in graph if '@id' in i and i['@id']==part['@id']]
       if len(docS)!=1 or backend.cwd is None:
         print('**ERROR zero or multiple nodes with same id', docS,' or cwd is None in '+part['@id'])
         return -1
       doc, elnID, children, dataType = json2pastaFunction(copy.deepcopy(docS[0]))
       if elnName == 'PASTA ELN' and elnID.startswith('http') and ':/' in elnID:
         fullPath = None
       elif elnName == 'PASTA ELN':
-        fullPath = backend.basePath/elnID
+        fullPath = backend.basePath/( '/'.join(elnID.split('/')[1:]) )
       else:
         fullPath = backend.basePath/backend.cwd/elnID.split('/')[-1]
-      datasetIsFolder = False
-      if dataType.lower()=='dataset':
-        #print('  Dataset',elnID,dataType)
-        if elnName == 'PASTA ELN':
-          supplementalInfo = Path(dirName)/elnID/'metadata.json'
-        elif elnName == 'eLabFTW':
-          supplementalInfo = Path(dirName)/elnID/'export-elabftw.json'
-        else:
-          logging.info('No additional information in %s', elnName)
-          supplementalInfo = Path('')
-        if supplementalInfo.as_posix() in elnFile.namelist():
-          datasetIsFolder = True
-          with elnFile.open(supplementalInfo.as_posix()) as fIn:
-            jsonContent = json.loads( fIn.read() )
-            if isinstance(jsonContent, list):
-              jsonContent = jsonContent[0]
-            if elnName == 'PASTA ELN':
-              doc.update( jsonContent['__main__'] )
-            else:
-              doc[f'from {elnName}'] = jsonContent
-      if not datasetIsFolder:
-        #print('  ELSE ',elnID,dataType)
-        if elnName == 'PASTA ELN':
-          if elnID.endswith('data_hierarchy.json'):
-            return 0
-          parentIDList = [i['@id'] for i in graph if 'hasPart' in i and {'@id':'./'+elnID} in i['hasPart']]
-          if not parentIDList: #if no parent found, aka for remote data
-            parentIDList = [i['@id'] for i in graph if 'hasPart' in i and {'@id':elnID} in i['hasPart']]
-          if len(parentIDList)==1:
-            metadataPath = Path(dirName)/parentIDList[0]/'metadata.json'
-            with elnFile.open(metadataPath.as_posix()) as fIn:
-              metadataContent = json.loads( fIn.read() )
-              doc.update( metadataContent[doc['_id']] )
-        elif elnName == 'eLabFTW' and elnID.endswith('export-elabftw.json'):
-          return 0
-        elif fullPath is not None:
-          if f'{dirName}/{elnID}' in elnFile.namelist():  #could be directory, nothing to copy then
-            target = open(fullPath, "wb")
-            source = elnFile.open(f'{dirName}/{elnID}')
-            with source, target:  #extract one file to its target directly
-              shutil.copyfileobj(source, target)
-      # save
+      if fullPath is not None:
+        if f'{dirName}/{elnID}' in elnFile.namelist():  #could be directory, nothing to copy then
+          target = open(fullPath, "wb")
+          source = elnFile.open(f'{dirName}/{elnID}')
+          with source, target:  #extract one file to its target directly
+            shutil.copyfileobj(source, target)
       # ALL ELNS
       if '-tags' not in doc:
         doc['-tags'] = []
       else:
         doc['-tags'] = [i.strip() for i in doc['-tags'].split(',')]
       # PASTA_ELN
       if elnName == 'PASTA ELN':
         doc['-user'] = '_'
-        if datasetIsFolder and fullPath is not None:
+        if fullPath is not None:
           fullPath.mkdir(exist_ok=True)
           with open(fullPath/'.id_pastaELN.json', 'w', encoding='utf-8') as fOut:
             fOut.write(json.dumps(doc))
         elif fullPath is not None:
           if not fullPath.parent.is_dir():
             fullPath.parent.mkdir()
           if f'{dirName}/' + part['@id'][2:] in files:  #if a file is saved
@@ -342,72 +307,74 @@
 
 
 
 
 ##########################################
 ###               EXPORT               ###
 ##########################################
-def exportELN(backend:Backend, projectID:str, fileName:str='', dTypes:list[str]=[], verbose:bool=True) -> str:
+def exportELN(backend:Backend, projectIDs:list[str], fileName:str, dTypes:list[str], verbose:bool=False) -> str:
   """
   export eln to file
 
   Args:
     backend (backend): PASTA backend instance
-    projectID (str): docId of project
-    fileName (str): fileName which to use for saving; default='' saves in local folder
-    dTypes (list): list of strings which should be included in the output, alongside folders x0 & x1; empty list=everything is exported
+    projectIDs (list): list of docIds of projects
+    fileName (str): fileName which to use for saving
+    dTypes (list): list of strings which should be included in the output, alongside folders x0 & x1
     verbose (bool): verbose
 
   Returns:
     str: report of exportation
   """
-  # define initial information
-  docProject = backend.db.getDoc(projectID)
-  dirNameProject = docProject['-branch'][0]['path']
-  fileName = fileName or dirNameProject
-  fileName = fileName if fileName.endswith('.eln') else f'{fileName}.eln'
-  keysInSupplemental:set[str] = set()
-  filesNotInProject = []
-
-  def separate(doc: dict[str,Any]) -> tuple[str, dict[str,Any], dict[str,Any]]:
+  def separate(doc: dict[str,Any], dirNameProject: str) -> tuple[str, dict[str,Any], Optional[str]]:
     """ separate document into
     - main information (for all elns) and
     - supplemental information (specific to PastaELN)
+
+    Args:
+      doc (dict): document to separate into main and supplemental information
+      dirNameProject (str): name of the project directory
     """
     path =  f"{doc['-branch'][0]['path']}/" if doc['-type'][0][0]=='x' else doc['-branch'][0]['path']
-    pathUsed = True
+    docMain:dict[str,Any] = {}
+    docSupp:dict[str,Any] = {}
+    filesNotInData = None
     if path is None:
-      pathUsed = False
-      path = './'+dirNameProject+'/'+doc['_id']
-    if not path.startswith(dirNameProject) and not path.startswith('http') and pathUsed:
-      filesNotInProject.append(path)
-    if not path.startswith('http') and pathUsed:
-      path = f'./{path}'
-    docMain= {'@id': path}
-    docSupp = {}
+      path = dirNameProject+'/'+doc['_id']
+    elif not path.startswith(dirNameProject) and not path.startswith('http'):
+      filesNotInData = path  # files elsewhere, standardOperatingProcedures
+    if not path.startswith('http'):
+      docMain['@id'] = f'./{dirNameGlobal}/{path}'
+    else:
+      docMain['@id'] = path
     for key, value in doc.items():
       if key in pasta2json and pasta2json[key] is not None:
         docMain[pasta2json[key]] = value
       else:
         docSupp[key] = value
     # clean individual entries of docSupp: remove personal data
-    del docSupp['-user']
-    if 'image' in docSupp:
-      del docSupp['image']
-    if '_attachments' in docSupp:
-      del docSupp['_attachments']
-    docSupp['_id'] = docMain['identifier'] #ensure id is present in main and supplementary information
+    for k in ['-user', '-client', 'image', '_attachments']:
+      if 'image' in docSupp:
+        del docSupp[k]
     # clean individual entries of docMain
     if 'keywords' in docMain:
       docMain['keywords'] = ','.join(docMain['keywords'])
+    if docMain['genre'][0] == '-' or docMain['genre'][0][0]=='x':
+      del docMain['genre']
+    else:
+      docMain['genre'] = '/'.join(docMain['genre'])
     docMain = {k:v for k,v in docMain.items() if v}
-    nonlocal keysInSupplemental
-    keysInSupplemental = keysInSupplemental.union(docSupp)
-    return path, docMain, docSupp
-
+    # move docSupp into docMain
+    variableMeasured = []
+    for kObject, v in flatten(docSupp).items():
+      name = ' \u2192 '.join([i.replace('_','').replace('-','').capitalize() for i in str(kObject).split('.')])
+      name = pastaNameTranslation[name] if name in pastaNameTranslation else name
+      variableMeasured.append({'value':v, 'propertyID':kObject, 'name':name})
+    docMain['variableMeasured'] = variableMeasured
+    return path, docMain, filesNotInData
 
   def appendDocToGraph(graph: list[dict[str,Any]], doc: dict[str,Any]) -> None:
     """
     Append a document / dictionary to a graph
 
     Args:
       graph (list): graph to be appended to
@@ -415,179 +382,195 @@
     """
     idsInGraph = [i['@id'] for i in graph]
     if doc['@id'] not in idsInGraph:
       graph.append(doc)
     return
 
 
-  def iterateTree(nodeHier:Node, graph:list[dict[str,Any]]) -> Optional[str]:
+  def iterateTree(nodeHier:Node, graph:list[dict[str,Any]], dirNameProject:str) -> tuple[Optional[str], list[str]]:
     """
     Recursive function to translate the hierarchical node into a tree-node
 
     Args:
       nodeHier (Anytree.Node): anytree node
       graph    (list): list of nodes
+      dirNameProject (str): name of the project
 
     Returns:
       str: tree node
     """
     # separate into main and supplemental information
     doc = backend.db.getDoc(nodeHier.id)
-    path, docMain, docSupp = separate(doc)
-
+    path, docMain, filesNotInBranch = separate(doc, dirNameProject)
+    filesNotInProject:list[str] = [] if filesNotInBranch is None else [filesNotInBranch]
     hasPart = []
-    if (nodeHier.docType[0] not in dTypes) and nodeHier.docType[0][0]!='x' and len(dTypes)>0:
-      return None
+    if (nodeHier.docType[0] not in dTypes) and nodeHier.docType[0][0]!='x':
+      return (None, [])
     for child in nodeHier.children:
-      res = iterateTree(child, graph)
+      res, filesNotInSubbranch = iterateTree(child, graph, dirNameProject)
+      filesNotInProject += filesNotInSubbranch
       if res is not None:
         hasPart.append( res )
     if nodeHier.id[0]=='x':
-      pathMetadata = f'{path}metadata.json'
-      docMain['hasPart'] = [{'@id':pathMetadata}]
+      parts = []
       if hasPart:
-        docMain['hasPart'] += [{'@id':i} for i in hasPart]
-
-      metadata = {'__main__':docSupp}
-      hierStack = docSupp['-branch'][0]['stack']+[docSupp['_id']]
-      viewFull = backend.db.getView('viewHierarchy/viewHierarchyAll', startKey=' '.join(hierStack))
-      viewIDs = [i['id'] for i in viewFull if len(i['key'].split())==len(hierStack)+1 and i['value'][1][0][0]!='x']
-      for childID in viewIDs:
-        _, _, docChildSupp = separate(backend.db.getDoc(childID))
-        metadata[childID] = docChildSupp
-      zipContent = json.dumps(metadata)
-      roCrateMetadata = {'@id':pathMetadata,
-                         '@type':'File',
-                         'name':'export_metadata.json',
-                         'description':'JSON export',
-                         'encodingFormat':'application/json',
-                         'contentSize':str(len(zipContent)),
-                         'sha256':hashlib.sha256(zipContent.encode()).hexdigest(),
-                         'dateModified': docMain['dateModified']
-                         }
-      elnFile.writestr(f'{dirNameProject}/{pathMetadata[2:]}', zipContent)
-      docMain['@type'] = 'Dataset'
-      appendDocToGraph(graph, roCrateMetadata)
-
+        parts += [{'@id':i} for i in hasPart]
+      if parts:
+        docMain['hasPart'] = parts
     fullPath = backend.basePath/path
     if path is not None and fullPath.exists() and fullPath.is_file():
       with open(fullPath, 'rb') as fIn:
         fileContent = fIn.read()
         docMain['contentSize'] = str(len(fileContent))
         docMain['sha256']      = hashlib.sha256(fileContent).hexdigest()
       docMain['@type'] = 'File'
     elif path.startswith('http'):
-      response = requests.get(path.replace(':/','://'))
+      response = requests.get(path.replace(':/','://'), timeout=10)
       if response.ok:
         docMain['contentSize'] = str(response.headers['content-length'])
         docMain['sha256']      = hashlib.sha256(response.content).hexdigest()
       else:
         print(f'Info: could not get file {path}')
       docMain['@type'] = 'File'
     elif '@type' not in docMain:  #samples will be here
       docMain['@type'] = 'Dataset'
       docMain['@id'] = docMain['@id'] if docMain['@id'].endswith('/') else f"{docMain['@id']}/"
-
     appendDocToGraph(graph, docMain)
-    return docMain['@id']
+    return docMain['@id'], filesNotInProject
+
 
+  # define initial information
+  fileName = fileName if fileName.endswith('.eln') else f'{fileName}.eln'
+  filesNotInProject:list[str] = []
+  dirNameGlobal = fileName.split('/')[-1][:-4]
   # == MAIN FUNCTION ==
   logging.info('Create eln file %s',fileName)
   with ZipFile(fileName, 'w', compression=ZIP_DEFLATED) as elnFile:
-    # ------- Create main graph -------------------
-    listHier = backend.db.getHierarchy(projectID, allItems=False)
     graph: list[dict[str,Any]] = []
-    iterateTree(listHier, graph)  # create json object from anytree
+    dirNameProjects = []
+    for projectID in projectIDs:       #for each project
+      docProject = backend.db.getDoc(projectID)
+      dirNameProject = docProject['-branch'][0]['path']
+      dirNameProjects.append(dirNameProject)
 
+
+      # ------- Create main graph -------------------
+      listHier = backend.db.getHierarchy(projectID, allItems=False)
+      _, filesNotInProject = iterateTree(listHier, graph, dirNameProject)  # create json object from anytree
+
+      # ------------------ copy data-files --------------------------
+      # datafiles are already in the graph-graph: only copy and no addition to graph
+      for path, _, files in os.walk(backend.basePath/dirNameProject):
+        if '/.git' in path:  #if use datalad
+          continue
+        relPath = os.path.relpath(path, backend.basePath) #path of the folder
+        for iFile in files:                         #iterate through all files in folder
+          if iFile.startswith('.git') or iFile=='.id_pastaELN.json':
+            continue
+          elnFile.write(f'{path}/{iFile}', f'{dirNameGlobal}/{relPath}/{iFile}')
+      for path in set(filesNotInProject):  #set ensures that only added once
+        elnFile.write(str(backend.basePath/path), f'{dirNameGlobal}/{path}')
+
+    # FOR ALL PROJECTS
     # ------------------- create ro-crate-metadata.json header -----------------------
     index:dict[str,Any] = {}
     index['@context']= 'https://w3id.org/ro/crate/1.1/context'
     # master node ro-crate-metadata.json
     graphMaster:list[dict[str,Any]] = []
     graphMisc:list[dict[str,Any]] = []
-    masterNodeInfo = {
-        '@id': 'ro-crate-metadata.json',
-        '@type': 'CreativeWork',
-        'about': {
-            '@id': './'
-        },
-        'conformsTo': {
-            '@id': 'https://w3id.org/ro/crate/1.1'
-        },
-        'schemaVersion': 'v1.0',
-        'dateCreated': datetime.now().isoformat(),
-        'sdPublisher': {
-            '@type': 'Organization',
-            'name': 'PASTA ELN',
-            'logo':
-            'https://raw.githubusercontent.com/PASTA-ELN/desktop/main/pasta.png',
+    masterNodeInfo = {'@id': 'ro-crate-metadata.json', '@type': 'CreativeWork', 'about': {'@id': './'},
+        'conformsTo': {'@id': 'https://w3id.org/ro/crate/1.1'}, 'schemaVersion': 'v1.0', 'version': '1.0',
+        'datePublished':datetime.now().isoformat(), 'dateCreated': datetime.now().isoformat(),
+        'sdPublisher': {'@type': 'Organization', 'name': 'PASTA ELN',
+            'logo': 'https://raw.githubusercontent.com/PASTA-ELN/desktop/main/pasta.png',
             'slogan': 'The favorite ELN for experimental scientists',
-            'url': 'https://github.com/PASTA-ELN/',
-            'description': f'Version {__version__}',
-        },
-        'version': '1.0',
-        'datePublished':datetime.now().isoformat(),
-    }
+            'url': 'https://github.com/PASTA-ELN/', 'description': f'Version {__version__}'}}
     graphMaster.append(masterNodeInfo)
+    zipContent = json.dumps(backend.db.getDoc('-dataHierarchy-'))
+    dataHierarchyInfo = {'@id':  f'./{dirNameGlobal}/data_hierarchy.json', '@type': 'File',
+        'name':  'data structure', 'description': 'data structure / schema of the stored data',
+        'contentSize':str(len(zipContent)), 'sha256':hashlib.sha256(zipContent.encode()).hexdigest(),
+        'datePublished': datetime.now().isoformat()}
+    graphMisc.append(dataHierarchyInfo)
+    elnFile.writestr(f'{dirNameGlobal}/data_hierarchy.json', zipContent)
     authors = backend.configuration['authors']
-    masterNodeRoot = {
-        '@id': './',
-        '@type': 'Dataset',
-        'hasPart': [
-            {'@id': f'./{dirNameProject}/'}
-        ],
-        'name': 'Exported from PASTA ELN',
-        'description': 'Exported content from PASTA ELN',
-        'license':'CC BY 4.0',
-        'author': [{
-            'firstName': authors[0]['first'],
-            'surname': authors[0]['last'],
-            'title': authors[0]['title'],
-            'emailAddress': authors[0]['email'],
+    masterParts = [{'@id': f'./{dirNameGlobal}/{i}/'} for i in dirNameProjects] + [{'@id': f'./{dirNameGlobal}/data_hierarchy.json'}]
+    masterNodeRoot = {'@id': './', '@type': 'Dataset', 'hasPart': masterParts,
+        'name': 'Exported from PASTA ELN', 'description': 'Exported content from PASTA ELN',
+        'license':'CC BY 4.0', 'datePublished':datetime.now().isoformat(),
+        'author': [{'firstName': authors[0]['first'], 'surname': authors[0]['last'],
+            'title': authors[0]['title'], 'emailAddress': authors[0]['email'],
             'ORCID': authors[0]['orcid'],
-            'affiliation': [{
-                'organization': authors[0]['organizations'][0]['organization'],
-                'RORID': authors[0]['organizations'][0]['rorid'],
-            }],
-        }],
-        'datePublished':datetime.now().isoformat(),
-    }
+            'affiliation': [{'organization': authors[0]['organizations'][0]['organization'],
+                'RORID': authors[0]['organizations'][0]['rorid']}]
+        }]}
     graphMaster.append(masterNodeRoot)
-    zipContent = json.dumps(backend.db.getDoc('-dataHierarchy-'))
-    dataHierarchyInfo = {
-        '@id':  f'./{dirNameProject}/data_hierarchy.json',
-        '@type': 'File',
-        'name':  'data structure',
-        'description': 'data structure / schema of the stored data',
-        'contentSize':str(len(zipContent)),
-        'sha256':hashlib.sha256(zipContent.encode()).hexdigest(),
-        'datePublished': datetime.now().isoformat()
-    }
-    graphMisc.append(dataHierarchyInfo)
-    graph[-1]['hasPart'] += [{'@id': f'./{dirNameProject}/data_hierarchy.json'}]
-    elnFile.writestr(f'{dirNameProject}/{dirNameProject}/data_hierarchy.json', zipContent)
-
-    # ------------------ copy data-files --------------------------
-    # datafiles are already in the graph-graph: only copy and no addition to graph
-    for path, _, files in os.walk(backend.basePath/dirNameProject):
-      if '/.git' in path:  #if use datalad
-        continue
-      relPath = os.path.relpath(path, backend.basePath) #path of the folder
-      for iFile in files:                         #iterate through all files in folder
-        if iFile.startswith('.git') or iFile=='.id_pastaELN.json':
-          continue
-        elnFile.write(f'{path}/{iFile}', f'{dirNameProject}/{relPath}/{iFile}')
-    for path in set(filesNotInProject):  #set ensures that only added once
-      elnFile.write(str(backend.basePath/path), f'{dirNameProject}/{path}')
 
     #finalize file
     index['@graph'] = graphMaster+graph+graphMisc
-    elnFile.writestr(f'{dirNameProject}/ro-crate-metadata.json', json.dumps(index))
-    if verbose:
-      print(json.dumps(index, indent=3))
+    elnFile.writestr(f'{dirNameGlobal}/ro-crate-metadata.json', json.dumps(index))
+    # if verbose:
+    #   print(json.dumps(index, indent=3))
+
+    #sign file
+    if 'signingKeyPair' not in backend.configuration:  #create a key-pair of secret and public key and save it locally
+      keyPairRaw = minisign.KeyPair.generate()
+      keyPair    = {'id':str(uuid.uuid4()), 'secret':bytes(keyPairRaw.secret_key).decode(), 'public':bytes(keyPairRaw.public_key).decode()}
+      backend.configuration['signingKeyPair'] = keyPair
+      with open(Path.home()/'.pastaELN.json', 'w', encoding='utf-8') as fConf:
+        fConf.write(json.dumps(backend.configuration,indent=2))
+    keyPair = backend.configuration['signingKeyPair']
+    secretKey = minisign.SecretKey.from_bytes(keyPair['secret'].encode())
+    comment   = {'pubkey_url':f'https://raw.githubusercontent.com/PASTA-ELN/Signatures/main/{keyPair["id"]}.pub',
+                 'name': f"{backend.configuration['authors'][0]['title']} {backend.configuration['authors'][0]['first']} {backend.configuration['authors'][0]['last']}",
+                 'email': backend.configuration['authors'][0]['email'],
+                 'orcid': backend.configuration['authors'][0]['orcid']}
+    signature = secretKey.sign(json.dumps(index).encode(), trusted_comment=json.dumps(comment))
+    elnFile.writestr(f'{dirNameGlobal}/ro-crate-metadata.json.minisig', bytes(signature).decode())
+    elnFile.writestr(f'{dirNameGlobal}/ro-crate.pubkey', keyPair['public'])
   # end writing zip file
+
   # temporary json output
-  # with open(fileName[:-3]+'json','w', encoding='utf-8') as fOut:
-  #   fOut.write( json.dumps(index, indent=2) )
-  keysInSupplemental = {i for i in keysInSupplemental if i not in pasta2json}
-  logging.info('Keys in supplemental information'+', '.join(keysInSupplemental))
+  if verbose:
+    with open(fileName[:-3]+'json','w', encoding='utf-8') as fOut:
+      fOut.write( json.dumps(index, indent=2) )
   return f'Success: exported {len(graph)} graph-nodes into file {fileName}'
+
+
+def testSignature(fileName:str) -> bool:
+  """ Test if signature is valid
+
+  Args:
+    fileName (str): file name to test against
+
+  Returns:
+    bool: success / failure of test
+  """
+  print(f'Test signature of : {fileName}')
+  with ZipFile(fileName, 'r', compression=ZIP_DEFLATED) as elnFile:
+    metadataJsonFile = [i for i in elnFile.namelist() if i.endswith(METADATA_FILE)][0]
+    with elnFile.open(metadataJsonFile) as fIn:
+      metadataData = fIn.read()
+    dirName          = metadataJsonFile.split('/')[0]
+    signatureFile    = f'{dirName}/{METADATA_FILE}.minisig'
+    with elnFile.open(signatureFile) as fIn:
+      signature = minisign.Signature.from_bytes(fIn.read())
+    publicKeyFile    = f'{dirName}/ro-crate.pubkey'
+    with elnFile.open(publicKeyFile) as fIn:
+      publicKey = minisign.PublicKey.from_bytes(fIn.read())
+    try:
+      publicKey.verify(metadataData, signature)
+      if 'pubkey_url' in signature.trusted_comment:
+        path = json.loads(signature.trusted_comment)['pubkey_url']
+        response = requests.get(path, timeout=10)
+        if response.ok:
+          pubKeyRemote = response.content.strip()
+          if pubKeyRemote.decode() == str(bytes(publicKey))[2:-1]:
+            print('Success: remote and local key match')
+          else:
+            print('**ERROR remote and local key differ')
+            raise minisign.VerifyError
+      print('Signature is acceptable:\n', json.dumps(json.loads(signature.trusted_comment), indent=2))
+      return True
+    except minisign.VerifyError:
+      print('**ERROR VERIFICATION ERROR')
+    return False
```

### Comparing `pasta_eln-2.5.2b2/pasta_eln/installationTools.py` & `pasta_eln-2.5.3b1/pasta_eln/installationTools.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
   Args:
     cmdLine (list): list of command line sections runAsAdmin(["c:\\Windows\\notepad.exe"])
   '''
   import win32con, win32event, win32process
   from win32com.shell.shell import ShellExecuteEx
   from win32com.shell import shellcon
-  procInfo = ShellExecuteEx(nShow=win32con.SW_SHOWNORMAL,
+  procInfo = ShellExecuteEx(nShow=win32con.SW_SHOWNORMAL,   # type: ignore[call-arg]
                             fMask=shellcon.SEE_MASK_NOCLOSEPROCESS,
                             lpVerb='runas',  # causes UAC elevation prompt.
                             lpFile= f'"{cmdLine[0]}"',
                             lpParameters=" ".join(cmdLine[1:]))
   procHandle = procInfo['hProcess']
   _ = win32event.WaitForSingleObject(procHandle, win32event.INFINITE)
   _   = win32process.GetExitCodeProcess(procHandle)
@@ -384,14 +384,16 @@
   backend.changeHierarchy(None)
   semStepID = backend.addData('x1',    {'-name': 'Data files'})
   if callbackPercent is not None:
     callbackPercent(11)
   backend.changeHierarchy(semStepID)
   if backend.cwd is not None:
     semDirName = backend.basePath/backend.cwd
+  else:
+    return "**ERROR: backend is incorrect"
   backend.changeHierarchy(None)
   outputString(outputFormat,'info',backend.outputHierarchy())
   if callbackPercent is not None:
     callbackPercent(12)
   logging.info('Finished project planning')
 
   ### TEST PROCEDURES
```

### Comparing `pasta_eln-2.5.2b2/pasta_eln/miscTools.py` & `pasta_eln-2.5.3b1/pasta_eln/miscTools.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """ Misc functions that do not require instances """
 import os, uuid, logging, traceback, json, sys, re
-from typing import Any
+from collections.abc import Mapping
+from typing import Any, Union
 from io import BufferedReader
 from urllib import request
 from pathlib import Path
 from re import sub, match
 import platform
 from .handleDictionaries import dict2ul
 
@@ -163,14 +164,15 @@
       logging.error('Could not download content / hashing issue '+path.as_posix().replace(':/','://')+'\n'+\
         traceback.format_exc())
       return ''
   if path.is_dir():
     raise ValueError(f'This seems to be a directory {path.as_posix()}')
   if forceFile and path.is_symlink():
     path = path.resolve()
+  shasum = ''
   if path.is_symlink():    #if link, hash the link
     shasum = symlink_hash(path)
   elif path.is_file():  #Local file
     with open(path, 'rb') as stream:
       shasum = blob_hash(stream, path.stat().st_size)
   return shasum
 
@@ -347,7 +349,104 @@
     return
   def show(self) -> None:
     """ show progress bar """
     return
   def hide(self) -> None:
     """ hide progress bar """
     return
+
+
+# adapted from flatten-dict https://github.com/ianlini/flatten-dict
+# - reduce dependencies and only have python 3 code
+# - add conversion of dict to list if applicable
+def flatten(d:Mapping[Any,Any]) -> dict[object, Any]:
+  """Flatten `Mapping` object.
+
+  Args:
+    d : dict-like object
+        The dict that will be flattened.
+
+  Returns:
+    flat_dict : dict
+  """
+  enumerate_types=(list,)
+  flatten_types = (Mapping,) + enumerate_types
+  flat_dict = {}
+
+  def dot_reducer(k1:object, k2:object) -> Union[str, object]:
+    """ Reducer function """
+    if k1 is None:
+      return k2
+    return f"{k1}.{k2}"
+
+  def _flatten(_d:Union[Mapping[Any, Any], list[Any]], depth:int, parent:object=None) -> bool:
+    """ Recursive function """
+    key_value_iterable = (enumerate(_d) if isinstance(_d, enumerate_types) else _d.items())
+    has_item = False
+    for key, value in key_value_iterable:
+      has_item = True
+      flat_key = dot_reducer(parent, key)
+      if isinstance(value, flatten_types):
+        # recursively build the result
+        has_child = _flatten(value, depth=depth + 1, parent=flat_key)
+        if has_child or not isinstance(value, ()): # ignore the key in this level because it already has child key or its value is empty
+          continue
+      # add an item to the result
+      if flat_key in flat_dict:
+        raise ValueError(f"duplicated key '{flat_key}'")
+      flat_dict[flat_key] = value
+    return has_item
+
+  # start recursive calling
+  _flatten(d, depth=1)
+  return flat_dict
+
+
+def hierarchy(d:dict[str,str]) -> dict[str,Any]:
+  """Reverse flattening of dict-like object
+
+  Args:
+    d : dict-like object
+      The dict that will be reversed
+
+  Returns
+    normalDict : dict
+  """
+  def dot_splitter(flat_key:str) -> tuple[str, ...]:
+    """ split using the . symbol """
+    keys = tuple(flat_key.split("."))
+    return keys
+
+  def nested_set_dict(d:dict[str,Any], keys:tuple[str, ...], value:Any) -> None:
+    """Set a value to a sequence of nested keys
+
+    Args:
+      d : Mapping
+      keys : Sequence[str]
+      value : Any
+    """
+    key = keys[0]
+    if len(keys) == 1:
+      if key in d:
+        raise ValueError(f"duplicated key '{key}'")
+      d[key] = value
+      return
+    d = d.setdefault(key, {})
+    nested_set_dict(d, keys[1:], value)
+    return
+
+  def dict2list(d:dict[str,Any]) -> Union[list[dict[str,Any]], dict[str,Any]]:
+    """ convert a dictionary to list if all keys are numbers """
+    for key in d.keys():
+      if isinstance(d[key], dict):
+        d[key] = dict2list(d[key])
+    if all(i.isdigit() for i in d.keys()):
+      d = list(d.values())                                                           # type: ignore[assignment]
+    return d
+
+  # start recursion
+  normalDict:dict[str,Any] = {}
+  for flat_key, value in d.items():
+    key_tuple = dot_splitter(flat_key)
+    nested_set_dict(normalDict, key_tuple, value)
+  normalDict =  dict2list(normalDict)                                                # type: ignore[assignment]
+  return normalDict
```

### Comparing `pasta_eln-2.5.2b2/pasta_eln/mixin_cli.py` & `pasta_eln-2.5.3b1/pasta_eln/mixin_cli.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/printer.py` & `pasta_eln-2.5.3b1/pasta_eln/printer.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,36 +8,37 @@
   - img = qrcode.make("testString",error_correction=qrcode.constants.ERROR_CORRECT_M)
   - or ERROR-CORRECT_H for better errorcorrection
   Sizes:
   - QR code size 1.5-2cm
   - with frame 2.25-3cm
   - Page size 18x27cm; 6x9 = 54
   """
-  import qrcode
-  import numpy as np
-  from PIL import Image
-  from commonTools import commonTools as cT  # don't import globally since it disturbs translation
-  img = qrcode.make(cT.uuidv4(),
-                    error_correction=qrcode.constants.ERROR_CORRECT_M)
-  size = img.size[0]
-  hSize = 6*size
-  vSize = 9*size
-  new_im = Image.new('RGB', (hSize, vSize))
-  for i in np.arange(0, hSize, size):
-    for j in np.arange(0, vSize, size):
-      img = qrcode.make(cT.uuidv4(),
-                        error_correction=qrcode.constants.ERROR_CORRECT_M)
-      # if j==0:  #make top row yellow
-      #   data = np.array(img.convert("RGB"))
-      #   red, green, blue = data.T
-      #   mask = (red==255) & (green==255) & (blue==255)
-      #   data[:,:,:][mask.T]=(255,255,0)
-      #   img = Image.fromarray(data)
-      new_im.paste(img, (i, j))
-  new_im.save(fileName)
+  # this code currently does not work, but not used anyhow. Have to fix it in the future
+
+  # import qrcode
+  # import numpy as np
+  # from PIL import Image
+  # #from commonTools import commonTools as cT  # don't import globally since it disturbs translation
+  # #img = qrcode.make(cT.uuidv4(), error_correction=qrcode.constants.ERROR_CORRECT_M)
+  # size = -1 # img.size[0]
+  # hSize = 6*size
+  # vSize = 9*size
+  # new_im = Image.new('RGB', (hSize, vSize))
+  # for i in np.arange(0, hSize, size):
+  #   for j in np.arange(0, vSize, size):
+  #     #img = qrcode.make(cT.uuidv4(), error_correction=qrcode.constants.ERROR_CORRECT_M)
+  #     # if j==0:  #make top row yellow
+  #     #   data = np.array(img.convert("RGB"))
+  #     #   red, green, blue = data.T
+  #     #   mask = (red==255) & (green==255) & (blue==255)
+  #     #   data[:,:,:][mask.T]=(255,255,0)
+  #     #   img = Image.fromarray(data)
+  #     # new_im.paste(img, (i, j))
+  #     print(i,j)
+  # new_im.save(fileName)
   return
 
 
 def printQRcodeSticker(codes:list[list[str]]=[],
                        page:dict[str,Any]={'size':[991,306], 'tiles':2, 'margin': 60, 'font':40},
                        printer:dict[str,str]={'model':'QL-700', 'dev':'0x04f9:0x2042/3', 'size':'29x90'}) -> None:
   """
@@ -52,43 +53,46 @@
 
   Printer:
    - model: brother label printer QL-700
    - dev: device in idVendor:idProduct/iSerial
      execute 'lsusb -v'; find printer
    - size: label size in mm
   """
-  import qrcode, tempfile
-  import numpy as np
-  from PIL import Image, ImageDraw, ImageFont
-  fnt = ImageFont.truetype("arial.ttf", page['font'])
-  offset    = int((page['size'][0]+page['margin'])/page['tiles'])
-  qrCodeSize= min(offset-page['font']-page['margin'], page['size'][1])
-  print("Effective label size",page['size'], "offset",offset, 'qrCodeSize',qrCodeSize)
-  cropQRCode  = 40         #created by qrcode library
-  image = Image.new('RGBA', page['size'], color=(255,255,255,255) )
-  for numCodes, idx in enumerate(range(page['tiles'])):
-    codeI, text = codes[idx] if idx<len(codes) else ('', '')
-    if len(codeI)==0:
-      codeI = uuid.uuid4().hex
-    # add text
-    width, height = fnt.getsize(text)
-    txtImage = Image.new('L', (width, height), color=255)
-    d = ImageDraw.Draw(txtImage)
-    d.text( (0, 0), text,  font=fnt, fill=0)
-    txtImage=txtImage.rotate(90, expand=1)
-    if width>page['size'][1]:  #shorten it to fit into height
-      txtImage=txtImage.crop((0,width-page['size'][1],height,width))
-    image.paste(txtImage, (numCodes*offset+qrCodeSize-4, int((page['size'][1]-txtImage.size[1])/2)   ))
-    # add qrcode
-    qrCode = qrcode.make(codeI, error_correction=qrcode.constants.ERROR_CORRECT_M)
-    qrCode = qrCode.crop((cropQRCode, cropQRCode, qrCode.size[0]-cropQRCode, qrCode.size[0]-cropQRCode))
-    qrCode = qrCode.resize((qrCodeSize, qrCodeSize))
-    image.paste(qrCode, (numCodes*offset, int((page['size'][1]-qrCodeSize)/2)))
-  tmpFileName = tempfile.gettempdir()+os.sep+'tmpQRcode.png'
-  print('Create temp-file',tmpFileName)
-  image.save(tmpFileName)
-  cmd = 'brother_ql -b pyusb -m '+printer['model']+' -p usb://'+printer['dev']+' print -l '+printer['size']+' -r auto '+tmpFileName
-  reply = os.system(cmd)
-  if reply>0:
-    print('**ERROR mpq01: Printing error')
-    image.show()
+  # this code currently does not work, but not used anyhow. Have to fix it in the future
+
+  # import qrcode, tempfile
+  # import numpy as np
+  # from PIL import Image, ImageDraw, ImageFont
+  # # fnt = ImageFont.truetype("arial.ttf", page['font'])
+  # offset    = int((page['size'][0]+page['margin'])/page['tiles'])
+  # qrCodeSize= min(offset-page['font']-page['margin'], page['size'][1])
+  # print("Effective label size",page['size'], "offset",offset, 'qrCodeSize',qrCodeSize)
+  # cropQRCode  = 40         #created by qrcode library
+  # image = Image.new('RGBA', page['size'], color=(255,255,255,255) )
+  # for numCodes, idx in enumerate(range(page['tiles'])):
+  #   codeI, text = codes[idx] if idx<len(codes) else ('', '')
+  #   print(text)
+  #   if len(codeI)==0:
+  #     codeI = uuid.uuid4().hex
+  #   # add text: temporary comment out since library updated and functions changed
+  #   # width, height = fnt.getsize(text)
+  #   # txtImage = Image.new('L', (width, height), color=255)
+  #   # d = ImageDraw.Draw(txtImage)
+  #   # d.text( (0, 0), text,  font=fnt, fill=0)
+  #   # txtImage=txtImage.rotate(90, expand=1)
+  #   # if width>page['size'][1]:  #shorten it to fit into height
+  #   #   txtImage=txtImage.crop((0,width-page['size'][1],height,width))
+  #   # image.paste(txtImage, (numCodes*offset+qrCodeSize-4, int((page['size'][1]-txtImage.size[1])/2)   ))
+  #   # add qrcode
+  #   qrCode = qrcode.make(codeI, error_correction=qrcode.constants.ERROR_CORRECT_M)
+  #   qrCode = qrCode.crop((cropQRCode, cropQRCode, qrCode.size[0]-cropQRCode, qrCode.size[0]-cropQRCode))
+  #   qrCode = qrCode.resize((qrCodeSize, qrCodeSize))
+  #   image.paste(qrCode, (numCodes*offset, int((page['size'][1]-qrCodeSize)/2)))
+  # tmpFileName = tempfile.gettempdir()+os.sep+'tmpQRcode.png'
+  # print('Create temp-file',tmpFileName)
+  # image.save(tmpFileName)
+  # cmd = 'brother_ql -b pyusb -m '+printer['model']+' -p usb://'+printer['dev']+' print -l '+printer['size']+' -r auto '+tmpFileName
+  # reply = os.system(cmd)
+  # if reply>0:
+  #   print('**ERROR mpq01: Printing error')
+  #   image.show()
   return
```

### Comparing `pasta_eln-2.5.2b2/pasta_eln/serverActions.py` & `pasta_eln-2.5.3b1/pasta_eln/serverActions.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,15 @@
   authUser = requests.auth.HTTPBasicAuth(userName, userPassword)
   if auth is None:
     userDB = [userName.replace('.','_')]
   else:
     # test if configuration corresponds to naming convention
     users     = listUsers(url, auth, False)
     userDB    = [i[:-2] for i in users[userName]]  #list
-    databases = listDB(url, auth, False)
+  databases = listDB(url, auth, False)
   for iDB in userDB:
     if auth is not None:
       write = databases[iDB][0][0]
       read  = databases[iDB][1][0]
       authen= databases[iDB][2]
       if write.endswith('-W') and read.endswith('-R') and authen.endswith('-W') and \
         write[:-2] == read[:-2] and write[:-2] == authen[:-2]:
@@ -377,15 +377,15 @@
         print('Special database', database, ': Nothing to do')
       else:
         print('Backup normal database ',database)
         resp = requests.get(f'http://{location}:5984/{database}/_all_docs', headers=headers, auth=authUser, timeout=10)
         for item in resp.json()['rows']:
           docID = item['id']
           doc   = requests.get(f'http://{location}:5984/{database}/{docID}', headers=headers, auth=authUser, timeout=10).json()
-          zipFile.writestr(f'{zipFileName}/{database}/{docID}', json.dumps(doc))
+          zipFile.writestr(f'{zipFileName}/research/{docID}', json.dumps(doc))
           if '_attachments' in doc:
             for att in doc['_attachments']:
               docAttach = requests.get(f'http://{location}:5984/{database}/{docID}/{att}',
                                         headers=headers, auth=authUser, timeout=10).json()
               zipFile.writestr(f'{zipFileName}/{database}/{docID}_attach/{att}', json.dumps(docAttach))
         #_design/authentication is automatically included
         #_security
@@ -444,21 +444,21 @@
     for idx, i in enumerate(possFiles):
       print(f'[{str(idx + 1)}] {i}')
     fileChoice = input(f'Which file to use for restored? (1-{len(possFiles)}) ')
     fileName = possFiles[int(fileChoice)-1] if fileChoice else possFiles[0]
   # use information
   authUser = requests.auth.HTTPBasicAuth(userName, password)
   with ZipFile(fileName, 'r', compression=ZIP_DEFLATED) as zipFile:
-    files = zipFile.namelist()
+    files = [i for i in zipFile.namelist() if not i.endswith('/')]  #only files, no folders
     #first run through: create documents and design documents
     for fileI in files:
       fileParts = fileI.split('/')[1:]
       if fileParts==['pastaELN.json']: #do not recreate file, it is only there for manual recovery
         continue
-      if len(fileParts)!=2 or fileParts[-1]=='':
+      if len(fileParts)!=2:
         print(f"**ERROR: Cannot process file {fileI}: does not have 1+2 parts")
         continue
       database = fileParts[0]
       docID = fileParts[1]
       if docID.endswith('_attach'):
         continue #Do in second loop
       #test if database is exists: create otherwise
@@ -482,17 +482,17 @@
           if resp.ok:
             print('Saved document:', database, docID)
           else:
             print("**ERROR: could not save document:",resp.reason, database, docID, '\n', doc)
     #second run through: create attachments
     for fileI in files:
       fileParts = fileI.split('/')[1:]
-      if fileParts==['pastaELN.json']: #do not recreate file, it is only there for manual recovery
+      if fileParts==['pastaELN.json'] or fileParts[-1]=='' or fileParts[-2]=='_design': #do not recreate file, it is only there for manual recovery
         continue
-      if len(fileParts)!=2 or fileParts[-1]=='':
+      if len(fileParts)!=2:
         print(f"**ERROR-Attachment: Cannot process file {fileI}: does not have 1+2 parts")
         continue
       database = fileParts[0]
       docID = fileParts[1]
       if not docID.endswith('_attach'):
         continue #Did already in the first loop
       #test if attachment exists: create otherwise
```

### Comparing `pasta_eln-2.5.2b2/pasta_eln/utils.py` & `pasta_eln-2.5.3b1/pasta_eln/utils.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln/webclient/http_client.py` & `pasta_eln-2.5.3b1/pasta_eln/webclient/http_client.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/pasta_eln.egg-info/PKG-INFO` & `pasta_eln-2.5.3b1/pasta_eln.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasta_eln
-Version: 2.5.2b2
+Version: 2.5.3b1
 Summary: The favorite ELN for experimental scientists
 Home-page: https://pasta-eln.github.io/
 Author: The PASTA-ELN Team and Steffen Brinckmann
 Author-email: sbrinckm@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pasta_eln-2.5.2b2/pasta_eln.egg-info/SOURCES.txt` & `pasta_eln-2.5.3b1/pasta_eln.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -108,14 +108,17 @@
 pasta_eln/GUI/dataverse/config_dialog_base.py
 pasta_eln/GUI/dataverse/config_dialog_base.ui
 pasta_eln/GUI/dataverse/controlled_vocab_frame.py
 pasta_eln/GUI/dataverse/dialog_extension.py
 pasta_eln/GUI/dataverse/edit_metadata_dialog.py
 pasta_eln/GUI/dataverse/edit_metadata_dialog_base.py
 pasta_eln/GUI/dataverse/edit_metadata_dialog_base.ui
+pasta_eln/GUI/dataverse/edit_metadata_summary_dialog.py
+pasta_eln/GUI/dataverse/edit_metadata_summary_dialog_base.py
+pasta_eln/GUI/dataverse/edit_metadata_summary_dialog_base.ui
 pasta_eln/GUI/dataverse/main_dialog.py
 pasta_eln/GUI/dataverse/main_dialog_base.py
 pasta_eln/GUI/dataverse/main_dialog_base.ui
 pasta_eln/GUI/dataverse/primitive_compound_controlled_frame_base.py
 pasta_eln/GUI/dataverse/primitive_compound_controlled_frame_base.ui
 pasta_eln/GUI/dataverse/primitive_compound_frame.py
 pasta_eln/GUI/dataverse/project_item_frame_base.py
@@ -142,19 +145,27 @@
 pasta_eln/dataverse/config_model.py
 pasta_eln/dataverse/data_upload_task.py
 pasta_eln/dataverse/database_api.py
 pasta_eln/dataverse/database_error.py
 pasta_eln/dataverse/dataset-create-new-all-default-fields.json
 pasta_eln/dataverse/generic_task_object.py
 pasta_eln/dataverse/incorrect_parameter_error.py
+pasta_eln/dataverse/progress_updater_thread.py
 pasta_eln/dataverse/project_model.py
 pasta_eln/dataverse/task_thread_extension.py
 pasta_eln/dataverse/upload_model.py
 pasta_eln/dataverse/upload_queue_manager.py
 pasta_eln/dataverse/upload_status_values.py
 pasta_eln/dataverse/utils.py
+pasta_eln/minisign/LICENSE
+pasta_eln/minisign/README.rst
+pasta_eln/minisign/__init__.py
+pasta_eln/minisign/exceptions.py
+pasta_eln/minisign/helpers.py
+pasta_eln/minisign/minisign.py
+pasta_eln/minisign/requirements.txt
 pasta_eln/webclient/__init__.py
 pasta_eln/webclient/http_client.py
 tests/test_01_3Projects.py
-tests/test_02_3Projects_ExportImport.py
-tests/test_50_importOthers.py
+tests/test_02_3Projects_ExportImport1.py
+tests/test_03_3Projects_ExportImport3.py
 tests/test_99_3Projects.py
```

### Comparing `pasta_eln-2.5.2b2/setup.cfg` & `pasta_eln-2.5.3b1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -63,29 +63,29 @@
 
 [mypy]
 check_untyped_defs = true
 disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_untyped_defs = true
 warn_redundant_casts = true
-warn_unused_ignores = true
 ignore_missing_imports = true
 exclude = (?x)(
 	pasta_eln/GUI/data_hierarchy/create_type_dialog_base.py
 	|pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog_base.py
 	|pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog_base.py
 	|pasta_eln/GUI/dataverse/completed_upload_task.py
 	|pasta_eln/GUI/dataverse/completed_uploads_base.py
 	|pasta_eln/GUI/dataverse/config_dialog_base.py
 	|pasta_eln/GUI/dataverse/edit_metadata_dialog_base.py
 	|pasta_eln/GUI/dataverse/main_dialog_base.py
 	|pasta_eln/GUI/dataverse/primitive_compound_controlled_frame_base.py
 	|pasta_eln/GUI/dataverse/project_item_frame_base.py
 	|pasta_eln/GUI/dataverse/upload_config_dialog_base.py
 	|pasta_eln/GUI/dataverse/upload_widget_base.py
+	|pasta_eln/GUI/dataverse/edit_metadata_summary_dialog_base.py
 	|pasta_eln/Extractors)
 
 [mypy-pasta_eln/GUI/data_hierarchy.*]
 follow_imports = skip
 
 [mypy-pasta_eln/GUI/dataverse.*]
 follow_imports = skip
```

### Comparing `pasta_eln-2.5.2b2/tests/test_01_3Projects.py` & `pasta_eln-2.5.3b1/tests/test_01_3Projects.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.2b2/tests/test_02_3Projects_ExportImport.py` & `pasta_eln-2.5.3b1/tests/test_02_3Projects_ExportImport1.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 #!/usr/bin/python3
 """TEST using the FULL set of python-requirements: create 3 projects; simplified form of testTutorialComplex """
-import os, shutil, logging,  json
+import os, shutil, logging, json
 import warnings
 import unittest
+from typing import Any
 from pathlib import Path
-from zipfile import ZIP_DEFLATED
-from zipfile import Path as ZPath
-from zipfile import ZipFile
+from zipfile import ZipFile, ZIP_DEFLATED
 import pytest
 from pasta_eln.backend import Backend
 from pasta_eln.inputOutput import exportELN, importELN
 from pasta_eln.miscTools import outputString
-from pasta_eln.miscTools import DummyProgressBar
+
 
 class TestStringMethods(unittest.TestCase):
   """
   derived class for this test
   """
   def __init__(self, *args, **kwargs):
     super().__init__(*args, **kwargs)
@@ -24,19 +23,22 @@
 
   @pytest.mark.skip(
     reason="Disabled for github since cannot create couchdb instance during actions")
   def test_main(self):
     """
     main function
     """
-
-
-    def test_A_File(fileName):
+    ###### BEGIN testELNFile: copy into all export tests in this folder   ######
+    def testELNFile(fileName:str, verbose:bool) -> None:
       """
-      main function
+      an test that is similar to the test of TheELNConsortium
+      - copied here for portability
+
+      Args:
+        fileName (str): file name of .eln to test
       """
       # global variables worth discussion
       ROCRATE_NOTE_MANDATORY = ['version','sdPublisher']
       DATASET_MANDATORY = ['name']
       DATASET_SUGGESTED = ['author','mentions',  'dateCreated', 'dateModified', 'identifier', 'text', 'keywords']
       FILE_MANDATORY = ['name']
       FILE_SUGGESTED = ['sha256', 'encodingFormat', 'contentSize', 'description']
@@ -44,108 +46,107 @@
       # runtime global variables
       METADATA_FILE = 'ro-crate-metadata.json'
       OUTPUT_INFO = False
       OUTPUT_COUNTS = True
       KNOWN_KEYS = DATASET_MANDATORY+DATASET_SUGGESTED+FILE_MANDATORY+FILE_SUGGESTED+['@id', '@type']
 
       logJson = {}
-
-      def processNode(graph, nodeID):
-          """
-          recursive function call to process each node
-
-          Args:
-            graph: full graph
-            nodeID: id of node in graph
-          """
-          globalSuccess = True
-          nodes = [ i for i in graph if '@id' in i and i['@id'] == nodeID]
-          if len(nodes)!=1:
-              print('**ERROR: all entries must only occur once in crate. check:', nodeID)
-              return
-          node = nodes[0]
-          # CHECK IF MANDATORY AND SUGGESTED KEYWORDS ARE PRESENT
-          if '@type' not in node:
-              print('**ERROR: all nodes must have @type. check:', nodeID)
-          if node['@type'] == 'Dataset':
-              for key in DATASET_MANDATORY:
-                  if not key in node:
-                      print(f'**ERROR in dataset: "{key}" not in @id={node["@id"]}')
-                      globalSuccess = False
-              for key in DATASET_SUGGESTED:
-                  if not key in node and OUTPUT_INFO:
-                      print(f'**INFO for dataset: "{key}" not in @id={node["@id"]}')
-          elif node['@type'] == 'File':
-              for key in FILE_MANDATORY:
-                  if not key in node:
-                      print(f'**ERROR in file: "{key}" not in @id={node["@id"]}')
-                      globalSuccess = False
-              for key in FILE_SUGGESTED:
-                  if not key in node and OUTPUT_INFO:
-                      print(f'**INFO for file: "{key}" not in @id={node["@id"]}')
-          # CHECK PROPERTIES FOR ALL KEYS
-          if any([str(i).strip()=='' for i in node.values()]):
-              print(f'**WARNING: {nodeID} contains empty values in the key-value pairs', node)
-          # SPECIFIC CHECKS ON CERTAIN KEYS
-          if isinstance(node.get('keywords', ''), list):
-              print(f'**ERROR: {nodeID} contains an array of keywords. Use comma or space separated string')
+      def processNode(graph: list[dict[str,Any]], nodeID:str) -> bool:
+        """
+        recursive function call to process each node
+
+        Args:
+        graph: full graph
+        nodeID: id of node in graph
+        """
+        globalSuccess = True
+        nodes = [i for i in graph if '@id' in i and i['@id'] == nodeID]
+        if len(nodes)!=1:
+          print('**ERROR: all entries must only occur once in crate. check:', nodeID)
+          return False
+        node = nodes[0]
+        # CHECK IF MANDATORY AND SUGGESTED KEYWORDS ARE PRESENT
+        if '@type' not in node:
+          print('**ERROR: all nodes must have @type. check:', nodeID)
+        if node['@type'] == 'Dataset':
+          for key in DATASET_MANDATORY:
+            if not key in node:
+              print(f'**ERROR in dataset: "{key}" not in @id={node["@id"]}')
+              globalSuccess = False
+          for key in DATASET_SUGGESTED:
+            if not key in node and OUTPUT_INFO and verbose:
+              print(f'**INFO for dataset: "{key}" not in @id={node["@id"]}')
+        elif node['@type'] == 'File':
+          for key in FILE_MANDATORY:
+            if not key in node:
+              print(f'**ERROR in file: "{key}" not in @id={node["@id"]}')
               globalSuccess = False
-          # recurse to children
-          children = node.pop('hasPart') if 'hasPart' in node else []
-          for child in children:
-              globalSuccess = processNode(graph, child['@id']) and globalSuccess
-          return globalSuccess
+          for key in FILE_SUGGESTED:
+            if not key in node and OUTPUT_INFO and verbose:
+              print(f'**INFO for file: "{key}" not in @id={node["@id"]}')
+        # CHECK PROPERTIES FOR ALL KEYS
+        if any(str(i).strip()=='' for i in node.values()):
+          print(f'**WARNING: {nodeID} contains empty values in the key-value pairs', node)
+        # SPECIFIC CHECKS ON CERTAIN KEYS
+        if isinstance(node.get('keywords', ''), list):
+          print(f'**ERROR: {nodeID} contains an array of keywords. Use comma or space separated string')
+          globalSuccess = False
+        # recurse to children
+        children = node.pop('hasPart') if 'hasPart' in node else []
+        for child in children:
+          globalSuccess = processNode(graph, child['@id']) and globalSuccess
+        return globalSuccess
 
-      print(f'\n\nParse: {fileName}')
+      if verbose:
+        print(f'\n\nParse: {fileName}')
       with ZipFile(fileName, 'r', compression=ZIP_DEFLATED) as elnFile:
-          success = True
-          p = ZPath(elnFile)
-          dirName = sorted(p.iterdir())[0]
-          metadataJsonFile = dirName.joinpath(METADATA_FILE)
-          metadataContent = json.loads(metadataJsonFile.read_bytes())
-          graph = metadataContent["@graph"]
-          # find information from master node
-          ro_crate_nodes = [i for i in graph if i["@id"] == METADATA_FILE]
-          if len(ro_crate_nodes) == 1:
-              for key in ROCRATE_NOTE_MANDATORY:
-                  if not key in ro_crate_nodes[0]:
-                      print(f'**ERROR: "{key}" not in @id={METADATA_FILE}')
-          else:
-              print(f'**ERROR: @id={METADATA_FILE} does not uniquely exist ')
-              success = False
-          main_node = [i for i in graph if i["@id"] == "./"][0]
-
-          # iteratively go through graph
-          for partI in main_node['hasPart']:
-              success = processNode(graph, partI['@id']) and success
-          if fileName not in logJson:
-              logJson[fileName] = {'params_metadata_json':success}
-          else:
-              logJson[fileName] = logJson[fileName] | {'params_metadata_json':success}
-
-          # count occurrences of all keys
-          counts = {}
-          for node in graph:
-              if node['@id'] in ['./',METADATA_FILE]:
-                  continue
-              for key in node.keys():
-                  if key in counts:
-                      counts[key] += 1
-                  else:
-                      counts[key] = 1
-
-          view = [ (v,k) for k,v in counts.items() ]
-          view.sort(reverse=True)
-          if OUTPUT_COUNTS:
-              print('===== Counts (* unspecified)')
-              for v,k in view:
-                  prefix = '   ' if k in KNOWN_KEYS else ' * '
-                  print(f'{prefix}{k:15}: {v}')
-      print('\n\nSuccess:', success)
-
+        success = True
+        metadataJsonFile = [i for i in elnFile.namelist() if i.endswith(METADATA_FILE)][0]
+        with elnFile.open(metadataJsonFile) as roCrateFile:
+          metadataContent = json.loads(roCrateFile.read())
+        graph = metadataContent["@graph"]
+        # find information from master node
+        ro_crate_nodes = [i for i in graph if i["@id"] == METADATA_FILE]
+        if len(ro_crate_nodes) == 1:
+          for key in ROCRATE_NOTE_MANDATORY:
+            if not key in ro_crate_nodes[0]:
+              print(f'**ERROR: "{key}" not in @id={METADATA_FILE}')
+        else:
+          print(f'**ERROR: @id={METADATA_FILE} does not uniquely exist ')
+          success = False
+        main_node = [i for i in graph if i["@id"] == "./"][0]
+
+        # iteratively go through graph
+        for partI in main_node['hasPart']:
+          success = processNode(graph, partI['@id']) and success
+        if fileName not in logJson:
+          logJson[fileName] = {'params_metadata_json':success}
+        else:
+          logJson[fileName] = logJson[fileName] | {'params_metadata_json':success}
+
+        # count occurrences of all keys
+        counts:dict[str,int] = {}
+        for node in graph:
+          if node['@id'] in ['./',METADATA_FILE]:
+            continue
+          for key in node.keys():
+            if key in counts:
+              counts[key] += 1
+            else:
+              counts[key] = 1
+        view = [ (v,k) for k,v in counts.items() ]
+        view.sort(reverse=True)
+        if OUTPUT_COUNTS and verbose:
+          print('===== Counts (* unspecified)')
+          for v,k in view:
+            prefix = '   ' if k in KNOWN_KEYS else ' * '
+            print(f'{prefix}{k:15}: {v}')
+          print('\n\nSuccess:', success)
+      return
+    ###### BEGIN testELNFile: copy into all export tests in this folder   ######
     # main test function: create stuff, test, ...
     outputFormat = 'print'
     # initialization: create database, destroy on filesystem and database and then create new one
     warnings.filterwarnings('ignore', message='numpy.ufunc size changed')
     warnings.filterwarnings('ignore', message='invalid escape sequence')
     warnings.filterwarnings('ignore', category=ResourceWarning, module='PIL')
     warnings.filterwarnings('ignore', category=ImportWarning)
@@ -160,46 +161,47 @@
       doc['comment'] = f'Test string {idx}'
       self.be.editData(doc)
 
     # export
     viewProj = self.be.db.getView('viewDocType/x0')
     idProj  = [i['id'] for i in viewProj if i['value'][0]=='Intermetals at interfaces'][0]
     self.fileName = str(Path.home()/'temporary_pastaTest.eln')
-    status = exportELN(self.be, idProj, self.fileName, ['procedure','measurement','sample'])
+    status = exportELN(self.be, [idProj], self.fileName, ['procedure','measurement','sample'])
     print(f'Export to: {self.fileName}\n{status}')
-    self.assertEqual(status[:21],'Success: exported 20 ','Export unsuccessful')
+    self.assertEqual(status[:21],'Success: exported 13 ','Export unsuccessful')
 
     # verify eln
     print('\n\nEnd export\n----------------------\nStart verification')
-    test_A_File(self.fileName)
+    testELNFile(self.fileName, False)
 
-    # remove old
-    docProj = self.be.db.getDoc(idProj)
-    oldPath = self.be.basePath/docProj['-branch'][0]['path']
-    shutil.rmtree(oldPath)
-    allDocs = self.be.db.getView('viewHierarchy/viewHierarchy',    startKey=idProj)
-    for doc in allDocs:
-      self.be.db.remove(doc['id'])
-
-    # import
-    print('\n\n---------------\nImport')
-    status = importELN(self.be, self.fileName)
-    print(status)
-    self.assertEqual(status[:7],'Success','Import unsuccessful')
+    # IMPORT NOT IMPLEMENTED YET
+    # # remove old
+    # docProj = self.be.db.getDoc(idProj)
+    # oldPath = self.be.basePath/docProj['-branch'][0]['path']
+    # shutil.rmtree(oldPath)
+    # allDocs = self.be.db.getView('viewHierarchy/viewHierarchy',    startKey=idProj)
+    # for doc in allDocs:
+    #   self.be.db.remove(doc['id'])
+
+    # # import
+    # print('\n\n---------------\nImport')
+    # status = importELN(self.be, self.fileName)
+    # print(status)
+    # self.assertEqual(status[:7],'Success','Import unsuccessful')
 
     #test / verify
     print('Number of documents', len(self.be.db.getView('viewHierarchy/viewHierarchy',    startKey=idProj)))
     outputString(outputFormat,'h2','VERIFY DATABASE INTEGRITY')
     outputString(outputFormat,'info', self.be.checkDB(outputStyle='text'))
     outputString(outputFormat,'h2','DONE WITH VERIFY')
     fileCount = 0
     for _, _, files in os.walk(self.be.basePath):
       fileCount+=len(files)
-    print(f'Number of files 15 (should be) = {fileCount} (are)')
-    self.assertEqual(fileCount, 15, 'Imported entries are not 15, as they should.')
+    print(f'Number of files 16 (should be) = {fileCount} (are)')
+    self.assertEqual(fileCount, 16, 'Imported entries are not 16, as they should.')
     return
 
   def tearDown(self):
     logging.info('End Export-import test')
     # Path(self.fileName).unlink()  #remove file
     return
```

### Comparing `pasta_eln-2.5.2b2/tests/test_99_3Projects.py` & `pasta_eln-2.5.3b1/tests/test_99_3Projects.py`

 * *Files identical despite different names*

