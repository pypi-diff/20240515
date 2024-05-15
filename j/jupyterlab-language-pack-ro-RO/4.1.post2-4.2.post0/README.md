# Comparing `tmp/jupyterlab_language_pack_ro_ro-4.1.post2.tar.gz` & `tmp/jupyterlab_language_pack_ro_ro-4.2.post0.tar.gz`

## Comparing `jupyterlab_language_pack_ro_ro-4.1.post2.tar` & `jupyterlab_language_pack_ro_ro-4.2.post0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.1.post2/.copier-answers.yml
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.1.post2/CONTRIBUTORS.md
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.1.post2/jupyterlab_language_pack_ro_RO/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.1.post2/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/.gitkeep
--rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.1.post2/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/dask_labextension.po
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.1.post2/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyter_archive.po
--rw-r--r--   0        0        0     3869 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.1.post2/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyter_collaboration.po
--rw-r--r--   0        0        0     9242 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.1.post2/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyter_resource_usage.po
--rw-r--r--   0        0        0   236809 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.1.post2/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyterlab.po
--rw-r--r--   0        0        0   119122 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.1.post2/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyterlab_git.po
--rw-r--r--   0        0        0    53462 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.1.post2/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyterlab_lsp.po
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.1.post2/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyterlab_recents.po
--rw-r--r--   0        0        0     4787 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.1.post2/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyterlab_search_replace.po
--rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.1.post2/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyterlab_spreadsheet_editor.po
--rw-r--r--   0        0        0    11873 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.1.post2/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyterlab_tour.po
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.1.post2/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyterlab_widgets.po
--rw-r--r--   0        0        0     6871 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.1.post2/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupytext.po
--rw-r--r--   0        0        0     5521 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.1.post2/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/nbdime.po
--rw-r--r--   0        0        0    11093 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.1.post2/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/notebook.po
--rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.1.post2/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/retrolab.po
--rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.1.post2/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/spellchecker.po
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.1.post2/.gitignore
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.1.post2/LICENSE.txt
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.1.post2/README.md
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.1.post2/pyproject.toml
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.1.post2/PKG-INFO
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.2.post0/.copier-answers.yml
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.2.post0/CONTRIBUTORS.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.2.post0/jupyterlab_language_pack_ro_RO/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.2.post0/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/.gitkeep
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.2.post0/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/dask_labextension.po
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.2.post0/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyter_archive.po
+-rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.2.post0/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyter_collaboration.po
+-rw-r--r--   0        0        0     9242 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.2.post0/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyter_resource_usage.po
+-rw-r--r--   0        0        0   274631 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.2.post0/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyterlab.po
+-rw-r--r--   0        0        0   134653 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.2.post0/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyterlab_git.po
+-rw-r--r--   0        0        0    53462 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.2.post0/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyterlab_lsp.po
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.2.post0/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyterlab_recents.po
+-rw-r--r--   0        0        0     4787 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.2.post0/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyterlab_search_replace.po
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.2.post0/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyterlab_spreadsheet_editor.po
+-rw-r--r--   0        0        0    11987 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.2.post0/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyterlab_tour.po
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.2.post0/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyterlab_widgets.po
+-rw-r--r--   0        0        0     6871 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.2.post0/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupytext.po
+-rw-r--r--   0        0        0     5521 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.2.post0/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/nbdime.po
+-rw-r--r--   0        0        0    11093 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.2.post0/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/notebook.po
+-rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.2.post0/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/retrolab.po
+-rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.2.post0/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/spellchecker.po
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.2.post0/.gitignore
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.2.post0/LICENSE.txt
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.2.post0/README.md
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.2.post0/pyproject.toml
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ro_ro-4.2.post0/PKG-INFO
```

### Comparing `jupyterlab_language_pack_ro_ro-4.1.post2/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/dask_labextension.po` & `jupyterlab_language_pack_ro_ro-4.2.post0/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/dask_labextension.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ro_ro-4.1.post2/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyter_archive.po` & `jupyterlab_language_pack_ro_ro-4.2.post0/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyter_archive.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ro_ro-4.1.post2/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyter_collaboration.po` & `jupyterlab_language_pack_ro_ro-4.2.post0/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyter_collaboration.po`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 "X-Crowdin-Project: jupyterlab\n"
 "X-Crowdin-Project-ID: 409874\n"
 "X-Crowdin-Language: ro\n"
 "X-Crowdin-File: /main/extensions/jupyter_collaboration/locale/jupyter_collaboration.pot\n"
 "X-Crowdin-File-ID: 229\n"
 "Language-Team: Romanian\n"
 "Language: ro_RO\n"
-"PO-Revision-Date: 2023-07-04 11:34\n"
+"PO-Revision-Date: 2024-03-29 11:19\n"
 
 #: /packages/collaboration-extension/schema/shared-link.json:/description
 msgctxt "schema"
 msgid "Shared link settings"
 msgstr ""
 
 #: /packages/collaboration-extension/schema/shared-link.json:/title
@@ -30,27 +30,27 @@
 msgstr ""
 
 #: /packages/collaboration-extension/schema/user-menu-bar.json:/title
 msgctxt "schema"
 msgid "User Menu Bar"
 msgstr ""
 
-#: packages/collaboration-extension/src/collaboration.ts:144 packages/collaboration-extension/src/collaboration.ts:151
+#: packages/collaboration-extension/src/collaboration.ts:144 packages/collaboration-extension/src/collaboration.ts:148 packages/collaboration-extension/src/collaboration.ts:151
 msgid "Collaboration"
 msgstr ""
 
-#: packages/collaboration-extension/src/collaboration.ts:149 packages/collaboration-extension/src/collaboration.ts:156
+#: packages/collaboration-extension/src/collaboration.ts:149 packages/collaboration-extension/src/collaboration.ts:153 packages/collaboration-extension/src/collaboration.ts:156
 msgid "User info"
 msgstr ""
 
-#: packages/collaboration-extension/src/collaboration.ts:150 packages/collaboration-extension/src/collaboration.ts:157
+#: packages/collaboration-extension/src/collaboration.ts:150 packages/collaboration-extension/src/collaboration.ts:154 packages/collaboration-extension/src/collaboration.ts:157
 msgid "User information"
 msgstr ""
 
-#: packages/collaboration-extension/src/collaboration.ts:162 packages/collaboration-extension/src/collaboration.ts:169
+#: packages/collaboration-extension/src/collaboration.ts:162 packages/collaboration-extension/src/collaboration.ts:166 packages/collaboration-extension/src/collaboration.ts:169
 msgid "Online Collaborators"
 msgstr ""
 
 #: packages/collaboration-extension/src/filebrowser.ts:199 packages/collaboration-extension/src/filebrowser.ts:248
 msgid "Warning"
 msgstr ""
 
@@ -116,11 +116,19 @@
 msgid "Copy Link"
 msgstr ""
 
 #: packages/collaboration/src/sharedlink.ts:60
 msgid "Copy the link to the Jupyter Server"
 msgstr ""
 
-#: packages/docprovider/src/yprovider.ts:124
+#: packages/docprovider/src/yprovider.ts:124 packages/docprovider/src/yprovider.ts:139
 msgid "Document session error"
 msgstr ""
 
+#: packages/docprovider/src/yprovider.ts:174
+msgid "File changed"
+msgstr ""
+
+#: packages/docprovider/src/yprovider.ts:175
+msgid "Do you want to overwrite the file or reload it?"
+msgstr ""
+
```

### Comparing `jupyterlab_language_pack_ro_ro-4.1.post2/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyter_resource_usage.po` & `jupyterlab_language_pack_ro_ro-4.2.post0/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyter_resource_usage.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ro_ro-4.1.post2/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyterlab.po` & `jupyterlab_language_pack_ro_ro-4.2.post0/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyterlab.po`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 "X-Crowdin-Project: jupyterlab\n"
 "X-Crowdin-Project-ID: 409874\n"
 "X-Crowdin-Language: ro\n"
 "X-Crowdin-File: /main/jupyterlab/locale/jupyterlab.pot\n"
 "X-Crowdin-File-ID: 191\n"
 "Language-Team: Romanian\n"
 "Language: ro_RO\n"
-"PO-Revision-Date: 2023-12-29 22:41\n"
+"PO-Revision-Date: 2024-05-06 08:14\n"
 
 #: /examples/federated/md_package/schema/plugin.json:/description /packages/markdownviewer-extension/schema/plugin.json:/description
 msgctxt "schema"
 msgid "Markdown viewer settings."
 msgstr ""
 
 #: /examples/federated/md_package/schema/plugin.json:/jupyter.lab.setting-icon-label /packages/markdownviewer-extension/schema/plugin.json:/jupyter.lab.setting-icon-label
@@ -92,14 +92,22 @@
 msgstr ""
 
 #: /examples/federated/md_package/schema/plugin.json:/title /packages/markdownviewer-extension/schema/plugin.json:/title
 msgctxt "schema"
 msgid "Markdown Viewer"
 msgstr ""
 
+#: /jupyterlab/extensions/manager.py:261
+msgid "The following plugins cannot be disabled as they are locked: "
+msgstr ""
+
+#: /jupyterlab/extensions/manager.py:287
+msgid "The following plugins cannot be enabled as they are locked: "
+msgstr ""
+
 #: /jupyterlab/extensions/readonly.py:63
 msgid "Extension installation not supported."
 msgstr ""
 
 #: /jupyterlab/extensions/readonly.py:81
 msgid "Extension removal not supported."
 msgstr ""
@@ -354,19 +362,14 @@
 #: /packages/apputils-extension/schema/notification.json:/description
 msgctxt "schema"
 msgid "Notifications settings."
 msgstr ""
 
 #: /packages/apputils-extension/schema/notification.json:/properties/checkForUpdates/description
 msgctxt "settings"
-msgid "Whether to check for newer version of JupyterLab or not. It requires `fechNews` to be `true` to be active. If `true`, it will make a request to a website."
-msgstr ""
-
-#: /packages/apputils-extension/schema/notification.json:/properties/checkForUpdates/description
-msgctxt "settings"
 msgid "Whether to check for newer version of JupyterLab or not. It requires `fetchNews` to be `true` to be active. If `true`, it will make a request to a website."
 msgstr ""
 
 #: /packages/apputils-extension/schema/notification.json:/properties/checkForUpdates/title
 msgctxt "settings"
 msgid "Check for JupyterLab updates"
 msgstr ""
@@ -482,37 +485,67 @@
 msgstr ""
 
 #: /packages/apputils-extension/schema/themes.json:/jupyter.lab.setting-icon-label
 msgctxt "settings"
 msgid "Theme Manager"
 msgstr ""
 
+#: /packages/apputils-extension/schema/themes.json:/properties/adaptive-theme/description
+msgctxt "settings"
+msgid "Synchronize visual styling theme with system settings"
+msgstr ""
+
+#: /packages/apputils-extension/schema/themes.json:/properties/adaptive-theme/title
+msgctxt "settings"
+msgid "Adaptive Theme"
+msgstr ""
+
 #: /packages/apputils-extension/schema/themes.json:/properties/overrides/description
 msgctxt "settings"
 msgid "Override theme CSS variables by setting key-value pairs here"
 msgstr ""
 
 #: /packages/apputils-extension/schema/themes.json:/properties/overrides/title
 msgctxt "settings"
 msgid "Theme CSS Overrides"
 msgstr ""
 
+#: /packages/apputils-extension/schema/themes.json:/properties/preferred-dark-theme/description
+msgctxt "settings"
+msgid "Application-level dark visual styling theme. Ignored when Adaptive Theme is disabled."
+msgstr ""
+
+#: /packages/apputils-extension/schema/themes.json:/properties/preferred-dark-theme/title
+msgctxt "settings"
+msgid "Preferred Dark Theme"
+msgstr ""
+
+#: /packages/apputils-extension/schema/themes.json:/properties/preferred-light-theme/description
+msgctxt "settings"
+msgid "Application-level light visual styling theme. Ignored when Adaptive Theme is disabled."
+msgstr ""
+
+#: /packages/apputils-extension/schema/themes.json:/properties/preferred-light-theme/title
+msgctxt "settings"
+msgid "Preferred Light Theme"
+msgstr ""
+
 #: /packages/apputils-extension/schema/themes.json:/properties/theme-scrollbars/description
 msgctxt "settings"
 msgid "Enable/disable styling of the application scrollbars"
 msgstr ""
 
 #: /packages/apputils-extension/schema/themes.json:/properties/theme-scrollbars/title
 msgctxt "settings"
 msgid "Scrollbar Theming"
 msgstr ""
 
 #: /packages/apputils-extension/schema/themes.json:/properties/theme/description
 msgctxt "settings"
-msgid "Application-level visual styling theme"
+msgid "Application-level visual styling theme. Ignored when Adaptive Theme is enabled."
 msgstr ""
 
 #: /packages/apputils-extension/schema/themes.json:/properties/theme/title
 msgctxt "settings"
 msgid "Selected Theme"
 msgstr ""
 
@@ -592,22 +625,97 @@
 msgstr ""
 
 #: /packages/codemirror-extension/schema/plugin.json:/title
 msgctxt "schema"
 msgid "CodeMirror"
 msgstr ""
 
+#: /packages/completer-extension/schema/inline-completer.json:/description
+msgctxt "schema"
+msgid "Inline completer settings."
+msgstr ""
+
+#: /packages/completer-extension/schema/inline-completer.json:/jupyter.lab.setting-icon-label
+msgctxt "settings"
+msgid "Inline Completer"
+msgstr ""
+
+#: /packages/completer-extension/schema/inline-completer.json:/properties/providers/title
+msgctxt "settings"
+msgid "Inline completion providers"
+msgstr ""
+
+#: /packages/completer-extension/schema/inline-completer.json:/properties/showShortcuts/description
+msgctxt "settings"
+msgid "Whether to show shortcuts in the inline completer widget."
+msgstr ""
+
+#: /packages/completer-extension/schema/inline-completer.json:/properties/showShortcuts/title
+msgctxt "settings"
+msgid "Show shortcuts in the widget"
+msgstr ""
+
+#: /packages/completer-extension/schema/inline-completer.json:/properties/showWidget/description
+msgctxt "settings"
+msgid "When to show the inline completer widget."
+msgstr ""
+
+#: /packages/completer-extension/schema/inline-completer.json:/properties/showWidget/oneOf[0]/title
+msgctxt "settings"
+msgid "Always"
+msgstr ""
+
+#: /packages/completer-extension/schema/inline-completer.json:/properties/showWidget/oneOf[1]/title
+msgctxt "settings"
+msgid "On hover"
+msgstr ""
+
+#: /packages/completer-extension/schema/inline-completer.json:/properties/showWidget/oneOf[2]/title
+msgctxt "settings"
+msgid "Never"
+msgstr ""
+
+#: /packages/completer-extension/schema/inline-completer.json:/properties/showWidget/title
+msgctxt "settings"
+msgid "Show widget"
+msgstr ""
+
+#: /packages/completer-extension/schema/inline-completer.json:/properties/streamingAnimation/description
+msgctxt "settings"
+msgid "Transition effect used when streaming tokens from model."
+msgstr ""
+
+#: /packages/completer-extension/schema/inline-completer.json:/properties/streamingAnimation/oneOf[0]/title
+msgctxt "settings"
+msgid "None"
+msgstr ""
+
+#: /packages/completer-extension/schema/inline-completer.json:/properties/streamingAnimation/oneOf[1]/title
+msgctxt "settings"
+msgid "Uncover"
+msgstr ""
+
+#: /packages/completer-extension/schema/inline-completer.json:/properties/streamingAnimation/title
+msgctxt "settings"
+msgid "Streaming animation"
+msgstr ""
+
+#: /packages/completer-extension/schema/inline-completer.json:/title
+msgctxt "schema"
+msgid "Inline Completer"
+msgstr ""
+
 #: /packages/completer-extension/schema/manager.json:/description
 msgctxt "schema"
 msgid "Code Completion settings."
 msgstr ""
 
 #: /packages/completer-extension/schema/manager.json:/jupyter.lab.setting-icon-label
 msgctxt "settings"
-msgid "Code Completion settings"
+msgid "Code Completer"
 msgstr ""
 
 #: /packages/completer-extension/schema/manager.json:/properties/autoCompletion/description
 msgctxt "settings"
 msgid "Autocompletion setting."
 msgstr ""
 
@@ -890,14 +998,24 @@
 msgstr ""
 
 #: /packages/docmanager-extension/schema/plugin.json:/properties/lastModifiedCheckMargin/title
 msgctxt "settings"
 msgid "Margin for last modified timestamp check"
 msgstr ""
 
+#: /packages/docmanager-extension/schema/plugin.json:/properties/maxNumberRecents/description
+msgctxt "settings"
+msgid "Number of recently opened/closed files and directories to remember."
+msgstr ""
+
+#: /packages/docmanager-extension/schema/plugin.json:/properties/maxNumberRecents/title
+msgctxt "settings"
+msgid "Recent Items Number"
+msgstr ""
+
 #: /packages/docmanager-extension/schema/plugin.json:/properties/renameUntitledFileOnSave/description
 msgctxt "settings"
 msgid "Whether to prompt to rename untitled file on first manual save."
 msgstr ""
 
 #: /packages/docmanager-extension/schema/plugin.json:/properties/renameUntitledFileOnSave/title
 msgctxt "settings"
@@ -915,14 +1033,24 @@
 msgstr "Plugin căutare document."
 
 #: /packages/documentsearch-extension/schema/plugin.json:/jupyter.lab.setting-icon-label
 msgctxt "settings"
 msgid "Document Search"
 msgstr ""
 
+#: /packages/documentsearch-extension/schema/plugin.json:/properties/autoSearchInSelection/description
+msgctxt "settings"
+msgid "When starting search, the 'search in selection' mode will be enabled if `any` text/cell is selected, or when `multiple` lines or cells are selected, or `never`."
+msgstr ""
+
+#: /packages/documentsearch-extension/schema/plugin.json:/properties/autoSearchInSelection/title
+msgctxt "settings"
+msgid "Search in selection automatically"
+msgstr ""
+
 #: /packages/documentsearch-extension/schema/plugin.json:/properties/searchDebounceTime/description
 msgctxt "settings"
 msgid "The debounce time in milliseconds applied to the search input field. The already opened input files will not be updated if you change that value"
 msgstr ""
 
 #: /packages/documentsearch-extension/schema/plugin.json:/properties/searchDebounceTime/title
 msgctxt "settings"
@@ -981,29 +1109,49 @@
 msgstr ""
 
 #: /packages/filebrowser-extension/schema/browser.json:/properties/filterDirectories/description
 msgctxt "settings"
 msgid "Whether to apply the search on directories"
 msgstr ""
 
+#: /packages/filebrowser-extension/schema/browser.json:/properties/filterDirectories/description
+msgctxt "settings"
+msgid "Whether to apply the search on folders"
+msgstr ""
+
 #: /packages/filebrowser-extension/schema/browser.json:/properties/filterDirectories/title
 msgctxt "settings"
 msgid "Filter directories"
 msgstr ""
 
+#: /packages/filebrowser-extension/schema/browser.json:/properties/filterDirectories/title
+msgctxt "settings"
+msgid "Filter folders"
+msgstr ""
+
 #: /packages/filebrowser-extension/schema/browser.json:/properties/navigateToCurrentDirectory/description
 msgctxt "settings"
 msgid "Whether to automatically navigate to a document's current directory"
 msgstr ""
 
+#: /packages/filebrowser-extension/schema/browser.json:/properties/navigateToCurrentDirectory/description
+msgctxt "settings"
+msgid "Whether to automatically navigate to a document's current folder"
+msgstr ""
+
 #: /packages/filebrowser-extension/schema/browser.json:/properties/navigateToCurrentDirectory/title
 msgctxt "settings"
 msgid "Navigate to current directory"
 msgstr ""
 
+#: /packages/filebrowser-extension/schema/browser.json:/properties/navigateToCurrentDirectory/title
+msgctxt "settings"
+msgid "Navigate to current folder"
+msgstr ""
+
 #: /packages/filebrowser-extension/schema/browser.json:/properties/showFileCheckboxes/description
 msgctxt "settings"
 msgid "Whether to show checkboxes next to files and folders"
 msgstr ""
 
 #: /packages/filebrowser-extension/schema/browser.json:/properties/showFileCheckboxes/title
 msgctxt "settings"
@@ -1016,14 +1164,24 @@
 msgstr ""
 
 #: /packages/filebrowser-extension/schema/browser.json:/properties/showFileSizeColumn/title
 msgctxt "settings"
 msgid "Show file size column"
 msgstr ""
 
+#: /packages/filebrowser-extension/schema/browser.json:/properties/showFullPath/description
+msgctxt "settings"
+msgid "Whether to show full path in browser bread crumbs"
+msgstr ""
+
+#: /packages/filebrowser-extension/schema/browser.json:/properties/showFullPath/title
+msgctxt "settings"
+msgid "Show full path in browser bread crumbs"
+msgstr ""
+
 #: /packages/filebrowser-extension/schema/browser.json:/properties/showHiddenFiles/description
 msgctxt "settings"
 msgid "Whether to show hidden files. The server parameter `ContentsManager.allow_hidden` must be set to `True` to display hidden files."
 msgstr ""
 
 #: /packages/filebrowser-extension/schema/browser.json:/properties/showHiddenFiles/title
 msgctxt "settings"
@@ -1566,14 +1724,19 @@
 #: /packages/notebook-extension/schema/export.json:/description
 msgctxt "schema"
 msgid "Notebook Export settings."
 msgstr ""
 
 #: /packages/notebook-extension/schema/export.json:/jupyter.lab.menus/main[0]/items[1]/submenu/label
 msgctxt "menu"
+msgid "Save and Export Notebook As"
+msgstr ""
+
+#: /packages/notebook-extension/schema/export.json:/jupyter.lab.menus/main[0]/items[1]/submenu/label
+msgctxt "menu"
 msgid "Save and Export Notebook As…"
 msgstr ""
 
 #: /packages/notebook-extension/schema/export.json:/title
 msgctxt "schema"
 msgid "Notebook Export"
 msgstr ""
@@ -1630,14 +1793,24 @@
 msgstr "Setări Notebook."
 
 #: /packages/notebook-extension/schema/tracker.json:/jupyter.lab.setting-icon-label
 msgctxt "settings"
 msgid "Notebook"
 msgstr ""
 
+#: /packages/notebook-extension/schema/tracker.json:/properties/accessKernelHistory/description
+msgctxt "settings"
+msgid "Enable kernel history access from notebook cells. Enabling this allows you to scroll through kernel history from a given notebook cell."
+msgstr ""
+
+#: /packages/notebook-extension/schema/tracker.json:/properties/accessKernelHistory/title
+msgctxt "settings"
+msgid "Kernel history access"
+msgstr ""
+
 #: /packages/notebook-extension/schema/tracker.json:/properties/autoStartDefaultKernel/description
 msgctxt "settings"
 msgid "Whether to automatically start the preferred kernel."
 msgstr ""
 
 #: /packages/notebook-extension/schema/tracker.json:/properties/autoStartDefaultKernel/title
 msgctxt "settings"
@@ -1670,14 +1843,24 @@
 msgstr ""
 
 #: /packages/notebook-extension/schema/tracker.json:/properties/documentWideUndoRedo/title
 msgctxt "settings"
 msgid "Enable undo/redo actions at the notebook document level."
 msgstr ""
 
+#: /packages/notebook-extension/schema/tracker.json:/properties/enableKernelInitNotification/description
+msgctxt "settings"
+msgid "Display notification if code cells are run while kernel is initializing."
+msgstr ""
+
+#: /packages/notebook-extension/schema/tracker.json:/properties/enableKernelInitNotification/title
+msgctxt "settings"
+msgid "Notify about code execution if kernel is initializing"
+msgstr ""
+
 #: /packages/notebook-extension/schema/tracker.json:/properties/inputHistoryScope/description
 msgctxt "settings"
 msgid "Whether the line history for standard input (e.g. the ipdb prompt) should kept separately for different kernel sessions (`session`) or combined (`global`)."
 msgstr ""
 
 #: /packages/notebook-extension/schema/tracker.json:/properties/inputHistoryScope/title
 msgctxt "settings"
@@ -1762,15 +1945,15 @@
 #: /packages/notebook-extension/schema/tracker.json:/properties/renderingLayout/title
 msgctxt "settings"
 msgid "Rendering Layout"
 msgstr ""
 
 #: /packages/notebook-extension/schema/tracker.json:/properties/scrollHeadingToTop/description
 msgctxt "settings"
-msgid "Whether to scroll heading to the document top when selecting it in the table of contents. Starting with JupyterLab 4.1 this setting will be enabled by default."
+msgid "Whether to scroll heading to the document top when selecting it in the table of contents."
 msgstr ""
 
 #: /packages/notebook-extension/schema/tracker.json:/properties/scrollHeadingToTop/title
 msgctxt "settings"
 msgid "Scroll heading to top"
 msgstr ""
 
@@ -1955,14 +2138,24 @@
 msgstr ""
 
 #: /packages/terminal-extension/schema/plugin.json:/properties/closeOnExit/title
 msgctxt "settings"
 msgid "Close on exit"
 msgstr ""
 
+#: /packages/terminal-extension/schema/plugin.json:/properties/cursorBlink/description
+msgctxt "settings"
+msgid "Whether to blink the cursor. Changes require reopening the terminal."
+msgstr ""
+
+#: /packages/terminal-extension/schema/plugin.json:/properties/cursorBlink/title
+msgctxt "settings"
+msgid "Blinking cursor"
+msgstr ""
+
 #: /packages/terminal-extension/schema/plugin.json:/properties/fontFamily/description
 msgctxt "settings"
 msgid "The font family used to render text."
 msgstr ""
 
 #: /packages/terminal-extension/schema/plugin.json:/properties/fontFamily/title
 msgctxt "settings"
@@ -2200,232 +2393,263 @@
 msgstr ""
 
 #: /packages/translation-extension/schema/plugin.json:/title
 msgctxt "schema"
 msgid "Language"
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:1078 packages/application-extension/src/index.tsx:1083
+#: /packages/workspaces-extension/schema/menu.json:/description /packages/workspaces-extension/schema/menu.json:/title
+msgctxt "schema"
+msgid "Workspaces Menu"
+msgstr ""
+
+#: /packages/workspaces-extension/schema/menu.json:/jupyter.lab.menus/main[0]/items[0]/submenu/label
+msgctxt "menu"
+msgid "Workspaces"
+msgstr ""
+
+#: /packages/workspaces-extension/schema/sidebar.json:/description /packages/workspaces-extension/schema/sidebar.json:/title
+msgctxt "schema"
+msgid "Workspaces Sidebar"
+msgstr ""
+
+#: packages/application-extension/src/index.tsx:1005 packages/application-extension/src/index.tsx:990
+msgid "The path: %1 was not found. JupyterLab redirected to: %2"
+msgstr "Calea: %1 nu a fost găsită. JupyterLab a fost redirecționat către: %2"
+
+#: packages/application-extension/src/index.tsx:1014 packages/application-extension/src/index.tsx:999
+msgid "Path Not Found"
+msgstr ""
+
+#: packages/application-extension/src/index.tsx:1143 packages/application-extension/src/index.tsx:1148 packages/application-extension/src/index.tsx:1158 packages/application-extension/src/index.tsx:1163
 msgid "Property Inspector"
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:1171
+#: packages/application-extension/src/index.tsx:1236 packages/application-extension/src/index.tsx:1251
 msgid "Simple Interface (%1)"
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:1173 packages/application-extension/src/index.tsx:385
+#: packages/application-extension/src/index.tsx:1238 packages/application-extension/src/index.tsx:1253 packages/application-extension/src/index.tsx:450 packages/application-extension/src/index.tsx:471
 msgid "Simple Interface"
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:1181
+#: packages/application-extension/src/index.tsx:1246 packages/application-extension/src/index.tsx:1261
 msgid "Simple"
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:1220 packages/application-extension/src/index.tsx:791 packages/apputils/src/toolbar/factory.ts:33 packages/extensionmanager/src/model.ts:504 packages/extensionmanager/src/model.ts:526 packages/extensionmanager/src/model.ts:529 packages/extensionmanager/src/model.ts:551 packages/mainmenu-extension/src/index.ts:770
+#: packages/application-extension/src/index.tsx:1286 packages/application-extension/src/index.tsx:1301 packages/application-extension/src/index.tsx:856 packages/application-extension/src/index.tsx:871 packages/apputils/src/toolbar/factory.ts:33 packages/extensionmanager/src/model.ts:529 packages/extensionmanager/src/model.ts:551 packages/mainmenu-extension/src/index.ts:767 packages/mainmenu-extension/src/index.ts:770
 msgid "Information"
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:1221
+#: packages/application-extension/src/index.tsx:1287 packages/application-extension/src/index.tsx:1302
 msgid "Context menu customization has changed. You will need to reload JupyterLab to see the changes."
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:1226 packages/application-extension/src/index.tsx:797 packages/apputils/src/toolbar/factory.ts:39 packages/docmanager-extension/src/index.tsx:739 packages/mainmenu-extension/src/index.ts:776
+#: packages/application-extension/src/index.tsx:1292 packages/application-extension/src/index.tsx:1307 packages/application-extension/src/index.tsx:862 packages/application-extension/src/index.tsx:877 packages/apputils/src/toolbar/factory.ts:39 packages/docmanager-extension/src/index.tsx:750 packages/docmanager-extension/src/index.tsx:762 packages/mainmenu-extension/src/index.ts:773 packages/mainmenu-extension/src/index.ts:776
 msgid "Reload"
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:132 packages/apputils-extension/src/index.ts:319 packages/documentsearch-extension/src/index.ts:325 packages/documentsearch-extension/src/index.ts:326 packages/logconsole-extension/src/index.tsx:246 packages/mainmenu-extension/src/index.ts:236 packages/mainmenu-extension/src/index.ts:240 packages/mainmenu-extension/src/index.ts:250 packages/statusbar-extension/src/index.ts:48
+#: packages/application-extension/src/index.tsx:135 packages/apputils-extension/src/index.ts:319 packages/apputils-extension/src/index.ts:323 packages/documentsearch-extension/src/index.ts:463 packages/documentsearch-extension/src/index.ts:469 packages/logconsole-extension/src/index.tsx:246 packages/mainmenu-extension/src/index.ts:236 packages/mainmenu-extension/src/index.ts:237 packages/mainmenu-extension/src/index.ts:240 packages/mainmenu-extension/src/index.ts:241 packages/mainmenu-extension/src/index.ts:250 packages/mainmenu-extension/src/index.ts:251 packages/statusbar-extension/src/index.ts:48
 msgid "Main Area"
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:136
+#: packages/application-extension/src/index.tsx:139
 msgid "Shift+Right Click for Browser Menu"
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:1402
+#: packages/application-extension/src/index.tsx:1468 packages/application-extension/src/index.tsx:1483
 msgid "Switch Sidebar Side"
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:205
+#: packages/application-extension/src/index.tsx:239
 msgid "Close Tab"
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:219
+#: packages/application-extension/src/index.tsx:253
 msgid "Close All Other Tabs"
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:239
+#: packages/application-extension/src/index.tsx:273
 msgid "Close Tabs to Right"
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:254
+#: packages/application-extension/src/index.tsx:288 packages/application-extension/src/index.tsx:296
 msgid "Activate Next Tab"
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:261
+#: packages/application-extension/src/index.tsx:295 packages/application-extension/src/index.tsx:303
 msgid "Activate Previous Tab"
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:268
+#: packages/application-extension/src/index.tsx:302 packages/application-extension/src/index.tsx:310
 msgid "Activate Next Tab Bar"
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:275
+#: packages/application-extension/src/index.tsx:309 packages/application-extension/src/index.tsx:317
 msgid "Activate Previous Tab Bar"
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:282
+#: packages/application-extension/src/index.tsx:316 packages/application-extension/src/index.tsx:324
 msgid "Close All Tabs"
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:289
+#: packages/application-extension/src/index.tsx:323 packages/application-extension/src/index.tsx:331
 msgid "Show Header"
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:300
+#: packages/application-extension/src/index.tsx:334 packages/application-extension/src/index.tsx:342
 msgid "Show Left Sidebar"
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:316
+#: packages/application-extension/src/index.tsx:350 packages/application-extension/src/index.tsx:358
 msgid "Show Right Sidebar"
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:334
+#: packages/application-extension/src/index.tsx:366 packages/application-extension/src/index.tsx:378
+msgid "Toggle Sidebar Element"
+msgstr ""
+
+#: packages/application-extension/src/index.tsx:380
+msgid "Toggle Element %1 in Right Sidebar"
+msgstr ""
+
+#: packages/application-extension/src/index.tsx:384
+msgid "Toggle Element %1 in Left Sidebar"
+msgstr ""
+
+#: packages/application-extension/src/index.tsx:399 packages/application-extension/src/index.tsx:420
 msgid "Show Right Activity Bar"
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:335
+#: packages/application-extension/src/index.tsx:400 packages/application-extension/src/index.tsx:421
 msgid "Show Left Activity Bar"
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:354
+#: packages/application-extension/src/index.tsx:419 packages/application-extension/src/index.tsx:440
 msgid "Presentation Mode"
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:365
+#: packages/application-extension/src/index.tsx:430 packages/application-extension/src/index.tsx:451
 msgid "Set %1 mode."
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:366
+#: packages/application-extension/src/index.tsx:431 packages/application-extension/src/index.tsx:452
 msgid "Set the layout `mode`."
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:367
+#: packages/application-extension/src/index.tsx:432 packages/application-extension/src/index.tsx:453
 msgid "The layout `mode` can be \"single-document\" or \"multiple-document\"."
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:397
+#: packages/application-extension/src/index.tsx:462 packages/application-extension/src/index.tsx:483
 msgid "Reset Default Layout"
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:527
+#: packages/application-extension/src/index.tsx:592 packages/application-extension/src/index.tsx:613
 msgid "Error Registering Plugins"
 msgstr "Eroare înregistrare Plugin-uri"
 
-#: packages/application-extension/src/index.tsx:577
+#: packages/application-extension/src/index.tsx:642 packages/application-extension/src/index.tsx:657
 msgid "Build Complete"
 msgstr "Build Finalizat"
 
-#: packages/application-extension/src/index.tsx:580
+#: packages/application-extension/src/index.tsx:645 packages/application-extension/src/index.tsx:660
 msgid "Build successfully completed, reload page?"
 msgstr "Build finalizat cu succes, reîncărcați pagina?"
 
-#: packages/application-extension/src/index.tsx:582
+#: packages/application-extension/src/index.tsx:647 packages/application-extension/src/index.tsx:662
 msgid "You will lose any unsaved changes."
 msgstr "Veţi pierde orice modificări nesalvate."
 
-#: packages/application-extension/src/index.tsx:587
+#: packages/application-extension/src/index.tsx:652 packages/application-extension/src/index.tsx:667
 msgid "Reload Without Saving"
 msgstr "Reîncarcă fără a salva"
 
-#: packages/application-extension/src/index.tsx:590
+#: packages/application-extension/src/index.tsx:655 packages/application-extension/src/index.tsx:670
 msgid "Save and Reload"
 msgstr "Salvează și Reîncarcă"
 
-#: packages/application-extension/src/index.tsx:603
+#: packages/application-extension/src/index.tsx:668 packages/application-extension/src/index.tsx:683
 msgid "Save Failed"
 msgstr "Salvare Eșuată"
 
-#: packages/application-extension/src/index.tsx:612
+#: packages/application-extension/src/index.tsx:677 packages/application-extension/src/index.tsx:692
 msgid "Build Failed"
 msgstr "Build Eșuat"
 
-#: packages/application-extension/src/index.tsx:630
+#: packages/application-extension/src/index.tsx:695 packages/application-extension/src/index.tsx:710
 msgid "JupyterLab build is suggested:"
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:637
+#: packages/application-extension/src/index.tsx:702 packages/application-extension/src/index.tsx:717
 msgid "Build Recommended"
 msgstr "Build Recomandat"
 
-#: packages/application-extension/src/index.tsx:641
+#: packages/application-extension/src/index.tsx:706 packages/application-extension/src/index.tsx:721
 msgid "Build"
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:707
+#: packages/application-extension/src/index.tsx:772 packages/application-extension/src/index.tsx:787
 msgid "Are you sure you want to exit JupyterLab?\n\n"
 "Any unsaved changes will be lost."
 msgstr "Ești sigur că vrei să ieși din JupyterLab?\n\n"
 "Se vor pierde orice modificări nesalvate."
 
-#: packages/application-extension/src/index.tsx:792
+#: packages/application-extension/src/index.tsx:857 packages/application-extension/src/index.tsx:872
 msgid "User layout customization has changed. You may need to reload JupyterLab to see the changes."
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:925
-msgid "The path: %1 was not found. JupyterLab redirected to: %2"
-msgstr "Calea: %1 nu a fost găsită. JupyterLab a fost redirecționat către: %2"
-
-#: packages/application-extension/src/index.tsx:934
-msgid "Path Not Found"
-msgstr ""
-
 #: packages/application/src/connectionlost.ts:19
 msgid "Server Connection Error"
 msgstr ""
 
 #: packages/application/src/connectionlost.ts:20
 msgid "A connection to the Jupyter server could not be established.\n"
 "JupyterLab will continue trying to reconnect.\n"
 "Check your network connection or Jupyter server configuration.\n"
 msgstr ""
 
-#: packages/application/src/shell.ts:713
-msgid "main"
+#: packages/application/src/shell.ts:734 packages/application/src/shell.ts:741
+msgid "main menu"
 msgstr ""
 
-#: packages/application/src/shell.ts:716 packages/application/src/shell.ts:720
+#: packages/application/src/shell.ts:738 packages/application/src/shell.ts:742 packages/application/src/shell.ts:745 packages/application/src/shell.ts:749
 msgid "main sidebar"
 msgstr ""
 
-#: packages/application/src/shell.ts:724 packages/application/src/shell.ts:728
+#: packages/application/src/shell.ts:746 packages/application/src/shell.ts:750 packages/application/src/shell.ts:753 packages/application/src/shell.ts:757
 msgid "alternate sidebar"
 msgstr ""
 
-#: packages/application/src/utils.ts:148
+#: packages/application/src/utils.ts:148 packages/application/src/utils.ts:253
 msgid "%1 and %2"
 msgstr ""
 
 #: packages/apputils-extension/src/announcements.ts:102
+msgid "Would you like to get notified about official Jupyter news?"
+msgstr ""
+
+#: packages/apputils-extension/src/announcements.ts:102
 msgid "Would you like to receive official Jupyter news?\n"
 "Please read the privacy policy."
 msgstr ""
 
 #: packages/apputils-extension/src/announcements.ts:110
 msgid "Open privacy policy"
 msgstr ""
 
 #: packages/apputils-extension/src/announcements.ts:116
 msgid "Privacy policies"
 msgstr ""
 
-#: packages/apputils-extension/src/announcements.ts:126 packages/extensionmanager/src/widget.tsx:434 packages/extensionmanager/src/widget.tsx:437 packages/extensionmanager/src/widget.tsx:449
+#: packages/apputils-extension/src/announcements.ts:126 packages/extensionmanager/src/widget.tsx:443 packages/pluginmanager/src/widget.tsx:125
 msgid "Yes"
 msgstr ""
 
-#: packages/apputils-extension/src/announcements.ts:143 packages/extensionmanager/src/widget.tsx:424 packages/extensionmanager/src/widget.tsx:427 packages/extensionmanager/src/widget.tsx:439
+#: packages/apputils-extension/src/announcements.ts:143 packages/extensionmanager/src/widget.tsx:433 packages/pluginmanager/src/widget.tsx:128
 msgid "No"
 msgstr ""
 
 #: packages/apputils-extension/src/announcements.ts:180
 msgid "Hide"
 msgstr ""
 
@@ -2458,98 +2682,102 @@
 msgid "Clear Workspace"
 msgstr ""
 
 #: packages/apputils-extension/src/index.ts:290
 msgid "Print…"
 msgstr ""
 
-#: packages/apputils-extension/src/index.ts:321
+#: packages/apputils-extension/src/index.ts:321 packages/apputils-extension/src/index.ts:325
 msgid "Show Header Above Content"
 msgstr ""
 
-#: packages/apputils-extension/src/index.ts:429
+#: packages/apputils-extension/src/index.ts:429 packages/apputils-extension/src/index.ts:438
 msgid "Load state for the current workspace."
 msgstr ""
 
-#: packages/apputils-extension/src/index.ts:493
+#: packages/apputils-extension/src/index.ts:493 packages/apputils-extension/src/index.ts:502
 msgid "Reset Application State"
 msgstr "Resetează Starea Aplicației"
 
-#: packages/apputils-extension/src/index.ts:504
+#: packages/apputils-extension/src/index.ts:504 packages/apputils-extension/src/index.ts:513
 msgid "Reset state when loading for the workspace."
 msgstr ""
 
-#: packages/apputils-extension/src/index.ts:595
+#: packages/apputils-extension/src/index.ts:595 packages/apputils-extension/src/index.ts:604
 msgid "Run First Enabled Command"
 msgstr "Rulează Prima Comandă Activată"
 
-#: packages/apputils-extension/src/index.ts:613
+#: packages/apputils-extension/src/index.ts:613 packages/apputils-extension/src/index.ts:622
 msgid "Run All Enabled Commands Passed as Args"
 msgstr ""
 
-#: packages/apputils-extension/src/index.ts:634 packages/apputils-extension/src/index.ts:644
+#: packages/apputils-extension/src/index.ts:644
 msgid "Show Keyboard Shortcuts"
 msgstr ""
 
-#: packages/apputils-extension/src/index.ts:635 packages/apputils-extension/src/index.ts:645
+#: packages/apputils-extension/src/index.ts:645 packages/apputils-extension/src/index.ts:654
 msgid "Show relevant keyboard shortcuts for the current active widget"
 msgstr ""
 
-#: packages/apputils-extension/src/index.ts:655 packages/apputils-extension/src/index.ts:662 packages/apputils-extension/src/index.ts:665 packages/help-extension/src/index.tsx:183 packages/help-extension/src/index.tsx:217 packages/help-extension/src/index.tsx:479 packages/help-extension/src/index.tsx:90
+#: packages/apputils-extension/src/index.ts:653
+msgid "Show Keyboard Shortcuts…"
+msgstr ""
+
+#: packages/apputils-extension/src/index.ts:662 packages/apputils-extension/src/index.ts:671 packages/help-extension/src/index.tsx:183 packages/help-extension/src/index.tsx:296 packages/help-extension/src/index.tsx:500 packages/help-extension/src/index.tsx:90
 msgid "Help"
 msgstr ""
 
-#: packages/apputils-extension/src/notificationplugin.tsx:166 packages/apputils-extension/src/notificationplugin.tsx:353
+#: packages/apputils-extension/src/notificationplugin.tsx:167 packages/apputils-extension/src/notificationplugin.tsx:354
 msgid "%1 notification"
 msgid_plural "%1 notifications"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 
-#: packages/apputils-extension/src/notificationplugin.tsx:167 packages/apputils-extension/src/notificationplugin.tsx:354
+#: packages/apputils-extension/src/notificationplugin.tsx:168 packages/apputils-extension/src/notificationplugin.tsx:355
 msgid "No notifications"
 msgstr ""
 
-#: packages/apputils-extension/src/notificationplugin.tsx:176
+#: packages/apputils-extension/src/notificationplugin.tsx:177
 msgid "Dismiss all notifications"
 msgstr ""
 
-#: packages/apputils-extension/src/notificationplugin.tsx:183
+#: packages/apputils-extension/src/notificationplugin.tsx:184
 msgid "Hide notifications"
 msgstr ""
 
-#: packages/apputils-extension/src/notificationplugin.tsx:229
+#: packages/apputils-extension/src/notificationplugin.tsx:230
 msgid "Dismiss notification"
 msgstr ""
 
-#: packages/apputils-extension/src/notificationplugin.tsx:401 packages/apputils-extension/src/notificationplugin.tsx:402
+#: packages/apputils-extension/src/notificationplugin.tsx:402
 msgid "Emit a notification"
 msgstr ""
 
-#: packages/apputils-extension/src/notificationplugin.tsx:402 packages/apputils-extension/src/notificationplugin.tsx:403
+#: packages/apputils-extension/src/notificationplugin.tsx:403
 msgid "Notification is described by {message: string, type?: string, options?: {autoClose?: number | false, actions: {label: string, commandId: string, args?: ReadOnlyJSONObject, caption?: string, className?: string}[], data?: ReadOnlyJSONValue}}."
 msgstr ""
 
-#: packages/apputils-extension/src/notificationplugin.tsx:439 packages/apputils-extension/src/notificationplugin.tsx:440
+#: packages/apputils-extension/src/notificationplugin.tsx:440
 msgid "Update a notification"
 msgstr ""
 
-#: packages/apputils-extension/src/notificationplugin.tsx:440 packages/apputils-extension/src/notificationplugin.tsx:441
+#: packages/apputils-extension/src/notificationplugin.tsx:441
 msgid "Notification is described by {id: string, message: string, type?: string, options?: {autoClose?: number | false, actions: {label: string, commandId: string, args?: ReadOnlyJSONObject, caption?: string, className?: string}[], data?: ReadOnlyJSONValue}}."
 msgstr ""
 
-#: packages/apputils-extension/src/notificationplugin.tsx:479 packages/apputils-extension/src/notificationplugin.tsx:480
+#: packages/apputils-extension/src/notificationplugin.tsx:480
 msgid "Dismiss a notification"
 msgstr ""
 
-#: packages/apputils-extension/src/notificationplugin.tsx:600 packages/apputils-extension/src/notificationplugin.tsx:601
+#: packages/apputils-extension/src/notificationplugin.tsx:601
 msgid "Show Notifications"
 msgstr ""
 
-#: packages/apputils-extension/src/notificationplugin.tsx:688 packages/apputils-extension/src/notificationplugin.tsx:689
+#: packages/apputils-extension/src/notificationplugin.tsx:699
 msgid "Hide notification"
 msgstr ""
 
 #: packages/apputils-extension/src/palette.ts:101
 msgid "Command Palette Section"
 msgstr ""
 
@@ -2569,107 +2797,135 @@
 msgid "SEARCH"
 msgstr "CAUTĂ"
 
 #: packages/apputils-extension/src/palette.ts:42
 msgid "Command Palette"
 msgstr "Paletă de comenzi"
 
-#: packages/apputils-extension/src/shortcuts.tsx:183 packages/apputils-extension/src/shortcuts.tsx:193
+#: packages/apputils-extension/src/shortcuts.tsx:193
 msgid "Keyboard Shortcuts"
 msgstr ""
 
-#: packages/apputils-extension/src/shortcuts.tsx:187 packages/apputils-extension/src/shortcuts.tsx:197 packages/docmanager/src/widgetmanager.ts:397 packages/filebrowser/src/listing.ts:1399 packages/filebrowser/src/listing.ts:1415 packages/running-extension/src/opentabs.ts:86
+#: packages/apputils-extension/src/shortcuts.tsx:197 packages/docmanager/src/widgetmanager.ts:397 packages/docmanager/src/widgetmanager.ts:468 packages/filebrowser/src/listing.ts:1415 packages/filebrowser/src/listing.ts:1436 packages/filebrowser/src/listing.ts:1488 packages/running-extension/src/opentabs.ts:86
 msgid "Close"
 msgstr ""
 
-#: packages/apputils-extension/src/themesplugins.ts:112
+#: packages/apputils-extension/src/themesplugins.ts:118
 msgid "Switch to the provided `theme`."
 msgstr ""
 
-#: packages/apputils-extension/src/themesplugins.ts:117
+#: packages/apputils-extension/src/themesplugins.ts:123
 msgid "Use Theme: %1"
 msgstr "Folosește Tema: %1"
 
-#: packages/apputils-extension/src/themesplugins.ts:131
+#: packages/apputils-extension/src/themesplugins.ts:143
+msgid "Switch to the provided light `theme`."
+msgstr ""
+
+#: packages/apputils-extension/src/themesplugins.ts:148
+msgid "Set Preferred Light Theme: %1"
+msgstr ""
+
+#: packages/apputils-extension/src/themesplugins.ts:164
+msgid "Switch to the provided dark `theme`."
+msgstr ""
+
+#: packages/apputils-extension/src/themesplugins.ts:169
+msgid "Set Preferred Dark Theme: %1"
+msgstr ""
+
+#: packages/apputils-extension/src/themesplugins.ts:186
+msgid "Synchronize Styling Theme with System Settings"
+msgstr ""
+
+#: packages/apputils-extension/src/themesplugins.ts:187
+msgid "Synchronize with System Settings"
+msgstr ""
+
+#: packages/apputils-extension/src/themesplugins.ts:195
 msgid "Theme Scrollbars"
 msgstr "Scrollbar-uri Temă"
 
-#: packages/apputils-extension/src/themesplugins.ts:138
+#: packages/apputils-extension/src/themesplugins.ts:202
 msgid "waiting for fonts"
 msgstr ""
 
-#: packages/apputils-extension/src/themesplugins.ts:149
+#: packages/apputils-extension/src/themesplugins.ts:213
 msgid "Increase Code Font Size"
 msgstr "Măreşte Dimensiunea Fontului Codului"
 
-#: packages/apputils-extension/src/themesplugins.ts:151
+#: packages/apputils-extension/src/themesplugins.ts:215
 msgid "Increase Content Font Size"
 msgstr ""
 
-#: packages/apputils-extension/src/themesplugins.ts:153
+#: packages/apputils-extension/src/themesplugins.ts:217
 msgid "Increase UI Font Size"
 msgstr ""
 
-#: packages/apputils-extension/src/themesplugins.ts:155 packages/fileeditor-extension/src/commands.ts:280 packages/fileeditor-extension/src/commands.ts:281
+#: packages/apputils-extension/src/themesplugins.ts:219 packages/fileeditor-extension/src/commands.ts:281 packages/fileeditor-extension/src/commands.ts:282
 msgid "Increase Font Size"
 msgstr ""
 
-#: packages/apputils-extension/src/themesplugins.ts:165
+#: packages/apputils-extension/src/themesplugins.ts:229
 msgid "Decrease Code Font Size"
 msgstr "Micșorează Dimensiunea Fontului Codului"
 
-#: packages/apputils-extension/src/themesplugins.ts:167
+#: packages/apputils-extension/src/themesplugins.ts:231
 msgid "Decrease Content Font Size"
 msgstr ""
 
-#: packages/apputils-extension/src/themesplugins.ts:169
+#: packages/apputils-extension/src/themesplugins.ts:233
 msgid "Decrease UI Font Size"
 msgstr ""
 
-#: packages/apputils-extension/src/themesplugins.ts:171 packages/fileeditor-extension/src/commands.ts:284 packages/fileeditor-extension/src/commands.ts:285
+#: packages/apputils-extension/src/themesplugins.ts:235 packages/fileeditor-extension/src/commands.ts:285 packages/fileeditor-extension/src/commands.ts:286
 msgid "Decrease Font Size"
 msgstr ""
 
-#: packages/apputils-extension/src/themesplugins.ts:231 packages/codemirror/src/extension.ts:851 packages/codemirror/src/extension.ts:865 packages/codemirror/src/extension.ts:871
+#: packages/apputils-extension/src/themesplugins.ts:295 packages/codemirror/src/extension.ts:1006 packages/codemirror/src/extension.ts:982
 msgid "Theme"
 msgstr "Tema"
 
-#: packages/apputils-extension/src/workspacesplugin.ts:181
+#: packages/apputils-extension/src/workspacesplugin.ts:181 packages/apputils-extension/src/workspacesplugin.ts:95
 msgid "Workspace loader"
 msgstr ""
 
-#: packages/apputils-extension/src/workspacesplugin.ts:266 packages/apputils-extension/src/workspacesplugin.ts:267 packages/apputils-extension/src/workspacesplugin.ts:272 packages/apputils-extension/src/workspacesplugin.ts:275 packages/docmanager/src/widgetmanager.ts:436 packages/docmanager/src/widgetmanager.ts:442 packages/docregistry/src/context.ts:1015 packages/docregistry/src/context.ts:1019 packages/docregistry/src/context.ts:992
+#: packages/apputils-extension/src/workspacesplugin.ts:271 packages/apputils-extension/src/workspacesplugin.ts:279 packages/docmanager/src/widgetmanager.ts:442 packages/docmanager/src/widgetmanager.ts:513 packages/docregistry/src/context.ts:1041 packages/docregistry/src/context.ts:1043 packages/workspaces-extension/src/commands.ts:587
 msgid "Save"
 msgstr "Salvează"
 
-#: packages/apputils-extension/src/workspacesplugin.ts:268 packages/apputils-extension/src/workspacesplugin.ts:271 packages/apputils-extension/src/workspacesplugin.ts:79
+#: packages/apputils-extension/src/workspacesplugin.ts:272 packages/apputils-extension/src/workspacesplugin.ts:93 packages/workspaces-extension/src/commands.ts:458
+msgid "Save Current Workspace"
+msgstr "Salvează Workspace-ul Curent"
+
+#: packages/apputils-extension/src/workspacesplugin.ts:275 packages/apputils-extension/src/workspacesplugin.ts:79 packages/workspaces-extension/src/commands.ts:449 packages/workspaces-extension/src/commands.ts:584
 msgid "Save Current Workspace As…"
 msgstr ""
 
-#: packages/apputils-extension/src/workspacesplugin.ts:268 packages/apputils-extension/src/workspacesplugin.ts:93
-msgid "Save Current Workspace"
-msgstr "Salvează Workspace-ul Curent"
+#: packages/apputils-extension/src/workspacesplugin.ts:72
+msgid "JupyterLab Workspace File"
+msgstr ""
 
 #: packages/apputils-extension/src/workspacesplugin.ts:72
 msgid "JupyterLab workspace File"
 msgstr ""
 
-#: packages/apputils/src/dialog.tsx:47 packages/help-extension/src/index.tsx:153 packages/help-extension/src/index.tsx:404 packages/hub-extension/src/index.ts:173 packages/lsp/src/adapters/adapter.ts:470 packages/lsp/src/adapters/adapter.ts:473 packages/mainmenu-extension/src/index.ts:548
+#: packages/apputils/src/dialog.tsx:47 packages/help-extension/src/index.tsx:153 packages/help-extension/src/index.tsx:425 packages/hub-extension/src/index.ts:180 packages/lsp/src/adapters/adapter.ts:497 packages/mainmenu-extension/src/index.ts:545 packages/mainmenu-extension/src/index.ts:548
 msgid "Dismiss"
 msgstr ""
 
-#: packages/apputils/src/dialog.tsx:763 packages/apputils/src/dialog.tsx:770 packages/apputils/src/dialog.tsx:862 packages/apputils/src/dialog.tsx:870 packages/apputils/src/sessioncontext.tsx:1335 packages/debugger-extension/src/index.ts:696 packages/filebrowser/src/listing.ts:429 packages/filebrowser/src/listing.ts:433 packages/filebrowser/src/model.ts:449 packages/notebook/src/searchprovider.ts:514 packages/notebook/src/searchprovider.ts:516 packages/settingeditor/src/plugineditor.ts:132 packages/shortcuts-extension/src/components/ShortcutItem.tsx:224 packages/translation-extension/src/index.ts:147 packages/translation-extension/src/index.ts:156
+#: packages/apputils/src/dialog.tsx:770 packages/apputils/src/dialog.tsx:793 packages/apputils/src/dialog.tsx:870 packages/apputils/src/dialog.tsx:893 packages/apputils/src/sessioncontext.tsx:1335 packages/debugger-extension/src/index.ts:739 packages/debugger-extension/src/index.ts:840 packages/filebrowser/src/listing.ts:433 packages/filebrowser/src/listing.ts:436 packages/filebrowser/src/model.ts:442 packages/filebrowser/src/model.ts:449 packages/notebook/src/searchprovider.ts:516 packages/notebook/src/searchprovider.ts:519 packages/notebook/src/searchprovider.ts:527 packages/settingeditor/src/plugineditor.ts:132 packages/shortcuts-extension/src/components/ShortcutItem.tsx:224 packages/shortcuts-extension/src/components/ShortcutItem.tsx:341 packages/translation-extension/src/index.ts:156
 msgid "Cancel"
 msgstr "Anulează"
 
-#: packages/apputils/src/dialog.tsx:763 packages/apputils/src/dialog.tsx:770 packages/extensionmanager/src/dialog.tsx:37 packages/extensionmanager/src/model.ts:508 packages/extensionmanager/src/model.ts:531 packages/extensionmanager/src/model.ts:533 packages/extensionmanager/src/model.ts:556 packages/notebook/src/model.ts:377 packages/notebook/src/panel.ts:234 packages/notebook/src/searchprovider.ts:515 packages/notebook/src/searchprovider.ts:517 packages/settingeditor/src/plugineditor.ts:133
+#: packages/apputils/src/dialog.tsx:770 packages/apputils/src/dialog.tsx:793 packages/extensionmanager/src/dialog.tsx:37 packages/extensionmanager/src/model.ts:533 packages/extensionmanager/src/model.ts:556 packages/notebook/src/model.ts:377 packages/notebook/src/panel.ts:228 packages/notebook/src/searchprovider.ts:517 packages/notebook/src/searchprovider.ts:520 packages/notebook/src/searchprovider.ts:528 packages/settingeditor/src/plugineditor.ts:133
 msgid "Ok"
 msgstr ""
 
-#: packages/apputils/src/kernelstatuses.tsx:210 packages/apputils/src/sessioncontext.tsx:1746 packages/apputils/src/sessioncontext.tsx:1757 packages/apputils/src/sessioncontext.tsx:631
+#: packages/apputils/src/kernelstatuses.tsx:221 packages/apputils/src/sessioncontext.tsx:1757 packages/apputils/src/sessioncontext.tsx:631
 msgid "No Kernel"
 msgstr ""
 
 #: packages/apputils/src/kernelstatuses.tsx:29
 msgid "Unknown"
 msgstr ""
 
@@ -2713,166 +2969,166 @@
 msgid "Disconnected"
 msgstr ""
 
 #: packages/apputils/src/kernelstatuses.tsx:40
 msgid "Initializing"
 msgstr ""
 
-#: packages/apputils/src/kernelstatuses.tsx:62
+#: packages/apputils/src/kernelstatuses.tsx:63
 msgid "Change kernel for %1"
 msgstr ""
 
 #: packages/apputils/src/mainareawidget.ts:47
 msgid "notebook content"
 msgstr ""
 
 #: packages/apputils/src/mainareawidget.ts:50
 msgid "notebook actions"
 msgstr ""
 
-#: packages/apputils/src/runningSessions.tsx:115
+#: packages/apputils/src/runningSessions.tsx:126
 msgid "%1 Terminals, %2 Kernel sessions"
 msgstr ""
 
 #: packages/apputils/src/sessioncontext.tsx:1051
 msgid "Error Starting Kernel"
 msgstr ""
 
-#: packages/apputils/src/sessioncontext.tsx:1341 packages/apputils/src/sessioncontext.tsx:1344 packages/filebrowser/src/opendialog.ts:83
+#: packages/apputils/src/sessioncontext.tsx:1344 packages/filebrowser/src/opendialog.ts:106 packages/filebrowser/src/opendialog.ts:95
 msgid "Select"
 msgstr "Selectează"
 
-#: packages/apputils/src/sessioncontext.tsx:1345 packages/apputils/src/sessioncontext.tsx:1348 packages/apputils/src/sessioncontext.tsx:1353
+#: packages/apputils/src/sessioncontext.tsx:1345 packages/apputils/src/sessioncontext.tsx:1353
 msgid "Select Kernel"
 msgstr ""
 
-#: packages/apputils/src/sessioncontext.tsx:1353 packages/apputils/src/sessioncontext.tsx:1358
+#: packages/apputils/src/sessioncontext.tsx:1358
 msgid "Always start the preferred kernel"
 msgstr ""
 
-#: packages/apputils/src/sessioncontext.tsx:1354 packages/apputils/src/sessioncontext.tsx:1359
+#: packages/apputils/src/sessioncontext.tsx:1359
 msgid "Remember my choice and always start the preferred kernel"
 msgstr ""
 
-#: packages/apputils/src/sessioncontext.tsx:1415 packages/apputils/src/sessioncontext.tsx:1423
-msgid "Restart Kernel?"
+#: packages/apputils/src/sessioncontext.tsx:1419 packages/hub-extension/src/index.ts:179
+msgid "Restart"
 msgstr ""
 
-#: packages/apputils/src/sessioncontext.tsx:1416 packages/apputils/src/sessioncontext.tsx:1424
-msgid "Do you want to restart the kernel of %1? All variables will be lost."
+#: packages/apputils/src/sessioncontext.tsx:1420
+msgid "Confirm Kernel Restart"
 msgstr ""
 
-#: packages/apputils/src/sessioncontext.tsx:1419 packages/hub-extension/src/index.ts:172
-msgid "Restart"
+#: packages/apputils/src/sessioncontext.tsx:1423
+msgid "Restart Kernel?"
 msgstr ""
 
-#: packages/apputils/src/sessioncontext.tsx:1420
-msgid "Confirm Kernel Restart"
+#: packages/apputils/src/sessioncontext.tsx:1424
+msgid "Do you want to restart the kernel of %1? All variables will be lost."
 msgstr ""
 
 #: packages/apputils/src/sessioncontext.tsx:1429
 msgid "Cancel Kernel Restart"
 msgstr ""
 
-#: packages/apputils/src/sessioncontext.tsx:1473 packages/apputils/src/sessioncontext.tsx:1484
+#: packages/apputils/src/sessioncontext.tsx:1484
 msgid "Select kernel for:"
 msgstr ""
 
-#: packages/apputils/src/sessioncontext.tsx:1607 packages/apputils/src/sessioncontext.tsx:1618
+#: packages/apputils/src/sessioncontext.tsx:1618
 msgid "Start Preferred Kernel"
 msgstr ""
 
-#: packages/apputils/src/sessioncontext.tsx:1622 packages/apputils/src/sessioncontext.tsx:1633
+#: packages/apputils/src/sessioncontext.tsx:1633
 msgid "Start Other Kernel"
 msgstr ""
 
-#: packages/apputils/src/sessioncontext.tsx:1679 packages/apputils/src/sessioncontext.tsx:1690
+#: packages/apputils/src/sessioncontext.tsx:1690
 msgid "Use Kernel from Preferred Session"
 msgstr ""
 
-#: packages/apputils/src/sessioncontext.tsx:1694 packages/apputils/src/sessioncontext.tsx:1705
+#: packages/apputils/src/sessioncontext.tsx:1705
 msgid "Use Kernel from Other Session"
 msgstr ""
 
-#: packages/apputils/src/sessioncontext.tsx:1744 packages/apputils/src/sessioncontext.tsx:1755
+#: packages/apputils/src/sessioncontext.tsx:1755
 msgid "Use No Kernel"
 msgstr ""
 
-#: packages/apputils/src/sessioncontext.tsx:1768 packages/apputils/src/sessioncontext.tsx:1779
+#: packages/apputils/src/sessioncontext.tsx:1779
 msgid "Path:"
 msgstr ""
 
-#: packages/apputils/src/sessioncontext.tsx:1769 packages/apputils/src/sessioncontext.tsx:1780
+#: packages/apputils/src/sessioncontext.tsx:1780
 msgid "Name:"
 msgstr ""
 
-#: packages/apputils/src/sessioncontext.tsx:1770 packages/apputils/src/sessioncontext.tsx:1781
+#: packages/apputils/src/sessioncontext.tsx:1781
 msgid "Kernel Name:"
 msgstr ""
 
-#: packages/apputils/src/sessioncontext.tsx:1771 packages/apputils/src/sessioncontext.tsx:1782
+#: packages/apputils/src/sessioncontext.tsx:1782
 msgid "Kernel Id:"
 msgstr ""
 
-#: packages/apputils/src/thememanager.ts:371
+#: packages/apputils/src/thememanager.ts:467
 msgid "Neither theme %1 nor default %2 loaded."
 msgstr ""
 
-#: packages/apputils/src/thememanager.ts:455
+#: packages/apputils/src/thememanager.ts:551
 msgid "Error Loading Theme"
 msgstr ""
 
-#: packages/apputils/src/thememanager.ts:457
+#: packages/apputils/src/thememanager.ts:553
 msgid "OK"
 msgstr ""
 
 #: packages/apputils/src/toolbar/factory.ts:34
 msgid "Toolbar customization has changed. You will need to reload JupyterLab to see the changes."
 msgstr ""
 
 #: packages/apputils/src/toolbar/widget.tsx:168
 msgid "Switch kernel"
 msgstr ""
 
-#: packages/apputils/src/toolbar/widget.tsx:208
+#: packages/apputils/src/toolbar/widget.tsx:210
 msgid "Kernel %1"
 msgstr ""
 
-#: packages/apputils/src/toolbar/widget.tsx:56 packages/mainmenu-extension/src/index.ts:469 packages/notebook-extension/src/index.ts:2453 packages/notebook-extension/src/index.ts:2458 packages/notebook-extension/src/index.ts:2477
+#: packages/apputils/src/toolbar/widget.tsx:56 packages/mainmenu-extension/src/index.ts:467 packages/mainmenu-extension/src/index.ts:469 packages/notebook-extension/src/index.ts:2529 packages/notebook-extension/src/index.ts:2536 packages/notebook-extension/src/index.ts:2547
 msgid "Interrupt the kernel"
 msgstr ""
 
-#: packages/apputils/src/toolbar/widget.tsx:80 packages/mainmenu-extension/src/index.ts:494 packages/notebook-extension/src/index.ts:2321 packages/notebook-extension/src/index.ts:2325 packages/notebook-extension/src/index.ts:2344
+#: packages/apputils/src/toolbar/widget.tsx:80 packages/mainmenu-extension/src/index.ts:492 packages/mainmenu-extension/src/index.ts:494 packages/notebook-extension/src/index.ts:2377 packages/notebook-extension/src/index.ts:2384 packages/notebook-extension/src/index.ts:2395
 msgid "Restart the kernel"
 msgstr ""
 
 #: packages/cells/src/placeholder.ts:85
 msgid "Click to expand"
 msgstr ""
 
-#: packages/cells/src/widget.ts:1009 packages/cells/src/widget.ts:1094 packages/cells/src/widget.ts:1096 packages/cells/src/widget.ts:1466 packages/cells/src/widget.ts:1468
+#: packages/cells/src/widget.ts:1010 packages/cells/src/widget.ts:1012 packages/cells/src/widget.ts:1075 packages/cells/src/widget.ts:1099 packages/cells/src/widget.ts:1101 packages/cells/src/widget.ts:1225 packages/cells/src/widget.ts:1506 packages/cells/src/widget.ts:1508 packages/cells/src/widget.ts:1509 packages/cells/src/widget.ts:1646
 msgid "Code Cell Content"
 msgstr ""
 
-#: packages/cells/src/widget.ts:1010 packages/cells/src/widget.ts:1095 packages/cells/src/widget.ts:1097 packages/cells/src/widget.ts:1467 packages/cells/src/widget.ts:1469
+#: packages/cells/src/widget.ts:1011 packages/cells/src/widget.ts:1013 packages/cells/src/widget.ts:1076 packages/cells/src/widget.ts:1100 packages/cells/src/widget.ts:1102 packages/cells/src/widget.ts:1226 packages/cells/src/widget.ts:1507 packages/cells/src/widget.ts:1509 packages/cells/src/widget.ts:1510 packages/cells/src/widget.ts:1647
 msgid "Code Cell Content with Output"
 msgstr ""
 
-#: packages/cells/src/widget.ts:1875 packages/cells/src/widget.ts:1884
+#: packages/cells/src/widget.ts:1931 packages/cells/src/widget.ts:1933 packages/cells/src/widget.ts:1935 packages/cells/src/widget.ts:1936 packages/cells/src/widget.ts:2076
 msgid "Markdown Cell Content"
 msgstr ""
 
-#: packages/cells/src/widget.ts:2118 packages/cells/src/widget.ts:2127
+#: packages/cells/src/widget.ts:2174 packages/cells/src/widget.ts:2176 packages/cells/src/widget.ts:2178 packages/cells/src/widget.ts:2179 packages/cells/src/widget.ts:2319
 msgid "%1 cell hidden"
 msgid_plural "%1 cells hidden"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 
-#: packages/cells/src/widget.ts:2338 packages/cells/src/widget.ts:2347 packages/cells/src/widget.ts:2350
+#: packages/cells/src/widget.ts:2397 packages/cells/src/widget.ts:2399 packages/cells/src/widget.ts:2401 packages/cells/src/widget.ts:2402 packages/cells/src/widget.ts:2542
 msgid "Raw Cell Content"
 msgstr ""
 
 #: packages/celltags-extension/src/celltag.tsx:211
 msgid "Add Tag"
 msgstr ""
 
@@ -2884,921 +3140,1029 @@
 msgid "Revert changes to data"
 msgstr ""
 
 #: packages/codeeditor/src/jsoneditor.ts:64
 msgid "Commit changes to data"
 msgstr ""
 
-#: packages/codeeditor/src/lineCol.tsx:131
+#: packages/codeeditor/src/lineCol.tsx:141
 msgid "Go to line number between 1 and %1"
 msgstr ""
 
-#: packages/codeeditor/src/lineCol.tsx:229
+#: packages/codeeditor/src/lineCol.tsx:252
 msgid "Ln %1, Col %2"
 msgstr ""
 
-#: packages/codeeditor/src/lineCol.tsx:230
+#: packages/codeeditor/src/lineCol.tsx:253
 msgid "Go to line number…"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:608 packages/codemirror/src/extension.ts:609 packages/codemirror/src/extension.ts:610
-msgid "Auto Closing Brackets"
+#: packages/codemirror-extension/src/commands.ts:107
+msgid "Select Next Occurrence"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:617 packages/codemirror/src/extension.ts:618 packages/codemirror/src/extension.ts:619
-msgid "Code Folding"
+#: packages/codemirror-extension/src/commands.ts:68
+msgid "Delete the current line"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:629 packages/codemirror/src/extension.ts:630 packages/codemirror/src/extension.ts:631
-msgid "Cursor blinking rate"
+#: packages/codemirror-extension/src/commands.ts:80
+msgid "Toggle Block Comment"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:630 packages/codemirror/src/extension.ts:631 packages/codemirror/src/extension.ts:632
-msgid "Half-period in milliseconds used for cursor blinking. The default blink rate is 1200ms. By setting this to zero, blinking can be disabled."
+#: packages/codemirror-extension/src/commands.ts:81
+msgid "Toggles block commends in languages which support it (e.g. C, JavaScript)"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:641 packages/codemirror/src/extension.ts:642 packages/codemirror/src/extension.ts:643
-msgid "Highlight the active line"
+#: packages/codemirror-extension/src/commands.ts:95
+msgid "Toggle Comment"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:651 packages/codemirror/src/extension.ts:652 packages/codemirror/src/extension.ts:653
-msgid "Highlight trailing white spaces"
+#: packages/codemirror/src/extension.ts:1000 packages/codemirror/src/extension.ts:1024
+msgid "Folded lines"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:660 packages/codemirror/src/extension.ts:661 packages/codemirror/src/extension.ts:662
-msgid "Highlight white spaces"
+#: packages/codemirror/src/extension.ts:1001 packages/codemirror/src/extension.ts:1025
+msgid "Unfolded lines"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:674 packages/codemirror/src/extension.ts:675 packages/codemirror/src/extension.ts:676
-msgid "Indentation unit"
+#: packages/codemirror/src/extension.ts:1002 packages/codemirror/src/extension.ts:1026
+msgid "to"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:675 packages/codemirror/src/extension.ts:676 packages/codemirror/src/extension.ts:677
-msgid "The indentation is a `Tab` or the number of spaces. This defaults to 4 spaces."
+#: packages/codemirror/src/extension.ts:1003 packages/codemirror/src/extension.ts:1027
+msgid "folded code"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:702 packages/codemirror/src/extension.ts:703 packages/codemirror/src/extension.ts:704
-msgid "Line Numbers"
+#: packages/codemirror/src/extension.ts:1004 packages/codemirror/src/extension.ts:1028
+msgid "unfold"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:711 packages/codemirror/src/extension.ts:712 packages/codemirror/src/extension.ts:713
-msgid "Line Wrap"
+#: packages/codemirror/src/extension.ts:1005 packages/codemirror/src/extension.ts:1029
+msgid "Fold line"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:720 packages/codemirror/src/extension.ts:721 packages/codemirror/src/extension.ts:727 packages/fileeditor-extension/src/commands.ts:421 packages/fileeditor-extension/src/commands.ts:422 packages/fileeditor-extension/src/commands.ts:428 packages/fileeditor-extension/src/commands.ts:429 packages/mainmenu-extension/src/index.ts:588
-msgid "Match Brackets"
+#: packages/codemirror/src/extension.ts:1006 packages/codemirror/src/extension.ts:1030
+msgid "Unfold line"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:733 packages/codemirror/src/extension.ts:734 packages/codemirror/src/extension.ts:740
-msgid "Rectangular selection"
+#: packages/codemirror/src/extension.ts:1007 packages/codemirror/src/extension.ts:983
+msgid "CodeMirror theme"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:734 packages/codemirror/src/extension.ts:735 packages/codemirror/src/extension.ts:741
-msgid "Rectangular (block) selection can be created by dragging the mouse pointer while holding the left mouse button and the Alt key. When the Alt key is pressed, a crosshair cursor will appear, indicating that the rectangular selection mode is active."
+#: packages/codemirror/src/extension.ts:1008 packages/codemirror/src/extension.ts:1032
+msgid "Go to line"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:759 packages/codemirror/src/extension.ts:760 packages/codemirror/src/extension.ts:766
-msgid "Rulers"
+#: packages/codemirror/src/extension.ts:1009 packages/codemirror/src/extension.ts:1033
+msgid "go"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:778 packages/codemirror/src/extension.ts:779 packages/codemirror/src/extension.ts:785
-msgid "Smart Indentation"
+#: packages/codemirror/src/extension.ts:1010 packages/codemirror/src/extension.ts:1034 packages/documentsearch/src/searchview.tsx:173 packages/documentsearch/src/searchview.tsx:178
+msgid "Find"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:790 packages/codemirror/src/extension.ts:791 packages/codemirror/src/extension.ts:797
-msgid "Tab size"
+#: packages/codemirror/src/extension.ts:1011 packages/codemirror/src/extension.ts:1035 packages/documentsearch/src/searchview.tsx:236 packages/documentsearch/src/searchview.tsx:240 packages/documentsearch/src/searchview.tsx:267
+msgid "Replace"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:802 packages/codemirror/src/extension.ts:816 packages/codemirror/src/extension.ts:822
-msgid "Multiple selections"
+#: packages/codemirror/src/extension.ts:1012 packages/codemirror/src/extension.ts:1036
+msgid "next"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:817 packages/codemirror/src/extension.ts:831 packages/codemirror/src/extension.ts:837
-msgid "Custom editor styles"
+#: packages/codemirror/src/extension.ts:1013 packages/codemirror/src/extension.ts:1037
+msgid "previous"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:822 packages/codemirror/src/extension.ts:836 packages/codemirror/src/extension.ts:842
-msgid "Font Family"
+#: packages/codemirror/src/extension.ts:1014 packages/codemirror/src/extension.ts:1038
+msgid "all"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:828 packages/codemirror/src/extension.ts:842 packages/codemirror/src/extension.ts:848
-msgid "Font Size"
+#: packages/codemirror/src/extension.ts:1015 packages/codemirror/src/extension.ts:1039
+msgid "match case"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:832 packages/codemirror/src/extension.ts:846 packages/codemirror/src/extension.ts:852
-msgid "Line Height"
+#: packages/codemirror/src/extension.ts:1016 packages/codemirror/src/extension.ts:1040
+msgid "replace"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:852 packages/codemirror/src/extension.ts:866 packages/codemirror/src/extension.ts:872
-msgid "CodeMirror theme"
+#: packages/codemirror/src/extension.ts:1017 packages/codemirror/src/extension.ts:1041
+msgid "replace all"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:865 packages/codemirror/src/extension.ts:879 packages/codemirror/src/extension.ts:885
+#: packages/codemirror/src/extension.ts:1018 packages/codemirror/src/extension.ts:1042
+msgid "close"
+msgstr ""
+
+#: packages/codemirror/src/extension.ts:1019 packages/codemirror/src/extension.ts:1043
+msgid "current match"
+msgstr ""
+
+#: packages/codemirror/src/extension.ts:1020 packages/codemirror/src/extension.ts:1044
+msgid "replaced $ matches"
+msgstr ""
+
+#: packages/codemirror/src/extension.ts:1020 packages/codemirror/src/extension.ts:996
 msgid "Control character"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:867 packages/codemirror/src/extension.ts:881 packages/codemirror/src/extension.ts:887
+#: packages/codemirror/src/extension.ts:1021 packages/codemirror/src/extension.ts:1045
+msgid "replaced match on line $"
+msgstr ""
+
+#: packages/codemirror/src/extension.ts:1022 packages/codemirror/src/extension.ts:1046
+msgid "on line"
+msgstr ""
+
+#: packages/codemirror/src/extension.ts:1022 packages/codemirror/src/extension.ts:998
 msgid "Selection deleted"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:869 packages/codemirror/src/extension.ts:883 packages/codemirror/src/extension.ts:889
-msgid "Folded lines"
+#: packages/codemirror/src/extension.ts:1024 packages/codemirror/src/extension.ts:1048
+msgid "Completions"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:870 packages/codemirror/src/extension.ts:884 packages/codemirror/src/extension.ts:890
-msgid "Unfolded lines"
+#: packages/codemirror/src/extension.ts:1026 packages/codemirror/src/extension.ts:1050
+msgid "Diagnostics"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:871 packages/codemirror/src/extension.ts:885 packages/codemirror/src/extension.ts:891
-msgid "to"
+#: packages/codemirror/src/extension.ts:1027 packages/codemirror/src/extension.ts:1051
+msgid "No diagnostics"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:872 packages/codemirror/src/extension.ts:886 packages/codemirror/src/extension.ts:892
-msgid "folded code"
+#: packages/codemirror/src/extension.ts:618 packages/codemirror/src/extension.ts:619
+msgid "Auto Closing Brackets"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:873 packages/codemirror/src/extension.ts:887 packages/codemirror/src/extension.ts:893
-msgid "unfold"
+#: packages/codemirror/src/extension.ts:627 packages/codemirror/src/extension.ts:628
+msgid "Code Folding"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:874 packages/codemirror/src/extension.ts:888 packages/codemirror/src/extension.ts:894
-msgid "Fold line"
+#: packages/codemirror/src/extension.ts:639 packages/codemirror/src/extension.ts:640
+msgid "Cursor blinking rate"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:875 packages/codemirror/src/extension.ts:889 packages/codemirror/src/extension.ts:895
-msgid "Unfold line"
+#: packages/codemirror/src/extension.ts:640 packages/codemirror/src/extension.ts:641
+msgid "Half-period in milliseconds used for cursor blinking. The default blink rate is 1200ms. By setting this to zero, blinking can be disabled."
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:877 packages/codemirror/src/extension.ts:891 packages/codemirror/src/extension.ts:897
-msgid "Go to line"
+#: packages/codemirror/src/extension.ts:651 packages/codemirror/src/extension.ts:652
+msgid "Highlight the active line"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:878 packages/codemirror/src/extension.ts:892 packages/codemirror/src/extension.ts:898
-msgid "go"
+#: packages/codemirror/src/extension.ts:660 packages/codemirror/src/extension.ts:661
+msgid "Highlight special characters"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:879 packages/codemirror/src/extension.ts:893 packages/codemirror/src/extension.ts:899 packages/documentsearch/src/searchview.tsx:154 packages/documentsearch/src/searchview.tsx:159 packages/documentsearch/src/searchview.tsx:163 packages/documentsearch/src/searchview.tsx:168
-msgid "Find"
+#: packages/codemirror/src/extension.ts:670 packages/codemirror/src/extension.ts:671
+msgid "Highlight trailing white spaces"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:880 packages/codemirror/src/extension.ts:894 packages/codemirror/src/extension.ts:900 packages/documentsearch/src/searchview.tsx:217 packages/documentsearch/src/searchview.tsx:221 packages/documentsearch/src/searchview.tsx:226 packages/documentsearch/src/searchview.tsx:230 packages/documentsearch/src/searchview.tsx:248 packages/documentsearch/src/searchview.tsx:257
-msgid "Replace"
+#: packages/codemirror/src/extension.ts:679 packages/codemirror/src/extension.ts:680
+msgid "Highlight white spaces"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:881 packages/codemirror/src/extension.ts:895 packages/codemirror/src/extension.ts:901
-msgid "next"
+#: packages/codemirror/src/extension.ts:693 packages/codemirror/src/extension.ts:694
+msgid "Indentation unit"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:882 packages/codemirror/src/extension.ts:896 packages/codemirror/src/extension.ts:902
-msgid "previous"
+#: packages/codemirror/src/extension.ts:694 packages/codemirror/src/extension.ts:695
+msgid "The indentation is a `Tab` or the number of spaces. This defaults to 4 spaces."
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:883 packages/codemirror/src/extension.ts:897 packages/codemirror/src/extension.ts:903
-msgid "all"
+#: packages/codemirror/src/extension.ts:730 packages/codemirror/src/extension.ts:755
+msgid "Line Numbers"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:884 packages/codemirror/src/extension.ts:898 packages/codemirror/src/extension.ts:904
-msgid "match case"
+#: packages/codemirror/src/extension.ts:739 packages/codemirror/src/extension.ts:764
+msgid "Line Wrap"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:885 packages/codemirror/src/extension.ts:899 packages/codemirror/src/extension.ts:905
-msgid "replace"
+#: packages/codemirror/src/extension.ts:753 packages/codemirror/src/extension.ts:778 packages/fileeditor-extension/src/commands.ts:422 packages/fileeditor-extension/src/commands.ts:423 packages/fileeditor-extension/src/commands.ts:429 packages/fileeditor-extension/src/commands.ts:430 packages/mainmenu-extension/src/index.ts:584 packages/mainmenu-extension/src/index.ts:588
+msgid "Match Brackets"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:886 packages/codemirror/src/extension.ts:900 packages/codemirror/src/extension.ts:906
-msgid "replace all"
+#: packages/codemirror/src/extension.ts:766 packages/codemirror/src/extension.ts:791
+msgid "Rectangular selection"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:887 packages/codemirror/src/extension.ts:901 packages/codemirror/src/extension.ts:907
-msgid "close"
+#: packages/codemirror/src/extension.ts:767 packages/codemirror/src/extension.ts:792
+msgid "Rectangular (block) selection can be created by dragging the mouse pointer while holding the left mouse button and the Alt key. When the Alt key is pressed, a crosshair cursor will appear, indicating that the rectangular selection mode is active."
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:888 packages/codemirror/src/extension.ts:902 packages/codemirror/src/extension.ts:908
-msgid "current match"
+#: packages/codemirror/src/extension.ts:792 packages/codemirror/src/extension.ts:817
+msgid "Rulers"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:889 packages/codemirror/src/extension.ts:903 packages/codemirror/src/extension.ts:909
-msgid "replaced $ matches"
+#: packages/codemirror/src/extension.ts:860 packages/codemirror/src/extension.ts:884
+msgid "Smart Indentation"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:890 packages/codemirror/src/extension.ts:904 packages/codemirror/src/extension.ts:910
-msgid "replaced match on line $"
+#: packages/codemirror/src/extension.ts:908 packages/codemirror/src/extension.ts:932
+msgid "Tab size"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:891 packages/codemirror/src/extension.ts:905 packages/codemirror/src/extension.ts:911
-msgid "on line"
+#: packages/codemirror/src/extension.ts:933 packages/codemirror/src/extension.ts:957
+msgid "Multiple selections"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:893 packages/codemirror/src/extension.ts:907 packages/codemirror/src/extension.ts:913
-msgid "Completions"
+#: packages/codemirror/src/extension.ts:948 packages/codemirror/src/extension.ts:972
+msgid "Custom editor styles"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:895 packages/codemirror/src/extension.ts:909 packages/codemirror/src/extension.ts:915
-msgid "Diagnostics"
+#: packages/codemirror/src/extension.ts:953 packages/codemirror/src/extension.ts:977
+msgid "Font Family"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:896 packages/codemirror/src/extension.ts:910 packages/codemirror/src/extension.ts:916
-msgid "No diagnostics"
+#: packages/codemirror/src/extension.ts:959 packages/codemirror/src/extension.ts:983
+msgid "Font Size"
+msgstr ""
+
+#: packages/codemirror/src/extension.ts:963 packages/codemirror/src/extension.ts:987
+msgid "Line Height"
+msgstr ""
+
+#: packages/codemirror/src/language.ts:1003 packages/codemirror/src/language.ts:996
+msgid "IDL"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1006
+#: packages/codemirror/src/language.ts:1006 packages/codemirror/src/language.ts:1013
 msgid "JSON-LD"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1017
+#: packages/codemirror/src/language.ts:1017 packages/codemirror/src/language.ts:1024
 msgid "Jinja2"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1027
+#: packages/codemirror/src/language.ts:1027 packages/codemirror/src/language.ts:1034
 msgid "Julia"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1037
+#: packages/codemirror/src/language.ts:1037 packages/codemirror/src/language.ts:1044
 msgid "Kotlin"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1047
+#: packages/codemirror/src/language.ts:1047 packages/codemirror/src/language.ts:1054
 msgid "LESS"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1057
+#: packages/codemirror/src/language.ts:1057 packages/codemirror/src/language.ts:1064
 msgid "LiveScript"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1068
+#: packages/codemirror/src/language.ts:1068 packages/codemirror/src/language.ts:1075
 msgid "Lua"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1078
+#: packages/codemirror/src/language.ts:1078 packages/codemirror/src/language.ts:1085
 msgid "mIRC"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1087
+#: packages/codemirror/src/language.ts:1087 packages/codemirror/src/language.ts:1094
 msgid "Mathematica"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1097
+#: packages/codemirror/src/language.ts:1097 packages/codemirror/src/language.ts:1104
 msgid "Modelica"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1107
+#: packages/codemirror/src/language.ts:1107 packages/codemirror/src/language.ts:1114
 msgid "MUMPS"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1117
+#: packages/codemirror/src/language.ts:1117 packages/codemirror/src/language.ts:1124
 msgid "mbox"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1127
+#: packages/codemirror/src/language.ts:1127 packages/codemirror/src/language.ts:1134
 msgid "Nginx"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1137
+#: packages/codemirror/src/language.ts:1137 packages/codemirror/src/language.ts:1144
 msgid "NSIS"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1147
+#: packages/codemirror/src/language.ts:1147 packages/codemirror/src/language.ts:1154
 msgid "NTriples"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1161
+#: packages/codemirror/src/language.ts:1161 packages/codemirror/src/language.ts:1168
 msgid "Objective-C"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1172
+#: packages/codemirror/src/language.ts:1172 packages/codemirror/src/language.ts:1179
 msgid "Objective-C++"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1183
+#: packages/codemirror/src/language.ts:1183 packages/codemirror/src/language.ts:1190
 msgid "OCaml"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1193
+#: packages/codemirror/src/language.ts:1193 packages/codemirror/src/language.ts:1200
 msgid "Octave"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1203
+#: packages/codemirror/src/language.ts:1203 packages/codemirror/src/language.ts:1210
 msgid "Oz"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1213
+#: packages/codemirror/src/language.ts:1213 packages/codemirror/src/language.ts:1220
 msgid "Pascal"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1223
+#: packages/codemirror/src/language.ts:1223 packages/codemirror/src/language.ts:1230
 msgid "Perl"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1233
+#: packages/codemirror/src/language.ts:1233 packages/codemirror/src/language.ts:1240
 msgid "Pig"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1243
+#: packages/codemirror/src/language.ts:1243 packages/codemirror/src/language.ts:1250
 msgid "PowerShell"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1253
+#: packages/codemirror/src/language.ts:1253 packages/codemirror/src/language.ts:1260
 msgid "Properties files"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1264
+#: packages/codemirror/src/language.ts:1264 packages/codemirror/src/language.ts:1271
 msgid "ProtoBuf"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1274
+#: packages/codemirror/src/language.ts:1274 packages/codemirror/src/language.ts:1281
 msgid "Puppet"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1284
+#: packages/codemirror/src/language.ts:1284 packages/codemirror/src/language.ts:1291
 msgid "Q"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1294
+#: packages/codemirror/src/language.ts:1294 packages/codemirror/src/language.ts:1301
 msgid "R"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1305
+#: packages/codemirror/src/language.ts:1305 packages/codemirror/src/language.ts:1312
 msgid "RPM Changes"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1314
+#: packages/codemirror/src/language.ts:1314 packages/codemirror/src/language.ts:1321
 msgid "RPM Spec"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1324
+#: packages/codemirror/src/language.ts:1324 packages/codemirror/src/language.ts:1331
 msgid "Ruby"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1335
+#: packages/codemirror/src/language.ts:1335 packages/codemirror/src/language.ts:1342
 msgid "SAS"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1345
+#: packages/codemirror/src/language.ts:1345 packages/codemirror/src/language.ts:1352
 msgid "Scala"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1355
+#: packages/codemirror/src/language.ts:1355 packages/codemirror/src/language.ts:1362
 msgid "Scheme"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1365
+#: packages/codemirror/src/language.ts:1365 packages/codemirror/src/language.ts:1372
 msgid "SCSS"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1375
+#: packages/codemirror/src/language.ts:1375 packages/codemirror/src/language.ts:1382
 msgid "Shell"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1387
+#: packages/codemirror/src/language.ts:1387 packages/codemirror/src/language.ts:1394
 msgid "Sieve"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1397
+#: packages/codemirror/src/language.ts:1397 packages/codemirror/src/language.ts:1404
 msgid "Smalltalk"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1407
+#: packages/codemirror/src/language.ts:1407 packages/codemirror/src/language.ts:1414
 msgid "Solr"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1416
+#: packages/codemirror/src/language.ts:1416 packages/codemirror/src/language.ts:1423
 msgid "SML"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1426
+#: packages/codemirror/src/language.ts:1426 packages/codemirror/src/language.ts:1433
 msgid "SPARQL"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1437
+#: packages/codemirror/src/language.ts:1437 packages/codemirror/src/language.ts:1444
 msgid "Spreadsheet"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1447
+#: packages/codemirror/src/language.ts:1447 packages/codemirror/src/language.ts:1454
 msgid "Squirrel"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1457
+#: packages/codemirror/src/language.ts:1457 packages/codemirror/src/language.ts:1464
 msgid "Stylus"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1467
+#: packages/codemirror/src/language.ts:1467 packages/codemirror/src/language.ts:1474
 msgid "Swift"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1477
+#: packages/codemirror/src/language.ts:1477 packages/codemirror/src/language.ts:1484
 msgid "sTeX"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1486 packages/notebook-extension/src/index.ts:3678 packages/notebook-extension/src/index.ts:3684 packages/notebook-extension/src/index.ts:3703
+#: packages/codemirror/src/language.ts:1486 packages/codemirror/src/language.ts:1493 packages/notebook-extension/src/index.ts:3800 packages/notebook-extension/src/index.ts:3807 packages/notebook-extension/src/index.ts:3866
 msgid "LaTeX"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1497
+#: packages/codemirror/src/language.ts:1497 packages/codemirror/src/language.ts:1504
 msgid "SystemVerilog"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1507
+#: packages/codemirror/src/language.ts:1507 packages/codemirror/src/language.ts:1514
 msgid "Tcl"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1517
+#: packages/codemirror/src/language.ts:1517 packages/codemirror/src/language.ts:1524
 msgid "Textile"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1527
+#: packages/codemirror/src/language.ts:1527 packages/codemirror/src/language.ts:1534
 msgid "TiddlyWiki"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1536
+#: packages/codemirror/src/language.ts:1536 packages/codemirror/src/language.ts:1543
 msgid "Tiki wiki"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1545
+#: packages/codemirror/src/language.ts:1545 packages/codemirror/src/language.ts:1552
 msgid "TOML"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1555
+#: packages/codemirror/src/language.ts:1555 packages/codemirror/src/language.ts:1562
 msgid "troff"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1565
+#: packages/codemirror/src/language.ts:1565 packages/codemirror/src/language.ts:1572
 msgid "TTCN"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1575
+#: packages/codemirror/src/language.ts:1575 packages/codemirror/src/language.ts:1582
 msgid "TTCN_CFG"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1585
+#: packages/codemirror/src/language.ts:1585 packages/codemirror/src/language.ts:1592
 msgid "Turtle"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1595
+#: packages/codemirror/src/language.ts:1595 packages/codemirror/src/language.ts:1602
 msgid "Web IDL"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1605
+#: packages/codemirror/src/language.ts:1605 packages/codemirror/src/language.ts:1612
 msgid "VB.NET"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1615
+#: packages/codemirror/src/language.ts:1615 packages/codemirror/src/language.ts:1622
 msgid "VBScript"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1625
+#: packages/codemirror/src/language.ts:1625 packages/codemirror/src/language.ts:1632
 msgid "Velocity"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1635
+#: packages/codemirror/src/language.ts:1635 packages/codemirror/src/language.ts:1642
 msgid "Verilog"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1645
+#: packages/codemirror/src/language.ts:1645 packages/codemirror/src/language.ts:1652
 msgid "VHDL"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1655
+#: packages/codemirror/src/language.ts:1655 packages/codemirror/src/language.ts:1662
 msgid "XQuery"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1665
+#: packages/codemirror/src/language.ts:1665 packages/codemirror/src/language.ts:1672
 msgid "Yacas"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1675
+#: packages/codemirror/src/language.ts:1675 packages/codemirror/src/language.ts:1682
 msgid "YAML"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1686
+#: packages/codemirror/src/language.ts:1686 packages/codemirror/src/language.ts:1693
 msgid "Z80"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1696
+#: packages/codemirror/src/language.ts:1696 packages/codemirror/src/language.ts:1703
 msgid "mscgen"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1706
+#: packages/codemirror/src/language.ts:1706 packages/codemirror/src/language.ts:1713
 msgid "xu"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:1716
+#: packages/codemirror/src/language.ts:1716 packages/codemirror/src/language.ts:1723
 msgid "msgenny"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:307
+#: packages/codemirror/src/language.ts:307 packages/codemirror/src/language.ts:308
 msgid "C"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:317
+#: packages/codemirror/src/language.ts:317 packages/codemirror/src/language.ts:318
 msgid "C++"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:327
+#: packages/codemirror/src/language.ts:327 packages/codemirror/src/language.ts:328
 msgid "CQL"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:336
+#: packages/codemirror/src/language.ts:336 packages/codemirror/src/language.ts:337
 msgid "CSS"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:346 packages/notebook-extension/src/index.ts:3677 packages/notebook-extension/src/index.ts:3683 packages/notebook-extension/src/index.ts:3702
+#: packages/codemirror/src/language.ts:346 packages/codemirror/src/language.ts:347 packages/notebook-extension/src/index.ts:3799 packages/notebook-extension/src/index.ts:3806 packages/notebook-extension/src/index.ts:3865
 msgid "HTML"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:357
+#: packages/codemirror/src/language.ts:357 packages/codemirror/src/language.ts:358
 msgid "Java"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:367
+#: packages/codemirror/src/language.ts:367 packages/codemirror/src/language.ts:368
 msgid "Javascript"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:384
+#: packages/codemirror/src/language.ts:384 packages/codemirror/src/language.ts:385
 msgid "JSON"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:395
+#: packages/codemirror/src/language.ts:395 packages/codemirror/src/language.ts:396
 msgid "JSX"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:405
+#: packages/codemirror/src/language.ts:405 packages/codemirror/src/language.ts:406
 msgid "MariaDB SQL"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:413 packages/notebook-extension/src/index.ts:3679 packages/notebook-extension/src/index.ts:3685 packages/notebook-extension/src/index.ts:3704 packages/notebook/src/default-toolbar.tsx:379
+#: packages/codemirror/src/language.ts:413 packages/codemirror/src/language.ts:414 packages/notebook-extension/src/index.ts:3801 packages/notebook-extension/src/index.ts:3808 packages/notebook-extension/src/index.ts:3867 packages/notebook/src/default-toolbar.tsx:379
 msgid "Markdown"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:423
+#: packages/codemirror/src/language.ts:423 packages/codemirror/src/language.ts:424
 msgid "MS SQL"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:431
+#: packages/codemirror/src/language.ts:431 packages/codemirror/src/language.ts:432
 msgid "MySQL"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:439
+#: packages/codemirror/src/language.ts:439 packages/codemirror/src/language.ts:440
 msgid "PHP"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:453
+#: packages/codemirror/src/language.ts:453 packages/codemirror/src/language.ts:454
 msgid "PLSQL"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:462
+#: packages/codemirror/src/language.ts:462 packages/codemirror/src/language.ts:463
 msgid "PostgreSQL"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:470
+#: packages/codemirror/src/language.ts:470 packages/codemirror/src/language.ts:471
 msgid "Python"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:481
+#: packages/codemirror/src/language.ts:481 packages/codemirror/src/language.ts:485
 msgid "ipython"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:493
+#: packages/codemirror/src/language.ts:493 packages/codemirror/src/language.ts:500
 msgid "Rust"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:503
+#: packages/codemirror/src/language.ts:503 packages/codemirror/src/language.ts:510
 msgid "SQL"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:512
+#: packages/codemirror/src/language.ts:512 packages/codemirror/src/language.ts:519
 msgid "SQLite"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:520
+#: packages/codemirror/src/language.ts:520 packages/codemirror/src/language.ts:527
 msgid "TSX"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:531
+#: packages/codemirror/src/language.ts:531 packages/codemirror/src/language.ts:538
 msgid "TypeScript"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:542
+#: packages/codemirror/src/language.ts:542 packages/codemirror/src/language.ts:549
 msgid "WebAssembly"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:552
+#: packages/codemirror/src/language.ts:552 packages/codemirror/src/language.ts:559
 msgid "XML"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:564
+#: packages/codemirror/src/language.ts:564 packages/codemirror/src/language.ts:571
 msgid "APL"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:574
+#: packages/codemirror/src/language.ts:574 packages/codemirror/src/language.ts:581
 msgid "PGP"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:590
+#: packages/codemirror/src/language.ts:590 packages/codemirror/src/language.ts:597
 msgid "ASN.1"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:600
+#: packages/codemirror/src/language.ts:600 packages/codemirror/src/language.ts:607
 msgid "Asterisk"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:610
+#: packages/codemirror/src/language.ts:610 packages/codemirror/src/language.ts:617
 msgid "Brainfuck"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:620
+#: packages/codemirror/src/language.ts:620 packages/codemirror/src/language.ts:627
 msgid "Cobol"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:630
+#: packages/codemirror/src/language.ts:630 packages/codemirror/src/language.ts:637
 msgid "C#"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:641
+#: packages/codemirror/src/language.ts:641 packages/codemirror/src/language.ts:648
 msgid "Clojure"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:651
+#: packages/codemirror/src/language.ts:651 packages/codemirror/src/language.ts:658
 msgid "ClojureScript"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:661
+#: packages/codemirror/src/language.ts:661 packages/codemirror/src/language.ts:668
 msgid "Closure Stylesheets (GSS)"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:671
+#: packages/codemirror/src/language.ts:671 packages/codemirror/src/language.ts:678
 msgid "CMake"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:682
+#: packages/codemirror/src/language.ts:682 packages/codemirror/src/language.ts:689
 msgid "CoffeeScript"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:697
+#: packages/codemirror/src/language.ts:697 packages/codemirror/src/language.ts:704
 msgid "Common Lisp"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:708
+#: packages/codemirror/src/language.ts:708 packages/codemirror/src/language.ts:715
 msgid "Cypher"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:718
+#: packages/codemirror/src/language.ts:718 packages/codemirror/src/language.ts:725
 msgid "Cython"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:728
+#: packages/codemirror/src/language.ts:728 packages/codemirror/src/language.ts:735
 msgid "Crystal"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:738
+#: packages/codemirror/src/language.ts:738 packages/codemirror/src/language.ts:745
 msgid "D"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:748
+#: packages/codemirror/src/language.ts:748 packages/codemirror/src/language.ts:755
 msgid "Dart"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:758
+#: packages/codemirror/src/language.ts:758 packages/codemirror/src/language.ts:765
 msgid "diff"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:768
+#: packages/codemirror/src/language.ts:768 packages/codemirror/src/language.ts:775
 msgid "Dockerfile"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:778
+#: packages/codemirror/src/language.ts:778 packages/codemirror/src/language.ts:785
 msgid "DTD"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:788
+#: packages/codemirror/src/language.ts:788 packages/codemirror/src/language.ts:795
 msgid "Dylan"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:798
+#: packages/codemirror/src/language.ts:798 packages/codemirror/src/language.ts:805
 msgid "EBNF"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:807
+#: packages/codemirror/src/language.ts:807 packages/codemirror/src/language.ts:814
 msgid "ECL"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:817
+#: packages/codemirror/src/language.ts:817 packages/codemirror/src/language.ts:824
 msgid "edn"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:827
+#: packages/codemirror/src/language.ts:827 packages/codemirror/src/language.ts:834
 msgid "Eiffel"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:837
+#: packages/codemirror/src/language.ts:837 packages/codemirror/src/language.ts:844
 msgid "Elm"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:847
+#: packages/codemirror/src/language.ts:847 packages/codemirror/src/language.ts:854
 msgid "Erlang"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:857
+#: packages/codemirror/src/language.ts:857 packages/codemirror/src/language.ts:864
 msgid "Esper"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:866
+#: packages/codemirror/src/language.ts:866 packages/codemirror/src/language.ts:873
 msgid "Factor"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:876
+#: packages/codemirror/src/language.ts:876 packages/codemirror/src/language.ts:883
 msgid "FCL"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:885
+#: packages/codemirror/src/language.ts:885 packages/codemirror/src/language.ts:892
 msgid "Forth"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:895
+#: packages/codemirror/src/language.ts:895 packages/codemirror/src/language.ts:902
 msgid "Fortran"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:905
+#: packages/codemirror/src/language.ts:905 packages/codemirror/src/language.ts:912
 msgid "F#"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:916
+#: packages/codemirror/src/language.ts:916 packages/codemirror/src/language.ts:923
 msgid "Gas"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:926
+#: packages/codemirror/src/language.ts:926 packages/codemirror/src/language.ts:933
 msgid "Gherkin"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:936
+#: packages/codemirror/src/language.ts:936 packages/codemirror/src/language.ts:943
 msgid "Go"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:946
+#: packages/codemirror/src/language.ts:946 packages/codemirror/src/language.ts:953
 msgid "Groovy"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:957
+#: packages/codemirror/src/language.ts:957 packages/codemirror/src/language.ts:964
 msgid "Haskell"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:967
+#: packages/codemirror/src/language.ts:967 packages/codemirror/src/language.ts:974
 msgid "Haxe"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:977
+#: packages/codemirror/src/language.ts:977 packages/codemirror/src/language.ts:984
 msgid "HXML"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:987
+#: packages/codemirror/src/language.ts:987 packages/codemirror/src/language.ts:994
 msgid "HTTP"
 msgstr ""
 
-#: packages/codemirror/src/language.ts:996
-msgid "IDL"
+#: packages/codemirror/src/theme.ts:234 packages/codemirror/src/theme.ts:238
+msgid "codemirror"
 msgstr ""
 
-#: packages/codemirror/src/theme.ts:215 packages/codemirror/src/theme.ts:225 packages/codemirror/src/theme.ts:229 packages/codemirror/src/theme.ts:234
-msgid "codemirror"
+#: packages/completer-extension/src/index.ts:138
+msgid "Previous"
+msgstr ""
+
+#: packages/completer-extension/src/index.ts:148 packages/debugger-extension/src/index.ts:908 packages/debugger-extension/src/index.ts:909
+msgid "Next"
+msgstr ""
+
+#: packages/completer-extension/src/index.ts:158
+msgid "Accept"
+msgstr ""
+
+#: packages/completer-extension/src/index.ts:192
+msgid "Next Inline Completion"
 msgstr ""
 
-#: packages/console-extension/src/foreign.ts:66 packages/console-extension/src/index.ts:262 packages/console-extension/src/index.ts:311 packages/console-extension/src/index.ts:530 packages/console/src/panel.ts:333 packages/launcher/src/widget.tsx:116 packages/launcher/src/widget.tsx:121
+#: packages/completer-extension/src/index.ts:202
+msgid "Previous Inline Completion"
+msgstr ""
+
+#: packages/completer-extension/src/index.ts:209
+msgid "Accept Inline Completion"
+msgstr ""
+
+#: packages/completer-extension/src/index.ts:216
+msgid "Invoke Inline Completer"
+msgstr ""
+
+#: packages/completer-extension/src/index.ts:263
+msgid "%1 provider"
+msgstr ""
+
+#: packages/completer-extension/src/index.ts:267
+msgid "Timeout"
+msgstr ""
+
+#: packages/completer-extension/src/index.ts:268
+msgid "Timeout for %1 provider (in milliseconds)."
+msgstr ""
+
+#: packages/completer-extension/src/index.ts:276
+msgid "Debouncer delay"
+msgstr ""
+
+#: packages/completer-extension/src/index.ts:278
+msgid "Time since the last key press to wait before requesting completions from %1 provider (in milliseconds)."
+msgstr ""
+
+#: packages/completer-extension/src/index.ts:285 packages/pluginmanager/src/widget.tsx:171
+msgid "Enabled"
+msgstr ""
+
+#: packages/completer-extension/src/index.ts:286
+msgid "Whether to fetch completions %1 provider."
+msgstr ""
+
+#: packages/completer/src/default/inlinehistoryprovider.ts:32
+msgid "History"
+msgstr ""
+
+#: packages/completer/src/default/inlinehistoryprovider.ts:43
+msgid "Maximum number of suggestions"
+msgstr ""
+
+#: packages/completer/src/default/inlinehistoryprovider.ts:44
+msgid "The maximum number of suggestions to retrieve from history."
+msgstr ""
+
+#: packages/completer/src/inline.ts:388
+msgid "%1/%2"
+msgstr ""
+
+#: packages/completer/src/inline.ts:393
+msgid "Provider: %1"
+msgstr ""
+
+#: packages/console-extension/src/foreign.ts:66 packages/console-extension/src/index.ts:262 packages/console-extension/src/index.ts:271 packages/console-extension/src/index.ts:275 packages/console-extension/src/index.ts:311 packages/console-extension/src/index.ts:320 packages/console-extension/src/index.ts:324 packages/console-extension/src/index.ts:530 packages/console-extension/src/index.ts:539 packages/console-extension/src/index.ts:542 packages/console/src/panel.ts:333 packages/console/src/panel.ts:341 packages/launcher/src/widget.tsx:116 packages/launcher/src/widget.tsx:121
 msgid "Console"
 msgstr ""
 
 #: packages/console-extension/src/foreign.ts:80
 msgid "Show All Kernel Activity"
 msgstr "Arată Toată Activitatea Kernel-ului"
 
-#: packages/console-extension/src/index.ts:464
+#: packages/console-extension/src/index.ts:464 packages/console-extension/src/index.ts:473 packages/console-extension/src/index.ts:478
 msgid "Auto Close Brackets for Code Console Prompt"
 msgstr ""
 
-#: packages/console-extension/src/index.ts:490
+#: packages/console-extension/src/index.ts:490 packages/console-extension/src/index.ts:499 packages/console-extension/src/index.ts:503
 msgid "Open a console for the provided `path`."
 msgstr ""
 
-#: packages/console-extension/src/index.ts:519
+#: packages/console-extension/src/index.ts:519 packages/console-extension/src/index.ts:528 packages/console-extension/src/index.ts:531
 msgid "New Console"
 msgstr ""
 
-#: packages/console-extension/src/index.ts:554
+#: packages/console-extension/src/index.ts:554 packages/console-extension/src/index.ts:631 packages/console-extension/src/index.ts:634
 msgid "Clear Console Cells"
 msgstr ""
 
-#: packages/console-extension/src/index.ts:566
+#: packages/console-extension/src/index.ts:566 packages/console-extension/src/index.ts:643 packages/console-extension/src/index.ts:646
 msgid "Run Cell (unforced)"
 msgstr ""
 
-#: packages/console-extension/src/index.ts:578
+#: packages/console-extension/src/index.ts:578 packages/console-extension/src/index.ts:655 packages/console-extension/src/index.ts:658
 msgid "Run Cell (forced)"
 msgstr ""
 
-#: packages/console-extension/src/index.ts:590
+#: packages/console-extension/src/index.ts:590 packages/console-extension/src/index.ts:667 packages/console-extension/src/index.ts:670
 msgid "Insert Line Break"
 msgstr ""
 
-#: packages/console-extension/src/index.ts:602
+#: packages/console-extension/src/index.ts:593 packages/console-extension/src/index.ts:596 packages/fileeditor-extension/src/commands.ts:853 packages/fileeditor-extension/src/commands.ts:854 packages/mainmenu-extension/src/index.ts:277 packages/notebook-extension/src/index.ts:3122 packages/notebook-extension/src/index.ts:3129 packages/notebook-extension/src/index.ts:3152
+msgid "Undo"
+msgstr ""
+
+#: packages/console-extension/src/index.ts:602 packages/console-extension/src/index.ts:679 packages/console-extension/src/index.ts:682
 msgid "Replace Selection in Console"
 msgstr ""
 
-#: packages/console-extension/src/index.ts:615 packages/mainmenu-extension/src/index.ts:468 packages/notebook-extension/src/index.ts:2452 packages/notebook-extension/src/index.ts:2457 packages/notebook-extension/src/index.ts:2476
+#: packages/console-extension/src/index.ts:615 packages/console-extension/src/index.ts:692 packages/console-extension/src/index.ts:695 packages/mainmenu-extension/src/index.ts:466 packages/mainmenu-extension/src/index.ts:468 packages/notebook-extension/src/index.ts:2528 packages/notebook-extension/src/index.ts:2535 packages/notebook-extension/src/index.ts:2546
 msgid "Interrupt Kernel"
 msgstr ""
 
-#: packages/console-extension/src/index.ts:630 packages/mainmenu-extension/src/index.ts:493 packages/notebook-extension/src/index.ts:2320 packages/notebook-extension/src/index.ts:2324 packages/notebook-extension/src/index.ts:2343
+#: packages/console-extension/src/index.ts:627 packages/console-extension/src/index.ts:630 packages/fileeditor-extension/src/commands.ts:883 packages/fileeditor-extension/src/commands.ts:884 packages/fileeditor-extension/src/commands.ts:885 packages/mainmenu-extension/src/index.ts:287 packages/mainmenu-extension/src/index.ts:288 packages/notebook-extension/src/index.ts:3108 packages/notebook-extension/src/index.ts:3115 packages/notebook-extension/src/index.ts:3138
+msgid "Redo"
+msgstr ""
+
+#: packages/console-extension/src/index.ts:630 packages/console-extension/src/index.ts:707 packages/console-extension/src/index.ts:710 packages/mainmenu-extension/src/index.ts:491 packages/mainmenu-extension/src/index.ts:493 packages/notebook-extension/src/index.ts:2376 packages/notebook-extension/src/index.ts:2383 packages/notebook-extension/src/index.ts:2394
 msgid "Restart Kernel…"
 msgstr ""
 
-#: packages/console-extension/src/index.ts:642 packages/lsp-extension/src/index.ts:275 packages/lsp-extension/src/index.ts:298 packages/mainmenu-extension/src/index.ts:375 packages/mainmenu-extension/src/index.ts:385 packages/running/src/index.tsx:161 packages/terminal-extension/src/index.ts:322
+#: packages/console-extension/src/index.ts:642 packages/console-extension/src/index.ts:719 packages/console-extension/src/index.ts:722 packages/lsp-extension/src/index.ts:303 packages/mainmenu-extension/src/index.ts:371 packages/mainmenu-extension/src/index.ts:375 packages/mainmenu-extension/src/index.ts:381 packages/mainmenu-extension/src/index.ts:385 packages/running/src/index.tsx:161 packages/running/src/index.tsx:221 packages/terminal-extension/src/index.ts:322
 msgid "Shut Down"
 msgstr ""
 
-#: packages/console-extension/src/index.ts:654
+#: packages/console-extension/src/index.ts:654 packages/console-extension/src/index.ts:731 packages/console-extension/src/index.ts:734
 msgid "Close and Shut Down…"
 msgstr ""
 
-#: packages/console-extension/src/index.ts:661
+#: packages/console-extension/src/index.ts:661 packages/console-extension/src/index.ts:738 packages/console-extension/src/index.ts:741
 msgid "Shut down the console?"
 msgstr ""
 
-#: packages/console-extension/src/index.ts:662 packages/notebook-extension/src/index.ts:2357 packages/notebook-extension/src/index.ts:2362 packages/notebook-extension/src/index.ts:2381
+#: packages/console-extension/src/index.ts:662 packages/console-extension/src/index.ts:739 packages/console-extension/src/index.ts:742 packages/notebook-extension/src/index.ts:2414 packages/notebook-extension/src/index.ts:2421 packages/notebook-extension/src/index.ts:2432
 msgid "Are you sure you want to close \"%1\"?"
 msgstr ""
 
-#: packages/console-extension/src/index.ts:668
+#: packages/console-extension/src/index.ts:668 packages/console-extension/src/index.ts:745 packages/console-extension/src/index.ts:748
 msgid "Cancel console Shut Down"
 msgstr ""
 
-#: packages/console-extension/src/index.ts:671
+#: packages/console-extension/src/index.ts:671 packages/console-extension/src/index.ts:748 packages/console-extension/src/index.ts:751
 msgid "Confirm console Shut Down"
 msgstr ""
 
-#: packages/console-extension/src/index.ts:684 packages/console-extension/src/index.ts:691
+#: packages/console-extension/src/index.ts:691 packages/console-extension/src/index.ts:768 packages/console-extension/src/index.ts:771
 msgid "Inject some code in a console."
 msgstr ""
 
-#: packages/console-extension/src/index.ts:705 packages/console-extension/src/index.ts:712 packages/mainmenu-extension/src/index.ts:519 packages/notebook-extension/src/index.ts:3059 packages/notebook-extension/src/index.ts:3065 packages/notebook-extension/src/index.ts:3084
+#: packages/console-extension/src/index.ts:712 packages/console-extension/src/index.ts:789 packages/console-extension/src/index.ts:792 packages/mainmenu-extension/src/index.ts:518 packages/mainmenu-extension/src/index.ts:519 packages/notebook-extension/src/index.ts:3136 packages/notebook-extension/src/index.ts:3143 packages/notebook-extension/src/index.ts:3166
 msgid "Change Kernel…"
 msgstr ""
 
-#: packages/console-extension/src/index.ts:717 packages/console-extension/src/index.ts:724 packages/mainmenu-extension/src/index.ts:754 packages/notebook-extension/src/index.ts:3070 packages/notebook-extension/src/index.ts:3076 packages/notebook-extension/src/index.ts:3095
+#: packages/console-extension/src/index.ts:724 packages/console-extension/src/index.ts:801 packages/console-extension/src/index.ts:804 packages/mainmenu-extension/src/index.ts:752 packages/mainmenu-extension/src/index.ts:754 packages/notebook-extension/src/index.ts:3147 packages/notebook-extension/src/index.ts:3154 packages/notebook-extension/src/index.ts:3177
 msgid "Get Kernel"
 msgstr ""
 
-#: packages/console-extension/src/index.ts:799 packages/console-extension/src/index.ts:806
+#: packages/console-extension/src/index.ts:806 packages/console-extension/src/index.ts:893 packages/console-extension/src/index.ts:907
 msgid "Execute with Shift+Enter"
 msgstr ""
 
-#: packages/console-extension/src/index.ts:800 packages/console-extension/src/index.ts:807
+#: packages/console-extension/src/index.ts:807 packages/console-extension/src/index.ts:894 packages/console-extension/src/index.ts:908
 msgid "Execute with Enter"
 msgstr ""
 
-#: packages/console-extension/src/index.ts:844 packages/console-extension/src/index.ts:851 packages/fileeditor-extension/src/commands.ts:1005 packages/fileeditor-extension/src/commands.ts:1012 packages/notebook-extension/src/index.ts:1974 packages/notebook-extension/src/index.ts:1977 packages/notebook-extension/src/index.ts:1996
+#: packages/console-extension/src/index.ts:851 packages/console-extension/src/index.ts:938 packages/console-extension/src/index.ts:952 packages/fileeditor-extension/src/commands.ts:1010 packages/fileeditor-extension/src/commands.ts:1012 packages/fileeditor-extension/src/commands.ts:1041 packages/notebook-extension/src/index.ts:2027 packages/notebook-extension/src/index.ts:2034 packages/notebook-extension/src/index.ts:2045
 msgid "Display the completion helper."
 msgstr ""
 
-#: packages/console-extension/src/index.ts:855 packages/console-extension/src/index.ts:862 packages/fileeditor-extension/src/commands.ts:1016 packages/fileeditor-extension/src/commands.ts:1023 packages/notebook-extension/src/index.ts:1984 packages/notebook-extension/src/index.ts:1987 packages/notebook-extension/src/index.ts:2006
+#: packages/console-extension/src/index.ts:862 packages/console-extension/src/index.ts:949 packages/console-extension/src/index.ts:963 packages/fileeditor-extension/src/commands.ts:1021 packages/fileeditor-extension/src/commands.ts:1023 packages/fileeditor-extension/src/commands.ts:1052 packages/notebook-extension/src/index.ts:2037 packages/notebook-extension/src/index.ts:2044 packages/notebook-extension/src/index.ts:2055
 msgid "Select the completion suggestion."
 msgstr ""
 
-#: packages/console/src/panel.ts:316
+#: packages/console/src/panel.ts:316 packages/console/src/panel.ts:324
 msgid "Name: %1\n"
 msgstr ""
 
-#: packages/console/src/panel.ts:317
+#: packages/console/src/panel.ts:317 packages/console/src/panel.ts:325
 msgid "Directory: %1\n"
 msgstr ""
 
-#: packages/console/src/panel.ts:318
+#: packages/console/src/panel.ts:318 packages/console/src/panel.ts:326
 msgid "Kernel: %1"
 msgstr ""
 
-#: packages/console/src/panel.ts:321
+#: packages/console/src/panel.ts:321 packages/console/src/panel.ts:329
 msgid "\n"
 "Connected: %1"
 msgstr ""
 
-#: packages/console/src/panel.ts:328
+#: packages/console/src/panel.ts:328 packages/console/src/panel.ts:336
 msgid "\n"
 "Last Execution: %1"
 msgstr ""
 
-#: packages/console/src/panel.ts:66
+#: packages/console/src/panel.ts:66 packages/console/src/panel.ts:68
 msgid "Console %1"
 msgstr ""
 
 #: packages/csvviewer-extension/src/index.ts:134
 msgid "CSV Viewer"
 msgstr ""
 
-#: packages/csvviewer-extension/src/index.ts:212 packages/csvviewer-extension/src/index.ts:216 packages/csvviewer-extension/src/index.ts:219 packages/csvviewer-extension/src/index.ts:223 packages/csvviewer-extension/src/index.ts:362 packages/csvviewer-extension/src/index.ts:369 packages/csvviewer-extension/src/index.ts:370 packages/csvviewer-extension/src/index.ts:377
+#: packages/csvviewer-extension/src/index.ts:216 packages/csvviewer-extension/src/index.ts:223 packages/csvviewer-extension/src/index.ts:370 packages/csvviewer-extension/src/index.ts:376 packages/csvviewer-extension/src/index.ts:377 packages/csvviewer-extension/src/index.ts:383
 msgid "Go to Line"
 msgstr ""
 
-#: packages/csvviewer-extension/src/index.ts:284 packages/csvviewer-extension/src/index.ts:288
+#: packages/csvviewer-extension/src/index.ts:288 packages/csvviewer-extension/src/index.ts:294
 msgid "TSV Viewer"
 msgstr ""
 
 #: packages/csvviewer/src/toolbar.ts:119
 msgid "tab"
 msgstr ""
 
@@ -3810,92 +4174,104 @@
 msgid "hash"
 msgstr ""
 
 #: packages/csvviewer/src/toolbar.ts:127
 msgid "Delimiter: "
 msgstr ""
 
-#: packages/debugger-extension/src/index.ts:214 packages/debugger-extension/src/index.ts:215
+#: packages/debugger-extension/src/index.ts:1003
+msgid "Debugger section"
+msgstr ""
+
+#: packages/debugger-extension/src/index.ts:1005 packages/debugger-extension/src/index.ts:1017
+msgid "Debugger"
+msgstr ""
+
+#: packages/debugger-extension/src/index.ts:1010
+msgid "Debugger Panel"
+msgstr ""
+
+#: packages/debugger-extension/src/index.ts:217 packages/debugger-extension/src/index.ts:218
 msgid "Restart Kernel and Debug…"
 msgstr ""
 
-#: packages/debugger-extension/src/index.ts:373 packages/debugger-extension/src/index.ts:374
+#: packages/debugger-extension/src/index.ts:376 packages/debugger-extension/src/index.ts:377
 msgid "Inspect Variable"
 msgstr ""
 
-#: packages/debugger-extension/src/index.ts:440
+#: packages/debugger-extension/src/index.ts:443
 msgid "Render Variable"
 msgstr ""
 
-#: packages/debugger-extension/src/index.ts:441
+#: packages/debugger-extension/src/index.ts:444
 msgid "Render variable according to its mime type"
 msgstr ""
 
-#: packages/debugger-extension/src/index.ts:518
+#: packages/debugger-extension/src/index.ts:521
 msgid "Copy to Clipboard"
 msgstr ""
 
-#: packages/debugger-extension/src/index.ts:519
+#: packages/debugger-extension/src/index.ts:522
 msgid "Copy text representation of the value to clipboard"
 msgstr ""
 
-#: packages/debugger-extension/src/index.ts:536
+#: packages/debugger-extension/src/index.ts:539
 msgid "Copy Variable to Globals"
 msgstr ""
 
-#: packages/debugger-extension/src/index.ts:537
+#: packages/debugger-extension/src/index.ts:540
 msgid "Copy variable to globals scope"
 msgstr ""
 
-#: packages/debugger-extension/src/index.ts:687 packages/debugger-extension/src/index.ts:688 packages/debugger-extension/src/index.ts:694
-msgid "Evaluate Code"
+#: packages/debugger-extension/src/index.ts:723 packages/debugger-extension/src/index.ts:724
+msgid "Open Source"
 msgstr ""
 
-#: packages/debugger-extension/src/index.ts:695
-msgid "Evaluate"
+#: packages/debugger-extension/src/index.ts:733
+msgid "Start debugger?"
 msgstr ""
 
-#: packages/debugger-extension/src/index.ts:728 packages/debugger-extension/src/index.ts:733
-msgid "Continue"
+#: packages/debugger-extension/src/index.ts:734
+msgid "The debugger service is needed to open the source %1"
 msgstr ""
 
-#: packages/debugger-extension/src/index.ts:729 packages/debugger-extension/src/index.ts:734
-msgid "Pause"
+#: packages/debugger-extension/src/index.ts:740
+msgid "Start debugger"
 msgstr ""
 
-#: packages/debugger-extension/src/index.ts:753 packages/debugger-extension/src/index.ts:754
-msgid "Terminate"
+#: packages/debugger-extension/src/index.ts:831 packages/debugger-extension/src/index.ts:832 packages/debugger-extension/src/index.ts:838
+msgid "Evaluate Code"
 msgstr ""
 
-#: packages/debugger-extension/src/index.ts:764 packages/debugger-extension/src/index.ts:765
-msgid "Next"
+#: packages/debugger-extension/src/index.ts:839
+msgid "Evaluate"
 msgstr ""
 
-#: packages/debugger-extension/src/index.ts:774 packages/debugger-extension/src/index.ts:775
-msgid "Step In"
+#: packages/debugger-extension/src/index.ts:872 packages/debugger-extension/src/index.ts:877
+msgid "Continue"
 msgstr ""
 
-#: packages/debugger-extension/src/index.ts:784 packages/debugger-extension/src/index.ts:785
-msgid "Step Out"
+#: packages/debugger-extension/src/index.ts:873 packages/debugger-extension/src/index.ts:878
+msgid "Pause"
 msgstr ""
 
-#: packages/debugger-extension/src/index.ts:811
-msgid "Select a filter for breakpoints on exception"
+#: packages/debugger-extension/src/index.ts:897 packages/debugger-extension/src/index.ts:898
+msgid "Terminate"
 msgstr ""
 
-#: packages/debugger-extension/src/index.ts:859
-msgid "Debugger section"
+#: packages/debugger-extension/src/index.ts:918 packages/debugger-extension/src/index.ts:919
+msgid "Step In"
 msgstr ""
 
-#: packages/debugger-extension/src/index.ts:861 packages/debugger-extension/src/index.ts:873
-msgid "Debugger"
+#: packages/debugger-extension/src/index.ts:928 packages/debugger-extension/src/index.ts:929
+msgid "Step Out"
 msgstr ""
 
-#: packages/debugger-extension/src/index.ts:866
-msgid "Debugger Panel"
+#: packages/debugger-extension/src/index.ts:955
+msgid "Select a filter for breakpoints on exception"
 msgstr ""
 
 #: packages/debugger/src/handler.ts:39
 msgid "Enable Debugger"
 msgstr ""
 
 #: packages/debugger/src/handler.ts:41
@@ -3926,23 +4302,27 @@
 msgid "Remove breakpoints"
 msgstr ""
 
 #: packages/debugger/src/panels/callstack/index.ts:27
 msgid "Callstack"
 msgstr ""
 
-#: packages/debugger/src/panels/kernelSources/body.tsx:83
+#: packages/debugger/src/panels/kernelSources/body.tsx:87
 msgid "Fail to get source"
 msgstr ""
 
-#: packages/debugger/src/panels/kernelSources/body.tsx:84
+#: packages/debugger/src/panels/kernelSources/body.tsx:88
 msgid "Fail to get '%1' source:\n"
 "%2"
 msgstr ""
 
+#: packages/debugger/src/panels/kernelSources/filter.tsx:33
+msgid "Filter the kernel sources"
+msgstr ""
+
 #: packages/debugger/src/panels/kernelSources/index.tsx:33
 msgid "Kernel Sources"
 msgstr ""
 
 #: packages/debugger/src/panels/kernelSources/index.tsx:49
 msgid "Toggle search filter"
 msgstr ""
@@ -3956,15 +4336,15 @@
 "%2"
 msgstr ""
 
 #: packages/debugger/src/panels/kernelSources/index.tsx:66
 msgid "Refresh kernel sources"
 msgstr ""
 
-#: packages/debugger/src/panels/sources/index.tsx:29 packages/shortcuts-extension/src/components/TopNav.tsx:185
+#: packages/debugger/src/panels/sources/index.tsx:29 packages/shortcuts-extension/src/components/TopNav.tsx:134 packages/shortcuts-extension/src/components/TopNav.tsx:186
 msgid "Source"
 msgstr ""
 
 #: packages/debugger/src/panels/sources/index.tsx:42
 msgid "Open in the Main Area"
 msgstr ""
 
@@ -3972,15 +4352,15 @@
 msgid "Type"
 msgstr ""
 
 #: packages/debugger/src/panels/variables/gridpanel.ts:218
 msgid "Value"
 msgstr ""
 
-#: packages/debugger/src/panels/variables/gridpanel.ts:221 packages/filebrowser/src/listing.ts:2258 packages/filebrowser/src/listing.ts:2275 packages/filebrowser/src/listing.ts:2277
+#: packages/debugger/src/panels/variables/gridpanel.ts:221 packages/filebrowser/src/listing.ts:2277 packages/filebrowser/src/listing.ts:2298 packages/filebrowser/src/listing.ts:2371
 msgid "Name"
 msgstr ""
 
 #: packages/debugger/src/panels/variables/index.ts:33
 msgid "Variables"
 msgstr ""
 
@@ -4004,245 +4384,269 @@
 msgid "Render variable: %1"
 msgstr ""
 
 #: packages/debugger/src/service.ts:378
 msgid "Globals"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:1002 packages/docmanager-extension/src/index.tsx:999
+#: packages/docmanager-extension/src/index.tsx:1007 packages/docmanager-extension/src/index.tsx:1019 packages/docmanager-extension/src/index.tsx:871 packages/docmanager-extension/src/index.tsx:883 packages/docmanager-extension/src/index.tsx:889 packages/docmanager-extension/src/index.tsx:901 packages/notebook/src/default-toolbar.tsx:68
+msgid "Cannot Save"
+msgstr ""
+
+#: packages/docmanager-extension/src/index.tsx:1008 packages/docmanager-extension/src/index.tsx:1020 packages/docmanager-extension/src/index.tsx:485 packages/docmanager-extension/src/index.tsx:495 packages/docmanager-extension/src/index.tsx:737 packages/docmanager-extension/src/index.tsx:749 packages/docmanager-extension/src/index.tsx:782 packages/docmanager-extension/src/index.tsx:794 packages/docmanager-extension/src/index.tsx:872 packages/docmanager-extension/src/index.tsx:884
+msgid "No context found for current widget!"
+msgstr ""
+
+#: packages/docmanager-extension/src/index.tsx:1010 packages/docmanager-extension/src/index.tsx:998
+msgid "Save %1 As…"
+msgstr ""
+
+#: packages/docmanager-extension/src/index.tsx:1011 packages/docmanager-extension/src/index.tsx:999
+msgid "Save with new path"
+msgstr ""
+
+#: packages/docmanager-extension/src/index.tsx:1039 packages/docmanager-extension/src/index.tsx:1063
 msgid "Autosave Documents"
 msgstr "Salvare Automată Documente"
 
-#: packages/docmanager-extension/src/index.tsx:1060 packages/docmanager-extension/src/index.tsx:1063
+#: packages/docmanager-extension/src/index.tsx:1100 packages/docmanager-extension/src/index.tsx:1124
 msgid "New View for %1"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:1084 packages/docmanager-extension/src/index.tsx:1087
+#: packages/docmanager-extension/src/index.tsx:1124 packages/docmanager-extension/src/index.tsx:1148
 msgid "Rename%1…"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:1098 packages/docmanager-extension/src/index.tsx:1101
+#: packages/docmanager-extension/src/index.tsx:1138 packages/docmanager-extension/src/index.tsx:1162
 msgid "Duplicate %1"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:1113 packages/docmanager-extension/src/index.tsx:1116
+#: packages/docmanager-extension/src/index.tsx:1153 packages/docmanager-extension/src/index.tsx:1177 packages/workspaces-extension/src/sidebar.ts:99
 msgid "Delete %1"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:1123 packages/docmanager-extension/src/index.tsx:1126 packages/docmanager-extension/src/index.tsx:1127 packages/docmanager-extension/src/index.tsx:1130 packages/filebrowser-extension/src/index.ts:922 packages/filebrowser-extension/src/index.ts:926 packages/filebrowser/src/listing.ts:426 packages/filebrowser/src/listing.ts:430 packages/filebrowser/src/listing.ts:434
+#: packages/docmanager-extension/src/index.tsx:1163 packages/docmanager-extension/src/index.tsx:1167 packages/docmanager-extension/src/index.tsx:1187 packages/docmanager-extension/src/index.tsx:1191 packages/filebrowser-extension/src/index.ts:929 packages/filebrowser-extension/src/index.ts:937 packages/filebrowser/src/listing.ts:430 packages/filebrowser/src/listing.ts:433 packages/filebrowser/src/listing.ts:434 packages/filebrowser/src/listing.ts:437 packages/workspaces-extension/src/commands.ts:199
 msgid "Delete"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:1124 packages/docmanager-extension/src/index.tsx:1127
+#: packages/docmanager-extension/src/index.tsx:1164 packages/docmanager-extension/src/index.tsx:1188
 msgid "Are you sure you want to delete %1"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:1141 packages/docmanager-extension/src/index.tsx:1144
+#: packages/docmanager-extension/src/index.tsx:1181 packages/docmanager-extension/src/index.tsx:1205
 msgid "Show in File Browser"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:1207 packages/docmanager-extension/src/index.tsx:1210
+#: packages/docmanager-extension/src/index.tsx:1247 packages/docmanager-extension/src/index.tsx:1283
 msgid "Are you sure you want to revert the %1 to checkpoint? "
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:1213 packages/docmanager-extension/src/index.tsx:1216
+#: packages/docmanager-extension/src/index.tsx:1253 packages/docmanager-extension/src/index.tsx:1289
 msgid "This cannot be undone."
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:1220 packages/docmanager-extension/src/index.tsx:1223
+#: packages/docmanager-extension/src/index.tsx:1260 packages/docmanager-extension/src/index.tsx:1296
 msgid "The checkpoint was last updated at: "
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:1254 packages/docmanager-extension/src/index.tsx:1257
+#: packages/docmanager-extension/src/index.tsx:1294 packages/docmanager-extension/src/index.tsx:1330
 msgid "Choose a checkpoint"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:344
+#: packages/docmanager-extension/src/index.tsx:345 packages/docmanager-extension/src/index.tsx:355
 msgid "Overrides for the default viewers for file types.\n"
 "Specify a mapping from file type name to document viewer name, for example:\n\n"
 "defaultViewers: {\n"
 "  markdown: \"Markdown Preview\"\n"
 "}\n\n"
 "If you specify non-existent file types or viewers, or if a viewer cannot\n"
 "open a given file type, the override will not function.\n\n"
 "Available viewers:\n"
 "%1\n\n"
 "Available file types:\n"
 "%2"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:474 packages/filebrowser-extension/src/index.ts:367 packages/filebrowser-extension/src/index.ts:371
+#: packages/docmanager-extension/src/index.tsx:475 packages/docmanager-extension/src/index.tsx:485 packages/filebrowser-extension/src/index.ts:374 packages/filebrowser-extension/src/index.ts:405
 msgid "Download"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:475
+#: packages/docmanager-extension/src/index.tsx:476 packages/docmanager-extension/src/index.tsx:486
 msgid "Download the file to your computer"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:483
+#: packages/docmanager-extension/src/index.tsx:484 packages/docmanager-extension/src/index.tsx:494
 msgid "Cannot Download"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:484 packages/docmanager-extension/src/index.tsx:726 packages/docmanager-extension/src/index.tsx:771 packages/docmanager-extension/src/index.tsx:844 packages/docmanager-extension/src/index.tsx:847 packages/docmanager-extension/src/index.tsx:968 packages/docmanager-extension/src/index.tsx:971
-msgid "No context found for current widget!"
-msgstr ""
-
-#: packages/docmanager-extension/src/index.tsx:493 packages/docmanager-extension/src/index.tsx:634 packages/filebrowser-extension/src/index.ts:1074 packages/filebrowser-extension/src/index.ts:1078 packages/filebrowser-extension/src/index.ts:566 packages/filebrowser-extension/src/index.ts:570 packages/filebrowser-extension/src/index.ts:892 packages/filebrowser-extension/src/index.ts:896 packages/htmlviewer-extension/src/index.tsx:206
+#: packages/docmanager-extension/src/index.tsx:494 packages/docmanager-extension/src/index.tsx:508 packages/docmanager-extension/src/index.tsx:635 packages/docmanager-extension/src/index.tsx:650 packages/filebrowser-extension/src/index.ts:1081 packages/filebrowser-extension/src/index.ts:1089 packages/filebrowser-extension/src/index.ts:573 packages/filebrowser-extension/src/index.ts:581 packages/filebrowser-extension/src/index.ts:899 packages/filebrowser-extension/src/index.ts:907 packages/htmlviewer-extension/src/index.tsx:206 packages/htmlviewer-extension/src/index.tsx:211
 msgid "File Operations"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:542 packages/filebrowser-extension/src/index.ts:772 packages/filebrowser-extension/src/index.ts:776
+#: packages/docmanager-extension/src/index.tsx:543 packages/docmanager-extension/src/index.tsx:557 packages/filebrowser-extension/src/index.ts:779 packages/filebrowser-extension/src/index.ts:787
 msgid "Open in New Browser Tab"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:670 packages/filebrowser/src/browser.ts:236 packages/filebrowser/src/browser.ts:252 packages/logconsole-extension/src/index.tsx:376
+#: packages/docmanager-extension/src/index.tsx:652
+msgid "%1 is permissioned as read-only. Use \"save as...\" instead."
+msgstr ""
+
+#: packages/docmanager-extension/src/index.tsx:667
+msgid "%1 is read-only. Use \"Save as…\" instead."
+msgstr ""
+
+#: packages/docmanager-extension/src/index.tsx:681 packages/docmanager-extension/src/index.tsx:693 packages/filebrowser/src/browser.ts:261 packages/filebrowser/src/browser.ts:267 packages/logconsole-extension/src/index.tsx:376
 msgid "Error"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:704
+#: packages/docmanager-extension/src/index.tsx:715 packages/docmanager-extension/src/index.tsx:727
 msgid "Open the provided `path`."
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:710 packages/docmanager-extension/src/index.tsx:732
+#: packages/docmanager-extension/src/index.tsx:721 packages/docmanager-extension/src/index.tsx:733 packages/docmanager-extension/src/index.tsx:743 packages/docmanager-extension/src/index.tsx:755
 msgid "Reload %1 from Disk"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:714
+#: packages/docmanager-extension/src/index.tsx:725 packages/docmanager-extension/src/index.tsx:737
 msgid "Reload contents from disk"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:725
+#: packages/docmanager-extension/src/index.tsx:736 packages/docmanager-extension/src/index.tsx:748
 msgid "Cannot Reload"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:733
+#: packages/docmanager-extension/src/index.tsx:744 packages/docmanager-extension/src/index.tsx:756
 msgid "Are you sure you want to reload the %1 from the disk?"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:756
+#: packages/docmanager-extension/src/index.tsx:767 packages/docmanager-extension/src/index.tsx:779
 msgid "Revert %1 to Checkpoint…"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:760
+#: packages/docmanager-extension/src/index.tsx:771 packages/docmanager-extension/src/index.tsx:783
 msgid "Revert contents to previous checkpoint"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:770
+#: packages/docmanager-extension/src/index.tsx:781 packages/docmanager-extension/src/index.tsx:793
 msgid "Cannot Revert"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:779
+#: packages/docmanager-extension/src/index.tsx:790 packages/docmanager-extension/src/index.tsx:802
 msgid "No checkpoints"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:780
+#: packages/docmanager-extension/src/index.tsx:791 packages/docmanager-extension/src/index.tsx:803
 msgid "No checkpoints are available for this %1."
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:793
+#: packages/docmanager-extension/src/index.tsx:804 packages/docmanager-extension/src/index.tsx:816
 msgid "Revert %1 to checkpoint"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:797 packages/docmanager-extension/src/index.tsx:798 packages/docregistry/src/context.ts:776 packages/docregistry/src/context.ts:801 packages/docregistry/src/context.ts:805
+#: packages/docmanager-extension/src/index.tsx:809 packages/docmanager-extension/src/index.tsx:821 packages/docregistry/src/context.ts:825 packages/docregistry/src/context.ts:827
 msgid "Revert"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:799
+#: packages/docmanager-extension/src/index.tsx:810 packages/docmanager-extension/src/index.tsx:822
 msgid "Revert to Checkpoint"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:820 packages/docmanager-extension/src/index.tsx:823
+#: packages/docmanager-extension/src/index.tsx:834 packages/docmanager-extension/src/index.tsx:846
 msgid "In collaborative mode, the document is saved automatically after every change"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:826 packages/docmanager-extension/src/index.tsx:829
+#: packages/docmanager-extension/src/index.tsx:839
+msgid "document is permissioned readonly; \"save\" is disabled, use \"save as...\" instead"
+msgstr ""
+
+#: packages/docmanager-extension/src/index.tsx:845 packages/docmanager-extension/src/index.tsx:857
 msgid "Save and create checkpoint"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:832 packages/docmanager-extension/src/index.tsx:835
+#: packages/docmanager-extension/src/index.tsx:851 packages/docmanager-extension/src/index.tsx:863
 msgid "Save %1"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:843 packages/docmanager-extension/src/index.tsx:846 packages/docmanager-extension/src/index.tsx:854 packages/docmanager-extension/src/index.tsx:857 packages/docmanager-extension/src/index.tsx:967 packages/docmanager-extension/src/index.tsx:970 packages/notebook/src/default-toolbar.tsx:68
-msgid "Cannot Save"
+#: packages/docmanager-extension/src/index.tsx:851 packages/docregistry/src/components.tsx:25
+msgid "Document is read-only. \"Save\" is disabled; use \"Save as…\" instead"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:855 packages/docmanager-extension/src/index.tsx:858 packages/notebook/src/default-toolbar.tsx:69
+#: packages/docmanager-extension/src/index.tsx:890 packages/docmanager-extension/src/index.tsx:902 packages/notebook/src/default-toolbar.tsx:69
 msgid "Document is read-only"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:870 packages/docmanager-extension/src/index.tsx:873
+#: packages/docmanager-extension/src/index.tsx:906 packages/docmanager-extension/src/index.tsx:918
 msgid "Rename file"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:871 packages/docmanager-extension/src/index.tsx:874 packages/docmanager/src/dialogs.ts:57 packages/docmanager/src/dialogs.ts:58 packages/filebrowser-extension/src/index.ts:1197 packages/filebrowser-extension/src/index.ts:1201
+#: packages/docmanager-extension/src/index.tsx:907 packages/docmanager-extension/src/index.tsx:919 packages/docmanager/src/dialogs.ts:58 packages/filebrowser-extension/src/index.ts:1204 packages/filebrowser-extension/src/index.ts:1212 packages/workspaces-extension/src/commands.ts:285
 msgid "Rename"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:872 packages/docmanager-extension/src/index.tsx:875
+#: packages/docmanager-extension/src/index.tsx:908 packages/docmanager-extension/src/index.tsx:920
 msgid "File name"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:876 packages/docmanager-extension/src/index.tsx:879 packages/docmanager/src/widgetmanager.ts:414 packages/docmanager/src/widgetmanager.ts:420
+#: packages/docmanager-extension/src/index.tsx:912 packages/docmanager-extension/src/index.tsx:924 packages/docmanager/src/widgetmanager.ts:420 packages/docmanager/src/widgetmanager.ts:491
 msgid "Do not ask me again."
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:877 packages/docmanager-extension/src/index.tsx:880
+#: packages/docmanager-extension/src/index.tsx:913 packages/docmanager-extension/src/index.tsx:925
 msgid "If checked, you will not be asked to rename future untitled files when saving them."
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:934 packages/docmanager-extension/src/index.tsx:937
+#: packages/docmanager-extension/src/index.tsx:970 packages/docmanager-extension/src/index.tsx:982
 msgid "Save All"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:935 packages/docmanager-extension/src/index.tsx:938
+#: packages/docmanager-extension/src/index.tsx:971 packages/docmanager-extension/src/index.tsx:983
 msgid "Save all open documents"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:958 packages/docmanager-extension/src/index.tsx:961
-msgid "Save %1 As…"
+#: packages/docmanager-extension/src/recents.ts:73
+msgid "Clear Recent Documents"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:959 packages/docmanager-extension/src/index.tsx:962
-msgid "Save with new path"
+#: packages/docmanager-extension/src/recents.ts:74
+msgid "Clear the list of recently opened items."
 msgstr ""
 
-#: packages/docmanager/src/dialogs.ts:114 packages/docmanager/src/dialogs.ts:117
+#: packages/docmanager/src/dialogs.ts:117
 msgid "Overwrite file?"
 msgstr ""
 
-#: packages/docmanager/src/dialogs.ts:115 packages/docmanager/src/dialogs.ts:118
+#: packages/docmanager/src/dialogs.ts:118
 msgid "\"%1\" already exists, overwrite?"
 msgstr ""
 
-#: packages/docmanager/src/dialogs.ts:118 packages/docmanager/src/dialogs.ts:122 packages/docregistry/src/context.ts:780 packages/docregistry/src/context.ts:805 packages/docregistry/src/context.ts:809 packages/docregistry/src/context.ts:816 packages/docregistry/src/context.ts:841 packages/docregistry/src/context.ts:845 packages/shortcuts-extension/src/components/ShortcutInput.tsx:495 packages/shortcuts-extension/src/components/ShortcutItem.tsx:231
+#: packages/docmanager/src/dialogs.ts:122 packages/docregistry/src/context.ts:829 packages/docregistry/src/context.ts:831 packages/docregistry/src/context.ts:865 packages/docregistry/src/context.ts:867 packages/shortcuts-extension/src/components/ShortcutInput.tsx:495 packages/shortcuts-extension/src/components/ShortcutInput.tsx:496 packages/shortcuts-extension/src/components/ShortcutItem.tsx:231 packages/shortcuts-extension/src/components/ShortcutItem.tsx:348
 msgid "Overwrite"
 msgstr ""
 
 #: packages/docmanager/src/dialogs.ts:123
 msgid "Overwrite Existing File"
 msgstr ""
 
-#: packages/docmanager/src/dialogs.ts:182 packages/docmanager/src/dialogs.ts:188
+#: packages/docmanager/src/dialogs.ts:188
 msgid "File Path"
 msgstr ""
 
-#: packages/docmanager/src/dialogs.ts:187 packages/docmanager/src/dialogs.ts:193
+#: packages/docmanager/src/dialogs.ts:193
 msgid "New Name"
 msgstr ""
 
 #: packages/docmanager/src/dialogs.ts:52 packages/docmanager/src/dialogs.ts:59
 msgid "Rename File"
 msgstr ""
 
-#: packages/docmanager/src/dialogs.ts:65 packages/docmanager/src/dialogs.ts:68 packages/filebrowser/src/listing.ts:1875 packages/filebrowser/src/listing.ts:1891
+#: packages/docmanager/src/dialogs.ts:68 packages/filebrowser/src/listing.ts:1891 packages/filebrowser/src/listing.ts:1912 packages/filebrowser/src/listing.ts:1964
 msgid "Rename Error"
 msgstr ""
 
-#: packages/docmanager/src/dialogs.ts:67 packages/docmanager/src/dialogs.ts:70
+#: packages/docmanager/src/dialogs.ts:70
 msgid "\"%1\" is not a valid name for a file. Names must have nonzero length, and cannot include \"/\", \"\\\", or \":\""
 msgstr ""
 
 #: packages/docmanager/src/savingstatus.tsx:58
 msgid "Saving completed"
 msgstr ""
 
@@ -4250,233 +4654,261 @@
 msgid "Saving started"
 msgstr ""
 
 #: packages/docmanager/src/savingstatus.tsx:60
 msgid "Saving failed"
 msgstr ""
 
-#: packages/docmanager/src/widgetmanager.ts:296
+#: packages/docmanager/src/widgetmanager.ts:296 packages/docmanager/src/widgetmanager.ts:307
 msgid "Name: %1\n"
 "Path: %2\n"
 msgstr ""
 
-#: packages/docmanager/src/widgetmanager.ts:302
+#: packages/docmanager/src/widgetmanager.ts:302 packages/docmanager/src/widgetmanager.ts:313
 msgid "Read-only"
 msgstr ""
 
-#: packages/docmanager/src/widgetmanager.ts:305
+#: packages/docmanager/src/widgetmanager.ts:305 packages/docmanager/src/widgetmanager.ts:316
 msgid "Last Saved: %1\n"
 msgstr ""
 
-#: packages/docmanager/src/widgetmanager.ts:306
+#: packages/docmanager/src/widgetmanager.ts:306 packages/docmanager/src/widgetmanager.ts:317
 msgid "Last Checkpoint: %1"
 msgstr ""
 
-#: packages/docmanager/src/widgetmanager.ts:397
+#: packages/docmanager/src/widgetmanager.ts:397 packages/docmanager/src/widgetmanager.ts:468
 msgid "Close and save"
 msgstr ""
 
-#: packages/docmanager/src/widgetmanager.ts:399
+#: packages/docmanager/src/widgetmanager.ts:399 packages/docmanager/src/widgetmanager.ts:470
 msgid "Close and save Document"
 msgstr ""
 
-#: packages/docmanager/src/widgetmanager.ts:400
+#: packages/docmanager/src/widgetmanager.ts:400 packages/docmanager/src/widgetmanager.ts:471
 msgid "Close Document"
 msgstr ""
 
-#: packages/docmanager/src/widgetmanager.ts:404 packages/docmanager/src/widgetmanager.ts:408
+#: packages/docmanager/src/widgetmanager.ts:408 packages/docmanager/src/widgetmanager.ts:479
 msgid "Close without saving"
 msgstr ""
 
-#: packages/docmanager/src/widgetmanager.ts:409
+#: packages/docmanager/src/widgetmanager.ts:409 packages/docmanager/src/widgetmanager.ts:480
 msgid "Close Document without saving"
 msgstr ""
 
-#: packages/docmanager/src/widgetmanager.ts:409 packages/docmanager/src/widgetmanager.ts:415 packages/notebook/src/searchprovider.ts:509 packages/notebook/src/searchprovider.ts:511
+#: packages/docmanager/src/widgetmanager.ts:415 packages/docmanager/src/widgetmanager.ts:486 packages/notebook/src/searchprovider.ts:511 packages/notebook/src/searchprovider.ts:514 packages/notebook/src/searchprovider.ts:522
 msgid "Confirmation"
 msgstr ""
 
-#: packages/docmanager/src/widgetmanager.ts:410 packages/docmanager/src/widgetmanager.ts:416
+#: packages/docmanager/src/widgetmanager.ts:416 packages/docmanager/src/widgetmanager.ts:487
 msgid "Please confirm you want to close \"%1\"."
 msgstr ""
 
-#: packages/docmanager/src/widgetmanager.ts:415 packages/docmanager/src/widgetmanager.ts:421
+#: packages/docmanager/src/widgetmanager.ts:421 packages/docmanager/src/widgetmanager.ts:492
 msgid "If checked, no confirmation to close a document will be asked in the future."
 msgstr ""
 
-#: packages/docmanager/src/widgetmanager.ts:437 packages/docmanager/src/widgetmanager.ts:443
+#: packages/docmanager/src/widgetmanager.ts:443 packages/docmanager/src/widgetmanager.ts:514
 msgid "Save as"
 msgstr ""
 
-#: packages/docmanager/src/widgetmanager.ts:439 packages/docmanager/src/widgetmanager.ts:445
+#: packages/docmanager/src/widgetmanager.ts:445 packages/docmanager/src/widgetmanager.ts:516
 msgid "Save your work"
 msgstr ""
 
-#: packages/docmanager/src/widgetmanager.ts:440 packages/docmanager/src/widgetmanager.ts:446
+#: packages/docmanager/src/widgetmanager.ts:446 packages/docmanager/src/widgetmanager.ts:517
 msgid "Save changes in \"%1\" before closing?"
 msgstr ""
 
-#: packages/docmanager/src/widgetmanager.ts:443 packages/docmanager/src/widgetmanager.ts:450
+#: packages/docmanager/src/widgetmanager.ts:450 packages/docmanager/src/widgetmanager.ts:521
 msgid "Discard"
 msgstr ""
 
-#: packages/docmanager/src/widgetmanager.ts:451
+#: packages/docmanager/src/widgetmanager.ts:451 packages/docmanager/src/widgetmanager.ts:522
 msgid "Discard changes to file"
 msgstr ""
 
-#: packages/docregistry/src/context.ts:1017 packages/docregistry/src/context.ts:1021 packages/docregistry/src/context.ts:994
+#: packages/docregistry/src/components.tsx:25
+msgid "Document is permissioned read-only; \"save\" is disabled, use \"save as...\" instead"
+msgstr ""
+
+#: packages/docregistry/src/components.tsx:29
+msgid "%1 is read-only"
+msgstr ""
+
+#: packages/docregistry/src/context.ts:1043 packages/docregistry/src/context.ts:1045
 msgid "Save File As…"
 msgstr ""
 
-#: packages/docregistry/src/context.ts:606 packages/docregistry/src/context.ts:627 packages/docregistry/src/context.ts:631 packages/docregistry/src/context.ts:865 packages/docregistry/src/context.ts:890 packages/docregistry/src/context.ts:894
+#: packages/docregistry/src/context.ts:614 packages/docregistry/src/context.ts:616 packages/docregistry/src/context.ts:914 packages/docregistry/src/context.ts:916
 msgid "File Save Error for %1"
 msgstr ""
 
-#: packages/docregistry/src/context.ts:670 packages/docregistry/src/context.ts:691 packages/docregistry/src/context.ts:695
+#: packages/docregistry/src/context.ts:679 packages/docregistry/src/context.ts:681
 msgid "File Load Error for %1"
 msgstr ""
 
-#: packages/docregistry/src/context.ts:769 packages/docregistry/src/context.ts:794 packages/docregistry/src/context.ts:798
+#: packages/docregistry/src/context.ts:818 packages/docregistry/src/context.ts:820
 msgid "\"%1\" has changed on disk since the last time it was opened or saved.\n"
 "Do you want to overwrite the file on disk with the version open here,\n"
 "or load the version on disk (revert)?"
 msgstr ""
 
-#: packages/docregistry/src/context.ts:785 packages/docregistry/src/context.ts:810 packages/docregistry/src/context.ts:814
+#: packages/docregistry/src/context.ts:834 packages/docregistry/src/context.ts:836
 msgid "File Changed"
 msgstr ""
 
-#: packages/docregistry/src/context.ts:811 packages/docregistry/src/context.ts:836 packages/docregistry/src/context.ts:840
+#: packages/docregistry/src/context.ts:860 packages/docregistry/src/context.ts:862
 msgid "\"%1\" already exists. Do you want to replace it?"
 msgstr ""
 
-#: packages/docregistry/src/context.ts:820 packages/docregistry/src/context.ts:845 packages/docregistry/src/context.ts:849
+#: packages/docregistry/src/context.ts:869 packages/docregistry/src/context.ts:871
 msgid "File Overwrite?"
 msgstr ""
 
-#: packages/docregistry/src/mimedocument.ts:174 packages/docregistry/src/mimedocument.ts:70 packages/markdownviewer/src/widget.ts:211
+#: packages/docregistry/src/mimedocument.ts:175 packages/docregistry/src/mimedocument.ts:71 packages/markdownviewer/src/widget.ts:211
 msgid "Renderer Failure: %1"
 msgstr ""
 
-#: packages/docregistry/src/registry.ts:1287
+#: packages/docregistry/src/registry.ts:1287 packages/docregistry/src/registry.ts:1297
 msgid "default"
 msgstr "implicit"
 
-#: packages/docregistry/src/registry.ts:1310
+#: packages/docregistry/src/registry.ts:1310 packages/docregistry/src/registry.ts:1320
 msgid "Text"
 msgstr ""
 
-#: packages/docregistry/src/registry.ts:1333 packages/launcher/src/widget.tsx:115 packages/launcher/src/widget.tsx:120 packages/notebook-extension/src/index.ts:1210 packages/notebook-extension/src/index.ts:1213 packages/notebook-extension/src/index.ts:1232 packages/notebook-extension/src/index.ts:1902 packages/notebook-extension/src/index.ts:1905 packages/notebook-extension/src/index.ts:1924 packages/notebook-extension/src/index.ts:1938 packages/notebook-extension/src/index.ts:1941 packages/notebook-extension/src/index.ts:1960
+#: packages/docregistry/src/registry.ts:1333 packages/docregistry/src/registry.ts:1343 packages/launcher/src/widget.tsx:115 packages/launcher/src/widget.tsx:120 packages/notebook-extension/src/index.ts:1243 packages/notebook-extension/src/index.ts:1247 packages/notebook-extension/src/index.ts:1255 packages/notebook-extension/src/index.ts:1955 packages/notebook-extension/src/index.ts:1960 packages/notebook-extension/src/index.ts:1971 packages/notebook-extension/src/index.ts:1991 packages/notebook-extension/src/index.ts:1998 packages/notebook-extension/src/index.ts:2009
 msgid "Notebook"
 msgstr ""
 
-#: packages/docregistry/src/registry.ts:1358
+#: packages/docregistry/src/registry.ts:1358 packages/docregistry/src/registry.ts:1368
 msgid "Directory"
 msgstr ""
 
-#: packages/docregistry/src/registry.ts:1385 packages/fileeditor-extension/src/commands.ts:810 packages/fileeditor-extension/src/commands.ts:817
+#: packages/docregistry/src/registry.ts:1385 packages/docregistry/src/registry.ts:1395 packages/fileeditor-extension/src/commands.ts:817 packages/fileeditor-extension/src/commands.ts:818
 msgid "Markdown File"
 msgstr ""
 
-#: packages/docregistry/src/registry.ts:1392
+#: packages/docregistry/src/registry.ts:1392 packages/docregistry/src/registry.ts:1402
 msgid "PDF File"
 msgstr ""
 
-#: packages/docregistry/src/registry.ts:1399 packages/fileeditor-extension/src/index.ts:329
+#: packages/docregistry/src/registry.ts:1399 packages/docregistry/src/registry.ts:1409 packages/fileeditor-extension/src/index.ts:331
 msgid "Python File"
 msgstr ""
 
-#: packages/docregistry/src/registry.ts:1406
+#: packages/docregistry/src/registry.ts:1406 packages/docregistry/src/registry.ts:1416
 msgid "JSON File"
 msgstr ""
 
-#: packages/docregistry/src/registry.ts:1413 packages/fileeditor-extension/src/index.ts:341
+#: packages/docregistry/src/registry.ts:1413 packages/docregistry/src/registry.ts:1423
+msgid "JSONLines File"
+msgstr ""
+
+#: packages/docregistry/src/registry.ts:1424 packages/docregistry/src/registry.ts:1434 packages/fileeditor-extension/src/index.ts:343
 msgid "Julia File"
 msgstr ""
 
-#: packages/docregistry/src/registry.ts:1420
+#: packages/docregistry/src/registry.ts:1431 packages/docregistry/src/registry.ts:1441
 msgid "CSV File"
 msgstr ""
 
-#: packages/docregistry/src/registry.ts:1427
+#: packages/docregistry/src/registry.ts:1438 packages/docregistry/src/registry.ts:1448
 msgid "TSV File"
 msgstr ""
 
-#: packages/docregistry/src/registry.ts:1434 packages/fileeditor-extension/src/index.ts:353
+#: packages/docregistry/src/registry.ts:1445 packages/docregistry/src/registry.ts:1455 packages/fileeditor-extension/src/index.ts:355
 msgid "R File"
 msgstr ""
 
-#: packages/docregistry/src/registry.ts:1441
+#: packages/docregistry/src/registry.ts:1452 packages/docregistry/src/registry.ts:1462
 msgid "YAML File"
 msgstr ""
 
-#: packages/docregistry/src/registry.ts:1448 packages/docregistry/src/registry.ts:1456 packages/docregistry/src/registry.ts:1464 packages/docregistry/src/registry.ts:1472 packages/docregistry/src/registry.ts:1480 packages/docregistry/src/registry.ts:1488 packages/docregistry/src/registry.ts:1496 packages/imageviewer-extension/src/index.ts:119
+#: packages/docregistry/src/registry.ts:1459 packages/docregistry/src/registry.ts:1467 packages/docregistry/src/registry.ts:1469 packages/docregistry/src/registry.ts:1475 packages/docregistry/src/registry.ts:1477 packages/docregistry/src/registry.ts:1483 packages/docregistry/src/registry.ts:1485 packages/docregistry/src/registry.ts:1491 packages/docregistry/src/registry.ts:1493 packages/docregistry/src/registry.ts:1499 packages/docregistry/src/registry.ts:1501 packages/docregistry/src/registry.ts:1507 packages/docregistry/src/registry.ts:1509 packages/docregistry/src/registry.ts:1517 packages/imageviewer-extension/src/index.ts:119
 msgid "Image"
 msgstr ""
 
-#: packages/documentsearch-extension/src/index.ts:229 packages/fileeditor-extension/src/commands.ts:525 packages/fileeditor-extension/src/commands.ts:526
+#: packages/documentsearch-extension/src/index.ts:326 packages/fileeditor-extension/src/commands.ts:526 packages/fileeditor-extension/src/commands.ts:527 packages/json-extension/src/component.tsx:78
 msgid "Find…"
 msgstr ""
 
-#: packages/documentsearch-extension/src/index.ts:248
+#: packages/documentsearch-extension/src/index.ts:363
 msgid "Find and Replace…"
 msgstr ""
 
-#: packages/documentsearch-extension/src/index.ts:272
+#: packages/documentsearch-extension/src/index.ts:387
 msgid "Find Next"
 msgstr ""
 
-#: packages/documentsearch-extension/src/index.ts:287
+#: packages/documentsearch-extension/src/index.ts:402
 msgid "Find Previous"
 msgstr ""
 
-#: packages/documentsearch-extension/src/index.ts:302
+#: packages/documentsearch-extension/src/index.ts:417
 msgid "End Search"
 msgstr ""
 
-#: packages/documentsearch/src/searchview.tsx:169 packages/documentsearch/src/searchview.tsx:178
+#: packages/documentsearch-extension/src/index.ts:431
+msgid "Search in Selection"
+msgstr ""
+
+#: packages/documentsearch/src/searchview.tsx:188
 msgid "Match Case"
 msgstr ""
 
-#: packages/documentsearch/src/searchview.tsx:177 packages/documentsearch/src/searchview.tsx:186
+#: packages/documentsearch/src/searchview.tsx:196
 msgid "Match Whole Word"
 msgstr ""
 
-#: packages/documentsearch/src/searchview.tsx:185 packages/documentsearch/src/searchview.tsx:194
+#: packages/documentsearch/src/searchview.tsx:204
 msgid "Use Regular Expression"
 msgstr ""
 
-#: packages/documentsearch/src/searchview.tsx:230 packages/documentsearch/src/searchview.tsx:239
+#: packages/documentsearch/src/searchview.tsx:249
 msgid "Preserve Case"
 msgstr ""
 
-#: packages/documentsearch/src/searchview.tsx:260 packages/documentsearch/src/searchview.tsx:269
+#: packages/documentsearch/src/searchview.tsx:279
 msgid "Replace All"
 msgstr ""
 
-#: packages/documentsearch/src/searchview.tsx:280 packages/documentsearch/src/searchview.tsx:289
+#: packages/documentsearch/src/searchview.tsx:313
 msgid "Previous Match"
 msgstr ""
 
-#: packages/documentsearch/src/searchview.tsx:291 packages/documentsearch/src/searchview.tsx:300
+#: packages/documentsearch/src/searchview.tsx:324 packages/documentsearch/src/searchview.tsx:328
 msgid "Next Match"
 msgstr ""
 
-#: packages/documentsearch/src/searchview.tsx:341 packages/documentsearch/src/searchview.tsx:350
+#: packages/documentsearch/src/searchview.tsx:374 packages/documentsearch/src/searchview.tsx:385
 msgid "Hide Search Filters"
 msgstr ""
 
-#: packages/documentsearch/src/searchview.tsx:342 packages/documentsearch/src/searchview.tsx:351
+#: packages/documentsearch/src/searchview.tsx:375 packages/documentsearch/src/searchview.tsx:386
 msgid "Show Search Filters"
 msgstr ""
 
-#: packages/documentsearch/src/searchview.tsx:637 packages/documentsearch/src/searchview.tsx:646
+#: packages/documentsearch/src/searchview.tsx:685
 msgid "Toggle Replace"
 msgstr ""
 
+#: packages/documentsearch/src/searchview.tsx:703
+msgid "Hide Replace"
+msgstr ""
+
+#: packages/documentsearch/src/searchview.tsx:704
+msgid "Show Replace"
+msgstr ""
+
+#: packages/documentsearch/src/searchview.tsx:753
+msgid "Close Search Box"
+msgstr ""
+
 #: packages/extensionmanager-extension/src/index.ts:131 packages/extensionmanager-extension/src/index.ts:153 packages/extensionmanager-extension/src/index.ts:59
 msgid "Extension Manager"
 msgstr "Mangerul de Extensii"
 
 #: packages/extensionmanager-extension/src/index.ts:141
 msgid "Enable Extension Manager"
 msgstr ""
@@ -4490,19 +4922,19 @@
 "The JupyterLab development team is excited to have a robust\n"
 "third-party extension community.\n"
 "However, we cannot vouch for every extension,\n"
 "and some may introduce security risks.\n"
 "Do you want to continue?"
 msgstr ""
 
-#: packages/extensionmanager-extension/src/index.ts:185 packages/extensionmanager/src/widget.tsx:161 packages/extensionmanager/src/widget.tsx:165
+#: packages/extensionmanager-extension/src/index.ts:185 packages/extensionmanager/src/widget.tsx:165
 msgid "Disable"
 msgstr ""
 
-#: packages/extensionmanager-extension/src/index.ts:186 packages/extensionmanager/src/widget.tsx:170 packages/extensionmanager/src/widget.tsx:174
+#: packages/extensionmanager-extension/src/index.ts:186 packages/extensionmanager/src/widget.tsx:174
 msgid "Enable"
 msgstr ""
 
 #: packages/extensionmanager-extension/src/index.ts:61
 msgid "Extension Manager section"
 msgstr ""
 
@@ -4510,144 +4942,144 @@
 msgid "Error message:"
 msgstr ""
 
 #: packages/extensionmanager/src/dialog.tsx:35
 msgid "Extension Installation Error"
 msgstr ""
 
-#: packages/extensionmanager/src/model.ts:505 packages/extensionmanager/src/model.ts:530
+#: packages/extensionmanager/src/model.ts:530
 msgid "You will need to restart JupyterLab to apply the changes."
 msgstr ""
 
-#: packages/extensionmanager/src/model.ts:516 packages/extensionmanager/src/model.ts:541
+#: packages/extensionmanager/src/model.ts:541
 msgid "reload JupyterLab"
 msgstr ""
 
-#: packages/extensionmanager/src/model.ts:517 packages/extensionmanager/src/model.ts:542
+#: packages/extensionmanager/src/model.ts:542
 msgid "refresh the web page"
 msgstr ""
 
-#: packages/extensionmanager/src/model.ts:522 packages/extensionmanager/src/model.ts:547
+#: packages/extensionmanager/src/model.ts:547
 msgid "install the extension in all kernels and restart them"
 msgstr ""
 
-#: packages/extensionmanager/src/model.ts:527 packages/extensionmanager/src/model.ts:552
+#: packages/extensionmanager/src/model.ts:552
 msgid "You will need to %1 to apply the changes."
 msgstr ""
 
-#: packages/extensionmanager/src/model.ts:529 packages/extensionmanager/src/model.ts:554
+#: packages/extensionmanager/src/model.ts:554
 msgid " and "
 msgstr ""
 
 #: packages/extensionmanager/src/widget.tsx:114
 msgid "This extension is approved by your security team."
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:133 packages/extensionmanager/src/widget.tsx:137
+#: packages/extensionmanager/src/widget.tsx:137
 msgid "Update \"%1\" to \"%2\""
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:141 packages/extensionmanager/src/widget.tsx:145
+#: packages/extensionmanager/src/widget.tsx:145
 msgid "Update to %1"
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:146 packages/extensionmanager/src/widget.tsx:150
+#: packages/extensionmanager/src/widget.tsx:150
 msgid "Uninstall \"%1\""
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:150 packages/extensionmanager/src/widget.tsx:154
+#: packages/extensionmanager/src/widget.tsx:154
 msgid "Uninstall"
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:157 packages/extensionmanager/src/widget.tsx:161
+#: packages/extensionmanager/src/widget.tsx:161
 msgid "Disable \"%1\""
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:166 packages/extensionmanager/src/widget.tsx:170
+#: packages/extensionmanager/src/widget.tsx:170
 msgid "Enable \"%1\""
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:178 packages/extensionmanager/src/widget.tsx:182
+#: packages/extensionmanager/src/widget.tsx:182
 msgid "Install \"%1\""
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:182 packages/extensionmanager/src/widget.tsx:186
+#: packages/extensionmanager/src/widget.tsx:186
 msgid "Install"
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:251 packages/extensionmanager/src/widget.tsx:259
+#: packages/extensionmanager/src/widget.tsx:259 packages/pluginmanager/src/widget.tsx:76
 msgid "No entries"
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:350 packages/extensionmanager/src/widget.tsx:362
+#: packages/extensionmanager/src/widget.tsx:356
 msgid "%1 Manager"
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:355 packages/extensionmanager/src/widget.tsx:367
+#: packages/extensionmanager/src/widget.tsx:361
 msgid "Extension installation path: %1"
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:363 packages/extensionmanager/src/widget.tsx:375
-msgid "Search"
+#: packages/extensionmanager/src/widget.tsx:369
+msgid "Search extensions"
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:379 packages/extensionmanager/src/widget.tsx:391
+#: packages/extensionmanager/src/widget.tsx:385 packages/pluginmanager/src/widget.tsx:302
 msgid "Error when performing an action."
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:380 packages/extensionmanager/src/widget.tsx:392
+#: packages/extensionmanager/src/widget.tsx:386 packages/pluginmanager/src/widget.tsx:303
 msgid "Reason given:"
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:400 packages/extensionmanager/src/widget.tsx:403 packages/extensionmanager/src/widget.tsx:415
+#: packages/extensionmanager/src/widget.tsx:409
 msgid "The JupyterLab development team is excited to have a robust\n"
 "third-party extension community. However, we do not review\n"
 "third-party extensions, and some extensions may introduce security\n"
 "risks or contain malicious code that runs on your machine. Moreover in order\n"
 "to work, this panel needs to fetch data from web services. Do you agree to\n"
 "activate this feature?"
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:413 packages/extensionmanager/src/widget.tsx:416 packages/extensionmanager/src/widget.tsx:428
+#: packages/extensionmanager/src/widget.tsx:422
 msgid "Please read the privacy policy."
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:422 packages/extensionmanager/src/widget.tsx:425 packages/extensionmanager/src/widget.tsx:437
+#: packages/extensionmanager/src/widget.tsx:431
 msgid "This will withdraw your consent."
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:441 packages/extensionmanager/src/widget.tsx:444 packages/extensionmanager/src/widget.tsx:456
+#: packages/extensionmanager/src/widget.tsx:450
 msgid "This will disable the extension manager panel; including the listing of installed extension."
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:445 packages/extensionmanager/src/widget.tsx:448 packages/extensionmanager/src/widget.tsx:460
+#: packages/extensionmanager/src/widget.tsx:454
 msgid "No, disable"
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:471 packages/extensionmanager/src/widget.tsx:477 packages/extensionmanager/src/widget.tsx:489 packages/extensionmanager/src/widget.tsx:565 packages/extensionmanager/src/widget.tsx:574 packages/extensionmanager/src/widget.tsx:596
+#: packages/extensionmanager/src/widget.tsx:483 packages/extensionmanager/src/widget.tsx:590
 msgid "Updating extensions list…"
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:591 packages/extensionmanager/src/widget.tsx:600 packages/extensionmanager/src/widget.tsx:622
+#: packages/extensionmanager/src/widget.tsx:616
 msgid "Search Results"
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:592 packages/extensionmanager/src/widget.tsx:601 packages/extensionmanager/src/widget.tsx:623
+#: packages/extensionmanager/src/widget.tsx:617
 msgid "Discover"
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:617 packages/extensionmanager/src/widget.tsx:626 packages/extensionmanager/src/widget.tsx:648 packages/logconsole-extension/src/index.tsx:377 packages/settingeditor/src/settingseditor.tsx:122 packages/settingeditor/src/settingseditor.tsx:134
+#: packages/extensionmanager/src/widget.tsx:642 packages/logconsole-extension/src/index.tsx:377 packages/settingeditor/src/settingseditor.tsx:122 packages/settingeditor/src/settingseditor.tsx:134
 msgid "Warning"
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:623 packages/extensionmanager/src/widget.tsx:632 packages/extensionmanager/src/widget.tsx:654
+#: packages/extensionmanager/src/widget.tsx:648
 msgid "Installed"
 msgstr ""
 
-#: packages/extensionmanager/src/widget.tsx:636 packages/extensionmanager/src/widget.tsx:645 packages/extensionmanager/src/widget.tsx:667
+#: packages/extensionmanager/src/widget.tsx:661
 msgid "Refresh extensions list"
 msgstr ""
 
 #: packages/extensionmanager/src/widget.tsx:81
 msgid "%1 extension home page"
 msgstr ""
 
@@ -4655,360 +5087,368 @@
 msgid "Version: %1"
 msgstr ""
 
 #: packages/extensionmanager/src/widget.tsx:97
 msgid "%1 extension is not allowed anymore. Please uninstall it immediately or contact your administrator."
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:1014 packages/filebrowser-extension/src/index.ts:1016 packages/filebrowser-extension/src/index.ts:1018 packages/filebrowser-extension/src/index.ts:1020 packages/filebrowser-extension/src/index.ts:837 packages/filebrowser-extension/src/index.ts:839 packages/filebrowser-extension/src/index.ts:841 packages/filebrowser-extension/src/index.ts:843
+#: packages/filebrowser-extension/src/index.ts:1021 packages/filebrowser-extension/src/index.ts:1023 packages/filebrowser-extension/src/index.ts:1029 packages/filebrowser-extension/src/index.ts:1031 packages/filebrowser-extension/src/index.ts:844 packages/filebrowser-extension/src/index.ts:846 packages/filebrowser-extension/src/index.ts:852 packages/filebrowser-extension/src/index.ts:854
 msgid "Open %1"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:1014 packages/filebrowser-extension/src/index.ts:1018
+#: packages/filebrowser-extension/src/index.ts:1021 packages/filebrowser-extension/src/index.ts:1029
 msgid "Open from Path…"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:1016 packages/filebrowser-extension/src/index.ts:1020
+#: packages/filebrowser-extension/src/index.ts:1023 packages/filebrowser-extension/src/index.ts:1031
 msgid "Open from path"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:1025 packages/filebrowser-extension/src/index.ts:1029
+#: packages/filebrowser-extension/src/index.ts:1032 packages/filebrowser-extension/src/index.ts:1040
 msgid "Path"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:1027 packages/filebrowser-extension/src/index.ts:1031
+#: packages/filebrowser-extension/src/index.ts:1034 packages/filebrowser-extension/src/index.ts:1042
 msgid "Open Path"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:1028 packages/filebrowser-extension/src/index.ts:1032 packages/filebrowser-extension/src/index.ts:1117 packages/filebrowser-extension/src/index.ts:1121 packages/filebrowser-extension/src/index.ts:849 packages/filebrowser-extension/src/index.ts:853
+#: packages/filebrowser-extension/src/index.ts:1035 packages/filebrowser-extension/src/index.ts:1043 packages/filebrowser-extension/src/index.ts:1124 packages/filebrowser-extension/src/index.ts:1132 packages/filebrowser-extension/src/index.ts:856 packages/filebrowser-extension/src/index.ts:864
 msgid "Open"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:1063 packages/filebrowser-extension/src/index.ts:1067
+#: packages/filebrowser-extension/src/index.ts:1070 packages/filebrowser-extension/src/index.ts:1078
 msgid "Could not find path: %1"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:1065 packages/filebrowser-extension/src/index.ts:1069
+#: packages/filebrowser-extension/src/index.ts:1072 packages/filebrowser-extension/src/index.ts:1080
 msgid "Cannot open"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:1130 packages/filebrowser-extension/src/index.ts:1134 packages/fileeditor-extension/src/commands.ts:974 packages/fileeditor-extension/src/commands.ts:981 packages/terminal-extension/src/index.ts:488 packages/terminal-extension/src/index.ts:494
+#: packages/filebrowser-extension/src/index.ts:1137 packages/filebrowser-extension/src/index.ts:1145 packages/fileeditor-extension/src/commands.ts:979 packages/fileeditor-extension/src/commands.ts:980 packages/fileeditor-extension/src/commands.ts:981 packages/terminal-extension/src/index.ts:494
 msgid "Paste"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:1143 packages/filebrowser-extension/src/index.ts:1147 packages/filebrowser/src/opendialog.ts:153
+#: packages/filebrowser-extension/src/index.ts:1150 packages/filebrowser-extension/src/index.ts:1158 packages/filebrowser/src/opendialog.ts:172 packages/filebrowser/src/opendialog.ts:184
 msgid "New Folder"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:1155 packages/filebrowser-extension/src/index.ts:1159
+#: packages/filebrowser-extension/src/index.ts:1162 packages/filebrowser-extension/src/index.ts:1170
 msgid "New File"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:1167 packages/filebrowser-extension/src/index.ts:1171 packages/fileeditor-extension/src/commands.ts:809 packages/fileeditor-extension/src/commands.ts:816
+#: packages/filebrowser-extension/src/index.ts:1174 packages/filebrowser-extension/src/index.ts:1182 packages/fileeditor-extension/src/commands.ts:816 packages/fileeditor-extension/src/commands.ts:817
 msgid "New Markdown File"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:1179 packages/filebrowser-extension/src/index.ts:1183
+#: packages/filebrowser-extension/src/index.ts:1186 packages/filebrowser-extension/src/index.ts:1194
 msgid "Refresh the file browser."
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:1180 packages/filebrowser-extension/src/index.ts:1184 packages/filebrowser/src/opendialog.ts:168
+#: packages/filebrowser-extension/src/index.ts:1187 packages/filebrowser-extension/src/index.ts:1195 packages/filebrowser/src/opendialog.ts:187 packages/filebrowser/src/opendialog.ts:199
 msgid "Refresh File List"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:1220 packages/filebrowser-extension/src/index.ts:1224
+#: packages/filebrowser-extension/src/index.ts:1235 packages/filebrowser-extension/src/index.ts:1243
 msgid "Copy Path"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:1232 packages/filebrowser-extension/src/index.ts:1236 packages/mainmenu-extension/src/index.ts:531 packages/notebook-extension/src/index.ts:2332 packages/notebook-extension/src/index.ts:2337 packages/notebook-extension/src/index.ts:2356 packages/running-extension/src/kernels.ts:118 packages/running-extension/src/kernels.ts:66
+#: packages/filebrowser-extension/src/index.ts:1247 packages/filebrowser-extension/src/index.ts:1255 packages/mainmenu-extension/src/index.ts:529 packages/mainmenu-extension/src/index.ts:531 packages/notebook-extension/src/index.ts:2389 packages/notebook-extension/src/index.ts:2396 packages/notebook-extension/src/index.ts:2407 packages/running-extension/src/kernels.ts:118 packages/running-extension/src/kernels.ts:66 packages/running-extension/src/kernels.tsx:139 packages/running-extension/src/kernels.tsx:86
 msgid "Shut Down Kernel"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:1236 packages/filebrowser-extension/src/index.ts:1240
+#: packages/filebrowser-extension/src/index.ts:1251 packages/filebrowser-extension/src/index.ts:1259
 msgid "Show Last Modified Column"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:1252 packages/filebrowser-extension/src/index.ts:1272
-msgid "Show File Size Column"
+#: packages/filebrowser-extension/src/index.ts:1267 packages/filebrowser-extension/src/index.ts:1275
+msgid "Show Full Path"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:1256
+#: packages/filebrowser-extension/src/index.ts:1283 packages/filebrowser-extension/src/index.ts:1291
 msgid "Sort Notebooks Above Files"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:1268 packages/filebrowser-extension/src/index.ts:1288
+#: packages/filebrowser-extension/src/index.ts:1299 packages/filebrowser-extension/src/index.ts:1307
+msgid "Show File Size Column"
+msgstr ""
+
+#: packages/filebrowser-extension/src/index.ts:1315 packages/filebrowser-extension/src/index.ts:1323
 msgid "Show Hidden Files"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:1285 packages/filebrowser-extension/src/index.ts:1305
+#: packages/filebrowser-extension/src/index.ts:1332 packages/filebrowser-extension/src/index.ts:1340
 msgid "Show File Checkboxes"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:1301 packages/filebrowser-extension/src/index.ts:1321
+#: packages/filebrowser-extension/src/index.ts:1348 packages/filebrowser-extension/src/index.ts:1356
 msgid "Search on File Names"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:1370 packages/filebrowser-extension/src/index.ts:1390
+#: packages/filebrowser-extension/src/index.ts:1417 packages/filebrowser-extension/src/index.ts:1425
 msgid "No browser for path"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:389 packages/filebrowser-extension/src/index.ts:393
-msgid "Copy Download Link"
-msgstr ""
-
-#: packages/filebrowser-extension/src/index.ts:432 packages/filebrowser-extension/src/index.ts:436
+#: packages/filebrowser-extension/src/index.ts:340 packages/filebrowser-extension/src/index.ts:439
 msgid "File Browser Section"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:443 packages/filebrowser-extension/src/index.ts:447
+#: packages/filebrowser-extension/src/index.ts:342 packages/filebrowser-extension/src/index.ts:354 packages/filebrowser-extension/src/index.ts:452 packages/filebrowser-extension/src/index.ts:504 packages/filebrowser-extension/src/index.ts:512 packages/filebrowser/src/browser.ts:73 packages/filebrowser/src/browser.ts:74
+msgid "File Browser"
+msgstr "Browser Fișiere"
+
+#: packages/filebrowser-extension/src/index.ts:352 packages/filebrowser-extension/src/index.ts:450
 msgid "File Browser (%1)"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:445 packages/filebrowser-extension/src/index.ts:449 packages/filebrowser-extension/src/index.ts:497 packages/filebrowser-extension/src/index.ts:501 packages/filebrowser/src/browser.ts:75
-msgid "File Browser"
-msgstr "Browser Fișiere"
+#: packages/filebrowser-extension/src/index.ts:396 packages/filebrowser-extension/src/index.ts:427
+msgid "Copy Download Link"
+msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:475 packages/filebrowser-extension/src/index.ts:479
+#: packages/filebrowser-extension/src/index.ts:482 packages/filebrowser-extension/src/index.ts:490
 msgid "Filter files by name"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:508 packages/filebrowser-extension/src/index.ts:512
+#: packages/filebrowser-extension/src/index.ts:515 packages/filebrowser-extension/src/index.ts:523
 msgid "Open the file browser for the provided `path`."
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:540 packages/filebrowser-extension/src/index.ts:544
+#: packages/filebrowser-extension/src/index.ts:547 packages/filebrowser-extension/src/index.ts:555
 msgid "Hide the file browser."
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:550 packages/filebrowser-extension/src/index.ts:554
+#: packages/filebrowser-extension/src/index.ts:557 packages/filebrowser-extension/src/index.ts:565
 msgid "Show Active File in File Browser"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:647 packages/filebrowser-extension/src/index.ts:651
+#: packages/filebrowser-extension/src/index.ts:654 packages/filebrowser-extension/src/index.ts:662
 msgid "Copy Shareable Link"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:771 packages/filebrowser-extension/src/index.ts:775
+#: packages/filebrowser-extension/src/index.ts:778 packages/filebrowser-extension/src/index.ts:786
 msgid "Open in Simple Mode"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:837 packages/filebrowser-extension/src/index.ts:841
+#: packages/filebrowser-extension/src/index.ts:844 packages/filebrowser-extension/src/index.ts:852
 msgid "Open from URL…"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:839 packages/filebrowser-extension/src/index.ts:843
+#: packages/filebrowser-extension/src/index.ts:846 packages/filebrowser-extension/src/index.ts:854
 msgid "Open from URL"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:846 packages/filebrowser-extension/src/index.ts:850
+#: packages/filebrowser-extension/src/index.ts:853 packages/filebrowser-extension/src/index.ts:861
 msgid "URL"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:848 packages/filebrowser-extension/src/index.ts:852
+#: packages/filebrowser-extension/src/index.ts:855 packages/filebrowser-extension/src/index.ts:863
 msgid "Open URL"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:867 packages/filebrowser-extension/src/index.ts:871
+#: packages/filebrowser-extension/src/index.ts:874 packages/filebrowser-extension/src/index.ts:882
 msgid "Could not open URL: %1"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:869 packages/filebrowser-extension/src/index.ts:873
+#: packages/filebrowser-extension/src/index.ts:876 packages/filebrowser-extension/src/index.ts:884
 msgid "Cannot fetch"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:882 packages/filebrowser-extension/src/index.ts:886 packages/filebrowser/src/upload.ts:52
+#: packages/filebrowser-extension/src/index.ts:889 packages/filebrowser-extension/src/index.ts:897 packages/filebrowser/src/upload.ts:52
 msgctxt "showErrorMessage"
 msgid "Upload Error"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:935 packages/filebrowser-extension/src/index.ts:939 packages/fileeditor-extension/src/commands.ts:947 packages/fileeditor-extension/src/commands.ts:954 packages/terminal-extension/src/index.ts:463 packages/terminal-extension/src/index.ts:469
+#: packages/filebrowser-extension/src/index.ts:942 packages/filebrowser-extension/src/index.ts:950 packages/fileeditor-extension/src/commands.ts:952 packages/fileeditor-extension/src/commands.ts:953 packages/fileeditor-extension/src/commands.ts:954 packages/terminal-extension/src/index.ts:469
 msgid "Copy"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:948 packages/filebrowser-extension/src/index.ts:952 packages/fileeditor-extension/src/commands.ts:913 packages/fileeditor-extension/src/commands.ts:920
+#: packages/filebrowser-extension/src/index.ts:955 packages/filebrowser-extension/src/index.ts:963 packages/fileeditor-extension/src/commands.ts:918 packages/fileeditor-extension/src/commands.ts:919 packages/fileeditor-extension/src/commands.ts:920
 msgid "Cut"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:960 packages/filebrowser-extension/src/index.ts:964
+#: packages/filebrowser-extension/src/index.ts:967 packages/filebrowser-extension/src/index.ts:975
 msgid "Duplicate"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:964 packages/filebrowser-extension/src/index.ts:968
+#: packages/filebrowser-extension/src/index.ts:971 packages/filebrowser-extension/src/index.ts:979
 msgid "Update the file browser to display the provided `path`."
 msgstr ""
 
-#: packages/filebrowser/src/browser.ts:372 packages/filebrowser/src/browser.ts:388
+#: packages/filebrowser/src/browser.ts:397 packages/filebrowser/src/browser.ts:403
 msgid "Directory not found"
 msgstr ""
 
-#: packages/filebrowser/src/browser.ts:373 packages/filebrowser/src/browser.ts:389 packages/filebrowser/src/model.ts:298
+#: packages/filebrowser/src/browser.ts:398 packages/filebrowser/src/browser.ts:404 packages/filebrowser/src/model.ts:291 packages/filebrowser/src/model.ts:298
 msgid "Directory not found: \"%1\""
 msgstr ""
 
-#: packages/filebrowser/src/browser.ts:69
+#: packages/filebrowser/src/browser.ts:67 packages/filebrowser/src/browser.ts:68
 msgid "file browser"
 msgstr ""
 
-#: packages/filebrowser/src/crumbs.ts:175 packages/filebrowser/src/crumbs.ts:180 packages/filebrowser/src/crumbs.ts:194 packages/filebrowser/src/crumbs.ts:199
+#: packages/filebrowser/src/crumbs.ts:192 packages/filebrowser/src/crumbs.ts:219
 msgid "Open Error"
 msgstr ""
 
-#: packages/filebrowser/src/crumbs.ts:302 packages/filebrowser/src/crumbs.ts:307
+#: packages/filebrowser/src/crumbs.ts:327
 msgid "Move Error"
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:1120 packages/filebrowser/src/listing.ts:1136
+#: packages/filebrowser/src/listing.ts:1136 packages/filebrowser/src/listing.ts:1157 packages/filebrowser/src/listing.ts:1209
 msgctxt "showErrorMessage"
 msgid "Open directory"
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:1395 packages/filebrowser/src/listing.ts:1411
+#: packages/filebrowser/src/listing.ts:1411 packages/filebrowser/src/listing.ts:1432 packages/filebrowser/src/listing.ts:1484
 msgid "Error Uploading Folder"
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:1396 packages/filebrowser/src/listing.ts:1412
+#: packages/filebrowser/src/listing.ts:1412 packages/filebrowser/src/listing.ts:1433 packages/filebrowser/src/listing.ts:1485
 msgid "Drag and Drop is currently not supported for folders"
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:1515 packages/filebrowser/src/listing.ts:1531
+#: packages/filebrowser/src/listing.ts:1531 packages/filebrowser/src/listing.ts:1552 packages/filebrowser/src/listing.ts:1604
 msgctxt "showErrorMessage"
 msgid "Error while copying/moving files"
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:1814 packages/filebrowser/src/listing.ts:1830
+#: packages/filebrowser/src/listing.ts:1830 packages/filebrowser/src/listing.ts:1851 packages/filebrowser/src/listing.ts:1903
 msgctxt "showErrorMessage"
 msgid "Delete Failed"
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:1877 packages/filebrowser/src/listing.ts:1893
+#: packages/filebrowser/src/listing.ts:1893 packages/filebrowser/src/listing.ts:1914 packages/filebrowser/src/listing.ts:1966
 msgctxt "showErrorMessage"
 msgid "\"%1\" is not a valid name for a file. Names must have nonzero length, and cannot include \"/\", \"\\\", or \":\""
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:1896 packages/filebrowser/src/listing.ts:1912
+#: packages/filebrowser/src/listing.ts:1912 packages/filebrowser/src/listing.ts:1933 packages/filebrowser/src/listing.ts:1985
 msgctxt "showErrorMessage"
 msgid "Rename Error"
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:2260 packages/filebrowser/src/listing.ts:2277 packages/filebrowser/src/listing.ts:2279
+#: packages/filebrowser/src/listing.ts:2279 packages/filebrowser/src/listing.ts:2300 packages/filebrowser/src/listing.ts:2375
 msgid "Last Modified"
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:2261 packages/filebrowser/src/listing.ts:2278 packages/filebrowser/src/listing.ts:2280
+#: packages/filebrowser/src/listing.ts:2280 packages/filebrowser/src/listing.ts:2301 packages/filebrowser/src/listing.ts:2377
 msgid "File Size"
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:2549 packages/filebrowser/src/listing.ts:2566 packages/filebrowser/src/listing.ts:2568
+#: packages/filebrowser/src/listing.ts:2374 packages/settingeditor/src/pluginlist.tsx:461
+msgid "Modified"
+msgstr ""
+
+#: packages/filebrowser/src/listing.ts:2568 packages/filebrowser/src/listing.ts:2589 packages/filebrowser/src/listing.ts:2696
 msgid "Name: %1"
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:2555 packages/filebrowser/src/listing.ts:2572 packages/filebrowser/src/listing.ts:2574
+#: packages/filebrowser/src/listing.ts:2574 packages/filebrowser/src/listing.ts:2595 packages/filebrowser/src/listing.ts:2702
 msgid "\n"
 "Size: %1"
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:2565 packages/filebrowser/src/listing.ts:2582 packages/filebrowser/src/listing.ts:2584
+#: packages/filebrowser/src/listing.ts:2584 packages/filebrowser/src/listing.ts:2605 packages/filebrowser/src/listing.ts:2712
 msgid "\n"
 "Path: %1"
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:2572 packages/filebrowser/src/listing.ts:2589 packages/filebrowser/src/listing.ts:2591
+#: packages/filebrowser/src/listing.ts:2591 packages/filebrowser/src/listing.ts:2612 packages/filebrowser/src/listing.ts:2719
 msgid "\n"
 "Created: %1"
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:2578 packages/filebrowser/src/listing.ts:2595 packages/filebrowser/src/listing.ts:2597
+#: packages/filebrowser/src/listing.ts:2597 packages/filebrowser/src/listing.ts:2618 packages/filebrowser/src/listing.ts:2725
 msgid "\n"
 "Modified: %1"
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:2583 packages/filebrowser/src/listing.ts:2600 packages/filebrowser/src/listing.ts:2602
+#: packages/filebrowser/src/listing.ts:2602 packages/filebrowser/src/listing.ts:2623 packages/filebrowser/src/listing.ts:2730
 msgid "\n"
 "Writable: %1"
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:2608 packages/filebrowser/src/listing.ts:2625 packages/filebrowser/src/listing.ts:2627
+#: packages/filebrowser/src/listing.ts:2627 packages/filebrowser/src/listing.ts:2648 packages/filebrowser/src/listing.ts:2755
 msgid "Deselect directory \"%1\""
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:2609 packages/filebrowser/src/listing.ts:2626 packages/filebrowser/src/listing.ts:2628
+#: packages/filebrowser/src/listing.ts:2628 packages/filebrowser/src/listing.ts:2649 packages/filebrowser/src/listing.ts:2756
 msgid "Select directory \"%1\""
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:2612 packages/filebrowser/src/listing.ts:2629 packages/filebrowser/src/listing.ts:2631
+#: packages/filebrowser/src/listing.ts:2631 packages/filebrowser/src/listing.ts:2652 packages/filebrowser/src/listing.ts:2759
 msgid "Deselect file \"%1\""
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:2613 packages/filebrowser/src/listing.ts:2630 packages/filebrowser/src/listing.ts:2632
+#: packages/filebrowser/src/listing.ts:2632 packages/filebrowser/src/listing.ts:2653 packages/filebrowser/src/listing.ts:2760
 msgid "Select file \"%1\""
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:2687 packages/filebrowser/src/listing.ts:2704 packages/filebrowser/src/listing.ts:2706
+#: packages/filebrowser/src/listing.ts:2706 packages/filebrowser/src/listing.ts:2727 packages/filebrowser/src/listing.ts:2833
 msgid "%1 Item"
 msgid_plural "%1 Items"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 
-#: packages/filebrowser/src/listing.ts:396 packages/filebrowser/src/listing.ts:400
+#: packages/filebrowser/src/listing.ts:400 packages/filebrowser/src/listing.ts:403
 msgctxt "showErrorMessage"
 msgid "Paste Error"
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:416 packages/filebrowser/src/listing.ts:420
+#: packages/filebrowser/src/listing.ts:420 packages/filebrowser/src/listing.ts:423
 msgid "Are you sure you want to permanently delete: %1?"
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:420 packages/filebrowser/src/listing.ts:424
+#: packages/filebrowser/src/listing.ts:424 packages/filebrowser/src/listing.ts:427
 msgid "Are you sure you want to permanently delete the %1 selected item?"
 msgid_plural "Are you sure you want to permanently delete the %1 selected items?"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 
-#: packages/filebrowser/src/listing.ts:472 packages/filebrowser/src/listing.ts:476
+#: packages/filebrowser/src/listing.ts:476 packages/filebrowser/src/listing.ts:479
 msgctxt "showErrorMessage"
 msgid "Duplicate file"
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:512 packages/filebrowser/src/listing.ts:516
+#: packages/filebrowser/src/listing.ts:516 packages/filebrowser/src/listing.ts:519
 msgctxt "showErrorMessage"
 msgid "Shut down kernel"
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:852 packages/filebrowser/src/listing.ts:856
+#: packages/filebrowser/src/listing.ts:856 packages/filebrowser/src/listing.ts:877 packages/filebrowser/src/listing.ts:974
 msgid "Deselect all files and directories"
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:853 packages/filebrowser/src/listing.ts:857
+#: packages/filebrowser/src/listing.ts:857 packages/filebrowser/src/listing.ts:878 packages/filebrowser/src/listing.ts:975
 msgid "Select all files and directories"
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:906 packages/filebrowser/src/listing.ts:910
+#: packages/filebrowser/src/listing.ts:899 packages/filebrowser/src/listing.ts:910 packages/filebrowser/src/listing.ts:931
 msgid "unknown"
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:908 packages/filebrowser/src/listing.ts:912
+#: packages/filebrowser/src/listing.ts:901 packages/filebrowser/src/listing.ts:912 packages/filebrowser/src/listing.ts:933
 msgid "%1\n"
 "Kernel: %2"
 msgstr ""
 
-#: packages/filebrowser/src/model.ts:414
+#: packages/filebrowser/src/model.ts:407 packages/filebrowser/src/model.ts:414
 msgid "Cannot upload file (>%1 MB). %2"
 msgstr ""
 
-#: packages/filebrowser/src/model.ts:443
+#: packages/filebrowser/src/model.ts:436 packages/filebrowser/src/model.ts:443
 msgid "Large file size warning"
 msgstr ""
 
-#: packages/filebrowser/src/model.ts:444
+#: packages/filebrowser/src/model.ts:437 packages/filebrowser/src/model.ts:444
 msgid "The file size is %1 MB. Do you still want to upload it?"
 msgstr ""
 
-#: packages/filebrowser/src/model.ts:450
+#: packages/filebrowser/src/model.ts:443 packages/filebrowser/src/model.ts:450
 msgid "Upload"
 msgstr ""
 
 #: packages/filebrowser/src/model.ts:83
 msgid "Files still uploading"
 msgstr ""
 
@@ -5020,168 +5460,160 @@
 msgid "Uploading…"
 msgstr ""
 
 #: packages/filebrowser/src/uploadstatus.tsx:96
 msgid "Complete!"
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:1100 packages/fileeditor-extension/src/commands.ts:1107 packages/fileeditor-extension/src/commands.ts:1114 packages/fileeditor-extension/src/commands.ts:1121 packages/fileeditor-extension/src/commands.ts:1130 packages/fileeditor-extension/src/commands.ts:1137 packages/launcher/src/widget.tsx:117 packages/launcher/src/widget.tsx:127 packages/launcher/src/widget.tsx:295 packages/terminal-extension/src/index.ts:271
+#: packages/fileeditor-extension/src/commands.ts:1105 packages/fileeditor-extension/src/commands.ts:1107 packages/fileeditor-extension/src/commands.ts:1119 packages/fileeditor-extension/src/commands.ts:1121 packages/fileeditor-extension/src/commands.ts:1135 packages/fileeditor-extension/src/commands.ts:1136 packages/fileeditor-extension/src/commands.ts:1137 packages/fileeditor-extension/src/commands.ts:1150 packages/fileeditor-extension/src/commands.ts:1166 packages/launcher/src/widget.tsx:117 packages/launcher/src/widget.tsx:127 packages/launcher/src/widget.tsx:296 packages/terminal-extension/src/index.ts:271
 msgid "Other"
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:1160 packages/fileeditor-extension/src/commands.ts:1167 packages/fileeditor-extension/src/commands.ts:1182 packages/fileeditor-extension/src/commands.ts:1189 packages/fileeditor-extension/src/commands.ts:1197 packages/fileeditor-extension/src/commands.ts:1204 packages/fileeditor-extension/src/commands.ts:1212 packages/fileeditor-extension/src/commands.ts:1219 packages/fileeditor-extension/src/commands.ts:1230 packages/fileeditor-extension/src/commands.ts:1237
+#: packages/fileeditor-extension/src/commands.ts:1165 packages/fileeditor-extension/src/commands.ts:1167 packages/fileeditor-extension/src/commands.ts:1187 packages/fileeditor-extension/src/commands.ts:1189 packages/fileeditor-extension/src/commands.ts:1196 packages/fileeditor-extension/src/commands.ts:1202 packages/fileeditor-extension/src/commands.ts:1204 packages/fileeditor-extension/src/commands.ts:1217 packages/fileeditor-extension/src/commands.ts:1218 packages/fileeditor-extension/src/commands.ts:1219 packages/fileeditor-extension/src/commands.ts:1233 packages/fileeditor-extension/src/commands.ts:1235 packages/fileeditor-extension/src/commands.ts:1237 packages/fileeditor-extension/src/commands.ts:1248 packages/fileeditor-extension/src/commands.ts:1266
 msgid "Text Editor"
 msgstr "Editor de Text"
 
-#: packages/fileeditor-extension/src/commands.ts:1358 packages/fileeditor-extension/src/commands.ts:1360 packages/fileeditor-extension/src/commands.ts:1367
+#: packages/fileeditor-extension/src/commands.ts:1365 packages/fileeditor-extension/src/commands.ts:1367 packages/fileeditor-extension/src/commands.ts:1396
 msgid "Code Viewer"
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:1377 packages/fileeditor-extension/src/commands.ts:1379 packages/fileeditor-extension/src/commands.ts:1386
+#: packages/fileeditor-extension/src/commands.ts:1384 packages/fileeditor-extension/src/commands.ts:1386 packages/fileeditor-extension/src/commands.ts:1415
 msgid "Open Code Viewer"
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:279 packages/fileeditor-extension/src/commands.ts:280
+#: packages/fileeditor-extension/src/commands.ts:280 packages/fileeditor-extension/src/commands.ts:281
 msgid "Increase Text Editor Font Size"
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:283 packages/fileeditor-extension/src/commands.ts:284
+#: packages/fileeditor-extension/src/commands.ts:284 packages/fileeditor-extension/src/commands.ts:285
 msgid "Decrease Text Editor Font Size"
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:306 packages/fileeditor-extension/src/commands.ts:307 packages/fileeditor-extension/src/commands.ts:310 packages/fileeditor-extension/src/commands.ts:311 packages/mainmenu-extension/src/index.ts:576 packages/notebook-extension/src/index.ts:2963 packages/notebook-extension/src/index.ts:2969 packages/notebook-extension/src/index.ts:2988
+#: packages/fileeditor-extension/src/commands.ts:307 packages/fileeditor-extension/src/commands.ts:308 packages/fileeditor-extension/src/commands.ts:311 packages/fileeditor-extension/src/commands.ts:312 packages/mainmenu-extension/src/index.ts:573 packages/mainmenu-extension/src/index.ts:576 packages/notebook-extension/src/index.ts:3040 packages/notebook-extension/src/index.ts:3047 packages/notebook-extension/src/index.ts:3070
 msgid "Show Line Numbers"
 msgstr "Arată numerele rândurilor"
 
-#: packages/fileeditor-extension/src/commands.ts:311 packages/fileeditor-extension/src/commands.ts:312
+#: packages/fileeditor-extension/src/commands.ts:312 packages/fileeditor-extension/src/commands.ts:313
 msgid "Show the line numbers for the current file."
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:351 packages/fileeditor-extension/src/commands.ts:352
+#: packages/fileeditor-extension/src/commands.ts:352 packages/fileeditor-extension/src/commands.ts:353
 msgid "Word Wrap"
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:355 packages/fileeditor-extension/src/commands.ts:356 packages/mainmenu-extension/src/index.ts:600
+#: packages/fileeditor-extension/src/commands.ts:356 packages/fileeditor-extension/src/commands.ts:357 packages/mainmenu-extension/src/index.ts:595 packages/mainmenu-extension/src/index.ts:600
 msgid "Wrap Words"
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:356 packages/fileeditor-extension/src/commands.ts:357
+#: packages/fileeditor-extension/src/commands.ts:357 packages/fileeditor-extension/src/commands.ts:358
 msgid "Wrap words for the current file."
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:382 packages/fileeditor-extension/src/commands.ts:383 packages/fileeditor-extension/src/index.ts:145
+#: packages/fileeditor-extension/src/commands.ts:383 packages/fileeditor-extension/src/commands.ts:384 packages/fileeditor-extension/src/index.ts:147
 msgctxt "v4"
 msgid "Spaces: %1"
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:384 packages/fileeditor-extension/src/commands.ts:385 packages/fileeditor-extension/src/index.ts:138
+#: packages/fileeditor-extension/src/commands.ts:385 packages/fileeditor-extension/src/commands.ts:386 packages/fileeditor-extension/src/index.ts:140
 msgid "Indent with Tab"
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:429 packages/fileeditor-extension/src/commands.ts:430
+#: packages/fileeditor-extension/src/commands.ts:430 packages/fileeditor-extension/src/commands.ts:431
 msgid "Change match brackets for the current file."
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:467 packages/fileeditor-extension/src/commands.ts:468
+#: packages/fileeditor-extension/src/commands.ts:468 packages/fileeditor-extension/src/commands.ts:469
 msgid "Auto Close Brackets in Text Editor"
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:495 packages/fileeditor-extension/src/commands.ts:496
+#: packages/fileeditor-extension/src/commands.ts:496 packages/fileeditor-extension/src/commands.ts:497
 msgid "Auto Close Brackets"
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:510 packages/fileeditor-extension/src/commands.ts:511
+#: packages/fileeditor-extension/src/commands.ts:511 packages/fileeditor-extension/src/commands.ts:512
 msgid "Editor Theme"
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:538 packages/fileeditor-extension/src/commands.ts:539 packages/mainmenu-extension/src/index.ts:324
+#: packages/fileeditor-extension/src/commands.ts:539 packages/fileeditor-extension/src/commands.ts:540 packages/mainmenu-extension/src/index.ts:320 packages/mainmenu-extension/src/index.ts:324
 msgid "Go to Line…"
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:563 packages/fileeditor-extension/src/commands.ts:564
+#: packages/fileeditor-extension/src/commands.ts:564 packages/fileeditor-extension/src/commands.ts:565
 msgid "Change editor language."
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:601 packages/fileeditor-extension/src/commands.ts:608
+#: packages/fileeditor-extension/src/commands.ts:608 packages/fileeditor-extension/src/commands.ts:609
 msgid "Replace Selection in Editor"
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:619 packages/fileeditor-extension/src/commands.ts:626
+#: packages/fileeditor-extension/src/commands.ts:626 packages/fileeditor-extension/src/commands.ts:627
 msgid "Create Console for Editor"
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:640 packages/fileeditor-extension/src/commands.ts:647
+#: packages/fileeditor-extension/src/commands.ts:647 packages/fileeditor-extension/src/commands.ts:648
 msgid "Restart Kernel"
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:705 packages/fileeditor-extension/src/commands.ts:712
+#: packages/fileeditor-extension/src/commands.ts:712 packages/fileeditor-extension/src/commands.ts:713
 msgid "Run Selected Code"
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:743 packages/fileeditor-extension/src/commands.ts:750
+#: packages/fileeditor-extension/src/commands.ts:750 packages/fileeditor-extension/src/commands.ts:751
 msgid "Run All Code"
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:770 packages/fileeditor-extension/src/commands.ts:777
+#: packages/fileeditor-extension/src/commands.ts:777 packages/fileeditor-extension/src/commands.ts:778
 msgid "Show Markdown Preview"
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:781 packages/fileeditor-extension/src/commands.ts:788
+#: packages/fileeditor-extension/src/commands.ts:788 packages/fileeditor-extension/src/commands.ts:789
 msgid "New Text File"
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:783 packages/fileeditor-extension/src/commands.ts:790
+#: packages/fileeditor-extension/src/commands.ts:790 packages/fileeditor-extension/src/commands.ts:791
 msgid "Text File"
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:786 packages/fileeditor-extension/src/commands.ts:793
+#: packages/fileeditor-extension/src/commands.ts:793 packages/fileeditor-extension/src/commands.ts:794
 msgid "Create a new text file"
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:811 packages/fileeditor-extension/src/commands.ts:818
+#: packages/fileeditor-extension/src/commands.ts:818 packages/fileeditor-extension/src/commands.ts:819
 msgid "Create a new markdown file"
 msgstr ""
 
-#: packages/fileeditor-extension/src/commands.ts:847 packages/fileeditor-extension/src/commands.ts:854 packages/mainmenu-extension/src/index.ts:277 packages/notebook-extension/src/index.ts:3045 packages/notebook-extension/src/index.ts:3051 packages/notebook-extension/src/index.ts:3070
-msgid "Undo"
-msgstr ""
-
-#: packages/fileeditor-extension/src/commands.ts:878 packages/fileeditor-extension/src/commands.ts:885 packages/mainmenu-extension/src/index.ts:288 packages/notebook-extension/src/index.ts:3031 packages/notebook-extension/src/index.ts:3037 packages/notebook-extension/src/index.ts:3056
-msgid "Redo"
-msgstr ""
-
-#: packages/fileeditor-extension/src/commands.ts:992 packages/fileeditor-extension/src/commands.ts:999
+#: packages/fileeditor-extension/src/commands.ts:997 packages/fileeditor-extension/src/commands.ts:998 packages/fileeditor-extension/src/commands.ts:999
 msgid "Select All"
 msgstr ""
 
-#: packages/fileeditor-extension/src/index.ts:307
+#: packages/fileeditor-extension/src/index.ts:309
 msgid "Editor"
 msgstr ""
 
-#: packages/fileeditor-extension/src/index.ts:330
+#: packages/fileeditor-extension/src/index.ts:332
 msgid "New Python File"
 msgstr ""
 
-#: packages/fileeditor-extension/src/index.ts:331
+#: packages/fileeditor-extension/src/index.ts:333
 msgid "Create a new Python file"
 msgstr ""
 
-#: packages/fileeditor-extension/src/index.ts:342
+#: packages/fileeditor-extension/src/index.ts:344
 msgid "New Julia File"
 msgstr ""
 
-#: packages/fileeditor-extension/src/index.ts:343
+#: packages/fileeditor-extension/src/index.ts:345
 msgid "Create a new Julia file"
 msgstr ""
 
-#: packages/fileeditor-extension/src/index.ts:354
+#: packages/fileeditor-extension/src/index.ts:356
 msgid "New R File"
 msgstr ""
 
-#: packages/fileeditor-extension/src/index.ts:355
+#: packages/fileeditor-extension/src/index.ts:357
 msgid "Create a new R file"
 msgstr ""
 
 #: packages/fileeditor/src/syntaxstatus.tsx:66
 msgid "Change text editor syntax highlighting"
 msgstr ""
 
@@ -5209,47 +5641,51 @@
 msgid "© 2015-2023 Project Jupyter Contributors"
 msgstr ""
 
 #: packages/help-extension/src/index.tsx:186
 msgid "Jupyter Forum"
 msgstr ""
 
-#: packages/help-extension/src/index.tsx:223
+#: packages/help-extension/src/index.tsx:243
+msgid "Open the provided `url` in a tab."
+msgstr ""
+
+#: packages/help-extension/src/index.tsx:300
 msgid "JupyterLab Reference"
 msgstr ""
 
-#: packages/help-extension/src/index.tsx:227
+#: packages/help-extension/src/index.tsx:304
 msgid "JupyterLab FAQ"
 msgstr ""
 
-#: packages/help-extension/src/index.tsx:231
+#: packages/help-extension/src/index.tsx:308
 msgid "Jupyter Reference"
 msgstr ""
 
-#: packages/help-extension/src/index.tsx:235
+#: packages/help-extension/src/index.tsx:312
 msgid "Markdown Reference"
 msgstr ""
 
-#: packages/help-extension/src/index.tsx:268
-msgid "Open the provided `url` in a tab."
+#: packages/help-extension/src/index.tsx:403
+msgid "About the %1 Kernel"
 msgstr ""
 
-#: packages/help-extension/src/index.tsx:384
-msgid "About the %1 Kernel"
+#: packages/help-extension/src/index.tsx:409
+msgid "Kernel Icon"
 msgstr ""
 
-#: packages/help-extension/src/index.tsx:480
+#: packages/help-extension/src/index.tsx:501
 msgid "Download All Licenses as"
 msgstr ""
 
-#: packages/help-extension/src/index.tsx:481 packages/help-extension/src/licenses.tsx:441
+#: packages/help-extension/src/index.tsx:502 packages/help-extension/src/licenses.tsx:441
 msgid "Licenses"
 msgstr ""
 
-#: packages/help-extension/src/index.tsx:482
+#: packages/help-extension/src/index.tsx:503
 msgid "Refresh Licenses"
 msgstr ""
 
 #: packages/help-extension/src/index.tsx:93
 msgid "About %1"
 msgstr ""
 
@@ -5312,74 +5748,67 @@
 "    Only enable for files you trust."
 msgstr ""
 
 #: packages/htmlviewer/src/widget.tsx:205
 msgid "Action disabled as the file is not trusted."
 msgstr ""
 
-#: packages/htmlviewer/src/widget.tsx:240 packages/htmlviewer/src/widget.tsx:279 packages/htmlviewer/src/widget.tsx:280
+#: packages/htmlviewer/src/widget.tsx:279
 msgid "Rerender HTML Document"
 msgstr ""
 
-#: packages/htmlviewer/src/widget.tsx:315
+#: packages/htmlviewer/src/widget.tsx:357
 msgid "Whether the HTML file is trusted.\n"
-"Trusting the file allows scripts to run in it,\n"
+"Trusting the file allows opening pop-ups and running scripts\n"
 "which may result in security risks.\n"
 "Only enable for files you trust."
 msgstr ""
 
-#: packages/htmlviewer/src/widget.tsx:321 packages/htmlviewer/src/widget.tsx:363 packages/htmlviewer/src/widget.tsx:364
+#: packages/htmlviewer/src/widget.tsx:363
 msgid "Distrust HTML"
 msgstr ""
 
-#: packages/htmlviewer/src/widget.tsx:322 packages/htmlviewer/src/widget.tsx:364 packages/htmlviewer/src/widget.tsx:365
+#: packages/htmlviewer/src/widget.tsx:364
 msgid "Trust HTML"
 msgstr ""
 
-#: packages/htmlviewer/src/widget.tsx:357 packages/htmlviewer/src/widget.tsx:358
-msgid "Whether the HTML file is trusted.\n"
-"Trusting the file allows opening pop-ups and running scripts\n"
-"which may result in security risks.\n"
-"Only enable for files you trust."
-msgstr ""
-
-#: packages/hub-extension/src/index.ts:166
+#: packages/hub-extension/src/index.ts:173
 msgid "Server unavailable or unreachable"
 msgstr ""
 
-#: packages/hub-extension/src/index.ts:167
+#: packages/hub-extension/src/index.ts:174
 msgid "Your server at %1 is not running.\n"
 "Would you like to restart it?"
 msgstr ""
 
-#: packages/hub-extension/src/index.ts:67
+#: packages/hub-extension/src/index.ts:74
 msgid "Restart Server"
 msgstr ""
 
-#: packages/hub-extension/src/index.ts:68
+#: packages/hub-extension/src/index.ts:75
 msgid "Request that the Hub restart this server"
 msgstr ""
 
-#: packages/hub-extension/src/index.ts:75
+#: packages/hub-extension/src/index.ts:82
 msgid "Hub Control Panel"
 msgstr ""
 
-#: packages/hub-extension/src/index.ts:76
+#: packages/hub-extension/src/index.ts:83
 msgid "Open the Hub control panel in a new browser tab"
 msgstr ""
 
-#: packages/hub-extension/src/index.ts:83 packages/mainmenu-extension/src/index.ts:443
+#: packages/hub-extension/src/index.ts:90 packages/mainmenu-extension/src/index.ts:440 packages/mainmenu-extension/src/index.ts:443
 msgid "Log Out"
 msgstr ""
 
-#: packages/hub-extension/src/index.ts:84
+#: packages/hub-extension/src/index.ts:91
 msgid "Log out of the Hub"
 msgstr ""
 
-#: packages/hub-extension/src/index.ts:92
+#: packages/hub-extension/src/index.ts:99
 msgid "Hub"
 msgstr ""
 
 #: packages/imageviewer-extension/src/index.ts:128
 msgid "Image (Text)"
 msgstr ""
 
@@ -5443,27 +5872,23 @@
 msgid "Are you sure that you want to run arbitrary Javascript within your JupyterLab session?"
 msgstr ""
 
 #: packages/javascript-extension/src/index.ts:45 packages/rendermime/src/renderers.ts:66
 msgid "Run"
 msgstr ""
 
-#: packages/json-extension/src/component.tsx:78
-msgid "Filter…"
-msgstr ""
-
-#: packages/launcher-extension/src/index.ts:148 packages/launcher-extension/src/index.ts:94
+#: packages/launcher-extension/src/index.ts:138 packages/launcher-extension/src/index.ts:148 packages/launcher-extension/src/index.ts:84 packages/launcher-extension/src/index.ts:94
 msgid "Launcher"
 msgstr ""
 
-#: packages/launcher-extension/src/index.ts:72 packages/ui-components/src/icon/widgets/tabbarsvg.ts:31
+#: packages/launcher-extension/src/index.ts:62 packages/launcher-extension/src/index.ts:72 packages/ui-components/src/icon/widgets/tabbarsvg.ts:31
 msgid "New Launcher"
 msgstr ""
 
-#: packages/launcher/src/widget.tsx:272
+#: packages/launcher/src/widget.tsx:273
 msgctxt "Error"
 msgid "Launcher Error"
 msgstr ""
 
 #: packages/logconsole-extension/src/index.tsx:136 packages/logconsole/src/widget.ts:389
 msgid "Log Console"
 msgstr ""
@@ -5524,738 +5949,814 @@
 msgid "No source selected."
 msgstr "Nici o sursă selectata."
 
 #: packages/logconsole/src/widget.ts:402
 msgid "No log messages."
 msgstr ""
 
-#: packages/lsp-extension/src/index.ts:257 packages/lsp-extension/src/index.ts:280
+#: packages/lsp-extension/src/index.ts:285
 msgid "Language servers"
 msgstr ""
 
-#: packages/lsp-extension/src/index.ts:276 packages/lsp-extension/src/index.ts:299 packages/mainmenu-extension/src/index.ts:549 packages/running-extension/src/kernels.ts:67 packages/running/src/index.tsx:357 packages/terminal-extension/src/index.ts:323
+#: packages/lsp-extension/src/index.ts:304 packages/mainmenu-extension/src/index.ts:546 packages/mainmenu-extension/src/index.ts:549 packages/running-extension/src/kernels.ts:67 packages/running-extension/src/kernels.tsx:87 packages/running/src/index.tsx:357 packages/running/src/index.tsx:573 packages/terminal-extension/src/index.ts:323
 msgid "Shut Down All"
 msgstr "Oprește Tot"
 
-#: packages/lsp-extension/src/index.ts:277 packages/lsp-extension/src/index.ts:300
+#: packages/lsp-extension/src/index.ts:305
 msgid "Are you sure you want to permanently shut down all running language servers?"
 msgstr ""
 
-#: packages/lsp-extension/src/renderer.tsx:216
+#: packages/lsp-extension/src/renderer.tsx:223
 msgid "Server name:"
 msgstr ""
 
-#: packages/lsp-extension/src/renderer.tsx:233
+#: packages/lsp-extension/src/renderer.tsx:241
 msgid "is a required property"
 msgstr ""
 
-#: packages/lsp-extension/src/renderer.tsx:296
+#: packages/lsp-extension/src/renderer.tsx:304
 msgid "Add property"
 msgstr ""
 
-#: packages/lsp-extension/src/renderer.tsx:302
+#: packages/lsp-extension/src/renderer.tsx:310
 msgid "Remove server"
 msgstr ""
 
-#: packages/lsp-extension/src/renderer.tsx:573
+#: packages/lsp-extension/src/renderer.tsx:581
 msgid "Add server"
 msgstr ""
 
-#: packages/lsp/src/adapters/adapter.ts:455 packages/lsp/src/adapters/adapter.ts:458 packages/lsp/src/adapters/adapter.ts:473 packages/lsp/src/adapters/adapter.ts:476
+#: packages/lsp/src/adapters/adapter.ts:482 packages/lsp/src/adapters/adapter.ts:500
 msgid "Message from "
 msgstr ""
 
-#: packages/mainmenu-extension/src/index.ts:193
+#: packages/mainmenu-extension/src/index.ts:193 packages/mainmenu-extension/src/index.ts:194
 msgid "Open Edit Menu"
 msgstr ""
 
-#: packages/mainmenu-extension/src/index.ts:197
+#: packages/mainmenu-extension/src/index.ts:197 packages/mainmenu-extension/src/index.ts:198
 msgid "Open File Menu"
 msgstr ""
 
-#: packages/mainmenu-extension/src/index.ts:201
+#: packages/mainmenu-extension/src/index.ts:201 packages/mainmenu-extension/src/index.ts:202
 msgid "Open Kernel Menu"
 msgstr ""
 
-#: packages/mainmenu-extension/src/index.ts:205
+#: packages/mainmenu-extension/src/index.ts:205 packages/mainmenu-extension/src/index.ts:206
 msgid "Open Run Menu"
 msgstr ""
 
-#: packages/mainmenu-extension/src/index.ts:209
+#: packages/mainmenu-extension/src/index.ts:209 packages/mainmenu-extension/src/index.ts:210
 msgid "Open View Menu"
 msgstr ""
 
-#: packages/mainmenu-extension/src/index.ts:213
+#: packages/mainmenu-extension/src/index.ts:213 packages/mainmenu-extension/src/index.ts:214
 msgid "Open Settings Menu"
 msgstr ""
 
-#: packages/mainmenu-extension/src/index.ts:217
+#: packages/mainmenu-extension/src/index.ts:217 packages/mainmenu-extension/src/index.ts:218
 msgid "Open Tabs Menu"
 msgstr ""
 
-#: packages/mainmenu-extension/src/index.ts:221
+#: packages/mainmenu-extension/src/index.ts:221 packages/mainmenu-extension/src/index.ts:222
 msgid "Open Help Menu"
 msgstr ""
 
-#: packages/mainmenu-extension/src/index.ts:225
+#: packages/mainmenu-extension/src/index.ts:225 packages/mainmenu-extension/src/index.ts:226
 msgid "Open First Menu"
 msgstr ""
 
-#: packages/mainmenu-extension/src/index.ts:245
+#: packages/mainmenu-extension/src/index.ts:245 packages/mainmenu-extension/src/index.ts:246
 msgid "Kernel Operations"
 msgstr ""
 
-#: packages/mainmenu-extension/src/index.ts:301
+#: packages/mainmenu-extension/src/index.ts:299 packages/mainmenu-extension/src/index.ts:301
 msgid "Clear"
 msgstr ""
 
-#: packages/mainmenu-extension/src/index.ts:312
+#: packages/mainmenu-extension/src/index.ts:309 packages/mainmenu-extension/src/index.ts:312
 msgid "Clear All"
 msgstr ""
 
-#: packages/mainmenu-extension/src/index.ts:352
+#: packages/mainmenu-extension/src/index.ts:348 packages/mainmenu-extension/src/index.ts:352
 msgid "Close and Shut Down"
 msgstr "Închide și Oprește"
 
-#: packages/mainmenu-extension/src/index.ts:368
+#: packages/mainmenu-extension/src/index.ts:365 packages/mainmenu-extension/src/index.ts:368
 msgid "New Console for Activity"
 msgstr ""
 
+#: packages/mainmenu-extension/src/index.ts:372
+msgid "Shut down %1"
+msgstr ""
+
 #: packages/mainmenu-extension/src/index.ts:376
 msgid "Shut down JupyterLab"
 msgstr ""
 
-#: packages/mainmenu-extension/src/index.ts:381
+#: packages/mainmenu-extension/src/index.ts:377 packages/mainmenu-extension/src/index.ts:381
 msgid "Shutdown confirmation"
 msgstr ""
 
+#: packages/mainmenu-extension/src/index.ts:378
+msgid "Please confirm you want to shut down %1."
+msgstr ""
+
 #: packages/mainmenu-extension/src/index.ts:382
 msgid "Please confirm you want to shut down JupyterLab."
 msgstr ""
 
-#: packages/mainmenu-extension/src/index.ts:414
+#: packages/mainmenu-extension/src/index.ts:410 packages/mainmenu-extension/src/index.ts:414
 msgid "You have shut down the Jupyter server. You can now close this tab."
 msgstr ""
 
+#: packages/mainmenu-extension/src/index.ts:414
+msgid "To use %1 again, you will need to relaunch it."
+msgstr ""
+
 #: packages/mainmenu-extension/src/index.ts:418
 msgid "To use JupyterLab again, you will need to relaunch it."
 msgstr ""
 
-#: packages/mainmenu-extension/src/index.ts:425
+#: packages/mainmenu-extension/src/index.ts:422 packages/mainmenu-extension/src/index.ts:425
 msgid "Server stopped"
 msgstr ""
 
+#: packages/mainmenu-extension/src/index.ts:441
+msgid "Log out of %1"
+msgstr ""
+
 #: packages/mainmenu-extension/src/index.ts:444
 msgid "Log out of JupyterLab"
 msgstr ""
 
-#: packages/mainmenu-extension/src/index.ts:482 packages/notebook-extension/src/index.ts:3081 packages/notebook-extension/src/index.ts:3087 packages/notebook-extension/src/index.ts:3106
+#: packages/mainmenu-extension/src/index.ts:480 packages/mainmenu-extension/src/index.ts:482 packages/notebook-extension/src/index.ts:3158 packages/notebook-extension/src/index.ts:3165 packages/notebook-extension/src/index.ts:3188
 msgid "Reconnect to Kernel"
 msgstr ""
 
 #: packages/mainmenu-extension/src/index.ts:507
 msgid "Restart Kernel and Clear…"
 msgstr "Repornește Kernel-ul și Șterge…"
 
-#: packages/mainmenu-extension/src/index.ts:532
+#: packages/mainmenu-extension/src/index.ts:530 packages/mainmenu-extension/src/index.ts:532
 msgid "Shut down kernel"
 msgstr ""
 
-#: packages/mainmenu-extension/src/index.ts:539
+#: packages/mainmenu-extension/src/index.ts:536 packages/mainmenu-extension/src/index.ts:539
 msgid "Shut Down All Kernels…"
 msgstr "Oprește Toate Kernel-urile…"
 
-#: packages/mainmenu-extension/src/index.ts:545
+#: packages/mainmenu-extension/src/index.ts:542 packages/mainmenu-extension/src/index.ts:545
 msgid "Shut Down All?"
 msgstr "Opriți Tot?"
 
-#: packages/mainmenu-extension/src/index.ts:546
+#: packages/mainmenu-extension/src/index.ts:543 packages/mainmenu-extension/src/index.ts:546
 msgid "Shut down all kernels?"
 msgstr "Opriți toate kernel-urile?"
 
-#: packages/mainmenu-extension/src/index.ts:622 packages/mainmenu-extension/src/index.ts:623
+#: packages/mainmenu-extension/src/index.ts:617 packages/mainmenu-extension/src/index.ts:618 packages/mainmenu-extension/src/index.ts:622 packages/mainmenu-extension/src/index.ts:623
 msgid "Run Selected"
 msgstr "Execută Selecţia"
 
-#: packages/mainmenu-extension/src/index.ts:636 packages/mainmenu-extension/src/index.ts:637
+#: packages/mainmenu-extension/src/index.ts:632 packages/mainmenu-extension/src/index.ts:633 packages/mainmenu-extension/src/index.ts:636 packages/mainmenu-extension/src/index.ts:637
 msgid "Run All"
 msgstr "Execută Tot"
 
-#: packages/mainmenu-extension/src/index.ts:648 packages/mainmenu-extension/src/index.ts:649
+#: packages/mainmenu-extension/src/index.ts:644 packages/mainmenu-extension/src/index.ts:645 packages/mainmenu-extension/src/index.ts:648 packages/mainmenu-extension/src/index.ts:649
 msgid "Restart Kernel and Run All"
 msgstr "Repornește Kernel-ul și Execută Tot"
 
-#: packages/mainmenu-extension/src/index.ts:677
+#: packages/mainmenu-extension/src/index.ts:674 packages/mainmenu-extension/src/index.ts:677
 msgid "Activate a widget by its `id`."
 msgstr ""
 
-#: packages/mainmenu-extension/src/index.ts:694
+#: packages/mainmenu-extension/src/index.ts:691 packages/mainmenu-extension/src/index.ts:694
 msgid "Activate Previously Used Tab"
 msgstr "Activează Tabul Folosit Anterior"
 
-#: packages/mainmenu-extension/src/index.ts:771
+#: packages/mainmenu-extension/src/index.ts:768 packages/mainmenu-extension/src/index.ts:771
 msgid "Menu customization has changed. You will need to reload JupyterLab to see the changes."
 msgstr ""
 
-#: packages/markdownviewer-extension/src/index.ts:117 packages/markdownviewer-extension/src/index.ts:143
+#: packages/mainmenu-extension/src/recents.ts:155
+msgid "Could Not Open Recent"
+msgstr ""
+
+#: packages/mainmenu-extension/src/recents.ts:156
+msgid "%1 is no longer valid and will be removed from the list"
+msgstr ""
+
+#: packages/mainmenu-extension/src/recents.ts:189
+msgid "Open a Recent Document (given by `recent` argument)"
+msgstr ""
+
+#: packages/mainmenu-extension/src/recents.ts:217
+msgid "Reopen %1"
+msgstr ""
+
+#: packages/mainmenu-extension/src/recents.ts:218
+msgid "Reopen Closed Document"
+msgstr ""
+
+#: packages/mainmenu-extension/src/recents.ts:223
+msgid "Reopen recently closed file or notebook."
+msgstr ""
+
+#: packages/mainmenu-extension/src/recents.ts:232
+msgid "Open Recent"
+msgstr ""
+
+#: packages/markdownviewer-extension/src/index.ts:124 packages/markdownviewer-extension/src/index.ts:150
 msgid "Markdown Preview"
 msgstr "Previzualizare Markdown"
 
-#: packages/markdownviewer-extension/src/index.ts:178
+#: packages/markdownviewer-extension/src/index.ts:185
 msgid "Show Markdown Editor"
 msgstr "Arată Editorul Markdown"
 
+#: packages/mermaid-extension/src/index.ts:81
+msgid "Mermaid Copy Diagram Source"
+msgstr ""
+
 #: packages/metadataform/src/metadataform.ts:54
 msgid "No metadata."
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:1113 packages/notebook-extension/src/index.ts:1116 packages/notebook-extension/src/index.ts:1135
+#: packages/notebook-extension/src/index.ts:1146 packages/notebook-extension/src/index.ts:1150 packages/notebook-extension/src/index.ts:1158
 msgid "Notebook Tools"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:1265 packages/notebook-extension/src/index.ts:1268 packages/notebook-extension/src/index.ts:1287
+#: packages/notebook-extension/src/index.ts:1298 packages/notebook-extension/src/index.ts:1302 packages/notebook-extension/src/index.ts:1310
 msgid "Create New View for Cell Output"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:1335 packages/notebook-extension/src/index.ts:1338 packages/notebook-extension/src/index.ts:1357
+#: packages/notebook-extension/src/index.ts:1368 packages/notebook-extension/src/index.ts:1372 packages/notebook-extension/src/index.ts:1380
 msgid "New Console for Notebook"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:1353 packages/notebook-extension/src/index.ts:1356 packages/notebook-extension/src/index.ts:1375
+#: packages/notebook-extension/src/index.ts:1386 packages/notebook-extension/src/index.ts:1390 packages/notebook-extension/src/index.ts:1398
 msgid "Run Selected Text or Current Line in Console"
 msgstr "Execută Textul Selectat sau Linia Curentă în Consolă"
 
-#: packages/notebook-extension/src/index.ts:1517 packages/notebook-extension/src/index.ts:1520 packages/notebook-extension/src/index.ts:1539
+#: packages/notebook-extension/src/index.ts:1550 packages/notebook-extension/src/index.ts:1554 packages/notebook-extension/src/index.ts:1562
 msgid "Copy Output to Clipboard"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:1673 packages/notebook-extension/src/index.ts:1676 packages/notebook-extension/src/index.ts:1695
+#: packages/notebook-extension/src/index.ts:1707 packages/notebook-extension/src/index.ts:1712 packages/notebook-extension/src/index.ts:1723
 msgid "Auto Close Brackets for All Notebook Cell Types"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:1682 packages/notebook-extension/src/index.ts:1685 packages/notebook-extension/src/index.ts:1704
+#: packages/notebook-extension/src/index.ts:1716 packages/notebook-extension/src/index.ts:1721 packages/notebook-extension/src/index.ts:1732
 msgid "Set side-by-side ratio"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:1685 packages/notebook-extension/src/index.ts:1688 packages/notebook-extension/src/index.ts:1707
+#: packages/notebook-extension/src/index.ts:1719 packages/notebook-extension/src/index.ts:1724 packages/notebook-extension/src/index.ts:1735
 msgid "Width of the output in side-by-side mode"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:1900 packages/notebook-extension/src/index.ts:1903 packages/notebook-extension/src/index.ts:1922
+#: packages/notebook-extension/src/index.ts:1953 packages/notebook-extension/src/index.ts:1958 packages/notebook-extension/src/index.ts:1969
 msgid "New Notebook"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:1904 packages/notebook-extension/src/index.ts:1907 packages/notebook-extension/src/index.ts:1926
+#: packages/notebook-extension/src/index.ts:1957 packages/notebook-extension/src/index.ts:1962 packages/notebook-extension/src/index.ts:1973
 msgid "Create a new notebook"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2158 packages/notebook-extension/src/index.ts:2161 packages/notebook-extension/src/index.ts:2180
+#: packages/notebook-extension/src/index.ts:2213 packages/notebook-extension/src/index.ts:2220 packages/notebook-extension/src/index.ts:2231
 msgid "Run Selected Cell"
 msgid_plural "Run Selected Cells"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 
-#: packages/notebook-extension/src/index.ts:2166 packages/notebook-extension/src/index.ts:2169 packages/notebook-extension/src/index.ts:2188
+#: packages/notebook-extension/src/index.ts:2221 packages/notebook-extension/src/index.ts:2228 packages/notebook-extension/src/index.ts:2239
 msgid "Run this cell and advance"
 msgid_plural "Run these %1 cells and advance"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 
-#: packages/notebook-extension/src/index.ts:2191 packages/notebook-extension/src/index.ts:2195 packages/notebook-extension/src/index.ts:2214
+#: packages/notebook-extension/src/index.ts:2247 packages/notebook-extension/src/index.ts:2254 packages/notebook-extension/src/index.ts:2265
 msgid "Run Selected Cell and Do not Advance"
 msgid_plural "Run Selected Cells and Do not Advance"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 
-#: packages/notebook-extension/src/index.ts:2216 packages/notebook-extension/src/index.ts:2220 packages/notebook-extension/src/index.ts:2239
+#: packages/notebook-extension/src/index.ts:2272 packages/notebook-extension/src/index.ts:2279 packages/notebook-extension/src/index.ts:2290
 msgid "Run Selected Cell and Insert Below"
 msgid_plural "Run Selected Cells and Insert Below"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 
-#: packages/notebook-extension/src/index.ts:2239 packages/notebook-extension/src/index.ts:2243 packages/notebook-extension/src/index.ts:2262
+#: packages/notebook-extension/src/index.ts:2295 packages/notebook-extension/src/index.ts:2302 packages/notebook-extension/src/index.ts:2313
 msgid "Run All Cells"
 msgstr "Execută Toate Celulele"
 
-#: packages/notebook-extension/src/index.ts:2240 packages/notebook-extension/src/index.ts:2244 packages/notebook-extension/src/index.ts:2263
+#: packages/notebook-extension/src/index.ts:2296 packages/notebook-extension/src/index.ts:2303 packages/notebook-extension/src/index.ts:2314
 msgid "Run all cells"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2258 packages/notebook-extension/src/index.ts:2262 packages/notebook-extension/src/index.ts:2281
+#: packages/notebook-extension/src/index.ts:2314 packages/notebook-extension/src/index.ts:2321 packages/notebook-extension/src/index.ts:2332
 msgid "Run All Above Selected Cell"
 msgstr "Execută Celulele Selectate şi Toate de Mai Sus"
 
-#: packages/notebook-extension/src/index.ts:2283 packages/notebook-extension/src/index.ts:2287 packages/notebook-extension/src/index.ts:2306
+#: packages/notebook-extension/src/index.ts:2339 packages/notebook-extension/src/index.ts:2346 packages/notebook-extension/src/index.ts:2357
 msgid "Run Selected Cell and All Below"
 msgstr "Execută Celulele Selectate şi Toate de Mai Jos"
 
-#: packages/notebook-extension/src/index.ts:2309 packages/notebook-extension/src/index.ts:2313 packages/notebook-extension/src/index.ts:2332
+#: packages/notebook-extension/src/index.ts:2365 packages/notebook-extension/src/index.ts:2372 packages/notebook-extension/src/index.ts:2383
 msgid "Render All Markdown Cells"
 msgstr "Randează Toate Celulele Markdown"
 
-#: packages/notebook-extension/src/index.ts:2345 packages/notebook-extension/src/index.ts:2350 packages/notebook-extension/src/index.ts:2369
+#: packages/notebook-extension/src/index.ts:2402 packages/notebook-extension/src/index.ts:2409
 msgid "Close and Shut Down Notebook"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2356 packages/notebook-extension/src/index.ts:2361 packages/notebook-extension/src/index.ts:2380
+#: packages/notebook-extension/src/index.ts:2413 packages/notebook-extension/src/index.ts:2420 packages/notebook-extension/src/index.ts:2431
 msgid "Shut down the notebook?"
 msgstr "Opriți notebookul?"
 
-#: packages/notebook-extension/src/index.ts:2372 packages/notebook-extension/src/index.ts:2377 packages/notebook-extension/src/index.ts:2396
+#: packages/notebook-extension/src/index.ts:2420
+msgid "Close and Shut Down Notebook…"
+msgstr ""
+
+#: packages/notebook-extension/src/index.ts:2429 packages/notebook-extension/src/index.ts:2436 packages/notebook-extension/src/index.ts:2447
 msgid "Trust Notebook"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2383 packages/notebook-extension/src/index.ts:2388 packages/notebook-extension/src/index.ts:2407
+#: packages/notebook-extension/src/index.ts:2440 packages/notebook-extension/src/index.ts:2447 packages/notebook-extension/src/index.ts:2458
 msgid "Restart Kernel and Clear Outputs of All Cells…"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2384 packages/notebook-extension/src/index.ts:2389 packages/notebook-extension/src/index.ts:2408
+#: packages/notebook-extension/src/index.ts:2441 packages/notebook-extension/src/index.ts:2448 packages/notebook-extension/src/index.ts:2459
 msgid "Restart the kernel and clear all outputs of all cells"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2396 packages/notebook-extension/src/index.ts:2401 packages/notebook-extension/src/index.ts:2420
+#: packages/notebook-extension/src/index.ts:2453 packages/notebook-extension/src/index.ts:2460 packages/notebook-extension/src/index.ts:2471
 msgid "Restart Kernel and Run up to Selected Cell…"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2414 packages/notebook-extension/src/index.ts:2419 packages/notebook-extension/src/index.ts:2438
+#: packages/notebook-extension/src/index.ts:2477 packages/notebook-extension/src/index.ts:2484 packages/notebook-extension/src/index.ts:2495
 msgid "Restart Kernel and Run All Cells…"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2415 packages/notebook-extension/src/index.ts:2420 packages/notebook-extension/src/index.ts:2439
+#: packages/notebook-extension/src/index.ts:2478 packages/notebook-extension/src/index.ts:2485 packages/notebook-extension/src/index.ts:2496
 msgid "Restart the kernel and run all cells"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2428 packages/notebook-extension/src/index.ts:2433 packages/notebook-extension/src/index.ts:2452
+#: packages/notebook-extension/src/index.ts:2504 packages/notebook-extension/src/index.ts:2511 packages/notebook-extension/src/index.ts:2522
 msgid "Clear Outputs of All Cells"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2429 packages/notebook-extension/src/index.ts:2434 packages/notebook-extension/src/index.ts:2453
+#: packages/notebook-extension/src/index.ts:2505 packages/notebook-extension/src/index.ts:2512 packages/notebook-extension/src/index.ts:2523
 msgid "Clear all outputs of all cells"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2440 packages/notebook-extension/src/index.ts:2445 packages/notebook-extension/src/index.ts:2464
+#: packages/notebook-extension/src/index.ts:2516 packages/notebook-extension/src/index.ts:2523 packages/notebook-extension/src/index.ts:2534
 msgid "Clear Cell Output"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2441 packages/notebook-extension/src/index.ts:2446 packages/notebook-extension/src/index.ts:2465
+#: packages/notebook-extension/src/index.ts:2517 packages/notebook-extension/src/index.ts:2524 packages/notebook-extension/src/index.ts:2535
 msgid "Clear outputs for the selected cells"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2470 packages/notebook-extension/src/index.ts:2476 packages/notebook-extension/src/index.ts:2495
+#: packages/notebook-extension/src/index.ts:2547 packages/notebook-extension/src/index.ts:2554 packages/notebook-extension/src/index.ts:2565
 msgid "Change to Code Cell Type"
 msgstr "Schimbă în Celulă de Tip Cod"
 
-#: packages/notebook-extension/src/index.ts:2481 packages/notebook-extension/src/index.ts:2487 packages/notebook-extension/src/index.ts:2506
+#: packages/notebook-extension/src/index.ts:2558 packages/notebook-extension/src/index.ts:2565 packages/notebook-extension/src/index.ts:2580
 msgid "Change to Markdown Cell Type"
 msgstr "Schimbă în Celulă de Tip Markdown"
 
-#: packages/notebook-extension/src/index.ts:2492 packages/notebook-extension/src/index.ts:2498 packages/notebook-extension/src/index.ts:2517
+#: packages/notebook-extension/src/index.ts:2569 packages/notebook-extension/src/index.ts:2576 packages/notebook-extension/src/index.ts:2595
 msgid "Change to Raw Cell Type"
 msgstr "Schimbă în Celulă de Tip Raw"
 
-#: packages/notebook-extension/src/index.ts:2505 packages/notebook-extension/src/index.ts:2511 packages/notebook-extension/src/index.ts:2530
+#: packages/notebook-extension/src/index.ts:2582 packages/notebook-extension/src/index.ts:2589 packages/notebook-extension/src/index.ts:2612
 msgid "Cut Cell"
 msgid_plural "Cut Cells"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 
-#: packages/notebook-extension/src/index.ts:2513 packages/notebook-extension/src/index.ts:2519 packages/notebook-extension/src/index.ts:2538
+#: packages/notebook-extension/src/index.ts:2590 packages/notebook-extension/src/index.ts:2597 packages/notebook-extension/src/index.ts:2620
 msgid "Cut this cell"
 msgid_plural "Cut these %1 cells"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 
-#: packages/notebook-extension/src/index.ts:2532 packages/notebook-extension/src/index.ts:2538 packages/notebook-extension/src/index.ts:2557
+#: packages/notebook-extension/src/index.ts:2609 packages/notebook-extension/src/index.ts:2616 packages/notebook-extension/src/index.ts:2639
 msgid "Copy Cell"
 msgid_plural "Copy Cells"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 
-#: packages/notebook-extension/src/index.ts:2540 packages/notebook-extension/src/index.ts:2546 packages/notebook-extension/src/index.ts:2565
+#: packages/notebook-extension/src/index.ts:2617 packages/notebook-extension/src/index.ts:2624 packages/notebook-extension/src/index.ts:2647
 msgid "Copy this cell"
 msgid_plural "Copy these %1 cells"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 
-#: packages/notebook-extension/src/index.ts:2559 packages/notebook-extension/src/index.ts:2565 packages/notebook-extension/src/index.ts:2584
+#: packages/notebook-extension/src/index.ts:2636 packages/notebook-extension/src/index.ts:2643 packages/notebook-extension/src/index.ts:2666
 msgid "Paste Cell Below"
 msgid_plural "Paste Cells Below"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 
-#: packages/notebook-extension/src/index.ts:2567 packages/notebook-extension/src/index.ts:2573 packages/notebook-extension/src/index.ts:2592 packages/notebook-extension/src/index.ts:2594 packages/notebook-extension/src/index.ts:2600 packages/notebook-extension/src/index.ts:2619
+#: packages/notebook-extension/src/index.ts:2644 packages/notebook-extension/src/index.ts:2651 packages/notebook-extension/src/index.ts:2671 packages/notebook-extension/src/index.ts:2674 packages/notebook-extension/src/index.ts:2678 packages/notebook-extension/src/index.ts:2701
 msgid "Paste this cell from the clipboard"
 msgid_plural "Paste these %1 cells from the clipboard"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 
-#: packages/notebook-extension/src/index.ts:2586 packages/notebook-extension/src/index.ts:2592 packages/notebook-extension/src/index.ts:2611
+#: packages/notebook-extension/src/index.ts:2663 packages/notebook-extension/src/index.ts:2670 packages/notebook-extension/src/index.ts:2693
 msgid "Paste Cell Above"
 msgid_plural "Paste Cells Above"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 
-#: packages/notebook-extension/src/index.ts:2612 packages/notebook-extension/src/index.ts:2618 packages/notebook-extension/src/index.ts:2637
+#: packages/notebook-extension/src/index.ts:2689 packages/notebook-extension/src/index.ts:2696 packages/notebook-extension/src/index.ts:2719
 msgid "Duplicate Cell Below"
 msgid_plural "Duplicate Cells Below"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 
-#: packages/notebook-extension/src/index.ts:2620 packages/notebook-extension/src/index.ts:2626 packages/notebook-extension/src/index.ts:2645
+#: packages/notebook-extension/src/index.ts:2697 packages/notebook-extension/src/index.ts:2704 packages/notebook-extension/src/index.ts:2727
 msgid "Create a duplicate of this cell below"
 msgid_plural "Create duplicates of %1 cells below"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 
-#: packages/notebook-extension/src/index.ts:2639 packages/notebook-extension/src/index.ts:2645 packages/notebook-extension/src/index.ts:2664
+#: packages/notebook-extension/src/index.ts:2716 packages/notebook-extension/src/index.ts:2723 packages/notebook-extension/src/index.ts:2746
 msgid "Paste Cell and Replace"
 msgid_plural "Paste Cells and Replace"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 
-#: packages/notebook-extension/src/index.ts:2657 packages/notebook-extension/src/index.ts:2663 packages/notebook-extension/src/index.ts:2682
+#: packages/notebook-extension/src/index.ts:2734 packages/notebook-extension/src/index.ts:2741 packages/notebook-extension/src/index.ts:2764
 msgid "Delete Cell"
 msgid_plural "Delete Cells"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 
-#: packages/notebook-extension/src/index.ts:2665 packages/notebook-extension/src/index.ts:2671 packages/notebook-extension/src/index.ts:2690
+#: packages/notebook-extension/src/index.ts:2742 packages/notebook-extension/src/index.ts:2749 packages/notebook-extension/src/index.ts:2772
 msgid "Delete this cell"
 msgid_plural "Delete these %1 cells"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 
-#: packages/notebook-extension/src/index.ts:2682 packages/notebook-extension/src/index.ts:2688 packages/notebook-extension/src/index.ts:2707
+#: packages/notebook-extension/src/index.ts:2759 packages/notebook-extension/src/index.ts:2766 packages/notebook-extension/src/index.ts:2789
 msgid "Split Cell"
 msgstr "Împarte Celula"
 
-#: packages/notebook-extension/src/index.ts:2693 packages/notebook-extension/src/index.ts:2699 packages/notebook-extension/src/index.ts:2718
+#: packages/notebook-extension/src/index.ts:2770 packages/notebook-extension/src/index.ts:2777 packages/notebook-extension/src/index.ts:2800
 msgid "Merge Selected Cells"
 msgstr "Îmbină Celulele Selectate"
 
-#: packages/notebook-extension/src/index.ts:2704 packages/notebook-extension/src/index.ts:2710 packages/notebook-extension/src/index.ts:2729
+#: packages/notebook-extension/src/index.ts:2781 packages/notebook-extension/src/index.ts:2788 packages/notebook-extension/src/index.ts:2811
 msgid "Merge Cell Above"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2715 packages/notebook-extension/src/index.ts:2721 packages/notebook-extension/src/index.ts:2740
+#: packages/notebook-extension/src/index.ts:2792 packages/notebook-extension/src/index.ts:2799 packages/notebook-extension/src/index.ts:2822
 msgid "Merge Cell Below"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2726 packages/notebook-extension/src/index.ts:2732 packages/notebook-extension/src/index.ts:2751
+#: packages/notebook-extension/src/index.ts:2803 packages/notebook-extension/src/index.ts:2810 packages/notebook-extension/src/index.ts:2833
 msgid "Insert Cell Above"
 msgstr "Inserează Celulă Deasupra"
 
-#: packages/notebook-extension/src/index.ts:2727 packages/notebook-extension/src/index.ts:2733 packages/notebook-extension/src/index.ts:2752
+#: packages/notebook-extension/src/index.ts:2804 packages/notebook-extension/src/index.ts:2811 packages/notebook-extension/src/index.ts:2834
 msgid "Insert a cell above"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2739 packages/notebook-extension/src/index.ts:2745 packages/notebook-extension/src/index.ts:2764
+#: packages/notebook-extension/src/index.ts:2816 packages/notebook-extension/src/index.ts:2823 packages/notebook-extension/src/index.ts:2846
 msgid "Insert Cell Below"
 msgstr "Inserează Celulă Dedesubt"
 
-#: packages/notebook-extension/src/index.ts:2740 packages/notebook-extension/src/index.ts:2746 packages/notebook-extension/src/index.ts:2765 packages/notebook/src/default-toolbar.tsx:121
+#: packages/notebook-extension/src/index.ts:2817 packages/notebook-extension/src/index.ts:2824 packages/notebook-extension/src/index.ts:2847 packages/notebook/src/default-toolbar.tsx:121
 msgid "Insert a cell below"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2752 packages/notebook-extension/src/index.ts:2758 packages/notebook-extension/src/index.ts:2777
+#: packages/notebook-extension/src/index.ts:2829 packages/notebook-extension/src/index.ts:2836 packages/notebook-extension/src/index.ts:2859
 msgid "Select Cell Above"
 msgstr "Selectează Celula de Deasupra"
 
-#: packages/notebook-extension/src/index.ts:2763 packages/notebook-extension/src/index.ts:2769 packages/notebook-extension/src/index.ts:2788
+#: packages/notebook-extension/src/index.ts:2840 packages/notebook-extension/src/index.ts:2847 packages/notebook-extension/src/index.ts:2870
 msgid "Select Cell Below"
 msgstr "Selectează Celula de Dedesubt"
 
-#: packages/notebook-extension/src/index.ts:2773 packages/notebook-extension/src/index.ts:2779 packages/notebook-extension/src/index.ts:2798
+#: packages/notebook-extension/src/index.ts:2850 packages/notebook-extension/src/index.ts:2857 packages/notebook-extension/src/index.ts:2880
 msgid "Insert Heading Above Current Heading"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2784 packages/notebook-extension/src/index.ts:2790 packages/notebook-extension/src/index.ts:2809
+#: packages/notebook-extension/src/index.ts:2861 packages/notebook-extension/src/index.ts:2868 packages/notebook-extension/src/index.ts:2891
 msgid "Insert Heading Below Current Heading"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2795 packages/notebook-extension/src/index.ts:2801 packages/notebook-extension/src/index.ts:2820
+#: packages/notebook-extension/src/index.ts:2872 packages/notebook-extension/src/index.ts:2879 packages/notebook-extension/src/index.ts:2902
 msgid "Select Heading Above or Collapse Heading"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2808 packages/notebook-extension/src/index.ts:2814 packages/notebook-extension/src/index.ts:2833
+#: packages/notebook-extension/src/index.ts:2885 packages/notebook-extension/src/index.ts:2892 packages/notebook-extension/src/index.ts:2915
 msgid "Select Heading Below or Expand Heading"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2821 packages/notebook-extension/src/index.ts:2827 packages/notebook-extension/src/index.ts:2846
+#: packages/notebook-extension/src/index.ts:2898 packages/notebook-extension/src/index.ts:2905 packages/notebook-extension/src/index.ts:2928
 msgid "Extend Selection Above"
 msgstr "Extinde Selecția Deasupra"
 
-#: packages/notebook-extension/src/index.ts:2832 packages/notebook-extension/src/index.ts:2838 packages/notebook-extension/src/index.ts:2857
+#: packages/notebook-extension/src/index.ts:2909 packages/notebook-extension/src/index.ts:2916 packages/notebook-extension/src/index.ts:2939
 msgid "Extend Selection to Top"
 msgstr "Extinde Selecția până Sus"
 
-#: packages/notebook-extension/src/index.ts:2843 packages/notebook-extension/src/index.ts:2849 packages/notebook-extension/src/index.ts:2868
+#: packages/notebook-extension/src/index.ts:2920 packages/notebook-extension/src/index.ts:2927 packages/notebook-extension/src/index.ts:2950
 msgid "Extend Selection Below"
 msgstr "Extinde Selecția Dedesubt"
 
-#: packages/notebook-extension/src/index.ts:2854 packages/notebook-extension/src/index.ts:2860 packages/notebook-extension/src/index.ts:2879
+#: packages/notebook-extension/src/index.ts:2931 packages/notebook-extension/src/index.ts:2938 packages/notebook-extension/src/index.ts:2961
 msgid "Extend Selection to Bottom"
 msgstr "Extinde Selecția până Jos"
 
-#: packages/notebook-extension/src/index.ts:2865 packages/notebook-extension/src/index.ts:2871 packages/notebook-extension/src/index.ts:2890
+#: packages/notebook-extension/src/index.ts:2942 packages/notebook-extension/src/index.ts:2949 packages/notebook-extension/src/index.ts:2972
 msgid "Select All Cells"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2876 packages/notebook-extension/src/index.ts:2882 packages/notebook-extension/src/index.ts:2901
+#: packages/notebook-extension/src/index.ts:2953 packages/notebook-extension/src/index.ts:2960 packages/notebook-extension/src/index.ts:2983
 msgid "Deselect All Cells"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2889 packages/notebook-extension/src/index.ts:2895 packages/notebook-extension/src/index.ts:2914
+#: packages/notebook-extension/src/index.ts:2966 packages/notebook-extension/src/index.ts:2973 packages/notebook-extension/src/index.ts:2996
 msgid "Move Cell Up"
 msgid_plural "Move Cells Up"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 
-#: packages/notebook-extension/src/index.ts:2897 packages/notebook-extension/src/index.ts:2903 packages/notebook-extension/src/index.ts:2922
+#: packages/notebook-extension/src/index.ts:2974 packages/notebook-extension/src/index.ts:2981 packages/notebook-extension/src/index.ts:3004
 msgid "Move this cell up"
 msgid_plural "Move these %1 cells up"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 
-#: packages/notebook-extension/src/index.ts:2909 packages/notebook-extension/src/index.ts:2915 packages/notebook-extension/src/index.ts:2934
+#: packages/notebook-extension/src/index.ts:2986 packages/notebook-extension/src/index.ts:2993 packages/notebook-extension/src/index.ts:3016
 msgid "Notebook cell shifted up successfully"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2926 packages/notebook-extension/src/index.ts:2932 packages/notebook-extension/src/index.ts:2951
+#: packages/notebook-extension/src/index.ts:3003 packages/notebook-extension/src/index.ts:3010 packages/notebook-extension/src/index.ts:3033
 msgid "Move Cell Down"
 msgid_plural "Move Cells Down"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 
-#: packages/notebook-extension/src/index.ts:2934 packages/notebook-extension/src/index.ts:2940 packages/notebook-extension/src/index.ts:2959
+#: packages/notebook-extension/src/index.ts:3011 packages/notebook-extension/src/index.ts:3018 packages/notebook-extension/src/index.ts:3041
 msgid "Move this cell down"
 msgid_plural "Move these %1 cells down"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 
-#: packages/notebook-extension/src/index.ts:2946 packages/notebook-extension/src/index.ts:2952 packages/notebook-extension/src/index.ts:2971
+#: packages/notebook-extension/src/index.ts:3023 packages/notebook-extension/src/index.ts:3030 packages/notebook-extension/src/index.ts:3053
 msgid "Notebook cell shifted down successfully"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:2987 packages/notebook-extension/src/index.ts:2993 packages/notebook-extension/src/index.ts:3012
+#: packages/notebook-extension/src/index.ts:3064 packages/notebook-extension/src/index.ts:3071 packages/notebook-extension/src/index.ts:3094
 msgid "Enter Command Mode"
 msgstr "Intră în modul comandă"
 
-#: packages/notebook-extension/src/index.ts:2998 packages/notebook-extension/src/index.ts:3004 packages/notebook-extension/src/index.ts:3023
+#: packages/notebook-extension/src/index.ts:3075 packages/notebook-extension/src/index.ts:3082 packages/notebook-extension/src/index.ts:3105
 msgid "Enter Edit Mode"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:3009 packages/notebook-extension/src/index.ts:3015 packages/notebook-extension/src/index.ts:3034
+#: packages/notebook-extension/src/index.ts:3086 packages/notebook-extension/src/index.ts:3093 packages/notebook-extension/src/index.ts:3116
 msgid "Undo Cell Operation"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:3020 packages/notebook-extension/src/index.ts:3026 packages/notebook-extension/src/index.ts:3045
+#: packages/notebook-extension/src/index.ts:3097 packages/notebook-extension/src/index.ts:3104 packages/notebook-extension/src/index.ts:3127
 msgid "Redo Cell Operation"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:3098 packages/notebook-extension/src/index.ts:3104 packages/notebook-extension/src/index.ts:3123
+#: packages/notebook-extension/src/index.ts:3175 packages/notebook-extension/src/index.ts:3182 packages/notebook-extension/src/index.ts:3205
 msgid "Change to Heading 1"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:3109 packages/notebook-extension/src/index.ts:3115 packages/notebook-extension/src/index.ts:3134
+#: packages/notebook-extension/src/index.ts:3186 packages/notebook-extension/src/index.ts:3193 packages/notebook-extension/src/index.ts:3220
 msgid "Change to Heading 2"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:3120 packages/notebook-extension/src/index.ts:3126 packages/notebook-extension/src/index.ts:3145
+#: packages/notebook-extension/src/index.ts:3197 packages/notebook-extension/src/index.ts:3204 packages/notebook-extension/src/index.ts:3235
 msgid "Change to Heading 3"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:3131 packages/notebook-extension/src/index.ts:3137 packages/notebook-extension/src/index.ts:3156
+#: packages/notebook-extension/src/index.ts:3208 packages/notebook-extension/src/index.ts:3215 packages/notebook-extension/src/index.ts:3250
 msgid "Change to Heading 4"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:3142 packages/notebook-extension/src/index.ts:3148 packages/notebook-extension/src/index.ts:3167
+#: packages/notebook-extension/src/index.ts:3219 packages/notebook-extension/src/index.ts:3226 packages/notebook-extension/src/index.ts:3265
 msgid "Change to Heading 5"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:3153 packages/notebook-extension/src/index.ts:3159 packages/notebook-extension/src/index.ts:3178
+#: packages/notebook-extension/src/index.ts:3230 packages/notebook-extension/src/index.ts:3237 packages/notebook-extension/src/index.ts:3280
 msgid "Change to Heading 6"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:3164 packages/notebook-extension/src/index.ts:3170 packages/notebook-extension/src/index.ts:3189
+#: packages/notebook-extension/src/index.ts:3241 packages/notebook-extension/src/index.ts:3248 packages/notebook-extension/src/index.ts:3295
 msgid "Collapse Selected Code"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:3175 packages/notebook-extension/src/index.ts:3181 packages/notebook-extension/src/index.ts:3200
+#: packages/notebook-extension/src/index.ts:3252 packages/notebook-extension/src/index.ts:3259 packages/notebook-extension/src/index.ts:3306
 msgid "Expand Selected Code"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:3186 packages/notebook-extension/src/index.ts:3192 packages/notebook-extension/src/index.ts:3211
+#: packages/notebook-extension/src/index.ts:3263 packages/notebook-extension/src/index.ts:3270 packages/notebook-extension/src/index.ts:3317
 msgid "Collapse All Code"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:3197 packages/notebook-extension/src/index.ts:3203 packages/notebook-extension/src/index.ts:3222
+#: packages/notebook-extension/src/index.ts:3274 packages/notebook-extension/src/index.ts:3281 packages/notebook-extension/src/index.ts:3328
 msgid "Expand All Code"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:3208 packages/notebook-extension/src/index.ts:3214 packages/notebook-extension/src/index.ts:3233
+#: packages/notebook-extension/src/index.ts:3285 packages/notebook-extension/src/index.ts:3292 packages/notebook-extension/src/index.ts:3339
 msgid "Collapse Selected Outputs"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:3219 packages/notebook-extension/src/index.ts:3225 packages/notebook-extension/src/index.ts:3244
+#: packages/notebook-extension/src/index.ts:3296 packages/notebook-extension/src/index.ts:3303 packages/notebook-extension/src/index.ts:3350
 msgid "Expand Selected Outputs"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:3230 packages/notebook-extension/src/index.ts:3236 packages/notebook-extension/src/index.ts:3255
+#: packages/notebook-extension/src/index.ts:3307 packages/notebook-extension/src/index.ts:3314 packages/notebook-extension/src/index.ts:3361
 msgid "Collapse All Outputs"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:3242 packages/notebook-extension/src/index.ts:3248 packages/notebook-extension/src/index.ts:3267
+#: packages/notebook-extension/src/index.ts:3319 packages/notebook-extension/src/index.ts:3326 packages/notebook-extension/src/index.ts:3373
 msgid "Render Side-by-Side"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:3264 packages/notebook-extension/src/index.ts:3270 packages/notebook-extension/src/index.ts:3289
+#: packages/notebook-extension/src/index.ts:3341 packages/notebook-extension/src/index.ts:3348 packages/notebook-extension/src/index.ts:3395
 msgid "Expand All Outputs"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:3275 packages/notebook-extension/src/index.ts:3281 packages/notebook-extension/src/index.ts:3300
+#: packages/notebook-extension/src/index.ts:3352 packages/notebook-extension/src/index.ts:3359 packages/notebook-extension/src/index.ts:3406
 msgid "Enable Scrolling for Outputs"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:3286 packages/notebook-extension/src/index.ts:3292 packages/notebook-extension/src/index.ts:3311
+#: packages/notebook-extension/src/index.ts:3363 packages/notebook-extension/src/index.ts:3370 packages/notebook-extension/src/index.ts:3417
 msgid "Disable Scrolling for Outputs"
 msgstr "Dezactivează derularea pentru rezultate"
 
-#: packages/notebook-extension/src/index.ts:3297 packages/notebook-extension/src/index.ts:3303 packages/notebook-extension/src/index.ts:3322
+#: packages/notebook-extension/src/index.ts:3374 packages/notebook-extension/src/index.ts:3381 packages/notebook-extension/src/index.ts:3428
 msgid "Select current running or last run cell"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:3308 packages/notebook-extension/src/index.ts:3314 packages/notebook-extension/src/index.ts:3333
+#: packages/notebook-extension/src/index.ts:3385 packages/notebook-extension/src/index.ts:3392 packages/notebook-extension/src/index.ts:3439
 msgid "Replace Selection in Notebook Cell"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:3320 packages/notebook-extension/src/index.ts:3326 packages/notebook-extension/src/index.ts:3345
+#: packages/notebook-extension/src/index.ts:3397 packages/notebook-extension/src/index.ts:3404 packages/notebook-extension/src/index.ts:3451
 msgid "Toggle Collapse Notebook Heading"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:3330 packages/notebook-extension/src/index.ts:3336 packages/notebook-extension/src/index.ts:3355 packages/toc-extension/src/index.ts:141
+#: packages/notebook-extension/src/index.ts:3407 packages/notebook-extension/src/index.ts:3414 packages/notebook-extension/src/index.ts:3461 packages/toc-extension/src/index.ts:141
 msgid "Collapse All Headings"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:3339 packages/notebook-extension/src/index.ts:3345 packages/notebook-extension/src/index.ts:3364 packages/toc-extension/src/index.ts:140
+#: packages/notebook-extension/src/index.ts:3416 packages/notebook-extension/src/index.ts:3423 packages/notebook-extension/src/index.ts:3470 packages/toc-extension/src/index.ts:140
 msgid "Expand All Headings"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:3349 packages/notebook-extension/src/index.ts:3355 packages/notebook-extension/src/index.ts:3374
+#: packages/notebook-extension/src/index.ts:3425 packages/notebook-extension/src/index.ts:3432 packages/notebook-extension/src/index.ts:3479
 msgid "Select and Run Cell(s) for this Heading"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:3399 packages/notebook-extension/src/index.ts:3405 packages/notebook-extension/src/index.ts:3424 packages/notebook-extension/src/index.ts:657 packages/notebook-extension/src/index.ts:660
+#: packages/notebook-extension/src/index.ts:3466 packages/notebook-extension/src/index.ts:3473 packages/notebook-extension/src/index.ts:3520
+msgid "Access Previous Kernel History Entry"
+msgstr ""
+
+#: packages/notebook-extension/src/index.ts:3475 packages/notebook-extension/src/index.ts:3482 packages/notebook-extension/src/index.ts:3529
+msgid "Access Next Kernel History Entry"
+msgstr ""
+
+#: packages/notebook-extension/src/index.ts:3484 packages/notebook-extension/src/index.ts:3491 packages/notebook-extension/src/index.ts:3539
+msgid "Virtual Scrollbar"
+msgstr ""
+
+#: packages/notebook-extension/src/index.ts:3485 packages/notebook-extension/src/index.ts:3492 packages/notebook-extension/src/index.ts:3540
+msgid "Toggle virtual scrollbar (enabled with windowing mode: full)"
+msgstr ""
+
+#: packages/notebook-extension/src/index.ts:3519 packages/notebook-extension/src/index.ts:3526 packages/notebook-extension/src/index.ts:3585 packages/notebook-extension/src/index.ts:670 packages/notebook-extension/src/index.ts:674 packages/notebook-extension/src/index.ts:681
 msgid "Notebook Operations"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:3435 packages/notebook-extension/src/index.ts:3441 packages/notebook-extension/src/index.ts:3460
+#: packages/notebook-extension/src/index.ts:3557 packages/notebook-extension/src/index.ts:3564 packages/notebook-extension/src/index.ts:3623
 msgid "Notebook Cell Operations"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:3680 packages/notebook-extension/src/index.ts:3686 packages/notebook-extension/src/index.ts:3705
+#: packages/notebook-extension/src/index.ts:3802 packages/notebook-extension/src/index.ts:3809 packages/notebook-extension/src/index.ts:3868
 msgid "PDF"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:3681 packages/notebook-extension/src/index.ts:3687 packages/notebook-extension/src/index.ts:3706
+#: packages/notebook-extension/src/index.ts:3803 packages/notebook-extension/src/index.ts:3810 packages/notebook-extension/src/index.ts:3869
 msgid "ReStructured Text"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:3682 packages/notebook-extension/src/index.ts:3688 packages/notebook-extension/src/index.ts:3707
+#: packages/notebook-extension/src/index.ts:3804 packages/notebook-extension/src/index.ts:3811 packages/notebook-extension/src/index.ts:3870
 msgid "Executable Script"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:3683 packages/notebook-extension/src/index.ts:3689 packages/notebook-extension/src/index.ts:3708
+#: packages/notebook-extension/src/index.ts:3805 packages/notebook-extension/src/index.ts:3812 packages/notebook-extension/src/index.ts:3871
 msgid "Reveal.js Slides"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:3737 packages/notebook-extension/src/index.ts:3743 packages/notebook-extension/src/index.ts:3762
+#: packages/notebook-extension/src/index.ts:3859 packages/notebook-extension/src/index.ts:3866 packages/notebook-extension/src/index.ts:3925
 msgid "For Notebook: %1"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:3738 packages/notebook-extension/src/index.ts:3744 packages/notebook-extension/src/index.ts:3763
+#: packages/notebook-extension/src/index.ts:3860 packages/notebook-extension/src/index.ts:3867 packages/notebook-extension/src/index.ts:3926
 msgid "For Notebook:"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:569 packages/notebook-extension/src/index.ts:572
+#: packages/notebook-extension/src/index.ts:582 packages/notebook-extension/src/index.ts:586 packages/notebook-extension/src/index.ts:593
 msgid "Save and Export Notebook to the given `format`."
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:573 packages/notebook-extension/src/index.ts:576
+#: packages/notebook-extension/src/index.ts:586 packages/notebook-extension/src/index.ts:590 packages/notebook-extension/src/index.ts:597
 msgid "Save and Export Notebook: %1"
 msgstr ""
 
-#: packages/notebook/src/actions.tsx:2032 packages/notebook/src/actions.tsx:2039
+#: packages/notebook/src/actions.tsx:2094 packages/notebook/src/actions.tsx:2099 packages/notebook/src/actions.tsx:2107
 msgid "A trusted Jupyter notebook may execute hidden malicious code when you open it."
 msgstr ""
 
-#: packages/notebook/src/actions.tsx:2036 packages/notebook/src/actions.tsx:2043
+#: packages/notebook/src/actions.tsx:2098 packages/notebook/src/actions.tsx:2103 packages/notebook/src/actions.tsx:2111
 msgid "Selecting \"Trust\" will re-render this notebook in a trusted state."
 msgstr ""
 
-#: packages/notebook/src/actions.tsx:2040 packages/notebook/src/actions.tsx:2047
+#: packages/notebook/src/actions.tsx:2102 packages/notebook/src/actions.tsx:2107 packages/notebook/src/actions.tsx:2115
 msgid "For more information, see"
 msgstr ""
 
-#: packages/notebook/src/actions.tsx:2046 packages/notebook/src/actions.tsx:2053
+#: packages/notebook/src/actions.tsx:2108 packages/notebook/src/actions.tsx:2113 packages/notebook/src/actions.tsx:2121
 msgid "the Jupyter security documentation"
 msgstr ""
 
-#: packages/notebook/src/actions.tsx:2054 packages/notebook/src/actions.tsx:2061
+#: packages/notebook/src/actions.tsx:2116 packages/notebook/src/actions.tsx:2121 packages/notebook/src/actions.tsx:2129
 msgid "Notebook is already trusted"
 msgstr ""
 
-#: packages/notebook/src/actions.tsx:2061 packages/notebook/src/actions.tsx:2068
+#: packages/notebook/src/actions.tsx:2123 packages/notebook/src/actions.tsx:2128 packages/notebook/src/actions.tsx:2136
 msgid "Trust this notebook?"
 msgstr ""
 
-#: packages/notebook/src/actions.tsx:2064 packages/notebook/src/actions.tsx:2065 packages/notebook/src/actions.tsx:2072
+#: packages/notebook/src/actions.tsx:2127 packages/notebook/src/actions.tsx:2132 packages/notebook/src/actions.tsx:2140
 msgid "Trust"
 msgstr ""
 
-#: packages/notebook/src/actions.tsx:2066 packages/notebook/src/actions.tsx:2073
+#: packages/notebook/src/actions.tsx:2128 packages/notebook/src/actions.tsx:2133 packages/notebook/src/actions.tsx:2141
 msgid "Confirm Trusting this notebook"
 msgstr ""
 
-#: packages/notebook/src/actions.tsx:2279 packages/notebook/src/actions.tsx:2282 packages/notebook/src/actions.tsx:2285 packages/notebook/src/actions.tsx:2289
+#: packages/notebook/src/actions.tsx:2488 packages/notebook/src/actions.tsx:2493 packages/notebook/src/cellexecutor.ts:46
 msgid "Kernel Terminating"
 msgstr ""
 
-#: packages/notebook/src/actions.tsx:2280 packages/notebook/src/actions.tsx:2283 packages/notebook/src/actions.tsx:2286 packages/notebook/src/actions.tsx:2290
+#: packages/notebook/src/actions.tsx:2489 packages/notebook/src/actions.tsx:2494 packages/notebook/src/cellexecutor.ts:47
 msgid "The kernel for %1 appears to be terminating. You can not run any cell for now."
 msgstr ""
 
-#: packages/notebook/src/actions.tsx:2290 packages/notebook/src/actions.tsx:2293 packages/notebook/src/actions.tsx:2296 packages/notebook/src/actions.tsx:2300
+#: packages/notebook/src/actions.tsx:2499 packages/notebook/src/actions.tsx:2504 packages/notebook/src/cellexecutor.ts:57
 msgid "Cell not executed due to pending input"
 msgstr ""
 
-#: packages/notebook/src/actions.tsx:2291 packages/notebook/src/actions.tsx:2294 packages/notebook/src/actions.tsx:2297 packages/notebook/src/actions.tsx:2301
+#: packages/notebook/src/actions.tsx:2500 packages/notebook/src/actions.tsx:2505 packages/notebook/src/cellexecutor.ts:58
 msgid "The cell has not been executed to avoid kernel deadlock as there is another pending input! Submit your pending input and try again."
 msgstr ""
 
+#: packages/notebook/src/actions.tsx:2610
+msgid "Cell type not changed due to pending input"
+msgstr ""
+
+#: packages/notebook/src/actions.tsx:2611
+msgid "The cell type has not been changed to avoid kernel deadlock as this cell has pending input! Submit your pending input and try again."
+msgstr ""
+
 #: packages/notebook/src/default-toolbar.tsx:141
 msgid "Cut the selected cells"
 msgstr ""
 
 #: packages/notebook/src/default-toolbar.tsx:161
 msgid "Copy the selected cells"
 msgstr ""
@@ -6310,14 +6811,18 @@
 msgid "Kernel status"
 msgstr ""
 
 #: packages/notebook/src/executionindicator.tsx:75
 msgid "Kernel status: %1"
 msgstr ""
 
+#: packages/notebook/src/history.ts:349
+msgid "History was unable to be retrieved"
+msgstr ""
+
 #: packages/notebook/src/model.ts:354
 msgid "This notebook has been converted from an older notebook format (v%1)\n"
 "to the current notebook format (v%2).\n"
 "The next time you save this notebook, the current notebook format (v%2) will be used.\n"
 "'Older versions of Jupyter may not be able to read the new format.' To preserve the original format version,\n"
 "close the notebook without saving it."
 msgstr ""
@@ -6338,186 +6843,362 @@
 msgid "Notebook converted"
 msgstr "Notebook convertit"
 
 #: packages/notebook/src/modestatus.tsx:29
 msgid "Mode: %1"
 msgstr "Mod: %1"
 
-#: packages/notebook/src/modestatus.tsx:71 packages/shortcuts-extension/src/components/TopNav.tsx:181
+#: packages/notebook/src/modestatus.tsx:71 packages/shortcuts-extension/src/components/TopNav.tsx:130 packages/shortcuts-extension/src/components/TopNav.tsx:182
 msgid "Command"
 msgstr ""
 
 #: packages/notebook/src/modestatus.tsx:72 packages/shortcuts-extension/src/components/ShortcutItem.tsx:61
 msgid "Edit"
 msgstr ""
 
 #: packages/notebook/src/modestatus.tsx:83
 msgid "Notebook is in %1 mode"
 msgstr "Notebook-ul este în modul %1"
 
-#: packages/notebook/src/notebookfooter.ts:24 packages/notebook/src/notebookfooter.ts:30
+#: packages/notebook/src/notebookfooter.ts:25
 msgid "Click to add a cell."
 msgstr ""
 
-#: packages/notebook/src/panel.ts:229
+#: packages/notebook/src/panel.ts:223
 msgid "Kernel Restarting"
 msgstr ""
 
-#: packages/notebook/src/panel.ts:230
+#: packages/notebook/src/panel.ts:224
 msgid "The kernel for %1 appears to have died. It will restart automatically."
 msgstr "Kernel-ul pentru %1 pare să fi murit. Va reporni automat."
 
-#: packages/notebook/src/searchprovider.ts:226
+#: packages/notebook/src/searchprovider.ts:234 packages/notebook/src/searchprovider.ts:237
 msgid "Search Cell Outputs"
 msgstr ""
 
-#: packages/notebook/src/searchprovider.ts:227
+#: packages/notebook/src/searchprovider.ts:235 packages/notebook/src/searchprovider.ts:238
 msgid "Search in the cell outputs."
 msgstr ""
 
-#: packages/notebook/src/searchprovider.ts:234
+#: packages/notebook/src/searchprovider.ts:236
+msgid "Search in the cell outputs (not available when replace options are shown)."
+msgstr ""
+
+#: packages/notebook/src/searchprovider.ts:242 packages/notebook/src/searchprovider.ts:245
 msgid "Search in %1 Selected Cell"
 msgid_plural "Search in %1 Selected Cells"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 
-#: packages/notebook/src/searchprovider.ts:239
+#: packages/notebook/src/searchprovider.ts:247 packages/notebook/src/searchprovider.ts:250
 msgid "Search in %1 Selected Line"
 msgid_plural "Search in %1 Selected Lines"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 
-#: packages/notebook/src/searchprovider.ts:244
+#: packages/notebook/src/searchprovider.ts:252 packages/notebook/src/searchprovider.ts:255
 msgid "Search only in the selected cells or text (depending on edit/command mode)."
 msgstr ""
 
-#: packages/notebook/src/searchprovider.ts:510 packages/notebook/src/searchprovider.ts:512
+#: packages/notebook/src/searchprovider.ts:512 packages/notebook/src/searchprovider.ts:523
 msgid "Searching outputs is expensive and requires to first rendered all outputs. Are you sure you want to search in the cell outputs?"
 msgstr ""
 
+#: packages/notebook/src/searchprovider.ts:515
+msgid "Searching outputs requires you to run all cells and render their outputs. Are you sure you want to search in the cell outputs?"
+msgstr ""
+
 #: packages/notebook/src/truststatus.tsx:30
 msgid "Notebook trusted: %1 of %2 code cells trusted."
 msgstr ""
 
 #: packages/notebook/src/truststatus.tsx:36
 msgid "Active cell trusted: %1 of %2 code cells trusted."
 msgstr ""
 
 #: packages/notebook/src/truststatus.tsx:42
 msgid "Notebook not trusted: %1 of %2 code cells trusted."
 msgstr ""
 
-#: packages/notebook/src/widget.ts:439 packages/notebook/src/widget.ts:445
+#: packages/notebook/src/widget.ts:444 packages/notebook/src/widget.ts:453 packages/notebook/src/widget.ts:470
 msgid "The notebook is empty. Click the + button on the toolbar to add a new cell."
 msgstr ""
 
-#: packages/outputarea/src/widget.ts:1054 packages/outputarea/src/widget.ts:1060 packages/outputarea/src/widget.ts:1087
+#: packages/outputarea/src/widget.ts:1096 packages/outputarea/src/widget.ts:1097 packages/outputarea/src/widget.ts:1128
 msgid "↑↓ for history. Search history with c-↑/c-↓"
 msgstr ""
 
-#: packages/outputarea/src/widget.ts:320 packages/outputarea/src/widget.ts:322
-msgid "Toggle output scrolling"
+#: packages/outputarea/src/widget.ts:640 packages/outputarea/src/widget.ts:662
+msgid "Javascript Error: %1"
 msgstr ""
 
-#: packages/outputarea/src/widget.ts:605 packages/outputarea/src/widget.ts:632
-msgid "Javascript Error: %1"
+#: packages/pluginmanager-extension/src/index.ts:100 packages/pluginmanager-extension/src/index.ts:64 packages/settingeditor-extension/src/index.ts:154
+msgid "Plugin Manager"
+msgstr ""
+
+#: packages/pluginmanager-extension/src/index.ts:133
+msgid "Refresh plugins list"
+msgstr ""
+
+#: packages/pluginmanager-extension/src/index.ts:65
+msgid "Advanced Plugin Manager"
+msgstr ""
+
+#: packages/pluginmanager-extension/src/index.ts:66
+msgid "Refresh Plugin List"
+msgstr ""
+
+#: packages/pluginmanager/src/dialogs.tsx:14
+msgid "The plugin \"%1\" cannot be disabled as it is required by other plugins:"
+msgstr ""
+
+#: packages/pluginmanager/src/dialogs.tsx:23
+msgid "Please disable the dependant plugins first."
+msgstr ""
+
+#: packages/pluginmanager/src/dialogs.tsx:35
+msgid "While the plugin \"%1\" is not required by other enabled plugins, some plugins provide optional features depending on it. These plugins are:"
+msgstr ""
+
+#: packages/pluginmanager/src/dialogs.tsx:44
+msgid "Do you want to disable it anyway?"
+msgstr ""
+
+#: packages/pluginmanager/src/model.ts:235
+msgid "This plugin is required by other plugins"
+msgstr ""
+
+#: packages/pluginmanager/src/model.ts:247
+msgid "This plugin is used by other plugins"
+msgstr ""
+
+#: packages/pluginmanager/src/model.ts:254
+msgid "Disable anyway"
+msgstr ""
+
+#: packages/pluginmanager/src/widget.tsx:109
+msgid "Description"
+msgstr ""
+
+#: packages/pluginmanager/src/widget.tsx:119
+msgid "Autostart?"
+msgstr ""
+
+#: packages/pluginmanager/src/widget.tsx:123
+msgid "Defer"
+msgstr ""
+
+#: packages/pluginmanager/src/widget.tsx:139
+msgid "Depends on"
+msgstr ""
+
+#: packages/pluginmanager/src/widget.tsx:149
+msgid "Extension"
+msgstr ""
+
+#: packages/pluginmanager/src/widget.tsx:156
+msgid "Provides"
+msgstr ""
+
+#: packages/pluginmanager/src/widget.tsx:181
+msgid "This plugin is locked."
+msgstr ""
+
+#: packages/pluginmanager/src/widget.tsx:182
+msgid "To enable/disable, please acknowledge the disclaimer."
+msgstr ""
+
+#: packages/pluginmanager/src/widget.tsx:186
+msgid "Disable %1 plugin"
+msgstr ""
+
+#: packages/pluginmanager/src/widget.tsx:187
+msgid "Enable %1 plugin"
+msgstr ""
+
+#: packages/pluginmanager/src/widget.tsx:205
+msgid "This plugin was locked by system administrator or is a critical dependency and cannot be enabled/disabled."
+msgstr ""
+
+#: packages/pluginmanager/src/widget.tsx:253
+msgid "Customise your experience/improve performance by disabling plugins you do not need. To disable or uninstall an entire extension use the Extension Manager instead. Changes will apply after reloading JupyterLab."
+msgstr ""
+
+#: packages/pluginmanager/src/widget.tsx:266
+msgid "I understand that disabling core application plugins may render features and parts of the user interface unavailable and recovery using `jupyter labextension enable <plugin-name>` command may be required"
+msgstr ""
+
+#: packages/pluginmanager/src/widget.tsx:288
+msgid "Filter"
+msgstr ""
+
+#: packages/pluginmanager/src/widget.tsx:64
+msgid "Error querying installed extensions%1"
+msgstr ""
+
+#: packages/pluginmanager/src/widget.tsx:71
+msgid "Updating plugin list…"
+msgstr ""
+
+#: packages/pluginmanager/src/widget.tsx:97
+msgid "Plugin"
 msgstr ""
 
 #: packages/property-inspector/src/index.ts:189
 msgid "No properties to inspect."
 msgstr "Nu există proprietăți de inspectat."
 
-#: packages/rendermime-extension/src/index.ts:67
+#: packages/rendermime-extension/src/index.ts:69
 msgid "Handle Local Link"
 msgstr "Gestionează Link-ul Local"
 
 #: packages/rendermime/src/renderers.ts:62
 msgid "This HTML output contains inline scripts. Are you sure that you want to run arbitrary Javascript within your JupyterLab session?"
 msgstr ""
 
-#: packages/rendermime/src/widgets.ts:428 packages/rendermime/src/widgets.ts:446
+#: packages/rendermime/src/widgets.ts:464 packages/rendermime/src/widgets.ts:492
 msgid "JavaScript output is disabled in JupyterLab"
 msgstr "Output-ul JavaScript este dezactivat în JupyterLab"
 
-#: packages/running-extension/src/index.ts:66
-msgid "Running Terminals and Kernels"
-msgstr ""
-
-#: packages/running-extension/src/index.ts:69
+#: packages/running-extension/src/index.ts:101 packages/running-extension/src/index.ts:69
 msgid "Running Sessions section"
 msgstr ""
 
-#: packages/running-extension/src/index.ts:86
+#: packages/running-extension/src/index.ts:115 packages/running-extension/src/index.ts:86
 msgid "Sessions and Tabs"
 msgstr ""
 
-#: packages/running-extension/src/kernels.ts:107
+#: packages/running-extension/src/index.ts:171
+msgid "Tabs and Running Sessions"
+msgstr ""
+
+#: packages/running-extension/src/index.ts:179
+msgid "Search Tabs and Running Sessions"
+msgstr ""
+
+#: packages/running-extension/src/index.ts:184
+msgid "Running"
+msgstr ""
+
+#: packages/running-extension/src/index.ts:66 packages/running-extension/src/index.ts:96
+msgid "Running Terminals and Kernels"
+msgstr ""
+
+#: packages/running-extension/src/kernels.ts:107 packages/running-extension/src/kernels.tsx:128
 msgid "Unknown Session"
 msgstr ""
 
-#: packages/running-extension/src/kernels.ts:250
+#: packages/running-extension/src/kernels.ts:250 packages/running-extension/src/kernels.tsx:320
 msgid "%1\n"
 "Path: %2"
 msgstr ""
 
-#: packages/running-extension/src/kernels.ts:49
+#: packages/running-extension/src/kernels.ts:49 packages/running-extension/src/kernels.tsx:54
 msgid "Kernels"
 msgstr "Kernel-uri"
 
-#: packages/running-extension/src/kernels.ts:68
+#: packages/running-extension/src/kernels.ts:68 packages/running-extension/src/kernels.tsx:88
 msgid "Are you sure you want to permanently shut down all running kernels?"
 msgstr ""
 
-#: packages/running-extension/src/kernels.ts:77
+#: packages/running-extension/src/kernels.ts:77 packages/running-extension/src/kernels.tsx:98
 msgid "New Console for Kernel"
 msgstr ""
 
-#: packages/running-extension/src/kernels.ts:88
+#: packages/running-extension/src/kernels.ts:88 packages/running-extension/src/kernels.tsx:109
 msgid "New Notebook for Kernel"
 msgstr ""
 
+#: packages/running-extension/src/kernels.tsx:329
+msgid "No sessions connected"
+msgstr ""
+
+#: packages/running-extension/src/kernels.tsx:333
+msgid "%1 and %2 more"
+msgstr ""
+
 #: packages/running-extension/src/opentabs.ts:70
 msgid "Open Tabs"
 msgstr ""
 
 #: packages/running-extension/src/opentabs.ts:87
 msgid "Close All"
 msgstr ""
 
 #: packages/running-extension/src/opentabs.ts:88
 msgid "Are you sure you want to close all open tabs?"
 msgstr ""
 
-#: packages/running/src/index.tsx:443
+#: packages/running-extension/src/recents.ts:31
+msgid "Recently Closed"
+msgstr ""
+
+#: packages/running-extension/src/recents.ts:46
+msgid "Forget"
+msgstr ""
+
+#: packages/running-extension/src/recents.ts:47
+msgid "Forget All"
+msgstr ""
+
+#: packages/running-extension/src/recents.ts:48
+msgid "Are you sure you want to clear recently closed tabs?"
+msgstr ""
+
+#: packages/running/src/index.tsx:366
+msgid "Search"
+msgstr ""
+
+#: packages/running/src/index.tsx:445 packages/running/src/index.tsx:765
 msgid "Refresh List"
 msgstr "Reîmprospătează Lista"
 
-#: packages/settingeditor-extension/src/index.ts:145
+#: packages/running/src/index.tsx:614
+msgid "Switch to List View"
+msgstr ""
+
+#: packages/running/src/index.tsx:615
+msgid "Switch to Tree View"
+msgstr ""
+
+#: packages/running/src/index.tsx:627
+msgid "Collapse All"
+msgstr ""
+
+#: packages/running/src/index.tsx:628
+msgid "Expand All"
+msgstr ""
+
+#: packages/running/src/index.tsx:885
+msgid "No matches"
+msgstr ""
+
+#: packages/settingeditor-extension/src/index.ts:165
 msgid "JSON Settings Editor"
 msgstr ""
 
-#: packages/settingeditor-extension/src/index.ts:152 packages/settingeditor-extension/src/index.ts:187 packages/settingeditor-extension/src/index.ts:319 packages/settingeditor/src/pluginlist.tsx:467
+#: packages/settingeditor-extension/src/index.ts:172 packages/settingeditor-extension/src/index.ts:207 packages/settingeditor-extension/src/index.ts:339 packages/settingeditor/src/pluginlist.tsx:467
 msgid "Settings"
 msgstr "Setări"
 
-#: packages/settingeditor-extension/src/index.ts:181
+#: packages/settingeditor-extension/src/index.ts:201
 msgid "Settings Editor"
 msgstr ""
 
-#: packages/settingeditor-extension/src/index.ts:309 packages/settingeditor-extension/src/index.ts:315
+#: packages/settingeditor-extension/src/index.ts:329 packages/settingeditor-extension/src/index.ts:335
 msgid "Advanced Settings Editor"
 msgstr ""
 
-#: packages/settingeditor-extension/src/index.ts:329
+#: packages/settingeditor-extension/src/index.ts:349
 msgid "Revert User Settings"
 msgstr ""
 
-#: packages/settingeditor-extension/src/index.ts:336
+#: packages/settingeditor-extension/src/index.ts:356
 msgid "Save User Settings"
 msgstr ""
 
 #: packages/settingeditor/src/InstructionsPlaceholder.tsx:21
 msgid "No Plugin Selected"
 msgstr ""
 
@@ -6569,20 +7250,16 @@
 msgid "Do you want to leave without saving?"
 msgstr ""
 
 #: packages/settingeditor/src/plugineditor.ts:255
 msgid "Your changes were not saved."
 msgstr ""
 
-#: packages/settingeditor/src/pluginlist.tsx:454 packages/shortcuts-extension/src/components/TopNav.tsx:167
-msgid "Search…"
-msgstr ""
-
-#: packages/settingeditor/src/pluginlist.tsx:461
-msgid "Modified"
+#: packages/settingeditor/src/pluginlist.tsx:454
+msgid "Search settings…"
 msgstr ""
 
 #: packages/settingeditor/src/pluginlist.tsx:473
 msgid "No items match your search."
 msgstr ""
 
 #: packages/settingeditor/src/raweditor.ts:368
@@ -6597,31 +7274,43 @@
 msgid "Unsaved changes due to validation error. Continue without saving?"
 msgstr ""
 
 #: packages/settingeditor/src/settingseditor.tsx:135
 msgid "Some changes have not been saved. Continue without saving?"
 msgstr ""
 
-#: packages/shortcuts-extension/src/components/ShortcutInput.tsx:445
+#: packages/shortcuts-extension/src/components/ShortcutInput.tsx:389 packages/shortcuts-extension/src/components/ShortcutInput.tsx:445 packages/shortcuts-extension/src/components/ShortcutInput.tsx:446
 msgid "press keys"
 msgstr ""
 
-#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:218
-msgid "Shortcut already in use by %1. Overwrite it?"
+#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:123
+msgid "(Command label missing)"
 msgstr ""
 
-#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:260 packages/shortcuts-extension/src/components/ShortcutItem.tsx:76
+#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:135 packages/shortcuts-extension/src/components/ShortcutItem.tsx:260 packages/shortcuts-extension/src/components/ShortcutItem.tsx:76 packages/workspaces-extension/src/commands.ts:327
 msgid "Reset"
 msgstr ""
 
-#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:332
+#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:147
+msgid "Custom"
+msgstr ""
+
+#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:147
+msgid "Default"
+msgstr ""
+
+#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:194 packages/shortcuts-extension/src/components/ShortcutItem.tsx:332
 msgid "or"
 msgstr ""
 
-#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:416 packages/shortcuts-extension/src/components/ShortcutItem.tsx:66 packages/shortcuts-extension/src/components/ShortcutItem.tsx:71 packages/ui-components/src/components/form.tsx:212
+#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:218 packages/shortcuts-extension/src/components/ShortcutItem.tsx:333
+msgid "Shortcut already in use by %1. Overwrite it?"
+msgstr ""
+
+#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:266 packages/shortcuts-extension/src/components/ShortcutItem.tsx:416 packages/shortcuts-extension/src/components/ShortcutItem.tsx:66 packages/shortcuts-extension/src/components/ShortcutItem.tsx:71 packages/ui-components/src/components/form.tsx:212
 msgid "Add"
 msgstr ""
 
 #: packages/shortcuts-extension/src/components/ShortcutItem.tsx:51
 msgid "Edit First"
 msgstr ""
 
@@ -6641,51 +7330,83 @@
 msgid "Add another shortcut"
 msgstr ""
 
 #: packages/shortcuts-extension/src/components/ShortcutItem.tsx:77
 msgid "Reset shortcut back to default"
 msgstr ""
 
-#: packages/shortcuts-extension/src/components/TopNav.tsx:126
-msgid "Toggle Selectors"
+#: packages/shortcuts-extension/src/components/TopNav.tsx:113 packages/shortcuts-extension/src/components/TopNav.tsx:165
+msgid "Search shortcuts"
 msgstr ""
 
-#: packages/shortcuts-extension/src/components/TopNav.tsx:127
-msgid "Toggle command selectors"
+#: packages/shortcuts-extension/src/components/TopNav.tsx:117 packages/shortcuts-extension/src/components/TopNav.tsx:168
+msgid "Search…"
 msgstr ""
 
-#: packages/shortcuts-extension/src/components/TopNav.tsx:136 packages/shortcuts-extension/src/components/TopNav.tsx:92
-msgid "Reset All"
+#: packages/shortcuts-extension/src/components/TopNav.tsx:126 packages/shortcuts-extension/src/index.ts:159
+msgid "Toggle Selectors"
 msgstr ""
 
-#: packages/shortcuts-extension/src/components/TopNav.tsx:137
-msgid "Reset all shortcuts"
+#: packages/shortcuts-extension/src/components/TopNav.tsx:127 packages/shortcuts-extension/src/index.ts:160
+msgid "Toggle command selectors"
 msgstr ""
 
-#: packages/shortcuts-extension/src/components/TopNav.tsx:180
+#: packages/shortcuts-extension/src/components/TopNav.tsx:129 packages/shortcuts-extension/src/components/TopNav.tsx:181
 msgid "Category"
 msgstr ""
 
-#: packages/shortcuts-extension/src/components/TopNav.tsx:183
+#: packages/shortcuts-extension/src/components/TopNav.tsx:132 packages/shortcuts-extension/src/components/TopNav.tsx:184
 msgid "Shortcut"
 msgstr ""
 
-#: packages/shortcuts-extension/src/components/TopNav.tsx:187
+#: packages/shortcuts-extension/src/components/TopNav.tsx:136 packages/shortcuts-extension/src/components/TopNav.tsx:188
 msgid "Selectors"
 msgstr ""
 
-#: packages/shortcuts-extension/src/components/TopNav.tsx:85
+#: packages/shortcuts-extension/src/components/TopNav.tsx:136 packages/shortcuts-extension/src/components/TopNav.tsx:69 packages/shortcuts-extension/src/components/TopNav.tsx:92 packages/shortcuts-extension/src/index.ts:169
+msgid "Reset All"
+msgstr ""
+
+#: packages/shortcuts-extension/src/components/TopNav.tsx:137 packages/shortcuts-extension/src/index.ts:170
+msgid "Reset all shortcuts"
+msgstr ""
+
+#: packages/shortcuts-extension/src/components/TopNav.tsx:62 packages/shortcuts-extension/src/components/TopNav.tsx:85
 msgid "Hide Selectors"
 msgstr ""
 
-#: packages/shortcuts-extension/src/components/TopNav.tsx:86
+#: packages/shortcuts-extension/src/components/TopNav.tsx:63 packages/shortcuts-extension/src/components/TopNav.tsx:86
 msgid "Show Selectors"
 msgstr ""
 
+#: packages/shortcuts-extension/src/index.ts:107
+msgid "Edit Keybinding"
+msgstr ""
+
+#: packages/shortcuts-extension/src/index.ts:108
+msgid "Edit existing keybinding"
+msgstr ""
+
+#: packages/shortcuts-extension/src/index.ts:125
+msgid "Delete Keybinding"
+msgstr ""
+
+#: packages/shortcuts-extension/src/index.ts:126
+msgid "Delete chosen keybinding"
+msgstr ""
+
 #: packages/shortcuts-extension/src/index.ts:143
+msgid "Add Keybinding"
+msgstr ""
+
+#: packages/shortcuts-extension/src/index.ts:144
+msgid "Add new keybinding for existing shortcut target"
+msgstr ""
+
+#: packages/shortcuts-extension/src/index.ts:152 packages/shortcuts-extension/src/index.ts:232
 msgid "Note: To disable a system default shortcut,\n"
 "copy it to User Preferences and add the\n"
 "\"disabled\" key, for example:\n"
 "{\n"
 "    \"command\": \"application:activate-next-tab\",\n"
 "    \"keys\": [\n"
 "        \"Ctrl Shift ]\"\n"
@@ -6707,23 +7428,23 @@
 msgstr ""
 
 #: packages/terminal-extension/src/index.ts:191
 msgctxt "menu"
 msgid "Terminal Theme"
 msgstr ""
 
-#: packages/terminal-extension/src/index.ts:196 packages/terminal-extension/src/index.ts:251 packages/terminal-extension/src/index.ts:534 packages/terminal-extension/src/index.ts:540
+#: packages/terminal-extension/src/index.ts:196 packages/terminal-extension/src/index.ts:251 packages/terminal-extension/src/index.ts:540
 msgid "Inherit"
 msgstr ""
 
-#: packages/terminal-extension/src/index.ts:204 packages/terminal-extension/src/index.ts:258 packages/terminal-extension/src/index.ts:535 packages/terminal-extension/src/index.ts:541
+#: packages/terminal-extension/src/index.ts:204 packages/terminal-extension/src/index.ts:258 packages/terminal-extension/src/index.ts:541
 msgid "Light"
 msgstr ""
 
-#: packages/terminal-extension/src/index.ts:210 packages/terminal-extension/src/index.ts:263 packages/terminal-extension/src/index.ts:536 packages/terminal-extension/src/index.ts:542
+#: packages/terminal-extension/src/index.ts:210 packages/terminal-extension/src/index.ts:263 packages/terminal-extension/src/index.ts:542
 msgid "Dark"
 msgstr ""
 
 #: packages/terminal-extension/src/index.ts:316
 msgid "Terminals"
 msgstr ""
 
@@ -6735,58 +7456,62 @@
 msgid "New Terminal"
 msgstr ""
 
 #: packages/terminal-extension/src/index.ts:351
 msgid "Start a new terminal session"
 msgstr ""
 
-#: packages/terminal-extension/src/index.ts:389 packages/terminal-extension/src/index.ts:395
+#: packages/terminal-extension/src/index.ts:395
 msgid "Open a terminal by its `name`."
 msgstr ""
 
-#: packages/terminal-extension/src/index.ts:407 packages/terminal-extension/src/index.ts:413
+#: packages/terminal-extension/src/index.ts:413
 msgid "Refresh Terminal"
 msgstr ""
 
-#: packages/terminal-extension/src/index.ts:408 packages/terminal-extension/src/index.ts:414
+#: packages/terminal-extension/src/index.ts:414
 msgid "Refresh the current terminal session"
 msgstr ""
 
-#: packages/terminal-extension/src/index.ts:492 packages/terminal-extension/src/index.ts:498
+#: packages/terminal-extension/src/index.ts:498
 msgid "Shutdown Terminal"
 msgstr ""
 
-#: packages/terminal-extension/src/index.ts:506 packages/terminal-extension/src/index.ts:512
+#: packages/terminal-extension/src/index.ts:512
 msgid "Increase Terminal Font Size"
 msgstr ""
 
-#: packages/terminal-extension/src/index.ts:520 packages/terminal-extension/src/index.ts:526
+#: packages/terminal-extension/src/index.ts:526
 msgid "Decrease Terminal Font Size"
 msgstr ""
 
-#: packages/terminal-extension/src/index.ts:542 packages/terminal-extension/src/index.ts:548
+#: packages/terminal-extension/src/index.ts:548
 msgid "Set terminal theme to the provided `theme`."
 msgstr ""
 
-#: packages/terminal-extension/src/index.ts:550 packages/terminal-extension/src/index.ts:556
+#: packages/terminal-extension/src/index.ts:556
 msgid "Use Terminal Theme: %1"
 msgstr ""
 
-#: packages/terminal-extension/src/index.ts:553 packages/terminal-extension/src/index.ts:559
+#: packages/terminal-extension/src/index.ts:559
 msgid "Set the terminal theme"
 msgstr ""
 
 #: packages/terminal/src/widget.ts:345
 msgid "Terminal %1"
 msgstr ""
 
 #: packages/theme-dark-extension/src/index.ts:31
 msgid "JupyterLab Dark"
 msgstr ""
 
+#: packages/theme-dark-high-contrast-extension/src/index.ts:31
+msgid "JupyterLab Dark High Contrast"
+msgstr ""
+
 #: packages/theme-light-extension/src/index.ts:31
 msgid "JupyterLab Light"
 msgstr ""
 
 #: packages/toc-extension/src/index.ts:113
 msgid "Show output headings"
 msgstr ""
@@ -6823,27 +7548,27 @@
 msgid "Open the tooltip"
 msgstr ""
 
 #: packages/tooltip-extension/src/index.ts:56
 msgid "Dismiss the tooltip"
 msgstr ""
 
-#: packages/translation-extension/src/index.ts:141 packages/translation-extension/src/index.ts:150
+#: packages/translation-extension/src/index.ts:150
 msgid "Change interface language?"
 msgstr ""
 
-#: packages/translation-extension/src/index.ts:142 packages/translation-extension/src/index.ts:151
+#: packages/translation-extension/src/index.ts:151
 msgid "After changing the interface language to %1, you will need to reload JupyterLab to see the changes."
 msgstr ""
 
-#: packages/translation-extension/src/index.ts:148 packages/translation-extension/src/index.ts:157
+#: packages/translation-extension/src/index.ts:157
 msgid "Change and reload"
 msgstr ""
 
-#: packages/translation-extension/src/index.ts:175 packages/translation-extension/src/index.ts:184
+#: packages/translation-extension/src/index.ts:184
 msgid "Display Languages"
 msgstr ""
 
 #: packages/ui-components/src/components/form.tsx:146
 msgid "Move down"
 msgstr ""
 
@@ -6851,31 +7576,190 @@
 msgid "Move up"
 msgstr ""
 
 #: packages/ui-components/src/components/form.tsx:183 packages/ui-components/src/components/form.tsx:570
 msgid "Remove"
 msgstr ""
 
-#: packages/ui-components/src/components/form.tsx:580 packages/ui-components/src/components/form.tsx:582
+#: packages/ui-components/src/components/form.tsx:582
 msgid "Default: %1"
 msgstr ""
 
-#: packages/ui-components/src/components/sidepanel.ts:118
+#: packages/ui-components/src/components/sidepanel.ts:117
 msgid "side panel actions"
 msgstr ""
 
 #: packages/ui-components/src/components/sidepanel.ts:41
 msgid "side panel content"
 msgstr ""
 
-#: packages/ui-components/src/components/toolbar.tsx:971 packages/ui-components/src/components/toolbar.tsx:975
+#: packages/ui-components/src/components/toolbar.tsx:1140 packages/ui-components/src/components/toolbar.tsx:1180 packages/ui-components/src/components/toolbar.tsx:1191 packages/ui-components/src/components/toolbar.tsx:1192
 msgid "More commands"
 msgstr ""
 
 #: packages/ui-components/src/icon/widgets/tabbarsvg.ts:51
 msgid "Close %1"
 msgstr ""
 
 #: packages/ui-components/src/icon/widgets/tabbarsvg.ts:52
 msgid "Close tab"
 msgstr ""
 
+#: packages/workspaces-extension/src/commands.ts:104
+msgid "Naming the workspace will create a unique URL. The name may contain letters, numbers, hyphens (-), and underscores (_)."
+msgstr ""
+
+#: packages/workspaces-extension/src/commands.ts:120
+msgid "workspace-name"
+msgstr ""
+
+#: packages/workspaces-extension/src/commands.ts:132
+msgid "Open Workspace"
+msgstr ""
+
+#: packages/workspaces-extension/src/commands.ts:133
+msgid "Open Workspace…"
+msgstr ""
+
+#: packages/workspaces-extension/src/commands.ts:140
+msgid "Choose Workspace To Open"
+msgstr ""
+
+#: packages/workspaces-extension/src/commands.ts:141
+msgid "Choose an existing workspace to open."
+msgstr ""
+
+#: packages/workspaces-extension/src/commands.ts:143 packages/workspaces-extension/src/commands.ts:180 packages/workspaces-extension/src/commands.ts:243 packages/workspaces-extension/src/commands.ts:406
+msgid "Choose"
+msgstr ""
+
+#: packages/workspaces-extension/src/commands.ts:169
+msgid "Delete Workspace…"
+msgstr ""
+
+#: packages/workspaces-extension/src/commands.ts:177
+msgid "Choose Workspace To Delete"
+msgstr ""
+
+#: packages/workspaces-extension/src/commands.ts:178
+msgid "Choose an existing workspace to delete."
+msgstr ""
+
+#: packages/workspaces-extension/src/commands.ts:192
+msgid "Delete workspace"
+msgstr ""
+
+#: packages/workspaces-extension/src/commands.ts:193
+msgid "Deleting workspace \"%1\" will also delete its URL. A deleted workspace cannot be recovered."
+msgstr ""
+
+#: packages/workspaces-extension/src/commands.ts:211
+msgid "Create New Workspace…"
+msgstr ""
+
+#: packages/workspaces-extension/src/commands.ts:217
+msgid "Create New Workspace"
+msgstr ""
+
+#: packages/workspaces-extension/src/commands.ts:218
+msgid "Create"
+msgstr ""
+
+#: packages/workspaces-extension/src/commands.ts:233
+msgid "Clone Workspace…"
+msgstr ""
+
+#: packages/workspaces-extension/src/commands.ts:240
+msgid "Choose Workspace To Clone"
+msgstr ""
+
+#: packages/workspaces-extension/src/commands.ts:241
+msgid "Choose an existing workspace to clone."
+msgstr ""
+
+#: packages/workspaces-extension/src/commands.ts:252
+msgid "Clone Workspace"
+msgstr ""
+
+#: packages/workspaces-extension/src/commands.ts:253
+msgid "%1-clone"
+msgstr ""
+
+#: packages/workspaces-extension/src/commands.ts:254
+msgid "Clone"
+msgstr ""
+
+#: packages/workspaces-extension/src/commands.ts:273
+msgid "Rename Workspace…"
+msgstr ""
+
+#: packages/workspaces-extension/src/commands.ts:283
+msgid "Rename Workspace"
+msgstr ""
+
+#: packages/workspaces-extension/src/commands.ts:304
+msgid "Reset Workspace…"
+msgstr ""
+
+#: packages/workspaces-extension/src/commands.ts:318
+msgid "Reset Workspace"
+msgstr ""
+
+#: packages/workspaces-extension/src/commands.ts:319
+msgid "Resetting workspace %2 will close its %1 tab and return to default layout."
+msgid_plural "Resetting workspace %2 will close its %1 tabs and return to default layout."
+msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
+
+#: packages/workspaces-extension/src/commands.ts:354
+msgid "Import Workspace…"
+msgstr ""
+
+#: packages/workspaces-extension/src/commands.ts:359
+msgid "Select Workspace Files to Import"
+msgstr ""
+
+#: packages/workspaces-extension/src/commands.ts:364
+msgid "You choose one or more workspace files to import. A Jupyter Workspace File has %1 extension."
+msgstr ""
+
+#: packages/workspaces-extension/src/commands.ts:390
+msgid "Export Workspace…"
+msgstr ""
+
+#: packages/workspaces-extension/src/commands.ts:403
+msgid "Choose Workspace To Export"
+msgstr ""
+
+#: packages/workspaces-extension/src/commands.ts:404
+msgid "Choose an existing workspace to export."
+msgstr ""
+
+#: packages/workspaces-extension/src/commands.ts:417
+msgid "Choose Workspace Export Directory"
+msgstr ""
+
+#: packages/workspaces-extension/src/commands.ts:420
+msgid "The \"%1\" workspace will be saved in the chosen directory as \"%1%2\"."
+msgstr ""
+
+#: packages/workspaces-extension/src/commands.ts:472 packages/workspaces-extension/src/sidebar.ts:81
+msgid "Workspaces"
+msgstr ""
+
+#: packages/workspaces-extension/src/commands.ts:586
+msgid "Path to save the workspace in"
+msgstr ""
+
+#: packages/workspaces-extension/src/sidebar.ts:100
+msgid "Delete All"
+msgstr ""
+
+#: packages/workspaces-extension/src/sidebar.ts:101
+msgid "Are you sure you want to delete all workspaces? Deleted workspaces cannot be recovered."
+msgstr ""
+
+#: packages/workspaces-extension/src/sidebar.ts:69
+msgid "%1 workspace with %2 tabs, last modified on %3"
+msgstr ""
+
```

### Comparing `jupyterlab_language_pack_ro_ro-4.1.post2/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyterlab_git.po` & `jupyterlab_language_pack_ro_ro-4.2.post0/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyterlab_git.po`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 "X-Crowdin-Project: jupyterlab\n"
 "X-Crowdin-Project-ID: 409874\n"
 "X-Crowdin-Language: ro\n"
 "X-Crowdin-File: /main/extensions/jupyterlab_git/locale/jupyterlab_git.pot\n"
 "X-Crowdin-File-ID: 197\n"
 "Language-Team: Romanian\n"
 "Language: ro_RO\n"
-"PO-Revision-Date: 2023-10-27 08:22\n"
+"PO-Revision-Date: 2024-03-29 11:17\n"
 
 #: /schema/plugin.json:/description
 msgctxt "schema"
 msgid "jupyterlab-git settings."
 msgstr ""
 
 #: /schema/plugin.json:/jupyter.lab.menus/context[0]/submenu/label /schema/plugin.json:/jupyter.lab.menus/main[0]/label
@@ -105,14 +105,24 @@
 msgstr ""
 
 #: /schema/plugin.json:/properties/doubleClickDiff/title
 msgctxt "settings"
 msgid "Show diff on double click"
 msgstr ""
 
+#: /schema/plugin.json:/properties/hideHiddenFileWarning/description
+msgctxt "settings"
+msgid "If true, the warning popup when opening the .gitignore file without hidden files will not be displayed."
+msgstr ""
+
+#: /schema/plugin.json:/properties/hideHiddenFileWarning/title
+msgctxt "settings"
+msgid "Hide hidden file warning"
+msgstr ""
+
 #: /schema/plugin.json:/properties/historyCount/description
 msgctxt "settings"
 msgid "Number of (most recent) commits shown in the history log"
 msgstr ""
 
 #: /schema/plugin.json:/properties/historyCount/title
 msgctxt "settings"
@@ -170,386 +180,506 @@
 msgstr ""
 
 #: /schema/plugin.json:/title
 msgctxt "schema"
 msgid "Git"
 msgstr ""
 
-#: src/cloneCommand.ts:35 src/cloneCommand.ts:37 src/commandsAndMenu.tsx:286 src/commandsAndMenu.tsx:288 src/commandsAndMenu.tsx:289 src/commandsAndMenu.tsx:290 src/commandsAndMenu.tsx:293 src/components/GitPanel.tsx:454 src/components/GitPanel.tsx:470 src/components/GitPanel.tsx:475 src/components/GitPanel.tsx:483 src/components/GitPanel.tsx:497 src/components/GitPanel.tsx:505 src/components/GitPanel.tsx:604 src/components/GitPanel.tsx:605 src/components/GitPanel.tsx:688 src/components/GitPanel.tsx:707 src/components/GitPanel.tsx:708
+#: src/cloneCommand.ts:35 src/cloneCommand.ts:37 src/cloneCommand.tsx:48 src/commandsAndMenu.tsx:286 src/commandsAndMenu.tsx:288 src/commandsAndMenu.tsx:289 src/commandsAndMenu.tsx:290 src/commandsAndMenu.tsx:293 src/components/GitPanel.tsx:454 src/components/GitPanel.tsx:470 src/components/GitPanel.tsx:475 src/components/GitPanel.tsx:483 src/components/GitPanel.tsx:497 src/components/GitPanel.tsx:505 src/components/GitPanel.tsx:604 src/components/GitPanel.tsx:605 src/components/GitPanel.tsx:688 src/components/GitPanel.tsx:701 src/components/GitPanel.tsx:707 src/components/GitPanel.tsx:708
 msgid "Clone a Repository"
 msgstr ""
 
-#: src/cloneCommand.ts:36 src/cloneCommand.ts:38 src/commandsAndMenu.tsx:287 src/commandsAndMenu.tsx:289 src/commandsAndMenu.tsx:290 src/commandsAndMenu.tsx:291 src/commandsAndMenu.tsx:294
+#: src/cloneCommand.ts:36 src/cloneCommand.ts:38 src/cloneCommand.tsx:49 src/commandsAndMenu.tsx:287 src/commandsAndMenu.tsx:289 src/commandsAndMenu.tsx:290 src/commandsAndMenu.tsx:291 src/commandsAndMenu.tsx:294
 msgid "Clone a repository from a URL"
 msgstr ""
 
-#: src/cloneCommand.ts:40 src/cloneCommand.ts:42 src/commandsAndMenu.tsx:291 src/commandsAndMenu.tsx:293 src/commandsAndMenu.tsx:294 src/commandsAndMenu.tsx:295 src/commandsAndMenu.tsx:298
+#: src/cloneCommand.ts:40 src/cloneCommand.ts:42 src/cloneCommand.tsx:53 src/commandsAndMenu.tsx:291 src/commandsAndMenu.tsx:293 src/commandsAndMenu.tsx:294 src/commandsAndMenu.tsx:295 src/commandsAndMenu.tsx:298
 msgid "Clone a repo"
 msgstr ""
 
-#: src/cloneCommand.ts:44 src/cloneCommand.ts:46 src/commandsAndMenu.tsx:1001 src/commandsAndMenu.tsx:1002 src/commandsAndMenu.tsx:1044 src/commandsAndMenu.tsx:1045 src/commandsAndMenu.tsx:1070 src/commandsAndMenu.tsx:1086 src/commandsAndMenu.tsx:1108 src/commandsAndMenu.tsx:1112 src/commandsAndMenu.tsx:1113 src/commandsAndMenu.tsx:1129 src/commandsAndMenu.tsx:1141 src/commandsAndMenu.tsx:1151 src/commandsAndMenu.tsx:1155 src/commandsAndMenu.tsx:1184 src/commandsAndMenu.tsx:1370 src/commandsAndMenu.tsx:1375 src/commandsAndMenu.tsx:1413 src/commandsAndMenu.tsx:1418 src/commandsAndMenu.tsx:182 src/commandsAndMenu.tsx:184 src/commandsAndMenu.tsx:185 src/commandsAndMenu.tsx:186 src/commandsAndMenu.tsx:189 src/commandsAndMenu.tsx:191 src/commandsAndMenu.tsx:192 src/commandsAndMenu.tsx:193 src/commandsAndMenu.tsx:194 src/commandsAndMenu.tsx:200 src/commandsAndMenu.tsx:204 src/commandsAndMenu.tsx:210 src/commandsAndMenu.tsx:211 src/commandsAndMenu.tsx:216 src/commandsAndMenu.tsx:295 src/commandsAndMenu.tsx:297 src/commandsAndMenu.tsx:298 src/commandsAndMenu.tsx:299 src/commandsAndMenu.tsx:302 src/commandsAndMenu.tsx:317 src/commandsAndMenu.tsx:323 src/commandsAndMenu.tsx:327 src/commandsAndMenu.tsx:333 src/commandsAndMenu.tsx:334 src/commandsAndMenu.tsx:339 src/commandsAndMenu.tsx:432 src/commandsAndMenu.tsx:433 src/commandsAndMenu.tsx:449 src/commandsAndMenu.tsx:471 src/commandsAndMenu.tsx:475 src/commandsAndMenu.tsx:481 src/commandsAndMenu.tsx:482 src/commandsAndMenu.tsx:487 src/commandsAndMenu.tsx:743 src/commandsAndMenu.tsx:745 src/commandsAndMenu.tsx:751 src/commandsAndMenu.tsx:756 src/commandsAndMenu.tsx:776 src/commandsAndMenu.tsx:777 src/commandsAndMenu.tsx:786 src/commandsAndMenu.tsx:788 src/commandsAndMenu.tsx:794 src/commandsAndMenu.tsx:799 src/commandsAndMenu.tsx:819 src/commandsAndMenu.tsx:820 src/commandsAndMenu.tsx:878 src/commandsAndMenu.tsx:921 src/commandsAndMenu.tsx:942 src/commandsAndMenu.tsx:985 src/components/BranchMenu.tsx:344 src/components/BranchMenu.tsx:367 src/components/BranchMenu.tsx:374 src/components/BranchPicker.tsx:196 src/components/FileList.tsx:182 src/components/FileList.tsx:191 src/components/FileList.tsx:193 src/components/FileList.tsx:196 src/components/FileList.tsx:207 src/components/FileList.tsx:216 src/components/FileList.tsx:218 src/components/FileList.tsx:257 src/components/FileList.tsx:267 src/components/MergeBranchDialog.tsx:173 src/components/NewBranchDialog.tsx:202 src/components/NewBranchDialog.tsx:209 src/components/NewTagDialog.tsx:468 src/components/NewTagDialog.tsx:485 src/widgets/discardAllChanges.ts:25
+#: src/cloneCommand.ts:44 src/cloneCommand.ts:46 src/cloneCommand.tsx:57 src/commandsAndMenu.tsx:1001 src/commandsAndMenu.tsx:1002 src/commandsAndMenu.tsx:1044 src/commandsAndMenu.tsx:1045 src/commandsAndMenu.tsx:1070 src/commandsAndMenu.tsx:1086 src/commandsAndMenu.tsx:1108 src/commandsAndMenu.tsx:1112 src/commandsAndMenu.tsx:1113 src/commandsAndMenu.tsx:1129 src/commandsAndMenu.tsx:1141 src/commandsAndMenu.tsx:1151 src/commandsAndMenu.tsx:1155 src/commandsAndMenu.tsx:1184 src/commandsAndMenu.tsx:1370 src/commandsAndMenu.tsx:1375 src/commandsAndMenu.tsx:1413 src/commandsAndMenu.tsx:1418 src/commandsAndMenu.tsx:1558 src/commandsAndMenu.tsx:1601 src/commandsAndMenu.tsx:182 src/commandsAndMenu.tsx:184 src/commandsAndMenu.tsx:185 src/commandsAndMenu.tsx:186 src/commandsAndMenu.tsx:189 src/commandsAndMenu.tsx:191 src/commandsAndMenu.tsx:192 src/commandsAndMenu.tsx:193 src/commandsAndMenu.tsx:194 src/commandsAndMenu.tsx:200 src/commandsAndMenu.tsx:204 src/commandsAndMenu.tsx:210 src/commandsAndMenu.tsx:211 src/commandsAndMenu.tsx:216 src/commandsAndMenu.tsx:225 src/commandsAndMenu.tsx:295 src/commandsAndMenu.tsx:297 src/commandsAndMenu.tsx:298 src/commandsAndMenu.tsx:299 src/commandsAndMenu.tsx:302 src/commandsAndMenu.tsx:317 src/commandsAndMenu.tsx:323 src/commandsAndMenu.tsx:327 src/commandsAndMenu.tsx:333 src/commandsAndMenu.tsx:334 src/commandsAndMenu.tsx:339 src/commandsAndMenu.tsx:415 src/commandsAndMenu.tsx:432 src/commandsAndMenu.tsx:433 src/commandsAndMenu.tsx:449 src/commandsAndMenu.tsx:467 src/commandsAndMenu.tsx:471 src/commandsAndMenu.tsx:475 src/commandsAndMenu.tsx:481 src/commandsAndMenu.tsx:482 src/commandsAndMenu.tsx:487 src/commandsAndMenu.tsx:624 src/commandsAndMenu.tsx:743 src/commandsAndMenu.tsx:745 src/commandsAndMenu.tsx:751 src/commandsAndMenu.tsx:756 src/commandsAndMenu.tsx:776 src/commandsAndMenu.tsx:777 src/commandsAndMenu.tsx:786 src/commandsAndMenu.tsx:788 src/commandsAndMenu.tsx:794 src/commandsAndMenu.tsx:799 src/commandsAndMenu.tsx:819 src/commandsAndMenu.tsx:820 src/commandsAndMenu.tsx:878 src/commandsAndMenu.tsx:921 src/commandsAndMenu.tsx:942 src/commandsAndMenu.tsx:985 src/components/BranchMenu.tsx:344 src/components/BranchMenu.tsx:367 src/components/BranchMenu.tsx:372 src/components/BranchMenu.tsx:374 src/components/BranchPicker.tsx:196 src/components/BranchPicker.tsx:198 src/components/FileList.tsx:182 src/components/FileList.tsx:191 src/components/FileList.tsx:193 src/components/FileList.tsx:196 src/components/FileList.tsx:207 src/components/FileList.tsx:216 src/components/FileList.tsx:218 src/components/FileList.tsx:257 src/components/FileList.tsx:267 src/components/FileList.tsx:268 src/components/MergeBranchDialog.tsx:173 src/components/NewBranchDialog.tsx:197 src/components/NewBranchDialog.tsx:202 src/components/NewBranchDialog.tsx:209 src/components/NewTagDialog.tsx:468 src/components/NewTagDialog.tsx:479 src/components/NewTagDialog.tsx:485 src/widgets/discardAllChanges.ts:25
 msgid "Cancel"
 msgstr ""
 
-#: src/cloneCommand.ts:45 src/cloneCommand.ts:47
+#: src/cloneCommand.ts:45 src/cloneCommand.ts:47 src/cloneCommand.tsx:58
 msgid "Clone"
 msgstr ""
 
-#: src/cloneCommand.ts:52 src/cloneCommand.ts:54
+#: src/cloneCommand.ts:52 src/cloneCommand.ts:54 src/cloneCommand.tsx:63
 msgid "Cloning…"
 msgstr ""
 
-#: src/cloneCommand.ts:62 src/cloneCommand.ts:66 src/cloneCommand.ts:67 src/cloneCommand.ts:69 src/commandsAndMenu.tsx:313 src/commandsAndMenu.tsx:315 src/commandsAndMenu.tsx:316 src/commandsAndMenu.tsx:317 src/commandsAndMenu.tsx:320
+#: src/cloneCommand.ts:62 src/cloneCommand.ts:66 src/cloneCommand.ts:67 src/cloneCommand.ts:69 src/cloneCommand.tsx:82 src/commandsAndMenu.tsx:313 src/commandsAndMenu.tsx:315 src/commandsAndMenu.tsx:316 src/commandsAndMenu.tsx:317 src/commandsAndMenu.tsx:320
 msgid "Successfully cloned"
 msgstr ""
 
-#: src/cloneCommand.ts:73 src/cloneCommand.ts:77 src/cloneCommand.ts:78 src/cloneCommand.ts:80 src/commandsAndMenu.tsx:324 src/commandsAndMenu.tsx:326 src/commandsAndMenu.tsx:327 src/commandsAndMenu.tsx:328 src/commandsAndMenu.tsx:331
+#: src/cloneCommand.ts:73 src/cloneCommand.ts:77 src/cloneCommand.ts:78 src/cloneCommand.ts:80 src/cloneCommand.tsx:94 src/commandsAndMenu.tsx:324 src/commandsAndMenu.tsx:326 src/commandsAndMenu.tsx:327 src/commandsAndMenu.tsx:328 src/commandsAndMenu.tsx:331
 msgid "Failed to clone"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1002 src/commandsAndMenu.tsx:1003 src/commandsAndMenu.tsx:1049 src/commandsAndMenu.tsx:1065 src/commandsAndMenu.tsx:1071 src/commandsAndMenu.tsx:1087 src/commandsAndMenu.tsx:1091 src/commandsAndMenu.tsx:1109 src/commandsAndMenu.tsx:1113 src/commandsAndMenu.tsx:1120 src/commandsAndMenu.tsx:1142 src/commandsAndMenu.tsx:1349 src/commandsAndMenu.tsx:1354 src/commandsAndMenu.tsx:1371 src/commandsAndMenu.tsx:1376 src/commandsAndMenu.tsx:722 src/commandsAndMenu.tsx:724 src/commandsAndMenu.tsx:730 src/commandsAndMenu.tsx:735 src/commandsAndMenu.tsx:744 src/commandsAndMenu.tsx:746 src/commandsAndMenu.tsx:752 src/commandsAndMenu.tsx:755 src/commandsAndMenu.tsx:756 src/commandsAndMenu.tsx:757 src/commandsAndMenu.tsx:777 src/commandsAndMenu.tsx:778 src/commandsAndMenu.tsx:857 src/commandsAndMenu.tsx:879 src/commandsAndMenu.tsx:921 src/commandsAndMenu.tsx:943 src/commandsAndMenu.tsx:980 src/commandsAndMenu.tsx:981 src/components/BranchMenu.tsx:345 src/components/BranchMenu.tsx:368 src/components/BranchMenu.tsx:375
+#: src/cloneCommand.tsx:122 src/widgets/gitClone.tsx:38
+msgid "Git Clone"
+msgstr ""
+
+#: src/commandsAndMenu.tsx:1002 src/commandsAndMenu.tsx:1003 src/commandsAndMenu.tsx:1049 src/commandsAndMenu.tsx:1065 src/commandsAndMenu.tsx:1071 src/commandsAndMenu.tsx:1087 src/commandsAndMenu.tsx:1091 src/commandsAndMenu.tsx:1109 src/commandsAndMenu.tsx:1113 src/commandsAndMenu.tsx:1120 src/commandsAndMenu.tsx:1142 src/commandsAndMenu.tsx:1349 src/commandsAndMenu.tsx:1354 src/commandsAndMenu.tsx:1371 src/commandsAndMenu.tsx:1376 src/commandsAndMenu.tsx:1537 src/commandsAndMenu.tsx:1559 src/commandsAndMenu.tsx:722 src/commandsAndMenu.tsx:724 src/commandsAndMenu.tsx:730 src/commandsAndMenu.tsx:735 src/commandsAndMenu.tsx:744 src/commandsAndMenu.tsx:746 src/commandsAndMenu.tsx:752 src/commandsAndMenu.tsx:755 src/commandsAndMenu.tsx:756 src/commandsAndMenu.tsx:757 src/commandsAndMenu.tsx:777 src/commandsAndMenu.tsx:778 src/commandsAndMenu.tsx:857 src/commandsAndMenu.tsx:879 src/commandsAndMenu.tsx:921 src/commandsAndMenu.tsx:943 src/commandsAndMenu.tsx:980 src/commandsAndMenu.tsx:981 src/components/BranchMenu.tsx:345 src/components/BranchMenu.tsx:368 src/components/BranchMenu.tsx:373 src/components/BranchMenu.tsx:375
 msgid "Delete"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1004 src/commandsAndMenu.tsx:1007 src/commandsAndMenu.tsx:1068 src/commandsAndMenu.tsx:1071 src/commandsAndMenu.tsx:1128 src/commandsAndMenu.tsx:1129 src/commandsAndMenu.tsx:1131 src/commandsAndMenu.tsx:1132 src/commandsAndMenu.tsx:1197 src/commandsAndMenu.tsx:1200 src/commandsAndMenu.tsx:1213 src/commandsAndMenu.tsx:1216 src/commandsAndMenu.tsx:1235 src/commandsAndMenu.tsx:1238 src/commandsAndMenu.tsx:1239 src/commandsAndMenu.tsx:1242 src/commandsAndMenu.tsx:1268 src/commandsAndMenu.tsx:1271 src/commandsAndMenu.tsx:1497 src/commandsAndMenu.tsx:1500 src/commandsAndMenu.tsx:1502 src/commandsAndMenu.tsx:1505 src/commandsAndMenu.tsx:869 src/commandsAndMenu.tsx:871 src/commandsAndMenu.tsx:872 src/commandsAndMenu.tsx:874 src/commandsAndMenu.tsx:877 src/commandsAndMenu.tsx:880 src/commandsAndMenu.tsx:882 src/commandsAndMenu.tsx:885 src/commandsAndMenu.tsx:902 src/commandsAndMenu.tsx:903 src/commandsAndMenu.tsx:905 src/commandsAndMenu.tsx:906
+#: src/commandsAndMenu.tsx:1004 src/commandsAndMenu.tsx:1007 src/commandsAndMenu.tsx:1068 src/commandsAndMenu.tsx:1071 src/commandsAndMenu.tsx:1128 src/commandsAndMenu.tsx:1129 src/commandsAndMenu.tsx:1131 src/commandsAndMenu.tsx:1132 src/commandsAndMenu.tsx:1197 src/commandsAndMenu.tsx:1200 src/commandsAndMenu.tsx:1213 src/commandsAndMenu.tsx:1216 src/commandsAndMenu.tsx:1235 src/commandsAndMenu.tsx:1238 src/commandsAndMenu.tsx:1239 src/commandsAndMenu.tsx:1242 src/commandsAndMenu.tsx:1268 src/commandsAndMenu.tsx:1271 src/commandsAndMenu.tsx:1497 src/commandsAndMenu.tsx:1500 src/commandsAndMenu.tsx:1502 src/commandsAndMenu.tsx:1505 src/commandsAndMenu.tsx:1694 src/commandsAndMenu.tsx:1697 src/commandsAndMenu.tsx:869 src/commandsAndMenu.tsx:871 src/commandsAndMenu.tsx:872 src/commandsAndMenu.tsx:874 src/commandsAndMenu.tsx:877 src/commandsAndMenu.tsx:880 src/commandsAndMenu.tsx:882 src/commandsAndMenu.tsx:885 src/commandsAndMenu.tsx:902 src/commandsAndMenu.tsx:903 src/commandsAndMenu.tsx:905 src/commandsAndMenu.tsx:906
 msgid "Ignore"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1004 src/commandsAndMenu.tsx:999
+#: src/commandsAndMenu.tsx:1004 src/commandsAndMenu.tsx:1181 src/commandsAndMenu.tsx:999
 msgid "Failed to get the stash"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1007 src/commandsAndMenu.tsx:1066 src/commandsAndMenu.tsx:1067 src/commandsAndMenu.tsx:1135 src/commandsAndMenu.tsx:1151 src/commandsAndMenu.tsx:1173 src/commandsAndMenu.tsx:1177 src/commandsAndMenu.tsx:1206 src/commandsAndMenu.tsx:1435 src/commandsAndMenu.tsx:1440 src/commandsAndMenu.tsx:808 src/commandsAndMenu.tsx:810 src/commandsAndMenu.tsx:816 src/commandsAndMenu.tsx:821 src/commandsAndMenu.tsx:841 src/commandsAndMenu.tsx:842 src/commandsAndMenu.tsx:943
+#: src/commandsAndMenu.tsx:1004 src/commandsAndMenu.tsx:834 src/commandsAndMenu.tsx:839
+msgid "Failed to rebase branch '%1' onto '%2'."
+msgstr ""
+
+#: src/commandsAndMenu.tsx:1007 src/commandsAndMenu.tsx:1066 src/commandsAndMenu.tsx:1067 src/commandsAndMenu.tsx:1135 src/commandsAndMenu.tsx:1151 src/commandsAndMenu.tsx:1173 src/commandsAndMenu.tsx:1177 src/commandsAndMenu.tsx:1206 src/commandsAndMenu.tsx:1435 src/commandsAndMenu.tsx:1440 src/commandsAndMenu.tsx:1623 src/commandsAndMenu.tsx:808 src/commandsAndMenu.tsx:810 src/commandsAndMenu.tsx:816 src/commandsAndMenu.tsx:821 src/commandsAndMenu.tsx:841 src/commandsAndMenu.tsx:842 src/commandsAndMenu.tsx:943
 msgid "Discard changes for %1 failed."
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1008 src/commandsAndMenu.tsx:1024 src/commandsAndMenu.tsx:1046 src/commandsAndMenu.tsx:1050 src/commandsAndMenu.tsx:1079 src/commandsAndMenu.tsx:1308 src/commandsAndMenu.tsx:1313 src/commandsAndMenu.tsx:681 src/commandsAndMenu.tsx:683 src/commandsAndMenu.tsx:689 src/commandsAndMenu.tsx:694 src/commandsAndMenu.tsx:714 src/commandsAndMenu.tsx:715 src/commandsAndMenu.tsx:816 src/commandsAndMenu.tsx:880 src/commandsAndMenu.tsx:939 src/commandsAndMenu.tsx:940
+#: src/commandsAndMenu.tsx:1008 src/commandsAndMenu.tsx:1024 src/commandsAndMenu.tsx:1046 src/commandsAndMenu.tsx:1050 src/commandsAndMenu.tsx:1079 src/commandsAndMenu.tsx:1308 src/commandsAndMenu.tsx:1313 src/commandsAndMenu.tsx:1496 src/commandsAndMenu.tsx:681 src/commandsAndMenu.tsx:683 src/commandsAndMenu.tsx:689 src/commandsAndMenu.tsx:694 src/commandsAndMenu.tsx:714 src/commandsAndMenu.tsx:715 src/commandsAndMenu.tsx:816 src/commandsAndMenu.tsx:880 src/commandsAndMenu.tsx:939 src/commandsAndMenu.tsx:940
 msgid "Track"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1009 src/commandsAndMenu.tsx:1013 src/commandsAndMenu.tsx:1014 src/commandsAndMenu.tsx:1068 src/commandsAndMenu.tsx:1069 src/commandsAndMenu.tsx:1082 src/commandsAndMenu.tsx:1098 src/commandsAndMenu.tsx:1120 src/commandsAndMenu.tsx:1124 src/commandsAndMenu.tsx:1137 src/commandsAndMenu.tsx:1153 src/commandsAndMenu.tsx:1175 src/commandsAndMenu.tsx:1179 src/commandsAndMenu.tsx:1208 src/commandsAndMenu.tsx:1382 src/commandsAndMenu.tsx:1387 src/commandsAndMenu.tsx:1437 src/commandsAndMenu.tsx:1442 src/commandsAndMenu.tsx:954 src/components/Alert.tsx:106 src/components/Alert.tsx:123 src/components/BranchMenu.tsx:69 src/components/BranchMenu.tsx:70 src/components/TagMenu.tsx:63 src/components/TagMenu.tsx:65 src/index.ts:135 src/index.ts:136 src/index.ts:141
+#: src/commandsAndMenu.tsx:1009 src/commandsAndMenu.tsx:1013 src/commandsAndMenu.tsx:1014 src/commandsAndMenu.tsx:1068 src/commandsAndMenu.tsx:1069 src/commandsAndMenu.tsx:1082 src/commandsAndMenu.tsx:1098 src/commandsAndMenu.tsx:1120 src/commandsAndMenu.tsx:1124 src/commandsAndMenu.tsx:1137 src/commandsAndMenu.tsx:1153 src/commandsAndMenu.tsx:1175 src/commandsAndMenu.tsx:1179 src/commandsAndMenu.tsx:1208 src/commandsAndMenu.tsx:1382 src/commandsAndMenu.tsx:1387 src/commandsAndMenu.tsx:1437 src/commandsAndMenu.tsx:1442 src/commandsAndMenu.tsx:1570 src/commandsAndMenu.tsx:1625 src/commandsAndMenu.tsx:954 src/components/Alert.tsx:106 src/components/Alert.tsx:123 src/components/BranchMenu.tsx:68 src/components/BranchMenu.tsx:69 src/components/BranchMenu.tsx:70 src/components/TagMenu.tsx:63 src/components/TagMenu.tsx:64 src/components/TagMenu.tsx:65 src/index.ts:135 src/index.ts:136 src/index.ts:141 src/index.ts:142 src/notifications.ts:22 src/notifications.ts:53
 msgid "Dismiss"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1009 src/commandsAndMenu.tsx:1014 src/commandsAndMenu.tsx:511 src/commandsAndMenu.tsx:513 src/commandsAndMenu.tsx:518 src/commandsAndMenu.tsx:522 src/commandsAndMenu.tsx:523 src/commandsAndMenu.tsx:579 src/commandsAndMenu.tsx:643 src/commandsAndMenu.tsx:702 src/commandsAndMenu.tsx:703 src/commandsAndMenu.tsx:722 src/commandsAndMenu.tsx:738 src/commandsAndMenu.tsx:760 src/commandsAndMenu.tsx:764 src/commandsAndMenu.tsx:785
+#: src/commandsAndMenu.tsx:1009 src/commandsAndMenu.tsx:1014 src/commandsAndMenu.tsx:1190 src/commandsAndMenu.tsx:511 src/commandsAndMenu.tsx:513 src/commandsAndMenu.tsx:518 src/commandsAndMenu.tsx:522 src/commandsAndMenu.tsx:523 src/commandsAndMenu.tsx:579 src/commandsAndMenu.tsx:643 src/commandsAndMenu.tsx:702 src/commandsAndMenu.tsx:703 src/commandsAndMenu.tsx:722 src/commandsAndMenu.tsx:738 src/commandsAndMenu.tsx:760 src/commandsAndMenu.tsx:764 src/commandsAndMenu.tsx:785
 msgid "Open"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1009 src/commandsAndMenu.tsx:1031 src/commandsAndMenu.tsx:1035 src/commandsAndMenu.tsx:1064 src/commandsAndMenu.tsx:1293 src/commandsAndMenu.tsx:1298 src/commandsAndMenu.tsx:666 src/commandsAndMenu.tsx:668 src/commandsAndMenu.tsx:674 src/commandsAndMenu.tsx:679 src/commandsAndMenu.tsx:699 src/commandsAndMenu.tsx:700 src/commandsAndMenu.tsx:801 src/commandsAndMenu.tsx:865 src/commandsAndMenu.tsx:924 src/commandsAndMenu.tsx:925 src/commandsAndMenu.tsx:993
+#: src/commandsAndMenu.tsx:1009 src/commandsAndMenu.tsx:1031 src/commandsAndMenu.tsx:1035 src/commandsAndMenu.tsx:1064 src/commandsAndMenu.tsx:1293 src/commandsAndMenu.tsx:1298 src/commandsAndMenu.tsx:1481 src/commandsAndMenu.tsx:666 src/commandsAndMenu.tsx:668 src/commandsAndMenu.tsx:674 src/commandsAndMenu.tsx:679 src/commandsAndMenu.tsx:699 src/commandsAndMenu.tsx:700 src/commandsAndMenu.tsx:801 src/commandsAndMenu.tsx:865 src/commandsAndMenu.tsx:924 src/commandsAndMenu.tsx:925 src/commandsAndMenu.tsx:993
 msgid "Stage"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1010 src/commandsAndMenu.tsx:1026 src/commandsAndMenu.tsx:1048 src/commandsAndMenu.tsx:1052 src/commandsAndMenu.tsx:1081 src/commandsAndMenu.tsx:1310 src/commandsAndMenu.tsx:1315 src/commandsAndMenu.tsx:683 src/commandsAndMenu.tsx:685 src/commandsAndMenu.tsx:691 src/commandsAndMenu.tsx:696 src/commandsAndMenu.tsx:716 src/commandsAndMenu.tsx:717 src/commandsAndMenu.tsx:818 src/commandsAndMenu.tsx:882 src/commandsAndMenu.tsx:941 src/commandsAndMenu.tsx:942
+#: src/commandsAndMenu.tsx:1010 src/commandsAndMenu.tsx:1026 src/commandsAndMenu.tsx:1048 src/commandsAndMenu.tsx:1052 src/commandsAndMenu.tsx:1081 src/commandsAndMenu.tsx:1310 src/commandsAndMenu.tsx:1315 src/commandsAndMenu.tsx:1498 src/commandsAndMenu.tsx:683 src/commandsAndMenu.tsx:685 src/commandsAndMenu.tsx:691 src/commandsAndMenu.tsx:696 src/commandsAndMenu.tsx:716 src/commandsAndMenu.tsx:717 src/commandsAndMenu.tsx:818 src/commandsAndMenu.tsx:882 src/commandsAndMenu.tsx:941 src/commandsAndMenu.tsx:942
 msgid "Start tracking selected file"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1011 src/commandsAndMenu.tsx:1016 src/commandsAndMenu.tsx:513 src/commandsAndMenu.tsx:515 src/commandsAndMenu.tsx:520 src/commandsAndMenu.tsx:524 src/commandsAndMenu.tsx:525 src/commandsAndMenu.tsx:581 src/commandsAndMenu.tsx:645 src/commandsAndMenu.tsx:704 src/commandsAndMenu.tsx:705 src/commandsAndMenu.tsx:724 src/commandsAndMenu.tsx:740 src/commandsAndMenu.tsx:762 src/commandsAndMenu.tsx:766 src/commandsAndMenu.tsx:787
+#: src/commandsAndMenu.tsx:1011 src/commandsAndMenu.tsx:1016 src/commandsAndMenu.tsx:1192 src/commandsAndMenu.tsx:513 src/commandsAndMenu.tsx:515 src/commandsAndMenu.tsx:520 src/commandsAndMenu.tsx:524 src/commandsAndMenu.tsx:525 src/commandsAndMenu.tsx:581 src/commandsAndMenu.tsx:645 src/commandsAndMenu.tsx:704 src/commandsAndMenu.tsx:705 src/commandsAndMenu.tsx:724 src/commandsAndMenu.tsx:740 src/commandsAndMenu.tsx:762 src/commandsAndMenu.tsx:766 src/commandsAndMenu.tsx:787
 msgid "Open selected file"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1011 src/commandsAndMenu.tsx:1027 src/commandsAndMenu.tsx:1049 src/commandsAndMenu.tsx:1053 src/commandsAndMenu.tsx:1082 src/commandsAndMenu.tsx:1311 src/commandsAndMenu.tsx:1316 src/commandsAndMenu.tsx:684 src/commandsAndMenu.tsx:686 src/commandsAndMenu.tsx:692 src/commandsAndMenu.tsx:697 src/commandsAndMenu.tsx:717 src/commandsAndMenu.tsx:718 src/commandsAndMenu.tsx:819 src/commandsAndMenu.tsx:883 src/commandsAndMenu.tsx:942 src/commandsAndMenu.tsx:943
+#: src/commandsAndMenu.tsx:1011 src/commandsAndMenu.tsx:1027 src/commandsAndMenu.tsx:1049 src/commandsAndMenu.tsx:1053 src/commandsAndMenu.tsx:1082 src/commandsAndMenu.tsx:1311 src/commandsAndMenu.tsx:1316 src/commandsAndMenu.tsx:1499 src/commandsAndMenu.tsx:684 src/commandsAndMenu.tsx:686 src/commandsAndMenu.tsx:692 src/commandsAndMenu.tsx:697 src/commandsAndMenu.tsx:717 src/commandsAndMenu.tsx:718 src/commandsAndMenu.tsx:819 src/commandsAndMenu.tsx:883 src/commandsAndMenu.tsx:942 src/commandsAndMenu.tsx:943
 msgid "Start tracking selected files"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1011 src/commandsAndMenu.tsx:1033 src/commandsAndMenu.tsx:1037 src/commandsAndMenu.tsx:1066 src/commandsAndMenu.tsx:1295 src/commandsAndMenu.tsx:1300 src/commandsAndMenu.tsx:668 src/commandsAndMenu.tsx:670 src/commandsAndMenu.tsx:676 src/commandsAndMenu.tsx:681 src/commandsAndMenu.tsx:701 src/commandsAndMenu.tsx:702 src/commandsAndMenu.tsx:803 src/commandsAndMenu.tsx:867 src/commandsAndMenu.tsx:926 src/commandsAndMenu.tsx:927 src/commandsAndMenu.tsx:995
+#: src/commandsAndMenu.tsx:1011 src/commandsAndMenu.tsx:1033 src/commandsAndMenu.tsx:1037 src/commandsAndMenu.tsx:1066 src/commandsAndMenu.tsx:1295 src/commandsAndMenu.tsx:1300 src/commandsAndMenu.tsx:1483 src/commandsAndMenu.tsx:668 src/commandsAndMenu.tsx:670 src/commandsAndMenu.tsx:676 src/commandsAndMenu.tsx:681 src/commandsAndMenu.tsx:701 src/commandsAndMenu.tsx:702 src/commandsAndMenu.tsx:803 src/commandsAndMenu.tsx:867 src/commandsAndMenu.tsx:926 src/commandsAndMenu.tsx:927 src/commandsAndMenu.tsx:995
 msgid "Stage the changes of selected file"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1012 src/commandsAndMenu.tsx:1013 src/commandsAndMenu.tsx:1081 src/commandsAndMenu.tsx:1097 src/commandsAndMenu.tsx:1119 src/commandsAndMenu.tsx:1123 src/commandsAndMenu.tsx:1152 src/commandsAndMenu.tsx:1381 src/commandsAndMenu.tsx:1386 src/commandsAndMenu.tsx:754 src/commandsAndMenu.tsx:756 src/commandsAndMenu.tsx:762 src/commandsAndMenu.tsx:767 src/commandsAndMenu.tsx:787 src/commandsAndMenu.tsx:788 src/commandsAndMenu.tsx:889 src/commandsAndMenu.tsx:953
+#: src/commandsAndMenu.tsx:1012 src/commandsAndMenu.tsx:1013 src/commandsAndMenu.tsx:1081 src/commandsAndMenu.tsx:1097 src/commandsAndMenu.tsx:1119 src/commandsAndMenu.tsx:1123 src/commandsAndMenu.tsx:1152 src/commandsAndMenu.tsx:1381 src/commandsAndMenu.tsx:1386 src/commandsAndMenu.tsx:1569 src/commandsAndMenu.tsx:754 src/commandsAndMenu.tsx:756 src/commandsAndMenu.tsx:762 src/commandsAndMenu.tsx:767 src/commandsAndMenu.tsx:787 src/commandsAndMenu.tsx:788 src/commandsAndMenu.tsx:889 src/commandsAndMenu.tsx:953
 msgid "Deleting %1 failed."
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1012 src/commandsAndMenu.tsx:1017 src/commandsAndMenu.tsx:514 src/commandsAndMenu.tsx:516 src/commandsAndMenu.tsx:521 src/commandsAndMenu.tsx:525 src/commandsAndMenu.tsx:526 src/commandsAndMenu.tsx:582 src/commandsAndMenu.tsx:646 src/commandsAndMenu.tsx:705 src/commandsAndMenu.tsx:706 src/commandsAndMenu.tsx:725 src/commandsAndMenu.tsx:741 src/commandsAndMenu.tsx:763 src/commandsAndMenu.tsx:767 src/commandsAndMenu.tsx:788
+#: src/commandsAndMenu.tsx:1012 src/commandsAndMenu.tsx:1017 src/commandsAndMenu.tsx:1193 src/commandsAndMenu.tsx:514 src/commandsAndMenu.tsx:516 src/commandsAndMenu.tsx:521 src/commandsAndMenu.tsx:525 src/commandsAndMenu.tsx:526 src/commandsAndMenu.tsx:582 src/commandsAndMenu.tsx:646 src/commandsAndMenu.tsx:705 src/commandsAndMenu.tsx:706 src/commandsAndMenu.tsx:725 src/commandsAndMenu.tsx:741 src/commandsAndMenu.tsx:763 src/commandsAndMenu.tsx:767 src/commandsAndMenu.tsx:788
 msgid "Open selected files"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1012 src/commandsAndMenu.tsx:1034 src/commandsAndMenu.tsx:1038 src/commandsAndMenu.tsx:1067 src/commandsAndMenu.tsx:1296 src/commandsAndMenu.tsx:1301 src/commandsAndMenu.tsx:669 src/commandsAndMenu.tsx:671 src/commandsAndMenu.tsx:677 src/commandsAndMenu.tsx:682 src/commandsAndMenu.tsx:702 src/commandsAndMenu.tsx:703 src/commandsAndMenu.tsx:804 src/commandsAndMenu.tsx:868 src/commandsAndMenu.tsx:927 src/commandsAndMenu.tsx:928 src/commandsAndMenu.tsx:996
+#: src/commandsAndMenu.tsx:1012 src/commandsAndMenu.tsx:1034 src/commandsAndMenu.tsx:1038 src/commandsAndMenu.tsx:1067 src/commandsAndMenu.tsx:1296 src/commandsAndMenu.tsx:1301 src/commandsAndMenu.tsx:1484 src/commandsAndMenu.tsx:669 src/commandsAndMenu.tsx:671 src/commandsAndMenu.tsx:677 src/commandsAndMenu.tsx:682 src/commandsAndMenu.tsx:702 src/commandsAndMenu.tsx:703 src/commandsAndMenu.tsx:804 src/commandsAndMenu.tsx:868 src/commandsAndMenu.tsx:927 src/commandsAndMenu.tsx:928 src/commandsAndMenu.tsx:996
 msgid "Stage the changes of selected files"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1016 src/commandsAndMenu.tsx:1020 src/commandsAndMenu.tsx:1049 src/commandsAndMenu.tsx:1278 src/commandsAndMenu.tsx:1283 src/commandsAndMenu.tsx:651 src/commandsAndMenu.tsx:653 src/commandsAndMenu.tsx:659 src/commandsAndMenu.tsx:664 src/commandsAndMenu.tsx:684 src/commandsAndMenu.tsx:685 src/commandsAndMenu.tsx:786 src/commandsAndMenu.tsx:850 src/commandsAndMenu.tsx:909 src/commandsAndMenu.tsx:910 src/commandsAndMenu.tsx:978 src/commandsAndMenu.tsx:994 src/components/ManageRemoteDialogue.tsx:159
+#: src/commandsAndMenu.tsx:1016 src/commandsAndMenu.tsx:1020 src/commandsAndMenu.tsx:1049 src/commandsAndMenu.tsx:1278 src/commandsAndMenu.tsx:1283 src/commandsAndMenu.tsx:1466 src/commandsAndMenu.tsx:651 src/commandsAndMenu.tsx:653 src/commandsAndMenu.tsx:659 src/commandsAndMenu.tsx:664 src/commandsAndMenu.tsx:684 src/commandsAndMenu.tsx:685 src/commandsAndMenu.tsx:786 src/commandsAndMenu.tsx:850 src/commandsAndMenu.tsx:909 src/commandsAndMenu.tsx:910 src/commandsAndMenu.tsx:978 src/commandsAndMenu.tsx:994 src/components/ManageRemoteDialogue.tsx:159
 msgid "Add"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1018 src/commandsAndMenu.tsx:1022 src/commandsAndMenu.tsx:1051 src/commandsAndMenu.tsx:1280 src/commandsAndMenu.tsx:1285 src/commandsAndMenu.tsx:653 src/commandsAndMenu.tsx:655 src/commandsAndMenu.tsx:661 src/commandsAndMenu.tsx:666 src/commandsAndMenu.tsx:686 src/commandsAndMenu.tsx:687 src/commandsAndMenu.tsx:788 src/commandsAndMenu.tsx:852 src/commandsAndMenu.tsx:911 src/commandsAndMenu.tsx:912 src/commandsAndMenu.tsx:980 src/commandsAndMenu.tsx:996
+#: src/commandsAndMenu.tsx:1017 src/commandsAndMenu.tsx:846 src/commandsAndMenu.tsx:851
+msgid "Branch '%1' rebase onto '%2'."
+msgstr ""
+
+#: src/commandsAndMenu.tsx:1018 src/commandsAndMenu.tsx:1022 src/commandsAndMenu.tsx:1051 src/commandsAndMenu.tsx:1280 src/commandsAndMenu.tsx:1285 src/commandsAndMenu.tsx:1468 src/commandsAndMenu.tsx:653 src/commandsAndMenu.tsx:655 src/commandsAndMenu.tsx:661 src/commandsAndMenu.tsx:666 src/commandsAndMenu.tsx:686 src/commandsAndMenu.tsx:687 src/commandsAndMenu.tsx:788 src/commandsAndMenu.tsx:852 src/commandsAndMenu.tsx:911 src/commandsAndMenu.tsx:912 src/commandsAndMenu.tsx:980 src/commandsAndMenu.tsx:996
 msgid "Stage or track the changes to selected file"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1019 src/commandsAndMenu.tsx:1023 src/commandsAndMenu.tsx:1052 src/commandsAndMenu.tsx:1281 src/commandsAndMenu.tsx:1286 src/commandsAndMenu.tsx:654 src/commandsAndMenu.tsx:656 src/commandsAndMenu.tsx:662 src/commandsAndMenu.tsx:667 src/commandsAndMenu.tsx:687 src/commandsAndMenu.tsx:688 src/commandsAndMenu.tsx:789 src/commandsAndMenu.tsx:853 src/commandsAndMenu.tsx:912 src/commandsAndMenu.tsx:913 src/commandsAndMenu.tsx:981 src/commandsAndMenu.tsx:997
+#: src/commandsAndMenu.tsx:1019 src/commandsAndMenu.tsx:1023 src/commandsAndMenu.tsx:1052 src/commandsAndMenu.tsx:1281 src/commandsAndMenu.tsx:1286 src/commandsAndMenu.tsx:1469 src/commandsAndMenu.tsx:654 src/commandsAndMenu.tsx:656 src/commandsAndMenu.tsx:662 src/commandsAndMenu.tsx:667 src/commandsAndMenu.tsx:687 src/commandsAndMenu.tsx:688 src/commandsAndMenu.tsx:789 src/commandsAndMenu.tsx:853 src/commandsAndMenu.tsx:912 src/commandsAndMenu.tsx:913 src/commandsAndMenu.tsx:981 src/commandsAndMenu.tsx:997
 msgid "Stage or track the changes of selected files"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1020 src/commandsAndMenu.tsx:1024 src/commandsAndMenu.tsx:1079 src/commandsAndMenu.tsx:1080 src/commandsAndMenu.tsx:1083 src/commandsAndMenu.tsx:1084 src/commandsAndMenu.tsx:1148 src/commandsAndMenu.tsx:1152 src/commandsAndMenu.tsx:1164 src/commandsAndMenu.tsx:1168 src/commandsAndMenu.tsx:1186 src/commandsAndMenu.tsx:1190 src/commandsAndMenu.tsx:1194 src/commandsAndMenu.tsx:1219 src/commandsAndMenu.tsx:1223 src/commandsAndMenu.tsx:1448 src/commandsAndMenu.tsx:1452 src/commandsAndMenu.tsx:1453 src/commandsAndMenu.tsx:1457 src/commandsAndMenu.tsx:821 src/commandsAndMenu.tsx:823 src/commandsAndMenu.tsx:825 src/commandsAndMenu.tsx:827 src/commandsAndMenu.tsx:829 src/commandsAndMenu.tsx:833 src/commandsAndMenu.tsx:834 src/commandsAndMenu.tsx:838 src/commandsAndMenu.tsx:854 src/commandsAndMenu.tsx:855 src/commandsAndMenu.tsx:858 src/commandsAndMenu.tsx:859 src/commandsAndMenu.tsx:956 src/commandsAndMenu.tsx:960
+#: src/commandsAndMenu.tsx:1020 src/commandsAndMenu.tsx:1024 src/commandsAndMenu.tsx:1079 src/commandsAndMenu.tsx:1080 src/commandsAndMenu.tsx:1083 src/commandsAndMenu.tsx:1084 src/commandsAndMenu.tsx:1148 src/commandsAndMenu.tsx:1152 src/commandsAndMenu.tsx:1164 src/commandsAndMenu.tsx:1168 src/commandsAndMenu.tsx:1186 src/commandsAndMenu.tsx:1190 src/commandsAndMenu.tsx:1194 src/commandsAndMenu.tsx:1219 src/commandsAndMenu.tsx:1223 src/commandsAndMenu.tsx:1448 src/commandsAndMenu.tsx:1452 src/commandsAndMenu.tsx:1453 src/commandsAndMenu.tsx:1457 src/commandsAndMenu.tsx:1636 src/commandsAndMenu.tsx:1640 src/commandsAndMenu.tsx:821 src/commandsAndMenu.tsx:823 src/commandsAndMenu.tsx:825 src/commandsAndMenu.tsx:827 src/commandsAndMenu.tsx:829 src/commandsAndMenu.tsx:833 src/commandsAndMenu.tsx:834 src/commandsAndMenu.tsx:838 src/commandsAndMenu.tsx:854 src/commandsAndMenu.tsx:855 src/commandsAndMenu.tsx:858 src/commandsAndMenu.tsx:859 src/commandsAndMenu.tsx:956 src/commandsAndMenu.tsx:960
 msgid "Ignore this file (add to .gitignore)"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1020 src/commandsAndMenu.tsx:1025 src/commandsAndMenu.tsx:522 src/commandsAndMenu.tsx:524 src/commandsAndMenu.tsx:529 src/commandsAndMenu.tsx:533 src/commandsAndMenu.tsx:534 src/commandsAndMenu.tsx:590 src/commandsAndMenu.tsx:654 src/commandsAndMenu.tsx:713 src/commandsAndMenu.tsx:714 src/commandsAndMenu.tsx:733 src/commandsAndMenu.tsx:749 src/commandsAndMenu.tsx:771 src/commandsAndMenu.tsx:775 src/commandsAndMenu.tsx:796
+#: src/commandsAndMenu.tsx:1020 src/commandsAndMenu.tsx:1025 src/commandsAndMenu.tsx:1201 src/commandsAndMenu.tsx:522 src/commandsAndMenu.tsx:524 src/commandsAndMenu.tsx:529 src/commandsAndMenu.tsx:533 src/commandsAndMenu.tsx:534 src/commandsAndMenu.tsx:590 src/commandsAndMenu.tsx:654 src/commandsAndMenu.tsx:713 src/commandsAndMenu.tsx:714 src/commandsAndMenu.tsx:733 src/commandsAndMenu.tsx:749 src/commandsAndMenu.tsx:771 src/commandsAndMenu.tsx:775 src/commandsAndMenu.tsx:796
 msgid "Open File Failed"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1021 src/commandsAndMenu.tsx:1025 src/commandsAndMenu.tsx:1080 src/commandsAndMenu.tsx:1081 src/commandsAndMenu.tsx:1084 src/commandsAndMenu.tsx:1085 src/commandsAndMenu.tsx:1149 src/commandsAndMenu.tsx:1153 src/commandsAndMenu.tsx:1165 src/commandsAndMenu.tsx:1169 src/commandsAndMenu.tsx:1187 src/commandsAndMenu.tsx:1191 src/commandsAndMenu.tsx:1195 src/commandsAndMenu.tsx:1220 src/commandsAndMenu.tsx:1224 src/commandsAndMenu.tsx:1449 src/commandsAndMenu.tsx:1453 src/commandsAndMenu.tsx:1454 src/commandsAndMenu.tsx:1458 src/commandsAndMenu.tsx:822 src/commandsAndMenu.tsx:824 src/commandsAndMenu.tsx:826 src/commandsAndMenu.tsx:828 src/commandsAndMenu.tsx:830 src/commandsAndMenu.tsx:834 src/commandsAndMenu.tsx:835 src/commandsAndMenu.tsx:839 src/commandsAndMenu.tsx:855 src/commandsAndMenu.tsx:856 src/commandsAndMenu.tsx:859 src/commandsAndMenu.tsx:860 src/commandsAndMenu.tsx:957 src/commandsAndMenu.tsx:961
+#: src/commandsAndMenu.tsx:1021 src/commandsAndMenu.tsx:1025 src/commandsAndMenu.tsx:1080 src/commandsAndMenu.tsx:1081 src/commandsAndMenu.tsx:1084 src/commandsAndMenu.tsx:1085 src/commandsAndMenu.tsx:1149 src/commandsAndMenu.tsx:1153 src/commandsAndMenu.tsx:1165 src/commandsAndMenu.tsx:1169 src/commandsAndMenu.tsx:1187 src/commandsAndMenu.tsx:1191 src/commandsAndMenu.tsx:1195 src/commandsAndMenu.tsx:1220 src/commandsAndMenu.tsx:1224 src/commandsAndMenu.tsx:1449 src/commandsAndMenu.tsx:1453 src/commandsAndMenu.tsx:1454 src/commandsAndMenu.tsx:1458 src/commandsAndMenu.tsx:1637 src/commandsAndMenu.tsx:1641 src/commandsAndMenu.tsx:822 src/commandsAndMenu.tsx:824 src/commandsAndMenu.tsx:826 src/commandsAndMenu.tsx:828 src/commandsAndMenu.tsx:830 src/commandsAndMenu.tsx:834 src/commandsAndMenu.tsx:835 src/commandsAndMenu.tsx:839 src/commandsAndMenu.tsx:855 src/commandsAndMenu.tsx:856 src/commandsAndMenu.tsx:859 src/commandsAndMenu.tsx:860 src/commandsAndMenu.tsx:957 src/commandsAndMenu.tsx:961
 msgid "Ignore these files (add to .gitignore)"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1021 src/commandsAndMenu.tsx:1026 src/commandsAndMenu.tsx:523 src/commandsAndMenu.tsx:525 src/commandsAndMenu.tsx:530 src/commandsAndMenu.tsx:534 src/commandsAndMenu.tsx:535 src/commandsAndMenu.tsx:591 src/commandsAndMenu.tsx:655 src/commandsAndMenu.tsx:714 src/commandsAndMenu.tsx:715 src/commandsAndMenu.tsx:734 src/commandsAndMenu.tsx:750 src/commandsAndMenu.tsx:772 src/commandsAndMenu.tsx:776 src/commandsAndMenu.tsx:797
+#: src/commandsAndMenu.tsx:1021 src/commandsAndMenu.tsx:1026 src/commandsAndMenu.tsx:1202 src/commandsAndMenu.tsx:523 src/commandsAndMenu.tsx:525 src/commandsAndMenu.tsx:530 src/commandsAndMenu.tsx:534 src/commandsAndMenu.tsx:535 src/commandsAndMenu.tsx:591 src/commandsAndMenu.tsx:655 src/commandsAndMenu.tsx:714 src/commandsAndMenu.tsx:715 src/commandsAndMenu.tsx:734 src/commandsAndMenu.tsx:750 src/commandsAndMenu.tsx:772 src/commandsAndMenu.tsx:776 src/commandsAndMenu.tsx:797
 msgid "This file has been deleted!"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1023 src/commandsAndMenu.tsx:1024 src/commandsAndMenu.tsx:1045 src/commandsAndMenu.tsx:1046 src/commandsAndMenu.tsx:1092 src/commandsAndMenu.tsx:1108 src/commandsAndMenu.tsx:1114 src/commandsAndMenu.tsx:1130 src/commandsAndMenu.tsx:1134 src/commandsAndMenu.tsx:1152 src/commandsAndMenu.tsx:1156 src/commandsAndMenu.tsx:1163 src/commandsAndMenu.tsx:1185 src/commandsAndMenu.tsx:1392 src/commandsAndMenu.tsx:1397 src/commandsAndMenu.tsx:1414 src/commandsAndMenu.tsx:1419 src/commandsAndMenu.tsx:765 src/commandsAndMenu.tsx:767 src/commandsAndMenu.tsx:773 src/commandsAndMenu.tsx:778 src/commandsAndMenu.tsx:787 src/commandsAndMenu.tsx:789 src/commandsAndMenu.tsx:795 src/commandsAndMenu.tsx:798 src/commandsAndMenu.tsx:799 src/commandsAndMenu.tsx:800 src/commandsAndMenu.tsx:820 src/commandsAndMenu.tsx:821 src/commandsAndMenu.tsx:900 src/commandsAndMenu.tsx:922 src/commandsAndMenu.tsx:964 src/commandsAndMenu.tsx:986 src/components/FileList.tsx:183 src/components/FileList.tsx:192 src/components/FileList.tsx:194 src/components/FileList.tsx:197 src/components/FileList.tsx:208 src/components/FileList.tsx:217 src/components/FileList.tsx:219 src/components/FileList.tsx:258 src/components/FileList.tsx:268 src/widgets/discardAllChanges.ts:26
+#: src/commandsAndMenu.tsx:1023 src/commandsAndMenu.tsx:1024 src/commandsAndMenu.tsx:1045 src/commandsAndMenu.tsx:1046 src/commandsAndMenu.tsx:1092 src/commandsAndMenu.tsx:1108 src/commandsAndMenu.tsx:1114 src/commandsAndMenu.tsx:1130 src/commandsAndMenu.tsx:1134 src/commandsAndMenu.tsx:1152 src/commandsAndMenu.tsx:1156 src/commandsAndMenu.tsx:1163 src/commandsAndMenu.tsx:1185 src/commandsAndMenu.tsx:1392 src/commandsAndMenu.tsx:1397 src/commandsAndMenu.tsx:1414 src/commandsAndMenu.tsx:1419 src/commandsAndMenu.tsx:1580 src/commandsAndMenu.tsx:1602 src/commandsAndMenu.tsx:765 src/commandsAndMenu.tsx:767 src/commandsAndMenu.tsx:773 src/commandsAndMenu.tsx:778 src/commandsAndMenu.tsx:787 src/commandsAndMenu.tsx:789 src/commandsAndMenu.tsx:795 src/commandsAndMenu.tsx:798 src/commandsAndMenu.tsx:799 src/commandsAndMenu.tsx:800 src/commandsAndMenu.tsx:820 src/commandsAndMenu.tsx:821 src/commandsAndMenu.tsx:900 src/commandsAndMenu.tsx:922 src/commandsAndMenu.tsx:964 src/commandsAndMenu.tsx:986 src/components/FileList.tsx:183 src/components/FileList.tsx:192 src/components/FileList.tsx:194 src/components/FileList.tsx:197 src/components/FileList.tsx:208 src/components/FileList.tsx:217 src/components/FileList.tsx:219 src/components/FileList.tsx:258 src/components/FileList.tsx:268 src/components/FileList.tsx:269 src/widgets/discardAllChanges.ts:26
 msgid "Discard"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1023 src/commandsAndMenu.tsx:1039 src/commandsAndMenu.tsx:1061 src/commandsAndMenu.tsx:1065 src/commandsAndMenu.tsx:1094 src/commandsAndMenu.tsx:1323 src/commandsAndMenu.tsx:1328 src/commandsAndMenu.tsx:696 src/commandsAndMenu.tsx:698 src/commandsAndMenu.tsx:704 src/commandsAndMenu.tsx:709 src/commandsAndMenu.tsx:729 src/commandsAndMenu.tsx:730 src/commandsAndMenu.tsx:831 src/commandsAndMenu.tsx:895 src/commandsAndMenu.tsx:954 src/commandsAndMenu.tsx:955
+#: src/commandsAndMenu.tsx:1023 src/commandsAndMenu.tsx:1039 src/commandsAndMenu.tsx:1061 src/commandsAndMenu.tsx:1065 src/commandsAndMenu.tsx:1094 src/commandsAndMenu.tsx:1323 src/commandsAndMenu.tsx:1328 src/commandsAndMenu.tsx:1511 src/commandsAndMenu.tsx:696 src/commandsAndMenu.tsx:698 src/commandsAndMenu.tsx:704 src/commandsAndMenu.tsx:709 src/commandsAndMenu.tsx:729 src/commandsAndMenu.tsx:730 src/commandsAndMenu.tsx:831 src/commandsAndMenu.tsx:895 src/commandsAndMenu.tsx:954 src/commandsAndMenu.tsx:955
 msgid "Unstage"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1024 src/commandsAndMenu.tsx:1088 src/commandsAndMenu.tsx:1148 src/commandsAndMenu.tsx:1149 src/commandsAndMenu.tsx:1217 src/commandsAndMenu.tsx:1233 src/commandsAndMenu.tsx:1255 src/commandsAndMenu.tsx:1259 src/commandsAndMenu.tsx:1288 src/commandsAndMenu.tsx:1517 src/commandsAndMenu.tsx:1522 src/commandsAndMenu.tsx:902 src/commandsAndMenu.tsx:922 src/commandsAndMenu.tsx:923 src/components/GitPanel.tsx:344 src/components/GitPanel.tsx:358 src/components/GitPanel.tsx:363 src/components/GitPanel.tsx:370 src/components/GitPanel.tsx:383 src/components/GitPanel.tsx:391 src/components/GitPanel.tsx:414 src/components/GitPanel.tsx:415 src/components/GitPanel.tsx:449 src/components/GitPanel.tsx:468
+#: src/commandsAndMenu.tsx:1024 src/commandsAndMenu.tsx:1088 src/commandsAndMenu.tsx:1148 src/commandsAndMenu.tsx:1149 src/commandsAndMenu.tsx:1217 src/commandsAndMenu.tsx:1233 src/commandsAndMenu.tsx:1255 src/commandsAndMenu.tsx:1259 src/commandsAndMenu.tsx:1288 src/commandsAndMenu.tsx:1517 src/commandsAndMenu.tsx:1522 src/commandsAndMenu.tsx:1714 src/commandsAndMenu.tsx:902 src/commandsAndMenu.tsx:922 src/commandsAndMenu.tsx:923 src/components/GitPanel.tsx:344 src/components/GitPanel.tsx:358 src/components/GitPanel.tsx:363 src/components/GitPanel.tsx:370 src/components/GitPanel.tsx:383 src/components/GitPanel.tsx:391 src/components/GitPanel.tsx:414 src/components/GitPanel.tsx:415 src/components/GitPanel.tsx:449 src/components/GitPanel.tsx:462 src/components/GitPanel.tsx:468
 msgid "History"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1025 src/commandsAndMenu.tsx:1026 src/commandsAndMenu.tsx:1094 src/commandsAndMenu.tsx:1110 src/commandsAndMenu.tsx:1132 src/commandsAndMenu.tsx:1136 src/commandsAndMenu.tsx:1165 src/commandsAndMenu.tsx:1394 src/commandsAndMenu.tsx:1399 src/commandsAndMenu.tsx:767 src/commandsAndMenu.tsx:769 src/commandsAndMenu.tsx:775 src/commandsAndMenu.tsx:780 src/commandsAndMenu.tsx:800 src/commandsAndMenu.tsx:801 src/commandsAndMenu.tsx:902 src/commandsAndMenu.tsx:966
+#: src/commandsAndMenu.tsx:1025 src/commandsAndMenu.tsx:1026 src/commandsAndMenu.tsx:1094 src/commandsAndMenu.tsx:1110 src/commandsAndMenu.tsx:1132 src/commandsAndMenu.tsx:1136 src/commandsAndMenu.tsx:1165 src/commandsAndMenu.tsx:1394 src/commandsAndMenu.tsx:1399 src/commandsAndMenu.tsx:1582 src/commandsAndMenu.tsx:767 src/commandsAndMenu.tsx:769 src/commandsAndMenu.tsx:775 src/commandsAndMenu.tsx:780 src/commandsAndMenu.tsx:800 src/commandsAndMenu.tsx:801 src/commandsAndMenu.tsx:902 src/commandsAndMenu.tsx:966
 msgid "Discard recent changes of selected file"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1025 src/commandsAndMenu.tsx:1041 src/commandsAndMenu.tsx:1063 src/commandsAndMenu.tsx:1067 src/commandsAndMenu.tsx:1096 src/commandsAndMenu.tsx:1325 src/commandsAndMenu.tsx:1330 src/commandsAndMenu.tsx:698 src/commandsAndMenu.tsx:700 src/commandsAndMenu.tsx:706 src/commandsAndMenu.tsx:711 src/commandsAndMenu.tsx:731 src/commandsAndMenu.tsx:732 src/commandsAndMenu.tsx:833 src/commandsAndMenu.tsx:897 src/commandsAndMenu.tsx:956 src/commandsAndMenu.tsx:957
+#: src/commandsAndMenu.tsx:1025 src/commandsAndMenu.tsx:1041 src/commandsAndMenu.tsx:1063 src/commandsAndMenu.tsx:1067 src/commandsAndMenu.tsx:1096 src/commandsAndMenu.tsx:1325 src/commandsAndMenu.tsx:1330 src/commandsAndMenu.tsx:1513 src/commandsAndMenu.tsx:698 src/commandsAndMenu.tsx:700 src/commandsAndMenu.tsx:706 src/commandsAndMenu.tsx:711 src/commandsAndMenu.tsx:731 src/commandsAndMenu.tsx:732 src/commandsAndMenu.tsx:833 src/commandsAndMenu.tsx:897 src/commandsAndMenu.tsx:956 src/commandsAndMenu.tsx:957
 msgid "Unstage the changes of selected file"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1025 src/commandsAndMenu.tsx:1089 src/commandsAndMenu.tsx:1149 src/commandsAndMenu.tsx:1150 src/commandsAndMenu.tsx:1218 src/commandsAndMenu.tsx:1234 src/commandsAndMenu.tsx:1256 src/commandsAndMenu.tsx:1260 src/commandsAndMenu.tsx:1289 src/commandsAndMenu.tsx:1518 src/commandsAndMenu.tsx:1523 src/commandsAndMenu.tsx:903 src/commandsAndMenu.tsx:923 src/commandsAndMenu.tsx:924
+#: src/commandsAndMenu.tsx:1025 src/commandsAndMenu.tsx:1089 src/commandsAndMenu.tsx:1149 src/commandsAndMenu.tsx:1150 src/commandsAndMenu.tsx:1218 src/commandsAndMenu.tsx:1234 src/commandsAndMenu.tsx:1256 src/commandsAndMenu.tsx:1260 src/commandsAndMenu.tsx:1289 src/commandsAndMenu.tsx:1518 src/commandsAndMenu.tsx:1523 src/commandsAndMenu.tsx:1715 src/commandsAndMenu.tsx:903 src/commandsAndMenu.tsx:923 src/commandsAndMenu.tsx:924
 msgid "View the history of this file"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1026 src/commandsAndMenu.tsx:1027 src/commandsAndMenu.tsx:1095 src/commandsAndMenu.tsx:1111 src/commandsAndMenu.tsx:1133 src/commandsAndMenu.tsx:1137 src/commandsAndMenu.tsx:1166 src/commandsAndMenu.tsx:1395 src/commandsAndMenu.tsx:1400 src/commandsAndMenu.tsx:768 src/commandsAndMenu.tsx:770 src/commandsAndMenu.tsx:776 src/commandsAndMenu.tsx:781 src/commandsAndMenu.tsx:801 src/commandsAndMenu.tsx:802 src/commandsAndMenu.tsx:903 src/commandsAndMenu.tsx:967
+#: src/commandsAndMenu.tsx:1026 src/commandsAndMenu.tsx:1027 src/commandsAndMenu.tsx:1095 src/commandsAndMenu.tsx:1111 src/commandsAndMenu.tsx:1133 src/commandsAndMenu.tsx:1137 src/commandsAndMenu.tsx:1166 src/commandsAndMenu.tsx:1395 src/commandsAndMenu.tsx:1400 src/commandsAndMenu.tsx:1583 src/commandsAndMenu.tsx:768 src/commandsAndMenu.tsx:770 src/commandsAndMenu.tsx:776 src/commandsAndMenu.tsx:781 src/commandsAndMenu.tsx:801 src/commandsAndMenu.tsx:802 src/commandsAndMenu.tsx:903 src/commandsAndMenu.tsx:967
 msgid "Discard recent changes of selected files"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1026 src/commandsAndMenu.tsx:1042 src/commandsAndMenu.tsx:1064 src/commandsAndMenu.tsx:1068 src/commandsAndMenu.tsx:1097 src/commandsAndMenu.tsx:1326 src/commandsAndMenu.tsx:1331 src/commandsAndMenu.tsx:699 src/commandsAndMenu.tsx:701 src/commandsAndMenu.tsx:707 src/commandsAndMenu.tsx:712 src/commandsAndMenu.tsx:732 src/commandsAndMenu.tsx:733 src/commandsAndMenu.tsx:834 src/commandsAndMenu.tsx:898 src/commandsAndMenu.tsx:957 src/commandsAndMenu.tsx:958
+#: src/commandsAndMenu.tsx:1026 src/commandsAndMenu.tsx:1042 src/commandsAndMenu.tsx:1064 src/commandsAndMenu.tsx:1068 src/commandsAndMenu.tsx:1097 src/commandsAndMenu.tsx:1326 src/commandsAndMenu.tsx:1331 src/commandsAndMenu.tsx:1514 src/commandsAndMenu.tsx:699 src/commandsAndMenu.tsx:701 src/commandsAndMenu.tsx:707 src/commandsAndMenu.tsx:712 src/commandsAndMenu.tsx:732 src/commandsAndMenu.tsx:733 src/commandsAndMenu.tsx:834 src/commandsAndMenu.tsx:898 src/commandsAndMenu.tsx:957 src/commandsAndMenu.tsx:958
 msgid "Unstage the changes of selected files"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1033 src/commandsAndMenu.tsx:1034 src/commandsAndMenu.tsx:1102 src/commandsAndMenu.tsx:1118 src/commandsAndMenu.tsx:1140 src/commandsAndMenu.tsx:1144 src/commandsAndMenu.tsx:1173 src/commandsAndMenu.tsx:1402 src/commandsAndMenu.tsx:1407 src/commandsAndMenu.tsx:775 src/commandsAndMenu.tsx:777 src/commandsAndMenu.tsx:783 src/commandsAndMenu.tsx:788 src/commandsAndMenu.tsx:808 src/commandsAndMenu.tsx:809 src/commandsAndMenu.tsx:910 src/commandsAndMenu.tsx:974 src/components/FileList.tsx:1125 src/components/FileList.tsx:1129 src/components/FileList.tsx:1151 src/components/FileList.tsx:1155 src/components/FileList.tsx:457 src/components/FileList.tsx:466 src/components/FileList.tsx:534 src/components/FileList.tsx:535 src/components/FileList.tsx:655 src/components/FileList.tsx:664 src/components/FileList.tsx:681 src/components/FileList.tsx:690 src/components/FileList.tsx:733 src/components/FileList.tsx:759 src/components/FileList.tsx:810 src/components/FileList.tsx:835 src/components/FileList.tsx:836 src/components/FileList.tsx:837
+#: src/commandsAndMenu.tsx:1033 src/commandsAndMenu.tsx:1034 src/commandsAndMenu.tsx:1102 src/commandsAndMenu.tsx:1118 src/commandsAndMenu.tsx:1140 src/commandsAndMenu.tsx:1144 src/commandsAndMenu.tsx:1173 src/commandsAndMenu.tsx:1402 src/commandsAndMenu.tsx:1407 src/commandsAndMenu.tsx:1590 src/commandsAndMenu.tsx:775 src/commandsAndMenu.tsx:777 src/commandsAndMenu.tsx:783 src/commandsAndMenu.tsx:788 src/commandsAndMenu.tsx:808 src/commandsAndMenu.tsx:809 src/commandsAndMenu.tsx:910 src/commandsAndMenu.tsx:974 src/components/FileList.tsx:1125 src/components/FileList.tsx:1129 src/components/FileList.tsx:1151 src/components/FileList.tsx:1153 src/components/FileList.tsx:1155 src/components/FileList.tsx:1179 src/components/FileList.tsx:457 src/components/FileList.tsx:466 src/components/FileList.tsx:534 src/components/FileList.tsx:535 src/components/FileList.tsx:655 src/components/FileList.tsx:664 src/components/FileList.tsx:681 src/components/FileList.tsx:690 src/components/FileList.tsx:733 src/components/FileList.tsx:759 src/components/FileList.tsx:810 src/components/FileList.tsx:835 src/components/FileList.tsx:836 src/components/FileList.tsx:837 src/components/FileList.tsx:859
 msgid "Discard changes"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1036 src/commandsAndMenu.tsx:1037 src/commandsAndMenu.tsx:1105 src/commandsAndMenu.tsx:1121 src/commandsAndMenu.tsx:1143 src/commandsAndMenu.tsx:1147 src/commandsAndMenu.tsx:1176 src/commandsAndMenu.tsx:1405 src/commandsAndMenu.tsx:1410 src/commandsAndMenu.tsx:778 src/commandsAndMenu.tsx:780 src/commandsAndMenu.tsx:786 src/commandsAndMenu.tsx:791 src/commandsAndMenu.tsx:811 src/commandsAndMenu.tsx:812 src/commandsAndMenu.tsx:913 src/commandsAndMenu.tsx:977
+#: src/commandsAndMenu.tsx:1035 src/commandsAndMenu.tsx:864 src/commandsAndMenu.tsx:869
+msgid "Continue rebase"
+msgstr ""
+
+#: src/commandsAndMenu.tsx:1036 src/commandsAndMenu.tsx:1037 src/commandsAndMenu.tsx:1105 src/commandsAndMenu.tsx:1121 src/commandsAndMenu.tsx:1143 src/commandsAndMenu.tsx:1147 src/commandsAndMenu.tsx:1176 src/commandsAndMenu.tsx:1405 src/commandsAndMenu.tsx:1410 src/commandsAndMenu.tsx:1593 src/commandsAndMenu.tsx:778 src/commandsAndMenu.tsx:780 src/commandsAndMenu.tsx:786 src/commandsAndMenu.tsx:791 src/commandsAndMenu.tsx:811 src/commandsAndMenu.tsx:812 src/commandsAndMenu.tsx:913 src/commandsAndMenu.tsx:977
 msgid "Are you sure you want to permanently discard changes to the following files?               This action cannot be undone."
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1042 src/commandsAndMenu.tsx:1047 src/commandsAndMenu.tsx:755 src/commandsAndMenu.tsx:771 src/commandsAndMenu.tsx:793 src/commandsAndMenu.tsx:797 src/commandsAndMenu.tsx:818
+#: src/commandsAndMenu.tsx:1037 src/commandsAndMenu.tsx:866 src/commandsAndMenu.tsx:871
+msgid "Skip current commit"
+msgstr ""
+
+#: src/commandsAndMenu.tsx:1039 src/commandsAndMenu.tsx:868 src/commandsAndMenu.tsx:873 src/components/RebaseAction.tsx:72 src/components/RebaseAction.tsx:76
+msgid "Abort rebase"
+msgstr ""
+
+#: src/commandsAndMenu.tsx:1041 src/commandsAndMenu.tsx:1055 src/commandsAndMenu.tsx:870 src/commandsAndMenu.tsx:875 src/commandsAndMenu.tsx:884 src/commandsAndMenu.tsx:889
+msgid "Resolve rebase"
+msgstr ""
+
+#: src/commandsAndMenu.tsx:1042 src/commandsAndMenu.tsx:1047 src/commandsAndMenu.tsx:1223 src/commandsAndMenu.tsx:755 src/commandsAndMenu.tsx:771 src/commandsAndMenu.tsx:793 src/commandsAndMenu.tsx:797 src/commandsAndMenu.tsx:818
 msgid "Open File"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1043 src/commandsAndMenu.tsx:1048 src/commandsAndMenu.tsx:756 src/commandsAndMenu.tsx:772 src/commandsAndMenu.tsx:794 src/commandsAndMenu.tsx:798 src/commandsAndMenu.tsx:819
+#: src/commandsAndMenu.tsx:1043 src/commandsAndMenu.tsx:1048 src/commandsAndMenu.tsx:1224 src/commandsAndMenu.tsx:756 src/commandsAndMenu.tsx:772 src/commandsAndMenu.tsx:794 src/commandsAndMenu.tsx:798 src/commandsAndMenu.tsx:819
 msgid "Open file from its diff view"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1043 src/commandsAndMenu.tsx:1103 src/commandsAndMenu.tsx:1104 src/commandsAndMenu.tsx:1172 src/commandsAndMenu.tsx:1188 src/commandsAndMenu.tsx:1210 src/commandsAndMenu.tsx:1214 src/commandsAndMenu.tsx:1243 src/commandsAndMenu.tsx:1472 src/commandsAndMenu.tsx:1477 src/commandsAndMenu.tsx:844 src/commandsAndMenu.tsx:846 src/commandsAndMenu.tsx:852 src/commandsAndMenu.tsx:857 src/commandsAndMenu.tsx:877 src/commandsAndMenu.tsx:878 src/commandsAndMenu.tsx:979
+#: src/commandsAndMenu.tsx:1043 src/commandsAndMenu.tsx:1103 src/commandsAndMenu.tsx:1104 src/commandsAndMenu.tsx:1172 src/commandsAndMenu.tsx:1188 src/commandsAndMenu.tsx:1210 src/commandsAndMenu.tsx:1214 src/commandsAndMenu.tsx:1243 src/commandsAndMenu.tsx:1472 src/commandsAndMenu.tsx:1477 src/commandsAndMenu.tsx:1669 src/commandsAndMenu.tsx:844 src/commandsAndMenu.tsx:846 src/commandsAndMenu.tsx:852 src/commandsAndMenu.tsx:857 src/commandsAndMenu.tsx:877 src/commandsAndMenu.tsx:878 src/commandsAndMenu.tsx:979
 msgid "Ignore %2 extension (add to .gitignore)"
 msgid_plural "Ignore %2 extensions (add to .gitignore)"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 
-#: src/commandsAndMenu.tsx:1043 src/commandsAndMenu.tsx:1107 src/commandsAndMenu.tsx:1167 src/commandsAndMenu.tsx:1168 src/commandsAndMenu.tsx:1236 src/commandsAndMenu.tsx:1252 src/commandsAndMenu.tsx:1274 src/commandsAndMenu.tsx:1278 src/commandsAndMenu.tsx:1307 src/commandsAndMenu.tsx:1536 src/commandsAndMenu.tsx:1541 src/commandsAndMenu.tsx:889 src/commandsAndMenu.tsx:891 src/commandsAndMenu.tsx:897 src/commandsAndMenu.tsx:921 src/commandsAndMenu.tsx:941 src/commandsAndMenu.tsx:942
+#: src/commandsAndMenu.tsx:1043 src/commandsAndMenu.tsx:1107 src/commandsAndMenu.tsx:1167 src/commandsAndMenu.tsx:1168 src/commandsAndMenu.tsx:1236 src/commandsAndMenu.tsx:1252 src/commandsAndMenu.tsx:1274 src/commandsAndMenu.tsx:1278 src/commandsAndMenu.tsx:1307 src/commandsAndMenu.tsx:1536 src/commandsAndMenu.tsx:1541 src/commandsAndMenu.tsx:1733 src/commandsAndMenu.tsx:889 src/commandsAndMenu.tsx:891 src/commandsAndMenu.tsx:897 src/commandsAndMenu.tsx:921 src/commandsAndMenu.tsx:941 src/commandsAndMenu.tsx:942
 msgid "No actions available"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1051 src/commandsAndMenu.tsx:1067 src/commandsAndMenu.tsx:1089 src/commandsAndMenu.tsx:1093 src/commandsAndMenu.tsx:1122 src/commandsAndMenu.tsx:1351 src/commandsAndMenu.tsx:1356 src/commandsAndMenu.tsx:724 src/commandsAndMenu.tsx:726 src/commandsAndMenu.tsx:732 src/commandsAndMenu.tsx:737 src/commandsAndMenu.tsx:757 src/commandsAndMenu.tsx:758 src/commandsAndMenu.tsx:859 src/commandsAndMenu.tsx:923 src/commandsAndMenu.tsx:982 src/commandsAndMenu.tsx:983
+#: src/commandsAndMenu.tsx:1047 src/commandsAndMenu.tsx:876 src/commandsAndMenu.tsx:881
+msgid "Continue the rebase by committing the current state."
+msgstr ""
+
+#: src/commandsAndMenu.tsx:1051 src/commandsAndMenu.tsx:1067 src/commandsAndMenu.tsx:1089 src/commandsAndMenu.tsx:1093 src/commandsAndMenu.tsx:1122 src/commandsAndMenu.tsx:1351 src/commandsAndMenu.tsx:1356 src/commandsAndMenu.tsx:1539 src/commandsAndMenu.tsx:724 src/commandsAndMenu.tsx:726 src/commandsAndMenu.tsx:732 src/commandsAndMenu.tsx:737 src/commandsAndMenu.tsx:757 src/commandsAndMenu.tsx:758 src/commandsAndMenu.tsx:859 src/commandsAndMenu.tsx:923 src/commandsAndMenu.tsx:982 src/commandsAndMenu.tsx:983
 msgid "Delete this file"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1051 src/commandsAndMenu.tsx:1111 src/commandsAndMenu.tsx:1112 src/commandsAndMenu.tsx:1180 src/commandsAndMenu.tsx:1196 src/commandsAndMenu.tsx:1218 src/commandsAndMenu.tsx:1222 src/commandsAndMenu.tsx:1251 src/commandsAndMenu.tsx:1480 src/commandsAndMenu.tsx:1485 src/commandsAndMenu.tsx:852 src/commandsAndMenu.tsx:854 src/commandsAndMenu.tsx:860 src/commandsAndMenu.tsx:865 src/commandsAndMenu.tsx:885 src/commandsAndMenu.tsx:886 src/commandsAndMenu.tsx:987
+#: src/commandsAndMenu.tsx:1051 src/commandsAndMenu.tsx:1111 src/commandsAndMenu.tsx:1112 src/commandsAndMenu.tsx:1180 src/commandsAndMenu.tsx:1196 src/commandsAndMenu.tsx:1218 src/commandsAndMenu.tsx:1222 src/commandsAndMenu.tsx:1251 src/commandsAndMenu.tsx:1480 src/commandsAndMenu.tsx:1485 src/commandsAndMenu.tsx:1677 src/commandsAndMenu.tsx:852 src/commandsAndMenu.tsx:854 src/commandsAndMenu.tsx:860 src/commandsAndMenu.tsx:865 src/commandsAndMenu.tsx:885 src/commandsAndMenu.tsx:886 src/commandsAndMenu.tsx:987
 msgid "Ignore this file extension (add to .gitignore)"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1052 src/commandsAndMenu.tsx:1068 src/commandsAndMenu.tsx:1090 src/commandsAndMenu.tsx:1094 src/commandsAndMenu.tsx:1123 src/commandsAndMenu.tsx:1352 src/commandsAndMenu.tsx:1357 src/commandsAndMenu.tsx:725 src/commandsAndMenu.tsx:727 src/commandsAndMenu.tsx:733 src/commandsAndMenu.tsx:738 src/commandsAndMenu.tsx:758 src/commandsAndMenu.tsx:759 src/commandsAndMenu.tsx:860 src/commandsAndMenu.tsx:924 src/commandsAndMenu.tsx:983 src/commandsAndMenu.tsx:984
+#: src/commandsAndMenu.tsx:1051 src/commandsAndMenu.tsx:880 src/commandsAndMenu.tsx:885
+msgid "Skip current commit and continue the rebase."
+msgstr ""
+
+#: src/commandsAndMenu.tsx:1052 src/commandsAndMenu.tsx:1068 src/commandsAndMenu.tsx:1090 src/commandsAndMenu.tsx:1094 src/commandsAndMenu.tsx:1123 src/commandsAndMenu.tsx:1352 src/commandsAndMenu.tsx:1357 src/commandsAndMenu.tsx:1540 src/commandsAndMenu.tsx:725 src/commandsAndMenu.tsx:727 src/commandsAndMenu.tsx:733 src/commandsAndMenu.tsx:738 src/commandsAndMenu.tsx:758 src/commandsAndMenu.tsx:759 src/commandsAndMenu.tsx:860 src/commandsAndMenu.tsx:924 src/commandsAndMenu.tsx:983 src/commandsAndMenu.tsx:984
 msgid "Delete these files"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1052 src/commandsAndMenu.tsx:1112 src/commandsAndMenu.tsx:1113 src/commandsAndMenu.tsx:1181 src/commandsAndMenu.tsx:1197 src/commandsAndMenu.tsx:1219 src/commandsAndMenu.tsx:1223 src/commandsAndMenu.tsx:1252 src/commandsAndMenu.tsx:1481 src/commandsAndMenu.tsx:1486 src/commandsAndMenu.tsx:853 src/commandsAndMenu.tsx:855 src/commandsAndMenu.tsx:861 src/commandsAndMenu.tsx:866 src/commandsAndMenu.tsx:886 src/commandsAndMenu.tsx:887 src/commandsAndMenu.tsx:988
+#: src/commandsAndMenu.tsx:1052 src/commandsAndMenu.tsx:1112 src/commandsAndMenu.tsx:1113 src/commandsAndMenu.tsx:1181 src/commandsAndMenu.tsx:1197 src/commandsAndMenu.tsx:1219 src/commandsAndMenu.tsx:1223 src/commandsAndMenu.tsx:1252 src/commandsAndMenu.tsx:1481 src/commandsAndMenu.tsx:1486 src/commandsAndMenu.tsx:1678 src/commandsAndMenu.tsx:853 src/commandsAndMenu.tsx:855 src/commandsAndMenu.tsx:861 src/commandsAndMenu.tsx:866 src/commandsAndMenu.tsx:886 src/commandsAndMenu.tsx:887 src/commandsAndMenu.tsx:988
 msgid "Ignore these files extension (add to .gitignore)"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1059 src/commandsAndMenu.tsx:1075 src/commandsAndMenu.tsx:1097 src/commandsAndMenu.tsx:1101 src/commandsAndMenu.tsx:1130 src/commandsAndMenu.tsx:1359 src/commandsAndMenu.tsx:1364 src/commandsAndMenu.tsx:732 src/commandsAndMenu.tsx:734 src/commandsAndMenu.tsx:740 src/commandsAndMenu.tsx:745 src/commandsAndMenu.tsx:765 src/commandsAndMenu.tsx:766 src/commandsAndMenu.tsx:867 src/commandsAndMenu.tsx:931 src/commandsAndMenu.tsx:990 src/commandsAndMenu.tsx:991
+#: src/commandsAndMenu.tsx:1053 src/commandsAndMenu.tsx:882 src/commandsAndMenu.tsx:887
+msgid "Abort the rebase"
+msgstr ""
+
+#: src/commandsAndMenu.tsx:1059 src/commandsAndMenu.tsx:1075 src/commandsAndMenu.tsx:1097 src/commandsAndMenu.tsx:1101 src/commandsAndMenu.tsx:1130 src/commandsAndMenu.tsx:1359 src/commandsAndMenu.tsx:1364 src/commandsAndMenu.tsx:1547 src/commandsAndMenu.tsx:732 src/commandsAndMenu.tsx:734 src/commandsAndMenu.tsx:740 src/commandsAndMenu.tsx:745 src/commandsAndMenu.tsx:765 src/commandsAndMenu.tsx:766 src/commandsAndMenu.tsx:867 src/commandsAndMenu.tsx:931 src/commandsAndMenu.tsx:990 src/commandsAndMenu.tsx:991
 msgid "Delete Files"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1061 src/commandsAndMenu.tsx:1121 src/commandsAndMenu.tsx:1122 src/commandsAndMenu.tsx:1190 src/commandsAndMenu.tsx:1206 src/commandsAndMenu.tsx:1228 src/commandsAndMenu.tsx:1232 src/commandsAndMenu.tsx:1261 src/commandsAndMenu.tsx:1490 src/commandsAndMenu.tsx:1495 src/commandsAndMenu.tsx:862 src/commandsAndMenu.tsx:864 src/commandsAndMenu.tsx:870 src/commandsAndMenu.tsx:875 src/commandsAndMenu.tsx:895 src/commandsAndMenu.tsx:896 src/commandsAndMenu.tsx:997
+#: src/commandsAndMenu.tsx:1061 src/commandsAndMenu.tsx:1121 src/commandsAndMenu.tsx:1122 src/commandsAndMenu.tsx:1190 src/commandsAndMenu.tsx:1206 src/commandsAndMenu.tsx:1228 src/commandsAndMenu.tsx:1232 src/commandsAndMenu.tsx:1261 src/commandsAndMenu.tsx:1490 src/commandsAndMenu.tsx:1495 src/commandsAndMenu.tsx:1687 src/commandsAndMenu.tsx:862 src/commandsAndMenu.tsx:864 src/commandsAndMenu.tsx:870 src/commandsAndMenu.tsx:875 src/commandsAndMenu.tsx:895 src/commandsAndMenu.tsx:896 src/commandsAndMenu.tsx:997
 msgid "Ignore file extension"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1062 src/commandsAndMenu.tsx:1078 src/commandsAndMenu.tsx:1100 src/commandsAndMenu.tsx:1104 src/commandsAndMenu.tsx:1133 src/commandsAndMenu.tsx:1362 src/commandsAndMenu.tsx:1367 src/commandsAndMenu.tsx:735 src/commandsAndMenu.tsx:737 src/commandsAndMenu.tsx:743 src/commandsAndMenu.tsx:748 src/commandsAndMenu.tsx:768 src/commandsAndMenu.tsx:769 src/commandsAndMenu.tsx:870 src/commandsAndMenu.tsx:934 src/commandsAndMenu.tsx:993 src/commandsAndMenu.tsx:994
+#: src/commandsAndMenu.tsx:1062 src/commandsAndMenu.tsx:1078 src/commandsAndMenu.tsx:1100 src/commandsAndMenu.tsx:1104 src/commandsAndMenu.tsx:1133 src/commandsAndMenu.tsx:1362 src/commandsAndMenu.tsx:1367 src/commandsAndMenu.tsx:1550 src/commandsAndMenu.tsx:735 src/commandsAndMenu.tsx:737 src/commandsAndMenu.tsx:743 src/commandsAndMenu.tsx:748 src/commandsAndMenu.tsx:768 src/commandsAndMenu.tsx:769 src/commandsAndMenu.tsx:870 src/commandsAndMenu.tsx:934 src/commandsAndMenu.tsx:993 src/commandsAndMenu.tsx:994
 msgid "Are you sure you want to permanently delete the following files?               This action cannot be undone."
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1062 src/commandsAndMenu.tsx:1122 src/commandsAndMenu.tsx:1123 src/commandsAndMenu.tsx:1191 src/commandsAndMenu.tsx:1207 src/commandsAndMenu.tsx:1229 src/commandsAndMenu.tsx:1233 src/commandsAndMenu.tsx:1262 src/commandsAndMenu.tsx:1491 src/commandsAndMenu.tsx:1496 src/commandsAndMenu.tsx:863 src/commandsAndMenu.tsx:865 src/commandsAndMenu.tsx:871 src/commandsAndMenu.tsx:876 src/commandsAndMenu.tsx:896 src/commandsAndMenu.tsx:897 src/commandsAndMenu.tsx:998
+#: src/commandsAndMenu.tsx:1062 src/commandsAndMenu.tsx:1122 src/commandsAndMenu.tsx:1123 src/commandsAndMenu.tsx:1191 src/commandsAndMenu.tsx:1207 src/commandsAndMenu.tsx:1229 src/commandsAndMenu.tsx:1233 src/commandsAndMenu.tsx:1262 src/commandsAndMenu.tsx:1491 src/commandsAndMenu.tsx:1496 src/commandsAndMenu.tsx:1688 src/commandsAndMenu.tsx:863 src/commandsAndMenu.tsx:865 src/commandsAndMenu.tsx:871 src/commandsAndMenu.tsx:876 src/commandsAndMenu.tsx:896 src/commandsAndMenu.tsx:897 src/commandsAndMenu.tsx:998
 msgid "Are you sure you want to ignore all %1 files within this git repository?"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1062 src/commandsAndMenu.tsx:1126 src/commandsAndMenu.tsx:1186 src/commandsAndMenu.tsx:1187 src/commandsAndMenu.tsx:1255 src/commandsAndMenu.tsx:1271 src/commandsAndMenu.tsx:1293 src/commandsAndMenu.tsx:1297 src/commandsAndMenu.tsx:1326 src/commandsAndMenu.tsx:1555 src/commandsAndMenu.tsx:1633 src/commandsAndMenu.tsx:908 src/commandsAndMenu.tsx:910 src/commandsAndMenu.tsx:916 src/commandsAndMenu.tsx:940 src/commandsAndMenu.tsx:960 src/commandsAndMenu.tsx:961
+#: src/commandsAndMenu.tsx:1062 src/commandsAndMenu.tsx:1126 src/commandsAndMenu.tsx:1186 src/commandsAndMenu.tsx:1187 src/commandsAndMenu.tsx:1255 src/commandsAndMenu.tsx:1271 src/commandsAndMenu.tsx:1293 src/commandsAndMenu.tsx:1297 src/commandsAndMenu.tsx:1326 src/commandsAndMenu.tsx:1555 src/commandsAndMenu.tsx:1633 src/commandsAndMenu.tsx:1823 src/commandsAndMenu.tsx:908 src/commandsAndMenu.tsx:910 src/commandsAndMenu.tsx:916 src/commandsAndMenu.tsx:940 src/commandsAndMenu.tsx:960 src/commandsAndMenu.tsx:961
 msgid "Set Up Remotes"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1066 src/commandsAndMenu.tsx:1130 src/commandsAndMenu.tsx:1190 src/commandsAndMenu.tsx:1191 src/commandsAndMenu.tsx:1259 src/commandsAndMenu.tsx:1275 src/commandsAndMenu.tsx:1297 src/commandsAndMenu.tsx:1301 src/commandsAndMenu.tsx:1330 src/commandsAndMenu.tsx:1559 src/commandsAndMenu.tsx:1637 src/commandsAndMenu.tsx:912 src/commandsAndMenu.tsx:914 src/commandsAndMenu.tsx:920 src/commandsAndMenu.tsx:944 src/commandsAndMenu.tsx:964 src/commandsAndMenu.tsx:965
+#: src/commandsAndMenu.tsx:1066 src/commandsAndMenu.tsx:1130 src/commandsAndMenu.tsx:1190 src/commandsAndMenu.tsx:1191 src/commandsAndMenu.tsx:1259 src/commandsAndMenu.tsx:1275 src/commandsAndMenu.tsx:1297 src/commandsAndMenu.tsx:1301 src/commandsAndMenu.tsx:1330 src/commandsAndMenu.tsx:1559 src/commandsAndMenu.tsx:1637 src/commandsAndMenu.tsx:1827 src/commandsAndMenu.tsx:912 src/commandsAndMenu.tsx:914 src/commandsAndMenu.tsx:920 src/commandsAndMenu.tsx:944 src/commandsAndMenu.tsx:964 src/commandsAndMenu.tsx:965
 msgid "Git Documentation"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1091 src/commandsAndMenu.tsx:1096 src/commandsAndMenu.tsx:544 src/commandsAndMenu.tsx:546 src/commandsAndMenu.tsx:551 src/commandsAndMenu.tsx:555 src/commandsAndMenu.tsx:556 src/commandsAndMenu.tsx:612 src/commandsAndMenu.tsx:676 src/commandsAndMenu.tsx:735 src/commandsAndMenu.tsx:736 src/commandsAndMenu.tsx:804 src/commandsAndMenu.tsx:820 src/commandsAndMenu.tsx:842 src/commandsAndMenu.tsx:846 src/commandsAndMenu.tsx:867
+#: src/commandsAndMenu.tsx:1066 src/commandsAndMenu.tsx:894 src/commandsAndMenu.tsx:899
+msgid "Continue the rebase…"
+msgstr ""
+
+#: src/commandsAndMenu.tsx:1068 src/commandsAndMenu.tsx:896 src/commandsAndMenu.tsx:901
+msgid "Skip current commit…"
+msgstr ""
+
+#: src/commandsAndMenu.tsx:1070 src/commandsAndMenu.tsx:898 src/commandsAndMenu.tsx:903
+msgid "Abort the rebase…"
+msgstr ""
+
+#: src/commandsAndMenu.tsx:1084 src/commandsAndMenu.tsx:912 src/commandsAndMenu.tsx:917
+msgid "Fail to continue rebasing."
+msgstr ""
+
+#: src/commandsAndMenu.tsx:1086 src/commandsAndMenu.tsx:914 src/commandsAndMenu.tsx:919
+msgid "Fail to skip current commit when rebasing."
+msgstr ""
+
+#: src/commandsAndMenu.tsx:1088 src/commandsAndMenu.tsx:916 src/commandsAndMenu.tsx:921
+msgid "Fail to abort the rebase."
+msgstr ""
+
+#: src/commandsAndMenu.tsx:1091 src/commandsAndMenu.tsx:1096 src/commandsAndMenu.tsx:1272 src/commandsAndMenu.tsx:544 src/commandsAndMenu.tsx:546 src/commandsAndMenu.tsx:551 src/commandsAndMenu.tsx:555 src/commandsAndMenu.tsx:556 src/commandsAndMenu.tsx:612 src/commandsAndMenu.tsx:676 src/commandsAndMenu.tsx:735 src/commandsAndMenu.tsx:736 src/commandsAndMenu.tsx:804 src/commandsAndMenu.tsx:820 src/commandsAndMenu.tsx:842 src/commandsAndMenu.tsx:846 src/commandsAndMenu.tsx:867
 msgid "Diff"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1093 src/commandsAndMenu.tsx:1098 src/commandsAndMenu.tsx:546 src/commandsAndMenu.tsx:548 src/commandsAndMenu.tsx:553 src/commandsAndMenu.tsx:557 src/commandsAndMenu.tsx:558 src/commandsAndMenu.tsx:614 src/commandsAndMenu.tsx:678 src/commandsAndMenu.tsx:737 src/commandsAndMenu.tsx:738 src/commandsAndMenu.tsx:806 src/commandsAndMenu.tsx:822 src/commandsAndMenu.tsx:844 src/commandsAndMenu.tsx:848 src/commandsAndMenu.tsx:869
+#: src/commandsAndMenu.tsx:1093 src/commandsAndMenu.tsx:1098 src/commandsAndMenu.tsx:1274 src/commandsAndMenu.tsx:546 src/commandsAndMenu.tsx:548 src/commandsAndMenu.tsx:553 src/commandsAndMenu.tsx:557 src/commandsAndMenu.tsx:558 src/commandsAndMenu.tsx:614 src/commandsAndMenu.tsx:678 src/commandsAndMenu.tsx:737 src/commandsAndMenu.tsx:738 src/commandsAndMenu.tsx:806 src/commandsAndMenu.tsx:822 src/commandsAndMenu.tsx:844 src/commandsAndMenu.tsx:848 src/commandsAndMenu.tsx:869
 msgid "Diff selected file"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1094 src/commandsAndMenu.tsx:1099 src/commandsAndMenu.tsx:547 src/commandsAndMenu.tsx:549 src/commandsAndMenu.tsx:554 src/commandsAndMenu.tsx:558 src/commandsAndMenu.tsx:559 src/commandsAndMenu.tsx:615 src/commandsAndMenu.tsx:679 src/commandsAndMenu.tsx:738 src/commandsAndMenu.tsx:739 src/commandsAndMenu.tsx:807 src/commandsAndMenu.tsx:823 src/commandsAndMenu.tsx:845 src/commandsAndMenu.tsx:849 src/commandsAndMenu.tsx:870
+#: src/commandsAndMenu.tsx:1094 src/commandsAndMenu.tsx:1099 src/commandsAndMenu.tsx:1275 src/commandsAndMenu.tsx:547 src/commandsAndMenu.tsx:549 src/commandsAndMenu.tsx:554 src/commandsAndMenu.tsx:558 src/commandsAndMenu.tsx:559 src/commandsAndMenu.tsx:615 src/commandsAndMenu.tsx:679 src/commandsAndMenu.tsx:738 src/commandsAndMenu.tsx:739 src/commandsAndMenu.tsx:807 src/commandsAndMenu.tsx:823 src/commandsAndMenu.tsx:845 src/commandsAndMenu.tsx:849 src/commandsAndMenu.tsx:870
 msgid "Diff selected files"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1100 src/commandsAndMenu.tsx:1168 src/commandsAndMenu.tsx:1229 src/commandsAndMenu.tsx:1230 src/commandsAndMenu.tsx:1298 src/commandsAndMenu.tsx:1314 src/commandsAndMenu.tsx:1336 src/commandsAndMenu.tsx:1340 src/commandsAndMenu.tsx:1369 src/commandsAndMenu.tsx:1599 src/commandsAndMenu.tsx:1677 src/commandsAndMenu.tsx:943 src/commandsAndMenu.tsx:945 src/commandsAndMenu.tsx:951 src/commandsAndMenu.tsx:978 src/commandsAndMenu.tsx:998 src/commandsAndMenu.tsx:999
+#: src/commandsAndMenu.tsx:1100 src/commandsAndMenu.tsx:1168 src/commandsAndMenu.tsx:1229 src/commandsAndMenu.tsx:1230 src/commandsAndMenu.tsx:1298 src/commandsAndMenu.tsx:1314 src/commandsAndMenu.tsx:1336 src/commandsAndMenu.tsx:1340 src/commandsAndMenu.tsx:1369 src/commandsAndMenu.tsx:1599 src/commandsAndMenu.tsx:1677 src/commandsAndMenu.tsx:1867 src/commandsAndMenu.tsx:943 src/commandsAndMenu.tsx:945 src/commandsAndMenu.tsx:951 src/commandsAndMenu.tsx:978 src/commandsAndMenu.tsx:998 src/commandsAndMenu.tsx:999
 msgid " Help "
 msgstr ""
 
-#: src/commandsAndMenu.tsx:117 src/commandsAndMenu.tsx:118 src/commandsAndMenu.tsx:119 src/commandsAndMenu.tsx:122 src/commandsAndMenu.tsx:124 src/commandsAndMenu.tsx:125 src/commandsAndMenu.tsx:126 src/commandsAndMenu.tsx:127 src/commandsAndMenu.tsx:133 src/commandsAndMenu.tsx:137 src/commandsAndMenu.tsx:139 src/commandsAndMenu.tsx:140 src/commandsAndMenu.tsx:145
+#: src/commandsAndMenu.tsx:1104 src/commandsAndMenu.tsx:930 src/commandsAndMenu.tsx:935
+msgid "Commit submitted continuing rebase."
+msgstr ""
+
+#: src/commandsAndMenu.tsx:1106 src/commandsAndMenu.tsx:932 src/commandsAndMenu.tsx:937
+msgid "Current commit skipped."
+msgstr ""
+
+#: src/commandsAndMenu.tsx:1108 src/commandsAndMenu.tsx:934 src/commandsAndMenu.tsx:939
+msgid "Rebase aborted."
+msgstr ""
+
+#: src/commandsAndMenu.tsx:1123 src/commandsAndMenu.tsx:947 src/commandsAndMenu.tsx:952
+msgid "Stash Changes"
+msgstr ""
+
+#: src/commandsAndMenu.tsx:1124 src/commandsAndMenu.tsx:948 src/commandsAndMenu.tsx:953
+msgid "Stash all current changes"
+msgstr ""
+
+#: src/commandsAndMenu.tsx:1129 src/commandsAndMenu.tsx:953 src/commandsAndMenu.tsx:958
+msgid "Do you want to stash your changes? "
+msgstr ""
+
+#: src/commandsAndMenu.tsx:1130 src/commandsAndMenu.tsx:954 src/commandsAndMenu.tsx:959
+msgid "Stash message (optional)"
+msgstr ""
+
+#: src/commandsAndMenu.tsx:1131 src/commandsAndMenu.tsx:955 src/commandsAndMenu.tsx:960 src/components/GitStash.tsx:240 src/components/GitStash.tsx:241
+msgid "Stash"
+msgstr ""
+
+#: src/commandsAndMenu.tsx:1137 src/commandsAndMenu.tsx:962 src/commandsAndMenu.tsx:967
+msgid "Stashing changes"
+msgstr ""
+
+#: src/commandsAndMenu.tsx:1146 src/commandsAndMenu.tsx:968 src/commandsAndMenu.tsx:973
+msgid "Successfully stashed"
+msgstr ""
+
+#: src/commandsAndMenu.tsx:1157
+msgid "Failed to stash"
+msgstr ""
+
+#: src/commandsAndMenu.tsx:117 src/commandsAndMenu.tsx:118 src/commandsAndMenu.tsx:119 src/commandsAndMenu.tsx:122 src/commandsAndMenu.tsx:124 src/commandsAndMenu.tsx:125 src/commandsAndMenu.tsx:126 src/commandsAndMenu.tsx:127 src/commandsAndMenu.tsx:133 src/commandsAndMenu.tsx:137 src/commandsAndMenu.tsx:139 src/commandsAndMenu.tsx:140 src/commandsAndMenu.tsx:145 src/commandsAndMenu.tsx:152
 msgid "Commit from the Commit Box"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1172 src/commandsAndMenu.tsx:1174 src/commandsAndMenu.tsx:1180 src/commandsAndMenu.tsx:1203 src/commandsAndMenu.tsx:1232 src/commandsAndMenu.tsx:1236 src/commandsAndMenu.tsx:1241 src/commandsAndMenu.tsx:1338 src/commandsAndMenu.tsx:1404 src/commandsAndMenu.tsx:1465 src/commandsAndMenu.tsx:1470 src/commandsAndMenu.tsx:1538 src/commandsAndMenu.tsx:1562 src/commandsAndMenu.tsx:1590 src/commandsAndMenu.tsx:1596 src/commandsAndMenu.tsx:1625 src/commandsAndMenu.tsx:1928 src/commandsAndMenu.tsx:2021
+#: src/commandsAndMenu.tsx:1171 src/commandsAndMenu.tsx:986 src/commandsAndMenu.tsx:991
+msgid "Stash List"
+msgstr ""
+
+#: src/commandsAndMenu.tsx:1172 src/commandsAndMenu.tsx:1174 src/commandsAndMenu.tsx:1180 src/commandsAndMenu.tsx:1203 src/commandsAndMenu.tsx:1232 src/commandsAndMenu.tsx:1236 src/commandsAndMenu.tsx:1241 src/commandsAndMenu.tsx:1338 src/commandsAndMenu.tsx:1404 src/commandsAndMenu.tsx:1465 src/commandsAndMenu.tsx:1470 src/commandsAndMenu.tsx:1538 src/commandsAndMenu.tsx:1562 src/commandsAndMenu.tsx:1590 src/commandsAndMenu.tsx:1596 src/commandsAndMenu.tsx:1625 src/commandsAndMenu.tsx:1928 src/commandsAndMenu.tsx:2021 src/commandsAndMenu.tsx:2216
 msgid "Git credentials required"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1175 src/commandsAndMenu.tsx:1177 src/commandsAndMenu.tsx:1183 src/commandsAndMenu.tsx:1206 src/commandsAndMenu.tsx:1235 src/commandsAndMenu.tsx:1239 src/commandsAndMenu.tsx:1244 src/commandsAndMenu.tsx:1341 src/commandsAndMenu.tsx:1407 src/commandsAndMenu.tsx:1468 src/commandsAndMenu.tsx:1473 src/commandsAndMenu.tsx:1541 src/commandsAndMenu.tsx:1565 src/commandsAndMenu.tsx:1593 src/commandsAndMenu.tsx:1599 src/commandsAndMenu.tsx:1628 src/commandsAndMenu.tsx:1931 src/commandsAndMenu.tsx:2024 src/widgets/CredentialsBox.tsx:14 src/widgets/CredentialsBox.tsx:15 src/widgets/CredentialsBox.tsx:16
+#: src/commandsAndMenu.tsx:1172 src/commandsAndMenu.tsx:987 src/commandsAndMenu.tsx:992
+msgid "Get all the stashed changes"
+msgstr ""
+
+#: src/commandsAndMenu.tsx:1175 src/commandsAndMenu.tsx:1177 src/commandsAndMenu.tsx:1183 src/commandsAndMenu.tsx:1206 src/commandsAndMenu.tsx:1235 src/commandsAndMenu.tsx:1239 src/commandsAndMenu.tsx:1244 src/commandsAndMenu.tsx:1341 src/commandsAndMenu.tsx:1407 src/commandsAndMenu.tsx:1468 src/commandsAndMenu.tsx:1473 src/commandsAndMenu.tsx:1541 src/commandsAndMenu.tsx:1565 src/commandsAndMenu.tsx:1593 src/commandsAndMenu.tsx:1599 src/commandsAndMenu.tsx:1628 src/commandsAndMenu.tsx:1931 src/commandsAndMenu.tsx:2024 src/commandsAndMenu.tsx:2219 src/widgets/CredentialsBox.tsx:14 src/widgets/CredentialsBox.tsx:15 src/widgets/CredentialsBox.tsx:16
 msgid "Enter credentials for remote repository"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1176 src/commandsAndMenu.tsx:1178 src/commandsAndMenu.tsx:1184 src/commandsAndMenu.tsx:1207 src/commandsAndMenu.tsx:1236 src/commandsAndMenu.tsx:1240 src/commandsAndMenu.tsx:1245 src/commandsAndMenu.tsx:1342 src/commandsAndMenu.tsx:1408 src/commandsAndMenu.tsx:1469 src/commandsAndMenu.tsx:1474 src/commandsAndMenu.tsx:1542 src/commandsAndMenu.tsx:1566 src/commandsAndMenu.tsx:1594 src/commandsAndMenu.tsx:1600 src/commandsAndMenu.tsx:1629 src/commandsAndMenu.tsx:1932 src/commandsAndMenu.tsx:2025
+#: src/commandsAndMenu.tsx:1176 src/commandsAndMenu.tsx:1178 src/commandsAndMenu.tsx:1184 src/commandsAndMenu.tsx:1207 src/commandsAndMenu.tsx:1236 src/commandsAndMenu.tsx:1240 src/commandsAndMenu.tsx:1245 src/commandsAndMenu.tsx:1342 src/commandsAndMenu.tsx:1408 src/commandsAndMenu.tsx:1469 src/commandsAndMenu.tsx:1474 src/commandsAndMenu.tsx:1542 src/commandsAndMenu.tsx:1566 src/commandsAndMenu.tsx:1594 src/commandsAndMenu.tsx:1600 src/commandsAndMenu.tsx:1629 src/commandsAndMenu.tsx:1932 src/commandsAndMenu.tsx:2025 src/commandsAndMenu.tsx:2220
 msgid "Incorrect username or password."
 msgstr ""
 
-#: src/commandsAndMenu.tsx:118 src/commandsAndMenu.tsx:119 src/commandsAndMenu.tsx:120 src/commandsAndMenu.tsx:123 src/commandsAndMenu.tsx:125 src/commandsAndMenu.tsx:126 src/commandsAndMenu.tsx:127 src/commandsAndMenu.tsx:128 src/commandsAndMenu.tsx:134 src/commandsAndMenu.tsx:138 src/commandsAndMenu.tsx:140 src/commandsAndMenu.tsx:141 src/commandsAndMenu.tsx:146
+#: src/commandsAndMenu.tsx:1178 src/commandsAndMenu.tsx:994 src/commandsAndMenu.tsx:999
+msgid "Got the stash list"
+msgstr ""
+
+#: src/commandsAndMenu.tsx:118 src/commandsAndMenu.tsx:119 src/commandsAndMenu.tsx:120 src/commandsAndMenu.tsx:123 src/commandsAndMenu.tsx:125 src/commandsAndMenu.tsx:126 src/commandsAndMenu.tsx:127 src/commandsAndMenu.tsx:128 src/commandsAndMenu.tsx:134 src/commandsAndMenu.tsx:138 src/commandsAndMenu.tsx:140 src/commandsAndMenu.tsx:141 src/commandsAndMenu.tsx:146 src/commandsAndMenu.tsx:153
 msgid "Submit the commit using the summary and description from commit box"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1195 src/commandsAndMenu.tsx:1200 src/commandsAndMenu.tsx:768 src/commandsAndMenu.tsx:827 src/commandsAndMenu.tsx:828 src/commandsAndMenu.tsx:896 src/commandsAndMenu.tsx:912 src/commandsAndMenu.tsx:934 src/commandsAndMenu.tsx:938 src/commandsAndMenu.tsx:966
+#: src/commandsAndMenu.tsx:1195 src/commandsAndMenu.tsx:1200 src/commandsAndMenu.tsx:1381 src/commandsAndMenu.tsx:768 src/commandsAndMenu.tsx:827 src/commandsAndMenu.tsx:828 src/commandsAndMenu.tsx:896 src/commandsAndMenu.tsx:912 src/commandsAndMenu.tsx:934 src/commandsAndMenu.tsx:938 src/commandsAndMenu.tsx:966
 msgid "Current"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1196 src/commandsAndMenu.tsx:1201 src/commandsAndMenu.tsx:769 src/commandsAndMenu.tsx:828 src/commandsAndMenu.tsx:829 src/commandsAndMenu.tsx:897 src/commandsAndMenu.tsx:913 src/commandsAndMenu.tsx:935 src/commandsAndMenu.tsx:939 src/commandsAndMenu.tsx:967
+#: src/commandsAndMenu.tsx:1196 src/commandsAndMenu.tsx:1201 src/commandsAndMenu.tsx:1382 src/commandsAndMenu.tsx:769 src/commandsAndMenu.tsx:828 src/commandsAndMenu.tsx:829 src/commandsAndMenu.tsx:897 src/commandsAndMenu.tsx:913 src/commandsAndMenu.tsx:935 src/commandsAndMenu.tsx:939 src/commandsAndMenu.tsx:967
 msgid "Incoming"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1212 src/commandsAndMenu.tsx:1217 src/commandsAndMenu.tsx:785 src/commandsAndMenu.tsx:844 src/commandsAndMenu.tsx:845 src/commandsAndMenu.tsx:913 src/commandsAndMenu.tsx:929 src/commandsAndMenu.tsx:951 src/commandsAndMenu.tsx:955 src/commandsAndMenu.tsx:983
+#: src/commandsAndMenu.tsx:1212 src/commandsAndMenu.tsx:1217 src/commandsAndMenu.tsx:1398 src/commandsAndMenu.tsx:785 src/commandsAndMenu.tsx:844 src/commandsAndMenu.tsx:845 src/commandsAndMenu.tsx:913 src/commandsAndMenu.tsx:929 src/commandsAndMenu.tsx:951 src/commandsAndMenu.tsx:955 src/commandsAndMenu.tsx:983
 msgid "Result"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:129 src/commandsAndMenu.tsx:130 src/commandsAndMenu.tsx:131 src/commandsAndMenu.tsx:134 src/commandsAndMenu.tsx:136 src/commandsAndMenu.tsx:137 src/commandsAndMenu.tsx:138 src/commandsAndMenu.tsx:139 src/commandsAndMenu.tsx:145 src/commandsAndMenu.tsx:149 src/commandsAndMenu.tsx:151 src/commandsAndMenu.tsx:152 src/commandsAndMenu.tsx:157
+#: src/commandsAndMenu.tsx:129 src/commandsAndMenu.tsx:130 src/commandsAndMenu.tsx:131 src/commandsAndMenu.tsx:134 src/commandsAndMenu.tsx:136 src/commandsAndMenu.tsx:137 src/commandsAndMenu.tsx:138 src/commandsAndMenu.tsx:139 src/commandsAndMenu.tsx:145 src/commandsAndMenu.tsx:149 src/commandsAndMenu.tsx:151 src/commandsAndMenu.tsx:152 src/commandsAndMenu.tsx:157 src/commandsAndMenu.tsx:164
 msgid "Open Git Repository in Terminal"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:130 src/commandsAndMenu.tsx:131 src/commandsAndMenu.tsx:132 src/commandsAndMenu.tsx:135 src/commandsAndMenu.tsx:137 src/commandsAndMenu.tsx:138 src/commandsAndMenu.tsx:139 src/commandsAndMenu.tsx:140 src/commandsAndMenu.tsx:146 src/commandsAndMenu.tsx:150 src/commandsAndMenu.tsx:152 src/commandsAndMenu.tsx:153 src/commandsAndMenu.tsx:158
+#: src/commandsAndMenu.tsx:130 src/commandsAndMenu.tsx:131 src/commandsAndMenu.tsx:132 src/commandsAndMenu.tsx:135 src/commandsAndMenu.tsx:137 src/commandsAndMenu.tsx:138 src/commandsAndMenu.tsx:139 src/commandsAndMenu.tsx:140 src/commandsAndMenu.tsx:146 src/commandsAndMenu.tsx:150 src/commandsAndMenu.tsx:152 src/commandsAndMenu.tsx:153 src/commandsAndMenu.tsx:158 src/commandsAndMenu.tsx:165
 msgid "Open a New Terminal to the Git Repository"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1303 src/commandsAndMenu.tsx:1307 src/commandsAndMenu.tsx:1336 src/commandsAndMenu.tsx:1509 src/commandsAndMenu.tsx:1513 src/commandsAndMenu.tsx:1542 src/commandsAndMenu.tsx:1565 src/commandsAndMenu.tsx:1643 src/commandsAndMenu.tsx:1772 src/commandsAndMenu.tsx:1865
+#: src/commandsAndMenu.tsx:1303 src/commandsAndMenu.tsx:1307 src/commandsAndMenu.tsx:1336 src/commandsAndMenu.tsx:1509 src/commandsAndMenu.tsx:1513 src/commandsAndMenu.tsx:1542 src/commandsAndMenu.tsx:1565 src/commandsAndMenu.tsx:1643 src/commandsAndMenu.tsx:1772 src/commandsAndMenu.tsx:1833 src/commandsAndMenu.tsx:1865 src/commandsAndMenu.tsx:2060
 msgid "Git"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1547
+#: src/commandsAndMenu.tsx:1547 src/commandsAndMenu.tsx:1739
 msgid "Add Tag"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1548
+#: src/commandsAndMenu.tsx:1548 src/commandsAndMenu.tsx:1740
 msgid "Add tag pointing to selected commit"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1586
+#: src/commandsAndMenu.tsx:1586 src/commandsAndMenu.tsx:1776
 msgid "Create tag pointing to '%1'..."
 msgstr ""
 
-#: src/commandsAndMenu.tsx:159 src/commandsAndMenu.tsx:161 src/commandsAndMenu.tsx:162 src/commandsAndMenu.tsx:163 src/commandsAndMenu.tsx:166 src/commandsAndMenu.tsx:168 src/commandsAndMenu.tsx:169 src/commandsAndMenu.tsx:170 src/commandsAndMenu.tsx:171 src/commandsAndMenu.tsx:177 src/commandsAndMenu.tsx:181 src/commandsAndMenu.tsx:187 src/commandsAndMenu.tsx:188 src/commandsAndMenu.tsx:193
+#: src/commandsAndMenu.tsx:159 src/commandsAndMenu.tsx:161 src/commandsAndMenu.tsx:162 src/commandsAndMenu.tsx:163 src/commandsAndMenu.tsx:166 src/commandsAndMenu.tsx:168 src/commandsAndMenu.tsx:169 src/commandsAndMenu.tsx:170 src/commandsAndMenu.tsx:171 src/commandsAndMenu.tsx:177 src/commandsAndMenu.tsx:181 src/commandsAndMenu.tsx:187 src/commandsAndMenu.tsx:188 src/commandsAndMenu.tsx:193 src/commandsAndMenu.tsx:200
 msgid "Git Interface"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1596
+#: src/commandsAndMenu.tsx:1596 src/commandsAndMenu.tsx:1784
 msgid "Failed to create tag '%1' poining to '%2'."
 msgstr ""
 
-#: src/commandsAndMenu.tsx:160 src/commandsAndMenu.tsx:162 src/commandsAndMenu.tsx:163 src/commandsAndMenu.tsx:164 src/commandsAndMenu.tsx:167 src/commandsAndMenu.tsx:169 src/commandsAndMenu.tsx:170 src/commandsAndMenu.tsx:171 src/commandsAndMenu.tsx:172 src/commandsAndMenu.tsx:178 src/commandsAndMenu.tsx:182 src/commandsAndMenu.tsx:188 src/commandsAndMenu.tsx:189 src/commandsAndMenu.tsx:194
+#: src/commandsAndMenu.tsx:160 src/commandsAndMenu.tsx:162 src/commandsAndMenu.tsx:163 src/commandsAndMenu.tsx:164 src/commandsAndMenu.tsx:167 src/commandsAndMenu.tsx:169 src/commandsAndMenu.tsx:170 src/commandsAndMenu.tsx:171 src/commandsAndMenu.tsx:172 src/commandsAndMenu.tsx:178 src/commandsAndMenu.tsx:182 src/commandsAndMenu.tsx:188 src/commandsAndMenu.tsx:189 src/commandsAndMenu.tsx:194 src/commandsAndMenu.tsx:201
 msgid "Go to Git user interface"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1608
+#: src/commandsAndMenu.tsx:1608 src/commandsAndMenu.tsx:1797
 msgid "Created tag '%1' pointing to '%2'."
 msgstr ""
 
-#: src/commandsAndMenu.tsx:172 src/commandsAndMenu.tsx:174 src/commandsAndMenu.tsx:175 src/commandsAndMenu.tsx:176 src/commandsAndMenu.tsx:179 src/commandsAndMenu.tsx:181 src/commandsAndMenu.tsx:182 src/commandsAndMenu.tsx:183 src/commandsAndMenu.tsx:184 src/commandsAndMenu.tsx:186 src/commandsAndMenu.tsx:188 src/commandsAndMenu.tsx:189 src/commandsAndMenu.tsx:190 src/commandsAndMenu.tsx:191 src/commandsAndMenu.tsx:194 src/commandsAndMenu.tsx:197 src/commandsAndMenu.tsx:200 src/commandsAndMenu.tsx:201 src/commandsAndMenu.tsx:206 src/commandsAndMenu.tsx:207 src/commandsAndMenu.tsx:208 src/commandsAndMenu.tsx:213 src/components/GitPanel.tsx:445 src/components/GitPanel.tsx:461 src/components/GitPanel.tsx:466 src/components/GitPanel.tsx:473 src/components/GitPanel.tsx:487 src/components/GitPanel.tsx:495 src/components/GitPanel.tsx:594 src/components/GitPanel.tsx:595 src/components/GitPanel.tsx:678 src/components/GitPanel.tsx:697 src/components/GitPanel.tsx:698
+#: src/commandsAndMenu.tsx:172 src/commandsAndMenu.tsx:174 src/commandsAndMenu.tsx:175 src/commandsAndMenu.tsx:176 src/commandsAndMenu.tsx:179 src/commandsAndMenu.tsx:181 src/commandsAndMenu.tsx:182 src/commandsAndMenu.tsx:183 src/commandsAndMenu.tsx:184 src/commandsAndMenu.tsx:186 src/commandsAndMenu.tsx:188 src/commandsAndMenu.tsx:189 src/commandsAndMenu.tsx:190 src/commandsAndMenu.tsx:191 src/commandsAndMenu.tsx:194 src/commandsAndMenu.tsx:197 src/commandsAndMenu.tsx:200 src/commandsAndMenu.tsx:201 src/commandsAndMenu.tsx:206 src/commandsAndMenu.tsx:207 src/commandsAndMenu.tsx:208 src/commandsAndMenu.tsx:213 src/commandsAndMenu.tsx:222 src/components/GitPanel.tsx:445 src/components/GitPanel.tsx:461 src/components/GitPanel.tsx:466 src/components/GitPanel.tsx:473 src/components/GitPanel.tsx:487 src/components/GitPanel.tsx:495 src/components/GitPanel.tsx:594 src/components/GitPanel.tsx:595 src/components/GitPanel.tsx:678 src/components/GitPanel.tsx:691 src/components/GitPanel.tsx:697 src/components/GitPanel.tsx:698
 msgid "Initialize a Repository"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:173 src/commandsAndMenu.tsx:175 src/commandsAndMenu.tsx:176 src/commandsAndMenu.tsx:177 src/commandsAndMenu.tsx:180 src/commandsAndMenu.tsx:182 src/commandsAndMenu.tsx:183 src/commandsAndMenu.tsx:184 src/commandsAndMenu.tsx:185 src/commandsAndMenu.tsx:191 src/commandsAndMenu.tsx:195 src/commandsAndMenu.tsx:201 src/commandsAndMenu.tsx:202 src/commandsAndMenu.tsx:207
+#: src/commandsAndMenu.tsx:173 src/commandsAndMenu.tsx:175 src/commandsAndMenu.tsx:176 src/commandsAndMenu.tsx:177 src/commandsAndMenu.tsx:180 src/commandsAndMenu.tsx:182 src/commandsAndMenu.tsx:183 src/commandsAndMenu.tsx:184 src/commandsAndMenu.tsx:185 src/commandsAndMenu.tsx:191 src/commandsAndMenu.tsx:195 src/commandsAndMenu.tsx:201 src/commandsAndMenu.tsx:202 src/commandsAndMenu.tsx:207 src/commandsAndMenu.tsx:214
 msgid "Create an empty Git repository or reinitialize an existing one"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:180 src/commandsAndMenu.tsx:182 src/commandsAndMenu.tsx:183 src/commandsAndMenu.tsx:184 src/commandsAndMenu.tsx:187 src/commandsAndMenu.tsx:189 src/commandsAndMenu.tsx:190 src/commandsAndMenu.tsx:191 src/commandsAndMenu.tsx:192 src/commandsAndMenu.tsx:198 src/commandsAndMenu.tsx:202 src/commandsAndMenu.tsx:208 src/commandsAndMenu.tsx:209 src/commandsAndMenu.tsx:214
+#: src/commandsAndMenu.tsx:180 src/commandsAndMenu.tsx:182 src/commandsAndMenu.tsx:183 src/commandsAndMenu.tsx:184 src/commandsAndMenu.tsx:187 src/commandsAndMenu.tsx:189 src/commandsAndMenu.tsx:190 src/commandsAndMenu.tsx:191 src/commandsAndMenu.tsx:192 src/commandsAndMenu.tsx:198 src/commandsAndMenu.tsx:202 src/commandsAndMenu.tsx:208 src/commandsAndMenu.tsx:209 src/commandsAndMenu.tsx:214 src/commandsAndMenu.tsx:223
 msgid "Do you really want to make this directory a Git Repo?"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:183 src/commandsAndMenu.tsx:185 src/commandsAndMenu.tsx:186 src/commandsAndMenu.tsx:187 src/commandsAndMenu.tsx:190 src/commandsAndMenu.tsx:192 src/commandsAndMenu.tsx:193 src/commandsAndMenu.tsx:194 src/commandsAndMenu.tsx:195 src/commandsAndMenu.tsx:201 src/commandsAndMenu.tsx:205 src/commandsAndMenu.tsx:211 src/commandsAndMenu.tsx:212 src/commandsAndMenu.tsx:217
+#: src/commandsAndMenu.tsx:183 src/commandsAndMenu.tsx:185 src/commandsAndMenu.tsx:186 src/commandsAndMenu.tsx:187 src/commandsAndMenu.tsx:190 src/commandsAndMenu.tsx:192 src/commandsAndMenu.tsx:193 src/commandsAndMenu.tsx:194 src/commandsAndMenu.tsx:195 src/commandsAndMenu.tsx:201 src/commandsAndMenu.tsx:205 src/commandsAndMenu.tsx:211 src/commandsAndMenu.tsx:212 src/commandsAndMenu.tsx:217 src/commandsAndMenu.tsx:226
 msgid "Yes"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1883 src/commandsAndMenu.tsx:1976 src/widgets/CredentialsBox.tsx:18 src/widgets/CredentialsBox.tsx:37 src/widgets/CredentialsBox.tsx:38 src/widgets/CredentialsBox.tsx:44
+#: src/commandsAndMenu.tsx:1883 src/commandsAndMenu.tsx:1976 src/commandsAndMenu.tsx:2171 src/widgets/CredentialsBox.tsx:18 src/widgets/CredentialsBox.tsx:37 src/widgets/CredentialsBox.tsx:38 src/widgets/CredentialsBox.tsx:44
 msgid "password / personal access token"
 msgstr ""
 
 #: src/commandsAndMenu.tsx:189 src/commandsAndMenu.tsx:191 src/commandsAndMenu.tsx:192 src/commandsAndMenu.tsx:193 src/commandsAndMenu.tsx:196
 msgid "Initializing..."
 msgstr ""
 
-#: src/commandsAndMenu.tsx:1924 src/commandsAndMenu.tsx:2017
+#: src/commandsAndMenu.tsx:1924 src/commandsAndMenu.tsx:2017 src/commandsAndMenu.tsx:2212
 msgid "personal access token"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:196 src/commandsAndMenu.tsx:198 src/commandsAndMenu.tsx:199 src/commandsAndMenu.tsx:200 src/commandsAndMenu.tsx:203 src/commandsAndMenu.tsx:205 src/commandsAndMenu.tsx:206 src/commandsAndMenu.tsx:207 src/commandsAndMenu.tsx:208 src/commandsAndMenu.tsx:214 src/commandsAndMenu.tsx:218 src/commandsAndMenu.tsx:224 src/commandsAndMenu.tsx:225 src/commandsAndMenu.tsx:230
+#: src/commandsAndMenu.tsx:196 src/commandsAndMenu.tsx:198 src/commandsAndMenu.tsx:199 src/commandsAndMenu.tsx:200 src/commandsAndMenu.tsx:203 src/commandsAndMenu.tsx:205 src/commandsAndMenu.tsx:206 src/commandsAndMenu.tsx:207 src/commandsAndMenu.tsx:208 src/commandsAndMenu.tsx:214 src/commandsAndMenu.tsx:218 src/commandsAndMenu.tsx:224 src/commandsAndMenu.tsx:225 src/commandsAndMenu.tsx:230 src/commandsAndMenu.tsx:239
 msgid "Git repository initialized."
 msgstr ""
 
-#: src/commandsAndMenu.tsx:198 src/commandsAndMenu.tsx:199 src/commandsAndMenu.tsx:200 src/commandsAndMenu.tsx:201 src/commandsAndMenu.tsx:207 src/commandsAndMenu.tsx:211 src/commandsAndMenu.tsx:217 src/commandsAndMenu.tsx:218 src/commandsAndMenu.tsx:223
+#: src/commandsAndMenu.tsx:198 src/commandsAndMenu.tsx:199 src/commandsAndMenu.tsx:200 src/commandsAndMenu.tsx:201 src/commandsAndMenu.tsx:207 src/commandsAndMenu.tsx:211 src/commandsAndMenu.tsx:217 src/commandsAndMenu.tsx:218 src/commandsAndMenu.tsx:223 src/commandsAndMenu.tsx:231
 msgid "Initializing…"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:201 src/commandsAndMenu.tsx:203 src/commandsAndMenu.tsx:204 src/commandsAndMenu.tsx:205 src/commandsAndMenu.tsx:208 src/commandsAndMenu.tsx:210 src/commandsAndMenu.tsx:211 src/commandsAndMenu.tsx:212 src/commandsAndMenu.tsx:213 src/commandsAndMenu.tsx:219 src/commandsAndMenu.tsx:223 src/commandsAndMenu.tsx:229 src/commandsAndMenu.tsx:230 src/commandsAndMenu.tsx:235
+#: src/commandsAndMenu.tsx:201 src/commandsAndMenu.tsx:203 src/commandsAndMenu.tsx:204 src/commandsAndMenu.tsx:205 src/commandsAndMenu.tsx:208 src/commandsAndMenu.tsx:210 src/commandsAndMenu.tsx:211 src/commandsAndMenu.tsx:212 src/commandsAndMenu.tsx:213 src/commandsAndMenu.tsx:219 src/commandsAndMenu.tsx:223 src/commandsAndMenu.tsx:229 src/commandsAndMenu.tsx:230 src/commandsAndMenu.tsx:235 src/commandsAndMenu.tsx:245
 msgid "Encountered an error when initializing the repository. Error: "
 msgstr ""
 
-#: src/commandsAndMenu.tsx:207 src/commandsAndMenu.tsx:209 src/commandsAndMenu.tsx:210 src/commandsAndMenu.tsx:211 src/commandsAndMenu.tsx:214 src/commandsAndMenu.tsx:216 src/commandsAndMenu.tsx:217 src/commandsAndMenu.tsx:218 src/commandsAndMenu.tsx:219 src/commandsAndMenu.tsx:225 src/commandsAndMenu.tsx:229 src/commandsAndMenu.tsx:235 src/commandsAndMenu.tsx:236 src/commandsAndMenu.tsx:241
+#: src/commandsAndMenu.tsx:207 src/commandsAndMenu.tsx:209 src/commandsAndMenu.tsx:210 src/commandsAndMenu.tsx:211 src/commandsAndMenu.tsx:214 src/commandsAndMenu.tsx:216 src/commandsAndMenu.tsx:217 src/commandsAndMenu.tsx:218 src/commandsAndMenu.tsx:219 src/commandsAndMenu.tsx:225 src/commandsAndMenu.tsx:229 src/commandsAndMenu.tsx:235 src/commandsAndMenu.tsx:236 src/commandsAndMenu.tsx:241 src/commandsAndMenu.tsx:252
 msgid "Failed to initialize the Git repository"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:228 src/commandsAndMenu.tsx:230 src/commandsAndMenu.tsx:231 src/commandsAndMenu.tsx:232 src/commandsAndMenu.tsx:235 src/commandsAndMenu.tsx:237 src/commandsAndMenu.tsx:238 src/commandsAndMenu.tsx:239 src/commandsAndMenu.tsx:240 src/commandsAndMenu.tsx:246 src/commandsAndMenu.tsx:250 src/commandsAndMenu.tsx:256 src/commandsAndMenu.tsx:257 src/commandsAndMenu.tsx:262
+#: src/commandsAndMenu.tsx:228 src/commandsAndMenu.tsx:230 src/commandsAndMenu.tsx:231 src/commandsAndMenu.tsx:232 src/commandsAndMenu.tsx:235 src/commandsAndMenu.tsx:237 src/commandsAndMenu.tsx:238 src/commandsAndMenu.tsx:239 src/commandsAndMenu.tsx:240 src/commandsAndMenu.tsx:246 src/commandsAndMenu.tsx:250 src/commandsAndMenu.tsx:256 src/commandsAndMenu.tsx:257 src/commandsAndMenu.tsx:262 src/commandsAndMenu.tsx:273
 msgid "Simple staging"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:237 src/commandsAndMenu.tsx:239 src/commandsAndMenu.tsx:240 src/commandsAndMenu.tsx:241 src/commandsAndMenu.tsx:244 src/commandsAndMenu.tsx:246 src/commandsAndMenu.tsx:247 src/commandsAndMenu.tsx:248 src/commandsAndMenu.tsx:249 src/commandsAndMenu.tsx:255 src/commandsAndMenu.tsx:259 src/commandsAndMenu.tsx:265 src/commandsAndMenu.tsx:266 src/commandsAndMenu.tsx:271
+#: src/commandsAndMenu.tsx:237 src/commandsAndMenu.tsx:239 src/commandsAndMenu.tsx:240 src/commandsAndMenu.tsx:241 src/commandsAndMenu.tsx:244 src/commandsAndMenu.tsx:246 src/commandsAndMenu.tsx:247 src/commandsAndMenu.tsx:248 src/commandsAndMenu.tsx:249 src/commandsAndMenu.tsx:255 src/commandsAndMenu.tsx:259 src/commandsAndMenu.tsx:265 src/commandsAndMenu.tsx:266 src/commandsAndMenu.tsx:271 src/commandsAndMenu.tsx:282
 msgid "Double click opens diff"
 msgstr ""
 
 #: src/commandsAndMenu.tsx:246 src/commandsAndMenu.tsx:248 src/commandsAndMenu.tsx:249 src/commandsAndMenu.tsx:250 src/commandsAndMenu.tsx:253 src/commandsAndMenu.tsx:255 src/commandsAndMenu.tsx:256 src/commandsAndMenu.tsx:257
 msgid "Add Remote Repository"
 msgstr ""
 
 #: src/commandsAndMenu.tsx:247 src/commandsAndMenu.tsx:249 src/commandsAndMenu.tsx:250 src/commandsAndMenu.tsx:251 src/commandsAndMenu.tsx:254 src/commandsAndMenu.tsx:256 src/commandsAndMenu.tsx:257 src/commandsAndMenu.tsx:258
 msgid "Add a Git remote repository"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:252 src/commandsAndMenu.tsx:254 src/commandsAndMenu.tsx:255 src/commandsAndMenu.tsx:256 src/commandsAndMenu.tsx:259 src/commandsAndMenu.tsx:261 src/commandsAndMenu.tsx:262 src/commandsAndMenu.tsx:263 src/commandsAndMenu.tsx:264 src/commandsAndMenu.tsx:270 src/commandsAndMenu.tsx:274 src/commandsAndMenu.tsx:280 src/commandsAndMenu.tsx:281 src/commandsAndMenu.tsx:286
+#: src/commandsAndMenu.tsx:252 src/commandsAndMenu.tsx:254 src/commandsAndMenu.tsx:255 src/commandsAndMenu.tsx:256 src/commandsAndMenu.tsx:259 src/commandsAndMenu.tsx:261 src/commandsAndMenu.tsx:262 src/commandsAndMenu.tsx:263 src/commandsAndMenu.tsx:264 src/commandsAndMenu.tsx:270 src/commandsAndMenu.tsx:274 src/commandsAndMenu.tsx:280 src/commandsAndMenu.tsx:281 src/commandsAndMenu.tsx:286 src/commandsAndMenu.tsx:297
 msgid "Not in a Git repository. Unable to add a remote."
 msgstr ""
 
-#: src/commandsAndMenu.tsx:258 src/commandsAndMenu.tsx:259 src/commandsAndMenu.tsx:264 src/commandsAndMenu.tsx:265 src/commandsAndMenu.tsx:268 src/commandsAndMenu.tsx:269 src/commandsAndMenu.tsx:274 src/commandsAndMenu.tsx:275 src/commandsAndMenu.tsx:276 src/commandsAndMenu.tsx:280 src/commandsAndMenu.tsx:281
+#: src/commandsAndMenu.tsx:258 src/commandsAndMenu.tsx:259 src/commandsAndMenu.tsx:264 src/commandsAndMenu.tsx:265 src/commandsAndMenu.tsx:268 src/commandsAndMenu.tsx:269 src/commandsAndMenu.tsx:274 src/commandsAndMenu.tsx:275 src/commandsAndMenu.tsx:276 src/commandsAndMenu.tsx:280 src/commandsAndMenu.tsx:281 src/commandsAndMenu.tsx:291 src/commandsAndMenu.tsx:292
 msgid "Manage Remote Repositories"
 msgstr ""
 
 #: src/commandsAndMenu.tsx:261 src/commandsAndMenu.tsx:263 src/commandsAndMenu.tsx:264 src/commandsAndMenu.tsx:265 src/commandsAndMenu.tsx:268 src/commandsAndMenu.tsx:270 src/commandsAndMenu.tsx:271 src/commandsAndMenu.tsx:272
 msgid "Add a remote repository"
 msgstr ""
 
@@ -557,195 +687,223 @@
 msgid "Remote Git repository URL"
 msgstr ""
 
 #: src/commandsAndMenu.tsx:276 src/commandsAndMenu.tsx:278 src/commandsAndMenu.tsx:279 src/commandsAndMenu.tsx:280 src/commandsAndMenu.tsx:283 src/commandsAndMenu.tsx:285 src/commandsAndMenu.tsx:286 src/commandsAndMenu.tsx:287 src/components/ManageRemoteDialogue.tsx:176
 msgid "Error when adding remote repository"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:291 src/commandsAndMenu.tsx:292 src/commandsAndMenu.tsx:295 src/commandsAndMenu.tsx:296 src/commandsAndMenu.tsx:297 src/commandsAndMenu.tsx:298 src/commandsAndMenu.tsx:301 src/commandsAndMenu.tsx:302 src/commandsAndMenu.tsx:307 src/commandsAndMenu.tsx:308 src/commandsAndMenu.tsx:309 src/commandsAndMenu.tsx:313 src/commandsAndMenu.tsx:314 src/commandsAndMenu.tsx:335 src/commandsAndMenu.tsx:336 src/commandsAndMenu.tsx:337 src/commandsAndMenu.tsx:338 src/commandsAndMenu.tsx:339 src/commandsAndMenu.tsx:340 src/commandsAndMenu.tsx:342 src/commandsAndMenu.tsx:343
+#: src/commandsAndMenu.tsx:291 src/commandsAndMenu.tsx:292 src/commandsAndMenu.tsx:295 src/commandsAndMenu.tsx:296 src/commandsAndMenu.tsx:297 src/commandsAndMenu.tsx:298 src/commandsAndMenu.tsx:301 src/commandsAndMenu.tsx:302 src/commandsAndMenu.tsx:307 src/commandsAndMenu.tsx:308 src/commandsAndMenu.tsx:309 src/commandsAndMenu.tsx:313 src/commandsAndMenu.tsx:314 src/commandsAndMenu.tsx:335 src/commandsAndMenu.tsx:336 src/commandsAndMenu.tsx:337 src/commandsAndMenu.tsx:338 src/commandsAndMenu.tsx:339 src/commandsAndMenu.tsx:340 src/commandsAndMenu.tsx:342 src/commandsAndMenu.tsx:343 src/commandsAndMenu.tsx:431 src/commandsAndMenu.tsx:432
 msgid "Open .gitignore"
 msgstr ""
 
 #: src/commandsAndMenu.tsx:296 src/commandsAndMenu.tsx:298 src/commandsAndMenu.tsx:299 src/commandsAndMenu.tsx:300 src/commandsAndMenu.tsx:303
 msgid "CLONE"
 msgstr ""
 
 #: src/commandsAndMenu.tsx:303 src/commandsAndMenu.tsx:305 src/commandsAndMenu.tsx:306 src/commandsAndMenu.tsx:307 src/commandsAndMenu.tsx:310
 msgid "Cloning..."
 msgstr ""
 
-#: src/commandsAndMenu.tsx:303 src/commandsAndMenu.tsx:309 src/commandsAndMenu.tsx:313 src/commandsAndMenu.tsx:319 src/commandsAndMenu.tsx:320 src/commandsAndMenu.tsx:325
+#: src/commandsAndMenu.tsx:303 src/commandsAndMenu.tsx:309 src/commandsAndMenu.tsx:313 src/commandsAndMenu.tsx:319 src/commandsAndMenu.tsx:320 src/commandsAndMenu.tsx:325 src/commandsAndMenu.tsx:452
 msgid "Push to Remote (Advanced)"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:304 src/commandsAndMenu.tsx:308 src/commandsAndMenu.tsx:309 src/commandsAndMenu.tsx:310 src/commandsAndMenu.tsx:314 src/commandsAndMenu.tsx:320 src/commandsAndMenu.tsx:321 src/commandsAndMenu.tsx:326 src/commandsAndMenu.tsx:345 src/commandsAndMenu.tsx:347 src/commandsAndMenu.tsx:351 src/commandsAndMenu.tsx:352 src/commandsAndMenu.tsx:355
+#: src/commandsAndMenu.tsx:304 src/commandsAndMenu.tsx:308 src/commandsAndMenu.tsx:309 src/commandsAndMenu.tsx:310 src/commandsAndMenu.tsx:314 src/commandsAndMenu.tsx:320 src/commandsAndMenu.tsx:321 src/commandsAndMenu.tsx:326 src/commandsAndMenu.tsx:345 src/commandsAndMenu.tsx:347 src/commandsAndMenu.tsx:351 src/commandsAndMenu.tsx:352 src/commandsAndMenu.tsx:355 src/commandsAndMenu.tsx:453
 msgid "Push to Remote"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:305 src/commandsAndMenu.tsx:309 src/commandsAndMenu.tsx:310 src/commandsAndMenu.tsx:311 src/commandsAndMenu.tsx:315 src/commandsAndMenu.tsx:321 src/commandsAndMenu.tsx:322 src/commandsAndMenu.tsx:327 src/commandsAndMenu.tsx:346 src/commandsAndMenu.tsx:348 src/commandsAndMenu.tsx:352 src/commandsAndMenu.tsx:353 src/commandsAndMenu.tsx:356
+#: src/commandsAndMenu.tsx:305 src/commandsAndMenu.tsx:309 src/commandsAndMenu.tsx:310 src/commandsAndMenu.tsx:311 src/commandsAndMenu.tsx:315 src/commandsAndMenu.tsx:321 src/commandsAndMenu.tsx:322 src/commandsAndMenu.tsx:327 src/commandsAndMenu.tsx:346 src/commandsAndMenu.tsx:348 src/commandsAndMenu.tsx:352 src/commandsAndMenu.tsx:353 src/commandsAndMenu.tsx:356 src/commandsAndMenu.tsx:454
 msgid "Push code to remote repository"
 msgstr ""
 
 #: src/commandsAndMenu.tsx:307 src/commandsAndMenu.tsx:308 src/commandsAndMenu.tsx:309 src/commandsAndMenu.tsx:350 src/commandsAndMenu.tsx:351 src/commandsAndMenu.tsx:354
 msgid "Push to Remote (Force)"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:314 src/commandsAndMenu.tsx:315 src/commandsAndMenu.tsx:316 src/commandsAndMenu.tsx:331 src/commandsAndMenu.tsx:337 src/commandsAndMenu.tsx:341 src/commandsAndMenu.tsx:347 src/commandsAndMenu.tsx:348 src/commandsAndMenu.tsx:353
+#: src/commandsAndMenu.tsx:314 src/commandsAndMenu.tsx:315 src/commandsAndMenu.tsx:316 src/commandsAndMenu.tsx:331 src/commandsAndMenu.tsx:337 src/commandsAndMenu.tsx:341 src/commandsAndMenu.tsx:347 src/commandsAndMenu.tsx:348 src/commandsAndMenu.tsx:353 src/commandsAndMenu.tsx:479
 msgid "Pushing…"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:314 src/commandsAndMenu.tsx:320 src/commandsAndMenu.tsx:324 src/commandsAndMenu.tsx:330 src/commandsAndMenu.tsx:331 src/commandsAndMenu.tsx:336
+#: src/commandsAndMenu.tsx:314 src/commandsAndMenu.tsx:320 src/commandsAndMenu.tsx:324 src/commandsAndMenu.tsx:330 src/commandsAndMenu.tsx:331 src/commandsAndMenu.tsx:336 src/commandsAndMenu.tsx:464
 msgid "Please select push options."
 msgstr ""
 
-#: src/commandsAndMenu.tsx:318 src/commandsAndMenu.tsx:324 src/commandsAndMenu.tsx:328 src/commandsAndMenu.tsx:334 src/commandsAndMenu.tsx:335 src/commandsAndMenu.tsx:340 src/commandsAndMenu.tsx:433 src/commandsAndMenu.tsx:434 src/commandsAndMenu.tsx:450 src/commandsAndMenu.tsx:472 src/commandsAndMenu.tsx:476 src/commandsAndMenu.tsx:482 src/commandsAndMenu.tsx:483 src/commandsAndMenu.tsx:488
+#: src/commandsAndMenu.tsx:318 src/commandsAndMenu.tsx:324 src/commandsAndMenu.tsx:328 src/commandsAndMenu.tsx:334 src/commandsAndMenu.tsx:335 src/commandsAndMenu.tsx:340 src/commandsAndMenu.tsx:433 src/commandsAndMenu.tsx:434 src/commandsAndMenu.tsx:450 src/commandsAndMenu.tsx:468 src/commandsAndMenu.tsx:472 src/commandsAndMenu.tsx:476 src/commandsAndMenu.tsx:482 src/commandsAndMenu.tsx:483 src/commandsAndMenu.tsx:488 src/commandsAndMenu.tsx:625
 msgid "Proceed"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:323 src/commandsAndMenu.tsx:324 src/commandsAndMenu.tsx:325 src/commandsAndMenu.tsx:341 src/commandsAndMenu.tsx:347 src/commandsAndMenu.tsx:351 src/commandsAndMenu.tsx:357 src/commandsAndMenu.tsx:358 src/commandsAndMenu.tsx:360 src/commandsAndMenu.tsx:362 src/commandsAndMenu.tsx:363 src/commandsAndMenu.tsx:366 src/commandsAndMenu.tsx:367 src/commandsAndMenu.tsx:370
+#: src/commandsAndMenu.tsx:323 src/commandsAndMenu.tsx:324 src/commandsAndMenu.tsx:325 src/commandsAndMenu.tsx:341 src/commandsAndMenu.tsx:347 src/commandsAndMenu.tsx:351 src/commandsAndMenu.tsx:357 src/commandsAndMenu.tsx:358 src/commandsAndMenu.tsx:360 src/commandsAndMenu.tsx:362 src/commandsAndMenu.tsx:363 src/commandsAndMenu.tsx:366 src/commandsAndMenu.tsx:367 src/commandsAndMenu.tsx:370 src/commandsAndMenu.tsx:491
 msgid "Successfully pushed"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:329 src/commandsAndMenu.tsx:330 src/commandsAndMenu.tsx:331 src/commandsAndMenu.tsx:347 src/commandsAndMenu.tsx:354 src/commandsAndMenu.tsx:358 src/commandsAndMenu.tsx:364 src/commandsAndMenu.tsx:365 src/commandsAndMenu.tsx:366 src/commandsAndMenu.tsx:368 src/commandsAndMenu.tsx:370 src/commandsAndMenu.tsx:372 src/commandsAndMenu.tsx:373 src/commandsAndMenu.tsx:376
+#: src/commandsAndMenu.tsx:329 src/commandsAndMenu.tsx:330 src/commandsAndMenu.tsx:331 src/commandsAndMenu.tsx:347 src/commandsAndMenu.tsx:354 src/commandsAndMenu.tsx:358 src/commandsAndMenu.tsx:364 src/commandsAndMenu.tsx:365 src/commandsAndMenu.tsx:366 src/commandsAndMenu.tsx:368 src/commandsAndMenu.tsx:370 src/commandsAndMenu.tsx:372 src/commandsAndMenu.tsx:373 src/commandsAndMenu.tsx:376 src/commandsAndMenu.tsx:498
 msgid "Encountered an error when pushing changes. Error: "
 msgstr ""
 
-#: src/commandsAndMenu.tsx:333 src/commandsAndMenu.tsx:334 src/commandsAndMenu.tsx:335 src/commandsAndMenu.tsx:351 src/commandsAndMenu.tsx:358 src/commandsAndMenu.tsx:362 src/commandsAndMenu.tsx:368 src/commandsAndMenu.tsx:369 src/commandsAndMenu.tsx:370 src/commandsAndMenu.tsx:372 src/commandsAndMenu.tsx:374 src/commandsAndMenu.tsx:376 src/commandsAndMenu.tsx:377 src/commandsAndMenu.tsx:380
+#: src/commandsAndMenu.tsx:333 src/commandsAndMenu.tsx:334 src/commandsAndMenu.tsx:335 src/commandsAndMenu.tsx:351 src/commandsAndMenu.tsx:358 src/commandsAndMenu.tsx:362 src/commandsAndMenu.tsx:368 src/commandsAndMenu.tsx:369 src/commandsAndMenu.tsx:370 src/commandsAndMenu.tsx:372 src/commandsAndMenu.tsx:374 src/commandsAndMenu.tsx:376 src/commandsAndMenu.tsx:377 src/commandsAndMenu.tsx:380 src/commandsAndMenu.tsx:502
 msgid "Failed to push"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:345 src/commandsAndMenu.tsx:346 src/commandsAndMenu.tsx:347 src/commandsAndMenu.tsx:363 src/commandsAndMenu.tsx:377 src/commandsAndMenu.tsx:381 src/commandsAndMenu.tsx:387 src/commandsAndMenu.tsx:388 src/commandsAndMenu.tsx:393
+#: src/commandsAndMenu.tsx:345 src/commandsAndMenu.tsx:346 src/commandsAndMenu.tsx:347 src/commandsAndMenu.tsx:363 src/commandsAndMenu.tsx:377 src/commandsAndMenu.tsx:381 src/commandsAndMenu.tsx:387 src/commandsAndMenu.tsx:388 src/commandsAndMenu.tsx:393 src/commandsAndMenu.tsx:527
 msgid "Pull from Remote (Force)"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:346 src/commandsAndMenu.tsx:347 src/commandsAndMenu.tsx:348 src/commandsAndMenu.tsx:364 src/commandsAndMenu.tsx:378 src/commandsAndMenu.tsx:380 src/commandsAndMenu.tsx:382 src/commandsAndMenu.tsx:386 src/commandsAndMenu.tsx:387 src/commandsAndMenu.tsx:388 src/commandsAndMenu.tsx:389 src/commandsAndMenu.tsx:390 src/commandsAndMenu.tsx:394
+#: src/commandsAndMenu.tsx:346 src/commandsAndMenu.tsx:347 src/commandsAndMenu.tsx:348 src/commandsAndMenu.tsx:364 src/commandsAndMenu.tsx:378 src/commandsAndMenu.tsx:380 src/commandsAndMenu.tsx:382 src/commandsAndMenu.tsx:386 src/commandsAndMenu.tsx:387 src/commandsAndMenu.tsx:388 src/commandsAndMenu.tsx:389 src/commandsAndMenu.tsx:390 src/commandsAndMenu.tsx:394 src/commandsAndMenu.tsx:528
 msgid "Pull from Remote"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:349 src/commandsAndMenu.tsx:350 src/commandsAndMenu.tsx:351 src/commandsAndMenu.tsx:367 src/commandsAndMenu.tsx:381 src/commandsAndMenu.tsx:385 src/commandsAndMenu.tsx:391 src/commandsAndMenu.tsx:392 src/commandsAndMenu.tsx:397
+#: src/commandsAndMenu.tsx:349 src/commandsAndMenu.tsx:350 src/commandsAndMenu.tsx:351 src/commandsAndMenu.tsx:367 src/commandsAndMenu.tsx:381 src/commandsAndMenu.tsx:385 src/commandsAndMenu.tsx:391 src/commandsAndMenu.tsx:392 src/commandsAndMenu.tsx:397 src/commandsAndMenu.tsx:531
 msgid "Discard all current changes and pull from remote repository"
 msgstr ""
 
 #: src/commandsAndMenu.tsx:351 src/commandsAndMenu.tsx:353 src/commandsAndMenu.tsx:357 src/commandsAndMenu.tsx:358 src/commandsAndMenu.tsx:361
 msgid "Pushing..."
 msgstr ""
 
-#: src/commandsAndMenu.tsx:352 src/commandsAndMenu.tsx:353 src/commandsAndMenu.tsx:354 src/commandsAndMenu.tsx:370 src/commandsAndMenu.tsx:381 src/commandsAndMenu.tsx:383 src/commandsAndMenu.tsx:384 src/commandsAndMenu.tsx:387 src/commandsAndMenu.tsx:388 src/commandsAndMenu.tsx:391 src/commandsAndMenu.tsx:394 src/commandsAndMenu.tsx:395 src/commandsAndMenu.tsx:400
+#: src/commandsAndMenu.tsx:352 src/commandsAndMenu.tsx:353 src/commandsAndMenu.tsx:354 src/commandsAndMenu.tsx:370 src/commandsAndMenu.tsx:381 src/commandsAndMenu.tsx:383 src/commandsAndMenu.tsx:384 src/commandsAndMenu.tsx:387 src/commandsAndMenu.tsx:388 src/commandsAndMenu.tsx:391 src/commandsAndMenu.tsx:394 src/commandsAndMenu.tsx:395 src/commandsAndMenu.tsx:400 src/commandsAndMenu.tsx:534
 msgid "Pull latest code from remote repository"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:361 src/commandsAndMenu.tsx:362 src/commandsAndMenu.tsx:363 src/commandsAndMenu.tsx:379 src/commandsAndMenu.tsx:393 src/commandsAndMenu.tsx:397 src/commandsAndMenu.tsx:403 src/commandsAndMenu.tsx:404 src/commandsAndMenu.tsx:409
+#: src/commandsAndMenu.tsx:361 src/commandsAndMenu.tsx:362 src/commandsAndMenu.tsx:363 src/commandsAndMenu.tsx:379 src/commandsAndMenu.tsx:393 src/commandsAndMenu.tsx:397 src/commandsAndMenu.tsx:403 src/commandsAndMenu.tsx:404 src/commandsAndMenu.tsx:409 src/commandsAndMenu.tsx:542
 msgid "Pulling…"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:369 src/commandsAndMenu.tsx:370 src/commandsAndMenu.tsx:371 src/commandsAndMenu.tsx:387 src/commandsAndMenu.tsx:395 src/commandsAndMenu.tsx:397 src/commandsAndMenu.tsx:401 src/commandsAndMenu.tsx:402 src/commandsAndMenu.tsx:405 src/commandsAndMenu.tsx:411 src/commandsAndMenu.tsx:412 src/commandsAndMenu.tsx:417
+#: src/commandsAndMenu.tsx:369
+msgid "Saves .gitignore"
+msgstr ""
+
+#: src/commandsAndMenu.tsx:369 src/commandsAndMenu.tsx:370 src/commandsAndMenu.tsx:371 src/commandsAndMenu.tsx:387 src/commandsAndMenu.tsx:395 src/commandsAndMenu.tsx:397 src/commandsAndMenu.tsx:401 src/commandsAndMenu.tsx:402 src/commandsAndMenu.tsx:405 src/commandsAndMenu.tsx:411 src/commandsAndMenu.tsx:412 src/commandsAndMenu.tsx:417 src/commandsAndMenu.tsx:552
 msgid "Successfully pulled"
 msgstr ""
 
 #: src/commandsAndMenu.tsx:386 src/commandsAndMenu.tsx:388 src/commandsAndMenu.tsx:392 src/commandsAndMenu.tsx:393 src/commandsAndMenu.tsx:396
 msgid "Pulling..."
 msgstr ""
 
-#: src/commandsAndMenu.tsx:403 src/commandsAndMenu.tsx:404 src/commandsAndMenu.tsx:405 src/commandsAndMenu.tsx:407 src/commandsAndMenu.tsx:411 src/commandsAndMenu.tsx:412 src/commandsAndMenu.tsx:415 src/commandsAndMenu.tsx:421 src/commandsAndMenu.tsx:436 src/commandsAndMenu.tsx:440 src/commandsAndMenu.tsx:446 src/commandsAndMenu.tsx:447 src/commandsAndMenu.tsx:452
+#: src/commandsAndMenu.tsx:388
+msgid "Warning: The .gitignore file is a hidden file."
+msgstr ""
+
+#: src/commandsAndMenu.tsx:391
+msgid "Hidden files by default cannot be accessed with the regular code editor. In order to open the .gitignore file you must:"
+msgstr ""
+
+#: src/commandsAndMenu.tsx:396
+msgid "Print the command below to create a jupyter_server_config.py file with defaults commented out. If you already have the file located in .jupyter, skip this step."
+msgstr ""
+
+#: src/commandsAndMenu.tsx:403 src/commandsAndMenu.tsx:404 src/commandsAndMenu.tsx:405 src/commandsAndMenu.tsx:407 src/commandsAndMenu.tsx:411 src/commandsAndMenu.tsx:412 src/commandsAndMenu.tsx:415 src/commandsAndMenu.tsx:421 src/commandsAndMenu.tsx:436 src/commandsAndMenu.tsx:440 src/commandsAndMenu.tsx:446 src/commandsAndMenu.tsx:447 src/commandsAndMenu.tsx:452 src/commandsAndMenu.tsx:584
 msgid "Failed to pull"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:416 src/commandsAndMenu.tsx:417 src/commandsAndMenu.tsx:421 src/commandsAndMenu.tsx:422 src/commandsAndMenu.tsx:433 src/commandsAndMenu.tsx:438 src/commandsAndMenu.tsx:455 src/commandsAndMenu.tsx:459 src/commandsAndMenu.tsx:460 src/commandsAndMenu.tsx:464 src/commandsAndMenu.tsx:465 src/commandsAndMenu.tsx:466 src/commandsAndMenu.tsx:470 src/commandsAndMenu.tsx:471 src/commandsAndMenu.tsx:476
+#: src/commandsAndMenu.tsx:404
+msgid "Open jupyter_server_config.py, uncomment out the following line and set it to True:"
+msgstr ""
+
+#: src/commandsAndMenu.tsx:416
+msgid "Show .gitignore file anyways"
+msgstr ""
+
+#: src/commandsAndMenu.tsx:416 src/commandsAndMenu.tsx:417 src/commandsAndMenu.tsx:421 src/commandsAndMenu.tsx:422 src/commandsAndMenu.tsx:433 src/commandsAndMenu.tsx:438 src/commandsAndMenu.tsx:455 src/commandsAndMenu.tsx:459 src/commandsAndMenu.tsx:460 src/commandsAndMenu.tsx:464 src/commandsAndMenu.tsx:465 src/commandsAndMenu.tsx:466 src/commandsAndMenu.tsx:470 src/commandsAndMenu.tsx:471 src/commandsAndMenu.tsx:476 src/commandsAndMenu.tsx:608 src/commandsAndMenu.tsx:613
 msgid "Reset to Remote"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:417 src/commandsAndMenu.tsx:418 src/commandsAndMenu.tsx:434 src/commandsAndMenu.tsx:456 src/commandsAndMenu.tsx:460 src/commandsAndMenu.tsx:466 src/commandsAndMenu.tsx:467 src/commandsAndMenu.tsx:472
+#: src/commandsAndMenu.tsx:417 src/commandsAndMenu.tsx:418 src/commandsAndMenu.tsx:434 src/commandsAndMenu.tsx:456 src/commandsAndMenu.tsx:460 src/commandsAndMenu.tsx:466 src/commandsAndMenu.tsx:467 src/commandsAndMenu.tsx:472 src/commandsAndMenu.tsx:609
 msgid "Reset Current Branch to Remote State"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:421 src/commandsAndMenu.tsx:422 src/commandsAndMenu.tsx:423 src/commandsAndMenu.tsx:427 src/commandsAndMenu.tsx:428 src/commandsAndMenu.tsx:432 src/commandsAndMenu.tsx:481 src/commandsAndMenu.tsx:482 src/commandsAndMenu.tsx:498 src/commandsAndMenu.tsx:520 src/commandsAndMenu.tsx:524 src/commandsAndMenu.tsx:530 src/commandsAndMenu.tsx:531 src/commandsAndMenu.tsx:536
+#: src/commandsAndMenu.tsx:419
+msgid "Do not show this warning again"
+msgstr ""
+
+#: src/commandsAndMenu.tsx:421 src/commandsAndMenu.tsx:422 src/commandsAndMenu.tsx:423 src/commandsAndMenu.tsx:427 src/commandsAndMenu.tsx:428 src/commandsAndMenu.tsx:432 src/commandsAndMenu.tsx:481 src/commandsAndMenu.tsx:482 src/commandsAndMenu.tsx:498 src/commandsAndMenu.tsx:520 src/commandsAndMenu.tsx:524 src/commandsAndMenu.tsx:530 src/commandsAndMenu.tsx:531 src/commandsAndMenu.tsx:536 src/commandsAndMenu.tsx:690
 msgid "Show Diff"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:422 src/commandsAndMenu.tsx:423 src/commandsAndMenu.tsx:424 src/commandsAndMenu.tsx:428 src/commandsAndMenu.tsx:429 src/commandsAndMenu.tsx:433 src/commandsAndMenu.tsx:482 src/commandsAndMenu.tsx:483 src/commandsAndMenu.tsx:499 src/commandsAndMenu.tsx:521 src/commandsAndMenu.tsx:525 src/commandsAndMenu.tsx:531 src/commandsAndMenu.tsx:532 src/commandsAndMenu.tsx:537
+#: src/commandsAndMenu.tsx:422 src/commandsAndMenu.tsx:423 src/commandsAndMenu.tsx:424 src/commandsAndMenu.tsx:428 src/commandsAndMenu.tsx:429 src/commandsAndMenu.tsx:433 src/commandsAndMenu.tsx:482 src/commandsAndMenu.tsx:483 src/commandsAndMenu.tsx:499 src/commandsAndMenu.tsx:521 src/commandsAndMenu.tsx:525 src/commandsAndMenu.tsx:531 src/commandsAndMenu.tsx:532 src/commandsAndMenu.tsx:537 src/commandsAndMenu.tsx:691
 msgid "Display a file diff."
 msgstr ""
 
-#: src/commandsAndMenu.tsx:423 src/commandsAndMenu.tsx:424 src/commandsAndMenu.tsx:440 src/commandsAndMenu.tsx:462 src/commandsAndMenu.tsx:466 src/commandsAndMenu.tsx:472 src/commandsAndMenu.tsx:473 src/commandsAndMenu.tsx:478
+#: src/commandsAndMenu.tsx:423 src/commandsAndMenu.tsx:424 src/commandsAndMenu.tsx:440 src/commandsAndMenu.tsx:462 src/commandsAndMenu.tsx:466 src/commandsAndMenu.tsx:472 src/commandsAndMenu.tsx:473 src/commandsAndMenu.tsx:478 src/commandsAndMenu.tsx:615
 msgid "To bring the current branch to the state of its corresponding remote tracking branch,             a hard reset will be performed, which may result in some files being permanently deleted             and some changes being permanently discarded. Are you sure you want to proceed?             This action cannot be undone."
 msgstr ""
 
-#: src/commandsAndMenu.tsx:429 src/commandsAndMenu.tsx:430 src/commandsAndMenu.tsx:446 src/commandsAndMenu.tsx:468 src/commandsAndMenu.tsx:472 src/commandsAndMenu.tsx:478 src/commandsAndMenu.tsx:479 src/commandsAndMenu.tsx:484
+#: src/commandsAndMenu.tsx:429 src/commandsAndMenu.tsx:430 src/commandsAndMenu.tsx:446 src/commandsAndMenu.tsx:468 src/commandsAndMenu.tsx:472 src/commandsAndMenu.tsx:478 src/commandsAndMenu.tsx:479 src/commandsAndMenu.tsx:484 src/commandsAndMenu.tsx:621
 msgid "Close all opened files to avoid conflicts"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:440 src/commandsAndMenu.tsx:441 src/commandsAndMenu.tsx:457 src/commandsAndMenu.tsx:479 src/commandsAndMenu.tsx:483 src/commandsAndMenu.tsx:489 src/commandsAndMenu.tsx:490 src/commandsAndMenu.tsx:495
+#: src/commandsAndMenu.tsx:440 src/commandsAndMenu.tsx:441 src/commandsAndMenu.tsx:457 src/commandsAndMenu.tsx:479 src/commandsAndMenu.tsx:483 src/commandsAndMenu.tsx:489 src/commandsAndMenu.tsx:490 src/commandsAndMenu.tsx:495 src/commandsAndMenu.tsx:633
 msgid "Closing all opened files..."
 msgstr ""
 
-#: src/commandsAndMenu.tsx:446 src/commandsAndMenu.tsx:447 src/commandsAndMenu.tsx:463 src/commandsAndMenu.tsx:485 src/commandsAndMenu.tsx:489 src/commandsAndMenu.tsx:495 src/commandsAndMenu.tsx:496 src/commandsAndMenu.tsx:501
+#: src/commandsAndMenu.tsx:446 src/commandsAndMenu.tsx:447 src/commandsAndMenu.tsx:463 src/commandsAndMenu.tsx:485 src/commandsAndMenu.tsx:489 src/commandsAndMenu.tsx:495 src/commandsAndMenu.tsx:496 src/commandsAndMenu.tsx:501 src/commandsAndMenu.tsx:638
 msgid "Resetting..."
 msgstr ""
 
-#: src/commandsAndMenu.tsx:451 src/commandsAndMenu.tsx:452 src/commandsAndMenu.tsx:468 src/commandsAndMenu.tsx:490 src/commandsAndMenu.tsx:494 src/commandsAndMenu.tsx:500 src/commandsAndMenu.tsx:501 src/commandsAndMenu.tsx:506
+#: src/commandsAndMenu.tsx:451 src/commandsAndMenu.tsx:452 src/commandsAndMenu.tsx:468 src/commandsAndMenu.tsx:490 src/commandsAndMenu.tsx:494 src/commandsAndMenu.tsx:500 src/commandsAndMenu.tsx:501 src/commandsAndMenu.tsx:506 src/commandsAndMenu.tsx:650
 msgid "Successfully reset"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:453 src/commandsAndMenu.tsx:454 src/commandsAndMenu.tsx:470 src/commandsAndMenu.tsx:492 src/commandsAndMenu.tsx:496 src/commandsAndMenu.tsx:502 src/commandsAndMenu.tsx:503 src/commandsAndMenu.tsx:508
+#: src/commandsAndMenu.tsx:453 src/commandsAndMenu.tsx:454 src/commandsAndMenu.tsx:470 src/commandsAndMenu.tsx:492 src/commandsAndMenu.tsx:496 src/commandsAndMenu.tsx:502 src/commandsAndMenu.tsx:503 src/commandsAndMenu.tsx:508 src/commandsAndMenu.tsx:653
 msgid "Successfully reset the current branch to its remote state"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:463 src/commandsAndMenu.tsx:464 src/commandsAndMenu.tsx:480 src/commandsAndMenu.tsx:502 src/commandsAndMenu.tsx:506 src/commandsAndMenu.tsx:512 src/commandsAndMenu.tsx:513 src/commandsAndMenu.tsx:518
+#: src/commandsAndMenu.tsx:463 src/commandsAndMenu.tsx:464 src/commandsAndMenu.tsx:480 src/commandsAndMenu.tsx:502 src/commandsAndMenu.tsx:506 src/commandsAndMenu.tsx:512 src/commandsAndMenu.tsx:513 src/commandsAndMenu.tsx:518 src/commandsAndMenu.tsx:664
 msgid "Reset failed"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:468 src/commandsAndMenu.tsx:470 src/commandsAndMenu.tsx:474 src/commandsAndMenu.tsx:475 src/commandsAndMenu.tsx:519 src/commandsAndMenu.tsx:529 src/commandsAndMenu.tsx:578 src/commandsAndMenu.tsx:579 src/commandsAndMenu.tsx:580 src/commandsAndMenu.tsx:596 src/commandsAndMenu.tsx:618 src/commandsAndMenu.tsx:622 src/commandsAndMenu.tsx:643 src/commandsAndMenu.tsx:644 src/commandsAndMenu.tsx:649
+#: src/commandsAndMenu.tsx:468 src/commandsAndMenu.tsx:470 src/commandsAndMenu.tsx:474 src/commandsAndMenu.tsx:475 src/commandsAndMenu.tsx:519 src/commandsAndMenu.tsx:529 src/commandsAndMenu.tsx:578 src/commandsAndMenu.tsx:579 src/commandsAndMenu.tsx:580 src/commandsAndMenu.tsx:596 src/commandsAndMenu.tsx:618 src/commandsAndMenu.tsx:622 src/commandsAndMenu.tsx:643 src/commandsAndMenu.tsx:644 src/commandsAndMenu.tsx:649 src/commandsAndMenu.tsx:811
 msgid "Refresh"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:473 src/commandsAndMenu.tsx:475 src/commandsAndMenu.tsx:479 src/commandsAndMenu.tsx:480 src/commandsAndMenu.tsx:524 src/commandsAndMenu.tsx:534 src/commandsAndMenu.tsx:583 src/commandsAndMenu.tsx:584 src/commandsAndMenu.tsx:585 src/commandsAndMenu.tsx:601 src/commandsAndMenu.tsx:623 src/commandsAndMenu.tsx:627 src/commandsAndMenu.tsx:648 src/commandsAndMenu.tsx:649 src/commandsAndMenu.tsx:654
+#: src/commandsAndMenu.tsx:473 src/commandsAndMenu.tsx:475 src/commandsAndMenu.tsx:479 src/commandsAndMenu.tsx:480 src/commandsAndMenu.tsx:524 src/commandsAndMenu.tsx:534 src/commandsAndMenu.tsx:583 src/commandsAndMenu.tsx:584 src/commandsAndMenu.tsx:585 src/commandsAndMenu.tsx:601 src/commandsAndMenu.tsx:623 src/commandsAndMenu.tsx:627 src/commandsAndMenu.tsx:648 src/commandsAndMenu.tsx:649 src/commandsAndMenu.tsx:654 src/commandsAndMenu.tsx:816
 msgid "Refresh diff widget"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:480 src/commandsAndMenu.tsx:490 src/commandsAndMenu.tsx:539 src/commandsAndMenu.tsx:540 src/commandsAndMenu.tsx:541 src/commandsAndMenu.tsx:557 src/commandsAndMenu.tsx:579 src/commandsAndMenu.tsx:583 src/commandsAndMenu.tsx:604 src/commandsAndMenu.tsx:605 src/commandsAndMenu.tsx:610
+#: src/commandsAndMenu.tsx:480 src/commandsAndMenu.tsx:490 src/commandsAndMenu.tsx:539 src/commandsAndMenu.tsx:540 src/commandsAndMenu.tsx:541 src/commandsAndMenu.tsx:557 src/commandsAndMenu.tsx:579 src/commandsAndMenu.tsx:583 src/commandsAndMenu.tsx:604 src/commandsAndMenu.tsx:605 src/commandsAndMenu.tsx:610 src/commandsAndMenu.tsx:773
 msgid "Mark as resolved"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:484 src/commandsAndMenu.tsx:494 src/commandsAndMenu.tsx:543 src/commandsAndMenu.tsx:544 src/commandsAndMenu.tsx:545 src/commandsAndMenu.tsx:561 src/commandsAndMenu.tsx:583 src/commandsAndMenu.tsx:587 src/commandsAndMenu.tsx:608 src/commandsAndMenu.tsx:609 src/commandsAndMenu.tsx:614
+#: src/commandsAndMenu.tsx:484 src/commandsAndMenu.tsx:494 src/commandsAndMenu.tsx:543 src/commandsAndMenu.tsx:544 src/commandsAndMenu.tsx:545 src/commandsAndMenu.tsx:561 src/commandsAndMenu.tsx:583 src/commandsAndMenu.tsx:587 src/commandsAndMenu.tsx:608 src/commandsAndMenu.tsx:609 src/commandsAndMenu.tsx:614 src/commandsAndMenu.tsx:777
 msgid "Resolve with conflicts"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:485 src/commandsAndMenu.tsx:495 src/commandsAndMenu.tsx:544 src/commandsAndMenu.tsx:545 src/commandsAndMenu.tsx:546 src/commandsAndMenu.tsx:562 src/commandsAndMenu.tsx:584 src/commandsAndMenu.tsx:588 src/commandsAndMenu.tsx:609 src/commandsAndMenu.tsx:610 src/commandsAndMenu.tsx:615
+#: src/commandsAndMenu.tsx:485 src/commandsAndMenu.tsx:495 src/commandsAndMenu.tsx:544 src/commandsAndMenu.tsx:545 src/commandsAndMenu.tsx:546 src/commandsAndMenu.tsx:562 src/commandsAndMenu.tsx:584 src/commandsAndMenu.tsx:588 src/commandsAndMenu.tsx:609 src/commandsAndMenu.tsx:610 src/commandsAndMenu.tsx:615 src/commandsAndMenu.tsx:778
 msgid "Are you sure you want to mark this file as resolved with merge conflicts?"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:496 src/commandsAndMenu.tsx:498 src/commandsAndMenu.tsx:503 src/commandsAndMenu.tsx:507 src/commandsAndMenu.tsx:508 src/commandsAndMenu.tsx:554 src/commandsAndMenu.tsx:564 src/commandsAndMenu.tsx:613 src/commandsAndMenu.tsx:614 src/commandsAndMenu.tsx:633 src/commandsAndMenu.tsx:649 src/commandsAndMenu.tsx:671 src/commandsAndMenu.tsx:675 src/commandsAndMenu.tsx:696 src/commandsAndMenu.tsx:697 src/commandsAndMenu.tsx:702
+#: src/commandsAndMenu.tsx:496 src/commandsAndMenu.tsx:498 src/commandsAndMenu.tsx:503 src/commandsAndMenu.tsx:507 src/commandsAndMenu.tsx:508 src/commandsAndMenu.tsx:554 src/commandsAndMenu.tsx:564 src/commandsAndMenu.tsx:613 src/commandsAndMenu.tsx:614 src/commandsAndMenu.tsx:633 src/commandsAndMenu.tsx:649 src/commandsAndMenu.tsx:671 src/commandsAndMenu.tsx:675 src/commandsAndMenu.tsx:696 src/commandsAndMenu.tsx:697 src/commandsAndMenu.tsx:702 src/commandsAndMenu.tsx:864
 msgid "Diff Not Supported"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:497 src/commandsAndMenu.tsx:499 src/commandsAndMenu.tsx:504 src/commandsAndMenu.tsx:508 src/commandsAndMenu.tsx:509 src/commandsAndMenu.tsx:555 src/commandsAndMenu.tsx:565 src/commandsAndMenu.tsx:614 src/commandsAndMenu.tsx:615 src/commandsAndMenu.tsx:634 src/commandsAndMenu.tsx:650 src/commandsAndMenu.tsx:672 src/commandsAndMenu.tsx:676 src/commandsAndMenu.tsx:697 src/commandsAndMenu.tsx:698 src/commandsAndMenu.tsx:703
+#: src/commandsAndMenu.tsx:497 src/commandsAndMenu.tsx:499 src/commandsAndMenu.tsx:504 src/commandsAndMenu.tsx:508 src/commandsAndMenu.tsx:509 src/commandsAndMenu.tsx:555 src/commandsAndMenu.tsx:565 src/commandsAndMenu.tsx:614 src/commandsAndMenu.tsx:615 src/commandsAndMenu.tsx:634 src/commandsAndMenu.tsx:650 src/commandsAndMenu.tsx:672 src/commandsAndMenu.tsx:676 src/commandsAndMenu.tsx:697 src/commandsAndMenu.tsx:698 src/commandsAndMenu.tsx:703 src/commandsAndMenu.tsx:865
 msgid "Diff is not supported for %1 files."
 msgstr ""
 
-#: src/commandsAndMenu.tsx:512 src/commandsAndMenu.tsx:522 src/commandsAndMenu.tsx:571 src/commandsAndMenu.tsx:572 src/commandsAndMenu.tsx:573 src/commandsAndMenu.tsx:589 src/commandsAndMenu.tsx:611 src/commandsAndMenu.tsx:615 src/commandsAndMenu.tsx:636 src/commandsAndMenu.tsx:637 src/commandsAndMenu.tsx:642
+#: src/commandsAndMenu.tsx:512 src/commandsAndMenu.tsx:522 src/commandsAndMenu.tsx:571 src/commandsAndMenu.tsx:572 src/commandsAndMenu.tsx:573 src/commandsAndMenu.tsx:589 src/commandsAndMenu.tsx:611 src/commandsAndMenu.tsx:615 src/commandsAndMenu.tsx:636 src/commandsAndMenu.tsx:637 src/commandsAndMenu.tsx:642 src/commandsAndMenu.tsx:804
 msgid "Mark file as resolved"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:568 src/commandsAndMenu.tsx:627 src/commandsAndMenu.tsx:628 src/commandsAndMenu.tsx:647 src/commandsAndMenu.tsx:663 src/commandsAndMenu.tsx:685 src/commandsAndMenu.tsx:689 src/commandsAndMenu.tsx:710 src/commandsAndMenu.tsx:711 src/commandsAndMenu.tsx:716
+#: src/commandsAndMenu.tsx:568 src/commandsAndMenu.tsx:627 src/commandsAndMenu.tsx:628 src/commandsAndMenu.tsx:647 src/commandsAndMenu.tsx:663 src/commandsAndMenu.tsx:685 src/commandsAndMenu.tsx:689 src/commandsAndMenu.tsx:710 src/commandsAndMenu.tsx:711 src/commandsAndMenu.tsx:716 src/commandsAndMenu.tsx:878
 msgid "Merge Branch…"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:569 src/commandsAndMenu.tsx:628 src/commandsAndMenu.tsx:629 src/commandsAndMenu.tsx:648 src/commandsAndMenu.tsx:664 src/commandsAndMenu.tsx:686 src/commandsAndMenu.tsx:690 src/commandsAndMenu.tsx:711 src/commandsAndMenu.tsx:712 src/commandsAndMenu.tsx:717
+#: src/commandsAndMenu.tsx:569 src/commandsAndMenu.tsx:628 src/commandsAndMenu.tsx:629 src/commandsAndMenu.tsx:648 src/commandsAndMenu.tsx:664 src/commandsAndMenu.tsx:686 src/commandsAndMenu.tsx:690 src/commandsAndMenu.tsx:711 src/commandsAndMenu.tsx:712 src/commandsAndMenu.tsx:717 src/commandsAndMenu.tsx:879
 msgid "Merge selected branch in the current branch"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:608 src/commandsAndMenu.tsx:667 src/commandsAndMenu.tsx:668 src/commandsAndMenu.tsx:687 src/commandsAndMenu.tsx:703 src/commandsAndMenu.tsx:725 src/commandsAndMenu.tsx:729 src/commandsAndMenu.tsx:750 src/commandsAndMenu.tsx:752 src/commandsAndMenu.tsx:757
+#: src/commandsAndMenu.tsx:608 src/commandsAndMenu.tsx:667 src/commandsAndMenu.tsx:668 src/commandsAndMenu.tsx:687 src/commandsAndMenu.tsx:703 src/commandsAndMenu.tsx:725 src/commandsAndMenu.tsx:729 src/commandsAndMenu.tsx:750 src/commandsAndMenu.tsx:752 src/commandsAndMenu.tsx:757 src/commandsAndMenu.tsx:918
 msgid "Merging branch '%1'…"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:615 src/commandsAndMenu.tsx:674 src/commandsAndMenu.tsx:675 src/commandsAndMenu.tsx:694 src/commandsAndMenu.tsx:710 src/commandsAndMenu.tsx:732 src/commandsAndMenu.tsx:736 src/commandsAndMenu.tsx:757 src/commandsAndMenu.tsx:759 src/commandsAndMenu.tsx:764
+#: src/commandsAndMenu.tsx:615 src/commandsAndMenu.tsx:674 src/commandsAndMenu.tsx:675 src/commandsAndMenu.tsx:694 src/commandsAndMenu.tsx:710 src/commandsAndMenu.tsx:732 src/commandsAndMenu.tsx:736 src/commandsAndMenu.tsx:757 src/commandsAndMenu.tsx:759 src/commandsAndMenu.tsx:764 src/commandsAndMenu.tsx:927
 msgid "Failed to merge branch '%1' into '%2'."
 msgstr ""
 
-#: src/commandsAndMenu.tsx:627 src/commandsAndMenu.tsx:686 src/commandsAndMenu.tsx:687 src/commandsAndMenu.tsx:706 src/commandsAndMenu.tsx:722 src/commandsAndMenu.tsx:744 src/commandsAndMenu.tsx:748 src/commandsAndMenu.tsx:769 src/commandsAndMenu.tsx:771 src/commandsAndMenu.tsx:776
+#: src/commandsAndMenu.tsx:627 src/commandsAndMenu.tsx:686 src/commandsAndMenu.tsx:687 src/commandsAndMenu.tsx:706 src/commandsAndMenu.tsx:722 src/commandsAndMenu.tsx:744 src/commandsAndMenu.tsx:748 src/commandsAndMenu.tsx:769 src/commandsAndMenu.tsx:771 src/commandsAndMenu.tsx:776 src/commandsAndMenu.tsx:940
 msgid "Branch '%1' merged into '%2'."
 msgstr ""
 
 #: src/commandsAndMenu.tsx:704
 msgid "CURRENT"
 msgstr ""
 
@@ -757,275 +915,175 @@
 msgid "RESULT"
 msgstr ""
 
 #: src/commandsAndMenu.tsx:755 src/commandsAndMenu.tsx:757 src/commandsAndMenu.tsx:763 src/commandsAndMenu.tsx:768 src/commandsAndMenu.tsx:788 src/commandsAndMenu.tsx:789 src/commandsAndMenu.tsx:810 src/commandsAndMenu.tsx:812 src/commandsAndMenu.tsx:818 src/commandsAndMenu.tsx:823 src/commandsAndMenu.tsx:843 src/commandsAndMenu.tsx:844 src/commandsAndMenu.tsx:890 src/commandsAndMenu.tsx:945 src/components/Alert.tsx:123 src/index.ts:128 src/index.ts:132 src/index.ts:134
 msgid "DISMISS"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:786 src/commandsAndMenu.tsx:791
+#: src/commandsAndMenu.tsx:786 src/commandsAndMenu.tsx:791 src/commandsAndMenu.tsx:955
 msgid "Rebase branch…"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:787 src/commandsAndMenu.tsx:792
+#: src/commandsAndMenu.tsx:787 src/commandsAndMenu.tsx:792 src/commandsAndMenu.tsx:956
 msgid "Rebase current branch onto the selected branch"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:827 src/commandsAndMenu.tsx:832
+#: src/commandsAndMenu.tsx:827 src/commandsAndMenu.tsx:832 src/commandsAndMenu.tsx:995
 msgid "Rebasing current branch onto '%1'…"
 msgstr ""
 
-#: src/commandsAndMenu.tsx:834 src/commandsAndMenu.tsx:839
-msgid "Failed to rebase branch '%1' onto '%2'."
-msgstr ""
-
-#: src/commandsAndMenu.tsx:846 src/commandsAndMenu.tsx:851
-msgid "Branch '%1' rebase onto '%2'."
-msgstr ""
-
-#: src/commandsAndMenu.tsx:864 src/commandsAndMenu.tsx:869
-msgid "Continue rebase"
-msgstr ""
-
-#: src/commandsAndMenu.tsx:866 src/commandsAndMenu.tsx:871
-msgid "Skip current commit"
-msgstr ""
-
-#: src/commandsAndMenu.tsx:868 src/commandsAndMenu.tsx:873 src/components/RebaseAction.tsx:76
-msgid "Abort rebase"
-msgstr ""
-
-#: src/commandsAndMenu.tsx:870 src/commandsAndMenu.tsx:875 src/commandsAndMenu.tsx:884 src/commandsAndMenu.tsx:889
-msgid "Resolve rebase"
-msgstr ""
-
-#: src/commandsAndMenu.tsx:876 src/commandsAndMenu.tsx:881
-msgid "Continue the rebase by committing the current state."
-msgstr ""
-
-#: src/commandsAndMenu.tsx:880 src/commandsAndMenu.tsx:885
-msgid "Skip current commit and continue the rebase."
-msgstr ""
-
-#: src/commandsAndMenu.tsx:882 src/commandsAndMenu.tsx:887
-msgid "Abort the rebase"
-msgstr ""
-
-#: src/commandsAndMenu.tsx:894 src/commandsAndMenu.tsx:899
-msgid "Continue the rebase…"
-msgstr ""
-
-#: src/commandsAndMenu.tsx:896 src/commandsAndMenu.tsx:901
-msgid "Skip current commit…"
-msgstr ""
-
-#: src/commandsAndMenu.tsx:898 src/commandsAndMenu.tsx:903
-msgid "Abort the rebase…"
-msgstr ""
-
-#: src/commandsAndMenu.tsx:912 src/commandsAndMenu.tsx:917
-msgid "Fail to continue rebasing."
-msgstr ""
-
-#: src/commandsAndMenu.tsx:914 src/commandsAndMenu.tsx:919
-msgid "Fail to skip current commit when rebasing."
-msgstr ""
-
-#: src/commandsAndMenu.tsx:916 src/commandsAndMenu.tsx:921
-msgid "Fail to abort the rebase."
-msgstr ""
-
-#: src/commandsAndMenu.tsx:930 src/commandsAndMenu.tsx:935
-msgid "Commit submitted continuing rebase."
-msgstr ""
-
-#: src/commandsAndMenu.tsx:932 src/commandsAndMenu.tsx:937
-msgid "Current commit skipped."
-msgstr ""
-
-#: src/commandsAndMenu.tsx:934 src/commandsAndMenu.tsx:939
-msgid "Rebase aborted."
-msgstr ""
-
-#: src/commandsAndMenu.tsx:947 src/commandsAndMenu.tsx:952
-msgid "Stash Changes"
-msgstr ""
-
-#: src/commandsAndMenu.tsx:948 src/commandsAndMenu.tsx:953
-msgid "Stash all current changes"
-msgstr ""
-
-#: src/commandsAndMenu.tsx:953 src/commandsAndMenu.tsx:958
-msgid "Do you want to stash your changes? "
-msgstr ""
-
-#: src/commandsAndMenu.tsx:954 src/commandsAndMenu.tsx:959
-msgid "Stash message (optional)"
-msgstr ""
-
-#: src/commandsAndMenu.tsx:955 src/commandsAndMenu.tsx:960 src/components/GitStash.tsx:240
-msgid "Stash"
-msgstr ""
-
-#: src/commandsAndMenu.tsx:962 src/commandsAndMenu.tsx:967
-msgid "Stashing changes"
-msgstr ""
-
-#: src/commandsAndMenu.tsx:968 src/commandsAndMenu.tsx:973
-msgid "Successfully stashed"
-msgstr ""
-
-#: src/commandsAndMenu.tsx:986 src/commandsAndMenu.tsx:991
-msgid "Stash List"
-msgstr ""
-
-#: src/commandsAndMenu.tsx:987 src/commandsAndMenu.tsx:992
-msgid "Get all the stashed changes"
-msgstr ""
-
-#: src/commandsAndMenu.tsx:994 src/commandsAndMenu.tsx:999
-msgid "Got the stash list"
-msgstr ""
-
-#: src/components/Alert.tsx:105
+#: src/components/Alert.tsx:105 src/notifications.ts:21
 msgid "Error"
 msgstr ""
 
 #: src/components/Alert.tsx:110
 msgid "SHOW"
 msgstr ""
 
-#: src/components/Alert.tsx:110
+#: src/components/Alert.tsx:110 src/notifications.ts:19
 msgid "Show"
 msgstr ""
 
-#: src/components/Alert.tsx:120
+#: src/components/Alert.tsx:120 src/notifications.ts:52
 msgid "Detailed message"
 msgstr ""
 
-#: src/components/Alert.tsx:128
+#: src/components/Alert.tsx:128 src/notifications.ts:50
 msgid "Details"
 msgstr ""
 
 #: src/components/Alert.tsx:148
 msgid "(missing message)"
 msgstr ""
 
 #: src/components/BranchMenu.tsx:148 src/components/BranchMenu.tsx:154
 msgid "The current branch contains files with uncommitted changes. Please commit or discard these changes before switching to or creating another branch."
 msgstr ""
 
-#: src/components/BranchMenu.tsx:195 src/components/BranchMenu.tsx:201 src/components/BranchPicker.tsx:157 src/components/MergeBranchDialog.tsx:138 src/components/NewBranchDialog.tsx:177 src/components/NewBranchDialog.tsx:184 src/components/TagMenu.tsx:185 src/components/TagMenu.tsx:189
+#: src/components/BranchMenu.tsx:195 src/components/BranchMenu.tsx:201 src/components/BranchPicker.tsx:157 src/components/BranchPicker.tsx:159 src/components/MergeBranchDialog.tsx:138 src/components/NewBranchDialog.tsx:172 src/components/NewBranchDialog.tsx:177 src/components/NewBranchDialog.tsx:184 src/components/TagMenu.tsx:180 src/components/TagMenu.tsx:185 src/components/TagMenu.tsx:189
 msgid "Filter"
 msgstr ""
 
-#: src/components/BranchMenu.tsx:196 src/components/BranchMenu.tsx:202 src/components/NewBranchDialog.tsx:178 src/components/NewBranchDialog.tsx:185 src/components/TagMenu.tsx:190
+#: src/components/BranchMenu.tsx:196 src/components/BranchMenu.tsx:202 src/components/NewBranchDialog.tsx:173 src/components/NewBranchDialog.tsx:178 src/components/NewBranchDialog.tsx:185 src/components/TagMenu.tsx:190
 msgid "Filter branch menu"
 msgstr ""
 
-#: src/components/BranchMenu.tsx:201 src/components/BranchMenu.tsx:207 src/components/BranchPicker.tsx:163 src/components/MergeBranchDialog.tsx:144 src/components/NewBranchDialog.tsx:183 src/components/NewBranchDialog.tsx:190 src/components/NewTagDialog.tsx:443 src/components/NewTagDialog.tsx:458 src/components/TagMenu.tsx:191 src/components/TagMenu.tsx:195
+#: src/components/BranchMenu.tsx:201 src/components/BranchMenu.tsx:207 src/components/BranchPicker.tsx:163 src/components/BranchPicker.tsx:165 src/components/MergeBranchDialog.tsx:144 src/components/NewBranchDialog.tsx:178 src/components/NewBranchDialog.tsx:183 src/components/NewBranchDialog.tsx:190 src/components/NewTagDialog.tsx:443 src/components/NewTagDialog.tsx:453 src/components/NewTagDialog.tsx:458 src/components/TagMenu.tsx:186 src/components/TagMenu.tsx:191 src/components/TagMenu.tsx:195
 msgid "Clear the current filter"
 msgstr ""
 
-#: src/components/BranchMenu.tsx:211 src/components/BranchMenu.tsx:217 src/components/NewBranchDialog.tsx:208 src/components/NewBranchDialog.tsx:215
+#: src/components/BranchMenu.tsx:211 src/components/BranchMenu.tsx:217 src/components/NewBranchDialog.tsx:203 src/components/NewBranchDialog.tsx:208 src/components/NewBranchDialog.tsx:215
 msgid "Create a new branch"
 msgstr ""
 
 #: src/components/BranchMenu.tsx:212 src/components/BranchMenu.tsx:218
 msgid "New Branch"
 msgstr ""
 
-#: src/components/BranchMenu.tsx:261 src/components/BranchMenu.tsx:269 src/components/BranchMenu.tsx:276
+#: src/components/BranchMenu.tsx:261 src/components/BranchMenu.tsx:269 src/components/BranchMenu.tsx:270 src/components/BranchMenu.tsx:276
 msgid "Switch to branch: %1"
 msgstr ""
 
-#: src/components/BranchMenu.tsx:275 src/components/BranchMenu.tsx:286 src/components/BranchMenu.tsx:293
+#: src/components/BranchMenu.tsx:275 src/components/BranchMenu.tsx:286 src/components/BranchMenu.tsx:288 src/components/BranchMenu.tsx:293
 msgid "Delete this branch locally"
 msgstr ""
 
-#: src/components/BranchMenu.tsx:295 src/components/BranchMenu.tsx:302
+#: src/components/BranchMenu.tsx:295 src/components/BranchMenu.tsx:299 src/components/BranchMenu.tsx:302
 msgid "Merge this branch into the current one"
 msgstr ""
 
-#: src/components/BranchMenu.tsx:332 src/components/BranchMenu.tsx:355 src/components/BranchMenu.tsx:362
+#: src/components/BranchMenu.tsx:332 src/components/BranchMenu.tsx:355 src/components/BranchMenu.tsx:360 src/components/BranchMenu.tsx:362
 msgid "Delete branch"
 msgstr ""
 
-#: src/components/BranchMenu.tsx:335 src/components/BranchMenu.tsx:358 src/components/BranchMenu.tsx:365
+#: src/components/BranchMenu.tsx:335 src/components/BranchMenu.tsx:358 src/components/BranchMenu.tsx:363 src/components/BranchMenu.tsx:365
 msgid "Are you sure you want to permanently delete the branch "
 msgstr ""
 
-#: src/components/BranchMenu.tsx:340 src/components/BranchMenu.tsx:363 src/components/BranchMenu.tsx:370
+#: src/components/BranchMenu.tsx:340 src/components/BranchMenu.tsx:363 src/components/BranchMenu.tsx:368 src/components/BranchMenu.tsx:370
 msgid "This action cannot be undone."
 msgstr ""
 
-#: src/components/BranchMenu.tsx:366 src/components/BranchMenu.tsx:398 src/components/BranchMenu.tsx:405
+#: src/components/BranchMenu.tsx:366 src/components/BranchMenu.tsx:398 src/components/BranchMenu.tsx:403 src/components/BranchMenu.tsx:405
 msgid "Creating a new branch is disabled"
 msgstr ""
 
-#: src/components/BranchMenu.tsx:51 src/components/BranchMenu.tsx:52
+#: src/components/BranchMenu.tsx:439
+msgid "Switching branches is disabled"
+msgstr ""
+
+#: src/components/BranchMenu.tsx:449
+msgid "Switching branch…"
+msgstr ""
+
+#: src/components/BranchMenu.tsx:462
+msgid "Switched branch."
+msgstr ""
+
+#: src/components/BranchMenu.tsx:50 src/components/BranchMenu.tsx:51 src/components/BranchMenu.tsx:52
 msgid "Unable to switch branch"
 msgstr ""
 
-#: src/components/BranchMenu.tsx:55 src/components/BranchMenu.tsx:56 src/components/TagMenu.tsx:49 src/components/TagMenu.tsx:51
+#: src/components/BranchMenu.tsx:54 src/components/BranchMenu.tsx:55 src/components/BranchMenu.tsx:56 src/components/TagMenu.tsx:49 src/components/TagMenu.tsx:50 src/components/TagMenu.tsx:51
 msgid "Your changes to the following files would be overwritten by switching:"
 msgstr ""
 
-#: src/components/BranchMenu.tsx:63 src/components/BranchMenu.tsx:64
+#: src/components/BranchMenu.tsx:62 src/components/BranchMenu.tsx:63 src/components/BranchMenu.tsx:64
 msgid "Please commit, stash, or discard your changes before you switch branches."
 msgstr ""
 
-#: src/components/BranchMenu.tsx:74 src/components/BranchMenu.tsx:75
+#: src/components/BranchMenu.tsx:73 src/components/BranchMenu.tsx:74 src/components/BranchMenu.tsx:75
 msgid "Failed to switch branch."
 msgstr ""
 
-#: src/components/BranchPicker.tsx:126 src/components/MergeBranchDialog.tsx:114
+#: src/components/BranchPicker.tsx:126 src/components/BranchPicker.tsx:128 src/components/MergeBranchDialog.tsx:114
 msgid "Merge Branch"
 msgstr ""
 
-#: src/components/BranchPicker.tsx:127
+#: src/components/BranchPicker.tsx:127 src/components/BranchPicker.tsx:129
 msgid "Rebase Branch"
 msgstr ""
 
-#: src/components/BranchPicker.tsx:131 src/components/ManageRemoteDialogue.tsx:95 src/components/MergeBranchDialog.tsx:117 src/components/NewBranchDialog.tsx:150 src/components/NewBranchDialog.tsx:157 src/components/NewTagDialog.tsx:412 src/components/NewTagDialog.tsx:426 src/components/ResetRevertDialog.tsx:130 src/components/ResetRevertDialog.tsx:132
+#: src/components/BranchPicker.tsx:131 src/components/BranchPicker.tsx:133 src/components/ManageRemoteDialogue.tsx:95 src/components/MergeBranchDialog.tsx:117 src/components/NewBranchDialog.tsx:145 src/components/NewBranchDialog.tsx:150 src/components/NewBranchDialog.tsx:157 src/components/NewTagDialog.tsx:412 src/components/NewTagDialog.tsx:421 src/components/NewTagDialog.tsx:426 src/components/ResetRevertDialog.tsx:126 src/components/ResetRevertDialog.tsx:130 src/components/ResetRevertDialog.tsx:132
 msgid "Close this dialog"
 msgstr ""
 
-#: src/components/BranchPicker.tsx:142 src/components/MergeBranchDialog.tsx:127
+#: src/components/BranchPicker.tsx:142 src/components/BranchPicker.tsx:144 src/components/MergeBranchDialog.tsx:127
 msgid "Select the branch to merge in %1"
 msgstr ""
 
-#: src/components/BranchPicker.tsx:143
+#: src/components/BranchPicker.tsx:143 src/components/BranchPicker.tsx:145
 msgid "Select the branch to rebase %1 onto"
 msgstr ""
 
-#: src/components/BranchPicker.tsx:158 src/components/MergeBranchDialog.tsx:139
+#: src/components/BranchPicker.tsx:158 src/components/BranchPicker.tsx:160 src/components/MergeBranchDialog.tsx:139
 msgid "Filter branch list"
 msgstr ""
 
-#: src/components/BranchPicker.tsx:193 src/components/MergeBranchDialog.tsx:172
+#: src/components/BranchPicker.tsx:193 src/components/BranchPicker.tsx:195 src/components/MergeBranchDialog.tsx:172
 msgid "Close this dialog without merging a branch"
 msgstr ""
 
-#: src/components/BranchPicker.tsx:194
+#: src/components/BranchPicker.tsx:194 src/components/BranchPicker.tsx:196
 msgid "Close this dialog without rebasing the branch"
 msgstr ""
 
-#: src/components/BranchPicker.tsx:206 src/components/MergeBranchDialog.tsx:181
+#: src/components/BranchPicker.tsx:206 src/components/BranchPicker.tsx:208 src/components/MergeBranchDialog.tsx:181
 msgid "Merge branch"
 msgstr ""
 
-#: src/components/BranchPicker.tsx:207
+#: src/components/BranchPicker.tsx:207 src/components/BranchPicker.tsx:209
 msgid "Rebase branch"
 msgstr ""
 
-#: src/components/BranchPicker.tsx:209
+#: src/components/BranchPicker.tsx:209 src/components/BranchPicker.tsx:211
 msgid "Rebase"
 msgstr ""
 
-#: src/components/BranchPicker.tsx:209 src/components/MergeBranchDialog.tsx:182
+#: src/components/BranchPicker.tsx:209 src/components/BranchPicker.tsx:211 src/components/MergeBranchDialog.tsx:182
 msgid "Merge"
 msgstr ""
 
 #: src/components/BranchPicker.tsx:95
 msgid "Merge branch %1"
 msgstr ""
 
@@ -1041,19 +1099,19 @@
 msgid "Summary (%1 to commit)"
 msgstr ""
 
 #: src/components/CommitBox.tsx:116 src/components/CommitBox.tsx:117 src/components/CommitMessage.tsx:117 src/components/CommitMessage.tsx:123 src/components/ResetRevertDialog.tsx:155
 msgid "Enter a commit message summary (a single line, preferably less than 50 characters)"
 msgstr ""
 
-#: src/components/CommitBox.tsx:126 src/components/CommitBox.tsx:127 src/components/CommitMessage.tsx:140 src/components/CommitMessage.tsx:146
+#: src/components/CommitBox.tsx:126 src/components/CommitBox.tsx:127 src/components/CommitMessage.tsx:140 src/components/CommitMessage.tsx:145 src/components/CommitMessage.tsx:146
 msgid "Description (optional)"
 msgstr ""
 
-#: src/components/CommitBox.tsx:127 src/components/CommitBox.tsx:128 src/components/CommitMessage.tsx:147 src/components/CommitMessage.tsx:153 src/components/ResetRevertDialog.tsx:165
+#: src/components/CommitBox.tsx:127 src/components/CommitBox.tsx:128 src/components/CommitMessage.tsx:147 src/components/CommitMessage.tsx:152 src/components/CommitMessage.tsx:153 src/components/ResetRevertDialog.tsx:165
 msgid "Enter a commit message description"
 msgstr ""
 
 #: src/components/CommitBox.tsx:141 src/components/CommitBox.tsx:146 src/components/CommitBox.tsx:148
 msgid "Create a new commit"
 msgstr ""
 
@@ -1069,267 +1127,303 @@
 msgid "Staged changes will be added to the previous commit and its date will be updated."
 msgstr ""
 
 #: src/components/CommitBox.tsx:176 src/components/CommitBox.tsx:181 src/components/CommitBox.tsx:183 src/components/CommitBox.tsx:98 src/components/CommitBox.tsx:99
 msgid "Disabled: No files are staged for commit"
 msgstr ""
 
-#: src/components/CommitBox.tsx:195 src/components/GitPanel.tsx:440 src/components/GitPanel.tsx:441 src/components/GitPanel.tsx:475 src/components/GitPanel.tsx:494
+#: src/components/CommitBox.tsx:195 src/components/GitPanel.tsx:440 src/components/GitPanel.tsx:441 src/components/GitPanel.tsx:475 src/components/GitPanel.tsx:488 src/components/GitPanel.tsx:494
 msgid "Warning"
 msgstr ""
 
 #: src/components/CommitBox.tsx:196
 msgid "Looks like you still have unsaved staged files. Remember to save and stage all needed changes before committing!"
 msgstr ""
 
-#: src/components/CommitComparisonBox.tsx:163
+#: src/components/CommitComparisonBox.tsx:159 src/components/CommitComparisonBox.tsx:163
 msgid "Close"
 msgstr ""
 
-#: src/components/CommitComparisonBox.tsx:184
+#: src/components/CommitComparisonBox.tsx:184 src/components/CommitComparisonBox.tsx:185
 msgid "No changes"
 msgstr ""
 
-#: src/components/CommitComparisonBox.tsx:185
+#: src/components/CommitComparisonBox.tsx:185 src/components/CommitComparisonBox.tsx:186
 msgid "No challenger commit selected."
 msgstr ""
 
 #: src/components/CommitDiff.tsx:103 src/components/SinglePastCommitInfo.tsx:179 src/components/SinglePastCommitInfo.tsx:190 src/components/SinglePastCommitInfo.tsx:192
 msgid "# Insertions"
 msgstr ""
 
 #: src/components/CommitDiff.tsx:110 src/components/SinglePastCommitInfo.tsx:186 src/components/SinglePastCommitInfo.tsx:197 src/components/SinglePastCommitInfo.tsx:199
 msgid "# Deletions"
 msgstr ""
 
-#: src/components/CommitDiff.tsx:121 src/components/FileList.tsx:1211 src/components/FileList.tsx:1215 src/components/FileList.tsx:518 src/components/FileList.tsx:527 src/components/FileList.tsx:595 src/components/FileList.tsx:596 src/components/FileList.tsx:728 src/components/FileList.tsx:737 src/components/FileList.tsx:806 src/components/FileList.tsx:883 src/components/FileList.tsx:906 src/components/FileList.tsx:910 src/components/SinglePastCommitInfo.tsx:197 src/components/SinglePastCommitInfo.tsx:208 src/components/SinglePastCommitInfo.tsx:210
+#: src/components/CommitDiff.tsx:121 src/components/FileList.tsx:1211 src/components/FileList.tsx:1215 src/components/FileList.tsx:1239 src/components/FileList.tsx:518 src/components/FileList.tsx:527 src/components/FileList.tsx:595 src/components/FileList.tsx:596 src/components/FileList.tsx:728 src/components/FileList.tsx:737 src/components/FileList.tsx:806 src/components/FileList.tsx:883 src/components/FileList.tsx:906 src/components/FileList.tsx:910 src/components/FileList.tsx:934 src/components/SinglePastCommitInfo.tsx:197 src/components/SinglePastCommitInfo.tsx:208 src/components/SinglePastCommitInfo.tsx:210
 msgid "Changed"
 msgstr ""
 
 #: src/components/CommitDiff.tsx:164 src/components/PastCommitNode.tsx:112 src/components/PastCommitNode.tsx:153 src/components/PastCommitNode.tsx:157 src/components/PastCommitNode.tsx:170 src/components/SinglePastCommitInfo.tsx:273 src/components/SinglePastCommitInfo.tsx:284 src/components/SinglePastCommitInfo.tsx:287
 msgid "View file changes"
 msgstr ""
 
 #: src/components/CommitDiff.tsx:99 src/components/SinglePastCommitInfo.tsx:175 src/components/SinglePastCommitInfo.tsx:186 src/components/SinglePastCommitInfo.tsx:188
 msgid "# Files Changed"
 msgstr ""
 
-#: src/components/CommitMessage.tsx:114 src/components/CommitMessage.tsx:120 src/components/CommitMessage.tsx:144 src/components/CommitMessage.tsx:150
+#: src/components/CommitMessage.tsx:114 src/components/CommitMessage.tsx:120 src/components/CommitMessage.tsx:144 src/components/CommitMessage.tsx:149 src/components/CommitMessage.tsx:150
 msgid "Amending the commit will re-use the previous commit summary"
 msgstr ""
 
-#: src/components/CommitMessage.tsx:66 src/components/CommitMessage.tsx:71
+#: src/components/CommitMessage.tsx:66 src/components/CommitMessage.tsx:71 src/components/CommitMessage.tsx:72
 msgid "Summary"
 msgstr ""
 
-#: src/components/FileList.tsx:1000 src/components/FileList.tsx:602 src/components/FileList.tsx:611 src/components/FileList.tsx:679 src/components/FileList.tsx:680 src/components/FileList.tsx:996
+#: src/components/FileItem.tsx:162
+msgid "Unmodified"
+msgstr ""
+
+#: src/components/FileItem.tsx:208 src/components/FileList.tsx:404 src/components/FileList.tsx:405 src/components/FileList.tsx:703 src/components/FileList.tsx:713 src/components/FileList.tsx:727
+msgid "Conflicted"
+msgstr ""
+
+#: src/components/FileItem.tsx:268
+msgid "Modified"
+msgstr ""
+
+#: src/components/FileItem.tsx:269
+msgid "Added"
+msgstr ""
+
+#: src/components/FileItem.tsx:270
+msgid "Deleted"
+msgstr ""
+
+#: src/components/FileItem.tsx:271
+msgid "Renamed"
+msgstr ""
+
+#: src/components/FileItem.tsx:272
+msgid "Copied"
+msgstr ""
+
+#: src/components/FileItem.tsx:273
+msgid "Updated"
+msgstr ""
+
+#: src/components/FileItem.tsx:274
+msgid "Behind"
+msgstr ""
+
+#: src/components/FileItem.tsx:275 src/components/FileList.tsx:1000 src/components/FileList.tsx:1024 src/components/FileList.tsx:602 src/components/FileList.tsx:611 src/components/FileList.tsx:679 src/components/FileList.tsx:680 src/components/FileList.tsx:996
 msgid "Untracked"
 msgstr ""
 
-#: src/components/FileList.tsx:1027 src/components/FileList.tsx:1031 src/components/FileList.tsx:1105 src/components/FileList.tsx:1109 src/components/FileList.tsx:1118 src/components/FileList.tsx:1122 src/components/FileList.tsx:1144 src/components/FileList.tsx:1148 src/components/FileList.tsx:363 src/components/FileList.tsx:372 src/components/FileList.tsx:440 src/components/FileList.tsx:441 src/components/FileList.tsx:450 src/components/FileList.tsx:459 src/components/FileList.tsx:527 src/components/FileList.tsx:528 src/components/FileList.tsx:549 src/components/FileList.tsx:558 src/components/FileList.tsx:626 src/components/FileList.tsx:627 src/components/FileList.tsx:635 src/components/FileList.tsx:644 src/components/FileList.tsx:648 src/components/FileList.tsx:657 src/components/FileList.tsx:674 src/components/FileList.tsx:683 src/components/FileList.tsx:710 src/components/FileList.tsx:713 src/components/FileList.tsx:726 src/components/FileList.tsx:734 src/components/FileList.tsx:744 src/components/FileList.tsx:752 src/components/FileList.tsx:790 src/components/FileList.tsx:803 src/components/FileList.tsx:826 src/components/FileList.tsx:828 src/components/FileList.tsx:829 src/components/FileList.tsx:937 src/components/FileList.tsx:941
+#: src/components/FileItem.tsx:276
+msgid "Ignored"
+msgstr ""
+
+#: src/components/FileList.tsx:1019 src/components/FileList.tsx:597 src/components/FileList.tsx:606 src/components/FileList.tsx:674 src/components/FileList.tsx:675 src/components/FileList.tsx:991 src/components/FileList.tsx:995
+msgid "Track all untracked files"
+msgstr ""
+
+#: src/components/FileList.tsx:1027 src/components/FileList.tsx:1031 src/components/FileList.tsx:1055 src/components/FileList.tsx:1105 src/components/FileList.tsx:1109 src/components/FileList.tsx:1118 src/components/FileList.tsx:1122 src/components/FileList.tsx:1133 src/components/FileList.tsx:1144 src/components/FileList.tsx:1146 src/components/FileList.tsx:1148 src/components/FileList.tsx:1172 src/components/FileList.tsx:363 src/components/FileList.tsx:372 src/components/FileList.tsx:440 src/components/FileList.tsx:441 src/components/FileList.tsx:450 src/components/FileList.tsx:459 src/components/FileList.tsx:527 src/components/FileList.tsx:528 src/components/FileList.tsx:549 src/components/FileList.tsx:558 src/components/FileList.tsx:626 src/components/FileList.tsx:627 src/components/FileList.tsx:635 src/components/FileList.tsx:644 src/components/FileList.tsx:648 src/components/FileList.tsx:657 src/components/FileList.tsx:674 src/components/FileList.tsx:683 src/components/FileList.tsx:710 src/components/FileList.tsx:713 src/components/FileList.tsx:726 src/components/FileList.tsx:734 src/components/FileList.tsx:744 src/components/FileList.tsx:752 src/components/FileList.tsx:758 src/components/FileList.tsx:790 src/components/FileList.tsx:803 src/components/FileList.tsx:826 src/components/FileList.tsx:828 src/components/FileList.tsx:829 src/components/FileList.tsx:850 src/components/FileList.tsx:937 src/components/FileList.tsx:941 src/components/FileList.tsx:965
 msgid "Open this file"
 msgstr ""
 
-#: src/components/FileList.tsx:1066 src/components/FileList.tsx:1070 src/components/FileList.tsx:751
+#: src/components/FileList.tsx:1066 src/components/FileList.tsx:1070 src/components/FileList.tsx:1094 src/components/FileList.tsx:751
 msgid "Pull from remote branch"
 msgstr ""
 
-#: src/components/FileList.tsx:1071 src/components/FileList.tsx:1075 src/components/FileList.tsx:756
+#: src/components/FileList.tsx:1071 src/components/FileList.tsx:1075 src/components/FileList.tsx:1099 src/components/FileList.tsx:756
 msgid "Remote Changes"
 msgstr ""
 
-#: src/components/FileList.tsx:1207 src/components/FileList.tsx:1211 src/components/FileList.tsx:505 src/components/FileList.tsx:514 src/components/FileList.tsx:582 src/components/FileList.tsx:583 src/components/FileList.tsx:724 src/components/FileList.tsx:733 src/components/FileList.tsx:802 src/components/FileList.tsx:879 src/components/FileList.tsx:893 src/components/FileList.tsx:897
+#: src/components/FileList.tsx:1207 src/components/FileList.tsx:1211 src/components/FileList.tsx:1235 src/components/FileList.tsx:505 src/components/FileList.tsx:514 src/components/FileList.tsx:582 src/components/FileList.tsx:583 src/components/FileList.tsx:724 src/components/FileList.tsx:733 src/components/FileList.tsx:802 src/components/FileList.tsx:879 src/components/FileList.tsx:893 src/components/FileList.tsx:897 src/components/FileList.tsx:921
 msgid "Discard All Changes"
 msgstr ""
 
-#: src/components/FileList.tsx:1244 src/components/FileList.tsx:1248 src/components/FileList.tsx:749 src/components/FileList.tsx:758 src/components/FileList.tsx:827 src/components/FileList.tsx:904
+#: src/components/FileList.tsx:1244 src/components/FileList.tsx:1248 src/components/FileList.tsx:1272 src/components/FileList.tsx:749 src/components/FileList.tsx:758 src/components/FileList.tsx:827 src/components/FileList.tsx:904
 msgid "Diff this file"
 msgstr ""
 
-#: src/components/FileList.tsx:177 src/components/FileList.tsx:186 src/components/FileList.tsx:188 src/components/FileList.tsx:191 src/components/FileList.tsx:202 src/components/FileList.tsx:211 src/components/FileList.tsx:213 src/components/FileList.tsx:252 src/components/FileList.tsx:262 src/widgets/discardAllChanges.ts:16
+#: src/components/FileList.tsx:177 src/components/FileList.tsx:186 src/components/FileList.tsx:188 src/components/FileList.tsx:191 src/components/FileList.tsx:202 src/components/FileList.tsx:211 src/components/FileList.tsx:213 src/components/FileList.tsx:252 src/components/FileList.tsx:262 src/components/FileList.tsx:263 src/widgets/discardAllChanges.ts:16
 msgid "Discard all changes"
 msgstr ""
 
 #: src/components/FileList.tsx:178 src/components/FileList.tsx:187 src/components/FileList.tsx:189 src/components/FileList.tsx:203 src/components/FileList.tsx:212 src/components/FileList.tsx:214 src/widgets/discardAllChanges.ts:21
 msgid "Are you sure you want to permanently discard changes to all files? This action cannot be undone."
 msgstr ""
 
-#: src/components/FileList.tsx:191 src/components/FileList.tsx:200 src/components/FileList.tsx:202 src/components/FileList.tsx:205 src/components/FileList.tsx:266 src/components/FileList.tsx:276
+#: src/components/FileList.tsx:191 src/components/FileList.tsx:200 src/components/FileList.tsx:202 src/components/FileList.tsx:205 src/components/FileList.tsx:266 src/components/FileList.tsx:276 src/components/FileList.tsx:277
 msgid "Discard all unstaged changes failed."
 msgstr ""
 
-#: src/components/FileList.tsx:192 src/components/FileList.tsx:253 src/components/FileList.tsx:263
+#: src/components/FileList.tsx:192 src/components/FileList.tsx:253 src/components/FileList.tsx:263 src/components/FileList.tsx:264
 msgid "Are you sure you want to permanently discard changes to all unstaged files? This action cannot be undone."
 msgstr ""
 
 #: src/components/FileList.tsx:216 src/components/FileList.tsx:225 src/components/FileList.tsx:227 src/widgets/discardAllChanges.ts:34
 msgid "Discard all changes failed."
 msgstr ""
 
-#: src/components/FileList.tsx:370 src/components/FileList.tsx:379 src/components/FileList.tsx:447 src/components/FileList.tsx:448 src/components/FileList.tsx:743 src/components/FileList.tsx:753
+#: src/components/FileList.tsx:370 src/components/FileList.tsx:379 src/components/FileList.tsx:447 src/components/FileList.tsx:448 src/components/FileList.tsx:743 src/components/FileList.tsx:753 src/components/FileList.tsx:767
 msgid "Unstage this change"
 msgstr ""
 
-#: src/components/FileList.tsx:404 src/components/FileList.tsx:405 src/components/FileList.tsx:703 src/components/FileList.tsx:713
-msgid "Conflicted"
-msgstr ""
-
-#: src/components/FileList.tsx:408 src/components/FileList.tsx:417 src/components/FileList.tsx:485 src/components/FileList.tsx:486 src/components/FileList.tsx:788 src/components/FileList.tsx:791
+#: src/components/FileList.tsx:408 src/components/FileList.tsx:417 src/components/FileList.tsx:485 src/components/FileList.tsx:486 src/components/FileList.tsx:788 src/components/FileList.tsx:791 src/components/FileList.tsx:812
 msgid "Unstage all changes"
 msgstr ""
 
-#: src/components/FileList.tsx:414 src/components/FileList.tsx:423 src/components/FileList.tsx:491 src/components/FileList.tsx:492 src/components/FileList.tsx:795 src/components/FileList.tsx:797
+#: src/components/FileList.tsx:414 src/components/FileList.tsx:423 src/components/FileList.tsx:491 src/components/FileList.tsx:492 src/components/FileList.tsx:795 src/components/FileList.tsx:797 src/components/FileList.tsx:819
 msgid "Staged"
 msgstr ""
 
-#: src/components/FileList.tsx:465 src/components/FileList.tsx:474 src/components/FileList.tsx:542 src/components/FileList.tsx:543 src/components/FileList.tsx:843 src/components/FileList.tsx:845
+#: src/components/FileList.tsx:465 src/components/FileList.tsx:474 src/components/FileList.tsx:542 src/components/FileList.tsx:543 src/components/FileList.tsx:843 src/components/FileList.tsx:845 src/components/FileList.tsx:867
 msgid "Stage this change"
 msgstr ""
 
-#: src/components/FileList.tsx:512 src/components/FileList.tsx:521 src/components/FileList.tsx:589 src/components/FileList.tsx:590 src/components/FileList.tsx:900 src/components/FileList.tsx:904
+#: src/components/FileList.tsx:512 src/components/FileList.tsx:521 src/components/FileList.tsx:589 src/components/FileList.tsx:590 src/components/FileList.tsx:900 src/components/FileList.tsx:904 src/components/FileList.tsx:928
 msgid "Stage all changes"
 msgstr ""
 
-#: src/components/FileList.tsx:559 src/components/FileList.tsx:568 src/components/FileList.tsx:636 src/components/FileList.tsx:637 src/components/FileList.tsx:945 src/components/FileList.tsx:949
+#: src/components/FileList.tsx:559 src/components/FileList.tsx:568 src/components/FileList.tsx:636 src/components/FileList.tsx:637 src/components/FileList.tsx:945 src/components/FileList.tsx:949 src/components/FileList.tsx:973
 msgid "Track this file"
 msgstr ""
 
-#: src/components/FileList.tsx:597 src/components/FileList.tsx:606 src/components/FileList.tsx:674 src/components/FileList.tsx:675 src/components/FileList.tsx:991 src/components/FileList.tsx:995
-msgid "Track all untracked files"
-msgstr ""
-
-#: src/components/FileList.tsx:782 src/components/FileList.tsx:891 src/components/GitPanel.tsx:503 src/components/GitPanel.tsx:522
+#: src/components/FileList.tsx:782 src/components/FileList.tsx:806 src/components/FileList.tsx:891 src/components/FileList.tsx:915 src/components/GitPanel.tsx:503 src/components/GitPanel.tsx:516 src/components/GitPanel.tsx:522
 msgid "Stash latest changes"
 msgstr ""
 
-#: src/components/GitPanel.tsx:216 src/components/GitPanel.tsx:506 src/components/GitPanel.tsx:533 src/components/GitPanel.tsx:547 src/components/GitPanel.tsx:561 src/components/GitPanel.tsx:569 src/components/GitPanel.tsx:668 src/components/GitPanel.tsx:669 src/components/GitPanel.tsx:752 src/components/GitPanel.tsx:771 src/components/GitPanel.tsx:772
+#: src/components/GitPanel.tsx:216 src/components/GitPanel.tsx:506 src/components/GitPanel.tsx:533 src/components/GitPanel.tsx:547 src/components/GitPanel.tsx:561 src/components/GitPanel.tsx:569 src/components/GitPanel.tsx:668 src/components/GitPanel.tsx:669 src/components/GitPanel.tsx:752 src/components/GitPanel.tsx:766 src/components/GitPanel.tsx:771 src/components/GitPanel.tsx:772
 msgid "Staging files..."
 msgstr ""
 
-#: src/components/GitPanel.tsx:237 src/components/GitPanel.tsx:523 src/components/GitPanel.tsx:550 src/components/GitPanel.tsx:564 src/components/GitPanel.tsx:578 src/components/GitPanel.tsx:586 src/components/GitPanel.tsx:685 src/components/GitPanel.tsx:686 src/components/GitPanel.tsx:769 src/components/GitPanel.tsx:788 src/components/GitPanel.tsx:789
+#: src/components/GitPanel.tsx:237 src/components/GitPanel.tsx:523 src/components/GitPanel.tsx:550 src/components/GitPanel.tsx:564 src/components/GitPanel.tsx:578 src/components/GitPanel.tsx:586 src/components/GitPanel.tsx:685 src/components/GitPanel.tsx:686 src/components/GitPanel.tsx:769 src/components/GitPanel.tsx:786 src/components/GitPanel.tsx:788 src/components/GitPanel.tsx:789
 msgid "Failed to commit changes."
 msgstr ""
 
-#: src/components/GitPanel.tsx:250 src/components/GitPanel.tsx:531 src/components/GitPanel.tsx:558 src/components/GitPanel.tsx:572 src/components/GitPanel.tsx:586 src/components/GitPanel.tsx:594 src/components/GitPanel.tsx:693 src/components/GitPanel.tsx:694 src/components/GitPanel.tsx:777 src/components/GitPanel.tsx:796 src/components/GitPanel.tsx:797
+#: src/components/GitPanel.tsx:250 src/components/GitPanel.tsx:531 src/components/GitPanel.tsx:558 src/components/GitPanel.tsx:572 src/components/GitPanel.tsx:586 src/components/GitPanel.tsx:594 src/components/GitPanel.tsx:693 src/components/GitPanel.tsx:694 src/components/GitPanel.tsx:777 src/components/GitPanel.tsx:791 src/components/GitPanel.tsx:796 src/components/GitPanel.tsx:797
 msgid "Committing changes..."
 msgstr ""
 
-#: src/components/GitPanel.tsx:257 src/components/GitPanel.tsx:538 src/components/GitPanel.tsx:569 src/components/GitPanel.tsx:583 src/components/GitPanel.tsx:597 src/components/GitPanel.tsx:605 src/components/GitPanel.tsx:704 src/components/GitPanel.tsx:705 src/components/GitPanel.tsx:788 src/components/GitPanel.tsx:807 src/components/GitPanel.tsx:808
+#: src/components/GitPanel.tsx:257 src/components/GitPanel.tsx:538 src/components/GitPanel.tsx:569 src/components/GitPanel.tsx:583 src/components/GitPanel.tsx:597 src/components/GitPanel.tsx:605 src/components/GitPanel.tsx:704 src/components/GitPanel.tsx:705 src/components/GitPanel.tsx:788 src/components/GitPanel.tsx:807 src/components/GitPanel.tsx:808 src/components/GitPanel.tsx:813
 msgid "Committed changes."
 msgstr ""
 
-#: src/components/GitPanel.tsx:333 src/components/GitPanel.tsx:347 src/components/GitPanel.tsx:352 src/components/GitPanel.tsx:359 src/components/GitPanel.tsx:372 src/components/GitPanel.tsx:380 src/components/GitPanel.tsx:403 src/components/GitPanel.tsx:404 src/components/GitPanel.tsx:438 src/components/GitPanel.tsx:457
+#: src/components/GitPanel.tsx:333 src/components/GitPanel.tsx:347 src/components/GitPanel.tsx:352 src/components/GitPanel.tsx:359 src/components/GitPanel.tsx:372 src/components/GitPanel.tsx:380 src/components/GitPanel.tsx:403 src/components/GitPanel.tsx:404 src/components/GitPanel.tsx:438 src/components/GitPanel.tsx:451 src/components/GitPanel.tsx:457
 msgid "View changed files"
 msgstr ""
 
-#: src/components/GitPanel.tsx:334 src/components/GitPanel.tsx:348 src/components/GitPanel.tsx:353 src/components/GitPanel.tsx:360 src/components/GitPanel.tsx:373 src/components/GitPanel.tsx:381 src/components/GitPanel.tsx:404 src/components/GitPanel.tsx:405 src/components/GitPanel.tsx:439 src/components/GitPanel.tsx:458
+#: src/components/GitPanel.tsx:334 src/components/GitPanel.tsx:348 src/components/GitPanel.tsx:353 src/components/GitPanel.tsx:360 src/components/GitPanel.tsx:373 src/components/GitPanel.tsx:381 src/components/GitPanel.tsx:404 src/components/GitPanel.tsx:405 src/components/GitPanel.tsx:439 src/components/GitPanel.tsx:452 src/components/GitPanel.tsx:458
 msgid "Changes"
 msgstr ""
 
-#: src/components/GitPanel.tsx:343 src/components/GitPanel.tsx:357 src/components/GitPanel.tsx:362 src/components/GitPanel.tsx:369 src/components/GitPanel.tsx:382 src/components/GitPanel.tsx:390 src/components/GitPanel.tsx:413 src/components/GitPanel.tsx:414 src/components/GitPanel.tsx:448 src/components/GitPanel.tsx:467
+#: src/components/GitPanel.tsx:343 src/components/GitPanel.tsx:357 src/components/GitPanel.tsx:362 src/components/GitPanel.tsx:369 src/components/GitPanel.tsx:382 src/components/GitPanel.tsx:390 src/components/GitPanel.tsx:413 src/components/GitPanel.tsx:414 src/components/GitPanel.tsx:448 src/components/GitPanel.tsx:461 src/components/GitPanel.tsx:467
 msgid "View commit history"
 msgstr ""
 
-#: src/components/GitPanel.tsx:364 src/components/GitPanel.tsx:378 src/components/GitPanel.tsx:383 src/components/GitPanel.tsx:390 src/components/GitPanel.tsx:403 src/components/GitPanel.tsx:411 src/components/GitPanel.tsx:436 src/components/GitPanel.tsx:437 src/components/GitPanel.tsx:471 src/components/GitPanel.tsx:490
+#: src/components/GitPanel.tsx:364 src/components/GitPanel.tsx:378 src/components/GitPanel.tsx:383 src/components/GitPanel.tsx:390 src/components/GitPanel.tsx:403 src/components/GitPanel.tsx:411 src/components/GitPanel.tsx:436 src/components/GitPanel.tsx:437 src/components/GitPanel.tsx:471 src/components/GitPanel.tsx:484 src/components/GitPanel.tsx:490
 msgid "Commit and Push"
 msgstr ""
 
-#: src/components/GitPanel.tsx:365 src/components/GitPanel.tsx:379 src/components/GitPanel.tsx:384 src/components/GitPanel.tsx:391 src/components/GitPanel.tsx:404 src/components/GitPanel.tsx:412 src/components/GitPanel.tsx:439 src/components/GitPanel.tsx:440 src/components/GitPanel.tsx:474 src/components/GitPanel.tsx:493
+#: src/components/GitPanel.tsx:365 src/components/GitPanel.tsx:379 src/components/GitPanel.tsx:384 src/components/GitPanel.tsx:391 src/components/GitPanel.tsx:404 src/components/GitPanel.tsx:412 src/components/GitPanel.tsx:439 src/components/GitPanel.tsx:440 src/components/GitPanel.tsx:474 src/components/GitPanel.tsx:487 src/components/GitPanel.tsx:493
 msgid "Commit"
 msgstr ""
 
-#: src/components/GitPanel.tsx:426 src/components/GitPanel.tsx:442 src/components/GitPanel.tsx:447 src/components/GitPanel.tsx:454 src/components/GitPanel.tsx:468 src/components/GitPanel.tsx:476 src/components/GitPanel.tsx:575 src/components/GitPanel.tsx:576 src/components/GitPanel.tsx:659 src/components/GitPanel.tsx:678 src/components/GitPanel.tsx:679
+#: src/components/GitPanel.tsx:426 src/components/GitPanel.tsx:442 src/components/GitPanel.tsx:447 src/components/GitPanel.tsx:454 src/components/GitPanel.tsx:468 src/components/GitPanel.tsx:476 src/components/GitPanel.tsx:575 src/components/GitPanel.tsx:576 src/components/GitPanel.tsx:659 src/components/GitPanel.tsx:672 src/components/GitPanel.tsx:678 src/components/GitPanel.tsx:679
 msgid "is not"
 msgstr ""
 
-#: src/components/GitPanel.tsx:429 src/components/GitPanel.tsx:445 src/components/GitPanel.tsx:450 src/components/GitPanel.tsx:457 src/components/GitPanel.tsx:471 src/components/GitPanel.tsx:479 src/components/GitPanel.tsx:578 src/components/GitPanel.tsx:579 src/components/GitPanel.tsx:662 src/components/GitPanel.tsx:681 src/components/GitPanel.tsx:682
+#: src/components/GitPanel.tsx:429 src/components/GitPanel.tsx:445 src/components/GitPanel.tsx:450 src/components/GitPanel.tsx:457 src/components/GitPanel.tsx:471 src/components/GitPanel.tsx:479 src/components/GitPanel.tsx:578 src/components/GitPanel.tsx:579 src/components/GitPanel.tsx:662 src/components/GitPanel.tsx:675 src/components/GitPanel.tsx:681 src/components/GitPanel.tsx:682
 msgid "You are not currently in"
 msgstr ""
 
-#: src/components/GitPanel.tsx:431 src/components/GitPanel.tsx:447 src/components/GitPanel.tsx:452 src/components/GitPanel.tsx:459 src/components/GitPanel.tsx:473 src/components/GitPanel.tsx:481 src/components/GitPanel.tsx:580 src/components/GitPanel.tsx:581 src/components/GitPanel.tsx:664 src/components/GitPanel.tsx:683 src/components/GitPanel.tsx:684
+#: src/components/GitPanel.tsx:431 src/components/GitPanel.tsx:447 src/components/GitPanel.tsx:452 src/components/GitPanel.tsx:459 src/components/GitPanel.tsx:473 src/components/GitPanel.tsx:481 src/components/GitPanel.tsx:580 src/components/GitPanel.tsx:581 src/components/GitPanel.tsx:664 src/components/GitPanel.tsx:677 src/components/GitPanel.tsx:683 src/components/GitPanel.tsx:684
 msgid " a Git repository. To use Git, navigate to a local repository, initialize a repository here, or clone an existing repository."
 msgstr ""
 
-#: src/components/GitPanel.tsx:435 src/components/GitPanel.tsx:436 src/components/GitPanel.tsx:470 src/components/GitPanel.tsx:489
+#: src/components/GitPanel.tsx:435 src/components/GitPanel.tsx:436 src/components/GitPanel.tsx:470 src/components/GitPanel.tsx:483 src/components/GitPanel.tsx:489
 msgid "Commit (Amend) and Push"
 msgstr ""
 
-#: src/components/GitPanel.tsx:438 src/components/GitPanel.tsx:439 src/components/GitPanel.tsx:473 src/components/GitPanel.tsx:492
+#: src/components/GitPanel.tsx:438 src/components/GitPanel.tsx:439 src/components/GitPanel.tsx:473 src/components/GitPanel.tsx:486 src/components/GitPanel.tsx:492
 msgid "Commit (Amend)"
 msgstr ""
 
-#: src/components/GitPanel.tsx:439 src/components/GitPanel.tsx:455 src/components/GitPanel.tsx:460 src/components/GitPanel.tsx:467 src/components/GitPanel.tsx:481 src/components/GitPanel.tsx:489 src/components/GitPanel.tsx:588 src/components/GitPanel.tsx:589 src/components/GitPanel.tsx:672 src/components/GitPanel.tsx:691 src/components/GitPanel.tsx:692
+#: src/components/GitPanel.tsx:439 src/components/GitPanel.tsx:455 src/components/GitPanel.tsx:460 src/components/GitPanel.tsx:467 src/components/GitPanel.tsx:481 src/components/GitPanel.tsx:489 src/components/GitPanel.tsx:588 src/components/GitPanel.tsx:589 src/components/GitPanel.tsx:672 src/components/GitPanel.tsx:685 src/components/GitPanel.tsx:691 src/components/GitPanel.tsx:692
 msgid "Open the FileBrowser"
 msgstr ""
 
-#: src/components/GitPanel.tsx:445 src/components/GitPanel.tsx:446 src/components/GitPanel.tsx:480 src/components/GitPanel.tsx:499
+#: src/components/GitPanel.tsx:445 src/components/GitPanel.tsx:446 src/components/GitPanel.tsx:480 src/components/GitPanel.tsx:493 src/components/GitPanel.tsx:499
 msgid "You have unsaved tracked files. You probably want to save all changes before committing."
 msgstr ""
 
-#: src/components/GitPanel.tsx:448 src/components/GitPanel.tsx:449 src/components/GitPanel.tsx:483 src/components/GitPanel.tsx:502
+#: src/components/GitPanel.tsx:448 src/components/GitPanel.tsx:449 src/components/GitPanel.tsx:483 src/components/GitPanel.tsx:496 src/components/GitPanel.tsx:502
 msgid "You have unsaved staged files. You probably want to save and stage all needed changes before committing."
 msgstr ""
 
-#: src/components/GitPanel.tsx:509 src/components/GitPanel.tsx:528
+#: src/components/GitPanel.tsx:509 src/components/GitPanel.tsx:522 src/components/GitPanel.tsx:528
 msgid "Apply the latest stash"
 msgstr ""
 
-#: src/components/GitPanel.tsx:513 src/components/GitPanel.tsx:571 src/components/GitPanel.tsx:602 src/components/GitPanel.tsx:616 src/components/GitPanel.tsx:630 src/components/GitPanel.tsx:638 src/components/GitPanel.tsx:737 src/components/GitPanel.tsx:738 src/components/GitPanel.tsx:840 src/components/GitPanel.tsx:859 src/components/GitPanel.tsx:860
+#: src/components/GitPanel.tsx:513 src/components/GitPanel.tsx:571 src/components/GitPanel.tsx:602 src/components/GitPanel.tsx:616 src/components/GitPanel.tsx:630 src/components/GitPanel.tsx:638 src/components/GitPanel.tsx:737 src/components/GitPanel.tsx:738 src/components/GitPanel.tsx:840 src/components/GitPanel.tsx:859 src/components/GitPanel.tsx:860 src/components/GitPanel.tsx:878
 msgid "Who is committing?"
 msgstr ""
 
-#: src/components/GitPanel.tsx:517 src/components/GitPanel.tsx:536
+#: src/components/GitPanel.tsx:517 src/components/GitPanel.tsx:530 src/components/GitPanel.tsx:536
 msgid "Clear the entire stash"
 msgstr ""
 
-#: src/components/GitPanel.tsx:524 src/components/GitPanel.tsx:525 src/components/GitPanel.tsx:608 src/components/GitPanel.tsx:627 src/components/GitPanel.tsx:628
+#: src/components/GitPanel.tsx:524 src/components/GitPanel.tsx:525 src/components/GitPanel.tsx:608 src/components/GitPanel.tsx:622 src/components/GitPanel.tsx:627 src/components/GitPanel.tsx:628
 msgid "Compare %1 and %2"
 msgstr ""
 
-#: src/components/GitPanel.tsx:537 src/components/GitPanel.tsx:594 src/components/GitPanel.tsx:625 src/components/GitPanel.tsx:639 src/components/GitPanel.tsx:653 src/components/GitPanel.tsx:661 src/components/GitPanel.tsx:760 src/components/GitPanel.tsx:761 src/components/GitPanel.tsx:871 src/components/GitPanel.tsx:890 src/components/GitPanel.tsx:891
+#: src/components/GitPanel.tsx:537 src/components/GitPanel.tsx:594 src/components/GitPanel.tsx:625 src/components/GitPanel.tsx:639 src/components/GitPanel.tsx:653 src/components/GitPanel.tsx:661 src/components/GitPanel.tsx:760 src/components/GitPanel.tsx:761 src/components/GitPanel.tsx:871 src/components/GitPanel.tsx:890 src/components/GitPanel.tsx:891 src/components/GitPanel.tsx:910
 msgid "Failed to set your identity. %1"
 msgstr ""
 
-#: src/components/GitPanel.tsx:577 src/components/GitPanel.tsx:608 src/components/GitPanel.tsx:622 src/components/GitPanel.tsx:636 src/components/GitPanel.tsx:644 src/components/GitPanel.tsx:743 src/components/GitPanel.tsx:744 src/components/GitPanel.tsx:846 src/components/GitPanel.tsx:865 src/components/GitPanel.tsx:866
+#: src/components/GitPanel.tsx:577 src/components/GitPanel.tsx:608 src/components/GitPanel.tsx:622 src/components/GitPanel.tsx:636 src/components/GitPanel.tsx:644 src/components/GitPanel.tsx:743 src/components/GitPanel.tsx:744 src/components/GitPanel.tsx:846 src/components/GitPanel.tsx:865 src/components/GitPanel.tsx:866 src/components/GitPanel.tsx:884
 msgid "User refused to set identity."
 msgstr ""
 
-#: src/components/GitPanel.tsx:685 src/components/GitPanel.tsx:699 src/components/GitPanel.tsx:707 src/components/GitPanel.tsx:806 src/components/GitPanel.tsx:807 src/components/GitPanel.tsx:917 src/components/GitPanel.tsx:936 src/components/GitPanel.tsx:937
+#: src/components/GitPanel.tsx:685 src/components/GitPanel.tsx:699 src/components/GitPanel.tsx:707 src/components/GitPanel.tsx:806 src/components/GitPanel.tsx:807 src/components/GitPanel.tsx:917 src/components/GitPanel.tsx:936 src/components/GitPanel.tsx:937 src/components/GitPanel.tsx:958
 msgid "One or more open files are behind %1 head. Do you want to pull the latest remote version?"
 msgstr ""
 
-#: src/components/GitPanel.tsx:694 src/components/GitPanel.tsx:708 src/components/GitPanel.tsx:716 src/components/GitPanel.tsx:815 src/components/GitPanel.tsx:816 src/components/GitPanel.tsx:926 src/components/GitPanel.tsx:945 src/components/GitPanel.tsx:946
+#: src/components/GitPanel.tsx:694 src/components/GitPanel.tsx:708 src/components/GitPanel.tsx:716 src/components/GitPanel.tsx:815 src/components/GitPanel.tsx:816 src/components/GitPanel.tsx:926 src/components/GitPanel.tsx:945 src/components/GitPanel.tsx:946 src/components/GitPanel.tsx:967
 msgid "Continue Without Pulling"
 msgstr ""
 
-#: src/components/GitPanel.tsx:697 src/components/GitPanel.tsx:711 src/components/GitPanel.tsx:719 src/components/GitPanel.tsx:818 src/components/GitPanel.tsx:819 src/components/GitPanel.tsx:929 src/components/GitPanel.tsx:948 src/components/GitPanel.tsx:949
+#: src/components/GitPanel.tsx:697 src/components/GitPanel.tsx:711 src/components/GitPanel.tsx:719 src/components/GitPanel.tsx:818 src/components/GitPanel.tsx:819 src/components/GitPanel.tsx:929 src/components/GitPanel.tsx:948 src/components/GitPanel.tsx:949 src/components/GitPanel.tsx:970
 msgid "Pull"
 msgstr ""
 
-#: src/components/GitPanel.tsx:698 src/components/GitPanel.tsx:712 src/components/GitPanel.tsx:720 src/components/GitPanel.tsx:819 src/components/GitPanel.tsx:820 src/components/GitPanel.tsx:930 src/components/GitPanel.tsx:949 src/components/GitPanel.tsx:950
+#: src/components/GitPanel.tsx:698 src/components/GitPanel.tsx:712 src/components/GitPanel.tsx:720 src/components/GitPanel.tsx:819 src/components/GitPanel.tsx:820 src/components/GitPanel.tsx:930 src/components/GitPanel.tsx:949 src/components/GitPanel.tsx:950 src/components/GitPanel.tsx:971
 msgid "Git Pull from Remote Branch"
 msgstr ""
 
-#: src/components/GitPanel.tsx:722 src/components/GitPanel.tsx:736 src/components/GitPanel.tsx:744 src/components/GitPanel.tsx:843 src/components/GitPanel.tsx:844 src/components/GitPanel.tsx:954 src/components/GitPanel.tsx:973 src/components/GitPanel.tsx:974
+#: src/components/GitPanel.tsx:722 src/components/GitPanel.tsx:736 src/components/GitPanel.tsx:744 src/components/GitPanel.tsx:843 src/components/GitPanel.tsx:844 src/components/GitPanel.tsx:954 src/components/GitPanel.tsx:973 src/components/GitPanel.tsx:974 src/components/GitPanel.tsx:995
 msgid "The following open files remain behind:"
 msgstr ""
 
-#: src/components/GitStash.tsx:144
+#: src/components/GitStash.tsx:144 src/components/GitStash.tsx:145
 msgid "%1 (on %2)"
 msgstr ""
 
-#: src/components/GitStash.tsx:282
+#: src/components/GitStash.tsx:282 src/components/GitStash.tsx:283
 msgid "Pop stash entry"
 msgstr ""
 
-#: src/components/GitStash.tsx:290
+#: src/components/GitStash.tsx:290 src/components/GitStash.tsx:291
 msgid "Apply stash entry"
 msgstr ""
 
-#: src/components/GitStash.tsx:298
+#: src/components/GitStash.tsx:298 src/components/GitStash.tsx:299
 msgid "Drop stash entry"
 msgstr ""
 
 #: src/components/HistorySideBar.tsx:104 src/components/HistorySideBar.tsx:106 src/components/HistorySideBar.tsx:115 src/components/HistorySideBar.tsx:122 src/components/HistorySideBar.tsx:124
 msgid "Uncommitted Changes"
 msgstr ""
 
@@ -1341,15 +1435,15 @@
 msgid "You"
 msgstr ""
 
 #: src/components/HistorySideBar.tsx:126 src/components/HistorySideBar.tsx:144 src/components/HistorySideBar.tsx:146 src/components/HistorySideBar.tsx:165 src/components/HistorySideBar.tsx:193
 msgid "Discard file history"
 msgstr ""
 
-#: src/components/HistorySideBar.tsx:187 src/components/HistorySideBar.tsx:189 src/components/HistorySideBar.tsx:192 src/components/HistorySideBar.tsx:241 src/components/HistorySideBar.tsx:271
+#: src/components/HistorySideBar.tsx:187 src/components/HistorySideBar.tsx:189 src/components/HistorySideBar.tsx:192 src/components/HistorySideBar.tsx:241 src/components/HistorySideBar.tsx:271 src/components/HistorySideBar.tsx:273
 msgid "No history found."
 msgstr ""
 
 #: src/components/ManageRemoteDialogue.tsx:104
 msgid "Enter a new remote repository name and URL"
 msgstr ""
 
@@ -1373,115 +1467,115 @@
 msgid "Remove this remote"
 msgstr ""
 
 #: src/components/ManageRemoteDialogue.tsx:92
 msgid "Manage Remotes"
 msgstr ""
 
-#: src/components/MergeBranchDialog.tsx:87 src/components/NewBranchDialog.tsx:309 src/components/NewBranchDialog.tsx:313 src/components/NewBranchDialog.tsx:315
+#: src/components/MergeBranchDialog.tsx:87 src/components/NewBranchDialog.tsx:309 src/components/NewBranchDialog.tsx:310 src/components/NewBranchDialog.tsx:313 src/components/NewBranchDialog.tsx:315
 msgid "Create a new branch based on: %1"
 msgstr ""
 
-#: src/components/NewBranchDialog.tsx:147 src/components/NewBranchDialog.tsx:154
+#: src/components/NewBranchDialog.tsx:142 src/components/NewBranchDialog.tsx:147 src/components/NewBranchDialog.tsx:154
 msgid "Create a Branch"
 msgstr ""
 
-#: src/components/NewBranchDialog.tsx:160 src/components/NewBranchDialog.tsx:167 src/components/NewTagDialog.tsx:420 src/components/NewTagDialog.tsx:434
+#: src/components/NewBranchDialog.tsx:155 src/components/NewBranchDialog.tsx:160 src/components/NewBranchDialog.tsx:167 src/components/NewTagDialog.tsx:420 src/components/NewTagDialog.tsx:429 src/components/NewTagDialog.tsx:434
 msgid "Name"
 msgstr ""
 
-#: src/components/NewBranchDialog.tsx:167 src/components/NewBranchDialog.tsx:174
+#: src/components/NewBranchDialog.tsx:162 src/components/NewBranchDialog.tsx:167 src/components/NewBranchDialog.tsx:174
 msgid "Enter a branch name"
 msgstr ""
 
-#: src/components/NewBranchDialog.tsx:169
+#: src/components/NewBranchDialog.tsx:164 src/components/NewBranchDialog.tsx:169
 msgid "Create branch based on…"
 msgstr ""
 
 #: src/components/NewBranchDialog.tsx:169 src/components/NewBranchDialog.tsx:176
 msgid "Create branch based on..."
 msgstr ""
 
-#: src/components/NewBranchDialog.tsx:199 src/components/NewBranchDialog.tsx:206
+#: src/components/NewBranchDialog.tsx:194 src/components/NewBranchDialog.tsx:199 src/components/NewBranchDialog.tsx:206
 msgid "Close this dialog without creating a new branch"
 msgstr ""
 
-#: src/components/NewBranchDialog.tsx:209 src/components/NewBranchDialog.tsx:216
+#: src/components/NewBranchDialog.tsx:204 src/components/NewBranchDialog.tsx:209 src/components/NewBranchDialog.tsx:216
 msgid "Create Branch"
 msgstr ""
 
-#: src/components/NewBranchDialog.tsx:300 src/components/NewBranchDialog.tsx:302
+#: src/components/NewBranchDialog.tsx:297 src/components/NewBranchDialog.tsx:300 src/components/NewBranchDialog.tsx:302
 msgid "The current branch. Pick this if you want to build on work done in this branch."
 msgstr ""
 
-#: src/components/NewBranchDialog.tsx:305 src/components/NewBranchDialog.tsx:307
+#: src/components/NewBranchDialog.tsx:302 src/components/NewBranchDialog.tsx:305 src/components/NewBranchDialog.tsx:307
 msgid "The default branch. Pick this if you want to start fresh from the default branch."
 msgstr ""
 
-#: src/components/NewBranchDialog.tsx:427 src/components/NewBranchDialog.tsx:434
+#: src/components/NewBranchDialog.tsx:419 src/components/NewBranchDialog.tsx:427 src/components/NewBranchDialog.tsx:434
 msgid "Creating branch…"
 msgstr ""
 
-#: src/components/NewBranchDialog.tsx:433 src/components/NewBranchDialog.tsx:434
-msgid "Creating branch..."
+#: src/components/NewBranchDialog.tsx:431 src/components/NewBranchDialog.tsx:437 src/components/NewBranchDialog.tsx:443 src/components/NewBranchDialog.tsx:444
+msgid "Failed to create branch."
 msgstr ""
 
-#: src/components/NewBranchDialog.tsx:437 src/components/NewBranchDialog.tsx:443 src/components/NewBranchDialog.tsx:444
-msgid "Failed to create branch."
+#: src/components/NewBranchDialog.tsx:433 src/components/NewBranchDialog.tsx:434
+msgid "Creating branch..."
 msgstr ""
 
-#: src/components/NewBranchDialog.tsx:444 src/components/NewBranchDialog.tsx:450 src/components/NewBranchDialog.tsx:451
+#: src/components/NewBranchDialog.tsx:440 src/components/NewBranchDialog.tsx:444 src/components/NewBranchDialog.tsx:450 src/components/NewBranchDialog.tsx:451
 msgid "Branch created."
 msgstr ""
 
-#: src/components/NewTagDialog.tsx:260 src/components/NewTagDialog.tsx:274
+#: src/components/NewTagDialog.tsx:260 src/components/NewTagDialog.tsx:264 src/components/NewTagDialog.tsx:274
 msgid "Create a new tag pointing to commit %1: %2 by %3"
 msgstr ""
 
-#: src/components/NewTagDialog.tsx:376 src/components/NewTagDialog.tsx:390
+#: src/components/NewTagDialog.tsx:376 src/components/NewTagDialog.tsx:379 src/components/NewTagDialog.tsx:390
 msgid "Creating tag…"
 msgstr ""
 
-#: src/components/NewTagDialog.tsx:384 src/components/NewTagDialog.tsx:398
+#: src/components/NewTagDialog.tsx:384 src/components/NewTagDialog.tsx:389 src/components/NewTagDialog.tsx:398
 msgid "Failed to create tag."
 msgstr ""
 
-#: src/components/NewTagDialog.tsx:391 src/components/NewTagDialog.tsx:405
+#: src/components/NewTagDialog.tsx:391 src/components/NewTagDialog.tsx:398 src/components/NewTagDialog.tsx:405
 msgid "Tag created."
 msgstr ""
 
-#: src/components/NewTagDialog.tsx:409 src/components/NewTagDialog.tsx:423
+#: src/components/NewTagDialog.tsx:409 src/components/NewTagDialog.tsx:418 src/components/NewTagDialog.tsx:423
 msgid "Create a Tag"
 msgstr ""
 
-#: src/components/NewTagDialog.tsx:427 src/components/NewTagDialog.tsx:441
+#: src/components/NewTagDialog.tsx:427 src/components/NewTagDialog.tsx:436 src/components/NewTagDialog.tsx:441
 msgid "Enter a tag name"
 msgstr ""
 
-#: src/components/NewTagDialog.tsx:429 src/components/NewTagDialog.tsx:443
+#: src/components/NewTagDialog.tsx:429 src/components/NewTagDialog.tsx:438 src/components/NewTagDialog.tsx:443
 msgid "Create tag pointing to…"
 msgstr ""
 
-#: src/components/NewTagDialog.tsx:437 src/components/NewTagDialog.tsx:452
+#: src/components/NewTagDialog.tsx:437 src/components/NewTagDialog.tsx:447 src/components/NewTagDialog.tsx:452
 msgid "Filter by commit message"
 msgstr ""
 
-#: src/components/NewTagDialog.tsx:438 src/components/NewTagDialog.tsx:453
+#: src/components/NewTagDialog.tsx:438 src/components/NewTagDialog.tsx:448 src/components/NewTagDialog.tsx:453
 msgid "Filter history of commits menu"
 msgstr ""
 
-#: src/components/NewTagDialog.tsx:467 src/components/NewTagDialog.tsx:484
+#: src/components/NewTagDialog.tsx:467 src/components/NewTagDialog.tsx:478 src/components/NewTagDialog.tsx:484
 msgid "Close this dialog without creating a new tag"
 msgstr ""
 
-#: src/components/NewTagDialog.tsx:474 src/components/NewTagDialog.tsx:491 src/components/TagMenu.tsx:201
+#: src/components/NewTagDialog.tsx:474 src/components/NewTagDialog.tsx:485 src/components/NewTagDialog.tsx:491 src/components/TagMenu.tsx:196 src/components/TagMenu.tsx:201
 msgid "Create a new tag"
 msgstr ""
 
-#: src/components/NewTagDialog.tsx:475 src/components/NewTagDialog.tsx:492
+#: src/components/NewTagDialog.tsx:475 src/components/NewTagDialog.tsx:486 src/components/NewTagDialog.tsx:492
 msgid "Create Tag"
 msgstr ""
 
 #: src/components/PastCommitNode.tsx:111 src/components/PastCommitNode.tsx:152 src/components/PastCommitNode.tsx:156 src/components/PastCommitNode.tsx:169
 msgid "View commit details"
 msgstr ""
 
@@ -1489,291 +1583,307 @@
 msgid "Select for compare"
 msgstr ""
 
 #: src/components/PastCommitNode.tsx:182 src/components/PastCommitNode.tsx:186 src/components/PastCommitNode.tsx:205
 msgid "Compare with selected"
 msgstr ""
 
-#: src/components/RebaseAction.tsx:100
+#: src/components/RebaseAction.tsx:100 src/components/RebaseAction.tsx:96
 msgid "Continue the rebase."
 msgstr ""
 
-#: src/components/RebaseAction.tsx:103
-msgid "Continue"
+#: src/components/RebaseAction.tsx:102 src/components/RebaseAction.tsx:106
+msgid "Pick another rebase action."
 msgstr ""
 
-#: src/components/RebaseAction.tsx:106
-msgid "Pick another rebase action."
+#: src/components/RebaseAction.tsx:103 src/components/RebaseAction.tsx:99
+msgid "Continue"
 msgstr ""
 
-#: src/components/RebaseAction.tsx:129
+#: src/components/RebaseAction.tsx:124 src/components/RebaseAction.tsx:129
 msgid "Skip the current commit."
 msgstr ""
 
-#: src/components/RebaseAction.tsx:131
+#: src/components/RebaseAction.tsx:126 src/components/RebaseAction.tsx:131
 msgid "Skip"
 msgstr ""
 
-#: src/components/RebaseAction.tsx:137
+#: src/components/RebaseAction.tsx:132 src/components/RebaseAction.tsx:137
 msgid "Abort the rebase."
 msgstr ""
 
-#: src/components/RebaseAction.tsx:139 src/components/RebaseAction.tsx:80
+#: src/components/RebaseAction.tsx:134 src/components/RebaseAction.tsx:139 src/components/RebaseAction.tsx:76 src/components/RebaseAction.tsx:80
 msgid "Abort"
 msgstr ""
 
-#: src/components/RebaseAction.tsx:77
+#: src/components/RebaseAction.tsx:73 src/components/RebaseAction.tsx:77
 msgid "Are you sure you want to abort the rebase?"
 msgstr ""
 
-#: src/components/ResetRevertDialog.tsx:125 src/components/ResetRevertDialog.tsx:127
+#: src/components/ResetRevertDialog.tsx:121 src/components/ResetRevertDialog.tsx:125 src/components/ResetRevertDialog.tsx:127
 msgid "Revert Changes"
 msgstr ""
 
-#: src/components/ResetRevertDialog.tsx:126 src/components/ResetRevertDialog.tsx:128
+#: src/components/ResetRevertDialog.tsx:122 src/components/ResetRevertDialog.tsx:126 src/components/ResetRevertDialog.tsx:128
 msgid "Reset Changes"
 msgstr ""
 
-#: src/components/ResetRevertDialog.tsx:139 src/components/ResetRevertDialog.tsx:141
+#: src/components/ResetRevertDialog.tsx:135 src/components/ResetRevertDialog.tsx:139 src/components/ResetRevertDialog.tsx:141
 msgid "These changes will be reverted. Only commit if you're sure you're okay losing these changes."
 msgstr ""
 
-#: src/components/ResetRevertDialog.tsx:142 src/components/ResetRevertDialog.tsx:144
+#: src/components/ResetRevertDialog.tsx:138 src/components/ResetRevertDialog.tsx:142 src/components/ResetRevertDialog.tsx:144
 msgid "All changes after commit %1 will be gone forever (hard reset). Are you sure?"
 msgstr ""
 
-#: src/components/ResetRevertDialog.tsx:166 src/components/ResetRevertDialog.tsx:179
+#: src/components/ResetRevertDialog.tsx:162 src/components/ResetRevertDialog.tsx:166 src/components/ResetRevertDialog.tsx:179
 msgid "Cancel changes"
 msgstr ""
 
-#: src/components/ResetRevertDialog.tsx:174 src/components/ResetRevertDialog.tsx:187
+#: src/components/ResetRevertDialog.tsx:170 src/components/ResetRevertDialog.tsx:174 src/components/ResetRevertDialog.tsx:187
 msgid "Submit changes"
 msgstr ""
 
-#: src/components/ResetRevertDialog.tsx:229
+#: src/components/ResetRevertDialog.tsx:224 src/components/ResetRevertDialog.tsx:229
 msgid "Discarding changes…"
 msgstr ""
 
 #: src/components/ResetRevertDialog.tsx:229 src/components/ResetRevertDialog.tsx:246
 msgid "Discarding changes..."
 msgstr ""
 
-#: src/components/ResetRevertDialog.tsx:235 src/components/ResetRevertDialog.tsx:252
+#: src/components/ResetRevertDialog.tsx:232 src/components/ResetRevertDialog.tsx:235 src/components/ResetRevertDialog.tsx:252
 msgid "Successfully discarded changes."
 msgstr ""
 
-#: src/components/ResetRevertDialog.tsx:240 src/components/ResetRevertDialog.tsx:257
+#: src/components/ResetRevertDialog.tsx:239 src/components/ResetRevertDialog.tsx:240 src/components/ResetRevertDialog.tsx:257
 msgid "Failed to discard changes."
 msgstr ""
 
-#: src/components/ResetRevertDialog.tsx:256
+#: src/components/ResetRevertDialog.tsx:256 src/components/ResetRevertDialog.tsx:258
 msgid "Reverting changes…"
 msgstr ""
 
 #: src/components/ResetRevertDialog.tsx:256 src/components/ResetRevertDialog.tsx:273
 msgid "Reverting changes..."
 msgstr ""
 
-#: src/components/ResetRevertDialog.tsx:262 src/components/ResetRevertDialog.tsx:279
+#: src/components/ResetRevertDialog.tsx:262 src/components/ResetRevertDialog.tsx:266 src/components/ResetRevertDialog.tsx:279
 msgid "Successfully reverted changes."
 msgstr ""
 
-#: src/components/ResetRevertDialog.tsx:267 src/components/ResetRevertDialog.tsx:284
+#: src/components/ResetRevertDialog.tsx:267 src/components/ResetRevertDialog.tsx:273 src/components/ResetRevertDialog.tsx:284
 msgid "Failed to revert changes."
 msgstr ""
 
-#: src/components/ResetRevertDialog.tsx:299 src/components/ResetRevertDialog.tsx:316
+#: src/components/ResetRevertDialog.tsx:299 src/components/ResetRevertDialog.tsx:309 src/components/ResetRevertDialog.tsx:316
 msgid "Revert '%1'"
 msgstr ""
 
-#: src/components/ResetRevertDialog.tsx:308 src/components/ResetRevertDialog.tsx:325
+#: src/components/ResetRevertDialog.tsx:308 src/components/ResetRevertDialog.tsx:318 src/components/ResetRevertDialog.tsx:325
 msgid "This reverts commit %1"
 msgstr ""
 
-#: src/components/SinglePastCommitInfo.tsx:159 src/components/SinglePastCommitInfo.tsx:169 src/components/SinglePastCommitInfo.tsx:180 src/components/SinglePastCommitInfo.tsx:182
+#: src/components/SinglePastCommitInfo.tsx:159 src/components/SinglePastCommitInfo.tsx:169 src/components/SinglePastCommitInfo.tsx:170 src/components/SinglePastCommitInfo.tsx:180 src/components/SinglePastCommitInfo.tsx:182
 msgid "Error loading commit data"
 msgstr ""
 
-#: src/components/SinglePastCommitInfo.tsx:168 src/components/SinglePastCommitInfo.tsx:180 src/components/SinglePastCommitInfo.tsx:201 src/components/SinglePastCommitInfo.tsx:212 src/components/SinglePastCommitInfo.tsx:214
+#: src/components/SinglePastCommitInfo.tsx:168 src/components/SinglePastCommitInfo.tsx:180 src/components/SinglePastCommitInfo.tsx:181 src/components/SinglePastCommitInfo.tsx:201 src/components/SinglePastCommitInfo.tsx:212 src/components/SinglePastCommitInfo.tsx:214
 msgid "Revert changes introduced by this commit"
 msgstr ""
 
-#: src/components/SinglePastCommitInfo.tsx:176 src/components/SinglePastCommitInfo.tsx:188 src/components/SinglePastCommitInfo.tsx:209 src/components/SinglePastCommitInfo.tsx:220 src/components/SinglePastCommitInfo.tsx:222
+#: src/components/SinglePastCommitInfo.tsx:176 src/components/SinglePastCommitInfo.tsx:188 src/components/SinglePastCommitInfo.tsx:189 src/components/SinglePastCommitInfo.tsx:209 src/components/SinglePastCommitInfo.tsx:220 src/components/SinglePastCommitInfo.tsx:222
 msgid "Discard changes introduced *after* this commit (hard reset)"
 msgstr ""
 
 #: src/components/StatusWidget.tsx:70 src/components/StatusWidget.tsx:74
 msgid "credentials required"
 msgstr ""
 
 #: src/components/TagMenu.tsx:157
 msgid "Fail to get the tags."
 msgstr ""
 
-#: src/components/TagMenu.tsx:186
+#: src/components/TagMenu.tsx:181 src/components/TagMenu.tsx:186
 msgid "Filter tag menu"
 msgstr ""
 
-#: src/components/TagMenu.tsx:202
+#: src/components/TagMenu.tsx:197 src/components/TagMenu.tsx:202
 msgid "New Tag"
 msgstr ""
 
 #: src/components/TagMenu.tsx:246 src/components/TagMenu.tsx:251
 msgid "Checkout to tag: %1"
 msgstr ""
 
-#: src/components/TagMenu.tsx:308 src/components/TagMenu.tsx:310
+#: src/components/TagMenu.tsx:304 src/components/TagMenu.tsx:308 src/components/TagMenu.tsx:310
 msgid "Creating a new tag is disabled"
 msgstr ""
 
-#: src/components/TagMenu.tsx:309 src/components/TagMenu.tsx:311
+#: src/components/TagMenu.tsx:305 src/components/TagMenu.tsx:309 src/components/TagMenu.tsx:311
 msgid "Error in creating new tag"
 msgstr ""
 
-#: src/components/TagMenu.tsx:45 src/components/TagMenu.tsx:47
+#: src/components/TagMenu.tsx:340
+msgid "Checkout tags is disabled"
+msgstr ""
+
+#: src/components/TagMenu.tsx:341
+msgid "The repository contains files with uncommitted changes. Please commit or discard these changes before switching to a tag."
+msgstr ""
+
+#: src/components/TagMenu.tsx:349
+msgid "Checking tag out…"
+msgstr ""
+
+#: src/components/TagMenu.tsx:362
+msgid "Tag checkout."
+msgstr ""
+
+#: src/components/TagMenu.tsx:45 src/components/TagMenu.tsx:46 src/components/TagMenu.tsx:47
 msgid "Unable to checkout tag"
 msgstr ""
 
-#: src/components/TagMenu.tsx:57 src/components/TagMenu.tsx:59
+#: src/components/TagMenu.tsx:57 src/components/TagMenu.tsx:58 src/components/TagMenu.tsx:59
 msgid "Please commit, stash, or discard your changes before you checkout tags."
 msgstr ""
 
-#: src/components/TagMenu.tsx:68 src/components/TagMenu.tsx:70
+#: src/components/TagMenu.tsx:68 src/components/TagMenu.tsx:69 src/components/TagMenu.tsx:70
 msgid "Failed to checkout tag."
 msgstr ""
 
-#: src/components/Toolbar.tsx:173 src/components/Toolbar.tsx:183
+#: src/components/Toolbar.tsx:173 src/components/Toolbar.tsx:178 src/components/Toolbar.tsx:183
 msgid "Pull latest changes"
 msgstr ""
 
-#: src/components/Toolbar.tsx:175 src/components/Toolbar.tsx:185
+#: src/components/Toolbar.tsx:175 src/components/Toolbar.tsx:180 src/components/Toolbar.tsx:185
 msgid " (behind by %1 commits)"
 msgstr ""
 
-#: src/components/Toolbar.tsx:180 src/components/Toolbar.tsx:190 src/components/Toolbar.tsx:208 src/components/Toolbar.tsx:218
+#: src/components/Toolbar.tsx:180 src/components/Toolbar.tsx:185 src/components/Toolbar.tsx:190 src/components/Toolbar.tsx:208 src/components/Toolbar.tsx:212 src/components/Toolbar.tsx:218
 msgid "No remote repository defined"
 msgstr ""
 
-#: src/components/Toolbar.tsx:200 src/components/Toolbar.tsx:210
+#: src/components/Toolbar.tsx:200 src/components/Toolbar.tsx:204 src/components/Toolbar.tsx:210
 msgid "Push committed changes"
 msgstr ""
 
-#: src/components/Toolbar.tsx:202 src/components/Toolbar.tsx:212
+#: src/components/Toolbar.tsx:202 src/components/Toolbar.tsx:206 src/components/Toolbar.tsx:212
 msgid " (ahead by %1 commits)"
 msgstr ""
 
-#: src/components/Toolbar.tsx:207 src/components/Toolbar.tsx:217
+#: src/components/Toolbar.tsx:207 src/components/Toolbar.tsx:211 src/components/Toolbar.tsx:217
 msgid "Publish branch"
 msgstr ""
 
-#: src/components/Toolbar.tsx:217 src/components/Toolbar.tsx:227
+#: src/components/Toolbar.tsx:217 src/components/Toolbar.tsx:221 src/components/Toolbar.tsx:227
 msgid "Refresh the repository to detect local and remote changes"
 msgstr ""
 
-#: src/components/Toolbar.tsx:236 src/components/Toolbar.tsx:240 src/components/Toolbar.tsx:250
+#: src/components/Toolbar.tsx:236 src/components/Toolbar.tsx:240 src/components/Toolbar.tsx:244 src/components/Toolbar.tsx:250
 msgid "Current repository: %1"
 msgstr ""
 
-#: src/components/Toolbar.tsx:245 src/components/Toolbar.tsx:248 src/components/Toolbar.tsx:258
+#: src/components/Toolbar.tsx:245 src/components/Toolbar.tsx:248 src/components/Toolbar.tsx:255 src/components/Toolbar.tsx:258
 msgid "Current Repository"
 msgstr ""
 
-#: src/components/Toolbar.tsx:269 src/components/Toolbar.tsx:279
+#: src/components/Toolbar.tsx:269 src/components/Toolbar.tsx:276 src/components/Toolbar.tsx:279
 msgid "Cherry picking in"
 msgstr ""
 
-#: src/components/Toolbar.tsx:272 src/components/Toolbar.tsx:273 src/components/Toolbar.tsx:291 src/components/Toolbar.tsx:301
+#: src/components/Toolbar.tsx:272 src/components/Toolbar.tsx:273 src/components/Toolbar.tsx:291 src/components/Toolbar.tsx:298 src/components/Toolbar.tsx:301
 msgid "Manage branches and tags"
 msgstr ""
 
-#: src/components/Toolbar.tsx:272 src/components/Toolbar.tsx:282
+#: src/components/Toolbar.tsx:272 src/components/Toolbar.tsx:279 src/components/Toolbar.tsx:282
 msgid "Detached Head at"
 msgstr ""
 
-#: src/components/Toolbar.tsx:275 src/components/Toolbar.tsx:285
+#: src/components/Toolbar.tsx:275 src/components/Toolbar.tsx:282 src/components/Toolbar.tsx:285
 msgid "Merging in"
 msgstr ""
 
-#: src/components/Toolbar.tsx:278 src/components/Toolbar.tsx:279 src/components/Toolbar.tsx:281 src/components/Toolbar.tsx:291
+#: src/components/Toolbar.tsx:278 src/components/Toolbar.tsx:279 src/components/Toolbar.tsx:281 src/components/Toolbar.tsx:288 src/components/Toolbar.tsx:291
 msgid "Current Branch"
 msgstr ""
 
-#: src/components/Toolbar.tsx:278 src/components/Toolbar.tsx:288
+#: src/components/Toolbar.tsx:278 src/components/Toolbar.tsx:285 src/components/Toolbar.tsx:288
 msgid "Rebasing"
 msgstr ""
 
-#: src/components/Toolbar.tsx:315 src/components/Toolbar.tsx:316 src/components/Toolbar.tsx:332 src/components/Toolbar.tsx:342
+#: src/components/Toolbar.tsx:315 src/components/Toolbar.tsx:316 src/components/Toolbar.tsx:332 src/components/Toolbar.tsx:342 src/components/Toolbar.tsx:345
 msgid "View branches"
 msgstr ""
 
-#: src/components/Toolbar.tsx:316 src/components/Toolbar.tsx:317 src/components/Toolbar.tsx:333 src/components/Toolbar.tsx:343
+#: src/components/Toolbar.tsx:316 src/components/Toolbar.tsx:317 src/components/Toolbar.tsx:333 src/components/Toolbar.tsx:343 src/components/Toolbar.tsx:346
 msgid "Branches"
 msgstr ""
 
-#: src/components/Toolbar.tsx:325 src/components/Toolbar.tsx:326 src/components/Toolbar.tsx:342 src/components/Toolbar.tsx:352
+#: src/components/Toolbar.tsx:325 src/components/Toolbar.tsx:326 src/components/Toolbar.tsx:342 src/components/Toolbar.tsx:352 src/components/Toolbar.tsx:355
 msgid "View tags"
 msgstr ""
 
-#: src/components/Toolbar.tsx:326 src/components/Toolbar.tsx:327 src/components/Toolbar.tsx:343 src/components/Toolbar.tsx:353
+#: src/components/Toolbar.tsx:326 src/components/Toolbar.tsx:327 src/components/Toolbar.tsx:343 src/components/Toolbar.tsx:353 src/components/Toolbar.tsx:356
 msgid "Tags"
 msgstr ""
 
 #: src/components/Toolbar.tsx:401 src/components/Toolbar.tsx:402
 msgid "Refreshing..."
 msgstr ""
 
 #: src/components/Toolbar.tsx:403 src/components/Toolbar.tsx:419 src/components/Toolbar.tsx:431
 msgid "Refreshing…"
 msgstr ""
 
-#: src/components/Toolbar.tsx:408 src/components/Toolbar.tsx:409 src/components/Toolbar.tsx:410 src/components/Toolbar.tsx:426 src/components/Toolbar.tsx:438
+#: src/components/Toolbar.tsx:408 src/components/Toolbar.tsx:409 src/components/Toolbar.tsx:410 src/components/Toolbar.tsx:426 src/components/Toolbar.tsx:438 src/components/Toolbar.tsx:440
 msgid "Successfully refreshed."
 msgstr ""
 
-#: src/components/Toolbar.tsx:414 src/components/Toolbar.tsx:415 src/components/Toolbar.tsx:416 src/components/Toolbar.tsx:432 src/components/Toolbar.tsx:444
+#: src/components/Toolbar.tsx:414 src/components/Toolbar.tsx:415 src/components/Toolbar.tsx:416 src/components/Toolbar.tsx:432 src/components/Toolbar.tsx:444 src/components/Toolbar.tsx:448
 msgid "Failed to refresh."
 msgstr ""
 
-#: src/components/diff/ImageDiff.tsx:142
+#: src/components/diff/ImageDiff.tsx:138 src/components/diff/ImageDiff.tsx:142
 msgid "View Image Diff in 2-up Mode"
 msgstr ""
 
-#: src/components/diff/ImageDiff.tsx:143
+#: src/components/diff/ImageDiff.tsx:139 src/components/diff/ImageDiff.tsx:143
 msgid "2-up"
 msgstr ""
 
-#: src/components/diff/ImageDiff.tsx:151
+#: src/components/diff/ImageDiff.tsx:147 src/components/diff/ImageDiff.tsx:151
 msgid "View Image Diff in Swipe Mode"
 msgstr ""
 
-#: src/components/diff/ImageDiff.tsx:152
+#: src/components/diff/ImageDiff.tsx:148 src/components/diff/ImageDiff.tsx:152
 msgid "Swipe"
 msgstr ""
 
-#: src/components/diff/ImageDiff.tsx:160
+#: src/components/diff/ImageDiff.tsx:156 src/components/diff/ImageDiff.tsx:160
 msgid "View Image Diff in Onion Skin Mode"
 msgstr ""
 
-#: src/components/diff/ImageDiff.tsx:161
+#: src/components/diff/ImageDiff.tsx:157 src/components/diff/ImageDiff.tsx:161
 msgid "Onion Skin"
 msgstr ""
 
-#: src/components/diff/ImageDiff.tsx:441
+#: src/components/diff/ImageDiff.tsx:426 src/components/diff/ImageDiff.tsx:441
 msgid "Failed to refresh Image diff."
 msgstr ""
 
-#: src/components/diff/ImageDiff.tsx:514 src/components/diff/NotebookDiff.ts:336 src/components/diff/NotebookDiff.ts:343 src/components/diff/PlainTextDiff.ts:244 src/components/diff/PlainTextDiff.ts:251 src/components/diff/PlainTextDiff.ts:294
+#: src/components/diff/ImageDiff.tsx:501 src/components/diff/ImageDiff.tsx:514 src/components/diff/NotebookDiff.ts:336 src/components/diff/NotebookDiff.ts:337 src/components/diff/NotebookDiff.ts:343 src/components/diff/PlainTextDiff.ts:244 src/components/diff/PlainTextDiff.ts:251 src/components/diff/PlainTextDiff.ts:282 src/components/diff/PlainTextDiff.ts:294
 msgid "Failed to load file diff."
 msgstr ""
 
-#: src/components/diff/ImageDiff.tsx:525
+#: src/components/diff/ImageDiff.tsx:512 src/components/diff/ImageDiff.tsx:525
 msgid "Error Loading Image Diff:"
 msgstr ""
 
-#: src/components/diff/NotebookDiff.ts:103
+#: src/components/diff/NotebookDiff.ts:100 src/components/diff/NotebookDiff.ts:103
 msgid "Hide unchanged cells"
 msgstr ""
 
 #: src/components/diff/NotebookDiff.ts:147
 msgid "Failed to refresh Notebook diff."
 msgstr ""
 
@@ -1785,23 +1895,23 @@
 msgid "Common Ancestor"
 msgstr ""
 
 #: src/components/diff/NotebookDiff.ts:277 src/components/diff/NotebookDiff.ts:284
 msgid "Failed to init notebook diff view: %1"
 msgstr ""
 
-#: src/components/diff/NotebookDiff.ts:347 src/components/diff/NotebookDiff.ts:354
+#: src/components/diff/NotebookDiff.ts:347 src/components/diff/NotebookDiff.ts:348 src/components/diff/NotebookDiff.ts:354
 msgid "Error Loading Notebook Diff:"
 msgstr ""
 
 #: src/components/diff/PlainTextDiff.ts:104 src/components/diff/PlainTextDiff.ts:111 src/components/diff/PlainTextDiff.ts:150
 msgid "Failed to get a valid file value."
 msgstr ""
 
-#: src/components/diff/PlainTextDiff.ts:250 src/components/diff/PlainTextDiff.ts:257 src/components/diff/PlainTextDiff.ts:300
+#: src/components/diff/PlainTextDiff.ts:250 src/components/diff/PlainTextDiff.ts:257 src/components/diff/PlainTextDiff.ts:293 src/components/diff/PlainTextDiff.ts:300
 msgid "Error Loading File Diff:"
 msgstr ""
 
 #: src/components/diff/PlainTextDiff.ts:53
 msgid "Control character"
 msgstr ""
 
@@ -1909,35 +2019,35 @@
 msgid "Push to left"
 msgstr ""
 
 #: src/components/diff/PlainTextDiff.ts:86
 msgid "Revert chunk"
 msgstr ""
 
-#: src/index.ts:100 src/index.ts:101 src/index.ts:102 src/index.ts:107 src/index.ts:94 src/index.ts:98
+#: src/index.ts:100 src/index.ts:101 src/index.ts:102 src/index.ts:107 src/index.ts:108 src/index.ts:94 src/index.ts:98
 msgid "git command not found - please ensure you have Git > 2 installed"
 msgstr ""
 
-#: src/index.ts:102 src/index.ts:106 src/index.ts:108 src/index.ts:109 src/index.ts:110 src/index.ts:115
+#: src/index.ts:102 src/index.ts:106 src/index.ts:108 src/index.ts:109 src/index.ts:110 src/index.ts:115 src/index.ts:116
 msgid "git command version must be > 2; got %1."
 msgstr ""
 
-#: src/index.ts:109 src/index.ts:113 src/index.ts:115 src/index.ts:116 src/index.ts:117 src/index.ts:122
+#: src/index.ts:109 src/index.ts:113 src/index.ts:115 src/index.ts:116 src/index.ts:117 src/index.ts:122 src/index.ts:123
 msgid "The versions of the JupyterLab Git server frontend and backend do not match. The @jupyterlab/git frontend extension has version: %1 while the python package has version %2. Please install identical version of jupyterlab-git Python package and the @jupyterlab/git extension. Try running: pip install --upgrade jupyterlab-git"
 msgstr ""
 
-#: src/index.ts:126 src/index.ts:130 src/index.ts:132 src/index.ts:133 src/index.ts:134 src/index.ts:139
+#: src/index.ts:126 src/index.ts:130 src/index.ts:132 src/index.ts:133 src/index.ts:134 src/index.ts:139 src/index.ts:140
 msgid "Failed to load the jupyterlab-git server extension"
 msgstr ""
 
-#: src/index.ts:128 src/index.ts:129 src/index.ts:130 src/index.ts:135
+#: src/index.ts:128 src/index.ts:129 src/index.ts:130 src/index.ts:135 src/index.ts:136
 msgid "Failed to load the jupyterlab-git server extension settings"
 msgstr ""
 
-#: src/index.ts:90 src/index.ts:91 src/index.ts:92 src/index.ts:97
+#: src/index.ts:90 src/index.ts:91 src/index.ts:92 src/index.ts:97 src/index.ts:98
 msgid "Failed to load settings for the Git Extension.\n"
 "%1"
 msgstr ""
 
 #: src/server.ts:27
 msgid "Git server extension is unavailable. Please ensure you have installed the JupyterLab Git server extension by running: pip install --upgrade jupyterlab-git. To confirm that the server extension is installed, run: jupyter server extension list."
 msgstr ""
@@ -1954,19 +2064,19 @@
 msgid "Loading remote repositories..."
 msgstr ""
 
 #: src/widgets/AdvancedPushForm.tsx:64
 msgid "Force Push"
 msgstr ""
 
-#: src/widgets/AuthorBox.ts:29
+#: src/widgets/AuthorBox.ts:29 src/widgets/AuthorBox.ts:30
 msgid "Committer name:"
 msgstr ""
 
-#: src/widgets/AuthorBox.ts:31
+#: src/widgets/AuthorBox.ts:31 src/widgets/AuthorBox.ts:32
 msgid "Committer email:"
 msgstr ""
 
 #: src/widgets/CredentialsBox.tsx:36 src/widgets/CredentialsBox.tsx:37 src/widgets/CredentialsBox.tsx:43 src/widgets/CredentialsBox.tsx:46
 msgid "username"
 msgstr ""
 
@@ -1998,11 +2108,7 @@
 msgid "If checked, the remote repository default branch will be downloaded instead of cloned"
 msgstr ""
 
 #: src/widgets/discardAllChanges.ts:18
 msgid "Your current changes forbid pulling the latest changes. Do you want to permanently discard those changes? This action cannot be undone."
 msgstr ""
 
-#: src/widgets/gitClone.tsx:38
-msgid "Git Clone"
-msgstr ""
-
```

### Comparing `jupyterlab_language_pack_ro_ro-4.1.post2/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyterlab_lsp.po` & `jupyterlab_language_pack_ro_ro-4.2.post0/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyterlab_lsp.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ro_ro-4.1.post2/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyterlab_recents.po` & `jupyterlab_language_pack_ro_ro-4.2.post0/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyterlab_recents.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ro_ro-4.1.post2/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyterlab_search_replace.po` & `jupyterlab_language_pack_ro_ro-4.2.post0/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyterlab_search_replace.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ro_ro-4.1.post2/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyterlab_spreadsheet_editor.po` & `jupyterlab_language_pack_ro_ro-4.2.post0/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyterlab_spreadsheet_editor.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ro_ro-4.1.post2/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyterlab_tour.po` & `jupyterlab_language_pack_ro_ro-4.2.post0/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyterlab_tour.po`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 "X-Crowdin-Project: jupyterlab\n"
 "X-Crowdin-Project-ID: 409874\n"
 "X-Crowdin-Language: ro\n"
 "X-Crowdin-File: /main/extensions/jupyterlab_tour/locale/jupyterlab_tour.pot\n"
 "X-Crowdin-File-ID: 205\n"
 "Language-Team: Romanian\n"
 "Language: ro_RO\n"
-"PO-Revision-Date: 2023-11-09 13:38\n"
+"PO-Revision-Date: 2024-03-29 11:18\n"
 
 #: /schema/user-tours.json:/description
 msgctxt "schema"
 msgid "Configuration for user-defined tours. This schema is generated from https://github.com/gilbarbara/react-joyride/blob/master/types/index.d.ts"
 msgstr ""
 
 #: /schema/user-tours.json:/jupyter.lab.setting-icon-label
@@ -135,15 +135,15 @@
 msgid "Settings"
 msgstr ""
 
 #: src/defaults.tsx:138
 msgid ": common settings and an advanced settings editor"
 msgstr ""
 
-#: src/defaults.tsx:141 src/defaults.tsx:636 src/plugin.tsx:143
+#: src/defaults.tsx:141 src/defaults.tsx:636 src/plugin.tsx:143 src/plugin.tsx:144
 msgid "Help"
 msgstr ""
 
 #: src/defaults.tsx:142 src/defaults.tsx:637
 msgid ": help links"
 msgstr ""
 
@@ -395,38 +395,38 @@
 msgid "Validation errors found: fix them in Advanced Settings"
 msgstr ""
 
 #: src/notebookTourManager.ts:124
 msgid "Error encountered adding notebook tour %1 (%2)"
 msgstr ""
 
-#: src/plugin.tsx:104
+#: src/plugin.tsx:100 src/plugin.tsx:99
+msgid "Launch a Tour"
+msgstr ""
+
+#: src/plugin.tsx:104 src/plugin.tsx:105
 msgid "Launch a tour.\n"
 "If no id provided, prompt the user.\n"
 "Arguments {id: Tour ID}"
 msgstr ""
 
-#: src/plugin.tsx:115
+#: src/plugin.tsx:115 src/plugin.tsx:116
 msgid "Choose a tour"
 msgstr ""
 
-#: src/plugin.tsx:132
+#: src/plugin.tsx:132 src/plugin.tsx:133
 msgid "Add a tour"
 msgstr ""
 
-#: src/plugin.tsx:133
+#: src/plugin.tsx:133 src/plugin.tsx:134
 msgid "Add a tour and returns it.\n"
 "Arguments {tour: ITour}\n"
 "Returns `null` if a failure occurs."
 msgstr ""
 
-#: src/plugin.tsx:99
-msgid "Launch a Tour"
-msgstr ""
-
 #: src/tourManager.ts:142
 msgid "Fail to add tour '%1' (%2)"
 msgstr ""
 
 #: src/tourManager.ts:172
 msgid "Error creating new tour. TourHandler id's must be unique.\n"
 "Tutorial with the id: '%1' already exists."
```

### Comparing `jupyterlab_language_pack_ro_ro-4.1.post2/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyterlab_widgets.po` & `jupyterlab_language_pack_ro_ro-4.2.post0/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupyterlab_widgets.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ro_ro-4.1.post2/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupytext.po` & `jupyterlab_language_pack_ro_ro-4.2.post0/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/jupytext.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ro_ro-4.1.post2/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/nbdime.po` & `jupyterlab_language_pack_ro_ro-4.2.post0/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/nbdime.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ro_ro-4.1.post2/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/notebook.po` & `jupyterlab_language_pack_ro_ro-4.2.post0/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/notebook.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ro_ro-4.1.post2/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/retrolab.po` & `jupyterlab_language_pack_ro_ro-4.2.post0/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/retrolab.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ro_ro-4.1.post2/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/spellchecker.po` & `jupyterlab_language_pack_ro_ro-4.2.post0/jupyterlab_language_pack_ro_RO/locale/ro_RO/LC_MESSAGES/spellchecker.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ro_ro-4.1.post2/.gitignore` & `jupyterlab_language_pack_ro_ro-4.2.post0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ro_ro-4.1.post2/LICENSE.txt` & `jupyterlab_language_pack_ro_ro-4.2.post0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ro_ro-4.1.post2/pyproject.toml` & `jupyterlab_language_pack_ro_ro-4.2.post0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ro_ro-4.1.post2/PKG-INFO` & `jupyterlab_language_pack_ro_ro-4.2.post0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyterlab-language-pack-ro-RO
-Version: 4.1.post2
+Version: 4.2.post0
 Summary: JupyterLab Romanian (Romania) Language Pack
 Project-URL: homepage, https://github.com/jupyterlab/language-packs
 Author-email: Project Jupyter Contributors <jupyter@googlegroups.com>
 License: Copyright (c) 2023 Project Jupyter Contributors
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

