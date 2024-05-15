# Comparing `tmp/uvx-2.0.8.tar.gz` & `tmp/uvx-2.1.0.tar.gz`

## Comparing `uvx-2.0.8.tar` & `uvx-2.1.0.tar`

### file list

```diff
@@ -1,38 +1,42 @@
--rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 uvx-2.0.8/Cargo.toml
--rw-rw-r--   0     1000     1000       77 2024-04-15 17:07:31.000000 uvx-2.0.8/.cargo/config.toml
--rw-rw-r--   0     1000     1000      686 2024-04-11 15:03:17.000000 uvx-2.0.8/.gitignore
--rw-rw-r--   0     1000     1000      933 2024-05-01 11:28:10.000000 uvx-2.0.8/CHANGELOG.md
--rw-rw-r--   0     1000     1000    92159 2024-05-01 11:27:13.000000 uvx-2.0.8/Cargo.lock
--rw-rw-r--   0     1000     1000     2203 2024-04-26 19:03:51.000000 uvx-2.0.8/README.md
--rwxrwxr-x   0     1000     1000      251 2024-05-01 11:18:56.000000 uvx-2.0.8/build.sh
--rw-rw-r--   0     1000     1000      106 2024-04-15 17:06:44.000000 uvx-2.0.8/rustfmt.toml
--rw-rw-r--   0     1000     1000     1821 2024-04-24 20:50:38.000000 uvx-2.0.8/src/animate.rs
--rw-rw-r--   0     1000     1000     9727 2024-04-24 20:50:21.000000 uvx-2.0.8/src/cli.rs
--rw-rw-r--   0     1000     1000     2314 2024-04-26 20:57:40.000000 uvx-2.0.8/src/cmd.rs
--rw-rw-r--   0     1000     1000      618 2024-04-24 20:49:18.000000 uvx-2.0.8/src/commands/completions.rs
--rw-rw-r--   0     1000     1000     2262 2024-04-29 13:40:19.000000 uvx-2.0.8/src/commands/ensurepath.rs
--rw-rw-r--   0     1000     1000     1617 2024-04-24 20:48:26.000000 uvx-2.0.8/src/commands/inject.rs
--rw-rw-r--   0     1000     1000     5100 2024-04-29 13:41:31.000000 uvx-2.0.8/src/commands/install.rs
--rw-rw-r--   0     1000     1000     2511 2024-04-24 20:45:17.000000 uvx-2.0.8/src/commands/list.rs
--rw-rw-r--   0     1000     1000      312 2024-04-15 19:40:37.000000 uvx-2.0.8/src/commands/mod.rs
--rw-rw-r--   0     1000     1000     2200 2024-04-24 20:43:02.000000 uvx-2.0.8/src/commands/reinstall.rs
--rw-rw-r--   0     1000     1000     1346 2024-04-24 20:41:37.000000 uvx-2.0.8/src/commands/reinstall_all.rs
--rw-rw-r--   0     1000     1000     4039 2024-04-24 20:42:18.000000 uvx-2.0.8/src/commands/run.rs
--rw-rw-r--   0     1000     1000      621 2024-04-24 20:39:59.000000 uvx-2.0.8/src/commands/runpip.rs
--rw-rw-r--   0     1000     1000     1195 2024-04-24 20:39:49.000000 uvx-2.0.8/src/commands/runpython.rs
--rw-rw-r--   0     1000     1000      527 2024-04-24 20:39:25.000000 uvx-2.0.8/src/commands/runuv.rs
--rw-rw-r--   0     1000     1000     3192 2024-04-26 20:57:17.000000 uvx-2.0.8/src/commands/self_update.rs
--rw-rw-r--   0     1000     1000     1631 2024-04-24 20:35:19.000000 uvx-2.0.8/src/commands/uninject.rs
--rw-rw-r--   0     1000     1000     2019 2024-04-24 20:34:30.000000 uvx-2.0.8/src/commands/uninstall.rs
--rw-rw-r--   0     1000     1000      948 2024-04-24 20:34:02.000000 uvx-2.0.8/src/commands/uninstall_all.rs
--rw-rw-r--   0     1000     1000     4054 2024-04-24 20:33:47.000000 uvx-2.0.8/src/commands/upgrade.rs
--rw-rw-r--   0     1000     1000     1021 2024-04-24 20:32:19.000000 uvx-2.0.8/src/commands/upgrade_all.rs
--rw-rw-r--   0     1000     1000      962 2024-04-24 20:32:00.000000 uvx-2.0.8/src/helpers.rs
--rw-rw-r--   0     1000     1000     1026 2024-04-24 20:02:25.000000 uvx-2.0.8/src/main.rs
--rw-rw-r--   0     1000     1000     8649 2024-04-29 13:41:09.000000 uvx-2.0.8/src/metadata.rs
--rw-rw-r--   0     1000     1000     4477 2024-04-24 20:41:56.000000 uvx-2.0.8/src/pip.rs
--rw-rw-r--   0     1000     1000     3722 2024-04-29 13:40:53.000000 uvx-2.0.8/src/symlinks.rs
--rw-rw-r--   0     1000     1000     3768 2024-04-24 20:51:25.000000 uvx-2.0.8/src/uv.rs
--rw-rw-r--   0     1000     1000     2352 2024-04-24 20:51:25.000000 uvx-2.0.8/src/venv.rs
--rw-rw-r--   0     1000     1000     1003 2024-05-01 11:26:34.000000 uvx-2.0.8/pyproject.toml
--rw-r--r--   0        0        0     2773 1970-01-01 00:00:00.000000 uvx-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 uvx-2.1.0/Cargo.toml
+-rw-rw-r--   0     1000     1000       77 2024-04-15 17:07:31.000000 uvx-2.1.0/.cargo/config.toml
+-rw-rw-r--   0     1000     1000      686 2024-04-11 15:03:17.000000 uvx-2.1.0/.gitignore
+-rw-rw-r--   0     1000     1000     1583 2024-05-15 09:28:05.000000 uvx-2.1.0/CHANGELOG.md
+-rw-rw-r--   0     1000     1000    92159 2024-05-15 09:19:02.000000 uvx-2.1.0/Cargo.lock
+-rw-rw-r--   0     1000     1000     2456 2024-05-15 08:49:40.000000 uvx-2.1.0/README.md
+-rwxrwxr-x   0     1000     1000      251 2024-05-01 11:18:56.000000 uvx-2.1.0/build.sh
+-rw-rw-r--   0     1000     1000      106 2024-04-15 17:06:44.000000 uvx-2.1.0/rustfmt.toml
+-rw-rw-r--   0     1000     1000     1821 2024-05-10 16:04:44.000000 uvx-2.1.0/src/animate.rs
+-rw-rw-r--   0     1000     1000    11134 2024-05-15 08:30:11.000000 uvx-2.1.0/src/cli.rs
+-rw-rw-r--   0     1000     1000     3194 2024-05-14 19:37:08.000000 uvx-2.1.0/src/cmd.rs
+-rw-rw-r--   0     1000     1000     1346 2024-05-15 07:59:15.000000 uvx-2.1.0/src/commands/activate.rs
+-rw-rw-r--   0     1000     1000      899 2024-05-14 19:03:10.000000 uvx-2.1.0/src/commands/completions.rs
+-rw-rw-r--   0     1000     1000     1156 2024-05-15 09:17:21.000000 uvx-2.1.0/src/commands/create.rs
+-rw-rw-r--   0     1000     1000     2462 2024-05-14 19:10:06.000000 uvx-2.1.0/src/commands/ensurepath.rs
+-rw-rw-r--   0     1000     1000     1617 2024-04-24 20:48:26.000000 uvx-2.1.0/src/commands/inject.rs
+-rw-rw-r--   0     1000     1000     5100 2024-04-29 13:41:31.000000 uvx-2.1.0/src/commands/install.rs
+-rw-rw-r--   0     1000     1000     2511 2024-04-24 20:45:17.000000 uvx-2.1.0/src/commands/list.rs
+-rw-rw-r--   0     1000     1000      362 2024-05-15 08:03:43.000000 uvx-2.1.0/src/commands/mod.rs
+-rw-rw-r--   0     1000     1000     2489 2024-05-15 09:17:35.000000 uvx-2.1.0/src/commands/reinstall.rs
+-rw-rw-r--   0     1000     1000     1346 2024-04-24 20:41:37.000000 uvx-2.1.0/src/commands/reinstall_all.rs
+-rw-rw-r--   0     1000     1000     4039 2024-04-24 20:42:18.000000 uvx-2.1.0/src/commands/run.rs
+-rw-rw-r--   0     1000     1000      621 2024-04-24 20:39:59.000000 uvx-2.1.0/src/commands/runpip.rs
+-rw-rw-r--   0     1000     1000     1195 2024-04-24 20:39:49.000000 uvx-2.1.0/src/commands/runpython.rs
+-rw-rw-r--   0     1000     1000      527 2024-04-24 20:39:25.000000 uvx-2.1.0/src/commands/runuv.rs
+-rw-rw-r--   0     1000     1000     3192 2024-04-26 20:57:17.000000 uvx-2.1.0/src/commands/self_update.rs
+-rw-rw-r--   0     1000     1000     3763 2024-05-15 08:51:29.000000 uvx-2.1.0/src/commands/setup.rs
+-rw-rw-r--   0     1000     1000     1631 2024-04-24 20:35:19.000000 uvx-2.1.0/src/commands/uninject.rs
+-rw-rw-r--   0     1000     1000     2019 2024-04-24 20:34:30.000000 uvx-2.1.0/src/commands/uninstall.rs
+-rw-rw-r--   0     1000     1000      948 2024-04-24 20:34:02.000000 uvx-2.1.0/src/commands/uninstall_all.rs
+-rw-rw-r--   0     1000     1000     4054 2024-04-24 20:33:47.000000 uvx-2.1.0/src/commands/upgrade.rs
+-rw-rw-r--   0     1000     1000     1021 2024-04-24 20:32:19.000000 uvx-2.1.0/src/commands/upgrade_all.rs
+-rw-rw-r--   0     1000     1000      962 2024-04-24 20:32:00.000000 uvx-2.1.0/src/helpers.rs
+-rw-rw-r--   0     1000     1000     1989 2024-05-14 19:10:14.000000 uvx-2.1.0/src/main.rs
+-rw-rw-r--   0     1000     1000     9823 2024-05-15 09:06:40.000000 uvx-2.1.0/src/metadata.rs
+-rw-rw-r--   0     1000     1000     4477 2024-04-24 20:41:56.000000 uvx-2.1.0/src/pip.rs
+-rw-rw-r--   0     1000     1000      487 2024-05-13 18:28:56.000000 uvx-2.1.0/src/shell/activate.sh
+-rw-rw-r--   0     1000     1000     3722 2024-04-29 13:40:53.000000 uvx-2.1.0/src/symlinks.rs
+-rw-rw-r--   0     1000     1000     3768 2024-04-24 20:51:25.000000 uvx-2.1.0/src/uv.rs
+-rw-rw-r--   0     1000     1000     2819 2024-05-15 08:51:43.000000 uvx-2.1.0/src/venv.rs
+-rw-rw-r--   0     1000     1000     1003 2024-05-01 11:26:34.000000 uvx-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3026 1970-01-01 00:00:00.000000 uvx-2.1.0/PKG-INFO
```

### Comparing `uvx-2.0.8/Cargo.toml` & `uvx-2.1.0/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "uvx"
-version = "2.0.8"
+version = "2.1.0"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 # [lib]
 # name = "uvx"
 # crate-type = ["cdylib"]
```

### Comparing `uvx-2.0.8/.gitignore` & `uvx-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `uvx-2.0.8/Cargo.lock` & `uvx-2.1.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -3321,15 +3321,15 @@
  "once_cell",
  "owo-colors",
  "rustc-hash",
 ]
 
 [[package]]
 name = "uvx"
-version = "2.0.8"
+version = "2.1.0"
 dependencies = [
  "anstyle",
  "chrono",
  "clap",
  "clap_complete",
  "configparser",
  "directories",
```

### Comparing `uvx-2.0.8/README.md` & `uvx-2.1.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -9,22 +9,24 @@
 
 1. Install via pip (or alternatives):
     ```bash
     pip install uvx  # or `uv`, `pipx`
     ```
 
 2. Optional (for bash users):
-    - Ensure that `~/.local/bin` is in your PATH:
-        ```bash
-        uvx ensurepath
-        ```
-    - Enable tab completion for `uvx`:
-        ```bash
-        uvx completions --install
-        ```
+      ```bash
+      uvx setup
+      ```
+
+   This installs the following features:
+
+- Ensures `~/.local/bin/` is added to your PATH, so commands can be found (unless `--skip-ensurepath`). Can also be
+  activated via `uvx ensurepath`
+- Enables tab completion for `uvx` (unless `--skip-completions`). Can also be enabled via `uvx completions --install`.
+- Enables `uvx activate` (unless `--skip-activate`) to activate uvx-managed virtualenvs from your shell
 
 ## Usage
 
 ```bash
 uvx
 ```
```

### Comparing `uvx-2.0.8/src/animate.rs` & `uvx-2.1.0/src/animate.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.8/src/cli.rs` & `uvx-2.1.0/src/cli.rs`

 * *Files 14% similar despite different names*

```diff
@@ -59,14 +59,30 @@
 //     }
 // }
 
 const PYTHON_HELP_TEXT: &str =
     "Python version or executable to use, e.g. `3.12`, `python3.12`, `/usr/bin/python3.12`";
 
 #[derive(Debug, Parser)]
+pub struct SetupOptions {
+    #[clap(long, help = "Don't update $PATH in .bashrc")]
+    pub skip_ensurepath: bool,
+    #[clap(long, help = "Don't enable completions via .bashrc")]
+    pub skip_completions: bool,
+    #[clap(long, help = "Don't enable `uvx activate` via .bashrc")]
+    pub skip_activate: bool,
+    #[clap(
+        short,
+        long,
+        help = "Setup features without checking previous installation."
+    )]
+    pub force: bool,
+}
+
+#[derive(Debug, Parser)]
 pub struct ListOptions {
     #[clap(short, long, help = "Short output", conflicts_with_all = ["verbose"])]
     pub short: bool,
     #[clap(short, long, help = "Verbose output", conflicts_with_all = ["short", "json"])]
     pub verbose: bool,
     #[clap(short, long, help = "Output in JSON format", conflicts_with_all = ["verbose"])]
     pub json: bool,
@@ -88,14 +104,30 @@
     #[clap(long, help = PYTHON_HELP_TEXT)]
     pub python: Option<String>,
     #[clap(long, short, help = "Editable Install")]
     pub editable: bool,
 }
 
 #[derive(Debug, Parser)]
+pub struct CreateOptions {
+    pub venv_name: String,
+    #[clap(long, help = PYTHON_HELP_TEXT)]
+    pub python: Option<String>,
+    #[clap(long, help = "Skip installing basic packages like 'pip'")]
+    pub no_seed: bool,
+    #[clap(short, long, help = "Overwrite existing venv with conflicting name")]
+    pub force: bool,
+}
+
+#[derive(Debug, Parser)]
+pub struct ActivateOptions {
+    pub venv_name: String,
+}
+
+#[derive(Debug, Parser)]
 pub struct UpgradeOptions {
     pub package_name: String,
     #[clap(short = 'f', long, help = "Ignore previous version constraint")]
     pub force: bool,
     #[clap(long, help = "Don't also upgrade injected packages")]
     pub skip_injected: bool,
     #[clap(long, help = "Run without `uv` cache")]
@@ -234,25 +266,29 @@
     #[clap(long, short, help = "Add to ~/.bashrc")]
     pub install: bool,
     // todo: support others than bash
 }
 
 #[derive(Subcommand, Debug)]
 pub enum Commands {
-    #[clap(about = "Use --install to install the autocomplete script (bash).")]
-    Completions(CompletionsOptions),
+    #[clap(about = "Setup additional (bash-specific) functionality.")]
+    Setup(SetupOptions),
     #[clap(about = "List packages and apps installed with uvx.")]
     List(ListOptions),
     #[clap(about = "Install a package (by pip name).")]
     Install(InstallOptions),
+    #[clap(about = "Create a new (empty) virtualenv")]
+    Create(CreateOptions),
+    #[clap(about = "Activate an uvx-managed virtualenv (bash only)")]
+    Activate(ActivateOptions),
     #[clap(about = "Upgrade a package.")]
     Upgrade(UpgradeOptions),
     #[clap(about = "Upgrade all uvx-installed packages.")]
     UpgradeAll(UpgradeAllOptions),
-    #[clap(about = "Uninstall a package (by pip name).")]
+    #[clap(aliases = &["delete", "remove"], about = "Uninstall a package (by pip name).")]
     Uninstall(UninstallOptions),
     #[clap(about = "Uninstall all uvx-installed packages.")]
     UninstallAll(UninstallAllOptions),
     #[clap(
         about = "Uninstall a package (by pip name) and re-install from the original spec (unless a new spec is supplied)."
     )]
     Reinstall(ReinstallOptions),
@@ -270,34 +306,39 @@
     Runpip(RunpipOptions),
     #[clap(about = "Run 'python' in the right venv.")]
     Runpython(RunpythonOptions),
     #[clap(
         about = "Update ~/.bashrc with a PATH that includes the local bin directory that uvx uses."
     )]
     Ensurepath(EnsurepathOptions),
+    #[clap(about = "Use --install to install the autocomplete script (bash).")]
+    Completions(CompletionsOptions),
     #[clap(about = "Update the current installation of uvx (and optionally uv).")]
     SelfUpdate(SelfUpdateOptions),
 }
 
 impl Process for Commands {
     async fn process(self) -> Result<i32, String> {
         match self {
             Commands::List(opts) => opts.process().await,
             Commands::Install(opts) => opts.process().await,
             Commands::Upgrade(opts) => opts.process().await,
             Commands::Uninstall(opts) => opts.process().await,
             Commands::Reinstall(opts) => opts.process().await,
             Commands::Inject(opts) => opts.process().await,
+            Commands::Activate(opts) => opts.process().await,
             Commands::UpgradeAll(opts) => opts.process().await,
             Commands::Runuv(opts) => opts.process().await,
             Commands::Runpip(opts) => opts.process().await,
             Commands::Runpython(opts) => opts.process().await,
             Commands::Ensurepath(opts) => opts.process().await,
             Commands::SelfUpdate(opts) => opts.process().await,
             Commands::UninstallAll(opts) => opts.process().await,
             Commands::ReinstallAll(opts) => opts.process().await,
             Commands::Uninject(opts) => opts.process().await,
             Commands::Completions(opts) => opts.process().await,
             Commands::Run(opts) => opts.process().await,
+            Commands::Setup(opts) => opts.process().await,
+            Commands::Create(opts) => opts.process().await,
         }
     }
 }
```

### Comparing `uvx-2.0.8/src/commands/ensurepath.rs` & `uvx-2.1.0/src/commands/ensurepath.rs`

 * *Files 7% similar despite different names*

```diff
@@ -76,13 +76,19 @@
 
     add_to_bashrc(&format!("export PATH=\"$PATH:{}\"", bin_dir), true).await?;
 
     println!("Added '{}' to ~/.bashrc", bin_dir.green());
     Ok(())
 }
 
+pub async fn ensure_path_generate() -> String {
+    let bin_path = ensure_bin_dir().await;
+    let bin_dir = bin_path.to_str().unwrap_or_default();
+    format!("export PATH=\"$PATH:{}\"", bin_dir)
+}
+
 impl Process for EnsurepathOptions {
     async fn process(self) -> Result<i32, String> {
         ensure_path(self.force).await?;
         Ok(0)
     }
 }
```

### Comparing `uvx-2.0.8/src/commands/inject.rs` & `uvx-2.1.0/src/commands/inject.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.8/src/commands/install.rs` & `uvx-2.1.0/src/commands/install.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.8/src/commands/list.rs` & `uvx-2.1.0/src/commands/list.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.8/src/commands/reinstall.rs` & `uvx-2.1.0/src/commands/reinstall.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 use owo_colors::OwoColorize;
 
+use crate::commands::create::create;
 use crate::{
     cli::{Process, ReinstallOptions},
     commands::{install::install_package, uninstall::uninstall_package},
     metadata::{venv_path, Metadata},
     pip::parse_requirement,
     uv::ExtractInfo,
 };
@@ -51,24 +52,34 @@
 
     let inject = if with_injected {
         current_metadata.vec_injected()
     } else {
         Vec::new()
     };
 
-    install_package(
-        new_install_spec,
-        None,
-        python,
-        force,
-        inject,
-        no_cache,
-        editable,
-    )
-    .await
+    if new_install_spec.is_empty() {
+        create(
+            &current_metadata.name,
+            python,
+            true, // force seed for now
+            force,
+        )
+        .await
+    } else {
+        install_package(
+            new_install_spec,
+            None,
+            python,
+            force,
+            inject,
+            no_cache,
+            editable,
+        )
+        .await
+    }
 }
 
 impl Process for ReinstallOptions {
     async fn process(self) -> Result<i32, String> {
         match reinstall(
             &self.package,
             self.python.as_ref(),
```

### Comparing `uvx-2.0.8/src/commands/reinstall_all.rs` & `uvx-2.1.0/src/commands/reinstall_all.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.8/src/commands/run.rs` & `uvx-2.1.0/src/commands/run.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.8/src/commands/runpip.rs` & `uvx-2.1.0/src/commands/runpip.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.8/src/commands/runpython.rs` & `uvx-2.1.0/src/commands/runpython.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.8/src/commands/runuv.rs` & `uvx-2.1.0/src/commands/runuv.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.8/src/commands/self_update.rs` & `uvx-2.1.0/src/commands/self_update.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.8/src/commands/uninject.rs` & `uvx-2.1.0/src/commands/uninject.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.8/src/commands/uninstall.rs` & `uvx-2.1.0/src/commands/uninstall.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.8/src/commands/uninstall_all.rs` & `uvx-2.1.0/src/commands/uninstall_all.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.8/src/commands/upgrade.rs` & `uvx-2.1.0/src/commands/upgrade.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.8/src/commands/upgrade_all.rs` & `uvx-2.1.0/src/commands/upgrade_all.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.8/src/helpers.rs` & `uvx-2.1.0/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.8/src/metadata.rs` & `uvx-2.1.0/src/metadata.rs`

 * *Files 10% similar despite different names*

```diff
@@ -94,48 +94,57 @@
 
         empty.installed_version = uv_get_installed_version(&req.name, None).unwrap_or_default();
 
         empty.fill(None);
         empty
     }
 
+    pub fn fill_python(
+        &mut self,
+        venv: &PythonEnvironment,
+    ) {
+        let python_info = venv.interpreter().markers();
+
+        if self.python.is_empty() {
+            self.python = format!(
+                "{} {}",
+                python_info.platform_python_implementation, python_info.python_full_version
+            )
+        }
+
+        if self.python_raw.is_empty() {
+            self.python_raw = venv.stdlib_as_string();
+        }
+    }
+
     /// try to guess/deduce some values
     pub fn fill(
         &mut self,
         maybe_venv: Option<&PythonEnvironment>,
     ) -> Option<()> {
         let _v: PythonEnvironment;
 
+        if self.install_spec.is_empty() {
+            self.install_spec = String::from(&self.name);
+        }
+
         let venv = match maybe_venv {
             Some(v) => v,
             None => match uv_venv(None) {
                 Some(v) => {
+                    // black magic fuckery to
+                    // get a reference to the currently active venv
                     _v = v;
                     &_v
                 },
                 None => return None,
             },
         };
 
-        let python_info = venv.interpreter().markers();
-
-        if self.install_spec.is_empty() {
-            self.install_spec = String::from(&self.name);
-        }
-
-        if self.python.is_empty() {
-            self.python = format!(
-                "{} {}",
-                python_info.platform_python_implementation, python_info.python_full_version
-            )
-        }
-
-        if self.python_raw.is_empty() {
-            self.python_raw = venv.stdlib_as_string();
-        }
+        self.fill_python(venv);
 
         Some(())
     }
 
     pub async fn for_dir(
         dirname: &Path,
         recheck_scripts: bool,
@@ -271,47 +280,75 @@
 fn add_header(buf: &mut Vec<u8>) {
     let mut new_buf = Vec::with_capacity(MAGIC_HEADER.len() + buf.len());
     new_buf.extend_from_slice(MAGIC_HEADER);
     new_buf.append(buf);
     *buf = new_buf;
 }
 
-pub async fn load_metadata(
+/// 'buf' is required to hold the data internally, with the same lifetime as the unserialized object
+/// Mimimal example:
+///
+///
+///     pub async fn load_setup_metadata(filename: &Path) -> Result<SetupMetadata, String> {
+///       let mut buf = Vec::new(); // allocate memory for the object
+///
+///       // Open the msgpack file
+///       let metadata: SetupMetadata = load_generic_msgpack(filename, &mut buf).await?;
+///
+///       Ok(metadata)
+///     }
+pub async fn load_generic_msgpack<'a, T: serde::Deserialize<'a>>(
     filename: &Path,
-    recheck_scripts: bool,
-) -> Result<Metadata, String> {
+    buf: &'a mut Vec<u8>,
+) -> Result<T, String> {
     // Open the msgpack file
     let mut file = File::open(filename).await.map_err_to_string()?;
 
-    let mut buf = Vec::new();
-    file.read_to_end(&mut buf).await.map_err_to_string()?;
-
-    strip_header(&mut buf);
+    // for some reason (I guess the lifetime), buf can just be passed around now?
+    file.read_to_end(buf).await.map_err_to_string()?;
+    strip_header(buf);
 
     // Read the contents of the file into a Metadata struct
-    let mut metadata: Metadata = rmp_serde::decode::from_slice(&buf[..]).map_err_to_string()?;
+    let metadata: T = rmp_serde::decode::from_slice(&buf[..]).map_err_to_string()?;
+
+    Ok(metadata)
+}
 
+pub async fn load_metadata(
+    filename: &Path,
+    recheck_scripts: bool,
+) -> Result<Metadata, String> {
+    let mut buf = Vec::new();
+
+    let mut metadata: Metadata = load_generic_msgpack(filename, &mut buf).await?;
     if recheck_scripts {
         if let Some(folder) = filename.parent() {
             metadata.check_scripts(folder).await
         }
     }
 
     Ok(metadata)
 }
 
-pub async fn store_metadata(
+pub async fn store_generic_msgpack<T: serde::Serialize>(
     filename: &Path,
-    metadata: &Metadata,
+    metadata: &T,
 ) -> Result<(), String> {
     // Open the msgpack file
     let mut file = File::create(filename).await.map_err_to_string()?;
 
     // Read the contents of the file into a Metadata struct
     let mut bytes = rmp_serde::encode::to_vec(metadata).map_err_to_string()?;
 
     add_header(&mut bytes);
 
     file.write_all(&bytes).await.map_err_to_string()?;
 
     Ok(())
 }
+
+pub async fn store_metadata(
+    filename: &Path,
+    metadata: &Metadata,
+) -> Result<(), String> {
+    store_generic_msgpack(filename, metadata).await
+}
```

### Comparing `uvx-2.0.8/src/pip.rs` & `uvx-2.1.0/src/pip.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.8/src/symlinks.rs` & `uvx-2.1.0/src/symlinks.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.8/src/uv.rs` & `uvx-2.1.0/src/uv.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.8/src/venv.rs` & `uvx-2.1.0/src/venv.rs`

 * *Files 9% similar despite different names*

```diff
@@ -4,56 +4,74 @@
 use crate::uv::{uv, uv_venv};
 use owo_colors::OwoColorize;
 use pep508_rs::{PackageName, Requirement};
 use std::path::{Path, PathBuf};
 
 use uv_interpreter::PythonEnvironment;
 
-pub async fn create_venv(
-    package_name: &PackageName,
+pub async fn create_venv_raw(
+    venv_path: &Path,
     python: Option<&String>,
     force: bool,
     with_pip: bool,
-    custom_prefix: Option<String>,
-) -> Result<PathBuf, String> {
-    let venv_path = match custom_prefix {
-        None => venv_path(package_name.as_ref()),
-        Some(prefix) => PathBuf::from(format!("{}{}", prefix, package_name)),
-    };
-
+) -> Result<(), String> {
     if !force && venv_path.exists() {
         return Err(
-            format!("'{}' is already installed.\nUse '{}' to update existing tools or pass '{}' to this command to ignore this message.", 
-            &package_name.to_string().green(), "uvx upgrade".green(), "--force".green())
+            format!("'{}' is already installed.\nUse '{}' to update existing tools or pass '{}' to this command to ignore this message.",
+                    &venv_path.to_str().unwrap_or_default().green(), "uvx upgrade".green(), "--force".green())
         );
     }
 
     let mut args: Vec<&str> = vec!["venv", venv_path.to_str().unwrap_or_default()];
 
-    // if let Some(py) = python {
     if let Some(py) = python {
         args.push("--python");
         args.push(py);
     }
     if with_pip {
         args.push("--seed");
     }
 
     uv(args).await?;
 
+    Ok(())
+}
+
+pub async fn create_venv(
+    package_name: &PackageName,
+    python: Option<&String>,
+    force: bool,
+    with_pip: bool,
+    custom_prefix: Option<String>,
+) -> Result<PathBuf, String> {
+    let venv_path = match custom_prefix {
+        None => venv_path(package_name.as_ref()),
+        Some(prefix) => PathBuf::from(format!("{}{}", prefix, package_name)),
+    };
+
+    create_venv_raw(&venv_path, python, force, with_pip).await?;
+
     Ok(venv_path)
 }
 
 pub async fn activate_venv(venv: &Path) -> Result<PythonEnvironment, String> {
     let venv_str = venv.to_str().unwrap_or_default();
     std::env::set_var("VIRTUAL_ENV", venv_str);
 
     uv_venv(None).ok_or_else(|| format!("Could not properly activate venv '{}'!", venv_str))
 }
 
+#[allow(dead_code)]
+pub async fn find_venv(install_spec: &str) -> Option<PathBuf> {
+    let (requirement, _) = parse_requirement(install_spec).await.ok()?;
+    let requirement_name = requirement.name.to_string();
+
+    Some(venv_path(&requirement_name))
+}
+
 pub async fn setup_environ_from_requirement(
     install_spec: &str
 ) -> Result<(Requirement, PythonEnvironment), String> {
     let (requirement, _) = parse_requirement(install_spec).await?;
     let requirement_name = requirement.name.to_string();
     let venv_dir = venv_path(&requirement_name);
     if !venv_dir.exists() {
```

### Comparing `uvx-2.0.8/pyproject.toml` & `uvx-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `uvx-2.0.8/PKG-INFO` & `uvx-2.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: uvx
-Version: 2.0.8
+Version: 2.1.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 4 - Beta
 Requires-Dist: uv
 Requires-Dist: pip
@@ -26,22 +26,24 @@
 
 1. Install via pip (or alternatives):
     ```bash
     pip install uvx  # or `uv`, `pipx`
     ```
 
 2. Optional (for bash users):
-    - Ensure that `~/.local/bin` is in your PATH:
-        ```bash
-        uvx ensurepath
-        ```
-    - Enable tab completion for `uvx`:
-        ```bash
-        uvx completions --install
-        ```
+      ```bash
+      uvx setup
+      ```
+
+   This installs the following features:
+
+- Ensures `~/.local/bin/` is added to your PATH, so commands can be found (unless `--skip-ensurepath`). Can also be
+  activated via `uvx ensurepath`
+- Enables tab completion for `uvx` (unless `--skip-completions`). Can also be enabled via `uvx completions --install`.
+- Enables `uvx activate` (unless `--skip-activate`) to activate uvx-managed virtualenvs from your shell
 
 ## Usage
 
 ```bash
 uvx
 ```
```

