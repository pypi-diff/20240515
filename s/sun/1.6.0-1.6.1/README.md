# Comparing `tmp/sun-1.6.0.tar.gz` & `tmp/sun-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sun-1.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sun-1.6.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sun-1.6.0.tar` & `sun-1.6.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      230 2024-02-13 19:39:49.000000 sun-1.6.0/README.md
--rw-r--r--   0        0        0     1458 2024-02-13 19:39:49.000000 sun-1.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-13 19:39:49.000000 sun-1.6.0/sun/__init__.py
--rw-r--r--   0        0        0      981 2024-02-13 19:39:49.000000 sun-1.6.0/sun/__metadata__.py
--rwxr-xr-x   0        0        0     1710 2024-02-13 19:39:49.000000 sun-1.6.0/sun/autostart.py
--rw-r--r--   0        0        0        0 2024-02-13 19:39:49.000000 sun-1.6.0/sun/cli/__init__.py
--rw-r--r--   0        0        0     4989 2024-02-13 19:39:49.000000 sun-1.6.0/sun/cli/tool.py
--rw-r--r--   0        0        0     2402 2024-02-13 19:39:49.000000 sun-1.6.0/sun/configs.py
--rw-r--r--   0        0        0     1410 2024-02-13 19:39:49.000000 sun-1.6.0/sun/daemon.py
--rw-r--r--   0        0        0        0 2024-02-13 19:39:49.000000 sun-1.6.0/sun/gtk/__init__.py
--rw-r--r--   0        0        0     6880 2024-02-13 19:39:49.000000 sun-1.6.0/sun/gtk/status_icon.py
--rw-r--r--   0        0        0     1277 2024-02-13 19:39:49.000000 sun-1.6.0/sun/licenses.py
--rw-r--r--   0        0        0     5724 2024-02-13 19:39:49.000000 sun-1.6.0/sun/utils.py
--rw-r--r--   0        0        0     1366 1970-01-01 00:00:00.000000 sun-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0      230 2024-05-13 18:13:05.000000 sun-1.6.1/README.md
+-rw-r--r--   0        0        0     1458 2024-05-13 18:13:05.000000 sun-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-13 18:13:05.000000 sun-1.6.1/sun/__init__.py
+-rw-r--r--   0        0        0      919 2024-05-13 18:13:05.000000 sun-1.6.1/sun/__metadata__.py
+-rw-r--r--   0        0        0     1776 2024-05-13 18:13:05.000000 sun-1.6.1/sun/autostart.py
+-rw-r--r--   0        0        0        0 2024-05-13 18:13:05.000000 sun-1.6.1/sun/cli/__init__.py
+-rw-r--r--   0        0        0     5418 2024-05-13 18:13:05.000000 sun-1.6.1/sun/cli/tool.py
+-rw-r--r--   0        0        0     2497 2024-05-13 18:13:05.000000 sun-1.6.1/sun/configs.py
+-rw-r--r--   0        0        0     1584 2024-05-13 18:13:05.000000 sun-1.6.1/sun/daemon.py
+-rw-r--r--   0        0        0        0 2024-05-13 18:13:05.000000 sun-1.6.1/sun/gtk/__init__.py
+-rw-r--r--   0        0        0     7078 2024-05-13 18:13:05.000000 sun-1.6.1/sun/gtk/status_icon.py
+-rw-r--r--   0        0        0     1379 2024-05-13 18:13:05.000000 sun-1.6.1/sun/licenses.py
+-rw-r--r--   0        0        0     6263 2024-05-13 18:13:05.000000 sun-1.6.1/sun/utils.py
+-rw-r--r--   0        0        0     1366 1970-01-01 00:00:00.000000 sun-1.6.1/PKG-INFO
```

### Comparing `sun-1.6.0/pyproject.toml` & `sun-1.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.2.0,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "sun"
-version = "1.6.0"
+version = "1.6.1"
 authors = [
     {name = "Dimitris Zlatanidis", email = "dslackw@gmail.com"},
 ]
 maintainers = [
     {name = "Dimitris Zlatanidis", email = "dslackw@gmail.com"},
 ]
 description = "Tray notification applet for informing about package updates in Slackware."
```

### Comparing `sun-1.6.0/sun/__metadata__.py` & `sun-1.6.1/sun/__metadata__.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,31 +4,30 @@
 import os
 import shutil
 import platform
 import subprocess
 from pathlib import Path
 
 
-__all__: str = 'sun'
+__prgnam__: str = 'sun'
 __author__: str = 'dslackw'
 __copyright__: str = '2015-2024'
-__version_info__: tuple = (1, 6, 0)
-__version__: str = '{0}.{1}.{2}'.format(*__version_info__)
+__version__: str = '1.6.1'
 __license__: str = 'GNU General Public License v3 (GPLv3)'
 __email__: str = 'dslackw@gmail.com'
 __website__: str = 'https://gitlab.com/dslackw/sun'
 
 
 data_configs: dict = {
     'bin_path': Path('/usr/bin/'),
     'pkg_path': Path('/var/log/packages'),
     'icon_path': Path('/usr/share/pixmaps'),
     'desktop_path': Path('/usr/share/applications'),
     'xdg_autostart': Path('/etc/xdg/autostart'),
-    'sun_conf_path': Path('/etc/', __all__),
+    'sun_conf_path': Path('/etc/', __prgnam__),
     'arch': platform.machine(),
     'kernel': os.uname()[2],
     'cpu': platform.processor(),
     'mem': subprocess.getoutput('free -h').split(),
     'disk': shutil.disk_usage('/'),
     'uptime': subprocess.getoutput('uptime -p')
 }
```

### Comparing `sun-1.6.0/sun/autostart.py` & `sun-1.6.1/sun/autostart.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 import sys
 import shutil
 from pathlib import Path
+from sun.__metadata__ import data_configs
 
 
-def autostart():
+def autostart() -> None:
+    """ SUN autostart enable-disable script
+    """
     args: list = sys.argv
     args.pop(0)
 
-    xdg_autostart_path: Path = Path('/etc/xdg/autostart')
-    enable_file: Path = Path(xdg_autostart_path, 'sun-daemon.desktop')
-    disable_file: Path = Path(xdg_autostart_path, 'sun-daemon.desktop.sample')
+    enable_file: Path = Path(data_configs['xdg_autostart'], 'sun-daemon.desktop')
+    disable_file: Path = Path(data_configs['xdg_autostart'], 'sun-daemon.desktop.sample')
 
     message: str = 'The sun-daemon autostart is'
     message_enabled: str = f'{message} enabled.'
     message_disabled: str = f'{message} disabled.'
     message_already_enabled: str = f'{message} already enabled.'
     message_already_disabled: str = f'{message} already disabled.'
```

### Comparing `sun-1.6.0/sun/cli/tool.py` & `sun-1.6.1/sun/cli/tool.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 from sun.configs import Configs
 from sun.utils import Utilities, Fetch
 from sun.__metadata__ import __version__, data_configs
 
 
 class Tools(Configs):
 
+    """ SUN Utilities.
+    """
+
     def __init__(self):
         super(Configs, self).__init__()
         self.data_configs: dict = data_configs
         self.utils = Utilities()
         self.fetch = Fetch()
 
     @staticmethod
@@ -40,15 +43,15 @@
         print(args)
 
     def check_updates(self) -> tuple:
         """ Returns the count of the packages and the message. """
         message: str = 'No news is good news!'
         packages: list = list(self.fetch.updates())
         count_packages: int = len(packages)
-        count_repositories: int = len(set([repo.split(':')[0] for repo in packages]))
+        count_repositories: int = len({repo.split(':')[0] for repo in packages})
         repositories_message: str = str()
 
         if count_repositories > 1:
             repositories_message: str = f'from {count_repositories} repositories'
 
         if count_packages > 0:
             message: str = f'{count_packages} software updates are available {repositories_message}\n'
@@ -56,21 +59,23 @@
         return message, packages
 
     def view_updates(self) -> None:
         """ Prints the updates packages to the terminal. """
         message, packages = self.check_updates()
         print(message)
         if len(packages) > 0:
-            [print(pkg) for pkg in packages]
+            for package in packages:
+                print(package)
 
     def daemon_status(self) -> bool:
         """ Returns the daemon status. """
-        output = subprocess.run(self.sun_daemon_running, shell=True).returncode
-        if output == 0:
+        output = subprocess.run(self.sun_daemon_running, shell=True, check=False)
+        if output.returncode == 0:
             return True
+        return False
 
     def daemon_process(self, arg: str, message: str) -> str:
         """ Returns the daemon status message. """
         output: int = 1
 
         command: dict = {
             'start': self.sun_daemon_start,
@@ -90,22 +95,25 @@
         if output > 0:
             message: str = f'FAILED [{output}]: {message}'
 
         return message
 
 
 class Cli:
-    """ Commandline control menu. """
+    """ Command line control menu.
+    """
 
     def __init__(self):
         self.args: list = []
         self.tools = Tools()
         self.utils = Utilities()
 
     def menu(self) -> None:
+        """ Menu call methods.
+        """
         self.tools.su()
         self.args: list = sys.argv
         self.args.pop(0)
 
         process: dict = {
             'start': self.view_start,
             'stop': self.view_stop,
@@ -115,38 +123,50 @@
             'info': self.view_info,
             'help': self.tools.usage
         }
 
         if len(self.args) == 1:
             try:
                 process[self.args[0]]()
-            except KeyError:
-                raise SystemExit("try: 'sun help'")
+            except KeyError as e:
+                raise SystemExit("try: 'sun help'") from e
 
         elif len(self.args) == 2 and self.args[0] == 'start' and self.args[1] == '--gtk':
             subprocess.call('sun-gtk &', shell=True)
 
         else:
             raise SystemExit("try: 'sun help'")
 
     def view_start(self) -> None:
+        """ View starting message.
+        """
         print(self.tools.daemon_process(self.args[0], 'Starting SUN daemon:  sun-daemon &'))
 
     def view_stop(self) -> None:
+        """ View stopping message.
+        """
         print(self.tools.daemon_process(self.args[0], 'Stopping SUN daemon:  sun-daemon'))
 
     def view_restart(self) -> None:
+        """ View restarting message.
+        """
         print(self.tools.daemon_process(self.args[0], 'Restarting SUN daemon:  sun-daemon'))
 
     def view_status(self) -> None:
+        """ View status message.
+        """
         print('SUN is running...' if self.tools.daemon_status() else 'SUN is not running')
 
     def view_info(self) -> None:
+        """ View info message.
+        """
         print(self.utils.os_info())
 
 
-def main():
+def main() -> None:
+    """ Call menu object.
+    """
     try:
         cli = Cli()
         cli.menu()
-    except KeyboardInterrupt:
-        raise SystemExit(1)
+    except KeyboardInterrupt as e:
+        raise SystemExit(1) from e
```

### Comparing `sun-1.6.0/sun/configs.py` & `sun-1.6.1/sun/configs.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
-import tomli
 from pathlib import Path
-from sun.__metadata__ import data_configs, __all__
+import tomli
+from sun.__metadata__ import data_configs, __prgnam__
+
 
+class Configs:  # pylint: disable=[R0903]
 
-class Configs:
+    """ General configs.
+    """
 
     # Configuration files.
-    config_file: str = f'{__all__}.toml'
+    config_file: str = f'{__prgnam__}.toml'
     repositories_file: str = 'repositories.toml'
     config_path: str = data_configs['sun_conf_path']
     slpkg_toml: Path = Path(config_path, config_file)
     repositories_toml: Path = Path(config_path, repositories_file)
     configs: dict = {}
     repos: dict = {}
 
@@ -30,36 +33,36 @@
     # Default repository
     repositories: list = [
         {'NAME': 'Slackware',
          'HTTP_MIRROR': 'https://mirrors.slackware.com/slackware/slackware64-15.0/',
          'LOG_PATH': '/var/lib/slackpkg/',
          'LOG_FILE': 'ChangeLog.txt',
          'PATTERN': 'Upgraded[.]|Rebuilt[.]|Added[.]|Removed[.]',
-         'COMPARE': '^\w[Mon|Tue|Wed|Thu|Fri|Sat|Sun]'}
+         'COMPARE': '^\\w[Mon|Tue|Wed|Thu|Fri|Sat|Sun]'}
     ]
 
     try:
         if slpkg_toml.is_file():
             with open(slpkg_toml, 'rb') as conf:
                 configs: dict = tomli.load(conf)
         else:
-            raise Exception(f"Error: Failed to find '{slpkg_toml}' file.")
+            raise FileNotFoundError(f"Error: Failed to find '{slpkg_toml}' file.")
 
         if repositories_toml.is_file():
             with open(repositories_toml, 'rb') as conf:
                 repos: dict = tomli.load(conf)
         else:
-            raise Exception(f"Error: Failed to find '{repositories_toml}' file.")
+            raise FileNotFoundError(f"Error: Failed to find '{repositories_toml}' file.")
 
         # Time configs.
         interval: int = configs['time']['INTERVAL']
         standby: int = configs['time']['STANDBY']
         # Daemon configs.
         sun_daemon_start: str = configs['daemon']['START']
         sun_daemon_stop: str = configs['daemon']['STOP']
         sun_daemon_restart: str = configs['daemon']['RESTART']
         sun_daemon_running: str = configs['daemon']['RUNNING']
         # Repositories configs.
         repositories: list = repos['repository']
 
     except (tomli.TOMLDecodeError, KeyError) as error:
-        raise SystemExit(f"Error: {error}: in the config file '{config_path}{config_file}'.")
+        raise SystemExit(f"Error: {error}: in the config file '{config_path}{config_file}'.") from error
```

### Comparing `sun-1.6.0/sun/daemon.py` & `sun-1.6.1/sun/daemon.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,50 +3,59 @@
 
 import time
 import notify2
 
 from sun.cli.tool import Tools
 from sun.configs import Configs
 from sun.utils import Fetch
-from sun.__metadata__ import __all__, data_configs
+from sun.__metadata__ import __prgnam__, data_configs
 
 
 class Notify(Configs):
-    """ Main notify Class. """
+    """ Main notify Class.
+    """
 
     def __init__(self):
         super(Configs, self).__init__()
         self.tool = Tools()
         self.fetch = Fetch()
 
         self.notify = None
         self.icon = None
         self.message: str = str()
         self.count_packages: int = 0
         self.title: str = f"{'':>10}Software Updates"
-        self.icon: str = f'{data_configs["icon_path"]}/{__all__}.png'
+        self.icon: str = f'{data_configs["icon_path"]}/{__prgnam__}.png'
 
         notify2.uninit()
         notify2.init('sun')
 
     def set_notification_message(self) -> None:
+        """ Set dbus notification message.
+        """
         self.count_packages: int = len(list(self.fetch.updates()))
         self.message: str = f"{'':>3}{self.count_packages} Software updates are available\n"
         self.notify = notify2.Notification(self.title, self.message, self.icon)
         self.notify.set_timeout(60000 * self.standby)
 
     def daemon(self) -> None:
-        """ SUN daemon. """
+        """ SUN daemon.
+        """
         while True:
             self.set_notification_message()
             if self.count_packages > 0:
                 self.notify.show()
 
             time.sleep(60 * self.interval)
 
 
-def main():
+def main() -> None:
+    """ Starts the daemon.
+
+    Raises:
+        SystemExit: Exit code 1.
+    """
     try:
         notify = Notify()
         notify.daemon()
-    except KeyboardInterrupt:
-        raise SystemExit(1)
+    except KeyboardInterrupt as e:
+        raise SystemExit(1) from e
```

### Comparing `sun-1.6.0/sun/gtk/status_icon.py` & `sun-1.6.1/sun/gtk/status_icon.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,41 +4,44 @@
 import gi
 gi.require_version('Gtk', '3.0')
 from gi.repository import Gtk
 from gi.repository.GdkPixbuf import Pixbuf
 
 from sun.licenses import ABOUT, LICENSE
 from sun.__metadata__ import (
-    __all__,
+    __prgnam__,
     __email__,
     __author__,
     __version__,
     __website__,
     data_configs
 )
 
 from sun.utils import Utilities
 from sun.configs import Configs
 from sun.cli.tool import Tools
 
 
 class GtkStatusIcon(Configs):
 
+    """ GTK Status Icon
+    """
+
     def __init__(self):
         super(Configs, self).__init__()
         self.data_configs: dict = data_configs
         self.menu = None
         self.tool = Tools()
 
-        self.sun_icon: str = f'{self.data_configs["icon_path"]}/{__all__}.png'
+        self.sun_icon: str = f'{self.data_configs["icon_path"]}/{__prgnam__}.png'
         self.status_icon = Gtk.StatusIcon()
         self.status_icon.set_from_file(self.sun_icon)
         self.status_icon.connect('popup-menu', self.right_click_event)
 
-    def right_click_event(self, icon, button, time):
+    def right_click_event(self, icon, button, time) -> None:  # pylint: disable=[R0914,R0915]
         """ Handler menu and submenu. """
 
         # Set Gtk menu and submenu
         submenu = Gtk.Menu()
         self.menu = Gtk.Menu()
 
         # Creating Start submenu handler
@@ -93,15 +96,15 @@
         img_info = Gtk.Image()
         img_info.set_from_stock(Gtk.STOCK_INFO, 1)
         os_info = Gtk.ImageMenuItem('Os Info')
         os_info.connect('activate', self.show_os_info)
         os_info.set_image(img_info)
         self.menu.append(os_info)
 
-        # Creating seperator
+        # Creating separator
         sep = Gtk.SeparatorMenuItem()
         self.menu.append(sep)
 
         # Creating About menu handler
         img_about = Gtk.Image()
         img_about.set_from_stock(Gtk.STOCK_ABOUT, 1)
         about = Gtk.ImageMenuItem('About')
@@ -117,45 +120,45 @@
         quit_and_exit.set_image(img_quit)
         self.menu.append(quit_and_exit)
 
         self.menu.show_all()
 
         self.menu.popup(None, None, None, self.status_icon, button, time)
 
-    def message(self, data, title):
+    def message(self, data, title) -> None:
         """ Method to display messages to the user. """
         msg = Gtk.MessageDialog(type=Gtk.MessageType.INFO,
                                 buttons=Gtk.ButtonsType.CLOSE)
         msg.set_resizable(0)
         msg.set_title(title)
         msg.format_secondary_text(data)
         msg.set_icon_from_file(self.sun_icon)
         msg.run()
         msg.destroy()
 
-    def show_check_updates(self, widget):
+    def show_check_updates(self, widget) -> None:
         """ Show message updates. """
         title: str = 'SUN - Check Updates'
         data, packages = self.tool.check_updates()
         count: int = len(packages)
         if count > 0:
             packages: list = packages[:10]
             if count > 10:
                 packages += ['\nand more...']
             self.message('{0}\n{1}'.format(data, '\n'.join(packages)), title)
         else:
             self.message(data, title)
 
-    def show_os_info(self, widget):
+    def show_os_info(self, widget) -> None:
         """ Show message OS info. """
         title: str = 'SUN - OS Info'
         data: str = Utilities().os_info()
         self.message(data, title)
 
-    def show_about_dialog(self, widget):
+    def show_about_dialog(self, widget) -> None:
         """ Show message About info. """
         about_dialog = Gtk.AboutDialog()
         about_dialog.set_destroy_with_parent(True)
         about_dialog.set_name('SUN - About')
         about_dialog.set_icon_from_file(self.sun_icon)
         about_dialog.set_program_name('SUN')
         about_dialog.set_version(__version__)
@@ -163,42 +166,43 @@
         about_dialog.set_license('\n'.join(LICENSE))
         about_dialog.set_website(__website__)
         about_dialog.set_logo(Pixbuf.new_from_file(self.sun_icon))
         about_dialog.set_comments(ABOUT)
         about_dialog.run()
         about_dialog.destroy()
 
-    def daemon_start(self, widget):
+    def daemon_start(self, widget) -> None:
         """ Show message and start the daemon. """
         title: str = 'SUN daemon'
         data: str = 'SUN daemon starts...'
         data: str = self.tool.daemon_process('start', data)
         self.message(data, title)
 
-    def daemon_stop(self, widget):
+    def daemon_stop(self, widget) -> None:
         """ Show message and stop the daemon. """
         title: str = 'SUN daemon'
         data: str = 'SUN daemon stops'
         data: str = self.tool.daemon_process('stop', data)
         self.message(data, title)
 
-    def daemon_restart(self, widget):
+    def daemon_restart(self, widget) -> None:
         """ Show message and restart the daemon. """
         title: str = 'SUN daemon'
         data: str = 'SUN daemon restarts...'
         data: str = self.tool.daemon_process('restart', data)
         self.message(data, title)
 
-    def show_daemon_status(self, widget):
+    def show_daemon_status(self, widget) -> None:
         """ Show message status about the daemon. """
         title: str = 'SUN daemon'
         data: str = ('SUN is running...' if self.tool.daemon_status() else 'SUN is not running')
         self.message(data, title)
 
 
-def main():
+def main() -> None:
+    """ GTK Main function.
+    """
     try:
         GtkStatusIcon()
         Gtk.main()
-    except KeyboardInterrupt:
-        raise SystemExit(1)
-
+    except KeyboardInterrupt as e:
+        raise SystemExit(1) from e
```

### Comparing `sun-1.6.0/sun/licenses.py` & `sun-1.6.1/sun/licenses.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,25 +3,24 @@
 
 from sun.__metadata__ import __copyright__
 
 
 ABOUT: str = ('SUN (Slackware Update Notifier)\n\n'
               'Tray notification applet for informing '
               'about package updates in Slackware.\n\n'
-              'Copyright {0} © Dimitris Zlatanidis\n'
+              f'Copyright {__copyright__} © Dimitris Zlatanidis\n'
               'Slackware® is a Registered Trademark of '
               'Patrick Volkerding.\n'
               'Linux® is a Registered Trademark of Linus '
-              'Torvalds.'.format(__copyright__))
+              'Torvalds.')
 
 
-LICENSE: tuple[str, str, str, str, str, str, str, str, str, str] = (
-     'This program is free software: you can redistribute it and/or modify',
-     'it under the terms of the GNU General Public License as published by',
-     'the Free Software Foundation, either version 3 of the License, or',
-     '(at your option) any later version.\n',
-     'This program is distributed in the hope that it will be useful',
-     'but WITHOUT ANY WARRANTY; without even the implied warranty of',
-     'MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the',
-     'GNU General Public License for more details.\n',
-     'You should have received a copy of the GNU General Public License',
-     'along with this program.  If not, see <http://www.gnu.org/licenses/>.')
+LICENSE: tuple[str] = ('This program is free software: you can redistribute it and/or modify',
+                       'it under the terms of the GNU General Public License as published by',
+                       'the Free Software Foundation, either version 3 of the License, or',
+                       '(at your option) any later version.\n',
+                       'This program is distributed in the hope that it will be useful',
+                       'but WITHOUT ANY WARRANTY; without even the implied warranty of',
+                       'MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the',
+                       'GNU General Public License for more details.\n',
+                       'You should have received a copy of the GNU General Public License',
+                       'along with this program.  If not, see <http://www.gnu.org/licenses/>.')
```

### Comparing `sun-1.6.0/sun/utils.py` & `sun-1.6.1/sun/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,81 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 import re
 import getpass
-import urllib3
 from pathlib import Path
 from typing import Generator
+import urllib3
 from urllib3.exceptions import HTTPError
+
 from sun.configs import Configs
 from sun.__metadata__ import data_configs
 
 
 class Utilities(Configs):
-    """ General utilities. """
+    """ General utilities.
+    """
 
     def __init__(self):
         super(Configs, self).__init__()
         self.data_configs: dict = data_configs
 
     @staticmethod
     def read_repo_text_file(mirror: str) -> str:
-        """ Reads and returns the mirror log text files. """
+        """ Reads repository ChangeLog.txt file.
+
+        Args:
+            mirror (str): HTTP mirror.
+
+        Returns:
+            str: The ChangeLog.txt file lines.
+        """
         log_txt: str = str()
         try:
             http = urllib3.PoolManager()
             con = http.request('GET', mirror)
             log_txt = con.data.decode()
         except KeyError:
             print('SUN: Error: Ftp mirror not supported')
         except HTTPError:
             print(f'SUN: Error: Failed to connect to {mirror}')
 
         return log_txt
 
     @staticmethod
     def read_local_text_file(registry: Path) -> str:
-        """ Reads and returns the local log text files. """
+        """ Reads the local ChangeLog.txt file.
+
+        Args:
+            registry (Path): The local file for reading.
+
+        Returns:
+            str: The ChangeLog.txt file lines.
+        """
         log_txt: str = str()
         if registry.is_file():
             with open(registry, 'r', encoding='utf-8', errors='ignore') as file_txt:
                 log_txt = file_txt.read()
         else:
             print(f"\nSUN: Error: Failed to find '{registry}' file.\n")
 
         return log_txt
 
     def slack_version(self) -> tuple:
-        """ Returns the distribution name and version. """
+        """ Returns the distribution name and version.
+        """
         version_file: str = self.read_local_text_file(Path('/etc/slackware-version'))
         slackware_version: list = re.findall(r'\d+\.\d+', version_file)
 
         return version_file.split()[0], ''.join(slackware_version)
 
     def os_info(self) -> str:
-        """ Returns the distribution information. """
+        """ Returns the distribution information.
+        """
         distribution: tuple = self.slack_version()
         os_name: str = distribution[0]
         version: str = distribution[1]
         return (f'User: {getpass.getuser()}\n'
                 f'OS: {os_name}\n'
                 f'Version: {version}\n'
                 f'Arch: {self.data_configs["arch"]}\n'
@@ -71,32 +89,34 @@
                 f'Free: {self.data_configs["disk"][2] // (2**30)}Gi, Used: '
                 f'{self.data_configs["disk"][1] // (2**30)}Gi, '
                 f'Total: {self.data_configs["disk"][0] // (2**30)}Gi\n'
                 f'[Processor]\n'
                 f'CPU: {self.data_configs["cpu"]}')
 
 
-class Fetch(Utilities):
+class Fetch(Utilities):  # pylint: disable=[R0902]
     """ Fetching how many packages and from where have upgraded,
-        removed or added. """
+        removed or added.
+    """
 
     def __init__(self):
         super(Utilities).__init__()
         self.local_date = None
         self.repo_name = None
         self.repo_mirror = None
         self.repo_log_path = None
         self.repo_log_file = None
         self.repo_pattern = None
         self.repo_compare = None
         self.mirror_log = None
         self.local_log = None
 
     def updates(self) -> Generator:
-        """ Fetching all the necessary packages. """
+        """ Fetching all the necessary packages.
+        """
         for repository in self.repositories:
             self.assign_repository_data(repository)
 
             if self.repo_mirror and self.repo_log_path:
                 self.assign_mirror_log_file()
                 self.assign_local_log_file()
                 self.assign_local_date()
@@ -105,41 +125,55 @@
                     if self.local_date == line.strip():
                         break
                     if re.findall(self.repo_pattern, line):
                         line: str = self.patch_line_for_slackware(line)
                         yield f'{self.repo_name}: {line.split("/")[-1]}'
 
     def assign_repository_data(self, repository: dict) -> None:
-        """ Assign the repository data from the .toml file. """
+        """ Assign the repository data from the .toml file.
+
+        Args:
+            repository (dict): Repository's data.
+        """
         try:
             self.repo_name: str = repository['REPOSITORY_NAME']
             self.repo_mirror: str = repository['HTTP_MIRROR']
             self.repo_log_path: str = repository['LOG_PATH']
             self.repo_log_file: str = repository['LOG_FILE']
             self.repo_pattern: str = repository['PACKAGE_PATTERN']
             self.repo_compare: str = repository['COMPARE_PATTERN']
         except KeyError as error:
             print(f"SUN: KeyError: {error}: in the config file '{self.config_path}{self.config_file}'.")
 
     def patch_line_for_slackware(self, line: str) -> str:
-        """ Patches the line for linux updates. """
+        """ Patches the line for linux updates.
+
+        Args:
+            line (str): ChangeLog.txt line for patching.
+
+        Returns:
+            str: Patching line.
+        """
         slack_name: tuple = ('Slackware', 'slackware', 'Slack', 'slack')
         if line.startswith('patches/packages/linux') and self.repo_name in slack_name:
             line = line.split("/")[-2]
         return line
 
     def assign_local_date(self) -> None:
-        """ Finds the date from the local log file and assigned. """
+        """ Finds the date from the local log file and assigned.
+        """
         for line in self.local_log.splitlines():
             if re.findall(self.repo_compare, line):
                 self.local_date: str = line.strip()
                 break
 
     def assign_mirror_log_file(self) -> None:
-        """ Reads the mirror log file and assigned. """
+        """ Assign the remote ChangeLog.txt file.
+        """
         self.mirror_log: str = self.read_repo_text_file(f'{self.repo_mirror}{self.repo_log_file}')
 
     def assign_local_log_file(self) -> None:
-        """ Reads the local log file and assigned. """
+        """ Assign the local ChangeLog.txt file.
+        """
         self.local_log: str = self.read_local_text_file(Path(self.repo_log_path, self.repo_log_file))
         if not self.local_log:
             self.local_date: str = str()
```

### Comparing `sun-1.6.0/PKG-INFO` & `sun-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sun
-Version: 1.6.0
+Version: 1.6.1
 Summary: Tray notification applet for informing about package updates in Slackware.
 Keywords: tray,notify,slackware,desktop
 Author-email: Dimitris Zlatanidis <dslackw@gmail.com>
 Maintainer-email: Dimitris Zlatanidis <dslackw@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
```

