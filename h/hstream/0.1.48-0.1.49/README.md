# Comparing `tmp/hstream-0.1.48.tar.gz` & `tmp/hstream-0.1.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hstream-0.1.48.tar", max compression
+gzip compressed data, was "hstream-0.1.49.tar", max compression
```

## Comparing `hstream-0.1.48.tar` & `hstream-0.1.49.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     4232 2024-05-12 11:26:27.408478 hstream-0.1.48/README.md
--rw-r--r--   0        0        0       53 2024-05-09 13:05:58.281504 hstream-0.1.48/hstream/__init__.py
--rw-r--r--   0        0        0       66 2024-05-12 11:26:20.930757 hstream-0.1.48/hstream/__main__.py
--rw-r--r--   0        0        0     2109 2024-05-12 11:26:20.931172 hstream-0.1.48/hstream/cli.py
--rw-r--r--   0        0        0    16890 2024-05-13 12:17:18.055215 hstream-0.1.48/hstream/components/components.py
--rw-r--r--   0        0        0     4625 2024-05-12 11:26:20.932358 hstream-0.1.48/hstream/components/styling_components.py
--rw-r--r--   0        0        0        0 2024-05-12 11:26:20.932458 hstream-0.1.48/hstream/django_server/hs/__init__.py
--rw-r--r--   0        0        0      136 2024-05-12 11:26:20.933121 hstream-0.1.48/hstream/django_server/hs/apps.py
--rw-r--r--   0        0        0      749 2024-05-12 11:26:20.933435 hstream-0.1.48/hstream/django_server/hs/session_utils.py
--rw-r--r--   0        0        0      424 2024-05-12 11:26:20.933722 hstream-0.1.48/hstream/django_server/hs/urls.py
--rw-r--r--   0        0        0     7579 2024-05-13 14:07:38.675320 hstream-0.1.48/hstream/django_server/hs/views.py
--rwxr-xr-x   0        0        0      661 2024-05-12 11:26:20.934370 hstream-0.1.48/hstream/django_server/manage.py
--rw-r--r--   0        0        0        0 2024-05-12 11:26:20.934433 hstream-0.1.48/hstream/django_server/root/__init__.py
--rw-r--r--   0        0        0      381 2024-05-12 11:26:20.934747 hstream-0.1.48/hstream/django_server/root/asgi.py
--rw-r--r--   0        0        0     3218 2024-05-13 12:18:29.663642 hstream-0.1.48/hstream/django_server/root/settings.py
--rw-r--r--   0        0        0      802 2024-05-12 11:26:20.935930 hstream-0.1.48/hstream/django_server/root/urls.py
--rw-r--r--   0        0        0      381 2024-05-12 11:26:20.936295 hstream-0.1.48/hstream/django_server/root/wsgi.py
--rw-r--r--   0        0        0      683 2024-05-12 11:26:20.936728 hstream-0.1.48/hstream/hs.py
--rw-r--r--   0        0        0      569 2024-05-13 12:18:29.651176 hstream-0.1.48/hstream/run.py
--rw-r--r--   0        0        0      394 2024-05-09 13:05:58.283832 hstream-0.1.48/hstream/template.py
--rw-r--r--   0        0        0      162 2024-05-12 11:26:20.937259 hstream-0.1.48/hstream/templates/error_html.html
--rw-r--r--   0        0        0     2446 2024-05-12 11:26:20.937650 hstream-0.1.48/hstream/templates/format_html.html
--rw-r--r--   0        0        0     2466 2024-05-12 11:26:20.937995 hstream-0.1.48/hstream/utils.py
--rw-r--r--   0        0        0      646 2024-05-13 14:07:46.288349 hstream-0.1.48/pyproject.toml
--rw-r--r--   0        0        0     4814 1970-01-01 00:00:00.000000 hstream-0.1.48/PKG-INFO
+-rw-r--r--   0        0        0     4232 2024-05-15 11:59:56.595400 hstream-0.1.49/README.md
+-rw-r--r--   0        0        0       53 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/__init__.py
+-rw-r--r--   0        0        0       66 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/__main__.py
+-rw-r--r--   0        0        0     3522 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/cli.py
+-rw-r--r--   0        0        0    19076 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/components/components.py
+-rw-r--r--   0        0        0     4625 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/components/styling_components.py
+-rw-r--r--   0        0        0        0 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/django_server/hs/__init__.py
+-rw-r--r--   0        0        0      136 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/django_server/hs/apps.py
+-rw-r--r--   0        0        0      749 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/django_server/hs/session_utils.py
+-rw-r--r--   0        0        0      424 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/django_server/hs/urls.py
+-rw-r--r--   0        0        0     7990 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/django_server/hs/views.py
+-rwxr-xr-x   0        0        0      661 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/django_server/manage.py
+-rw-r--r--   0        0        0        0 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/django_server/root/__init__.py
+-rw-r--r--   0        0        0      381 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/django_server/root/asgi.py
+-rw-r--r--   0        0        0     3218 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/django_server/root/settings.py
+-rw-r--r--   0        0        0      802 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/django_server/root/urls.py
+-rw-r--r--   0        0        0      381 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/django_server/root/wsgi.py
+-rw-r--r--   0        0        0      683 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/hs.py
+-rw-r--r--   0        0        0      638 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/run.py
+-rw-r--r--   0        0        0      394 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/template.py
+-rw-r--r--   0        0        0      162 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/templates/error_html.html
+-rw-r--r--   0        0        0     2446 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/templates/format_html.html
+-rw-r--r--   0        0        0     2466 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/utils.py
+-rw-r--r--   0        0        0      646 2024-05-15 11:59:56.607400 hstream-0.1.49/pyproject.toml
+-rw-r--r--   0        0        0     4814 1970-01-01 00:00:00.000000 hstream-0.1.49/PKG-INFO
```

### Comparing `hstream-0.1.48/README.md` & `hstream-0.1.49/README.md`

 * *Files identical despite different names*

### Comparing `hstream-0.1.48/hstream/cli.py` & `hstream-0.1.49/hstream/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -73,14 +73,63 @@
         f.write(content)
 
     click.echo("Initialized example.py")
     click.echo("Now run:")
     click.echo(click.style("     hstream run example.py", fg="green"))
 
 
+@click.command()
+@click.argument("file", default=False)
+def deploy(file=False):
+    if not file:
+        file = click.prompt(
+            "Enter the file containing the hstream app you want to deploy ",
+            default="./app",
+        )
+    if Path("Dockerfile").exists():
+        click.echo(
+            click.style("Dockerfile already exist - can't over write", fg="red"),
+            err=True,
+        )
+        return
+    else:
+        with open("Dockerfile", "w") as f:
+            f.write(DOCKERFILE.format(filename=file))
+
+    click.echo("Dockerfile created successfully")
+    click.echo("""We recommend deploying on Railway using the below""")
+    click.echo(
+        """If you don't have an account create one (free):
+                https://railway.app?referralCode=1OLHEp"""
+    )
+    click.echo(
+        click.style(
+            f"""
+                {"brew install railway" if shutil.which("brew") else "Follow: https://docs.railway.app/guides/cli for install railway cli"}
+                railway login
+                railway link
+                railway up""",
+            fg="green",
+        )
+    )
+
+
 cli.add_command(eject)
+cli.add_command(deploy)
 cli.add_command(run)
 cli.add_command(init)
 
 
 if __name__ == "__main__":
     cli()
+
+
+DOCKERFILE = """
+FROM python:3.11-slim
+WORKDIR /code
+RUN pip install --upgrade pip
+RUN pip install hstream
+# RUN pip install -r requirements.txt # uncomment if you have a requirements.txt
+# COPY requirements.txt /code/
+COPY . /code/
+CMD hstream run {filename}
+"""
```

### Comparing `hstream-0.1.48/hstream/components/components.py` & `hstream-0.1.49/hstream/components/components.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,37 +37,45 @@
             return value
 
     return wrapped_component_function
 
 
 class ComponentsGeneric:
     def get_key_based_on_call(self, message):
-        """
-        Get the concat the functions call line and arguments to get a key
+        """Displays a navigation bar with a list of items.
 
-        * Gothca * : loop will be on the same line and therefor get the same key,
-                     we need the user to specify a key in that case
-                     this case is not checked for atm
+        Args:
+            label (List[str]): List of items to display in the navigation bar.
+            key (str, optional): Unique key for the component. Defaults to None.
+            default_value (Any, optional): Default value for the navigation bar. Defaults to None.
+        Concatenate the function's call line and arguments to get a key.
+
+        * Gotcha * : Loop will be on the same line and therefore get the same key,
+                     we need the user to specify a key in that case.
+                     This case is not checked for at the moment.
         """
         for i in range(20):
             # import ipdb; ipdb.set_trace()
             inspect_caller = getframeinfo(stack()[i][0])
             if "HS_STREAM_USER_FILE" in inspect_caller.filename:
                 call_signiture = (
                     f"{Path(inspect_caller.filename).stem}, {inspect_caller.lineno}"
                 )
                 key = "".join(x for x in call_signiture if x.isalpha() or x.isnumeric())
                 return key
 
     def component_value(self, default_value=None, key=None, **kwargs):
-        """Writes a component to the HS front end
+        """Get the value of a component from the HS front end.
 
         Args:
-            label (_type_, optional): Must be unique within the app. Content to write to the web front end. Defaults to None.
-            default_value (_type_, optional): default value the component returns before use enters value - will always be null for text or component where user doesn't input. Defaults to None.
+            default_value (Any, optional): Default value the component returns before user enters value. Defaults to None.
+            key (str, optional): Unique key for the component. Defaults to None.
+
+        Returns:
+            Any: The value of the component.
         """
         # `_hs_session` is injected by the django view - it contains values the user has inputted and sent to
         #  the django server
         return _hs_session.get(key, default_value)  # noqa: F821
 
 
 class Components(ComponentsGeneric):
@@ -87,21 +95,26 @@
         self,
         label: str,
         default_value: str = "",
         key: str = None,
         placeholder: str = False,
         **kwargs,
     ) -> str:
-        """Displays text input for user to input text
+        """Displays text input for user to input text.
 
         Args:
-            text (str): label to display to user describing the text input
-            default_value (str): value innitially entered into text box
+            label (str): Label to display to user describing the text input.
+            default_value (str, optional): Value initially entered into text box. Defaults to "".
+            key (str, optional): Unique key for the component. Defaults to None.
+            placeholder (str, optional): Placeholder text for the input box. Defaults to False.
+
         Returns:
-            str: text inputted by user
+            str: Text inputted by user.
+        Returns:
+            str: Text inputted by user.
         """
         with self.tag("label"):
             self.text(label)
         with self.tag(
             "input",
             ("hx-ext", "debug"),
             ("name", "new_value"),
@@ -118,18 +131,23 @@
     def html(self, *args, **kwargs):
         return self.tag(*args, **kwargs)
 
     @component_wrapper
     def number_input(
         self, label: str, default_value: int = 0, key: str = None, **kwargs
     ) -> str:
-        """Displays text input for user to input text
+        """Displays number input for user to input a number.
+
         Args:
-            text (str): label to display to user describing the text input
-            default_value (str): value innitially entered into text box
+            label (str): Label to display to user describing the number input.
+            default_value (int, optional): Value initially entered into number box. Defaults to 0.
+            key (str, optional): Unique key for the component. Defaults to None.
+
+        Returns:
+            str: Number inputted by user.
         Returns:
             str: text inputted by user
         """
         with self.tag("label"):
             self.text(label)
         with self.tag(
             "input",
@@ -141,24 +159,23 @@
         ):
             pass
 
     @component_wrapper
     def select_box(
         self, label: List[str], default_value: str = None, key: str = None, **kwargs
     ) -> str:
-        """
-        Dropdown component for user to select from a list of options
+        """Dropdown component for user to select from a list of options.
 
         Args:
-            label (List[str]): Options to display to user
-            default_value (str, optional): Value to select when component load the first time. Defaults to False.
-            key (str, optional): Unique key - default is set based on label (options) so set this if there are multiple inputs with same label argument. Defaults to None.
+            label (List[str]): Options to display to user.
+            default_value (str, optional): Value to select when component loads the first time. Defaults to None.
+            key (str, optional): Unique key for the component. Defaults to None.
 
         Returns:
-            str: Selected value
+            str: Selected value.
         """
         # HStream developer note: The default value logic is handled by the `@component_wrapper`
         with self.doc.select(
             ("name", "new_value"),
             ("hx-post", f"/set_component_value?component_id={key}"),
         ):
             for value in label:
@@ -172,24 +189,24 @@
                     self.text(str(value))
 
     # @component_wrapper
     # def multiselect(
     #     self, label: List[str], default_value: List[int] = [], key: str = None, **kwargs
     # ) -> List[int]:
     #     """
-    #     Dropdown component for user to select multiple options from a list and returns a comma separated string of the  of selected options
+    #     """Dropdown component for user to select multiple options from a list.
 
     #     Args:
-    #         label (List[str]): Options to display to user
-    #         default_value (str, optional): Value to select when component load the first time. Defaults to False.
-    #         key (str, optional): Unique key - default is set based on label (options) so set this if there are multiple inputs with same label argument. Defaults to None.
+    #         label (List[str]): Options to display to user.
+    #         default_value (List[int], optional): Values to select when component loads the first time. Defaults to [].
+    #         key (str, optional): Unique key for the component. Defaults to None.
 
     #     Returns:
-    #         str: Selected value
-    #     """
+    #         List[int]: Selected values.
+    # #     """
 
     #     assert type(label) == type([]) and type(default_value) == type(
     #         []
     #     ), "multiselect requires a list of options and a list of default values"
 
     #     # HStream developer note: The default value logic is handled by the `@component_wrapper`
     #     if type(kwargs["value"]) == type(""):
@@ -266,15 +283,26 @@
         label: str,
         minValue: int,
         maxValue: int,
         default_value: int = None,
         key: str = None,
         **kwargs,
     ) -> str:
-        """ """
+        """Displays a slider for user to input a value within a range.
+
+        Args:
+            label (str): Label to display to user describing the slider.
+            minValue (int): Minimum value of the slider.
+            maxValue (int): Maximum value of the slider.
+            default_value (int, optional): Value initially set on the slider. Defaults to None.
+            key (str, optional): Unique key for the component. Defaults to None.
+
+        Returns:
+            str: Value selected by user.
+        """
         with self.tag("label", ("for", key)):
             self.text(label)
         with self.tag(
             "input",
             ("name", "new_value"),
             ("id", key),
             ("type", "range"),
@@ -339,20 +367,24 @@
                                     "a",
                                     # ("style", f"color:{color}"),
                                 ):
                                     self.text(str(item))
 
     @component_wrapper
     def pyplot(self, fig, height="200px", key: str = None, **kwargs) -> None:
-        """Displays matplotlib plot to user
+        """Displays a matplotlib plot to the user.
+
         Args:
-            fig (matplotlib.figure.Figure): label to display to user describing the text input
+            fig (matplotlib.figure.Figure): Matplotlib figure to display.
+            height (str, optional): Height of the plot. Defaults to "200px".
+            key (str, optional): Unique key for the component. Defaults to None.
+
         Returns:
-            str: text inputted by user
-        Example:
+            None.
+        Example::
             import matplotlib.pyplot as plt
             import numpy as np
             x = np.arange(0,4*np.pi,0.1)   # start,stop,step
             y = np.sin(x) * float(sine_height)
             fig, ax = plt.subplots()
             ax.plot(x,y)
             hs.pyplot(fig, key='myplot')
@@ -382,53 +414,72 @@
     def checkbox(
         self,
         label: str,
         default_value: bool = False,
         key: str = None,
         **kwargs,
     ) -> str:
-        """ """
+        """Displays a checkbox for user to input a boolean value.
 
-        def bool_checker_fromat_fn(user_checkbox_value):
-            return user_checkbox_value == "True"
+        Args:
+            label (str): Label to display to user describing the checkbox.
+            default_value (bool, optional): Value initially set on the checkbox. Defaults to False.
+            key (str, optional): Unique key for the component. Defaults to None.
 
-        value = bool_checker_fromat_fn(kwargs["value"])
+        Returns:
+            str: Boolean value inputted by user.
+        """
+
+        def bool_checker_format_fn(user_checkbox_value):
+            return str(user_checkbox_value).lower() == "true"
+
+        value = bool_checker_format_fn(kwargs["value"])
         with self.tag("label", ("for", key)):
             with self.tag(
                 "input",
                 ("id", key),
                 ("type", "checkbox"),
                 (
                     "checked" if value else "notchecked",
                     "",
                 ),
                 # annoyingly a blank checkbox is not sent back in a submit event,
                 # so we attach the state of the checkbox here
                 # https://htmx.org/attributes/hx-vals/, https://github.com/bigskysoftware/htmx/issues/894
-                # ("hx-vals", "js:{" + key + ": event.srcElement.checked}"),
-                # ("hx-post", f"/set_component_value?component_id={key}"),
-                (
-                    "hx-post",
-                    f"/set_component_value/?component_id={key}&new_value={not value}",
-                ),
+                ("hx-vals", "js:{new_value: event.srcElement.checked}"),
+                ("hx-post", f"/set_component_value?component_id={key}"),
+                # (
+                #     "hx-get",
+                #     f"/set_component_value/?component_id={key}&new_value={not value}",
+                # ),
             ):
                 pass
             self.text(label)
-        return bool_checker_fromat_fn
+        return bool_checker_format_fn
 
     @component_wrapper
     def button(
         self,
         label: str,
         default_value: bool = False,
         key: str = None,
         full_width: bool = False,
         **kwargs,
     ) -> bool:
-        """ """
+        """Displays a button for user to click.
+
+        Args:
+            label (str): Label to display on the button.
+            default_value (bool, optional): Value initially set on the button. Defaults to False.
+            key (str, optional): Unique key for the component. Defaults to None.
+            full_width (bool, optional): Whether the button should take the full width of its container. Defaults to False.
+
+        Returns:
+            bool: True if the button is clicked, otherwise False.
+        """
         with self.tag(
             "button",
             ("id", key),
             ("type", "submit") if full_width else ("type", "button"),
             ("hx-trigger", "click"),
             ("hx-post", f"/set_component_value?component_id={key}&new_value=true"),
             ("hx-swap", "none"),
@@ -440,19 +491,23 @@
         ] = False  # set the button back to false after it has been clicked
         return lambda s: True if s in ["True", "true", True] else False
 
     def grid(self, *args, **kwargs):
         return self.tag("div", ("class", "grid"), *args, **kwargs)
 
     def write_dataframe(self, df, key: str = None, striped=False, **kwargs) -> None:
-        """Writes a dataframe to the
+        """Writes a dataframe to the web front end.
 
         Args:
-            df (pd.DataFrame): Dataframe to write to the web front end
-            key (str): Must be unique within the app. Used to reference the dataframe in the front end
+            df (pd.DataFrame): Dataframe to write to the web front end.
+            key (str, optional): Unique key for the component. Defaults to None.
+            striped (bool, optional): Whether to add striped styling to the table. Defaults to False.
+
+        Returns:
+            None
         """
         with self.tag(
             "div",
             klass="overflow-auto",
         ):
             html = (
                 df.to_html(classes="", border="", justify="unset")
```

### Comparing `hstream-0.1.48/hstream/components/styling_components.py` & `hstream-0.1.49/hstream/components/styling_components.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.48/hstream/django_server/hs/session_utils.py` & `hstream-0.1.49/hstream/django_server/hs/session_utils.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.48/hstream/django_server/hs/views.py` & `hstream-0.1.49/hstream/django_server/hs/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,19 +146,29 @@
                 compiled_code,
                 namespace,
             )
             try:
                 for var_name, var_value in namespace.items():
                     if var_value.__class__.__name__ == "hs":
                         users_hs_instance = var_value
+                if users_hs_instance is None:
+                    raise ValueError(
+                        "Seems your file does not import hs `from hstream import hs`"
+                    )
                 html = users_hs_instance.doc.getvalue()
                 # TODO: if the script sets component values we should honour these as well
                 # for example a button reverting itself back to false after being clicked
                 request.session = namespace["__builtins__"]["_hs_session"]
                 set_session_var(request, "hs_html", html)
+            except ValueError as e:
+                if (
+                    e.args[0]
+                    == "Seems your file does not import hs `from hstream import hs`"
+                ):
+                    raise e
             except:  # noqa #E722
                 pass
     except Exception as e:
         e.args = (f"Line: {line}, code: {block}", *e.args)
         raise e
     finally:
         users_hs_instance.clear()
```

### Comparing `hstream-0.1.48/hstream/django_server/manage.py` & `hstream-0.1.49/hstream/django_server/manage.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.48/hstream/django_server/root/settings.py` & `hstream-0.1.49/hstream/django_server/root/settings.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.48/hstream/django_server/root/urls.py` & `hstream-0.1.49/hstream/django_server/root/urls.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.48/hstream/hs.py` & `hstream-0.1.49/hstream/hs.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.48/hstream/run.py` & `hstream-0.1.49/hstream/run.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,9 +10,10 @@
 ):
     path_to_hstream_dir = os.path.dirname(os.path.abspath(hstream.__file__))
 
     os.system(f"python {path_to_hstream_dir}/django_server/manage.py migrate")
     os.environ["HS_FILE_TO_RUN"] = str(file)
     command = f"python {path_to_hstream_dir}/django_server/manage.py runserver"
     if os.environ.get("PORT", False):
+        print(f"found port in env, using port {os.environ['PORT']}")
         command += f" 0.0.0.0:{os.environ['PORT']}"
     os.system(command)
```

### Comparing `hstream-0.1.48/hstream/templates/format_html.html` & `hstream-0.1.49/hstream/templates/format_html.html`

 * *Files identical despite different names*

### Comparing `hstream-0.1.48/hstream/utils.py` & `hstream-0.1.49/hstream/utils.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.48/pyproject.toml` & `hstream-0.1.49/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hstream"
-version = "0.1.48"
+version = "0.1.49"
 description = ""
 authors = ["Conrad <conradbez1@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 hstream = "hstream.cli:cli"
```

### Comparing `hstream-0.1.48/PKG-INFO` & `hstream-0.1.49/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hstream
-Version: 0.1.48
+Version: 0.1.49
 Summary: 
 Author: Conrad
 Author-email: conradbez1@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

