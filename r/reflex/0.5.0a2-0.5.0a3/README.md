# Comparing `tmp/reflex-0.5.0a2.tar.gz` & `tmp/reflex-0.5.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex-0.5.0a2.tar", max compression
+gzip compressed data, was "reflex-0.5.0a3.tar", max compression
```

## Comparing `reflex-0.5.0a2.tar` & `reflex-0.5.0a3.tar`

### file list

```diff
@@ -1,520 +1,520 @@
--rw-r--r--   0        0        0    11358 2023-07-20 22:42:41.698164 reflex-0.5.0a2/LICENSE
--rw-r--r--   0        0        0     9842 2024-05-07 15:33:05.680965 reflex-0.5.0a2/README.md
--rw-r--r--   0        0        0     2974 2024-05-11 03:29:51.729539 reflex-0.5.0a2/pyproject.toml
--rw-r--r--   0        0        0     4286 2023-11-09 03:24:59.498329 reflex-0.5.0a2/reflex/.templates/apps/blank/assets/favicon.ico
--rw-r--r--   0        0        0        0 2023-11-09 03:24:59.498383 reflex-0.5.0a2/reflex/.templates/apps/blank/code/__init__.py
--rw-r--r--   0        0        0      926 2024-05-09 00:05:27.334397 reflex-0.5.0a2/reflex/.templates/apps/blank/code/blank.py
--rw-r--r--   0        0        0       32 2023-11-09 03:24:59.498951 reflex-0.5.0a2/reflex/.templates/apps/demo/.gitignore
--rw-r--r--   0        0        0     4286 2023-11-09 03:24:59.499075 reflex-0.5.0a2/reflex/.templates/apps/demo/assets/favicon.ico
--rw-r--r--   0        0        0     1475 2023-11-09 03:24:59.499137 reflex-0.5.0a2/reflex/.templates/apps/demo/assets/github.svg
--rw-r--r--   0        0        0     1899 2023-11-09 03:24:59.499199 reflex-0.5.0a2/reflex/.templates/apps/demo/assets/icon.svg
--rw-r--r--   0        0        0     5403 2023-11-09 03:24:59.499298 reflex-0.5.0a2/reflex/.templates/apps/demo/assets/logo.svg
--rw-r--r--   0        0        0      807 2023-11-09 03:24:59.499362 reflex-0.5.0a2/reflex/.templates/apps/demo/assets/paneleft.svg
--rw-r--r--   0        0        0       32 2023-11-09 03:24:59.499458 reflex-0.5.0a2/reflex/.templates/apps/demo/code/__init__.py
--rw-r--r--   0        0        0     2928 2024-02-17 20:02:02.399454 reflex-0.5.0a2/reflex/.templates/apps/demo/code/demo.py
--rw-r--r--   0        0        0      194 2023-11-09 03:24:59.499716 reflex-0.5.0a2/reflex/.templates/apps/demo/code/pages/__init__.py
--rw-r--r--   0        0        0      706 2024-02-17 20:02:02.399560 reflex-0.5.0a2/reflex/.templates/apps/demo/code/pages/chatapp.py
--rw-r--r--   0        0        0    10906 2024-04-24 21:16:40.835599 reflex-0.5.0a2/reflex/.templates/apps/demo/code/pages/datatable.py
--rw-r--r--   0        0        0     8381 2024-04-24 21:16:40.835772 reflex-0.5.0a2/reflex/.templates/apps/demo/code/pages/forms.py
--rw-r--r--   0        0        0     8519 2024-03-20 23:54:55.830529 reflex-0.5.0a2/reflex/.templates/apps/demo/code/pages/graphing.py
--rw-r--r--   0        0        0     1822 2024-02-17 20:02:02.400769 reflex-0.5.0a2/reflex/.templates/apps/demo/code/pages/home.py
--rw-r--r--   0        0        0     4722 2024-02-17 20:02:02.400919 reflex-0.5.0a2/reflex/.templates/apps/demo/code/sidebar.py
--rw-r--r--   0        0        0      510 2023-11-09 03:24:59.500529 reflex-0.5.0a2/reflex/.templates/apps/demo/code/state.py
--rw-r--r--   0        0        0      912 2023-11-09 03:24:59.500616 reflex-0.5.0a2/reflex/.templates/apps/demo/code/states/form_state.py
--rw-r--r--   0        0        0     1189 2023-11-09 03:24:59.500682 reflex-0.5.0a2/reflex/.templates/apps/demo/code/states/pie_state.py
--rw-r--r--   0        0        0     1486 2024-02-17 20:02:02.401042 reflex-0.5.0a2/reflex/.templates/apps/demo/code/styles.py
--rw-r--r--   0        0        0        0 2023-11-09 03:24:59.500792 reflex-0.5.0a2/reflex/.templates/apps/demo/code/webui/__init__.py
--rw-r--r--   0        0        0      120 2023-11-09 03:24:59.500879 reflex-0.5.0a2/reflex/.templates/apps/demo/code/webui/components/__init__.py
--rw-r--r--   0        0        0     3584 2024-02-17 20:02:02.401162 reflex-0.5.0a2/reflex/.templates/apps/demo/code/webui/components/chat.py
--rw-r--r--   0        0        0      680 2023-11-09 03:24:59.500996 reflex-0.5.0a2/reflex/.templates/apps/demo/code/webui/components/loading_icon.py
--rw-r--r--   0        0        0     1829 2024-02-17 20:02:02.401269 reflex-0.5.0a2/reflex/.templates/apps/demo/code/webui/components/modal.py
--rw-r--r--   0        0        0     2251 2024-02-17 20:02:02.401372 reflex-0.5.0a2/reflex/.templates/apps/demo/code/webui/components/navbar.py
--rw-r--r--   0        0        0     1735 2024-02-17 20:02:02.401457 reflex-0.5.0a2/reflex/.templates/apps/demo/code/webui/components/sidebar.py
--rw-r--r--   0        0        0     4001 2023-11-09 03:24:59.501230 reflex-0.5.0a2/reflex/.templates/apps/demo/code/webui/state.py
--rw-r--r--   0        0        0     2281 2024-02-17 20:02:02.401582 reflex-0.5.0a2/reflex/.templates/apps/demo/code/webui/styles.py
--rw-r--r--   0        0        0       74 2023-10-22 18:57:13.188650 reflex-0.5.0a2/reflex/.templates/jinja/app/rxconfig.py.jinja2
--rw-r--r--   0        0        0      127 2024-03-20 23:54:55.833038 reflex-0.5.0a2/reflex/.templates/jinja/custom_components/README.md.jinja2
--rw-r--r--   0        0        0       32 2024-03-20 23:54:55.833129 reflex-0.5.0a2/reflex/.templates/jinja/custom_components/__init__.py.jinja2
--rw-r--r--   0        0        0      826 2024-03-20 23:54:55.833525 reflex-0.5.0a2/reflex/.templates/jinja/custom_components/demo_app.py.jinja2
--rw-r--r--   0        0        0      614 2024-04-04 14:57:26.374812 reflex-0.5.0a2/reflex/.templates/jinja/custom_components/pyproject.toml.jinja2
--rw-r--r--   0        0        0     2403 2024-04-05 17:14:14.457446 reflex-0.5.0a2/reflex/.templates/jinja/custom_components/src.py.jinja2
--rw-r--r--   0        0        0      548 2023-10-22 18:57:13.188813 reflex-0.5.0a2/reflex/.templates/jinja/web/package.json.jinja2
--rw-r--r--   0        0        0      930 2024-03-20 23:54:55.834237 reflex-0.5.0a2/reflex/.templates/jinja/web/pages/_app.js.jinja2
--rw-r--r--   0        0        0      182 2023-07-20 22:42:41.708822 reflex-0.5.0a2/reflex/.templates/jinja/web/pages/_document.js.jinja2
--rw-r--r--   0        0        0      400 2024-02-06 00:51:31.970380 reflex-0.5.0a2/reflex/.templates/jinja/web/pages/base_page.js.jinja2
--rw-r--r--   0        0        0       86 2023-10-22 18:57:13.188983 reflex-0.5.0a2/reflex/.templates/jinja/web/pages/component.js.jinja2
--rw-r--r--   0        0        0      882 2023-12-01 04:51:31.091531 reflex-0.5.0a2/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
--rw-r--r--   0        0        0      343 2024-04-04 14:57:26.375114 reflex-0.5.0a2/reflex/.templates/jinja/web/pages/index.js.jinja2
--rw-r--r--   0        0        0      388 2024-04-05 17:14:14.457553 reflex-0.5.0a2/reflex/.templates/jinja/web/pages/stateful_component.js.jinja2
--rw-r--r--   0        0        0      101 2023-12-01 04:51:31.092250 reflex-0.5.0a2/reflex/.templates/jinja/web/pages/stateful_components.js.jinja2
--rw-r--r--   0        0        0     3883 2024-02-06 00:51:31.970618 reflex-0.5.0a2/reflex/.templates/jinja/web/pages/utils.js.jinja2
--rw-r--r--   0        0        0      141 2023-12-06 18:41:46.628030 reflex-0.5.0a2/reflex/.templates/jinja/web/styles/styles.css.jinja2
--rw-r--r--   0        0        0      761 2024-05-11 03:29:42.707807 reflex-0.5.0a2/reflex/.templates/jinja/web/tailwind.config.js.jinja2
--rw-r--r--   0        0        0     3790 2024-03-20 23:54:55.834608 reflex-0.5.0a2/reflex/.templates/jinja/web/utils/context.js.jinja2
--rw-r--r--   0        0        0       37 2023-12-06 19:37:00.189183 reflex-0.5.0a2/reflex/.templates/jinja/web/utils/theme.js.jinja2
--rw-r--r--   0        0        0      417 2023-07-20 22:42:41.709243 reflex-0.5.0a2/reflex/.templates/web/.gitignore
--rw-r--r--   0        0        0      595 2023-10-30 01:36:56.133208 reflex-0.5.0a2/reflex/.templates/web/components/reflex/chakra_color_mode_provider.js
--rw-r--r--   0        0        0      645 2024-03-20 23:54:55.835034 reflex-0.5.0a2/reflex/.templates/web/components/reflex/radix_themes_color_mode_provider.js
--rw-r--r--   0        0        0       97 2023-10-22 18:57:13.190257 reflex-0.5.0a2/reflex/.templates/web/jsconfig.json
--rw-r--r--   0        0        0      118 2023-11-22 05:49:24.669539 reflex-0.5.0a2/reflex/.templates/web/next.config.js
--rw-r--r--   0        0        0       82 2023-07-20 22:42:41.710359 reflex-0.5.0a2/reflex/.templates/web/postcss.config.js
--rw-r--r--   0        0        0       59 2023-07-20 22:42:41.710616 reflex-0.5.0a2/reflex/.templates/web/styles/tailwind.css
--rw-r--r--   0        0        0     1254 2023-09-16 20:27:37.277783 reflex-0.5.0a2/reflex/.templates/web/utils/client_side_routing.js
--rw-r--r--   0        0        0     1622 2024-02-06 00:51:31.970968 reflex-0.5.0a2/reflex/.templates/web/utils/helpers/dataeditor.js
--rw-r--r--   0        0        0      528 2024-05-05 01:15:24.052298 reflex-0.5.0a2/reflex/.templates/web/utils/helpers/debounce.js
--rw-r--r--   0        0        0     1152 2023-11-22 05:49:24.669991 reflex-0.5.0a2/reflex/.templates/web/utils/helpers/range.js
--rw-r--r--   0        0        0      566 2024-05-05 01:15:24.052363 reflex-0.5.0a2/reflex/.templates/web/utils/helpers/throttle.js
--rw-r--r--   0        0        0    22511 2024-05-05 01:15:24.052487 reflex-0.5.0a2/reflex/.templates/web/utils/state.js
--rw-r--r--   0        0        0     5831 2024-05-09 00:05:27.334655 reflex-0.5.0a2/reflex/__init__.py
--rw-r--r--   0        0        0     7791 2024-05-09 12:11:15.217578 reflex-0.5.0a2/reflex/__init__.pyi
--rw-r--r--   0        0        0      108 2023-08-05 17:01:44.301997 reflex-0.5.0a2/reflex/__main__.py
--rw-r--r--   0        0        0      373 2023-07-20 22:42:41.710893 reflex-0.5.0a2/reflex/admin.py
--rw-r--r--   0        0        0    46314 2024-05-09 00:05:27.335022 reflex-0.5.0a2/reflex/app.py
--rw-r--r--   0        0        0     1152 2024-05-05 01:15:24.053241 reflex-0.5.0a2/reflex/app_module_for_backend.py
--rw-r--r--   0        0        0     4213 2024-05-09 00:05:27.335300 reflex-0.5.0a2/reflex/base.py
--rw-r--r--   0        0        0       27 2023-07-20 22:42:41.711176 reflex-0.5.0a2/reflex/compiler/__init__.py
--rw-r--r--   0        0        0    17455 2024-05-07 15:33:05.682544 reflex-0.5.0a2/reflex/compiler/compiler.py
--rw-r--r--   0        0        0     4344 2024-03-20 23:54:55.838388 reflex-0.5.0a2/reflex/compiler/templates.py
--rw-r--r--   0        0        0    13274 2024-05-09 00:05:27.335443 reflex-0.5.0a2/reflex/compiler/utils.py
--rw-r--r--   0        0        0      552 2024-05-05 01:15:24.053486 reflex-0.5.0a2/reflex/components/__init__.py
--rw-r--r--   0        0        0      325 2024-02-06 00:51:31.973078 reflex-0.5.0a2/reflex/components/base/__init__.py
--rw-r--r--   0        0        0      573 2024-02-06 00:51:31.973178 reflex-0.5.0a2/reflex/components/base/app_wrap.py
--rw-r--r--   0        0        0     2890 2024-04-24 19:31:24.924269 reflex-0.5.0a2/reflex/components/base/app_wrap.pyi
--rw-r--r--   0        0        0     1234 2024-04-04 14:57:26.376921 reflex-0.5.0a2/reflex/components/base/bare.py
--rw-r--r--   0        0        0      151 2023-07-20 22:42:41.711762 reflex-0.5.0a2/reflex/components/base/body.py
--rw-r--r--   0        0        0     3206 2024-04-24 19:31:56.503225 reflex-0.5.0a2/reflex/components/base/body.pyi
--rw-r--r--   0        0        0      583 2024-03-20 23:54:55.839153 reflex-0.5.0a2/reflex/components/base/document.py
--rw-r--r--   0        0        0    14232 2024-04-24 19:31:51.758673 reflex-0.5.0a2/reflex/components/base/document.pyi
--rw-r--r--   0        0        0      312 2024-02-06 00:51:31.973871 reflex-0.5.0a2/reflex/components/base/fragment.py
--rw-r--r--   0        0        0     3218 2024-04-24 19:31:51.784884 reflex-0.5.0a2/reflex/components/base/fragment.pyi
--rw-r--r--   0        0        0      297 2023-12-05 17:15:35.585518 reflex-0.5.0a2/reflex/components/base/head.py
--rw-r--r--   0        0        0     6002 2024-04-24 19:31:53.335977 reflex-0.5.0a2/reflex/components/base/head.pyi
--rw-r--r--   0        0        0      929 2023-07-20 22:42:41.711911 reflex-0.5.0a2/reflex/components/base/link.py
--rw-r--r--   0        0        0     6990 2024-04-24 19:31:27.077164 reflex-0.5.0a2/reflex/components/base/link.pyi
--rw-r--r--   0        0        0     1438 2023-09-16 20:27:37.279391 reflex-0.5.0a2/reflex/components/base/meta.py
--rw-r--r--   0        0        0    12804 2024-04-24 19:31:22.783259 reflex-0.5.0a2/reflex/components/base/meta.pyi
--rw-r--r--   0        0        0     2298 2023-10-30 01:36:56.136333 reflex-0.5.0a2/reflex/components/base/script.py
--rw-r--r--   0        0        0     4500 2024-04-24 19:31:45.804898 reflex-0.5.0a2/reflex/components/base/script.pyi
--rw-r--r--   0        0        0     6378 2024-02-17 20:02:02.406461 reflex-0.5.0a2/reflex/components/chakra/__init__.py
--rw-r--r--   0        0        0     5242 2024-02-07 21:49:00.589344 reflex-0.5.0a2/reflex/components/chakra/base.py
--rw-r--r--   0        0        0    10917 2024-04-24 19:31:39.254151 reflex-0.5.0a2/reflex/components/chakra/base.pyi
--rw-r--r--   0        0        0      459 2024-02-17 20:02:02.406937 reflex-0.5.0a2/reflex/components/chakra/datadisplay/__init__.py
--rw-r--r--   0        0        0      352 2024-02-07 21:48:43.271089 reflex-0.5.0a2/reflex/components/chakra/datadisplay/badge.py
--rw-r--r--   0        0        0     3654 2024-04-24 19:31:56.520176 reflex-0.5.0a2/reflex/components/chakra/datadisplay/badge.pyi
--rw-r--r--   0        0        0      174 2024-02-17 20:02:02.407242 reflex-0.5.0a2/reflex/components/chakra/datadisplay/code.py
--rw-r--r--   0        0        0     3229 2024-04-24 19:31:20.836024 reflex-0.5.0a2/reflex/components/chakra/datadisplay/code.pyi
--rw-r--r--   0        0        0      657 2024-02-07 21:48:43.271979 reflex-0.5.0a2/reflex/components/chakra/datadisplay/divider.py
--rw-r--r--   0        0        0     3934 2024-04-24 19:31:33.713586 reflex-0.5.0a2/reflex/components/chakra/datadisplay/divider.pyi
--rw-r--r--   0        0        0      180 2024-02-07 21:48:43.272341 reflex-0.5.0a2/reflex/components/chakra/datadisplay/keyboard_key.py
--rw-r--r--   0        0        0     3251 2024-04-24 19:31:32.872876 reflex-0.5.0a2/reflex/components/chakra/datadisplay/keyboard_key.pyi
--rw-r--r--   0        0        0     1484 2024-05-05 01:15:24.053780 reflex-0.5.0a2/reflex/components/chakra/datadisplay/list.py
--rw-r--r--   0        0        0    12991 2024-05-05 01:15:24.053953 reflex-0.5.0a2/reflex/components/chakra/datadisplay/list.pyi
--rw-r--r--   0        0        0     2149 2024-02-07 21:48:43.272980 reflex-0.5.0a2/reflex/components/chakra/datadisplay/stat.py
--rw-r--r--   0        0        0    17461 2024-04-24 19:31:58.481785 reflex-0.5.0a2/reflex/components/chakra/datadisplay/stat.pyi
--rw-r--r--   0        0        0     9122 2024-02-07 21:48:43.273484 reflex-0.5.0a2/reflex/components/chakra/datadisplay/table.py
--rw-r--r--   0        0        0    27252 2024-04-24 19:32:01.076794 reflex-0.5.0a2/reflex/components/chakra/datadisplay/table.pyi
--rw-r--r--   0        0        0     2294 2024-02-07 21:48:43.273971 reflex-0.5.0a2/reflex/components/chakra/datadisplay/tag.py
--rw-r--r--   0        0        0    15734 2024-04-24 19:31:39.394572 reflex-0.5.0a2/reflex/components/chakra/datadisplay/tag.pyi
--rw-r--r--   0        0        0      384 2024-02-06 00:51:31.976988 reflex-0.5.0a2/reflex/components/chakra/disclosure/__init__.py
--rw-r--r--   0        0        0     3510 2024-04-24 21:16:40.836539 reflex-0.5.0a2/reflex/components/chakra/disclosure/accordion.py
--rw-r--r--   0        0        0    15803 2024-04-24 19:31:46.785267 reflex-0.5.0a2/reflex/components/chakra/disclosure/accordion.pyi
--rw-r--r--   0        0        0     3295 2024-02-07 21:48:43.274669 reflex-0.5.0a2/reflex/components/chakra/disclosure/tabs.py
--rw-r--r--   0        0        0    18525 2024-04-24 19:31:51.181381 reflex-0.5.0a2/reflex/components/chakra/disclosure/tabs.pyi
--rw-r--r--   0        0        0     1732 2024-02-07 21:48:43.274917 reflex-0.5.0a2/reflex/components/chakra/disclosure/transition.py
--rw-r--r--   0        0        0    20003 2024-04-24 19:31:47.452515 reflex-0.5.0a2/reflex/components/chakra/disclosure/transition.pyi
--rw-r--r--   0        0        0      278 2024-02-07 21:48:43.275325 reflex-0.5.0a2/reflex/components/chakra/disclosure/visuallyhidden.py
--rw-r--r--   0        0        0     3258 2024-04-24 19:31:21.739444 reflex-0.5.0a2/reflex/components/chakra/disclosure/visuallyhidden.pyi
--rw-r--r--   0        0        0      313 2024-02-06 00:51:31.977813 reflex-0.5.0a2/reflex/components/chakra/feedback/__init__.py
--rw-r--r--   0        0        0     1623 2024-02-07 21:48:43.275534 reflex-0.5.0a2/reflex/components/chakra/feedback/alert.py
--rw-r--r--   0        0        0    12381 2024-04-24 19:31:36.018582 reflex-0.5.0a2/reflex/components/chakra/feedback/alert.pyi
--rw-r--r--   0        0        0     2006 2024-02-07 21:48:43.275746 reflex-0.5.0a2/reflex/components/chakra/feedback/circularprogress.py
--rw-r--r--   0        0        0     7637 2024-04-24 19:31:35.464688 reflex-0.5.0a2/reflex/components/chakra/feedback/circularprogress.pyi
--rw-r--r--   0        0        0      871 2024-02-07 21:48:43.275966 reflex-0.5.0a2/reflex/components/chakra/feedback/progress.py
--rw-r--r--   0        0        0     4278 2024-04-24 19:31:39.746055 reflex-0.5.0a2/reflex/components/chakra/feedback/progress.pyi
--rw-r--r--   0        0        0     1776 2024-02-07 21:48:43.276180 reflex-0.5.0a2/reflex/components/chakra/feedback/skeleton.py
--rw-r--r--   0        0        0    10690 2024-04-24 19:32:01.405002 reflex-0.5.0a2/reflex/components/chakra/feedback/skeleton.pyi
--rw-r--r--   0        0        0      704 2024-02-07 21:48:43.276461 reflex-0.5.0a2/reflex/components/chakra/feedback/spinner.py
--rw-r--r--   0        0        0     4107 2024-04-24 19:31:21.992081 reflex-0.5.0a2/reflex/components/chakra/feedback/spinner.pyi
--rw-r--r--   0        0        0     1453 2024-02-17 20:02:02.409691 reflex-0.5.0a2/reflex/components/chakra/forms/__init__.py
--rw-r--r--   0        0        0     2395 2024-02-07 21:48:43.276688 reflex-0.5.0a2/reflex/components/chakra/forms/button.py
--rw-r--r--   0        0        0    10545 2024-04-24 19:32:02.037829 reflex-0.5.0a2/reflex/components/chakra/forms/button.pyi
--rw-r--r--   0        0        0     2764 2024-02-07 21:48:43.277006 reflex-0.5.0a2/reflex/components/chakra/forms/checkbox.py
--rw-r--r--   0        0        0    10301 2024-04-24 19:31:34.287807 reflex-0.5.0a2/reflex/components/chakra/forms/checkbox.pyi
--rw-r--r--   0        0        0     2860 2024-02-17 20:02:02.410102 reflex-0.5.0a2/reflex/components/chakra/forms/colormodeswitch.py
--rw-r--r--   0        0        0    18459 2024-04-24 19:31:24.856589 reflex-0.5.0a2/reflex/components/chakra/forms/colormodeswitch.pyi
--rw-r--r--   0        0        0      246 2024-02-06 00:51:31.979244 reflex-0.5.0a2/reflex/components/chakra/forms/date_picker.py
--rw-r--r--   0        0        0     5841 2024-04-24 19:31:54.024641 reflex-0.5.0a2/reflex/components/chakra/forms/date_picker.pyi
--rw-r--r--   0        0        0      280 2024-02-06 00:51:31.979387 reflex-0.5.0a2/reflex/components/chakra/forms/date_time_picker.py
--rw-r--r--   0        0        0     5854 2024-04-24 19:31:40.823621 reflex-0.5.0a2/reflex/components/chakra/forms/date_time_picker.pyi
--rw-r--r--   0        0        0     2110 2024-02-07 21:48:43.277649 reflex-0.5.0a2/reflex/components/chakra/forms/editable.py
--rw-r--r--   0        0        0    13339 2024-04-24 19:31:15.703021 reflex-0.5.0a2/reflex/components/chakra/forms/editable.pyi
--rw-r--r--   0        0        0      246 2024-02-06 00:51:31.979682 reflex-0.5.0a2/reflex/components/chakra/forms/email.py
--rw-r--r--   0        0        0     5825 2024-04-24 19:31:50.788652 reflex-0.5.0a2/reflex/components/chakra/forms/email.pyi
--rw-r--r--   0        0        0     2579 2024-03-20 23:54:55.839690 reflex-0.5.0a2/reflex/components/chakra/forms/form.py
--rw-r--r--   0        0        0    20619 2024-04-24 19:31:56.858215 reflex-0.5.0a2/reflex/components/chakra/forms/form.pyi
--rw-r--r--   0        0        0      935 2024-02-06 00:51:31.980162 reflex-0.5.0a2/reflex/components/chakra/forms/iconbutton.py
--rw-r--r--   0        0        0     4668 2024-04-24 19:31:50.346409 reflex-0.5.0a2/reflex/components/chakra/forms/iconbutton.pyi
--rw-r--r--   0        0        0     4312 2024-03-20 23:54:55.840321 reflex-0.5.0a2/reflex/components/chakra/forms/input.py
--rw-r--r--   0        0        0    21514 2024-04-24 19:31:59.673777 reflex-0.5.0a2/reflex/components/chakra/forms/input.pyi
--rw-r--r--   0        0        0    12940 2024-02-06 00:51:31.980569 reflex-0.5.0a2/reflex/components/chakra/forms/multiselect.py
--rw-r--r--   0        0        0     4334 2024-02-07 21:48:43.278754 reflex-0.5.0a2/reflex/components/chakra/forms/numberinput.py
--rw-r--r--   0        0        0    18093 2024-04-24 19:31:56.097983 reflex-0.5.0a2/reflex/components/chakra/forms/numberinput.pyi
--rw-r--r--   0        0        0      256 2024-02-06 00:51:31.980851 reflex-0.5.0a2/reflex/components/chakra/forms/password.py
--rw-r--r--   0        0        0     5834 2024-04-24 19:31:37.858051 reflex-0.5.0a2/reflex/components/chakra/forms/password.pyi
--rw-r--r--   0        0        0     6503 2024-04-12 01:14:12.262063 reflex-0.5.0a2/reflex/components/chakra/forms/pininput.py
--rw-r--r--   0        0        0     9369 2024-05-05 01:15:24.054063 reflex-0.5.0a2/reflex/components/chakra/forms/pininput.pyi
--rw-r--r--   0        0        0     3172 2024-04-12 01:14:12.263122 reflex-0.5.0a2/reflex/components/chakra/forms/radio.py
--rw-r--r--   0        0        0     8410 2024-04-24 19:31:17.428977 reflex-0.5.0a2/reflex/components/chakra/forms/radio.pyi
--rw-r--r--   0        0        0     4543 2024-04-12 01:14:12.263746 reflex-0.5.0a2/reflex/components/chakra/forms/rangeslider.py
--rw-r--r--   0        0        0    13939 2024-04-24 19:31:59.377848 reflex-0.5.0a2/reflex/components/chakra/forms/rangeslider.pyi
--rw-r--r--   0        0        0     3624 2024-02-07 21:48:43.280461 reflex-0.5.0a2/reflex/components/chakra/forms/select.py
--rw-r--r--   0        0        0     8868 2024-04-24 19:31:48.346816 reflex-0.5.0a2/reflex/components/chakra/forms/select.pyi
--rw-r--r--   0        0        0     3532 2024-02-07 21:48:43.280779 reflex-0.5.0a2/reflex/components/chakra/forms/slider.py
--rw-r--r--   0        0        0    17461 2024-04-24 19:32:01.264082 reflex-0.5.0a2/reflex/components/chakra/forms/slider.pyi
--rw-r--r--   0        0        0     1838 2024-02-07 21:48:43.281044 reflex-0.5.0a2/reflex/components/chakra/forms/switch.py
--rw-r--r--   0        0        0     6531 2024-04-24 19:31:48.016708 reflex-0.5.0a2/reflex/components/chakra/forms/switch.pyi
--rw-r--r--   0        0        0     2474 2024-02-09 10:00:28.809203 reflex-0.5.0a2/reflex/components/chakra/forms/textarea.py
--rw-r--r--   0        0        0     5419 2024-04-24 19:31:51.889720 reflex-0.5.0a2/reflex/components/chakra/forms/textarea.pyi
--rw-r--r--   0        0        0      246 2024-02-06 00:51:31.982573 reflex-0.5.0a2/reflex/components/chakra/forms/time_picker.py
--rw-r--r--   0        0        0     5841 2024-04-24 19:31:46.686774 reflex-0.5.0a2/reflex/components/chakra/forms/time_picker.pyi
--rw-r--r--   0        0        0      487 2024-02-17 20:02:02.413006 reflex-0.5.0a2/reflex/components/chakra/layout/__init__.py
--rw-r--r--   0        0        0      315 2024-02-07 21:48:43.281752 reflex-0.5.0a2/reflex/components/chakra/layout/aspect_ratio.py
--rw-r--r--   0        0        0     3379 2024-04-24 19:31:52.881611 reflex-0.5.0a2/reflex/components/chakra/layout/aspect_ratio.pyi
--rw-r--r--   0        0        0      755 2024-02-07 21:48:43.281982 reflex-0.5.0a2/reflex/components/chakra/layout/box.py
--rw-r--r--   0        0        0     3662 2024-04-24 19:31:18.516418 reflex-0.5.0a2/reflex/components/chakra/layout/box.pyi
--rw-r--r--   0        0        0     2967 2024-02-07 21:48:43.282202 reflex-0.5.0a2/reflex/components/chakra/layout/card.py
--rw-r--r--   0        0        0    13850 2024-04-24 19:31:48.005155 reflex-0.5.0a2/reflex/components/chakra/layout/card.pyi
--rw-r--r--   0        0        0      389 2024-02-07 21:48:43.282417 reflex-0.5.0a2/reflex/components/chakra/layout/center.py
--rw-r--r--   0        0        0     8692 2024-04-24 19:31:24.264440 reflex-0.5.0a2/reflex/components/chakra/layout/center.pyi
--rw-r--r--   0        0        0      354 2024-02-07 21:48:43.282843 reflex-0.5.0a2/reflex/components/chakra/layout/container.py
--rw-r--r--   0        0        0     3431 2024-04-24 19:31:47.990635 reflex-0.5.0a2/reflex/components/chakra/layout/container.pyi
--rw-r--r--   0        0        0      715 2024-02-07 21:48:43.283082 reflex-0.5.0a2/reflex/components/chakra/layout/flex.py
--rw-r--r--   0        0        0     4138 2024-04-24 19:31:44.830583 reflex-0.5.0a2/reflex/components/chakra/layout/flex.pyi
--rw-r--r--   0        0        0     4318 2024-02-07 21:48:43.283328 reflex-0.5.0a2/reflex/components/chakra/layout/grid.py
--rw-r--r--   0        0        0    13853 2024-04-24 19:31:41.333938 reflex-0.5.0a2/reflex/components/chakra/layout/grid.pyi
--rw-r--r--   0        0        0      179 2024-02-07 21:48:43.283579 reflex-0.5.0a2/reflex/components/chakra/layout/spacer.py
--rw-r--r--   0        0        0     3230 2024-04-24 19:31:48.988499 reflex-0.5.0a2/reflex/components/chakra/layout/spacer.pyi
--rw-r--r--   0        0        0     1077 2024-02-07 21:48:43.283791 reflex-0.5.0a2/reflex/components/chakra/layout/stack.py
--rw-r--r--   0        0        0    12219 2024-04-24 19:31:34.279618 reflex-0.5.0a2/reflex/components/chakra/layout/stack.pyi
--rw-r--r--   0        0        0     1463 2024-02-07 21:48:43.284089 reflex-0.5.0a2/reflex/components/chakra/layout/wrap.py
--rw-r--r--   0        0        0     6943 2024-04-24 19:31:33.351664 reflex-0.5.0a2/reflex/components/chakra/layout/wrap.pyi
--rw-r--r--   0        0        0      190 2024-02-06 00:51:31.985088 reflex-0.5.0a2/reflex/components/chakra/media/__init__.py
--rw-r--r--   0        0        0     1668 2024-02-07 21:48:43.284332 reflex-0.5.0a2/reflex/components/chakra/media/avatar.py
--rw-r--r--   0        0        0    10445 2024-04-24 19:31:27.389378 reflex-0.5.0a2/reflex/components/chakra/media/avatar.pyi
--rw-r--r--   0        0        0     2462 2024-04-24 21:16:40.836689 reflex-0.5.0a2/reflex/components/chakra/media/icon.py
--rw-r--r--   0        0        0     6271 2024-04-24 19:31:19.854478 reflex-0.5.0a2/reflex/components/chakra/media/icon.pyi
--rw-r--r--   0        0        0     2400 2024-02-07 21:48:43.284781 reflex-0.5.0a2/reflex/components/chakra/media/image.py
--rw-r--r--   0        0        0     5423 2024-04-24 19:31:52.691354 reflex-0.5.0a2/reflex/components/chakra/media/image.pyi
--rw-r--r--   0        0        0      419 2024-02-06 00:51:31.986093 reflex-0.5.0a2/reflex/components/chakra/navigation/__init__.py
--rw-r--r--   0        0        0     2925 2024-02-07 21:48:43.285023 reflex-0.5.0a2/reflex/components/chakra/navigation/breadcrumb.py
--rw-r--r--   0        0        0    13575 2024-04-24 19:32:01.936776 reflex-0.5.0a2/reflex/components/chakra/navigation/breadcrumb.pyi
--rw-r--r--   0        0        0     1475 2024-02-06 00:51:31.986318 reflex-0.5.0a2/reflex/components/chakra/navigation/link.py
--rw-r--r--   0        0        0     3999 2024-04-24 19:31:19.850596 reflex-0.5.0a2/reflex/components/chakra/navigation/link.pyi
--rw-r--r--   0        0        0      521 2024-02-06 00:51:31.986581 reflex-0.5.0a2/reflex/components/chakra/navigation/linkoverlay.py
--rw-r--r--   0        0        0     6233 2024-04-24 19:31:59.056993 reflex-0.5.0a2/reflex/components/chakra/navigation/linkoverlay.pyi
--rw-r--r--   0        0        0     2935 2024-02-07 21:48:43.285634 reflex-0.5.0a2/reflex/components/chakra/navigation/stepper.py
--rw-r--r--   0        0        0    27922 2024-04-24 19:31:59.991438 reflex-0.5.0a2/reflex/components/chakra/navigation/stepper.pyi
--rw-r--r--   0        0        0      850 2024-02-06 00:51:31.987014 reflex-0.5.0a2/reflex/components/chakra/overlay/__init__.py
--rw-r--r--   0        0        0     5200 2024-02-07 21:48:43.285952 reflex-0.5.0a2/reflex/components/chakra/overlay/alertdialog.py
--rw-r--r--   0        0        0    23985 2024-04-24 19:31:53.441920 reflex-0.5.0a2/reflex/components/chakra/overlay/alertdialog.pyi
--rw-r--r--   0        0        0     5186 2024-02-06 00:51:31.987467 reflex-0.5.0a2/reflex/components/chakra/overlay/drawer.py
--rw-r--r--   0        0        0    25406 2024-04-24 19:32:02.090146 reflex-0.5.0a2/reflex/components/chakra/overlay/drawer.pyi
--rw-r--r--   0        0        0     6974 2024-02-07 21:48:43.286352 reflex-0.5.0a2/reflex/components/chakra/overlay/menu.py
--rw-r--r--   0        0        0    28682 2024-04-24 19:32:03.285218 reflex-0.5.0a2/reflex/components/chakra/overlay/menu.pyi
--rw-r--r--   0        0        0     5270 2024-02-07 21:48:43.286588 reflex-0.5.0a2/reflex/components/chakra/overlay/modal.py
--rw-r--r--   0        0        0    23549 2024-04-24 19:32:01.507839 reflex-0.5.0a2/reflex/components/chakra/overlay/modal.pyi
--rw-r--r--   0        0        0     5967 2024-02-07 21:48:43.286836 reflex-0.5.0a2/reflex/components/chakra/overlay/popover.py
--rw-r--r--   0        0        0    29893 2024-04-24 19:32:01.594206 reflex-0.5.0a2/reflex/components/chakra/overlay/popover.pyi
--rw-r--r--   0        0        0     2127 2024-02-07 21:48:43.287207 reflex-0.5.0a2/reflex/components/chakra/overlay/tooltip.py
--rw-r--r--   0        0        0     6060 2024-04-24 19:31:15.213215 reflex-0.5.0a2/reflex/components/chakra/overlay/tooltip.pyi
--rw-r--r--   0        0        0      271 2024-02-06 00:51:31.988661 reflex-0.5.0a2/reflex/components/chakra/typography/__init__.py
--rw-r--r--   0        0        0      379 2024-02-07 21:48:43.287449 reflex-0.5.0a2/reflex/components/chakra/typography/heading.py
--rw-r--r--   0        0        0     3706 2024-04-24 19:31:17.288584 reflex-0.5.0a2/reflex/components/chakra/typography/heading.pyi
--rw-r--r--   0        0        0      671 2024-02-07 21:48:43.287662 reflex-0.5.0a2/reflex/components/chakra/typography/highlight.py
--rw-r--r--   0        0        0     3645 2024-04-24 19:31:37.053293 reflex-0.5.0a2/reflex/components/chakra/typography/highlight.pyi
--rw-r--r--   0        0        0      328 2024-02-07 21:48:43.287874 reflex-0.5.0a2/reflex/components/chakra/typography/span.py
--rw-r--r--   0        0        0     3372 2024-04-24 19:31:23.281815 reflex-0.5.0a2/reflex/components/chakra/typography/span.pyi
--rw-r--r--   0        0        0      472 2024-02-07 21:48:43.288076 reflex-0.5.0a2/reflex/components/chakra/typography/text.py
--rw-r--r--   0        0        0     3596 2024-04-24 19:31:50.785304 reflex-0.5.0a2/reflex/components/chakra/typography/text.pyi
--rw-r--r--   0        0        0    75744 2024-05-11 03:29:42.708073 reflex-0.5.0a2/reflex/components/component.py
--rw-r--r--   0        0        0      857 2024-04-25 16:52:48.840950 reflex-0.5.0a2/reflex/components/core/__init__.py
--rw-r--r--   0        0        0     5943 2024-04-04 14:57:26.386161 reflex-0.5.0a2/reflex/components/core/banner.py
--rw-r--r--   0        0        0    17164 2024-04-24 19:32:01.784962 reflex-0.5.0a2/reflex/components/core/banner.pyi
--rw-r--r--   0        0        0     1873 2024-02-06 00:51:31.991625 reflex-0.5.0a2/reflex/components/core/client_side_routing.py
--rw-r--r--   0        0        0     6264 2024-04-24 19:31:22.918462 reflex-0.5.0a2/reflex/components/core/client_side_routing.pyi
--rw-r--r--   0        0        0      590 2024-02-17 20:02:02.417474 reflex-0.5.0a2/reflex/components/core/colors.py
--rw-r--r--   0        0        0     6005 2024-05-07 15:33:05.683015 reflex-0.5.0a2/reflex/components/core/cond.py
--rw-r--r--   0        0        0     4888 2024-05-09 00:05:27.335942 reflex-0.5.0a2/reflex/components/core/debounce.py
--rw-r--r--   0        0        0     4216 2024-04-25 16:52:48.841425 reflex-0.5.0a2/reflex/components/core/debounce.pyi
--rw-r--r--   0        0        0     4334 2024-05-11 03:29:42.708393 reflex-0.5.0a2/reflex/components/core/foreach.py
--rw-r--r--   0        0        0     1284 2024-05-05 01:15:24.054752 reflex-0.5.0a2/reflex/components/core/html.py
--rw-r--r--   0        0        0     6616 2024-04-25 05:29:57.085054 reflex-0.5.0a2/reflex/components/core/html.pyi
--rw-r--r--   0        0        0       30 2024-02-07 21:48:43.290204 reflex-0.5.0a2/reflex/components/core/layout/__init__.py
--rw-r--r--   0        0        0     9484 2024-05-07 15:33:05.683232 reflex-0.5.0a2/reflex/components/core/match.py
--rw-r--r--   0        0        0     1907 2024-04-04 14:19:59.331992 reflex-0.5.0a2/reflex/components/core/responsive.py
--rw-r--r--   0        0        0    10193 2024-05-05 01:15:24.055101 reflex-0.5.0a2/reflex/components/core/upload.py
--rw-r--r--   0        0        0    17147 2024-04-25 16:52:48.841883 reflex-0.5.0a2/reflex/components/core/upload.pyi
--rw-r--r--   0        0        0      357 2024-04-05 17:14:14.460655 reflex-0.5.0a2/reflex/components/datadisplay/__init__.py
--rw-r--r--   0        0        0    11363 2024-05-07 15:33:05.683354 reflex-0.5.0a2/reflex/components/datadisplay/code.py
--rw-r--r--   0        0        0    31213 2024-05-07 15:33:05.683489 reflex-0.5.0a2/reflex/components/datadisplay/code.pyi
--rw-r--r--   0        0        0    12632 2024-02-06 00:51:31.995005 reflex-0.5.0a2/reflex/components/datadisplay/dataeditor.py
--rw-r--r--   0        0        0    10485 2024-04-24 19:31:43.237754 reflex-0.5.0a2/reflex/components/datadisplay/dataeditor.pyi
--rw-r--r--   0        0        0     2562 2024-04-05 17:14:14.460754 reflex-0.5.0a2/reflex/components/datadisplay/logo.py
--rw-r--r--   0        0        0       73 2023-11-26 20:56:44.132351 reflex-0.5.0a2/reflex/components/el/__init__.py
--rw-r--r--   0        0        0      113 2023-11-26 20:56:44.132431 reflex-0.5.0a2/reflex/components/el/constants/__init__.py
--rw-r--r--   0        0        0     7175 2023-11-26 20:56:44.132596 reflex-0.5.0a2/reflex/components/el/constants/html.py
--rw-r--r--   0        0        0    15554 2023-11-26 20:56:44.132713 reflex-0.5.0a2/reflex/components/el/constants/react.py
--rw-r--r--   0        0        0     1713 2023-11-26 20:56:44.132789 reflex-0.5.0a2/reflex/components/el/constants/reflex.py
--rw-r--r--   0        0        0      494 2023-12-01 04:51:31.098496 reflex-0.5.0a2/reflex/components/el/element.py
--rw-r--r--   0        0        0     3213 2024-04-24 19:32:01.854505 reflex-0.5.0a2/reflex/components/el/element.pyi
--rw-r--r--   0        0        0     3529 2024-03-20 23:54:55.843475 reflex-0.5.0a2/reflex/components/el/elements/__init__.py
--rw-r--r--   0        0        0     1982 2024-02-17 20:02:02.419390 reflex-0.5.0a2/reflex/components/el/elements/base.py
--rw-r--r--   0        0        0     6340 2024-04-24 19:31:34.952107 reflex-0.5.0a2/reflex/components/el/elements/base.pyi
--rw-r--r--   0        0        0    20103 2024-04-25 16:52:48.842221 reflex-0.5.0a2/reflex/components/el/elements/forms.py
--rw-r--r--   0        0        0    99555 2024-04-25 16:52:48.842962 reflex-0.5.0a2/reflex/components/el/elements/forms.pyi
--rw-r--r--   0        0        0     3610 2024-02-06 00:51:31.998070 reflex-0.5.0a2/reflex/components/el/elements/inline.py
--rw-r--r--   0        0        0   164607 2024-04-24 19:32:05.408521 reflex-0.5.0a2/reflex/components/el/elements/inline.pyi
--rw-r--r--   0        0        0     7929 2024-03-20 23:54:55.844702 reflex-0.5.0a2/reflex/components/el/elements/media.py
--rw-r--r--   0        0        0    93567 2024-04-24 19:32:03.850879 reflex-0.5.0a2/reflex/components/el/elements/media.pyi
--rw-r--r--   0        0        0     1337 2023-11-26 20:56:44.134404 reflex-0.5.0a2/reflex/components/el/elements/metadata.py
--rw-r--r--   0        0        0    28031 2024-04-24 19:32:01.554937 reflex-0.5.0a2/reflex/components/el/elements/metadata.pyi
--rw-r--r--   0        0        0     1569 2023-11-26 20:56:44.134590 reflex-0.5.0a2/reflex/components/el/elements/other.py
--rw-r--r--   0        0        0    42033 2024-04-24 19:31:59.581160 reflex-0.5.0a2/reflex/components/el/elements/other.pyi
--rw-r--r--   0        0        0     1406 2024-02-17 20:02:02.421306 reflex-0.5.0a2/reflex/components/el/elements/scripts.py
--rw-r--r--   0        0        0    19615 2024-04-24 19:31:22.715670 reflex-0.5.0a2/reflex/components/el/elements/scripts.pyi
--rw-r--r--   0        0        0     1535 2024-02-17 20:02:02.421507 reflex-0.5.0a2/reflex/components/el/elements/sectioning.py
--rw-r--r--   0        0        0    87242 2024-04-24 19:32:04.046011 reflex-0.5.0a2/reflex/components/el/elements/sectioning.pyi
--rw-r--r--   0        0        0     2767 2024-02-17 20:02:02.421759 reflex-0.5.0a2/reflex/components/el/elements/tables.py
--rw-r--r--   0        0        0    61849 2024-04-24 19:32:03.007985 reflex-0.5.0a2/reflex/components/el/elements/tables.pyi
--rw-r--r--   0        0        0     2432 2024-02-17 20:02:02.421997 reflex-0.5.0a2/reflex/components/el/elements/typography.py
--rw-r--r--   0        0        0    89115 2024-04-24 19:32:04.312119 reflex-0.5.0a2/reflex/components/el/elements/typography.pyi
--rw-r--r--   0        0        0       88 2024-02-06 00:51:31.999860 reflex-0.5.0a2/reflex/components/gridjs/__init__.py
--rw-r--r--   0        0        0     4300 2024-02-06 00:51:32.000048 reflex-0.5.0a2/reflex/components/gridjs/datatable.py
--rw-r--r--   0        0        0     7053 2024-04-24 19:31:36.593992 reflex-0.5.0a2/reflex/components/gridjs/datatable.pyi
--rw-r--r--   0        0        0      501 2024-02-06 00:51:32.000350 reflex-0.5.0a2/reflex/components/literals.py
--rw-r--r--   0        0        0       73 2024-02-07 21:48:43.293647 reflex-0.5.0a2/reflex/components/lucide/__init__.py
--rw-r--r--   0        0        0    34077 2024-05-09 00:05:27.336308 reflex-0.5.0a2/reflex/components/lucide/icon.py
--rw-r--r--   0        0        0    37918 2024-05-05 01:15:24.056110 reflex-0.5.0a2/reflex/components/lucide/icon.pyi
--rw-r--r--   0        0        0       87 2024-02-06 00:51:32.000748 reflex-0.5.0a2/reflex/components/markdown/__init__.py
--rw-r--r--   0        0        0    10867 2024-05-09 00:05:27.336466 reflex-0.5.0a2/reflex/components/markdown/markdown.py
--rw-r--r--   0        0        0     5100 2024-05-09 00:05:27.336616 reflex-0.5.0a2/reflex/components/markdown/markdown.pyi
--rw-r--r--   0        0        0       44 2024-02-06 00:51:32.001397 reflex-0.5.0a2/reflex/components/media/__init__.py
--rw-r--r--   0        0        0      102 2024-02-06 00:51:32.001492 reflex-0.5.0a2/reflex/components/media/icon.py
--rw-r--r--   0        0        0       79 2024-02-06 00:51:32.001557 reflex-0.5.0a2/reflex/components/moment/__init__.py
--rw-r--r--   0        0        0     3925 2024-02-06 00:51:32.001623 reflex-0.5.0a2/reflex/components/moment/moment.py
--rw-r--r--   0        0        0     6870 2024-04-24 19:31:51.190910 reflex-0.5.0a2/reflex/components/moment/moment.pyi
--rw-r--r--   0        0        0      239 2024-02-06 00:51:32.001924 reflex-0.5.0a2/reflex/components/next/__init__.py
--rw-r--r--   0        0        0      189 2024-01-08 22:19:50.677879 reflex-0.5.0a2/reflex/components/next/base.py
--rw-r--r--   0        0        0     3233 2024-04-24 19:31:43.822514 reflex-0.5.0a2/reflex/components/next/base.pyi
--rw-r--r--   0        0        0     3831 2024-01-08 22:19:50.678013 reflex-0.5.0a2/reflex/components/next/image.py
--rw-r--r--   0        0        0     5795 2024-04-24 19:31:33.244479 reflex-0.5.0a2/reflex/components/next/image.pyi
--rw-r--r--   0        0        0      503 2024-02-06 00:51:32.002304 reflex-0.5.0a2/reflex/components/next/link.py
--rw-r--r--   0        0        0     3461 2024-04-24 19:31:15.603661 reflex-0.5.0a2/reflex/components/next/link.pyi
--rw-r--r--   0        0        0      730 2024-01-08 22:19:50.678316 reflex-0.5.0a2/reflex/components/next/video.py
--rw-r--r--   0        0        0     3429 2024-04-24 19:31:46.249185 reflex-0.5.0a2/reflex/components/next/video.pyi
--rw-r--r--   0        0        0       77 2024-02-06 00:51:32.002529 reflex-0.5.0a2/reflex/components/plotly/__init__.py
--rw-r--r--   0        0        0      964 2024-03-20 23:54:55.846069 reflex-0.5.0a2/reflex/components/plotly/plotly.py
--rw-r--r--   0        0        0     6865 2024-04-24 19:31:24.224015 reflex-0.5.0a2/reflex/components/plotly/plotly.pyi
--rw-r--r--   0        0        0      112 2024-02-17 20:02:02.423429 reflex-0.5.0a2/reflex/components/radix/__init__.py
--rw-r--r--   0        0        0      214 2024-02-17 20:02:02.423526 reflex-0.5.0a2/reflex/components/radix/primitives/__init__.py
--rw-r--r--   0        0        0    16247 2024-05-11 03:29:42.708577 reflex-0.5.0a2/reflex/components/radix/primitives/accordion.py
--rw-r--r--   0        0        0    37999 2024-05-11 03:29:42.708959 reflex-0.5.0a2/reflex/components/radix/primitives/accordion.pyi
--rw-r--r--   0        0        0      869 2024-02-06 00:51:32.004050 reflex-0.5.0a2/reflex/components/radix/primitives/base.py
--rw-r--r--   0        0        0     6478 2024-04-24 19:31:44.069976 reflex-0.5.0a2/reflex/components/radix/primitives/base.pyi
--rw-r--r--   0        0        0     8660 2024-03-20 23:54:55.846917 reflex-0.5.0a2/reflex/components/radix/primitives/drawer.py
--rw-r--r--   0        0        0    34484 2024-04-24 19:32:02.551316 reflex-0.5.0a2/reflex/components/radix/primitives/drawer.pyi
--rw-r--r--   0        0        0     4964 2024-05-11 03:29:42.709212 reflex-0.5.0a2/reflex/components/radix/primitives/form.py
--rw-r--r--   0        0        0    48138 2024-05-07 15:33:05.684481 reflex-0.5.0a2/reflex/components/radix/primitives/form.pyi
--rw-r--r--   0        0        0     4160 2024-05-07 15:33:05.684814 reflex-0.5.0a2/reflex/components/radix/primitives/progress.py
--rw-r--r--   0        0        0    22874 2024-05-07 15:33:05.685122 reflex-0.5.0a2/reflex/components/radix/primitives/progress.pyi
--rw-r--r--   0        0        0     5198 2024-05-07 15:33:05.685275 reflex-0.5.0a2/reflex/components/radix/primitives/slider.py
--rw-r--r--   0        0        0    16877 2024-05-07 15:33:05.685394 reflex-0.5.0a2/reflex/components/radix/primitives/slider.pyi
--rw-r--r--   0        0        0      292 2024-02-17 20:02:02.426799 reflex-0.5.0a2/reflex/components/radix/themes/__init__.py
--rw-r--r--   0        0        0     8294 2024-04-26 18:47:21.875701 reflex-0.5.0a2/reflex/components/radix/themes/base.py
--rw-r--r--   0        0        0    26971 2024-05-05 01:15:24.056523 reflex-0.5.0a2/reflex/components/radix/themes/base.pyi
--rw-r--r--   0        0        0     4819 2024-05-05 01:15:24.056812 reflex-0.5.0a2/reflex/components/radix/themes/color_mode.py
--rw-r--r--   0        0        0    15461 2024-05-05 01:15:24.056928 reflex-0.5.0a2/reflex/components/radix/themes/color_mode.pyi
--rw-r--r--   0        0        0     2440 2024-05-09 00:05:27.336999 reflex-0.5.0a2/reflex/components/radix/themes/components/__init__.py
--rw-r--r--   0        0        0     3267 2024-03-20 23:54:55.849529 reflex-0.5.0a2/reflex/components/radix/themes/components/alert_dialog.py
--rw-r--r--   0        0        0    24434 2024-04-24 19:31:57.706076 reflex-0.5.0a2/reflex/components/radix/themes/components/alert_dialog.pyi
--rw-r--r--   0        0        0      400 2024-02-17 20:02:02.428862 reflex-0.5.0a2/reflex/components/radix/themes/components/aspect_ratio.py
--rw-r--r--   0        0        0     3640 2024-04-24 19:31:17.911074 reflex-0.5.0a2/reflex/components/radix/themes/components/aspect_ratio.pyi
--rw-r--r--   0        0        0      989 2024-03-20 23:54:55.849841 reflex-0.5.0a2/reflex/components/radix/themes/components/avatar.py
--rw-r--r--   0        0        0     6562 2024-04-24 19:31:52.410239 reflex-0.5.0a2/reflex/components/radix/themes/components/avatar.pyi
--rw-r--r--   0        0        0      821 2024-04-26 18:47:21.876311 reflex-0.5.0a2/reflex/components/radix/themes/components/badge.py
--rw-r--r--   0        0        0     9347 2024-04-26 18:47:21.876509 reflex-0.5.0a2/reflex/components/radix/themes/components/badge.pyi
--rw-r--r--   0        0        0     1125 2024-04-26 18:47:21.876620 reflex-0.5.0a2/reflex/components/radix/themes/components/button.py
--rw-r--r--   0        0        0    11939 2024-04-26 18:47:21.876761 reflex-0.5.0a2/reflex/components/radix/themes/components/button.pyi
--rw-r--r--   0        0        0     2378 2024-03-20 23:54:55.850376 reflex-0.5.0a2/reflex/components/radix/themes/components/callout.py
--rw-r--r--   0        0        0    38710 2024-04-24 19:32:02.594947 reflex-0.5.0a2/reflex/components/radix/themes/components/callout.pyi
--rw-r--r--   0        0        0      659 2024-02-17 20:02:02.430724 reflex-0.5.0a2/reflex/components/radix/themes/components/card.py
--rw-r--r--   0        0        0     7200 2024-04-24 19:31:48.002992 reflex-0.5.0a2/reflex/components/radix/themes/components/card.pyi
--rw-r--r--   0        0        0     4679 2024-03-20 23:54:55.851297 reflex-0.5.0a2/reflex/components/radix/themes/components/checkbox.py
--rw-r--r--   0        0        0    20877 2024-04-24 19:32:01.819836 reflex-0.5.0a2/reflex/components/radix/themes/components/checkbox.pyi
--rw-r--r--   0        0        0     1301 2024-04-26 18:47:21.876837 reflex-0.5.0a2/reflex/components/radix/themes/components/checkbox_cards.py
--rw-r--r--   0        0        0     9591 2024-04-26 18:47:21.876955 reflex-0.5.0a2/reflex/components/radix/themes/components/checkbox_cards.pyi
--rw-r--r--   0        0        0     1024 2024-04-26 18:47:21.877018 reflex-0.5.0a2/reflex/components/radix/themes/components/checkbox_group.py
--rw-r--r--   0        0        0     9012 2024-04-26 18:47:21.877125 reflex-0.5.0a2/reflex/components/radix/themes/components/checkbox_group.pyi
--rw-r--r--   0        0        0     5049 2024-03-20 23:54:55.852012 reflex-0.5.0a2/reflex/components/radix/themes/components/context_menu.py
--rw-r--r--   0        0        0    31192 2024-04-24 19:32:03.158519 reflex-0.5.0a2/reflex/components/radix/themes/components/context_menu.pyi
--rw-r--r--   0        0        0     1508 2024-04-26 18:47:21.877372 reflex-0.5.0a2/reflex/components/radix/themes/components/data_list.py
--rw-r--r--   0        0        0    15403 2024-04-26 18:47:21.877634 reflex-0.5.0a2/reflex/components/radix/themes/components/data_list.pyi
--rw-r--r--   0        0        0     2600 2024-03-20 23:54:55.852519 reflex-0.5.0a2/reflex/components/radix/themes/components/dialog.py
--rw-r--r--   0        0        0    24895 2024-04-24 19:32:02.097223 reflex-0.5.0a2/reflex/components/radix/themes/components/dialog.pyi
--rw-r--r--   0        0        0    11256 2024-03-20 23:54:55.852973 reflex-0.5.0a2/reflex/components/radix/themes/components/dropdown_menu.py
--rw-r--r--   0        0        0    37901 2024-04-24 19:32:02.303816 reflex-0.5.0a2/reflex/components/radix/themes/components/dropdown_menu.pyi
--rw-r--r--   0        0        0     2405 2024-03-20 23:54:55.853285 reflex-0.5.0a2/reflex/components/radix/themes/components/hover_card.py
--rw-r--r--   0        0        0    17744 2024-04-24 19:31:56.396802 reflex-0.5.0a2/reflex/components/radix/themes/components/hover_card.pyi
--rw-r--r--   0        0        0     2940 2024-05-09 00:05:27.337231 reflex-0.5.0a2/reflex/components/radix/themes/components/icon_button.py
--rw-r--r--   0        0        0    12126 2024-05-07 15:33:05.685671 reflex-0.5.0a2/reflex/components/radix/themes/components/icon_button.pyi
--rw-r--r--   0        0        0     1015 2024-03-20 23:54:55.853906 reflex-0.5.0a2/reflex/components/radix/themes/components/inset.py
--rw-r--r--   0        0        0     7889 2024-04-24 19:31:39.003439 reflex-0.5.0a2/reflex/components/radix/themes/components/inset.pyi
--rw-r--r--   0        0        0     3177 2024-03-20 23:54:55.854041 reflex-0.5.0a2/reflex/components/radix/themes/components/popover.py
--rw-r--r--   0        0        0    17404 2024-04-24 19:32:01.605821 reflex-0.5.0a2/reflex/components/radix/themes/components/popover.pyi
--rw-r--r--   0        0        0     1598 2024-05-09 00:05:27.337432 reflex-0.5.0a2/reflex/components/radix/themes/components/progress.py
--rw-r--r--   0        0        0     6676 2024-05-09 00:05:27.337586 reflex-0.5.0a2/reflex/components/radix/themes/components/progress.pyi
--rw-r--r--   0        0        0      762 2024-04-26 18:47:21.878308 reflex-0.5.0a2/reflex/components/radix/themes/components/radio.py
--rw-r--r--   0        0        0     5924 2024-04-26 18:47:21.878424 reflex-0.5.0a2/reflex/components/radix/themes/components/radio.pyi
--rw-r--r--   0        0        0     1250 2024-04-26 18:47:21.878499 reflex-0.5.0a2/reflex/components/radix/themes/components/radio_cards.py
--rw-r--r--   0        0        0     9561 2024-04-26 18:47:21.878615 reflex-0.5.0a2/reflex/components/radix/themes/components/radio_cards.pyi
--rw-r--r--   0        0        0     6233 2024-04-24 21:16:40.838796 reflex-0.5.0a2/reflex/components/radix/themes/components/radio_group.py
--rw-r--r--   0        0        0    24106 2024-04-24 19:32:02.212695 reflex-0.5.0a2/reflex/components/radix/themes/components/radio_group.pyi
--rw-r--r--   0        0        0      920 2024-03-20 23:54:55.855386 reflex-0.5.0a2/reflex/components/radix/themes/components/scroll_area.py
--rw-r--r--   0        0        0     4427 2024-04-24 19:31:54.699499 reflex-0.5.0a2/reflex/components/radix/themes/components/scroll_area.pyi
--rw-r--r--   0        0        0     1292 2024-04-26 18:47:21.878708 reflex-0.5.0a2/reflex/components/radix/themes/components/segmented_control.py
--rw-r--r--   0        0        0     9507 2024-04-26 18:47:21.878829 reflex-0.5.0a2/reflex/components/radix/themes/components/segmented_control.pyi
--rw-r--r--   0        0        0     8028 2024-04-05 17:14:14.462095 reflex-0.5.0a2/reflex/components/radix/themes/components/select.py
--rw-r--r--   0        0        0    45123 2024-04-24 19:32:01.973018 reflex-0.5.0a2/reflex/components/radix/themes/components/select.pyi
--rw-r--r--   0        0        0      868 2024-03-20 23:54:55.856979 reflex-0.5.0a2/reflex/components/radix/themes/components/separator.py
--rw-r--r--   0        0        0     6078 2024-04-24 19:32:00.501335 reflex-0.5.0a2/reflex/components/radix/themes/components/separator.pyi
--rw-r--r--   0        0        0      643 2024-04-26 18:47:21.878906 reflex-0.5.0a2/reflex/components/radix/themes/components/skeleton.py
--rw-r--r--   0        0        0     4289 2024-04-26 18:47:21.879004 reflex-0.5.0a2/reflex/components/radix/themes/components/skeleton.pyi
--rw-r--r--   0        0        0     3234 2024-03-20 23:54:55.857144 reflex-0.5.0a2/reflex/components/radix/themes/components/slider.py
--rw-r--r--   0        0        0     8162 2024-04-24 19:31:52.441948 reflex-0.5.0a2/reflex/components/radix/themes/components/slider.pyi
--rw-r--r--   0        0        0      431 2024-04-26 18:47:21.879090 reflex-0.5.0a2/reflex/components/radix/themes/components/spinner.py
--rw-r--r--   0        0        0     3845 2024-04-26 18:47:21.879165 reflex-0.5.0a2/reflex/components/radix/themes/components/spinner.pyi
--rw-r--r--   0        0        0     1976 2024-02-17 20:02:02.440152 reflex-0.5.0a2/reflex/components/radix/themes/components/switch.py
--rw-r--r--   0        0        0     7404 2024-04-24 19:31:46.185370 reflex-0.5.0a2/reflex/components/radix/themes/components/switch.pyi
--rw-r--r--   0        0        0     3111 2024-03-20 23:54:55.857388 reflex-0.5.0a2/reflex/components/radix/themes/components/table.py
--rw-r--r--   0        0        0    47387 2024-04-24 19:32:03.411460 reflex-0.5.0a2/reflex/components/radix/themes/components/table.pyi
--rw-r--r--   0        0        0     2986 2024-05-07 15:33:05.685861 reflex-0.5.0a2/reflex/components/radix/themes/components/tabs.py
--rw-r--r--   0        0        0    19119 2024-05-07 15:33:05.685968 reflex-0.5.0a2/reflex/components/radix/themes/components/tabs.pyi
--rw-r--r--   0        0        0     3233 2024-02-17 20:02:02.441460 reflex-0.5.0a2/reflex/components/radix/themes/components/text_area.py
--rw-r--r--   0        0        0    11711 2024-04-24 19:31:45.665204 reflex-0.5.0a2/reflex/components/radix/themes/components/text_area.pyi
--rw-r--r--   0        0        0     6527 2024-05-09 00:05:27.337867 reflex-0.5.0a2/reflex/components/radix/themes/components/text_field.py
--rw-r--r--   0        0        0    26637 2024-05-09 00:05:27.338008 reflex-0.5.0a2/reflex/components/radix/themes/components/text_field.pyi
--rw-r--r--   0        0        0     4465 2024-02-17 20:02:02.442324 reflex-0.5.0a2/reflex/components/radix/themes/components/tooltip.py
--rw-r--r--   0        0        0     8092 2024-04-24 19:31:32.491941 reflex-0.5.0a2/reflex/components/radix/themes/components/tooltip.pyi
--rw-r--r--   0        0        0      811 2024-04-04 14:19:59.340548 reflex-0.5.0a2/reflex/components/radix/themes/layout/__init__.py
--rw-r--r--   0        0        0     1211 2024-04-26 18:47:21.880131 reflex-0.5.0a2/reflex/components/radix/themes/layout/base.py
--rw-r--r--   0        0        0     7663 2024-04-26 18:47:21.880279 reflex-0.5.0a2/reflex/components/radix/themes/layout/base.pyi
--rw-r--r--   0        0        0      281 2024-02-07 21:48:43.318485 reflex-0.5.0a2/reflex/components/radix/themes/layout/box.py
--rw-r--r--   0        0        0     6462 2024-04-24 19:31:52.197501 reflex-0.5.0a2/reflex/components/radix/themes/layout/box.pyi
--rw-r--r--   0        0        0      509 2024-05-07 15:33:05.686074 reflex-0.5.0a2/reflex/components/radix/themes/layout/center.py
--rw-r--r--   0        0        0     8271 2024-05-07 15:33:05.686180 reflex-0.5.0a2/reflex/components/radix/themes/layout/center.pyi
--rw-r--r--   0        0        0     1405 2024-05-05 01:15:24.057627 reflex-0.5.0a2/reflex/components/radix/themes/layout/container.py
--rw-r--r--   0        0        0     5247 2024-05-05 01:15:24.057873 reflex-0.5.0a2/reflex/components/radix/themes/layout/container.pyi
--rw-r--r--   0        0        0     1374 2024-03-20 23:54:55.859776 reflex-0.5.0a2/reflex/components/radix/themes/layout/flex.py
--rw-r--r--   0        0        0     8501 2024-04-24 19:31:47.609497 reflex-0.5.0a2/reflex/components/radix/themes/layout/flex.pyi
--rw-r--r--   0        0        0     1498 2024-03-20 23:54:55.860131 reflex-0.5.0a2/reflex/components/radix/themes/layout/grid.py
--rw-r--r--   0        0        0     8907 2024-04-24 19:31:44.336304 reflex-0.5.0a2/reflex/components/radix/themes/layout/grid.pyi
--rw-r--r--   0        0        0     4991 2024-05-07 15:33:05.686298 reflex-0.5.0a2/reflex/components/radix/themes/layout/list.py
--rw-r--r--   0        0        0    28927 2024-05-07 15:33:05.686398 reflex-0.5.0a2/reflex/components/radix/themes/layout/list.pyi
--rw-r--r--   0        0        0      458 2024-02-07 21:48:43.320250 reflex-0.5.0a2/reflex/components/radix/themes/layout/section.py
--rw-r--r--   0        0        0     6758 2024-04-24 19:31:48.032806 reflex-0.5.0a2/reflex/components/radix/themes/layout/section.pyi
--rw-r--r--   0        0        0      492 2024-05-07 15:33:05.686501 reflex-0.5.0a2/reflex/components/radix/themes/layout/spacer.py
--rw-r--r--   0        0        0     8271 2024-05-07 15:33:05.686608 reflex-0.5.0a2/reflex/components/radix/themes/layout/spacer.pyi
--rw-r--r--   0        0        0     1522 2024-05-05 01:15:24.058360 reflex-0.5.0a2/reflex/components/radix/themes/layout/stack.py
--rw-r--r--   0        0        0    22132 2024-05-05 01:15:24.058618 reflex-0.5.0a2/reflex/components/radix/themes/layout/stack.pyi
--rw-r--r--   0        0        0      343 2024-02-17 20:02:02.446123 reflex-0.5.0a2/reflex/components/radix/themes/typography/__init__.py
--rw-r--r--   0        0        0      408 2024-01-08 22:19:50.686081 reflex-0.5.0a2/reflex/components/radix/themes/typography/base.py
--rw-r--r--   0        0        0      799 2024-02-07 21:48:43.321231 reflex-0.5.0a2/reflex/components/radix/themes/typography/blockquote.py
--rw-r--r--   0        0        0     9316 2024-04-24 19:31:18.815043 reflex-0.5.0a2/reflex/components/radix/themes/typography/blockquote.pyi
--rw-r--r--   0        0        0      909 2024-02-07 21:48:43.321463 reflex-0.5.0a2/reflex/components/radix/themes/typography/code.py
--rw-r--r--   0        0        0     9513 2024-04-24 19:31:42.716182 reflex-0.5.0a2/reflex/components/radix/themes/typography/code.pyi
--rw-r--r--   0        0        0     1324 2024-02-07 21:48:43.322172 reflex-0.5.0a2/reflex/components/radix/themes/typography/heading.py
--rw-r--r--   0        0        0    10106 2024-04-24 19:31:48.004994 reflex-0.5.0a2/reflex/components/radix/themes/typography/heading.pyi
--rw-r--r--   0        0        0     3291 2024-05-05 01:15:24.058911 reflex-0.5.0a2/reflex/components/radix/themes/typography/link.py
--rw-r--r--   0        0        0    12144 2024-05-05 01:15:24.059174 reflex-0.5.0a2/reflex/components/radix/themes/typography/link.pyi
--rw-r--r--   0        0        0     2604 2024-03-20 23:54:55.863112 reflex-0.5.0a2/reflex/components/radix/themes/typography/text.py
--rw-r--r--   0        0        0    57238 2024-04-24 19:32:03.568126 reflex-0.5.0a2/reflex/components/radix/themes/typography/text.pyi
--rw-r--r--   0        0        0      144 2024-02-06 00:51:32.026767 reflex-0.5.0a2/reflex/components/react_player/__init__.py
--rw-r--r--   0        0        0      185 2024-02-06 00:51:32.026827 reflex-0.5.0a2/reflex/components/react_player/audio.py
--rw-r--r--   0        0        0     4327 2024-04-24 19:31:20.559612 reflex-0.5.0a2/reflex/components/react_player/audio.pyi
--rw-r--r--   0        0        0     1087 2024-02-06 00:51:32.027069 reflex-0.5.0a2/reflex/components/react_player/react_player.py
--rw-r--r--   0        0        0     4354 2024-04-24 19:31:40.833679 reflex-0.5.0a2/reflex/components/react_player/react_player.pyi
--rw-r--r--   0        0        0      185 2024-02-06 00:51:32.027295 reflex-0.5.0a2/reflex/components/react_player/video.py
--rw-r--r--   0        0        0     4327 2024-04-24 19:31:23.657166 reflex-0.5.0a2/reflex/components/react_player/video.pyi
--rw-r--r--   0        0        0     2373 2024-02-06 00:51:32.027723 reflex-0.5.0a2/reflex/components/recharts/__init__.py
--rw-r--r--   0        0        0    19595 2024-02-06 00:51:32.027828 reflex-0.5.0a2/reflex/components/recharts/cartesian.py
--rw-r--r--   0        0        0    84151 2024-04-24 19:32:04.125732 reflex-0.5.0a2/reflex/components/recharts/cartesian.pyi
--rw-r--r--   0        0        0    18493 2024-02-06 00:51:32.028086 reflex-0.5.0a2/reflex/components/recharts/charts.py
--rw-r--r--   0        0        0    48757 2024-04-24 19:32:04.230664 reflex-0.5.0a2/reflex/components/recharts/charts.pyi
--rw-r--r--   0        0        0     5624 2024-04-25 02:07:40.442483 reflex-0.5.0a2/reflex/components/recharts/general.py
--rw-r--r--   0        0        0    22787 2024-04-24 19:31:57.383382 reflex-0.5.0a2/reflex/components/recharts/general.pyi
--rw-r--r--   0        0        0    10410 2024-02-06 00:51:32.028623 reflex-0.5.0a2/reflex/components/recharts/polar.py
--rw-r--r--   0        0        0    24326 2024-04-24 19:32:02.075893 reflex-0.5.0a2/reflex/components/recharts/polar.pyi
--rw-r--r--   0        0        0     2870 2024-02-06 00:51:32.028787 reflex-0.5.0a2/reflex/components/recharts/recharts.py
--rw-r--r--   0        0        0     8535 2024-04-24 19:31:59.348537 reflex-0.5.0a2/reflex/components/recharts/recharts.pyi
--rw-r--r--   0        0        0       68 2024-05-05 01:15:24.059268 reflex-0.5.0a2/reflex/components/sonner/__init__.py
--rw-r--r--   0        0        0     7638 2024-05-05 01:15:24.059336 reflex-0.5.0a2/reflex/components/sonner/toast.py
--rw-r--r--   0        0        0     7635 2024-05-05 01:15:24.059415 reflex-0.5.0a2/reflex/components/sonner/toast.pyi
--rw-r--r--   0        0        0      109 2024-02-06 00:51:32.028942 reflex-0.5.0a2/reflex/components/suneditor/__init__.py
--rw-r--r--   0        0        0     7360 2024-02-06 00:51:32.029131 reflex-0.5.0a2/reflex/components/suneditor/editor.py
--rw-r--r--   0        0        0    10330 2024-04-24 19:32:02.124688 reflex-0.5.0a2/reflex/components/suneditor/editor.pyi
--rw-r--r--   0        0        0      152 2024-02-06 00:51:32.029339 reflex-0.5.0a2/reflex/components/tags/__init__.py
--rw-r--r--   0        0        0      447 2023-07-20 22:42:41.717618 reflex-0.5.0a2/reflex/components/tags/cond_tag.py
--rw-r--r--   0        0        0     3927 2024-05-09 06:53:37.971823 reflex-0.5.0a2/reflex/components/tags/iter_tag.py
--rw-r--r--   0        0        0      387 2024-02-06 00:51:32.029522 reflex-0.5.0a2/reflex/components/tags/match_tag.py
--rw-r--r--   0        0        0     2778 2024-03-20 23:54:55.863973 reflex-0.5.0a2/reflex/components/tags/tag.py
--rw-r--r--   0        0        0      587 2023-07-20 22:42:41.717805 reflex-0.5.0a2/reflex/components/tags/tagless.py
--rw-r--r--   0        0        0    10673 2024-05-09 00:05:27.338296 reflex-0.5.0a2/reflex/config.py
--rw-r--r--   0        0        0     3318 2024-04-05 17:14:06.329003 reflex-0.5.0a2/reflex/config.pyi
--rw-r--r--   0        0        0     2036 2024-05-07 15:33:05.687073 reflex-0.5.0a2/reflex/constants/__init__.py
--rw-r--r--   0        0        0     5640 2024-05-07 15:33:05.687194 reflex-0.5.0a2/reflex/constants/base.py
--rw-r--r--   0        0        0     2980 2024-04-24 19:34:30.973419 reflex-0.5.0a2/reflex/constants/base.pyi
--rw-r--r--   0        0        0     1625 2024-05-07 15:33:05.687387 reflex-0.5.0a2/reflex/constants/colors.py
--rw-r--r--   0        0        0     4207 2024-04-12 01:14:12.277724 reflex-0.5.0a2/reflex/constants/compiler.py
--rw-r--r--   0        0        0     1331 2024-01-08 22:19:50.692361 reflex-0.5.0a2/reflex/constants/config.py
--rw-r--r--   0        0        0     1268 2024-03-20 23:54:55.865280 reflex-0.5.0a2/reflex/constants/custom_components.py
--rw-r--r--   0        0        0     2668 2024-03-20 00:01:07.211135 reflex-0.5.0a2/reflex/constants/event.py
--rw-r--r--   0        0        0     3419 2024-05-05 01:15:24.059627 reflex-0.5.0a2/reflex/constants/installer.py
--rw-r--r--   0        0        0     2144 2024-05-05 01:15:24.059871 reflex-0.5.0a2/reflex/constants/route.py
--rw-r--r--   0        0        0      636 2024-02-06 00:51:32.030238 reflex-0.5.0a2/reflex/constants/style.py
--rw-r--r--   0        0        0       36 2024-03-20 23:54:55.865552 reflex-0.5.0a2/reflex/custom_components/__init__.py
--rw-r--r--   0        0        0    32293 2024-05-05 01:15:24.060009 reflex-0.5.0a2/reflex/custom_components/custom_components.py
--rw-r--r--   0        0        0    27893 2024-05-05 01:15:24.060128 reflex-0.5.0a2/reflex/event.py
--rw-r--r--   0        0        0      608 2024-05-09 00:05:27.338786 reflex-0.5.0a2/reflex/experimental/__init__.py
--rw-r--r--   0        0        0     2196 2024-04-24 21:16:40.840090 reflex-0.5.0a2/reflex/experimental/hooks.py
--rw-r--r--   0        0        0     7234 2024-05-07 15:33:05.687514 reflex-0.5.0a2/reflex/experimental/layout.py
--rw-r--r--   0        0        0      281 2024-04-12 01:14:12.278217 reflex-0.5.0a2/reflex/experimental/misc.py
--rw-r--r--   0        0        0      111 2023-07-20 22:42:41.719277 reflex-0.5.0a2/reflex/middleware/__init__.py
--rw-r--r--   0        0        0     1484 2024-03-28 17:56:29.082526 reflex-0.5.0a2/reflex/middleware/hydrate_middleware.py
--rw-r--r--   0        0        0     1169 2023-12-01 04:51:31.116521 reflex-0.5.0a2/reflex/middleware/middleware.py
--rw-r--r--   0        0        0    13227 2024-05-09 00:05:27.338971 reflex-0.5.0a2/reflex/model.py
--rw-r--r--   0        0        0     2077 2024-04-24 21:16:40.840737 reflex-0.5.0a2/reflex/page.py
--rw-r--r--   0        0        0    17826 2024-05-05 01:15:24.060260 reflex-0.5.0a2/reflex/reflex.py
--rw-r--r--   0        0        0     4198 2024-05-05 01:15:24.060365 reflex-0.5.0a2/reflex/route.py
--rw-r--r--   0        0        0   105748 2024-05-09 00:05:27.339322 reflex-0.5.0a2/reflex/state.py
--rw-r--r--   0        0        0     9405 2024-05-11 03:29:42.709528 reflex-0.5.0a2/reflex/style.py
--rw-r--r--   0        0        0    30743 2024-05-07 15:33:05.688166 reflex-0.5.0a2/reflex/testing.py
--rw-r--r--   0        0        0       24 2023-11-09 03:24:59.510665 reflex-0.5.0a2/reflex/utils/__init__.py
--rw-r--r--   0        0        0     8573 2024-02-06 00:51:32.031946 reflex-0.5.0a2/reflex/utils/build.py
--rw-r--r--   0        0        0     1255 2024-04-12 01:14:12.279414 reflex-0.5.0a2/reflex/utils/compat.py
--rw-r--r--   0        0        0     5182 2024-04-24 21:16:40.841356 reflex-0.5.0a2/reflex/utils/console.py
--rw-r--r--   0        0        0      504 2024-02-06 00:51:32.032065 reflex-0.5.0a2/reflex/utils/exceptions.py
--rw-r--r--   0        0        0    10406 2024-05-07 15:33:05.688300 reflex-0.5.0a2/reflex/utils/exec.py
--rw-r--r--   0        0        0     2270 2024-04-12 01:14:12.279905 reflex-0.5.0a2/reflex/utils/export.py
--rw-r--r--   0        0        0    22652 2024-04-24 21:16:40.841498 reflex-0.5.0a2/reflex/utils/format.py
--rw-r--r--   0        0        0     2309 2024-04-24 21:16:40.841612 reflex-0.5.0a2/reflex/utils/imports.py
--rw-r--r--   0        0        0     4737 2024-02-06 00:51:32.033457 reflex-0.5.0a2/reflex/utils/path_ops.py
--rw-r--r--   0        0        0    51212 2024-05-09 00:05:27.339607 reflex-0.5.0a2/reflex/utils/prerequisites.py
--rw-r--r--   0        0        0    11242 2024-05-07 15:33:05.688585 reflex-0.5.0a2/reflex/utils/processes.py
--rw-r--r--   0        0        0    30637 2024-05-05 01:15:24.061383 reflex-0.5.0a2/reflex/utils/pyi_generator.py
--rw-r--r--   0        0        0     9037 2024-04-24 21:16:40.842319 reflex-0.5.0a2/reflex/utils/serializers.py
--rw-r--r--   0        0        0     4688 2024-05-07 15:33:05.688896 reflex-0.5.0a2/reflex/utils/telemetry.py
--rw-r--r--   0        0        0    14842 2024-05-09 00:05:27.339984 reflex-0.5.0a2/reflex/utils/types.py
--rw-r--r--   0        0        0     2609 2023-10-22 18:57:13.223189 reflex-0.5.0a2/reflex/utils/watch.py
--rw-r--r--   0        0        0    67317 2024-04-25 16:52:48.845338 reflex-0.5.0a2/reflex/vars.py
--rw-r--r--   0        0        0     5583 2024-04-04 14:57:26.401034 reflex-0.5.0a2/reflex/vars.pyi
--rw-r--r--   0        0        0    12089 1970-01-01 00:00:00.000000 reflex-0.5.0a2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-07-20 22:42:41.698164 reflex-0.5.0a3/LICENSE
+-rw-r--r--   0        0        0     9842 2024-05-07 15:33:05.680965 reflex-0.5.0a3/README.md
+-rw-r--r--   0        0        0     2974 2024-05-13 23:06:02.764016 reflex-0.5.0a3/pyproject.toml
+-rw-r--r--   0        0        0     4286 2023-11-09 03:24:59.498329 reflex-0.5.0a3/reflex/.templates/apps/blank/assets/favicon.ico
+-rw-r--r--   0        0        0        0 2023-11-09 03:24:59.498383 reflex-0.5.0a3/reflex/.templates/apps/blank/code/__init__.py
+-rw-r--r--   0        0        0      926 2024-05-09 00:05:27.334397 reflex-0.5.0a3/reflex/.templates/apps/blank/code/blank.py
+-rw-r--r--   0        0        0       32 2023-11-09 03:24:59.498951 reflex-0.5.0a3/reflex/.templates/apps/demo/.gitignore
+-rw-r--r--   0        0        0     4286 2023-11-09 03:24:59.499075 reflex-0.5.0a3/reflex/.templates/apps/demo/assets/favicon.ico
+-rw-r--r--   0        0        0     1475 2023-11-09 03:24:59.499137 reflex-0.5.0a3/reflex/.templates/apps/demo/assets/github.svg
+-rw-r--r--   0        0        0     1899 2023-11-09 03:24:59.499199 reflex-0.5.0a3/reflex/.templates/apps/demo/assets/icon.svg
+-rw-r--r--   0        0        0     5403 2023-11-09 03:24:59.499298 reflex-0.5.0a3/reflex/.templates/apps/demo/assets/logo.svg
+-rw-r--r--   0        0        0      807 2023-11-09 03:24:59.499362 reflex-0.5.0a3/reflex/.templates/apps/demo/assets/paneleft.svg
+-rw-r--r--   0        0        0       32 2023-11-09 03:24:59.499458 reflex-0.5.0a3/reflex/.templates/apps/demo/code/__init__.py
+-rw-r--r--   0        0        0     2927 2024-05-13 23:05:41.140799 reflex-0.5.0a3/reflex/.templates/apps/demo/code/demo.py
+-rw-r--r--   0        0        0      194 2023-11-09 03:24:59.499716 reflex-0.5.0a3/reflex/.templates/apps/demo/code/pages/__init__.py
+-rw-r--r--   0        0        0      706 2024-02-17 20:02:02.399560 reflex-0.5.0a3/reflex/.templates/apps/demo/code/pages/chatapp.py
+-rw-r--r--   0        0        0    10906 2024-04-24 21:16:40.835599 reflex-0.5.0a3/reflex/.templates/apps/demo/code/pages/datatable.py
+-rw-r--r--   0        0        0     8381 2024-04-24 21:16:40.835772 reflex-0.5.0a3/reflex/.templates/apps/demo/code/pages/forms.py
+-rw-r--r--   0        0        0     8519 2024-03-20 23:54:55.830529 reflex-0.5.0a3/reflex/.templates/apps/demo/code/pages/graphing.py
+-rw-r--r--   0        0        0     1822 2024-02-17 20:02:02.400769 reflex-0.5.0a3/reflex/.templates/apps/demo/code/pages/home.py
+-rw-r--r--   0        0        0     4722 2024-02-17 20:02:02.400919 reflex-0.5.0a3/reflex/.templates/apps/demo/code/sidebar.py
+-rw-r--r--   0        0        0      510 2023-11-09 03:24:59.500529 reflex-0.5.0a3/reflex/.templates/apps/demo/code/state.py
+-rw-r--r--   0        0        0      912 2023-11-09 03:24:59.500616 reflex-0.5.0a3/reflex/.templates/apps/demo/code/states/form_state.py
+-rw-r--r--   0        0        0     1189 2023-11-09 03:24:59.500682 reflex-0.5.0a3/reflex/.templates/apps/demo/code/states/pie_state.py
+-rw-r--r--   0        0        0     1486 2024-02-17 20:02:02.401042 reflex-0.5.0a3/reflex/.templates/apps/demo/code/styles.py
+-rw-r--r--   0        0        0        0 2023-11-09 03:24:59.500792 reflex-0.5.0a3/reflex/.templates/apps/demo/code/webui/__init__.py
+-rw-r--r--   0        0        0      120 2023-11-09 03:24:59.500879 reflex-0.5.0a3/reflex/.templates/apps/demo/code/webui/components/__init__.py
+-rw-r--r--   0        0        0     3584 2024-02-17 20:02:02.401162 reflex-0.5.0a3/reflex/.templates/apps/demo/code/webui/components/chat.py
+-rw-r--r--   0        0        0      680 2023-11-09 03:24:59.500996 reflex-0.5.0a3/reflex/.templates/apps/demo/code/webui/components/loading_icon.py
+-rw-r--r--   0        0        0     1829 2024-02-17 20:02:02.401269 reflex-0.5.0a3/reflex/.templates/apps/demo/code/webui/components/modal.py
+-rw-r--r--   0        0        0     2251 2024-02-17 20:02:02.401372 reflex-0.5.0a3/reflex/.templates/apps/demo/code/webui/components/navbar.py
+-rw-r--r--   0        0        0     1735 2024-02-17 20:02:02.401457 reflex-0.5.0a3/reflex/.templates/apps/demo/code/webui/components/sidebar.py
+-rw-r--r--   0        0        0     4001 2023-11-09 03:24:59.501230 reflex-0.5.0a3/reflex/.templates/apps/demo/code/webui/state.py
+-rw-r--r--   0        0        0     2281 2024-02-17 20:02:02.401582 reflex-0.5.0a3/reflex/.templates/apps/demo/code/webui/styles.py
+-rw-r--r--   0        0        0       74 2023-10-22 18:57:13.188650 reflex-0.5.0a3/reflex/.templates/jinja/app/rxconfig.py.jinja2
+-rw-r--r--   0        0        0      127 2024-03-20 23:54:55.833038 reflex-0.5.0a3/reflex/.templates/jinja/custom_components/README.md.jinja2
+-rw-r--r--   0        0        0       32 2024-03-20 23:54:55.833129 reflex-0.5.0a3/reflex/.templates/jinja/custom_components/__init__.py.jinja2
+-rw-r--r--   0        0        0      826 2024-03-20 23:54:55.833525 reflex-0.5.0a3/reflex/.templates/jinja/custom_components/demo_app.py.jinja2
+-rw-r--r--   0        0        0      614 2024-04-04 14:57:26.374812 reflex-0.5.0a3/reflex/.templates/jinja/custom_components/pyproject.toml.jinja2
+-rw-r--r--   0        0        0     2403 2024-04-05 17:14:14.457446 reflex-0.5.0a3/reflex/.templates/jinja/custom_components/src.py.jinja2
+-rw-r--r--   0        0        0      548 2023-10-22 18:57:13.188813 reflex-0.5.0a3/reflex/.templates/jinja/web/package.json.jinja2
+-rw-r--r--   0        0        0      930 2024-03-20 23:54:55.834237 reflex-0.5.0a3/reflex/.templates/jinja/web/pages/_app.js.jinja2
+-rw-r--r--   0        0        0      182 2023-07-20 22:42:41.708822 reflex-0.5.0a3/reflex/.templates/jinja/web/pages/_document.js.jinja2
+-rw-r--r--   0        0        0      400 2024-02-06 00:51:31.970380 reflex-0.5.0a3/reflex/.templates/jinja/web/pages/base_page.js.jinja2
+-rw-r--r--   0        0        0       86 2023-10-22 18:57:13.188983 reflex-0.5.0a3/reflex/.templates/jinja/web/pages/component.js.jinja2
+-rw-r--r--   0        0        0      882 2023-12-01 04:51:31.091531 reflex-0.5.0a3/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
+-rw-r--r--   0        0        0      343 2024-04-04 14:57:26.375114 reflex-0.5.0a3/reflex/.templates/jinja/web/pages/index.js.jinja2
+-rw-r--r--   0        0        0      388 2024-04-05 17:14:14.457553 reflex-0.5.0a3/reflex/.templates/jinja/web/pages/stateful_component.js.jinja2
+-rw-r--r--   0        0        0      101 2023-12-01 04:51:31.092250 reflex-0.5.0a3/reflex/.templates/jinja/web/pages/stateful_components.js.jinja2
+-rw-r--r--   0        0        0     3883 2024-02-06 00:51:31.970618 reflex-0.5.0a3/reflex/.templates/jinja/web/pages/utils.js.jinja2
+-rw-r--r--   0        0        0      141 2023-12-06 18:41:46.628030 reflex-0.5.0a3/reflex/.templates/jinja/web/styles/styles.css.jinja2
+-rw-r--r--   0        0        0      761 2024-05-11 03:29:42.707807 reflex-0.5.0a3/reflex/.templates/jinja/web/tailwind.config.js.jinja2
+-rw-r--r--   0        0        0     3790 2024-03-20 23:54:55.834608 reflex-0.5.0a3/reflex/.templates/jinja/web/utils/context.js.jinja2
+-rw-r--r--   0        0        0       37 2023-12-06 19:37:00.189183 reflex-0.5.0a3/reflex/.templates/jinja/web/utils/theme.js.jinja2
+-rw-r--r--   0        0        0      417 2023-07-20 22:42:41.709243 reflex-0.5.0a3/reflex/.templates/web/.gitignore
+-rw-r--r--   0        0        0      595 2023-10-30 01:36:56.133208 reflex-0.5.0a3/reflex/.templates/web/components/reflex/chakra_color_mode_provider.js
+-rw-r--r--   0        0        0      645 2024-03-20 23:54:55.835034 reflex-0.5.0a3/reflex/.templates/web/components/reflex/radix_themes_color_mode_provider.js
+-rw-r--r--   0        0        0       97 2023-10-22 18:57:13.190257 reflex-0.5.0a3/reflex/.templates/web/jsconfig.json
+-rw-r--r--   0        0        0      118 2023-11-22 05:49:24.669539 reflex-0.5.0a3/reflex/.templates/web/next.config.js
+-rw-r--r--   0        0        0       82 2023-07-20 22:42:41.710359 reflex-0.5.0a3/reflex/.templates/web/postcss.config.js
+-rw-r--r--   0        0        0       59 2023-07-20 22:42:41.710616 reflex-0.5.0a3/reflex/.templates/web/styles/tailwind.css
+-rw-r--r--   0        0        0     1254 2023-09-16 20:27:37.277783 reflex-0.5.0a3/reflex/.templates/web/utils/client_side_routing.js
+-rw-r--r--   0        0        0     1622 2024-02-06 00:51:31.970968 reflex-0.5.0a3/reflex/.templates/web/utils/helpers/dataeditor.js
+-rw-r--r--   0        0        0      528 2024-05-05 01:15:24.052298 reflex-0.5.0a3/reflex/.templates/web/utils/helpers/debounce.js
+-rw-r--r--   0        0        0     1152 2023-11-22 05:49:24.669991 reflex-0.5.0a3/reflex/.templates/web/utils/helpers/range.js
+-rw-r--r--   0        0        0      566 2024-05-05 01:15:24.052363 reflex-0.5.0a3/reflex/.templates/web/utils/helpers/throttle.js
+-rw-r--r--   0        0        0    22511 2024-05-05 01:15:24.052487 reflex-0.5.0a3/reflex/.templates/web/utils/state.js
+-rw-r--r--   0        0        0     5831 2024-05-09 00:05:27.334655 reflex-0.5.0a3/reflex/__init__.py
+-rw-r--r--   0        0        0     7791 2024-05-09 12:11:15.217578 reflex-0.5.0a3/reflex/__init__.pyi
+-rw-r--r--   0        0        0      108 2023-08-05 17:01:44.301997 reflex-0.5.0a3/reflex/__main__.py
+-rw-r--r--   0        0        0      373 2023-07-20 22:42:41.710893 reflex-0.5.0a3/reflex/admin.py
+-rw-r--r--   0        0        0    46314 2024-05-09 00:05:27.335022 reflex-0.5.0a3/reflex/app.py
+-rw-r--r--   0        0        0     1152 2024-05-05 01:15:24.053241 reflex-0.5.0a3/reflex/app_module_for_backend.py
+-rw-r--r--   0        0        0     4213 2024-05-09 00:05:27.335300 reflex-0.5.0a3/reflex/base.py
+-rw-r--r--   0        0        0       27 2023-07-20 22:42:41.711176 reflex-0.5.0a3/reflex/compiler/__init__.py
+-rw-r--r--   0        0        0    17455 2024-05-07 15:33:05.682544 reflex-0.5.0a3/reflex/compiler/compiler.py
+-rw-r--r--   0        0        0     4344 2024-03-20 23:54:55.838388 reflex-0.5.0a3/reflex/compiler/templates.py
+-rw-r--r--   0        0        0    13274 2024-05-09 00:05:27.335443 reflex-0.5.0a3/reflex/compiler/utils.py
+-rw-r--r--   0        0        0      552 2024-05-05 01:15:24.053486 reflex-0.5.0a3/reflex/components/__init__.py
+-rw-r--r--   0        0        0      325 2024-02-06 00:51:31.973078 reflex-0.5.0a3/reflex/components/base/__init__.py
+-rw-r--r--   0        0        0      573 2024-02-06 00:51:31.973178 reflex-0.5.0a3/reflex/components/base/app_wrap.py
+-rw-r--r--   0        0        0     2890 2024-04-24 19:31:24.924269 reflex-0.5.0a3/reflex/components/base/app_wrap.pyi
+-rw-r--r--   0        0        0     1234 2024-04-04 14:57:26.376921 reflex-0.5.0a3/reflex/components/base/bare.py
+-rw-r--r--   0        0        0      151 2023-07-20 22:42:41.711762 reflex-0.5.0a3/reflex/components/base/body.py
+-rw-r--r--   0        0        0     3206 2024-04-24 19:31:56.503225 reflex-0.5.0a3/reflex/components/base/body.pyi
+-rw-r--r--   0        0        0      583 2024-03-20 23:54:55.839153 reflex-0.5.0a3/reflex/components/base/document.py
+-rw-r--r--   0        0        0    14232 2024-04-24 19:31:51.758673 reflex-0.5.0a3/reflex/components/base/document.pyi
+-rw-r--r--   0        0        0      312 2024-02-06 00:51:31.973871 reflex-0.5.0a3/reflex/components/base/fragment.py
+-rw-r--r--   0        0        0     3218 2024-04-24 19:31:51.784884 reflex-0.5.0a3/reflex/components/base/fragment.pyi
+-rw-r--r--   0        0        0      297 2023-12-05 17:15:35.585518 reflex-0.5.0a3/reflex/components/base/head.py
+-rw-r--r--   0        0        0     6002 2024-04-24 19:31:53.335977 reflex-0.5.0a3/reflex/components/base/head.pyi
+-rw-r--r--   0        0        0      929 2023-07-20 22:42:41.711911 reflex-0.5.0a3/reflex/components/base/link.py
+-rw-r--r--   0        0        0     6990 2024-04-24 19:31:27.077164 reflex-0.5.0a3/reflex/components/base/link.pyi
+-rw-r--r--   0        0        0     1438 2023-09-16 20:27:37.279391 reflex-0.5.0a3/reflex/components/base/meta.py
+-rw-r--r--   0        0        0    12804 2024-04-24 19:31:22.783259 reflex-0.5.0a3/reflex/components/base/meta.pyi
+-rw-r--r--   0        0        0     2298 2023-10-30 01:36:56.136333 reflex-0.5.0a3/reflex/components/base/script.py
+-rw-r--r--   0        0        0     4500 2024-04-24 19:31:45.804898 reflex-0.5.0a3/reflex/components/base/script.pyi
+-rw-r--r--   0        0        0     6378 2024-02-17 20:02:02.406461 reflex-0.5.0a3/reflex/components/chakra/__init__.py
+-rw-r--r--   0        0        0     5242 2024-02-07 21:49:00.589344 reflex-0.5.0a3/reflex/components/chakra/base.py
+-rw-r--r--   0        0        0    10917 2024-04-24 19:31:39.254151 reflex-0.5.0a3/reflex/components/chakra/base.pyi
+-rw-r--r--   0        0        0      459 2024-02-17 20:02:02.406937 reflex-0.5.0a3/reflex/components/chakra/datadisplay/__init__.py
+-rw-r--r--   0        0        0      352 2024-02-07 21:48:43.271089 reflex-0.5.0a3/reflex/components/chakra/datadisplay/badge.py
+-rw-r--r--   0        0        0     3654 2024-04-24 19:31:56.520176 reflex-0.5.0a3/reflex/components/chakra/datadisplay/badge.pyi
+-rw-r--r--   0        0        0      174 2024-02-17 20:02:02.407242 reflex-0.5.0a3/reflex/components/chakra/datadisplay/code.py
+-rw-r--r--   0        0        0     3229 2024-04-24 19:31:20.836024 reflex-0.5.0a3/reflex/components/chakra/datadisplay/code.pyi
+-rw-r--r--   0        0        0      657 2024-02-07 21:48:43.271979 reflex-0.5.0a3/reflex/components/chakra/datadisplay/divider.py
+-rw-r--r--   0        0        0     3934 2024-04-24 19:31:33.713586 reflex-0.5.0a3/reflex/components/chakra/datadisplay/divider.pyi
+-rw-r--r--   0        0        0      180 2024-02-07 21:48:43.272341 reflex-0.5.0a3/reflex/components/chakra/datadisplay/keyboard_key.py
+-rw-r--r--   0        0        0     3251 2024-04-24 19:31:32.872876 reflex-0.5.0a3/reflex/components/chakra/datadisplay/keyboard_key.pyi
+-rw-r--r--   0        0        0     1484 2024-05-05 01:15:24.053780 reflex-0.5.0a3/reflex/components/chakra/datadisplay/list.py
+-rw-r--r--   0        0        0    12991 2024-05-05 01:15:24.053953 reflex-0.5.0a3/reflex/components/chakra/datadisplay/list.pyi
+-rw-r--r--   0        0        0     2149 2024-02-07 21:48:43.272980 reflex-0.5.0a3/reflex/components/chakra/datadisplay/stat.py
+-rw-r--r--   0        0        0    17461 2024-04-24 19:31:58.481785 reflex-0.5.0a3/reflex/components/chakra/datadisplay/stat.pyi
+-rw-r--r--   0        0        0     9122 2024-02-07 21:48:43.273484 reflex-0.5.0a3/reflex/components/chakra/datadisplay/table.py
+-rw-r--r--   0        0        0    27252 2024-04-24 19:32:01.076794 reflex-0.5.0a3/reflex/components/chakra/datadisplay/table.pyi
+-rw-r--r--   0        0        0     2294 2024-02-07 21:48:43.273971 reflex-0.5.0a3/reflex/components/chakra/datadisplay/tag.py
+-rw-r--r--   0        0        0    15734 2024-04-24 19:31:39.394572 reflex-0.5.0a3/reflex/components/chakra/datadisplay/tag.pyi
+-rw-r--r--   0        0        0      384 2024-02-06 00:51:31.976988 reflex-0.5.0a3/reflex/components/chakra/disclosure/__init__.py
+-rw-r--r--   0        0        0     3510 2024-04-24 21:16:40.836539 reflex-0.5.0a3/reflex/components/chakra/disclosure/accordion.py
+-rw-r--r--   0        0        0    15803 2024-04-24 19:31:46.785267 reflex-0.5.0a3/reflex/components/chakra/disclosure/accordion.pyi
+-rw-r--r--   0        0        0     3295 2024-02-07 21:48:43.274669 reflex-0.5.0a3/reflex/components/chakra/disclosure/tabs.py
+-rw-r--r--   0        0        0    18525 2024-04-24 19:31:51.181381 reflex-0.5.0a3/reflex/components/chakra/disclosure/tabs.pyi
+-rw-r--r--   0        0        0     1732 2024-02-07 21:48:43.274917 reflex-0.5.0a3/reflex/components/chakra/disclosure/transition.py
+-rw-r--r--   0        0        0    20003 2024-04-24 19:31:47.452515 reflex-0.5.0a3/reflex/components/chakra/disclosure/transition.pyi
+-rw-r--r--   0        0        0      278 2024-02-07 21:48:43.275325 reflex-0.5.0a3/reflex/components/chakra/disclosure/visuallyhidden.py
+-rw-r--r--   0        0        0     3258 2024-04-24 19:31:21.739444 reflex-0.5.0a3/reflex/components/chakra/disclosure/visuallyhidden.pyi
+-rw-r--r--   0        0        0      313 2024-02-06 00:51:31.977813 reflex-0.5.0a3/reflex/components/chakra/feedback/__init__.py
+-rw-r--r--   0        0        0     1623 2024-02-07 21:48:43.275534 reflex-0.5.0a3/reflex/components/chakra/feedback/alert.py
+-rw-r--r--   0        0        0    12381 2024-04-24 19:31:36.018582 reflex-0.5.0a3/reflex/components/chakra/feedback/alert.pyi
+-rw-r--r--   0        0        0     2006 2024-02-07 21:48:43.275746 reflex-0.5.0a3/reflex/components/chakra/feedback/circularprogress.py
+-rw-r--r--   0        0        0     7637 2024-04-24 19:31:35.464688 reflex-0.5.0a3/reflex/components/chakra/feedback/circularprogress.pyi
+-rw-r--r--   0        0        0      871 2024-02-07 21:48:43.275966 reflex-0.5.0a3/reflex/components/chakra/feedback/progress.py
+-rw-r--r--   0        0        0     4278 2024-04-24 19:31:39.746055 reflex-0.5.0a3/reflex/components/chakra/feedback/progress.pyi
+-rw-r--r--   0        0        0     1776 2024-02-07 21:48:43.276180 reflex-0.5.0a3/reflex/components/chakra/feedback/skeleton.py
+-rw-r--r--   0        0        0    10690 2024-04-24 19:32:01.405002 reflex-0.5.0a3/reflex/components/chakra/feedback/skeleton.pyi
+-rw-r--r--   0        0        0      704 2024-02-07 21:48:43.276461 reflex-0.5.0a3/reflex/components/chakra/feedback/spinner.py
+-rw-r--r--   0        0        0     4107 2024-04-24 19:31:21.992081 reflex-0.5.0a3/reflex/components/chakra/feedback/spinner.pyi
+-rw-r--r--   0        0        0     1453 2024-02-17 20:02:02.409691 reflex-0.5.0a3/reflex/components/chakra/forms/__init__.py
+-rw-r--r--   0        0        0     2395 2024-02-07 21:48:43.276688 reflex-0.5.0a3/reflex/components/chakra/forms/button.py
+-rw-r--r--   0        0        0    10545 2024-04-24 19:32:02.037829 reflex-0.5.0a3/reflex/components/chakra/forms/button.pyi
+-rw-r--r--   0        0        0     2764 2024-02-07 21:48:43.277006 reflex-0.5.0a3/reflex/components/chakra/forms/checkbox.py
+-rw-r--r--   0        0        0    10301 2024-04-24 19:31:34.287807 reflex-0.5.0a3/reflex/components/chakra/forms/checkbox.pyi
+-rw-r--r--   0        0        0     2860 2024-02-17 20:02:02.410102 reflex-0.5.0a3/reflex/components/chakra/forms/colormodeswitch.py
+-rw-r--r--   0        0        0    18459 2024-04-24 19:31:24.856589 reflex-0.5.0a3/reflex/components/chakra/forms/colormodeswitch.pyi
+-rw-r--r--   0        0        0      246 2024-02-06 00:51:31.979244 reflex-0.5.0a3/reflex/components/chakra/forms/date_picker.py
+-rw-r--r--   0        0        0     5841 2024-04-24 19:31:54.024641 reflex-0.5.0a3/reflex/components/chakra/forms/date_picker.pyi
+-rw-r--r--   0        0        0      280 2024-02-06 00:51:31.979387 reflex-0.5.0a3/reflex/components/chakra/forms/date_time_picker.py
+-rw-r--r--   0        0        0     5854 2024-04-24 19:31:40.823621 reflex-0.5.0a3/reflex/components/chakra/forms/date_time_picker.pyi
+-rw-r--r--   0        0        0     2110 2024-02-07 21:48:43.277649 reflex-0.5.0a3/reflex/components/chakra/forms/editable.py
+-rw-r--r--   0        0        0    13339 2024-04-24 19:31:15.703021 reflex-0.5.0a3/reflex/components/chakra/forms/editable.pyi
+-rw-r--r--   0        0        0      246 2024-02-06 00:51:31.979682 reflex-0.5.0a3/reflex/components/chakra/forms/email.py
+-rw-r--r--   0        0        0     5825 2024-04-24 19:31:50.788652 reflex-0.5.0a3/reflex/components/chakra/forms/email.pyi
+-rw-r--r--   0        0        0     2579 2024-03-20 23:54:55.839690 reflex-0.5.0a3/reflex/components/chakra/forms/form.py
+-rw-r--r--   0        0        0    20619 2024-04-24 19:31:56.858215 reflex-0.5.0a3/reflex/components/chakra/forms/form.pyi
+-rw-r--r--   0        0        0      935 2024-02-06 00:51:31.980162 reflex-0.5.0a3/reflex/components/chakra/forms/iconbutton.py
+-rw-r--r--   0        0        0     4668 2024-04-24 19:31:50.346409 reflex-0.5.0a3/reflex/components/chakra/forms/iconbutton.pyi
+-rw-r--r--   0        0        0     4312 2024-03-20 23:54:55.840321 reflex-0.5.0a3/reflex/components/chakra/forms/input.py
+-rw-r--r--   0        0        0    21514 2024-04-24 19:31:59.673777 reflex-0.5.0a3/reflex/components/chakra/forms/input.pyi
+-rw-r--r--   0        0        0    12940 2024-02-06 00:51:31.980569 reflex-0.5.0a3/reflex/components/chakra/forms/multiselect.py
+-rw-r--r--   0        0        0     4334 2024-02-07 21:48:43.278754 reflex-0.5.0a3/reflex/components/chakra/forms/numberinput.py
+-rw-r--r--   0        0        0    18093 2024-04-24 19:31:56.097983 reflex-0.5.0a3/reflex/components/chakra/forms/numberinput.pyi
+-rw-r--r--   0        0        0      256 2024-02-06 00:51:31.980851 reflex-0.5.0a3/reflex/components/chakra/forms/password.py
+-rw-r--r--   0        0        0     5834 2024-04-24 19:31:37.858051 reflex-0.5.0a3/reflex/components/chakra/forms/password.pyi
+-rw-r--r--   0        0        0     6503 2024-04-12 01:14:12.262063 reflex-0.5.0a3/reflex/components/chakra/forms/pininput.py
+-rw-r--r--   0        0        0     9369 2024-05-05 01:15:24.054063 reflex-0.5.0a3/reflex/components/chakra/forms/pininput.pyi
+-rw-r--r--   0        0        0     3172 2024-04-12 01:14:12.263122 reflex-0.5.0a3/reflex/components/chakra/forms/radio.py
+-rw-r--r--   0        0        0     8410 2024-04-24 19:31:17.428977 reflex-0.5.0a3/reflex/components/chakra/forms/radio.pyi
+-rw-r--r--   0        0        0     4543 2024-04-12 01:14:12.263746 reflex-0.5.0a3/reflex/components/chakra/forms/rangeslider.py
+-rw-r--r--   0        0        0    13939 2024-04-24 19:31:59.377848 reflex-0.5.0a3/reflex/components/chakra/forms/rangeslider.pyi
+-rw-r--r--   0        0        0     3624 2024-02-07 21:48:43.280461 reflex-0.5.0a3/reflex/components/chakra/forms/select.py
+-rw-r--r--   0        0        0     8868 2024-04-24 19:31:48.346816 reflex-0.5.0a3/reflex/components/chakra/forms/select.pyi
+-rw-r--r--   0        0        0     3532 2024-02-07 21:48:43.280779 reflex-0.5.0a3/reflex/components/chakra/forms/slider.py
+-rw-r--r--   0        0        0    17461 2024-04-24 19:32:01.264082 reflex-0.5.0a3/reflex/components/chakra/forms/slider.pyi
+-rw-r--r--   0        0        0     1838 2024-02-07 21:48:43.281044 reflex-0.5.0a3/reflex/components/chakra/forms/switch.py
+-rw-r--r--   0        0        0     6531 2024-04-24 19:31:48.016708 reflex-0.5.0a3/reflex/components/chakra/forms/switch.pyi
+-rw-r--r--   0        0        0     2474 2024-02-09 10:00:28.809203 reflex-0.5.0a3/reflex/components/chakra/forms/textarea.py
+-rw-r--r--   0        0        0     5419 2024-04-24 19:31:51.889720 reflex-0.5.0a3/reflex/components/chakra/forms/textarea.pyi
+-rw-r--r--   0        0        0      246 2024-02-06 00:51:31.982573 reflex-0.5.0a3/reflex/components/chakra/forms/time_picker.py
+-rw-r--r--   0        0        0     5841 2024-04-24 19:31:46.686774 reflex-0.5.0a3/reflex/components/chakra/forms/time_picker.pyi
+-rw-r--r--   0        0        0      487 2024-02-17 20:02:02.413006 reflex-0.5.0a3/reflex/components/chakra/layout/__init__.py
+-rw-r--r--   0        0        0      315 2024-02-07 21:48:43.281752 reflex-0.5.0a3/reflex/components/chakra/layout/aspect_ratio.py
+-rw-r--r--   0        0        0     3379 2024-04-24 19:31:52.881611 reflex-0.5.0a3/reflex/components/chakra/layout/aspect_ratio.pyi
+-rw-r--r--   0        0        0      755 2024-02-07 21:48:43.281982 reflex-0.5.0a3/reflex/components/chakra/layout/box.py
+-rw-r--r--   0        0        0     3662 2024-04-24 19:31:18.516418 reflex-0.5.0a3/reflex/components/chakra/layout/box.pyi
+-rw-r--r--   0        0        0     2967 2024-02-07 21:48:43.282202 reflex-0.5.0a3/reflex/components/chakra/layout/card.py
+-rw-r--r--   0        0        0    13850 2024-04-24 19:31:48.005155 reflex-0.5.0a3/reflex/components/chakra/layout/card.pyi
+-rw-r--r--   0        0        0      389 2024-02-07 21:48:43.282417 reflex-0.5.0a3/reflex/components/chakra/layout/center.py
+-rw-r--r--   0        0        0     8692 2024-04-24 19:31:24.264440 reflex-0.5.0a3/reflex/components/chakra/layout/center.pyi
+-rw-r--r--   0        0        0      354 2024-02-07 21:48:43.282843 reflex-0.5.0a3/reflex/components/chakra/layout/container.py
+-rw-r--r--   0        0        0     3431 2024-04-24 19:31:47.990635 reflex-0.5.0a3/reflex/components/chakra/layout/container.pyi
+-rw-r--r--   0        0        0      715 2024-02-07 21:48:43.283082 reflex-0.5.0a3/reflex/components/chakra/layout/flex.py
+-rw-r--r--   0        0        0     4138 2024-04-24 19:31:44.830583 reflex-0.5.0a3/reflex/components/chakra/layout/flex.pyi
+-rw-r--r--   0        0        0     4318 2024-02-07 21:48:43.283328 reflex-0.5.0a3/reflex/components/chakra/layout/grid.py
+-rw-r--r--   0        0        0    13853 2024-04-24 19:31:41.333938 reflex-0.5.0a3/reflex/components/chakra/layout/grid.pyi
+-rw-r--r--   0        0        0      179 2024-02-07 21:48:43.283579 reflex-0.5.0a3/reflex/components/chakra/layout/spacer.py
+-rw-r--r--   0        0        0     3230 2024-04-24 19:31:48.988499 reflex-0.5.0a3/reflex/components/chakra/layout/spacer.pyi
+-rw-r--r--   0        0        0     1077 2024-02-07 21:48:43.283791 reflex-0.5.0a3/reflex/components/chakra/layout/stack.py
+-rw-r--r--   0        0        0    12219 2024-04-24 19:31:34.279618 reflex-0.5.0a3/reflex/components/chakra/layout/stack.pyi
+-rw-r--r--   0        0        0     1463 2024-02-07 21:48:43.284089 reflex-0.5.0a3/reflex/components/chakra/layout/wrap.py
+-rw-r--r--   0        0        0     6943 2024-04-24 19:31:33.351664 reflex-0.5.0a3/reflex/components/chakra/layout/wrap.pyi
+-rw-r--r--   0        0        0      190 2024-02-06 00:51:31.985088 reflex-0.5.0a3/reflex/components/chakra/media/__init__.py
+-rw-r--r--   0        0        0     1668 2024-02-07 21:48:43.284332 reflex-0.5.0a3/reflex/components/chakra/media/avatar.py
+-rw-r--r--   0        0        0    10445 2024-04-24 19:31:27.389378 reflex-0.5.0a3/reflex/components/chakra/media/avatar.pyi
+-rw-r--r--   0        0        0     2462 2024-04-24 21:16:40.836689 reflex-0.5.0a3/reflex/components/chakra/media/icon.py
+-rw-r--r--   0        0        0     6271 2024-04-24 19:31:19.854478 reflex-0.5.0a3/reflex/components/chakra/media/icon.pyi
+-rw-r--r--   0        0        0     2400 2024-02-07 21:48:43.284781 reflex-0.5.0a3/reflex/components/chakra/media/image.py
+-rw-r--r--   0        0        0     5423 2024-04-24 19:31:52.691354 reflex-0.5.0a3/reflex/components/chakra/media/image.pyi
+-rw-r--r--   0        0        0      419 2024-02-06 00:51:31.986093 reflex-0.5.0a3/reflex/components/chakra/navigation/__init__.py
+-rw-r--r--   0        0        0     2925 2024-02-07 21:48:43.285023 reflex-0.5.0a3/reflex/components/chakra/navigation/breadcrumb.py
+-rw-r--r--   0        0        0    13575 2024-04-24 19:32:01.936776 reflex-0.5.0a3/reflex/components/chakra/navigation/breadcrumb.pyi
+-rw-r--r--   0        0        0     1475 2024-02-06 00:51:31.986318 reflex-0.5.0a3/reflex/components/chakra/navigation/link.py
+-rw-r--r--   0        0        0     3999 2024-04-24 19:31:19.850596 reflex-0.5.0a3/reflex/components/chakra/navigation/link.pyi
+-rw-r--r--   0        0        0      521 2024-02-06 00:51:31.986581 reflex-0.5.0a3/reflex/components/chakra/navigation/linkoverlay.py
+-rw-r--r--   0        0        0     6233 2024-04-24 19:31:59.056993 reflex-0.5.0a3/reflex/components/chakra/navigation/linkoverlay.pyi
+-rw-r--r--   0        0        0     2935 2024-02-07 21:48:43.285634 reflex-0.5.0a3/reflex/components/chakra/navigation/stepper.py
+-rw-r--r--   0        0        0    27922 2024-04-24 19:31:59.991438 reflex-0.5.0a3/reflex/components/chakra/navigation/stepper.pyi
+-rw-r--r--   0        0        0      850 2024-02-06 00:51:31.987014 reflex-0.5.0a3/reflex/components/chakra/overlay/__init__.py
+-rw-r--r--   0        0        0     5200 2024-02-07 21:48:43.285952 reflex-0.5.0a3/reflex/components/chakra/overlay/alertdialog.py
+-rw-r--r--   0        0        0    23985 2024-04-24 19:31:53.441920 reflex-0.5.0a3/reflex/components/chakra/overlay/alertdialog.pyi
+-rw-r--r--   0        0        0     5186 2024-02-06 00:51:31.987467 reflex-0.5.0a3/reflex/components/chakra/overlay/drawer.py
+-rw-r--r--   0        0        0    25406 2024-04-24 19:32:02.090146 reflex-0.5.0a3/reflex/components/chakra/overlay/drawer.pyi
+-rw-r--r--   0        0        0     6974 2024-02-07 21:48:43.286352 reflex-0.5.0a3/reflex/components/chakra/overlay/menu.py
+-rw-r--r--   0        0        0    28682 2024-04-24 19:32:03.285218 reflex-0.5.0a3/reflex/components/chakra/overlay/menu.pyi
+-rw-r--r--   0        0        0     5270 2024-02-07 21:48:43.286588 reflex-0.5.0a3/reflex/components/chakra/overlay/modal.py
+-rw-r--r--   0        0        0    23549 2024-04-24 19:32:01.507839 reflex-0.5.0a3/reflex/components/chakra/overlay/modal.pyi
+-rw-r--r--   0        0        0     5967 2024-02-07 21:48:43.286836 reflex-0.5.0a3/reflex/components/chakra/overlay/popover.py
+-rw-r--r--   0        0        0    29893 2024-04-24 19:32:01.594206 reflex-0.5.0a3/reflex/components/chakra/overlay/popover.pyi
+-rw-r--r--   0        0        0     2127 2024-02-07 21:48:43.287207 reflex-0.5.0a3/reflex/components/chakra/overlay/tooltip.py
+-rw-r--r--   0        0        0     6060 2024-04-24 19:31:15.213215 reflex-0.5.0a3/reflex/components/chakra/overlay/tooltip.pyi
+-rw-r--r--   0        0        0      271 2024-02-06 00:51:31.988661 reflex-0.5.0a3/reflex/components/chakra/typography/__init__.py
+-rw-r--r--   0        0        0      379 2024-02-07 21:48:43.287449 reflex-0.5.0a3/reflex/components/chakra/typography/heading.py
+-rw-r--r--   0        0        0     3706 2024-04-24 19:31:17.288584 reflex-0.5.0a3/reflex/components/chakra/typography/heading.pyi
+-rw-r--r--   0        0        0      671 2024-02-07 21:48:43.287662 reflex-0.5.0a3/reflex/components/chakra/typography/highlight.py
+-rw-r--r--   0        0        0     3645 2024-04-24 19:31:37.053293 reflex-0.5.0a3/reflex/components/chakra/typography/highlight.pyi
+-rw-r--r--   0        0        0      328 2024-02-07 21:48:43.287874 reflex-0.5.0a3/reflex/components/chakra/typography/span.py
+-rw-r--r--   0        0        0     3372 2024-04-24 19:31:23.281815 reflex-0.5.0a3/reflex/components/chakra/typography/span.pyi
+-rw-r--r--   0        0        0      472 2024-02-07 21:48:43.288076 reflex-0.5.0a3/reflex/components/chakra/typography/text.py
+-rw-r--r--   0        0        0     3596 2024-04-24 19:31:50.785304 reflex-0.5.0a3/reflex/components/chakra/typography/text.pyi
+-rw-r--r--   0        0        0    75744 2024-05-11 03:29:42.708073 reflex-0.5.0a3/reflex/components/component.py
+-rw-r--r--   0        0        0      857 2024-04-25 16:52:48.840950 reflex-0.5.0a3/reflex/components/core/__init__.py
+-rw-r--r--   0        0        0     5943 2024-04-04 14:57:26.386161 reflex-0.5.0a3/reflex/components/core/banner.py
+-rw-r--r--   0        0        0    17164 2024-04-24 19:32:01.784962 reflex-0.5.0a3/reflex/components/core/banner.pyi
+-rw-r--r--   0        0        0     1873 2024-02-06 00:51:31.991625 reflex-0.5.0a3/reflex/components/core/client_side_routing.py
+-rw-r--r--   0        0        0     6264 2024-04-24 19:31:22.918462 reflex-0.5.0a3/reflex/components/core/client_side_routing.pyi
+-rw-r--r--   0        0        0      590 2024-02-17 20:02:02.417474 reflex-0.5.0a3/reflex/components/core/colors.py
+-rw-r--r--   0        0        0     6005 2024-05-07 15:33:05.683015 reflex-0.5.0a3/reflex/components/core/cond.py
+-rw-r--r--   0        0        0     4888 2024-05-09 00:05:27.335942 reflex-0.5.0a3/reflex/components/core/debounce.py
+-rw-r--r--   0        0        0     4216 2024-04-25 16:52:48.841425 reflex-0.5.0a3/reflex/components/core/debounce.pyi
+-rw-r--r--   0        0        0     4334 2024-05-11 03:29:42.708393 reflex-0.5.0a3/reflex/components/core/foreach.py
+-rw-r--r--   0        0        0     1284 2024-05-05 01:15:24.054752 reflex-0.5.0a3/reflex/components/core/html.py
+-rw-r--r--   0        0        0     6616 2024-04-25 05:29:57.085054 reflex-0.5.0a3/reflex/components/core/html.pyi
+-rw-r--r--   0        0        0       30 2024-02-07 21:48:43.290204 reflex-0.5.0a3/reflex/components/core/layout/__init__.py
+-rw-r--r--   0        0        0     9484 2024-05-07 15:33:05.683232 reflex-0.5.0a3/reflex/components/core/match.py
+-rw-r--r--   0        0        0     1907 2024-04-04 14:19:59.331992 reflex-0.5.0a3/reflex/components/core/responsive.py
+-rw-r--r--   0        0        0    10193 2024-05-05 01:15:24.055101 reflex-0.5.0a3/reflex/components/core/upload.py
+-rw-r--r--   0        0        0    17147 2024-04-25 16:52:48.841883 reflex-0.5.0a3/reflex/components/core/upload.pyi
+-rw-r--r--   0        0        0      357 2024-04-05 17:14:14.460655 reflex-0.5.0a3/reflex/components/datadisplay/__init__.py
+-rw-r--r--   0        0        0    11363 2024-05-07 15:33:05.683354 reflex-0.5.0a3/reflex/components/datadisplay/code.py
+-rw-r--r--   0        0        0    31213 2024-05-07 15:33:05.683489 reflex-0.5.0a3/reflex/components/datadisplay/code.pyi
+-rw-r--r--   0        0        0    12632 2024-02-06 00:51:31.995005 reflex-0.5.0a3/reflex/components/datadisplay/dataeditor.py
+-rw-r--r--   0        0        0    10485 2024-04-24 19:31:43.237754 reflex-0.5.0a3/reflex/components/datadisplay/dataeditor.pyi
+-rw-r--r--   0        0        0     2562 2024-04-05 17:14:14.460754 reflex-0.5.0a3/reflex/components/datadisplay/logo.py
+-rw-r--r--   0        0        0       73 2023-11-26 20:56:44.132351 reflex-0.5.0a3/reflex/components/el/__init__.py
+-rw-r--r--   0        0        0      113 2023-11-26 20:56:44.132431 reflex-0.5.0a3/reflex/components/el/constants/__init__.py
+-rw-r--r--   0        0        0     7175 2023-11-26 20:56:44.132596 reflex-0.5.0a3/reflex/components/el/constants/html.py
+-rw-r--r--   0        0        0    15554 2023-11-26 20:56:44.132713 reflex-0.5.0a3/reflex/components/el/constants/react.py
+-rw-r--r--   0        0        0     1713 2023-11-26 20:56:44.132789 reflex-0.5.0a3/reflex/components/el/constants/reflex.py
+-rw-r--r--   0        0        0      494 2023-12-01 04:51:31.098496 reflex-0.5.0a3/reflex/components/el/element.py
+-rw-r--r--   0        0        0     3213 2024-04-24 19:32:01.854505 reflex-0.5.0a3/reflex/components/el/element.pyi
+-rw-r--r--   0        0        0     3529 2024-03-20 23:54:55.843475 reflex-0.5.0a3/reflex/components/el/elements/__init__.py
+-rw-r--r--   0        0        0     1982 2024-02-17 20:02:02.419390 reflex-0.5.0a3/reflex/components/el/elements/base.py
+-rw-r--r--   0        0        0     6340 2024-04-24 19:31:34.952107 reflex-0.5.0a3/reflex/components/el/elements/base.pyi
+-rw-r--r--   0        0        0    20103 2024-04-25 16:52:48.842221 reflex-0.5.0a3/reflex/components/el/elements/forms.py
+-rw-r--r--   0        0        0    99555 2024-04-25 16:52:48.842962 reflex-0.5.0a3/reflex/components/el/elements/forms.pyi
+-rw-r--r--   0        0        0     3610 2024-02-06 00:51:31.998070 reflex-0.5.0a3/reflex/components/el/elements/inline.py
+-rw-r--r--   0        0        0   164607 2024-04-24 19:32:05.408521 reflex-0.5.0a3/reflex/components/el/elements/inline.pyi
+-rw-r--r--   0        0        0     7929 2024-03-20 23:54:55.844702 reflex-0.5.0a3/reflex/components/el/elements/media.py
+-rw-r--r--   0        0        0    93567 2024-04-24 19:32:03.850879 reflex-0.5.0a3/reflex/components/el/elements/media.pyi
+-rw-r--r--   0        0        0     1337 2023-11-26 20:56:44.134404 reflex-0.5.0a3/reflex/components/el/elements/metadata.py
+-rw-r--r--   0        0        0    28031 2024-04-24 19:32:01.554937 reflex-0.5.0a3/reflex/components/el/elements/metadata.pyi
+-rw-r--r--   0        0        0     1569 2023-11-26 20:56:44.134590 reflex-0.5.0a3/reflex/components/el/elements/other.py
+-rw-r--r--   0        0        0    42033 2024-04-24 19:31:59.581160 reflex-0.5.0a3/reflex/components/el/elements/other.pyi
+-rw-r--r--   0        0        0     1406 2024-02-17 20:02:02.421306 reflex-0.5.0a3/reflex/components/el/elements/scripts.py
+-rw-r--r--   0        0        0    19615 2024-04-24 19:31:22.715670 reflex-0.5.0a3/reflex/components/el/elements/scripts.pyi
+-rw-r--r--   0        0        0     1535 2024-02-17 20:02:02.421507 reflex-0.5.0a3/reflex/components/el/elements/sectioning.py
+-rw-r--r--   0        0        0    87242 2024-04-24 19:32:04.046011 reflex-0.5.0a3/reflex/components/el/elements/sectioning.pyi
+-rw-r--r--   0        0        0     2767 2024-02-17 20:02:02.421759 reflex-0.5.0a3/reflex/components/el/elements/tables.py
+-rw-r--r--   0        0        0    61849 2024-04-24 19:32:03.007985 reflex-0.5.0a3/reflex/components/el/elements/tables.pyi
+-rw-r--r--   0        0        0     2432 2024-02-17 20:02:02.421997 reflex-0.5.0a3/reflex/components/el/elements/typography.py
+-rw-r--r--   0        0        0    89115 2024-04-24 19:32:04.312119 reflex-0.5.0a3/reflex/components/el/elements/typography.pyi
+-rw-r--r--   0        0        0       88 2024-02-06 00:51:31.999860 reflex-0.5.0a3/reflex/components/gridjs/__init__.py
+-rw-r--r--   0        0        0     4300 2024-02-06 00:51:32.000048 reflex-0.5.0a3/reflex/components/gridjs/datatable.py
+-rw-r--r--   0        0        0     7053 2024-04-24 19:31:36.593992 reflex-0.5.0a3/reflex/components/gridjs/datatable.pyi
+-rw-r--r--   0        0        0      501 2024-02-06 00:51:32.000350 reflex-0.5.0a3/reflex/components/literals.py
+-rw-r--r--   0        0        0       73 2024-02-07 21:48:43.293647 reflex-0.5.0a3/reflex/components/lucide/__init__.py
+-rw-r--r--   0        0        0    34077 2024-05-09 00:05:27.336308 reflex-0.5.0a3/reflex/components/lucide/icon.py
+-rw-r--r--   0        0        0    37918 2024-05-05 01:15:24.056110 reflex-0.5.0a3/reflex/components/lucide/icon.pyi
+-rw-r--r--   0        0        0       87 2024-02-06 00:51:32.000748 reflex-0.5.0a3/reflex/components/markdown/__init__.py
+-rw-r--r--   0        0        0    10867 2024-05-09 00:05:27.336466 reflex-0.5.0a3/reflex/components/markdown/markdown.py
+-rw-r--r--   0        0        0     5100 2024-05-09 00:05:27.336616 reflex-0.5.0a3/reflex/components/markdown/markdown.pyi
+-rw-r--r--   0        0        0       44 2024-02-06 00:51:32.001397 reflex-0.5.0a3/reflex/components/media/__init__.py
+-rw-r--r--   0        0        0      102 2024-02-06 00:51:32.001492 reflex-0.5.0a3/reflex/components/media/icon.py
+-rw-r--r--   0        0        0       79 2024-02-06 00:51:32.001557 reflex-0.5.0a3/reflex/components/moment/__init__.py
+-rw-r--r--   0        0        0     3925 2024-02-06 00:51:32.001623 reflex-0.5.0a3/reflex/components/moment/moment.py
+-rw-r--r--   0        0        0     6870 2024-04-24 19:31:51.190910 reflex-0.5.0a3/reflex/components/moment/moment.pyi
+-rw-r--r--   0        0        0      239 2024-02-06 00:51:32.001924 reflex-0.5.0a3/reflex/components/next/__init__.py
+-rw-r--r--   0        0        0      189 2024-01-08 22:19:50.677879 reflex-0.5.0a3/reflex/components/next/base.py
+-rw-r--r--   0        0        0     3233 2024-04-24 19:31:43.822514 reflex-0.5.0a3/reflex/components/next/base.pyi
+-rw-r--r--   0        0        0     3831 2024-01-08 22:19:50.678013 reflex-0.5.0a3/reflex/components/next/image.py
+-rw-r--r--   0        0        0     5795 2024-04-24 19:31:33.244479 reflex-0.5.0a3/reflex/components/next/image.pyi
+-rw-r--r--   0        0        0      503 2024-02-06 00:51:32.002304 reflex-0.5.0a3/reflex/components/next/link.py
+-rw-r--r--   0        0        0     3461 2024-04-24 19:31:15.603661 reflex-0.5.0a3/reflex/components/next/link.pyi
+-rw-r--r--   0        0        0      730 2024-01-08 22:19:50.678316 reflex-0.5.0a3/reflex/components/next/video.py
+-rw-r--r--   0        0        0     3429 2024-04-24 19:31:46.249185 reflex-0.5.0a3/reflex/components/next/video.pyi
+-rw-r--r--   0        0        0       77 2024-02-06 00:51:32.002529 reflex-0.5.0a3/reflex/components/plotly/__init__.py
+-rw-r--r--   0        0        0      964 2024-03-20 23:54:55.846069 reflex-0.5.0a3/reflex/components/plotly/plotly.py
+-rw-r--r--   0        0        0     6865 2024-04-24 19:31:24.224015 reflex-0.5.0a3/reflex/components/plotly/plotly.pyi
+-rw-r--r--   0        0        0      112 2024-02-17 20:02:02.423429 reflex-0.5.0a3/reflex/components/radix/__init__.py
+-rw-r--r--   0        0        0      214 2024-02-17 20:02:02.423526 reflex-0.5.0a3/reflex/components/radix/primitives/__init__.py
+-rw-r--r--   0        0        0    16159 2024-05-13 23:05:40.957488 reflex-0.5.0a3/reflex/components/radix/primitives/accordion.py
+-rw-r--r--   0        0        0    37999 2024-05-11 03:29:42.708959 reflex-0.5.0a3/reflex/components/radix/primitives/accordion.pyi
+-rw-r--r--   0        0        0      869 2024-02-06 00:51:32.004050 reflex-0.5.0a3/reflex/components/radix/primitives/base.py
+-rw-r--r--   0        0        0     6478 2024-04-24 19:31:44.069976 reflex-0.5.0a3/reflex/components/radix/primitives/base.pyi
+-rw-r--r--   0        0        0     8660 2024-03-20 23:54:55.846917 reflex-0.5.0a3/reflex/components/radix/primitives/drawer.py
+-rw-r--r--   0        0        0    34484 2024-04-24 19:32:02.551316 reflex-0.5.0a3/reflex/components/radix/primitives/drawer.pyi
+-rw-r--r--   0        0        0     4964 2024-05-11 03:29:42.709212 reflex-0.5.0a3/reflex/components/radix/primitives/form.py
+-rw-r--r--   0        0        0    48138 2024-05-07 15:33:05.684481 reflex-0.5.0a3/reflex/components/radix/primitives/form.pyi
+-rw-r--r--   0        0        0     4160 2024-05-07 15:33:05.684814 reflex-0.5.0a3/reflex/components/radix/primitives/progress.py
+-rw-r--r--   0        0        0    22874 2024-05-07 15:33:05.685122 reflex-0.5.0a3/reflex/components/radix/primitives/progress.pyi
+-rw-r--r--   0        0        0     5198 2024-05-07 15:33:05.685275 reflex-0.5.0a3/reflex/components/radix/primitives/slider.py
+-rw-r--r--   0        0        0    16877 2024-05-07 15:33:05.685394 reflex-0.5.0a3/reflex/components/radix/primitives/slider.pyi
+-rw-r--r--   0        0        0      292 2024-02-17 20:02:02.426799 reflex-0.5.0a3/reflex/components/radix/themes/__init__.py
+-rw-r--r--   0        0        0     8294 2024-04-26 18:47:21.875701 reflex-0.5.0a3/reflex/components/radix/themes/base.py
+-rw-r--r--   0        0        0    26971 2024-05-05 01:15:24.056523 reflex-0.5.0a3/reflex/components/radix/themes/base.pyi
+-rw-r--r--   0        0        0     5543 2024-05-13 23:05:41.231938 reflex-0.5.0a3/reflex/components/radix/themes/color_mode.py
+-rw-r--r--   0        0        0    22145 2024-05-13 23:05:41.232088 reflex-0.5.0a3/reflex/components/radix/themes/color_mode.pyi
+-rw-r--r--   0        0        0     2440 2024-05-09 00:05:27.336999 reflex-0.5.0a3/reflex/components/radix/themes/components/__init__.py
+-rw-r--r--   0        0        0     3267 2024-03-20 23:54:55.849529 reflex-0.5.0a3/reflex/components/radix/themes/components/alert_dialog.py
+-rw-r--r--   0        0        0    24434 2024-04-24 19:31:57.706076 reflex-0.5.0a3/reflex/components/radix/themes/components/alert_dialog.pyi
+-rw-r--r--   0        0        0      400 2024-02-17 20:02:02.428862 reflex-0.5.0a3/reflex/components/radix/themes/components/aspect_ratio.py
+-rw-r--r--   0        0        0     3640 2024-04-24 19:31:17.911074 reflex-0.5.0a3/reflex/components/radix/themes/components/aspect_ratio.pyi
+-rw-r--r--   0        0        0      989 2024-03-20 23:54:55.849841 reflex-0.5.0a3/reflex/components/radix/themes/components/avatar.py
+-rw-r--r--   0        0        0     6562 2024-04-24 19:31:52.410239 reflex-0.5.0a3/reflex/components/radix/themes/components/avatar.pyi
+-rw-r--r--   0        0        0      821 2024-04-26 18:47:21.876311 reflex-0.5.0a3/reflex/components/radix/themes/components/badge.py
+-rw-r--r--   0        0        0     9347 2024-04-26 18:47:21.876509 reflex-0.5.0a3/reflex/components/radix/themes/components/badge.pyi
+-rw-r--r--   0        0        0     1125 2024-04-26 18:47:21.876620 reflex-0.5.0a3/reflex/components/radix/themes/components/button.py
+-rw-r--r--   0        0        0    11939 2024-04-26 18:47:21.876761 reflex-0.5.0a3/reflex/components/radix/themes/components/button.pyi
+-rw-r--r--   0        0        0     2378 2024-03-20 23:54:55.850376 reflex-0.5.0a3/reflex/components/radix/themes/components/callout.py
+-rw-r--r--   0        0        0    38710 2024-04-24 19:32:02.594947 reflex-0.5.0a3/reflex/components/radix/themes/components/callout.pyi
+-rw-r--r--   0        0        0      659 2024-02-17 20:02:02.430724 reflex-0.5.0a3/reflex/components/radix/themes/components/card.py
+-rw-r--r--   0        0        0     7200 2024-04-24 19:31:48.002992 reflex-0.5.0a3/reflex/components/radix/themes/components/card.pyi
+-rw-r--r--   0        0        0     4679 2024-03-20 23:54:55.851297 reflex-0.5.0a3/reflex/components/radix/themes/components/checkbox.py
+-rw-r--r--   0        0        0    20877 2024-04-24 19:32:01.819836 reflex-0.5.0a3/reflex/components/radix/themes/components/checkbox.pyi
+-rw-r--r--   0        0        0     1301 2024-04-26 18:47:21.876837 reflex-0.5.0a3/reflex/components/radix/themes/components/checkbox_cards.py
+-rw-r--r--   0        0        0     9591 2024-04-26 18:47:21.876955 reflex-0.5.0a3/reflex/components/radix/themes/components/checkbox_cards.pyi
+-rw-r--r--   0        0        0     1024 2024-04-26 18:47:21.877018 reflex-0.5.0a3/reflex/components/radix/themes/components/checkbox_group.py
+-rw-r--r--   0        0        0     9012 2024-04-26 18:47:21.877125 reflex-0.5.0a3/reflex/components/radix/themes/components/checkbox_group.pyi
+-rw-r--r--   0        0        0     5049 2024-03-20 23:54:55.852012 reflex-0.5.0a3/reflex/components/radix/themes/components/context_menu.py
+-rw-r--r--   0        0        0    31192 2024-04-24 19:32:03.158519 reflex-0.5.0a3/reflex/components/radix/themes/components/context_menu.pyi
+-rw-r--r--   0        0        0     1508 2024-04-26 18:47:21.877372 reflex-0.5.0a3/reflex/components/radix/themes/components/data_list.py
+-rw-r--r--   0        0        0    15403 2024-04-26 18:47:21.877634 reflex-0.5.0a3/reflex/components/radix/themes/components/data_list.pyi
+-rw-r--r--   0        0        0     2600 2024-03-20 23:54:55.852519 reflex-0.5.0a3/reflex/components/radix/themes/components/dialog.py
+-rw-r--r--   0        0        0    24895 2024-04-24 19:32:02.097223 reflex-0.5.0a3/reflex/components/radix/themes/components/dialog.pyi
+-rw-r--r--   0        0        0    11256 2024-03-20 23:54:55.852973 reflex-0.5.0a3/reflex/components/radix/themes/components/dropdown_menu.py
+-rw-r--r--   0        0        0    37901 2024-04-24 19:32:02.303816 reflex-0.5.0a3/reflex/components/radix/themes/components/dropdown_menu.pyi
+-rw-r--r--   0        0        0     2405 2024-03-20 23:54:55.853285 reflex-0.5.0a3/reflex/components/radix/themes/components/hover_card.py
+-rw-r--r--   0        0        0    17744 2024-04-24 19:31:56.396802 reflex-0.5.0a3/reflex/components/radix/themes/components/hover_card.pyi
+-rw-r--r--   0        0        0     2940 2024-05-09 00:05:27.337231 reflex-0.5.0a3/reflex/components/radix/themes/components/icon_button.py
+-rw-r--r--   0        0        0    12126 2024-05-07 15:33:05.685671 reflex-0.5.0a3/reflex/components/radix/themes/components/icon_button.pyi
+-rw-r--r--   0        0        0     1015 2024-03-20 23:54:55.853906 reflex-0.5.0a3/reflex/components/radix/themes/components/inset.py
+-rw-r--r--   0        0        0     7889 2024-04-24 19:31:39.003439 reflex-0.5.0a3/reflex/components/radix/themes/components/inset.pyi
+-rw-r--r--   0        0        0     3177 2024-03-20 23:54:55.854041 reflex-0.5.0a3/reflex/components/radix/themes/components/popover.py
+-rw-r--r--   0        0        0    17404 2024-04-24 19:32:01.605821 reflex-0.5.0a3/reflex/components/radix/themes/components/popover.pyi
+-rw-r--r--   0        0        0     1598 2024-05-09 00:05:27.337432 reflex-0.5.0a3/reflex/components/radix/themes/components/progress.py
+-rw-r--r--   0        0        0     6676 2024-05-09 00:05:27.337586 reflex-0.5.0a3/reflex/components/radix/themes/components/progress.pyi
+-rw-r--r--   0        0        0      762 2024-04-26 18:47:21.878308 reflex-0.5.0a3/reflex/components/radix/themes/components/radio.py
+-rw-r--r--   0        0        0     5924 2024-04-26 18:47:21.878424 reflex-0.5.0a3/reflex/components/radix/themes/components/radio.pyi
+-rw-r--r--   0        0        0     1250 2024-04-26 18:47:21.878499 reflex-0.5.0a3/reflex/components/radix/themes/components/radio_cards.py
+-rw-r--r--   0        0        0     9561 2024-04-26 18:47:21.878615 reflex-0.5.0a3/reflex/components/radix/themes/components/radio_cards.pyi
+-rw-r--r--   0        0        0     6233 2024-04-24 21:16:40.838796 reflex-0.5.0a3/reflex/components/radix/themes/components/radio_group.py
+-rw-r--r--   0        0        0    24106 2024-04-24 19:32:02.212695 reflex-0.5.0a3/reflex/components/radix/themes/components/radio_group.pyi
+-rw-r--r--   0        0        0      920 2024-03-20 23:54:55.855386 reflex-0.5.0a3/reflex/components/radix/themes/components/scroll_area.py
+-rw-r--r--   0        0        0     4427 2024-04-24 19:31:54.699499 reflex-0.5.0a3/reflex/components/radix/themes/components/scroll_area.pyi
+-rw-r--r--   0        0        0     1292 2024-04-26 18:47:21.878708 reflex-0.5.0a3/reflex/components/radix/themes/components/segmented_control.py
+-rw-r--r--   0        0        0     9507 2024-04-26 18:47:21.878829 reflex-0.5.0a3/reflex/components/radix/themes/components/segmented_control.pyi
+-rw-r--r--   0        0        0     8028 2024-04-05 17:14:14.462095 reflex-0.5.0a3/reflex/components/radix/themes/components/select.py
+-rw-r--r--   0        0        0    45123 2024-04-24 19:32:01.973018 reflex-0.5.0a3/reflex/components/radix/themes/components/select.pyi
+-rw-r--r--   0        0        0      868 2024-03-20 23:54:55.856979 reflex-0.5.0a3/reflex/components/radix/themes/components/separator.py
+-rw-r--r--   0        0        0     6078 2024-04-24 19:32:00.501335 reflex-0.5.0a3/reflex/components/radix/themes/components/separator.pyi
+-rw-r--r--   0        0        0      643 2024-04-26 18:47:21.878906 reflex-0.5.0a3/reflex/components/radix/themes/components/skeleton.py
+-rw-r--r--   0        0        0     4289 2024-04-26 18:47:21.879004 reflex-0.5.0a3/reflex/components/radix/themes/components/skeleton.pyi
+-rw-r--r--   0        0        0     3234 2024-03-20 23:54:55.857144 reflex-0.5.0a3/reflex/components/radix/themes/components/slider.py
+-rw-r--r--   0        0        0     8162 2024-04-24 19:31:52.441948 reflex-0.5.0a3/reflex/components/radix/themes/components/slider.pyi
+-rw-r--r--   0        0        0      431 2024-04-26 18:47:21.879090 reflex-0.5.0a3/reflex/components/radix/themes/components/spinner.py
+-rw-r--r--   0        0        0     3845 2024-04-26 18:47:21.879165 reflex-0.5.0a3/reflex/components/radix/themes/components/spinner.pyi
+-rw-r--r--   0        0        0     1976 2024-02-17 20:02:02.440152 reflex-0.5.0a3/reflex/components/radix/themes/components/switch.py
+-rw-r--r--   0        0        0     7404 2024-04-24 19:31:46.185370 reflex-0.5.0a3/reflex/components/radix/themes/components/switch.pyi
+-rw-r--r--   0        0        0     3111 2024-03-20 23:54:55.857388 reflex-0.5.0a3/reflex/components/radix/themes/components/table.py
+-rw-r--r--   0        0        0    47387 2024-04-24 19:32:03.411460 reflex-0.5.0a3/reflex/components/radix/themes/components/table.pyi
+-rw-r--r--   0        0        0     2986 2024-05-07 15:33:05.685861 reflex-0.5.0a3/reflex/components/radix/themes/components/tabs.py
+-rw-r--r--   0        0        0    19119 2024-05-07 15:33:05.685968 reflex-0.5.0a3/reflex/components/radix/themes/components/tabs.pyi
+-rw-r--r--   0        0        0     3233 2024-02-17 20:02:02.441460 reflex-0.5.0a3/reflex/components/radix/themes/components/text_area.py
+-rw-r--r--   0        0        0    11711 2024-04-24 19:31:45.665204 reflex-0.5.0a3/reflex/components/radix/themes/components/text_area.pyi
+-rw-r--r--   0        0        0     6527 2024-05-09 00:05:27.337867 reflex-0.5.0a3/reflex/components/radix/themes/components/text_field.py
+-rw-r--r--   0        0        0    26637 2024-05-09 00:05:27.338008 reflex-0.5.0a3/reflex/components/radix/themes/components/text_field.pyi
+-rw-r--r--   0        0        0     4465 2024-02-17 20:02:02.442324 reflex-0.5.0a3/reflex/components/radix/themes/components/tooltip.py
+-rw-r--r--   0        0        0     8092 2024-04-24 19:31:32.491941 reflex-0.5.0a3/reflex/components/radix/themes/components/tooltip.pyi
+-rw-r--r--   0        0        0      811 2024-04-04 14:19:59.340548 reflex-0.5.0a3/reflex/components/radix/themes/layout/__init__.py
+-rw-r--r--   0        0        0     1211 2024-04-26 18:47:21.880131 reflex-0.5.0a3/reflex/components/radix/themes/layout/base.py
+-rw-r--r--   0        0        0     7663 2024-04-26 18:47:21.880279 reflex-0.5.0a3/reflex/components/radix/themes/layout/base.pyi
+-rw-r--r--   0        0        0      281 2024-02-07 21:48:43.318485 reflex-0.5.0a3/reflex/components/radix/themes/layout/box.py
+-rw-r--r--   0        0        0     6462 2024-04-24 19:31:52.197501 reflex-0.5.0a3/reflex/components/radix/themes/layout/box.pyi
+-rw-r--r--   0        0        0      509 2024-05-07 15:33:05.686074 reflex-0.5.0a3/reflex/components/radix/themes/layout/center.py
+-rw-r--r--   0        0        0     8271 2024-05-07 15:33:05.686180 reflex-0.5.0a3/reflex/components/radix/themes/layout/center.pyi
+-rw-r--r--   0        0        0     1405 2024-05-05 01:15:24.057627 reflex-0.5.0a3/reflex/components/radix/themes/layout/container.py
+-rw-r--r--   0        0        0     5247 2024-05-05 01:15:24.057873 reflex-0.5.0a3/reflex/components/radix/themes/layout/container.pyi
+-rw-r--r--   0        0        0     1374 2024-03-20 23:54:55.859776 reflex-0.5.0a3/reflex/components/radix/themes/layout/flex.py
+-rw-r--r--   0        0        0     8501 2024-04-24 19:31:47.609497 reflex-0.5.0a3/reflex/components/radix/themes/layout/flex.pyi
+-rw-r--r--   0        0        0     1498 2024-03-20 23:54:55.860131 reflex-0.5.0a3/reflex/components/radix/themes/layout/grid.py
+-rw-r--r--   0        0        0     8907 2024-04-24 19:31:44.336304 reflex-0.5.0a3/reflex/components/radix/themes/layout/grid.pyi
+-rw-r--r--   0        0        0     4991 2024-05-07 15:33:05.686298 reflex-0.5.0a3/reflex/components/radix/themes/layout/list.py
+-rw-r--r--   0        0        0    28927 2024-05-07 15:33:05.686398 reflex-0.5.0a3/reflex/components/radix/themes/layout/list.pyi
+-rw-r--r--   0        0        0      458 2024-02-07 21:48:43.320250 reflex-0.5.0a3/reflex/components/radix/themes/layout/section.py
+-rw-r--r--   0        0        0     6758 2024-04-24 19:31:48.032806 reflex-0.5.0a3/reflex/components/radix/themes/layout/section.pyi
+-rw-r--r--   0        0        0      492 2024-05-07 15:33:05.686501 reflex-0.5.0a3/reflex/components/radix/themes/layout/spacer.py
+-rw-r--r--   0        0        0     8271 2024-05-07 15:33:05.686608 reflex-0.5.0a3/reflex/components/radix/themes/layout/spacer.pyi
+-rw-r--r--   0        0        0     1522 2024-05-05 01:15:24.058360 reflex-0.5.0a3/reflex/components/radix/themes/layout/stack.py
+-rw-r--r--   0        0        0    22132 2024-05-05 01:15:24.058618 reflex-0.5.0a3/reflex/components/radix/themes/layout/stack.pyi
+-rw-r--r--   0        0        0      343 2024-02-17 20:02:02.446123 reflex-0.5.0a3/reflex/components/radix/themes/typography/__init__.py
+-rw-r--r--   0        0        0      408 2024-01-08 22:19:50.686081 reflex-0.5.0a3/reflex/components/radix/themes/typography/base.py
+-rw-r--r--   0        0        0      799 2024-02-07 21:48:43.321231 reflex-0.5.0a3/reflex/components/radix/themes/typography/blockquote.py
+-rw-r--r--   0        0        0     9316 2024-04-24 19:31:18.815043 reflex-0.5.0a3/reflex/components/radix/themes/typography/blockquote.pyi
+-rw-r--r--   0        0        0      909 2024-02-07 21:48:43.321463 reflex-0.5.0a3/reflex/components/radix/themes/typography/code.py
+-rw-r--r--   0        0        0     9513 2024-04-24 19:31:42.716182 reflex-0.5.0a3/reflex/components/radix/themes/typography/code.pyi
+-rw-r--r--   0        0        0     1324 2024-02-07 21:48:43.322172 reflex-0.5.0a3/reflex/components/radix/themes/typography/heading.py
+-rw-r--r--   0        0        0    10106 2024-04-24 19:31:48.004994 reflex-0.5.0a3/reflex/components/radix/themes/typography/heading.pyi
+-rw-r--r--   0        0        0     3291 2024-05-05 01:15:24.058911 reflex-0.5.0a3/reflex/components/radix/themes/typography/link.py
+-rw-r--r--   0        0        0    12144 2024-05-05 01:15:24.059174 reflex-0.5.0a3/reflex/components/radix/themes/typography/link.pyi
+-rw-r--r--   0        0        0     2604 2024-03-20 23:54:55.863112 reflex-0.5.0a3/reflex/components/radix/themes/typography/text.py
+-rw-r--r--   0        0        0    57238 2024-04-24 19:32:03.568126 reflex-0.5.0a3/reflex/components/radix/themes/typography/text.pyi
+-rw-r--r--   0        0        0      144 2024-02-06 00:51:32.026767 reflex-0.5.0a3/reflex/components/react_player/__init__.py
+-rw-r--r--   0        0        0      185 2024-02-06 00:51:32.026827 reflex-0.5.0a3/reflex/components/react_player/audio.py
+-rw-r--r--   0        0        0     4327 2024-04-24 19:31:20.559612 reflex-0.5.0a3/reflex/components/react_player/audio.pyi
+-rw-r--r--   0        0        0     1087 2024-02-06 00:51:32.027069 reflex-0.5.0a3/reflex/components/react_player/react_player.py
+-rw-r--r--   0        0        0     4354 2024-04-24 19:31:40.833679 reflex-0.5.0a3/reflex/components/react_player/react_player.pyi
+-rw-r--r--   0        0        0      185 2024-02-06 00:51:32.027295 reflex-0.5.0a3/reflex/components/react_player/video.py
+-rw-r--r--   0        0        0     4327 2024-04-24 19:31:23.657166 reflex-0.5.0a3/reflex/components/react_player/video.pyi
+-rw-r--r--   0        0        0     2373 2024-02-06 00:51:32.027723 reflex-0.5.0a3/reflex/components/recharts/__init__.py
+-rw-r--r--   0        0        0    19595 2024-02-06 00:51:32.027828 reflex-0.5.0a3/reflex/components/recharts/cartesian.py
+-rw-r--r--   0        0        0    84151 2024-04-24 19:32:04.125732 reflex-0.5.0a3/reflex/components/recharts/cartesian.pyi
+-rw-r--r--   0        0        0    18493 2024-02-06 00:51:32.028086 reflex-0.5.0a3/reflex/components/recharts/charts.py
+-rw-r--r--   0        0        0    48757 2024-04-24 19:32:04.230664 reflex-0.5.0a3/reflex/components/recharts/charts.pyi
+-rw-r--r--   0        0        0     5624 2024-04-25 02:07:40.442483 reflex-0.5.0a3/reflex/components/recharts/general.py
+-rw-r--r--   0        0        0    22787 2024-04-24 19:31:57.383382 reflex-0.5.0a3/reflex/components/recharts/general.pyi
+-rw-r--r--   0        0        0    10410 2024-02-06 00:51:32.028623 reflex-0.5.0a3/reflex/components/recharts/polar.py
+-rw-r--r--   0        0        0    24326 2024-04-24 19:32:02.075893 reflex-0.5.0a3/reflex/components/recharts/polar.pyi
+-rw-r--r--   0        0        0     2870 2024-02-06 00:51:32.028787 reflex-0.5.0a3/reflex/components/recharts/recharts.py
+-rw-r--r--   0        0        0     8535 2024-04-24 19:31:59.348537 reflex-0.5.0a3/reflex/components/recharts/recharts.pyi
+-rw-r--r--   0        0        0       68 2024-05-05 01:15:24.059268 reflex-0.5.0a3/reflex/components/sonner/__init__.py
+-rw-r--r--   0        0        0     7638 2024-05-05 01:15:24.059336 reflex-0.5.0a3/reflex/components/sonner/toast.py
+-rw-r--r--   0        0        0     7635 2024-05-05 01:15:24.059415 reflex-0.5.0a3/reflex/components/sonner/toast.pyi
+-rw-r--r--   0        0        0      109 2024-02-06 00:51:32.028942 reflex-0.5.0a3/reflex/components/suneditor/__init__.py
+-rw-r--r--   0        0        0     7360 2024-02-06 00:51:32.029131 reflex-0.5.0a3/reflex/components/suneditor/editor.py
+-rw-r--r--   0        0        0    10330 2024-04-24 19:32:02.124688 reflex-0.5.0a3/reflex/components/suneditor/editor.pyi
+-rw-r--r--   0        0        0      152 2024-02-06 00:51:32.029339 reflex-0.5.0a3/reflex/components/tags/__init__.py
+-rw-r--r--   0        0        0      447 2023-07-20 22:42:41.717618 reflex-0.5.0a3/reflex/components/tags/cond_tag.py
+-rw-r--r--   0        0        0     3927 2024-05-09 06:53:37.971823 reflex-0.5.0a3/reflex/components/tags/iter_tag.py
+-rw-r--r--   0        0        0      387 2024-02-06 00:51:32.029522 reflex-0.5.0a3/reflex/components/tags/match_tag.py
+-rw-r--r--   0        0        0     2778 2024-03-20 23:54:55.863973 reflex-0.5.0a3/reflex/components/tags/tag.py
+-rw-r--r--   0        0        0      587 2023-07-20 22:42:41.717805 reflex-0.5.0a3/reflex/components/tags/tagless.py
+-rw-r--r--   0        0        0    10673 2024-05-09 00:05:27.338296 reflex-0.5.0a3/reflex/config.py
+-rw-r--r--   0        0        0     3318 2024-04-05 17:14:06.329003 reflex-0.5.0a3/reflex/config.pyi
+-rw-r--r--   0        0        0     2036 2024-05-07 15:33:05.687073 reflex-0.5.0a3/reflex/constants/__init__.py
+-rw-r--r--   0        0        0     5640 2024-05-07 15:33:05.687194 reflex-0.5.0a3/reflex/constants/base.py
+-rw-r--r--   0        0        0     2980 2024-04-24 19:34:30.973419 reflex-0.5.0a3/reflex/constants/base.pyi
+-rw-r--r--   0        0        0     1625 2024-05-07 15:33:05.687387 reflex-0.5.0a3/reflex/constants/colors.py
+-rw-r--r--   0        0        0     4207 2024-04-12 01:14:12.277724 reflex-0.5.0a3/reflex/constants/compiler.py
+-rw-r--r--   0        0        0     1331 2024-01-08 22:19:50.692361 reflex-0.5.0a3/reflex/constants/config.py
+-rw-r--r--   0        0        0     1268 2024-03-20 23:54:55.865280 reflex-0.5.0a3/reflex/constants/custom_components.py
+-rw-r--r--   0        0        0     2668 2024-03-20 00:01:07.211135 reflex-0.5.0a3/reflex/constants/event.py
+-rw-r--r--   0        0        0     3419 2024-05-05 01:15:24.059627 reflex-0.5.0a3/reflex/constants/installer.py
+-rw-r--r--   0        0        0     2144 2024-05-05 01:15:24.059871 reflex-0.5.0a3/reflex/constants/route.py
+-rw-r--r--   0        0        0      636 2024-02-06 00:51:32.030238 reflex-0.5.0a3/reflex/constants/style.py
+-rw-r--r--   0        0        0       36 2024-03-20 23:54:55.865552 reflex-0.5.0a3/reflex/custom_components/__init__.py
+-rw-r--r--   0        0        0    32298 2024-05-13 23:05:41.048157 reflex-0.5.0a3/reflex/custom_components/custom_components.py
+-rw-r--r--   0        0        0    27893 2024-05-05 01:15:24.060128 reflex-0.5.0a3/reflex/event.py
+-rw-r--r--   0        0        0      608 2024-05-09 00:05:27.338786 reflex-0.5.0a3/reflex/experimental/__init__.py
+-rw-r--r--   0        0        0     2196 2024-04-24 21:16:40.840090 reflex-0.5.0a3/reflex/experimental/hooks.py
+-rw-r--r--   0        0        0     7234 2024-05-07 15:33:05.687514 reflex-0.5.0a3/reflex/experimental/layout.py
+-rw-r--r--   0        0        0      281 2024-04-12 01:14:12.278217 reflex-0.5.0a3/reflex/experimental/misc.py
+-rw-r--r--   0        0        0      111 2023-07-20 22:42:41.719277 reflex-0.5.0a3/reflex/middleware/__init__.py
+-rw-r--r--   0        0        0     1484 2024-03-28 17:56:29.082526 reflex-0.5.0a3/reflex/middleware/hydrate_middleware.py
+-rw-r--r--   0        0        0     1169 2023-12-01 04:51:31.116521 reflex-0.5.0a3/reflex/middleware/middleware.py
+-rw-r--r--   0        0        0    13227 2024-05-09 00:05:27.338971 reflex-0.5.0a3/reflex/model.py
+-rw-r--r--   0        0        0     2077 2024-04-24 21:16:40.840737 reflex-0.5.0a3/reflex/page.py
+-rw-r--r--   0        0        0    17826 2024-05-05 01:15:24.060260 reflex-0.5.0a3/reflex/reflex.py
+-rw-r--r--   0        0        0     4198 2024-05-05 01:15:24.060365 reflex-0.5.0a3/reflex/route.py
+-rw-r--r--   0        0        0   105748 2024-05-09 00:05:27.339322 reflex-0.5.0a3/reflex/state.py
+-rw-r--r--   0        0        0     9405 2024-05-11 03:29:42.709528 reflex-0.5.0a3/reflex/style.py
+-rw-r--r--   0        0        0    30743 2024-05-07 15:33:05.688166 reflex-0.5.0a3/reflex/testing.py
+-rw-r--r--   0        0        0       24 2023-11-09 03:24:59.510665 reflex-0.5.0a3/reflex/utils/__init__.py
+-rw-r--r--   0        0        0     8573 2024-02-06 00:51:32.031946 reflex-0.5.0a3/reflex/utils/build.py
+-rw-r--r--   0        0        0     1255 2024-04-12 01:14:12.279414 reflex-0.5.0a3/reflex/utils/compat.py
+-rw-r--r--   0        0        0     5182 2024-04-24 21:16:40.841356 reflex-0.5.0a3/reflex/utils/console.py
+-rw-r--r--   0        0        0      504 2024-02-06 00:51:32.032065 reflex-0.5.0a3/reflex/utils/exceptions.py
+-rw-r--r--   0        0        0    10406 2024-05-07 15:33:05.688300 reflex-0.5.0a3/reflex/utils/exec.py
+-rw-r--r--   0        0        0     2270 2024-04-12 01:14:12.279905 reflex-0.5.0a3/reflex/utils/export.py
+-rw-r--r--   0        0        0    22652 2024-04-24 21:16:40.841498 reflex-0.5.0a3/reflex/utils/format.py
+-rw-r--r--   0        0        0     2309 2024-04-24 21:16:40.841612 reflex-0.5.0a3/reflex/utils/imports.py
+-rw-r--r--   0        0        0     4737 2024-02-06 00:51:32.033457 reflex-0.5.0a3/reflex/utils/path_ops.py
+-rw-r--r--   0        0        0    51212 2024-05-09 00:05:27.339607 reflex-0.5.0a3/reflex/utils/prerequisites.py
+-rw-r--r--   0        0        0    11242 2024-05-07 15:33:05.688585 reflex-0.5.0a3/reflex/utils/processes.py
+-rw-r--r--   0        0        0    30637 2024-05-05 01:15:24.061383 reflex-0.5.0a3/reflex/utils/pyi_generator.py
+-rw-r--r--   0        0        0     9037 2024-04-24 21:16:40.842319 reflex-0.5.0a3/reflex/utils/serializers.py
+-rw-r--r--   0        0        0     4688 2024-05-07 15:33:05.688896 reflex-0.5.0a3/reflex/utils/telemetry.py
+-rw-r--r--   0        0        0    14842 2024-05-09 00:05:27.339984 reflex-0.5.0a3/reflex/utils/types.py
+-rw-r--r--   0        0        0     2609 2023-10-22 18:57:13.223189 reflex-0.5.0a3/reflex/utils/watch.py
+-rw-r--r--   0        0        0    67317 2024-04-25 16:52:48.845338 reflex-0.5.0a3/reflex/vars.py
+-rw-r--r--   0        0        0     5583 2024-04-04 14:57:26.401034 reflex-0.5.0a3/reflex/vars.pyi
+-rw-r--r--   0        0        0    12089 1970-01-01 00:00:00.000000 reflex-0.5.0a3/PKG-INFO
```

### Comparing `reflex-0.5.0a2/LICENSE` & `reflex-0.5.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/README.md` & `reflex-0.5.0a3/README.md`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/pyproject.toml` & `reflex-0.5.0a3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reflex"
-version = "0.5.0a2"
+version = "0.5.0a3"
 description = "Web apps in pure Python."
 license = "Apache-2.0"
 authors = [
     "Nikhil Rao <nikhil@reflex.dev>",
     "Alek Petuskey <alek@reflex.dev>",
     "Masen Furer <masen@reflex.dev>",
     "Elijah Ahianyo <elijah@reflex.dev>",
```

### Comparing `reflex-0.5.0a2/reflex/.templates/apps/blank/assets/favicon.ico` & `reflex-0.5.0a3/reflex/.templates/apps/blank/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/apps/blank/code/blank.py` & `reflex-0.5.0a3/reflex/.templates/apps/blank/code/blank.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/apps/demo/assets/favicon.ico` & `reflex-0.5.0a3/reflex/.templates/apps/demo/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/apps/demo/assets/github.svg` & `reflex-0.5.0a3/reflex/.templates/apps/demo/assets/github.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/apps/demo/assets/icon.svg` & `reflex-0.5.0a3/reflex/.templates/apps/demo/assets/icon.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/apps/demo/assets/logo.svg` & `reflex-0.5.0a3/reflex/.templates/apps/demo/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/apps/demo/assets/paneleft.svg` & `reflex-0.5.0a3/reflex/.templates/apps/demo/assets/paneleft.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/apps/demo/code/demo.py` & `reflex-0.5.0a3/reflex/.templates/apps/demo/code/demo.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                 rx.chakra.menu_item(
                     rx.chakra.link(
                         "About", href="https://github.com/reflex-dev", width="100%"
                     )
                 ),
                 rx.chakra.menu_item(
                     rx.chakra.link(
-                        "Contact", href="mailto:founders@=reflex.dev", width="100%"
+                        "Contact", href="mailto:founders@reflex.dev", width="100%"
                     )
                 ),
             ),
         ),
         position="fixed",
         right="1.5em",
         top="1.5em",
```

### Comparing `reflex-0.5.0a2/reflex/.templates/apps/demo/code/pages/chatapp.py` & `reflex-0.5.0a3/reflex/.templates/apps/demo/code/pages/chatapp.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/apps/demo/code/pages/datatable.py` & `reflex-0.5.0a3/reflex/.templates/apps/demo/code/pages/datatable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/apps/demo/code/pages/forms.py` & `reflex-0.5.0a3/reflex/.templates/apps/demo/code/pages/forms.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/apps/demo/code/pages/graphing.py` & `reflex-0.5.0a3/reflex/.templates/apps/demo/code/pages/graphing.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/apps/demo/code/pages/home.py` & `reflex-0.5.0a3/reflex/.templates/apps/demo/code/pages/home.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/apps/demo/code/sidebar.py` & `reflex-0.5.0a3/reflex/.templates/apps/demo/code/sidebar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/apps/demo/code/states/form_state.py` & `reflex-0.5.0a3/reflex/.templates/apps/demo/code/states/form_state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/apps/demo/code/states/pie_state.py` & `reflex-0.5.0a3/reflex/.templates/apps/demo/code/states/pie_state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/apps/demo/code/styles.py` & `reflex-0.5.0a3/reflex/.templates/apps/demo/code/styles.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/apps/demo/code/webui/components/chat.py` & `reflex-0.5.0a3/reflex/.templates/apps/demo/code/webui/components/chat.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/apps/demo/code/webui/components/loading_icon.py` & `reflex-0.5.0a3/reflex/.templates/apps/demo/code/webui/components/loading_icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/apps/demo/code/webui/components/modal.py` & `reflex-0.5.0a3/reflex/.templates/apps/demo/code/webui/components/modal.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/apps/demo/code/webui/components/navbar.py` & `reflex-0.5.0a3/reflex/.templates/apps/demo/code/webui/components/navbar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/apps/demo/code/webui/components/sidebar.py` & `reflex-0.5.0a3/reflex/.templates/apps/demo/code/webui/components/sidebar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/apps/demo/code/webui/state.py` & `reflex-0.5.0a3/reflex/.templates/apps/demo/code/webui/state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/apps/demo/code/webui/styles.py` & `reflex-0.5.0a3/reflex/.templates/apps/demo/code/webui/styles.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/jinja/custom_components/demo_app.py.jinja2` & `reflex-0.5.0a3/reflex/.templates/jinja/custom_components/demo_app.py.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/jinja/custom_components/pyproject.toml.jinja2` & `reflex-0.5.0a3/reflex/.templates/jinja/custom_components/pyproject.toml.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/jinja/custom_components/src.py.jinja2` & `reflex-0.5.0a3/reflex/.templates/jinja/custom_components/src.py.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/jinja/web/package.json.jinja2` & `reflex-0.5.0a3/reflex/.templates/jinja/web/package.json.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/jinja/web/pages/_app.js.jinja2` & `reflex-0.5.0a3/reflex/.templates/jinja/web/pages/_app.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/jinja/web/pages/custom_component.js.jinja2` & `reflex-0.5.0a3/reflex/.templates/jinja/web/pages/custom_component.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/jinja/web/pages/utils.js.jinja2` & `reflex-0.5.0a3/reflex/.templates/jinja/web/pages/utils.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/jinja/web/tailwind.config.js.jinja2` & `reflex-0.5.0a3/reflex/.templates/jinja/web/tailwind.config.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/jinja/web/utils/context.js.jinja2` & `reflex-0.5.0a3/reflex/.templates/jinja/web/utils/context.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/web/components/reflex/chakra_color_mode_provider.js` & `reflex-0.5.0a3/reflex/.templates/web/components/reflex/chakra_color_mode_provider.js`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/web/components/reflex/radix_themes_color_mode_provider.js` & `reflex-0.5.0a3/reflex/.templates/web/components/reflex/radix_themes_color_mode_provider.js`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/web/utils/client_side_routing.js` & `reflex-0.5.0a3/reflex/.templates/web/utils/client_side_routing.js`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/web/utils/helpers/dataeditor.js` & `reflex-0.5.0a3/reflex/.templates/web/utils/helpers/dataeditor.js`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/web/utils/helpers/debounce.js` & `reflex-0.5.0a3/reflex/.templates/web/utils/helpers/debounce.js`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/web/utils/helpers/range.js` & `reflex-0.5.0a3/reflex/.templates/web/utils/helpers/range.js`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/web/utils/helpers/throttle.js` & `reflex-0.5.0a3/reflex/.templates/web/utils/helpers/throttle.js`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/.templates/web/utils/state.js` & `reflex-0.5.0a3/reflex/.templates/web/utils/state.js`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/__init__.py` & `reflex-0.5.0a3/reflex/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/__init__.pyi` & `reflex-0.5.0a3/reflex/__init__.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/app.py` & `reflex-0.5.0a3/reflex/app.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/app_module_for_backend.py` & `reflex-0.5.0a3/reflex/app_module_for_backend.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/base.py` & `reflex-0.5.0a3/reflex/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/compiler/compiler.py` & `reflex-0.5.0a3/reflex/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/compiler/templates.py` & `reflex-0.5.0a3/reflex/compiler/templates.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/compiler/utils.py` & `reflex-0.5.0a3/reflex/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/__init__.py` & `reflex-0.5.0a3/reflex/components/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/base/app_wrap.py` & `reflex-0.5.0a3/reflex/components/base/app_wrap.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/base/app_wrap.pyi` & `reflex-0.5.0a3/reflex/components/base/app_wrap.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/base/bare.py` & `reflex-0.5.0a3/reflex/components/base/bare.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/base/body.pyi` & `reflex-0.5.0a3/reflex/components/base/body.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/base/document.py` & `reflex-0.5.0a3/reflex/components/base/document.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/base/document.pyi` & `reflex-0.5.0a3/reflex/components/base/document.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/base/fragment.pyi` & `reflex-0.5.0a3/reflex/components/base/fragment.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/base/head.pyi` & `reflex-0.5.0a3/reflex/components/base/head.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/base/link.py` & `reflex-0.5.0a3/reflex/components/base/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/base/link.pyi` & `reflex-0.5.0a3/reflex/components/base/link.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/base/meta.py` & `reflex-0.5.0a3/reflex/components/base/meta.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/base/meta.pyi` & `reflex-0.5.0a3/reflex/components/base/meta.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/base/script.py` & `reflex-0.5.0a3/reflex/components/base/script.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/base/script.pyi` & `reflex-0.5.0a3/reflex/components/base/script.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/__init__.py` & `reflex-0.5.0a3/reflex/components/chakra/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/base.py` & `reflex-0.5.0a3/reflex/components/chakra/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/base.pyi` & `reflex-0.5.0a3/reflex/components/chakra/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/datadisplay/badge.pyi` & `reflex-0.5.0a3/reflex/components/chakra/datadisplay/badge.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/datadisplay/code.pyi` & `reflex-0.5.0a3/reflex/components/chakra/datadisplay/code.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/datadisplay/divider.py` & `reflex-0.5.0a3/reflex/components/chakra/datadisplay/divider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/datadisplay/divider.pyi` & `reflex-0.5.0a3/reflex/components/chakra/datadisplay/divider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/datadisplay/keyboard_key.pyi` & `reflex-0.5.0a3/reflex/components/chakra/datadisplay/keyboard_key.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/datadisplay/list.py` & `reflex-0.5.0a3/reflex/components/chakra/datadisplay/list.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/datadisplay/list.pyi` & `reflex-0.5.0a3/reflex/components/chakra/datadisplay/list.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/datadisplay/stat.py` & `reflex-0.5.0a3/reflex/components/chakra/datadisplay/stat.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/datadisplay/stat.pyi` & `reflex-0.5.0a3/reflex/components/chakra/datadisplay/stat.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/datadisplay/table.py` & `reflex-0.5.0a3/reflex/components/chakra/datadisplay/table.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/datadisplay/table.pyi` & `reflex-0.5.0a3/reflex/components/chakra/datadisplay/table.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/datadisplay/tag.py` & `reflex-0.5.0a3/reflex/components/chakra/datadisplay/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/datadisplay/tag.pyi` & `reflex-0.5.0a3/reflex/components/chakra/datadisplay/tag.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/disclosure/accordion.py` & `reflex-0.5.0a3/reflex/components/chakra/disclosure/accordion.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/disclosure/accordion.pyi` & `reflex-0.5.0a3/reflex/components/chakra/disclosure/accordion.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/disclosure/tabs.py` & `reflex-0.5.0a3/reflex/components/chakra/disclosure/tabs.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/disclosure/tabs.pyi` & `reflex-0.5.0a3/reflex/components/chakra/disclosure/tabs.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/disclosure/transition.py` & `reflex-0.5.0a3/reflex/components/chakra/disclosure/transition.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/disclosure/transition.pyi` & `reflex-0.5.0a3/reflex/components/chakra/disclosure/transition.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/disclosure/visuallyhidden.pyi` & `reflex-0.5.0a3/reflex/components/chakra/disclosure/visuallyhidden.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/feedback/alert.py` & `reflex-0.5.0a3/reflex/components/chakra/feedback/alert.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/feedback/alert.pyi` & `reflex-0.5.0a3/reflex/components/chakra/feedback/alert.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/feedback/circularprogress.py` & `reflex-0.5.0a3/reflex/components/chakra/feedback/circularprogress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/feedback/circularprogress.pyi` & `reflex-0.5.0a3/reflex/components/chakra/feedback/circularprogress.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/feedback/progress.py` & `reflex-0.5.0a3/reflex/components/chakra/feedback/progress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/feedback/progress.pyi` & `reflex-0.5.0a3/reflex/components/chakra/feedback/progress.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/feedback/skeleton.py` & `reflex-0.5.0a3/reflex/components/chakra/feedback/skeleton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/feedback/skeleton.pyi` & `reflex-0.5.0a3/reflex/components/chakra/feedback/skeleton.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/feedback/spinner.py` & `reflex-0.5.0a3/reflex/components/chakra/feedback/spinner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/feedback/spinner.pyi` & `reflex-0.5.0a3/reflex/components/chakra/feedback/spinner.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/forms/__init__.py` & `reflex-0.5.0a3/reflex/components/chakra/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/forms/button.py` & `reflex-0.5.0a3/reflex/components/chakra/forms/button.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/forms/button.pyi` & `reflex-0.5.0a3/reflex/components/chakra/forms/button.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/forms/checkbox.py` & `reflex-0.5.0a3/reflex/components/chakra/forms/checkbox.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/forms/checkbox.pyi` & `reflex-0.5.0a3/reflex/components/chakra/forms/checkbox.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/forms/colormodeswitch.py` & `reflex-0.5.0a3/reflex/components/chakra/forms/colormodeswitch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/forms/colormodeswitch.pyi` & `reflex-0.5.0a3/reflex/components/chakra/forms/colormodeswitch.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/forms/date_picker.pyi` & `reflex-0.5.0a3/reflex/components/chakra/forms/date_picker.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/forms/date_time_picker.pyi` & `reflex-0.5.0a3/reflex/components/chakra/forms/date_time_picker.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/forms/editable.py` & `reflex-0.5.0a3/reflex/components/chakra/forms/editable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/forms/editable.pyi` & `reflex-0.5.0a3/reflex/components/chakra/forms/editable.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/forms/email.pyi` & `reflex-0.5.0a3/reflex/components/chakra/forms/email.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/forms/form.py` & `reflex-0.5.0a3/reflex/components/chakra/forms/form.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/forms/form.pyi` & `reflex-0.5.0a3/reflex/components/chakra/forms/form.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/forms/iconbutton.py` & `reflex-0.5.0a3/reflex/components/chakra/forms/iconbutton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/forms/iconbutton.pyi` & `reflex-0.5.0a3/reflex/components/chakra/forms/iconbutton.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/forms/input.py` & `reflex-0.5.0a3/reflex/components/chakra/forms/input.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/forms/input.pyi` & `reflex-0.5.0a3/reflex/components/chakra/forms/input.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/forms/multiselect.py` & `reflex-0.5.0a3/reflex/components/chakra/forms/multiselect.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/forms/numberinput.py` & `reflex-0.5.0a3/reflex/components/chakra/forms/numberinput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/forms/numberinput.pyi` & `reflex-0.5.0a3/reflex/components/chakra/forms/numberinput.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/forms/password.pyi` & `reflex-0.5.0a3/reflex/components/chakra/forms/password.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/forms/pininput.py` & `reflex-0.5.0a3/reflex/components/chakra/forms/pininput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/forms/pininput.pyi` & `reflex-0.5.0a3/reflex/components/chakra/forms/pininput.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/forms/radio.py` & `reflex-0.5.0a3/reflex/components/chakra/forms/radio.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/forms/radio.pyi` & `reflex-0.5.0a3/reflex/components/chakra/forms/radio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/forms/rangeslider.py` & `reflex-0.5.0a3/reflex/components/chakra/forms/rangeslider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/forms/rangeslider.pyi` & `reflex-0.5.0a3/reflex/components/chakra/forms/rangeslider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/forms/select.py` & `reflex-0.5.0a3/reflex/components/chakra/forms/select.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/forms/select.pyi` & `reflex-0.5.0a3/reflex/components/chakra/forms/select.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/forms/slider.py` & `reflex-0.5.0a3/reflex/components/chakra/forms/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/forms/slider.pyi` & `reflex-0.5.0a3/reflex/components/chakra/forms/slider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/forms/switch.py` & `reflex-0.5.0a3/reflex/components/chakra/forms/switch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/forms/switch.pyi` & `reflex-0.5.0a3/reflex/components/chakra/forms/switch.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/forms/textarea.py` & `reflex-0.5.0a3/reflex/components/chakra/forms/textarea.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/forms/textarea.pyi` & `reflex-0.5.0a3/reflex/components/chakra/forms/textarea.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/forms/time_picker.pyi` & `reflex-0.5.0a3/reflex/components/chakra/forms/time_picker.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/layout/aspect_ratio.pyi` & `reflex-0.5.0a3/reflex/components/chakra/layout/aspect_ratio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/layout/box.py` & `reflex-0.5.0a3/reflex/components/chakra/layout/box.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/layout/box.pyi` & `reflex-0.5.0a3/reflex/components/chakra/layout/box.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/layout/card.py` & `reflex-0.5.0a3/reflex/components/chakra/layout/card.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/layout/card.pyi` & `reflex-0.5.0a3/reflex/components/chakra/layout/card.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/layout/center.pyi` & `reflex-0.5.0a3/reflex/components/chakra/layout/center.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/layout/container.pyi` & `reflex-0.5.0a3/reflex/components/chakra/layout/container.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/layout/flex.py` & `reflex-0.5.0a3/reflex/components/chakra/layout/flex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/layout/flex.pyi` & `reflex-0.5.0a3/reflex/components/chakra/layout/flex.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/layout/grid.py` & `reflex-0.5.0a3/reflex/components/chakra/layout/grid.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/layout/grid.pyi` & `reflex-0.5.0a3/reflex/components/chakra/layout/grid.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/layout/spacer.pyi` & `reflex-0.5.0a3/reflex/components/chakra/layout/spacer.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/layout/stack.py` & `reflex-0.5.0a3/reflex/components/chakra/layout/stack.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/layout/stack.pyi` & `reflex-0.5.0a3/reflex/components/chakra/layout/stack.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/layout/wrap.py` & `reflex-0.5.0a3/reflex/components/chakra/layout/wrap.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/layout/wrap.pyi` & `reflex-0.5.0a3/reflex/components/chakra/layout/wrap.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/media/avatar.py` & `reflex-0.5.0a3/reflex/components/chakra/media/avatar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/media/avatar.pyi` & `reflex-0.5.0a3/reflex/components/chakra/media/avatar.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/media/icon.py` & `reflex-0.5.0a3/reflex/components/chakra/media/icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/media/icon.pyi` & `reflex-0.5.0a3/reflex/components/chakra/media/icon.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/media/image.py` & `reflex-0.5.0a3/reflex/components/chakra/media/image.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/media/image.pyi` & `reflex-0.5.0a3/reflex/components/chakra/media/image.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/navigation/breadcrumb.py` & `reflex-0.5.0a3/reflex/components/chakra/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/navigation/breadcrumb.pyi` & `reflex-0.5.0a3/reflex/components/chakra/navigation/breadcrumb.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/navigation/link.py` & `reflex-0.5.0a3/reflex/components/chakra/navigation/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/navigation/link.pyi` & `reflex-0.5.0a3/reflex/components/chakra/navigation/link.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/navigation/linkoverlay.py` & `reflex-0.5.0a3/reflex/components/chakra/navigation/linkoverlay.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/navigation/linkoverlay.pyi` & `reflex-0.5.0a3/reflex/components/chakra/navigation/linkoverlay.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/navigation/stepper.py` & `reflex-0.5.0a3/reflex/components/chakra/navigation/stepper.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/navigation/stepper.pyi` & `reflex-0.5.0a3/reflex/components/chakra/navigation/stepper.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/overlay/__init__.py` & `reflex-0.5.0a3/reflex/components/chakra/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/overlay/alertdialog.py` & `reflex-0.5.0a3/reflex/components/chakra/overlay/alertdialog.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/overlay/alertdialog.pyi` & `reflex-0.5.0a3/reflex/components/chakra/overlay/alertdialog.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/overlay/drawer.py` & `reflex-0.5.0a3/reflex/components/chakra/overlay/drawer.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/overlay/drawer.pyi` & `reflex-0.5.0a3/reflex/components/chakra/overlay/drawer.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/overlay/menu.py` & `reflex-0.5.0a3/reflex/components/chakra/overlay/menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/overlay/menu.pyi` & `reflex-0.5.0a3/reflex/components/chakra/overlay/menu.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/overlay/modal.py` & `reflex-0.5.0a3/reflex/components/chakra/overlay/modal.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/overlay/modal.pyi` & `reflex-0.5.0a3/reflex/components/chakra/overlay/modal.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/overlay/popover.py` & `reflex-0.5.0a3/reflex/components/chakra/overlay/popover.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/overlay/popover.pyi` & `reflex-0.5.0a3/reflex/components/chakra/overlay/popover.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/overlay/tooltip.py` & `reflex-0.5.0a3/reflex/components/chakra/overlay/tooltip.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/overlay/tooltip.pyi` & `reflex-0.5.0a3/reflex/components/chakra/overlay/tooltip.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/typography/heading.pyi` & `reflex-0.5.0a3/reflex/components/chakra/typography/heading.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/typography/highlight.py` & `reflex-0.5.0a3/reflex/components/chakra/typography/highlight.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/typography/highlight.pyi` & `reflex-0.5.0a3/reflex/components/chakra/typography/highlight.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/typography/span.pyi` & `reflex-0.5.0a3/reflex/components/chakra/typography/span.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/chakra/typography/text.pyi` & `reflex-0.5.0a3/reflex/components/chakra/typography/text.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/component.py` & `reflex-0.5.0a3/reflex/components/component.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/core/__init__.py` & `reflex-0.5.0a3/reflex/components/core/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/core/banner.py` & `reflex-0.5.0a3/reflex/components/core/banner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/core/banner.pyi` & `reflex-0.5.0a3/reflex/components/core/banner.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/core/client_side_routing.py` & `reflex-0.5.0a3/reflex/components/core/client_side_routing.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/core/client_side_routing.pyi` & `reflex-0.5.0a3/reflex/components/core/client_side_routing.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/core/colors.py` & `reflex-0.5.0a3/reflex/components/core/colors.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/core/cond.py` & `reflex-0.5.0a3/reflex/components/core/cond.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/core/debounce.py` & `reflex-0.5.0a3/reflex/components/core/debounce.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/core/debounce.pyi` & `reflex-0.5.0a3/reflex/components/core/debounce.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/core/foreach.py` & `reflex-0.5.0a3/reflex/components/core/foreach.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/core/html.py` & `reflex-0.5.0a3/reflex/components/core/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/core/html.pyi` & `reflex-0.5.0a3/reflex/components/core/html.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/core/match.py` & `reflex-0.5.0a3/reflex/components/core/match.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/core/responsive.py` & `reflex-0.5.0a3/reflex/components/core/responsive.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/core/upload.py` & `reflex-0.5.0a3/reflex/components/core/upload.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/core/upload.pyi` & `reflex-0.5.0a3/reflex/components/core/upload.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/datadisplay/code.py` & `reflex-0.5.0a3/reflex/components/datadisplay/code.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/datadisplay/code.pyi` & `reflex-0.5.0a3/reflex/components/datadisplay/code.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/datadisplay/dataeditor.py` & `reflex-0.5.0a3/reflex/components/datadisplay/dataeditor.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/datadisplay/dataeditor.pyi` & `reflex-0.5.0a3/reflex/components/datadisplay/dataeditor.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/datadisplay/logo.py` & `reflex-0.5.0a3/reflex/components/datadisplay/logo.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/el/constants/html.py` & `reflex-0.5.0a3/reflex/components/el/constants/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/el/constants/react.py` & `reflex-0.5.0a3/reflex/components/el/constants/react.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/el/constants/reflex.py` & `reflex-0.5.0a3/reflex/components/el/constants/reflex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/el/element.pyi` & `reflex-0.5.0a3/reflex/components/el/element.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/el/elements/__init__.py` & `reflex-0.5.0a3/reflex/components/el/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/el/elements/base.py` & `reflex-0.5.0a3/reflex/components/el/elements/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/el/elements/base.pyi` & `reflex-0.5.0a3/reflex/components/el/elements/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/el/elements/forms.py` & `reflex-0.5.0a3/reflex/components/el/elements/forms.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/el/elements/forms.pyi` & `reflex-0.5.0a3/reflex/components/el/elements/forms.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/el/elements/inline.py` & `reflex-0.5.0a3/reflex/components/el/elements/inline.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/el/elements/inline.pyi` & `reflex-0.5.0a3/reflex/components/el/elements/inline.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/el/elements/media.py` & `reflex-0.5.0a3/reflex/components/el/elements/media.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/el/elements/media.pyi` & `reflex-0.5.0a3/reflex/components/el/elements/media.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/el/elements/metadata.py` & `reflex-0.5.0a3/reflex/components/el/elements/metadata.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/el/elements/metadata.pyi` & `reflex-0.5.0a3/reflex/components/el/elements/metadata.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/el/elements/other.py` & `reflex-0.5.0a3/reflex/components/el/elements/other.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/el/elements/other.pyi` & `reflex-0.5.0a3/reflex/components/el/elements/other.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/el/elements/scripts.py` & `reflex-0.5.0a3/reflex/components/el/elements/scripts.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/el/elements/scripts.pyi` & `reflex-0.5.0a3/reflex/components/el/elements/scripts.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/el/elements/sectioning.py` & `reflex-0.5.0a3/reflex/components/el/elements/sectioning.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/el/elements/sectioning.pyi` & `reflex-0.5.0a3/reflex/components/el/elements/sectioning.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/el/elements/tables.py` & `reflex-0.5.0a3/reflex/components/el/elements/tables.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/el/elements/tables.pyi` & `reflex-0.5.0a3/reflex/components/el/elements/tables.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/el/elements/typography.py` & `reflex-0.5.0a3/reflex/components/el/elements/typography.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/el/elements/typography.pyi` & `reflex-0.5.0a3/reflex/components/el/elements/typography.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/gridjs/datatable.py` & `reflex-0.5.0a3/reflex/components/gridjs/datatable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/gridjs/datatable.pyi` & `reflex-0.5.0a3/reflex/components/gridjs/datatable.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/lucide/icon.py` & `reflex-0.5.0a3/reflex/components/lucide/icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/lucide/icon.pyi` & `reflex-0.5.0a3/reflex/components/lucide/icon.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/markdown/markdown.py` & `reflex-0.5.0a3/reflex/components/markdown/markdown.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/markdown/markdown.pyi` & `reflex-0.5.0a3/reflex/components/markdown/markdown.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/moment/moment.py` & `reflex-0.5.0a3/reflex/components/moment/moment.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/moment/moment.pyi` & `reflex-0.5.0a3/reflex/components/moment/moment.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/next/base.pyi` & `reflex-0.5.0a3/reflex/components/next/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/next/image.py` & `reflex-0.5.0a3/reflex/components/next/image.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/next/image.pyi` & `reflex-0.5.0a3/reflex/components/next/image.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/next/link.pyi` & `reflex-0.5.0a3/reflex/components/next/link.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/next/video.py` & `reflex-0.5.0a3/reflex/components/next/video.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/next/video.pyi` & `reflex-0.5.0a3/reflex/components/next/video.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/plotly/plotly.py` & `reflex-0.5.0a3/reflex/components/plotly/plotly.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/plotly/plotly.pyi` & `reflex-0.5.0a3/reflex/components/plotly/plotly.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/primitives/accordion.py` & `reflex-0.5.0a3/reflex/components/radix/primitives/accordion.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,20 +262,20 @@
                 "overflow": "hidden",
                 "width": "100%",
                 "margin_top": "1px",
                 "border_top": divider_style,
                 "&:first-child": {
                     "margin_top": 0,
                     "border_top": 0,
-                    "border_top_left_radius": "max(var(--radius-2), var(--radius-6))",
-                    "border_top_right_radius": "max(var(--radius-2), var(--radius-6))",
+                    "border_top_left_radius": "var(--radius-4)",
+                    "border_top_right_radius": "var(--radius-4)",
                 },
                 "&:last-child": {
-                    "border_bottom_left_radius": "max(var(--radius-2), var(--radius-6))",
-                    "border_bottom_right_radius": "max(var(--radius-2), var(--radius-6))",
+                    "border_bottom_left_radius": "var(--radius-4)",
+                    "border_bottom_right_radius": "var(--radius-4)",
                 },
                 "&:focus-within": {
                     "position": "relative",
                     "z_index": 1,
                 },
                 _inherited_variant_selector("ghost", "&:first-child"): {
                     "border_radius": 0,
```

### Comparing `reflex-0.5.0a2/reflex/components/radix/primitives/accordion.pyi` & `reflex-0.5.0a3/reflex/components/radix/primitives/accordion.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/primitives/base.py` & `reflex-0.5.0a3/reflex/components/radix/primitives/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/primitives/base.pyi` & `reflex-0.5.0a3/reflex/components/radix/primitives/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/primitives/drawer.py` & `reflex-0.5.0a3/reflex/components/radix/primitives/drawer.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/primitives/drawer.pyi` & `reflex-0.5.0a3/reflex/components/radix/primitives/drawer.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/primitives/form.py` & `reflex-0.5.0a3/reflex/components/radix/primitives/form.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/primitives/form.pyi` & `reflex-0.5.0a3/reflex/components/radix/primitives/form.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/primitives/progress.py` & `reflex-0.5.0a3/reflex/components/radix/primitives/progress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/primitives/progress.pyi` & `reflex-0.5.0a3/reflex/components/radix/primitives/progress.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/primitives/slider.py` & `reflex-0.5.0a3/reflex/components/radix/primitives/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/primitives/slider.pyi` & `reflex-0.5.0a3/reflex/components/radix/primitives/slider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/base.py` & `reflex-0.5.0a3/reflex/components/radix/themes/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/base.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/color_mode.py` & `reflex-0.5.0a3/reflex/components/radix/themes/color_mode.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 import dataclasses
 from typing import Literal, get_args
 
 from reflex.components.component import BaseComponent
 from reflex.components.core.cond import Cond, color_mode_cond, cond
 from reflex.components.lucide.icon import Icon
-from reflex.style import color_mode, toggle_color_mode
+from reflex.components.radix.themes.components.switch import Switch
+from reflex.style import LIGHT_COLOR_MODE, color_mode, toggle_color_mode
 from reflex.utils import console
 from reflex.vars import BaseVar, Var
 
 from .components.icon_button import IconButton
 
 DEFAULT_LIGHT_ICON: Icon = Icon.create(tag="sun")
 DEFAULT_DARK_ICON: Icon = Icon.create(tag="moon")
@@ -139,15 +140,38 @@
         return super().create(
             ColorModeIcon.create(),
             on_click=toggle_color_mode,
             **props,
         )
 
 
+class ColorModeSwitch(Switch):
+    """Switch for toggling light / dark mode via toggle_color_mode."""
+
+    @classmethod
+    def create(cls, *children, **props):
+        """Create a switch component bound to color_mode.
+
+        Args:
+            *children: The children of the component.
+            **props: The props to pass to the component.
+
+        Returns:
+            The switch component.
+        """
+        return Switch.create(
+            *children,
+            checked=color_mode != LIGHT_COLOR_MODE,
+            on_change=toggle_color_mode,
+            **props,
+        )
+
+
 class ColorModeNamespace(BaseVar):
     """Namespace for color mode components."""
 
     icon = staticmethod(ColorModeIcon.create)
     button = staticmethod(ColorModeIconButton.create)
+    switch = staticmethod(ColorModeSwitch.create)
 
 
 color_mode_var_and_namespace = ColorModeNamespace(**dataclasses.asdict(color_mode))
```

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/color_mode.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/components/hover_card.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,34 @@
-"""Stub file for reflex/components/radix/themes/color_mode.py"""
+"""Stub file for reflex/components/radix/themes/components/hover_card.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-import dataclasses
-from typing import Literal, get_args
-from reflex.components.component import BaseComponent
-from reflex.components.core.cond import Cond, color_mode_cond, cond
-from reflex.components.lucide.icon import Icon
-from reflex.style import color_mode, toggle_color_mode
-from reflex.utils import console
-from reflex.vars import BaseVar, Var
-from .components.icon_button import IconButton
+from typing import Any, Dict, Literal
+from reflex import el
+from reflex.components.component import ComponentNamespace
+from reflex.constants import EventTriggers
+from reflex.vars import Var
+from ..base import RadixThemesComponent, RadixThemesTriggerComponent
 
-DEFAULT_LIGHT_ICON: Icon
-DEFAULT_DARK_ICON: Icon
-
-class ColorModeIcon(Cond):
+class HoverCardRoot(RadixThemesComponent):
+    def get_event_triggers(self) -> Dict[str, Any]: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        cond: Optional[Union[Var[Any], Any]] = None,
-        comp1: Optional[BaseComponent] = None,
-        comp2: Optional[BaseComponent] = None,
+        default_open: Optional[Union[Var[bool], bool]] = None,
+        open: Optional[Union[Var[bool], bool]] = None,
+        open_delay: Optional[Union[Var[int], int]] = None,
+        close_delay: Optional[Union[Var[int], int]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -70,156 +66,139 @@
         ] = None,
         on_mouse_over: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_up: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_open_change: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "ColorModeIcon":
-        """Create an icon component based on color_mode.
+    ) -> "HoverCardRoot":
+        """Create a new component instance.
+
+        Will prepend "RadixThemes" to the component tag to avoid conflicts with
+        other UI libraries for common names, like Text and Button.
 
         Args:
-            light_component: the component to display when color mode is default
-            dark_component: the component to display when color mode is dark (non-default)
+            *children: Child components.
+            default_open: The open state of the hover card when it is initially rendered. Use when you do not need to control its open state.
+            open: The controlled open state of the hover card. Must be used in conjunction with onOpenChange.
+            open_delay: The duration from when the mouse enters the trigger until the hover card opens.
+            close_delay: The duration from when the mouse leaves the trigger until the hover card closes.
+            style: The style of the component.
+            key: A unique key for the component.
+            id: The id for the component.
+            class_name: The class name for the component.
+            autofocus: Whether the component should take the focus once the page is loaded
+            custom_attrs: custom attribute
+            **props: Component properties.
 
         Returns:
-            The conditionally rendered component
+            A new component instance.
         """
         ...
 
-LiteralPosition = Literal["top-left", "top-right", "bottom-left", "bottom-right"]
-position_values = get_args(LiteralPosition)
-position_map = {
-    "position": position_values,
-    "left": ["top-left", "bottom-left"],
-    "right": ["top-right", "bottom-right"],
-    "top": ["top-left", "top-right"],
-    "bottom": ["bottom-left", "bottom-right"],
-}
-
-class ColorModeIconButton(IconButton):
+class HoverCardTrigger(RadixThemesTriggerComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        position: Optional[
-            Literal["top-left", "top-right", "bottom-left", "bottom-right"]
+        style: Optional[Style] = None,
+        key: Optional[Any] = None,
+        id: Optional[Any] = None,
+        class_name: Optional[Any] = None,
+        autofocus: Optional[bool] = None,
+        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
+        on_blur: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        as_child: Optional[Union[Var[bool], bool]] = None,
-        size: Optional[
-            Union[Var[Literal["1", "2", "3", "4"]], Literal["1", "2", "3", "4"]]
+        on_click: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        variant: Optional[
-            Union[
-                Var[Literal["classic", "solid", "soft", "surface", "outline", "ghost"]],
-                Literal["classic", "solid", "soft", "surface", "outline", "ghost"],
-            ]
+        on_context_menu: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        color_scheme: Optional[
-            Union[
-                Var[
-                    Literal[
-                        "tomato",
-                        "red",
-                        "ruby",
-                        "crimson",
-                        "pink",
-                        "plum",
-                        "purple",
-                        "violet",
-                        "iris",
-                        "indigo",
-                        "blue",
-                        "cyan",
-                        "teal",
-                        "jade",
-                        "green",
-                        "grass",
-                        "brown",
-                        "orange",
-                        "sky",
-                        "mint",
-                        "lime",
-                        "yellow",
-                        "amber",
-                        "gold",
-                        "bronze",
-                        "gray",
-                    ]
-                ],
-                Literal[
-                    "tomato",
-                    "red",
-                    "ruby",
-                    "crimson",
-                    "pink",
-                    "plum",
-                    "purple",
-                    "violet",
-                    "iris",
-                    "indigo",
-                    "blue",
-                    "cyan",
-                    "teal",
-                    "jade",
-                    "green",
-                    "grass",
-                    "brown",
-                    "orange",
-                    "sky",
-                    "mint",
-                    "lime",
-                    "yellow",
-                    "amber",
-                    "gold",
-                    "bronze",
-                    "gray",
-                ],
-            ]
+        on_double_click: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        high_contrast: Optional[Union[Var[bool], bool]] = None,
-        radius: Optional[
-            Union[
-                Var[Literal["none", "small", "medium", "large", "full"]],
-                Literal["none", "small", "medium", "large", "full"],
-            ]
+        on_focus: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        auto_focus: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mount: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        disabled: Optional[Union[Var[bool], bool]] = None,
-        form: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        form_action: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_down: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        form_enc_type: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_enter: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        form_method: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_leave: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        form_no_validate: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_move: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        form_target: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_out: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        name: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        type: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        value: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_over: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_up: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_scroll: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_unmount: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        **props
+    ) -> "HoverCardTrigger":
+        """Create a new RadixThemesTriggerComponent instance.
+
+        Args:
+            children: The children of the component.
+            props: The properties of the component.
+
+        Returns:
+            The new RadixThemesTriggerComponent instance.
+        """
+        ...
+
+class HoverCardContent(el.Div, RadixThemesComponent):
+    @overload
+    @classmethod
+    def create(  # type: ignore
+        cls,
+        *children,
+        side: Optional[
+            Union[
+                Var[Literal["top", "right", "bottom", "left"]],
+                Literal["top", "right", "bottom", "left"],
+            ]
+        ] = None,
+        side_offset: Optional[Union[Var[int], int]] = None,
+        align: Optional[
+            Union[
+                Var[Literal["start", "center", "end"]],
+                Literal["start", "center", "end"],
+            ]
         ] = None,
+        avoid_collisions: Optional[Union[Var[bool], bool]] = None,
         access_key: Optional[
             Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
         auto_capitalize: Optional[
             Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
         content_editable: Optional[
@@ -252,15 +231,14 @@
         ] = None,
         tab_index: Optional[
             Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
         title: Optional[
             Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        loading: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -305,37 +283,26 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "ColorModeIconButton":
-        """Create a icon button component that calls toggle_color_mode on click.
+    ) -> "HoverCardContent":
+        """Create a new component instance.
+
+        Will prepend "RadixThemes" to the component tag to avoid conflicts with
+        other UI libraries for common names, like Text and Button.
 
         Args:
-            *children: The children of the component.
-            position: The position of the icon button. Follow document flow if None.
-            as_child: Change the default rendered element for the one passed as a child, merging their props and behavior.
-            size: Button size "1" - "4"
-            variant: Variant of button: "classic" | "solid" | "soft" | "surface" | "outline" | "ghost"
-            color_scheme: Override theme color for button
-            high_contrast: Whether to render the button with higher contrast color against background
-            radius: Override theme radius for button: "none" | "small" | "medium" | "large" | "full"
-            auto_focus: Automatically focuses the button when the page loads
-            disabled: Disables the button
-            form: Associates the button with a form (by id)
-            form_action: URL to send the form data to (for type="submit" buttons)
-            form_enc_type: How the form data should be encoded when submitting to the server (for type="submit" buttons)
-            form_method: HTTP method to use for sending form data (for type="submit" buttons)
-            form_no_validate: Bypasses form validation when submitting (for type="submit" buttons)
-            form_target: Specifies where to display the response after submitting the form (for type="submit" buttons)
-            name: Name of the button, used when sending form data
-            type: Type of the button (submit, reset, or button)
-            value: Value of the button, used when sending form data
+            *children: Child components.
+            side: The preferred side of the trigger to render against when open. Will be reversed when collisions occur and avoidCollisions is enabled.
+            side_offset: The distance in pixels from the trigger.
+            align: The preferred alignment against the trigger. May change when collisions occur.
+            avoid_collisions: Whether or not the hover card should avoid collisions with its trigger.
             access_key:  Provides a hint for generating a keyboard shortcut for the current element.
             auto_capitalize: Controls whether and how text input is automatically capitalized as it is entered/edited by the user.
             content_editable: Indicates whether the element's content is editable.
             context_menu: Defines the ID of a <menu> element which will serve as the element's context menu.
             dir: Defines the text direction. Allowed values are ltr (Left-To-Right) or rtl (Right-To-Left)
             draggable: Defines whether the element can be dragged.
             enter_key_hint: Hints what media types the media element is able to play.
@@ -344,26 +311,113 @@
             item_prop: Defines the name of the element for metadata purposes.
             lang: Defines the language used in the element.
             role: Defines the role of the element.
             slot: Assigns a slot in a shadow DOM shadow tree to an element.
             spell_check: Defines whether the element may be checked for spelling errors.
             tab_index: Defines the position of the current element in the tabbing order.
             title: Defines a tooltip for the element.
-            loading: If set, show an rx.spinner instead of the component children.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: The props to pass to the component.
+            **props: Component properties.
 
         Returns:
-            The button component.
+            A new component instance.
         """
         ...
 
-class ColorModeNamespace(BaseVar):
-    icon = staticmethod(ColorModeIcon.create)
-    button = staticmethod(ColorModeIconButton.create)
+class HoverCard(ComponentNamespace):
+    root = staticmethod(HoverCardRoot.create)
+    trigger = staticmethod(HoverCardTrigger.create)
+    content = staticmethod(HoverCardContent.create)
+
+    @staticmethod
+    def __call__(
+        *children,
+        default_open: Optional[Union[Var[bool], bool]] = None,
+        open: Optional[Union[Var[bool], bool]] = None,
+        open_delay: Optional[Union[Var[int], int]] = None,
+        close_delay: Optional[Union[Var[int], int]] = None,
+        style: Optional[Style] = None,
+        key: Optional[Any] = None,
+        id: Optional[Any] = None,
+        class_name: Optional[Any] = None,
+        autofocus: Optional[bool] = None,
+        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
+        on_blur: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_click: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_context_menu: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_double_click: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_focus: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mount: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_down: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_enter: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_leave: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_move: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_out: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_over: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_up: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_open_change: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_scroll: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_unmount: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        **props
+    ) -> "HoverCardRoot":
+        """Create a new component instance.
+
+        Will prepend "RadixThemes" to the component tag to avoid conflicts with
+        other UI libraries for common names, like Text and Button.
+
+        Args:
+            *children: Child components.
+            default_open: The open state of the hover card when it is initially rendered. Use when you do not need to control its open state.
+            open: The controlled open state of the hover card. Must be used in conjunction with onOpenChange.
+            open_delay: The duration from when the mouse enters the trigger until the hover card opens.
+            close_delay: The duration from when the mouse leaves the trigger until the hover card closes.
+            style: The style of the component.
+            key: A unique key for the component.
+            id: The id for the component.
+            class_name: The class name for the component.
+            autofocus: Whether the component should take the focus once the page is loaded
+            custom_attrs: custom attribute
+            **props: Component properties.
+
+        Returns:
+            A new component instance.
+        """
+        ...
 
-color_mode_var_and_namespace = ColorModeNamespace(**dataclasses.asdict(color_mode))
+hover_card = HoverCard()
```

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/__init__.py` & `reflex-0.5.0a3/reflex/components/radix/themes/components/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/alert_dialog.py` & `reflex-0.5.0a3/reflex/components/radix/themes/components/alert_dialog.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/alert_dialog.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/components/alert_dialog.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/aspect_ratio.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/components/aspect_ratio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/avatar.py` & `reflex-0.5.0a3/reflex/components/radix/themes/components/avatar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/avatar.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/components/avatar.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/badge.py` & `reflex-0.5.0a3/reflex/components/radix/themes/components/badge.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/badge.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/components/badge.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/button.py` & `reflex-0.5.0a3/reflex/components/radix/themes/components/button.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/button.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/components/button.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/callout.py` & `reflex-0.5.0a3/reflex/components/radix/themes/components/callout.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/callout.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/components/callout.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/card.py` & `reflex-0.5.0a3/reflex/components/radix/themes/components/card.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/card.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/components/card.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/checkbox.py` & `reflex-0.5.0a3/reflex/components/radix/themes/components/checkbox.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/checkbox.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/components/checkbox.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/checkbox_cards.py` & `reflex-0.5.0a3/reflex/components/radix/themes/components/checkbox_cards.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/checkbox_cards.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/components/checkbox_cards.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/checkbox_group.py` & `reflex-0.5.0a3/reflex/components/radix/themes/components/checkbox_group.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/checkbox_group.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/components/checkbox_group.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/context_menu.py` & `reflex-0.5.0a3/reflex/components/radix/themes/components/context_menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/context_menu.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/components/context_menu.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/data_list.py` & `reflex-0.5.0a3/reflex/components/radix/themes/components/data_list.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/data_list.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/components/data_list.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/dialog.py` & `reflex-0.5.0a3/reflex/components/radix/themes/components/dialog.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/dialog.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/components/dialog.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/dropdown_menu.py` & `reflex-0.5.0a3/reflex/components/radix/themes/components/dropdown_menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/dropdown_menu.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/components/dropdown_menu.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/hover_card.py` & `reflex-0.5.0a3/reflex/components/radix/themes/components/hover_card.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/hover_card.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/components/popover.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Stub file for reflex/components/radix/themes/components/hover_card.py"""
+"""Stub file for reflex/components/radix/themes/components/popover.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
@@ -10,25 +10,23 @@
 from typing import Any, Dict, Literal
 from reflex import el
 from reflex.components.component import ComponentNamespace
 from reflex.constants import EventTriggers
 from reflex.vars import Var
 from ..base import RadixThemesComponent, RadixThemesTriggerComponent
 
-class HoverCardRoot(RadixThemesComponent):
+class PopoverRoot(RadixThemesComponent):
     def get_event_triggers(self) -> Dict[str, Any]: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        default_open: Optional[Union[Var[bool], bool]] = None,
         open: Optional[Union[Var[bool], bool]] = None,
-        open_delay: Optional[Union[Var[int], int]] = None,
-        close_delay: Optional[Union[Var[int], int]] = None,
+        modal: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -76,40 +74,38 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "HoverCardRoot":
+    ) -> "PopoverRoot":
         """Create a new component instance.
 
         Will prepend "RadixThemes" to the component tag to avoid conflicts with
         other UI libraries for common names, like Text and Button.
 
         Args:
             *children: Child components.
-            default_open: The open state of the hover card when it is initially rendered. Use when you do not need to control its open state.
-            open: The controlled open state of the hover card. Must be used in conjunction with onOpenChange.
-            open_delay: The duration from when the mouse enters the trigger until the hover card opens.
-            close_delay: The duration from when the mouse leaves the trigger until the hover card closes.
+            open: The controlled open state of the popover.
+            modal: The modality of the popover. When set to true, interaction with outside elements will be disabled and only popover content will be visible to screen readers.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
 
-class HoverCardTrigger(RadixThemesTriggerComponent):
+class PopoverTrigger(RadixThemesTriggerComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
@@ -159,45 +155,50 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "HoverCardTrigger":
+    ) -> "PopoverTrigger":
         """Create a new RadixThemesTriggerComponent instance.
 
         Args:
             children: The children of the component.
             props: The properties of the component.
 
         Returns:
             The new RadixThemesTriggerComponent instance.
         """
         ...
 
-class HoverCardContent(el.Div, RadixThemesComponent):
+class PopoverContent(el.Div, RadixThemesComponent):
+    def get_event_triggers(self) -> Dict[str, Any]: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
+        size: Optional[
+            Union[Var[Literal["1", "2", "3", "4"]], Literal["1", "2", "3", "4"]]
+        ] = None,
         side: Optional[
             Union[
                 Var[Literal["top", "right", "bottom", "left"]],
                 Literal["top", "right", "bottom", "left"],
             ]
         ] = None,
         side_offset: Optional[Union[Var[int], int]] = None,
         align: Optional[
             Union[
                 Var[Literal["start", "center", "end"]],
                 Literal["start", "center", "end"],
             ]
         ] = None,
+        align_offset: Optional[Union[Var[int], int]] = None,
         avoid_collisions: Optional[Union[Var[bool], bool]] = None,
         access_key: Optional[
             Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
         auto_capitalize: Optional[
             Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
@@ -243,23 +244,35 @@
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_close_auto_focus: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_context_menu: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_double_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_escape_key_down: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_focus: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_focus_outside: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_interact_outside: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_mount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_down: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_enter: Optional[
@@ -276,33 +289,41 @@
         ] = None,
         on_mouse_over: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_up: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_open_auto_focus: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_pointer_down_outside: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "HoverCardContent":
+    ) -> "PopoverContent":
         """Create a new component instance.
 
         Will prepend "RadixThemes" to the component tag to avoid conflicts with
         other UI libraries for common names, like Text and Button.
 
         Args:
             *children: Child components.
-            side: The preferred side of the trigger to render against when open. Will be reversed when collisions occur and avoidCollisions is enabled.
-            side_offset: The distance in pixels from the trigger.
-            align: The preferred alignment against the trigger. May change when collisions occur.
-            avoid_collisions: Whether or not the hover card should avoid collisions with its trigger.
+            size: Size of the button: "1" | "2" | "3" | "4"
+            side: The preferred side of the anchor to render against when open. Will be reversed when collisions occur and avoidCollisions is enabled.
+            side_offset: The distance in pixels from the anchor.
+            align: The preferred alignment against the anchor. May change when collisions occur.
+            align_offset: The vertical distance in pixels from the anchor.
+            avoid_collisions: When true, overrides the side andalign preferences to prevent collisions with boundary edges.
             access_key:  Provides a hint for generating a keyboard shortcut for the current element.
             auto_capitalize: Controls whether and how text input is automatically capitalized as it is entered/edited by the user.
             content_editable: Indicates whether the element's content is editable.
             context_menu: Defines the ID of a <menu> element which will serve as the element's context menu.
             dir: Defines the text direction. Allowed values are ltr (Left-To-Right) or rtl (Right-To-Left)
             draggable: Defines whether the element can be dragged.
             enter_key_hint: Hints what media types the media element is able to play.
@@ -324,26 +345,20 @@
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
 
-class HoverCard(ComponentNamespace):
-    root = staticmethod(HoverCardRoot.create)
-    trigger = staticmethod(HoverCardTrigger.create)
-    content = staticmethod(HoverCardContent.create)
-
-    @staticmethod
-    def __call__(
+class PopoverClose(RadixThemesTriggerComponent):
+    @overload
+    @classmethod
+    def create(  # type: ignore
+        cls,
         *children,
-        default_open: Optional[Union[Var[bool], bool]] = None,
-        open: Optional[Union[Var[bool], bool]] = None,
-        open_delay: Optional[Union[Var[int], int]] = None,
-        close_delay: Optional[Union[Var[int], int]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -381,43 +396,33 @@
         ] = None,
         on_mouse_over: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_up: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_open_change: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "HoverCardRoot":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
+    ) -> "PopoverClose":
+        """Create a new RadixThemesTriggerComponent instance.
 
         Args:
-            *children: Child components.
-            default_open: The open state of the hover card when it is initially rendered. Use when you do not need to control its open state.
-            open: The controlled open state of the hover card. Must be used in conjunction with onOpenChange.
-            open_delay: The duration from when the mouse enters the trigger until the hover card opens.
-            close_delay: The duration from when the mouse leaves the trigger until the hover card closes.
-            style: The style of the component.
-            key: A unique key for the component.
-            id: The id for the component.
-            class_name: The class name for the component.
-            autofocus: Whether the component should take the focus once the page is loaded
-            custom_attrs: custom attribute
-            **props: Component properties.
+            children: The children of the component.
+            props: The properties of the component.
 
         Returns:
-            A new component instance.
+            The new RadixThemesTriggerComponent instance.
         """
         ...
 
-hover_card = HoverCard()
+class Popover(ComponentNamespace):
+    root = staticmethod(PopoverRoot.create)
+    trigger = staticmethod(PopoverTrigger.create)
+    content = staticmethod(PopoverContent.create)
+    close = staticmethod(PopoverClose.create)
+
+popover = Popover()
```

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/icon_button.py` & `reflex-0.5.0a3/reflex/components/radix/themes/components/icon_button.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/icon_button.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/components/icon_button.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/inset.py` & `reflex-0.5.0a3/reflex/components/radix/themes/components/inset.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/inset.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/components/inset.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/popover.py` & `reflex-0.5.0a3/reflex/components/radix/themes/components/popover.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/popover.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/layout/stack.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,116 +1,88 @@
-"""Stub file for reflex/components/radix/themes/components/popover.py"""
+"""Stub file for reflex/components/radix/themes/layout/stack.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Any, Dict, Literal
-from reflex import el
-from reflex.components.component import ComponentNamespace
-from reflex.constants import EventTriggers
+from reflex.components.component import Component
 from reflex.vars import Var
-from ..base import RadixThemesComponent, RadixThemesTriggerComponent
+from ..base import LiteralAlign, LiteralSpacing
+from .flex import Flex, LiteralFlexDirection
 
-class PopoverRoot(RadixThemesComponent):
-    def get_event_triggers(self) -> Dict[str, Any]: ...
+class Stack(Flex):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        open: Optional[Union[Var[bool], bool]] = None,
-        modal: Optional[Union[Var[bool], bool]] = None,
-        style: Optional[Style] = None,
-        key: Optional[Any] = None,
-        id: Optional[Any] = None,
-        class_name: Optional[Any] = None,
-        autofocus: Optional[bool] = None,
-        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
-        on_blur: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_click: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        spacing: Optional[LiteralSpacing] = "3",
+        align: Optional[LiteralAlign] = "start",
+        as_child: Optional[Union[Var[bool], bool]] = None,
+        direction: Optional[
+            Union[
+                Var[Literal["row", "column", "row-reverse", "column-reverse"]],
+                Literal["row", "column", "row-reverse", "column-reverse"],
+            ]
         ] = None,
-        on_context_menu: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        justify: Optional[
+            Union[
+                Var[Literal["start", "center", "end", "between"]],
+                Literal["start", "center", "end", "between"],
+            ]
         ] = None,
-        on_double_click: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        wrap: Optional[
+            Union[
+                Var[Literal["nowrap", "wrap", "wrap-reverse"]],
+                Literal["nowrap", "wrap", "wrap-reverse"],
+            ]
         ] = None,
-        on_focus: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        access_key: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_mount: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        auto_capitalize: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_mouse_down: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        content_editable: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_mouse_enter: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        context_menu: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_mouse_leave: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        dir: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        draggable: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_mouse_move: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        enter_key_hint: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_mouse_out: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        hidden: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_mouse_over: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        input_mode: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_mouse_up: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        item_prop: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_open_change: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        lang: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        role: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        slot: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        spell_check: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_scroll: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        tab_index: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_unmount: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        title: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        **props
-    ) -> "PopoverRoot":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
-
-        Args:
-            *children: Child components.
-            open: The controlled open state of the popover.
-            modal: The modality of the popover. When set to true, interaction with outside elements will be disabled and only popover content will be visible to screen readers.
-            style: The style of the component.
-            key: A unique key for the component.
-            id: The id for the component.
-            class_name: The class name for the component.
-            autofocus: Whether the component should take the focus once the page is loaded
-            custom_attrs: custom attribute
-            **props: Component properties.
-
-        Returns:
-            A new component instance.
-        """
-        ...
-
-class PopoverTrigger(RadixThemesTriggerComponent):
-    @overload
-    @classmethod
-    def create(  # type: ignore
-        cls,
-        *children,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -155,51 +127,81 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "PopoverTrigger":
-        """Create a new RadixThemesTriggerComponent instance.
+    ) -> "Stack":
+        """Create a new instance of the component.
 
         Args:
-            children: The children of the component.
-            props: The properties of the component.
+            *children: The children of the stack.
+            spacing: The spacing between each stack item.
+            align: The alignment of the stack items.
+            as_child: Change the default rendered element for the one passed as a child, merging their props and behavior.
+            direction: How child items are layed out: "row" | "column" | "row-reverse" | "column-reverse"
+            justify: Alignment of children along the cross axis: "start" | "center" | "end" | "between"
+            wrap: Whether children should wrap when they reach the end of their container: "nowrap" | "wrap" | "wrap-reverse"
+            access_key:  Provides a hint for generating a keyboard shortcut for the current element.
+            auto_capitalize: Controls whether and how text input is automatically capitalized as it is entered/edited by the user.
+            content_editable: Indicates whether the element's content is editable.
+            context_menu: Defines the ID of a <menu> element which will serve as the element's context menu.
+            dir: Defines the text direction. Allowed values are ltr (Left-To-Right) or rtl (Right-To-Left)
+            draggable: Defines whether the element can be dragged.
+            enter_key_hint: Hints what media types the media element is able to play.
+            hidden: Defines whether the element is hidden.
+            input_mode: Defines the type of the element.
+            item_prop: Defines the name of the element for metadata purposes.
+            lang: Defines the language used in the element.
+            role: Defines the role of the element.
+            slot: Assigns a slot in a shadow DOM shadow tree to an element.
+            spell_check: Defines whether the element may be checked for spelling errors.
+            tab_index: Defines the position of the current element in the tabbing order.
+            title: Defines a tooltip for the element.
+            style: The style of the component.
+            key: A unique key for the component.
+            id: The id for the component.
+            class_name: The class name for the component.
+            autofocus: Whether the component should take the focus once the page is loaded
+            custom_attrs: custom attribute
+            **props: The properties of the stack.
 
         Returns:
-            The new RadixThemesTriggerComponent instance.
+            The stack component.
         """
         ...
 
-class PopoverContent(el.Div, RadixThemesComponent):
-    def get_event_triggers(self) -> Dict[str, Any]: ...
+class VStack(Stack):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        size: Optional[
-            Union[Var[Literal["1", "2", "3", "4"]], Literal["1", "2", "3", "4"]]
+        spacing: Optional[LiteralSpacing] = "3",
+        align: Optional[LiteralAlign] = "start",
+        direction: Optional[
+            Union[
+                Var[Literal["row", "column", "row-reverse", "column-reverse"]],
+                Literal["row", "column", "row-reverse", "column-reverse"],
+            ]
         ] = None,
-        side: Optional[
+        as_child: Optional[Union[Var[bool], bool]] = None,
+        justify: Optional[
             Union[
-                Var[Literal["top", "right", "bottom", "left"]],
-                Literal["top", "right", "bottom", "left"],
+                Var[Literal["start", "center", "end", "between"]],
+                Literal["start", "center", "end", "between"],
             ]
         ] = None,
-        side_offset: Optional[Union[Var[int], int]] = None,
-        align: Optional[
+        wrap: Optional[
             Union[
-                Var[Literal["start", "center", "end"]],
-                Literal["start", "center", "end"],
+                Var[Literal["nowrap", "wrap", "wrap-reverse"]],
+                Literal["nowrap", "wrap", "wrap-reverse"],
             ]
         ] = None,
-        align_offset: Optional[Union[Var[int], int]] = None,
-        avoid_collisions: Optional[Union[Var[bool], bool]] = None,
         access_key: Optional[
             Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
         auto_capitalize: Optional[
             Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
         content_editable: Optional[
@@ -244,35 +246,23 @@
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_close_auto_focus: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_context_menu: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_double_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_escape_key_down: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_focus: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_focus_outside: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_interact_outside: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_mount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_down: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_enter: Optional[
@@ -289,41 +279,32 @@
         ] = None,
         on_mouse_over: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_up: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_open_auto_focus: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_pointer_down_outside: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "PopoverContent":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
+    ) -> "VStack":
+        """Create a new instance of the component.
 
         Args:
-            *children: Child components.
-            size: Size of the button: "1" | "2" | "3" | "4"
-            side: The preferred side of the anchor to render against when open. Will be reversed when collisions occur and avoidCollisions is enabled.
-            side_offset: The distance in pixels from the anchor.
-            align: The preferred alignment against the anchor. May change when collisions occur.
-            align_offset: The vertical distance in pixels from the anchor.
-            avoid_collisions: When true, overrides the side andalign preferences to prevent collisions with boundary edges.
+            *children: The children of the stack.
+            spacing: The spacing between each stack item.
+            align: The alignment of the stack items.
+            direction: How child items are layed out: "row" | "column" | "row-reverse" | "column-reverse"
+            as_child: Change the default rendered element for the one passed as a child, merging their props and behavior.
+            justify: Alignment of children along the cross axis: "start" | "center" | "end" | "between"
+            wrap: Whether children should wrap when they reach the end of their container: "nowrap" | "wrap" | "wrap-reverse"
             access_key:  Provides a hint for generating a keyboard shortcut for the current element.
             auto_capitalize: Controls whether and how text input is automatically capitalized as it is entered/edited by the user.
             content_editable: Indicates whether the element's content is editable.
             context_menu: Defines the ID of a <menu> element which will serve as the element's context menu.
             dir: Defines the text direction. Allowed values are ltr (Left-To-Right) or rtl (Right-To-Left)
             draggable: Defines whether the element can be dragged.
             enter_key_hint: Hints what media types the media element is able to play.
@@ -338,27 +319,88 @@
             title: Defines a tooltip for the element.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: Component properties.
+            **props: The properties of the stack.
 
         Returns:
-            A new component instance.
+            The stack component.
         """
         ...
 
-class PopoverClose(RadixThemesTriggerComponent):
+class HStack(Stack):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
+        spacing: Optional[LiteralSpacing] = "3",
+        align: Optional[LiteralAlign] = "start",
+        direction: Optional[
+            Union[
+                Var[Literal["row", "column", "row-reverse", "column-reverse"]],
+                Literal["row", "column", "row-reverse", "column-reverse"],
+            ]
+        ] = None,
+        as_child: Optional[Union[Var[bool], bool]] = None,
+        justify: Optional[
+            Union[
+                Var[Literal["start", "center", "end", "between"]],
+                Literal["start", "center", "end", "between"],
+            ]
+        ] = None,
+        wrap: Optional[
+            Union[
+                Var[Literal["nowrap", "wrap", "wrap-reverse"]],
+                Literal["nowrap", "wrap", "wrap-reverse"],
+            ]
+        ] = None,
+        access_key: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        auto_capitalize: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        content_editable: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        context_menu: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        dir: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        draggable: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        enter_key_hint: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        hidden: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        input_mode: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        item_prop: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        lang: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        role: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        slot: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        spell_check: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        tab_index: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        title: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -403,26 +445,46 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "PopoverClose":
-        """Create a new RadixThemesTriggerComponent instance.
+    ) -> "HStack":
+        """Create a new instance of the component.
 
         Args:
-            children: The children of the component.
-            props: The properties of the component.
+            *children: The children of the stack.
+            spacing: The spacing between each stack item.
+            align: The alignment of the stack items.
+            direction: How child items are layed out: "row" | "column" | "row-reverse" | "column-reverse"
+            as_child: Change the default rendered element for the one passed as a child, merging their props and behavior.
+            justify: Alignment of children along the cross axis: "start" | "center" | "end" | "between"
+            wrap: Whether children should wrap when they reach the end of their container: "nowrap" | "wrap" | "wrap-reverse"
+            access_key:  Provides a hint for generating a keyboard shortcut for the current element.
+            auto_capitalize: Controls whether and how text input is automatically capitalized as it is entered/edited by the user.
+            content_editable: Indicates whether the element's content is editable.
+            context_menu: Defines the ID of a <menu> element which will serve as the element's context menu.
+            dir: Defines the text direction. Allowed values are ltr (Left-To-Right) or rtl (Right-To-Left)
+            draggable: Defines whether the element can be dragged.
+            enter_key_hint: Hints what media types the media element is able to play.
+            hidden: Defines whether the element is hidden.
+            input_mode: Defines the type of the element.
+            item_prop: Defines the name of the element for metadata purposes.
+            lang: Defines the language used in the element.
+            role: Defines the role of the element.
+            slot: Assigns a slot in a shadow DOM shadow tree to an element.
+            spell_check: Defines whether the element may be checked for spelling errors.
+            tab_index: Defines the position of the current element in the tabbing order.
+            title: Defines a tooltip for the element.
+            style: The style of the component.
+            key: A unique key for the component.
+            id: The id for the component.
+            class_name: The class name for the component.
+            autofocus: Whether the component should take the focus once the page is loaded
+            custom_attrs: custom attribute
+            **props: The properties of the stack.
 
         Returns:
-            The new RadixThemesTriggerComponent instance.
+            The stack component.
         """
         ...
-
-class Popover(ComponentNamespace):
-    root = staticmethod(PopoverRoot.create)
-    trigger = staticmethod(PopoverTrigger.create)
-    content = staticmethod(PopoverContent.create)
-    close = staticmethod(PopoverClose.create)
-
-popover = Popover()
```

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/progress.py` & `reflex-0.5.0a3/reflex/components/radix/themes/components/progress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/progress.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/components/progress.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/radio.py` & `reflex-0.5.0a3/reflex/components/radix/themes/components/radio.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/radio.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/components/radio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/radio_cards.py` & `reflex-0.5.0a3/reflex/components/radix/themes/components/radio_cards.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/radio_cards.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/components/radio_cards.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/radio_group.py` & `reflex-0.5.0a3/reflex/components/radix/themes/components/radio_group.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/radio_group.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/components/radio_group.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/scroll_area.py` & `reflex-0.5.0a3/reflex/components/radix/themes/components/scroll_area.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/scroll_area.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/components/scroll_area.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/segmented_control.py` & `reflex-0.5.0a3/reflex/components/radix/themes/components/segmented_control.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/segmented_control.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/components/segmented_control.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/select.py` & `reflex-0.5.0a3/reflex/components/radix/themes/components/select.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/select.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/components/select.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/separator.py` & `reflex-0.5.0a3/reflex/components/radix/themes/components/separator.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/separator.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/components/separator.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/skeleton.py` & `reflex-0.5.0a3/reflex/components/radix/themes/components/skeleton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/skeleton.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/components/skeleton.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/slider.py` & `reflex-0.5.0a3/reflex/components/radix/themes/components/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/slider.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/components/slider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/spinner.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/components/spinner.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/switch.py` & `reflex-0.5.0a3/reflex/components/radix/themes/components/switch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/switch.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/components/switch.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/table.py` & `reflex-0.5.0a3/reflex/components/radix/themes/components/table.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/table.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/components/table.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/tabs.py` & `reflex-0.5.0a3/reflex/components/radix/themes/components/tabs.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/tabs.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/components/tabs.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/text_area.py` & `reflex-0.5.0a3/reflex/components/radix/themes/components/text_area.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/text_area.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/components/text_area.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/text_field.py` & `reflex-0.5.0a3/reflex/components/radix/themes/components/text_field.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/text_field.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/components/text_field.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/tooltip.py` & `reflex-0.5.0a3/reflex/components/radix/themes/components/tooltip.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/components/tooltip.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/components/tooltip.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/layout/__init__.py` & `reflex-0.5.0a3/reflex/components/radix/themes/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/layout/base.py` & `reflex-0.5.0a3/reflex/components/radix/themes/layout/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/layout/base.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/layout/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/layout/box.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/layout/box.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/layout/center.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/layout/center.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/layout/container.py` & `reflex-0.5.0a3/reflex/components/radix/themes/layout/container.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/layout/container.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/layout/container.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/layout/flex.py` & `reflex-0.5.0a3/reflex/components/radix/themes/layout/flex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/layout/flex.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/layout/flex.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/layout/grid.py` & `reflex-0.5.0a3/reflex/components/radix/themes/layout/grid.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/layout/grid.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/layout/grid.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/layout/list.py` & `reflex-0.5.0a3/reflex/components/radix/themes/layout/list.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/layout/list.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/layout/list.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/layout/section.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/layout/section.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/layout/spacer.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/layout/spacer.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/layout/stack.py` & `reflex-0.5.0a3/reflex/components/radix/themes/layout/stack.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/layout/stack.pyi` & `reflex-0.5.0a3/reflex/components/recharts/polar.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,87 +1,130 @@
-"""Stub file for reflex/components/radix/themes/layout/stack.py"""
+"""Stub file for reflex/components/recharts/polar.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from reflex.components.component import Component
+from typing import Any, Dict, List, Union
+from reflex.constants import EventTriggers
 from reflex.vars import Var
-from ..base import LiteralAlign, LiteralSpacing
-from .flex import Flex, LiteralFlexDirection
+from .recharts import (
+    LiteralAnimationEasing,
+    LiteralGridType,
+    LiteralPolarRadiusType,
+    LiteralScale,
+    Recharts,
+)
 
-class Stack(Flex):
+class Pie(Recharts):
+    def get_event_triggers(self) -> dict[str, Union[Var, Any]]: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        spacing: Optional[LiteralSpacing] = "3",
-        align: Optional[LiteralAlign] = "start",
-        as_child: Optional[Union[Var[bool], bool]] = None,
-        direction: Optional[
-            Union[
-                Var[Literal["row", "column", "row-reverse", "column-reverse"]],
-                Literal["row", "column", "row-reverse", "column-reverse"],
-            ]
-        ] = None,
-        justify: Optional[
-            Union[
-                Var[Literal["start", "center", "end", "between"]],
-                Literal["start", "center", "end", "between"],
-            ]
-        ] = None,
-        wrap: Optional[
-            Union[
-                Var[Literal["nowrap", "wrap", "wrap-reverse"]],
-                Literal["nowrap", "wrap", "wrap-reverse"],
-            ]
-        ] = None,
-        access_key: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        auto_capitalize: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        content_editable: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        context_menu: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        dir: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        draggable: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        enter_key_hint: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        data: Optional[Union[Var[List[Dict[str, Any]]], List[Dict[str, Any]]]] = None,
+        data_key: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        cx: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        cy: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        inner_radius: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        outer_radius: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        start_angle: Optional[Union[Var[int], int]] = None,
+        end_angle: Optional[Union[Var[int], int]] = None,
+        min_angle: Optional[Union[Var[int], int]] = None,
+        padding_angle: Optional[Union[Var[int], int]] = None,
+        name_key: Optional[Union[Var[str], str]] = None,
+        legend_type: Optional[Union[Var[str], str]] = None,
+        label: Optional[Union[Var[bool], bool]] = None,
+        label_line: Optional[Union[Var[bool], bool]] = None,
+        fill: Optional[Union[Var[str], str]] = None,
+        stroke: Optional[Union[Var[str], str]] = None,
+        style: Optional[Style] = None,
+        key: Optional[Any] = None,
+        id: Optional[Any] = None,
+        class_name: Optional[Any] = None,
+        autofocus: Optional[bool] = None,
+        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
+        on_click: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        hidden: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_enter: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        input_mode: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_leave: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        item_prop: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_move: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        lang: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        role: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        slot: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        spell_check: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_out: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        tab_index: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_over: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        title: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        **props
+    ) -> "Pie":
+        """Create the component.
+
+        Args:
+            *children: The children of the component.
+            data: data
+            data_key: The key of each sector's value.
+            cx: The x-coordinate of center. If set a percentage, the final value is obtained by multiplying the percentage of container width.
+            cy: The y-coordinate of center. If set a percentage, the final value is obtained by multiplying the percentage of container height.
+            inner_radius: The inner radius of pie, which can be set to a percent value.
+            outer_radius: The outer radius of pie, which can be set to a percent value.
+            start_angle: The angle of first sector.
+            end_angle: The direction of sectors. 1 means clockwise and -1 means anticlockwise.
+            min_angle: The minimum angle of each unzero data.
+            padding_angle: The angle between two sectors.
+            name_key: The key of each sector's name.
+            legend_type: The type of icon in legend. If set to 'none', no legend item will be rendered.
+            label: If false set, labels will not be drawn.
+            label_line: If false set, label lines will not be drawn.
+            fill: fill color
+            stroke: stroke color
+            style: The style of the component.
+            key: A unique key for the component.
+            id: The id for the component.
+            class_name: The class name for the component.
+            autofocus: Whether the component should take the focus once the page is loaded
+            custom_attrs: custom attribute
+            **props: The props of the component.
+
+        Returns:
+            The component.
+        """
+        ...
+
+class Radar(Recharts):
+    @overload
+    @classmethod
+    def create(  # type: ignore
+        cls,
+        *children,
+        data_key: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        points: Optional[Union[Var[List[Dict[str, Any]]], List[Dict[str, Any]]]] = None,
+        dot: Optional[Union[Var[bool], bool]] = None,
+        stroke: Optional[Union[Var[str], str]] = None,
+        fill: Optional[Union[Var[str], str]] = None,
+        fill_opacity: Optional[Union[Var[float], float]] = None,
+        legend_type: Optional[Union[Var[str], str]] = None,
+        label: Optional[Union[Var[bool], bool]] = None,
+        animation_begin: Optional[Union[Var[int], int]] = None,
+        animation_duration: Optional[Union[Var[int], int]] = None,
+        animation_easing: Optional[
+            Union[
+                Var[Literal["ease", "ease-in", "ease-out", "ease-in-out", "linear"]],
+                Literal["ease", "ease-in", "ease-out", "ease-in-out", "linear"],
+            ]
         ] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
@@ -127,120 +170,193 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "Stack":
-        """Create a new instance of the component.
+    ) -> "Radar":
+        """Create the component.
 
         Args:
-            *children: The children of the stack.
-            spacing: The spacing between each stack item.
-            align: The alignment of the stack items.
-            as_child: Change the default rendered element for the one passed as a child, merging their props and behavior.
-            direction: How child items are layed out: "row" | "column" | "row-reverse" | "column-reverse"
-            justify: Alignment of children along the cross axis: "start" | "center" | "end" | "between"
-            wrap: Whether children should wrap when they reach the end of their container: "nowrap" | "wrap" | "wrap-reverse"
-            access_key:  Provides a hint for generating a keyboard shortcut for the current element.
-            auto_capitalize: Controls whether and how text input is automatically capitalized as it is entered/edited by the user.
-            content_editable: Indicates whether the element's content is editable.
-            context_menu: Defines the ID of a <menu> element which will serve as the element's context menu.
-            dir: Defines the text direction. Allowed values are ltr (Left-To-Right) or rtl (Right-To-Left)
-            draggable: Defines whether the element can be dragged.
-            enter_key_hint: Hints what media types the media element is able to play.
-            hidden: Defines whether the element is hidden.
-            input_mode: Defines the type of the element.
-            item_prop: Defines the name of the element for metadata purposes.
-            lang: Defines the language used in the element.
-            role: Defines the role of the element.
-            slot: Assigns a slot in a shadow DOM shadow tree to an element.
-            spell_check: Defines whether the element may be checked for spelling errors.
-            tab_index: Defines the position of the current element in the tabbing order.
-            title: Defines a tooltip for the element.
+            *children: The children of the component.
+            data_key: The key of a group of data which should be unique in a radar chart.
+            points: The coordinates of all the vertexes of the radar shape, like [{ x, y }].
+            dot: If false set, dots will not be drawn
+            stroke: Stoke color
+            fill: Fill color
+            fill_opacity: opacity
+            legend_type: The type of icon in legend. If set to 'none', no legend item will be rendered.
+            label: If false set, labels will not be drawn
+            animation_begin: Specifies when the animation should begin, the unit of this option is ms.
+            animation_duration: Specifies the duration of animation, the unit of this option is ms.
+            animation_easing: The type of easing function. 'ease' | 'ease-in' | 'ease-out' | 'ease-in-out' | 'linear'
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: The properties of the stack.
+            **props: The props of the component.
 
         Returns:
-            The stack component.
+            The component.
         """
         ...
 
-class VStack(Stack):
+class RadialBar(Recharts):
+    def get_event_triggers(self) -> dict[str, Union[Var, Any]]: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        spacing: Optional[LiteralSpacing] = "3",
-        align: Optional[LiteralAlign] = "start",
-        direction: Optional[
-            Union[
-                Var[Literal["row", "column", "row-reverse", "column-reverse"]],
-                Literal["row", "column", "row-reverse", "column-reverse"],
-            ]
-        ] = None,
-        as_child: Optional[Union[Var[bool], bool]] = None,
-        justify: Optional[
-            Union[
-                Var[Literal["start", "center", "end", "between"]],
-                Literal["start", "center", "end", "between"],
-            ]
-        ] = None,
-        wrap: Optional[
-            Union[
-                Var[Literal["nowrap", "wrap", "wrap-reverse"]],
-                Literal["nowrap", "wrap", "wrap-reverse"],
-            ]
+        data: Optional[Union[Var[List[Dict[str, Any]]], List[Dict[str, Any]]]] = None,
+        min_angle: Optional[Union[Var[int], int]] = None,
+        legend_type: Optional[Union[Var[str], str]] = None,
+        label: Optional[Union[Var[bool], bool]] = None,
+        background: Optional[Union[Var[bool], bool]] = None,
+        style: Optional[Style] = None,
+        key: Optional[Any] = None,
+        id: Optional[Any] = None,
+        class_name: Optional[Any] = None,
+        autofocus: Optional[bool] = None,
+        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
+        on_click: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        access_key: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_enter: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        auto_capitalize: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_leave: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        content_editable: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_move: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        context_menu: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_out: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        dir: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        draggable: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_over: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        enter_key_hint: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        **props
+    ) -> "RadialBar":
+        """Create the component.
+
+        Args:
+            *children: The children of the component.
+            data: The source data which each element is an object.
+            min_angle: Min angle of each bar. A positive value between 0 and 360.
+            legend_type: Type of legend
+            label: If false set, labels will not be drawn.
+            background: If false set, background sector will not be drawn.
+            style: The style of the component.
+            key: A unique key for the component.
+            id: The id for the component.
+            class_name: The class name for the component.
+            autofocus: Whether the component should take the focus once the page is loaded
+            custom_attrs: custom attribute
+            **props: The props of the component.
+
+        Returns:
+            The component.
+        """
+        ...
+
+class PolarAngleAxis(Recharts):
+    def get_event_triggers(self) -> dict[str, Union[Var, Any]]: ...
+    @overload
+    @classmethod
+    def create(  # type: ignore
+        cls,
+        *children,
+        data_key: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        cx: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        cy: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        radius: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        axis_line: Optional[
+            Union[Var[Union[bool, Dict[str, Any]]], Union[bool, Dict[str, Any]]]
+        ] = None,
+        axis_line_type: Optional[Union[Var[str], str]] = None,
+        tick_line: Optional[
+            Union[Var[Union[bool, Dict[str, Any]]], Union[bool, Dict[str, Any]]]
+        ] = None,
+        tick: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        ticks: Optional[Union[Var[List[Dict[str, Any]]], List[Dict[str, Any]]]] = None,
+        orient: Optional[Union[Var[str], str]] = None,
+        allow_duplicated_category: Optional[Union[Var[bool], bool]] = None,
+        style: Optional[Style] = None,
+        key: Optional[Any] = None,
+        id: Optional[Any] = None,
+        class_name: Optional[Any] = None,
+        autofocus: Optional[bool] = None,
+        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
+        on_click: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        hidden: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_enter: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        input_mode: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_leave: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        item_prop: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_move: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        lang: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        role: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        slot: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        spell_check: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_out: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        tab_index: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_over: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        title: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        **props
+    ) -> "PolarAngleAxis":
+        """Create the component.
+
+        Args:
+            *children: The children of the component.
+            data_key: The key of a group of data which should be unique to show the meaning of angle axis.
+            cx: The x-coordinate of center. If set a percentage, the final value is obtained by multiplying the percentage of container width.
+            cy: The y-coordinate of center. If set a percentage, the final value is obtained by multiplying the percentage of container height.
+            radius: The outer radius of circle grid. If set a percentage, the final value is obtained by multiplying the percentage of maxRadius which is calculated by the width, height, cx, cy.
+            axis_line: If false set, axis line will not be drawn. If true set, axis line will be drawn which have the props calculated internally. If object set, axis line will be drawn which have the props mergered by the internal calculated props and the option.
+            axis_line_type: The type of axis line.
+            tick_line: If false set, tick lines will not be drawn. If true set, tick lines will be drawn which have the props calculated internally. If object set, tick lines will be drawn which have the props mergered by the internal calculated props and the option.
+            tick: The width or height of tick.
+            ticks: The array of every tick's value and angle.
+            orient: The orientation of axis text.
+            allow_duplicated_category: Allow the axis has duplicated categorys or not when the type of axis is "category".
+            style: The style of the component.
+            key: A unique key for the component.
+            id: The id for the component.
+            class_name: The class name for the component.
+            autofocus: Whether the component should take the focus once the page is loaded
+            custom_attrs: custom attribute
+            **props: The props of the component.
+
+        Returns:
+            The component.
+        """
+        ...
+
+class PolarGrid(Recharts):
+    @overload
+    @classmethod
+    def create(  # type: ignore
+        cls,
+        *children,
+        cx: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        cy: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        inner_radius: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        outer_radius: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        polar_angles: Optional[Union[Var[List[int]], List[int]]] = None,
+        polar_radius: Optional[Union[Var[List[int]], List[int]]] = None,
+        grid_type: Optional[
+            Union[Var[Literal["polygon", "circle"]], Literal["polygon", "circle"]]
         ] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
@@ -286,148 +402,109 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "VStack":
-        """Create a new instance of the component.
+    ) -> "PolarGrid":
+        """Create the component.
 
         Args:
-            *children: The children of the stack.
-            spacing: The spacing between each stack item.
-            align: The alignment of the stack items.
-            direction: How child items are layed out: "row" | "column" | "row-reverse" | "column-reverse"
-            as_child: Change the default rendered element for the one passed as a child, merging their props and behavior.
-            justify: Alignment of children along the cross axis: "start" | "center" | "end" | "between"
-            wrap: Whether children should wrap when they reach the end of their container: "nowrap" | "wrap" | "wrap-reverse"
-            access_key:  Provides a hint for generating a keyboard shortcut for the current element.
-            auto_capitalize: Controls whether and how text input is automatically capitalized as it is entered/edited by the user.
-            content_editable: Indicates whether the element's content is editable.
-            context_menu: Defines the ID of a <menu> element which will serve as the element's context menu.
-            dir: Defines the text direction. Allowed values are ltr (Left-To-Right) or rtl (Right-To-Left)
-            draggable: Defines whether the element can be dragged.
-            enter_key_hint: Hints what media types the media element is able to play.
-            hidden: Defines whether the element is hidden.
-            input_mode: Defines the type of the element.
-            item_prop: Defines the name of the element for metadata purposes.
-            lang: Defines the language used in the element.
-            role: Defines the role of the element.
-            slot: Assigns a slot in a shadow DOM shadow tree to an element.
-            spell_check: Defines whether the element may be checked for spelling errors.
-            tab_index: Defines the position of the current element in the tabbing order.
-            title: Defines a tooltip for the element.
+            *children: The children of the component.
+            cx: The x-coordinate of center. If set a percentage, the final value is obtained by multiplying the percentage of container width.
+            cy: The y-coordinate of center. If set a percentage, the final value is obtained by multiplying the percentage of container height.
+            inner_radius: The radius of the inner polar grid.
+            outer_radius: The radius of the outer polar grid.
+            polar_angles: The array of every line grid's angle.
+            polar_radius: The array of every line grid's radius.
+            grid_type: The type of polar grids. 'polygon' | 'circle'
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: The properties of the stack.
+            **props: The props of the component.
 
         Returns:
-            The stack component.
+            The component.
         """
         ...
 
-class HStack(Stack):
+class PolarRadiusAxis(Recharts):
+    def get_event_triggers(self) -> dict[str, Union[Var, Any]]: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        spacing: Optional[LiteralSpacing] = "3",
-        align: Optional[LiteralAlign] = "start",
-        direction: Optional[
+        angle: Optional[Union[Var[int], int]] = None,
+        type_: Optional[
+            Union[Var[Literal["number", "category"]], Literal["number", "category"]]
+        ] = None,
+        allow_duplicated_category: Optional[Union[Var[bool], bool]] = None,
+        cx: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        cy: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        reversed: Optional[Union[Var[bool], bool]] = None,
+        orientation: Optional[Union[Var[str], str]] = None,
+        axis_line: Optional[
+            Union[Var[Union[bool, Dict[str, Any]]], Union[bool, Dict[str, Any]]]
+        ] = None,
+        tick: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        tick_count: Optional[Union[Var[int], int]] = None,
+        scale: Optional[
             Union[
-                Var[Literal["row", "column", "row-reverse", "column-reverse"]],
-                Literal["row", "column", "row-reverse", "column-reverse"],
+                Var[
+                    Literal[
+                        "auto",
+                        "linear",
+                        "pow",
+                        "sqrt",
+                        "log",
+                        "identity",
+                        "time",
+                        "band",
+                        "point",
+                        "ordinal",
+                        "quantile",
+                        "quantize",
+                        "utc",
+                        "sequential",
+                        "threshold",
+                    ]
+                ],
+                Literal[
+                    "auto",
+                    "linear",
+                    "pow",
+                    "sqrt",
+                    "log",
+                    "identity",
+                    "time",
+                    "band",
+                    "point",
+                    "ordinal",
+                    "quantile",
+                    "quantize",
+                    "utc",
+                    "sequential",
+                    "threshold",
+                ],
             ]
         ] = None,
-        as_child: Optional[Union[Var[bool], bool]] = None,
-        justify: Optional[
-            Union[
-                Var[Literal["start", "center", "end", "between"]],
-                Literal["start", "center", "end", "between"],
-            ]
-        ] = None,
-        wrap: Optional[
-            Union[
-                Var[Literal["nowrap", "wrap", "wrap-reverse"]],
-                Literal["nowrap", "wrap", "wrap-reverse"],
-            ]
-        ] = None,
-        access_key: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        auto_capitalize: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        content_editable: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        context_menu: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        dir: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        draggable: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        enter_key_hint: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        hidden: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        input_mode: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        item_prop: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        lang: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        role: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        slot: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        spell_check: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        tab_index: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        title: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
-        on_blur: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_context_menu: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_double_click: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_focus: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mount: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_down: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_mouse_enter: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_leave: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_move: Optional[
@@ -435,56 +512,36 @@
         ] = None,
         on_mouse_out: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_over: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_mouse_up: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_scroll: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_unmount: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         **props
-    ) -> "HStack":
-        """Create a new instance of the component.
+    ) -> "PolarRadiusAxis":
+        """Create the component.
 
         Args:
-            *children: The children of the stack.
-            spacing: The spacing between each stack item.
-            align: The alignment of the stack items.
-            direction: How child items are layed out: "row" | "column" | "row-reverse" | "column-reverse"
-            as_child: Change the default rendered element for the one passed as a child, merging their props and behavior.
-            justify: Alignment of children along the cross axis: "start" | "center" | "end" | "between"
-            wrap: Whether children should wrap when they reach the end of their container: "nowrap" | "wrap" | "wrap-reverse"
-            access_key:  Provides a hint for generating a keyboard shortcut for the current element.
-            auto_capitalize: Controls whether and how text input is automatically capitalized as it is entered/edited by the user.
-            content_editable: Indicates whether the element's content is editable.
-            context_menu: Defines the ID of a <menu> element which will serve as the element's context menu.
-            dir: Defines the text direction. Allowed values are ltr (Left-To-Right) or rtl (Right-To-Left)
-            draggable: Defines whether the element can be dragged.
-            enter_key_hint: Hints what media types the media element is able to play.
-            hidden: Defines whether the element is hidden.
-            input_mode: Defines the type of the element.
-            item_prop: Defines the name of the element for metadata purposes.
-            lang: Defines the language used in the element.
-            role: Defines the role of the element.
-            slot: Assigns a slot in a shadow DOM shadow tree to an element.
-            spell_check: Defines whether the element may be checked for spelling errors.
-            tab_index: Defines the position of the current element in the tabbing order.
-            title: Defines a tooltip for the element.
+            *children: The children of the component.
+            angle: The angle of radial direction line to display axis text.
+            type_: The type of axis line. 'number' | 'category'
+            allow_duplicated_category: Allow the axis has duplicated categorys or not when the type of axis is "category".
+            cx: The x-coordinate of center.
+            cy: The y-coordinate of center.
+            reversed: If set to true, the ticks of this axis are reversed.
+            orientation: The orientation of axis text.
+            axis_line: If false set, axis line will not be drawn. If true set, axis line will be drawn which have the props calculated internally. If object set, axis line will be drawn which have the props mergered by the internal calculated props and the option.
+            tick: The width or height of tick.
+            tick_count: The count of ticks.
+            scale: If 'auto' set, the scale funtion is linear scale. 'auto' | 'linear' | 'pow' | 'sqrt' | 'log' | 'identity' | 'time' | 'band' | 'point' | 'ordinal' | 'quantile' | 'quantize' | 'utc' | 'sequential' | 'threshold'
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: The properties of the stack.
+            **props: The props of the component.
 
         Returns:
-            The stack component.
+            The component.
         """
         ...
```

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/typography/blockquote.py` & `reflex-0.5.0a3/reflex/components/radix/themes/typography/blockquote.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/typography/blockquote.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/typography/blockquote.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/typography/code.py` & `reflex-0.5.0a3/reflex/components/radix/themes/typography/code.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/typography/code.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/typography/code.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/typography/heading.py` & `reflex-0.5.0a3/reflex/components/radix/themes/typography/heading.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/typography/heading.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/typography/heading.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/typography/link.py` & `reflex-0.5.0a3/reflex/components/radix/themes/typography/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/typography/link.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/typography/link.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/typography/text.py` & `reflex-0.5.0a3/reflex/components/radix/themes/typography/text.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/radix/themes/typography/text.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/typography/text.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/react_player/audio.pyi` & `reflex-0.5.0a3/reflex/components/react_player/audio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/react_player/react_player.py` & `reflex-0.5.0a3/reflex/components/react_player/react_player.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/react_player/react_player.pyi` & `reflex-0.5.0a3/reflex/components/react_player/react_player.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/react_player/video.pyi` & `reflex-0.5.0a3/reflex/components/react_player/video.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/recharts/__init__.py` & `reflex-0.5.0a3/reflex/components/recharts/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/recharts/cartesian.py` & `reflex-0.5.0a3/reflex/components/recharts/cartesian.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/recharts/cartesian.pyi` & `reflex-0.5.0a3/reflex/components/recharts/cartesian.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/recharts/charts.py` & `reflex-0.5.0a3/reflex/components/recharts/charts.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/recharts/charts.pyi` & `reflex-0.5.0a3/reflex/components/recharts/charts.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/recharts/general.py` & `reflex-0.5.0a3/reflex/components/recharts/general.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/recharts/general.pyi` & `reflex-0.5.0a3/reflex/components/recharts/general.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/recharts/polar.py` & `reflex-0.5.0a3/reflex/components/recharts/polar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/recharts/polar.pyi` & `reflex-0.5.0a3/reflex/components/radix/themes/color_mode.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,131 +1,39 @@
-"""Stub file for reflex/components/recharts/polar.py"""
+"""Stub file for reflex/components/radix/themes/color_mode.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Any, Dict, List, Union
-from reflex.constants import EventTriggers
-from reflex.vars import Var
-from .recharts import (
-    LiteralAnimationEasing,
-    LiteralGridType,
-    LiteralPolarRadiusType,
-    LiteralScale,
-    Recharts,
-)
+import dataclasses
+from typing import Literal, get_args
+from reflex.components.component import BaseComponent
+from reflex.components.core.cond import Cond, color_mode_cond, cond
+from reflex.components.lucide.icon import Icon
+from reflex.components.radix.themes.components.switch import Switch
+from reflex.style import LIGHT_COLOR_MODE, color_mode, toggle_color_mode
+from reflex.utils import console
+from reflex.vars import BaseVar, Var
+from .components.icon_button import IconButton
 
-class Pie(Recharts):
-    def get_event_triggers(self) -> dict[str, Union[Var, Any]]: ...
-    @overload
-    @classmethod
-    def create(  # type: ignore
-        cls,
-        *children,
-        data: Optional[Union[Var[List[Dict[str, Any]]], List[Dict[str, Any]]]] = None,
-        data_key: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
-        cx: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
-        cy: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
-        inner_radius: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
-        outer_radius: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
-        start_angle: Optional[Union[Var[int], int]] = None,
-        end_angle: Optional[Union[Var[int], int]] = None,
-        min_angle: Optional[Union[Var[int], int]] = None,
-        padding_angle: Optional[Union[Var[int], int]] = None,
-        name_key: Optional[Union[Var[str], str]] = None,
-        legend_type: Optional[Union[Var[str], str]] = None,
-        label: Optional[Union[Var[bool], bool]] = None,
-        label_line: Optional[Union[Var[bool], bool]] = None,
-        fill: Optional[Union[Var[str], str]] = None,
-        stroke: Optional[Union[Var[str], str]] = None,
-        style: Optional[Style] = None,
-        key: Optional[Any] = None,
-        id: Optional[Any] = None,
-        class_name: Optional[Any] = None,
-        autofocus: Optional[bool] = None,
-        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
-        on_click: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_enter: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_leave: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_move: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_out: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_over: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        **props
-    ) -> "Pie":
-        """Create the component.
-
-        Args:
-            *children: The children of the component.
-            data: data
-            data_key: The key of each sector's value.
-            cx: The x-coordinate of center. If set a percentage, the final value is obtained by multiplying the percentage of container width.
-            cy: The y-coordinate of center. If set a percentage, the final value is obtained by multiplying the percentage of container height.
-            inner_radius: The inner radius of pie, which can be set to a percent value.
-            outer_radius: The outer radius of pie, which can be set to a percent value.
-            start_angle: The angle of first sector.
-            end_angle: The direction of sectors. 1 means clockwise and -1 means anticlockwise.
-            min_angle: The minimum angle of each unzero data.
-            padding_angle: The angle between two sectors.
-            name_key: The key of each sector's name.
-            legend_type: The type of icon in legend. If set to 'none', no legend item will be rendered.
-            label: If false set, labels will not be drawn.
-            label_line: If false set, label lines will not be drawn.
-            fill: fill color
-            stroke: stroke color
-            style: The style of the component.
-            key: A unique key for the component.
-            id: The id for the component.
-            class_name: The class name for the component.
-            autofocus: Whether the component should take the focus once the page is loaded
-            custom_attrs: custom attribute
-            **props: The props of the component.
-
-        Returns:
-            The component.
-        """
-        ...
+DEFAULT_LIGHT_ICON: Icon
+DEFAULT_DARK_ICON: Icon
 
-class Radar(Recharts):
+class ColorModeIcon(Cond):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        data_key: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
-        points: Optional[Union[Var[List[Dict[str, Any]]], List[Dict[str, Any]]]] = None,
-        dot: Optional[Union[Var[bool], bool]] = None,
-        stroke: Optional[Union[Var[str], str]] = None,
-        fill: Optional[Union[Var[str], str]] = None,
-        fill_opacity: Optional[Union[Var[float], float]] = None,
-        legend_type: Optional[Union[Var[str], str]] = None,
-        label: Optional[Union[Var[bool], bool]] = None,
-        animation_begin: Optional[Union[Var[int], int]] = None,
-        animation_duration: Optional[Union[Var[int], int]] = None,
-        animation_easing: Optional[
-            Union[
-                Var[Literal["ease", "ease-in", "ease-out", "ease-in-out", "linear"]],
-                Literal["ease", "ease-in", "ease-out", "ease-in-out", "linear"],
-            ]
-        ] = None,
+        cond: Optional[Union[Var[Any], Any]] = None,
+        comp1: Optional[BaseComponent] = None,
+        comp2: Optional[BaseComponent] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -170,194 +78,190 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "Radar":
-        """Create the component.
+    ) -> "ColorModeIcon":
+        """Create an icon component based on color_mode.
 
         Args:
-            *children: The children of the component.
-            data_key: The key of a group of data which should be unique in a radar chart.
-            points: The coordinates of all the vertexes of the radar shape, like [{ x, y }].
-            dot: If false set, dots will not be drawn
-            stroke: Stoke color
-            fill: Fill color
-            fill_opacity: opacity
-            legend_type: The type of icon in legend. If set to 'none', no legend item will be rendered.
-            label: If false set, labels will not be drawn
-            animation_begin: Specifies when the animation should begin, the unit of this option is ms.
-            animation_duration: Specifies the duration of animation, the unit of this option is ms.
-            animation_easing: The type of easing function. 'ease' | 'ease-in' | 'ease-out' | 'ease-in-out' | 'linear'
-            style: The style of the component.
-            key: A unique key for the component.
-            id: The id for the component.
-            class_name: The class name for the component.
-            autofocus: Whether the component should take the focus once the page is loaded
-            custom_attrs: custom attribute
-            **props: The props of the component.
+            light_component: the component to display when color mode is default
+            dark_component: the component to display when color mode is dark (non-default)
 
         Returns:
-            The component.
+            The conditionally rendered component
         """
         ...
 
-class RadialBar(Recharts):
-    def get_event_triggers(self) -> dict[str, Union[Var, Any]]: ...
+LiteralPosition = Literal["top-left", "top-right", "bottom-left", "bottom-right"]
+position_values = get_args(LiteralPosition)
+position_map = {
+    "position": position_values,
+    "left": ["top-left", "bottom-left"],
+    "right": ["top-right", "bottom-right"],
+    "top": ["top-left", "top-right"],
+    "bottom": ["bottom-left", "bottom-right"],
+}
+
+class ColorModeIconButton(IconButton):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        data: Optional[Union[Var[List[Dict[str, Any]]], List[Dict[str, Any]]]] = None,
-        min_angle: Optional[Union[Var[int], int]] = None,
-        legend_type: Optional[Union[Var[str], str]] = None,
-        label: Optional[Union[Var[bool], bool]] = None,
-        background: Optional[Union[Var[bool], bool]] = None,
-        style: Optional[Style] = None,
-        key: Optional[Any] = None,
-        id: Optional[Any] = None,
-        class_name: Optional[Any] = None,
-        autofocus: Optional[bool] = None,
-        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
-        on_click: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        position: Optional[
+            Literal["top-left", "top-right", "bottom-left", "bottom-right"]
         ] = None,
-        on_mouse_enter: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        as_child: Optional[Union[Var[bool], bool]] = None,
+        size: Optional[
+            Union[Var[Literal["1", "2", "3", "4"]], Literal["1", "2", "3", "4"]]
         ] = None,
-        on_mouse_leave: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        variant: Optional[
+            Union[
+                Var[Literal["classic", "solid", "soft", "surface", "outline", "ghost"]],
+                Literal["classic", "solid", "soft", "surface", "outline", "ghost"],
+            ]
         ] = None,
-        on_mouse_move: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        color_scheme: Optional[
+            Union[
+                Var[
+                    Literal[
+                        "tomato",
+                        "red",
+                        "ruby",
+                        "crimson",
+                        "pink",
+                        "plum",
+                        "purple",
+                        "violet",
+                        "iris",
+                        "indigo",
+                        "blue",
+                        "cyan",
+                        "teal",
+                        "jade",
+                        "green",
+                        "grass",
+                        "brown",
+                        "orange",
+                        "sky",
+                        "mint",
+                        "lime",
+                        "yellow",
+                        "amber",
+                        "gold",
+                        "bronze",
+                        "gray",
+                    ]
+                ],
+                Literal[
+                    "tomato",
+                    "red",
+                    "ruby",
+                    "crimson",
+                    "pink",
+                    "plum",
+                    "purple",
+                    "violet",
+                    "iris",
+                    "indigo",
+                    "blue",
+                    "cyan",
+                    "teal",
+                    "jade",
+                    "green",
+                    "grass",
+                    "brown",
+                    "orange",
+                    "sky",
+                    "mint",
+                    "lime",
+                    "yellow",
+                    "amber",
+                    "gold",
+                    "bronze",
+                    "gray",
+                ],
+            ]
         ] = None,
-        on_mouse_out: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        high_contrast: Optional[Union[Var[bool], bool]] = None,
+        radius: Optional[
+            Union[
+                Var[Literal["none", "small", "medium", "large", "full"]],
+                Literal["none", "small", "medium", "large", "full"],
+            ]
         ] = None,
-        on_mouse_over: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        auto_focus: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        **props
-    ) -> "RadialBar":
-        """Create the component.
-
-        Args:
-            *children: The children of the component.
-            data: The source data which each element is an object.
-            min_angle: Min angle of each bar. A positive value between 0 and 360.
-            legend_type: Type of legend
-            label: If false set, labels will not be drawn.
-            background: If false set, background sector will not be drawn.
-            style: The style of the component.
-            key: A unique key for the component.
-            id: The id for the component.
-            class_name: The class name for the component.
-            autofocus: Whether the component should take the focus once the page is loaded
-            custom_attrs: custom attribute
-            **props: The props of the component.
-
-        Returns:
-            The component.
-        """
-        ...
-
-class PolarAngleAxis(Recharts):
-    def get_event_triggers(self) -> dict[str, Union[Var, Any]]: ...
-    @overload
-    @classmethod
-    def create(  # type: ignore
-        cls,
-        *children,
-        data_key: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
-        cx: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
-        cy: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
-        radius: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
-        axis_line: Optional[
-            Union[Var[Union[bool, Dict[str, Any]]], Union[bool, Dict[str, Any]]]
-        ] = None,
-        axis_line_type: Optional[Union[Var[str], str]] = None,
-        tick_line: Optional[
-            Union[Var[Union[bool, Dict[str, Any]]], Union[bool, Dict[str, Any]]]
-        ] = None,
-        tick: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
-        ticks: Optional[Union[Var[List[Dict[str, Any]]], List[Dict[str, Any]]]] = None,
-        orient: Optional[Union[Var[str], str]] = None,
-        allow_duplicated_category: Optional[Union[Var[bool], bool]] = None,
-        style: Optional[Style] = None,
-        key: Optional[Any] = None,
-        id: Optional[Any] = None,
-        class_name: Optional[Any] = None,
-        autofocus: Optional[bool] = None,
-        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
-        on_click: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        disabled: Optional[Union[Var[bool], bool]] = None,
+        form: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        form_action: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_mouse_enter: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        form_enc_type: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_mouse_leave: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        form_method: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_mouse_move: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        form_no_validate: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_mouse_out: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        form_target: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_mouse_over: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        name: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        type: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        value: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        **props
-    ) -> "PolarAngleAxis":
-        """Create the component.
-
-        Args:
-            *children: The children of the component.
-            data_key: The key of a group of data which should be unique to show the meaning of angle axis.
-            cx: The x-coordinate of center. If set a percentage, the final value is obtained by multiplying the percentage of container width.
-            cy: The y-coordinate of center. If set a percentage, the final value is obtained by multiplying the percentage of container height.
-            radius: The outer radius of circle grid. If set a percentage, the final value is obtained by multiplying the percentage of maxRadius which is calculated by the width, height, cx, cy.
-            axis_line: If false set, axis line will not be drawn. If true set, axis line will be drawn which have the props calculated internally. If object set, axis line will be drawn which have the props mergered by the internal calculated props and the option.
-            axis_line_type: The type of axis line.
-            tick_line: If false set, tick lines will not be drawn. If true set, tick lines will be drawn which have the props calculated internally. If object set, tick lines will be drawn which have the props mergered by the internal calculated props and the option.
-            tick: The width or height of tick.
-            ticks: The array of every tick's value and angle.
-            orient: The orientation of axis text.
-            allow_duplicated_category: Allow the axis has duplicated categorys or not when the type of axis is "category".
-            style: The style of the component.
-            key: A unique key for the component.
-            id: The id for the component.
-            class_name: The class name for the component.
-            autofocus: Whether the component should take the focus once the page is loaded
-            custom_attrs: custom attribute
-            **props: The props of the component.
-
-        Returns:
-            The component.
-        """
-        ...
-
-class PolarGrid(Recharts):
-    @overload
-    @classmethod
-    def create(  # type: ignore
-        cls,
-        *children,
-        cx: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
-        cy: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
-        inner_radius: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
-        outer_radius: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
-        polar_angles: Optional[Union[Var[List[int]], List[int]]] = None,
-        polar_radius: Optional[Union[Var[List[int]], List[int]]] = None,
-        grid_type: Optional[
-            Union[Var[Literal["polygon", "circle"]], Literal["polygon", "circle"]]
+        access_key: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        auto_capitalize: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        content_editable: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
+        context_menu: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        dir: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        draggable: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        enter_key_hint: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        hidden: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        input_mode: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        item_prop: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        lang: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        role: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        slot: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        spell_check: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        tab_index: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        title: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        loading: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -402,109 +306,187 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "PolarGrid":
-        """Create the component.
+    ) -> "ColorModeIconButton":
+        """Create a icon button component that calls toggle_color_mode on click.
 
         Args:
             *children: The children of the component.
-            cx: The x-coordinate of center. If set a percentage, the final value is obtained by multiplying the percentage of container width.
-            cy: The y-coordinate of center. If set a percentage, the final value is obtained by multiplying the percentage of container height.
-            inner_radius: The radius of the inner polar grid.
-            outer_radius: The radius of the outer polar grid.
-            polar_angles: The array of every line grid's angle.
-            polar_radius: The array of every line grid's radius.
-            grid_type: The type of polar grids. 'polygon' | 'circle'
+            position: The position of the icon button. Follow document flow if None.
+            as_child: Change the default rendered element for the one passed as a child, merging their props and behavior.
+            size: Button size "1" - "4"
+            variant: Variant of button: "classic" | "solid" | "soft" | "surface" | "outline" | "ghost"
+            color_scheme: Override theme color for button
+            high_contrast: Whether to render the button with higher contrast color against background
+            radius: Override theme radius for button: "none" | "small" | "medium" | "large" | "full"
+            auto_focus: Automatically focuses the button when the page loads
+            disabled: Disables the button
+            form: Associates the button with a form (by id)
+            form_action: URL to send the form data to (for type="submit" buttons)
+            form_enc_type: How the form data should be encoded when submitting to the server (for type="submit" buttons)
+            form_method: HTTP method to use for sending form data (for type="submit" buttons)
+            form_no_validate: Bypasses form validation when submitting (for type="submit" buttons)
+            form_target: Specifies where to display the response after submitting the form (for type="submit" buttons)
+            name: Name of the button, used when sending form data
+            type: Type of the button (submit, reset, or button)
+            value: Value of the button, used when sending form data
+            access_key:  Provides a hint for generating a keyboard shortcut for the current element.
+            auto_capitalize: Controls whether and how text input is automatically capitalized as it is entered/edited by the user.
+            content_editable: Indicates whether the element's content is editable.
+            context_menu: Defines the ID of a <menu> element which will serve as the element's context menu.
+            dir: Defines the text direction. Allowed values are ltr (Left-To-Right) or rtl (Right-To-Left)
+            draggable: Defines whether the element can be dragged.
+            enter_key_hint: Hints what media types the media element is able to play.
+            hidden: Defines whether the element is hidden.
+            input_mode: Defines the type of the element.
+            item_prop: Defines the name of the element for metadata purposes.
+            lang: Defines the language used in the element.
+            role: Defines the role of the element.
+            slot: Assigns a slot in a shadow DOM shadow tree to an element.
+            spell_check: Defines whether the element may be checked for spelling errors.
+            tab_index: Defines the position of the current element in the tabbing order.
+            title: Defines a tooltip for the element.
+            loading: If set, show an rx.spinner instead of the component children.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: The props of the component.
+            **props: The props to pass to the component.
 
         Returns:
-            The component.
+            The button component.
         """
         ...
 
-class PolarRadiusAxis(Recharts):
-    def get_event_triggers(self) -> dict[str, Union[Var, Any]]: ...
+class ColorModeSwitch(Switch):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        angle: Optional[Union[Var[int], int]] = None,
-        type_: Optional[
-            Union[Var[Literal["number", "category"]], Literal["number", "category"]]
-        ] = None,
-        allow_duplicated_category: Optional[Union[Var[bool], bool]] = None,
-        cx: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
-        cy: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
-        reversed: Optional[Union[Var[bool], bool]] = None,
-        orientation: Optional[Union[Var[str], str]] = None,
-        axis_line: Optional[
-            Union[Var[Union[bool, Dict[str, Any]]], Union[bool, Dict[str, Any]]]
-        ] = None,
-        tick: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
-        tick_count: Optional[Union[Var[int], int]] = None,
-        scale: Optional[
+        as_child: Optional[Union[Var[bool], bool]] = None,
+        default_checked: Optional[Union[Var[bool], bool]] = None,
+        checked: Optional[Union[Var[bool], bool]] = None,
+        disabled: Optional[Union[Var[bool], bool]] = None,
+        required: Optional[Union[Var[bool], bool]] = None,
+        name: Optional[Union[Var[str], str]] = None,
+        value: Optional[Union[Var[str], str]] = None,
+        size: Optional[
+            Union[Var[Literal["1", "2", "3"]], Literal["1", "2", "3"]]
+        ] = None,
+        variant: Optional[
+            Union[
+                Var[Literal["classic", "surface", "soft"]],
+                Literal["classic", "surface", "soft"],
+            ]
+        ] = None,
+        color_scheme: Optional[
             Union[
                 Var[
                     Literal[
-                        "auto",
-                        "linear",
-                        "pow",
-                        "sqrt",
-                        "log",
-                        "identity",
-                        "time",
-                        "band",
-                        "point",
-                        "ordinal",
-                        "quantile",
-                        "quantize",
-                        "utc",
-                        "sequential",
-                        "threshold",
+                        "tomato",
+                        "red",
+                        "ruby",
+                        "crimson",
+                        "pink",
+                        "plum",
+                        "purple",
+                        "violet",
+                        "iris",
+                        "indigo",
+                        "blue",
+                        "cyan",
+                        "teal",
+                        "jade",
+                        "green",
+                        "grass",
+                        "brown",
+                        "orange",
+                        "sky",
+                        "mint",
+                        "lime",
+                        "yellow",
+                        "amber",
+                        "gold",
+                        "bronze",
+                        "gray",
                     ]
                 ],
                 Literal[
-                    "auto",
-                    "linear",
-                    "pow",
-                    "sqrt",
-                    "log",
-                    "identity",
-                    "time",
-                    "band",
-                    "point",
-                    "ordinal",
-                    "quantile",
-                    "quantize",
-                    "utc",
-                    "sequential",
-                    "threshold",
+                    "tomato",
+                    "red",
+                    "ruby",
+                    "crimson",
+                    "pink",
+                    "plum",
+                    "purple",
+                    "violet",
+                    "iris",
+                    "indigo",
+                    "blue",
+                    "cyan",
+                    "teal",
+                    "jade",
+                    "green",
+                    "grass",
+                    "brown",
+                    "orange",
+                    "sky",
+                    "mint",
+                    "lime",
+                    "yellow",
+                    "amber",
+                    "gold",
+                    "bronze",
+                    "gray",
                 ],
             ]
         ] = None,
+        high_contrast: Optional[Union[Var[bool], bool]] = None,
+        radius: Optional[
+            Union[
+                Var[Literal["none", "small", "full"]], Literal["none", "small", "full"]
+            ]
+        ] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
+        on_blur: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_change: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_context_menu: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_double_click: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_focus: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mount: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_down: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_mouse_enter: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_leave: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_move: Optional[
@@ -512,36 +494,53 @@
         ] = None,
         on_mouse_out: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_over: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_mouse_up: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_scroll: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_unmount: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         **props
-    ) -> "PolarRadiusAxis":
-        """Create the component.
+    ) -> "ColorModeSwitch":
+        """Create a switch component bound to color_mode.
 
         Args:
             *children: The children of the component.
-            angle: The angle of radial direction line to display axis text.
-            type_: The type of axis line. 'number' | 'category'
-            allow_duplicated_category: Allow the axis has duplicated categorys or not when the type of axis is "category".
-            cx: The x-coordinate of center.
-            cy: The y-coordinate of center.
-            reversed: If set to true, the ticks of this axis are reversed.
-            orientation: The orientation of axis text.
-            axis_line: If false set, axis line will not be drawn. If true set, axis line will be drawn which have the props calculated internally. If object set, axis line will be drawn which have the props mergered by the internal calculated props and the option.
-            tick: The width or height of tick.
-            tick_count: The count of ticks.
-            scale: If 'auto' set, the scale funtion is linear scale. 'auto' | 'linear' | 'pow' | 'sqrt' | 'log' | 'identity' | 'time' | 'band' | 'point' | 'ordinal' | 'quantile' | 'quantize' | 'utc' | 'sequential' | 'threshold'
+            as_child: Change the default rendered element for the one passed as a child, merging their props and behavior.
+            default_checked: Whether the switch is checked by default
+            checked: Whether the switch is checked
+            disabled: If true, prevent the user from interacting with the switch
+            required: If true, the user must interact with the switch to submit the form
+            name: The name of the switch (when submitting a form)
+            value: The value associated with the "on" position
+            size: Switch size "1" - "4"
+            variant: Variant of switch: "classic" | "surface" | "soft"
+            color_scheme: Override theme color for switch
+            high_contrast: Whether to render the switch with higher contrast color against background
+            radius: Override theme radius for switch: "none" | "small" | "full"
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: The props of the component.
+            **props: The props to pass to the component.
 
         Returns:
-            The component.
+            The switch component.
         """
         ...
+
+class ColorModeNamespace(BaseVar):
+    icon = staticmethod(ColorModeIcon.create)
+    button = staticmethod(ColorModeIconButton.create)
+    switch = staticmethod(ColorModeSwitch.create)
+
+color_mode_var_and_namespace = ColorModeNamespace(**dataclasses.asdict(color_mode))
```

### Comparing `reflex-0.5.0a2/reflex/components/recharts/recharts.py` & `reflex-0.5.0a3/reflex/components/recharts/recharts.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/recharts/recharts.pyi` & `reflex-0.5.0a3/reflex/components/recharts/recharts.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/sonner/toast.py` & `reflex-0.5.0a3/reflex/components/sonner/toast.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/sonner/toast.pyi` & `reflex-0.5.0a3/reflex/components/sonner/toast.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/suneditor/editor.py` & `reflex-0.5.0a3/reflex/components/suneditor/editor.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/suneditor/editor.pyi` & `reflex-0.5.0a3/reflex/components/suneditor/editor.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/tags/iter_tag.py` & `reflex-0.5.0a3/reflex/components/tags/iter_tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/tags/tag.py` & `reflex-0.5.0a3/reflex/components/tags/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/components/tags/tagless.py` & `reflex-0.5.0a3/reflex/components/tags/tagless.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/config.py` & `reflex-0.5.0a3/reflex/config.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/config.pyi` & `reflex-0.5.0a3/reflex/config.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/constants/__init__.py` & `reflex-0.5.0a3/reflex/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/constants/base.py` & `reflex-0.5.0a3/reflex/constants/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/constants/base.pyi` & `reflex-0.5.0a3/reflex/constants/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/constants/colors.py` & `reflex-0.5.0a3/reflex/constants/colors.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/constants/compiler.py` & `reflex-0.5.0a3/reflex/constants/compiler.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/constants/config.py` & `reflex-0.5.0a3/reflex/constants/config.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/constants/custom_components.py` & `reflex-0.5.0a3/reflex/constants/custom_components.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/constants/event.py` & `reflex-0.5.0a3/reflex/constants/event.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/constants/installer.py` & `reflex-0.5.0a3/reflex/constants/installer.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/constants/route.py` & `reflex-0.5.0a3/reflex/constants/route.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/constants/style.py` & `reflex-0.5.0a3/reflex/constants/style.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/custom_components/custom_components.py` & `reflex-0.5.0a3/reflex/custom_components/custom_components.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 import typer
 from tomlkit.exceptions import TOMLKitError
 
 from reflex import constants
 from reflex.config import get_config
 from reflex.constants import CustomComponents
 from reflex.utils import console
-from reflex.utils.pyi_generator import PyiGenerator
 
 config = get_config()
 custom_components_cli = typer.Typer()
 
 POST_CUSTOM_COMPONENTS_GALLERY_ENDPOINT = (
     f"{config.cp_backend_url}/custom-components/gallery"
 )
@@ -434,14 +433,16 @@
         console.error(cpe.stdout)
         console.error(cpe.stderr)
         return False
 
 
 def _make_pyi_files():
     """Create pyi files for the custom component."""
+    from reflex.utils.pyi_generator import PyiGenerator
+
     package_name = _get_package_config()["project"]["name"]
 
     for dir, _, _ in os.walk(f"./{package_name}"):
         if "__pycache__" in dir:
             continue
         PyiGenerator().scan_all([dir])
```

### Comparing `reflex-0.5.0a2/reflex/event.py` & `reflex-0.5.0a3/reflex/event.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/experimental/__init__.py` & `reflex-0.5.0a3/reflex/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/experimental/hooks.py` & `reflex-0.5.0a3/reflex/experimental/hooks.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/experimental/layout.py` & `reflex-0.5.0a3/reflex/experimental/layout.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/middleware/hydrate_middleware.py` & `reflex-0.5.0a3/reflex/middleware/hydrate_middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/middleware/middleware.py` & `reflex-0.5.0a3/reflex/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/model.py` & `reflex-0.5.0a3/reflex/model.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/page.py` & `reflex-0.5.0a3/reflex/page.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/reflex.py` & `reflex-0.5.0a3/reflex/reflex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/route.py` & `reflex-0.5.0a3/reflex/route.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/state.py` & `reflex-0.5.0a3/reflex/state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/style.py` & `reflex-0.5.0a3/reflex/style.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/testing.py` & `reflex-0.5.0a3/reflex/testing.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/utils/build.py` & `reflex-0.5.0a3/reflex/utils/build.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/utils/compat.py` & `reflex-0.5.0a3/reflex/utils/compat.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/utils/console.py` & `reflex-0.5.0a3/reflex/utils/console.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/utils/exec.py` & `reflex-0.5.0a3/reflex/utils/exec.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/utils/export.py` & `reflex-0.5.0a3/reflex/utils/export.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/utils/format.py` & `reflex-0.5.0a3/reflex/utils/format.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/utils/imports.py` & `reflex-0.5.0a3/reflex/utils/imports.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/utils/path_ops.py` & `reflex-0.5.0a3/reflex/utils/path_ops.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/utils/prerequisites.py` & `reflex-0.5.0a3/reflex/utils/prerequisites.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/utils/processes.py` & `reflex-0.5.0a3/reflex/utils/processes.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/utils/pyi_generator.py` & `reflex-0.5.0a3/reflex/utils/pyi_generator.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/utils/serializers.py` & `reflex-0.5.0a3/reflex/utils/serializers.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/utils/telemetry.py` & `reflex-0.5.0a3/reflex/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/utils/types.py` & `reflex-0.5.0a3/reflex/utils/types.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/utils/watch.py` & `reflex-0.5.0a3/reflex/utils/watch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/vars.py` & `reflex-0.5.0a3/reflex/vars.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/reflex/vars.pyi` & `reflex-0.5.0a3/reflex/vars.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a2/PKG-INFO` & `reflex-0.5.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex
-Version: 0.5.0a2
+Version: 0.5.0a3
 Summary: Web apps in pure Python.
 Home-page: https://reflex.dev
 License: Apache-2.0
 Keywords: web,framework
 Author: Nikhil Rao
 Author-email: nikhil@reflex.dev
 Requires-Python: >=3.8,<4.0
```

