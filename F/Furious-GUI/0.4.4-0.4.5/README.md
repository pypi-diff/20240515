# Comparing `tmp/Furious-GUI-0.4.4.tar.gz` & `tmp/Furious-GUI-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Furious-GUI-0.4.4.tar", last modified: Mon May 13 14:25:46 2024, max compression
+gzip compressed data, was "Furious-GUI-0.4.5.tar", last modified: Wed May 15 05:15:52 2024, max compression
```

## Comparing `Furious-GUI-0.4.4.tar` & `Furious-GUI-0.4.5.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:25:46.540198 Furious-GUI-0.4.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:25:46.484198 Furious-GUI-0.4.4/Furious/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:25:46.488198 Furious-GUI-0.4.4/Furious/Core/
--rw-r--r--   0 runner    (1001) docker     (127)    16625 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Core/CoreManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Core/Hysteria1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Core/Hysteria2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Core/Tun2socks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Core/XrayCore.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:25:46.484198 Furious-GUI-0.4.4/Furious/Data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:25:46.488198 Furious-GUI-0.4.4/Furious/Data/font/
--rw-r--r--   0 runner    (1001) docker     (127)   624892 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Data/font/CascadiaMono
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Data/font/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:25:46.492198 Furious-GUI-0.4.4/Furious/Data/hysteria/
--rw-r--r--   0 runner    (1001) docker     (127)  1974430 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Data/hysteria/bypass-Iran.acl
--rw-r--r--   0 runner    (1001) docker     (127)  1390176 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Data/hysteria/bypass-mainland-China.acl
--rw-r--r--   0 runner    (1001) docker     (127)  6444374 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Data/hysteria/country.mmdb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:25:46.520198 Furious-GUI-0.4.4/Furious/Data/xray/
--rw-r--r--   0 runner    (1001) docker     (127) 10715744 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Data/xray/geoip.dat
--rw-r--r--   0 runner    (1001) docker     (127)  6057957 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Data/xray/geosite.dat
--rw-r--r--   0 runner    (1001) docker     (127)  3199463 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Data/xray/iran.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:25:46.524198 Furious-GUI-0.4.4/Furious/Externals/
--rw-r--r--   0 runner    (1001) docker     (127)    40204 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Externals/GenTranslation.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Externals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:25:46.528198 Furious-GUI-0.4.4/Furious/Interface/
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Interface/Application.py
--rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Interface/ConfigurationFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Interface/CoreFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Interface/Encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Interface/GuiEditorItemFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Interface/ItemUpdateProtocol.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Interface/Storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Interface/UserServersTableItem.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:25:46.528198 Furious-GUI-0.4.4/Furious/Library/
--rw-r--r--   0 runner    (1001) docker     (127)    55774 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Library/Configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Library/EmptyFactoryHelper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Library/Encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Library/Tcping.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:25:46.528198 Furious-GUI-0.4.4/Furious/PyFramework/
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/PyFramework/Ancestors.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/PyFramework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:25:46.532198 Furious-GUI-0.4.4/Furious/QtFramework/
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/QtFramework/Ancestors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/QtFramework/CoreProcess.py
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/QtFramework/DNSResolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/QtFramework/DynamicTheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/QtFramework/DynamicTranslate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11381 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/QtFramework/GuiEditorXXX.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/QtFramework/NetworkStateManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/QtFramework/QtGui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/QtFramework/QtNetwork.py
--rw-r--r--   0 runner    (1001) docker     (127)    16523 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/QtFramework/QtWidgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     9416 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/QtFramework/TextEditor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/QtFramework/TextEditorTheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/QtFramework/UpdatesManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/QtFramework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:25:46.532198 Furious-GUI-0.4.4/Furious/Storage/
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Storage/UserServers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Storage/UserSubs.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:25:46.532198 Furious-GUI-0.4.4/Furious/TrayActions/
--rw-r--r--   0 runner    (1001) docker     (127)    10277 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/TrayActions/Connect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/TrayActions/EditConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/TrayActions/Exit.py
--rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/TrayActions/Import.py
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/TrayActions/Language.py
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/TrayActions/Routing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/TrayActions/Settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/TrayActions/SystemProxy.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/TrayActions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:25:46.536198 Furious-GUI-0.4.4/Furious/Utility/
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Utility/AppMainProcess.py
--rw-r--r--   0 runner    (1001) docker     (127)    80238 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Utility/AppResources.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Utility/AppSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Utility/AppSettingsFn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Utility/Constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Utility/PySide6Legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Utility/StartupOnBoot.py
--rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Utility/SystemProxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    15978 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Utility/SystemRoutingTable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Utility/SystemRuntime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Utility/Utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:25:46.536198 Furious-GUI-0.4.4/Furious/Widget/
--rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Widget/Application.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Widget/ConnectProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (127)     9602 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Widget/GuiHysteria1.py
--rw-r--r--   0 runner    (1001) docker     (127)    13476 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Widget/GuiHysteria2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Widget/GuiShadowsocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Widget/GuiTrojan.py
--rw-r--r--   0 runner    (1001) docker     (127)     9638 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Widget/GuiVLESS.py
--rw-r--r--   0 runner    (1001) docker     (127)     9578 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Widget/GuiVMess.py
--rw-r--r--   0 runner    (1001) docker     (127)    16043 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Widget/GuiVTLS.py
--rw-r--r--   0 runner    (1001) docker     (127)    32650 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Widget/GuiVTransport.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Widget/IndentSpinBox.py
--rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Widget/SystemTrayIcon.py
--rw-r--r--   0 runner    (1001) docker     (127)    50832 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Widget/UserServersQTableWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Widget/UserSubsQTableWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Widget/XrayAssetViewerQListWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Widget/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:25:46.540198 Furious-GUI-0.4.4/Furious/Window/
--rw-r--r--   0 runner    (1001) docker     (127)    15068 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Window/AppMainWindow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Window/LogViewerWindow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Window/QRCodeWindow.py
--rw-r--r--   0 runner    (1001) docker     (127)    14571 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Window/TextEditorWindow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Window/UserSubsWindow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Window/XrayAssetViewerWindow.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/Window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/Furious/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:25:46.540198 Furious-GUI-0.4.4/Furious_GUI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-13 14:25:46.000000 Furious-GUI-0.4.4/Furious_GUI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-05-13 14:25:46.000000 Furious-GUI-0.4.4/Furious_GUI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 14:25:46.000000 Furious-GUI-0.4.4/Furious_GUI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-13 14:25:46.000000 Furious-GUI-0.4.4/Furious_GUI.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-13 14:25:46.000000 Furious-GUI-0.4.4/Furious_GUI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-13 14:25:46.000000 Furious-GUI-0.4.4/Furious_GUI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-13 14:25:46.540198 Furious-GUI-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 14:25:46.540198 Furious-GUI-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-13 14:25:11.000000 Furious-GUI-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:15:52.299387 Furious-GUI-0.4.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:15:52.251387 Furious-GUI-0.4.5/Furious/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:15:52.251387 Furious-GUI-0.4.5/Furious/Core/
+-rw-r--r--   0 runner    (1001) docker     (127)    16625 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Core/CoreManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Core/Hysteria1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Core/Hysteria2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Core/Tun2socks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Core/XrayCore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:15:52.247387 Furious-GUI-0.4.5/Furious/Data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:15:52.251387 Furious-GUI-0.4.5/Furious/Data/font/
+-rw-r--r--   0 runner    (1001) docker     (127)   624892 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Data/font/CascadiaMono
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Data/font/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:15:52.255386 Furious-GUI-0.4.5/Furious/Data/hysteria/
+-rw-r--r--   0 runner    (1001) docker     (127)  1974430 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Data/hysteria/bypass-Iran.acl
+-rw-r--r--   0 runner    (1001) docker     (127)  1390176 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Data/hysteria/bypass-mainland-China.acl
+-rw-r--r--   0 runner    (1001) docker     (127)  6444374 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Data/hysteria/country.mmdb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:15:52.283387 Furious-GUI-0.4.5/Furious/Data/xray/
+-rw-r--r--   0 runner    (1001) docker     (127) 10715744 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Data/xray/geoip.dat
+-rw-r--r--   0 runner    (1001) docker     (127)  6057957 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Data/xray/geosite.dat
+-rw-r--r--   0 runner    (1001) docker     (127)  3199463 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Data/xray/iran.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:15:52.287387 Furious-GUI-0.4.5/Furious/Externals/
+-rw-r--r--   0 runner    (1001) docker     (127)    40204 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Externals/GenTranslation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Externals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:15:52.291386 Furious-GUI-0.4.5/Furious/Interface/
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Interface/Application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Interface/ConfigurationFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Interface/CoreFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Interface/Encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Interface/GuiEditorItemFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Interface/ItemUpdateProtocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Interface/Storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Interface/UserServersTableItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:15:52.291386 Furious-GUI-0.4.5/Furious/Library/
+-rw-r--r--   0 runner    (1001) docker     (127)    55774 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Library/Configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Library/EmptyFactoryHelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Library/Encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Library/Tcping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:15:52.291386 Furious-GUI-0.4.5/Furious/PyFramework/
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/PyFramework/Ancestors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/PyFramework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:15:52.291386 Furious-GUI-0.4.5/Furious/QtFramework/
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/QtFramework/Ancestors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/QtFramework/CoreProcess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/QtFramework/DNSResolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/QtFramework/DynamicTheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/QtFramework/DynamicTranslate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11381 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/QtFramework/GuiEditorXXX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/QtFramework/NetworkStateManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/QtFramework/QtGui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/QtFramework/QtNetwork.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16523 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/QtFramework/QtWidgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9416 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/QtFramework/TextEditor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/QtFramework/TextEditorTheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/QtFramework/UpdatesManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/QtFramework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:15:52.291386 Furious-GUI-0.4.5/Furious/Storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Storage/UserServers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Storage/UserSubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:15:52.295387 Furious-GUI-0.4.5/Furious/TrayActions/
+-rw-r--r--   0 runner    (1001) docker     (127)    10277 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/TrayActions/Connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/TrayActions/EditConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/TrayActions/Exit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/TrayActions/Import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/TrayActions/Language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/TrayActions/Routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/TrayActions/Settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/TrayActions/SystemProxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/TrayActions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:15:52.295387 Furious-GUI-0.4.5/Furious/Utility/
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Utility/AppMainProcess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80238 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Utility/AppResources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Utility/AppSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Utility/AppSettingsFn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Utility/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Utility/PySide6Legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Utility/StartupOnBoot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Utility/SystemProxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15978 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Utility/SystemRoutingTable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Utility/SystemRuntime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Utility/Utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:15:52.299387 Furious-GUI-0.4.5/Furious/Widget/
+-rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Widget/Application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Widget/ConnectProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9602 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Widget/GuiHysteria1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13476 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Widget/GuiHysteria2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Widget/GuiShadowsocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Widget/GuiTrojan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9638 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Widget/GuiVLESS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9578 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Widget/GuiVMess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16043 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Widget/GuiVTLS.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32650 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Widget/GuiVTransport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Widget/IndentSpinBox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Widget/SystemTrayIcon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50832 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Widget/UserServersQTableWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7979 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Widget/UserSubsQTableWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Widget/XrayAssetViewerQListWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Widget/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:15:52.299387 Furious-GUI-0.4.5/Furious/Window/
+-rw-r--r--   0 runner    (1001) docker     (127)    15068 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Window/AppMainWindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Window/LogViewerWindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Window/QRCodeWindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14571 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Window/TextEditorWindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Window/UserSubsWindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Window/XrayAssetViewerWindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:15:52.299387 Furious-GUI-0.4.5/Furious_GUI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-15 05:15:52.000000 Furious-GUI-0.4.5/Furious_GUI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-05-15 05:15:52.000000 Furious-GUI-0.4.5/Furious_GUI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 05:15:52.000000 Furious-GUI-0.4.5/Furious_GUI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-15 05:15:52.000000 Furious-GUI-0.4.5/Furious_GUI.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-15 05:15:52.000000 Furious-GUI-0.4.5/Furious_GUI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 05:15:52.000000 Furious-GUI-0.4.5/Furious_GUI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-15 05:15:52.299387 Furious-GUI-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 05:15:52.299387 Furious-GUI-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/setup.py
```

### Comparing `Furious-GUI-0.4.4/Furious/Core/CoreManager.py` & `Furious-GUI-0.4.5/Furious/Core/CoreManager.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Core/Hysteria1.py` & `Furious-GUI-0.4.5/Furious/Core/Hysteria1.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Core/Hysteria2.py` & `Furious-GUI-0.4.5/Furious/Core/Hysteria2.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Core/Tun2socks.py` & `Furious-GUI-0.4.5/Furious/Core/Tun2socks.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Core/XrayCore.py` & `Furious-GUI-0.4.5/Furious/Core/XrayCore.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Core/__init__.py` & `Furious-GUI-0.4.5/Furious/Core/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Data/font/CascadiaMono` & `Furious-GUI-0.4.5/Furious/Data/font/CascadiaMono`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Data/font/LICENSE` & `Furious-GUI-0.4.5/Furious/Data/font/LICENSE`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Data/hysteria/bypass-Iran.acl` & `Furious-GUI-0.4.5/Furious/Data/hysteria/bypass-Iran.acl`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Data/hysteria/bypass-mainland-China.acl` & `Furious-GUI-0.4.5/Furious/Data/hysteria/bypass-mainland-China.acl`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Data/hysteria/country.mmdb` & `Furious-GUI-0.4.5/Furious/Data/hysteria/country.mmdb`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Data/xray/geoip.dat` & `Furious-GUI-0.4.5/Furious/Data/xray/geoip.dat`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Data/xray/geosite.dat` & `Furious-GUI-0.4.5/Furious/Data/xray/geosite.dat`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Data/xray/iran.dat` & `Furious-GUI-0.4.5/Furious/Data/xray/iran.dat`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Externals/GenTranslation.py` & `Furious-GUI-0.4.5/Furious/Externals/GenTranslation.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Externals/__init__.py` & `Furious-GUI-0.4.5/Furious/Externals/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Interface/Application.py` & `Furious-GUI-0.4.5/Furious/Interface/Application.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Interface/ConfigurationFactory.py` & `Furious-GUI-0.4.5/Furious/Interface/ConfigurationFactory.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Interface/CoreFactory.py` & `Furious-GUI-0.4.5/Furious/Interface/CoreFactory.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Interface/Encoder.py` & `Furious-GUI-0.4.5/Furious/Interface/Encoder.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Interface/GuiEditorItemFactory.py` & `Furious-GUI-0.4.5/Furious/Interface/GuiEditorItemFactory.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Interface/ItemUpdateProtocol.py` & `Furious-GUI-0.4.5/Furious/Interface/ItemUpdateProtocol.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Interface/Storage.py` & `Furious-GUI-0.4.5/Furious/Interface/Storage.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Interface/UserServersTableItem.py` & `Furious-GUI-0.4.5/Furious/Interface/UserServersTableItem.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Interface/__init__.py` & `Furious-GUI-0.4.5/Furious/Interface/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Library/Configuration.py` & `Furious-GUI-0.4.5/Furious/Library/Configuration.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Library/EmptyFactoryHelper.py` & `Furious-GUI-0.4.5/Furious/Library/EmptyFactoryHelper.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Library/Encoder.py` & `Furious-GUI-0.4.5/Furious/Library/Encoder.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Library/Tcping.py` & `Furious-GUI-0.4.5/Furious/Library/Tcping.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Library/__init__.py` & `Furious-GUI-0.4.5/Furious/Library/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/PyFramework/Ancestors.py` & `Furious-GUI-0.4.5/Furious/PyFramework/Ancestors.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/PyFramework/__init__.py` & `Furious-GUI-0.4.5/Furious/PyFramework/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/QtFramework/Ancestors.py` & `Furious-GUI-0.4.5/Furious/QtFramework/Ancestors.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/QtFramework/CoreProcess.py` & `Furious-GUI-0.4.5/Furious/QtFramework/CoreProcess.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/QtFramework/DNSResolver.py` & `Furious-GUI-0.4.5/Furious/QtFramework/DNSResolver.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/QtFramework/DynamicTheme.py` & `Furious-GUI-0.4.5/Furious/QtFramework/DynamicTheme.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/QtFramework/DynamicTranslate.py` & `Furious-GUI-0.4.5/Furious/QtFramework/DynamicTranslate.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/QtFramework/GuiEditorXXX.py` & `Furious-GUI-0.4.5/Furious/QtFramework/GuiEditorXXX.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/QtFramework/NetworkStateManager.py` & `Furious-GUI-0.4.5/Furious/QtFramework/NetworkStateManager.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/QtFramework/QtGui.py` & `Furious-GUI-0.4.5/Furious/QtFramework/QtGui.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/QtFramework/QtNetwork.py` & `Furious-GUI-0.4.5/Furious/QtFramework/QtNetwork.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/QtFramework/QtWidgets.py` & `Furious-GUI-0.4.5/Furious/QtFramework/QtWidgets.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/QtFramework/TextEditor.py` & `Furious-GUI-0.4.5/Furious/QtFramework/TextEditor.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/QtFramework/TextEditorTheme.py` & `Furious-GUI-0.4.5/Furious/QtFramework/TextEditorTheme.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/QtFramework/UpdatesManager.py` & `Furious-GUI-0.4.5/Furious/QtFramework/UpdatesManager.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/QtFramework/__init__.py` & `Furious-GUI-0.4.5/Furious/QtFramework/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Storage/UserServers.py` & `Furious-GUI-0.4.5/Furious/Storage/UserServers.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Storage/UserSubs.py` & `Furious-GUI-0.4.5/Furious/Storage/UserSubs.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Storage/__init__.py` & `Furious-GUI-0.4.5/Furious/Storage/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/TrayActions/Connect.py` & `Furious-GUI-0.4.5/Furious/TrayActions/Connect.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/TrayActions/EditConfiguration.py` & `Furious-GUI-0.4.5/Furious/TrayActions/EditConfiguration.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/TrayActions/Exit.py` & `Furious-GUI-0.4.5/Furious/TrayActions/Exit.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/TrayActions/Import.py` & `Furious-GUI-0.4.5/Furious/TrayActions/Import.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/TrayActions/Language.py` & `Furious-GUI-0.4.5/Furious/TrayActions/Language.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/TrayActions/Routing.py` & `Furious-GUI-0.4.5/Furious/TrayActions/Routing.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/TrayActions/Settings.py` & `Furious-GUI-0.4.5/Furious/TrayActions/Settings.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/TrayActions/SystemProxy.py` & `Furious-GUI-0.4.5/Furious/TrayActions/SystemProxy.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/TrayActions/__init__.py` & `Furious-GUI-0.4.5/Furious/TrayActions/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Utility/AppMainProcess.py` & `Furious-GUI-0.4.5/Furious/Utility/AppMainProcess.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Utility/AppResources.py` & `Furious-GUI-0.4.5/Furious/Utility/AppResources.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Utility/AppSettings.py` & `Furious-GUI-0.4.5/Furious/Utility/AppSettings.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Utility/AppSettingsFn.py` & `Furious-GUI-0.4.5/Furious/Utility/AppSettingsFn.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Utility/Constants.py` & `Furious-GUI-0.4.5/Furious/Utility/Constants.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Utility/PySide6Legacy.py` & `Furious-GUI-0.4.5/Furious/Utility/PySide6Legacy.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Utility/StartupOnBoot.py` & `Furious-GUI-0.4.5/Furious/Utility/StartupOnBoot.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Utility/SystemProxy.py` & `Furious-GUI-0.4.5/Furious/Utility/SystemProxy.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Utility/SystemRoutingTable.py` & `Furious-GUI-0.4.5/Furious/Utility/SystemRoutingTable.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Utility/SystemRuntime.py` & `Furious-GUI-0.4.5/Furious/Utility/SystemRuntime.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Utility/Utility.py` & `Furious-GUI-0.4.5/Furious/Utility/Utility.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Utility/__init__.py` & `Furious-GUI-0.4.5/Furious/Utility/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Version.py` & `Furious-GUI-0.4.5/Furious/Version.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-__version__ = '0.4.4'
+__version__ = '0.4.5'
```

### Comparing `Furious-GUI-0.4.4/Furious/Widget/Application.py` & `Furious-GUI-0.4.5/Furious/Widget/Application.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Widget/ConnectProgressBar.py` & `Furious-GUI-0.4.5/Furious/Widget/ConnectProgressBar.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Widget/GuiHysteria1.py` & `Furious-GUI-0.4.5/Furious/Widget/GuiHysteria1.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Widget/GuiHysteria2.py` & `Furious-GUI-0.4.5/Furious/Widget/GuiHysteria2.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Widget/GuiShadowsocks.py` & `Furious-GUI-0.4.5/Furious/Widget/GuiShadowsocks.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Widget/GuiTrojan.py` & `Furious-GUI-0.4.5/Furious/Widget/GuiTrojan.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Widget/GuiVLESS.py` & `Furious-GUI-0.4.5/Furious/Widget/GuiVLESS.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Widget/GuiVMess.py` & `Furious-GUI-0.4.5/Furious/Widget/GuiVMess.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Widget/GuiVTLS.py` & `Furious-GUI-0.4.5/Furious/Widget/GuiVTLS.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Widget/GuiVTransport.py` & `Furious-GUI-0.4.5/Furious/Widget/GuiVTransport.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Widget/IndentSpinBox.py` & `Furious-GUI-0.4.5/Furious/Widget/IndentSpinBox.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Widget/SystemTrayIcon.py` & `Furious-GUI-0.4.5/Furious/Widget/SystemTrayIcon.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Widget/UserServersQTableWidget.py` & `Furious-GUI-0.4.5/Furious/Widget/UserServersQTableWidget.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Widget/UserSubsQTableWidget.py` & `Furious-GUI-0.4.5/Furious/Widget/UserSubsQTableWidget.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,14 @@
         else:
             # macOS & linux
             mbox = QuestionDeleteMBox(
                 icon=AppQMessageBox.Icon.Question, parent=self.parent()
             )
             mbox.setWindowModality(QtCore.Qt.WindowModality.WindowModal)
 
-        mbox = QuestionDeleteMBox(icon=AppQMessageBox.Icon.Question)
         mbox.isMulti = bool(len(indexes) > 1)
         mbox.possibleRemark = self.item(indexes[0], 0).text()
         mbox.setText(mbox.customText())
         mbox.finished.connect(functools.partial(handleResultCode, indexes))
 
         # dummy ref
         setattr(self, '_questionDeleteMBox', mbox)
```

### Comparing `Furious-GUI-0.4.4/Furious/Widget/XrayAssetViewerQListWidget.py` & `Furious-GUI-0.4.5/Furious/Widget/XrayAssetViewerQListWidget.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Widget/__init__.py` & `Furious-GUI-0.4.5/Furious/Widget/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Window/AppMainWindow.py` & `Furious-GUI-0.4.5/Furious/Window/AppMainWindow.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Window/LogViewerWindow.py` & `Furious-GUI-0.4.5/Furious/Window/LogViewerWindow.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Window/QRCodeWindow.py` & `Furious-GUI-0.4.5/Furious/Window/QRCodeWindow.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Window/TextEditorWindow.py` & `Furious-GUI-0.4.5/Furious/Window/TextEditorWindow.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Window/UserSubsWindow.py` & `Furious-GUI-0.4.5/Furious/Window/UserSubsWindow.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Window/XrayAssetViewerWindow.py` & `Furious-GUI-0.4.5/Furious/Window/XrayAssetViewerWindow.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/Window/__init__.py` & `Furious-GUI-0.4.5/Furious/Window/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/__init__.py` & `Furious-GUI-0.4.5/Furious/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious/__main__.py` & `Furious-GUI-0.4.5/Furious/__main__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious_GUI.egg-info/PKG-INFO` & `Furious-GUI-0.4.5/Furious_GUI.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Furious-GUI
-Version: 0.4.4
-Summary: A PySide6-based cross platform GUI client that launches your beloved GFW to outer space.
+Version: 0.4.5
+Summary: A GUI proxy client based on PySide6. Support Xray-core & hysteria
 Home-page: https://github.com/LorenEteval/Furious
 Author: Loren Eteval
 Author-email: loren.eteval@proton.me
 License: GPL v3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `Furious-GUI-0.4.4/Furious_GUI.egg-info/SOURCES.txt` & `Furious-GUI-0.4.5/Furious_GUI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/Furious_GUI.egg-info/requires.txt` & `Furious-GUI-0.4.5/Furious_GUI.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/LICENSE` & `Furious-GUI-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/PKG-INFO` & `Furious-GUI-0.4.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Furious-GUI
-Version: 0.4.4
-Summary: A PySide6-based cross platform GUI client that launches your beloved GFW to outer space.
+Version: 0.4.5
+Summary: A GUI proxy client based on PySide6. Support Xray-core & hysteria
 Home-page: https://github.com/LorenEteval/Furious
 Author: Loren Eteval
 Author-email: loren.eteval@proton.me
 License: GPL v3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `Furious-GUI-0.4.4/README.md` & `Furious-GUI-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.4/setup.py` & `Furious-GUI-0.4.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 with open('README.md', 'r', encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
     name='Furious-GUI',
     version=__version__,
     license='GPL v3.0',
-    description='A PySide6-based cross platform GUI client that launches your beloved GFW to outer space.',
+    description='A GUI proxy client based on PySide6. Support Xray-core & hysteria',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Loren Eteval',
     author_email='loren.eteval@proton.me',
     url='https://github.com/LorenEteval/Furious',
     packages=find_packages(),
     package_data={'Furious': ['Data/**']},
```

