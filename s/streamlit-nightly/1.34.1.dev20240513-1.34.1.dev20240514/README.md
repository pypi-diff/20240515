# Comparing `tmp/streamlit_nightly-1.34.1.dev20240513.tar.gz` & `tmp/streamlit_nightly-1.34.1.dev20240514.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_nightly-1.34.1.dev20240513.tar", last modified: Tue May 14 06:54:32 2024, max compression
+gzip compressed data, was "streamlit_nightly-1.34.1.dev20240514.tar", last modified: Wed May 15 11:51:50 2024, max compression
```

## Comparing `streamlit_nightly-1.34.1.dev20240513.tar` & `streamlit_nightly-1.34.1.dev20240514.tar`

### file list

```diff
@@ -1,576 +1,576 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.171996 streamlit_nightly-1.34.1.dev20240513/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-14 06:54:32.171996 streamlit_nightly-1.34.1.dev20240513/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.055995 streamlit_nightly-1.34.1.dev20240513/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/bin/streamlit.cmd
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 06:54:32.171996 streamlit_nightly-1.34.1.dev20240513/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.063995 streamlit_nightly-1.34.1.dev20240513/streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)     8150 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/case_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/cli_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/code_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/color_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/column_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.063995 streamlit_nightly-1.34.1.dev20240513/streamlit/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/commands/execution_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/commands/experimental_query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/commands/logo.py
--rw-r--r--   0 runner    (1001) docker     (127)    12997 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/commands/page_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.063995 streamlit_nightly-1.34.1.dev20240513/streamlit/components/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.063995 streamlit_nightly-1.34.1.dev20240513/streamlit/components/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/components/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/components/lib/local_component_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.067995 streamlit_nightly-1.34.1.dev20240513/streamlit/components/types/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/components/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/components/types/base_component_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/components/types/base_custom_component.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.067995 streamlit_nightly-1.34.1.dev20240513/streamlit/components/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/components/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/components/v1/component_arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/components/v1/component_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/components/v1/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     8869 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/components/v1/custom_component.py
--rw-r--r--   0 runner    (1001) docker     (127)    43895 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/config_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/config_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.067995 streamlit_nightly-1.34.1.dev20240513/streamlit/connections/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/connections/base_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/connections/snowflake_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/connections/snowpark_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12234 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/connections/sql_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/connections/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    28228 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/delta_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/deprecation_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/development.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/echo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.071995 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7432 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)    23818 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/balloons.py
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/bokeh_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/code.py
--rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/deck_gl_json_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/dialog_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    16168 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/doc_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/empty.py
--rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)    12072 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/form.py
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/graphviz_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)    11268 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/heading.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/iframe.py
--rw-r--r--   0 runner    (1001) docker     (127)    20394 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/json.py
--rw-r--r--   0 runner    (1001) docker     (127)    28251 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/layouts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.075995 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30666 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/lib/built_in_chart_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17226 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/lib/column_config_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    51174 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/lib/column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/lib/dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/lib/dicttools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/lib/event_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/lib/mutable_status_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/lib/pandas_styler_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/lib/streamlit_plotly_theme.py
--rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/lib/subtitle_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/map.py
--rw-r--r--   0 runner    (1001) docker     (127)    10384 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)    29678 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/media.py
--rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    15332 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/plotly_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/pyplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/snow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/spinner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/toast.py
--rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    43912 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/vega_charts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.079995 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32860 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/widgets/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/widgets/camera_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    14320 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/widgets/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)    12573 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/widgets/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     9142 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/widgets/color_picker.py
--rw-r--r--   0 runner    (1001) docker     (127)    35827 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/widgets/data_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)    17656 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/widgets/file_uploader.py
--rw-r--r--   0 runner    (1001) docker     (127)    13752 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/widgets/multiselect.py
--rw-r--r--   0 runner    (1001) docker     (127)    18036 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/widgets/number_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    12824 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/widgets/radio.py
--rw-r--r--   0 runner    (1001) docker     (127)    13442 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/widgets/select_slider.py
--rw-r--r--   0 runner    (1001) docker     (127)    11665 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/widgets/selectbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    26661 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/widgets/slider.py
--rw-r--r--   0 runner    (1001) docker     (127)    22333 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/widgets/text_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)    30042 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/widgets/time_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)    20804 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/elements/write.py
--rw-r--r--   0 runner    (1001) docker     (127)    73749 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/emojis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/env_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/error_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.079995 streamlit_nightly-1.34.1.dev20240513/streamlit/external/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.079995 streamlit_nightly-1.34.1.dev20240513/streamlit/external/langchain/
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/external/langchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15280 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/external/langchain/streamlit_callback_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/folder_black_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/git_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.079995 streamlit_nightly-1.34.1.dev20240513/streamlit/hello/
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/hello/Hello.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/hello/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.079995 streamlit_nightly-1.34.1.dev20240513/streamlit/hello/pages/
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/hello/pages/0_Animation_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/hello/pages/1_Plotting_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/hello/pages/2_Mapping_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/hello/pages/3_DataFrame_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/hello/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/js_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    57136 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/material_icon_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/net_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.103995 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Alert_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Alert_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/AppPage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/AppPage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/ArrowNamedDataSet_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/ArrowNamedDataSet_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/ArrowVegaLiteChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/ArrowVegaLiteChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Arrow_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Arrow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Audio_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Audio_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/AutoRerun_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/AutoRerun_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/BackMsg_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/BackMsg_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Balloons_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Balloons_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Block_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Block_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/BokehChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/BokehChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Button_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Button_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/CameraInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/CameraInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/ChatInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/ChatInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Checkbox_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Checkbox_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/ClientState_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/ClientState_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Code_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Code_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/ColorPicker_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/ColorPicker_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Components_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Components_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/DataFrame_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15040 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/DataFrame_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/DateInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/DateInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/DeckGlJsonChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/DeckGlJsonChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Delta_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Delta_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/DocString_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/DocString_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/DownloadButton_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/DownloadButton_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10146 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Element_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Element_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Empty_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Empty_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Exception_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Exception_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Favicon_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Favicon_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/FileUploader_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/FileUploader_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/ForwardMsg_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12312 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/ForwardMsg_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/GitInfo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/GitInfo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/GraphVizChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/GraphVizChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Heading_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Heading_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Html_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Html_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/IFrame_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/IFrame_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Image_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Image_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Json_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Json_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/LabelVisibilityMessage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/LabelVisibilityMessage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/LinkButton_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/LinkButton_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Logo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Logo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Markdown_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Markdown_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Metric_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Metric_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/MultiSelect_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/MultiSelect_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/NamedDataSet_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/NamedDataSet_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/NewSession_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    18437 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/NewSession_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/NumberInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/NumberInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/PageConfig_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/PageConfig_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/PageInfo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/PageInfo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/PageLink_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/PageLink_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/PageNotFound_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/PageNotFound_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/PageProfile_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/PageProfile_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/PagesChanged_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/PagesChanged_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/ParentMessage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/ParentMessage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/PlotlyChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/PlotlyChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Progress_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Progress_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Radio_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Radio_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/RootContainer_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/RootContainer_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Selectbox_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Selectbox_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/SessionEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/SessionEvent_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/SessionStatus_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/SessionStatus_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Skeleton_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Skeleton_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Slider_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Slider_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Snow_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Snow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Spinner_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Spinner_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/TextArea_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/TextArea_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/TextInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/TextInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Text_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Text_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/TimeInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/TimeInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Toast_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Toast_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/VegaLiteChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/VegaLiteChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Video_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Video_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/WidgetStates_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/WidgetStates_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/openmetrics_data_model_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    20476 2024-05-14 06:50:44.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/proto/openmetrics_data_model_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.107995 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36646 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/app_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.111996 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/caching/
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/caching/cache_data_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/caching/cache_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    21616 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/caching/cache_resource_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/caching/cache_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    18329 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/caching/cache_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17358 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/caching/cached_message_replay.py
--rw-r--r--   0 runner    (1001) docker     (127)    18986 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/caching/hashing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.111996 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/caching/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/caching/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/caching/storage/cache_storage_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/caching/storage/dummy_cache_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/caching/storage/local_disk_cache_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    12414 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/connection_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/forward_msg_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/forward_msg_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/fragment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.111996 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/legacy_caching/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/legacy_caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27873 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/legacy_caching/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)    35033 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/legacy_caching/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/media_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/media_file_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/memory_media_file_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/memory_session_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/memory_uploaded_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    14265 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/metrics_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    29438 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/runtime_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/script_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.111996 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/scriptrunner/
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/scriptrunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/scriptrunner/magic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/scriptrunner/magic_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/scriptrunner/script_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/scriptrunner/script_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     8818 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/scriptrunner/script_run_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    29911 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/scriptrunner/script_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12302 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/session_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.115996 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/state/
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/state/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/state/query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     7192 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/state/query_params_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/state/safe_session_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    27500 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/state/session_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/state/session_state_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11300 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/state/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/uploaded_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/websocket_session_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/source_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.115996 streamlit_nightly-1.34.1.dev20240513/streamlit/static/
--rw-r--r--   0 runner    (1001) docker     (127)    14509 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-14 06:51:12.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.055995 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.115996 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    33275 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/css/3466.8b8f33d6.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/css/5441.e3b876c5.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/css/8148.49dfd2ce.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)    29246 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/css/main.3aaaea00.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.147996 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/1074.73973756.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    14999 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/1168.7452e363.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/1307.0f0cca93.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/1451.3b0a3e31.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/1479.6709db03.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/178.7bea8c5d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/1792.8bd6ce2a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    33075 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/2178.90362aae.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    32468 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/2187.9469f035.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/2469.09ea79bb.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/2634.1249dc7a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    65522 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/2736.4336e2b9.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/3053.7e70ec3b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  3637630 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/329.464ed8ec.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/329.464ed8ec.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/3301.1d1b10bb.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  2306325 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/3466.05d62820.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/3466.05d62820.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/3513.7dedbda2.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/3631.be5c35fa.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/4113.99983645.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/4132.49bf3f2c.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/4132.49bf3f2c.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/4177.69f9f18d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/4319.bf1c86bf.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    20662 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/4477.1bd49702.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/4500.b6f348d1.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    14830 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/4666.c4b22a63.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/474.87506447.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/5106.44f0ff51.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    21681 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/5117.04bfe5d3.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  2263616 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/5249.f2f4070d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/5345.65c91ee7.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    10874 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/5379.6571574f.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    12231 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/5441.5bacdeda.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)   107585 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/5791.9a42fb4b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    11449 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/6013.4ba2d616.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/6405.ac5a6f23.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    24494 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/6718.802da17e.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/6853.93dd1c4c.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)   398809 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/6950.70fe55c2.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/6950.70fe55c2.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    88545 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/7142.83028745.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/7175.be4076bc.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  3388121 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/7323.b74cc85b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/7323.b74cc85b.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   936700 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/7483.64f23be7.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/7483.64f23be7.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13275 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/7602.e8abc06b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/7805.acc6316a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/8005.43974a35.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    49951 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/8148.cc5b50d8.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/8427.bd0a7cf3.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/8477.de889fe5.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    15493 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/8492.0d93bd08.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/8536.f8de3d9a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/8570.6de19120.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/8691.9ccf7f89.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/9330.2b4c99e0.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/9336.2d95d840.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    20791 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/937.a1248039.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/937.a1248039.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    22113 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/9656.8c935274.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/9758.6e6d8662.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/9865.fd93213d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  4403722 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/main.45247b52.js
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/main.45247b52.js.LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.163996 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/
--rw-r--r--   0 runner    (1001) docker     (127)    28076 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    63632 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    33516 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    29912 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff
--rw-r--r--   0 runner    (1001) docker     (127)    25324 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    51336 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16780 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff
--rw-r--r--   0 runner    (1001) docker     (127)    32968 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    33580 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    19676 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff
--rw-r--r--   0 runner    (1001) docker     (127)    16988 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30772 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff
--rw-r--r--   0 runner    (1001) docker     (127)    53580 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    26272 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff
--rw-r--r--   0 runner    (1001) docker     (127)    31196 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    31308 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    18748 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff
--rw-r--r--   0 runner    (1001) docker     (127)    24504 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    14112 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff
--rw-r--r--   0 runner    (1001) docker     (127)    22364 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff
--rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff
--rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff
--rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16028 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13568 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    27556 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   247332 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/MaterialSymbols-Outlined.909d2dce4aba724ad02f.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    74492 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    63060 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    62096 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    74052 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    74132 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    62988 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    76860 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    44640 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    44748 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    77664 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    77452 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    44608 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    72892 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30756 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    29384 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    68356 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    72668 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30628 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/checkmark.29851c8e9e6ef0c3d6c1e4efe3c1bb9e.svg
--rw-r--r--   0 runner    (1001) docker     (127)   101906 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif
--rw-r--r--   0 runner    (1001) docker     (127)    73528 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png
--rw-r--r--   0 runner    (1001) docker     (127)    86179 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png
--rw-r--r--   0 runner    (1001) docker     (127)    92182 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg
--rw-r--r--   0 runner    (1001) docker     (127)    39315 2024-05-14 06:54:29.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/string_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/temporary_directory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.163996 streamlit_nightly-1.34.1.dev20240513/streamlit/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.163996 streamlit_nightly-1.34.1.dev20240513/streamlit/testing/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/testing/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36577 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/testing/v1/app_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    59854 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/testing/v1/element_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/testing/v1/local_script_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/testing/v1/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/time_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    48389 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/type_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/url_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/user_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.167997 streamlit_nightly-1.34.1.dev20240513/streamlit/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.167997 streamlit_nightly-1.34.1.dev20240513/streamlit/vendor/ipython/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/vendor/ipython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/vendor/ipython/modified_sys_path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.167997 streamlit_nightly-1.34.1.dev20240513/streamlit/vendor/pympler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/vendor/pympler/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    87925 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/vendor/pympler/asizeof.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.167997 streamlit_nightly-1.34.1.dev20240513/streamlit/watcher/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/watcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/watcher/event_based_path_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/watcher/local_sources_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/watcher/path_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/watcher/polling_path_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/watcher/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.167997 streamlit_nightly-1.34.1.dev20240513/streamlit/web/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14233 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/web/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/web/cache_storage_manager_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/web/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.171996 streamlit_nightly-1.34.1.dev20240513/streamlit/web/server/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/web/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/web/server/app_static_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/web/server/browser_websocket_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/web/server/component_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/web/server/media_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/web/server/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)    14834 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/web/server/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/web/server/server_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/web/server/stats_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/web/server/upload_file_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/streamlit/web/server/websocket_headers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.171996 streamlit_nightly-1.34.1.dev20240513/streamlit_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-14 06:54:30.000000 streamlit_nightly-1.34.1.dev20240513/streamlit_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23416 2024-05-14 06:54:30.000000 streamlit_nightly-1.34.1.dev20240513/streamlit_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 06:54:30.000000 streamlit_nightly-1.34.1.dev20240513/streamlit_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-14 06:54:30.000000 streamlit_nightly-1.34.1.dev20240513/streamlit_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 06:50:41.000000 streamlit_nightly-1.34.1.dev20240513/streamlit_nightly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-14 06:54:30.000000 streamlit_nightly-1.34.1.dev20240513/streamlit_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 06:54:30.000000 streamlit_nightly-1.34.1.dev20240513/streamlit_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:54:32.171996 streamlit_nightly-1.34.1.dev20240513/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-14 06:48:55.000000 streamlit_nightly-1.34.1.dev20240513/tests/testutil.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.319947 streamlit_nightly-1.34.1.dev20240514/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-15 11:51:50.319947 streamlit_nightly-1.34.1.dev20240514/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.195947 streamlit_nightly-1.34.1.dev20240514/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/bin/streamlit.cmd
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 11:51:50.319947 streamlit_nightly-1.34.1.dev20240514/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.203947 streamlit_nightly-1.34.1.dev20240514/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)     8150 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/case_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/cli_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/code_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/color_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/column_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.203947 streamlit_nightly-1.34.1.dev20240514/streamlit/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/commands/execution_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/commands/experimental_query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/commands/logo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12997 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/commands/page_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.203947 streamlit_nightly-1.34.1.dev20240514/streamlit/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.207947 streamlit_nightly-1.34.1.dev20240514/streamlit/components/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/components/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/components/lib/local_component_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.207947 streamlit_nightly-1.34.1.dev20240514/streamlit/components/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/components/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/components/types/base_component_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/components/types/base_custom_component.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.207947 streamlit_nightly-1.34.1.dev20240514/streamlit/components/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/components/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/components/v1/component_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/components/v1/component_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/components/v1/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8869 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/components/v1/custom_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43895 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/config_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/config_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.207947 streamlit_nightly-1.34.1.dev20240514/streamlit/connections/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/connections/base_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/connections/snowflake_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/connections/snowpark_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12234 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/connections/sql_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/connections/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28200 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/delta_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/deprecation_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/development.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/echo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.215947 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7432 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23830 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/balloons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/bokeh_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/deck_gl_json_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/dialog_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16168 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/doc_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12072 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/graphviz_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11268 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/heading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/iframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20394 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28251 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/layouts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.215947 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30666 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/built_in_chart_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17226 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/column_config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51174 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/dicttools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/event_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/mutable_status_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/pandas_styler_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/streamlit_plotly_theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/subtitle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10384 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29678 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15344 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/plotly_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/pyplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/snow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/toast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58273 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/vega_charts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.219947 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32860 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/camera_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14320 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12573 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9142 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/color_picker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35827 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/data_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17656 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/file_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13752 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/multiselect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18036 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/number_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12824 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/radio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13442 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/select_slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11665 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/selectbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26661 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22333 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/text_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30042 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/time_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20804 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/write.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73749 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/emojis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/env_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/error_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.219947 streamlit_nightly-1.34.1.dev20240514/streamlit/external/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.219947 streamlit_nightly-1.34.1.dev20240514/streamlit/external/langchain/
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/external/langchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15280 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/external/langchain/streamlit_callback_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/folder_black_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/git_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.219947 streamlit_nightly-1.34.1.dev20240514/streamlit/hello/
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/hello/Hello.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/hello/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.219947 streamlit_nightly-1.34.1.dev20240514/streamlit/hello/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/hello/pages/0_Animation_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/hello/pages/1_Plotting_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/hello/pages/2_Mapping_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/hello/pages/3_DataFrame_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/hello/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/js_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57136 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/material_icon_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/net_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.247947 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Alert_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Alert_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/AppPage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/AppPage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ArrowNamedDataSet_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ArrowNamedDataSet_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ArrowVegaLiteChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ArrowVegaLiteChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Arrow_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Arrow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Audio_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Audio_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/AutoRerun_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/AutoRerun_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/BackMsg_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/BackMsg_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Balloons_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Balloons_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Block_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Block_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/BokehChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/BokehChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Button_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Button_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/CameraInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/CameraInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ChatInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ChatInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Checkbox_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Checkbox_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ClientState_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ClientState_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Code_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Code_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ColorPicker_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ColorPicker_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Components_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Components_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DataFrame_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15040 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DataFrame_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DateInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DateInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DeckGlJsonChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DeckGlJsonChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Delta_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Delta_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DocString_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DocString_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DownloadButton_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DownloadButton_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10146 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Element_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Element_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Empty_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Empty_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Exception_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Exception_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Favicon_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Favicon_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/FileUploader_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/FileUploader_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ForwardMsg_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12312 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ForwardMsg_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/GitInfo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/GitInfo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/GraphVizChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/GraphVizChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Heading_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Heading_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Html_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Html_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/IFrame_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/IFrame_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Image_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Image_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Json_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Json_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/LabelVisibilityMessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/LabelVisibilityMessage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/LinkButton_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/LinkButton_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Logo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Logo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Markdown_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Markdown_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Metric_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Metric_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/MultiSelect_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/MultiSelect_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/NamedDataSet_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/NamedDataSet_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/NewSession_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18437 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/NewSession_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/NumberInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/NumberInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageConfig_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageConfig_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageInfo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageInfo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageLink_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageLink_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageNotFound_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageNotFound_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageProfile_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageProfile_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PagesChanged_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PagesChanged_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ParentMessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ParentMessage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PlotlyChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PlotlyChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Progress_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Progress_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Radio_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Radio_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/RootContainer_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/RootContainer_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Selectbox_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Selectbox_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/SessionEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/SessionEvent_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/SessionStatus_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/SessionStatus_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Skeleton_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Skeleton_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Slider_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Slider_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Snow_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Snow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Spinner_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Spinner_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/TextArea_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/TextArea_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/TextInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/TextInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Text_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Text_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/TimeInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/TimeInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Toast_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Toast_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/VegaLiteChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/VegaLiteChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Video_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Video_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/WidgetStates_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/WidgetStates_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/openmetrics_data_model_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20476 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/openmetrics_data_model_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.251947 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36646 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/app_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.251947 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/cache_data_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/cache_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21616 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/cache_resource_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/cache_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18329 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/cache_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17358 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/cached_message_replay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18986 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/hashing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.251947 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/storage/cache_storage_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/storage/dummy_cache_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/storage/local_disk_cache_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12414 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/connection_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/forward_msg_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/forward_msg_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/fragment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.255947 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/legacy_caching/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/legacy_caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27873 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/legacy_caching/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35033 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/legacy_caching/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/media_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/media_file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/memory_media_file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/memory_session_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/memory_uploaded_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14265 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/metrics_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29438 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/runtime_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/script_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.255947 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/scriptrunner/
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/scriptrunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/scriptrunner/magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/scriptrunner/magic_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/scriptrunner/script_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/scriptrunner/script_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8818 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/scriptrunner/script_run_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29911 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/scriptrunner/script_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12302 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/session_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.255947 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/state/
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8159 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/state/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/state/query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7192 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/state/query_params_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/state/safe_session_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27500 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/state/session_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/state/session_state_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/state/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/uploaded_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/websocket_session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/source_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.255947 streamlit_nightly-1.34.1.dev20240514/streamlit/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    14509 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-15 11:48:28.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.195947 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.259947 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    33275 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/css/3466.8b8f33d6.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/css/5441.e3b876c5.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/css/8148.49dfd2ce.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)    29246 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/css/main.3aaaea00.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.291947 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/1074.73973756.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15023 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/1168.14f7c6ff.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/1307.0f0cca93.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/1451.3b0a3e31.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/1479.6709db03.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/178.7bea8c5d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/1792.8bd6ce2a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    33075 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/2178.90362aae.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    32468 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/2187.9469f035.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/2469.09ea79bb.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/2634.1249dc7a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    65522 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/2736.4336e2b9.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/3053.7e70ec3b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  3637630 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/329.464ed8ec.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/329.464ed8ec.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/3301.1d1b10bb.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  2306325 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/3466.05d62820.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/3466.05d62820.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/3513.7dedbda2.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/3631.be5c35fa.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/4113.99983645.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/4132.49bf3f2c.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/4132.49bf3f2c.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/4177.69f9f18d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/4319.bf1c86bf.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20662 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/4477.1bd49702.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/4500.b6f348d1.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14830 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/4666.c4b22a63.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/474.87506447.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/5106.44f0ff51.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21681 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/5117.04bfe5d3.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  2263616 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/5249.f2f4070d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/5345.65c91ee7.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10874 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/5379.6571574f.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14533 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/5441.1b94928f.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)   107585 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/5791.9a42fb4b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11449 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/6013.4ba2d616.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/6405.ac5a6f23.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    24494 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/6718.802da17e.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/6853.93dd1c4c.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)   398809 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/6950.70fe55c2.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/6950.70fe55c2.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    88545 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/7142.83028745.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/7175.be4076bc.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  3388121 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/7323.b74cc85b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/7323.b74cc85b.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   936700 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/7483.64f23be7.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/7483.64f23be7.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13275 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/7602.e8abc06b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/7805.acc6316a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/8005.43974a35.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    50192 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/8148.a5f74d47.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/8427.bd0a7cf3.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/8477.de889fe5.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15493 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/8492.0d93bd08.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/8536.f8de3d9a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/8570.6de19120.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/8691.9ccf7f89.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/9330.2b4c99e0.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/9336.2d95d840.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20791 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/937.a1248039.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/937.a1248039.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    22113 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/9656.8c935274.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/9758.6e6d8662.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/9865.fd93213d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  4405405 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/main.32c71338.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/main.32c71338.js.LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.307947 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/
+-rw-r--r--   0 runner    (1001) docker     (127)    28076 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    63632 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    33516 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    29912 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    25324 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    51336 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16780 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    32968 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    33580 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    19676 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    16988 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30772 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    53580 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    26272 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    31196 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    31308 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    18748 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    24504 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    14112 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    22364 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16028 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13568 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    27556 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   247332 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/MaterialSymbols-Outlined.909d2dce4aba724ad02f.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    74492 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    63060 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    62096 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    74052 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    74132 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    62988 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    76860 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    44640 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    44748 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    77664 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    77452 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    44608 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    72892 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30756 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    29384 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    68356 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    72668 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30628 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/checkmark.29851c8e9e6ef0c3d6c1e4efe3c1bb9e.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   101906 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    73528 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    86179 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png
+-rw-r--r--   0 runner    (1001) docker     (127)    92182 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    39315 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/string_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/temporary_directory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.311947 streamlit_nightly-1.34.1.dev20240514/streamlit/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.311947 streamlit_nightly-1.34.1.dev20240514/streamlit/testing/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/testing/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36577 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/testing/v1/app_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59854 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/testing/v1/element_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/testing/v1/local_script_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/testing/v1/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/time_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48389 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/type_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/url_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/user_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.311947 streamlit_nightly-1.34.1.dev20240514/streamlit/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.311947 streamlit_nightly-1.34.1.dev20240514/streamlit/vendor/ipython/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/vendor/ipython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/vendor/ipython/modified_sys_path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.311947 streamlit_nightly-1.34.1.dev20240514/streamlit/vendor/pympler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/vendor/pympler/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    87925 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/vendor/pympler/asizeof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.311947 streamlit_nightly-1.34.1.dev20240514/streamlit/watcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/watcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/watcher/event_based_path_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/watcher/local_sources_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/watcher/path_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/watcher/polling_path_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/watcher/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.311947 streamlit_nightly-1.34.1.dev20240514/streamlit/web/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14233 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/web/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/web/cache_storage_manager_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/web/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.315947 streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/app_static_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/browser_websocket_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/component_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/media_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14834 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/server_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/stats_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/upload_file_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/websocket_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.315947 streamlit_nightly-1.34.1.dev20240514/streamlit_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-15 11:51:48.000000 streamlit_nightly-1.34.1.dev20240514/streamlit_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23416 2024-05-15 11:51:48.000000 streamlit_nightly-1.34.1.dev20240514/streamlit_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 11:51:48.000000 streamlit_nightly-1.34.1.dev20240514/streamlit_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-15 11:51:48.000000 streamlit_nightly-1.34.1.dev20240514/streamlit_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 11:47:55.000000 streamlit_nightly-1.34.1.dev20240514/streamlit_nightly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-15 11:51:48.000000 streamlit_nightly-1.34.1.dev20240514/streamlit_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 11:51:48.000000 streamlit_nightly-1.34.1.dev20240514/streamlit_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.315947 streamlit_nightly-1.34.1.dev20240514/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/tests/testutil.py
```

### Comparing `streamlit_nightly-1.34.1.dev20240513/PKG-INFO` & `streamlit_nightly-1.34.1.dev20240514/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-nightly
-Version: 1.34.1.dev20240513
+Version: 1.34.1.dev20240514
 Summary: A faster way to build and share data apps
 Home-page: https://streamlit.io
 Author: Snowflake Inc
 Author-email: hello@streamlit.io
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/streamlit/streamlit
 Project-URL: Bug Tracker, https://github.com/streamlit/streamlit/issues
```

### Comparing `streamlit_nightly-1.34.1.dev20240513/bin/streamlit.cmd` & `streamlit_nightly-1.34.1.dev20240514/bin/streamlit.cmd`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/setup.py` & `streamlit_nightly-1.34.1.dev20240514/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 from setuptools.command.install import install
 
 THIS_DIRECTORY = Path(__file__).parent
 
-VERSION = "1.34.1.dev20240513"  # PEP-440
+VERSION = "1.34.1.dev20240514"  # PEP-440
 
 # IMPORTANT: We should try very hard *not* to add dependencies to Streamlit.
 # And if you do add one, make the required version as general as possible:
 # - Include relevant lower bound for any features we use from our dependencies
 # - Always include the lower bound as >= VERSION, to keep testing min versions easy
 # - And include an upper bound that's < NEXT_MAJOR_VERSION
 INSTALL_REQUIRES = [
```

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/__init__.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/__main__.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/__main__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/case_converters.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/case_converters.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/cli_util.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/cli_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/code_util.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/code_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/color_util.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/color_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/column_config.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/column_config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/commands/__init__.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/commands/execution_control.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/commands/execution_control.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/commands/experimental_query_params.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/commands/experimental_query_params.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/commands/logo.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/commands/logo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/commands/page_config.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/commands/page_config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/components/__init__.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/components/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/components/lib/__init__.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/components/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/components/lib/local_component_registry.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/components/lib/local_component_registry.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/components/types/__init__.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/components/types/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/components/types/base_component_registry.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/components/types/base_component_registry.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/components/types/base_custom_component.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/components/types/base_custom_component.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/components/v1/__init__.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/components/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/components/v1/component_arrow.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/components/v1/component_arrow.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/components/v1/component_registry.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/components/v1/component_registry.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/components/v1/components.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/components/v1/components.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/components/v1/custom_component.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/components/v1/custom_component.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/config.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/config_option.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/config_option.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/config_util.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/config_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/connections/__init__.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/connections/base_connection.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/connections/base_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/connections/snowflake_connection.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/connections/snowflake_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/connections/snowpark_connection.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/connections/snowpark_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/connections/sql_connection.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/connections/sql_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/connections/util.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/connections/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/constants.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/constants.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/cursor.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/cursor.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/delta_generator.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/delta_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -583,39 +583,39 @@
         ...
         >>> my_table = st.table(df1)
         >>>
         >>> df2 = pd.DataFrame(
         ...    np.random.randn(50, 20),
         ...    columns=('col %d' % i for i in range(20)))
         ...
-        >>> my_table._arrow_add_rows(df2)
+        >>> my_table.add_rows(df2)
         >>> # Now the table shown in the Streamlit app contains the data for
         >>> # df1 followed by the data for df2.
 
         You can do the same thing with plots. For example, if you want to add
         more data to a line chart:
 
         >>> # Assuming df1 and df2 from the example above still exist...
         >>> my_chart = st.line_chart(df1)
-        >>> my_chart._arrow_add_rows(df2)
+        >>> my_chart.add_rows(df2)
         >>> # Now the chart shown in the Streamlit app contains the data for
         >>> # df1 followed by the data for df2.
 
         And for plots whose datasets are named, you can pass the data with a
         keyword argument where the key is the name:
 
-        >>> my_chart = st._arrow_vega_lite_chart({
+        >>> my_chart = st.vega_lite_chart({
         ...     'mark': 'line',
         ...     'encoding': {'x': 'a', 'y': 'b'},
         ...     'datasets': {
         ...       'some_fancy_name': df1,  # <-- named dataset
         ...      },
         ...     'data': {'name': 'some_fancy_name'},
         ... }),
-        >>> my_chart._arrow_add_rows(some_fancy_name=df2)  # <-- name used as keyword
+        >>> my_chart.add_rows(some_fancy_name=df2)  # <-- name used as keyword
 
         """
         if self._root_container is None or self._cursor is None:
             return self
 
         if not self._cursor.is_locked:
             raise StreamlitAPIException("Only existing elements can `add_rows`.")
```

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/deprecation_util.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/deprecation_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/development.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/development.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/echo.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/echo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/__init__.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/alert.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/alert.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/arrow.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/arrow.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,37 +101,37 @@
 
 class DataframeState(TypedDict, total=False):
     """
     A dictionary representing the current state of the dataframe.
 
     Attributes
     ----------
-    select : DataframeSelectionState
+    selection : DataframeSelectionState
         The state of the `on_select` event.
     """
 
-    select: DataframeSelectionState
+    selection: DataframeSelectionState
 
 
 @dataclass
 class DataframeSelectionSerde:
     """DataframeSelectionSerde is used to serialize and deserialize the dataframe selection state."""
 
     def deserialize(self, ui_value: str | None, widget_id: str = "") -> DataframeState:
         empty_selection_state: DataframeState = {
-            "select": {
+            "selection": {
                 "rows": [],
                 "columns": [],
             },
         }
         selection_state: DataframeState = (
             empty_selection_state if ui_value is None else json.loads(ui_value)
         )
 
-        if "select" not in selection_state:
+        if "selection" not in selection_state:
             selection_state = empty_selection_state
 
         return cast(DataframeState, AttributeDictionary(selection_state))
 
     def serialize(self, editing_state: DataframeState) -> str:
         return json.dumps(editing_state, default=str)
```

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/balloons.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/balloons.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/bokeh_chart.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/bokeh_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/code.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/code.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/deck_gl_json_chart.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/deck_gl_json_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/dialog_decorator.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/dialog_decorator.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/doc_string.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/doc_string.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/empty.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/empty.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/exception.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/exception.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/form.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/form.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/graphviz_chart.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/graphviz_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/heading.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/heading.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/html.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/html.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/iframe.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/iframe.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/image.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/image.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/json.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/json.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/layouts.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/layouts.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/lib/__init__.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/lib/built_in_chart_utils.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/built_in_chart_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/lib/column_config_utils.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/column_config_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/lib/column_types.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/column_types.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/lib/dialog.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/dialog.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/lib/dicttools.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/dicttools.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/lib/event_utils.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/event_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/lib/mutable_status_container.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/mutable_status_container.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/lib/pandas_styler_utils.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/pandas_styler_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/lib/streamlit_plotly_theme.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/streamlit_plotly_theme.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/lib/subtitle_utils.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/subtitle_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/map.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/map.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/markdown.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/markdown.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/media.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/media.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/metric.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/metric.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/plotly_chart.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/plotly_chart.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,42 +110,42 @@
 
 class PlotlyState(TypedDict, total=False):
     """
     A dictionary representing the current selection state of the plotly chart.
 
     Attributes
     ----------
-    select : PlotlySelectionState
+    selection : PlotlySelectionState
         The state of the `on_select` event.
     """
 
-    select: PlotlySelectionState
+    selection: PlotlySelectionState
 
 
 @dataclass
 class PlotlyChartSelectionSerde:
     """PlotlyChartSelectionSerde is used to serialize and deserialize the Plotly Chart selection state."""
 
     def deserialize(self, ui_value: str | None, widget_id: str = "") -> PlotlyState:
         empty_selection_state: PlotlyState = {
-            "select": {
+            "selection": {
                 "points": [],
                 "point_indices": [],
                 "box": [],
                 "lasso": [],
             },
         }
 
         selection_state = (
             empty_selection_state
             if ui_value is None
             else cast(PlotlyState, AttributeDictionary(json.loads(ui_value)))
         )
 
-        if "select" not in selection_state:
+        if "selection" not in selection_state:
             selection_state = empty_selection_state
 
         return cast(PlotlyState, AttributeDictionary(selection_state))
 
     def serialize(self, selection_state: PlotlyState) -> str:
         return json.dumps(selection_state, default=str)
```

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/progress.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/progress.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/pyplot.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/pyplot.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/snow.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/snow.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/spinner.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/spinner.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/text.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/text.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/toast.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/toast.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/utils.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/widgets/__init__.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/widgets/button.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/button.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/widgets/camera_input.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/camera_input.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/widgets/chat.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/chat.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/widgets/checkbox.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/widgets/color_picker.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/color_picker.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/widgets/data_editor.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/data_editor.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/widgets/file_uploader.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/file_uploader.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/widgets/multiselect.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/multiselect.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/widgets/number_input.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/number_input.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/widgets/radio.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/radio.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/widgets/select_slider.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/select_slider.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/widgets/selectbox.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/selectbox.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/widgets/slider.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/widgets/text_widgets.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/text_widgets.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/widgets/time_widgets.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/time_widgets.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/elements/write.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/write.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/emojis.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/emojis.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/env_util.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/env_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/error_util.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/error_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/errors.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/errors.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/external/__init__.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/external/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/external/langchain/__init__.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/external/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/external/langchain/streamlit_callback_handler.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/external/langchain/streamlit_callback_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/file_util.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/file_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/folder_black_list.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/folder_black_list.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/git_util.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/git_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/hello/Hello.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/hello/Hello.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/hello/__init__.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/hello/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/hello/pages/0_Animation_Demo.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/hello/pages/0_Animation_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/hello/pages/1_Plotting_Demo.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/hello/pages/1_Plotting_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/hello/pages/2_Mapping_Demo.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/hello/pages/2_Mapping_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/hello/pages/3_DataFrame_Demo.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/hello/pages/3_DataFrame_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/hello/utils.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/hello/utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/js_number.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/js_number.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/logger.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/logger.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/material_icon_names.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/material_icon_names.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/net_util.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/net_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/platform.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/platform.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Alert_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Alert_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Alert_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/AppPage_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/AppPage_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/AppPage_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/AppPage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/ArrowNamedDataSet_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ArrowNamedDataSet_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/ArrowNamedDataSet_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ArrowNamedDataSet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/ArrowVegaLiteChart_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ArrowVegaLiteChart_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 _sym_db = _symbol_database.Default()
 
 
 from streamlit.proto import Arrow_pb2 as streamlit_dot_proto_dot_Arrow__pb2
 from streamlit.proto import ArrowNamedDataSet_pb2 as streamlit_dot_proto_dot_ArrowNamedDataSet__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(streamlit/proto/ArrowVegaLiteChart.proto\x1a\x1bstreamlit/proto/Arrow.proto\x1a\'streamlit/proto/ArrowNamedDataSet.proto\"\x90\x01\n\x12\x41rrowVegaLiteChart\x12\x0c\n\x04spec\x18\x01 \x01(\t\x12\x14\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x06.Arrow\x12$\n\x08\x64\x61tasets\x18\x04 \x03(\x0b\x32\x12.ArrowNamedDataSet\x12\x1b\n\x13use_container_width\x18\x05 \x01(\x08\x12\r\n\x05theme\x18\x06 \x01(\tJ\x04\x08\x03\x10\x04\x42\x37\n\x1c\x63om.snowflake.apps.streamlitB\x17\x41rrowVegaLiteChartProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(streamlit/proto/ArrowVegaLiteChart.proto\x1a\x1bstreamlit/proto/Arrow.proto\x1a\'streamlit/proto/ArrowNamedDataSet.proto\"\xc5\x01\n\x12\x41rrowVegaLiteChart\x12\x0c\n\x04spec\x18\x01 \x01(\t\x12\x14\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x06.Arrow\x12$\n\x08\x64\x61tasets\x18\x04 \x03(\x0b\x32\x12.ArrowNamedDataSet\x12\x1b\n\x13use_container_width\x18\x05 \x01(\x08\x12\r\n\x05theme\x18\x06 \x01(\t\x12\n\n\x02id\x18\x07 \x01(\t\x12\x16\n\x0eselection_mode\x18\x08 \x03(\t\x12\x0f\n\x07\x66orm_id\x18\t \x01(\tJ\x04\x08\x03\x10\x04\x42\x37\n\x1c\x63om.snowflake.apps.streamlitB\x17\x41rrowVegaLiteChartProtob\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'streamlit.proto.ArrowVegaLiteChart_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\034com.snowflake.apps.streamlitB\027ArrowVegaLiteChartProto'
   _ARROWVEGALITECHART._serialized_start=115
-  _ARROWVEGALITECHART._serialized_end=259
+  _ARROWVEGALITECHART._serialized_end=312
 # @@protoc_insertion_point(module_scope)
```

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/ArrowVegaLiteChart_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Image_pb2.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -17,55 +17,66 @@
 limitations under the License.
 """
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
-import streamlit.proto.ArrowNamedDataSet_pb2
-import streamlit.proto.Arrow_pb2
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-class ArrowVegaLiteChart(google.protobuf.message.Message):
+class Image(google.protobuf.message.Message):
+    """An image which can be displayed on the screen."""
+
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    SPEC_FIELD_NUMBER: builtins.int
-    DATA_FIELD_NUMBER: builtins.int
-    DATASETS_FIELD_NUMBER: builtins.int
-    USE_CONTAINER_WIDTH_FIELD_NUMBER: builtins.int
-    THEME_FIELD_NUMBER: builtins.int
-    spec: builtins.str
-    """The a JSON-formatted string with the Vega-Lite spec."""
-    @property
-    def data(self) -> streamlit.proto.Arrow_pb2.Arrow:
-        """The dataframe that will be used as the chart's main data source, if
-        specified using Vega-Lite's inline API.
-        """
+    URL_FIELD_NUMBER: builtins.int
+    CAPTION_FIELD_NUMBER: builtins.int
+    MARKUP_FIELD_NUMBER: builtins.int
+    url: builtins.str
+    caption: builtins.str
+    markup: builtins.str
+    """DEPRECATED: markup is not used anymore.
+    SVGs are added as data uris in the url field.
+    """
+    def __init__(
+        self,
+        *,
+        url: builtins.str = ...,
+        caption: builtins.str = ...,
+        markup: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["caption", b"caption", "markup", b"markup", "url", b"url"]) -> None: ...
+
+global___Image = Image
+
+class ImageList(google.protobuf.message.Message):
+    """A set of images."""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    IMGS_FIELD_NUMBER: builtins.int
+    WIDTH_FIELD_NUMBER: builtins.int
     @property
-    def datasets(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[streamlit.proto.ArrowNamedDataSet_pb2.ArrowNamedDataSet]:
-        """Dataframes associated with this chart using Vega-Lite's datasets API, if
-        any.
-        """
-    use_container_width: builtins.bool
-    """If True, will overwrite the chart width spec to fit to container."""
-    theme: builtins.str
-    """override the properties with a theme. Currently, only "streamlit" or None are accepted."""
+    def imgs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Image]: ...
+    width: builtins.int
+    """The width of each image.
+    >0 sets the image width explicitly
+    -1 means use the image width
+    -2 means use the column width
+    -3 means use the smaller of image width & column width
+    """
     def __init__(
         self,
         *,
-        spec: builtins.str = ...,
-        data: streamlit.proto.Arrow_pb2.Arrow | None = ...,
-        datasets: collections.abc.Iterable[streamlit.proto.ArrowNamedDataSet_pb2.ArrowNamedDataSet] | None = ...,
-        use_container_width: builtins.bool = ...,
-        theme: builtins.str = ...,
+        imgs: collections.abc.Iterable[global___Image] | None = ...,
+        width: builtins.int = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["data", b"data"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["data", b"data", "datasets", b"datasets", "spec", b"spec", "theme", b"theme", "use_container_width", b"use_container_width"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["imgs", b"imgs", "width", b"width"]) -> None: ...
 
-global___ArrowVegaLiteChart = ArrowVegaLiteChart
+global___ImageList = ImageList
```

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Arrow_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Arrow_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Arrow_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Arrow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Audio_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Audio_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Audio_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Audio_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/AutoRerun_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/AutoRerun_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/AutoRerun_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/AutoRerun_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/BackMsg_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/BackMsg_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/BackMsg_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/BackMsg_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Balloons_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Balloons_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Balloons_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Balloons_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Block_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Block_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Block_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Block_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/BokehChart_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/BokehChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/BokehChart_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/BokehChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Button_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Button_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Button_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Button_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/CameraInput_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/CameraInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/CameraInput_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/CameraInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/ChatInput_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ChatInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/ChatInput_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ChatInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Checkbox_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Checkbox_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Checkbox_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Checkbox_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/ClientState_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ClientState_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/ClientState_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ClientState_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Code_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Code_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Code_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Code_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/ColorPicker_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ColorPicker_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/ColorPicker_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ColorPicker_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Common_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Common_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Common_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Components_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Components_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Components_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Components_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/DataFrame_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DataFrame_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/DataFrame_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DataFrame_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/DateInput_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DateInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/DateInput_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DateInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/DeckGlJsonChart_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DeckGlJsonChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/DeckGlJsonChart_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DeckGlJsonChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Delta_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Delta_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Delta_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Delta_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/DocString_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DocString_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/DocString_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DocString_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/DownloadButton_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DownloadButton_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/DownloadButton_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DownloadButton_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Element_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Element_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Element_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Element_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Empty_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Empty_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Empty_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Empty_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Exception_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Exception_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Exception_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Exception_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Favicon_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Favicon_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Favicon_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Favicon_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/FileUploader_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/FileUploader_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/FileUploader_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/FileUploader_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/ForwardMsg_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ForwardMsg_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/ForwardMsg_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ForwardMsg_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/GitInfo_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/GitInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/GitInfo_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/GitInfo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/GraphVizChart_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/GraphVizChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/GraphVizChart_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/GraphVizChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Heading_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Heading_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Heading_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Heading_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Html_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Html_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Html_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Html_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/IFrame_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/IFrame_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/IFrame_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/IFrame_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Image_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Image_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Image_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/LinkButton_pb2.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -13,70 +13,46 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import builtins
-import collections.abc
 import google.protobuf.descriptor
-import google.protobuf.internal.containers
 import google.protobuf.message
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-class Image(google.protobuf.message.Message):
-    """An image which can be displayed on the screen."""
-
+class LinkButton(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    LABEL_FIELD_NUMBER: builtins.int
+    HELP_FIELD_NUMBER: builtins.int
     URL_FIELD_NUMBER: builtins.int
-    CAPTION_FIELD_NUMBER: builtins.int
-    MARKUP_FIELD_NUMBER: builtins.int
+    DISABLED_FIELD_NUMBER: builtins.int
+    USE_CONTAINER_WIDTH_FIELD_NUMBER: builtins.int
+    TYPE_FIELD_NUMBER: builtins.int
+    label: builtins.str
+    help: builtins.str
     url: builtins.str
-    caption: builtins.str
-    markup: builtins.str
-    """DEPRECATED: markup is not used anymore.
-    SVGs are added as data uris in the url field.
-    """
+    disabled: builtins.bool
+    use_container_width: builtins.bool
+    type: builtins.str
     def __init__(
         self,
         *,
+        label: builtins.str = ...,
+        help: builtins.str = ...,
         url: builtins.str = ...,
-        caption: builtins.str = ...,
-        markup: builtins.str = ...,
-    ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["caption", b"caption", "markup", b"markup", "url", b"url"]) -> None: ...
-
-global___Image = Image
-
-class ImageList(google.protobuf.message.Message):
-    """A set of images."""
-
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-    IMGS_FIELD_NUMBER: builtins.int
-    WIDTH_FIELD_NUMBER: builtins.int
-    @property
-    def imgs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Image]: ...
-    width: builtins.int
-    """The width of each image.
-    >0 sets the image width explicitly
-    -1 means use the image width
-    -2 means use the column width
-    -3 means use the smaller of image width & column width
-    """
-    def __init__(
-        self,
-        *,
-        imgs: collections.abc.Iterable[global___Image] | None = ...,
-        width: builtins.int = ...,
+        disabled: builtins.bool = ...,
+        use_container_width: builtins.bool = ...,
+        type: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["imgs", b"imgs", "width", b"width"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["disabled", b"disabled", "help", b"help", "label", b"label", "type", b"type", "url", b"url", "use_container_width", b"use_container_width"]) -> None: ...
 
-global___ImageList = ImageList
+global___LinkButton = LinkButton
```

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Json_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Json_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Json_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Json_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/LabelVisibilityMessage_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/LabelVisibilityMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/LabelVisibilityMessage_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/LabelVisibilityMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/LinkButton_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/LinkButton_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/LinkButton_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageLink_pb2.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -24,35 +24,43 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-class LinkButton(google.protobuf.message.Message):
+class PageLink(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    PAGE_FIELD_NUMBER: builtins.int
     LABEL_FIELD_NUMBER: builtins.int
+    ICON_FIELD_NUMBER: builtins.int
+    PAGE_SCRIPT_HASH_FIELD_NUMBER: builtins.int
     HELP_FIELD_NUMBER: builtins.int
-    URL_FIELD_NUMBER: builtins.int
-    DISABLED_FIELD_NUMBER: builtins.int
     USE_CONTAINER_WIDTH_FIELD_NUMBER: builtins.int
-    TYPE_FIELD_NUMBER: builtins.int
+    DISABLED_FIELD_NUMBER: builtins.int
+    EXTERNAL_FIELD_NUMBER: builtins.int
+    page: builtins.str
     label: builtins.str
+    icon: builtins.str
+    page_script_hash: builtins.str
     help: builtins.str
-    url: builtins.str
-    disabled: builtins.bool
     use_container_width: builtins.bool
-    type: builtins.str
+    disabled: builtins.bool
+    external: builtins.bool
     def __init__(
         self,
         *,
+        page: builtins.str = ...,
         label: builtins.str = ...,
+        icon: builtins.str = ...,
+        page_script_hash: builtins.str = ...,
         help: builtins.str = ...,
-        url: builtins.str = ...,
+        use_container_width: builtins.bool | None = ...,
         disabled: builtins.bool = ...,
-        use_container_width: builtins.bool = ...,
-        type: builtins.str = ...,
+        external: builtins.bool = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["disabled", b"disabled", "help", b"help", "label", b"label", "type", b"type", "url", b"url", "use_container_width", b"use_container_width"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_use_container_width", b"_use_container_width", "use_container_width", b"use_container_width"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_use_container_width", b"_use_container_width", "disabled", b"disabled", "external", b"external", "help", b"help", "icon", b"icon", "label", b"label", "page", b"page", "page_script_hash", b"page_script_hash", "use_container_width", b"use_container_width"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_use_container_width", b"_use_container_width"]) -> typing_extensions.Literal["use_container_width"] | None: ...
 
-global___LinkButton = LinkButton
+global___PageLink = PageLink
```

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Logo_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Logo_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Logo_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Logo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Markdown_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Markdown_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Markdown_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Markdown_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Metric_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Metric_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Metric_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Metric_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/MultiSelect_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/MultiSelect_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/MultiSelect_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/MultiSelect_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/NamedDataSet_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/NamedDataSet_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/NamedDataSet_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/NamedDataSet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/NewSession_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/NewSession_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/NewSession_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/NewSession_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/NumberInput_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/NumberInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/NumberInput_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/NumberInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/PageConfig_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageConfig_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/PageConfig_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageConfig_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/PageInfo_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/PageInfo_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageInfo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/PageLink_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageLink_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/PageLink_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Selectbox_pb2.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -13,54 +13,72 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import builtins
+import collections.abc
 import google.protobuf.descriptor
+import google.protobuf.internal.containers
 import google.protobuf.message
+import streamlit.proto.LabelVisibilityMessage_pb2
 import sys
+import typing
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-class PageLink(google.protobuf.message.Message):
+class Selectbox(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    PAGE_FIELD_NUMBER: builtins.int
+    ID_FIELD_NUMBER: builtins.int
     LABEL_FIELD_NUMBER: builtins.int
-    ICON_FIELD_NUMBER: builtins.int
-    PAGE_SCRIPT_HASH_FIELD_NUMBER: builtins.int
+    DEFAULT_FIELD_NUMBER: builtins.int
+    OPTIONS_FIELD_NUMBER: builtins.int
     HELP_FIELD_NUMBER: builtins.int
-    USE_CONTAINER_WIDTH_FIELD_NUMBER: builtins.int
+    FORM_ID_FIELD_NUMBER: builtins.int
+    VALUE_FIELD_NUMBER: builtins.int
+    SET_VALUE_FIELD_NUMBER: builtins.int
     DISABLED_FIELD_NUMBER: builtins.int
-    EXTERNAL_FIELD_NUMBER: builtins.int
-    page: builtins.str
+    LABEL_VISIBILITY_FIELD_NUMBER: builtins.int
+    PLACEHOLDER_FIELD_NUMBER: builtins.int
+    id: builtins.str
     label: builtins.str
-    icon: builtins.str
-    page_script_hash: builtins.str
+    default: builtins.int
+    @property
+    def options(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
     help: builtins.str
-    use_container_width: builtins.bool
+    form_id: builtins.str
+    value: builtins.int
+    set_value: builtins.bool
     disabled: builtins.bool
-    external: builtins.bool
+    @property
+    def label_visibility(self) -> streamlit.proto.LabelVisibilityMessage_pb2.LabelVisibilityMessage: ...
+    placeholder: builtins.str
     def __init__(
         self,
         *,
-        page: builtins.str = ...,
+        id: builtins.str = ...,
         label: builtins.str = ...,
-        icon: builtins.str = ...,
-        page_script_hash: builtins.str = ...,
+        default: builtins.int | None = ...,
+        options: collections.abc.Iterable[builtins.str] | None = ...,
         help: builtins.str = ...,
-        use_container_width: builtins.bool | None = ...,
+        form_id: builtins.str = ...,
+        value: builtins.int | None = ...,
+        set_value: builtins.bool = ...,
         disabled: builtins.bool = ...,
-        external: builtins.bool = ...,
+        label_visibility: streamlit.proto.LabelVisibilityMessage_pb2.LabelVisibilityMessage | None = ...,
+        placeholder: builtins.str = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_use_container_width", b"_use_container_width", "use_container_width", b"use_container_width"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_use_container_width", b"_use_container_width", "disabled", b"disabled", "external", b"external", "help", b"help", "icon", b"icon", "label", b"label", "page", b"page", "page_script_hash", b"page_script_hash", "use_container_width", b"use_container_width"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["_use_container_width", b"_use_container_width"]) -> typing_extensions.Literal["use_container_width"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_default", b"_default", "_value", b"_value", "default", b"default", "label_visibility", b"label_visibility", "value", b"value"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_default", b"_default", "_value", b"_value", "default", b"default", "disabled", b"disabled", "form_id", b"form_id", "help", b"help", "id", b"id", "label", b"label", "label_visibility", b"label_visibility", "options", b"options", "placeholder", b"placeholder", "set_value", b"set_value", "value", b"value"]) -> None: ...
+    @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_default", b"_default"]) -> typing_extensions.Literal["default"] | None: ...
+    @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_value", b"_value"]) -> typing_extensions.Literal["value"] | None: ...
 
-global___PageLink = PageLink
+global___Selectbox = Selectbox
```

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/PageNotFound_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageNotFound_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/PageNotFound_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageNotFound_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/PageProfile_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageProfile_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/PageProfile_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageProfile_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/PagesChanged_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PagesChanged_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/PagesChanged_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PagesChanged_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/ParentMessage_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ParentMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/ParentMessage_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ParentMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/PlotlyChart_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PlotlyChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/PlotlyChart_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PlotlyChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Progress_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Progress_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Progress_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Progress_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Radio_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Radio_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Radio_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Radio_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/RootContainer_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/RootContainer_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/RootContainer_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/RootContainer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Selectbox_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Selectbox_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Selectbox_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/TextArea_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -13,72 +13,72 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import builtins
-import collections.abc
 import google.protobuf.descriptor
-import google.protobuf.internal.containers
 import google.protobuf.message
 import streamlit.proto.LabelVisibilityMessage_pb2
 import sys
 import typing
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-class Selectbox(google.protobuf.message.Message):
+class TextArea(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ID_FIELD_NUMBER: builtins.int
     LABEL_FIELD_NUMBER: builtins.int
     DEFAULT_FIELD_NUMBER: builtins.int
-    OPTIONS_FIELD_NUMBER: builtins.int
+    HEIGHT_FIELD_NUMBER: builtins.int
+    MAX_CHARS_FIELD_NUMBER: builtins.int
     HELP_FIELD_NUMBER: builtins.int
     FORM_ID_FIELD_NUMBER: builtins.int
     VALUE_FIELD_NUMBER: builtins.int
     SET_VALUE_FIELD_NUMBER: builtins.int
+    PLACEHOLDER_FIELD_NUMBER: builtins.int
     DISABLED_FIELD_NUMBER: builtins.int
     LABEL_VISIBILITY_FIELD_NUMBER: builtins.int
-    PLACEHOLDER_FIELD_NUMBER: builtins.int
     id: builtins.str
     label: builtins.str
-    default: builtins.int
-    @property
-    def options(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
+    default: builtins.str
+    height: builtins.int
+    max_chars: builtins.int
     help: builtins.str
     form_id: builtins.str
-    value: builtins.int
+    value: builtins.str
     set_value: builtins.bool
+    placeholder: builtins.str
     disabled: builtins.bool
     @property
     def label_visibility(self) -> streamlit.proto.LabelVisibilityMessage_pb2.LabelVisibilityMessage: ...
-    placeholder: builtins.str
     def __init__(
         self,
         *,
         id: builtins.str = ...,
         label: builtins.str = ...,
-        default: builtins.int | None = ...,
-        options: collections.abc.Iterable[builtins.str] | None = ...,
+        default: builtins.str | None = ...,
+        height: builtins.int = ...,
+        max_chars: builtins.int = ...,
         help: builtins.str = ...,
         form_id: builtins.str = ...,
-        value: builtins.int | None = ...,
+        value: builtins.str | None = ...,
         set_value: builtins.bool = ...,
+        placeholder: builtins.str = ...,
         disabled: builtins.bool = ...,
         label_visibility: streamlit.proto.LabelVisibilityMessage_pb2.LabelVisibilityMessage | None = ...,
-        placeholder: builtins.str = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["_default", b"_default", "_value", b"_value", "default", b"default", "label_visibility", b"label_visibility", "value", b"value"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_default", b"_default", "_value", b"_value", "default", b"default", "disabled", b"disabled", "form_id", b"form_id", "help", b"help", "id", b"id", "label", b"label", "label_visibility", b"label_visibility", "options", b"options", "placeholder", b"placeholder", "set_value", b"set_value", "value", b"value"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_default", b"_default", "_value", b"_value", "default", b"default", "disabled", b"disabled", "form_id", b"form_id", "height", b"height", "help", b"help", "id", b"id", "label", b"label", "label_visibility", b"label_visibility", "max_chars", b"max_chars", "placeholder", b"placeholder", "set_value", b"set_value", "value", b"value"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_default", b"_default"]) -> typing_extensions.Literal["default"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_value", b"_value"]) -> typing_extensions.Literal["value"] | None: ...
 
-global___Selectbox = Selectbox
+global___TextArea = TextArea
```

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/SessionEvent_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/SessionEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/SessionEvent_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/SessionEvent_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/SessionStatus_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/SessionStatus_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/SessionStatus_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/SessionStatus_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Skeleton_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Skeleton_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Skeleton_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Skeleton_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Slider_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Slider_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Slider_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Slider_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Snow_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Snow_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Snow_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Snow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Spinner_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Spinner_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Spinner_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Spinner_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/TextArea_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/TextArea_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/TextArea_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/TimeInput_pb2.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -26,59 +26,53 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-class TextArea(google.protobuf.message.Message):
+class TimeInput(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ID_FIELD_NUMBER: builtins.int
     LABEL_FIELD_NUMBER: builtins.int
     DEFAULT_FIELD_NUMBER: builtins.int
-    HEIGHT_FIELD_NUMBER: builtins.int
-    MAX_CHARS_FIELD_NUMBER: builtins.int
     HELP_FIELD_NUMBER: builtins.int
     FORM_ID_FIELD_NUMBER: builtins.int
     VALUE_FIELD_NUMBER: builtins.int
     SET_VALUE_FIELD_NUMBER: builtins.int
-    PLACEHOLDER_FIELD_NUMBER: builtins.int
     DISABLED_FIELD_NUMBER: builtins.int
     LABEL_VISIBILITY_FIELD_NUMBER: builtins.int
+    STEP_FIELD_NUMBER: builtins.int
     id: builtins.str
     label: builtins.str
     default: builtins.str
-    height: builtins.int
-    max_chars: builtins.int
     help: builtins.str
     form_id: builtins.str
     value: builtins.str
     set_value: builtins.bool
-    placeholder: builtins.str
     disabled: builtins.bool
     @property
     def label_visibility(self) -> streamlit.proto.LabelVisibilityMessage_pb2.LabelVisibilityMessage: ...
+    step: builtins.int
     def __init__(
         self,
         *,
         id: builtins.str = ...,
         label: builtins.str = ...,
         default: builtins.str | None = ...,
-        height: builtins.int = ...,
-        max_chars: builtins.int = ...,
         help: builtins.str = ...,
         form_id: builtins.str = ...,
         value: builtins.str | None = ...,
         set_value: builtins.bool = ...,
-        placeholder: builtins.str = ...,
         disabled: builtins.bool = ...,
         label_visibility: streamlit.proto.LabelVisibilityMessage_pb2.LabelVisibilityMessage | None = ...,
+        step: builtins.int = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["_default", b"_default", "_value", b"_value", "default", b"default", "label_visibility", b"label_visibility", "value", b"value"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_default", b"_default", "_value", b"_value", "default", b"default", "disabled", b"disabled", "form_id", b"form_id", "height", b"height", "help", b"help", "id", b"id", "label", b"label", "label_visibility", b"label_visibility", "max_chars", b"max_chars", "placeholder", b"placeholder", "set_value", b"set_value", "value", b"value"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_default", b"_default", "_value", b"_value", "default", b"default", "disabled", b"disabled", "form_id", b"form_id", "help", b"help", "id", b"id", "label", b"label", "label_visibility", b"label_visibility", "set_value", b"set_value", "step", b"step", "value", b"value"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_default", b"_default"]) -> typing_extensions.Literal["default"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_value", b"_value"]) -> typing_extensions.Literal["value"] | None: ...
 
-global___TextArea = TextArea
+global___TimeInput = TimeInput
```

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/TextInput_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/TextInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/TextInput_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/TextInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Text_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Text_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Text_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Text_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/TimeInput_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/TimeInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/TimeInput_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ArrowVegaLiteChart_pb2.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -13,66 +13,72 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import builtins
+import collections.abc
 import google.protobuf.descriptor
+import google.protobuf.internal.containers
 import google.protobuf.message
-import streamlit.proto.LabelVisibilityMessage_pb2
+import streamlit.proto.ArrowNamedDataSet_pb2
+import streamlit.proto.Arrow_pb2
 import sys
-import typing
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-class TimeInput(google.protobuf.message.Message):
+class ArrowVegaLiteChart(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    SPEC_FIELD_NUMBER: builtins.int
+    DATA_FIELD_NUMBER: builtins.int
+    DATASETS_FIELD_NUMBER: builtins.int
+    USE_CONTAINER_WIDTH_FIELD_NUMBER: builtins.int
+    THEME_FIELD_NUMBER: builtins.int
     ID_FIELD_NUMBER: builtins.int
-    LABEL_FIELD_NUMBER: builtins.int
-    DEFAULT_FIELD_NUMBER: builtins.int
-    HELP_FIELD_NUMBER: builtins.int
+    SELECTION_MODE_FIELD_NUMBER: builtins.int
     FORM_ID_FIELD_NUMBER: builtins.int
-    VALUE_FIELD_NUMBER: builtins.int
-    SET_VALUE_FIELD_NUMBER: builtins.int
-    DISABLED_FIELD_NUMBER: builtins.int
-    LABEL_VISIBILITY_FIELD_NUMBER: builtins.int
-    STEP_FIELD_NUMBER: builtins.int
+    spec: builtins.str
+    """The a JSON-formatted string with the Vega-Lite spec."""
+    @property
+    def data(self) -> streamlit.proto.Arrow_pb2.Arrow:
+        """The dataframe that will be used as the chart's main data source, if
+        specified using Vega-Lite's inline API.
+        """
+    @property
+    def datasets(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[streamlit.proto.ArrowNamedDataSet_pb2.ArrowNamedDataSet]:
+        """Dataframes associated with this chart using Vega-Lite's datasets API, if
+        any. The data is either in `data` field or in the `datasets` field.
+        """
+    use_container_width: builtins.bool
+    """If True, will overwrite the chart width spec to fit to container."""
+    theme: builtins.str
+    """override the properties with a theme. Currently, only "streamlit" or None are accepted."""
     id: builtins.str
-    label: builtins.str
-    default: builtins.str
-    help: builtins.str
-    form_id: builtins.str
-    value: builtins.str
-    set_value: builtins.bool
-    disabled: builtins.bool
+    """ID, required for selection events."""
     @property
-    def label_visibility(self) -> streamlit.proto.LabelVisibilityMessage_pb2.LabelVisibilityMessage: ...
-    step: builtins.int
+    def selection_mode(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
+        """Named selection parameters that are activated to trigger reruns."""
+    form_id: builtins.str
+    """The form ID of the widget, this is required if selections are activated on the chart."""
     def __init__(
         self,
         *,
+        spec: builtins.str = ...,
+        data: streamlit.proto.Arrow_pb2.Arrow | None = ...,
+        datasets: collections.abc.Iterable[streamlit.proto.ArrowNamedDataSet_pb2.ArrowNamedDataSet] | None = ...,
+        use_container_width: builtins.bool = ...,
+        theme: builtins.str = ...,
         id: builtins.str = ...,
-        label: builtins.str = ...,
-        default: builtins.str | None = ...,
-        help: builtins.str = ...,
+        selection_mode: collections.abc.Iterable[builtins.str] | None = ...,
         form_id: builtins.str = ...,
-        value: builtins.str | None = ...,
-        set_value: builtins.bool = ...,
-        disabled: builtins.bool = ...,
-        label_visibility: streamlit.proto.LabelVisibilityMessage_pb2.LabelVisibilityMessage | None = ...,
-        step: builtins.int = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_default", b"_default", "_value", b"_value", "default", b"default", "label_visibility", b"label_visibility", "value", b"value"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_default", b"_default", "_value", b"_value", "default", b"default", "disabled", b"disabled", "form_id", b"form_id", "help", b"help", "id", b"id", "label", b"label", "label_visibility", b"label_visibility", "set_value", b"set_value", "step", b"step", "value", b"value"]) -> None: ...
-    @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["_default", b"_default"]) -> typing_extensions.Literal["default"] | None: ...
-    @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["_value", b"_value"]) -> typing_extensions.Literal["value"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["data", b"data"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["data", b"data", "datasets", b"datasets", "form_id", b"form_id", "id", b"id", "selection_mode", b"selection_mode", "spec", b"spec", "theme", b"theme", "use_container_width", b"use_container_width"]) -> None: ...
 
-global___TimeInput = TimeInput
+global___ArrowVegaLiteChart = ArrowVegaLiteChart
```

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Toast_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Toast_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Toast_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Toast_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/VegaLiteChart_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/VegaLiteChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/VegaLiteChart_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/VegaLiteChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Video_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Video_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/Video_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Video_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/WidgetStates_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/WidgetStates_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/WidgetStates_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/WidgetStates_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/__init__.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/openmetrics_data_model_pb2.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/openmetrics_data_model_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/proto/openmetrics_data_model_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/openmetrics_data_model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/__init__.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/app_session.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/app_session.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/caching/__init__.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/caching/cache_data_api.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/cache_data_api.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/caching/cache_errors.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/cache_errors.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/caching/cache_resource_api.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/cache_resource_api.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/caching/cache_type.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/cache_type.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/caching/cache_utils.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/cache_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/caching/cached_message_replay.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/cached_message_replay.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/caching/hashing.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/hashing.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/caching/storage/__init__.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/caching/storage/cache_storage_protocol.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/storage/cache_storage_protocol.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/caching/storage/dummy_cache_storage.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/storage/dummy_cache_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/caching/storage/local_disk_cache_storage.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/storage/local_disk_cache_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/connection_factory.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/connection_factory.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/credentials.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/credentials.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/forward_msg_cache.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/forward_msg_cache.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/forward_msg_queue.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/forward_msg_queue.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/fragment.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/fragment.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/legacy_caching/__init__.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/legacy_caching/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/legacy_caching/caching.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/legacy_caching/caching.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/legacy_caching/hashing.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/legacy_caching/hashing.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/media_file_manager.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/media_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/media_file_storage.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/media_file_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/memory_media_file_storage.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/memory_media_file_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/memory_session_storage.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/memory_session_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/memory_uploaded_file_manager.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/memory_uploaded_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/metrics_util.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/metrics_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/runtime.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/runtime.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/runtime_util.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/runtime_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/script_data.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/script_data.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/scriptrunner/__init__.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/scriptrunner/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/scriptrunner/magic.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/scriptrunner/magic.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/scriptrunner/magic_funcs.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/scriptrunner/magic_funcs.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/scriptrunner/script_cache.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/scriptrunner/script_cache.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/scriptrunner/script_requests.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/scriptrunner/script_requests.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/scriptrunner/script_run_context.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/scriptrunner/script_run_context.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/scriptrunner/script_runner.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/scriptrunner/script_runner.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/secrets.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/secrets.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/session_manager.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/session_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/state/__init__.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/state/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/state/common.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/state/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 
 from google.protobuf.message import Message
 from typing_extensions import TypeAlias
 
 from streamlit import config, util
 from streamlit.errors import StreamlitAPIException
 from streamlit.proto.Arrow_pb2 import Arrow
+from streamlit.proto.ArrowVegaLiteChart_pb2 import ArrowVegaLiteChart
 from streamlit.proto.Button_pb2 import Button
 from streamlit.proto.CameraInput_pb2 import CameraInput
 from streamlit.proto.ChatInput_pb2 import ChatInput
 from streamlit.proto.Checkbox_pb2 import Checkbox
 from streamlit.proto.ColorPicker_pb2 import ColorPicker
 from streamlit.proto.Components_pb2 import ComponentInstance
 from streamlit.proto.DateInput_pb2 import DateInput
@@ -65,32 +66,33 @@
     from streamlit.runtime.scriptrunner.script_run_context import ScriptRunContext
     from streamlit.runtime.state.widgets import NoValue
 
 
 # Protobuf types for all widgets.
 WidgetProto: TypeAlias = Union[
     Arrow,
+    ArrowVegaLiteChart,
     Button,
     CameraInput,
     ChatInput,
     Checkbox,
     ColorPicker,
     ComponentInstance,
     DateInput,
     DownloadButton,
     FileUploader,
     MultiSelect,
     NumberInput,
+    PlotlyChart,
     Radio,
     Selectbox,
     Slider,
     TextArea,
     TextInput,
     TimeInput,
-    PlotlyChart,
 ]
 
 GENERATED_WIDGET_ID_PREFIX: Final = "$$WIDGET_ID"
 TESTING_KEY = "$$STREAMLIT_INTERNAL_KEY_TESTING"
 
 
 T = TypeVar("T")
```

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/state/query_params.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/state/query_params.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/state/query_params_proxy.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/state/query_params_proxy.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/state/safe_session_state.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/state/safe_session_state.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/state/session_state.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/state/session_state.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/state/session_state_proxy.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/state/session_state_proxy.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/state/widgets.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/state/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
         "plotly_chart": "string_value",
         "radio": "int_value",
         "selectbox": "int_value",
         "slider": "double_array_value",
         "text_area": "string_value",
         "text_input": "string_value",
         "time_input": "string_value",
+        "vega_lite_chart": "string_value",
     }
 )
 
 
 class NoValue:
     """Return this from DeltaGenerator.foo_widget() when you want the st.foo_widget()
     call to return None. This is needed because `DeltaGenerator._enqueue`
```

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/stats.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/stats.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/uploaded_file_manager.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/uploaded_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/runtime/websocket_session_manager.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/websocket_session_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/source_util.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/source_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/asset-manifest.json` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/asset-manifest.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8227124183006536%*

 * *Differences: {"'entrypoints'": "{insert: [(1, 'static/js/main.32c71338.js')], delete: [1]}",*

 * * "'files'": "{'main.js': './static/js/main.32c71338.js', 'static/js/8148.a5f74d47.chunk.js': "*

 * *            "'./static/js/8148.a5f74d47.chunk.js', 'static/js/5441.1b94928f.chunk.js': "*

 * *            "'./static/js/5441.1b94928f.chunk.js', 'static/js/1168.14f7c6ff.chunk.js': "*

 * *            "'./static/js/1168.14f7c6ff.chunk.js', delete: ['static/js/8148.cc5b50d8.chunk.js', "*

 * *            "'static/js/5441.5bacdeda.chunk.js', 'static/js/1 […]*

```diff
@@ -1,21 +1,21 @@
 {
     "entrypoints": [
         "static/css/main.3aaaea00.css",
-        "static/js/main.45247b52.js"
+        "static/js/main.32c71338.js"
     ],
     "files": {
         "index.html": "./index.html",
         "main.css": "./static/css/main.3aaaea00.css",
-        "main.js": "./static/js/main.45247b52.js",
+        "main.js": "./static/js/main.32c71338.js",
         "static/css/3466.8b8f33d6.chunk.css": "./static/css/3466.8b8f33d6.chunk.css",
         "static/css/5441.e3b876c5.chunk.css": "./static/css/5441.e3b876c5.chunk.css",
         "static/css/8148.49dfd2ce.chunk.css": "./static/css/8148.49dfd2ce.chunk.css",
         "static/js/1074.73973756.chunk.js": "./static/js/1074.73973756.chunk.js",
-        "static/js/1168.7452e363.chunk.js": "./static/js/1168.7452e363.chunk.js",
+        "static/js/1168.14f7c6ff.chunk.js": "./static/js/1168.14f7c6ff.chunk.js",
         "static/js/1307.0f0cca93.chunk.js": "./static/js/1307.0f0cca93.chunk.js",
         "static/js/1451.3b0a3e31.chunk.js": "./static/js/1451.3b0a3e31.chunk.js",
         "static/js/1479.6709db03.chunk.js": "./static/js/1479.6709db03.chunk.js",
         "static/js/178.7bea8c5d.chunk.js": "./static/js/178.7bea8c5d.chunk.js",
         "static/js/1792.8bd6ce2a.chunk.js": "./static/js/1792.8bd6ce2a.chunk.js",
         "static/js/2178.90362aae.chunk.js": "./static/js/2178.90362aae.chunk.js",
         "static/js/2187.9469f035.chunk.js": "./static/js/2187.9469f035.chunk.js",
@@ -37,29 +37,29 @@
         "static/js/4666.c4b22a63.chunk.js": "./static/js/4666.c4b22a63.chunk.js",
         "static/js/474.87506447.chunk.js": "./static/js/474.87506447.chunk.js",
         "static/js/5106.44f0ff51.chunk.js": "./static/js/5106.44f0ff51.chunk.js",
         "static/js/5117.04bfe5d3.chunk.js": "./static/js/5117.04bfe5d3.chunk.js",
         "static/js/5249.f2f4070d.chunk.js": "./static/js/5249.f2f4070d.chunk.js",
         "static/js/5345.65c91ee7.chunk.js": "./static/js/5345.65c91ee7.chunk.js",
         "static/js/5379.6571574f.chunk.js": "./static/js/5379.6571574f.chunk.js",
-        "static/js/5441.5bacdeda.chunk.js": "./static/js/5441.5bacdeda.chunk.js",
+        "static/js/5441.1b94928f.chunk.js": "./static/js/5441.1b94928f.chunk.js",
         "static/js/5791.9a42fb4b.chunk.js": "./static/js/5791.9a42fb4b.chunk.js",
         "static/js/6013.4ba2d616.chunk.js": "./static/js/6013.4ba2d616.chunk.js",
         "static/js/6405.ac5a6f23.chunk.js": "./static/js/6405.ac5a6f23.chunk.js",
         "static/js/6718.802da17e.chunk.js": "./static/js/6718.802da17e.chunk.js",
         "static/js/6853.93dd1c4c.chunk.js": "./static/js/6853.93dd1c4c.chunk.js",
         "static/js/6950.70fe55c2.chunk.js": "./static/js/6950.70fe55c2.chunk.js",
         "static/js/7142.83028745.chunk.js": "./static/js/7142.83028745.chunk.js",
         "static/js/7175.be4076bc.chunk.js": "./static/js/7175.be4076bc.chunk.js",
         "static/js/7323.b74cc85b.chunk.js": "./static/js/7323.b74cc85b.chunk.js",
         "static/js/7483.64f23be7.chunk.js": "./static/js/7483.64f23be7.chunk.js",
         "static/js/7602.e8abc06b.chunk.js": "./static/js/7602.e8abc06b.chunk.js",
         "static/js/7805.acc6316a.chunk.js": "./static/js/7805.acc6316a.chunk.js",
         "static/js/8005.43974a35.chunk.js": "./static/js/8005.43974a35.chunk.js",
-        "static/js/8148.cc5b50d8.chunk.js": "./static/js/8148.cc5b50d8.chunk.js",
+        "static/js/8148.a5f74d47.chunk.js": "./static/js/8148.a5f74d47.chunk.js",
         "static/js/8427.bd0a7cf3.chunk.js": "./static/js/8427.bd0a7cf3.chunk.js",
         "static/js/8477.de889fe5.chunk.js": "./static/js/8477.de889fe5.chunk.js",
         "static/js/8492.0d93bd08.chunk.js": "./static/js/8492.0d93bd08.chunk.js",
         "static/js/8536.f8de3d9a.chunk.js": "./static/js/8536.f8de3d9a.chunk.js",
         "static/js/8570.6de19120.chunk.js": "./static/js/8570.6de19120.chunk.js",
         "static/js/8691.9ccf7f89.chunk.js": "./static/js/8691.9ccf7f89.chunk.js",
         "static/js/9330.2b4c99e0.chunk.js": "./static/js/9330.2b4c99e0.chunk.js",
```

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/favicon.png` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/favicon.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/index.html` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1,shrink-to-fit=no"/><link rel="shortcut icon" href="./favicon.png"/><link rel="preload" href="./static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2" as="font" type="font/woff2" crossorigin><link rel="preload" href="./static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2" as="font" type="font/woff2" crossorigin><link rel="preload" href="./static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2" as="font" type="font/woff2" crossorigin><title>Streamlit</title><script>window.prerenderReady=!1</script><script defer="defer" src="./static/js/main.45247b52.js"></script><link href="./static/css/main.3aaaea00.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
+<!doctype html><html lang="en"><head><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1,shrink-to-fit=no"/><link rel="shortcut icon" href="./favicon.png"/><link rel="preload" href="./static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2" as="font" type="font/woff2" crossorigin><link rel="preload" href="./static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2" as="font" type="font/woff2" crossorigin><link rel="preload" href="./static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2" as="font" type="font/woff2" crossorigin><title>Streamlit</title><script>window.prerenderReady=!1</script><script defer="defer" src="./static/js/main.32c71338.js"></script><link href="./static/css/main.3aaaea00.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
```

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/css/3466.8b8f33d6.chunk.css` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/css/3466.8b8f33d6.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/css/5441.e3b876c5.chunk.css` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/css/5441.e3b876c5.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/css/8148.49dfd2ce.chunk.css` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/css/8148.49dfd2ce.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/css/main.3aaaea00.css` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/css/main.3aaaea00.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/1074.73973756.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/1074.73973756.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/1168.7452e363.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/1168.14f7c6ff.chunk.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -287,15 +287,15 @@
                     }
                 }(l.layout, t), l
             }
 
             function A(e, o, t, l) {
                 if (!e) return;
                 const n = {
-                        select: {
+                        selection: {
                             points: [],
                             point_indices: [],
                             box: [],
                             lasso: []
                         }
                     },
                     i = new Set,
@@ -353,16 +353,16 @@
                                     xref: e.xref,
                                     yref: e.yref,
                                     x: o.x,
                                     y: o.y
                                 };
                             a.push(t)
                         }
-                    })), n.select.point_indices = Array.from(i), n.select.points = d.map((e => (0, c.KI)(e))), n.select.box = s, n.select.lasso = a, n.select.box.length > 0 && !t.selectionMode.includes(r.hP.SelectionMode.BOX)) return;
-                if (n.select.lasso.length > 0 && !t.selectionMode.includes(r.hP.SelectionMode.LASSO)) return;
+                    })), n.selection.point_indices = Array.from(i), n.selection.points = d.map((e => (0, c.KI)(e))), n.selection.box = s, n.selection.lasso = a, n.selection.box.length > 0 && !t.selectionMode.includes(r.hP.SelectionMode.BOX)) return;
+                if (n.selection.lasso.length > 0 && !t.selectionMode.includes(r.hP.SelectionMode.LASSO)) return;
                 const h = o.getStringValue(t),
                     m = JSON.stringify(n);
                 h !== m && o.setStringValue(t, m, {
                     fromUi: !0
                 }, l)
             }
             const w = (0, s.Z)((function(e) {
@@ -439,15 +439,15 @@
                         A(e, m, p, y)
                     }), [p.id, m, y]),
                     V = (0, l.useCallback)((function() {
                         let e = !(arguments.length > 0 && void 0 !== arguments[0]) || arguments[0];
                         ! function(e, o, t) {
                             const l = e.getStringValue(o),
                                 n = JSON.stringify({
-                                    select: {
+                                    selection: {
                                         points: [],
                                         point_indices: [],
                                         box: [],
                                         lasso: []
                                     }
                                 });
                             l !== n && e.setStringValue(o, n, {
```

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/1307.0f0cca93.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/1307.0f0cca93.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/1451.3b0a3e31.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/1451.3b0a3e31.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/1479.6709db03.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/1479.6709db03.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/178.7bea8c5d.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/178.7bea8c5d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/1792.8bd6ce2a.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/1792.8bd6ce2a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/2178.90362aae.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/2178.90362aae.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/2187.9469f035.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/2187.9469f035.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/2469.09ea79bb.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/2469.09ea79bb.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/2634.1249dc7a.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/2634.1249dc7a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/2736.4336e2b9.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/2736.4336e2b9.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/3053.7e70ec3b.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/3053.7e70ec3b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/329.464ed8ec.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/329.464ed8ec.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/329.464ed8ec.chunk.js.LICENSE.txt` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/329.464ed8ec.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/3301.1d1b10bb.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/3301.1d1b10bb.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/3466.05d62820.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/3466.05d62820.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/3466.05d62820.chunk.js.LICENSE.txt` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/3466.05d62820.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/3513.7dedbda2.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/3513.7dedbda2.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/3631.be5c35fa.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/3631.be5c35fa.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/4113.99983645.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/4113.99983645.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/4132.49bf3f2c.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/4132.49bf3f2c.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/4177.69f9f18d.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/4177.69f9f18d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/4319.bf1c86bf.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/4319.bf1c86bf.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/4477.1bd49702.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/4477.1bd49702.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/4500.b6f348d1.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/4500.b6f348d1.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/4666.c4b22a63.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/4666.c4b22a63.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/474.87506447.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/474.87506447.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/5106.44f0ff51.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/5106.44f0ff51.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/5117.04bfe5d3.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/5117.04bfe5d3.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/5249.f2f4070d.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/5249.f2f4070d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/5345.65c91ee7.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/5345.65c91ee7.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/5379.6571574f.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/5379.6571574f.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/5441.5bacdeda.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/5441.1b94928f.chunk.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -1,75 +1,79 @@
 "use strict";
 (self.webpackChunk_streamlit_app = self.webpackChunk_streamlit_app || []).push([
     [5441], {
         5441: (e, t, o) => {
             o.r(t), o.d(t, {
-                default: () => W
+                default: () => P
             });
             var n = o(66845),
                 i = o(25621),
                 s = o(72965),
                 a = o(94206),
                 r = o(60784),
-                l = o(23849),
-                d = o(23593),
-                c = o(63765),
-                h = o(91191);
-            const u = {
+                l = o(62813),
+                d = o.n(l),
+                c = o(50641),
+                h = o(23849),
+                u = o(23593),
+                m = o(63765),
+                g = o(87814),
+                p = o(91191);
+            const f = {
                     DATAFRAME_INDEX: "(index)"
                 },
-                m = new Set([h.GI.DatetimeIndex, h.GI.Float64Index, h.GI.Int64Index, h.GI.RangeIndex, h.GI.UInt64Index]);
+                v = new Set([p.GI.DatetimeIndex, p.GI.Float64Index, p.GI.Int64Index, p.GI.RangeIndex, p.GI.UInt64Index]);
 
-            function g(e) {
+            function b(e) {
                 var t;
                 if (0 === (null === (t = e.datasets) || void 0 === t ? void 0 : t.length)) return null;
                 const o = {};
                 return e.datasets.forEach((e => {
                     if (!e) return;
                     const t = e.hasName ? e.name : null;
                     o[t] = e.data
                 })), o
             }
 
-            function p(e) {
+            function w(e) {
                 let t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 0;
                 if (e.isEmpty()) return [];
                 const o = [],
                     {
                         dataRows: n,
                         dataColumns: i
                     } = e.dimensions,
-                    s = h.fu.getTypeName(e.types.index[0]),
-                    a = m.has(s);
+                    s = p.fu.getTypeName(e.types.index[0]),
+                    a = v.has(s);
                 for (let r = t; r < n; r++) {
                     const t = {};
                     if (a) {
                         const o = e.getIndexValue(r, 0);
-                        t[u.DATAFRAME_INDEX] = "bigint" === typeof o ? Number(o) : o
+                        t[f.DATAFRAME_INDEX] = "bigint" === typeof o ? Number(o) : o
                     }
                     for (let o = 0; o < i; o++) {
                         const n = e.getDataValue(r, o),
                             i = e.types.data[o],
-                            s = h.fu.getTypeName(i);
+                            s = p.fu.getTypeName(i);
                         if ("datetimetz" !== s && (n instanceof Date || Number.isFinite(n)) && (s.startsWith("datetime") || "date" === s)) {
                             const i = 60 * new Date(n).getTimezoneOffset() * 1e3;
                             t[e.columns[0][o]] = n.valueOf() + i
                         } else t[e.columns[0][o]] = "bigint" === typeof n ? Number(n) : n
                     }
                     o.push(t)
                 }
                 return o
             }
-            var f = o(96825),
-                b = o.n(f),
-                w = o(99394),
-                y = o.n(w),
-                x = o(27466);
+            var y = o(96825),
+                x = o.n(y),
+                S = o(99394),
+                F = o.n(S),
+                C = o(27466);
 
-            function v(e, t) {
+            function z(e, t) {
                 const o = {
                     font: t.genericFonts.bodyFont,
                     background: t.colors.bgColor,
                     fieldTitle: "verbal",
                     autosize: {
                         type: "fit",
                         contains: "padding"
@@ -83,64 +87,64 @@
                         fontSize: t.fontSizes.smPx + 2,
                         orient: "top",
                         offset: 26
                     },
                     header: {
                         titleFontWeight: t.fontWeights.normal,
                         titleFontSize: t.fontSizes.mdPx,
-                        titleColor: (0, x.Xy)(t),
+                        titleColor: (0, C.Xy)(t),
                         titleFontStyle: "normal",
                         labelFontSize: t.fontSizes.twoSmPx,
                         labelFontWeight: t.fontWeights.normal,
-                        labelColor: (0, x.Xy)(t),
+                        labelColor: (0, C.Xy)(t),
                         labelFontStyle: "normal"
                     },
                     axis: {
                         labelFontSize: t.fontSizes.twoSmPx,
                         labelFontWeight: t.fontWeights.normal,
-                        labelColor: (0, x.Xy)(t),
+                        labelColor: (0, C.Xy)(t),
                         labelFontStyle: "normal",
                         titleFontWeight: t.fontWeights.normal,
                         titleFontSize: t.fontSizes.smPx,
-                        titleColor: (0, x.Xy)(t),
+                        titleColor: (0, C.Xy)(t),
                         titleFontStyle: "normal",
                         ticks: !1,
-                        gridColor: (0, x.ny)(t),
+                        gridColor: (0, C.ny)(t),
                         domain: !1,
                         domainWidth: 1,
-                        domainColor: (0, x.ny)(t),
+                        domainColor: (0, C.ny)(t),
                         labelFlush: !0,
                         labelFlushOffset: 1,
                         labelBound: !1,
                         labelLimit: 100,
                         titlePadding: t.spacing.lgPx,
                         labelPadding: t.spacing.lgPx,
                         labelSeparation: t.spacing.twoXSPx,
                         labelOverlap: !0
                     },
                     legend: {
                         labelFontSize: t.fontSizes.smPx,
                         labelFontWeight: t.fontWeights.normal,
-                        labelColor: (0, x.Xy)(t),
+                        labelColor: (0, C.Xy)(t),
                         titleFontSize: t.fontSizes.smPx,
                         titleFontWeight: t.fontWeights.normal,
                         titleFontStyle: "normal",
-                        titleColor: (0, x.Xy)(t),
+                        titleColor: (0, C.Xy)(t),
                         titlePadding: 5,
                         labelPadding: t.spacing.lgPx,
                         columnPadding: t.spacing.smPx,
                         rowPadding: t.spacing.twoXSPx,
                         padding: 7,
                         symbolStrokeWidth: 4
                     },
                     range: {
-                        category: (0, x.iY)(t),
-                        diverging: (0, x.ru)(t),
-                        ramp: (0, x.Gy)(t),
-                        heatmap: (0, x.Gy)(t)
+                        category: (0, C.iY)(t),
+                        diverging: (0, C.ru)(t),
+                        ramp: (0, C.Gy)(t),
+                        heatmap: (0, C.Gy)(t)
                     },
                     view: {
                         columns: 1,
                         strokeWidth: 0,
                         stroke: "transparent",
                         continuousHeight: 350,
                         continuousWidth: 400,
@@ -153,15 +157,15 @@
                         columns: 1
                     },
                     facet: {
                         columns: 1
                     },
                     mark: {
                         tooltip: !0,
-                        ...(0, x.Iy)(t) ? {
+                        ...(0, C.Iy)(t) ? {
                             color: "#0068C9"
                         } : {
                             color: "#83C9FF"
                         }
                     },
                     bar: {
                         binSpacing: t.spacing.twoXSPx,
@@ -178,17 +182,17 @@
                     axisTemporal: {
                         grid: !1
                     },
                     axisXBand: {
                         grid: !1
                     }
                 };
-                return e ? y()({}, o, e, ((e, t) => Array.isArray(t) ? t : void 0)) : o
+                return e ? F()({}, o, e, ((e, t) => Array.isArray(t) ? t : void 0)) : o
             }
-            const S = (0, o(1515).Z)("div", {
+            const W = (0, o(1515).Z)("div", {
                 target: "egd2k5h0"
             })((e => {
                 let {
                     theme: t,
                     useContainerWidth: o,
                     isFullScreen: n
                 } = e;
@@ -243,49 +247,49 @@
                                 opacity: "1 !important",
                                 background: t.colors.darkenedBgMix25
                             }
                         }
                     }
                 }
             }), "");
-            var F = o(40864);
-            const z = "source";
-            class C extends n.PureComponent {
+            var V = o(40864);
+            const I = "source";
+            class D extends n.PureComponent {
                 constructor() {
-                    super(...arguments), this.vegaView = void 0, this.vegaFinalizer = void 0, this.defaultDataName = z, this.element = null, this.state = {
+                    super(...arguments), this.vegaView = void 0, this.vegaFinalizer = void 0, this.defaultDataName = I, this.element = null, this.formClearHelper = new g.K, this.state = {
                         error: void 0
                     }, this.finalizeView = () => {
                         this.vegaFinalizer && this.vegaFinalizer(), this.vegaFinalizer = void 0, this.vegaView = void 0
                     }, this.generateSpec = () => {
                         var e, t;
                         const {
                             element: o,
                             theme: n,
                             isFullScreen: i,
                             width: s,
                             height: a
                         } = this.props, r = JSON.parse(o.spec), {
                             useContainerWidth: l
                         } = o;
-                        if ("streamlit" === o.vegaLiteTheme ? r.config = v(r.config, n) : "streamlit" === (null === (e = r.usermeta) || void 0 === e || null === (t = e.embedOptions) || void 0 === t ? void 0 : t.theme) ? (r.config = v(r.config, n), r.usermeta.embedOptions.theme = void 0) : r.config = function(e, t) {
+                        if ("streamlit" === o.vegaLiteTheme ? r.config = z(r.config, n) : "streamlit" === (null === (e = r.usermeta) || void 0 === e || null === (t = e.embedOptions) || void 0 === t ? void 0 : t.theme) ? (r.config = z(r.config, n), r.usermeta.embedOptions.theme = void 0) : r.config = function(e, t) {
                                 const {
                                     colors: o,
                                     fontSizes: n,
                                     genericFonts: i
                                 } = t, s = {
                                     labelFont: i.bodyFont,
                                     titleFont: i.bodyFont,
                                     labelFontSize: n.twoSmPx,
                                     titleFontSize: n.twoSmPx
                                 }, a = {
                                     background: o.bgColor,
                                     axis: {
                                         labelColor: o.bodyText,
                                         titleColor: o.bodyText,
-                                        gridColor: (0, x.ny)(t),
+                                        gridColor: (0, C.ny)(t),
                                         ...s
                                     },
                                     legend: {
                                         labelColor: o.bodyText,
                                         titleColor: o.bodyText,
                                         ...s
                                     },
@@ -296,40 +300,97 @@
                                     },
                                     header: {
                                         labelColor: o.bodyText,
                                         titleColor: o.bodyText,
                                         ...s
                                     },
                                     view: {
-                                        stroke: (0, x.ny)(t),
+                                        stroke: (0, C.ny)(t),
                                         continuousHeight: 350,
                                         continuousWidth: 400,
                                         discreteHeight: 350,
                                         discreteWidth: {
                                             step: 20
                                         }
                                     },
                                     mark: {
                                         tooltip: !0
                                     }
                                 };
-                                return e ? b()({}, a, e) : a
+                                return e ? x()({}, a, e) : a
                             }(r.config, n), i ? (r.width = s, r.height = a, "vconcat" in r && r.vconcat.forEach((e => {
                                 e.width = s
                             }))) : l && (r.width = s, "vconcat" in r && r.vconcat.forEach((e => {
                                 e.width = s
                             }))), r.padding || (r.padding = {}), null == r.padding.bottom && (r.padding.bottom = 20), r.datasets) throw new Error("Datasets should not be passed as part of the spec");
-                        return r
+                        return o.selectionMode.length > 0 && function(e) {
+                            "params" in e && "encoding" in e && e.params.forEach((t => {
+                                "select" in t && (["interval", "point"].includes(t.select) && (t.select = {
+                                    type: t.select
+                                }), "type" in t.select && "point" === t.select.type && !("encodings" in t.select) && (0, c.le)(t.select.encodings) && (t.select.encodings = Object.keys(e.encoding)))
+                            }))
+                        }(r), r
+                    }, this.maybeConfigureSelections = () => {
+                        if (void 0 === this.vegaView) return;
+                        const {
+                            widgetMgr: e,
+                            element: t
+                        } = this.props;
+                        if (null === t || void 0 === t || !t.id || 0 === t.selectionMode.length) return;
+                        const o = e.getElementState(this.props.element.id, "viewState");
+                        if ((0, c.bb)(o)) try {
+                            this.vegaView = this.vegaView.setState(o)
+                        } catch (i) {
+                            (0, h.KE)("Failed to restore view state", i)
+                        }
+                        t.selectionMode.forEach(((o, n) => {
+                            var i;
+                            null === (i = this.vegaView) || void 0 === i || i.addSignalListener(o, (0, c.Ds)(150, ((o, n) => {
+                                var i;
+                                const s = null === (i = this.vegaView) || void 0 === i ? void 0 : i.getState({
+                                    data: (e, o) => t.selectionMode.some((t => "".concat(t, "_store") === e)),
+                                    recurse: !1
+                                });
+                                (0, c.bb)(s) && e.setElementState(t.id, "viewState", s);
+                                let a = n;
+                                "vlPoint" in n && "or" in n.vlPoint && (a = n.vlPoint.or);
+                                const r = JSON.parse(e.getStringValue(t) || "{}"),
+                                    l = {
+                                        selection: {
+                                            ...(null === r || void 0 === r ? void 0 : r.selection) || {},
+                                            [o]: a || {}
+                                        }
+                                    };
+                                d()(r, l) || e.setStringValue(t, JSON.stringify(l), {
+                                    fromUi: !0
+                                }, this.props.fragmentId)
+                            })))
+                        }));
+                        const n = () => {
+                            const o = {
+                                selection: {}
+                            };
+                            this.props.element.selectionMode.forEach((e => {
+                                o.selection[e] = {}
+                            }));
+                            const n = e.getStringValue(t),
+                                i = n ? JSON.parse(n) : o;
+                            var s;
+                            d()(i, o) || (null === (s = this.props.widgetMgr) || void 0 === s || s.setStringValue(this.props.element, JSON.stringify(o), {
+                                fromUi: !0
+                            }, this.props.fragmentId))
+                        };
+                        this.props.element.formId && this.formClearHelper.manageFormClearListener(this.props.widgetMgr, this.props.element.formId, n)
                     }
                 }
                 async componentDidMount() {
                     try {
                         await this.createView()
                     } catch (e) {
-                        const t = (0, c.b)(e);
+                        const t = (0, m.b)(e);
                         this.setState({
                             error: t
                         })
                     }
                 }
                 componentWillUnmount() {
                     this.finalizeView()
@@ -340,124 +401,121 @@
                         theme: o
                     } = e, {
                         element: n,
                         theme: i
                     } = this.props, s = t.spec, {
                         spec: a
                     } = n;
-                    if (!this.vegaView || s !== a || o !== i || e.width !== this.props.width || e.height !== this.props.height || e.element.vegaLiteTheme !== this.props.element.vegaLiteTheme) {
-                        (0, l.ji)("Vega spec changed.");
+                    if (!this.vegaView || s !== a || o !== i || e.width !== this.props.width || e.height !== this.props.height || e.element.vegaLiteTheme !== this.props.element.vegaLiteTheme || !d()(e.element.selectionMode, this.props.element.selectionMode)) {
+                        (0, h.ji)("Vega spec changed.");
                         try {
                             await this.createView()
-                        } catch (m) {
-                            const e = (0, c.b)(m);
+                        } catch (g) {
+                            const e = (0, m.b)(g);
                             this.setState({
                                 error: e
                             })
                         }
                         return
                     }
                     const r = t.data,
                         {
-                            data: d
+                            data: l
                         } = n;
-                    (r || d) && this.updateData(this.defaultDataName, r, d);
-                    const h = g(t) || {},
-                        u = g(n) || {};
-                    for (const [l, c] of Object.entries(u)) {
-                        const e = l || this.defaultDataName,
-                            t = h[e];
-                        this.updateData(e, t, c)
+                    (r || l) && this.updateData(this.defaultDataName, r, l);
+                    const c = b(t) || {},
+                        u = b(n) || {};
+                    for (const [d, h] of Object.entries(u)) {
+                        const e = d || this.defaultDataName,
+                            t = c[e];
+                        this.updateData(e, t, h)
                     }
-                    for (const l of Object.keys(h)) u.hasOwnProperty(l) || l === this.defaultDataName || this.updateData(l, null, null);
+                    for (const d of Object.keys(c)) u.hasOwnProperty(d) || d === this.defaultDataName || this.updateData(d, null, null);
                     this.vegaView.resize().runAsync()
                 }
                 updateData(e, t, o) {
                     if (!this.vegaView) throw new Error("Chart has not been drawn yet");
-                    if (!o || 0 === o.data.numRows) {
-                        return void(this.vegaView._runtime.data.hasOwnProperty(e) && this.vegaView.remove(e, a.truthy))
+                    if (!o || 0 === o.data.numRows) try {
+                        this.vegaView.remove(e, a.truthy)
+                    } finally {
+                        return
                     }
-                    if (!t || 0 === t.data.numRows) return void this.vegaView.insert(e, p(o));
+                    if (!t || 0 === t.data.numRows) return void this.vegaView.insert(e, w(o));
                     const {
                         dataRows: n,
                         dataColumns: i
                     } = t.dimensions, {
                         dataRows: s,
                         dataColumns: r
                     } = o.dimensions;
-                    if (function(e, t, o, n, i, s) {
-                            if (o !== s) return !1;
-                            if (t >= i) return !1;
-                            if (0 === t) return !1;
-                            const a = s - 1,
-                                r = t - 1;
-                            return e.getDataValue(0, a) === n.getDataValue(0, a) && e.getDataValue(r, a) === n.getDataValue(r, a)
-                        }(t, n, i, o, s, r)) n < s && this.vegaView.insert(e, p(o, n));
-                    else {
-                        const t = a.changeset().remove(a.truthy).insert(p(o));
-                        this.vegaView.change(e, t), (0, l.ji)("Had to clear the ".concat(e, " dataset before inserting data through Vega view."))
-                    }
+                    ! function(e, t, o, n, i, s) {
+                        if (o !== s) return !1;
+                        if (t >= i) return !1;
+                        if (0 === t) return !1;
+                        const a = s - 1,
+                            r = t - 1;
+                        return e.getDataValue(0, a) === n.getDataValue(0, a) && e.getDataValue(r, a) === n.getDataValue(r, a)
+                    }(t, n, i, o, s, r) ? (this.vegaView.data(e, w(o)), (0, h.ji)("Had to clear the ".concat(e, " dataset before inserting data through Vega view."))) : n < s && this.vegaView.insert(e, w(o, n))
                 }
                 async createView() {
-                    if ((0, l.ji)("Creating a new Vega view."), !this.element) throw Error("Element missing.");
+                    if ((0, h.ji)("Creating a new Vega view."), !this.element) throw Error("Element missing.");
                     this.finalizeView();
-                    const e = this.props.element,
-                        t = this.generateSpec(),
-                        o = {
-                            ast: !0,
-                            expr: r.N,
-                            tooltip: {
-                                disableDefaultStyle: !0
-                            },
-                            defaultStyle: !1,
-                            forceActionsMenu: !0
+                    const {
+                        element: e
+                    } = this.props, t = this.generateSpec(), o = {
+                        ast: !0,
+                        expr: r.N,
+                        tooltip: {
+                            disableDefaultStyle: !0
                         },
-                        {
-                            vgSpec: n,
-                            view: i,
-                            finalize: a
-                        } = await (0, s.ZP)(this.element, t, o);
-                    this.vegaView = i, this.vegaFinalizer = a;
-                    const d = function(e) {
-                            const t = g(e);
+                        defaultStyle: !1,
+                        forceActionsMenu: !0
+                    }, {
+                        vgSpec: n,
+                        view: i,
+                        finalize: a
+                    } = await (0, s.ZP)(this.element, t, o);
+                    this.vegaView = i, this.maybeConfigureSelections(), this.vegaFinalizer = a;
+                    const l = function(e) {
+                            const t = b(e);
                             if (null == t) return null;
                             const o = {};
-                            for (const [n, i] of Object.entries(t)) o[n] = p(i);
+                            for (const [n, i] of Object.entries(t)) o[n] = w(i);
                             return o
                         }(e),
-                        c = d ? Object.keys(d) : [];
-                    if (1 === c.length) {
-                        const [e] = c;
+                        d = l ? Object.keys(l) : [];
+                    if (1 === d.length) {
+                        const [e] = d;
                         this.defaultDataName = e
-                    } else 0 === c.length && n.data && (this.defaultDataName = z);
-                    const h = function(e) {
+                    } else 0 === d.length && n.data && (this.defaultDataName = I);
+                    const c = function(e) {
                         const t = e.data;
-                        return t && 0 !== t.data.numRows ? p(t) : null
+                        return t && 0 !== t.data.numRows ? w(t) : null
                     }(e);
-                    if (h && i.insert(this.defaultDataName, h), d)
-                        for (const [s, r] of Object.entries(d)) i.insert(s, r);
+                    if (c && i.insert(this.defaultDataName, c), l)
+                        for (const [s, r] of Object.entries(l)) i.insert(s, r);
                     await i.runAsync(), this.vegaView.resize().runAsync()
                 }
                 render() {
                     if (this.state.error) throw this.state.error;
-                    return (0, F.jsx)(S, {
+                    return (0, V.jsx)(W, {
                         "data-testid": "stArrowVegaLiteChart",
                         useContainerWidth: this.props.element.useContainerWidth,
                         isFullScreen: this.props.isFullScreen,
                         ref: e => {
                             this.element = e
                         }
                     })
                 }
             }
-            const W = (0, i.b)((0, d.Z)(C))
+            const P = (0, i.b)((0, u.Z)(D))
         },
         23593: (e, t, o) => {
             o.d(t, {
-                Z: () => b
+                Z: () => v
             });
             var n = o(66845),
                 i = o(13005),
                 s = o.n(i),
                 a = o(25621),
                 r = o(82218),
                 l = o(97781),
@@ -614,15 +672,15 @@
                             collapse: this.zoomOut
                         })]
                     })
                 }
             }
             p.contextType = c.E;
             const f = (0, a.b)(p);
-            const b = function(e) {
+            const v = function(e) {
                 let t = arguments.length > 1 && void 0 !== arguments[1] && arguments[1];
                 class o extends n.PureComponent {
                     constructor() {
                         super(...arguments), this.render = () => {
                             const {
                                 width: o,
                                 height: n,
@@ -651,10 +709,28 @@
                                 }
                             })
                         }
                     }
                 }
                 return o.displayName = "withFullScreenWrapper(".concat(e.displayName || e.name, ")"), s()(o, e)
             }
+        },
+        87814: (e, t, o) => {
+            o.d(t, {
+                K: () => i
+            });
+            var n = o(50641);
+            class i {
+                constructor() {
+                    this.formClearListener = void 0, this.lastWidgetMgr = void 0, this.lastFormId = void 0
+                }
+                manageFormClearListener(e, t, o) {
+                    null != this.formClearListener && this.lastWidgetMgr === e && this.lastFormId === t || (this.disconnect(), (0, n.bM)(t) && (this.formClearListener = e.addFormClearedListener(t, o), this.lastWidgetMgr = e, this.lastFormId = t))
+                }
+                disconnect() {
+                    var e;
+                    null === (e = this.formClearListener) || void 0 === e || e.disconnect(), this.formClearListener = void 0, this.lastWidgetMgr = void 0, this.lastFormId = void 0
+                }
+            }
         }
     }
 ]);
```

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/5791.9a42fb4b.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/5791.9a42fb4b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/6013.4ba2d616.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/6013.4ba2d616.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/6405.ac5a6f23.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/6405.ac5a6f23.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/6718.802da17e.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/6718.802da17e.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/6853.93dd1c4c.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/6853.93dd1c4c.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/6950.70fe55c2.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/6950.70fe55c2.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/7142.83028745.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/7142.83028745.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/7175.be4076bc.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/7175.be4076bc.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/7323.b74cc85b.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/7323.b74cc85b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/7323.b74cc85b.chunk.js.LICENSE.txt` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/7323.b74cc85b.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/7483.64f23be7.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/7483.64f23be7.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/7602.e8abc06b.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/7602.e8abc06b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/7805.acc6316a.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/7805.acc6316a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/8005.43974a35.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/8005.43974a35.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/8148.cc5b50d8.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/8148.a5f74d47.chunk.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -226,18 +226,18 @@
                 f = n(25621),
                 b = n(34367),
                 v = n(31011),
                 y = n(63730),
                 w = n(68411),
                 x = n(9003),
                 C = n(81354),
-                M = n(46927),
-                S = n(1515),
-                E = n(27466);
-            const T = (0, S.Z)("div", {
+                E = n(46927),
+                M = n(1515),
+                S = n(27466);
+            const T = (0, M.Z)("div", {
                     target: "e2wxzia1"
                 })((e => {
                     let {
                         theme: t,
                         locked: n,
                         target: i
                     } = e;
@@ -260,22 +260,22 @@
                                     opacity: 1,
                                     top: "-2.4rem"
                                 }
                             }
                         }
                     }
                 }), ""),
-                k = (0, S.Z)("div", {
+                k = (0, M.Z)("div", {
                     target: "e2wxzia0"
                 })((e => {
                     let {
                         theme: t
                     } = e;
                     return {
-                        color: (0, E.Iy)(t) ? t.colors.fadedText60 : t.colors.bodyText,
+                        color: (0, S.Iy)(t) ? t.colors.fadedText60 : t.colors.bodyText,
                         display: "flex",
                         flexDirection: "row",
                         alignItems: "center",
                         justifyContent: "flex-end",
                         boxShadow: "1px 2px 8px rgba(0, 0, 0, 0.08)",
                         borderRadius: t.radii.lg,
                         backgroundColor: t.colors.lightenedBg05,
@@ -308,15 +308,15 @@
                         onMouseEnterDelay: 1e3,
                         inline: !0,
                         children: (0, R.jsxs)(x.ZP, {
                             onClick: e => {
                                 o && o(), e.stopPropagation()
                             },
                             kind: C.nW.ELEMENT_TOOLBAR,
-                            children: [i && (0, R.jsx)(M.Z, {
+                            children: [i && (0, R.jsx)(E.Z, {
                                 content: i,
                                 size: "md",
                                 testid: "stElementToolbarButtonIcon"
                             }), r && (0, R.jsx)("span", {
                                 children: r
                             })]
                         })
@@ -869,15 +869,15 @@
                         return (0, g.le)(null === (n = e.data) || void 0 === n ? void 0 : n.value) || "" === (null === (i = e.data) || void 0 === i ? void 0 : i.value) ? null : "number" === t ? null !== (l = $(null === (r = e.data) || void 0 === r ? void 0 : r.value)) && void 0 !== l ? l : null : "boolean" === t ? null !== (a = Q(null === (s = e.data) || void 0 === s ? void 0 : s.value)) && void 0 !== a ? a : null : null === (o = e.data) || void 0 === o ? void 0 : o.value
                     }
                 }
             }
             xe.isEditableType = !0;
             const Ce = xe;
 
-            function Me(e) {
+            function Ee(e) {
                 const t = {
                     kind: o.p6.Bubble,
                     data: [],
                     allowOverlay: !0,
                     contentAlign: e.contentAlignment,
                     style: e.isIndex ? "faded" : "normal"
                 };
@@ -894,18 +894,18 @@
                             isMissingValue: (0, g.le)(e),
                             copyData: (0, g.le)(e) ? "" : X(n.map((e => "string" === typeof e && e.includes(",") ? e.replace(/,/g, " ") : e)))
                         }
                     },
                     getCellValue: e => (0, g.le)(e.data) || Y(e) ? null : e.data
                 }
             }
-            Me.isEditableType = !1;
-            const Se = Me;
+            Ee.isEditableType = !1;
+            const Me = Ee;
 
-            function Ee(e, t, n) {
+            function Se(e, t, n) {
                 const i = new RegExp("".concat(e, "[,\\s].*{(?:[^}]*[\\s;]{1})?").concat(t, ":\\s*([^;}]+)[;]?.*}"), "gm");
                 n = n.replace(/{/g, " {");
                 const o = i.exec(n);
                 if (o) return o[1].trim()
             }
 
             function Te(e, t) {
@@ -978,17 +978,17 @@
                                 ...l.data,
                                 displayDate: e
                             }
                         })
                     }
                     n && t.cssId && (l = function(e, t, n) {
                         const i = {},
-                            o = Ee(t, "color", n);
+                            o = Se(t, "color", n);
                         o && (i.textDark = o);
-                        const l = Ee(t, "background-color", n);
+                        const l = Se(t, "background-color", n);
                         return l && (i.bgCell = l), "yellow" === l && void 0 === o && (i.textDark = "#31333F"), i ? {
                             ...e,
                             themeOverride: i
                         } : e
                     }(l, t.cssId, n))
                 }
                 return l
@@ -1234,15 +1234,15 @@
             }
             ze.isEditableType = !1, Ve.isEditableType = !1, He.isEditableType = !1;
             const Le = new Map(Object.entries({
                     object: se,
                     text: ce,
                     checkbox: be,
                     selectbox: Ce,
-                    list: Se,
+                    list: Me,
                     number: we,
                     link: Ie,
                     datetime: he,
                     date: ge,
                     time: pe,
                     line_chart: ze,
                     bar_chart: Ve,
@@ -1283,15 +1283,15 @@
 
             function Ue(e) {
                 var t;
                 const n = null === (t = e.columnTypeOptions) || void 0 === t ? void 0 : t.type;
                 let i;
                 return (0, g.bb)(n) && (Le.has(n) ? i = Le.get(n) : (0, re.KE)("Unknown column type configured in column configuration: ".concat(n))), (0, g.le)(i) && (i = function(e) {
                     let t = e ? W.fu.getTypeName(e) : null;
-                    return t ? (t = t.toLowerCase().trim(), ["unicode", "empty"].includes(t) ? ce : ["datetime", "datetimetz"].includes(t) ? he : "time" === t ? pe : "date" === t ? ge : ["object", "bytes"].includes(t) ? se : ["bool"].includes(t) ? be : ["int8", "int16", "int32", "int64", "uint8", "uint16", "uint32", "uint64", "float16", "float32", "float64", "float96", "float128", "range", "decimal"].includes(t) ? we : "categorical" === t ? Ce : t.startsWith("list") ? Se : se) : se
+                    return t ? (t = t.toLowerCase().trim(), ["unicode", "empty"].includes(t) ? ce : ["datetime", "datetimetz"].includes(t) ? he : "time" === t ? pe : "date" === t ? ge : ["object", "bytes"].includes(t) ? se : ["bool"].includes(t) ? be : ["int8", "int16", "int32", "int64", "uint8", "uint16", "uint32", "uint64", "float16", "float32", "float64", "float96", "float128", "range", "decimal"].includes(t) ? we : "categorical" === t ? Ce : t.startsWith("list") ? Me : se) : se
                 }(e.arrowType)), i
             }
             const qe = function(e, t, n) {
                 const o = (0, f.u)(),
                     l = i.useMemo((() => function(e) {
                         if (!e) return new Map;
                         try {
@@ -1425,23 +1425,25 @@
                             if (l) {
                                 const e = l.getCell(n);
                                 var r;
                                 if (e) this.editedCells.has(t) || this.editedCells.set(t, new Map), null === (r = this.editedCells.get(t)) || void 0 === r || r.set(l.indexNumber, e)
                             }
                         }))
                     })), n.added_rows.forEach((e => {
-                        const t = new Map;
-                        Object.keys(e).forEach((n => {
-                            const i = e[n],
-                                l = o.get(n);
+                        const n = new Map;
+                        t.forEach((e => {
+                            n.set(e.indexNumber, e.getCell(null))
+                        })), Object.keys(e).forEach((t => {
+                            const i = e[t],
+                                l = o.get(t);
                             if (l) {
                                 const e = l.getCell(i);
-                                e && t.set(l.indexNumber, e)
+                                e && n.set(l.indexNumber, e)
                             }
-                        })), this.addedRows.push(t)
+                        })), this.addedRows.push(n)
                     })), this.deletedRows = n.deleted_rows
                 }
                 isAddedRow(e) {
                     return e >= this.numRows
                 }
                 getCell(e, t) {
                     if (this.isAddedRow(t)) return this.addedRows[t - this.numRows].get(e);
@@ -1525,23 +1527,25 @@
                 return {
                     getCellContent: i.useCallback((i => {
                         let [l, r] = i;
                         if (l > t.length - 1) return P("Column index out of bounds.", "This should never happen. Please report this bug.");
                         if (r > n - 1) return P("Row index out of bounds.", "This should never happen. Please report this bug.");
                         const a = t[l],
                             s = a.indexNumber,
-                            d = o.current.getOriginalRowIndex(r);
-                        if (a.isEditable || o.current.isAddedRow(d)) {
+                            d = o.current.getOriginalRowIndex(r),
+                            c = o.current.isAddedRow(d);
+                        if (a.isEditable || c) {
                             const e = o.current.getCell(s, d);
-                            if (void 0 !== e) return e
+                            if ((0, g.bb)(e)) return e;
+                            if (c) return P("Error during cell creation.", "This should never happen. Please report this bug. " + "No cell found for an added row: col=".concat(s, "; row=").concat(d))
                         }
                         try {
                             return Re(a, e.getCell(d + 1, s), e.cssStyles)
-                        } catch (c) {
-                            return P("Error during cell creation.", "This should never happen. Please report this bug. \nError: ".concat(c))
+                        } catch (u) {
+                            return P("Error during cell creation.", "This should never happen. Please report this bug. \nError: ".concat(u))
                         }
                     }), [t, n, e, o])
                 }
             };
             var $e = n(32700);
             const et = function(e, t, n) {
                 const [o, l] = i.useState(), {
@@ -1858,21 +1862,21 @@
                         } : e))), [e, t]),
                         onColumnResize: o
                     }
                 },
                 wt = 2,
                 xt = 35,
                 Ct = 50 + wt,
-                Mt = 2 * xt + wt;
-            const St = function(e, t, n, o, l) {
+                Et = 2 * xt + wt;
+            const Mt = function(e, t, n, o, l) {
                     let r, a = function(e) {
-                            return Math.max(e * xt + wt, Mt)
+                            return Math.max(e * xt + wt, Et)
                         }(t + 1 + (e.editingMode === p.Eh.EditingMode.DYNAMIC ? 1 : 0)),
                         s = Math.min(a, 400);
-                    e.height && (s = Math.max(e.height, Mt), a = Math.max(e.height, a)), o && (s = Math.min(s, o), a = Math.min(a, o), e.height || (s = a));
+                    e.height && (s = Math.max(e.height, Et), a = Math.max(e.height, a)), o && (s = Math.min(s, o), a = Math.min(a, o), e.height || (s = a));
                     let d = n;
                     e.useContainerWidth ? r = n : e.width && (r = Math.min(Math.max(e.width, Ct), n), d = Math.min(Math.max(e.width, d), n));
                     const [c, u] = i.useState({
                         width: r || "100%",
                         height: s
                     });
                     return i.useLayoutEffect((() => {
@@ -1903,23 +1907,23 @@
                                 height: a
                             })
                         } else u({
                             width: r || "100%",
                             height: s
                         })
                     }), [l]), {
-                        minHeight: Mt,
+                        minHeight: Et,
                         maxHeight: a,
                         minWidth: Ct,
                         maxWidth: d,
                         resizableSize: c,
                         setResizableSize: u
                     }
                 },
-                Et = (0, S.Z)("img", {
+                St = (0, M.Z)("img", {
                     target: "e24uaba0"
                 })((() => ({
                     maxWidth: "100%",
                     maxHeight: "600px",
                     objectFit: "scale-down"
                 })), ""),
                 Tt = e => {
@@ -1927,18 +1931,18 @@
                         urls: t
                     } = e;
                     const n = t && t.length > 0 ? t[0] : "";
                     return n.startsWith("http") ? (0, R.jsx)("a", {
                         href: n,
                         target: "_blank",
                         rel: "noreferrer noopener",
-                        children: (0, R.jsx)(Et, {
+                        children: (0, R.jsx)(St, {
                             src: n
                         })
-                    }) : (0, R.jsx)(Et, {
+                    }) : (0, R.jsx)(St, {
                         src: n
                     })
                 };
             var kt = n(31572),
                 Rt = n(13553),
                 Nt = n(80152);
             const It = function(e) {
@@ -1984,15 +1988,15 @@
                                     paddingLeft: "0 !important",
                                     paddingRight: "0 !important",
                                     backgroundColor: "transparent"
                                 }
                             },
                             Inner: {
                                 style: {
-                                    backgroundColor: (0, E.Iy)(s) ? d.bgColor : d.secondaryBg,
+                                    backgroundColor: (0, S.Iy)(s) ? d.bgColor : d.secondaryBg,
                                     color: d.bodyText,
                                     fontSize: c.sm,
                                     fontWeight: "normal",
                                     paddingTop: "0 !important",
                                     paddingBottom: "0 !important",
                                     paddingLeft: "0 !important",
                                     paddingRight: "0 !important"
@@ -2007,15 +2011,15 @@
                                 position: "fixed",
                                 top: t,
                                 left: n
                             }
                         })
                     })
                 },
-                _t = (0, S.Z)("div", {
+                _t = (0, M.Z)("div", {
                     target: "e1w7nams0"
                 })((e => {
                     let {
                         hasCustomizedScrollbars: t,
                         theme: n
                     } = e;
                     return {
@@ -2044,18 +2048,18 @@
                     height: f,
                     disabled: b,
                     widgetMgr: v,
                     isFullScreen: y,
                     disableFullscreenMode: w,
                     expand: x,
                     collapse: C,
-                    fragmentId: M
+                    fragmentId: E
                 } = e;
-                const S = i.useRef(null),
-                    E = i.useRef(null),
+                const M = i.useRef(null),
+                    S = i.useRef(null),
                     T = i.useRef(null),
                     {
                         theme: k,
                         headerIcons: _,
                         tableBorderRadius: O
                     } = Xe(),
                     [D, F] = i.useState(!0),
@@ -2091,32 +2095,32 @@
                 } = Qe(n, te, Q, X), {
                     columns: ie,
                     sortColumn: oe,
                     getOriginalIndex: le,
                     getCellContent: re
                 } = et(U, te, ne), ae = i.useCallback((0, g.Ds)(150, (e => {
                     const n = {
-                        select: {
+                        selection: {
                             rows: [],
                             columns: []
                         }
                     };
-                    n.select.rows = e.rows.toArray().map((e => le(e))), n.select.columns = e.columns.toArray().map((e => Je(te[e])));
+                    n.selection.rows = e.rows.toArray().map((e => le(e))), n.selection.columns = e.columns.toArray().map((e => Je(te[e])));
                     const i = JSON.stringify(n),
                         o = v.getStringValue({
                             id: t.id,
                             formId: t.formId
                         });
                     void 0 !== o && o === i || v.setStringValue({
                         id: t.id,
                         formId: t.formId
                     }, i, {
                         fromUi: !0
-                    }, M)
-                })), [t.id, t.formId, v, M]), {
+                    }, E)
+                })), [t.id, t.formId, v, E]), {
                     gridSelection: se,
                     isRowSelectionActivated: de,
                     isMultiRowSelectionActivated: ce,
                     isColumnSelectionActivated: ue,
                     isMultiColumnSelectionActivated: me,
                     isRowSelected: he,
                     isColumnSelected: pe,
@@ -2125,31 +2129,31 @@
                     processSelectionChange: be
                 } = it(t, K, b, ae);
                 i.useEffect((() => {
                     fe(!0, !0)
                 }), [y]);
                 const ve = i.useCallback((e => {
                     var t;
-                    null === (t = E.current) || void 0 === t || t.updateCells(e)
+                    null === (t = S.current) || void 0 === t || t.updateCells(e)
                 }), []);
                 i.useEffect((() => {
                     if (!de && !ue) return;
                     const e = v.getStringValue({
                         id: t.id,
                         formId: t.formId
                     });
                     if (e) {
                         var n, i, l, r;
                         const t = ie.map((e => Je(e))),
                             a = JSON.parse(e);
                         let s = o.EV.empty(),
                             d = o.EV.empty();
-                        if (null === (n = a.select) || void 0 === n || null === (i = n.rows) || void 0 === i || i.forEach((e => {
+                        if (null === (n = a.selection) || void 0 === n || null === (i = n.rows) || void 0 === i || i.forEach((e => {
                                 s = s.add(e)
-                            })), null === (l = a.select) || void 0 === l || null === (r = l.columns) || void 0 === r || r.forEach((e => {
+                            })), null === (l = a.selection) || void 0 === l || null === (r = l.columns) || void 0 === r || r.forEach((e => {
                                 d = d.add(t.indexOf(e))
                             })), s.length > 0 || d.length > 0) {
                             be({
                                 rows: s,
                                 columns: d,
                                 current: void 0
                             })
@@ -2166,24 +2170,24 @@
                             formId: t.formId
                         });
                         void 0 === n && (n = new Ke(0).toJson([])), e !== n && v.setStringValue({
                             id: t.id,
                             formId: t.formId
                         }, e, {
                             fromUi: !0
-                        }, M)
-                    })), [t.id, t.formId, v, M, ie, X.current]),
+                        }, E)
+                    })), [t.id, t.formId, v, E, ie, X.current]),
                     {
                         exportToCsv: xe
                     } = ct(re, ie, Q),
                     {
                         onCellEdited: Ce,
-                        onPaste: Me,
-                        onRowAppended: Se,
-                        onDelete: Ee,
+                        onPaste: Ee,
+                        onRowAppended: Me,
+                        onDelete: Se,
                         validateCell: Te
                     } = ut(ie, t.editingMode !== Z, X, re, le, ve, ye, we, fe),
                     {
                         tooltip: ke,
                         clearTooltip: Re,
                         onItemHovered: Ne
                     } = mt(ie, re),
@@ -2199,15 +2203,15 @@
                     {
                         minHeight: Ae,
                         maxHeight: ze,
                         minWidth: Ve,
                         maxWidth: He,
                         resizableSize: Le,
                         setResizableSize: We
-                    } = St(t, Q, h, f, y),
+                    } = Mt(t, Q, h, f, y),
                     je = i.useCallback((e => {
                         let [t, n] = e;
                         return {
                             ...q(!0, !1),
                             displayData: "empty",
                             contentAlign: "center",
                             allowOverlay: !1,
@@ -2226,15 +2230,15 @@
                         e.disconnect()
                     }
                 }), [t.formId, ee, fe, v]);
                 const Be = !K && t.editingMode === Z && !b,
                     Pe = K ? 0 : ie.filter((e => e.isIndex)).length;
                 return i.useEffect((() => {
                     setTimeout((() => {
-                        if (T.current && E.current) {
+                        if (T.current && S.current) {
                             var e, t;
                             const n = null === (e = T.current) || void 0 === e || null === (t = e.querySelector(".dvn-stack")) || void 0 === t ? void 0 : t.getBoundingClientRect();
                             n && (H(n.height > T.current.clientHeight), W(n.width > T.current.clientWidth))
                         }
                     }), 1)
                 }), [Le, Q, De]), (0, R.jsxs)(_t, {
                     "data-testid": "stDataFrame",
@@ -2263,36 +2267,36 @@
                             onClick: () => {
                                 fe(), Re()
                             }
                         }), Be && he && (0, R.jsx)(N, {
                             label: "Delete row(s)",
                             icon: s.H,
                             onClick: () => {
-                                Ee && (Ee(se), Re())
+                                Se && (Se(se), Re())
                             }
                         }), Be && !he && (0, R.jsx)(N, {
                             label: "Add row",
                             icon: d.m,
                             onClick: () => {
-                                Se && (F(!0), Se(), Re())
+                                Me && (F(!0), Me(), Re())
                             }
                         }), !G && !K && (0, R.jsx)(N, {
                             label: "Download as CSV",
                             icon: c.k,
                             onClick: () => xe()
                         }), !K && (0, R.jsx)(N, {
                             label: "Search",
                             icon: u.o,
                             onClick: () => {
                                 A ? z(!1) : (F(!0), z(!0)), Re()
                             }
                         })]
                     }), (0, R.jsx)(r.e, {
                         "data-testid": "stDataFrameResizable",
-                        ref: S,
+                        ref: M,
                         defaultSize: Le,
                         style: {
                             border: "1px solid ".concat(k.borderColor),
                             borderRadius: "".concat(O)
                         },
                         minHeight: Ae,
                         maxHeight: ze,
@@ -2308,22 +2312,22 @@
                             bottomRight: !0,
                             bottomLeft: !1,
                             topLeft: !1
                         },
                         grid: [1, xt],
                         snapGap: xt / 3,
                         onResizeStop: (e, t, n, i) => {
-                            S.current && We({
-                                width: S.current.size.width,
-                                height: ze - S.current.size.height === wt ? S.current.size.height + wt : S.current.size.height
+                            M.current && We({
+                                width: M.current.size.width,
+                                height: ze - M.current.size.height === wt ? M.current.size.height + wt : M.current.size.height
                             })
                         },
                         children: (0, R.jsx)(l.F, {
                             className: "glideDataEditor",
-                            ref: E,
+                            ref: S,
                             columns: De,
                             rows: K ? 1 : Q,
                             minColumnWidth: 50,
                             maxColumnWidth: 1e3,
                             maxColumnAutoWidth: 500,
                             rowHeight: xt,
                             headerHeight: xt,
@@ -2394,16 +2398,16 @@
                                 columnSelect: b ? "none" : me ? "multi" : "single",
                                 columnSelectionBlending: "mixed",
                                 rangeSelectionBlending: "exclusive"
                             },
                             ...!K && t.editingMode !== P && !b && {
                                 fillHandle: !j,
                                 onCellEdited: Ce,
-                                onPaste: Me,
-                                onDelete: Ee
+                                onPaste: Ee,
+                                onDelete: Se
                             },
                             ...!K && t.editingMode === Z && {
                                 trailingRowOptions: {
                                     sticky: !1,
                                     tint: !0
                                 },
                                 rowMarkers: {
@@ -2412,15 +2416,15 @@
                                     theme: {
                                         bgCell: k.bgHeader,
                                         bgCellMedium: k.bgHeader
                                     }
                                 },
                                 rowSelectionMode: "multi",
                                 rowSelect: b ? "none" : "multi",
-                                onRowAppended: b ? void 0 : Se,
+                                onRowAppended: b ? void 0 : Me,
                                 onHeaderClicked: void 0
                             }
                         })
                     }), ke && ke.content && (0, R.jsx)(It, {
                         top: ke.top,
                         left: ke.left,
                         content: ke.content,
```

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/8427.bd0a7cf3.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/8427.bd0a7cf3.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/8477.de889fe5.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/8477.de889fe5.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/8492.0d93bd08.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/8492.0d93bd08.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/8536.f8de3d9a.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/8536.f8de3d9a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/8570.6de19120.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/8570.6de19120.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/8691.9ccf7f89.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/8691.9ccf7f89.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/9330.2b4c99e0.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/9330.2b4c99e0.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/9336.2d95d840.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/9336.2d95d840.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/937.a1248039.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/937.a1248039.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/9656.8c935274.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/9656.8c935274.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/9758.6e6d8662.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/9758.6e6d8662.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/9865.fd93213d.chunk.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/9865.fd93213d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/main.45247b52.js` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/main.32c71338.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.45247b52.js.LICENSE.txt */
+/*! For license information please see main.32c71338.js.LICENSE.txt */
 (() => {
     var __webpack_modules__ = {
             68785: (e, t, n) => {
                 "use strict";
                 n.d(t, {
                     B: () => i,
                     Id: () => r,
@@ -7379,17 +7379,17 @@
                                 children: i && (0, Xi.jsx)(Li.Hp, {
                                     children: (0, Xi.jsx)(Ii.Z, {
                                         content: i,
                                         placement: Pi.u.TOP_RIGHT
                                     })
                                 })
                             }), (0, Xi.jsx)(o.Z, {
-                                "data-testid": "stColorPickerPopover",
                                 onClose: this.onColorClose,
                                 content: () => (0, Xi.jsx)(Fi, {
+                                    "data-testid": "stColorPickerPopover",
                                     children: (0, Xi.jsx)(Jo, {
                                         color: s,
                                         onChange: this.onColorChange,
                                         disableAlpha: !0
                                     })
                                 }),
                                 children: (0, Xi.jsxs)(Ui, {
@@ -36558,23 +36558,25 @@
                         }, e.prototype.toJSON = function() {
                             return this.constructor.toObject(this, r.util.toJSONOptions)
                         }, e.getTypeUrl = function(e) {
                             return void 0 === e && (e = "type.googleapis.com"), e + "/ArrowNamedDataSet"
                         }, e
                     })(), s.ArrowVegaLiteChart = (() => {
                         function e(e) {
-                            if (this.datasets = [], e)
+                            if (this.datasets = [], this.selectionMode = [], e)
                                 for (let t = Object.keys(e), n = 0; n < t.length; ++n) null != e[t[n]] && (this[t[n]] = e[t[n]])
                         }
-                        return e.prototype.spec = "", e.prototype.data = null, e.prototype.datasets = a.emptyArray, e.prototype.useContainerWidth = !1, e.prototype.theme = "", e.create = function(t) {
+                        return e.prototype.spec = "", e.prototype.data = null, e.prototype.datasets = a.emptyArray, e.prototype.useContainerWidth = !1, e.prototype.theme = "", e.prototype.id = "", e.prototype.selectionMode = a.emptyArray, e.prototype.formId = "", e.create = function(t) {
                             return new e(t)
                         }, e.encode = function(e, t) {
                             if (t || (t = i.create()), null != e.spec && Object.hasOwnProperty.call(e, "spec") && t.uint32(10).string(e.spec), null != e.data && Object.hasOwnProperty.call(e, "data") && s.Arrow.encode(e.data, t.uint32(18).fork()).ldelim(), null != e.datasets && e.datasets.length)
                                 for (let n = 0; n < e.datasets.length; ++n) s.ArrowNamedDataSet.encode(e.datasets[n], t.uint32(34).fork()).ldelim();
-                            return null != e.useContainerWidth && Object.hasOwnProperty.call(e, "useContainerWidth") && t.uint32(40).bool(e.useContainerWidth), null != e.theme && Object.hasOwnProperty.call(e, "theme") && t.uint32(50).string(e.theme), t
+                            if (null != e.useContainerWidth && Object.hasOwnProperty.call(e, "useContainerWidth") && t.uint32(40).bool(e.useContainerWidth), null != e.theme && Object.hasOwnProperty.call(e, "theme") && t.uint32(50).string(e.theme), null != e.id && Object.hasOwnProperty.call(e, "id") && t.uint32(58).string(e.id), null != e.selectionMode && e.selectionMode.length)
+                                for (let n = 0; n < e.selectionMode.length; ++n) t.uint32(66).string(e.selectionMode[n]);
+                            return null != e.formId && Object.hasOwnProperty.call(e, "formId") && t.uint32(74).string(e.formId), t
                         }, e.encodeDelimited = function(e, t) {
                             return this.encode(e, t).ldelim()
                         }, e.decode = function(e, t) {
                             e instanceof o || (e = o.create(e));
                             let n = void 0 === t ? e.len : e.pos + t,
                                 r = new s.ArrowVegaLiteChart;
                             for (; e.pos < n;) {
@@ -36591,14 +36593,23 @@
                                         break;
                                     case 5:
                                         r.useContainerWidth = e.bool();
                                         break;
                                     case 6:
                                         r.theme = e.string();
                                         break;
+                                    case 7:
+                                        r.id = e.string();
+                                        break;
+                                    case 8:
+                                        r.selectionMode && r.selectionMode.length || (r.selectionMode = []), r.selectionMode.push(e.string());
+                                        break;
+                                    case 9:
+                                        r.formId = e.string();
+                                        break;
                                     default:
                                         e.skipType(7 & t)
                                 }
                             }
                             return r
                         }, e.decodeDelimited = function(e) {
                             return e instanceof o || (e = new o(e)), this.decode(e, e.uint32())
@@ -36612,15 +36623,23 @@
                             if (null != e.datasets && e.hasOwnProperty("datasets")) {
                                 if (!Array.isArray(e.datasets)) return "datasets: array expected";
                                 for (let t = 0; t < e.datasets.length; ++t) {
                                     let n = s.ArrowNamedDataSet.verify(e.datasets[t]);
                                     if (n) return "datasets." + n
                                 }
                             }
-                            return null != e.useContainerWidth && e.hasOwnProperty("useContainerWidth") && "boolean" !== typeof e.useContainerWidth ? "useContainerWidth: boolean expected" : null != e.theme && e.hasOwnProperty("theme") && !a.isString(e.theme) ? "theme: string expected" : null
+                            if (null != e.useContainerWidth && e.hasOwnProperty("useContainerWidth") && "boolean" !== typeof e.useContainerWidth) return "useContainerWidth: boolean expected";
+                            if (null != e.theme && e.hasOwnProperty("theme") && !a.isString(e.theme)) return "theme: string expected";
+                            if (null != e.id && e.hasOwnProperty("id") && !a.isString(e.id)) return "id: string expected";
+                            if (null != e.selectionMode && e.hasOwnProperty("selectionMode")) {
+                                if (!Array.isArray(e.selectionMode)) return "selectionMode: array expected";
+                                for (let t = 0; t < e.selectionMode.length; ++t)
+                                    if (!a.isString(e.selectionMode[t])) return "selectionMode: string[] expected"
+                            }
+                            return null != e.formId && e.hasOwnProperty("formId") && !a.isString(e.formId) ? "formId: string expected" : null
                         }, e.fromObject = function(e) {
                             if (e instanceof s.ArrowVegaLiteChart) return e;
                             let t = new s.ArrowVegaLiteChart;
                             if (null != e.spec && (t.spec = String(e.spec)), null != e.data) {
                                 if ("object" !== typeof e.data) throw TypeError(".ArrowVegaLiteChart.data: object expected");
                                 t.data = s.Arrow.fromObject(e.data)
                             }
@@ -36628,23 +36647,32 @@
                                 if (!Array.isArray(e.datasets)) throw TypeError(".ArrowVegaLiteChart.datasets: array expected");
                                 t.datasets = [];
                                 for (let n = 0; n < e.datasets.length; ++n) {
                                     if ("object" !== typeof e.datasets[n]) throw TypeError(".ArrowVegaLiteChart.datasets: object expected");
                                     t.datasets[n] = s.ArrowNamedDataSet.fromObject(e.datasets[n])
                                 }
                             }
-                            return null != e.useContainerWidth && (t.useContainerWidth = Boolean(e.useContainerWidth)), null != e.theme && (t.theme = String(e.theme)), t
+                            if (null != e.useContainerWidth && (t.useContainerWidth = Boolean(e.useContainerWidth)), null != e.theme && (t.theme = String(e.theme)), null != e.id && (t.id = String(e.id)), e.selectionMode) {
+                                if (!Array.isArray(e.selectionMode)) throw TypeError(".ArrowVegaLiteChart.selectionMode: array expected");
+                                t.selectionMode = [];
+                                for (let n = 0; n < e.selectionMode.length; ++n) t.selectionMode[n] = String(e.selectionMode[n])
+                            }
+                            return null != e.formId && (t.formId = String(e.formId)), t
                         }, e.toObject = function(e, t) {
                             t || (t = {});
                             let n = {};
-                            if ((t.arrays || t.defaults) && (n.datasets = []), t.defaults && (n.spec = "", n.data = null, n.useContainerWidth = !1, n.theme = ""), null != e.spec && e.hasOwnProperty("spec") && (n.spec = e.spec), null != e.data && e.hasOwnProperty("data") && (n.data = s.Arrow.toObject(e.data, t)), e.datasets && e.datasets.length) {
+                            if ((t.arrays || t.defaults) && (n.datasets = [], n.selectionMode = []), t.defaults && (n.spec = "", n.data = null, n.useContainerWidth = !1, n.theme = "", n.id = "", n.formId = ""), null != e.spec && e.hasOwnProperty("spec") && (n.spec = e.spec), null != e.data && e.hasOwnProperty("data") && (n.data = s.Arrow.toObject(e.data, t)), e.datasets && e.datasets.length) {
                                 n.datasets = [];
                                 for (let r = 0; r < e.datasets.length; ++r) n.datasets[r] = s.ArrowNamedDataSet.toObject(e.datasets[r], t)
                             }
-                            return null != e.useContainerWidth && e.hasOwnProperty("useContainerWidth") && (n.useContainerWidth = e.useContainerWidth), null != e.theme && e.hasOwnProperty("theme") && (n.theme = e.theme), n
+                            if (null != e.useContainerWidth && e.hasOwnProperty("useContainerWidth") && (n.useContainerWidth = e.useContainerWidth), null != e.theme && e.hasOwnProperty("theme") && (n.theme = e.theme), null != e.id && e.hasOwnProperty("id") && (n.id = e.id), e.selectionMode && e.selectionMode.length) {
+                                n.selectionMode = [];
+                                for (let t = 0; t < e.selectionMode.length; ++t) n.selectionMode[t] = e.selectionMode[t]
+                            }
+                            return null != e.formId && e.hasOwnProperty("formId") && (n.formId = e.formId), n
                         }, e.prototype.toJSON = function() {
                             return this.constructor.toObject(this, r.util.toJSONOptions)
                         }, e.getTypeUrl = function(e) {
                             return void 0 === e && (e = "type.googleapis.com"), e + "/ArrowVegaLiteChart"
                         }, e
                     })(), s.Audio = (() => {
                         function e(e) {
@@ -116042,15 +116070,15 @@
         })
     }, __webpack_require__.f = {}, __webpack_require__.e = e => Promise.all(Object.keys(__webpack_require__.f).reduce(((t, n) => (__webpack_require__.f[n](e, t), t)), [])), __webpack_require__.u = e => "static/js/" + e + "." + {
         178: "7bea8c5d",
         329: "464ed8ec",
         474: "87506447",
         937: "a1248039",
         1074: "73973756",
-        1168: "7452e363",
+        1168: "14f7c6ff",
         1307: "0f0cca93",
         1451: "3b0a3e31",
         1479: "6709db03",
         1792: "8bd6ce2a",
         2178: "90362aae",
         2187: "9469f035",
         2469: "09ea79bb",
@@ -116069,29 +116097,29 @@
         4500: "b6f348d1",
         4666: "c4b22a63",
         5106: "44f0ff51",
         5117: "04bfe5d3",
         5249: "f2f4070d",
         5345: "65c91ee7",
         5379: "6571574f",
-        5441: "5bacdeda",
+        5441: "1b94928f",
         5791: "9a42fb4b",
         6013: "4ba2d616",
         6405: "ac5a6f23",
         6718: "802da17e",
         6853: "93dd1c4c",
         6950: "70fe55c2",
         7142: "83028745",
         7175: "be4076bc",
         7323: "b74cc85b",
         7483: "64f23be7",
         7602: "e8abc06b",
         7805: "acc6316a",
         8005: "43974a35",
-        8148: "cc5b50d8",
+        8148: "a5f74d47",
         8427: "bd0a7cf3",
         8477: "de889fe5",
         8492: "0d93bd08",
         8536: "f8de3d9a",
         8570: "6de19120",
         8691: "9ccf7f89",
         9330: "2b4c99e0",
@@ -117026,15 +117054,18 @@
                         data: new Ve.fu(e.data)
                     }))) : [];
                 const r = {
                     data: t,
                     spec: e.spec,
                     datasets: n,
                     useContainerWidth: e.useContainerWidth,
-                    vegaLiteTheme: e.theme
+                    vegaLiteTheme: e.theme,
+                    id: e.id,
+                    selectionMode: e.selectionMode,
+                    formId: e.formId
                 };
                 return this.lazyVegaLiteChartElement = r, r
             }
             getIn() {}
             setIn() {
                 throw new Error("'setIn' cannot be called on an ElementNode")
             }
@@ -121176,19 +121207,14 @@
                         })
                     }
                     case "arrowTable":
                         return (0, ze.jsx)($r, {
                             element: t.quiverElement,
                             ...n
                         });
-                    case "arrowVegaLiteChart":
-                        return (0, ze.jsx)(ji, {
-                            element: t.vegaLiteChartElement,
-                            ...n
-                        });
                     case "audio":
                         return (0, ze.jsx)(Ii, {
                             element: t.element.audio,
                             endpoints: e.endpoints,
                             ...n,
                             elementMgr: e.widgetMgr
                         });
@@ -121323,14 +121349,20 @@
                             data: t.quiverElement,
                             ...e.id && {
                                 key: e.id
                             },
                             ...r
                         })
                     }
+                    case "arrowVegaLiteChart":
+                        const o = t.vegaLiteChartElement;
+                        return (0, ze.jsx)(ji, {
+                            element: o,
+                            ...r
+                        }, o.id || void 0);
                     case "button": {
                         const n = t.element.button;
                         if (r.disabled = r.disabled || n.disabled, n.isFormSubmitter) {
                             const {
                                 formId: t
                             } = n, o = e.formsData.formsWithUploads.has(t);
                             return (0, ze.jsx)(Si, {
```

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/js/main.45247b52.js.LICENSE.txt` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/main.32c71338.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/MaterialSymbols-Outlined.909d2dce4aba724ad02f.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/MaterialSymbols-Outlined.909d2dce4aba724ad02f.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg` & `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/string_util.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/string_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/temporary_directory.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/temporary_directory.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/testing/__init__.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/testing/v1/__init__.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/testing/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/testing/v1/app_test.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/testing/v1/app_test.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/testing/v1/element_tree.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/testing/v1/element_tree.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/testing/v1/local_script_runner.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/testing/v1/local_script_runner.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/testing/v1/util.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/testing/v1/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/time_util.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/time_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/type_util.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/type_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/url_util.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/url_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/user_info.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/user_info.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/util.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/vendor/ipython/modified_sys_path.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/vendor/ipython/modified_sys_path.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/vendor/pympler/asizeof.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/vendor/pympler/asizeof.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/version.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/version.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/watcher/__init__.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/watcher/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/watcher/event_based_path_watcher.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/watcher/event_based_path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/watcher/local_sources_watcher.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/watcher/local_sources_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/watcher/path_watcher.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/watcher/path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/watcher/polling_path_watcher.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/watcher/polling_path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/watcher/util.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/watcher/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/web/__init__.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/web/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/web/bootstrap.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/web/bootstrap.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/web/cache_storage_manager_config.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/web/cache_storage_manager_config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/web/cli.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/web/cli.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/web/server/__init__.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/web/server/app_static_file_handler.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/app_static_file_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/web/server/browser_websocket_handler.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/browser_websocket_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/web/server/component_request_handler.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/component_request_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/web/server/media_file_handler.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/media_file_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/web/server/routes.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/routes.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/web/server/server.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/server.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/web/server/server_util.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/server_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/web/server/stats_request_handler.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/stats_request_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/web/server/upload_file_request_handler.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/upload_file_request_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit/web/server/websocket_headers.py` & `streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/websocket_headers.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit_nightly.egg-info/PKG-INFO` & `streamlit_nightly-1.34.1.dev20240514/streamlit_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-nightly
-Version: 1.34.1.dev20240513
+Version: 1.34.1.dev20240514
 Summary: A faster way to build and share data apps
 Home-page: https://streamlit.io
 Author: Snowflake Inc
 Author-email: hello@streamlit.io
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/streamlit/streamlit
 Project-URL: Bug Tracker, https://github.com/streamlit/streamlit/issues
```

### Comparing `streamlit_nightly-1.34.1.dev20240513/streamlit_nightly.egg-info/SOURCES.txt` & `streamlit_nightly-1.34.1.dev20240514/streamlit_nightly.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -338,15 +338,15 @@
 streamlit/static/favicon.png
 streamlit/static/index.html
 streamlit/static/static/css/3466.8b8f33d6.chunk.css
 streamlit/static/static/css/5441.e3b876c5.chunk.css
 streamlit/static/static/css/8148.49dfd2ce.chunk.css
 streamlit/static/static/css/main.3aaaea00.css
 streamlit/static/static/js/1074.73973756.chunk.js
-streamlit/static/static/js/1168.7452e363.chunk.js
+streamlit/static/static/js/1168.14f7c6ff.chunk.js
 streamlit/static/static/js/1307.0f0cca93.chunk.js
 streamlit/static/static/js/1451.3b0a3e31.chunk.js
 streamlit/static/static/js/1479.6709db03.chunk.js
 streamlit/static/static/js/178.7bea8c5d.chunk.js
 streamlit/static/static/js/1792.8bd6ce2a.chunk.js
 streamlit/static/static/js/2178.90362aae.chunk.js
 streamlit/static/static/js/2187.9469f035.chunk.js
@@ -371,15 +371,15 @@
 streamlit/static/static/js/4666.c4b22a63.chunk.js
 streamlit/static/static/js/474.87506447.chunk.js
 streamlit/static/static/js/5106.44f0ff51.chunk.js
 streamlit/static/static/js/5117.04bfe5d3.chunk.js
 streamlit/static/static/js/5249.f2f4070d.chunk.js
 streamlit/static/static/js/5345.65c91ee7.chunk.js
 streamlit/static/static/js/5379.6571574f.chunk.js
-streamlit/static/static/js/5441.5bacdeda.chunk.js
+streamlit/static/static/js/5441.1b94928f.chunk.js
 streamlit/static/static/js/5791.9a42fb4b.chunk.js
 streamlit/static/static/js/6013.4ba2d616.chunk.js
 streamlit/static/static/js/6405.ac5a6f23.chunk.js
 streamlit/static/static/js/6718.802da17e.chunk.js
 streamlit/static/static/js/6853.93dd1c4c.chunk.js
 streamlit/static/static/js/6950.70fe55c2.chunk.js
 streamlit/static/static/js/6950.70fe55c2.chunk.js.LICENSE.txt
@@ -388,30 +388,30 @@
 streamlit/static/static/js/7323.b74cc85b.chunk.js
 streamlit/static/static/js/7323.b74cc85b.chunk.js.LICENSE.txt
 streamlit/static/static/js/7483.64f23be7.chunk.js
 streamlit/static/static/js/7483.64f23be7.chunk.js.LICENSE.txt
 streamlit/static/static/js/7602.e8abc06b.chunk.js
 streamlit/static/static/js/7805.acc6316a.chunk.js
 streamlit/static/static/js/8005.43974a35.chunk.js
-streamlit/static/static/js/8148.cc5b50d8.chunk.js
+streamlit/static/static/js/8148.a5f74d47.chunk.js
 streamlit/static/static/js/8427.bd0a7cf3.chunk.js
 streamlit/static/static/js/8477.de889fe5.chunk.js
 streamlit/static/static/js/8492.0d93bd08.chunk.js
 streamlit/static/static/js/8536.f8de3d9a.chunk.js
 streamlit/static/static/js/8570.6de19120.chunk.js
 streamlit/static/static/js/8691.9ccf7f89.chunk.js
 streamlit/static/static/js/9330.2b4c99e0.chunk.js
 streamlit/static/static/js/9336.2d95d840.chunk.js
 streamlit/static/static/js/937.a1248039.chunk.js
 streamlit/static/static/js/937.a1248039.chunk.js.LICENSE.txt
 streamlit/static/static/js/9656.8c935274.chunk.js
 streamlit/static/static/js/9758.6e6d8662.chunk.js
 streamlit/static/static/js/9865.fd93213d.chunk.js
-streamlit/static/static/js/main.45247b52.js
-streamlit/static/static/js/main.45247b52.js.LICENSE.txt
+streamlit/static/static/js/main.32c71338.js
+streamlit/static/static/js/main.32c71338.js.LICENSE.txt
 streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2
 streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf
 streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff
 streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf
 streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2
 streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff
 streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf
```

### Comparing `streamlit_nightly-1.34.1.dev20240513/tests/testutil.py` & `streamlit_nightly-1.34.1.dev20240514/tests/testutil.py`

 * *Files identical despite different names*

