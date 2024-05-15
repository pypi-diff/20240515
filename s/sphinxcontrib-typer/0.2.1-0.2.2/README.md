# Comparing `tmp/sphinxcontrib_typer-0.2.1.tar.gz` & `tmp/sphinxcontrib_typer-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib_typer-0.2.1.tar", max compression
+gzip compressed data, was "sphinxcontrib_typer-0.2.2.tar", max compression
```

## Comparing `sphinxcontrib_typer-0.2.1.tar` & `sphinxcontrib_typer-0.2.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1068 2024-04-11 19:06:12.851603 sphinxcontrib_typer-0.2.1/LICENSE
--rw-r--r--   0        0        0     5272 2024-04-11 20:21:38.783615 sphinxcontrib_typer-0.2.1/README.md
--rw-r--r--   0        0        0     3124 2024-04-11 20:23:05.351328 sphinxcontrib_typer-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    34776 2024-04-11 20:22:02.389785 sphinxcontrib_typer-0.2.1/sphinxcontrib/typer/__init__.py
--rw-r--r--   0        0        0     6912 1970-01-01 00:00:00.000000 sphinxcontrib_typer-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-12-14 00:10:27.893967 sphinxcontrib_typer-0.2.2/LICENSE
+-rw-r--r--   0        0        0     5272 2024-05-15 04:52:56.770601 sphinxcontrib_typer-0.2.2/README.md
+-rw-r--r--   0        0        0     2914 2024-05-15 05:55:36.320976 sphinxcontrib_typer-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0    34219 2024-05-15 05:54:45.783863 sphinxcontrib_typer-0.2.2/sphinxcontrib/typer/__init__.py
+-rw-r--r--   0        0        0     6899 1970-01-01 00:00:00.000000 sphinxcontrib_typer-0.2.2/PKG-INFO
```

### Comparing `sphinxcontrib_typer-0.2.1/LICENSE` & `sphinxcontrib_typer-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_typer-0.2.1/README.md` & `sphinxcontrib_typer-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_typer-0.2.1/pyproject.toml` & `sphinxcontrib_typer-0.2.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphinxcontrib-typer"
-version = "0.2.1"
+version = "0.2.2"
 description = "Auto generate docs for typer commands."
 authors = ["Brian Kohan <bckohan@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sphinx-contrib/typer"
 homepage = "https://sphinxcontrib-typer.readthedocs.io"
 classifiers = [
@@ -12,47 +12,45 @@
     "Environment :: Console",
     "Environment :: Web Environment",
     "Framework :: Sphinx :: Extension",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Documentation",
     "Topic :: Utilities",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 packages = [
   { include = "sphinxcontrib", from = "" }
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 sphinx = ">=4.0.0"
+
 selenium = "^4.0.0"
 webdriver-manager = ">=3.0.0,<5.0.0"
 cairosvg = "^2.4.0"
 lxml = ">=4.2.0,<6.0.0"
 typer-slim = {extras = ["standard"], version = ">=0.12.0,<1.0.0"}
 pillow = ">=8.0.0"
+ruff = "^0.4.4"
 
 [tool.poetry.group.dev.dependencies]
 sphinx-rtd-theme = ">=1.0.0"
 ipdb = "^0.13.13"
 pytest = ">=7.4.3,<9.0.0"
-isort = "^5.13.2"
-pylint = "^3.0.3"
 pytest-cov = "^4.1.0"
 doc8 = ">0.1"
-black = ">=23.12,<25.0"
 mypy = "^1.7.1"
 readme-renderer = {extras = ["md"], version = ">=42,<44"}
 aiohttp = "^3.9.1"
 numpy = [
     { version = ">=1.26", markers = "python_version > '3.8'" },
     { version = "<=1.24", markers = "python_version <= '3.8'" },
 ]
@@ -79,31 +77,25 @@
 pdf = ["cairosvg", "lxml"]
 png = ["selenium", "webdriver-manager", "pillow"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.black]
-line-length = 80
-target-version = ['py38']
-skip-string-normalization = true
-exclude = '''
-(
-  /(
-      \.eggs
-    | \.git
-    | \.tox
-    | \.venv
-    | build
-    | dist
-    | doc
-  )
-)
-'''
+[tool.ruff]
+line-length = 88
+exclude = [
+    "doc",
+    "dist"
+]
+
+[tool.ruff.lint]
+exclude = [
+    "tests/**/*"
+]
 
 [tool.pytest.ini_options]
 testpaths = [
     "tests/tests.py",
 ]
 addopts = [
     "--doctest-modules",
@@ -114,13 +106,9 @@
     "--cov-report=term-missing:skip-covered",
     "--no-cov-on-fail",
     #"-x",
     #"--pdb",
     #"--flake8",
 ]
 
-[tool.isort]
-profile = "black"
-
 [tool.doc8]
 max-line-length = 100
-
```

### Comparing `sphinxcontrib_typer-0.2.1/sphinxcontrib/typer/__init__.py` & `sphinxcontrib_typer-0.2.2/sphinxcontrib/typer/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,66 +44,62 @@
 from sphinx.util import logging
 
 from typer import rich_utils as typer_rich_utils
 from typer.main import Typer, TyperGroup
 from typer.main import get_command as get_typer_command
 from typer.models import Context as TyperContext
 
-VERSION = (0, 2, 1)
+VERSION = (0, 2, 2)
 
-__title__ = 'SphinxContrib Typer'
-__version__ = '.'.join(str(i) for i in VERSION)
-__author__ = 'Brian Kohan'
-__license__ = 'MIT'
-__copyright__ = 'Copyright 2023 Brian Kohan'
+__title__ = "SphinxContrib Typer"
+__version__ = ".".join(str(i) for i in VERSION)
+__author__ = "Brian Kohan"
+__license__ = "MIT"
+__copyright__ = "Copyright 2023 Brian Kohan"
 
 
 SELENIUM_DEFAULT_WINDOW_WIDTH = 1920
 SELENIUM_DEFAULT_WINDOW_HEIGHT = 2048
 
 
-def _filter_commands(
-    ctx: click.Context, cmd_filter: t.Optional[t.List[str]] = None
-):
+def _filter_commands(ctx: click.Context, cmd_filter: t.Optional[t.List[str]] = None):
     return sorted(
         [
             cmd
             for name, cmd in getattr(
                 ctx.command,
-                'commands',
+                "commands",
                 {
                     name: ctx.command.get_command(ctx, name)
-                    for name in getattr(
-                        ctx.command, 'list_commands', lambda _: []
-                    )(ctx)
+                    for name in getattr(ctx.command, "list_commands", lambda _: [])(ctx)
                     or cmd_filter
                     or []
                 },
             ).items()
             if not cmd_filter or name in cmd_filter
         ],
         key=lambda item: item.name,
     )
 
 
 class RenderTarget(str, Enum):
-    HTML = 'html'
-    SVG = 'svg'
-    TEXT = 'text'
+    HTML = "html"
+    SVG = "svg"
+    TEXT = "text"
 
     def __str__(self) -> str:
         return self.value
 
 
 class RenderTheme(str, Enum):
-    LIGHT = 'light'
-    MONOKAI = 'monokai'
-    DIMMED_MONOKAI = 'dimmed_monokai'
-    NIGHT_OWLISH = 'night_owlish'
-    DARK = 'dark'
+    LIGHT = "light"
+    MONOKAI = "monokai"
+    DIMMED_MONOKAI = "dimmed_monokai"
+    NIGHT_OWLISH = "night_owlish"
+    DARK = "dark"
 
     def __str__(self) -> str:
         return self.value
 
     @property
     def terminal_theme(self) -> rich_theme.TerminalTheme:
         return {
@@ -119,15 +115,15 @@
 
 """
 Callbacks that return a dict of kwargs to pass to various renderer functions
 must all have the RenderCallback function signature:
 """
 RenderCallback = t.Callable[
     [
-        'TyperDirective',  # directive - the TyperDirective instance
+        "TyperDirective",  # directive - the TyperDirective instance
         str,  # name - the name of the command
         Command,  # command - the command instance
         click.Context,  # ctx - the click.Context instance
         t.Optional[click.Context],  # parent - the parent click.Context instance
     ],
     t.Dict[str, t.Any],
 ]
@@ -150,33 +146,33 @@
 
     .. code-block:: rst
 
         .. typer:: import.path.to.typer.app:subcommand
             :prog: script_name
     """
 
-    logger = logging.getLogger('sphinxcontrib.typer')
+    logger = logging.getLogger("sphinxcontrib.typer")
 
     has_content = False
     required_arguments = 1
     option_spec = {
-        'prog': directives.unchanged_required,
-        'make-sections': directives.flag,
-        'show-nested': directives.flag,
-        'markup-mode': directives.unchanged,
-        'width': directives.nonnegative_int,
-        'theme': RenderTheme,
-        'svg-kwargs': directives.unchanged,
-        'text-kwargs': directives.unchanged,
-        'html-kwargs': directives.unchanged,
-        'console-kwargs': directives.unchanged,
-        'preferred': RenderTarget,
-        'builders': directives.unchanged,
-        'iframe-height': directives.nonnegative_int,
-        'convert-png': directives.unchanged,
+        "prog": directives.unchanged_required,
+        "make-sections": directives.flag,
+        "show-nested": directives.flag,
+        "markup-mode": directives.unchanged,
+        "width": directives.nonnegative_int,
+        "theme": RenderTheme,
+        "svg-kwargs": directives.unchanged,
+        "text-kwargs": directives.unchanged,
+        "html-kwargs": directives.unchanged,
+        "console-kwargs": directives.unchanged,
+        "preferred": RenderTarget,
+        "builders": directives.unchanged,
+        "iframe-height": directives.nonnegative_int,
+        "convert-png": directives.unchanged,
     }
 
     # resolved options
     prog_name: str
     nested: bool
     make_sections: bool
     width: int
@@ -200,28 +196,28 @@
 
     target: RenderTarget
 
     builder_targets = {
         **{
             builder: [RenderTarget.SVG, RenderTarget.HTML, RenderTarget.TEXT]
             for builder in [
-                'html',
-                'dirhtml',
-                'singlehtml',
-                'htmlhelp',
-                'qthelp',
-                'devhelp',
+                "html",
+                "dirhtml",
+                "singlehtml",
+                "htmlhelp",
+                "qthelp",
+                "devhelp",
             ]
         },
-        'epub': [RenderTarget.HTML, RenderTarget.SVG, RenderTarget.TEXT],
+        "epub": [RenderTarget.HTML, RenderTarget.SVG, RenderTarget.TEXT],
         **{
             builder: [RenderTarget.SVG, RenderTarget.TEXT]
-            for builder in ['latex', 'latexpdf', 'texinfo']
+            for builder in ["latex", "latexpdf", "texinfo"]
         },
-        **{builder: [RenderTarget.TEXT] for builder in ['text', 'gettext']},
+        **{builder: [RenderTarget.TEXT] for builder in ["text", "gettext"]},
     }
 
     @property
     def builder(self) -> str:
         return self.env.app.builder.name
 
     def uuid(self, normal_cmd: str) -> str:
@@ -234,67 +230,65 @@
         :param normal_cmd: The normalized command name
         """
         # Contextual information
         source = self.state_machine.get_source_and_line()[0]
         line_number = self.state_machine.get_source_and_line()[1]
         source = os.path.relpath(source, self.env.app.builder.srcdir)
         return hashlib.sha256(
-            f"{source}.{line_number}[{normal_cmd}]".encode('utf-8')
+            f"{source}.{line_number}[{normal_cmd}]".encode("utf-8")
         ).hexdigest()[:8]
 
     def import_object(
         self,
         obj_path: t.Optional[str],
-        accessor: t.Callable[
-            [t.Any, str], t.Any
-        ] = lambda obj, attr, _: getattr(obj, attr),
+        accessor: t.Callable[[t.Any, str, t.Any], t.Any] = lambda obj, attr, _: getattr(
+            obj, attr
+        ),
     ) -> t.Any:
         """
         Imports an arbitrary object from a python string path.
         Delimiters can be '.', '::' or ':'.
 
         :param obj_path: The python path to the object, if False, returns None
         """
         if not obj_path:
             return None
-        parts = re.split(r'::|[.:]', obj_path)
+        parts = re.split(r"::|[.:]", obj_path)
         tries = 1
         try:
             while True:
                 # walk up the import path until we find something importable
                 # then walk down the path fetching all the attributes
                 # this allows import strings to reach into nested class
                 # attributes
                 try:
                     tries += 1
-                    try_path = '.'.join(parts[0 : -(tries - 1)])
+                    try_path = ".".join(parts[0 : -(tries - 1)])
                     obj = import_module(try_path)
                     for attr in parts[-(tries - 1) :]:
                         obj = accessor(obj, attr, try_path)
                     break
                 except (ImportError, ModuleNotFoundError):
                     if tries >= len(parts):
                         raise
 
         except (Exception, SystemExit) as exc:
             err_msg = f'Failed to import "{obj_path}"'
             if isinstance(exc, SystemExit):
-                err_msg += 'The module appeared to call sys.exit().'
+                err_msg += "The module appeared to call sys.exit()."
             else:
-                err_msg += 'The following exception was raised:\n{}'.format(
+                err_msg += "The following exception was raised:\n{}".format(
                     traceback.format_exc()
                 )
 
             raise self.severe(err_msg)
 
         return obj
 
-    def load_root_command(
-        self, typer_path: str
-    ) -> t.Union[click.Command, click.Group]:
+    def load_root_command(self, typer_path: str) -> t.Union[click.Command, click.Group]:
         """
         Load the module.
 
         :param typer_path: The python path to the Typer app instance.
         """
 
         def resolve_root_command(obj):
@@ -309,15 +303,15 @@
                 if isinstance(ret, Typer):
                     return get_typer_command(obj)
                 if isinstance(ret, (click.Command, click.Group)):
                     return ret
 
             raise self.error(
                 f'"{typer_path}" of type {type(obj)} is not Typer, click.Command or '
-                'click.Group.'
+                "click.Group."
             )
 
         def access_command(
             obj, attr, imprt_path
         ) -> t.Union[click.Command, click.Group]:
             attr_obj = None
             try:
@@ -331,21 +325,21 @@
                         # command - but it is probably the best bet for
                         # subsequent commands - so if this is a nested
                         # import pull out the name attribute if it exists
                         # otherwise we use the last successful import path
                         # part because it is probably the module with main
                         info_name=(
                             (
-                                getattr(obj, 'name', '')
-                                if getattr(self, 'parent', None)
-                                else ''
+                                getattr(obj, "name", "")
+                                if getattr(self, "parent", None)
+                                else ""
                             )
-                            or imprt_path.split('.')[-1]
+                            or imprt_path.split(".")[-1]
                         ),
-                        parent=getattr(self, 'parent', None),
+                        parent=getattr(self, "parent", None),
                     )
                     cmds = _filter_commands(self.parent, [attr])
                     if cmds:
                         return cmds[0]
                 except (IndexError, rst.DirectiveError):
                     if attr_obj:
                         return attr_obj
@@ -353,24 +347,24 @@
 
         return resolve_root_command(
             self.import_object(typer_path, accessor=access_command)
         )
 
     def get_html(self, **options):
         return self.console.export_html(
-            **{'theme': self.theme.terminal_theme, **options, 'clear': False}
+            **{"theme": self.theme.terminal_theme, **options, "clear": False}
         )
 
     def get_svg(self, **options):
         return self.console.export_svg(
-            **{'theme': self.theme.terminal_theme, **options, 'clear': False}
+            **{"theme": self.theme.terminal_theme, **options, "clear": False}
         )
 
     def get_text(self, **options):
-        return self.console.export_text(**{**options, 'clear': False})
+        return self.console.export_text(**{**options, "clear": False})
 
     def generate_nodes(
         self,
         name: str,
         command: click.Command,
         parent: t.Optional[click.Context],
     ) -> t.List[nodes.section]:
@@ -391,24 +385,24 @@
             max_content_width=self.width,
         )
 
         if command.hidden:
             return []
 
         source_name = ctx.command_path
-        normal_cmd = ':'.join(source_name.split(' '))
+        normal_cmd = ":".join(source_name.split(" "))
 
         section = (
             nodes.section(
-                '',
+                "",
                 nodes.title(
                     text=(
                         name
-                        if not getattr(self, 'parent', None)
-                        else f'{self.parent.command_path} {name}'
+                        if not getattr(self, "parent", None)
+                        else f"{self.parent.command_path} {name}"
                     )
                 ),
                 ids=[nodes.make_id(source_name)],
                 names=[nodes.fully_normalize_name(source_name)],
             )
             if self.make_sections
             else nodes.container()
@@ -419,204 +413,184 @@
             options: RenderOptions, parameter: str
         ) -> t.Dict[str, t.Any]:
             if callable(options):
                 options = options(self, name, command, ctx, parent)
             if isinstance(options, dict):
                 return options
             raise self.severe(
-                f'Invalid {parameter}, must be a dict or callable, got {type(options)}'
+                f"Invalid {parameter}, must be a dict or callable, got {type(options)}"
             )
 
         def get_console(stderr: bool = False) -> Console:
             self.console = Console(
                 **{
-                    'theme': Theme(
+                    "theme": Theme(
                         {
                             "option": typer_rich_utils.STYLE_OPTION,
                             "switch": typer_rich_utils.STYLE_SWITCH,
                             "negative_option": typer_rich_utils.STYLE_NEGATIVE_OPTION,
                             "negative_switch": typer_rich_utils.STYLE_NEGATIVE_SWITCH,
                             "metavar": typer_rich_utils.STYLE_METAVAR,
                             "metavar_sep": typer_rich_utils.STYLE_METAVAR_SEPARATOR,
                             "usage": typer_rich_utils.STYLE_USAGE,
                         },
                     ),
-                    'highlighter': typer_rich_utils.highlighter,
-                    'color_system': typer_rich_utils.COLOR_SYSTEM,
-                    'force_terminal': typer_rich_utils.FORCE_TERMINAL,
-                    'width': self.width or typer_rich_utils.MAX_WIDTH,
-                    'stderr': stderr,
+                    "highlighter": typer_rich_utils.highlighter,
+                    "color_system": typer_rich_utils.COLOR_SYSTEM,
+                    "force_terminal": typer_rich_utils.FORCE_TERMINAL,
+                    "width": self.width or typer_rich_utils.MAX_WIDTH,
+                    "stderr": stderr,
                     # overrides any defaults above
-                    **resolve_options(self.console_kwargs, 'console-kwargs'),
-                    'record': True,
+                    **resolve_options(self.console_kwargs, "console-kwargs"),
+                    "record": True,
                 }
             )
             return self.console
 
         # todo
         # typer provides no official way to alter the console that prints out the help
         # command so we have to monkey patch it - revisit in future if this changes!
         # we also monkey patch get_help incase its a click command
         orig_getter = typer_rich_utils._get_rich_console
         orig_format_help = command.format_help
         command.rich_markup_mode = getattr(
-            self, 'markup_mode', getattr(command, 'rich_markup_mode', None)
-        )
-        command.format_help = TyperGroup.format_help.__get__(
-            command, command.__class__
+            self, "markup_mode", getattr(command, "rich_markup_mode", None)
         )
+        command.format_help = TyperGroup.format_help.__get__(command, command.__class__)
         typer_rich_utils._get_rich_console = get_console
         with contextlib.redirect_stdout(io.StringIO()):
             command.get_help(ctx)
         typer_rich_utils._get_rich_console = orig_getter
         command.format_help = orig_format_help
         ##############################################################################
 
         export_options = resolve_options(
-            getattr(self, f'{self.target}_kwargs', {}), f'{self.target}-kwargs'
+            getattr(self, f"{self.target}_kwargs", {}), f"{self.target}-kwargs"
         )
 
-        rendered = getattr(self, f'get_{self.target}')(
-            **(
-                {'title': source_name}
-                if self.target is RenderTarget.SVG
-                else {}
-            ),
+        rendered = getattr(self, f"get_{self.target}")(
+            **({"title": source_name} if self.target is RenderTarget.SVG else {}),
             **export_options,
         )
 
         if self.typer_convert_png:
             png_path = Path(self.env.app.builder.outdir) / (
                 f'{normal_cmd.replace(":", "_")}_{self.uuid(normal_cmd)}.png'
             )
             self.env.app.config.typer_convert_png(self, rendered, png_path)
             section += nodes.image(
                 uri=os.path.relpath(png_path, Path(self.env.srcdir)),
                 alt=source_name,
             )
         elif self.target == RenderTarget.HTML:
             section += nodes.raw(
-                '',
-                self.env.app.config.typer_render_html(
-                    self, normal_cmd, rendered
-                ),
-                format='html',
+                "",
+                self.env.app.config.typer_render_html(self, normal_cmd, rendered),
+                format="html",
             )
         elif self.target == RenderTarget.SVG:
-            if 'html' in self.builder:
-                section += nodes.raw('', rendered, format='html')
+            if "html" in self.builder:
+                section += nodes.raw("", rendered, format="html")
             else:
-                img_name = (
-                    f'{normal_cmd.replace(":", "_")}_{self.uuid(normal_cmd)}'
-                )
+                img_name = f'{normal_cmd.replace(":", "_")}_{self.uuid(normal_cmd)}'
                 out_dir = Path(self.env.app.builder.outdir)
-                (out_dir / f'{img_name}.svg').write_text(rendered)
-                pdf_img = out_dir / f'{img_name}.pdf'
+                (out_dir / f"{img_name}.svg").write_text(rendered)
+                pdf_img = out_dir / f"{img_name}.pdf"
                 self.env.app.config.typer_svg2pdf(self, rendered, pdf_img)
                 section += nodes.image(
                     uri=os.path.relpath(pdf_img, Path(self.env.srcdir)),
                     alt=source_name,
                 )
 
         elif self.target == RenderTarget.TEXT:
-            section += nodes.literal_block('', rendered)
+            section += nodes.literal_block("", rendered)
         else:
-            raise self.severe(f'Invalid typer render target: {self.target}')
+            raise self.severe(f"Invalid typer render target: {self.target}")
 
         # recurse through subcommands if we should
         if self.nested and isinstance(command, click.MultiCommand):
             commands = _filter_commands(ctx, command.list_commands(ctx))
             for command in commands:
-                section.extend(
-                    self.generate_nodes(command.name, command, parent=ctx)
-                )
+                section.extend(self.generate_nodes(command.name, command, parent=ctx))
         return [section]
 
     def run(self) -> t.Iterable[nodes.section]:
         self.env = self.state.document.settings.env
 
         command = self.load_root_command(self.arguments[0])
 
-        self.make_sections = 'make-sections' in self.options
-        self.nested = 'show-nested' in self.options
-        self.prog_name = self.options.get('prog', None)
-        if 'markup-mode' in self.options:
-            self.markup_mode = self.options['markup-mode']
+        self.make_sections = "make-sections" in self.options
+        self.nested = "show-nested" in self.options
+        self.prog_name = self.options.get("prog", None)
+        if "markup-mode" in self.options:
+            self.markup_mode = self.options["markup-mode"]
 
         if not self.prog_name:
             try:
                 self.prog_name = (
-                    command.callback.__module__.split('.')[-1]
-                    if hasattr(command, 'callback')
-                    and not hasattr(self, 'parent')
-                    else re.split(r'::|[.:]', self.arguments[0])[-1]
+                    command.callback.__module__.split(".")[-1]
+                    if hasattr(command, "callback") and not hasattr(self, "parent")
+                    else re.split(r"::|[.:]", self.arguments[0])[-1]
                 )
             except Exception as err:
                 raise self.severe(
-                    'Unable to determine program name, please specify using '
-                    ':prog:'
+                    "Unable to determine program name, please specify using " ":prog:"
                 ) from err
 
-        self.width = self.options.get('width', 65)
-        self.iframe_height = self.options.get('iframe-height', None)
+        self.width = self.options.get("width", 65)
+        self.iframe_height = self.options.get("iframe-height", None)
 
         # if no builders supplied but convert-png is set,
         # force png for all builders, otherwise require the builder
         # to be in the list of typer_convert_png builders
-        self.typer_convert_png = 'convert-png' in self.options
+        self.typer_convert_png = "convert-png" in self.options
         if self.typer_convert_png:
-            builders = self.options['convert-png'].strip()
-            self.typer_convert_png = (
-                self.builder in builders if builders else True
-            )
+            builders = self.options["convert-png"].strip()
+            self.typer_convert_png = self.builder in builders if builders else True
 
-        for trg in ['console', *list(RenderTarget)]:
+        for trg in ["console", *list(RenderTarget)]:
             setattr(
                 self,
-                f'{trg}_kwargs',
-                self.import_object(self.options.get(f'{trg}-kwargs', None))
-                or {},
+                f"{trg}_kwargs",
+                self.import_object(self.options.get(f"{trg}-kwargs", None)) or {},
             )
 
-        self.preferred = self.options.get('preferred', None)
-        self.theme = self.options.get('theme', self.theme)
+        self.preferred = self.options.get("preferred", None)
+        self.theme = self.options.get("theme", self.theme)
 
         builder_targets = {}
-        for builder_target in self.options.get('builders', '').split(':'):
+        for builder_target in self.options.get("builders", "").split(":"):
             if builder_target.strip():
-                builder, targets = builder_target.split('=')[0:2]
+                builder, targets = builder_target.split("=")[0:2]
                 builder_targets[builder.strip()] = [
-                    RenderTarget(target.strip())
-                    for target in targets.split(',')
+                    RenderTarget(target.strip()) for target in targets.split(",")
                 ]
 
         builder_targets = {**self.builder_targets, **builder_targets}
 
         if self.typer_convert_png:
             self.target = (
                 self.preferred
-                or (
-                    builder_targets.get(self.builder, []) or [RenderTarget.SVG]
-                )[0]
+                or (builder_targets.get(self.builder, []) or [RenderTarget.SVG])[0]
             )
         elif self.builder not in builder_targets:
             self.target = self.preferred or RenderTarget.TEXT
             self.logger.debug(
-                'Unable to resolve render target for builder: %s - using: %s',
+                "Unable to resolve render target for builder: %s - using: %s",
                 self.builder,
                 self.target,
             )
         else:
             supported = builder_targets[self.builder]
             self.target = (
                 self.preferred if self.preferred in supported else supported[0]
             )
 
         return self.generate_nodes(
-            self.prog_name, command, getattr(self, 'parent', None)
+            self.prog_name, command, getattr(self, "parent", None)
         )
 
 
 def typer_get_iframe_height(
     directive: TyperDirective, normal_cmd: str, html_page: str
 ) -> int:
     """
@@ -637,42 +611,42 @@
     :param normal_cmd: The normalized name of the command.
         (Subcommands are delimited by :)
     :param html_page: The full html document that will be rendered in the iframe
     """
     if directive.iframe_height is not None:
         return directive.iframe_height
 
-    cache = {'iframe_heights': {}}
+    cache = {"iframe_heights": {}}
     cache_path = (
         None
         if not directive.env.app.config.typer_iframe_height_cache_path
         else Path(directive.env.app.config.typer_iframe_height_cache_path)
     )
     if cache_path and cache_path.is_file():
         cache = json.loads(cache_path.read_text())
-        cache.setdefault('iframe_heights', {})
+        cache.setdefault("iframe_heights", {})
 
-    if cache['iframe_heights'].get(normal_cmd):
-        return cache['iframe_heights'][normal_cmd]
+    if cache["iframe_heights"].get(normal_cmd):
+        return cache["iframe_heights"][normal_cmd]
 
     with directive.env.app.config.typer_get_web_driver(directive) as driver:
         # use base64 to avoid issues with special characters
         driver.get(
             f'data:text/html;base64,'
             f'{base64.b64encode(html_page.encode("utf-8")).decode()}'
         )
         height = (
             int(
                 driver.execute_script(
-                    'return document.documentElement.getBoundingClientRect().height'
+                    "return document.documentElement.getBoundingClientRect().height"
                 )
             )
             + directive.env.app.config.typer_iframe_height_padding
         )
-    cache['iframe_heights'][normal_cmd] = height
+    cache["iframe_heights"][normal_cmd] = height
     if cache_path:
         cache_path.write_text(json.dumps(cache, indent=4))
     return height
 
 
 def typer_render_html(
     directive: TyperDirective, normal_cmd: str, html_page: str
@@ -714,15 +688,15 @@
     :param pdf_path: The path to write the pdf to
     """
     try:
         import cairosvg
 
         cairosvg.svg2pdf(bytestring=svg_contents, write_to=str(pdf_path))
     except ImportError:
-        directive.severe(f'cairosvg must be installed to render SVG in pdfs')
+        directive.severe("cairosvg must be installed to render SVG in pdfs")
 
 
 @contextmanager
 def typer_get_web_driver(
     directive: TyperDirective,
     width: int = SELENIUM_DEFAULT_WINDOW_WIDTH,
     height: int = SELENIUM_DEFAULT_WINDOW_HEIGHT,
@@ -744,16 +718,15 @@
     import platform
 
     try:
         from selenium import webdriver
         from selenium.webdriver.chrome.options import Options as ChromeOptions
     except ImportError:
         raise directive.severe(
-            f'This feature requires selenium and webdriver-manager to be '
-            'installed.'
+            "This feature requires selenium and webdriver-manager to be " "installed."
         )
 
     # Set up headless browser options
     def opts(options=ChromeOptions()):
         options.add_argument("--headless")
         options.add_argument("--no-sandbox")
         options.add_argument("--disable-dev-shm-usage")
@@ -802,33 +775,31 @@
         return webdriver.Edge(
             service=EdgeService(EdgeChromiumDriverManager().install()),
             options=opts(options),
         )
 
     services = [
         chrome,
-        edge if platform.system().lower() == 'windows' else chromium,
+        edge if platform.system().lower() == "windows" else chromium,
         firefox,
     ]
 
     driver = None
     for service in services:
         try:
             driver = service()
             break  # use the first one that works!
         except Exception as err:
-            directive.debug(
-                f'Unable to initialize webdriver {service.__name__}: {err}'
-            )
+            directive.debug(f"Unable to initialize webdriver {service.__name__}: {err}")
 
     if driver:
         yield driver
         driver.quit()
     else:
-        raise directive.severe(f'Unable to initialize any webdriver.')
+        raise directive.severe("Unable to initialize any webdriver.")
 
 
 def typer_convert_png(
     directive: TyperDirective,
     rendered: str,
     png_path: t.Union[str, Path],
     selenium_width: int = SELENIUM_DEFAULT_WINDOW_WIDTH,
@@ -850,54 +821,49 @@
     """
     import tempfile
     from io import BytesIO
 
     from PIL import Image
     from selenium.webdriver.common.by import By
 
-    tag = 'code'
+    tag = "code"
     with directive.env.app.config.typer_get_web_driver(directive) as driver:
-        with tempfile.NamedTemporaryFile(suffix='.html') as tmp:
+        with tempfile.NamedTemporaryFile(suffix=".html") as tmp:
             if directive.target is RenderTarget.TEXT:
-                tag = 'pre'
-                rendered = f'<html><body><pre>{rendered}</pre></body></html>'
+                tag = "pre"
+                rendered = f"<html><body><pre>{rendered}</pre></body></html>"
             elif directive.target is RenderTarget.SVG:
-                tag = 'svg'
-                rendered = f'<html><body>{rendered}</body></html>'
+                tag = "svg"
+                rendered = f"<html><body>{rendered}</body></html>"
 
-            tmp.write(rendered.encode('utf-8'))
+            tmp.write(rendered.encode("utf-8"))
             tmp.flush()
             driver.get(f"file://{tmp.name}")
             png = driver.get_screenshot_as_png()
             # Find the element you want a screenshot of
             element = driver.find_element(By.CSS_SELECTOR, tag)
-            pixel_ratio = driver.execute_script(
-                "return window.devicePixelRatio"
-            )
+            pixel_ratio = driver.execute_script("return window.devicePixelRatio")
             # Get the element's location and size
             location = element.location
             size = element.size
 
-            if (
-                size['width'] > selenium_width
-                or size['height'] > selenium_height
-            ):
+            if size["width"] > selenium_width or size["height"] > selenium_height:
                 # if our window is too small, resize it with some padding and try again
                 return typer_convert_png(
                     directive,
                     rendered,
                     png_path,
-                    size['width'] + 100,
-                    size['height'] + 100,
+                    size["width"] + 100,
+                    size["height"] + 100,
                 )
 
             # Open the screenshot and crop it to the element
             im = Image.open(BytesIO(png))
-            left = location['x'] * pixel_ratio
-            top = location['y'] * pixel_ratio
+            left = location["x"] * pixel_ratio
+            top = location["y"] * pixel_ratio
             if directive.target is RenderTarget.TEXT:
                 # getting the width of the text is actually a bit tricky
                 script = """
                     const pre = arguments[0];
                     const textContent = pre.textContent || pre.innerText;
                     const temporarySpan = document.createElement('span');
                     document.body.appendChild(temporarySpan);
@@ -910,23 +876,23 @@
                     temporarySpan.textContent = textContent;
 
                     return temporarySpan.offsetWidth;
                 """
                 width = driver.execute_script(script, element)
                 right = left + width * pixel_ratio
             else:
-                right = left + size['width'] * pixel_ratio
-            bottom = top + size['height'] * pixel_ratio
+                right = left + size["width"] * pixel_ratio
+            bottom = top + size["height"] * pixel_ratio
             im = im.crop((left, top, right, bottom))  # Defines crop points
             im.save(str(png_path))  # Saves the screenshot
 
 
 def setup(app: application.Sphinx) -> t.Dict[str, t.Any]:
     # Need autodoc to support mocking modules
-    app.add_directive('typer', TyperDirective)
+    app.add_directive("typer", TyperDirective)
 
     def get_default_render_html(_):
         return typer_render_html
 
     def get_default_get_iframe_height(_):
         return typer_get_iframe_height
 
@@ -935,27 +901,25 @@
 
     def get_default_convert_png(_):
         return typer_convert_png
 
     def get_default_web_driver(_):
         return typer_get_web_driver
 
-    app.add_config_value('typer_render_html', get_default_render_html, 'env')
+    app.add_config_value("typer_render_html", get_default_render_html, "")
 
+    app.add_config_value("typer_get_iframe_height", get_default_get_iframe_height, "")
+    app.add_config_value("typer_svg2pdf", get_default_svg2pdf, "")
+    app.add_config_value("typer_iframe_height_padding", 30, "env")
     app.add_config_value(
-        'typer_get_iframe_height', get_default_get_iframe_height, 'env'
-    )
-    app.add_config_value('typer_svg2pdf', get_default_svg2pdf, 'env')
-    app.add_config_value('typer_iframe_height_padding', 30, 'env')
-    app.add_config_value(
-        'typer_iframe_height_cache_path',
-        Path(app.confdir) / 'typer_cache.json',
-        'env',
+        "typer_iframe_height_cache_path",
+        Path(app.confdir) / "typer_cache.json",
+        "env",
     )
 
-    app.add_config_value('typer_convert_png', get_default_convert_png, 'env')
-    app.add_config_value('typer_get_web_driver', get_default_web_driver, 'env')
+    app.add_config_value("typer_convert_png", get_default_convert_png, "")
+    app.add_config_value("typer_get_web_driver", get_default_web_driver, "")
 
     return {
-        'parallel_read_safe': True,
-        'parallel_write_safe': True,
+        "parallel_read_safe": True,
+        "parallel_write_safe": True,
     }
```

### Comparing `sphinxcontrib_typer-0.2.1/PKG-INFO` & `sphinxcontrib_typer-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-typer
-Version: 0.2.1
+Version: 0.2.2
 Summary: Auto generate docs for typer commands.
 Home-page: https://sphinxcontrib-typer.readthedocs.io
 License: MIT
 Author: Brian Kohan
 Author-email: bckohan@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Provides-Extra: html
 Provides-Extra: pdf
 Provides-Extra: png
 Requires-Dist: cairosvg (>=2.4.0,<3.0.0) ; extra == "pdf"
 Requires-Dist: lxml (>=4.2.0,<6.0.0) ; extra == "pdf"
 Requires-Dist: pillow (>=8.0.0) ; extra == "png"
+Requires-Dist: ruff (>=0.4.4,<0.5.0)
 Requires-Dist: selenium (>=4.0.0,<5.0.0) ; extra == "html" or extra == "png"
 Requires-Dist: sphinx (>=4.0.0)
 Requires-Dist: typer-slim[standard] (>=0.12.0,<1.0.0)
 Requires-Dist: webdriver-manager (>=3.0.0,<5.0.0) ; extra == "html" or extra == "png"
 Project-URL: Repository, https://github.com/sphinx-contrib/typer
 Description-Content-Type: text/markdown
```

