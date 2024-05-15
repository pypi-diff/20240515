# Comparing `tmp/screenpy_playwright-0.0.3.tar.gz` & `tmp/screenpy_playwright-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screenpy_playwright-0.0.3.tar", max compression
+gzip compressed data, was "screenpy_playwright-0.0.4.tar", max compression
```

## Comparing `screenpy_playwright-0.0.3.tar` & `screenpy_playwright-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,30 @@
--rw-r--r--   0        0        0     1071 2024-02-21 15:58:55.512826 screenpy_playwright-0.0.3/LICENSE
--rw-r--r--   0        0        0     3480 2024-02-21 15:58:55.516826 screenpy_playwright-0.0.3/README.md
--rw-r--r--   0        0        0     6199 2024-02-21 15:58:55.516826 screenpy_playwright-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      754 2024-02-21 15:58:55.516826 screenpy_playwright-0.0.3/screenpy_playwright/__init__.py
--rw-r--r--   0        0        0      938 2024-02-21 15:58:55.516826 screenpy_playwright-0.0.3/screenpy_playwright/__version__.py
--rw-r--r--   0        0        0      189 2024-02-21 15:58:55.516826 screenpy_playwright-0.0.3/screenpy_playwright/abilities/__init__.py
--rw-r--r--   0        0        0     2760 2024-02-21 15:58:55.516826 screenpy_playwright-0.0.3/screenpy_playwright/abilities/browse_the_web_synchronously.py
--rw-r--r--   0        0        0      329 2024-02-21 15:58:55.516826 screenpy_playwright-0.0.3/screenpy_playwright/actions/__init__.py
--rw-r--r--   0        0        0      892 2024-02-21 15:58:55.516826 screenpy_playwright-0.0.3/screenpy_playwright/actions/click.py
--rw-r--r--   0        0        0     2603 2024-02-21 15:58:55.516826 screenpy_playwright-0.0.3/screenpy_playwright/actions/enter.py
--rw-r--r--   0        0        0     1638 2024-02-21 15:58:55.516826 screenpy_playwright-0.0.3/screenpy_playwright/actions/open.py
--rw-r--r--   0        0        0     3307 2024-02-21 15:58:55.516826 screenpy_playwright-0.0.3/screenpy_playwright/actions/save_screenshot.py
--rw-r--r--   0        0        0      186 2024-02-21 15:58:55.516826 screenpy_playwright-0.0.3/screenpy_playwright/exceptions.py
--rw-r--r--   0        0        0      165 2024-02-21 15:58:55.516826 screenpy_playwright-0.0.3/screenpy_playwright/protocols.py
--rw-r--r--   0        0        0       39 2024-02-21 15:58:55.516826 screenpy_playwright-0.0.3/screenpy_playwright/py.typed
--rw-r--r--   0        0        0      221 2024-02-21 15:58:55.516826 screenpy_playwright-0.0.3/screenpy_playwright/questions/__init__.py
--rw-r--r--   0        0        0     1868 2024-02-21 15:58:55.516826 screenpy_playwright-0.0.3/screenpy_playwright/questions/attribute.py
--rw-r--r--   0        0        0     1259 2024-02-21 15:58:55.516826 screenpy_playwright-0.0.3/screenpy_playwright/questions/number.py
--rw-r--r--   0        0        0     1297 2024-02-21 15:58:55.516826 screenpy_playwright-0.0.3/screenpy_playwright/questions/text.py
--rw-r--r--   0        0        0     3033 2024-02-21 15:58:55.516826 screenpy_playwright-0.0.3/screenpy_playwright/target.py
--rw-r--r--   0        0        0     5530 1970-01-01 00:00:00.000000 screenpy_playwright-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-15 19:35:56.065664 screenpy_playwright-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3480 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/README.md
+-rw-r--r--   0        0        0     6199 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      877 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/__init__.py
+-rw-r--r--   0        0        0      938 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/__version__.py
+-rw-r--r--   0        0        0      189 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/abilities/__init__.py
+-rw-r--r--   0        0        0     2706 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/abilities/browse_the_web_synchronously.py
+-rw-r--r--   0        0        0      898 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/actions/__init__.py
+-rw-r--r--   0        0        0     2008 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/actions/click.py
+-rw-r--r--   0        0        0     2914 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/actions/enter.py
+-rw-r--r--   0        0        0     2123 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/actions/open.py
+-rw-r--r--   0        0        0     1352 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/actions/refresh_the_page.py
+-rw-r--r--   0        0        0     3205 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/actions/save_screenshot.py
+-rw-r--r--   0        0        0     3250 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/actions/scroll.py
+-rw-r--r--   0        0        0     3368 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/actions/select.py
+-rw-r--r--   0        0        0      274 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/exceptions.py
+-rw-r--r--   0        0        0      165 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/protocols.py
+-rw-r--r--   0        0        0       39 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/py.typed
+-rw-r--r--   0        0        0      554 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/questions/__init__.py
+-rw-r--r--   0        0        0     1870 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/questions/attribute.py
+-rw-r--r--   0        0        0     1369 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/questions/browser_url.py
+-rw-r--r--   0        0        0      709 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/questions/element.py
+-rw-r--r--   0        0        0     1259 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/questions/number.py
+-rw-r--r--   0        0        0     1297 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/questions/text.py
+-rw-r--r--   0        0        0      199 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/resolutions/__init__.py
+-rw-r--r--   0        0        0      146 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/resolutions/custom_matchers/__init__.py
+-rw-r--r--   0        0        0     1466 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/resolutions/custom_matchers/is_visible_element.py
+-rw-r--r--   0        0        0      714 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/resolutions/is_visible.py
+-rw-r--r--   0        0        0     6191 2024-05-15 19:35:56.073664 screenpy_playwright-0.0.4/screenpy_playwright/target.py
+-rw-r--r--   0        0        0     5530 1970-01-01 00:00:00.000000 screenpy_playwright-0.0.4/PKG-INFO
```

### Comparing `screenpy_playwright-0.0.3/LICENSE` & `screenpy_playwright-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `screenpy_playwright-0.0.3/README.md` & `screenpy_playwright-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `screenpy_playwright-0.0.3/pyproject.toml` & `screenpy_playwright-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 
 ################################################################################
 #                 END OF BOILERPLATE ScreenPyHQ CONFIGURATIONS                 #
 ################################################################################
 
 [tool.poetry]
 name = "screenpy_playwright"
-version = "0.0.3"
+version = "0.0.4"
 description = "ScreenPy extension to enable interacting with Playwright."
 authors = ["Perry Goy <perry.goy@gmail.com>"]
 maintainers = ["Marcel Wilson"]
 license = "MIT"
 repository = "https://github.com/ScreenPyHQ/screenpy_playwright"
 documentation = "https://screenpy-playwright-docs.readthedocs.io"
 readme = "README.md"
```

### Comparing `screenpy_playwright-0.0.3/screenpy_playwright/__init__.py` & `screenpy_playwright-0.0.4/screenpy_playwright/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,18 +8,24 @@
 ScreenPy Playwright is an extension for ScreenPy which enables Actors to use
 the Playwright browser automation tool.
 
 :copyright: (c) 2019-2024 by Perry Goy.
 :license: MIT, see LICENSE for more details.
 """
 
-from . import abilities, actions, questions
+from . import abilities, actions, questions, resolutions
 from .abilities import *  # noqa: F403
 from .actions import *  # noqa: F403
-from .exceptions import TargetingError
+from .exceptions import NoPageError, TargetingError
 from .protocols import PageObject
 from .questions import *  # noqa: F403
+from .resolutions import *  # noqa: F403
 from .target import Target
 
-__all__ = ["Target", "TargetingError", "PageObject"]
+__all__ = [
+    "NoPageError",
+    "PageObject",
+    "Target",
+    "TargetingError",
+]
 
-__all__ += abilities.__all__ + actions.__all__ + questions.__all__
+__all__ += abilities.__all__ + actions.__all__ + questions.__all__ + resolutions.__all__
```

### Comparing `screenpy_playwright-0.0.3/screenpy_playwright/__version__.py` & `screenpy_playwright-0.0.4/screenpy_playwright/__version__.py`

 * *Files identical despite different names*

### Comparing `screenpy_playwright-0.0.3/screenpy_playwright/abilities/browse_the_web_synchronously.py` & `screenpy_playwright-0.0.4/screenpy_playwright/abilities/browse_the_web_synchronously.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,22 +2,19 @@
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from playwright.sync_api import sync_playwright
 
-if TYPE_CHECKING:
-    from typing import TypeVar
+from ..exceptions import NoPageError
 
+if TYPE_CHECKING:
     from playwright.sync_api import Browser, BrowserContext, Page, Playwright
-
-    SelfBrowseTheWebSynchronously = TypeVar(
-        "SelfBrowseTheWebSynchronously", bound="BrowseTheWebSynchronously"
-    )
+    from typing_extensions import Self
 
 
 class BrowseTheWebSynchronously:
     """Use a synchronous Playwright instance to browse the web.
 
     Examples::
 
@@ -29,61 +26,62 @@
 
         the_actor.can(
             BrowseTheWebSynchronously.using(playwright, cust_browser)
         )
     """
 
     playwright: Playwright | None = None
-    current_page: Page | None
+    _current_page: Page | None
     pages: list[Page]
 
     @classmethod
-    def using(
-        cls: type[SelfBrowseTheWebSynchronously],
-        playwright: Playwright,
-        browser: Browser | BrowserContext,
-    ) -> SelfBrowseTheWebSynchronously:
+    def using(cls, playwright: Playwright, browser: Browser | BrowserContext) -> Self:
         """Supply a pre-defined Playwright browser to use."""
         cls.playwright = playwright
         return cls(browser)
 
     @classmethod
-    def using_firefox(
-        cls: type[SelfBrowseTheWebSynchronously],
-    ) -> SelfBrowseTheWebSynchronously:
+    def using_firefox(cls) -> Self:
         """Use a synchronous Firefox browser."""
         if cls.playwright is None:
             cls.playwright = sync_playwright().start()
         return cls(cls.playwright.firefox.launch())
 
     @classmethod
-    def using_chromium(
-        cls: type[SelfBrowseTheWebSynchronously],
-    ) -> SelfBrowseTheWebSynchronously:
+    def using_chromium(cls) -> Self:
         """Use a synchronous Chromium (i.e. Chrome, Edge, Opera, etc.) browser."""
         if cls.playwright is None:
             cls.playwright = sync_playwright().start()
         return cls(cls.playwright.chromium.launch())
 
     @classmethod
-    def using_webkit(
-        cls: type[SelfBrowseTheWebSynchronously],
-    ) -> BrowseTheWebSynchronously:
+    def using_webkit(cls) -> Self:
         """Use a synchronous WebKit (i.e. Safari, etc.) browser."""
         if cls.playwright is None:
             cls.playwright = sync_playwright().start()
         return cls(cls.playwright.webkit.launch())
 
-    def forget(self: SelfBrowseTheWebSynchronously) -> None:
+    @property
+    def current_page(self) -> Page:
+        """Get the current page.
+
+        Raises a :class:`~screenpy_playwright.exceptions.NoPageError` if there
+        is no current page.
+        """
+        if self._current_page is None:
+            msg = "There is no current page. Did you forget to `Open` a page?"
+            raise NoPageError(msg)
+        return self._current_page
+
+    @current_page.setter
+    def current_page(self, page: Page) -> None:
+        """Set the current page."""
+        self._current_page = page
+
+    def forget(self) -> None:
         """Forget everything you knew about being a playwright."""
         self.browser.close()
-        if self.playwright:
-            self.playwright.stop()
-        self.__class__.playwright = None
-
-    def __init__(
-        self: SelfBrowseTheWebSynchronously,
-        browser: Browser | BrowserContext,
-    ) -> None:
+
+    def __init__(self, browser: Browser | BrowserContext) -> None:
         self.browser = browser
-        self.current_page = None
+        self._current_page = None
         self.pages = []
```

### Comparing `screenpy_playwright-0.0.3/screenpy_playwright/actions/click.py` & `screenpy_playwright-0.0.4/screenpy_playwright/questions/number.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,53 @@
-"""Click on an element."""
+"""Ask about the number of an element."""
+
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
 
-from screenpy import Actor
 from screenpy.pacing import beat
 
-from ..target import Target
+if TYPE_CHECKING:
+    from screenpy import Actor
 
+    from ..target import Target
 
-class Click:
-    """Click on an element!
 
-    Abilities Required:
-        :class:`~screenpy_playwright.abilities.BrowseTheWebSynchronously`
+class Number:
+    """Ask how many of an element are on the page.
 
     Examples::
 
-        the_actor.attempts_to(Click.on_the(LOG_IN_BUTTON))
+        the_actor.should(See.the(Number.of(CONFETTI), IsEqualTo(10)))
     """
 
     @staticmethod
-    def on_the(target: Target) -> "Click":
-        """Specify the element on which to click."""
-        return Click(target)
+    def of(target: Target) -> Number:
+        """Supply the Target to count.
+
+        Args:
+            target: the Target which describes the element to count.
+
+        Returns:
+            A new Number instance.
+        """
+        return Number(target)
 
     def describe(self) -> str:
-        """Describe the Action in present tense."""
-        return f"Click on the {self.target}."
+        """Describe the Question in the present tense.
 
-    @beat("{} clicks on the {target}.")
-    def perform_as(self, the_actor: Actor) -> None:
-        """Direct the Actor to click on the element."""
-        self.target.found_by(the_actor).click()
+        Returns:
+            A description of this Question.
+        """
+        return f"The number of {self.target}."
+
+    @beat("{} examines the Number of the {target}.")
+    def answered_by(self, the_actor: Actor) -> int:
+        """Direct the Actor to read the Number from the target.
+
+        Returns:
+            The number of elements the Actor found.
+        """
+        return self.target.found_by(the_actor).count()
 
     def __init__(self, target: Target) -> None:
         self.target = target
```

### Comparing `screenpy_playwright-0.0.3/screenpy_playwright/actions/enter.py` & `screenpy_playwright-0.0.4/screenpy_playwright/actions/enter.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,99 +1,99 @@
 """Enter text into an input field."""
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, TypedDict
 
 from screenpy.exceptions import UnableToAct
 from screenpy.pacing import beat
 
 if TYPE_CHECKING:
     from screenpy import Actor
+    from typing_extensions import NotRequired, Self, Unpack
 
     from ..target import Target
 
+    class EnterTypes(TypedDict):
+        """Types that can be passed to Playwright's ElementHandle.fill method."""
+
+        timeout: NotRequired[float | None]
+        no_wait_after: NotRequired[bool | None]
+        force: NotRequired[bool | None]
+
 
 class Enter:
     """Enter text into an input field.
 
     Abilities Required:
         :class:`~screenpy_playwright.abilities.BrowseTheWebSynchronously`
 
     Examples::
 
         the_actor.attempts_to(Enter("Hello!").into_the(GREETING_INPUT))
 
+        the_actor.attempts_to(Enter("Hello!", force=True).into_the(GREETING_INPUT))
+
         the_actor.attempts_to(Enter.the_text("eggs").into_the(GROCERY_FIELD))
 
         the_actor.attempts_to(Enter.the_secret("12345").into_the(PASSWORD_FIELD))
     """
 
     target: Target | None
 
-    @staticmethod
-    def the_text(text: str) -> Enter:
-        """Provide the text to enter into the field.
-
-        Args:
-            text: the text to enter into the field.
-
-        Returns:
-            A new instance of Enter, with mask et to False.
-        """
-        return Enter(text)
-
-    @staticmethod
-    def the_secret(text: str) -> Enter:
-        """Provide the SECRET text to enter into the field.
+    @classmethod
+    def the_text(cls, text: str, **kwargs: Unpack[EnterTypes]) -> Self:
+        """Provide the text to enter into the field."""
+        return cls(text, **kwargs)
+
+    @classmethod
+    def the_secret(cls, text: str, **kwargs: Unpack[EnterTypes]) -> Self:
+        """Provide the **secret** text to enter into the field.
 
-        The text will be masked, and appear as "[CENSORED]".
+        The text will be masked, and appear as "[CENSORED]" in logs.
 
-        Returns:
-            A new instance of Enter, with mask set to True.
+        Aliases:
+            - ``the_password``
         """
-        return Enter(text, mask=True)
+        return cls(text, mask=True, **kwargs)
 
     the_password = the_secret
 
-    def into_the(self, target: Target) -> Enter:
+    def into_the(self, target: Target, **kwargs: Unpack[EnterTypes]) -> Enter:
         """Target the element to enter text into.
 
-        Args:
-            target: the Target which describes the element to enter text into.
-
-        Returns:
-            self
+        Aliases:
+            - ``into``
         """
         self.target = target
+        self.kwargs.update(kwargs)
         return self
 
     into = into_the
 
     def describe(self) -> str:
-        """Describe the Action in present tense.
-
-        Returns:
-            A description of this Action.
-        """
+        """Describe the Action in present tense."""
         return f'Enter "{self.text_to_log}" into the {self.target}.'
 
     @beat('{} enters "{text_to_log}" into the {target}.')
     def perform_as(self, the_actor: Actor) -> None:
         """Direct the Actor to enter text into the Target."""
         if self.target is None:
             msg = (
                 "Target was not supplied for Enter. Provide a Target by using either "
                 "the .into(), .into_the(), or into_the_first_of_the() method."
             )
             raise UnableToAct(msg)
 
-        self.target.found_by(the_actor).fill(self.text)
+        self.target.found_by(the_actor).fill(self.text, **self.kwargs)
 
-    def __init__(self, text: str, *, mask: bool = False) -> None:
+    def __init__(
+        self, text: str, *, mask: bool = False, **kwargs: Unpack[EnterTypes]
+    ) -> None:
         self.text = text
         self.target = None
+        self.kwargs = kwargs
 
         if mask:
             self.text_to_log = "[CENSORED]"
         else:
             self.text_to_log = text
```

### Comparing `screenpy_playwright-0.0.3/screenpy_playwright/actions/open.py` & `screenpy_playwright-0.0.4/screenpy_playwright/actions/open.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 """Open a URL using the Actor's browser."""
 
 from __future__ import annotations
 
 import os
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, TypedDict
 
 from screenpy.pacing import beat
 
 from ..abilities import BrowseTheWebSynchronously
 
 if TYPE_CHECKING:
     from screenpy import Actor
+    from typing_extensions import Literal, NotRequired, Unpack
 
     from ..protocols import PageObject
 
+    class OpenTypes(TypedDict):
+        """Types that can be passed to Playwright's Page.goto method."""
+
+        timeout: NotRequired[float | None]
+        wait_until: NotRequired[
+            Literal["commit", "domcontentloaded", "load", "networkidle"] | None
+        ]
+        referer: NotRequired[str | None]
+
 
 class Open:
     """Go to a specific URL!
 
     This Action supports using the BASE_URL environment variable to
     set a base URL. If you set BASE_URL, the url passed in to this
     Action will be appended to the end of it. For example, if you
@@ -31,24 +41,28 @@
         :class:`~screenpy_playwright.abilities.BrowseTheWebSynchronously`
 
     Examples::
 
         the_actor.attempts_to(Open("https://www.nintendo.com/"))
     """
 
+    kwargs: OpenTypes
+
     def describe(self) -> str:
         """Describe the Action in present tense."""
         return f"Visit {self.url}"
 
     @beat("{} visits {url}")
     def perform_as(self, the_actor: Actor) -> None:
         """Direct the actor to Open a webpage."""
         browse_the_web = the_actor.ability_to(BrowseTheWebSynchronously)
         page = browse_the_web.browser.new_page()
-        page.goto(self.url)
+        page.goto(self.url, **self.kwargs)
         browse_the_web.current_page = page
         browse_the_web.pages.append(page)
 
-    def __init__(self, location: str | PageObject) -> None:
+    def __init__(self, location: str | PageObject, **kwargs: Unpack[OpenTypes]) -> None:
         url = getattr(location, "url", location)
         url = f'{os.getenv("BASE_URL", "")}{url}'
+
         self.url = url
+        self.kwargs = kwargs
```

### Comparing `screenpy_playwright-0.0.3/screenpy_playwright/actions/save_screenshot.py` & `screenpy_playwright-0.0.4/screenpy_playwright/actions/save_screenshot.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,44 +57,37 @@
         """Supply the name and/or filepath for the screenshot.
 
         If only a name is supplied, the screenshot will appear in the current
         working directory.
 
         Args:
             path: The filepath for the screenshot, including its name.
-
-        Returns:
-            Self
         """
         return cls(path=path)
 
     def and_attach_it(self, **kwargs: Any) -> Self:  # noqa: ANN401
         """Indicate the screenshot should be attached to any reports.
 
         This method accepts any additional keywords needed by any adapters
         attached for :external+screenpy:ref:`Narration`.
 
+        Aliases:
+            - ``and_attach_it_with``
+
         Args:
             kwargs: keyword arguments for the adapters used by the narrator.
-
-        Returns:
-            Self
         """
         self.attach_kwargs = kwargs
         return self
 
     and_attach_it_with = and_attach_it
 
     @beat("{} saves a screenshot as {filename}")
     def perform_as(self, the_actor: Actor) -> None:
-        """Direct the actor to save a screenshot.
-
-        Args:
-            the_actor: The actor who will perform this Action.
-        """
+        """Direct the actor to save a screenshot."""
         current_page = the_actor.ability_to(BrowseTheWebSynchronously).current_page
         if current_page is None:
             msg = "No page has been opened! Cannot save a screenshot."
             raise UnableToAct(msg)
 
         screenshot = current_page.screenshot(path=self.path)
         Path(self.path).write_bytes(screenshot)
```

### Comparing `screenpy_playwright-0.0.3/screenpy_playwright/questions/attribute.py` & `screenpy_playwright-0.0.4/screenpy_playwright/questions/attribute.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 
 class Attribute:
     """Ask about the value of an HTML attribute on a Target.
 
     Abilities Required:
         :class:`~screenpy_playwright.abilities.BrowseTheWebSynchronously`
 
-    Examples:
+    Examples::
+
         the_actor.should(
             See.the(
                 Attribute("aria-label").of_the(LOGIN_LINK),
                 ContainsTheText("Log in to the application.")
             )
         )
```

### Comparing `screenpy_playwright-0.0.3/screenpy_playwright/questions/number.py` & `screenpy_playwright-0.0.4/screenpy_playwright/questions/text.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,55 @@
-"""Ask about the number of an element."""
+"""Ask about the text in an element."""
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from screenpy.pacing import beat
 
 if TYPE_CHECKING:
     from screenpy import Actor
 
     from ..target import Target
 
 
-class Number:
-    """Ask how many of an element are on the page.
+class Text:
+    """Ask for the text from a Target.
 
     Examples::
 
-        the_actor.should(See.the(Number.of(CONFETTI), IsEqualTo(10)))
+        the_actor.should(
+            See.the(Text.of_the(WELCOME_BANNER), ReadsExactly("Welcome!"))
+        )
     """
 
     @staticmethod
-    def of(target: Target) -> Number:
-        """Supply the Target to count.
+    def of_the(target: Target) -> Text:
+        """Supply the Target whose text to read.
 
         Args:
-            target: the Target which describes the element to count.
+            target: the Target which describes the Element to read.
 
         Returns:
-            A new Number instance.
+            A new instance of Text.
         """
-        return Number(target)
+        return Text(target)
 
     def describe(self) -> str:
         """Describe the Question in the present tense.
 
         Returns:
             A description of this Question.
         """
-        return f"The number of {self.target}."
+        return f"The text from the {self.target}."
 
-    @beat("{} examines the Number of the {target}.")
-    def answered_by(self, the_actor: Actor) -> int:
-        """Direct the Actor to read the Number from the target.
+    @beat("{} examines the text of the {target}.")
+    def answered_by(self, the_actor: Actor) -> str | None:
+        """Direct the Actor to read the text from the target.
 
         Returns:
-            The number of elements the Actor found.
+            The text found by the Actor.
         """
-        return self.target.found_by(the_actor).count()
+        return self.target.found_by(the_actor).text_content()
 
     def __init__(self, target: Target) -> None:
         self.target = target
```

### Comparing `screenpy_playwright-0.0.3/PKG-INFO` & `screenpy_playwright-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screenpy_playwright
-Version: 0.0.3
+Version: 0.0.4
 Summary: ScreenPy extension to enable interacting with Playwright.
 Home-page: https://github.com/ScreenPyHQ/screenpy_playwright
 License: MIT
 Author: Perry Goy
 Author-email: perry.goy@gmail.com
 Maintainer: Marcel Wilson
 Requires-Python: >=3.8,<4.0
```

