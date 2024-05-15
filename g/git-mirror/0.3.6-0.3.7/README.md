# Comparing `tmp/git_mirror-0.3.6.tar.gz` & `tmp/git_mirror-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_mirror-0.3.6.tar", max compression
+gzip compressed data, was "git_mirror-0.3.7.tar", max compression
```

## Comparing `git_mirror-0.3.6.tar` & `git_mirror-0.3.7.tar`

### file list

```diff
@@ -1,28 +1,30 @@
--rw-r--r--   0        0        0     1071 2024-02-26 03:49:58.011479 git_mirror-0.3.6/LICENSE
--rw-r--r--   0        0        0     5656 2024-02-26 03:49:58.011479 git_mirror-0.3.6/README.md
--rw-r--r--   0        0        0      907 2024-02-26 03:50:48.711195 git_mirror-0.3.6/git_mirror/__about__.py
--rw-r--r--   0        0        0      285 2024-02-26 03:49:58.011479 git_mirror-0.3.6/git_mirror/__init__.py
--rw-r--r--   0        0        0    17188 2024-02-26 03:49:58.011479 git_mirror-0.3.6/git_mirror/__main__.py
--rw-r--r--   0        0        0     5197 2024-02-26 03:49:58.011479 git_mirror-0.3.6/git_mirror/bug_report.py
--rw-r--r--   0        0        0      819 2024-02-26 03:49:58.011479 git_mirror-0.3.6/git_mirror/check_cli_deps.py
--rw-r--r--   0        0        0     9466 2024-02-26 03:49:58.011479 git_mirror-0.3.6/git_mirror/cross_repo_sync.py
--rw-r--r--   0        0        0     3191 2024-02-26 03:49:58.015478 git_mirror-0.3.6/git_mirror/custom_types.py
--rw-r--r--   0        0        0      116 2024-02-26 03:49:58.015478 git_mirror-0.3.6/git_mirror/dummies.py
--rw-r--r--   0        0        0       15 2024-02-26 03:49:58.015478 git_mirror-0.3.6/git_mirror/features.py
--rw-r--r--   0        0        0      921 2024-02-26 03:49:58.015478 git_mirror-0.3.6/git_mirror/file_system.py
--rw-r--r--   0        0        0     2679 2024-02-26 03:49:58.015478 git_mirror-0.3.6/git_mirror/logging_config.py
--rw-r--r--   0        0        0    13278 2024-02-26 03:49:58.015478 git_mirror-0.3.6/git_mirror/manage_config.py
--rw-r--r--   0        0        0     5706 2024-02-26 03:49:58.015478 git_mirror-0.3.6/git_mirror/manage_git.py
--rw-r--r--   0        0        0    25967 2024-02-26 03:49:58.015478 git_mirror-0.3.6/git_mirror/manage_github.py
--rw-r--r--   0        0        0    30169 2024-02-26 03:49:58.015478 git_mirror-0.3.6/git_mirror/manage_gitlab.py
--rw-r--r--   0        0        0     3532 2024-02-26 03:49:58.015478 git_mirror-0.3.6/git_mirror/manage_poetry.py
--rw-r--r--   0        0        0     4389 2024-02-26 03:49:58.015478 git_mirror-0.3.6/git_mirror/manage_pypi.py
--rw-r--r--   0        0        0     3827 2024-02-26 03:49:58.015478 git_mirror-0.3.6/git_mirror/menu.py
--rw-r--r--   0        0        0     2572 2024-02-26 03:49:58.015478 git_mirror-0.3.6/git_mirror/pat_init.py
--rw-r--r--   0        0        0     2514 2024-02-26 03:49:58.015478 git_mirror-0.3.6/git_mirror/pat_init_gitlab.py
--rw-r--r--   0        0        0       80 2024-02-26 03:49:58.015478 git_mirror-0.3.6/git_mirror/py.typed
--rw-r--r--   0        0        0    12615 2024-02-26 03:49:58.015478 git_mirror-0.3.6/git_mirror/router.py
--rw-r--r--   0        0        0     1840 2024-02-26 03:49:58.015478 git_mirror-0.3.6/git_mirror/safe_env.py
--rw-r--r--   0        0        0     1499 2024-02-26 03:49:58.015478 git_mirror-0.3.6/git_mirror/version_check.py
--rw-r--r--   0        0        0     5970 2024-02-26 03:49:58.015478 git_mirror-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     7519 1970-01-01 00:00:00.000000 git_mirror-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-02-27 21:44:05.324554 git_mirror-0.3.7/LICENSE
+-rw-r--r--   0        0        0     5656 2024-02-27 21:44:05.324554 git_mirror-0.3.7/README.md
+-rw-r--r--   0        0        0      907 2024-02-27 21:45:02.424474 git_mirror-0.3.7/git_mirror/__about__.py
+-rw-r--r--   0        0        0      285 2024-02-27 21:44:05.324554 git_mirror-0.3.7/git_mirror/__init__.py
+-rw-r--r--   0        0        0    17502 2024-02-27 21:44:05.324554 git_mirror-0.3.7/git_mirror/__main__.py
+-rw-r--r--   0        0        0     5392 2024-02-27 21:44:05.324554 git_mirror-0.3.7/git_mirror/bug_report.py
+-rw-r--r--   0        0        0      905 2024-02-27 21:44:05.324554 git_mirror-0.3.7/git_mirror/check_cli_deps.py
+-rw-r--r--   0        0        0     9621 2024-02-27 21:44:05.324554 git_mirror-0.3.7/git_mirror/cross_repo_sync.py
+-rw-r--r--   0        0        0     3191 2024-02-27 21:44:05.328554 git_mirror-0.3.7/git_mirror/custom_types.py
+-rw-r--r--   0        0        0      116 2024-02-27 21:44:05.328554 git_mirror-0.3.7/git_mirror/dummies.py
+-rw-r--r--   0        0        0       15 2024-02-27 21:44:05.328554 git_mirror-0.3.7/git_mirror/features.py
+-rw-r--r--   0        0        0      921 2024-02-27 21:44:05.328554 git_mirror-0.3.7/git_mirror/file_system.py
+-rw-r--r--   0        0        0     2679 2024-02-27 21:44:05.328554 git_mirror-0.3.7/git_mirror/logging_config.py
+-rw-r--r--   0        0        0    13411 2024-02-27 21:44:05.328554 git_mirror-0.3.7/git_mirror/manage_config.py
+-rw-r--r--   0        0        0     6753 2024-02-27 21:44:05.328554 git_mirror-0.3.7/git_mirror/manage_git.py
+-rw-r--r--   0        0        0    29587 2024-02-27 21:44:05.328554 git_mirror-0.3.7/git_mirror/manage_github.py
+-rw-r--r--   0        0        0    34647 2024-02-27 21:44:05.328554 git_mirror-0.3.7/git_mirror/manage_gitlab.py
+-rw-r--r--   0        0        0     3925 2024-02-27 21:44:05.328554 git_mirror-0.3.7/git_mirror/manage_poetry.py
+-rw-r--r--   0        0        0     4254 2024-02-27 21:44:05.328554 git_mirror-0.3.7/git_mirror/manage_pypi.py
+-rw-r--r--   0        0        0     3829 2024-02-27 21:44:05.328554 git_mirror-0.3.7/git_mirror/menu.py
+-rw-r--r--   0        0        0     2753 2024-02-27 21:44:05.328554 git_mirror-0.3.7/git_mirror/pat_init.py
+-rw-r--r--   0        0        0     2695 2024-02-27 21:44:05.328554 git_mirror-0.3.7/git_mirror/pat_init_gitlab.py
+-rw-r--r--   0        0        0     1287 2024-02-27 21:44:05.328554 git_mirror-0.3.7/git_mirror/performance.py
+-rw-r--r--   0        0        0       80 2024-02-27 21:44:05.328554 git_mirror-0.3.7/git_mirror/py.typed
+-rw-r--r--   0        0        0    13399 2024-02-27 21:44:05.328554 git_mirror-0.3.7/git_mirror/router.py
+-rw-r--r--   0        0        0     2006 2024-02-27 21:44:05.328554 git_mirror-0.3.7/git_mirror/safe_env.py
+-rw-r--r--   0        0        0      364 2024-02-27 21:44:05.328554 git_mirror-0.3.7/git_mirror/ui.py
+-rw-r--r--   0        0        0     1608 2024-02-27 21:44:05.328554 git_mirror-0.3.7/git_mirror/version_check.py
+-rw-r--r--   0        0        0     5997 2024-02-27 21:44:05.328554 git_mirror-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     7481 1970-01-01 00:00:00.000000 git_mirror-0.3.7/PKG-INFO
```

### Comparing `git_mirror-0.3.6/LICENSE` & `git_mirror-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `git_mirror-0.3.6/README.md` & `git_mirror-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `git_mirror-0.3.6/git_mirror/__about__.py` & `git_mirror-0.3.7/git_mirror/__about__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "__readme__",
     "__repository__",
     "__homepage__",
     "__documentation__",
 ]
 
 __title__ = "git_mirror"
-__version__ = "0.3.6"
+__version__ = "0.3.7"
 __description__ = "Make your local git repos look like github or gitlab. See readme for how this differs from the many other multi-repo tools."
 __author__ = "Matthew Martin"
 __author_email__ = "matthewdeanmartin@gmail.com"
 __keywords__ = ["git", "gitlab", "github", "polyrepo"]
 __status__ = "4 - Beta"
 __license__ = "MIT"
 __readme__ = "README.md"
```

### Comparing `git_mirror-0.3.6/git_mirror/__main__.py` & `git_mirror-0.3.7/git_mirror/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,26 +15,29 @@
 import git_mirror.router as router
 from git_mirror import logging_config
 from git_mirror.__about__ import __description__, __version__
 from git_mirror.bug_report import BugReporter
 from git_mirror.manage_config import ConfigManager, default_config_path
 from git_mirror.menu import get_command_info
 from git_mirror.safe_env import load_env
+from git_mirror.ui import console_with_theme
 from git_mirror.version_check import display_version_check_message
 
 # Assuming RepoManager and other necessary imports are defined elsewhere
 
 load_env()
 
 LOGGER = logging.getLogger(__name__)
 
 backend = requests_cache.SQLiteCache(use_cache_dir=True, fast_save=True)
 
 requests_cache.install_cache("git_mirror_cache", backend=backend, expire_after=300)
 
+console = console_with_theme()
+
 
 def validate_host_token(args: argparse.Namespace) -> tuple[Optional[str], int]:
     """
     Get token from env or raise a helpful message.
 
     Args:
         args (argparse.Namespace): The parsed arguments.
@@ -45,48 +48,48 @@
     host = args.host if hasattr(args, "host") else None
     config_path = args.config_path if hasattr(args, "config_path") else default_config_path()
     # HACK: This needs to be redone somehow.
     config_manager = ConfigManager(config_path)
     invalid_or_missing_host = not host or host not in ("github", "gitlab", "selfhosted")
     needs_host = args.command not in ("init", "list-config")
     if invalid_or_missing_host and needs_host:
-        print(
+        console.print(
             "Please specify a host with --host or use gh_mirror for Github, gl_mirror for Gitlab, or sh_mirror for self hosted. "
             "Specify selfhosted in config file with a host_type of github or gitlab."
         )
         return "", 1
     if not needs_host:
         return None, 0
     config_data = config_manager.load_config(args.host)
     # github or self hosted github
     selfhosted_type_is_github = args.host == "selfhosted" and config_data and config_data.host_type == "github"
     selfhosted_type_is_gitlab = args.host == "selfhosted" and config_data and config_data.host_type == "gitlab"
     # SELFHOSTED_ACCESS_TOKEN
     if selfhosted_type_is_github or selfhosted_type_is_gitlab:
         token = os.getenv("SELFHOSTED_ACCESS_TOKEN")
         if selfhosted_type_is_github and not token:
-            print("Self hosted Github access token is missing. Setup and re-run command.")
+            console.print("Self hosted Github access token is missing. Setup and re-run command.")
             pat_init.setup_github_pat()
             return "", 1
         if selfhosted_type_is_gitlab and not token:
-            print(
+            console.print(
                 "Self hosted GitLab access token must be provided through SELFHOSTED_ACCESS_TOKEN environment variable."
             )
             pat_init_gitlab.setup_gitlab_pat()
             return "", 1
     elif args.host == "github" or selfhosted_type_is_github:
         token = os.getenv("GITHUB_ACCESS_TOKEN")
         if not token:
-            print("Github access token is missing. Setup and re-run command.")
+            console.print("Github access token is missing. Setup and re-run command.")
             pat_init.setup_github_pat()
             return "", 1
     elif args.host == "gitlab" or selfhosted_type_is_gitlab:
         token = os.getenv("GITLAB_ACCESS_TOKEN")
         if not token:
-            print("GitLab access token must be provided through GITLAB_ACCESS_TOKEN environment variable.")
+            console.print("GitLab access token must be provided through GITLAB_ACCESS_TOKEN environment variable.")
             pat_init_gitlab.setup_gitlab_pat()
             return "", 1
     elif args.command in ("init", "list-config"):
         token = None
     else:
         raise ValueError(f"Invalid host: {args.host}")
     return token, 0
@@ -103,15 +106,15 @@
     if (
         (not args.user_name or not args.target_dir)
         and not args.first_time_init
         and args.command not in ("init", "list-config")
     ):
         config_manager = ConfigManager(args.config_path)
         if not args.host:
-            print("Please specify a host, eg. --host github or --host gitlab.")
+            console.print("Please specify a host, eg. --host github or --host gitlab.")
             return domain, group_id, 1
         config_data = config_manager.load_config(args.host)
         config_path = args.config_path
         if config_data and config_path.exists():
             if not args.user_name:
                 args.user_name = config_data.user_name
             if not args.target_dir:
@@ -129,15 +132,15 @@
             if hasattr(args, "global_template_dir") and not args.global_template_dir:
                 args.global_template_dir = config_data.global_template_dir
     if (
         (not args.user_name or not args.target_dir)
         and not args.first_time_init
         and args.command not in ("init", "list-config")
     ):
-        print("user-name and target-dir are required if not specified in ~/git_mirror.toml.")
+        console.print("user-name and target-dir are required if not specified in ~/git_mirror.toml.")
         return domain, group_id, 1
     return domain, group_id, 0
 
 
 def enable_logging(args):
     # No logging above this line!
     if hasattr(args, "verbose") and args.verbose > 0:
@@ -175,14 +178,15 @@
         include_private=args.include_private,
         include_forks=args.include_forks,
         config_path=args.config_path,
         domain=domain,
         group_id=group_id,
         logging_level=args.verbose,
         dry_run=args.dry_run,
+        prompt_for_changes=not args.yes,
     )
 
 
 def handle_config(args: argparse.Namespace) -> None:
     router.route_config(
         command=args.command,
         config_path=args.config_path,
@@ -224,14 +228,15 @@
         host=args.host,
         include_private=args.include_private,
         include_forks=args.include_forks,
         domain=domain,
         logging_level=args.verbose,
         dry_run=args.dry_run,
         template_dir=args.global_template_dir,
+        prompt_for_changes=not args.yes,
     )
 
 
 def handle_simple(args: argparse.Namespace) -> None:
     router.route_simple(
         command=args.command,
         config_path=args.config_path,
@@ -395,15 +400,15 @@
             new_command = [selection] + original_arv[2:]
             args = parser.parse_args(new_command)
 
     args.use_github = use_github
     # UX - help user who doesn't enter any specific command and is likely just starting out
     args.first_time_init = False
     if not sys.argv[1:] and not default_config_path().exists():
-        print("This appears to be first time setup. Let's initialize configuration.")
+        console.print("This appears to be first time setup. Let's initialize configuration.")
         argv = ["init"]
         args.first_time_init = True
 
     enable_logging(args)
     LOGGER.debug(f"Cache store at {backend.db_path}")
 
     if use_github:
@@ -439,23 +444,26 @@
         help="Path to the TOML config file.",
     )
     parser.add_argument(
         "-v",
         "--verbose",
         action="count",
         default=0,
-        # shared=True,
         help="Verbose output, repeat for more verbose",
     )
     parser.add_argument(
         "--dry-run",
         action="store_true",
-        # shared=True,
         help="Don't change anything.",
     )
+    parser.add_argument(
+        "--yes",
+        action="store_true",
+        help="Don't prompt before slow actions or writes.",
+    )
 
 
 def host_specific_args(parser: argparse.ArgumentParser, use_github: bool, use_gitlab: bool, use_selfhosted: bool):
     host_choices = ["gitlab", "github"]
     if use_gitlab:
         host_choices = ["gitlab"]
         host_default = "gitlab"
```

### Comparing `git_mirror-0.3.6/git_mirror/bug_report.py` & `git_mirror-0.3.7/git_mirror/bug_report.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,27 +6,30 @@
 
 import github as gh
 from github.Issue import Issue
 from rich.console import Console
 from rich.panel import Panel
 from rich.text import Text
 
+from git_mirror.ui import console_with_theme
+
 LOGGER = logging.getLogger(__name__)
 
 
 class BugReporter:
     def __init__(self, token: str, repository_name: str) -> None:
         """
         Initializes the bug reporter with the GitHub API token and repository name.
 
         Args:
             token (str): The GitHub API token.
             repository_name (str): The full name of the repository (e.g., "user/repo").
         """
         try:
+            self.console = console_with_theme()
             self.github = gh.Github(token)
             self.repository_name = repository_name
             self.repo = self.github.get_repo(repository_name)
             self.user = self.github.get_user()
             self.invalid_token = False
         except gh.GithubException:
             self.invalid_token = True
@@ -55,18 +58,18 @@
 
         Args:
             issue_title (str): The title of the issue to be created.
             issue_body (str): The body text of the issue, providing details.
         """
         try:
             issue: Issue = self.repo.create_issue(title=issue_title, body=issue_body)
-            print(f"Issue titled '{issue_title}' created in {self.repository_name}.")
+            self.console.print(f"Issue titled '{issue_title}' created in {self.repository_name}.")
             return issue
         except gh.GithubException as e:
-            print(f"Failed to create issue in {self.repository_name}: {e}")
+            self.console.print(f"Failed to create issue in {self.repository_name}: {e}", style="danger")
         return None
 
     def find_existing_issue_by_title_and_creator(self, title: str) -> Optional[Issue]:
         """
         Searches for an existing issue by title and the issue creator.
 
         Args:
@@ -95,15 +98,15 @@
         traceback_details = traceback.format_exception(exc_type, exc_value, exc_traceback)
         issue_body = self.mask_secrets(f"An exception occurred:\n{''.join(traceback_details)}")
         issue_title = self.mask_secrets(f"Bug report: {exc_value}")
 
         # Check if the issue already exists
         existing_issue = self.find_existing_issue_by_title_and_creator(issue_title)
         if existing_issue:
-            print(f"An issue with the title '{issue_title}' has already been reported by you.")
+            self.console.print(f"An issue with the title '{issue_title}' has already been reported by you.")
             return
 
         # Ask the user for permission to report the bug
         console = Console()
         summary = Text.assemble(
             ("Issue Title: ", "bold cyan"),
             f"{issue_title}\n",
@@ -115,17 +118,19 @@
         response = input(
             "An error occurred. Would you like to report this bug? "
             "It will be posted as a public issue using your gitlab token as credentials. (yes/no): "
         )
         if response.lower().startswith("y"):
             issue = self.report_issue(issue_title, issue_body)
             if issue:
-                print(f"Bug report created at: {issue.html_url}")
+                console.print(f"Bug report created at: {issue.html_url}")
         else:
-            print("You can manually report this issue at https://github.com/matthewdeanmartin/git_mirror/issues")
+            console.print(
+                "You can manually report this issue at https://github.com/matthewdeanmartin/git_mirror/issues"
+            )
             LOGGER.info("Bug report canceled by the user.")
 
     def register_global_handler(self) -> None:
         """
         Registers the global exception handler to capture unhandled exceptions and report them as bugs.
         """
         if not self.invalid_token:
```

### Comparing `git_mirror-0.3.6/git_mirror/check_cli_deps.py` & `git_mirror-0.3.7/git_mirror/check_cli_deps.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 import cli_tool_audit as cta
 import cli_tool_audit.models as models
 
+from git_mirror.ui import console_with_theme
+
+console = console_with_theme()
+
 
 def check_tool_availability():
     """
     This function is used to check the availability of the 3rd party cli tools
     """
     git_version = models.CliToolConfig(
         name="git",
@@ -18,12 +22,12 @@
     )
     to_check = {
         "git": git_version,
         "poetry": poetry_version,
     }
     results = cta.process_tools(to_check, no_cache=True, disable_progress_bar=True)
     for result in results:
-        print(f"{result.tool}: available {result.is_available}, compatible {result.is_compatible}")
+        console.print(f"{result.tool}: available {result.is_available}, compatible {result.is_compatible}")
 
 
 if __name__ == "__main__":
     check_tool_availability()
```

### Comparing `git_mirror-0.3.6/git_mirror/cross_repo_sync.py` & `git_mirror-0.3.7/git_mirror/cross_repo_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 import shutil
 import sys
 from pathlib import Path
 
 from rich.console import Console
 from rich.text import Text
 
+from git_mirror.ui import console_with_theme
+
 LOGGER = logging.getLogger(__name__)
 
 
 class TemplateSync:
     """
     A class to synchronize template directories across multiple target directories, with detailed file comparison.
     """
@@ -35,14 +37,15 @@
         self.templates_dir = templates_dir
         self.console = Console()
         self.project_name_token = "{{{PROJECT_NAME}}}"  # nosec
         self.template_map_file = templates_dir / "template_map.txt"
         self.template_map = self.read_template_map()
         self.default_template = "default"
         self.use_default = use_default
+        self.console = console_with_theme()
 
     def read_template_map(self) -> dict[str, str]:
         if not self.template_map_file.exists():
             return {}
         with open(self.template_map_file, encoding="utf-8", newline=None) as template_map_handle:
             template_file_lines = template_map_handle.readlines()
         template_map = {}
@@ -64,33 +67,33 @@
         with open(self.template_map_file, "w", encoding="utf-8", newline=None) as template_map_handle:
             for path in missing_dirs:
                 if self.use_default:
                     template_map_handle.write(f"{path.name}:{self.default_template}\n")
                 else:
                     template_map_handle.write(f"{path.name}:\n")
         if not self.use_default:
-            print("Please fill in the template_map.txt file with the correct template for each project.")
-            print(f"File is located at {self.template_map_file}")
+            self.console.print("Please fill in the template_map.txt file with the correct template for each project.")
+            self.console.print(f"File is located at {self.template_map_file}")
             sys.exit(1)
 
     def get_template_dir(self, project: str) -> Path:
         return self.templates_dir / self.template_map[project]
 
     def report_differences(self, target_dirs: list[Path]) -> None:
         """
         Reports detailed differences between the template directory and each target directory.
         """
         self.write_template_map(target_dirs)
         differences = self._report_differences_data(target_dirs)
-        print(differences)
+        self.console.print(differences)
         for target_dir, diff_files in differences.items():
             if diff_files:
-                print(f"Differences in {target_dir}: {diff_files}")
+                self.console.print(f"Differences in {target_dir}: {diff_files}")
             else:
-                print(f"No differences in {target_dir}")
+                self.console.print(f"No differences in {target_dir}")
 
         self.report_content_differences(target_dirs)
 
     def _report_differences_data(self, target_dirs: list[Path]) -> dict[str, list[dict[str, str]]]:
         differences = {}
         for target_path in target_dirs:
             template_dir = self.get_template_dir(target_path.name)
```

### Comparing `git_mirror-0.3.6/git_mirror/custom_types.py` & `git_mirror-0.3.7/git_mirror/custom_types.py`

 * *Files identical despite different names*

### Comparing `git_mirror-0.3.6/git_mirror/file_system.py` & `git_mirror-0.3.7/git_mirror/file_system.py`

 * *Files identical despite different names*

### Comparing `git_mirror-0.3.6/git_mirror/logging_config.py` & `git_mirror-0.3.7/git_mirror/logging_config.py`

 * *Files identical despite different names*

### Comparing `git_mirror-0.3.6/git_mirror/manage_config.py` & `git_mirror-0.3.7/git_mirror/manage_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,20 +13,23 @@
 import tomlkit
 from rich.console import Console
 from rich.panel import Panel
 from rich.text import Text
 from tomlkit import TOMLDocument
 
 from git_mirror.safe_env import load_env
+from git_mirror.ui import console_with_theme
 
 load_env()
 
 # Configure logging
 LOGGER = logging.getLogger(__name__)
 
+console = console_with_theme()
+
 
 def default_config_path() -> Path:
     """This is only for defaults, if provided by user, let it throw."""
     try:
         path = Path("~/git_mirror.toml").expanduser()
         return path
     except RuntimeError:
@@ -65,15 +68,15 @@
     include_forks: bool = False
     group_id: int = 0
     global_template_dir: Optional[Path] = None
 
 
 def ask_for_section(already_configured: list[str]) -> Optional[ConfigData]:
     if len(already_configured) == 3:
-        print("All Github, Gitlab and a self-hosted Gitlab are already configured.")
+        console.print("All Github, Gitlab and a self-hosted Gitlab are already configured.")
         return None
     choices = ["github", "gitlab", "selfhosted"]
     for host in already_configured:
         choices.remove(host)
 
     first_questions = [
         inquirer.List(
@@ -90,15 +93,15 @@
     answers = inquirer.prompt(first_questions)
 
     target_dir = Path(answers["target_dir"]).expanduser()
     while not target_dir.exists():
         answer = inquirer.prompt(
             [inquirer.Confirm("create_target_dir", message="Target directory does not exist. Create it?", default=True)]
         )
-        print(answer)
+        console.print(answer)
         if answer["create_target_dir"]:
             os.makedirs(target_dir)
         else:
             target_dir_answer = inquirer.prompt([inquirer.Text("target_dir", message="Enter the target directory")])
             target_dir = Path(target_dir_answer).expanduser()
 
     host_type = answers["host_type"]
@@ -182,15 +185,15 @@
         found = 0
         for host_type in ["selfhosted", "gitlab", "github"]:
             data = self.load_config(host_type)
             if data:
                 found += 1
                 display_config(data)
         if not found:
-            print("No configuration found. Run `git-mirror init` to create a new configuration.")
+            console.print("No configuration found. Run `git-mirror init` to create a new configuration.")
 
     def initialize_config(self) -> list[str]:
         already_configured: list[str] = []
         while len(already_configured) < 3:
             toml_config, git_mirror_section = self.load_if_exists()
 
             def already(gm) -> list[str]:
@@ -198,25 +201,25 @@
                 already_done = []
                 for host_type in ["selfhosted", "gitlab", "github"]:
                     if host_type in gm:
                         already_done.append(host_type)
                 return already_done
 
             already_configured = already(git_mirror_section)
-            print(f"Already configured: {already_configured}")
+            console.print(f"Already configured: {already_configured}")
             config_section = ask_for_section(already_configured)
             if not config_section:
                 break
 
             if toml_config["tool"]["git-mirror"].get(config_section.host_type, {}):  # type: ignore
                 raise ValueError(
                     f"Configuration for {config_section.host_type} " f"already exists in {self.config_path.resolve()}"
                 )
             if config_section.target_dir and not config_section.target_dir.exists():
-                print(f"Creating directory {config_section.target_dir}")
+                console.print(f"Creating directory {config_section.target_dir}")
                 os.makedirs(config_section.target_dir)
 
             if config_section.host_type not in ("github", "gitlab"):
                 raise ValueError(f"host_type must be github or gitlab even if self hosted. {config_section.host_type}")
             section = {
                 "host_type": config_section.host_type,
                 "host_url": config_section.host_url,
@@ -256,15 +259,15 @@
             if not tool_config:
                 return None
             target_dir = tool_config.get("target_dir")
             if not target_dir:
                 raise ValueError(f"target_dir not found in config file at {self.config_path.resolve()}")
 
             if target_dir and not Path(target_dir).exists():
-                print(f"Creating directory {target_dir}")
+                console.print(f"Creating directory {target_dir}")
                 os.makedirs(target_dir)
             data = ConfigData(
                 host,
                 tool_config.get("host_type", host),
                 tool_config.get("host_url", ""),
                 tool_config.get("user_name"),
                 target_dir,
@@ -318,15 +321,15 @@
         # Remove repositories no longer present
         for repo_name in list(git_mirror.keys()):
             if repo_name not in repos:
                 del git_mirror[repo_name]
 
         config["tool"]["git-mirror"][host]["repos"] = git_mirror  # type: ignore
 
-        print(f"Syncing configuration with {len(repos)} repositories to {self.config_path.resolve()}")
+        console.print(f"Syncing configuration with {len(repos)} repositories to {self.config_path.resolve()}")
         with open(self.config_path, "w", encoding="utf-8") as file:
             file.write(tomlkit.dumps(config))
 
         return config
 
     def load_if_exists(self) -> tuple[TOMLDocument, dict[str, Any]]:
         if self.config_path.exists():
```

### Comparing `git_mirror-0.3.6/git_mirror/manage_git.py` & `git_mirror-0.3.7/git_mirror/manage_git.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 """
 Pure git actions.
 """
 
 import logging
+import multiprocessing
+import os
 from pathlib import Path
 
 import git as g
-from termcolor import colored
 
+from git_mirror.performance import log_duration
 from git_mirror.safe_env import load_env
+from git_mirror.ui import console_with_theme
 
 load_env()
 
 # Configure logging
 LOGGER = logging.getLogger(__name__)
 
 
 def find_git_repos(base_dir: Path) -> list[Path]:
     """
-    Recursively finds all Git repositories in the given base directory.
+    Recursively finds all Git repositories in the given base directory using two methods:
+    First, it uses `os.walk`, and then it uses `pathlib.Path.rglob` to ensure no repositories are missed.
 
     Args:
         base_dir (Path): The base directory to search for Git repositories.
 
     Returns:
         List[Path]: A list of Paths representing the Git repositories found.
     """
-    git_repos = []
+    git_repos_set = set()
 
-    for path in base_dir.rglob("*"):
-        if path.name == ".git" and path.is_dir():
-            git_repos.append(path.parent)  # Add the parent directory of '.git'
+    # Rlgob is 2x slower
+    for root, dirs, _ in os.walk(base_dir):
+        if ".git" in dirs:
+            git_repos_set.add(Path(root))
 
+    git_repos = list(git_repos_set)
     return git_repos
 
 
 def extract_repo_name(remote_url: str) -> str:
     """
     Extracts the repository name from its remote URL.
 
@@ -60,23 +66,27 @@
 
 
 class GitManager:
     def __init__(
         self,
         base_dir: Path,
         dry_run: bool = False,
+        prompt_for_changes: bool = True,
     ):
         """
         Initializes base directory for git operations.
 
         Args:
             base_dir (Path): Base directory path where repositories will be cloned.
             dry_run (bool): Flag to determine whether the operation should be a dry run.
+            prompt_for_changes (bool): Flag to determine whether the operation should prompt for changes.
         """
         self.base_dir = base_dir
+        self.dry_run = dry_run
+        self.prompt_for_changes = prompt_for_changes
 
     def local_repos_with_file_in_root(self, file_name: str) -> list[Path]:
         """
         Finds local git repositories within the base directory that have a specific file in their root.
 
         Args:
             file_name (str): The name of the file to search for in the root of each repository.
@@ -89,72 +99,82 @@
             if repo_dir.is_dir() and (repo_dir / ".git").exists():
                 target_file_path = repo_dir / file_name
                 if target_file_path.exists():
                     LOGGER.info(f"Found {file_name} in {repo_dir}")
                     found_repos.append(repo_dir)
         return found_repos
 
-    def check_for_uncommitted_or_unpushed_changes(self) -> list[str]:
+    @log_duration
+    def check_for_uncommitted_or_unpushed_changes(self, single_threaded: bool = False) -> int:
         """
         Checks all local repositories for uncommitted changes or commits that haven't been pushed to the remote.
         """
-        messages = []
+        console = console_with_theme()
+        repos = list(find_git_repos(self.base_dir))
+        console.print(f"Checking {len(repos)} repositories for uncommitted changes and unpushed commits.")
         have_uncommitted = 0
-        for repo_dir in find_git_repos(self.base_dir):
-            if repo_dir.is_dir():
-                try:
-                    repo = g.Repo(repo_dir)
-                    conclusion = ""
-                    if repo.is_dirty(untracked_files=True):
-                        conclusion = f"{repo_dir} has uncommitted changes."
-                        have_uncommitted += 1
-                    else:
-                        LOGGER.debug(f"{repo_dir} has no uncommitted changes.")
+        if single_threaded or len(repos) < 2:
+            for repo_dir in repos:
+                have_uncommitted += self.check_single_repo(repo_dir)
+        else:
+            with multiprocessing.Pool(multiprocessing.cpu_count()) as pool:
+                # TODO: may need to figure out how to add a lock for print()
+                # manager = multiprocessing.Manager()
+                # lock = manager.Lock()
+                results = pool.starmap(self.check_single_repo, [(repo_dir,) for repo_dir in repos])
+                have_uncommitted = sum(results)
+        if have_uncommitted == 0:
+            console.print("All repositories are clean, no uncommitted changes.")
+        return have_uncommitted
+
+    def check_single_repo(self, repo_dir: Path) -> int:
+        console = console_with_theme()
+        have_uncommitted = 0
+        if repo_dir.is_dir():
+            try:
+                repo = g.Repo(repo_dir)
+                conclusion = ""
+                if repo.is_dirty(untracked_files=True):
+                    conclusion = f"{repo_dir} has uncommitted changes."
+                    have_uncommitted = 1
+                else:
+                    LOGGER.debug(f"{repo_dir} has no uncommitted changes.")
 
-                    if conclusion:
-                        print(colored(conclusion, "red"))
+                if conclusion:
+                    console.print(conclusion)
 
-                    self._check_for_unpushed_commits(repo, repo_dir)
+                self._check_for_unpushed_commits(repo, repo_dir)
 
-                except g.InvalidGitRepositoryError:
-                    message = f"{repo_dir} is not a valid Git repository."
-                    messages.append(message)
-                    LOGGER.warning(message)
-                except Exception as e:
-                    message = f"Error checking {repo_dir}: {e}"
-                    messages.append(message)
-                    LOGGER.error(message)
-        if have_uncommitted == 0:
-            print(colored("All repositories are clean, no uncommitted changes.", "green"))
-        return messages
+            except g.InvalidGitRepositoryError:
+                console.print(f"{repo_dir} is not a valid Git repository.")
+            except Exception as e:
+                console.print(f"Error checking {repo_dir}: {e}", style="danger")
+        return have_uncommitted
 
-    def _check_for_unpushed_commits(self, repo: g.Repo, repo_dir: Path) -> list[str]:
+    def _check_for_unpushed_commits(self, repo: g.Repo, repo_dir: Path) -> int:
         """
         Checks if the repository has commits that haven't been pushed to its tracked remote branches.
 
         Args:
             repo (Repo): The repository object.
             repo_dir (Path): The directory of the repository.
         """
-        messages = []
+        console = console_with_theme()
+        branches_checked = 0
         for branch in repo.heads:  # branches. Mypy doesn't like the alias.
+            branches_checked += 1
             try:
                 # Compare local branch commit with remote branch commit
                 if branch.tracking_branch():
                     ahead_count, _behind_count = repo.iter_commits(
                         f"{branch}..{branch.tracking_branch()}"
                     ), repo.iter_commits(f"{branch.tracking_branch()}..{branch}")
                     if sum(1 for _ in ahead_count) > 0:
-                        message = f"{repo_dir} has unpushed commits on branch {branch}."
-                        messages.append(message)
+                        console.print(f"{repo_dir} has unpushed commits on branch {branch}.")
                     else:
-                        message = f"{repo_dir} is up to date with remote on branch {branch}."
-                        messages.append(message)
+                        LOGGER.info(f"{repo_dir} is up to date with remote on branch {branch}.")
                 else:
-                    message = f"{repo_dir} branch {branch} does not track a remote."
-                    messages.append(message)
+                    console.print(f"{repo_dir} branch {branch} does not track a remote.")
             except g.GitCommandError as e:
                 message = f"Error checking for unpushed commits in {repo_dir} on branch {branch}: {e}"
-                LOGGER.error(message)
-                messages.append(message)
-
-        return messages
+                console.print(message, style="danger")
+        return branches_checked
```

### Comparing `git_mirror-0.3.6/git_mirror/manage_github.py` & `git_mirror-0.3.7/git_mirror/manage_github.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,26 +14,27 @@
 import git as g
 import github as gh
 import github.AuthenticatedUser as ghau
 import github.NamedUser as ghnu
 import github.Repository as ghr
 import httpx
 import inquirer
-from rich.console import Console
 from rich.panel import Panel
 from rich.table import Table
 from rich.text import Text
 from termcolor import colored
 
 import git_mirror.manage_git as mg
 from git_mirror.cross_repo_sync import TemplateSync
 from git_mirror.custom_types import SourceHost, UpdateBranchArgs
 from git_mirror.dummies import Dummy
 from git_mirror.manage_pypi import PyPiManager, pretty_print_pypi_results
+from git_mirror.performance import log_duration
 from git_mirror.safe_env import load_env
+from git_mirror.ui import console_with_theme
 
 load_env()
 
 # Configure logging
 LOGGER = logging.getLogger(__name__)
 
 
@@ -43,37 +44,40 @@
         token: str,
         base_dir: Path,
         user_login: str,
         include_private: bool = True,
         include_forks: bool = False,
         host_domain: str = "https://github.com",
         dry_run: bool = False,
+        prompt_for_changes: bool = True,
     ):
         """
         Initializes the RepoManager with a GitHub token and a base directory for cloning repositories.
 
         Args:
             token (str): GitHub personal access token.
             base_dir (Path): Base directory path where repositories will be cloned.
             user_login (str): The GitHub username.
             include_private (bool): Whether to include private repositories.
             include_forks (bool): Whether to include forked repositories.
             host_domain (str): The domain of the GitHub instance.
             dry_run (bool): Whether to perform a dry run.
+            prompt_for_changes (bool): Whether to prompt for changes.
         """
         # self.client() = gh.Github(token)
         self.token = token
         self.base_dir = base_dir
         # cache user
         self.user: Optional[Union[ghnu.NamedUser, ghau.AuthenticatedUser]] = None
         self.user_login = user_login
         self.include_private = include_private
         self.include_forks = include_forks
         self.host_domain = host_domain
         self.dry_run = dry_run
+        self.prompt_for_changes = prompt_for_changes
         LOGGER.debug(
             f"GithubRepoManager initialized with user_login: {user_login}, include_private: {include_private}, include_forks: {include_forks}"
         )
 
     def client(self) -> gh.Github:
         return gh.Github(self.token)
 
@@ -87,222 +91,255 @@
                     "private": "Yes" if repo.private else "No",
                     "fork": "Yes" if repo.fork else "No",
                     "html_url": repo.html_url,
                 }
             )
         return repos
 
-    def _get_user_repos(
-        self,
-    ) -> list[ghr.Repository]:
+    def _get_user_repos(self, ignore_users_filters: bool = False) -> list[ghr.Repository]:
         """
         Fetches the user's repositories from GitHub, optionally including private repositories and forks.
 
         Returns:
             list[Repository]: A list of Repository objects.
         """
+        console = console_with_theme()
         if not self.user:
             self.user = self.client().get_user()
 
         try:
             repos = []
             for repo in self.user.get_repos():
-                if (
+                # ignore user's filters when checking if something local isn't a remote repo.
+                if ignore_users_filters or (
                     (self.include_private or not repo.private)
                     and (self.include_forks or not repo.fork)
                     and repo.owner.login == self.user_login
                 ):
                     repos.append(repo)
 
             return repos
         except gh.GithubException as e:
-            LOGGER.error(f"Failed to fetch repositories: {e}")
+            console.print(f"Failed to fetch repositories: {e}", style="danger")
             return []
 
+    @log_duration
     def clone_all(self, single_threaded: bool = False):
+        console = console_with_theme()
         repos = self._get_user_repos()
-        print(f"Cloning {len(repos)} repositories.")
+        if self.prompt_for_changes:
+            answer = inquirer.prompt(
+                [
+                    inquirer.Confirm(
+                        "clone-all", message=f"Are you sure you want to clone {len(repos)} repositories?", default=False
+                    )
+                ]
+            )
+            if not answer["clone-all"]:
+                console.print("Cloning cancelled.")
+                return
+
+        console.print(f"Cloning {len(repos)} repositories.")
+
         if single_threaded or len(repos) < 4:  # or features.CACHING:
             for repo in self._thread_safe_repos(repos):
                 self._clone_repo((repo, Dummy()))
         else:
             with multiprocessing.Pool(multiprocessing.cpu_count()) as pool:
                 manager = multiprocessing.Manager()
                 lock = manager.Lock()
                 results = pool.map(self._clone_repo, [(repo, lock) for repo in self._thread_safe_repos(repos)])
                 for output in results:
                     if output:
-                        print(output, end="")
+                        console.print(output, end="")
 
     def _clone_repo(self, repo_args: tuple[dict[str, Any], ContextManager[Any]]) -> None:
         """
         Clones the given repository into the target directory.
 
         Args:
             repo_args (tuple[dict[str, Any], ContextManager[Any]]): A tuple containing the repository data and a lock.
 
         Returns:
         str: The captured print output.
         """
+        console = console_with_theme()
         repo, lock = repo_args
         try:
             if not (self.base_dir / repo["name"]).exists():
                 if not self.dry_run:
                     message = f"Cloning {repo['html_url']} into {self.base_dir}"
                     with lock:
-                        print(message)
+                        console.print(message)
                     g.Repo.clone_from(f"{repo['html_url']}.git", self.base_dir / repo["name"])
                 else:
                     message = f"Would have cloned {repo['html_url']} into {self.base_dir}"
                     with lock:
-                        print(message)
+                        console.print(message)
             else:
                 message = f"Repository {repo['name']} already exists locally. Skipping clone."
                 with lock:
-                    print(message)
+                    console.print(message)
         except g.GitCommandError as e:
             message = f"Failed to clone {repo['name']}: {e}"
             with lock:
-                print(message)
+                console.print(message, style="danger")
 
+    @log_duration
     def pull_all(self, single_threaded: bool = False):
+        console = console_with_theme()
         directories = mg.find_git_repos(self.base_dir)
-        print(f"Pulling {len(directories)} repositories.")
+        console.print(f"Pulling {len(directories)} repositories.")
         if single_threaded or len(directories) < 4:
             for repo_dir in directories:
                 self.pull_repo((repo_dir, Dummy()))
         else:
             with multiprocessing.Pool(multiprocessing.cpu_count()) as pool:
                 manager = multiprocessing.Manager()
                 lock = manager.Lock()
-                results = pool.map(self.pull_repo, (print(repo_dir) or (repo_dir, lock) for repo_dir in directories))
+                results = pool.map(self.pull_repo, ((repo_dir, lock) for repo_dir in directories))
                 for output in results:
                     if output:
-                        print(output, end="")
+                        console.print(output, end="")
 
+    @log_duration
     def pull_repo(self, args: tuple[Path, ContextManager[Any]]) -> None:
         """
         Performs a git pull operation on the repository at the given path.
 
         Args:
             args (tuple[Path, ContextManager[Any]]): A tuple containing the path to the repository and a lock.
 
         Returns:
             str: The captured print output.
         """
+        console = console_with_theme()
         repo_path, lock = args
         try:
             repo = g.Repo(repo_path)
             origin = repo.remotes.origin
             if not self.dry_run:
                 with lock:
-                    print(f"Pulling latest changes in {repo_path}")
+                    console.print(f"Pulling latest changes in {repo_path}")
                 origin.pull()
             else:
                 with lock:
-                    print(f"Would have pulled latest changes in {repo_path}")
+                    console.print(f"Would have pulled latest changes in {repo_path}")
         except Exception as e:
             with lock:
-                print(f"Failed to pull repo at {repo_path}: {e}")
+                console.print(f"Failed to pull repo at {repo_path}: {e}", style="danger")
 
+    @log_duration
     def not_repo(self) -> tuple[int, int, int, int]:
         """
         Lists directories in the base directory that are not valid Git repositories,
         or are not owned by the user, or are forks of another repository.
 
         Uses both git and github because of fork checking.
         """
-        user_repos = {repo.name: repo for repo in self._get_user_repos()}
+        console = console_with_theme()
+        user_repos = {repo.name: repo for repo in self._get_user_repos(ignore_users_filters=True)}
 
         no_remote = 0
         not_found = 0
         is_fork = 0
         not_repo = 0
-        for repo_dir in mg.find_git_repos(self.base_dir):
+        repos = mg.find_git_repos(self.base_dir)
+        console.print(f"Checking {len(repos)} repositories for stray, non-repo subfolders in {self.base_dir}.")
+        for repo_dir in repos:
             if repo_dir.is_dir():
                 try:
                     repo = g.Repo(repo_dir)
                     remotes = repo.remotes
                     if not remotes:
                         no_remote += 1
-                        print(f"{repo_dir} has no remote repositories defined.")
+                        console.print(f"{repo_dir} has no remote repositories defined.")
                         continue
 
                     remote_url = remotes[0].config_reader.get("url")
                     repo_name = mg.extract_repo_name(remote_url)
 
                     if repo_name not in user_repos:
                         not_found += 1
-                        print(f"{repo_dir} is not found in your GitHub account.")
+                        console.print(f"{repo_dir} is not found in your GitHub account.")
                         continue
 
                     github_repo = user_repos[repo_name]
                     if github_repo.fork:
                         is_fork += 1
-                        print(f"{repo_dir} is a fork of another repository.")
+                        console.print(f"{repo_dir} is in your account, but is a fork of another user's repository.")
                         continue
 
                 except g.InvalidGitRepositoryError:
                     not_repo += 1
-                    print(f"{repo_dir} is not a valid Git repository.")
+                    console.print(f"{repo_dir} is not a valid Git repository.", style="danger")
         return no_remote, not_found, is_fork, not_repo
 
+    @log_duration
     def list_repo_builds(self) -> list[tuple[str, str]]:
         """
         Lists the most recent GitHub Actions workflow runs for each repository of the authenticated user,
         with the status color-coded: green for success, red for failure, and yellow for cancelled.
         """
+        console = console_with_theme()
         if not self.user:
             self.user = self.client().get_user()
 
         messages = []
-        for repo in self._get_user_repos():
-            print(f"Repository: {repo.name}")
+        repos = self._get_user_repos()
+        console.print(f"Checking {len(repos)} repositories for build statuses.")
+        for repo in repos:
+            console.print(f"Repository: {repo.name}")
             statuses = repo.get_workflow_runs()
             messages.extend(self._loop_actions(statuses))
         return messages
 
     def _loop_actions(self, statuses) -> list[tuple[str, str]]:
+        console = console_with_theme()
         actions_per_repo = 1
         status_count = 0
         messages = []
         for action in statuses:
             if status_count >= actions_per_repo:
                 break
             status_count += 1
 
             status_message = f"Date: {action.created_at} - {action.display_title} - Conclusion - {action.conclusion}  Status: {action.status} - URL: {action.html_url}"
             conclusion = (action.conclusion or "").lower()
             messages.append((conclusion, status_message))
             if conclusion == "success":
-                print(colored(status_message, "green"))
+                console.print(colored(status_message, "green"))
             elif conclusion == "failure":
-                print(colored(status_message, "red"))
+                console.print(colored(status_message, "red"))
             elif conclusion == "cancelled":
-                print(colored(status_message, "yellow"))
+                console.print(colored(status_message, "yellow"))
             else:
-                print(status_message)  # Default, no color
+                console.print(status_message)  # Default, no color
         return messages
 
+    @log_duration
     def check_pypi_publish_status(self, pypi_owner_name: Optional[str] = None) -> list[dict[str, Any]]:
         """
         Checks if the repositories as Python packages are published on PyPI and compares the last change dates.
         """
+        console = console_with_theme()
         results = []
         if pypi_owner_name:
             pypi_owner_name = pypi_owner_name.strip().lower()
 
         async def get_infos_async(package_names):
             pypi_manager = PyPiManager()
             return await pypi_manager.get_infos(package_names)
 
         package_names = [path.name for path in mg.find_git_repos(self.base_dir)]
         package_infos = asyncio.run(get_infos_async(package_names))
 
-        for repo_dir in mg.find_git_repos(self.base_dir):
+        repos = mg.find_git_repos(self.base_dir)
+        console.print(f"Checking {len(repos)} repositories for PyPI publish status.")
+        for repo_dir in repos:
             if repo_dir.is_dir():
                 try:
                     repo = g.Repo(repo_dir)
                     package_name = repo_dir.name  # Assuming the repo name is the package name
 
                     pypi_data, status_code = package_infos[package_name]
                     any_owner_is_fine = pypi_owner_name is None
@@ -324,15 +361,16 @@
                                 "Days difference": days_difference,
                             }
                         )
                 except g.InvalidGitRepositoryError:
                     LOGGER.warning(f"{repo_dir} is not a valid Git repository.")
                 except Exception as e:
                     LOGGER.error(f"Error checking {repo_dir}: {e}")
-        print(pretty_print_pypi_results(results))
+        print()
+        console.print(pretty_print_pypi_results(results))
         return results
 
     @classmethod
     def _get_latest_commit_date(self, repo: g.Repo) -> datetime:
         """
         Gets the date of the latest commit in the repository.
 
@@ -341,27 +379,30 @@
 
         Returns:
             datetime: The datetime of the latest commit.
         """
         last_commit = next(repo.iter_commits())
         return datetime.fromtimestamp(last_commit.committed_date)
 
+    @log_duration
     def list_repo_names(self) -> list[str]:
         """
         Returns a list of repository names.
 
         Returns:
             List[str]: A list of repository names.
         """
         return [repo.full_name for repo in self._get_user_repos()]
 
+    @log_duration
     def list_repos(self) -> Optional[Table]:
         """
         Fetches and prints beautifully formatted information about the user's GitHub repositories.
         """
+        console = console_with_theme()
         try:
             user = self.client().get_user(self.user_login)
             repos = user.get_repos()
             table = Table(title="GitHub Repositories")
 
             table.add_column("Name", style="cyan", no_wrap=True)
             table.add_column("Description", style="magenta")
@@ -375,26 +416,26 @@
                         repo.name,
                         repo.description or "No description",
                         # repo.html_url, # doesn't fit
                         "Yes" if repo.private else "No",
                         "Yes" if repo.fork else "No",
                     )
 
-            console = Console()
             console.print(table)
             return table
         except gh.GithubException as e:
-            print(f"An error occurred: {e}")
+            console.print(f"An error occurred: {e}", style="danger")
         return None
 
+    @log_duration
     def print_user_summary(self) -> None:
         """
         Fetches and prints a summary of the user's GitHub account.
         """
-        console = Console()
+        console = console_with_theme()
         try:
             user = self.client().get_user(self.user_login)
             summary = Text.assemble(
                 ("Username: ", "bold cyan"),
                 f"{user.login}\n",
                 ("Name: ", "bold cyan"),
                 f"{user.name}\n",
@@ -411,55 +452,58 @@
                 ("Company: ", "bold cyan"),
                 f"{user.company or 'Not specified'}",
             )
             console.print(Panel(summary, title="GitHub User Summary", subtitle=user.login))
         except gh.GithubException as e:
             console.print(f"An error occurred: {e}", style="bold red")
 
+    @log_duration
     def update_all_branches(self, single_threaded: bool = False, prefer_rebase: bool = False):
         """
         Updates each local branch with the latest changes from the main/master branch on GitHub.
 
         Args:
             single_threaded (bool): Whether to run the operation in a single thread.
             prefer_rebase (bool): Whether to prefer rebasing instead of merging.
         """
+        console = console_with_theme()
         directories = mg.find_git_repos(self.base_dir)
-        print(f"Merging/rebasing {len(directories)} main to local repositories.")
+        console.print(f"Merging/rebasing {len(directories)} main to local repositories.")
         if single_threaded or len(directories) < 4:
             for repo_dir in directories:
                 self._update_local_branches(UpdateBranchArgs(repo_dir, repo_dir.name, prefer_rebase, Dummy()))
         else:
             with multiprocessing.Pool(multiprocessing.cpu_count()) as pool:
                 manager = multiprocessing.Manager()
                 lock = manager.Lock()
                 results = pool.map(
                     self._update_local_branches,
                     (UpdateBranchArgs(repo_dir, repo_dir.name, prefer_rebase, lock) for repo_dir in directories),
                 )
                 for output in results:
                     if output:
                         if output:
-                            print(output, end="")
+                            console.print(output, end="")
 
     # def _update_local_branches(self, repo_path: Path, github_repo_full_name: str, prefer_rebase: bool = False):
     def _update_local_branches(self, args: UpdateBranchArgs):
         """
         Updates each local branch with the latest changes from the main/master branch on GitHub.
 
         Args:
             args: UpdateBranchArgs
         """
+        console = console_with_theme()
         repo_path, github_repo_full_name, prefer_rebase = args.repo_path, args.github_repo_full_name, args.prefer_rebase
         github_repo_full_name = self.user_login + "/" + github_repo_full_name
         repo = g.Repo(str(repo_path))
         try:
             github_repo = self.client().get_repo(github_repo_full_name)
         except gh.GithubException as e:
-            print(f"Failed to retrieve info on GitHub repository {github_repo_full_name}: {e}")
+            console.print(f"Failed to retrieve info on GitHub repository {github_repo_full_name}: {e}", style="danger")
             return
         # Get the default branch name from GitHub
         default_branch = github_repo.default_branch
 
         # Fetch all changes from remote
         origin = repo.remotes.origin
         if not self.dry_run:
@@ -479,125 +523,160 @@
                     if prefer_rebase:
                         # Perform rebase
                         repo.git.rebase(f"origin/{default_branch}")
                     else:
                         # Perform merge
                         repo.git.merge(f"origin/{default_branch}")
 
-                    print(f"Updated branch '{branch}' with latest changes from '{default_branch}'.")
+                    console.print(f"Updated branch '{branch}' with latest changes from '{default_branch}'.")
                 else:
-                    print(f"Would have updated branch '{branch}' with latest changes from '{default_branch}'.")
+                    console.print(f"Would have updated branch '{branch}' with latest changes from '{default_branch}'.")
             except g.exc.GitCommandError as e:
-                print(f"Failed to update branch '{branch}': {e}")
+                console.print(f"Failed to update branch '{branch}': {e}", style="danger")
 
+    @log_duration
     def prune_all(self) -> None:
-        for repo_dir in mg.find_git_repos(self.base_dir):
+        """
+        Prunes all local branches that have been deleted on GitHub.
+        """
+        console = console_with_theme()
+        repos = mg.find_git_repos(self.base_dir)
+        console.print(f"Ready to Pruning {len(repos)} repositories of branches no longer on remote.")
+        if self.prompt_for_changes:
+            answer = inquirer.prompt(
+                [inquirer.Confirm("prune", message="Are you sure you want to prune all repositories?", default=False)]
+            )
+            if not answer["prune"]:
+                console.print("Pruning cancelled.")
+                return
+
+        for repo_dir in repos:
             if repo_dir.is_dir():
                 self._delete_local_branches_if_not_on_github(repo_dir, f"{self.user_login}/{repo_dir.name}")
 
     def _delete_local_branches_if_not_on_github(self, repo_path: Path, github_repo_full_name: str):
         """
         Loops through all local branches, checks if they exist on GitHub, and prompts the user for deletion if they don't.
 
         Args:
             repo_path (Path): The file system path to the local git repository.
             github_repo_full_name (str): The full name of the GitHub repository (e.g., "owner/repo").
         """
-        # Initialize GitHub client and GitPython Repo
+        console = console_with_theme()
         try:
             repo = g.Repo(str(repo_path))
         except g.InvalidGitRepositoryError:
-            print(f"{repo_path} is not a valid Git repository.")
+            console.print(f"{repo_path} is not a valid Git repository.", style="danger")
             return
         try:
             github_repo = self.client().get_repo(github_repo_full_name)
         except gh.GithubException as e:
-            print(f"Failed to retrieve info on GitHub repository {github_repo_full_name}: {e}")
+            console.print(f"Failed to retrieve info on GitHub repository {github_repo_full_name}: {e}", style="danger")
             return
 
         # Get a list of all branch names on GitHub
         remote_branches = [branch.name for branch in github_repo.get_branches()]
 
         # Get a list of all local branch names
         local_branches = [branch.name for branch in repo.heads]  # alias to branches
 
         # Determine branches that are local but not on GitHub
         branches_to_consider = [branch for branch in local_branches if branch not in remote_branches]
 
         if not branches_to_consider:
-            print(f"For {github_repo_full_name}, no local branches exist that are missing on GitHub.")
+            console.print(f"For {github_repo_full_name}, no local branches exist that are missing on GitHub.")
             return
 
         # Prompt user for each branch that doesn't exist on GitHub
         for branch in branches_to_consider:
-            question = [
-                inquirer.Confirm(
-                    "delete", message=f"The branch '{branch}' does not exist on GitHub. Delete locally?", default=False
-                )
-            ]
-            answer = inquirer.prompt(question)
+            if self.prompt_for_changes:
+                question = [
+                    inquirer.Confirm(
+                        "delete",
+                        message=f"The branch '{branch}' does not exist on GitHub. Delete locally?",
+                        default=False,
+                    )
+                ]
+                answer = inquirer.prompt(question)
 
-            if answer["delete"]:
-                try:
-                    if not self.dry_run:
-                        # Safely delete the branch
-                        repo.git.branch("-d", branch)
-                        print(f"Deleted branch '{branch}' locally.")
-                    else:
-                        print(f"Would have deleted branch '{branch}' locally.")
-                except g.exc.GitCommandError as e:
-                    print(f"Could not delete branch '{branch}'. It may not be fully merged. Error: {e}")
-            else:
-                print(f"Skipped deletion of branch '{branch}'.")
+                if not answer["delete"]:
+                    console.print(f"Skipped deletion of branch '{branch}'.")
+                    continue
+            try:
+                if not self.dry_run:
+                    # Safely delete the branch
+                    repo.git.branch("-d", branch)
+                    console.print(f"Deleted branch '{branch}' locally.")
+                else:
+                    console.print(f"Would have deleted branch '{branch}' locally.")
+            except g.exc.GitCommandError as e:
+                console.print(
+                    f"Could not delete branch '{branch}'. It may not be fully merged. Error: {e}", style="danger"
+                )
 
+    @log_duration
     def version_info(self) -> dict[str, Any]:
         """
         Return API version information.
         """
         # pygithub doesn't support this endpoint?
         response = httpx.get(f"{self.host_domain}/versions")
         response.raise_for_status()  # Raises an exception for 4XX/5XX responses
         data = response.json()
         versions_supported = data["info"]["version"]
         return {"version": versions_supported}
 
+    @log_duration
     def cross_repo_sync_report(self, template_dir: Path) -> None:
         """
         Reports differences between the template directory and the target directories.
         """
+        console = console_with_theme()
         if not template_dir or not template_dir.exists():
-            print(f"Template directory {template_dir} does not exist.")
+            console.print(f"Template directory {template_dir} does not exist.")
             return
         # right now just the easy case of all repos need to match 1 template_dir
-        print("Reporting differences between the template directory and the target directories.")
+        console.print("Reporting differences between the template directory and the target directories.")
         syncer = TemplateSync(template_dir)
         directories = mg.find_git_repos(self.base_dir)
-        print(f"Found {len(directories)} repositories.")
+        console.print(f"Found {len(directories)} repositories.")
         syncer.report_content_differences(directories)
 
-    def cross_repo_init(self, template_dir: Path):
+    @log_duration
+    def cross_repo_init(self, template_dir: Path) -> None:
+        console = console_with_theme()
         if not template_dir or not template_dir.exists():
-            print(f"Template directory {template_dir} does not exist.")
+            console.print(f"Template directory {template_dir} does not exist.")
             return
         syncer = TemplateSync(template_dir, use_default=True)
         directories = mg.find_git_repos(self.base_dir)
-        print(f"Found {len(directories)} repositories.")
+        console.print(f"Found {len(directories)} repositories.")
         syncer.write_template_map(directories)
-        print(f"Initialized template map for {len(directories)} repositories.")
+        console.print(f"Initialized template map for {len(directories)} repositories.")
 
-    def cross_repo_sync(self, template_dir: Path):
+    @log_duration
+    def cross_repo_sync(self, template_dir: Path) -> None:
+        console = console_with_theme()
         if not template_dir or not template_dir.exists():
-            print(f"Template directory {template_dir} does not exist.")
+            console.print(f"Template directory {template_dir} does not exist.")
             return
         syncer = TemplateSync(template_dir, use_default=True)
         directories = mg.find_git_repos(self.base_dir)
-        print(f"Found {len(directories)} repositories.")
+        console.print(f"Found {len(directories)} repositories.")
+        if self.prompt_for_changes:
+            answer = inquirer.prompt(
+                [inquirer.Confirm("sync", message="Are you sure you want to sync all repositories?", default=False)]
+            )
+            if not answer["sync"]:
+                console.print("Sync cancelled.")
+                return
         syncer.sync_template(directories)
-        print(f"Synchronized {len(directories)} repositories with the template directory.")
+        console.print(f"Synchronized {len(directories)} repositories with the template directory.")
 
+    @log_duration
     def merge_request(
         self, source_branch: str, target_branch: str, title: str, reviewer: str, project_id: int, repo_name: str
     ) -> None:
         """
         Create a pull request on GitHub and assign a reviewer.
 
         Args:
@@ -607,14 +686,15 @@
             reviewer: GitHub username of the reviewer.
             project_id: The ID of the GitLab project (unused here).
             repo_name: The name of the repository, e.g., "user/repo".
 
         Returns:
             None
         """
+        console = console_with_theme()
         repo = self.client().get_repo(repo_name)
         if not self.user:
             self.user = self.client().get_user()
 
         # Create pull request
         pull_request = repo.create_pull(
             title=title,
@@ -624,8 +704,8 @@
             maintainer_can_modify=True,  # Allows maintainer to modify the PR if needed
         )
 
         # Assign user and request a review
         pull_request.assignees.append(self.user)  # type: ignore
         pull_request.create_review_request(reviewers=[reviewer])
 
-        print(f"Pull request created: {pull_request.html_url}")
+        console.print(f"Pull request created: {pull_request.html_url}")
```

### Comparing `git_mirror-0.3.6/git_mirror/manage_gitlab.py` & `git_mirror-0.3.7/git_mirror/manage_gitlab.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 from termcolor import colored
 
 import git_mirror.manage_git as mg
 from git_mirror.cross_repo_sync import TemplateSync
 from git_mirror.custom_types import SourceHost, UpdateBranchArgs
 from git_mirror.dummies import Dummy
 from git_mirror.manage_pypi import PyPiManager
+from git_mirror.performance import log_duration
 from git_mirror.safe_env import load_env
+from git_mirror.ui import console_with_theme
 
 load_env()
 
 
 # Configure logging
 LOGGER = logging.getLogger(__name__)
 
@@ -44,39 +46,42 @@
         user_login: str,
         include_private: bool = True,
         include_forks: bool = False,
         host_domain: str = "https://gitlab.com",
         group_id: Optional[int] = None,
         logging_level: int = 1,
         dry_run: bool = False,
+        prompt_for_changes: bool = True,
     ):
         """
         Initializes the RepoManager with a GitLab token and a base directory for cloning repositories.
 
         Args:
             token (str): GitLab personal access token.
             base_dir (Path): Base directory path where repositories will be cloned.
             user_login (str): The GitLab username.
             include_private (bool): Whether to include private repositories.
             include_forks (bool): Whether to include forked repositories.
             host_domain (str): The GitLab host domain.
             group_id (int): The ID of the group to clone repositories from.
             logging_level (int): The logging level.
             dry_run (bool): Whether the operation should be a dry run.
+            prompt_for_changes (bool): Whether to prompt for confirmation before making changes.
         """
         self.token = token
         self.host_domain = host_domain
         self.base_dir = base_dir
         self.user_login = user_login
         self.include_private = include_private
         self.include_forks = include_forks
         # self.user: Optional[RESTObject] = None
         self.group_id = group_id
         self.verbose_logging = logging_level
         self.dry_run = dry_run
+        self.prompt_for_changes = prompt_for_changes
 
     def client(self) -> gitlab.Gitlab:
         the_client = gitlab.Gitlab(self.host_domain, private_token=self.token)
         if self.verbose_logging >= 2:
             the_client.enable_debug()
         return the_client
 
@@ -96,16 +101,15 @@
     def _get_user_repos(self) -> list[Project]:
         """
         Fetches the user's repositories from GitLab, optionally including private repositories and forks.
 
         Returns:
             List[gitlab.v4.objects.Project]: A list of Project objects.
         """
-        # user = self.gitlab.users.list(username=self.user_login, get_all=True)[0]  # type: ignore
-
+        console = console_with_theme()
         try:
             kwargs: dict[str, Union[bool, str]] = {"owned": True}
             if not self.include_private:
                 kwargs["visibility"] = "public"
             projects = self.client().projects.list(**kwargs, get_all=True)
             projects = [self.client().projects.get(id=project.id) for project in projects]
 
@@ -117,275 +121,338 @@
                 else:
                     forked = False
                 if (self.include_forks or not forked) and project.namespace["path"] == self.user_login:
                     filtered_projects.append(project)
 
             return filtered_projects  # type: ignore
         except gitlab.exceptions.GitlabError as e:
-            print(f"Failed to fetch repositories: {e}")
+            console.print(f"Failed to fetch repositories: {e}", style="danger")
             return []
 
+    @log_duration
     def clone_all(self, single_threaded: bool = False) -> None:
         """
         Clones all repositories for a user.
         """
+        console = console_with_theme()
         repos = self._get_user_repos()
-        print(f"Cloning {len(repos)} repositories.")
+        if self.prompt_for_changes:
+            answer = inquirer.prompt(
+                [
+                    inquirer.Confirm(
+                        "clone-all", message=f"Are you sure you want to clone {len(repos)} repositories?", default=False
+                    )
+                ]
+            )
+            if not answer["clone-all"]:
+                console.print("Cloning cancelled.")
+                return
+
+        console.print(f"Cloning {len(repos)} repositories.")
         if single_threaded or len(repos) < 4:
             for repo in self._thread_safe_repos(repos):
                 self._clone_repo((repo, Dummy()))
         else:
             with multiprocessing.Pool(multiprocessing.cpu_count()) as pool:
                 manager = multiprocessing.Manager()
                 lock = manager.Lock()
                 work_load = [(repo, lock) for repo in self._thread_safe_repos(repos)]
                 results = pool.map(self._clone_repo, work_load)
                 for output in results:
                     if output:
-                        print(output, end="")
+                        console.print(output, end="")
 
+    @log_duration
     def clone_group(self, group_id: int):
         """
         Clones all repositories for a user or all repositories within a group.
 
         Args:
             group_id (int): The ID of the group to clone repositories from.
         """
         if group_id == 0:
             raise ValueError("Group ID cannot be 0.")
-        print(f"Cloning all repositories for group with ID {group_id}")
         self._clone_group_repos(group_id)
 
     def _clone_group_repos(self, group_id: int) -> None:
         """
         Clones all repositories within a specified group, including subgroups.
 
         Args:
             group_id (int): The ID of the group.
         """
         if group_id == 0:
             raise ValueError("Group ID cannot be 0.")
-
+        console = console_with_theme()
         groups_to_process = [group_id]
 
         while groups_to_process:
             current_group_id = groups_to_process.pop(0)
             group = self._get_group_by_id(current_group_id)
             # subgroups = self._get_subgroups(group)
             if not group:
-                print(f"Group with ID {current_group_id} not found. Skipping.")
+                console.print(f"Group with ID {current_group_id} not found. Skipping.")
             repos = self._get_repos(group)
 
+            if self.prompt_for_changes:
+                answer = inquirer.prompt(
+                    [
+                        inquirer.Confirm(
+                            "clone-all",
+                            message=f"Are you sure you want to clone {len(repos)} repositories?",
+                            default=False,
+                        )
+                    ]
+                )
+                if not answer["clone-all"]:
+                    console.print("Cloning cancelled.")
+                    return
+            console.print(f"Cloning all {len(repos)} repositories for group with ID {group_id}")
+
             for repo in self._thread_safe_repos(repos):
-                print(".", end="")
+                console.print(".", end="")
                 self._clone_repo((repo, Dummy()))  # , extra_path=group.full_path)
 
             # for subgroup in subgroups:
             #     groups_to_process.append(subgroup.id)
 
     def _clone_repo(self, repo_args: tuple[dict[str, Any], ContextManager[Any]]) -> None:
         """
         Clones the given project into the target directory, respecting group/subgroup structure.
 
         Args:
             repo_args (tuple[dict[str, Any], ContextManager[Any]]): A tuple containing the project and a lock.
         """
+        console = console_with_theme()
         extra_path = ""
         project, lock = repo_args
         try:
             repo_path = self.base_dir / extra_path / project["path"]
             if not repo_path.exists():
                 if self.dry_run:
                     with lock:
-                        print(f"Would clone {project['web_url']} into {repo_path}")
+                        console.print(f"Would clone {project['web_url']} into {repo_path}")
                 else:
                     with lock:
-                        print(f"Cloning {project['web_url']} into {repo_path}")
+                        console.print(f"Cloning {project['web_url']} into {repo_path}")
                     repo_path.parent.mkdir(parents=True, exist_ok=True)
                     g.Repo.clone_from(project["http_url_to_repo"], repo_path)
             else:
                 with lock:
-                    print(f"Project {project['path']} already exists locally. Skipping clone.")
+                    console.print(f"Project {project['path']} already exists locally. Skipping clone.")
         except g.GitCommandError as e:
             with lock:
-                print(f"Failed to clone {project['path']}: {e}")
+                console.print(f"Failed to clone {project['path']}: {e}", style="danger")
 
     def _get_group_by_id(self, group_id: int):
         """
         Fetches a GitLab group by its ID using the python-gitlab library.
 
         Args:
             group_id (int): The ID of the group to fetch.
 
         Returns:
             gitlab.v4.objects.Group: The GitLab Group object.
         """
+        console = console_with_theme()
         try:
             # Fetch the group by ID
             group = self.client().groups.get(group_id)
             return group
         except gitlab.exceptions.GitlabGetError as e:
-            print(f"Failed to get group with ID {group_id}: {e}")
+            console.print(f"Failed to get group with ID {group_id}: {e}", style="danger")
             return None
 
     def _get_subgroups(self, group):
         """
         Fetches all subgroups for a given GitLab group.
 
         Args:
             group (gitlab.v4.objects.Group): The GitLab Group object.
 
         Returns:
             List[gitlab.v4.objects.Group]: A list of GitLab Subgroup objects.
         """
+        console = console_with_theme()
         try:
             subgroups = group.projects.list(all=True, include_subgroups=True)
             return subgroups
         except gitlab.exceptions.GitlabListError as e:
-            print(f"Failed to list subgroups for group {group.id}: {e}")
+            console.print(f"Failed to list subgroups for group {group.id}: {e}", style="danger")
             return []
 
     def _get_repos(self, group: gitlab.v4.objects.Group) -> list[gitlab.v4.objects.Project]:
         """
         Fetches all repositories (projects) for a given GitLab group, including those in its subgroups.
 
         Args:
             group (gitlab.v4.objects.Group): The GitLab Group object.
 
         Returns:
             List[gitlab.v4.objects.Project]: A list of GitLab Project objects.
         """
+        console = console_with_theme()
         try:
             # Retrieve all projects for the group, including those in subgroups
             projects = group.projects.list(include_subgroups=True, all=True)
             return projects  # type: ignore
         except gitlab.exceptions.GitlabListError as e:
-            print(f"Failed to list projects for group {group.id}: {e}")
+            console.print(f"Failed to list projects for group {group.id}: {e}", style="danger")
             return []
 
-    def pull_all(self, single_threaded: bool = False):
+    @log_duration
+    def pull_all(self, single_threaded: bool = False) -> None:
+        console = console_with_theme()
         directories = mg.find_git_repos(self.base_dir)
-        print(f"Pulling {len(directories)} repositories.")
+        console.print(f"Pulling {len(directories)} repositories.")
         if single_threaded or len(directories) < 4:
             for repo_dir in directories:
                 self.pull_repo((repo_dir, Dummy()))
         else:
             with multiprocessing.Pool(multiprocessing.cpu_count()) as pool:
                 manager = multiprocessing.Manager()
                 lock = manager.Lock()
-                results = pool.map(self.pull_repo, (print(repo_dir) or (repo_dir, lock) for repo_dir in directories))
+                results = pool.map(self.pull_repo, ((repo_dir, lock) for repo_dir in directories))
                 for output in results:
                     if output:
-                        print(output, end="")
+                        console.print(output, end="")
 
+    @log_duration
     def pull_repo(self, args: tuple[Path, ContextManager[Any]]) -> None:
         """
         Performs a git pull operation on the repository at the given path.
 
         Args:
             args (tuple[Path, ContextManager[Any]]): A tuple containing the path to the repository and a lock.
         """
+        console = console_with_theme()
         repo_path, lock = args
         try:
             repo = g.Repo(repo_path)
+
+            # Get the current branch
+            current_branch = repo.active_branch.name
+
+            # Fetch the latest info from the remote
+            origin = repo.remotes.origin
+            origin.fetch()
+            commits_behind = repo.iter_commits(f"{current_branch}..origin/{current_branch}")
+
+            count = sum(1 for _ in commits_behind)
+            if count <= 0:
+                with lock:
+                    console.print(f"{repo_path} is up to date.")
+                return
+
             origin = repo.remotes.origin
             if not self.dry_run:
                 with lock:
-                    print(f"Pulling latest changes in {repo_path}")
+                    console.print(f"Pulling latest changes in {repo_path}")
                 origin.pull()
+                # confusing mess.
+                # for info in infos:
+                #     with lock:
+                #         if info.note:
+                #             console.print(info.note)
+                #         console.print(info)
             else:
                 with lock:
-                    print(f"Would have pulled latest changes in {repo_path}")
+                    console.print(f"Would have pulled latest changes in {repo_path}")
         except Exception as e:
             with lock:
-                print(f"Failed to pull repo at {repo_path}: {e}")
+                console.print(f"Failed to pull repo at {repo_path}: {e}", style="danger")
 
+    @log_duration
     def not_repo(self) -> tuple[int, int, int, int]:
         """
         Lists directories in the base directory that are not valid Git repositories,
         or are not owned by the user, or are forks of another repository.
 
         Returns:
             tuple: Counts of no_remote, not_found, is_fork, not_repo scenarios.
         """
-        kwargs: dict[str, Union[str, bool]] = {"owned": True, "get_all": True}
-        if not self.include_private:
-            kwargs["visibility"] = "public"
+        console = console_with_theme()
+        # Get all the user's repos broadly, without filtering by visibility or forking
         user_projects = {
-            project.path: self.client().projects.get(id=project.id) for project in self.client().projects.list(**kwargs)
+            project.path: self.client().projects.get(id=project.id) for project in self.client().projects.list()
         }
 
         no_remote = 0
         not_found = 0
         is_fork = 0
         not_repo = 0
-        for repo_dir in mg.find_git_repos(self.base_dir):
+        repos = mg.find_git_repos(self.base_dir)
+        console.print(f"Checking {len(repos)} repositories for stray, non-repo subfolders in {self.base_dir}.")
+        for repo_dir in repos:
             if repo_dir.is_dir():
                 try:
                     repo = g.Repo(repo_dir)
                     remotes = repo.remotes
                     if not remotes:
                         no_remote += 1
-                        print(f"{repo_dir} has no remote repositories defined.")
+                        console.print(f"{repo_dir} has no remote repositories defined.")
                         continue
 
                     remote_url = remotes[0].config_reader.get("url")
                     repo_name = mg.extract_repo_name(remote_url)
 
                     if repo_name not in user_projects:
                         not_found += 1
-                        print(f"{repo_dir} is not found in your GitLab account.")
+                        console.print(f"{repo_dir} is not found in your GitLab account.")
                         continue
 
                     gitlab_project = user_projects[repo_name]
                     if hasattr(gitlab_project, "forked_from_project") and gitlab_project.forked_from_project:
                         forked = True
                     else:
                         forked = False
                     if not forked:
                         is_fork += 1
-                        print(f"{repo_dir} is a fork of another repository.")
+                        console.print(f"{repo_dir} is a fork of another repository.")
                         continue
 
                 except g.InvalidGitRepositoryError:
                     not_repo += 1
-                    print(f"{repo_dir} is not a valid Git repository.")
+                    console.print(f"{repo_dir} is not a valid Git repository.", style="danger")
         return no_remote, not_found, is_fork, not_repo
 
+    @log_duration
     def list_repo_builds(self) -> list[tuple[str, str]]:
         """
         Lists the most recent GitLab CI/CD pipeline runs for each project of the authenticated user,
         with the status color-coded: green for success, red for failure, and yellow for canceled.
         """
+        console = console_with_theme()
         messages = []
         for project in self._get_user_repos():
-            print(f"Project: {project.name}")
+            console.print(f"Project: {project.name}")
             pipelines = cast(
                 RESTObjectList, project.pipelines.list(order_by="updated_at", sort="desc", per_page=1, iterator=True)
             )  # Get the most recent pipeline
             messages.extend(self._loop_pipelines(pipelines))
         return messages
 
     def _loop_pipelines(self, pipelines: RESTObjectList, count: int = 1) -> list[tuple[str, str]]:
+        console = console_with_theme()
         messages = []
         seen = 0
         for pipeline in pipelines:
             seen += 1
             if seen > count:
                 break
             status_message = f"Date: {pipeline.updated_at} - Pipeline #{pipeline.id} - Status: {pipeline.status} - URL: {pipeline.web_url}"
             status = pipeline.status.lower()
             messages.append((status, status_message))
 
             if status in ["passed", "success"]:
-                print(colored(status_message, "green"))
+                console.print(colored(status_message, "green"))
             elif status in ["failed"]:
-                print(colored(status_message, "red"))
+                console.print(colored(status_message, "red"))
             elif status in ["canceled", "cancelled"]:  # Checking both spellings to be safe
-                print(colored(status_message, "yellow"))
+                console.print(colored(status_message, "yellow"))
             else:
                 raise ValueError(f"Unknown status: {status}")
         return messages
 
     def _get_latest_commit_date(self, repo: g.Repo) -> datetime:
         """
         Gets the date of the latest commit in the repository.
@@ -395,19 +462,21 @@
 
         Returns:
             datetime: The datetime of the latest commit.
         """
         last_commit = next(repo.iter_commits())
         return datetime.fromtimestamp(last_commit.committed_date)
 
+    @log_duration
     def check_pypi_publish_status(self, pypi_owner_name: Optional[str] = None) -> list[dict[str, Any]]:
         """
         Checks if the repositories as Python packages are published on PyPI and compares the last change dates.
         """
-        print("Checking if your gitlab repos have been published to pypi.")
+        console = console_with_theme()
+        console.print("Checking if your gitlab repos have been published to pypi.")
         results = []
 
         async def get_infos_async(package_names):
             pypi_manager = PyPiManager()
             return await pypi_manager.get_infos(package_names)
 
         package_names = [path.name for path in mg.find_git_repos(self.base_dir)]
@@ -441,37 +510,40 @@
                                     "PyPI last change date": pypi_release_date.date(),
                                     "Days difference": days_difference,
                                 }
                             )
                     # else:
                     #     LOGGER.debug(f"{package_name} is not a pypi package name.")
                 except g.InvalidGitRepositoryError:
-                    print(f"{repo_dir} is not a valid Git repository.")
+                    console.print(f"{repo_dir} is not a valid Git repository.", style="danger")
                 except Exception as e:
-                    print(f"Error checking {repo_dir}: {e}")
+                    console.print(f"Error checking {repo_dir}: {e}", style="danger")
         if found == 0:
-            print(
+            console.print(
                 "None of your repositories are published on PyPI under the project name and "
                 f"owner name of {pypi_owner_name}."
             )
         return results
 
+    @log_duration
     def list_repo_names(self) -> list[str]:
         """
         Returns a list of repository names.
 
         Returns:
             List[str]: A list of repository names.
         """
         return [project.name for project in self._get_user_repos()]
 
+    @log_duration
     def list_repos(self) -> Optional[Table]:
         """
         Fetches and prints beautifully formatted information about the user's Gitlab repositories.
         """
+        console = console_with_theme()
         try:
             table = Table(title="Gitlab Repositories")
 
             table.add_column("Name", style="cyan", no_wrap=True)
             table.add_column("Description", style="magenta")
             table.add_column("URL", style="green")
             table.add_column("Private", style="red")
@@ -495,25 +567,26 @@
                         project.name,
                         project.description or "No description",
                         project.web_url,
                         project.visibility,
                         "Yes" if forked else "No",
                     )
 
-            console = Console()
             console.print(table)
             return table
         except gitlab.exceptions.GitlabError as e:
-            print(f"An error occurred: {e}")
+            console.print(f"An error occurred: {e}", style="danger")
         return None
 
+    @log_duration
     def print_user_summary(self) -> None:
         """
         Fetches and prints a summary of the user's Gitlab account.
         """
+        console = console_with_theme()
         try:
             user = self.load_user()
 
             summary = Text.assemble(
                 ("Username: ", "bold cyan"),
                 f"{user.username}\n",
                 ("Name: ", "bold cyan"),
@@ -524,57 +597,60 @@
                 f"{user.public_email or 'N/A'}\n",
                 # I don't think Gitlab has following, followers.
                 ("Location: ", "bold cyan"),
                 f"{user.location or 'Not specified'}\n",
                 ("Company: ", "bold cyan"),
                 f"{user.organization or 'Not specified'}",
             )
-            console = Console()
+            Console()
             console.print(Panel(summary, title="GitLab User Summary", subtitle=user.username))
         except Exception as e:
-            print("Failed to fetch GitLab user info: %s", str(e))
+            console.print(f"Failed to fetch GitLab user info: {e}", style="danger")
 
     def load_user(self) -> RESTObject:
         list_info = self.client().users.list(username=self.user_login, get_all=True)[0]  # type: ignore
         user = self.client().users.get(list_info.id)
         # to make mypy happy
         return user
 
+    @log_duration
     def update_all_branches(self, single_threaded: bool = False, prefer_rebase: bool = False):
         """
         Updates each local branch with the latest changes from the main/master branch on Gitlab.
 
         Args:
             single_threaded (bool): Whether to run the operation in a single thread.
             prefer_rebase (bool): Whether to prefer rebasing instead of merging.
         """
+        console = console_with_theme()
         directories = mg.find_git_repos(self.base_dir)
-        print(f"Merging/rebasing {len(directories)} main to local repositories.")
+        console.print(f"Merging/rebasing {len(directories)} main to local repositories.")
         if single_threaded or len(directories) < 4:
             for repo_dir in directories:
                 self._update_local_branches(UpdateBranchArgs(repo_dir, repo_dir.name, prefer_rebase, Dummy()))
         else:
             with multiprocessing.Pool(multiprocessing.cpu_count()) as pool:
                 manager = multiprocessing.Manager()
                 lock = manager.Lock()
                 results = pool.map(
                     self._update_local_branches,
                     (UpdateBranchArgs(repo_dir, repo_dir.name, prefer_rebase, lock) for repo_dir in directories),
                 )
                 for output in results:
                     if output:
-                        print(output, end="")
+                        console.print(output, end="")
 
     def _update_local_branches(self, args: UpdateBranchArgs):
         """
         Updates each local branch with the latest changes from the main/master branch on Gitlab.
 
         Args:
             args: UpdateBranchArgs
         """
+        console = console_with_theme()
         repo_path, project_name, prefer_rebase = args.repo_path, args.github_repo_full_name, args.prefer_rebase
         repo = g.Repo(str(repo_path))
 
         # Search for the project using the namespace and project name
         projects = self.client().projects.list(search=project_name, owned=True)[0]  # type: ignore
         # for project in projects:
         #     if project.path_with_namespace == f"{self.user_login}/{project_name}":
@@ -603,118 +679,150 @@
                     # Perform rebase
                     repo.git.rebase(f"origin/{default_branch}")
                 else:
                     # Perform merge
                     repo.git.merge(f"origin/{default_branch}")
                 if not self.dry_run:
                     with args.lock:
-                        print(f"Updated branch '{branch}' with latest changes from '{default_branch}'.")
+                        console.print(f"Updated branch '{branch}' with latest changes from '{default_branch}'.")
                 else:
                     with args.lock:
-                        print(f"Would have updated branch '{branch}' with latest changes from '{default_branch}'.")
+                        console.print(
+                            f"Would have updated branch '{branch}' with latest changes from '{default_branch}'."
+                        )
             except g.exc.GitCommandError as e:
                 with args.lock:
-                    print(f"Failed to update branch '{branch}': {e}")
+                    console.print(f"Failed to update branch '{branch}': {e}", style="danger")
 
+    @log_duration
     def prune_all(self):
-        for repo_dir in mg.find_git_repos(self.base_dir):
+        console = console_with_theme()
+        repos = mg.find_git_repos(self.base_dir)
+        console.print(f"Checking {len(repos)} repositories for uncommitted changes and unpushed commits.")
+        if self.prompt_for_changes:
+            answer = inquirer.confirm("Do you want to prune all repositories?", default=False).execute()
+            if not answer:
+                console.print("Aborted.")
+                return
+
+        for repo_dir in repos:
             if repo_dir.is_dir():
                 self._delete_local_branches_if_not_on_host(repo_dir, f"{self.user_login}/{repo_dir.name}")
 
     def _delete_local_branches_if_not_on_host(self, repo_path: Path, project_name: str):
         """
         Loops through all local branches, checks if they exist on Gitlab, and prompts the user for deletion if they don't.
 
         Args:
             repo_path (Path): The file system path to the local git repository.
             project_name (str): The name of the project on Gitlab.
         """
+        console = console_with_theme()
         try:
             repo = g.Repo(str(repo_path))
         except g.InvalidGitRepositoryError:
-            print(f"{repo_path} is not a valid Git repository.")
+            console.print(f"{repo_path} is not a valid Git repository.", style="danger")
             return
         project = self.client().projects.list(search=project_name, owned=True)[0]  # type: ignore
 
         # Get a list of all branch names on Gitlab
         remote_branches = [branch.name for branch in project.get_branches()]
 
         # Get a list of all local branch names
         local_branches = [branch.name for branch in repo.heads]  # alias to branches
 
         # Determine branches that are local but not on Gitlab
         branches_to_consider = [branch for branch in local_branches if branch not in remote_branches]
 
         if not branches_to_consider:
-            print("No local branches exist that are missing on Gitlab.")
+            console.print("No local branches exist that are missing on Gitlab.")
             return
 
         # Prompt user for each branch that doesn't exist on Gitlab
         for branch in branches_to_consider:
-            question = [
-                inquirer.Confirm(
-                    "delete", message=f"The branch '{branch}' does not exist on Gitlab. Delete locally?", default=False
-                )
-            ]
-            answer = inquirer.prompt(question)
+            if self.prompt_for_changes:
+                question = [
+                    inquirer.Confirm(
+                        "delete",
+                        message=f"The branch '{branch}' does not exist on Gitlab. Delete locally?",
+                        default=False,
+                    )
+                ]
+                answer = inquirer.prompt(question)
 
-            if answer["delete"]:
-                try:
-                    if not self.dry_run:
-                        # Safely delete the branch
-                        repo.git.branch("-d", branch)
-                        print(f"Deleted branch '{branch}' locally.")
-                    else:
-                        print(f"Would have deleted branch '{branch}' locally.")
-                except g.exc.GitCommandError as e:
-                    print(f"Could not delete branch '{branch}'. It may not be fully merged. Error: {e}")
-            else:
-                print(f"Skipped deletion of branch '{branch}'.")
+                if not answer["delete"]:
+                    console.print(f"Skipped deletion of branch '{branch}'.")
+                    continue
+            try:
+                if not self.dry_run:
+                    # Safely delete the branch
+                    repo.git.branch("-d", branch)
+                    console.print(f"Deleted branch '{branch}' locally.")
+                else:
+                    console.print(f"Would have deleted branch '{branch}' locally.")
+            except g.exc.GitCommandError as e:
+                console.print(
+                    f"Could not delete branch '{branch}'. It may not be fully merged. Error: {e}", style="danger"
+                )
 
+    @log_duration
     def version_info(self) -> dict[str, Any]:
         """
         Return API version information.
         """
         version, revision = self.client().version()
         return {"version": version, "revision": revision}
 
+    @log_duration
     def cross_repo_sync_report(self, template_dir: Path) -> None:
         """
         Reports differences between the template directory and the target directories.
         """
+        console = console_with_theme()
         if not template_dir or not template_dir.exists():
-            print(f"Template directory {template_dir} does not exist.")
+            console.print(f"Template directory {template_dir} does not exist.")
             return
         # right now just the easy case of all repos need to match 1 template_dir
-        print("Reporting differences between the template directory and the target directories.")
+        console.print("Reporting differences between the template directory and the target directories.")
         syncer = TemplateSync(template_dir)
         directories = mg.find_git_repos(self.base_dir)
-        print(f"Found {len(directories)} repositories.")
+        console.print(f"Found {len(directories)} repositories.")
         syncer.report_content_differences(directories)
 
+    @log_duration
     def cross_repo_init(self, template_dir: Path):
+        console = console_with_theme()
         if not template_dir or not template_dir.exists():
-            print(f"Template directory {template_dir} does not exist.")
+            console.print(f"Template directory {template_dir} does not exist.")
             return
         syncer = TemplateSync(template_dir, use_default=True)
         directories = mg.find_git_repos(self.base_dir)
-        print(f"Found {len(directories)} repositories.")
+        console.print(f"Found {len(directories)} repositories.")
         syncer.write_template_map(directories)
-        print(f"Initialized template map for {len(directories)} repositories.")
+        console.print(f"Initialized template map for {len(directories)} repositories.")
 
+    @log_duration
     def cross_repo_sync(self, template_dir: Path):
+        console = console_with_theme()
         if not template_dir or not template_dir.exists():
-            print(f"Template directory {template_dir} does not exist.")
+            console.print(f"Template directory {template_dir} does not exist.")
             return
         syncer = TemplateSync(template_dir, use_default=True)
         directories = mg.find_git_repos(self.base_dir)
-        print(f"Found {len(directories)} repositories.")
+        console.print(f"Found {len(directories)} repositories.")
+        answer = inquirer.confirm(
+            "Do you want to synchronize all repositories with the template directory?", default=False
+        ).execute()
+        if not answer:
+            console.print("Aborted.")
+            return
         syncer.sync_template(directories)
-        print(f"Synchronized {len(directories)} repositories with the template directory.")
+        console.print(f"Synchronized {len(directories)} repositories with the template directory.")
 
+    @log_duration
     def merge_request(
         self, source_branch: str, target_branch: str, title: str, reviewer: str, project_id: int, repo_name: str
     ):
         user = self.load_user()
         project = self.client().projects.get(project_id)
         reviewer_object = self.client().users.list(username=reviewer, get_all=True)[0]  # type: ignore
         mr = project.mergerequests.create(
```

### Comparing `git_mirror-0.3.6/git_mirror/manage_poetry.py` & `git_mirror-0.3.7/git_mirror/manage_poetry.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 import os
 import subprocess  # nosec
 
 import git
 
 from git_mirror.custom_types import SourceHost
+from git_mirror.performance import log_duration
 
 logger = logging.getLogger(__name__)
 
 
 def clean_gone_branches(repo: git.Repo) -> None:
     """Clean branches that are gone from remote.
 
@@ -21,17 +22,26 @@
         if "[gone]" in ref
     ]
     for branch in gone_branches:
         repo.git.branch("-D", branch)
 
 
 class PoetryManager:
-    def __init__(self, host: SourceHost):
+    def __init__(self, host: SourceHost, dry_run: bool = False, prompt_for_changes: bool = True):
+        """
+        Args:
+            host: The source host.
+            dry_run: Whether to perform a dry run.
+            prompt_for_changes: Whether to prompt for changes.
+        """
         self.host = host
+        self.dry_run = dry_run
+        self.prompt_for_changes = prompt_for_changes
 
+    @log_duration
     def update_dependencies(
         self, main_branch: str, dependency_update_branch: str, project_id: int, repo_name: str, user: str, reviewer: str
     ) -> None:
         """Update project dependencies and create a merge request if changes are made.
 
         Args:
             main_branch: The main branch name.
```

### Comparing `git_mirror-0.3.6/git_mirror/manage_pypi.py` & `git_mirror-0.3.7/git_mirror/manage_pypi.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,80 +1,76 @@
 """
 Pure pypi actions.
 """
 
 import asyncio
 import logging
-import os
 from datetime import datetime
-from typing import Any, Optional, Union
+from typing import Any, Optional
 
-import colorama
 import httpx
-from prettytable import PrettyTable
-from prettytable.colortable import ColorTable, Themes
+from rich.table import Table
 
 from git_mirror.safe_env import load_env
 
 load_env()
 
 # Configure logging
 LOGGER = logging.getLogger(__name__)
 
 
-def pretty_print_pypi_results(results: list[dict[str, Any]]) -> Union[PrettyTable, ColorTable]:
+def pretty_print_pypi_results(results: list[dict[str, Any]]) -> Table:
     """
-    Pretty print the results of the audit.
+    Pretty prints the results of the PyPI audit using the rich library.
 
-    Returns:
-        Union[PrettyTable, ColorTable]: A PrettyTable or ColorTable object.
+    Args:
+        results (List[dict[str, Any]]): A list of dictionaries containing the audit results.
     """
-    if os.environ.get("NO_COLOR") or os.environ.get("CI"):
-        table = PrettyTable()
-    else:
-        table = ColorTable(theme=Themes.OCEAN)
-    table.field_names = [
-        "Package",
-        "On PyPI",
-        "Pypi Owner",
-        "Repo last change date",
-        "PyPI last change date",
-        "Days difference",
-    ]
+    table = Table()
 
-    all_rows: list[list[str]] = []
+    table.add_column("Package")
+    table.add_column("On PyPI")
+    table.add_column("Pypi Owner")
+    table.add_column("Repo last change date")
+    table.add_column("PyPI last change date")
+    table.add_column("Days difference")
 
     for result in results:
+        days_difference = int(result.get("Days difference", "0"))
+        style = "red" if days_difference * -1 > 60 else ""
+
         row_data = [
             result["Package"],
             result["On PyPI"],
             result["Pypi Owner"],
-            result["Repo last change date"],
-            result["PyPI last change date"],
-            result["Days difference"],
+            str(result["Repo last change date"]),
+            str(result["PyPI last change date"]),
+            str(result["Days difference"]),
         ]
-        row_transformed = []
-        # Turn values red if more than 2 months stale.
-        for datum in row_data:
-            try:
-                days_difference = int(result["Days difference"])
-            except ValueError:
-                days_difference = 0
-            if (days_difference * -1) > 60:
-                transformed = f"{colorama.Fore.RED}{datum}{colorama.Style.RESET_ALL}"
-            else:
-                transformed = str(datum)
-            row_transformed.append(transformed)
-        all_rows.append(row_transformed)
-
-    table.add_rows(sorted(all_rows, key=lambda x: x[0]))
 
+        # Apply style to the entire row if needed
+        table.add_row(*row_data, style=style)
     return table
 
 
+if __name__ == "__main__":
+    # Example usage
+    results = [
+        {
+            "Package": "ExamplePackage",
+            "On PyPI": "Yes",
+            "Pypi Owner": "OwnerName",
+            "Repo last change date": "2023-01-01",
+            "PyPI last change date": "2023-02-01",
+            "Days difference": "-30",
+        }
+    ]
+    pretty_print_pypi_results(results)
+
+
 class PyPiManager:
 
     def __init__(self, pypi_owner_name: Optional[str] = None):
         self.pypi_owner_name = pypi_owner_name
         self.client = httpx.AsyncClient()
 
     async def get_info(self, package_name: str) -> tuple[dict[str, Any], int]:
@@ -86,14 +82,15 @@
 
         Returns:
             Tuple[Dict[str, Any], int]: A tuple containing the package information and the HTTP status code.
         """
         pypi_url = f"https://pypi.org/pypi/{package_name}/json"
         response = await self.client.get(pypi_url)
         data = response.json()
+        print(".", end="", flush=True)
         return data, response.status_code
 
     async def get_infos(self, package_names: list[str]) -> dict[str, tuple[dict[str, Any], int]]:
         """
         Asynchronously get information for multiple packages from PyPI.
 
         Args:
```

### Comparing `git_mirror-0.3.6/git_mirror/menu.py` & `git_mirror-0.3.7/git_mirror/menu.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     commands: list[tuple[str, str]] = [
         ("Initialize Configuration", "init"),
         ("Show Account Info", "show-account"),
         ("List repositories", "list-repos"),
         ("Clone all repositories", "clone-all"),
         ("Run pull for all repositories", "pull-all"),
         ("Report uncommitted/unpushed changes", "local-changes"),
-        ("Report non-repo files in target folder", "not-repo"),
+        ("Report non-repo folders in target folder", "not-repo"),
         ("Report all build statuses", "build-status"),
         ("Sync repo list in config with source control host", "sync-config"),
         ("Report current configuration", "list-config"),
         ("Report unpublished pypi packages", "pypi-status"),
         ("Update all branches from main", "update-from-main"),
         ("Prune all branches", "prune-all"),
         ("Cross-repo report", "cross-repo-report"),
```

### Comparing `git_mirror-0.3.6/git_mirror/pat_init.py` & `git_mirror-0.3.7/git_mirror/pat_init_gitlab.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,85 +3,85 @@
 import os
 from pathlib import Path
 
 import httpx
 from dotenv import find_dotenv, load_dotenv, set_key
 
 from git_mirror.safe_env import env_info
+from git_mirror.ui import console_with_theme
 
 LOGGER = logging.getLogger(__name__)
 
+console = console_with_theme()
+
 
 def check_pat_validity(token: str) -> bool:
     """
-    Check if the GitHub Personal Access Token (PAT) is still valid.
+    Check if the GitLab Personal Access Token (PAT) is still valid.
 
     Args:
-        token (str): The GitHub Personal Access Token.
+        token (str): The GitLab Personal Access Token.
 
     Returns:
         bool: True if the token is valid, False otherwise.
     """
-    headers = {"Authorization": f"token {token}"}
+    headers = {"Authorization": f"Bearer {token}"}
     try:
-        response = httpx.get("https://api.github.com/user", headers=headers)
+        response = httpx.get("https://gitlab.com/api/v4/user", headers=headers)
         return response.status_code == 200
     except httpx.RequestError as e:
-        print(f"An error occurred while checking PAT validity: {e}")
+        console.print(f"An error occurred while checking PAT validity: {e}", style="danger")
         return False
 
 
-def setup_github_pat() -> None:
+def setup_gitlab_pat() -> None:
     """
-    Setup the GitHub Personal Access Token (PAT) either globally or locally.
+    Setup the GitLab Personal Access Token (PAT) either globally or locally.
     Checks if it exists and is valid, then asks the user for their preference
     on storing the PAT.
     """
-    print("Checking environment...")
+    console.print("Checking environment...")
     env_info()
-    print()
+    console.print()
     # Attempt to load existing .env and check for existing PAT
     dotenv_path = Path(find_dotenv())
     load_dotenv(dotenv_path)
-    existing_pat = os.getenv("GITHUB_ACCESS_TOKEN")
+    existing_pat = os.getenv("GITLAB_ACCESS_TOKEN")
 
     # Check validity of an existing PAT
     if existing_pat and check_pat_validity(existing_pat):
-        print("Existing PAT is valid.")
+        console.print("Existing PAT is valid.")
         return
     else:
-        print("No valid PAT found.")
-
-    print(
-        "https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens"
-    )
+        console.print("No valid PAT found.")
 
-    print("Next we will create a local or global .env file to store the PAT.")
+    console.print("https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html")
+    console.print("Next we will create a local or global .env file to store the PAT.")
     # Ask for new PAT
-    new_pat = getpass.getpass("Enter your new GitHub PAT: ")
+    new_pat = getpass.getpass("Enter your new GitLab PAT: ")
 
     # Validate the new PAT
     if not check_pat_validity(new_pat):
-        print("The provided PAT is invalid.")
+        console.print("The provided PAT is invalid.")
         return
 
     # Ask user for global or local setup
     choice = (
-        input("Do you want to save the PAT globally or locally? [G/L]. If you don't know select globally. ")
+        input("Do you want to save the PAT globally or locally? [G/L]. If you don't know, select globally. ")
         .strip()
         .lower()
     )
 
     if choice == "g":
         home_path = Path.home() / ".env"
-        set_key(home_path, "GITHUB_ACCESS_TOKEN", new_pat)
-        print(f"PAT saved globally in {home_path}")
+        set_key(home_path, "GITLAB_ACCESS_TOKEN", new_pat)
+        console.print(f"PAT saved globally in {home_path}")
     elif choice == "l":
         local_path = Path(".env")
-        set_key(local_path, "GITHUB_ACCESS_TOKEN", new_pat)
-        print(f"PAT saved locally in {local_path}")
+        set_key(local_path, "GITLAB_ACCESS_TOKEN", new_pat)
+        console.print(f"PAT saved locally in {local_path}")
     else:
-        print("Invalid option selected. PAT setup aborted.")
+        console.print("Invalid option selected. PAT setup aborted.")
 
 
 if __name__ == "__main__":
-    setup_github_pat()
+    setup_gitlab_pat()
```

### Comparing `git_mirror-0.3.6/git_mirror/router.py` & `git_mirror-0.3.7/git_mirror/router.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,20 +9,23 @@
 import git_mirror.manage_config as mc
 import git_mirror.manage_git as mg
 import git_mirror.manage_github as mgh
 import git_mirror.manage_gitlab as mgl
 from git_mirror.custom_types import SourceHost
 from git_mirror.manage_poetry import PoetryManager
 from git_mirror.safe_env import load_env
+from git_mirror.ui import console_with_theme
 
 load_env()
 
 # Configure logging
 LOGGER = logging.getLogger(__name__)
 
+console = console_with_theme()
+
 
 def route_simple(
     command: str,
     config_path: Optional[Path] = None,
 ):
     """
     Main function to handle clone-all or pull-all operations, with an option to include forks.
@@ -34,15 +37,15 @@
     if config_path is None:
         config_path = mc.default_config_path()
 
     if command == "init":
         config_manager = mc.ConfigManager(config_path=config_path)
         config_manager.initialize_config()
     else:
-        print(f"Unknown command: {command}")
+        console.print(f"Unknown command: {command}")
 
 
 def route_config(
     command: str,
     config_path: Optional[Path] = None,
     dry_run: bool = False,
 ):
@@ -57,15 +60,15 @@
     if config_path is None:
         config_path = mc.default_config_path()
 
     if command == "list-config":
         config_manager = mc.ConfigManager(config_path=config_path)
         config_manager.list_config()
     else:
-        print(f"Unknown command: {command}")
+        console.print(f"Unknown command: {command}")
 
 
 def route_repos(
     command: str,
     user_name: str,
     target_dir: Path,
     token: str,
@@ -74,14 +77,15 @@
     include_forks: bool,
     config_path: Optional[Path] = None,
     domain: Optional[str] = None,
     group_id: Optional[int] = None,
     logging_level: int = 1,
     dry_run: bool = False,
     template_dir: Optional[Path] = None,
+    prompt_for_changes: bool = True,
 ):
     """
     Main function to handle clone-all or pull-all operations, with an option to include forks.
 
     Args:
         command (str): The command to execute ('clone-all' or 'pull-all').
         user_name (str): The GitHub username.
@@ -92,44 +96,47 @@
         include_forks (bool): Flag to determine whether forked repositories should be included.
         config_path (Path): Path to the TOML config file.
         domain (str): The GitLab domain.
         group_id (int): The GitLab group id.
         logging_level (int): The logging level.
         dry_run (bool): Flag to determine whether the operation should be a dry run.
         template_dir (Path): The directory containing the templates to sync.
+        prompt_for_changes (bool): Flag to determine whether to prompt for changes.
     """
     if config_path is None:
         config_path = mc.default_config_path()
 
     if command == "local-changes":
         base_path = Path(target_dir).expanduser()
-        git_manager = mg.GitManager(base_path, dry_run)
+        git_manager = mg.GitManager(base_path, dry_run, prompt_for_changes=prompt_for_changes)
         git_manager.check_for_uncommitted_or_unpushed_changes()
     elif host in ("github", "gitlab", "selfhosted"):
         if host == "github":
             base_path = Path(target_dir).expanduser()
             manager: SourceHost = mgh.GithubRepoManager(
                 token,
                 base_path,
                 user_name,
                 include_private=include_private,
                 include_forks=include_forks,
                 dry_run=dry_run,
+                prompt_for_changes=prompt_for_changes,
             )
         elif host in ("gitlab", "selfhosted"):
             base_path = Path(target_dir).expanduser()
             manager = mgl.GitlabRepoManager(
                 token,
                 base_path,
                 user_name,
                 include_private=include_private,
                 include_forks=include_forks,
                 host_domain=domain or "https://gitlab.com",
                 logging_level=logging_level,
                 dry_run=dry_run,
+                prompt_for_changes=prompt_for_changes,
             )
         else:
             raise ValueError(f"Unknown host: {host}")
 
         if command == "clone-all" and host in ("gitlab", "selfhosted") and group_id is not None and group_id != 0:
             # TODO: confusion with clone all by user name and by group id.
             # If they are both filled in, then what does the user want?
@@ -139,14 +146,15 @@
                 base_path,
                 user_name,
                 include_private=include_private,
                 include_forks=include_forks,
                 host_domain=domain or "https://gitlab.com",
                 logging_level=logging_level,
                 dry_run=dry_run,
+                prompt_for_changes=prompt_for_changes,
             )
             gl_manager.clone_group(group_id)
         elif command == "clone-all":
             manager.clone_all()
         elif command == "pull-all":
             manager.pull_all()
         elif command == "not-repo":
@@ -162,57 +170,58 @@
         elif command == "show-account":
             manager.print_user_summary()
         elif command == "sync-config":
             config_manager = mc.ConfigManager(config_path=config_path)
             config_manager.load_and_sync_config(host, manager.list_repo_names())
         elif command == "cross-repo-report":
             if not template_dir:
-                print("Template directory is required for cross-repo-report")
+                console.print("Template directory is required for cross-repo-report")
                 return
             manager.cross_repo_sync_report(template_dir)
         elif command == "cross-repo-sync":
             if not template_dir:
-                print("Template directory is required for cross-repo-sync")
+                console.print("Template directory is required for cross-repo-sync")
                 return
             manager.cross_repo_sync(template_dir)
         elif command == "cross-repo-init":
             if not template_dir:
-                print("Template directory is required for cross-repo-init")
+                console.print("Template directory is required for cross-repo-init")
                 return
             manager.cross_repo_init(template_dir)
         elif command == "poetry-relock":
-            git_manager = mg.GitManager(base_path, dry_run)
+            git_manager = mg.GitManager(base_path, dry_run, prompt_for_changes=prompt_for_changes)
             poetry_manager = PoetryManager(manager)
             for repo in git_manager.local_repos_with_file_in_root("pyproject.toml"):
                 poetry_manager.update_dependencies(
                     main_branch="TODO-lookup",
                     dependency_update_branch="poetry-update",
                     reviewer="TODO-config",
                     project_id=0,  # TODO- config
                     repo_name=repo.name,  # Github only
                     user="TODO-lookup",
                 )
         else:
-            print(f"Unknown command: {command}")
+            console.print(f"Unknown command: {command}")
     else:
-        print(f"Unknown host: {host}")
+        console.print(f"Unknown host: {host}")
 
 
 def route_cross_repo(
     command: str,
     user_name: str,
     target_dir: Path,
     token: str,
     host: str,
     include_private: bool,
     include_forks: bool,
     domain: Optional[str] = None,
     logging_level: int = 1,
     dry_run: bool = False,
     template_dir: Optional[Path] = None,
+    prompt_for_changes: bool = True,
 ):
     """
     Main function to handle clone-all or pull-all operations, with an option to include forks.
 
     Args:
         command (str): The command to execute ('clone-all' or 'pull-all').
         user_name (str): The GitHub username.
@@ -223,61 +232,64 @@
         include_forks (bool): Flag to determine whether forked repositories should be included.
         config_path (Path): Path to the TOML config file.
         domain (str): The GitLab domain.
         group_id (int): The GitLab group id.
         logging_level (int): The logging level.
         dry_run (bool): Flag to determine whether the operation should be a dry run.
         template_dir (Path): The directory containing the templates to sync.
+        prompt_for_changes (bool): Flag to determine whether to prompt for changes.
     """
     if host in ("github", "gitlab", "selfhosted"):
         if host == "github":
             base_path = Path(target_dir).expanduser()
             manager: SourceHost = mgh.GithubRepoManager(
                 token,
                 base_path,
                 user_name,
                 include_private=include_private,
                 include_forks=include_forks,
                 dry_run=dry_run,
+                prompt_for_changes=prompt_for_changes,
             )
         elif host in ("gitlab", "selfhosted"):
             base_path = Path(target_dir).expanduser()
             manager = mgl.GitlabRepoManager(
                 token,
                 base_path,
                 user_name,
                 include_private=include_private,
                 include_forks=include_forks,
                 host_domain=domain or "https://gitlab.com",
                 logging_level=logging_level,
                 dry_run=dry_run,
+                prompt_for_changes=prompt_for_changes,
             )
         else:
             raise ValueError(f"Unknown host: {host}")
 
         if not template_dir:
-            print("Template directory is required for cross-repo-report")
+            console.print("Template directory is required for cross-repo-report")
             return
 
         if command == "cross-repo-report":
             manager.cross_repo_sync_report(template_dir)
         elif command == "cross-repo-sync":
             if not template_dir:
-                print("Template directory is required for cross-repo-sync")
+                console.print("Template directory is required for cross-repo-sync")
                 return
             manager.cross_repo_sync(template_dir)
         elif command == "cross-repo-init":
             if not template_dir:
-                print("Template directory is required for cross-repo-init")
+                console.print("Template directory is required for cross-repo-init")
                 return
             manager.cross_repo_init(template_dir)
         else:
-            print(f"Unknown command: {command}")
+            console.print(f"Unknown command: {command}")
     else:
-        print(f"Unknown host: {host}")
+        console.print(f"Unknown host: {host}")
 
 
 def route_pypi(
     command: str,
     user_name: str,
     target_dir: Path,
     token: str,
@@ -330,10 +342,10 @@
             )
         else:
             raise ValueError(f"Unknown host: {host}")
 
         if command == "pypi-status":
             manager.check_pypi_publish_status(pypi_owner_name=pypi_owner_name)
         else:
-            print(f"Unknown command: {command}")
+            console.print(f"Unknown command: {command}")
     else:
-        print(f"Unknown host: {host}")
+        console.print(f"Unknown host: {host}")
```

### Comparing `git_mirror-0.3.6/git_mirror/version_check.py` & `git_mirror-0.3.7/git_mirror/version_check.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import httpx
 from packaging import version
 from packaging.version import Version
 
 # Import the current version of your package
 from git_mirror.__about__ import __version__
+from git_mirror.ui import console_with_theme
+
+console = console_with_theme()
 
 
 def call_pypi_with_version_check(package_name: str, current_version: str) -> tuple[bool, Version]:
     """
     Synchronously checks if the latest version of the package on PyPI is greater than the current version.
 
     Args:
@@ -28,14 +31,14 @@
 
 # Example usage
 def display_version_check_message() -> None:
     try:
         package_name = "git_mirror"
         available, new_version = call_pypi_with_version_check(package_name, __version__)
         if available:
-            print(f"A newer version of {package_name} is available on PyPI. Upgrade to {new_version}.")
+            console.print(f"A newer version of {package_name} is available on PyPI. Upgrade to {new_version}.")
     except httpx.HTTPError as e:
-        print(f"An error occurred while checking the latest version: {e}")
+        console.print(f"An error occurred while checking the latest version: {e}", style="danger")
 
 
 if __name__ == "__main__":
     display_version_check_message()
```

### Comparing `git_mirror-0.3.6/pyproject.toml` & `git_mirror-0.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "git_mirror"
-version = "0.3.6"
+version = "0.3.7"
 description = "Make your local git repos look like github or gitlab. See readme for how this differs from the many other multi-repo tools."
 authors = ["Matthew Martin <matthewdeanmartin@gmail.com>"]
 keywords = ["git", "gitlab", "github", "polyrepo" ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
@@ -45,21 +45,24 @@
 [tool.poetry.dependencies]
 python = ">=3.9"
 
 # core
 python-dotenv = ">=1.0.1, <2"
 
 # ui
-termcolor = ">=2.4.0, <3"
-prettytable = "3.9.0, <4"
-colorlog = ">=6.8.0, <7"
 rich = ">=13.7.0, <14"
 inquirer = ">=3.2.3, <4"
+
+# one table uses this...
+prettytable = "3.9.0, <4"
 colorama = ">=0.4.6, <1"
 
+# ui for verbose loggging
+colorlog = ">=6.8.0, <7"
+
 # git
 PyGithub=">=2.2.0"
 python-gitlab = ">=4.4.0"
 # needs git >=1.7.*
 GitPython= ">=3.1.42"
 
 # api calls
```

### Comparing `git_mirror-0.3.6/PKG-INFO` & `git_mirror-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git_mirror
-Version: 0.3.6
+Version: 0.3.7
 Summary: Make your local git repos look like github or gitlab. See readme for how this differs from the many other multi-repo tools.
 Home-page: https://github.com/matthewdeanmartin/git_mirror
 License: MIT
 Keywords: git,gitlab,github,polyrepo
 Author: Matthew Martin
 Author-email: matthewdeanmartin@gmail.com
 Requires-Python: >=3.9
@@ -27,15 +27,14 @@
 Requires-Dist: httpx (>=0.26.0,<1)
 Requires-Dist: inquirer (>=3.2.3,<4)
 Requires-Dist: prettytable (==3.9.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2)
 Requires-Dist: python-gitlab (>=4.4.0)
 Requires-Dist: requests-cache (>=1.2.0,<2)
 Requires-Dist: rich (>=13.7.0,<14)
-Requires-Dist: termcolor (>=2.4.0,<3)
 Requires-Dist: toml (>=0.10.2,<1)
 Requires-Dist: tomlkit (>=0.12.3,<1)
 Project-URL: Bug Tracker, https://github.com/matthewdeanmartin/git_mirror/issues
 Project-URL: Change Log, https://github.com/matthewdeanmartin/git_mirror/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://matthewdeanmartin.github.io/git_mirror/git_mirror/index.html
 Project-URL: Repository, https://github.com/matthewdeanmartin/git_mirror
 Description-Content-Type: text/markdown
```

