# Comparing `tmp/lunes-cms-2024.5.0.tar.gz` & `tmp/lunes-cms-2024.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lunes-cms-2024.5.0.tar", last modified: Mon May 13 08:32:43 2024, max compression
+gzip compressed data, was "lunes-cms-2024.5.1.tar", last modified: Wed May 15 16:25:32 2024, max compression
```

## Comparing `lunes-cms-2024.5.0.tar` & `lunes-cms-2024.5.1.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.233021 lunes-cms-2024.5.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1136 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/NOTICE.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4345 2024-05-13 08:32:43.233021 lunes-cms-2024.5.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1577 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.205021 lunes-cms-2024.5.0/lunes_cms/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       96 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.209021 lunes-cms-2024.5.0/lunes_cms/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      278 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      311 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/apps.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      833 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/permissions.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.209021 lunes-cms-2024.5.0/lunes_cms/api/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      186 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/templates/swagger_ui.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      408 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/urls.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4961 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.209021 lunes-cms-2024.5.0/lunes_cms/api/v1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.209021 lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      433 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/alternative_word_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1360 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/discipline_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1050 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/document_image_list_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      540 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/document_image_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      865 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/document_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      812 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/fallback_icon_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1568 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/feedback_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1206 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/group_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      436 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/sponsor_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      543 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/training_set_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1902 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/urls.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.213021 lunes-cms-2024.5.0/lunes_cms/api/v1/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      511 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/views/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1870 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/views/discipline_filtered_viewset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1655 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/views/discipline_viewset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1097 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/views/document_by_id_viewset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1623 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/views/document_viewset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      308 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/views/feedback_viewset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1423 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/views/group_viewset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      671 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/views/sponsors_viewset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1325 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/views/training_set_by_id_viewset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1591 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/views/training_set_viewset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1858 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/views/word_viewset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.213021 lunes-cms-2024.5.0/lunes_cms/cms/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      128 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1901 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/admin.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.217022 lunes-cms-2024.5.0/lunes_cms/cms/admins/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      417 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/admins/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      392 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/admins/alternative_word_admin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12953 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/admins/discipline_admin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8083 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/admins/document_admin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1127 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/admins/document_image_admin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2169 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/admins/feedback_admin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      372 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/admins/group_api_key_admin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1185 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/admins/sponsor_admin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14258 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/admins/training_set_admin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      312 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/apps.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2797 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/forms.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10231 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/list_filter.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.217022 lunes-cms-2024.5.0/lunes_cms/cms/migrations/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12826 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/migrations/0001_initial.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1819 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/migrations/0002_modify_group_model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      395 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/migrations/0003_remove_documentimage_name.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2868 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/migrations/0004_feedback.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1493 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/migrations/0005_auto_create_id.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3316 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/migrations/0006_convert_group_api_key.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2571 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/migrations/0007_document_created_by_link.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      889 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/migrations/0008_add_numerals_adverbs_and_pronouns_as_word_types.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1428 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/migrations/0009_sponsor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      445 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/migrations/0010_sponsor_url.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      485 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/migrations/0011_document_example_sentence.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1158 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/migrations/0012_add_additional_field.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/migrations/0013_add_plural_field.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2500 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/migrations/0014_add_plural_field_and_plural_article.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1308 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/migrations/0015_add_grammatical_gender_fields.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/migrations/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.221022 lunes-cms-2024.5.0/lunes_cms/cms/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      647 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/models/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1569 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/models/alternative_word.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      154 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/models/content_type.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3035 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/models/discipline.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4461 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/models/document.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3865 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/models/document_image.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2953 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/models/feedback.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      316 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/models/group.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4886 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/models/group_api_key.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1014 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/models/sponsor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3332 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/models/static.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3390 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/models/training_set.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.205021 lunes-cms-2024.5.0/lunes_cms/cms/templates/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.221022 lunes-cms-2024.5.0/lunes_cms/cms/templates/admin/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      965 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/templates/admin/base.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3954 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/templates/admin/delete_confirmation.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3905 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/templates/admin/delete_selected_confirmation.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1232 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/templates/admin/discipline_filter.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      463 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/templates/admin/object_delete_summary.html
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.221022 lunes-cms-2024.5.0/lunes_cms/cms/templatetags/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      391 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/templatetags/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      909 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/templatetags/admin_filter_tags.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1194 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/urls.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4913 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1364 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/validators.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      889 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/widgets.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.225021 lunes-cms-2024.5.0/lunes_cms/core/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/core/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      557 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/core/context_processors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1049 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/core/logging_formatter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17883 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/core/settings.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1690 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/core/urls.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1272 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/core/wsgi.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.225021 lunes-cms-2024.5.0/lunes_cms/help/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       67 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/help/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      320 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/help/apps.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.225021 lunes-cms-2024.5.0/lunes_cms/help/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5641 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/help/templates/public_upload.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      353 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/help/urls.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.225021 lunes-cms-2024.5.0/lunes_cms/help/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       41 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/help/views/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2137 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/help/views/public_upload.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.205021 lunes-cms-2024.5.0/lunes_cms/locale/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.205021 lunes-cms-2024.5.0/lunes_cms/locale/de/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.225021 lunes-cms-2024.5.0/lunes_cms/locale/de/LC_MESSAGES/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10993 2024-05-13 08:32:34.000000 lunes-cms-2024.5.0/lunes_cms/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 circleci  (1001) circleci  (1002)      592 2024-05-13 08:32:34.000000 lunes-cms-2024.5.0/lunes_cms/locale/de/LC_MESSAGES/djangojs.mo
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      983 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/lunes-cms-cli
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.205021 lunes-cms-2024.5.0/lunes_cms/static/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.205021 lunes-cms-2024.5.0/lunes_cms/static/bootstrap/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.225021 lunes-cms-2024.5.0/lunes_cms/static/bootstrap/css/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6573 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/static/bootstrap/css/bootstrap.min.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.229021 lunes-cms-2024.5.0/lunes_cms/static/css/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3988 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/static/css/corporate_identity.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)       76 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/static/css/document_form.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)      972 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/static/css/feedback.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1384 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/static/css/overlay.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.229021 lunes-cms-2024.5.0/lunes_cms/static/guidelines/
--rw-r--r--   0 circleci  (1001) circleci  (1002)  1447497 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/static/guidelines/fotoguide.pdf
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.229021 lunes-cms-2024.5.0/lunes_cms/static/images/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      264 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/static/images/fallback-icon.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3177 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/static/images/logo-lunes-dark.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3181 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/static/images/logo-lunes.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      933 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/static/images/logo.svg
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.233021 lunes-cms-2024.5.0/lunes_cms/static/js/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      705 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/static/js/color_unread_feedback.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      235 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/static/js/corporate_identity.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1430 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/static/js/image_preview.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2613 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/static/js/manytomany_overlay.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4545 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/static/js/overlay.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      465 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/static/js/toggle_plural_field.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.233021 lunes-cms-2024.5.0/lunes_cms.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4345 2024-05-13 08:32:43.000000 lunes-cms-2024.5.0/lunes_cms.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4873 2024-05-13 08:32:43.000000 lunes-cms-2024.5.0/lunes_cms.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-13 08:32:43.000000 lunes-cms-2024.5.0/lunes_cms.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      568 2024-05-13 08:32:43.000000 lunes-cms-2024.5.0/lunes_cms.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-05-13 08:32:43.000000 lunes-cms-2024.5.0/lunes_cms.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2438 2024-05-13 08:32:43.237022 lunes-cms-2024.5.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      187 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 16:25:32.934925 lunes-cms-2024.5.1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1136 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/NOTICE.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4345 2024-05-15 16:25:32.934925 lunes-cms-2024.5.1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1577 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 16:25:32.910925 lunes-cms-2024.5.1/lunes_cms/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       96 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 16:25:32.910925 lunes-cms-2024.5.1/lunes_cms/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      278 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      311 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/api/apps.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      833 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/api/permissions.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 16:25:32.910925 lunes-cms-2024.5.1/lunes_cms/api/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      186 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/api/templates/swagger_ui.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      408 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/api/urls.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4961 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/api/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 16:25:32.910925 lunes-cms-2024.5.1/lunes_cms/api/v1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/api/v1/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 16:25:32.914925 lunes-cms-2024.5.1/lunes_cms/api/v1/serializers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/api/v1/serializers/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      491 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/api/v1/serializers/alternative_word_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1360 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/api/v1/serializers/discipline_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1050 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/api/v1/serializers/document_image_list_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      540 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/api/v1/serializers/document_image_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      923 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/api/v1/serializers/document_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      812 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/api/v1/serializers/fallback_icon_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1568 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/api/v1/serializers/feedback_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1206 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/api/v1/serializers/group_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      436 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/api/v1/serializers/sponsor_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      543 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/api/v1/serializers/training_set_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1902 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/api/v1/urls.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 16:25:32.914925 lunes-cms-2024.5.1/lunes_cms/api/v1/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      511 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/api/v1/views/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1870 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/api/v1/views/discipline_filtered_viewset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1655 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/api/v1/views/discipline_viewset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1097 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/api/v1/views/document_by_id_viewset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1623 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/api/v1/views/document_viewset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      308 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/api/v1/views/feedback_viewset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1423 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/api/v1/views/group_viewset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      671 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/api/v1/views/sponsors_viewset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1325 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/api/v1/views/training_set_by_id_viewset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1591 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/api/v1/views/training_set_viewset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1858 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/api/v1/views/word_viewset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 16:25:32.918925 lunes-cms-2024.5.1/lunes_cms/cms/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      128 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1901 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/admin.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 16:25:32.918925 lunes-cms-2024.5.1/lunes_cms/cms/admins/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      417 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/admins/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      392 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/admins/alternative_word_admin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12953 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/admins/discipline_admin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8083 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/admins/document_admin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1127 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/admins/document_image_admin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2169 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/admins/feedback_admin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      372 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/admins/group_api_key_admin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1185 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/admins/sponsor_admin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14258 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/admins/training_set_admin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      312 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/apps.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2797 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/forms.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10231 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/list_filter.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 16:25:32.922925 lunes-cms-2024.5.1/lunes_cms/cms/migrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12826 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/migrations/0001_initial.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1819 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/migrations/0002_modify_group_model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      395 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/migrations/0003_remove_documentimage_name.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2868 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/migrations/0004_feedback.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1493 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/migrations/0005_auto_create_id.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3316 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/migrations/0006_convert_group_api_key.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2571 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/migrations/0007_document_created_by_link.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      889 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/migrations/0008_add_numerals_adverbs_and_pronouns_as_word_types.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1428 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/migrations/0009_sponsor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      445 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/migrations/0010_sponsor_url.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      485 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/migrations/0011_document_example_sentence.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1158 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/migrations/0012_add_additional_field.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/migrations/0013_add_plural_field.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2500 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/migrations/0014_add_plural_field_and_plural_article.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1308 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/migrations/0015_add_grammatical_gender_fields.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/migrations/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 16:25:32.922925 lunes-cms-2024.5.1/lunes_cms/cms/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      647 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/models/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1569 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/models/alternative_word.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      154 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/models/content_type.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3035 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/models/discipline.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4461 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/models/document.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3865 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/models/document_image.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2953 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/models/feedback.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      316 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/models/group.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4886 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/models/group_api_key.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1014 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/models/sponsor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3332 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/models/static.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3390 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/models/training_set.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 16:25:32.906925 lunes-cms-2024.5.1/lunes_cms/cms/templates/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 16:25:32.926925 lunes-cms-2024.5.1/lunes_cms/cms/templates/admin/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      965 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/templates/admin/base.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3954 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/templates/admin/delete_confirmation.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3905 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/templates/admin/delete_selected_confirmation.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1232 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/templates/admin/discipline_filter.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      463 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/templates/admin/object_delete_summary.html
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 16:25:32.926925 lunes-cms-2024.5.1/lunes_cms/cms/templatetags/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      391 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/templatetags/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      909 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/templatetags/admin_filter_tags.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1194 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/urls.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4913 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1364 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/validators.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      889 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/cms/widgets.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 16:25:32.926925 lunes-cms-2024.5.1/lunes_cms/core/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/core/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      557 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/core/context_processors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1049 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/core/logging_formatter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17883 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/core/settings.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1690 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/core/urls.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1272 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/core/wsgi.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 16:25:32.926925 lunes-cms-2024.5.1/lunes_cms/help/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       67 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/help/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      320 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/help/apps.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 16:25:32.926925 lunes-cms-2024.5.1/lunes_cms/help/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5641 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/help/templates/public_upload.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      353 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/help/urls.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 16:25:32.926925 lunes-cms-2024.5.1/lunes_cms/help/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       41 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/help/views/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2137 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/help/views/public_upload.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 16:25:32.906925 lunes-cms-2024.5.1/lunes_cms/locale/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 16:25:32.906925 lunes-cms-2024.5.1/lunes_cms/locale/de/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 16:25:32.926925 lunes-cms-2024.5.1/lunes_cms/locale/de/LC_MESSAGES/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10993 2024-05-15 16:25:22.000000 lunes-cms-2024.5.1/lunes_cms/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      592 2024-05-15 16:25:22.000000 lunes-cms-2024.5.1/lunes_cms/locale/de/LC_MESSAGES/djangojs.mo
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      983 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/lunes-cms-cli
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 16:25:32.906925 lunes-cms-2024.5.1/lunes_cms/static/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 16:25:32.906925 lunes-cms-2024.5.1/lunes_cms/static/bootstrap/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 16:25:32.926925 lunes-cms-2024.5.1/lunes_cms/static/bootstrap/css/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6573 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/static/bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 16:25:32.926925 lunes-cms-2024.5.1/lunes_cms/static/css/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3988 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/static/css/corporate_identity.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       76 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/static/css/document_form.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      972 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/static/css/feedback.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1384 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/static/css/overlay.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 16:25:32.926925 lunes-cms-2024.5.1/lunes_cms/static/guidelines/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  1447497 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/static/guidelines/fotoguide.pdf
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 16:25:32.930925 lunes-cms-2024.5.1/lunes_cms/static/images/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      264 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/static/images/fallback-icon.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3177 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/static/images/logo-lunes-dark.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3181 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/static/images/logo-lunes.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      933 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/static/images/logo.svg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 16:25:32.930925 lunes-cms-2024.5.1/lunes_cms/static/js/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      705 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/static/js/color_unread_feedback.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      235 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/static/js/corporate_identity.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1430 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/static/js/image_preview.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2613 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/static/js/manytomany_overlay.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4545 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/static/js/overlay.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      465 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/lunes_cms/static/js/toggle_plural_field.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 16:25:32.930925 lunes-cms-2024.5.1/lunes_cms.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4345 2024-05-15 16:25:32.000000 lunes-cms-2024.5.1/lunes_cms.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4873 2024-05-15 16:25:32.000000 lunes-cms-2024.5.1/lunes_cms.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-15 16:25:32.000000 lunes-cms-2024.5.1/lunes_cms.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      568 2024-05-15 16:25:32.000000 lunes-cms-2024.5.1/lunes_cms.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-05-15 16:25:32.000000 lunes-cms-2024.5.1/lunes_cms.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2438 2024-05-15 16:25:32.934925 lunes-cms-2024.5.1/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      187 2024-05-15 16:25:29.000000 lunes-cms-2024.5.1/setup.py
```

### Comparing `lunes-cms-2024.5.0/LICENSE` & `lunes-cms-2024.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/MANIFEST.in` & `lunes-cms-2024.5.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/NOTICE.md` & `lunes-cms-2024.5.1/NOTICE.md`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/PKG-INFO` & `lunes-cms-2024.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lunes-cms
-Version: 2024.5.0
+Version: 2024.5.1
 Summary: Content Management System for the Lunes Vocabulary Trainer App
 Home-page: https://lunes.app/
 Author: Tür an Tür – Digitalfabrik gGmbH
 Author-email: tech@integreat-app.de
 License: Apache License 2.0
 Project-URL: Documentation, https://lunes-cms.rtfd.io
 Project-URL: Issues, https://github.com/digitalfabrik/lunes-cms/issues
```

### Comparing `lunes-cms-2024.5.0/README.md` & `lunes-cms-2024.5.1/README.md`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/api/permissions.py` & `lunes-cms-2024.5.1/lunes_cms/api/permissions.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/api/utils.py` & `lunes-cms-2024.5.1/lunes_cms/api/utils.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/__init__.py` & `lunes-cms-2024.5.1/lunes_cms/api/v1/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/discipline_serializer.py` & `lunes-cms-2024.5.1/lunes_cms/api/v1/serializers/discipline_serializer.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/document_image_list_serializer.py` & `lunes-cms-2024.5.1/lunes_cms/api/v1/serializers/document_image_list_serializer.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/document_image_serializer.py` & `lunes-cms-2024.5.1/lunes_cms/api/v1/serializers/document_image_serializer.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/document_serializer.py` & `lunes-cms-2024.5.1/lunes_cms/api/v1/serializers/document_serializer.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,23 +10,25 @@
     Serializer for the Document module. Inherits from
     `serializers.ModelSerializer`.
     """
 
     alternatives = AlternativeWordSerializer(many=True, read_only=True)
     document_image = DocumentImageSerializer(many=True, read_only=True)
 
+    article = serializers.IntegerField(source="singular_article")
+
     class Meta:
         """
         Define model and the corresponding fields
         """
 
         model = Document
         fields = (
             "id",
             "word",
-            "singular_article",
+            "article",
             "audio",
             "word_type",
             "alternatives",
             "document_image",
             "example_sentence",
         )
```

### Comparing `lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/fallback_icon_serializer.py` & `lunes-cms-2024.5.1/lunes_cms/api/v1/serializers/fallback_icon_serializer.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/feedback_serializer.py` & `lunes-cms-2024.5.1/lunes_cms/api/v1/serializers/feedback_serializer.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/group_serializer.py` & `lunes-cms-2024.5.1/lunes_cms/api/v1/serializers/group_serializer.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/training_set_serializer.py` & `lunes-cms-2024.5.1/lunes_cms/api/v1/serializers/training_set_serializer.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/api/v1/urls.py` & `lunes-cms-2024.5.1/lunes_cms/api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/api/v1/views/discipline_filtered_viewset.py` & `lunes-cms-2024.5.1/lunes_cms/api/v1/views/discipline_filtered_viewset.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/api/v1/views/discipline_viewset.py` & `lunes-cms-2024.5.1/lunes_cms/api/v1/views/discipline_viewset.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/api/v1/views/document_by_id_viewset.py` & `lunes-cms-2024.5.1/lunes_cms/api/v1/views/document_by_id_viewset.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/api/v1/views/document_viewset.py` & `lunes-cms-2024.5.1/lunes_cms/api/v1/views/document_viewset.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/api/v1/views/group_viewset.py` & `lunes-cms-2024.5.1/lunes_cms/api/v1/views/group_viewset.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/api/v1/views/sponsors_viewset.py` & `lunes-cms-2024.5.1/lunes_cms/api/v1/views/sponsors_viewset.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/api/v1/views/training_set_by_id_viewset.py` & `lunes-cms-2024.5.1/lunes_cms/api/v1/views/training_set_by_id_viewset.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/api/v1/views/training_set_viewset.py` & `lunes-cms-2024.5.1/lunes_cms/api/v1/views/training_set_viewset.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/api/v1/views/word_viewset.py` & `lunes-cms-2024.5.1/lunes_cms/api/v1/views/word_viewset.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/admin.py` & `lunes-cms-2024.5.1/lunes_cms/cms/admin.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/admins/discipline_admin.py` & `lunes-cms-2024.5.1/lunes_cms/cms/admins/discipline_admin.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/admins/document_admin.py` & `lunes-cms-2024.5.1/lunes_cms/cms/admins/document_admin.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/admins/document_image_admin.py` & `lunes-cms-2024.5.1/lunes_cms/cms/admins/document_image_admin.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/admins/feedback_admin.py` & `lunes-cms-2024.5.1/lunes_cms/cms/admins/feedback_admin.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/admins/sponsor_admin.py` & `lunes-cms-2024.5.1/lunes_cms/cms/admins/sponsor_admin.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/admins/training_set_admin.py` & `lunes-cms-2024.5.1/lunes_cms/cms/admins/training_set_admin.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/forms.py` & `lunes-cms-2024.5.1/lunes_cms/cms/forms.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/list_filter.py` & `lunes-cms-2024.5.1/lunes_cms/cms/list_filter.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/migrations/0001_initial.py` & `lunes-cms-2024.5.1/lunes_cms/cms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/migrations/0002_modify_group_model.py` & `lunes-cms-2024.5.1/lunes_cms/cms/migrations/0002_modify_group_model.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/migrations/0004_feedback.py` & `lunes-cms-2024.5.1/lunes_cms/cms/migrations/0004_feedback.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/migrations/0005_auto_create_id.py` & `lunes-cms-2024.5.1/lunes_cms/cms/migrations/0005_auto_create_id.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/migrations/0006_convert_group_api_key.py` & `lunes-cms-2024.5.1/lunes_cms/cms/migrations/0006_convert_group_api_key.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/migrations/0007_document_created_by_link.py` & `lunes-cms-2024.5.1/lunes_cms/cms/migrations/0007_document_created_by_link.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/migrations/0008_add_numerals_adverbs_and_pronouns_as_word_types.py` & `lunes-cms-2024.5.1/lunes_cms/cms/migrations/0008_add_numerals_adverbs_and_pronouns_as_word_types.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/migrations/0009_sponsor.py` & `lunes-cms-2024.5.1/lunes_cms/cms/migrations/0009_sponsor.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/migrations/0012_add_additional_field.py` & `lunes-cms-2024.5.1/lunes_cms/cms/migrations/0012_add_additional_field.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/migrations/0013_add_plural_field.py` & `lunes-cms-2024.5.1/lunes_cms/cms/migrations/0013_add_plural_field.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/migrations/0014_add_plural_field_and_plural_article.py` & `lunes-cms-2024.5.1/lunes_cms/cms/migrations/0014_add_plural_field_and_plural_article.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/migrations/0015_add_grammatical_gender_fields.py` & `lunes-cms-2024.5.1/lunes_cms/cms/migrations/0015_add_grammatical_gender_fields.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/models/__init__.py` & `lunes-cms-2024.5.1/lunes_cms/cms/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/models/alternative_word.py` & `lunes-cms-2024.5.1/lunes_cms/cms/models/alternative_word.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/models/discipline.py` & `lunes-cms-2024.5.1/lunes_cms/cms/models/discipline.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/models/document.py` & `lunes-cms-2024.5.1/lunes_cms/cms/models/document.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/models/document_image.py` & `lunes-cms-2024.5.1/lunes_cms/cms/models/document_image.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/models/feedback.py` & `lunes-cms-2024.5.1/lunes_cms/cms/models/feedback.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/models/group_api_key.py` & `lunes-cms-2024.5.1/lunes_cms/cms/models/group_api_key.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/models/sponsor.py` & `lunes-cms-2024.5.1/lunes_cms/cms/models/sponsor.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/models/static.py` & `lunes-cms-2024.5.1/lunes_cms/cms/models/static.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/models/training_set.py` & `lunes-cms-2024.5.1/lunes_cms/cms/models/training_set.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/templates/admin/base.html` & `lunes-cms-2024.5.1/lunes_cms/cms/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/templates/admin/delete_confirmation.html` & `lunes-cms-2024.5.1/lunes_cms/cms/templates/admin/delete_confirmation.html`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/templates/admin/delete_selected_confirmation.html` & `lunes-cms-2024.5.1/lunes_cms/cms/templates/admin/delete_selected_confirmation.html`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/templates/admin/discipline_filter.html` & `lunes-cms-2024.5.1/lunes_cms/cms/templates/admin/discipline_filter.html`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/templatetags/admin_filter_tags.py` & `lunes-cms-2024.5.1/lunes_cms/cms/templatetags/admin_filter_tags.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/urls.py` & `lunes-cms-2024.5.1/lunes_cms/cms/urls.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/utils.py` & `lunes-cms-2024.5.1/lunes_cms/cms/utils.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/validators.py` & `lunes-cms-2024.5.1/lunes_cms/cms/validators.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/cms/widgets.py` & `lunes-cms-2024.5.1/lunes_cms/cms/widgets.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/core/context_processors.py` & `lunes-cms-2024.5.1/lunes_cms/core/context_processors.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/core/logging_formatter.py` & `lunes-cms-2024.5.1/lunes_cms/core/logging_formatter.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/core/settings.py` & `lunes-cms-2024.5.1/lunes_cms/core/settings.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/core/urls.py` & `lunes-cms-2024.5.1/lunes_cms/core/urls.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/core/wsgi.py` & `lunes-cms-2024.5.1/lunes_cms/core/wsgi.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/help/templates/public_upload.html` & `lunes-cms-2024.5.1/lunes_cms/help/templates/public_upload.html`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/help/views/public_upload.py` & `lunes-cms-2024.5.1/lunes_cms/help/views/public_upload.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/locale/de/LC_MESSAGES/django.mo` & `lunes-cms-2024.5.1/lunes_cms/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/locale/de/LC_MESSAGES/djangojs.mo` & `lunes-cms-2024.5.1/lunes_cms/locale/de/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/lunes-cms-cli` & `lunes-cms-2024.5.1/lunes_cms/lunes-cms-cli`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/static/bootstrap/css/bootstrap.min.css` & `lunes-cms-2024.5.1/lunes_cms/static/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/static/css/corporate_identity.css` & `lunes-cms-2024.5.1/lunes_cms/static/css/corporate_identity.css`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/static/css/feedback.css` & `lunes-cms-2024.5.1/lunes_cms/static/css/feedback.css`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/static/css/overlay.css` & `lunes-cms-2024.5.1/lunes_cms/static/css/overlay.css`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/static/guidelines/fotoguide.pdf` & `lunes-cms-2024.5.1/lunes_cms/static/guidelines/fotoguide.pdf`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/static/images/logo-lunes-dark.svg` & `lunes-cms-2024.5.1/lunes_cms/static/images/logo-lunes-dark.svg`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/static/images/logo-lunes.svg` & `lunes-cms-2024.5.1/lunes_cms/static/images/logo-lunes.svg`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/static/images/logo.svg` & `lunes-cms-2024.5.1/lunes_cms/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/static/js/color_unread_feedback.js` & `lunes-cms-2024.5.1/lunes_cms/static/js/color_unread_feedback.js`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/static/js/image_preview.js` & `lunes-cms-2024.5.1/lunes_cms/static/js/image_preview.js`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/static/js/manytomany_overlay.js` & `lunes-cms-2024.5.1/lunes_cms/static/js/manytomany_overlay.js`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms/static/js/overlay.js` & `lunes-cms-2024.5.1/lunes_cms/static/js/overlay.js`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms.egg-info/PKG-INFO` & `lunes-cms-2024.5.1/lunes_cms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lunes-cms
-Version: 2024.5.0
+Version: 2024.5.1
 Summary: Content Management System for the Lunes Vocabulary Trainer App
 Home-page: https://lunes.app/
 Author: Tür an Tür – Digitalfabrik gGmbH
 Author-email: tech@integreat-app.de
 License: Apache License 2.0
 Project-URL: Documentation, https://lunes-cms.rtfd.io
 Project-URL: Issues, https://github.com/digitalfabrik/lunes-cms/issues
```

### Comparing `lunes-cms-2024.5.0/lunes_cms.egg-info/SOURCES.txt` & `lunes-cms-2024.5.1/lunes_cms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/lunes_cms.egg-info/requires.txt` & `lunes-cms-2024.5.1/lunes_cms.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `lunes-cms-2024.5.0/setup.cfg` & `lunes-cms-2024.5.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lunes-cms
-version = 2024.5.0
+version = 2024.5.1
 author = Tür an Tür – Digitalfabrik gGmbH
 author_email = tech@integreat-app.de
 description = Content Management System for the Lunes Vocabulary Trainer App
 url = https://lunes.app/
 project_urls = 
 	Documentation=https://lunes-cms.rtfd.io
 	Issues=https://github.com/digitalfabrik/lunes-cms/issues
@@ -78,15 +78,15 @@
 	pytest-circleci-parallelized==0.1.0
 	pytest-cov==4.1.0
 	pytest-django==4.5.2
 	pytest-icdiff==0.8
 	pytest-xdist==3.3.1
 
 [bumpver]
-current_version = 2024.5.0
+current_version = 2024.5.1
 version_pattern = YYYY.MM.INC0[-TAG]
 commit_message = 
 	Bump version to {new_version}
 	[skip ci]
 commit = True
 tag = False
 push = False
```

