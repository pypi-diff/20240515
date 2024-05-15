# Comparing `tmp/altmol-0.2.1.tar.gz` & `tmp/altmol-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altmol-0.2.1.tar", max compression
+gzip compressed data, was "altmol-0.2.2.tar", max compression
```

## Comparing `altmol-0.2.1.tar` & `altmol-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1068 2024-05-06 13:53:46.086366 altmol-0.2.1/LICENSE
--rw-r--r--   0        0        0     2620 2024-05-06 13:53:46.086366 altmol-0.2.1/README.md
--rw-r--r--   0        0        0       20 2024-05-06 13:53:46.086366 altmol-0.2.1/altmol/__init__.py
--rw-r--r--   0        0        0     3927 2024-05-06 13:53:46.086366 altmol-0.2.1/altmol/main.py
--rw-r--r--   0        0        0      450 2024-05-06 13:53:46.134366 altmol-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3196 1970-01-01 00:00:00.000000 altmol-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-15 14:59:17.866749 altmol-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2806 2024-05-15 14:59:17.866749 altmol-0.2.2/README.md
+-rw-r--r--   0        0        0       20 2024-05-15 14:59:17.866749 altmol-0.2.2/altmol/__init__.py
+-rw-r--r--   0        0        0     5099 2024-05-15 14:59:17.866749 altmol-0.2.2/altmol/chem.py
+-rw-r--r--   0        0        0     4038 2024-05-15 14:59:17.866749 altmol-0.2.2/altmol/plot.py
+-rw-r--r--   0        0        0      469 2024-05-15 14:59:17.926748 altmol-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3382 1970-01-01 00:00:00.000000 altmol-0.2.2/PKG-INFO
```

### Comparing `altmol-0.2.1/LICENSE` & `altmol-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `altmol-0.2.1/README.md` & `altmol-0.2.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,38 @@
+Metadata-Version: 2.1
+Name: altmol
+Version: 0.2.2
+Summary: 
+Author: Tagir Akhmetshin
+Author-email: tagirshin@gmail.com
+Requires-Python: >=3.9,<3.13
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: altair (>=5,<6)
+Requires-Dist: numpy (>=1.25)
+Requires-Dist: pandas (>=2.1)
+Requires-Dist: rdkit (>=2023.9.6,<2024.0.0)
+Description-Content-Type: text/markdown
+
 ![check](https://github.com/tagirshin/altmol/actions/workflows/check.yml/badge.svg?branch=main)
+[![PyPI version](https://badge.fury.io/py/altmol.svg)](https://badge.fury.io/py/altmol)
+[![PyPI Supported Python Versions](https://img.shields.io/pypi/pyversions/altmol.svg)](https://pypi.python.org/pypi/altmol/)
 
 # altmol
 
 `altmol` enhances Altair visualizations by integrating interactive 2D molecular structures, 
 leveraging RDKit for rendering.
 This package is inspired by the capabilities of [molplotly](https://github.com/wjm41/molplotly). 
 
+![Beautiful :)](https://raw.githubusercontent.com/tagirshin/altmol/main/images/esol_regression.gif)
+![Beautiful :)](https://raw.githubusercontent.com/tagirshin/altmol/main/images/aizynthfinder_templates.gif)
+
 ## Installation
 
 `altmol` can be easily installed using `pip` or `poetry`, accommodating both traditional and modern Python workflows.
 
 ### Using pip
 
 ```sh
@@ -35,55 +58,52 @@
 To get started with `altmol`, ensure you have Altair and RDKit installed in your environment. 
 Here's a simple example to illustrate how to create an interactive scatter plot with molecule visualizations:
 
 ```python
 import altair as alt
 import pandas as pd
 
-from altmol import encode_molecules, mol_plot
+from altmol.plot import chem_plot
+from altmol.chem import encode_molecules
 
 # URL of the ESOL dataset
 url_esol = 'https://raw.githubusercontent.com/deepchem/deepchem/master/datasets/delaney-processed.csv'
 
 # Load your dataset
 df = pd.read_csv(url_esol)
 
 # Prepare your data (ensure you have a 'smiles' column for molecular structures)
 df = encode_molecules(df, smiles_col_name='smiles', img_format='svg')
 
 x_col_name = "measured log solubility in mols per litre"
 y_col_name = "ESOL predicted log solubility in mols per litre"
 
 # Generate and display the interactive plot
-chart = mol_plot(
+chart = chem_plot(
     df,
     x_axis=alt.X(f"{x_col_name}:Q", title="True Log solubility"),
     y_axis=alt.Y(f"{y_col_name}:Q", title="Pred Log solubility"),
     tooltip=[x_col_name, y_col_name],
     selector=False,
     interactive=False,
     title="ESOL Regression"
 )
 chart.display()
 ```
 
-## Documentation
-
-For detailed documentation, including a full list of features, installation instructions, 
-and advanced usage examples, please visit altmol documentation.
 
 ## Contributing
 
 Contributions to `altmol` are welcome! Whether it's bug reports, feature requests, 
-or contributions to the code, we value your input. Please refer to our Contributing Guidelines 
-for more information on how you can contribute.
+or contributions to the code, we value your input.
 
 ## License
 
 `altmol` is released under the [MIT License](LICENSE). See the LICENSE file for more details.
 
 ## Acknowledgements
 
 `altmol` is built upon the powerful capabilities of [RDKit](https://www.rdkit.org/) 
 and [Altair](https://altair-viz.github.io/), and we are grateful to the developers and contributors of these projects.
 
  
+
```

### Comparing `altmol-0.2.1/altmol/main.py` & `altmol-0.2.2/altmol/plot.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,95 +1,102 @@
-import base64
-from io import BytesIO
-
 import altair as alt
 import pandas as pd
-from rdkit import Chem
-from rdkit.Chem import Descriptors, Draw, AllChem
-from rdkit.Chem.Draw import rdMolDraw2D
-from rdkit.Chem.rdChemReactions import ReactionFromSmarts
-
-
-def get_rdkit_object(smiles: str):
-    if ">" in smiles:
-        if ";" in smiles:
-            return AllChem.ReactionFromSmarts(smiles)
-        else:
-            try:
-                return ReactionFromSmarts(smiles, useSmiles=True)
-            except:
-                return AllChem.ReactionFromSmarts(smiles)
-    else:
-        return Chem.MolFromSmiles(smiles)
-
-
-def mol_to_png_data_url(mol, width=200, height=200):
-    if mol is None:
-        return None
-    if isinstance(mol, Chem.Mol):
-        img = Draw.MolToImage(mol, size=(width, height))
-    else:
-        img = Draw.ReactionToImage(mol, size=(width, height))
-    with BytesIO() as buffer:
-        img.save(buffer, format="PNG")
-        data = base64.b64encode(buffer.getvalue()).decode("utf8")
-    return f"data:image/png;base64,{data}"
-
-
-def mol_to_svg_data_url(mol, width=200, height=200):
-    d2d = rdMolDraw2D.MolDraw2DSVG(width, height)
-    opts = d2d.drawOptions()
-    opts.clearBackground = False
-    if isinstance(mol, Chem.Mol):
-        d2d.DrawMolecule(mol)
-    else:
-        d2d.DrawReaction(mol)
-    d2d.FinishDrawing()
-    img_str = d2d.GetDrawingText()
-    with BytesIO() as buffer:
-        buffer.write(str.encode(img_str))
-        data = base64.b64encode(buffer.getvalue()).decode("utf8")
-    return f"data:image/svg+xml;base64,{data}"
-
-
-def encode_molecules(
-    df: pd.DataFrame,
-    smiles_col_name="smiles",
-    img_format="svg",
-    img_width=200,
-    img_height=200,
-):
-    df["Mol"] = df[smiles_col_name].apply(lambda x: get_rdkit_object(x))
-    if isinstance(df["Mol"][0], Chem.Mol):
-        df["MolecularWeight"] = df["Mol"].apply(lambda x: Descriptors.MolWt(x))
-    if img_format == "png":
-        df["image"] = df["Mol"].apply(mol_to_png_data_url, args=(img_width, img_height))
-    elif img_format == "svg":
-        df["image"] = df["Mol"].apply(mol_to_svg_data_url)
-    return df.drop(columns=["Mol"])
-
-
-def mol_plot(
-    source,
-    x_axis,
-    y_axis,
+
+
+def chem_plot(
+    source: pd.DataFrame,
+    x_axis: alt.X,
+    y_axis: alt.Y,
     tooltip: list = None,
     color=None,
     selector=False,
     interactive=True,
     width=600,
     height=400,
     title="",
     chart_type="scatter",
     mark_size=20,
     mark_opacity=1.0,
     mark_fill=False,
     mark_shape="circle",
     mark_color="#1f77b4",
-):
+) -> alt.Chart:
+    """
+    Generate an Altair plot for molecular data.
+
+    Parameters
+    ----------
+    source : pd.DataFrame
+        Data source for the plot.
+    x_axis : alt.X
+        Altair X encoding.
+    y_axis : alt.Y
+        Altair Y encoding.
+    tooltip : list, optional
+        List of columns to show as tooltips, by default None.
+    color : alt.Color, optional
+        Color encoding, by default None.
+    selector : bool or alt.selection, optional
+        Selection for interactivity, by default False.
+    interactive : bool, optional
+        Enable interactivity, by default True.
+    width : int, optional
+        Width of the chart, by default 600.
+    height : int, optional
+        Height of the chart, by default 400.
+    title : str, optional
+        Title of the chart, by default "".
+    chart_type : str, optional
+        Type of chart ('scatter' or 'bar'), by default 'scatter'.
+    mark_size : int, optional
+        Size of the marks, by default 20.
+    mark_opacity : float, optional
+        Opacity of the marks, by default 1.0.
+    mark_fill : bool, optional
+        Fill the marks, by default False.
+    mark_shape : str, optional
+        Shape of the marks, by default "circle".
+    mark_color : str, optional
+        Color of the marks, by default "#1f77b4".
+
+    Returns
+    -------
+    alt.Chart
+        Altair chart object.
+
+    Notes
+    -----
+    This function generates a scatter or bar plot with molecular images as tooltips.
+
+    Examples
+    --------
+    >>> import pandas as pd
+    >>> import altair as alt
+    >>> from altmol.plot import chem_plot
+    >>> data = {
+    ...     'x': [1, 2, 3],
+    ...     'y': [4, 5, 6],
+    ...     'image': [
+    ...         'data:image/svg+xml;base64,...',
+    ...         'data:image/svg+xml;base64,...',
+    ...         'data:image/svg+xml;base64,...'
+    ...     ]
+    ... }
+    >>> df = pd.DataFrame(data)
+    >>> x_axis = alt.X('x:Q', title='X Axis')
+    >>> y_axis = alt.Y('y:Q', title='Y Axis')
+    >>> points = chem_plot(
+    ...     df,
+    ...     x_axis=x_axis,
+    ...     y_axis=y_axis,
+    ...     tooltip=['x', 'y'],
+    ...     title='Example Plot'
+    ... )
+    >>> points.show()
+    """
     if tooltip is None:
         tooltip = []
     if isinstance(selector, bool) and selector:
         selector = alt.selection_point()
 
     if selector and color:
         color = alt.condition(selector, color.legend(None), alt.value("lightgray"))
```

### Comparing `altmol-0.2.1/PKG-INFO` & `altmol-0.2.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,20 @@
-Metadata-Version: 2.1
-Name: altmol
-Version: 0.2.1
-Summary: 
-Author: Tagir Akhmetshin
-Author-email: tagirshin@gmail.com
-Requires-Python: >=3.9,<3.13
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: altair (>=5,<6)
-Requires-Dist: numpy (>=1.25)
-Requires-Dist: pandas (>=2.1)
-Requires-Dist: rdkit (>=2023.9.6,<2024.0.0)
-Description-Content-Type: text/markdown
-
 ![check](https://github.com/tagirshin/altmol/actions/workflows/check.yml/badge.svg?branch=main)
+[![PyPI version](https://badge.fury.io/py/altmol.svg)](https://badge.fury.io/py/altmol)
+[![PyPI Supported Python Versions](https://img.shields.io/pypi/pyversions/altmol.svg)](https://pypi.python.org/pypi/altmol/)
 
 # altmol
 
 `altmol` enhances Altair visualizations by integrating interactive 2D molecular structures, 
 leveraging RDKit for rendering.
 This package is inspired by the capabilities of [molplotly](https://github.com/wjm41/molplotly). 
 
+![Beautiful :)](https://raw.githubusercontent.com/tagirshin/altmol/main/images/esol_regression.gif)
+![Beautiful :)](https://raw.githubusercontent.com/tagirshin/altmol/main/images/aizynthfinder_templates.gif)
+
 ## Installation
 
 `altmol` can be easily installed using `pip` or `poetry`, accommodating both traditional and modern Python workflows.
 
 ### Using pip
 
 ```sh
@@ -53,56 +40,51 @@
 To get started with `altmol`, ensure you have Altair and RDKit installed in your environment. 
 Here's a simple example to illustrate how to create an interactive scatter plot with molecule visualizations:
 
 ```python
 import altair as alt
 import pandas as pd
 
-from altmol import encode_molecules, mol_plot
+from altmol.plot import chem_plot
+from altmol.chem import encode_molecules
 
 # URL of the ESOL dataset
 url_esol = 'https://raw.githubusercontent.com/deepchem/deepchem/master/datasets/delaney-processed.csv'
 
 # Load your dataset
 df = pd.read_csv(url_esol)
 
 # Prepare your data (ensure you have a 'smiles' column for molecular structures)
 df = encode_molecules(df, smiles_col_name='smiles', img_format='svg')
 
 x_col_name = "measured log solubility in mols per litre"
 y_col_name = "ESOL predicted log solubility in mols per litre"
 
 # Generate and display the interactive plot
-chart = mol_plot(
+chart = chem_plot(
     df,
     x_axis=alt.X(f"{x_col_name}:Q", title="True Log solubility"),
     y_axis=alt.Y(f"{y_col_name}:Q", title="Pred Log solubility"),
     tooltip=[x_col_name, y_col_name],
     selector=False,
     interactive=False,
     title="ESOL Regression"
 )
 chart.display()
 ```
 
-## Documentation
-
-For detailed documentation, including a full list of features, installation instructions, 
-and advanced usage examples, please visit altmol documentation.
 
 ## Contributing
 
 Contributions to `altmol` are welcome! Whether it's bug reports, feature requests, 
-or contributions to the code, we value your input. Please refer to our Contributing Guidelines 
-for more information on how you can contribute.
+or contributions to the code, we value your input.
 
 ## License
 
 `altmol` is released under the [MIT License](LICENSE). See the LICENSE file for more details.
 
 ## Acknowledgements
 
 `altmol` is built upon the powerful capabilities of [RDKit](https://www.rdkit.org/) 
 and [Altair](https://altair-viz.github.io/), and we are grateful to the developers and contributors of these projects.
 
  
-
```

