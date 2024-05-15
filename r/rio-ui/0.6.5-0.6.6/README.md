# Comparing `tmp/rio_ui-0.6.5.tar.gz` & `tmp/rio_ui-0.6.6.tar.gz`

## Comparing `rio_ui-0.6.5.tar` & `rio_ui-0.6.6.tar`

### file list

```diff
@@ -1,354 +1,354 @@
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 rio_ui-0.6.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 rio_ui-0.6.5/.prettierrc
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 rio_ui-0.6.5/.sassrc
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 rio_ui-0.6.5/README-DEV.md
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 rio_ui-0.6.5/__init__.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 rio_ui-0.6.5/package.json
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 rio_ui-0.6.5/vite.config.js
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/index.html
--rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/app.ts
--rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/colorConversion.ts
--rw-r--r--   0        0        0    20600 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/componentManagement.ts
--rw-r--r--   0        0        0     5795 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/cssUtils.ts
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/dataModels.ts
--rw-r--r--   0        0        0     6925 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/designApplication.ts
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/easeFunctions.ts
--rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/eventHandling.ts
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/inputBoxTools.ts
--rw-r--r--   0        0        0     6081 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/layoutHelpers.ts
--rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/layouting.ts
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/rippleEffect.ts
--rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/rpc.ts
--rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/rpcFunctions.ts
--rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/utils.ts
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/align.ts
--rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/buildFailed.ts
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/button.ts
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/card.ts
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/classContainer.ts
--rw-r--r--   0        0        0    15146 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/codeExplorer.ts
--rw-r--r--   0        0        0    13820 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/colorPicker.ts
--rw-r--r--   0        0        0    13570 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/componentBase.ts
--rw-r--r--   0        0        0    14334 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/componentTree.ts
--rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/customListItem.ts
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/debuggerConnector.ts
--rw-r--r--   0        0        0    11400 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/drawer.ts
--rw-r--r--   0        0        0    16927 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/dropdown.ts
--rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/flowContainer.ts
--rw-r--r--   0        0        0     5700 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/fundamentalRootComponent.ts
--rw-r--r--   0        0        0    11004 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/grid.ts
--rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/headingListItem.ts
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/html.ts
--rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/icon.ts
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/image.ts
--rw-r--r--   0        0        0    19839 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/keyEventListener.ts
--rw-r--r--   0        0        0    13885 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/linearContainers.ts
--rw-r--r--   0        0        0     4962 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/link.ts
--rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/listView.ts
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/margin.ts
--rw-r--r--   0        0        0     8919 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/markdown.ts
--rw-r--r--   0        0        0    27995 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/mediaPlayer.ts
--rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/mouseEventListener.ts
--rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/multiLineTextInput.ts
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/nodeInput.ts
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/nodeOutput.ts
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/overlay.ts
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/placeholder.ts
--rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/plot.ts
--rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/popup.ts
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/progressBar.ts
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/progressCircle.ts
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/rectangle.ts
--rw-r--r--   0        0        0    10840 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/revealer.ts
--rw-r--r--   0        0        0     9454 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/scrollContainer.ts
--rw-r--r--   0        0        0     6620 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/scrollTarget.ts
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/separator.ts
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/separatorListItem.ts
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/singleContainer.ts
--rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/slider.ts
--rw-r--r--   0        0        0     7104 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/slideshow.ts
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/stack.ts
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/switch.ts
--rw-r--r--   0        0        0     8056 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/switcher.ts
--rw-r--r--   0        0        0    19999 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/switcherBar.ts
--rw-r--r--   0        0        0     8067 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/table.ts
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/text.ts
--rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/textInput.ts
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/themeContextSwitcher.ts
--rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/tooltip.ts
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/code/components/website.ts
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/css/highlightjs-default-dark.css
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/css/highlightjs-default-light.css
--rw-r--r--   0        0        0    51321 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/css/style.scss
--rw-r--r--   0        0        0     8244 2020-02-02 00:00:00.000000 rio_ui-0.6.5/frontend/css/switcheroos.scss
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 rio_ui-0.6.5/prototyping/icon_search.py
--rw-r--r--   0        0        0     7432 2020-02-02 00:00:00.000000 rio_ui-0.6.5/prototyping/pack.py
--rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 rio_ui-0.6.5/prototyping/webgl.html
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 rio_ui-0.6.5/prototyping/node_editor/__main__.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 rio_ui-0.6.5/prototyping/node_editor/index.html
--rw-r--r--   0        0        0    14707 2020-02-02 00:00:00.000000 rio_ui-0.6.5/prototyping/node_editor/script.ts
--rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 rio_ui-0.6.5/prototyping/node_editor/styles.scss
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 rio_ui-0.6.5/raw-icons/custom-material-icons/twinkle.svg
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 rio_ui-0.6.5/raw-icons/custom-material-icons/fill/twinkle.svg
--rw-r--r--   0        0        0    10067 2020-02-02 00:00:00.000000 rio_ui-0.6.5/raw-icons/rio/logo-and-text-horizontal.svg
--rw-r--r--   0        0        0    10127 2020-02-02 00:00:00.000000 rio_ui-0.6.5/raw-icons/rio/logo-and-text-vertical.svg
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 rio_ui-0.6.5/raw-icons/rio/logo.svg
--rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 rio_ui-0.6.5/raw-icons/rio/color/logo-and-text-horizontal.svg
--rw-r--r--   0        0        0     5961 2020-02-02 00:00:00.000000 rio_ui-0.6.5/raw-icons/rio/color/logo-and-text-vertical.svg
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 rio_ui-0.6.5/raw-icons/rio/color/logo.svg
--rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 rio_ui-0.6.5/raw-icons/rio/fill/logo-and-text-horizontal.svg
--rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 rio_ui-0.6.5/raw-icons/rio/fill/logo-and-text-vertical.svg
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 rio_ui-0.6.5/raw-icons/rio/fill/logo.svg
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 rio_ui-0.6.5/raw-icons/styling/corner-round-bottom-left.svg
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 rio_ui-0.6.5/raw-icons/styling/corner-round-bottom-right.svg
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 rio_ui-0.6.5/raw-icons/styling/corner-round-top-left.svg
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 rio_ui-0.6.5/raw-icons/styling/corner-round-top-right.svg
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/__init__.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/__main__.py
--rw-r--r--   0        0        0    19054 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/app.py
--rw-r--r--   0        0        0    32394 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/app_server.py
--rw-r--r--   0        0        0     8673 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/assets.py
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/byte_serving.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/changelog.txt
--rw-r--r--   0        0        0    19465 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/color.py
--rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/common.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/cursor_style.py
--rw-r--r--   0        0        0     5777 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/dataclass.py
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/errors.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/event.py
--rw-r--r--   0        0        0     6691 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/fills.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/global_state.py
--rw-r--r--   0        0        0     9862 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/icon_registry.py
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/inspection.py
--rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/maybes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/py.typed
--rw-r--r--   0        0        0     8059 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/routing.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/self_serializing.py
--rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/serialization.py
--rw-r--r--   0        0        0    81323 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/session.py
--rw-r--r--   0        0        0     8246 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/state_properties.py
--rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/text_style.py
--rw-r--r--   0        0        0    28637 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/theme.py
--rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/user_settings_module.py
--rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/world_units.py
--rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/assets/fonts/Roboto/LICENSE.txt
--rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/assets/fonts/Roboto/Roboto-Bold.ttf
--rw-r--r--   0        0        0   171508 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/assets/fonts/Roboto/Roboto-BoldItalic.ttf
--rw-r--r--   0        0        0   170504 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/assets/fonts/Roboto/Roboto-Italic.ttf
--rw-r--r--   0        0        0   168260 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/assets/fonts/Roboto/Roboto-Regular.ttf
--rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/assets/fonts/Roboto Mono/LICENSE.txt
--rw-r--r--   0        0        0    87392 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/assets/fonts/Roboto Mono/RobotoMono-Bold.ttf
--rw-r--r--   0        0        0    94636 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/assets/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf
--rw-r--r--   0        0        0    94372 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/assets/fonts/Roboto Mono/RobotoMono-Italic.ttf
--rw-r--r--   0        0        0    87236 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/assets/fonts/Roboto Mono/RobotoMono-Regular.ttf
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/assets/hosted/README.md
--rw-r--r--   0        0        0    54189 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png
--rw-r--r--   0        0        0    31665 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/assets/hosted/rio-logos/rio-logo-square.png
--rw-r--r--   0        0        0  1081336 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/assets/icon-sets/material.tar.xz
--rw-r--r--   0        0        0    14992 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/assets/icon-sets/rio.tar.xz
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/assets/icon-sets/styling.tar.xz
--rw-r--r--   0        0        0     7375 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/cli/__init__.py
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/cli/cli_instance.py
--rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/cli/nice_traceback.py
--rw-r--r--   0        0        0    14016 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/cli/project.py
--rw-r--r--   0        0        0    12858 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/cli/project_setup.py
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/cli/rio_api.py
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/cli/rioignore.py
--rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/cli/tomlconfig.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/cli/run_project/__init__.py
--rw-r--r--   0        0        0     5450 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/cli/run_project/app_loading.py
--rw-r--r--   0        0        0    22580 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/cli/run_project/arbiter.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/cli/run_project/file_watcher_worker.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/cli/run_project/run_models.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/cli/run_project/run_utils.py
--rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/cli/run_project/uvicorn_worker.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/cli/run_project/webview_worker.py
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/__init__.py
--rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/app_root.py
--rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/auto_form.py
--rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/banner.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/build_failed.py
--rw-r--r--   0        0        0    12739 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/button.py
--rw-r--r--   0        0        0     5325 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/card.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/class_container.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/code_explorer.py
--rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/color_picker.py
--rw-r--r--   0        0        0    26340 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/component.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/component_tree.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/container.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/debugger_connector.py
--rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/devel_component.py
--rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/drawer.py
--rw-r--r--   0        0        0     6886 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/dropdown.py
--rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/flow_container.py
--rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/fundamental_component.py
--rw-r--r--   0        0        0     7087 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/grid.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/html.py
--rw-r--r--   0        0        0     7709 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/icon.py
--rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/image.py
--rw-r--r--   0        0        0    14201 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/key_event_listener.py
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/labeled_column.py
--rw-r--r--   0        0        0     9705 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/linear_containers.py
--rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/link.py
--rw-r--r--   0        0        0    10178 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/list_items.py
--rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/list_view.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/markdown.py
--rw-r--r--   0        0        0     4991 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/media_player.py
--rw-r--r--   0        0        0     9091 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/mouse_event_listener.py
--rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/multi_line_text_input.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/node_input.py
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/node_output.py
--rw-r--r--   0        0        0     8852 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/number_input.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/overlay.py
--rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/page_view.py
--rw-r--r--   0        0        0     4992 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/plot.py
--rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/popup.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/progress_bar.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/progress_circle.py
--rw-r--r--   0        0        0     5425 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/rectangle.py
--rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/revealer.py
--rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/root_components.py
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/scroll_container.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/scroll_target.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/separator.py
--rw-r--r--   0        0        0     5947 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/slider.py
--rw-r--r--   0        0        0     3585 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/slideshow.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/spacer.py
--rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/stack.py
--rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/switch.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/switcher.py
--rw-r--r--   0        0        0     9204 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/switcher_bar.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/table.py
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/text.py
--rw-r--r--   0        0        0     5772 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/text_input.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/theme_context_switcher.py
--rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/tooltip.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/components/website.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/debug/__init__.py
--rw-r--r--   0        0        0     7485 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/debug/monkeypatches.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/debug/typing_utils.py
--rw-r--r--   0        0        0    14479 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/debug/validator.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/debug/dev_tools/__init__.py
--rw-r--r--   0        0        0    10587 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/debug/dev_tools/component_details.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/debug/dev_tools/deploy_page.py
--rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/debug/dev_tools/dev_tools_sidebar.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/debug/dev_tools/docs_page.py
--rw-r--r--   0        0        0    12890 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/debug/dev_tools/icons_page.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/debug/dev_tools/layout_preview.py
--rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/debug/dev_tools/project_page.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/debug/dev_tools/sample_icons_grid.py
--rw-r--r--   0        0        0    17346 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/debug/dev_tools/theme_picker_page.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/debug/dev_tools/tree_page.py
--rw-r--r--   0        0        0    10303 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/docs/__init__.py
--rw-r--r--   0        0        0   417644 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/generated/index.html
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/patches_for_3rd_party_stuff/_OverlappedFuture_cancel_overlapped.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/patches_for_3rd_party_stuff/__init__.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/README.md
--rw-r--r--   0        0        0    14448 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/__init__.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/howtos/core-classes.md
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/howtos/debugging-setup.md
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/howtos/deployment.md
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/howtos/howto-custom-events.md
--rw-r--r--   0        0        0     5820 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/howtos/howto-get-value-from-child-component.md
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/howtos/howto-install.md
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/howtos/howto-pass-value-to-event.md
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/howtos/persistent-settings.md
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/howtos/project-setup.md
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/howtos/run-project.md
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/howtos/theming.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/howtos-todo/attribute-bindings.md
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/howtos-todo/component-lifecycle.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/howtos-todo/custom-events.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/howtos-todo/force-refresh.md
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/howtos-todo/initialize-component-asynchronously.md
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/howtos-todo/layouting.md
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/howtos-todo/multiple-pages.md
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/other-examples/simple_counter_app.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-AI Chatbot/README.md
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-AI Chatbot/meta.json
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-AI Chatbot/root_init.py
--rw-r--r--   0        0        0   258496 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-AI Chatbot/components/__init__.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py
--rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-AI Chatbot/pages/__init__.py
--rw-r--r--   0        0        0     5823 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/README.md
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/data_models.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/meta.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/root_init.py
--rw-r--r--   0        0        0   270445 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/thumbnail.svg
--rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/assets/cryptos.csv
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/__init__.py
--rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/balance_card.py
--rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_card.py
--rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_chart.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/__init__.py
--rw-r--r--   0        0        0     7668 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/dashboard_page.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Empty/README.md
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Empty/meta.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Empty/root_init.py
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Empty/pages/__init__.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Empty/pages/sample_page.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Simple CRUD/README.md
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Simple CRUD/meta.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Simple CRUD/root_init.py
--rw-r--r--   0        0        0   350009 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Simple CRUD/components/__init__.py
--rw-r--r--   0        0        0     7285 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py
--rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Simple CRUD/pages/__init__.py
--rw-r--r--   0        0        0     8624 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/README.md
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/meta.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/root_init.py
--rw-r--r--   0        0        0    23769 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/__init__.py
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/__init__.py
--rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/components/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/__init__.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/__init__.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/__init__.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/__init__.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/__init__.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/__init__.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/__init__.py
--rw-r--r--   0        0        0     4348 2020-02-02 00:00:00.000000 rio_ui-0.6.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 rio_ui-0.6.5/scripts/benchmark.py
--rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 rio_ui-0.6.5/scripts/build_material_icon_set.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 rio_ui-0.6.5/scripts/cloc.sh
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 rio_ui-0.6.5/scripts/code_coverage.py
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 rio_ui-0.6.5/scripts/publish_new_release.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 rio_ui-0.6.5/tests/test_app_build.py
--rw-r--r--   0        0        0     8822 2020-02-02 00:00:00.000000 rio_ui-0.6.5/tests/test_attribute_bindings.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 rio_ui-0.6.5/tests/test_custom_components.py
--rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 rio_ui-0.6.5/tests/test_docstring_code_blocks.py
--rw-r--r--   0        0        0     3797 2020-02-02 00:00:00.000000 rio_ui-0.6.5/tests/test_documentation.py
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 rio_ui-0.6.5/tests/test_events.py
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 rio_ui-0.6.5/tests/test_project_templates.py
--rw-r--r--   0        0        0    11737 2020-02-02 00:00:00.000000 rio_ui-0.6.5/tests/test_reconciliation.py
--rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 rio_ui-0.6.5/tests/test_refresh.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 rio_ui-0.6.5/tests/test_session.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 rio_ui-0.6.5/tests/test_user_settings.py
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 rio_ui-0.6.5/tests/test_zzz_guardrails.py
--rw-r--r--   0        0        0     8596 2020-02-02 00:00:00.000000 rio_ui-0.6.5/tests/utils.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 rio_ui-0.6.5/.gitignore
--rw-r--r--   0        0        0    11315 2020-02-02 00:00:00.000000 rio_ui-0.6.5/LICENSE.txt
--rw-r--r--   0        0        0     7256 2020-02-02 00:00:00.000000 rio_ui-0.6.5/README.md
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 rio_ui-0.6.5/pyproject.toml
--rw-r--r--   0        0        0    22477 2020-02-02 00:00:00.000000 rio_ui-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 rio_ui-0.6.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 rio_ui-0.6.6/.prettierrc
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 rio_ui-0.6.6/.sassrc
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 rio_ui-0.6.6/README-DEV.md
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 rio_ui-0.6.6/__init__.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 rio_ui-0.6.6/package.json
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 rio_ui-0.6.6/vite.config.js
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/index.html
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/app.ts
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/colorConversion.ts
+-rw-r--r--   0        0        0    20600 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/componentManagement.ts
+-rw-r--r--   0        0        0     5795 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/cssUtils.ts
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/dataModels.ts
+-rw-r--r--   0        0        0     6925 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/designApplication.ts
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/easeFunctions.ts
+-rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/eventHandling.ts
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/inputBoxTools.ts
+-rw-r--r--   0        0        0     6081 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/layoutHelpers.ts
+-rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/layouting.ts
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/rippleEffect.ts
+-rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/rpc.ts
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/rpcFunctions.ts
+-rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/utils.ts
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/align.ts
+-rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/buildFailed.ts
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/button.ts
+-rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/card.ts
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/classContainer.ts
+-rw-r--r--   0        0        0    15146 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/codeExplorer.ts
+-rw-r--r--   0        0        0    13820 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/colorPicker.ts
+-rw-r--r--   0        0        0    13570 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/componentBase.ts
+-rw-r--r--   0        0        0    14334 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/componentTree.ts
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/customListItem.ts
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/debuggerConnector.ts
+-rw-r--r--   0        0        0    11400 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/drawer.ts
+-rw-r--r--   0        0        0    16927 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/dropdown.ts
+-rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/flowContainer.ts
+-rw-r--r--   0        0        0     5700 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/fundamentalRootComponent.ts
+-rw-r--r--   0        0        0    11004 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/grid.ts
+-rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/headingListItem.ts
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/html.ts
+-rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/icon.ts
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/image.ts
+-rw-r--r--   0        0        0    19839 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/keyEventListener.ts
+-rw-r--r--   0        0        0    13885 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/linearContainers.ts
+-rw-r--r--   0        0        0     4962 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/link.ts
+-rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/listView.ts
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/margin.ts
+-rw-r--r--   0        0        0     8919 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/markdown.ts
+-rw-r--r--   0        0        0    27995 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/mediaPlayer.ts
+-rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/mouseEventListener.ts
+-rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/multiLineTextInput.ts
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/nodeInput.ts
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/nodeOutput.ts
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/overlay.ts
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/placeholder.ts
+-rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/plot.ts
+-rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/popup.ts
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/progressBar.ts
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/progressCircle.ts
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/rectangle.ts
+-rw-r--r--   0        0        0    10840 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/revealer.ts
+-rw-r--r--   0        0        0     9454 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/scrollContainer.ts
+-rw-r--r--   0        0        0     6620 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/scrollTarget.ts
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/separator.ts
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/separatorListItem.ts
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/singleContainer.ts
+-rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/slider.ts
+-rw-r--r--   0        0        0     7104 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/slideshow.ts
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/stack.ts
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/switch.ts
+-rw-r--r--   0        0        0     8056 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/switcher.ts
+-rw-r--r--   0        0        0    19999 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/switcherBar.ts
+-rw-r--r--   0        0        0     8067 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/table.ts
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/text.ts
+-rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/textInput.ts
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/themeContextSwitcher.ts
+-rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/tooltip.ts
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/code/components/website.ts
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/css/highlightjs-default-dark.css
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/css/highlightjs-default-light.css
+-rw-r--r--   0        0        0    51321 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/css/style.scss
+-rw-r--r--   0        0        0     8244 2020-02-02 00:00:00.000000 rio_ui-0.6.6/frontend/css/switcheroos.scss
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 rio_ui-0.6.6/prototyping/icon_search.py
+-rw-r--r--   0        0        0     7432 2020-02-02 00:00:00.000000 rio_ui-0.6.6/prototyping/pack.py
+-rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 rio_ui-0.6.6/prototyping/webgl.html
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 rio_ui-0.6.6/prototyping/node_editor/__main__.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 rio_ui-0.6.6/prototyping/node_editor/index.html
+-rw-r--r--   0        0        0    14707 2020-02-02 00:00:00.000000 rio_ui-0.6.6/prototyping/node_editor/script.ts
+-rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 rio_ui-0.6.6/prototyping/node_editor/styles.scss
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 rio_ui-0.6.6/raw-icons/custom-material-icons/twinkle.svg
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 rio_ui-0.6.6/raw-icons/custom-material-icons/fill/twinkle.svg
+-rw-r--r--   0        0        0    10067 2020-02-02 00:00:00.000000 rio_ui-0.6.6/raw-icons/rio/logo-and-text-horizontal.svg
+-rw-r--r--   0        0        0    10127 2020-02-02 00:00:00.000000 rio_ui-0.6.6/raw-icons/rio/logo-and-text-vertical.svg
+-rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 rio_ui-0.6.6/raw-icons/rio/logo.svg
+-rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 rio_ui-0.6.6/raw-icons/rio/color/logo-and-text-horizontal.svg
+-rw-r--r--   0        0        0     5961 2020-02-02 00:00:00.000000 rio_ui-0.6.6/raw-icons/rio/color/logo-and-text-vertical.svg
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 rio_ui-0.6.6/raw-icons/rio/color/logo.svg
+-rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 rio_ui-0.6.6/raw-icons/rio/fill/logo-and-text-horizontal.svg
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 rio_ui-0.6.6/raw-icons/rio/fill/logo-and-text-vertical.svg
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 rio_ui-0.6.6/raw-icons/rio/fill/logo.svg
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 rio_ui-0.6.6/raw-icons/styling/corner-round-bottom-left.svg
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 rio_ui-0.6.6/raw-icons/styling/corner-round-bottom-right.svg
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 rio_ui-0.6.6/raw-icons/styling/corner-round-top-left.svg
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 rio_ui-0.6.6/raw-icons/styling/corner-round-top-right.svg
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/__init__.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/__main__.py
+-rw-r--r--   0        0        0    19054 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/app.py
+-rw-r--r--   0        0        0    32394 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/app_server.py
+-rw-r--r--   0        0        0     8673 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/assets.py
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/byte_serving.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/changelog.txt
+-rw-r--r--   0        0        0    19465 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/color.py
+-rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/common.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/cursor_style.py
+-rw-r--r--   0        0        0     5777 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/dataclass.py
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/errors.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/event.py
+-rw-r--r--   0        0        0     6691 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/fills.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/global_state.py
+-rw-r--r--   0        0        0     9862 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/icon_registry.py
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/inspection.py
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/maybes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/py.typed
+-rw-r--r--   0        0        0     8059 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/routing.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/self_serializing.py
+-rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/serialization.py
+-rw-r--r--   0        0        0    81323 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/session.py
+-rw-r--r--   0        0        0     8246 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/state_properties.py
+-rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/text_style.py
+-rw-r--r--   0        0        0    28637 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/theme.py
+-rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/user_settings_module.py
+-rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/world_units.py
+-rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/assets/fonts/Roboto/LICENSE.txt
+-rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/assets/fonts/Roboto/Roboto-Bold.ttf
+-rw-r--r--   0        0        0   171508 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/assets/fonts/Roboto/Roboto-BoldItalic.ttf
+-rw-r--r--   0        0        0   170504 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/assets/fonts/Roboto/Roboto-Italic.ttf
+-rw-r--r--   0        0        0   168260 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/assets/fonts/Roboto/Roboto-Regular.ttf
+-rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/assets/fonts/Roboto Mono/LICENSE.txt
+-rw-r--r--   0        0        0    87392 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/assets/fonts/Roboto Mono/RobotoMono-Bold.ttf
+-rw-r--r--   0        0        0    94636 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/assets/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf
+-rw-r--r--   0        0        0    94372 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/assets/fonts/Roboto Mono/RobotoMono-Italic.ttf
+-rw-r--r--   0        0        0    87236 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/assets/fonts/Roboto Mono/RobotoMono-Regular.ttf
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/assets/hosted/README.md
+-rw-r--r--   0        0        0    54189 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png
+-rw-r--r--   0        0        0    31665 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/assets/hosted/rio-logos/rio-logo-square.png
+-rw-r--r--   0        0        0  1081336 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/assets/icon-sets/material.tar.xz
+-rw-r--r--   0        0        0    14992 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/assets/icon-sets/rio.tar.xz
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/assets/icon-sets/styling.tar.xz
+-rw-r--r--   0        0        0     7375 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/cli/__init__.py
+-rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/cli/cli_instance.py
+-rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/cli/nice_traceback.py
+-rw-r--r--   0        0        0    14016 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/cli/project.py
+-rw-r--r--   0        0        0    12858 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/cli/project_setup.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/cli/rio_api.py
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/cli/rioignore.py
+-rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/cli/tomlconfig.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/cli/run_project/__init__.py
+-rw-r--r--   0        0        0     5450 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/cli/run_project/app_loading.py
+-rw-r--r--   0        0        0    22580 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/cli/run_project/arbiter.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/cli/run_project/file_watcher_worker.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/cli/run_project/run_models.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/cli/run_project/run_utils.py
+-rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/cli/run_project/uvicorn_worker.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/cli/run_project/webview_worker.py
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/__init__.py
+-rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/app_root.py
+-rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/auto_form.py
+-rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/banner.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/build_failed.py
+-rw-r--r--   0        0        0    12739 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/button.py
+-rw-r--r--   0        0        0     5325 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/card.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/class_container.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/code_explorer.py
+-rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/color_picker.py
+-rw-r--r--   0        0        0    26340 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/component.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/component_tree.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/container.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/debugger_connector.py
+-rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/devel_component.py
+-rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/drawer.py
+-rw-r--r--   0        0        0     6886 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/dropdown.py
+-rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/flow_container.py
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/fundamental_component.py
+-rw-r--r--   0        0        0     7087 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/grid.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/html.py
+-rw-r--r--   0        0        0     7709 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/icon.py
+-rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/image.py
+-rw-r--r--   0        0        0    14201 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/key_event_listener.py
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/labeled_column.py
+-rw-r--r--   0        0        0     9705 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/linear_containers.py
+-rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/link.py
+-rw-r--r--   0        0        0    10178 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/list_items.py
+-rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/list_view.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/markdown.py
+-rw-r--r--   0        0        0     4991 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/media_player.py
+-rw-r--r--   0        0        0     9091 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/mouse_event_listener.py
+-rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/multi_line_text_input.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/node_input.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/node_output.py
+-rw-r--r--   0        0        0     8919 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/number_input.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/overlay.py
+-rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/page_view.py
+-rw-r--r--   0        0        0     4992 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/plot.py
+-rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/popup.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/progress_bar.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/progress_circle.py
+-rw-r--r--   0        0        0     5425 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/rectangle.py
+-rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/revealer.py
+-rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/root_components.py
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/scroll_container.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/scroll_target.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/separator.py
+-rw-r--r--   0        0        0     5947 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/slider.py
+-rw-r--r--   0        0        0     3585 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/slideshow.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/spacer.py
+-rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/stack.py
+-rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/switch.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/switcher.py
+-rw-r--r--   0        0        0     9204 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/switcher_bar.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/table.py
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/text.py
+-rw-r--r--   0        0        0     5772 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/text_input.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/theme_context_switcher.py
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/tooltip.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/components/website.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/debug/__init__.py
+-rw-r--r--   0        0        0     7485 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/debug/monkeypatches.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/debug/typing_utils.py
+-rw-r--r--   0        0        0    14479 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/debug/validator.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/debug/dev_tools/__init__.py
+-rw-r--r--   0        0        0    10587 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/debug/dev_tools/component_details.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/debug/dev_tools/deploy_page.py
+-rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/debug/dev_tools/dev_tools_sidebar.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/debug/dev_tools/docs_page.py
+-rw-r--r--   0        0        0    12890 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/debug/dev_tools/icons_page.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/debug/dev_tools/layout_preview.py
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/debug/dev_tools/project_page.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/debug/dev_tools/sample_icons_grid.py
+-rw-r--r--   0        0        0    17346 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/debug/dev_tools/theme_picker_page.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/debug/dev_tools/tree_page.py
+-rw-r--r--   0        0        0    10303 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/docs/__init__.py
+-rw-r--r--   0        0        0   417644 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/generated/index.html
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/patches_for_3rd_party_stuff/_OverlappedFuture_cancel_overlapped.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/patches_for_3rd_party_stuff/__init__.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/README.md
+-rw-r--r--   0        0        0    14448 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/__init__.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/howtos/core-classes.md
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/howtos/debugging-setup.md
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/howtos/deployment.md
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/howtos/howto-custom-events.md
+-rw-r--r--   0        0        0     5820 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/howtos/howto-get-value-from-child-component.md
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/howtos/howto-install.md
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/howtos/howto-pass-value-to-event.md
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/howtos/persistent-settings.md
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/howtos/project-setup.md
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/howtos/run-project.md
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/howtos/theming.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/howtos-todo/attribute-bindings.md
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/howtos-todo/component-lifecycle.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/howtos-todo/custom-events.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/howtos-todo/force-refresh.md
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/howtos-todo/initialize-component-asynchronously.md
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/howtos-todo/layouting.md
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/howtos-todo/multiple-pages.md
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/other-examples/simple_counter_app.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-AI Chatbot/README.md
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-AI Chatbot/meta.json
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-AI Chatbot/root_init.py
+-rw-r--r--   0        0        0   258496 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/__init__.py
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py
+-rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-AI Chatbot/pages/__init__.py
+-rw-r--r--   0        0        0     5823 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/README.md
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/data_models.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/meta.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/root_init.py
+-rw-r--r--   0        0        0   270445 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/thumbnail.svg
+-rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/assets/cryptos.csv
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/__init__.py
+-rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/balance_card.py
+-rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_card.py
+-rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_chart.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/__init__.py
+-rw-r--r--   0        0        0     7668 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/dashboard_page.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Empty/README.md
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Empty/meta.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Empty/root_init.py
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Empty/pages/__init__.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Empty/pages/sample_page.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Simple CRUD/README.md
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Simple CRUD/meta.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Simple CRUD/root_init.py
+-rw-r--r--   0        0        0   350009 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Simple CRUD/components/__init__.py
+-rw-r--r--   0        0        0     7285 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py
+-rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Simple CRUD/pages/__init__.py
+-rw-r--r--   0        0        0     8624 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/README.md
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/meta.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/root_init.py
+-rw-r--r--   0        0        0    23769 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/__init__.py
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/__init__.py
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/components/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/__init__.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/__init__.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/__init__.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/__init__.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/__init__.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/__init__.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/__init__.py
+-rw-r--r--   0        0        0     4348 2020-02-02 00:00:00.000000 rio_ui-0.6.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 rio_ui-0.6.6/scripts/benchmark.py
+-rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 rio_ui-0.6.6/scripts/build_material_icon_set.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 rio_ui-0.6.6/scripts/cloc.sh
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 rio_ui-0.6.6/scripts/code_coverage.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 rio_ui-0.6.6/scripts/publish_new_release.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 rio_ui-0.6.6/tests/test_app_build.py
+-rw-r--r--   0        0        0     8822 2020-02-02 00:00:00.000000 rio_ui-0.6.6/tests/test_attribute_bindings.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 rio_ui-0.6.6/tests/test_custom_components.py
+-rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 rio_ui-0.6.6/tests/test_docstring_code_blocks.py
+-rw-r--r--   0        0        0     3797 2020-02-02 00:00:00.000000 rio_ui-0.6.6/tests/test_documentation.py
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 rio_ui-0.6.6/tests/test_events.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 rio_ui-0.6.6/tests/test_project_templates.py
+-rw-r--r--   0        0        0    11737 2020-02-02 00:00:00.000000 rio_ui-0.6.6/tests/test_reconciliation.py
+-rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 rio_ui-0.6.6/tests/test_refresh.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 rio_ui-0.6.6/tests/test_session.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 rio_ui-0.6.6/tests/test_user_settings.py
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 rio_ui-0.6.6/tests/test_zzz_guardrails.py
+-rw-r--r--   0        0        0     8596 2020-02-02 00:00:00.000000 rio_ui-0.6.6/tests/utils.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 rio_ui-0.6.6/.gitignore
+-rw-r--r--   0        0        0    11315 2020-02-02 00:00:00.000000 rio_ui-0.6.6/LICENSE.txt
+-rw-r--r--   0        0        0     7256 2020-02-02 00:00:00.000000 rio_ui-0.6.6/README.md
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 rio_ui-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0    22477 2020-02-02 00:00:00.000000 rio_ui-0.6.6/PKG-INFO
```

### Comparing `rio_ui-0.6.5/README-DEV.md` & `rio_ui-0.6.6/README-DEV.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/package.json` & `rio_ui-0.6.6/package.json`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/index.html` & `rio_ui-0.6.6/frontend/index.html`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/app.ts` & `rio_ui-0.6.6/frontend/code/app.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/colorConversion.ts` & `rio_ui-0.6.6/frontend/code/colorConversion.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/componentManagement.ts` & `rio_ui-0.6.6/frontend/code/componentManagement.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/cssUtils.ts` & `rio_ui-0.6.6/frontend/code/cssUtils.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/dataModels.ts` & `rio_ui-0.6.6/frontend/code/dataModels.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/designApplication.ts` & `rio_ui-0.6.6/frontend/code/designApplication.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/easeFunctions.ts` & `rio_ui-0.6.6/frontend/code/easeFunctions.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/eventHandling.ts` & `rio_ui-0.6.6/frontend/code/eventHandling.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/inputBoxTools.ts` & `rio_ui-0.6.6/frontend/code/inputBoxTools.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/layoutHelpers.ts` & `rio_ui-0.6.6/frontend/code/layoutHelpers.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/layouting.ts` & `rio_ui-0.6.6/frontend/code/layouting.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/rippleEffect.ts` & `rio_ui-0.6.6/frontend/code/rippleEffect.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/rpc.ts` & `rio_ui-0.6.6/frontend/code/rpc.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/rpcFunctions.ts` & `rio_ui-0.6.6/frontend/code/rpcFunctions.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/utils.ts` & `rio_ui-0.6.6/frontend/code/utils.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/align.ts` & `rio_ui-0.6.6/frontend/code/components/align.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/buildFailed.ts` & `rio_ui-0.6.6/frontend/code/components/buildFailed.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/button.ts` & `rio_ui-0.6.6/frontend/code/components/button.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/card.ts` & `rio_ui-0.6.6/frontend/code/components/card.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/classContainer.ts` & `rio_ui-0.6.6/frontend/code/components/classContainer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/codeExplorer.ts` & `rio_ui-0.6.6/frontend/code/components/codeExplorer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/colorPicker.ts` & `rio_ui-0.6.6/frontend/code/components/colorPicker.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/componentBase.ts` & `rio_ui-0.6.6/frontend/code/components/componentBase.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/componentTree.ts` & `rio_ui-0.6.6/frontend/code/components/componentTree.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/customListItem.ts` & `rio_ui-0.6.6/frontend/code/components/customListItem.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/debuggerConnector.ts` & `rio_ui-0.6.6/frontend/code/components/debuggerConnector.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/drawer.ts` & `rio_ui-0.6.6/frontend/code/components/drawer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/dropdown.ts` & `rio_ui-0.6.6/frontend/code/components/dropdown.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/flowContainer.ts` & `rio_ui-0.6.6/frontend/code/components/flowContainer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/fundamentalRootComponent.ts` & `rio_ui-0.6.6/frontend/code/components/fundamentalRootComponent.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/grid.ts` & `rio_ui-0.6.6/frontend/code/components/grid.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/headingListItem.ts` & `rio_ui-0.6.6/frontend/code/components/headingListItem.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/html.ts` & `rio_ui-0.6.6/frontend/code/components/html.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/icon.ts` & `rio_ui-0.6.6/frontend/code/components/icon.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/image.ts` & `rio_ui-0.6.6/frontend/code/components/image.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/keyEventListener.ts` & `rio_ui-0.6.6/frontend/code/components/keyEventListener.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/linearContainers.ts` & `rio_ui-0.6.6/frontend/code/components/linearContainers.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/link.ts` & `rio_ui-0.6.6/frontend/code/components/link.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/listView.ts` & `rio_ui-0.6.6/frontend/code/components/listView.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/margin.ts` & `rio_ui-0.6.6/frontend/code/components/margin.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/markdown.ts` & `rio_ui-0.6.6/frontend/code/components/markdown.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/mediaPlayer.ts` & `rio_ui-0.6.6/frontend/code/components/mediaPlayer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/mouseEventListener.ts` & `rio_ui-0.6.6/frontend/code/components/mouseEventListener.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/multiLineTextInput.ts` & `rio_ui-0.6.6/frontend/code/components/multiLineTextInput.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/nodeInput.ts` & `rio_ui-0.6.6/frontend/code/components/nodeInput.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/nodeOutput.ts` & `rio_ui-0.6.6/frontend/code/components/nodeOutput.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/overlay.ts` & `rio_ui-0.6.6/frontend/code/components/overlay.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/placeholder.ts` & `rio_ui-0.6.6/frontend/code/components/placeholder.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/plot.ts` & `rio_ui-0.6.6/frontend/code/components/plot.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/popup.ts` & `rio_ui-0.6.6/frontend/code/components/popup.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/progressBar.ts` & `rio_ui-0.6.6/frontend/code/components/progressBar.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/progressCircle.ts` & `rio_ui-0.6.6/frontend/code/components/progressCircle.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/rectangle.ts` & `rio_ui-0.6.6/frontend/code/components/rectangle.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/revealer.ts` & `rio_ui-0.6.6/frontend/code/components/revealer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/scrollContainer.ts` & `rio_ui-0.6.6/frontend/code/components/scrollContainer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/scrollTarget.ts` & `rio_ui-0.6.6/frontend/code/components/scrollTarget.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/separator.ts` & `rio_ui-0.6.6/frontend/code/components/separator.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/separatorListItem.ts` & `rio_ui-0.6.6/frontend/code/components/separatorListItem.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/singleContainer.ts` & `rio_ui-0.6.6/frontend/code/components/singleContainer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/slider.ts` & `rio_ui-0.6.6/frontend/code/components/slider.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/slideshow.ts` & `rio_ui-0.6.6/frontend/code/components/slideshow.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/stack.ts` & `rio_ui-0.6.6/frontend/code/components/stack.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/switch.ts` & `rio_ui-0.6.6/frontend/code/components/switch.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/switcher.ts` & `rio_ui-0.6.6/frontend/code/components/switcher.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/switcherBar.ts` & `rio_ui-0.6.6/frontend/code/components/switcherBar.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/table.ts` & `rio_ui-0.6.6/frontend/code/components/table.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/text.ts` & `rio_ui-0.6.6/frontend/code/components/text.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/textInput.ts` & `rio_ui-0.6.6/frontend/code/components/textInput.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/themeContextSwitcher.ts` & `rio_ui-0.6.6/frontend/code/components/themeContextSwitcher.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/tooltip.ts` & `rio_ui-0.6.6/frontend/code/components/tooltip.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/code/components/website.ts` & `rio_ui-0.6.6/frontend/code/components/website.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/css/highlightjs-default-dark.css` & `rio_ui-0.6.6/frontend/css/highlightjs-default-dark.css`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/css/highlightjs-default-light.css` & `rio_ui-0.6.6/frontend/css/highlightjs-default-light.css`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/css/style.scss` & `rio_ui-0.6.6/frontend/css/style.scss`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/frontend/css/switcheroos.scss` & `rio_ui-0.6.6/frontend/css/switcheroos.scss`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/prototyping/icon_search.py` & `rio_ui-0.6.6/prototyping/icon_search.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/prototyping/pack.py` & `rio_ui-0.6.6/prototyping/pack.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/prototyping/webgl.html` & `rio_ui-0.6.6/prototyping/webgl.html`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/prototyping/node_editor/__main__.py` & `rio_ui-0.6.6/prototyping/node_editor/__main__.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/prototyping/node_editor/index.html` & `rio_ui-0.6.6/prototyping/node_editor/index.html`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/prototyping/node_editor/script.ts` & `rio_ui-0.6.6/prototyping/node_editor/script.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/prototyping/node_editor/styles.scss` & `rio_ui-0.6.6/prototyping/node_editor/styles.scss`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/raw-icons/custom-material-icons/twinkle.svg` & `rio_ui-0.6.6/raw-icons/custom-material-icons/twinkle.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/raw-icons/custom-material-icons/fill/twinkle.svg` & `rio_ui-0.6.6/raw-icons/custom-material-icons/fill/twinkle.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/raw-icons/rio/logo-and-text-horizontal.svg` & `rio_ui-0.6.6/raw-icons/rio/logo-and-text-horizontal.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/raw-icons/rio/logo-and-text-vertical.svg` & `rio_ui-0.6.6/raw-icons/rio/logo-and-text-vertical.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/raw-icons/rio/logo.svg` & `rio_ui-0.6.6/raw-icons/rio/logo.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/raw-icons/rio/color/logo-and-text-horizontal.svg` & `rio_ui-0.6.6/raw-icons/rio/color/logo-and-text-horizontal.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/raw-icons/rio/color/logo-and-text-vertical.svg` & `rio_ui-0.6.6/raw-icons/rio/color/logo-and-text-vertical.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/raw-icons/rio/color/logo.svg` & `rio_ui-0.6.6/raw-icons/rio/color/logo.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/raw-icons/rio/fill/logo-and-text-horizontal.svg` & `rio_ui-0.6.6/raw-icons/rio/fill/logo-and-text-horizontal.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/raw-icons/rio/fill/logo-and-text-vertical.svg` & `rio_ui-0.6.6/raw-icons/rio/fill/logo-and-text-vertical.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/raw-icons/rio/fill/logo.svg` & `rio_ui-0.6.6/raw-icons/rio/fill/logo.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/raw-icons/styling/corner-round-bottom-left.svg` & `rio_ui-0.6.6/raw-icons/styling/corner-round-bottom-left.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/raw-icons/styling/corner-round-bottom-right.svg` & `rio_ui-0.6.6/raw-icons/styling/corner-round-bottom-right.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/raw-icons/styling/corner-round-top-left.svg` & `rio_ui-0.6.6/raw-icons/styling/corner-round-top-left.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/raw-icons/styling/corner-round-top-right.svg` & `rio_ui-0.6.6/raw-icons/styling/corner-round-top-right.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/__init__.py` & `rio_ui-0.6.6/rio/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.6.5"
+__version__ = "0.6.6"
 
 import logging
 
 _logger = logging.getLogger(__name__)
 
 # Re-export dataclass stuff for easy use.
 from dataclasses import KW_ONLY as KW_ONLY
```

### Comparing `rio_ui-0.6.5/rio/app.py` & `rio_ui-0.6.6/rio/app.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/app_server.py` & `rio_ui-0.6.6/rio/app_server.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/assets.py` & `rio_ui-0.6.6/rio/assets.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/byte_serving.py` & `rio_ui-0.6.6/rio/byte_serving.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/color.py` & `rio_ui-0.6.6/rio/color.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/common.py` & `rio_ui-0.6.6/rio/common.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/dataclass.py` & `rio_ui-0.6.6/rio/dataclass.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/errors.py` & `rio_ui-0.6.6/rio/errors.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/event.py` & `rio_ui-0.6.6/rio/event.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/fills.py` & `rio_ui-0.6.6/rio/fills.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/global_state.py` & `rio_ui-0.6.6/rio/global_state.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/icon_registry.py` & `rio_ui-0.6.6/rio/icon_registry.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/inspection.py` & `rio_ui-0.6.6/rio/inspection.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/maybes.py` & `rio_ui-0.6.6/rio/maybes.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/routing.py` & `rio_ui-0.6.6/rio/routing.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/serialization.py` & `rio_ui-0.6.6/rio/serialization.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/session.py` & `rio_ui-0.6.6/rio/session.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/state_properties.py` & `rio_ui-0.6.6/rio/state_properties.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/text_style.py` & `rio_ui-0.6.6/rio/text_style.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/theme.py` & `rio_ui-0.6.6/rio/theme.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/user_settings_module.py` & `rio_ui-0.6.6/rio/user_settings_module.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/world_units.py` & `rio_ui-0.6.6/rio/world_units.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/assets/fonts/Roboto/LICENSE.txt` & `rio_ui-0.6.6/rio/assets/fonts/Roboto/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/assets/fonts/Roboto/Roboto-Bold.ttf` & `rio_ui-0.6.6/rio/assets/fonts/Roboto/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/assets/fonts/Roboto/Roboto-BoldItalic.ttf` & `rio_ui-0.6.6/rio/assets/fonts/Roboto/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/assets/fonts/Roboto/Roboto-Italic.ttf` & `rio_ui-0.6.6/rio/assets/fonts/Roboto/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/assets/fonts/Roboto/Roboto-Regular.ttf` & `rio_ui-0.6.6/rio/assets/fonts/Roboto/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/assets/fonts/Roboto Mono/LICENSE.txt` & `rio_ui-0.6.6/rio/assets/fonts/Roboto Mono/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/assets/fonts/Roboto Mono/RobotoMono-Bold.ttf` & `rio_ui-0.6.6/rio/assets/fonts/Roboto Mono/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/assets/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf` & `rio_ui-0.6.6/rio/assets/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/assets/fonts/Roboto Mono/RobotoMono-Italic.ttf` & `rio_ui-0.6.6/rio/assets/fonts/Roboto Mono/RobotoMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/assets/fonts/Roboto Mono/RobotoMono-Regular.ttf` & `rio_ui-0.6.6/rio/assets/fonts/Roboto Mono/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png` & `rio_ui-0.6.6/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/assets/hosted/rio-logos/rio-logo-square.png` & `rio_ui-0.6.6/rio/assets/hosted/rio-logos/rio-logo-square.png`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/assets/icon-sets/material.tar.xz` & `rio_ui-0.6.6/rio/assets/icon-sets/material.tar.xz`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/assets/icon-sets/rio.tar.xz` & `rio_ui-0.6.6/rio/assets/icon-sets/rio.tar.xz`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/assets/icon-sets/styling.tar.xz` & `rio_ui-0.6.6/rio/assets/icon-sets/styling.tar.xz`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/cli/__init__.py` & `rio_ui-0.6.6/rio/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/cli/cli_instance.py` & `rio_ui-0.6.6/rio/cli/cli_instance.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/cli/nice_traceback.py` & `rio_ui-0.6.6/rio/cli/nice_traceback.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/cli/project.py` & `rio_ui-0.6.6/rio/cli/project.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/cli/project_setup.py` & `rio_ui-0.6.6/rio/cli/project_setup.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/cli/rio_api.py` & `rio_ui-0.6.6/rio/cli/rio_api.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/cli/rioignore.py` & `rio_ui-0.6.6/rio/cli/rioignore.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/cli/tomlconfig.py` & `rio_ui-0.6.6/rio/cli/tomlconfig.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/cli/run_project/app_loading.py` & `rio_ui-0.6.6/rio/cli/run_project/app_loading.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/cli/run_project/arbiter.py` & `rio_ui-0.6.6/rio/cli/run_project/arbiter.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/cli/run_project/file_watcher_worker.py` & `rio_ui-0.6.6/rio/cli/run_project/file_watcher_worker.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/cli/run_project/uvicorn_worker.py` & `rio_ui-0.6.6/rio/cli/run_project/uvicorn_worker.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/cli/run_project/webview_worker.py` & `rio_ui-0.6.6/rio/cli/run_project/webview_worker.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/__init__.py` & `rio_ui-0.6.6/rio/components/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/app_root.py` & `rio_ui-0.6.6/rio/components/app_root.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/auto_form.py` & `rio_ui-0.6.6/rio/components/auto_form.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/banner.py` & `rio_ui-0.6.6/rio/components/banner.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/build_failed.py` & `rio_ui-0.6.6/rio/components/build_failed.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/button.py` & `rio_ui-0.6.6/rio/components/button.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/card.py` & `rio_ui-0.6.6/rio/components/card.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/class_container.py` & `rio_ui-0.6.6/rio/components/class_container.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/color_picker.py` & `rio_ui-0.6.6/rio/components/color_picker.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/component.py` & `rio_ui-0.6.6/rio/components/component.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/component_tree.py` & `rio_ui-0.6.6/rio/components/component_tree.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/container.py` & `rio_ui-0.6.6/rio/components/container.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/devel_component.py` & `rio_ui-0.6.6/rio/components/devel_component.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/drawer.py` & `rio_ui-0.6.6/rio/components/drawer.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/dropdown.py` & `rio_ui-0.6.6/rio/components/dropdown.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/flow_container.py` & `rio_ui-0.6.6/rio/components/flow_container.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/fundamental_component.py` & `rio_ui-0.6.6/rio/components/fundamental_component.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/grid.py` & `rio_ui-0.6.6/rio/components/grid.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/html.py` & `rio_ui-0.6.6/rio/components/html.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/icon.py` & `rio_ui-0.6.6/rio/components/icon.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/image.py` & `rio_ui-0.6.6/rio/components/image.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/key_event_listener.py` & `rio_ui-0.6.6/rio/components/key_event_listener.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/labeled_column.py` & `rio_ui-0.6.6/rio/components/labeled_column.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/linear_containers.py` & `rio_ui-0.6.6/rio/components/linear_containers.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/link.py` & `rio_ui-0.6.6/rio/components/link.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/list_items.py` & `rio_ui-0.6.6/rio/components/list_items.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/list_view.py` & `rio_ui-0.6.6/rio/components/list_view.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/markdown.py` & `rio_ui-0.6.6/rio/components/markdown.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/media_player.py` & `rio_ui-0.6.6/rio/components/media_player.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/mouse_event_listener.py` & `rio_ui-0.6.6/rio/components/mouse_event_listener.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/multi_line_text_input.py` & `rio_ui-0.6.6/rio/components/multi_line_text_input.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/node_input.py` & `rio_ui-0.6.6/rio/components/node_input.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/node_output.py` & `rio_ui-0.6.6/rio/components/node_output.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/number_input.py` & `rio_ui-0.6.6/rio/components/number_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,9 +287,14 @@
             is_valid=self.is_valid,
             on_change=self._on_change,
             on_confirm=self._on_confirm,
         )
         return self._text_input
 
     async def grab_keyboard_focus(self) -> None:
+        """
+        ## Metadata
+
+        public: False
+        """
         if self._text_input is not None:
             await self._text_input.grab_keyboard_focus()
```

### Comparing `rio_ui-0.6.5/rio/components/overlay.py` & `rio_ui-0.6.6/rio/components/overlay.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/page_view.py` & `rio_ui-0.6.6/rio/components/page_view.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/plot.py` & `rio_ui-0.6.6/rio/components/plot.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/popup.py` & `rio_ui-0.6.6/rio/components/popup.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/progress_bar.py` & `rio_ui-0.6.6/rio/components/progress_bar.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/progress_circle.py` & `rio_ui-0.6.6/rio/components/progress_circle.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/rectangle.py` & `rio_ui-0.6.6/rio/components/rectangle.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/revealer.py` & `rio_ui-0.6.6/rio/components/revealer.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/root_components.py` & `rio_ui-0.6.6/rio/components/root_components.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/scroll_container.py` & `rio_ui-0.6.6/rio/components/scroll_container.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/scroll_target.py` & `rio_ui-0.6.6/rio/components/scroll_target.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/separator.py` & `rio_ui-0.6.6/rio/components/separator.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/slider.py` & `rio_ui-0.6.6/rio/components/slider.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/slideshow.py` & `rio_ui-0.6.6/rio/components/slideshow.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/spacer.py` & `rio_ui-0.6.6/rio/components/spacer.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/stack.py` & `rio_ui-0.6.6/rio/components/stack.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/switch.py` & `rio_ui-0.6.6/rio/components/switch.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/switcher.py` & `rio_ui-0.6.6/rio/components/switcher.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/switcher_bar.py` & `rio_ui-0.6.6/rio/components/switcher_bar.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/table.py` & `rio_ui-0.6.6/rio/components/table.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/text.py` & `rio_ui-0.6.6/rio/components/text.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/text_input.py` & `rio_ui-0.6.6/rio/components/text_input.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/theme_context_switcher.py` & `rio_ui-0.6.6/rio/components/theme_context_switcher.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/tooltip.py` & `rio_ui-0.6.6/rio/components/tooltip.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/components/website.py` & `rio_ui-0.6.6/rio/components/website.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/debug/monkeypatches.py` & `rio_ui-0.6.6/rio/debug/monkeypatches.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/debug/typing_utils.py` & `rio_ui-0.6.6/rio/debug/typing_utils.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/debug/validator.py` & `rio_ui-0.6.6/rio/debug/validator.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/debug/dev_tools/component_details.py` & `rio_ui-0.6.6/rio/debug/dev_tools/component_details.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/debug/dev_tools/deploy_page.py` & `rio_ui-0.6.6/rio/debug/dev_tools/deploy_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/debug/dev_tools/dev_tools_sidebar.py` & `rio_ui-0.6.6/rio/debug/dev_tools/dev_tools_sidebar.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/debug/dev_tools/docs_page.py` & `rio_ui-0.6.6/rio/debug/dev_tools/docs_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/debug/dev_tools/icons_page.py` & `rio_ui-0.6.6/rio/debug/dev_tools/icons_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/debug/dev_tools/layout_preview.py` & `rio_ui-0.6.6/rio/debug/dev_tools/layout_preview.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/debug/dev_tools/project_page.py` & `rio_ui-0.6.6/rio/debug/dev_tools/project_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/debug/dev_tools/sample_icons_grid.py` & `rio_ui-0.6.6/rio/debug/dev_tools/sample_icons_grid.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/debug/dev_tools/theme_picker_page.py` & `rio_ui-0.6.6/rio/debug/dev_tools/theme_picker_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/debug/dev_tools/tree_page.py` & `rio_ui-0.6.6/rio/debug/dev_tools/tree_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/docs/__init__.py` & `rio_ui-0.6.6/rio/docs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -330,15 +330,15 @@
                 "Session",
             )
             and func.name == "__init__"
         ):
             keep = False
 
         # Check if it's explicitly excluded
-        if not docs.metadata.public:
+        if not func.metadata.public:
             keep = False
 
         # Strip it out, if necessary
         if keep:
             index += 1
         else:
             del docs.functions[index]
```

### Comparing `rio_ui-0.6.5/rio/generated/index.html` & `rio_ui-0.6.6/rio/generated/index.html`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py` & `rio_ui-0.6.6/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py` & `rio_ui-0.6.6/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/patches_for_3rd_party_stuff/_OverlappedFuture_cancel_overlapped.py` & `rio_ui-0.6.6/rio/patches_for_3rd_party_stuff/_OverlappedFuture_cancel_overlapped.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/README.md` & `rio_ui-0.6.6/rio/snippets/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/__init__.py` & `rio_ui-0.6.6/rio/snippets/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/howtos/core-classes.md` & `rio_ui-0.6.6/rio/snippets/snippet-files/howtos/core-classes.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/howtos/debugging-setup.md` & `rio_ui-0.6.6/rio/snippets/snippet-files/howtos/debugging-setup.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/howtos/deployment.md` & `rio_ui-0.6.6/rio/snippets/snippet-files/howtos/deployment.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/howtos/howto-custom-events.md` & `rio_ui-0.6.6/rio/snippets/snippet-files/howtos/howto-custom-events.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/howtos/howto-get-value-from-child-component.md` & `rio_ui-0.6.6/rio/snippets/snippet-files/howtos/howto-get-value-from-child-component.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/howtos/howto-install.md` & `rio_ui-0.6.6/rio/snippets/snippet-files/howtos/howto-install.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/howtos/howto-pass-value-to-event.md` & `rio_ui-0.6.6/rio/snippets/snippet-files/howtos/howto-pass-value-to-event.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/howtos/persistent-settings.md` & `rio_ui-0.6.6/rio/snippets/snippet-files/howtos/persistent-settings.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/howtos/project-setup.md` & `rio_ui-0.6.6/rio/snippets/snippet-files/howtos/project-setup.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/howtos/run-project.md` & `rio_ui-0.6.6/rio/snippets/snippet-files/howtos/run-project.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/howtos/theming.md` & `rio_ui-0.6.6/rio/snippets/snippet-files/howtos/theming.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/other-examples/simple_counter_app.py` & `rio_ui-0.6.6/rio/snippets/snippet-files/other-examples/simple_counter_app.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/project-template-AI Chatbot/README.md` & `rio_ui-0.6.6/rio/snippets/snippet-files/project-template-AI Chatbot/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py` & `rio_ui-0.6.6/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/project-template-AI Chatbot/root_init.py` & `rio_ui-0.6.6/rio/snippets/snippet-files/project-template-AI Chatbot/root_init.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg` & `rio_ui-0.6.6/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py` & `rio_ui-0.6.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py` & `rio_ui-0.6.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py` & `rio_ui-0.6.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py` & `rio_ui-0.6.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py` & `rio_ui-0.6.6/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/README.md` & `rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/data_models.py` & `rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/data_models.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/thumbnail.svg` & `rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/assets/cryptos.csv` & `rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/assets/cryptos.csv`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/balance_card.py` & `rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/balance_card.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_card.py` & `rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_card.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_chart.py` & `rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_chart.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/dashboard_page.py` & `rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/dashboard_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg` & `rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Empty/pages/sample_page.py` & `rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Empty/pages/sample_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Simple CRUD/README.md` & `rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Simple CRUD/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py` & `rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg` & `rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py` & `rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py` & `rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py` & `rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg` & `rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py` & `rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py` & `rio_ui-0.6.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py` & `rio_ui-0.6.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py` & `rio_ui-0.6.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py` & `rio_ui-0.6.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py` & `rio_ui-0.6.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py` & `rio_ui-0.6.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py` & `rio_ui-0.6.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py` & `rio_ui-0.6.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/scripts/benchmark.py` & `rio_ui-0.6.6/scripts/benchmark.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/scripts/build_material_icon_set.py` & `rio_ui-0.6.6/scripts/build_material_icon_set.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/scripts/code_coverage.py` & `rio_ui-0.6.6/scripts/code_coverage.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/scripts/publish_new_release.py` & `rio_ui-0.6.6/scripts/publish_new_release.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         text=True,
     )
     if process.stdout.strip("\n") != "dev":
         revel.fatal("You must checkout the 'dev' branch")
 
     # Make sure there are no uncommitted changes
     process = subprocess.run(
-        ["git", "status", "--porcelain"],
+        ["git", "status", "--porcelain", "--untracked-files=no"],
         check=True,
         capture_output=True,
         text=True,
     )
     if process.stdout.strip():
         revel.fatal("There are uncommitted changes")
```

### Comparing `rio_ui-0.6.5/tests/test_attribute_bindings.py` & `rio_ui-0.6.6/tests/test_attribute_bindings.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/tests/test_custom_components.py` & `rio_ui-0.6.6/tests/test_custom_components.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/tests/test_docstring_code_blocks.py` & `rio_ui-0.6.6/tests/test_docstring_code_blocks.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/tests/test_documentation.py` & `rio_ui-0.6.6/tests/test_documentation.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/tests/test_events.py` & `rio_ui-0.6.6/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/tests/test_project_templates.py` & `rio_ui-0.6.6/tests/test_project_templates.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/tests/test_reconciliation.py` & `rio_ui-0.6.6/tests/test_reconciliation.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/tests/test_refresh.py` & `rio_ui-0.6.6/tests/test_refresh.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/tests/test_session.py` & `rio_ui-0.6.6/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/tests/test_user_settings.py` & `rio_ui-0.6.6/tests/test_user_settings.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/tests/test_zzz_guardrails.py` & `rio_ui-0.6.6/tests/test_zzz_guardrails.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/tests/utils.py` & `rio_ui-0.6.6/tests/utils.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/LICENSE.txt` & `rio_ui-0.6.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/README.md` & `rio_ui-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/pyproject.toml` & `rio_ui-0.6.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rio_ui-0.6.5/PKG-INFO` & `rio_ui-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rio-ui
-Version: 0.6.5
+Version: 0.6.6
 Summary: Build modern Websites and Apps just with Python
 Project-URL: homepage, https://rio.dev
 Project-URL: documentation, https://rio.dev/docs
 Author-email: Jakob Pinterits <jakob.pinterits@gmail.com>, Paul Pinterits <rawing7@gmail.com>
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

