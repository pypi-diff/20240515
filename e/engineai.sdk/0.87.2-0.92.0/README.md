# Comparing `tmp/engineai_sdk-0.87.2.tar.gz` & `tmp/engineai_sdk-0.92.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "engineai_sdk-0.87.2.tar", max compression
+gzip compressed data, was "engineai_sdk-0.92.0.tar", max compression
```

## Comparing `engineai_sdk-0.87.2.tar` & `engineai_sdk-0.92.0.tar`

### file list

```diff
@@ -1,366 +1,365 @@
--rw-r--r--   0        0        0     1065 2024-04-24 14:07:11.083692 engineai_sdk-0.87.2/LICENSE
--rw-r--r--   0        0        0      987 2024-04-24 14:07:11.083692 engineai_sdk-0.87.2/README.md
--rw-r--r--   0        0        0      435 2024-04-24 14:07:11.083692 engineai_sdk-0.87.2/engineai/sdk/__init__.py
--rw-r--r--   0        0        0       28 2024-04-24 14:07:11.083692 engineai_sdk-0.87.2/engineai/sdk/cli/__init__.py
--rw-r--r--   0        0        0       33 2024-04-24 14:07:11.083692 engineai_sdk-0.87.2/engineai/sdk/cli/commands/__init__.py
--rw-r--r--   0        0        0     2541 2024-04-24 14:07:11.083692 engineai_sdk-0.87.2/engineai/sdk/cli/commands/app.py
--rw-r--r--   0        0        0    14251 2024-04-24 14:07:11.083692 engineai_sdk-0.87.2/engineai/sdk/cli/commands/dashboard.py
--rw-r--r--   0        0        0     1379 2024-04-24 14:07:11.083692 engineai_sdk-0.87.2/engineai/sdk/cli/console.py
--rw-r--r--   0        0        0     4806 2024-04-24 14:07:11.083692 engineai_sdk-0.87.2/engineai/sdk/cli/generator.py
--rw-r--r--   0        0        0       43 2024-04-24 14:07:11.083692 engineai_sdk-0.87.2/engineai/sdk/cli/template/content/.env.sample
--rw-r--r--   0        0        0     5396 2024-04-24 14:07:11.083692 engineai_sdk-0.87.2/engineai/sdk/cli/template/content/data/example.json
--rw-r--r--   0        0        0      411 2024-04-24 14:07:11.083692 engineai_sdk-0.87.2/engineai/sdk/cli/template/content/main.py
--rw-r--r--   0        0        0    10363 2024-04-24 14:07:11.083692 engineai_sdk-0.87.2/engineai/sdk/cli/utils.py
--rw-r--r--   0        0        0       38 2024-04-24 14:07:11.083692 engineai_sdk-0.87.2/engineai/sdk/dashboard/__init__.py
--rw-r--r--   0        0        0      121 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/abstract/__init__.py
--rw-r--r--   0        0        0     2181 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/abstract/layout.py
--rw-r--r--   0        0        0      207 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/abstract/selectable_widgets.py
--rw-r--r--   0        0        0      570 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/abstract/typing.py
--rw-r--r--   0        0        0     1600 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/base.py
--rw-r--r--   0        0        0       96 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/clients/__init__.py
--rw-r--r--   0        0        0     3574 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/clients/activate_dashboard.py
--rw-r--r--   0        0        0     7670 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/clients/api.py
--rw-r--r--   0        0        0     1451 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/clients/exceptions.py
--rw-r--r--   0        0        0      217 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/clients/storage/__init__.py
--rw-r--r--   0        0        0      472 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/clients/storage/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/clients/storage/py.typed
--rw-r--r--   0        0        0      207 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/clients/storage/serialization/__init__.py
--rw-r--r--   0        0        0     6861 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/clients/storage/serialization/dataframe.py
--rw-r--r--   0        0        0     3134 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/clients/storage/serialization/json.py
--rw-r--r--   0        0        0     4618 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/clients/storage/storage.py
--rw-r--r--   0        0        0      515 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/config.py
--rw-r--r--   0        0        0      310 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/__init__.py
--rw-r--r--   0        0        0    13364 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/dashboard.py
--rw-r--r--   0        0        0      140 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/enums.py
--rw-r--r--   0        0        0     4691 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/exceptions.py
--rw-r--r--   0        0        0       27 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/graph/__init__.py
--rw-r--r--   0        0        0     2417 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/graph/executor_config.py
--rw-r--r--   0        0        0     8389 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/graph/instance.py
--rw-r--r--   0        0        0     1231 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/graph/node.py
--rw-r--r--   0        0        0     2586 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/graph/utils.py
--rw-r--r--   0        0        0       41 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/page/__init__.py
--rw-r--r--   0        0        0     1431 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/page/dependency.py
--rw-r--r--   0        0        0     5667 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/page/page.py
--rw-r--r--   0        0        0     1909 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/page/root.py
--rw-r--r--   0        0        0     2932 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/page/route.py
--rw-r--r--   0        0        0      345 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/typings.py
--rw-r--r--   0        0        0       33 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/version/__init__.py
--rw-r--r--   0        0        0     5105 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/version/version.py
--rw-r--r--   0        0        0      185 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/data/__init__.py
--rw-r--r--   0        0        0    12893 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/data/decorator.py
--rw-r--r--   0        0        0     1822 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/data/duplicated.py
--rw-r--r--   0        0        0     1047 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/data/enums.py
--rw-r--r--   0        0        0     4676 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/data/exceptions.py
--rw-r--r--   0        0        0     1996 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/data/http.py
--rw-r--r--   0        0        0     3616 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/data/io_handler.py
--rw-r--r--   0        0        0     1306 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/data/manager/interface.py
--rw-r--r--   0        0        0     9994 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/data/manager/manager.py
--rw-r--r--   0        0        0     2892 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/decorator.py
--rw-r--r--   0        0        0      441 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dependencies/__init__.py
--rw-r--r--   0        0        0     3521 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dependencies/datastore.py
--rw-r--r--   0        0        0      141 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dependencies/http/__init__.py
--rw-r--r--   0        0        0      966 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dependencies/http/header.py
--rw-r--r--   0        0        0     2555 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dependencies/http/http.py
--rw-r--r--   0        0        0     2026 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dependencies/route.py
--rw-r--r--   0        0        0     2518 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dependencies/widget.py
--rw-r--r--   0        0        0      369 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/enum/__init__.py
--rw-r--r--   0        0        0     1112 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/enum/align.py
--rw-r--r--   0        0        0      741 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/enum/legend_position.py
--rw-r--r--   0        0        0     5156 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/exceptions.py
--rw-r--r--   0        0        0      569 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/formatting/__init__.py
--rw-r--r--   0        0        0     3817 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/formatting/axis.py
--rw-r--r--   0        0        0     1888 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/formatting/datetime.py
--rw-r--r--   0        0        0      661 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/formatting/exceptions.py
--rw-r--r--   0        0        0     1331 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/formatting/mapper.py
--rw-r--r--   0        0        0     5254 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/formatting/number.py
--rw-r--r--   0        0        0     1421 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/formatting/text.py
--rw-r--r--   0        0        0      331 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/formatting/typing.py
--rw-r--r--   0        0        0      985 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/formatting/validator.py
--rw-r--r--   0        0        0     1056 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/interface.py
--rw-r--r--   0        0        0      825 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/__init__.py
--rw-r--r--   0        0        0      417 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/build_item.py
--rw-r--r--   0        0        0       28 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/card/__init__.py
--rw-r--r--   0        0        0     5990 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/card/card.py
--rw-r--r--   0        0        0     2889 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/card/chip.py
--rw-r--r--   0        0        0     1679 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/card/header.py
--rw-r--r--   0        0        0       55 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/collapsible/__init__.py
--rw-r--r--   0        0        0     3082 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/collapsible/chip.py
--rw-r--r--   0        0        0     1968 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/collapsible/header.py
--rw-r--r--   0        0        0     6641 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/collapsible/section.py
--rw-r--r--   0        0        0     5999 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/column.py
--rw-r--r--   0        0        0     2679 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/components/chip.py
--rw-r--r--   0        0        0     2165 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/components/header.py
--rw-r--r--   0        0        0     2385 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/components/label.py
--rw-r--r--   0        0        0     4695 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/exceptions.py
--rw-r--r--   0        0        0       31 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/fluid_row/__init__.py
--rw-r--r--   0        0        0     5791 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/fluid_row/fluid_row.py
--rw-r--r--   0        0        0     1921 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/fluid_row/items_build.py
--rw-r--r--   0        0        0     7313 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/grid.py
--rw-r--r--   0        0        0    10423 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/row.py
--rw-r--r--   0        0        0       36 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/selectable/__init__.py
--rw-r--r--   0        0        0     7582 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/selectable/base.py
--rw-r--r--   0        0        0     2171 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/selectable/exceptions.py
--rw-r--r--   0        0        0     4397 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/selectable/tab.py
--rw-r--r--   0        0        0      676 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/typings.py
--rw-r--r--   0        0        0      244 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/links/__init__.py
--rw-r--r--   0        0        0     6016 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/links/abstract.py
--rw-r--r--   0        0        0     2201 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/links/route_link.py
--rw-r--r--   0        0        0     2576 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/links/template_string_link.py
--rw-r--r--   0        0        0      202 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/links/typing.py
--rw-r--r--   0        0        0     1427 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/links/url.py
--rw-r--r--   0        0        0      934 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/links/widget_dependency.py
--rw-r--r--   0        0        0     3039 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/links/widget_field.py
--rw-r--r--   0        0        0        0 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/py.typed
--rw-r--r--   0        0        0     2020 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/selected.py
--rw-r--r--   0        0        0      100 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/__init__.py
--rw-r--r--   0        0        0      744 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/color/__init__.py
--rw-r--r--   0        0        0     5872 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/color/default_specs.py
--rw-r--r--   0        0        0     6985 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/color/discrete_map.py
--rw-r--r--   0        0        0     1679 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/color/divergent.py
--rw-r--r--   0        0        0     4055 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/color/gradient.py
--rw-r--r--   0        0        0     5949 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/color/palette.py
--rw-r--r--   0        0        0      920 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/color/single.py
--rw-r--r--   0        0        0      946 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/color/spec.py
--rw-r--r--   0        0        0      436 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/color/typing.py
--rw-r--r--   0        0        0     3436 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/icons.py
--rw-r--r--   0        0        0     8298 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/templated_string.py
--rw-r--r--   0        0        0     3514 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/utils.py
--rw-r--r--   0        0        0       25 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/__init__.py
--rw-r--r--   0        0        0     8541 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/base.py
--rw-r--r--   0        0        0     2647 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/__init__.py
--rw-r--r--   0        0        0       44 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/axis/__init__.py
--rw-r--r--   0        0        0     3566 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/axis/base.py
--rw-r--r--   0        0        0      365 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/axis/typing.py
--rw-r--r--   0        0        0     2149 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/axis/x_axis.py
--rw-r--r--   0        0        0     5237 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/axis/y_axis.py
--rw-r--r--   0        0        0     4410 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/cartesian.py
--rw-r--r--   0        0        0     4481 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/chart.py
--rw-r--r--   0        0        0     1468 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/exceptions.py
--rw-r--r--   0        0        0      987 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/legend.py
--rw-r--r--   0        0        0       45 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/series/__init__.py
--rw-r--r--   0        0        0     2640 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/series/area.py
--rw-r--r--   0        0        0     4026 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/series/area_range.py
--rw-r--r--   0        0        0     7256 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/series/base.py
--rw-r--r--   0        0        0     5303 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/series/bubble.py
--rw-r--r--   0        0        0     2660 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/series/column.py
--rw-r--r--   0        0        0     2640 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/series/line.py
--rw-r--r--   0        0        0     2679 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/series/scatter.py
--rw-r--r--   0        0        0      573 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/series/typing.py
--rw-r--r--   0        0        0     4957 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/chart_utils.py
--rw-r--r--   0        0        0       39 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/__init__.py
--rw-r--r--   0        0        0       87 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/actions/links/__init__.py
--rw-r--r--   0        0        0     2630 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/actions/links/base.py
--rw-r--r--   0        0        0     1475 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/actions/links/exceptions.py
--rw-r--r--   0        0        0     1910 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/actions/links/url_link.py
--rw-r--r--   0        0        0       47 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/__init__.py
--rw-r--r--   0        0        0       56 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/axis/__init__.py
--rw-r--r--   0        0        0      416 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/axis/scale/__init__.py
--rw-r--r--   0        0        0     1079 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/axis/scale/dynamic.py
--rw-r--r--   0        0        0     1764 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/axis/scale/negative.py
--rw-r--r--   0        0        0     1764 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/axis/scale/positive.py
--rw-r--r--   0        0        0     1117 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/axis/scale/scale.py
--rw-r--r--   0        0        0     2785 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/axis/scale/symmetric.py
--rw-r--r--   0        0        0      338 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/axis/scale/typing.py
--rw-r--r--   0        0        0      151 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/consts.py
--rw-r--r--   0        0        0     7162 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/exceptions.py
--rw-r--r--   0        0        0       25 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/series/__init__.py
--rw-r--r--   0        0        0     2787 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/series/base.py
--rw-r--r--   0        0        0       23 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/series/entities/__init__.py
--rw-r--r--   0        0        0      955 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/series/entities/base.py
--rw-r--r--   0        0        0     2138 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/series/entities/country.py
--rw-r--r--   0        0        0      806 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/series/entities/custom.py
--rw-r--r--   0        0        0      314 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/series/entities/typing.py
--rw-r--r--   0        0        0      696 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/__init__.py
--rw-r--r--   0        0        0     1491 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/area.py
--rw-r--r--   0        0        0     1573 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/area_range.py
--rw-r--r--   0        0        0     4041 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/base.py
--rw-r--r--   0        0        0     3527 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/bubble_circle.py
--rw-r--r--   0        0        0     3132 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/bubble_country.py
--rw-r--r--   0        0        0     1484 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/column.py
--rw-r--r--   0        0        0     1047 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/enums.py
--rw-r--r--   0        0        0     1540 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/error_bar.py
--rw-r--r--   0        0        0     3635 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/line.py
--rw-r--r--   0        0        0     1473 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/point.py
--rw-r--r--   0        0        0     1514 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/scatter.py
--rw-r--r--   0        0        0      802 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/typing.py
--rw-r--r--   0        0        0      282 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/toolbar.py
--rw-r--r--   0        0        0      319 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/__init__.py
--rw-r--r--   0        0        0     3647 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/base.py
--rw-r--r--   0        0        0     1490 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/category.py
--rw-r--r--   0        0        0     1641 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/datetime.py
--rw-r--r--   0        0        0      617 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/exceptions.py
--rw-r--r--   0        0        0     1102 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/item.py
--rw-r--r--   0        0        0     1526 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/number.py
--rw-r--r--   0        0        0     1594 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/text.py
--rw-r--r--   0        0        0      647 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/typing.py
--rw-r--r--   0        0        0       29 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/__init__.py
--rw-r--r--   0        0        0     1192 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/__init__.py
--rw-r--r--   0        0        0     4758 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/base.py
--rw-r--r--   0        0        0       35 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/chart/__init__.py
--rw-r--r--   0        0        0      228 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/chart/area.py
--rw-r--r--   0        0        0      236 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/chart/column.py
--rw-r--r--   0        0        0      228 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/chart/line.py
--rw-r--r--   0        0        0     1184 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/chart/stacked_bar.py
--rw-r--r--   0        0        0      379 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/chart/typing.py
--rw-r--r--   0        0        0      974 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/exceptions.py
--rw-r--r--   0        0        0       36 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/number/__init__.py
--rw-r--r--   0        0        0     1451 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/number/arrow.py
--rw-r--r--   0        0        0      902 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/number/chip.py
--rw-r--r--   0        0        0      893 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/number/dot.py
--rw-r--r--   0        0        0      906 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/number/font.py
--rw-r--r--   0        0        0     1263 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/number/progress_bar.py
--rw-r--r--   0        0        0      339 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/number/typing.py
--rw-r--r--   0        0        0       34 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/text/__init__.py
--rw-r--r--   0        0        0      879 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/text/chip.py
--rw-r--r--   0        0        0     1388 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/text/country_flag.py
--rw-r--r--   0        0        0      943 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/text/dot.py
--rw-r--r--   0        0        0      903 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/text/font.py
--rw-r--r--   0        0        0      331 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/text/typing.py
--rw-r--r--   0        0        0     1313 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/tooltip/format_build.py
--rw-r--r--   0        0        0     2014 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/tooltip/header.py
--rw-r--r--   0        0        0     2003 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/tooltip/tooltip.py
--rw-r--r--   0        0        0      136 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/content/__init__.py
--rw-r--r--   0        0        0     2890 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/content/content.py
--rw-r--r--   0        0        0     1265 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/content/exceptions.py
--rw-r--r--   0        0        0      613 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/content/item.py
--rw-r--r--   0        0        0     1431 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/content/markdown.py
--rw-r--r--   0        0        0     3756 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/exceptions.py
--rw-r--r--   0        0        0      573 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/__init__.py
--rw-r--r--   0        0        0     1369 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/color_axis.py
--rw-r--r--   0        0        0     1043 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/enums.py
--rw-r--r--   0        0        0      980 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/exceptions.py
--rw-r--r--   0        0        0       25 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/geo/__init__.py
--rw-r--r--   0        0        0     8048 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/geo/base.py
--rw-r--r--   0        0        0     4272 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/geo/geo.py
--rw-r--r--   0        0        0       29 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/geo/styling/__init__.py
--rw-r--r--   0        0        0      832 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/geo/styling/label.py
--rw-r--r--   0        0        0      988 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/geo/styling/styling.py
--rw-r--r--   0        0        0      954 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/legend.py
--rw-r--r--   0        0        0       42 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/series/__init__.py
--rw-r--r--   0        0        0     4887 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/series/numeric.py
--rw-r--r--   0        0        0      625 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/series/series.py
--rw-r--r--   0        0        0     2937 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/series/styling.py
--rw-r--r--   0        0        0     2113 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pandas_utils.py
--rw-r--r--   0        0        0      672 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/__init__.py
--rw-r--r--   0        0        0     1949 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/chart.py
--rw-r--r--   0        0        0      852 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/exceptions.py
--rw-r--r--   0        0        0      851 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/legend.py
--rw-r--r--   0        0        0     6296 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/pie.py
--rw-r--r--   0        0        0       35 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/series/__init__.py
--rw-r--r--   0        0        0     6044 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/series/base.py
--rw-r--r--   0        0        0     3413 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/series/country.py
--rw-r--r--   0        0        0     3059 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/series/series.py
--rw-r--r--   0        0        0     3185 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/series/styling.py
--rw-r--r--   0        0        0      165 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/series/typings.py
--rw-r--r--   0        0        0     2402 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/tooltip.py
--rw-r--r--   0        0        0      391 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/__init__.py
--rw-r--r--   0        0        0     3415 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/exceptions.py
--rw-r--r--   0        0        0       28 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/results/__init__.py
--rw-r--r--   0        0        0     2793 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/results/base.py
--rw-r--r--   0        0        0      900 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/results/build_result.py
--rw-r--r--   0        0        0     3470 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/results/number.py
--rw-r--r--   0        0        0       21 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/results/styling/__init__.py
--rw-r--r--   0        0        0     3252 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/results/styling/base_styling.py
--rw-r--r--   0        0        0     1523 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/results/styling/number.py
--rw-r--r--   0        0        0     1712 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/results/styling/text.py
--rw-r--r--   0        0        0     2432 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/results/text.py
--rw-r--r--   0        0        0      280 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/results/typing.py
--rw-r--r--   0        0        0     8158 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/search.py
--rw-r--r--   0        0        0       79 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/select/__init__.py
--rw-r--r--   0        0        0     2135 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/select/exceptions.py
--rw-r--r--   0        0        0     1783 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/select/group.py
--rw-r--r--   0        0        0     6575 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/select/select.py
--rw-r--r--   0        0        0     2453 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/__init__.py
--rw-r--r--   0        0        0       50 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/__init__.py
--rw-r--r--   0        0        0       26 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/__init__.py
--rw-r--r--   0        0        0     6147 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/base.py
--rw-r--r--   0        0        0     6201 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/category.py
--rw-r--r--   0        0        0       46 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/charts/__init__.py
--rw-r--r--   0        0        0     5611 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/charts/area.py
--rw-r--r--   0        0        0     6726 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/charts/base.py
--rw-r--r--   0        0        0     5672 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/charts/column.py
--rw-r--r--   0        0        0     5669 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/charts/line.py
--rw-r--r--   0        0        0     5330 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/charts/stack_bar.py
--rw-r--r--   0        0        0     5103 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/country.py
--rw-r--r--   0        0        0     5869 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/datetime.py
--rw-r--r--   0        0        0     4011 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/exceptions.py
--rw-r--r--   0        0        0     6105 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/number.py
--rw-r--r--   0        0        0     5601 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/range.py
--rw-r--r--   0        0        0     5419 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/text.py
--rw-r--r--   0        0        0     3727 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/url_column.py
--rw-r--r--   0        0        0       49 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/__init__.py
--rw-r--r--   0        0        0     1146 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/area.py
--rw-r--r--   0        0        0     1659 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/arrow.py
--rw-r--r--   0        0        0     5055 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/base.py
--rw-r--r--   0        0        0     1541 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/cell.py
--rw-r--r--   0        0        0     2510 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/color_bar.py
--rw-r--r--   0        0        0     1161 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/column.py
--rw-r--r--   0        0        0     1321 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/country_flag.py
--rw-r--r--   0        0        0     1271 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/dot.py
--rw-r--r--   0        0        0     1537 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/exceptions.py
--rw-r--r--   0        0        0     1418 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/font.py
--rw-r--r--   0        0        0     1233 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/icon.py
--rw-r--r--   0        0        0     1147 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/line.py
--rw-r--r--   0        0        0     1494 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/range.py
--rw-r--r--   0        0        0     2723 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/split_bar.py
--rw-r--r--   0        0        0     1727 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/stacked_bar.py
--rw-r--r--   0        0        0     1779 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/utils.py
--rw-r--r--   0        0        0      473 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/enums.py
--rw-r--r--   0        0        0     5447 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/exceptions.py
--rw-r--r--   0        0        0     1864 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/group.py
--rw-r--r--   0        0        0     9162 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/header.py
--rw-r--r--   0        0        0     2713 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/initial_state.py
--rw-r--r--   0        0        0     2046 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/styling.py
--rw-r--r--   0        0        0    17305 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/table.py
--rw-r--r--   0        0        0     3155 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/__init__.py
--rw-r--r--   0        0        0       45 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/axis/__init__.py
--rw-r--r--   0        0        0     1722 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/axis/base.py
--rw-r--r--   0        0        0      381 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/axis/x_axis.py
--rw-r--r--   0        0        0       35 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/__init__.py
--rw-r--r--   0        0        0     4983 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/base.py
--rw-r--r--   0        0        0      902 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/build_y_axis.py
--rw-r--r--   0        0        0     3279 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/y_axis.py
--rw-r--r--   0        0        0     4413 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/y_axis_mirror.py
--rw-r--r--   0        0        0     9066 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/chart.py
--rw-r--r--   0        0        0      513 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/consts.py
--rw-r--r--   0        0        0     1562 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/enums.py
--rw-r--r--   0        0        0    12101 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/exceptions.py
--rw-r--r--   0        0        0     1126 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/legend.py
--rw-r--r--   0        0        0     3322 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/navigator.py
--rw-r--r--   0        0        0       56 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/period_selector/__init__.py
--rw-r--r--   0        0        0     2692 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/period_selector/custom_period.py
--rw-r--r--   0        0        0     1051 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/period_selector/period.py
--rw-r--r--   0        0        0     5436 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/period_selector/selector.py
--rw-r--r--   0        0        0     1339 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/period_selector/standard.py
--rw-r--r--   0        0        0       46 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/__init__.py
--rw-r--r--   0        0        0     3472 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/area.py
--rw-r--r--   0        0        0     4698 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/area_range.py
--rw-r--r--   0        0        0     7615 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/base.py
--rw-r--r--   0        0        0     6061 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/bubble.py
--rw-r--r--   0        0        0     3621 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/column.py
--rw-r--r--   0        0        0     4728 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/error_bar.py
--rw-r--r--   0        0        0     3637 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/line.py
--rw-r--r--   0        0        0     3623 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/point.py
--rw-r--r--   0        0        0     3654 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/scatter.py
--rw-r--r--   0        0        0      618 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/typing.py
--rw-r--r--   0        0        0    23062 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/timeseries.py
--rw-r--r--   0        0        0     2038 2024-04-24 14:07:11.103692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/transform.py
--rw-r--r--   0        0        0       87 2024-04-24 14:07:11.103692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/toggle/__init__.py
--rw-r--r--   0        0        0      543 2024-04-24 14:07:11.103692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/toggle/exceptions.py
--rw-r--r--   0        0        0     5107 2024-04-24 14:07:11.103692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/toggle/toggle.py
--rw-r--r--   0        0        0     2755 2024-04-24 14:07:11.103692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/utils.py
--rw-r--r--   0        0        0       33 2024-04-24 14:07:11.103692 engineai_sdk-0.87.2/engineai/sdk/internal/__init__.py
--rw-r--r--   0        0        0     1336 2024-04-24 14:07:11.103692 engineai_sdk-0.87.2/engineai/sdk/internal/authentication/auth0.py
--rw-r--r--   0        0        0     5852 2024-04-24 14:07:11.103692 engineai_sdk-0.87.2/engineai/sdk/internal/authentication/utils.py
--rw-r--r--   0        0        0       92 2024-04-24 14:07:11.103692 engineai_sdk-0.87.2/engineai/sdk/internal/clients/__init__.py
--rw-r--r--   0        0        0     5038 2024-04-24 14:07:11.103692 engineai_sdk-0.87.2/engineai/sdk/internal/clients/api.py
--rw-r--r--   0        0        0     1195 2024-04-24 14:07:11.103692 engineai_sdk-0.87.2/engineai/sdk/internal/clients/exceptions.py
--rw-r--r--   0        0        0      482 2024-04-24 14:07:11.103692 engineai_sdk-0.87.2/engineai/sdk/internal/exceptions.py
--rw-r--r--   0        0        0      432 2024-04-24 14:07:11.103692 engineai_sdk-0.87.2/engineai/sdk/internal/graphql_dataclasses/__init__.py
--rw-r--r--   0        0        0      348 2024-04-24 14:07:11.103692 engineai_sdk-0.87.2/engineai/sdk/internal/graphql_dataclasses/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-24 14:07:11.103692 engineai_sdk-0.87.2/engineai/sdk/internal/graphql_dataclasses/py.typed
--rw-r--r--   0        0        0     3169 2024-04-24 14:07:11.103692 engineai_sdk-0.87.2/engineai/sdk/internal/graphql_dataclasses/schema.py
--rw-r--r--   0        0        0     6996 2024-04-24 14:07:11.103692 engineai_sdk-0.87.2/engineai/sdk/internal/graphql_dataclasses/types.py
--rw-r--r--   0        0        0      319 2024-04-24 14:07:11.103692 engineai_sdk-0.87.2/engineai/sdk/internal/url_config.py
--rw-r--r--   0        0        0     1841 2024-04-24 14:07:29.015686 engineai_sdk-0.87.2/pyproject.toml
--rw-r--r--   0        0        0     2422 1970-01-01 00:00:00.000000 engineai_sdk-0.87.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-15 08:39:55.683648 engineai_sdk-0.92.0/LICENSE
+-rw-r--r--   0        0        0      987 2024-05-15 08:39:55.683648 engineai_sdk-0.92.0/README.md
+-rw-r--r--   0        0        0      435 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/cli/__init__.py
+-rw-r--r--   0        0        0       33 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2521 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/cli/commands/app.py
+-rw-r--r--   0        0        0    14231 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/cli/commands/dashboard.py
+-rw-r--r--   0        0        0     1379 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/cli/console.py
+-rw-r--r--   0        0        0     4806 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/cli/generator.py
+-rw-r--r--   0        0        0       43 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/cli/template/content/.env.sample
+-rw-r--r--   0        0        0     5396 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/cli/template/content/data/example.json
+-rw-r--r--   0        0        0      411 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/cli/template/content/main.py
+-rw-r--r--   0        0        0    10363 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/cli/utils.py
+-rw-r--r--   0        0        0       38 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/__init__.py
+-rw-r--r--   0        0        0      121 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/abstract/__init__.py
+-rw-r--r--   0        0        0     2181 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/abstract/layout.py
+-rw-r--r--   0        0        0      207 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/abstract/selectable_widgets.py
+-rw-r--r--   0        0        0      570 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/abstract/typing.py
+-rw-r--r--   0        0        0     1635 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/base.py
+-rw-r--r--   0        0        0       96 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/clients/__init__.py
+-rw-r--r--   0        0        0     3429 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/clients/activate_dashboard.py
+-rw-r--r--   0        0        0     7407 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/clients/api.py
+-rw-r--r--   0        0        0     1451 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/clients/exceptions.py
+-rw-r--r--   0        0        0      217 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/clients/storage/__init__.py
+-rw-r--r--   0        0        0      472 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/clients/storage/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/clients/storage/py.typed
+-rw-r--r--   0        0        0      207 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/clients/storage/serialization/__init__.py
+-rw-r--r--   0        0        0     6861 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/clients/storage/serialization/dataframe.py
+-rw-r--r--   0        0        0     3134 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/clients/storage/serialization/json.py
+-rw-r--r--   0        0        0     4665 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/clients/storage/storage.py
+-rw-r--r--   0        0        0      515 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/config.py
+-rw-r--r--   0        0        0      310 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/dashboard/__init__.py
+-rw-r--r--   0        0        0    14052 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/dashboard/dashboard.py
+-rw-r--r--   0        0        0      140 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/dashboard/enums.py
+-rw-r--r--   0        0        0     4691 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/dashboard/exceptions.py
+-rw-r--r--   0        0        0       27 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/dashboard/graph/__init__.py
+-rw-r--r--   0        0        0     2417 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/dashboard/graph/executor_config.py
+-rw-r--r--   0        0        0     8389 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/dashboard/graph/instance.py
+-rw-r--r--   0        0        0     1231 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/dashboard/graph/node.py
+-rw-r--r--   0        0        0     2586 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/dashboard/graph/utils.py
+-rw-r--r--   0        0        0       41 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/dashboard/page/__init__.py
+-rw-r--r--   0        0        0     1363 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/dashboard/page/dependency.py
+-rw-r--r--   0        0        0     5541 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/dashboard/page/page.py
+-rw-r--r--   0        0        0     1831 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/dashboard/page/root.py
+-rw-r--r--   0        0        0     2967 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/dashboard/page/route.py
+-rw-r--r--   0        0        0      345 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/dashboard/typings.py
+-rw-r--r--   0        0        0       33 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/dashboard/version/__init__.py
+-rw-r--r--   0        0        0     5068 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/dashboard/version/version.py
+-rw-r--r--   0        0        0      185 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/data/__init__.py
+-rw-r--r--   0        0        0    12893 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/data/decorator.py
+-rw-r--r--   0        0        0     1822 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/data/duplicated.py
+-rw-r--r--   0        0        0     1047 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/data/enums.py
+-rw-r--r--   0        0        0     4676 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/data/exceptions.py
+-rw-r--r--   0        0        0     2007 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/data/http.py
+-rw-r--r--   0        0        0     3616 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/data/io_handler.py
+-rw-r--r--   0        0        0     1306 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/data/manager/interface.py
+-rw-r--r--   0        0        0     9908 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/data/manager/manager.py
+-rw-r--r--   0        0        0     2892 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/decorator.py
+-rw-r--r--   0        0        0      441 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/dependencies/__init__.py
+-rw-r--r--   0        0        0     2993 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/dependencies/datastore.py
+-rw-r--r--   0        0        0      141 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/dependencies/http/__init__.py
+-rw-r--r--   0        0        0      841 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/dependencies/http/header.py
+-rw-r--r--   0        0        0     2500 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/dependencies/http/http.py
+-rw-r--r--   0        0        0     1942 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/dependencies/route.py
+-rw-r--r--   0        0        0     2455 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/dependencies/widget.py
+-rw-r--r--   0        0        0      369 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/enum/__init__.py
+-rw-r--r--   0        0        0     1112 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/enum/align.py
+-rw-r--r--   0        0        0      741 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/enum/legend_position.py
+-rw-r--r--   0        0        0     5156 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/exceptions.py
+-rw-r--r--   0        0        0      569 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/formatting/__init__.py
+-rw-r--r--   0        0        0     3729 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/formatting/axis.py
+-rw-r--r--   0        0        0     1820 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/formatting/datetime.py
+-rw-r--r--   0        0        0      661 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/formatting/exceptions.py
+-rw-r--r--   0        0        0     1278 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/formatting/mapper.py
+-rw-r--r--   0        0        0     5176 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/formatting/number.py
+-rw-r--r--   0        0        0     1357 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/formatting/text.py
+-rw-r--r--   0        0        0      331 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/formatting/typing.py
+-rw-r--r--   0        0        0      985 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/formatting/validator.py
+-rw-r--r--   0        0        0     1056 2024-05-15 08:39:55.687648 engineai_sdk-0.92.0/engineai/sdk/dashboard/interface.py
+-rw-r--r--   0        0        0      825 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/__init__.py
+-rw-r--r--   0        0        0      326 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/build_item.py
+-rw-r--r--   0        0        0       28 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/card/__init__.py
+-rw-r--r--   0        0        0     5881 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/card/card.py
+-rw-r--r--   0        0        0     2889 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/card/chip.py
+-rw-r--r--   0        0        0     1679 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/card/header.py
+-rw-r--r--   0        0        0       55 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/collapsible/__init__.py
+-rw-r--r--   0        0        0     3082 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/collapsible/chip.py
+-rw-r--r--   0        0        0     1968 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/collapsible/header.py
+-rw-r--r--   0        0        0     6520 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/collapsible/section.py
+-rw-r--r--   0        0        0     5951 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/column.py
+-rw-r--r--   0        0        0     2599 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/components/chip.py
+-rw-r--r--   0        0        0     2103 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/components/header.py
+-rw-r--r--   0        0        0     2150 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/components/label.py
+-rw-r--r--   0        0        0     4695 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/exceptions.py
+-rw-r--r--   0        0        0       31 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/fluid_row/__init__.py
+-rw-r--r--   0        0        0     5813 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/fluid_row/fluid_row.py
+-rw-r--r--   0        0        0     7221 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/grid.py
+-rw-r--r--   0        0        0    10378 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/row.py
+-rw-r--r--   0        0        0       36 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/selectable/__init__.py
+-rw-r--r--   0        0        0     7216 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/selectable/base.py
+-rw-r--r--   0        0        0     2171 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/selectable/exceptions.py
+-rw-r--r--   0        0        0     4251 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/selectable/tab.py
+-rw-r--r--   0        0        0      676 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/typings.py
+-rw-r--r--   0        0        0      244 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/links/__init__.py
+-rw-r--r--   0        0        0     6016 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/links/abstract.py
+-rw-r--r--   0        0        0     2201 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/links/route_link.py
+-rw-r--r--   0        0        0     2576 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/links/template_string_link.py
+-rw-r--r--   0        0        0      202 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/links/typing.py
+-rw-r--r--   0        0        0     1427 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/links/url.py
+-rw-r--r--   0        0        0      866 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/links/widget_dependency.py
+-rw-r--r--   0        0        0     3039 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/links/widget_field.py
+-rw-r--r--   0        0        0        0 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/py.typed
+-rw-r--r--   0        0        0     2020 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/selected.py
+-rw-r--r--   0        0        0      100 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/styling/__init__.py
+-rw-r--r--   0        0        0      744 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/styling/color/__init__.py
+-rw-r--r--   0        0        0     5872 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/styling/color/default_specs.py
+-rw-r--r--   0        0        0     6802 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/styling/color/discrete_map.py
+-rw-r--r--   0        0        0     1614 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/styling/color/divergent.py
+-rw-r--r--   0        0        0     3952 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/styling/color/gradient.py
+-rw-r--r--   0        0        0     5949 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/styling/color/palette.py
+-rw-r--r--   0        0        0      856 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/styling/color/single.py
+-rw-r--r--   0        0        0      889 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/styling/color/spec.py
+-rw-r--r--   0        0        0      436 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/styling/color/typing.py
+-rw-r--r--   0        0        0     3436 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/styling/icons.py
+-rw-r--r--   0        0        0     8087 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/templated_string.py
+-rw-r--r--   0        0        0     2360 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/utils.py
+-rw-r--r--   0        0        0       25 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/__init__.py
+-rw-r--r--   0        0        0     8642 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/base.py
+-rw-r--r--   0        0        0     2647 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/cartesian/__init__.py
+-rw-r--r--   0        0        0       44 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/cartesian/axis/__init__.py
+-rw-r--r--   0        0        0     3124 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/cartesian/axis/base.py
+-rw-r--r--   0        0        0      365 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/cartesian/axis/typing.py
+-rw-r--r--   0        0        0     2094 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/cartesian/axis/x_axis.py
+-rw-r--r--   0        0        0     5182 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/cartesian/axis/y_axis.py
+-rw-r--r--   0        0        0     4368 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/cartesian/cartesian.py
+-rw-r--r--   0        0        0     4404 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/cartesian/chart.py
+-rw-r--r--   0        0        0     1468 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/cartesian/exceptions.py
+-rw-r--r--   0        0        0      893 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/cartesian/legend.py
+-rw-r--r--   0        0        0       45 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/cartesian/series/__init__.py
+-rw-r--r--   0        0        0     2581 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/cartesian/series/area.py
+-rw-r--r--   0        0        0     3962 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/cartesian/series/area_range.py
+-rw-r--r--   0        0        0     7257 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/cartesian/series/base.py
+-rw-r--r--   0        0        0     5277 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/cartesian/series/bubble.py
+-rw-r--r--   0        0        0     2599 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/cartesian/series/column.py
+-rw-r--r--   0        0        0     2581 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/cartesian/series/line.py
+-rw-r--r--   0        0        0     2617 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/cartesian/series/scatter.py
+-rw-r--r--   0        0        0      573 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/cartesian/series/typing.py
+-rw-r--r--   0        0        0     4957 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/chart_utils.py
+-rw-r--r--   0        0        0       39 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/__init__.py
+-rw-r--r--   0        0        0       87 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/actions/links/__init__.py
+-rw-r--r--   0        0        0     2641 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/actions/links/base.py
+-rw-r--r--   0        0        0     1475 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/actions/links/exceptions.py
+-rw-r--r--   0        0        0     1859 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/actions/links/url_link.py
+-rw-r--r--   0        0        0       47 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/__init__.py
+-rw-r--r--   0        0        0       56 2024-05-15 08:39:55.691648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/axis/__init__.py
+-rw-r--r--   0        0        0      416 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/axis/scale/__init__.py
+-rw-r--r--   0        0        0      988 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/axis/scale/dynamic.py
+-rw-r--r--   0        0        0     1640 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/axis/scale/negative.py
+-rw-r--r--   0        0        0     1640 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/axis/scale/positive.py
+-rw-r--r--   0        0        0     1037 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/axis/scale/scale.py
+-rw-r--r--   0        0        0     2619 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/axis/scale/symmetric.py
+-rw-r--r--   0        0        0      338 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/axis/scale/typing.py
+-rw-r--r--   0        0        0      151 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/consts.py
+-rw-r--r--   0        0        0     7162 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/exceptions.py
+-rw-r--r--   0        0        0       25 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/series/__init__.py
+-rw-r--r--   0        0        0     2352 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/series/base.py
+-rw-r--r--   0        0        0       23 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/series/entities/__init__.py
+-rw-r--r--   0        0        0      888 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/series/entities/base.py
+-rw-r--r--   0        0        0     2029 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/series/entities/country.py
+-rw-r--r--   0        0        0      693 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/series/entities/custom.py
+-rw-r--r--   0        0        0      314 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/series/entities/typing.py
+-rw-r--r--   0        0        0      696 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/styling/__init__.py
+-rw-r--r--   0        0        0     1444 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/styling/area.py
+-rw-r--r--   0        0        0     1521 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/styling/area_range.py
+-rw-r--r--   0        0        0     3494 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/styling/base.py
+-rw-r--r--   0        0        0     3383 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/styling/bubble_circle.py
+-rw-r--r--   0        0        0     2993 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/styling/bubble_country.py
+-rw-r--r--   0        0        0     1435 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/styling/column.py
+-rw-r--r--   0        0        0     1047 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/styling/enums.py
+-rw-r--r--   0        0        0     1489 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/styling/error_bar.py
+-rw-r--r--   0        0        0     3588 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/styling/line.py
+-rw-r--r--   0        0        0     1425 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/styling/point.py
+-rw-r--r--   0        0        0     1464 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/styling/scatter.py
+-rw-r--r--   0        0        0      802 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/styling/typing.py
+-rw-r--r--   0        0        0      212 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/toolbar.py
+-rw-r--r--   0        0        0      486 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/tooltip/__init__.py
+-rw-r--r--   0        0        0     3448 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/tooltip/base.py
+-rw-r--r--   0        0        0     1443 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/tooltip/category.py
+-rw-r--r--   0        0        0     3066 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/tooltip/country.py
+-rw-r--r--   0        0        0     1597 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/tooltip/datetime.py
+-rw-r--r--   0        0        0      617 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/tooltip/exceptions.py
+-rw-r--r--   0        0        0     1158 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/tooltip/item.py
+-rw-r--r--   0        0        0     1484 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/tooltip/number.py
+-rw-r--r--   0        0        0      939 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/tooltip/styling/country/base.py
+-rw-r--r--   0        0        0      922 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/tooltip/styling/country/flag.py
+-rw-r--r--   0        0        0      151 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/tooltip/styling/country/typings.py
+-rw-r--r--   0        0        0     1554 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/tooltip/text.py
+-rw-r--r--   0        0        0      759 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/typing.py
+-rw-r--r--   0        0        0       29 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/__init__.py
+-rw-r--r--   0        0        0     1192 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/styling/__init__.py
+-rw-r--r--   0        0        0     4103 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/styling/base.py
+-rw-r--r--   0        0        0       35 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/styling/chart/__init__.py
+-rw-r--r--   0        0        0      182 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/styling/chart/area.py
+-rw-r--r--   0        0        0      188 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/styling/chart/column.py
+-rw-r--r--   0        0        0      182 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/styling/chart/line.py
+-rw-r--r--   0        0        0      196 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/styling/chart/stacked_bar.py
+-rw-r--r--   0        0        0      379 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/styling/chart/typing.py
+-rw-r--r--   0        0        0      974 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/styling/exceptions.py
+-rw-r--r--   0        0        0       36 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/styling/number/__init__.py
+-rw-r--r--   0        0        0     1346 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/styling/number/arrow.py
+-rw-r--r--   0        0        0      855 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/styling/number/chip.py
+-rw-r--r--   0        0        0      852 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/styling/number/dot.py
+-rw-r--r--   0        0        0      864 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/styling/number/font.py
+-rw-r--r--   0        0        0     1154 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/styling/number/progress_bar.py
+-rw-r--r--   0        0        0      339 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/styling/number/typing.py
+-rw-r--r--   0        0        0       34 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/styling/text/__init__.py
+-rw-r--r--   0        0        0      839 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/styling/text/chip.py
+-rw-r--r--   0        0        0     1284 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/styling/text/country_flag.py
+-rw-r--r--   0        0        0      904 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/styling/text/dot.py
+-rw-r--r--   0        0        0      863 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/styling/text/font.py
+-rw-r--r--   0        0        0      331 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/styling/text/typing.py
+-rw-r--r--   0        0        0     1259 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/tooltip/format_build.py
+-rw-r--r--   0        0        0     1917 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/tooltip/header.py
+-rw-r--r--   0        0        0     2564 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/tooltip/stacked_bar.py
+-rw-r--r--   0        0        0     1906 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/tooltip/tooltip.py
+-rw-r--r--   0        0        0      136 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/content/__init__.py
+-rw-r--r--   0        0        0     2830 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/content/content.py
+-rw-r--r--   0        0        0     1265 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/content/exceptions.py
+-rw-r--r--   0        0        0      554 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/content/item.py
+-rw-r--r--   0        0        0     1341 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/content/markdown.py
+-rw-r--r--   0        0        0     3756 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/exceptions.py
+-rw-r--r--   0        0        0      573 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/maps/__init__.py
+-rw-r--r--   0        0        0     1301 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/maps/color_axis.py
+-rw-r--r--   0        0        0     1043 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/maps/enums.py
+-rw-r--r--   0        0        0      980 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/maps/exceptions.py
+-rw-r--r--   0        0        0       25 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/maps/geo/__init__.py
+-rw-r--r--   0        0        0     7968 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/maps/geo/base.py
+-rw-r--r--   0        0        0     4249 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/maps/geo/geo.py
+-rw-r--r--   0        0        0       29 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/maps/geo/styling/__init__.py
+-rw-r--r--   0        0        0      772 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/maps/geo/styling/label.py
+-rw-r--r--   0        0        0      916 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/maps/geo/styling/styling.py
+-rw-r--r--   0        0        0      898 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/maps/legend.py
+-rw-r--r--   0        0        0       42 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/maps/series/__init__.py
+-rw-r--r--   0        0        0     4833 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/maps/series/numeric.py
+-rw-r--r--   0        0        0      568 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/maps/series/series.py
+-rw-r--r--   0        0        0     2865 2024-05-15 08:39:55.695648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/maps/series/styling.py
+-rw-r--r--   0        0        0     2113 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/pandas_utils.py
+-rw-r--r--   0        0        0      672 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/pie/__init__.py
+-rw-r--r--   0        0        0     1885 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/pie/chart.py
+-rw-r--r--   0        0        0      852 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/pie/exceptions.py
+-rw-r--r--   0        0        0      786 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/pie/legend.py
+-rw-r--r--   0        0        0     6115 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/pie/pie.py
+-rw-r--r--   0        0        0       35 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/pie/series/__init__.py
+-rw-r--r--   0        0        0     5639 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/pie/series/base.py
+-rw-r--r--   0        0        0     3397 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/pie/series/country.py
+-rw-r--r--   0        0        0     3007 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/pie/series/series.py
+-rw-r--r--   0        0        0     3139 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/pie/series/styling.py
+-rw-r--r--   0        0        0      165 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/pie/series/typings.py
+-rw-r--r--   0        0        0     2339 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/pie/tooltip.py
+-rw-r--r--   0        0        0      391 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/search/__init__.py
+-rw-r--r--   0        0        0     3415 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/search/exceptions.py
+-rw-r--r--   0        0        0       28 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/search/results/__init__.py
+-rw-r--r--   0        0        0     2334 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/search/results/base.py
+-rw-r--r--   0        0        0      813 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/search/results/build_result.py
+-rw-r--r--   0        0        0     3415 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/search/results/number.py
+-rw-r--r--   0        0        0       21 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/search/results/styling/__init__.py
+-rw-r--r--   0        0        0     2713 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/search/results/styling/base_styling.py
+-rw-r--r--   0        0        0     1456 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/search/results/styling/number.py
+-rw-r--r--   0        0        0     1647 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/search/results/styling/text.py
+-rw-r--r--   0        0        0     2379 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/search/results/text.py
+-rw-r--r--   0        0        0      280 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/search/results/typing.py
+-rw-r--r--   0        0        0     7931 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/search/search.py
+-rw-r--r--   0        0        0       79 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/select/__init__.py
+-rw-r--r--   0        0        0     2135 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/select/exceptions.py
+-rw-r--r--   0        0        0     1713 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/select/group.py
+-rw-r--r--   0        0        0     6261 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/select/select.py
+-rw-r--r--   0        0        0     3418 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/__init__.py
+-rw-r--r--   0        0        0       50 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/__init__.py
+-rw-r--r--   0        0        0       26 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/items/__init__.py
+-rw-r--r--   0        0        0     6115 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/items/base.py
+-rw-r--r--   0        0        0     5975 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/items/category.py
+-rw-r--r--   0        0        0       46 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/items/charts/__init__.py
+-rw-r--r--   0        0        0     5510 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/items/charts/area.py
+-rw-r--r--   0        0        0     6736 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/items/charts/base.py
+-rw-r--r--   0        0        0     5569 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/items/charts/column.py
+-rw-r--r--   0        0        0     5568 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/items/charts/line.py
+-rw-r--r--   0        0        0     7471 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/items/charts/stack_bar.py
+-rw-r--r--   0        0        0     4879 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/items/country.py
+-rw-r--r--   0        0        0     5643 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/items/datetime.py
+-rw-r--r--   0        0        0     4011 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/items/exceptions.py
+-rw-r--r--   0        0        0     5856 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/items/number.py
+-rw-r--r--   0        0        0     5489 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/items/range.py
+-rw-r--r--   0        0        0     5201 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/items/text.py
+-rw-r--r--   0        0        0     3530 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/items/url_column.py
+-rw-r--r--   0        0        0       49 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/styling/__init__.py
+-rw-r--r--   0        0        0     1100 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/styling/area.py
+-rw-r--r--   0        0        0     1611 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/styling/arrow.py
+-rw-r--r--   0        0        0     4397 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/styling/base.py
+-rw-r--r--   0        0        0     1494 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/styling/cell.py
+-rw-r--r--   0        0        0     2459 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/styling/color_bar.py
+-rw-r--r--   0        0        0     1113 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/styling/column.py
+-rw-r--r--   0        0        0     1267 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/styling/country_flag.py
+-rw-r--r--   0        0        0     1225 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/styling/dot.py
+-rw-r--r--   0        0        0     1537 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/styling/exceptions.py
+-rw-r--r--   0        0        0     1371 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/styling/font.py
+-rw-r--r--   0        0        0     1186 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/styling/icon.py
+-rw-r--r--   0        0        0     1101 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/styling/line.py
+-rw-r--r--   0        0        0     1446 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/styling/range.py
+-rw-r--r--   0        0        0     2672 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/styling/split_bar.py
+-rw-r--r--   0        0        0     1502 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/styling/stacked_bar.py
+-rw-r--r--   0        0        0     1785 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/styling/utils.py
+-rw-r--r--   0        0        0      473 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/enums.py
+-rw-r--r--   0        0        0     5447 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/exceptions.py
+-rw-r--r--   0        0        0     1794 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/group.py
+-rw-r--r--   0        0        0     9030 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/header.py
+-rw-r--r--   0        0        0     2656 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/initial_state.py
+-rw-r--r--   0        0        0     1987 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/styling.py
+-rw-r--r--   0        0        0    17144 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/table.py
+-rw-r--r--   0        0        0     3155 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/__init__.py
+-rw-r--r--   0        0        0       45 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/axis/__init__.py
+-rw-r--r--   0        0        0     1242 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/axis/base.py
+-rw-r--r--   0        0        0      330 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/axis/x_axis.py
+-rw-r--r--   0        0        0       35 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/__init__.py
+-rw-r--r--   0        0        0     4983 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/base.py
+-rw-r--r--   0        0        0      812 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/build_y_axis.py
+-rw-r--r--   0        0        0     4017 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/y_axis.py
+-rw-r--r--   0        0        0     5996 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/y_axis_mirror.py
+-rw-r--r--   0        0        0     8974 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/chart.py
+-rw-r--r--   0        0        0      513 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/consts.py
+-rw-r--r--   0        0        0     1562 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/enums.py
+-rw-r--r--   0        0        0    12101 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/exceptions.py
+-rw-r--r--   0        0        0     1041 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/legend.py
+-rw-r--r--   0        0        0     3247 2024-05-15 08:39:55.699648 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/navigator.py
+-rw-r--r--   0        0        0       56 2024-05-15 08:39:55.703647 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/period_selector/__init__.py
+-rw-r--r--   0        0        0     2617 2024-05-15 08:39:55.703647 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/period_selector/custom_period.py
+-rw-r--r--   0        0        0      814 2024-05-15 08:39:55.703647 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/period_selector/period.py
+-rw-r--r--   0        0        0     5359 2024-05-15 08:39:55.703647 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/period_selector/selector.py
+-rw-r--r--   0        0        0     1339 2024-05-15 08:39:55.703647 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/period_selector/standard.py
+-rw-r--r--   0        0        0       46 2024-05-15 08:39:55.703647 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/series/__init__.py
+-rw-r--r--   0        0        0     3422 2024-05-15 08:39:55.703647 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/series/area.py
+-rw-r--r--   0        0        0     4643 2024-05-15 08:39:55.703647 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/series/area_range.py
+-rw-r--r--   0        0        0     7608 2024-05-15 08:39:55.703647 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/series/base.py
+-rw-r--r--   0        0        0     6009 2024-05-15 08:39:55.703647 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/series/bubble.py
+-rw-r--r--   0        0        0     3569 2024-05-15 08:39:55.703647 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/series/column.py
+-rw-r--r--   0        0        0     4674 2024-05-15 08:39:55.703647 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/series/error_bar.py
+-rw-r--r--   0        0        0     3587 2024-05-15 08:39:55.703647 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/series/line.py
+-rw-r--r--   0        0        0     3572 2024-05-15 08:39:55.703647 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/series/point.py
+-rw-r--r--   0        0        0     3601 2024-05-15 08:39:55.703647 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/series/scatter.py
+-rw-r--r--   0        0        0      618 2024-05-15 08:39:55.703647 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/series/typing.py
+-rw-r--r--   0        0        0    21384 2024-05-15 08:39:55.703647 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/timeseries.py
+-rw-r--r--   0        0        0     1968 2024-05-15 08:39:55.703647 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/transform.py
+-rw-r--r--   0        0        0       87 2024-05-15 08:39:55.703647 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/toggle/__init__.py
+-rw-r--r--   0        0        0      543 2024-05-15 08:39:55.703647 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/toggle/exceptions.py
+-rw-r--r--   0        0        0     4793 2024-05-15 08:39:55.703647 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/toggle/toggle.py
+-rw-r--r--   0        0        0     2606 2024-05-15 08:39:55.703647 engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/utils.py
+-rw-r--r--   0        0        0       33 2024-05-15 08:39:55.703647 engineai_sdk-0.92.0/engineai/sdk/internal/__init__.py
+-rw-r--r--   0        0        0     1336 2024-05-15 08:39:55.703647 engineai_sdk-0.92.0/engineai/sdk/internal/authentication/auth0.py
+-rw-r--r--   0        0        0     5852 2024-05-15 08:39:55.703647 engineai_sdk-0.92.0/engineai/sdk/internal/authentication/utils.py
+-rw-r--r--   0        0        0       92 2024-05-15 08:39:55.703647 engineai_sdk-0.92.0/engineai/sdk/internal/clients/__init__.py
+-rw-r--r--   0        0        0     4836 2024-05-15 08:39:55.703647 engineai_sdk-0.92.0/engineai/sdk/internal/clients/api.py
+-rw-r--r--   0        0        0     1195 2024-05-15 08:39:55.703647 engineai_sdk-0.92.0/engineai/sdk/internal/clients/exceptions.py
+-rw-r--r--   0        0        0      792 2024-05-15 08:39:55.703647 engineai_sdk-0.92.0/engineai/sdk/internal/exceptions.py
+-rw-r--r--   0        0        0      319 2024-05-15 08:39:55.703647 engineai_sdk-0.92.0/engineai/sdk/internal/url_config.py
+-rw-r--r--   0        0        0     1841 2024-05-15 08:40:07.859539 engineai_sdk-0.92.0/pyproject.toml
+-rw-r--r--   0        0        0     2422 1970-01-01 00:00:00.000000 engineai_sdk-0.92.0/PKG-INFO
```

### Comparing `engineai_sdk-0.87.2/LICENSE` & `engineai_sdk-0.92.0/LICENSE`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/README.md` & `engineai_sdk-0.92.0/README.md`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/cli/commands/app.py` & `engineai_sdk-0.92.0/engineai/sdk/cli/commands/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from rich.console import Console
 from rich.table import Table
 
 from engineai.sdk.cli.utils import set_env_var
 from engineai.sdk.cli.utils import write_console
 from engineai.sdk.dashboard.clients.api import DashboardAPI
 from engineai.sdk.dashboard.clients.exceptions import APIServerError
-from engineai.sdk.internal.graphql_dataclasses.exceptions import UnauthenticatedError
+from engineai.sdk.internal.exceptions import UnauthenticatedError
 
 
 def _get_apps() -> List:
     api = DashboardAPI()
     try:
         apps = api.list_my_apps()
     except (APIServerError, UnauthenticatedError) as e:
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/cli/commands/dashboard.py` & `engineai_sdk-0.92.0/engineai/sdk/cli/commands/dashboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from engineai.sdk.dashboard.dashboard.dashboard import PLATFORM_URL
 from engineai.sdk.dashboard.data.exceptions import DataValidationError
 from engineai.sdk.internal.authentication.utils import MalformedURLError
 from engineai.sdk.internal.authentication.utils import URLNotSupportedError
 from engineai.sdk.internal.authentication.utils import add_url_into_env_file
 from engineai.sdk.internal.authentication.utils import get_url
 from engineai.sdk.internal.clients.exceptions import APIServerError
-from engineai.sdk.internal.graphql_dataclasses.exceptions import UnauthenticatedError
+from engineai.sdk.internal.exceptions import UnauthenticatedError
 
 DASHBOARD_CREATED_MSG = (
     "\nDashboard created! To publish your dashboard, navigate to "
     "`{}` folder and run `engineai dashboard publish` to publish.\n"
 )
 
 API_USER_ERRORS = ("NOT_FOUND", "FORBIDDEN")
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/cli/console.py` & `engineai_sdk-0.92.0/engineai/sdk/cli/console.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/cli/generator.py` & `engineai_sdk-0.92.0/engineai/sdk/cli/generator.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/cli/template/content/data/example.json` & `engineai_sdk-0.92.0/engineai/sdk/cli/template/content/data/example.json`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/cli/utils.py` & `engineai_sdk-0.92.0/engineai/sdk/cli/utils.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/abstract/layout.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/abstract/layout.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/abstract/typing.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/abstract/typing.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/base.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """Top-level package for Dashboard factories."""
 import logging
 from abc import ABC
 from abc import abstractmethod
 from typing import Any
+from typing import Dict
 from typing import Optional
 
 logger = logging.getLogger(__name__)
 
 HEIGHT_ROUND_VALUE = 2
 
 
 class AbstractFactory(ABC):
     """Abstract Class implemented by all factories."""
 
     @abstractmethod
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/clients/activate_dashboard.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/clients/activate_dashboard.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Spec for a activate dashboard."""
 
 from typing import Any
+from typing import Dict
 from typing import Optional
 
-from engineai.sdk.dashboard.utils import generate_input
-
 
 class ActivateDashboardVersion:
     """Spec for ActivateDashboardVersion class."""
 
     def __init__(self, version: str, activate: bool) -> None:
         """Construct for ActivateDashboardVersion class.
 
@@ -25,21 +24,20 @@
         return self.__version
 
     @property
     def activate(self) -> bool:
         """Activate."""
         return self.__activate
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Builds spec for dashboard API."""
-        return generate_input(
-            "ActivateDashboardVersionInput",
-            version=self.__version,
-            activate=self.__activate,
-        )
+        return {
+            "version": self.__version,
+            "activate": self.__activate,
+        }
 
 
 class ActivateDashboardRun:
     """Spec for ActivateDashboardRun class."""
 
     def __init__(self, run: str, activate: bool) -> None:
         """Construct for ActivateDashboardRun class.
@@ -57,21 +55,20 @@
         return self.__run
 
     @property
     def activate(self) -> bool:
         """Activate."""
         return self.__activate
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Builds spec for dashboard API."""
-        return generate_input(
-            "ActivateDashboardRunInput",
-            run=self.__run,
-            activate=self.__activate,
-        )
+        return {
+            "run": self.__run,
+            "activate": self.__activate,
+        }
 
 
 class ActivateDashboard:
     """Spec for ActivateDashboard class."""
 
     def __init__(
         self,
@@ -121,15 +118,14 @@
         return self.__run.run
 
     @property
     def activate_run(self) -> bool:
         """Activate run."""
         return self.__run.activate
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Builds spec for dashboard API."""
-        return generate_input(
-            "ActivateDashboardInput",
-            id=self.__dashboard_id,
-            version=self.__version.build(),
-            run=self.__run.build(),
-        )
+        return {
+            "id": self.__dashboard_id,
+            "version": self.__version.build(),
+            "run": self.__run.build(),
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/clients/api.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/clients/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Helper class to connect to Dashboard API and obtain base types."""
 
 import logging
-from dataclasses import dataclass
 from typing import Any
 from typing import Dict
 from typing import Generator
 from typing import List
 from typing import Optional
 
 from engineai.sdk.dashboard.clients.activate_dashboard import ActivateDashboard
@@ -13,32 +12,18 @@
 
 from .exceptions import DashboardAPINoVersionFoundError
 
 logger = logging.getLogger(__name__)
 logging.getLogger("urllib3").propagate = False
 
 
-@dataclass
-class DashboardResponse:
-    """API response."""
-
-    url_path: str
-    dashboard_id: str
-    version: Optional[str]
-    run: Optional[str]
-    app_id: Optional[str]
-    dashboard_slug: str
-
-
 class DashboardAPI(APIClient):
     """Dashboard API Connector and Types."""
 
-    def publish_dashboard(
-        self, dashboard: Dict[Any, Any]
-    ) -> Optional[DashboardResponse]:
+    def publish_dashboard(self, dashboard: Dict[Any, Any]) -> Optional[Dict[Any, Any]]:
         """Publish a Dashboard."""
         content = self._request(
             query="""
                 mutation PublishDashboard ($input: DashboardInput!) {
                     publishDashboard(input: $input) {
                         run
                         id
@@ -55,22 +40,22 @@
         )
 
         data = content.get("data", {}).get("publishDashboard", {})
 
         if data is None:
             return None
 
-        return DashboardResponse(
-            url_path=data.get("url"),
-            dashboard_id=data.get("id"),
-            version=data.get("version", None),
-            run=data.get("run", None),
-            app_id=data.get("appId"),
-            dashboard_slug=dashboard.get("slug", "").replace(" ", "-"),
-        )
+        return {
+            "url_path": data.get("url"),
+            "dashboard_id": data.get("id"),
+            "version": data.get("version", None),
+            "run": data.get("run", None),
+            "app_id": data.get("appId"),
+            "dashboard_slug": dashboard.get("slug", "").replace(" ", "-"),
+        }
 
     def get_dashboard(
         self, dashboard_slug: str, app_id: Optional[str], version: Optional[str]
     ) -> None:
         """Get a dashboard."""
         return self._request(
             query="""query Dashboard($slug: String, $appId: String!, $version: String) {
@@ -162,15 +147,15 @@
             if dashboard_version.get("version") == version:
                 for run in dashboard_version.get("runs", []):
                     yield run
                 break
 
     def activate_dashboard(self, activate_dashboard: ActivateDashboard) -> None:
         """Activate a dashboard."""
-        activate_dashboard_spec = activate_dashboard.build().to_dict()
+        activate_dashboard_spec = activate_dashboard.build()
 
         return self._request(
             query="""
                 mutation ActivateDashboard($input: ActivateDashboardInput!) {
                     activateDashboard(input: $input)
                 }""",
             variables={"input": activate_dashboard_spec},
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/clients/exceptions.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/clients/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/clients/storage/serialization/dataframe.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/clients/storage/serialization/dataframe.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/clients/storage/serialization/json.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/clients/storage/serialization/json.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/clients/storage/storage.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/clients/storage/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,15 +159,16 @@
 
     def _create_session(self) -> requests.Session:
         """Create a session."""
         session = requests.Session()
         retry = Retry(
             total=10,
             backoff_factor=0.5,
-            status_forcelist=[500, 502, 503, 504],
+            status_forcelist=[500, 502, 503, 504, 400, 401],
+            allowed_methods=["PUT"],
         )
         adapter = HTTPAdapter(max_retries=retry)
         session.mount("http://", adapter)
         session.mount("https://", adapter)
         return session
 
     def close(self) -> None:
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/config.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/config.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/dashboard.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/dashboard/dashboard.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """Spec for a Dashboard."""
 import enum
 import logging
 import os
 import re
 import sys
 import webbrowser
+from dataclasses import dataclass
 from datetime import datetime
 from pathlib import Path
 from typing import Any
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 from typing import cast
 from urllib.parse import urlparse
 
 from environs import Env
 
 from engineai.sdk.dashboard.clients.activate_dashboard import ActivateDashboard
 from engineai.sdk.dashboard.clients.storage import StorageConfig
 from engineai.sdk.dashboard.dashboard.typings import DashboardContent
 from engineai.sdk.dashboard.data import StorageType
 from engineai.sdk.dashboard.decorator import type_check
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.internal.url_config import PLATFORM_URL
 
 from ..abstract.typing import PrepareParams
 from ..clients import DashboardAPI
-from ..clients.api import DashboardResponse
 from ..clients.exceptions import APIServerError
 from .enums import DashboardStatus
 from .exceptions import DashboardDuplicatedPathsError
 from .exceptions import DashboardEmptyContentError
 from .exceptions import DashboardInvalidSlugError
 from .exceptions import DashboardNoDashboardFoundError
 from .exceptions import DashboardSkipDataCannotCreateRunError
@@ -40,14 +40,26 @@
 
 logger = logging.getLogger(__name__)
 
 
 env = Env()
 
 
+@dataclass
+class DashboardResponse:
+    """API response."""
+
+    url_path: str
+    dashboard_id: str
+    version: Optional[str]
+    run: Optional[str]
+    app_id: Optional[str]
+    dashboard_slug: str
+
+
 class PublishMode(enum.Enum):
     """Dashboard Publish Mode.
 
     Attributes:
         DEFAULT: Default publish mode. The dashboard does not create new
             runs and automatically activates the published version.
         DEV: Development publish mode. The dashboard creates new
@@ -225,14 +237,17 @@
         platform_url = PLATFORM_URL.get(urlparse(self._api_client.url).netloc)
         url = (
             f"{platform_url}{dashboard_response.url_path}"
             if self._api_client.url is not None
             else None
         )
 
+        if url is None:
+            raise ValueError("URL not found")
+
         return (
             url
             if self.__publish_mode in [PublishMode.DEFAULT, PublishMode.DEV]
             else (
                 f"{url}?"
                 f"dashboard-version={dashboard_response.version}&"
                 f"dashboard-version-run={dashboard_response.run}"
@@ -250,15 +265,28 @@
                 "To activate please run this command:\n"
                 f"engineai dashboard -s {dashboard_response.dashboard_slug} "
                 f"activate -v {dashboard_response.version} "
                 f"-r {dashboard_response.run}\n\n"
             )
 
     def _publish_in_api(self) -> Optional[DashboardResponse]:
-        return self._api_client.publish_dashboard(dashboard=self._build().to_dict())
+        response = self._api_client.publish_dashboard(dashboard=self._build())
+
+        return (
+            DashboardResponse(
+                url_path=response.get("url_path", None),
+                dashboard_id=response.get("dashboard_id", None),
+                version=response.get("version", None),
+                run=response.get("run", None),
+                app_id=response.get("app_id", None),
+                dashboard_slug=response.get("dashboard_slug", None),
+            )
+            if response is not None
+            else None
+        )
 
     def __validate_pages(self) -> None:
         paths = set()
         for page in self.__pages:
             if page.path not in paths:
                 paths.add(page.path)
             else:
@@ -341,23 +369,22 @@
                 version=dashboard_response.version,
                 activate_version=self.__activate_version,
                 run=dashboard_response.run,
                 activate_run=self.__activate_run,
             )
         )
 
-    def _build(self) -> Any:
+    def _build(self) -> Dict[str, Any]:
         """Builds spec for dashboard API."""
-        return generate_input(
-            "DashboardInput",
-            name=self.__name,
-            slug=self.__slug.replace("_", "-"),
-            description=self.__description,
-            version=self.__version.build() if self.__version else None,
-            pages=[page.build() for page in self.__pages],
-            appId=self.__app_id,
-        )
+        return {
+            "name": self.__name,
+            "slug": self.__slug.replace("_", "-"),
+            "description": self.__description,
+            "version": self.__version.build() if self.__version else None,
+            "pages": [page.build() for page in self.__pages],
+            "appId": self.__app_id,
+        }
 
 
 def _reset_data_writes() -> None:
     if Path(".storage.txt").exists():
         Path(".storage.txt").unlink()
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/exceptions.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/dashboard/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/graph/executor_config.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/dashboard/graph/executor_config.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/graph/instance.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/dashboard/graph/instance.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/graph/node.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/dashboard/graph/node.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/graph/utils.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/dashboard/graph/utils.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/page/dependency.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/dashboard/page/dependency.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Specs for Dashboard Route Datastore Dependency."""
 
 from typing import Any
+from typing import Dict
 
 from engineai.sdk.dashboard.base import AbstractFactory
 from engineai.sdk.dashboard.decorator import type_check
-from engineai.sdk.dashboard.utils import generate_input
 
 
 class RouteDatastoreDependency(AbstractFactory):
     """Specs for Dashboard Route Datastore Dependency."""
 
     _INPUT_KEY: str = "urlQuery"
 
@@ -39,18 +39,17 @@
         """Returns dependency id.
 
         Returns:
             str: dependency
         """
         return self.__dependency_id
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Builds spec for dashboard API.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "UrlQueryDependencyInput",
-            name=self.__dependency_id,
-            query=self.__query_parameter,
-        )
+        return {
+            "name": self.__dependency_id,
+            "query": self.__query_parameter,
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/page/page.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/dashboard/page/page.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """DashboardPage spec."""
 from typing import Any
+from typing import Dict
 from typing import Final
 from typing import List
 from typing import Optional
 from typing import Union
 
 from typing_extensions import Unpack
 
@@ -18,15 +19,14 @@
 from engineai.sdk.dashboard.interface import CollapsibleInterface
 from engineai.sdk.dashboard.interface import WidgetInterface as Widget
 from engineai.sdk.dashboard.layout.card.card import Card
 from engineai.sdk.dashboard.layout.grid import Grid
 from engineai.sdk.dashboard.layout.selectable.base import SelectableSection
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 
 from ...base import DependencyInterface
 from ...links import RouteLink
 from .dependency import RouteDatastoreDependency
 from .root import RootGrid
 from .route import Route
 
@@ -120,49 +120,46 @@
             if dashboard_widget_ids.count(widget_id) > 1:
                 duplicated_widget_ids.append(widget_id)
         if duplicated_widget_ids:
             raise DashboardDuplicatedWidgetIdsError(
                 slug=self.__dashboard_slug, widget_ids=duplicated_widget_ids
             )
 
-    def _build_content(self) -> Any:
+    def _build_content(self) -> Dict[str, Any]:
         return {
-            "grid": generate_input(
-                "DashboardPageContentGridInput",
-                rowHeightPixels=ROW_HEIGHT_PIXELS,
-                rootGrid=self.__grid.build(),
-            )
+            "grid": {
+                "rowHeightPixels": ROW_HEIGHT_PIXELS,
+                "rootGrid": self.__grid.build(),
+            }
         }
 
-    def __build_dependencies(self) -> Any:
+    def __build_dependencies(self) -> List[Dict[str, Any]]:
         dependencies = set()
         if self.__route is not None:
             for dependency in self.__route.dependency:
                 dependencies.add(dependency)
 
         if not isinstance(self.__name, (str, RouteLink)):
             dependencies.add(self.__name.dependency)
 
         return [self.__build_dependency(dependency) for dependency in dependencies]
 
     @staticmethod
     def __build_dependency(
         dependency: Union[RouteDatastoreDependency, DependencyInterface]
-    ) -> Any:
-        return generate_input(
-            "DashboardPageDependencyUnionInput",
+    ) -> Dict[str, Any]:
+        return {
             **{dependency.input_key: dependency.build()},
-        )
+        }
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Builds spec for Dashboard Page."""
-        return generate_input(
-            "DashboardPageInput",
-            path=self.__path,
-            name=build_templated_strings(items=self.__name),
-            content=self._build_content(),
-            selectable=False,
-            searchable=False,
-            controlBar=None,
-            entities=[],
-            dependencies=self.__build_dependencies(),
-        )
+        return {
+            "path": self.__path,
+            "name": build_templated_strings(items=self.__name),
+            "content": self._build_content(),
+            "selectable": False,
+            "searchable": False,
+            "controlBar": None,
+            "entities": [],
+            "dependencies": self.__build_dependencies(),
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/page/root.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/dashboard/page/root.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Spec for a root grid in a dashboard."""
 
 from typing import Any
+from typing import Dict
 from typing import List
 from typing import Union
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.interface import CollapsibleInterface as CollapsibleSection
 from engineai.sdk.dashboard.layout import FluidRow
 from engineai.sdk.dashboard.layout import Grid
 from engineai.sdk.dashboard.layout import Row
 from engineai.sdk.dashboard.layout.typings import LayoutItem
-from engineai.sdk.dashboard.utils import generate_input
 
 
 class RootGrid(Grid):
     """Spec for a root grid in a dashboard."""
 
     @type_check
     def __init__(
@@ -28,30 +28,30 @@
         """
         super().__init__()
         self._rows: List[Union[Row, FluidRow, CollapsibleSection]] = [
             item if isinstance(item, (Row, FluidRow, CollapsibleSection)) else Row(item)
             for item in items
         ]
 
-    def __build_rows(self) -> List[Any]:
+    def __build_rows(self) -> List[Dict[str, Any]]:
         rows = []
         for row in self._rows:
             rows.append(
-                generate_input(
-                    "DashboardRootGridRowUnionInput",
-                    fluid=row.build() if isinstance(row, FluidRow) else None,
-                    responsive=row.build() if isinstance(row, Row) else None,
-                    card=row.build() if isinstance(row, CollapsibleSection) else None,
-                )
+                {
+                    "fluid": row.build() if isinstance(row, FluidRow) else None,
+                    "responsive": row.build() if isinstance(row, Row) else None,
+                    "card": row.build()
+                    if isinstance(row, CollapsibleSection)
+                    else None,
+                }
             )
         return rows
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "DashboardRootGridInput",
-            rows=self.__build_rows(),
-        )
+        return {
+            "rows": self.__build_rows(),
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/page/route.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/dashboard/page/route.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Specs for dashboard Route."""
 from typing import Any
+from typing import Dict
 from typing import List
 from typing import Union
 
 import pandas as pd
 from typing_extensions import Unpack
 
 from engineai.sdk.dashboard.abstract.typing import PrepareParams
@@ -74,10 +75,10 @@
         """Page routing has no validations to do."""
 
     @property
     def dependency(self) -> List[Union[RouteDatastoreDependency, DependencyInterface]]:
         """Returns dependency."""
         return [self.__dependency, self._route_data_dependency]
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Build Item."""
         # TODO Need to validate if we can remove this method.
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/version/version.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/dashboard/version/version.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Dashboard version class."""
 import re
 import warnings
 from datetime import datetime
 from typing import Any
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 from typing import cast
 
 import pytz
 from typing_extensions import Unpack
@@ -16,15 +17,14 @@
 from engineai.sdk.dashboard.dashboard.exceptions import DashboardVersionValueError
 from engineai.sdk.dashboard.dashboard.exceptions import (
     MetadataLastAvailableDataTypeError,
 )
 
 from ... import config
 from ...abstract.typing import PrepareParams
-from ...utils import generate_input
 
 
 class DashboardVersion(AbstractFactory):
     """Spec for Dashboard version."""
 
     def __init__(
         self,
@@ -123,25 +123,24 @@
                     f"Setting `last_available_data` to None."
                 )
 
             self.__last_available_data = (
                 datetime.fromtimestamp(cast(float, date)) if date is not None else date
             )
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Builds spec for dashboard API.
 
         Returns:
             Input object for Dashboard API
 
         Raises:
             AttributeError: if widgets were added to dashboards but not to layout, or
                 vice-versa.
         """
-        return generate_input(
-            "DashboardVersionInput",
-            version=self.__version,
-            createRun=self.__create_run,
-            lastRunDate=datetime.timestamp(datetime.now(tz=pytz.utc)) * 1000,
-            lastAvailableData=self._get_last_available_data,
-            status=self.__status.value if self.__status is not None else None,
-        )
+        return {
+            "version": self.__version,
+            "createRun": self.__create_run,
+            "lastRunDate": datetime.timestamp(datetime.now(tz=pytz.utc)) * 1000,
+            "lastAvailableData": self._get_last_available_data,
+            "status": self.__status.value if self.__status is not None else None,
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/data/decorator.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/data/decorator.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/data/duplicated.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/data/duplicated.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/data/enums.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/data/enums.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/data/exceptions.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/data/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/data/http.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/data/http.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,14 @@
         return "/"
 
     @property
     def dependency(self) -> HttpDependency:
         """Property to get the dependency object."""
         return self.__dependency
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
         return self.__dependency.build()
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/data/io_handler.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/data/io_handler.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/data/manager/interface.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/data/manager/interface.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/data/manager/manager.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/data/manager/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 from engineai.sdk.dashboard.links import RouteLink
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.abstract import AbstractFactoryLinkItemsHandler
 from engineai.sdk.dashboard.widgets.exceptions import WidgetTemplateStringWidgetNotFound
 
 from ...base import DependencyInterface
 from ...dependencies.datastore import DashboardStorage
-from ...utils import generate_input
 from ..decorator import DataSource
 from ..decorator import OperationItem
 from ..enums import StorageType
 from ..http import Http
 from .interface import DependencyManagerInterface
 from .interface import StaticDataType
 
@@ -118,19 +117,18 @@
     def build_datastore_dependencies(self) -> List[Any]:
         """Build datastore dependencies."""
         return [
             self.__build_dependency(dependency) for dependency in self.__dependencies
         ]
 
     @staticmethod
-    def __build_dependency(dependency: DependencyInterface) -> Any:
-        return generate_input(
-            "WidgetOwnedDependencyUnionInput",
+    def __build_dependency(dependency: DependencyInterface) -> Dict[str, Any]:
+        return {
             **{dependency.input_key: dependency.build()},
-        )
+        }
 
     def __prepare_widget_dependencies(self, page_id: str) -> None:
         for dependency in self.__dependencies:
             if (
                 isinstance(dependency, WidgetSelectDependency)
                 and page_id
                 and not dependency.widget_id.endswith(page_id)
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/decorator.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/decorator.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/dependencies/datastore.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/dependencies/datastore.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 """Spec for defining a dependency with a widget."""
 
 from typing import Any
+from typing import Dict
 from typing import Generator
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 from engineai.sdk.dashboard.base import DependencyInterface
 from engineai.sdk.dashboard.interface import OperationInterface as OperationItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 
 
 class BaseStorage(DependencyInterface):
     """Spec for defining a dependency with a datastore."""
 
-    _API_TYPE: Optional[str] = None
-
     def __init__(
         self,
         *,
         dependency_id: str,
         series_id: str,
         operations: Optional[List[OperationItem]] = None,
     ):
@@ -66,54 +64,38 @@
         """Returns series id.
 
         Returns:
             str: series id
         """
         return self.__series_id
 
-    @property
-    def api_type(self) -> str:
-        """Returns API type.
-
-        Returns:
-            str: API type
-        """
-        if self._API_TYPE is None:
-            raise NotImplementedError(
-                f"Class {self.__class__.__name__}._API_TYPE not defined."
-            )
-        return self._API_TYPE
-
     def prepare(self, route_dependency_id: str) -> None:
         """Prepare dependency."""
         if len(route_dependency_id) > 0:
             self.__series_id = f"{self.__series_id}/{{{{{route_dependency_id}}}}}"
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Builds spec for dashboard API.
 
         Returns:
             Any: Input object for Dashboard API
         """
-        return generate_input(
-            self.api_type,
-            fileName=build_templated_strings(items=self.__series_id),
-            name=self.__dependency_id,
-            operations=[operation.build() for operation in self.__operations],
-        )
+        return {
+            "fileName": build_templated_strings(items=self.__series_id),
+            "name": self.__dependency_id,
+            "operations": [operation.build() for operation in self.__operations],
+        }
 
 
 class DashboardBlobStorage(BaseStorage):
     """Spec for defining a dependency with a datastore."""
 
     _INPUT_KEY = "dashboardSelfBlobStore"
-    _API_TYPE = "DashboardStoreSelfBlobDependencyInput"
 
 
 class DashboardFileShareStorage(BaseStorage):
     """Spec for defining a dependency with a datastore."""
 
     _INPUT_KEY = "azureFileShareSelfStorage"
-    _API_TYPE = "AzureFileShareStorageSelfDependencyInput"
 
 
 DashboardStorage = Union[DashboardBlobStorage, DashboardFileShareStorage]
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/dependencies/http/header.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/dependencies/http/header.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Specs for defining an Http Header."""
 from typing import Any
+from typing import Dict
 
 from engineai.sdk.dashboard.base import AbstractFactory
-from engineai.sdk.dashboard.utils import generate_input
 
 
 class HttpHeader(AbstractFactory):
     """Specs for defining an Http Header."""
 
     def __init__(self, key: str, value: str) -> None:
         """Constructor for HttpHeader class.
@@ -16,19 +16,16 @@
             value: value of the header.
 
         Note: Only `application/json` are supported for `Content-Type` header.
         """
         self.__key = key
         self.__value = value
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "HttpHeaderUnionInput",
-            header=generate_input(
-                "HttpHeaderInput", key=self.__key, value=self.__value
-            ),
-        )
+        return {
+            "header": {"key": self.__key, "value": self.__value},
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/dependencies/http/http.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/dependencies/http/http.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Spec for defining dependencies with a widget."""
 from typing import Any
+from typing import Dict
 from typing import List
 from typing import Optional
 
 from engineai.sdk.dashboard.base import DependencyInterface
 from engineai.sdk.dashboard.interface import OperationInterface as OperationItem
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 
 from .header import HttpHeader
 
 
 class HttpDependency(DependencyInterface):
     """Specs base for defining the Widget Dependency."""
 
@@ -55,25 +55,24 @@
         self.__dependency_id = dependency_id
 
     @property
     def operations(self) -> Optional[List[OperationItem]]:
         """Returns operations to be performed on the data."""
         return self.__operations
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Builds spec for dashboard API.
 
         Returns:
             Any: Input object for Dashboard API
         """
-        return generate_input(
-            "HttpDependencyInput",
-            name=self.dependency_id,
-            path=build_templated_strings(items=self.__path),
-            host=self.__host,
-            headers=[header.build() for header in self.__headers]
+        return {
+            "name": self.dependency_id,
+            "path": build_templated_strings(items=self.__path),
+            "host": self.__host,
+            "headers": [header.build() for header in self.__headers]
             if self.__headers is not None
             else None,
-            operations=[operation.build() for operation in self.__operations]
+            "operations": [operation.build() for operation in self.__operations]
             if self.__operations is not None
             else None,
-        )
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/dependencies/route.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/dependencies/route.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Spec for defining a dependency with a widget."""
 
 from typing import Any
+from typing import Dict
 from typing import Generator
 from typing import Optional
 from typing import Tuple
 
 from engineai.sdk.dashboard.base import DependencyInterface
-from engineai.sdk.dashboard.utils import generate_input
 
 
 class RouteDependency(DependencyInterface):
     """Spec for defining a dependency with a datastore."""
 
     API_DEPENDENCY_INPUT: Optional[str] = None
     _INPUT_KEY = "dashboardPage"
@@ -51,17 +51,16 @@
         return self.__dependency_id
 
     @property
     def field_id(self) -> str:
         """Get Field ID."""
         return self.__field_id
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Builds spec for dashboard API.
 
         Returns:
             Any: Input object for Dashboard API
         """
-        return generate_input(
-            "DashboardPageVariableDependencyInput",
-            name=self.__dependency_id,
-        )
+        return {
+            "name": self.__dependency_id,
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/dependencies/widget.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/dependencies/widget.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Spec for defining dependencies with a widget."""
 from typing import Any
+from typing import Dict
 from typing import Generator
 from typing import Optional
 from typing import Tuple
 
 from engineai.sdk.dashboard.base import DependencyInterface
-from engineai.sdk.dashboard.utils import generate_input
 
 
 class WidgetSelectDependency(DependencyInterface):
     """Specs base for defining the Widget Dependency."""
 
     API_DEPENDENCY_INPUT: Optional[str] = None
     _INPUT_KEY = "widget"
@@ -62,19 +62,18 @@
         return self.__widget_id
 
     @widget_id.setter
     def widget_id(self, widget_id: str) -> None:
         """Change widget_id associated with WidgetDependency."""
         self.__widget_id = widget_id
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Builds spec for dashboard API.
 
         Returns:
             Any: Input object for Dashboard API
         """
-        return generate_input(
-            "WidgetDependencyInput",
-            widgetId=self.__widget_id,
-            path=self.__path,
-            name=self.__dependency_id,
-        )
+        return {
+            "widgetId": self.__widget_id,
+            "path": self.__path,
+            "name": self.__dependency_id,
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/enum/align.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/enum/align.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/enum/legend_position.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/enum/legend_position.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/exceptions.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/formatting/__init__.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/formatting/__init__.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/formatting/axis.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/formatting/axis.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import pandas as pd
 
 from engineai.sdk.dashboard.formatting import validator
 from engineai.sdk.dashboard.links.abstract import AbstractFactoryLinkItemsHandler
 from engineai.sdk.dashboard.templated_string import DataField
 from engineai.sdk.dashboard.templated_string import InternalDataField
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
-from engineai.sdk.dashboard.utils import generate_input
 
 from .number import NumberScale
 
 
 class AxisNumberFormatting(AbstractFactoryLinkItemsHandler):
     """Numeric axis formatting.
 
@@ -85,20 +84,19 @@
 
         Args:
             data (Union[pd.DataFrame, Dict[str, Any]]): pandas DataFrame or dict where
                 the data is present.
         """
         validator.validate(data=data, prefix=self.__prefix, suffix=self.__suffix)
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Builds spec for dashboard API.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "AxisNumberFormattingInput",
-            scale=self.scale.value,
-            seriesDecimals=self.decimals,
-            prefix=self.__prefix.build() if self.__prefix else None,
-            suffix=self.__suffix.build() if self.__suffix else None,
-        )
+        return {
+            "scale": self.scale.value,
+            "seriesDecimals": self.decimals,
+            "prefix": self.__prefix.build() if self.__prefix else None,
+            "suffix": self.__suffix.build() if self.__suffix else None,
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/formatting/datetime.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/formatting/datetime.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Formatting spec for dates."""
 import enum
 import warnings
 from typing import Any
+from typing import Dict
 from typing import Optional
 
 from engineai.sdk.dashboard.base import AbstractFactory
-from engineai.sdk.dashboard.utils import generate_input
 
 
 class DateTimeUnit(enum.Enum):
     """DateTime units."""
 
     DATE = "DATE"
     TIME = "TIME"
@@ -51,18 +51,17 @@
         }
 
         self.__template = (
             default_template[time_unit.value] if not template else template
         )
         self.__time_unit = time_unit
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Builds spec for dashboard API.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "DateTimeFormattingInput",
-            template=self.__template,
-            timeUnit=self.__time_unit.value,
-        )
+        return {
+            "template": self.__template,
+            "timeUnit": self.__time_unit.value,
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/formatting/exceptions.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/formatting/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/formatting/mapper.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/formatting/mapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Formatting spec for Key/Value."""
 
 from typing import Any
+from typing import Dict
+from typing import List
 from typing import Mapping
 
 from engineai.sdk.dashboard.base import AbstractFactory
-from engineai.sdk.dashboard.utils import generate_input
 
 
 class MapperFormatting(AbstractFactory):
     """Factory class to map a column with ordinal numbers to text.
 
     Factory class to map ordinal numbers to text
     labels for categorical data.
@@ -28,20 +29,19 @@
         """Returns formatting mapping between integer numbers and labels.
 
         Returns:
             Mapping[int, str]: formatting mapping
         """
         return self.__mapping
 
-    def _build_mapping(self) -> Any:
+    def _build_mapping(self) -> List[Dict[str, Any]]:
         return [
-            generate_input("KeyValueInput", key=str(key), value=self.__mapping[key])
-            for key in self.__mapping
+            {"key": str(key), "value": self.__mapping[key]} for key in self.__mapping
         ]
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Builds spec for dashboard API.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input("MapperFormattingInput", mapping=self._build_mapping())
+        return {"mapping": self._build_mapping()}
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/formatting/number.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/formatting/number.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from engineai.sdk.dashboard.formatting import validator
 from engineai.sdk.dashboard.links.abstract import AbstractFactoryLinkItemsHandler
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.templated_string import DataField
 from engineai.sdk.dashboard.templated_string import InternalDataField
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 
 
 class NumberScale(enum.Enum):
     """Scales to format numbers."""
 
     BASE = "BASE"  # no scale applied
     PERCENTAGE = "PERCENTAGE"  # numbers are multiplied by 100 and a suffix % is added
@@ -109,24 +108,23 @@
 
         Args:
             data (Union[pd.DataFrame, Dict[str, Any]]): pandas DataFrame or dict where
                 the data is present.
         """
         validator.validate(data=data, prefix=self.__prefix, suffix=self.__suffix)
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Builds spec for dashboard API.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "NumberFormattingInput",
-            scale=self.scale.value if isinstance(self.scale, NumberScale) else None,
-            scaleOverrideVariable=build_templated_strings(items=self.__scale)
+        return {
+            "scale": self.scale.value if isinstance(self.scale, NumberScale) else None,
+            "scaleOverrideVariable": build_templated_strings(items=self.__scale)
             if not isinstance(self.__scale, NumberScale)
             else None,
-            decimals=self.decimals,
-            prefix=self.__prefix.build() if self.__prefix else None,
-            suffix=self.__suffix.build() if self.__suffix else None,
-            showPositiveSign=self.__show_positive_sign,
-        )
+            "decimals": self.decimals,
+            "prefix": self.__prefix.build() if self.__prefix else None,
+            "suffix": self.__suffix.build() if self.__suffix else None,
+            "showPositiveSign": self.__show_positive_sign,
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/formatting/text.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/formatting/text.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Formatting spec for text."""
 
 from typing import Any
+from typing import Dict
 from typing import Optional
 
 from engineai.sdk.dashboard.base import AbstractFactory
-from engineai.sdk.dashboard.utils import generate_input
 
 
 class TextFormatting(AbstractFactory):
     """Customize maximum characters and splitting options.
 
     Description for formatting text, allowing customization
     of maximum characters and splitting.
@@ -26,18 +26,17 @@
                 After split character, ... are added and full text shown on hover.
                 Defaults to None.
         """
         super().__init__()
         self.__max_characters = max_characters
         self.__split = split
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Builds spec for dashboard API.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "TextFormattingInput",
-            maxCharacters=self.__max_characters,
-            split=self.__split,
-        )
+        return {
+            "maxCharacters": self.__max_characters,
+            "split": self.__split,
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/formatting/validator.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/formatting/validator.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/interface.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/interface.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/__init__.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/card/card.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/card/card.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Spec for a Card in a dashboard  grid layout."""
 
 from typing import Any
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 from typing_extensions import Unpack
 
 from engineai.sdk.dashboard.abstract.layout import AbstractLayoutItem
@@ -12,15 +13,14 @@
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.interface import CardInterface
 from engineai.sdk.dashboard.interface import WidgetInterface as Widget
 from engineai.sdk.dashboard.layout.build_item import build_item
 from engineai.sdk.dashboard.layout.exceptions import ElementHeightNotDefinedError
 from engineai.sdk.dashboard.layout.typings import LayoutItem
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
-from engineai.sdk.dashboard.utils import generate_input
 
 from ...base import DependencyInterface
 from .header import CardHeader
 
 
 class Card(CardInterface):
     """Groups content with widgets, grids, and selectable sections.
@@ -137,33 +137,31 @@
     def prepare_heights(self, row_height: Optional[Union[float, int]] = None) -> None:
         """Prepare Selectable Layout heights."""
         if not isinstance(self.__content, Widget):
             self.__content.prepare_heights(row_height=row_height)
 
         self.__height = row_height or self.__content.height
 
-    def __build_dependencies(self) -> List[Any]:
+    def __build_dependencies(self) -> List[Dict[str, Any]]:
         """Build dependencies for Card."""
         dependencies = []
         for dependency in self.__header.dependencies:
             dependencies.append(self.__build_dependency(dependency))
         return dependencies
 
     @staticmethod
-    def __build_dependency(dependency: DependencyInterface) -> Any:
-        return generate_input(
-            "DashboardGridCardDependencyUnionInput",
+    def __build_dependency(dependency: DependencyInterface) -> Dict[str, Any]:
+        return {
             **{dependency.input_key: dependency.build()},
-        )
+        }
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "DashboardGridCardInput",
-            item=build_item(self.__content),
-            header=self.__header.build(),
-            dependencies=self.__build_dependencies(),
-        )
+        return {
+            "item": build_item(self.__content),
+            "header": self.__header.build(),
+            "dependencies": self.__build_dependencies(),
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/card/chip.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/card/chip.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/card/header.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/card/header.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/collapsible/chip.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/collapsible/chip.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/collapsible/header.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/collapsible/header.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/collapsible/section.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/collapsible/section.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Spec for a Collapsible Section in a dashboard grid layout."""
 
 from typing import Any
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 from typing_extensions import Unpack
 
 from engineai.sdk.dashboard.abstract.layout import AbstractLayoutItem
@@ -13,15 +14,14 @@
 from engineai.sdk.dashboard.interface import CollapsibleInterface
 from engineai.sdk.dashboard.interface import WidgetInterface as Widget
 from engineai.sdk.dashboard.layout.build_item import build_item
 from engineai.sdk.dashboard.layout.exceptions import ElementHeightNotDefinedError
 from engineai.sdk.dashboard.layout.grid import Grid
 from engineai.sdk.dashboard.layout.typings import LayoutItem
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
-from engineai.sdk.dashboard.utils import generate_input
 
 from ...base import DependencyInterface
 from .header import CollapsibleSectionHeader
 
 
 class CollapsibleSection(CollapsibleInterface):
     """Organize and group content with expandable/collapsible sections.
@@ -159,27 +159,25 @@
         """Build dependencies for Card."""
         dependencies = []
         for dependency in self.__header.dependencies:
             dependencies.append(self.__build_dependency(dependency))
         return dependencies
 
     @staticmethod
-    def __build_dependency(dependency: DependencyInterface) -> Any:
-        return generate_input(
-            "DashboardGridCardDependencyUnionInput",
+    def __build_dependency(dependency: DependencyInterface) -> Dict[str, Any]:
+        return {
             **{dependency.input_key: dependency.build()},
-        )
+        }
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "DashboardCollapsibleCardInput",
-            item=build_item(self.__content),
-            height=self.height,
-            header=self.__header.build(),
-            expanded=self.__expanded,
-            dependencies=self.__build_dependencies(),
-        )
+        return {
+            "item": build_item(self.__content),
+            "height": self.height,
+            "header": self.__header.build(),
+            "expanded": self.__expanded,
+            "dependencies": self.__build_dependencies(),
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/column.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/column.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Spec for a column in a dashboard vertical grid layout."""
 
 from typing import Any
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 from typing_extensions import Unpack
 
 from engineai.sdk.dashboard.base import AbstractFactory
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.layout.build_item import build_item
 from engineai.sdk.dashboard.layout.typings import LayoutItem
 
 from ..abstract.layout import AbstractLayoutItem
 from ..abstract.typing import PrepareParams
-from ..utils import generate_input
 from ..widgets.base import Widget
 from .exceptions import ColumnLimitsWidthError
 from .exceptions import ColumnWrongWidthSizeError
 from .exceptions import ElementHeightNotDefinedError
 
 
 class Column(AbstractFactory):
@@ -154,18 +154,17 @@
         """Returns if the Column has a forced height form the of item."""
         return self.__item.force_height if isinstance(self.__item, Widget) else False
 
     def items(self) -> List[AbstractLayoutItem]:
         """Returns list of grid items that need to be inserted individually."""
         return self.__item.items()
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "DashboardGridColumnInput",
-            width=self.__width,
-            item=build_item(self.__item),
-        )
+        return {
+            "width": self.__width,
+            "item": build_item(self.__item),
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/components/chip.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/components/chip.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Spec for the layout chip component."""
 
 from typing import Any
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 from engineai.sdk.dashboard.base import AbstractFactory
 from engineai.sdk.dashboard.base import DependencyInterface
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.layout.components.label import build_context_label
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 
 
 class BaseChip(AbstractFactory):
     """Spec for the layout chip component.
 
     This component is used in Card and CollapsibleSection components.
     """
@@ -51,26 +51,25 @@
         self.__suffix = suffix
 
     @property
     def dependencies(self) -> List[DependencyInterface]:
         """Method to generate the dependencies list from the elements of this class."""
         return [self.__label.dependency] if not isinstance(self.__label, str) else []
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Builds spec for dashboard API.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "DashboardGridCardHeaderContextInput",
-            label=build_context_label(
+        return {
+            "label": build_context_label(
                 label=self.__label,
                 separator=self.__separator,
                 prefix=self.__prefix,
                 suffix=self.__suffix,
             ),
-            tooltipText=[
+            "tooltipText": [
                 build_templated_strings(items=tooltip)
                 for tooltip in self.__tooltip_text
             ],
-        )
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/components/header.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/components/header.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Spec for the layout Header component."""
 
 from typing import Any
+from typing import Dict
 from typing import List
 from typing import Optional
 
 from engineai.sdk.dashboard.base import AbstractFactory
 from engineai.sdk.dashboard.base import DependencyInterface
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 
 from .chip import BaseChip
 
 
 class BaseHeader(AbstractFactory):
     """Spec for the layout Header component.
 
@@ -50,20 +50,19 @@
             dependencies_list.extend(chip.dependencies)
 
         if self.__title is not None and not isinstance(self.__title, str):
             if isinstance(self.__title, list):
                 dependencies_list.extend([title.dependency for title in self.__title])
             else:
                 dependencies_list.extend([self.__title.dependency])
-        return dependencies_list
+        return list(set(dependencies_list))
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Builds spec for dashboard API.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "DashboardGridCardHeaderInput",
-            title=build_templated_strings(items=self.__title),
-            context=[chip.build() for chip in self.__chips],
-        )
+        return {
+            "title": build_templated_strings(items=self.__title),
+            "context": [chip.build() for chip in self.__chips],
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/exceptions.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/fluid_row/fluid_row.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/fluid_row/fluid_row.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 """Spec for a fluid row in a dashboard vertical grid layout."""
 
 from typing import Any
+from typing import Dict
 from typing import Iterable
 from typing import List
 from typing import Optional
 from typing import Union
 
 from typing_extensions import Unpack
 
 from engineai.sdk.dashboard.abstract.typing import PrepareParams
 from engineai.sdk.dashboard.base import AbstractFactory
 from engineai.sdk.dashboard.enum.align import (
     FluidHorizontalAlignment as HorizontalAlignment,
 )
 from engineai.sdk.dashboard.enum.align import VerticalAlignment
-from engineai.sdk.dashboard.utils import generate_input
 
+from ...widgets.base import Widget
 from ..exceptions import ElementHeightNotDefinedError
-from .items_build import DashboardFluidRowItem
-from .items_build import build_fluid_item
 
 
 class FluidRow(AbstractFactory):
     """Enables flexible and responsive content alignment in a vertical grid layout.
 
     The FluidRow class represents a fluid row within a vertical grid layout,
     allowing for flexible and responsive content alignment.
     """
 
     def __init__(
         self,
-        *items: DashboardFluidRowItem,
+        *items: Widget,
         vertical_alignment: VerticalAlignment = VerticalAlignment.TOP,
         horizontal_alignment: HorizontalAlignment = HorizontalAlignment.CENTER,
     ) -> None:
         """Constructor for FluidRow.
 
         Args:
-            items: item within the FluidRow. One of Select, Toggle.
+            items: item within the FluidRow must be compatible.
             vertical_alignment: Fluid Row vertical alignment option.
                 `TOP`, `MIDDLE` or `BOTTOM`, available.
             horizontal_alignment: Fluid Row horizontal alignment option.
                 `LEFT`, `CENTER`, `RIGHT` or `STRETCH` available.
 
         Examples:
             ??? example "Create Fluid Row with widget"
@@ -102,23 +101,28 @@
                             horizontal_alignment=align.FluidHorizontalAlignment.LEFT,
                         )
                     )
                 )
                 ```
         """
         super().__init__()
-        self.__items: List[DashboardFluidRowItem] = []
+        self.__items: List[Widget] = []
         self.__set_items(*items)
         self.__height: Optional[Union[float, int]] = None
         self.__vertical_alignment = vertical_alignment.value
         self.__horizontal_alignment = horizontal_alignment.value
 
-    def __set_items(self, *items: DashboardFluidRowItem) -> None:
+    def __set_items(self, *items: Widget) -> None:
         """Set items for fluid row."""
         for item in items:
+            if not item.fluid_row_compatible:
+                raise ValueError(
+                    f"Item {item} is not compatible with FluidRow. "
+                    "Please use a compatible item."
+                )
             self.__items.append(item)
 
     def prepare_heights(self) -> None:
         """Prepare fluid row heights."""
         self.__height = float(max(item.height for item in self.__items))
 
     @property
@@ -129,38 +133,37 @@
     @property
     def height(self) -> Union[float, int]:
         """Get row height."""
         if self.__height is None:
             raise ElementHeightNotDefinedError()
         return self.__height
 
-    def items(self) -> Iterable[DashboardFluidRowItem]:
+    def items(self) -> Iterable[Widget]:
         """Return items associated."""
         return self.__items
 
     @property
-    def widgets(self) -> List[DashboardFluidRowItem]:
+    def widgets(self) -> List[Widget]:
         """Returns list of widgets in dashboard grid row layout.
 
         Returns:
             List[Widget]: list of widget
         """
         return self.__items
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "DashboardFluidRowInput",
-            height=self.__height,
-            items=[build_fluid_item(item=item) for item in self.__items],
-            verticalAlign=self.__vertical_alignment,
-            horizontalAlign=self.__horizontal_alignment,
-        )
+        return {
+            "height": self.__height,
+            "items": [{"widget": item.build()} for item in self.__items],
+            "verticalAlign": self.__vertical_alignment,
+            "horizontalAlign": self.__horizontal_alignment,
+        }
 
     def prepare(self, **kwargs: Unpack[PrepareParams]) -> None:
         """Prepare row."""
         for item in self.__items:
             item.prepare(**kwargs)
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/grid.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/grid.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Spec for a grid in a dashboard vertical grid layout."""
 
 from typing import Any
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 from typing_extensions import Unpack
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.layout.typings import LayoutItem
 
 from ..abstract.layout import AbstractLayoutItem
 from ..abstract.typing import PrepareParams
 from ..interface import GridInterface
-from ..utils import generate_input
 from .exceptions import ElementHeightNotDefinedError
 from .fluid_row.fluid_row import FluidRow
 from .row import Row
 
 
 class Grid(GridInterface):
     """Organize dashboard content with vertical grid structure.
@@ -181,29 +181,27 @@
     def items(self) -> List[AbstractLayoutItem]:
         """Returns list of grid items that need to be inserted individually."""
         items: List[AbstractLayoutItem] = []
         for row in self._rows:
             items += row.items()
         return items
 
-    def __build_rows(self) -> List[Any]:
+    def __build_rows(self) -> List[Dict[str, Any]]:
         rows = []
         for row in self._rows:
             rows.append(
-                generate_input(
-                    "DashboardGridRowUnionInput",
-                    fluid=row.build() if isinstance(row, FluidRow) else None,
-                    responsive=row.build() if isinstance(row, Row) else None,
-                )
+                {
+                    "fluid": row.build() if isinstance(row, FluidRow) else None,
+                    "responsive": row.build() if isinstance(row, Row) else None,
+                }
             )
         return rows
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "DashboardGridInput",
-            rows=self.__build_rows(),
-        )
+        return {
+            "rows": self.__build_rows(),
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/row.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/row.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Spec for a row in a dashboard vertical grid layout."""
 
 from typing import Any
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 from typing_extensions import Unpack
 
 from engineai.sdk.dashboard.base import AbstractFactory
 from engineai.sdk.dashboard.decorator import type_check
 
 from ..abstract.layout import AbstractLayoutItem
 from ..abstract.typing import PrepareParams
-from ..utils import generate_input
 from .column import Column
 from .exceptions import ElementHeightNotDefinedError
 from .exceptions import RowColumnsAutoWidthError
 from .exceptions import RowColumnsCustomWidthError
 from .exceptions import RowColumnsMaximumWidthError
 from .exceptions import RowMaximumAutoWidthItemsError
 from .exceptions import RowMaximumItemsError
@@ -265,18 +265,17 @@
     def items(self) -> List[AbstractLayoutItem]:
         """Returns list of grid items that need to be inserted individually."""
         items: List[AbstractLayoutItem] = []
         for column in self.__columns:
             items += column.items()
         return items
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "DashboardGridRowInput",
-            height=self.__height,
-            columns=[column.build() for column in self.__columns],
-        )
+        return {
+            "height": self.__height,
+            "columns": [column.build() for column in self.__columns],
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/selectable/base.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/selectable/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Specs for selectable layouts in a dashboard vertical grid."""
 
 import logging
 from abc import abstractmethod
 from typing import Any
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Set
 from typing import Union
 
 from typing_extensions import Unpack
 
@@ -113,26 +114,25 @@
         return self.__label
 
     def items(self) -> List[AbstractLayoutItem]:
         """Returns list of grid items that need to be inserted individually."""
         return self.__content.items()
 
     @abstractmethod
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
 
 
 class SelectableSection(SelectableInterface):
     """Spec for section in a dashboard vertical grid layout."""
 
-    _API_TYPE: Optional[str] = None
     _HEIGHT_TITLE = 0.48
 
     @type_check
     def __init__(
         self,
     ) -> None:
         """Construct Selectable Section for dashboard vertical grid layout."""
@@ -170,26 +170,14 @@
         return self.__height
 
     @property
     def has_custom_heights(self) -> bool:
         """Returns whether grid has custom heights."""
         return any(item.has_custom_heights for item in self._items)
 
-    @property
-    def _api_type(self) -> str:
-        """Returns API type argument value.
-
-        All Select Layout Items must now have the _API_TYPE defined.
-        """
-        if self._API_TYPE is None:
-            raise NotImplementedError(
-                f"Class {self.__class__.__name__}._API_TYPE not defined."
-            )
-        return self._API_TYPE
-
     def items(self) -> List[AbstractLayoutItem]:
         """Returns list of grid items that need to be inserted individually."""
         items: List[AbstractLayoutItem] = [self]
         for selectable in self._items:
             items += selectable.items()
         return items
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/selectable/exceptions.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/selectable/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/selectable/tab.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/selectable/tab.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Specs for Tab and TabSection."""
 
 from typing import Any
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.layout.build_item import build_item
 from engineai.sdk.dashboard.layout.typings import LayoutItem
 from engineai.sdk.dashboard.links.widget_field import WidgetField
 from engineai.sdk.dashboard.styling.icons import Icons
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.utils import is_valid_url
 
 from .base import SelectableItem
 from .base import SelectableSection
 
 
 class Tab(SelectableItem):
@@ -47,40 +47,38 @@
 
     def validate_icon(self, icon: Optional[Union[Icons, WidgetField, str]]) -> None:
         """Check if the icon is valid."""
         if icon is not None:
             if isinstance(icon, str):
                 is_valid_url(icon)
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec."""
-        return generate_input(
-            "DashboardGridTabSectionOptionInput",
-            label=build_templated_strings(items=self.label),
-            item=build_item(self.item),
-            icon=build_templated_strings(
+        return {
+            "label": build_templated_strings(items=self.label),
+            "item": build_item(self.item),
+            "icon": build_templated_strings(
                 items=self.__icon.value
                 if isinstance(self.__icon, Icons)
                 else self.__icon
             )
             if self.__icon is not None
             else None,
-            preSelected=self.default_selected,
-        )
+            "preSelected": self.default_selected,
+        }
 
 
 class TabSection(SelectableSection):
     """Organize dashboard content within tabs.
 
     The TabSection class is a crucial part of a dashboard
     layout, allowing users to organize content within tabs.
 
     """
 
-    _API_TYPE = "tabSection"
     _INPUT_KEY = "tabSection"
 
     @type_check
     def __init__(
         self,
         *tabs: Tab,
     ):
@@ -116,17 +114,16 @@
 
                 Dashboard(content=TabSection(tab_1, tab_2, tab_3))
                 ```
         """
         super().__init__()
         self._add_items(*tabs)
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "DashboardGridTabSectionInput",
-            options=[tab.build() for tab in self._items],
-        )
+        return {
+            "options": [tab.build() for tab in self._items],
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/typings.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/layout/typings.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/links/abstract.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/links/abstract.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/links/route_link.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/links/route_link.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/links/template_string_link.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/links/template_string_link.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/links/url.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/links/url.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/links/widget_dependency.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/links/widget_dependency.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 """Specs for WidgetDependencyValue."""
 
 from typing import Any
+from typing import Dict
 
 from engineai.sdk.dashboard.base import AbstractFactory
 from engineai.sdk.dashboard.links.widget_field import WidgetField
-from engineai.sdk.dashboard.utils import generate_input
 
 
 class WidgetDependencyValue(AbstractFactory):
     """Specs for Widget Dependency Value."""
 
     def __init__(self, widget_field: WidgetField):
         """Construct for WidgetDependencyValue class.
 
         Args:
             widget_field (WidgetField): Widget field.
         """
         self.__widget_field = widget_field
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Builds spec for dashboard API.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "WidgetDependencyValueInput",
-            id=self.__widget_field.link_component.widget_id,
-            state="selected",
-            path=["0", self.__widget_field.field],
-        )
+        return {
+            "id": self.__widget_field.link_component.widget_id,
+            "state": "selected",
+            "path": ["0", self.__widget_field.field],
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/links/widget_field.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/links/widget_field.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/selected.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/selected.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/color/__init__.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/styling/color/__init__.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/color/default_specs.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/styling/color/default_specs.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/color/discrete_map.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/styling/color/discrete_map.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Spec for Discrete color map."""
 
 from typing import Any
+from typing import Dict
 from typing import List
 from typing import Protocol
 from typing import Union
 
 from engineai.sdk.dashboard.base import AbstractFactory
 from engineai.sdk.dashboard.decorator import type_check
-from engineai.sdk.dashboard.utils import generate_input
 
 from .palette import Palette
 from .single import Single
 
 
 class DiscreteMapIntervalItem(AbstractFactory):
     """Map value intervals to colors.
@@ -44,28 +44,27 @@
         super().__init__()
         self.__color = color if isinstance(color, Single) else Single(color=color)
         self.__min = min_value
         self.__max = max_value
         self.__exclude_min = exclude_min
         self.__exclude_max = exclude_max
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Builds spec for dashboard API.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "ColorDiscreteMapIntervalInput",
-            min=self.__min,
-            max=self.__max,
-            color=self.__color.build(),
-            excludeMax=self.__exclude_max,
-            excludeMin=self.__exclude_min,
-        )
+        return {
+            "min": self.__min,
+            "max": self.__max,
+            "color": self.__color.build(),
+            "excludeMax": self.__exclude_max,
+            "excludeMin": self.__exclude_min,
+        }
 
 
 class DiscreteMapValueItem(AbstractFactory):
     """Map single values to colors.
 
     Create a specification to represent a discrete mapping between a
     single value and a specific color within a discrete color map.
@@ -84,23 +83,21 @@
             color: color applied to interval (Palette)
                 or color itself (Single).
         """
         super().__init__()
         self.__color = color if isinstance(color, Single) else Single(color=color)
         self.__value = value
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Builds spec for dashboard API.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "ColorDiscreteMapValueInput", color=self.__color.build(), value=self.__value
-        )
+        return {"color": self.__color.build(), "value": self.__value}
 
 
 DiscreteMapItem = Union[DiscreteMapIntervalItem, DiscreteMapValueItem]
 
 
 class DiscreteMap(AbstractFactory):
     """Map values to specific colors.
@@ -153,32 +150,31 @@
         """
         super().__init__()
         self.__items: List[DiscreteMapItem] = list(items)
 
     @staticmethod
     def __build_item(
         item: DiscreteMapItem,
-    ) -> Any:
+    ) -> Dict[str, Any]:
         if isinstance(item, DiscreteMapValueItem):
             input_key = "value"
         else:
             input_key = "interval"
 
-        return generate_input("ColorDiscreteMapItemInput", **{input_key: item.build()})
+        return {**{input_key: item.build()}}
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Builds spec for dashboard API.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "ColorDiscreteMapInput",
-            items=[self.__build_item(item) for item in self.__items],
-        )
+        return {
+            "items": [self.__build_item(item) for item in self.__items],
+        }
 
 
 class _ColorMethod(Protocol):
     def __call__(self, *, index: int) -> Palette:
         ...
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/color/divergent.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/styling/color/divergent.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Spec for Color Divergent class."""
 
 from typing import Any
+from typing import Dict
 
 from engineai.sdk.dashboard.base import AbstractFactory
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.styling.color.palette import Palette
 from engineai.sdk.dashboard.styling.color.spec import ColorSpec
 from engineai.sdk.dashboard.styling.color.spec import build_color_spec
-from engineai.sdk.dashboard.utils import generate_input
 
 from .single import Single
 
 
 class Divergent(AbstractFactory):
     """Creates a class for a Color Divergent."""
 
@@ -34,20 +34,19 @@
         """
         super().__init__()
         self.__mid_value = mid_value
         self.__mid_color = Single(color=mid_color)
         self.__above_color = above_color
         self.__below_color = below_color
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Builds spec for dashboard API.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "ColorDivergentPaletteInput",
-            midValue=self.__mid_value,
-            midColor=self.__mid_color.build(),
-            aboveColor=build_color_spec(self.__above_color),
-            belowColor=build_color_spec(self.__below_color),
-        )
+        return {
+            "midValue": self.__mid_value,
+            "midColor": self.__mid_color.build(),
+            "aboveColor": build_color_spec(self.__above_color),
+            "belowColor": build_color_spec(self.__below_color),
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/color/gradient.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/styling/color/gradient.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Spec for Gradients."""
 
 from typing import Any
+from typing import Dict
 from typing import Union
 
 from engineai.sdk.dashboard.base import AbstractFactory
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.styling.color.palette import Palette
-from engineai.sdk.dashboard.utils import generate_input
 
 from .single import Single
 
 
 class GradientItem(AbstractFactory):
     """Represents value and corresponding color in a gradient.
 
@@ -33,23 +33,21 @@
             color: color applied to interval (Palette)
                 or color itself (Single).
         """
         super().__init__()
         self.__color = color if isinstance(color, Single) else Single(color=color)
         self.__value = value
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Builds spec for dashboard API.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "GradientItemInput", color=self.__color.build(), value=self.__value
-        )
+        return {"color": self.__color.build(), "value": self.__value}
 
 
 class Gradient(AbstractFactory):
     """Define gradient for smooth transitions between colors.
 
     Create a specification for defining a color gradient, allowing
     for smooth transitions between colors. The Gradient class
@@ -102,18 +100,17 @@
                 Dashboard(content=ts)
                 ```
         """
         super().__init__()
         self.__items = items
         self.__steps = steps
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Builds spec for dashboard API.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "ColorGradientInput",
-            colorMap=[item.build() for item in self.__items],
-            nSteps=self.__steps,
-        )
+        return {
+            "colorMap": [item.build() for item in self.__items],
+            "nSteps": self.__steps,
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/color/palette.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/styling/color/palette.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/color/single.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/cartesian/legend.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,29 @@
-"""Spec for SingleColor class."""
-
+"""Spec for legend of a categorical widget."""
 from typing import Any
+from typing import Dict
 
 from engineai.sdk.dashboard.base import AbstractFactory
 from engineai.sdk.dashboard.decorator import type_check
-from engineai.sdk.dashboard.utils import generate_input
-
-from .palette import Palette
+from engineai.sdk.dashboard.enum.legend_position import LegendPosition
 
 
-class Single(AbstractFactory):
-    """Class for creating a single color instance.
+class Legend(AbstractFactory):
+    """Spec for legend of a categorical widget.
 
-    Create a class representing a single color within
-    a palette for a Timeseries widget.
+    Args:
+        position: location of position relative to data, charts.
     """
 
     @type_check
-    def __init__(self, color: Palette):
-        """Constructor for Single.
-
-        Args:
-            color: a color from Palette.
-        """
+    def __init__(self, *, position: LegendPosition = LegendPosition.BOTTOM):
+        """Construct a legend for a categorical widget."""
         super().__init__()
-        self.__color = color.color
+        self.__position = position
 
-    def build(self) -> Any:
-        """Builds spec for dashboard API.
+    def build(self) -> Dict[str, Any]:
+        """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "ColorSingleInput",
-            customColor=self.__color,
-        )
+        return {"position": self.__position.value}
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/color/spec.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/styling/color/spec.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Color spec helpers."""
 
 from typing import Any
+from typing import Dict
 
 from engineai.sdk.dashboard.styling.color.palette import Palette
-from engineai.sdk.dashboard.utils import generate_input
 
 from .discrete_map import DiscreteMap
 from .gradient import Gradient
 from .single import Single
 from .typing import ColorSpec
 
 
-def build_color_spec(spec: ColorSpec) -> Any:
+def build_color_spec(spec: ColorSpec) -> Dict[str, Any]:
     """Builds spec for dashboard API.
 
     Returns:
         Input object for Dashboard API
     """
     if isinstance(spec, Gradient):
         input_key = "gradient"
@@ -27,8 +27,8 @@
         spec = Single(color=spec)
         input_key = "single"
     else:
         raise TypeError(
             "spec needs to be one of Palette, Gradient, Single, DiscreteMap."
         )
 
-    return generate_input("ColorSpecInput", **{input_key: spec.build()})
+    return {input_key: spec.build()}
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/icons.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/styling/icons.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/templated_string.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/templated_string.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from typing import cast
 
 import pandas as pd
 
 from engineai.sdk.dashboard.exceptions import DataFieldColumnNameNotProvidedError
 from engineai.sdk.dashboard.exceptions import DataFieldInItemIDKeyNotFoundError
 from engineai.sdk.dashboard.exceptions import DataFieldNotFoundError
-from engineai.sdk.dashboard.utils import generate_input
 
 from .base import AbstractLink
 
 TemplatedStringItem = Union[
     str,
     AbstractLink,
     List[AbstractLink],
@@ -85,35 +84,35 @@
         else:
             return param in cast(Dict[str, Any], data).keys()
 
     def __build_value_dependency(
         self,
         value: Optional[TemplatedStringItem] = None,
         value_key: Optional[TemplatedStringItem] = None,
-    ) -> Optional[Any]:
+    ) -> Optional[Dict[str, Any]]:
         """Builds spec for value dependency.
 
         Args:
             value (TemplatedStringItem]): value to be
                 displayed in the templated string.
             value_key (TemplatedStringItem]): value key to be
                 displayed in the templated string.
 
         """
         if value is None and value_key is None:
-            return generate_input(
-                "WidgetVariableDependencyValueInput",
-                value=build_templated_strings(items=None),
-                valueKey=build_templated_strings(items=None),
-            )
-        return generate_input(
-            "WidgetVariableDependencyValueInput",
-            value=build_templated_strings(items=value) if value is not None else None,
-            valueKey=build_templated_strings(items=value_key) if value_key else None,
-        )
+            return {
+                "value": build_templated_strings(items=None),
+                "valueKey": build_templated_strings(items=None),
+            }
+        return {
+            "value": build_templated_strings(items=value)
+            if value is not None
+            else None,
+            "valueKey": build_templated_strings(items=value_key) if value_key else None,
+        }
 
     def validate(
         self,
         data: Union[pd.DataFrame, Dict[str, Any]],
         column_name: Optional[str] = None,
         node: Optional[str] = None,
         item_id_key: Optional[str] = None,
@@ -194,16 +193,16 @@
             f"Use str or WidgetField."
         )
 
     if items is not None:
         template = _build_template(
             items=items, separator=separator, prefix=prefix, suffix=suffix
         )
-        return generate_input("TemplatedStringInput", template=template)
-    return generate_input("TemplatedStringInput", template="")
+        return {"template": template}
+    return {"template": ""}
 
 
 def _build_template(
     *,
     items: TemplatedStringItem,
     separator: str = "-",
     prefix: str = "",
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/base.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Base spec shared by all widgets."""
 import re
 from abc import abstractmethod
 from typing import Any
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 import pandas as pd
 from typing_extensions import Unpack
 
@@ -16,29 +17,29 @@
 from engineai.sdk.dashboard.dependencies import WidgetSelectDependency
 from engineai.sdk.dashboard.exceptions import WidgetDataNotFoundError
 from engineai.sdk.dashboard.exceptions import WidgetFieldNotFoundError
 from engineai.sdk.dashboard.interface import WidgetInterface
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.selected import Selected
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.exceptions import WidgetIdValueError
 
 from ..abstract.layout import AbstractLayoutItem
 from ..abstract.selectable_widgets import AbstractSelectWidget
 
 WidgetTitleType = Optional[Union[str, GenericLink]]
 
 
 class Widget(DependencyManager, AbstractLayoutItem, WidgetInterface):
     """Building blocks of visualizations within the Platform SDK."""
 
     _WIDGET_API_TYPE: Optional[str] = None
     _DEFAULT_HEIGHT: Union[int, float] = 4
     _FORCE_HEIGHT: bool = False
+    _FLUID_ROW_COMPATIBLE: bool = False
     _WIDGET_HEIGHT_STEP = 0.1
     _WIDGET_ID_COUNTER = 0
     _INPUT_KEY = "widget"
 
     @type_check
     def __init__(
         self,
@@ -57,14 +58,19 @@
         super().__init__(
             base_path=(__widget_id := self.__set_widget_id(widget_id)),
             data=data,
         )
         self.__widget_id = __widget_id
 
     @property
+    def fluid_row_compatible(self) -> bool:
+        """Returns True if widget is compatible with fluid row."""
+        return self._FLUID_ROW_COMPATIBLE
+
+    @property
     def data_id(self) -> str:
         """Returns data id."""
         return self.__widget_id
 
     def __set_widget_id(self, widget_id: Optional[str]) -> str:
         if widget_id is None:
             self._increment_widget_id_counter()
@@ -148,15 +154,15 @@
         if self._INPUT_KEY is None:
             raise NotImplementedError(
                 f"Class {self.__class__.__name__}._INPUT_KEY not defined."
             )
         return self._INPUT_KEY
 
     @abstractmethod
-    def _build_widget_input(self) -> Any:
+    def _build_widget_input(self) -> Dict[str, Any]:
         """Builds widget Input specs for dashboard API.
 
         Returns:
             Dictionary with widget name and spec.
         """
 
     def prepare(self, **kwargs: Unpack[PrepareParams]) -> None:
@@ -169,31 +175,28 @@
         page_id = re.sub(r"\W+", "", path)
         if page_id:
             self.__widget_id = f"{self.__widget_id}_{page_id}"
 
     def _prepare(self, **kwargs: object) -> None:
         """Method for each Widget prepare before building."""
 
-    def _build_widget_type(self) -> Any:
-        return generate_input(
-            "WidgetTypeInput", **{self._widget_api_type: self._build_widget_input()}
-        )
+    def _build_widget_type(self) -> Dict[str, Any]:
+        return {**{self._widget_api_type: self._build_widget_input()}}
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Builds spec for dashboard API.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "WidgetInput",
-            widgetId=self.__widget_id,
-            dependencies=self.build_datastore_dependencies(),
-            widgetType=self._build_widget_type(),
-        )
+        return {
+            "widgetId": self.__widget_id,
+            "dependencies": self.build_datastore_dependencies(),
+            "widgetType": self._build_widget_type(),
+        }
 
 
 class _Selected(Selected[AbstractSelectWidget, WidgetField, Widget]):
     """Widget Selected property configuration."""
 
 
 class SelectableWidget(Widget, AbstractSelectWidget):
@@ -248,15 +251,14 @@
         """
         if data is None or data.empty:
             raise WidgetDataNotFoundError(widget_id=self.widget_id)
 
         if field not in data.columns:
             raise WidgetFieldNotFoundError(field=field, columns=list(data.columns))
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Select widget build."""
-        return generate_input(
-            "WidgetInput",
-            widgetId=self.widget_id,
-            dependencies=self.build_datastore_dependencies(),
-            widgetType=self._build_widget_type(),
-        )
+        return {
+            "widgetId": self.widget_id,
+            "dependencies": self.build_datastore_dependencies(),
+            "widgetType": self._build_widget_type(),
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/__init__.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/cartesian/__init__.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/axis/base.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,109 +1,144 @@
-"""Specs for x axis of a Cartesian chart."""
+"""Specs for y axis of a Timeseries chart."""
 
 from abc import abstractmethod
 from typing import Any
+from typing import List
 from typing import Mapping
 from typing import Optional
+from typing import Set
 from typing import Union
 
 import pandas as pd
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import AxisNumberFormatting
-from engineai.sdk.dashboard.links.abstract import AbstractFactoryLinkItemsHandler
-from engineai.sdk.dashboard.links.typing import GenericLink
+from engineai.sdk.dashboard.links import WidgetField
+from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.charts.axis.scale import AxisScale
 from engineai.sdk.dashboard.widgets.components.charts.axis.scale import AxisScaleDynamic
 from engineai.sdk.dashboard.widgets.components.charts.axis.scale import build_axis_scale
+from engineai.sdk.dashboard.widgets.components.charts.exceptions import (
+    ChartSeriesNameAlreadyExistsError,
+)
 
+from ...exceptions import TimeseriesAxisEmptyDefinitionError
+from ...series.typing import TimeseriesSeries
+from ..base import TimeseriesBaseAxis
 
-class CartesianBaseAxis(AbstractFactoryLinkItemsHandler):
-    """Specs for X Axis of a Cartesian chart."""
 
-    _API_TYPE: Optional[str] = None
+class BaseTimeseriesYAxis(TimeseriesBaseAxis):
+    """Specs for y axis of a Timeseries chart."""
 
     @type_check
     def __init__(
         self,
         *,
-        title: Union[str, GenericLink] = "",
-        enable_crosshair: bool = False,
         formatting: Optional[AxisNumberFormatting] = None,
+        title: Union[str, WidgetField] = "",
+        enable_crosshair: bool = False,
         scale: Optional[AxisScale] = None,
     ):
-        """Construct x axis for a Cartesian chart.
+        """Construct y axis for a Timeseries chart.
 
         Args:
-            title: axis title.
-            enable_crosshair: whether to enable crosshair that follows either
+            formatting (Optional[AxisNumberFormatting]): formatting spec for axis
+                labels.
+                Defaults to None.
+            title (Union[str, WidgetField]): axis title.
+                Defaults to empty string.
+            enable_crosshair (bool): whether to enable crosshair that follows either
                 the mouse pointer or the hovered point.
-            formatting: formatting spec for axis labels.
-            scale: y axis scale, one of AxisSymmetricScale, AxisDynamicScale,
-                AxisPositiveScale, AxisNegativeScale.
+                Defaults to False.
+            scale (Optional[YAxisScale]): y axis scale, one of
+                AxisScaleSymmetric, AxisScaleDynamic,
+                AxisScalePositive, AxisScaleNegative.
+                Defaults to AxisScaleSymmetric.
         """
-        super().__init__()
-        self.__title = title
+        super().__init__(enable_crosshair=enable_crosshair)
 
-        self.__formatting = formatting or AxisNumberFormatting()
-
-        self.__enable_crosshair = enable_crosshair
-        self.__scale = scale or AxisScaleDynamic()
+        self.__formatting = (
+            formatting if formatting is not None else AxisNumberFormatting()
+        )
 
-    @property
-    def _api_type(self) -> str:
-        """Returns API type argument value.
+        self.__title = title
+        self.__scale = scale if scale else AxisScaleDynamic()
 
-        All Cartesian Axis must now have the _API_TYPE defined.
-        """
-        if self._API_TYPE is None:
-            raise NotImplementedError(
-                f"Class {self.__class__.__name__}._API_TYPE not defined."
-            )
-        return self._API_TYPE
+        # used for getting a color from the index of each bands
+        self.__series_names: Set[str] = set()
 
     def validate(
         self,
         *,
         data: pd.DataFrame,
     ) -> None:
         """Validate if dataframe has the required columns and dependencies for axis.
 
         Args:
-            data: pandas dataframe which will be used for table.
+            data (pd.DataFrame): pandas dataframe which will be used for table.
 
         Raises:
-            CartesianValidateSeriesDataColumnNotFound: when data is not found
+            ChartDependencyNotFoundError: when `datastore_id` does not exists on
+                current datastores
         """
-        self._axis_validate(data=data)
+        self._validate_series(
+            data=data,
+        )
         self.__formatting.validate(data=data)
 
     @abstractmethod
-    def _axis_validate(
+    def _validate_series(
         self,
         *,
         data: pd.DataFrame,
     ) -> None:
-        """Validate Cartesian Axis."""
+        """Validate timeseries y axis series."""
 
-    def _build_extra_axis(self) -> Mapping[str, Any]:
-        """Method that generates the input for axis extra attribute."""
-        return {}
-
-    def build(self) -> Any:
-        """Method implemented by all factories to generate Input spec.
+    def _add_series(
+        self, current_series: List[TimeseriesSeries], *series: TimeseriesSeries
+    ) -> "BaseTimeseriesYAxis":
+        """Auxiliary method to add series to top y axis.
 
         Returns:
-            Input object for Dashboard API.
+            YAxis: reference to this axis to facilitate inline manipulation.
+
+        Raises:
+            TimeseriesAxisEmptyDefinitionError: when no series data are added
+            ChartSeriesNameAlreadyExistsError: when series have duplicated names
         """
-        return generate_input(
-            self._api_type,
-            enableCrosshair=self.__enable_crosshair,
-            title=build_templated_strings(items=self.__title),
-            scale=build_axis_scale(scale=self.__scale),
-            formatting=self.__formatting.build(),
-            bands=[],
-            lines=[],
-            **self._build_extra_axis(),
-        )
+        if len(series) == 0:
+            raise TimeseriesAxisEmptyDefinitionError()
+
+        for element in series:
+            if element.name in current_series:
+                raise ChartSeriesNameAlreadyExistsError(
+                    class_name=self.__class__.__name__,
+                    series_name=element.name,
+                )
+            if isinstance(element.name, str):
+                self.__series_names.add(str(element.name))
+
+        current_series.extend(series)
+
+        return self
+
+    @abstractmethod
+    def prepare(self, date_column: TemplatedStringItem, offset: int = 0) -> None:
+        """Prepare layout for building."""
+
+    @abstractmethod
+    def _build_extra_y_axis(self) -> Mapping[str, Any]:
+        """Method that generates the input for a specific y axis."""
+
+    def _build_axis(self) -> Mapping[str, Any]:
+        """Method that generates the input for a specific axis."""
+        return {
+            "formatting": self.__formatting.build()
+            if self.__formatting is not None
+            else None,
+            "title": build_templated_strings(
+                items=self.__title if self.__title else ""
+            ),
+            "scale": build_axis_scale(scale=self.__scale),
+            **self._build_extra_y_axis(),
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/axis/x_axis.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/cartesian/axis/x_axis.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,16 +15,14 @@
 
 from .base import CartesianBaseAxis
 
 
 class XAxis(CartesianBaseAxis):
     """Specs for X Axis of a Cartesian chart."""
 
-    _API_TYPE = "ContinuousCartesianWidgetXAxisInput"
-
     @type_check
     def __init__(
         self,
         data_column: Union[str, GenericLink],
         *,
         title: Union[str, GenericLink] = "X",
         enable_crosshair: bool = False,
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/axis/y_axis.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/cartesian/axis/y_axis.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,14 @@
 from ..series.typing import CartesianSeries
 from .base import CartesianBaseAxis
 
 
 class YAxis(CartesianBaseAxis):
     """Specs for Y Axis of a Cartesian chart."""
 
-    _API_TYPE = "ContinuousCartesianWidgetYAxisInput"
-
     @type_check
     def __init__(
         self,
         series: YAxisSeries,
         *,
         title: Union[str, WidgetField] = "Y",
         enable_crosshair: bool = False,
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/cartesian.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/cartesian/cartesian.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Spec for Cartesian widget."""
 
 from typing import Any
+from typing import Dict
 from typing import Optional
 from typing import Union
 
 import pandas as pd
 
 from engineai.sdk.dashboard.data import DataSource
 from engineai.sdk.dashboard.data.http import Http
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.cartesian.axis.typing import YAxisSeries
 from engineai.sdk.dashboard.widgets.cartesian.axis.y_axis import YAxis
 from engineai.sdk.dashboard.widgets.components.charts.toolbar import build_chart_toolbar
 
 from ..base import Widget
 from ..base import WidgetTitleType
 from ..utils import build_data
@@ -103,21 +103,22 @@
         """Validates widget spec.
 
         Args:
             data: pandas DataFrame where the data is present.
         """
         self._chart.validate(data=data)
 
-    def _build_widget_input(self) -> Any:
-        return generate_input(
-            "ContinuousCartesianWidgetInput",
-            title=build_templated_strings(items=self._title) if self._title else None,
-            chart=self._chart.build(),
-            legend=self._legend.build(),
-            toolbar=build_chart_toolbar(enable=self._enable_toolbar),
-            data=build_data(self.dependency_id, self._json_data),
-        )
+    def _build_widget_input(self) -> Dict[str, Any]:
+        return {
+            "title": build_templated_strings(items=self._title)
+            if self._title
+            else None,
+            "chart": self._chart.build(),
+            "legend": self._legend.build(),
+            "toolbar": build_chart_toolbar(enable=self._enable_toolbar),
+            "data": build_data(self.dependency_id, self._json_data),
+        }
 
     def _prepare(self, **kwargs: object) -> None:
         """Method that prepares the spec to be built."""
         self._chart.prepare()
         self._json_data = kwargs.get("json_data", None)
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/chart.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/cartesian/chart.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Spec for charts in a Cartesian widget."""
 
 from typing import Any
+from typing import Dict
 from typing import Optional
 from typing import Union
 
 import pandas as pd
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links.abstract import AbstractFactoryLinkItemsHandler
 from engineai.sdk.dashboard.links.typing import GenericLink
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.cartesian.axis.typing import YAxisSeries
 from engineai.sdk.dashboard.widgets.cartesian.exceptions import (
     CartesianMissingChartAxisError,
 )
 
 from .axis.x_axis import XAxis
 from .axis.y_axis import YAxis
@@ -100,30 +100,29 @@
                 data=data,
             )
         if self.__right_y_axis is not None:
             self.__right_y_axis.validate(
                 data=data,
             )
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API.
         """
-        return generate_input(
-            "ContinuousCartesianWidgetChartInput",
-            xAxis=self.__x_axis.build(),
-            yAxisLeft=[self.__left_y_axis.build()]
+        return {
+            "xAxis": self.__x_axis.build(),
+            "yAxisLeft": [self.__left_y_axis.build()]
             if self.__left_y_axis is not None
             else [],
-            yAxisRight=[self.__right_y_axis.build()]
+            "yAxisRight": [self.__right_y_axis.build()]
             if self.__right_y_axis is not None
             else [],
-        )
+        }
 
     def prepare(self) -> None:
         """Method that prepares the spec to be built."""
         if self.__left_y_axis is not None:
             self.__left_y_axis.prepare(self.__x_axis.data_column)
         if self.__right_y_axis is not None:
             self.__right_y_axis.prepare(
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/exceptions.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/cartesian/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/legend.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/maps/legend.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-"""Spec for legend of a categorical widget."""
+"""Spec for legend of a Map Shape widget."""
+
 from typing import Any
+from typing import Dict
 
 from engineai.sdk.dashboard.base import AbstractFactory
 from engineai.sdk.dashboard.decorator import type_check
-from engineai.sdk.dashboard.enum.legend_position import LegendPosition
-from engineai.sdk.dashboard.utils import generate_input
+from engineai.sdk.dashboard.widgets.maps.enums import LegendPosition
 
 
 class Legend(AbstractFactory):
-    """Spec for legend of a categorical widget.
-
-    Args:
-        position: location of position relative to data, charts.
-    """
+    """Spec for legend of a Map widget."""
 
     @type_check
     def __init__(self, *, position: LegendPosition = LegendPosition.BOTTOM):
-        """Construct a legend for a categorical widget."""
+        """Constructor for Legend.
+
+        Args:
+            position (Position): location of position
+                relative to data, maps.
+        """
         super().__init__()
         self.__position = position
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "ContinuousCartesianWidgetLegendInput", position=self.__position.value
-        )
+        return {"position": self.__position.value}
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/series/area.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/cartesian/series/line.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,43 @@
-"""Spec for a Area series of a Cartesian widget."""
+"""Spec for a line series of a Cartesian widget."""
 
 from typing import Optional
 from typing import Union
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import NumberFormatting
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.styling.color import Palette
-from engineai.sdk.dashboard.widgets.components.charts.styling import AreaSeriesStyling
+from engineai.sdk.dashboard.widgets.components.charts.styling import LineSeriesStyling
 from engineai.sdk.dashboard.widgets.components.charts.typing import TooltipItems
 
 from .base import CartesianBaseSeries
 
 
-class AreaSeries(CartesianBaseSeries):
-    """Spec for a Area series of a Cartesian widget."""
+class LineSeries(CartesianBaseSeries):
+    """Spec for a line series of a Cartesian widget."""
 
-    _API_TYPE = "ContinuousCartesianWidgetAreaSeriesInput"
-    _INPUT_KEY = "area"
-    _styling_class = AreaSeriesStyling
+    _INPUT_KEY = "line"
+    _styling_class = LineSeriesStyling
 
     @type_check
     def __init__(
         self,
         *,
         data_column: Union[str, WidgetField],
         formatting: Optional[NumberFormatting] = None,
         name: Optional[Union[str, WidgetField]] = None,
-        styling: Optional[Union[Palette, AreaSeriesStyling]] = None,
+        styling: Optional[Union[Palette, LineSeriesStyling]] = None,
         show_in_legend: bool = True,
         required: bool = True,
         visible: bool = True,
         point_label_column: Optional[Union[str, WidgetField]] = None,
         tooltips: Optional[TooltipItems] = None,
     ):
-        """Construct area series.
+        """Construct line series.
 
         Args:
             data_column: name of column in pandas dataframe(s) used for the values of
                 this series for the Y Axis.
             formatting: formatting spec for value associated with Y Axis.
             name: series name (shown in legend and tooltip).
             styling: styling spec.
@@ -58,11 +57,11 @@
             show_in_legend=show_in_legend,
             required=required,
             visible=visible,
             point_label_column=point_label_column,
             tooltips=tooltips,
         )
         self._styling = (
-            AreaSeriesStyling(color_spec=styling)
+            LineSeriesStyling(color_spec=styling)
             if isinstance(styling, Palette)
             else styling
         )
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/series/area_range.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/cartesian/series/area_range.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 from .base import CartesianBaseSeries
 
 
 class AreaRangeSeries(CartesianBaseSeries):
     """Spec for a area range series of a Cartesian widget."""
 
-    _API_TYPE = "ContinuousCartesianWidgetAreaRangeSeriesInput"
     _INPUT_KEY = "areaRange"
     _styling_class = AreaRangeSeriesStyling
 
     @type_check
     def __init__(
         self,
         *,
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/series/base.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/cartesian/series/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import NumberFormatting
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.styling.color.palette import qualitative_palette
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.charts.series.base import ChartSeriesBase
 from engineai.sdk.dashboard.widgets.components.charts.styling.typing import (
     ColoredSeriesStyling,
 )
 from engineai.sdk.dashboard.widgets.components.charts.tooltip.item import (
     build_tooltip_item,
 )
@@ -119,20 +118,19 @@
         """Prepare series to be rendered."""
         self._x_column = x_column
         if self._styling is None:
             self.__set_default_styling(color=qualitative_palette(index=index))
         else:
             self._styling.prepare(self._data_column)
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Build Input spec for Dashboard API."""
-        return generate_input(
-            "ContinuousCartesianWidgetSeriesInput",
+        return {
             **{self._input_key: self._build_series()},
-        )
+        }
 
     def _build_extra_inputs(self) -> Dict[str, Any]:
         return {}
 
     def _validate_data_column(
         self,
         *,
@@ -144,39 +142,43 @@
             if data_column not in data.columns:
                 raise CartesianValidateDataColumnNotFound(
                     class_name=self.__class__.__name__,
                     column_name=data_column_name,
                     column_value=data_column,
                 )
 
-    def _build_series(self) -> Any:
+    def _build_series(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            self._api_type,
-            name=build_templated_strings(items=self.name),
-            xAxisKey=build_templated_strings(items=self._x_column),
-            xValueFormatting=NumberFormatting().build(),
-            showInLegend=self._show_in_legend,
-            required=self._required,
-            isVisible=self._visible,
-            tooltipItems=[
+        return {
+            "name": build_templated_strings(items=self.name),
+            "xAxisKey": build_templated_strings(items=self._x_column),
+            "xValueFormatting": NumberFormatting().build(),
+            "showInLegend": self._show_in_legend,
+            "required": self._required,
+            "isVisible": self._visible,
+            "tooltipItems": [
                 build_tooltip_item(item=item) for item in self._tooltip_items
             ],
-            styling=self._styling.build() if self._styling else None,
-            **{"yAxisKey": build_templated_strings(items=self._data_column)}
-            if self._data_column is not None
-            else {},
-            pointLabelKey=build_templated_strings(items=self._point_label_column)
+            "styling": self._styling.build() if self._styling else None,
+            "pointLabelKey": build_templated_strings(items=self._point_label_column)
             if self._point_label_column
             else None,
             **self._build_extra_inputs(),
+            **self._build_y_axis_key(),
+        }
+
+    def _build_y_axis_key(self) -> Dict[str, Any]:
+        return (
+            {"yAxisKey": build_templated_strings(items=self._data_column)}
+            if self._data_column is not None
+            else {}
         )
 
     def __set_default_styling(self, color: ColorSpec) -> None:
         if self._styling_class is None:
             raise NotImplementedError(
                 f"Class {self.__class__.__name__} does not have the variable "
                 f"`_styling_class` initialized."
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/series/bubble.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/cartesian/series/bubble.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Spec for a bubble series of a Cartesian widget."""
 
 from typing import Any
+from typing import Dict
 from typing import Optional
 from typing import Union
 
 import pandas as pd
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import NumberFormatting
@@ -32,15 +33,14 @@
     BubbleCountrySeriesStyling,
 ]
 
 
 class BubbleSeries(CartesianBaseSeries):
     """Spec for a bubble series of a Cartesian widget."""
 
-    _API_TYPE = "ContinuousCartesianWidgetBubbleSeriesInput"
     _INPUT_KEY = "bubble"
     _styling_class = BubbleCircleSeriesStyling
 
     @type_check
     def __init__(
         self,
         *,
@@ -120,15 +120,15 @@
             data_column_name="bubble_size_column",
         )
         self._bubble_size_formatting.validate(data=data)
 
         if self._entity is not None and isinstance(self._entity, CountryEntity):
             self._entity.validate_data_column(data=data)
 
-    def _build_extra_inputs(self) -> Any:
+    def _build_extra_inputs(self) -> Dict[str, Any]:
         return {
             "zValueKey": build_templated_strings(items=self._bubble_size_column)
             if self._bubble_size_column
             else {},
             "zValueTitle": build_templated_strings(items=self._bubble_name_column)
             if self._bubble_name_column
             else {},
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/series/column.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/cartesian/series/column.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 from .base import CartesianBaseSeries
 
 
 class ColumnSeries(CartesianBaseSeries):
     """Spec for a column series of a Cartesian widget."""
 
-    _API_TYPE = "ContinuousCartesianWidgetColumnSeriesInput"
     _INPUT_KEY = "column"
     _styling_class = ColumnSeriesStyling
 
     @type_check
     def __init__(
         self,
         *,
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/series/line.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/cartesian/series/scatter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,45 @@
-"""Spec for a line series of a Cartesian widget."""
+"""Spec for a scatter series of a Cartesian widget."""
 
 from typing import Optional
 from typing import Union
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import NumberFormatting
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.styling.color import Palette
-from engineai.sdk.dashboard.widgets.components.charts.styling import LineSeriesStyling
+from engineai.sdk.dashboard.widgets.components.charts.styling import (
+    ScatterSeriesStyling,
+)
 from engineai.sdk.dashboard.widgets.components.charts.typing import TooltipItems
 
 from .base import CartesianBaseSeries
 
 
-class LineSeries(CartesianBaseSeries):
-    """Spec for a line series of a Cartesian widget."""
+class ScatterSeries(CartesianBaseSeries):
+    """Spec for a scatter series of a Cartesian widget."""
 
-    _API_TYPE = "ContinuousCartesianWidgetLineSeriesInput"
-    _INPUT_KEY = "line"
-    _styling_class = LineSeriesStyling
+    _INPUT_KEY = "scatter"
+    _styling_class = ScatterSeriesStyling
 
     @type_check
     def __init__(
         self,
         *,
         data_column: Union[str, WidgetField],
         formatting: Optional[NumberFormatting] = None,
         name: Optional[Union[str, WidgetField]] = None,
-        styling: Optional[Union[Palette, LineSeriesStyling]] = None,
+        styling: Optional[Union[Palette, ScatterSeriesStyling]] = None,
         show_in_legend: bool = True,
         required: bool = True,
         visible: bool = True,
         point_label_column: Optional[Union[str, WidgetField]] = None,
         tooltips: Optional[TooltipItems] = None,
     ):
-        """Construct line series.
+        """Construct scatter series.
 
         Args:
             data_column: name of column in pandas dataframe(s) used for the values of
                 this series for the Y Axis.
             formatting: formatting spec for value associated with Y Axis.
             name: series name (shown in legend and tooltip).
             styling: styling spec.
@@ -58,11 +59,11 @@
             show_in_legend=show_in_legend,
             required=required,
             visible=visible,
             point_label_column=point_label_column,
             tooltips=tooltips,
         )
         self._styling = (
-            LineSeriesStyling(color_spec=styling)
+            ScatterSeriesStyling(color_spec=styling)
             if isinstance(styling, Palette)
             else styling
         )
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/series/scatter.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/cartesian/series/area.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,43 @@
-"""Spec for a scatter series of a Cartesian widget."""
+"""Spec for a Area series of a Cartesian widget."""
 
 from typing import Optional
 from typing import Union
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import NumberFormatting
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.styling.color import Palette
-from engineai.sdk.dashboard.widgets.components.charts.styling import (
-    ScatterSeriesStyling,
-)
+from engineai.sdk.dashboard.widgets.components.charts.styling import AreaSeriesStyling
 from engineai.sdk.dashboard.widgets.components.charts.typing import TooltipItems
 
 from .base import CartesianBaseSeries
 
 
-class ScatterSeries(CartesianBaseSeries):
-    """Spec for a scatter series of a Cartesian widget."""
+class AreaSeries(CartesianBaseSeries):
+    """Spec for a Area series of a Cartesian widget."""
 
-    _API_TYPE = "ContinuousCartesianWidgetScatterSeriesInput"
-    _INPUT_KEY = "scatter"
-    _styling_class = ScatterSeriesStyling
+    _INPUT_KEY = "area"
+    _styling_class = AreaSeriesStyling
 
     @type_check
     def __init__(
         self,
         *,
         data_column: Union[str, WidgetField],
         formatting: Optional[NumberFormatting] = None,
         name: Optional[Union[str, WidgetField]] = None,
-        styling: Optional[Union[Palette, ScatterSeriesStyling]] = None,
+        styling: Optional[Union[Palette, AreaSeriesStyling]] = None,
         show_in_legend: bool = True,
         required: bool = True,
         visible: bool = True,
         point_label_column: Optional[Union[str, WidgetField]] = None,
         tooltips: Optional[TooltipItems] = None,
     ):
-        """Construct scatter series.
+        """Construct area series.
 
         Args:
             data_column: name of column in pandas dataframe(s) used for the values of
                 this series for the Y Axis.
             formatting: formatting spec for value associated with Y Axis.
             name: series name (shown in legend and tooltip).
             styling: styling spec.
@@ -60,11 +57,11 @@
             show_in_legend=show_in_legend,
             required=required,
             visible=visible,
             point_label_column=point_label_column,
             tooltips=tooltips,
         )
         self._styling = (
-            ScatterSeriesStyling(color_spec=styling)
+            AreaSeriesStyling(color_spec=styling)
             if isinstance(styling, Palette)
             else styling
         )
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/series/typing.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/cartesian/series/typing.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/chart_utils.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/chart_utils.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/actions/links/base.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/actions/links/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,13 +72,13 @@
                 data=data,
                 column_name=data_column,
                 node=key,
                 warning_flags=warnings_flag,
             )
 
     @abstractmethod
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/actions/links/exceptions.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/actions/links/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/actions/links/url_link.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/actions/links/url_link.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Spec for Url Link."""
 
 from typing import Any
+from typing import Dict
 from typing import Iterable
 from typing import List
 from typing import Optional
 from typing import Union
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.templated_string import DataField
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.actions.links.base import BaseLink
 
 
 class UrlLink(BaseLink):
     """Spec for Url Link."""
 
     @type_check
@@ -32,29 +32,28 @@
                 tooltip spec.
         """
         super().__init__(
             data_column=data_column,
             tooltip=tooltip,
         )
 
-    def _build_tooltip(self) -> Any:
+    def _build_tooltip(self) -> Dict[str, Any]:
         build_tooltip = self._tooltip.build() if self._tooltip else None
         if self._tooltip and isinstance(build_tooltip, Iterable):
             tooltip = build_tooltip
         elif self._tooltip:
             tooltip = [build_tooltip]
         else:
             tooltip = []
         return tooltip
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "ActionHyperLinkInput",
-            urlKey=build_templated_strings(items=self._data_column),
-            tooltip=self._build_tooltip(),
-            params=[],
-        )
+        return {
+            "urlKey": build_templated_strings(items=self._data_column),
+            "tooltip": self._build_tooltip(),
+            "params": [],
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/axis/scale/dynamic.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/axis/scale/dynamic.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Spec for dynamic scale for y axis."""
 
 from typing import Any
+from typing import Dict
 
 from engineai.sdk.dashboard.base import AbstractFactory
 from engineai.sdk.dashboard.decorator import type_check
-from engineai.sdk.dashboard.utils import generate_input
 
 
 class AxisScaleDynamic(AbstractFactory):
     """Dynamically set y-axis extremes for optimal spacing.
 
     Construct specifications for a dynamic scale for the y-axis of a chart.
     By default, it dynamically calculates axis extremes to minimize
@@ -21,16 +21,14 @@
 
         Args:
             tick_amount: number of ticks beyond min and max.
         """
         super().__init__()
         self.__tick_amount = tick_amount
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "ChartNumericAxisScaleDynamicInput", tickAmount=self.__tick_amount
-        )
+        return {"tickAmount": self.__tick_amount}
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/axis/scale/negative.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/axis/scale/negative.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Spec for scale for y axis with only negative values."""
 
 from typing import Any
+from typing import Dict
 from typing import Optional
 
 from engineai.sdk.dashboard.base import AbstractFactory
 from engineai.sdk.dashboard.decorator import type_check
-from engineai.sdk.dashboard.utils import generate_input
 
 
 class AxisScaleNegative(AbstractFactory):
     """Y-axis scale for charts with negative values.
 
     Construct specifications for a scale for the y-axis with only
     negative values. It assumes the maximum value of the chart to
@@ -29,26 +29,24 @@
                 Defaults to None (min value calculated dynamically)
             intermediate_tick_amount: number of extra ticks between extremes.
         """
         super().__init__()
         self.__min_value = min_value
         self.__intermediate_tick_amount = intermediate_tick_amount
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "ChartNumericAxisScaleNegativeInput",
-            min=self.__build_min_value(),
-            tickAmount=self.__intermediate_tick_amount,
-        )
+        return {
+            "min": self.__build_min_value(),
+            "tickAmount": self.__intermediate_tick_amount,
+        }
 
     def __build_min_value(
         self,
-    ) -> Any:
-        return generate_input(
-            "ChartNumericAxisScaleMinInput",
-            min=self.__min_value,
-        )
+    ) -> Dict[str, Any]:
+        return {
+            "min": self.__min_value,
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/axis/scale/positive.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/axis/scale/positive.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Spec for scale for y axis with only positive values."""
 
 from typing import Any
+from typing import Dict
 from typing import Optional
 
 from engineai.sdk.dashboard.base import AbstractFactory
 from engineai.sdk.dashboard.decorator import type_check
-from engineai.sdk.dashboard.utils import generate_input
 
 
 class AxisScalePositive(AbstractFactory):
     """Y-axis scale for charts with positive values.
 
     Construct specifications for a scale for the y-axis with only
     positive values. It assumes the minimum value of the chart to be
@@ -29,26 +29,24 @@
                 Defaults to None (max value calculated dynamically)
             intermediate_tick_amount: number of extra ticks between extremes.
         """
         super().__init__()
         self.__max_value = max_value
         self.__intermediate_tick_amount = intermediate_tick_amount
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "ChartNumericAxisScalePositiveInput",
-            max=self.__build_max_value(),
-            tickAmount=self.__intermediate_tick_amount,
-        )
+        return {
+            "max": self.__build_max_value(),
+            "tickAmount": self.__intermediate_tick_amount,
+        }
 
     def __build_max_value(
         self,
-    ) -> Any:
-        return generate_input(
-            "ChartNumericAxisScaleMaxInput",
-            max=self.__max_value,
-        )
+    ) -> Dict[str, Any]:
+        return {
+            "max": self.__max_value,
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/axis/scale/scale.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/axis/scale/scale.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 """Spec to build different scales supported by y axis."""
 
 from typing import Any
-
-from engineai.sdk.dashboard.utils import generate_input
+from typing import Dict
 
 from .dynamic import AxisScaleDynamic
 from .negative import AxisScaleNegative
 from .positive import AxisScalePositive
 from .symmetric import AxisScaleSymmetric
 from .typing import AxisScale
 
 
-def build_axis_scale(scale: AxisScale) -> Any:
+def build_axis_scale(scale: AxisScale) -> Dict[str, Any]:
     """Builds spec for dashboard API.
 
     Returns:
         Input object for Dashboard API
     """
-    return generate_input(
-        "ChartNumericAxisScaleInput", **{_get_input_key(scale): scale.build()}
-    )
+    return {**{_get_input_key(scale): scale.build()}}
 
 
 def _get_input_key(scale: AxisScale) -> str:
     if isinstance(scale, AxisScaleDynamic):
         return "dynamic"
     elif isinstance(scale, AxisScaleSymmetric):
         return "symmetrical"
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/axis/scale/symmetric.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/axis/scale/symmetric.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Spec for scale for y axis with only positive and negative values."""
 
 from typing import Any
+from typing import Dict
 from typing import Optional
 
 from engineai.sdk.dashboard.base import AbstractFactory
 from engineai.sdk.dashboard.decorator import type_check
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.charts.exceptions import (
     ChartScaleSymmetricValueError,
 )
 
 
 class AxisScaleSymmetric(AbstractFactory):
     """Y-axis scale for charts with positive and negative values.
@@ -45,36 +45,33 @@
         if min_value is not None and max_value is not None and strict is not None:
             raise ChartScaleSymmetricValueError(class_name=self.__class__.__name__)
         self.__min_value = min_value
         self.__max_value = max_value
         self.__intermediate_tick_amount = intermediate_tick_amount
         self.__strict = strict
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "ChartNumericAxisScaleSymmetricalInput",
-            min=self.__build_min_value(),
-            max=self.__build_max_value(),
-            intermediateTickAmount=self.__intermediate_tick_amount,
-            strict=self.__strict if self.__strict is not None else True,
-        )
+        return {
+            "min": self.__build_min_value(),
+            "max": self.__build_max_value(),
+            "intermediateTickAmount": self.__intermediate_tick_amount,
+            "strict": self.__strict if self.__strict is not None else True,
+        }
 
     def __build_min_value(
         self,
-    ) -> Any:
-        return generate_input(
-            "ChartNumericAxisScaleMinInput",
-            min=self.__min_value,
-        )
+    ) -> Dict[str, Any]:
+        return {
+            "min": self.__min_value,
+        }
 
     def __build_max_value(
         self,
-    ) -> Any:
-        return generate_input(
-            "ChartNumericAxisScaleMaxInput",
-            max=self.__max_value,
-        )
+    ) -> Dict[str, Any]:
+        return {
+            "max": self.__max_value,
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/exceptions.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/series/base.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/series/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 from ..exceptions import SeriesMissingLabelError
 from ..exceptions import SeriesUnsupportedDataColumnError
 
 
 class ChartSeriesBase(AbstractFactoryLinkItemsHandler):
     """Chart Base Series class."""
 
-    _API_TYPE: Optional[str] = None
-
     def __init__(
         self,
         name: Optional[Union[str, GenericLink]] = None,
         data_column: Optional[Union[str, GenericLink]] = None,
     ) -> None:
         """Constructor for Chart Base Series class.
 
@@ -33,24 +31,14 @@
             data_column (Optional[Union[str, WidgetField]]): column
                 in dataframe(s) that will be transformed to be series name.
         """
         super().__init__()
         self.__name = self._set_name(name=name, data_column=data_column)
 
     @property
-    def _api_type(self) -> str:
-        if self._API_TYPE is None:
-            raise NotImplementedError(
-                f"Class {self.__class__.__name__} does not have the variable "
-                f"`_API_TYPE` initialized. Please add the proper value or overwrite "
-                f"this method {self.__class__.__name__}._api_type."
-            )
-        return self._API_TYPE
-
-    @property
     def name(self) -> Union[str, GenericLink]:
         """Returns name of series.
 
         Returns:
             Union[str, WidgetField]: name
         """
         return self.__name
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/series/entities/base.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/series/entities/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Chart Series Entities base."""
 from abc import abstractmethod
 from typing import Any
+from typing import Dict
 from typing import Optional
 
 from engineai.sdk.dashboard.links.abstract import AbstractFactoryLinkItemsHandler
-from engineai.sdk.dashboard.utils import generate_input
 
 
 class Entity(AbstractFactoryLinkItemsHandler):
     """Chart Series Entities base spec."""
 
     _INPUT_KEY: Optional[str] = None
 
@@ -18,16 +18,15 @@
         if self._INPUT_KEY is None:
             raise NotImplementedError(
                 f"Class {self.__class__.__name__}._INPUT_KEY not defined."
             )
         return self._INPUT_KEY
 
     @abstractmethod
-    def _build_entity(self) -> Any:
+    def _build_entity(self) -> Dict[str, Any]:
         pass
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Build entities Input spec."""
-        return generate_input(
-            "ChartSeriesEntityUnionInput",
+        return {
             **{self._input_key: self._build_entity()},
-        )
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/series/entities/country.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/series/entities/country.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Chart Series Country Entity."""
 import pandas as pd
 
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.charts.exceptions import (
     ChartSeriesEntityInvalidCountryCodeError,
 )
 from engineai.sdk.dashboard.widgets.components.charts.exceptions import (
     ChartSeriesEntityNoDataColumnError,
 )
 from engineai.sdk.dashboard.widgets.components.charts.series.entities.base import Entity
@@ -55,12 +54,11 @@
             and self.__country_code not in COUNTRY_CODES
         ):
             raise ChartSeriesEntityInvalidCountryCodeError(
                 self.__class__.__name__, self.__country_code
             )
 
     def _build_entity(self):
-        return generate_input(
-            "ChartSeriesCountryEntityInput",
-            countryCodeKey=build_templated_strings(items=self.__country_code),
-            showFlag=self.__flag,
-        )
+        return {
+            "countryCodeKey": build_templated_strings(items=self.__country_code),
+            "showFlag": self.__flag,
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/series/entities/custom.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/series/entities/custom.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Chart Series Custom Entity."""
 
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.charts.series.entities.base import Entity
 
 
 class CustomEntity(Entity):
     """Custom entity spec."""
 
     _INPUT_KEY = "standard"
@@ -17,11 +16,10 @@
         Args:
             name: name for custom entity.
         """
         super().__init__()
         self.__name = name
 
     def _build_entity(self):
-        return generate_input(
-            "ChartSeriesStandardEntityInput",
-            name=build_templated_strings(items=self.__name),
-        )
+        return {
+            "name": build_templated_strings(items=self.__name),
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/__init__.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/styling/__init__.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/area.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/styling/error_bar.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,42 @@
-"""Spec to style an area series."""
+"""Spec to style a column series."""
 from typing import Optional
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
 from .base import BaseChartSeriesStyling
 from .enums import MarkerSymbol
 
 
-class AreaSeriesStyling(BaseChartSeriesStyling):
-    """Customize appearance of filled areas in Charts.
+class ErrorBarSeriesStyling(BaseChartSeriesStyling):
+    """Customize appearance of error bars in Chart.
 
-    Specify styling options for an area series within a Chart
-    widget to customize the appearance of filled areas on the chart.
+    Specify styling options for an error bar series within a
+    Chart widget to customize the appearance of error bars
+    representing data variability or uncertainty on the chart.
     """
 
-    _API_TYPE = "ChartAreaSeriesStylingInput"
-
     @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_column: Optional[TemplatedStringItem] = None,
-        marker_symbol: MarkerSymbol = MarkerSymbol.CIRCLE,
+        marker_symbol: MarkerSymbol = MarkerSymbol.SQUARE,
     ):
-        """Constructor for AreaSeriesStyling.
+        """Constructor for ErrorBarSeriesStyling.
 
         Args:
-            color_spec: spec for coloring area.
+            color_spec: spec for coloring columns.
             data_column: name of column in pandas dataframe(s) used for color spec if
                 a gradient is used. Optional for single colors.
             marker_symbol: symbol for marker in tooltips and legends.
 
         Raises:
-            ChartStylingMissingDataColumnError: if color_spec is
-                ColorDiscreteMap/ColorGradient and data_column
-                has not been specified
+            ChartStylingMissingDataColumnError: if a data_column is not defined when
+                color_spec is a ColorDiscreteMap or ColorGradient
         """
         super().__init__(
             color_spec=color_spec, data_column=data_column, marker_symbol=marker_symbol
         )
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/area_range.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/styling/area_range.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,14 @@
     """Customize appearance of filled areas between values.
 
     Specify styling specifications for an area range series within a
     Timeseries widget to customize the appearance of filled areas
     between low and high values on the chart.
     """
 
-    _API_TYPE = "ChartAreaRangeSeriesStylingInput"
-
     @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_column: Optional[TemplatedStringItem] = None,
         marker_symbol: MarkerSymbol = MarkerSymbol.CIRCLE,
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/base.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/styling/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,26 +11,23 @@
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.styling.color import DiscreteMap
 from engineai.sdk.dashboard.styling.color import Gradient
 from engineai.sdk.dashboard.styling.color.spec import build_color_spec
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 
 from ..exceptions import ChartStylingMissingDataColumnError
 from ..exceptions import ChartStylingNoDataColumnError
 from .enums import MarkerSymbol
 
 
 class BaseChartSeriesStyling(AbstractFactory):
     """Spec base for style a chart series."""
 
-    _API_TYPE: Optional[str] = None
-
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_column: Optional[TemplatedStringItem] = None,
         marker_symbol: Optional[MarkerSymbol] = None,
     ):
@@ -43,25 +40,14 @@
             marker_symbol: symbol for marker in tooltips and legends.
         """
         super().__init__()
         self.__color_spec = color_spec
         self.__data_column = data_column
         self.__marker_symbol = marker_symbol
 
-    @property
-    def _api_type(self) -> str:
-        """Returns API Type."""
-        if self._API_TYPE is None:
-            raise NotImplementedError(
-                f"Class {self.__class__.__name__} does not have the variable "
-                f"`_API_TYPE` initialized. Please add the proper value or overwrite "
-                f"this method {self.__class__.__name__}.api_type."
-            )
-        return self._API_TYPE
-
     def prepare(
         self, data_column: Optional[Union[str, TemplatedStringItem, GenericLink]]
     ) -> None:
         """Prepare data column."""
         if (
             isinstance(self.__color_spec, (DiscreteMap, Gradient))
             and self.__data_column is None
@@ -95,25 +81,24 @@
             )
 
     def _build_extra_fields(
         self,
     ) -> Dict[str, Any]:
         return {}
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
         if self.__marker_symbol is not None:
             maker_symbol = {"markerSymbol": self.__marker_symbol.value}
         else:
             maker_symbol = {}
 
-        return generate_input(
-            self._api_type,
-            colorSpec=build_color_spec(spec=self.__color_spec),
-            valueKey=build_templated_strings(items=self.__data_column),
+        return {
+            "colorSpec": build_color_spec(spec=self.__color_spec),
+            "valueKey": build_templated_strings(items=self.__data_column),
             **maker_symbol,
             **self._build_extra_fields(),
-        )
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/bubble_circle.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/styling/bubble_circle.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,29 +7,26 @@
 
 import pandas as pd
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 
 from ..exceptions import ChartStylingNoDataColumnError
 from .base import BaseChartSeriesStyling
 
 
 class BubbleCircleSeriesStyling(BaseChartSeriesStyling):
     """Customize appearance of bubble markers.
 
     Specify styling options for a bubble circle series within a Chart
     widget to customize the appearance of bubble markers on the chart.
     """
 
-    _API_TYPE = "ChartBubbleSeriesStylingCircleInput"
-
     @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_column: Optional[TemplatedStringItem] = None,
         label_column: Optional[TemplatedStringItem] = None,
@@ -82,14 +79,14 @@
     def _build_extra_fields(self) -> Dict[str, Any]:
         return {
             "maxSizePercentage": self.__max_size_percentage,
             "minSizePercentage": self.__min_size_percentage,
             "labelKey": build_templated_strings(items=self.__label_column),
         }
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input("ChartBubbleSeriesStylingInput", circle=super().build())
+        return {"circle": super().build()}
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/bubble_country.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/styling/bubble_country.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Spec to style a bubble series using country flags."""
 
 from typing import Any
+from typing import Dict
 from typing import Optional
 from typing import Union
 
 import pandas as pd
 
 from engineai.sdk.dashboard.base import AbstractFactory
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.charts.exceptions import (
     ChartStylingNoDataColumnError,
 )
 
 
 class BubbleCountrySeriesStyling(AbstractFactory):
     """Customize appearance of country bubble markers.
@@ -64,27 +64,25 @@
             and self.__country_column not in data.columns
         ):
             raise ChartStylingNoDataColumnError(
                 class_name=self.__class__.__name__,
                 data_column=self.__country_column,
             )
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "ChartBubbleSeriesStylingInput",
-            country=generate_input(
-                "ChartBubbleSeriesStylingCountryInput",
-                countryKey=build_templated_strings(items=self.__country_column),
-                maxSizePercentage=self.__max_size_percentage,
-                minSizePercentage=self.__min_size_percentage,
-            ),
-        )
+        return {
+            "country": {
+                "countryKey": build_templated_strings(items=self.__country_column),
+                "maxSizePercentage": self.__max_size_percentage,
+                "minSizePercentage": self.__min_size_percentage,
+            }
+        }
 
     def prepare(
         self, data_column: Optional[Union[str, TemplatedStringItem, GenericLink]]
     ) -> None:
         """Prepare data column."""
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/column.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/styling/column.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 class ColumnSeriesStyling(BaseChartSeriesStyling):
     """Customize appearance of vertical columns.
 
     Specify styling options for a column series within a
     Chart widget to customize the appearance of vertical columns on the chart.
     """
 
-    _API_TYPE = "ChartColumnSeriesStylingInput"
-
     @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_column: Optional[TemplatedStringItem] = None,
         marker_symbol: MarkerSymbol = MarkerSymbol.SQUARE,
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/enums.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/styling/enums.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/error_bar.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/styling/scatter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,41 @@
-"""Spec to style a column series."""
+"""Spec to style a scatter series."""
 from typing import Optional
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
 from .base import BaseChartSeriesStyling
 from .enums import MarkerSymbol
 
 
-class ErrorBarSeriesStyling(BaseChartSeriesStyling):
-    """Customize appearance of error bars in Chart.
+class ScatterSeriesStyling(BaseChartSeriesStyling):
+    """Customize appearance of scatter markers.
 
-    Specify styling options for an error bar series within a
-    Chart widget to customize the appearance of error bars
-    representing data variability or uncertainty on the chart.
+    Specify styling options for a scatter series within a Timeseries
+    widget to customize the appearance of individual data points
+    represented as scatter markers on the chart.
     """
 
-    _API_TYPE = "ChartErrorBarSeriesStylingInput"
-
     @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_column: Optional[TemplatedStringItem] = None,
-        marker_symbol: MarkerSymbol = MarkerSymbol.SQUARE,
+        marker_symbol: MarkerSymbol = MarkerSymbol.CIRCLE,
     ):
-        """Constructor for ErrorBarSeriesStyling.
+        """Constructor for ScatterSeriesStyling.
 
         Args:
             color_spec: spec for coloring columns.
             data_column: name of column in pandas dataframe(s) used for color spec if
                 a gradient is used. Optional for single colors.
-            marker_symbol: symbol for marker in tooltips and legends.
+            marker_symbol: symbol for each point.
 
         Raises:
             ChartStylingMissingDataColumnError: if a data_column is not defined when
                 color_spec is a ColorDiscreteMap or ColorGradient
         """
         super().__init__(
             color_spec=color_spec, data_column=data_column, marker_symbol=marker_symbol
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/line.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/styling/line.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,14 @@
 class LineSeriesStyling(BaseChartSeriesStyling):
     """Customize appearance of lines in Chart.
 
     Specify styling options for a line series within a Chart widget
     to customize the appearance of the lines connecting data points on the chart.
     """
 
-    _API_TYPE = "ChartLineSeriesStylingInput"
-
     @type_check
     def __init__(
         self,
         *,
         color_spec: Optional[ColorSpec] = None,
         data_column: Optional[TemplatedStringItem] = None,
         dash_style: Union[DashStyle, TemplatedStringItem] = DashStyle.SOLID,
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/point.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/styling/area.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,42 @@
-"""Spec to style a point series."""
+"""Spec to style an area series."""
 from typing import Optional
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
 from .base import BaseChartSeriesStyling
 from .enums import MarkerSymbol
 
 
-class PointSeriesStyling(BaseChartSeriesStyling):
-    """Customize appearance of data points in Chart.
+class AreaSeriesStyling(BaseChartSeriesStyling):
+    """Customize appearance of filled areas in Charts.
 
-    Specify styling options for a point series within a Chart
-    widget to customize the appearance of individual
-    data points on the chart.
+    Specify styling options for an area series within a Chart
+    widget to customize the appearance of filled areas on the chart.
     """
 
-    _API_TYPE = "ChartPointSeriesStylingInput"
-
     @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_column: Optional[TemplatedStringItem] = None,
         marker_symbol: MarkerSymbol = MarkerSymbol.CIRCLE,
     ):
-        """Constructor for PointSeriesStyling.
+        """Constructor for AreaSeriesStyling.
 
         Args:
-            color_spec: spec for coloring columns.
+            color_spec: spec for coloring area.
             data_column: name of column in pandas dataframe(s) used for color spec if
                 a gradient is used. Optional for single colors.
-            marker_symbol: symbol for each point.
+            marker_symbol: symbol for marker in tooltips and legends.
 
         Raises:
-            ChartStylingMissingDataColumnError: if a data_column is not defined when
-                color_spec is a ColorDiscreteMap or ColorGradient
+            ChartStylingMissingDataColumnError: if color_spec is
+                ColorDiscreteMap/ColorGradient and data_column
+                has not been specified
         """
         super().__init__(
             color_spec=color_spec, data_column=data_column, marker_symbol=marker_symbol
         )
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/scatter.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/styling/point.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-"""Spec to style a scatter series."""
+"""Spec to style a point series."""
 from typing import Optional
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
 from .base import BaseChartSeriesStyling
 from .enums import MarkerSymbol
 
 
-class ScatterSeriesStyling(BaseChartSeriesStyling):
-    """Customize appearance of scatter markers.
+class PointSeriesStyling(BaseChartSeriesStyling):
+    """Customize appearance of data points in Chart.
 
-    Specify styling options for a scatter series within a Timeseries
-    widget to customize the appearance of individual data points
-    represented as scatter markers on the chart.
+    Specify styling options for a point series within a Chart
+    widget to customize the appearance of individual
+    data points on the chart.
     """
 
-    _API_TYPE = "ChartScatterSeriesStylingInput"
-
     @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_column: Optional[TemplatedStringItem] = None,
         marker_symbol: MarkerSymbol = MarkerSymbol.CIRCLE,
     ):
-        """Constructor for ScatterSeriesStyling.
+        """Constructor for PointSeriesStyling.
 
         Args:
             color_spec: spec for coloring columns.
             data_column: name of column in pandas dataframe(s) used for color spec if
                 a gradient is used. Optional for single colors.
             marker_symbol: symbol for each point.
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/typing.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/styling/typing.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/base.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/tooltip/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Base Tooltip Item class."""
 
 from typing import Any
+from typing import Dict
 from typing import Optional
 from typing import Union
 
 import pandas as pd
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import DateTimeFormatting
@@ -12,28 +13,25 @@
 from engineai.sdk.dashboard.formatting import NumberFormatting
 from engineai.sdk.dashboard.formatting import TextFormatting
 from engineai.sdk.dashboard.links.abstract import AbstractFactoryLinkItemsHandler
 from engineai.sdk.dashboard.templated_string import DataField
 from engineai.sdk.dashboard.templated_string import InternalDataField
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 
 from .exceptions import TooltipItemColumnNotFoundError
 
 TooltipItemFormatter = Union[
     MapperFormatting, NumberFormatting, TextFormatting, DateTimeFormatting
 ]
 
 
 class BaseTooltipItem(AbstractFactoryLinkItemsHandler):
     """Base Tooltip Item class."""
 
-    _API_TYPE: Optional[str] = None
-
     @type_check
     def __init__(
         self,
         *,
         data_column: TemplatedStringItem,
         formatting: TooltipItemFormatter,
         label: Optional[Union[str, DataField]] = None,
@@ -56,20 +54,17 @@
 
     @property
     def label(self) -> InternalDataField:
         """Get label."""
         return self.__label
 
     @property
-    def _api_type(self) -> str:
-        if self._API_TYPE is None:
-            raise NotImplementedError(
-                f"Class {self.__class__.__name__}.API_TYPE not defined."
-            )
-        return self._API_TYPE
+    def data_column(self) -> TemplatedStringItem:
+        """Get data column."""
+        return self.__data_column
 
     def __reformat_data_column(self, data_column: str) -> str:
         return data_column.replace("_", " ").title()
 
     def validate(self, *, data: pd.DataFrame) -> None:
         """Validate if dataframe that will be used for column contains required columns.
 
@@ -86,19 +81,18 @@
                 class_name=self.__class__.__name__,
                 column_name="data_column",
                 column_value=self.__data_column,
             )
         if isinstance(self.__formatting, NumberFormatting):
             self.__formatting.validate(data)
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            self._api_type,
-            label=self.__label.build(),
-            valueKey=build_templated_strings(items=self.__data_column),
-            formatting=self.__formatting.build(),
-        )
+        return {
+            "label": self.__label.build(),
+            "valueKey": build_templated_strings(items=self.__data_column),
+            "formatting": self.__formatting.build(),
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/category.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/tooltip/category.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 class CategoryTooltipItem(BaseTooltipItem):
     """Customize tooltips for categorical data in Chart widget.
 
     Define specifications for a category tooltip item within a Chart widget to
     customize the appearance and content of tooltips displayed for categorical data.
     """
 
-    _API_TYPE = "TooltipCategoricalItemInput"
-
     @type_check
     def __init__(
         self,
         *,
         data_column: TemplatedStringItem,
         formatting: MapperFormatting,
         label: Optional[Union[str, DataField]] = None,
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/datetime.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/tooltip/datetime.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,16 +15,14 @@
     """Customize tooltips for datetime data in Chart.
 
     Define specifications for a datetime item within a tooltip for a
     Chart widget to customize the appearance and content
     of tooltips displayed for datetime data.
     """
 
-    _API_TYPE = "TooltipDateTimeItemInput"
-
     @type_check
     def __init__(
         self,
         *,
         data_column: TemplatedStringItem,
         formatting: Optional[DateTimeFormatting] = None,
         label: Optional[Union[str, DataField]] = None,
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/exceptions.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/tooltip/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/item.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/tooltip/item.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 """Spec to build tooltip items supported by different charts."""
 
 from typing import Any
-
-from engineai.sdk.dashboard.utils import generate_input
+from typing import Dict
 
 from ..typing import TooltipItem
 from .category import CategoryTooltipItem
+from .country import CountryTooltipItem
 from .datetime import DatetimeTooltipItem
 from .number import NumberTooltipItem
 from .text import TextTooltipItem
 
 
-def build_tooltip_item(item: TooltipItem) -> Any:
+def build_tooltip_item(item: TooltipItem) -> Dict[str, Any]:
     """Builds spec for dashboard API.
 
     Args:
         item (TooltipItem): item spec
 
     Returns:
         Input object for Dashboard API
     """
-    return generate_input("TooltipItemInput", **{_get_input_key(item): item.build()})
+    return {**{_get_input_key(item): item.build()}}
 
 
 def _get_input_key(item: TooltipItem) -> str:
     if isinstance(item, NumberTooltipItem):
         return "number"
     elif isinstance(item, TextTooltipItem):
         return "text"
     elif isinstance(item, DatetimeTooltipItem):
         return "dateTime"
     elif isinstance(item, CategoryTooltipItem):
         return "categorical"
+    elif isinstance(item, CountryTooltipItem):
+        return "country"
     else:
         raise TypeError(
             "item needs to be one of CategoryItem, DateTimeItem, "
             "NumberItem, TextItem"
         )
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/number.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/tooltip/number.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,14 @@
     """Customize tooltips for numerical data in Chart.
 
     Define specifications for a number item within a tooltip for a Chart
     widget to customize the appearance and content of tooltips displayed
     for numerical data.
     """
 
-    _API_TYPE = "TooltipNumberItemInput"
-
     @type_check
     def __init__(
         self,
         *,
         data_column: TemplatedStringItem,
         formatting: Optional[NumberFormatting] = None,
         label: Optional[Union[str, DataField]] = None,
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/text.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/tooltip/text.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,16 +15,14 @@
     """Customize tooltips for textual data in Chart.
 
     Define specifications for a text item within a tooltip
     for a Chart widget to customize the appearance and
     content of tooltips displayed for textual data.
     """
 
-    _API_TYPE = "TooltipTextItemInput"
-
     @type_check
     def __init__(
         self,
         *,
         data_column: TemplatedStringItem,
         formatting: Optional[TextFormatting] = None,
         label: Optional[Union[str, DataField]] = None,
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/typing.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/charts/typing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Specs for extra elements for tooltip of timeseries chart and series."""
 from typing import List
 from typing import Union
 
 from engineai.sdk.dashboard.widgets.components.charts.tooltip import CategoryTooltipItem
+from engineai.sdk.dashboard.widgets.components.charts.tooltip import CountryTooltipItem
 from engineai.sdk.dashboard.widgets.components.charts.tooltip import DatetimeTooltipItem
 from engineai.sdk.dashboard.widgets.components.charts.tooltip import NumberTooltipItem
 from engineai.sdk.dashboard.widgets.components.charts.tooltip import TextTooltipItem
 
 TooltipItem = Union[
     CategoryTooltipItem,
     DatetimeTooltipItem,
     NumberTooltipItem,
     TextTooltipItem,
+    CountryTooltipItem,
 ]
 
 TooltipItems = Union[TooltipItem, List[TooltipItem]]
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/__init__.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/styling/__init__.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/base.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/styling/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,33 +6,29 @@
 from typing import Optional
 from typing import Union
 from typing import cast
 
 import pandas as pd
 
 from engineai.sdk.dashboard.decorator import type_check
-from engineai.sdk.dashboard.exceptions import ImproperlyConfiguredError
 from engineai.sdk.dashboard.links.abstract import AbstractFactoryLinkItemsHandler
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.styling.color import Single
 from engineai.sdk.dashboard.styling.color.spec import build_color_spec
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 
 from .exceptions import ItemStylingValidationError
 
 
 class BaseItemStyling(AbstractFactoryLinkItemsHandler):
     """Spec for Number Styling Base class."""
 
-    _API_TYPE: Optional[str] = None
-
     @type_check
     def __init__(
         self,
         *,
         color_spec: Optional[ColorSpec] = None,
         data_column: Optional[TemplatedStringItem] = None,
     ):
@@ -68,26 +64,14 @@
                 UserWarning,
             )
 
     def _build_extra_inputs(self) -> Dict[str, Any]:
         return {}
 
     @property
-    def _api_type(self) -> str:
-        """Get API TYPE value."""
-        if self._API_TYPE is None:
-            raise ImproperlyConfiguredError(
-                f"Class {self.__class__.__name__} does not have the "
-                f"`_api_type` configured. Please set "
-                f"{self.__class__.__name__}._API_TYPE or change the "
-                f"{self.__class__.__name__}._api_type property."
-            )
-        return self._API_TYPE
-
-    @property
     def column(
         self,
     ) -> Optional[TemplatedStringItem]:
         """Return Data Column."""
         return self.__data_column
 
     @column.setter
@@ -124,21 +108,20 @@
         if not self.__contains_key(data=data):
             raise ItemStylingValidationError(
                 class_name=self.__class__.__name__,
                 column_value=str(self.__data_column),
                 column_name=column_name,
             )
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            self._api_type,
-            colorSpec=build_color_spec(spec=self.__color_spec)
+        return {
+            "colorSpec": build_color_spec(spec=self.__color_spec)
             if self.__color_spec
             else self.__color_spec,
-            valueKey=build_templated_strings(items=self.__data_column),
+            "valueKey": build_templated_strings(items=self.__data_column),
             **self._build_extra_inputs(),
-        )
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/chart/stacked_bar.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/styling/number/progress_bar.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,37 @@
-"""Spec for Widget Stacked Bar Chart Styling."""
+"""Spec for Number Styling Progress Bar."""
 from typing import Any
 from typing import Dict
 from typing import Optional
 
-from engineai.sdk.dashboard.styling.color.typing import ColorSpec
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
+from engineai.sdk.dashboard.templated_string import build_templated_strings
+from engineai.sdk.dashboard.widgets.components.items.styling.base import BaseItemStyling
 
-from ..base import BaseItemStyling
 
+class NumberStylingProgressBar(BaseItemStyling):
+    """Spec for Number Styling Progress Bar class."""
 
-class StackedBarChartItemStyling(BaseItemStyling):
-    """Spec for styling used by Stacked Bar Chart Item."""
-
-    _API_TYPE = "SparkChartStackedBarStylingInput"
-
+    @type_check
     def __init__(
         self,
         *,
-        data_column: Optional[TemplatedStringItem] = None,
-        color_spec: Optional[ColorSpec] = None,
-        show_total_value: bool = False
+        column: Optional[TemplatedStringItem] = None,
     ):
-        """Construct spec for the StackedBarChartItemStyling class.
+        """Construct spec for Number Styling Progress Bar.
 
         Args:
-            data_column (Optional[str]): styling data key.
-            color_spec (Optional[ColorSpec]): specs for color.
-            show_total_value (bool): whether to show total value.
+            column (Optional[TemplatedStringItem]): styling value key.
+                Defaults to None.
         """
-        super().__init__(data_column=data_column, color_spec=color_spec)
-        self.__show_total_value = show_total_value
+        super().__init__(data_column=column)
 
-    def _build_extra_inputs(self) -> Dict[str, Any]:
-        return {"showTotalOnTooltip": self.__show_total_value}
+    def build(self) -> Dict[str, Any]:
+        """Method implemented by all factories to generate Input spec.
+
+        Returns:
+            Input object for Dashboard API
+        """
+        return {
+            "valueKey": build_templated_strings(items=self.column),
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/exceptions.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/styling/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/number/arrow.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/styling/cell.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,43 @@
-"""Spec fot Number Styling Arrow."""
-
+"""Specification for styling a column with an arrow next to value."""
 from typing import Any
+from typing import Dict
 from typing import Optional
+from typing import Union
 
 from engineai.sdk.dashboard.decorator import type_check
-from engineai.sdk.dashboard.styling.color.divergent import Divergent
-from engineai.sdk.dashboard.templated_string import TemplatedStringItem
-from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
+from engineai.sdk.dashboard.links import WidgetField
+from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 
-from ..base import BaseItemStyling
+from .base import TableColumnStylingBase
 
 
-class NumberStylingArrow(BaseItemStyling):
-    """Spec for Number Arrow Styling class."""
+class CellStyling(TableColumnStylingBase):
+    """Styling options for table widget cell.
 
-    _API_TYPE: str = "NumberStylingArrowInput"
+    Specify the styling options for a cell in the table widget,
+    including color, data column, and percentage fill.
+    """
 
     @type_check
     def __init__(
         self,
         *,
-        data_column: Optional[TemplatedStringItem] = None,
-        color_divergent: Divergent,
+        color_spec: ColorSpec,
+        data_column: Optional[Union[str, WidgetField]] = None,
+        percentage_fill: Optional[Union[float, int]] = 1,
     ):
-        """Construct spec Number Arrow Styling.
+        """Constructor for CellStyling.
 
         Args:
-            color_divergent (ColorDivergent): specs for color.
-            data_column (TemplatedStringItem): styling value key.
+            data_column: id of column which values are used to determine behavior of
+                arrow. By default, will use values of column to which styling is
+                applied.
+            percentage_fill: how much of the cell should the color
+                fill. Default to 1, meaning the whole cell
+            color_spec: spec for color of arrows.
         """
-        super().__init__(
-            data_column=data_column,
-        )
-        self.__color_divergent = color_divergent
-
-    def build(self) -> Any:
-        """Method implemented by all factories to generate Input spec.
+        super().__init__(color_spec=color_spec, data_column=data_column)
+        self.__percentage_fill = percentage_fill
 
-        Returns:
-            Input object for Dashboard API
-        """
-        return generate_input(
-            self._api_type,
-            divergentPalette=self.__color_divergent.build(),
-            valueKey=build_templated_strings(items=self.column),
-        )
+    def _build_extra_inputs(self) -> Dict[str, Any]:
+        return {"percentageFill": self.__percentage_fill}
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/number/chip.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/styling/number/font.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,29 @@
-"""Spec fot Number Styling Chip."""
+"""Spec fot Number Styling Font."""
 
 from typing import Optional
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.styling.color.spec import ColorSpec
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
 from ..base import BaseItemStyling
 
 
-class NumberStylingChip(BaseItemStyling):
-    """Spec for Number Chip Styling class."""
-
-    _API_TYPE: str = "NumberStylingChipInput"
+class NumberStylingFont(BaseItemStyling):
+    """Spec for Number Font Styling class."""
 
     @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_column: Optional[TemplatedStringItem] = None,
     ):
-        """Construct spec for Number Chip Styling.
+        """Construct spec for Number Font Styling.
 
         Args:
-            color_spec (ColorSpec): specs for color.
+            color_spec (Optional[ColorSpec): specs for color.
             data_column (Optional[TemplatedStringItem]): styling value key.
                 Defaults to None.
         """
         super().__init__(data_column=data_column, color_spec=color_spec)
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/number/dot.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/styling/number/chip.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,29 @@
-"""Spec fot Number Styling Dot."""
+"""Spec fot Number Styling Chip."""
 
 from typing import Optional
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.styling.color.spec import ColorSpec
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
 from ..base import BaseItemStyling
 
 
-class NumberStylingDot(BaseItemStyling):
-    """Spec for Number Dot Styling class."""
-
-    _API_TYPE = "NumberStylingDotInput"
+class NumberStylingChip(BaseItemStyling):
+    """Spec for Number Chip Styling class."""
 
     @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_column: Optional[TemplatedStringItem] = None,
     ):
-        """Construct spec for Number Dot Styling.
+        """Construct spec for Number Chip Styling.
 
         Args:
             color_spec (ColorSpec): specs for color.
             data_column (Optional[TemplatedStringItem]): styling value key.
+                Defaults to None.
         """
-        super().__init__(
-            color_spec=color_spec,
-            data_column=data_column,
-        )
+        super().__init__(data_column=data_column, color_spec=color_spec)
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/number/font.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/styling/text/chip.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,27 @@
-"""Spec fot Number Styling Font."""
-
+"""Spec fot Text Styling Font."""
 from typing import Optional
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.styling.color.spec import ColorSpec
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
 from ..base import BaseItemStyling
 
 
-class NumberStylingFont(BaseItemStyling):
-    """Spec for Number Font Styling class."""
-
-    _API_TYPE = "NumberStylingFontInput"
+class TextStylingChip(BaseItemStyling):
+    """Spec for Text Chip Styling Class."""
 
     @type_check
     def __init__(
         self,
         *,
-        color_spec: ColorSpec,
+        color_spec: Optional[ColorSpec] = None,
         data_column: Optional[TemplatedStringItem] = None,
     ):
-        """Construct spec for Number Font Styling.
+        """Construct spec for Text Chip Styling.
 
         Args:
-            color_spec (Optional[ColorSpec): specs for color.
+            color_spec (Optional[ColorSpec]): specs for color.
             data_column (Optional[TemplatedStringItem]): styling value key.
-                Defaults to None.
         """
         super().__init__(data_column=data_column, color_spec=color_spec)
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/number/progress_bar.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/styling/text/font.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,28 @@
-"""Spec for Number Styling Progress Bar."""
-from typing import Any
+"""Spec fot Text Styling Font."""
 from typing import Optional
 
 from engineai.sdk.dashboard.decorator import type_check
+from engineai.sdk.dashboard.styling.color.spec import ColorSpec
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
-from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
-from engineai.sdk.dashboard.widgets.components.items.styling.base import BaseItemStyling
 
+from ..base import BaseItemStyling
 
-class NumberStylingProgressBar(BaseItemStyling):
-    """Spec for Number Styling Progress Bar class."""
 
-    _API_TYPE = "NumberStylingProgressBarInput"
+class TextStylingFont(BaseItemStyling):
+    """Spec for Text Font Styling Class."""
 
     @type_check
     def __init__(
         self,
         *,
-        column: Optional[TemplatedStringItem] = None,
+        color_spec: Optional[ColorSpec] = None,
+        data_column: Optional[TemplatedStringItem] = None,
     ):
-        """Construct spec for Number Styling Progress Bar.
+        """Construct spec for Text Font Styling.
 
         Args:
-            column (Optional[TemplatedStringItem]): styling value key.
+            color_spec (ColorSpec): specs for color.
+            data_column (Optional[TemplatedStringItem]): styling value key.
                 Defaults to None.
         """
-        super().__init__(data_column=column)
-
-    def build(self) -> Any:
-        """Method implemented by all factories to generate Input spec.
-
-        Returns:
-            Input object for Dashboard API
-        """
-        return generate_input(
-            self._api_type,
-            valueKey=build_templated_strings(items=self.column),
-        )
+        super().__init__(data_column=data_column, color_spec=color_spec)
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/text/chip.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/styling/number/dot.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-"""Spec fot Text Styling Font."""
+"""Spec fot Number Styling Dot."""
+
 from typing import Optional
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.styling.color.spec import ColorSpec
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
 from ..base import BaseItemStyling
 
 
-class TextStylingChip(BaseItemStyling):
-    """Spec for Text Chip Styling Class."""
-
-    _API_TYPE = "TextStylingChipInput"
+class NumberStylingDot(BaseItemStyling):
+    """Spec for Number Dot Styling class."""
 
     @type_check
     def __init__(
         self,
         *,
-        color_spec: Optional[ColorSpec] = None,
+        color_spec: ColorSpec,
         data_column: Optional[TemplatedStringItem] = None,
     ):
-        """Construct spec for Text Chip Styling.
+        """Construct spec for Number Dot Styling.
 
         Args:
-            color_spec (Optional[ColorSpec]): specs for color.
+            color_spec (ColorSpec): specs for color.
             data_column (Optional[TemplatedStringItem]): styling value key.
         """
-        super().__init__(data_column=data_column, color_spec=color_spec)
+        super().__init__(
+            color_spec=color_spec,
+            data_column=data_column,
+        )
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/text/country_flag.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/styling/text/country_flag.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 """Spec fot Text Styling Font."""
 from typing import Any
+from typing import Dict
 from typing import Optional
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 
 from ..base import BaseItemStyling
 
 
 class TextStylingCountryFlag(BaseItemStyling):
     """Spec for Text Country Flag Styling Class."""
 
-    _API_TYPE = "TextStylingCountryFlagInput"
-
     @type_check
     def __init__(
         self,
         *,
         left: bool = True,
         data_column: Optional[TemplatedStringItem] = None,
     ):
@@ -28,18 +26,17 @@
             data_column (Optional[TemplatedStringItem]): styling value key.
             left (bool): whether to put flag to the left (True) or
                 right (False) of column value.
         """
         super().__init__(data_column=data_column, color_spec=None)
         self.__left = left
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            self._api_type,
-            left=self.__left,
-            valueKey=build_templated_strings(items=self.column),
-        )
+        return {
+            "left": self.__left,
+            "valueKey": build_templated_strings(items=self.column),
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/text/dot.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/styling/text/dot.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 
 from ..base import BaseItemStyling
 
 
 class TextStylingDot(BaseItemStyling):
     """Spec for Text Dot Styling Class."""
 
-    _API_TYPE = "TextStylingDotInput"
-
     @type_check
     def __init__(
         self,
         *,
         color_spec: Optional[ColorSpec] = None,
         data_column: Optional[TemplatedStringItem] = None,
     ):
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/text/font.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/styling/country_flag.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,40 @@
-"""Spec fot Text Styling Font."""
+"""Specification for styling a column with a country flag to a value."""
+from typing import Any
+from typing import Dict
 from typing import Optional
+from typing import Union
 
 from engineai.sdk.dashboard.decorator import type_check
-from engineai.sdk.dashboard.styling.color.spec import ColorSpec
-from engineai.sdk.dashboard.templated_string import TemplatedStringItem
+from engineai.sdk.dashboard.links import WidgetField
 
-from ..base import BaseItemStyling
+from .base import TableColumnStylingBase
 
 
-class TextStylingFont(BaseItemStyling):
-    """Spec for Text Font Styling Class."""
+class CountryFlagStyling(TableColumnStylingBase):
+    """Styling options for country flag column.
 
-    _API_TYPE = "TextStylingFontInput"
+    Specify the styling options for a country flag column
+    in the table widget, including position and data column.
+    """
 
     @type_check
     def __init__(
         self,
         *,
-        color_spec: Optional[ColorSpec] = None,
-        data_column: Optional[TemplatedStringItem] = None,
+        left: bool = True,
+        data_column: Optional[Union[str, WidgetField]] = None,
     ):
-        """Construct spec for Text Font Styling.
+        """Constructor for CountryFlagStyling.
 
         Args:
-            color_spec (ColorSpec): specs for color.
-            data_column (Optional[TemplatedStringItem]): styling value key.
-                Defaults to None.
+            data_column: id of column which values are used to determine behavior of
+                arrow.
+                By default, will use values of column to which styling is applied.
+            left: whether to put flag to the left (True) or right (False) of column
+                value.
         """
-        super().__init__(data_column=data_column, color_spec=color_spec)
+        super().__init__(data_column=data_column, color_spec=None)
+        self.__left = left
+
+    def _build_extra_inputs(self) -> Dict[str, Any]:
+        return {"left": self.__left}
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/tooltip/format_build.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/tooltip/format_build.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """Spec to build different items supported by tile widget."""
 
 from typing import Any
+from typing import Dict
 
 from engineai.sdk.dashboard.formatting import DateTimeFormatting
 from engineai.sdk.dashboard.formatting import MapperFormatting
 from engineai.sdk.dashboard.formatting import NumberFormatting
 from engineai.sdk.dashboard.formatting import TextFormatting
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.charts.tooltip.base import (
     TooltipItemFormatter,
 )
 
 
-def build_items(item: TooltipItemFormatter) -> Any:
+def build_items(item: TooltipItemFormatter) -> Dict[str, Any]:
     """Builds spec for dashboard API.
 
     Args:
         item (TileItem): item spec
 
     Returns:
         Input object for Dashboard API
     """
-    return generate_input("FormattingInput", **{_get_input_key(item): item.build()})
+    return {**{_get_input_key(item): item.build()}}
 
 
 def _get_input_key(item: TooltipItemFormatter) -> str:
     if isinstance(item, TextFormatting):
         result = "text"
     elif isinstance(item, NumberFormatting):
         result = "number"
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/tooltip/header.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/tooltip/header.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from typing import Union
 
 import pandas as pd
 
 from engineai.sdk.dashboard.links.abstract import AbstractFactoryLinkItemsHandler
 from engineai.sdk.dashboard.templated_string import DataField
 from engineai.sdk.dashboard.templated_string import InternalDataField
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.charts.tooltip.base import (
     TooltipItemFormatter,
 )
 
 from .format_build import build_items
 
 
@@ -47,18 +46,17 @@
             data (Union[pd.DataFrame, Dict[str, Any]]): pandas DataFrame or dict where
                 the data is present.
             item_id_key: Optional[str]: key in data (if using data as dict) used to
                 identify the data that feeds this item.
         """
         self.__title.validate(data=data, item_id_key=item_id_key)
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Builds spec for dashboard API.
 
         Returns:
             Any: Input object for Dashboard API
         """
-        return generate_input(
-            "SparkChartTooltipHeaderInput",
-            title=self.__title.build(),
-            format=build_items(self.__format) if self.__format else None,
-        )
+        return {
+            "title": self.__title.build(),
+            "format": build_items(self.__format) if self.__format else None,
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/tooltip/tooltip.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/tooltip/tooltip.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from typing import Union
 
 import pandas as pd
 
 from engineai.sdk.dashboard.formatting.text import TextFormatting
 from engineai.sdk.dashboard.links.abstract import AbstractFactoryLinkItemsHandler
 from engineai.sdk.dashboard.templated_string import DataField
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.charts.tooltip.base import (
     TooltipItemFormatter,
 )
 
 from .header import HeaderTooltip
 
 
@@ -29,15 +28,15 @@
         """Construct for ChartTooltip class.
 
         Args:
             title (Union[str, DataField]): header title spec.
             formatting (Optional[TooltipItemFormatter]): header tooltip formatting.
         """
         super().__init__()
-        self.__header = HeaderTooltip(
+        self._header = HeaderTooltip(
             title=title,
             formatting=formatting or TextFormatting(),
         )
 
     def validate(
         self,
         data: Union[pd.DataFrame, Dict[str, Any]],
@@ -47,19 +46,18 @@
 
         Args:
             data (Union[pd.DataFrame, Dict[str, Any]]): pandas DataFrame or dict where
                 the data is present.
             item_id_key: Optional[str]: key in data (if using data as dict) used to
                 identify the data that feeds this item.
         """
-        self.__header.validate(data=data, item_id_key=item_id_key)
+        self._header.validate(data=data, item_id_key=item_id_key)
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Builds spec for dashboard API.
 
         Returns:
             Any: Input object for Dashboard API
         """
-        return generate_input(
-            "SparkChartTooltipInput",
-            header=self.__header.build(),
-        )
+        return {
+            "header": self._header.build(),
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/content/content.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/content/content.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from typing import Optional
 from typing import Union
 
 from engineai.sdk.dashboard.data import DataSource
 from engineai.sdk.dashboard.data.http import Http
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.utils import build_data
 
 from ..base import Widget
 from ..base import WidgetTitleType
 from .exceptions import ContentNoItemsError
 from .item import ContentItem
 from .item import build_content_item
@@ -68,23 +67,24 @@
         Returns:
             Content: reference to this Content Widget to facilitate inline manipulation.
 
         """
         self.__items.extend(items)
         return self
 
-    def _build_widget_input(self) -> Any:
+    def _build_widget_input(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
         if len(self.__items) == 0:
             raise ContentNoItemsError(
                 widget_id=self.widget_id,
             )
-        return generate_input(
-            "ContentWidgetInput",
-            title=build_templated_strings(items=self.__title) if self.__title else None,
-            contentItems=[build_content_item(item=item) for item in self.__items],
-            data=build_data(path=self.dependency_id),
-        )
+        return {
+            "title": build_templated_strings(items=self.__title)
+            if self.__title
+            else None,
+            "contentItems": [build_content_item(item=item) for item in self.__items],
+            "data": build_data(path=self.dependency_id),
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/content/exceptions.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/content/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/content/markdown.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/content/markdown.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Spec for MarkdownItem class."""
 
 from typing import Any
 from typing import Dict
 
 from engineai.sdk.dashboard.base import AbstractFactory
 from engineai.sdk.dashboard.decorator import type_check
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.content.exceptions import ContentItemNoValueError
 
 
 class MarkdownItem(AbstractFactory):
     """Spec for MarkdownItem class."""
 
     @type_check
@@ -36,14 +35,14 @@
         if self.__data_key not in data:
             raise ContentItemNoValueError(
                 data_key="data_key",
                 data_key_value=self.__data_key,
                 class_name=self.__class__.__name__,
             )
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input("ContentWidgetMarkdownItemInput", dataKey=self.__data_key)
+        return {"dataKey": self.__data_key}
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/exceptions.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/__init__.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/maps/__init__.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/color_axis.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/maps/color_axis.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Spec for ColorAxis of a Map Shape widget."""
 
 from typing import Any
+from typing import Dict
 from typing import Optional
 
 from engineai.sdk.dashboard.base import AbstractFactory
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting.number import NumberFormatting
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.maps.enums import LegendPosition
 
 
 class ColorAxis(AbstractFactory):
     """Spec for ColorAxis of a Map widget."""
 
     @type_check
@@ -27,18 +27,17 @@
                 relative to data, maps.
             formatting: formatting spec for value.
         """
         super().__init__()
         self._position = position
         self._formatting = formatting if formatting else NumberFormatting()
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "MapWidgetColorAxisInput",
-            position=self._position.value,
-            formatting=self._formatting.build(),
-        )
+        return {
+            "position": self._position.value,
+            "formatting": self._formatting.build(),
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/enums.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/maps/enums.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/exceptions.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/maps/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/geo/base.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/maps/geo/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from pandas.api.types import is_numeric_dtype
 from pandas.api.types import is_object_dtype
 from pandas.api.types import is_string_dtype
 
 from engineai.sdk.dashboard.data.decorator import DataSource
 from engineai.sdk.dashboard.data.http import Http
 from engineai.sdk.dashboard.decorator import type_check
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.chart_utils import get_object_columns_tooltip
 from engineai.sdk.dashboard.widgets.components.charts.tooltip.datetime import (
     DatetimeTooltipItem,
 )
 from engineai.sdk.dashboard.widgets.components.charts.tooltip.item import (
     build_tooltip_item,
 )
@@ -138,35 +137,34 @@
 
     def _validate_series(self, data: T) -> None:
         """Validates styling for map series spec."""
         if isinstance(data, pd.DataFrame):
             for series in self._series:
                 series.validate(data=data)
 
-    def _build_series(self) -> Any:
+    def _build_series(self) -> Dict[str, Any]:
         """Builds series spec."""
         series_spec = []
         for series in self._series:
             series_spec.append(build_map_series(series=series))
         return series_spec
 
-    def _build_tooltips(self) -> Any:
+    def _build_tooltips(self) -> Dict[str, Any]:
         """Builds tooltip spec."""
         if self._extra_tooltip_items:
-            return generate_input(
-                "MapWidgetTooltipInput",
-                regionKey=self._region_column,
-                data=build_data(path=self.dependency_id, json_data=self._json_data),
-                items=[
+            return {
+                "regionKey": self._region_column,
+                "data": build_data(path=self.dependency_id, json_data=self._json_data),
+                "items": [
                     build_tooltip_item(item=tooltip)
                     for tooltip in self._extra_tooltip_items
                 ]
                 if self._extra_tooltip_items
                 else [],
-            )
+            }
         return None
 
     def _auto_generate_tooltips(
         self,
         data: Union[DataSource, T],
         series: Optional[MapSeries],
         region_column: str,
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/geo/geo.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/maps/geo/geo.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Spec for Map Geo widget."""
 
 from typing import Any
+from typing import Dict
 from typing import Optional
 from typing import Union
 
 import pandas as pd
 
 from engineai.sdk.dashboard.data import DataSource
 from engineai.sdk.dashboard.data.http import Http
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.charts.typing import TooltipItems
 from engineai.sdk.dashboard.widgets.maps.color_axis import ColorAxis
 from engineai.sdk.dashboard.widgets.maps.enums import LegendPosition
 from engineai.sdk.dashboard.widgets.maps.enums import Region
 
 from ...base import WidgetTitleType
 from ..series.series import MapSeries
@@ -83,26 +83,27 @@
             legend_position=legend_position,
             color_axis=color_axis,
             styling=styling,
             region=region,
             tooltips=tooltips,
         )
 
-    def _build_widget_input(self) -> Any:
+    def _build_widget_input(self) -> Dict[str, Any]:
         """Method to build map widget."""
-        return generate_input(
-            "MapGeoWidgetInput",
-            title=build_templated_strings(items=self._title) if self._title else None,
-            colorAxis=self._color_axis.build(),
-            legend=self._legend_position.build(),
-            series=self._build_series(),
-            region=self._region.value,
-            styling=self._styling.build(),
-            tooltip=self._build_tooltips(),
-        )
+        return {
+            "title": build_templated_strings(items=self._title)
+            if self._title
+            else None,
+            "colorAxis": self._color_axis.build(),
+            "legend": self._legend_position.build(),
+            "series": self._build_series(),
+            "region": self._region.value,
+            "styling": self._styling.build(),
+            "tooltip": self._build_tooltips(),
+        }
 
     def validate(self, data: pd.DataFrame, **kwargs: Any) -> None:
         """Validates widget spec.
 
         Args:
             data: pandas DataFrame where
                 the data is present.
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/geo/styling/label.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/maps/geo/styling/label.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Spec for legend of a Map Shape widget."""
 
 from typing import Any
+from typing import Dict
 
 from engineai.sdk.dashboard.base import AbstractFactory
 from engineai.sdk.dashboard.decorator import type_check
-from engineai.sdk.dashboard.utils import generate_input
 
 
 class MapStylingLabel(AbstractFactory):
     """Spec for Map Geo Styling Label of a Map widget."""
 
     @type_check
     def __init__(self, *, hidden: bool = False):
@@ -16,14 +16,14 @@
 
         Args:
             hidden: Hide labels.
         """
         super().__init__()
         self._hidden = hidden
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input("MapGeoWidgetStylingLabel", hidden=self._hidden)
+        return {"hidden": self._hidden}
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/geo/styling/styling.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/maps/geo/styling/styling.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Spec for MapSryling of a Map Geo widget."""
 
 from typing import Any
+from typing import Dict
 from typing import Optional
 
 from engineai.sdk.dashboard.base import AbstractFactory
 from engineai.sdk.dashboard.decorator import type_check
-from engineai.sdk.dashboard.utils import generate_input
 
 from .label import MapStylingLabel
 
 
 class MapStyling(AbstractFactory):
     """Spec for MapStyling of a Map Geo widget."""
 
@@ -19,17 +19,16 @@
 
         Args:
             label: label style for map
         """
         super().__init__()
         self._label = label if label is not None else MapStylingLabel()
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "MapGeoWidgetStylingInput",
-            label=self._label.build(),
-        )
+        return {
+            "label": self._label.build(),
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/legend.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/legend.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,34 @@
-"""Spec for legend of a Map Shape widget."""
-
+"""Spec for legend of a timeseries widget."""
 from typing import Any
+from typing import Dict
 
 from engineai.sdk.dashboard.base import AbstractFactory
 from engineai.sdk.dashboard.decorator import type_check
-from engineai.sdk.dashboard.utils import generate_input
-from engineai.sdk.dashboard.widgets.maps.enums import LegendPosition
+from engineai.sdk.dashboard.enum.legend_position import LegendPosition
 
 
 class Legend(AbstractFactory):
-    """Spec for legend of a Map widget."""
+    """Spec for legend of a timeseries widget."""
 
     @type_check
     def __init__(self, *, position: LegendPosition = LegendPosition.BOTTOM):
-        """Constructor for Legend.
+        """Construct a legend for a timeseries widget.
 
         Args:
-            position (Position): location of position
-                relative to data, maps.
+            position: location of position relative to data, charts.
         """
         super().__init__()
         self.__position = position
 
-    def build(self) -> Any:
+    @property
+    def position(self) -> LegendPosition:
+        """Returns the current Legend Position."""
+        return self.__position
+
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input("MapWidgetLegendInput", position=self.__position.value)
+        return {"position": self.__position.value}
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/series/numeric.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/maps/series/numeric.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Spec for a numeric series of a Map widget."""
 
 from typing import Any
+from typing import Dict
 from typing import Optional
 from typing import Union
 
 import pandas as pd
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import NumberFormatting
 from engineai.sdk.dashboard.styling import color
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.charts.tooltip.item import (
     build_tooltip_item,
 )
 from engineai.sdk.dashboard.widgets.components.charts.typing import TooltipItems
 from engineai.sdk.dashboard.widgets.maps.exceptions import MapColumnDataNotFoundError
 from engineai.sdk.dashboard.widgets.maps.series.styling import SeriesStyling
 
@@ -105,26 +105,25 @@
         if self.__styling is None:
             self.__styling = SeriesStyling(
                 color_spec=color.Single(
                     color=color.palette.qualitative_palette(index=index)
                 )
             )
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "MapWidgetNumericSeriesInput",
-            valueKey=build_templated_strings(items=self.__data_column),
-            regionKey=build_templated_strings(items=self.__region_column),
-            name=build_templated_strings(items=self.__name),
-            formatting=self.__formatting.build(),
-            styling=self.__styling.build() if self.__styling else None,
-            tooltipItems=[
+        return {
+            "valueKey": build_templated_strings(items=self.__data_column),
+            "regionKey": build_templated_strings(items=self.__region_column),
+            "name": build_templated_strings(items=self.__name),
+            "formatting": self.__formatting.build(),
+            "styling": self.__styling.build() if self.__styling else None,
+            "tooltipItems": [
                 build_tooltip_item(item=item) for item in self.__tooltip_items
             ],
-            data=build_data(path=self.__dependency_id, json_data=self.__json_data),
-            required=self.__required,
-        )
+            "data": build_data(path=self.__dependency_id, json_data=self.__json_data),
+            "required": self.__required,
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/series/styling.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/maps/series/styling.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Spec to style a line series."""
 
 from typing import Any
+from typing import Dict
 from typing import Optional
 
 import pandas as pd
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.styling.color.discrete_map import DiscreteMap
 from engineai.sdk.dashboard.styling.color.gradient import Gradient
 from engineai.sdk.dashboard.styling.color.palette import Palette
 from engineai.sdk.dashboard.styling.color.single import Single
 from engineai.sdk.dashboard.styling.color.spec import build_color_spec
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.charts.styling.enums import MarkerSymbol
 from engineai.sdk.dashboard.widgets.maps.exceptions import MapColumnDataNotFoundError
 
 
 class SeriesStyling:
     """Style numeric series appearance on map.
 
@@ -68,18 +68,17 @@
         if (
             not isinstance(self.__color_spec, Single)
             and self.__data_column
             and self.__data_column not in data.columns
         ):
             raise MapColumnDataNotFoundError(column_data=self.__data_column)
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "MapWidgetSeriesStylingInput",
-            colorSpec=build_color_spec(spec=self.__color_spec),
-            markerSymbol=MarkerSymbol.CIRCLE.value,
-        )
+        return {
+            "colorSpec": build_color_spec(spec=self.__color_spec),
+            "markerSymbol": MarkerSymbol.CIRCLE.value,
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pandas_utils.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/__init__.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/pie/__init__.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/chart.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/pie/chart.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Spec for Pie Chart."""
 
 from typing import Any
+from typing import Dict
 from typing import Optional
 
 import pandas as pd
 
 from engineai.sdk.dashboard.base import AbstractFactory
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.charts.typing import TooltipItems
 
 from .series.typings import ChartSeries
 from .tooltip import Tooltip
 
 
 class Chart(AbstractFactory):
@@ -47,18 +47,17 @@
                 not in data.
         """
         self._series.validate(
             data=data,
         )
         self._tooltip.validate(data=data)
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Builds spec for dashboard API.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "PieWidgetChartInput",
-            series_temp=self._series.build(),
-            tooltip=self._tooltip.build() if self._tooltip else None,
-        )
+        return {
+            "series_temp": self._series.build(),
+            "tooltip": self._tooltip.build() if self._tooltip else None,
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/exceptions.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/pie/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/legend.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/pie/legend.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Spec for Legend position and respective build."""
 import enum
 from typing import Any
-
-from engineai.sdk.dashboard.utils import generate_input
+from typing import Dict
 
 
 class LegendPosition(enum.Enum):
     """Legend position options.
 
     Options for positioning the legend on the pie chart,
     including right, bottom, and next to the data.
@@ -18,17 +17,16 @@
     """
 
     RIGHT = "RIGHT"
     BOTTOM = "BOTTOM"
     NEXT_TO_DATA = "NEXT_TO_DATA"
 
 
-def build_legend(legend: LegendPosition) -> Any:
+def build_legend(legend: LegendPosition) -> Dict[str, Any]:
     """Builds spec for dashboard API.
 
     Returns:
         Input object for Dashboard API
     """
-    return generate_input(
-        "PieWidgetLegendInput",
-        position=legend.value,
-    )
+    return {
+        "position": legend.value,
+    }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/pie.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/pie/pie.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Spec for Pie Widget."""
 from typing import Any
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 import pandas as pd
 from pandas.api.types import is_datetime64_dtype
 from pandas.api.types import is_numeric_dtype
 from pandas.api.types import is_object_dtype
 from pandas.api.types import is_string_dtype
 
 from engineai.sdk.dashboard.data import DataSource
 from engineai.sdk.dashboard.data.http import Http
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.chart_utils import TooltipItem
 from engineai.sdk.dashboard.widgets.chart_utils import get_object_columns_tooltip
 from engineai.sdk.dashboard.widgets.components.charts.tooltip.datetime import (
     DatetimeTooltipItem,
 )
 from engineai.sdk.dashboard.widgets.components.charts.tooltip.number import (
     NumberTooltipItem,
@@ -151,19 +151,16 @@
         """Validates Pie Widget and the inner components specs."""
         self._chart.validate(data=data)
 
     def _prepare(self, **kwargs: object) -> None:
         """Method for each Widget prepare before building."""
         self._chart.prepare(self.dependency_id, kwargs.get("json_data", None))
 
-    def _build_widget_input(self) -> Any:
+    def _build_widget_input(self) -> Dict[str, Any]:
         """Builds spec for dashboard API."""
-        return generate_input(
-            "PieWidgetInput",
-            title=build_templated_strings(items=self._title) if self._title else None,
-            chart=self._chart.build(),
-            legend=build_legend(self._legend_position),
-        )
-
-    def build_widget_input(self) -> Any:
-        """Method to access the build from outside the class."""
-        return self._build_widget_input()
+        return {
+            "title": build_templated_strings(items=self._title)
+            if self._title
+            else None,
+            "chart": self._chart.build(),
+            "legend": build_legend(self._legend_position),
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/series/base.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/pie/series/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 """Spec for Pie Series."""
 
 from typing import Any
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 import pandas as pd
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting.number import NumberFormatting
 from engineai.sdk.dashboard.links.abstract import AbstractFactoryLinkItemsHandler
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.charts.tooltip.item import (
     build_tooltip_item,
 )
 from engineai.sdk.dashboard.widgets.components.charts.typing import TooltipItem
 from engineai.sdk.dashboard.widgets.components.charts.typing import TooltipItems
 from engineai.sdk.dashboard.widgets.utils import build_data
 
 from ..exceptions import PieValidateValueError
 from .styling import SeriesStyling
 
 
 class BaseSeries(AbstractFactoryLinkItemsHandler):
     """Spec for BaseSeries."""
 
-    _API_TYPE: Optional[str] = None
     _INPUT_KEY: Optional[str] = None
 
     @type_check
     def __init__(
         self,
         *,
         name: TemplatedStringItem,
@@ -70,23 +69,14 @@
             if isinstance(tooltips, list)
             else ([tooltips] if tooltips is not None else [])
         )
         self._dependency_id: str = " "
         self._json_data: Any = None
 
     @property
-    def _api_type(self) -> str:
-        """Returns API type argument value."""
-        if self._API_TYPE is None:
-            raise NotImplementedError(
-                f"Class {self.__class__.__name__}._API_TYPE not defined."
-            )
-        return self._API_TYPE
-
-    @property
     def _input_key(self) -> str:
         """Returns styling Input Key argument value."""
         if self._INPUT_KEY is None:
             raise NotImplementedError(
                 f"Class {self.__class__.__name__}._INPUT_KEY not defined."
             )
         return self._INPUT_KEY
@@ -139,43 +129,41 @@
         )
         for tooltip in self._tooltip_items:
             tooltip.validate(data=data)
 
         if self._styling is not None:
             self._styling.validate(data=data)
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Builds spec for dashboard API.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "PieWidgetChartSeriesUnionInput",
+        return {
             **{
                 self._input_key: self._build_series(),
             },
-        )
+        }
 
-    def _build_series(self) -> Any:
+    def _build_series(self) -> Dict[str, Any]:
         """Builds spec for dashboard API.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            self._api_type,
-            name=build_templated_strings(items=self._name),
-            valueKey=build_templated_strings(items=self._data_column),
-            formatting=self._formatting.build(),
-            data=build_data(path=self._dependency_id, json_data=self._json_data),
-            styling=self._styling.build() if self._styling is not None else None,
-            tooltipItems=[
+        return {
+            "name": build_templated_strings(items=self._name),
+            "valueKey": build_templated_strings(items=self._data_column),
+            "formatting": self._formatting.build(),
+            "data": build_data(path=self._dependency_id, json_data=self._json_data),
+            "styling": self._styling.build() if self._styling is not None else None,
+            "tooltipItems": [
                 build_tooltip_item(item=item) for item in self._tooltip_items
             ],
             **self._build_category_key(),
-        )
+        }
 
-    def _build_category_key(self) -> Any:
+    def _build_category_key(self) -> Dict[str, Any]:
         return {
             "categoryIdKey": build_templated_strings(items=self._category_column),
         }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/series/country.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/pie/series/country.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Spec for Pie Series."""
 
 from typing import Any
+from typing import Dict
 from typing import Optional
 from typing import Union
 
 import pandas as pd
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting.number import NumberFormatting
@@ -21,15 +22,14 @@
     """Define country-based pie chart series.
 
     Define a series specifically for pie charts representing data
     categorized by country, with options for customizing country code
     column, data column, formatting, styling, and tooltips.
     """
 
-    _API_TYPE = "PieWidgetChartSeriesCountryInput"
     _INPUT_KEY = "country"
 
     @type_check
     def __init__(
         self,
         *,
         name: TemplatedStringItem = "Country Series",
@@ -91,11 +91,11 @@
         self._validate_field(
             data=data,
             field="country_column",
             item=self._category_column,
         )
         super().validate(data=data)
 
-    def _build_category_key(self) -> Any:
+    def _build_category_key(self) -> Dict[str, Any]:
         return {
             "countryCodeKey": build_templated_strings(items=self._category_column),
         }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/series/series.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/pie/series/series.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 class Series(BaseSeries):
     """Define pie chart series.
 
     Define a generic series for the pie chart, specifying
     category and data columns, formatting, styling, and tooltips.
     """
 
-    _API_TYPE = "PieWidgetChartSeriesStandardInput"
     _INPUT_KEY = "standard"
 
     @type_check
     def __init__(
         self,
         *,
         name: TemplatedStringItem = "Series",
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/series/styling.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/pie/series/styling.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 class SeriesStyling(BaseChartSeriesStyling):
     """Style pie chart series.
 
     Specify styling options for pie chart series, including
     color specifications and data column mapping.
     """
 
-    _API_TYPE = "ChartPieSeriesStylingInput"
-
     @type_check
     def __init__(
         self,
         color_spec: Optional[ColorSpec] = None,
         data_column: Optional[TemplatedStringItem] = None,
     ):
         """Constructor for SeriesStyling.
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/tooltip.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/pie/tooltip.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Spec for Pie Tooltip."""
 
 from typing import Any
+from typing import Dict
 from typing import Optional
 
 import pandas as pd
 
 from engineai.sdk.dashboard.base import AbstractFactory
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.charts.tooltip.item import (
     build_tooltip_item,
 )
 from engineai.sdk.dashboard.widgets.components.charts.typing import TooltipItems
 from engineai.sdk.dashboard.widgets.utils import build_data
 
 
@@ -60,19 +60,18 @@
 
         Args:
             data: data associated to path
         """
         for tooltip in self._tooltips:
             tooltip.validate(data=data)
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Builds spec for dashboard API.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "PieWidgetTooltipInput",
-            items=[build_tooltip_item(item=item) for item in self._tooltips],
-            data=build_data(path=self._dependency_id, json_data=self._json_data),
-            categoryIdKey=build_templated_strings(items=self._category_column),
-        )
+        return {
+            "items": [build_tooltip_item(item=item) for item in self._tooltips],
+            "data": build_data(path=self._dependency_id, json_data=self._json_data),
+            "categoryIdKey": build_templated_strings(items=self._category_column),
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/exceptions.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/search/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/results/base.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/search/results/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 """Specs for Base Search Result Column."""
 from typing import Any
+from typing import Dict
 from typing import Mapping
 from typing import Optional
 from typing import Union
 
 import pandas as pd
 
 from engineai.sdk.dashboard.base import AbstractFactory
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 
 from ..exceptions import SearchValidateNoDataColumnError
 from .styling.base_styling import ResultColumnStyling
 
 
 class BaseResultItem(AbstractFactory):
     """Specs for Base Search Result Column."""
 
-    _API_TYPE: Optional[str] = None
-
     def __init__(
         self,
         data_column: TemplatedStringItem,
         styling: Optional[Union[Palette, ResultColumnStyling]] = None,
     ) -> None:
         """Constructor for Base Search Result Column.
 
@@ -37,26 +35,14 @@
         self._data_column = data_column
         self.__styling = (
             ResultColumnStyling(color_spec=styling)
             if isinstance(styling, Palette)
             else styling
         )
 
-    @property
-    def _api_type(self) -> str:
-        """Returns API type argument value.
-
-        All Select Layout Items must now have the _API_TYPE defined.
-        """
-        if self._API_TYPE is None:
-            raise NotImplementedError(
-                f"Class {self.__class__.__name__}._API_TYPE not defined."
-            )
-        return self._API_TYPE
-
     def _build_extra_inputs(self) -> Mapping[str, Any]:
         """Method used to build extra fields."""
         return {}
 
     def validate(self, *, data: pd.DataFrame) -> None:
         """Validate if data has the right columns.
 
@@ -68,19 +54,18 @@
         """
         if isinstance(self._data_column, str) and self._data_column not in data.columns:
             raise SearchValidateNoDataColumnError(data_column=self._data_column)
 
         if self.__styling is not None:
             self.__styling.validate(data=data)
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            self._api_type,
-            dataKey=build_templated_strings(items=self._data_column),
-            styling=self.__styling.build() if self.__styling is not None else None,
+        return {
+            "dataKey": build_templated_strings(items=self._data_column),
+            "styling": self.__styling.build() if self.__styling is not None else None,
             **self._build_extra_inputs(),
-        )
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/results/build_result.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/search/results/build_result.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 """Specs for build Search result."""
 
 from typing import Any
+from typing import Dict
 
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.search.results.number import ResultNumberItem
 from engineai.sdk.dashboard.widgets.search.results.text import ResultTextItem
 
 from .typing import ResultItemType
 
 
-def build_search_result(item: ResultItemType) -> Any:
+def build_search_result(item: ResultItemType) -> Dict[str, Any]:
     """Builds spec for dashboard API.
 
     Args:
         item: item spec
 
     Returns:
         Input object for Dashboard API
     """
-    return generate_input(
-        "SearchWidgetResultColumnUnionInput", **{_get_input_key(item): item.build()}
-    )
+    return {**{_get_input_key(item): item.build()}}
 
 
 def _get_input_key(item: ResultItemType) -> str:
     if isinstance(item, ResultNumberItem):
         return "number"
     elif isinstance(item, ResultTextItem):
         return "text"
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/results/number.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/search/results/number.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,14 @@
 class ResultNumberItem(BaseResultItem):
     """Define number item for search results.
 
     Define a number item for search results, specifying the data column
     to display, formatting options, and styling options.
     """
 
-    _API_TYPE = "SearchWidgetResultColumnNumberInput"
-
     def __init__(
         self,
         data_column: TemplatedStringItem,
         formatting: Optional[NumberFormatting] = None,
         styling: Optional[Union[Palette, ResultNumberStyling]] = None,
     ) -> None:
         """Constructor for ResultNumberItem.
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/results/styling/base_styling.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/search/results/styling/base_styling.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 """Spec for Search Widget Result Column Style."""
 
 from typing import Any
+from typing import Dict
 from typing import Optional
 
 import pandas as pd
 
 from engineai.sdk.dashboard.styling.color.discrete_map import DiscreteMap
 from engineai.sdk.dashboard.styling.color.gradient import Gradient
 from engineai.sdk.dashboard.styling.color.palette import Palette
 from engineai.sdk.dashboard.styling.color.spec import build_color_spec
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 
 from ...exceptions import SearchStylingMissingDataColumnError
 from ...exceptions import SearchValidateNoDataColumnError
 
 
 class ResultColumnStyling:
     """Spec for Search Widget Result Column Style."""
 
-    _API_TYPE: Optional[str] = None
-
     def __init__(
         self,
         *,
         color_spec: Optional[ColorSpec] = None,
         data_column: Optional[TemplatedStringItem] = None,
     ):
         """Construct for Search Widget Result Column Style.
@@ -43,26 +41,14 @@
             and isinstance(color_spec, (DiscreteMap, Gradient))
             and data_column is None
         ):
             raise SearchStylingMissingDataColumnError()
         self.__color_spec = color_spec or Palette.AQUA_GREEN
         self.__data_column = data_column
 
-    @property
-    def _api_type(self) -> str:
-        """Returns styling API type argument value.
-
-        All Select Layout Items must now have the _API_TYPE defined.
-        """
-        if self._API_TYPE is None:
-            raise NotImplementedError(
-                f"Class {self.__class__.__name__}._API_TYPE not defined."
-            )
-        return self._API_TYPE
-
     def validate(
         self,
         *,
         data: pd.DataFrame,
     ) -> None:
         """Validate if data has the right columns.
 
@@ -76,23 +62,21 @@
             isinstance(self.__data_column, str)
             and self.__data_column not in data.columns
         ):
             raise SearchValidateNoDataColumnError(data_column=self.__data_column)
 
         # TODO: Validate abstractLinks if used (widgetField, f.e)
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            self._api_type,
-            chip=generate_input(
-                "SearchWidgetResultColumnChipStylingInput",
-                colorSpec=build_color_spec(spec=self.__color_spec)
+        return {
+            "chip": {
+                "colorSpec": build_color_spec(spec=self.__color_spec)
                 if self.__color_spec
                 else None,
-                dataKey=build_templated_strings(items=self.__data_column),
-            ),
-        )
+                "dataKey": build_templated_strings(items=self.__data_column),
+            }
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/results/styling/number.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/search/results/styling/number.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,9 +38,7 @@
                     ),
                 ],
             )
 
             Dashboard(content=search_widget)
             ```
     """
-
-    _API_TYPE = "SearchWidgetResultColumnNumberStylingUnionInput"
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/results/styling/text.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/search/results/styling/text.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,9 +43,7 @@
                     ),
                 ],
             )
 
             Dashboard(content=search_widget)
             ```
     """
-
-    _API_TYPE = "SearchWidgetResultColumnTextStylingUnionInput"
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/results/text.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/search/results/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,14 @@
 class ResultTextItem(BaseResultItem):
     """Define text item for search results.
 
     Define a text item for search results, specifying the data column
     to display, whether it's searchable, and styling options.
     """
 
-    _API_TYPE = "SearchWidgetResultColumnTextInput"
-
     def __init__(
         self,
         data_column: TemplatedStringItem,
         searchable: bool = True,
         styling: Optional[Union[Palette, ResultTextStyling]] = None,
     ) -> None:
         """Constructor for ResultTextItem.
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/search.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/search/search.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """Specs for Search Widget."""
 
 import warnings
 from typing import Any
+from typing import Dict
 from typing import Iterable
 from typing import List
 from typing import Optional
 from typing import Union
 from typing import get_args
 
 import pandas as pd
 
 from engineai.sdk.dashboard.data.decorator import DataSource
 from engineai.sdk.dashboard.data.http import Http
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.chart_utils import column_is_of_type
 from engineai.sdk.dashboard.widgets.search.results.number import ResultNumberItem
 from engineai.sdk.dashboard.widgets.search.results.text import ResultTextItem
 from engineai.sdk.dashboard.widgets.search.results.typing import ResultItemType
 
 from ..base import SelectableWidget
 from ..utils import build_data
@@ -37,14 +37,15 @@
     and placeholder text.
     """
 
     _WIDGET_API_TYPE = "search"
     _DEPENDENCY_ID = "__SEARCH_DATA_DEPENDENCY__"
     _DEFAULT_HEIGHT = 0.6
     _FORCE_HEIGHT = True
+    _FLUID_ROW_COMPATIBLE = True
 
     @type_check
     def __init__(
         self,
         *,
         data: Union[DataSource, pd.DataFrame, Http],
         selected_text_column: TemplatedStringItem,
@@ -190,31 +191,25 @@
             if (
                 not self.__has_searchable
                 and isinstance(item, ResultTextItem)
                 and item.searchable
             ):
                 self.__has_searchable = item.searchable
 
-    def _build_widget_input(self) -> Any:
+    def _build_widget_input(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "SearchWidgetInput",
-            placeholder=build_templated_strings(items=self.__placeholder),
-            data=build_data(path=self.dependency_id),
-            selectedValueLabel=build_templated_strings(
+        return {
+            "placeholder": build_templated_strings(items=self.__placeholder),
+            "data": build_data(path=self.dependency_id),
+            "selectedValueLabel": build_templated_strings(
                 items=f"{{{{{self.__selected_text_column}}}}}"
             ),
-            results=generate_input(
-                "SearchWidgetResultsInput",
-                columns=[
+            "results": {
+                "columns": [
                     build_search_result(result) for result in self.__search_columns
                 ],
-            ),
-        )
-
-    def build_widget_input(self) -> Any:
-        """Method to access the build from outside the class."""
-        return self._build_widget_input()
+            },
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/select/exceptions.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/select/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/select/group.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/select/group.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Specs for Select Widget Group."""
 from typing import Any
+from typing import Dict
 
 import pandas as pd
 
 from engineai.sdk.dashboard.base import AbstractFactory
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 
 from .exceptions import SelectValidateValueError
 
 
 class Group(AbstractFactory):
     """Constructor for Select Widget Group spec."""
 
@@ -38,18 +38,17 @@
         """
         if self.__group_column not in data.columns:
             raise SelectValidateValueError(
                 argument="group_column",
                 value=str(self.__group_column),
             )
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "SelectWidgetGroupingInput",
-            groupKey=build_templated_strings(items=self.__group_column),
-            showGroupOnSelection=self.__show_group_when_selected,
-        )
+        return {
+            "groupKey": build_templated_strings(items=self.__group_column),
+            "showGroupOnSelection": self.__show_group_when_selected,
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/select/select.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/select/select.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Spec for Select widget."""
 
 from typing import Any
+from typing import Dict
 from typing import Optional
 from typing import Union
 
 import pandas as pd
 
 from engineai.sdk.dashboard.data import DataSource
 from engineai.sdk.dashboard.data.http import Http
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.utils import build_data
 
 from ..base import SelectableWidget
 from .exceptions import SelectValidateUniqueIDError
 from .exceptions import SelectValidateValueError
 from .group import Group
 
@@ -28,14 +28,15 @@
     default selection, label column, widget ID, label text,
     grouping, and label display options.
     """
 
     _DEPENDENCY_ID = "__SELECT_DATA_DEPENDENCY__"
 
     _WIDGET_API_TYPE = "select"
+    _FLUID_ROW_COMPATIBLE = True
 
     _DEFAULT_HEIGHT = 0.5
     _FORCE_HEIGHT = True
 
     @type_check
     def __init__(
         self,
@@ -142,39 +143,31 @@
                 argument="label_column",
                 value=self.__label_column,
             )
 
         if self.__group is not None:
             self.__group.validate(data)
 
-    def _build_widget_input(self) -> Any:
+    def _build_widget_input(self) -> Dict[str, Any]:
         """Builds spec for dashboard API.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "SelectWidgetInput",
-            option=generate_input(
-                "SelectWidgetOptionInput",
-                idKey=build_templated_strings(items=self.__id_column),
-                labelKey=build_templated_strings(items=self.__label_column),
-                grouping=self.__group.build() if self.__group is not None else None,
-            ),
-            label=generate_input(
-                "SelectWidgetLabelInput",
-                text=build_templated_strings(items=self.__label),
-                isOutside=self.__label_outside,
-            ),
-            initialState=generate_input(
-                "SelectStateInput",
-                preselectFirst=True,
-                selected=[self.__default_selection]
+        return {
+            "option": {
+                "idKey": build_templated_strings(items=self.__id_column),
+                "labelKey": build_templated_strings(items=self.__label_column),
+                "grouping": self.__group.build() if self.__group is not None else None,
+            },
+            "label": {
+                "text": build_templated_strings(items=self.__label),
+                "isOutside": self.__label_outside,
+            },
+            "initialState": {
+                "preselectFirst": True,
+                "selected": [self.__default_selection]
                 if self.__default_selection is not None
                 else [],
-            ),
-            data=build_data(self.dependency_id),
-        )
-
-    def build_widget_input(self) -> Any:
-        """Method to access the build from outside the class."""
-        return self._build_widget_input()
+            },
+            "data": build_data(self.dependency_id),
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/__init__.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,28 @@
 """Specs for TableGrid Widget."""
+from engineai.sdk.dashboard.enum.align import HorizontalAlignment
+from engineai.sdk.dashboard.widgets.components.charts.tooltip import CategoryTooltipItem
+from engineai.sdk.dashboard.widgets.components.charts.tooltip import CountryTooltipItem
+from engineai.sdk.dashboard.widgets.components.charts.tooltip import (
+    CountryTooltipItemStylingFlag,
+)
+from engineai.sdk.dashboard.widgets.components.charts.tooltip import DatetimeTooltipItem
+from engineai.sdk.dashboard.widgets.components.charts.tooltip import NumberTooltipItem
+from engineai.sdk.dashboard.widgets.components.charts.tooltip import TextTooltipItem
+from engineai.sdk.dashboard.widgets.components.items.tooltip.stacked_bar import (
+    StackedBarTooltipItem,
+)
 from engineai.sdk.dashboard.widgets.components.items.tooltip.tooltip import ChartTooltip
 
 from .columns.items.category import CategoryColumn
 from .columns.items.charts.area import AreaChartColumn
 from .columns.items.charts.column import ColumnChartColumn
 from .columns.items.charts.line import LineChartColumn
 from .columns.items.charts.stack_bar import StackedBarColumn
+from .columns.items.charts.stack_bar import StackedBarTooltip
 from .columns.items.country import CountryColumn
 from .columns.items.country import FlagPositions
 from .columns.items.datetime import DatetimeColumn
 from .columns.items.number import NumberColumn
 from .columns.items.range import RangeColumn
 from .columns.items.text import TextColumn
 from .columns.items.url_column import UrlColumn
@@ -23,15 +36,14 @@
 from .columns.styling.font import FontStyling
 from .columns.styling.icon import IconStyling
 from .columns.styling.line import LineChartStyling
 from .columns.styling.range import RangeShape
 from .columns.styling.range import RangeStyling
 from .columns.styling.split_bar import SplitBarStyling
 from .columns.styling.stacked_bar import StackedBarStyling
-from .enums import HorizontalAlignment
 from .group import Group
 from .header import Header
 from .initial_state import InitialState
 from .styling import TableStyling
 from .table import Table
 
 __all__ = [
@@ -66,14 +78,22 @@
     "IconStyling",
     "DotStyling",
     "FontStyling",
     "LineChartStyling",
     "SplitBarStyling",
     "RangeStyling",
     "StackedBarStyling",
+    "CountryTooltipItemStylingFlag",
     # enums,"
     "HorizontalAlignment",
     "RangeShape",
     "FlagPositions",
     # tooltip
     "ChartTooltip",
+    "StackedBarTooltip",
+    "StackedBarTooltipItem",
+    "CategoryTooltipItem",
+    "DatetimeTooltipItem",
+    "NumberTooltipItem",
+    "TextTooltipItem",
+    "CountryTooltipItem",
 ]
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/base.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/items/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Base spec shared by all column types."""
 
 from abc import abstractmethod
 from typing import Any
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 import pandas as pd
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.abstract import AbstractFactoryLinkItemsHandler
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.table.columns.items.exceptions import (
     TableColumnDataColumnNotFoundError,
 )
 from engineai.sdk.dashboard.widgets.table.columns.items.exceptions import (
     TableColumnMissingLabelError,
 )
 
@@ -158,30 +158,29 @@
 
         Returns:
             str: column label
         """
         return self.__label
 
     @abstractmethod
-    def _build_column(self) -> Any:
+    def _build_column(self) -> Dict[str, Any]:
         """Build Column input."""
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Builds spec for dashboard API.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "TableColumnInput",
-            dataKey=build_templated_strings(items=self._data_column),
-            columnId=self.item_id,
-            label=build_templated_strings(items=self.__label),
-            fixed=False,
-            tooltipText=[
+        return {
+            "dataKey": build_templated_strings(items=self._data_column),
+            "columnId": self.item_id,
+            "label": build_templated_strings(items=self.__label),
+            "fixed": False,
+            "tooltipText": [
                 build_templated_strings(items=tooltip)
                 for tooltip in self.__tooltip_text
             ],
-            hidingPriority=self.__hiding_priority,
-            minWidth=self.__min_width,
-            columnType=self._build_column(),
-        )
+            "hidingPriority": self.__hiding_priority,
+            "minWidth": self.__min_width,
+            "columnType": self._build_column(),
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/category.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/items/category.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Specification for Category Columns in Table widget."""
 
 from typing import Any
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 import pandas as pd
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import MapperFormatting
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.table.columns.items.exceptions import (
     TableCategoryColumnMappingError,
 )
 from engineai.sdk.dashboard.widgets.table.enums import HorizontalAlignment
 
 from ..styling.cell import CellStyling
 from ..styling.country_flag import CountryFlagStyling
@@ -142,30 +142,26 @@
 
         if len(missing_formatting) > 0:
             raise TableCategoryColumnMappingError(
                 missing_formatting=missing_formatting,
                 data_column=self.data_column,
             )
 
-    def _build_styling(self) -> Any:
-        column_styling = None
-        if self.__styling:
-            column_styling = generate_input(
-                "TableCategoryColumnStylingInput",
-                **build_styling_input(
-                    data_column=self.data_column, styling=self.__styling
-                ),
+    def _build_styling(self) -> Dict[str, Any]:
+        return (
+            None
+            if self.__styling is None
+            else build_styling_input(
+                data_column=self.data_column, styling=self.__styling
             )
-        return column_styling
-
-    def _build_column(self) -> Any:
-        return generate_input(
-            "TableColumnTypeInput",
-            categoryColumn=generate_input(
-                "TableCategoryColumnInput",
-                sortable=self.__sortable,
-                formatting=self.__formatting.build(),
-                align=self.__align.value,
-                styling=self._build_styling(),
-                optional=self._optional,
-            ),
         )
+
+    def _build_column(self) -> Dict[str, Any]:
+        return {
+            "categoryColumn": {
+                "sortable": self.__sortable,
+                "formatting": self.__formatting.build(),
+                "align": self.__align.value,
+                "styling": self._build_styling(),
+                "optional": self._optional,
+            }
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/charts/area.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/items/charts/area.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """Specification for Area Chart Column in Table widget."""
 
 from typing import Any
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 import pandas as pd
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import NumberFormatting
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.styling import color
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.items.tooltip.tooltip import ChartTooltip
 
 from ...styling.area import AreaChartStyling
 from .base import ChartColumn
 from .base import ReferenceLineType
 
 
@@ -111,30 +111,28 @@
         )
         self.__sortable = sortable
         self.__formatting = formatting if formatting else NumberFormatting()
         self.__display_first_value = display_first_value
         self.__display_last_value = display_last_value
         self.__tooltip = tooltip
 
-    def _build_column(self) -> Any:
-        return generate_input(
-            "TableColumnTypeInput",
-            areaChartColumn=generate_input(
-                "TableAreaChartColumnInput",
-                formatting=self.__formatting.build(),
-                styling=self._build_styling(),
-                displayFirstValue=self.__display_first_value,
-                displayLastValue=self.__display_last_value,
-                valueKey=build_templated_strings(items=self.data_key),
-                referenceLine=self.reference_line.build()
+    def _build_column(self) -> Dict[str, Any]:
+        return {
+            "areaChartColumn": {
+                "formatting": self.__formatting.build(),
+                "styling": self._build_styling(),
+                "displayFirstValue": self.__display_first_value,
+                "displayLastValue": self.__display_last_value,
+                "valueKey": build_templated_strings(items=self.data_key),
+                "referenceLine": self.reference_line.build()
                 if self.reference_line
                 else None,
-                sortable=self.__sortable,
-                optional=self._optional,
-                tooltip=self.__tooltip.build() if self.__tooltip else None,
-            ),
-        )
+                "sortable": self.__sortable,
+                "optional": self._optional,
+                "tooltip": self.__tooltip.build() if self.__tooltip else None,
+            }
+        }
 
     def _custom_validation(self, *, data: pd.DataFrame) -> None:
         super()._custom_validation(data=data)
         if self.__tooltip:
             self.__tooltip.validate(data=data)
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/charts/base.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/items/charts/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         if reference_line is None:
             self.__reference_line = None
         elif isinstance(reference_line, (DataField)):
             self.__reference_line = InternalDataField(reference_line)
         else:
             self.__reference_line = InternalDataField(str(reference_line))
 
-    def _build_styling(self) -> Any:
+    def _build_styling(self) -> Dict[str, Any]:
         return None if self.styling is None else self.styling.build()
 
     def _validate_list_row_data(self, *, row_data: List[Dict[str, Any]]) -> None:
         for value in row_data:
             if not isinstance(value, dict):
                 raise TableDataColumnValueTypeError(
                     data_column=self.data_column, value=value
@@ -121,15 +121,14 @@
             raise TableDataColumnValueKeyError(
                 data_column=self.data_column, data_key=self.data_key
             )
         if self.styling:
             self.styling.validate(data=row_data)
 
             styling_data_column = self.styling.data_column
-
             if styling_data_column is not None:
                 if len(row_data[str(self.data_key)]) != len(
                     row_data[str(styling_data_column)]
                 ):
                     raise TableColumnChartIncorrectLengthError(
                         data_column=self.data_column
                     )
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/charts/column.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/items/charts/column.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """Specification for Column Chart columns in Table widget."""
 
 from typing import Any
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 import pandas as pd
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import NumberFormatting
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.styling import color
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.items.tooltip.tooltip import ChartTooltip
 
 from ...styling.column import ColumnChartStyling
 from .base import ChartColumn
 from .base import ReferenceLineType
 
 
@@ -112,30 +112,28 @@
         )
         self.__formatting = formatting if formatting else NumberFormatting()
         self.__display_first_value = display_first_value
         self.__display_last_value = display_last_value
         self.__sortable = sortable
         self.__tooltip = tooltip
 
-    def _build_column(self) -> Any:
-        return generate_input(
-            "TableColumnTypeInput",
-            columnChartColumn=generate_input(
-                "TableColumnChartColumnInput",
-                formatting=self.__formatting.build(),
-                styling=self._build_styling(),
-                displayFirstValue=self.__display_first_value,
-                displayLastValue=self.__display_last_value,
-                referenceLine=self.reference_line.build()
+    def _build_column(self) -> Dict[str, Any]:
+        return {
+            "columnChartColumn": {
+                "formatting": self.__formatting.build(),
+                "styling": self._build_styling(),
+                "displayFirstValue": self.__display_first_value,
+                "displayLastValue": self.__display_last_value,
+                "referenceLine": self.reference_line.build()
                 if self.reference_line
                 else None,
-                valueKey=build_templated_strings(items=self.data_key),
-                sortable=self.__sortable,
-                optional=self._optional,
-                tooltip=self.__tooltip.build() if self.__tooltip else None,
-            ),
-        )
+                "valueKey": build_templated_strings(items=self.data_key),
+                "sortable": self.__sortable,
+                "optional": self._optional,
+                "tooltip": self.__tooltip.build() if self.__tooltip else None,
+            }
+        }
 
     def _custom_validation(self, *, data: pd.DataFrame) -> None:
         super()._custom_validation(data=data)
         if self.__tooltip:
             self.__tooltip.validate(data=data)
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/charts/line.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/items/charts/line.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """Specification for line chart columns in Table widget."""
 
 from typing import Any
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 import pandas as pd
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import NumberFormatting
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.styling import color
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.items.tooltip.tooltip import ChartTooltip
 
 from ...styling.line import LineChartStyling
 from .base import ChartColumn
 from .base import ReferenceLineType
 
 
@@ -113,30 +113,28 @@
         )
         self.__formatting = formatting if formatting else NumberFormatting()
         self.__display_first_value = display_first_value
         self.__display_last_value = display_last_value
         self.__sortable = sortable
         self.__tooltip = tooltip
 
-    def _build_column(self) -> Any:
-        return generate_input(
-            "TableColumnTypeInput",
-            lineChartColumn=generate_input(
-                "TableLineChartColumnInput",
-                formatting=self.__formatting.build(),
-                styling=self._build_styling(),
-                displayFirstValue=self.__display_first_value,
-                displayLastValue=self.__display_last_value,
-                referenceLine=self.reference_line.build()
+    def _build_column(self) -> Dict[str, Any]:
+        return {
+            "lineChartColumn": {
+                "formatting": self.__formatting.build(),
+                "styling": self._build_styling(),
+                "displayFirstValue": self.__display_first_value,
+                "displayLastValue": self.__display_last_value,
+                "referenceLine": self.reference_line.build()
                 if self.reference_line
                 else None,
-                valueKey=build_templated_strings(items=self.data_key),
-                sortable=self.__sortable,
-                optional=self._optional,
-                tooltip=self.__tooltip.build() if self.__tooltip else None,
-            ),
-        )
+                "valueKey": build_templated_strings(items=self.data_key),
+                "sortable": self.__sortable,
+                "optional": self._optional,
+                "tooltip": self.__tooltip.build() if self.__tooltip else None,
+            }
+        }
 
     def _custom_validation(self, *, data: pd.DataFrame) -> None:
         super()._custom_validation(data=data)
         if self.__tooltip:
             self.__tooltip.validate(data=data)
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/charts/stack_bar.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/items/country.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,135 +1,140 @@
-"""Specification for staked bar chart columns in Table widget."""
-
+"""Specification for Country Column in Table widget."""
+import enum
 from typing import Any
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
+import pandas as pd
+
 from engineai.sdk.dashboard.decorator import type_check
-from engineai.sdk.dashboard.formatting import NumberFormatting
+from engineai.sdk.dashboard.formatting import TextFormatting
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
-from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
+from engineai.sdk.dashboard.widgets.table.enums import HorizontalAlignment
+
+from ..styling.country_flag import CountryFlagStyling
+from ..styling.utils import build_styling_input
+from .base import Column
+
+
+class FlagPositions(enum.Enum):
+    """Country Column Flag Position Options.
+
+    Attributes:
+        LEFT: Flag at the left of the country name.
+        RIGHT: Flag at the right of the country name.
+        HIDDEN: Flag is hidden.
+    """
 
-from ...styling.stacked_bar import StackedBarStyling
-from .base import ChartColumn
+    LEFT: bool = True
+    RIGHT: bool = False
+    HIDDEN: None = None
 
 
-class StackedBarColumn(ChartColumn):
-    """Define table widget column: Stacked bar chart with data.
+class CountryColumn(Column):
+    """Define table widget column: Country information with data source.
 
-    Define a column in the table widget that displays a stacked bar chart,
-    including options for data, formatting, styling, and more.
+    Define a column in the table widget that displays country information,
+    including options for data source, label, formatting, and alignment.
     """
 
-    _ITEM_ID_TYPE: str = "STACKED_BAR"
+    _ITEM_ID_TYPE: str = "COUNTRY"
 
     @type_check
     def __init__(
         self,
         *,
         data_column: Union[str, WidgetField],
-        data_key: Union[str, WidgetField],
         label: Optional[Union[str, GenericLink]] = None,
-        styling: StackedBarStyling,
-        label_key: Optional[str] = None,
-        formatting: Optional[NumberFormatting] = None,
+        formatting: Optional[TextFormatting] = None,
+        flag_position: FlagPositions = FlagPositions.LEFT,
+        align: HorizontalAlignment = HorizontalAlignment.LEFT,
         hiding_priority: int = 0,
         tooltip_text: Optional[List[TemplatedStringItem]] = None,
         min_width: Optional[int] = None,
-        sortable: bool = True,
-        display_total_value: bool = True,
+        sortable: bool = False,
         optional: bool = False,
     ):
-        """Constructor for StackedBarColumn.
+        """Constructor for Country Column.
 
         Args:
             data_column: name of column in pandas dataframe(s) used for this widget.
-            data_key: key in object that contains the value for the stack bar chart.
-            label_key: key in object that contains the label for the stack bar chart.
+                Data in this column should be ISO 3166-1 alpha-2 country codes.
             label: label to be displayed for this column.
-            formatting: formatting spec.
-            styling: styling spec for stacked chart.
+            flag_position: position of country flag.
+            formatting: text formatting spec.
+            align: column alignment.
             hiding_priority: columns with lower hiding_priority are hidden first
                 if not all data can be shown.
             tooltip_text: info text to explain column. Each element of list is
                 displayed as a separate paragraph.
             min_width: min width of the column in pixels.
             sortable: determines if column can be sorted.
-            display_total_value: display total value after stacked bars chart.
             optional: flag to make the column optional if there is no Data for that
                 columns.
 
         Examples:
-            ??? example "Create a Table widget with StackedBarColumn"
+            ??? example "Create a Table widget with Country Column"
                 ```py linenums="1"
                 import pandas as pd
                 from engineai.sdk.dashboard.dashboard import Dashboard
                 from engineai.sdk.dashboard.widgets import table
                 data = pd.DataFrame(
                     {
-                        "stacked_data": [
-                            {"key": 10, "category": 1},
-                            {"key": 10, "category": 2},
-                        ],
+                        "country_code": ["US", "CA", "MX"],
                     },
                 )
-
-                color_spec = color.DiscreteMap(
-                        color.DiscreteMapValueItem(
-                            value=1, color=color.Palette.MINT_GREEN
-                        ),
-                        color.DiscreteMapValueItem(
-                            value=2, color=color.Palette.SUNSET_ORANGE
-                        ),
-                    ),
-                )
-
                 Dashboard(
                     content=table.Table(
                         data=data,
                         columns=[
-                            table.StackedBarColumn(
-                                data_column="stacked_data",
-                                data_key="key",
-                                styling=table.StackedBarStyling(
-                                    data_column="category",
-                                    color_spec=color_spec,
+                            table.CountryColumn(
+                                data_column="country_code",
                             ),
                         ],
                     )
                 )
                 ```
         """
         super().__init__(
             data_column=data_column,
-            data_key=data_key,
-            styling=styling,
             label=label,
             hiding_priority=hiding_priority,
             tooltip_text=tooltip_text,
             min_width=min_width,
-            reference_line=None,
             optional=optional,
         )
-        self.__formatting = formatting if formatting else NumberFormatting()
+        self.__align = align
+        self.__styling = (
+            None
+            if flag_position == FlagPositions.HIDDEN
+            else CountryFlagStyling(data_column=data_column, left=flag_position.value)
+        )
         self.__sortable = sortable
-        self.__display_total_value = display_total_value
-        self.__label_key = label_key
+        self.__formatting = formatting if formatting else TextFormatting()
+
+    def _custom_validation(self, *, data: pd.DataFrame) -> None:
+        pass
 
-    def _build_column(self) -> Any:
-        return generate_input(
-            "TableColumnTypeInput",
-            stackedBarColumn=generate_input(
-                "TableStackedBarColumnInput",
-                formatting=self.__formatting.build(),
-                styling=self._build_styling(),
-                valueKey=build_templated_strings(items=self.data_key),
-                labelKey=build_templated_strings(items=self.__label_key),
-                sortable=self.__sortable,
-                displayTotalValue=self.__display_total_value,
-                optional=self._optional,
-            ),
+    def _build_styling(self) -> Dict[str, Any]:
+        return (
+            None
+            if self.__styling is None
+            else build_styling_input(
+                data_column=self.data_column, styling=self.__styling
+            )
         )
+
+    def _build_column(self) -> Dict[str, Any]:
+        return {
+            "countryColumn": {
+                "sortable": self.__sortable,
+                "formatting": self.__formatting.build(),
+                "align": self.__align.value,
+                "styling": self._build_styling(),
+                "optional": self._optional,
+            }
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/country.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/items/text.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,102 +1,103 @@
-"""Specification for Country Column in Table widget."""
-import enum
+"""Specification for text columns."""
+
 from typing import Any
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 import pandas as pd
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import TextFormatting
-from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.typing import GenericLink
+from engineai.sdk.dashboard.links.widget_field import WidgetField
+from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.table.enums import HorizontalAlignment
 
+from ..styling.cell import CellStyling
 from ..styling.country_flag import CountryFlagStyling
+from ..styling.dot import DotStyling
+from ..styling.font import FontStyling
+from ..styling.icon import IconStyling
 from ..styling.utils import build_styling_input
 from .base import Column
 
+TextColumnStyling = Union[
+    CellStyling,
+    CountryFlagStyling,
+    DotStyling,
+    FontStyling,
+    IconStyling,
+]
 
-class FlagPositions(enum.Enum):
-    """Country Column Flag Position Options.
 
-    Attributes:
-        LEFT: Flag at the left of the country name.
-        RIGHT: Flag at the right of the country name.
-        HIDDEN: Flag is hidden.
+class TextColumn(Column):
+    """Define table widget column: Text data with data source.
+
+    Define a column in the table widget that displays text data,
+    including options for data source, label, formatting, styling,
+    and alignment.
     """
 
-    LEFT: bool = True
-    RIGHT: bool = False
-    HIDDEN: None = None
-
-
-class CountryColumn(Column):
-    """Define table widget column: Country information with data source.
-
-    Define a column in the table widget that displays country information,
-    including options for data source, label, formatting, and alignment.
-    """
-
-    _ITEM_ID_TYPE: str = "COUNTRY"
+    _ITEM_ID_TYPE: str = "TEXT"
 
     @type_check
     def __init__(
         self,
         *,
         data_column: Union[str, WidgetField],
         label: Optional[Union[str, GenericLink]] = None,
         formatting: Optional[TextFormatting] = None,
-        flag_position: FlagPositions = FlagPositions.LEFT,
+        styling: Optional[Union[Palette, TextColumnStyling]] = None,
         align: HorizontalAlignment = HorizontalAlignment.LEFT,
         hiding_priority: int = 0,
         tooltip_text: Optional[List[TemplatedStringItem]] = None,
         min_width: Optional[int] = None,
-        sortable: bool = False,
+        sortable: bool = True,
         optional: bool = False,
     ):
-        """Constructor for Country Column.
+        """Constructor for TextColumn.
 
         Args:
             data_column: name of column in pandas dataframe(s) used for this widget.
-                Data in this column should be ISO 3166-1 alpha-2 country codes.
             label: label to be displayed for this column.
-            flag_position: position of country flag.
-            formatting: text formatting spec.
-            align: column alignment.
+            formatting: formatting spec.
+            styling: styling spec for column. One of CellStyling, CountryFlagStyling
+                DotStyling, FontStyling or IconStyling.
+            align: align text.
             hiding_priority: columns with lower hiding_priority are hidden first
                 if not all data can be shown.
-            tooltip_text: info text to explain column. Each element of list is
-                displayed as a separate paragraph.
+            tooltip_text: info text to explain column.
+                Each element of list is displayed as a separate paragraph.
             min_width: min width of the column in pixels.
             sortable: determines if column can be sorted.
             optional: flag to make the column optional if there is no Data for that
                 columns.
 
         Examples:
-            ??? example "Create a Table widget with Country Column"
+            ??? example "Create a Table widget with TextColumn"
                 ```py linenums="1"
                 import pandas as pd
                 from engineai.sdk.dashboard.dashboard import Dashboard
                 from engineai.sdk.dashboard.widgets import table
                 data = pd.DataFrame(
                     {
-                        "country_code": ["US", "CA", "MX"],
-                    },
+                        "text": "Apple has ticker=AAPL",
+                    }
                 )
                 Dashboard(
                     content=table.Table(
                         data=data,
                         columns=[
-                            table.CountryColumn(
-                                data_column="country_code",
+                            table.TextColumn(
+                                data_column="text",
+                                ),
                             ),
                         ],
                     )
                 )
                 ```
         """
         super().__init__(
@@ -105,40 +106,45 @@
             hiding_priority=hiding_priority,
             tooltip_text=tooltip_text,
             min_width=min_width,
             optional=optional,
         )
         self.__align = align
         self.__styling = (
-            None
-            if flag_position == FlagPositions.HIDDEN
-            else CountryFlagStyling(data_column=data_column, left=flag_position.value)
+            CellStyling(color_spec=styling) if isinstance(styling, Palette) else styling
         )
         self.__sortable = sortable
         self.__formatting = formatting if formatting else TextFormatting()
 
+    def prepare(self) -> None:
+        """Prepare data column."""
+        if self.__styling is not None:
+            self.__styling.prepare(self._data_column)
+
     def _custom_validation(self, *, data: pd.DataFrame) -> None:
-        pass
+        """Custom validation for each columns to implement.
 
-    def _build_styling(self) -> Any:
-        column_styling = None
-        if self.__styling:
-            column_styling = generate_input(
-                "TableCountryColumnStylingInput",
-                **build_styling_input(
-                    data_column=self.data_column, styling=self.__styling
-                ),
-            )
-        return column_styling
+        Args:
+            data: pandas dataframe which will be used for table.
+        """
+        if self.__styling is not None:
+            self.__styling.validate(data=data)
 
-    def _build_column(self) -> Any:
-        return generate_input(
-            "TableColumnTypeInput",
-            countryColumn=generate_input(
-                "TableCountryColumnInput",
-                sortable=self.__sortable,
-                formatting=self.__formatting.build(),
-                align=self.__align.value,
-                styling=self._build_styling(),
-                optional=self._optional,
-            ),
+    def _build_styling(self) -> Dict[str, Any]:
+        return (
+            None
+            if self.__styling is None
+            else build_styling_input(
+                data_column=self.data_column, styling=self.__styling
+            )
         )
+
+    def _build_column(self) -> Dict[str, Any]:
+        return {
+            "textColumn": {
+                "sortable": self.__sortable,
+                "formatting": self.__formatting.build(),
+                "align": self.__align.value,
+                "styling": self._build_styling(),
+                "optional": self._optional,
+            }
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/datetime.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/items/datetime.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Specification for text columns."""
 
 from typing import Any
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 import pandas as pd
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import DateTimeFormatting
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.table.enums import HorizontalAlignment
 
 from ..styling.cell import CellStyling
 from ..styling.country_flag import CountryFlagStyling
 from ..styling.dot import DotStyling
 from ..styling.font import FontStyling
 from ..styling.utils import build_styling_input
@@ -133,30 +133,26 @@
             pd.to_datetime(data[self.data_column], unit="ms")
         except ValueError as e:
             raise TableDatetimeColumnMappingError(data_column=self.data_column) from e
 
         if self.__styling:
             self.__styling.validate(data=data)
 
-    def _build_styling(self) -> Any:
-        column_styling = None
-        if self.__styling:
-            column_styling = generate_input(
-                "TableDateTimeColumnStylingInput",
-                **build_styling_input(
-                    data_column=self.data_column, styling=self.__styling
-                ),
+    def _build_styling(self) -> Dict[str, Any]:
+        return (
+            None
+            if self.__styling is None
+            else build_styling_input(
+                data_column=self.data_column, styling=self.__styling
             )
-        return column_styling
-
-    def _build_column(self) -> Any:
-        return generate_input(
-            "TableColumnTypeInput",
-            dateTimeColumn=generate_input(
-                "TableDateTimeColumnInput",
-                sortable=self.__sortable,
-                formatting=self.__formatting.build(),
-                align=self.__align.value,
-                styling=self._build_styling(),
-                optional=self._optional,
-            ),
         )
+
+    def _build_column(self) -> Dict[str, Any]:
+        return {
+            "dateTimeColumn": {
+                "sortable": self.__sortable,
+                "formatting": self.__formatting.build(),
+                "align": self.__align.value,
+                "styling": self._build_styling(),
+                "optional": self._optional,
+            }
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/exceptions.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/items/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/number.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/items/number.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Specification for text columns."""
 
 from typing import Any
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 import pandas as pd
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import NumberFormatting
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.table.enums import HorizontalAlignment
 
 from ..styling.arrow import ArrowStyling
 from ..styling.cell import CellStyling
 from ..styling.color_bar import ColorBarStyling
 from ..styling.country_flag import CountryFlagStyling
 from ..styling.dot import DotStyling
@@ -141,30 +141,26 @@
 
         Args:
             data: pandas dataframe which will be used for table.
         """
         if self.__styling is not None:
             self.__styling.validate(data=data)
 
-    def _build_styling(self) -> Any:
-        column_styling_spec = None
-        if self.__styling is not None:
-            column_styling_spec = generate_input(
-                "TableNumberColumnStylingInput",
-                **build_styling_input(
-                    data_column=self.data_column, styling=self.__styling
-                ),
+    def _build_styling(self) -> Dict[str, Any]:
+        return (
+            None
+            if self.__styling is None
+            else build_styling_input(
+                data_column=self.data_column, styling=self.__styling
             )
-        return column_styling_spec
-
-    def _build_column(self) -> Any:
-        return generate_input(
-            "TableColumnTypeInput",
-            numberColumn=generate_input(
-                "TableNumberColumnInput",
-                formatting=self.__formatting.build(),
-                align=self.__align.value,
-                sortable=self.__sortable,
-                styling=self._build_styling(),
-                optional=self._optional,
-            ),
         )
+
+    def _build_column(self) -> Dict[str, Any]:
+        return {
+            "numberColumn": {
+                "formatting": self.__formatting.build(),
+                "align": self.__align.value,
+                "styling": self._build_styling(),
+                "sortable": self.__sortable,
+                "optional": self._optional,
+            }
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/range.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/items/range.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Specification for range columns in Table widget."""
 
 from typing import Any
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 import pandas as pd
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.formatting import NumberFormatting
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.styling import color
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
-from engineai.sdk.dashboard.utils import generate_input
 
 from ..styling.range import RangeStyling
 from .base import Column
 from .exceptions import TableColumnDataTypeError
 from .exceptions import TableRangeColumnValueError
 
 
@@ -133,18 +133,16 @@
                         if field not in element:
                             raise TableRangeColumnValueError(
                                 data_column=self.data_column, key=field
                             )
         if self.__styling:
             self.__styling.validate(data=data)
 
-    def _build_column(self) -> Any:
-        return generate_input(
-            "TableColumnTypeInput",
-            rangeColumn=generate_input(
-                "TableRangeColumnInput",
-                formatting=self.__formatting.build(),
-                styling=self.__styling.build(),
-                sortable=self.__sortable,
-                optional=self._optional,
-            ),
-        )
+    def _build_column(self) -> Dict[str, Any]:
+        return {
+            "rangeColumn": {
+                "formatting": self.__formatting.build(),
+                "styling": self.__styling.build(),
+                "sortable": self.__sortable,
+                "optional": self._optional,
+            }
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/text.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/series/error_bar.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,154 +1,123 @@
-"""Specification for text columns."""
+"""Spec for error bar series of a Timeseries widget."""
 
 from typing import Any
-from typing import List
+from typing import Dict
 from typing import Optional
 from typing import Union
 
 import pandas as pd
 
 from engineai.sdk.dashboard.decorator import type_check
-from engineai.sdk.dashboard.formatting import TextFormatting
+from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.typing import GenericLink
-from engineai.sdk.dashboard.links.widget_field import WidgetField
 from engineai.sdk.dashboard.styling.color import Palette
-from engineai.sdk.dashboard.templated_string import TemplatedStringItem
-from engineai.sdk.dashboard.utils import generate_input
-from engineai.sdk.dashboard.widgets.table.enums import HorizontalAlignment
-
-from ..styling.cell import CellStyling
-from ..styling.country_flag import CountryFlagStyling
-from ..styling.dot import DotStyling
-from ..styling.font import FontStyling
-from ..styling.icon import IconStyling
-from ..styling.utils import build_styling_input
-from .base import Column
-
-TextColumnStyling = Union[
-    CellStyling,
-    CountryFlagStyling,
-    DotStyling,
-    FontStyling,
-    IconStyling,
-]
-
-
-class TextColumn(Column):
-    """Define table widget column: Text data with data source.
-
-    Define a column in the table widget that displays text data,
-    including options for data source, label, formatting, styling,
-    and alignment.
+from engineai.sdk.dashboard.templated_string import build_templated_strings
+from engineai.sdk.dashboard.widgets.components.charts.series.entities.country import (
+    CountryEntity,
+)
+from engineai.sdk.dashboard.widgets.components.charts.series.entities.typing import (
+    Entities,
+)
+from engineai.sdk.dashboard.widgets.components.charts.styling import (
+    ErrorBarSeriesStyling,
+)
+
+from ...components.charts.typing import TooltipItems
+from .base import TimeseriesBaseSeries
+
+
+class ErrorBarSeries(TimeseriesBaseSeries):
+    """Depict data variability with error bars in Timeseries.
+
+    Construct specifications for an error bar series within a Timeseries widget,
+    providing a visual representation of the variability or uncertainty
+    associated with data points. Each data point is depicted on the chart
+    along with error bars, which indicate the range of possible values or the
+    extent of deviation from a central value.
     """
 
-    _ITEM_ID_TYPE: str = "TEXT"
+    _INPUT_KEY = "errorBar"
+    _styling_class = ErrorBarSeriesStyling
 
     @type_check
     def __init__(
         self,
         *,
-        data_column: Union[str, WidgetField],
-        label: Optional[Union[str, GenericLink]] = None,
-        formatting: Optional[TextFormatting] = None,
-        styling: Optional[Union[Palette, TextColumnStyling]] = None,
-        align: HorizontalAlignment = HorizontalAlignment.LEFT,
-        hiding_priority: int = 0,
-        tooltip_text: Optional[List[TemplatedStringItem]] = None,
-        min_width: Optional[int] = None,
-        sortable: bool = True,
-        optional: bool = False,
+        low_data_column: Union[str, WidgetField],
+        high_data_column: Union[str, WidgetField],
+        name: Optional[Union[str, GenericLink]] = None,
+        styling: Optional[Union[Palette, ErrorBarSeriesStyling]] = None,
+        entity: Optional[Entities] = None,
+        show_in_legend: bool = True,
+        required: bool = True,
+        visible: bool = True,
+        right_axis: bool = False,
+        tooltips: Optional[TooltipItems] = None,
     ):
-        """Constructor for TextColumn.
+        """Constructor for ErrorBarSeries.
 
         Args:
-            data_column: name of column in pandas dataframe(s) used for this widget.
-            label: label to be displayed for this column.
-            formatting: formatting spec.
-            styling: styling spec for column. One of CellStyling, CountryFlagStyling
-                DotStyling, FontStyling or IconStyling.
-            align: align text.
-            hiding_priority: columns with lower hiding_priority are hidden first
-                if not all data can be shown.
-            tooltip_text: info text to explain column.
-                Each element of list is displayed as a separate paragraph.
-            min_width: min width of the column in pixels.
-            sortable: determines if column can be sorted.
-            optional: flag to make the column optional if there is no Data for that
-                columns.
-
-        Examples:
-            ??? example "Create a Table widget with TextColumn"
-                ```py linenums="1"
-                import pandas as pd
-                from engineai.sdk.dashboard.dashboard import Dashboard
-                from engineai.sdk.dashboard.widgets import table
-                data = pd.DataFrame(
-                    {
-                        "text": "Apple has ticker=AAPL",
-                    }
-                )
-                Dashboard(
-                    content=table.Table(
-                        data=data,
-                        columns=[
-                            table.TextColumn(
-                                data_column="text",
-                                ),
-                            ),
-                        ],
-                    )
-                )
-                ```
+            low_data_column: name of data column in pandas dataframe(s) used for the
+                low values of this series.
+            high_data_column: name of data column in pandas dataframe(s) used for the
+                high values of this series.
+            name: series name (shown in legend and tooltip).
+            styling: styling spec, by default uses the values from the sequential
+                palette.
+            entity: entity spec.
+            show_in_legend: whether to show series in legend or not.
+            required: Flag to make the Series mandatory. If required == True and no
+                Data the widget will show an error. If required==False and no Data,
+                the widget hides the Series.
+            visible: Flag to make the Series visible when chart is loaded.
+            right_axis: Flag to make the Series visible on the right axis.
+            tooltips: tooltip items to be displayed at Series level.
         """
         super().__init__(
-            data_column=data_column,
-            label=label,
-            hiding_priority=hiding_priority,
-            tooltip_text=tooltip_text,
-            min_width=min_width,
-            optional=optional,
+            name=name,
+            data_column=None,
+            show_in_legend=show_in_legend,
+            required=required,
+            visible=visible,
+            styling=ErrorBarSeriesStyling(color_spec=styling)
+            if isinstance(styling, Palette)
+            else styling,
+            entity=entity,
+            right_axis=right_axis,
+            tooltips=tooltips,
         )
-        self.__align = align
-        self.__styling = (
-            CellStyling(color_spec=styling) if isinstance(styling, Palette) else styling
+        self._low_data_column: Union[str, WidgetField] = (
+            low_data_column if isinstance(low_data_column, str) else low_data_column
+        )
+        self._high_data_column: Union[str, WidgetField] = (
+            high_data_column if isinstance(high_data_column, str) else high_data_column
         )
-        self.__sortable = sortable
-        self.__formatting = formatting if formatting else TextFormatting()
-
-    def prepare(self) -> None:
-        """Prepare data column."""
-        if self.__styling is not None:
-            self.__styling.prepare(self._data_column)
 
-    def _custom_validation(self, *, data: pd.DataFrame) -> None:
-        """Custom validation for each columns to implement.
+    def validate(self, *, data: pd.DataFrame) -> None:
+        """Validate if dataframe that will be used for series contains required columns.
 
         Args:
-            data: pandas dataframe which will be used for table.
+            data: pandas dataframe which will be used for table
         """
-        if self.__styling is not None:
-            self.__styling.validate(data=data)
+        super().validate(data=data)
+
+        self._validate_data_column(
+            data=data,
+            data_column=self._low_data_column,
+            data_column_name="low_data_column",
+        )
 
-    def _build_styling(self) -> Any:
-        column_styling = None
-        if self.__styling:
-            column_styling = generate_input(
-                "TableTextColumnStylingInput",
-                **build_styling_input(
-                    data_column=self.data_column, styling=self.__styling
-                ),
-            )
-        return column_styling
-
-    def _build_column(self) -> Any:
-        return generate_input(
-            "TableColumnTypeInput",
-            textColumn=generate_input(
-                "TableTextColumnInput",
-                sortable=self.__sortable,
-                formatting=self.__formatting.build(),
-                align=self.__align.value,
-                styling=self._build_styling(),
-                optional=self._optional,
-            ),
+        self._validate_data_column(
+            data=data,
+            data_column=self._high_data_column,
+            data_column_name="high_data_column",
         )
+
+        if self._entity is not None and isinstance(self._entity, CountryEntity):
+            self._entity.validate_country_code()
+
+    def _build_extra_inputs(self) -> Dict[str, Any]:
+        return {
+            "lowKey": build_templated_strings(items=self._low_data_column),
+            "highKey": build_templated_strings(items=self._high_data_column),
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/url_column.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/items/url_column.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Specification for url columns in Table widget."""
 
 from typing import Any
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 import pandas as pd
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.templated_string import DataField
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.actions.links import UrlLink
 
 from .base import Column
 
 
 class UrlColumn(Column):
     """Specifications for UrlColumn class."""
@@ -97,16 +97,11 @@
             data: pandas dataframe which will be used for table.
 
         Raises:
             ValueError: if data does not contain data_column for TableColumn
         """
         self.__url_link.validate(data=data, widget_class="Table")
 
-    def _build_column(self) -> Any:
-        actions = generate_input(
-            "TableActionColumnActionInput", hyperLink=self.__url_link.build()
-        )
-
-        return generate_input(
-            "TableColumnTypeInput",
-            actionColumn=generate_input("TableActionColumnInput", actions=actions),
-        )
+    def _build_column(self) -> Dict[str, Any]:
+        return {
+            "actionColumn": {"actions": {"hyperLink": self.__url_link.build()}},
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/area.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/styling/column.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,36 @@
-"""Specification for Area Chart Styling."""
+"""Specification for styling a column chart."""
 from typing import Optional
 from typing import Union
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 
 from .base import TableSparklineColumnStylingBase
 
 
-class AreaChartStyling(TableSparklineColumnStylingBase):
-    """Styling options for area chart column.
+class ColumnChartStyling(TableSparklineColumnStylingBase):
+    """Styling options for column chart column.
 
-    Specify the styling options for an area chart column in
+    Specify the styling options for a column chart column in
     the table widget, including color and data key.
     """
 
-    _API_TYPE = "SparkChartAreaStylingInput"
-
     @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_key: Optional[Union[str, WidgetField]] = None,
     ):
-        """Constructor for AreaChartStyling.
+        """Constructor for ColumnChartStyling.
 
         Args:
             data_key: Dictionary key, stored in data, that is used for chart.
                 By default, will use values of column to which styling is applied.
-            color_spec: spec for color of area chart.
+            color_spec: spec for color of column chart.
         """
         super().__init__(
             data_column=data_key,
             color_spec=color_spec,
         )
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/arrow.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/styling/arrow.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,14 @@
 class ArrowStyling(TableColumnStylingBase):
     """Styling options for arrow column.
 
     Specify the styling options for an arrow column in the
     table widget, including data column, mid value, and color.
     """
 
-    _API_TYPE = "TableColumnStylingArrowInput"
-
     @type_check
     def __init__(
         self,
         *,
         data_column: Optional[Union[str, WidgetField]] = None,
         mid: Union[float, int] = 0,
         color_spec: Optional[ColorSpec] = None,
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/base.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/styling/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,35 +5,32 @@
 from typing import Mapping
 from typing import Optional
 from typing import Union
 
 import pandas as pd
 
 from engineai.sdk.dashboard.decorator import type_check
-from engineai.sdk.dashboard.exceptions import ImproperlyConfiguredError
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.abstract import AbstractFactoryLinkItemsHandler
 from engineai.sdk.dashboard.styling.color import DiscreteMap
 from engineai.sdk.dashboard.styling.color import Gradient
 from engineai.sdk.dashboard.styling.color.spec import build_color_spec
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.table.columns.styling.exceptions import (
     TableColumnStylingValidationError,
 )
 from engineai.sdk.dashboard.widgets.table.columns.styling.exceptions import (
     TableColumnStylingValueError,
 )
 
 
 class TableColumnStylingBase(AbstractFactoryLinkItemsHandler):
     """Specification for Table Column Styling Base class."""
 
-    _API_TYPE: Optional[str] = None
     _API_DATA_KEY: Optional[str] = "dataKey"
 
     @type_check
     def __init__(
         self,
         *,
         color_spec: Optional[ColorSpec] = None,
@@ -62,26 +59,14 @@
         return (
             {"colorSpec": build_color_spec(spec=self.__color_spec)}
             if self.__color_spec is not None
             else {}
         )
 
     @property
-    def _api_type(self) -> str:
-        """Get API TYPE value."""
-        if self._API_TYPE is None:
-            raise ImproperlyConfiguredError(
-                f"Class {self.__class__.__name__} does not have the "
-                f"`api_type` configured. Please set "
-                f"{self.__class__.__name__}._API_TYPE or change the "
-                f"{self.__class__.__name__}.api_type property."
-            )
-        return self._API_TYPE
-
-    @property
     def data_column(
         self,
     ) -> Optional[Union[str, WidgetField]]:
         """Name of column used in pandas dataframe.
 
         Returns None if a single color is used.
 
@@ -124,25 +109,24 @@
                 )
 
     def _build_key_input(self) -> Mapping[str, Any]:
         return {
             self._API_DATA_KEY: build_templated_strings(items=self._data_column or " ")
         }
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Builds spec for dashboard API.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            self._api_type,
+        return {
             **self._build_key_input(),
             **self._build_color_spec(),
             **self._build_extra_inputs(),
-        )
+        }
 
 
 class TableSparklineColumnStylingBase(TableColumnStylingBase):
     """Specification for Table Sparkline Column Styling Base class."""
 
     _API_DATA_KEY: Optional[str] = "valueKey"
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/cell.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/styling/icon.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,39 @@
-"""Specification for styling a column with an arrow next to value."""
+"""Specification for styling a column with an icon to a value."""
 from typing import Any
 from typing import Dict
-from typing import Optional
 from typing import Union
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links import WidgetField
-from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 
 from .base import TableColumnStylingBase
 
 
-class CellStyling(TableColumnStylingBase):
-    """Styling options for table widget cell.
+class IconStyling(TableColumnStylingBase):
+    """Styling options for icon column.
 
-    Specify the styling options for a cell in the table widget,
-    including color, data column, and percentage fill.
+    Specify the styling options for an icon column in the
+    table widget, including data column and position.
     """
 
-    _API_TYPE = "TableColumnStylingCellInput"
-
     @type_check
     def __init__(
         self,
         *,
-        color_spec: ColorSpec,
-        data_column: Optional[Union[str, WidgetField]] = None,
-        percentage_fill: Optional[Union[float, int]] = 1,
+        data_column: Union[str, WidgetField],
+        left: bool = True,
     ):
-        """Constructor for CellStyling.
+        """Constructor for IconStyling.
 
         Args:
             data_column: id of column which values are used to determine behavior of
-                arrow. By default, will use values of column to which styling is
-                applied.
-            percentage_fill: how much of the cell should the color
-                fill. Default to 1, meaning the whole cell
-            color_spec: spec for color of arrows.
+                arrow.
+                By default, will use values of column to which styling is applied.
+            left: whether to put icon to the left (True) or right (False) of column
+                value.
         """
-        super().__init__(color_spec=color_spec, data_column=data_column)
-        self.__percentage_fill = percentage_fill
+        super().__init__(data_column=data_column, color_spec=None)
+        self.__left = left
 
     def _build_extra_inputs(self) -> Dict[str, Any]:
-        return {"percentageFill": self.__percentage_fill}
+        return {"left": self.__left}
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/color_bar.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/styling/color_bar.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,14 @@
     """Styling options for split color bar column.
 
     Specify the styling options for a color bar column in the
     table widget, including color, data column, direction,
     min/max values, and percentage fill.
     """
 
-    _API_TYPE = "TableColumnStylingColorBarInput"
-
     @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_column: Optional[Union[str, WidgetField]] = None,
         left_to_right: bool = True,
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/column.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/styling/line.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,36 @@
-"""Specification for styling a column chart."""
+"""Specification for styling a line chart."""
 from typing import Optional
 from typing import Union
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 
 from .base import TableSparklineColumnStylingBase
 
 
-class ColumnChartStyling(TableSparklineColumnStylingBase):
-    """Styling options for column chart column.
+class LineChartStyling(TableSparklineColumnStylingBase):
+    """Styling options for line chart column.
 
-    Specify the styling options for a column chart column in
+    Specify the styling options for a line chart column in
     the table widget, including color and data key.
     """
 
-    _API_TYPE = "SparkChartColumnStylingInput"
-
     @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_key: Optional[Union[str, WidgetField]] = None,
     ):
-        """Constructor for ColumnChartStyling.
+        """Constructor for LineChartStyling.
 
         Args:
             data_key: Dictionary key, stored in data, that is used for chart.
                 By default, will use values of column to which styling is applied.
-            color_spec: spec for color of column chart.
+            color_spec: spec for color of line chart.
         """
         super().__init__(
             data_column=data_key,
             color_spec=color_spec,
         )
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/country_flag.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/styling/range.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,52 @@
-"""Specification for styling a column with a country flag to a value."""
+"""Specification for styling a column with an arrow next to value."""
+import enum
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Union
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links import WidgetField
+from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 
 from .base import TableColumnStylingBase
 
 
-class CountryFlagStyling(TableColumnStylingBase):
-    """Styling options for country flag column.
+class RangeShape(enum.Enum):
+    """Range shape options."""
+
+    CIRCLE = "CIRCLE"
+    RECTANGLE = "RECTANGLE"
 
-    Specify the styling options for a country flag column
-    in the table widget, including position and data column.
-    """
 
-    _API_TYPE = "TableColumnStylingCountryFlagInput"
+class RangeStyling(TableColumnStylingBase):
+    """Styling options for range column.
+
+    Specify the styling options for a range column in the
+    table widget, including color, data column, and shape.
+    """
 
     @type_check
     def __init__(
         self,
         *,
-        left: bool = True,
+        color_spec: ColorSpec,
         data_column: Optional[Union[str, WidgetField]] = None,
+        shape: RangeShape = RangeShape.CIRCLE,
     ):
-        """Constructor for CountryFlagStyling.
+        """Constructor for RangeStyling.
 
         Args:
             data_column: id of column which values are used to determine behavior of
                 arrow.
-                By default, will use values of column to which styling is applied.
-            left: whether to put flag to the left (True) or right (False) of column
-                value.
+            color_spec: spec for color of range value.
+            shape: shape of range indicator.
         """
-        super().__init__(data_column=data_column, color_spec=None)
-        self.__left = left
+        super().__init__(
+            data_column=data_column,
+            color_spec=color_spec,
+        )
+        self.__shape = shape
 
     def _build_extra_inputs(self) -> Dict[str, Any]:
-        return {"left": self.__left}
+        return {"shape": self.__shape.value}
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/dot.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/styling/dot.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 class DotStyling(TableColumnStylingBase):
     """Styling options for dot column.
 
     Specify the styling options for a dot column in the table
     widget, including color and data column.
     """
 
-    _API_TYPE = "TableColumnStylingDotInput"
-
     @type_check
     def __init__(
         self,
         *,
         color_spec: Optional[ColorSpec] = None,
         data_column: Optional[Union[str, WidgetField]] = None,
     ):
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/exceptions.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/styling/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/font.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/styling/font.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 class FontStyling(TableColumnStylingBase):
     """Font styling options.
 
     Specify the font styling options for a column in the table widget,
     including color, data column, and background highlighting.
     """
 
-    _API_TYPE = "TableColumnStylingFontInput"
-
     @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_column: Optional[Union[str, WidgetField]] = None,
         highlight_background: bool = False
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/icon.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/styling/stacked_bar.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,49 @@
-"""Specification for styling a column with an icon to a value."""
+"""Specification for styling the stacked bar column."""
+
 from typing import Any
 from typing import Dict
+from typing import Optional
 from typing import Union
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links import WidgetField
+from engineai.sdk.dashboard.styling.color import DiscreteMap
+from engineai.sdk.dashboard.styling.color.spec import build_color_spec
 
-from .base import TableColumnStylingBase
+from .base import TableSparklineColumnStylingBase
 
 
-class IconStyling(TableColumnStylingBase):
-    """Styling options for icon column.
+class StackedBarStyling(TableSparklineColumnStylingBase):
+    """Styling options for stacked bar column.
 
-    Specify the styling options for an icon column in the
-    table widget, including data column and position.
+    Specify the styling options for a stacked bar column in
+    the table widget, including color, data column, and total display.
     """
 
-    _API_TYPE = "TableColumnStylingIconInput"
-
     @type_check
     def __init__(
         self,
         *,
-        data_column: Union[str, WidgetField],
-        left: bool = True,
+        color_spec: DiscreteMap,
+        data_column: Optional[Union[str, WidgetField]] = None,
     ):
-        """Constructor for IconStyling.
+        """Constructor for StackedBarStyling.
 
         Args:
-            data_column: id of column which values are used to determine behavior of
-                arrow.
-                By default, will use values of column to which styling is applied.
-            left: whether to put icon to the left (True) or right (False) of column
-                value.
+            data_column: id of column which values are used for chart.
+            color_spec: spec for discrete color map of stacked bar column chart.
+            show_total_on_tooltip: show stacked bar total on tooltip.
         """
-        super().__init__(data_column=data_column, color_spec=None)
-        self.__left = left
-
-    def _build_extra_inputs(self) -> Dict[str, Any]:
-        return {"left": self.__left}
+        super().__init__(
+            data_column=data_column,
+            color_spec=color_spec,
+        )
+
+    def _build_color_spec(self) -> Dict[str, Any]:
+        return (
+            {
+                "colorSpec": build_color_spec(spec=self.color_spec),
+            }
+            if self.color_spec is not None
+            else {}
+        )
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/line.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/styling/area.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,36 @@
-"""Specification for styling a line chart."""
+"""Specification for Area Chart Styling."""
 from typing import Optional
 from typing import Union
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 
 from .base import TableSparklineColumnStylingBase
 
 
-class LineChartStyling(TableSparklineColumnStylingBase):
-    """Styling options for line chart column.
+class AreaChartStyling(TableSparklineColumnStylingBase):
+    """Styling options for area chart column.
 
-    Specify the styling options for a line chart column in
+    Specify the styling options for an area chart column in
     the table widget, including color and data key.
     """
 
-    _API_TYPE = "SparkChartLineStylingInput"
-
     @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_key: Optional[Union[str, WidgetField]] = None,
     ):
-        """Constructor for LineChartStyling.
+        """Constructor for AreaChartStyling.
 
         Args:
             data_key: Dictionary key, stored in data, that is used for chart.
                 By default, will use values of column to which styling is applied.
-            color_spec: spec for color of line chart.
+            color_spec: spec for color of area chart.
         """
         super().__init__(
             data_column=data_key,
             color_spec=color_spec,
         )
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/range.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/group.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,61 @@
-"""Specification for styling a column with an arrow next to value."""
-import enum
+"""Spec for Table group column."""
+
 from typing import Any
 from typing import Dict
-from typing import Optional
 from typing import Union
 
+import pandas as pd
+
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links import WidgetField
-from engineai.sdk.dashboard.styling.color.typing import ColorSpec
-
-from .base import TableColumnStylingBase
+from engineai.sdk.dashboard.links.abstract import AbstractFactoryLinkItemsHandler
+from engineai.sdk.dashboard.templated_string import build_templated_strings
 
+from .exceptions import TableGroupColumnKeyNotFoundError
 
-class RangeShape(enum.Enum):
-    """Range shape options."""
 
-    CIRCLE = "CIRCLE"
-    RECTANGLE = "RECTANGLE"
+class Group(AbstractFactoryLinkItemsHandler):
+    """Define group column for table widget.
 
-
-class RangeStyling(TableColumnStylingBase):
-    """Styling options for range column.
-
-    Specify the styling options for a range column in the
-    table widget, including color, data column, and shape.
+    Define a group column for the table widget,
+    which allows grouping rows based on specified columns.
     """
 
-    _API_TYPE = "TableColumnStylingRangeInput"
-
     @type_check
     def __init__(
         self,
-        *,
-        color_spec: ColorSpec,
-        data_column: Optional[Union[str, WidgetField]] = None,
-        shape: RangeShape = RangeShape.CIRCLE,
+        data_column: Union[str, WidgetField],
+        label: Union[str, WidgetField],
     ):
-        """Constructor for RangeStyling.
+        """Constructor for Group.
 
         Args:
-            data_column: id of column which values are used to determine behavior of
-                arrow.
-            color_spec: spec for color of range value.
-            shape: shape of range indicator.
+            data_column: column that will be used to group the table rows.
+            label: table group label.
         """
-        super().__init__(
-            data_column=data_column,
-            color_spec=color_spec,
-        )
-        self.__shape = shape
+        super().__init__()
+        self.__data_column = data_column
+        self.__label = label
 
-    def _build_extra_inputs(self) -> Dict[str, Any]:
-        return {"shape": self.__shape.value}
+    def validate(self, data: pd.DataFrame) -> None:
+        """Validates column key.
+
+        Args:
+            data: pandas DataFrame or dict where the data is present.
+        """
+        if (
+            isinstance(self.__data_column, str)
+            and self.__data_column not in data.columns
+        ):
+            raise TableGroupColumnKeyNotFoundError(data_column=self.__data_column)
+
+    def build(self) -> Dict[str, Any]:
+        """Builds spec for dashboard API.
+
+        Returns:
+            Input object for Dashboard API
+        """
+        return {
+            "columnKey": build_templated_strings(items=self.__data_column),
+            "label": build_templated_strings(items=self.__label),
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/split_bar.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/styling/split_bar.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,14 @@
     """Styling options for split color bar column.
 
     Specify the styling options for a split color bar column in the
     table widget, including color, data column, min/max values,
     and percentage fill.
     """
 
-    _API_TYPE = "TableColumnStylingSplitBarInput"
-
     @type_check
     def __init__(
         self,
         *,
         data_column: Optional[Union[str, WidgetField]] = None,
         color_spec: Optional[ColorSpec] = None,
         min_value: Optional[Union[float, int]] = None,
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/stacked_bar.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/components/items/styling/number/arrow.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,45 @@
-"""Specification for styling the stacked bar column."""
+"""Spec fot Number Styling Arrow."""
 
 from typing import Any
 from typing import Dict
 from typing import Optional
-from typing import Union
 
 from engineai.sdk.dashboard.decorator import type_check
-from engineai.sdk.dashboard.links import WidgetField
-from engineai.sdk.dashboard.styling.color import DiscreteMap
-from engineai.sdk.dashboard.styling.color.spec import build_color_spec
+from engineai.sdk.dashboard.styling.color.divergent import Divergent
+from engineai.sdk.dashboard.templated_string import TemplatedStringItem
+from engineai.sdk.dashboard.templated_string import build_templated_strings
 
-from .base import TableSparklineColumnStylingBase
+from ..base import BaseItemStyling
 
 
-class StackedBarStyling(TableSparklineColumnStylingBase):
-    """Styling options for stacked bar column.
-
-    Specify the styling options for a stacked bar column in
-    the table widget, including color, data column, and total display.
-    """
-
-    _API_TYPE = "SparkChartStackedBarStylingInput"
+class NumberStylingArrow(BaseItemStyling):
+    """Spec for Number Arrow Styling class."""
 
     @type_check
     def __init__(
         self,
         *,
-        color_spec: DiscreteMap,
-        data_column: Optional[Union[str, WidgetField]] = None,
-        show_total_on_tooltip: bool = False
+        data_column: Optional[TemplatedStringItem] = None,
+        color_divergent: Divergent,
     ):
-        """Constructor for StackedBarStyling.
+        """Construct spec Number Arrow Styling.
 
         Args:
-            data_column: id of column which values are used for chart.
-            color_spec: spec for discrete color map of stacked bar column chart.
-            show_total_on_tooltip: show stacked bar total on tooltip.
+            color_divergent (ColorDivergent): specs for color.
+            data_column (TemplatedStringItem): styling value key.
         """
         super().__init__(
             data_column=data_column,
-            color_spec=color_spec,
         )
-        self.__show_total_on_tooltip = show_total_on_tooltip
+        self.__color_divergent = color_divergent
 
-    def _build_color_spec(self) -> Dict[str, Any]:
-        return (
-            {
-                "colorSpec": build_color_spec(spec=self.color_spec),
-                "showTotalOnTooltip": self.__show_total_on_tooltip,
-            }
-            if self.color_spec is not None
-            else {}
-        )
+    def build(self) -> Dict[str, Any]:
+        """Method implemented by all factories to generate Input spec.
+
+        Returns:
+            Input object for Dashboard API
+        """
+        return {
+            "divergentPalette": self.__color_divergent.build(),
+            "valueKey": build_templated_strings(items=self.column),
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/utils.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/columns/styling/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 
 def build_styling_input(
     data_column: TemplatedStringItem,
     styling: _ColumnStyling,
 ) -> Dict[str, Any]:
     """Build the styling class."""
     styling_spec = styling.build()
-    if not styling_spec.dataKey:
-        styling_spec.dataKey = build_templated_strings(items=data_column)
+    if not styling_spec["dataKey"]:
+        styling_spec["dataKey"] = build_templated_strings(items=data_column)
     return {_get_key(styling): styling_spec}
 
 
 def _get_key(
     styling: _ColumnStyling,
 ) -> str:
     if isinstance(styling, CountryFlagStyling):
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/exceptions.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/header.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/header.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Spec for table header columns (i.e. above normal columns)."""
 
 from typing import Any
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Set
 from typing import Union
 
 import pandas as pd
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links.abstract import AbstractFactoryLinkItemsHandler
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.table.columns.items.text import TextColumn
 
 from .columns.items.base import Column
 from .exceptions import TableColumnsEmptyError
 from .exceptions import TableDuplicatedItemIdError
 from .exceptions import TableHeaderChildTypeError
 from .exceptions import TableHeaderLevelsError
@@ -247,31 +247,30 @@
                 child.set_children_id(item_id=item_id)
             child.set_item_id(item_id=item_id)
 
     def _build_children(self) -> List[Any]:
         children = []
         for item in self.__children:
             if isinstance(item, Header):
-                child = generate_input("TableHeaderColumnInput", header=item.build())
+                child = {"header": item.build()}
             elif isinstance(item, Column):
-                child = generate_input("TableHeaderColumnInput", column=item.build())
+                child = {"column": item.build()}
             else:
                 raise TableHeaderChildTypeError(_type=type(item))
 
             children.append(child)
         return children
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Builds spec for dashboard API.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "TableHeaderInput",
-            label=build_templated_strings(items=self.__label),
-            tooltipText=[
+        return {
+            "label": build_templated_strings(items=self.__label),
+            "tooltipText": [
                 build_templated_strings(items=tooltip)
                 for tooltip in self.__tooltip_text
             ],
-            children=self._build_children(),
-        )
+            "children": self._build_children(),
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/initial_state.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/initial_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Spec for Table widget state."""
 
 from typing import Any
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import cast
 
 from engineai.sdk.dashboard.base import AbstractFactory
 from engineai.sdk.dashboard.decorator import type_check
-from engineai.sdk.dashboard.utils import generate_input
 
 from .exceptions import TableInitialStateIncompatiblePreSelectedIndexError
 from .exceptions import TableInitialStateIncompatiblePreSelectedRowsError
 
 
 class InitialState(AbstractFactory):
     """Define initial state for table widget.
@@ -69,21 +69,20 @@
             pre_selected_max_index: int = cast(int, max(self.__selected))
 
             if int(pre_selected_max_index) > dataframe_rows:
                 raise TableInitialStateIncompatiblePreSelectedIndexError(
                     pre_selected_max_index, dataframe_rows
                 )
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Builds spec for dashboard API.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "TableWidgetStateInput",
-            page=self.__page,
-            rowsPerPage=self.__rows_per_page,
-            searchText=self.__search_text,
-            selected=self.__selected,
-            expanded=[],
-        )
+        return {
+            "page": self.__page,
+            "rowsPerPage": self.__rows_per_page,
+            "searchText": self.__search_text,
+            "selected": self.__selected,
+            "expanded": [],
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/styling.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/styling.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Spec for Table widget styling."""
 
 from typing import Any
+from typing import Dict
 
 from engineai.sdk.dashboard.base import AbstractFactory
 from engineai.sdk.dashboard.decorator import type_check
-from engineai.sdk.dashboard.utils import generate_input
 
 
 class TableStyling(AbstractFactory):
     """Visual styling options for table widget.
 
     Specify the visual styling options for the table widget,
     including borders, column lines, row lines, and row height.
@@ -39,21 +39,20 @@
         super().__init__()
         self.__has_borders = has_borders
         self.__has_column_lines = has_column_lines
         self.__has_body_column_lines = has_body_column_lines
         self.__has_row_lines = has_row_lines
         self.__single_height_row = single_height_row
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Builds spec for dashboard API.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "TableWidgetStylingInput",
-            hasBorders=self.__has_borders,
-            hasColumnLines=self.__has_column_lines,
-            hasBodyColumnLines=self.__has_body_column_lines,
-            hasRowLines=self.__has_row_lines,
-            rowHeightSize="SINGLE" if self.__single_height_row else "DOUBLE",
-        )
+        return {
+            "hasBorders": self.__has_borders,
+            "hasColumnLines": self.__has_column_lines,
+            "hasBodyColumnLines": self.__has_body_column_lines,
+            "hasRowLines": self.__has_row_lines,
+            "rowHeightSize": "SINGLE" if self.__single_height_row else "DOUBLE",
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/table.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/table/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Spec for Table widget."""
 
 import math
 from typing import Any
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Set
 from typing import Union
 
 import pandas as pd
 from pandas.api.types import is_datetime64_dtype
@@ -25,15 +26,14 @@
     PercentageAllPositiveSequentialColorGradient,
 )
 from engineai.sdk.dashboard.styling.color.default_specs import (
     PositiveNegativeDiscreteMap,
 )
 from engineai.sdk.dashboard.styling.color.default_specs import ScoreColorDiscreteMap
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.pandas_utils import are_values_relative
 from engineai.sdk.dashboard.widgets.pandas_utils import only_integers
 from engineai.sdk.dashboard.widgets.pandas_utils import only_negative_or_positive_values
 from engineai.sdk.dashboard.widgets.pandas_utils import only_negative_values
 from engineai.sdk.dashboard.widgets.pandas_utils import only_positive_values
 from engineai.sdk.dashboard.widgets.table.columns.items.datetime import DatetimeColumn
 from engineai.sdk.dashboard.widgets.table.columns.items.number import NumberColumn
@@ -408,37 +408,34 @@
 
         return height
 
     def _get_items_specs(self) -> List[Any]:
         items_spec = []
         for item in self.__items:
             if isinstance(item, Header):
-                items_spec.append(
-                    generate_input("TableHeaderColumnInput", header=item.build())
-                )
+                items_spec.append({"header": item.build()})
             else:
-                items_spec.append(
-                    generate_input("TableHeaderColumnInput", column=item.build())
-                )
+                items_spec.append({"column": item.build()})
         return items_spec
 
-    def _build_widget_input(self) -> Any:
+    def _build_widget_input(self) -> Dict[str, Any]:
         """Builds spec for dashboard API.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "TableGridWidgetInput",
-            title=build_templated_strings(items=self.__title),
-            hasSearchBox=self.__has_search_box,
-            hasFilterRow=self.__has_filter_row,
-            hasHeaderFilter=self.__has_header_filter,
-            rowSelection=self.__row_selection,
-            columns=self._get_items_specs(),
-            defaultState=self.__initial_state.build(),
-            data=build_data(path=self.dependency_id, json_data=self._json_data),
-            styling=self.__styling.build(),
-            groupColumns=[group_column.build() for group_column in self.__group_columns]
+        return {
+            "title": build_templated_strings(items=self.__title),
+            "hasSearchBox": self.__has_search_box,
+            "hasFilterRow": self.__has_filter_row,
+            "hasHeaderFilter": self.__has_header_filter,
+            "rowSelection": self.__row_selection,
+            "columns": self._get_items_specs(),
+            "defaultState": self.__initial_state.build(),
+            "data": build_data(path=self.dependency_id, json_data=self._json_data),
+            "styling": self.__styling.build(),
+            "groupColumns": [
+                group_column.build() for group_column in self.__group_columns
+            ]
             if self.__group_columns is not None
             else None,
-        )
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/__init__.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/build_y_axis.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/build_y_axis.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 """Spec to build different series supported by timeseries widget."""
 
 from typing import Any
+from typing import Dict
 from typing import Union
 
-from engineai.sdk.dashboard.utils import generate_input
-
 from .y_axis import YAxis
 from .y_axis_mirror import MirrorYAxis
 
 YAxisSpec = Union[
     YAxis,
     MirrorYAxis,
 ]
 
 
-def build_timeseries_y_axis(axis: YAxisSpec) -> Any:
+def build_timeseries_y_axis(axis: YAxisSpec) -> Dict[str, Any]:
     """Builds spec for dashboard API.
 
     Args:
         axis (YAxisSpec): axis spec
 
     Returns:
         Input object for Dashboard API
     """
-    return generate_input(
-        "TimeseriesWidgetChartYAxisUnionInput", **{_get_input_key(axis): axis.build()}
-    )
+    return {**{_get_input_key(axis): axis.build()}}
 
 
 def _get_input_key(axis: YAxisSpec) -> str:
     if isinstance(axis, YAxis):
         result = "standard"
     elif isinstance(axis, MirrorYAxis):
         result = "mirror"
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/y_axis.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/navigator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,96 +1,97 @@
-"""Specs for y axis of a Timeseries chart."""
+"""Spec for navigator of a timeseries widget."""
 
 from typing import Any
-from typing import List
-from typing import Mapping
+from typing import Dict
 from typing import Optional
-from typing import Union
-from typing import cast
 
 import pandas as pd
 
 from engineai.sdk.dashboard.decorator import type_check
-from engineai.sdk.dashboard.formatting import AxisNumberFormatting
-from engineai.sdk.dashboard.links import WidgetField
+from engineai.sdk.dashboard.links.abstract import AbstractFactoryLinkItemsHandler
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
-from engineai.sdk.dashboard.widgets.components.charts.axis.scale import AxisScale
+from engineai.sdk.dashboard.templated_string import build_templated_strings
+from engineai.sdk.dashboard.widgets.base import WidgetTitleType
 
-from ...series.typing import TimeseriesSeries
-from .base import BaseTimeseriesYAxis
+from .exceptions import TimeseriesNavigatorEmptyDefinitionError
+from .series.typing import TimeseriesSeries
 
 
-class YAxis(BaseTimeseriesYAxis):
-    """Specify y-axis appearance & behavior in Timeseries chart.
+class Navigator(AbstractFactoryLinkItemsHandler):
+    """Navigation of Timeseries data.
 
-    Construct specifications for the y-axis of a Timeseries chart with
-    a range of options to customize its appearance and behavior.
+    Construct a navigator for a timeseries widget for efficient
+    navigation and exploration of time-series data. Specify one or
+    more series to be included in the navigator for easy visualization
+    of trends and patterns across different metrics.
     """
 
-    _API_TYPE = "TimeseriesWidgetChartStandardYAxisInput"
-
     @type_check
     def __init__(
-        self,
-        *,
-        formatting: Optional[AxisNumberFormatting] = None,
-        title: Union[str, WidgetField] = "",
-        enable_crosshair: bool = False,
-        scale: Optional[AxisScale] = None,
-    ):
-        """Constructor for YAxis.
+        self, *series: TimeseriesSeries, title: Optional[WidgetTitleType] = None
+    ) -> None:
+        """Constructor for Navigator.
 
         Args:
-            formatting (Optional[AxisNumberFormatting]): formatting spec for axis
-                labels.
-                Defaults to None (Base AxisFormatting).
-            title (Union[str, WidgetField]): axis title.
-                Defaults to empty string.
-            enable_crosshair (bool): whether to enable crosshair that follows either
-                the mouse pointer or the hovered point.
-                Defaults to False.
-            scale (Optional[YAxisScale]): y axis scale, one of
-                AxisScaleSymmetric, AxisScaleDynamic,
-                AxisScalePositive, AxisScaleNegative.
-                Defaults to AxisScaleSymmetric.
+            title: title to be added to navigator
+            series: series to be added to navigator
+
+        Examples:
+            ??? examples "Create a minimal timeseries widget with a navigator"
+                ```python linenums="1"
+                import pandas as pd
+
+                from engineai.sdk.dashboard.dashboard import Dashboard
+                from engineai.sdk.dashboard.widgets import timeseries
+
+                data = pd.DataFrame(
+                    {
+                        "value": [1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
+                    },
+                    index=pd.date_range("2020-01-01", "2020-01-10"),
+                )
+
+                ts = timeseries.Timeseries(
+                    data=data,
+                    navigator=timeseries.Navigator(
+                        timeseries.ColumnSeries(data_column="value")
+                    )
+                )
+                Dashboard(content=ts)
+                ```
         """
-        super().__init__(
-            formatting=formatting,
-            title=title,
-            enable_crosshair=enable_crosshair,
-            scale=scale,
-        )
-        self.__series: List[TimeseriesSeries] = []
+        super().__init__()
 
-    def __len__(self) -> int:
-        """Returns number of series in axis.
+        if len(series) == 0:
+            raise TimeseriesNavigatorEmptyDefinitionError()
 
-        Returns:
-            int: number of series in axis.
-        """
-        return len(self.__series)
+        self.__series = series
+        self.__title = title
+
+    def prepare(self, date_column: TemplatedStringItem) -> None:
+        """Method that prepares the spec to be build."""
+        for index, series in enumerate(self.__series):
+            series.prepare(date_column, index=index)
+
+    def validate(self, *, data: pd.DataFrame) -> None:
+        """Validate if dataframe that will be used for column contains required columns.
 
-    def _validate_series(self, *, data: pd.DataFrame) -> None:
-        """Validate timeseries y axis series."""
+        Args:
+            data: pandas dataframe which will be used for table
+
+        """
         for series in self.__series:
             series.validate(data=data)
 
-    def add_series(self, *series: TimeseriesSeries) -> "YAxis":
-        """Add series to y axis.
+    def build(self) -> Dict[str, Any]:
+        """Method implemented by all factories to generate Input spec.
 
         Returns:
-            YAxis: reference to this axis to facilitate inline manipulation.
-
+            Input object for Dashboard API
         """
-        return cast(YAxis, self._add_series(self.__series, *series))
-
-    def prepare(self, date_column: TemplatedStringItem, offset: int = 0) -> None:
-        """Prepare layout for building."""
-        for index, element in enumerate(self.__series):
-            element.prepare(
-                date_column=date_column,
-                index=index + offset,
-            )
-
-    def _build_extra_y_axis(self) -> Mapping[str, Any]:
-        """Method that generates the input for a specific y axis."""
-        return {"series": [series.build() for series in self.__series]}
+        series_spec = []
+        for series in self.__series:
+            series_spec.append(series.build())
+        return {
+            "series": series_spec,
+            "title": build_templated_strings(items=self.__title),
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/chart.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/chart.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Spec for charts in a Timeseries widget."""
 
 from typing import Any
+from typing import Dict
 from typing import Optional
 from typing import Union
 
 import pandas as pd
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.abstract import AbstractFactoryLinkItemsHandler
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.charts.tooltip.item import (
     build_tooltip_item,
 )
 
 from ..components.charts.typing import TooltipItems
 from ..utils import get_tooltips
 from .axis.x_axis import XAxis
@@ -93,23 +93,23 @@
         right_y_axis: Optional[Union[YAxisSpec, TimeseriesSeries]] = None,
     ) -> None:
         self.__validate_axis_position(left_y_axis)
 
         self.__left_y_axis = (
             left_y_axis
             if isinstance(left_y_axis, (YAxis, MirrorYAxis))
-            else YAxis().add_series(left_y_axis)
+            else YAxis(series=[left_y_axis])
             if left_y_axis is not None
             else None
         )
 
         self.__right_y_axis = (
             right_y_axis
             if isinstance(right_y_axis, (YAxis, MirrorYAxis))
-            else YAxis().add_series(right_y_axis)
+            else YAxis(series=[right_y_axis])
             if right_y_axis is not None
             else None
         )
 
         self.__validate_axis()
 
     def __validate_axis(
@@ -204,39 +204,40 @@
                 data=data,
             )
         if self.__right_y_axis is not None:
             self.__right_y_axis.validate(
                 data=data,
             )
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API.
         """
-        return generate_input(
-            "TimeseriesWidgetChartInput",
-            xAxis=self.__x_axis.build(),
-            yAxisLeft=[build_timeseries_y_axis(axis=self.__left_y_axis)]
+        return {
+            "xAxis": self.__x_axis.build(),
+            "yAxisLeft": [build_timeseries_y_axis(axis=self.__left_y_axis)]
             if self.__left_y_axis is not None
             else [],
-            yAxisRight=[build_timeseries_y_axis(axis=self.__right_y_axis)]
+            "yAxisRight": [build_timeseries_y_axis(axis=self.__right_y_axis)]
             if self.__right_y_axis is not None
             else [],
-            title=build_templated_strings(items=self.__title) if self.__title else None,
-            heightPercentage=self.height_percentage,
+            "title": build_templated_strings(items=self.__title)
+            if self.__title
+            else None,
+            "heightPercentage": self.height_percentage,
             **self.__build_tooltip(),
-            enableAreaStacking=self.__area_series_stacked,
-        )
+            "enableAreaStacking": self.__area_series_stacked,
+        }
 
-    def __build_tooltip(self) -> Any:
+    def __build_tooltip(self) -> Dict[str, Any]:
         tooltip_spec = None
         if len(self.__extra_tooltip_items) > 0:
-            tooltip_spec = generate_input(
-                "TimeseriesWidgetChartTooltipInput",
-                xAxisKey=build_templated_strings(items=self._date_column),
-                items=[
+            tooltip_spec = {
+                "xAxisKey": build_templated_strings(items=self._date_column),
+                "items": [
                     build_tooltip_item(item=item) for item in self.__extra_tooltip_items
                 ],
-            )
+            }
+
         return {"tooltip": tooltip_spec}
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/consts.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/consts.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/enums.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/enums.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/exceptions.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/navigator.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/series/column.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,98 +1,97 @@
-"""Spec for navigator of a timeseries widget."""
+"""Spec for a column series of a Timeseries widget."""
 
 from typing import Any
+from typing import Dict
 from typing import Optional
+from typing import Union
 
 import pandas as pd
 
 from engineai.sdk.dashboard.decorator import type_check
-from engineai.sdk.dashboard.links.abstract import AbstractFactoryLinkItemsHandler
-from engineai.sdk.dashboard.templated_string import TemplatedStringItem
-from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
-from engineai.sdk.dashboard.widgets.base import WidgetTitleType
-
-from .exceptions import TimeseriesNavigatorEmptyDefinitionError
-from .series.typing import TimeseriesSeries
-
-
-class Navigator(AbstractFactoryLinkItemsHandler):
-    """Navigation of Timeseries data.
-
-    Construct a navigator for a timeseries widget for efficient
-    navigation and exploration of time-series data. Specify one or
-    more series to be included in the navigator for easy visualization
-    of trends and patterns across different metrics.
+from engineai.sdk.dashboard.links import WidgetField
+from engineai.sdk.dashboard.links.typing import GenericLink
+from engineai.sdk.dashboard.styling.color import Palette
+from engineai.sdk.dashboard.widgets.components.charts.series.entities.country import (
+    CountryEntity,
+)
+from engineai.sdk.dashboard.widgets.components.charts.series.entities.typing import (
+    Entities,
+)
+from engineai.sdk.dashboard.widgets.components.charts.styling import ColumnSeriesStyling
+
+from ...components.charts.typing import TooltipItems
+from .base import TimeseriesBaseSeries
+
+
+class ColumnSeries(TimeseriesBaseSeries):
+    """Visualize data as vertical columns in Timeseries widget.
+
+    Construct specifications for a column series within a Timeseries widget to
+    visualize data as vertical columns on the chart. Each column represents a
+    distinct data point, with the height of the column reflecting its
+    corresponding value.
     """
 
+    _INPUT_KEY = "column"
+    _styling_class = ColumnSeriesStyling
+
     @type_check
     def __init__(
-        self, *series: TimeseriesSeries, title: Optional[WidgetTitleType] = None
-    ) -> None:
-        """Constructor for Navigator.
+        self,
+        *,
+        data_column: Union[str, WidgetField],
+        name: Optional[Union[str, GenericLink]] = None,
+        styling: Optional[Union[Palette, ColumnSeriesStyling]] = None,
+        entity: Optional[Entities] = None,
+        show_in_legend: bool = True,
+        required: bool = True,
+        visible: bool = True,
+        right_axis: bool = False,
+        tooltips: Optional[TooltipItems] = None,
+    ):
+        """Constructor for ColumnSeries.
 
         Args:
-            title: title to be added to navigator
-            series: series to be added to navigator
-
-        Examples:
-            ??? examples "Create a minimal timeseries widget with a navigator"
-                ```python linenums="1"
-                import pandas as pd
-
-                from engineai.sdk.dashboard.dashboard import Dashboard
-                from engineai.sdk.dashboard.widgets import timeseries
-
-                data = pd.DataFrame(
-                    {
-                        "value": [1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
-                    },
-                    index=pd.date_range("2020-01-01", "2020-01-10"),
-                )
-
-                ts = timeseries.Timeseries(
-                    data=data,
-                    navigator=timeseries.Navigator(
-                        timeseries.ColumnSeries(data_column="value")
-                    )
-                )
-                Dashboard(content=ts)
-                ```
+            data_column: name of column in pandas dataframe(s) used for the values of
+                this series.
+            name: series name (shown in legend and tooltip).
+            styling: styling spec, by default uses the values from the sequential
+                palette.
+            entity: entity spec.
+            show_in_legend: whether to show series in legend or not.
+            required: Flag to make the Series mandatory. If required == True and no
+                Data the widget will show an error. If required==False and no Data,
+                the widget hides the Series.
+            visible: Flag to make the Series visible when chart is loaded.
+            right_axis: Flag to make the Series visible on the right axis.
+            tooltips: tooltip items to be displayed at Series level.
         """
-        super().__init__()
-
-        if len(series) == 0:
-            raise TimeseriesNavigatorEmptyDefinitionError()
-
-        self.__series = series
-        self.__title = title
-
-    def prepare(self, date_column: TemplatedStringItem) -> None:
-        """Method that prepares the spec to be build."""
-        for index, series in enumerate(self.__series):
-            series.prepare(date_column, index=index)
+        super().__init__(
+            name=name,
+            data_column=data_column,
+            show_in_legend=show_in_legend,
+            required=required,
+            visible=visible,
+            styling=ColumnSeriesStyling(color_spec=styling)
+            if isinstance(styling, Palette)
+            else styling,
+            entity=entity,
+            right_axis=right_axis,
+            tooltips=tooltips,
+        )
 
     def validate(self, *, data: pd.DataFrame) -> None:
-        """Validate if dataframe that will be used for column contains required columns.
+        """Validate if dataframe that will be used for series contains required columns.
 
         Args:
             data: pandas dataframe which will be used for table
-
         """
-        for series in self.__series:
-            series.validate(data=data)
+        super().validate(data=data)
 
-    def build(self) -> Any:
-        """Method implemented by all factories to generate Input spec.
+        if self._entity is not None and isinstance(self._entity, CountryEntity):
+            self._entity.validate_country_code()
 
-        Returns:
-            Input object for Dashboard API
-        """
-        series_spec = []
-        for series in self.__series:
-            series_spec.append(series.build())
-        return generate_input(
-            "TimeseriesWidgetNavigatorInput",
-            series=series_spec,
-            title=build_templated_strings(items=self.__title),
-        )
+    def _build_extra_inputs(self) -> Dict[str, Any]:
+        return {
+            "transforms": [transform.build() for transform in self._transforms],
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/period_selector/custom_period.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/period_selector/custom_period.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Spec for a custom period for a period selector."""
 
 from datetime import datetime
 from typing import Any
+from typing import Dict
 from typing import Optional
 from typing import Union
 
 import pandas as pd
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links.abstract import AbstractFactoryLinkItemsHandler
-from engineai.sdk.dashboard.utils import generate_input
 
 from ..exceptions import TimeseriesPeriodSelectorDatesDefinitionError
 
 
 class CustomPeriod(AbstractFactoryLinkItemsHandler):
     """Define custom time intervals for period selector in Timeseries.
 
@@ -67,19 +67,18 @@
         """Returns label associated with custom period.
 
         Returns:
             str: label
         """
         return self.__label if self.__label else ""
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "TimeseriesWidgetCustomPeriodInput",
-            label=self.__label,
-            startDate=self.__start_date,
-            endDate=self.__end_date,
-        )
+        return {
+            "label": self.__label,
+            "startDate": self.__start_date,
+            "endDate": self.__end_date,
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/period_selector/period.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/period_selector/period.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,31 @@
 """Spec to build different periods supported by period selector."""
 
 from typing import Any
 from typing import Dict
 from typing import Union
 
-from engineai.sdk.dashboard.utils import generate_input
-
 from .custom_period import CustomPeriod
 from .standard import Period
 
 PeriodType = Union[Period, CustomPeriod]
 
 
-def build_timeseries_period(period: PeriodType) -> Any:
+def build_timeseries_period(period: PeriodType) -> Dict[str, Any]:
     """Builds spec for dashboard API.
 
     Returns:
         Input object for Dashboard API
     """
-    return generate_input(
-        "TimeseriesWidgetPeriodInput",
-        **_get_input(period),
-    )
+    return _get_input(period)
 
 
 def _get_input(period: PeriodType) -> Dict[str, Any]:
     if isinstance(period, Period):
-        return {
-            "standard": generate_input(
-                "TimeseriesWidgetStandardPeriodInput",
-                period=period.value,
-            )
-        }
+        return {"standard": {"period": period.value}}
     elif isinstance(period, CustomPeriod):
         return {"custom": period.build()}
 
     else:
         raise TypeError(
             f"period needs to be of Period, CustomPeriod. " f"{type(period)} provided"
         )
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/period_selector/selector.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/period_selector/selector.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Spec for period selector of a timeseries widget."""
 
 from typing import Any
+from typing import Dict
 from typing import List
 from typing import Optional
 
 from engineai.sdk.dashboard.base import AbstractFactory
 from engineai.sdk.dashboard.decorator import type_check
-from engineai.sdk.dashboard.utils import generate_input
 
 from ..exceptions import TimeseriesPeriodSelectorHiddenPeriodsError
 from ..exceptions import TimeseriesPeriodSelectorNoAvailableDefaultOptionError
 from .custom_period import CustomPeriod
 from .period import PeriodType
 from .period import build_timeseries_period
 from .standard import Period
@@ -129,23 +129,22 @@
 
         if len(custom_periods) == 1:
             custom_periods[0].prepare("Custom Period")
         else:
             for i in range(0, len(custom_periods)):
                 custom_periods[i].prepare("Period " + str(i + 1))
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "TimeseriesWidgetPeriodSelectorInput",
-            periods=[
+        return {
+            "periods": [
                 build_timeseries_period(period=period) for period in self.__periods
             ]
             if self.__periods
             else [],
-            selected=self.__selected,
-            isDatePickerVisible=self.__visible,
-        )
+            "selected": self.__selected,
+            "isDatePickerVisible": self.__visible,
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/period_selector/standard.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/period_selector/standard.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/area.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/series/area.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 class AreaSeries(TimeseriesBaseSeries):
     """Visualize data as filled areas in Timeseries widget.
 
     Construct specifications for an area series within a Timeseries
     widget to visualize data as filled areas on the chart.
     """
 
-    _API_TYPE = "TimeseriesWidgetAreaSeriesInput"
     _INPUT_KEY = "area"
     _styling_class = AreaSeriesStyling
 
     @type_check
     def __init__(
         self,
         *,
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/area_range.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/series/area_range.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 class AreaRangeSeries(TimeseriesBaseSeries):
     """Visualize data as filled areas between low and high values.
 
     Construct specifications for an area range series within a Timeseries
     widget to visualize data as filled areas between low and high values on the chart.
     """
 
-    _API_TYPE = "TimeseriesWidgetAreaRangeSeriesInput"
     _INPUT_KEY = "range"
     _styling_class = AreaRangeSeriesStyling
 
     @type_check
     def __init__(
         self,
         *,
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/base.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/series/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.styling.color.palette import qualitative_palette
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.charts.series.base import ChartSeriesBase
 from engineai.sdk.dashboard.widgets.components.charts.series.entities.typing import (
     Entities,
 )
 from engineai.sdk.dashboard.widgets.components.charts.styling.typing import (
     ColoredSeriesStyling,
 )
@@ -130,19 +129,17 @@
 
         for item in self._tooltip_items:
             item.validate(data=data)
 
         if self._styling is not None:
             self._styling.validate(data=data)
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Build series Input spec."""
-        return generate_input(
-            "TimeseriesWidgetSeriesInput", **{self._input_key: self._build_series()}
-        )
+        return {self._input_key: self._build_series()}
 
     def _validate_data_column(
         self,
         *,
         data: pd.DataFrame,
         data_column: Optional[Union[str, GenericLink]],
         data_column_name: str,
@@ -153,36 +150,40 @@
                 if data_column not in data.columns:
                     raise TimeseriesValidateSeriesDataColumnNotFound(
                         series_class_name=self.__class__.__name__,
                         column_name=data_column_name,
                         column_value=data_column,
                     )
 
-    def _build_series(self) -> Any:
+    def _build_series(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            self._api_type,
-            name=build_templated_strings(items=self.name),
-            xAxisKey=build_templated_strings(items=self._date_column),
-            showInLegend=self._show_in_legend,
-            tooltipItems=[
+        return {
+            "name": build_templated_strings(items=self.name),
+            "xAxisKey": build_templated_strings(items=self._date_column),
+            "showInLegend": self._show_in_legend,
+            "tooltipItems": [
                 build_tooltip_item(item=item) for item in self._tooltip_items
             ],
-            required=self._required,
-            isVisible=self._visible,
-            **{"yAxisKey": build_templated_strings(items=self._data_column)}
-            if self._data_column is not None
-            else {},
+            "required": self._required,
+            "isVisible": self._visible,
+            "styling": self._styling.build() if self._styling is not None else None,
+            "entity": self._entity.build() if self._entity is not None else None,
             **self._build_extra_inputs(),
-            styling=self._styling.build() if self._styling is not None else None,
-            entity=self._entity.build() if self._entity is not None else None,
+            **self._build_y_axis_key(),
+        }
+
+    def _build_y_axis_key(self) -> Dict[str, Any]:
+        return (
+            {"yAxisKey": build_templated_strings(items=self._data_column)}
+            if self._data_column is not None
+            else {}
         )
 
     def _build_extra_inputs(self) -> Dict[str, Any]:
         return {}
 
     def __set_default_styling(self, color: ColorSpec) -> None:
         if self._styling_class is None:
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/bubble.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/series/bubble.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 
     Construct specifications for a bubble series within a Timeseries widget.
     Visually represent data with bubbles on the chart. The size of each
     bubble corresponds to a specific data value, providing an intuitive way
     to grasp the magnitude of each data point.
     """
 
-    _API_TYPE = "TimeseriesWidgetBubbleSeriesInput"
     _INPUT_KEY = "bubble"
     _styling_class = BubbleCircleSeriesStyling
 
     @type_check
     def __init__(
         self,
         *,
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/column.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/series/line.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Spec for a column series of a Timeseries widget."""
+"""Spec for a line series of a Timeseries widget."""
 
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Union
 
 import pandas as pd
@@ -13,52 +13,51 @@
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.widgets.components.charts.series.entities.country import (
     CountryEntity,
 )
 from engineai.sdk.dashboard.widgets.components.charts.series.entities.typing import (
     Entities,
 )
-from engineai.sdk.dashboard.widgets.components.charts.styling import ColumnSeriesStyling
+from engineai.sdk.dashboard.widgets.components.charts.styling import LineSeriesStyling
 
 from ...components.charts.typing import TooltipItems
 from .base import TimeseriesBaseSeries
 
 
-class ColumnSeries(TimeseriesBaseSeries):
-    """Visualize data as vertical columns in Timeseries widget.
+class LineSeries(TimeseriesBaseSeries):
+    """Visualize data with continuous lines in Timeseries.
 
-    Construct specifications for a column series within a Timeseries widget to
-    visualize data as vertical columns on the chart. Each column represents a
-    distinct data point, with the height of the column reflecting its
-    corresponding value.
+    Construct specifications for a line series within a Timeseries widget to
+    visualize data as a continuous line connecting data points on the chart.
+    Each data point represents a specific value along the timeline, and the
+    lines provide a clear depiction of the trends and patterns present in the data.
     """
 
-    _API_TYPE = "TimeseriesWidgetColumnSeriesInput"
-    _INPUT_KEY = "column"
-    _styling_class = ColumnSeriesStyling
+    _INPUT_KEY = "line"
+    _styling_class = LineSeriesStyling
 
     @type_check
     def __init__(
         self,
         *,
         data_column: Union[str, WidgetField],
         name: Optional[Union[str, GenericLink]] = None,
-        styling: Optional[Union[Palette, ColumnSeriesStyling]] = None,
+        styling: Optional[Union[Palette, LineSeriesStyling]] = None,
         entity: Optional[Entities] = None,
         show_in_legend: bool = True,
         required: bool = True,
         visible: bool = True,
         right_axis: bool = False,
         tooltips: Optional[TooltipItems] = None,
     ):
-        """Constructor for ColumnSeries.
+        """Constructor for LineSeries.
 
         Args:
-            data_column: name of column in pandas dataframe(s) used for the values of
-                this series.
+            data_column: name of column in pandas dataframe(s) used for the values
+                of this series.
             name: series name (shown in legend and tooltip).
             styling: styling spec, by default uses the values from the sequential
                 palette.
             entity: entity spec.
             show_in_legend: whether to show series in legend or not.
             required: Flag to make the Series mandatory. If required == True and no
                 Data the widget will show an error. If required==False and no Data,
@@ -69,15 +68,15 @@
         """
         super().__init__(
             name=name,
             data_column=data_column,
             show_in_legend=show_in_legend,
             required=required,
             visible=visible,
-            styling=ColumnSeriesStyling(color_spec=styling)
+            styling=LineSeriesStyling(color_spec=styling)
             if isinstance(styling, Palette)
             else styling,
             entity=entity,
             right_axis=right_axis,
             tooltips=tooltips,
         )
 
@@ -89,10 +88,8 @@
         """
         super().validate(data=data)
 
         if self._entity is not None and isinstance(self._entity, CountryEntity):
             self._entity.validate_country_code()
 
     def _build_extra_inputs(self) -> Dict[str, Any]:
-        return {
-            "transforms": [transform.build() for transform in self._transforms],
-        }
+        return {"transforms": [transform.build() for transform in self._transforms]}
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/line.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/series/scatter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Spec for a line series of a Timeseries widget."""
+"""Spec for a scatter series of a Timeseries widget."""
 
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Union
 
 import pandas as pd
@@ -13,52 +13,53 @@
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.widgets.components.charts.series.entities.country import (
     CountryEntity,
 )
 from engineai.sdk.dashboard.widgets.components.charts.series.entities.typing import (
     Entities,
 )
-from engineai.sdk.dashboard.widgets.components.charts.styling import LineSeriesStyling
+from engineai.sdk.dashboard.widgets.components.charts.styling import (
+    ScatterSeriesStyling,
+)
 
 from ...components.charts.typing import TooltipItems
 from .base import TimeseriesBaseSeries
 
 
-class LineSeries(TimeseriesBaseSeries):
-    """Visualize data with continuous lines in Timeseries.
+class ScatterSeries(TimeseriesBaseSeries):
+    """Visualize data as individual points in Timeseries.
 
-    Construct specifications for a line series within a Timeseries widget to
-    visualize data as a continuous line connecting data points on the chart.
-    Each data point represents a specific value along the timeline, and the
-    lines provide a clear depiction of the trends and patterns present in the data.
+    Construct specifications for a scatter series within a Timeseries widget
+    to visualize data as individual points on the chart without any connections
+    between them. Each data point is represented by a distinct marker, providing
+    a clear depiction of the data distribution over time.
     """
 
-    _API_TYPE = "TimeseriesWidgetLineSeriesInput"
-    _INPUT_KEY = "line"
-    _styling_class = LineSeriesStyling
+    _INPUT_KEY = "scatter"
+    _styling_class = ScatterSeriesStyling
 
     @type_check
     def __init__(
         self,
         *,
         data_column: Union[str, WidgetField],
         name: Optional[Union[str, GenericLink]] = None,
-        styling: Optional[Union[Palette, LineSeriesStyling]] = None,
+        styling: Optional[Union[Palette, ScatterSeriesStyling]] = None,
         entity: Optional[Entities] = None,
         show_in_legend: bool = True,
         required: bool = True,
         visible: bool = True,
         right_axis: bool = False,
         tooltips: Optional[TooltipItems] = None,
     ):
-        """Constructor for LineSeries.
+        """Constructor for ScatterSeries.
 
         Args:
-            data_column: name of column in pandas dataframe(s) used for the values
-                of this series.
+            data_column: name of column in pandas dataframe(s) used for the values of
+                this series.
             name: series name (shown in legend and tooltip).
             styling: styling spec, by default uses the values from the sequential
                 palette.
             entity: entity spec.
             show_in_legend: whether to show series in legend or not.
             required: Flag to make the Series mandatory. If required == True and no
                 Data the widget will show an error. If required==False and no Data,
@@ -69,15 +70,15 @@
         """
         super().__init__(
             name=name,
             data_column=data_column,
             show_in_legend=show_in_legend,
             required=required,
             visible=visible,
-            styling=LineSeriesStyling(color_spec=styling)
+            styling=ScatterSeriesStyling(color_spec=styling)
             if isinstance(styling, Palette)
             else styling,
             entity=entity,
             right_axis=right_axis,
             tooltips=tooltips,
         )
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/point.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/series/point.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 
     Construct specifications for a point series within a Timeseries widget,
     enabling users to visualize individual data points on the chart as
     distinct markers. Each marker represents a specific data value,
     providing a clear and concise depiction of the data distribution over time.
     """
 
-    _API_TYPE = "TimeseriesWidgetPointSeriesInput"
     _INPUT_KEY = "point"
     _styling_class = PointSeriesStyling
 
     @type_check
     def __init__(
         self,
         *,
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/typing.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/series/typing.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/timeseries.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/timeseries.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Spec for Timeseries widget."""
 
 import math
+import warnings
 from typing import Any
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Type
 from typing import Union
 from typing import cast
 
 import pandas as pd
@@ -16,15 +18,14 @@
 from engineai.sdk.dashboard.data.http import Http
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.styling.color.default_specs import (
     PositiveNegativeDiscreteMap,
 )
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.charts.toolbar import build_chart_toolbar
 from engineai.sdk.dashboard.widgets.utils import build_data
 
 from ...data.manager.manager import StaticDataType
 from ...enum.legend_position import LegendPosition
 from ..base import Widget
 from ..base import WidgetTitleType
@@ -69,27 +70,30 @@
     _DEPENDENCY_ID = "__TIMESERIES_DATA_DEPENDENCY__"
 
     @type_check
     def __init__(
         self,
         data: Union[DataSource, pd.DataFrame, Http],
         *,
+        charts: Optional[List[Union[str, TimeseriesSeries, Chart]]] = None,
         date_column: Optional[TemplatedStringItem] = None,
         widget_id: Optional[str] = None,
         period_selector: Optional[PeriodSelector] = None,
         title: Optional[WidgetTitleType] = None,
         legend: Optional[LegendPosition] = None,
         navigator: Optional[Union[Navigator, TimeseriesSeries]] = None,
         enable_toolbar: bool = True,
     ):
         """Constructor for Timeseries widget.
 
         Args:
             data: data to be used by widget. Accepts DataSource method as well as raw
                 data.
+            charts: list of charts to be added to the widget.
+                Each element in the list is a new chart, with a maximum of 5 Charts.
             date_column: column that must be used as x axis date. This column must be
                 of type datetime.
             widget_id: unique widget id in a dashboard.
             period_selector: selector for particular periods in a chart.
             title: title of widget can be either a string (fixed value) or determined
                 by a value from another widget using a WidgetLink.
             legend: legend of timeseries widget.
@@ -111,15 +115,16 @@
                     },
                     index=pd.date_range("2020-01-01", "2020-01-10"),
                 )
                 Dashboard(content=timeseries.Timeseries(data=data))
                 ```
         """
         super().__init__(widget_id=widget_id, data=data)
-        self.__charts: List[Chart] = []
+        self.__new_version = False
+        self.__charts: List[Chart] = self.__set_charts(charts)
         self.__date_column = date_column
         self.__set_basic_timeseries(data=data)
         self.__period_selector = (
             period_selector if period_selector else PeriodSelector()
         )
         self.__set_navigator(navigator=navigator)
         self.__set_legend(legend=legend)
@@ -131,16 +136,48 @@
     @property
     def date_column(self) -> TemplatedStringItem:
         """Get date column."""
         if self.__date_column is None:
             raise TimeseriesEmptyDateColumnError()
         return self.__date_column
 
-    def __set_basic_timeseries(self, data: Union[DataSource, pd.DataFrame]) -> None:
+    def __set_charts(
+        self, charts: Optional[List[Union[str, TimeseriesSeries, Chart]]]
+    ) -> List[Chart]:
+        result: List[Chart] = []
+
+        if charts is not None:
+            if len(charts) == 0:
+                raise TimeseriesChartsEmptyDefinitionError()
+
+            if len(charts) > 5:
+                raise TimeseriesTooManyChartsError(widget_id=self.widget_id)
+
+            self.__new_version = True
+            for item in charts:
+                if isinstance(item, str):
+                    result.append(Chart(left_y_axis=LineSeries(data_column=item)))
+                elif isinstance(item, Chart):
+                    result.append(item)
+                else:
+                    axis_position = {
+                        "left_y_axis"
+                        if not item.is_right_axis
+                        else "right_y_axis": item
+                    }
+                    result.append(Chart(**axis_position))
+
+        return result
+
+    def __set_basic_timeseries(
+        self, data: Union[DataSource, pd.DataFrame, Http]
+    ) -> None:
         """Set basic timeseries widget."""
+        if self.__new_version:
+            return
         if isinstance(data, pd.DataFrame):
             if len(data.columns) == 0:
                 raise TimeseriesDataWithoutColumnsError()
 
             self.__set_date_column(data=data)
             self.__adapt_timeseries(data=data)
 
@@ -180,25 +217,23 @@
         if ratios:
             group_counter = 1
             for value in ratios.values():
                 if group_counter <= 2:
                     group_counter += 1
                     decimals_col = self.__get_round_column(value[0])
                     axis = YAxis(
-                        formatting=formatting.AxisNumberFormatting(
-                            decimals=int(scales[decimals_col].iloc[-1])
-                        )
-                    )
-                    axis.add_series(
-                        *self.__create_timeseries_specs(
+                        series=self.__create_timeseries_specs(
                             data=data,
                             group=value,
                             scales=scales,
                             spec_class=LineSeries,
-                        )
+                        ),
+                        formatting=formatting.AxisNumberFormatting(
+                            decimals=int(scales[decimals_col].iloc[-1])
+                        ),
                     )
                     axis_list.append(axis)
                 else:
                     tooltips += self.__create_timeseries_specs(
                         data=data,
                         group=value,
                         scales=scales,
@@ -294,67 +329,23 @@
                 add multiple series to the same chart. If you want to add multiple
                 charts to the same widget, use set_charts method instead.
 
                 By default, when adding a series, the series will be a line series,
                 if you want to change the type of series, you can pass
                 on series at your choice.
 
-        Examples:
-            ??? example "Add a basic line series"
-                ```py linenums="1"
-                import pandas as pd
-
-                from engineai.sdk.dashboard.dashboard import Dashboard
-                from engineai.sdk.dashboard.widgets import timeseries
-
-                # Create a dataframe
-                df = pd.DataFrame(
-                    {
-                        "date": pd.date_range("2020-01-01", "2020-01-10"),
-                        "column_name_1": [1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
-                        "column_name_2": [10, 9, 8, 7, 6, 5, 4, 3, 2, 1],
-                        "column_name_3": [5, 4, 3, 2, 1, 2, 3, 4, 5, 6],
-                    }
-                )
-                ts = timeseries.Timeseries(df).set_series("column_name_1")
-                Dashboard(content=ts)
-                ```
-
-            ??? example "Add a column series"
-                ```py linenums="15"
-                ts = timeseries.Timeseries(df).set_series(
-                    timeseries.ColumnSeries(data_column="column_name_1")
-                )
-                ```
-
-            ??? example "Add multiple series both line series"
-                ```py linenums="15"
-                ts = timeseries.Timeseries(df).set_series(
-                    "column_name_1", "column_name_2"
-                )
-
-                ```
-
-            ??? example "Add multiple series with different types"
-                ```py linenums="15"
-                # Add multiple series with different types, first series will be
-                # line series, second will be column series and third will be area
-                # series
-
-                ts = timeseries.Timeseries(df).set_series(
-                    "column_name_1",
-                    timeseries.ColumnSeries(data_column="column_name_2"),
-                    timeseries.AreaSeries(data_column="column_name_3"),
-                )
-                ```
-
         Notes:
             If you use set_series method more than once, the previous series
             will be replaced by the new one, same behavior as set_charts method.
         """
+        warnings.warn(
+            "`set_series` method is deprecated and it will be removed in the future.",
+            DeprecationWarning,
+        )
+
         if len(items) == 0:
             raise TimeseriesChartsEmptyDefinitionError()
 
         return self.set_charts(
             Chart(
                 left_y_axis=self.__y_left_axis(*items),
                 right_y_axis=self.__y_right_axis(*items),
@@ -367,77 +358,47 @@
 
         for item in items:
             if isinstance(item, str):
                 series.append(LineSeries(data_column=item))
             elif not item.is_right_axis:
                 series.append(item)
 
-        return YAxis().add_series(*series) if len(series) > 0 else None
+        return YAxis(series=series) if len(series) > 0 else None
 
     @staticmethod
     def __y_right_axis(*items: Union[str, TimeseriesSeries]) -> Optional[YAxis]:
         series: List[TimeseriesSeries] = [
             item
             for item in list(items)
             if not isinstance(item, str) and item.is_right_axis
         ]
-        return YAxis().add_series(*series) if len(series) > 0 else None
+        return YAxis(series=series) if len(series) > 0 else None
 
     @type_check
     def set_charts(self, *items: Union[str, TimeseriesSeries, Chart]) -> "Timeseries":
         """Set charts for timeseries widget.
 
         Allows the addition of one or more charts to a timeseries widget.
         Include multiple charts within the same widget using this method,
         allowing for the simultaneous visualization of
         diverse datasets or metrics
 
         Args:
             items: chart(s) to be added to timeseries widget, using this method you
                 can add multiple charts to the same widget.
 
-        Examples:
-            ??? example "Add a basic chart with a line series"
-                ```py linenums="1"
-                import pandas as pd
-
-                from engineai.sdk.dashboard.dashboard import Dashboard
-                from engineai.sdk.dashboard.widgets import timeseries
-
-                df = pd.DataFrame(
-                    {
-                        "date": pd.date_range("2020-01-01", "2020-01-10"),
-                        "column_name_1": [1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
-                        "column_name_2": [10, 9, 8, 7, 6, 5, 4, 3, 2, 1],
-                    }
-                )
-
-                ts = timeseries.Timeseries(df).set_charts("column_name_1")
-                Dashboard(content=ts)
-                ```
-
-            ??? example "Add a chart with a column series"
-                ```py linenums="14"
-                ts = timeseries.Timeseries(df).set_charts(
-                    timeseries.ColumnSeries(data_column="column_name_1")
-                )
-                ```
-
-            ??? example "Add multiple charts"
-                ```py linenums="14"
-                ts = timeseries.Timeseries(df).set_charts(
-                    "column_name_1",
-                    timeseries.ColumnSeries(data_column="column_name_2")
-                )
-                ```
-
         Notes:
             If you use set_charts method more than once, the previous charts
             will be replaced by the new one, same behavior as set_series method.
         """
+        warnings.warn(
+            "`set_charts` method is deprecated and it will be removed in the future.",
+            DeprecationWarning,
+        )
+
         if len(items) == 0:
             raise TimeseriesChartsEmptyDefinitionError()
 
         if len(items) > 5:
             raise TimeseriesTooManyChartsError(widget_id=self.widget_id)
 
         self.__total_height = 0
@@ -570,30 +531,31 @@
 
         return round(
             int(math.ceil(height / self._WIDGET_HEIGHT_STEP))
             * self._WIDGET_HEIGHT_STEP,
             HEIGHT_ROUND_VALUE,
         )
 
-    def _build_widget_input(self) -> Any:
+    def _build_widget_input(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "TimeseriesWidgetInput",
-            title=build_templated_strings(items=self.__title) if self.__title else None,
-            charts=self._build_charts(),
-            data=build_data(path=self.dependency_id, json_data=self._json_data),
-            periodSelector=self.__period_selector.build(),
-            legend=self.__legend.build(),
-            navigator=self.__navigator.build() if self.__navigator else None,
-            toolbar=build_chart_toolbar(enable=self._enable_toolbar),
-        )
+        return {
+            "title": build_templated_strings(items=self.__title)
+            if self.__title
+            else None,
+            "charts": self._build_charts(),
+            "data": build_data(path=self.dependency_id, json_data=self._json_data),
+            "periodSelector": self.__period_selector.build(),
+            "legend": self.__legend.build(),
+            "navigator": self.__navigator.build() if self.__navigator else None,
+            "toolbar": build_chart_toolbar(enable=self._enable_toolbar),
+        }
 
     def _build_charts(self) -> List[Any]:
         return [chart.build() for chart in self.__charts]
 
     def post_process_data(self, data: StaticDataType) -> StaticDataType:
         """Post process data."""
         if self.date_column != "__index":
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/transform.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/timeseries/transform.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Spec for legend of a timeseries widget."""
 from typing import Any
+from typing import Dict
 from typing import Optional
 from typing import Union
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links.abstract import AbstractFactoryLinkItemsHandler
-from engineai.sdk.dashboard.utils import generate_input
 
 from .enums import TransformChoices
 from .exceptions import TimeseriesTransformScalarRequiredError
 
 
 class Transform(AbstractFactoryLinkItemsHandler):
     """Modify data representation in Timeseries with various transformations.
@@ -45,16 +45,14 @@
             ]
         ) and scalar is None:
             raise TimeseriesTransformScalarRequiredError(transformation=transform.value)
 
         self._transform = transform
         self._scalar = scalar
 
-    def build(self) -> Any:
+    def build(self) -> Dict[str, Any]:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "SeriesTransform", transform=self._transform.value, scalar=self._scalar
-        )
+        return {"transform": self._transform.value, "scalar": self._scalar}
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/toggle/exceptions.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/toggle/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/toggle/toggle.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/toggle/toggle.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Spec for Toggle Widget."""
 
 from typing import Any
+from typing import Dict
 from typing import Optional
 from typing import Union
 
 import pandas as pd
 
 from engineai.sdk.dashboard.data import DataSource
 from engineai.sdk.dashboard.data.http import Http
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.templated_string import build_templated_strings
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.utils import build_data
 
 from ..base import SelectableWidget
 from .exceptions import ToggleValidateValueError
 
 
 class Toggle(SelectableWidget):
@@ -25,14 +25,15 @@
     toggle between different selections or settings.
     """
 
     _DEPENDENCY_ID = "__TOGGLE_DATA_DEPENDENCY__"
     _WIDGET_API_TYPE = "toggle"
     _DEFAULT_HEIGHT = 0.5
     _FORCE_HEIGHT = True
+    _FLUID_ROW_COMPATIBLE = True
 
     @type_check
     def __init__(
         self,
         data: Union[DataSource, pd.DataFrame, Http],
         *,
         id_column: str = "id",
@@ -83,36 +84,34 @@
         """
         super().__init__(widget_id=widget_id, data=data)
         self.__label = label
         self.__label_column = label_column if label_column is not None else id_column
         self.__id_column = id_column
         self.__default_selection = default_selection
 
-    def _build_label(self) -> Any:
+    def _build_label(self) -> Dict[str, Any]:
         """Builds spec for dashboard API.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "ToggleWidgetLabelInput",
-            text=build_templated_strings(items=self.__label),
-        )
+        return {
+            "text": build_templated_strings(items=self.__label),
+        }
 
-    def _build_option(self) -> Any:
+    def _build_option(self) -> Dict[str, Any]:
         """Builds spec for dashboard API.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "ToggleWidgetOptionInput",
-            labelKey=build_templated_strings(items=self.__label_column),
-            idKey=build_templated_strings(items=self.__id_column),
-        )
+        return {
+            "labelKey": build_templated_strings(items=self.__label_column),
+            "idKey": build_templated_strings(items=self.__id_column),
+        }
 
     def validate(self, data: pd.DataFrame, **kwargs: Any) -> None:
         """Validates widget spec.
 
         Args:
             data (DataFrame): pandas DataFrame or dict where
                 the data is present.
@@ -124,29 +123,21 @@
             )
         if self.__id_column not in data.columns:
             raise ToggleValidateValueError(
                 argument="id_column",
                 value=self.__id_column,
             )
 
-    def _build_widget_input(self) -> Any:
+    def _build_widget_input(self) -> Dict[str, Any]:
         """Builds spec for dashboard API.
 
         Returns:
             Input object for Dashboard API
         """
-        return generate_input(
-            "ToggleWidgetInput",
-            label=self._build_label(),
-            data=build_data(path=self.dependency_id),
-            option=self._build_option(),
-            initialState=generate_input(
-                "ToggleWidgetStateInput",
-                selected=build_templated_strings(items=self.__default_selection),
-            ),
-        )
-
-    def build_widget_input(
-        self,
-    ) -> Any:
-        """Method to access the build from outside the class."""
-        return self._build_widget_input()
+        return {
+            "label": self._build_label(),
+            "data": build_data(path=self.dependency_id),
+            "option": self._build_option(),
+            "initialState": {
+                "selected": build_templated_strings(items=self.__default_selection),
+            },
+        }
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/utils.py` & `engineai_sdk-0.92.0/engineai/sdk/dashboard/widgets/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Utils related to Widgets classes."""
 
 from typing import Any
+from typing import Dict
 from typing import Optional
 from typing import get_args
 
-from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.charts.typing import TooltipItem
 from engineai.sdk.dashboard.widgets.components.charts.typing import TooltipItems
 
 COUNTRY_CODES = {
     "FO",
     "US",
     "JP",
@@ -184,26 +184,24 @@
     "IS",
     "EG",
     "KG",
     "NP",
 }
 
 
-def build_data(path: str, json_data: Any = None) -> Any:
+def build_data(path: str, json_data: Any = None) -> Dict[str, Any]:
     """Build Data Input."""
     if json_data is not None:
-        return generate_input(
-            "WidgetDataInput",
-            json=json_data,
-        )
+        return {
+            "json": json_data,
+        }
     else:
-        return generate_input(
-            "WidgetDataInput",
-            dependency=generate_input("WidgetDependencyVariableInput", path=path),
-        )
+        return {
+            "dependency": {"path": path},
+        }
 
 
 def get_tooltips(tooltips: Optional[TooltipItems]) -> Any:
     """Get tooltips."""
     return (
         tooltips
         if isinstance(tooltips, list)
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/internal/authentication/auth0.py` & `engineai_sdk-0.92.0/engineai/sdk/internal/authentication/auth0.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/internal/authentication/utils.py` & `engineai_sdk-0.92.0/engineai/sdk/internal/authentication/utils.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/engineai/sdk/internal/clients/api.py` & `engineai_sdk-0.92.0/engineai/sdk/internal/clients/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 import requests
 import urllib3
 from jwt.exceptions import PyJWTError
 from requests.adapters import CaseInsensitiveDict
 from requests.adapters import HTTPAdapter
 
 from engineai.sdk.internal.authentication.utils import authenticate
-from engineai.sdk.internal.graphql_dataclasses.exceptions import UnauthenticatedError
-from engineai.sdk.internal.graphql_dataclasses.types import APITypes
+from engineai.sdk.internal.exceptions import UnauthenticatedError
 
 from .exceptions import APIServerError
 from .exceptions import APIUrlNotFound
 
 logger = logging.getLogger(__name__)
 logging.getLogger("urllib3").propagate = False
 
@@ -34,18 +33,14 @@
         """Create connector to an API instance.
 
         Args:
             max_retries (int): maximum number of requests retries
         """
         self.__url = self._set_url()
         self.__token = self._get_token()
-        APITypes().set_types(
-            url=self.__url,
-            request_headers={"Authorization": f"Bearer {self.__token}"},
-        )
         self.__session = self.__initialize_session(max_retries=max_retries)
 
     @property
     def url(self) -> str:
         """Get address of dashboard API."""
         return self.__url
 
@@ -63,16 +58,17 @@
             raise APIUrlNotFound()
 
     @staticmethod
     def __initialize_session(max_retries: int = 3) -> requests.Session:
         """Creates a HTTP/HTTPS session and returns."""
         retries = urllib3.Retry(
             total=max_retries,
-            backoff_factor=0.1,
-            status_forcelist=[500, 502, 503, 504, 400, 401],
+            backoff_factor=0.5,
+            status_forcelist=[500, 502, 503, 504],
+            allowed_methods=["POST"],
         )
         adapter = HTTPAdapter(max_retries=retries)
         session = requests.Session()
         session.mount("https://", adapter)
         session.mount("http://", adapter)
         return session
```

### Comparing `engineai_sdk-0.87.2/engineai/sdk/internal/clients/exceptions.py` & `engineai_sdk-0.92.0/engineai/sdk/internal/clients/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.87.2/pyproject.toml` & `engineai_sdk-0.92.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "engineai.sdk"
-version = "0.87.2"
+version = "0.92.0"
 description = "EngineAI's Platform SDK"
 authors = ["Pedro Rodrigues <pedro@dystematic.com>"]
 maintainers = [
   "Pedro Cunha <cunha@engineai.com>",
   "Pedro Feiteira <feiteira@engineai.com>",
   "Li Zixiang <li.zixiang@engineai.com>",
   "Joao Matos <matos@engineai.com>",
```

### Comparing `engineai_sdk-0.87.2/PKG-INFO` & `engineai_sdk-0.92.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: engineai.sdk
-Version: 0.87.2
+Version: 0.92.0
 Summary: EngineAI's Platform SDK
 License: MIT
 Author: Pedro Rodrigues
 Author-email: pedro@dystematic.com
 Maintainer: Pedro Cunha
 Maintainer-email: cunha@engineai.com
 Requires-Python: >=3.8,<3.12
```

