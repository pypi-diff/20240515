# Comparing `tmp/jupyterlab_language_pack_ru_ru-4.1.post2.tar.gz` & `tmp/jupyterlab_language_pack_ru_ru-4.2.post0.tar.gz`

## Comparing `jupyterlab_language_pack_ru_ru-4.1.post2.tar` & `jupyterlab_language_pack_ru_ru-4.2.post0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.1.post2/.copier-answers.yml
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.1.post2/CONTRIBUTORS.md
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.1.post2/jupyterlab_language_pack_ru_RU/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.1.post2/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/.gitkeep
--rw-r--r--   0        0        0     6727 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.1.post2/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/dask_labextension.po
--rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.1.post2/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyter_archive.po
--rw-r--r--   0        0        0     6550 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.1.post2/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyter_collaboration.po
--rw-r--r--   0        0        0    11669 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.1.post2/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyter_resource_usage.po
--rw-r--r--   0        0        0   302012 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.1.post2/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyterlab.po
--rw-r--r--   0        0        0   161221 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.1.post2/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyterlab_git.po
--rw-r--r--   0        0        0    77017 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.1.post2/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyterlab_lsp.po
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.1.post2/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyterlab_recents.po
--rw-r--r--   0        0        0     7753 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.1.post2/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyterlab_search_replace.po
--rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.1.post2/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyterlab_spreadsheet_editor.po
--rw-r--r--   0        0        0    13434 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.1.post2/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyterlab_tour.po
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.1.post2/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyterlab_widgets.po
--rw-r--r--   0        0        0     7933 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.1.post2/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupytext.po
--rw-r--r--   0        0        0     5641 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.1.post2/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/nbdime.po
--rw-r--r--   0        0        0    15703 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.1.post2/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/notebook.po
--rw-r--r--   0        0        0     6364 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.1.post2/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/retrolab.po
--rw-r--r--   0        0        0     8270 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.1.post2/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/spellchecker.po
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.1.post2/.gitignore
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.1.post2/LICENSE.txt
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.1.post2/README.md
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.1.post2/pyproject.toml
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.1.post2/PKG-INFO
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.2.post0/.copier-answers.yml
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.2.post0/CONTRIBUTORS.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.2.post0/jupyterlab_language_pack_ru_RU/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.2.post0/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/.gitkeep
+-rw-r--r--   0        0        0     6727 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.2.post0/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/dask_labextension.po
+-rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.2.post0/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyter_archive.po
+-rw-r--r--   0        0        0     6550 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.2.post0/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyter_collaboration.po
+-rw-r--r--   0        0        0    11669 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.2.post0/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyter_resource_usage.po
+-rw-r--r--   0        0        0   362375 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.2.post0/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyterlab.po
+-rw-r--r--   0        0        0   161221 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.2.post0/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyterlab_git.po
+-rw-r--r--   0        0        0    77017 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.2.post0/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyterlab_lsp.po
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.2.post0/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyterlab_recents.po
+-rw-r--r--   0        0        0     7753 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.2.post0/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyterlab_search_replace.po
+-rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.2.post0/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyterlab_spreadsheet_editor.po
+-rw-r--r--   0        0        0    13548 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.2.post0/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyterlab_tour.po
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.2.post0/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyterlab_widgets.po
+-rw-r--r--   0        0        0     7933 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.2.post0/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupytext.po
+-rw-r--r--   0        0        0     5641 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.2.post0/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/nbdime.po
+-rw-r--r--   0        0        0    15703 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.2.post0/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/notebook.po
+-rw-r--r--   0        0        0     6364 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.2.post0/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/retrolab.po
+-rw-r--r--   0        0        0     8270 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.2.post0/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/spellchecker.po
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.2.post0/.gitignore
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.2.post0/LICENSE.txt
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.2.post0/README.md
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.2.post0/pyproject.toml
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ru_ru-4.2.post0/PKG-INFO
```

### Comparing `jupyterlab_language_pack_ru_ru-4.1.post2/CONTRIBUTORS.md` & `jupyterlab_language_pack_ru_ru-4.2.post0/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ru_ru-4.1.post2/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/dask_labextension.po` & `jupyterlab_language_pack_ru_ru-4.2.post0/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/dask_labextension.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ru_ru-4.1.post2/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyter_archive.po` & `jupyterlab_language_pack_ru_ru-4.2.post0/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyter_archive.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ru_ru-4.1.post2/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyter_collaboration.po` & `jupyterlab_language_pack_ru_ru-4.2.post0/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyter_collaboration.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ru_ru-4.1.post2/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyter_resource_usage.po` & `jupyterlab_language_pack_ru_ru-4.2.post0/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyter_resource_usage.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ru_ru-4.1.post2/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyterlab.po` & `jupyterlab_language_pack_ru_ru-4.2.post0/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyterlab.po`

 * *Files 27% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 "X-Crowdin-Project: jupyterlab\n"
 "X-Crowdin-Project-ID: 409874\n"
 "X-Crowdin-Language: ru\n"
 "X-Crowdin-File: /main/jupyterlab/locale/jupyterlab.pot\n"
 "X-Crowdin-File-ID: 191\n"
 "Language-Team: Russian\n"
 "Language: ru_RU\n"
-"PO-Revision-Date: 2024-02-07 16:49\n"
+"PO-Revision-Date: 2024-05-06 08:14\n"
 
 #: /examples/federated/md_package/schema/plugin.json:/description /packages/markdownviewer-extension/schema/plugin.json:/description
 msgctxt "schema"
 msgid "Markdown viewer settings."
 msgstr "Настройки просмотра Markdown."
 
 #: /examples/federated/md_package/schema/plugin.json:/jupyter.lab.setting-icon-label /packages/markdownviewer-extension/schema/plugin.json:/jupyter.lab.setting-icon-label
@@ -1041,14 +1041,24 @@
 msgstr "Максимально допустимое различие, в миллисекундах, между последними измененными временными метками на диске и клиентом"
 
 #: /packages/docmanager-extension/schema/plugin.json:/properties/lastModifiedCheckMargin/title
 msgctxt "settings"
 msgid "Margin for last modified timestamp check"
 msgstr "Отступ для последней измененной отметки времени"
 
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
 msgstr "Нужно ли предлагать переименовать файл без названия при первом сохранении вручную."
 
 #: /packages/docmanager-extension/schema/plugin.json:/properties/renameUntitledFileOnSave/title
 msgctxt "settings"
@@ -1143,29 +1153,49 @@
 msgstr "Файловый менеджер"
 
 #: /packages/filebrowser-extension/schema/browser.json:/properties/filterDirectories/description
 msgctxt "settings"
 msgid "Whether to apply the search on directories"
 msgstr "Применить ли поиск по каталогам"
 
+#: /packages/filebrowser-extension/schema/browser.json:/properties/filterDirectories/description
+msgctxt "settings"
+msgid "Whether to apply the search on folders"
+msgstr ""
+
 #: /packages/filebrowser-extension/schema/browser.json:/properties/filterDirectories/title
 msgctxt "settings"
 msgid "Filter directories"
 msgstr "Фильтр директорий"
 
+#: /packages/filebrowser-extension/schema/browser.json:/properties/filterDirectories/title
+msgctxt "settings"
+msgid "Filter folders"
+msgstr ""
+
 #: /packages/filebrowser-extension/schema/browser.json:/properties/navigateToCurrentDirectory/description
 msgctxt "settings"
 msgid "Whether to automatically navigate to a document's current directory"
 msgstr "Нужно ли автоматически перемещаться в текущий каталог документа"
 
+#: /packages/filebrowser-extension/schema/browser.json:/properties/navigateToCurrentDirectory/description
+msgctxt "settings"
+msgid "Whether to automatically navigate to a document's current folder"
+msgstr ""
+
 #: /packages/filebrowser-extension/schema/browser.json:/properties/navigateToCurrentDirectory/title
 msgctxt "settings"
 msgid "Navigate to current directory"
 msgstr "Перейти в текущий каталог"
 
+#: /packages/filebrowser-extension/schema/browser.json:/properties/navigateToCurrentDirectory/title
+msgctxt "settings"
+msgid "Navigate to current folder"
+msgstr ""
+
 #: /packages/filebrowser-extension/schema/browser.json:/properties/showFileCheckboxes/description
 msgctxt "settings"
 msgid "Whether to show checkboxes next to files and folders"
 msgstr "Показывать ли флажки рядом с файлами и папками"
 
 #: /packages/filebrowser-extension/schema/browser.json:/properties/showFileCheckboxes/title
 msgctxt "settings"
@@ -1775,14 +1805,19 @@
 #: /packages/notebook-extension/schema/export.json:/description
 msgctxt "schema"
 msgid "Notebook Export settings."
 msgstr "Настройки экспорта блокнота."
 
 #: /packages/notebook-extension/schema/export.json:/jupyter.lab.menus/main[0]/items[1]/submenu/label
 msgctxt "menu"
+msgid "Save and Export Notebook As"
+msgstr ""
+
+#: /packages/notebook-extension/schema/export.json:/jupyter.lab.menus/main[0]/items[1]/submenu/label
+msgctxt "menu"
 msgid "Save and Export Notebook As…"
 msgstr "Сохранить и экспортировать блокнот как…"
 
 #: /packages/notebook-extension/schema/export.json:/title
 msgctxt "schema"
 msgid "Notebook Export"
 msgstr "Экспорт блокнота"
@@ -2448,51 +2483,74 @@
 msgstr "Префикс локализованных строк"
 
 #: /packages/translation-extension/schema/plugin.json:/title
 msgctxt "schema"
 msgid "Language"
 msgstr "Язык"
 
-#: packages/application-extension/src/index.tsx:1143 packages/application-extension/src/index.tsx:1148
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
+msgstr "Путь %1 не найден. JupyterLab перенаправлен в: %2"
+
+#: packages/application-extension/src/index.tsx:1014 packages/application-extension/src/index.tsx:999
+msgid "Path Not Found"
+msgstr "Путь не найден"
+
+#: packages/application-extension/src/index.tsx:1143 packages/application-extension/src/index.tsx:1148 packages/application-extension/src/index.tsx:1158 packages/application-extension/src/index.tsx:1163
 msgid "Property Inspector"
 msgstr "Инспектор свойств"
 
-#: packages/application-extension/src/index.tsx:1236
+#: packages/application-extension/src/index.tsx:1236 packages/application-extension/src/index.tsx:1251
 msgid "Simple Interface (%1)"
 msgstr "Простой интерфейс (%1)"
 
-#: packages/application-extension/src/index.tsx:1238 packages/application-extension/src/index.tsx:450
+#: packages/application-extension/src/index.tsx:1238 packages/application-extension/src/index.tsx:1253 packages/application-extension/src/index.tsx:450 packages/application-extension/src/index.tsx:471
 msgid "Simple Interface"
 msgstr "Упрощенный интерфейс"
 
-#: packages/application-extension/src/index.tsx:1246
+#: packages/application-extension/src/index.tsx:1246 packages/application-extension/src/index.tsx:1261
 msgid "Simple"
 msgstr "Простой"
 
-#: packages/application-extension/src/index.tsx:1286 packages/application-extension/src/index.tsx:856 packages/apputils/src/toolbar/factory.ts:33 packages/extensionmanager/src/model.ts:529 packages/extensionmanager/src/model.ts:551 packages/mainmenu-extension/src/index.ts:770
+#: packages/application-extension/src/index.tsx:1286 packages/application-extension/src/index.tsx:1301 packages/application-extension/src/index.tsx:856 packages/application-extension/src/index.tsx:871 packages/apputils/src/toolbar/factory.ts:33 packages/extensionmanager/src/model.ts:529 packages/extensionmanager/src/model.ts:551 packages/mainmenu-extension/src/index.ts:767 packages/mainmenu-extension/src/index.ts:770
 msgid "Information"
 msgstr "Информация"
 
-#: packages/application-extension/src/index.tsx:1287
+#: packages/application-extension/src/index.tsx:1287 packages/application-extension/src/index.tsx:1302
 msgid "Context menu customization has changed. You will need to reload JupyterLab to see the changes."
 msgstr "Контекстное меню изменилось. Вам нужно будет перезагрузить JupyterLab для просмотра изменений."
 
-#: packages/application-extension/src/index.tsx:1292 packages/application-extension/src/index.tsx:862 packages/apputils/src/toolbar/factory.ts:39 packages/docmanager-extension/src/index.tsx:750 packages/mainmenu-extension/src/index.ts:776
+#: packages/application-extension/src/index.tsx:1292 packages/application-extension/src/index.tsx:1307 packages/application-extension/src/index.tsx:862 packages/application-extension/src/index.tsx:877 packages/apputils/src/toolbar/factory.ts:39 packages/docmanager-extension/src/index.tsx:750 packages/docmanager-extension/src/index.tsx:762 packages/mainmenu-extension/src/index.ts:773 packages/mainmenu-extension/src/index.ts:776
 msgid "Reload"
 msgstr "Перезагрузить"
 
-#: packages/application-extension/src/index.tsx:135 packages/apputils-extension/src/index.ts:319 packages/documentsearch-extension/src/index.ts:463 packages/logconsole-extension/src/index.tsx:246 packages/mainmenu-extension/src/index.ts:236 packages/mainmenu-extension/src/index.ts:240 packages/mainmenu-extension/src/index.ts:250 packages/statusbar-extension/src/index.ts:48
+#: packages/application-extension/src/index.tsx:135 packages/apputils-extension/src/index.ts:319 packages/apputils-extension/src/index.ts:323 packages/documentsearch-extension/src/index.ts:463 packages/documentsearch-extension/src/index.ts:469 packages/logconsole-extension/src/index.tsx:246 packages/mainmenu-extension/src/index.ts:236 packages/mainmenu-extension/src/index.ts:237 packages/mainmenu-extension/src/index.ts:240 packages/mainmenu-extension/src/index.ts:241 packages/mainmenu-extension/src/index.ts:250 packages/mainmenu-extension/src/index.ts:251 packages/statusbar-extension/src/index.ts:48
 msgid "Main Area"
 msgstr "Основная область"
 
 #: packages/application-extension/src/index.tsx:139
 msgid "Shift+Right Click for Browser Menu"
 msgstr "Shift+правый клик для меню браузера"
 
-#: packages/application-extension/src/index.tsx:1468
+#: packages/application-extension/src/index.tsx:1468 packages/application-extension/src/index.tsx:1483
 msgid "Switch Sidebar Side"
 msgstr "Переключить боковую панель"
 
 #: packages/application-extension/src/index.tsx:239
 msgid "Close Tab"
 msgstr "Закрыть вкладку"
 
@@ -2500,168 +2558,172 @@
 msgid "Close All Other Tabs"
 msgstr "Закрыть остальные вкладки"
 
 #: packages/application-extension/src/index.tsx:273
 msgid "Close Tabs to Right"
 msgstr "Закрыть вкладки справа"
 
-#: packages/application-extension/src/index.tsx:288
+#: packages/application-extension/src/index.tsx:288 packages/application-extension/src/index.tsx:296
 msgid "Activate Next Tab"
 msgstr "Перейти к следующей вкладке"
 
-#: packages/application-extension/src/index.tsx:295
+#: packages/application-extension/src/index.tsx:295 packages/application-extension/src/index.tsx:303
 msgid "Activate Previous Tab"
 msgstr "Перейти к предыдущей вкладке"
 
-#: packages/application-extension/src/index.tsx:302
+#: packages/application-extension/src/index.tsx:302 packages/application-extension/src/index.tsx:310
 msgid "Activate Next Tab Bar"
 msgstr "Перейти к следующей панели вкладок"
 
-#: packages/application-extension/src/index.tsx:309
+#: packages/application-extension/src/index.tsx:309 packages/application-extension/src/index.tsx:317
 msgid "Activate Previous Tab Bar"
 msgstr "Перейти к предыдущей панели вкладок"
 
-#: packages/application-extension/src/index.tsx:316
+#: packages/application-extension/src/index.tsx:316 packages/application-extension/src/index.tsx:324
 msgid "Close All Tabs"
 msgstr "Закрыть все вкладки"
 
-#: packages/application-extension/src/index.tsx:323
+#: packages/application-extension/src/index.tsx:323 packages/application-extension/src/index.tsx:331
 msgid "Show Header"
 msgstr "Показать заголовок"
 
-#: packages/application-extension/src/index.tsx:334
+#: packages/application-extension/src/index.tsx:334 packages/application-extension/src/index.tsx:342
 msgid "Show Left Sidebar"
 msgstr "Показать левую боковую панель"
 
-#: packages/application-extension/src/index.tsx:350
+#: packages/application-extension/src/index.tsx:350 packages/application-extension/src/index.tsx:358
 msgid "Show Right Sidebar"
 msgstr "Показать правую боковую панель"
 
-#: packages/application-extension/src/index.tsx:366
+#: packages/application-extension/src/index.tsx:366 packages/application-extension/src/index.tsx:378
 msgid "Toggle Sidebar Element"
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:399
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
 msgstr "Показать правую панель активности"
 
-#: packages/application-extension/src/index.tsx:400
+#: packages/application-extension/src/index.tsx:400 packages/application-extension/src/index.tsx:421
 msgid "Show Left Activity Bar"
 msgstr "Показать левую панель активности"
 
-#: packages/application-extension/src/index.tsx:419
+#: packages/application-extension/src/index.tsx:419 packages/application-extension/src/index.tsx:440
 msgid "Presentation Mode"
 msgstr "Режим презентации"
 
-#: packages/application-extension/src/index.tsx:430
+#: packages/application-extension/src/index.tsx:430 packages/application-extension/src/index.tsx:451
 msgid "Set %1 mode."
 msgstr "Установить режим %1."
 
-#: packages/application-extension/src/index.tsx:431
+#: packages/application-extension/src/index.tsx:431 packages/application-extension/src/index.tsx:452
 msgid "Set the layout `mode`."
 msgstr "Установите макет `mode`."
 
-#: packages/application-extension/src/index.tsx:432
+#: packages/application-extension/src/index.tsx:432 packages/application-extension/src/index.tsx:453
 msgid "The layout `mode` can be \"single-document\" or \"multiple-document\"."
 msgstr "`mode` макета может быть \"single-document\" или \"multiple-document\"."
 
-#: packages/application-extension/src/index.tsx:462
+#: packages/application-extension/src/index.tsx:462 packages/application-extension/src/index.tsx:483
 msgid "Reset Default Layout"
 msgstr "Сбросить макет по умолчанию"
 
-#: packages/application-extension/src/index.tsx:592
+#: packages/application-extension/src/index.tsx:592 packages/application-extension/src/index.tsx:613
 msgid "Error Registering Plugins"
 msgstr "Ошибка регистрации плагинов"
 
-#: packages/application-extension/src/index.tsx:642
+#: packages/application-extension/src/index.tsx:642 packages/application-extension/src/index.tsx:657
 msgid "Build Complete"
 msgstr "Сборка завершена"
 
-#: packages/application-extension/src/index.tsx:645
+#: packages/application-extension/src/index.tsx:645 packages/application-extension/src/index.tsx:660
 msgid "Build successfully completed, reload page?"
 msgstr "Сборка завершена, перезагрузить страницу?"
 
-#: packages/application-extension/src/index.tsx:647
+#: packages/application-extension/src/index.tsx:647 packages/application-extension/src/index.tsx:662
 msgid "You will lose any unsaved changes."
 msgstr "Вы потеряете все несохраненные изменения."
 
-#: packages/application-extension/src/index.tsx:652
+#: packages/application-extension/src/index.tsx:652 packages/application-extension/src/index.tsx:667
 msgid "Reload Without Saving"
 msgstr "Перезагрузить без сохранения"
 
-#: packages/application-extension/src/index.tsx:655
+#: packages/application-extension/src/index.tsx:655 packages/application-extension/src/index.tsx:670
 msgid "Save and Reload"
 msgstr "Сохранить и Перезагрузить"
 
-#: packages/application-extension/src/index.tsx:668
+#: packages/application-extension/src/index.tsx:668 packages/application-extension/src/index.tsx:683
 msgid "Save Failed"
 msgstr "Не удалось сохранить"
 
-#: packages/application-extension/src/index.tsx:677
+#: packages/application-extension/src/index.tsx:677 packages/application-extension/src/index.tsx:692
 msgid "Build Failed"
 msgstr "Сборка завершилась ошибкой"
 
-#: packages/application-extension/src/index.tsx:695
+#: packages/application-extension/src/index.tsx:695 packages/application-extension/src/index.tsx:710
 msgid "JupyterLab build is suggested:"
 msgstr "Предлагается сборка JupyterLab:"
 
-#: packages/application-extension/src/index.tsx:702
+#: packages/application-extension/src/index.tsx:702 packages/application-extension/src/index.tsx:717
 msgid "Build Recommended"
 msgstr "Собирать рекомендуемое"
 
-#: packages/application-extension/src/index.tsx:706
+#: packages/application-extension/src/index.tsx:706 packages/application-extension/src/index.tsx:721
 msgid "Build"
 msgstr "Собрать"
 
-#: packages/application-extension/src/index.tsx:772
+#: packages/application-extension/src/index.tsx:772 packages/application-extension/src/index.tsx:787
 msgid "Are you sure you want to exit JupyterLab?\n\n"
 "Any unsaved changes will be lost."
 msgstr "Вы уверены, что хотите выйти? Все несохраненные изменения будут потеряны."
 
-#: packages/application-extension/src/index.tsx:857
+#: packages/application-extension/src/index.tsx:857 packages/application-extension/src/index.tsx:872
 msgid "User layout customization has changed. You may need to reload JupyterLab to see the changes."
 msgstr "Пользовательская настройка макета изменилась. Возможно, вам придется перезагрузить JupyterLab, чтобы увидеть изменения."
 
-#: packages/application-extension/src/index.tsx:990
-msgid "The path: %1 was not found. JupyterLab redirected to: %2"
-msgstr "Путь %1 не найден. JupyterLab перенаправлен в: %2"
-
-#: packages/application-extension/src/index.tsx:999
-msgid "Path Not Found"
-msgstr "Путь не найден"
-
 #: packages/application/src/connectionlost.ts:19
 msgid "Server Connection Error"
 msgstr "Ошибка соединения с сервером"
 
 #: packages/application/src/connectionlost.ts:20
 msgid "A connection to the Jupyter server could not be established.\n"
 "JupyterLab will continue trying to reconnect.\n"
 "Check your network connection or Jupyter server configuration.\n"
 msgstr "Подключение к серверу Jupyter не может быть установлено.\n"
 "JupyterLab продолжит пытаться переподключиться.\n"
 "Проверьте Ваше подключение к сети или конфигурацию сервера Jupyter.\n"
 
-#: packages/application/src/shell.ts:734
+#: packages/application/src/shell.ts:734 packages/application/src/shell.ts:741
 msgid "main menu"
 msgstr ""
 
-#: packages/application/src/shell.ts:738 packages/application/src/shell.ts:742
+#: packages/application/src/shell.ts:738 packages/application/src/shell.ts:742 packages/application/src/shell.ts:745 packages/application/src/shell.ts:749
 msgid "main sidebar"
 msgstr "основная боковая панель"
 
-#: packages/application/src/shell.ts:746 packages/application/src/shell.ts:750
+#: packages/application/src/shell.ts:746 packages/application/src/shell.ts:750 packages/application/src/shell.ts:753 packages/application/src/shell.ts:757
 msgid "alternate sidebar"
 msgstr "альтернативная боковая панель"
 
-#: packages/application/src/utils.ts:148
+#: packages/application/src/utils.ts:148 packages/application/src/utils.ts:253
 msgid "%1 and %2"
 msgstr "%1 и %2"
 
 #: packages/apputils-extension/src/announcements.ts:102
+msgid "Would you like to get notified about official Jupyter news?"
+msgstr ""
+
+#: packages/apputils-extension/src/announcements.ts:102
 msgid "Would you like to receive official Jupyter news?\n"
 "Please read the privacy policy."
 msgstr "Вы хотели бы получать официальные новости от Jupyter?\n"
 "Пожалуйста, прочитайте политику конфиденциальности."
 
 #: packages/apputils-extension/src/announcements.ts:110
 msgid "Open privacy policy"
@@ -2713,47 +2775,51 @@
 msgid "Clear Workspace"
 msgstr "Очистить рабочую область"
 
 #: packages/apputils-extension/src/index.ts:290
 msgid "Print…"
 msgstr "Печать…"
 
-#: packages/apputils-extension/src/index.ts:321
+#: packages/apputils-extension/src/index.ts:321 packages/apputils-extension/src/index.ts:325
 msgid "Show Header Above Content"
 msgstr "Показывать заголовок над содержимым"
 
-#: packages/apputils-extension/src/index.ts:429
+#: packages/apputils-extension/src/index.ts:429 packages/apputils-extension/src/index.ts:438
 msgid "Load state for the current workspace."
 msgstr "Статус загрузки для текущей рабочей области."
 
-#: packages/apputils-extension/src/index.ts:493
+#: packages/apputils-extension/src/index.ts:493 packages/apputils-extension/src/index.ts:502
 msgid "Reset Application State"
 msgstr "Сбросить состояние приложения"
 
-#: packages/apputils-extension/src/index.ts:504
+#: packages/apputils-extension/src/index.ts:504 packages/apputils-extension/src/index.ts:513
 msgid "Reset state when loading for the workspace."
 msgstr "Сбросить состояние при загрузке для рабочей области."
 
-#: packages/apputils-extension/src/index.ts:595
+#: packages/apputils-extension/src/index.ts:595 packages/apputils-extension/src/index.ts:604
 msgid "Run First Enabled Command"
 msgstr "Запуск первой включенной команды"
 
-#: packages/apputils-extension/src/index.ts:613
+#: packages/apputils-extension/src/index.ts:613 packages/apputils-extension/src/index.ts:622
 msgid "Run All Enabled Commands Passed as Args"
 msgstr "Выполнить все команды, передаваемые как аргументы"
 
 #: packages/apputils-extension/src/index.ts:644
 msgid "Show Keyboard Shortcuts"
 msgstr "Показать горячие клавиши"
 
-#: packages/apputils-extension/src/index.ts:645
+#: packages/apputils-extension/src/index.ts:645 packages/apputils-extension/src/index.ts:654
 msgid "Show relevant keyboard shortcuts for the current active widget"
 msgstr "Показать соответствующие сочетания клавиш для текущего активного виджета"
 
-#: packages/apputils-extension/src/index.ts:662 packages/help-extension/src/index.tsx:183 packages/help-extension/src/index.tsx:296 packages/help-extension/src/index.tsx:500 packages/help-extension/src/index.tsx:90
+#: packages/apputils-extension/src/index.ts:653
+msgid "Show Keyboard Shortcuts…"
+msgstr ""
+
+#: packages/apputils-extension/src/index.ts:662 packages/apputils-extension/src/index.ts:671 packages/help-extension/src/index.tsx:183 packages/help-extension/src/index.tsx:296 packages/help-extension/src/index.tsx:500 packages/help-extension/src/index.tsx:90
 msgid "Help"
 msgstr "Справка"
 
 #: packages/apputils-extension/src/notificationplugin.tsx:167 packages/apputils-extension/src/notificationplugin.tsx:354
 msgid "%1 notification"
 msgid_plural "%1 notifications"
 msgstr[0] "%1 уведомление"
@@ -2829,15 +2895,15 @@
 msgid "Command Palette"
 msgstr "Палитра команд"
 
 #: packages/apputils-extension/src/shortcuts.tsx:193
 msgid "Keyboard Shortcuts"
 msgstr "Горячие клавиши"
 
-#: packages/apputils-extension/src/shortcuts.tsx:197 packages/docmanager/src/widgetmanager.ts:397 packages/filebrowser/src/listing.ts:1415 packages/running-extension/src/opentabs.ts:86
+#: packages/apputils-extension/src/shortcuts.tsx:197 packages/docmanager/src/widgetmanager.ts:397 packages/docmanager/src/widgetmanager.ts:468 packages/filebrowser/src/listing.ts:1415 packages/filebrowser/src/listing.ts:1436 packages/filebrowser/src/listing.ts:1488 packages/running-extension/src/opentabs.ts:86
 msgid "Close"
 msgstr "Закрыть"
 
 #: packages/apputils-extension/src/themesplugins.ts:118
 msgid "Switch to the provided `theme`."
 msgstr "Переключиться на предоставленную `theme`."
 
@@ -2885,15 +2951,15 @@
 msgid "Increase Content Font Size"
 msgstr "Увеличить размер шрифта содержимого"
 
 #: packages/apputils-extension/src/themesplugins.ts:217
 msgid "Increase UI Font Size"
 msgstr "Увеличить размер шрифта интерфейса"
 
-#: packages/apputils-extension/src/themesplugins.ts:219 packages/fileeditor-extension/src/commands.ts:281
+#: packages/apputils-extension/src/themesplugins.ts:219 packages/fileeditor-extension/src/commands.ts:281 packages/fileeditor-extension/src/commands.ts:282
 msgid "Increase Font Size"
 msgstr "Увеличить размер шрифта"
 
 #: packages/apputils-extension/src/themesplugins.ts:229
 msgid "Decrease Code Font Size"
 msgstr "Уменьшить размер шрифта кода"
 
@@ -2901,51 +2967,55 @@
 msgid "Decrease Content Font Size"
 msgstr "Уменьшить размер шрифта содержимого"
 
 #: packages/apputils-extension/src/themesplugins.ts:233
 msgid "Decrease UI Font Size"
 msgstr "Уменьшить размер шрифта интерфейса"
 
-#: packages/apputils-extension/src/themesplugins.ts:235 packages/fileeditor-extension/src/commands.ts:285
+#: packages/apputils-extension/src/themesplugins.ts:235 packages/fileeditor-extension/src/commands.ts:285 packages/fileeditor-extension/src/commands.ts:286
 msgid "Decrease Font Size"
 msgstr "Уменьшить размер шрифта"
 
-#: packages/apputils-extension/src/themesplugins.ts:295 packages/codemirror/src/extension.ts:982
+#: packages/apputils-extension/src/themesplugins.ts:295 packages/codemirror/src/extension.ts:1006 packages/codemirror/src/extension.ts:982
 msgid "Theme"
 msgstr "Тема"
 
-#: packages/apputils-extension/src/workspacesplugin.ts:181
+#: packages/apputils-extension/src/workspacesplugin.ts:181 packages/apputils-extension/src/workspacesplugin.ts:95
 msgid "Workspace loader"
 msgstr "Загрузчик рабочей области"
 
-#: packages/apputils-extension/src/workspacesplugin.ts:271 packages/apputils-extension/src/workspacesplugin.ts:279 packages/docmanager/src/widgetmanager.ts:442 packages/docregistry/src/context.ts:1043
+#: packages/apputils-extension/src/workspacesplugin.ts:271 packages/apputils-extension/src/workspacesplugin.ts:279 packages/docmanager/src/widgetmanager.ts:442 packages/docmanager/src/widgetmanager.ts:513 packages/docregistry/src/context.ts:1041 packages/docregistry/src/context.ts:1043 packages/workspaces-extension/src/commands.ts:587
 msgid "Save"
 msgstr "Сохранить"
 
-#: packages/apputils-extension/src/workspacesplugin.ts:272 packages/apputils-extension/src/workspacesplugin.ts:93
+#: packages/apputils-extension/src/workspacesplugin.ts:272 packages/apputils-extension/src/workspacesplugin.ts:93 packages/workspaces-extension/src/commands.ts:458
 msgid "Save Current Workspace"
 msgstr "Сохранить текущую рабочую область"
 
-#: packages/apputils-extension/src/workspacesplugin.ts:275 packages/apputils-extension/src/workspacesplugin.ts:79
+#: packages/apputils-extension/src/workspacesplugin.ts:275 packages/apputils-extension/src/workspacesplugin.ts:79 packages/workspaces-extension/src/commands.ts:449 packages/workspaces-extension/src/commands.ts:584
 msgid "Save Current Workspace As…"
 msgstr "Сохранить текущую рабочую область как…"
 
 #: packages/apputils-extension/src/workspacesplugin.ts:72
+msgid "JupyterLab Workspace File"
+msgstr ""
+
+#: packages/apputils-extension/src/workspacesplugin.ts:72
 msgid "JupyterLab workspace File"
 msgstr "Файл рабочей области JupyterLab"
 
-#: packages/apputils/src/dialog.tsx:47 packages/help-extension/src/index.tsx:153 packages/help-extension/src/index.tsx:425 packages/hub-extension/src/index.ts:180 packages/lsp/src/adapters/adapter.ts:497 packages/mainmenu-extension/src/index.ts:548
+#: packages/apputils/src/dialog.tsx:47 packages/help-extension/src/index.tsx:153 packages/help-extension/src/index.tsx:425 packages/hub-extension/src/index.ts:180 packages/lsp/src/adapters/adapter.ts:497 packages/mainmenu-extension/src/index.ts:545 packages/mainmenu-extension/src/index.ts:548
 msgid "Dismiss"
 msgstr "Отклонить"
 
-#: packages/apputils/src/dialog.tsx:770 packages/apputils/src/dialog.tsx:870 packages/apputils/src/sessioncontext.tsx:1335 packages/debugger-extension/src/index.ts:739 packages/debugger-extension/src/index.ts:840 packages/filebrowser/src/listing.ts:433 packages/filebrowser/src/model.ts:449 packages/notebook/src/searchprovider.ts:527 packages/settingeditor/src/plugineditor.ts:132 packages/shortcuts-extension/src/components/ShortcutItem.tsx:224 packages/translation-extension/src/index.ts:156
+#: packages/apputils/src/dialog.tsx:770 packages/apputils/src/dialog.tsx:793 packages/apputils/src/dialog.tsx:870 packages/apputils/src/dialog.tsx:893 packages/apputils/src/sessioncontext.tsx:1335 packages/debugger-extension/src/index.ts:739 packages/debugger-extension/src/index.ts:840 packages/filebrowser/src/listing.ts:433 packages/filebrowser/src/listing.ts:436 packages/filebrowser/src/model.ts:442 packages/filebrowser/src/model.ts:449 packages/notebook/src/searchprovider.ts:516 packages/notebook/src/searchprovider.ts:519 packages/notebook/src/searchprovider.ts:527 packages/settingeditor/src/plugineditor.ts:132 packages/shortcuts-extension/src/components/ShortcutItem.tsx:224 packages/shortcuts-extension/src/components/ShortcutItem.tsx:341 packages/translation-extension/src/index.ts:156
 msgid "Cancel"
 msgstr "Отмена"
 
-#: packages/apputils/src/dialog.tsx:770 packages/extensionmanager/src/dialog.tsx:37 packages/extensionmanager/src/model.ts:533 packages/extensionmanager/src/model.ts:556 packages/notebook/src/model.ts:377 packages/notebook/src/panel.ts:228 packages/notebook/src/searchprovider.ts:528 packages/settingeditor/src/plugineditor.ts:133
+#: packages/apputils/src/dialog.tsx:770 packages/apputils/src/dialog.tsx:793 packages/extensionmanager/src/dialog.tsx:37 packages/extensionmanager/src/model.ts:533 packages/extensionmanager/src/model.ts:556 packages/notebook/src/model.ts:377 packages/notebook/src/panel.ts:228 packages/notebook/src/searchprovider.ts:517 packages/notebook/src/searchprovider.ts:520 packages/notebook/src/searchprovider.ts:528 packages/settingeditor/src/plugineditor.ts:133
 msgid "Ok"
 msgstr "Ок"
 
 #: packages/apputils/src/kernelstatuses.tsx:221 packages/apputils/src/sessioncontext.tsx:1757 packages/apputils/src/sessioncontext.tsx:631
 msgid "No Kernel"
 msgstr "Нет Ядра"
 
@@ -3013,15 +3083,15 @@
 msgid "%1 Terminals, %2 Kernel sessions"
 msgstr "%1 терминалов, %2 сессий ядра"
 
 #: packages/apputils/src/sessioncontext.tsx:1051
 msgid "Error Starting Kernel"
 msgstr "Ошибка запуска ядра"
 
-#: packages/apputils/src/sessioncontext.tsx:1344 packages/filebrowser/src/opendialog.ts:95
+#: packages/apputils/src/sessioncontext.tsx:1344 packages/filebrowser/src/opendialog.ts:106 packages/filebrowser/src/opendialog.ts:95
 msgid "Select"
 msgstr "Выбрать"
 
 #: packages/apputils/src/sessioncontext.tsx:1345 packages/apputils/src/sessioncontext.tsx:1353
 msgid "Select Kernel"
 msgstr "Выбрать Ядро"
 
@@ -3113,47 +3183,47 @@
 msgid "Switch kernel"
 msgstr "Переключить ядро"
 
 #: packages/apputils/src/toolbar/widget.tsx:210
 msgid "Kernel %1"
 msgstr "Ядро %1"
 
-#: packages/apputils/src/toolbar/widget.tsx:56 packages/mainmenu-extension/src/index.ts:469 packages/notebook-extension/src/index.ts:2529
+#: packages/apputils/src/toolbar/widget.tsx:56 packages/mainmenu-extension/src/index.ts:467 packages/mainmenu-extension/src/index.ts:469 packages/notebook-extension/src/index.ts:2529 packages/notebook-extension/src/index.ts:2536 packages/notebook-extension/src/index.ts:2547
 msgid "Interrupt the kernel"
 msgstr "Прервать работу ядра"
 
-#: packages/apputils/src/toolbar/widget.tsx:80 packages/mainmenu-extension/src/index.ts:494 packages/notebook-extension/src/index.ts:2377
+#: packages/apputils/src/toolbar/widget.tsx:80 packages/mainmenu-extension/src/index.ts:492 packages/mainmenu-extension/src/index.ts:494 packages/notebook-extension/src/index.ts:2377 packages/notebook-extension/src/index.ts:2384 packages/notebook-extension/src/index.ts:2395
 msgid "Restart the kernel"
 msgstr "Перезапустить ядро"
 
 #: packages/cells/src/placeholder.ts:85
 msgid "Click to expand"
 msgstr "Нажмите, чтобы раскрыть"
 
-#: packages/cells/src/widget.ts:1010 packages/cells/src/widget.ts:1099 packages/cells/src/widget.ts:1506
+#: packages/cells/src/widget.ts:1010 packages/cells/src/widget.ts:1012 packages/cells/src/widget.ts:1075 packages/cells/src/widget.ts:1099 packages/cells/src/widget.ts:1101 packages/cells/src/widget.ts:1225 packages/cells/src/widget.ts:1506 packages/cells/src/widget.ts:1508 packages/cells/src/widget.ts:1509 packages/cells/src/widget.ts:1646
 msgid "Code Cell Content"
 msgstr "Содержимое ячейки кода"
 
-#: packages/cells/src/widget.ts:1011 packages/cells/src/widget.ts:1100 packages/cells/src/widget.ts:1507
+#: packages/cells/src/widget.ts:1011 packages/cells/src/widget.ts:1013 packages/cells/src/widget.ts:1076 packages/cells/src/widget.ts:1100 packages/cells/src/widget.ts:1102 packages/cells/src/widget.ts:1226 packages/cells/src/widget.ts:1507 packages/cells/src/widget.ts:1509 packages/cells/src/widget.ts:1510 packages/cells/src/widget.ts:1647
 msgid "Code Cell Content with Output"
 msgstr "Содержимое ячейки с выводом"
 
-#: packages/cells/src/widget.ts:1931
+#: packages/cells/src/widget.ts:1931 packages/cells/src/widget.ts:1933 packages/cells/src/widget.ts:1935 packages/cells/src/widget.ts:1936 packages/cells/src/widget.ts:2076
 msgid "Markdown Cell Content"
 msgstr "Markdown контент ячейки"
 
-#: packages/cells/src/widget.ts:2174
+#: packages/cells/src/widget.ts:2174 packages/cells/src/widget.ts:2176 packages/cells/src/widget.ts:2178 packages/cells/src/widget.ts:2179 packages/cells/src/widget.ts:2319
 msgid "%1 cell hidden"
 msgid_plural "%1 cells hidden"
 msgstr[0] "%1 ячейка скрыта"
 msgstr[1] "%1 ячейки скрыты"
 msgstr[2] "%1 ячеек скрыто"
 msgstr[3] "%1 ячеек скрыто"
 
-#: packages/cells/src/widget.ts:2397
+#: packages/cells/src/widget.ts:2397 packages/cells/src/widget.ts:2399 packages/cells/src/widget.ts:2401 packages/cells/src/widget.ts:2402 packages/cells/src/widget.ts:2542
 msgid "Raw Cell Content"
 msgstr "Сырое содержание ячейки"
 
 #: packages/celltags-extension/src/celltag.tsx:211
 msgid "Add Tag"
 msgstr "Добавить тег"
 
@@ -3177,775 +3247,795 @@
 msgid "Ln %1, Col %2"
 msgstr "Строка %1, столбец %2"
 
 #: packages/codeeditor/src/lineCol.tsx:253
 msgid "Go to line number…"
 msgstr "Перейти к номеру строки…"
 
-#: packages/codemirror/src/extension.ts:1000
+#: packages/codemirror-extension/src/commands.ts:107
+msgid "Select Next Occurrence"
+msgstr ""
+
+#: packages/codemirror-extension/src/commands.ts:68
+msgid "Delete the current line"
+msgstr ""
+
+#: packages/codemirror-extension/src/commands.ts:80
+msgid "Toggle Block Comment"
+msgstr ""
+
+#: packages/codemirror-extension/src/commands.ts:81
+msgid "Toggles block commends in languages which support it (e.g. C, JavaScript)"
+msgstr ""
+
+#: packages/codemirror-extension/src/commands.ts:95
+msgid "Toggle Comment"
+msgstr ""
+
+#: packages/codemirror/src/extension.ts:1000 packages/codemirror/src/extension.ts:1024
 msgid "Folded lines"
 msgstr "Свернутые строки"
 
-#: packages/codemirror/src/extension.ts:1001
+#: packages/codemirror/src/extension.ts:1001 packages/codemirror/src/extension.ts:1025
 msgid "Unfolded lines"
 msgstr "Развернутые строки"
 
-#: packages/codemirror/src/extension.ts:1002
+#: packages/codemirror/src/extension.ts:1002 packages/codemirror/src/extension.ts:1026
 msgid "to"
 msgstr "к"
 
-#: packages/codemirror/src/extension.ts:1003
+#: packages/codemirror/src/extension.ts:1003 packages/codemirror/src/extension.ts:1027
 msgid "folded code"
 msgstr "свёрнутый код"
 
-#: packages/codemirror/src/extension.ts:1004
+#: packages/codemirror/src/extension.ts:1004 packages/codemirror/src/extension.ts:1028
 msgid "unfold"
 msgstr "развернуть"
 
-#: packages/codemirror/src/extension.ts:1005
+#: packages/codemirror/src/extension.ts:1005 packages/codemirror/src/extension.ts:1029
 msgid "Fold line"
 msgstr "Свернуть строку"
 
-#: packages/codemirror/src/extension.ts:1006
+#: packages/codemirror/src/extension.ts:1006 packages/codemirror/src/extension.ts:1030
 msgid "Unfold line"
 msgstr "Развернуть строку"
 
-#: packages/codemirror/src/extension.ts:1008
+#: packages/codemirror/src/extension.ts:1007 packages/codemirror/src/extension.ts:983
+msgid "CodeMirror theme"
+msgstr "CodeMirror тема"
+
+#: packages/codemirror/src/extension.ts:1008 packages/codemirror/src/extension.ts:1032
 msgid "Go to line"
 msgstr "Перейти к строке"
 
-#: packages/codemirror/src/extension.ts:1009
+#: packages/codemirror/src/extension.ts:1009 packages/codemirror/src/extension.ts:1033
 msgid "go"
 msgstr "вперед"
 
-#: packages/codemirror/src/extension.ts:1010 packages/documentsearch/src/searchview.tsx:173 packages/documentsearch/src/searchview.tsx:178
+#: packages/codemirror/src/extension.ts:1010 packages/codemirror/src/extension.ts:1034 packages/documentsearch/src/searchview.tsx:173 packages/documentsearch/src/searchview.tsx:178
 msgid "Find"
 msgstr "Найти"
 
-#: packages/codemirror/src/extension.ts:1011 packages/documentsearch/src/searchview.tsx:236 packages/documentsearch/src/searchview.tsx:240 packages/documentsearch/src/searchview.tsx:267
+#: packages/codemirror/src/extension.ts:1011 packages/codemirror/src/extension.ts:1035 packages/documentsearch/src/searchview.tsx:236 packages/documentsearch/src/searchview.tsx:240 packages/documentsearch/src/searchview.tsx:267
 msgid "Replace"
 msgstr "Заменить"
 
-#: packages/codemirror/src/extension.ts:1012
+#: packages/codemirror/src/extension.ts:1012 packages/codemirror/src/extension.ts:1036
 msgid "next"
 msgstr "следующий"
 
-#: packages/codemirror/src/extension.ts:1013
+#: packages/codemirror/src/extension.ts:1013 packages/codemirror/src/extension.ts:1037
 msgid "previous"
 msgstr "назад"
 
-#: packages/codemirror/src/extension.ts:1014
+#: packages/codemirror/src/extension.ts:1014 packages/codemirror/src/extension.ts:1038
 msgid "all"
 msgstr "все"
 
-#: packages/codemirror/src/extension.ts:1015
+#: packages/codemirror/src/extension.ts:1015 packages/codemirror/src/extension.ts:1039
 msgid "match case"
 msgstr "учитывать регистр"
 
-#: packages/codemirror/src/extension.ts:1016
+#: packages/codemirror/src/extension.ts:1016 packages/codemirror/src/extension.ts:1040
 msgid "replace"
 msgstr "заменить"
 
-#: packages/codemirror/src/extension.ts:1017
+#: packages/codemirror/src/extension.ts:1017 packages/codemirror/src/extension.ts:1041
 msgid "replace all"
 msgstr "заменить всё"
 
-#: packages/codemirror/src/extension.ts:1018
+#: packages/codemirror/src/extension.ts:1018 packages/codemirror/src/extension.ts:1042
 msgid "close"
 msgstr "закрыть"
 
-#: packages/codemirror/src/extension.ts:1019
+#: packages/codemirror/src/extension.ts:1019 packages/codemirror/src/extension.ts:1043
 msgid "current match"
 msgstr "текущее совпадение"
 
-#: packages/codemirror/src/extension.ts:1020
+#: packages/codemirror/src/extension.ts:1020 packages/codemirror/src/extension.ts:1044
 msgid "replaced $ matches"
 msgstr "заменено $ совпадений"
 
-#: packages/codemirror/src/extension.ts:1021
+#: packages/codemirror/src/extension.ts:1020 packages/codemirror/src/extension.ts:996
+msgid "Control character"
+msgstr "Контрольный символ"
+
+#: packages/codemirror/src/extension.ts:1021 packages/codemirror/src/extension.ts:1045
 msgid "replaced match on line $"
 msgstr "заменил совпадение на строке $"
 
-#: packages/codemirror/src/extension.ts:1022
+#: packages/codemirror/src/extension.ts:1022 packages/codemirror/src/extension.ts:1046
 msgid "on line"
 msgstr "в строке"
 
-#: packages/codemirror/src/extension.ts:1024
+#: packages/codemirror/src/extension.ts:1022 packages/codemirror/src/extension.ts:998
+msgid "Selection deleted"
+msgstr "Выделение удалено"
+
+#: packages/codemirror/src/extension.ts:1024 packages/codemirror/src/extension.ts:1048
 msgid "Completions"
 msgstr "Завершения"
 
-#: packages/codemirror/src/extension.ts:1026
+#: packages/codemirror/src/extension.ts:1026 packages/codemirror/src/extension.ts:1050
 msgid "Diagnostics"
 msgstr "Диагностика"
 
-#: packages/codemirror/src/extension.ts:1027
+#: packages/codemirror/src/extension.ts:1027 packages/codemirror/src/extension.ts:1051
 msgid "No diagnostics"
 msgstr "Нет диагностики"
 
-#: packages/codemirror/src/extension.ts:619
+#: packages/codemirror/src/extension.ts:618 packages/codemirror/src/extension.ts:619
 msgid "Auto Closing Brackets"
 msgstr "Автоматически закрывать скобки"
 
-#: packages/codemirror/src/extension.ts:628
+#: packages/codemirror/src/extension.ts:627 packages/codemirror/src/extension.ts:628
 msgid "Code Folding"
 msgstr "Свёртывание кода"
 
-#: packages/codemirror/src/extension.ts:640
+#: packages/codemirror/src/extension.ts:639 packages/codemirror/src/extension.ts:640
 msgid "Cursor blinking rate"
 msgstr "Частота мигания курсора"
 
-#: packages/codemirror/src/extension.ts:641
+#: packages/codemirror/src/extension.ts:640 packages/codemirror/src/extension.ts:641
 msgid "Half-period in milliseconds used for cursor blinking. The default blink rate is 1200ms. By setting this to zero, blinking can be disabled."
 msgstr "Полупериод в миллисекундах, используемый для мигания курсора. Частота мерцания по умолчанию составляет 1200 мс. Установив это значение на ноль, мигание можно отключить."
 
-#: packages/codemirror/src/extension.ts:652
+#: packages/codemirror/src/extension.ts:651 packages/codemirror/src/extension.ts:652
 msgid "Highlight the active line"
 msgstr "Выделите активную строку"
 
-#: packages/codemirror/src/extension.ts:661
+#: packages/codemirror/src/extension.ts:660 packages/codemirror/src/extension.ts:661
 msgid "Highlight special characters"
 msgstr ""
 
-#: packages/codemirror/src/extension.ts:671
+#: packages/codemirror/src/extension.ts:670 packages/codemirror/src/extension.ts:671
 msgid "Highlight trailing white spaces"
 msgstr "Выделять конечные пробелы"
 
-#: packages/codemirror/src/extension.ts:680
+#: packages/codemirror/src/extension.ts:679 packages/codemirror/src/extension.ts:680
 msgid "Highlight white spaces"
 msgstr "Выделить белые пробелы"
 
-#: packages/codemirror/src/extension.ts:694
+#: packages/codemirror/src/extension.ts:693 packages/codemirror/src/extension.ts:694
 msgid "Indentation unit"
 msgstr "Единица отступа"
 
-#: packages/codemirror/src/extension.ts:695
+#: packages/codemirror/src/extension.ts:694 packages/codemirror/src/extension.ts:695
 msgid "The indentation is a `Tab` or the number of spaces. This defaults to 4 spaces."
 msgstr "Отступ `Tab` представляет собой количество пробелов. По умолчанию это 4 пробела."
 
-#: packages/codemirror/src/extension.ts:730
+#: packages/codemirror/src/extension.ts:730 packages/codemirror/src/extension.ts:755
 msgid "Line Numbers"
 msgstr "Номера строк"
 
-#: packages/codemirror/src/extension.ts:739
+#: packages/codemirror/src/extension.ts:739 packages/codemirror/src/extension.ts:764
 msgid "Line Wrap"
 msgstr "Перенос строк"
 
-#: packages/codemirror/src/extension.ts:753 packages/fileeditor-extension/src/commands.ts:422 packages/fileeditor-extension/src/commands.ts:429 packages/mainmenu-extension/src/index.ts:588
+#: packages/codemirror/src/extension.ts:753 packages/codemirror/src/extension.ts:778 packages/fileeditor-extension/src/commands.ts:422 packages/fileeditor-extension/src/commands.ts:423 packages/fileeditor-extension/src/commands.ts:429 packages/fileeditor-extension/src/commands.ts:430 packages/mainmenu-extension/src/index.ts:584 packages/mainmenu-extension/src/index.ts:588
 msgid "Match Brackets"
 msgstr "Совпадения скобок"
 
-#: packages/codemirror/src/extension.ts:766
+#: packages/codemirror/src/extension.ts:766 packages/codemirror/src/extension.ts:791
 msgid "Rectangular selection"
 msgstr "Прямоугольное выделение"
 
-#: packages/codemirror/src/extension.ts:767
+#: packages/codemirror/src/extension.ts:767 packages/codemirror/src/extension.ts:792
 msgid "Rectangular (block) selection can be created by dragging the mouse pointer while holding the left mouse button and the Alt key. When the Alt key is pressed, a crosshair cursor will appear, indicating that the rectangular selection mode is active."
 msgstr "Прямоугольное (блочное) выделение можно создать, перетаскивая указатель мыши, удерживая левую кнопку мыши и клавишу Alt. При нажатии клавиши Alt появится курсор в виде перекрестия, указывающий на то, что режим прямоугольного выделения активен."
 
-#: packages/codemirror/src/extension.ts:792
+#: packages/codemirror/src/extension.ts:792 packages/codemirror/src/extension.ts:817
 msgid "Rulers"
 msgstr "Линейки"
 
-#: packages/codemirror/src/extension.ts:860
+#: packages/codemirror/src/extension.ts:860 packages/codemirror/src/extension.ts:884
 msgid "Smart Indentation"
 msgstr "Умные отступы"
 
-#: packages/codemirror/src/extension.ts:908
+#: packages/codemirror/src/extension.ts:908 packages/codemirror/src/extension.ts:932
 msgid "Tab size"
 msgstr "Размер вкладки"
 
-#: packages/codemirror/src/extension.ts:933
+#: packages/codemirror/src/extension.ts:933 packages/codemirror/src/extension.ts:957
 msgid "Multiple selections"
 msgstr "Множественный выбор"
 
-#: packages/codemirror/src/extension.ts:948
+#: packages/codemirror/src/extension.ts:948 packages/codemirror/src/extension.ts:972
 msgid "Custom editor styles"
 msgstr "Пользовательские стили редактора"
 
-#: packages/codemirror/src/extension.ts:953
+#: packages/codemirror/src/extension.ts:953 packages/codemirror/src/extension.ts:977
 msgid "Font Family"
 msgstr "Семейство шрифта"
 
-#: packages/codemirror/src/extension.ts:959
+#: packages/codemirror/src/extension.ts:959 packages/codemirror/src/extension.ts:983
 msgid "Font Size"
 msgstr "Размер шрифта"
 
-#: packages/codemirror/src/extension.ts:963
+#: packages/codemirror/src/extension.ts:963 packages/codemirror/src/extension.ts:987
 msgid "Line Height"
 msgstr "Высота строки"
 
-#: packages/codemirror/src/extension.ts:983
-msgid "CodeMirror theme"
-msgstr "CodeMirror тема"
-
-#: packages/codemirror/src/extension.ts:996
-msgid "Control character"
-msgstr "Контрольный символ"
-
-#: packages/codemirror/src/extension.ts:998
-msgid "Selection deleted"
-msgstr "Выделение удалено"
+#: packages/codemirror/src/language.ts:1003 packages/codemirror/src/language.ts:996
+msgid "IDL"
+msgstr "IDL"
 
-#: packages/codemirror/src/language.ts:1006
+#: packages/codemirror/src/language.ts:1006 packages/codemirror/src/language.ts:1013
 msgid "JSON-LD"
 msgstr "JSON-LD"
 
-#: packages/codemirror/src/language.ts:1017
+#: packages/codemirror/src/language.ts:1017 packages/codemirror/src/language.ts:1024
 msgid "Jinja2"
 msgstr "Jinja2"
 
-#: packages/codemirror/src/language.ts:1027
+#: packages/codemirror/src/language.ts:1027 packages/codemirror/src/language.ts:1034
 msgid "Julia"
 msgstr "Julia"
 
-#: packages/codemirror/src/language.ts:1037
+#: packages/codemirror/src/language.ts:1037 packages/codemirror/src/language.ts:1044
 msgid "Kotlin"
 msgstr "Kotlin"
 
-#: packages/codemirror/src/language.ts:1047
+#: packages/codemirror/src/language.ts:1047 packages/codemirror/src/language.ts:1054
 msgid "LESS"
 msgstr "LESS"
 
-#: packages/codemirror/src/language.ts:1057
+#: packages/codemirror/src/language.ts:1057 packages/codemirror/src/language.ts:1064
 msgid "LiveScript"
 msgstr "LiveScript"
 
-#: packages/codemirror/src/language.ts:1068
+#: packages/codemirror/src/language.ts:1068 packages/codemirror/src/language.ts:1075
 msgid "Lua"
 msgstr "Lua"
 
-#: packages/codemirror/src/language.ts:1078
+#: packages/codemirror/src/language.ts:1078 packages/codemirror/src/language.ts:1085
 msgid "mIRC"
 msgstr "mIRC"
 
-#: packages/codemirror/src/language.ts:1087
+#: packages/codemirror/src/language.ts:1087 packages/codemirror/src/language.ts:1094
 msgid "Mathematica"
 msgstr "Mathematica"
 
-#: packages/codemirror/src/language.ts:1097
+#: packages/codemirror/src/language.ts:1097 packages/codemirror/src/language.ts:1104
 msgid "Modelica"
 msgstr "Modelica"
 
-#: packages/codemirror/src/language.ts:1107
+#: packages/codemirror/src/language.ts:1107 packages/codemirror/src/language.ts:1114
 msgid "MUMPS"
 msgstr "MUMPS"
 
-#: packages/codemirror/src/language.ts:1117
+#: packages/codemirror/src/language.ts:1117 packages/codemirror/src/language.ts:1124
 msgid "mbox"
 msgstr "mbox"
 
-#: packages/codemirror/src/language.ts:1127
+#: packages/codemirror/src/language.ts:1127 packages/codemirror/src/language.ts:1134
 msgid "Nginx"
 msgstr "Nginx"
 
-#: packages/codemirror/src/language.ts:1137
+#: packages/codemirror/src/language.ts:1137 packages/codemirror/src/language.ts:1144
 msgid "NSIS"
 msgstr "NSIS"
 
-#: packages/codemirror/src/language.ts:1147
+#: packages/codemirror/src/language.ts:1147 packages/codemirror/src/language.ts:1154
 msgid "NTriples"
 msgstr "NTriples"
 
-#: packages/codemirror/src/language.ts:1161
+#: packages/codemirror/src/language.ts:1161 packages/codemirror/src/language.ts:1168
 msgid "Objective-C"
 msgstr "Objective-C"
 
-#: packages/codemirror/src/language.ts:1172
+#: packages/codemirror/src/language.ts:1172 packages/codemirror/src/language.ts:1179
 msgid "Objective-C++"
 msgstr "Objective-C++"
 
-#: packages/codemirror/src/language.ts:1183
+#: packages/codemirror/src/language.ts:1183 packages/codemirror/src/language.ts:1190
 msgid "OCaml"
 msgstr "OCaml"
 
-#: packages/codemirror/src/language.ts:1193
+#: packages/codemirror/src/language.ts:1193 packages/codemirror/src/language.ts:1200
 msgid "Octave"
 msgstr "Octave"
 
-#: packages/codemirror/src/language.ts:1203
+#: packages/codemirror/src/language.ts:1203 packages/codemirror/src/language.ts:1210
 msgid "Oz"
 msgstr "Oz"
 
-#: packages/codemirror/src/language.ts:1213
+#: packages/codemirror/src/language.ts:1213 packages/codemirror/src/language.ts:1220
 msgid "Pascal"
 msgstr "Pascal"
 
-#: packages/codemirror/src/language.ts:1223
+#: packages/codemirror/src/language.ts:1223 packages/codemirror/src/language.ts:1230
 msgid "Perl"
 msgstr "Perl"
 
-#: packages/codemirror/src/language.ts:1233
+#: packages/codemirror/src/language.ts:1233 packages/codemirror/src/language.ts:1240
 msgid "Pig"
 msgstr "Pig"
 
-#: packages/codemirror/src/language.ts:1243
+#: packages/codemirror/src/language.ts:1243 packages/codemirror/src/language.ts:1250
 msgid "PowerShell"
 msgstr "PowerShell"
 
-#: packages/codemirror/src/language.ts:1253
+#: packages/codemirror/src/language.ts:1253 packages/codemirror/src/language.ts:1260
 msgid "Properties files"
 msgstr "Свойства файлов"
 
-#: packages/codemirror/src/language.ts:1264
+#: packages/codemirror/src/language.ts:1264 packages/codemirror/src/language.ts:1271
 msgid "ProtoBuf"
 msgstr "ProtoBuf"
 
-#: packages/codemirror/src/language.ts:1274
+#: packages/codemirror/src/language.ts:1274 packages/codemirror/src/language.ts:1281
 msgid "Puppet"
 msgstr "Puppet"
 
-#: packages/codemirror/src/language.ts:1284
+#: packages/codemirror/src/language.ts:1284 packages/codemirror/src/language.ts:1291
 msgid "Q"
 msgstr "Q"
 
-#: packages/codemirror/src/language.ts:1294
+#: packages/codemirror/src/language.ts:1294 packages/codemirror/src/language.ts:1301
 msgid "R"
 msgstr "R"
 
-#: packages/codemirror/src/language.ts:1305
+#: packages/codemirror/src/language.ts:1305 packages/codemirror/src/language.ts:1312
 msgid "RPM Changes"
 msgstr "Изменения RPM"
 
-#: packages/codemirror/src/language.ts:1314
+#: packages/codemirror/src/language.ts:1314 packages/codemirror/src/language.ts:1321
 msgid "RPM Spec"
 msgstr "Спецификация RPM"
 
-#: packages/codemirror/src/language.ts:1324
+#: packages/codemirror/src/language.ts:1324 packages/codemirror/src/language.ts:1331
 msgid "Ruby"
 msgstr "Ruby"
 
-#: packages/codemirror/src/language.ts:1335
+#: packages/codemirror/src/language.ts:1335 packages/codemirror/src/language.ts:1342
 msgid "SAS"
 msgstr "SAS"
 
-#: packages/codemirror/src/language.ts:1345
+#: packages/codemirror/src/language.ts:1345 packages/codemirror/src/language.ts:1352
 msgid "Scala"
 msgstr "Scala"
 
-#: packages/codemirror/src/language.ts:1355
+#: packages/codemirror/src/language.ts:1355 packages/codemirror/src/language.ts:1362
 msgid "Scheme"
 msgstr "Схема"
 
-#: packages/codemirror/src/language.ts:1365
+#: packages/codemirror/src/language.ts:1365 packages/codemirror/src/language.ts:1372
 msgid "SCSS"
 msgstr "SCSS"
 
-#: packages/codemirror/src/language.ts:1375
+#: packages/codemirror/src/language.ts:1375 packages/codemirror/src/language.ts:1382
 msgid "Shell"
 msgstr "Оболочка"
 
-#: packages/codemirror/src/language.ts:1387
+#: packages/codemirror/src/language.ts:1387 packages/codemirror/src/language.ts:1394
 msgid "Sieve"
 msgstr "Sieve"
 
-#: packages/codemirror/src/language.ts:1397
+#: packages/codemirror/src/language.ts:1397 packages/codemirror/src/language.ts:1404
 msgid "Smalltalk"
 msgstr "Smalltalk"
 
-#: packages/codemirror/src/language.ts:1407
+#: packages/codemirror/src/language.ts:1407 packages/codemirror/src/language.ts:1414
 msgid "Solr"
 msgstr "Solr"
 
-#: packages/codemirror/src/language.ts:1416
+#: packages/codemirror/src/language.ts:1416 packages/codemirror/src/language.ts:1423
 msgid "SML"
 msgstr "SML"
 
-#: packages/codemirror/src/language.ts:1426
+#: packages/codemirror/src/language.ts:1426 packages/codemirror/src/language.ts:1433
 msgid "SPARQL"
 msgstr "SPARQL"
 
-#: packages/codemirror/src/language.ts:1437
+#: packages/codemirror/src/language.ts:1437 packages/codemirror/src/language.ts:1444
 msgid "Spreadsheet"
 msgstr "Spreadsheet"
 
-#: packages/codemirror/src/language.ts:1447
+#: packages/codemirror/src/language.ts:1447 packages/codemirror/src/language.ts:1454
 msgid "Squirrel"
 msgstr "Squirrel"
 
-#: packages/codemirror/src/language.ts:1457
+#: packages/codemirror/src/language.ts:1457 packages/codemirror/src/language.ts:1464
 msgid "Stylus"
 msgstr "Stylus"
 
-#: packages/codemirror/src/language.ts:1467
+#: packages/codemirror/src/language.ts:1467 packages/codemirror/src/language.ts:1474
 msgid "Swift"
 msgstr "Swift"
 
-#: packages/codemirror/src/language.ts:1477
+#: packages/codemirror/src/language.ts:1477 packages/codemirror/src/language.ts:1484
 msgid "sTeX"
 msgstr "sTeX"
 
-#: packages/codemirror/src/language.ts:1486 packages/notebook-extension/src/index.ts:3800
+#: packages/codemirror/src/language.ts:1486 packages/codemirror/src/language.ts:1493 packages/notebook-extension/src/index.ts:3800 packages/notebook-extension/src/index.ts:3807 packages/notebook-extension/src/index.ts:3866
 msgid "LaTeX"
 msgstr "LaTeX"
 
-#: packages/codemirror/src/language.ts:1497
+#: packages/codemirror/src/language.ts:1497 packages/codemirror/src/language.ts:1504
 msgid "SystemVerilog"
 msgstr "SystemVerilog"
 
-#: packages/codemirror/src/language.ts:1507
+#: packages/codemirror/src/language.ts:1507 packages/codemirror/src/language.ts:1514
 msgid "Tcl"
 msgstr "Tcl"
 
-#: packages/codemirror/src/language.ts:1517
+#: packages/codemirror/src/language.ts:1517 packages/codemirror/src/language.ts:1524
 msgid "Textile"
 msgstr "Textile"
 
-#: packages/codemirror/src/language.ts:1527
+#: packages/codemirror/src/language.ts:1527 packages/codemirror/src/language.ts:1534
 msgid "TiddlyWiki"
 msgstr "TiddlyWiki"
 
-#: packages/codemirror/src/language.ts:1536
+#: packages/codemirror/src/language.ts:1536 packages/codemirror/src/language.ts:1543
 msgid "Tiki wiki"
 msgstr "Tiki wiki"
 
-#: packages/codemirror/src/language.ts:1545
+#: packages/codemirror/src/language.ts:1545 packages/codemirror/src/language.ts:1552
 msgid "TOML"
 msgstr "TOML"
 
-#: packages/codemirror/src/language.ts:1555
+#: packages/codemirror/src/language.ts:1555 packages/codemirror/src/language.ts:1562
 msgid "troff"
 msgstr "troff"
 
-#: packages/codemirror/src/language.ts:1565
+#: packages/codemirror/src/language.ts:1565 packages/codemirror/src/language.ts:1572
 msgid "TTCN"
 msgstr "TTCN"
 
-#: packages/codemirror/src/language.ts:1575
+#: packages/codemirror/src/language.ts:1575 packages/codemirror/src/language.ts:1582
 msgid "TTCN_CFG"
 msgstr "TTCN_CFG"
 
-#: packages/codemirror/src/language.ts:1585
+#: packages/codemirror/src/language.ts:1585 packages/codemirror/src/language.ts:1592
 msgid "Turtle"
 msgstr "Turtle"
 
-#: packages/codemirror/src/language.ts:1595
+#: packages/codemirror/src/language.ts:1595 packages/codemirror/src/language.ts:1602
 msgid "Web IDL"
 msgstr "Web IDL"
 
-#: packages/codemirror/src/language.ts:1605
+#: packages/codemirror/src/language.ts:1605 packages/codemirror/src/language.ts:1612
 msgid "VB.NET"
 msgstr "VB.NET"
 
-#: packages/codemirror/src/language.ts:1615
+#: packages/codemirror/src/language.ts:1615 packages/codemirror/src/language.ts:1622
 msgid "VBScript"
 msgstr "VBScript"
 
-#: packages/codemirror/src/language.ts:1625
+#: packages/codemirror/src/language.ts:1625 packages/codemirror/src/language.ts:1632
 msgid "Velocity"
 msgstr "Velocity"
 
-#: packages/codemirror/src/language.ts:1635
+#: packages/codemirror/src/language.ts:1635 packages/codemirror/src/language.ts:1642
 msgid "Verilog"
 msgstr "Verilog"
 
-#: packages/codemirror/src/language.ts:1645
+#: packages/codemirror/src/language.ts:1645 packages/codemirror/src/language.ts:1652
 msgid "VHDL"
 msgstr "VHDL"
 
-#: packages/codemirror/src/language.ts:1655
+#: packages/codemirror/src/language.ts:1655 packages/codemirror/src/language.ts:1662
 msgid "XQuery"
 msgstr "XQuery"
 
-#: packages/codemirror/src/language.ts:1665
+#: packages/codemirror/src/language.ts:1665 packages/codemirror/src/language.ts:1672
 msgid "Yacas"
 msgstr "Yacas"
 
-#: packages/codemirror/src/language.ts:1675
+#: packages/codemirror/src/language.ts:1675 packages/codemirror/src/language.ts:1682
 msgid "YAML"
 msgstr "YAML"
 
-#: packages/codemirror/src/language.ts:1686
+#: packages/codemirror/src/language.ts:1686 packages/codemirror/src/language.ts:1693
 msgid "Z80"
 msgstr "Z80"
 
-#: packages/codemirror/src/language.ts:1696
+#: packages/codemirror/src/language.ts:1696 packages/codemirror/src/language.ts:1703
 msgid "mscgen"
 msgstr "mscgen"
 
-#: packages/codemirror/src/language.ts:1706
+#: packages/codemirror/src/language.ts:1706 packages/codemirror/src/language.ts:1713
 msgid "xu"
 msgstr "xu"
 
-#: packages/codemirror/src/language.ts:1716
+#: packages/codemirror/src/language.ts:1716 packages/codemirror/src/language.ts:1723
 msgid "msgenny"
 msgstr "msgenny"
 
-#: packages/codemirror/src/language.ts:307
+#: packages/codemirror/src/language.ts:307 packages/codemirror/src/language.ts:308
 msgid "C"
 msgstr "C"
 
-#: packages/codemirror/src/language.ts:317
+#: packages/codemirror/src/language.ts:317 packages/codemirror/src/language.ts:318
 msgid "C++"
 msgstr "C++"
 
-#: packages/codemirror/src/language.ts:327
+#: packages/codemirror/src/language.ts:327 packages/codemirror/src/language.ts:328
 msgid "CQL"
 msgstr "CQL"
 
-#: packages/codemirror/src/language.ts:336
+#: packages/codemirror/src/language.ts:336 packages/codemirror/src/language.ts:337
 msgid "CSS"
 msgstr "CSS"
 
-#: packages/codemirror/src/language.ts:346 packages/notebook-extension/src/index.ts:3799
+#: packages/codemirror/src/language.ts:346 packages/codemirror/src/language.ts:347 packages/notebook-extension/src/index.ts:3799 packages/notebook-extension/src/index.ts:3806 packages/notebook-extension/src/index.ts:3865
 msgid "HTML"
 msgstr "HTML"
 
-#: packages/codemirror/src/language.ts:357
+#: packages/codemirror/src/language.ts:357 packages/codemirror/src/language.ts:358
 msgid "Java"
 msgstr "Java"
 
-#: packages/codemirror/src/language.ts:367
+#: packages/codemirror/src/language.ts:367 packages/codemirror/src/language.ts:368
 msgid "Javascript"
 msgstr "Javascript"
 
-#: packages/codemirror/src/language.ts:384
+#: packages/codemirror/src/language.ts:384 packages/codemirror/src/language.ts:385
 msgid "JSON"
 msgstr "JSON"
 
-#: packages/codemirror/src/language.ts:395
+#: packages/codemirror/src/language.ts:395 packages/codemirror/src/language.ts:396
 msgid "JSX"
 msgstr "JSX"
 
-#: packages/codemirror/src/language.ts:405
+#: packages/codemirror/src/language.ts:405 packages/codemirror/src/language.ts:406
 msgid "MariaDB SQL"
 msgstr "MariaDB SQL"
 
-#: packages/codemirror/src/language.ts:413 packages/notebook-extension/src/index.ts:3801 packages/notebook/src/default-toolbar.tsx:379
+#: packages/codemirror/src/language.ts:413 packages/codemirror/src/language.ts:414 packages/notebook-extension/src/index.ts:3801 packages/notebook-extension/src/index.ts:3808 packages/notebook-extension/src/index.ts:3867 packages/notebook/src/default-toolbar.tsx:379
 msgid "Markdown"
 msgstr "Markdown"
 
-#: packages/codemirror/src/language.ts:423
+#: packages/codemirror/src/language.ts:423 packages/codemirror/src/language.ts:424
 msgid "MS SQL"
 msgstr "MS SQL"
 
-#: packages/codemirror/src/language.ts:431
+#: packages/codemirror/src/language.ts:431 packages/codemirror/src/language.ts:432
 msgid "MySQL"
 msgstr "MySQL"
 
-#: packages/codemirror/src/language.ts:439
+#: packages/codemirror/src/language.ts:439 packages/codemirror/src/language.ts:440
 msgid "PHP"
 msgstr "PHP"
 
-#: packages/codemirror/src/language.ts:453
+#: packages/codemirror/src/language.ts:453 packages/codemirror/src/language.ts:454
 msgid "PLSQL"
 msgstr "PLSQL"
 
-#: packages/codemirror/src/language.ts:462
+#: packages/codemirror/src/language.ts:462 packages/codemirror/src/language.ts:463
 msgid "PostgreSQL"
 msgstr "PostgreSQL"
 
-#: packages/codemirror/src/language.ts:470
+#: packages/codemirror/src/language.ts:470 packages/codemirror/src/language.ts:471
 msgid "Python"
 msgstr "Python"
 
-#: packages/codemirror/src/language.ts:481
+#: packages/codemirror/src/language.ts:481 packages/codemirror/src/language.ts:485
 msgid "ipython"
 msgstr "ipython"
 
-#: packages/codemirror/src/language.ts:493
+#: packages/codemirror/src/language.ts:493 packages/codemirror/src/language.ts:500
 msgid "Rust"
 msgstr "Rust"
 
-#: packages/codemirror/src/language.ts:503
+#: packages/codemirror/src/language.ts:503 packages/codemirror/src/language.ts:510
 msgid "SQL"
 msgstr "SQL"
 
-#: packages/codemirror/src/language.ts:512
+#: packages/codemirror/src/language.ts:512 packages/codemirror/src/language.ts:519
 msgid "SQLite"
 msgstr "SQLite"
 
-#: packages/codemirror/src/language.ts:520
+#: packages/codemirror/src/language.ts:520 packages/codemirror/src/language.ts:527
 msgid "TSX"
 msgstr "TSX"
 
-#: packages/codemirror/src/language.ts:531
+#: packages/codemirror/src/language.ts:531 packages/codemirror/src/language.ts:538
 msgid "TypeScript"
 msgstr "TypeScript"
 
-#: packages/codemirror/src/language.ts:542
+#: packages/codemirror/src/language.ts:542 packages/codemirror/src/language.ts:549
 msgid "WebAssembly"
 msgstr "WebAssembly"
 
-#: packages/codemirror/src/language.ts:552
+#: packages/codemirror/src/language.ts:552 packages/codemirror/src/language.ts:559
 msgid "XML"
 msgstr "XML"
 
-#: packages/codemirror/src/language.ts:564
+#: packages/codemirror/src/language.ts:564 packages/codemirror/src/language.ts:571
 msgid "APL"
 msgstr "APL"
 
-#: packages/codemirror/src/language.ts:574
+#: packages/codemirror/src/language.ts:574 packages/codemirror/src/language.ts:581
 msgid "PGP"
 msgstr "PGP"
 
-#: packages/codemirror/src/language.ts:590
+#: packages/codemirror/src/language.ts:590 packages/codemirror/src/language.ts:597
 msgid "ASN.1"
 msgstr "ASN.1"
 
-#: packages/codemirror/src/language.ts:600
+#: packages/codemirror/src/language.ts:600 packages/codemirror/src/language.ts:607
 msgid "Asterisk"
 msgstr "Аstеrisк"
 
-#: packages/codemirror/src/language.ts:610
+#: packages/codemirror/src/language.ts:610 packages/codemirror/src/language.ts:617
 msgid "Brainfuck"
 msgstr "Brainfuck"
 
-#: packages/codemirror/src/language.ts:620
+#: packages/codemirror/src/language.ts:620 packages/codemirror/src/language.ts:627
 msgid "Cobol"
 msgstr "Cobol"
 
-#: packages/codemirror/src/language.ts:630
+#: packages/codemirror/src/language.ts:630 packages/codemirror/src/language.ts:637
 msgid "C#"
 msgstr "C#"
 
-#: packages/codemirror/src/language.ts:641
+#: packages/codemirror/src/language.ts:641 packages/codemirror/src/language.ts:648
 msgid "Clojure"
 msgstr "Clojure"
 
-#: packages/codemirror/src/language.ts:651
+#: packages/codemirror/src/language.ts:651 packages/codemirror/src/language.ts:658
 msgid "ClojureScript"
 msgstr "ClojureScript"
 
-#: packages/codemirror/src/language.ts:661
+#: packages/codemirror/src/language.ts:661 packages/codemirror/src/language.ts:668
 msgid "Closure Stylesheets (GSS)"
 msgstr "Стили Closure (GSS)"
 
-#: packages/codemirror/src/language.ts:671
+#: packages/codemirror/src/language.ts:671 packages/codemirror/src/language.ts:678
 msgid "CMake"
 msgstr "CMake"
 
-#: packages/codemirror/src/language.ts:682
+#: packages/codemirror/src/language.ts:682 packages/codemirror/src/language.ts:689
 msgid "CoffeeScript"
 msgstr "CoffeeScript"
 
-#: packages/codemirror/src/language.ts:697
+#: packages/codemirror/src/language.ts:697 packages/codemirror/src/language.ts:704
 msgid "Common Lisp"
 msgstr "Common Lisp"
 
-#: packages/codemirror/src/language.ts:708
+#: packages/codemirror/src/language.ts:708 packages/codemirror/src/language.ts:715
 msgid "Cypher"
 msgstr "Cypher"
 
-#: packages/codemirror/src/language.ts:718
+#: packages/codemirror/src/language.ts:718 packages/codemirror/src/language.ts:725
 msgid "Cython"
 msgstr "Cython"
 
-#: packages/codemirror/src/language.ts:728
+#: packages/codemirror/src/language.ts:728 packages/codemirror/src/language.ts:735
 msgid "Crystal"
 msgstr "Crystal"
 
-#: packages/codemirror/src/language.ts:738
+#: packages/codemirror/src/language.ts:738 packages/codemirror/src/language.ts:745
 msgid "D"
 msgstr "D"
 
-#: packages/codemirror/src/language.ts:748
+#: packages/codemirror/src/language.ts:748 packages/codemirror/src/language.ts:755
 msgid "Dart"
 msgstr "Dart"
 
-#: packages/codemirror/src/language.ts:758
+#: packages/codemirror/src/language.ts:758 packages/codemirror/src/language.ts:765
 msgid "diff"
 msgstr "разница"
 
-#: packages/codemirror/src/language.ts:768
+#: packages/codemirror/src/language.ts:768 packages/codemirror/src/language.ts:775
 msgid "Dockerfile"
 msgstr "Dockerfile"
 
-#: packages/codemirror/src/language.ts:778
+#: packages/codemirror/src/language.ts:778 packages/codemirror/src/language.ts:785
 msgid "DTD"
 msgstr "DTD"
 
-#: packages/codemirror/src/language.ts:788
+#: packages/codemirror/src/language.ts:788 packages/codemirror/src/language.ts:795
 msgid "Dylan"
 msgstr "Dylan"
 
-#: packages/codemirror/src/language.ts:798
+#: packages/codemirror/src/language.ts:798 packages/codemirror/src/language.ts:805
 msgid "EBNF"
 msgstr "EBNF"
 
-#: packages/codemirror/src/language.ts:807
+#: packages/codemirror/src/language.ts:807 packages/codemirror/src/language.ts:814
 msgid "ECL"
 msgstr "ECL"
 
-#: packages/codemirror/src/language.ts:817
+#: packages/codemirror/src/language.ts:817 packages/codemirror/src/language.ts:824
 msgid "edn"
 msgstr "edn"
 
-#: packages/codemirror/src/language.ts:827
+#: packages/codemirror/src/language.ts:827 packages/codemirror/src/language.ts:834
 msgid "Eiffel"
 msgstr "Eiffel"
 
-#: packages/codemirror/src/language.ts:837
+#: packages/codemirror/src/language.ts:837 packages/codemirror/src/language.ts:844
 msgid "Elm"
 msgstr "Elm"
 
-#: packages/codemirror/src/language.ts:847
+#: packages/codemirror/src/language.ts:847 packages/codemirror/src/language.ts:854
 msgid "Erlang"
 msgstr "Erlang"
 
-#: packages/codemirror/src/language.ts:857
+#: packages/codemirror/src/language.ts:857 packages/codemirror/src/language.ts:864
 msgid "Esper"
 msgstr "Esper"
 
-#: packages/codemirror/src/language.ts:866
+#: packages/codemirror/src/language.ts:866 packages/codemirror/src/language.ts:873
 msgid "Factor"
 msgstr "Factor"
 
-#: packages/codemirror/src/language.ts:876
+#: packages/codemirror/src/language.ts:876 packages/codemirror/src/language.ts:883
 msgid "FCL"
 msgstr "FCL"
 
-#: packages/codemirror/src/language.ts:885
+#: packages/codemirror/src/language.ts:885 packages/codemirror/src/language.ts:892
 msgid "Forth"
 msgstr "Forth"
 
-#: packages/codemirror/src/language.ts:895
+#: packages/codemirror/src/language.ts:895 packages/codemirror/src/language.ts:902
 msgid "Fortran"
 msgstr "Fortran"
 
-#: packages/codemirror/src/language.ts:905
+#: packages/codemirror/src/language.ts:905 packages/codemirror/src/language.ts:912
 msgid "F#"
 msgstr "F#"
 
-#: packages/codemirror/src/language.ts:916
+#: packages/codemirror/src/language.ts:916 packages/codemirror/src/language.ts:923
 msgid "Gas"
 msgstr "Gas"
 
-#: packages/codemirror/src/language.ts:926
+#: packages/codemirror/src/language.ts:926 packages/codemirror/src/language.ts:933
 msgid "Gherkin"
 msgstr "Gherkin"
 
-#: packages/codemirror/src/language.ts:936
+#: packages/codemirror/src/language.ts:936 packages/codemirror/src/language.ts:943
 msgid "Go"
 msgstr "Go"
 
-#: packages/codemirror/src/language.ts:946
+#: packages/codemirror/src/language.ts:946 packages/codemirror/src/language.ts:953
 msgid "Groovy"
 msgstr "Groovy"
 
-#: packages/codemirror/src/language.ts:957
+#: packages/codemirror/src/language.ts:957 packages/codemirror/src/language.ts:964
 msgid "Haskell"
 msgstr "Haskell"
 
-#: packages/codemirror/src/language.ts:967
+#: packages/codemirror/src/language.ts:967 packages/codemirror/src/language.ts:974
 msgid "Haxe"
 msgstr "Haxe"
 
-#: packages/codemirror/src/language.ts:977
+#: packages/codemirror/src/language.ts:977 packages/codemirror/src/language.ts:984
 msgid "HXML"
 msgstr "HXML"
 
-#: packages/codemirror/src/language.ts:987
+#: packages/codemirror/src/language.ts:987 packages/codemirror/src/language.ts:994
 msgid "HTTP"
 msgstr "HTTP"
 
-#: packages/codemirror/src/language.ts:996
-msgid "IDL"
-msgstr "IDL"
-
-#: packages/codemirror/src/theme.ts:234
+#: packages/codemirror/src/theme.ts:234 packages/codemirror/src/theme.ts:238
 msgid "codemirror"
 msgstr "зеркало кода"
 
 #: packages/completer-extension/src/index.ts:138
 msgid "Previous"
 msgstr ""
 
@@ -4017,151 +4107,159 @@
 msgid "%1/%2"
 msgstr ""
 
 #: packages/completer/src/inline.ts:393
 msgid "Provider: %1"
 msgstr ""
 
-#: packages/console-extension/src/foreign.ts:66 packages/console-extension/src/index.ts:262 packages/console-extension/src/index.ts:311 packages/console-extension/src/index.ts:530 packages/console/src/panel.ts:333 packages/launcher/src/widget.tsx:116 packages/launcher/src/widget.tsx:121
+#: packages/console-extension/src/foreign.ts:66 packages/console-extension/src/index.ts:262 packages/console-extension/src/index.ts:271 packages/console-extension/src/index.ts:275 packages/console-extension/src/index.ts:311 packages/console-extension/src/index.ts:320 packages/console-extension/src/index.ts:324 packages/console-extension/src/index.ts:530 packages/console-extension/src/index.ts:539 packages/console-extension/src/index.ts:542 packages/console/src/panel.ts:333 packages/console/src/panel.ts:341 packages/launcher/src/widget.tsx:116 packages/launcher/src/widget.tsx:121
 msgid "Console"
 msgstr "Консоль"
 
 #: packages/console-extension/src/foreign.ts:80
 msgid "Show All Kernel Activity"
 msgstr "Показать всю активность ядра"
 
-#: packages/console-extension/src/index.ts:464
+#: packages/console-extension/src/index.ts:464 packages/console-extension/src/index.ts:473 packages/console-extension/src/index.ts:478
 msgid "Auto Close Brackets for Code Console Prompt"
 msgstr "Автоматическое закрытие скобок для консоли"
 
-#: packages/console-extension/src/index.ts:490
+#: packages/console-extension/src/index.ts:490 packages/console-extension/src/index.ts:499 packages/console-extension/src/index.ts:503
 msgid "Open a console for the provided `path`."
 msgstr "Откройте консоль для указанного `path`."
 
-#: packages/console-extension/src/index.ts:519
+#: packages/console-extension/src/index.ts:519 packages/console-extension/src/index.ts:528 packages/console-extension/src/index.ts:531
 msgid "New Console"
 msgstr "Новая консоль"
 
-#: packages/console-extension/src/index.ts:554
+#: packages/console-extension/src/index.ts:554 packages/console-extension/src/index.ts:631 packages/console-extension/src/index.ts:634
 msgid "Clear Console Cells"
 msgstr "Очистить ячейки консоли"
 
-#: packages/console-extension/src/index.ts:566
+#: packages/console-extension/src/index.ts:566 packages/console-extension/src/index.ts:643 packages/console-extension/src/index.ts:646
 msgid "Run Cell (unforced)"
 msgstr "Выполнить ячейку (без принудительного использования)"
 
-#: packages/console-extension/src/index.ts:578
+#: packages/console-extension/src/index.ts:578 packages/console-extension/src/index.ts:655 packages/console-extension/src/index.ts:658
 msgid "Run Cell (forced)"
 msgstr "Выполнить ячейку (принудительно)"
 
-#: packages/console-extension/src/index.ts:590
+#: packages/console-extension/src/index.ts:590 packages/console-extension/src/index.ts:667 packages/console-extension/src/index.ts:670
 msgid "Insert Line Break"
 msgstr "Вставить разрыв строки"
 
-#: packages/console-extension/src/index.ts:602
+#: packages/console-extension/src/index.ts:593 packages/console-extension/src/index.ts:596 packages/fileeditor-extension/src/commands.ts:853 packages/fileeditor-extension/src/commands.ts:854 packages/mainmenu-extension/src/index.ts:277 packages/notebook-extension/src/index.ts:3122 packages/notebook-extension/src/index.ts:3129 packages/notebook-extension/src/index.ts:3152
+msgid "Undo"
+msgstr "Отменить"
+
+#: packages/console-extension/src/index.ts:602 packages/console-extension/src/index.ts:679 packages/console-extension/src/index.ts:682
 msgid "Replace Selection in Console"
 msgstr "Заменить выделенное в консоли"
 
-#: packages/console-extension/src/index.ts:615 packages/mainmenu-extension/src/index.ts:468 packages/notebook-extension/src/index.ts:2528
+#: packages/console-extension/src/index.ts:615 packages/console-extension/src/index.ts:692 packages/console-extension/src/index.ts:695 packages/mainmenu-extension/src/index.ts:466 packages/mainmenu-extension/src/index.ts:468 packages/notebook-extension/src/index.ts:2528 packages/notebook-extension/src/index.ts:2535 packages/notebook-extension/src/index.ts:2546
 msgid "Interrupt Kernel"
 msgstr "Прервать выполнение ядра"
 
-#: packages/console-extension/src/index.ts:630 packages/mainmenu-extension/src/index.ts:493 packages/notebook-extension/src/index.ts:2376
+#: packages/console-extension/src/index.ts:627 packages/console-extension/src/index.ts:630 packages/fileeditor-extension/src/commands.ts:883 packages/fileeditor-extension/src/commands.ts:884 packages/fileeditor-extension/src/commands.ts:885 packages/mainmenu-extension/src/index.ts:287 packages/mainmenu-extension/src/index.ts:288 packages/notebook-extension/src/index.ts:3108 packages/notebook-extension/src/index.ts:3115 packages/notebook-extension/src/index.ts:3138
+msgid "Redo"
+msgstr "Повторить"
+
+#: packages/console-extension/src/index.ts:630 packages/console-extension/src/index.ts:707 packages/console-extension/src/index.ts:710 packages/mainmenu-extension/src/index.ts:491 packages/mainmenu-extension/src/index.ts:493 packages/notebook-extension/src/index.ts:2376 packages/notebook-extension/src/index.ts:2383 packages/notebook-extension/src/index.ts:2394
 msgid "Restart Kernel…"
 msgstr "Перезапустить ядро…"
 
-#: packages/console-extension/src/index.ts:642 packages/lsp-extension/src/index.ts:303 packages/mainmenu-extension/src/index.ts:375 packages/mainmenu-extension/src/index.ts:385 packages/running/src/index.tsx:161 packages/terminal-extension/src/index.ts:322
+#: packages/console-extension/src/index.ts:642 packages/console-extension/src/index.ts:719 packages/console-extension/src/index.ts:722 packages/lsp-extension/src/index.ts:303 packages/mainmenu-extension/src/index.ts:371 packages/mainmenu-extension/src/index.ts:375 packages/mainmenu-extension/src/index.ts:381 packages/mainmenu-extension/src/index.ts:385 packages/running/src/index.tsx:161 packages/running/src/index.tsx:221 packages/terminal-extension/src/index.ts:322
 msgid "Shut Down"
 msgstr "Завершить работу"
 
-#: packages/console-extension/src/index.ts:654
+#: packages/console-extension/src/index.ts:654 packages/console-extension/src/index.ts:731 packages/console-extension/src/index.ts:734
 msgid "Close and Shut Down…"
 msgstr "Закрыть и выключить…"
 
-#: packages/console-extension/src/index.ts:661
+#: packages/console-extension/src/index.ts:661 packages/console-extension/src/index.ts:738 packages/console-extension/src/index.ts:741
 msgid "Shut down the console?"
 msgstr "Завершить работу консоли?"
 
-#: packages/console-extension/src/index.ts:662 packages/notebook-extension/src/index.ts:2414
+#: packages/console-extension/src/index.ts:662 packages/console-extension/src/index.ts:739 packages/console-extension/src/index.ts:742 packages/notebook-extension/src/index.ts:2414 packages/notebook-extension/src/index.ts:2421 packages/notebook-extension/src/index.ts:2432
 msgid "Are you sure you want to close \"%1\"?"
 msgstr "Вы уверены, что хотите закрыть \"%1\"?"
 
-#: packages/console-extension/src/index.ts:668
+#: packages/console-extension/src/index.ts:668 packages/console-extension/src/index.ts:745 packages/console-extension/src/index.ts:748
 msgid "Cancel console Shut Down"
 msgstr "Отменить закрытие консоли"
 
-#: packages/console-extension/src/index.ts:671
+#: packages/console-extension/src/index.ts:671 packages/console-extension/src/index.ts:748 packages/console-extension/src/index.ts:751
 msgid "Confirm console Shut Down"
 msgstr "Подтвердите остановку консоли"
 
-#: packages/console-extension/src/index.ts:691
+#: packages/console-extension/src/index.ts:691 packages/console-extension/src/index.ts:768 packages/console-extension/src/index.ts:771
 msgid "Inject some code in a console."
 msgstr "Вставьте код в консоль."
 
-#: packages/console-extension/src/index.ts:712 packages/mainmenu-extension/src/index.ts:519 packages/notebook-extension/src/index.ts:3136
+#: packages/console-extension/src/index.ts:712 packages/console-extension/src/index.ts:789 packages/console-extension/src/index.ts:792 packages/mainmenu-extension/src/index.ts:518 packages/mainmenu-extension/src/index.ts:519 packages/notebook-extension/src/index.ts:3136 packages/notebook-extension/src/index.ts:3143 packages/notebook-extension/src/index.ts:3166
 msgid "Change Kernel…"
 msgstr "Сменить ядро…"
 
-#: packages/console-extension/src/index.ts:724 packages/mainmenu-extension/src/index.ts:754 packages/notebook-extension/src/index.ts:3147
+#: packages/console-extension/src/index.ts:724 packages/console-extension/src/index.ts:801 packages/console-extension/src/index.ts:804 packages/mainmenu-extension/src/index.ts:752 packages/mainmenu-extension/src/index.ts:754 packages/notebook-extension/src/index.ts:3147 packages/notebook-extension/src/index.ts:3154 packages/notebook-extension/src/index.ts:3177
 msgid "Get Kernel"
 msgstr "Получить ядро"
 
-#: packages/console-extension/src/index.ts:806
+#: packages/console-extension/src/index.ts:806 packages/console-extension/src/index.ts:893 packages/console-extension/src/index.ts:907
 msgid "Execute with Shift+Enter"
 msgstr "Выполнение с помощью Shift+Enter"
 
-#: packages/console-extension/src/index.ts:807
+#: packages/console-extension/src/index.ts:807 packages/console-extension/src/index.ts:894 packages/console-extension/src/index.ts:908
 msgid "Execute with Enter"
 msgstr "Выполнение с помощью Enter"
 
-#: packages/console-extension/src/index.ts:851 packages/fileeditor-extension/src/commands.ts:1012 packages/notebook-extension/src/index.ts:2027
+#: packages/console-extension/src/index.ts:851 packages/console-extension/src/index.ts:938 packages/console-extension/src/index.ts:952 packages/fileeditor-extension/src/commands.ts:1010 packages/fileeditor-extension/src/commands.ts:1012 packages/fileeditor-extension/src/commands.ts:1041 packages/notebook-extension/src/index.ts:2027 packages/notebook-extension/src/index.ts:2034 packages/notebook-extension/src/index.ts:2045
 msgid "Display the completion helper."
 msgstr "Отобразить помощника завершения."
 
-#: packages/console-extension/src/index.ts:862 packages/fileeditor-extension/src/commands.ts:1023 packages/notebook-extension/src/index.ts:2037
+#: packages/console-extension/src/index.ts:862 packages/console-extension/src/index.ts:949 packages/console-extension/src/index.ts:963 packages/fileeditor-extension/src/commands.ts:1021 packages/fileeditor-extension/src/commands.ts:1023 packages/fileeditor-extension/src/commands.ts:1052 packages/notebook-extension/src/index.ts:2037 packages/notebook-extension/src/index.ts:2044 packages/notebook-extension/src/index.ts:2055
 msgid "Select the completion suggestion."
 msgstr "Выберите вариант завершения."
 
-#: packages/console/src/panel.ts:316
+#: packages/console/src/panel.ts:316 packages/console/src/panel.ts:324
 msgid "Name: %1\n"
 msgstr "Имя: %1\n"
 
-#: packages/console/src/panel.ts:317
+#: packages/console/src/panel.ts:317 packages/console/src/panel.ts:325
 msgid "Directory: %1\n"
 msgstr "Каталог: %1\n"
 
-#: packages/console/src/panel.ts:318
+#: packages/console/src/panel.ts:318 packages/console/src/panel.ts:326
 msgid "Kernel: %1"
 msgstr "Ядро: %1"
 
-#: packages/console/src/panel.ts:321
+#: packages/console/src/panel.ts:321 packages/console/src/panel.ts:329
 msgid "\n"
 "Connected: %1"
 msgstr "\n"
 "Подключён к: %1"
 
-#: packages/console/src/panel.ts:328
+#: packages/console/src/panel.ts:328 packages/console/src/panel.ts:336
 msgid "\n"
 "Last Execution: %1"
 msgstr "\n"
 "Последнее выполнение: %1"
 
-#: packages/console/src/panel.ts:66
+#: packages/console/src/panel.ts:66 packages/console/src/panel.ts:68
 msgid "Console %1"
 msgstr "Консоль %1"
 
 #: packages/csvviewer-extension/src/index.ts:134
 msgid "CSV Viewer"
 msgstr "Средство просмотра CSV"
 
-#: packages/csvviewer-extension/src/index.ts:216 packages/csvviewer-extension/src/index.ts:223 packages/csvviewer-extension/src/index.ts:370 packages/csvviewer-extension/src/index.ts:377
+#: packages/csvviewer-extension/src/index.ts:216 packages/csvviewer-extension/src/index.ts:223 packages/csvviewer-extension/src/index.ts:370 packages/csvviewer-extension/src/index.ts:376 packages/csvviewer-extension/src/index.ts:377 packages/csvviewer-extension/src/index.ts:383
 msgid "Go to Line"
 msgstr "Перейти к строке"
 
-#: packages/csvviewer-extension/src/index.ts:288
+#: packages/csvviewer-extension/src/index.ts:288 packages/csvviewer-extension/src/index.ts:294
 msgid "TSV Viewer"
 msgstr "Средство просмотра TSV"
 
 #: packages/csvviewer/src/toolbar.ts:119
 msgid "tab"
 msgstr "вкладка"
 
@@ -4310,14 +4408,18 @@
 msgstr "Не удалось получить источник"
 
 #: packages/debugger/src/panels/kernelSources/body.tsx:88
 msgid "Fail to get '%1' source:\n"
 "%2"
 msgstr "Не удалось получить '%1' источник: %2"
 
+#: packages/debugger/src/panels/kernelSources/filter.tsx:33
+msgid "Filter the kernel sources"
+msgstr ""
+
 #: packages/debugger/src/panels/kernelSources/index.tsx:33
 msgid "Kernel Sources"
 msgstr "Источники ядра"
 
 #: packages/debugger/src/panels/kernelSources/index.tsx:49
 msgid "Toggle search filter"
 msgstr "Переключить панель поиска"
@@ -4332,15 +4434,15 @@
 msgstr "Не удалось получить ресурсы ядра:\n"
 "%2"
 
 #: packages/debugger/src/panels/kernelSources/index.tsx:66
 msgid "Refresh kernel sources"
 msgstr "Обновить ресурсов ядра"
 
-#: packages/debugger/src/panels/sources/index.tsx:29 packages/shortcuts-extension/src/components/TopNav.tsx:186
+#: packages/debugger/src/panels/sources/index.tsx:29 packages/shortcuts-extension/src/components/TopNav.tsx:134 packages/shortcuts-extension/src/components/TopNav.tsx:186
 msgid "Source"
 msgstr "Источник"
 
 #: packages/debugger/src/panels/sources/index.tsx:42
 msgid "Open in the Main Area"
 msgstr "Открыть в Главной Области"
 
@@ -4348,15 +4450,15 @@
 msgid "Type"
 msgstr "Тип"
 
 #: packages/debugger/src/panels/variables/gridpanel.ts:218
 msgid "Value"
 msgstr "Значение"
 
-#: packages/debugger/src/panels/variables/gridpanel.ts:221 packages/filebrowser/src/listing.ts:2277
+#: packages/debugger/src/panels/variables/gridpanel.ts:221 packages/filebrowser/src/listing.ts:2277 packages/filebrowser/src/listing.ts:2298 packages/filebrowser/src/listing.ts:2371
 msgid "Name"
 msgstr "Имя"
 
 #: packages/debugger/src/panels/variables/index.ts:33
 msgid "Variables"
 msgstr "Переменные"
 
@@ -4380,71 +4482,79 @@
 msgid "Render variable: %1"
 msgstr "Рендер переменной: %1"
 
 #: packages/debugger/src/service.ts:378
 msgid "Globals"
 msgstr "Глобальные значения"
 
-#: packages/docmanager-extension/src/index.tsx:1007 packages/docmanager-extension/src/index.tsx:871 packages/docmanager-extension/src/index.tsx:889 packages/notebook/src/default-toolbar.tsx:68
+#: packages/docmanager-extension/src/index.tsx:1007 packages/docmanager-extension/src/index.tsx:1019 packages/docmanager-extension/src/index.tsx:871 packages/docmanager-extension/src/index.tsx:883 packages/docmanager-extension/src/index.tsx:889 packages/docmanager-extension/src/index.tsx:901 packages/notebook/src/default-toolbar.tsx:68
 msgid "Cannot Save"
 msgstr "Не удается сохранить"
 
-#: packages/docmanager-extension/src/index.tsx:1008 packages/docmanager-extension/src/index.tsx:485 packages/docmanager-extension/src/index.tsx:737 packages/docmanager-extension/src/index.tsx:782 packages/docmanager-extension/src/index.tsx:872
+#: packages/docmanager-extension/src/index.tsx:1008 packages/docmanager-extension/src/index.tsx:1020 packages/docmanager-extension/src/index.tsx:485 packages/docmanager-extension/src/index.tsx:495 packages/docmanager-extension/src/index.tsx:737 packages/docmanager-extension/src/index.tsx:749 packages/docmanager-extension/src/index.tsx:782 packages/docmanager-extension/src/index.tsx:794 packages/docmanager-extension/src/index.tsx:872 packages/docmanager-extension/src/index.tsx:884
 msgid "No context found for current widget!"
 msgstr "Контекст для текущего виджета не найден!"
 
-#: packages/docmanager-extension/src/index.tsx:1039
+#: packages/docmanager-extension/src/index.tsx:1010 packages/docmanager-extension/src/index.tsx:998
+msgid "Save %1 As…"
+msgstr "Сохранить %1 как…"
+
+#: packages/docmanager-extension/src/index.tsx:1011 packages/docmanager-extension/src/index.tsx:999
+msgid "Save with new path"
+msgstr "Сохранить по новому пути"
+
+#: packages/docmanager-extension/src/index.tsx:1039 packages/docmanager-extension/src/index.tsx:1063
 msgid "Autosave Documents"
 msgstr "Автосохранение документов"
 
-#: packages/docmanager-extension/src/index.tsx:1100
+#: packages/docmanager-extension/src/index.tsx:1100 packages/docmanager-extension/src/index.tsx:1124
 msgid "New View for %1"
 msgstr "Новое представление для %1"
 
-#: packages/docmanager-extension/src/index.tsx:1124
+#: packages/docmanager-extension/src/index.tsx:1124 packages/docmanager-extension/src/index.tsx:1148
 msgid "Rename%1…"
 msgstr "Переименовать %1…"
 
-#: packages/docmanager-extension/src/index.tsx:1138
+#: packages/docmanager-extension/src/index.tsx:1138 packages/docmanager-extension/src/index.tsx:1162
 msgid "Duplicate %1"
 msgstr "Дублировать %1"
 
-#: packages/docmanager-extension/src/index.tsx:1153
+#: packages/docmanager-extension/src/index.tsx:1153 packages/docmanager-extension/src/index.tsx:1177 packages/workspaces-extension/src/sidebar.ts:99
 msgid "Delete %1"
 msgstr "Удалить %1"
 
-#: packages/docmanager-extension/src/index.tsx:1163 packages/docmanager-extension/src/index.tsx:1167 packages/filebrowser-extension/src/index.ts:929 packages/filebrowser/src/listing.ts:430 packages/filebrowser/src/listing.ts:434
+#: packages/docmanager-extension/src/index.tsx:1163 packages/docmanager-extension/src/index.tsx:1167 packages/docmanager-extension/src/index.tsx:1187 packages/docmanager-extension/src/index.tsx:1191 packages/filebrowser-extension/src/index.ts:929 packages/filebrowser-extension/src/index.ts:937 packages/filebrowser/src/listing.ts:430 packages/filebrowser/src/listing.ts:433 packages/filebrowser/src/listing.ts:434 packages/filebrowser/src/listing.ts:437 packages/workspaces-extension/src/commands.ts:199
 msgid "Delete"
 msgstr "Удалить"
 
-#: packages/docmanager-extension/src/index.tsx:1164
+#: packages/docmanager-extension/src/index.tsx:1164 packages/docmanager-extension/src/index.tsx:1188
 msgid "Are you sure you want to delete %1"
 msgstr "Вы уверены, что хотите удалить %1"
 
-#: packages/docmanager-extension/src/index.tsx:1181
+#: packages/docmanager-extension/src/index.tsx:1181 packages/docmanager-extension/src/index.tsx:1205
 msgid "Show in File Browser"
 msgstr "Показать в проводнике"
 
-#: packages/docmanager-extension/src/index.tsx:1247
+#: packages/docmanager-extension/src/index.tsx:1247 packages/docmanager-extension/src/index.tsx:1283
 msgid "Are you sure you want to revert the %1 to checkpoint? "
 msgstr "Вы уверены, что хотите вернуть %1 к контрольной точке? "
 
-#: packages/docmanager-extension/src/index.tsx:1253
+#: packages/docmanager-extension/src/index.tsx:1253 packages/docmanager-extension/src/index.tsx:1289
 msgid "This cannot be undone."
 msgstr "Это действие не может быть отменено."
 
-#: packages/docmanager-extension/src/index.tsx:1260
+#: packages/docmanager-extension/src/index.tsx:1260 packages/docmanager-extension/src/index.tsx:1296
 msgid "The checkpoint was last updated at: "
 msgstr "Контрольная точка была последний раз обновлена в: "
 
-#: packages/docmanager-extension/src/index.tsx:1294
+#: packages/docmanager-extension/src/index.tsx:1294 packages/docmanager-extension/src/index.tsx:1330
 msgid "Choose a checkpoint"
 msgstr "Выберите контрольную точку"
 
-#: packages/docmanager-extension/src/index.tsx:345
+#: packages/docmanager-extension/src/index.tsx:345 packages/docmanager-extension/src/index.tsx:355
 msgid "Overrides for the default viewers for file types.\n"
 "Specify a mapping from file type name to document viewer name, for example:\n\n"
 "defaultViewers: {\n"
 "  markdown: \"Markdown Preview\"\n"
 "}\n\n"
 "If you specify non-existent file types or viewers, or if a viewer cannot\n"
 "open a given file type, the override will not function.\n\n"
@@ -4459,159 +4569,167 @@
 "If you specify non-existent file types or viewers, or if a viewer cannot\n"
 "open a given file type, the override will not function.\n\n"
 "Available viewers:\n"
 "%1\n\n"
 "Available file types:\n"
 "%2"
 
-#: packages/docmanager-extension/src/index.tsx:475 packages/filebrowser-extension/src/index.ts:374
+#: packages/docmanager-extension/src/index.tsx:475 packages/docmanager-extension/src/index.tsx:485 packages/filebrowser-extension/src/index.ts:374 packages/filebrowser-extension/src/index.ts:405
 msgid "Download"
 msgstr "Скачать"
 
-#: packages/docmanager-extension/src/index.tsx:476
+#: packages/docmanager-extension/src/index.tsx:476 packages/docmanager-extension/src/index.tsx:486
 msgid "Download the file to your computer"
 msgstr "Скачать файл на ваш компьютер"
 
-#: packages/docmanager-extension/src/index.tsx:484
+#: packages/docmanager-extension/src/index.tsx:484 packages/docmanager-extension/src/index.tsx:494
 msgid "Cannot Download"
 msgstr "Не удается скачать"
 
-#: packages/docmanager-extension/src/index.tsx:494 packages/docmanager-extension/src/index.tsx:635 packages/filebrowser-extension/src/index.ts:1081 packages/filebrowser-extension/src/index.ts:573 packages/filebrowser-extension/src/index.ts:899 packages/htmlviewer-extension/src/index.tsx:206
+#: packages/docmanager-extension/src/index.tsx:494 packages/docmanager-extension/src/index.tsx:508 packages/docmanager-extension/src/index.tsx:635 packages/docmanager-extension/src/index.tsx:650 packages/filebrowser-extension/src/index.ts:1081 packages/filebrowser-extension/src/index.ts:1089 packages/filebrowser-extension/src/index.ts:573 packages/filebrowser-extension/src/index.ts:581 packages/filebrowser-extension/src/index.ts:899 packages/filebrowser-extension/src/index.ts:907 packages/htmlviewer-extension/src/index.tsx:206 packages/htmlviewer-extension/src/index.tsx:211
 msgid "File Operations"
 msgstr "Операции с файлом"
 
-#: packages/docmanager-extension/src/index.tsx:543 packages/filebrowser-extension/src/index.ts:779
+#: packages/docmanager-extension/src/index.tsx:543 packages/docmanager-extension/src/index.tsx:557 packages/filebrowser-extension/src/index.ts:779 packages/filebrowser-extension/src/index.ts:787
 msgid "Open in New Browser Tab"
 msgstr "Открыть в новой вкладке браузера"
 
 #: packages/docmanager-extension/src/index.tsx:652
 msgid "%1 is permissioned as read-only. Use \"save as...\" instead."
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:681 packages/filebrowser/src/browser.ts:261 packages/logconsole-extension/src/index.tsx:376
+#: packages/docmanager-extension/src/index.tsx:667
+msgid "%1 is read-only. Use \"Save as…\" instead."
+msgstr ""
+
+#: packages/docmanager-extension/src/index.tsx:681 packages/docmanager-extension/src/index.tsx:693 packages/filebrowser/src/browser.ts:261 packages/filebrowser/src/browser.ts:267 packages/logconsole-extension/src/index.tsx:376
 msgid "Error"
 msgstr "Ошибка"
 
-#: packages/docmanager-extension/src/index.tsx:715
+#: packages/docmanager-extension/src/index.tsx:715 packages/docmanager-extension/src/index.tsx:727
 msgid "Open the provided `path`."
 msgstr "Откройте указанный путь `path`."
 
-#: packages/docmanager-extension/src/index.tsx:721 packages/docmanager-extension/src/index.tsx:743
+#: packages/docmanager-extension/src/index.tsx:721 packages/docmanager-extension/src/index.tsx:733 packages/docmanager-extension/src/index.tsx:743 packages/docmanager-extension/src/index.tsx:755
 msgid "Reload %1 from Disk"
 msgstr "Перезагрузить %1 с диска"
 
-#: packages/docmanager-extension/src/index.tsx:725
+#: packages/docmanager-extension/src/index.tsx:725 packages/docmanager-extension/src/index.tsx:737
 msgid "Reload contents from disk"
 msgstr "Перезагрузить содержимое с диска"
 
-#: packages/docmanager-extension/src/index.tsx:736
+#: packages/docmanager-extension/src/index.tsx:736 packages/docmanager-extension/src/index.tsx:748
 msgid "Cannot Reload"
 msgstr "Невозможно перезагрузить"
 
-#: packages/docmanager-extension/src/index.tsx:744
+#: packages/docmanager-extension/src/index.tsx:744 packages/docmanager-extension/src/index.tsx:756
 msgid "Are you sure you want to reload the %1 from the disk?"
 msgstr "Вы уверены, что хотите перезагрузить %1 с диска?"
 
-#: packages/docmanager-extension/src/index.tsx:767
+#: packages/docmanager-extension/src/index.tsx:767 packages/docmanager-extension/src/index.tsx:779
 msgid "Revert %1 to Checkpoint…"
 msgstr "Вернуть %1 к контрольной точке…"
 
-#: packages/docmanager-extension/src/index.tsx:771
+#: packages/docmanager-extension/src/index.tsx:771 packages/docmanager-extension/src/index.tsx:783
 msgid "Revert contents to previous checkpoint"
 msgstr "Вернуть содержимое к предыдущей контрольной точке"
 
-#: packages/docmanager-extension/src/index.tsx:781
+#: packages/docmanager-extension/src/index.tsx:781 packages/docmanager-extension/src/index.tsx:793
 msgid "Cannot Revert"
 msgstr "Не удается восстановить"
 
-#: packages/docmanager-extension/src/index.tsx:790
+#: packages/docmanager-extension/src/index.tsx:790 packages/docmanager-extension/src/index.tsx:802
 msgid "No checkpoints"
 msgstr "Нет контрольных точек"
 
-#: packages/docmanager-extension/src/index.tsx:791
+#: packages/docmanager-extension/src/index.tsx:791 packages/docmanager-extension/src/index.tsx:803
 msgid "No checkpoints are available for this %1."
 msgstr "Для %1 нет доступных контрольных точек."
 
-#: packages/docmanager-extension/src/index.tsx:804
+#: packages/docmanager-extension/src/index.tsx:804 packages/docmanager-extension/src/index.tsx:816
 msgid "Revert %1 to checkpoint"
 msgstr "Вернуть %1 к контрольной точке"
 
-#: packages/docmanager-extension/src/index.tsx:809 packages/docregistry/src/context.ts:827
+#: packages/docmanager-extension/src/index.tsx:809 packages/docmanager-extension/src/index.tsx:821 packages/docregistry/src/context.ts:825 packages/docregistry/src/context.ts:827
 msgid "Revert"
 msgstr "Вернуть"
 
-#: packages/docmanager-extension/src/index.tsx:810
+#: packages/docmanager-extension/src/index.tsx:810 packages/docmanager-extension/src/index.tsx:822
 msgid "Revert to Checkpoint"
 msgstr "Вернуться к контрольной точке"
 
-#: packages/docmanager-extension/src/index.tsx:834
+#: packages/docmanager-extension/src/index.tsx:834 packages/docmanager-extension/src/index.tsx:846
 msgid "In collaborative mode, the document is saved automatically after every change"
 msgstr "В совместном режиме документ сохраняется автоматически после каждого изменения"
 
 #: packages/docmanager-extension/src/index.tsx:839
 msgid "document is permissioned readonly; \"save\" is disabled, use \"save as...\" instead"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:845
+#: packages/docmanager-extension/src/index.tsx:845 packages/docmanager-extension/src/index.tsx:857
 msgid "Save and create checkpoint"
 msgstr "Сохранить и создать контрольную точку"
 
-#: packages/docmanager-extension/src/index.tsx:851
+#: packages/docmanager-extension/src/index.tsx:851 packages/docmanager-extension/src/index.tsx:863
 msgid "Save %1"
 msgstr "Сохранить %1"
 
-#: packages/docmanager-extension/src/index.tsx:890 packages/notebook/src/default-toolbar.tsx:69
+#: packages/docmanager-extension/src/index.tsx:851 packages/docregistry/src/components.tsx:25
+msgid "Document is read-only. \"Save\" is disabled; use \"Save as…\" instead"
+msgstr ""
+
+#: packages/docmanager-extension/src/index.tsx:890 packages/docmanager-extension/src/index.tsx:902 packages/notebook/src/default-toolbar.tsx:69
 msgid "Document is read-only"
 msgstr "Документ доступен только для чтения"
 
-#: packages/docmanager-extension/src/index.tsx:906
+#: packages/docmanager-extension/src/index.tsx:906 packages/docmanager-extension/src/index.tsx:918
 msgid "Rename file"
 msgstr "Переименовать файл"
 
-#: packages/docmanager-extension/src/index.tsx:907 packages/docmanager/src/dialogs.ts:58 packages/filebrowser-extension/src/index.ts:1204
+#: packages/docmanager-extension/src/index.tsx:907 packages/docmanager-extension/src/index.tsx:919 packages/docmanager/src/dialogs.ts:58 packages/filebrowser-extension/src/index.ts:1204 packages/filebrowser-extension/src/index.ts:1212 packages/workspaces-extension/src/commands.ts:285
 msgid "Rename"
 msgstr "Переименовать"
 
-#: packages/docmanager-extension/src/index.tsx:908
+#: packages/docmanager-extension/src/index.tsx:908 packages/docmanager-extension/src/index.tsx:920
 msgid "File name"
 msgstr "Имя файла"
 
-#: packages/docmanager-extension/src/index.tsx:912 packages/docmanager/src/widgetmanager.ts:420
+#: packages/docmanager-extension/src/index.tsx:912 packages/docmanager-extension/src/index.tsx:924 packages/docmanager/src/widgetmanager.ts:420 packages/docmanager/src/widgetmanager.ts:491
 msgid "Do not ask me again."
 msgstr "Не спрашивать в следующий раз."
 
-#: packages/docmanager-extension/src/index.tsx:913
+#: packages/docmanager-extension/src/index.tsx:913 packages/docmanager-extension/src/index.tsx:925
 msgid "If checked, you will not be asked to rename future untitled files when saving them."
 msgstr "Если флажок установлен, то при сохранении файлов без названия вас не попросят переименовывать будущие файлы."
 
-#: packages/docmanager-extension/src/index.tsx:970
+#: packages/docmanager-extension/src/index.tsx:970 packages/docmanager-extension/src/index.tsx:982
 msgid "Save All"
 msgstr "Сохранить всё"
 
-#: packages/docmanager-extension/src/index.tsx:971
+#: packages/docmanager-extension/src/index.tsx:971 packages/docmanager-extension/src/index.tsx:983
 msgid "Save all open documents"
 msgstr "Сохранить все открытые документы"
 
-#: packages/docmanager-extension/src/index.tsx:998
-msgid "Save %1 As…"
-msgstr "Сохранить %1 как…"
+#: packages/docmanager-extension/src/recents.ts:73
+msgid "Clear Recent Documents"
+msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:999
-msgid "Save with new path"
-msgstr "Сохранить по новому пути"
+#: packages/docmanager-extension/src/recents.ts:74
+msgid "Clear the list of recently opened items."
+msgstr ""
 
 #: packages/docmanager/src/dialogs.ts:117
 msgid "Overwrite file?"
 msgstr "Перезаписать файл?"
 
 #: packages/docmanager/src/dialogs.ts:118
 msgid "\"%1\" already exists, overwrite?"
 msgstr "\"%1\" уже существует. Перезаписать?"
 
-#: packages/docmanager/src/dialogs.ts:122 packages/docregistry/src/context.ts:831 packages/docregistry/src/context.ts:867 packages/shortcuts-extension/src/components/ShortcutInput.tsx:495 packages/shortcuts-extension/src/components/ShortcutItem.tsx:231
+#: packages/docmanager/src/dialogs.ts:122 packages/docregistry/src/context.ts:829 packages/docregistry/src/context.ts:831 packages/docregistry/src/context.ts:865 packages/docregistry/src/context.ts:867 packages/shortcuts-extension/src/components/ShortcutInput.tsx:495 packages/shortcuts-extension/src/components/ShortcutInput.tsx:496 packages/shortcuts-extension/src/components/ShortcutItem.tsx:231 packages/shortcuts-extension/src/components/ShortcutItem.tsx:348
 msgid "Overwrite"
 msgstr "Перезаписать"
 
 #: packages/docmanager/src/dialogs.ts:123
 msgid "Overwrite Existing File"
 msgstr "Перезаписать существующий файл"
 
@@ -4623,15 +4741,15 @@
 msgid "New Name"
 msgstr "Новое имя"
 
 #: packages/docmanager/src/dialogs.ts:52 packages/docmanager/src/dialogs.ts:59
 msgid "Rename File"
 msgstr "Переименовать файл"
 
-#: packages/docmanager/src/dialogs.ts:68 packages/filebrowser/src/listing.ts:1891
+#: packages/docmanager/src/dialogs.ts:68 packages/filebrowser/src/listing.ts:1891 packages/filebrowser/src/listing.ts:1912 packages/filebrowser/src/listing.ts:1964
 msgid "Rename Error"
 msgstr "Ошибка переименования"
 
 #: packages/docmanager/src/dialogs.ts:70
 msgid "\"%1\" is not a valid name for a file. Names must have nonzero length, and cannot include \"/\", \"\\\", or \":\""
 msgstr "\"%1\" не является допустимым именем для файла. Имена должны иметь ненулевую длину и не могут включать \"/\", \"\\\" или \":\""
 
@@ -4643,189 +4761,189 @@
 msgid "Saving started"
 msgstr "Сохранение началось"
 
 #: packages/docmanager/src/savingstatus.tsx:60
 msgid "Saving failed"
 msgstr "Ошибка сохранения"
 
-#: packages/docmanager/src/widgetmanager.ts:296
+#: packages/docmanager/src/widgetmanager.ts:296 packages/docmanager/src/widgetmanager.ts:307
 msgid "Name: %1\n"
 "Path: %2\n"
 msgstr "Имя: %1\n"
 "Путь: %2\n"
 
-#: packages/docmanager/src/widgetmanager.ts:302
+#: packages/docmanager/src/widgetmanager.ts:302 packages/docmanager/src/widgetmanager.ts:313
 msgid "Read-only"
 msgstr "Только для чтения"
 
-#: packages/docmanager/src/widgetmanager.ts:305
+#: packages/docmanager/src/widgetmanager.ts:305 packages/docmanager/src/widgetmanager.ts:316
 msgid "Last Saved: %1\n"
 msgstr "Последнее сохранение: %1\n"
 
-#: packages/docmanager/src/widgetmanager.ts:306
+#: packages/docmanager/src/widgetmanager.ts:306 packages/docmanager/src/widgetmanager.ts:317
 msgid "Last Checkpoint: %1"
 msgstr "Последняя контрольная точка: %1"
 
-#: packages/docmanager/src/widgetmanager.ts:397
+#: packages/docmanager/src/widgetmanager.ts:397 packages/docmanager/src/widgetmanager.ts:468
 msgid "Close and save"
 msgstr "Закрыть и сохранить"
 
-#: packages/docmanager/src/widgetmanager.ts:399
+#: packages/docmanager/src/widgetmanager.ts:399 packages/docmanager/src/widgetmanager.ts:470
 msgid "Close and save Document"
 msgstr "Закрыть и сохранить документ"
 
-#: packages/docmanager/src/widgetmanager.ts:400
+#: packages/docmanager/src/widgetmanager.ts:400 packages/docmanager/src/widgetmanager.ts:471
 msgid "Close Document"
 msgstr "Закрыть документ"
 
-#: packages/docmanager/src/widgetmanager.ts:408
+#: packages/docmanager/src/widgetmanager.ts:408 packages/docmanager/src/widgetmanager.ts:479
 msgid "Close without saving"
 msgstr "Закрыть без сохранения"
 
-#: packages/docmanager/src/widgetmanager.ts:409
+#: packages/docmanager/src/widgetmanager.ts:409 packages/docmanager/src/widgetmanager.ts:480
 msgid "Close Document without saving"
 msgstr "Закрыть документ без сохранения"
 
-#: packages/docmanager/src/widgetmanager.ts:415 packages/notebook/src/searchprovider.ts:522
+#: packages/docmanager/src/widgetmanager.ts:415 packages/docmanager/src/widgetmanager.ts:486 packages/notebook/src/searchprovider.ts:511 packages/notebook/src/searchprovider.ts:514 packages/notebook/src/searchprovider.ts:522
 msgid "Confirmation"
 msgstr "Подтверждение"
 
-#: packages/docmanager/src/widgetmanager.ts:416
+#: packages/docmanager/src/widgetmanager.ts:416 packages/docmanager/src/widgetmanager.ts:487
 msgid "Please confirm you want to close \"%1\"."
 msgstr "Пожалуйста, подтвердите, что вы хотите закрыть \"%1\"."
 
-#: packages/docmanager/src/widgetmanager.ts:421
+#: packages/docmanager/src/widgetmanager.ts:421 packages/docmanager/src/widgetmanager.ts:492
 msgid "If checked, no confirmation to close a document will be asked in the future."
 msgstr "Если отмечено, в будущем не будет запрошено подтверждение о закрытии документа."
 
-#: packages/docmanager/src/widgetmanager.ts:443
+#: packages/docmanager/src/widgetmanager.ts:443 packages/docmanager/src/widgetmanager.ts:514
 msgid "Save as"
 msgstr "Сохранить как"
 
-#: packages/docmanager/src/widgetmanager.ts:445
+#: packages/docmanager/src/widgetmanager.ts:445 packages/docmanager/src/widgetmanager.ts:516
 msgid "Save your work"
 msgstr "Сохранить вашу работу"
 
-#: packages/docmanager/src/widgetmanager.ts:446
+#: packages/docmanager/src/widgetmanager.ts:446 packages/docmanager/src/widgetmanager.ts:517
 msgid "Save changes in \"%1\" before closing?"
 msgstr "Сохранить изменения в \"%1\" перед закрытием?"
 
-#: packages/docmanager/src/widgetmanager.ts:450
+#: packages/docmanager/src/widgetmanager.ts:450 packages/docmanager/src/widgetmanager.ts:521
 msgid "Discard"
 msgstr "Отклонить"
 
-#: packages/docmanager/src/widgetmanager.ts:451
+#: packages/docmanager/src/widgetmanager.ts:451 packages/docmanager/src/widgetmanager.ts:522
 msgid "Discard changes to file"
 msgstr "Отменить изменения в файле"
 
 #: packages/docregistry/src/components.tsx:25
 msgid "Document is permissioned read-only; \"save\" is disabled, use \"save as...\" instead"
 msgstr ""
 
 #: packages/docregistry/src/components.tsx:29
 msgid "%1 is read-only"
 msgstr ""
 
-#: packages/docregistry/src/context.ts:1045
+#: packages/docregistry/src/context.ts:1043 packages/docregistry/src/context.ts:1045
 msgid "Save File As…"
 msgstr "Сохранить файл как…"
 
-#: packages/docregistry/src/context.ts:616 packages/docregistry/src/context.ts:916
+#: packages/docregistry/src/context.ts:614 packages/docregistry/src/context.ts:616 packages/docregistry/src/context.ts:914 packages/docregistry/src/context.ts:916
 msgid "File Save Error for %1"
 msgstr "Ошибка сохранения файла для %1"
 
-#: packages/docregistry/src/context.ts:681
+#: packages/docregistry/src/context.ts:679 packages/docregistry/src/context.ts:681
 msgid "File Load Error for %1"
 msgstr "Ошибка загрузки файла для %1"
 
-#: packages/docregistry/src/context.ts:820
+#: packages/docregistry/src/context.ts:818 packages/docregistry/src/context.ts:820
 msgid "\"%1\" has changed on disk since the last time it was opened or saved.\n"
 "Do you want to overwrite the file on disk with the version open here,\n"
 "or load the version on disk (revert)?"
 msgstr "\"%1\" изменился на диске с момента его последнего открытия или сохранения.\n"
 "Вы хотите перезаписать файл на диске версией открытой здесь, \n"
 "или загрузить версию на диске (откат)?"
 
-#: packages/docregistry/src/context.ts:836
+#: packages/docregistry/src/context.ts:834 packages/docregistry/src/context.ts:836
 msgid "File Changed"
 msgstr "Файл изменён"
 
-#: packages/docregistry/src/context.ts:862
+#: packages/docregistry/src/context.ts:860 packages/docregistry/src/context.ts:862
 msgid "\"%1\" already exists. Do you want to replace it?"
 msgstr "«%1» уже существует. Вы хотите заменить его?"
 
-#: packages/docregistry/src/context.ts:871
+#: packages/docregistry/src/context.ts:869 packages/docregistry/src/context.ts:871
 msgid "File Overwrite?"
 msgstr "Перезапись файл?"
 
 #: packages/docregistry/src/mimedocument.ts:175 packages/docregistry/src/mimedocument.ts:71 packages/markdownviewer/src/widget.ts:211
 msgid "Renderer Failure: %1"
 msgstr "Ошибка визуализации: %1"
 
-#: packages/docregistry/src/registry.ts:1287
+#: packages/docregistry/src/registry.ts:1287 packages/docregistry/src/registry.ts:1297
 msgid "default"
 msgstr "по умолчанию"
 
-#: packages/docregistry/src/registry.ts:1310
+#: packages/docregistry/src/registry.ts:1310 packages/docregistry/src/registry.ts:1320
 msgid "Text"
 msgstr "Текст"
 
-#: packages/docregistry/src/registry.ts:1333 packages/launcher/src/widget.tsx:115 packages/launcher/src/widget.tsx:120 packages/notebook-extension/src/index.ts:1243 packages/notebook-extension/src/index.ts:1955 packages/notebook-extension/src/index.ts:1991
+#: packages/docregistry/src/registry.ts:1333 packages/docregistry/src/registry.ts:1343 packages/launcher/src/widget.tsx:115 packages/launcher/src/widget.tsx:120 packages/notebook-extension/src/index.ts:1243 packages/notebook-extension/src/index.ts:1247 packages/notebook-extension/src/index.ts:1255 packages/notebook-extension/src/index.ts:1955 packages/notebook-extension/src/index.ts:1960 packages/notebook-extension/src/index.ts:1971 packages/notebook-extension/src/index.ts:1991 packages/notebook-extension/src/index.ts:1998 packages/notebook-extension/src/index.ts:2009
 msgid "Notebook"
 msgstr "Блокнот"
 
-#: packages/docregistry/src/registry.ts:1358
+#: packages/docregistry/src/registry.ts:1358 packages/docregistry/src/registry.ts:1368
 msgid "Directory"
 msgstr "Каталог"
 
-#: packages/docregistry/src/registry.ts:1385 packages/fileeditor-extension/src/commands.ts:817
+#: packages/docregistry/src/registry.ts:1385 packages/docregistry/src/registry.ts:1395 packages/fileeditor-extension/src/commands.ts:817 packages/fileeditor-extension/src/commands.ts:818
 msgid "Markdown File"
 msgstr "Файл Markdown"
 
-#: packages/docregistry/src/registry.ts:1392
+#: packages/docregistry/src/registry.ts:1392 packages/docregistry/src/registry.ts:1402
 msgid "PDF File"
 msgstr "PDF файл"
 
-#: packages/docregistry/src/registry.ts:1399 packages/fileeditor-extension/src/index.ts:331
+#: packages/docregistry/src/registry.ts:1399 packages/docregistry/src/registry.ts:1409 packages/fileeditor-extension/src/index.ts:331
 msgid "Python File"
 msgstr "Файл Python"
 
-#: packages/docregistry/src/registry.ts:1406
+#: packages/docregistry/src/registry.ts:1406 packages/docregistry/src/registry.ts:1416
 msgid "JSON File"
 msgstr "Файл JSON"
 
-#: packages/docregistry/src/registry.ts:1413
+#: packages/docregistry/src/registry.ts:1413 packages/docregistry/src/registry.ts:1423
 msgid "JSONLines File"
 msgstr ""
 
-#: packages/docregistry/src/registry.ts:1424 packages/fileeditor-extension/src/index.ts:343
+#: packages/docregistry/src/registry.ts:1424 packages/docregistry/src/registry.ts:1434 packages/fileeditor-extension/src/index.ts:343
 msgid "Julia File"
 msgstr "Файл Julia"
 
-#: packages/docregistry/src/registry.ts:1431
+#: packages/docregistry/src/registry.ts:1431 packages/docregistry/src/registry.ts:1441
 msgid "CSV File"
 msgstr "Файл CSV"
 
-#: packages/docregistry/src/registry.ts:1438
+#: packages/docregistry/src/registry.ts:1438 packages/docregistry/src/registry.ts:1448
 msgid "TSV File"
 msgstr "Файл TSV"
 
-#: packages/docregistry/src/registry.ts:1445 packages/fileeditor-extension/src/index.ts:355
+#: packages/docregistry/src/registry.ts:1445 packages/docregistry/src/registry.ts:1455 packages/fileeditor-extension/src/index.ts:355
 msgid "R File"
 msgstr "Файл R"
 
-#: packages/docregistry/src/registry.ts:1452
+#: packages/docregistry/src/registry.ts:1452 packages/docregistry/src/registry.ts:1462
 msgid "YAML File"
 msgstr "Файл YAML"
 
-#: packages/docregistry/src/registry.ts:1459 packages/docregistry/src/registry.ts:1467 packages/docregistry/src/registry.ts:1475 packages/docregistry/src/registry.ts:1483 packages/docregistry/src/registry.ts:1491 packages/docregistry/src/registry.ts:1499 packages/docregistry/src/registry.ts:1507 packages/imageviewer-extension/src/index.ts:119
+#: packages/docregistry/src/registry.ts:1459 packages/docregistry/src/registry.ts:1467 packages/docregistry/src/registry.ts:1469 packages/docregistry/src/registry.ts:1475 packages/docregistry/src/registry.ts:1477 packages/docregistry/src/registry.ts:1483 packages/docregistry/src/registry.ts:1485 packages/docregistry/src/registry.ts:1491 packages/docregistry/src/registry.ts:1493 packages/docregistry/src/registry.ts:1499 packages/docregistry/src/registry.ts:1501 packages/docregistry/src/registry.ts:1507 packages/docregistry/src/registry.ts:1509 packages/docregistry/src/registry.ts:1517 packages/imageviewer-extension/src/index.ts:119
 msgid "Image"
 msgstr "Изображение"
 
-#: packages/documentsearch-extension/src/index.ts:326 packages/fileeditor-extension/src/commands.ts:526 packages/json-extension/src/component.tsx:78
+#: packages/documentsearch-extension/src/index.ts:326 packages/fileeditor-extension/src/commands.ts:526 packages/fileeditor-extension/src/commands.ts:527 packages/json-extension/src/component.tsx:78
 msgid "Find…"
 msgstr "Найти…"
 
 #: packages/documentsearch-extension/src/index.ts:363
 msgid "Find and Replace…"
 msgstr "Найти и заменить…"
 
@@ -4865,30 +4983,42 @@
 msgid "Replace All"
 msgstr "Заменить все"
 
 #: packages/documentsearch/src/searchview.tsx:313
 msgid "Previous Match"
 msgstr "Предыдущее соответствие"
 
-#: packages/documentsearch/src/searchview.tsx:324
+#: packages/documentsearch/src/searchview.tsx:324 packages/documentsearch/src/searchview.tsx:328
 msgid "Next Match"
 msgstr "Следующее совпадение"
 
-#: packages/documentsearch/src/searchview.tsx:374
+#: packages/documentsearch/src/searchview.tsx:374 packages/documentsearch/src/searchview.tsx:385
 msgid "Hide Search Filters"
 msgstr "Скрыть поисковые фильтры"
 
-#: packages/documentsearch/src/searchview.tsx:375
+#: packages/documentsearch/src/searchview.tsx:375 packages/documentsearch/src/searchview.tsx:386
 msgid "Show Search Filters"
 msgstr "Показать фильтры поиска"
 
 #: packages/documentsearch/src/searchview.tsx:685
 msgid "Toggle Replace"
 msgstr "Переключить замену"
 
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
 msgstr "Менеджер расширений"
 
 #: packages/extensionmanager-extension/src/index.ts:141
 msgid "Enable Extension Manager"
 msgstr "Включить Менеджер расширений"
@@ -5077,372 +5207,376 @@
 msgid "Version: %1"
 msgstr "Версия: %1"
 
 #: packages/extensionmanager/src/widget.tsx:97
 msgid "%1 extension is not allowed anymore. Please uninstall it immediately or contact your administrator."
 msgstr "Расширение %1 больше не разрешено. Немедленно удалите его или обратитесь к администратору."
 
-#: packages/filebrowser-extension/src/index.ts:1021
-msgid "Open from Path…"
-msgstr "Открыть из пути…"
-
-#: packages/filebrowser-extension/src/index.ts:1021 packages/filebrowser-extension/src/index.ts:1023 packages/filebrowser-extension/src/index.ts:844 packages/filebrowser-extension/src/index.ts:846
+#: packages/filebrowser-extension/src/index.ts:1021 packages/filebrowser-extension/src/index.ts:1023 packages/filebrowser-extension/src/index.ts:1029 packages/filebrowser-extension/src/index.ts:1031 packages/filebrowser-extension/src/index.ts:844 packages/filebrowser-extension/src/index.ts:846 packages/filebrowser-extension/src/index.ts:852 packages/filebrowser-extension/src/index.ts:854
 msgid "Open %1"
 msgstr "Открыть %1"
 
-#: packages/filebrowser-extension/src/index.ts:1023
+#: packages/filebrowser-extension/src/index.ts:1021 packages/filebrowser-extension/src/index.ts:1029
+msgid "Open from Path…"
+msgstr "Открыть из пути…"
+
+#: packages/filebrowser-extension/src/index.ts:1023 packages/filebrowser-extension/src/index.ts:1031
 msgid "Open from path"
 msgstr "Открыть из пути"
 
-#: packages/filebrowser-extension/src/index.ts:1032
+#: packages/filebrowser-extension/src/index.ts:1032 packages/filebrowser-extension/src/index.ts:1040
 msgid "Path"
 msgstr "Путь"
 
-#: packages/filebrowser-extension/src/index.ts:1034
+#: packages/filebrowser-extension/src/index.ts:1034 packages/filebrowser-extension/src/index.ts:1042
 msgid "Open Path"
 msgstr "Открыть путь"
 
-#: packages/filebrowser-extension/src/index.ts:1035 packages/filebrowser-extension/src/index.ts:1124 packages/filebrowser-extension/src/index.ts:856
+#: packages/filebrowser-extension/src/index.ts:1035 packages/filebrowser-extension/src/index.ts:1043 packages/filebrowser-extension/src/index.ts:1124 packages/filebrowser-extension/src/index.ts:1132 packages/filebrowser-extension/src/index.ts:856 packages/filebrowser-extension/src/index.ts:864
 msgid "Open"
 msgstr "Открыть"
 
-#: packages/filebrowser-extension/src/index.ts:1070
+#: packages/filebrowser-extension/src/index.ts:1070 packages/filebrowser-extension/src/index.ts:1078
 msgid "Could not find path: %1"
 msgstr "Не удалось найти путь: %1"
 
-#: packages/filebrowser-extension/src/index.ts:1072
+#: packages/filebrowser-extension/src/index.ts:1072 packages/filebrowser-extension/src/index.ts:1080
 msgid "Cannot open"
 msgstr "Невозможно открыть"
 
-#: packages/filebrowser-extension/src/index.ts:1137 packages/fileeditor-extension/src/commands.ts:981 packages/terminal-extension/src/index.ts:494
+#: packages/filebrowser-extension/src/index.ts:1137 packages/filebrowser-extension/src/index.ts:1145 packages/fileeditor-extension/src/commands.ts:979 packages/fileeditor-extension/src/commands.ts:980 packages/fileeditor-extension/src/commands.ts:981 packages/terminal-extension/src/index.ts:494
 msgid "Paste"
 msgstr "Вставить"
 
-#: packages/filebrowser-extension/src/index.ts:1150 packages/filebrowser/src/opendialog.ts:172
+#: packages/filebrowser-extension/src/index.ts:1150 packages/filebrowser-extension/src/index.ts:1158 packages/filebrowser/src/opendialog.ts:172 packages/filebrowser/src/opendialog.ts:184
 msgid "New Folder"
 msgstr "Новая папка"
 
-#: packages/filebrowser-extension/src/index.ts:1162
+#: packages/filebrowser-extension/src/index.ts:1162 packages/filebrowser-extension/src/index.ts:1170
 msgid "New File"
 msgstr "Новый файл"
 
-#: packages/filebrowser-extension/src/index.ts:1174 packages/fileeditor-extension/src/commands.ts:816
+#: packages/filebrowser-extension/src/index.ts:1174 packages/filebrowser-extension/src/index.ts:1182 packages/fileeditor-extension/src/commands.ts:816 packages/fileeditor-extension/src/commands.ts:817
 msgid "New Markdown File"
 msgstr "Новый файл Markdown"
 
-#: packages/filebrowser-extension/src/index.ts:1186
+#: packages/filebrowser-extension/src/index.ts:1186 packages/filebrowser-extension/src/index.ts:1194
 msgid "Refresh the file browser."
 msgstr "Обновить файловый менеджер."
 
-#: packages/filebrowser-extension/src/index.ts:1187 packages/filebrowser/src/opendialog.ts:187
+#: packages/filebrowser-extension/src/index.ts:1187 packages/filebrowser-extension/src/index.ts:1195 packages/filebrowser/src/opendialog.ts:187 packages/filebrowser/src/opendialog.ts:199
 msgid "Refresh File List"
 msgstr "Обновить список файлов"
 
-#: packages/filebrowser-extension/src/index.ts:1235
+#: packages/filebrowser-extension/src/index.ts:1235 packages/filebrowser-extension/src/index.ts:1243
 msgid "Copy Path"
 msgstr "Скопировать путь"
 
-#: packages/filebrowser-extension/src/index.ts:1247 packages/mainmenu-extension/src/index.ts:531 packages/notebook-extension/src/index.ts:2389 packages/running-extension/src/kernels.ts:118 packages/running-extension/src/kernels.ts:66
+#: packages/filebrowser-extension/src/index.ts:1247 packages/filebrowser-extension/src/index.ts:1255 packages/mainmenu-extension/src/index.ts:529 packages/mainmenu-extension/src/index.ts:531 packages/notebook-extension/src/index.ts:2389 packages/notebook-extension/src/index.ts:2396 packages/notebook-extension/src/index.ts:2407 packages/running-extension/src/kernels.ts:118 packages/running-extension/src/kernels.ts:66 packages/running-extension/src/kernels.tsx:139 packages/running-extension/src/kernels.tsx:86
 msgid "Shut Down Kernel"
 msgstr "Завершить работу ядра"
 
-#: packages/filebrowser-extension/src/index.ts:1251
+#: packages/filebrowser-extension/src/index.ts:1251 packages/filebrowser-extension/src/index.ts:1259
 msgid "Show Last Modified Column"
 msgstr "Показывать последнее изменение"
 
-#: packages/filebrowser-extension/src/index.ts:1267
+#: packages/filebrowser-extension/src/index.ts:1267 packages/filebrowser-extension/src/index.ts:1275
 msgid "Show Full Path"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:1283
+#: packages/filebrowser-extension/src/index.ts:1283 packages/filebrowser-extension/src/index.ts:1291
 msgid "Sort Notebooks Above Files"
 msgstr "Сортировать блокноты над файлами"
 
-#: packages/filebrowser-extension/src/index.ts:1299
+#: packages/filebrowser-extension/src/index.ts:1299 packages/filebrowser-extension/src/index.ts:1307
 msgid "Show File Size Column"
 msgstr "Показать столбец размера файла"
 
-#: packages/filebrowser-extension/src/index.ts:1315
+#: packages/filebrowser-extension/src/index.ts:1315 packages/filebrowser-extension/src/index.ts:1323
 msgid "Show Hidden Files"
 msgstr "Показывать скрытые файлы"
 
-#: packages/filebrowser-extension/src/index.ts:1332
+#: packages/filebrowser-extension/src/index.ts:1332 packages/filebrowser-extension/src/index.ts:1340
 msgid "Show File Checkboxes"
 msgstr "Показать флажки для файлов"
 
-#: packages/filebrowser-extension/src/index.ts:1348
+#: packages/filebrowser-extension/src/index.ts:1348 packages/filebrowser-extension/src/index.ts:1356
 msgid "Search on File Names"
 msgstr "Поиск по именам файлов"
 
-#: packages/filebrowser-extension/src/index.ts:1417
+#: packages/filebrowser-extension/src/index.ts:1417 packages/filebrowser-extension/src/index.ts:1425
 msgid "No browser for path"
 msgstr "Нет браузера для пути"
 
-#: packages/filebrowser-extension/src/index.ts:396
-msgid "Copy Download Link"
-msgstr "Скопировать ссылку на скачивание"
-
-#: packages/filebrowser-extension/src/index.ts:439
+#: packages/filebrowser-extension/src/index.ts:340 packages/filebrowser-extension/src/index.ts:439
 msgid "File Browser Section"
 msgstr "Секция файлового менеджера"
 
-#: packages/filebrowser-extension/src/index.ts:450
+#: packages/filebrowser-extension/src/index.ts:342 packages/filebrowser-extension/src/index.ts:354 packages/filebrowser-extension/src/index.ts:452 packages/filebrowser-extension/src/index.ts:504 packages/filebrowser-extension/src/index.ts:512 packages/filebrowser/src/browser.ts:73 packages/filebrowser/src/browser.ts:74
+msgid "File Browser"
+msgstr "Файловый менеджер"
+
+#: packages/filebrowser-extension/src/index.ts:352 packages/filebrowser-extension/src/index.ts:450
 msgid "File Browser (%1)"
 msgstr "Файловый менеджер (%1)"
 
-#: packages/filebrowser-extension/src/index.ts:452 packages/filebrowser-extension/src/index.ts:504 packages/filebrowser/src/browser.ts:73
-msgid "File Browser"
-msgstr "Файловый менеджер"
+#: packages/filebrowser-extension/src/index.ts:396 packages/filebrowser-extension/src/index.ts:427
+msgid "Copy Download Link"
+msgstr "Скопировать ссылку на скачивание"
 
-#: packages/filebrowser-extension/src/index.ts:482
+#: packages/filebrowser-extension/src/index.ts:482 packages/filebrowser-extension/src/index.ts:490
 msgid "Filter files by name"
 msgstr "Фильтровать файлы по имени"
 
-#: packages/filebrowser-extension/src/index.ts:515
+#: packages/filebrowser-extension/src/index.ts:515 packages/filebrowser-extension/src/index.ts:523
 msgid "Open the file browser for the provided `path`."
 msgstr "Откройте файловый браузер для пути `path`."
 
-#: packages/filebrowser-extension/src/index.ts:547
+#: packages/filebrowser-extension/src/index.ts:547 packages/filebrowser-extension/src/index.ts:555
 msgid "Hide the file browser."
 msgstr "Скрыть файловый браузер."
 
-#: packages/filebrowser-extension/src/index.ts:557
+#: packages/filebrowser-extension/src/index.ts:557 packages/filebrowser-extension/src/index.ts:565
 msgid "Show Active File in File Browser"
 msgstr "Показать активный файл в менеджере файлов"
 
-#: packages/filebrowser-extension/src/index.ts:654
+#: packages/filebrowser-extension/src/index.ts:654 packages/filebrowser-extension/src/index.ts:662
 msgid "Copy Shareable Link"
 msgstr "Копировать ссылку общего доступа"
 
-#: packages/filebrowser-extension/src/index.ts:778
+#: packages/filebrowser-extension/src/index.ts:778 packages/filebrowser-extension/src/index.ts:786
 msgid "Open in Simple Mode"
 msgstr "Открыть в простом режиме"
 
-#: packages/filebrowser-extension/src/index.ts:844
+#: packages/filebrowser-extension/src/index.ts:844 packages/filebrowser-extension/src/index.ts:852
 msgid "Open from URL…"
 msgstr "Открыть из URL…"
 
-#: packages/filebrowser-extension/src/index.ts:846
+#: packages/filebrowser-extension/src/index.ts:846 packages/filebrowser-extension/src/index.ts:854
 msgid "Open from URL"
 msgstr "Открыть из URL"
 
-#: packages/filebrowser-extension/src/index.ts:853
+#: packages/filebrowser-extension/src/index.ts:853 packages/filebrowser-extension/src/index.ts:861
 msgid "URL"
 msgstr "URL"
 
-#: packages/filebrowser-extension/src/index.ts:855
+#: packages/filebrowser-extension/src/index.ts:855 packages/filebrowser-extension/src/index.ts:863
 msgid "Open URL"
 msgstr "Открыть URL"
 
-#: packages/filebrowser-extension/src/index.ts:874
+#: packages/filebrowser-extension/src/index.ts:874 packages/filebrowser-extension/src/index.ts:882
 msgid "Could not open URL: %1"
 msgstr "Не удалось открыть файл URL: %1"
 
-#: packages/filebrowser-extension/src/index.ts:876
+#: packages/filebrowser-extension/src/index.ts:876 packages/filebrowser-extension/src/index.ts:884
 msgid "Cannot fetch"
 msgstr "Не удается получить"
 
-#: packages/filebrowser-extension/src/index.ts:889 packages/filebrowser/src/upload.ts:52
+#: packages/filebrowser-extension/src/index.ts:889 packages/filebrowser-extension/src/index.ts:897 packages/filebrowser/src/upload.ts:52
 msgctxt "showErrorMessage"
 msgid "Upload Error"
 msgstr "Ошибка загрузки"
 
-#: packages/filebrowser-extension/src/index.ts:942 packages/fileeditor-extension/src/commands.ts:954 packages/terminal-extension/src/index.ts:469
+#: packages/filebrowser-extension/src/index.ts:942 packages/filebrowser-extension/src/index.ts:950 packages/fileeditor-extension/src/commands.ts:952 packages/fileeditor-extension/src/commands.ts:953 packages/fileeditor-extension/src/commands.ts:954 packages/terminal-extension/src/index.ts:469
 msgid "Copy"
 msgstr "Копировать"
 
-#: packages/filebrowser-extension/src/index.ts:955 packages/fileeditor-extension/src/commands.ts:920
+#: packages/filebrowser-extension/src/index.ts:955 packages/filebrowser-extension/src/index.ts:963 packages/fileeditor-extension/src/commands.ts:918 packages/fileeditor-extension/src/commands.ts:919 packages/fileeditor-extension/src/commands.ts:920
 msgid "Cut"
 msgstr "Вырезать"
 
-#: packages/filebrowser-extension/src/index.ts:967
+#: packages/filebrowser-extension/src/index.ts:967 packages/filebrowser-extension/src/index.ts:975
 msgid "Duplicate"
 msgstr "Дублировать"
 
-#: packages/filebrowser-extension/src/index.ts:971
+#: packages/filebrowser-extension/src/index.ts:971 packages/filebrowser-extension/src/index.ts:979
 msgid "Update the file browser to display the provided `path`."
 msgstr "Обновите файловый браузер, чтобы отобразить указанный путь `path`."
 
-#: packages/filebrowser/src/browser.ts:397
+#: packages/filebrowser/src/browser.ts:397 packages/filebrowser/src/browser.ts:403
 msgid "Directory not found"
 msgstr "Каталог не найден"
 
-#: packages/filebrowser/src/browser.ts:398 packages/filebrowser/src/model.ts:298
+#: packages/filebrowser/src/browser.ts:398 packages/filebrowser/src/browser.ts:404 packages/filebrowser/src/model.ts:291 packages/filebrowser/src/model.ts:298
 msgid "Directory not found: \"%1\""
 msgstr "Каталог не найден: \"%1\""
 
-#: packages/filebrowser/src/browser.ts:67
+#: packages/filebrowser/src/browser.ts:67 packages/filebrowser/src/browser.ts:68
 msgid "file browser"
 msgstr "файловый менеджер"
 
 #: packages/filebrowser/src/crumbs.ts:192 packages/filebrowser/src/crumbs.ts:219
 msgid "Open Error"
 msgstr "Ошибка открытия файла"
 
 #: packages/filebrowser/src/crumbs.ts:327
 msgid "Move Error"
 msgstr "Ошибка перемещения"
 
-#: packages/filebrowser/src/listing.ts:1136
+#: packages/filebrowser/src/listing.ts:1136 packages/filebrowser/src/listing.ts:1157 packages/filebrowser/src/listing.ts:1209
 msgctxt "showErrorMessage"
 msgid "Open directory"
 msgstr "Открыть каталог"
 
-#: packages/filebrowser/src/listing.ts:1411
+#: packages/filebrowser/src/listing.ts:1411 packages/filebrowser/src/listing.ts:1432 packages/filebrowser/src/listing.ts:1484
 msgid "Error Uploading Folder"
 msgstr "Ошибка при загрузке папки"
 
-#: packages/filebrowser/src/listing.ts:1412
+#: packages/filebrowser/src/listing.ts:1412 packages/filebrowser/src/listing.ts:1433 packages/filebrowser/src/listing.ts:1485
 msgid "Drag and Drop is currently not supported for folders"
 msgstr "Drag and Drop в настоящее время не поддерживается для папок"
 
-#: packages/filebrowser/src/listing.ts:1531
+#: packages/filebrowser/src/listing.ts:1531 packages/filebrowser/src/listing.ts:1552 packages/filebrowser/src/listing.ts:1604
 msgctxt "showErrorMessage"
 msgid "Error while copying/moving files"
 msgstr "Ошибка копирования/перемещения файлов"
 
-#: packages/filebrowser/src/listing.ts:1830
+#: packages/filebrowser/src/listing.ts:1830 packages/filebrowser/src/listing.ts:1851 packages/filebrowser/src/listing.ts:1903
 msgctxt "showErrorMessage"
 msgid "Delete Failed"
 msgstr "Ошибка удаления"
 
-#: packages/filebrowser/src/listing.ts:1893
+#: packages/filebrowser/src/listing.ts:1893 packages/filebrowser/src/listing.ts:1914 packages/filebrowser/src/listing.ts:1966
 msgctxt "showErrorMessage"
 msgid "\"%1\" is not a valid name for a file. Names must have nonzero length, and cannot include \"/\", \"\\\", or \":\""
 msgstr "\"%1\" не является допустимым именем для файла. Имена должны иметь ненулевую длину и не могут включать \"/\", \"\\\" или \":\""
 
-#: packages/filebrowser/src/listing.ts:1912
+#: packages/filebrowser/src/listing.ts:1912 packages/filebrowser/src/listing.ts:1933 packages/filebrowser/src/listing.ts:1985
 msgctxt "showErrorMessage"
 msgid "Rename Error"
 msgstr "Ошибка переименования"
 
-#: packages/filebrowser/src/listing.ts:2279
+#: packages/filebrowser/src/listing.ts:2279 packages/filebrowser/src/listing.ts:2300 packages/filebrowser/src/listing.ts:2375
 msgid "Last Modified"
 msgstr "Последнее изменение"
 
-#: packages/filebrowser/src/listing.ts:2280
+#: packages/filebrowser/src/listing.ts:2280 packages/filebrowser/src/listing.ts:2301 packages/filebrowser/src/listing.ts:2377
 msgid "File Size"
 msgstr "Размер файла"
 
-#: packages/filebrowser/src/listing.ts:2568
+#: packages/filebrowser/src/listing.ts:2374 packages/settingeditor/src/pluginlist.tsx:461
+msgid "Modified"
+msgstr "Изменён"
+
+#: packages/filebrowser/src/listing.ts:2568 packages/filebrowser/src/listing.ts:2589 packages/filebrowser/src/listing.ts:2696
 msgid "Name: %1"
 msgstr "Имя: %1"
 
-#: packages/filebrowser/src/listing.ts:2574
+#: packages/filebrowser/src/listing.ts:2574 packages/filebrowser/src/listing.ts:2595 packages/filebrowser/src/listing.ts:2702
 msgid "\n"
 "Size: %1"
 msgstr "\n"
 "Размер: %1"
 
-#: packages/filebrowser/src/listing.ts:2584
+#: packages/filebrowser/src/listing.ts:2584 packages/filebrowser/src/listing.ts:2605 packages/filebrowser/src/listing.ts:2712
 msgid "\n"
 "Path: %1"
 msgstr "\n"
 "Путь: %1"
 
-#: packages/filebrowser/src/listing.ts:2591
+#: packages/filebrowser/src/listing.ts:2591 packages/filebrowser/src/listing.ts:2612 packages/filebrowser/src/listing.ts:2719
 msgid "\n"
 "Created: %1"
 msgstr "\n"
 "Создано: %1"
 
-#: packages/filebrowser/src/listing.ts:2597
+#: packages/filebrowser/src/listing.ts:2597 packages/filebrowser/src/listing.ts:2618 packages/filebrowser/src/listing.ts:2725
 msgid "\n"
 "Modified: %1"
 msgstr "\n"
 "Изменено: %1"
 
-#: packages/filebrowser/src/listing.ts:2602
+#: packages/filebrowser/src/listing.ts:2602 packages/filebrowser/src/listing.ts:2623 packages/filebrowser/src/listing.ts:2730
 msgid "\n"
 "Writable: %1"
 msgstr "\n"
 "Доступно для записи: %1"
 
-#: packages/filebrowser/src/listing.ts:2627
+#: packages/filebrowser/src/listing.ts:2627 packages/filebrowser/src/listing.ts:2648 packages/filebrowser/src/listing.ts:2755
 msgid "Deselect directory \"%1\""
 msgstr "Отменить выбор директории \"%1\""
 
-#: packages/filebrowser/src/listing.ts:2628
+#: packages/filebrowser/src/listing.ts:2628 packages/filebrowser/src/listing.ts:2649 packages/filebrowser/src/listing.ts:2756
 msgid "Select directory \"%1\""
 msgstr "Выберите директорию \"%1\""
 
-#: packages/filebrowser/src/listing.ts:2631
+#: packages/filebrowser/src/listing.ts:2631 packages/filebrowser/src/listing.ts:2652 packages/filebrowser/src/listing.ts:2759
 msgid "Deselect file \"%1\""
 msgstr "Отменить выбор файла \"%1\""
 
-#: packages/filebrowser/src/listing.ts:2632
+#: packages/filebrowser/src/listing.ts:2632 packages/filebrowser/src/listing.ts:2653 packages/filebrowser/src/listing.ts:2760
 msgid "Select file \"%1\""
 msgstr "Выберите файл \"%1\""
 
-#: packages/filebrowser/src/listing.ts:2706
+#: packages/filebrowser/src/listing.ts:2706 packages/filebrowser/src/listing.ts:2727 packages/filebrowser/src/listing.ts:2833
 msgid "%1 Item"
 msgid_plural "%1 Items"
 msgstr[0] "%1 элемент"
 msgstr[1] "%1 элемента"
 msgstr[2] "%1 элементов"
 msgstr[3] "%1 элементов"
 
-#: packages/filebrowser/src/listing.ts:400
+#: packages/filebrowser/src/listing.ts:400 packages/filebrowser/src/listing.ts:403
 msgctxt "showErrorMessage"
 msgid "Paste Error"
 msgstr "Ошибка вставки"
 
-#: packages/filebrowser/src/listing.ts:420
+#: packages/filebrowser/src/listing.ts:420 packages/filebrowser/src/listing.ts:423
 msgid "Are you sure you want to permanently delete: %1?"
 msgstr "Вы действительно хотите удалить «%1» навсегда?"
 
-#: packages/filebrowser/src/listing.ts:424
+#: packages/filebrowser/src/listing.ts:424 packages/filebrowser/src/listing.ts:427
 msgid "Are you sure you want to permanently delete the %1 selected item?"
 msgid_plural "Are you sure you want to permanently delete the %1 selected items?"
 msgstr[0] "Вы уверены, что хотите навсегда удалить %1 выбранный элемент?"
 msgstr[1] "Вы уверены, что хотите навсегда удалить %1 выбранных элемента?"
 msgstr[2] "Вы уверены, что хотите навсегда удалить %1 выбранных элементов?"
 msgstr[3] "Вы уверены, что хотите навсегда удалить %1 выбранных элементов?"
 
-#: packages/filebrowser/src/listing.ts:476
+#: packages/filebrowser/src/listing.ts:476 packages/filebrowser/src/listing.ts:479
 msgctxt "showErrorMessage"
 msgid "Duplicate file"
 msgstr "Дублировать файл"
 
-#: packages/filebrowser/src/listing.ts:516
+#: packages/filebrowser/src/listing.ts:516 packages/filebrowser/src/listing.ts:519
 msgctxt "showErrorMessage"
 msgid "Shut down kernel"
 msgstr "Завершить работу ядра"
 
-#: packages/filebrowser/src/listing.ts:856
+#: packages/filebrowser/src/listing.ts:856 packages/filebrowser/src/listing.ts:877 packages/filebrowser/src/listing.ts:974
 msgid "Deselect all files and directories"
 msgstr "Отменить выбор всех файлов и каталогов"
 
-#: packages/filebrowser/src/listing.ts:857
+#: packages/filebrowser/src/listing.ts:857 packages/filebrowser/src/listing.ts:878 packages/filebrowser/src/listing.ts:975
 msgid "Select all files and directories"
 msgstr "Выбрать все файлы и каталоги"
 
-#: packages/filebrowser/src/listing.ts:910
+#: packages/filebrowser/src/listing.ts:899 packages/filebrowser/src/listing.ts:910 packages/filebrowser/src/listing.ts:931
 msgid "unknown"
 msgstr "неизвестный"
 
-#: packages/filebrowser/src/listing.ts:912
+#: packages/filebrowser/src/listing.ts:901 packages/filebrowser/src/listing.ts:912 packages/filebrowser/src/listing.ts:933
 msgid "%1\n"
 "Kernel: %2"
 msgstr "%1\n"
 "Ядро: %2"
 
-#: packages/filebrowser/src/model.ts:414
+#: packages/filebrowser/src/model.ts:407 packages/filebrowser/src/model.ts:414
 msgid "Cannot upload file (>%1 MB). %2"
 msgstr "Не удается загрузить файл (>%1 MB). %2"
 
-#: packages/filebrowser/src/model.ts:443
+#: packages/filebrowser/src/model.ts:436 packages/filebrowser/src/model.ts:443
 msgid "Large file size warning"
 msgstr "Предупреждение о большом размере файла"
 
-#: packages/filebrowser/src/model.ts:444
+#: packages/filebrowser/src/model.ts:437 packages/filebrowser/src/model.ts:444
 msgid "The file size is %1 MB. Do you still want to upload it?"
 msgstr "Размер файла %1 МБ. Вы уверены, что хотите загрузить его?"
 
-#: packages/filebrowser/src/model.ts:450
+#: packages/filebrowser/src/model.ts:443 packages/filebrowser/src/model.ts:450
 msgid "Upload"
 msgstr "Загрузить"
 
 #: packages/filebrowser/src/model.ts:83
 msgid "Files still uploading"
 msgstr "Файлы всё ещё загружаются"
 
@@ -5454,140 +5588,132 @@
 msgid "Uploading…"
 msgstr "Загрузка…"
 
 #: packages/filebrowser/src/uploadstatus.tsx:96
 msgid "Complete!"
 msgstr "Готово!"
 
-#: packages/fileeditor-extension/src/commands.ts:1107 packages/fileeditor-extension/src/commands.ts:1121 packages/fileeditor-extension/src/commands.ts:1137 packages/launcher/src/widget.tsx:117 packages/launcher/src/widget.tsx:127 packages/launcher/src/widget.tsx:296 packages/terminal-extension/src/index.ts:271
+#: packages/fileeditor-extension/src/commands.ts:1105 packages/fileeditor-extension/src/commands.ts:1107 packages/fileeditor-extension/src/commands.ts:1119 packages/fileeditor-extension/src/commands.ts:1121 packages/fileeditor-extension/src/commands.ts:1135 packages/fileeditor-extension/src/commands.ts:1136 packages/fileeditor-extension/src/commands.ts:1137 packages/fileeditor-extension/src/commands.ts:1150 packages/fileeditor-extension/src/commands.ts:1166 packages/launcher/src/widget.tsx:117 packages/launcher/src/widget.tsx:127 packages/launcher/src/widget.tsx:296 packages/terminal-extension/src/index.ts:271
 msgid "Other"
 msgstr "Другое"
 
-#: packages/fileeditor-extension/src/commands.ts:1167 packages/fileeditor-extension/src/commands.ts:1189 packages/fileeditor-extension/src/commands.ts:1204 packages/fileeditor-extension/src/commands.ts:1219 packages/fileeditor-extension/src/commands.ts:1237
+#: packages/fileeditor-extension/src/commands.ts:1165 packages/fileeditor-extension/src/commands.ts:1167 packages/fileeditor-extension/src/commands.ts:1187 packages/fileeditor-extension/src/commands.ts:1189 packages/fileeditor-extension/src/commands.ts:1196 packages/fileeditor-extension/src/commands.ts:1202 packages/fileeditor-extension/src/commands.ts:1204 packages/fileeditor-extension/src/commands.ts:1217 packages/fileeditor-extension/src/commands.ts:1218 packages/fileeditor-extension/src/commands.ts:1219 packages/fileeditor-extension/src/commands.ts:1233 packages/fileeditor-extension/src/commands.ts:1235 packages/fileeditor-extension/src/commands.ts:1237 packages/fileeditor-extension/src/commands.ts:1248 packages/fileeditor-extension/src/commands.ts:1266
 msgid "Text Editor"
 msgstr "Текстовый редактор"
 
-#: packages/fileeditor-extension/src/commands.ts:1367
+#: packages/fileeditor-extension/src/commands.ts:1365 packages/fileeditor-extension/src/commands.ts:1367 packages/fileeditor-extension/src/commands.ts:1396
 msgid "Code Viewer"
 msgstr "Просмотр кода"
 
-#: packages/fileeditor-extension/src/commands.ts:1386
+#: packages/fileeditor-extension/src/commands.ts:1384 packages/fileeditor-extension/src/commands.ts:1386 packages/fileeditor-extension/src/commands.ts:1415
 msgid "Open Code Viewer"
 msgstr "Открыть просмотр кода"
 
-#: packages/fileeditor-extension/src/commands.ts:280
+#: packages/fileeditor-extension/src/commands.ts:280 packages/fileeditor-extension/src/commands.ts:281
 msgid "Increase Text Editor Font Size"
 msgstr "Увеличить размер шрифта текстового редактора"
 
-#: packages/fileeditor-extension/src/commands.ts:284
+#: packages/fileeditor-extension/src/commands.ts:284 packages/fileeditor-extension/src/commands.ts:285
 msgid "Decrease Text Editor Font Size"
 msgstr "Уменьшить размер шрифта текстового редактора"
 
-#: packages/fileeditor-extension/src/commands.ts:307 packages/fileeditor-extension/src/commands.ts:311 packages/mainmenu-extension/src/index.ts:576 packages/notebook-extension/src/index.ts:3040
+#: packages/fileeditor-extension/src/commands.ts:307 packages/fileeditor-extension/src/commands.ts:308 packages/fileeditor-extension/src/commands.ts:311 packages/fileeditor-extension/src/commands.ts:312 packages/mainmenu-extension/src/index.ts:573 packages/mainmenu-extension/src/index.ts:576 packages/notebook-extension/src/index.ts:3040 packages/notebook-extension/src/index.ts:3047 packages/notebook-extension/src/index.ts:3070
 msgid "Show Line Numbers"
 msgstr "Показывать номера строк"
 
-#: packages/fileeditor-extension/src/commands.ts:312
+#: packages/fileeditor-extension/src/commands.ts:312 packages/fileeditor-extension/src/commands.ts:313
 msgid "Show the line numbers for the current file."
 msgstr "Показывать номера строк текущего файла."
 
-#: packages/fileeditor-extension/src/commands.ts:352
+#: packages/fileeditor-extension/src/commands.ts:352 packages/fileeditor-extension/src/commands.ts:353
 msgid "Word Wrap"
 msgstr "Перенос по словам"
 
-#: packages/fileeditor-extension/src/commands.ts:356 packages/mainmenu-extension/src/index.ts:600
+#: packages/fileeditor-extension/src/commands.ts:356 packages/fileeditor-extension/src/commands.ts:357 packages/mainmenu-extension/src/index.ts:595 packages/mainmenu-extension/src/index.ts:600
 msgid "Wrap Words"
 msgstr "Переносить по словам"
 
-#: packages/fileeditor-extension/src/commands.ts:357
+#: packages/fileeditor-extension/src/commands.ts:357 packages/fileeditor-extension/src/commands.ts:358
 msgid "Wrap words for the current file."
 msgstr "Перенос слов для текущего файла."
 
-#: packages/fileeditor-extension/src/commands.ts:383 packages/fileeditor-extension/src/index.ts:147
+#: packages/fileeditor-extension/src/commands.ts:383 packages/fileeditor-extension/src/commands.ts:384 packages/fileeditor-extension/src/index.ts:147
 msgctxt "v4"
 msgid "Spaces: %1"
 msgstr "Пробелы: %1"
 
-#: packages/fileeditor-extension/src/commands.ts:385 packages/fileeditor-extension/src/index.ts:140
+#: packages/fileeditor-extension/src/commands.ts:385 packages/fileeditor-extension/src/commands.ts:386 packages/fileeditor-extension/src/index.ts:140
 msgid "Indent with Tab"
 msgstr "Отступы табуляцией"
 
-#: packages/fileeditor-extension/src/commands.ts:430
+#: packages/fileeditor-extension/src/commands.ts:430 packages/fileeditor-extension/src/commands.ts:431
 msgid "Change match brackets for the current file."
 msgstr "Измените скобки соответствия для текущего файла."
 
-#: packages/fileeditor-extension/src/commands.ts:468
+#: packages/fileeditor-extension/src/commands.ts:468 packages/fileeditor-extension/src/commands.ts:469
 msgid "Auto Close Brackets in Text Editor"
 msgstr "Автоматически закрывать скобки в текстовом редакторе"
 
-#: packages/fileeditor-extension/src/commands.ts:496
+#: packages/fileeditor-extension/src/commands.ts:496 packages/fileeditor-extension/src/commands.ts:497
 msgid "Auto Close Brackets"
 msgstr "Автоматическое закрытие скобок"
 
-#: packages/fileeditor-extension/src/commands.ts:511
+#: packages/fileeditor-extension/src/commands.ts:511 packages/fileeditor-extension/src/commands.ts:512
 msgid "Editor Theme"
 msgstr "Тема редактора"
 
-#: packages/fileeditor-extension/src/commands.ts:539 packages/mainmenu-extension/src/index.ts:324
+#: packages/fileeditor-extension/src/commands.ts:539 packages/fileeditor-extension/src/commands.ts:540 packages/mainmenu-extension/src/index.ts:320 packages/mainmenu-extension/src/index.ts:324
 msgid "Go to Line…"
 msgstr "Перейти к строке…"
 
-#: packages/fileeditor-extension/src/commands.ts:564
+#: packages/fileeditor-extension/src/commands.ts:564 packages/fileeditor-extension/src/commands.ts:565
 msgid "Change editor language."
 msgstr "Изменить язык редактора."
 
-#: packages/fileeditor-extension/src/commands.ts:608
+#: packages/fileeditor-extension/src/commands.ts:608 packages/fileeditor-extension/src/commands.ts:609
 msgid "Replace Selection in Editor"
 msgstr "Заменить выделенное в редакторе"
 
-#: packages/fileeditor-extension/src/commands.ts:626
+#: packages/fileeditor-extension/src/commands.ts:626 packages/fileeditor-extension/src/commands.ts:627
 msgid "Create Console for Editor"
 msgstr "Создать консоль для редактора"
 
-#: packages/fileeditor-extension/src/commands.ts:647
+#: packages/fileeditor-extension/src/commands.ts:647 packages/fileeditor-extension/src/commands.ts:648
 msgid "Restart Kernel"
 msgstr "Перезапустить ядро"
 
-#: packages/fileeditor-extension/src/commands.ts:712
+#: packages/fileeditor-extension/src/commands.ts:712 packages/fileeditor-extension/src/commands.ts:713
 msgid "Run Selected Code"
 msgstr "Запустить выбранный код"
 
-#: packages/fileeditor-extension/src/commands.ts:750
+#: packages/fileeditor-extension/src/commands.ts:750 packages/fileeditor-extension/src/commands.ts:751
 msgid "Run All Code"
 msgstr "Запустить весь код"
 
-#: packages/fileeditor-extension/src/commands.ts:777
+#: packages/fileeditor-extension/src/commands.ts:777 packages/fileeditor-extension/src/commands.ts:778
 msgid "Show Markdown Preview"
 msgstr "Показать предпросмотр Markdown"
 
-#: packages/fileeditor-extension/src/commands.ts:788
+#: packages/fileeditor-extension/src/commands.ts:788 packages/fileeditor-extension/src/commands.ts:789
 msgid "New Text File"
 msgstr "Новый текстовый файл"
 
-#: packages/fileeditor-extension/src/commands.ts:790
+#: packages/fileeditor-extension/src/commands.ts:790 packages/fileeditor-extension/src/commands.ts:791
 msgid "Text File"
 msgstr "Текстовый файл"
 
-#: packages/fileeditor-extension/src/commands.ts:793
+#: packages/fileeditor-extension/src/commands.ts:793 packages/fileeditor-extension/src/commands.ts:794
 msgid "Create a new text file"
 msgstr "Создать новый текстовый файл"
 
-#: packages/fileeditor-extension/src/commands.ts:818
+#: packages/fileeditor-extension/src/commands.ts:818 packages/fileeditor-extension/src/commands.ts:819
 msgid "Create a new markdown file"
 msgstr "Создать новый markdown файл"
 
-#: packages/fileeditor-extension/src/commands.ts:854 packages/mainmenu-extension/src/index.ts:277 packages/notebook-extension/src/index.ts:3122
-msgid "Undo"
-msgstr "Отменить"
-
-#: packages/fileeditor-extension/src/commands.ts:885 packages/mainmenu-extension/src/index.ts:288 packages/notebook-extension/src/index.ts:3108
-msgid "Redo"
-msgstr "Повторить"
-
-#: packages/fileeditor-extension/src/commands.ts:999
+#: packages/fileeditor-extension/src/commands.ts:997 packages/fileeditor-extension/src/commands.ts:998 packages/fileeditor-extension/src/commands.ts:999
 msgid "Select All"
 msgstr "Выбрать все"
 
 #: packages/fileeditor-extension/src/index.ts:309
 msgid "Editor"
 msgstr "Редактор"
 
@@ -5801,15 +5927,15 @@
 msgid "Hub Control Panel"
 msgstr "Панель управления Хабом"
 
 #: packages/hub-extension/src/index.ts:83
 msgid "Open the Hub control panel in a new browser tab"
 msgstr "Открыть панель управления Хабом в новой вкладке браузера"
 
-#: packages/hub-extension/src/index.ts:90 packages/mainmenu-extension/src/index.ts:443
+#: packages/hub-extension/src/index.ts:90 packages/mainmenu-extension/src/index.ts:440 packages/mainmenu-extension/src/index.ts:443
 msgid "Log Out"
 msgstr "Выйти"
 
 #: packages/hub-extension/src/index.ts:91
 msgid "Log out of the Hub"
 msgstr "Выйти из Хаба"
 
@@ -5881,19 +6007,19 @@
 msgid "Are you sure that you want to run arbitrary Javascript within your JupyterLab session?"
 msgstr "Вы уверены, что хотите запустить произвольный Javascript в вашей сессии JupyterLab?"
 
 #: packages/javascript-extension/src/index.ts:45 packages/rendermime/src/renderers.ts:66
 msgid "Run"
 msgstr "Запуск"
 
-#: packages/launcher-extension/src/index.ts:148 packages/launcher-extension/src/index.ts:94
+#: packages/launcher-extension/src/index.ts:138 packages/launcher-extension/src/index.ts:148 packages/launcher-extension/src/index.ts:84 packages/launcher-extension/src/index.ts:94
 msgid "Launcher"
 msgstr "Лаунчер"
 
-#: packages/launcher-extension/src/index.ts:72 packages/ui-components/src/icon/widgets/tabbarsvg.ts:31
+#: packages/launcher-extension/src/index.ts:62 packages/launcher-extension/src/index.ts:72 packages/ui-components/src/icon/widgets/tabbarsvg.ts:31
 msgid "New Launcher"
 msgstr "Новый лаунчер"
 
 #: packages/launcher/src/widget.tsx:273
 msgctxt "Error"
 msgid "Launcher Error"
 msgstr "Ошибка лаунчера"
@@ -5962,15 +6088,15 @@
 msgid "No log messages."
 msgstr "В журнале нет сообщений."
 
 #: packages/lsp-extension/src/index.ts:285
 msgid "Language servers"
 msgstr "Языковой сервер"
 
-#: packages/lsp-extension/src/index.ts:304 packages/mainmenu-extension/src/index.ts:549 packages/running-extension/src/kernels.ts:67 packages/running/src/index.tsx:357 packages/terminal-extension/src/index.ts:323
+#: packages/lsp-extension/src/index.ts:304 packages/mainmenu-extension/src/index.ts:546 packages/mainmenu-extension/src/index.ts:549 packages/running-extension/src/kernels.ts:67 packages/running-extension/src/kernels.tsx:87 packages/running/src/index.tsx:357 packages/running/src/index.tsx:573 packages/terminal-extension/src/index.ts:323
 msgid "Shut Down All"
 msgstr "Завершить все"
 
 #: packages/lsp-extension/src/index.ts:305
 msgid "Are you sure you want to permanently shut down all running language servers?"
 msgstr "Вы уверены, что хотите навсегда выключить все работающие языковые серверы?"
 
@@ -5994,146 +6120,190 @@
 msgid "Add server"
 msgstr "Добавить сервер"
 
 #: packages/lsp/src/adapters/adapter.ts:482 packages/lsp/src/adapters/adapter.ts:500
 msgid "Message from "
 msgstr "Сообщение от "
 
-#: packages/mainmenu-extension/src/index.ts:193
+#: packages/mainmenu-extension/src/index.ts:193 packages/mainmenu-extension/src/index.ts:194
 msgid "Open Edit Menu"
 msgstr "Открыть меню \"Редактировать\""
 
-#: packages/mainmenu-extension/src/index.ts:197
+#: packages/mainmenu-extension/src/index.ts:197 packages/mainmenu-extension/src/index.ts:198
 msgid "Open File Menu"
 msgstr "Открыть меню \"Файл\""
 
-#: packages/mainmenu-extension/src/index.ts:201
+#: packages/mainmenu-extension/src/index.ts:201 packages/mainmenu-extension/src/index.ts:202
 msgid "Open Kernel Menu"
 msgstr "Открыть меню \"Ядро\""
 
-#: packages/mainmenu-extension/src/index.ts:205
+#: packages/mainmenu-extension/src/index.ts:205 packages/mainmenu-extension/src/index.ts:206
 msgid "Open Run Menu"
 msgstr "Открыть меню \"Запуск\""
 
-#: packages/mainmenu-extension/src/index.ts:209
+#: packages/mainmenu-extension/src/index.ts:209 packages/mainmenu-extension/src/index.ts:210
 msgid "Open View Menu"
 msgstr "Открыть меню \"Вид\""
 
-#: packages/mainmenu-extension/src/index.ts:213
+#: packages/mainmenu-extension/src/index.ts:213 packages/mainmenu-extension/src/index.ts:214
 msgid "Open Settings Menu"
 msgstr "Открыть меню \"Настройки\""
 
-#: packages/mainmenu-extension/src/index.ts:217
+#: packages/mainmenu-extension/src/index.ts:217 packages/mainmenu-extension/src/index.ts:218
 msgid "Open Tabs Menu"
 msgstr "Открыть меню \"Вкладки\""
 
-#: packages/mainmenu-extension/src/index.ts:221
+#: packages/mainmenu-extension/src/index.ts:221 packages/mainmenu-extension/src/index.ts:222
 msgid "Open Help Menu"
 msgstr "Открыть меню \"Помощь\""
 
-#: packages/mainmenu-extension/src/index.ts:225
+#: packages/mainmenu-extension/src/index.ts:225 packages/mainmenu-extension/src/index.ts:226
 msgid "Open First Menu"
 msgstr "Открыть первое меню"
 
-#: packages/mainmenu-extension/src/index.ts:245
+#: packages/mainmenu-extension/src/index.ts:245 packages/mainmenu-extension/src/index.ts:246
 msgid "Kernel Operations"
 msgstr "Операции с ядром"
 
-#: packages/mainmenu-extension/src/index.ts:301
+#: packages/mainmenu-extension/src/index.ts:299 packages/mainmenu-extension/src/index.ts:301
 msgid "Clear"
 msgstr "Очистить"
 
-#: packages/mainmenu-extension/src/index.ts:312
+#: packages/mainmenu-extension/src/index.ts:309 packages/mainmenu-extension/src/index.ts:312
 msgid "Clear All"
 msgstr "Очистить все"
 
-#: packages/mainmenu-extension/src/index.ts:352
+#: packages/mainmenu-extension/src/index.ts:348 packages/mainmenu-extension/src/index.ts:352
 msgid "Close and Shut Down"
 msgstr "Закрыть и завершить работу"
 
-#: packages/mainmenu-extension/src/index.ts:368
+#: packages/mainmenu-extension/src/index.ts:365 packages/mainmenu-extension/src/index.ts:368
 msgid "New Console for Activity"
 msgstr "Новая консоль для действий"
 
+#: packages/mainmenu-extension/src/index.ts:372
+msgid "Shut down %1"
+msgstr ""
+
 #: packages/mainmenu-extension/src/index.ts:376
 msgid "Shut down JupyterLab"
 msgstr "Завершить работу Jupyterlab"
 
-#: packages/mainmenu-extension/src/index.ts:381
+#: packages/mainmenu-extension/src/index.ts:377 packages/mainmenu-extension/src/index.ts:381
 msgid "Shutdown confirmation"
 msgstr "Подтверждение завершения работы"
 
+#: packages/mainmenu-extension/src/index.ts:378
+msgid "Please confirm you want to shut down %1."
+msgstr ""
+
 #: packages/mainmenu-extension/src/index.ts:382
 msgid "Please confirm you want to shut down JupyterLab."
 msgstr "Пожалуйста, подтвердите, что вы хотите завершить работу JupyterLab."
 
-#: packages/mainmenu-extension/src/index.ts:414
+#: packages/mainmenu-extension/src/index.ts:410 packages/mainmenu-extension/src/index.ts:414
 msgid "You have shut down the Jupyter server. You can now close this tab."
 msgstr "Вы выключили Jupyter сервер. Теперь вы можете закрыть эту вкладку."
 
+#: packages/mainmenu-extension/src/index.ts:414
+msgid "To use %1 again, you will need to relaunch it."
+msgstr ""
+
 #: packages/mainmenu-extension/src/index.ts:418
 msgid "To use JupyterLab again, you will need to relaunch it."
 msgstr "Чтобы использовать JupyterLab снова, вам нужно будет перезапустить его."
 
-#: packages/mainmenu-extension/src/index.ts:425
+#: packages/mainmenu-extension/src/index.ts:422 packages/mainmenu-extension/src/index.ts:425
 msgid "Server stopped"
 msgstr "Сервер остановлен"
 
+#: packages/mainmenu-extension/src/index.ts:441
+msgid "Log out of %1"
+msgstr ""
+
 #: packages/mainmenu-extension/src/index.ts:444
 msgid "Log out of JupyterLab"
 msgstr "Выйти из JupyterLab"
 
-#: packages/mainmenu-extension/src/index.ts:482 packages/notebook-extension/src/index.ts:3158
+#: packages/mainmenu-extension/src/index.ts:480 packages/mainmenu-extension/src/index.ts:482 packages/notebook-extension/src/index.ts:3158 packages/notebook-extension/src/index.ts:3165 packages/notebook-extension/src/index.ts:3188
 msgid "Reconnect to Kernel"
 msgstr "Переподключиться к ядру"
 
 #: packages/mainmenu-extension/src/index.ts:507
 msgid "Restart Kernel and Clear…"
 msgstr "Перезапустить ядро и очистить…"
 
-#: packages/mainmenu-extension/src/index.ts:532
+#: packages/mainmenu-extension/src/index.ts:530 packages/mainmenu-extension/src/index.ts:532
 msgid "Shut down kernel"
 msgstr "Завершить работу ядра"
 
-#: packages/mainmenu-extension/src/index.ts:539
+#: packages/mainmenu-extension/src/index.ts:536 packages/mainmenu-extension/src/index.ts:539
 msgid "Shut Down All Kernels…"
 msgstr "Завершить работу всех ядер…"
 
-#: packages/mainmenu-extension/src/index.ts:545
+#: packages/mainmenu-extension/src/index.ts:542 packages/mainmenu-extension/src/index.ts:545
 msgid "Shut Down All?"
 msgstr "Завершить все?"
 
-#: packages/mainmenu-extension/src/index.ts:546
+#: packages/mainmenu-extension/src/index.ts:543 packages/mainmenu-extension/src/index.ts:546
 msgid "Shut down all kernels?"
 msgstr "Завершить все ядра?"
 
-#: packages/mainmenu-extension/src/index.ts:622 packages/mainmenu-extension/src/index.ts:623
+#: packages/mainmenu-extension/src/index.ts:617 packages/mainmenu-extension/src/index.ts:618 packages/mainmenu-extension/src/index.ts:622 packages/mainmenu-extension/src/index.ts:623
 msgid "Run Selected"
 msgstr "Выполнить выбранное"
 
-#: packages/mainmenu-extension/src/index.ts:636 packages/mainmenu-extension/src/index.ts:637
+#: packages/mainmenu-extension/src/index.ts:632 packages/mainmenu-extension/src/index.ts:633 packages/mainmenu-extension/src/index.ts:636 packages/mainmenu-extension/src/index.ts:637
 msgid "Run All"
 msgstr "Выполнить всё"
 
-#: packages/mainmenu-extension/src/index.ts:648 packages/mainmenu-extension/src/index.ts:649
+#: packages/mainmenu-extension/src/index.ts:644 packages/mainmenu-extension/src/index.ts:645 packages/mainmenu-extension/src/index.ts:648 packages/mainmenu-extension/src/index.ts:649
 msgid "Restart Kernel and Run All"
 msgstr "Перезапустить ядро и выполнить всё"
 
-#: packages/mainmenu-extension/src/index.ts:677
+#: packages/mainmenu-extension/src/index.ts:674 packages/mainmenu-extension/src/index.ts:677
 msgid "Activate a widget by its `id`."
 msgstr "Активируйте виджет по его `id`."
 
-#: packages/mainmenu-extension/src/index.ts:694
+#: packages/mainmenu-extension/src/index.ts:691 packages/mainmenu-extension/src/index.ts:694
 msgid "Activate Previously Used Tab"
 msgstr "Перейти к предыдущей использованной вкладке"
 
-#: packages/mainmenu-extension/src/index.ts:771
+#: packages/mainmenu-extension/src/index.ts:768 packages/mainmenu-extension/src/index.ts:771
 msgid "Menu customization has changed. You will need to reload JupyterLab to see the changes."
 msgstr "Меню изменилось. Вам нужно будет перезагрузить JupyterLab для просмотра изменений."
 
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
 #: packages/markdownviewer-extension/src/index.ts:124 packages/markdownviewer-extension/src/index.ts:150
 msgid "Markdown Preview"
 msgstr "Предпросмотр Markdown"
 
 #: packages/markdownviewer-extension/src/index.ts:185
 msgid "Show Markdown Editor"
 msgstr "Показать редактор Markdown"
@@ -6142,594 +6312,606 @@
 msgid "Mermaid Copy Diagram Source"
 msgstr ""
 
 #: packages/metadataform/src/metadataform.ts:54
 msgid "No metadata."
 msgstr "Нет метаданных."
 
-#: packages/notebook-extension/src/index.ts:1146
+#: packages/notebook-extension/src/index.ts:1146 packages/notebook-extension/src/index.ts:1150 packages/notebook-extension/src/index.ts:1158
 msgid "Notebook Tools"
 msgstr "Инструменты Блокнота"
 
-#: packages/notebook-extension/src/index.ts:1298
+#: packages/notebook-extension/src/index.ts:1298 packages/notebook-extension/src/index.ts:1302 packages/notebook-extension/src/index.ts:1310
 msgid "Create New View for Cell Output"
 msgstr "Создать новый вид для результата ячейки"
 
-#: packages/notebook-extension/src/index.ts:1368
+#: packages/notebook-extension/src/index.ts:1368 packages/notebook-extension/src/index.ts:1372 packages/notebook-extension/src/index.ts:1380
 msgid "New Console for Notebook"
 msgstr "Новая консоль для Блокнота"
 
-#: packages/notebook-extension/src/index.ts:1386
+#: packages/notebook-extension/src/index.ts:1386 packages/notebook-extension/src/index.ts:1390 packages/notebook-extension/src/index.ts:1398
 msgid "Run Selected Text or Current Line in Console"
 msgstr "Запустить выделенный текст или текущую строку в консоли"
 
-#: packages/notebook-extension/src/index.ts:1550
+#: packages/notebook-extension/src/index.ts:1550 packages/notebook-extension/src/index.ts:1554 packages/notebook-extension/src/index.ts:1562
 msgid "Copy Output to Clipboard"
 msgstr "Скопировать Output в буфер обмена"
 
-#: packages/notebook-extension/src/index.ts:1707
+#: packages/notebook-extension/src/index.ts:1707 packages/notebook-extension/src/index.ts:1712 packages/notebook-extension/src/index.ts:1723
 msgid "Auto Close Brackets for All Notebook Cell Types"
 msgstr "Автоматически закрывать скобки для всех типов ячеек"
 
-#: packages/notebook-extension/src/index.ts:1716
+#: packages/notebook-extension/src/index.ts:1716 packages/notebook-extension/src/index.ts:1721 packages/notebook-extension/src/index.ts:1732
 msgid "Set side-by-side ratio"
 msgstr "Установка соотношения бок о бок"
 
-#: packages/notebook-extension/src/index.ts:1719
+#: packages/notebook-extension/src/index.ts:1719 packages/notebook-extension/src/index.ts:1724 packages/notebook-extension/src/index.ts:1735
 msgid "Width of the output in side-by-side mode"
 msgstr "Ширина вывода в боковом режиме"
 
-#: packages/notebook-extension/src/index.ts:1953
+#: packages/notebook-extension/src/index.ts:1953 packages/notebook-extension/src/index.ts:1958 packages/notebook-extension/src/index.ts:1969
 msgid "New Notebook"
 msgstr "Новый Блокнот"
 
-#: packages/notebook-extension/src/index.ts:1957
+#: packages/notebook-extension/src/index.ts:1957 packages/notebook-extension/src/index.ts:1962 packages/notebook-extension/src/index.ts:1973
 msgid "Create a new notebook"
 msgstr "Создать новый блокнот"
 
-#: packages/notebook-extension/src/index.ts:2213
+#: packages/notebook-extension/src/index.ts:2213 packages/notebook-extension/src/index.ts:2220 packages/notebook-extension/src/index.ts:2231
 msgid "Run Selected Cell"
 msgid_plural "Run Selected Cells"
 msgstr[0] "Выполнить выбранную ячейку"
 msgstr[1] "Выполнить выбранные ячейки"
 msgstr[2] "Выполнить выбранных ячеек"
 msgstr[3] "Выполнить выбранных ячеек"
 
-#: packages/notebook-extension/src/index.ts:2221
+#: packages/notebook-extension/src/index.ts:2221 packages/notebook-extension/src/index.ts:2228 packages/notebook-extension/src/index.ts:2239
 msgid "Run this cell and advance"
 msgid_plural "Run these %1 cells and advance"
 msgstr[0] "Выполнить эту ячейку и продвинуться вперед"
 msgstr[1] "Выполнить эти %1 ячейки и продвинуться вперед"
 msgstr[2] "Выполнить эти %1 ячеек и продвинуться вперед"
 msgstr[3] "Выполнить эти %1 ячеек и продвинуться вперед"
 
-#: packages/notebook-extension/src/index.ts:2247
+#: packages/notebook-extension/src/index.ts:2247 packages/notebook-extension/src/index.ts:2254 packages/notebook-extension/src/index.ts:2265
 msgid "Run Selected Cell and Do not Advance"
 msgid_plural "Run Selected Cells and Do not Advance"
 msgstr[0] "Выполнить выбранную ячейку и не продвигаться дальше"
 msgstr[1] "Выполнить выбранные ячейки и не продвигаться дальше"
 msgstr[2] "Выполнить выбранные ячейки и не продвигаться дальше"
 msgstr[3] "Выполнить выбранные ячейки и не продвигаться дальше"
 
-#: packages/notebook-extension/src/index.ts:2272
+#: packages/notebook-extension/src/index.ts:2272 packages/notebook-extension/src/index.ts:2279 packages/notebook-extension/src/index.ts:2290
 msgid "Run Selected Cell and Insert Below"
 msgid_plural "Run Selected Cells and Insert Below"
 msgstr[0] "Запустить выбранную ячейку и вставить ниже"
 msgstr[1] "Запустить выбранные ячейки и вставить ниже"
 msgstr[2] "Запустить выбранные ячейки и вставить ниже"
 msgstr[3] "Запустить выбранные ячейки и вставить ниже"
 
-#: packages/notebook-extension/src/index.ts:2295
+#: packages/notebook-extension/src/index.ts:2295 packages/notebook-extension/src/index.ts:2302 packages/notebook-extension/src/index.ts:2313
 msgid "Run All Cells"
 msgstr "Запустить все ячейки"
 
-#: packages/notebook-extension/src/index.ts:2296
+#: packages/notebook-extension/src/index.ts:2296 packages/notebook-extension/src/index.ts:2303 packages/notebook-extension/src/index.ts:2314
 msgid "Run all cells"
 msgstr "Запустить все ячейки"
 
-#: packages/notebook-extension/src/index.ts:2314
+#: packages/notebook-extension/src/index.ts:2314 packages/notebook-extension/src/index.ts:2321 packages/notebook-extension/src/index.ts:2332
 msgid "Run All Above Selected Cell"
 msgstr "Выполнить все ячейки, выше выбранной"
 
-#: packages/notebook-extension/src/index.ts:2339
+#: packages/notebook-extension/src/index.ts:2339 packages/notebook-extension/src/index.ts:2346 packages/notebook-extension/src/index.ts:2357
 msgid "Run Selected Cell and All Below"
 msgstr "Выполнить выбранную ячейку и ниже"
 
-#: packages/notebook-extension/src/index.ts:2365
+#: packages/notebook-extension/src/index.ts:2365 packages/notebook-extension/src/index.ts:2372 packages/notebook-extension/src/index.ts:2383
 msgid "Render All Markdown Cells"
 msgstr "Отрисовать все ячейки Markdown"
 
-#: packages/notebook-extension/src/index.ts:2402
+#: packages/notebook-extension/src/index.ts:2402 packages/notebook-extension/src/index.ts:2409
 msgid "Close and Shut Down Notebook"
 msgstr "Закрыть и выключить блокнот"
 
-#: packages/notebook-extension/src/index.ts:2413
+#: packages/notebook-extension/src/index.ts:2413 packages/notebook-extension/src/index.ts:2420 packages/notebook-extension/src/index.ts:2431
 msgid "Shut down the notebook?"
 msgstr "Завершить работу данного блокнота?"
 
-#: packages/notebook-extension/src/index.ts:2429
+#: packages/notebook-extension/src/index.ts:2420
+msgid "Close and Shut Down Notebook…"
+msgstr ""
+
+#: packages/notebook-extension/src/index.ts:2429 packages/notebook-extension/src/index.ts:2436 packages/notebook-extension/src/index.ts:2447
 msgid "Trust Notebook"
 msgstr "Доверять блокноту"
 
-#: packages/notebook-extension/src/index.ts:2440
+#: packages/notebook-extension/src/index.ts:2440 packages/notebook-extension/src/index.ts:2447 packages/notebook-extension/src/index.ts:2458
 msgid "Restart Kernel and Clear Outputs of All Cells…"
 msgstr "Перезапустите ядро и очистите выводы всех ячеек…"
 
-#: packages/notebook-extension/src/index.ts:2441
+#: packages/notebook-extension/src/index.ts:2441 packages/notebook-extension/src/index.ts:2448 packages/notebook-extension/src/index.ts:2459
 msgid "Restart the kernel and clear all outputs of all cells"
 msgstr "Перезапустите ядро и очистите все выводы всех ячеек"
 
-#: packages/notebook-extension/src/index.ts:2453
+#: packages/notebook-extension/src/index.ts:2453 packages/notebook-extension/src/index.ts:2460 packages/notebook-extension/src/index.ts:2471
 msgid "Restart Kernel and Run up to Selected Cell…"
 msgstr "Перезапустить ядро и выполнить до выбранной ячейки…"
 
-#: packages/notebook-extension/src/index.ts:2477
+#: packages/notebook-extension/src/index.ts:2477 packages/notebook-extension/src/index.ts:2484 packages/notebook-extension/src/index.ts:2495
 msgid "Restart Kernel and Run All Cells…"
 msgstr "Перезапустить ядро и выполнить все ячейки…"
 
-#: packages/notebook-extension/src/index.ts:2478
+#: packages/notebook-extension/src/index.ts:2478 packages/notebook-extension/src/index.ts:2485 packages/notebook-extension/src/index.ts:2496
 msgid "Restart the kernel and run all cells"
 msgstr "Перезапустите ядро и запустите все ячейки"
 
-#: packages/notebook-extension/src/index.ts:2504
+#: packages/notebook-extension/src/index.ts:2504 packages/notebook-extension/src/index.ts:2511 packages/notebook-extension/src/index.ts:2522
 msgid "Clear Outputs of All Cells"
 msgstr "Очистить результаты всех ячеек"
 
-#: packages/notebook-extension/src/index.ts:2505
+#: packages/notebook-extension/src/index.ts:2505 packages/notebook-extension/src/index.ts:2512 packages/notebook-extension/src/index.ts:2523
 msgid "Clear all outputs of all cells"
 msgstr "Очистить все результаты всех ячеек"
 
-#: packages/notebook-extension/src/index.ts:2516
+#: packages/notebook-extension/src/index.ts:2516 packages/notebook-extension/src/index.ts:2523 packages/notebook-extension/src/index.ts:2534
 msgid "Clear Cell Output"
 msgstr "Очистить вывод ячейки"
 
-#: packages/notebook-extension/src/index.ts:2517
+#: packages/notebook-extension/src/index.ts:2517 packages/notebook-extension/src/index.ts:2524 packages/notebook-extension/src/index.ts:2535
 msgid "Clear outputs for the selected cells"
 msgstr "Очистить результаты для выбранных ячеек"
 
-#: packages/notebook-extension/src/index.ts:2547
+#: packages/notebook-extension/src/index.ts:2547 packages/notebook-extension/src/index.ts:2554 packages/notebook-extension/src/index.ts:2565
 msgid "Change to Code Cell Type"
 msgstr "Преобразовать в ячейку с кодом"
 
-#: packages/notebook-extension/src/index.ts:2558
+#: packages/notebook-extension/src/index.ts:2558 packages/notebook-extension/src/index.ts:2565 packages/notebook-extension/src/index.ts:2580
 msgid "Change to Markdown Cell Type"
 msgstr "Преобразовать в ячейку c Markdown"
 
-#: packages/notebook-extension/src/index.ts:2569
+#: packages/notebook-extension/src/index.ts:2569 packages/notebook-extension/src/index.ts:2576 packages/notebook-extension/src/index.ts:2595
 msgid "Change to Raw Cell Type"
 msgstr "Преобразовать в ячейку с сырым текстом"
 
-#: packages/notebook-extension/src/index.ts:2582
+#: packages/notebook-extension/src/index.ts:2582 packages/notebook-extension/src/index.ts:2589 packages/notebook-extension/src/index.ts:2612
 msgid "Cut Cell"
 msgid_plural "Cut Cells"
 msgstr[0] "Вырезать ячейку"
 msgstr[1] "Вырезать ячейки"
 msgstr[2] "Вырезать ячеек"
 msgstr[3] "Вырезать ячеек"
 
-#: packages/notebook-extension/src/index.ts:2590
+#: packages/notebook-extension/src/index.ts:2590 packages/notebook-extension/src/index.ts:2597 packages/notebook-extension/src/index.ts:2620
 msgid "Cut this cell"
 msgid_plural "Cut these %1 cells"
 msgstr[0] "Вырезать эту ячейку"
 msgstr[1] "Вырезать эти %1 ячейки"
 msgstr[2] "Вырезать эти %1 ячеек"
 msgstr[3] "Вырезать эти %1 ячеек"
 
-#: packages/notebook-extension/src/index.ts:2609
+#: packages/notebook-extension/src/index.ts:2609 packages/notebook-extension/src/index.ts:2616 packages/notebook-extension/src/index.ts:2639
 msgid "Copy Cell"
 msgid_plural "Copy Cells"
 msgstr[0] "Копировать ячейку"
 msgstr[1] "Копировать ячейки"
 msgstr[2] "Копировать ячеек"
 msgstr[3] "Копировать ячеек"
 
-#: packages/notebook-extension/src/index.ts:2617
+#: packages/notebook-extension/src/index.ts:2617 packages/notebook-extension/src/index.ts:2624 packages/notebook-extension/src/index.ts:2647
 msgid "Copy this cell"
 msgid_plural "Copy these %1 cells"
 msgstr[0] "Копировать эту ячейку"
 msgstr[1] "Копировать эти %1 ячейки"
 msgstr[2] "Копировать эти %1 ячеек"
 msgstr[3] "Копировать эти %1 ячеек"
 
-#: packages/notebook-extension/src/index.ts:2636
+#: packages/notebook-extension/src/index.ts:2636 packages/notebook-extension/src/index.ts:2643 packages/notebook-extension/src/index.ts:2666
 msgid "Paste Cell Below"
 msgid_plural "Paste Cells Below"
 msgstr[0] "Вставить ячейку ниже"
 msgstr[1] "Вставить ячейки ниже"
 msgstr[2] "Вставить ячейки ниже"
 msgstr[3] "Вставить ячейки ниже"
 
-#: packages/notebook-extension/src/index.ts:2644 packages/notebook-extension/src/index.ts:2671
+#: packages/notebook-extension/src/index.ts:2644 packages/notebook-extension/src/index.ts:2651 packages/notebook-extension/src/index.ts:2671 packages/notebook-extension/src/index.ts:2674 packages/notebook-extension/src/index.ts:2678 packages/notebook-extension/src/index.ts:2701
 msgid "Paste this cell from the clipboard"
 msgid_plural "Paste these %1 cells from the clipboard"
 msgstr[0] "Вставить эту ячейку из буфера обмена"
 msgstr[1] "Вставить эти %1 ячейки из буфера обмена"
 msgstr[2] "Вставить эти %1 ячеек из буфера обмена"
 msgstr[3] "Вставить эти %1 ячеек из буфера обмена"
 
-#: packages/notebook-extension/src/index.ts:2663
+#: packages/notebook-extension/src/index.ts:2663 packages/notebook-extension/src/index.ts:2670 packages/notebook-extension/src/index.ts:2693
 msgid "Paste Cell Above"
 msgid_plural "Paste Cells Above"
 msgstr[0] "Вставить ячейку выше"
 msgstr[1] "Вставить ячейки выше"
 msgstr[2] "Вставить ячейки выше"
 msgstr[3] "Вставить ячейки выше"
 
-#: packages/notebook-extension/src/index.ts:2689
+#: packages/notebook-extension/src/index.ts:2689 packages/notebook-extension/src/index.ts:2696 packages/notebook-extension/src/index.ts:2719
 msgid "Duplicate Cell Below"
 msgid_plural "Duplicate Cells Below"
 msgstr[0] "Дублировать ячейку ниже"
 msgstr[1] "Дублировать ячейки ниже"
 msgstr[2] "Дублировать ячейки ниже"
 msgstr[3] "Дублировать ячейки ниже"
 
-#: packages/notebook-extension/src/index.ts:2697
+#: packages/notebook-extension/src/index.ts:2697 packages/notebook-extension/src/index.ts:2704 packages/notebook-extension/src/index.ts:2727
 msgid "Create a duplicate of this cell below"
 msgid_plural "Create duplicates of %1 cells below"
 msgstr[0] "Создать дубликат этой ячейки ниже"
 msgstr[1] "Создать дубликаты %1 ячеек ниже"
 msgstr[2] "Создать дубликаты %1 ячеек ниже"
 msgstr[3] "Создать дубликаты %1 ячеек ниже"
 
-#: packages/notebook-extension/src/index.ts:2716
+#: packages/notebook-extension/src/index.ts:2716 packages/notebook-extension/src/index.ts:2723 packages/notebook-extension/src/index.ts:2746
 msgid "Paste Cell and Replace"
 msgid_plural "Paste Cells and Replace"
 msgstr[0] "Вставить ячейку и заменить"
 msgstr[1] "Вставить ячейки и заменить"
 msgstr[2] "Вставить ячейки и заменить"
 msgstr[3] "Вставить ячейки и заменить"
 
-#: packages/notebook-extension/src/index.ts:2734
+#: packages/notebook-extension/src/index.ts:2734 packages/notebook-extension/src/index.ts:2741 packages/notebook-extension/src/index.ts:2764
 msgid "Delete Cell"
 msgid_plural "Delete Cells"
 msgstr[0] "Удалить ячейку"
 msgstr[1] "Удалить ячейки"
 msgstr[2] "Удалить ячейки"
 msgstr[3] "Удалить ячейки"
 
-#: packages/notebook-extension/src/index.ts:2742
+#: packages/notebook-extension/src/index.ts:2742 packages/notebook-extension/src/index.ts:2749 packages/notebook-extension/src/index.ts:2772
 msgid "Delete this cell"
 msgid_plural "Delete these %1 cells"
 msgstr[0] "Удалить эту ячейку"
 msgstr[1] "Удалить эти %1 ячейки"
 msgstr[2] "Удалить эти %1 ячеек"
 msgstr[3] "Удалить эти %1 ячеек"
 
-#: packages/notebook-extension/src/index.ts:2759
+#: packages/notebook-extension/src/index.ts:2759 packages/notebook-extension/src/index.ts:2766 packages/notebook-extension/src/index.ts:2789
 msgid "Split Cell"
 msgstr "Разделить ячейки"
 
-#: packages/notebook-extension/src/index.ts:2770
+#: packages/notebook-extension/src/index.ts:2770 packages/notebook-extension/src/index.ts:2777 packages/notebook-extension/src/index.ts:2800
 msgid "Merge Selected Cells"
 msgstr "Объединить выделенные ячейки"
 
-#: packages/notebook-extension/src/index.ts:2781
+#: packages/notebook-extension/src/index.ts:2781 packages/notebook-extension/src/index.ts:2788 packages/notebook-extension/src/index.ts:2811
 msgid "Merge Cell Above"
 msgstr "Объединить ячейку выше"
 
-#: packages/notebook-extension/src/index.ts:2792
+#: packages/notebook-extension/src/index.ts:2792 packages/notebook-extension/src/index.ts:2799 packages/notebook-extension/src/index.ts:2822
 msgid "Merge Cell Below"
 msgstr "Объединить ячейку ниже"
 
-#: packages/notebook-extension/src/index.ts:2803
+#: packages/notebook-extension/src/index.ts:2803 packages/notebook-extension/src/index.ts:2810 packages/notebook-extension/src/index.ts:2833
 msgid "Insert Cell Above"
 msgstr "Вставить ячейку выше"
 
-#: packages/notebook-extension/src/index.ts:2804
+#: packages/notebook-extension/src/index.ts:2804 packages/notebook-extension/src/index.ts:2811 packages/notebook-extension/src/index.ts:2834
 msgid "Insert a cell above"
 msgstr "Вставить ячейку выше"
 
-#: packages/notebook-extension/src/index.ts:2816
+#: packages/notebook-extension/src/index.ts:2816 packages/notebook-extension/src/index.ts:2823 packages/notebook-extension/src/index.ts:2846
 msgid "Insert Cell Below"
 msgstr "Вставить ячейку ниже"
 
-#: packages/notebook-extension/src/index.ts:2817 packages/notebook/src/default-toolbar.tsx:121
+#: packages/notebook-extension/src/index.ts:2817 packages/notebook-extension/src/index.ts:2824 packages/notebook-extension/src/index.ts:2847 packages/notebook/src/default-toolbar.tsx:121
 msgid "Insert a cell below"
 msgstr "Вставить ячейку ниже"
 
-#: packages/notebook-extension/src/index.ts:2829
+#: packages/notebook-extension/src/index.ts:2829 packages/notebook-extension/src/index.ts:2836 packages/notebook-extension/src/index.ts:2859
 msgid "Select Cell Above"
 msgstr "Выбрать ячейку выше"
 
-#: packages/notebook-extension/src/index.ts:2840
+#: packages/notebook-extension/src/index.ts:2840 packages/notebook-extension/src/index.ts:2847 packages/notebook-extension/src/index.ts:2870
 msgid "Select Cell Below"
 msgstr "Выбрать ячейку ниже"
 
-#: packages/notebook-extension/src/index.ts:2850
+#: packages/notebook-extension/src/index.ts:2850 packages/notebook-extension/src/index.ts:2857 packages/notebook-extension/src/index.ts:2880
 msgid "Insert Heading Above Current Heading"
 msgstr "Вставить заголовок выше текущего заголовка"
 
-#: packages/notebook-extension/src/index.ts:2861
+#: packages/notebook-extension/src/index.ts:2861 packages/notebook-extension/src/index.ts:2868 packages/notebook-extension/src/index.ts:2891
 msgid "Insert Heading Below Current Heading"
 msgstr "Вставить заголовок ниже текущего заголовка"
 
-#: packages/notebook-extension/src/index.ts:2872
+#: packages/notebook-extension/src/index.ts:2872 packages/notebook-extension/src/index.ts:2879 packages/notebook-extension/src/index.ts:2902
 msgid "Select Heading Above or Collapse Heading"
 msgstr "Выбрать заголовок выше или свернуть заголовок"
 
-#: packages/notebook-extension/src/index.ts:2885
+#: packages/notebook-extension/src/index.ts:2885 packages/notebook-extension/src/index.ts:2892 packages/notebook-extension/src/index.ts:2915
 msgid "Select Heading Below or Expand Heading"
 msgstr "Выбрать заголовок ниже или развернуть заголовок"
 
-#: packages/notebook-extension/src/index.ts:2898
+#: packages/notebook-extension/src/index.ts:2898 packages/notebook-extension/src/index.ts:2905 packages/notebook-extension/src/index.ts:2928
 msgid "Extend Selection Above"
 msgstr "Продлить выделение выше"
 
-#: packages/notebook-extension/src/index.ts:2909
+#: packages/notebook-extension/src/index.ts:2909 packages/notebook-extension/src/index.ts:2916 packages/notebook-extension/src/index.ts:2939
 msgid "Extend Selection to Top"
 msgstr "Продлить выделение до верха"
 
-#: packages/notebook-extension/src/index.ts:2920
+#: packages/notebook-extension/src/index.ts:2920 packages/notebook-extension/src/index.ts:2927 packages/notebook-extension/src/index.ts:2950
 msgid "Extend Selection Below"
 msgstr "Продлить выделение ниже"
 
-#: packages/notebook-extension/src/index.ts:2931
+#: packages/notebook-extension/src/index.ts:2931 packages/notebook-extension/src/index.ts:2938 packages/notebook-extension/src/index.ts:2961
 msgid "Extend Selection to Bottom"
 msgstr "Продлить выделение до низа"
 
-#: packages/notebook-extension/src/index.ts:2942
+#: packages/notebook-extension/src/index.ts:2942 packages/notebook-extension/src/index.ts:2949 packages/notebook-extension/src/index.ts:2972
 msgid "Select All Cells"
 msgstr "Выбрать все ячейки"
 
-#: packages/notebook-extension/src/index.ts:2953
+#: packages/notebook-extension/src/index.ts:2953 packages/notebook-extension/src/index.ts:2960 packages/notebook-extension/src/index.ts:2983
 msgid "Deselect All Cells"
 msgstr "Отменить выбор всех ячеек"
 
-#: packages/notebook-extension/src/index.ts:2966
+#: packages/notebook-extension/src/index.ts:2966 packages/notebook-extension/src/index.ts:2973 packages/notebook-extension/src/index.ts:2996
 msgid "Move Cell Up"
 msgid_plural "Move Cells Up"
 msgstr[0] "Переместить ячейку вверх"
 msgstr[1] "Переместить ячейки вверх"
 msgstr[2] "Переместить ячейки вверх"
 msgstr[3] "Переместить ячейки вверх"
 
-#: packages/notebook-extension/src/index.ts:2974
+#: packages/notebook-extension/src/index.ts:2974 packages/notebook-extension/src/index.ts:2981 packages/notebook-extension/src/index.ts:3004
 msgid "Move this cell up"
 msgid_plural "Move these %1 cells up"
 msgstr[0] "Переместить эту ячейку вверх"
 msgstr[1] "Переместить эти %1 ячейки вверх"
 msgstr[2] "Переместить эти %1 ячеек вверх"
 msgstr[3] "Переместить эти %1 ячеек вверх"
 
-#: packages/notebook-extension/src/index.ts:2986
+#: packages/notebook-extension/src/index.ts:2986 packages/notebook-extension/src/index.ts:2993 packages/notebook-extension/src/index.ts:3016
 msgid "Notebook cell shifted up successfully"
 msgstr "Ячейка блокнота успешно перемещена"
 
-#: packages/notebook-extension/src/index.ts:3003
+#: packages/notebook-extension/src/index.ts:3003 packages/notebook-extension/src/index.ts:3010 packages/notebook-extension/src/index.ts:3033
 msgid "Move Cell Down"
 msgid_plural "Move Cells Down"
 msgstr[0] "Переместить ячейку вниз"
 msgstr[1] "Переместить ячейки вниз"
 msgstr[2] "Переместить ячейки вниз"
 msgstr[3] "Переместить ячейки вниз"
 
-#: packages/notebook-extension/src/index.ts:3011
+#: packages/notebook-extension/src/index.ts:3011 packages/notebook-extension/src/index.ts:3018 packages/notebook-extension/src/index.ts:3041
 msgid "Move this cell down"
 msgid_plural "Move these %1 cells down"
 msgstr[0] "Переместить эту ячейку вниз"
 msgstr[1] "Переместить эти %1 ячейки вниз"
 msgstr[2] "Переместить эти %1 ячеек вниз"
 msgstr[3] "Переместить эти %1 ячеек вниз"
 
-#: packages/notebook-extension/src/index.ts:3023
+#: packages/notebook-extension/src/index.ts:3023 packages/notebook-extension/src/index.ts:3030 packages/notebook-extension/src/index.ts:3053
 msgid "Notebook cell shifted down successfully"
 msgstr "Ячейка блокнота успешно перемещена вниз"
 
-#: packages/notebook-extension/src/index.ts:3064
+#: packages/notebook-extension/src/index.ts:3064 packages/notebook-extension/src/index.ts:3071 packages/notebook-extension/src/index.ts:3094
 msgid "Enter Command Mode"
 msgstr "Войти в режим команд"
 
-#: packages/notebook-extension/src/index.ts:3075
+#: packages/notebook-extension/src/index.ts:3075 packages/notebook-extension/src/index.ts:3082 packages/notebook-extension/src/index.ts:3105
 msgid "Enter Edit Mode"
 msgstr "Войти в режим редактирования"
 
-#: packages/notebook-extension/src/index.ts:3086
+#: packages/notebook-extension/src/index.ts:3086 packages/notebook-extension/src/index.ts:3093 packages/notebook-extension/src/index.ts:3116
 msgid "Undo Cell Operation"
 msgstr "Отменить операцию с ячейкой"
 
-#: packages/notebook-extension/src/index.ts:3097
+#: packages/notebook-extension/src/index.ts:3097 packages/notebook-extension/src/index.ts:3104 packages/notebook-extension/src/index.ts:3127
 msgid "Redo Cell Operation"
 msgstr "Повторить операцию с ячейкой"
 
-#: packages/notebook-extension/src/index.ts:3175
+#: packages/notebook-extension/src/index.ts:3175 packages/notebook-extension/src/index.ts:3182 packages/notebook-extension/src/index.ts:3205
 msgid "Change to Heading 1"
 msgstr "Изменить на Заголовок 1"
 
-#: packages/notebook-extension/src/index.ts:3186
+#: packages/notebook-extension/src/index.ts:3186 packages/notebook-extension/src/index.ts:3193 packages/notebook-extension/src/index.ts:3220
 msgid "Change to Heading 2"
 msgstr "Изменить на Заголовок 2"
 
-#: packages/notebook-extension/src/index.ts:3197
+#: packages/notebook-extension/src/index.ts:3197 packages/notebook-extension/src/index.ts:3204 packages/notebook-extension/src/index.ts:3235
 msgid "Change to Heading 3"
 msgstr "Изменить на Заголовок 3"
 
-#: packages/notebook-extension/src/index.ts:3208
+#: packages/notebook-extension/src/index.ts:3208 packages/notebook-extension/src/index.ts:3215 packages/notebook-extension/src/index.ts:3250
 msgid "Change to Heading 4"
 msgstr "Изменить на Заголовок 4"
 
-#: packages/notebook-extension/src/index.ts:3219
+#: packages/notebook-extension/src/index.ts:3219 packages/notebook-extension/src/index.ts:3226 packages/notebook-extension/src/index.ts:3265
 msgid "Change to Heading 5"
 msgstr "Изменить на Заголовок 5"
 
-#: packages/notebook-extension/src/index.ts:3230
+#: packages/notebook-extension/src/index.ts:3230 packages/notebook-extension/src/index.ts:3237 packages/notebook-extension/src/index.ts:3280
 msgid "Change to Heading 6"
 msgstr "Изменить на Заголовок 6"
 
-#: packages/notebook-extension/src/index.ts:3241
+#: packages/notebook-extension/src/index.ts:3241 packages/notebook-extension/src/index.ts:3248 packages/notebook-extension/src/index.ts:3295
 msgid "Collapse Selected Code"
 msgstr "Свернуть выбранный код"
 
-#: packages/notebook-extension/src/index.ts:3252
+#: packages/notebook-extension/src/index.ts:3252 packages/notebook-extension/src/index.ts:3259 packages/notebook-extension/src/index.ts:3306
 msgid "Expand Selected Code"
 msgstr "Развернуть выбранный код"
 
-#: packages/notebook-extension/src/index.ts:3263
+#: packages/notebook-extension/src/index.ts:3263 packages/notebook-extension/src/index.ts:3270 packages/notebook-extension/src/index.ts:3317
 msgid "Collapse All Code"
 msgstr "Свернуть весь код"
 
-#: packages/notebook-extension/src/index.ts:3274
+#: packages/notebook-extension/src/index.ts:3274 packages/notebook-extension/src/index.ts:3281 packages/notebook-extension/src/index.ts:3328
 msgid "Expand All Code"
 msgstr "Развернуть весь код"
 
-#: packages/notebook-extension/src/index.ts:3285
+#: packages/notebook-extension/src/index.ts:3285 packages/notebook-extension/src/index.ts:3292 packages/notebook-extension/src/index.ts:3339
 msgid "Collapse Selected Outputs"
 msgstr "Свернуть выбранные выходные данные"
 
-#: packages/notebook-extension/src/index.ts:3296
+#: packages/notebook-extension/src/index.ts:3296 packages/notebook-extension/src/index.ts:3303 packages/notebook-extension/src/index.ts:3350
 msgid "Expand Selected Outputs"
 msgstr "Развернуть выбранные выходные данные"
 
-#: packages/notebook-extension/src/index.ts:3307
+#: packages/notebook-extension/src/index.ts:3307 packages/notebook-extension/src/index.ts:3314 packages/notebook-extension/src/index.ts:3361
 msgid "Collapse All Outputs"
 msgstr "Свернуть весь вывод"
 
-#: packages/notebook-extension/src/index.ts:3319
+#: packages/notebook-extension/src/index.ts:3319 packages/notebook-extension/src/index.ts:3326 packages/notebook-extension/src/index.ts:3373
 msgid "Render Side-by-Side"
 msgstr "Рендер бок о бок"
 
-#: packages/notebook-extension/src/index.ts:3341
+#: packages/notebook-extension/src/index.ts:3341 packages/notebook-extension/src/index.ts:3348 packages/notebook-extension/src/index.ts:3395
 msgid "Expand All Outputs"
 msgstr "Развернуть весь вывод"
 
-#: packages/notebook-extension/src/index.ts:3352
+#: packages/notebook-extension/src/index.ts:3352 packages/notebook-extension/src/index.ts:3359 packages/notebook-extension/src/index.ts:3406
 msgid "Enable Scrolling for Outputs"
 msgstr "Включить прокрутку для вывода"
 
-#: packages/notebook-extension/src/index.ts:3363
+#: packages/notebook-extension/src/index.ts:3363 packages/notebook-extension/src/index.ts:3370 packages/notebook-extension/src/index.ts:3417
 msgid "Disable Scrolling for Outputs"
 msgstr "Отключить прокрутку для вывода"
 
-#: packages/notebook-extension/src/index.ts:3374
+#: packages/notebook-extension/src/index.ts:3374 packages/notebook-extension/src/index.ts:3381 packages/notebook-extension/src/index.ts:3428
 msgid "Select current running or last run cell"
 msgstr "Выбрать текущую запущенную или последнюю запущенную ячейку"
 
-#: packages/notebook-extension/src/index.ts:3385
+#: packages/notebook-extension/src/index.ts:3385 packages/notebook-extension/src/index.ts:3392 packages/notebook-extension/src/index.ts:3439
 msgid "Replace Selection in Notebook Cell"
 msgstr "Заменить выделенное в ячейке блокнота"
 
-#: packages/notebook-extension/src/index.ts:3397
+#: packages/notebook-extension/src/index.ts:3397 packages/notebook-extension/src/index.ts:3404 packages/notebook-extension/src/index.ts:3451
 msgid "Toggle Collapse Notebook Heading"
 msgstr "Свернуть заголовок блокнота"
 
-#: packages/notebook-extension/src/index.ts:3407 packages/toc-extension/src/index.ts:141
+#: packages/notebook-extension/src/index.ts:3407 packages/notebook-extension/src/index.ts:3414 packages/notebook-extension/src/index.ts:3461 packages/toc-extension/src/index.ts:141
 msgid "Collapse All Headings"
 msgstr "Свернуть все заголовки"
 
-#: packages/notebook-extension/src/index.ts:3416 packages/toc-extension/src/index.ts:140
+#: packages/notebook-extension/src/index.ts:3416 packages/notebook-extension/src/index.ts:3423 packages/notebook-extension/src/index.ts:3470 packages/toc-extension/src/index.ts:140
 msgid "Expand All Headings"
 msgstr "Развернуть все заголовки"
 
-#: packages/notebook-extension/src/index.ts:3425
+#: packages/notebook-extension/src/index.ts:3425 packages/notebook-extension/src/index.ts:3432 packages/notebook-extension/src/index.ts:3479
 msgid "Select and Run Cell(s) for this Heading"
 msgstr "Выберите и запустите ячейку(и) для этого заголовка"
 
-#: packages/notebook-extension/src/index.ts:3466
+#: packages/notebook-extension/src/index.ts:3466 packages/notebook-extension/src/index.ts:3473 packages/notebook-extension/src/index.ts:3520
 msgid "Access Previous Kernel History Entry"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:3475
+#: packages/notebook-extension/src/index.ts:3475 packages/notebook-extension/src/index.ts:3482 packages/notebook-extension/src/index.ts:3529
 msgid "Access Next Kernel History Entry"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:3484
+#: packages/notebook-extension/src/index.ts:3484 packages/notebook-extension/src/index.ts:3491 packages/notebook-extension/src/index.ts:3539
 msgid "Virtual Scrollbar"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:3485
+#: packages/notebook-extension/src/index.ts:3485 packages/notebook-extension/src/index.ts:3492 packages/notebook-extension/src/index.ts:3540
 msgid "Toggle virtual scrollbar (enabled with windowing mode: full)"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:3519 packages/notebook-extension/src/index.ts:670
+#: packages/notebook-extension/src/index.ts:3519 packages/notebook-extension/src/index.ts:3526 packages/notebook-extension/src/index.ts:3585 packages/notebook-extension/src/index.ts:670 packages/notebook-extension/src/index.ts:674 packages/notebook-extension/src/index.ts:681
 msgid "Notebook Operations"
 msgstr "Операции с блокнотом"
 
-#: packages/notebook-extension/src/index.ts:3557
+#: packages/notebook-extension/src/index.ts:3557 packages/notebook-extension/src/index.ts:3564 packages/notebook-extension/src/index.ts:3623
 msgid "Notebook Cell Operations"
 msgstr "Операции с ячейками блокнота"
 
-#: packages/notebook-extension/src/index.ts:3802
+#: packages/notebook-extension/src/index.ts:3802 packages/notebook-extension/src/index.ts:3809 packages/notebook-extension/src/index.ts:3868
 msgid "PDF"
 msgstr "PDF"
 
-#: packages/notebook-extension/src/index.ts:3803
+#: packages/notebook-extension/src/index.ts:3803 packages/notebook-extension/src/index.ts:3810 packages/notebook-extension/src/index.ts:3869
 msgid "ReStructured Text"
 msgstr "Реструктурированный текст"
 
-#: packages/notebook-extension/src/index.ts:3804
+#: packages/notebook-extension/src/index.ts:3804 packages/notebook-extension/src/index.ts:3811 packages/notebook-extension/src/index.ts:3870
 msgid "Executable Script"
 msgstr "Исполняемый скрипт"
 
-#: packages/notebook-extension/src/index.ts:3805
+#: packages/notebook-extension/src/index.ts:3805 packages/notebook-extension/src/index.ts:3812 packages/notebook-extension/src/index.ts:3871
 msgid "Reveal.js Slides"
 msgstr "Слайды Reveal.js"
 
-#: packages/notebook-extension/src/index.ts:3859
+#: packages/notebook-extension/src/index.ts:3859 packages/notebook-extension/src/index.ts:3866 packages/notebook-extension/src/index.ts:3925
 msgid "For Notebook: %1"
 msgstr "Для Блокнота: %1"
 
-#: packages/notebook-extension/src/index.ts:3860
+#: packages/notebook-extension/src/index.ts:3860 packages/notebook-extension/src/index.ts:3867 packages/notebook-extension/src/index.ts:3926
 msgid "For Notebook:"
 msgstr "Для Блокнота:"
 
-#: packages/notebook-extension/src/index.ts:582
+#: packages/notebook-extension/src/index.ts:582 packages/notebook-extension/src/index.ts:586 packages/notebook-extension/src/index.ts:593
 msgid "Save and Export Notebook to the given `format`."
 msgstr "Сохранить и экспортировать заметки в указанный `format`."
 
-#: packages/notebook-extension/src/index.ts:586
+#: packages/notebook-extension/src/index.ts:586 packages/notebook-extension/src/index.ts:590 packages/notebook-extension/src/index.ts:597
 msgid "Save and Export Notebook: %1"
 msgstr "Сохранить и экспортировать ноутбук как: %1"
 
-#: packages/notebook/src/actions.tsx:2094
+#: packages/notebook/src/actions.tsx:2094 packages/notebook/src/actions.tsx:2099 packages/notebook/src/actions.tsx:2107
 msgid "A trusted Jupyter notebook may execute hidden malicious code when you open it."
 msgstr "Доверенный блокнот Jupyter может выполнить скрытый вредоносный код при открытии."
 
-#: packages/notebook/src/actions.tsx:2098
+#: packages/notebook/src/actions.tsx:2098 packages/notebook/src/actions.tsx:2103 packages/notebook/src/actions.tsx:2111
 msgid "Selecting \"Trust\" will re-render this notebook in a trusted state."
 msgstr "При выборе «Trust» этот блокнот будет повторно отображать в надёжном состоянии."
 
-#: packages/notebook/src/actions.tsx:2102
+#: packages/notebook/src/actions.tsx:2102 packages/notebook/src/actions.tsx:2107 packages/notebook/src/actions.tsx:2115
 msgid "For more information, see"
 msgstr "Дополнительные сведения см. в"
 
-#: packages/notebook/src/actions.tsx:2108
+#: packages/notebook/src/actions.tsx:2108 packages/notebook/src/actions.tsx:2113 packages/notebook/src/actions.tsx:2121
 msgid "the Jupyter security documentation"
 msgstr "документация по безопасности Jupyter"
 
-#: packages/notebook/src/actions.tsx:2116
+#: packages/notebook/src/actions.tsx:2116 packages/notebook/src/actions.tsx:2121 packages/notebook/src/actions.tsx:2129
 msgid "Notebook is already trusted"
 msgstr "Блокнот уже является доверенным"
 
-#: packages/notebook/src/actions.tsx:2123
+#: packages/notebook/src/actions.tsx:2123 packages/notebook/src/actions.tsx:2128 packages/notebook/src/actions.tsx:2136
 msgid "Trust this notebook?"
 msgstr "Доверять этому блокноту?"
 
-#: packages/notebook/src/actions.tsx:2127
+#: packages/notebook/src/actions.tsx:2127 packages/notebook/src/actions.tsx:2132 packages/notebook/src/actions.tsx:2140
 msgid "Trust"
 msgstr "Доверять"
 
-#: packages/notebook/src/actions.tsx:2128
+#: packages/notebook/src/actions.tsx:2128 packages/notebook/src/actions.tsx:2133 packages/notebook/src/actions.tsx:2141
 msgid "Confirm Trusting this notebook"
 msgstr "Подтвердите доверие этому блокноту"
 
-#: packages/notebook/src/actions.tsx:2488
+#: packages/notebook/src/actions.tsx:2488 packages/notebook/src/actions.tsx:2493 packages/notebook/src/cellexecutor.ts:46
 msgid "Kernel Terminating"
 msgstr "Завершение ядра"
 
-#: packages/notebook/src/actions.tsx:2489
+#: packages/notebook/src/actions.tsx:2489 packages/notebook/src/actions.tsx:2494 packages/notebook/src/cellexecutor.ts:47
 msgid "The kernel for %1 appears to be terminating. You can not run any cell for now."
 msgstr "Похоже, что ядро %1 завершается. Сейчас вы не можете запускать ячейки."
 
-#: packages/notebook/src/actions.tsx:2499
+#: packages/notebook/src/actions.tsx:2499 packages/notebook/src/actions.tsx:2504 packages/notebook/src/cellexecutor.ts:57
 msgid "Cell not executed due to pending input"
 msgstr "Ячейка не выполняется из-за незавершенного ввода"
 
-#: packages/notebook/src/actions.tsx:2500
+#: packages/notebook/src/actions.tsx:2500 packages/notebook/src/actions.tsx:2505 packages/notebook/src/cellexecutor.ts:58
 msgid "The cell has not been executed to avoid kernel deadlock as there is another pending input! Submit your pending input and try again."
 msgstr "Ячейка не был выполнена, чтобы избежать блокировки ядра, так как есть еще один ожидающий вход! Отправьте ваш ввод и повторите попытку."
 
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
 msgstr "Вырезать выбранные ячейки"
 
 #: packages/notebook/src/default-toolbar.tsx:161
 msgid "Copy the selected cells"
 msgstr "Скопировать выбранные ячейки"
@@ -6822,15 +7004,15 @@
 msgid "Notebook converted"
 msgstr "Блокнот преобразован"
 
 #: packages/notebook/src/modestatus.tsx:29
 msgid "Mode: %1"
 msgstr "Режим: %1"
 
-#: packages/notebook/src/modestatus.tsx:71 packages/shortcuts-extension/src/components/TopNav.tsx:182
+#: packages/notebook/src/modestatus.tsx:71 packages/shortcuts-extension/src/components/TopNav.tsx:130 packages/shortcuts-extension/src/components/TopNav.tsx:182
 msgid "Command"
 msgstr "Команда"
 
 #: packages/notebook/src/modestatus.tsx:72 packages/shortcuts-extension/src/components/ShortcutItem.tsx:61
 msgid "Edit"
 msgstr "Редактировать"
 
@@ -6846,67 +7028,75 @@
 msgid "Kernel Restarting"
 msgstr "Перезапуск ядра"
 
 #: packages/notebook/src/panel.ts:224
 msgid "The kernel for %1 appears to have died. It will restart automatically."
 msgstr "Похоже, что ядро %1 не запущено. Оно будет перезапущено автоматически."
 
-#: packages/notebook/src/searchprovider.ts:237
+#: packages/notebook/src/searchprovider.ts:234 packages/notebook/src/searchprovider.ts:237
 msgid "Search Cell Outputs"
 msgstr "Поиск выходных данных ячеек"
 
-#: packages/notebook/src/searchprovider.ts:238
+#: packages/notebook/src/searchprovider.ts:235 packages/notebook/src/searchprovider.ts:238
 msgid "Search in the cell outputs."
 msgstr "Поиск в выходе ячейки."
 
-#: packages/notebook/src/searchprovider.ts:245
+#: packages/notebook/src/searchprovider.ts:236
+msgid "Search in the cell outputs (not available when replace options are shown)."
+msgstr ""
+
+#: packages/notebook/src/searchprovider.ts:242 packages/notebook/src/searchprovider.ts:245
 msgid "Search in %1 Selected Cell"
 msgid_plural "Search in %1 Selected Cells"
 msgstr[0] "Поиск в %1 выбранной ячейке"
 msgstr[1] "Поиск в %1 выбранных ячейках"
 msgstr[2] "Поиск в %1 выбранных ячейках"
 msgstr[3] "Поиск в %1 выбранных ячейках"
 
-#: packages/notebook/src/searchprovider.ts:250
+#: packages/notebook/src/searchprovider.ts:247 packages/notebook/src/searchprovider.ts:250
 msgid "Search in %1 Selected Line"
 msgid_plural "Search in %1 Selected Lines"
 msgstr[0] "Искать в %1 выбранной строке"
 msgstr[1] "Искать в %1 выбранных строках"
 msgstr[2] "Искать в %1 выбранных строках"
 msgstr[3] "Искать в %1 выбранных строках"
 
-#: packages/notebook/src/searchprovider.ts:255
+#: packages/notebook/src/searchprovider.ts:252 packages/notebook/src/searchprovider.ts:255
 msgid "Search only in the selected cells or text (depending on edit/command mode)."
 msgstr "Искать только в выбранных ячейках или тексте (в зависимости от режима редактирования/команды)."
 
-#: packages/notebook/src/searchprovider.ts:523
+#: packages/notebook/src/searchprovider.ts:512 packages/notebook/src/searchprovider.ts:523
 msgid "Searching outputs is expensive and requires to first rendered all outputs. Are you sure you want to search in the cell outputs?"
 msgstr "Поиск результатов является дорогостоящим и требует первого рендеринга всех выводов. Вы уверены, что хотите найти данные в выводах?"
 
+#: packages/notebook/src/searchprovider.ts:515
+msgid "Searching outputs requires you to run all cells and render their outputs. Are you sure you want to search in the cell outputs?"
+msgstr ""
+
 #: packages/notebook/src/truststatus.tsx:30
 msgid "Notebook trusted: %1 of %2 code cells trusted."
 msgstr "Блокнот является доверенным: %1 из %2 ячеек кода являются доверенными."
 
 #: packages/notebook/src/truststatus.tsx:36
 msgid "Active cell trusted: %1 of %2 code cells trusted."
 msgstr "Активная ячейка является доверенной: %1 из %2 ячеек кода являются доверенными."
 
 #: packages/notebook/src/truststatus.tsx:42
 msgid "Notebook not trusted: %1 of %2 code cells trusted."
 msgstr "Блокнот не является доверенным: %1 из %2 ячеек кода являются доверенными."
 
-#: packages/notebook/src/widget.ts:444
+#: packages/notebook/src/widget.ts:444 packages/notebook/src/widget.ts:453 packages/notebook/src/widget.ts:470
 msgid "The notebook is empty. Click the + button on the toolbar to add a new cell."
 msgstr "Блокнот пуст. Нажмите кнопку +, чтобы добавить новую ячейку."
 
-#: packages/outputarea/src/widget.ts:1096
+#: packages/outputarea/src/widget.ts:1096 packages/outputarea/src/widget.ts:1097 packages/outputarea/src/widget.ts:1128
 msgid "↑↓ for history. Search history with c-↑/c-↓"
 msgstr "↑↓ для истории. Поиск истории с c-↑/c-↓"
 
-#: packages/outputarea/src/widget.ts:640
+#: packages/outputarea/src/widget.ts:640 packages/outputarea/src/widget.ts:662
 msgid "Javascript Error: %1"
 msgstr "Ошибка Javascript: %1"
 
 #: packages/pluginmanager-extension/src/index.ts:100 packages/pluginmanager-extension/src/index.ts:64 packages/settingeditor-extension/src/index.ts:154
 msgid "Plugin Manager"
 msgstr ""
 
@@ -7026,72 +7216,132 @@
 msgid "Handle Local Link"
 msgstr "Обработка локальной ссылки"
 
 #: packages/rendermime/src/renderers.ts:62
 msgid "This HTML output contains inline scripts. Are you sure that you want to run arbitrary Javascript within your JupyterLab session?"
 msgstr "Этот HTML-вывод содержит встроенные скрипты. Вы уверены, что хотите запустить произвольный Javascript в вашей сессии JupyterLab?"
 
-#: packages/rendermime/src/widgets.ts:464
+#: packages/rendermime/src/widgets.ts:464 packages/rendermime/src/widgets.ts:492
 msgid "JavaScript output is disabled in JupyterLab"
 msgstr "Вывод JavaScript отключен в JupyterLab"
 
-#: packages/running-extension/src/index.ts:66
-msgid "Running Terminals and Kernels"
-msgstr "Запущенные терминалы и ядра"
-
-#: packages/running-extension/src/index.ts:69
+#: packages/running-extension/src/index.ts:101 packages/running-extension/src/index.ts:69
 msgid "Running Sessions section"
 msgstr "Раздел \"Запуск сессий\""
 
-#: packages/running-extension/src/index.ts:86
+#: packages/running-extension/src/index.ts:115 packages/running-extension/src/index.ts:86
 msgid "Sessions and Tabs"
 msgstr "Сессии и вкладки"
 
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
+msgstr "Запущенные терминалы и ядра"
+
+#: packages/running-extension/src/kernels.ts:107 packages/running-extension/src/kernels.tsx:128
 msgid "Unknown Session"
 msgstr "Неизвестная сессия"
 
-#: packages/running-extension/src/kernels.ts:250
+#: packages/running-extension/src/kernels.ts:250 packages/running-extension/src/kernels.tsx:320
 msgid "%1\n"
 "Path: %2"
 msgstr "%1\n"
 "Путь: %2"
 
-#: packages/running-extension/src/kernels.ts:49
+#: packages/running-extension/src/kernels.ts:49 packages/running-extension/src/kernels.tsx:54
 msgid "Kernels"
 msgstr "Ядра"
 
-#: packages/running-extension/src/kernels.ts:68
+#: packages/running-extension/src/kernels.ts:68 packages/running-extension/src/kernels.tsx:88
 msgid "Are you sure you want to permanently shut down all running kernels?"
 msgstr "Вы уверены, что хотите навсегда выключить все запущенные ядра?"
 
-#: packages/running-extension/src/kernels.ts:77
+#: packages/running-extension/src/kernels.ts:77 packages/running-extension/src/kernels.tsx:98
 msgid "New Console for Kernel"
 msgstr "Новая консоль для ядра"
 
-#: packages/running-extension/src/kernels.ts:88
+#: packages/running-extension/src/kernels.ts:88 packages/running-extension/src/kernels.tsx:109
 msgid "New Notebook for Kernel"
 msgstr "Новый блокнот для ядра"
 
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
 msgstr "Открытые вкладки"
 
 #: packages/running-extension/src/opentabs.ts:87
 msgid "Close All"
 msgstr "Закрыть все"
 
 #: packages/running-extension/src/opentabs.ts:88
 msgid "Are you sure you want to close all open tabs?"
 msgstr "Вы уверены, что хотите закрыть все открытые вкладки?"
 
-#: packages/running/src/index.tsx:445
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
 msgstr "Обновить список"
 
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
 #: packages/settingeditor-extension/src/index.ts:165
 msgid "JSON Settings Editor"
 msgstr "Настройка редактора JSON"
 
 #: packages/settingeditor-extension/src/index.ts:172 packages/settingeditor-extension/src/index.ts:207 packages/settingeditor-extension/src/index.ts:339 packages/settingeditor/src/pluginlist.tsx:467
 msgid "Settings"
 msgstr "Настройки"
@@ -7168,18 +7418,14 @@
 msgid "Your changes were not saved."
 msgstr "Ваши изменения не были сохранены."
 
 #: packages/settingeditor/src/pluginlist.tsx:454
 msgid "Search settings…"
 msgstr ""
 
-#: packages/settingeditor/src/pluginlist.tsx:461
-msgid "Modified"
-msgstr "Изменён"
-
 #: packages/settingeditor/src/pluginlist.tsx:473
 msgid "No items match your search."
 msgstr "По вашему запросу нет результатов."
 
 #: packages/settingeditor/src/raweditor.ts:368
 msgid "System Defaults"
 msgstr "Настройки по умолчанию"
@@ -7192,31 +7438,43 @@
 msgid "Unsaved changes due to validation error. Continue without saving?"
 msgstr "Несохраненные изменения из-за ошибки проверки. Продолжить без сохранения?"
 
 #: packages/settingeditor/src/settingseditor.tsx:135
 msgid "Some changes have not been saved. Continue without saving?"
 msgstr "Некоторые изменения не были сохранены. Продолжить без сохранения?"
 
-#: packages/shortcuts-extension/src/components/ShortcutInput.tsx:445
+#: packages/shortcuts-extension/src/components/ShortcutInput.tsx:389 packages/shortcuts-extension/src/components/ShortcutInput.tsx:445 packages/shortcuts-extension/src/components/ShortcutInput.tsx:446
 msgid "press keys"
 msgstr "нажмите клавиши"
 
-#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:218
-msgid "Shortcut already in use by %1. Overwrite it?"
-msgstr "Ярлык уже используется %1. Перезаписать его?"
+#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:123
+msgid "(Command label missing)"
+msgstr ""
 
-#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:260 packages/shortcuts-extension/src/components/ShortcutItem.tsx:76
+#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:135 packages/shortcuts-extension/src/components/ShortcutItem.tsx:260 packages/shortcuts-extension/src/components/ShortcutItem.tsx:76 packages/workspaces-extension/src/commands.ts:327
 msgid "Reset"
 msgstr "Сброс"
 
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
 msgstr "или"
 
-#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:416 packages/shortcuts-extension/src/components/ShortcutItem.tsx:66 packages/shortcuts-extension/src/components/ShortcutItem.tsx:71 packages/ui-components/src/components/form.tsx:212
+#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:218 packages/shortcuts-extension/src/components/ShortcutItem.tsx:333
+msgid "Shortcut already in use by %1. Overwrite it?"
+msgstr "Ярлык уже используется %1. Перезаписать его?"
+
+#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:266 packages/shortcuts-extension/src/components/ShortcutItem.tsx:416 packages/shortcuts-extension/src/components/ShortcutItem.tsx:66 packages/shortcuts-extension/src/components/ShortcutItem.tsx:71 packages/ui-components/src/components/form.tsx:212
 msgid "Add"
 msgstr "Добавить"
 
 #: packages/shortcuts-extension/src/components/ShortcutItem.tsx:51
 msgid "Edit First"
 msgstr "Изменить первым"
 
@@ -7236,59 +7494,83 @@
 msgid "Add another shortcut"
 msgstr "Добавить другой ярлык"
 
 #: packages/shortcuts-extension/src/components/ShortcutItem.tsx:77
 msgid "Reset shortcut back to default"
 msgstr "Сбросить ярлыки до значений по умолчанию"
 
-#: packages/shortcuts-extension/src/components/TopNav.tsx:126
-msgid "Toggle Selectors"
-msgstr "Переключить селекторы"
-
-#: packages/shortcuts-extension/src/components/TopNav.tsx:127
-msgid "Toggle command selectors"
-msgstr "Переключить селекторы команд"
-
-#: packages/shortcuts-extension/src/components/TopNav.tsx:136 packages/shortcuts-extension/src/components/TopNav.tsx:92
-msgid "Reset All"
-msgstr "Сбросить все"
-
-#: packages/shortcuts-extension/src/components/TopNav.tsx:137
-msgid "Reset all shortcuts"
-msgstr "Сбросить все сочетания клавиш"
-
-#: packages/shortcuts-extension/src/components/TopNav.tsx:165
+#: packages/shortcuts-extension/src/components/TopNav.tsx:113 packages/shortcuts-extension/src/components/TopNav.tsx:165
 msgid "Search shortcuts"
 msgstr ""
 
-#: packages/shortcuts-extension/src/components/TopNav.tsx:168
+#: packages/shortcuts-extension/src/components/TopNav.tsx:117 packages/shortcuts-extension/src/components/TopNav.tsx:168
 msgid "Search…"
 msgstr "Поиск…"
 
-#: packages/shortcuts-extension/src/components/TopNav.tsx:181
+#: packages/shortcuts-extension/src/components/TopNav.tsx:126 packages/shortcuts-extension/src/index.ts:159
+msgid "Toggle Selectors"
+msgstr "Переключить селекторы"
+
+#: packages/shortcuts-extension/src/components/TopNav.tsx:127 packages/shortcuts-extension/src/index.ts:160
+msgid "Toggle command selectors"
+msgstr "Переключить селекторы команд"
+
+#: packages/shortcuts-extension/src/components/TopNav.tsx:129 packages/shortcuts-extension/src/components/TopNav.tsx:181
 msgid "Category"
 msgstr "Категория"
 
-#: packages/shortcuts-extension/src/components/TopNav.tsx:184
+#: packages/shortcuts-extension/src/components/TopNav.tsx:132 packages/shortcuts-extension/src/components/TopNav.tsx:184
 msgid "Shortcut"
 msgstr "Ярлык"
 
-#: packages/shortcuts-extension/src/components/TopNav.tsx:188
+#: packages/shortcuts-extension/src/components/TopNav.tsx:136 packages/shortcuts-extension/src/components/TopNav.tsx:188
 msgid "Selectors"
 msgstr "Селекторы"
 
-#: packages/shortcuts-extension/src/components/TopNav.tsx:85
+#: packages/shortcuts-extension/src/components/TopNav.tsx:136 packages/shortcuts-extension/src/components/TopNav.tsx:69 packages/shortcuts-extension/src/components/TopNav.tsx:92 packages/shortcuts-extension/src/index.ts:169
+msgid "Reset All"
+msgstr "Сбросить все"
+
+#: packages/shortcuts-extension/src/components/TopNav.tsx:137 packages/shortcuts-extension/src/index.ts:170
+msgid "Reset all shortcuts"
+msgstr "Сбросить все сочетания клавиш"
+
+#: packages/shortcuts-extension/src/components/TopNav.tsx:62 packages/shortcuts-extension/src/components/TopNav.tsx:85
 msgid "Hide Selectors"
 msgstr "Скрыть селекторы"
 
-#: packages/shortcuts-extension/src/components/TopNav.tsx:86
+#: packages/shortcuts-extension/src/components/TopNav.tsx:63 packages/shortcuts-extension/src/components/TopNav.tsx:86
 msgid "Show Selectors"
 msgstr "Показать селекторы"
 
-#: packages/shortcuts-extension/src/index.ts:152
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
+#: packages/shortcuts-extension/src/index.ts:143
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
@@ -7393,14 +7675,18 @@
 msgid "Terminal %1"
 msgstr "Терминал %1"
 
 #: packages/theme-dark-extension/src/index.ts:31
 msgid "JupyterLab Dark"
 msgstr "Тёмная JupyterLab"
 
+#: packages/theme-dark-high-contrast-extension/src/index.ts:31
+msgid "JupyterLab Dark High Contrast"
+msgstr ""
+
 #: packages/theme-light-extension/src/index.ts:31
 msgid "JupyterLab Light"
 msgstr "Светлая JupyterLab"
 
 #: packages/toc-extension/src/index.ts:113
 msgid "Show output headings"
 msgstr "Показать выводимые заголовки"
@@ -7477,19 +7763,179 @@
 msgid "side panel actions"
 msgstr "действия боковой панели"
 
 #: packages/ui-components/src/components/sidepanel.ts:41
 msgid "side panel content"
 msgstr "контент боковой панели"
 
-#: packages/ui-components/src/components/toolbar.tsx:1140
+#: packages/ui-components/src/components/toolbar.tsx:1140 packages/ui-components/src/components/toolbar.tsx:1180 packages/ui-components/src/components/toolbar.tsx:1191 packages/ui-components/src/components/toolbar.tsx:1192
 msgid "More commands"
 msgstr "Больше команд"
 
 #: packages/ui-components/src/icon/widgets/tabbarsvg.ts:51
 msgid "Close %1"
 msgstr "Выполнить закрытие %1"
 
 #: packages/ui-components/src/icon/widgets/tabbarsvg.ts:52
 msgid "Close tab"
 msgstr "Закрыть вкладку"
 
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
+msgstr[3] ""
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

### Comparing `jupyterlab_language_pack_ru_ru-4.1.post2/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyterlab_git.po` & `jupyterlab_language_pack_ru_ru-4.2.post0/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyterlab_git.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ru_ru-4.1.post2/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyterlab_lsp.po` & `jupyterlab_language_pack_ru_ru-4.2.post0/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyterlab_lsp.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ru_ru-4.1.post2/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyterlab_recents.po` & `jupyterlab_language_pack_ru_ru-4.2.post0/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyterlab_recents.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ru_ru-4.1.post2/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyterlab_search_replace.po` & `jupyterlab_language_pack_ru_ru-4.2.post0/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyterlab_search_replace.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ru_ru-4.1.post2/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyterlab_spreadsheet_editor.po` & `jupyterlab_language_pack_ru_ru-4.2.post0/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyterlab_spreadsheet_editor.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ru_ru-4.1.post2/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyterlab_tour.po` & `jupyterlab_language_pack_ru_ru-4.2.post0/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyterlab_tour.po`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 "X-Crowdin-Project: jupyterlab\n"
 "X-Crowdin-Project-ID: 409874\n"
 "X-Crowdin-Language: ru\n"
 "X-Crowdin-File: /main/extensions/jupyterlab_tour/locale/jupyterlab_tour.pot\n"
 "X-Crowdin-File-ID: 205\n"
 "Language-Team: Russian\n"
 "Language: ru_RU\n"
-"PO-Revision-Date: 2023-11-09 13:39\n"
+"PO-Revision-Date: 2024-03-29 11:18\n"
 
 #: /schema/user-tours.json:/description
 msgctxt "schema"
 msgid "Configuration for user-defined tours. This schema is generated from https://github.com/gilbarbara/react-joyride/blob/master/types/index.d.ts"
 msgstr "Конфигурация для определенных пользователем туров. Эта схема генерируется из https://github.com/gilbarbara/react-joyride/blob/master/types/index.d.ts"
 
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
 msgstr "Не удалось добавить тур '%1' (%2)"
 
 #: src/tourManager.ts:172
 msgid "Error creating new tour. TourHandler id's must be unique.\n"
 "Tutorial with the id: '%1' already exists."
```

### Comparing `jupyterlab_language_pack_ru_ru-4.1.post2/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyterlab_widgets.po` & `jupyterlab_language_pack_ru_ru-4.2.post0/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupyterlab_widgets.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ru_ru-4.1.post2/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupytext.po` & `jupyterlab_language_pack_ru_ru-4.2.post0/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/jupytext.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ru_ru-4.1.post2/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/nbdime.po` & `jupyterlab_language_pack_ru_ru-4.2.post0/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/nbdime.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ru_ru-4.1.post2/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/notebook.po` & `jupyterlab_language_pack_ru_ru-4.2.post0/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/notebook.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ru_ru-4.1.post2/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/retrolab.po` & `jupyterlab_language_pack_ru_ru-4.2.post0/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/retrolab.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ru_ru-4.1.post2/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/spellchecker.po` & `jupyterlab_language_pack_ru_ru-4.2.post0/jupyterlab_language_pack_ru_RU/locale/ru_RU/LC_MESSAGES/spellchecker.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ru_ru-4.1.post2/.gitignore` & `jupyterlab_language_pack_ru_ru-4.2.post0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ru_ru-4.1.post2/LICENSE.txt` & `jupyterlab_language_pack_ru_ru-4.2.post0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ru_ru-4.1.post2/pyproject.toml` & `jupyterlab_language_pack_ru_ru-4.2.post0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ru_ru-4.1.post2/PKG-INFO` & `jupyterlab_language_pack_ru_ru-4.2.post0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyterlab-language-pack-ru-RU
-Version: 4.1.post2
+Version: 4.2.post0
 Summary: JupyterLab Russian (Russia) Language Pack
 Project-URL: homepage, https://github.com/jupyterlab/language-packs
 Author-email: Project Jupyter Contributors <jupyter@googlegroups.com>
 License: Copyright (c) 2023 Project Jupyter Contributors
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

