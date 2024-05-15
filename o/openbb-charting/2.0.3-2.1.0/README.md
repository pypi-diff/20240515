# Comparing `tmp/openbb_charting-2.0.3.tar.gz` & `tmp/openbb_charting-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_charting-2.0.3.tar", max compression
+gzip compressed data, was "openbb_charting-2.1.0.tar", max compression
```

## Comparing `openbb_charting-2.0.3.tar` & `openbb_charting-2.1.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     5148 2024-04-17 12:33:20.505645 openbb_charting-2.0.3/README.md
--rw-r--r--   0        0        0    19798 2024-04-19 16:25:42.940943 openbb_charting-2.0.3/openbb_charting/__init__.py
--rw-r--r--   0        0        0     1852 2024-04-17 12:33:20.505645 openbb_charting-2.0.3/openbb_charting/builder.py
--rw-r--r--   0        0        0    40926 2024-04-19 16:31:25.534563 openbb_charting-2.0.3/openbb_charting/charting_router.py
--rw-r--r--   0        0        0       28 2024-04-17 12:33:20.505645 openbb_charting-2.0.3/openbb_charting/core/__init__.py
--rw-r--r--   0        0        0   418780 2024-04-17 12:33:20.505645 openbb_charting-2.0.3/openbb_charting/core/assets/Terminal_icon.png
--rw-r--r--   0        0        0  3585992 2024-04-17 12:33:20.521645 openbb_charting-2.0.3/openbb_charting/core/assets/plotly-2.24.2.min.js
--rw-r--r--   0        0        0    17442 2024-04-17 12:33:20.521645 openbb_charting-2.0.3/openbb_charting/core/backend.py
--rw-r--r--   0        0        0     7362 2024-04-17 12:33:20.521645 openbb_charting-2.0.3/openbb_charting/core/chart_style.py
--rw-r--r--   0        0        0       42 2024-04-17 12:33:20.521645 openbb_charting-2.0.3/openbb_charting/core/config/__init__.py
--rw-r--r--   0        0        0     8068 2024-04-19 13:09:31.715183 openbb_charting-2.0.3/openbb_charting/core/config/openbb_styles.py
--rw-r--r--   0        0        0     2554 2024-04-17 12:33:20.521645 openbb_charting-2.0.3/openbb_charting/core/dummy_backend.py
--rw-r--r--   0        0        0    58532 2024-04-19 13:09:31.715183 openbb_charting-2.0.3/openbb_charting/core/openbb_figure.py
--rw-r--r--   0        0        0  5228579 2024-04-19 13:09:31.735184 openbb_charting-2.0.3/openbb_charting/core/plotly.html
--rw-r--r--   0        0        0       30 2024-04-17 12:33:20.541645 openbb_charting-2.0.3/openbb_charting/core/plotly_ta/__init__.py
--rw-r--r--   0        0        0     7185 2024-04-17 12:33:20.541645 openbb_charting-2.0.3/openbb_charting/core/plotly_ta/base.py
--rw-r--r--   0        0        0    12381 2024-04-19 13:09:31.735184 openbb_charting-2.0.3/openbb_charting/core/plotly_ta/data_classes.py
--rw-r--r--   0        0        0       25 2024-04-19 13:09:31.735184 openbb_charting-2.0.3/openbb_charting/core/plotly_ta/plugins/__init__.py
--rw-r--r--   0        0        0     8555 2024-04-19 13:09:31.735184 openbb_charting-2.0.3/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py
--rw-r--r--   0        0        0    19572 2024-04-19 13:09:31.735184 openbb_charting-2.0.3/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py
--rw-r--r--   0        0        0     3300 2024-04-19 13:09:31.735184 openbb_charting-2.0.3/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py
--rw-r--r--   0        0        0     5697 2024-04-19 13:09:31.735184 openbb_charting-2.0.3/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py
--rw-r--r--   0        0        0     6877 2024-04-19 13:09:31.735184 openbb_charting-2.0.3/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py
--rw-r--r--   0        0        0     3547 2024-04-19 13:09:31.735184 openbb_charting-2.0.3/openbb_charting/core/plotly_ta/plugins/volume_plugin.py
--rw-r--r--   0        0        0    25006 2024-04-19 13:10:31.744034 openbb_charting-2.0.3/openbb_charting/core/plotly_ta/ta_class.py
--rw-r--r--   0        0        0     1437 2024-04-17 12:33:20.541645 openbb_charting-2.0.3/openbb_charting/core/plotly_ta/ta_helpers.py
--rw-r--r--   0        0        0   717892 2024-04-17 12:33:20.545645 openbb_charting-2.0.3/openbb_charting/core/table.html
--rw-r--r--   0        0        0     2246 2024-04-17 12:33:20.545645 openbb_charting-2.0.3/openbb_charting/core/to_chart.py
--rw-r--r--   0        0        0    26843 2024-04-19 16:31:25.534563 openbb_charting-2.0.3/openbb_charting/query_params.py
--rw-r--r--   0        0        0       32 2024-04-19 13:09:31.735184 openbb_charting-2.0.3/openbb_charting/styles/__init__.py
--rw-r--r--   0        0        0      603 2024-04-19 13:09:31.735184 openbb_charting-2.0.3/openbb_charting/styles/colors.py
--rw-r--r--   0        0        0     3462 2024-04-19 16:31:25.534563 openbb_charting-2.0.3/openbb_charting/styles/default/dark.pltstyle.json
--rw-r--r--   0        0        0     3491 2024-04-19 16:31:25.534563 openbb_charting-2.0.3/openbb_charting/styles/default/light.pltstyle.json
--rw-r--r--   0        0        0     2505 2024-04-17 12:33:20.545645 openbb_charting-2.0.3/openbb_charting/styles/default/tables.pltstyle.json
--rw-r--r--   0        0        0       29 2024-04-17 12:33:20.545645 openbb_charting-2.0.3/openbb_charting/utils/__init__.py
--rw-r--r--   0        0        0    20295 2024-04-19 13:10:31.744034 openbb_charting-2.0.3/openbb_charting/utils/generic_charts.py
--rw-r--r--   0        0        0     2493 2024-04-19 13:09:31.735184 openbb_charting-2.0.3/openbb_charting/utils/helpers.py
--rw-r--r--   0        0        0    16657 2024-04-19 16:31:25.534563 openbb_charting-2.0.3/openbb_charting/utils/relative_rotation.py
--rw-r--r--   0        0        0      661 2024-04-19 16:43:24.571555 openbb_charting-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     5990 1970-01-01 00:00:00.000000 openbb_charting-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0     5148 2024-04-08 12:02:16.536826 openbb_charting-2.1.0/README.md
+-rw-r--r--   0        0        0    21664 2024-05-10 19:27:56.005288 openbb_charting-2.1.0/openbb_charting/__init__.py
+-rw-r--r--   0        0        0     1852 2024-04-08 12:02:16.537191 openbb_charting-2.1.0/openbb_charting/builder.py
+-rw-r--r--   0        0        0    40926 2024-04-23 10:22:39.613433 openbb_charting-2.1.0/openbb_charting/charting_router.py
+-rw-r--r--   0        0        0       28 2024-04-23 10:22:39.613545 openbb_charting-2.1.0/openbb_charting/core/__init__.py
+-rw-r--r--   0        0        0   418780 2024-04-08 12:02:16.538054 openbb_charting-2.1.0/openbb_charting/core/assets/Terminal_icon.png
+-rw-r--r--   0        0        0  3585992 2024-04-08 12:02:16.549064 openbb_charting-2.1.0/openbb_charting/core/assets/plotly-2.24.2.min.js
+-rw-r--r--   0        0        0    17655 2024-05-14 15:30:05.607181 openbb_charting-2.1.0/openbb_charting/core/backend.py
+-rw-r--r--   0        0        0     7362 2024-04-08 12:02:16.549412 openbb_charting-2.1.0/openbb_charting/core/chart_style.py
+-rw-r--r--   0        0        0       42 2024-04-23 10:22:39.613822 openbb_charting-2.1.0/openbb_charting/core/config/__init__.py
+-rw-r--r--   0        0        0     8068 2024-04-23 10:22:39.613958 openbb_charting-2.1.0/openbb_charting/core/config/openbb_styles.py
+-rw-r--r--   0        0        0     2554 2024-04-23 10:22:39.614087 openbb_charting-2.1.0/openbb_charting/core/dummy_backend.py
+-rw-r--r--   0        0        0    58532 2024-04-23 10:22:39.614381 openbb_charting-2.1.0/openbb_charting/core/openbb_figure.py
+-rw-r--r--   0        0        0  5228579 2024-04-23 10:22:39.633120 openbb_charting-2.1.0/openbb_charting/core/plotly.html
+-rw-r--r--   0        0        0       30 2024-04-23 10:22:39.633423 openbb_charting-2.1.0/openbb_charting/core/plotly_ta/__init__.py
+-rw-r--r--   0        0        0     7185 2024-04-23 10:22:39.633576 openbb_charting-2.1.0/openbb_charting/core/plotly_ta/base.py
+-rw-r--r--   0        0        0    12381 2024-04-23 10:22:39.634613 openbb_charting-2.1.0/openbb_charting/core/plotly_ta/data_classes.py
+-rw-r--r--   0        0        0       25 2024-04-23 10:22:39.634692 openbb_charting-2.1.0/openbb_charting/core/plotly_ta/plugins/__init__.py
+-rw-r--r--   0        0        0     8555 2024-04-23 10:22:39.634821 openbb_charting-2.1.0/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py
+-rw-r--r--   0        0        0    19572 2024-04-23 10:22:39.634962 openbb_charting-2.1.0/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py
+-rw-r--r--   0        0        0     3300 2024-04-23 10:22:39.635088 openbb_charting-2.1.0/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py
+-rw-r--r--   0        0        0     5697 2024-04-23 10:22:39.635193 openbb_charting-2.1.0/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py
+-rw-r--r--   0        0        0     6877 2024-04-23 10:22:39.635294 openbb_charting-2.1.0/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py
+-rw-r--r--   0        0        0     3547 2024-04-23 10:22:39.635394 openbb_charting-2.1.0/openbb_charting/core/plotly_ta/plugins/volume_plugin.py
+-rw-r--r--   0        0        0    25006 2024-04-23 10:22:39.635564 openbb_charting-2.1.0/openbb_charting/core/plotly_ta/ta_class.py
+-rw-r--r--   0        0        0     1437 2024-04-23 10:22:39.635680 openbb_charting-2.1.0/openbb_charting/core/plotly_ta/ta_helpers.py
+-rw-r--r--   0        0        0   717892 2024-04-23 10:22:39.639210 openbb_charting-2.1.0/openbb_charting/core/table.html
+-rw-r--r--   0        0        0     2246 2024-04-23 10:22:39.639394 openbb_charting-2.1.0/openbb_charting/core/to_chart.py
+-rw-r--r--   0        0        0    26843 2024-04-23 10:22:39.639558 openbb_charting-2.1.0/openbb_charting/query_params.py
+-rw-r--r--   0        0        0       32 2024-04-23 10:22:39.639639 openbb_charting-2.1.0/openbb_charting/styles/__init__.py
+-rw-r--r--   0        0        0      603 2024-04-23 10:22:39.639695 openbb_charting-2.1.0/openbb_charting/styles/colors.py
+-rw-r--r--   0        0        0     3462 2024-04-23 10:22:39.639822 openbb_charting-2.1.0/openbb_charting/styles/default/dark.pltstyle.json
+-rw-r--r--   0        0        0     3491 2024-04-23 10:22:39.639908 openbb_charting-2.1.0/openbb_charting/styles/default/light.pltstyle.json
+-rw-r--r--   0        0        0     2505 2024-04-08 12:02:16.569604 openbb_charting-2.1.0/openbb_charting/styles/default/tables.pltstyle.json
+-rw-r--r--   0        0        0       29 2024-04-08 12:02:16.569664 openbb_charting-2.1.0/openbb_charting/utils/__init__.py
+-rw-r--r--   0        0        0    20295 2024-04-23 10:22:39.640016 openbb_charting-2.1.0/openbb_charting/utils/generic_charts.py
+-rw-r--r--   0        0        0     2493 2024-04-23 10:22:39.640140 openbb_charting-2.1.0/openbb_charting/utils/helpers.py
+-rw-r--r--   0        0        0    16657 2024-04-23 10:22:39.640241 openbb_charting-2.1.0/openbb_charting/utils/relative_rotation.py
+-rw-r--r--   0        0        0      687 2024-05-15 16:07:43.939624 openbb_charting-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6089 1970-01-01 00:00:00.000000 openbb_charting-2.1.0/PKG-INFO
```

### Comparing `openbb_charting-2.0.3/README.md` & `openbb_charting-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.3/openbb_charting/__init__.py` & `openbb_charting-2.1.0/openbb_charting/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,21 +31,20 @@
 from openbb_charting.utils.generic_charts import bar_chart, line_chart
 from openbb_charting.utils.helpers import get_charting_functions
 
 warnings.filterwarnings(
     "ignore", category=UserWarning, module="openbb_core.app.model.extension", lineno=47
 )
 
-ext = Extension(name="charting")
+ext = Extension(name="charting", description="Create custom charts from OBBject data.")
 
 
 @ext.obbject_accessor
 class Charting:
-    """
-    Charting extension.
+    """Charting extension.
 
     Methods
     -------
     show
         Display chart and save it to the OBBject.
     to_chart
         Redraw the chart and save it to the OBBject, with an optional entry point for Data.
@@ -57,14 +56,16 @@
         Return the list of the available technical indicators to use with the `to_chart` method and OHLC+V data.
     table
         Display an interactive table.
     create_line_chart
         Create a line chart from external data.
     create_bar_chart
         Create a bar chart, on a single x-axis with one or more values for the y-axis, from external data.
+    toggle_chart_style
+        Toggle the chart style, of an existing chart, between light and dark mode.
     """
 
     def __init__(self, obbject):
         """Initialize Charting extension."""
         # pylint: disable=import-outside-toplevel
         from openbb_core.app.model.charts.charting_settings import ChartingSettings
 
@@ -73,45 +74,43 @@
             user_settings=self._obbject._user_settings,  # type: ignore
             system_settings=self._obbject._system_settings,  # type: ignore
         )
         self._backend: Backend = self._handle_backend()
 
     @classmethod
     def indicators(cls):
-        """
-        Return an instance of the IndicatorsParams class, containing all available indicators and their parameters.
+        """Return an instance of the IndicatorsParams class, containing all available indicators and their parameters.
+
         Without assigning to a variable, it will print the the information to the console.
         """
         return IndicatorsParams()
 
     @classmethod
     def functions(cls):
         """Return a list of the available functions."""
         return get_charting_functions()
 
     def _handle_backend(self) -> Backend:
         """Create and start the backend."""
-
         create_backend(self._charting_settings)
         backend = get_backend()
         backend.start(debug=self._charting_settings.debug_mode)
         return backend
 
     @staticmethod
     def _get_chart_function(route: str) -> Callable:
         """Given a route, it returns the chart function. The module must contain the given route."""
-
         if route is None:
             raise ValueError("OBBject was initialized with no function route.")
         adjusted_route = route.replace("/", "_")[1:]
         return getattr(charting_router, adjusted_route)
 
     def get_params(self) -> ChartParams:
-        """
-        Return the ChartQueryParams class for the function the OBBject was created from.
+        """Return the ChartQueryParams class for the function the OBBject was created from.
+
         Without assigning to a variable, it will print the docstring to the console.
         """
         if self._obbject._route is None:  # pylint: disable=protected-access
             raise ValueError("OBBject was initialized with no function route.")
         charting_function = (
             self._obbject._route  # pylint: disable=protected-access
         ).replace("/", "_")[1:]
@@ -122,15 +121,15 @@
         )
 
     def _prepare_data_as_df(
         self, data: Optional[Union[pd.DataFrame, pd.Series]]
     ) -> Tuple[pd.DataFrame, bool]:
         """Convert supplied data to a DataFrame."""
         has_data = (
-            isinstance(data, (Data, pd.DataFrame, pd.Series)) and not data.empty
+            isinstance(data, (Data, pd.DataFrame, pd.Series)) and not data.empty  # type: ignore
         ) or (bool(data))
         index = (
             data.index.name
             if has_data and isinstance(data, (pd.DataFrame, pd.Series))
             else None
         )
         data_as_df: pd.DataFrame = (
@@ -230,14 +229,15 @@
             layout_kwargs=layout_kwargs,
             scatter_kwargs=scatter_kwargs,
             normalize=normalize,
             returns=returns,
             same_axis=same_axis,
             **kwargs,
         )
+        fig = self._set_chart_style(fig)
         if render:
             return fig.show(**kwargs)
 
         return fig
 
     def create_bar_chart(
         self,
@@ -294,39 +294,37 @@
         layout_kwargs : Dict[str, Any], optional
             Additional keyword arguments to apply with figure.update_layout(), by default None.
         Returns
         -------
         OpenBBFigure
             The OpenBBFigure object.
         """
-
         fig = bar_chart(
             data=data,
             x=x,
             y=y,
             barmode=barmode,
             xtype=xtype,
             title=title,
             xtitle=xtitle,
             ytitle=ytitle,
             orientation=orientation,
             colors=colors,
             bar_kwargs=bar_kwargs,
             layout_kwargs=layout_kwargs,
         )
-
+        fig = self._set_chart_style(fig)
         if render:
             return fig.show(**kwargs)
 
         return fig
 
     # pylint: disable=inconsistent-return-statements
     def show(self, render: bool = True, **kwargs):
         """Display chart and save it to the OBBject."""
-
         try:
             charting_function = self._get_chart_function(
                 self._obbject._route  # pylint: disable=protected-access
             )
             kwargs["obbject_item"] = self._obbject.results
             kwargs["charting_settings"] = self._charting_settings
             if (
@@ -341,22 +339,25 @@
             )  # pylint: disable=protected-access
             kwargs["extra"] = self._obbject.extra  # pylint: disable=protected-access
 
             if "kwargs" in kwargs:
                 _kwargs = kwargs.pop("kwargs")
                 kwargs.update(_kwargs.get("chart_params", {}))
             fig, content = charting_function(**kwargs)
+            fig = self._set_chart_style(fig)
+            content = fig.show(external=True, **kwargs).to_plotly_json()
             self._obbject.chart = Chart(
                 fig=fig, content=content, format=charting_router.CHART_FORMAT
             )
             if render:
                 fig.show(**kwargs)
-        except Exception:
+        except Exception:  # pylint: disable=W0718
             try:
                 fig = self.create_line_chart(data=self._obbject.results, render=False, **kwargs)  # type: ignore
+                fig = self._set_chart_style(fig)
                 content = fig.show(external=True, **kwargs).to_plotly_json()  # type: ignore
                 self._obbject.chart = Chart(
                     fig=fig, content=content, format=charting_router.CHART_FORMAT
                 )
                 if render:
                     return fig.show(**kwargs)  # type: ignore
             except Exception as e:
@@ -385,19 +386,18 @@
         symbol: str = "",
         candles: bool = True,
         volume: bool = True,
         volume_ticks_x: int = 7,
         render: bool = True,
         **kwargs,
     ):
-        """
-        Create an OpenBBFigure with user customizations (if any) and save it to the OBBject.
+        """Create an OpenBBFigure with user customizations (if any) and save it to the OBBject.
+
         This function is used to populate, or re-populate, the OBBject with a chart using the data within
         the OBBject or external data supplied via the `data` parameter.
-
         This function modifies the original OBBject by overwriting the existing chart.
 
         Parameters
         ----------
         data : Union[Data, pd.DataFrame, pd.Series]
             Data to be plotted.
         indicators : Dict[str, Dict[str, Any]], optional
@@ -463,35 +463,63 @@
             _kwargs = kwargs.pop("kwargs")
             kwargs.update(_kwargs.get("chart_params", {}))
         try:
             if has_data:
                 self.show(data=data_as_df, render=render, **kwargs)
             else:
                 self.show(**kwargs, render=render)
-        except Exception:
+        except Exception:  # pylint: disable=W0718
             try:
                 fig = self.create_line_chart(data=data_as_df, render=False, **kwargs)
+                fig = self._set_chart_style(fig)
                 content = fig.show(external=True, **kwargs).to_plotly_json()  # type: ignore
                 self._obbject.chart = Chart(
                     fig=fig, content=content, format=charting_router.CHART_FORMAT
                 )
                 if render:
                     return fig.show(**kwargs)  # type: ignore
-            except Exception as e:
+            except Exception as e:  # pylint: disable=W0718
                 raise RuntimeError(
                     "Failed to automatically create a generic chart with the data provided."
                 ) from e
 
+    def _set_chart_style(self, figure: Figure):
+        """Set the user preference for light or dark mode."""
+        style = self._charting_settings.chart_style  # pylint: disable=protected-access
+        font_color = "black" if style == "light" else "white"
+        paper_bgcolor = "white" if style == "light" else "black"
+        figure = figure.update_layout(
+            dict(  # pylint: disable=R1735
+                font_color=font_color, paper_bgcolor=paper_bgcolor
+            )
+        )
+        return figure
+
+    def toggle_chart_style(self):  # pylint: disable=protected-access
+        """Toggle the chart style between light and dark mode."""
+        if not hasattr(self._obbject.chart, "fig"):
+            raise ValueError(
+                "Error: No chart has been created. Please create a chart first."
+            )
+        current = self._charting_settings.chart_style
+        new = "light" if current == "dark" else "dark"
+        self._charting_settings.chart_style = new
+        figure = self._obbject.chart.fig  # type: ignore[union-attr]
+        updated_figure = self._set_chart_style(figure)
+        self._obbject.chart.fig = updated_figure  # type: ignore[union-attr]
+        self._obbject.chart.content = updated_figure.show(  # type: ignore[union-attr]
+            external=True
+        ).to_plotly_json()
+
     def table(
         self,
         data: Optional[Union[pd.DataFrame, pd.Series]] = None,
         title: str = "",
     ):
-        """
-        Display an interactive table.
+        """Display an interactive table.
 
         Parameters
         ----------
         data : Optional[Union[pd.DataFrame, pd.Series]], optional
             Data to be plotted, by default None.
             If no data is provided the OBBject results will be used.
         title : str, optional
@@ -506,15 +534,15 @@
             try:
                 self._backend.send_table(
                     df_table=data_as_df,
                     title=title
                     or self._obbject._route,  # pylint: disable=protected-access
                     theme=self._charting_settings.table_style,
                 )
-            except Exception as e:
+            except Exception as e:  # pylint: disable=W0718
                 warn(f"Failed to show figure with backend. {e}")
 
         else:
             from plotly import (  # pylint:disable=import-outside-toplevel
                 optional_imports,
             )
```

### Comparing `openbb_charting-2.0.3/openbb_charting/builder.py` & `openbb_charting-2.1.0/openbb_charting/builder.py`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.3/openbb_charting/charting_router.py` & `openbb_charting-2.1.0/openbb_charting/charting_router.py`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.3/openbb_charting/core/assets/Terminal_icon.png` & `openbb_charting-2.1.0/openbb_charting/core/assets/Terminal_icon.png`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.3/openbb_charting/core/assets/plotly-2.24.2.min.js` & `openbb_charting-2.1.0/openbb_charting/core/assets/plotly-2.24.2.min.js`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.3/openbb_charting/core/backend.py` & `openbb_charting-2.1.0/openbb_charting/core/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,29 +194,34 @@
         command_location : str, optional
             Location of the command, by default "".
             We can use the route here to display it on the chart title.
         """
         self.check_backend()
         # pylint: disable=C0415
 
+        paper_bg = (
+            "rgba(0,0,0,0)"
+            if self.charting_settings.chart_style == "dark"
+            else "rgba(255,255,255,0)"
+        )
+
         title = "Interactive Chart"
 
         fig.layout.title.text = re.sub(
             r"<[^>]*>", "", fig.layout.title.text if fig.layout.title.text else title
         )
 
         fig.layout.height += 69
 
         if export_image and isinstance(export_image, str):
             export_image = Path(export_image).resolve()
 
         json_data = json.loads(fig.to_json())
-
         json_data.update(self.get_json_update(command_location))
-
+        json_data["layout"]["paper_bgcolor"] = paper_bg
         outgoing = dict(
             html=self.get_plotly_html(),
             json_data=json_data,
             export_image=export_image,
             **self.get_kwargs(command_location),
         )
         self.send_outgoing(outgoing)
```

### Comparing `openbb_charting-2.0.3/openbb_charting/core/chart_style.py` & `openbb_charting-2.1.0/openbb_charting/core/chart_style.py`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.3/openbb_charting/core/config/openbb_styles.py` & `openbb_charting-2.1.0/openbb_charting/core/config/openbb_styles.py`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.3/openbb_charting/core/dummy_backend.py` & `openbb_charting-2.1.0/openbb_charting/core/dummy_backend.py`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.3/openbb_charting/core/openbb_figure.py` & `openbb_charting-2.1.0/openbb_charting/core/openbb_figure.py`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.3/openbb_charting/core/plotly.html` & `openbb_charting-2.1.0/openbb_charting/core/plotly.html`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.3/openbb_charting/core/plotly_ta/base.py` & `openbb_charting-2.1.0/openbb_charting/core/plotly_ta/base.py`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.3/openbb_charting/core/plotly_ta/data_classes.py` & `openbb_charting-2.1.0/openbb_charting/core/plotly_ta/data_classes.py`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.3/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py` & `openbb_charting-2.1.0/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.3/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py` & `openbb_charting-2.1.0/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.3/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py` & `openbb_charting-2.1.0/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.3/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py` & `openbb_charting-2.1.0/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.3/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py` & `openbb_charting-2.1.0/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.3/openbb_charting/core/plotly_ta/plugins/volume_plugin.py` & `openbb_charting-2.1.0/openbb_charting/core/plotly_ta/plugins/volume_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.3/openbb_charting/core/plotly_ta/ta_class.py` & `openbb_charting-2.1.0/openbb_charting/core/plotly_ta/ta_class.py`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.3/openbb_charting/core/plotly_ta/ta_helpers.py` & `openbb_charting-2.1.0/openbb_charting/core/plotly_ta/ta_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.3/openbb_charting/core/table.html` & `openbb_charting-2.1.0/openbb_charting/core/table.html`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.3/openbb_charting/core/to_chart.py` & `openbb_charting-2.1.0/openbb_charting/core/to_chart.py`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.3/openbb_charting/query_params.py` & `openbb_charting-2.1.0/openbb_charting/query_params.py`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.3/openbb_charting/styles/colors.py` & `openbb_charting-2.1.0/openbb_charting/styles/colors.py`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.3/openbb_charting/styles/default/dark.pltstyle.json` & `openbb_charting-2.1.0/openbb_charting/styles/default/dark.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.3/openbb_charting/styles/default/light.pltstyle.json` & `openbb_charting-2.1.0/openbb_charting/styles/default/light.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.3/openbb_charting/styles/default/tables.pltstyle.json` & `openbb_charting-2.1.0/openbb_charting/styles/default/tables.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.3/openbb_charting/utils/generic_charts.py` & `openbb_charting-2.1.0/openbb_charting/utils/generic_charts.py`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.3/openbb_charting/utils/helpers.py` & `openbb_charting-2.1.0/openbb_charting/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.3/openbb_charting/utils/relative_rotation.py` & `openbb_charting-2.1.0/openbb_charting/utils/relative_rotation.py`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.3/pyproject.toml` & `openbb_charting-2.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [tool.poetry]
 name = "openbb-charting"
-version = "2.0.3"
+version = "2.1.0"
 description = "Charting extension for OpenBB"
 authors = ["OpenBB Team <hello@openbb.co>"]
+license = "AGPL-3.0-only"
 readme = "README.md"
 packages = [{ include = "openbb_charting" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"  # scipy forces python <4.0 explicitly
 scipy = "^1.10.0"
 plotly = "^5.17.0"
 statsmodels = "^0.14.0"
 reportlab = "^4.0.4"
 pywry = "^0.6.1"
 svglib = "^1.5.1"
 nbformat = "^5.9.2"
 pandas-ta = "^0.3.14b"
-openbb-core = "^1.1.6"
+openbb-core = "^1.2.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."openbb_obbject_extension"]
 openbb_charting = "openbb_charting:ext"
```

### Comparing `openbb_charting-2.0.3/PKG-INFO` & `openbb_charting-2.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: openbb-charting
-Version: 2.0.3
+Version: 2.1.0
 Summary: Charting extension for OpenBB
+License: AGPL-3.0-only
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<3.12
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: nbformat (>=5.9.2,<6.0.0)
-Requires-Dist: openbb-core (>=1.1.6,<2.0.0)
+Requires-Dist: openbb-core (>=1.2.1,<2.0.0)
 Requires-Dist: pandas-ta (>=0.3.14b,<0.4.0)
 Requires-Dist: plotly (>=5.17.0,<6.0.0)
 Requires-Dist: pywry (>=0.6.1,<0.7.0)
 Requires-Dist: reportlab (>=4.0.4,<5.0.0)
 Requires-Dist: scipy (>=1.10.0,<2.0.0)
 Requires-Dist: statsmodels (>=0.14.0,<0.15.0)
 Requires-Dist: svglib (>=1.5.1,<2.0.0)
```

